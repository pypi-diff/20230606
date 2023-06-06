# Comparing `tmp/auto-test-common-1.0.8.tar.gz` & `tmp/auto-test-common-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-test-common-1.0.8.tar", last modified: Mon Jun  5 08:02:49 2023, max compression
+gzip compressed data, was "auto-test-common-1.0.9.tar", last modified: Mon Jun  5 09:09:23 2023, max compression
```

## Comparing `auto-test-common-1.0.8.tar` & `auto-test-common-1.0.9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-05 08:02:49.427003 auto-test-common-1.0.8/
--rw-r--r--   0 edz        (502) staff       (20)      547 2023-06-05 08:02:49.427184 auto-test-common-1.0.8/PKG-INFO
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-05 08:02:49.395959 auto-test-common-1.0.8/auto_test_common.egg-info/
--rw-r--r--   0 edz        (502) staff       (20)      547 2023-06-05 08:02:49.000000 auto-test-common-1.0.8/auto_test_common.egg-info/PKG-INFO
--rw-r--r--   0 edz        (502) staff       (20)     1611 2023-06-05 08:02:49.000000 auto-test-common-1.0.8/auto_test_common.egg-info/SOURCES.txt
--rw-r--r--   0 edz        (502) staff       (20)        1 2023-06-05 08:02:49.000000 auto-test-common-1.0.8/auto_test_common.egg-info/dependency_links.txt
--rw-r--r--   0 edz        (502) staff       (20)       56 2023-06-05 08:02:49.000000 auto-test-common-1.0.8/auto_test_common.egg-info/entry_points.txt
--rw-r--r--   0 edz        (502) staff       (20)      571 2023-06-05 08:02:49.000000 auto-test-common-1.0.8/auto_test_common.egg-info/requires.txt
--rw-r--r--   0 edz        (502) staff       (20)        7 2023-06-05 08:02:49.000000 auto-test-common-1.0.8/auto_test_common.egg-info/top_level.txt
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-05 08:02:49.396355 auto-test-common-1.0.8/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-1.0.8/common/__init__.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-05 08:02:49.398859 auto-test-common-1.0.8/common/autotest/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-1.0.8/common/autotest/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     8490 2023-05-09 01:49:15.000000 auto-test-common-1.0.8/common/autotest/base_requests.py
--rw-r--r--   0 edz        (502) staff       (20)     6429 2023-03-22 09:11:00.000000 auto-test-common-1.0.8/common/autotest/handle_allure.py
--rw-r--r--   0 edz        (502) staff       (20)    10869 2023-06-02 07:24:35.000000 auto-test-common-1.0.8/common/autotest/handle_assert.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-05 08:02:49.401553 auto-test-common-1.0.8/common/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-1.0.8/common/common/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2126 2023-04-23 02:46:40.000000 auto-test-common-1.0.8/common/common/api_driver.py
--rw-r--r--   0 edz        (502) staff       (20)     3612 2023-05-30 05:55:54.000000 auto-test-common-1.0.8/common/common/constant.py
--rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-1.0.8/common/common/test.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-05 08:02:49.402608 auto-test-common-1.0.8/common/config/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.0.8/common/config/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2429 2022-12-01 00:35:00.000000 auto-test-common-1.0.8/common/config/config.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-05 08:02:49.404728 auto-test-common-1.0.8/common/data/
--rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-1.0.8/common/data/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    17370 2023-05-24 07:32:32.000000 auto-test-common-1.0.8/common/data/data_process.py
--rw-r--r--   0 edz        (502) staff       (20)     8641 2023-05-30 08:45:37.000000 auto-test-common-1.0.8/common/data/handle_common.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-05 08:02:49.408091 auto-test-common-1.0.8/common/db/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.0.8/common/db/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-1.0.8/common/db/handle_db.py
--rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-1.0.8/common/db/handle_db_batch.py
--rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-1.0.8/common/db/handle_mysqldb.py
--rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-1.0.8/common/db/handle_oracle.py
--rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-1.0.8/common/db/handle_sqlserver.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-05 08:02:49.409301 auto-test-common-1.0.8/common/driver/
--rw-r--r--   0 edz        (502) staff       (20)        0 2023-06-05 07:58:39.000000 auto-test-common-1.0.8/common/driver/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)      127 2023-06-05 08:02:38.000000 auto-test-common-1.0.8/common/driver/api_page.py
--rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-05 08:02:38.000000 auto-test-common-1.0.8/common/driver/ui_page.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-05 08:02:49.413035 auto-test-common-1.0.8/common/file/
--rw-r--r--   0 edz        (502) staff       (20)     4508 2023-04-14 00:29:00.000000 auto-test-common-1.0.8/common/file/ReadFile.py
--rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-1.0.8/common/file/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    11473 2023-05-31 08:51:34.000000 auto-test-common-1.0.8/common/file/handle_excel.py
--rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-1.0.8/common/file/handle_file.py
--rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-1.0.8/common/file/handle_reques.py
--rw-r--r--   0 edz        (502) staff       (20)     2201 2022-10-24 01:09:00.000000 auto-test-common-1.0.8/common/file/handle_system.py
--rw-r--r--   0 edz        (502) staff       (20)      955 2023-06-01 02:02:40.000000 auto-test-common-1.0.8/common/file/handle_yaml.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-05 08:02:49.413900 auto-test-common-1.0.8/common/mq/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.0.8/common/mq/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-1.0.8/common/mq/handle_rabbit.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-05 08:02:49.417245 auto-test-common-1.0.8/common/plat/
--rw-r--r--   0 edz        (502) staff       (20)     3543 2023-05-31 01:13:42.000000 auto-test-common-1.0.8/common/plat/ATF_platform.py
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-1.0.8/common/plat/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-1.0.8/common/plat/jenkin_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     7851 2023-05-30 02:15:47.000000 auto-test-common-1.0.8/common/plat/jira_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     8129 2023-05-30 07:56:22.000000 auto-test-common-1.0.8/common/plat/mysql_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     8826 2023-05-31 01:13:42.000000 auto-test-common-1.0.8/common/plat/service_platform.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-05 08:02:49.426487 auto-test-common-1.0.8/common/plugin/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-1.0.8/common/plugin/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1330 2023-01-16 07:33:00.000000 auto-test-common-1.0.8/common/plugin/allure_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     2054 2022-07-28 02:48:00.000000 auto-test-common-1.0.8/common/plugin/assert_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     8259 2023-05-31 03:06:08.000000 auto-test-common-1.0.8/common/plugin/atf_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     6768 2023-05-15 07:47:06.000000 auto-test-common-1.0.8/common/plugin/data_bus.py
--rw-r--r--   0 edz        (502) staff       (20)     3654 2023-05-27 02:43:55.000000 auto-test-common-1.0.8/common/plugin/data_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    12181 2023-06-05 06:08:01.000000 auto-test-common-1.0.8/common/plugin/file_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-1.0.8/common/plugin/hooks_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-1.0.8/common/plugin/pytest_playwright.py
--rw-r--r--   0 edz        (502) staff       (20)    17733 2023-06-02 09:00:42.000000 auto-test-common-1.0.8/common/plugin/pytest_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      617 2023-06-02 00:42:40.000000 auto-test-common-1.0.8/common/plugin/yaml_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      443 2023-06-05 08:02:49.428099 auto-test-common-1.0.8/setup.cfg
--rw-r--r--   0 edz        (502) staff       (20)     1784 2023-06-01 00:45:28.000000 auto-test-common-1.0.8/setup.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-05 09:09:23.284946 auto-test-common-1.0.9/
+-rw-r--r--   0 edz        (502) staff       (20)      547 2023-06-05 09:09:23.285081 auto-test-common-1.0.9/PKG-INFO
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-05 09:09:23.248790 auto-test-common-1.0.9/auto_test_common.egg-info/
+-rw-r--r--   0 edz        (502) staff       (20)      547 2023-06-05 09:09:22.000000 auto-test-common-1.0.9/auto_test_common.egg-info/PKG-INFO
+-rw-r--r--   0 edz        (502) staff       (20)     1611 2023-06-05 09:09:23.000000 auto-test-common-1.0.9/auto_test_common.egg-info/SOURCES.txt
+-rw-r--r--   0 edz        (502) staff       (20)        1 2023-06-05 09:09:22.000000 auto-test-common-1.0.9/auto_test_common.egg-info/dependency_links.txt
+-rw-r--r--   0 edz        (502) staff       (20)       56 2023-06-05 09:09:22.000000 auto-test-common-1.0.9/auto_test_common.egg-info/entry_points.txt
+-rw-r--r--   0 edz        (502) staff       (20)      571 2023-06-05 09:09:22.000000 auto-test-common-1.0.9/auto_test_common.egg-info/requires.txt
+-rw-r--r--   0 edz        (502) staff       (20)        7 2023-06-05 09:09:22.000000 auto-test-common-1.0.9/auto_test_common.egg-info/top_level.txt
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-05 09:09:23.249195 auto-test-common-1.0.9/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-1.0.9/common/__init__.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-05 09:09:23.251499 auto-test-common-1.0.9/common/autotest/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-1.0.9/common/autotest/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     8490 2023-05-09 01:49:15.000000 auto-test-common-1.0.9/common/autotest/base_requests.py
+-rw-r--r--   0 edz        (502) staff       (20)     6429 2023-03-22 09:11:00.000000 auto-test-common-1.0.9/common/autotest/handle_allure.py
+-rw-r--r--   0 edz        (502) staff       (20)    10869 2023-06-02 07:24:35.000000 auto-test-common-1.0.9/common/autotest/handle_assert.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-05 09:09:23.254955 auto-test-common-1.0.9/common/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-1.0.9/common/common/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2126 2023-04-23 02:46:40.000000 auto-test-common-1.0.9/common/common/api_driver.py
+-rw-r--r--   0 edz        (502) staff       (20)     3612 2023-05-30 05:55:54.000000 auto-test-common-1.0.9/common/common/constant.py
+-rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-1.0.9/common/common/test.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-05 09:09:23.256394 auto-test-common-1.0.9/common/config/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.0.9/common/config/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2429 2022-12-01 00:35:00.000000 auto-test-common-1.0.9/common/config/config.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-05 09:09:23.260002 auto-test-common-1.0.9/common/data/
+-rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-1.0.9/common/data/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    17370 2023-05-24 07:32:32.000000 auto-test-common-1.0.9/common/data/data_process.py
+-rw-r--r--   0 edz        (502) staff       (20)     8641 2023-05-30 08:45:37.000000 auto-test-common-1.0.9/common/data/handle_common.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-05 09:09:23.265019 auto-test-common-1.0.9/common/db/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.0.9/common/db/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-1.0.9/common/db/handle_db.py
+-rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-1.0.9/common/db/handle_db_batch.py
+-rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-1.0.9/common/db/handle_mysqldb.py
+-rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-1.0.9/common/db/handle_oracle.py
+-rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-1.0.9/common/db/handle_sqlserver.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-05 09:09:23.266378 auto-test-common-1.0.9/common/driver/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2023-06-05 07:58:39.000000 auto-test-common-1.0.9/common/driver/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)      127 2023-06-05 08:02:38.000000 auto-test-common-1.0.9/common/driver/api_page.py
+-rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-05 08:02:38.000000 auto-test-common-1.0.9/common/driver/ui_page.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-05 09:09:23.272146 auto-test-common-1.0.9/common/file/
+-rw-r--r--   0 edz        (502) staff       (20)     4508 2023-04-14 00:29:00.000000 auto-test-common-1.0.9/common/file/ReadFile.py
+-rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-1.0.9/common/file/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    11473 2023-05-31 08:51:34.000000 auto-test-common-1.0.9/common/file/handle_excel.py
+-rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-1.0.9/common/file/handle_file.py
+-rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-1.0.9/common/file/handle_reques.py
+-rw-r--r--   0 edz        (502) staff       (20)     2201 2022-10-24 01:09:00.000000 auto-test-common-1.0.9/common/file/handle_system.py
+-rw-r--r--   0 edz        (502) staff       (20)      955 2023-06-01 02:02:40.000000 auto-test-common-1.0.9/common/file/handle_yaml.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-05 09:09:23.273405 auto-test-common-1.0.9/common/mq/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.0.9/common/mq/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-1.0.9/common/mq/handle_rabbit.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-05 09:09:23.277250 auto-test-common-1.0.9/common/plat/
+-rw-r--r--   0 edz        (502) staff       (20)     3543 2023-05-31 01:13:42.000000 auto-test-common-1.0.9/common/plat/ATF_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-1.0.9/common/plat/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-1.0.9/common/plat/jenkin_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     7851 2023-05-30 02:15:47.000000 auto-test-common-1.0.9/common/plat/jira_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     8129 2023-05-30 07:56:22.000000 auto-test-common-1.0.9/common/plat/mysql_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     8826 2023-05-31 01:13:42.000000 auto-test-common-1.0.9/common/plat/service_platform.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-05 09:09:23.284567 auto-test-common-1.0.9/common/plugin/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-1.0.9/common/plugin/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1330 2023-01-16 07:33:00.000000 auto-test-common-1.0.9/common/plugin/allure_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     2054 2022-07-28 02:48:00.000000 auto-test-common-1.0.9/common/plugin/assert_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     8259 2023-05-31 03:06:08.000000 auto-test-common-1.0.9/common/plugin/atf_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     6768 2023-05-15 07:47:06.000000 auto-test-common-1.0.9/common/plugin/data_bus.py
+-rw-r--r--   0 edz        (502) staff       (20)     3654 2023-05-27 02:43:55.000000 auto-test-common-1.0.9/common/plugin/data_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    12181 2023-06-05 06:08:01.000000 auto-test-common-1.0.9/common/plugin/file_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-1.0.9/common/plugin/hooks_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-1.0.9/common/plugin/pytest_playwright.py
+-rw-r--r--   0 edz        (502) staff       (20)    17687 2023-06-05 09:09:16.000000 auto-test-common-1.0.9/common/plugin/pytest_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      617 2023-06-02 00:42:40.000000 auto-test-common-1.0.9/common/plugin/yaml_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      443 2023-06-05 09:09:23.285848 auto-test-common-1.0.9/setup.cfg
+-rw-r--r--   0 edz        (502) staff       (20)     1784 2023-06-01 00:45:28.000000 auto-test-common-1.0.9/setup.py
```

### Comparing `auto-test-common-1.0.8/PKG-INFO` & `auto-test-common-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-test-common
-Version: 1.0.8
+Version: 1.0.9
 Author: shiqiang.ou
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `auto-test-common-1.0.8/auto_test_common.egg-info/PKG-INFO` & `auto-test-common-1.0.9/auto_test_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-test-common
-Version: 1.0.8
+Version: 1.0.9
 Author: shiqiang.ou
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `auto-test-common-1.0.8/auto_test_common.egg-info/SOURCES.txt` & `auto-test-common-1.0.9/auto_test_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/auto_test_common.egg-info/requires.txt` & `auto-test-common-1.0.9/auto_test_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/autotest/base_requests.py` & `auto-test-common-1.0.9/common/autotest/base_requests.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/autotest/handle_allure.py` & `auto-test-common-1.0.9/common/autotest/handle_allure.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/autotest/handle_assert.py` & `auto-test-common-1.0.9/common/autotest/handle_assert.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/common/api_driver.py` & `auto-test-common-1.0.9/common/common/api_driver.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/common/constant.py` & `auto-test-common-1.0.9/common/common/constant.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/common/test.py` & `auto-test-common-1.0.9/common/common/test.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/config/config.py` & `auto-test-common-1.0.9/common/config/config.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/data/data_process.py` & `auto-test-common-1.0.9/common/data/data_process.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/data/handle_common.py` & `auto-test-common-1.0.9/common/data/handle_common.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/db/handle_db.py` & `auto-test-common-1.0.9/common/db/handle_db.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/db/handle_db_batch.py` & `auto-test-common-1.0.9/common/db/handle_db_batch.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/db/handle_mysqldb.py` & `auto-test-common-1.0.9/common/db/handle_mysqldb.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/db/handle_oracle.py` & `auto-test-common-1.0.9/common/db/handle_oracle.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/db/handle_sqlserver.py` & `auto-test-common-1.0.9/common/db/handle_sqlserver.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/driver/ui_page.py` & `auto-test-common-1.0.9/common/driver/ui_page.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/file/ReadFile.py` & `auto-test-common-1.0.9/common/file/ReadFile.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/file/handle_excel.py` & `auto-test-common-1.0.9/common/file/handle_excel.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/file/handle_file.py` & `auto-test-common-1.0.9/common/file/handle_file.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/file/handle_reques.py` & `auto-test-common-1.0.9/common/file/handle_reques.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/file/handle_system.py` & `auto-test-common-1.0.9/common/file/handle_system.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/file/handle_yaml.py` & `auto-test-common-1.0.9/common/file/handle_yaml.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/mq/handle_rabbit.py` & `auto-test-common-1.0.9/common/mq/handle_rabbit.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/plat/ATF_platform.py` & `auto-test-common-1.0.9/common/plat/ATF_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/plat/jenkin_platform.py` & `auto-test-common-1.0.9/common/plat/jenkin_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/plat/jira_platform.py` & `auto-test-common-1.0.9/common/plat/jira_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/plat/mysql_platform.py` & `auto-test-common-1.0.9/common/plat/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/plat/service_platform.py` & `auto-test-common-1.0.9/common/plat/service_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/plugin/allure_plugin.py` & `auto-test-common-1.0.9/common/plugin/allure_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/plugin/assert_plugin.py` & `auto-test-common-1.0.9/common/plugin/assert_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/plugin/atf_plugin.py` & `auto-test-common-1.0.9/common/plugin/atf_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/plugin/data_bus.py` & `auto-test-common-1.0.9/common/plugin/data_bus.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/plugin/data_plugin.py` & `auto-test-common-1.0.9/common/plugin/data_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/plugin/file_plugin.py` & `auto-test-common-1.0.9/common/plugin/file_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/plugin/hooks_plugin.py` & `auto-test-common-1.0.9/common/plugin/hooks_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/plugin/pytest_playwright.py` & `auto-test-common-1.0.9/common/plugin/pytest_playwright.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/common/plugin/pytest_plugin.py` & `auto-test-common-1.0.9/common/plugin/pytest_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,15 +314,14 @@
                             isRun = False
                         else:
                             if run['status'] == '执行中':
                                 logger.info(f"用例信息：{str(run)} 执行状态:用例执行中")
                                 isRun = True
                             else:
                                 logger.info(f"用例信息：{str(run)} 执行状态:用例状态不在执行中")
-                                isRun = False
             else:
                 _name = _caseTitleList[0]
                 run = ATFPlatForm.getCaseRun(_name)
                 if run['caserunid'] != '00000':
                     isRun = True
         else:
             isRun = True
```

### Comparing `auto-test-common-1.0.8/common/plugin/yaml_plugin.py` & `auto-test-common-1.0.9/common/plugin/yaml_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.8/setup.py` & `auto-test-common-1.0.9/setup.py`

 * *Files identical despite different names*

