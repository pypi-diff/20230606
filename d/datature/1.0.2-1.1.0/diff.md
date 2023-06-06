# Comparing `tmp/datature-1.0.2.tar.gz` & `tmp/datature-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/Puppeteer/Puppeteer/pypi/puppeteer/dist/.tmp-78ndph57/datature-1.0.2.tar", last modified: Wed May 31 09:04:42 2023, max compression
+gzip compressed data, was "/home/runner/work/Puppeteer/Puppeteer/pypi/puppeteer/dist/.tmp-67kkp98n/datature-1.1.0.tar", last modified: Tue Jun  6 07:05:53 2023, max compression
```

## Comparing `datature-1.0.2.tar` & `datature-1.1.0.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-05-31 09:04:27.000000 datature-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-31 09:04:27.000000 datature-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-31 09:04:42.000000 datature-1.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/datature/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-31 09:04:27.000000 datature-1.0.2/datature/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/datature/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:27.000000 datature-1.0.2/datature/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-05-31 09:04:27.000000 datature-1.0.2/datature/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-05-31 09:04:27.000000 datature-1.0.2/datature/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17290 2023-05-31 09:04:27.000000 datature-1.0.2/datature/cli/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-31 09:04:27.000000 datature-1.0.2/datature/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-31 09:04:27.000000 datature-1.0.2/datature/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/datature/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:27.000000 datature-1.0.2/datature/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-31 09:04:27.000000 datature-1.0.2/datature/http/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-31 09:04:27.000000 datature-1.0.2/datature/http/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-31 09:04:27.000000 datature-1.0.2/datature/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-31 09:04:27.000000 datature-1.0.2/datature/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/datature/processor/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-31 09:04:27.000000 datature-1.0.2/datature/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-31 09:04:27.000000 datature-1.0.2/datature/processor/base_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-31 09:04:27.000000 datature-1.0.2/datature/processor/dicom_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-31 09:04:27.000000 datature-1.0.2/datature/processor/nii_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/datature/rest/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-31 09:04:27.000000 datature-1.0.2/datature/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15223 2023-05-31 09:04:27.000000 datature-1.0.2/datature/rest/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-05-31 09:04:27.000000 datature-1.0.2/datature/rest/artifact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/datature/rest/asset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:27.000000 datature-1.0.2/datature/rest/asset/__int__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-05-31 09:04:27.000000 datature-1.0.2/datature/rest/asset/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-05-31 09:04:27.000000 datature-1.0.2/datature/rest/asset/upload_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-05-31 09:04:27.000000 datature-1.0.2/datature/rest/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-05-31 09:04:27.000000 datature-1.0.2/datature/rest/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-05-31 09:04:27.000000 datature-1.0.2/datature/rest/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    14570 2023-05-31 09:04:27.000000 datature-1.0.2/datature/rest/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-31 09:04:27.000000 datature-1.0.2/datature/rest/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-05-31 09:04:27.000000 datature-1.0.2/datature/rest/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-31 09:04:27.000000 datature-1.0.2/datature/rest/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/datature/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:27.000000 datature-1.0.2/datature/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-31 09:04:27.000000 datature-1.0.2/datature/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/datature.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-31 09:04:42.000000 datature-1.0.2/datature.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-31 09:04:42.000000 datature-1.0.2/datature.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:04:42.000000 datature-1.0.2/datature.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-31 09:04:42.000000 datature-1.0.2/datature.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-31 09:04:42.000000 datature-1.0.2/datature.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-31 09:04:42.000000 datature-1.0.2/datature.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-31 09:04:27.000000 datature-1.0.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-31 09:04:27.000000 datature-1.0.2/docs/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-31 09:04:27.000000 datature-1.0.2/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:04:42.000000 datature-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-31 09:04:27.000000 datature-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:27.000000 datature-1.0.2/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/test/fixture/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:27.000000 datature-1.0.2/test/fixture/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/test/fixture/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:27.000000 datature-1.0.2/test/fixture/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-31 09:04:27.000000 datature-1.0.2/test/fixture/data/error_fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-31 09:04:27.000000 datature-1.0.2/test/fixture/data/operation_fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-31 09:04:27.000000 datature-1.0.2/test/fixture/data/upload_session_fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-31 09:04:27.000000 datature-1.0.2/test/fixture/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/test/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:27.000000 datature-1.0.2/test/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-05-31 09:04:27.000000 datature-1.0.2/test/http/test_requester.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-31 09:04:27.000000 datature-1.0.2/test/http/test_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/test/rest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:27.000000 datature-1.0.2/test/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-05-31 09:04:27.000000 datature-1.0.2/test/rest/test_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-31 09:04:27.000000 datature-1.0.2/test/rest/test_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-31 09:04:27.000000 datature-1.0.2/test/rest/test_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-05-31 09:04:27.000000 datature-1.0.2/test/rest/test_asset_upload_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-31 09:04:27.000000 datature-1.0.2/test/rest/test_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-31 09:04:27.000000 datature-1.0.2/test/rest/test_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-31 09:04:27.000000 datature-1.0.2/test/rest/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-31 09:04:27.000000 datature-1.0.2/test/rest/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-31 09:04:27.000000 datature-1.0.2/test/rest/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-31 09:04:27.000000 datature-1.0.2/test/rest/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-31 09:04:27.000000 datature-1.0.2/test/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-31 09:04:27.000000 datature-1.0.2/test/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-06-06 07:05:39.000000 datature-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-06 07:05:39.000000 datature-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-06 07:05:53.000000 datature-1.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/datature/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-06 07:05:39.000000 datature-1.1.0/datature/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/datature/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:39.000000 datature-1.1.0/datature/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-06-06 07:05:39.000000 datature-1.1.0/datature/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-06-06 07:05:39.000000 datature-1.1.0/datature/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17214 2023-06-06 07:05:39.000000 datature-1.1.0/datature/cli/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-06 07:05:39.000000 datature-1.1.0/datature/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-06 07:05:39.000000 datature-1.1.0/datature/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/datature/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:39.000000 datature-1.1.0/datature/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-06 07:05:39.000000 datature-1.1.0/datature/http/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-06 07:05:39.000000 datature-1.1.0/datature/http/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-06 07:05:39.000000 datature-1.1.0/datature/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-06 07:05:39.000000 datature-1.1.0/datature/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/datature/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-06 07:05:39.000000 datature-1.1.0/datature/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-06 07:05:39.000000 datature-1.1.0/datature/processor/base_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-06 07:05:39.000000 datature-1.1.0/datature/processor/dicom_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-06-06 07:05:39.000000 datature-1.1.0/datature/processor/nii_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/datature/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-06 07:05:39.000000 datature-1.1.0/datature/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15282 2023-06-06 07:05:39.000000 datature-1.1.0/datature/rest/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-06-06 07:05:39.000000 datature-1.1.0/datature/rest/artifact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/datature/rest/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:39.000000 datature-1.1.0/datature/rest/asset/__int__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-06-06 07:05:39.000000 datature-1.1.0/datature/rest/asset/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-06-06 07:05:39.000000 datature-1.1.0/datature/rest/asset/upload_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-06-06 07:05:39.000000 datature-1.1.0/datature/rest/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-06-06 07:05:39.000000 datature-1.1.0/datature/rest/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-06-06 07:05:39.000000 datature-1.1.0/datature/rest/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14873 2023-06-06 07:05:39.000000 datature-1.1.0/datature/rest/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-06-06 07:05:39.000000 datature-1.1.0/datature/rest/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-06-06 07:05:39.000000 datature-1.1.0/datature/rest/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-06 07:05:39.000000 datature-1.1.0/datature/rest/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/datature/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:39.000000 datature-1.1.0/datature/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-06 07:05:39.000000 datature-1.1.0/datature/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/datature.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-06 07:05:53.000000 datature-1.1.0/datature.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-06 07:05:53.000000 datature-1.1.0/datature.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 07:05:53.000000 datature-1.1.0/datature.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-06 07:05:53.000000 datature-1.1.0/datature.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-06 07:05:53.000000 datature-1.1.0/datature.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-06 07:05:53.000000 datature-1.1.0/datature.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-06 07:05:39.000000 datature-1.1.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-06 07:05:39.000000 datature-1.1.0/docs/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-06 07:05:39.000000 datature-1.1.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 07:05:53.000000 datature-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-06 07:05:39.000000 datature-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:39.000000 datature-1.1.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/test/fixture/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:39.000000 datature-1.1.0/test/fixture/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/test/fixture/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:39.000000 datature-1.1.0/test/fixture/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-06 07:05:39.000000 datature-1.1.0/test/fixture/data/error_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-06 07:05:39.000000 datature-1.1.0/test/fixture/data/operation_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-06 07:05:39.000000 datature-1.1.0/test/fixture/data/upload_session_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-06 07:05:39.000000 datature-1.1.0/test/fixture/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/test/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:39.000000 datature-1.1.0/test/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-06 07:05:39.000000 datature-1.1.0/test/http/test_requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-06 07:05:39.000000 datature-1.1.0/test/http/test_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/test/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:39.000000 datature-1.1.0/test/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-06-06 07:05:39.000000 datature-1.1.0/test/rest/test_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-06 07:05:39.000000 datature-1.1.0/test/rest/test_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-06-06 07:05:39.000000 datature-1.1.0/test/rest/test_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-06-06 07:05:39.000000 datature-1.1.0/test/rest/test_asset_upload_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-06 07:05:39.000000 datature-1.1.0/test/rest/test_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-06 07:05:39.000000 datature-1.1.0/test/rest/test_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-06 07:05:39.000000 datature-1.1.0/test/rest/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-06 07:05:39.000000 datature-1.1.0/test/rest/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-06 07:05:39.000000 datature-1.1.0/test/rest/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-06 07:05:39.000000 datature-1.1.0/test/rest/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-06 07:05:39.000000 datature-1.1.0/test/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-06 07:05:39.000000 datature-1.1.0/test/test_logger.py
```

### Comparing `datature-1.0.2/LICENSE` & `datature-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datature-1.0.2/PKG-INFO` & `datature-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datature
-Version: 1.0.2
+Version: 1.1.0
 Summary: Python bindings for the Datature API
 Author: Raighne Weng
 Author-email: raighne@datature.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `datature-1.0.2/datature/cli/commands.py` & `datature-1.1.0/datature/cli/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   commands.py
 @Author  :   Raighne.Weng
-@Version :   0.7.3
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   CLI supported commands
 '''
 
 import sys
 from argparse import ArgumentParser, _SubParsersAction
```

