# Comparing `tmp/aheadworks_deploy_manager-1.4.8.tar.gz` & `tmp/aheadworks_deploy_manager-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aheadworks_deploy_manager-1.4.8.tar", last modified: Mon Sep 19 09:27:27 2022, max compression
+gzip compressed data, was "dist/aheadworks_deploy_manager-1.4.9.tar", last modified: Mon Sep 19 10:46:26 2022, max compression
```

## Comparing `aheadworks_deploy_manager-1.4.8.tar` & `aheadworks_deploy_manager-1.4.9.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 09:27:27.000000 aheadworks_deploy_manager-1.4.8/
--rw-r--r--   0 root         (0) root         (0)      266 2022-09-19 09:27:27.000000 aheadworks_deploy_manager-1.4.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 09:27:27.000000 aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      144 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 09:27:27.000000 aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7744 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/api/bitbucket_api_manager.py
--rw-rw-rw-   0 root         (0) root         (0)      640 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/api/db_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     5205 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/api/dockerhub_api_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     1198 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/api/file_manager.py
--rw-rw-rw-   0 root         (0) root         (0)    14044 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/api/version_control_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 09:27:27.000000 aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/console/
--rw-rw-rw-   0 root         (0) root         (0)    10041 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/console/console.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 09:27:27.000000 aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/model/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 09:27:27.000000 aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/model/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/model/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1523 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/model/data/bitbucket.py
--rw-rw-rw-   0 root         (0) root         (0)     1282 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/model/data/dockerhub.py
--rw-rw-rw-   0 root         (0) root         (0)      423 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/model/logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 09:27:27.000000 aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/model/parser/
--rw-rw-rw-   0 root         (0) root         (0)      786 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/model/parser/php.py
--rw-rw-rw-   0 root         (0) root         (0)      354 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/model/ssh_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 09:27:27.000000 aheadworks_deploy_manager-1.4.8/aheadworks_composer_manager/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_composer_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8102 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_composer_manager/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 09:27:27.000000 aheadworks_deploy_manager-1.4.8/aheadworks_composer_manager/model/
--rw-rw-rw-   0 root         (0) root         (0)     3227 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_composer_manager/model/extension.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 09:27:27.000000 aheadworks_deploy_manager-1.4.8/aheadworks_core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      131 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_core/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 09:27:27.000000 aheadworks_deploy_manager-1.4.8/aheadworks_core/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_core/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      952 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_core/api/composer_manager.py
--rw-rw-rw-   0 root         (0) root         (0)      198 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_core/api/discord_api_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2863 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_core/api/file_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_core/api/jira_api_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     7569 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_core/api/magento_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     1047 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_core/api/sftp_client_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 09:27:27.000000 aheadworks_deploy_manager-1.4.8/aheadworks_core/console/
--rw-rw-rw-   0 root         (0) root         (0)      563 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_core/console/console.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 09:27:27.000000 aheadworks_deploy_manager-1.4.8/aheadworks_core/model/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_core/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      353 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_core/model/cd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 09:27:27.000000 aheadworks_deploy_manager-1.4.8/aheadworks_core/model/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_core/model/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       36 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_core/model/data/data_object.py
--rw-rw-rw-   0 root         (0) root         (0)      233 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_core/model/data/jira.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 09:27:27.000000 aheadworks_deploy_manager-1.4.8/aheadworks_core/model/http/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_core/model/http/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2732 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_core/model/http/api_request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 09:27:27.000000 aheadworks_deploy_manager-1.4.8/aheadworks_core/model/parser/
--rw-rw-rw-   0 root         (0) root         (0)      541 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_core/model/parser/json.py
--rw-rw-rw-   0 root         (0) root         (0)      646 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_core/model/parser/xml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 09:27:27.000000 aheadworks_deploy_manager-1.4.8/aheadworks_deploy_manager.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)      266 2022-09-19 09:27:26.000000 aheadworks_deploy_manager-1.4.8/aheadworks_deploy_manager.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2213 2022-09-19 09:27:27.000000 aheadworks_deploy_manager-1.4.8/aheadworks_deploy_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2022-09-19 09:27:26.000000 aheadworks_deploy_manager-1.4.8/aheadworks_deploy_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      103 2022-09-19 09:27:26.000000 aheadworks_deploy_manager-1.4.8/aheadworks_deploy_manager.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)      124 2022-09-19 09:27:26.000000 aheadworks_deploy_manager-1.4.8/aheadworks_deploy_manager.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2022-09-19 09:27:21.000000 aheadworks_deploy_manager-1.4.8/aheadworks_deploy_manager.egg-info/zip-safe
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 09:27:27.000000 aheadworks_deploy_manager-1.4.8/aheadworks_release_manager/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_release_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      142 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_release_manager/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 09:27:27.000000 aheadworks_deploy_manager-1.4.8/aheadworks_release_manager/api/
--rw-rw-rw-   0 root         (0) root         (0)     3762 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_release_manager/api/pipeline_manager.py
--rw-rw-rw-   0 root         (0) root         (0)    20895 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_release_manager/api/release_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 09:27:27.000000 aheadworks_deploy_manager-1.4.8/aheadworks_release_manager/console/
--rw-rw-rw-   0 root         (0) root         (0)     3321 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_release_manager/console/console.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 09:27:27.000000 aheadworks_deploy_manager-1.4.8/aheadworks_test_manager/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_test_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10286 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/aheadworks_test_manager/__main__.py
--rw-r--r--   0 root         (0) root         (0)       38 2022-09-19 09:27:27.000000 aheadworks_deploy_manager-1.4.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1504 2022-09-19 09:27:11.000000 aheadworks_deploy_manager-1.4.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 10:46:26.000000 aheadworks_deploy_manager-1.4.9/
+-rw-r--r--   0 root         (0) root         (0)      266 2022-09-19 10:46:26.000000 aheadworks_deploy_manager-1.4.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 10:46:26.000000 aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      144 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 10:46:26.000000 aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7744 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/api/bitbucket_api_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)      640 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/api/db_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     5205 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/api/dockerhub_api_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1198 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/api/file_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    14044 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/api/version_control_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 10:46:26.000000 aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/console/
+-rw-rw-rw-   0 root         (0) root         (0)    10041 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/console/console.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 10:46:26.000000 aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/model/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 10:46:26.000000 aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/model/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/model/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1523 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/model/data/bitbucket.py
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/model/data/dockerhub.py
+-rw-rw-rw-   0 root         (0) root         (0)      423 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/model/logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 10:46:26.000000 aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/model/parser/
+-rw-rw-rw-   0 root         (0) root         (0)      786 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/model/parser/php.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/model/ssh_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 10:46:26.000000 aheadworks_deploy_manager-1.4.9/aheadworks_composer_manager/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_composer_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8102 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_composer_manager/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 10:46:26.000000 aheadworks_deploy_manager-1.4.9/aheadworks_composer_manager/model/
+-rw-rw-rw-   0 root         (0) root         (0)     3227 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_composer_manager/model/extension.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 10:46:26.000000 aheadworks_deploy_manager-1.4.9/aheadworks_core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      131 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_core/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 10:46:26.000000 aheadworks_deploy_manager-1.4.9/aheadworks_core/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_core/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      952 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_core/api/composer_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_core/api/discord_api_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2863 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_core/api/file_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_core/api/jira_api_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     7569 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_core/api/magento_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1047 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_core/api/sftp_client_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 10:46:26.000000 aheadworks_deploy_manager-1.4.9/aheadworks_core/console/
+-rw-rw-rw-   0 root         (0) root         (0)      563 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_core/console/console.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 10:46:26.000000 aheadworks_deploy_manager-1.4.9/aheadworks_core/model/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_core/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      353 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_core/model/cd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 10:46:26.000000 aheadworks_deploy_manager-1.4.9/aheadworks_core/model/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_core/model/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       36 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_core/model/data/data_object.py
+-rw-rw-rw-   0 root         (0) root         (0)      233 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_core/model/data/jira.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 10:46:26.000000 aheadworks_deploy_manager-1.4.9/aheadworks_core/model/http/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_core/model/http/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2732 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_core/model/http/api_request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 10:46:26.000000 aheadworks_deploy_manager-1.4.9/aheadworks_core/model/parser/
+-rw-rw-rw-   0 root         (0) root         (0)      541 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_core/model/parser/json.py
+-rw-rw-rw-   0 root         (0) root         (0)      646 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_core/model/parser/xml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 10:46:26.000000 aheadworks_deploy_manager-1.4.9/aheadworks_deploy_manager.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)      266 2022-09-19 10:46:26.000000 aheadworks_deploy_manager-1.4.9/aheadworks_deploy_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2213 2022-09-19 10:46:26.000000 aheadworks_deploy_manager-1.4.9/aheadworks_deploy_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2022-09-19 10:46:26.000000 aheadworks_deploy_manager-1.4.9/aheadworks_deploy_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      103 2022-09-19 10:46:26.000000 aheadworks_deploy_manager-1.4.9/aheadworks_deploy_manager.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)      124 2022-09-19 10:46:26.000000 aheadworks_deploy_manager-1.4.9/aheadworks_deploy_manager.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2022-09-19 10:46:19.000000 aheadworks_deploy_manager-1.4.9/aheadworks_deploy_manager.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 10:46:26.000000 aheadworks_deploy_manager-1.4.9/aheadworks_release_manager/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_release_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      142 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_release_manager/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 10:46:26.000000 aheadworks_deploy_manager-1.4.9/aheadworks_release_manager/api/
+-rw-rw-rw-   0 root         (0) root         (0)     3722 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_release_manager/api/pipeline_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    20895 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_release_manager/api/release_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 10:46:26.000000 aheadworks_deploy_manager-1.4.9/aheadworks_release_manager/console/
+-rw-rw-rw-   0 root         (0) root         (0)     3321 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_release_manager/console/console.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 10:46:26.000000 aheadworks_deploy_manager-1.4.9/aheadworks_test_manager/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_test_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10286 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/aheadworks_test_manager/__main__.py
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-19 10:46:26.000000 aheadworks_deploy_manager-1.4.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2022-09-19 10:46:08.000000 aheadworks_deploy_manager-1.4.9/setup.py
```

### Comparing `aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/api/bitbucket_api_manager.py` & `aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/api/bitbucket_api_manager.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/api/db_manager.py` & `aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/api/db_manager.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/api/dockerhub_api_manager.py` & `aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/api/dockerhub_api_manager.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/api/file_manager.py` & `aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/api/file_manager.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/api/version_control_manager.py` & `aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/api/version_control_manager.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/console/console.py` & `aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/console/console.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/model/data/bitbucket.py` & `aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/model/data/bitbucket.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/model/data/dockerhub.py` & `aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/model/data/dockerhub.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.4.8/aheadworks_bitbucket_manager/model/parser/php.py` & `aheadworks_deploy_manager-1.4.9/aheadworks_bitbucket_manager/model/parser/php.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.4.8/aheadworks_composer_manager/__main__.py` & `aheadworks_deploy_manager-1.4.9/aheadworks_composer_manager/__main__.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.4.8/aheadworks_composer_manager/model/extension.py` & `aheadworks_deploy_manager-1.4.9/aheadworks_composer_manager/model/extension.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.4.8/aheadworks_core/api/composer_manager.py` & `aheadworks_deploy_manager-1.4.9/aheadworks_core/api/composer_manager.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.4.8/aheadworks_core/api/file_manager.py` & `aheadworks_deploy_manager-1.4.9/aheadworks_core/api/file_manager.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.4.8/aheadworks_core/api/jira_api_manager.py` & `aheadworks_deploy_manager-1.4.9/aheadworks_core/api/jira_api_manager.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.4.8/aheadworks_core/api/magento_manager.py` & `aheadworks_deploy_manager-1.4.9/aheadworks_core/api/magento_manager.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.4.8/aheadworks_core/api/sftp_client_manager.py` & `aheadworks_deploy_manager-1.4.9/aheadworks_core/api/sftp_client_manager.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.4.8/aheadworks_core/console/console.py` & `aheadworks_deploy_manager-1.4.9/aheadworks_core/console/console.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.4.8/aheadworks_core/model/http/api_request.py` & `aheadworks_deploy_manager-1.4.9/aheadworks_core/model/http/api_request.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.4.8/aheadworks_core/model/parser/json.py` & `aheadworks_deploy_manager-1.4.9/aheadworks_core/model/parser/json.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.4.8/aheadworks_core/model/parser/xml.py` & `aheadworks_deploy_manager-1.4.9/aheadworks_core/model/parser/xml.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.4.8/aheadworks_deploy_manager.egg-info/SOURCES.txt` & `aheadworks_deploy_manager-1.4.9/aheadworks_deploy_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.4.8/aheadworks_release_manager/api/pipeline_manager.py` & `aheadworks_deploy_manager-1.4.9/aheadworks_release_manager/api/pipeline_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,29 +44,29 @@
         lastIndex = None
         firstInstructionIndex = None
         lastInstructionIndex = None
         for index, line in enumerate(lines):
             if line.find('&deployPipelines') != -1:
                 firstInstructionIndex = index
             # TODO: This line is going to change once we migrate to deploy-tools library
