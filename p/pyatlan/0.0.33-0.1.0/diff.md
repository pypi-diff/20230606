# Comparing `tmp/pyatlan-0.0.33.tar.gz` & `tmp/pyatlan-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatlan-0.0.33.tar", last modified: Wed May 24 15:25:52 2023, max compression
+gzip compressed data, was "pyatlan-0.1.0.tar", last modified: Tue Jun  6 15:55:49 2023, max compression
```

## Comparing `pyatlan-0.0.33.tar` & `pyatlan-0.1.0.tar`

### file list

```diff
@@ -1,75 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:25:52.332696 pyatlan-0.0.33/
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-05-24 15:25:40.000000 pyatlan-0.0.33/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-24 15:25:40.000000 pyatlan-0.0.33/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-24 15:25:40.000000 pyatlan-0.0.33/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-24 15:25:52.332696 pyatlan-0.0.33/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-24 15:25:40.000000 pyatlan-0.0.33/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:25:52.324695 pyatlan-0.0.33/pyatlan/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:25:52.324695 pyatlan-0.0.33/pyatlan/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/cache/classification_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    11601 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/cache/custom_metadata_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/cache/enum_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/cache/group_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/cache/role_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/cache/user_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:25:52.324695 pyatlan-0.0.33/pyatlan/client/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40525 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/client/atlan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:25:52.324695 pyatlan-0.0.33/pyatlan/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/generator/generate_from_typdefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:25:52.324695 pyatlan-0.0.33/pyatlan/generator/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/generator/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:25:52.328695 pyatlan-0.0.33/pyatlan/model/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   828487 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/model/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/model/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/model/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/model/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/model/lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/model/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/model/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    59796 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/model/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/model/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24322 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/model/typedef.py
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 15:25:40.000000 pyatlan-0.0.33/pyatlan/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:25:52.324695 pyatlan-0.0.33/pyatlan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-24 15:25:52.000000 pyatlan-0.0.33/pyatlan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-24 15:25:52.000000 pyatlan-0.0.33/pyatlan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:25:52.000000 pyatlan-0.0.33/pyatlan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:25:52.000000 pyatlan-0.0.33/pyatlan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-24 15:25:52.000000 pyatlan-0.0.33/pyatlan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-24 15:25:52.000000 pyatlan-0.0.33/pyatlan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 15:25:52.332696 pyatlan-0.0.33/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-24 15:25:40.000000 pyatlan-0.0.33/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:25:52.328695 pyatlan-0.0.33/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:25:52.328695 pyatlan-0.0.33/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/integration/admin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/integration/classification_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/integration/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    37526 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/integration/custom_metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/integration/glossary_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    34056 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/integration/test_entity_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/integration/test_index_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:25:52.332696 pyatlan-0.0.33/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/unit/test_classification_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/unit/test_glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/unit/test_lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)    73762 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    31770 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/unit/test_search_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/unit/test_typedef_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-24 15:25:40.000000 pyatlan-0.0.33/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:55:49.585760 pyatlan-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-06-06 15:55:33.000000 pyatlan-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-06 15:55:33.000000 pyatlan-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-06 15:55:33.000000 pyatlan-0.1.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-06 15:55:49.585760 pyatlan-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-06 15:55:33.000000 pyatlan-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:55:49.573760 pyatlan-0.1.0/pyatlan/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:55:49.577760 pyatlan-0.1.0/pyatlan/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/cache/classification_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/cache/custom_metadata_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/cache/enum_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/cache/group_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/cache/role_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/cache/user_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:55:49.577760 pyatlan-0.1.0/pyatlan/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40989 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/client/atlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:55:49.577760 pyatlan-0.1.0/pyatlan/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/generator/generate_from_typdefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:55:49.577760 pyatlan-0.1.0/pyatlan/generator/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/generator/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:55:49.581760 pyatlan-0.1.0/pyatlan/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   852385 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/model/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/model/custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/model/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/model/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/model/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/model/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/model/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59796 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/model/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/model/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24335 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/model/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:55:49.577760 pyatlan-0.1.0/pyatlan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-06 15:55:49.000000 pyatlan-0.1.0/pyatlan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-06 15:55:49.000000 pyatlan-0.1.0/pyatlan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 15:55:49.000000 pyatlan-0.1.0/pyatlan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 15:55:49.000000 pyatlan-0.1.0/pyatlan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-06 15:55:49.000000 pyatlan-0.1.0/pyatlan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-06 15:55:49.000000 pyatlan-0.1.0/pyatlan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 15:55:49.585760 pyatlan-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-06 15:55:33.000000 pyatlan-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:55:49.581760 pyatlan-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:55:49.585760 pyatlan-0.1.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/integration/admin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/integration/classification_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/integration/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/integration/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38214 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/integration/custom_metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/integration/glossary_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23633 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/integration/lineage_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/integration/query_parser_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/integration/s3_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34056 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/integration/test_entity_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/integration/test_index_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:55:49.585760 pyatlan-0.1.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/unit/test_classification_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/unit/test_custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/unit/test_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/unit/test_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66551 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31770 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/unit/test_search_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/unit/test_typedef_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/unit/test_utils.py
```

### Comparing `pyatlan-0.0.33/LICENSE` & `pyatlan-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.33/PKG-INFO` & `pyatlan-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.0.33
+Version: 0.1.0
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.0.33/README.md` & `pyatlan-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.33/pyatlan/cache/classification_cache.py` & `pyatlan-0.1.0/pyatlan/cache/classification_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.33/pyatlan/cache/custom_metadata_cache.py` & `pyatlan-0.1.0/pyatlan/cache/custom_metadata_cache.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
-import json
-from typing import Any, Optional
+from typing import Optional
 
-from pyatlan.client.atlan import AtlanClient
 from pyatlan.error import InvalidRequestError, LogicError, NotFoundError
-from pyatlan.model.core import CustomMetadata
 from pyatlan.model.enums import AtlanTypeCategory
 from pyatlan.model.typedef import AttributeDef, CustomMetadataDef
 
 
 class Synonym:
     def __init__(self, storage_name):
         self.storage_name = storage_name
@@ -31,15 +28,15 @@
     map_attr_id_to_name: dict[str, dict[str, str]] = dict()
     map_attr_name_to_id: dict[str, dict[str, str]] = dict()
     archived_attr_ids: dict[str, str] = dict()
     types_by_asset: dict[str, set[type]] = dict()
 
     @classmethod
     def refresh_cache(cls) -> None:
-        from pyatlan.model.core import CustomMetadata, to_snake_case
+        from pyatlan.client.atlan import AtlanClient
 
         client = AtlanClient.get_default_client()
         if client is None:
             client = AtlanClient()
         response = client.get_typedefs(type_category=AtlanTypeCategory.CUSTOM_METADATA)
         if response is not None:
             cls.map_id_to_name = {}
@@ -52,47 +49,29 @@
                 type_id = cm.name
                 type_name = cm.display_name
                 cls.cache_by_id[type_id] = cm
                 cls.map_id_to_name[type_id] = type_name
                 cls.map_name_to_id[type_name] = type_id
                 cls.map_attr_id_to_name[type_id] = {}
                 cls.map_attr_name_to_id[type_id] = {}
-                meta_name = cm.display_name.replace(" ", "")
-                attribute_class_name = f"Attributes_{meta_name}"
-                attrib_type = type(attribute_class_name, (CustomMetadata,), {})
-                attrib_type._meta_data_type_id = type_id  # type: ignore
-                attrib_type._meta_data_type_name = type_name  # type: ignore
-                cls.map_id_to_type[type_id] = attrib_type
-                applicable_types: set[str] = set()
                 if cm.attribute_defs:
                     for attr in cm.attribute_defs:
-                        if attr.options and attr.options.custom_applicable_entity_types:
-                            applicable_types.update(
-                                json.loads(attr.options.custom_applicable_entity_types)
-                            )
                         attr_id = str(attr.name)
                         attr_name = str(attr.display_name)
-                        # Use a renamed attribute everywhere
-                        attr_renamed = to_snake_case(attr_name)
-                        cls.map_attr_id_to_name[type_id][attr_id] = attr_renamed
+                        cls.map_attr_id_to_name[type_id][attr_id] = attr_name
                         if attr.options and attr.options.is_archived:
-                            cls.archived_attr_ids[attr_id] = attr_renamed
-                        elif attr_renamed in cls.map_attr_name_to_id[type_id]:
+                            cls.archived_attr_ids[attr_id] = attr_name
+                        elif attr_name in cls.map_attr_name_to_id[type_id]:
                             raise LogicError(
-                                f"Multiple custom attributes with exactly the same name ({attr_renamed}) "
+                                f"Multiple custom attributes with exactly the same name ({attr_name}) "
                                 f"found for: {type_name}",
                                 code="ATLAN-PYTHON-500-100",
                             )
                         else:
-                            setattr(attrib_type, attr_renamed, Synonym(attr_id))
-                            cls.map_attr_name_to_id[type_id][attr_renamed] = attr_id
-                    for asset_type in applicable_types:
-                        if asset_type not in cls.types_by_asset:
-                            cls.types_by_asset[asset_type] = set()
-                        cls.types_by_asset[asset_type].add(attrib_type)
+                            cls.map_attr_name_to_id[type_id][attr_name] = attr_id
 
     @classmethod
     def get_id_for_name(cls, name: str) -> str:
         """
         Translate the provided human-readable custom metadata set name to its Atlan-internal ID string.
         """
         if name is None or not name.strip():
@@ -198,26 +177,30 @@
             )
         raise NotFoundError(
             message=f"Custom metadata with ID {set_id} does not exist.",
             code="ATLAN-PYTHON-404-009",
         )
 
     @classmethod
-    def get_attr_name_for_id(cls, set_id: str, attr_id: str) -> Optional[str]:
+    def get_attr_name_for_id(cls, set_id: str, attr_id: str) -> str:
         """
-        Translate the provided human-readable custom metadata set and attribute names to the Atlan-internal ID string
-        for the attribute.
+        Given the Atlan-internal ID stringfor the set and the Atlan-internal ID for the attribute return the
+        human-readable custom metadata name for the attribute.
         """
         if sub_map := cls.map_attr_id_to_name.get(set_id):
             if attr_name := sub_map.get(attr_id):
                 return attr_name
             cls.refresh_cache()
             if sub_map := cls.map_attr_id_to_name.get(set_id):
-                return sub_map.get(attr_id)
-        return None
+                if attr_name := sub_map.get(attr_id):
+                    return attr_name
+        raise NotFoundError(
+            message=f"Custom metadata property with ID {attr_id} does not exist in the custom metadata {set_id}.",
+            code="ATLAN-PYTHON-404-009",
+        )
 
     @classmethod
     def _get_attributes_for_search_results(cls, set_id: str) -> Optional[list[str]]:
         if sub_map := cls.map_attr_name_to_id.get(set_id):
             attr_ids = sub_map.values()
             return [f"{set_id}.{idstr}" for idstr in attr_ids]
         return None
@@ -231,41 +214,14 @@
             if dot_names := cls._get_attributes_for_search_results(set_id):
                 return dot_names
             cls.refresh_cache()
             return cls._get_attributes_for_search_results(set_id)
         return None
 
     @classmethod
-    def get_custom_metadata(
-        cls,
-        name: str,
-        asset_type: type,
-        business_attributes: Optional[dict[str, Any]] = None,
-    ) -> CustomMetadata:
-        type_name = asset_type.__name__
-        ba_id = cls.get_id_for_name(name)
-        if ba_id is None:
-            raise ValueError(f"No custom metadata with the name: {name} exist")
-        for a_type in CustomMetadataCache.types_by_asset[type_name]:
-            if (
-                hasattr(a_type, "_meta_data_type_name")
-                and a_type._meta_data_type_name == name
-            ):
-                break
-        else:
-            raise ValueError(f"Custom metadata {name} is not applicable to {type_name}")
-        if ba_type := CustomMetadataCache.get_type_for_id(ba_id):
-            return (
-                ba_type(business_attributes[ba_id])
-                if business_attributes and ba_id in business_attributes
-                else ba_type()
-            )
-        raise ValueError(f"Custom metadata {name} is not applicable to {type_name}")
-
-    @classmethod
     def get_custom_metadata_def(cls, name: str) -> CustomMetadataDef:
         """
         Retrieve the full custom metadata structure definition.
         """
         ba_id = cls.get_id_for_name(name)
         if ba_id is None:
             raise ValueError(f"No custom metadata with the name: {name} exist")
```

### Comparing `pyatlan-0.0.33/pyatlan/cache/enum_cache.py` & `pyatlan-0.1.0/pyatlan/cache/enum_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.33/pyatlan/cache/group_cache.py` & `pyatlan-0.1.0/pyatlan/cache/group_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.33/pyatlan/cache/role_cache.py` & `pyatlan-0.1.0/pyatlan/cache/role_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.33/pyatlan/cache/user_cache.py` & `pyatlan-0.1.0/pyatlan/cache/user_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.33/pyatlan/client/atlan.py` & `pyatlan-0.1.0/pyatlan/client/atlan.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,18 +35,20 @@
     GET_ALL_TYPE_DEFS,
     GET_CURRENT_USER,
     GET_ENTITY_BY_GUID,
     GET_ENTITY_BY_UNIQUE_ATTRIBUTE,
     GET_GROUP_MEMBERS,
     GET_GROUPS,
     GET_LINEAGE,
+    GET_LINEAGE_LIST,
     GET_ROLES,
     GET_USER_GROUPS,
     GET_USERS,
     INDEX_SEARCH,
+    PARSE_QUERY,
     PARTIAL_UPDATE_ENTITY_BY_ATTRIBUTE,
     REMOVE_USERS_FROM_GROUP,
     UPDATE_ENTITY_BY_ATTRIBUTE,
     UPDATE_GROUP,
     UPDATE_TYPE_DEFS,
     UPDATE_USER,
 )
@@ -70,31 +72,37 @@
     AssetRequest,
     AssetResponse,
     AtlanObject,
     BulkRequest,
     Classification,
     ClassificationName,
     Classifications,
-    CustomMetadata,
-    CustomMetadataReqest,
 )
+from pyatlan.model.custom_metadata import CustomMetadataDict, CustomMetadataRequest
 from pyatlan.model.enums import (
     AtlanConnectorType,
     AtlanDeleteType,
     AtlanTypeCategory,
     CertificateStatus,
+    LineageDirection,
 )
 from pyatlan.model.group import (
     AtlanGroup,
     CreateGroupRequest,
     CreateGroupResponse,
     GroupResponse,
     RemoveFromGroupRequest,
 )
-from pyatlan.model.lineage import LineageRequest, LineageResponse
+from pyatlan.model.lineage import (
+    LineageListRequest,
+    LineageListResponse,
+    LineageRequest,
+    LineageResponse,
+)
+from pyatlan.model.query import ParsedQuery, QueryParserRequest
 from pyatlan.model.response import AssetMutationResponse
 from pyatlan.model.role import RoleResponse
 from pyatlan.model.search import DSL, IndexSearchRequest, Term
 from pyatlan.model.typedef import (
     ClassificationDef,
     CustomMetadataDef,
     EnumDef,
@@ -136,18 +144,18 @@
     Type[View],
     Type[MaterialisedView],
 ]
 
 
 def get_session():
     retry_strategy = Retry(
-        total=6,
+        total=10,
         backoff_factor=1,
         status_forcelist=[403, 500, 502, 503, 504],
-        allowed_methods=["HEAD", "GET", "OPTIONS"],
+        allowed_methods=["HEAD", "GET", "OPTIONS", "POST", "PUT", "DELETE"],
     )
     adapter = HTTPAdapter(max_retries=retry_strategy)
     session = requests.session()
     session.mount("https://", adapter)
     session.headers.update({"x-atlan-agent": "sdk", "x-atlan-agent-id": "python"})
     return session
 
@@ -628,14 +636,25 @@
             limit=5,
             post_filter='{"username":"' + username + '"}',
         ):
             if response.records and len(response.records) >= 1:
                 return response.records[0]
         return None
 
+    def parse_query(self, query: QueryParserRequest) -> Optional[ParsedQuery]:
+        """
+        Parses the provided query to describe its component parts.
+        """
+        raw_json = self._call_api(
+            PARSE_QUERY,
+            request_obj=query,
+            exclude_unset=True,
+        )
+        return ParsedQuery(**raw_json)
+
     @validate_arguments()
     def get_asset_by_qualified_name(
         self,
         qualified_name: str,
         asset_type: Type[A],
         min_ext_info: bool = False,
         ignore_relationships: bool = False,
@@ -991,68 +1010,64 @@
         asset = asset_type()
         asset.qualified_name = qualified_name
         asset.name = name
         asset.remove_announcement()
         return self._update_asset_by_attribute(asset, asset_type, qualified_name)
 
     def update_custom_metadata_attributes(
-        self, guid: str, custom_metadata: CustomMetadata
+        self, guid: str, custom_metadata: CustomMetadataDict
     ):
-        custom_metadata_request = CustomMetadataReqest(__root__=custom_metadata)
+        custom_metadata_request = CustomMetadataRequest.create(
+            custom_metadata_dict=custom_metadata
+        )
         self._call_api(
             ADD_BUSINESS_ATTRIBUTE_BY_ID.format_path(
-                {"entity_guid": guid, "bm_id": custom_metadata._meta_data_type_id}
+                {
+                    "entity_guid": guid,
+                    "bm_id": custom_metadata_request.custom_metadata_set_id,
+                }
             ),
             None,
             custom_metadata_request,
         )
 
-    def replace_custom_metadata(self, guid: str, custom_metadata: CustomMetadata):
-        from pyatlan.cache.custom_metadata_cache import CustomMetadataCache
-
-        # Iterate through the custom metadata provided and explicitly set every
-        # single attribute, so that they are all serialized out (forcing removal
-        # of any empty ones)
-        for k, v in custom_metadata.items():
-            # Need to translate the hashed-string key here back to an attribute name
-            attr_name = str(
-                CustomMetadataCache.get_attr_name_for_id(
-                    set_id=custom_metadata._meta_data_type_id, attr_id=k
-                )
-            )
-            if not v:
-                setattr(custom_metadata, attr_name, None)
-            else:
-                setattr(custom_metadata, attr_name, v)
-        custom_metadata_request = CustomMetadataReqest(__root__=custom_metadata)
+    def replace_custom_metadata(self, guid: str, custom_metadata: CustomMetadataDict):
+        # clear unset attributes so that they are removed
+        custom_metadata.clear_unset()
+        custom_metadata_request = CustomMetadataRequest.create(
+            custom_metadata_dict=custom_metadata
+        )
         self._call_api(
             ADD_BUSINESS_ATTRIBUTE_BY_ID.format_path(
-                {"entity_guid": guid, "bm_id": custom_metadata._meta_data_type_id}
+                {
+                    "entity_guid": guid,
+                    "bm_id": custom_metadata_request.custom_metadata_set_id,
+                }
             ),
             None,
             custom_metadata_request,
         )
 
     def remove_custom_metadata(self, guid: str, cm_name: str):
-        from pyatlan.cache.custom_metadata_cache import CustomMetadataCache
-
-        # Ensure the custom metadata exists first - let this throw an error if not
-        if cm_id := CustomMetadataCache.get_id_for_name(cm_name):
-            # Initialize a dict of empty attributes for the custom metadata, and then
-            # send that so that they are removed accordingly
-            if cm_type := CustomMetadataCache.get_type_for_id(cm_id):
-                custom_metadata = cm_type()
-                custom_metadata_request = CustomMetadataReqest(__root__=custom_metadata)
-                self._call_api(
-                    ADD_BUSINESS_ATTRIBUTE_BY_ID.format_path(
-                        {"entity_guid": guid, "bm_id": cm_id}
-                    ),
-                    None,
-                    custom_metadata_request,
-                )
+        custom_metadata = CustomMetadataDict(name=cm_name)
+        # invoke clear_all so all attributes are set to None and consequently removed
+        custom_metadata.clear_all()
+        custom_metadata_request = CustomMetadataRequest.create(
+            custom_metadata_dict=custom_metadata
+        )
+        self._call_api(
+            ADD_BUSINESS_ATTRIBUTE_BY_ID.format_path(
+                {
+                    "entity_guid": guid,
+                    "bm_id": custom_metadata_request.custom_metadata_set_id,
+                }
+            ),
+            None,
+            custom_metadata_request,
+        )
 
     @validate_arguments()
     def append_terms(
         self,
         asset_type: Type[A],
         terms: list[AtlasGlossaryTerm],
         guid: Optional[str] = None,
@@ -1171,7 +1186,19 @@
         return [asset for asset in results if isinstance(asset, Connection)]
 
     def get_lineage(self, lineage_request: LineageRequest) -> LineageResponse:
         raw_json = self._call_api(
             GET_LINEAGE, None, lineage_request, exclude_unset=False
         )
         return LineageResponse(**raw_json)
+
+    def get_lineage_list(
+        self, lineage_request: LineageListRequest
+    ) -> LineageListResponse:
+        if lineage_request.direction == LineageDirection.BOTH:
+            raise InvalidRequestException(
+                message="Unable to request both directions of lineage at the same time through the lineage list API.",
+            )
+        raw_json = self._call_api(
+            GET_LINEAGE_LIST, None, lineage_request, exclude_unset=True
+        )
+        return LineageListResponse(**raw_json)
```

### Comparing `pyatlan-0.0.33/pyatlan/client/constants.py` & `pyatlan-0.1.0/pyatlan/client/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 from pyatlan.utils import (
     ADMIN_URI,
     API,
     APPLICATION_JSON,
     APPLICATION_OCTET_STREAM,
     BASE_URI,
     MULTIPART_FORM_DATA,
+    SQL_URI,
     HTTPMethod,
     HTTPStatus,
 )
 
 ROLE_API = f"{ADMIN_URI}roles"
 GROUP_API = f"{ADMIN_URI}groups"
 USER_API = f"{ADMIN_URI}users"
+QUERY_API = f"{SQL_URI}query"
 
 # Role APIs
 GET_ROLES = API(ROLE_API, HTTPMethod.GET, HTTPStatus.OK)
 
 # Group APIs
 GET_GROUPS = API(GROUP_API, HTTPMethod.GET, HTTPStatus.OK)
 CREATE_GROUP = API(GROUP_API, HTTPMethod.POST, HTTPStatus.OK)
@@ -41,26 +43,30 @@
     USER_API + "/{user_guid}/groups", HTTPMethod.POST, HTTPStatus.OK
 )
 CHANGE_USER_ROLE = API(
     USER_API + "/{user_guid}/roles/update", HTTPMethod.POST, HTTPStatus.OK
 )
 GET_CURRENT_USER = API(f"{USER_API}/current", HTTPMethod.GET, HTTPStatus.OK)
 
+# SQL parsing APIs
+PARSE_QUERY = API(f"{QUERY_API}/parse", HTTPMethod.POST, HTTPStatus.OK)
+
 ENTITY_API = f"{BASE_URI}entity/"
 PREFIX_ATTR = "attr:"
 PREFIX_ATTR_ = "attr_"
 ADMIN_API = f"{BASE_URI}admin/"
 ENTITY_PURGE_API = f"{ADMIN_API}purge/"
 ENTITY_BULK_API = f"{ENTITY_API}bulk/"
 BULK_SET_CLASSIFICATIONS = "bulk/setClassifications"
 BULK_HEADERS = "bulk/headers"
 
 BULK_UPDATE = API(ENTITY_BULK_API, HTTPMethod.POST, HTTPStatus.OK)
 # Lineage APIs
 GET_LINEAGE = API(f"{BASE_URI}lineage/getlineage", HTTPMethod.POST, HTTPStatus.OK)
+GET_LINEAGE_LIST = API(f"{BASE_URI}lineage/list", HTTPMethod.POST, HTTPStatus.OK)
 # Entity APIs
 GET_ENTITY_BY_GUID = API(f"{ENTITY_API}guid", HTTPMethod.GET, HTTPStatus.OK)
 GET_ENTITY_BY_UNIQUE_ATTRIBUTE = API(
     f"{ENTITY_API}uniqueAttribute/type", HTTPMethod.GET, HTTPStatus.OK
 )
 GET_ENTITIES_BY_GUIDS = API(ENTITY_BULK_API, HTTPMethod.GET, HTTPStatus.OK)
 GET_ENTITIES_BY_UNIQUE_ATTRIBUTE = API(
```

### Comparing `pyatlan-0.0.33/pyatlan/error.py` & `pyatlan-0.1.0/pyatlan/error.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.33/pyatlan/exceptions.py` & `pyatlan-0.1.0/pyatlan/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.33/pyatlan/generator/generate_from_typdefs.py` & `pyatlan-0.1.0/pyatlan/generator/generate_from_typdefs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.33/pyatlan/model/assets.py` & `pyatlan-0.1.0/pyatlan/model/assets.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,37 +6,33 @@
 import hashlib
 import sys
 from datetime import datetime
 from io import StringIO
 from typing import Any, ClassVar, Dict, List, Optional, TypeVar
 from urllib.parse import quote, unquote
 
-from pydantic import Field, StrictStr, root_validator, validator
+from pydantic import Field, PrivateAttr, StrictStr, root_validator, validator
 
-from pyatlan.model.core import (
-    Announcement,
-    AtlanObject,
-    Classification,
-    CustomMetadata,
-    Meaning,
-)
+from pyatlan.model.core import Announcement, AtlanObject, Classification, Meaning
+from pyatlan.model.custom_metadata import CustomMetadataDict, CustomMetadataProxy
 from pyatlan.model.enums import (
     ADLSAccessTier,
     ADLSAccountStatus,
     ADLSEncryptionTypes,
     ADLSLeaseState,
     ADLSLeaseStatus,
     ADLSObjectArchiveStatus,
     ADLSObjectType,
     ADLSPerformance,
     ADLSProvisionState,
     ADLSReplicationType,
     ADLSStorageKind,
     AnnouncementType,
     AtlanConnectorType,
+    AuthPolicyType,
     CertificateStatus,
     EntityStatus,
     FileType,
     GoogleDatastudioAssetType,
     IconType,
     KafkaTopicCompressionType,
     PowerbiEndorsement,
@@ -45,14 +41,16 @@
     QuickSightDatasetFieldType,
     QuickSightDatasetImportMode,
     QuickSightFolderType,
     SourceCostUnitType,
 )
 from pyatlan.model.internal import AtlasServer, Internal
 from pyatlan.model.structs import (
+    AuthPolicyCondition,
+    AuthPolicyValiditySchedule,
     AwsTag,
     AzureTag,
     BadgeCondition,
     ColumnValueFrequencyMap,
     DbtMetricFilter,
     GoogleLabel,
     GoogleTag,
@@ -84,14 +82,21 @@
 
 class Referenceable(AtlanObject):
     """Description"""
 
     def __init__(__pydantic_self__, **data: Any) -> None:
         super().__init__(**data)
         __pydantic_self__.__fields_set__.update(["attributes", "type_name"])
+        __pydantic_self__._metadata_proxy = CustomMetadataProxy(
+            __pydantic_self__.business_attributes
+        )
+
+    def json(self, *args, **kwargs) -> str:
+        self.business_attributes = self._metadata_proxy.business_attributes
+        return super().json(**kwargs)
 
     def __setattr__(self, name, value):
         if name in Referenceable._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
@@ -152,14 +157,15 @@
         meanings: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="meanings"
         )  # relationship
 
         def validate_required(self):
             pass
 
+    _metadata_proxy: CustomMetadataProxy = PrivateAttr()
     attributes: "Referenceable.Attributes" = Field(
         default_factory=lambda: Referenceable.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary "
         "by type, so are described in the sub-types of this schema.\n",
     )
     business_attributes: Optional[Dict[str, Any]] = Field(
         None,
@@ -252,59 +258,22 @@
 
     unique_attributes: Optional[dict[str, Any]] = Field(None)
 
     def validate_required(self):
         if not self.create_time or self.created_by:
             self.attributes.validate_required()
 
-    def get_custom_metadata(self, name: str) -> CustomMetadata:
-        from pyatlan.cache.custom_metadata_cache import CustomMetadataCache
+    def get_custom_metadata(self, name: str) -> CustomMetadataDict:
+        return self._metadata_proxy.get_custom_metadata(name=name)
 
-        ba_id = CustomMetadataCache.get_id_for_name(name)
-        if ba_id is None:
-            raise ValueError(f"No custom metadata with the name: {name} exist")
-        for a_type in CustomMetadataCache.types_by_asset[self.type_name]:
-            if (
-                hasattr(a_type, "_meta_data_type_name")
-                and a_type._meta_data_type_name == name
-            ):
-                break
-        else:
-            raise ValueError(
-                f"Custom metadata attributes {name} are not applicable to {self.type_name}"
-            )
-        if ba_type := CustomMetadataCache.get_type_for_id(ba_id):
-            return (
-                ba_type(self.business_attributes[ba_id])
-                if self.business_attributes and ba_id in self.business_attributes
-                else ba_type()
-            )
-        else:
-            raise ValueError(
-                f"Custom metadata attributes {name} are not applicable to {self.type_name}"
-            )
-
-    def set_custom_metadata(self, custom_metadata: CustomMetadata) -> None:
-        from pyatlan.cache.custom_metadata_cache import CustomMetadataCache
+    def set_custom_metadata(self, custom_metadata: CustomMetadataDict):
+        return self._metadata_proxy.set_custom_metadata(custom_metadata=custom_metadata)
 
-        if not isinstance(custom_metadata, CustomMetadata):
-            raise ValueError(
-                "business_attributes must be an instance of CustomMetadata"
-            )
-        if (
-            type(custom_metadata)
-            not in CustomMetadataCache.types_by_asset[self.type_name]
-        ):
-            raise ValueError(
-                f"Business attributes {custom_metadata._meta_data_type_name} are not applicable to {self.type_name}"
-            )
-        ba_dict = dict(custom_metadata)
-        if not self.business_attributes:
-            self.business_attributes = {}
-        self.business_attributes[custom_metadata._meta_data_type_id] = ba_dict
+    def flush_custom_metadata(self):
+        self.business_attributes = self._metadata_proxy.business_attributes
 
 
 class Asset(Referenceable):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Asset._convience_properties:
@@ -2191,158 +2160,14 @@
     def remove_owners(self):
         self.attributes.remove_owners()
 
     def remove_certificate(self):
         self.attributes.remove_certificate()
 
 
-class AtlasGlossary(Asset, type_name="AtlasGlossary"):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in AtlasGlossary._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "short_description",
-        "long_description",
-        "language",
-        "usage",
-        "additional_attributes",
-        "terms",
-        "categories",
-    ]
-
-    @property
-    def short_description(self) -> Optional[str]:
-        return self.attributes.short_description
-
-    @short_description.setter
-    def short_description(self, short_description: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.short_description = short_description
-
-    @property
-    def long_description(self) -> Optional[str]:
-        return self.attributes.long_description
-
-    @long_description.setter
-    def long_description(self, long_description: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.long_description = long_description
-
-    @property
-    def language(self) -> Optional[str]:
-        return self.attributes.language
-
-    @language.setter
-    def language(self, language: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.language = language
-
-    @property
-    def usage(self) -> Optional[str]:
-        return self.attributes.usage
-
-    @usage.setter
-    def usage(self, usage: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.usage = usage
-
-    @property
-    def additional_attributes(self) -> Optional[dict[str, str]]:
-        return self.attributes.additional_attributes
-
-    @additional_attributes.setter
-    def additional_attributes(self, additional_attributes: Optional[dict[str, str]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.additional_attributes = additional_attributes
-
-    @property
-    def terms(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.terms
-
-    @terms.setter
-    def terms(self, terms: Optional[list[AtlasGlossaryTerm]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.terms = terms
-
-    @property
-    def categories(self) -> Optional[list[AtlasGlossaryCategory]]:
-        return self.attributes.categories
-
-    @categories.setter
-    def categories(self, categories: Optional[list[AtlasGlossaryCategory]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.categories = categories
-
-    type_name: str = Field("AtlasGlossary", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "AtlasGlossary":
-            raise ValueError("must be AtlasGlossary")
-        return v
-
-    class Attributes(Asset.Attributes):
-        short_description: Optional[str] = Field(
-            None, description="", alias="shortDescription"
-        )
-        long_description: Optional[str] = Field(
-            None, description="", alias="longDescription"
-        )
-        language: Optional[str] = Field(None, description="", alias="language")
-        usage: Optional[str] = Field(None, description="", alias="usage")
-        additional_attributes: Optional[dict[str, str]] = Field(
-            None, description="", alias="additionalAttributes"
-        )
-        terms: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="terms"
-        )  # relationship
-        categories: Optional[list[AtlasGlossaryCategory]] = Field(
-            None, description="", alias="categories"
-        )  # relationship
-
-        @classmethod
-        # @validate_arguments()
-        def create(cls, *, name: StrictStr) -> AtlasGlossary.Attributes:
-            validate_required_fields(["name"], [name])
-            return AtlasGlossary.Attributes(name=name, qualified_name=next_id())
-
-    attributes: "AtlasGlossary.Attributes" = Field(
-        default_factory=lambda: AtlasGlossary.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-    @root_validator()
-    def update_qualified_name(cls, values):
-        if (
-            "attributes" in values
-            and values["attributes"]
-            and not values["attributes"].qualified_name
-        ):
-            values["attributes"].qualified_name = values["guid"]
-        return values
-
-    @classmethod
-    # @validate_arguments()
-    def create(cls, *, name: StrictStr) -> AtlasGlossary:
-        validate_required_fields(["name"], [name])
-        return AtlasGlossary(attributes=AtlasGlossary.Attributes.create(name=name))
-
-
 class DataSet(Asset, type_name="DataSet"):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in DataSet._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -2354,481 +2179,14 @@
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "DataSet":
             raise ValueError("must be DataSet")
         return v
 
 
-class ProcessExecution(Asset, type_name="ProcessExecution"):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in ProcessExecution._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = []
-
-    type_name: str = Field("ProcessExecution", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "ProcessExecution":
-            raise ValueError("must be ProcessExecution")
-        return v
-
-
-class AtlasGlossaryTerm(Asset, type_name="AtlasGlossaryTerm"):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in AtlasGlossaryTerm._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "short_description",
-        "long_description",
-        "examples",
-        "abbreviation",
-        "usage",
-        "additional_attributes",
-        "translation_terms",
-        "valid_values_for",
-        "synonyms",
-        "replaced_by",
-        "valid_values",
-        "replacement_terms",
-        "see_also",
-        "translated_terms",
-        "is_a",
-        "anchor",
-        "antonyms",
-        "assigned_entities",
-        "classifies",
-        "categories",
-        "preferred_to_terms",
-        "preferred_terms",
-    ]
-
-    @property
-    def short_description(self) -> Optional[str]:
-        return self.attributes.short_description
-
-    @short_description.setter
-    def short_description(self, short_description: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.short_description = short_description
-
-    @property
-    def long_description(self) -> Optional[str]:
-        return self.attributes.long_description
-
-    @long_description.setter
-    def long_description(self, long_description: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.long_description = long_description
-
-    @property
-    def examples(self) -> Optional[set[str]]:
-        return self.attributes.examples
-
-    @examples.setter
-    def examples(self, examples: Optional[set[str]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.examples = examples
-
-    @property
-    def abbreviation(self) -> Optional[str]:
-        return self.attributes.abbreviation
-
-    @abbreviation.setter
-    def abbreviation(self, abbreviation: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.abbreviation = abbreviation
-
-    @property
-    def usage(self) -> Optional[str]:
-        return self.attributes.usage
-
-    @usage.setter
-    def usage(self, usage: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.usage = usage
-
-    @property
-    def additional_attributes(self) -> Optional[dict[str, str]]:
-        return self.attributes.additional_attributes
-
-    @additional_attributes.setter
-    def additional_attributes(self, additional_attributes: Optional[dict[str, str]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.additional_attributes = additional_attributes
-
-    @property
-    def translation_terms(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.translation_terms
-
-    @translation_terms.setter
-    def translation_terms(self, translation_terms: Optional[list[AtlasGlossaryTerm]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.translation_terms = translation_terms
-
-    @property
-    def valid_values_for(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.valid_values_for
-
-    @valid_values_for.setter
-    def valid_values_for(self, valid_values_for: Optional[list[AtlasGlossaryTerm]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.valid_values_for = valid_values_for
-
-    @property
-    def synonyms(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.synonyms
-
-    @synonyms.setter
-    def synonyms(self, synonyms: Optional[list[AtlasGlossaryTerm]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.synonyms = synonyms
-
-    @property
-    def replaced_by(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.replaced_by
-
-    @replaced_by.setter
-    def replaced_by(self, replaced_by: Optional[list[AtlasGlossaryTerm]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.replaced_by = replaced_by
-
-    @property
-    def valid_values(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.valid_values
-
-    @valid_values.setter
-    def valid_values(self, valid_values: Optional[list[AtlasGlossaryTerm]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.valid_values = valid_values
-
-    @property
-    def replacement_terms(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.replacement_terms
-
-    @replacement_terms.setter
-    def replacement_terms(self, replacement_terms: Optional[list[AtlasGlossaryTerm]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.replacement_terms = replacement_terms
-
-    @property
-    def see_also(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.see_also
-
-    @see_also.setter
-    def see_also(self, see_also: Optional[list[AtlasGlossaryTerm]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.see_also = see_also
-
-    @property
-    def translated_terms(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.translated_terms
-
-    @translated_terms.setter
-    def translated_terms(self, translated_terms: Optional[list[AtlasGlossaryTerm]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.translated_terms = translated_terms
-
-    @property
-    def is_a(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.is_a
-
-    @is_a.setter
-    def is_a(self, is_a: Optional[list[AtlasGlossaryTerm]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.is_a = is_a
-
-    @property
-    def anchor(self) -> AtlasGlossary:
-        return self.attributes.anchor
-
-    @anchor.setter
-    def anchor(self, anchor: AtlasGlossary):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.anchor = anchor
-
-    @property
-    def antonyms(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.antonyms
-
-    @antonyms.setter
-    def antonyms(self, antonyms: Optional[list[AtlasGlossaryTerm]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.antonyms = antonyms
-
-    @property
-    def assigned_entities(self) -> Optional[list[Referenceable]]:
-        return self.attributes.assigned_entities
-
-    @assigned_entities.setter
-    def assigned_entities(self, assigned_entities: Optional[list[Referenceable]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.assigned_entities = assigned_entities
-
-    @property
-    def classifies(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.classifies
-
-    @classifies.setter
-    def classifies(self, classifies: Optional[list[AtlasGlossaryTerm]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.classifies = classifies
-
-    @property
-    def categories(self) -> Optional[list[AtlasGlossaryCategory]]:
-        return self.attributes.categories
-
-    @categories.setter
-    def categories(self, categories: Optional[list[AtlasGlossaryCategory]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.categories = categories
-
-    @property
-    def preferred_to_terms(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.preferred_to_terms
-
-    @preferred_to_terms.setter
-    def preferred_to_terms(self, preferred_to_terms: Optional[list[AtlasGlossaryTerm]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.preferred_to_terms = preferred_to_terms
-
-    @property
-    def preferred_terms(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.preferred_terms
-
-    @preferred_terms.setter
-    def preferred_terms(self, preferred_terms: Optional[list[AtlasGlossaryTerm]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.preferred_terms = preferred_terms
-
-    type_name: str = Field("AtlasGlossaryTerm", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "AtlasGlossaryTerm":
-            raise ValueError("must be AtlasGlossaryTerm")
-        return v
-
-    class Attributes(Asset.Attributes):
-        short_description: Optional[str] = Field(
-            None, description="", alias="shortDescription"
-        )
-        long_description: Optional[str] = Field(
-            None, description="", alias="longDescription"
-        )
-        examples: Optional[set[str]] = Field(None, description="", alias="examples")
-        abbreviation: Optional[str] = Field(None, description="", alias="abbreviation")
-        usage: Optional[str] = Field(None, description="", alias="usage")
-        additional_attributes: Optional[dict[str, str]] = Field(
-            None, description="", alias="additionalAttributes"
-        )
-        translation_terms: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="translationTerms"
-        )  # relationship
-        valid_values_for: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="validValuesFor"
-        )  # relationship
-        synonyms: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="synonyms"
-        )  # relationship
-        replaced_by: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="replacedBy"
-        )  # relationship
-        valid_values: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="validValues"
-        )  # relationship
-        replacement_terms: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="replacementTerms"
-        )  # relationship
-        see_also: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="seeAlso"
-        )  # relationship
-        translated_terms: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="translatedTerms"
-        )  # relationship
-        is_a: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="isA"
-        )  # relationship
-        anchor: AtlasGlossary = Field(
-            None, description="", alias="anchor"
-        )  # relationship
-        antonyms: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="antonyms"
-        )  # relationship
-        assigned_entities: Optional[list[Referenceable]] = Field(
-            None, description="", alias="assignedEntities"
-        )  # relationship
-        classifies: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="classifies"
-        )  # relationship
-        categories: Optional[list[AtlasGlossaryCategory]] = Field(
-            None, description="", alias="categories"
-        )  # relationship
-        preferred_to_terms: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="preferredToTerms"
-        )  # relationship
-        preferred_terms: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="preferredTerms"
-        )  # relationship
-
-        @classmethod
-        # @validate_arguments()
-        def create(
-            cls,
-            *,
-            name: StrictStr,
-            anchor: Optional[AtlasGlossary] = None,
-            glossary_qualified_name: Optional[StrictStr] = None,
-            glossary_guid: Optional[StrictStr] = None,
-            categories: Optional[list[AtlasGlossaryCategory]] = None,
-        ) -> AtlasGlossaryTerm.Attributes:
-            validate_required_fields(["name"], [name])
-            validate_single_required_field(
-                ["anchor", "glossary_qualified_name", "glossary_guid"],
-                [anchor, glossary_qualified_name, glossary_guid],
-            )
-            if glossary_qualified_name:
-                anchor = AtlasGlossary()
-                anchor.unique_attributes = {"qualifiedName": glossary_qualified_name}
-            if glossary_guid:
-                anchor = AtlasGlossary()
-                anchor.guid = glossary_guid
-            return AtlasGlossaryTerm.Attributes(
-                name=name,
-                anchor=anchor,
-                categories=categories,
-                qualified_name=next_id(),
-            )
-
-    attributes: "AtlasGlossaryTerm.Attributes" = Field(
-        default_factory=lambda: AtlasGlossaryTerm.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-    @root_validator()
-    def update_qualified_name(cls, values):
-        if (
-            "attributes" in values
-            and values["attributes"]
-            and not values["attributes"].qualified_name
-        ):
-            values["attributes"].qualified_name = values["guid"]
-        return values
-
-    @classmethod
-    # @validate_arguments()
-    def create(
-        cls,
-        *,
-        name: StrictStr,
-        anchor: Optional[AtlasGlossary] = None,
-        glossary_qualified_name: Optional[StrictStr] = None,
-        glossary_guid: Optional[StrictStr] = None,
-        categories: Optional[list[AtlasGlossaryCategory]] = None,
-    ) -> AtlasGlossaryTerm:
-        validate_required_fields(["name"], [name])
-        return cls(
-            attributes=AtlasGlossaryTerm.Attributes.create(
-                name=name,
-                anchor=anchor,
-                glossary_qualified_name=glossary_qualified_name,
-                glossary_guid=glossary_guid,
-                categories=categories,
-            )
-        )
-
-    @classmethod
-    def create_for_modification(
-        cls: type[SelfAsset],
-        qualified_name: str = "",
-        name: str = "",
-        glossary_guid: str = "",
-    ) -> SelfAsset:
-        validate_required_fields(
-            ["name", "qualified_name", "glossary_guid"],
-            [name, qualified_name, glossary_guid],
-        )
-        glossary = AtlasGlossary()
-        glossary.guid = glossary_guid
-        return cls(
-            attributes=cls.Attributes(
-                qualified_name=qualified_name, name=name, anchor=glossary
-            )
-        )
-
-
-class Cloud(Asset, type_name="Cloud"):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in Cloud._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = []
-
-    type_name: str = Field("Cloud", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Cloud":
-            raise ValueError("must be Cloud")
-        return v
-
-
-class Infrastructure(Asset, type_name="Infrastructure"):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in Infrastructure._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = []
-
-    type_name: str = Field("Infrastructure", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Infrastructure":
-            raise ValueError("must be Infrastructure")
-        return v
-
-
 class Connection(Asset, type_name="Connection"):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Connection._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -3160,43 +2518,14 @@
             if not self.qualified_name:
                 raise ValueError("qualified_name is required")
             if not self.category:
                 raise ValueError("category is required")
             if not self.connector_name:
                 raise ValueError("connector_name is required")
 
-        @classmethod
-        # @validate_arguments()
-        def create(
-            cls,
-            *,
-            name: str,
-            connector_type: AtlanConnectorType,
-            admin_users: Optional[list[str]] = None,
-            admin_groups: Optional[list[str]] = None,
-            admin_roles: Optional[list[str]] = None,
-        ) -> Connection.Attributes:
-            if not name:
-                raise ValueError("name cannot be blank")
-            validate_required_fields(["connector_type"], [connector_type])
-            if admin_users or admin_groups or admin_roles:
-                return cls(
-                    name=name,
-                    qualified_name=connector_type.to_qualified_name(),
-                    connector_name=connector_type.value,
-                    category=connector_type.category.value,
-                    admin_users=admin_users,
-                    admin_groups=admin_groups,
-                    admin_roles=admin_roles,
-                )
-            else:
-                raise ValueError(
-                    "One of admin_user, admin_groups or admin_roles is required"
-                )
-
     attributes: "Connection.Attributes" = Field(
         default_factory=lambda: Connection.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
     @classmethod
@@ -3209,29 +2538,52 @@
         admin_users: Optional[list[str]] = None,
         admin_groups: Optional[list[str]] = None,
         admin_roles: Optional[list[str]] = None,
     ) -> Connection:
         if not name:
             raise ValueError("name cannot be blank")
         validate_required_fields(["connector_type"], [connector_type])
-        if admin_users or admin_groups or admin_roles:
-            attr = cls.Attributes(
-                name=name,
-                qualified_name=connector_type.to_qualified_name(),
-                connector_name=connector_type.value,
-                category=connector_type.category.value,
-                admin_users=admin_users,
-                admin_groups=admin_groups,
-                admin_roles=admin_roles,
-            )
-            return cls(attributes=attr)
-        else:
+        if not admin_users and not admin_groups and not admin_roles:
             raise ValueError(
                 "One of admin_user, admin_groups or admin_roles is required"
             )
+        if admin_roles:
+            from pyatlan.cache.role_cache import RoleCache
+
+            for role_id in admin_roles:
+                if not RoleCache.get_name_for_id(role_id):
+                    raise ValueError(
+                        f"Provided role ID {role_id} was not found in Atlan."
+                    )
+        if admin_groups:
+            from pyatlan.cache.group_cache import GroupCache
+
+            for group_alias in admin_groups:
+                if not GroupCache.get_id_for_alias(group_alias):
+                    raise ValueError(
+                        f"Provided group name {group_alias} was not found in Atlan."
+                    )
+        if admin_users:
+            from pyatlan.cache.user_cache import UserCache
+
+            for username in admin_users:
+                if not UserCache.get_id_for_name(username):
+                    raise ValueError(
+                        f"Provided username {username} was not found in Atlan."
+                    )
+        attr = cls.Attributes(
+            name=name,
+            qualified_name=connector_type.to_qualified_name(),
+            connector_name=connector_type.value,
+            category=connector_type.category.value,
+            admin_users=admin_users if admin_users else [],
+            admin_groups=admin_groups if admin_groups else [],
+            admin_roles=admin_roles if admin_roles else [],
+        )
+        return cls(attributes=attr)
 
 
 class Process(Asset, type_name="Process"):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Process._convience_properties:
@@ -3686,14 +3038,112 @@
     attributes: "Badge.Attributes" = Field(
         default_factory=lambda: Badge.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
+class AccessControl(Asset, type_name="AccessControl"):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in AccessControl._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "is_access_control_enabled",
+        "deny_custom_metadata_guids",
+        "deny_asset_tabs",
+        "channel_link",
+        "policies",
+    ]
+
+    @property
+    def is_access_control_enabled(self) -> Optional[bool]:
+        return self.attributes.is_access_control_enabled
+
+    @is_access_control_enabled.setter
+    def is_access_control_enabled(self, is_access_control_enabled: Optional[bool]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.is_access_control_enabled = is_access_control_enabled
+
+    @property
+    def deny_custom_metadata_guids(self) -> Optional[set[str]]:
+        return self.attributes.deny_custom_metadata_guids
+
+    @deny_custom_metadata_guids.setter
+    def deny_custom_metadata_guids(
+        self, deny_custom_metadata_guids: Optional[set[str]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.deny_custom_metadata_guids = deny_custom_metadata_guids
+
+    @property
+    def deny_asset_tabs(self) -> Optional[set[str]]:
+        return self.attributes.deny_asset_tabs
+
+    @deny_asset_tabs.setter
+    def deny_asset_tabs(self, deny_asset_tabs: Optional[set[str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.deny_asset_tabs = deny_asset_tabs
+
+    @property
+    def channel_link(self) -> Optional[str]:
+        return self.attributes.channel_link
+
+    @channel_link.setter
+    def channel_link(self, channel_link: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.channel_link = channel_link
+
+    @property
+    def policies(self) -> Optional[list[AuthPolicy]]:
+        return self.attributes.policies
+
+    @policies.setter
+    def policies(self, policies: Optional[list[AuthPolicy]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.policies = policies
+
+    type_name: str = Field("AccessControl", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "AccessControl":
+            raise ValueError("must be AccessControl")
+        return v
+
+    class Attributes(Asset.Attributes):
+        is_access_control_enabled: Optional[bool] = Field(
+            None, description="", alias="isAccessControlEnabled"
+        )
+        deny_custom_metadata_guids: Optional[set[str]] = Field(
+            None, description="", alias="denyCustomMetadataGuids"
+        )
+        deny_asset_tabs: Optional[set[str]] = Field(
+            None, description="", alias="denyAssetTabs"
+        )
+        channel_link: Optional[str] = Field(None, description="", alias="channelLink")
+        policies: Optional[list[AuthPolicy]] = Field(
+            None, description="", alias="policies"
+        )  # relationship
+
+    attributes: "AccessControl.Attributes" = Field(
+        default_factory=lambda: AccessControl.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
 class Namespace(Asset, type_name="Namespace"):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Namespace._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -3798,383 +3248,1004 @@
     attributes: "Catalog.Attributes" = Field(
         default_factory=lambda: Catalog.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
-class Google(Cloud):
+class AtlasGlossary(Asset, type_name="AtlasGlossary"):
     """Description"""
 
     def __setattr__(self, name, value):
-        if name in Google._convience_properties:
+        if name in AtlasGlossary._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
-        "google_service",
-        "google_project_name",
-        "google_project_id",
-        "google_project_number",
-        "google_location",
-        "google_location_type",
-        "google_labels",
-        "google_tags",
+        "short_description",
+        "long_description",
+        "language",
+        "usage",
+        "additional_attributes",
+        "terms",
+        "categories",
     ]
 
     @property
-    def google_service(self) -> Optional[str]:
-        return self.attributes.google_service
-
-    @google_service.setter
-    def google_service(self, google_service: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.google_service = google_service
-
-    @property
-    def google_project_name(self) -> Optional[str]:
-        return self.attributes.google_project_name
+    def short_description(self) -> Optional[str]:
+        return self.attributes.short_description
 
-    @google_project_name.setter
-    def google_project_name(self, google_project_name: Optional[str]):
+    @short_description.setter
+    def short_description(self, short_description: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.google_project_name = google_project_name
+        self.attributes.short_description = short_description
 
     @property
-    def google_project_id(self) -> Optional[str]:
-        return self.attributes.google_project_id
+    def long_description(self) -> Optional[str]:
+        return self.attributes.long_description
 
-    @google_project_id.setter
-    def google_project_id(self, google_project_id: Optional[str]):
+    @long_description.setter
+    def long_description(self, long_description: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.google_project_id = google_project_id
+        self.attributes.long_description = long_description
 
     @property
-    def google_project_number(self) -> Optional[int]:
-        return self.attributes.google_project_number
+    def language(self) -> Optional[str]:
+        return self.attributes.language
 
-    @google_project_number.setter
-    def google_project_number(self, google_project_number: Optional[int]):
+    @language.setter
+    def language(self, language: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.google_project_number = google_project_number
+        self.attributes.language = language
 
     @property
-    def google_location(self) -> Optional[str]:
-        return self.attributes.google_location
+    def usage(self) -> Optional[str]:
+        return self.attributes.usage
 
-    @google_location.setter
-    def google_location(self, google_location: Optional[str]):
+    @usage.setter
+    def usage(self, usage: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.google_location = google_location
+        self.attributes.usage = usage
 
     @property
-    def google_location_type(self) -> Optional[str]:
-        return self.attributes.google_location_type
+    def additional_attributes(self) -> Optional[dict[str, str]]:
+        return self.attributes.additional_attributes
 
-    @google_location_type.setter
-    def google_location_type(self, google_location_type: Optional[str]):
+    @additional_attributes.setter
+    def additional_attributes(self, additional_attributes: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.google_location_type = google_location_type
+        self.attributes.additional_attributes = additional_attributes
 
     @property
-    def google_labels(self) -> Optional[list[GoogleLabel]]:
-        return self.attributes.google_labels
+    def terms(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.terms
 
-    @google_labels.setter
-    def google_labels(self, google_labels: Optional[list[GoogleLabel]]):
+    @terms.setter
+    def terms(self, terms: Optional[list[AtlasGlossaryTerm]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.google_labels = google_labels
+        self.attributes.terms = terms
 
     @property
-    def google_tags(self) -> Optional[list[GoogleTag]]:
-        return self.attributes.google_tags
+    def categories(self) -> Optional[list[AtlasGlossaryCategory]]:
+        return self.attributes.categories
 
-    @google_tags.setter
-    def google_tags(self, google_tags: Optional[list[GoogleTag]]):
+    @categories.setter
+    def categories(self, categories: Optional[list[AtlasGlossaryCategory]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.google_tags = google_tags
+        self.attributes.categories = categories
 
-    type_name: str = Field("Google", allow_mutation=False)
+    type_name: str = Field("AtlasGlossary", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
-        if v != "Google":
-            raise ValueError("must be Google")
+        if v != "AtlasGlossary":
+            raise ValueError("must be AtlasGlossary")
         return v
 
-    class Attributes(Cloud.Attributes):
-        google_service: Optional[str] = Field(
-            None, description="", alias="googleService"
-        )
-        google_project_name: Optional[str] = Field(
-            None, description="", alias="googleProjectName"
-        )
-        google_project_id: Optional[str] = Field(
-            None, description="", alias="googleProjectId"
-        )
-        google_project_number: Optional[int] = Field(
-            None, description="", alias="googleProjectNumber"
-        )
-        google_location: Optional[str] = Field(
-            None, description="", alias="googleLocation"
-        )
-        google_location_type: Optional[str] = Field(
-            None, description="", alias="googleLocationType"
+    class Attributes(Asset.Attributes):
+        short_description: Optional[str] = Field(
+            None, description="", alias="shortDescription"
         )
-        google_labels: Optional[list[GoogleLabel]] = Field(
-            None, description="", alias="googleLabels"
+        long_description: Optional[str] = Field(
+            None, description="", alias="longDescription"
         )
-        google_tags: Optional[list[GoogleTag]] = Field(
-            None, description="", alias="googleTags"
+        language: Optional[str] = Field(None, description="", alias="language")
+        usage: Optional[str] = Field(None, description="", alias="usage")
+        additional_attributes: Optional[dict[str, str]] = Field(
+            None, description="", alias="additionalAttributes"
         )
+        terms: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="terms"
+        )  # relationship
+        categories: Optional[list[AtlasGlossaryCategory]] = Field(
+            None, description="", alias="categories"
+        )  # relationship
 
-    attributes: "Google.Attributes" = Field(
-        default_factory=lambda: Google.Attributes(),
+        @classmethod
+        # @validate_arguments()
+        def create(cls, *, name: StrictStr) -> AtlasGlossary.Attributes:
+            validate_required_fields(["name"], [name])
+            return AtlasGlossary.Attributes(name=name, qualified_name=next_id())
+
+    attributes: "AtlasGlossary.Attributes" = Field(
+        default_factory=lambda: AtlasGlossary.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
+    @root_validator()
+    def update_qualified_name(cls, values):
+        if (
+            "attributes" in values
+            and values["attributes"]
+            and not values["attributes"].qualified_name
+        ):
+            values["attributes"].qualified_name = values["guid"]
+        return values
 
-class Azure(Cloud):
+    @classmethod
+    # @validate_arguments()
+    def create(cls, *, name: StrictStr) -> AtlasGlossary:
+        validate_required_fields(["name"], [name])
+        return AtlasGlossary(attributes=AtlasGlossary.Attributes.create(name=name))
+
+
+class AuthPolicy(Asset, type_name="AuthPolicy"):
     """Description"""
 
     def __setattr__(self, name, value):
-        if name in Azure._convience_properties:
+        if name in AuthPolicy._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
-        "azure_resource_id",
-        "azure_location",
-        "adls_account_secondary_location",
-        "azure_tags",
+        "policy_type",
+        "policy_service_name",
+        "policy_category",
+        "policy_sub_category",
+        "policy_users",
+        "policy_groups",
+        "policy_roles",
+        "policy_actions",
+        "policy_resources",
+        "policy_resource_category",
+        "policy_priority",
+        "is_policy_enabled",
+        "policy_mask_type",
+        "policy_validity_schedule",
+        "policy_resource_signature",
+        "policy_delegate_admin",
+        "policy_conditions",
+        "access_control",
     ]
 
     @property
-    def azure_resource_id(self) -> Optional[str]:
-        return self.attributes.azure_resource_id
+    def policy_type(self) -> Optional[AuthPolicyType]:
+        return self.attributes.policy_type
 
-    @azure_resource_id.setter
-    def azure_resource_id(self, azure_resource_id: Optional[str]):
+    @policy_type.setter
+    def policy_type(self, policy_type: Optional[AuthPolicyType]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.azure_resource_id = azure_resource_id
+        self.attributes.policy_type = policy_type
 
     @property
-    def azure_location(self) -> Optional[str]:
-        return self.attributes.azure_location
+    def policy_service_name(self) -> Optional[str]:
+        return self.attributes.policy_service_name
 
-    @azure_location.setter
-    def azure_location(self, azure_location: Optional[str]):
+    @policy_service_name.setter
+    def policy_service_name(self, policy_service_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.azure_location = azure_location
+        self.attributes.policy_service_name = policy_service_name
 
     @property
-    def adls_account_secondary_location(self) -> Optional[str]:
-        return self.attributes.adls_account_secondary_location
+    def policy_category(self) -> Optional[str]:
+        return self.attributes.policy_category
 
-    @adls_account_secondary_location.setter
-    def adls_account_secondary_location(
-        self, adls_account_secondary_location: Optional[str]
+    @policy_category.setter
+    def policy_category(self, policy_category: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.policy_category = policy_category
+
+    @property
+    def policy_sub_category(self) -> Optional[str]:
+        return self.attributes.policy_sub_category
+
+    @policy_sub_category.setter
+    def policy_sub_category(self, policy_sub_category: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.policy_sub_category = policy_sub_category
+
+    @property
+    def policy_users(self) -> Optional[set[str]]:
+        return self.attributes.policy_users
+
+    @policy_users.setter
+    def policy_users(self, policy_users: Optional[set[str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.policy_users = policy_users
+
+    @property
+    def policy_groups(self) -> Optional[set[str]]:
+        return self.attributes.policy_groups
+
+    @policy_groups.setter
+    def policy_groups(self, policy_groups: Optional[set[str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.policy_groups = policy_groups
+
+    @property
+    def policy_roles(self) -> Optional[set[str]]:
+        return self.attributes.policy_roles
+
+    @policy_roles.setter
+    def policy_roles(self, policy_roles: Optional[set[str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.policy_roles = policy_roles
+
+    @property
+    def policy_actions(self) -> Optional[set[str]]:
+        return self.attributes.policy_actions
+
+    @policy_actions.setter
+    def policy_actions(self, policy_actions: Optional[set[str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.policy_actions = policy_actions
+
+    @property
+    def policy_resources(self) -> Optional[set[str]]:
+        return self.attributes.policy_resources
+
+    @policy_resources.setter
+    def policy_resources(self, policy_resources: Optional[set[str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.policy_resources = policy_resources
+
+    @property
+    def policy_resource_category(self) -> Optional[str]:
+        return self.attributes.policy_resource_category
+
+    @policy_resource_category.setter
+    def policy_resource_category(self, policy_resource_category: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.policy_resource_category = policy_resource_category
+
+    @property
+    def policy_priority(self) -> Optional[int]:
+        return self.attributes.policy_priority
+
+    @policy_priority.setter
+    def policy_priority(self, policy_priority: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.policy_priority = policy_priority
+
+    @property
+    def is_policy_enabled(self) -> Optional[bool]:
+        return self.attributes.is_policy_enabled
+
+    @is_policy_enabled.setter
+    def is_policy_enabled(self, is_policy_enabled: Optional[bool]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.is_policy_enabled = is_policy_enabled
+
+    @property
+    def policy_mask_type(self) -> Optional[str]:
+        return self.attributes.policy_mask_type
+
+    @policy_mask_type.setter
+    def policy_mask_type(self, policy_mask_type: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.policy_mask_type = policy_mask_type
+
+    @property
+    def policy_validity_schedule(self) -> Optional[list[AuthPolicyValiditySchedule]]:
+        return self.attributes.policy_validity_schedule
+
+    @policy_validity_schedule.setter
+    def policy_validity_schedule(
+        self, policy_validity_schedule: Optional[list[AuthPolicyValiditySchedule]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.adls_account_secondary_location = (
-            adls_account_secondary_location
-        )
+        self.attributes.policy_validity_schedule = policy_validity_schedule
 
     @property
-    def azure_tags(self) -> Optional[list[AzureTag]]:
-        return self.attributes.azure_tags
+    def policy_resource_signature(self) -> Optional[str]:
+        return self.attributes.policy_resource_signature
 
-    @azure_tags.setter
-    def azure_tags(self, azure_tags: Optional[list[AzureTag]]):
+    @policy_resource_signature.setter
+    def policy_resource_signature(self, policy_resource_signature: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.azure_tags = azure_tags
+        self.attributes.policy_resource_signature = policy_resource_signature
 
-    type_name: str = Field("Azure", allow_mutation=False)
+    @property
+    def policy_delegate_admin(self) -> Optional[bool]:
+        return self.attributes.policy_delegate_admin
+
+    @policy_delegate_admin.setter
+    def policy_delegate_admin(self, policy_delegate_admin: Optional[bool]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.policy_delegate_admin = policy_delegate_admin
+
+    @property
+    def policy_conditions(self) -> Optional[list[AuthPolicyCondition]]:
+        return self.attributes.policy_conditions
+
+    @policy_conditions.setter
+    def policy_conditions(self, policy_conditions: Optional[list[AuthPolicyCondition]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.policy_conditions = policy_conditions
+
+    @property
+    def access_control(self) -> Optional[AccessControl]:
+        return self.attributes.access_control
+
+    @access_control.setter
+    def access_control(self, access_control: Optional[AccessControl]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.access_control = access_control
+
+    type_name: str = Field("AuthPolicy", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
-        if v != "Azure":
-            raise ValueError("must be Azure")
+        if v != "AuthPolicy":
+            raise ValueError("must be AuthPolicy")
         return v
 
-    class Attributes(Cloud.Attributes):
-        azure_resource_id: Optional[str] = Field(
-            None, description="", alias="azureResourceId"
+    class Attributes(Asset.Attributes):
+        policy_type: Optional[AuthPolicyType] = Field(
+            None, description="", alias="policyType"
         )
-        azure_location: Optional[str] = Field(
-            None, description="", alias="azureLocation"
+        policy_service_name: Optional[str] = Field(
+            None, description="", alias="policyServiceName"
         )
-        adls_account_secondary_location: Optional[str] = Field(
-            None, description="", alias="adlsAccountSecondaryLocation"
+        policy_category: Optional[str] = Field(
+            None, description="", alias="policyCategory"
         )
-        azure_tags: Optional[list[AzureTag]] = Field(
-            None, description="", alias="azureTags"
+        policy_sub_category: Optional[str] = Field(
+            None, description="", alias="policySubCategory"
+        )
+        policy_users: Optional[set[str]] = Field(
+            None, description="", alias="policyUsers"
+        )
+        policy_groups: Optional[set[str]] = Field(
+            None, description="", alias="policyGroups"
+        )
+        policy_roles: Optional[set[str]] = Field(
+            None, description="", alias="policyRoles"
+        )
+        policy_actions: Optional[set[str]] = Field(
+            None, description="", alias="policyActions"
+        )
+        policy_resources: Optional[set[str]] = Field(
+            None, description="", alias="policyResources"
+        )
+        policy_resource_category: Optional[str] = Field(
+            None, description="", alias="policyResourceCategory"
+        )
+        policy_priority: Optional[int] = Field(
+            None, description="", alias="policyPriority"
+        )
+        is_policy_enabled: Optional[bool] = Field(
+            None, description="", alias="isPolicyEnabled"
+        )
+        policy_mask_type: Optional[str] = Field(
+            None, description="", alias="policyMaskType"
+        )
+        policy_validity_schedule: Optional[list[AuthPolicyValiditySchedule]] = Field(
+            None, description="", alias="policyValiditySchedule"
+        )
+        policy_resource_signature: Optional[str] = Field(
+            None, description="", alias="policyResourceSignature"
+        )
+        policy_delegate_admin: Optional[bool] = Field(
+            None, description="", alias="policyDelegateAdmin"
+        )
+        policy_conditions: Optional[list[AuthPolicyCondition]] = Field(
+            None, description="", alias="policyConditions"
         )
+        access_control: Optional[AccessControl] = Field(
+            None, description="", alias="accessControl"
+        )  # relationship
 
-    attributes: "Azure.Attributes" = Field(
-        default_factory=lambda: Azure.Attributes(),
+    attributes: "AuthPolicy.Attributes" = Field(
+        default_factory=lambda: AuthPolicy.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
-class AWS(Cloud):
+class ProcessExecution(Asset, type_name="ProcessExecution"):
     """Description"""
 
     def __setattr__(self, name, value):
-        if name in AWS._convience_properties:
+        if name in ProcessExecution._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = []
+
+    type_name: str = Field("ProcessExecution", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "ProcessExecution":
+            raise ValueError("must be ProcessExecution")
+        return v
+
+
+class AtlasGlossaryTerm(Asset, type_name="AtlasGlossaryTerm"):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in AtlasGlossaryTerm._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
-        "aws_arn",
-        "aws_partition",
-        "aws_service",
-        "aws_region",
-        "aws_account_id",
-        "aws_resource_id",
-        "aws_owner_name",
-        "aws_owner_id",
-        "aws_tags",
+        "short_description",
+        "long_description",
+        "examples",
+        "abbreviation",
+        "usage",
+        "additional_attributes",
+        "translation_terms",
+        "valid_values_for",
+        "synonyms",
+        "replaced_by",
+        "valid_values",
+        "replacement_terms",
+        "see_also",
+        "translated_terms",
+        "is_a",
+        "anchor",
+        "antonyms",
+        "assigned_entities",
+        "categories",
+        "classifies",
+        "preferred_to_terms",
+        "preferred_terms",
     ]
 
     @property
-    def aws_arn(self) -> Optional[str]:
-        return self.attributes.aws_arn
+    def short_description(self) -> Optional[str]:
+        return self.attributes.short_description
 
-    @aws_arn.setter
-    def aws_arn(self, aws_arn: Optional[str]):
+    @short_description.setter
+    def short_description(self, short_description: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.aws_arn = aws_arn
+        self.attributes.short_description = short_description
 
     @property
-    def aws_partition(self) -> Optional[str]:
-        return self.attributes.aws_partition
+    def long_description(self) -> Optional[str]:
+        return self.attributes.long_description
 
-    @aws_partition.setter
-    def aws_partition(self, aws_partition: Optional[str]):
+    @long_description.setter
+    def long_description(self, long_description: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.aws_partition = aws_partition
+        self.attributes.long_description = long_description
 
     @property
-    def aws_service(self) -> Optional[str]:
-        return self.attributes.aws_service
+    def examples(self) -> Optional[set[str]]:
+        return self.attributes.examples
 
-    @aws_service.setter
-    def aws_service(self, aws_service: Optional[str]):
+    @examples.setter
+    def examples(self, examples: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.aws_service = aws_service
+        self.attributes.examples = examples
 
     @property
-    def aws_region(self) -> Optional[str]:
-        return self.attributes.aws_region
+    def abbreviation(self) -> Optional[str]:
+        return self.attributes.abbreviation
 
-    @aws_region.setter
-    def aws_region(self, aws_region: Optional[str]):
+    @abbreviation.setter
+    def abbreviation(self, abbreviation: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.aws_region = aws_region
+        self.attributes.abbreviation = abbreviation
 
     @property
-    def aws_account_id(self) -> Optional[str]:
-        return self.attributes.aws_account_id
+    def usage(self) -> Optional[str]:
+        return self.attributes.usage
 
-    @aws_account_id.setter
-    def aws_account_id(self, aws_account_id: Optional[str]):
+    @usage.setter
+    def usage(self, usage: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.aws_account_id = aws_account_id
+        self.attributes.usage = usage
 
     @property
-    def aws_resource_id(self) -> Optional[str]:
-        return self.attributes.aws_resource_id
+    def additional_attributes(self) -> Optional[dict[str, str]]:
+        return self.attributes.additional_attributes
 
-    @aws_resource_id.setter
-    def aws_resource_id(self, aws_resource_id: Optional[str]):
+    @additional_attributes.setter
+    def additional_attributes(self, additional_attributes: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.aws_resource_id = aws_resource_id
+        self.attributes.additional_attributes = additional_attributes
 
     @property
-    def aws_owner_name(self) -> Optional[str]:
-        return self.attributes.aws_owner_name
+    def translation_terms(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.translation_terms
 
-    @aws_owner_name.setter
-    def aws_owner_name(self, aws_owner_name: Optional[str]):
+    @translation_terms.setter
+    def translation_terms(self, translation_terms: Optional[list[AtlasGlossaryTerm]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.aws_owner_name = aws_owner_name
+        self.attributes.translation_terms = translation_terms
 
     @property
-    def aws_owner_id(self) -> Optional[str]:
-        return self.attributes.aws_owner_id
+    def valid_values_for(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.valid_values_for
 
-    @aws_owner_id.setter
-    def aws_owner_id(self, aws_owner_id: Optional[str]):
+    @valid_values_for.setter
+    def valid_values_for(self, valid_values_for: Optional[list[AtlasGlossaryTerm]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.aws_owner_id = aws_owner_id
+        self.attributes.valid_values_for = valid_values_for
 
     @property
-    def aws_tags(self) -> Optional[list[AwsTag]]:
-        return self.attributes.aws_tags
+    def synonyms(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.synonyms
 
-    @aws_tags.setter
-    def aws_tags(self, aws_tags: Optional[list[AwsTag]]):
+    @synonyms.setter
+    def synonyms(self, synonyms: Optional[list[AtlasGlossaryTerm]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.aws_tags = aws_tags
+        self.attributes.synonyms = synonyms
 
-    type_name: str = Field("AWS", allow_mutation=False)
+    @property
+    def replaced_by(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.replaced_by
+
+    @replaced_by.setter
+    def replaced_by(self, replaced_by: Optional[list[AtlasGlossaryTerm]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.replaced_by = replaced_by
+
+    @property
+    def valid_values(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.valid_values
+
+    @valid_values.setter
+    def valid_values(self, valid_values: Optional[list[AtlasGlossaryTerm]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.valid_values = valid_values
+
+    @property
+    def replacement_terms(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.replacement_terms
+
+    @replacement_terms.setter
+    def replacement_terms(self, replacement_terms: Optional[list[AtlasGlossaryTerm]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.replacement_terms = replacement_terms
+
+    @property
+    def see_also(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.see_also
+
+    @see_also.setter
+    def see_also(self, see_also: Optional[list[AtlasGlossaryTerm]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.see_also = see_also
+
+    @property
+    def translated_terms(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.translated_terms
+
+    @translated_terms.setter
+    def translated_terms(self, translated_terms: Optional[list[AtlasGlossaryTerm]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.translated_terms = translated_terms
+
+    @property
+    def is_a(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.is_a
+
+    @is_a.setter
+    def is_a(self, is_a: Optional[list[AtlasGlossaryTerm]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.is_a = is_a
+
+    @property
+    def anchor(self) -> AtlasGlossary:
+        return self.attributes.anchor
+
+    @anchor.setter
+    def anchor(self, anchor: AtlasGlossary):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.anchor = anchor
+
+    @property
+    def antonyms(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.antonyms
+
+    @antonyms.setter
+    def antonyms(self, antonyms: Optional[list[AtlasGlossaryTerm]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.antonyms = antonyms
+
+    @property
+    def assigned_entities(self) -> Optional[list[Referenceable]]:
+        return self.attributes.assigned_entities
+
+    @assigned_entities.setter
+    def assigned_entities(self, assigned_entities: Optional[list[Referenceable]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.assigned_entities = assigned_entities
+
+    @property
+    def categories(self) -> Optional[list[AtlasGlossaryCategory]]:
+        return self.attributes.categories
+
+    @categories.setter
+    def categories(self, categories: Optional[list[AtlasGlossaryCategory]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.categories = categories
+
+    @property
+    def classifies(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.classifies
+
+    @classifies.setter
+    def classifies(self, classifies: Optional[list[AtlasGlossaryTerm]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.classifies = classifies
+
+    @property
+    def preferred_to_terms(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.preferred_to_terms
+
+    @preferred_to_terms.setter
+    def preferred_to_terms(self, preferred_to_terms: Optional[list[AtlasGlossaryTerm]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.preferred_to_terms = preferred_to_terms
+
+    @property
+    def preferred_terms(self) -> Optional[list[AtlasGlossaryTerm]]:
+        return self.attributes.preferred_terms
+
+    @preferred_terms.setter
+    def preferred_terms(self, preferred_terms: Optional[list[AtlasGlossaryTerm]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.preferred_terms = preferred_terms
+
+    type_name: str = Field("AtlasGlossaryTerm", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
-        if v != "AWS":
-            raise ValueError("must be AWS")
+        if v != "AtlasGlossaryTerm":
+            raise ValueError("must be AtlasGlossaryTerm")
         return v
 
-    class Attributes(Cloud.Attributes):
-        aws_arn: Optional[str] = Field(None, description="", alias="awsArn")
-        aws_partition: Optional[str] = Field(None, description="", alias="awsPartition")
-        aws_service: Optional[str] = Field(None, description="", alias="awsService")
-        aws_region: Optional[str] = Field(None, description="", alias="awsRegion")
-        aws_account_id: Optional[str] = Field(
-            None, description="", alias="awsAccountId"
+    class Attributes(Asset.Attributes):
+        short_description: Optional[str] = Field(
+            None, description="", alias="shortDescription"
         )
-        aws_resource_id: Optional[str] = Field(
-            None, description="", alias="awsResourceId"
+        long_description: Optional[str] = Field(
+            None, description="", alias="longDescription"
         )
-        aws_owner_name: Optional[str] = Field(
-            None, description="", alias="awsOwnerName"
+        examples: Optional[set[str]] = Field(None, description="", alias="examples")
+        abbreviation: Optional[str] = Field(None, description="", alias="abbreviation")
+        usage: Optional[str] = Field(None, description="", alias="usage")
+        additional_attributes: Optional[dict[str, str]] = Field(
+            None, description="", alias="additionalAttributes"
         )
-        aws_owner_id: Optional[str] = Field(None, description="", alias="awsOwnerId")
-        aws_tags: Optional[list[AwsTag]] = Field(None, description="", alias="awsTags")
+        translation_terms: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="translationTerms"
+        )  # relationship
+        valid_values_for: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="validValuesFor"
+        )  # relationship
+        synonyms: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="synonyms"
+        )  # relationship
+        replaced_by: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="replacedBy"
+        )  # relationship
+        valid_values: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="validValues"
+        )  # relationship
+        replacement_terms: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="replacementTerms"
+        )  # relationship
+        see_also: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="seeAlso"
+        )  # relationship
+        translated_terms: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="translatedTerms"
+        )  # relationship
+        is_a: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="isA"
+        )  # relationship
+        anchor: AtlasGlossary = Field(
+            None, description="", alias="anchor"
+        )  # relationship
+        antonyms: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="antonyms"
+        )  # relationship
+        assigned_entities: Optional[list[Referenceable]] = Field(
+            None, description="", alias="assignedEntities"
+        )  # relationship
+        categories: Optional[list[AtlasGlossaryCategory]] = Field(
+            None, description="", alias="categories"
+        )  # relationship
+        classifies: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="classifies"
+        )  # relationship
+        preferred_to_terms: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="preferredToTerms"
+        )  # relationship
+        preferred_terms: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="preferredTerms"
+        )  # relationship
 
-    attributes: "AWS.Attributes" = Field(
-        default_factory=lambda: AWS.Attributes(),
+        @classmethod
+        # @validate_arguments()
+        def create(
+            cls,
+            *,
+            name: StrictStr,
+            anchor: Optional[AtlasGlossary] = None,
+            glossary_qualified_name: Optional[StrictStr] = None,
+            glossary_guid: Optional[StrictStr] = None,
+            categories: Optional[list[AtlasGlossaryCategory]] = None,
+        ) -> AtlasGlossaryTerm.Attributes:
+            validate_required_fields(["name"], [name])
+            validate_single_required_field(
+                ["anchor", "glossary_qualified_name", "glossary_guid"],
+                [anchor, glossary_qualified_name, glossary_guid],
+            )
+            if glossary_qualified_name:
+                anchor = AtlasGlossary()
+                anchor.unique_attributes = {"qualifiedName": glossary_qualified_name}
+            if glossary_guid:
+                anchor = AtlasGlossary()
+                anchor.guid = glossary_guid
+            return AtlasGlossaryTerm.Attributes(
+                name=name,
+                anchor=anchor,
+                categories=categories,
+                qualified_name=next_id(),
+            )
+
+    attributes: "AtlasGlossaryTerm.Attributes" = Field(
+        default_factory=lambda: AtlasGlossaryTerm.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
+    @root_validator()
+    def update_qualified_name(cls, values):
+        if (
+            "attributes" in values
+            and values["attributes"]
+            and not values["attributes"].qualified_name
+        ):
+            values["attributes"].qualified_name = values["guid"]
+        return values
+
+    @classmethod
+    # @validate_arguments()
+    def create(
+        cls,
+        *,
+        name: StrictStr,
+        anchor: Optional[AtlasGlossary] = None,
+        glossary_qualified_name: Optional[StrictStr] = None,
+        glossary_guid: Optional[StrictStr] = None,
+        categories: Optional[list[AtlasGlossaryCategory]] = None,
+    ) -> AtlasGlossaryTerm:
+        validate_required_fields(["name"], [name])
+        return cls(
+            attributes=AtlasGlossaryTerm.Attributes.create(
+                name=name,
+                anchor=anchor,
+                glossary_qualified_name=glossary_qualified_name,
+                glossary_guid=glossary_guid,
+                categories=categories,
+            )
+        )
+
+    @classmethod
+    def create_for_modification(
+        cls: type[SelfAsset],
+        qualified_name: str = "",
+        name: str = "",
+        glossary_guid: str = "",
+    ) -> SelfAsset:
+        validate_required_fields(
+            ["name", "qualified_name", "glossary_guid"],
+            [name, qualified_name, glossary_guid],
+        )
+        glossary = AtlasGlossary()
+        glossary.guid = glossary_guid
+        return cls(
+            attributes=cls.Attributes(
+                qualified_name=qualified_name, name=name, anchor=glossary
+            )
+        )
+
+
+class AuthService(Asset, type_name="AuthService"):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in AuthService._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "auth_service_type",
+        "tag_service",
+        "auth_service_is_enabled",
+        "auth_service_config",
+        "auth_service_policy_last_sync",
+    ]
+
+    @property
+    def auth_service_type(self) -> Optional[str]:
+        return self.attributes.auth_service_type
+
+    @auth_service_type.setter
+    def auth_service_type(self, auth_service_type: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.auth_service_type = auth_service_type
+
+    @property
+    def tag_service(self) -> Optional[str]:
+        return self.attributes.tag_service
+
+    @tag_service.setter
+    def tag_service(self, tag_service: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.tag_service = tag_service
+
+    @property
+    def auth_service_is_enabled(self) -> Optional[bool]:
+        return self.attributes.auth_service_is_enabled
+
+    @auth_service_is_enabled.setter
+    def auth_service_is_enabled(self, auth_service_is_enabled: Optional[bool]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.auth_service_is_enabled = auth_service_is_enabled
+
+    @property
+    def auth_service_config(self) -> Optional[dict[str, str]]:
+        return self.attributes.auth_service_config
+
+    @auth_service_config.setter
+    def auth_service_config(self, auth_service_config: Optional[dict[str, str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.auth_service_config = auth_service_config
+
+    @property
+    def auth_service_policy_last_sync(self) -> Optional[int]:
+        return self.attributes.auth_service_policy_last_sync
+
+    @auth_service_policy_last_sync.setter
+    def auth_service_policy_last_sync(
+        self, auth_service_policy_last_sync: Optional[int]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.auth_service_policy_last_sync = auth_service_policy_last_sync
+
+    type_name: str = Field("AuthService", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "AuthService":
+            raise ValueError("must be AuthService")
+        return v
+
+    class Attributes(Asset.Attributes):
+        auth_service_type: Optional[str] = Field(
+            None, description="", alias="authServiceType"
+        )
+        tag_service: Optional[str] = Field(None, description="", alias="tagService")
+        auth_service_is_enabled: Optional[bool] = Field(
+            None, description="", alias="authServiceIsEnabled"
+        )
+        auth_service_config: Optional[dict[str, str]] = Field(
+            None, description="", alias="authServiceConfig"
+        )
+        auth_service_policy_last_sync: Optional[int] = Field(
+            None, description="", alias="authServicePolicyLastSync"
+        )
+
+    attributes: "AuthService.Attributes" = Field(
+        default_factory=lambda: AuthService.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class Cloud(Asset, type_name="Cloud"):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in Cloud._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = []
+
+    type_name: str = Field("Cloud", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Cloud":
+            raise ValueError("must be Cloud")
+        return v
+
+
+class Infrastructure(Asset, type_name="Infrastructure"):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in Infrastructure._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = []
+
+    type_name: str = Field("Infrastructure", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Infrastructure":
+            raise ValueError("must be Infrastructure")
+        return v
+
 
 class BIProcess(Process):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in BIProcess._convience_properties:
             return object.__setattr__(self, name, value)
@@ -4294,14 +4365,124 @@
     attributes: "ColumnProcess.Attributes" = Field(
         default_factory=lambda: ColumnProcess.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
+class Persona(AccessControl):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in Persona._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "persona_groups",
+        "persona_users",
+        "role_id",
+    ]
+
+    @property
+    def persona_groups(self) -> Optional[set[str]]:
+        return self.attributes.persona_groups
+
+    @persona_groups.setter
+    def persona_groups(self, persona_groups: Optional[set[str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.persona_groups = persona_groups
+
+    @property
+    def persona_users(self) -> Optional[set[str]]:
+        return self.attributes.persona_users
+
+    @persona_users.setter
+    def persona_users(self, persona_users: Optional[set[str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.persona_users = persona_users
+
+    @property
+    def role_id(self) -> Optional[str]:
+        return self.attributes.role_id
+
+    @role_id.setter
+    def role_id(self, role_id: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.role_id = role_id
+
+    type_name: str = Field("Persona", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Persona":
+            raise ValueError("must be Persona")
+        return v
+
+    class Attributes(AccessControl.Attributes):
+        persona_groups: Optional[set[str]] = Field(
+            None, description="", alias="personaGroups"
+        )
+        persona_users: Optional[set[str]] = Field(
+            None, description="", alias="personaUsers"
+        )
+        role_id: Optional[str] = Field(None, description="", alias="roleId")
+
+    attributes: "Persona.Attributes" = Field(
+        default_factory=lambda: Persona.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class Purpose(AccessControl):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in Purpose._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "purpose_classifications",
+    ]
+
+    @property
+    def purpose_classifications(self) -> Optional[set[str]]:
+        return self.attributes.purpose_classifications
+
+    @purpose_classifications.setter
+    def purpose_classifications(self, purpose_classifications: Optional[set[str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.purpose_classifications = purpose_classifications
+
+    type_name: str = Field("Purpose", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Purpose":
+            raise ValueError("must be Purpose")
+        return v
+
+    class Attributes(AccessControl.Attributes):
+        purpose_classifications: Optional[set[str]] = Field(
+            None, description="", alias="purposeClassifications"
+        )
+
+    attributes: "Purpose.Attributes" = Field(
+        default_factory=lambda: Purpose.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
 class Collection(Namespace):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Collection._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -5338,270 +5519,34 @@
     attributes: "SQL.Attributes" = Field(
         default_factory=lambda: SQL.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
-class DataStudio(Google):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in DataStudio._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "google_service",
-        "google_project_name",
-        "google_project_id",
-        "google_project_number",
-        "google_location",
-        "google_location_type",
-        "google_labels",
-        "google_tags",
-        "input_to_processes",
-        "output_from_processes",
-    ]
-
-    @property
-    def google_service(self) -> Optional[str]:
-        return self.attributes.google_service
-
-    @google_service.setter
-    def google_service(self, google_service: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.google_service = google_service
-
-    @property
-    def google_project_name(self) -> Optional[str]:
-        return self.attributes.google_project_name
-
-    @google_project_name.setter
-    def google_project_name(self, google_project_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.google_project_name = google_project_name
-
-    @property
-    def google_project_id(self) -> Optional[str]:
-        return self.attributes.google_project_id
-
-    @google_project_id.setter
-    def google_project_id(self, google_project_id: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.google_project_id = google_project_id
-
-    @property
-    def google_project_number(self) -> Optional[int]:
-        return self.attributes.google_project_number
-
-    @google_project_number.setter
-    def google_project_number(self, google_project_number: Optional[int]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.google_project_number = google_project_number
-
-    @property
-    def google_location(self) -> Optional[str]:
-        return self.attributes.google_location
-
-    @google_location.setter
-    def google_location(self, google_location: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.google_location = google_location
-
-    @property
-    def google_location_type(self) -> Optional[str]:
-        return self.attributes.google_location_type
-
-    @google_location_type.setter
-    def google_location_type(self, google_location_type: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.google_location_type = google_location_type
-
-    @property
-    def google_labels(self) -> Optional[list[GoogleLabel]]:
-        return self.attributes.google_labels
-
-    @google_labels.setter
-    def google_labels(self, google_labels: Optional[list[GoogleLabel]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.google_labels = google_labels
-
-    @property
-    def google_tags(self) -> Optional[list[GoogleTag]]:
-        return self.attributes.google_tags
-
-    @google_tags.setter
-    def google_tags(self, google_tags: Optional[list[GoogleTag]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.google_tags = google_tags
-
-    @property
-    def input_to_processes(self) -> Optional[list[Process]]:
-        return self.attributes.input_to_processes
-
-    @input_to_processes.setter
-    def input_to_processes(self, input_to_processes: Optional[list[Process]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.input_to_processes = input_to_processes
-
-    @property
-    def output_from_processes(self) -> Optional[list[Process]]:
-        return self.attributes.output_from_processes
-
-    @output_from_processes.setter
-    def output_from_processes(self, output_from_processes: Optional[list[Process]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.output_from_processes = output_from_processes
-
-    type_name: str = Field("DataStudio", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "DataStudio":
-            raise ValueError("must be DataStudio")
-        return v
-
-    class Attributes(Google.Attributes):
-        google_service: Optional[str] = Field(
-            None, description="", alias="googleService"
-        )
-        google_project_name: Optional[str] = Field(
-            None, description="", alias="googleProjectName"
-        )
-        google_project_id: Optional[str] = Field(
-            None, description="", alias="googleProjectId"
-        )
-        google_project_number: Optional[int] = Field(
-            None, description="", alias="googleProjectNumber"
-        )
-        google_location: Optional[str] = Field(
-            None, description="", alias="googleLocation"
-        )
-        google_location_type: Optional[str] = Field(
-            None, description="", alias="googleLocationType"
-        )
-        google_labels: Optional[list[GoogleLabel]] = Field(
-            None, description="", alias="googleLabels"
-        )
-        google_tags: Optional[list[GoogleTag]] = Field(
-            None, description="", alias="googleTags"
-        )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
-
-    attributes: "DataStudio.Attributes" = Field(
-        default_factory=lambda: DataStudio.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class GCS(Google):
+class Google(Cloud):
     """Description"""
 
     def __setattr__(self, name, value):
-        if name in GCS._convience_properties:
+        if name in Google._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
-        "gcs_storage_class",
-        "gcs_encryption_type",
-        "gcs_e_tag",
-        "gcs_requester_pays",
-        "gcs_access_control",
-        "gcs_meta_generation_id",
         "google_service",
         "google_project_name",
         "google_project_id",
         "google_project_number",
         "google_location",
         "google_location_type",
         "google_labels",
         "google_tags",
-        "input_to_processes",
-        "output_from_processes",
     ]
 
     @property
-    def gcs_storage_class(self) -> Optional[str]:
-        return self.attributes.gcs_storage_class
-
-    @gcs_storage_class.setter
-    def gcs_storage_class(self, gcs_storage_class: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.gcs_storage_class = gcs_storage_class
-
-    @property
-    def gcs_encryption_type(self) -> Optional[str]:
-        return self.attributes.gcs_encryption_type
-
-    @gcs_encryption_type.setter
-    def gcs_encryption_type(self, gcs_encryption_type: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.gcs_encryption_type = gcs_encryption_type
-
-    @property
-    def gcs_e_tag(self) -> Optional[str]:
-        return self.attributes.gcs_e_tag
-
-    @gcs_e_tag.setter
-    def gcs_e_tag(self, gcs_e_tag: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.gcs_e_tag = gcs_e_tag
-
-    @property
-    def gcs_requester_pays(self) -> Optional[bool]:
-        return self.attributes.gcs_requester_pays
-
-    @gcs_requester_pays.setter
-    def gcs_requester_pays(self, gcs_requester_pays: Optional[bool]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.gcs_requester_pays = gcs_requester_pays
-
-    @property
-    def gcs_access_control(self) -> Optional[str]:
-        return self.attributes.gcs_access_control
-
-    @gcs_access_control.setter
-    def gcs_access_control(self, gcs_access_control: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.gcs_access_control = gcs_access_control
-
-    @property
-    def gcs_meta_generation_id(self) -> Optional[int]:
-        return self.attributes.gcs_meta_generation_id
-
-    @gcs_meta_generation_id.setter
-    def gcs_meta_generation_id(self, gcs_meta_generation_id: Optional[int]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.gcs_meta_generation_id = gcs_meta_generation_id
-
-    @property
     def google_service(self) -> Optional[str]:
         return self.attributes.google_service
 
     @google_service.setter
     def google_service(self, google_service: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -5673,265 +5618,23 @@
 
     @google_tags.setter
     def google_tags(self, google_tags: Optional[list[GoogleTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_tags = google_tags
 
-    @property
-    def input_to_processes(self) -> Optional[list[Process]]:
-        return self.attributes.input_to_processes
-
-    @input_to_processes.setter
-    def input_to_processes(self, input_to_processes: Optional[list[Process]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.input_to_processes = input_to_processes
-
-    @property
-    def output_from_processes(self) -> Optional[list[Process]]:
-        return self.attributes.output_from_processes
-
-    @output_from_processes.setter
-    def output_from_processes(self, output_from_processes: Optional[list[Process]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.output_from_processes = output_from_processes
-
-    type_name: str = Field("GCS", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "GCS":
-            raise ValueError("must be GCS")
-        return v
-
-    class Attributes(Google.Attributes):
-        gcs_storage_class: Optional[str] = Field(
-            None, description="", alias="gcsStorageClass"
-        )
-        gcs_encryption_type: Optional[str] = Field(
-            None, description="", alias="gcsEncryptionType"
-        )
-        gcs_e_tag: Optional[str] = Field(None, description="", alias="gcsETag")
-        gcs_requester_pays: Optional[bool] = Field(
-            None, description="", alias="gcsRequesterPays"
-        )
-        gcs_access_control: Optional[str] = Field(
-            None, description="", alias="gcsAccessControl"
-        )
-        gcs_meta_generation_id: Optional[int] = Field(
-            None, description="", alias="gcsMetaGenerationId"
-        )
-        google_service: Optional[str] = Field(
-            None, description="", alias="googleService"
-        )
-        google_project_name: Optional[str] = Field(
-            None, description="", alias="googleProjectName"
-        )
-        google_project_id: Optional[str] = Field(
-            None, description="", alias="googleProjectId"
-        )
-        google_project_number: Optional[int] = Field(
-            None, description="", alias="googleProjectNumber"
-        )
-        google_location: Optional[str] = Field(
-            None, description="", alias="googleLocation"
-        )
-        google_location_type: Optional[str] = Field(
-            None, description="", alias="googleLocationType"
-        )
-        google_labels: Optional[list[GoogleLabel]] = Field(
-            None, description="", alias="googleLabels"
-        )
-        google_tags: Optional[list[GoogleTag]] = Field(
-            None, description="", alias="googleTags"
-        )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
-
-    attributes: "GCS.Attributes" = Field(
-        default_factory=lambda: GCS.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class DataStudioAsset(DataStudio):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in DataStudioAsset._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "data_studio_asset_type",
-        "data_studio_asset_title",
-        "data_studio_asset_owner",
-        "is_trashed_data_studio_asset",
-        "google_service",
-        "google_project_name",
-        "google_project_id",
-        "google_project_number",
-        "google_location",
-        "google_location_type",
-        "google_labels",
-        "google_tags",
-    ]
-
-    @property
-    def data_studio_asset_type(self) -> Optional[GoogleDatastudioAssetType]:
-        return self.attributes.data_studio_asset_type
-
-    @data_studio_asset_type.setter
-    def data_studio_asset_type(
-        self, data_studio_asset_type: Optional[GoogleDatastudioAssetType]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.data_studio_asset_type = data_studio_asset_type
-
-    @property
-    def data_studio_asset_title(self) -> Optional[str]:
-        return self.attributes.data_studio_asset_title
-
-    @data_studio_asset_title.setter
-    def data_studio_asset_title(self, data_studio_asset_title: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.data_studio_asset_title = data_studio_asset_title
-
-    @property
-    def data_studio_asset_owner(self) -> Optional[str]:
-        return self.attributes.data_studio_asset_owner
-
-    @data_studio_asset_owner.setter
-    def data_studio_asset_owner(self, data_studio_asset_owner: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.data_studio_asset_owner = data_studio_asset_owner
-
-    @property
-    def is_trashed_data_studio_asset(self) -> Optional[bool]:
-        return self.attributes.is_trashed_data_studio_asset
-
-    @is_trashed_data_studio_asset.setter
-    def is_trashed_data_studio_asset(
-        self, is_trashed_data_studio_asset: Optional[bool]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.is_trashed_data_studio_asset = is_trashed_data_studio_asset
-
-    @property
-    def google_service(self) -> Optional[str]:
-        return self.attributes.google_service
-
-    @google_service.setter
-    def google_service(self, google_service: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.google_service = google_service
-
-    @property
-    def google_project_name(self) -> Optional[str]:
-        return self.attributes.google_project_name
-
-    @google_project_name.setter
-    def google_project_name(self, google_project_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.google_project_name = google_project_name
-
-    @property
-    def google_project_id(self) -> Optional[str]:
-        return self.attributes.google_project_id
-
-    @google_project_id.setter
-    def google_project_id(self, google_project_id: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.google_project_id = google_project_id
-
-    @property
-    def google_project_number(self) -> Optional[int]:
-        return self.attributes.google_project_number
-
-    @google_project_number.setter
-    def google_project_number(self, google_project_number: Optional[int]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.google_project_number = google_project_number
-
-    @property
-    def google_location(self) -> Optional[str]:
-        return self.attributes.google_location
-
-    @google_location.setter
-    def google_location(self, google_location: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.google_location = google_location
-
-    @property
-    def google_location_type(self) -> Optional[str]:
-        return self.attributes.google_location_type
-
-    @google_location_type.setter
-    def google_location_type(self, google_location_type: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.google_location_type = google_location_type
-
-    @property
-    def google_labels(self) -> Optional[list[GoogleLabel]]:
-        return self.attributes.google_labels
-
-    @google_labels.setter
-    def google_labels(self, google_labels: Optional[list[GoogleLabel]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.google_labels = google_labels
-
-    @property
-    def google_tags(self) -> Optional[list[GoogleTag]]:
-        return self.attributes.google_tags
-
-    @google_tags.setter
-    def google_tags(self, google_tags: Optional[list[GoogleTag]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.google_tags = google_tags
-
-    type_name: str = Field("DataStudioAsset", allow_mutation=False)
+    type_name: str = Field("Google", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
-        if v != "DataStudioAsset":
-            raise ValueError("must be DataStudioAsset")
+        if v != "Google":
+            raise ValueError("must be Google")
         return v
 
-    class Attributes(DataStudio.Attributes):
-        data_studio_asset_type: Optional[GoogleDatastudioAssetType] = Field(
-            None, description="", alias="dataStudioAssetType"
-        )
-        data_studio_asset_title: Optional[str] = Field(
-            None, description="", alias="dataStudioAssetTitle"
-        )
-        data_studio_asset_owner: Optional[str] = Field(
-            None, description="", alias="dataStudioAssetOwner"
-        )
-        is_trashed_data_studio_asset: Optional[bool] = Field(
-            None, description="", alias="isTrashedDataStudioAsset"
-        )
+    class Attributes(Cloud.Attributes):
         google_service: Optional[str] = Field(
             None, description="", alias="googleService"
         )
         google_project_name: Optional[str] = Field(
             None, description="", alias="googleProjectName"
         )
         google_project_id: Optional[str] = Field(
@@ -5949,48 +5652,37 @@
         google_labels: Optional[list[GoogleLabel]] = Field(
             None, description="", alias="googleLabels"
         )
         google_tags: Optional[list[GoogleTag]] = Field(
             None, description="", alias="googleTags"
         )
 
-    attributes: "DataStudioAsset.Attributes" = Field(
-        default_factory=lambda: DataStudioAsset.Attributes(),
+    attributes: "Google.Attributes" = Field(
+        default_factory=lambda: Google.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
-class ADLS(ObjectStore):
+class Azure(Cloud):
     """Description"""
 
     def __setattr__(self, name, value):
-        if name in ADLS._convience_properties:
+        if name in Azure._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
-        "adls_account_qualified_name",
         "azure_resource_id",
         "azure_location",
         "adls_account_secondary_location",
         "azure_tags",
     ]
 
     @property
-    def adls_account_qualified_name(self) -> Optional[str]:
-        return self.attributes.adls_account_qualified_name
-
-    @adls_account_qualified_name.setter
-    def adls_account_qualified_name(self, adls_account_qualified_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.adls_account_qualified_name = adls_account_qualified_name
-
-    @property
     def azure_resource_id(self) -> Optional[str]:
         return self.attributes.azure_resource_id
 
     @azure_resource_id.setter
     def azure_resource_id(self, azure_resource_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -6026,89 +5718,64 @@
 
     @azure_tags.setter
     def azure_tags(self, azure_tags: Optional[list[AzureTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.azure_tags = azure_tags
 
-    type_name: str = Field("ADLS", allow_mutation=False)
+    type_name: str = Field("Azure", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
-        if v != "ADLS":
-            raise ValueError("must be ADLS")
+        if v != "Azure":
+            raise ValueError("must be Azure")
         return v
 
-    class Attributes(ObjectStore.Attributes):
-        adls_account_qualified_name: Optional[str] = Field(
-            None, description="", alias="adlsAccountQualifiedName"
-        )
+    class Attributes(Cloud.Attributes):
         azure_resource_id: Optional[str] = Field(
             None, description="", alias="azureResourceId"
         )
         azure_location: Optional[str] = Field(
             None, description="", alias="azureLocation"
         )
         adls_account_secondary_location: Optional[str] = Field(
             None, description="", alias="adlsAccountSecondaryLocation"
         )
         azure_tags: Optional[list[AzureTag]] = Field(
             None, description="", alias="azureTags"
         )
 
-    attributes: "ADLS.Attributes" = Field(
-        default_factory=lambda: ADLS.Attributes(),
+    attributes: "Azure.Attributes" = Field(
+        default_factory=lambda: Azure.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
-class S3(ObjectStore):
+class AWS(Cloud):
     """Description"""
 
     def __setattr__(self, name, value):
-        if name in S3._convience_properties:
+        if name in AWS._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
-        "s3_e_tag",
-        "s3_encryption",
         "aws_arn",
         "aws_partition",
         "aws_service",
         "aws_region",
         "aws_account_id",
         "aws_resource_id",
         "aws_owner_name",
         "aws_owner_id",
         "aws_tags",
     ]
 
     @property
-    def s3_e_tag(self) -> Optional[str]:
-        return self.attributes.s3_e_tag
-
-    @s3_e_tag.setter
-    def s3_e_tag(self, s3_e_tag: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.s3_e_tag = s3_e_tag
-
-    @property
-    def s3_encryption(self) -> Optional[str]:
-        return self.attributes.s3_encryption
-
-    @s3_encryption.setter
-    def s3_encryption(self, s3_encryption: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.s3_encryption = s3_encryption
-
-    @property
     def aws_arn(self) -> Optional[str]:
         return self.attributes.aws_arn
 
     @aws_arn.setter
     def aws_arn(self, aws_arn: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -6190,25 +5857,23 @@
 
     @aws_tags.setter
     def aws_tags(self, aws_tags: Optional[list[AwsTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.aws_tags = aws_tags
 
-    type_name: str = Field("S3", allow_mutation=False)
+    type_name: str = Field("AWS", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
-        if v != "S3":
-            raise ValueError("must be S3")
+        if v != "AWS":
+            raise ValueError("must be AWS")
         return v
 
-    class Attributes(ObjectStore.Attributes):
-        s3_e_tag: Optional[str] = Field(None, description="", alias="s3ETag")
-        s3_encryption: Optional[str] = Field(None, description="", alias="s3Encryption")
+    class Attributes(Cloud.Attributes):
         aws_arn: Optional[str] = Field(None, description="", alias="awsArn")
         aws_partition: Optional[str] = Field(None, description="", alias="awsPartition")
         aws_service: Optional[str] = Field(None, description="", alias="awsService")
         aws_region: Optional[str] = Field(None, description="", alias="awsRegion")
         aws_account_id: Optional[str] = Field(
             None, description="", alias="awsAccountId"
         )
@@ -6217,16 +5882,16 @@
         )
         aws_owner_name: Optional[str] = Field(
             None, description="", alias="awsOwnerName"
         )
         aws_owner_id: Optional[str] = Field(None, description="", alias="awsOwnerId")
         aws_tags: Optional[list[AwsTag]] = Field(None, description="", alias="awsTags")
 
-    attributes: "S3.Attributes" = Field(
-        default_factory=lambda: S3.Attributes(),
+    attributes: "AWS.Attributes" = Field(
+        default_factory=lambda: AWS.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class DbtColumnProcess(Dbt):
     """Description"""
@@ -6621,14 +6286,560 @@
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Kafka":
             raise ValueError("must be Kafka")
         return v
 
 
+class S3(ObjectStore):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in S3._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "s3_e_tag",
+        "s3_encryption",
+        "aws_arn",
+        "aws_partition",
+        "aws_service",
+        "aws_region",
+        "aws_account_id",
+        "aws_resource_id",
+        "aws_owner_name",
+        "aws_owner_id",
+        "aws_tags",
+    ]
+
+    @property
+    def s3_e_tag(self) -> Optional[str]:
+        return self.attributes.s3_e_tag
+
+    @s3_e_tag.setter
+    def s3_e_tag(self, s3_e_tag: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.s3_e_tag = s3_e_tag
+
+    @property
+    def s3_encryption(self) -> Optional[str]:
+        return self.attributes.s3_encryption
+
+    @s3_encryption.setter
+    def s3_encryption(self, s3_encryption: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.s3_encryption = s3_encryption
+
+    @property
+    def aws_arn(self) -> Optional[str]:
+        return self.attributes.aws_arn
+
+    @aws_arn.setter
+    def aws_arn(self, aws_arn: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.aws_arn = aws_arn
+
+    @property
+    def aws_partition(self) -> Optional[str]:
+        return self.attributes.aws_partition
+
+    @aws_partition.setter
+    def aws_partition(self, aws_partition: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.aws_partition = aws_partition
+
+    @property
+    def aws_service(self) -> Optional[str]:
+        return self.attributes.aws_service
+
+    @aws_service.setter
+    def aws_service(self, aws_service: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.aws_service = aws_service
+
+    @property
+    def aws_region(self) -> Optional[str]:
+        return self.attributes.aws_region
+
+    @aws_region.setter
+    def aws_region(self, aws_region: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.aws_region = aws_region
+
+    @property
+    def aws_account_id(self) -> Optional[str]:
+        return self.attributes.aws_account_id
+
+    @aws_account_id.setter
+    def aws_account_id(self, aws_account_id: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.aws_account_id = aws_account_id
+
+    @property
+    def aws_resource_id(self) -> Optional[str]:
+        return self.attributes.aws_resource_id
+
+    @aws_resource_id.setter
+    def aws_resource_id(self, aws_resource_id: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.aws_resource_id = aws_resource_id
+
+    @property
+    def aws_owner_name(self) -> Optional[str]:
+        return self.attributes.aws_owner_name
+
+    @aws_owner_name.setter
+    def aws_owner_name(self, aws_owner_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.aws_owner_name = aws_owner_name
+
+    @property
+    def aws_owner_id(self) -> Optional[str]:
+        return self.attributes.aws_owner_id
+
+    @aws_owner_id.setter
+    def aws_owner_id(self, aws_owner_id: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.aws_owner_id = aws_owner_id
+
+    @property
+    def aws_tags(self) -> Optional[list[AwsTag]]:
+        return self.attributes.aws_tags
+
+    @aws_tags.setter
+    def aws_tags(self, aws_tags: Optional[list[AwsTag]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.aws_tags = aws_tags
+
+    type_name: str = Field("S3", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "S3":
+            raise ValueError("must be S3")
+        return v
+
+    class Attributes(ObjectStore.Attributes):
+        s3_e_tag: Optional[str] = Field(None, description="", alias="s3ETag")
+        s3_encryption: Optional[str] = Field(None, description="", alias="s3Encryption")
+        aws_arn: Optional[str] = Field(None, description="", alias="awsArn")
+        aws_partition: Optional[str] = Field(None, description="", alias="awsPartition")
+        aws_service: Optional[str] = Field(None, description="", alias="awsService")
+        aws_region: Optional[str] = Field(None, description="", alias="awsRegion")
+        aws_account_id: Optional[str] = Field(
+            None, description="", alias="awsAccountId"
+        )
+        aws_resource_id: Optional[str] = Field(
+            None, description="", alias="awsResourceId"
+        )
+        aws_owner_name: Optional[str] = Field(
+            None, description="", alias="awsOwnerName"
+        )
+        aws_owner_id: Optional[str] = Field(None, description="", alias="awsOwnerId")
+        aws_tags: Optional[list[AwsTag]] = Field(None, description="", alias="awsTags")
+
+    attributes: "S3.Attributes" = Field(
+        default_factory=lambda: S3.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class ADLS(Azure):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in ADLS._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "adls_account_qualified_name",
+        "azure_resource_id",
+        "azure_location",
+        "adls_account_secondary_location",
+        "azure_tags",
+        "input_to_processes",
+        "output_from_processes",
+    ]
+
+    @property
+    def adls_account_qualified_name(self) -> Optional[str]:
+        return self.attributes.adls_account_qualified_name
+
+    @adls_account_qualified_name.setter
+    def adls_account_qualified_name(self, adls_account_qualified_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.adls_account_qualified_name = adls_account_qualified_name
+
+    @property
+    def azure_resource_id(self) -> Optional[str]:
+        return self.attributes.azure_resource_id
+
+    @azure_resource_id.setter
+    def azure_resource_id(self, azure_resource_id: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.azure_resource_id = azure_resource_id
+
+    @property
+    def azure_location(self) -> Optional[str]:
+        return self.attributes.azure_location
+
+    @azure_location.setter
+    def azure_location(self, azure_location: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.azure_location = azure_location
+
+    @property
+    def adls_account_secondary_location(self) -> Optional[str]:
+        return self.attributes.adls_account_secondary_location
+
+    @adls_account_secondary_location.setter
+    def adls_account_secondary_location(
+        self, adls_account_secondary_location: Optional[str]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.adls_account_secondary_location = (
+            adls_account_secondary_location
+        )
+
+    @property
+    def azure_tags(self) -> Optional[list[AzureTag]]:
+        return self.attributes.azure_tags
+
+    @azure_tags.setter
+    def azure_tags(self, azure_tags: Optional[list[AzureTag]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.azure_tags = azure_tags
+
+    @property
+    def input_to_processes(self) -> Optional[list[Process]]:
+        return self.attributes.input_to_processes
+
+    @input_to_processes.setter
+    def input_to_processes(self, input_to_processes: Optional[list[Process]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.input_to_processes = input_to_processes
+
+    @property
+    def output_from_processes(self) -> Optional[list[Process]]:
+        return self.attributes.output_from_processes
+
+    @output_from_processes.setter
+    def output_from_processes(self, output_from_processes: Optional[list[Process]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.output_from_processes = output_from_processes
+
+    type_name: str = Field("ADLS", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "ADLS":
+            raise ValueError("must be ADLS")
+        return v
+
+    class Attributes(Azure.Attributes):
+        adls_account_qualified_name: Optional[str] = Field(
+            None, description="", alias="adlsAccountQualifiedName"
+        )
+        azure_resource_id: Optional[str] = Field(
+            None, description="", alias="azureResourceId"
+        )
+        azure_location: Optional[str] = Field(
+            None, description="", alias="azureLocation"
+        )
+        adls_account_secondary_location: Optional[str] = Field(
+            None, description="", alias="adlsAccountSecondaryLocation"
+        )
+        azure_tags: Optional[list[AzureTag]] = Field(
+            None, description="", alias="azureTags"
+        )
+        input_to_processes: Optional[list[Process]] = Field(
+            None, description="", alias="inputToProcesses"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
+
+    attributes: "ADLS.Attributes" = Field(
+        default_factory=lambda: ADLS.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class GCS(Google):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in GCS._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "gcs_storage_class",
+        "gcs_encryption_type",
+        "gcs_e_tag",
+        "gcs_requester_pays",
+        "gcs_access_control",
+        "gcs_meta_generation_id",
+        "google_service",
+        "google_project_name",
+        "google_project_id",
+        "google_project_number",
+        "google_location",
+        "google_location_type",
+        "google_labels",
+        "google_tags",
+        "input_to_processes",
+        "output_from_processes",
+    ]
+
+    @property
+    def gcs_storage_class(self) -> Optional[str]:
+        return self.attributes.gcs_storage_class
+
+    @gcs_storage_class.setter
+    def gcs_storage_class(self, gcs_storage_class: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.gcs_storage_class = gcs_storage_class
+
+    @property
+    def gcs_encryption_type(self) -> Optional[str]:
+        return self.attributes.gcs_encryption_type
+
+    @gcs_encryption_type.setter
+    def gcs_encryption_type(self, gcs_encryption_type: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.gcs_encryption_type = gcs_encryption_type
+
+    @property
+    def gcs_e_tag(self) -> Optional[str]:
+        return self.attributes.gcs_e_tag
+
+    @gcs_e_tag.setter
+    def gcs_e_tag(self, gcs_e_tag: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.gcs_e_tag = gcs_e_tag
+
+    @property
+    def gcs_requester_pays(self) -> Optional[bool]:
+        return self.attributes.gcs_requester_pays
+
+    @gcs_requester_pays.setter
+    def gcs_requester_pays(self, gcs_requester_pays: Optional[bool]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.gcs_requester_pays = gcs_requester_pays
+
+    @property
+    def gcs_access_control(self) -> Optional[str]:
+        return self.attributes.gcs_access_control
+
+    @gcs_access_control.setter
+    def gcs_access_control(self, gcs_access_control: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.gcs_access_control = gcs_access_control
+
+    @property
+    def gcs_meta_generation_id(self) -> Optional[int]:
+        return self.attributes.gcs_meta_generation_id
+
+    @gcs_meta_generation_id.setter
+    def gcs_meta_generation_id(self, gcs_meta_generation_id: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.gcs_meta_generation_id = gcs_meta_generation_id
+
+    @property
+    def google_service(self) -> Optional[str]:
+        return self.attributes.google_service
+
+    @google_service.setter
+    def google_service(self, google_service: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.google_service = google_service
+
+    @property
+    def google_project_name(self) -> Optional[str]:
+        return self.attributes.google_project_name
+
+    @google_project_name.setter
+    def google_project_name(self, google_project_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.google_project_name = google_project_name
+
+    @property
+    def google_project_id(self) -> Optional[str]:
+        return self.attributes.google_project_id
+
+    @google_project_id.setter
+    def google_project_id(self, google_project_id: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.google_project_id = google_project_id
+
+    @property
+    def google_project_number(self) -> Optional[int]:
+        return self.attributes.google_project_number
+
+    @google_project_number.setter
+    def google_project_number(self, google_project_number: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.google_project_number = google_project_number
+
+    @property
+    def google_location(self) -> Optional[str]:
+        return self.attributes.google_location
+
+    @google_location.setter
+    def google_location(self, google_location: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.google_location = google_location
+
+    @property
+    def google_location_type(self) -> Optional[str]:
+        return self.attributes.google_location_type
+
+    @google_location_type.setter
+    def google_location_type(self, google_location_type: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.google_location_type = google_location_type
+
+    @property
+    def google_labels(self) -> Optional[list[GoogleLabel]]:
+        return self.attributes.google_labels
+
+    @google_labels.setter
+    def google_labels(self, google_labels: Optional[list[GoogleLabel]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.google_labels = google_labels
+
+    @property
+    def google_tags(self) -> Optional[list[GoogleTag]]:
+        return self.attributes.google_tags
+
+    @google_tags.setter
+    def google_tags(self, google_tags: Optional[list[GoogleTag]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.google_tags = google_tags
+
+    @property
+    def input_to_processes(self) -> Optional[list[Process]]:
+        return self.attributes.input_to_processes
+
+    @input_to_processes.setter
+    def input_to_processes(self, input_to_processes: Optional[list[Process]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.input_to_processes = input_to_processes
+
+    @property
+    def output_from_processes(self) -> Optional[list[Process]]:
+        return self.attributes.output_from_processes
+
+    @output_from_processes.setter
+    def output_from_processes(self, output_from_processes: Optional[list[Process]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.output_from_processes = output_from_processes
+
+    type_name: str = Field("GCS", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "GCS":
+            raise ValueError("must be GCS")
+        return v
+
+    class Attributes(Google.Attributes):
+        gcs_storage_class: Optional[str] = Field(
+            None, description="", alias="gcsStorageClass"
+        )
+        gcs_encryption_type: Optional[str] = Field(
+            None, description="", alias="gcsEncryptionType"
+        )
+        gcs_e_tag: Optional[str] = Field(None, description="", alias="gcsETag")
+        gcs_requester_pays: Optional[bool] = Field(
+            None, description="", alias="gcsRequesterPays"
+        )
+        gcs_access_control: Optional[str] = Field(
+            None, description="", alias="gcsAccessControl"
+        )
+        gcs_meta_generation_id: Optional[int] = Field(
+            None, description="", alias="gcsMetaGenerationId"
+        )
+        google_service: Optional[str] = Field(
+            None, description="", alias="googleService"
+        )
+        google_project_name: Optional[str] = Field(
+            None, description="", alias="googleProjectName"
+        )
+        google_project_id: Optional[str] = Field(
+            None, description="", alias="googleProjectId"
+        )
+        google_project_number: Optional[int] = Field(
+            None, description="", alias="googleProjectNumber"
+        )
+        google_location: Optional[str] = Field(
+            None, description="", alias="googleLocation"
+        )
+        google_location_type: Optional[str] = Field(
+            None, description="", alias="googleLocationType"
+        )
+        google_labels: Optional[list[GoogleLabel]] = Field(
+            None, description="", alias="googleLabels"
+        )
+        google_tags: Optional[list[GoogleTag]] = Field(
+            None, description="", alias="googleTags"
+        )
+        input_to_processes: Optional[list[Process]] = Field(
+            None, description="", alias="inputToProcesses"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
+
+    attributes: "GCS.Attributes" = Field(
+        default_factory=lambda: GCS.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
 class MonteCarlo(DataQuality):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in MonteCarlo._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -6799,14 +7010,182 @@
     attributes: "Metric.Attributes" = Field(
         default_factory=lambda: Metric.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
+class DataStudio(Google):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in DataStudio._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "google_service",
+        "google_project_name",
+        "google_project_id",
+        "google_project_number",
+        "google_location",
+        "google_location_type",
+        "google_labels",
+        "google_tags",
+        "input_to_processes",
+        "output_from_processes",
+    ]
+
+    @property
+    def google_service(self) -> Optional[str]:
+        return self.attributes.google_service
+
+    @google_service.setter
+    def google_service(self, google_service: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.google_service = google_service
+
+    @property
+    def google_project_name(self) -> Optional[str]:
+        return self.attributes.google_project_name
+
+    @google_project_name.setter
+    def google_project_name(self, google_project_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.google_project_name = google_project_name
+
+    @property
+    def google_project_id(self) -> Optional[str]:
+        return self.attributes.google_project_id
+
+    @google_project_id.setter
+    def google_project_id(self, google_project_id: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.google_project_id = google_project_id
+
+    @property
+    def google_project_number(self) -> Optional[int]:
+        return self.attributes.google_project_number
+
+    @google_project_number.setter
+    def google_project_number(self, google_project_number: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.google_project_number = google_project_number
+
+    @property
+    def google_location(self) -> Optional[str]:
+        return self.attributes.google_location
+
+    @google_location.setter
+    def google_location(self, google_location: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.google_location = google_location
+
+    @property
+    def google_location_type(self) -> Optional[str]:
+        return self.attributes.google_location_type
+
+    @google_location_type.setter
+    def google_location_type(self, google_location_type: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.google_location_type = google_location_type
+
+    @property
+    def google_labels(self) -> Optional[list[GoogleLabel]]:
+        return self.attributes.google_labels
+
+    @google_labels.setter
+    def google_labels(self, google_labels: Optional[list[GoogleLabel]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.google_labels = google_labels
+
+    @property
+    def google_tags(self) -> Optional[list[GoogleTag]]:
+        return self.attributes.google_tags
+
+    @google_tags.setter
+    def google_tags(self, google_tags: Optional[list[GoogleTag]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.google_tags = google_tags
+
+    @property
+    def input_to_processes(self) -> Optional[list[Process]]:
+        return self.attributes.input_to_processes
+
+    @input_to_processes.setter
+    def input_to_processes(self, input_to_processes: Optional[list[Process]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.input_to_processes = input_to_processes
+
+    @property
+    def output_from_processes(self) -> Optional[list[Process]]:
+        return self.attributes.output_from_processes
+
+    @output_from_processes.setter
+    def output_from_processes(self, output_from_processes: Optional[list[Process]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.output_from_processes = output_from_processes
+
+    type_name: str = Field("DataStudio", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "DataStudio":
+            raise ValueError("must be DataStudio")
+        return v
+
+    class Attributes(Google.Attributes):
+        google_service: Optional[str] = Field(
+            None, description="", alias="googleService"
+        )
+        google_project_name: Optional[str] = Field(
+            None, description="", alias="googleProjectName"
+        )
+        google_project_id: Optional[str] = Field(
+            None, description="", alias="googleProjectId"
+        )
+        google_project_number: Optional[int] = Field(
+            None, description="", alias="googleProjectNumber"
+        )
+        google_location: Optional[str] = Field(
+            None, description="", alias="googleLocation"
+        )
+        google_location_type: Optional[str] = Field(
+            None, description="", alias="googleLocationType"
+        )
+        google_labels: Optional[list[GoogleLabel]] = Field(
+            None, description="", alias="googleLabels"
+        )
+        google_tags: Optional[list[GoogleTag]] = Field(
+            None, description="", alias="googleTags"
+        )
+        input_to_processes: Optional[list[Process]] = Field(
+            None, description="", alias="inputToProcesses"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
+
+    attributes: "DataStudio.Attributes" = Field(
+        default_factory=lambda: DataStudio.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
 class Metabase(BI):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Metabase._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -7165,14 +7544,132 @@
     attributes: "Preset.Attributes" = Field(
         default_factory=lambda: Preset.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
+class Sigma(BI):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in Sigma._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "sigma_workbook_qualified_name",
+        "sigma_workbook_name",
+        "sigma_page_qualified_name",
+        "sigma_page_name",
+        "sigma_data_element_qualified_name",
+        "sigma_data_element_name",
+    ]
+
+    @property
+    def sigma_workbook_qualified_name(self) -> Optional[str]:
+        return self.attributes.sigma_workbook_qualified_name
+
+    @sigma_workbook_qualified_name.setter
+    def sigma_workbook_qualified_name(
+        self, sigma_workbook_qualified_name: Optional[str]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.sigma_workbook_qualified_name = sigma_workbook_qualified_name
+
+    @property
+    def sigma_workbook_name(self) -> Optional[str]:
+        return self.attributes.sigma_workbook_name
+
+    @sigma_workbook_name.setter
+    def sigma_workbook_name(self, sigma_workbook_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.sigma_workbook_name = sigma_workbook_name
+
+    @property
+    def sigma_page_qualified_name(self) -> Optional[str]:
+        return self.attributes.sigma_page_qualified_name
+
+    @sigma_page_qualified_name.setter
+    def sigma_page_qualified_name(self, sigma_page_qualified_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.sigma_page_qualified_name = sigma_page_qualified_name
+
+    @property
+    def sigma_page_name(self) -> Optional[str]:
+        return self.attributes.sigma_page_name
+
+    @sigma_page_name.setter
+    def sigma_page_name(self, sigma_page_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.sigma_page_name = sigma_page_name
+
+    @property
+    def sigma_data_element_qualified_name(self) -> Optional[str]:
+        return self.attributes.sigma_data_element_qualified_name
+
+    @sigma_data_element_qualified_name.setter
+    def sigma_data_element_qualified_name(
+        self, sigma_data_element_qualified_name: Optional[str]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.sigma_data_element_qualified_name = (
+            sigma_data_element_qualified_name
+        )
+
+    @property
+    def sigma_data_element_name(self) -> Optional[str]:
+        return self.attributes.sigma_data_element_name
+
+    @sigma_data_element_name.setter
+    def sigma_data_element_name(self, sigma_data_element_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.sigma_data_element_name = sigma_data_element_name
+
+    type_name: str = Field("Sigma", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Sigma":
+            raise ValueError("must be Sigma")
+        return v
+
+    class Attributes(BI.Attributes):
+        sigma_workbook_qualified_name: Optional[str] = Field(
+            None, description="", alias="sigmaWorkbookQualifiedName"
+        )
+        sigma_workbook_name: Optional[str] = Field(
+            None, description="", alias="sigmaWorkbookName"
+        )
+        sigma_page_qualified_name: Optional[str] = Field(
+            None, description="", alias="sigmaPageQualifiedName"
+        )
+        sigma_page_name: Optional[str] = Field(
+            None, description="", alias="sigmaPageName"
+        )
+        sigma_data_element_qualified_name: Optional[str] = Field(
+            None, description="", alias="sigmaDataElementQualifiedName"
+        )
+        sigma_data_element_name: Optional[str] = Field(
+            None, description="", alias="sigmaDataElementName"
+        )
+
+    attributes: "Sigma.Attributes" = Field(
+        default_factory=lambda: Sigma.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
 class Mode(BI):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Mode._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -7317,132 +7814,14 @@
     attributes: "Mode.Attributes" = Field(
         default_factory=lambda: Mode.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
-class Sigma(BI):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in Sigma._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "sigma_workbook_qualified_name",
-        "sigma_workbook_name",
-        "sigma_page_qualified_name",
-        "sigma_page_name",
-        "sigma_data_element_qualified_name",
-        "sigma_data_element_name",
-    ]
-
-    @property
-    def sigma_workbook_qualified_name(self) -> Optional[str]:
-        return self.attributes.sigma_workbook_qualified_name
-
-    @sigma_workbook_qualified_name.setter
-    def sigma_workbook_qualified_name(
-        self, sigma_workbook_qualified_name: Optional[str]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.sigma_workbook_qualified_name = sigma_workbook_qualified_name
-
-    @property
-    def sigma_workbook_name(self) -> Optional[str]:
-        return self.attributes.sigma_workbook_name
-
-    @sigma_workbook_name.setter
-    def sigma_workbook_name(self, sigma_workbook_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.sigma_workbook_name = sigma_workbook_name
-
-    @property
-    def sigma_page_qualified_name(self) -> Optional[str]:
-        return self.attributes.sigma_page_qualified_name
-
-    @sigma_page_qualified_name.setter
-    def sigma_page_qualified_name(self, sigma_page_qualified_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.sigma_page_qualified_name = sigma_page_qualified_name
-
-    @property
-    def sigma_page_name(self) -> Optional[str]:
-        return self.attributes.sigma_page_name
-
-    @sigma_page_name.setter
-    def sigma_page_name(self, sigma_page_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.sigma_page_name = sigma_page_name
-
-    @property
-    def sigma_data_element_qualified_name(self) -> Optional[str]:
-        return self.attributes.sigma_data_element_qualified_name
-
-    @sigma_data_element_qualified_name.setter
-    def sigma_data_element_qualified_name(
-        self, sigma_data_element_qualified_name: Optional[str]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.sigma_data_element_qualified_name = (
-            sigma_data_element_qualified_name
-        )
-
-    @property
-    def sigma_data_element_name(self) -> Optional[str]:
-        return self.attributes.sigma_data_element_name
-
-    @sigma_data_element_name.setter
-    def sigma_data_element_name(self, sigma_data_element_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.sigma_data_element_name = sigma_data_element_name
-
-    type_name: str = Field("Sigma", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Sigma":
-            raise ValueError("must be Sigma")
-        return v
-
-    class Attributes(BI.Attributes):
-        sigma_workbook_qualified_name: Optional[str] = Field(
-            None, description="", alias="sigmaWorkbookQualifiedName"
-        )
-        sigma_workbook_name: Optional[str] = Field(
-            None, description="", alias="sigmaWorkbookName"
-        )
-        sigma_page_qualified_name: Optional[str] = Field(
-            None, description="", alias="sigmaPageQualifiedName"
-        )
-        sigma_page_name: Optional[str] = Field(
-            None, description="", alias="sigmaPageName"
-        )
-        sigma_data_element_qualified_name: Optional[str] = Field(
-            None, description="", alias="sigmaDataElementQualifiedName"
-        )
-        sigma_data_element_name: Optional[str] = Field(
-            None, description="", alias="sigmaDataElementName"
-        )
-
-    attributes: "Sigma.Attributes" = Field(
-        default_factory=lambda: Sigma.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
 class Qlik(BI):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Qlik._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -10158,16 +10537,18 @@
         "external_location_format",
         "is_partitioned",
         "partition_strategy",
         "partition_count",
         "partition_list",
         "partitions",
         "columns",
+        "facts",
         "queries",
         "atlan_schema",
+        "dimensions",
     ]
 
     @property
     def column_count(self) -> Optional[int]:
         return self.attributes.column_count
 
     @column_count.setter
@@ -10323,14 +10704,24 @@
     @columns.setter
     def columns(self, columns: Optional[list[Column]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.columns = columns
 
     @property
+    def facts(self) -> Optional[list[Table]]:
+        return self.attributes.facts
+
+    @facts.setter
+    def facts(self, facts: Optional[list[Table]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.facts = facts
+
+    @property
     def queries(self) -> Optional[list[Query]]:
         return self.attributes.queries
 
     @queries.setter
     def queries(self, queries: Optional[list[Query]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -10342,14 +10733,24 @@
 
     @atlan_schema.setter
     def atlan_schema(self, atlan_schema: Optional[Schema]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.atlan_schema = atlan_schema
 
+    @property
+    def dimensions(self) -> Optional[list[Table]]:
+        return self.attributes.dimensions
+
+    @dimensions.setter
+    def dimensions(self, dimensions: Optional[list[Table]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dimensions = dimensions
+
     type_name: str = Field("Table", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Table":
             raise ValueError("must be Table")
         return v
@@ -10389,20 +10790,26 @@
         )
         partitions: Optional[list[TablePartition]] = Field(
             None, description="", alias="partitions"
         )  # relationship
         columns: Optional[list[Column]] = Field(
             None, description="", alias="columns"
         )  # relationship
+        facts: Optional[list[Table]] = Field(
+            None, description="", alias="facts"
+        )  # relationship
         queries: Optional[list[Query]] = Field(
             None, description="", alias="queries"
         )  # relationship
         atlan_schema: Optional[Schema] = Field(
             None, description="", alias="atlanSchema"
         )  # relationship
+        dimensions: Optional[list[Table]] = Field(
+            None, description="", alias="dimensions"
+        )  # relationship
 
         @classmethod
         # @validate_arguments()
         def create(cls, *, name: str, schema_qualified_name: str) -> Table.Attributes:
             if not name:
                 raise ValueError("name cannot be blank")
             validate_required_fields(["schema_qualified_name"], [schema_qualified_name])
@@ -11543,16 +11950,16 @@
         if name in Schema._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "table_count",
         "views_count",
-        "snowflake_tags",
         "materialised_views",
+        "snowflake_tags",
         "tables",
         "database",
         "snowflake_pipes",
         "snowflake_streams",
         "procedures",
         "views",
     ]
@@ -11574,34 +11981,34 @@
     @views_count.setter
     def views_count(self, views_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.views_count = views_count
 
     @property
-    def snowflake_tags(self) -> Optional[list[SnowflakeTag]]:
-        return self.attributes.snowflake_tags
-
-    @snowflake_tags.setter
-    def snowflake_tags(self, snowflake_tags: Optional[list[SnowflakeTag]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.snowflake_tags = snowflake_tags
-
-    @property
     def materialised_views(self) -> Optional[list[MaterialisedView]]:
         return self.attributes.materialised_views
 
     @materialised_views.setter
     def materialised_views(self, materialised_views: Optional[list[MaterialisedView]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.materialised_views = materialised_views
 
     @property
+    def snowflake_tags(self) -> Optional[list[SnowflakeTag]]:
+        return self.attributes.snowflake_tags
+
+    @snowflake_tags.setter
+    def snowflake_tags(self, snowflake_tags: Optional[list[SnowflakeTag]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.snowflake_tags = snowflake_tags
+
+    @property
     def tables(self) -> Optional[list[Table]]:
         return self.attributes.tables
 
     @tables.setter
     def tables(self, tables: Optional[list[Table]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -11664,20 +12071,20 @@
         if v != "Schema":
             raise ValueError("must be Schema")
         return v
 
     class Attributes(SQL.Attributes):
         table_count: Optional[int] = Field(None, description="", alias="tableCount")
         views_count: Optional[int] = Field(None, description="", alias="viewsCount")
-        snowflake_tags: Optional[list[SnowflakeTag]] = Field(
-            None, description="", alias="snowflakeTags"
-        )  # relationship
         materialised_views: Optional[list[MaterialisedView]] = Field(
             None, description="", alias="materialisedViews"
         )  # relationship
+        snowflake_tags: Optional[list[SnowflakeTag]] = Field(
+            None, description="", alias="snowflakeTags"
+        )  # relationship
         tables: Optional[list[Table]] = Field(
             None, description="", alias="tables"
         )  # relationship
         database: Optional[Database] = Field(
             None, description="", alias="database"
         )  # relationship
         snowflake_pipes: Optional[list[SnowflakePipe]] = Field(
@@ -11734,14 +12141,115 @@
         )
         attributes = Schema.Attributes.create(
             name=name, database_qualified_name=database_qualified_name
         )
         return cls(attributes=attributes)
 
 
+class Database(SQL):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in Database._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "schema_count",
+        "schemas",
+    ]
+
+    @property
+    def schema_count(self) -> Optional[int]:
+        return self.attributes.schema_count
+
+    @schema_count.setter
+    def schema_count(self, schema_count: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.schema_count = schema_count
+
+    @property
+    def schemas(self) -> Optional[list[Schema]]:
+        return self.attributes.schemas
+
+    @schemas.setter
+    def schemas(self, schemas: Optional[list[Schema]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.schemas = schemas
+
+    type_name: str = Field("Database", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Database":
+            raise ValueError("must be Database")
+        return v
+
+    class Attributes(SQL.Attributes):
+        schema_count: Optional[int] = Field(None, description="", alias="schemaCount")
+        schemas: Optional[list[Schema]] = Field(
+            None, description="", alias="schemas"
+        )  # relationship
+
+        @classmethod
+        # @validate_arguments()
+        def create(
+            cls, name: str, connection_qualified_name: str
+        ) -> Database.Attributes:
+            if not name:
+                raise ValueError("name cannot be blank")
+            validate_required_fields(
+                ["connection_qualified_name"], [connection_qualified_name]
+            )
+            fields = connection_qualified_name.split("/")
+            if len(fields) != 3:
+                raise ValueError("Invalid connection_qualified_name")
+            try:
+                connector_type = AtlanConnectorType(fields[1])  # type:ignore
+            except ValueError as e:
+                raise ValueError("Invalid connection_qualified_name") from e
+            return Database.Attributes(
+                name=name,
+                connection_qualified_name=connection_qualified_name,
+                qualified_name=f"{connection_qualified_name}/{name}",
+                connector_name=connector_type.value,
+            )
+
+    attributes: "Database.Attributes" = Field(
+        default_factory=lambda: Database.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+    @classmethod
+    # @validate_arguments()
+    def create(cls, *, name: str, connection_qualified_name: str) -> Database:
+        if not name:
+            raise ValueError("name cannot be blank")
+        validate_required_fields(
+            ["connection_qualified_name"], [connection_qualified_name]
+        )
+        fields = connection_qualified_name.split("/")
+        if len(fields) != 3:
+            raise ValueError("Invalid connection_qualified_name")
+        try:
+            connector_type = AtlanConnectorType(fields[1])  # type:ignore
+        except ValueError as e:
+            raise ValueError("Invalid connection_qualified_name") from e
+        attributes = Database.Attributes(
+            name=name,
+            connection_qualified_name=connection_qualified_name,
+            qualified_name=f"{connection_qualified_name}/{name}",
+            connector_name=connector_type.value,
+        )
+        return cls(attributes=attributes)
+
+
 class SnowflakeStream(SQL):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in SnowflakeStream._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -11938,115 +12446,14 @@
     attributes: "SnowflakePipe.Attributes" = Field(
         default_factory=lambda: SnowflakePipe.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
-class Database(SQL):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in Database._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "schema_count",
-        "schemas",
-    ]
-
-    @property
-    def schema_count(self) -> Optional[int]:
-        return self.attributes.schema_count
-
-    @schema_count.setter
-    def schema_count(self, schema_count: Optional[int]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.schema_count = schema_count
-
-    @property
-    def schemas(self) -> Optional[list[Schema]]:
-        return self.attributes.schemas
-
-    @schemas.setter
-    def schemas(self, schemas: Optional[list[Schema]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.schemas = schemas
-
-    type_name: str = Field("Database", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Database":
-            raise ValueError("must be Database")
-        return v
-
-    class Attributes(SQL.Attributes):
-        schema_count: Optional[int] = Field(None, description="", alias="schemaCount")
-        schemas: Optional[list[Schema]] = Field(
-            None, description="", alias="schemas"
-        )  # relationship
-
-        @classmethod
-        # @validate_arguments()
-        def create(
-            cls, name: str, connection_qualified_name: str
-        ) -> Database.Attributes:
-            if not name:
-                raise ValueError("name cannot be blank")
-            validate_required_fields(
-                ["connection_qualified_name"], [connection_qualified_name]
-            )
-            fields = connection_qualified_name.split("/")
-            if len(fields) != 3:
-                raise ValueError("Invalid connection_qualified_name")
-            try:
-                connector_type = AtlanConnectorType(fields[1])  # type:ignore
-            except ValueError as e:
-                raise ValueError("Invalid connection_qualified_name") from e
-            return Database.Attributes(
-                name=name,
-                connection_qualified_name=connection_qualified_name,
-                qualified_name=f"{connection_qualified_name}/{name}",
-                connector_name=connector_type.value,
-            )
-
-    attributes: "Database.Attributes" = Field(
-        default_factory=lambda: Database.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-    @classmethod
-    # @validate_arguments()
-    def create(cls, *, name: str, connection_qualified_name: str) -> Database:
-        if not name:
-            raise ValueError("name cannot be blank")
-        validate_required_fields(
-            ["connection_qualified_name"], [connection_qualified_name]
-        )
-        fields = connection_qualified_name.split("/")
-        if len(fields) != 3:
-            raise ValueError("Invalid connection_qualified_name")
-        try:
-            connector_type = AtlanConnectorType(fields[1])  # type:ignore
-        except ValueError as e:
-            raise ValueError("Invalid connection_qualified_name") from e
-        attributes = Database.Attributes(
-            name=name,
-            connection_qualified_name=connection_qualified_name,
-            qualified_name=f"{connection_qualified_name}/{name}",
-            connector_name=connector_type.value,
-        )
-        return cls(attributes=attributes)
-
-
 class Procedure(SQL):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Procedure._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -12500,428 +12907,877 @@
         columns: Optional[list[Column]] = Field(
             None, description="", alias="columns"
         )  # relationship
         atlan_schema: Optional[Schema] = Field(
             None, description="", alias="atlanSchema"
         )  # relationship
 
+        @classmethod
+        # @validate_arguments()
+        def create(
+            cls, *, name: str, schema_qualified_name: str
+        ) -> MaterialisedView.Attributes:
+            if not name:
+                raise ValueError("name cannot be blank")
+            validate_required_fields(["schema_qualified_name"], [schema_qualified_name])
+            fields = schema_qualified_name.split("/")
+            if len(fields) != 5:
+                raise ValueError("Invalid schema_qualified_name")
+            try:
+                connector_type = AtlanConnectorType(fields[1])  # type:ignore
+            except ValueError as e:
+                raise ValueError("Invalid schema_qualified_name") from e
+            return MaterialisedView.Attributes(
+                name=name,
+                database_name=fields[3],
+                connection_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}",
+                database_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}/{fields[3]}",
+                qualified_name=f"{schema_qualified_name}/{name}",
+                schema_qualified_name=schema_qualified_name,
+                schema_name=fields[4],
+                connector_name=connector_type.value,
+                atlan_schema=Schema.ref_by_qualified_name(schema_qualified_name),
+            )
+
     attributes: "MaterialisedView.Attributes" = Field(
         default_factory=lambda: MaterialisedView.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
+    @classmethod
+    # @validate_arguments()
+    def create(cls, *, name: str, schema_qualified_name: str) -> MaterialisedView:
+        validate_required_fields(
+            ["name", "schema_qualified_name"], [name, schema_qualified_name]
+        )
+        attributes = MaterialisedView.Attributes.create(
+            name=name, schema_qualified_name=schema_qualified_name
+        )
+        return cls(attributes=attributes)
+
 
-class GCSObject(GCS):
+class DataStudioAsset(DataStudio):
     """Description"""
 
     def __setattr__(self, name, value):
-        if name in GCSObject._convience_properties:
+        if name in DataStudioAsset._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
-        "gcs_bucket_name",
-        "gcs_bucket_qualified_name",
-        "gcs_object_size",
-        "gcs_object_key",
-        "gcs_object_media_link",
-        "gcs_object_hold_type",
-        "gcs_object_generation_id",
-        "gcs_object_c_r_c32_c_hash",
-        "gcs_object_m_d5_hash",
-        "gcs_object_data_last_modified_time",
-        "gcs_object_content_type",
-        "gcs_object_content_encoding",
-        "gcs_object_content_disposition",
-        "gcs_object_content_language",
-        "gcs_object_retention_expiration_date",
-        "gcs_bucket",
+        "data_studio_asset_type",
+        "data_studio_asset_title",
+        "data_studio_asset_owner",
+        "is_trashed_data_studio_asset",
+        "google_service",
+        "google_project_name",
+        "google_project_id",
+        "google_project_number",
+        "google_location",
+        "google_location_type",
+        "google_labels",
+        "google_tags",
     ]
 
     @property
-    def gcs_bucket_name(self) -> Optional[str]:
-        return self.attributes.gcs_bucket_name
+    def data_studio_asset_type(self) -> Optional[GoogleDatastudioAssetType]:
+        return self.attributes.data_studio_asset_type
 
-    @gcs_bucket_name.setter
-    def gcs_bucket_name(self, gcs_bucket_name: Optional[str]):
+    @data_studio_asset_type.setter
+    def data_studio_asset_type(
+        self, data_studio_asset_type: Optional[GoogleDatastudioAssetType]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.gcs_bucket_name = gcs_bucket_name
+        self.attributes.data_studio_asset_type = data_studio_asset_type
 
     @property
-    def gcs_bucket_qualified_name(self) -> Optional[str]:
-        return self.attributes.gcs_bucket_qualified_name
+    def data_studio_asset_title(self) -> Optional[str]:
+        return self.attributes.data_studio_asset_title
 
-    @gcs_bucket_qualified_name.setter
-    def gcs_bucket_qualified_name(self, gcs_bucket_qualified_name: Optional[str]):
+    @data_studio_asset_title.setter
+    def data_studio_asset_title(self, data_studio_asset_title: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.gcs_bucket_qualified_name = gcs_bucket_qualified_name
+        self.attributes.data_studio_asset_title = data_studio_asset_title
 
     @property
-    def gcs_object_size(self) -> Optional[int]:
-        return self.attributes.gcs_object_size
+    def data_studio_asset_owner(self) -> Optional[str]:
+        return self.attributes.data_studio_asset_owner
 
-    @gcs_object_size.setter
-    def gcs_object_size(self, gcs_object_size: Optional[int]):
+    @data_studio_asset_owner.setter
+    def data_studio_asset_owner(self, data_studio_asset_owner: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.gcs_object_size = gcs_object_size
+        self.attributes.data_studio_asset_owner = data_studio_asset_owner
 
     @property
-    def gcs_object_key(self) -> Optional[str]:
-        return self.attributes.gcs_object_key
+    def is_trashed_data_studio_asset(self) -> Optional[bool]:
+        return self.attributes.is_trashed_data_studio_asset
 
-    @gcs_object_key.setter
-    def gcs_object_key(self, gcs_object_key: Optional[str]):
+    @is_trashed_data_studio_asset.setter
+    def is_trashed_data_studio_asset(
+        self, is_trashed_data_studio_asset: Optional[bool]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.gcs_object_key = gcs_object_key
+        self.attributes.is_trashed_data_studio_asset = is_trashed_data_studio_asset
 
     @property
-    def gcs_object_media_link(self) -> Optional[str]:
-        return self.attributes.gcs_object_media_link
+    def google_service(self) -> Optional[str]:
+        return self.attributes.google_service
 
-    @gcs_object_media_link.setter
-    def gcs_object_media_link(self, gcs_object_media_link: Optional[str]):
+    @google_service.setter
+    def google_service(self, google_service: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.gcs_object_media_link = gcs_object_media_link
+        self.attributes.google_service = google_service
 
     @property
-    def gcs_object_hold_type(self) -> Optional[str]:
-        return self.attributes.gcs_object_hold_type
+    def google_project_name(self) -> Optional[str]:
+        return self.attributes.google_project_name
 
-    @gcs_object_hold_type.setter
-    def gcs_object_hold_type(self, gcs_object_hold_type: Optional[str]):
+    @google_project_name.setter
+    def google_project_name(self, google_project_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.gcs_object_hold_type = gcs_object_hold_type
+        self.attributes.google_project_name = google_project_name
 
     @property
-    def gcs_object_generation_id(self) -> Optional[int]:
-        return self.attributes.gcs_object_generation_id
+    def google_project_id(self) -> Optional[str]:
+        return self.attributes.google_project_id
 
-    @gcs_object_generation_id.setter
-    def gcs_object_generation_id(self, gcs_object_generation_id: Optional[int]):
+    @google_project_id.setter
+    def google_project_id(self, google_project_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.gcs_object_generation_id = gcs_object_generation_id
+        self.attributes.google_project_id = google_project_id
 
     @property
-    def gcs_object_c_r_c32_c_hash(self) -> Optional[str]:
-        return self.attributes.gcs_object_c_r_c32_c_hash
+    def google_project_number(self) -> Optional[int]:
+        return self.attributes.google_project_number
 
-    @gcs_object_c_r_c32_c_hash.setter
-    def gcs_object_c_r_c32_c_hash(self, gcs_object_c_r_c32_c_hash: Optional[str]):
+    @google_project_number.setter
+    def google_project_number(self, google_project_number: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.gcs_object_c_r_c32_c_hash = gcs_object_c_r_c32_c_hash
+        self.attributes.google_project_number = google_project_number
 
     @property
-    def gcs_object_m_d5_hash(self) -> Optional[str]:
-        return self.attributes.gcs_object_m_d5_hash
+    def google_location(self) -> Optional[str]:
+        return self.attributes.google_location
 
-    @gcs_object_m_d5_hash.setter
-    def gcs_object_m_d5_hash(self, gcs_object_m_d5_hash: Optional[str]):
+    @google_location.setter
+    def google_location(self, google_location: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.gcs_object_m_d5_hash = gcs_object_m_d5_hash
+        self.attributes.google_location = google_location
 
     @property
-    def gcs_object_data_last_modified_time(self) -> Optional[datetime]:
-        return self.attributes.gcs_object_data_last_modified_time
+    def google_location_type(self) -> Optional[str]:
+        return self.attributes.google_location_type
 
-    @gcs_object_data_last_modified_time.setter
-    def gcs_object_data_last_modified_time(
-        self, gcs_object_data_last_modified_time: Optional[datetime]
-    ):
+    @google_location_type.setter
+    def google_location_type(self, google_location_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.gcs_object_data_last_modified_time = (
-            gcs_object_data_last_modified_time
+        self.attributes.google_location_type = google_location_type
+
+    @property
+    def google_labels(self) -> Optional[list[GoogleLabel]]:
+        return self.attributes.google_labels
+
+    @google_labels.setter
+    def google_labels(self, google_labels: Optional[list[GoogleLabel]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.google_labels = google_labels
+
+    @property
+    def google_tags(self) -> Optional[list[GoogleTag]]:
+        return self.attributes.google_tags
+
+    @google_tags.setter
+    def google_tags(self, google_tags: Optional[list[GoogleTag]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.google_tags = google_tags
+
+    type_name: str = Field("DataStudioAsset", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "DataStudioAsset":
+            raise ValueError("must be DataStudioAsset")
+        return v
+
+    class Attributes(DataStudio.Attributes):
+        data_studio_asset_type: Optional[GoogleDatastudioAssetType] = Field(
+            None, description="", alias="dataStudioAssetType"
+        )
+        data_studio_asset_title: Optional[str] = Field(
+            None, description="", alias="dataStudioAssetTitle"
+        )
+        data_studio_asset_owner: Optional[str] = Field(
+            None, description="", alias="dataStudioAssetOwner"
+        )
+        is_trashed_data_studio_asset: Optional[bool] = Field(
+            None, description="", alias="isTrashedDataStudioAsset"
+        )
+        google_service: Optional[str] = Field(
+            None, description="", alias="googleService"
+        )
+        google_project_name: Optional[str] = Field(
+            None, description="", alias="googleProjectName"
+        )
+        google_project_id: Optional[str] = Field(
+            None, description="", alias="googleProjectId"
+        )
+        google_project_number: Optional[int] = Field(
+            None, description="", alias="googleProjectNumber"
+        )
+        google_location: Optional[str] = Field(
+            None, description="", alias="googleLocation"
+        )
+        google_location_type: Optional[str] = Field(
+            None, description="", alias="googleLocationType"
+        )
+        google_labels: Optional[list[GoogleLabel]] = Field(
+            None, description="", alias="googleLabels"
+        )
+        google_tags: Optional[list[GoogleTag]] = Field(
+            None, description="", alias="googleTags"
         )
 
+    attributes: "DataStudioAsset.Attributes" = Field(
+        default_factory=lambda: DataStudioAsset.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class KafkaTopic(Kafka):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in KafkaTopic._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "kafka_topic_is_internal",
+        "kafka_topic_compression_type",
+        "kafka_topic_replication_factor",
+        "kafka_topic_segment_bytes",
+        "kafka_topic_partitions_count",
+        "kafka_topic_size_in_bytes",
+        "kafka_topic_record_count",
+        "kafka_topic_cleanup_policy",
+        "kafka_consumer_groups",
+    ]
+
     @property
-    def gcs_object_content_type(self) -> Optional[str]:
-        return self.attributes.gcs_object_content_type
+    def kafka_topic_is_internal(self) -> Optional[bool]:
+        return self.attributes.kafka_topic_is_internal
 
-    @gcs_object_content_type.setter
-    def gcs_object_content_type(self, gcs_object_content_type: Optional[str]):
+    @kafka_topic_is_internal.setter
+    def kafka_topic_is_internal(self, kafka_topic_is_internal: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.gcs_object_content_type = gcs_object_content_type
+        self.attributes.kafka_topic_is_internal = kafka_topic_is_internal
 
     @property
-    def gcs_object_content_encoding(self) -> Optional[str]:
-        return self.attributes.gcs_object_content_encoding
+    def kafka_topic_compression_type(self) -> Optional[KafkaTopicCompressionType]:
+        return self.attributes.kafka_topic_compression_type
 
-    @gcs_object_content_encoding.setter
-    def gcs_object_content_encoding(self, gcs_object_content_encoding: Optional[str]):
+    @kafka_topic_compression_type.setter
+    def kafka_topic_compression_type(
+        self, kafka_topic_compression_type: Optional[KafkaTopicCompressionType]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.gcs_object_content_encoding = gcs_object_content_encoding
+        self.attributes.kafka_topic_compression_type = kafka_topic_compression_type
 
     @property
-    def gcs_object_content_disposition(self) -> Optional[str]:
-        return self.attributes.gcs_object_content_disposition
+    def kafka_topic_replication_factor(self) -> Optional[int]:
+        return self.attributes.kafka_topic_replication_factor
 
-    @gcs_object_content_disposition.setter
-    def gcs_object_content_disposition(
-        self, gcs_object_content_disposition: Optional[str]
+    @kafka_topic_replication_factor.setter
+    def kafka_topic_replication_factor(
+        self, kafka_topic_replication_factor: Optional[int]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.gcs_object_content_disposition = gcs_object_content_disposition
+        self.attributes.kafka_topic_replication_factor = kafka_topic_replication_factor
 
     @property
-    def gcs_object_content_language(self) -> Optional[str]:
-        return self.attributes.gcs_object_content_language
+    def kafka_topic_segment_bytes(self) -> Optional[int]:
+        return self.attributes.kafka_topic_segment_bytes
 
-    @gcs_object_content_language.setter
-    def gcs_object_content_language(self, gcs_object_content_language: Optional[str]):
+    @kafka_topic_segment_bytes.setter
+    def kafka_topic_segment_bytes(self, kafka_topic_segment_bytes: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.gcs_object_content_language = gcs_object_content_language
+        self.attributes.kafka_topic_segment_bytes = kafka_topic_segment_bytes
 
     @property
-    def gcs_object_retention_expiration_date(self) -> Optional[datetime]:
-        return self.attributes.gcs_object_retention_expiration_date
+    def kafka_topic_partitions_count(self) -> Optional[int]:
+        return self.attributes.kafka_topic_partitions_count
 
-    @gcs_object_retention_expiration_date.setter
-    def gcs_object_retention_expiration_date(
-        self, gcs_object_retention_expiration_date: Optional[datetime]
+    @kafka_topic_partitions_count.setter
+    def kafka_topic_partitions_count(self, kafka_topic_partitions_count: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.kafka_topic_partitions_count = kafka_topic_partitions_count
+
+    @property
+    def kafka_topic_size_in_bytes(self) -> Optional[int]:
+        return self.attributes.kafka_topic_size_in_bytes
+
+    @kafka_topic_size_in_bytes.setter
+    def kafka_topic_size_in_bytes(self, kafka_topic_size_in_bytes: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.kafka_topic_size_in_bytes = kafka_topic_size_in_bytes
+
+    @property
+    def kafka_topic_record_count(self) -> Optional[int]:
+        return self.attributes.kafka_topic_record_count
+
+    @kafka_topic_record_count.setter
+    def kafka_topic_record_count(self, kafka_topic_record_count: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.kafka_topic_record_count = kafka_topic_record_count
+
+    @property
+    def kafka_topic_cleanup_policy(self) -> Optional[PowerbiEndorsement]:
+        return self.attributes.kafka_topic_cleanup_policy
+
+    @kafka_topic_cleanup_policy.setter
+    def kafka_topic_cleanup_policy(
+        self, kafka_topic_cleanup_policy: Optional[PowerbiEndorsement]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.gcs_object_retention_expiration_date = (
-            gcs_object_retention_expiration_date
-        )
+        self.attributes.kafka_topic_cleanup_policy = kafka_topic_cleanup_policy
 
     @property
-    def gcs_bucket(self) -> Optional[GCSBucket]:
-        return self.attributes.gcs_bucket
+    def kafka_consumer_groups(self) -> Optional[list[KafkaConsumerGroup]]:
+        return self.attributes.kafka_consumer_groups
 
-    @gcs_bucket.setter
-    def gcs_bucket(self, gcs_bucket: Optional[GCSBucket]):
+    @kafka_consumer_groups.setter
+    def kafka_consumer_groups(
+        self, kafka_consumer_groups: Optional[list[KafkaConsumerGroup]]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.gcs_bucket = gcs_bucket
+        self.attributes.kafka_consumer_groups = kafka_consumer_groups
 
-    type_name: str = Field("GCSObject", allow_mutation=False)
+    type_name: str = Field("KafkaTopic", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
-        if v != "GCSObject":
-            raise ValueError("must be GCSObject")
+        if v != "KafkaTopic":
+            raise ValueError("must be KafkaTopic")
         return v
 
-    class Attributes(GCS.Attributes):
-        gcs_bucket_name: Optional[str] = Field(
-            None, description="", alias="gcsBucketName"
-        )
-        gcs_bucket_qualified_name: Optional[str] = Field(
-            None, description="", alias="gcsBucketQualifiedName"
+    class Attributes(Kafka.Attributes):
+        kafka_topic_is_internal: Optional[bool] = Field(
+            None, description="", alias="kafkaTopicIsInternal"
         )
-        gcs_object_size: Optional[int] = Field(
-            None, description="", alias="gcsObjectSize"
+        kafka_topic_compression_type: Optional[KafkaTopicCompressionType] = Field(
+            None, description="", alias="kafkaTopicCompressionType"
         )
-        gcs_object_key: Optional[str] = Field(
-            None, description="", alias="gcsObjectKey"
+        kafka_topic_replication_factor: Optional[int] = Field(
+            None, description="", alias="kafkaTopicReplicationFactor"
         )
-        gcs_object_media_link: Optional[str] = Field(
-            None, description="", alias="gcsObjectMediaLink"
+        kafka_topic_segment_bytes: Optional[int] = Field(
+            None, description="", alias="kafkaTopicSegmentBytes"
         )
-        gcs_object_hold_type: Optional[str] = Field(
-            None, description="", alias="gcsObjectHoldType"
+        kafka_topic_partitions_count: Optional[int] = Field(
+            None, description="", alias="kafkaTopicPartitionsCount"
         )
-        gcs_object_generation_id: Optional[int] = Field(
-            None, description="", alias="gcsObjectGenerationId"
+        kafka_topic_size_in_bytes: Optional[int] = Field(
+            None, description="", alias="kafkaTopicSizeInBytes"
         )
-        gcs_object_c_r_c32_c_hash: Optional[str] = Field(
-            None, description="", alias="gcsObjectCRC32CHash"
+        kafka_topic_record_count: Optional[int] = Field(
+            None, description="", alias="kafkaTopicRecordCount"
         )
-        gcs_object_m_d5_hash: Optional[str] = Field(
-            None, description="", alias="gcsObjectMD5Hash"
+        kafka_topic_cleanup_policy: Optional[PowerbiEndorsement] = Field(
+            None, description="", alias="kafkaTopicCleanupPolicy"
         )
-        gcs_object_data_last_modified_time: Optional[datetime] = Field(
-            None, description="", alias="gcsObjectDataLastModifiedTime"
+        kafka_consumer_groups: Optional[list[KafkaConsumerGroup]] = Field(
+            None, description="", alias="kafkaConsumerGroups"
+        )  # relationship
+
+    attributes: "KafkaTopic.Attributes" = Field(
+        default_factory=lambda: KafkaTopic.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class KafkaConsumerGroup(Kafka):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in KafkaConsumerGroup._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "kafka_consumer_group_topic_consumption_properties",
+        "kafka_consumer_group_member_count",
+        "kafka_topic_names",
+        "kafka_topic_qualified_names",
+        "kafka_topics",
+    ]
+
+    @property
+    def kafka_consumer_group_topic_consumption_properties(
+        self,
+    ) -> Optional[list[KafkaTopicConsumption]]:
+        return self.attributes.kafka_consumer_group_topic_consumption_properties
+
+    @kafka_consumer_group_topic_consumption_properties.setter
+    def kafka_consumer_group_topic_consumption_properties(
+        self,
+        kafka_consumer_group_topic_consumption_properties: Optional[
+            list[KafkaTopicConsumption]
+        ],
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.kafka_consumer_group_topic_consumption_properties = (
+            kafka_consumer_group_topic_consumption_properties
         )
-        gcs_object_content_type: Optional[str] = Field(
-            None, description="", alias="gcsObjectContentType"
+
+    @property
+    def kafka_consumer_group_member_count(self) -> Optional[int]:
+        return self.attributes.kafka_consumer_group_member_count
+
+    @kafka_consumer_group_member_count.setter
+    def kafka_consumer_group_member_count(
+        self, kafka_consumer_group_member_count: Optional[int]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.kafka_consumer_group_member_count = (
+            kafka_consumer_group_member_count
         )
-        gcs_object_content_encoding: Optional[str] = Field(
-            None, description="", alias="gcsObjectContentEncoding"
+
+    @property
+    def kafka_topic_names(self) -> Optional[set[str]]:
+        return self.attributes.kafka_topic_names
+
+    @kafka_topic_names.setter
+    def kafka_topic_names(self, kafka_topic_names: Optional[set[str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.kafka_topic_names = kafka_topic_names
+
+    @property
+    def kafka_topic_qualified_names(self) -> Optional[set[str]]:
+        return self.attributes.kafka_topic_qualified_names
+
+    @kafka_topic_qualified_names.setter
+    def kafka_topic_qualified_names(
+        self, kafka_topic_qualified_names: Optional[set[str]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.kafka_topic_qualified_names = kafka_topic_qualified_names
+
+    @property
+    def kafka_topics(self) -> Optional[list[KafkaTopic]]:
+        return self.attributes.kafka_topics
+
+    @kafka_topics.setter
+    def kafka_topics(self, kafka_topics: Optional[list[KafkaTopic]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.kafka_topics = kafka_topics
+
+    type_name: str = Field("KafkaConsumerGroup", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "KafkaConsumerGroup":
+            raise ValueError("must be KafkaConsumerGroup")
+        return v
+
+    class Attributes(Kafka.Attributes):
+        kafka_consumer_group_topic_consumption_properties: Optional[
+            list[KafkaTopicConsumption]
+        ] = Field(
+            None, description="", alias="kafkaConsumerGroupTopicConsumptionProperties"
         )
-        gcs_object_content_disposition: Optional[str] = Field(
-            None, description="", alias="gcsObjectContentDisposition"
+        kafka_consumer_group_member_count: Optional[int] = Field(
+            None, description="", alias="kafkaConsumerGroupMemberCount"
         )
-        gcs_object_content_language: Optional[str] = Field(
-            None, description="", alias="gcsObjectContentLanguage"
+        kafka_topic_names: Optional[set[str]] = Field(
+            None, description="", alias="kafkaTopicNames"
         )
-        gcs_object_retention_expiration_date: Optional[datetime] = Field(
-            None, description="", alias="gcsObjectRetentionExpirationDate"
+        kafka_topic_qualified_names: Optional[set[str]] = Field(
+            None, description="", alias="kafkaTopicQualifiedNames"
         )
-        gcs_bucket: Optional[GCSBucket] = Field(
-            None, description="", alias="gcsBucket"
+        kafka_topics: Optional[list[KafkaTopic]] = Field(
+            None, description="", alias="kafkaTopics"
         )  # relationship
 
-    attributes: "GCSObject.Attributes" = Field(
-        default_factory=lambda: GCSObject.Attributes(),
+    attributes: "KafkaConsumerGroup.Attributes" = Field(
+        default_factory=lambda: KafkaConsumerGroup.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
-class GCSBucket(GCS):
+class S3Bucket(S3):
     """Description"""
 
     def __setattr__(self, name, value):
-        if name in GCSBucket._convience_properties:
+        if name in S3Bucket._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
-        "gcs_object_count",
-        "gcs_bucket_versioning_enabled",
-        "gcs_bucket_retention_locked",
-        "gcs_bucket_retention_period",
-        "gcs_bucket_retention_effective_time",
-        "gcs_bucket_lifecycle_rules",
-        "gcs_bucket_retention_policy",
-        "gcs_objects",
+        "s3_object_count",
+        "s3_bucket_versioning_enabled",
+        "objects",
     ]
 
     @property
-    def gcs_object_count(self) -> Optional[int]:
-        return self.attributes.gcs_object_count
+    def s3_object_count(self) -> Optional[int]:
+        return self.attributes.s3_object_count
 
-    @gcs_object_count.setter
-    def gcs_object_count(self, gcs_object_count: Optional[int]):
+    @s3_object_count.setter
+    def s3_object_count(self, s3_object_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.gcs_object_count = gcs_object_count
+        self.attributes.s3_object_count = s3_object_count
 
     @property
-    def gcs_bucket_versioning_enabled(self) -> Optional[bool]:
-        return self.attributes.gcs_bucket_versioning_enabled
+    def s3_bucket_versioning_enabled(self) -> Optional[bool]:
+        return self.attributes.s3_bucket_versioning_enabled
 
-    @gcs_bucket_versioning_enabled.setter
-    def gcs_bucket_versioning_enabled(
-        self, gcs_bucket_versioning_enabled: Optional[bool]
+    @s3_bucket_versioning_enabled.setter
+    def s3_bucket_versioning_enabled(
+        self, s3_bucket_versioning_enabled: Optional[bool]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.gcs_bucket_versioning_enabled = gcs_bucket_versioning_enabled
+        self.attributes.s3_bucket_versioning_enabled = s3_bucket_versioning_enabled
 
     @property
-    def gcs_bucket_retention_locked(self) -> Optional[bool]:
-        return self.attributes.gcs_bucket_retention_locked
+    def objects(self) -> Optional[list[S3Object]]:
+        return self.attributes.objects
 
-    @gcs_bucket_retention_locked.setter
-    def gcs_bucket_retention_locked(self, gcs_bucket_retention_locked: Optional[bool]):
+    @objects.setter
+    def objects(self, objects: Optional[list[S3Object]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.gcs_bucket_retention_locked = gcs_bucket_retention_locked
+        self.attributes.objects = objects
+
+    type_name: str = Field("S3Bucket", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "S3Bucket":
+            raise ValueError("must be S3Bucket")
+        return v
+
+    class Attributes(S3.Attributes):
+        s3_object_count: Optional[int] = Field(
+            None, description="", alias="s3ObjectCount"
+        )
+        s3_bucket_versioning_enabled: Optional[bool] = Field(
+            None, description="", alias="s3BucketVersioningEnabled"
+        )
+        objects: Optional[list[S3Object]] = Field(
+            None, description="", alias="objects"
+        )  # relationship
+
+        @classmethod
+        # @validate_arguments()
+        def create(
+            cls, *, name: str, connection_qualified_name: str, aws_arn: str
+        ) -> S3Bucket.Attributes:
+            validate_required_fields(
+                ["name", "connection_qualified_name", "aws_arn"],
+                [name, connection_qualified_name, aws_arn],
+            )
+            fields = connection_qualified_name.split("/")
+            if len(fields) != 3:
+                raise ValueError("Invalid connection_qualified_name")
+            try:
+                if fields[0].replace(" ", "") == "" or fields[2].replace(" ", "") == "":
+                    raise ValueError("Invalid connection_qualified_name")
+                connector_type = AtlanConnectorType(fields[1])  # type:ignore
+                if connector_type != AtlanConnectorType.S3:
+                    raise ValueError("Connector type must be s3")
+            except ValueError as e:
+                raise ValueError("Invalid connection_qualified_name") from e
+            return S3Bucket.Attributes(
+                aws_arn=aws_arn,
+                name=name,
+                connection_qualified_name=connection_qualified_name,
+                qualified_name=f"{connection_qualified_name}/{aws_arn}",
+                connector_name=connector_type.value,
+            )
+
+    attributes: "S3Bucket.Attributes" = Field(
+        default_factory=lambda: S3Bucket.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+    @classmethod
+    # @validate_arguments()
+    def create(
+        cls, *, name: str, connection_qualified_name: str, aws_arn: str
+    ) -> S3Bucket:
+        validate_required_fields(
+            ["name", "connection_qualified_name", "aws_arn"],
+            [name, connection_qualified_name, aws_arn],
+        )
+        attributes = S3Bucket.Attributes.create(
+            name=name,
+            connection_qualified_name=connection_qualified_name,
+            aws_arn=aws_arn,
+        )
+        return cls(attributes=attributes)
+
+
+class S3Object(S3):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in S3Object._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "s3_object_last_modified_time",
+        "s3_bucket_name",
+        "s3_bucket_qualified_name",
+        "s3_object_size",
+        "s3_object_storage_class",
+        "s3_object_key",
+        "s3_object_content_type",
+        "s3_object_content_disposition",
+        "s3_object_version_id",
+        "bucket",
+    ]
 
     @property
-    def gcs_bucket_retention_period(self) -> Optional[int]:
-        return self.attributes.gcs_bucket_retention_period
+    def s3_object_last_modified_time(self) -> Optional[datetime]:
+        return self.attributes.s3_object_last_modified_time
 
-    @gcs_bucket_retention_period.setter
-    def gcs_bucket_retention_period(self, gcs_bucket_retention_period: Optional[int]):
+    @s3_object_last_modified_time.setter
+    def s3_object_last_modified_time(
+        self, s3_object_last_modified_time: Optional[datetime]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.gcs_bucket_retention_period = gcs_bucket_retention_period
+        self.attributes.s3_object_last_modified_time = s3_object_last_modified_time
 
     @property
-    def gcs_bucket_retention_effective_time(self) -> Optional[datetime]:
-        return self.attributes.gcs_bucket_retention_effective_time
+    def s3_bucket_name(self) -> Optional[str]:
+        return self.attributes.s3_bucket_name
 
-    @gcs_bucket_retention_effective_time.setter
-    def gcs_bucket_retention_effective_time(
-        self, gcs_bucket_retention_effective_time: Optional[datetime]
-    ):
+    @s3_bucket_name.setter
+    def s3_bucket_name(self, s3_bucket_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.gcs_bucket_retention_effective_time = (
-            gcs_bucket_retention_effective_time
-        )
+        self.attributes.s3_bucket_name = s3_bucket_name
 
     @property
-    def gcs_bucket_lifecycle_rules(self) -> Optional[str]:
-        return self.attributes.gcs_bucket_lifecycle_rules
+    def s3_bucket_qualified_name(self) -> Optional[str]:
+        return self.attributes.s3_bucket_qualified_name
 
-    @gcs_bucket_lifecycle_rules.setter
-    def gcs_bucket_lifecycle_rules(self, gcs_bucket_lifecycle_rules: Optional[str]):
+    @s3_bucket_qualified_name.setter
+    def s3_bucket_qualified_name(self, s3_bucket_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.gcs_bucket_lifecycle_rules = gcs_bucket_lifecycle_rules
+        self.attributes.s3_bucket_qualified_name = s3_bucket_qualified_name
 
     @property
-    def gcs_bucket_retention_policy(self) -> Optional[str]:
-        return self.attributes.gcs_bucket_retention_policy
+    def s3_object_size(self) -> Optional[int]:
+        return self.attributes.s3_object_size
 
-    @gcs_bucket_retention_policy.setter
-    def gcs_bucket_retention_policy(self, gcs_bucket_retention_policy: Optional[str]):
+    @s3_object_size.setter
+    def s3_object_size(self, s3_object_size: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.gcs_bucket_retention_policy = gcs_bucket_retention_policy
+        self.attributes.s3_object_size = s3_object_size
 
     @property
-    def gcs_objects(self) -> Optional[list[GCSObject]]:
-        return self.attributes.gcs_objects
+    def s3_object_storage_class(self) -> Optional[str]:
+        return self.attributes.s3_object_storage_class
 
-    @gcs_objects.setter
-    def gcs_objects(self, gcs_objects: Optional[list[GCSObject]]):
+    @s3_object_storage_class.setter
+    def s3_object_storage_class(self, s3_object_storage_class: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.gcs_objects = gcs_objects
+        self.attributes.s3_object_storage_class = s3_object_storage_class
 
-    type_name: str = Field("GCSBucket", allow_mutation=False)
+    @property
+    def s3_object_key(self) -> Optional[str]:
+        return self.attributes.s3_object_key
+
+    @s3_object_key.setter
+    def s3_object_key(self, s3_object_key: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.s3_object_key = s3_object_key
+
+    @property
+    def s3_object_content_type(self) -> Optional[str]:
+        return self.attributes.s3_object_content_type
+
+    @s3_object_content_type.setter
+    def s3_object_content_type(self, s3_object_content_type: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.s3_object_content_type = s3_object_content_type
+
+    @property
+    def s3_object_content_disposition(self) -> Optional[str]:
+        return self.attributes.s3_object_content_disposition
+
+    @s3_object_content_disposition.setter
+    def s3_object_content_disposition(
+        self, s3_object_content_disposition: Optional[str]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.s3_object_content_disposition = s3_object_content_disposition
+
+    @property
+    def s3_object_version_id(self) -> Optional[str]:
+        return self.attributes.s3_object_version_id
+
+    @s3_object_version_id.setter
+    def s3_object_version_id(self, s3_object_version_id: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.s3_object_version_id = s3_object_version_id
+
+    @property
+    def bucket(self) -> Optional[S3Bucket]:
+        return self.attributes.bucket
+
+    @bucket.setter
+    def bucket(self, bucket: Optional[S3Bucket]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.bucket = bucket
+
+    type_name: str = Field("S3Object", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
-        if v != "GCSBucket":
-            raise ValueError("must be GCSBucket")
+        if v != "S3Object":
+            raise ValueError("must be S3Object")
         return v
 
-    class Attributes(GCS.Attributes):
-        gcs_object_count: Optional[int] = Field(
-            None, description="", alias="gcsObjectCount"
+    class Attributes(S3.Attributes):
+        s3_object_last_modified_time: Optional[datetime] = Field(
+            None, description="", alias="s3ObjectLastModifiedTime"
         )
-        gcs_bucket_versioning_enabled: Optional[bool] = Field(
-            None, description="", alias="gcsBucketVersioningEnabled"
+        s3_bucket_name: Optional[str] = Field(
+            None, description="", alias="s3BucketName"
         )
-        gcs_bucket_retention_locked: Optional[bool] = Field(
-            None, description="", alias="gcsBucketRetentionLocked"
+        s3_bucket_qualified_name: Optional[str] = Field(
+            None, description="", alias="s3BucketQualifiedName"
         )
-        gcs_bucket_retention_period: Optional[int] = Field(
-            None, description="", alias="gcsBucketRetentionPeriod"
+        s3_object_size: Optional[int] = Field(
+            None, description="", alias="s3ObjectSize"
         )
-        gcs_bucket_retention_effective_time: Optional[datetime] = Field(
-            None, description="", alias="gcsBucketRetentionEffectiveTime"
+        s3_object_storage_class: Optional[str] = Field(
+            None, description="", alias="s3ObjectStorageClass"
         )
-        gcs_bucket_lifecycle_rules: Optional[str] = Field(
-            None, description="", alias="gcsBucketLifecycleRules"
+        s3_object_key: Optional[str] = Field(None, description="", alias="s3ObjectKey")
+        s3_object_content_type: Optional[str] = Field(
+            None, description="", alias="s3ObjectContentType"
         )
-        gcs_bucket_retention_policy: Optional[str] = Field(
-            None, description="", alias="gcsBucketRetentionPolicy"
+        s3_object_content_disposition: Optional[str] = Field(
+            None, description="", alias="s3ObjectContentDisposition"
         )
-        gcs_objects: Optional[list[GCSObject]] = Field(
-            None, description="", alias="gcsObjects"
+        s3_object_version_id: Optional[str] = Field(
+            None, description="", alias="s3ObjectVersionId"
+        )
+        bucket: Optional[S3Bucket] = Field(
+            None, description="", alias="bucket"
         )  # relationship
 
-    attributes: "GCSBucket.Attributes" = Field(
-        default_factory=lambda: GCSBucket.Attributes(),
+        @classmethod
+        # @validate_arguments()
+        def create(
+            cls,
+            *,
+            name: str,
+            connection_qualified_name: str,
+            aws_arn: str,
+            s3_bucket_qualified_name: Optional[str] = None,
+        ) -> S3Object.Attributes:
+            validate_required_fields(
+                ["name", "connection_qualified_name", "aws_arn"],
+                [name, connection_qualified_name, aws_arn],
+            )
+            fields = connection_qualified_name.split("/")
+            if len(fields) != 3:
+                raise ValueError("Invalid connection_qualified_name")
+            try:
+                if fields[0].replace(" ", "") == "" or fields[2].replace(" ", "") == "":
+                    raise ValueError("Invalid connection_qualified_name")
+                connector_type = AtlanConnectorType(fields[1])  # type:ignore
+                if connector_type != AtlanConnectorType.S3:
+                    raise ValueError("Connector type must be s3")
+            except ValueError as e:
+                raise ValueError("Invalid connection_qualified_name") from e
+            return S3Object.Attributes(
+                aws_arn=aws_arn,
+                name=name,
+                connection_qualified_name=connection_qualified_name,
+                qualified_name=f"{connection_qualified_name}/{aws_arn}",
+                connector_name=connector_type.value,
+                s3_bucket_qualified_name=s3_bucket_qualified_name,
+            )
+
+    attributes: "S3Object.Attributes" = Field(
+        default_factory=lambda: S3Object.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
+    @classmethod
+    # @validate_arguments()
+    def create(
+        cls,
+        *,
+        name: str,
+        connection_qualified_name: str,
+        aws_arn: str,
+        s3_bucket_qualified_name: Optional[str] = None,
+    ) -> S3Object:
+        validate_required_fields(
+            ["name", "connection_qualified_name", "aws_arn"],
+            [name, connection_qualified_name, aws_arn],
+        )
+        attributes = S3Object.Attributes.create(
+            name=name,
+            connection_qualified_name=connection_qualified_name,
+            aws_arn=aws_arn,
+            s3_bucket_qualified_name=s3_bucket_qualified_name,
+        )
+        return cls(attributes=attributes)
+
 
 class ADLSAccount(ADLS):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in ADLSAccount._convience_properties:
             return object.__setattr__(self, name, value)
@@ -13559,628 +14415,417 @@
     attributes: "ADLSObject.Attributes" = Field(
         default_factory=lambda: ADLSObject.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
-class S3Bucket(S3):
+class GCSObject(GCS):
     """Description"""
 
     def __setattr__(self, name, value):
-        if name in S3Bucket._convience_properties:
+        if name in GCSObject._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
-        "s3_object_count",
-        "s3_bucket_versioning_enabled",
-        "objects",
+        "gcs_bucket_name",
+        "gcs_bucket_qualified_name",
+        "gcs_object_size",
+        "gcs_object_key",
+        "gcs_object_media_link",
+        "gcs_object_hold_type",
+        "gcs_object_generation_id",
+        "gcs_object_c_r_c32_c_hash",
+        "gcs_object_m_d5_hash",
+        "gcs_object_data_last_modified_time",
+        "gcs_object_content_type",
+        "gcs_object_content_encoding",
+        "gcs_object_content_disposition",
+        "gcs_object_content_language",
+        "gcs_object_retention_expiration_date",
+        "gcs_bucket",
     ]
 
     @property
-    def s3_object_count(self) -> Optional[int]:
-        return self.attributes.s3_object_count
+    def gcs_bucket_name(self) -> Optional[str]:
+        return self.attributes.gcs_bucket_name
 
-    @s3_object_count.setter
-    def s3_object_count(self, s3_object_count: Optional[int]):
+    @gcs_bucket_name.setter
+    def gcs_bucket_name(self, gcs_bucket_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.s3_object_count = s3_object_count
+        self.attributes.gcs_bucket_name = gcs_bucket_name
 
     @property
-    def s3_bucket_versioning_enabled(self) -> Optional[bool]:
-        return self.attributes.s3_bucket_versioning_enabled
+    def gcs_bucket_qualified_name(self) -> Optional[str]:
+        return self.attributes.gcs_bucket_qualified_name
 
-    @s3_bucket_versioning_enabled.setter
-    def s3_bucket_versioning_enabled(
-        self, s3_bucket_versioning_enabled: Optional[bool]
-    ):
+    @gcs_bucket_qualified_name.setter
+    def gcs_bucket_qualified_name(self, gcs_bucket_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.s3_bucket_versioning_enabled = s3_bucket_versioning_enabled
+        self.attributes.gcs_bucket_qualified_name = gcs_bucket_qualified_name
 
     @property
-    def objects(self) -> Optional[list[S3Object]]:
-        return self.attributes.objects
+    def gcs_object_size(self) -> Optional[int]:
+        return self.attributes.gcs_object_size
 
-    @objects.setter
-    def objects(self, objects: Optional[list[S3Object]]):
+    @gcs_object_size.setter
+    def gcs_object_size(self, gcs_object_size: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.objects = objects
-
-    type_name: str = Field("S3Bucket", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "S3Bucket":
-            raise ValueError("must be S3Bucket")
-        return v
-
-    class Attributes(S3.Attributes):
-        s3_object_count: Optional[int] = Field(
-            None, description="", alias="s3ObjectCount"
-        )
-        s3_bucket_versioning_enabled: Optional[bool] = Field(
-            None, description="", alias="s3BucketVersioningEnabled"
-        )
-        objects: Optional[list[S3Object]] = Field(
-            None, description="", alias="objects"
-        )  # relationship
-
-        @classmethod
-        # @validate_arguments()
-        def create(
-            cls, *, name: str, connection_qualified_name: str, aws_arn: str
-        ) -> S3Bucket.Attributes:
-            validate_required_fields(
-                ["name", "connection_qualified_name", "aws_arn"],
-                [name, connection_qualified_name, aws_arn],
-            )
-            fields = connection_qualified_name.split("/")
-            if len(fields) != 3:
-                raise ValueError("Invalid connection_qualified_name")
-            try:
-                if fields[0].replace(" ", "") == "" or fields[2].replace(" ", "") == "":
-                    raise ValueError("Invalid connection_qualified_name")
-                connector_type = AtlanConnectorType(fields[1])  # type:ignore
-                if connector_type != AtlanConnectorType.S3:
-                    raise ValueError("Connector type must be s3")
-            except ValueError as e:
-                raise ValueError("Invalid connection_qualified_name") from e
-            return S3Bucket.Attributes(
-                aws_arn=aws_arn,
-                name=name,
-                connection_qualified_name=connection_qualified_name,
-                qualified_name=f"{connection_qualified_name}/{aws_arn}",
-                connector_name=connector_type.value,
-            )
+        self.attributes.gcs_object_size = gcs_object_size
 
-    attributes: "S3Bucket.Attributes" = Field(
-        default_factory=lambda: S3Bucket.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
+    @property
+    def gcs_object_key(self) -> Optional[str]:
+        return self.attributes.gcs_object_key
 
-    @classmethod
-    # @validate_arguments()
-    def create(
-        cls, *, name: str, connection_qualified_name: str, aws_arn: str
-    ) -> S3Bucket:
-        validate_required_fields(
-            ["name", "connection_qualified_name", "aws_arn"],
-            [name, connection_qualified_name, aws_arn],
-        )
-        attributes = S3Bucket.Attributes.create(
-            name=name,
-            connection_qualified_name=connection_qualified_name,
-            aws_arn=aws_arn,
-        )
-        return cls(attributes=attributes)
+    @gcs_object_key.setter
+    def gcs_object_key(self, gcs_object_key: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.gcs_object_key = gcs_object_key
 
+    @property
+    def gcs_object_media_link(self) -> Optional[str]:
+        return self.attributes.gcs_object_media_link
 
-class S3Object(S3):
-    """Description"""
+    @gcs_object_media_link.setter
+    def gcs_object_media_link(self, gcs_object_media_link: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.gcs_object_media_link = gcs_object_media_link
 
-    def __setattr__(self, name, value):
-        if name in S3Object._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
+    @property
+    def gcs_object_hold_type(self) -> Optional[str]:
+        return self.attributes.gcs_object_hold_type
 
-    _convience_properties: ClassVar[list[str]] = [
-        "s3_object_last_modified_time",
-        "s3_bucket_name",
-        "s3_bucket_qualified_name",
-        "s3_object_size",
-        "s3_object_storage_class",
-        "s3_object_key",
-        "s3_object_content_type",
-        "s3_object_content_disposition",
-        "s3_object_version_id",
-        "bucket",
-    ]
+    @gcs_object_hold_type.setter
+    def gcs_object_hold_type(self, gcs_object_hold_type: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.gcs_object_hold_type = gcs_object_hold_type
 
     @property
-    def s3_object_last_modified_time(self) -> Optional[datetime]:
-        return self.attributes.s3_object_last_modified_time
+    def gcs_object_generation_id(self) -> Optional[int]:
+        return self.attributes.gcs_object_generation_id
 
-    @s3_object_last_modified_time.setter
-    def s3_object_last_modified_time(
-        self, s3_object_last_modified_time: Optional[datetime]
-    ):
+    @gcs_object_generation_id.setter
+    def gcs_object_generation_id(self, gcs_object_generation_id: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.s3_object_last_modified_time = s3_object_last_modified_time
+        self.attributes.gcs_object_generation_id = gcs_object_generation_id
 
     @property
-    def s3_bucket_name(self) -> Optional[str]:
-        return self.attributes.s3_bucket_name
+    def gcs_object_c_r_c32_c_hash(self) -> Optional[str]:
+        return self.attributes.gcs_object_c_r_c32_c_hash
 
-    @s3_bucket_name.setter
-    def s3_bucket_name(self, s3_bucket_name: Optional[str]):
+    @gcs_object_c_r_c32_c_hash.setter
+    def gcs_object_c_r_c32_c_hash(self, gcs_object_c_r_c32_c_hash: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.s3_bucket_name = s3_bucket_name
+        self.attributes.gcs_object_c_r_c32_c_hash = gcs_object_c_r_c32_c_hash
 
     @property
-    def s3_bucket_qualified_name(self) -> Optional[str]:
-        return self.attributes.s3_bucket_qualified_name
+    def gcs_object_m_d5_hash(self) -> Optional[str]:
+        return self.attributes.gcs_object_m_d5_hash
 
-    @s3_bucket_qualified_name.setter
-    def s3_bucket_qualified_name(self, s3_bucket_qualified_name: Optional[str]):
+    @gcs_object_m_d5_hash.setter
+    def gcs_object_m_d5_hash(self, gcs_object_m_d5_hash: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.s3_bucket_qualified_name = s3_bucket_qualified_name
+        self.attributes.gcs_object_m_d5_hash = gcs_object_m_d5_hash
 
     @property
-    def s3_object_size(self) -> Optional[int]:
-        return self.attributes.s3_object_size
+    def gcs_object_data_last_modified_time(self) -> Optional[datetime]:
+        return self.attributes.gcs_object_data_last_modified_time
 
-    @s3_object_size.setter
-    def s3_object_size(self, s3_object_size: Optional[int]):
+    @gcs_object_data_last_modified_time.setter
+    def gcs_object_data_last_modified_time(
+        self, gcs_object_data_last_modified_time: Optional[datetime]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.s3_object_size = s3_object_size
+        self.attributes.gcs_object_data_last_modified_time = (
+            gcs_object_data_last_modified_time
+        )
 
     @property
-    def s3_object_storage_class(self) -> Optional[str]:
-        return self.attributes.s3_object_storage_class
+    def gcs_object_content_type(self) -> Optional[str]:
+        return self.attributes.gcs_object_content_type
 
-    @s3_object_storage_class.setter
-    def s3_object_storage_class(self, s3_object_storage_class: Optional[str]):
+    @gcs_object_content_type.setter
+    def gcs_object_content_type(self, gcs_object_content_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.s3_object_storage_class = s3_object_storage_class
+        self.attributes.gcs_object_content_type = gcs_object_content_type
 
     @property
-    def s3_object_key(self) -> Optional[str]:
-        return self.attributes.s3_object_key
+    def gcs_object_content_encoding(self) -> Optional[str]:
+        return self.attributes.gcs_object_content_encoding
 
-    @s3_object_key.setter
-    def s3_object_key(self, s3_object_key: Optional[str]):
+    @gcs_object_content_encoding.setter
+    def gcs_object_content_encoding(self, gcs_object_content_encoding: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.s3_object_key = s3_object_key
+        self.attributes.gcs_object_content_encoding = gcs_object_content_encoding
 
     @property
-    def s3_object_content_type(self) -> Optional[str]:
-        return self.attributes.s3_object_content_type
+    def gcs_object_content_disposition(self) -> Optional[str]:
+        return self.attributes.gcs_object_content_disposition
 
-    @s3_object_content_type.setter
-    def s3_object_content_type(self, s3_object_content_type: Optional[str]):
+    @gcs_object_content_disposition.setter
+    def gcs_object_content_disposition(
+        self, gcs_object_content_disposition: Optional[str]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.s3_object_content_type = s3_object_content_type
+        self.attributes.gcs_object_content_disposition = gcs_object_content_disposition
 
     @property
-    def s3_object_content_disposition(self) -> Optional[str]:
-        return self.attributes.s3_object_content_disposition
+    def gcs_object_content_language(self) -> Optional[str]:
+        return self.attributes.gcs_object_content_language
 
-    @s3_object_content_disposition.setter
-    def s3_object_content_disposition(
-        self, s3_object_content_disposition: Optional[str]
-    ):
+    @gcs_object_content_language.setter
+    def gcs_object_content_language(self, gcs_object_content_language: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.s3_object_content_disposition = s3_object_content_disposition
+        self.attributes.gcs_object_content_language = gcs_object_content_language
 
     @property
-    def s3_object_version_id(self) -> Optional[str]:
-        return self.attributes.s3_object_version_id
+    def gcs_object_retention_expiration_date(self) -> Optional[datetime]:
+        return self.attributes.gcs_object_retention_expiration_date
 
-    @s3_object_version_id.setter
-    def s3_object_version_id(self, s3_object_version_id: Optional[str]):
+    @gcs_object_retention_expiration_date.setter
+    def gcs_object_retention_expiration_date(
+        self, gcs_object_retention_expiration_date: Optional[datetime]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.s3_object_version_id = s3_object_version_id
+        self.attributes.gcs_object_retention_expiration_date = (
+            gcs_object_retention_expiration_date
+        )
 
     @property
-    def bucket(self) -> Optional[S3Bucket]:
-        return self.attributes.bucket
+    def gcs_bucket(self) -> Optional[GCSBucket]:
+        return self.attributes.gcs_bucket
 
-    @bucket.setter
-    def bucket(self, bucket: Optional[S3Bucket]):
+    @gcs_bucket.setter
+    def gcs_bucket(self, gcs_bucket: Optional[GCSBucket]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.bucket = bucket
+        self.attributes.gcs_bucket = gcs_bucket
 
-    type_name: str = Field("S3Object", allow_mutation=False)
+    type_name: str = Field("GCSObject", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
-        if v != "S3Object":
-            raise ValueError("must be S3Object")
+        if v != "GCSObject":
+            raise ValueError("must be GCSObject")
         return v
 
-    class Attributes(S3.Attributes):
-        s3_object_last_modified_time: Optional[datetime] = Field(
-            None, description="", alias="s3ObjectLastModifiedTime"
+    class Attributes(GCS.Attributes):
+        gcs_bucket_name: Optional[str] = Field(
+            None, description="", alias="gcsBucketName"
         )
-        s3_bucket_name: Optional[str] = Field(
-            None, description="", alias="s3BucketName"
+        gcs_bucket_qualified_name: Optional[str] = Field(
+            None, description="", alias="gcsBucketQualifiedName"
         )
-        s3_bucket_qualified_name: Optional[str] = Field(
-            None, description="", alias="s3BucketQualifiedName"
+        gcs_object_size: Optional[int] = Field(
+            None, description="", alias="gcsObjectSize"
         )
-        s3_object_size: Optional[int] = Field(
-            None, description="", alias="s3ObjectSize"
+        gcs_object_key: Optional[str] = Field(
+            None, description="", alias="gcsObjectKey"
         )
-        s3_object_storage_class: Optional[str] = Field(
-            None, description="", alias="s3ObjectStorageClass"
+        gcs_object_media_link: Optional[str] = Field(
+            None, description="", alias="gcsObjectMediaLink"
         )
-        s3_object_key: Optional[str] = Field(None, description="", alias="s3ObjectKey")
-        s3_object_content_type: Optional[str] = Field(
-            None, description="", alias="s3ObjectContentType"
+        gcs_object_hold_type: Optional[str] = Field(
+            None, description="", alias="gcsObjectHoldType"
         )
-        s3_object_content_disposition: Optional[str] = Field(
-            None, description="", alias="s3ObjectContentDisposition"
+        gcs_object_generation_id: Optional[int] = Field(
+            None, description="", alias="gcsObjectGenerationId"
         )
-        s3_object_version_id: Optional[str] = Field(
-            None, description="", alias="s3ObjectVersionId"
+        gcs_object_c_r_c32_c_hash: Optional[str] = Field(
+            None, description="", alias="gcsObjectCRC32CHash"
         )
-        bucket: Optional[S3Bucket] = Field(
-            None, description="", alias="bucket"
+        gcs_object_m_d5_hash: Optional[str] = Field(
+            None, description="", alias="gcsObjectMD5Hash"
+        )
+        gcs_object_data_last_modified_time: Optional[datetime] = Field(
+            None, description="", alias="gcsObjectDataLastModifiedTime"
+        )
+        gcs_object_content_type: Optional[str] = Field(
+            None, description="", alias="gcsObjectContentType"
+        )
+        gcs_object_content_encoding: Optional[str] = Field(
+            None, description="", alias="gcsObjectContentEncoding"
+        )
+        gcs_object_content_disposition: Optional[str] = Field(
+            None, description="", alias="gcsObjectContentDisposition"
+        )
+        gcs_object_content_language: Optional[str] = Field(
+            None, description="", alias="gcsObjectContentLanguage"
+        )
+        gcs_object_retention_expiration_date: Optional[datetime] = Field(
+            None, description="", alias="gcsObjectRetentionExpirationDate"
+        )
+        gcs_bucket: Optional[GCSBucket] = Field(
+            None, description="", alias="gcsBucket"
         )  # relationship
 
-        @classmethod
-        # @validate_arguments()
-        def create(
-            cls,
-            *,
-            name: str,
-            connection_qualified_name: str,
-            aws_arn: str,
-            s3_bucket_qualified_name: Optional[str] = None,
-        ) -> S3Object.Attributes:
-            validate_required_fields(
-                ["name", "connection_qualified_name", "aws_arn"],
-                [name, connection_qualified_name, aws_arn],
-            )
-            fields = connection_qualified_name.split("/")
-            if len(fields) != 3:
-                raise ValueError("Invalid connection_qualified_name")
-            try:
-                if fields[0].replace(" ", "") == "" or fields[2].replace(" ", "") == "":
-                    raise ValueError("Invalid connection_qualified_name")
-                connector_type = AtlanConnectorType(fields[1])  # type:ignore
-                if connector_type != AtlanConnectorType.S3:
-                    raise ValueError("Connector type must be s3")
-            except ValueError as e:
-                raise ValueError("Invalid connection_qualified_name") from e
-            return S3Object.Attributes(
-                aws_arn=aws_arn,
-                name=name,
-                connection_qualified_name=connection_qualified_name,
-                qualified_name=f"{connection_qualified_name}/{aws_arn}",
-                connector_name=connector_type.value,
-                s3_bucket_qualified_name=s3_bucket_qualified_name,
-            )
-
-    attributes: "S3Object.Attributes" = Field(
-        default_factory=lambda: S3Object.Attributes(),
+    attributes: "GCSObject.Attributes" = Field(
+        default_factory=lambda: GCSObject.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
-    @classmethod
-    # @validate_arguments()
-    def create(
-        cls,
-        *,
-        name: str,
-        connection_qualified_name: str,
-        aws_arn: str,
-        s3_bucket_qualified_name: Optional[str] = None,
-    ) -> S3Object:
-        validate_required_fields(
-            ["name", "connection_qualified_name", "aws_arn"],
-            [name, connection_qualified_name, aws_arn],
-        )
-        attributes = S3Object.Attributes.create(
-            name=name,
-            connection_qualified_name=connection_qualified_name,
-            aws_arn=aws_arn,
-            s3_bucket_qualified_name=s3_bucket_qualified_name,
-        )
-        return cls(attributes=attributes)
 
-
-class KafkaTopic(Kafka):
+class GCSBucket(GCS):
     """Description"""
 
     def __setattr__(self, name, value):
-        if name in KafkaTopic._convience_properties:
+        if name in GCSBucket._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
-        "kafka_topic_is_internal",
-        "kafka_topic_compression_type",
-        "kafka_topic_replication_factor",
-        "kafka_topic_segment_bytes",
-        "kafka_topic_partitions_count",
-        "kafka_topic_size_in_bytes",
-        "kafka_topic_record_count",
-        "kafka_topic_cleanup_policy",
-        "kafka_consumer_groups",
+        "gcs_object_count",
+        "gcs_bucket_versioning_enabled",
+        "gcs_bucket_retention_locked",
+        "gcs_bucket_retention_period",
+        "gcs_bucket_retention_effective_time",
+        "gcs_bucket_lifecycle_rules",
+        "gcs_bucket_retention_policy",
+        "gcs_objects",
     ]
 
     @property
-    def kafka_topic_is_internal(self) -> Optional[bool]:
-        return self.attributes.kafka_topic_is_internal
-
-    @kafka_topic_is_internal.setter
-    def kafka_topic_is_internal(self, kafka_topic_is_internal: Optional[bool]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.kafka_topic_is_internal = kafka_topic_is_internal
-
-    @property
-    def kafka_topic_compression_type(self) -> Optional[KafkaTopicCompressionType]:
-        return self.attributes.kafka_topic_compression_type
+    def gcs_object_count(self) -> Optional[int]:
+        return self.attributes.gcs_object_count
 
-    @kafka_topic_compression_type.setter
-    def kafka_topic_compression_type(
-        self, kafka_topic_compression_type: Optional[KafkaTopicCompressionType]
-    ):
+    @gcs_object_count.setter
+    def gcs_object_count(self, gcs_object_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.kafka_topic_compression_type = kafka_topic_compression_type
+        self.attributes.gcs_object_count = gcs_object_count
 
     @property
-    def kafka_topic_replication_factor(self) -> Optional[int]:
-        return self.attributes.kafka_topic_replication_factor
+    def gcs_bucket_versioning_enabled(self) -> Optional[bool]:
+        return self.attributes.gcs_bucket_versioning_enabled
 
-    @kafka_topic_replication_factor.setter
-    def kafka_topic_replication_factor(
-        self, kafka_topic_replication_factor: Optional[int]
+    @gcs_bucket_versioning_enabled.setter
+    def gcs_bucket_versioning_enabled(
+        self, gcs_bucket_versioning_enabled: Optional[bool]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.kafka_topic_replication_factor = kafka_topic_replication_factor
+        self.attributes.gcs_bucket_versioning_enabled = gcs_bucket_versioning_enabled
 
     @property
-    def kafka_topic_segment_bytes(self) -> Optional[int]:
-        return self.attributes.kafka_topic_segment_bytes
+    def gcs_bucket_retention_locked(self) -> Optional[bool]:
+        return self.attributes.gcs_bucket_retention_locked
 
-    @kafka_topic_segment_bytes.setter
-    def kafka_topic_segment_bytes(self, kafka_topic_segment_bytes: Optional[int]):
+    @gcs_bucket_retention_locked.setter
+    def gcs_bucket_retention_locked(self, gcs_bucket_retention_locked: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.kafka_topic_segment_bytes = kafka_topic_segment_bytes
+        self.attributes.gcs_bucket_retention_locked = gcs_bucket_retention_locked
 
     @property
-    def kafka_topic_partitions_count(self) -> Optional[int]:
-        return self.attributes.kafka_topic_partitions_count
+    def gcs_bucket_retention_period(self) -> Optional[int]:
+        return self.attributes.gcs_bucket_retention_period
 
-    @kafka_topic_partitions_count.setter
-    def kafka_topic_partitions_count(self, kafka_topic_partitions_count: Optional[int]):
+    @gcs_bucket_retention_period.setter
+    def gcs_bucket_retention_period(self, gcs_bucket_retention_period: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.kafka_topic_partitions_count = kafka_topic_partitions_count
+        self.attributes.gcs_bucket_retention_period = gcs_bucket_retention_period
 
     @property
-    def kafka_topic_size_in_bytes(self) -> Optional[int]:
-        return self.attributes.kafka_topic_size_in_bytes
+    def gcs_bucket_retention_effective_time(self) -> Optional[datetime]:
+        return self.attributes.gcs_bucket_retention_effective_time
 
-    @kafka_topic_size_in_bytes.setter
-    def kafka_topic_size_in_bytes(self, kafka_topic_size_in_bytes: Optional[int]):
+    @gcs_bucket_retention_effective_time.setter
+    def gcs_bucket_retention_effective_time(
+        self, gcs_bucket_retention_effective_time: Optional[datetime]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.kafka_topic_size_in_bytes = kafka_topic_size_in_bytes
+        self.attributes.gcs_bucket_retention_effective_time = (
+            gcs_bucket_retention_effective_time
+        )
 
     @property
-    def kafka_topic_record_count(self) -> Optional[int]:
-        return self.attributes.kafka_topic_record_count
+    def gcs_bucket_lifecycle_rules(self) -> Optional[str]:
+        return self.attributes.gcs_bucket_lifecycle_rules
 
-    @kafka_topic_record_count.setter
-    def kafka_topic_record_count(self, kafka_topic_record_count: Optional[int]):
+    @gcs_bucket_lifecycle_rules.setter
+    def gcs_bucket_lifecycle_rules(self, gcs_bucket_lifecycle_rules: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.kafka_topic_record_count = kafka_topic_record_count
+        self.attributes.gcs_bucket_lifecycle_rules = gcs_bucket_lifecycle_rules
 
     @property
-    def kafka_topic_cleanup_policy(self) -> Optional[PowerbiEndorsement]:
-        return self.attributes.kafka_topic_cleanup_policy
+    def gcs_bucket_retention_policy(self) -> Optional[str]:
+        return self.attributes.gcs_bucket_retention_policy
 
-    @kafka_topic_cleanup_policy.setter
-    def kafka_topic_cleanup_policy(
-        self, kafka_topic_cleanup_policy: Optional[PowerbiEndorsement]
-    ):
+    @gcs_bucket_retention_policy.setter
+    def gcs_bucket_retention_policy(self, gcs_bucket_retention_policy: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.kafka_topic_cleanup_policy = kafka_topic_cleanup_policy
+        self.attributes.gcs_bucket_retention_policy = gcs_bucket_retention_policy
 
     @property
-    def kafka_consumer_groups(self) -> Optional[list[KafkaConsumerGroup]]:
-        return self.attributes.kafka_consumer_groups
+    def gcs_objects(self) -> Optional[list[GCSObject]]:
+        return self.attributes.gcs_objects
 
-    @kafka_consumer_groups.setter
-    def kafka_consumer_groups(
-        self, kafka_consumer_groups: Optional[list[KafkaConsumerGroup]]
-    ):
+    @gcs_objects.setter
+    def gcs_objects(self, gcs_objects: Optional[list[GCSObject]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.kafka_consumer_groups = kafka_consumer_groups
+        self.attributes.gcs_objects = gcs_objects
 
-    type_name: str = Field("KafkaTopic", allow_mutation=False)
+    type_name: str = Field("GCSBucket", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
-        if v != "KafkaTopic":
-            raise ValueError("must be KafkaTopic")
+        if v != "GCSBucket":
+            raise ValueError("must be GCSBucket")
         return v
 
-    class Attributes(Kafka.Attributes):
-        kafka_topic_is_internal: Optional[bool] = Field(
-            None, description="", alias="kafkaTopicIsInternal"
-        )
-        kafka_topic_compression_type: Optional[KafkaTopicCompressionType] = Field(
-            None, description="", alias="kafkaTopicCompressionType"
-        )
-        kafka_topic_replication_factor: Optional[int] = Field(
-            None, description="", alias="kafkaTopicReplicationFactor"
-        )
-        kafka_topic_segment_bytes: Optional[int] = Field(
-            None, description="", alias="kafkaTopicSegmentBytes"
-        )
-        kafka_topic_partitions_count: Optional[int] = Field(
-            None, description="", alias="kafkaTopicPartitionsCount"
-        )
-        kafka_topic_size_in_bytes: Optional[int] = Field(
-            None, description="", alias="kafkaTopicSizeInBytes"
-        )
-        kafka_topic_record_count: Optional[int] = Field(
-            None, description="", alias="kafkaTopicRecordCount"
-        )
-        kafka_topic_cleanup_policy: Optional[PowerbiEndorsement] = Field(
-            None, description="", alias="kafkaTopicCleanupPolicy"
+    class Attributes(GCS.Attributes):
+        gcs_object_count: Optional[int] = Field(
+            None, description="", alias="gcsObjectCount"
         )
-        kafka_consumer_groups: Optional[list[KafkaConsumerGroup]] = Field(
-            None, description="", alias="kafkaConsumerGroups"
-        )  # relationship
-
-    attributes: "KafkaTopic.Attributes" = Field(
-        default_factory=lambda: KafkaTopic.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class KafkaConsumerGroup(Kafka):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in KafkaConsumerGroup._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "kafka_consumer_group_topic_consumption_properties",
-        "kafka_consumer_group_member_count",
-        "kafka_topic_names",
-        "kafka_topic_qualified_names",
-        "kafka_topics",
-    ]
-
-    @property
-    def kafka_consumer_group_topic_consumption_properties(
-        self,
-    ) -> Optional[list[KafkaTopicConsumption]]:
-        return self.attributes.kafka_consumer_group_topic_consumption_properties
-
-    @kafka_consumer_group_topic_consumption_properties.setter
-    def kafka_consumer_group_topic_consumption_properties(
-        self,
-        kafka_consumer_group_topic_consumption_properties: Optional[
-            list[KafkaTopicConsumption]
-        ],
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.kafka_consumer_group_topic_consumption_properties = (
-            kafka_consumer_group_topic_consumption_properties
+        gcs_bucket_versioning_enabled: Optional[bool] = Field(
+            None, description="", alias="gcsBucketVersioningEnabled"
         )
-
-    @property
-    def kafka_consumer_group_member_count(self) -> Optional[int]:
-        return self.attributes.kafka_consumer_group_member_count
-
-    @kafka_consumer_group_member_count.setter
-    def kafka_consumer_group_member_count(
-        self, kafka_consumer_group_member_count: Optional[int]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.kafka_consumer_group_member_count = (
-            kafka_consumer_group_member_count
+        gcs_bucket_retention_locked: Optional[bool] = Field(
+            None, description="", alias="gcsBucketRetentionLocked"
         )
-
-    @property
-    def kafka_topic_names(self) -> Optional[set[str]]:
-        return self.attributes.kafka_topic_names
-
-    @kafka_topic_names.setter
-    def kafka_topic_names(self, kafka_topic_names: Optional[set[str]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.kafka_topic_names = kafka_topic_names
-
-    @property
-    def kafka_topic_qualified_names(self) -> Optional[set[str]]:
-        return self.attributes.kafka_topic_qualified_names
-
-    @kafka_topic_qualified_names.setter
-    def kafka_topic_qualified_names(
-        self, kafka_topic_qualified_names: Optional[set[str]]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.kafka_topic_qualified_names = kafka_topic_qualified_names
-
-    @property
-    def kafka_topics(self) -> Optional[list[KafkaTopic]]:
-        return self.attributes.kafka_topics
-
-    @kafka_topics.setter
-    def kafka_topics(self, kafka_topics: Optional[list[KafkaTopic]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.kafka_topics = kafka_topics
-
-    type_name: str = Field("KafkaConsumerGroup", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "KafkaConsumerGroup":
-            raise ValueError("must be KafkaConsumerGroup")
-        return v
-
-    class Attributes(Kafka.Attributes):
-        kafka_consumer_group_topic_consumption_properties: Optional[
-            list[KafkaTopicConsumption]
-        ] = Field(
-            None, description="", alias="kafkaConsumerGroupTopicConsumptionProperties"
+        gcs_bucket_retention_period: Optional[int] = Field(
+            None, description="", alias="gcsBucketRetentionPeriod"
         )
-        kafka_consumer_group_member_count: Optional[int] = Field(
-            None, description="", alias="kafkaConsumerGroupMemberCount"
+        gcs_bucket_retention_effective_time: Optional[datetime] = Field(
+            None, description="", alias="gcsBucketRetentionEffectiveTime"
         )
-        kafka_topic_names: Optional[set[str]] = Field(
-            None, description="", alias="kafkaTopicNames"
+        gcs_bucket_lifecycle_rules: Optional[str] = Field(
+            None, description="", alias="gcsBucketLifecycleRules"
         )
-        kafka_topic_qualified_names: Optional[set[str]] = Field(
-            None, description="", alias="kafkaTopicQualifiedNames"
+        gcs_bucket_retention_policy: Optional[str] = Field(
+            None, description="", alias="gcsBucketRetentionPolicy"
         )
-        kafka_topics: Optional[list[KafkaTopic]] = Field(
-            None, description="", alias="kafkaTopics"
+        gcs_objects: Optional[list[GCSObject]] = Field(
+            None, description="", alias="gcsObjects"
         )  # relationship
 
-    attributes: "KafkaConsumerGroup.Attributes" = Field(
-        default_factory=lambda: KafkaConsumerGroup.Attributes(),
+    attributes: "GCSBucket.Attributes" = Field(
+        default_factory=lambda: GCSBucket.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class MCIncident(MonteCarlo):
     """Description"""
@@ -15070,14 +15715,144 @@
     attributes: "QuickSightDashboardVisual.Attributes" = Field(
         default_factory=lambda: QuickSightDashboardVisual.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
+class QuickSightAnalysis(QuickSight):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in QuickSightAnalysis._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "quick_sight_analysis_status",
+        "quick_sight_analysis_calculated_fields",
+        "quick_sight_analysis_parameter_declarations",
+        "quick_sight_analysis_filter_groups",
+        "quick_sight_analysis_visuals",
+        "quick_sight_analysis_folders",
+    ]
+
+    @property
+    def quick_sight_analysis_status(self) -> Optional[QuickSightAnalysisStatus]:
+        return self.attributes.quick_sight_analysis_status
+
+    @quick_sight_analysis_status.setter
+    def quick_sight_analysis_status(
+        self, quick_sight_analysis_status: Optional[QuickSightAnalysisStatus]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_analysis_status = quick_sight_analysis_status
+
+    @property
+    def quick_sight_analysis_calculated_fields(self) -> Optional[set[str]]:
+        return self.attributes.quick_sight_analysis_calculated_fields
+
+    @quick_sight_analysis_calculated_fields.setter
+    def quick_sight_analysis_calculated_fields(
+        self, quick_sight_analysis_calculated_fields: Optional[set[str]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_analysis_calculated_fields = (
+            quick_sight_analysis_calculated_fields
+        )
+
+    @property
+    def quick_sight_analysis_parameter_declarations(self) -> Optional[set[str]]:
+        return self.attributes.quick_sight_analysis_parameter_declarations
+
+    @quick_sight_analysis_parameter_declarations.setter
+    def quick_sight_analysis_parameter_declarations(
+        self, quick_sight_analysis_parameter_declarations: Optional[set[str]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_analysis_parameter_declarations = (
+            quick_sight_analysis_parameter_declarations
+        )
+
+    @property
+    def quick_sight_analysis_filter_groups(self) -> Optional[set[str]]:
+        return self.attributes.quick_sight_analysis_filter_groups
+
+    @quick_sight_analysis_filter_groups.setter
+    def quick_sight_analysis_filter_groups(
+        self, quick_sight_analysis_filter_groups: Optional[set[str]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_analysis_filter_groups = (
+            quick_sight_analysis_filter_groups
+        )
+
+    @property
+    def quick_sight_analysis_visuals(self) -> Optional[list[QuickSightAnalysisVisual]]:
+        return self.attributes.quick_sight_analysis_visuals
+
+    @quick_sight_analysis_visuals.setter
+    def quick_sight_analysis_visuals(
+        self, quick_sight_analysis_visuals: Optional[list[QuickSightAnalysisVisual]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_analysis_visuals = quick_sight_analysis_visuals
+
+    @property
+    def quick_sight_analysis_folders(self) -> Optional[list[QuickSightFolder]]:
+        return self.attributes.quick_sight_analysis_folders
+
+    @quick_sight_analysis_folders.setter
+    def quick_sight_analysis_folders(
+        self, quick_sight_analysis_folders: Optional[list[QuickSightFolder]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_analysis_folders = quick_sight_analysis_folders
+
+    type_name: str = Field("QuickSightAnalysis", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "QuickSightAnalysis":
+            raise ValueError("must be QuickSightAnalysis")
+        return v
+
+    class Attributes(QuickSight.Attributes):
+        quick_sight_analysis_status: Optional[QuickSightAnalysisStatus] = Field(
+            None, description="", alias="quickSightAnalysisStatus"
+        )
+        quick_sight_analysis_calculated_fields: Optional[set[str]] = Field(
+            None, description="", alias="quickSightAnalysisCalculatedFields"
+        )
+        quick_sight_analysis_parameter_declarations: Optional[set[str]] = Field(
+            None, description="", alias="quickSightAnalysisParameterDeclarations"
+        )
+        quick_sight_analysis_filter_groups: Optional[set[str]] = Field(
+            None, description="", alias="quickSightAnalysisFilterGroups"
+        )
+        quick_sight_analysis_visuals: Optional[list[QuickSightAnalysisVisual]] = Field(
+            None, description="", alias="quickSightAnalysisVisuals"
+        )  # relationship
+        quick_sight_analysis_folders: Optional[list[QuickSightFolder]] = Field(
+            None, description="", alias="quickSightAnalysisFolders"
+        )  # relationship
+
+    attributes: "QuickSightAnalysis.Attributes" = Field(
+        default_factory=lambda: QuickSightAnalysis.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
 class QuickSightAnalysisVisual(QuickSight):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in QuickSightAnalysisVisual._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -15206,144 +15981,14 @@
     attributes: "QuickSightDatasetField.Attributes" = Field(
         default_factory=lambda: QuickSightDatasetField.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
-class QuickSightAnalysis(QuickSight):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in QuickSightAnalysis._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "quick_sight_analysis_status",
-        "quick_sight_analysis_calculated_fields",
-        "quick_sight_analysis_parameter_declarations",
-        "quick_sight_analysis_filter_groups",
-        "quick_sight_analysis_visuals",
-        "quick_sight_analysis_folders",
-    ]
-
-    @property
-    def quick_sight_analysis_status(self) -> Optional[QuickSightAnalysisStatus]:
-        return self.attributes.quick_sight_analysis_status
-
-    @quick_sight_analysis_status.setter
-    def quick_sight_analysis_status(
-        self, quick_sight_analysis_status: Optional[QuickSightAnalysisStatus]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_analysis_status = quick_sight_analysis_status
-
-    @property
-    def quick_sight_analysis_calculated_fields(self) -> Optional[set[str]]:
-        return self.attributes.quick_sight_analysis_calculated_fields
-
-    @quick_sight_analysis_calculated_fields.setter
-    def quick_sight_analysis_calculated_fields(
-        self, quick_sight_analysis_calculated_fields: Optional[set[str]]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_analysis_calculated_fields = (
-            quick_sight_analysis_calculated_fields
-        )
-
-    @property
-    def quick_sight_analysis_parameter_declarations(self) -> Optional[set[str]]:
-        return self.attributes.quick_sight_analysis_parameter_declarations
-
-    @quick_sight_analysis_parameter_declarations.setter
-    def quick_sight_analysis_parameter_declarations(
-        self, quick_sight_analysis_parameter_declarations: Optional[set[str]]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_analysis_parameter_declarations = (
-            quick_sight_analysis_parameter_declarations
-        )
-
-    @property
-    def quick_sight_analysis_filter_groups(self) -> Optional[set[str]]:
-        return self.attributes.quick_sight_analysis_filter_groups
-
-    @quick_sight_analysis_filter_groups.setter
-    def quick_sight_analysis_filter_groups(
-        self, quick_sight_analysis_filter_groups: Optional[set[str]]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_analysis_filter_groups = (
-            quick_sight_analysis_filter_groups
-        )
-
-    @property
-    def quick_sight_analysis_visuals(self) -> Optional[list[QuickSightAnalysisVisual]]:
-        return self.attributes.quick_sight_analysis_visuals
-
-    @quick_sight_analysis_visuals.setter
-    def quick_sight_analysis_visuals(
-        self, quick_sight_analysis_visuals: Optional[list[QuickSightAnalysisVisual]]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_analysis_visuals = quick_sight_analysis_visuals
-
-    @property
-    def quick_sight_analysis_folders(self) -> Optional[list[QuickSightFolder]]:
-        return self.attributes.quick_sight_analysis_folders
-
-    @quick_sight_analysis_folders.setter
-    def quick_sight_analysis_folders(
-        self, quick_sight_analysis_folders: Optional[list[QuickSightFolder]]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_analysis_folders = quick_sight_analysis_folders
-
-    type_name: str = Field("QuickSightAnalysis", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "QuickSightAnalysis":
-            raise ValueError("must be QuickSightAnalysis")
-        return v
-
-    class Attributes(QuickSight.Attributes):
-        quick_sight_analysis_status: Optional[QuickSightAnalysisStatus] = Field(
-            None, description="", alias="quickSightAnalysisStatus"
-        )
-        quick_sight_analysis_calculated_fields: Optional[set[str]] = Field(
-            None, description="", alias="quickSightAnalysisCalculatedFields"
-        )
-        quick_sight_analysis_parameter_declarations: Optional[set[str]] = Field(
-            None, description="", alias="quickSightAnalysisParameterDeclarations"
-        )
-        quick_sight_analysis_filter_groups: Optional[set[str]] = Field(
-            None, description="", alias="quickSightAnalysisFilterGroups"
-        )
-        quick_sight_analysis_visuals: Optional[list[QuickSightAnalysisVisual]] = Field(
-            None, description="", alias="quickSightAnalysisVisuals"
-        )  # relationship
-        quick_sight_analysis_folders: Optional[list[QuickSightFolder]] = Field(
-            None, description="", alias="quickSightAnalysisFolders"
-        )  # relationship
-
-    attributes: "QuickSightAnalysis.Attributes" = Field(
-        default_factory=lambda: QuickSightAnalysis.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
 class QuickSightDashboard(QuickSight):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in QuickSightDashboard._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -16037,14 +16682,112 @@
     attributes: "PowerBIColumn.Attributes" = Field(
         default_factory=lambda: PowerBIColumn.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
+class PowerBITile(PowerBI):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in PowerBITile._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "workspace_qualified_name",
+        "dashboard_qualified_name",
+        "report",
+        "dataset",
+        "dashboard",
+    ]
+
+    @property
+    def workspace_qualified_name(self) -> Optional[str]:
+        return self.attributes.workspace_qualified_name
+
+    @workspace_qualified_name.setter
+    def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.workspace_qualified_name = workspace_qualified_name
+
+    @property
+    def dashboard_qualified_name(self) -> Optional[str]:
+        return self.attributes.dashboard_qualified_name
+
+    @dashboard_qualified_name.setter
+    def dashboard_qualified_name(self, dashboard_qualified_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dashboard_qualified_name = dashboard_qualified_name
+
+    @property
+    def report(self) -> Optional[PowerBIReport]:
+        return self.attributes.report
+
+    @report.setter
+    def report(self, report: Optional[PowerBIReport]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.report = report
+
+    @property
+    def dataset(self) -> Optional[PowerBIDataset]:
+        return self.attributes.dataset
+
+    @dataset.setter
+    def dataset(self, dataset: Optional[PowerBIDataset]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dataset = dataset
+
+    @property
+    def dashboard(self) -> Optional[PowerBIDashboard]:
+        return self.attributes.dashboard
+
+    @dashboard.setter
+    def dashboard(self, dashboard: Optional[PowerBIDashboard]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dashboard = dashboard
+
+    type_name: str = Field("PowerBITile", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "PowerBITile":
+            raise ValueError("must be PowerBITile")
+        return v
+
+    class Attributes(PowerBI.Attributes):
+        workspace_qualified_name: Optional[str] = Field(
+            None, description="", alias="workspaceQualifiedName"
+        )
+        dashboard_qualified_name: Optional[str] = Field(
+            None, description="", alias="dashboardQualifiedName"
+        )
+        report: Optional[PowerBIReport] = Field(
+            None, description="", alias="report"
+        )  # relationship
+        dataset: Optional[PowerBIDataset] = Field(
+            None, description="", alias="dataset"
+        )  # relationship
+        dashboard: Optional[PowerBIDashboard] = Field(
+            None, description="", alias="dashboard"
+        )  # relationship
+
+    attributes: "PowerBITile.Attributes" = Field(
+        default_factory=lambda: PowerBITile.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
 class PowerBITable(PowerBI):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in PowerBITable._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -16183,112 +16926,14 @@
     attributes: "PowerBITable.Attributes" = Field(
         default_factory=lambda: PowerBITable.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
-class PowerBITile(PowerBI):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in PowerBITile._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "workspace_qualified_name",
-        "dashboard_qualified_name",
-        "report",
-        "dataset",
-        "dashboard",
-    ]
-
-    @property
-    def workspace_qualified_name(self) -> Optional[str]:
-        return self.attributes.workspace_qualified_name
-
-    @workspace_qualified_name.setter
-    def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.workspace_qualified_name = workspace_qualified_name
-
-    @property
-    def dashboard_qualified_name(self) -> Optional[str]:
-        return self.attributes.dashboard_qualified_name
-
-    @dashboard_qualified_name.setter
-    def dashboard_qualified_name(self, dashboard_qualified_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.dashboard_qualified_name = dashboard_qualified_name
-
-    @property
-    def report(self) -> Optional[PowerBIReport]:
-        return self.attributes.report
-
-    @report.setter
-    def report(self, report: Optional[PowerBIReport]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.report = report
-
-    @property
-    def dataset(self) -> Optional[PowerBIDataset]:
-        return self.attributes.dataset
-
-    @dataset.setter
-    def dataset(self, dataset: Optional[PowerBIDataset]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.dataset = dataset
-
-    @property
-    def dashboard(self) -> Optional[PowerBIDashboard]:
-        return self.attributes.dashboard
-
-    @dashboard.setter
-    def dashboard(self, dashboard: Optional[PowerBIDashboard]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.dashboard = dashboard
-
-    type_name: str = Field("PowerBITile", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "PowerBITile":
-            raise ValueError("must be PowerBITile")
-        return v
-
-    class Attributes(PowerBI.Attributes):
-        workspace_qualified_name: Optional[str] = Field(
-            None, description="", alias="workspaceQualifiedName"
-        )
-        dashboard_qualified_name: Optional[str] = Field(
-            None, description="", alias="dashboardQualifiedName"
-        )
-        report: Optional[PowerBIReport] = Field(
-            None, description="", alias="report"
-        )  # relationship
-        dataset: Optional[PowerBIDataset] = Field(
-            None, description="", alias="dataset"
-        )  # relationship
-        dashboard: Optional[PowerBIDashboard] = Field(
-            None, description="", alias="dashboard"
-        )  # relationship
-
-    attributes: "PowerBITile.Attributes" = Field(
-        default_factory=lambda: PowerBITile.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
 class PowerBIDatasource(PowerBI):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in PowerBIDatasource._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -16717,161 +17362,161 @@
     attributes: "PowerBIDashboard.Attributes" = Field(
         default_factory=lambda: PowerBIDashboard.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
-class PowerBIDataflow(PowerBI):
+class PowerBIPage(PowerBI):
     """Description"""
 
     def __setattr__(self, name, value):
-        if name in PowerBIDataflow._convience_properties:
+        if name in PowerBIPage._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "workspace_qualified_name",
-        "web_url",
-        "workspace",
-        "datasets",
+        "report_qualified_name",
+        "report",
     ]
 
     @property
     def workspace_qualified_name(self) -> Optional[str]:
         return self.attributes.workspace_qualified_name
 
     @workspace_qualified_name.setter
     def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.workspace_qualified_name = workspace_qualified_name
 
     @property
-    def web_url(self) -> Optional[str]:
-        return self.attributes.web_url
-
-    @web_url.setter
-    def web_url(self, web_url: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.web_url = web_url
-
-    @property
-    def workspace(self) -> Optional[PowerBIWorkspace]:
-        return self.attributes.workspace
+    def report_qualified_name(self) -> Optional[str]:
+        return self.attributes.report_qualified_name
 
-    @workspace.setter
-    def workspace(self, workspace: Optional[PowerBIWorkspace]):
+    @report_qualified_name.setter
+    def report_qualified_name(self, report_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.workspace = workspace
+        self.attributes.report_qualified_name = report_qualified_name
 
     @property
-    def datasets(self) -> Optional[list[PowerBIDataset]]:
-        return self.attributes.datasets
+    def report(self) -> Optional[PowerBIReport]:
+        return self.attributes.report
 
-    @datasets.setter
-    def datasets(self, datasets: Optional[list[PowerBIDataset]]):
+    @report.setter
+    def report(self, report: Optional[PowerBIReport]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.datasets = datasets
+        self.attributes.report = report
 
-    type_name: str = Field("PowerBIDataflow", allow_mutation=False)
+    type_name: str = Field("PowerBIPage", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
-        if v != "PowerBIDataflow":
-            raise ValueError("must be PowerBIDataflow")
+        if v != "PowerBIPage":
+            raise ValueError("must be PowerBIPage")
         return v
 
     class Attributes(PowerBI.Attributes):
         workspace_qualified_name: Optional[str] = Field(
             None, description="", alias="workspaceQualifiedName"
         )
-        web_url: Optional[str] = Field(None, description="", alias="webUrl")
-        workspace: Optional[PowerBIWorkspace] = Field(
-            None, description="", alias="workspace"
-        )  # relationship
-        datasets: Optional[list[PowerBIDataset]] = Field(
-            None, description="", alias="datasets"
+        report_qualified_name: Optional[str] = Field(
+            None, description="", alias="reportQualifiedName"
+        )
+        report: Optional[PowerBIReport] = Field(
+            None, description="", alias="report"
         )  # relationship
 
-    attributes: "PowerBIDataflow.Attributes" = Field(
-        default_factory=lambda: PowerBIDataflow.Attributes(),
+    attributes: "PowerBIPage.Attributes" = Field(
+        default_factory=lambda: PowerBIPage.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
-class PowerBIPage(PowerBI):
+class PowerBIDataflow(PowerBI):
     """Description"""
 
     def __setattr__(self, name, value):
-        if name in PowerBIPage._convience_properties:
+        if name in PowerBIDataflow._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "workspace_qualified_name",
-        "report_qualified_name",
-        "report",
+        "web_url",
+        "workspace",
+        "datasets",
     ]
 
     @property
     def workspace_qualified_name(self) -> Optional[str]:
         return self.attributes.workspace_qualified_name
 
     @workspace_qualified_name.setter
     def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.workspace_qualified_name = workspace_qualified_name
 
     @property
-    def report_qualified_name(self) -> Optional[str]:
-        return self.attributes.report_qualified_name
+    def web_url(self) -> Optional[str]:
+        return self.attributes.web_url
 
-    @report_qualified_name.setter
-    def report_qualified_name(self, report_qualified_name: Optional[str]):
+    @web_url.setter
+    def web_url(self, web_url: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.report_qualified_name = report_qualified_name
+        self.attributes.web_url = web_url
 
     @property
-    def report(self) -> Optional[PowerBIReport]:
-        return self.attributes.report
+    def workspace(self) -> Optional[PowerBIWorkspace]:
+        return self.attributes.workspace
 
-    @report.setter
-    def report(self, report: Optional[PowerBIReport]):
+    @workspace.setter
+    def workspace(self, workspace: Optional[PowerBIWorkspace]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.report = report
+        self.attributes.workspace = workspace
 
-    type_name: str = Field("PowerBIPage", allow_mutation=False)
+    @property
+    def datasets(self) -> Optional[list[PowerBIDataset]]:
+        return self.attributes.datasets
+
+    @datasets.setter
+    def datasets(self, datasets: Optional[list[PowerBIDataset]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.datasets = datasets
+
+    type_name: str = Field("PowerBIDataflow", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
-        if v != "PowerBIPage":
-            raise ValueError("must be PowerBIPage")
+        if v != "PowerBIDataflow":
+            raise ValueError("must be PowerBIDataflow")
         return v
 
     class Attributes(PowerBI.Attributes):
         workspace_qualified_name: Optional[str] = Field(
             None, description="", alias="workspaceQualifiedName"
         )
-        report_qualified_name: Optional[str] = Field(
-            None, description="", alias="reportQualifiedName"
-        )
-        report: Optional[PowerBIReport] = Field(
-            None, description="", alias="report"
+        web_url: Optional[str] = Field(None, description="", alias="webUrl")
+        workspace: Optional[PowerBIWorkspace] = Field(
+            None, description="", alias="workspace"
+        )  # relationship
+        datasets: Optional[list[PowerBIDataset]] = Field(
+            None, description="", alias="datasets"
         )  # relationship
 
-    attributes: "PowerBIPage.Attributes" = Field(
-        default_factory=lambda: PowerBIPage.Attributes(),
+    attributes: "PowerBIDataflow.Attributes" = Field(
+        default_factory=lambda: PowerBIDataflow.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class PresetChart(Preset):
     """Description"""
@@ -17383,448 +18028,14 @@
     attributes: "PresetWorkspace.Attributes" = Field(
         default_factory=lambda: PresetWorkspace.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
-class ModeReport(Mode):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in ModeReport._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "mode_collection_token",
-        "mode_report_published_at",
-        "mode_query_count",
-        "mode_chart_count",
-        "mode_query_preview",
-        "mode_is_public",
-        "mode_is_shared",
-        "mode_collections",
-        "mode_queries",
-    ]
-
-    @property
-    def mode_collection_token(self) -> Optional[str]:
-        return self.attributes.mode_collection_token
-
-    @mode_collection_token.setter
-    def mode_collection_token(self, mode_collection_token: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.mode_collection_token = mode_collection_token
-
-    @property
-    def mode_report_published_at(self) -> Optional[datetime]:
-        return self.attributes.mode_report_published_at
-
-    @mode_report_published_at.setter
-    def mode_report_published_at(self, mode_report_published_at: Optional[datetime]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.mode_report_published_at = mode_report_published_at
-
-    @property
-    def mode_query_count(self) -> Optional[int]:
-        return self.attributes.mode_query_count
-
-    @mode_query_count.setter
-    def mode_query_count(self, mode_query_count: Optional[int]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.mode_query_count = mode_query_count
-
-    @property
-    def mode_chart_count(self) -> Optional[int]:
-        return self.attributes.mode_chart_count
-
-    @mode_chart_count.setter
-    def mode_chart_count(self, mode_chart_count: Optional[int]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.mode_chart_count = mode_chart_count
-
-    @property
-    def mode_query_preview(self) -> Optional[str]:
-        return self.attributes.mode_query_preview
-
-    @mode_query_preview.setter
-    def mode_query_preview(self, mode_query_preview: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.mode_query_preview = mode_query_preview
-
-    @property
-    def mode_is_public(self) -> Optional[bool]:
-        return self.attributes.mode_is_public
-
-    @mode_is_public.setter
-    def mode_is_public(self, mode_is_public: Optional[bool]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.mode_is_public = mode_is_public
-
-    @property
-    def mode_is_shared(self) -> Optional[bool]:
-        return self.attributes.mode_is_shared
-
-    @mode_is_shared.setter
-    def mode_is_shared(self, mode_is_shared: Optional[bool]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.mode_is_shared = mode_is_shared
-
-    @property
-    def mode_collections(self) -> Optional[list[ModeCollection]]:
-        return self.attributes.mode_collections
-
-    @mode_collections.setter
-    def mode_collections(self, mode_collections: Optional[list[ModeCollection]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.mode_collections = mode_collections
-
-    @property
-    def mode_queries(self) -> Optional[list[ModeQuery]]:
-        return self.attributes.mode_queries
-
-    @mode_queries.setter
-    def mode_queries(self, mode_queries: Optional[list[ModeQuery]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.mode_queries = mode_queries
-
-    type_name: str = Field("ModeReport", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "ModeReport":
-            raise ValueError("must be ModeReport")
-        return v
-
-    class Attributes(Mode.Attributes):
-        mode_collection_token: Optional[str] = Field(
-            None, description="", alias="modeCollectionToken"
-        )
-        mode_report_published_at: Optional[datetime] = Field(
-            None, description="", alias="modeReportPublishedAt"
-        )
-        mode_query_count: Optional[int] = Field(
-            None, description="", alias="modeQueryCount"
-        )
-        mode_chart_count: Optional[int] = Field(
-            None, description="", alias="modeChartCount"
-        )
-        mode_query_preview: Optional[str] = Field(
-            None, description="", alias="modeQueryPreview"
-        )
-        mode_is_public: Optional[bool] = Field(
-            None, description="", alias="modeIsPublic"
-        )
-        mode_is_shared: Optional[bool] = Field(
-            None, description="", alias="modeIsShared"
-        )
-        mode_collections: Optional[list[ModeCollection]] = Field(
-            None, description="", alias="modeCollections"
-        )  # relationship
-        mode_queries: Optional[list[ModeQuery]] = Field(
-            None, description="", alias="modeQueries"
-        )  # relationship
-
-    attributes: "ModeReport.Attributes" = Field(
-        default_factory=lambda: ModeReport.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class ModeQuery(Mode):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in ModeQuery._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "mode_raw_query",
-        "mode_report_import_count",
-        "mode_charts",
-        "mode_report",
-    ]
-
-    @property
-    def mode_raw_query(self) -> Optional[str]:
-        return self.attributes.mode_raw_query
-
-    @mode_raw_query.setter
-    def mode_raw_query(self, mode_raw_query: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.mode_raw_query = mode_raw_query
-
-    @property
-    def mode_report_import_count(self) -> Optional[int]:
-        return self.attributes.mode_report_import_count
-
-    @mode_report_import_count.setter
-    def mode_report_import_count(self, mode_report_import_count: Optional[int]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.mode_report_import_count = mode_report_import_count
-
-    @property
-    def mode_charts(self) -> Optional[list[ModeChart]]:
-        return self.attributes.mode_charts
-
-    @mode_charts.setter
-    def mode_charts(self, mode_charts: Optional[list[ModeChart]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.mode_charts = mode_charts
-
-    @property
-    def mode_report(self) -> Optional[ModeReport]:
-        return self.attributes.mode_report
-
-    @mode_report.setter
-    def mode_report(self, mode_report: Optional[ModeReport]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.mode_report = mode_report
-
-    type_name: str = Field("ModeQuery", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "ModeQuery":
-            raise ValueError("must be ModeQuery")
-        return v
-
-    class Attributes(Mode.Attributes):
-        mode_raw_query: Optional[str] = Field(
-            None, description="", alias="modeRawQuery"
-        )
-        mode_report_import_count: Optional[int] = Field(
-            None, description="", alias="modeReportImportCount"
-        )
-        mode_charts: Optional[list[ModeChart]] = Field(
-            None, description="", alias="modeCharts"
-        )  # relationship
-        mode_report: Optional[ModeReport] = Field(
-            None, description="", alias="modeReport"
-        )  # relationship
-
-    attributes: "ModeQuery.Attributes" = Field(
-        default_factory=lambda: ModeQuery.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class ModeChart(Mode):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in ModeChart._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "mode_chart_type",
-        "mode_query",
-    ]
-
-    @property
-    def mode_chart_type(self) -> Optional[str]:
-        return self.attributes.mode_chart_type
-
-    @mode_chart_type.setter
-    def mode_chart_type(self, mode_chart_type: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.mode_chart_type = mode_chart_type
-
-    @property
-    def mode_query(self) -> Optional[ModeQuery]:
-        return self.attributes.mode_query
-
-    @mode_query.setter
-    def mode_query(self, mode_query: Optional[ModeQuery]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.mode_query = mode_query
-
-    type_name: str = Field("ModeChart", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "ModeChart":
-            raise ValueError("must be ModeChart")
-        return v
-
-    class Attributes(Mode.Attributes):
-        mode_chart_type: Optional[str] = Field(
-            None, description="", alias="modeChartType"
-        )
-        mode_query: Optional[ModeQuery] = Field(
-            None, description="", alias="modeQuery"
-        )  # relationship
-
-    attributes: "ModeChart.Attributes" = Field(
-        default_factory=lambda: ModeChart.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class ModeWorkspace(Mode):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in ModeWorkspace._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "mode_collection_count",
-        "mode_collections",
-    ]
-
-    @property
-    def mode_collection_count(self) -> Optional[int]:
-        return self.attributes.mode_collection_count
-
-    @mode_collection_count.setter
-    def mode_collection_count(self, mode_collection_count: Optional[int]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.mode_collection_count = mode_collection_count
-
-    @property
-    def mode_collections(self) -> Optional[list[ModeCollection]]:
-        return self.attributes.mode_collections
-
-    @mode_collections.setter
-    def mode_collections(self, mode_collections: Optional[list[ModeCollection]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.mode_collections = mode_collections
-
-    type_name: str = Field("ModeWorkspace", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "ModeWorkspace":
-            raise ValueError("must be ModeWorkspace")
-        return v
-
-    class Attributes(Mode.Attributes):
-        mode_collection_count: Optional[int] = Field(
-            None, description="", alias="modeCollectionCount"
-        )
-        mode_collections: Optional[list[ModeCollection]] = Field(
-            None, description="", alias="modeCollections"
-        )  # relationship
-
-    attributes: "ModeWorkspace.Attributes" = Field(
-        default_factory=lambda: ModeWorkspace.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class ModeCollection(Mode):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in ModeCollection._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "mode_collection_type",
-        "mode_collection_state",
-        "mode_workspace",
-        "mode_reports",
-    ]
-
-    @property
-    def mode_collection_type(self) -> Optional[str]:
-        return self.attributes.mode_collection_type
-
-    @mode_collection_type.setter
-    def mode_collection_type(self, mode_collection_type: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.mode_collection_type = mode_collection_type
-
-    @property
-    def mode_collection_state(self) -> Optional[str]:
-        return self.attributes.mode_collection_state
-
-    @mode_collection_state.setter
-    def mode_collection_state(self, mode_collection_state: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.mode_collection_state = mode_collection_state
-
-    @property
-    def mode_workspace(self) -> Optional[ModeWorkspace]:
-        return self.attributes.mode_workspace
-
-    @mode_workspace.setter
-    def mode_workspace(self, mode_workspace: Optional[ModeWorkspace]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.mode_workspace = mode_workspace
-
-    @property
-    def mode_reports(self) -> Optional[list[ModeReport]]:
-        return self.attributes.mode_reports
-
-    @mode_reports.setter
-    def mode_reports(self, mode_reports: Optional[list[ModeReport]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.mode_reports = mode_reports
-
-    type_name: str = Field("ModeCollection", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "ModeCollection":
-            raise ValueError("must be ModeCollection")
-        return v
-
-    class Attributes(Mode.Attributes):
-        mode_collection_type: Optional[str] = Field(
-            None, description="", alias="modeCollectionType"
-        )
-        mode_collection_state: Optional[str] = Field(
-            None, description="", alias="modeCollectionState"
-        )
-        mode_workspace: Optional[ModeWorkspace] = Field(
-            None, description="", alias="modeWorkspace"
-        )  # relationship
-        mode_reports: Optional[list[ModeReport]] = Field(
-            None, description="", alias="modeReports"
-        )  # relationship
-
-    attributes: "ModeCollection.Attributes" = Field(
-        default_factory=lambda: ModeCollection.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
 class SigmaDatasetColumn(Sigma):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in SigmaDatasetColumn._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -18253,14 +18464,448 @@
     attributes: "SigmaDataElement.Attributes" = Field(
         default_factory=lambda: SigmaDataElement.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
+class ModeReport(Mode):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in ModeReport._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "mode_collection_token",
+        "mode_report_published_at",
+        "mode_query_count",
+        "mode_chart_count",
+        "mode_query_preview",
+        "mode_is_public",
+        "mode_is_shared",
+        "mode_collections",
+        "mode_queries",
+    ]
+
+    @property
+    def mode_collection_token(self) -> Optional[str]:
+        return self.attributes.mode_collection_token
+
+    @mode_collection_token.setter
+    def mode_collection_token(self, mode_collection_token: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mode_collection_token = mode_collection_token
+
+    @property
+    def mode_report_published_at(self) -> Optional[datetime]:
+        return self.attributes.mode_report_published_at
+
+    @mode_report_published_at.setter
+    def mode_report_published_at(self, mode_report_published_at: Optional[datetime]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mode_report_published_at = mode_report_published_at
+
+    @property
+    def mode_query_count(self) -> Optional[int]:
+        return self.attributes.mode_query_count
+
+    @mode_query_count.setter
+    def mode_query_count(self, mode_query_count: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mode_query_count = mode_query_count
+
+    @property
+    def mode_chart_count(self) -> Optional[int]:
+        return self.attributes.mode_chart_count
+
+    @mode_chart_count.setter
+    def mode_chart_count(self, mode_chart_count: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mode_chart_count = mode_chart_count
+
+    @property
+    def mode_query_preview(self) -> Optional[str]:
+        return self.attributes.mode_query_preview
+
+    @mode_query_preview.setter
+    def mode_query_preview(self, mode_query_preview: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mode_query_preview = mode_query_preview
+
+    @property
+    def mode_is_public(self) -> Optional[bool]:
+        return self.attributes.mode_is_public
+
+    @mode_is_public.setter
+    def mode_is_public(self, mode_is_public: Optional[bool]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mode_is_public = mode_is_public
+
+    @property
+    def mode_is_shared(self) -> Optional[bool]:
+        return self.attributes.mode_is_shared
+
+    @mode_is_shared.setter
+    def mode_is_shared(self, mode_is_shared: Optional[bool]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mode_is_shared = mode_is_shared
+
+    @property
+    def mode_collections(self) -> Optional[list[ModeCollection]]:
+        return self.attributes.mode_collections
+
+    @mode_collections.setter
+    def mode_collections(self, mode_collections: Optional[list[ModeCollection]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mode_collections = mode_collections
+
+    @property
+    def mode_queries(self) -> Optional[list[ModeQuery]]:
+        return self.attributes.mode_queries
+
+    @mode_queries.setter
+    def mode_queries(self, mode_queries: Optional[list[ModeQuery]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mode_queries = mode_queries
+
+    type_name: str = Field("ModeReport", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "ModeReport":
+            raise ValueError("must be ModeReport")
+        return v
+
+    class Attributes(Mode.Attributes):
+        mode_collection_token: Optional[str] = Field(
+            None, description="", alias="modeCollectionToken"
+        )
+        mode_report_published_at: Optional[datetime] = Field(
+            None, description="", alias="modeReportPublishedAt"
+        )
+        mode_query_count: Optional[int] = Field(
+            None, description="", alias="modeQueryCount"
+        )
+        mode_chart_count: Optional[int] = Field(
+            None, description="", alias="modeChartCount"
+        )
+        mode_query_preview: Optional[str] = Field(
+            None, description="", alias="modeQueryPreview"
+        )
+        mode_is_public: Optional[bool] = Field(
+            None, description="", alias="modeIsPublic"
+        )
+        mode_is_shared: Optional[bool] = Field(
+            None, description="", alias="modeIsShared"
+        )
+        mode_collections: Optional[list[ModeCollection]] = Field(
+            None, description="", alias="modeCollections"
+        )  # relationship
+        mode_queries: Optional[list[ModeQuery]] = Field(
+            None, description="", alias="modeQueries"
+        )  # relationship
+
+    attributes: "ModeReport.Attributes" = Field(
+        default_factory=lambda: ModeReport.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class ModeQuery(Mode):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in ModeQuery._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "mode_raw_query",
+        "mode_report_import_count",
+        "mode_charts",
+        "mode_report",
+    ]
+
+    @property
+    def mode_raw_query(self) -> Optional[str]:
+        return self.attributes.mode_raw_query
+
+    @mode_raw_query.setter
+    def mode_raw_query(self, mode_raw_query: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mode_raw_query = mode_raw_query
+
+    @property
+    def mode_report_import_count(self) -> Optional[int]:
+        return self.attributes.mode_report_import_count
+
+    @mode_report_import_count.setter
+    def mode_report_import_count(self, mode_report_import_count: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mode_report_import_count = mode_report_import_count
+
+    @property
+    def mode_charts(self) -> Optional[list[ModeChart]]:
+        return self.attributes.mode_charts
+
+    @mode_charts.setter
+    def mode_charts(self, mode_charts: Optional[list[ModeChart]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mode_charts = mode_charts
+
+    @property
+    def mode_report(self) -> Optional[ModeReport]:
+        return self.attributes.mode_report
+
+    @mode_report.setter
+    def mode_report(self, mode_report: Optional[ModeReport]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mode_report = mode_report
+
+    type_name: str = Field("ModeQuery", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "ModeQuery":
+            raise ValueError("must be ModeQuery")
+        return v
+
+    class Attributes(Mode.Attributes):
+        mode_raw_query: Optional[str] = Field(
+            None, description="", alias="modeRawQuery"
+        )
+        mode_report_import_count: Optional[int] = Field(
+            None, description="", alias="modeReportImportCount"
+        )
+        mode_charts: Optional[list[ModeChart]] = Field(
+            None, description="", alias="modeCharts"
+        )  # relationship
+        mode_report: Optional[ModeReport] = Field(
+            None, description="", alias="modeReport"
+        )  # relationship
+
+    attributes: "ModeQuery.Attributes" = Field(
+        default_factory=lambda: ModeQuery.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class ModeChart(Mode):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in ModeChart._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "mode_chart_type",
+        "mode_query",
+    ]
+
+    @property
+    def mode_chart_type(self) -> Optional[str]:
+        return self.attributes.mode_chart_type
+
+    @mode_chart_type.setter
+    def mode_chart_type(self, mode_chart_type: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mode_chart_type = mode_chart_type
+
+    @property
+    def mode_query(self) -> Optional[ModeQuery]:
+        return self.attributes.mode_query
+
+    @mode_query.setter
+    def mode_query(self, mode_query: Optional[ModeQuery]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mode_query = mode_query
+
+    type_name: str = Field("ModeChart", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "ModeChart":
+            raise ValueError("must be ModeChart")
+        return v
+
+    class Attributes(Mode.Attributes):
+        mode_chart_type: Optional[str] = Field(
+            None, description="", alias="modeChartType"
+        )
+        mode_query: Optional[ModeQuery] = Field(
+            None, description="", alias="modeQuery"
+        )  # relationship
+
+    attributes: "ModeChart.Attributes" = Field(
+        default_factory=lambda: ModeChart.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class ModeWorkspace(Mode):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in ModeWorkspace._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "mode_collection_count",
+        "mode_collections",
+    ]
+
+    @property
+    def mode_collection_count(self) -> Optional[int]:
+        return self.attributes.mode_collection_count
+
+    @mode_collection_count.setter
+    def mode_collection_count(self, mode_collection_count: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mode_collection_count = mode_collection_count
+
+    @property
+    def mode_collections(self) -> Optional[list[ModeCollection]]:
+        return self.attributes.mode_collections
+
+    @mode_collections.setter
+    def mode_collections(self, mode_collections: Optional[list[ModeCollection]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mode_collections = mode_collections
+
+    type_name: str = Field("ModeWorkspace", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "ModeWorkspace":
+            raise ValueError("must be ModeWorkspace")
+        return v
+
+    class Attributes(Mode.Attributes):
+        mode_collection_count: Optional[int] = Field(
+            None, description="", alias="modeCollectionCount"
+        )
+        mode_collections: Optional[list[ModeCollection]] = Field(
+            None, description="", alias="modeCollections"
+        )  # relationship
+
+    attributes: "ModeWorkspace.Attributes" = Field(
+        default_factory=lambda: ModeWorkspace.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class ModeCollection(Mode):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in ModeCollection._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "mode_collection_type",
+        "mode_collection_state",
+        "mode_workspace",
+        "mode_reports",
+    ]
+
+    @property
+    def mode_collection_type(self) -> Optional[str]:
+        return self.attributes.mode_collection_type
+
+    @mode_collection_type.setter
+    def mode_collection_type(self, mode_collection_type: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mode_collection_type = mode_collection_type
+
+    @property
+    def mode_collection_state(self) -> Optional[str]:
+        return self.attributes.mode_collection_state
+
+    @mode_collection_state.setter
+    def mode_collection_state(self, mode_collection_state: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mode_collection_state = mode_collection_state
+
+    @property
+    def mode_workspace(self) -> Optional[ModeWorkspace]:
+        return self.attributes.mode_workspace
+
+    @mode_workspace.setter
+    def mode_workspace(self, mode_workspace: Optional[ModeWorkspace]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mode_workspace = mode_workspace
+
+    @property
+    def mode_reports(self) -> Optional[list[ModeReport]]:
+        return self.attributes.mode_reports
+
+    @mode_reports.setter
+    def mode_reports(self, mode_reports: Optional[list[ModeReport]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mode_reports = mode_reports
+
+    type_name: str = Field("ModeCollection", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "ModeCollection":
+            raise ValueError("must be ModeCollection")
+        return v
+
+    class Attributes(Mode.Attributes):
+        mode_collection_type: Optional[str] = Field(
+            None, description="", alias="modeCollectionType"
+        )
+        mode_collection_state: Optional[str] = Field(
+            None, description="", alias="modeCollectionState"
+        )
+        mode_workspace: Optional[ModeWorkspace] = Field(
+            None, description="", alias="modeWorkspace"
+        )  # relationship
+        mode_reports: Optional[list[ModeReport]] = Field(
+            None, description="", alias="modeReports"
+        )  # relationship
+
+    attributes: "ModeCollection.Attributes" = Field(
+        default_factory=lambda: ModeCollection.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
 class QlikSpace(Qlik):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in QlikSpace._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -19657,56 +20302,14 @@
     attributes: "TableauMetric.Attributes" = Field(
         default_factory=lambda: TableauMetric.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
-class TableauSite(Tableau):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in TableauSite._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "projects",
-    ]
-
-    @property
-    def projects(self) -> Optional[list[TableauProject]]:
-        return self.attributes.projects
-
-    @projects.setter
-    def projects(self, projects: Optional[list[TableauProject]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.projects = projects
-
-    type_name: str = Field("TableauSite", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "TableauSite":
-            raise ValueError("must be TableauSite")
-        return v
-
-    class Attributes(Tableau.Attributes):
-        projects: Optional[list[TableauProject]] = Field(
-            None, description="", alias="projects"
-        )  # relationship
-
-    attributes: "TableauSite.Attributes" = Field(
-        default_factory=lambda: TableauSite.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
 class TableauDatasource(Tableau):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in TableauDatasource._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -19951,14 +20554,56 @@
     attributes: "TableauDatasource.Attributes" = Field(
         default_factory=lambda: TableauDatasource.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
+class TableauSite(Tableau):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in TableauSite._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "projects",
+    ]
+
+    @property
+    def projects(self) -> Optional[list[TableauProject]]:
+        return self.attributes.projects
+
+    @projects.setter
+    def projects(self, projects: Optional[list[TableauProject]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.projects = projects
+
+    type_name: str = Field("TableauSite", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "TableauSite":
+            raise ValueError("must be TableauSite")
+        return v
+
+    class Attributes(Tableau.Attributes):
+        projects: Optional[list[TableauProject]] = Field(
+            None, description="", alias="projects"
+        )  # relationship
+
+    attributes: "TableauSite.Attributes" = Field(
+        default_factory=lambda: TableauSite.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
 class TableauDashboard(Tableau):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in TableauDashboard._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -22691,48 +23336,52 @@
 Referenceable.update_forward_refs()
 AtlasGlossary.update_forward_refs()
 
 Referenceable.Attributes.update_forward_refs()
 
 Asset.Attributes.update_forward_refs()
 
-AtlasGlossary.Attributes.update_forward_refs()
-
 DataSet.Attributes.update_forward_refs()
 
-ProcessExecution.Attributes.update_forward_refs()
-
-AtlasGlossaryTerm.Attributes.update_forward_refs()
-
-Cloud.Attributes.update_forward_refs()
-
-Infrastructure.Attributes.update_forward_refs()
-
 Connection.Attributes.update_forward_refs()
 
 Process.Attributes.update_forward_refs()
 
 AtlasGlossaryCategory.Attributes.update_forward_refs()
 
 Badge.Attributes.update_forward_refs()
 
+AccessControl.Attributes.update_forward_refs()
+
 Namespace.Attributes.update_forward_refs()
 
 Catalog.Attributes.update_forward_refs()
 
-Google.Attributes.update_forward_refs()
+AtlasGlossary.Attributes.update_forward_refs()
 
-Azure.Attributes.update_forward_refs()
+AuthPolicy.Attributes.update_forward_refs()
 
-AWS.Attributes.update_forward_refs()
+ProcessExecution.Attributes.update_forward_refs()
+
+AtlasGlossaryTerm.Attributes.update_forward_refs()
+
+AuthService.Attributes.update_forward_refs()
+
+Cloud.Attributes.update_forward_refs()
+
+Infrastructure.Attributes.update_forward_refs()
 
 BIProcess.Attributes.update_forward_refs()
 
 ColumnProcess.Attributes.update_forward_refs()
 
+Persona.Attributes.update_forward_refs()
+
+Purpose.Attributes.update_forward_refs()
+
 Collection.Attributes.update_forward_refs()
 
 Folder.Attributes.update_forward_refs()
 
 EventStore.Attributes.update_forward_refs()
 
 ObjectStore.Attributes.update_forward_refs()
@@ -22751,46 +23400,50 @@
 
 API.Attributes.update_forward_refs()
 
 Tag.Attributes.update_forward_refs()
 
 SQL.Attributes.update_forward_refs()
 
-DataStudio.Attributes.update_forward_refs()
+Google.Attributes.update_forward_refs()
 
-GCS.Attributes.update_forward_refs()
+Azure.Attributes.update_forward_refs()
 
-DataStudioAsset.Attributes.update_forward_refs()
+AWS.Attributes.update_forward_refs()
 
-ADLS.Attributes.update_forward_refs()
+DbtColumnProcess.Attributes.update_forward_refs()
+
+Kafka.Attributes.update_forward_refs()
 
 S3.Attributes.update_forward_refs()
 
-DbtColumnProcess.Attributes.update_forward_refs()
+ADLS.Attributes.update_forward_refs()
 
-Kafka.Attributes.update_forward_refs()
+GCS.Attributes.update_forward_refs()
 
 MonteCarlo.Attributes.update_forward_refs()
 
 Metric.Attributes.update_forward_refs()
 
+DataStudio.Attributes.update_forward_refs()
+
 Metabase.Attributes.update_forward_refs()
 
 QuickSight.Attributes.update_forward_refs()
 
 Thoughtspot.Attributes.update_forward_refs()
 
 PowerBI.Attributes.update_forward_refs()
 
 Preset.Attributes.update_forward_refs()
 
-Mode.Attributes.update_forward_refs()
-
 Sigma.Attributes.update_forward_refs()
 
+Mode.Attributes.update_forward_refs()
+
 Qlik.Attributes.update_forward_refs()
 
 Tableau.Attributes.update_forward_refs()
 
 Looker.Attributes.update_forward_refs()
 
 Redash.Attributes.update_forward_refs()
@@ -22827,43 +23480,45 @@
 
 Query.Attributes.update_forward_refs()
 
 Column.Attributes.update_forward_refs()
 
 Schema.Attributes.update_forward_refs()
 
+Database.Attributes.update_forward_refs()
+
 SnowflakeStream.Attributes.update_forward_refs()
 
 SnowflakePipe.Attributes.update_forward_refs()
 
-Database.Attributes.update_forward_refs()
-
 Procedure.Attributes.update_forward_refs()
 
 View.Attributes.update_forward_refs()
 
 MaterialisedView.Attributes.update_forward_refs()
 
-GCSObject.Attributes.update_forward_refs()
+DataStudioAsset.Attributes.update_forward_refs()
 
-GCSBucket.Attributes.update_forward_refs()
+KafkaTopic.Attributes.update_forward_refs()
+
+KafkaConsumerGroup.Attributes.update_forward_refs()
+
+S3Bucket.Attributes.update_forward_refs()
+
+S3Object.Attributes.update_forward_refs()
 
 ADLSAccount.Attributes.update_forward_refs()
 
 ADLSContainer.Attributes.update_forward_refs()
 
 ADLSObject.Attributes.update_forward_refs()
 
-S3Bucket.Attributes.update_forward_refs()
-
-S3Object.Attributes.update_forward_refs()
-
-KafkaTopic.Attributes.update_forward_refs()
+GCSObject.Attributes.update_forward_refs()
 
-KafkaConsumerGroup.Attributes.update_forward_refs()
+GCSBucket.Attributes.update_forward_refs()
 
 MCIncident.Attributes.update_forward_refs()
 
 MCMonitor.Attributes.update_forward_refs()
 
 MetabaseQuestion.Attributes.update_forward_refs()
 
@@ -22871,20 +23526,20 @@
 
 MetabaseDashboard.Attributes.update_forward_refs()
 
 QuickSightFolder.Attributes.update_forward_refs()
 
 QuickSightDashboardVisual.Attributes.update_forward_refs()
 
+QuickSightAnalysis.Attributes.update_forward_refs()
+
 QuickSightAnalysisVisual.Attributes.update_forward_refs()
 
 QuickSightDatasetField.Attributes.update_forward_refs()
 
-QuickSightAnalysis.Attributes.update_forward_refs()
-
 QuickSightDashboard.Attributes.update_forward_refs()
 
 QuickSightDataset.Attributes.update_forward_refs()
 
 ThoughtspotLiveboard.Attributes.update_forward_refs()
 
 ThoughtspotDashlet.Attributes.update_forward_refs()
@@ -22893,60 +23548,60 @@
 
 PowerBIReport.Attributes.update_forward_refs()
 
 PowerBIMeasure.Attributes.update_forward_refs()
 
 PowerBIColumn.Attributes.update_forward_refs()
 
-PowerBITable.Attributes.update_forward_refs()
-
 PowerBITile.Attributes.update_forward_refs()
 
+PowerBITable.Attributes.update_forward_refs()
+
 PowerBIDatasource.Attributes.update_forward_refs()
 
 PowerBIWorkspace.Attributes.update_forward_refs()
 
 PowerBIDataset.Attributes.update_forward_refs()
 
 PowerBIDashboard.Attributes.update_forward_refs()
 
-PowerBIDataflow.Attributes.update_forward_refs()
-
 PowerBIPage.Attributes.update_forward_refs()
 
+PowerBIDataflow.Attributes.update_forward_refs()
+
 PresetChart.Attributes.update_forward_refs()
 
 PresetDataset.Attributes.update_forward_refs()
 
 PresetDashboard.Attributes.update_forward_refs()
 
 PresetWorkspace.Attributes.update_forward_refs()
 
-ModeReport.Attributes.update_forward_refs()
-
-ModeQuery.Attributes.update_forward_refs()
-
-ModeChart.Attributes.update_forward_refs()
-
-ModeWorkspace.Attributes.update_forward_refs()
-
-ModeCollection.Attributes.update_forward_refs()
-
 SigmaDatasetColumn.Attributes.update_forward_refs()
 
 SigmaDataset.Attributes.update_forward_refs()
 
 SigmaWorkbook.Attributes.update_forward_refs()
 
 SigmaDataElementField.Attributes.update_forward_refs()
 
 SigmaPage.Attributes.update_forward_refs()
 
 SigmaDataElement.Attributes.update_forward_refs()
 
+ModeReport.Attributes.update_forward_refs()
+
+ModeQuery.Attributes.update_forward_refs()
+
+ModeChart.Attributes.update_forward_refs()
+
+ModeWorkspace.Attributes.update_forward_refs()
+
+ModeCollection.Attributes.update_forward_refs()
+
 QlikSpace.Attributes.update_forward_refs()
 
 QlikApp.Attributes.update_forward_refs()
 
 QlikChart.Attributes.update_forward_refs()
 
 QlikDataset.Attributes.update_forward_refs()
@@ -22959,18 +23614,18 @@
 
 TableauCalculatedField.Attributes.update_forward_refs()
 
 TableauProject.Attributes.update_forward_refs()
 
 TableauMetric.Attributes.update_forward_refs()
 
-TableauSite.Attributes.update_forward_refs()
-
 TableauDatasource.Attributes.update_forward_refs()
 
+TableauSite.Attributes.update_forward_refs()
+
 TableauDashboard.Attributes.update_forward_refs()
 
 TableauFlow.Attributes.update_forward_refs()
 
 TableauWorksheet.Attributes.update_forward_refs()
 
 LookerLook.Attributes.update_forward_refs()
```

### Comparing `pyatlan-0.0.33/pyatlan/model/core.py` & `pyatlan-0.1.0/pyatlan/model/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
 from typing import TYPE_CHECKING
 
-from pydantic import BaseModel, Extra, Field
+from pydantic import BaseModel, Extra, Field, validator
 
 if TYPE_CHECKING:
     from dataclasses import dataclass
 else:
     from pydantic.dataclasses import dataclass
 
 from datetime import datetime
@@ -180,24 +180,26 @@
         "entity object of the related entity.\n",
     )
 
 
 class AssetRequest(AtlanObject, GenericModel, Generic[T]):
     entity: T
 
+    @validator("entity")
+    def flush_custom_metadata(cls, v):
+        from pyatlan.model.assets import Asset
+
+        if isinstance(v, Asset):
+            v.flush_custom_metadata()
+        return v
+
 
 class BulkRequest(AtlanObject, GenericModel, Generic[T]):
     entities: list[T]
 
-
-class CustomMetadata(dict):
-    _meta_data_type_name = ""
-    _meta_data_type_id = ""
-
-    def __setattr__(self, key, value):
-        if not hasattr(self, key):
-            raise AttributeError(f"Attribute {key} does not exist")
-        super().__setattr__(key, value)
-
-
-class CustomMetadataReqest(AtlanObject):
-    __root__: CustomMetadata
+    @validator("entities", each_item=True)
+    def flush_custom_metadata(cls, v):
+        from pyatlan.model.assets import Asset
+
+        if isinstance(v, Asset):
+            v.flush_custom_metadata()
+        return v
```

### Comparing `pyatlan-0.0.33/pyatlan/model/enums.py` & `pyatlan-0.1.0/pyatlan/model/enums.py`

 * *Files 8% similar despite different names*

```diff
@@ -285,14 +285,29 @@
     SINGLESTORE = ("singlestore", AtlanConnectionCategory.WAREHOUSE)
     FIREBIRD = ("firebird", AtlanConnectionCategory.DATABASE)
     THOUGHTSPOT = ("thoughtspot", AtlanConnectionCategory.BI)
     CLICKHOUSE = ("clickhouse", AtlanConnectionCategory.WAREHOUSE)
     MULESOFT = ("mulesoft", AtlanConnectionCategory.API)
     CLARI = ("clari", AtlanConnectionCategory.SAAS)
     MARKETO = ("marketo", AtlanConnectionCategory.SAAS)
+    AZURE_DATA_LAKE = ("azure-data-lake", AtlanConnectionCategory.LAKE)
+    DELTA_LAKE = ("delta-lake", AtlanConnectionCategory.LAKE)
+    MINISQL = ("minisql", AtlanConnectionCategory.DATABASE)
+    ICEBERG = ("iceberg", AtlanConnectionCategory.WAREHOUSE)
+    IMPALA = ("impala", AtlanConnectionCategory.WAREHOUSE)
+    SPARK_SQL = ("spark-sql", AtlanConnectionCategory.LAKE)
+    MARIADB = ("mariadb", AtlanConnectionCategory.DATABASE)
+    FIREBOLT = ("firebolt", AtlanConnectionCategory.WAREHOUSE)
+    CLOUDERA_DATA_WAREHOUSE = (
+        "cloudera-data-warehouse",
+        AtlanConnectionCategory.WAREHOUSE,
+    )
+    STARBURST_GALAXY = ("starburst-galaxy", AtlanConnectionCategory.WAREHOUSE)
+    REDIS = ("redis", AtlanConnectionCategory.DATABASE)
+    GRAPHQL = ("graphql", AtlanConnectionCategory.DATABASE)
 
 
 class AtlanCustomAttributePrimitiveType(str, Enum):
     def __new__(cls, value: str) -> "AtlanCustomAttributePrimitiveType":
         obj = str.__new__(cls, value)
         obj._value_ = value
         return obj
@@ -316,14 +331,18 @@
 
 class LineageDirection(str, Enum):
     UPSTREAM = "INPUT"
     DOWNSTREAM = "OUTPUT"
     BOTH = "BOTH"
 
 
+class AtlanComparisonOperator(str, Enum):
+    CONTAINS = "contains"
+
+
 class BadgeComparisonOperator(str, Enum):
     GT = "gt"
     GTE = "gte"
     LT = "lt"
     LTE = "lte"
     EQ = "eq"
     NEQ = "neq"
@@ -348,7 +367,46 @@
     ZIP = "zip"
 
 
 class AtlanClassificationColor(str, Enum):
     GREEN = "Green"
     YELLOW = "Yellow"
     RED = "Red"
+
+
+class QueryParserSourceType(str, Enum):
+    ANSI = "ansi"
+    BIGQUERY = "bigquery"
+    HANA = "hana"
+    HIVE = "hive"
+    MSSQL = "mssql"
+    MYSQL = "mysql"
+    ORACLE = "oracle"
+    POSTGRESQL = "postgresql"
+    REDSHIFT = "redshift"
+    SNOWFLAKE = "snowflake"
+    SPARKSQL = "sparksql"
+    ATHENA = "athena"
+
+
+class AuthPolicyType(str, Enum):
+    ALLOW = "allow"
+    DENY = "deny"
+    ALLOWEXCEPTIONS = "allowExceptions"
+    DENYEXCEPTIONS = "denyExceptions"
+    DATAMASK = "dataMask"
+    ROWFILTER = "rowFilter"
+
+
+class AuthPolicyCategory(str, Enum):
+    BOOTSTRAP = "bootstrap"
+    PERSONA = "persona"
+    PURPOSE = "purpose"
+
+
+class AuthPolicyResourceCategory(str, Enum):
+    ENTITY = "ENTITY"
+    RELATIONSHIP = "RELATIONSHIP"
+    TAG = "TAG"
+    CUSTOM = "CUSTOM"
+    TYPEDEFS = "TYPEDEFS"
+    ADMIN = "ADMIN"
```

### Comparing `pyatlan-0.0.33/pyatlan/model/group.py` & `pyatlan-0.1.0/pyatlan/model/group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.33/pyatlan/model/response.py` & `pyatlan-0.1.0/pyatlan/model/response.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.33/pyatlan/model/role.py` & `pyatlan-0.1.0/pyatlan/model/role.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.33/pyatlan/model/search.py` & `pyatlan-0.1.0/pyatlan/model/search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.33/pyatlan/model/structs.py` & `pyatlan-0.1.0/pyatlan/model/structs.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,62 +12,64 @@
 )
 from pyatlan.utils import validate_required_fields
 
 
 class MCRuleSchedule(AtlanObject):
     """Description"""
 
-    mc_rule_schedule_type: Optional[str] = Field(
+    mc_rule_schedule_type: Optional["str"] = Field(
         None, description="", alias="mcRuleScheduleType"
     )
-    mc_rule_schedule_interval_in_minutes: Optional[int] = Field(
+    mc_rule_schedule_interval_in_minutes: Optional["int"] = Field(
         None, description="", alias="mcRuleScheduleIntervalInMinutes"
     )
-    mc_rule_schedule_start_time: Optional[datetime] = Field(
+    mc_rule_schedule_start_time: Optional["datetime"] = Field(
         None, description="", alias="mcRuleScheduleStartTime"
     )
-    mc_rule_schedule_crontab: Optional[str] = Field(
+    mc_rule_schedule_crontab: Optional["str"] = Field(
         None, description="", alias="mcRuleScheduleCrontab"
     )
 
 
 class AwsCloudWatchMetric(AtlanObject):
     """Description"""
 
-    aws_cloud_watch_metric_name: str = Field(
+    aws_cloud_watch_metric_name: "str" = Field(
         None, description="", alias="awsCloudWatchMetricName"
     )
-    aws_cloud_watch_metric_scope: str = Field(
+    aws_cloud_watch_metric_scope: "str" = Field(
         None, description="", alias="awsCloudWatchMetricScope"
     )
 
 
 class Histogram(AtlanObject):
     """Description"""
 
-    boundaries: set[float] = Field(None, description="", alias="boundaries")
-    frequencies: set[float] = Field(None, description="", alias="frequencies")
+    boundaries: "set[float]" = Field(None, description="", alias="boundaries")
+    frequencies: "set[float]" = Field(None, description="", alias="frequencies")
 
 
 class KafkaTopicConsumption(AtlanObject):
     """Description"""
 
-    topic_name: Optional[str] = Field(None, description="", alias="topicName")
-    topic_partition: Optional[str] = Field(None, description="", alias="topicPartition")
-    topic_lag: Optional[int] = Field(None, description="", alias="topicLag")
-    topic_current_offset: Optional[int] = Field(
+    topic_name: Optional["str"] = Field(None, description="", alias="topicName")
+    topic_partition: Optional["str"] = Field(
+        None, description="", alias="topicPartition"
+    )
+    topic_lag: Optional["int"] = Field(None, description="", alias="topicLag")
+    topic_current_offset: Optional["int"] = Field(
         None, description="", alias="topicCurrentOffset"
     )
 
 
 class ColumnValueFrequencyMap(AtlanObject):
     """Description"""
 
-    column_value: Optional[str] = Field(None, description="", alias="columnValue")
-    column_value_frequency: Optional[int] = Field(
+    column_value: Optional["str"] = Field(None, description="", alias="columnValue")
+    column_value_frequency: Optional["int"] = Field(
         None, description="", alias="columnValueFrequency"
     )
 
 
 class BadgeCondition(AtlanObject):
     """Description"""
 
@@ -92,165 +94,194 @@
             badge_condition_operator=badge_condition_operator.value,
             badge_condition_value=badge_condition_value,
             badge_condition_colorhex=badge_condition_colorhex.value
             if isinstance(badge_condition_colorhex, BadgeConditionColor)
             else badge_condition_colorhex,
         )
 
-    badge_condition_operator: Optional[str] = Field(
+    badge_condition_operator: Optional["str"] = Field(
         None, description="", alias="badgeConditionOperator"
     )
-    badge_condition_value: Optional[str] = Field(
+    badge_condition_value: Optional["str"] = Field(
         None, description="", alias="badgeConditionValue"
     )
-    badge_condition_colorhex: Optional[str] = Field(
+    badge_condition_colorhex: Optional["str"] = Field(
         None, description="", alias="badgeConditionColorhex"
     )
 
 
-class SourceTagAttachmentValue(AtlanObject):
-    """Description"""
-
-    tag_attachment_key: Optional[str] = Field(
-        None, description="", alias="tagAttachmentKey"
-    )
-    tag_attachment_value: Optional[str] = Field(
-        None, description="", alias="tagAttachmentValue"
-    )
-
-
 class SourceTagAttachment(AtlanObject):
     """Description"""
 
-    source_tag_name: Optional[str] = Field(None, description="", alias="sourceTagName")
-    source_tag_qualified_name: Optional[str] = Field(
+    source_tag_name: Optional["str"] = Field(
+        None, description="", alias="sourceTagName"
+    )
+    source_tag_qualified_name: Optional["str"] = Field(
         None, description="", alias="sourceTagQualifiedName"
     )
-    source_tag_guid: Optional[str] = Field(None, description="", alias="sourceTagGuid")
-    source_tag_connector_name: Optional[str] = Field(
+    source_tag_guid: Optional["str"] = Field(
+        None, description="", alias="sourceTagGuid"
+    )
+    source_tag_connector_name: Optional["str"] = Field(
         None, description="", alias="sourceTagConnectorName"
     )
-    source_tag_value: Optional[list[SourceTagAttachmentValue]] = Field(
+    source_tag_value: Optional["list[SourceTagAttachmentValue]"] = Field(
         None, description="", alias="sourceTagValue"
     )
-    is_source_tag_synced: Optional[bool] = Field(
+    is_source_tag_synced: Optional["bool"] = Field(
         None, description="", alias="isSourceTagSynced"
     )
-    source_tag_sync_timestamp: Optional[datetime] = Field(
+    source_tag_sync_timestamp: Optional["datetime"] = Field(
         None, description="", alias="sourceTagSyncTimestamp"
     )
-    source_tag_sync_error: Optional[str] = Field(
+    source_tag_sync_error: Optional["str"] = Field(
         None, description="", alias="sourceTagSyncError"
     )
 
 
+class SourceTagAttachmentValue(AtlanObject):
+    """Description"""
+
+    tag_attachment_key: Optional["str"] = Field(
+        None, description="", alias="tagAttachmentKey"
+    )
+    tag_attachment_value: Optional["str"] = Field(
+        None, description="", alias="tagAttachmentValue"
+    )
+
+
 class AzureTag(AtlanObject):
     """Description"""
 
-    azure_tag_key: str = Field(None, description="", alias="azureTagKey")
-    azure_tag_value: str = Field(None, description="", alias="azureTagValue")
+    azure_tag_key: "str" = Field(None, description="", alias="azureTagKey")
+    azure_tag_value: "str" = Field(None, description="", alias="azureTagValue")
+
+
+class AuthPolicyCondition(AtlanObject):
+    """Description"""
+
+    policy_condition_type: "str" = Field(
+        None, description="", alias="policyConditionType"
+    )
+    policy_condition_values: "set[str]" = Field(
+        None, description="", alias="policyConditionValues"
+    )
 
 
 class AwsTag(AtlanObject):
     """Description"""
 
-    aws_tag_key: str = Field(None, description="", alias="awsTagKey")
-    aws_tag_value: str = Field(None, description="", alias="awsTagValue")
+    aws_tag_key: "str" = Field(None, description="", alias="awsTagKey")
+    aws_tag_value: "str" = Field(None, description="", alias="awsTagValue")
 
 
 class DbtMetricFilter(AtlanObject):
     """Description"""
 
-    dbt_metric_filter_column_qualified_name: Optional[str] = Field(
+    dbt_metric_filter_column_qualified_name: Optional["str"] = Field(
         None, description="", alias="dbtMetricFilterColumnQualifiedName"
     )
-    dbt_metric_filter_field: Optional[str] = Field(
+    dbt_metric_filter_field: Optional["str"] = Field(
         None, description="", alias="dbtMetricFilterField"
     )
-    dbt_metric_filter_operator: Optional[str] = Field(
+    dbt_metric_filter_operator: Optional["str"] = Field(
         None, description="", alias="dbtMetricFilterOperator"
     )
-    dbt_metric_filter_value: Optional[str] = Field(
+    dbt_metric_filter_value: Optional["str"] = Field(
         None, description="", alias="dbtMetricFilterValue"
     )
 
 
 class GoogleTag(AtlanObject):
     """Description"""
 
-    google_tag_key: str = Field(None, description="", alias="googleTagKey")
-    google_tag_value: str = Field(None, description="", alias="googleTagValue")
+    google_tag_key: "str" = Field(None, description="", alias="googleTagKey")
+    google_tag_value: "str" = Field(None, description="", alias="googleTagValue")
+
+
+class AuthPolicyValiditySchedule(AtlanObject):
+    """Description"""
+
+    policy_validity_schedule_start_time: "str" = Field(
+        None, description="", alias="policyValidityScheduleStartTime"
+    )
+    policy_validity_schedule_end_time: "str" = Field(
+        None, description="", alias="policyValidityScheduleEndTime"
+    )
+    policy_validity_schedule_timezone: "str" = Field(
+        None, description="", alias="policyValidityScheduleTimezone"
+    )
 
 
 class MCRuleComparison(AtlanObject):
     """Description"""
 
-    mc_rule_comparison_type: Optional[str] = Field(
+    mc_rule_comparison_type: Optional["str"] = Field(
         None, description="", alias="mcRuleComparisonType"
     )
-    mc_rule_comparison_field: Optional[str] = Field(
+    mc_rule_comparison_field: Optional["str"] = Field(
         None, description="", alias="mcRuleComparisonField"
     )
-    mc_rule_comparison_metric: Optional[str] = Field(
+    mc_rule_comparison_metric: Optional["str"] = Field(
         None, description="", alias="mcRuleComparisonMetric"
     )
-    mc_rule_comparison_operator: Optional[str] = Field(
+    mc_rule_comparison_operator: Optional["str"] = Field(
         None, description="", alias="mcRuleComparisonOperator"
     )
-    mc_rule_comparison_threshold: Optional[float] = Field(
+    mc_rule_comparison_threshold: Optional["float"] = Field(
         None, description="", alias="mcRuleComparisonThreshold"
     )
-    mc_rule_comparison_is_threshold_relative: Optional[bool] = Field(
+    mc_rule_comparison_is_threshold_relative: Optional["bool"] = Field(
         None, description="", alias="mcRuleComparisonIsThresholdRelative"
     )
 
 
 class GoogleLabel(AtlanObject):
     """Description"""
 
-    google_label_key: str = Field(None, description="", alias="googleLabelKey")
-    google_label_value: str = Field(None, description="", alias="googleLabelValue")
+    google_label_key: "str" = Field(None, description="", alias="googleLabelKey")
+    google_label_value: "str" = Field(None, description="", alias="googleLabelValue")
 
 
 class PopularityInsights(AtlanObject):
     """Description"""
 
-    record_user: Optional[str] = Field(None, description="", alias="recordUser")
-    record_query: Optional[str] = Field(None, description="", alias="recordQuery")
-    record_query_duration: Optional[int] = Field(
+    record_user: Optional["str"] = Field(None, description="", alias="recordUser")
+    record_query: Optional["str"] = Field(None, description="", alias="recordQuery")
+    record_query_duration: Optional["int"] = Field(
         None, description="", alias="recordQueryDuration"
     )
-    record_query_count: Optional[int] = Field(
+    record_query_count: Optional["int"] = Field(
         None, description="", alias="recordQueryCount"
     )
-    record_total_user_count: Optional[int] = Field(
+    record_total_user_count: Optional["int"] = Field(
         None, description="", alias="recordTotalUserCount"
     )
-    record_compute_cost: Optional[float] = Field(
+    record_compute_cost: Optional["float"] = Field(
         None, description="", alias="recordComputeCost"
     )
-    record_max_compute_cost: Optional[float] = Field(
+    record_max_compute_cost: Optional["float"] = Field(
         None, description="", alias="recordMaxComputeCost"
     )
-    record_compute_cost_unit: Optional[SourceCostUnitType] = Field(
+    record_compute_cost_unit: Optional["SourceCostUnitType"] = Field(
         None, description="", alias="recordComputeCostUnit"
     )
-    record_last_timestamp: Optional[datetime] = Field(
+    record_last_timestamp: Optional["datetime"] = Field(
         None, description="", alias="recordLastTimestamp"
     )
-    record_warehouse: Optional[str] = Field(
+    record_warehouse: Optional["str"] = Field(
         None, description="", alias="recordWarehouse"
     )
 
 
 class SourceTagAttribute(AtlanObject):
     """Description"""
 
-    tag_attribute_key: Optional[str] = Field(
+    tag_attribute_key: Optional["str"] = Field(
         None, description="", alias="tagAttributeKey"
     )
-    tag_attribute_value: Optional[str] = Field(
+    tag_attribute_value: Optional["str"] = Field(
         None, description="", alias="tagAttributeValue"
     )
-    tag_attribute_properties: Optional[dict[str, str]] = Field(
+    tag_attribute_properties: Optional["dict[str,str]"] = Field(
         None, description="", alias="tagAttributeProperties"
     )
```

### Comparing `pyatlan-0.0.33/pyatlan/model/typedef.py` & `pyatlan-0.1.0/pyatlan/model/typedef.py`

 * *Files identical despite different names*

```diff
@@ -585,15 +585,15 @@
             from pyatlan.model.assets import validate_required_fields
 
             validate_required_fields(
                 ["emoji"],
                 [emoji],
             )
             return CustomMetadataDef.Options(
-                emoji=emoji, logo_type="emoji", is_locked=locked
+                emoji=emoji, logo_type="emoji", is_locked=str(locked).lower()
             )
 
         @staticmethod
         def with_logo_from_url(
             url: str, locked: bool = False
         ) -> CustomMetadataDef.Options:
             from pyatlan.model.assets import validate_required_fields
```

### Comparing `pyatlan-0.0.33/pyatlan/model/user.py` & `pyatlan-0.1.0/pyatlan/model/user.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.33/pyatlan/utils.py` & `pyatlan-0.1.0/pyatlan/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import logging
 import time
 from functools import reduce
 from typing import Any, Optional
 
 ADMIN_URI = "api/service/"
 BASE_URI = "api/meta/"
+SQL_URI = "api/sql/"
 APPLICATION_JSON = "application/json"
 APPLICATION_OCTET_STREAM = "application/octet-stream"
 MULTIPART_FORM_DATA = "multipart/form-data"
 PREFIX_ATTR = "attr:"
 PREFIX_ATTR_ = "attr_"
 
 s_nextId = milliseconds = int(round(time.time() * 1000)) + 1
```

### Comparing `pyatlan-0.0.33/pyatlan.egg-info/PKG-INFO` & `pyatlan-0.1.0/pyatlan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.0.33
+Version: 0.1.0
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.0.33/pyatlan.egg-info/SOURCES.txt` & `pyatlan-0.1.0/pyatlan.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -26,37 +26,44 @@
 pyatlan/client/constants.py
 pyatlan/generator/__init__.py
 pyatlan/generator/generate_from_typdefs.py
 pyatlan/generator/templates/__init__.py
 pyatlan/model/__init__.py
 pyatlan/model/assets.py
 pyatlan/model/core.py
+pyatlan/model/custom_metadata.py
 pyatlan/model/enums.py
 pyatlan/model/group.py
 pyatlan/model/internal.py
 pyatlan/model/lineage.py
+pyatlan/model/query.py
 pyatlan/model/response.py
 pyatlan/model/role.py
 pyatlan/model/search.py
 pyatlan/model/structs.py
 pyatlan/model/typedef.py
 pyatlan/model/user.py
 tests/__init__.py
 tests/conftest.py
 tests/integration/__init__.py
 tests/integration/admin_test.py
 tests/integration/classification_test.py
 tests/integration/client.py
+tests/integration/connection_test.py
 tests/integration/custom_metadata_test.py
 tests/integration/glossary_test.py
+tests/integration/lineage_test.py
+tests/integration/query_parser_test.py
+tests/integration/s3_asset_test.py
 tests/integration/test_client.py
 tests/integration/test_entity_model.py
 tests/integration/test_index_search.py
 tests/unit/__init__.py
 tests/unit/test_classification_name.py
 tests/unit/test_client.py
+tests/unit/test_custom_metadata.py
 tests/unit/test_glossary_term.py
 tests/unit/test_lineage.py
 tests/unit/test_model.py
 tests/unit/test_search_model.py
 tests/unit/test_typedef_model.py
 tests/unit/test_utils.py
```

### Comparing `pyatlan-0.0.33/setup.py` & `pyatlan-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.33/tests/integration/admin_test.py` & `pyatlan-0.1.0/tests/integration/admin_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,21 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
-from typing import Generator, Optional
+from typing import Callable, Generator, Optional
 
 import pytest
 from pydantic import StrictStr
 
 from pyatlan.cache.role_cache import RoleCache
-
 from pyatlan.client.atlan import AtlanClient
 from pyatlan.model.group import AtlanGroup, CreateGroupResponse
 from pyatlan.model.user import AtlanUser
 
-PREFIX = "psdk-Admin"
-GROUP_NAME1 = f"{PREFIX}1"
-GROUP_NAME2 = f"{PREFIX}2"
-
+MODULE_NAME = "Admin"
 EMAIL_DOMAIN = "@example.com"
-USER_EMAIL1 = f"{GROUP_NAME1}{EMAIL_DOMAIN}"
-USER_EMAIL2 = f"{GROUP_NAME2}{EMAIL_DOMAIN}"
-USER_EMAIL3 = f"{PREFIX}3{EMAIL_DOMAIN}"
 
 _default_group_count: int = 0
 
 
 def create_group(client: AtlanClient, name: str) -> CreateGroupResponse:
     g = AtlanGroup.create(alias=StrictStr(name))
     r = client.create_group(g)
@@ -35,158 +28,199 @@
 
 def test_retrieve_roles():
     admin_role_guid = RoleCache.get_id_for_name("$admin")
     assert admin_role_guid
 
 
 @pytest.fixture(scope="module")
-def group1(client: AtlanClient) -> Generator[CreateGroupResponse, None, None]:
-    g = create_group(client, GROUP_NAME1)
+def group1(
+    client: AtlanClient, make_unique: Callable[[str], str]
+) -> Generator[CreateGroupResponse, None, None]:
+    group_name = make_unique(f"{MODULE_NAME}1")
+    g = create_group(client, group_name)
     yield g
     delete_group(client, g.group)
 
 
-def test_create_group1(client: AtlanClient, group1: CreateGroupResponse):
+def test_create_group1(
+    client: AtlanClient, make_unique: Callable[[str], str], group1: CreateGroupResponse
+):
     assert group1
-    r = client.get_group_by_name(GROUP_NAME1)
+    group_name = make_unique(f"{MODULE_NAME}1")
+    r = client.get_group_by_name(group_name)
     assert r
     assert len(r) == 1
     group1_full = r[0]
     assert group1_full
     assert group1_full.path
     assert group1_full.name
     assert group1_full.id == group1.group
     assert group1_full.attributes
     assert not group1_full.attributes.description
 
 
-def test_retrieve_all_groups(client: AtlanClient, group1: CreateGroupResponse):
+def test_retrieve_all_groups(
+    client: AtlanClient, make_unique: Callable[[str], str], group1: CreateGroupResponse
+):
     global _default_group_count
     groups = client.get_all_groups()
     assert groups
     assert len(groups) >= 1
     for group in groups:
         if group.is_default():
             _default_group_count += 1
 
 
 @pytest.mark.order(after="test_create_group1")
-def test_update_groups(client: AtlanClient, group1: CreateGroupResponse):
-    groups = client.get_group_by_name(alias=GROUP_NAME1)
+def test_update_groups(
+    client: AtlanClient, make_unique: Callable[[str], str], group1: CreateGroupResponse
+):
+    group_name = make_unique(f"{MODULE_NAME}1")
+    groups = client.get_group_by_name(alias=group_name)
     assert groups
     assert len(groups) == 1
     group = groups[0]
     group.attributes = AtlanGroup.Attributes(description=["Now with a description!"])
     client.update_group(group)
 
 
-def _get_user1_from_list(users: list[AtlanUser]) -> Optional[AtlanUser]:
-    return next((user for user in users if user.email == USER_EMAIL1.lower()), None)
-
-
-def _get_user2_from_list(users: list[AtlanUser]) -> Optional[AtlanUser]:
-    return next((user for user in users if user.email == USER_EMAIL2.lower()), None)
-
-
-def _get_user3_from_list(users: list[AtlanUser]) -> Optional[AtlanUser]:
-    return next((user for user in users if user.email == USER_EMAIL3.lower()), None)
+def _get_user1_from_list(
+    users: list[AtlanUser], make_unique: Callable[[str], str]
+) -> Optional[AtlanUser]:
+    username = make_unique(f"{MODULE_NAME}1")
+    user_email = f"{username}{EMAIL_DOMAIN}".lower()
+    return next((user for user in users if user.email == user_email), None)
+
+
+def _get_user2_from_list(
+    users: list[AtlanUser], make_unique: Callable[[str], str]
+) -> Optional[AtlanUser]:
+    username = make_unique(f"{MODULE_NAME}2")
+    user_email = f"{username}{EMAIL_DOMAIN}".lower()
+    return next((user for user in users if user.email == user_email), None)
+
+
+def _get_user3_from_list(
+    users: list[AtlanUser], make_unique: Callable[[str], str]
+) -> Optional[AtlanUser]:
+    username = make_unique(f"{MODULE_NAME}3")
+    user_email = f"{username}{EMAIL_DOMAIN}".lower()
+    return next((user for user in users if user.email == user_email), None)
 
 
 @pytest.fixture(scope="module")
-def users(client: AtlanClient) -> Generator[list[AtlanUser], None, None]:
+def users(
+    client: AtlanClient, make_unique: Callable[[str], str]
+) -> Generator[list[AtlanUser], None, None]:
+    username1 = make_unique(f"{MODULE_NAME}1")
+    username2 = make_unique(f"{MODULE_NAME}2")
+    username3 = make_unique(f"{MODULE_NAME}3")
+    user_email1 = f"{username1}{EMAIL_DOMAIN}"
+    user_email2 = f"{username2}{EMAIL_DOMAIN}"
+    user_email3 = f"{username3}{EMAIL_DOMAIN}"
     users: list[AtlanUser] = [
-        AtlanUser.create(email=USER_EMAIL1, role_name="$guest"),
-        AtlanUser.create(email=USER_EMAIL2, role_name="$guest"),
-        AtlanUser.create(email=USER_EMAIL3, role_name="$guest"),
+        AtlanUser.create(email=user_email1, role_name="$guest"),
+        AtlanUser.create(email=user_email2, role_name="$guest"),
+        AtlanUser.create(email=user_email3, role_name="$guest"),
     ]
     client.create_users(users=users)
     created = client.get_users_by_email(email=EMAIL_DOMAIN)
     assert created  # must be here for mypy
     yield created
     for user in created:
         client.purge_user(str(user.id))
 
 
 @pytest.mark.order(after="test_retrieve_all_groups")
-def test_retrieve_users(client: AtlanClient, users: list[AtlanUser]):
+def test_retrieve_users(
+    client: AtlanClient, make_unique: Callable[[str], str], users: list[AtlanUser]
+):
     global _default_group_count
     all_users = client.get_all_users()
     assert all_users
     assert len(all_users) >= 3
-    users_list = client.get_users_by_email(USER_EMAIL1)
+    username = make_unique(f"{MODULE_NAME}1")
+    user_email1 = f"{username}{EMAIL_DOMAIN}"
+    users_list = client.get_users_by_email(user_email1)
     assert users_list
     assert len(users_list) == 1
     user1 = users_list[0]
     assert user1
     assert user1.id
     assert user1.attributes
     assert not user1.attributes.designation
     assert user1.group_count == _default_group_count
     users_list = client.get_users_by_email(EMAIL_DOMAIN)
     assert users_list
     assert len(users_list) == 3
-    assert _get_user1_from_list(users)
-    assert _get_user2_from_list(users)
-    assert _get_user3_from_list(users)
+    assert _get_user1_from_list(users, make_unique)
+    assert _get_user2_from_list(users, make_unique)
+    assert _get_user3_from_list(users, make_unique)
 
 
 @pytest.fixture(scope="module")
 def group2(
-    client: AtlanClient, users: list[AtlanUser]
+    client: AtlanClient, make_unique: Callable[[str], str], users: list[AtlanUser]
 ) -> Generator[CreateGroupResponse, None, None]:
-    to_create = AtlanGroup.create(GROUP_NAME2)
-    user2 = _get_user2_from_list(users)
+    group_name = make_unique(f"{MODULE_NAME}2")
+    to_create = AtlanGroup.create(group_name)
+    user2 = _get_user2_from_list(users, make_unique)
     assert user2  # must be here for mypy
-    user3 = _get_user3_from_list(users)
+    user3 = _get_user3_from_list(users, make_unique)
     assert user3  # must be here for mypy
     g = client.create_group(group=to_create, user_ids=[str(user2.id), str(user3.id)])
     yield g
     delete_group(client, g.group)
 
 
 def test_create_group2(
-    client: AtlanClient, users: list[AtlanUser], group2: CreateGroupResponse
+    client: AtlanClient,
+    make_unique: Callable[[str], str],
+    users: list[AtlanUser],
+    group2: CreateGroupResponse,
 ):
     assert group2
     assert group2.group
     mapped_users = group2.users
     assert mapped_users
-    user2 = _get_user2_from_list(users)
+    user2 = _get_user2_from_list(users, make_unique)
     assert user2
     assert user2.id in mapped_users.keys()
     user_status = mapped_users.get(str(user2.id))
     assert user_status
     assert user_status.was_successful()
-    user3 = _get_user3_from_list(users)
+    user3 = _get_user3_from_list(users, make_unique)
     assert user3
     assert user3.id in mapped_users.keys()
     user_status = mapped_users.get(str(user3.id))
     assert user_status
     assert user_status.was_successful()
-    r = client.get_group_by_name(GROUP_NAME2)
+    group_name = make_unique(f"{MODULE_NAME}2")
+    r = client.get_group_by_name(group_name)
     assert r
     assert len(r) == 1
     group2_full = r[0]
     assert group2_full
     assert group2_full.path
     assert group2_full.name
     assert group2_full.id == group2.group
     assert group2_full.attributes
     assert not group2_full.attributes.description
 
 
 @pytest.mark.order(after="test_retrieve_all_groups")
 def test_update_users(
     client: AtlanClient,
+    make_unique: Callable[[str], str],
     users: list[AtlanUser],
     group1: CreateGroupResponse,
     group2: CreateGroupResponse,
 ):
     global _default_group_count
-    user1 = _get_user1_from_list(users)
+    user1 = _get_user1_from_list(users, make_unique)
     assert user1
     assert user1.id
     client.add_user_to_groups(guid=user1.id, group_ids=[group1.group])
     client.change_user_role(
         guid=user1.id, role_id=str(RoleCache.get_id_for_name("$member"))
     )
     response = client.get_groups_for_user(guid=user1.id)
@@ -194,81 +228,90 @@
     assert response.records
     assert len(response.records) == 1 + _default_group_count
 
 
 @pytest.mark.order(after="test_update_users")
 def test_updated_users(
     client: AtlanClient,
+    make_unique: Callable[[str], str],
     users: list[AtlanUser],
     group1: CreateGroupResponse,
     group2: CreateGroupResponse,
 ):
     global _default_group_count
-    candidates = client.get_users_by_email(USER_EMAIL1)
+    username = make_unique(f"{MODULE_NAME}1")
+    user_email = f"{username}{EMAIL_DOMAIN}"
+    candidates = client.get_users_by_email(user_email)
     assert candidates
     assert len(candidates) == 1
     one = candidates[0]
     assert one
-    user1 = _get_user1_from_list(users)
+    user1 = _get_user1_from_list(users, make_unique)
     assert user1
     assert one.id == user1.id
     assert one.group_count == 1 + _default_group_count
-    guest = client.get_user_by_username(GROUP_NAME1.lower())
+    group_name = make_unique(f"{MODULE_NAME}1")
+    guest = client.get_user_by_username(group_name.lower())
     assert guest
     assert guest == one
 
 
 @pytest.mark.order(after=["test_update_groups", "test_update_users"])
 def test_updated_groups(
     client: AtlanClient,
+    make_unique: Callable[[str], str],
     users: list[AtlanUser],
     group1: CreateGroupResponse,
     group2: CreateGroupResponse,
 ):
-    groups = client.get_group_by_name(alias=GROUP_NAME1)
+    group_name = make_unique(f"{MODULE_NAME}1")
+    groups = client.get_group_by_name(alias=group_name)
     assert groups
     assert len(groups) == 1
     group = groups[0]
     assert group
     assert group.id == group1.group
     assert group.attributes
     assert group.attributes.description == ["Now with a description!"]
     assert group.user_count == 1
 
 
 @pytest.mark.order(after="test_updated_groups")
 def test_remove_user_from_group(
     client: AtlanClient,
+    make_unique: Callable[[str], str],
     users: list[AtlanUser],
     group1: CreateGroupResponse,
     group2: CreateGroupResponse,
 ):
-    groups = client.get_group_by_name(alias=GROUP_NAME1)
+    group_name = make_unique(f"{MODULE_NAME}1")
+    groups = client.get_group_by_name(alias=group_name)
     assert groups
     assert len(groups) == 1
     group = groups[0]
     assert group.id
-    user1 = _get_user1_from_list(users)
+    user1 = _get_user1_from_list(users, make_unique)
     assert user1
     assert user1.id
     client.remove_users_from_group(guid=group.id, user_ids=[user1.id])
     response = client.get_group_members(guid=group.id)
     assert response
     assert not response.records
 
 
 @pytest.mark.order(after="test_remove_user_from_group")
 def test_final_user_state(
     client: AtlanClient,
+    make_unique: Callable[[str], str],
     users: list[AtlanUser],
     group1: CreateGroupResponse,
     group2: CreateGroupResponse,
 ):
     global _default_group_count
-    user1 = _get_user1_from_list(users)
+    user1 = _get_user1_from_list(users, make_unique)
     assert user1
     assert user1.id
     response = client.get_groups_for_user(user1.id)
     assert (
         response.records is None
         or len(response.records) == 0
         or len(response.records) == _default_group_count
```

### Comparing `pyatlan-0.0.33/tests/integration/classification_test.py` & `pyatlan-0.1.0/tests/integration/classification_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,19 +10,18 @@
 from pyatlan.client.atlan import AtlanClient
 from pyatlan.error import AtlanError
 from pyatlan.model.enums import AtlanClassificationColor
 from pyatlan.model.typedef import ClassificationDef
 
 LOGGER = logging.getLogger(__name__)
 
+MODULE_NAME = "CLS"
 
-CLS_NAME = "psdk-classification"
 
-
-@pytest.fixture(scope="module", autouse=True)
+@pytest.fixture(scope="module")
 def make_classification(
     client: AtlanClient,
 ) -> Generator[Callable[[str], ClassificationDef], None, None]:
     created_names = []
 
     @retry(
         AtlanError,
@@ -52,31 +51,39 @@
             _wait_for_successful_purge(n)
         except AtlanError as err:
             LOGGER.error(err)
 
 
 @pytest.fixture(scope="module")
 def classification_def(
-    client: AtlanClient, make_classification: Callable[[str], ClassificationDef]
+    client: AtlanClient,
+    make_unique: Callable[[str], str],
+    make_classification: Callable[[str], ClassificationDef],
 ) -> ClassificationDef:
-    return make_classification(CLS_NAME)
+    cls_name = make_unique(MODULE_NAME)
+    return make_classification(cls_name)
 
 
-def test_classification_def(classification_def: ClassificationDef):
+def test_classification_def(
+    classification_def: ClassificationDef, make_unique: Callable[[str], str]
+):
     assert classification_def
     assert classification_def.guid
-    assert classification_def.display_name == CLS_NAME
-    assert classification_def.name != CLS_NAME
+    assert classification_def.display_name == make_unique(MODULE_NAME)
+    assert classification_def.name != make_unique(MODULE_NAME)
     assert classification_def.options
     assert "color" in classification_def.options.keys()
     assert (
         classification_def.options.get("color") == AtlanClassificationColor.GREEN.value
     )
 
 
-def test_classification_cache(classification_def: ClassificationDef):
-    cls_id = ClassificationCache.get_id_for_name(CLS_NAME)
+def test_classification_cache(
+    classification_def: ClassificationDef, make_unique: Callable[[str], str]
+):
+    cls_name = make_unique(MODULE_NAME)
+    cls_id = ClassificationCache.get_id_for_name(cls_name)
     assert cls_id
     assert cls_id == classification_def.name
-    cls_name = ClassificationCache.get_name_for_id(cls_id)
-    assert cls_name
-    assert cls_name == CLS_NAME
+    cls_name_found = ClassificationCache.get_name_for_id(cls_id)
+    assert cls_name_found
+    assert cls_name_found == cls_name
```

### Comparing `pyatlan-0.0.33/tests/integration/custom_metadata_test.py` & `pyatlan-0.1.0/tests/integration/custom_metadata_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,93 +1,62 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
 import logging
 import time
-from typing import Generator, List, Optional, Tuple
+from typing import Callable, Generator, List, Optional, Tuple
 
 import pytest
 
 from pyatlan.cache.custom_metadata_cache import CustomMetadataCache
 from pyatlan.client.atlan import AtlanClient
-from pyatlan.error import NotFoundError
-from pyatlan.model.assets import (
-    AtlasGlossary,
-    AtlasGlossaryTerm,
-    Badge,
-    BadgeCondition,
-    Table,
-)
-from pyatlan.model.core import CustomMetadata, to_snake_case
+from pyatlan.model.assets import AtlasGlossary, AtlasGlossaryTerm, Badge, BadgeCondition
+from pyatlan.model.custom_metadata import CustomMetadataDict
 from pyatlan.model.enums import (
     AtlanCustomAttributePrimitiveType,
     AtlanTypeCategory,
     BadgeComparisonOperator,
     BadgeConditionColor,
 )
 from pyatlan.model.group import AtlanGroup, CreateGroupResponse
 from pyatlan.model.search import DSL, Bool, Exists, IndexSearchRequest, Term
 from pyatlan.model.typedef import AttributeDef, CustomMetadataDef, EnumDef
+from tests.integration.admin_test import create_group, delete_group
 from tests.integration.client import delete_asset
 from tests.integration.glossary_test import create_glossary, create_term
-from tests.integration.admin_test import create_group, delete_group
 
 LOGGER = logging.getLogger(__name__)
 
-PREFIX = "psdk-"
-CM_PREFIX = f"{PREFIX}CM"
+MODULE_NAME = "CM"
 FIXED_USER = "ernest"
 
-CM_RACI = f"{PREFIX}RACI"
-CM_IPR = f"{PREFIX}IPR"
-CM_QUALITY = f"{PREFIX}DQ"
-
 CM_ATTR_RACI_RESPONSIBLE = "Responsible"
 CM_ATTR_RACI_ACCOUNTABLE = "Accountable"
 CM_ATTR_RACI_CONSULTED = "Consulted"
 CM_ATTR_RACI_INFORMED = "Informed"
 CM_ATTR_RACI_EXTRA = "Extra"
 
-CM_ATTR_RACI_RESPONSIBLE_RENAMED = to_snake_case(CM_ATTR_RACI_RESPONSIBLE)
-CM_ATTR_RACI_ACCOUNTABLE_RENAMED = to_snake_case(CM_ATTR_RACI_ACCOUNTABLE)
-CM_ATTR_RACI_CONSULTED_RENAMED = to_snake_case(CM_ATTR_RACI_CONSULTED)
-CM_ATTR_RACI_INFORMED_RENAMED = to_snake_case(CM_ATTR_RACI_INFORMED)
-CM_ATTR_RACI_EXTRA_RENAMED = to_snake_case(CM_ATTR_RACI_EXTRA)
 
 CM_ATTR_IPR_LICENSE = "License"
 CM_ATTR_IPR_VERSION = "Version"
 CM_ATTR_IPR_MANDATORY = "Mandatory"
 CM_ATTR_IPR_DATE = "Date"
 CM_ATTR_IPR_URL = "URL"
 
-CM_ATTR_IPR_LICENSE_RENAMED = to_snake_case(CM_ATTR_IPR_LICENSE)
-CM_ATTR_IPR_VERSION_RENAMED = to_snake_case(CM_ATTR_IPR_VERSION)
-CM_ATTR_IPR_MANDATORY_RENAMED = to_snake_case(CM_ATTR_IPR_MANDATORY)
-CM_ATTR_IPR_DATE_RENAMED = to_snake_case(CM_ATTR_IPR_DATE)
-CM_ATTR_IPR_URL_RENAMED = to_snake_case(CM_ATTR_IPR_URL)
-
 CM_ATTR_QUALITY_COUNT = "Count"
 CM_ATTR_QUALITY_SQL = "SQL"
 CM_ATTR_QUALITY_TYPE = "Type"
-CM_ENUM_DQ_TYPE = f"{PREFIX.replace('-', '_')}DataQualityType"
 DQ_TYPE_LIST = [
     "Accuracy",
     "Completeness",
     "Consistency",
     "Timeliness",
     "Validity",
     "Uniqueness",
 ]
 
-CM_ATTR_QUALITY_COUNT_RENAMED = to_snake_case(CM_ATTR_QUALITY_COUNT)
-CM_ATTR_QUALITY_SQL_RENAMED = to_snake_case(CM_ATTR_QUALITY_SQL)
-CM_ATTR_QUALITY_TYPE_RENAMED = to_snake_case(CM_ATTR_QUALITY_TYPE)
-
-GROUP_NAME1 = f"{CM_PREFIX}1"
-GROUP_NAME2 = f"{CM_PREFIX}2"
-
 _removal_epoch: Optional[int]
 
 
 def create_custom_metadata(
     client: AtlanClient,
     name: str,
     attribute_defs: List[AttributeDef],
@@ -107,15 +76,18 @@
 def create_enum(client: AtlanClient, name: str, values: List[str]) -> EnumDef:
     enum_def = EnumDef.create(name=name, values=values)
     r = client.create_typedef(enum_def)
     return r.enum_defs[0]
 
 
 @pytest.fixture(scope="module")
-def cm_ipr(client: AtlanClient) -> Generator[CustomMetadataDef, None, None]:
+def cm_ipr(
+    client: AtlanClient,
+    make_unique: Callable[[str], str],
+) -> Generator[CustomMetadataDef, None, None]:
     attribute_defs = [
         AttributeDef.create(
             display_name=CM_ATTR_IPR_LICENSE,
             attribute_type=AtlanCustomAttributePrimitiveType.STRING,
         ),
         AttributeDef.create(
             display_name=CM_ATTR_IPR_VERSION,
@@ -130,26 +102,31 @@
             attribute_type=AtlanCustomAttributePrimitiveType.DATE,
         ),
         AttributeDef.create(
             display_name=CM_ATTR_IPR_URL,
             attribute_type=AtlanCustomAttributePrimitiveType.URL,
         ),
     ]
+    cm_name = make_unique("IPR")
     cm = create_custom_metadata(
-        client, name=CM_IPR, attribute_defs=attribute_defs, logo="⚖️", locked=False
+        client, name=cm_name, attribute_defs=attribute_defs, logo="⚖️", locked=True
     )
     yield cm
-    client.purge_typedef(CM_IPR, CustomMetadataDef)
+    client.purge_typedef(cm_name, CustomMetadataDef)
 
 
-def test_cm_ipr(cm_ipr: CustomMetadataDef):
+def test_cm_ipr(
+    cm_ipr: CustomMetadataDef,
+    make_unique: Callable[[str], str],
+):
+    cm_name = make_unique("IPR")
     assert cm_ipr.category == AtlanTypeCategory.CUSTOM_METADATA
     assert cm_ipr.guid
-    assert cm_ipr.name != CM_IPR
-    assert cm_ipr.display_name == CM_IPR
+    assert cm_ipr.name != cm_name
+    assert cm_ipr.display_name == cm_name
     attributes = cm_ipr.attribute_defs
     assert attributes
     assert len(attributes) == 5
     one = attributes[0]
     assert one
     assert one.display_name == CM_ATTR_IPR_LICENSE
     assert one.name
@@ -180,15 +157,18 @@
     assert one.name != CM_ATTR_IPR_URL
     assert one.type_name == AtlanCustomAttributePrimitiveType.STRING.value
     assert one.options
     assert not one.options.multi_value_select
 
 
 @pytest.fixture(scope="module")
-def cm_raci(client: AtlanClient) -> Generator[CustomMetadataDef, None, None]:
+def cm_raci(
+    client: AtlanClient,
+    make_unique: Callable[[str], str],
+) -> Generator[CustomMetadataDef, None, None]:
     attribute_defs = [
         AttributeDef.create(
             display_name=CM_ATTR_RACI_RESPONSIBLE,
             attribute_type=AtlanCustomAttributePrimitiveType.USERS,
             multi_valued=True,
         ),
         AttributeDef.create(
@@ -206,27 +186,32 @@
             multi_valued=True,
         ),
         AttributeDef.create(
             display_name=CM_ATTR_RACI_EXTRA,
             attribute_type=AtlanCustomAttributePrimitiveType.STRING,
         ),
     ]
+    cm_name = make_unique("RACI")
     cm = create_custom_metadata(
-        client, name=CM_RACI, attribute_defs=attribute_defs, logo="👪", locked=False
+        client, name=cm_name, attribute_defs=attribute_defs, logo="👪", locked=False
     )
     yield cm
-    client.purge_typedef(CM_RACI, CustomMetadataDef)
+    client.purge_typedef(cm_name, CustomMetadataDef)
 
 
-def test_cm_raci(cm_raci: CustomMetadataDef):
+def test_cm_raci(
+    cm_raci: CustomMetadataDef,
+    make_unique: Callable[[str], str],
+):
     assert cm_raci.category == AtlanTypeCategory.CUSTOM_METADATA
     assert cm_raci.name
     assert cm_raci.guid
-    assert cm_raci.name != CM_RACI
-    assert cm_raci.display_name == CM_RACI
+    cm_name = make_unique("RACI")
+    assert cm_raci.name != cm_name
+    assert cm_raci.display_name == cm_name
     attributes = cm_raci.attribute_defs
     assert attributes
     assert len(attributes) == 5
     one = attributes[0]
     assert one
     assert one.display_name == CM_ATTR_RACI_RESPONSIBLE
     assert one.name
@@ -257,66 +242,79 @@
     assert one.name != CM_ATTR_RACI_EXTRA
     assert one.type_name == AtlanCustomAttributePrimitiveType.STRING.value
     assert one.options
     assert not one.options.multi_value_select
 
 
 @pytest.fixture(scope="module")
-def cm_enum(client: AtlanClient) -> Generator[EnumDef, None, None]:
-    enum_def = create_enum(client, name=CM_ENUM_DQ_TYPE, values=DQ_TYPE_LIST)
+def cm_enum(
+    client: AtlanClient,
+    make_unique: Callable[[str], str],
+) -> Generator[EnumDef, None, None]:
+    dq_enum_name = make_unique(f"{MODULE_NAME}_DataQualityType")
+    enum_def = create_enum(client, name=dq_enum_name, values=DQ_TYPE_LIST)
     yield enum_def
-    client.purge_typedef(CM_ENUM_DQ_TYPE, EnumDef)
+    client.purge_typedef(dq_enum_name, EnumDef)
 
 
-def test_cm_enum(cm_enum: EnumDef):
+def test_cm_enum(
+    cm_enum: EnumDef,
+    make_unique: Callable[[str], str],
+):
     assert cm_enum.category == AtlanTypeCategory.ENUM
-    assert cm_enum.name == CM_ENUM_DQ_TYPE
+    assert cm_enum.name == make_unique(f"{MODULE_NAME}_DataQualityType")
     assert cm_enum.guid
     assert cm_enum.element_defs
     assert len(cm_enum.element_defs) == len(DQ_TYPE_LIST)
 
 
 @pytest.fixture(scope="module")
 def cm_dq(
     client: AtlanClient,
+    make_unique: Callable[[str], str],
     cm_enum: EnumDef,
 ) -> Generator[CustomMetadataDef, None, None]:
     attribute_defs = [
         AttributeDef.create(
             display_name=CM_ATTR_QUALITY_COUNT,
             attribute_type=AtlanCustomAttributePrimitiveType.INTEGER,
         ),
         AttributeDef.create(
             display_name=CM_ATTR_QUALITY_SQL,
             attribute_type=AtlanCustomAttributePrimitiveType.SQL,
         ),
         AttributeDef.create(
             display_name=CM_ATTR_QUALITY_TYPE,
             attribute_type=AtlanCustomAttributePrimitiveType.OPTIONS,
-            options_name=CM_ENUM_DQ_TYPE,
+            options_name=make_unique(f"{MODULE_NAME}_DataQualityType"),
         ),
     ]
+    cm_name = make_unique("DQ")
     cm = create_custom_metadata(
         client,
-        name=CM_QUALITY,
+        name=cm_name,
         attribute_defs=attribute_defs,
         logo="https://github.com/great-expectations/great_expectations/raw/develop/docs/docusaurus/static/img/"
         "gx-mark-160.png",
-        locked=False,
+        locked=True,
     )
     yield cm
-    client.purge_typedef(CM_QUALITY, CustomMetadataDef)
+    client.purge_typedef(cm_name, CustomMetadataDef)
 
 
-def test_cm_dq(cm_dq: CustomMetadataDef):
+def test_cm_dq(
+    cm_dq: CustomMetadataDef,
+    make_unique: Callable[[str], str],
+):
+    cm_name = make_unique("DQ")
     assert cm_dq.category == AtlanTypeCategory.CUSTOM_METADATA
     assert cm_dq.name
     assert cm_dq.guid
-    assert cm_dq.name != CM_QUALITY
-    assert cm_dq.display_name == CM_QUALITY
+    assert cm_dq.name != cm_name
+    assert cm_dq.display_name == cm_name
     attributes = cm_dq.attribute_defs
     assert attributes
     assert len(attributes) == 3
     one = attributes[0]
     assert one
     assert one.display_name == CM_ATTR_QUALITY_COUNT
     assert one.name
@@ -330,178 +328,218 @@
     assert one.type_name == AtlanCustomAttributePrimitiveType.STRING.value
     assert one.options
     assert not one.options.multi_value_select
     assert one.options.custom_type == AtlanCustomAttributePrimitiveType.SQL.value
     one = attributes[2]
     assert one.display_name == CM_ATTR_QUALITY_TYPE
     assert one.name != CM_ATTR_QUALITY_TYPE
-    assert one.type_name == CM_ENUM_DQ_TYPE
+    assert one.type_name == make_unique(f"{MODULE_NAME}_DataQualityType")
     assert one.options
     assert not one.options.multi_value_select
     assert one.options.primitive_type == AtlanCustomAttributePrimitiveType.OPTIONS.value
 
 
 @pytest.fixture(scope="module")
-def glossary(client: AtlanClient) -> Generator[AtlasGlossary, None, None]:
-    g = create_glossary(client, name=CM_PREFIX)
+def glossary(
+    client: AtlanClient,
+    make_unique: Callable[[str], str],
+) -> Generator[AtlasGlossary, None, None]:
+    glossary_name = make_unique(MODULE_NAME)
+    g = create_glossary(client, name=glossary_name)
     yield g
     delete_asset(client, guid=g.guid, asset_type=AtlasGlossary)
 
 
 @pytest.fixture(scope="module")
 def term(
     client: AtlanClient,
+    make_unique: Callable[[str], str],
     glossary: AtlasGlossary,
     cm_raci: CustomMetadataDef,
     cm_ipr: CustomMetadataDef,
     cm_dq: CustomMetadataDef,
 ) -> Generator[AtlasGlossaryTerm, None, None]:
-    t = create_term(client, name=CM_PREFIX, glossary_guid=glossary.guid)
+    term_name = make_unique(MODULE_NAME)
+    t = create_term(client, name=term_name, glossary_guid=glossary.guid)
     yield t
     delete_asset(client, guid=t.guid, asset_type=AtlasGlossaryTerm)
 
 
 @pytest.fixture(scope="module")
 def groups(
     client: AtlanClient,
+    make_unique: Callable[[str], str],
     glossary: AtlasGlossary,
     term: AtlasGlossaryTerm,
     cm_raci: CustomMetadataDef,
     cm_ipr: CustomMetadataDef,
     cm_dq: CustomMetadataDef,
 ) -> Generator[List[CreateGroupResponse], None, None]:
-    g1 = create_group(client, GROUP_NAME1)
-    g2 = create_group(client, GROUP_NAME2)
+    g1 = create_group(client, make_unique(f"{MODULE_NAME}1"))
+    g2 = create_group(client, make_unique(f"{MODULE_NAME}2"))
     yield [g1, g2]
     delete_group(client, g1.group)
     delete_group(client, g2.group)
 
 
-def _get_groups(client: AtlanClient) -> Tuple[AtlanGroup, AtlanGroup]:
-    candidates = client.get_group_by_name(GROUP_NAME1)
+def _get_groups(
+    client: AtlanClient,
+    make_unique: Callable[[str], str],
+) -> Tuple[AtlanGroup, AtlanGroup]:
+    candidates = client.get_group_by_name(make_unique(f"{MODULE_NAME}1"))
     assert candidates
     assert len(candidates) == 1
     group1 = candidates[0]
-    candidates = client.get_group_by_name(GROUP_NAME2)
+    candidates = client.get_group_by_name(make_unique(f"{MODULE_NAME}2"))
     assert candidates
     assert len(candidates) == 1
     group2 = candidates[0]
     return group1, group2
 
 
 def test_add_term_cm_raci(
     client: AtlanClient,
+    make_unique: Callable[[str], str],
     cm_raci: CustomMetadataDef,
     term: AtlasGlossaryTerm,
     groups: List[AtlanGroup],
 ):
-    raci_attrs = term.get_custom_metadata(CM_RACI)
+    cm_name = make_unique("RACI")
+    raci_attrs = CustomMetadataDict(cm_name)
     _validate_raci_empty(raci_attrs)
-    group1, group2 = _get_groups(client)
-    setattr(raci_attrs, CM_ATTR_RACI_RESPONSIBLE_RENAMED, [FIXED_USER])
-    setattr(raci_attrs, CM_ATTR_RACI_ACCOUNTABLE_RENAMED, FIXED_USER)
-    setattr(raci_attrs, CM_ATTR_RACI_CONSULTED_RENAMED, [group1.name])
-    setattr(raci_attrs, CM_ATTR_RACI_INFORMED_RENAMED, [group1.name, group2.name])
+    group1, group2 = _get_groups(client, make_unique)
+    raci_attrs[CM_ATTR_RACI_RESPONSIBLE] = [FIXED_USER]
+    raci_attrs[CM_ATTR_RACI_ACCOUNTABLE] = FIXED_USER
+    raci_attrs[CM_ATTR_RACI_CONSULTED] = [group1.name]
+    raci_attrs[CM_ATTR_RACI_INFORMED] = [group1.name, group2.name]
     client.update_custom_metadata_attributes(term.guid, raci_attrs)
     t = client.retrieve_minimal(guid=term.guid, asset_type=AtlasGlossaryTerm)
     assert t
-    _validate_raci_attributes(client, t.get_custom_metadata(name=CM_RACI))
+    _validate_raci_attributes(client, make_unique, t.get_custom_metadata(name=cm_name))
 
 
 def test_add_term_cm_ipr(
-    client: AtlanClient, cm_ipr: CustomMetadataDef, term: AtlasGlossaryTerm
+    client: AtlanClient,
+    make_unique: Callable[[str], str],
+    cm_ipr: CustomMetadataDef,
+    term: AtlasGlossaryTerm,
 ):
-    ipr_attrs = term.get_custom_metadata(CM_IPR)
+    cm_name = make_unique("IPR")
+    ipr_attrs = CustomMetadataDict(cm_name)
     _validate_ipr_empty(ipr_attrs)
-    setattr(ipr_attrs, CM_ATTR_IPR_LICENSE_RENAMED, "CC BY")
-    setattr(ipr_attrs, CM_ATTR_IPR_VERSION_RENAMED, 2.0)
-    setattr(ipr_attrs, CM_ATTR_IPR_MANDATORY_RENAMED, True)
-    setattr(ipr_attrs, CM_ATTR_IPR_DATE_RENAMED, 1659308400000)
-    setattr(
-        ipr_attrs,
-        CM_ATTR_IPR_URL_RENAMED,
-        "https://creativecommons.org/licenses/by/2.0/",
-    )
+    ipr_attrs[CM_ATTR_IPR_LICENSE] = "CC BY"
+    ipr_attrs[CM_ATTR_IPR_VERSION] = 2.0
+    ipr_attrs[CM_ATTR_IPR_MANDATORY] = True
+    ipr_attrs[CM_ATTR_IPR_DATE] = 1659308400000
+    ipr_attrs[CM_ATTR_IPR_URL] = "https://creativecommons.org/licenses/by/2.0/"
+
     client.update_custom_metadata_attributes(term.guid, ipr_attrs)
     t = client.retrieve_minimal(guid=term.guid, asset_type=AtlasGlossaryTerm)
     assert t
-    _validate_ipr_attributes(t.get_custom_metadata(name=CM_IPR))
+    _validate_ipr_attributes(t.get_custom_metadata(name=cm_name))
 
 
 def test_add_term_cm_dq(
-    client: AtlanClient, cm_dq: CustomMetadataDef, term: AtlasGlossaryTerm
+    client: AtlanClient,
+    make_unique: Callable[[str], str],
+    cm_dq: CustomMetadataDef,
+    term: AtlasGlossaryTerm,
 ):
-    dq_attrs = term.get_custom_metadata(CM_QUALITY)
+    cm_name = make_unique("DQ")
+    dq_attrs = CustomMetadataDict(cm_name)
     _validate_dq_empty(dq_attrs)
-    setattr(dq_attrs, CM_ATTR_QUALITY_COUNT_RENAMED, 42)
-    setattr(dq_attrs, CM_ATTR_QUALITY_SQL_RENAMED, "SELECT * from SOMEWHERE;")
-    setattr(dq_attrs, CM_ATTR_QUALITY_TYPE_RENAMED, "Completeness")
+    dq_attrs[CM_ATTR_QUALITY_COUNT] = 42
+    dq_attrs[CM_ATTR_QUALITY_SQL] = "SELECT * from SOMEWHERE;"
+    dq_attrs[CM_ATTR_QUALITY_TYPE] = "Completeness"
     client.update_custom_metadata_attributes(term.guid, dq_attrs)
     t = client.retrieve_minimal(guid=term.guid, asset_type=AtlasGlossaryTerm)
     assert t
-    _validate_dq_attributes(t.get_custom_metadata(name=CM_QUALITY))
+    _validate_dq_attributes(t.get_custom_metadata(name=cm_name))
 
 
 @pytest.mark.order(after="test_add_term_cm_dq")
 def test_update_term_cm_ipr(
-    client: AtlanClient, cm_ipr: CustomMetadataDef, term: AtlasGlossaryTerm
+    client: AtlanClient,
+    make_unique: Callable[[str], str],
+    cm_ipr: CustomMetadataDef,
+    term: AtlasGlossaryTerm,
 ):
-    ipr = term.get_custom_metadata(CM_IPR)
+    cm_name = make_unique("IPR")
+    ipr = CustomMetadataDict(cm_name)
     # Note: MUST access the getter / setter, not the underlying store
-    setattr(ipr, CM_ATTR_IPR_MANDATORY_RENAMED, False)
+    ipr[CM_ATTR_IPR_MANDATORY] = False
     client.update_custom_metadata_attributes(term.guid, ipr)
     t = client.retrieve_minimal(guid=term.guid, asset_type=AtlasGlossaryTerm)
     assert t
-    _validate_ipr_attributes(t.get_custom_metadata(name=CM_IPR), mandatory=False)
-    _validate_raci_attributes(client, t.get_custom_metadata(name=CM_RACI))
-    _validate_dq_attributes(t.get_custom_metadata(name=CM_QUALITY))
+    _validate_ipr_attributes(t.get_custom_metadata(name=cm_name), mandatory=False)
+    _validate_raci_attributes(
+        client, make_unique, t.get_custom_metadata(name=make_unique("RACI"))
+    )
+    _validate_dq_attributes(t.get_custom_metadata(name=make_unique("DQ")))
 
 
 @pytest.mark.order(after="test_update_term_cm_ipr")
 def test_replace_term_cm_raci(
-    client: AtlanClient, cm_raci: CustomMetadataDef, term: AtlasGlossaryTerm
+    client: AtlanClient,
+    make_unique: Callable[[str], str],
+    cm_raci: CustomMetadataDef,
+    term: AtlasGlossaryTerm,
 ):
-    raci = term.get_custom_metadata(CM_RACI)
-    group1, group2 = _get_groups(client)
-    # Note: MUST access the getter / setter, not the underlying store
-    setattr(raci, CM_ATTR_RACI_RESPONSIBLE_RENAMED, [FIXED_USER])
-    setattr(raci, CM_ATTR_RACI_ACCOUNTABLE_RENAMED, FIXED_USER)
-    setattr(raci, CM_ATTR_RACI_CONSULTED_RENAMED, None)
-    setattr(raci, CM_ATTR_RACI_INFORMED_RENAMED, [group1.name, group2.name])
+    CM_RACI = make_unique("RACI")
+    CM_IPR = make_unique("IPR")
+    CM_QUALITY = make_unique("DQ")
+    raci = CustomMetadataDict(CM_RACI)
+    group1, group2 = _get_groups(client, make_unique)
+    raci[CM_ATTR_RACI_RESPONSIBLE] = [FIXED_USER]
+    raci[CM_ATTR_RACI_ACCOUNTABLE] = FIXED_USER
+    raci[CM_ATTR_RACI_CONSULTED] = None
+    raci[CM_ATTR_RACI_INFORMED] = [group1.name, group2.name]
     client.replace_custom_metadata(term.guid, raci)
     t = client.retrieve_minimal(guid=term.guid, asset_type=AtlasGlossaryTerm)
     assert t
-    _validate_raci_attributes_replacement(client, t.get_custom_metadata(name=CM_RACI))
+    _validate_raci_attributes_replacement(
+        client, make_unique, t.get_custom_metadata(name=CM_RACI)
+    )
     _validate_ipr_attributes(t.get_custom_metadata(name=CM_IPR), mandatory=False)
     _validate_dq_attributes(t.get_custom_metadata(name=CM_QUALITY))
 
 
 @pytest.mark.order(after="test_replace_term_cm_raci")
 def test_replace_term_cm_ipr(
-    client: AtlanClient, cm_ipr: CustomMetadataDef, term: AtlasGlossaryTerm
+    client: AtlanClient,
+    make_unique: Callable[[str], str],
+    cm_ipr: CustomMetadataDef,
+    term: AtlasGlossaryTerm,
 ):
-    client.replace_custom_metadata(term.guid, term.get_custom_metadata(CM_IPR))
+    CM_RACI = make_unique("RACI")
+    CM_IPR = make_unique("IPR")
+    CM_QUALITY = make_unique("DQ")
+    term_cm_ipr = CustomMetadataDict(CM_IPR)
+    client.replace_custom_metadata(term.guid, term_cm_ipr)
     t = client.retrieve_minimal(guid=term.guid, asset_type=AtlasGlossaryTerm)
     assert t
-    _validate_raci_attributes_replacement(client, t.get_custom_metadata(name=CM_RACI))
+    _validate_raci_attributes_replacement(
+        client, make_unique, t.get_custom_metadata(name=CM_RACI)
+    )
     _validate_dq_attributes(t.get_custom_metadata(name=CM_QUALITY))
     _validate_ipr_empty(t.get_custom_metadata(name=CM_IPR))
 
 
 @pytest.mark.order(after="test_replace_term_cm_ipr")
 def test_search_by_any_accountable(
     client: AtlanClient,
+    make_unique: Callable[[str], str],
     cm_raci: CustomMetadataDef,
     glossary: AtlasGlossary,
     term: AtlasGlossaryTerm,
 ):
     be_active = Term.with_state("ACTIVE")
     be_a_term = Term.with_type_name("AtlasGlossaryTerm")
     have_attr = Exists.with_custom_metadata(
-        set_name=CM_RACI, attr_name=CM_ATTR_RACI_ACCOUNTABLE_RENAMED
+        set_name=make_unique("RACI"), attr_name=CM_ATTR_RACI_ACCOUNTABLE
     )
     query = Bool(must=[be_active, be_a_term, have_attr])
     dsl = DSL(query=query)
     request = IndexSearchRequest(
         dsl=dsl, attributes=["name", "anchor"], relation_attributes=["name"]
     )
     response = client.search(criteria=request)
@@ -521,22 +559,25 @@
         assert anchor
         assert anchor.name == glossary.name
 
 
 @pytest.mark.order(after="test_replace_term_cm_ipr")
 def test_search_by_specific_accountable(
     client: AtlanClient,
+    make_unique: Callable[[str], str],
     cm_raci: CustomMetadataDef,
     glossary: AtlasGlossary,
     term: AtlasGlossaryTerm,
 ):
     be_active = Term.with_state("ACTIVE")
     be_a_term = Term.with_type_name("AtlasGlossaryTerm")
     have_attr = Term.with_custom_metadata(
-        set_name=CM_RACI, attr_name=CM_ATTR_RACI_ACCOUNTABLE_RENAMED, value=FIXED_USER
+        set_name=make_unique("RACI"),
+        attr_name=CM_ATTR_RACI_ACCOUNTABLE,
+        value=FIXED_USER,
     )
     query = Bool(must=[be_active, be_a_term, have_attr])
     dsl = DSL(query=query)
     request = IndexSearchRequest(
         dsl=dsl, attributes=["name", "anchor"], relation_attributes=["name"]
     )
     response = client.search(criteria=request)
@@ -557,40 +598,55 @@
         assert anchor.name == glossary.name
 
 
 @pytest.mark.order(
     after=["test_search_by_any_accountable", "test_search_by_specific_accountable"]
 )
 def test_remove_term_cm_raci(
-    client: AtlanClient, cm_raci: CustomMetadataDef, term: AtlasGlossaryTerm
+    client: AtlanClient,
+    make_unique: Callable[[str], str],
+    cm_raci: CustomMetadataDef,
+    term: AtlasGlossaryTerm,
 ):
+    CM_RACI = make_unique("RACI")
+    CM_IPR = make_unique("IPR")
+    CM_QUALITY = make_unique("DQ")
     client.remove_custom_metadata(term.guid, cm_name=CM_RACI)
     t = client.retrieve_minimal(guid=term.guid, asset_type=AtlasGlossaryTerm)
     assert t
     _validate_dq_attributes(t.get_custom_metadata(name=CM_QUALITY))
     _validate_ipr_empty(t.get_custom_metadata(name=CM_IPR))
     _validate_raci_empty(t.get_custom_metadata(name=CM_RACI))
 
 
 @pytest.mark.order(after="test_remove_term_cm_raci")
 def test_remove_term_cm_ipr(
-    client: AtlanClient, cm_ipr: CustomMetadataDef, term: AtlasGlossaryTerm
+    client: AtlanClient,
+    make_unique: Callable[[str], str],
+    cm_ipr: CustomMetadataDef,
+    term: AtlasGlossaryTerm,
 ):
+    CM_RACI = make_unique("RACI")
+    CM_IPR = make_unique("IPR")
+    CM_QUALITY = make_unique("DQ")
     client.remove_custom_metadata(term.guid, cm_name=CM_IPR)
     t = client.retrieve_minimal(guid=term.guid, asset_type=AtlasGlossaryTerm)
     assert t
     _validate_dq_attributes(t.get_custom_metadata(name=CM_QUALITY))
     _validate_ipr_empty(t.get_custom_metadata(name=CM_IPR))
     _validate_raci_empty(t.get_custom_metadata(name=CM_RACI))
 
 
 @pytest.mark.order(after="test_remove_term_cm_raci")
-def test_remove_attribute(client: AtlanClient, cm_raci: CustomMetadataDef):
+def test_remove_attribute(
+    client: AtlanClient, make_unique: Callable[[str], str], cm_raci: CustomMetadataDef
+):
     global _removal_epoch
-    existing = CustomMetadataCache.get_custom_metadata_def(name=CM_RACI)
+    cm_name = make_unique("RACI")
+    existing = CustomMetadataCache.get_custom_metadata_def(name=cm_name)
     existing_attrs = existing.attribute_defs
     updated_attrs = []
     for existing_attr in existing_attrs:
         to_keep = existing_attr
         if existing_attr.display_name == CM_ATTR_RACI_EXTRA:
             to_keep = existing_attr.archive(by="test-automation")
             assert to_keep.options
@@ -598,33 +654,38 @@
         updated_attrs.append(to_keep)
     existing.attribute_defs = updated_attrs
     response = client.update_typedef(existing)
     assert response
     assert len(response.custom_metadata_defs) == 1
     updated = response.custom_metadata_defs[0]
     assert updated.category == AtlanTypeCategory.CUSTOM_METADATA
-    assert updated.name != CM_RACI
+    assert updated.name != cm_name
     assert updated.guid
-    assert updated.display_name == CM_RACI
+    assert updated.display_name == cm_name
     attributes = updated.attribute_defs
     archived = _validate_raci_structure(attributes, 5)
     assert archived
     assert (
         archived.display_name == f"{CM_ATTR_RACI_EXTRA}-archived-{str(_removal_epoch)}"
     )
     assert archived.name != CM_ATTR_RACI_EXTRA
     assert archived.type_name == AtlanCustomAttributePrimitiveType.STRING.value
     assert not archived.options.multi_value_select
     assert archived.is_archived()
 
 
 @pytest.mark.order(after="test_remove_attribute")
-def test_retrieve_structures(client: AtlanClient, cm_raci: CustomMetadataDef):
+def test_retrieve_structures(
+    client: AtlanClient, make_unique: Callable[[str], str], cm_raci: CustomMetadataDef
+):
     global _removal_epoch
     custom_attributes = CustomMetadataCache.get_all_custom_attributes()
+    CM_RACI = make_unique("RACI")
+    CM_IPR = make_unique("IPR")
+    CM_QUALITY = make_unique("DQ")
     assert custom_attributes
     assert len(custom_attributes) >= 3
     assert CM_RACI in custom_attributes.keys()
     assert CM_IPR in custom_attributes.keys()
     assert CM_QUALITY in custom_attributes.keys()
     extra = _validate_raci_structure(custom_attributes.get(CM_RACI), 4)
     assert not extra
@@ -642,15 +703,18 @@
     assert extra.type_name == AtlanCustomAttributePrimitiveType.STRING.value
     assert "Database" in extra.options.custom_applicable_entity_types
     assert not extra.options.multi_value_select
     assert extra.is_archived()
 
 
 @pytest.mark.order(after="test_retrieve_structures")
-def test_recreate_attribute(client: AtlanClient, cm_raci: CustomMetadataDef):
+def test_recreate_attribute(
+    client: AtlanClient, make_unique: Callable[[str], str], cm_raci: CustomMetadataDef
+):
+    CM_RACI = make_unique("RACI")
     existing = CustomMetadataCache.get_custom_metadata_def(name=CM_RACI)
     existing_attrs = existing.attribute_defs
     updated_attrs = []
     for existing_attr in existing_attrs:
         existing_attr.is_new = None
         updated_attrs.append(existing_attr)
     new_attr = AttributeDef.create(
@@ -675,16 +739,19 @@
     assert extra.type_name == AtlanCustomAttributePrimitiveType.STRING.value
     assert not extra.options.multi_value_select
     assert not extra.is_archived()
 
 
 @pytest.mark.order(after="test_recreate_attribute")
 def test_retrieve_structure_without_archived(
-    client: AtlanClient, cm_raci: CustomMetadataDef
+    client: AtlanClient, make_unique: Callable[[str], str], cm_raci: CustomMetadataDef
 ):
+    CM_RACI = make_unique("RACI")
+    CM_IPR = make_unique("IPR")
+    CM_QUALITY = make_unique("DQ")
     custom_attributes = CustomMetadataCache.get_all_custom_attributes()
     assert custom_attributes
     assert len(custom_attributes) >= 3
     assert CM_RACI in custom_attributes.keys()
     assert CM_IPR in custom_attributes.keys()
     assert CM_QUALITY in custom_attributes.keys()
     extra = _validate_raci_structure(custom_attributes.get(CM_RACI), 5)
@@ -694,16 +761,19 @@
     assert extra.type_name == AtlanCustomAttributePrimitiveType.STRING.value
     assert "Database" in extra.options.custom_applicable_entity_types
     assert not extra.is_archived()
 
 
 @pytest.mark.order(after="test_recreate_attribute")
 def test_retrieve_structure_with_archived(
-    client: AtlanClient, cm_raci: CustomMetadataDef
+    client: AtlanClient, make_unique: Callable[[str], str], cm_raci: CustomMetadataDef
 ):
+    CM_RACI = make_unique("RACI")
+    CM_IPR = make_unique("IPR")
+    CM_QUALITY = make_unique("DQ")
     custom_attributes = CustomMetadataCache.get_all_custom_attributes(
         include_deleted=True
     )
     assert custom_attributes
     assert len(custom_attributes) >= 3
     assert CM_RACI in custom_attributes.keys()
     assert CM_IPR in custom_attributes.keys()
@@ -721,22 +791,26 @@
 def test_update_replacing_cm(
     term: AtlasGlossaryTerm,
     glossary: AtlasGlossary,
     cm_raci: CustomMetadataDef,
     cm_ipr: CustomMetadataDef,
     cm_dq: CustomMetadataDef,
     client: AtlanClient,
+    make_unique: Callable[[str], str],
 ):
-    raci = term.get_custom_metadata(CM_RACI)
-    group1, group2 = _get_groups(client)
-    setattr(raci, CM_ATTR_RACI_RESPONSIBLE_RENAMED, [FIXED_USER])
-    setattr(raci, CM_ATTR_RACI_ACCOUNTABLE_RENAMED, FIXED_USER)
-    setattr(raci, CM_ATTR_RACI_CONSULTED_RENAMED, [group1.name])
-    setattr(raci, CM_ATTR_RACI_INFORMED_RENAMED, [group1.name, group2.name])
-    setattr(raci, CM_ATTR_RACI_EXTRA_RENAMED, "something extra...")
+    CM_RACI = make_unique("RACI")
+    CM_IPR = make_unique("IPR")
+    CM_QUALITY = make_unique("DQ")
+    raci = CustomMetadataDict(CM_RACI)
+    group1, group2 = _get_groups(client, make_unique)
+    raci[CM_ATTR_RACI_RESPONSIBLE] = [FIXED_USER]
+    raci[CM_ATTR_RACI_ACCOUNTABLE] = FIXED_USER
+    raci[CM_ATTR_RACI_CONSULTED] = [group1.name]
+    raci[CM_ATTR_RACI_INFORMED] = [group1.name, group2.name]
+    raci[CM_ATTR_RACI_EXTRA] = "something extra..."
     to_update = AtlasGlossaryTerm.create_for_modification(
         qualified_name=term.qualified_name, name=term.name, glossary_guid=glossary.guid
     )
     to_update.set_custom_metadata(custom_metadata=raci)
     response = client.upsert_replacing_cm(to_update, replace_classifications=False)
     assert response
     assert len(response.assets_deleted(asset_type=AtlasGlossaryTerm)) == 0
@@ -749,134 +823,130 @@
     x = client.get_asset_by_qualified_name(
         qualified_name=term.qualified_name, asset_type=AtlasGlossaryTerm
     )
     assert x
     assert not x.is_incomplete
     assert x.qualified_name == term.qualified_name
     raci = x.get_custom_metadata(CM_RACI)
-    _validate_raci_attributes(client, raci)
-    assert getattr(raci, CM_ATTR_RACI_EXTRA_RENAMED) == "something extra..."
+    _validate_raci_attributes(client, make_unique, raci)
+    assert raci[CM_ATTR_RACI_EXTRA] == "something extra..."
     _validate_ipr_empty(x.get_custom_metadata(CM_IPR))
     _validate_dq_empty(x.get_custom_metadata(CM_QUALITY))
 
 
 # TODO: test entity audit retrieval and parsing, once available
 
 
-def test_get_custom_metadata_when_name_is_invalid_then_raises_not_found_error():
-    with pytest.raises(
-        NotFoundError, match="Custom metadata with name Bogs does not exist"
-    ):
-        CustomMetadataCache.get_custom_metadata(name="Bogs", asset_type=Table)
-
-
-def _validate_raci_attributes(client: AtlanClient, cma: CustomMetadata):
+def _validate_raci_attributes(
+    client: AtlanClient, make_unique: Callable[[str], str], cma: CustomMetadataDict
+):
     assert cma
     # Note: MUST access the getter / setter, not the underlying store
-    responsible = getattr(cma, CM_ATTR_RACI_RESPONSIBLE_RENAMED)
-    accountable = getattr(cma, CM_ATTR_RACI_ACCOUNTABLE_RENAMED)
-    consulted = getattr(cma, CM_ATTR_RACI_CONSULTED_RENAMED)
-    informed = getattr(cma, CM_ATTR_RACI_INFORMED_RENAMED)
-    group1, group2 = _get_groups(client)
+    responsible = cma[CM_ATTR_RACI_RESPONSIBLE]
+    accountable = cma[CM_ATTR_RACI_ACCOUNTABLE]
+    consulted = cma[CM_ATTR_RACI_CONSULTED]
+    informed = cma[CM_ATTR_RACI_INFORMED]
+    group1, group2 = _get_groups(client, make_unique)
     assert responsible
     assert len(responsible) == 1
     assert FIXED_USER in responsible
     assert accountable
     assert accountable == FIXED_USER
     assert consulted == [group1.name]
     assert informed == [group1.name, group2.name]
 
 
-def _validate_raci_attributes_replacement(client: AtlanClient, cma: CustomMetadata):
+def _validate_raci_attributes_replacement(
+    client: AtlanClient, make_unique: Callable[[str], str], cma: CustomMetadataDict
+):
     assert cma
     # Note: MUST access the getter / setter, not the underlying store
-    responsible = getattr(cma, CM_ATTR_RACI_RESPONSIBLE_RENAMED)
-    accountable = getattr(cma, CM_ATTR_RACI_ACCOUNTABLE_RENAMED)
-    consulted = getattr(cma, CM_ATTR_RACI_CONSULTED_RENAMED)
-    informed = getattr(cma, CM_ATTR_RACI_INFORMED_RENAMED)
-    group1, group2 = _get_groups(client)
+    responsible = cma[CM_ATTR_RACI_RESPONSIBLE]
+    accountable = cma[CM_ATTR_RACI_ACCOUNTABLE]
+    consulted = cma[CM_ATTR_RACI_CONSULTED]
+    informed = cma[CM_ATTR_RACI_INFORMED]
+    group1, group2 = _get_groups(client, make_unique)
     assert responsible
     assert responsible == [FIXED_USER]
     assert accountable
     assert accountable == FIXED_USER
     assert not consulted
     assert informed == [group1.name, group2.name]
 
 
-def _validate_raci_empty(raci_attrs: CustomMetadata):
-    assert hasattr(raci_attrs, CM_ATTR_RACI_RESPONSIBLE_RENAMED)
-    assert hasattr(raci_attrs, CM_ATTR_RACI_ACCOUNTABLE_RENAMED)
-    assert hasattr(raci_attrs, CM_ATTR_RACI_CONSULTED_RENAMED)
-    assert hasattr(raci_attrs, CM_ATTR_RACI_INFORMED_RENAMED)
-    assert hasattr(raci_attrs, CM_ATTR_RACI_EXTRA_RENAMED)
-    assert not getattr(
-        raci_attrs, CM_ATTR_RACI_RESPONSIBLE_RENAMED
-    )  # could be empty list
-    assert getattr(raci_attrs, CM_ATTR_RACI_ACCOUNTABLE_RENAMED) is None
-    assert not getattr(
-        raci_attrs, CM_ATTR_RACI_CONSULTED_RENAMED
-    )  # could be empty list
-    assert not getattr(raci_attrs, CM_ATTR_RACI_INFORMED_RENAMED)  # could be empty list
-    assert getattr(raci_attrs, CM_ATTR_RACI_EXTRA_RENAMED) is None
+def _validate_raci_empty(raci_attrs: CustomMetadataDict):
+    attribute_names = raci_attrs.attribute_names
+    assert CM_ATTR_RACI_RESPONSIBLE in attribute_names
+    assert CM_ATTR_RACI_ACCOUNTABLE in attribute_names
+    assert CM_ATTR_RACI_CONSULTED in attribute_names
+    assert CM_ATTR_RACI_INFORMED in attribute_names
+    assert CM_ATTR_RACI_EXTRA in attribute_names
+    assert not raci_attrs[CM_ATTR_RACI_RESPONSIBLE]
+    assert raci_attrs[CM_ATTR_RACI_ACCOUNTABLE] is None
+    assert not raci_attrs[CM_ATTR_RACI_CONSULTED]  # could be empty list
+    assert not raci_attrs[CM_ATTR_RACI_INFORMED]  # could be empty list
+    assert raci_attrs[CM_ATTR_RACI_EXTRA] is None
 
 
-def _validate_ipr_attributes(cma: CustomMetadata, mandatory: bool = True):
+def _validate_ipr_attributes(cma: CustomMetadataDict, mandatory: bool = True):
     assert cma
-    license = getattr(cma, CM_ATTR_IPR_LICENSE_RENAMED)
-    v = getattr(cma, CM_ATTR_IPR_VERSION_RENAMED)
-    m = getattr(cma, CM_ATTR_IPR_MANDATORY_RENAMED)
-    d = getattr(cma, CM_ATTR_IPR_DATE_RENAMED)
-    u = getattr(cma, CM_ATTR_IPR_URL_RENAMED)
+    license = cma[CM_ATTR_IPR_LICENSE]
+    v = cma[CM_ATTR_IPR_VERSION]
+    m = cma[CM_ATTR_IPR_MANDATORY]
+    d = cma[CM_ATTR_IPR_DATE]
+    u = cma[CM_ATTR_IPR_URL]
     assert license
     assert license == "CC BY"
     assert v
     assert v == 2.0
     if mandatory:
         assert m
     else:
         assert not m
     assert d
     assert d == 1659308400000
     assert u
     assert u == "https://creativecommons.org/licenses/by/2.0/"
 
 
-def _validate_ipr_empty(ipr_attrs: CustomMetadata):
-    assert hasattr(ipr_attrs, CM_ATTR_IPR_LICENSE_RENAMED)
-    assert hasattr(ipr_attrs, CM_ATTR_IPR_VERSION_RENAMED)
-    assert hasattr(ipr_attrs, CM_ATTR_IPR_MANDATORY_RENAMED)
-    assert hasattr(ipr_attrs, CM_ATTR_IPR_DATE_RENAMED)
-    assert hasattr(ipr_attrs, CM_ATTR_IPR_URL_RENAMED)
-    assert getattr(ipr_attrs, CM_ATTR_IPR_LICENSE_RENAMED) is None
-    assert getattr(ipr_attrs, CM_ATTR_IPR_VERSION_RENAMED) is None
-    assert getattr(ipr_attrs, CM_ATTR_IPR_MANDATORY_RENAMED) is None
-    assert getattr(ipr_attrs, CM_ATTR_IPR_DATE_RENAMED) is None
-    assert getattr(ipr_attrs, CM_ATTR_IPR_URL_RENAMED) is None
+def _validate_ipr_empty(ipr_attrs: CustomMetadataDict):
+    attribute_names = ipr_attrs.attribute_names
+    assert CM_ATTR_IPR_LICENSE in attribute_names
+    assert CM_ATTR_IPR_VERSION in attribute_names
+    assert CM_ATTR_IPR_MANDATORY in attribute_names
+    assert CM_ATTR_IPR_DATE in attribute_names
+    assert CM_ATTR_IPR_URL in attribute_names
+    assert ipr_attrs[CM_ATTR_IPR_LICENSE] is None
+    assert ipr_attrs[CM_ATTR_IPR_VERSION] is None
+    assert ipr_attrs[CM_ATTR_IPR_MANDATORY] is None
+    assert ipr_attrs[CM_ATTR_IPR_DATE] is None
+    assert ipr_attrs[CM_ATTR_IPR_URL] is None
 
 
-def _validate_dq_attributes(cma: CustomMetadata):
+def _validate_dq_attributes(cma: CustomMetadataDict):
     assert cma
-    c = getattr(cma, CM_ATTR_QUALITY_COUNT_RENAMED)
-    s = getattr(cma, CM_ATTR_QUALITY_SQL_RENAMED)
-    t = getattr(cma, CM_ATTR_QUALITY_TYPE_RENAMED)
+    c = cma[CM_ATTR_QUALITY_COUNT]
+    s = cma[CM_ATTR_QUALITY_SQL]
+    t = cma[CM_ATTR_QUALITY_TYPE]
     assert c
     assert c == 42
     assert s
     assert s == "SELECT * from SOMEWHERE;"
     assert t
     assert t == "Completeness"
 
 
-def _validate_dq_empty(dq_attrs: CustomMetadata):
-    assert hasattr(dq_attrs, CM_ATTR_QUALITY_COUNT_RENAMED)
-    assert hasattr(dq_attrs, CM_ATTR_QUALITY_SQL_RENAMED)
-    assert hasattr(dq_attrs, CM_ATTR_QUALITY_TYPE_RENAMED)
-    assert getattr(dq_attrs, CM_ATTR_QUALITY_COUNT_RENAMED) is None
-    assert getattr(dq_attrs, CM_ATTR_QUALITY_SQL_RENAMED) is None
-    assert getattr(dq_attrs, CM_ATTR_QUALITY_TYPE_RENAMED) is None
+def _validate_dq_empty(dq_attrs: CustomMetadataDict):
+    attribute_names = dq_attrs.attribute_names
+    assert CM_ATTR_QUALITY_COUNT in attribute_names
+    assert CM_ATTR_QUALITY_SQL in attribute_names
+    assert CM_ATTR_QUALITY_TYPE in attribute_names
+    assert dq_attrs[CM_ATTR_QUALITY_COUNT] is None
+    assert dq_attrs[CM_ATTR_QUALITY_SQL] is None
+    assert dq_attrs[CM_ATTR_QUALITY_TYPE] is None
 
 
 def _validate_raci_structure(
     attributes: Optional[List[AttributeDef]], total_expected: int
 ):
     global _removal_epoch
     assert attributes
@@ -932,20 +1002,22 @@
     if total_expected > 4:
         return attributes[total_expected - 1]
     return None
 
 
 def test_add_badge_cm_dq(
     client: AtlanClient,
+    make_unique: Callable[[str], str],
     cm_dq: CustomMetadataDef,
 ):
+    CM_QUALITY = make_unique("DQ")
     badge = Badge.create(
         name=CM_ATTR_QUALITY_COUNT,
         cm_name=CM_QUALITY,
-        cm_attribute=CM_ATTR_QUALITY_COUNT_RENAMED,
+        cm_attribute=CM_ATTR_QUALITY_COUNT,
         badge_conditions=[
             BadgeCondition.create(
                 badge_condition_operator=BadgeComparisonOperator.GTE,
                 badge_condition_value="5",
                 badge_condition_colorhex=BadgeConditionColor.GREEN,
             ),
             BadgeCondition.create(
```

### Comparing `pyatlan-0.0.33/tests/integration/glossary_test.py` & `pyatlan-0.1.0/tests/integration/glossary_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
-import logging
-from typing import Generator
+from typing import Callable, Generator
 
 import pytest
 from pydantic import StrictStr
 
 from pyatlan.client.atlan import AtlanClient
 from pyatlan.model.assets import AtlasGlossary, AtlasGlossaryTerm
 from tests.integration.client import delete_asset
 
-LOGGER = logging.getLogger(__name__)
-
-PREFIX = "psdk-Glossary"
-
-GLOSSARY_NAME = f"{PREFIX} Traversable"
-TERM_NAME1 = f"{PREFIX} Term1"
-TERM_NAME2 = f"{PREFIX} Term2"
+MODULE_NAME = "GLS"
 
 
 def create_glossary(client: AtlanClient, name: str) -> AtlasGlossary:
     g = AtlasGlossary.create(name=StrictStr(name))
     r = client.upsert(g)
     return r.assets_created(AtlasGlossary)[0]
 
@@ -32,62 +25,81 @@
         name=StrictStr(name), glossary_guid=StrictStr(glossary_guid)
     )
     r = client.upsert(t)
     return r.assets_created(AtlasGlossaryTerm)[0]
 
 
 @pytest.fixture(scope="module")
-def glossary(client: AtlanClient) -> Generator[AtlasGlossary, None, None]:
-    g = create_glossary(client, GLOSSARY_NAME)
+def glossary(
+    client: AtlanClient,
+    make_unique: Callable[[str], str],
+) -> Generator[AtlasGlossary, None, None]:
+    glossary_name = make_unique(f"{MODULE_NAME}")
+    g = create_glossary(client, glossary_name)
     yield g
     delete_asset(client, guid=g.guid, asset_type=AtlasGlossary)
 
 
-def test_glossary(glossary: AtlasGlossary):
+def test_glossary(
+    glossary: AtlasGlossary,
+    make_unique: Callable[[str], str],
+):
     assert glossary.guid
-    assert glossary.name == GLOSSARY_NAME
+    assert glossary.name == make_unique(f"{MODULE_NAME}")
     assert glossary.qualified_name
-    assert glossary.qualified_name != GLOSSARY_NAME
+    assert glossary.qualified_name != make_unique(f"{MODULE_NAME}")
 
 
 @pytest.fixture(scope="module")
 def term1(
-    client: AtlanClient, glossary: AtlasGlossary
+    client: AtlanClient, make_unique: Callable[[str], str], glossary: AtlasGlossary
 ) -> Generator[AtlasGlossaryTerm, None, None]:
-    t = create_term(client, name=TERM_NAME1, glossary_guid=glossary.guid)
+    term_name1 = make_unique(f"{MODULE_NAME}1")
+    t = create_term(client, name=term_name1, glossary_guid=glossary.guid)
     yield t
     delete_asset(client, guid=t.guid, asset_type=AtlasGlossaryTerm)
 
 
-def test_term1(client: AtlanClient, term1: AtlasGlossaryTerm, glossary: AtlasGlossary):
+def test_term1(
+    client: AtlanClient,
+    make_unique: Callable[[str], str],
+    term1: AtlasGlossaryTerm,
+    glossary: AtlasGlossary,
+):
     assert term1.guid
-    assert term1.name == TERM_NAME1
+    assert term1.name == make_unique(f"{MODULE_NAME}1")
     assert term1.qualified_name
-    assert term1.qualified_name != TERM_NAME1
+    assert term1.qualified_name != make_unique(f"{MODULE_NAME}1")
     t = client.get_asset_by_guid(term1.guid, asset_type=AtlasGlossaryTerm)
     assert t
     assert t.guid == term1.guid
     assert t.attributes.anchor
     assert t.attributes.anchor.guid == glossary.guid
 
 
 @pytest.fixture(scope="module")
 def term2(
-    client: AtlanClient, glossary: AtlasGlossary
+    client: AtlanClient, make_unique: Callable[[str], str], glossary: AtlasGlossary
 ) -> Generator[AtlasGlossaryTerm, None, None]:
-    t = create_term(client, name=TERM_NAME2, glossary_guid=glossary.guid)
+    term_name2 = make_unique(f"{MODULE_NAME}2")
+    t = create_term(client, name=term_name2, glossary_guid=glossary.guid)
     yield t
     delete_asset(client, guid=t.guid, asset_type=AtlasGlossaryTerm)
 
 
-def test_term2(client: AtlanClient, term2: AtlasGlossaryTerm, glossary: AtlasGlossary):
+def test_term2(
+    client: AtlanClient,
+    make_unique: Callable[[str], str],
+    term2: AtlasGlossaryTerm,
+    glossary: AtlasGlossary,
+):
     assert term2.guid
-    assert term2.name == TERM_NAME2
+    assert term2.name == make_unique(f"{MODULE_NAME}2")
     assert term2.qualified_name
-    assert term2.qualified_name != TERM_NAME2
+    assert term2.qualified_name != make_unique(f"{MODULE_NAME}2")
     t = client.get_asset_by_guid(term2.guid, asset_type=AtlasGlossaryTerm)
     assert t
     assert t.guid == term2.guid
     assert t.attributes.anchor
     assert t.attributes.anchor.guid == glossary.guid
```

### Comparing `pyatlan-0.0.33/tests/integration/test_client.py` & `pyatlan-0.1.0/tests/integration/test_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.33/tests/integration/test_entity_model.py` & `pyatlan-0.1.0/tests/integration/test_entity_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.33/tests/integration/test_index_search.py` & `pyatlan-0.1.0/tests/integration/test_index_search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.33/tests/unit/test_classification_name.py` & `pyatlan-0.1.0/tests/unit/test_classification_name.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.33/tests/unit/test_client.py` & `pyatlan-0.1.0/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.33/tests/unit/test_glossary_term.py` & `pyatlan-0.1.0/tests/unit/test_glossary_term.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.33/tests/unit/test_lineage.py` & `pyatlan-0.1.0/tests/unit/test_lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.33/tests/unit/test_model.py` & `pyatlan-0.1.0/tests/unit/test_model.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
 import json
 from datetime import datetime
 from hashlib import md5
 from inspect import signature
 from pathlib import Path
-from unittest.mock import create_autospec, patch
+from unittest.mock import create_autospec
 
 import pytest
-from deepdiff import DeepDiff
+
+# from deepdiff import DeepDiff
 from pydantic.error_wrappers import ValidationError
 
 import pyatlan.cache.classification_cache
-from pyatlan.cache.custom_metadata_cache import CustomMetadataCache
-from pyatlan.error import NotFoundError
 from pyatlan.model.assets import (
     SQL,
+    AccessControl,
     ADLSAccount,
     ADLSAccountStatus,
     ADLSContainer,
     ADLSEncryptionTypes,
     ADLSObject,
     ADLSReplicationType,
     APIPath,
     APISpec,
     Asset,
     AtlasGlossary,
     AtlasGlossaryCategory,
     AtlasGlossaryTerm,
     AtlasServer,
+    AuthPolicy,
+    AuthPolicyCondition,
+    AuthPolicyValiditySchedule,
     AwsTag,
     AzureTag,
     Badge,
     BadgeCondition,
     Catalog,
     Column,
     ColumnProcess,
@@ -142,26 +145,27 @@
     TableauWorksheet,
     TablePartition,
     ThoughtspotDashlet,
     ThoughtspotLiveboard,
     View,
     validate_single_required_field,
 )
-from pyatlan.model.core import Announcement, AssetResponse
+from pyatlan.model.core import Announcement
 from pyatlan.model.enums import (
     ADLSAccessTier,
     ADLSLeaseState,
     ADLSLeaseStatus,
     ADLSObjectArchiveStatus,
     ADLSObjectType,
     ADLSPerformance,
     ADLSProvisionState,
     ADLSStorageKind,
     AnnouncementType,
     AtlanConnectorType,
+    AuthPolicyType,
     BadgeComparisonOperator,
     BadgeConditionColor,
     CertificateStatus,
     FileType,
     GoogleDatastudioAssetType,
     IconType,
     KafkaTopicCompressionType,
@@ -169,15 +173,14 @@
     QueryUsernameStrategy,
     QuickSightAnalysisStatus,
     QuickSightDatasetFieldType,
     QuickSightDatasetImportMode,
     QuickSightFolderType,
     SourceCostUnitType,
 )
-from pyatlan.model.response import AssetMutationResponse
 from pyatlan.model.structs import (
     KafkaTopicConsumption,
     MCRuleComparison,
     MCRuleSchedule,
     SourceTagAttribute,
 )
 from pyatlan.model.typedef import TypeDefResponse
@@ -408,14 +411,19 @@
     "Optional[Database]": Database(),
     "Optional[list[MaterialisedView]]": [MaterialisedView()],
     "Optional[list[Procedure]]": [Procedure()],
     "Optional[list[SnowflakePipe]]": [SnowflakePipe()],
     "Optional[list[SnowflakeStream]]": [SnowflakeStream()],
     "Optional[list[SnowflakeTag]]": [SnowflakeTag()],
     "Optional[list[Schema]]": [Schema()],
+    "Optional[list[AuthPolicy]]": [AuthPolicy()],
+    "Optional[AccessControl]": AccessControl(),
+    "Optional[list[AuthPolicyCondition]]": [AuthPolicyCondition()],
+    "Optional[AuthPolicyType]": AuthPolicyType.ALLOW,
+    "Optional[list[AuthPolicyValiditySchedule]]": [AuthPolicyValiditySchedule()],
 }
 
 
 def load_json(filename):
     with (DATA_DIR / filename).open() as input_file:
         return json.load(input_file)
 
@@ -656,172 +664,82 @@
 
 
 def test_wrong_json(glossary_json):
     with pytest.raises(ValidationError):
         AtlasGlossaryTerm(**glossary_json)
 
 
-def test_asset_response(glossary_category_json):
-    asset_response_json = {"referredEntities": {}, "entity": glossary_category_json}
-    glossary_category = AssetResponse[AtlasGlossaryCategory](
-        **asset_response_json
-    ).entity
-    assert glossary_category == AtlasGlossaryCategory(**glossary_category_json)
-
-
 @pytest.fixture(scope="function")
 def the_json(request):
     return load_json(request.param)
 
 
-@pytest.mark.parametrize(
-    "the_json, a_type",
-    [
-        ("glossary.json", AtlasGlossary),
-        ("glossary_category.json", AtlasGlossaryCategory),
-        ("glossary_term.json", AtlasGlossaryTerm),
-        ("glossary_term2.json", AtlasGlossaryTerm),
-        ("asset_mutated_response_empty.json", AssetMutationResponse),
-        ("asset_mutated_response_update.json", AssetMutationResponse),
-    ],
-    indirect=["the_json"],
-)
-def test_constructor(the_json, a_type, monkeypatch):
-    def get_name_for_id(value):
-        return "PII"
-
-    def get_id_for_name(value):
-        return "WQ6XGXwq9o7UnZlkWyKhQN"
-
-    monkeypatch.setattr(
-        pyatlan.cache.classification_cache.ClassificationCache,
-        "get_id_for_name",
-        get_id_for_name,
-    )
-
-    monkeypatch.setattr(
-        pyatlan.cache.classification_cache.ClassificationCache,
-        "get_name_for_id",
-        get_name_for_id,
-    )
-
-    asset = a_type(**the_json)
-    assert not DeepDiff(
-        the_json,
-        json.loads(asset.json(by_alias=True, exclude_unset=True)),
-        ignore_order=True,
-    )
-
-
-def test_has_announcement(glossary):
-    assert glossary.has_announcement() == (
-        bool(glossary.attributes.announcement_type)
-        or bool(glossary.attributes.announcement_title)
-    )
-
-
-def test_set_announcement(glossary, announcement):
-    glossary.set_announcement(announcement)
-    assert glossary.has_announcement() is True
-    assert announcement == glossary.get_announcment()
-
-
 def test_create_glossary():
     glossary = AtlasGlossary(
         attributes=AtlasGlossary.Attributes(
             name="Integration Test Glossary", user_description="This a test glossary"
         )
     )
     assert "AtlasGlossary" == glossary.type_name
 
 
-def test_clear_announcement(glossary, announcement):
-    glossary.set_announcement(announcement)
-    glossary.remove_announcement()
-    assert not glossary.has_announcement()
-    assert glossary.attributes.announcement_title is None
-    assert glossary.attributes.announcement_type is None
-    assert glossary.attributes.announcement_message is None
-
-
 @pytest.mark.parametrize(
     "name, connector_type, admin_users, admin_groups, admin_roles, error",
     [
         (None, AtlanConnectorType.BIGQUERY, None, None, ["123"], ValueError),
         ("", AtlanConnectorType.BIGQUERY, None, None, ["123"], ValueError),
         ("query", None, None, None, ["123"], ValueError),
         ("query", AtlanConnectorType.BIGQUERY, None, None, None, ValueError),
         ("query", AtlanConnectorType.BIGQUERY, [], [], [], ValueError),
     ],
 )
 def test_connection_attributes_create_without_required_parameters_raises_validation_error(
     name, connector_type, admin_users, admin_groups, admin_roles, error
 ):
     with pytest.raises(error):
-        Connection.Attributes.create(
+        Connection.Attributes(
             name=name,
             connector_type=connector_type,
             admin_users=admin_users,
             admin_groups=admin_groups,
             admin_roles=admin_roles,
-        )
+        ).validate_required()
 
 
 @pytest.mark.parametrize(
     "name, connector_type, admin_users, admin_groups, admin_roles",
     [
         ("query", AtlanConnectorType.BIGQUERY, {"bob"}, None, None),
         ("query", AtlanConnectorType.BIGQUERY, None, {"bob"}, None),
         ("query", AtlanConnectorType.BIGQUERY, None, None, {"bob"}),
         ("query", AtlanConnectorType.BIGQUERY, {"bob"}, {"ted"}, {"alice"}),
     ],
 )
 def test_connection_attributes_create_with_required_parameters(
     name, connector_type, admin_users, admin_groups, admin_roles
 ):
-    c = Connection.Attributes.create(
+    c = Connection.Attributes(
         name=name,
-        connector_type=connector_type,
+        qualified_name=connector_type.to_qualified_name(),
+        connector_name=connector_type.value,
+        category=connector_type.category.value,
         admin_users=admin_users,
         admin_groups=admin_groups,
         admin_roles=admin_roles,
     )
     assert c.qualified_name
     assert c.qualified_name <= connector_type.to_qualified_name()
     assert c.connector_name == connector_type.value
     assert c.category == connector_type.category.value
     assert c.admin_roles == admin_roles
     assert c.admin_users == admin_users
     assert c.admin_groups == admin_groups
 
 
 @pytest.mark.parametrize(
-    "name, connector_type, admin_users, admin_groups, admin_roles",
-    [("somequery", AtlanConnectorType.BIGQUERY, {"bob"}, {"ted"}, {"alice"})],
-)
-def test_connection_create_with_required_parameters(
-    name, connector_type, admin_users, admin_groups, admin_roles
-):
-    c = Connection.create(
-        name=name,
-        connector_type=connector_type,
-        admin_users=admin_users,
-        admin_groups=admin_groups,
-        admin_roles=admin_roles,
-    )
-    assert c.attributes.qualified_name
-    assert c.attributes.qualified_name <= connector_type.to_qualified_name()
-    assert c.attributes.connector_name == connector_type.value
-    assert c.attributes.category == connector_type.category.value
-    assert c.attributes.admin_roles == admin_roles
-    assert c.attributes.admin_users == admin_users
-    assert c.attributes.admin_groups == admin_groups
-
-
-@pytest.mark.parametrize(
     "name, connector_type, admin_users, admin_groups, admin_roles, error",
     [
         (None, AtlanConnectorType.BIGQUERY, None, None, ["123"], ValueError),
         ("", AtlanConnectorType.BIGQUERY, None, None, ["123"], ValueError),
         ("SomeQuery", None, None, None, ["123"], ValueError),
         ("SomeQuery", AtlanConnectorType.BIGQUERY, None, None, None, ValueError),
         ("SomeQuery", AtlanConnectorType.BIGQUERY, [], [], [], ValueError),
@@ -1304,144 +1222,14 @@
 def test_glossary_term_attributes_create_sets_name_anchor():
     glossary = AtlasGlossary.create(name="Glossary")
     sut = AtlasGlossaryTerm.Attributes.create(name="Bob", anchor=glossary)
     assert sut.name == "Bob"
     assert sut.anchor == glossary
 
 
-@patch("pyatlan.cache.custom_metadata_cache.AtlanClient")
-def test_get_business_attributes_when_name_not_valid_raises_not_found_error(
-    mock_client, table, type_def_response
-):
-    mock_client.return_value.get_typedefs.return_value = type_def_response
-    with pytest.raises(
-        NotFoundError, match="Custom metadata with name Zoro does not exist."
-    ):
-        table.get_custom_metadata("Zoro")
-
-
-@patch("pyatlan.cache.custom_metadata_cache.AtlanClient")
-def test_get_business_attributes_when_name_not_appropriate_for_asset_raises_value_error(
-    mock_client, table, type_def_response
-):
-    mock_client.get_default_client.return_value = mock_client
-    mock_client.get_typedefs.return_value = type_def_response
-    with pytest.raises(
-        ValueError, match="Custom metadata attributes Moon are not applicable to Table"
-    ):
-        table.get_custom_metadata("Moon")
-
-
-@patch("pyatlan.cache.custom_metadata_cache.AtlanClient")
-def test_get_business_attributes_with_valid_name_returns_empty_attribute_when_table_does_not_have_attribute(
-    mock_client, table, type_def_response
-):
-    mock_client.return_value.get_typedefs.return_value = type_def_response
-
-    monte_carlo = table.get_custom_metadata("Monte Carlo")
-
-    assert monte_carlo is not None
-    assert monte_carlo.freshness is None
-    assert monte_carlo.freshness_date is None
-    assert monte_carlo.table_url is None
-
-
-@patch("pyatlan.cache.custom_metadata_cache.AtlanClient")
-def test_get_business_attributes_with_valid_name_returns_attribute_when_table_has_attribute(
-    mock_client, table, type_def_response
-):
-    mock_client.return_value.get_typedefs.return_value = type_def_response
-    table.business_attributes = {
-        MONTE_CARLO: {
-            FRESHNESS: "pass",
-            TABLE_URL: "https://getmontecarlo.com/catalog/",
-        }
-    }
-
-    monte_carlo = table.get_custom_metadata("Monte Carlo")
-
-    assert monte_carlo is not None
-    assert monte_carlo.freshness == "pass"
-    assert monte_carlo.table_url == "https://getmontecarlo.com/catalog/"
-
-
-def test_set_busines_attributes_with_non_business_attributes_object_raises_value_error(
-    table,
-):
-    with pytest.raises(
-        ValueError,
-        match="business_attributes must be an instance of CustomMetadata",
-    ):
-        table.set_custom_metadata({})
-
-
-def test_set_business_attributes_with_non_appropriate_meta_data_type_name_raises_value_error(
-    table,
-):
-    with pytest.raises(
-        ValueError,
-        match="business_attributes must be an instance of CustomMetadata",
-    ):
-        table.set_custom_metadata({})
-
-
-@patch("pyatlan.cache.custom_metadata_cache.AtlanClient")
-def test_assigning_to_invalid_business_attribute_raises_attribute_error(
-    mock_client, table, type_def_response
-):
-    mock_client.return_value.get_typedefs.return_value = type_def_response
-    table.business_attributes = {
-        MONTE_CARLO: {
-            FRESHNESS: "pass",
-            TABLE_URL: "https://getmontecarlo.com/catalog/",
-        }
-    }
-    business_attributes = table.get_custom_metadata("Monte Carlo")
-    with pytest.raises(AttributeError, match="Attribute bogus does not exist"):
-        business_attributes.bogus = "123"
-
-
-@patch("pyatlan.cache.custom_metadata_cache.AtlanClient")
-def test_set_business_attributes_with_business_attribute_not_appropriate_to_asset_raises_value_error(
-    mock_client, table, type_def_response
-):
-    mock_client.return_value.get_typedefs.return_value = type_def_response
-
-    moon = CustomMetadataCache.get_type_for_id(MOON)()
-
-    with pytest.raises(
-        ValueError,
-        match="Business attributes Moon are not applicable to Table",
-    ):
-        table.set_custom_metadata(moon)
-
-
-@patch("pyatlan.cache.custom_metadata_cache.AtlanClient")
-def test_set_business_attributes_with_appropriate_business_attribute_updates_dictionary(
-    mock_client, table, type_def_response
-):
-    mock_client.return_value.get_typedefs.return_value = type_def_response
-
-    table.business_attributes = {
-        MONTE_CARLO: {
-            FRESHNESS: "pass",
-            TABLE_URL: "https://getmontecarlo.com/catalog/",
-        }
-    }
-    monte_carlo = table.get_custom_metadata("Monte Carlo")
-
-    monte_carlo.freshness = "fail"
-    monte_carlo.table_url = "http://anywhere.com"
-    table.set_custom_metadata(monte_carlo)
-
-    monte_carlo_dict = table.business_attributes[MONTE_CARLO]
-    assert monte_carlo_dict[FRESHNESS] == monte_carlo.freshness
-    assert monte_carlo_dict[TABLE_URL] == monte_carlo.table_url
-
-
 @pytest.mark.parametrize(
     "cls, name, connection_qualified_name, aws_arn, msg",
     [
         (cls, values[0], values[1], values[2], values[3])
         for values in [
             (None, "default/s3/production", "abc", "name is required"),
             ("my-bucket", None, "abc", "connection_qualified_name is required"),
```

### Comparing `pyatlan-0.0.33/tests/unit/test_search_model.py` & `pyatlan-0.1.0/tests/unit/test_search_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.33/tests/unit/test_typedef_model.py` & `pyatlan-0.1.0/tests/unit/test_typedef_model.py`

 * *Files identical despite different names*