### Comparing `datature-1.0.2/datature/cli/config.py` & `datature-1.1.0/datature/cli/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   config.py
 @Author  :   Raighne.Weng
-@Version :   0.7.1
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   CLI config class
 '''
 
 import io
 import sys
```

### Comparing `datature-1.0.2/datature/cli/functions.py` & `datature-1.1.0/datature/cli/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   functions.py
 @Author  :   Raighne.Weng
-@Version :   1.0.2
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   CLI functions
 '''
 
 import os
 import re
@@ -34,18 +34,14 @@
 from datature.rest.types import AnnotationFormat
 
 # pylint: disable=E1102
 
 ASSET_UPLOAD_BATCH_SIZE = datature.ASSET_UPLOAD_BATCH_SIZE
 datature.SHOW_PROGRESS = True
 
-if 'DATATURE_API_BASE_URL' in os.environ:
-    datature.API_BASE_URL = os.environ['DATATURE_API_BASE_URL']
-
-
 def authenticate():
     """
     Authenticate the Project Secret with the server and creates a configuration file for it.
 
     :param project_secret: Secret key to use for the client login.
     :return: None
     """
@@ -180,15 +176,15 @@
     if not path:
         questions = [
             inquirer.Path("path_result",
                           message=messages.ASSETS_FOLDER_MESSAGE,
                           default=os.getcwd()),
         ]
         answer = inquirer.prompt(questions, raise_keyboard_interrupt=True)
