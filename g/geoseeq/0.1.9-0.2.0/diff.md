# Comparing `tmp/geoseeq-0.1.9.tar.gz` & `tmp/geoseeq-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoseeq-0.1.9.tar", last modified: Wed Mar  8 14:59:14 2023, max compression
+gzip compressed data, was "geoseeq-0.2.0.tar", last modified: Tue Jun  6 16:56:51 2023, max compression
```

## Comparing `geoseeq-0.1.9.tar` & `geoseeq-0.2.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2023-03-08 14:59:14.000184 geoseeq-0.1.9/
--rw-r--r--   0 dcdanko    (501) staff       (20)     1067 2023-02-09 21:51:44.000000 geoseeq-0.1.9/LICENSE
--rw-r--r--   0 dcdanko    (501) staff       (20)      341 2023-03-08 14:59:14.000027 geoseeq-0.1.9/PKG-INFO
--rw-r--r--   0 dcdanko    (501) staff       (20)     1112 2023-02-10 02:57:33.000000 geoseeq-0.1.9/README.md
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2023-03-08 14:59:13.993993 geoseeq-0.1.9/geoseeq/
--rw-r--r--   0 dcdanko    (501) staff       (20)      712 2023-02-09 20:30:23.000000 geoseeq-0.1.9/geoseeq/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)    22221 2023-03-08 14:57:47.000000 geoseeq-0.1.9/geoseeq/analysis_result.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     5314 2023-02-05 03:22:49.000000 geoseeq-0.1.9/geoseeq/blob_constructors.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1963 2023-02-09 20:30:23.000000 geoseeq-0.1.9/geoseeq/bulk_creators.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2023-03-08 14:59:13.997147 geoseeq-0.1.9/geoseeq/cli/
--rw-r--r--   0 dcdanko    (501) staff       (20)       24 2023-01-20 01:26:16.000000 geoseeq-0.1.9/geoseeq/cli/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1393 2023-02-10 03:30:51.000000 geoseeq-0.1.9/geoseeq/cli/add.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      176 2023-01-20 01:26:16.000000 geoseeq-0.1.9/geoseeq/cli/constants.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1997 2023-02-10 03:31:15.000000 geoseeq-0.1.9/geoseeq/cli/copy.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     6686 2023-02-10 03:31:24.000000 geoseeq-0.1.9/geoseeq/cli/create.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      919 2023-02-10 03:31:43.000000 geoseeq-0.1.9/geoseeq/cli/delete.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3968 2023-02-10 03:31:48.000000 geoseeq-0.1.9/geoseeq/cli/download.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3083 2023-01-20 01:26:16.000000 geoseeq-0.1.9/geoseeq/cli/fastq_utils.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      568 2023-02-10 03:31:56.000000 geoseeq-0.1.9/geoseeq/cli/list.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      975 2023-03-08 14:58:29.000000 geoseeq-0.1.9/geoseeq/cli/main.py
--rw-r--r--   0 dcdanko    (501) staff       (20)    10120 2023-02-24 17:33:38.000000 geoseeq-0.1.9/geoseeq/cli/upload.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      925 2023-02-10 03:32:14.000000 geoseeq-0.1.9/geoseeq/cli/user.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2564 2023-02-24 16:14:04.000000 geoseeq-0.1.9/geoseeq/cli/utils.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      645 2023-02-14 22:10:03.000000 geoseeq-0.1.9/geoseeq/cli/view.py
--rw-r--r--   0 dcdanko    (501) staff       (20)       26 2023-01-20 01:26:16.000000 geoseeq-0.1.9/geoseeq/constants.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2023-03-08 14:59:13.997289 geoseeq-0.1.9/geoseeq/contrib/
--rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-01-20 01:26:16.000000 geoseeq-0.1.9/geoseeq/contrib/__init__.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2023-03-08 14:59:13.997969 geoseeq-0.1.9/geoseeq/contrib/ncbi/
--rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-01-20 01:26:16.000000 geoseeq-0.1.9/geoseeq/contrib/ncbi/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1056 2023-02-09 21:51:44.000000 geoseeq-0.1.9/geoseeq/contrib/ncbi/api.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4341 2023-02-09 21:51:44.000000 geoseeq-0.1.9/geoseeq/contrib/ncbi/bioproject.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2400 2023-02-10 03:00:45.000000 geoseeq-0.1.9/geoseeq/contrib/ncbi/cli.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      175 2023-01-20 01:26:16.000000 geoseeq-0.1.9/geoseeq/contrib/ncbi/setup_logging.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3405 2023-01-20 01:26:16.000000 geoseeq-0.1.9/geoseeq/file_system_cache.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     5897 2023-02-09 20:30:23.000000 geoseeq-0.1.9/geoseeq/knex.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1965 2023-01-20 01:26:16.000000 geoseeq-0.1.9/geoseeq/organization.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4265 2023-01-20 01:26:16.000000 geoseeq-0.1.9/geoseeq/pipeline.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     6085 2023-02-24 16:14:34.000000 geoseeq-0.1.9/geoseeq/remote_object.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4287 2023-02-10 01:07:36.000000 geoseeq-0.1.9/geoseeq/sample.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     6555 2023-02-09 20:30:23.000000 geoseeq-0.1.9/geoseeq/sample_group.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      690 2023-01-20 01:26:16.000000 geoseeq-0.1.9/geoseeq/user.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1118 2023-01-20 01:26:16.000000 geoseeq-0.1.9/geoseeq/utils.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2023-03-08 14:59:13.999448 geoseeq-0.1.9/geoseeq/vc/
--rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-02-10 03:25:58.000000 geoseeq-0.1.9/geoseeq/vc/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      710 2023-02-10 03:23:35.000000 geoseeq-0.1.9/geoseeq/vc/checksum.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2853 2023-02-10 03:33:48.000000 geoseeq-0.1.9/geoseeq/vc/cli.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2486 2023-01-20 01:26:16.000000 geoseeq-0.1.9/geoseeq/vc/clone.py
--rw-r--r--   0 dcdanko    (501) staff       (20)       19 2023-01-20 01:26:16.000000 geoseeq-0.1.9/geoseeq/vc/constants.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      730 2023-01-20 01:26:16.000000 geoseeq-0.1.9/geoseeq/vc/vc_cache.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      457 2023-01-20 01:26:16.000000 geoseeq-0.1.9/geoseeq/vc/vc_dir.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3900 2023-02-10 03:23:23.000000 geoseeq-0.1.9/geoseeq/vc/vc_sample.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3160 2023-02-10 03:23:17.000000 geoseeq-0.1.9/geoseeq/vc/vc_stub.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     8076 2023-01-20 01:26:16.000000 geoseeq-0.1.9/geoseeq/work_orders.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2023-03-08 14:59:13.994982 geoseeq-0.1.9/geoseeq.egg-info/
--rw-r--r--   0 dcdanko    (501) staff       (20)      341 2023-03-08 14:59:13.000000 geoseeq-0.1.9/geoseeq.egg-info/PKG-INFO
--rw-r--r--   0 dcdanko    (501) staff       (20)     1326 2023-03-08 14:59:13.000000 geoseeq-0.1.9/geoseeq.egg-info/SOURCES.txt
--rw-r--r--   0 dcdanko    (501) staff       (20)        1 2023-03-08 14:59:13.000000 geoseeq-0.1.9/geoseeq.egg-info/dependency_links.txt
--rw-r--r--   0 dcdanko    (501) staff       (20)       45 2023-03-08 14:59:13.000000 geoseeq-0.1.9/geoseeq.egg-info/entry_points.txt
--rw-r--r--   0 dcdanko    (501) staff       (20)       32 2023-03-08 14:59:13.000000 geoseeq-0.1.9/geoseeq.egg-info/requires.txt
--rw-r--r--   0 dcdanko    (501) staff       (20)       14 2023-03-08 14:59:13.000000 geoseeq-0.1.9/geoseeq.egg-info/top_level.txt
--rw-r--r--   0 dcdanko    (501) staff       (20)       86 2023-02-10 03:38:06.000000 geoseeq-0.1.9/pyproject.toml
--rw-r--r--   0 dcdanko    (501) staff       (20)       38 2023-03-08 14:59:14.000230 geoseeq-0.1.9/setup.cfg
--rw-r--r--   0 dcdanko    (501) staff       (20)      783 2023-03-08 14:59:09.000000 geoseeq-0.1.9/setup.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2023-03-08 14:59:13.999839 geoseeq-0.1.9/tests/
--rw-r--r--   0 dcdanko    (501) staff       (20)        0 2022-11-14 20:29:34.000000 geoseeq-0.1.9/tests/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)    14444 2023-01-20 01:26:16.000000 geoseeq-0.1.9/tests/test_api_client.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      498 2023-01-20 01:26:16.000000 geoseeq-0.1.9/tests/test_work_orders.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2023-06-06 16:56:51.495526 geoseeq-0.2.0/
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1067 2023-02-09 21:51:44.000000 geoseeq-0.2.0/LICENSE
+-rw-r--r--   0 dcdanko    (501) staff       (20)      341 2023-06-06 16:56:51.495378 geoseeq-0.2.0/PKG-INFO
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1112 2023-02-10 02:57:33.000000 geoseeq-0.2.0/README.md
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2023-06-06 16:56:51.489267 geoseeq-0.2.0/geoseeq/
+-rw-r--r--   0 dcdanko    (501) staff       (20)      813 2023-06-06 16:55:01.000000 geoseeq-0.2.0/geoseeq/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     5539 2023-06-06 16:55:01.000000 geoseeq-0.2.0/geoseeq/blob_constructors.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2115 2023-06-06 16:55:01.000000 geoseeq-0.2.0/geoseeq/bulk_creators.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2023-06-06 16:56:51.492210 geoseeq-0.2.0/geoseeq/cli/
+-rw-r--r--   0 dcdanko    (501) staff       (20)       24 2023-01-20 01:26:16.000000 geoseeq-0.2.0/geoseeq/cli/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1393 2023-02-10 03:30:51.000000 geoseeq-0.2.0/geoseeq/cli/add.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      176 2023-01-20 01:26:16.000000 geoseeq-0.2.0/geoseeq/cli/constants.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1997 2023-02-10 03:31:15.000000 geoseeq-0.2.0/geoseeq/cli/copy.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     6686 2023-02-10 03:31:24.000000 geoseeq-0.2.0/geoseeq/cli/create.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      919 2023-02-10 03:31:43.000000 geoseeq-0.2.0/geoseeq/cli/delete.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4192 2023-06-06 16:55:01.000000 geoseeq-0.2.0/geoseeq/cli/download.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3083 2023-01-20 01:26:16.000000 geoseeq-0.2.0/geoseeq/cli/fastq_utils.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1712 2023-06-06 16:55:01.000000 geoseeq-0.2.0/geoseeq/cli/list.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      975 2023-06-06 16:55:36.000000 geoseeq-0.2.0/geoseeq/cli/main.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)    10120 2023-02-24 17:33:38.000000 geoseeq-0.2.0/geoseeq/cli/upload.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      925 2023-02-10 03:32:14.000000 geoseeq-0.2.0/geoseeq/cli/user.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2564 2023-02-24 16:14:04.000000 geoseeq-0.2.0/geoseeq/cli/utils.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      645 2023-02-14 22:10:03.000000 geoseeq-0.2.0/geoseeq/cli/view.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)       26 2023-01-20 01:26:16.000000 geoseeq-0.2.0/geoseeq/constants.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2023-06-06 16:56:51.492407 geoseeq-0.2.0/geoseeq/contrib/
+-rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-01-20 01:26:16.000000 geoseeq-0.2.0/geoseeq/contrib/__init__.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2023-06-06 16:56:51.493459 geoseeq-0.2.0/geoseeq/contrib/ncbi/
+-rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-01-20 01:26:16.000000 geoseeq-0.2.0/geoseeq/contrib/ncbi/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1056 2023-02-09 21:51:44.000000 geoseeq-0.2.0/geoseeq/contrib/ncbi/api.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4341 2023-02-09 21:51:44.000000 geoseeq-0.2.0/geoseeq/contrib/ncbi/bioproject.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2400 2023-02-10 03:00:45.000000 geoseeq-0.2.0/geoseeq/contrib/ncbi/cli.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      175 2023-01-20 01:26:16.000000 geoseeq-0.2.0/geoseeq/contrib/ncbi/setup_logging.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3405 2023-01-20 01:26:16.000000 geoseeq-0.2.0/geoseeq/file_system_cache.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     5987 2023-04-05 15:01:11.000000 geoseeq-0.2.0/geoseeq/knex.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2462 2023-06-06 16:55:01.000000 geoseeq-0.2.0/geoseeq/organization.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     6555 2023-06-06 16:54:47.000000 geoseeq-0.2.0/geoseeq/pipeline.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     8578 2023-06-06 16:55:01.000000 geoseeq-0.2.0/geoseeq/project.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     6458 2023-06-06 16:54:47.000000 geoseeq-0.2.0/geoseeq/remote_object.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)    24710 2023-06-06 16:55:01.000000 geoseeq-0.2.0/geoseeq/result.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4553 2023-06-06 16:55:01.000000 geoseeq-0.2.0/geoseeq/sample.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      690 2023-01-20 01:26:16.000000 geoseeq-0.2.0/geoseeq/user.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2387 2023-06-06 16:54:47.000000 geoseeq-0.2.0/geoseeq/utils.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2023-06-06 16:56:51.494735 geoseeq-0.2.0/geoseeq/vc/
+-rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-02-10 03:25:58.000000 geoseeq-0.2.0/geoseeq/vc/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      710 2023-02-10 03:23:35.000000 geoseeq-0.2.0/geoseeq/vc/checksum.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2853 2023-02-10 03:33:48.000000 geoseeq-0.2.0/geoseeq/vc/cli.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2486 2023-01-20 01:26:16.000000 geoseeq-0.2.0/geoseeq/vc/clone.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)       19 2023-01-20 01:26:16.000000 geoseeq-0.2.0/geoseeq/vc/constants.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      730 2023-01-20 01:26:16.000000 geoseeq-0.2.0/geoseeq/vc/vc_cache.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      457 2023-01-20 01:26:16.000000 geoseeq-0.2.0/geoseeq/vc/vc_dir.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3900 2023-02-10 03:23:23.000000 geoseeq-0.2.0/geoseeq/vc/vc_sample.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3160 2023-02-10 03:23:17.000000 geoseeq-0.2.0/geoseeq/vc/vc_stub.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     8071 2023-06-06 16:55:01.000000 geoseeq-0.2.0/geoseeq/work_orders.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2023-06-06 16:56:51.490126 geoseeq-0.2.0/geoseeq.egg-info/
+-rw-r--r--   0 dcdanko    (501) staff       (20)      341 2023-06-06 16:56:51.000000 geoseeq-0.2.0/geoseeq.egg-info/PKG-INFO
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1312 2023-06-06 16:56:51.000000 geoseeq-0.2.0/geoseeq.egg-info/SOURCES.txt
+-rw-r--r--   0 dcdanko    (501) staff       (20)        1 2023-06-06 16:56:51.000000 geoseeq-0.2.0/geoseeq.egg-info/dependency_links.txt
+-rw-r--r--   0 dcdanko    (501) staff       (20)       45 2023-06-06 16:56:51.000000 geoseeq-0.2.0/geoseeq.egg-info/entry_points.txt
+-rw-r--r--   0 dcdanko    (501) staff       (20)       32 2023-06-06 16:56:51.000000 geoseeq-0.2.0/geoseeq.egg-info/requires.txt
+-rw-r--r--   0 dcdanko    (501) staff       (20)       14 2023-06-06 16:56:51.000000 geoseeq-0.2.0/geoseeq.egg-info/top_level.txt
+-rw-r--r--   0 dcdanko    (501) staff       (20)       86 2023-02-10 03:38:06.000000 geoseeq-0.2.0/pyproject.toml
+-rw-r--r--   0 dcdanko    (501) staff       (20)       38 2023-06-06 16:56:51.495571 geoseeq-0.2.0/setup.cfg
+-rw-r--r--   0 dcdanko    (501) staff       (20)      783 2023-06-06 16:55:29.000000 geoseeq-0.2.0/setup.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2023-06-06 16:56:51.495163 geoseeq-0.2.0/tests/
+-rw-r--r--   0 dcdanko    (501) staff       (20)        0 2022-11-14 20:29:34.000000 geoseeq-0.2.0/tests/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)    14444 2023-01-20 01:26:16.000000 geoseeq-0.2.0/tests/test_api_client.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      498 2023-01-20 01:26:16.000000 geoseeq-0.2.0/tests/test_work_orders.py
```

### Comparing `geoseeq-0.1.9/LICENSE` & `geoseeq-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geoseeq-0.1.9/README.md` & `geoseeq-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `geoseeq-0.1.9/geoseeq/__init__.py` & `geoseeq-0.2.0/geoseeq/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,31 @@
-
-from .analysis_result import (
+from .result import (
+    SampleResultFolder,
+    SampleResultFile,
+    ProjectResultFolder,
+    ProjectResultFile,
     SampleAnalysisResult,
     SampleAnalysisResultField,
     SampleGroupAnalysisResult,
     SampleGroupAnalysisResultField,
 )
 from .knex import (
     GeoseeqForbiddenError,
     GeoseeqGeneralError,
     GeoseeqInternalError,
     GeoseeqNotFoundError,
-    GeoseeqTimeoutError,
     GeoseeqOtherError,
+    GeoseeqTimeoutError,
     Knex,
 )
 from .organization import Organization
-from .pipeline import Pipeline, PipelineModule
+from .pipeline import Pipeline, PipelineModule, PipelineRun
 from .remote_object import RemoteObjectError, RemoteObjectOverwriteError
 from .sample import Sample
-from .sample_group import SampleGroup
+from .project import Project, SampleGroup
 from .user import User
 from .work_orders import (
     GroupWorkOrder,
     GroupWorkOrderProto,
     JobOrder,
     WorkOrder,
     WorkOrderProto,
```

