# Comparing `tmp/gen3_util-0.0.2rc2.tar.gz` & `tmp/gen3_util-0.0.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen3_util-0.0.2rc2.tar", last modified: Mon Jun  5 20:44:26 2023, max compression
+gzip compressed data, was "gen3_util-0.0.2rc3.tar", last modified: Mon Jun  5 23:59:58 2023, max compression
```

## Comparing `gen3_util-0.0.2rc2.tar` & `gen3_util-0.0.2rc3.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 20:44:26.632985 gen3_util-0.0.2rc2/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1065 2023-05-04 14:32:05.000000 gen3_util-0.0.2rc2/LICENSE
--rw-r--r--   0 walsbr   (320923486) 1971611142     7059 2023-06-05 20:44:26.632799 gen3_util-0.0.2rc2/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     6374 2023-05-25 21:06:12.000000 gen3_util-0.0.2rc2/README.md
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 20:44:26.589522 gen3_util-0.0.2rc2/gen3_util/
--rw-r--r--   0 walsbr   (320923486) 1971611142       71 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc2/gen3_util/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 20:44:26.597962 gen3_util-0.0.2rc2/gen3_util/access/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1819 2023-05-12 00:08:03.000000 gen3_util-0.0.2rc2/gen3_util/access/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1948 2023-05-12 00:08:03.000000 gen3_util-0.0.2rc2/gen3_util/access/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1869 2023-05-11 17:49:58.000000 gen3_util-0.0.2rc2/gen3_util/access/requestor.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 20:44:26.603402 gen3_util-0.0.2rc2/gen3_util/buckets/
--rw-r--r--   0 walsbr   (320923486) 1971611142      803 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/buckets/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      628 2023-05-12 12:59:15.000000 gen3_util-0.0.2rc2/gen3_util/buckets/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      474 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/buckets/lister.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 20:44:26.604403 gen3_util-0.0.2rc2/gen3_util/cli/
--rw-r--r--   0 walsbr   (320923486) 1971611142     4355 2023-06-01 15:53:03.000000 gen3_util-0.0.2rc2/gen3_util/cli/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1667 2023-05-10 23:46:59.000000 gen3_util-0.0.2rc2/gen3_util/cli/cli.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 20:44:26.604880 gen3_util-0.0.2rc2/gen3_util/common/
--rw-r--r--   0 walsbr   (320923486) 1971611142     4119 2023-06-01 15:00:31.000000 gen3_util-0.0.2rc2/gen3_util/common/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 20:44:26.606081 gen3_util-0.0.2rc2/gen3_util/config/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2425 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/config/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      485 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/config/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      503 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/config/config.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 20:44:26.624043 gen3_util-0.0.2rc2/gen3_util/files/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1270 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/files/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2246 2023-05-12 13:00:59.000000 gen3_util-0.0.2rc2/gen3_util/files/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      920 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/files/downloader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      192 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/files/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      202 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/files/remover.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    13289 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/files/uploader.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 20:44:26.627087 gen3_util-0.0.2rc2/gen3_util/meta/
--rw-r--r--   0 walsbr   (320923486) 1971611142     4117 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/meta/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1291 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/meta/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      210 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc2/gen3_util/meta/downloader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     5483 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/meta/importer.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      191 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/meta/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      201 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/meta/remover.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      208 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/meta/uploader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3248 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/meta/validator.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 20:44:26.628677 gen3_util-0.0.2rc2/gen3_util/projects/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2247 2023-06-01 15:31:29.000000 gen3_util-0.0.2rc2/gen3_util/projects/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1660 2023-06-01 15:39:25.000000 gen3_util-0.0.2rc2/gen3_util/projects/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1888 2023-06-01 14:31:34.000000 gen3_util-0.0.2rc2/gen3_util/projects/creator.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1112 2023-06-01 15:38:13.000000 gen3_util-0.0.2rc2/gen3_util/projects/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1040 2023-06-01 14:31:34.000000 gen3_util-0.0.2rc2/gen3_util/projects/remover.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 20:44:26.596214 gen3_util-0.0.2rc2/gen3_util.egg-info/
--rw-r--r--   0 walsbr   (320923486) 1971611142     7059 2023-06-05 20:44:26.000000 gen3_util-0.0.2rc2/gen3_util.egg-info/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     1502 2023-06-05 20:44:26.000000 gen3_util-0.0.2rc2/gen3_util.egg-info/SOURCES.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142        1 2023-06-05 20:44:26.000000 gen3_util-0.0.2rc2/gen3_util.egg-info/dependency_links.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       53 2023-06-05 20:44:26.000000 gen3_util-0.0.2rc2/gen3_util.egg-info/entry_points.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142      128 2023-06-05 20:44:26.000000 gen3_util-0.0.2rc2/gen3_util.egg-info/requires.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       16 2023-06-05 20:44:26.000000 gen3_util-0.0.2rc2/gen3_util.egg-info/top_level.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       38 2023-06-05 20:44:26.633035 gen3_util-0.0.2rc2/setup.cfg
--rw-r--r--   0 walsbr   (320923486) 1971611142     5580 2023-06-05 20:44:08.000000 gen3_util-0.0.2rc2/setup.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 20:44:26.586303 gen3_util-0.0.2rc2/tests/
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 20:44:26.630462 gen3_util-0.0.2rc2/tests/integration/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc2/tests/integration/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      108 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc2/tests/integration/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2941 2023-05-12 13:32:44.000000 gen3_util-0.0.2rc2/tests/integration/test_access.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      433 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/tests/integration/test_buckets.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2047 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/tests/integration/test_files.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1225 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/tests/integration/test_project.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 20:44:26.632492 gen3_util-0.0.2rc2/tests/unit/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc2/tests/unit/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      322 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc2/tests/unit/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3222 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/tests/unit/test_cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      565 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc2/tests/unit/test_coding_conventions.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      551 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc2/tests/unit/test_config.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1760 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/tests/unit/test_files.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      867 2023-05-11 22:42:33.000000 gen3_util-0.0.2rc2/tests/unit/test_meta.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1546 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/tests/unit/test_validate_directory.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 23:59:58.831361 gen3_util-0.0.2rc3/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1065 2023-05-04 14:32:05.000000 gen3_util-0.0.2rc3/LICENSE
+-rw-r--r--   0 walsbr   (320923486) 1971611142     7059 2023-06-05 23:59:58.831184 gen3_util-0.0.2rc3/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     6374 2023-05-25 21:06:12.000000 gen3_util-0.0.2rc3/README.md
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 23:59:58.786926 gen3_util-0.0.2rc3/gen3_util/
+-rw-r--r--   0 walsbr   (320923486) 1971611142       71 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc3/gen3_util/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 23:59:58.790365 gen3_util-0.0.2rc3/gen3_util/access/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1819 2023-05-12 00:08:03.000000 gen3_util-0.0.2rc3/gen3_util/access/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1948 2023-05-12 00:08:03.000000 gen3_util-0.0.2rc3/gen3_util/access/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1869 2023-05-11 17:49:58.000000 gen3_util-0.0.2rc3/gen3_util/access/requestor.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 23:59:58.791476 gen3_util-0.0.2rc3/gen3_util/buckets/
+-rw-r--r--   0 walsbr   (320923486) 1971611142      803 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc3/gen3_util/buckets/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      629 2023-06-05 23:40:34.000000 gen3_util-0.0.2rc3/gen3_util/buckets/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      474 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc3/gen3_util/buckets/lister.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 23:59:58.795259 gen3_util-0.0.2rc3/gen3_util/cli/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4469 2023-06-05 23:43:44.000000 gen3_util-0.0.2rc3/gen3_util/cli/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1667 2023-05-10 23:46:59.000000 gen3_util-0.0.2rc3/gen3_util/cli/cli.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 23:59:58.798437 gen3_util-0.0.2rc3/gen3_util/common/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4119 2023-06-01 15:00:31.000000 gen3_util-0.0.2rc3/gen3_util/common/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 23:59:58.807342 gen3_util-0.0.2rc3/gen3_util/config/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2425 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc3/gen3_util/config/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      485 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc3/gen3_util/config/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      503 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc3/gen3_util/config/config.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 23:59:58.809815 gen3_util-0.0.2rc3/gen3_util/files/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1285 2023-06-05 23:52:37.000000 gen3_util-0.0.2rc3/gen3_util/files/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2246 2023-05-12 13:00:59.000000 gen3_util-0.0.2rc3/gen3_util/files/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      920 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc3/gen3_util/files/downloader.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      192 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc3/gen3_util/files/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      202 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc3/gen3_util/files/remover.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    13289 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc3/gen3_util/files/uploader.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 23:59:58.821319 gen3_util-0.0.2rc3/gen3_util/meta/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4117 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc3/gen3_util/meta/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1291 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc3/gen3_util/meta/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      210 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc3/gen3_util/meta/downloader.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5483 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc3/gen3_util/meta/importer.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      191 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc3/gen3_util/meta/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      201 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc3/gen3_util/meta/remover.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      208 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc3/gen3_util/meta/uploader.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3248 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc3/gen3_util/meta/validator.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 23:59:58.827922 gen3_util-0.0.2rc3/gen3_util/projects/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2247 2023-06-01 15:31:29.000000 gen3_util-0.0.2rc3/gen3_util/projects/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1667 2023-06-05 23:49:25.000000 gen3_util-0.0.2rc3/gen3_util/projects/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1888 2023-06-01 14:31:34.000000 gen3_util-0.0.2rc3/gen3_util/projects/creator.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      793 2023-06-05 23:48:55.000000 gen3_util-0.0.2rc3/gen3_util/projects/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1040 2023-06-01 14:31:34.000000 gen3_util-0.0.2rc3/gen3_util/projects/remover.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 23:59:58.789489 gen3_util-0.0.2rc3/gen3_util.egg-info/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     7059 2023-06-05 23:59:58.000000 gen3_util-0.0.2rc3/gen3_util.egg-info/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1502 2023-06-05 23:59:58.000000 gen3_util-0.0.2rc3/gen3_util.egg-info/SOURCES.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142        1 2023-06-05 23:59:58.000000 gen3_util-0.0.2rc3/gen3_util.egg-info/dependency_links.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       53 2023-06-05 23:59:58.000000 gen3_util-0.0.2rc3/gen3_util.egg-info/entry_points.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142      128 2023-06-05 23:59:58.000000 gen3_util-0.0.2rc3/gen3_util.egg-info/requires.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       16 2023-06-05 23:59:58.000000 gen3_util-0.0.2rc3/gen3_util.egg-info/top_level.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       38 2023-06-05 23:59:58.831416 gen3_util-0.0.2rc3/setup.cfg
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5580 2023-06-05 23:59:34.000000 gen3_util-0.0.2rc3/setup.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 23:59:58.780561 gen3_util-0.0.2rc3/tests/
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 23:59:58.829261 gen3_util-0.0.2rc3/tests/integration/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc3/tests/integration/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      108 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc3/tests/integration/conftest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2941 2023-05-12 13:32:44.000000 gen3_util-0.0.2rc3/tests/integration/test_access.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      433 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc3/tests/integration/test_buckets.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2055 2023-06-05 23:54:31.000000 gen3_util-0.0.2rc3/tests/integration/test_files.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1225 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc3/tests/integration/test_project.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 23:59:58.830938 gen3_util-0.0.2rc3/tests/unit/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc3/tests/unit/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      322 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc3/tests/unit/conftest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3222 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc3/tests/unit/test_cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      565 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc3/tests/unit/test_coding_conventions.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      551 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc3/tests/unit/test_config.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1760 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc3/tests/unit/test_files.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      867 2023-05-11 22:42:33.000000 gen3_util-0.0.2rc3/tests/unit/test_meta.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1546 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc3/tests/unit/test_validate_directory.py
```

### Comparing `gen3_util-0.0.2rc2/LICENSE` & `gen3_util-0.0.2rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc2/PKG-INFO` & `gen3_util-0.0.2rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3_util
-Version: 0.0.2rc2
+Version: 0.0.2rc3
 Summary: Commons utilities
 Home-page: https://github.com/ACED-IDP/gen3_util
 Author: Ellrott Lab
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/ACED-IDP/gen3_util/issues
 Project-URL: Source, https://github.com/ACED-IDP/gen3_util
 Keywords: gen3 bioinformatics
