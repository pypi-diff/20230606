# Comparing `tmp/spotinst-sdk2-2.1.8.tar.gz` & `tmp/spotinst-sdk2-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotinst-sdk2-2.1.8.tar", last modified: Wed Jun 23 15:33:47 2021, max compression
+gzip compressed data, was "spotinst-sdk2-2.1.9.tar", last modified: Thu Jun 24 12:50:34 2021, max compression
```

## Comparing `spotinst-sdk2-2.1.8.tar` & `spotinst-sdk2-2.1.9.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-06-23 15:33:47.716305 spotinst-sdk2-2.1.8/
--rwxr-xr-x   0 cadurikatzav   (502) staff       (20)    11356 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/LICENSE
--rwxr-xr-x   0 cadurikatzav   (502) staff       (20)       43 2021-01-17 21:52:54.000000 spotinst-sdk2-2.1.8/MANIFEST.in
--rw-r--r--   0 cadurikatzav   (502) staff       (20)      751 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/NOTICE.md
--rw-r--r--   0 cadurikatzav   (502) staff       (20)     8155 2021-06-23 15:33:47.716478 spotinst-sdk2-2.1.8/PKG-INFO
--rwxr-xr-x   0 cadurikatzav   (502) staff       (20)     6244 2021-06-23 15:19:07.000000 spotinst-sdk2-2.1.8/README.md
--rwxr-xr-x   0 cadurikatzav   (502) staff       (20)       63 2021-06-23 15:33:47.716935 spotinst-sdk2-2.1.8/setup.cfg
--rwxr-xr-x   0 cadurikatzav   (502) staff       (20)     2561 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/setup.py
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-06-23 15:33:47.699826 spotinst-sdk2-2.1.8/spotinst_sdk2/
--rwxr-xr-x   0 cadurikatzav   (502) staff       (20)     2835 2021-06-23 15:19:07.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/__init__.py
--rw-r--r--   0 cadurikatzav   (502) staff       (20)    11482 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/client.py
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-06-23 15:33:47.701987 spotinst-sdk2-2.1.8/spotinst_sdk2/clients/
--rw-r--r--   0 cadurikatzav   (502) staff       (20)        0 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/clients/__init__.py
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-06-23 15:33:47.702327 spotinst-sdk2-2.1.8/spotinst_sdk2/clients/admin/
--rw-r--r--   0 cadurikatzav   (502) staff       (20)     9083 2021-06-23 15:19:07.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/clients/admin/__init__.py
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-06-23 15:33:47.703023 spotinst-sdk2-2.1.8/spotinst_sdk2/clients/elastigroup/
--rw-r--r--   0 cadurikatzav   (502) staff       (20)    69145 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/clients/elastigroup/__init__.py
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-06-23 15:33:47.704442 spotinst-sdk2-2.1.8/spotinst_sdk2/clients/functions/
--rw-r--r--   0 cadurikatzav   (502) staff       (20)     3217 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/clients/functions/__init__.py
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-06-23 15:33:47.704918 spotinst-sdk2-2.1.8/spotinst_sdk2/clients/mcs/
--rw-r--r--   0 cadurikatzav   (502) staff       (20)      935 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/clients/mcs/__init__.py
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-06-23 15:33:47.705285 spotinst-sdk2-2.1.8/spotinst_sdk2/clients/mlb/
--rw-r--r--   0 cadurikatzav   (502) staff       (20)    28337 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/clients/mlb/__init__.py
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-06-23 15:33:47.705830 spotinst-sdk2-2.1.8/spotinst_sdk2/clients/mrscaler/
--rw-r--r--   0 cadurikatzav   (502) staff       (20)     6739 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/clients/mrscaler/__init__.py
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-06-23 15:33:47.706249 spotinst-sdk2-2.1.8/spotinst_sdk2/clients/ocean/
--rw-r--r--   0 cadurikatzav   (502) staff       (20)     4100 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/clients/ocean/__init__.py
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-06-23 15:33:47.706710 spotinst-sdk2-2.1.8/spotinst_sdk2/clients/subscription/
--rw-r--r--   0 cadurikatzav   (502) staff       (20)     3947 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/clients/subscription/__init__.py
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-06-23 15:33:47.707202 spotinst-sdk2-2.1.8/spotinst_sdk2/models/
--rw-r--r--   0 cadurikatzav   (502) staff       (20)        0 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/models/__init__.py
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-06-23 15:33:47.708055 spotinst-sdk2-2.1.8/spotinst_sdk2/models/admin/
--rw-r--r--   0 cadurikatzav   (502) staff       (20)        0 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/models/admin/__init__.py
--rw-r--r--   0 cadurikatzav   (502) staff       (20)      548 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/models/admin/user_mapping.py
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-06-23 15:33:47.708714 spotinst-sdk2-2.1.8/spotinst_sdk2/models/elastigroup/
--rw-r--r--   0 cadurikatzav   (502) staff       (20)        0 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/models/elastigroup/__init__.py
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-06-23 15:33:47.711063 spotinst-sdk2-2.1.8/spotinst_sdk2/models/elastigroup/aws/
--rwxr-xr-x   0 cadurikatzav   (502) staff       (20)    37739 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/models/elastigroup/aws/__init__.py
--rw-r--r--   0 cadurikatzav   (502) staff       (20)      570 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/models/elastigroup/aws/asg.py
--rw-r--r--   0 cadurikatzav   (502) staff       (20)     1075 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/models/elastigroup/aws/deployment.py
--rw-r--r--   0 cadurikatzav   (502) staff       (20)      837 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/models/elastigroup/aws/deployment_action.py
--rw-r--r--   0 cadurikatzav   (502) staff       (20)     1261 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/models/elastigroup/aws/stateful.py
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-06-23 15:33:47.711866 spotinst-sdk2-2.1.8/spotinst_sdk2/models/elastigroup/azure/
--rw-r--r--   0 cadurikatzav   (502) staff       (20)    15596 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/models/elastigroup/azure/__init__.py
--rw-r--r--   0 cadurikatzav   (502) staff       (20)     1440 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/models/elastigroup/azure/task.py
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-06-23 15:33:47.713015 spotinst-sdk2-2.1.8/spotinst_sdk2/models/elastigroup/gcp/
--rw-r--r--   0 cadurikatzav   (502) staff       (20)    13950 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/models/elastigroup/gcp/__init__.py
--rw-r--r--   0 cadurikatzav   (502) staff       (20)     1283 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/models/elastigroup/gcp/gke.py
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-06-23 15:33:47.713581 spotinst-sdk2-2.1.8/spotinst_sdk2/models/functions/
--rw-r--r--   0 cadurikatzav   (502) staff       (20)     3690 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/models/functions/__init__.py
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-06-23 15:33:47.713958 spotinst-sdk2-2.1.8/spotinst_sdk2/models/mlb/
--rw-r--r--   0 cadurikatzav   (502) staff       (20)     7381 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/models/mlb/__init__.py
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-06-23 15:33:47.714520 spotinst-sdk2-2.1.8/spotinst_sdk2/models/mrscaler/
--rw-r--r--   0 cadurikatzav   (502) staff       (20)        0 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/models/mrscaler/__init__.py
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-06-23 15:33:47.714787 spotinst-sdk2-2.1.8/spotinst_sdk2/models/mrscaler/aws/
--rw-r--r--   0 cadurikatzav   (502) staff       (20)    10804 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/models/mrscaler/aws/__init__.py
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-06-23 15:33:47.715280 spotinst-sdk2-2.1.8/spotinst_sdk2/models/ocean/
--rw-r--r--   0 cadurikatzav   (502) staff       (20)        0 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/models/ocean/__init__.py
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-06-23 15:33:47.715543 spotinst-sdk2-2.1.8/spotinst_sdk2/models/ocean/aws/
--rw-r--r--   0 cadurikatzav   (502) staff       (20)     4139 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/models/ocean/aws/__init__.py
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-06-23 15:33:47.715936 spotinst-sdk2-2.1.8/spotinst_sdk2/models/subscription/
--rw-r--r--   0 cadurikatzav   (502) staff       (20)      737 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/models/subscription/__init__.py
--rw-r--r--   0 cadurikatzav   (502) staff       (20)     1829 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/session.py
--rwxr-xr-x   0 cadurikatzav   (502) staff       (20)       22 2021-06-14 11:34:51.000000 spotinst-sdk2-2.1.8/spotinst_sdk2/version.py
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-06-23 15:33:47.701553 spotinst-sdk2-2.1.8/spotinst_sdk2.egg-info/
--rw-r--r--   0 cadurikatzav   (502) staff       (20)     8155 2021-06-23 15:33:47.000000 spotinst-sdk2-2.1.8/spotinst_sdk2.egg-info/PKG-INFO
--rw-r--r--   0 cadurikatzav   (502) staff       (20)     1610 2021-06-23 15:33:47.000000 spotinst-sdk2-2.1.8/spotinst_sdk2.egg-info/SOURCES.txt
--rw-r--r--   0 cadurikatzav   (502) staff       (20)        1 2021-06-23 15:33:47.000000 spotinst-sdk2-2.1.8/spotinst_sdk2.egg-info/dependency_links.txt
--rw-r--r--   0 cadurikatzav   (502) staff       (20)       16 2021-06-23 15:33:47.000000 spotinst-sdk2-2.1.8/spotinst_sdk2.egg-info/requires.txt
--rw-r--r--   0 cadurikatzav   (502) staff       (20)       14 2021-06-23 15:33:47.000000 spotinst-sdk2-2.1.8/spotinst_sdk2.egg-info/top_level.txt
+drwxr-xr-x   0 liran      (502) staff       (20)        0 2021-06-24 12:50:34.081469 spotinst-sdk2-2.1.9/
+-rwxr-xr-x   0 liran      (502) staff       (20)    11356 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/LICENSE
+-rwxr-xr-x   0 liran      (502) staff       (20)       43 2020-12-01 16:58:05.000000 spotinst-sdk2-2.1.9/MANIFEST.in
+-rw-r--r--   0 liran      (502) staff       (20)      751 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/NOTICE.md
+-rw-r--r--   0 liran      (502) staff       (20)     9312 2021-06-24 12:50:34.081838 spotinst-sdk2-2.1.9/PKG-INFO
+-rwxr-xr-x   0 liran      (502) staff       (20)     7049 2021-06-24 12:47:03.000000 spotinst-sdk2-2.1.9/README.md
+-rwxr-xr-x   0 liran      (502) staff       (20)       63 2021-06-24 12:50:34.083041 spotinst-sdk2-2.1.9/setup.cfg
+-rwxr-xr-x   0 liran      (502) staff       (20)     2561 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/setup.py
+drwxr-xr-x   0 liran      (502) staff       (20)        0 2021-06-24 12:50:34.050000 spotinst-sdk2-2.1.9/spotinst_sdk2/
+-rwxr-xr-x   0 liran      (502) staff       (20)     2835 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/__init__.py
+-rw-r--r--   0 liran      (502) staff       (20)    11482 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/client.py
+drwxr-xr-x   0 liran      (502) staff       (20)        0 2021-06-24 12:50:34.055237 spotinst-sdk2-2.1.9/spotinst_sdk2/clients/
+-rw-r--r--   0 liran      (502) staff       (20)        0 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/clients/__init__.py
+drwxr-xr-x   0 liran      (502) staff       (20)        0 2021-06-24 12:50:34.055779 spotinst-sdk2-2.1.9/spotinst_sdk2/clients/admin/
+-rw-r--r--   0 liran      (502) staff       (20)     9083 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/clients/admin/__init__.py
+drwxr-xr-x   0 liran      (502) staff       (20)        0 2021-06-24 12:50:34.057024 spotinst-sdk2-2.1.9/spotinst_sdk2/clients/elastigroup/
+-rw-r--r--   0 liran      (502) staff       (20)    69145 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/clients/elastigroup/__init__.py
+drwxr-xr-x   0 liran      (502) staff       (20)        0 2021-06-24 12:50:34.058533 spotinst-sdk2-2.1.9/spotinst_sdk2/clients/functions/
+-rw-r--r--   0 liran      (502) staff       (20)     3217 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/clients/functions/__init__.py
+drwxr-xr-x   0 liran      (502) staff       (20)        0 2021-06-24 12:50:34.059471 spotinst-sdk2-2.1.9/spotinst_sdk2/clients/mcs/
+-rw-r--r--   0 liran      (502) staff       (20)      935 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/clients/mcs/__init__.py
+drwxr-xr-x   0 liran      (502) staff       (20)        0 2021-06-24 12:50:34.060527 spotinst-sdk2-2.1.9/spotinst_sdk2/clients/mlb/
+-rw-r--r--   0 liran      (502) staff       (20)    28337 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/clients/mlb/__init__.py
+drwxr-xr-x   0 liran      (502) staff       (20)        0 2021-06-24 12:50:34.062366 spotinst-sdk2-2.1.9/spotinst_sdk2/clients/mrscaler/
+-rw-r--r--   0 liran      (502) staff       (20)     6739 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/clients/mrscaler/__init__.py
+drwxr-xr-x   0 liran      (502) staff       (20)        0 2021-06-24 12:50:34.063360 spotinst-sdk2-2.1.9/spotinst_sdk2/clients/ocean/
+-rw-r--r--   0 liran      (502) staff       (20)     4100 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/clients/ocean/__init__.py
+drwxr-xr-x   0 liran      (502) staff       (20)        0 2021-06-24 12:50:34.064150 spotinst-sdk2-2.1.9/spotinst_sdk2/clients/subscription/
+-rw-r--r--   0 liran      (502) staff       (20)     3947 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/clients/subscription/__init__.py
+drwxr-xr-x   0 liran      (502) staff       (20)        0 2021-06-24 12:50:34.065145 spotinst-sdk2-2.1.9/spotinst_sdk2/models/
+-rw-r--r--   0 liran      (502) staff       (20)        0 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/models/__init__.py
+drwxr-xr-x   0 liran      (502) staff       (20)        0 2021-06-24 12:50:34.066358 spotinst-sdk2-2.1.9/spotinst_sdk2/models/admin/
+-rw-r--r--   0 liran      (502) staff       (20)        0 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/models/admin/__init__.py
+-rw-r--r--   0 liran      (502) staff       (20)      548 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/models/admin/user_mapping.py
+drwxr-xr-x   0 liran      (502) staff       (20)        0 2021-06-24 12:50:34.067192 spotinst-sdk2-2.1.9/spotinst_sdk2/models/elastigroup/
+-rw-r--r--   0 liran      (502) staff       (20)        0 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/models/elastigroup/__init__.py
+drwxr-xr-x   0 liran      (502) staff       (20)        0 2021-06-24 12:50:34.071737 spotinst-sdk2-2.1.9/spotinst_sdk2/models/elastigroup/aws/
+-rwxr-xr-x   0 liran      (502) staff       (20)    37739 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/models/elastigroup/aws/__init__.py
+-rw-r--r--   0 liran      (502) staff       (20)      570 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/models/elastigroup/aws/asg.py
+-rw-r--r--   0 liran      (502) staff       (20)     1075 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/models/elastigroup/aws/deployment.py
+-rw-r--r--   0 liran      (502) staff       (20)      837 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/models/elastigroup/aws/deployment_action.py
+-rw-r--r--   0 liran      (502) staff       (20)     1261 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/models/elastigroup/aws/stateful.py
+drwxr-xr-x   0 liran      (502) staff       (20)        0 2021-06-24 12:50:34.073320 spotinst-sdk2-2.1.9/spotinst_sdk2/models/elastigroup/azure/
+-rw-r--r--   0 liran      (502) staff       (20)    15596 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/models/elastigroup/azure/__init__.py
+-rw-r--r--   0 liran      (502) staff       (20)     1440 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/models/elastigroup/azure/task.py
+drwxr-xr-x   0 liran      (502) staff       (20)        0 2021-06-24 12:50:34.075379 spotinst-sdk2-2.1.9/spotinst_sdk2/models/elastigroup/gcp/
+-rw-r--r--   0 liran      (502) staff       (20)    13950 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/models/elastigroup/gcp/__init__.py
+-rw-r--r--   0 liran      (502) staff       (20)     1283 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/models/elastigroup/gcp/gke.py
+drwxr-xr-x   0 liran      (502) staff       (20)        0 2021-06-24 12:50:34.076148 spotinst-sdk2-2.1.9/spotinst_sdk2/models/functions/
+-rw-r--r--   0 liran      (502) staff       (20)     3690 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/models/functions/__init__.py
+drwxr-xr-x   0 liran      (502) staff       (20)        0 2021-06-24 12:50:34.077019 spotinst-sdk2-2.1.9/spotinst_sdk2/models/mlb/
+-rw-r--r--   0 liran      (502) staff       (20)     7381 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/models/mlb/__init__.py
+drwxr-xr-x   0 liran      (502) staff       (20)        0 2021-06-24 12:50:34.077821 spotinst-sdk2-2.1.9/spotinst_sdk2/models/mrscaler/
+-rw-r--r--   0 liran      (502) staff       (20)        0 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/models/mrscaler/__init__.py
+drwxr-xr-x   0 liran      (502) staff       (20)        0 2021-06-24 12:50:34.078395 spotinst-sdk2-2.1.9/spotinst_sdk2/models/mrscaler/aws/
+-rw-r--r--   0 liran      (502) staff       (20)    10804 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/models/mrscaler/aws/__init__.py
+drwxr-xr-x   0 liran      (502) staff       (20)        0 2021-06-24 12:50:34.079140 spotinst-sdk2-2.1.9/spotinst_sdk2/models/ocean/
+-rw-r--r--   0 liran      (502) staff       (20)        0 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/models/ocean/__init__.py
+drwxr-xr-x   0 liran      (502) staff       (20)        0 2021-06-24 12:50:34.079627 spotinst-sdk2-2.1.9/spotinst_sdk2/models/ocean/aws/
+-rw-r--r--   0 liran      (502) staff       (20)     4139 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/models/ocean/aws/__init__.py
+drwxr-xr-x   0 liran      (502) staff       (20)        0 2021-06-24 12:50:34.080548 spotinst-sdk2-2.1.9/spotinst_sdk2/models/subscription/
+-rw-r--r--   0 liran      (502) staff       (20)      737 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/models/subscription/__init__.py
+-rw-r--r--   0 liran      (502) staff       (20)     2409 2021-06-24 12:45:34.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/session.py
+-rwxr-xr-x   0 liran      (502) staff       (20)       22 2021-06-24 12:45:31.000000 spotinst-sdk2-2.1.9/spotinst_sdk2/version.py
+drwxr-xr-x   0 liran      (502) staff       (20)        0 2021-06-24 12:50:34.054548 spotinst-sdk2-2.1.9/spotinst_sdk2.egg-info/
+-rw-r--r--   0 liran      (502) staff       (20)     9312 2021-06-24 12:50:33.000000 spotinst-sdk2-2.1.9/spotinst_sdk2.egg-info/PKG-INFO
+-rw-r--r--   0 liran      (502) staff       (20)     1610 2021-06-24 12:50:33.000000 spotinst-sdk2-2.1.9/spotinst_sdk2.egg-info/SOURCES.txt
+-rw-r--r--   0 liran      (502) staff       (20)        1 2021-06-24 12:50:33.000000 spotinst-sdk2-2.1.9/spotinst_sdk2.egg-info/dependency_links.txt
+-rw-r--r--   0 liran      (502) staff       (20)       16 2021-06-24 12:50:33.000000 spotinst-sdk2-2.1.9/spotinst_sdk2.egg-info/requires.txt
+-rw-r--r--   0 liran      (502) staff       (20)       14 2021-06-24 12:50:33.000000 spotinst-sdk2-2.1.9/spotinst_sdk2.egg-info/top_level.txt
```

### Comparing `spotinst-sdk2-2.1.8/LICENSE` & `spotinst-sdk2-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.1.8/NOTICE.md` & `spotinst-sdk2-2.1.9/NOTICE.md`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.1.8/PKG-INFO` & `spotinst-sdk2-2.1.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-sdk2
-Version: 2.1.8
+Version: 2.1.9
 Summary: A Python SDK for Spotinst
 Home-page: https://github.com/spotinst/spotinst-sdk-python
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Description: [![Build Status](https://travis-ci.org/spotinst/spotinst-sdk-python.svg?branch=v2)](https://travis-ci.org/spotinst/spotinst-sdk-python)
         [![Coverage Status](https://coveralls.io/repos/github/spotinst/spotinst-sdk-python/badge.svg?branch=v2)](https://coveralls.io/github/spotinst/spotinst-sdk-python?branch=master)
@@ -58,15 +58,15 @@
         client.create_ocean_cluster(ocean=ocean)
         ```
         
         In the [SDK Client documentation](./docs/clients/) you can view what methods are supported by each client. <br>
         For information on what models are supported checkout the [SDK Model documentation](./docs/models/). <br>
         More examples can be found in the [SDK Examples Documentation](./docs/examples/). <br>
         
