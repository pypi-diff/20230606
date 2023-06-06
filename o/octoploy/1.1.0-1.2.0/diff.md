# Comparing `tmp/octoploy-1.1.0.tar.gz` & `tmp/octoploy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octoploy-1.1.0.tar", last modified: Wed Dec 28 07:45:34 2022, max compression
+gzip compressed data, was "octoploy-1.2.0.tar", last modified: Tue Jun  6 07:49:27 2023, max compression
```

## Comparing `octoploy-1.1.0.tar` & `octoploy-1.2.0.tar`

### file list

```diff
@@ -1,74 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 07:45:34.563372 octoploy-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2022-12-28 07:45:26.000000 octoploy-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13860 2022-12-28 07:45:34.563372 octoploy-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9788 2022-12-28 07:45:26.000000 octoploy-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 07:45:34.559372 octoploy-1.1.0/octoploy/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 07:45:34.559372 octoploy-1.1.0/octoploy/backup/
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/backup/BackupGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/backup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 07:45:34.559372 octoploy-1.1.0/octoploy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/config/AppConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/config/BaseConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     5525 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/config/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/config/ConfigMap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/config/DeploymentActionConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/config/YmlConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 07:45:34.559372 octoploy-1.1.0/octoploy/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/deploy/AppDeploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/deploy/DeploymentBundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/deploy/K8sObjectDeployer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/deploy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 07:45:34.563372 octoploy-1.1.0/octoploy/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/k8s/BaseObj.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/k8s/SecretObj.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/k8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 07:45:34.563372 octoploy-1.1.0/octoploy/oc/
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/oc/Model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/oc/Oc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/oc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6501 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/octoploy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 07:45:34.563372 octoploy-1.1.0/octoploy/processing/
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/processing/DataPreProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/processing/DecryptionProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/processing/OcObjectMerge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/processing/TreeWalker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/processing/ValueLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7337 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/processing/YmlTemplateProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 07:45:34.563372 octoploy-1.1.0/octoploy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/utils/Cert.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/utils/DictUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/utils/Encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/utils/Errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/utils/Log.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/utils/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/utils/Yml.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/utils/YmlWriter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-28 07:45:26.000000 octoploy-1.1.0/octoploy/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 07:45:34.559372 octoploy-1.1.0/octoploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13860 2022-12-28 07:45:34.000000 octoploy-1.1.0/octoploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2022-12-28 07:45:34.000000 octoploy-1.1.0/octoploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-28 07:45:34.000000 octoploy-1.1.0/octoploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2022-12-28 07:45:34.000000 octoploy-1.1.0/octoploy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2022-12-28 07:45:34.000000 octoploy-1.1.0/octoploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-28 07:45:34.000000 octoploy-1.1.0/octoploy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2022-12-28 07:45:34.563372 octoploy-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2022-12-28 07:45:26.000000 octoploy-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 07:45:34.563372 octoploy-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2022-12-28 07:45:26.000000 octoploy-1.1.0/tests/AppDeploymentTest.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2022-12-28 07:45:26.000000 octoploy-1.1.0/tests/DictUtilsTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2022-12-28 07:45:26.000000 octoploy-1.1.0/tests/OcObjectMergeTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2022-12-28 07:45:26.000000 octoploy-1.1.0/tests/YmlTempalteProcessorTest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-28 07:45:26.000000 octoploy-1.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 07:45:34.563372 octoploy-1.1.0/tests/config/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2022-12-28 07:45:26.000000 octoploy-1.1.0/tests/config/AppConfigTest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-28 07:45:26.000000 octoploy-1.1.0/tests/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 07:45:34.563372 octoploy-1.1.0/tests/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2022-12-28 07:45:26.000000 octoploy-1.1.0/tests/processing/ValueLoaderTest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-28 07:45:26.000000 octoploy-1.1.0/tests/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 07:45:34.563372 octoploy-1.1.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2022-12-28 07:45:26.000000 octoploy-1.1.0/tests/utils/EncryptionTest.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2022-12-28 07:45:26.000000 octoploy-1.1.0/tests/utils/YmlWriterTest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-28 07:45:26.000000 octoploy-1.1.0/tests/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:27.558266 octoploy-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-06 07:49:14.000000 octoploy-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-06-06 07:49:27.558266 octoploy-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-06-06 07:49:14.000000 octoploy-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:27.554266 octoploy-1.2.0/octoploy/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:27.554266 octoploy-1.2.0/octoploy/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/api/Model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/api/Oc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:27.554266 octoploy-1.2.0/octoploy/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/backup/BackupGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/backup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:27.554266 octoploy-1.2.0/octoploy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/config/AppConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/config/BaseConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/config/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/config/DeploymentActionConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/config/DynamicConfigMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/config/YmlConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:27.554266 octoploy-1.2.0/octoploy/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/deploy/AppDeploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/deploy/DeploymentBundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/deploy/K8sObjectDeployer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/deploy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:27.554266 octoploy-1.2.0/octoploy/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/k8s/BaseObj.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/k8s/SecretObj.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/octoploy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:27.554266 octoploy-1.2.0/octoploy/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/processing/DataPreProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/processing/DecryptionProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/processing/K8sObjectMerge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/processing/TreeWalker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/processing/ValueLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/processing/YmlTemplateProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:27.558266 octoploy-1.2.0/octoploy/state/
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/state/StateTracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/state/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:27.558266 octoploy-1.2.0/octoploy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/utils/Cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/utils/DictUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/utils/Encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/utils/Errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/utils/Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/utils/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/utils/Yml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/utils/YmlWriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:27.554266 octoploy-1.2.0/octoploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-06-06 07:49:27.000000 octoploy-1.2.0/octoploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-06 07:49:27.000000 octoploy-1.2.0/octoploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 07:49:27.000000 octoploy-1.2.0/octoploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 07:49:27.000000 octoploy-1.2.0/octoploy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-06 07:49:27.000000 octoploy-1.2.0/octoploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-06 07:49:27.000000 octoploy-1.2.0/octoploy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-06 07:49:27.558266 octoploy-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-06 07:49:14.000000 octoploy-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:27.558266 octoploy-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-06 07:49:14.000000 octoploy-1.2.0/tests/AppDeploymentTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-06 07:49:14.000000 octoploy-1.2.0/tests/DictUtilsTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-06 07:49:14.000000 octoploy-1.2.0/tests/OcObjectMergeTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-06-06 07:49:14.000000 octoploy-1.2.0/tests/StateTrackingTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-06 07:49:14.000000 octoploy-1.2.0/tests/TestUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-06-06 07:49:14.000000 octoploy-1.2.0/tests/YmlTempalteProcessorTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:14.000000 octoploy-1.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:27.558266 octoploy-1.2.0/tests/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-06 07:49:14.000000 octoploy-1.2.0/tests/config/AppConfigTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:14.000000 octoploy-1.2.0/tests/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:27.558266 octoploy-1.2.0/tests/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-06 07:49:14.000000 octoploy-1.2.0/tests/processing/ValueLoaderTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:14.000000 octoploy-1.2.0/tests/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:27.558266 octoploy-1.2.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-06 07:49:14.000000 octoploy-1.2.0/tests/utils/EncryptionTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-06 07:49:14.000000 octoploy-1.2.0/tests/utils/YmlWriterTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:14.000000 octoploy-1.2.0/tests/utils/__init__.py
```

### Comparing `octoploy-1.1.0/LICENSE` & `octoploy-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `octoploy-1.1.0/PKG-INFO` & `octoploy-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octoploy
-Version: 1.1.0
+Version: 1.2.0
 Summary: Simple kubernetes / openshift templating engine with templating, libraries, state tracking
 Home-page: https://github.com/davidgiga1993/octoploy
 Author: davidgiga1993
 Author-email: david@dev-core.org
 License: UNKNOWN
 Description: # Kubernetes / openshift templating and deployment engine
         
@@ -80,15 +80,15 @@
         
         ### Root config
         
         Here is a sample `_root.yml` file
         
         ```yml
         # Name of the namespace / openshift project
