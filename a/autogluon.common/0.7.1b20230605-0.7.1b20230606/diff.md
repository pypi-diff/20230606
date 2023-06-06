# Comparing `tmp/autogluon.common-0.7.1b20230605.tar.gz` & `tmp/autogluon.common-0.7.1b20230606.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.common-0.7.1b20230605.tar", last modified: Mon Jun  5 09:04:02 2023, max compression
+gzip compressed data, was "autogluon.common-0.7.1b20230606.tar", last modified: Tue Jun  6 09:03:42 2023, max compression
```

## Comparing `autogluon.common-0.7.1b20230605.tar` & `autogluon.common-0.7.1b20230606.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:02.571964 autogluon.common-0.7.1b20230605/
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    12537 2023-06-05 09:04:02.571964 autogluon.common-0.7.1b20230605/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 09:04:02.571964 autogluon.common-0.7.1b20230605/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:02.567964 autogluon.common-0.7.1b20230605/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:02.567964 autogluon.common-0.7.1b20230605/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:02.567964 autogluon.common-0.7.1b20230605/src/autogluon/common/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:02.567964 autogluon.common-0.7.1b20230605/src/autogluon/common/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22684 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/features/feature_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/features/infer_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/features/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:02.571964 autogluon.common-0.7.1b20230605/src/autogluon/common/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/loaders/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/loaders/load_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/loaders/load_pd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/loaders/load_pkl.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/loaders/load_pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/loaders/load_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/loaders/load_str.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/loaders/load_zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:02.571964 autogluon.common-0.7.1b20230605/src/autogluon/common/model_filter/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/model_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/model_filter/_model_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:02.571964 autogluon.common-0.7.1b20230605/src/autogluon/common/savers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/savers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/savers/save_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/savers/save_pd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/savers/save_pkl.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/savers/save_pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/savers/save_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:02.571964 autogluon.common-0.7.1b20230605/src/autogluon/common/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/utils/compression_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/utils/deprecated_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/utils/distribute_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/utils/lite.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/utils/multiprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/utils/nvutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/utils/pandas_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/utils/resource_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16670 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/utils/s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/utils/try_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-06-05 09:03:52.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-05 09:04:02.000000 autogluon.common-0.7.1b20230605/src/autogluon/common/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:02.567964 autogluon.common-0.7.1b20230605/src/autogluon.common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12537 2023-06-05 09:04:02.000000 autogluon.common-0.7.1b20230605/src/autogluon.common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-05 09:04:02.000000 autogluon.common-0.7.1b20230605/src/autogluon.common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 09:04:02.000000 autogluon.common-0.7.1b20230605/src/autogluon.common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 09:04:02.000000 autogluon.common-0.7.1b20230605/src/autogluon.common.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-05 09:04:02.000000 autogluon.common-0.7.1b20230605/src/autogluon.common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 09:04:02.000000 autogluon.common-0.7.1b20230605/src/autogluon.common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 09:04:02.000000 autogluon.common-0.7.1b20230605/src/autogluon.common.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:42.192690 autogluon.common-0.7.1b20230606/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    12537 2023-06-06 09:03:42.192690 autogluon.common-0.7.1b20230606/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 09:03:42.192690 autogluon.common-0.7.1b20230606/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:42.184690 autogluon.common-0.7.1b20230606/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:42.184690 autogluon.common-0.7.1b20230606/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:42.184690 autogluon.common-0.7.1b20230606/src/autogluon/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:42.188690 autogluon.common-0.7.1b20230606/src/autogluon/common/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22684 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/features/feature_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/features/infer_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/features/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:42.188690 autogluon.common-0.7.1b20230606/src/autogluon/common/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/loaders/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/loaders/load_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/loaders/load_pd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/loaders/load_pkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/loaders/load_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/loaders/load_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/loaders/load_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/loaders/load_zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:42.188690 autogluon.common-0.7.1b20230606/src/autogluon/common/model_filter/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/model_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/model_filter/_model_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:42.188690 autogluon.common-0.7.1b20230606/src/autogluon/common/savers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/savers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/savers/save_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/savers/save_pd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/savers/save_pkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/savers/save_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/savers/save_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:42.192690 autogluon.common-0.7.1b20230606/src/autogluon/common/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/utils/compression_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/utils/deprecated_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/utils/distribute_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/utils/lite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/utils/multiprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/utils/nvutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/utils/pandas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/utils/path_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/utils/resource_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16670 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/utils/s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/utils/try_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-06-06 09:03:26.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-06 09:03:41.000000 autogluon.common-0.7.1b20230606/src/autogluon/common/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:42.184690 autogluon.common-0.7.1b20230606/src/autogluon.common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12537 2023-06-06 09:03:41.000000 autogluon.common-0.7.1b20230606/src/autogluon.common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-06 09:03:42.000000 autogluon.common-0.7.1b20230606/src/autogluon.common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 09:03:41.000000 autogluon.common-0.7.1b20230606/src/autogluon.common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-06 09:03:41.000000 autogluon.common-0.7.1b20230606/src/autogluon.common.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-06 09:03:41.000000 autogluon.common-0.7.1b20230606/src/autogluon.common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-06 09:03:41.000000 autogluon.common-0.7.1b20230606/src/autogluon.common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 09:03:41.000000 autogluon.common-0.7.1b20230606/src/autogluon.common.egg-info/zip-safe
```

### Comparing `autogluon.common-0.7.1b20230605/LICENSE` & `autogluon.common-0.7.1b20230606/LICENSE`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230605/PKG-INFO` & `autogluon.common-0.7.1b20230606/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.common
-Version: 0.7.1b20230605
+Version: 0.7.1b20230606
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.common-0.7.1b20230605/setup.py` & `autogluon.common-0.7.1b20230606/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230605/src/autogluon/common/features/feature_metadata.py` & `autogluon.common-0.7.1b20230606/src/autogluon/common/features/feature_metadata.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230605/src/autogluon/common/features/infer_types.py` & `autogluon.common-0.7.1b20230606/src/autogluon/common/features/infer_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230605/src/autogluon/common/features/types.py` & `autogluon.common-0.7.1b20230606/src/autogluon/common/features/types.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230605/src/autogluon/common/loaders/_utils.py` & `autogluon.common-0.7.1b20230606/src/autogluon/common/loaders/_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230605/src/autogluon/common/loaders/load_pd.py` & `autogluon.common-0.7.1b20230606/src/autogluon/common/loaders/load_pd.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230605/src/autogluon/common/loaders/load_pkl.py` & `autogluon.common-0.7.1b20230606/src/autogluon/common/loaders/load_pkl.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230605/src/autogluon/common/loaders/load_pointer.py` & `autogluon.common-0.7.1b20230606/src/autogluon/common/loaders/load_pointer.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230605/src/autogluon/common/loaders/load_s3.py` & `autogluon.common-0.7.1b20230606/src/autogluon/common/loaders/load_s3.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230605/src/autogluon/common/loaders/load_str.py` & `autogluon.common-0.7.1b20230606/src/autogluon/common/loaders/load_str.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230605/src/autogluon/common/loaders/load_zip.py` & `autogluon.common-0.7.1b20230606/src/autogluon/common/loaders/load_zip.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230605/src/autogluon/common/model_filter/_model_filter.py` & `autogluon.common-0.7.1b20230606/src/autogluon/common/model_filter/_model_filter.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230605/src/autogluon/common/savers/save_json.py` & `autogluon.common-0.7.1b20230606/src/autogluon/common/savers/save_json.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230605/src/autogluon/common/savers/save_pd.py` & `autogluon.common-0.7.1b20230606/src/autogluon/common/savers/save_pd.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230605/src/autogluon/common/savers/save_pkl.py` & `autogluon.common-0.7.1b20230606/src/autogluon/common/savers/save_pkl.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230605/src/autogluon/common/savers/save_str.py` & `autogluon.common-0.7.1b20230606/src/autogluon/common/savers/save_str.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230605/src/autogluon/common/space.py` & `autogluon.common-0.7.1b20230606/src/autogluon/common/space.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230605/src/autogluon/common/utils/compression_utils.py` & `autogluon.common-0.7.1b20230606/src/autogluon/common/utils/compression_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230605/src/autogluon/common/utils/deprecated_utils.py` & `autogluon.common-0.7.1b20230606/src/autogluon/common/utils/deprecated_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230605/src/autogluon/common/utils/distribute_utils.py` & `autogluon.common-0.7.1b20230606/src/autogluon/common/utils/distribute_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230605/src/autogluon/common/utils/file_utils.py` & `autogluon.common-0.7.1b20230606/src/autogluon/common/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230605/src/autogluon/common/utils/log_utils.py` & `autogluon.common-0.7.1b20230606/src/autogluon/common/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230605/src/autogluon/common/utils/multiprocessing_utils.py` & `autogluon.common-0.7.1b20230606/src/autogluon/common/utils/multiprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230605/src/autogluon/common/utils/nvutil.py` & `autogluon.common-0.7.1b20230606/src/autogluon/common/utils/nvutil.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230605/src/autogluon/common/utils/pandas_utils.py` & `autogluon.common-0.7.1b20230606/src/autogluon/common/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230605/src/autogluon/common/utils/resource_utils.py` & `autogluon.common-0.7.1b20230606/src/autogluon/common/utils/resource_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230605/src/autogluon/common/utils/s3_utils.py` & `autogluon.common-0.7.1b20230606/src/autogluon/common/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230605/src/autogluon/common/utils/try_import.py` & `autogluon.common-0.7.1b20230606/src/autogluon/common/utils/try_import.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230605/src/autogluon/common/utils/utils.py` & `autogluon.common-0.7.1b20230606/src/autogluon/common/utils/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230605/src/autogluon.common.egg-info/PKG-INFO` & `autogluon.common-0.7.1b20230606/src/autogluon.common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.common
-Version: 0.7.1b20230605
+Version: 0.7.1b20230606
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.common-0.7.1b20230605/src/autogluon.common.egg-info/SOURCES.txt` & `autogluon.common-0.7.1b20230606/src/autogluon.common.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -39,11 +39,12 @@
 src/autogluon/common/utils/distribute_utils.py
 src/autogluon/common/utils/file_utils.py
 src/autogluon/common/utils/lite.py
 src/autogluon/common/utils/log_utils.py
 src/autogluon/common/utils/multiprocessing_utils.py
 src/autogluon/common/utils/nvutil.py
 src/autogluon/common/utils/pandas_utils.py
+src/autogluon/common/utils/path_converter.py
 src/autogluon/common/utils/resource_utils.py
 src/autogluon/common/utils/s3_utils.py
 src/autogluon/common/utils/try_import.py
 src/autogluon/common/utils/utils.py
```