-            elif line.find('deploypipeline.py') != -1 or line.find("send_pipelines_to_workspace") != -1:
+            elif line.find("send-pipelines-to-workspace") != -1:
                 lastInstructionIndex = index + 1
             elif line.find('deploy-pipeline') != -1:
                 firstIndex = index
             elif line.find('*deployPipelines') != -1:
                 lastIndex = index + 1
         del lines[firstIndex:lastIndex]
         del lines[firstInstructionIndex:lastInstructionIndex]
         return "".join(lines)
 
     def update_repository_pipelines(self, url, new_bitbucket_pipelines):
         subprocess.Popen(['git', 'clone', url]).communicate()
-        subprocess.Popen(['ls', '-la']).communicate()
         module = url.split('/')[-1].replace('.git', '')
         os.chdir(module)
+        subprocess.Popen(['ls', '-la']).communicate()
         output = subprocess.check_output("git branch -al --no-merged", shell=True)
         decoded = output.decode('UTF-8')
         branches = decoded.splitlines()
         #'UTF-8' remove bin format, then 'splitlines' -- from str to list
         for branch in branches:
             clean_branch = branch.strip().removeprefix("remotes/origin/")
             # Update release or develop branches only
```

### Comparing `aheadworks_deploy_manager-1.4.8/aheadworks_release_manager/api/release_manager.py` & `aheadworks_deploy_manager-1.4.9/aheadworks_release_manager/api/release_manager.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.4.8/aheadworks_release_manager/console/console.py` & `aheadworks_deploy_manager-1.4.9/aheadworks_release_manager/console/console.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.4.8/aheadworks_test_manager/__main__.py` & `aheadworks_deploy_manager-1.4.9/aheadworks_test_manager/__main__.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.4.8/setup.py` & `aheadworks_deploy_manager-1.4.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='aheadworks_deploy_manager',
-    version='1.4.8',
+    version='1.4.9',
     zip_safe=True,
     packages=[
         'aheadworks_composer_manager',
         'aheadworks_core',
         'aheadworks_bitbucket_manager',
         'aheadworks_release_manager',
         'aheadworks_test_manager'
```