-        project: 'my-oc-project'
+        namespace: 'my-oc-project'
         
         # K8s context which should be used for deploying
         context: 'my-k8s-cluster-config'
         
         # OPTIONAL STUFF
         # Global variables
         vars:
@@ -291,74 +291,74 @@
         with features. A common example would be a template which adds a monitoring sidecar container. In the `examples` you can
         find the `nsq-template` which defines a sidecar container.
         
         Here is a minimal example:
         
         ```yml
         # examples/nsq-template/dc.yml
-        kind: DeploymentConfig
-        apiVersion: v1
+        kind: Deployment
+        apiVersion: apps/v1
         spec:
           template:
             spec:
-            containers:
-              - name: "nsqd"
-              image: "nsqio/nsq"
+              containers:
+                - name: "nsqd"
+                image: "nsqio/nsq"
         ```
         
         ```yml
         # examples/my-app/dc.yml
-        kind: DeploymentConfig
-        apiVersion: v1
+        kind: Deployment
+        apiVersion: apps/v1
         metadata:
-          name: "${DC_NAME}"
+          name: "${APP_NAME}"
         
         spec:
           replicas: 1
           selector:
-            name: "${DC_NAME}"
+            name: "${APP_NAME}"
           strategy:
-            type: Rolling
+            type: RollingUpdate
         
           template:
             metadata:
               labels:
-                name: "${DC_NAME}"
+                name: "${APP_NAME}"
         
             spec:
               containers:
-                - name: "${DC_NAME}"
+                - name: "${APP_NAME}"
                   image: "docker-registry.default.svc:5000/oc-project/my-app:prod"
         ```
         
         If we now apply the nsq-template to our app using `postApplyTemplates: [nsq-template]` the
         `DeploymentConfig` object gets automatically merged:
         
         ```yml
         # Merged result after applying template
-        kind: DeploymentConfig
-        apiVersion: v1
+        kind: Deployment
+        apiVersion: apps/v1
         metadata:
-          name: "${DC_NAME}"
+          name: "${APP_NAME}"
         
         spec:
           replicas: 1
           selector:
-            name: "${DC_NAME}"
+            name: "${APP_NAME}"
           strategy:
-            type: Rolling
+            type: RollingUpdate
         
           template:
             metadata:
               labels:
-                name: "${DC_NAME}"
+                name: "${APP_NAME}"
         
             spec:
               containers:
-                - name: "${DC_NAME}"
+                - name: "${APP_NAME}"
                   image: "docker-registry.default.svc:5000/oc-project/my-app:prod"
                 # This is the part of the template
                 - name: "nsqd"
                   image: "nsqio/nsq"
         ```
         
         #### Loops
@@ -394,15 +394,15 @@
           - domain
           - dockerDomain
           - imageStreamTag
         ```
         
         ```yml
         # prod/_root.yml
-        project: 'prod-project'
+        namespace: 'prod-project'
         inherit: testLib
         
         # Required parameters
         vars:
           domain: my-prod.dev-core.org
           dockerDomain: prod-docker.com
           imageStreamTag: prod
@@ -420,18 +420,22 @@
         ```
         
         The file will be updated in place.
         
         For deploying encrypted secrets, you'll need to set the environment variable
         `OCTOPLOY_KEY` with your key used to encrypt the data.
         
-        ## Change tracking
+        ## State tracking
+        
+        Octoploy currently uses a ConfigMap called `octoploy-state` to keep track of the object states.
+        
+        The ConfigMap contains  all managed objects and their md5 sum. If this hash has changed the whole object will be
+        applied. If the object does already exist, but is not listed in the state it will simply be added to the state.
         
-        Changes are detected by storing a md5 sum in the label of the object. If this hash has changed the whole object will be
-        applied. If no label has been found in openshift the object is assumed to be equal, and the label is added.
+        You can modify the name of the configmap by setting the `stateName` variable in the `_root.yml` file.
         
         Currently, the actual fields of the yml files are not compared, however this is a planned feature.  
         
         ## Examples
         
         All examples can be found in the `examples` folder.
```

### Comparing `octoploy-1.1.0/README.md` & `octoploy-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 ### Root config
 
 Here is a sample `_root.yml` file
 
 ```yml
 # Name of the namespace / openshift project
-project: 'my-oc-project'
+namespace: 'my-oc-project'
 
 # K8s context which should be used for deploying
 context: 'my-k8s-cluster-config'
 
 # OPTIONAL STUFF
 # Global variables
 vars:
@@ -283,74 +283,74 @@
 with features. A common example would be a template which adds a monitoring sidecar container. In the `examples` you can
 find the `nsq-template` which defines a sidecar container.
 
 Here is a minimal example:
 
 ```yml
 # examples/nsq-template/dc.yml
-kind: DeploymentConfig
-apiVersion: v1
+kind: Deployment
+apiVersion: apps/v1
 spec:
   template:
     spec:
-    containers:
-      - name: "nsqd"
-      image: "nsqio/nsq"
+      containers:
+        - name: "nsqd"
+        image: "nsqio/nsq"
 ```
 
 ```yml
 # examples/my-app/dc.yml
-kind: DeploymentConfig
-apiVersion: v1
+kind: Deployment
+apiVersion: apps/v1
 metadata:
-  name: "${DC_NAME}"
+  name: "${APP_NAME}"
 
 spec:
   replicas: 1
   selector:
-    name: "${DC_NAME}"
+    name: "${APP_NAME}"
   strategy:
-    type: Rolling
+    type: RollingUpdate
 
   template:
     metadata:
       labels:
-        name: "${DC_NAME}"
+        name: "${APP_NAME}"
 
     spec:
       containers:
-        - name: "${DC_NAME}"
+        - name: "${APP_NAME}"
           image: "docker-registry.default.svc:5000/oc-project/my-app:prod"
 ```
 
 If we now apply the nsq-template to our app using `postApplyTemplates: [nsq-template]` the
 `DeploymentConfig` object gets automatically merged:
 
 ```yml
 # Merged result after applying template
-kind: DeploymentConfig
-apiVersion: v1
+kind: Deployment
+apiVersion: apps/v1
 metadata:
-  name: "${DC_NAME}"
+  name: "${APP_NAME}"
 
 spec:
   replicas: 1
   selector:
-    name: "${DC_NAME}"
+    name: "${APP_NAME}"
   strategy:
-    type: Rolling
+    type: RollingUpdate
 
   template:
     metadata:
       labels:
-        name: "${DC_NAME}"
+        name: "${APP_NAME}"
 
     spec:
       containers:
-        - name: "${DC_NAME}"
+        - name: "${APP_NAME}"
           image: "docker-registry.default.svc:5000/oc-project/my-app:prod"
         # This is the part of the template
         - name: "nsqd"
           image: "nsqio/nsq"
 ```
 
 #### Loops
@@ -386,15 +386,15 @@
   - domain
   - dockerDomain
   - imageStreamTag
 ```
 
 ```yml
 # prod/_root.yml
-project: 'prod-project'
+namespace: 'prod-project'
 inherit: testLib
 
 # Required parameters
 vars:
   domain: my-prod.dev-core.org
   dockerDomain: prod-docker.com
   imageStreamTag: prod
@@ -412,18 +412,22 @@
 ```
 
 The file will be updated in place.
 
 For deploying encrypted secrets, you'll need to set the environment variable
 `OCTOPLOY_KEY` with your key used to encrypt the data.
 
