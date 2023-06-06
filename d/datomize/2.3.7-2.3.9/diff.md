# Comparing `tmp/datomize-2.3.7.tar.gz` & `tmp/datomize-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datomize-2.3.7.tar", last modified: Mon Jun  5 08:54:13 2023, max compression
+gzip compressed data, was "dist/datomize-2.3.9.tar", last modified: Tue Jun  6 21:06:02 2023, max compression
```

## Comparing `datomize-2.3.7.tar` & `datomize-2.3.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:54:13.000000 datomize-2.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-06-05 08:54:13.000000 datomize-2.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-06-05 08:52:02.000000 datomize-2.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:54:13.000000 datomize-2.3.7/datomize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-06-05 08:54:13.000000 datomize-2.3.7/datomize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-05 08:54:13.000000 datomize-2.3.7/datomize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 08:54:13.000000 datomize-2.3.7/datomize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-05 08:54:13.000000 datomize-2.3.7/datomize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 08:54:13.000000 datomize-2.3.7/datomize.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/datoenhancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/datogenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/datomapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/datomizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/datotrainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/datotuner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/helpers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/helpers/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/helpers/authentication/authentication_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/helpers/autodiscovery/
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/helpers/autodiscovery/autodiscovery_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/helpers/business_unit_project/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/helpers/business_unit_project/business_unit_project_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/helpers/common_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/helpers/datasource/
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/helpers/datasource/datasource_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/helpers/generator/
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/helpers/generator/generator_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/helpers/train/
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/helpers/train/datatuner_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/helpers/train/enhance_ml_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/helpers/train/train_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/helpers/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/helpers/wrapper/evaluation_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/helpers/wrapper/schema_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/protos/
--rw-r--r--   0 runner    (1001) docker     (123)    37487 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/protos/autodiscoveryservice_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/protos/constantsservice_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/protos/datakubeservice_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/protos/datasourceconfigservice_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20073 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/protos/datatunerservice_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/protos/enhancemlresults_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/protos/fieldsettingsservice_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/protos/infrastructuresettings_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12101 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/protos/privacyevaluationservice_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    21243 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/protos/synthschemavalidationresult_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/utils/enhance_ml.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/utils/general.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/utils/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/utils/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/utils/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/utils/step_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/utils/thresholds.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 08:54:13.000000 datomize-2.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-05 08:54:13.000000 datomize-2.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:06:02.000000 datomize-2.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-06-06 21:06:02.000000 datomize-2.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-06-06 21:04:16.000000 datomize-2.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:06:02.000000 datomize-2.3.9/datomize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-06-06 21:06:01.000000 datomize-2.3.9/datomize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-06 21:06:02.000000 datomize-2.3.9/datomize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 21:06:01.000000 datomize-2.3.9/datomize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-06 21:06:01.000000 datomize-2.3.9/datomize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-06 21:06:01.000000 datomize-2.3.9/datomize.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:06:02.000000 datomize-2.3.9/datomizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-06 21:04:16.000000 datomize-2.3.9/datomizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-06-06 21:04:16.000000 datomize-2.3.9/datomizer/datoenhancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-06-06 21:04:16.000000 datomize-2.3.9/datomizer/datogenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-06 21:04:16.000000 datomize-2.3.9/datomizer/datomapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-06-06 21:04:16.000000 datomize-2.3.9/datomizer/datomizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-06-06 21:04:16.000000 datomize-2.3.9/datomizer/datotrainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-06-06 21:04:16.000000 datomize-2.3.9/datomizer/datotuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:06:02.000000 datomize-2.3.9/datomizer/helpers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:06:02.000000 datomize-2.3.9/datomizer/helpers/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-06 21:04:16.000000 datomize-2.3.9/datomizer/helpers/authentication/authentication_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:06:02.000000 datomize-2.3.9/datomizer/helpers/autodiscovery/
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-06-06 21:04:16.000000 datomize-2.3.9/datomizer/helpers/autodiscovery/autodiscovery_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:06:02.000000 datomize-2.3.9/datomizer/helpers/business_unit_project/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-06 21:04:16.000000 datomize-2.3.9/datomizer/helpers/business_unit_project/business_unit_project_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-06-06 21:04:16.000000 datomize-2.3.9/datomizer/helpers/common_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:06:02.000000 datomize-2.3.9/datomizer/helpers/datasource/
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-06-06 21:04:16.000000 datomize-2.3.9/datomizer/helpers/datasource/datasource_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:06:02.000000 datomize-2.3.9/datomizer/helpers/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-06 21:04:16.000000 datomize-2.3.9/datomizer/helpers/generator/generator_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:06:02.000000 datomize-2.3.9/datomizer/helpers/train/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-06 21:04:16.000000 datomize-2.3.9/datomizer/helpers/train/datatuner_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-06 21:04:16.000000 datomize-2.3.9/datomizer/helpers/train/enhance_ml_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-06 21:04:16.000000 datomize-2.3.9/datomizer/helpers/train/train_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:06:02.000000 datomize-2.3.9/datomizer/helpers/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-06 21:04:16.000000 datomize-2.3.9/datomizer/helpers/wrapper/evaluation_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-06 21:04:16.000000 datomize-2.3.9/datomizer/helpers/wrapper/schema_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:06:02.000000 datomize-2.3.9/datomizer/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)    37487 2023-06-06 21:06:01.000000 datomize-2.3.9/datomizer/protos/autodiscoveryservice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-06 21:06:01.000000 datomize-2.3.9/datomizer/protos/constantsservice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-06-06 21:06:01.000000 datomize-2.3.9/datomizer/protos/datakubeservice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-06-06 21:06:01.000000 datomize-2.3.9/datomizer/protos/datasourceconfigservice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20073 2023-06-06 21:06:01.000000 datomize-2.3.9/datomizer/protos/datatunerservice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-06-06 21:06:01.000000 datomize-2.3.9/datomizer/protos/enhancemlresults_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-06-06 21:06:01.000000 datomize-2.3.9/datomizer/protos/fieldsettingsservice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-06 21:06:01.000000 datomize-2.3.9/datomizer/protos/infrastructuresettings_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12101 2023-06-06 21:06:01.000000 datomize-2.3.9/datomizer/protos/privacyevaluationservice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21243 2023-06-06 21:06:01.000000 datomize-2.3.9/datomizer/protos/synthschemavalidationresult_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:06:02.000000 datomize-2.3.9/datomizer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-06-06 21:04:16.000000 datomize-2.3.9/datomizer/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-06 21:04:16.000000 datomize-2.3.9/datomizer/utils/enhance_ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-06 21:04:16.000000 datomize-2.3.9/datomizer/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-06 21:04:16.000000 datomize-2.3.9/datomizer/utils/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-06 21:04:16.000000 datomize-2.3.9/datomizer/utils/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-06 21:04:16.000000 datomize-2.3.9/datomizer/utils/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-06 21:04:16.000000 datomize-2.3.9/datomizer/utils/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-06 21:04:16.000000 datomize-2.3.9/datomizer/utils/step_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-06 21:04:16.000000 datomize-2.3.9/datomizer/utils/thresholds.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 21:06:02.000000 datomize-2.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-06 21:06:01.000000 datomize-2.3.9/setup.py
```

### Comparing `datomize-2.3.7/PKG-INFO` & `datomize-2.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datomize
-Version: 2.3.7
+Version: 2.3.9
 Summary: Datomize python client
 Home-page: https://datomize.github.io/datomizeSDK
 Author: Datomize Ltd.
 Author-email: support@datomize.com
 License: Apache Software License (https://www.apache.org/licenses/LICENSE-2.0)
 Project-URL: Documentation, https://datomize.github.io/datomizeSDK
 Description: Welcome to Datomize Python SDK
```

### Comparing `datomize-2.3.7/README.md` & `datomize-2.3.9/README.md`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/datomize.egg-info/PKG-INFO` & `datomize-2.3.9/datomize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datomize
-Version: 2.3.7
+Version: 2.3.9
 Summary: Datomize python client
 Home-page: https://datomize.github.io/datomizeSDK
 Author: Datomize Ltd.
 Author-email: support@datomize.com
 License: Apache Software License (https://www.apache.org/licenses/LICENSE-2.0)
 Project-URL: Documentation, https://datomize.github.io/datomizeSDK
 Description: Welcome to Datomize Python SDK
```

### Comparing `datomize-2.3.7/datomize.egg-info/SOURCES.txt` & `datomize-2.3.9/datomize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/datomizer/datoenhancer.py` & `datomize-2.3.9/datomizer/datoenhancer.py`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/datomizer/datogenerator.py` & `datomize-2.3.9/datomizer/datogenerator.py`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/datomizer/datomapper.py` & `datomize-2.3.9/datomizer/datomapper.py`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/datomizer/datomizer.py` & `datomize-2.3.9/datomizer/datomizer.py`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/datomizer/datotrainer.py` & `datomize-2.3.9/datomizer/datotrainer.py`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/datomizer/datotuner.py` & `datomize-2.3.9/datomizer/datotuner.py`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/datomizer/helpers/authentication/authentication_helper.py` & `datomize-2.3.9/datomizer/helpers/authentication/authentication_helper.py`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/datomizer/helpers/autodiscovery/autodiscovery_helper.py` & `datomize-2.3.9/datomizer/helpers/autodiscovery/autodiscovery_helper.py`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/datomizer/helpers/business_unit_project/business_unit_project_helper.py` & `datomize-2.3.9/datomizer/helpers/business_unit_project/business_unit_project_helper.py`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/datomizer/helpers/common_helper.py` & `datomize-2.3.9/datomizer/helpers/common_helper.py`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/datomizer/helpers/datasource/datasource_helper.py` & `datomize-2.3.9/datomizer/helpers/datasource/datasource_helper.py`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/datomizer/helpers/generator/generator_helper.py` & `datomize-2.3.9/datomizer/helpers/generator/generator_helper.py`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/datomizer/helpers/train/datatuner_helper.py` & `datomize-2.3.9/datomizer/helpers/train/datatuner_helper.py`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/datomizer/helpers/train/enhance_ml_helper.py` & `datomize-2.3.9/datomizer/helpers/train/enhance_ml_helper.py`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/datomizer/helpers/train/train_helper.py` & `datomize-2.3.9/datomizer/helpers/train/train_helper.py`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/datomizer/helpers/wrapper/schema_wrapper.py` & `datomize-2.3.9/datomizer/helpers/wrapper/schema_wrapper.py`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/datomizer/protos/autodiscoveryservice_pb2.py` & `datomize-2.3.9/datomizer/protos/autodiscoveryservice_pb2.py`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/datomizer/protos/constantsservice_pb2.py` & `datomize-2.3.9/datomizer/protos/constantsservice_pb2.py`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/datomizer/protos/datakubeservice_pb2.py` & `datomize-2.3.9/datomizer/protos/datakubeservice_pb2.py`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/datomizer/protos/datasourceconfigservice_pb2.py` & `datomize-2.3.9/datomizer/protos/datasourceconfigservice_pb2.py`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/datomizer/protos/datatunerservice_pb2.py` & `datomize-2.3.9/datomizer/protos/datatunerservice_pb2.py`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/datomizer/protos/enhancemlresults_pb2.py` & `datomize-2.3.9/datomizer/protos/enhancemlresults_pb2.py`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/datomizer/protos/fieldsettingsservice_pb2.py` & `datomize-2.3.9/datomizer/protos/fieldsettingsservice_pb2.py`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/datomizer/protos/infrastructuresettings_pb2.py` & `datomize-2.3.9/datomizer/protos/infrastructuresettings_pb2.py`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/datomizer/protos/privacyevaluationservice_pb2.py` & `datomize-2.3.9/datomizer/protos/privacyevaluationservice_pb2.py`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/datomizer/protos/synthschemavalidationresult_pb2.py` & `datomize-2.3.9/datomizer/protos/synthschemavalidationresult_pb2.py`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/datomizer/utils/constants.py` & `datomize-2.3.9/datomizer/utils/constants.py`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/datomizer/utils/enhance_ml.py` & `datomize-2.3.9/datomizer/utils/enhance_ml.py`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/datomizer/utils/general.py` & `datomize-2.3.9/datomizer/utils/general.py`

 * *Files identical despite different names*

### Comparing `datomize-2.3.7/setup.py` & `datomize-2.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name="datomize",
-    version="2.3.7",
+    version="2.3.9",
     license='Apache Software License (https://www.apache.org/licenses/LICENSE-2.0)',
     description="Datomize python client",
     packages=find_namespace_packages(),
     install_requires=[
         'requests', 'protobuf==3.19.4'
     ],
     url="https://datomize.github.io/datomizeSDK",
```