-        ## Contents
+        ## Table of Contents
         
         - [Installation](#installation)
         - [Authentication](#authentication)
         - [Setup Clients](#setup-clients)
         - [Documentation](#documentation)
         - [Getting Help](#getting-help)
         - [Community](#community)
@@ -76,43 +76,87 @@
         
         ```bash
         pip install --upgrade spotinst-sdk2
         ```
         
         ## Authentication
         
-        The mechanism in which the sdk looks for credentials is to search through a list of possible locations and stop as soon as it finds credentials. The order in which the sdk searches for credentials is:
+        The mechanism in which the SDK looks for credentials is to search through a list of possible locations and stop as soon as it finds credentials. The order in which the SDK searches for credentials is:
         
-        1. Passing credentials as parameters to the `SpotinstSession()` constructor
+        1. Passing credentials as parameters when creating a `SpotinstSession` object:
         
         ```python
-        session = SpotinstSession(auth_token='token', account_id='act-123')
+        session = SpotinstSession(auth_token='foo', account_id='bar')
         ```
         
-        2. Fetching the account and token from environment variables under `SPOTINST_ACCOUNT` & `SPOTINST_TOKEN`.
-        If you choose to not pass your credentials directly you configure a credentials file, this file should be a valid `.yml` file. The default shared credential file location is `~/.spotinst/credentials` and the default profile is `default`
+        2. Environment variables:
+        
+        ```sh
+        export SPOTINST_TOKEN=foo
+        export SPOTINST_ACCOUNT=bar
+        ```
+        
+        3. Shared credentials file:
+        
+        - The shared credentials file has a default location of `~/.spotinst/credentials`. This file is an INI formatted file with section names corresponding to profiles. With each section, two configuration variables can be specified: `token`, `account`. These are the only supported values in the shared credential file.
+        
+        - Below is a minimal example of the shared credentials file:
+        
+        ```ini
+        [default]
+        token   = foo
+        account = bar
+        ```
+        
+        - The shared credentials file also supports the concept of profiles. Profiles represent logical groups of configuration. The shared credential file can have multiple profiles:
+        
+        ```ini
+        [default]
+        token   = foo
+        account = bar
+        
+        [dev]
+        token   = foo2
+        account = bar2
+        
+        [prod]
+        token   = foo3
+        account = bar3
+        ```
+        
+        - You can configure your Spot credentials using the `spotctl configure` command. For more information, see the `spotctl` [Getting Started](https://github.com/spotinst/spotctl#getting-started).
+        
+        - To maintain compatibility with previous SDK versions, the file can also be in YAML format:
         
         ```yaml
-        default: #profile
-          token: $defaul_spotinst_token
-          account: $default_spotinst-account-id
-        my_profile:
-          token: $my_spotinst_token
-          account: $my_spotinst-account-id
+        default:
+          token: foo
+          account: bar
+          
+        dev:
+          token: foo2
+          account: bar2
+          
+        prod:
+          token: foo3
+          account: bar3
         ```
         
-        3. You can overwrite the credentials file location and the profile used as parameters in the `SpotinstSession()` constructor
+        - You can change the location of the credentials file and the profile used by setting the `SPOTINST_SHARED_CREDENTIALS_FILE` and/or `SPOTINST_PROFILE` environment variables:
         
-        ```python
-        session = SpotinstSession(credentials_file='/path/to/file', profile='my_profile')
+        ```sh
+        export SPOTINST_SHARED_CREDENTIALS_FILE=/path/to/credentials_file
+        export SPOTINST_PROFILE=dev
         ```
         
-        4. You can overwrite the credentials file location and the profile used as environment variables `SPOTINST_PROFILE` and/or `SPOTINST_SHARED_CREDENTIALS_FILE`
+        - Passing the credentials file location and the profile used as parameters when creating a `SpotinstSession` object:
         
-        5. Fetching from the default location with the default profile
+        ```python
+        session = SpotinstSession(credentials_file='/path/to/credentials_file', profile='dev')
+        ```
           
         ## Setup Clients
         
         After a session is created you can use the session object to create clients. Clients are used to make request to the different services that Spotinsts has to offer. To create a client simply use the method `client` from the session object and pass in the string of the client you wish to create. Here is an example:
         
         ```python
         session = SpotinstSession()
```

### Comparing `spotinst-sdk2-2.1.8/README.md` & `spotinst-sdk2-2.1.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 client.create_ocean_cluster(ocean=ocean)
 ```
 
 In the [SDK Client documentation](./docs/clients/) you can view what methods are supported by each client. <br>
 For information on what models are supported checkout the [SDK Model documentation](./docs/models/). <br>
 More examples can be found in the [SDK Examples Documentation](./docs/examples/). <br>
 
-## Contents
+## Table of Contents
 
 - [Installation](#installation)
 - [Authentication](#authentication)
 - [Setup Clients](#setup-clients)
 - [Documentation](#documentation)
 - [Getting Help](#getting-help)
 - [Community](#community)
@@ -68,43 +68,87 @@
 
 ```bash
 pip install --upgrade spotinst-sdk2
 ```
 
 ## Authentication
 
-The mechanism in which the sdk looks for credentials is to search through a list of possible locations and stop as soon as it finds credentials. The order in which the sdk searches for credentials is:
+The mechanism in which the SDK looks for credentials is to search through a list of possible locations and stop as soon as it finds credentials. The order in which the SDK searches for credentials is:
 
-1. Passing credentials as parameters to the `SpotinstSession()` constructor
+1. Passing credentials as parameters when creating a `SpotinstSession` object:
 
 ```python
-session = SpotinstSession(auth_token='token', account_id='act-123')
+session = SpotinstSession(auth_token='foo', account_id='bar')
 ```
 
-2. Fetching the account and token from environment variables under `SPOTINST_ACCOUNT` & `SPOTINST_TOKEN`.
-If you choose to not pass your credentials directly you configure a credentials file, this file should be a valid `.yml` file. The default shared credential file location is `~/.spotinst/credentials` and the default profile is `default`
+2. Environment variables:
+
+```sh
+export SPOTINST_TOKEN=foo
+export SPOTINST_ACCOUNT=bar
+```
+
+3. Shared credentials file:
+
+- The shared credentials file has a default location of `~/.spotinst/credentials`. This file is an INI formatted file with section names corresponding to profiles. With each section, two configuration variables can be specified: `token`, `account`. These are the only supported values in the shared credential file.
+
+- Below is a minimal example of the shared credentials file:
+
+```ini
+[default]
+token   = foo
+account = bar
+```
+
+- The shared credentials file also supports the concept of profiles. Profiles represent logical groups of configuration. The shared credential file can have multiple profiles:
+
+```ini
+[default]
+token   = foo
+account = bar
+
+[dev]
+token   = foo2
+account = bar2
+
+[prod]
+token   = foo3
+account = bar3
+```
+
+- You can configure your Spot credentials using the `spotctl configure` command. For more information, see the `spotctl` [Getting Started](https://github.com/spotinst/spotctl#getting-started).
+
+- To maintain compatibility with previous SDK versions, the file can also be in YAML format:
 
 ```yaml
-default: #profile
-  token: $defaul_spotinst_token
-  account: $default_spotinst-account-id
-my_profile:
-  token: $my_spotinst_token
-  account: $my_spotinst-account-id
+default:
+  token: foo
+  account: bar
+  
+dev:
+  token: foo2
+  account: bar2
+  
+prod:
+  token: foo3
+  account: bar3
 ```
 
-3. You can overwrite the credentials file location and the profile used as parameters in the `SpotinstSession()` constructor
+- You can change the location of the credentials file and the profile used by setting the `SPOTINST_SHARED_CREDENTIALS_FILE` and/or `SPOTINST_PROFILE` environment variables:
 
-```python
-session = SpotinstSession(credentials_file='/path/to/file', profile='my_profile')
+```sh
+export SPOTINST_SHARED_CREDENTIALS_FILE=/path/to/credentials_file
+export SPOTINST_PROFILE=dev
 ```
 
-4. You can overwrite the credentials file location and the profile used as environment variables `SPOTINST_PROFILE` and/or `SPOTINST_SHARED_CREDENTIALS_FILE`
+- Passing the credentials file location and the profile used as parameters when creating a `SpotinstSession` object:
 
-5. Fetching from the default location with the default profile
+```python
+session = SpotinstSession(credentials_file='/path/to/credentials_file', profile='dev')
+```
   
 ## Setup Clients
 
 After a session is created you can use the session object to create clients. Clients are used to make request to the different services that Spotinsts has to offer. To create a client simply use the method `client` from the session object and pass in the string of the client you wish to create. Here is an example:
 
 ```python
 session = SpotinstSession()
```

### Comparing `spotinst-sdk2-2.1.8/setup.py` & `spotinst-sdk2-2.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.1.8/spotinst_sdk2/__init__.py` & `spotinst-sdk2-2.1.9/spotinst_sdk2/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.1.8/spotinst_sdk2/client.py` & `spotinst-sdk2-2.1.9/spotinst_sdk2/client.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.1.8/spotinst_sdk2/clients/admin/__init__.py` & `spotinst-sdk2-2.1.9/spotinst_sdk2/clients/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.1.8/spotinst_sdk2/clients/elastigroup/__init__.py` & `spotinst-sdk2-2.1.9/spotinst_sdk2/clients/elastigroup/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.1.8/spotinst_sdk2/clients/functions/__init__.py` & `spotinst-sdk2-2.1.9/spotinst_sdk2/clients/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.1.8/spotinst_sdk2/clients/mcs/__init__.py` & `spotinst-sdk2-2.1.9/spotinst_sdk2/clients/mcs/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.1.8/spotinst_sdk2/clients/mlb/__init__.py` & `spotinst-sdk2-2.1.9/spotinst_sdk2/clients/mlb/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.1.8/spotinst_sdk2/clients/mrscaler/__init__.py` & `spotinst-sdk2-2.1.9/spotinst_sdk2/clients/mrscaler/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.1.8/spotinst_sdk2/clients/ocean/__init__.py` & `spotinst-sdk2-2.1.9/spotinst_sdk2/clients/ocean/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.1.8/spotinst_sdk2/clients/subscription/__init__.py` & `spotinst-sdk2-2.1.9/spotinst_sdk2/clients/subscription/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.1.8/spotinst_sdk2/models/admin/user_mapping.py` & `spotinst-sdk2-2.1.9/spotinst_sdk2/models/admin/user_mapping.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.1.8/spotinst_sdk2/models/elastigroup/aws/__init__.py` & `spotinst-sdk2-2.1.9/spotinst_sdk2/models/elastigroup/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.1.8/spotinst_sdk2/models/elastigroup/aws/asg.py` & `spotinst-sdk2-2.1.9/spotinst_sdk2/models/elastigroup/aws/asg.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.1.8/spotinst_sdk2/models/elastigroup/aws/deployment.py` & `spotinst-sdk2-2.1.9/spotinst_sdk2/models/elastigroup/aws/deployment.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.1.8/spotinst_sdk2/models/elastigroup/aws/deployment_action.py` & `spotinst-sdk2-2.1.9/spotinst_sdk2/models/elastigroup/aws/deployment_action.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.1.8/spotinst_sdk2/models/elastigroup/aws/stateful.py` & `spotinst-sdk2-2.1.9/spotinst_sdk2/models/elastigroup/aws/stateful.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.1.8/spotinst_sdk2/models/elastigroup/azure/__init__.py` & `spotinst-sdk2-2.1.9/spotinst_sdk2/models/elastigroup/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.1.8/spotinst_sdk2/models/elastigroup/azure/task.py` & `spotinst-sdk2-2.1.9/spotinst_sdk2/models/elastigroup/azure/task.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.1.8/spotinst_sdk2/models/elastigroup/gcp/__init__.py` & `spotinst-sdk2-2.1.9/spotinst_sdk2/models/elastigroup/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.1.8/spotinst_sdk2/models/elastigroup/gcp/gke.py` & `spotinst-sdk2-2.1.9/spotinst_sdk2/models/elastigroup/gcp/gke.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.1.8/spotinst_sdk2/models/functions/__init__.py` & `spotinst-sdk2-2.1.9/spotinst_sdk2/models/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.1.8/spotinst_sdk2/models/mlb/__init__.py` & `spotinst-sdk2-2.1.9/spotinst_sdk2/models/mlb/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.1.8/spotinst_sdk2/models/mrscaler/aws/__init__.py` & `spotinst-sdk2-2.1.9/spotinst_sdk2/models/mrscaler/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.1.8/spotinst_sdk2/models/ocean/aws/__init__.py` & `spotinst-sdk2-2.1.9/spotinst_sdk2/models/ocean/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.1.8/spotinst_sdk2/models/subscription/__init__.py` & `spotinst-sdk2-2.1.9/spotinst_sdk2/models/subscription/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.1.8/spotinst_sdk2/session.py` & `spotinst-sdk2-2.1.9/spotinst_sdk2/session.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import json
 import os
 import yaml
+import configparser
 from spotinst_sdk2.client import SpotinstClientException
 
 VAR_SPOTINST_SHARED_CREDENTIALS_FILE = 'SPOTINST_SHARED_CREDENTIALS_FILE'
 VAR_SPOTINST_PROFILE = 'SPOTINST_PROFILE'
 VAR_SPOTINST_TOKEN = 'SPOTINST_TOKEN'
 VAR_SPOTINST_ACCOUNT = 'SPOTINST_ACCOUNT'
 
@@ -34,18 +34,32 @@
 
             if not credentials_file:
                 credentials_file = os.environ.get(
                     VAR_SPOTINST_SHARED_CREDENTIALS_FILE,
                     DEFAULT_CREDENTIALS_FILE)
 
             with open(credentials_file, 'r') as credentials_file:
-                config = yaml.load(credentials_file, Loader=yaml.SafeLoader)
-
-                if config:
-                    self.account_id = config.get(
-                        profile, {}).get(
-                        "account", None)
-                    self.auth_token = config.get(
-                        profile, {}).get("token", None)
+                self.__load_credentials_yaml(profile, credentials_file)
+                if not self.auth_token:
+                    self.__load_credentials_ini(profile, credentials_file)
 
             if not self.auth_token:
                 raise SpotinstClientException("failed to load credentials", "ERROR")
+
+    def __load_credentials_yaml(self, profile, credentials_file):
+        try:
+            config = yaml.load(credentials_file, Loader=yaml.SafeLoader)
+            if config:
+                self.account_id = config.get(profile, {}).get("account", None)
+                self.auth_token = config.get(profile, {}).get("token", None)
+        except:
+            return
+
+    def __load_credentials_ini(self, profile, credentials_file):
+        try:
+            config = configparser.ConfigParser()
+            config.read(credentials_file.name)
+            if config[profile]:
+                self.account_id = config[profile]["account"]
+                self.auth_token = config[profile]["token"]
+        except:
+            return
```

### Comparing `spotinst-sdk2-2.1.8/spotinst_sdk2.egg-info/PKG-INFO` & `spotinst-sdk2-2.1.9/spotinst_sdk2.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-sdk2
-Version: 2.1.8
+Version: 2.1.9
 Summary: A Python SDK for Spotinst
 Home-page: https://github.com/spotinst/spotinst-sdk-python
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Description: [![Build Status](https://travis-ci.org/spotinst/spotinst-sdk-python.svg?branch=v2)](https://travis-ci.org/spotinst/spotinst-sdk-python)
         [![Coverage Status](https://coveralls.io/repos/github/spotinst/spotinst-sdk-python/badge.svg?branch=v2)](https://coveralls.io/github/spotinst/spotinst-sdk-python?branch=master)
@@ -58,15 +58,15 @@
         client.create_ocean_cluster(ocean=ocean)
         ```
         
         In the [SDK Client documentation](./docs/clients/) you can view what methods are supported by each client. <br>
         For information on what models are supported checkout the [SDK Model documentation](./docs/models/). <br>
         More examples can be found in the [SDK Examples Documentation](./docs/examples/). <br>
         
-        ## Contents
+        ## Table of Contents
         
         - [Installation](#installation)
         - [Authentication](#authentication)
         - [Setup Clients](#setup-clients)
         - [Documentation](#documentation)
         - [Getting Help](#getting-help)
         - [Community](#community)
@@ -76,43 +76,87 @@
         
         ```bash
         pip install --upgrade spotinst-sdk2
         ```
         
         ## Authentication
         
-        The mechanism in which the sdk looks for credentials is to search through a list of possible locations and stop as soon as it finds credentials. The order in which the sdk searches for credentials is:
+        The mechanism in which the SDK looks for credentials is to search through a list of possible locations and stop as soon as it finds credentials. The order in which the SDK searches for credentials is:
         
-        1. Passing credentials as parameters to the `SpotinstSession()` constructor
+        1. Passing credentials as parameters when creating a `SpotinstSession` object:
         
         ```python
-        session = SpotinstSession(auth_token='token', account_id='act-123')
+        session = SpotinstSession(auth_token='foo', account_id='bar')
         ```
         
-        2. Fetching the account and token from environment variables under `SPOTINST_ACCOUNT` & `SPOTINST_TOKEN`.
-        If you choose to not pass your credentials directly you configure a credentials file, this file should be a valid `.yml` file. The default shared credential file location is `~/.spotinst/credentials` and the default profile is `default`
+        2. Environment variables:
+        
+        ```sh
+        export SPOTINST_TOKEN=foo
+        export SPOTINST_ACCOUNT=bar
+        ```
+        
+        3. Shared credentials file:
+        
+        - The shared credentials file has a default location of `~/.spotinst/credentials`. This file is an INI formatted file with section names corresponding to profiles. With each section, two configuration variables can be specified: `token`, `account`. These are the only supported values in the shared credential file.
+        
+        - Below is a minimal example of the shared credentials file:
+        
+        ```ini
+        [default]
+        token   = foo
+        account = bar
+        ```
+        
+        - The shared credentials file also supports the concept of profiles. Profiles represent logical groups of configuration. The shared credential file can have multiple profiles:
+        
+        ```ini
+        [default]
+        token   = foo
+        account = bar
+        
+        [dev]
+        token   = foo2
+        account = bar2
+        
+        [prod]
+        token   = foo3
+        account = bar3
+        ```
+        
+        - You can configure your Spot credentials using the `spotctl configure` command. For more information, see the `spotctl` [Getting Started](https://github.com/spotinst/spotctl#getting-started).
+        
+        - To maintain compatibility with previous SDK versions, the file can also be in YAML format:
         
         ```yaml
-        default: #profile
-          token: $defaul_spotinst_token
-          account: $default_spotinst-account-id
-        my_profile:
-          token: $my_spotinst_token
-          account: $my_spotinst-account-id
+        default:
+          token: foo
+          account: bar
+          
+        dev:
+          token: foo2
+          account: bar2
+          
+        prod:
+          token: foo3
+          account: bar3
         ```
         
-        3. You can overwrite the credentials file location and the profile used as parameters in the `SpotinstSession()` constructor
+        - You can change the location of the credentials file and the profile used by setting the `SPOTINST_SHARED_CREDENTIALS_FILE` and/or `SPOTINST_PROFILE` environment variables:
         
-        ```python
-        session = SpotinstSession(credentials_file='/path/to/file', profile='my_profile')
+        ```sh
+        export SPOTINST_SHARED_CREDENTIALS_FILE=/path/to/credentials_file
+        export SPOTINST_PROFILE=dev
         ```
         
-        4. You can overwrite the credentials file location and the profile used as environment variables `SPOTINST_PROFILE` and/or `SPOTINST_SHARED_CREDENTIALS_FILE`
+        - Passing the credentials file location and the profile used as parameters when creating a `SpotinstSession` object:
         
-        5. Fetching from the default location with the default profile
+        ```python
+        session = SpotinstSession(credentials_file='/path/to/credentials_file', profile='dev')
+        ```
           
         ## Setup Clients
         
         After a session is created you can use the session object to create clients. Clients are used to make request to the different services that Spotinsts has to offer. To create a client simply use the method `client` from the session object and pass in the string of the client you wish to create. Here is an example:
         
         ```python
         session = SpotinstSession()
```

### Comparing `spotinst-sdk2-2.1.8/spotinst_sdk2.egg-info/SOURCES.txt` & `spotinst-sdk2-2.1.9/spotinst_sdk2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