-## Change tracking
+## State tracking
+
+Octoploy currently uses a ConfigMap called `octoploy-state` to keep track of the object states.
+
+The ConfigMap contains  all managed objects and their md5 sum. If this hash has changed the whole object will be
+applied. If the object does already exist, but is not listed in the state it will simply be added to the state.
 
-Changes are detected by storing a md5 sum in the label of the object. If this hash has changed the whole object will be
-applied. If no label has been found in openshift the object is assumed to be equal, and the label is added.
+You can modify the name of the configmap by setting the `stateName` variable in the `_root.yml` file.
 
 Currently, the actual fields of the yml files are not compared, however this is a planned feature.  
 
 ## Examples
 
 All examples can be found in the `examples` folder.
```

### Comparing `octoploy-1.1.0/octoploy/backup/BackupGenerator.py` & `octoploy-1.2.0/octoploy/backup/BackupGenerator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 import os
 
-from octoploy.config.Config import ProjectConfig
+from octoploy.config.Config import RootConfig
 from octoploy.utils.Log import Log
 
 
 class BackupGenerator(Log):
     """
     Very crude backup implementation.
     """
 
-    def __init__(self, config: ProjectConfig):
+    def __init__(self, config: RootConfig):
         super().__init__()
         self._config = config
 
     def create_backup(self, dir_name: str):
         if not os.path.exists(dir_name):
             os.mkdir(dir_name)
 
         oc = self._config.create_api()
         namespaces = oc.get_namespaces()
         apis = oc._exec(['api-resources', '--namespaced', '-o', 'name']).splitlines()
         for namespace in namespaces:
             namespace = namespace.split('/')[1]
             self.log.info(f'Backup up namespace {namespace}')
-            oc.set_namespace(namespace)
             for api in apis:
                 try:
-                    names = oc._exec(['get', api, '-o', 'name']).splitlines()
+                    names = oc._exec(['get', api, '-o', 'name'], namespace=namespace).splitlines()
                 except Exception:
                     continue
                 self.log.info(f'Backing up api {api}')
                 for item in names:
-                    output = oc._exec(['get', item, '-o', 'yaml'])
+                    output = oc._exec(['get', item, '-o', 'yaml'], namespace=namespace)
                     file_name = namespace + '_' + item.replace('/', '_') + '.yaml'
                     with open(os.path.join(dir_name, file_name), 'w') as f:
                         f.write(output)
```

### Comparing `octoploy-1.1.0/octoploy/config/AppConfig.py` & `octoploy-1.2.0/octoploy/config/AppConfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from __future__ import annotations
 
 from typing import List, Optional, Dict
 
 from octoploy.config.BaseConfig import BaseConfig
-from octoploy.config.ConfigMap import ConfigMap
+from octoploy.config.DynamicConfigMap import DynamicConfigMap
 from octoploy.config.DeploymentActionConfig import DeploymentActionConfig
 from octoploy.utils.DictUtils import DictUtils
 from octoploy.utils.Errors import MissingVar
 
 
 class AppConfig(BaseConfig):
     """
     Contains the configuration for the deployment of a single app
     """
 
     def __init__(self, config_root: str, path: Optional[str], external_vars: Dict[str, str] = None):
         super().__init__(path, external_vars)
         self._config_root = config_root
 
-    def get_config_maps(self) -> List[ConfigMap]:
+    def get_config_maps(self) -> List[DynamicConfigMap]:
         """
         Returns additional config maps which should contain the content of a file
         """
-        return [ConfigMap(data) for data in self.data.get('configmaps', [])]
+        return [DynamicConfigMap(data) for data in self.data.get('configmaps', [])]
 
     def enabled(self) -> bool:
         """
         True if this app is enabled
         """
         return self.data.get('enabled', True)
 
@@ -50,15 +50,15 @@
         :raise MissingVar: Gets raised if the data inside forEach is not complete
         """
         instances = []
         for instance_vars in self.data.get('forEach', []):
             assert isinstance(instance_vars, dict)
             dc_name = instance_vars.get('APP_NAME')
             if dc_name is None:
-                raise MissingVar('APP_NAME not defined in forEach for app ' + str(self.get_dc_name()))
+                raise MissingVar('APP_NAME not defined in forEach for app ' + str(self.get_name()))
 
             config = AppConfig(self._config_root, None, instance_vars)
             # Inherit all parameters
             config.data.update(self.data)
             # Update the DC_NAME
             DictUtils.set(config.data, 'name', dc_name)
             instances.append(config)
@@ -86,30 +86,30 @@
 
     def get_reload_actions(self) -> List[DeploymentActionConfig]:
         """
         Returns all actions that should be executed after a configuration change of the app
         """
         return [DeploymentActionConfig(self, x) for x in self.data.get('on-config-change', [])]
 
-    def get_dc_name(self) -> Optional[str]:
+    def get_name(self) -> Optional[str]:
         """
         Returns the app name
-        :return: Name
+        :return: Name or None if not defined
         """
         name = DictUtils.get(self.data, 'name')
         if name is not None:
             return name
         return DictUtils.get(self.data, 'dc.name')  # Deprecated
 
     def get_replacements(self) -> Dict[str, str]:
         """
         Returns all variables which are available for the yml files
         :return: Key, value map
         """
         items = super().get_replacements()
-        dc_name = self.get_dc_name()
+        dc_name = self.get_name()
         if dc_name is not None:
             items.update({
                 'APP_NAME': dc_name,
                 'DC_NAME': dc_name  # Deprecated
             })
         return items
```

### Comparing `octoploy-1.1.0/octoploy/config/BaseConfig.py` & `octoploy-1.2.0/octoploy/config/BaseConfig.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -57,17 +57,17 @@
             # Value can be a primitive or object
             if isinstance(value, dict):
                 # Is a object, use a loader to load the value
                 loader_name = value.get('loader')
                 if loader_name is not None:
                     loader = ValueLoaderFactory.create(self, value['loader'])
                     new_values = loader.load(value)
+                    new_items[key] = 'viaLoader'
                     for new_key, new_val in new_values.items():
                         new_items[key + new_key] = new_val
-                    new_items[key] = 'viaLoader'
                     continue
 
         items.update(new_items)
         items.update(self._external_vars)
         return items
 
     def get_params(self) -> List[str]:
```

### Comparing `octoploy-1.1.0/octoploy/config/Config.py` & `octoploy-1.2.0/octoploy/config/Config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
 import os
 from typing import Optional, Dict, List
 
+from octoploy.api.Oc import Oc, K8, K8sApi
 from octoploy.config.AppConfig import AppConfig
 from octoploy.config.BaseConfig import BaseConfig
-from octoploy.oc.Oc import Oc, K8, K8sApi
 from octoploy.processing.DataPreProcessor import DataPreProcessor, OcToK8PreProcessor
 from octoploy.processing.YmlTemplateProcessor import YmlTemplateProcessor
+from octoploy.state.StateTracking import StateTracking
 from octoploy.utils.Errors import ConfigError
 
 
 class RunMode:
     def __init__(self):
         self.out_file = None  # type: Optional[str]
         """
@@ -25,39 +26,55 @@
 
         self.plan = False
         """
         True if changes should be previewed
         """
 
 
-class ProjectConfig(BaseConfig):
+class RootConfig(BaseConfig):
     """
-    Configuration for a project (aka a collection of apps inside a single context/namespace)
+    Root configuration for a project (aka a collection of apps inside a single context/namespace)
     """
 
     def __init__(self, config_root: str, path: str):
         super().__init__(path)
         self._config_root = config_root
         self._oc = None