-        path = answer.get("path_result")
+        path = answer.get("path_result").strip()
 
     if not exists(path):
         print(messages.PATH_NOT_EXISTS_MESSAGE)
         sys.exit(1)
 
     # find all images under folder and sub folders
     file_paths = utils.find_all_assets(path)
@@ -257,15 +253,15 @@
     """
     if not path:
         questions = [
             inquirer.Path("path_result",
                           message=messages.ANNOTATION_FOLDER_MESSAGE),
         ]
         answer = inquirer.prompt(questions, raise_keyboard_interrupt=True)
-        path = answer.get("path_result")
+        path = answer.get("path_result").strip()
 
     if not annotation_format:
         questions = [
             inquirer.List(
                 "annotation_format",
                 message=messages.ANNOTATION_FORMAT_MESSAGE,
                 choices=[format.value for format in AnnotationFormat],
@@ -322,15 +318,15 @@
     if not path:
         questions = [
             inquirer.Path("path_result",
                           message=messages.ARTIFACT_MODEL_FOLDER_MESSAGE,
                           default=os.getcwd()),
         ]
         answer = inquirer.prompt(questions, raise_keyboard_interrupt=True)
-        path = answer.get("path_result")
+        path = answer.get("path_result").strip()
 
     if not exists(path):
         print(messages.PATH_NOT_EXISTS_MESSAGE)
         sys.exit(1)
 
     if not artifact_id:
         # call server to list all artifacts
@@ -415,15 +411,15 @@
     if not path:
         questions = [
             inquirer.Path("path_result",
                           message=messages.EXPORT_ANNOTATION_FOLDER_MESSAGE,
                           default=os.getcwd()),
         ]
         answer = inquirer.prompt(questions, raise_keyboard_interrupt=True)
-        path = answer.get("path_result")
+        path = answer.get("path_result").strip()
 
     if not exists(path):
         print(messages.PATH_NOT_EXISTS_MESSAGE)
         sys.exit(1)
 
     if not annotation_format:
         questions = [
```

### Comparing `datature-1.0.2/datature/cli/main.py` & `datature-1.1.0/datature/cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   main.py
 @Author  :   Raighne.Weng
-@Version :   0.7.1
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   CLI main entrance
 '''
 
 import sys
```

### Comparing `datature-1.0.2/datature/error.py` & `datature-1.1.0/datature/error.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   error.py
 @Author  :   Raighne.Weng
-@Version :   0.1.0
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Error Class module
 '''
 
 
 class Error(Exception):
```

### Comparing `datature-1.0.2/datature/http/requester.py` & `datature-1.1.0/datature/http/requester.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,21 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   requester.py
 @Author  :   Raighne.Weng
-@Version :   0.6.2
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   A wrapper to make HTTP requests
 '''
 
+import os
 import json
 from urllib.parse import urlencode
 
 import humps
 from requests import Response, request
 
 import datature
@@ -47,14 +48,17 @@
 
         # CHeck Secret
         if datature.secret_key is None:
             raise error.UnauthorizedError(
                 "No project secret key provided. (Set your secret key"
                 " using datature.secret_key = <secret_key>)")
 
+        if 'DATATURE_API_BASE_URL' in os.environ:
+            datature.API_BASE_URL = os.environ['DATATURE_API_BASE_URL']
+
         absolute_url = f"{datature.API_BASE_URL}{url}"
 
         # Assemble queries and request body.
         post_data = None
         post_files = None
 
         if query:
```

### Comparing `datature-1.0.2/datature/http/resource.py` & `datature-1.1.0/datature/http/resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   resource.py
 @Author  :   Raighne.Weng
-@Version :   0.1.0
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Base class for REST API resources
 '''
 
 from halo import Halo
```

### Comparing `datature-1.0.2/datature/logger.py` & `datature-1.1.0/datature/logger.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.2/datature/messages.py` & `datature-1.1.0/datature/messages.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   messages.py
 @Author  :   Raighne.Weng
-@Version :   0.7.1
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   collect all string messages variables
 '''
 
 REQUEST_SERVER_MESSAGE = "Communicating with server."
 SERVER_COMPLETED_MESSAGE = "Server processing completed."
```

### Comparing `datature-1.0.2/datature/processor/__init__.py` & `datature-1.1.0/datature/processor/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   __init__.py
 @Author  :   Raighne.Weng
-@Version :   0.7.3
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Processor package
 '''
 
 from os import PathLike
 import pathlib
```

### Comparing `datature-1.0.2/datature/processor/base_processor.py` & `datature-1.1.0/datature/processor/base_processor.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   base_processor.py
 @Author  :   Raighne.Weng
-@Version :   0.7.3
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Base Processor module
 '''
 
 from typing import List
 from abc import ABC, abstractmethod
```

### Comparing `datature-1.0.2/datature/processor/dicom_processor.py` & `datature-1.1.0/datature/processor/dicom_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   dicom_processor.py
 @Author  :   Raighne.Weng
-@Version :   0.7.3
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Dicom Processor
 '''
 
 import tempfile
 from typing import List
```

### Comparing `datature-1.0.2/datature/processor/nii_processor.py` & `datature-1.1.0/datature/processor/nii_processor.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   nii_processor.py
 @Author  :   Raighne.Weng
-@Version :   0.7.3
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Nii Processor
 '''
 
 import tempfile
 from typing import List
@@ -61,47 +61,61 @@
             makedirs(video_output)
 
         scan = nib.load(file_path)
 
         # Read data and get scan's shape
         scan_array = scan.get_fdata()
 
+        # Get image pixel
+        scan_headers = scan.header
+        pix_dim = scan_headers['pixdim'][1:4]
+
+        # Calculate new image dimensions from aspect ratio
+        new_scan_dims = np.multiply(scan_array.shape, pix_dim)
+        new_scan_dims = (round(new_scan_dims[0]), round(new_scan_dims[1]),
+                     round(new_scan_dims[2]))
+
         # if client provide the orientation
         if orientation and orientation in ["x", "y", "z"]:
             output_file_path = f"{video_output}/{file_name}-{orientation}.mp4"
 
-            self.__write_video(scan_array, orientation, output_file_path)
+            self.__write_video(scan_array, orientation, output_file_path, new_scan_dims)
 
             return [output_file_path]
 
         # if not then save all orientations
         output_file_paths = []
         for orientation in ["x", "y", "z"]:
             output_file_path = f"{video_output}/{file_name}-{orientation}.mp4"
 
-            self.__write_video(scan_array, orientation, output_file_path)
+            self.__write_video(scan_array, orientation, output_file_path, new_scan_dims)
 
             output_file_paths.append(output_file_path)
 
         return output_file_paths
 
-    def __write_video(self, scan_array, orientation, saved_path):
+    def __write_video(self, scan_array, orientation, saved_path, scan_dims):
         """Write video to file
 
         :param scan_array: The NIfTI scan array data.
         :param axis: The orientation of the pics.
         :param saved_path: The saved file path.