### Comparing `geoseeq-0.1.9/geoseeq/analysis_result.py` & `geoseeq-0.2.0/geoseeq/result.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,42 @@
 import json
 import logging
 import os
 import time
 from os.path import basename, getsize, join
 from pathlib import Path
 from tempfile import NamedTemporaryFile
-from urllib.request import urlretrieve
+import urllib.request
 
 import requests
 
 from .constants import FIVE_MB
 from .remote_object import RemoteObject, RemoteObjectError
-from .utils import md5_checksum
+from .utils import md5_checksum, download_ftp
 
 logger = logging.getLogger("geoseeq_api")  # Same name as calling module
 logger.addHandler(logging.NullHandler())  # No output unless configured by calling program
 
 
+def _download_head(url, filename, head=None):
+    if head and head > 0:
+        opener = urllib.request.build_opener()
+        if head:
+            opener.addheaders = [('Range', f'bytes=0-{head}')]
+        urllib.request.install_opener(opener)
+    try:
+        urllib.request.urlretrieve(url, filename)  # can throw 416 error if head is too large
+    except urllib.error.HTTPError as e:
+        if e.code == 416:
+            logger.warning(f"HEAD request failed, trying again without HEAD.")
+            _download_head(url, filename, head=None)
+        else:
+            raise e
+    
+
 def diff_dicts(blob1, blob2):
     for problem in _diff_dicts("original", "$", blob1, blob2):
         yield problem
     for problem in _diff_dicts("serialized", "$", blob2, blob1):
         yield problem
 
 