-        self._library = None  # type: Optional[ProjectConfig]
+        self._library = None  # type: Optional[RootConfig]
 
         inherit = self.data.get('inherit')
         if inherit is not None:
             # Use a library
             parent_dir = os.path.abspath(os.path.join(path, os.pardir, os.pardir))
             lib_dir = os.path.join(parent_dir, inherit)
             if not os.path.isdir(lib_dir):
                 raise FileNotFoundError('Library not found: ' + lib_dir)
-            self._library = ProjectConfig.load(lib_dir)
+            self._library = RootConfig.load(lib_dir)
             if not self._library.is_library():
                 raise ConfigError('Project ' + inherit + ' referenced as library but is not a library')
 
+        state_name = self.data.get('stateName', '')
+        self._state = StateTracking(self.create_api(), state_name)
+
     @classmethod
-    def load(cls, path: str) -> ProjectConfig:
-        return ProjectConfig(path, os.path.join(path, '_root.yml'))
+    def load(cls, path: str) -> RootConfig:
+        return RootConfig(path, os.path.join(path, '_root.yml'))
+
+    def get_state(self) -> StateTracking:
+        return self._state
+
+    def initialize_state(self, run_mode: RunMode):
+        if run_mode.dry_run:
+            return
+        self._state.restore(self.get_namespace_name())
+
+    def persist_state(self, run_mode: RunMode):
+        if run_mode.dry_run or run_mode.plan:
+            return
+        self._state.store(self.get_namespace_name())
 
     def get_config_root(self) -> str:
         return self._config_root
 
     def is_library(self) -> bool:
         """
         Indicates if this collection is a library
@@ -65,33 +82,33 @@
         return self.data.get('type', '') == 'library'
 
     def get_pre_processor(self) -> DataPreProcessor:
         """
         Returns the pre processor for the current config
         """
         mode = self._get_mode()
-        if mode == 'k8':
+        if mode == 'k8s' or mode == 'k8s':
             return OcToK8PreProcessor()
         return DataPreProcessor()
 
     def _get_mode(self) -> str:
-        return self.data.get('mode', 'oc')
+        return self.data.get('mode', 'k8s')
 
     def create_api(self) -> K8sApi:
         """
-        Creates a new openshift / k8 client
+        Creates a new openshift / k8s client
         :return: Client
         """
         if self._oc is not None:
             return self._oc
 
         mode = self._get_mode()
         if mode == 'oc':
             oc = Oc()
-        elif mode == 'k8':
+        elif mode == 'k8s' or mode == 'k8':
             oc = K8()
         else:
             raise ValueError(f'Invalid mode: {mode}')
         self._oc = oc
         return oc
 
     def get_namespace_name(self) -> Optional[str]:
@@ -132,27 +149,32 @@
 
     def load_app_configs(self) -> List[AppConfig]:
         """
         Loads all app configurations available in this project
         :return:
         """
         items = []
+        names = set()
         for dir_item in os.listdir(self._config_root):
             path = os.path.join(self._config_root, dir_item)
             if not os.path.isdir(path):
                 continue
             try:
                 app_config = self.load_app_config(dir_item)
             except FileNotFoundError:
                 # Index file missing
                 continue
 
             if app_config.is_template() or not app_config.enabled():
                 # Silently skip
                 continue
+            app_name = app_config.get_name()
+            if app_name in names:
+                raise ValueError(f'The app name {app_name} has already been used')
+            names.add(app_name)
             items.append(app_config)
         if self._library is not None:
             items.extend(self._library.load_app_configs())
         return items
 
     def load_app_config(self, name: str) -> AppConfig:
         folder_path = os.path.join(self._config_root, name)
```

### Comparing `octoploy-1.1.0/octoploy/config/ConfigMap.py` & `octoploy-1.2.0/octoploy/config/DynamicConfigMap.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     disable_templating: bool = False
 
     def __init__(self, data: Dict, disable_templating: bool = False):
         self.data = data
         self.disable_templating = disable_templating
 
 
-class ConfigMap:
+class DynamicConfigMap:
     def __init__(self, data):
         self._data = data
         self.name = data['name']
         self.files = data['files']
         self.disable_templating = data.get('disableTemplating', False)
 
     def build_object(self, config_root: str) -> ConfigMapObject:
```

### Comparing `octoploy-1.1.0/octoploy/config/DeploymentActionConfig.py` & `octoploy-1.2.0/octoploy/config/DeploymentActionConfig.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 from typing import TYPE_CHECKING
 
 from octoploy.utils.Log import Log
 
 if TYPE_CHECKING:
     from octoploy.config.Config import AppConfig
 
-from octoploy.oc.Oc import K8sApi
+from octoploy.api.Oc import K8sApi
 
 
 class DeploymentActionConfig(Log):
     """
     Configuration for a single user configurable deployment step
     """
 
     def __init__(self, app_config: AppConfig, data):
         super().__init__()
         self._data = data
         self._app_config = app_config
 
     def run(self, oc: K8sApi):
         if self._data == 'deploy':
-            oc.rollout(self._app_config.get_dc_name())
+            oc.rollout(self._app_config.get_name())
             return
 
         exec_config = self._data.get('exec', None)
         if exec_config is not None:
             cmd = exec_config['command']
             args = exec_config['args']
 
-            dc_name = self._app_config.get_dc_name()
+            dc_name = self._app_config.get_name()
             self.log.info('Reloading via exec in pods of ' + dc_name)
             pods = oc.get_pods(dc_name=dc_name)
             for pod in pods:
                 oc.exec(pod.name, cmd, args)
             return
```

### Comparing `octoploy-1.1.0/octoploy/deploy/AppDeploy.py` & `octoploy-1.2.0/octoploy/deploy/AppDeploy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from __future__ import annotations
 
 import os
 from typing import List
 
 import yaml
 
-from octoploy.config.Config import ProjectConfig, AppConfig, RunMode
+from octoploy.config.Config import RootConfig, AppConfig, RunMode
 from octoploy.deploy.DeploymentBundle import DeploymentBundle
 from octoploy.deploy.K8sObjectDeployer import K8sObjectDeployer
 from octoploy.processing.YmlTemplateProcessor import YmlTemplateProcessor
 from octoploy.utils.Errors import SkipObject
 from octoploy.utils.Log import Log
 from octoploy.utils.Yml import Yml
 
 
 class AppDeployment:
     """
-    Deploys a single application
+    Deploys a single application (aka all yml files inside an app directory)
     """
 
-    def __init__(self, root_config: ProjectConfig, app_config: AppConfig, mode: RunMode):
+    def __init__(self, root_config: RootConfig, app_config: AppConfig, mode: RunMode):
         self._root_config = root_config
         self._app_config = app_config
         self._mode = mode
 
     def deploy(self):
         """
         Deploys all instances of the app
@@ -39,15 +39,15 @@
 
 
 class AppDeployRunnerFactory:
     """
     Creates AppDeployRunner objects
     """
 
