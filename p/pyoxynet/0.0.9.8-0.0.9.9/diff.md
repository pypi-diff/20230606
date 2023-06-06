# Comparing `tmp/pyoxynet-0.0.9.8.tar.gz` & `tmp/pyoxynet-0.0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoxynet-0.0.9.8.tar", last modified: Mon Jun 27 03:55:21 2022, max compression
+gzip compressed data, was "pyoxynet-0.0.9.9.tar", last modified: Mon Jun 27 03:58:27 2022, max compression
```

## Comparing `pyoxynet-0.0.9.8.tar` & `pyoxynet-0.0.9.9.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 andreazignoli   (502) staff       (20)        0 2022-06-27 03:55:21.367880 pyoxynet-0.0.9.8/
--rw-r--r--   0 andreazignoli   (502) staff       (20)     1073 2022-01-08 10:03:20.000000 pyoxynet-0.0.9.8/LICENSE.txt
--rw-r--r--   0 andreazignoli   (502) staff       (20)     2368 2022-06-27 03:55:21.367259 pyoxynet-0.0.9.8/PKG-INFO
--rw-r--r--   0 andreazignoli   (502) staff       (20)     1968 2022-01-09 16:44:17.000000 pyoxynet-0.0.9.8/README.md
-drwxr-xr-x   0 andreazignoli   (502) staff       (20)        0 2022-06-27 03:55:21.095127 pyoxynet-0.0.9.8/pyoxynet/
--rw-r--r--   0 andreazignoli   (502) staff       (20)       96 2022-01-09 13:19:59.000000 pyoxynet-0.0.9.8/pyoxynet/__init__.py
-drwxr-xr-x   0 andreazignoli   (502) staff       (20)        0 2022-06-27 03:55:21.359014 pyoxynet-0.0.9.8/pyoxynet/data_test/
--rw-r--r--   0 andreazignoli   (502) staff       (20)        0 2022-03-23 10:51:06.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/__init__.py
--rw-r--r--   0 andreazignoli   (502) staff       (20)   163078 2021-01-06 17:36:26.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/data_test.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)    31571 2022-05-22 23:09:56.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/database_statistics.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   263130 2021-01-06 17:33:56.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_1.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   174531 2021-01-25 11:24:54.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_10.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   238372 2021-01-25 11:23:24.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_11.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   116025 2021-01-06 17:36:06.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_12.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   136588 2021-01-25 11:23:20.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_13.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   277905 2021-01-25 11:22:55.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_14.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   161813 2021-01-25 11:24:34.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_15.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   198532 2021-01-06 17:38:54.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_16.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   147659 2021-01-25 11:24:56.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_17.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   136854 2021-01-25 11:22:57.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_18.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   135113 2021-01-25 11:24:33.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_19.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   114036 2021-01-06 17:34:56.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_2.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   171991 2021-01-25 11:23:26.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_20.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   132605 2021-01-25 11:23:49.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_21.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   149566 2021-01-25 11:24:00.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_22.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   211982 2021-01-06 17:35:32.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_23.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   123010 2021-01-25 11:24:06.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_24.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   138988 2021-01-25 11:23:49.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_25.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   138651 2021-01-25 11:23:29.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_26.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   174453 2021-01-06 17:35:19.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_27.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   152090 2021-01-06 17:34:32.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_28.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   124311 2021-01-06 17:37:37.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_29.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   142536 2021-01-06 17:35:06.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_3.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   264403 2021-01-06 17:37:47.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_30.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   135854 2021-01-06 17:38:01.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_31.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   129424 2021-01-06 17:36:10.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_32.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   155808 2021-01-06 17:33:29.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_33.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   516330 2021-01-06 17:37:08.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_34.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)    85736 2021-01-06 17:35:05.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_35.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   188337 2021-01-06 17:35:43.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_36.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   255380 2021-01-06 17:37:10.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_37.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   148568 2021-01-06 17:37:43.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_38.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   152341 2021-01-06 17:34:41.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_39.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   114053 2021-01-06 17:39:02.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_4.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   195009 2021-01-06 17:33:35.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_40.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   130735 2021-01-06 17:34:41.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_41.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   172755 2021-01-06 17:35:39.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_42.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   142268 2021-01-06 17:36:05.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_43.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   177228 2021-01-06 17:39:19.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_44.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   183364 2021-01-06 17:38:43.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_45.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   137039 2021-04-28 15:36:49.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_46.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   232641 2021-01-06 17:39:17.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_47.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   242149 2021-01-06 17:37:55.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_48.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   220752 2021-01-06 17:39:03.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_49.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   208463 2021-01-25 11:23:13.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_5.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   268630 2021-01-06 17:38:46.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_50.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   258436 2021-01-06 17:35:40.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_6.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   250712 2021-01-25 11:24:48.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_7.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   176143 2021-01-25 11:22:48.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_8.csv
--rw-r--r--   0 andreazignoli   (502) staff       (20)   197626 2021-01-25 11:22:47.000000 pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_9.csv
-drwxr-xr-x   0 andreazignoli   (502) staff       (20)        0 2022-06-27 03:55:21.364775 pyoxynet-0.0.9.8/pyoxynet/models/
--rw-r--r--   0 andreazignoli   (502) staff       (20)    53713 2022-05-23 02:54:28.000000 pyoxynet-0.0.9.8/pyoxynet/models/generator.pickle
--rw-r--r--   0 andreazignoli   (502) staff       (20)    44889 2022-06-27 03:26:02.000000 pyoxynet-0.0.9.8/pyoxynet/models/tfl_model.pickle
--rw-r--r--   0 andreazignoli   (502) staff       (20)   108778 2022-01-11 10:57:09.000000 pyoxynet-0.0.9.8/pyoxynet/models/tfl_model_5_40.pickle
--rw-r--r--   0 andreazignoli   (502) staff       (20)    24185 2022-06-23 09:32:24.000000 pyoxynet-0.0.9.8/pyoxynet/utilities.py
-drwxr-xr-x   0 andreazignoli   (502) staff       (20)        0 2022-06-27 03:55:21.102532 pyoxynet-0.0.9.8/pyoxynet.egg-info/
--rw-r--r--   0 andreazignoli   (502) staff       (20)     2368 2022-06-27 03:55:20.000000 pyoxynet-0.0.9.8/pyoxynet.egg-info/PKG-INFO
--rw-r--r--   0 andreazignoli   (502) staff       (20)     2249 2022-06-27 03:55:21.000000 pyoxynet-0.0.9.8/pyoxynet.egg-info/SOURCES.txt
--rw-r--r--   0 andreazignoli   (502) staff       (20)        1 2022-06-27 03:55:20.000000 pyoxynet-0.0.9.8/pyoxynet.egg-info/dependency_links.txt
--rw-r--r--   0 andreazignoli   (502) staff       (20)       48 2022-06-27 03:55:20.000000 pyoxynet-0.0.9.8/pyoxynet.egg-info/requires.txt
--rw-r--r--   0 andreazignoli   (502) staff       (20)        9 2022-06-27 03:55:20.000000 pyoxynet-0.0.9.8/pyoxynet.egg-info/top_level.txt
--rw-r--r--   0 andreazignoli   (502) staff       (20)      103 2022-01-08 18:33:28.000000 pyoxynet-0.0.9.8/pyproject.toml
--rw-r--r--   0 andreazignoli   (502) staff       (20)       38 2022-06-27 03:55:21.368611 pyoxynet-0.0.9.8/setup.cfg
--rw-r--r--   0 andreazignoli   (502) staff       (20)     1080 2022-06-27 03:52:54.000000 pyoxynet-0.0.9.8/setup.py
+drwxr-xr-x   0 andreazignoli   (502) staff       (20)        0 2022-06-27 03:58:27.863383 pyoxynet-0.0.9.9/
+-rw-r--r--   0 andreazignoli   (502) staff       (20)     1073 2022-01-08 10:03:20.000000 pyoxynet-0.0.9.9/LICENSE.txt
+-rw-r--r--   0 andreazignoli   (502) staff       (20)     2368 2022-06-27 03:58:27.861954 pyoxynet-0.0.9.9/PKG-INFO
+-rw-r--r--   0 andreazignoli   (502) staff       (20)     1968 2022-01-09 16:44:17.000000 pyoxynet-0.0.9.9/README.md
+drwxr-xr-x   0 andreazignoli   (502) staff       (20)        0 2022-06-27 03:58:27.556564 pyoxynet-0.0.9.9/pyoxynet/
+-rw-r--r--   0 andreazignoli   (502) staff       (20)       96 2022-01-09 13:19:59.000000 pyoxynet-0.0.9.9/pyoxynet/__init__.py
+drwxr-xr-x   0 andreazignoli   (502) staff       (20)        0 2022-06-27 03:58:27.843908 pyoxynet-0.0.9.9/pyoxynet/data_test/
+-rw-r--r--   0 andreazignoli   (502) staff       (20)        0 2022-03-23 10:51:06.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/__init__.py
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   163078 2021-01-06 17:36:26.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/data_test.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)    31571 2022-05-22 23:09:56.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/database_statistics.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   263130 2021-01-06 17:33:56.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_1.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   174531 2021-01-25 11:24:54.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_10.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   238372 2021-01-25 11:23:24.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_11.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   116025 2021-01-06 17:36:06.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_12.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   136588 2021-01-25 11:23:20.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_13.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   277905 2021-01-25 11:22:55.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_14.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   161813 2021-01-25 11:24:34.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_15.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   198532 2021-01-06 17:38:54.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_16.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   147659 2021-01-25 11:24:56.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_17.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   136854 2021-01-25 11:22:57.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_18.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   135113 2021-01-25 11:24:33.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_19.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   114036 2021-01-06 17:34:56.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_2.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   171991 2021-01-25 11:23:26.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_20.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   132605 2021-01-25 11:23:49.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_21.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   149566 2021-01-25 11:24:00.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_22.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   211982 2021-01-06 17:35:32.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_23.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   123010 2021-01-25 11:24:06.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_24.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   138988 2021-01-25 11:23:49.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_25.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   138651 2021-01-25 11:23:29.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_26.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   174453 2021-01-06 17:35:19.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_27.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   152090 2021-01-06 17:34:32.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_28.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   124311 2021-01-06 17:37:37.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_29.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   142536 2021-01-06 17:35:06.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_3.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   264403 2021-01-06 17:37:47.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_30.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   135854 2021-01-06 17:38:01.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_31.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   129424 2021-01-06 17:36:10.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_32.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   155808 2021-01-06 17:33:29.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_33.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   516330 2021-01-06 17:37:08.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_34.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)    85736 2021-01-06 17:35:05.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_35.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   188337 2021-01-06 17:35:43.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_36.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   255380 2021-01-06 17:37:10.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_37.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   148568 2021-01-06 17:37:43.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_38.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   152341 2021-01-06 17:34:41.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_39.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   114053 2021-01-06 17:39:02.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_4.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   195009 2021-01-06 17:33:35.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_40.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   130735 2021-01-06 17:34:41.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_41.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   172755 2021-01-06 17:35:39.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_42.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   142268 2021-01-06 17:36:05.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_43.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   177228 2021-01-06 17:39:19.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_44.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   183364 2021-01-06 17:38:43.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_45.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   137039 2021-04-28 15:36:49.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_46.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   232641 2021-01-06 17:39:17.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_47.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   242149 2021-01-06 17:37:55.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_48.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   220752 2021-01-06 17:39:03.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_49.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   208463 2021-01-25 11:23:13.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_5.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   268630 2021-01-06 17:38:46.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_50.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   258436 2021-01-06 17:35:40.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_6.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   250712 2021-01-25 11:24:48.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_7.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   176143 2021-01-25 11:22:48.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_8.csv
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   197626 2021-01-25 11:22:47.000000 pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_9.csv
+drwxr-xr-x   0 andreazignoli   (502) staff       (20)        0 2022-06-27 03:58:27.858109 pyoxynet-0.0.9.9/pyoxynet/models/
+-rw-r--r--   0 andreazignoli   (502) staff       (20)    53713 2022-05-23 02:54:28.000000 pyoxynet-0.0.9.9/pyoxynet/models/generator.pickle
+-rw-r--r--   0 andreazignoli   (502) staff       (20)    44889 2022-06-27 03:26:02.000000 pyoxynet-0.0.9.9/pyoxynet/models/tfl_model.pickle
+-rw-r--r--   0 andreazignoli   (502) staff       (20)   108778 2022-01-11 10:57:09.000000 pyoxynet-0.0.9.9/pyoxynet/models/tfl_model_5_40.pickle
+-rw-r--r--   0 andreazignoli   (502) staff       (20)    24185 2022-06-23 09:32:24.000000 pyoxynet-0.0.9.9/pyoxynet/utilities.py
+drwxr-xr-x   0 andreazignoli   (502) staff       (20)        0 2022-06-27 03:58:27.567580 pyoxynet-0.0.9.9/pyoxynet.egg-info/
+-rw-r--r--   0 andreazignoli   (502) staff       (20)     2368 2022-06-27 03:58:26.000000 pyoxynet-0.0.9.9/pyoxynet.egg-info/PKG-INFO
+-rw-r--r--   0 andreazignoli   (502) staff       (20)     2249 2022-06-27 03:58:27.000000 pyoxynet-0.0.9.9/pyoxynet.egg-info/SOURCES.txt
+-rw-r--r--   0 andreazignoli   (502) staff       (20)        1 2022-06-27 03:58:26.000000 pyoxynet-0.0.9.9/pyoxynet.egg-info/dependency_links.txt
+-rw-r--r--   0 andreazignoli   (502) staff       (20)       48 2022-06-27 03:58:27.000000 pyoxynet-0.0.9.9/pyoxynet.egg-info/requires.txt
+-rw-r--r--   0 andreazignoli   (502) staff       (20)        9 2022-06-27 03:58:27.000000 pyoxynet-0.0.9.9/pyoxynet.egg-info/top_level.txt
+-rw-r--r--   0 andreazignoli   (502) staff       (20)      103 2022-01-08 18:33:28.000000 pyoxynet-0.0.9.9/pyproject.toml
+-rw-r--r--   0 andreazignoli   (502) staff       (20)       38 2022-06-27 03:58:27.863557 pyoxynet-0.0.9.9/setup.cfg
+-rw-r--r--   0 andreazignoli   (502) staff       (20)     1080 2022-06-27 03:58:17.000000 pyoxynet-0.0.9.9/setup.py
```

### Comparing `pyoxynet-0.0.9.8/LICENSE.txt` & `pyoxynet-0.0.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/PKG-INFO` & `pyoxynet-0.0.9.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pyoxynet
-Version: 0.0.9.8
+Version: 0.0.9.9
 Summary: Python package of the Oxynet project
 Author: Andrea Zignoli
 Author-email: andrea.zignoli@unitn.it
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Pyoxynet package
 
 This README has been intentionally created for Pypi. Please find a more extended and detailed description of the project on the [GitHub repository](https://github.com/andreazignoli/pyoxynet).
```

### Comparing `pyoxynet-0.0.9.8/README.md` & `pyoxynet-0.0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/data_test.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/data_test.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/database_statistics.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/database_statistics.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_1.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_1.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_10.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_10.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_11.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_11.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_12.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_12.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_13.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_13.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_14.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_14.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_15.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_15.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_16.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_16.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_17.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_17.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_18.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_18.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_19.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_19.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_2.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_2.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_20.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_20.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_21.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_21.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_22.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_22.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_23.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_23.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_24.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_24.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_25.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_25.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_26.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_26.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_27.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_27.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_28.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_28.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_29.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_29.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_3.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_3.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_30.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_30.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_31.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_31.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_32.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_32.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_33.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_33.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_34.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_34.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_35.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_35.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_36.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_36.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_37.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_37.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_38.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_38.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_39.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_39.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_4.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_4.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_40.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_40.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_41.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_41.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_42.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_42.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_43.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_43.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_44.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_44.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_45.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_45.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_46.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_46.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_47.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_47.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_48.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_48.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_49.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_49.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_5.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_5.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_50.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_50.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_6.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_6.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_7.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_7.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_8.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_8.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/data_test/real_test_9.csv` & `pyoxynet-0.0.9.9/pyoxynet/data_test/real_test_9.csv`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/models/generator.pickle` & `pyoxynet-0.0.9.9/pyoxynet/models/generator.pickle`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/models/tfl_model.pickle` & `pyoxynet-0.0.9.9/pyoxynet/models/tfl_model.pickle`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/models/tfl_model_5_40.pickle` & `pyoxynet-0.0.9.9/pyoxynet/models/tfl_model_5_40.pickle`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet/utilities.py` & `pyoxynet-0.0.9.9/pyoxynet/utilities.py`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/pyoxynet.egg-info/PKG-INFO` & `pyoxynet-0.0.9.9/pyoxynet.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pyoxynet
-Version: 0.0.9.8
+Version: 0.0.9.9
 Summary: Python package of the Oxynet project
 Author: Andrea Zignoli
 Author-email: andrea.zignoli@unitn.it
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Pyoxynet package
 
 This README has been intentionally created for Pypi. Please find a more extended and detailed description of the project on the [GitHub repository](https://github.com/andreazignoli/pyoxynet).
```

### Comparing `pyoxynet-0.0.9.8/pyoxynet.egg-info/SOURCES.txt` & `pyoxynet-0.0.9.9/pyoxynet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyoxynet-0.0.9.8/setup.py` & `pyoxynet-0.0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory/"README.md").read_text()
 
 setuptools.setup(
     name="pyoxynet",
-    version="0.0.9.8",
+    version="0.0.9.9",
     author="Andrea Zignoli",
     author_email="andrea.zignoli@unitn.it",
     description="Python package of the Oxynet project",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     install_requires=['importlib-resources', 'pandas', 'uniplot', 'scipy', 'models'],
@@ -23,9 +23,9 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     include_package_data=True,
     package_data={'': ['models/*', 'data_test/*', 'data_test/real_tests/*']},
     #exclude_package_data={
     #    '': 'debugging.py.c'},
-    python_requires='>=3.8',
+    python_requires='>=3.9',
 )
```