@@ -70,38 +86,36 @@
     else:
         issues = [("MISMATCHED_VALUES:values_only:0", blob, json_serialized)]
     issues = [str(el) for el in issues]
     issues = "\n".join(issues)
     raise RemoteObjectError(f"JSON Serialization modifies object\nIssues:\n{issues}")
 
 
-class AnalysisResult(RemoteObject):
+class ResultFolder(RemoteObject):
     remote_fields = [
         "uuid",
         "created_at",
         "updated_at",
         "module_name",
         "replicate",
-        "metadata",
         "description",
         "is_private",
-        "pipeline_module",
     ]
 
-    def _get(self):
+    def _get(self, allow_overwrite=False):
         """Fetch the result from the server."""
         self.parent.idem()
         logger.debug(f"Getting AnalysisResult.")
         blob = self.get_cached_blob()
         if not blob:
             url = self.nested_url()
             if self.replicate:
                 url += f"?replicate={self.replicate}"
             blob = self.knex.get(url, url_options=self.inherited_url_options)
-            self.load_blob(blob)
+            self.load_blob(blob, allow_overwrite=allow_overwrite)
             self.cache_blob(blob)
         else:
             self.load_blob(blob)
 
     def pre_hash(self):
         key = self.module_name + self.parent.pre_hash()
         key += self.replicate if self.replicate else ""
@@ -113,16 +127,18 @@
         )
         for field in self.get_fields():
             field.copy(copied, save=save)
         if save:
             copied.idem()
         return copied
 
+AnalysisResult = ResultFolder # for backwards compatibility
 
-class SampleAnalysisResult(AnalysisResult):
+
+class SampleResultFolder(ResultFolder):
     parent_field = "sample"
 
     def __init__(self, knex, sample, module_name, replicate=None, metadata={}, is_private=False):
         super().__init__(self)
         self.knex = knex
         self.sample = sample
         self.parent = self.sample
@@ -161,20 +177,28 @@
         d = {"data": data, "sample_ar": self}
         logger.debug(f"Creating SampleAnalysisResult. {d}")
         blob = self.knex.post(
             f"sample_ars?format=json", json=data, url_options=self.inherited_url_options
         )
         self.load_blob(blob)
 
-    def field(self, field_name, data={}):
-        d = {"data": data, "field_name": field_name, "sample_ar": self}
+    def result_file(self, field_name, pipeline_run=None, data={}):
+        d = {
+            "data": data,
+            "field_name": field_name,
+            "pipeline_run": pipeline_run,
+            "sample_ar": self,
+        }
         logger.debug(f"Creating SampleAnalysisResultField for SampleAnalysisResult. {d}")
-        return SampleAnalysisResultField(self.knex, self, field_name, data=data)
+        return SampleResultFile(self.knex, self, field_name, pipeline_run=None, data=data)
+
+    def field(self, *args, **kwargs):
+        return self.result_file(*args, **kwargs)
 
-    def get_fields(self, cache=True):
+    def get_result_files(self, cache=True):
         """Return a list of ar-fields fetched from the server."""
         if cache and self._get_field_cache:
             for field in self._get_field_cache:
                 yield field
             return
         url = f"sample_ar_fields?analysis_result_id={self.uuid}"
         # url = self.nested_url() + f"/fields"
@@ -191,19 +215,24 @@
                 self._get_field_cache.append(result)
             else:
                 yield result
         if cache:
             for field in self._get_field_cache:
                 yield field
 
+    def get_fields(self, *args, **kwargs):
+        return self.get_result_files(*args, **kwargs)
+
     def __str__(self):
-        return f"<Geoseeq::SampleResult {self.module_name} {self.replicate} {self.uuid} />"
+        return f"<Geoseeq::SampleResultFolder {self.module_name} {self.replicate} {self.uuid} />"
+
+SampleAnalysisResult = SampleResultFolder # for backwards compatibility
 
 
-class SampleGroupAnalysisResult(AnalysisResult):
+class ProjectResultFolder(ResultFolder):
     parent_field = "grp"
 
     def __init__(self, knex, grp, module_name, replicate=None, metadata={}, is_private=False):
         super().__init__(self)
         self.knex = knex
         self.grp = grp
         self.parent = self.grp
@@ -225,53 +254,68 @@
         self.grp.idem()
         data = {
             "sample_group": self.grp.uuid,
             "module_name": self.module_name,
         }
         if self.replicate:
             data["replicate"] = self.replicate
+        if self.uuid:
+            data["uuid"] = self.uuid
         blob = self.knex.post(f"sample_group_ars?format=json", json=data)
         self.load_blob(blob)
 
-    def field(self, field_name, data={}):
-        return SampleGroupAnalysisResultField(self.knex, self, field_name, data=data)
+    def result_file(self, field_name, data={}):
+        return ProjectResultFile(self.knex, self, field_name, data=data)
+
+    def field(self, *args, **kwargs):
+        return self.result_file(*args, **kwargs)
 