-    def __init__(self, root_config: ProjectConfig, mode: RunMode):
+    def __init__(self, root_config: RootConfig, mode: RunMode):
         self._root_config = root_config
         self._mode = mode
 
     def create(self, root_app_config: AppConfig) -> List[AppDeployRunner]:
         """
         Creates deployment runner instances for the given app
         :param root_app_config: App for which the instances should be created
@@ -60,29 +60,29 @@
 
 
 class AppDeployRunner(Log):
     """
     Executes the deployment of a single app
     """
 
-    def __init__(self, root_config: ProjectConfig, app_config: AppConfig, mode: RunMode = RunMode()):
+    def __init__(self, root_config: RootConfig, app_config: AppConfig, mode: RunMode = RunMode()):
         super().__init__()
         self._root_config = root_config
         self._app_config = app_config
         self._bundle = DeploymentBundle(self._root_config.get_pre_processor())
         self._mode = mode
 
     def deploy(self):
         """
         Deploys all items for the given app
         """
         if not self._app_config.enabled():
             raise ValueError('App is disabled')
         if self._app_config.is_template():
-            raise ValueError('App is a template and can\'t be deployed')
+            raise ValueError("App is a template and can't be deployed")
 
         # Resolve all templating references
         template_processor = self._app_config.get_template_processor()
         template_processor.parent(self._root_config.get_template_processor())
 
         self._apply_templates(self._app_config.get_pre_template_refs(), template_processor)
         self._load_files(self._app_config.get_config_root(), template_processor)
@@ -95,22 +95,23 @@
             for data in list(self._bundle.objects):
                 try:
                     processor.process(data)
                 except SkipObject as e:
                     self.log.warning(f'Skipping object: {e}')
                     self._bundle.objects.remove(data)
 
-        k8sapi = self._root_config.create_api()
+        api = self._root_config.create_api()
         if self._mode.out_file is not None:
             self._bundle.dump_objects(self._mode.out_file)
+
         if self._mode.dry_run:
             return
 
-        self.log.info(f'Checking {self._app_config.get_dc_name()}')
-        object_deployer = K8sObjectDeployer(self._root_config, k8sapi, self._app_config, mode=self._mode)
+        self.log.info(f'Checking {self._app_config.get_name()}')
+        object_deployer = K8sObjectDeployer(self._root_config, api, self._app_config, mode=self._mode)
         self._bundle.deploy(object_deployer)
 
     def _apply_templates(self, template_names: List[str], template_processor: YmlTemplateProcessor):
         """
         Deploys all referenced templates (recursively)
         """
         for template_name in template_names:
```

### Comparing `octoploy-1.1.0/octoploy/deploy/DeploymentBundle.py` & `octoploy-1.2.0/octoploy/deploy/DeploymentBundle.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import yaml
 
 from octoploy.deploy.K8sObjectDeployer import K8sObjectDeployer
 from octoploy.k8s.BaseObj import BaseObj
 from octoploy.processing.DataPreProcessor import DataPreProcessor
 from octoploy.processing.DecryptionProcessor import DecryptionProcessor
-from octoploy.processing.OcObjectMerge import OcObjectMerge
+from octoploy.processing.K8sObjectMerge import K8sObjectMerge
 from octoploy.processing.YmlTemplateProcessor import YmlTemplateProcessor
 from octoploy.utils.Log import Log
 from octoploy.utils.YmlWriter import YmlWriter
 
 
 class DeploymentBundle(Log):
     """
@@ -38,30 +38,30 @@
             self.log.info('Unknown object kind: ' + str(data))
             return
 
         # Pre-process any variables
         if template_processor is not None:
             template_processor.process(data)
 
-        merger = OcObjectMerge()
+        merger = K8sObjectMerge()
         # Check if the new data can be merged into any existing objects
         for item in self.objects:
             if merger.merge(item, data):
                 # Data has been merged
                 return
 
         self._pre_processor.process(data)
         self.objects.append(data)
 
     def deploy(self, deploy_runner: K8sObjectDeployer):
         """
-        Deploys all object
+        Deploys all objects in this bundle
         :param deploy_runner: Deployment runner which should be used
         """
-        deploy_runner.select_namespace()
+        deploy_runner.select_context()
 
         # First sort the objects, we want "deployments" to be the last object type
         # so all prerequisites are available
         def sorting(x):
             k8s_object = BaseObj(x)
             object_kind = k8s_object.kind.lower()
             if object_kind == 'DeploymentConfig'.lower() or \
@@ -69,14 +69,16 @@
                 return 1
             return 0
 
         self.objects.sort(key=sorting)
         for item in self.objects:
             deploy_runner.deploy_object(item)
 
+        deploy_runner.delete_abandoned_objects()
+
     def dump_objects(self, path: str):
         """
         Very crude method for dumping the objects to a yml file.
         If the file does already exist the content will be appended
         :param path: Path to a file
         """
         all_objects = []
```

### Comparing `octoploy-1.1.0/octoploy/oc/Model.py` & `octoploy-1.2.0/octoploy/api/Model.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.1.0/octoploy/octoploy.py` & `octoploy-1.2.0/octoploy/octoploy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from __future__ import annotations
 
 import argparse
 
-from octoploy.processing.DecryptionProcessor import DecryptionProcessor
-
 from octoploy.backup.BackupGenerator import BackupGenerator
-from octoploy.config.Config import ProjectConfig, RunMode
+from octoploy.config.Config import RootConfig, RunMode
 from octoploy.deploy.AppDeploy import AppDeployment
+from octoploy.processing.DecryptionProcessor import DecryptionProcessor
 from octoploy.utils.Encryption import YmlEncrypter
 from octoploy.utils.Log import Log
 
 log_instance = Log('octoploy')
 
 
-def load_project(config_dir: str) -> ProjectConfig:
+def load_project(config_dir: str) -> RootConfig:
     if config_dir != '':
-        return ProjectConfig.load(config_dir)
+        return RootConfig.load(config_dir)
 
     # No path specified, try a few common ones
     paths = ['.', 'configs', 'octoploy']
     for path in paths:
         try:
-            return ProjectConfig.load(path)
+            return RootConfig.load(path)
         except FileNotFoundError:
             continue
     raise FileNotFoundError(f'Did not find config in any of {paths}')
 
 
 def reload_config(args):
     root_config = load_project(args.config_dir)
@@ -34,35 +33,43 @@
         log_instance.log.error('App is disabled')
         return
     if app_config.is_template():
         log_instance.log.error('App is a template')
         return
 
     oc = root_config.create_api()
-    log_instance.log.info('Reloading ' + app_config.get_dc_name())
+    log_instance.log.info('Reloading ' + app_config.get_name())
     reload_actions = app_config.get_reload_actions()
     for action in reload_actions:
         action.run(oc)
     log_instance.log.info('Done')
 
 
 def _run_app_deploy(config_dir: str, app_name: str, mode: RunMode):
     root_config = load_project(config_dir)
     app_config = root_config.load_app_config(app_name)
-    deployment = AppDeployment(root_config, app_config, mode)
-    deployment.deploy()
+    root_config.initialize_state(mode)
+    try:
+        deployment = AppDeployment(root_config, app_config, mode)
+        deployment.deploy()
+    finally:
+        root_config.persist_state(mode)
     log_instance.log.info('Done')
 
 
 def _run_apps_deploy(config_dir: str, mode: RunMode):
     root_config = load_project(config_dir)
     configs = root_config.load_app_configs()
-    log_instance.log.info(f'Got {len(configs)} configs')
-    for app_config in configs:
-        AppDeployment(root_config, app_config, mode).deploy()
+    root_config.initialize_state(mode)
+    log_instance.log.debug(f'Found {len(configs)} apps to deploy')
+    try:
+        for app_config in configs:
+            AppDeployment(root_config, app_config, mode).deploy()
+    finally:
+        root_config.persist_state(mode)
     log_instance.log.info('Done')
 
 
 def plan_app(args):
     mode = RunMode()
     mode.plan = True
     _run_app_deploy(args.config_dir, args.name[0], mode)
@@ -95,30 +102,52 @@
 
 def encrypt_secrets(args):
     files = args.file
     for file in files:
         YmlEncrypter(file).encrypt()
 
 
+def move_state(args):
+    run_mode = RunMode()
+    source = args.items[0]
+    dest = args.items[1]
+
+    root_config = load_project(args.config_dir)
+    root_config.initialize_state(run_mode)
+
+    state = root_config.get_state()
+    state.move(source, dest)
+    root_config.persist_state(run_mode)
+
+
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('--version', dest='version', action='store_true',
                         help='Prints the current version')
     parser.add_argument('--debug', dest='debug', action='store_true',
                         help='Enables debug logging')
     parser.add_argument('--skip-secrets', dest='skip_secrets', action='store_true',
                         help="Skips all secret objects and therefore doesn't require a key to be set")
