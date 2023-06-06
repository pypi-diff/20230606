# Comparing `tmp/kemlglearn-0.4.2.tar.gz` & `tmp/kemlglearn-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kemlglearn-0.4.2.tar", last modified: Thu Feb 11 07:48:24 2021, max compression
+gzip compressed data, was "kemlglearn-0.4.3.tar", last modified: Tue Jun  6 12:54:41 2023, max compression
```

## Comparing `kemlglearn-0.4.2.tar` & `kemlglearn-0.4.3.tar`

### file list

```diff
@@ -1,57 +1,65 @@
-drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2021-02-11 07:48:24.073407 kemlglearn-0.4.2/
--rw-rw-r--   0 bejar     (1000) bejar     (1000)      250 2021-02-11 07:48:24.073407 kemlglearn-0.4.2/PKG-INFO
-drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2021-02-11 07:48:24.072407 kemlglearn-0.4.2/kemlglearn/
--rw-rw-r--   0 bejar     (1000) bejar     (1000)      182 2016-07-28 09:50:32.119298 kemlglearn-0.4.2/kemlglearn/__init__.py
-drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2021-02-11 07:48:24.072407 kemlglearn-0.4.2/kemlglearn/cluster/
--rw-rw-r--   0 bejar     (1000) bejar     (1000)     6445 2018-02-09 06:45:27.376243 kemlglearn-0.4.2/kemlglearn/cluster/GlobalKMeans.py
--rw-rw-r--   0 bejar     (1000) bejar     (1000)     6900 2021-02-09 07:17:39.115100 kemlglearn-0.4.2/kemlglearn/cluster/KMedoidsFlexible.py
--rw-rw-r--   0 bejar     (1000) bejar     (1000)    11418 2018-02-09 06:45:27.376243 kemlglearn-0.4.2/kemlglearn/cluster/KModes.py
--rw-rw-r--   0 bejar     (1000) bejar     (1000)    12151 2016-07-28 09:50:37.590425 kemlglearn-0.4.2/kemlglearn/cluster/KPrototypes.py
--rw-rw-r--   0 bejar     (1000) bejar     (1000)     4121 2016-07-28 09:50:37.259418 kemlglearn-0.4.2/kemlglearn/cluster/KernelKMeans.py
--rw-rw-r--   0 bejar     (1000) bejar     (1000)     3406 2018-02-09 06:45:27.376243 kemlglearn-0.4.2/kemlglearn/cluster/Leader.py
--rw-rw-r--   0 bejar     (1000) bejar     (1000)      506 2018-02-09 06:45:27.376243 kemlglearn-0.4.2/kemlglearn/cluster/__init__.py
-drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2021-02-11 07:48:24.072407 kemlglearn-0.4.2/kemlglearn/cluster/border/
--rw-rw-r--   0 bejar     (1000) bejar     (1000)     1995 2021-02-09 07:17:39.231103 kemlglearn-0.4.2/kemlglearn/cluster/border/BorderDetection.py
--rw-rw-r--   0 bejar     (1000) bejar     (1000)      250 2018-02-09 06:45:27.376243 kemlglearn-0.4.2/kemlglearn/cluster/border/__init__.py
-drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2021-02-11 07:48:24.072407 kemlglearn-0.4.2/kemlglearn/cluster/consensus/
--rw-rw-r--   0 bejar     (1000) bejar     (1000)     2317 2021-02-09 07:17:39.334105 kemlglearn-0.4.2/kemlglearn/cluster/consensus/MeanPartition.py
--rw-rw-r--   0 bejar     (1000) bejar     (1000)     4669 2021-02-11 07:47:14.033853 kemlglearn-0.4.2/kemlglearn/cluster/consensus/SimpleConsensusClustering.py
--rw-rw-r--   0 bejar     (1000) bejar     (1000)      377 2016-07-28 09:50:35.160369 kemlglearn-0.4.2/kemlglearn/cluster/consensus/__init__.py
--rw-rw-r--   0 bejar     (1000) bejar     (1000)      905 2016-07-28 09:50:35.492377 kemlglearn-0.4.2/kemlglearn/cluster/consensus/test.py
--rw-rw-r--   0 bejar     (1000) bejar     (1000)     4405 2018-02-09 06:45:27.376243 kemlglearn-0.4.2/kemlglearn/cluster/test.py
-drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2021-02-11 07:48:24.072407 kemlglearn-0.4.2/kemlglearn/datasets/
--rw-rw-r--   0 bejar     (1000) bejar     (1000)      249 2018-02-09 06:45:27.376243 kemlglearn-0.4.2/kemlglearn/datasets/__init__.py
--rw-rw-r--   0 bejar     (1000) bejar     (1000)     5132 2021-02-09 07:17:39.062099 kemlglearn-0.4.2/kemlglearn/datasets/samples_generator.py
-drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2021-02-11 07:48:24.072407 kemlglearn-0.4.2/kemlglearn/feature_selection/
--rw-rw-r--   0 bejar     (1000) bejar     (1000)      184 2016-07-28 09:50:41.710521 kemlglearn-0.4.2/kemlglearn/feature_selection/__init__.py
-drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2021-02-11 07:48:24.072407 kemlglearn-0.4.2/kemlglearn/feature_selection/unsupervised/
--rw-rw-r--   0 bejar     (1000) bejar     (1000)     2836 2021-02-09 07:17:39.280104 kemlglearn-0.4.2/kemlglearn/feature_selection/unsupervised/LaplacianScore.py
--rw-rw-r--   0 bejar     (1000) bejar     (1000)      254 2018-02-09 06:45:27.376243 kemlglearn-0.4.2/kemlglearn/feature_selection/unsupervised/__init__.py
--rw-rw-r--   0 bejar     (1000) bejar     (1000)      730 2018-02-09 06:45:27.376243 kemlglearn-0.4.2/kemlglearn/feature_selection/unsupervised/test.py
-drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2021-02-11 07:48:24.073407 kemlglearn-0.4.2/kemlglearn/metrics/
--rw-rw-r--   0 bejar     (1000) bejar     (1000)     1660 2016-07-28 09:50:39.650473 kemlglearn-0.4.2/kemlglearn/metrics/Xu.py
--rw-rw-r--   0 bejar     (1000) bejar     (1000)     1192 2021-02-09 07:02:31.168290 kemlglearn-0.4.2/kemlglearn/metrics/__init__.py
--rw-rw-r--   0 bejar     (1000) bejar     (1000)    14040 2021-02-09 06:43:53.611677 kemlglearn-0.4.2/kemlglearn/metrics/cluster.py
--rw-rw-r--   0 bejar     (1000) bejar     (1000)     2308 2016-07-28 09:50:39.815477 kemlglearn-0.4.2/kemlglearn/metrics/divergences.py
--rw-rw-r--   0 bejar     (1000) bejar     (1000)     4478 2016-07-28 09:50:40.329489 kemlglearn-0.4.2/kemlglearn/metrics/nestedpartition.py
--rw-rw-r--   0 bejar     (1000) bejar     (1000)     1920 2021-02-09 07:17:38.989097 kemlglearn-0.4.2/kemlglearn/metrics/quantization_error.py
--rw-rw-r--   0 bejar     (1000) bejar     (1000)      772 2016-07-28 09:50:40.496493 kemlglearn-0.4.2/kemlglearn/metrics/test.py
-drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2021-02-11 07:48:24.073407 kemlglearn-0.4.2/kemlglearn/preprocessing/
--rw-rw-r--   0 bejar     (1000) bejar     (1000)     3642 2016-07-28 09:50:38.789453 kemlglearn-0.4.2/kemlglearn/preprocessing/Discretizer.py
--rw-rw-r--   0 bejar     (1000) bejar     (1000)     3355 2018-02-09 06:45:27.415243 kemlglearn-0.4.2/kemlglearn/preprocessing/Imputer.py
--rw-rw-r--   0 bejar     (1000) bejar     (1000)      290 2018-02-09 06:45:27.415243 kemlglearn-0.4.2/kemlglearn/preprocessing/__init__.py
--rw-rw-r--   0 bejar     (1000) bejar     (1000)      579 2016-07-28 09:50:38.456445 kemlglearn-0.4.2/kemlglearn/preprocessing/test.py
-drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2021-02-11 07:48:24.073407 kemlglearn-0.4.2/kemlglearn/time_series/
--rw-rw-r--   0 bejar     (1000) bejar     (1000)      181 2016-07-28 09:50:31.209277 kemlglearn-0.4.2/kemlglearn/time_series/__init__.py
-drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2021-02-11 07:48:24.073407 kemlglearn-0.4.2/kemlglearn/time_series/decomposition/
--rw-rw-r--   0 bejar     (1000) bejar     (1000)     1902 2018-02-09 06:45:27.415243 kemlglearn-0.4.2/kemlglearn/time_series/decomposition/MFT.py
--rw-rw-r--   0 bejar     (1000) bejar     (1000)      823 2018-02-09 06:45:27.415243 kemlglearn-0.4.2/kemlglearn/time_series/decomposition/STFT.py
--rw-rw-r--   0 bejar     (1000) bejar     (1000)      252 2018-02-09 06:45:27.415243 kemlglearn-0.4.2/kemlglearn/time_series/decomposition/__init__.py
-drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2021-02-11 07:48:24.073407 kemlglearn-0.4.2/kemlglearn/time_series/discretization/
--rw-rw-r--   0 bejar     (1000) bejar     (1000)     4543 2018-02-09 06:45:27.415243 kemlglearn-0.4.2/kemlglearn/time_series/discretization/BOSS.py
--rw-rw-r--   0 bejar     (1000) bejar     (1000)     2822 2018-02-09 06:45:27.508246 kemlglearn-0.4.2/kemlglearn/time_series/discretization/SAX.py
--rw-rw-r--   0 bejar     (1000) bejar     (1000)      253 2018-02-09 06:45:27.415243 kemlglearn-0.4.2/kemlglearn/time_series/discretization/__init__.py
-drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2021-02-11 07:48:24.073407 kemlglearn-0.4.2/kemlglearn/time_series/smoothing/
--rw-rw-r--   0 bejar     (1000) bejar     (1000)    10480 2018-02-09 06:45:27.415243 kemlglearn-0.4.2/kemlglearn/time_series/smoothing/Smoothing.py
--rw-rw-r--   0 bejar     (1000) bejar     (1000)      181 2018-02-09 06:45:27.415243 kemlglearn-0.4.2/kemlglearn/time_series/smoothing/__init__.py
--rw-rw-r--   0 bejar     (1000) bejar     (1000)      844 2021-02-11 07:31:09.734466 kemlglearn-0.4.2/setup.py
+drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2023-06-06 12:54:41.158793 kemlglearn-0.4.3/
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)     1096 2015-05-06 08:01:46.000000 kemlglearn-0.4.3/LICENSE
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)      233 2023-06-06 12:54:41.158793 kemlglearn-0.4.3/PKG-INFO
+-rw-r--r--   0 bejar     (1000) bejar     (1000)      469 2023-06-06 12:50:16.000000 kemlglearn-0.4.3/README.md
+drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2023-06-06 12:54:41.148793 kemlglearn-0.4.3/kemlglearn/
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)      182 2016-07-19 12:18:18.000000 kemlglearn-0.4.3/kemlglearn/__init__.py
+drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2023-06-06 12:54:41.150793 kemlglearn-0.4.3/kemlglearn/cluster/
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)     6445 2018-02-01 07:52:53.000000 kemlglearn-0.4.3/kemlglearn/cluster/GlobalKMeans.py
+-rw-r--r--   0 bejar     (1000) bejar     (1000)     6900 2023-06-06 12:50:16.000000 kemlglearn-0.4.3/kemlglearn/cluster/KMedoidsFlexible.py
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)    11418 2018-02-01 07:52:53.000000 kemlglearn-0.4.3/kemlglearn/cluster/KModes.py
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)    12151 2015-07-13 05:16:38.000000 kemlglearn-0.4.3/kemlglearn/cluster/KPrototypes.py
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)     4121 2016-03-30 09:34:36.000000 kemlglearn-0.4.3/kemlglearn/cluster/KernelKMeans.py
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)     3406 2018-02-01 07:52:53.000000 kemlglearn-0.4.3/kemlglearn/cluster/Leader.py
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)      506 2017-12-18 12:42:40.000000 kemlglearn-0.4.3/kemlglearn/cluster/__init__.py
+drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2023-06-06 12:54:41.151793 kemlglearn-0.4.3/kemlglearn/cluster/border/
+-rw-r--r--   0 bejar     (1000) bejar     (1000)     1995 2023-06-06 12:50:16.000000 kemlglearn-0.4.3/kemlglearn/cluster/border/BorderDetection.py
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)      250 2017-12-18 12:42:40.000000 kemlglearn-0.4.3/kemlglearn/cluster/border/__init__.py
+drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2023-06-06 12:54:41.152793 kemlglearn-0.4.3/kemlglearn/cluster/consensus/
+-rw-r--r--   0 bejar     (1000) bejar     (1000)     2317 2023-06-06 12:50:16.000000 kemlglearn-0.4.3/kemlglearn/cluster/consensus/MeanPartition.py
+-rw-r--r--   0 bejar     (1000) bejar     (1000)     4684 2023-06-06 12:51:24.000000 kemlglearn-0.4.3/kemlglearn/cluster/consensus/SimpleConsensusClustering.py
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)      377 2015-02-10 12:45:43.000000 kemlglearn-0.4.3/kemlglearn/cluster/consensus/__init__.py
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)      905 2015-02-12 14:56:41.000000 kemlglearn-0.4.3/kemlglearn/cluster/consensus/test.py
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)     4405 2017-12-19 14:05:06.000000 kemlglearn-0.4.3/kemlglearn/cluster/test.py
+drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2023-06-06 12:54:41.152793 kemlglearn-0.4.3/kemlglearn/datasets/
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)      249 2017-12-18 13:48:06.000000 kemlglearn-0.4.3/kemlglearn/datasets/__init__.py
+-rw-r--r--   0 bejar     (1000) bejar     (1000)     5132 2023-06-06 12:50:16.000000 kemlglearn-0.4.3/kemlglearn/datasets/samples_generator.py
+drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2023-06-06 12:54:41.152793 kemlglearn-0.4.3/kemlglearn/feature_selection/
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)      184 2015-01-21 08:18:17.000000 kemlglearn-0.4.3/kemlglearn/feature_selection/__init__.py
+drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2023-06-06 12:54:41.153793 kemlglearn-0.4.3/kemlglearn/feature_selection/unsupervised/
+-rw-r--r--   0 bejar     (1000) bejar     (1000)     2836 2023-06-06 12:50:16.000000 kemlglearn-0.4.3/kemlglearn/feature_selection/unsupervised/LaplacianScore.py
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)      254 2018-02-01 07:52:53.000000 kemlglearn-0.4.3/kemlglearn/feature_selection/unsupervised/__init__.py
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)      730 2018-02-01 07:52:53.000000 kemlglearn-0.4.3/kemlglearn/feature_selection/unsupervised/test.py
+drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2023-06-06 12:54:41.155793 kemlglearn-0.4.3/kemlglearn/metrics/
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)     1660 2016-03-30 09:32:41.000000 kemlglearn-0.4.3/kemlglearn/metrics/Xu.py
+-rw-r--r--   0 bejar     (1000) bejar     (1000)     1192 2023-06-06 12:50:16.000000 kemlglearn-0.4.3/kemlglearn/metrics/__init__.py
+-rw-r--r--   0 bejar     (1000) bejar     (1000)    14040 2023-06-06 12:50:16.000000 kemlglearn-0.4.3/kemlglearn/metrics/cluster.py
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)     2308 2016-01-04 12:31:51.000000 kemlglearn-0.4.3/kemlglearn/metrics/divergences.py
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)     4478 2016-03-30 09:36:29.000000 kemlglearn-0.4.3/kemlglearn/metrics/nestedpartition.py
+-rw-r--r--   0 bejar     (1000) bejar     (1000)     1920 2023-06-06 12:50:16.000000 kemlglearn-0.4.3/kemlglearn/metrics/quantization_error.py
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)      772 2016-03-30 09:31:34.000000 kemlglearn-0.4.3/kemlglearn/metrics/test.py
+drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2023-06-06 12:54:41.156793 kemlglearn-0.4.3/kemlglearn/preprocessing/
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)     3642 2015-09-01 10:18:18.000000 kemlglearn-0.4.3/kemlglearn/preprocessing/Discretizer.py
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)     3355 2016-09-07 08:06:00.000000 kemlglearn-0.4.3/kemlglearn/preprocessing/Imputer.py
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)      290 2017-12-18 08:50:53.000000 kemlglearn-0.4.3/kemlglearn/preprocessing/__init__.py
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)      579 2016-03-30 09:35:00.000000 kemlglearn-0.4.3/kemlglearn/preprocessing/test.py
+drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2023-06-06 12:54:41.156793 kemlglearn-0.4.3/kemlglearn/time_series/
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)      181 2015-03-18 12:48:40.000000 kemlglearn-0.4.3/kemlglearn/time_series/__init__.py
+drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2023-06-06 12:54:41.156793 kemlglearn-0.4.3/kemlglearn/time_series/decomposition/
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)     1902 2017-06-30 10:39:07.000000 kemlglearn-0.4.3/kemlglearn/time_series/decomposition/MFT.py
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)      823 2017-04-24 07:45:20.000000 kemlglearn-0.4.3/kemlglearn/time_series/decomposition/STFT.py
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)      252 2018-02-01 11:28:58.000000 kemlglearn-0.4.3/kemlglearn/time_series/decomposition/__init__.py
+drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2023-06-06 12:54:41.157793 kemlglearn-0.4.3/kemlglearn/time_series/discretization/
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)     4543 2017-06-30 10:39:07.000000 kemlglearn-0.4.3/kemlglearn/time_series/discretization/BOSS.py
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)     2822 2018-01-26 13:15:15.000000 kemlglearn-0.4.3/kemlglearn/time_series/discretization/SAX.py
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)      253 2018-02-01 11:26:46.000000 kemlglearn-0.4.3/kemlglearn/time_series/discretization/__init__.py
+drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2023-06-06 12:54:41.158793 kemlglearn-0.4.3/kemlglearn/time_series/smoothing/
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)    10480 2018-02-01 07:52:53.000000 kemlglearn-0.4.3/kemlglearn/time_series/smoothing/Smoothing.py
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)      181 2017-06-30 10:32:30.000000 kemlglearn-0.4.3/kemlglearn/time_series/smoothing/__init__.py
+drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2023-06-06 12:54:41.148793 kemlglearn-0.4.3/kemlglearn.egg-info/
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)      233 2023-06-06 12:54:41.000000 kemlglearn-0.4.3/kemlglearn.egg-info/PKG-INFO
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)     1764 2023-06-06 12:54:41.000000 kemlglearn-0.4.3/kemlglearn.egg-info/SOURCES.txt
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)        1 2023-06-06 12:54:41.000000 kemlglearn-0.4.3/kemlglearn.egg-info/dependency_links.txt
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)       11 2023-06-06 12:54:41.000000 kemlglearn-0.4.3/kemlglearn.egg-info/top_level.txt
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)       38 2023-06-06 12:54:41.158793 kemlglearn-0.4.3/setup.cfg
+-rw-r--r--   0 bejar     (1000) bejar     (1000)      844 2023-06-06 12:50:47.000000 kemlglearn-0.4.3/setup.py
```

### Comparing `kemlglearn-0.4.2/kemlglearn/cluster/GlobalKMeans.py` & `kemlglearn-0.4.3/kemlglearn/cluster/GlobalKMeans.py`

 * *Files identical despite different names*

### Comparing `kemlglearn-0.4.2/kemlglearn/cluster/KMedoidsFlexible.py` & `kemlglearn-0.4.3/kemlglearn/cluster/KMedoidsFlexible.py`

 * *Files identical despite different names*

### Comparing `kemlglearn-0.4.2/kemlglearn/cluster/KModes.py` & `kemlglearn-0.4.3/kemlglearn/cluster/KModes.py`

 * *Files identical despite different names*

### Comparing `kemlglearn-0.4.2/kemlglearn/cluster/KPrototypes.py` & `kemlglearn-0.4.3/kemlglearn/cluster/KPrototypes.py`

 * *Files identical despite different names*

### Comparing `kemlglearn-0.4.2/kemlglearn/cluster/KernelKMeans.py` & `kemlglearn-0.4.3/kemlglearn/cluster/KernelKMeans.py`

 * *Files identical despite different names*

### Comparing `kemlglearn-0.4.2/kemlglearn/cluster/Leader.py` & `kemlglearn-0.4.3/kemlglearn/cluster/Leader.py`

 * *Files identical despite different names*

### Comparing `kemlglearn-0.4.2/kemlglearn/cluster/border/BorderDetection.py` & `kemlglearn-0.4.3/kemlglearn/cluster/border/BorderDetection.py`

 * *Files identical despite different names*

### Comparing `kemlglearn-0.4.2/kemlglearn/cluster/consensus/MeanPartition.py` & `kemlglearn-0.4.3/kemlglearn/cluster/consensus/MeanPartition.py`

 * *Files identical despite different names*

### Comparing `kemlglearn-0.4.2/kemlglearn/cluster/consensus/SimpleConsensusClustering.py` & `kemlglearn-0.4.3/kemlglearn/cluster/consensus/SimpleConsensusClustering.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
         coin_matrix = np.zeros((X.shape[0], X.shape[0]))
         for l in clabels:
             coin_matrix += (l[None, :] == l[:, None])
 
         coin_matrix /= self.n_components
         if self.consensus2 == 'kmeans':