+        :param scan_dims: The image dimensions of the file.
         """
-        four_cc = cv2.VideoWriter_fourcc(*"mp4v")
-        video_writer = cv2.VideoWriter(saved_path, four_cc, 30.0, (1024, 1024))
-
         axis = {'x': 0, 'y': 1, 'z': 2}[orientation]
+        size = {'x': [scan_dims[2],scan_dims[1]],
+                'y': [scan_dims[2],scan_dims[0]],
+                'z': [scan_dims[1],scan_dims[0]]
+                }[orientation]
+
+        four_cc = cv2.VideoWriter_fourcc(*"mp4v")
+        video_writer = cv2.VideoWriter(saved_path, four_cc, 30.0, size)
 
         for i in range(scan_array.shape[axis]):
             # Get slice along the correct axis and resize
             slice_axis = scan_array.take(i, axis=axis)
-            image = cv2.resize(slice_axis, (1024, 1024))
+            image = cv2.resize(slice_axis, size)
 
             # Convert to RGB and write to video file
             new_image = cv2.cvtColor(np.uint8(image), cv2.COLOR_GRAY2RGB)
             video_writer.write(new_image)
         video_writer.release()
```

### Comparing `datature-1.0.2/datature/rest/__init__.py` & `datature-1.1.0/datature/rest/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   __init__.py
 @Author  :   Raighne.Weng
-@Version :   0.5.0
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature rest module
 '''
 
 from datature.rest.project import Project
 from datature.rest.asset.asset import Asset
```

### Comparing `datature-1.0.2/datature/rest/annotation.py` & `datature-1.1.0/datature/rest/annotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,28 +4,27 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   annotation.py
 @Author  :   Raighne.Weng
-@Version :   1.0.2
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Annotation API
 '''
 
 from datature.utils import utils
 from datature.http.resource import RESTResource
 from datature.rest.operation import Operation
 from datature.rest.types import (AnnotationExportOptions, AnnotationFormat,
                                  AnnotationMetadata)
 
 
-
 class Annotation(RESTResource):
     """Datature Annotation API Resource."""
 
     @classmethod
     def list(cls, asset_id: str) -> dict:
         """Lists all annotations of a specific asset.
 