```

### Comparing `gen3_util-0.0.2rc2/README.md` & `gen3_util-0.0.2rc3/README.md`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc2/gen3_util/access/__init__.py` & `gen3_util-0.0.2rc3/gen3_util/access/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc2/gen3_util/access/cli.py` & `gen3_util-0.0.2rc3/gen3_util/access/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc2/gen3_util/access/requestor.py` & `gen3_util-0.0.2rc3/gen3_util/access/requestor.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc2/gen3_util/buckets/__init__.py` & `gen3_util-0.0.2rc3/gen3_util/buckets/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc2/gen3_util/buckets/cli.py` & `gen3_util-0.0.2rc3/gen3_util/buckets/cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 
 @bucket_group.command(name="ls")
 @click.pass_obj
 def ls_command(config: Config):
     """Test connectivity to Gen3 endpoint."""
     with CLIOutput(config=config) as output:
         auth = ensure_auth(config.gen3.refresh_file, validate=True)
-        output['endpoint'] = auth.endpoint
-        output.update(ls(config).dict())
+        output.update({'endpoint': auth.endpoint})
+        output.update(ls(config))
```

### Comparing `gen3_util-0.0.2rc2/gen3_util/cli/__init__.py` & `gen3_util-0.0.2rc3/gen3_util/cli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,18 @@
     def __enter__(self):
         return self.output
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         rc = 0
         _ = {}
         if self.output.obj is not None:
-            _.update(self.output.obj.dict())
+            if isinstance(self.output.obj, dict):
+                _.update(self.output.obj)
+            else:
+                _.update(self.output.obj.dict())
         if exc_type is not None:
             _['exception'] = f"{str(exc_val)}"
             rc = 1
             logging.getLogger(__name__).exception(exc_val)
         if 'msg' not in _:
             if rc == 1:
                 _['msg'] = 'FAIL'
```

### Comparing `gen3_util-0.0.2rc2/gen3_util/cli/cli.py` & `gen3_util-0.0.2rc3/gen3_util/cli/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc2/gen3_util/common/__init__.py` & `gen3_util-0.0.2rc3/gen3_util/common/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc2/gen3_util/config/__init__.py` & `gen3_util-0.0.2rc3/gen3_util/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc2/gen3_util/files/__init__.py` & `gen3_util-0.0.2rc3/gen3_util/files/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,8 +28,8 @@
         logger.warning(f"project {project} does not exist")
     assert all([program_exists, project_exists]), f"{project_id} does not exist."
 
 
 def assert_valid_bucket(config, bucket_name):
     buckets = get_buckets(config=config)
     bucket_names = [_ for _ in buckets['GS_BUCKETS']] + [_ for _ in buckets['S3_BUCKETS']]