-            kmc = KMeans(n_clusters=self.n_clusters)
+            kmc = KMeans(n_clusters=self.n_clusters, n_init='auto')
             kmc.fit(coin_matrix)
             return kmc.cluster_centers_, kmc.labels_
         elif self.consensus2 == 'spectral':
             kmc = SpectralClustering(n_clusters=self.n_clusters, assign_labels='discretize',
                                      affinity='nearest_neighbors', n_neighbors=40)
             kmc.fit(coin_matrix)
```

### Comparing `kemlglearn-0.4.2/kemlglearn/cluster/consensus/test.py` & `kemlglearn-0.4.3/kemlglearn/cluster/consensus/test.py`

 * *Files identical despite different names*

### Comparing `kemlglearn-0.4.2/kemlglearn/cluster/test.py` & `kemlglearn-0.4.3/kemlglearn/cluster/test.py`

 * *Files identical despite different names*

### Comparing `kemlglearn-0.4.2/kemlglearn/datasets/samples_generator.py` & `kemlglearn-0.4.3/kemlglearn/datasets/samples_generator.py`

 * *Files identical despite different names*

### Comparing `kemlglearn-0.4.2/kemlglearn/feature_selection/unsupervised/LaplacianScore.py` & `kemlglearn-0.4.3/kemlglearn/feature_selection/unsupervised/LaplacianScore.py`

 * *Files identical despite different names*

### Comparing `kemlglearn-0.4.2/kemlglearn/feature_selection/unsupervised/test.py` & `kemlglearn-0.4.3/kemlglearn/feature_selection/unsupervised/test.py`

 * *Files identical despite different names*

### Comparing `kemlglearn-0.4.2/kemlglearn/metrics/Xu.py` & `kemlglearn-0.4.3/kemlglearn/metrics/Xu.py`

 * *Files identical despite different names*

### Comparing `kemlglearn-0.4.2/kemlglearn/metrics/__init__.py` & `kemlglearn-0.4.3/kemlglearn/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kemlglearn-0.4.2/kemlglearn/metrics/cluster.py` & `kemlglearn-0.4.3/kemlglearn/metrics/cluster.py`

 * *Files identical despite different names*

### Comparing `kemlglearn-0.4.2/kemlglearn/metrics/divergences.py` & `kemlglearn-0.4.3/kemlglearn/metrics/divergences.py`

 * *Files identical despite different names*

### Comparing `kemlglearn-0.4.2/kemlglearn/metrics/nestedpartition.py` & `kemlglearn-0.4.3/kemlglearn/metrics/nestedpartition.py`

 * *Files identical despite different names*

### Comparing `kemlglearn-0.4.2/kemlglearn/metrics/quantization_error.py` & `kemlglearn-0.4.3/kemlglearn/metrics/quantization_error.py`

 * *Files identical despite different names*

### Comparing `kemlglearn-0.4.2/kemlglearn/metrics/test.py` & `kemlglearn-0.4.3/kemlglearn/metrics/test.py`

 * *Files identical despite different names*

### Comparing `kemlglearn-0.4.2/kemlglearn/preprocessing/Discretizer.py` & `kemlglearn-0.4.3/kemlglearn/preprocessing/Discretizer.py`

 * *Files identical despite different names*

### Comparing `kemlglearn-0.4.2/kemlglearn/preprocessing/Imputer.py` & `kemlglearn-0.4.3/kemlglearn/preprocessing/Imputer.py`

 * *Files identical despite different names*

### Comparing `kemlglearn-0.4.2/kemlglearn/preprocessing/test.py` & `kemlglearn-0.4.3/kemlglearn/preprocessing/test.py`

 * *Files identical despite different names*

### Comparing `kemlglearn-0.4.2/kemlglearn/time_series/decomposition/MFT.py` & `kemlglearn-0.4.3/kemlglearn/time_series/decomposition/MFT.py`

 * *Files identical despite different names*

### Comparing `kemlglearn-0.4.2/kemlglearn/time_series/decomposition/STFT.py` & `kemlglearn-0.4.3/kemlglearn/time_series/decomposition/STFT.py`

 * *Files identical despite different names*

### Comparing `kemlglearn-0.4.2/kemlglearn/time_series/discretization/BOSS.py` & `kemlglearn-0.4.3/kemlglearn/time_series/discretization/BOSS.py`

 * *Files identical despite different names*

### Comparing `kemlglearn-0.4.2/kemlglearn/time_series/discretization/SAX.py` & `kemlglearn-0.4.3/kemlglearn/time_series/discretization/SAX.py`

 * *Files identical despite different names*

### Comparing `kemlglearn-0.4.2/kemlglearn/time_series/smoothing/Smoothing.py` & `kemlglearn-0.4.3/kemlglearn/time_series/smoothing/Smoothing.py`

 * *Files identical despite different names*

### Comparing `kemlglearn-0.4.2/setup.py` & `kemlglearn-0.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name='kemlglearn',
-    version='0.4.2',
+    version='0.4.3',
     packages=['kemlglearn',
               'kemlglearn.cluster',
               'kemlglearn.cluster.consensus',
               'kemlglearn.cluster.border',
               'kemlglearn.metrics',
               'kemlglearn.datasets',
               'kemlglearn.feature_selection',
```