@@ -344,20 +343,22 @@
                         import datature
 
                         datature.secret_key = "5aa41e8ba........"
 
                         datature.Annotation.upload("csv_fourcorner",
                                                 "Your file path")
         """
-        upload_paths = utils.find_all_annotations_files(file_path, annotation_format)
+        upload_paths = utils.find_all_annotations_files(
+            file_path, annotation_format)
 
-        upload_list =[]
+        upload_list = []
         for upload_path in upload_paths:
             with open(upload_path, "rb") as file:
-                upload_list.append(('files', (file.name, file.read(), 'application/octet-stream')))
+                upload_list.append(('files', (file.name, file.read(),
+                                              'application/octet-stream')))
 
         response = cls.request(
             "POST",
             "/annotation/import",
             query={"format": annotation_format},
             request_files=upload_list,
         )
```

### Comparing `datature-1.0.2/datature/rest/artifact.py` & `datature-1.1.0/datature/rest/artifact.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   artifact.py
 @Author  :   Raighne.Weng
-@Version :   0.4.0
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Artifact API
 '''
 
 from datature.http.resource import RESTResource
```

### Comparing `datature-1.0.2/datature/rest/asset/asset.py` & `datature-1.1.0/datature/rest/asset/asset.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   asset.py
 @Author  :   Raighne.Weng
-@Version :   0.7.6
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Asset API
 '''
 
 from datature.http.resource import RESTResource
 from datature.rest.asset.upload_session import UploadSession
```

### Comparing `datature-1.0.2/datature/rest/asset/upload_session.py` & `datature-1.1.0/datature/rest/asset/upload_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   upload_session.py
 @Author  :   Raighne.Weng
-@Version :   0.7.6
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Asset Upload Session
 '''
 
 import json
 import struct
```

### Comparing `datature-1.0.2/datature/rest/deploy.py` & `datature-1.1.0/datature/rest/deploy.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   Deploy.py
 @Author  :   Raighne.Weng
-@Version :   0.5.0
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Deploy API
 '''
 
 from datature.http.resource import RESTResource
 from datature.rest.types import DeploymentMetadata
```

### Comparing `datature-1.0.2/datature/rest/operation.py` & `datature-1.1.0/datature/rest/operation.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   operation.py
 @Author  :   Raighne.Weng
-@Version :   0.1.0
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Operation API
 '''
 
 import time
```

### Comparing `datature-1.0.2/datature/rest/project.py` & `datature-1.1.0/datature/rest/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   project.py
 @Author  :   Raighne.Weng
-@Version :   0.6.5
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Project API
 '''
 
 from datature.http.resource import RESTResource
 from datature.rest.types import ProjectMetadata
@@ -107,16 +107,15 @@
                 .. code-block:: python
 
                         import datature
 
                         datature.secret_key = "5aa41e8ba........"
                         datature.Project.modify({"name":"My Cool Project"})
         """