-    assert bucket_name in bucket_names, f"{bucket_name} not in configured buckets"
+    assert bucket_name in bucket_names, f"{bucket_name} not in configured buckets {bucket_names}"
```

### Comparing `gen3_util-0.0.2rc2/gen3_util/files/cli.py` & `gen3_util-0.0.2rc3/gen3_util/files/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc2/gen3_util/files/downloader.py` & `gen3_util-0.0.2rc3/gen3_util/files/downloader.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc2/gen3_util/files/uploader.py` & `gen3_util-0.0.2rc3/gen3_util/files/uploader.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc2/gen3_util/meta/__init__.py` & `gen3_util-0.0.2rc3/gen3_util/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc2/gen3_util/meta/cli.py` & `gen3_util-0.0.2rc3/gen3_util/meta/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc2/gen3_util/meta/importer.py` & `gen3_util-0.0.2rc3/gen3_util/meta/importer.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc2/gen3_util/meta/validator.py` & `gen3_util-0.0.2rc3/gen3_util/meta/validator.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc2/gen3_util/projects/__init__.py` & `gen3_util-0.0.2rc3/gen3_util/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc2/gen3_util/projects/cli.py` & `gen3_util-0.0.2rc3/gen3_util/projects/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 @project_group.command(name="ping")
 @click.pass_obj
 def ping(config: Config):
     """Test connectivity to Gen3 endpoint."""
     with CLIOutput(config=config) as output:
         auth = ensure_auth(config.gen3.refresh_file, validate=True)
-        output['endpoint'] = auth.endpoint
+        output.update({'endpoint': auth.endpoint})
 
 
 @project_group.command(name="ls")
 @click.pass_obj
 def project_ls(config: Config):
     """List all projects user has access to."""
     with CLIOutput(config=config) as output:
@@ -49,8 +49,7 @@
 @click.pass_obj
 def project_rm(config: Config, project_id: str):
     """Remove project.
     PROJECT_ID: /programs/XXX/project/YYY
     """
     with CLIOutput(config=config) as output:
         output.update(rm(config, project_id))
-
```

### Comparing `gen3_util-0.0.2rc2/gen3_util/projects/creator.py` & `gen3_util-0.0.2rc3/gen3_util/projects/creator.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc2/gen3_util/projects/lister.py` & `gen3_util-0.0.2rc3/gen3_util/projects/remover.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,32 @@
-
 from gen3.submission import Gen3Submission
+from requests import HTTPError
 
 from gen3_util.config import Config, ensure_auth
-from gen3_util.projects import get_user, ProjectSummaries, get_projects, ProjectSummary
-
+from gen3_util.projects import ProjectSummaries
 