+    parser.add_argument('--deploy-plain-secrets', dest='deploy_plain_text', action='store_true',
+                        help="Deploys plain text secret objects")
     parser.add_argument('-c', '--config-dir', dest='config_dir',
                         help='Path to the folder containing all configurations',
                         default='')
 
     subparsers = parser.add_subparsers(help='Commands')
-    backup_parser = subparsers.add_parser('encrypt', help='Encrypts k8s secrets objects')
-    backup_parser.add_argument('file', help='Yml file to be encrypted', nargs=1)
-    backup_parser.set_defaults(func=encrypt_secrets)
+    state_parser = subparsers.add_parser('move-state', help='Moves objects from the state to other places')
+    state_parser.add_argument('items', help='Source and destination.\n'
+                                            'The format for an object is: octoployName/Namespace/Kind/K8sObjectName\n'
+                                            'For example: "my-old-app/Namespace2/Deployment/app" '
+                                            '"my-new-app/Namespace2/Deployment/app"', nargs=2)
+    state_parser.set_defaults(func=move_state)
+
+    encrypt_parser = subparsers.add_parser('encrypt', help='Encrypts k8s secrets objects')
+    encrypt_parser.add_argument('file', help='Yml file to be encrypted', nargs=1)
+    encrypt_parser.set_defaults(func=encrypt_secrets)
 
     backup_parser = subparsers.add_parser('backup', help='Creates a backup of all resources in the cluster')
     backup_parser.add_argument('name', help='Name of the backup folder', nargs=1)
     backup_parser.set_defaults(func=create_backup)
 
     reload_parser = subparsers.add_parser('reload', help='Reloads the configuration of a running application')
     reload_parser.add_argument('name', help='Name of the app which should be reloaded (folder name)', nargs=1)
@@ -132,15 +161,18 @@
                                             help='Verifies what changes have to be applied for all apps')
     plan_all_parser.set_defaults(func=plan_all)
 
     deploy_parser = subparsers.add_parser('deploy', help='Deploys the configuration of an application')
     deploy_parser.add_argument('--out-file', dest='out_file',
                                help='Writes all objects into a yml file instead of deploying them. '
                                     'This does not communicate with openshift in any way')