-        return cls.request("PUT",
-                           "/project", request_body=project)
+        return cls.request("PUT", "/project", request_body=project)
 
     @classmethod
     def quota(cls) -> dict:
         """Retrieves the project quota showing the limits based on the tier the project account is on and the current usage.
 
         :return: A dictionary containing the project quota metadata with the following structure:
```

### Comparing `datature-1.0.2/datature/rest/run.py` & `datature-1.1.0/datature/rest/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,16 @@
                                     "checkpoint": {
                                         "strategy": "STRAT_LOWEST_VALIDATION_LOSS",
                                         "evaluation_interval": 100,
                                         "metric": "Loss/total_loss"
                                     }
                                 },
                                 "features": {
-                                    "preview": true
+                                    "preview": True,
+                                    "matrix": True
                                 },
                                 "create_date": 1676353954729,
                                 "last_modified_date": 1676356061724,
                                 "logs": [
                                     "log_63eb212ff0f856bf95085095"
                                 ]
                             }
@@ -118,15 +119,16 @@
                                     "checkpoint": {
                                         "strategy": "STRAT_LOWEST_VALIDATION_LOSS",
                                         "evaluation_interval": 100,
                                         "metric": "Loss/total_loss"
                                     }
                                 },
                                 "features": {
-                                    "preview": true
+                                    "preview": True,
+                                    "matrix": True
                                 },
                                 "create_date": 1676353954729,
                                 "last_modified_date": 1676356061724,
                                 "logs": [
                                     "log_63eb212ff0f856bf95085095"
                                 ]
                             }
@@ -178,15 +180,16 @@
                                     "checkpoint": {
                                         "strategy": "STRAT_LOWEST_VALIDATION_LOSS",
                                         "evaluation_interval": 100,
                                         "metric": "Loss/total_loss"
                                     }
                                 },
                                 "features": {
-                                    "preview": true
+                                    "preview": True,
+                                    "matrix": True
                                 },
                                 "create_date": 1676353954729,
                                 "last_modified_date": 1676356061724,
                                 "logs": [
                                     "log_63eb212ff0f856bf95085095"
                                 ]
                             }
@@ -241,15 +244,16 @@
                                     "checkpoint": {
                                         "strategy": "STRAT_LOWEST_VALIDATION_LOSS",
                                         "evaluation_interval": 100,
                                         "metric": "Loss/total_loss"
                                     }
                                 },
                                 "features": {
-                                    "preview": true
+                                    "preview": True,
+                                    "matrix": True
                                 },
                                 "create_date": 1676353954729,
                                 "last_modified_date": 1676356061724,
                                 "logs": [
                                     "log_63eb212ff0f856bf95085095"
                                 ]
                             }
@@ -270,15 +274,16 @@
                                 "strategy": "STRAT_ALWAYS_SAVE_LATEST",
                                 "evaluation_interval": 1
                             },
                             "limit": {
                                 "metric": "LIM_NONE",
                                 "value": 0
                             },
-                            "preview": True
+                            "preview": True,
+                            "matrix": True
                         })
         """
         return cls.request(
             "POST",
             "/run",
             request_body={
                 "flowId": flow_id,
@@ -298,15 +303,16 @@
                     "limit": {
                         "metric": setup.get("limit").get("metric"),
                         "value": setup.get("limit").get("value"),
                     },
                     "debug": setup.get("debug"),
                 },
                 "features": {
-                    "preview": setup.get("preview")
+                    "preview": setup.get("preview"),
+                    "matrix": setup.get("matrix")
                 }
             })
 
     @classmethod
     def log(cls, log_id: str) -> dict:
         """Retrieves a specific training log using the log ID.
```

### Comparing `datature-1.0.2/datature/rest/tag.py` & `datature-1.1.0/datature/rest/tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   tag.py
 @Author  :   Raighne.Weng
-@Version :   0.2.0
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Tag API
 '''
 
 from datature.http.resource import RESTResource
```

### Comparing `datature-1.0.2/datature/rest/types.py` & `datature-1.1.0/datature/rest/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,32 +4,34 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   types.py
 @Author  :   Raighne.Weng
-@Version :   1.0.2
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Types for Datature API resources.
 '''
 
 from enum import Enum
 from dataclasses import dataclass
 
+
 @dataclass
 class ProjectMetadata:
     """Project metadata.
 
     :param name: The name of the project.
     """
 
     name: str
 
+
 @dataclass
 class AnnotationMetadata:
     """Annotation metadata.
 
     :param asset_id: The unique ID of the asset.
     :param tag: The tag class name of the annotation.
     :param bound_type: The bound type of the annotation (rectangle or polygon).
@@ -68,25 +70,27 @@
     :param limit: A limit on the number of objects to be returned in a page. Defaults to 10.
         If the length of the function call results exceeds the limit, the results will be broken into multiple pages.
     """
 
     page: str
     limit: int = 10
 
+
 @dataclass
 class AssetMetadata:
     """Asset Metadata.
 
     :param status: The annotation status of the asset (annotated, review, completed, tofix, none).
     :param custom_metadata: A dictionary containing any key-value pairs.
     """
 
     status: str
     custom_metadata: object
 
+
 class AnnotationFormat(Enum):
     """Annotation CSV Format.
 
     Bounding Box Options:
         coco
         csv_fourcorner
         csv_widthheight