-    def get_fields(self):
+    def get_result_files(self):
         """Return a list of ar-fields fetched from the server."""
         url = f"sample_group_ar_fields?analysis_result_id={self.uuid}"
         result = self.knex.get(url)
         for result_blob in result["results"]:
             result = self.field(result_blob["name"])
             result.load_blob(result_blob)
             # We just fetched from the server so we change the RemoteObject
             # meta properties to reflect that
             result._already_fetched = True
             result._modified = False
             yield result
 
+    def get_fields(self, *args, **kwargs):
+        return self.get_result_files(*args, **kwargs)
+
     def __str__(self):
-        return f"<Geoseeq::SampleGroupResult {self.module_name} {self.replicate} {self.uuid} />"
+        return f"<Geoseeq::ProjectResultFolder {self.module_name} {self.replicate} {self.uuid} />"
+
+SampleGroupAnalysisResult = ProjectResultFolder # for backwards compatibility
 
 
-class AnalysisResultField(RemoteObject):
+class ResultFile(RemoteObject):
     remote_fields = [
         "uuid",
         "created_at",
         "updated_at",
         "name",
         "stored_data",
+        "pipeline_run",
+    ]
+    optional_remote_fields = [
+        "pipeline_run",
     ]
     parent_field = "parent"
 
-    def __init__(self, knex, parent, field_name, data={}):
+    def __init__(self, knex, parent, field_name, pipeline_run=None, data={}):
         super().__init__(self)
         self.knex = knex
         self.parent = parent
         self.name = field_name
         self.stored_data = data
+        self.pipeline_run = pipeline_run
         self._cached_filename = None  # Used if the field points to S3, FTP, etc
         self._temp_filename = False
 
     @property
     def brn(self):
         obj_type = "sample" if self.canon_url() == "sample_ar_fields" else "project"
         brn = f"brn:{self.knex.instance_code()}:{obj_type}_result_field:{self.uuid}"
@@ -317,26 +361,27 @@
 
     def _save(self):
         data = {field: getattr(self, field) for field in self.remote_fields if hasattr(self, field)}
         data["analysis_result"] = self.parent.uuid
         url = f"{self.canon_url()}/{self.uuid}"
         self.knex.put(url, json=data)
 
-    def _get(self):
+    def _get(self, allow_overwrite=False):
         """Fetch the result from the server."""
         self.parent.idem()
         blob = self.knex.get(self.nested_url())
-        self.load_blob(blob)
+        self.load_blob(blob, allow_overwrite=allow_overwrite)
 
     def get_post_data(self):
         """Return a dict that can be used to POST this field to the server."""
         data = {
             "analysis_result": self.parent.uuid,
             "name": self.name,
             "stored_data": self.stored_data,
+            "pipeline_run": self.pipeline_run,
         }
         return data
 
     def link_file(self, link_type, *args, **kwargs):
         if link_type == "s3":
             return self.link_s3(*args, **kwargs)
         elif link_type == "ftp":
@@ -423,59 +468,75 @@
             if url.startswith("s3://"):
                 url = self.stored_data["endpoint_url"] + "/" + url[5:]
             return url
         elif blob_type == "sra":
             url = self.stored_data["url"]
             return url
 
-    def download_file(self, filename=None, cache=True):
+    def download_file(self, filename=None, cache=True, head=None):
         """Return a local filepath to the file this result points to."""
+        if not filename:
+            self._temp_filename = True
+            myfile = NamedTemporaryFile(delete=False)
+            myfile.close()
+            filename = myfile.name
         blob_type = self.stored_data.get("__type__", "").lower()
-        if blob_type not in ["s3", "sra", "ftp"]:
-            raise TypeError("Cannot fetch a file for a BLOB type result field.")
         if cache and self._cached_filename:
             return self._cached_filename
         if blob_type == "s3":
-            return self._download_s3(filename, cache)
+            return self._download_s3(filename, cache, head=head)
         elif blob_type == "sra":
             return self._download_sra(filename, cache)
         elif blob_type == "ftp":
             return self._download_ftp(filename, cache)
+        elif blob_type == "azure":
+            return self._download_azure(filename, cache, head=head)
+        else:
+            raise TypeError("Cannot fetch a file for a BLOB type result field.")
 
-    def _download_s3(self, filename, cache):
+    def _download_s3(self, filename, cache, head=None):
+        logger.info(f"Downloading S3 file to {filename}")
         try:
             url = self.stored_data["presigned_url"]
         except KeyError:
-            url = self.stored_data["uri"]
+            key = 'uri' if 'uri' in self.stored_data else 'url'
+            url = self.stored_data[key]
         if url.startswith("s3://"):
             url = self.stored_data["endpoint_url"] + "/" + url[5:]
-        if not filename:
-            self._temp_filename = True
-            myfile = NamedTemporaryFile(delete=False)
-            myfile.close()
-            filename = myfile.name
-        urlretrieve(url, filename)
+        _download_head(url, filename, head=head) 
+        if cache:
+            self._cached_filename = filename
+        return filename
+
+    def _download_azure(self, filename, cache, head=None):
+        logger.info(f"Downloading Azure file to {filename}")
+        try:
+            url = self.stored_data["presigned_url"]
+        except KeyError:
+            key = 'uri' if 'uri' in self.stored_data else 'url'
+            url = self.stored_data[key]
+        _download_head(url, filename, head=head)
         if cache:
             self._cached_filename = filename
         return filename
 
     def _download_sra(self, filename, cache):
         return self._download_generic_url(filename, cache)
 
-    def _download_ftp(self, filename, cache):
-        return self._download_generic_url(filename, cache)
+    def _download_ftp(self, filename, cache, head=None):
+        logger.info(f"Downloading FTP file to {filename}")
+        key = 'url' if 'url' in self.stored_data else 'uri'
+        download_ftp(self.stored_data[key], filename, head=head)
+        return filename
 
     def _download_generic_url(self, filename, cache):
-        url = self.stored_data["url"]
-        if not filename:
-            self._temp_filename = True
-            myfile = NamedTemporaryFile(delete=False)
-            myfile.close()
-            filename = myfile.name
-        urlretrieve(url, filename)
+        logger.info(f"Downloading generic URL file to {filename}")
+        key = 'url' if 'url' in self.stored_data else 'uri'
+        url = self.stored_data[key]
+        urllib.request.urlretrieve(url, filename)
         if cache:
             self._cached_filename = filename
         return filename
 
     # DEV: to simplify the uplaod process we will use only the multipart upload. It works well for small files also.
     # This function is currently unused.
     def upload_small_file(self, filepath, optional_fields={}):
@@ -556,14 +617,15 @@
                         attempts += 1
                         if attempts == max_retries:
                             raise
                         time.sleep(10**attempts)  # exponential backoff, (10 ** 2)s default max
                 complete_parts.append(
                     {"ETag": http_response.headers["ETag"], "PartNumber": num + 1}
                 )