-def ls(config: Config) -> ProjectSummaries:
-    """List projects."""
-    auth = ensure_auth(config.gen3.refresh_file)
-    user = get_user(auth=auth)
-    return ProjectSummaries(**{
-        'endpoint': auth.endpoint,
-        'projects': [_ for _ in user['authz'].keys() if _.startswith('/programs')],
-    })
 
-
-def ls(config: Config):
-    """List projects."""
+def rm(config: Config, project_id: str):
+    """Remove project."""
+    assert '-' in project_id, f'Invalid project_id: {project_id}'
+    program, project = project_id.split('-')
+    assert program and project, f'Invalid project_id: {project_id}'
 
     auth = ensure_auth(config.gen3.refresh_file)
     submission = Gen3Submission(auth)
 
-    msgs = []
-    projects = get_projects(auth, submission)
-
-    project_messages = {}
-    for _program in projects:
-        for _project in projects[_program]['projects']:
-            project_messages[
-                f"/programs/{_program}/projects/{_project}"
-            ] = ProjectSummary(exists=projects[_program]['projects'][_project])
-
-    return ProjectSummaries(**{
-        'endpoint': auth.endpoint,
-        'projects': project_messages,
-        'messages': msgs
-    })
+    try:
+        response = submission.delete_project(program=program, project=project)
+        response.raise_for_status()
+
+        return ProjectSummaries(**{
+            'endpoint': auth.endpoint,
+            'projects': [project_id],
+            'messages': [f'Deleted {project_id}']
+        })
+
+    except HTTPError as e:
+        return ProjectSummaries(**{
+            'endpoint': auth.endpoint,
+            'projects': [project_id],
+            'messages': [f'Error deleting {project_id}: {e} {e.response.text}']
+        })
```

### Comparing `gen3_util-0.0.2rc2/gen3_util.egg-info/PKG-INFO` & `gen3_util-0.0.2rc3/gen3_util.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3-util
-Version: 0.0.2rc2
+Version: 0.0.2rc3
 Summary: Commons utilities
 Home-page: https://github.com/ACED-IDP/gen3_util
 Author: Ellrott Lab
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/ACED-IDP/gen3_util/issues
 Project-URL: Source, https://github.com/ACED-IDP/gen3_util
 Keywords: gen3 bioinformatics
```

### Comparing `gen3_util-0.0.2rc2/gen3_util.egg-info/SOURCES.txt` & `gen3_util-0.0.2rc3/gen3_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc2/setup.py` & `gen3_util-0.0.2rc3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
     name='gen3_util',  # Required
 
     # Versions should comply with PEP 440:
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.2-rc2',  # Required
+    version='0.0.2-rc3',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Commons utilities',
     # Optional
```

### Comparing `gen3_util-0.0.2rc2/tests/integration/test_access.py` & `gen3_util-0.0.2rc3/tests/integration/test_access.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc2/tests/integration/test_files.py` & `gen3_util-0.0.2rc3/tests/integration/test_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,13 +35,13 @@
     assert result.exit_code == 1
     print(result.output)
     expected_strings = ['bar not in configured buckets']
     for expected_string in expected_strings:
         assert expected_string in result.output, "Did not find bucket does not exist error"
 
     result = runner.invoke(cli, ['files', 'cp', '--project_id', 'aced-Alcoholism', '--ignore_state',
-                                 'tmp/Alcoholism/DocumentReference.ndjson', 'bucket://aced-ohsu'])
+                                 'tmp/Alcoholism/DocumentReference.ndjson', 'bucket://aced-ohsu-staging'])
     assert result.exit_code == 0
     print(result.output)
     expected_strings = ['OK']
     for expected_string in expected_strings:
         assert expected_string in result.output, "Did not find OK message"
```

### Comparing `gen3_util-0.0.2rc2/tests/integration/test_project.py` & `gen3_util-0.0.2rc3/tests/integration/test_project.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc2/tests/unit/test_cli.py` & `gen3_util-0.0.2rc3/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc2/tests/unit/test_coding_conventions.py` & `gen3_util-0.0.2rc3/tests/unit/test_coding_conventions.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc2/tests/unit/test_config.py` & `gen3_util-0.0.2rc3/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc2/tests/unit/test_files.py` & `gen3_util-0.0.2rc3/tests/unit/test_files.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc2/tests/unit/test_meta.py` & `gen3_util-0.0.2rc3/tests/unit/test_meta.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc2/tests/unit/test_validate_directory.py` & `gen3_util-0.0.2rc3/tests/unit/test_validate_directory.py`

 * *Files identical despite different names*

