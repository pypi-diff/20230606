# Comparing `tmp/cdk-opinionated-constructs-2.1.3.tar.gz` & `tmp/cdk-opinionated-constructs-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-opinionated-constructs-2.1.3.tar", last modified: Mon May 22 07:45:48 2023, max compression
+gzip compressed data, was "cdk-opinionated-constructs-2.1.4.tar", last modified: Mon Jun  5 22:23:51 2023, max compression
```

## Comparing `cdk-opinionated-constructs-2.1.3.tar` & `cdk-opinionated-constructs-2.1.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-05-22 07:45:48.593133 cdk-opinionated-constructs-2.1.3/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1071 2022-11-05 20:03:58.000000 cdk-opinionated-constructs-2.1.3/LICENSE
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      340 2023-05-22 07:45:48.593237 cdk-opinionated-constructs-2.1.3/PKG-INFO
--rw-r--r--   0 tomaszszuster   (501) staff       (20)    27443 2023-04-18 12:21:33.000000 cdk-opinionated-constructs-2.1.3/README.md
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-05-22 07:45:48.504099 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)       50 2022-11-05 21:10:53.000000 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     4879 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/alb.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2235 2022-11-20 14:04:19.000000 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/ecr.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     8661 2023-04-20 10:19:32.000000 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/lmb.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     5811 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/nlb.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     4643 2022-12-24 14:23:29.000000 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/rds_instance.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3325 2023-05-19 08:53:43.000000 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/s3.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1464 2022-11-22 22:16:47.000000 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/sns.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)    12369 2023-05-22 07:42:39.000000 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/wafv2.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-05-22 07:45:48.592880 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs.egg-info/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      340 2023-05-22 07:45:48.000000 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs.egg-info/PKG-INFO
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1221 2023-05-22 07:45:48.000000 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        1 2023-05-22 07:45:48.000000 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)       89 2023-05-22 07:45:48.000000 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs.egg-info/requires.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)       32 2023-05-22 07:45:48.000000 cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs.egg-info/top_level.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3649 2023-05-22 07:45:48.593990 cdk-opinionated-constructs-2.1.3/setup.cfg
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      761 2023-05-22 07:43:04.000000 cdk-opinionated-constructs-2.1.3/setup.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-05-22 07:45:48.509090 cdk-opinionated-constructs-2.1.3/test/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.1.3/test/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1781 2023-04-20 10:28:48.000000 cdk-opinionated-constructs-2.1.3/test/app.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-05-22 07:45:48.538517 cdk-opinionated-constructs-2.1.3/test/stacks/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.1.3/test/stacks/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2322 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.3/test/stacks/alb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1012 2022-11-20 14:04:19.000000 cdk-opinionated-constructs-2.1.3/test/stacks/ecr_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3241 2023-04-20 10:37:59.000000 cdk-opinionated-constructs-2.1.3/test/stacks/lmb_docker_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3590 2022-11-25 10:57:28.000000 cdk-opinionated-constructs-2.1.3/test/stacks/lmb_monitoring_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2810 2023-04-20 10:37:59.000000 cdk-opinionated-constructs-2.1.3/test/stacks/lmb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2225 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.3/test/stacks/nlb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3290 2022-12-24 14:23:29.000000 cdk-opinionated-constructs-2.1.3/test/stacks/rds_mysql_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3304 2022-12-24 14:23:29.000000 cdk-opinionated-constructs-2.1.3/test/stacks/rds_postgresql_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1630 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.3/test/stacks/s3_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1108 2022-11-22 22:16:47.000000 cdk-opinionated-constructs-2.1.3/test/stacks/sns_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2593 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.3/test/stacks/wafv2_stack.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-05-22 07:45:48.587443 cdk-opinionated-constructs-2.1.3/test/unit/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.1.3/test/unit/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1102 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.3/test/unit/test_alb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      701 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.3/test/unit/test_ecr_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1100 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.3/test/unit/test_lmb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      852 2023-05-19 08:53:43.000000 cdk-opinionated-constructs-2.1.3/test/unit/test_s3_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      685 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.3/test/unit/test_sns_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1921 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.3/test/unit/test_wafv2_stack.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-06-05 22:23:51.846311 cdk-opinionated-constructs-2.1.4/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1071 2022-11-05 20:03:58.000000 cdk-opinionated-constructs-2.1.4/LICENSE
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      340 2023-06-05 22:23:51.846384 cdk-opinionated-constructs-2.1.4/PKG-INFO
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)    27651 2023-05-22 07:55:27.000000 cdk-opinionated-constructs-2.1.4/README.md
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-06-05 22:23:51.796326 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)       50 2022-11-05 21:10:53.000000 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     4879 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/alb.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2235 2022-11-20 14:04:19.000000 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/ecr.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     8661 2023-04-20 10:19:32.000000 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/lmb.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     5811 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/nlb.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     4643 2022-12-24 14:23:29.000000 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/rds_instance.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3325 2023-05-19 08:53:43.000000 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/s3.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1464 2022-11-22 22:16:47.000000 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/sns.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)    12369 2023-05-22 07:49:31.000000 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/wafv2.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-06-05 22:23:51.846041 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs.egg-info/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      340 2023-06-05 22:23:51.000000 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1221 2023-06-05 22:23:51.000000 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        1 2023-06-05 22:23:51.000000 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)       88 2023-06-05 22:23:51.000000 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs.egg-info/requires.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)       32 2023-06-05 22:23:51.000000 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs.egg-info/top_level.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3649 2023-06-05 22:23:51.846978 cdk-opinionated-constructs-2.1.4/setup.cfg
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      760 2023-06-05 22:23:38.000000 cdk-opinionated-constructs-2.1.4/setup.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-06-05 22:23:51.803569 cdk-opinionated-constructs-2.1.4/test/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.1.4/test/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1781 2023-04-20 10:28:48.000000 cdk-opinionated-constructs-2.1.4/test/app.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-06-05 22:23:51.819347 cdk-opinionated-constructs-2.1.4/test/stacks/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.1.4/test/stacks/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2322 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.4/test/stacks/alb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1012 2022-11-20 14:04:19.000000 cdk-opinionated-constructs-2.1.4/test/stacks/ecr_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3241 2023-04-20 10:37:59.000000 cdk-opinionated-constructs-2.1.4/test/stacks/lmb_docker_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3590 2022-11-25 10:57:28.000000 cdk-opinionated-constructs-2.1.4/test/stacks/lmb_monitoring_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2810 2023-04-20 10:37:59.000000 cdk-opinionated-constructs-2.1.4/test/stacks/lmb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2225 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.4/test/stacks/nlb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3290 2022-12-24 14:23:29.000000 cdk-opinionated-constructs-2.1.4/test/stacks/rds_mysql_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3304 2022-12-24 14:23:29.000000 cdk-opinionated-constructs-2.1.4/test/stacks/rds_postgresql_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1630 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.4/test/stacks/s3_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1108 2022-11-22 22:16:47.000000 cdk-opinionated-constructs-2.1.4/test/stacks/sns_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2593 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.4/test/stacks/wafv2_stack.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-06-05 22:23:51.840314 cdk-opinionated-constructs-2.1.4/test/unit/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.1.4/test/unit/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1102 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.4/test/unit/test_alb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      701 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.4/test/unit/test_ecr_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1100 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.4/test/unit/test_lmb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      852 2023-05-19 08:53:43.000000 cdk-opinionated-constructs-2.1.4/test/unit/test_s3_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      685 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.4/test/unit/test_sns_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1921 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.4/test/unit/test_wafv2_stack.py
```

### Comparing `cdk-opinionated-constructs-2.1.3/LICENSE` & `cdk-opinionated-constructs-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.3/README.md` & `cdk-opinionated-constructs-2.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+[![auto-merge](https://github.com/airmonitor/cdk-opinionated-constructs/actions/workflows/auto_merge.yml/badge.svg)](https://github.com/airmonitor/cdk-opinionated-constructs/actions/workflows/auto_merge.yml)
 [![tests](https://github.com/airmonitor/cdk-opinionated-constructs/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/airmonitor/cdk-opinionated-constructs/actions/workflows/tests.yml)
 
 # cdk-opinionated-constructs
 CDK constructs with added security configuration
 
 ## S3 Bucket example:
 ```python
```

### Comparing `cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/alb.py` & `cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/alb.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/ecr.py` & `cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/ecr.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/lmb.py` & `cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/lmb.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/nlb.py` & `cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/nlb.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/rds_instance.py` & `cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/rds_instance.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/s3.py` & `cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/s3.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/sns.py` & `cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/sns.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs/wafv2.py` & `cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/wafv2.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.3/cdk_opinionated_constructs.egg-info/SOURCES.txt` & `cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.3/setup.cfg` & `cdk-opinionated-constructs-2.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.3/test/app.py` & `cdk-opinionated-constructs-2.1.4/test/app.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.3/test/stacks/alb_stack.py` & `cdk-opinionated-constructs-2.1.4/test/stacks/alb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.3/test/stacks/ecr_stack.py` & `cdk-opinionated-constructs-2.1.4/test/stacks/ecr_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.3/test/stacks/lmb_docker_stack.py` & `cdk-opinionated-constructs-2.1.4/test/stacks/lmb_docker_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.3/test/stacks/lmb_monitoring_stack.py` & `cdk-opinionated-constructs-2.1.4/test/stacks/lmb_monitoring_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.3/test/stacks/lmb_stack.py` & `cdk-opinionated-constructs-2.1.4/test/stacks/lmb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.3/test/stacks/nlb_stack.py` & `cdk-opinionated-constructs-2.1.4/test/stacks/nlb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.3/test/stacks/rds_mysql_stack.py` & `cdk-opinionated-constructs-2.1.4/test/stacks/rds_mysql_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.3/test/stacks/rds_postgresql_stack.py` & `cdk-opinionated-constructs-2.1.4/test/stacks/rds_postgresql_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.3/test/stacks/s3_stack.py` & `cdk-opinionated-constructs-2.1.4/test/stacks/s3_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.3/test/stacks/sns_stack.py` & `cdk-opinionated-constructs-2.1.4/test/stacks/sns_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.3/test/stacks/wafv2_stack.py` & `cdk-opinionated-constructs-2.1.4/test/stacks/wafv2_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.3/test/unit/test_alb_stack.py` & `cdk-opinionated-constructs-2.1.4/test/unit/test_alb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.3/test/unit/test_ecr_stack.py` & `cdk-opinionated-constructs-2.1.4/test/unit/test_ecr_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.3/test/unit/test_lmb_stack.py` & `cdk-opinionated-constructs-2.1.4/test/unit/test_lmb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.3/test/unit/test_s3_stack.py` & `cdk-opinionated-constructs-2.1.4/test/unit/test_s3_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.3/test/unit/test_sns_stack.py` & `cdk-opinionated-constructs-2.1.4/test/unit/test_sns_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.3/test/unit/test_wafv2_stack.py` & `cdk-opinionated-constructs-2.1.4/test/unit/test_wafv2_stack.py`

 * *Files identical despite different names*