+
                 logger.info(f'Uploaded part {num + 1} of {len(urls)} for "{filepath}"')
         response = self.knex.post(
             f"/ar_fields/{self.uuid}/complete_upload",
             json={
                 "parts": complete_parts,
                 "upload_id": upload_id,
                 "result_type": "sample" if is_sample_result else "group",
@@ -595,22 +657,27 @@
     def checksum(self):
         """Return a checksum for this field as a blob.
 
         TODO
         """
         return {"value": "", "method": "none"}
 
+AnalysisResultField = ResultFile
 
-class SampleAnalysisResultField(AnalysisResultField):
+class SampleResultFile(ResultFile):
     def canon_url(self):
         return "sample_ar_fields"
 
     def __str__(self):
-        return f"<Geoseeq::SampleResultField {self.name} {self.uuid} />"
+        return f"<Geoseeq::SampleResultFile {self.name} {self.uuid} />"
 
+SampleAnalysisResultField = SampleResultFile
 
-class SampleGroupAnalysisResultField(AnalysisResultField):
+
+class ProjectResultFile(ResultFile):
     def canon_url(self):
         return "sample_group_ar_fields"
 
     def __str__(self):
-        return f"<Geoseeq::SampleGroupResultField {self.name} {self.uuid} />"
+        return f"<Geoseeq::ProjectResultFile {self.name} {self.uuid} />"
+
+SampleGroupAnalysisResultField = ProjectResultFile
```

### Comparing `geoseeq-0.1.9/geoseeq/bulk_creators.py` & `geoseeq-0.2.0/geoseeq/bulk_creators.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 
 from .blob_constructors import (
     sample_from_blob,
-    sample_result_from_blob,
-    sample_ar_field_from_blob,
+    sample_result_folder_from_blob,
+    sample_result_file_from_blob,
 )
+import json
 
 
 def bulk_create_samples(knex, samples):
     """Create multiple samples at once. Returns a list of created samples.
     
     Only returns samples which were newly created.
     If a sample already exists on the server, it will not be returned.
     """
-    result = knex.post(
-        "bulk_samples",
-        json={"samples": [sample.get_post_data() for sample in samples]},
-    )
+    data = {"samples": [sample.get_post_data() for sample in samples]}
+    # print(json.dumps(data, indent=4))
+    result = knex.post("bulk_samples", json=data)
     created_samples = [
-        sample_from_blob(knex, result_blob) for result_blob in result if result_blob
+        sample_from_blob(knex, result_blob) for result_blob in result['samples'] if result_blob
     ]
     return created_samples
 
 
-def bulk_create_sample_results(knex, sample_results):
+def bulk_create_sample_result_folders(knex, sample_results):
     """Create multiple sample results at once. Returns a list of created sample results.
     
     Only returns sample results which were newly created.
     If a sample result already exists on the server, it will not be returned.
     """
+    data = {"sample_results": [sample_result.get_post_data() for sample_result in sample_results]}
     result = knex.post(
         "bulk_sample_results",
-        json={"sample_results": [sample_result.get_post_data() for sample_result in sample_results]},
+        json=data,
     )
-    created_sample_results = [
-        sample_result_from_blob(knex, result_blob) for result_blob in result if result_blob
+    created_sample_result_folders = [
+        sample_result_folder_from_blob(knex, result_blob) for result_blob in result['sample_results'] if result_blob
     ]
-    return created_sample_results
+    return created_sample_result_folders
 
 
-def bulk_create_sample_result_fields(knex, sample_result_fields):
+def bulk_create_sample_result_files(knex, sample_result_fields):
     """Create multiple sample result fields at once. Returns a list of created sample result fields.
     
     Only returns sample result fields which were newly created.
     If a sample result field already exists on the server, it will not be returned.    
     """
     result = knex.post(
         "bulk_sample_result_fields",
         json={"sample_result_fields": [sample_result_field.get_post_data() for sample_result_field in sample_result_fields]},
     )
-    created_sample_result_fields = [
-        sample_ar_field_from_blob(knex, result_blob) for result_blob in result if result_blob
+    created_sample_result_files = [
+        sample_result_file_from_blob(knex, result_blob) for result_blob in result['sample_result_fields'] if result_blob
     ]
-    return created_sample_result_fields
+    return created_sample_result_files
```

### Comparing `geoseeq-0.1.9/geoseeq/cli/add.py` & `geoseeq-0.2.0/geoseeq/cli/add.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.1.9/geoseeq/cli/copy.py` & `geoseeq-0.2.0/geoseeq/cli/copy.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.1.9/geoseeq/cli/create.py` & `geoseeq-0.2.0/geoseeq/cli/create.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.1.9/geoseeq/cli/delete.py` & `geoseeq-0.2.0/geoseeq/cli/delete.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.1.9/geoseeq/cli/download.py` & `geoseeq-0.2.0/geoseeq/cli/download.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,48 +43,52 @@
     metadata = pd.DataFrame.from_dict(metadata, orient="index")
     metadata.to_csv(state.outfile)
     click.echo("Metadata successfully downloaded for samples.", err=True)
 
 
 @cli_download.command("sample-results")
 @use_common_state
-@click.option("--module-name")
-@click.option("--field-name")
+@click.option("--folder-name", multiple=True, help='Name of folder on GeoSeeq to download from')
+@click.option("--file-name", help="Name of file on GeoSeeq to download from")
 @click.option("--target-dir", default=".")
 @click.option(
     "--sample-manifest",
     default=None,
     type=click.File("r"),
     help="List of sample names to download from",
 )
 @click.option("--download/--urls-only", default=True, help="Download files or just print urls")
 @click.argument("org_name")
 @click.argument("grp_name")
 @click.argument("sample_names", nargs=-1)
 def cli_download_sample_results(
     state,
-    module_name,
-    field_name,
+    folder_name,
+    file_name,
     target_dir,
     sample_manifest,
     download,
     org_name,
     grp_name,
     sample_names,
 ):
     """Download Sample Analysis Results for a set of samples."""
     grp, sample_names = _setup_download(state, sample_manifest, org_name, grp_name, sample_names)
-    for sample in grp.get_samples(cache=False):
-        if sample_names and sample.name not in sample_names:
-            continue
-        for ar in sample.get_analysis_results(cache=False):
-            if module_name and ar.module_name != module_name:
-                continue
+    if sample_names:
+        samples = [grp.sample(name).get() for name in sample_names]
+    else:
+        samples = grp.get_samples(cache=False)
+    for sample in samples:
+        if folder_name:
+            result_folders = [sample.result_folder(name).get() for name in folder_name]
+        else:
+            result_folders = sample.get_result_folders()
+        for ar in result_folders:
             for field in ar.get_fields(cache=False):
-                if field_name and field.name != field_name:
+                if file_name and field.name != file_name:
                     continue
                 if not download:  # download urls to a file, not actual files.
                     try:
                         print(
                             field.get_download_url(),
                             field.get_referenced_filename(),
                             file=state.outfile,
```

### Comparing `geoseeq-0.1.9/geoseeq/cli/fastq_utils.py` & `geoseeq-0.2.0/geoseeq/cli/fastq_utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.1.9/geoseeq/cli/main.py` & `geoseeq-0.2.0/geoseeq/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 def main():
     pass
 
 
 @main.command()
 def version():
     """Print the version of the Geoseeq API being used."""
-    click.echo('0.1.9')  # remember to update setup
+    click.echo('0.2.0')  # remember to update setup
 
 
 
 main.add_command(cli_add)
 main.add_command(cli_create)
 main.add_command(cli_download)
 main.add_command(cli_list)
```

### Comparing `geoseeq-0.1.9/geoseeq/cli/upload.py` & `geoseeq-0.2.0/geoseeq/cli/upload.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.1.9/geoseeq/cli/user.py` & `geoseeq-0.2.0/geoseeq/cli/user.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.1.9/geoseeq/cli/utils.py` & `geoseeq-0.2.0/geoseeq/cli/utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.1.9/geoseeq/cli/view.py` & `geoseeq-0.2.0/geoseeq/cli/view.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.1.9/geoseeq/contrib/ncbi/api.py` & `geoseeq-0.2.0/geoseeq/contrib/ncbi/api.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.1.9/geoseeq/contrib/ncbi/bioproject.py` & `geoseeq-0.2.0/geoseeq/contrib/ncbi/bioproject.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.1.9/geoseeq/contrib/ncbi/cli.py` & `geoseeq-0.2.0/geoseeq/contrib/ncbi/cli.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.1.9/geoseeq/file_system_cache.py` & `geoseeq-0.2.0/geoseeq/file_system_cache.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.1.9/geoseeq/knex.py` & `geoseeq-0.2.0/geoseeq/knex.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,22 +119,22 @@
         self.sess = self._new_session()
 
     def _handle_response(self, response, json_response=True):
         try:
             response.raise_for_status()
         except requests.exceptions.HTTPError as e:
             if response.status_code == 403:
-                raise GeoseeqForbiddenError(e)
+                raise GeoseeqForbiddenError(e, response.content)
             if response.status_code == 404:
-                raise GeoseeqNotFoundError(e)
+                raise GeoseeqNotFoundError(e, response.content)
             if response.status_code == 500:
-                raise GeoseeqInternalError(e)
+                raise GeoseeqInternalError(e, response.content)
             if response.status_code == 504:
-                raise GeoseeqTimeoutError(e)
-            raise GeoseeqOtherError(e)
+                raise GeoseeqTimeoutError(e, response.content)
+            raise GeoseeqOtherError(e, response.content)
         except Exception:
             logger.debug(f"Request failed. {response}\n{response.content}")
             raise
         if json_response:
             return response.json()
         return response
```

### Comparing `geoseeq-0.1.9/geoseeq/organization.py` & `geoseeq-0.2.0/geoseeq/organization.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,79 @@
 
 from .remote_object import RemoteObject
-from .sample_group import SampleGroup
+from .project import Project
 
 
 class Organization(RemoteObject):
     remote_fields = [
         'uuid',
         'created_at',
         'updated_at',
         'name',
     ]
     parent_field = None
+    url_prefix = 'organizations'
 
     def __init__(self, knex, name):
         super().__init__(self)
         self.knex = knex
         self.name = name
 
     def nested_url(self):
         return f'nested/{self.name}'
 
     def _save(self):
         data = {
             field: getattr(self, field)
             for field in self.remote_fields if hasattr(self, field)
         }
-        url = f'organizations/{self.uuid}'
+        url = f'{self.url_prefix}/{self.uuid}'
         self.knex.put(url, json=data)
 
-    def _get(self):
+    def _get(self, allow_overwrite=False):
         """Fetch the result from the server."""
         blob = self.get_cached_blob()
         if not blob:
             blob = self.knex.get(self.nested_url())
-            self.load_blob(blob)
+            self.load_blob(blob, allow_overwrite=allow_overwrite)
             self.cache_blob(blob)
         else:
             self.load_blob(blob)
 
     def _create(self):
-        blob = self.knex.post(f'organizations', json={'name': self.name})
+        blob = self.knex.post(self.url_prefix, json={'name': self.name})
         self.load_blob(blob)
 
-    def sample_group(self, group_name, metadata={}, is_library=True, is_public=False):
-        return SampleGroup(self.knex, self, group_name,
-                           is_library=is_library, is_public=is_public,
-                           metadata=metadata)
+    def sample_group(self, *args, **kwargs):
+        """Create a new project in this organization.
+        
+        This is an alias for project() for backwards compatibility.
+        """
+        return self.project(*args, **kwargs)
+
+    def project(self, project_name, metadata={}, is_public=False):
+        """Create a new project in this organization."""
+        return Project(self.knex, self, project_name, is_public=is_public, metadata=metadata)
 
-    def get_sample_groups(self):
-        """Yield samplegroups fetched from the server."""
+    def get_projects(self):
+        """Yield projects in this org fetched from the server."""
         url = f'sample_groups?organization_id={self.uuid}'
         result = self.knex.get(url)
         for result_blob in result['results']:
             result = self.sample_group(result_blob['name'])
             result.load_blob(result_blob)
             # We just fetched from the server so we change the RemoteObject
             # meta properties to reflect that
             result._already_fetched = True
             result._modified = False
             yield result
 
+    def get_sample_groups(self):
+        """Yield projects in this org fetched from the server.
+
+        This is an alias for get_projects() for backwards compatibility.
+        """
+        return self.get_projects()
+
+
     def pre_hash(self):
         return 'ORG' + self.name
```

### Comparing `geoseeq-0.1.9/geoseeq/pipeline.py` & `geoseeq-0.2.0/geoseeq/sample.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,148 +1,140 @@
-
+from .result import SampleResultFolder
 from .remote_object import RemoteObject
 
 
-class Pipeline(RemoteObject):
+class Sample(RemoteObject):
     remote_fields = [
-        'uuid',
-        'created_at',
-        'updated_at',
-        'name',
-        'description',
-        'long_description',
+        "uuid",
+        "created_at",
+        "updated_at",
+        "name",
+        "metadata",
+        "library",
+        "description",
     ]
-    parent_field = None
+    parent_field = "lib"
+    url_prefix = "samples"
 
-    def __init__(self, knex, name):
+    def __init__(self, knex, lib, name, metadata={}):
         super().__init__(self)
         self.knex = knex
+        self.lib = lib
+        self.new_lib = None
         self.name = name
-        self.description = ''
-        self.long_description = ''
+        self.metadata = metadata
+        self._get_result_cache = []
+
+    @property
+    def brn(self):
+        return f'brn:{self.knex.instance_code()}:sample:{self.uuid}'
+
+    def nested_url(self):
+        return self.lib.nested_url() + f"/samples/{self.name}"
+
+    def change_library(self, new_lib):
+        self.new_lib = new_lib
+        self._modified = True
 
     def _save(self):
-        data = {
-            field: getattr(self, field)
-            for field in self.remote_fields if hasattr(self, field)
-        }
-        url = f'pipelines/{self.uuid}'
-        self.knex.put(url, json=data)
+        data = self.get_post_data()
+        url = f"samples/{self.uuid}"
+        self.knex.put(url, json=data, url_options=self.inherited_url_options)
+        if self.new_lib:
+            self.lib = self.new_lib
+            self.new_lib = None
 
-    def _get(self):
+    def _get(self, allow_overwrite=False):
         """Fetch the result from the server."""
+        self.lib.get()
         blob = self.get_cached_blob()
         if not blob:
-            blob = self.knex.get(f'pipelines/name/{self.name}')
-            self.load_blob(blob)
+            url = self.nested_url()
+            blob = self.knex.get(url, url_options=self.inherited_url_options)
+            self.load_blob(blob, allow_overwrite=allow_overwrite)
             self.cache_blob(blob)
         else:
-            self.load_blob(blob)
+            self.load_blob(blob, allow_overwrite=allow_overwrite)
+
+    def get_post_data(self):
+        data = {field: getattr(self, field) for field in self.remote_fields if hasattr(self, field)}
+        data["library"] = self.lib.uuid
+        if self.new_lib:
+            if isinstance(self.new_lib, RemoteObject):
+                data["library"] = self.new_lib.uuid
+            else:
+                data["library"] = self.new_lib
+        if data['uuid'] is None:
+            data.pop('uuid')
+        return data
 
     def _create(self):
-        data = {
-            'name': self.name,
-            'description': self.description,
-            'long_description': self.long_description,
-        }
-        url = 'pipelines?format=json'
-        blob = self.knex.post(url, json=data)
+        assert self.lib.is_library
+        self.lib.idem()
+        data = self.get_post_data()
+        url = f"samples"
+        blob = self.knex.post(url, json=data, url_options=self.inherited_url_options)
         self.load_blob(blob)
 
-    def __str__(self):
-        return f'<Geoseeq::Pipeline {self.name} {self.uuid} />'
-
-    def __repr__(self):
-        return f'<Geoseeq::Pipeline {self.name} {self.uuid} />'
-
-    def pre_hash(self):
-        return 'PIPELINE' + self.name
-
-    def module(self, name, version, metadata={}):
-        return PipelineModule(
-            self.knex,
-            self,
-            name,
-            version,
-            metadata=metadata,
+    def delete(self):
+        url = f"samples/{self.uuid}"
+        self.knex.delete(url)
+        self._already_fetched = False
+        self._deleted = True
+
+    def result_folder(self, module_name, replicate=None, metadata=None):
+        """Return a SampleResultFolder for this sample."""
+        return SampleResultFolder(
+            self.knex, self, module_name, replicate=replicate, metadata=metadata
         )
 
-    def get_modules(self):
-        url = f'pipeline_modules?pipeline={self.uuid}'
+    def analysis_result(self, *args, **kwargs):
+        """Return a SampleResultFolder for this sample.
+        
+        This is an alias for result_folder."""
+        return self.result_folder(*args, **kwargs)
+
+    def get_analysis_results(self, cache=True):
+        """Yield sample analysis results fetched from the server."""
+        self.get()
+        if cache and self._get_result_cache:
+            for ar in self._get_result_cache:
+                yield ar
+            return
+        url =  f"sample_ars?sample_id={self.uuid}"
         result = self.knex.get(url)
-        for result_blob in result['results']:
-            result = self.module(result_blob['name'], result_blob['version'])
+        for result_blob in result["results"]:
+            result = self.analysis_result(result_blob["module_name"])
             result.load_blob(result_blob)
             # We just fetched from the server so we change the RemoteObject
             # meta properties to reflect that
             result._already_fetched = True
             result._modified = False
-            yield result
-
-
-class PipelineModule(RemoteObject):
-    remote_fields = [
-        'uuid',
-        'created_at',
-        'updated_at',
-        'name',
-        'version',
-        'metadata',
-        'description',
-        'long_description',
-        'dependencies',
-    ]
-    parent_field = 'pip'
-
-    def __init__(self, knex, pipeline, name, version, metadata={}):
-        super().__init__(self)
-        self.knex = knex
-        self.pip = pipeline
-        self.name = name
-        self.version = version
-        self.metadata = metadata
-        self.description = ''
-        self.long_description = ''
-        self.dependencies = []
-
-    def _save(self):
-        data = {
-            field: getattr(self, field)
-            for field in self.remote_fields if hasattr(self, field)
-        }
-        url = f'pipeline_modules/{self.uuid}'
-        self.knex.put(url, json=data)
-
-    def _get(self):
-        """Fetch the result from the server."""
-        blob = self.get_cached_blob()
-        if not blob:
-            blob = self.knex.get(f'pipelines/{self.pip.uuid}/modules/{self.name}/{self.version}')
-            self.load_blob(blob)
-            self.cache_blob(blob)
-        else:
-            self.load_blob(blob)
-
-    def _create(self):
-        data = {
-            'pipeline': self.pip.uuid,
-            'name': self.name,
-            'version': self.version,
-            'metadata': self.metadata,
-            'description': self.description,
-            'long_description': self.long_description,
-        }
-        url = 'pipeline_modules?format=json'
-        blob = self.knex.post(url, json=data)
-        self.load_blob(blob)
-
-    def add_dependency(self, upstream):
-        self.dependencies.append(upstream.uuid)
+            if cache:
+                self._get_result_cache.append(result)
+            else:
+                yield result
+        if cache:
+            for ar in self._get_result_cache:
+                yield ar
+
+    def get_manifest(self):
+        """Return a manifest for this sample."""
+        url = f"samples/{self.uuid}/manifest"
+        return self.knex.get(url)
 
     def __str__(self):
-        return f'<Geoseeq::PipelineModule "{self.name}" "{self.version}" {self.uuid} />'
+        return f"<Geoseeq::Sample {self.name} {self.uuid} />"
 
     def __repr__(self):
-        return f'<Geoseeq::PipelineModule "{self.name}" "{self.version}" {self.uuid} />'
+        return f"<Geoseeq::Sample {self.name} {self.uuid} />"
 
     def pre_hash(self):
-        return 'PIPELINE_MODULE' + self.name + self.version + self.pip.pre_hash()
+        return "SAMPLE" + self.name + self.lib.pre_hash()
+
+    def copy(self, sample_group, save=True):
+        copied = sample_group.sample(self.name, self.metadata)
+        for ar in self.get_analysis_results():
+            ar.copy(copied, save=save)
+        if save:
+            copied.idem()
+        return copied
```

### Comparing `geoseeq-0.1.9/geoseeq/remote_object.py` & `geoseeq-0.2.0/geoseeq/remote_object.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     def get_cached_blob(self):
         return self.cache.get_cached_blob(self)
 
     def cache_blob(self, blob):
         return self.cache.cache_blob(self, blob)
 
-    def load_blob(self, blob):
+    def load_blob(self, blob, allow_overwrite=False):
         logger.debug(f"Loading blob. {blob}")
         if self._deleted:
             logger.error(f"Cannot load blob, RemoteObject has been deleted. {self}")
             raise RemoteObjectError("This object has been deleted.")
         for field in self.remote_fields:
             current = getattr(self, field, None)
             try:
@@ -67,15 +67,15 @@
                 if field not in self.optional_remote_fields:
                     logger.error(f"Blob being loaded is missing key. {field}")
                     raise KeyError(
                         f"Key {field} is missing for object {self} (type {type(self)})\
                              in blob: {blob}"
                     )
                 new = None
-            if current and current != new:
+            if not allow_overwrite and current and current != new:
                 is_overwrite = True
                 if isinstance(current, dict) and isinstance(new, dict):
                     append_only = True
                     for k, v in current.items():
                         if (k not in new) or (new[k] != v):
                             append_only = False
                         break
@@ -88,29 +88,29 @@
                             f'Loading blob would overwrite field "{field}":\n\t'
                             f'current: "{current}" (type: "{type(current)}")\n\t'
                             f'new:     "{new}" (type: "{type(new)}")'
                         )
                     )
             setattr(self, field, new)
 
-    def exists(self):
+    def exists(self, allow_overwrite=False):
         try:
-            self.get()
+            self.get(allow_overwrite=allow_overwrite)
             return True
         except HTTPError:
             return False
 
-    def get(self):
+    def get(self, allow_overwrite=False):
         """Fetch the object from the server."""
         if self._deleted:
             logger.error(f"Cannot GET blob, RemoteObject has been deleted. {self}")
             raise RemoteObjectError("This object has been deleted.")
         if not self._already_fetched:
             logger.debug(f"Fetching RemoteBlob. {self}")
-            self._get()
+            self._get(allow_overwrite=allow_overwrite)
             self._already_fetched = True
             self._modified = False
         else:
             logger.debug(f"RemoteObject has already been fetched. {self}")
         return self
 
     def create(self):
@@ -160,7 +160,16 @@
         return self
 
     def delete(self):
         logger.debug(f"Deleting RemoteBlob. {self}")
         self.knex.delete(self.nested_url())
         self._already_fetched = False
         self._deleted = True
+
+    @classmethod
+    def all_uuids(self, knex):
+        """Return a list of all objects of this type."""
+        results = knex.get(self.url_prefix)['results']
+        return [result['uuid'] for result in results]
+
+
+
```

### Comparing `geoseeq-0.1.9/geoseeq/sample_group.py` & `geoseeq-0.2.0/geoseeq/project.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,139 +1,175 @@
-from .analysis_result import SampleGroupAnalysisResult
+from .result import ProjectResultFolder
 from .remote_object import RemoteObject
 from .sample import Sample
 from .utils import paginated_iterator
+import json
 
 
-class SampleGroup(RemoteObject):
+
+class Project(RemoteObject):
     remote_fields = [
         "uuid",
         "created_at",
         "updated_at",
         "name",
         "is_library",
         "is_public",
+        "privacy_level",
         "metadata",
         "long_description",
         "description",
         "bucket",
         "storage_provider_name",
     ]
+    optional_remote_fields = [
+        "privacy_level",
+    ]
     parent_field = "org"
+    url_prefix = "sample_groups"
 
     def __init__(
         self,
         knex,
         org,
         name,
         metadata={},
         is_library=True,
         is_public=False,
         storage_provider="default",
+        privacy_level=None,
     ):
         super().__init__(self)
         self.knex = knex
         self.org = org
+        self.new_org = None
         self.name = name
         self.is_library = is_library
         self.is_public = is_public
         self._sample_cache = []
         self._deleted_sample_cache = []
         self._get_sample_cache = []
         self._get_result_cache = []
         self.metadata = metadata
         self.storage_provider = storage_provider
+        self.privacy_level = privacy_level
+
+    def change_org(self, org):
+        self.new_org = org
+        self._modified = True
+
+    def get_post_data(self):
+        data = {field: getattr(self, field) for field in self.remote_fields if hasattr(self, field)}
+        data["organization"] = self.org.uuid
+        data['description'] = self.description if hasattr(self, 'description') and self.description else self.name
+        data['privacy_level'] = self.privacy_level if hasattr(self, 'privacy_level') and self.privacy_level else 'private'
+        data['storage_provider_name'] = self.storage_provider
+        if self.new_org:
+            if isinstance(self.new_org, RemoteObject):
+                data["organization"] = self.new_org.uuid
+            else:
+                data["organization"] = self.new_org
+        if data["uuid"] is None:
+            data.pop("uuid")
+        return data
 
     def nested_url(self):
         return self.org.nested_url() + f"/sample_groups/{self.name}"
 
     def _save_group_obj(self):
-        data = {field: getattr(self, field) for field in self.remote_fields if hasattr(self, field)}
-        data["organization"] = self.org.uuid
-        data["description"] = self.description if self.description else self.name
+        data = self.get_post_data()
         url = f"sample_groups/{self.uuid}"
         self.knex.put(url, json=data)
 
     def _save_sample_list(self):
         sample_uuids = []
-        for sample in self._sample_cache:
-            sample.idem()
-            sample_uuids.append(sample.uuid)
+        for sample_uuid in self._sample_cache:
+            sample_uuids.append(sample_uuid)
         if sample_uuids:
             url = f"sample_groups/{self.uuid}/samples"
             self.knex.post(url, json={"sample_uuids": sample_uuids})
         self._sample_cache = []
 
     def _delete_sample_list(self):
         sample_uuids = []
-        for sample in self._deleted_sample_cache:
-            sample.idem()
-            sample_uuids.append(sample.uuid)
+        for sample_uuid in self._deleted_sample_cache:
+            sample_uuids.append(sample_uuid)
         if sample_uuids:
             url = f"sample_groups/{self.uuid}/samples"
             self.knex.delete(url, json={"sample_uuids": sample_uuids})
         self._deleted_sample_cache = []
 
     def _save(self):
         self._save_group_obj()
         self._save_sample_list()
         self._delete_sample_list()
 
-    def _get(self):
+    def _get(self, allow_overwrite=False):
         """Fetch the result from the server."""
         self.org.idem()
         blob = self.get_cached_blob()
         if not blob:
             blob = self.knex.get(self.nested_url())
-            self.load_blob(blob)
+            self.load_blob(blob, allow_overwrite=allow_overwrite)
             self.cache_blob(blob)
         else:
             self.load_blob(blob)
 
     def _create(self):
         self.org.idem()
+        post_data = self.get_post_data()
         blob = self.knex.post(
             f"sample_groups?format=json",
-            json={
-                "organization": self.org.uuid,
-                "name": self.name,
-                "is_library": self.is_library,
-                "is_public": self.is_public,
-                "metadata": self.metadata,
-                "storage_provider_name": self.storage_provider,
-            },
+            json=post_data,
         )
         self.load_blob(blob)
+    
+    def add_sample_uuids(self, sample_uuids):
+        """Return this group and add a sample to this group.
+
+        Do not contact server until `.save()` is called on this group.
+        """
+        for sample_uuid in sample_uuids:
+            self._sample_cache.append(sample_uuid)
+        self._modified = True
+        return self
 
     def add_sample(self, sample):
         """Return this group and add a sample to this group.
 
         Do not contact server until `.save()` is called on this group.
         """
-        self._sample_cache.append(sample)
+        self._sample_cache.append(sample.uuid)
         self._modified = True
         return self
 
     def remove_sample(self, sample):
         """Return this group and remove a sample to this group.
 
         Do not contact server until `.save()` is called on this group.
         """
-        self._deleted_sample_cache.append(sample)
+        self._deleted_sample_cache.append(sample.uuid)
         self._modified = True
         return self
 
     def sample(self, sample_name, metadata={}):
         return Sample(self.knex, self, sample_name, metadata=metadata)
 
-    def analysis_result(self, module_name, replicate=None, metadata={}):
-        return SampleGroupAnalysisResult(
+    def result_folder(self, module_name, replicate=None, metadata={}):
+        """Return a ProjectResultFolder object for this project."""
+        return ProjectResultFolder(
             self.knex, self, module_name, replicate=replicate, metadata=metadata
         )
 
+    def analysis_result(self, *args, **kwargs):
+        """Return a ProjectResultFolder object for this project.
+        
+        Alias for result_folder."""
+        return self.result_folder(*args, **kwargs)
+
     def get_samples(self, cache=True, error_handler=None):
         """Yield samples fetched from the server."""
         if cache and self._get_sample_cache:
             for sample in self._get_sample_cache:
                 yield sample
             return
         url = f"sample_groups/{self.uuid}/samples"
@@ -149,14 +185,24 @@
                 self._get_sample_cache.append(sample)
             else:
                 yield sample
         if cache:
             for sample in self._get_sample_cache:
                 yield sample
 
+    def get_sample_uuids(self, cache=True, error_handler=None):
+        """Yield samples uuids fetched from the server."""
+        if cache and self._get_sample_cache:
+            for sample in self._get_sample_cache:
+                yield sample.uuid
+            return
+        url = f"sample_groups/{self.uuid}/samples"
+        for sample_blob in paginated_iterator(self.knex, url, error_handler=error_handler):
+            yield sample_blob['uuid']
+
     def get_analysis_results(self, cache=True):
         """Yield group analysis results fetched from the server."""
         if cache and self._get_result_cache:
             for ar in self._get_result_cache:
                 yield ar
             return
         url = f"sample_group_ars?sample_group_id={self.uuid}"
@@ -182,15 +228,23 @@
         return self.knex.get(url)
 
     def get_module_counts(self):
         """Return a dictionary with module counts for samples in this group."""
         url = f"sample_groups/{self.uuid}/module_counts"
         return self.knex.get(url)
 
+    def get_sample_metadata(self):
+        """Return a pandas dataframe with sample metadata."""
+        url = f"sample_groups/{self.uuid}/metadata"
+        blob = self.knex.get(url)
+        return pd.DataFrame.from_dict(blob["metadata"], orient="index")
+
     def __str__(self):
-        return f"<Geoseeq::SampleGroup {self.name} {self.uuid} />"
+        return f"<Geoseeq::Project {self.name} {self.uuid} />"
 
     def __repr__(self):
-        return f"<Geoseeq::SampleGroup {self.name} {self.uuid} />"
+        return f"<Geoseeq::Project {self.name} {self.uuid} />"
 
     def pre_hash(self):
-        return "SG" + self.name + self.org.pre_hash()
+        return "PROJ" + self.name + self.org.pre_hash()
+
+SampleGroup = Project  # alias for backwards compatibility
```

### Comparing `geoseeq-0.1.9/geoseeq/user.py` & `geoseeq-0.2.0/geoseeq/user.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.1.9/geoseeq/vc/checksum.py` & `geoseeq-0.2.0/geoseeq/vc/checksum.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.1.9/geoseeq/vc/cli.py` & `geoseeq-0.2.0/geoseeq/vc/cli.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.1.9/geoseeq/vc/clone.py` & `geoseeq-0.2.0/geoseeq/vc/clone.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.1.9/geoseeq/vc/vc_cache.py` & `geoseeq-0.2.0/geoseeq/vc/vc_cache.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.1.9/geoseeq/vc/vc_sample.py` & `geoseeq-0.2.0/geoseeq/vc/vc_sample.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.1.9/geoseeq/vc/vc_stub.py` & `geoseeq-0.2.0/geoseeq/vc/vc_stub.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.1.9/geoseeq/work_orders.py` & `geoseeq-0.2.0/geoseeq/work_orders.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-from .blob_constructors import sample_from_uuid, sample_group_from_uuid
+from .blob_constructors import sample_from_uuid, project_from_uuid
 from .remote_object import RemoteObject
 
 
 class WorkOrderProto(RemoteObject):
     remote_fields = [
         'uuid',
         'created_at',
```

### Comparing `geoseeq-0.1.9/geoseeq.egg-info/SOURCES.txt` & `geoseeq-0.2.0/geoseeq.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 geoseeq/__init__.py
-geoseeq/analysis_result.py
 geoseeq/blob_constructors.py
 geoseeq/bulk_creators.py
 geoseeq/constants.py
 geoseeq/file_system_cache.py
 geoseeq/knex.py
 geoseeq/organization.py
 geoseeq/pipeline.py
+geoseeq/project.py
 geoseeq/remote_object.py
+geoseeq/result.py
 geoseeq/sample.py
-geoseeq/sample_group.py
 geoseeq/user.py
 geoseeq/utils.py
 geoseeq/work_orders.py
 geoseeq.egg-info/PKG-INFO
 geoseeq.egg-info/SOURCES.txt
 geoseeq.egg-info/dependency_links.txt
 geoseeq.egg-info/entry_points.txt
```

### Comparing `geoseeq-0.1.9/setup.py` & `geoseeq-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import setuptools
 
 setuptools.setup(
     name='geoseeq',
-    version='0.1.9',  # remember to update version string in CLI as well
+    version='0.2.0',  # remember to update version string in CLI as well
     author="David C. Danko",
     author_email='dcdanko@biotia.io',
     description=open('README.md').read(),
     packages=setuptools.find_packages(),
     package_dir={'geoseeq': 'geoseeq'},
     install_requires=[
         'requests',
```

### Comparing `geoseeq-0.1.9/tests/test_api_client.py` & `geoseeq-0.2.0/tests/test_api_client.py`

 * *Files identical despite different names*