-    deploy_parser.add_argument('--dry-run', dest='dry_run', help='Does not interact with openshift',
+    deploy_parser.add_argument('--dry-run', dest='dry_run', help='Does not interact with k8s/openshift '
+                                                                 '(pure template processing). '
+                                                                 'Can be used in conjunction with out-file to preview '
+                                                                 'templates',
                                action='store_true')
     deploy_parser.add_argument('name', help='Name of the app which should be deployed (folder name)', nargs=1)
     deploy_parser.set_defaults(func=deploy_app)
 
     deploy_all_parser = subparsers.add_parser('deploy-all',
                                               help='Deploys all objects of all enabled application')
     deploy_all_parser.add_argument('--out-file', dest='out_file',
@@ -161,12 +193,13 @@
         exit(1)
         return
 
     if args.debug:
         Log.set_debug()
 
     DecryptionProcessor.skip_secrets = args.skip_secrets
+    DecryptionProcessor.deploy_plain_text = args.deploy_plain_text
     args.func(args)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `octoploy-1.1.0/octoploy/processing/DataPreProcessor.py` & `octoploy-1.2.0/octoploy/processing/DataPreProcessor.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.1.0/octoploy/processing/DecryptionProcessor.py` & `octoploy-1.2.0/octoploy/processing/DecryptionProcessor.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 from typing import Dict, Optional
 
 from octoploy.k8s.SecretObj import SecretObj
 from octoploy.processing.TreeWalker import TreeProcessor, TreeWalker
 from octoploy.utils import Utils
 from octoploy.utils.Encryption import Encryption
 from octoploy.utils.Errors import SkipObject
+from octoploy.utils.Log import Log
 
 
-class DecryptionProcessor(TreeProcessor):
+class DecryptionProcessor(TreeProcessor, Log):
     """
     Processes all objects, and replaces any encrypted placeholders.
     If skip_secrets is True, all secret object types wil lbe skipped
     """
 
     skip_secrets: bool = False
     """
     Indicates if all secrets should be skipped
     """
 
+    deploy_plain_text: bool = False
+    """
+    Indicates if plain text secrets should be skipped
+    """
+
     _secret_obj: Optional[SecretObj]
 
     def __init__(self):
+        super().__init__(__name__)
         self.encryption = Encryption()
 
     def process(self, root: Dict[str, any]):
         try:
             self._secret_obj = SecretObj(root)
         except ValueError:
             self._secret_obj = None
@@ -40,16 +47,20 @@
 
             # The secret may contain non encrypted values
             # We'll ignore them for now since we don't want to change the behavior
             # of octoploy for existing projects.
             # Also, it may increase chances of accidentally storing them in vcs
             if key in self._secret_obj.base64_data or \
                     key in self._secret_obj.string_data:
-                raise SkipObject('Secret contains plain text - use "octoploy encrypt" to encrypt your secrets')
+                if not DecryptionProcessor.deploy_plain_text:
+                    raise SkipObject(
+                        f'Secret {self._secret_obj.get_fqn()} contains plain text - '
+                        f'use "octoploy encrypt" to encrypt your secrets')
 
             return value
+
         if DecryptionProcessor.skip_secrets and self._secret_obj is not None:
             # We should skip the secret
             raise SkipObject('Secrets should be skipped')
 
         payload = Utils.remove_prefix(value, Encryption.CRYPT_PREFIX)
         return self.encryption.decrypt(payload)
```

### Comparing `octoploy-1.1.0/octoploy/processing/OcObjectMerge.py` & `octoploy-1.2.0/octoploy/processing/K8sObjectMerge.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Dict
 
-from octoploy.oc.Model import DeploymentConfig, NamedItem
+from octoploy.api.Model import DeploymentConfig, NamedItem
 from octoploy.utils.DictUtils import DictUtils
 from octoploy.utils.Log import Log
 
 
-class OcObjectMerge(Log):
+class K8sObjectMerge(Log):
     """
-    Merges openshift objects
+    Merges kubernetes objects
     """
     NAME_PATH = 'metadata.name'
 
     def __init__(self):
         super().__init__()
         self._existing_dc = None  # type: DeploymentConfig
         self._new_dc = None  # type: DeploymentConfig
@@ -29,15 +29,15 @@
             return False
 
         expected_name = DictUtils.get(existing, self.NAME_PATH)
         name = DictUtils.get(to_add, self.NAME_PATH)
         if name is not None and expected_name is not None and expected_name != name:
             return False
 
-        if expected_type == 'DeploymentConfig'.lower():
+        if expected_type == 'DeploymentConfig'.lower() or expected_type == 'Deployment'.lower():
             self._merge_dc(DeploymentConfig(existing), DeploymentConfig(to_add))
             return True
 
         self.log.warning('Don\'t know how to merge ' + expected_type)
 
     def _merge_dc(self, existing: DeploymentConfig, to_add: DeploymentConfig):
         """
```

### Comparing `octoploy-1.1.0/octoploy/processing/TreeWalker.py` & `octoploy-1.2.0/octoploy/processing/TreeWalker.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.1.0/octoploy/processing/ValueLoader.py` & `octoploy-1.2.0/octoploy/processing/ValueLoader.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,25 +16,30 @@
     def __init__(self, config: BaseConfig):
         self._config = config
 
     @abstractmethod
     def load(self, data: Dict) -> Dict[str, str]:
         pass
 
+    def _resolve_path(self, path: str) -> str:
+        if os.path.isabs(path):
+            return path
+        return self._config.get_file(path)
+
 
 class EnvLoader(ValueLoader):
 
     def load(self, data: Dict) -> Dict[str, str]:
         return dict(os.environ)
 
 
 class FileLoader(ValueLoader):
 
     def load(self, data: Dict) -> Dict[str, str]:
-        file = data['file']
+        file = self._resolve_path(data['file'])
         encoding = data.get('encoding', 'utf-8')
         conversion = data.get('conversion')
 
         with open(file, 'rb') as f:
             content = f.read()
 
         if conversion is not None:
@@ -44,15 +49,15 @@
 
         return {'': content.decode(encoding)}
 
 
 class PemLoader(ValueLoader):
 
     def load(self, data: Dict) -> Dict[str, str]:
-        file = data['file']
+        file = self._resolve_path(data['file'])
         cert = Cert(self._config.get_file(file))
         return {
             '_PUBLIC': cert.cert,
             '_KEY': cert.key,
             '_CACERT': ''.join(cert.cacerts),
         }
```

### Comparing `octoploy-1.1.0/octoploy/processing/YmlTemplateProcessor.py` & `octoploy-1.2.0/octoploy/processing/YmlTemplateProcessor.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.1.0/octoploy/utils/Cert.py` & `octoploy-1.2.0/octoploy/utils/Cert.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.1.0/octoploy/utils/DictUtils.py` & `octoploy-1.2.0/octoploy/utils/DictUtils.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.1.0/octoploy/utils/Encryption.py` & `octoploy-1.2.0/octoploy/utils/Encryption.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.1.0/octoploy/utils/Log.py` & `octoploy-1.2.0/octoploy/utils/Log.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.1.0/octoploy/utils/YmlWriter.py` & `octoploy-1.2.0/octoploy/utils/YmlWriter.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.1.0/octoploy.egg-info/PKG-INFO` & `octoploy-1.2.0/octoploy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octoploy
-Version: 1.1.0
+Version: 1.2.0
 Summary: Simple kubernetes / openshift templating engine with templating, libraries, state tracking
 Home-page: https://github.com/davidgiga1993/octoploy
 Author: davidgiga1993
 Author-email: david@dev-core.org
 License: UNKNOWN
 Description: # Kubernetes / openshift templating and deployment engine
         
@@ -80,15 +80,15 @@
         
         ### Root config
         
         Here is a sample `_root.yml` file
         
         ```yml
         # Name of the namespace / openshift project
-        project: 'my-oc-project'
+        namespace: 'my-oc-project'
         
         # K8s context which should be used for deploying
         context: 'my-k8s-cluster-config'
         
         # OPTIONAL STUFF
         # Global variables
         vars:
@@ -291,74 +291,74 @@
         with features. A common example would be a template which adds a monitoring sidecar container. In the `examples` you can
         find the `nsq-template` which defines a sidecar container.
         
         Here is a minimal example:
         
         ```yml
         # examples/nsq-template/dc.yml
-        kind: DeploymentConfig
-        apiVersion: v1
+        kind: Deployment
+        apiVersion: apps/v1
         spec:
           template:
             spec:
-            containers:
-              - name: "nsqd"
-              image: "nsqio/nsq"
+              containers:
+                - name: "nsqd"
+                image: "nsqio/nsq"
         ```
         
         ```yml
         # examples/my-app/dc.yml
-        kind: DeploymentConfig
-        apiVersion: v1
+        kind: Deployment
+        apiVersion: apps/v1
         metadata:
-          name: "${DC_NAME}"
+          name: "${APP_NAME}"
         
         spec:
           replicas: 1
           selector:
-            name: "${DC_NAME}"
+            name: "${APP_NAME}"
           strategy:
-            type: Rolling
+            type: RollingUpdate
         
           template:
             metadata:
               labels:
-                name: "${DC_NAME}"
+                name: "${APP_NAME}"
         
             spec:
               containers:
-                - name: "${DC_NAME}"
+                - name: "${APP_NAME}"
                   image: "docker-registry.default.svc:5000/oc-project/my-app:prod"
         ```
         
         If we now apply the nsq-template to our app using `postApplyTemplates: [nsq-template]` the
         `DeploymentConfig` object gets automatically merged:
         
         ```yml
         # Merged result after applying template
-        kind: DeploymentConfig
-        apiVersion: v1
+        kind: Deployment
+        apiVersion: apps/v1
         metadata:
-          name: "${DC_NAME}"
+          name: "${APP_NAME}"
         
         spec:
           replicas: 1
           selector:
-            name: "${DC_NAME}"
+            name: "${APP_NAME}"
           strategy:
-            type: Rolling
+            type: RollingUpdate
         
           template:
             metadata:
               labels:
-                name: "${DC_NAME}"
+                name: "${APP_NAME}"
         
             spec:
               containers:
-                - name: "${DC_NAME}"
+                - name: "${APP_NAME}"
                   image: "docker-registry.default.svc:5000/oc-project/my-app:prod"
                 # This is the part of the template
                 - name: "nsqd"
                   image: "nsqio/nsq"
         ```
         
         #### Loops
@@ -394,15 +394,15 @@
           - domain
           - dockerDomain
           - imageStreamTag
         ```
         
         ```yml
         # prod/_root.yml
-        project: 'prod-project'
+        namespace: 'prod-project'
         inherit: testLib
         
         # Required parameters
         vars:
           domain: my-prod.dev-core.org
           dockerDomain: prod-docker.com
           imageStreamTag: prod
@@ -420,18 +420,22 @@
         ```
         
         The file will be updated in place.
         
         For deploying encrypted secrets, you'll need to set the environment variable
         `OCTOPLOY_KEY` with your key used to encrypt the data.
         
-        ## Change tracking
+        ## State tracking
+        
+        Octoploy currently uses a ConfigMap called `octoploy-state` to keep track of the object states.
+        
+        The ConfigMap contains  all managed objects and their md5 sum. If this hash has changed the whole object will be
+        applied. If the object does already exist, but is not listed in the state it will simply be added to the state.
         
-        Changes are detected by storing a md5 sum in the label of the object. If this hash has changed the whole object will be
-        applied. If no label has been found in openshift the object is assumed to be equal, and the label is added.
+        You can modify the name of the configmap by setting the `stateName` variable in the `_root.yml` file.
         
         Currently, the actual fields of the yml files are not compared, however this is a planned feature.  
         
         ## Examples
         
         All examples can be found in the `examples` folder.
```

### Comparing `octoploy-1.1.0/octoploy.egg-info/SOURCES.txt` & `octoploy-1.2.0/octoploy.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,52 +6,56 @@
 octoploy/octoploy.py
 octoploy.egg-info/PKG-INFO
 octoploy.egg-info/SOURCES.txt
 octoploy.egg-info/dependency_links.txt
 octoploy.egg-info/entry_points.txt
 octoploy.egg-info/requires.txt
 octoploy.egg-info/top_level.txt
+octoploy/api/Model.py
+octoploy/api/Oc.py
+octoploy/api/__init__.py
 octoploy/backup/BackupGenerator.py
 octoploy/backup/__init__.py
 octoploy/config/AppConfig.py
 octoploy/config/BaseConfig.py
 octoploy/config/Config.py
-octoploy/config/ConfigMap.py
 octoploy/config/DeploymentActionConfig.py
+octoploy/config/DynamicConfigMap.py
 octoploy/config/YmlConfig.py
 octoploy/config/__init__.py
 octoploy/deploy/AppDeploy.py
 octoploy/deploy/DeploymentBundle.py
 octoploy/deploy/K8sObjectDeployer.py
 octoploy/deploy/__init__.py
 octoploy/k8s/BaseObj.py
 octoploy/k8s/SecretObj.py
 octoploy/k8s/__init__.py
-octoploy/oc/Model.py
-octoploy/oc/Oc.py
-octoploy/oc/__init__.py
 octoploy/processing/DataPreProcessor.py
 octoploy/processing/DecryptionProcessor.py
-octoploy/processing/OcObjectMerge.py
+octoploy/processing/K8sObjectMerge.py
 octoploy/processing/TreeWalker.py
 octoploy/processing/ValueLoader.py
 octoploy/processing/YmlTemplateProcessor.py
 octoploy/processing/__init__.py
+octoploy/state/StateTracking.py
+octoploy/state/__init__.py
 octoploy/utils/Cert.py
 octoploy/utils/DictUtils.py
 octoploy/utils/Encryption.py
 octoploy/utils/Errors.py
 octoploy/utils/Log.py
 octoploy/utils/Utils.py
 octoploy/utils/Yml.py
 octoploy/utils/YmlWriter.py
 octoploy/utils/__init__.py
 tests/AppDeploymentTest.py
 tests/DictUtilsTest.py
 tests/OcObjectMergeTest.py
+tests/StateTrackingTest.py
+tests/TestUtils.py
 tests/YmlTempalteProcessorTest.py
 tests/__init__.py
 tests/config/AppConfigTest.py
 tests/config/__init__.py
 tests/processing/ValueLoaderTest.py
 tests/processing/__init__.py
 tests/utils/EncryptionTest.py
```

### Comparing `octoploy-1.1.0/setup.py` & `octoploy-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.1.0/tests/AppDeploymentTest.py` & `octoploy-1.2.0/tests/AppDeploymentTest.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import os
+from time import sleep
 from unittest import TestCase
 
 import yaml
 
-from octoploy.config.Config import ProjectConfig, RunMode
+from octoploy.config.Config import RootConfig, RunMode
 from octoploy.deploy.AppDeploy import AppDeployment
 from octoploy.utils.Errors import MissingParam
 from octoploy.utils.Yml import Yml
+from tests import TestUtils
 
 
 class AppDeploymentTest(TestCase):
 
     def setUp(self) -> None:
         self._base_path = os.path.dirname(__file__)
         self._tmp_file = 'out.yml'
@@ -72,15 +74,15 @@
 
         # We should have two instances
         self.assertEqual(2, len(docs))
         self.assertEqual('hello', docs[0]['metadata']['REMAPPED'])
         self.assertEqual('hello', docs[1]['metadata']['REMAPPED'])
 
     def test_params(self):
-        prj_config = ProjectConfig.load(os.path.join(self._base_path, 'app_deploy_test'))
+        prj_config = RootConfig.load(os.path.join(self._base_path, 'app_deploy_test_params'))
         app_config = prj_config.load_app_config('app-params')
         runner = AppDeployment(prj_config, app_config, self._mode)
         try:
             runner.deploy()
             self.fail('No exception raised for missing param')
         except MissingParam:
             pass
@@ -95,26 +97,26 @@
             data = yaml.load(f, Loader=yaml.FullLoader)
         self.assertEqual('input', data['someObj']['param'])
 
     def test_secret_without_encryption(self):
         """
         Makes s ure secrets without encrypted values are not deployed
         """
-        os.environ['OCTOPLOY_KEY'] = 'key123'
+        os.environ['OCTOPLOY_KEY'] = TestUtils.OCTOPLOY_KEY
         self._deploy('secrets')
         with open(self._tmp_file) as f:
             data = yaml.load(f, Loader=yaml.FullLoader)
         self.assertTrue('plainText' not in data['stringData'])
 
     def test_decryption(self):
-        os.environ['OCTOPLOY_KEY'] = 'key123'
+        os.environ['OCTOPLOY_KEY'] = TestUtils.OCTOPLOY_KEY
         self._deploy('secrets')
         with open(self._tmp_file) as f:
             data = yaml.load(f, Loader=yaml.FullLoader)
         self.assertEqual('hello world', data['stringData']['ref'])
         self.assertEqual('hello world', data['stringData']['field'])
 
     def _deploy(self, app: str, project: str = 'app_deploy_test'):
-        prj_config = ProjectConfig.load(os.path.join(self._base_path, project))
+        prj_config = RootConfig.load(os.path.join(self._base_path, project))
         app_config = prj_config.load_app_config(app)
         runner = AppDeployment(prj_config, app_config, self._mode)
         runner.deploy()
```

### Comparing `octoploy-1.1.0/tests/DictUtilsTest.py` & `octoploy-1.2.0/tests/DictUtilsTest.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.1.0/tests/OcObjectMergeTest.py` & `octoploy-1.2.0/tests/OcObjectMergeTest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from unittest import TestCase
 
 import yaml
 
-from octoploy.processing.OcObjectMerge import OcObjectMerge
+from octoploy.processing.K8sObjectMerge import K8sObjectMerge
 
 
-class OcObjectMergeTest(TestCase):
+class K8sObjectMergeTest(TestCase):
 
     def test_append_sidecar_container(self):
-        existing = '''kind: DeploymentConfig
+        existing = '''kind: Deployment
 apiVersion: v1
 metadata:
   name: "${DC_NAME}"
 
 spec:
   replicas: 1
   selector:
@@ -29,22 +29,22 @@
       containers:
         - name: "${DC_NAME}"
           volumeMounts:
             - name: java-cacerts-volume
               mountPath: /java/java-cacerts
 '''
         new = '''
-kind: DeploymentConfig
+kind: Deployment
 spec:
   template:
     spec:
       containers:
         - name: "sidecar-container"
 '''
-        merge = OcObjectMerge()
+        merge = K8sObjectMerge()
         data = yaml.safe_load(existing)
         merge.merge(data, yaml.safe_load(new))
 
         def validate(data):
             self.assertEqual('v1', data['apiVersion'])
             containers = data['spec']['template']['spec']['containers']
             self.assertEqual(2, len(containers))
@@ -59,15 +59,15 @@
 
         # Now invert the inputs, the result should be the same
         new_data = yaml.safe_load(new)
         merge.merge(new_data, yaml.safe_load(existing))
         validate(new_data)
 
     def test_merge_same_container(self):
-        existing = '''kind: DeploymentConfig
+        existing = '''kind: Deployment
 apiVersion: v1
 metadata:
   name: "${DC_NAME}"
 
 spec:
   replicas: 1
   selector:
@@ -113,15 +113,15 @@
         containerNames:
           - "${DC_NAME}"
         from:
           kind: ImageStreamTag
           name: '${DC_NAME}:prod'
 '''
         new = '''
-kind: DeploymentConfig
+kind: Deployment
 metadata:
   name: "${DC_NAME}"
 
 spec:
   template:
     metadata:
       labels:
@@ -135,15 +135,15 @@
               mountPath: /packages
 
       volumes:
         - name: crawler-packages-volume
           persistentVolumeClaim:
             claimName: "pvc-crawler-packages"'''
 
-        merge = OcObjectMerge()
+        merge = K8sObjectMerge()
         data = yaml.safe_load(existing)
         merge.merge(data, yaml.safe_load(new))
 
         containers = data['spec']['template']['spec']['containers']
         self.assertEqual(1, len(containers))
 
         container = containers[0]
```

### Comparing `octoploy-1.1.0/tests/YmlTempalteProcessorTest.py` & `octoploy-1.2.0/tests/YmlTempalteProcessorTest.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.1.0/tests/processing/ValueLoaderTest.py` & `octoploy-1.2.0/tests/processing/ValueLoaderTest.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.1.0/tests/utils/EncryptionTest.py` & `octoploy-1.2.0/tests/utils/EncryptionTest.py`

 * *Files identical despite different names*