@@ -215,16 +219,16 @@
     """
 
     accelerator: Accelerator
     checkpoint: Checkpoint
     limit: Limit
     preview: bool = True
 
+
 @dataclass
 class FlowMetadata:
     """Workflow Metadata.
 
     :param title: The title of the workflow.
     """
 
     title: str
-
```

### Comparing `datature-1.0.2/datature/rest/workflow.py` & `datature-1.1.0/datature/rest/workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   workflow.py
 @Author  :   Raighne.Weng
-@Version :   0.3.0
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Workflow API
 '''
 
 from datature.rest.types import FlowMetadata
 from datature.http.resource import RESTResource
@@ -99,17 +99,15 @@
 
                         import datature
 
                         datature.secret_key = "5aa41e8ba........"
                         datature.Workflow.modify(
                             "flow_639309be08b4488a914b8802", {"title": "My awesome workflow"})
         """
-        return cls.request("PUT",
-                           f"/workflow/{flow_id}",
-                           request_body=flow)
+        return cls.request("PUT", f"/workflow/{flow_id}", request_body=flow)
 
     @classmethod
     def delete(cls, flow_id: str) -> dict:
         """Deletes a specific workflow using the flow ID.
 
         :param flow_id: The ID of the workflow
         :return: A dictionary containing the deleted workflow ID and deletion status with the following structure:
```

### Comparing `datature-1.0.2/datature/utils/utils.py` & `datature-1.1.0/datature/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   utils.py
 @Author  :   Raighne.Weng
-@Version :   1.0.2
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Utils Class module
 '''
 
 import os
 import glob
@@ -75,23 +75,25 @@
     """
     List all annotations files under folder, include sub folder.
 
     :param path: The folder to upload annotations files.
     :param annotation_format: The format of the annotation type.
     :return: assets path list.
     """
-    file_extensions = ANNOTATION_FORMAT_EXTENSIONS_MAPPING.get(annotation_format)
+    file_extensions = ANNOTATION_FORMAT_EXTENSIONS_MAPPING.get(
+        annotation_format)
 
     if not file_extensions:
         raise Error("The annotation format is not valid")
 
-    file_paths =[]
+    file_paths = []
     if isfile(path):
         file_paths.append(path)
     elif isdir(path):
         for file_ext in file_extensions:
-            file_paths.extend(glob.glob(os.path.join(path, '**', file_ext), recursive=True))
+            file_paths.extend(
+                glob.glob(os.path.join(path, '**', file_ext), recursive=True))
 
     if len(file_paths) <= 0:
         raise Error("Could not find the annotation file")
 
     return file_paths
```

### Comparing `datature-1.0.2/datature.egg-info/PKG-INFO` & `datature-1.1.0/datature.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datature
-Version: 1.0.2
+Version: 1.1.0
 Summary: Python bindings for the Datature API
 Author: Raighne Weng
 Author-email: raighne@datature.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `datature-1.0.2/datature.egg-info/SOURCES.txt` & `datature-1.1.0/datature.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datature-1.0.2/docs/source/conf.py` & `datature-1.1.0/docs/source/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   conf.py
 @Author  :   Raighne.Weng
-@Version :   0.6.5
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Python Doc
 '''
 
 import os
 import sys
```

### Comparing `datature-1.0.2/docs/upload.py` & `datature-1.1.0/docs/upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   upload.py
 @Author  :   Raighne.Weng
-@Version :   0.7.7
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Upload python SDK documentation to readme
 '''
 
 import os
 import re
```

### Comparing `datature-1.0.2/readme.md` & `datature-1.1.0/readme.md`

 * *Files identical despite different names*

### Comparing `datature-1.0.2/setup.py` & `datature-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   setup.py
 @Author  :   Raighne.Weng
-@Version :   0.7.4
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Setup module
 '''
 
 import re
 import setuptools
```

### Comparing `datature-1.0.2/test/fixture/data/error_fixture.py` & `datature-1.1.0/test/fixture/data/error_fixture.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   error_fixture.py
 @Author  :   Raighne.Weng
-@Version :   0.1.0
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Error Response Test Data
 '''
 
 forbidden_error_response = {
     "code": "ForbiddenError",
```

### Comparing `datature-1.0.2/test/fixture/data/operation_fixture.py` & `datature-1.1.0/test/fixture/data/operation_fixture.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   operation_fixture.py
 @Author  :   Raighne.Weng
-@Version :   0.1.0
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Operation Test Data
 '''
 
 pending_operation_response = {
     'id': 'op_c26ea31d-599c-4a03-8b0d-b2bc9995fa8a',
```

### Comparing `datature-1.0.2/test/fixture/data/upload_session_fixture.py` & `datature-1.1.0/test/fixture/data/upload_session_fixture.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   upload_session_fixture.py
 @Author  :   Raighne.Weng
-@Version :   0.1.0
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Upload Session Test Data
 '''
 
 # pylint: disable=C0301
 upload_assets_response = {
```

### Comparing `datature-1.0.2/test/fixture/mock.py` & `datature-1.1.0/test/fixture/mock.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   mock.py
 @Author  :   Raighne.Weng
-@Version :   0.1.0
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Test Mock Cases
 '''
 
 
 # pylint: disable=R0903
```

### Comparing `datature-1.0.2/test/http/test_requester.py` & `datature-1.1.0/test/http/test_requester.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_requester.py
 @Author  :   Raighne.Weng
-@Version :   0.1.0
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature HTTP Resource Test Cases
 '''
 
 import unittest
 from unittest.mock import patch
```

### Comparing `datature-1.0.2/test/http/test_resource.py` & `datature-1.1.0/test/http/test_resource.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_resource.py
 @Author  :   Raighne.Weng
-@Version :   0.1.0
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature HTTP Resource Test Cases
 '''
 
 import unittest
 from unittest.mock import patch
```

### Comparing `datature-1.0.2/test/rest/test_annotation.py` & `datature-1.1.0/test/rest/test_annotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_annotation.py
 @Author  :   Raighne.Weng
-@Version :   0.1.0
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Annotation API Test Cases
 '''
 
 import unittest
 from unittest.mock import MagicMock, patch
```

### Comparing `datature-1.0.2/test/rest/test_artifact.py` & `datature-1.1.0/test/rest/test_artifact.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_artifact.py
 @Author  :   Raighne.Weng
-@Version :   0.4.0
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Artifact API Test Cases
 '''
 
 import unittest
 from unittest.mock import MagicMock
```

### Comparing `datature-1.0.2/test/rest/test_asset.py` & `datature-1.1.0/test/rest/test_asset.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_asset.py
 @Author  :   Raighne.Weng
-@Version :   0.1.0
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Asset API Test Cases
 '''
 
 import unittest
 from unittest.mock import MagicMock, patch
```

### Comparing `datature-1.0.2/test/rest/test_asset_upload_session.py` & `datature-1.1.0/test/rest/test_asset_upload_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_asset_upload_session.py
 @Author  :   Raighne.Weng
-@Version :   0.1.0
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Asset Upload Session API Test Cases
 '''
 
 import unittest
 from unittest.mock import MagicMock, patch
```

### Comparing `datature-1.0.2/test/rest/test_deploy.py` & `datature-1.1.0/test/rest/test_deploy.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_deploy.py
 @Author  :   Raighne.Weng
-@Version :   0.5.0
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Deploy API Test Cases
 '''
 
 import unittest
 from unittest.mock import MagicMock
```

### Comparing `datature-1.0.2/test/rest/test_operation.py` & `datature-1.1.0/test/rest/test_operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_operation.py
 @Author  :   Raighne.Weng
-@Version :   0.1.0
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Operation API Test Cases
 '''
 
 import unittest
 from unittest.mock import MagicMock
```

### Comparing `datature-1.0.2/test/rest/test_project.py` & `datature-1.1.0/test/rest/test_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_project.py
 @Author  :   Raighne.Weng
-@Version :   0.1.0
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Project API Test Cases
 '''
 
 import unittest
 from unittest.mock import MagicMock
```

### Comparing `datature-1.0.2/test/rest/test_run.py` & `datature-1.1.0/test/rest/test_run.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_run.py
 @Author  :   Raighne.Weng
-@Version :   0.7.2
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Run API Test Cases
 '''
 
 import unittest
 from unittest.mock import MagicMock
@@ -63,15 +63,16 @@
                     "evaluation_interval": 1,
                     "metric": "Loss/total_loss"
                 },
                 "limit": {
                     "metric": "LIM_MINUTE",
                     "value": 260
                 },
-                "preview": True
+                "preview": True,
+                "matrix": True
             })
 
         Run.request.assert_called_once_with(
             "POST",
             "/run",
             request_body={
                 "flowId": "flow_id",
@@ -88,15 +89,16 @@
                     "limit": {
                         "metric": "LIM_MINUTE",
                         "value": 260
                     },
                     "debug": None
                 },
                 "features": {
-                    "preview": True
+                    "preview": True,
+                    "matrix": True
                 }
             })
 
     def test_log(self):
         """Test retrieve a training log."""
         Run.request = MagicMock()
```

### Comparing `datature-1.0.2/test/rest/test_tag.py` & `datature-1.1.0/test/rest/test_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_tag.py
 @Author  :   Raighne.Weng
-@Version :   0.2.0
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Project API Test Cases.
 '''
 
 import unittest
 from unittest.mock import MagicMock
```

### Comparing `datature-1.0.2/test/rest/test_workflow.py` & `datature-1.1.0/test/rest/test_workflow.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_workflow.py
 @Author  :   Raighne.Weng
-@Version :   0.3.0
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Workflow API Test Cases
 '''
 
 import unittest
 from unittest.mock import MagicMock
```

### Comparing `datature-1.0.2/test/test_error.py` & `datature-1.1.0/test/test_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_error.py
 @Author  :   Raighne.Weng
-@Version :   0.1.0
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Error Test Cases
 '''
 
 import unittest
 from datature.error import BadRequestError
```

### Comparing `datature-1.0.2/test/test_logger.py` & `datature-1.1.0/test/test_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_logger.py
 @Author  :   Raighne.Weng
-@Version :   0.1.0
+@Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Logger Test Cases
 '''
 
 import unittest
 from unittest.mock import patch
```

