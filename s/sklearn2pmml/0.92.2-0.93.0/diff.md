# Comparing `tmp/sklearn2pmml-0.92.2.tar.gz` & `tmp/sklearn2pmml-0.93.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sklearn2pmml-0.92.2.tar", last modified: Wed May 17 06:59:33 2023, max compression
+gzip compressed data, was "dist/sklearn2pmml-0.93.0.tar", last modified: Tue Jun  6 07:43:51 2023, max compression
```

## Comparing `sklearn2pmml-0.92.2.tar` & `sklearn2pmml-0.93.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)       40 2018-03-12 15:29:56.000000 sklearn2pmml-0.92.2/setup.cfg
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    34520 2018-03-12 15:29:56.000000 sklearn2pmml-0.92.2/LICENSE.txt
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1386 2023-03-03 19:54:54.000000 sklearn2pmml-0.92.2/setup.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      739 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/PKG-INFO
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      840 2022-11-15 10:41:18.000000 sklearn2pmml-0.92.2/sklearn2pmml/h2o.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/ruleset/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      888 2023-02-25 19:29:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/ruleset/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/pipeline/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     6005 2022-12-20 20:55:09.000000 sklearn2pmml-0.92.2/sklearn2pmml/pipeline/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      769 2023-04-30 07:17:22.000000 sklearn2pmml-0.92.2/sklearn2pmml/tpot.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    11627 2023-05-17 05:52:06.000000 sklearn2pmml-0.92.2/sklearn2pmml/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/decoration/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    16904 2023-01-03 17:06:18.000000 sklearn2pmml-0.92.2/sklearn2pmml/decoration/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/neural_network/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      777 2022-12-11 13:16:56.000000 sklearn2pmml-0.92.2/sklearn2pmml/neural_network/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      640 2022-12-07 19:44:36.000000 sklearn2pmml-0.92.2/sklearn2pmml/pycaret.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/util/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7471 2023-04-29 08:24:42.000000 sklearn2pmml-0.92.2/sklearn2pmml/util/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1108 2023-01-30 14:56:55.000000 sklearn2pmml-0.92.2/sklearn2pmml/xgboost.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/feature_extraction/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2018-03-12 15:29:56.000000 sklearn2pmml-0.92.2/sklearn2pmml/feature_extraction/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/feature_extraction/text/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1123 2021-01-09 09:21:36.000000 sklearn2pmml-0.92.2/sklearn2pmml/feature_extraction/text/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/ensemble/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     9179 2023-02-25 19:29:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/ensemble/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     3237 2023-03-15 18:26:47.000000 sklearn2pmml-0.92.2/sklearn2pmml/statsmodels.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/feature_selection/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      846 2022-04-01 09:50:44.000000 sklearn2pmml-0.92.2/sklearn2pmml/feature_selection/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/postprocessing/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1628 2022-12-11 13:56:03.000000 sklearn2pmml-0.92.2/sklearn2pmml/postprocessing/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1300 2020-10-11 20:49:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   139727 2021-10-23 18:57:27.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/jaxb-core-3.0.2.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    68173 2023-04-08 17:17:57.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-lightgbm-1.4.5.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     5099 2023-05-17 06:50:31.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.28.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      297 2020-07-25 07:02:00.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    41125 2022-02-16 09:19:19.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/slf4j-api-1.7.36.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    75714 2022-07-22 17:55:51.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/jackson-annotations-2.13.3.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    69254 2018-02-17 21:50:20.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/jcommander-1.72.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)  1138813 2022-08-01 13:09:48.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-model-1.6.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    54279 2022-06-05 15:53:19.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/pickle-1.3.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   432826 2023-05-01 06:26:58.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/h2o-genmodel-3.40.0.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   191286 2022-08-21 07:39:07.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-converter-1.5.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     2235 2022-05-06 18:22:34.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/ubjson-gson-0.1.8.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7977 2023-05-17 06:50:31.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.28.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)  2521113 2017-01-28 20:01:27.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/guava-21.0.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    27449 2023-03-28 18:11:11.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-statsmodels-1.0.2.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     4708 2022-08-01 13:10:01.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    39662 2022-05-06 18:22:34.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/ubjson-0.1.8.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   198275 2023-03-11 19:58:17.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-python-1.1.14.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   466641 2023-05-17 06:50:30.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-sklearn-1.7.28.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    46362 2022-08-31 13:41:52.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-h2o-1.2.5.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    84308 2023-05-17 06:50:30.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-sklearn-extension-1.7.28.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      810 2023-05-17 06:56:56.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/classpath.txt
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     4526 2023-05-01 06:26:58.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/h2o-logger-3.40.0.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     5703 2023-05-17 06:56:57.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     6332 2023-05-17 06:50:31.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.28.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    72620 2023-01-07 07:34:52.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-xgboost-1.7.3.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     8436 2022-02-16 09:19:19.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   913701 2021-10-23 18:57:29.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    44790 2021-06-01 08:00:08.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/serpent-1.40.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    29896 2021-10-23 18:57:27.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7312 2023-05-17 06:50:31.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.28.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    62154 2021-10-23 18:57:27.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/jakarta.activation-2.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   128941 2021-10-23 18:57:27.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   286235 2022-12-26 20:16:36.000000 sklearn2pmml-0.92.2/sklearn2pmml/resources/gson-2.10.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      144 2023-05-17 06:56:45.000000 sklearn2pmml-0.92.2/sklearn2pmml/metadata.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/preprocessing/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      880 2022-04-15 15:03:20.000000 sklearn2pmml-0.92.2/sklearn2pmml/preprocessing/h2o.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    16202 2023-04-30 08:35:42.000000 sklearn2pmml-0.92.2/sklearn2pmml/preprocessing/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1724 2023-04-30 08:35:42.000000 sklearn2pmml-0.92.2/sklearn2pmml/preprocessing/xgboost.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1868 2023-04-30 08:35:42.000000 sklearn2pmml-0.92.2/sklearn2pmml/preprocessing/lightgbm.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/tree/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1941 2022-12-19 19:21:40.000000 sklearn2pmml-0.92.2/sklearn2pmml/tree/chaid.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2022-06-06 08:17:18.000000 sklearn2pmml-0.92.2/sklearn2pmml/tree/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-17 06:59:33.000000 sklearn2pmml-0.92.2/sklearn2pmml/expression/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     2944 2023-03-03 19:54:59.000000 sklearn2pmml-0.92.2/sklearn2pmml/expression/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)       40 2018-03-12 15:29:56.000000 sklearn2pmml-0.93.0/setup.cfg
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    34520 2018-03-12 15:29:56.000000 sklearn2pmml-0.93.0/LICENSE.txt
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1386 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/setup.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      739 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/PKG-INFO
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      840 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/h2o.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/ruleset/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      888 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/ruleset/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/pipeline/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     6005 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/pipeline/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      769 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/tpot.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    11627 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/decoration/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    16924 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/decoration/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/neural_network/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      777 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/neural_network/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      640 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/pycaret.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/util/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     7471 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/util/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1108 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/xgboost.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/feature_extraction/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2018-03-12 15:29:56.000000 sklearn2pmml-0.93.0/sklearn2pmml/feature_extraction/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/feature_extraction/text/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1123 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/feature_extraction/text/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/ensemble/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     9294 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/ensemble/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4574 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/statsmodels.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/feature_selection/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      846 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/feature_selection/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/postprocessing/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1740 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/postprocessing/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1300 2020-10-11 20:49:33.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     6244 2023-06-06 07:35:43.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.29.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   139727 2021-10-23 18:57:27.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/jaxb-core-3.0.2.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    68173 2023-04-08 17:17:57.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-lightgbm-1.4.5.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      297 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    41125 2022-02-16 09:19:19.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/slf4j-api-1.7.36.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    75714 2022-07-22 17:55:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/jackson-annotations-2.13.3.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    69254 2018-02-17 21:50:20.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/jcommander-1.72.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     7312 2023-06-06 07:35:43.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.29.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)  1138813 2022-08-01 13:09:48.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-model-1.6.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    54279 2022-06-05 15:53:19.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/pickle-1.3.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     7978 2023-06-06 07:35:43.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.29.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   432826 2023-05-01 06:26:58.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/h2o-genmodel-3.40.0.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   191286 2022-08-21 07:39:07.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-converter-1.5.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     2235 2022-05-06 18:22:34.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/ubjson-gson-0.1.8.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)  2521113 2017-01-28 20:01:27.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/guava-21.0.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4708 2022-08-01 13:10:01.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    39662 2022-05-06 18:22:34.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/ubjson-0.1.8.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   198275 2023-03-11 19:58:17.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-python-1.1.14.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      810 2023-06-06 07:41:16.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/classpath.txt
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    84309 2023-06-06 07:35:43.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-sklearn-extension-1.7.29.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4526 2023-05-01 06:26:58.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/h2o-logger-3.40.0.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     5704 2023-06-06 07:41:17.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    72620 2023-01-07 07:34:52.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-xgboost-1.7.3.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    46363 2023-05-30 19:11:53.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-h2o-1.2.6.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    34545 2023-05-30 08:51:06.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-statsmodels-1.0.3.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     8436 2022-02-16 09:19:19.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   913701 2021-10-23 18:57:29.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    44790 2021-06-01 08:00:08.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/serpent-1.40.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    29896 2021-10-23 18:57:27.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    62154 2021-10-23 18:57:27.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/jakarta.activation-2.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   128941 2021-10-23 18:57:27.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     6333 2023-06-06 07:35:43.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.29.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   467741 2023-06-06 07:35:42.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-sklearn-1.7.29.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   286235 2022-12-26 20:16:36.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/gson-2.10.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      144 2023-06-06 07:40:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/metadata.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/preprocessing/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      880 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/preprocessing/h2o.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    16423 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/preprocessing/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1724 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/preprocessing/xgboost.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1868 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/preprocessing/lightgbm.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/tree/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1941 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/tree/chaid.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/tree/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/expression/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     2944 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/expression/__init__.py
```

### Comparing `sklearn2pmml-0.92.2/LICENSE.txt` & `sklearn2pmml-0.93.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/setup.py` & `sklearn2pmml-0.93.0/setup.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/PKG-INFO` & `sklearn2pmml-0.93.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: sklearn2pmml
-Version: 0.92.2
+Version: 0.93.0
 Summary: Python library for converting Scikit-Learn pipelines to PMML
 Home-page: https://github.com/jpmml/sklearn2pmml
 Author: Villu Ruusmann
 Author-email: villu.ruusmann@gmail.com
 License: GNU Affero General Public License (AGPL) version 3.0
-Download-URL: https://github.com/jpmml/sklearn2pmml/archive/0.92.2.tar.gz
+Download-URL: https://github.com/jpmml/sklearn2pmml/archive/0.93.0.tar.gz
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/h2o.py` & `sklearn2pmml-0.93.0/sklearn2pmml/h2o.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/ruleset/__init__.py` & `sklearn2pmml-0.93.0/sklearn2pmml/ruleset/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/pipeline/__init__.py` & `sklearn2pmml-0.93.0/sklearn2pmml/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/tpot.py` & `sklearn2pmml-0.93.0/sklearn2pmml/tpot.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/__init__.py` & `sklearn2pmml-0.93.0/sklearn2pmml/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/decoration/__init__.py` & `sklearn2pmml-0.93.0/sklearn2pmml/decoration/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from pandas import DataFrame
 from sklearn.base import clone, BaseEstimator, TransformerMixin
 from sklearn2pmml import _is_pandas_categorical
 from sklearn2pmml.util import cast, common_dtype, ensure_1d, eval_rows
 
+import copy
 import numpy
 import pandas
 
 class TransformerWrapper(BaseEstimator, TransformerMixin):
 
 	def __init__(self, transformer, prefit = False):
 		self.transformer = transformer
 		self.prefit = prefit
 		if prefit:
-			self.transformer_ = clone(self.transformer)
+			self.transformer_ = copy.deepcopy(self.transformer)
 
 	def fit(self, X, y = None, **fit_params):
 		self.transformer_ = clone(self.transformer)
 		if y is None:
 			self.transformer_.fit(X, **fit_params)
 		else:
 			self.transformer_.fit(X, y, **fit_params)
```

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/neural_network/__init__.py` & `sklearn2pmml-0.93.0/sklearn2pmml/neural_network/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/pycaret.py` & `sklearn2pmml-0.93.0/sklearn2pmml/pycaret.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/util/__init__.py` & `sklearn2pmml-0.93.0/sklearn2pmml/util/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/xgboost.py` & `sklearn2pmml-0.93.0/sklearn2pmml/xgboost.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/feature_extraction/text/__init__.py` & `sklearn2pmml-0.93.0/sklearn2pmml/feature_extraction/text/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/ensemble/__init__.py` & `sklearn2pmml-0.93.0/sklearn2pmml/ensemble/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 	from sklearn.linear_model._base import LinearClassifierMixin, LinearModel, SparseCoefMixin
 except ImportError:
 	from sklearn.linear_model.base import LinearClassifierMixin, LinearModel, LinearRegression, SparseCoefMixin
 from sklearn.preprocessing import OneHotEncoder
 from sklearn.utils.metaestimators import _BaseComposition
 from sklearn2pmml.util import eval_expr_rows, fqn, Predicate
 
+import copy
 import numpy
 
 def _checkGBDTRegressor(gbdt):
 	if hasattr(gbdt, "apply"):
 		return gbdt
 	else:
 		try:
@@ -175,15 +176,15 @@
 class Link(BaseEstimator):
 
 	def __init__(self, estimator, augment_funcs, prefit = False):
 		self.estimator = estimator
 		self.augment_funcs = augment_funcs
 		self.prefit = prefit
 		if prefit:
-			self.estimator_ = clone(self.estimator)
+			self.estimator_ = copy.deepcopy(self.estimator)
 
 	def fit(self, X, y, **fit_params):
 		self.estimator_ = clone(self.estimator)
 		self.estimator_.fit(X, y, **fit_params)
 		return self
 
 	def predict(self, X):
@@ -218,34 +219,36 @@
 				raise ValueError()
 			y = numpy.asarray(y)
 		i = 0
 		for name, estimator, predicate in self.steps:
 			step_mask = eval_expr_rows(X, predicate, dtype = bool)
 			if numpy.sum(step_mask) < 1:
 				raise ValueError(predicate)
+			step_X = X[step_mask]
 			if len(y.shape) == 1:
 				step_y = y[step_mask]
 			elif len(y.shape) == 2:
 				step_y = y[step_mask, i]
 			else:
 				raise ValueError()
-			step_fit_params = _extract_step_params(name, fit_params)
-			estimator.fit(X[step_mask], step_y, **_mask_params(step_fit_params, step_mask))
+			step_fit_params = _mask_params(_extract_step_params(name, fit_params), step_mask)
+			estimator.fit(step_X, step_y, **step_fit_params)
 			if isinstance(estimator, Link):
 				X = estimator.augment(X)
 			i += 1
 		return self
 
 	def _predict(self, X, predict_method):
 		result = None
 		for name, estimator, predicate in self.steps:
 			step_mask = eval_expr_rows(X, predicate, dtype = bool)
 			if numpy.sum(step_mask) < 1:
 				continue
-			step_result = getattr(estimator, predict_method)(X[step_mask])
+			step_X = X[step_mask]
+			step_result = getattr(estimator, predict_method)(step_X)
 			step_result = _to_sparse(X, step_mask, step_result)
 			if self.multioutput:
 				step_result = step_result.reshape(X.shape[0], -1)
 			if result is None:
 				result = step_result
 			else:
 				if self.multioutput:
@@ -272,28 +275,31 @@
 	def fit(self, X, y, **fit_params):
 		mask = numpy.zeros(X.shape[0], dtype = bool)
 		for name, estimator, predicate in self.steps:
 			step_mask = eval_expr_rows(X, predicate, dtype = bool)
 			step_mask[mask] = False
 			if numpy.sum(step_mask) < 1:
 				raise ValueError(predicate)
-			step_fit_params = _extract_step_params(name, fit_params)
-			estimator.fit(X[step_mask], y[step_mask], **_mask_params(step_fit_params, step_mask))
+			step_X = X[step_mask]
+			step_y = y[step_mask]
+			step_fit_params = _mask_params(_extract_step_params(name, fit_params), step_mask)
+			estimator.fit(step_X, step_y, **step_fit_params)
 			mask = numpy.logical_or(mask, step_mask)
 		return self
 
 	def _predict(self, X, predict_method):
 		result = None
 		mask = numpy.zeros(X.shape[0], dtype = bool)
 		for name, estimator, predicate in self.steps:
 			step_mask = eval_expr_rows(X, predicate, dtype = bool)
 			step_mask[mask] = False
 			if numpy.sum(step_mask) < 1:
 				continue
-			step_result = getattr(estimator, predict_method)(X[step_mask])
+			step_X = X[step_mask]
+			step_result = getattr(estimator, predict_method)(step_X)
 			step_result = _to_sparse(X, step_mask, step_result)
 			if result is None:
 				result = step_result
 			else:
 				result[step_mask] = step_result[step_mask]
 			mask = numpy.logical_or(mask, step_mask)
 		return result
```

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/statsmodels.py` & `sklearn2pmml-0.93.0/sklearn2pmml/statsmodels.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from pandas import CategoricalDtype
 from sklearn.base import BaseEstimator, ClassifierMixin, RegressorMixin
 from statsmodels.base.model import Model
 from statsmodels.tools import add_constant
 
 import numpy
 
 class StatsModelsEstimator(BaseEstimator):
@@ -68,14 +69,58 @@
 		if self.fit_intercept:
 			X = add_constant(X, has_constant = "add")
 		proba = self.results_.predict(X, **predict_proba_params)
 		if proba.ndim == 1:
 			proba = numpy.vstack((1 - proba, proba)).T
 		return proba
 
+class StatsModelsOrdinalClassifier(StatsModelsEstimator):
+
+	def __init__(self, model_class, **init_params):
+		super(StatsModelsOrdinalClassifier, self).__init__(model_class = model_class, fit_intercept = False, **init_params)
+
+	def regression_table_(self):
+		params = self.results_.params
+		coef_params = params[0:-(len(self.classes_) - 1)]
+		return coef_params.T
+
+	@property
+	def coef_(self):
+		reg_table = self.regression_table_()
+		return reg_table
+
+	@property
+	def intercept_(self):
+		if hasattr(self.results_, "offset"):
+			return self.results_.offset
+		return 0.0
+
+	@property
+	def threshold_(self):
+		params = self.results_.params
+		th_params = params[-(len(self.classes_) - 1):]
+		return th_params.T
+
+	def fit(self, X, y, **fit_params):
+		dtype = y.dtype
+		if (not isinstance(dtype, CategoricalDtype)) or (not dtype.ordered):
+			raise TypeError()
+		self.classes_ = numpy.asarray(dtype.categories)
+		super(StatsModelsOrdinalClassifier, self).fit(X = X, y = y, **fit_params)
+		return self
+
+	def predict(self, X, **predict_params):
+		proba = self.predict_proba(X, **predict_params)
+		indices = numpy.argmax(proba, axis = 1)
+		return numpy.take(self.classes_, indices)
+
+	def predict_proba(self, X, **predict_proba_params):
+		proba = self.results_.predict(X, **predict_proba_params)
+		return proba
+
 class StatsModelsRegressor(StatsModelsEstimator, RegressorMixin):
 
 	def __init__(self, model_class, fit_intercept = True, **init_params):
 		super(StatsModelsRegressor, self).__init__(model_class = model_class, fit_intercept = fit_intercept, **init_params)
 
 	def regression_table_(self):
 		return self.results_.params.T
```

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/feature_selection/__init__.py` & `sklearn2pmml-0.93.0/sklearn2pmml/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/postprocessing/__init__.py` & `sklearn2pmml-0.93.0/sklearn2pmml/postprocessing/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from sklearn.base import clone, BaseEstimator, TransformerMixin
 from sklearn2pmml.preprocessing import ExpressionTransformer
 
+import copy
+
 class BusinessDecisionTransformer(BaseEstimator, TransformerMixin):
 
 	def __init__(self, transformer, business_problem, decisions, prefit = True):
 		if transformer is None:
 			pass
 		elif isinstance(transformer, str):
 			pass
@@ -18,28 +20,30 @@
 			if type(decision) is not tuple:
 				raise TypeError("Decision is not a tuple")
 			if len(decision) != 2:
 				raise TypeError("Decision is not a two-element (value, description) tuple")
 		self.decisions = decisions
 		self.prefit = prefit
 		if prefit:
-			self.transformer_ = self._make_transformer()
+			self.transformer_ = self._make_transformer(prefit = True)
 
-	def _make_transformer(self):
+	def _make_transformer(self, prefit = True):
 		if self.transformer is None:
 			return None
 		elif isinstance(self.transformer, str):
 			return ExpressionTransformer(self.transformer)
 		elif isinstance(self.transformer, TransformerMixin):
+			if prefit:
+				return copy.deepcopy(self.transformer)
 			return clone(self.transformer)
 		else:
 			raise TypeError("The transformer object is not an instance of {0}".format(TransformerMixin.__name__))
 
 	def fit(self, X, y = None):
-		self.transformer_ = self._make_transformer()
+		self.transformer_ = self._make_transformer(prefit = False)
 		if self.transformer_ is not None:
 			if y is None:
 				self.transformer_.fit(X)
 			else:
 				self.transformer_.fit(X, y)
 		return self
```

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/jaxb-core-3.0.2.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/jaxb-core-3.0.2.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-lightgbm-1.4.5.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-lightgbm-1.4.5.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/slf4j-api-1.7.36.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/slf4j-api-1.7.36.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/jackson-annotations-2.13.3.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/jackson-annotations-2.13.3.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/jcommander-1.72.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/jcommander-1.72.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-model-1.6.4.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-model-1.6.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/pickle-1.3.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/pickle-1.3.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/h2o-genmodel-3.40.0.4.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/h2o-genmodel-3.40.0.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-converter-1.5.4.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-converter-1.5.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/ubjson-gson-0.1.8.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/ubjson-gson-0.1.8.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.28.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.29.jar`

 * *Files 11% similar despite different names*

#### zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 7977 bytes, number of entries: 15
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-May-17 09:50 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 xgboost/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 xgboost/sklearn/
--rw-rw-r--  2.0 unx      364 b- defN 23-May-17 09:50 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx      168 b- defN 23-May-17 09:50 xgboost/sklearn/HasBooster.class
--rw-rw-r--  2.0 unx     2270 b- defN 23-May-17 09:50 xgboost/sklearn/XGBClassifier.class
--rw-rw-r--  2.0 unx     2210 b- defN 23-May-17 09:50 xgboost/sklearn/Booster.class
--rw-rw-r--  2.0 unx     2246 b- defN 23-May-17 09:50 xgboost/sklearn/XGBRegressor.class
--rw-rw-r--  2.0 unx     4204 b- defN 23-May-17 09:50 xgboost/sklearn/BoosterUtil.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/
--rw-rw-r--  2.0 unx     1453 b- defN 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml
--rw-rw-r--  2.0 unx      116 b- defN 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.properties
-15 files, 13161 bytes uncompressed, 5921 bytes compressed:  55.0%
+Zip file size: 7978 bytes, number of entries: 15
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Jun-06 10:35 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 xgboost/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 xgboost/sklearn/
+-rw-rw-r--  2.0 unx      364 b- defN 23-Jun-06 10:35 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx      168 b- defN 23-Jun-06 10:35 xgboost/sklearn/HasBooster.class
+-rw-rw-r--  2.0 unx     2270 b- defN 23-Jun-06 10:35 xgboost/sklearn/XGBClassifier.class
+-rw-rw-r--  2.0 unx     2210 b- defN 23-Jun-06 10:35 xgboost/sklearn/Booster.class
+-rw-rw-r--  2.0 unx     2246 b- defN 23-Jun-06 10:35 xgboost/sklearn/XGBRegressor.class
+-rw-rw-r--  2.0 unx     4204 b- defN 23-Jun-06 10:35 xgboost/sklearn/BoosterUtil.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/
+-rw-rw-r--  2.0 unx     1453 b- defN 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml
+-rw-rw-r--  2.0 unx      116 b- defN 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.properties
+15 files, 13161 bytes uncompressed, 5922 bytes compressed:  55.0%
```

#### META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.28</version>
+    <version>1.7.29</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-xgboost</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn XGBoost converter</name>
   <description>JPMML Scikit-Learn XGBoost to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Wed May 17 09:50:31 EEST 2023
-version=1.7.28
+#Tue Jun 06 10:35:43 EEST 2023
+version=1.7.29
 groupId=org.jpmml
 artifactId=pmml-sklearn-xgboost
```

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/guava-21.0.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/guava-21.0.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-statsmodels-1.0.2.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-statsmodels-1.0.3.jar`

 * *Files 26% similar despite different names*

#### zipinfo {}

```diff
@@ -1,41 +1,49 @@
-Zip file size: 27449 bytes, number of entries: 39
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-28 21:11 META-INF/
--rw-r--r--  2.0 unx      162 b- defN 23-Mar-28 21:11 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-28 21:11 org/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-28 21:11 org/jpmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-28 21:11 org/jpmml/statsmodels/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-28 21:11 org/jpmml/statsmodels/testing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-28 21:11 statsmodels/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-28 21:11 statsmodels/data/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-28 21:11 statsmodels/discrete/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-28 21:11 statsmodels/regression/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-28 21:11 statsmodels/genmod/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-28 21:11 META-INF/maven/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-28 21:11 META-INF/maven/org.jpmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-28 21:11 META-INF/maven/org.jpmml/pmml-statsmodels/
--rw-rw-r--  2.0 unx     2068 b- defN 23-Mar-28 21:11 META-INF/statsmodels2pmml.properties
--rw-rw-r--  2.0 unx      741 b- defN 23-Mar-28 21:11 org/jpmml/statsmodels/InterceptFeature.class
--rw-rw-r--  2.0 unx     1959 b- defN 23-Mar-28 21:11 org/jpmml/statsmodels/testing/StatsModelsEncoderBatchTest.class
--rw-rw-r--  2.0 unx     1839 b- defN 23-Mar-28 21:11 org/jpmml/statsmodels/testing/StatsModelsEncoderBatchTest$1.class
--rw-rw-r--  2.0 unx     2015 b- defN 23-Mar-28 21:11 org/jpmml/statsmodels/testing/StatsModelsEncoderBatch.class
--rw-rw-r--  2.0 unx      671 b- defN 23-Mar-28 21:11 org/jpmml/statsmodels/StatsModelsEncoder.class
--rw-rw-r--  2.0 unx     1425 b- defN 23-Mar-28 21:11 statsmodels/data/ModelData$Cache.class
--rw-rw-r--  2.0 unx     2653 b- defN 23-Mar-28 21:11 statsmodels/data/ModelData.class
--rw-rw-r--  2.0 unx     2299 b- defN 23-Mar-28 21:11 statsmodels/Results.class
--rw-rw-r--  2.0 unx     1706 b- defN 23-Mar-28 21:11 statsmodels/discrete/BinaryModel.class
--rw-rw-r--  2.0 unx      427 b- defN 23-Mar-28 21:11 statsmodels/discrete/DiscreteModel.class
--rw-rw-r--  2.0 unx     1731 b- defN 23-Mar-28 21:11 statsmodels/discrete/Logit.class
--rw-rw-r--  2.0 unx     4417 b- defN 23-Mar-28 21:11 statsmodels/discrete/MNLogit.class
--rw-rw-r--  2.0 unx     1714 b- defN 23-Mar-28 21:11 statsmodels/discrete/Poisson.class
--rw-rw-r--  2.0 unx     2941 b- defN 23-Mar-28 21:11 statsmodels/discrete/MultinomialRegressionModel.class
--rw-rw-r--  2.0 unx      414 b- defN 23-Mar-28 21:11 statsmodels/discrete/CountModel.class
--rw-rw-r--  2.0 unx     6513 b- defN 23-Mar-28 21:11 statsmodels/Model.class
--rw-rw-r--  2.0 unx     1110 b- defN 23-Mar-28 21:11 statsmodels/ResultsWrapper.class
--rw-rw-r--  2.0 unx     1753 b- defN 23-Mar-28 21:11 statsmodels/regression/LinearRegression.class
--rw-rw-r--  2.0 unx     2395 b- defN 23-Mar-28 21:11 statsmodels/regression/RegressionModel.class
--rw-rw-r--  2.0 unx     8159 b- defN 23-Mar-28 21:11 statsmodels/genmod/GLM.class
--rw-rw-r--  2.0 unx      591 b- defN 23-Mar-28 21:11 statsmodels/genmod/Link.class
--rw-rw-r--  2.0 unx      615 b- defN 23-Mar-28 21:11 statsmodels/genmod/Family.class
--rw-rw-r--  2.0 unx     1837 b- defN 23-Mar-28 21:10 META-INF/maven/org.jpmml/pmml-statsmodels/pom.xml
--rw-rw-r--  2.0 unx       60 b- defN 23-Mar-28 21:11 META-INF/maven/org.jpmml/pmml-statsmodels/pom.properties
-39 files, 52215 bytes uncompressed, 21899 bytes compressed:  58.1%
+Zip file size: 34545 bytes, number of entries: 47
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-30 11:51 META-INF/
+-rw-r--r--  2.0 unx      162 b- defN 23-May-30 11:51 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 11:50 org/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 11:50 org/jpmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 11:50 org/jpmml/statsmodels/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 11:50 org/jpmml/statsmodels/testing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 11:50 statsmodels/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 11:50 statsmodels/miscmodels/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 11:50 statsmodels/data/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 11:50 statsmodels/discrete/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 11:50 statsmodels/regression/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 11:50 statsmodels/genmod/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 11:50 scipy/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 11:50 scipy/stats/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-30 11:51 META-INF/maven/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-30 11:51 META-INF/maven/org.jpmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-30 11:51 META-INF/maven/org.jpmml/pmml-statsmodels/
+-rw-rw-r--  2.0 unx     2327 b- defN 23-May-30 11:50 META-INF/statsmodels2pmml.properties
+-rw-rw-r--  2.0 unx      137 b- defN 23-May-30 11:50 META-INF/python2pmml.properties
+-rw-rw-r--  2.0 unx      741 b- defN 23-May-30 11:50 org/jpmml/statsmodels/InterceptFeature.class
+-rw-rw-r--  2.0 unx     1959 b- defN 23-May-30 11:50 org/jpmml/statsmodels/testing/StatsModelsEncoderBatchTest.class
+-rw-rw-r--  2.0 unx     1839 b- defN 23-May-30 11:50 org/jpmml/statsmodels/testing/StatsModelsEncoderBatchTest$1.class
+-rw-rw-r--  2.0 unx     2015 b- defN 23-May-30 11:50 org/jpmml/statsmodels/testing/StatsModelsEncoderBatch.class
+-rw-rw-r--  2.0 unx     3688 b- defN 23-May-30 11:50 org/jpmml/statsmodels/OrdinalLabel.class
+-rw-rw-r--  2.0 unx      671 b- defN 23-May-30 11:50 org/jpmml/statsmodels/StatsModelsEncoder.class
+-rw-rw-r--  2.0 unx     9305 b- defN 23-May-30 11:50 statsmodels/miscmodels/OrderedModel.class
+-rw-rw-r--  2.0 unx     1425 b- defN 23-May-30 11:50 statsmodels/data/ModelData$Cache.class
+-rw-rw-r--  2.0 unx     2653 b- defN 23-May-30 11:50 statsmodels/data/ModelData.class
+-rw-rw-r--  2.0 unx     2299 b- defN 23-May-30 11:50 statsmodels/Results.class
+-rw-rw-r--  2.0 unx     1706 b- defN 23-May-30 11:50 statsmodels/discrete/BinaryModel.class
+-rw-rw-r--  2.0 unx      427 b- defN 23-May-30 11:50 statsmodels/discrete/DiscreteModel.class
+-rw-rw-r--  2.0 unx     1731 b- defN 23-May-30 11:50 statsmodels/discrete/Logit.class
+-rw-rw-r--  2.0 unx     4417 b- defN 23-May-30 11:50 statsmodels/discrete/MNLogit.class
+-rw-rw-r--  2.0 unx     1714 b- defN 23-May-30 11:50 statsmodels/discrete/Poisson.class
+-rw-rw-r--  2.0 unx     2941 b- defN 23-May-30 11:50 statsmodels/discrete/MultinomialRegressionModel.class
+-rw-rw-r--  2.0 unx      414 b- defN 23-May-30 11:50 statsmodels/discrete/CountModel.class
+-rw-rw-r--  2.0 unx     6687 b- defN 23-May-30 11:50 statsmodels/Model.class
+-rw-rw-r--  2.0 unx     1110 b- defN 23-May-30 11:50 statsmodels/ResultsWrapper.class
+-rw-rw-r--  2.0 unx     1753 b- defN 23-May-30 11:50 statsmodels/regression/LinearRegression.class
+-rw-rw-r--  2.0 unx     2395 b- defN 23-May-30 11:50 statsmodels/regression/RegressionModel.class
+-rw-rw-r--  2.0 unx     8223 b- defN 23-May-30 11:50 statsmodels/genmod/GLM.class
+-rw-rw-r--  2.0 unx      591 b- defN 23-May-30 11:50 statsmodels/genmod/Link.class
+-rw-rw-r--  2.0 unx      615 b- defN 23-May-30 11:50 statsmodels/genmod/Family.class
+-rw-rw-r--  2.0 unx      388 b- defN 23-May-30 11:50 scipy/stats/RVGeneric.class
+-rw-rw-r--  2.0 unx      559 b- defN 23-May-30 11:50 scipy/stats/RVContinuous.class
+-rw-rw-r--  2.0 unx     1837 b- defN 23-May-30 11:50 META-INF/maven/org.jpmml/pmml-statsmodels/pom.xml
+-rw-rw-r--  2.0 unx       60 b- defN 23-May-30 11:51 META-INF/maven/org.jpmml/pmml-statsmodels/pom.properties
+47 files, 66789 bytes uncompressed, 27967 bytes compressed:  58.1%
```

#### zipnote «TEMP»/diffoscope__evcigd9_/tmp88lnevlz_.zip

```diff
@@ -15,53 +15,71 @@
 
 Filename: org/jpmml/statsmodels/testing/
 Comment: 
 
 Filename: statsmodels/
 Comment: 
 
+Filename: statsmodels/miscmodels/
+Comment: 
+
 Filename: statsmodels/data/
 Comment: 
 
 Filename: statsmodels/discrete/
 Comment: 
 
 Filename: statsmodels/regression/
 Comment: 
 
 Filename: statsmodels/genmod/
 Comment: 
 
+Filename: scipy/
+Comment: 
+
+Filename: scipy/stats/
+Comment: 
+
 Filename: META-INF/maven/
 Comment: 
 
 Filename: META-INF/maven/org.jpmml/
 Comment: 
 
 Filename: META-INF/maven/org.jpmml/pmml-statsmodels/
 Comment: 
 
 Filename: META-INF/statsmodels2pmml.properties
 Comment: 
 
+Filename: META-INF/python2pmml.properties
+Comment: 
+
 Filename: org/jpmml/statsmodels/InterceptFeature.class
 Comment: 
 
 Filename: org/jpmml/statsmodels/testing/StatsModelsEncoderBatchTest.class
 Comment: 
 
 Filename: org/jpmml/statsmodels/testing/StatsModelsEncoderBatchTest$1.class
 Comment: 
 
 Filename: org/jpmml/statsmodels/testing/StatsModelsEncoderBatch.class
 Comment: 
 
+Filename: org/jpmml/statsmodels/OrdinalLabel.class
+Comment: 
+
 Filename: org/jpmml/statsmodels/StatsModelsEncoder.class
 Comment: 
 
+Filename: statsmodels/miscmodels/OrderedModel.class
+Comment: 
+
 Filename: statsmodels/data/ModelData$Cache.class
 Comment: 
 
 Filename: statsmodels/data/ModelData.class
 Comment: 
 
 Filename: statsmodels/Results.class
@@ -105,14 +123,20 @@
 
 Filename: statsmodels/genmod/Link.class
 Comment: 
 
 Filename: statsmodels/genmod/Family.class
 Comment: 
 
+Filename: scipy/stats/RVGeneric.class
+Comment: 
+
+Filename: scipy/stats/RVContinuous.class
+Comment: 
+
 Filename: META-INF/maven/org.jpmml/pmml-statsmodels/pom.xml
 Comment: 
 
 Filename: META-INF/maven/org.jpmml/pmml-statsmodels/pom.properties
 Comment: 
 
 Zip file comment:
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,6 +1,6 @@
 Manifest-Version: 1.0
 Implementation-Title: JPMML-StatsModels library
-Implementation-Version: 1.0.2
+Implementation-Version: 1.0.3
 Build-Jdk-Spec: 1.8
 Created-By: Maven JAR Plugin 3.3.0
```

#### META-INF/statsmodels2pmml.properties

```diff
@@ -11,16 +11,19 @@
 statsmodels.discrete.discrete_model.MNLogit = statsmodels.discrete.MNLogit
 statsmodels.discrete.discrete_model.MultinomialResults = statsmodels.Results
 statsmodels.discrete.discrete_model.MultinomialResultsWrapper = statsmodels.ResultsWrapper
 statsmodels.discrete.discrete_model.Poisson = statsmodels.discrete.Poisson
 statsmodels.discrete.discrete_model.PoissonResults = statsmodels.Results
 statsmodels.discrete.discrete_model.PoissonResultsWrapper = statsmodels.ResultsWrapper
 statsmodels.genmod.families.family.(Binomial|Gaussian|Poisson) = statsmodels.genmod.Family
-statsmodels.genmod.families.links.(identity|Log|Logit|) = statsmodels.genmod.Link
+statsmodels.genmod.families.links.(identity|Identity|Log|Logit|) = statsmodels.genmod.Link
 statsmodels.genmod.generalized_linear_model.GLM = statsmodels.genmod.GLM
 statsmodels.genmod.generalized_linear_model.GLMResults = statsmodels.Results
 statsmodels.genmod.generalized_linear_model.GLMResultsWrapper = statsmodels.ResultsWrapper
+statsmodels.miscmodels.ordinal_model.OrderedModel = statsmodels.miscmodels.OrderedModel
+statsmodels.miscmodels.ordinal_model.OrderedResults = statsmodels.Results
+statsmodels.miscmodels.ordinal_model.OrderedResultsWrapper = statsmodels.ResultsWrapper
 statsmodels.regression.linear_model.OLS = statsmodels.regression.LinearRegression
 statsmodels.regression.linear_model.OLSResults = statsmodels.Results
 statsmodels.regression.linear_model.WLS = statsmodels.regression.LinearRegression
 statsmodels.regression.linear_model.RegressionResults = statsmodels.Results
 statsmodels.regression.linear_model.RegressionResultsWrapper = statsmodels.ResultsWrapper
```

#### statsmodels/Model.class

##### procyon -ec {}

```diff
@@ -116,14 +116,22 @@
         return (ModelData)this.get("data", (Class)ModelData.class);
     }
     
     public Integer getKConstant() {
         return this.getInteger("k_constant");
     }
     
+    public Integer getKExtra() {
+        return this.getInteger("k_extra");
+    }
+    
+    public Integer getKVars() {
+        return this.getInteger("k_vars");
+    }
+    
     protected static List<? extends Feature> dropInterceptFeature(List<? extends Feature> features, final int index) {
         final Feature feature = (Feature)features.get(index);
         if (feature instanceof InterceptFeature) {
             final InterceptFeature interceptFeature = (InterceptFeature)feature;
             features = new ArrayList<Feature>(features);
             features.remove(interceptFeature);
             return features;
```

#### statsmodels/genmod/GLM.class

##### procyon -ec {}

```diff
@@ -201,37 +201,45 @@
             case -135761730: {
                 if (pythonName.equals("identity")) {
                     n = 0;
                     break;
                 }
                 break;
             }
+            case -71117602: {
+                if (pythonName.equals("Identity")) {
+                    n = 1;
+                    break;
+                }
+                break;
+            }
             case 76580: {
                 if (pythonName.equals("Log")) {
-                    n = 1;
+                    n = 2;
                     break;
                 }
                 break;
             }
             case 73596751: {
                 if (pythonName.equals("Logit")) {
-                    n = 2;
+                    n = 3;
                     break;
                 }
                 break;
             }
         }
         switch (n) {
-            case 0: {
+            case 0:
+            case 1: {
                 return GeneralRegressionModel.LinkFunction.IDENTITY;
             }
-            case 1: {
+            case 2: {
                 return GeneralRegressionModel.LinkFunction.LOG;
             }
-            case 2: {
+            case 3: {
                 return GeneralRegressionModel.LinkFunction.LOGIT;
             }
             default: {
                 throw new IllegalArgumentException(linkName);
             }
         }
     }
@@ -244,33 +252,41 @@
             case -135761730: {
                 if (pythonName.equals("identity")) {
                     n = 0;
                     break;
                 }
                 break;
             }
+            case -71117602: {
+                if (pythonName.equals("Identity")) {
+                    n = 1;
+                    break;
+                }
+                break;
+            }
             case 76580: {
                 if (pythonName.equals("Log")) {
-                    n = 1;
+                    n = 2;
                     break;
                 }
                 break;
             }
             case 73596751: {
                 if (pythonName.equals("Logit")) {
-                    n = 2;
+                    n = 3;
                     break;
                 }
                 break;
             }
         }
         switch (n) {
             case 0:
             case 1:
-            case 2: {
+            case 2:
+            case 3: {
                 return null;
             }
             default: {
                 throw new IllegalArgumentException(linkName);
             }
         }
     }
```

#### META-INF/maven/org.jpmml/pmml-statsmodels/pom.xml

##### META-INF/maven/org.jpmml/pmml-statsmodels/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-statsmodels</artifactId>
-    <version>1.0.2</version>
+    <version>1.0.3</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-statsmodels</artifactId>
   <packaging>jar</packaging>
   <name>JPMML StatsModels converter</name>
   <description>JPMML StatsModels to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-statsmodels/pom.properties

```diff
@@ -1,3 +1,3 @@
 artifactId=pmml-statsmodels
 groupId=org.jpmml
-version=1.0.2
+version=1.0.3
```

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/ubjson-0.1.8.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/ubjson-0.1.8.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-python-1.1.14.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-python-1.1.14.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-sklearn-1.7.28.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-sklearn-1.7.29.jar`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,405 +1,405 @@
-Zip file size: 466641 bytes, number of entries: 403
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/
--rw-r--r--  2.0 unx      159 b- defN 23-May-17 09:50 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn_pandas/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 chaid/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 stop_words/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/calibration/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/pipeline/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/dummy/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/svm/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/neural_network/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/impute/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/naive_bayes/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/linear_model/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/linear_model/logistic/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/linear_model/ridge/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/linear_model/glm/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/linear_model/stochastic_gradient/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/compose/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/model_selection/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/decomposition/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/neighbors/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/multioutput/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/isotonic/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/feature_extraction/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/feature_extraction/text/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/metrics/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/ensemble/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/ensemble/bagging/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/ensemble/stacking/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/ensemble/gradient_boosting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/ensemble/forest/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/ensemble/iforest/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/ensemble/voting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/ensemble/hist_gradient_boosting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/ensemble/weight_boosting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/feature_selection/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/loss/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/discriminant_analysis/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/preprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/tree/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/tree/visitors/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/cluster/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn/multiclass/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/ruleset/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/pipeline/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/decoration/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/neural_network/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/util/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/feature_extraction/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/feature_extraction/text/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/ensemble/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/feature_selection/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/postprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/preprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/tree/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/expression/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 org/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 org/jpmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 org/jpmml/sklearn/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 org/jpmml/sklearn/testing/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/org.jpmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn/
--rw-rw-r--  2.0 unx    16829 b- defN 23-May-17 09:50 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx     2287 b- defN 23-May-17 09:50 sklearn_pandas/CategoricalImputer.class
--rw-rw-r--  2.0 unx      656 b- defN 23-May-17 09:50 sklearn_pandas/TransformerPipeline.class
--rw-rw-r--  2.0 unx     1154 b- defN 23-May-17 09:50 sklearn_pandas/DataFrameMapper$2.class
--rw-rw-r--  2.0 unx     6280 b- defN 23-May-17 09:50 sklearn_pandas/DataFrameMapper.class
--rw-rw-r--  2.0 unx     1126 b- defN 23-May-17 09:50 sklearn_pandas/DataFrameMapper$1.class
--rw-rw-r--  2.0 unx      609 b- defN 23-May-17 09:50 chaid/ContinuousColumn.class
--rw-rw-r--  2.0 unx      925 b- defN 23-May-17 09:50 chaid/Node.class
--rw-rw-r--  2.0 unx      467 b- defN 23-May-17 09:50 chaid/Column.class
--rw-rw-r--  2.0 unx     3283 b- defN 23-May-17 09:50 chaid/Split.class
--rw-rw-r--  2.0 unx      401 b- defN 23-May-17 09:50 chaid/InvalidSplitReason.class
--rw-rw-r--  2.0 unx      602 b- defN 23-May-17 09:50 chaid/NominalColumn.class
--rw-rw-r--  2.0 unx     1912 b- defN 23-May-17 09:50 stop_words/english.txt
--rw-rw-r--  2.0 unx      147 b- defN 23-May-17 09:50 sklearn/HasHead.class
--rw-rw-r--  2.0 unx     1728 b- defN 23-May-17 09:50 sklearn/StepUtil.class
--rw-rw-r--  2.0 unx    11436 b- defN 23-May-17 09:50 sklearn/calibration/CalibratedClassifier.class
--rw-rw-r--  2.0 unx     2972 b- defN 23-May-17 09:50 sklearn/calibration/SigmoidCalibration.class
--rw-rw-r--  2.0 unx      683 b- defN 23-May-17 09:50 sklearn/calibration/CalibratedClassifier$1.class
--rw-rw-r--  2.0 unx     1475 b- defN 23-May-17 09:50 sklearn/calibration/CalibratedClassifierCV.class
--rw-rw-r--  2.0 unx     1862 b- defN 23-May-17 09:50 sklearn/pipeline/PipelineTransformer.class
--rw-rw-r--  2.0 unx     1671 b- defN 23-May-17 09:50 sklearn/pipeline/Pipeline$2.class
--rw-rw-r--  2.0 unx     2536 b- defN 23-May-17 09:50 sklearn/pipeline/FeatureUnion.class
--rw-rw-r--  2.0 unx     5062 b- defN 23-May-17 09:50 sklearn/pipeline/Pipeline.class
--rw-rw-r--  2.0 unx     2003 b- defN 23-May-17 09:50 sklearn/pipeline/PipelineRegressor.class
--rw-rw-r--  2.0 unx     1773 b- defN 23-May-17 09:50 sklearn/pipeline/Pipeline$1.class
--rw-rw-r--  2.0 unx     1111 b- defN 23-May-17 09:50 sklearn/pipeline/PipelineUtil.class
--rw-rw-r--  2.0 unx     2298 b- defN 23-May-17 09:50 sklearn/pipeline/PipelineClassifier.class
--rw-rw-r--  2.0 unx     4973 b- defN 23-May-17 09:50 sklearn/dummy/DummyClassifier.class
--rw-rw-r--  2.0 unx     2055 b- defN 23-May-17 09:50 sklearn/dummy/DummyRegressor.class
--rw-rw-r--  2.0 unx      454 b- defN 23-May-17 09:50 sklearn/SkLearnFields.class
--rw-rw-r--  2.0 unx     2293 b- defN 23-May-17 09:50 sklearn/SkLearnOutlierTransformation.class
--rw-rw-r--  2.0 unx      240 b- defN 23-May-17 09:50 sklearn/HasEstimator.class
--rw-rw-r--  2.0 unx     1182 b- defN 23-May-17 09:50 sklearn/HasMultiApplyField.class
--rw-rw-r--  2.0 unx      908 b- defN 23-May-17 09:50 sklearn/None.class
--rw-rw-r--  2.0 unx     2393 b- defN 23-May-17 09:50 sklearn/svm/SupportVectorMachineUtil.class
--rw-rw-r--  2.0 unx     2052 b- defN 23-May-17 09:50 sklearn/svm/OneClassSVMUtil.class
--rw-rw-r--  2.0 unx     1439 b- defN 23-May-17 09:50 sklearn/svm/OneClassSVMUtil$1.class
--rw-rw-r--  2.0 unx     1109 b- defN 23-May-17 09:50 sklearn/svm/LinearSVC.class
--rw-rw-r--  2.0 unx     5037 b- defN 23-May-17 09:50 sklearn/svm/LibSVMClassifier.class
--rw-rw-r--  2.0 unx      966 b- defN 23-May-17 09:50 sklearn/svm/SupportVectorMachineUtil$1.class
--rw-rw-r--  2.0 unx     1274 b- defN 23-May-17 09:50 sklearn/svm/OneClassSVM.class
--rw-rw-r--  2.0 unx     3594 b- defN 23-May-17 09:50 sklearn/svm/LibSVMRegressor.class
--rw-rw-r--  2.0 unx     4114 b- defN 23-May-17 09:50 sklearn/InitializerUtil$1.class
--rw-rw-r--  2.0 unx      735 b- defN 23-May-17 09:50 sklearn/Estimator$1.class
--rw-rw-r--  2.0 unx      214 b- defN 23-May-17 09:50 sklearn/HasNumberOfFeatures.class
--rw-rw-r--  2.0 unx      660 b- defN 23-May-17 09:50 sklearn/MultiTransformer.class
--rw-rw-r--  2.0 unx     2110 b- defN 23-May-17 09:50 sklearn/neural_network/MLPRegressor.class
--rw-rw-r--  2.0 unx     2633 b- defN 23-May-17 09:50 sklearn/neural_network/MLPClassifier.class
--rw-rw-r--  2.0 unx      759 b- defN 23-May-17 09:50 sklearn/neural_network/MultilayerPerceptronUtil$1.class
--rw-rw-r--  2.0 unx    11996 b- defN 23-May-17 09:50 sklearn/neural_network/MultilayerPerceptronUtil.class
--rw-rw-r--  2.0 unx     1880 b- defN 23-May-17 09:50 sklearn/Step.class
--rw-rw-r--  2.0 unx      168 b- defN 23-May-17 09:50 sklearn/HasDefaultValue.class
--rw-rw-r--  2.0 unx     2936 b- defN 23-May-17 09:50 sklearn/impute/MissingIndicator.class
--rw-rw-r--  2.0 unx     4027 b- defN 23-May-17 09:50 sklearn/impute/ImputerUtil.class
--rw-rw-r--  2.0 unx     5703 b- defN 23-May-17 09:50 sklearn/impute/SimpleImputer.class
--rw-rw-r--  2.0 unx     7021 b- defN 23-May-17 09:50 sklearn/naive_bayes/GaussianNB.class
--rw-rw-r--  2.0 unx     4460 b- defN 23-May-17 09:50 sklearn/linear_model/LinearRegressor.class
--rw-rw-r--  2.0 unx     4715 b- defN 23-May-17 09:50 sklearn/linear_model/LinearClassifier.class
--rw-rw-r--  2.0 unx     7535 b- defN 23-May-17 09:50 sklearn/linear_model/logistic/LogisticRegression.class
--rw-rw-r--  2.0 unx     1042 b- defN 23-May-17 09:50 sklearn/linear_model/ridge/RidgeClassifier.class
--rw-rw-r--  2.0 unx      596 b- defN 23-May-17 09:50 sklearn/linear_model/glm/DistributionBoundary.class
--rw-rw-r--  2.0 unx     1601 b- defN 23-May-17 09:50 sklearn/linear_model/glm/GeneralizedLinearRegressor.class
--rw-rw-r--  2.0 unx      911 b- defN 23-May-17 09:50 sklearn/linear_model/stochastic_gradient/Hinge.class
--rw-rw-r--  2.0 unx     2449 b- defN 23-May-17 09:50 sklearn/linear_model/stochastic_gradient/SGDOneClassSVM.class
--rw-rw-r--  2.0 unx      461 b- defN 23-May-17 09:50 sklearn/linear_model/stochastic_gradient/LossFunction.class
--rw-rw-r--  2.0 unx      452 b- defN 23-May-17 09:50 sklearn/linear_model/stochastic_gradient/Log.class
--rw-rw-r--  2.0 unx     1165 b- defN 23-May-17 09:50 sklearn/linear_model/stochastic_gradient/SGDClassifier.class
--rw-rw-r--  2.0 unx      482 b- defN 23-May-17 09:50 sklearn/linear_model/stochastic_gradient/ModifiedHuber.class
--rw-rw-r--  2.0 unx      932 b- defN 23-May-17 09:50 sklearn/linear_model/stochastic_gradient/SquaredHinge.class
--rw-rw-r--  2.0 unx     1720 b- defN 23-May-17 09:50 sklearn/compose/ColumnTransformer$1.class
--rw-rw-r--  2.0 unx     3239 b- defN 23-May-17 09:50 sklearn/compose/TransformedTargetRegressor.class
--rw-rw-r--  2.0 unx     3649 b- defN 23-May-17 09:50 sklearn/compose/ColumnTransformer.class
--rw-rw-r--  2.0 unx     1534 b- defN 23-May-17 09:50 sklearn/compose/TransformedTargetRegressor$1.class
--rw-rw-r--  2.0 unx     2825 b- defN 23-May-17 09:50 sklearn/Classifier.class
--rw-rw-r--  2.0 unx     1457 b- defN 23-May-17 09:50 sklearn/model_selection/EstimatorSearcher.class
--rw-rw-r--  2.0 unx     1685 b- defN 23-May-17 09:50 sklearn/Selector.class
--rw-rw-r--  2.0 unx      419 b- defN 23-May-17 09:50 sklearn/decomposition/IncrementalPCA.class
--rw-rw-r--  2.0 unx     3471 b- defN 23-May-17 09:50 sklearn/decomposition/TruncatedSVD.class
--rw-rw-r--  2.0 unx     4759 b- defN 23-May-17 09:50 sklearn/decomposition/PCA.class
--rw-rw-r--  2.0 unx      911 b- defN 23-May-17 09:50 sklearn/decomposition/BasePCA.class
--rw-rw-r--  2.0 unx      336 b- defN 23-May-17 09:50 sklearn/HasPredictField.class
--rw-rw-r--  2.0 unx     3018 b- defN 23-May-17 09:50 sklearn/neighbors/NearestNeighbors.class
--rw-rw-r--  2.0 unx     4505 b- defN 23-May-17 09:50 sklearn/neighbors/KNeighborsClassifier.class
--rw-rw-r--  2.0 unx     3794 b- defN 23-May-17 09:50 sklearn/neighbors/NearestCentroid.class
--rw-rw-r--  2.0 unx     2025 b- defN 23-May-17 09:50 sklearn/neighbors/BinaryTree.class
--rw-rw-r--  2.0 unx     1266 b- defN 23-May-17 09:50 sklearn/neighbors/KNeighborsUtil$1.class
--rw-rw-r--  2.0 unx      181 b- defN 23-May-17 09:50 sklearn/neighbors/HasMetric.class
--rw-rw-r--  2.0 unx    10748 b- defN 23-May-17 09:50 sklearn/neighbors/KNeighborsUtil.class
--rw-rw-r--  2.0 unx     4387 b- defN 23-May-17 09:50 sklearn/neighbors/KNeighborsRegressor.class
--rw-rw-r--  2.0 unx     1032 b- defN 23-May-17 09:50 sklearn/neighbors/DistanceMetric.class
--rw-rw-r--  2.0 unx      351 b- defN 23-May-17 09:50 sklearn/neighbors/HasTrainingData.class
--rw-rw-r--  2.0 unx      176 b- defN 23-May-17 09:50 sklearn/neighbors/HasNumberOfNeighbors.class
--rw-rw-r--  2.0 unx     2235 b- defN 23-May-17 09:50 sklearn/multioutput/MultiOutputUtil.class
--rw-rw-r--  2.0 unx     3383 b- defN 23-May-17 09:50 sklearn/multioutput/ChainUtil.class
--rw-rw-r--  2.0 unx     1601 b- defN 23-May-17 09:50 sklearn/multioutput/RegressorChain.class
--rw-rw-r--  2.0 unx     1316 b- defN 23-May-17 09:50 sklearn/multioutput/MultiOutputClassifier.class
--rw-rw-r--  2.0 unx     1310 b- defN 23-May-17 09:50 sklearn/multioutput/MultiOutputRegressor.class
--rw-rw-r--  2.0 unx     1745 b- defN 23-May-17 09:50 sklearn/multioutput/ClassifierChain.class
--rw-rw-r--  2.0 unx     4469 b- defN 23-May-17 09:50 sklearn/isotonic/IsotonicRegression.class
--rw-rw-r--  2.0 unx      326 b- defN 23-May-17 09:50 sklearn/HasApplyField.class
--rw-rw-r--  2.0 unx      273 b- defN 23-May-17 09:50 sklearn/HasEstimatorEnsemble.class
--rw-rw-r--  2.0 unx     1929 b- defN 23-May-17 09:50 sklearn/Transformer$1.class
--rw-rw-r--  2.0 unx      953 b- defN 23-May-17 09:50 sklearn/LabelEncoderClassifier.class
--rw-rw-r--  2.0 unx      937 b- defN 23-May-17 09:50 sklearn/PassThrough.class
--rw-rw-r--  2.0 unx      181 b- defN 23-May-17 09:50 sklearn/HasPriorProbability.class
--rw-rw-r--  2.0 unx     5693 b- defN 23-May-17 09:50 sklearn/feature_extraction/text/TfidfVectorizer.class
--rw-rw-r--  2.0 unx      809 b- defN 23-May-17 09:50 sklearn/feature_extraction/text/TfidfVectorizer$1.class
--rw-rw-r--  2.0 unx      675 b- defN 23-May-17 09:50 sklearn/feature_extraction/text/Tokenizer.class
--rw-rw-r--  2.0 unx    13329 b- defN 23-May-17 09:50 sklearn/feature_extraction/text/CountVectorizer.class
--rw-rw-r--  2.0 unx     2129 b- defN 23-May-17 09:50 sklearn/feature_extraction/text/CountVectorizer$1.class
--rw-rw-r--  2.0 unx     1433 b- defN 23-May-17 09:50 sklearn/feature_extraction/text/TfidfTransformer.class
--rw-rw-r--  2.0 unx     4031 b- defN 23-May-17 09:50 sklearn/feature_extraction/DictVectorizer.class
--rw-rw-r--  2.0 unx      762 b- defN 23-May-17 09:50 sklearn/Clusterer.class
--rw-rw-r--  2.0 unx     1375 b- defN 23-May-17 09:50 sklearn/metrics/DistanceMetric.class
--rw-rw-r--  2.0 unx     1069 b- defN 23-May-17 09:50 sklearn/ensemble/EnsembleUtil.class
--rw-rw-r--  2.0 unx     2112 b- defN 23-May-17 09:50 sklearn/ensemble/bagging/BaggingRegressor.class
--rw-rw-r--  2.0 unx     3293 b- defN 23-May-17 09:50 sklearn/ensemble/bagging/BaggingUtil.class
--rw-rw-r--  2.0 unx     3083 b- defN 23-May-17 09:50 sklearn/ensemble/bagging/BaggingClassifier.class
--rw-rw-r--  2.0 unx     1409 b- defN 23-May-17 09:50 sklearn/ensemble/EnsembleRegressor.class
--rw-rw-r--  2.0 unx     3485 b- defN 23-May-17 09:50 sklearn/ensemble/stacking/StackingClassifier.class
--rw-rw-r--  2.0 unx      495 b- defN 23-May-17 09:50 sklearn/ensemble/stacking/StackingUtil$PredictFunction.class
--rw-rw-r--  2.0 unx     3109 b- defN 23-May-17 09:50 sklearn/ensemble/stacking/StackingRegressor.class
--rw-rw-r--  2.0 unx     3706 b- defN 23-May-17 09:50 sklearn/ensemble/stacking/StackingUtil.class
--rw-rw-r--  2.0 unx     4851 b- defN 23-May-17 09:50 sklearn/ensemble/stacking/StackingClassifier$1.class
--rw-rw-r--  2.0 unx     2254 b- defN 23-May-17 09:50 sklearn/ensemble/stacking/StackingRegressor$1.class
--rw-rw-r--  2.0 unx      495 b- defN 23-May-17 09:50 sklearn/ensemble/gradient_boosting/ScaledLogOddsEstimator.class
--rw-rw-r--  2.0 unx     1440 b- defN 23-May-17 09:50 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$GradientBoostingClassifierProxy.class
--rw-rw-r--  2.0 unx     1862 b- defN 23-May-17 09:50 sklearn/ensemble/gradient_boosting/MultinomialDeviance.class
--rw-rw-r--  2.0 unx     2563 b- defN 23-May-17 09:50 sklearn/ensemble/gradient_boosting/GradientBoostingRegressor.class
--rw-rw-r--  2.0 unx      858 b- defN 23-May-17 09:50 sklearn/ensemble/gradient_boosting/LossFunction.class
--rw-rw-r--  2.0 unx     1588 b- defN 23-May-17 09:50 sklearn/ensemble/gradient_boosting/ExponentialLoss.class
--rw-rw-r--  2.0 unx     1317 b- defN 23-May-17 09:50 sklearn/ensemble/gradient_boosting/PriorProbabilityEstimator.class
--rw-rw-r--  2.0 unx     7718 b- defN 23-May-17 09:50 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier.class
--rw-rw-r--  2.0 unx     1288 b- defN 23-May-17 09:50 sklearn/ensemble/gradient_boosting/LogOddsEstimator.class
--rw-rw-r--  2.0 unx      960 b- defN 23-May-17 09:50 sklearn/ensemble/gradient_boosting/MeanEstimator.class
--rw-rw-r--  2.0 unx     1265 b- defN 23-May-17 09:50 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$1.class
--rw-rw-r--  2.0 unx      980 b- defN 23-May-17 09:50 sklearn/ensemble/gradient_boosting/QuantileEstimator.class
--rw-rw-r--  2.0 unx     1578 b- defN 23-May-17 09:50 sklearn/ensemble/gradient_boosting/BinomialDeviance.class
--rw-rw-r--  2.0 unx      811 b- defN 23-May-17 09:50 sklearn/ensemble/gradient_boosting/ZeroEstimator.class
--rw-rw-r--  2.0 unx     3003 b- defN 23-May-17 09:50 sklearn/ensemble/gradient_boosting/GradientBoostingUtil.class
--rw-rw-r--  2.0 unx     1148 b- defN 23-May-17 09:50 sklearn/ensemble/EnsembleUtil$1.class
--rw-rw-r--  2.0 unx     3059 b- defN 23-May-17 09:50 sklearn/ensemble/forest/ForestUtil.class
--rw-rw-r--  2.0 unx     2558 b- defN 23-May-17 09:50 sklearn/ensemble/forest/ForestRegressor.class
--rw-rw-r--  2.0 unx     3078 b- defN 23-May-17 09:50 sklearn/ensemble/forest/ForestClassifier.class
--rw-rw-r--  2.0 unx     1752 b- defN 23-May-17 09:50 sklearn/ensemble/iforest/IsolationForest$3.class
--rw-rw-r--  2.0 unx     2206 b- defN 23-May-17 09:50 sklearn/ensemble/iforest/IsolationForest$1.class
--rw-rw-r--  2.0 unx     2050 b- defN 23-May-17 09:50 sklearn/ensemble/iforest/IsolationForest$4.class
--rw-rw-r--  2.0 unx     1716 b- defN 23-May-17 09:50 sklearn/ensemble/iforest/IsolationForest$2.class
--rw-rw-r--  2.0 unx     8150 b- defN 23-May-17 09:50 sklearn/ensemble/iforest/IsolationForest.class
--rw-rw-r--  2.0 unx     4981 b- defN 23-May-17 09:50 sklearn/ensemble/voting/VotingClassifier.class
--rw-rw-r--  2.0 unx     3716 b- defN 23-May-17 09:50 sklearn/ensemble/voting/VotingRegressor.class
--rw-rw-r--  2.0 unx     2814 b- defN 23-May-17 09:50 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingRegressor.class
--rw-rw-r--  2.0 unx     1247 b- defN 23-May-17 09:50 sklearn/ensemble/hist_gradient_boosting/BinMapper$1.class
--rw-rw-r--  2.0 unx     3041 b- defN 23-May-17 09:50 sklearn/ensemble/hist_gradient_boosting/TreePredictor.class
--rw-rw-r--  2.0 unx     6152 b- defN 23-May-17 09:50 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingUtil.class
--rw-rw-r--  2.0 unx      505 b- defN 23-May-17 09:50 sklearn/ensemble/hist_gradient_boosting/CategoricalCrossEntropy.class
--rw-rw-r--  2.0 unx      490 b- defN 23-May-17 09:50 sklearn/ensemble/hist_gradient_boosting/BinaryCrossEntropy.class
--rw-rw-r--  2.0 unx     1572 b- defN 23-May-17 09:50 sklearn/ensemble/hist_gradient_boosting/BinMapper.class
--rw-rw-r--  2.0 unx     6118 b- defN 23-May-17 09:50 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingClassifier.class
--rw-rw-r--  2.0 unx     8868 b- defN 23-May-17 09:50 sklearn/ensemble/hist_gradient_boosting/TreePredictorUtil.class
--rw-rw-r--  2.0 unx      441 b- defN 23-May-17 09:50 sklearn/ensemble/hist_gradient_boosting/BaseLoss.class
--rw-rw-r--  2.0 unx     1418 b- defN 23-May-17 09:50 sklearn/ensemble/EnsembleClassifier.class
--rw-rw-r--  2.0 unx     3564 b- defN 23-May-17 09:50 sklearn/ensemble/weight_boosting/AdaBoostRegressor.class
--rw-rw-r--  2.0 unx     5361 b- defN 23-May-17 09:50 sklearn/Transformer.class
--rw-rw-r--  2.0 unx      859 b- defN 23-May-17 09:50 sklearn/Transformer$1$1.class
--rw-rw-r--  2.0 unx      981 b- defN 23-May-17 09:50 sklearn/Drop.class
--rw-rw-r--  2.0 unx     1772 b- defN 23-May-17 09:50 sklearn/feature_selection/SelectKBest$Entry.class
--rw-rw-r--  2.0 unx     3486 b- defN 23-May-17 09:50 sklearn/feature_selection/SelectFromModel.class
--rw-rw-r--  2.0 unx     2922 b- defN 23-May-17 09:50 sklearn/feature_selection/SelectKBest.class
--rw-rw-r--  2.0 unx     1451 b- defN 23-May-17 09:50 sklearn/feature_selection/PySelector.class
--rw-rw-r--  2.0 unx      607 b- defN 23-May-17 09:50 sklearn/Transformer$2.class
--rw-rw-r--  2.0 unx     2216 b- defN 23-May-17 09:50 sklearn/SkLearnUtil.class
--rw-rw-r--  2.0 unx      412 b- defN 23-May-17 09:50 sklearn/loss/HalfMultinomialLoss.class
--rw-rw-r--  2.0 unx      602 b- defN 23-May-17 09:50 sklearn/loss/CyLossFunction.class
--rw-rw-r--  2.0 unx      403 b- defN 23-May-17 09:50 sklearn/loss/HalfBinomialLoss.class
--rw-rw-r--  2.0 unx      387 b- defN 23-May-17 09:50 sklearn/loss/BaseLoss.class
--rw-rw-r--  2.0 unx      381 b- defN 23-May-17 09:50 sklearn/HasDecisionFunctionField.class
--rw-rw-r--  2.0 unx      338 b- defN 23-May-17 09:50 sklearn/SkLearnMethods.class
--rw-rw-r--  2.0 unx     3091 b- defN 23-May-17 09:50 sklearn/ScalarLabelUtil.class
--rw-rw-r--  2.0 unx      195 b- defN 23-May-17 09:50 sklearn/HasClasses.class
--rw-rw-r--  2.0 unx     4524 b- defN 23-May-17 09:50 sklearn/discriminant_analysis/LinearDiscriminantAnalysis.class
--rw-rw-r--  2.0 unx      696 b- defN 23-May-17 09:50 sklearn/EstimatorUtil$1.class
--rw-rw-r--  2.0 unx     3311 b- defN 23-May-17 09:50 sklearn/Composite.class
--rw-rw-r--  2.0 unx     1194 b- defN 23-May-17 09:50 sklearn/preprocessing/KBinsDiscretizer$1.class
--rw-rw-r--  2.0 unx     4567 b- defN 23-May-17 09:50 sklearn/preprocessing/PowerTransformer.class
--rw-rw-r--  2.0 unx     2381 b- defN 23-May-17 09:50 sklearn/preprocessing/LabelEncoder.class
--rw-rw-r--  2.0 unx     4924 b- defN 23-May-17 09:50 sklearn/preprocessing/LabelBinarizer.class
--rw-rw-r--  2.0 unx      729 b- defN 23-May-17 09:50 sklearn/preprocessing/EncoderUtil$3.class
--rw-rw-r--  2.0 unx      389 b- defN 23-May-17 09:50 sklearn/preprocessing/Scaler.class
--rw-rw-r--  2.0 unx     3242 b- defN 23-May-17 09:50 sklearn/preprocessing/MaxAbsScaler.class
--rw-rw-r--  2.0 unx     2948 b- defN 23-May-17 09:50 sklearn/preprocessing/FunctionTransformer.class
--rw-rw-r--  2.0 unx     3291 b- defN 23-May-17 09:50 sklearn/preprocessing/BaseEncoder.class
--rw-rw-r--  2.0 unx     1270 b- defN 23-May-17 09:50 sklearn/preprocessing/EncoderUtil$1.class
--rw-rw-r--  2.0 unx     4549 b- defN 23-May-17 09:50 sklearn/preprocessing/StandardScaler.class
--rw-rw-r--  2.0 unx     6971 b- defN 23-May-17 09:50 sklearn/preprocessing/EncoderUtil.class
--rw-rw-r--  2.0 unx     6343 b- defN 23-May-17 09:50 sklearn/preprocessing/PolynomialFeatures.class
--rw-rw-r--  2.0 unx     8486 b- defN 23-May-17 09:50 sklearn/preprocessing/KBinsDiscretizer.class
--rw-rw-r--  2.0 unx     4671 b- defN 23-May-17 09:50 sklearn/preprocessing/OneHotEncoder.class
--rw-rw-r--  2.0 unx     2553 b- defN 23-May-17 09:50 sklearn/preprocessing/Binarizer.class
--rw-rw-r--  2.0 unx     1054 b- defN 23-May-17 09:50 sklearn/preprocessing/EncoderUtil$2.class
--rw-rw-r--  2.0 unx     3595 b- defN 23-May-17 09:50 sklearn/preprocessing/MinMaxScaler.class
--rw-rw-r--  2.0 unx     4467 b- defN 23-May-17 09:50 sklearn/preprocessing/RobustScaler.class
--rw-rw-r--  2.0 unx     3740 b- defN 23-May-17 09:50 sklearn/preprocessing/OrdinalEncoder.class
--rw-rw-r--  2.0 unx      957 b- defN 23-May-17 09:50 sklearn/preprocessing/Imputer.class
--rw-rw-r--  2.0 unx     2033 b- defN 23-May-17 09:50 sklearn/preprocessing/PolynomialFeatures$1.class
--rw-rw-r--  2.0 unx     7408 b- defN 23-May-17 09:50 sklearn/preprocessing/MultiOneHotEncoder.class
--rw-rw-r--  2.0 unx     2173 b- defN 23-May-17 09:50 sklearn/tree/TreeClassifier.class
--rw-rw-r--  2.0 unx     3111 b- defN 23-May-17 09:50 sklearn/tree/TreeUtil$1.class
--rw-rw-r--  2.0 unx     2664 b- defN 23-May-17 09:50 sklearn/tree/TreeUtil$4.class
--rw-rw-r--  2.0 unx     4805 b- defN 23-May-17 09:50 sklearn/tree/visitors/TreeModelFlattener.class
--rw-rw-r--  2.0 unx      739 b- defN 23-May-17 09:50 sklearn/tree/visitors/TreeModelCompactor$1.class
--rw-rw-r--  2.0 unx     5431 b- defN 23-May-17 09:50 sklearn/tree/visitors/TreeModelCompactor.class
--rw-rw-r--  2.0 unx     2988 b- defN 23-May-17 09:50 sklearn/tree/visitors/TreeModelPruner.class
--rw-rw-r--  2.0 unx      739 b- defN 23-May-17 09:50 sklearn/tree/visitors/TreeModelFlattener$1.class
--rw-rw-r--  2.0 unx      730 b- defN 23-May-17 09:50 sklearn/tree/visitors/TreeModelPruner$1.class
--rw-rw-r--  2.0 unx     1489 b- defN 23-May-17 09:50 sklearn/tree/TreeUtil$8.class
--rw-rw-r--  2.0 unx      879 b- defN 23-May-17 09:50 sklearn/tree/RegressionCriterion.class
--rw-rw-r--  2.0 unx     1151 b- defN 23-May-17 09:50 sklearn/tree/TreeUtil$5.class
--rw-rw-r--  2.0 unx      978 b- defN 23-May-17 09:50 sklearn/tree/PresortBestSplitter.class
--rw-rw-r--  2.0 unx      977 b- defN 23-May-17 09:50 sklearn/tree/TreeUtil$6.class
--rw-rw-r--  2.0 unx     1764 b- defN 23-May-17 09:50 sklearn/tree/TreeRegressor.class
--rw-rw-r--  2.0 unx     1589 b- defN 23-May-17 09:50 sklearn/tree/TreeUtil$7.class
--rw-rw-r--  2.0 unx    20190 b- defN 23-May-17 09:50 sklearn/tree/TreeUtil.class
--rw-rw-r--  2.0 unx     1123 b- defN 23-May-17 09:50 sklearn/tree/TreeUtil$3.class
--rw-rw-r--  2.0 unx     1373 b- defN 23-May-17 09:50 sklearn/tree/HasTreeOptions.class
--rw-rw-r--  2.0 unx     2257 b- defN 23-May-17 09:50 sklearn/tree/Tree.class
--rw-rw-r--  2.0 unx      754 b- defN 23-May-17 09:50 sklearn/tree/TreeUtil$2.class
--rw-rw-r--  2.0 unx      150 b- defN 23-May-17 09:50 sklearn/tree/HasTree.class
--rw-rw-r--  2.0 unx     1967 b- defN 23-May-17 09:50 sklearn/InitializerUtil.class
--rw-rw-r--  2.0 unx      570 b- defN 23-May-17 09:50 sklearn/Regressor.class
--rw-rw-r--  2.0 unx      211 b- defN 23-May-17 09:50 sklearn/HasNumberOfOutputs.class
--rw-rw-r--  2.0 unx     2366 b- defN 23-May-17 09:50 sklearn/Calibrator.class
--rw-rw-r--  2.0 unx      273 b- defN 23-May-17 09:50 sklearn/HasClassifierOptions.class
--rw-rw-r--  2.0 unx     6878 b- defN 23-May-17 09:50 sklearn/EstimatorUtil.class
--rw-rw-r--  2.0 unx      199 b- defN 23-May-17 09:50 sklearn/HasType.class
--rw-rw-r--  2.0 unx      678 b- defN 23-May-17 09:50 sklearn/cluster/MiniBatchKMeans.class
--rw-rw-r--  2.0 unx     5086 b- defN 23-May-17 09:50 sklearn/cluster/KMeans.class
--rw-rw-r--  2.0 unx     8327 b- defN 23-May-17 09:50 sklearn/Estimator.class
--rw-rw-r--  2.0 unx     1624 b- defN 23-May-17 09:50 sklearn/Initializer.class
--rw-rw-r--  2.0 unx     4598 b- defN 23-May-17 09:50 sklearn/multiclass/OneVsRestClassifier.class
--rw-rw-r--  2.0 unx     5157 b- defN 23-May-17 09:50 sklearn2pmml/ruleset/RuleSetClassifier.class
--rw-rw-r--  2.0 unx     1023 b- defN 23-May-17 09:50 sklearn2pmml/pipeline/PMMLPipeline$3.class
--rw-rw-r--  2.0 unx    28185 b- defN 23-May-17 09:50 sklearn2pmml/pipeline/PMMLPipeline.class
--rw-rw-r--  2.0 unx      980 b- defN 23-May-17 09:50 sklearn2pmml/pipeline/PMMLPipeline$2.class
--rw-rw-r--  2.0 unx     1421 b- defN 23-May-17 09:50 sklearn2pmml/pipeline/PMMLPipeline$1.class
--rw-rw-r--  2.0 unx     1811 b- defN 23-May-17 09:50 sklearn2pmml/pipeline/Verification.class
--rw-rw-r--  2.0 unx     2162 b- defN 23-May-17 09:50 sklearn2pmml/decoration/MultiDomain.class
--rw-rw-r--  2.0 unx     1152 b- defN 23-May-17 09:50 sklearn2pmml/decoration/ContinuousDomainEraser.class
--rw-rw-r--  2.0 unx     1654 b- defN 23-May-17 09:50 sklearn2pmml/decoration/Alias.class
--rw-rw-r--  2.0 unx     1772 b- defN 23-May-17 09:50 sklearn2pmml/decoration/TemporalDomain.class
--rw-rw-r--  2.0 unx      779 b- defN 23-May-17 09:50 sklearn2pmml/decoration/ContinuousDomain$1.class
--rw-rw-r--  2.0 unx    11878 b- defN 23-May-17 09:50 sklearn2pmml/decoration/Domain.class
--rw-rw-r--  2.0 unx     1416 b- defN 23-May-17 09:50 sklearn2pmml/decoration/MultiAlias.class
--rw-rw-r--  2.0 unx     5055 b- defN 23-May-17 09:50 sklearn2pmml/decoration/DiscreteDomain.class
--rw-rw-r--  2.0 unx     1952 b- defN 23-May-17 09:50 sklearn2pmml/decoration/CategoricalDomain.class
--rw-rw-r--  2.0 unx     1453 b- defN 23-May-17 09:50 sklearn2pmml/decoration/DomainEraser.class
--rw-rw-r--  2.0 unx      613 b- defN 23-May-17 09:50 sklearn2pmml/decoration/DateTimeDomain.class
--rw-rw-r--  2.0 unx     7764 b- defN 23-May-17 09:50 sklearn2pmml/decoration/ContinuousDomain.class
--rw-rw-r--  2.0 unx     1083 b- defN 23-May-17 09:50 sklearn2pmml/decoration/DiscreteDomainEraser.class
--rw-rw-r--  2.0 unx     1590 b- defN 23-May-17 09:50 sklearn2pmml/decoration/TransformerWrapper.class
--rw-rw-r--  2.0 unx     1045 b- defN 23-May-17 09:50 sklearn2pmml/decoration/Domain$2.class
--rw-rw-r--  2.0 unx      596 b- defN 23-May-17 09:50 sklearn2pmml/decoration/DateDomain.class
--rw-rw-r--  2.0 unx     3544 b- defN 23-May-17 09:50 sklearn2pmml/decoration/DomainUtil.class
--rw-rw-r--  2.0 unx     1033 b- defN 23-May-17 09:50 sklearn2pmml/decoration/Domain$1.class
--rw-rw-r--  2.0 unx     1577 b- defN 23-May-17 09:50 sklearn2pmml/decoration/OrdinalDomain.class
--rw-rw-r--  2.0 unx      672 b- defN 23-May-17 09:50 sklearn2pmml/decoration/Domain$4.class
--rw-rw-r--  2.0 unx      799 b- defN 23-May-17 09:50 sklearn2pmml/decoration/Domain$3.class
--rw-rw-r--  2.0 unx     7862 b- defN 23-May-17 09:50 sklearn2pmml/neural_network/MLPTransformer.class
--rw-rw-r--  2.0 unx      335 b- defN 23-May-17 09:50 sklearn2pmml/SkLearn2PMMLFields.class
--rw-rw-r--  2.0 unx     1160 b- defN 23-May-17 09:50 sklearn2pmml/util/Evaluatable.class
--rw-rw-r--  2.0 unx     1196 b- defN 23-May-17 09:50 sklearn2pmml/util/Expression.class
--rw-rw-r--  2.0 unx     1189 b- defN 23-May-17 09:50 sklearn2pmml/util/Predicate.class
--rw-rw-r--  2.0 unx     1434 b- defN 23-May-17 09:50 sklearn2pmml/util/Reshaper.class
--rw-rw-r--  2.0 unx     3392 b- defN 23-May-17 09:50 sklearn2pmml/util/EvaluatableUtil.class
--rw-rw-r--  2.0 unx     1658 b- defN 23-May-17 09:50 sklearn2pmml/util/Slicer.class
--rw-rw-r--  2.0 unx     2418 b- defN 23-May-17 09:50 sklearn2pmml/feature_extraction/text/Splitter.class
--rw-rw-r--  2.0 unx     3184 b- defN 23-May-17 09:50 sklearn2pmml/feature_extraction/text/Matcher.class
--rw-rw-r--  2.0 unx     1262 b- defN 23-May-17 09:50 sklearn2pmml/ensemble/SelectFirstRegressor.class
--rw-rw-r--  2.0 unx     2083 b- defN 23-May-17 09:50 sklearn2pmml/ensemble/GBDTUtil$2.class
--rw-rw-r--  2.0 unx     1134 b- defN 23-May-17 09:50 sklearn2pmml/ensemble/EstimatorChain$1.class
--rw-rw-r--  2.0 unx     1934 b- defN 23-May-17 09:50 sklearn2pmml/ensemble/GBDTLMRegressor.class
--rw-rw-r--  2.0 unx      948 b- defN 23-May-17 09:50 sklearn2pmml/ensemble/GBDTUtil$1.class
--rw-rw-r--  2.0 unx     7358 b- defN 23-May-17 09:50 sklearn2pmml/ensemble/EstimatorChain.class
--rw-rw-r--  2.0 unx     6578 b- defN 23-May-17 09:50 sklearn2pmml/ensemble/GBDTUtil.class
--rw-rw-r--  2.0 unx     3995 b- defN 23-May-17 09:50 sklearn2pmml/ensemble/Link.class
--rw-rw-r--  2.0 unx     4360 b- defN 23-May-17 09:50 sklearn2pmml/ensemble/SelectFirstUtil.class
--rw-rw-r--  2.0 unx     3773 b- defN 23-May-17 09:50 sklearn2pmml/ensemble/GBDTLRClassifier.class
--rw-rw-r--  2.0 unx     2608 b- defN 23-May-17 09:50 sklearn2pmml/ensemble/SelectFirstClassifier.class
--rw-rw-r--  2.0 unx     1438 b- defN 23-May-17 09:50 sklearn2pmml/EstimatorProxy$1.class
--rw-rw-r--  2.0 unx      946 b- defN 23-May-17 09:50 sklearn2pmml/feature_selection/SelectUnique.class
--rw-rw-r--  2.0 unx     6477 b- defN 23-May-17 09:50 sklearn2pmml/postprocessing/BusinessDecisionTransformer.class
--rw-rw-r--  2.0 unx      791 b- defN 23-May-17 09:50 sklearn2pmml/postprocessing/BusinessDecisionTransformer$1.class
--rw-rw-r--  2.0 unx     1197 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/PatternTransformer.class
--rw-rw-r--  2.0 unx     2908 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/ReplaceTransformer.class
--rw-rw-r--  2.0 unx     1844 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/WordCountTransformer.class
--rw-rw-r--  2.0 unx      597 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/DateTimeFormatter.class
--rw-rw-r--  2.0 unx     1288 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/PMMLLabelBinarizer.class
--rw-rw-r--  2.0 unx     4621 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/DurationTransformer.class
--rw-rw-r--  2.0 unx      444 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/PMMLLabelEncoder.class
--rw-rw-r--  2.0 unx     2777 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/FilterLookupTransformer.class
--rw-rw-r--  2.0 unx     2545 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/Formatter.class
--rw-rw-r--  2.0 unx     3341 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/CastTransformer.class
--rw-rw-r--  2.0 unx     2758 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/MatchesTransformer.class
--rw-rw-r--  2.0 unx      589 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/NumberFormatter.class
--rw-rw-r--  2.0 unx     4149 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/MultiLookupTransformer.class
--rw-rw-r--  2.0 unx     3871 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/StringNormalizer.class
--rw-rw-r--  2.0 unx     7145 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/ExpressionTransformer.class
--rw-rw-r--  2.0 unx      635 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/DaysSinceYearTransformer.class
--rw-rw-r--  2.0 unx     3604 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/DataFrameConstructor.class
--rw-rw-r--  2.0 unx     2847 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/ConcatTransformer.class
--rw-rw-r--  2.0 unx     5993 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/CutTransformer.class
--rw-rw-r--  2.0 unx     7025 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/BSplineTransformer.class
--rw-rw-r--  2.0 unx     6410 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/LookupTransformer.class
--rw-rw-r--  2.0 unx     3236 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/SubstringTransformer.class
--rw-rw-r--  2.0 unx     3181 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/SecondsSinceMidnightTransformer.class
--rw-rw-r--  2.0 unx     2132 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/PowerFunctionTransformer.class
--rw-rw-r--  2.0 unx     3328 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/Aggregator.class
--rw-rw-r--  2.0 unx      647 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/SecondsSinceYearTransformer.class
--rw-rw-r--  2.0 unx     1082 b- defN 23-May-17 09:50 sklearn2pmml/tree/CHAIDRegressor.class
--rw-rw-r--  2.0 unx    11309 b- defN 23-May-17 09:50 sklearn2pmml/tree/CHAIDUtil.class
--rw-rw-r--  2.0 unx     2019 b- defN 23-May-17 09:50 sklearn2pmml/tree/CHAIDClassifier.class
--rw-rw-r--  2.0 unx     1417 b- defN 23-May-17 09:50 sklearn2pmml/tree/CHAIDUtil$1.class
--rw-rw-r--  2.0 unx     3864 b- defN 23-May-17 09:50 sklearn2pmml/EstimatorProxy.class
--rw-rw-r--  2.0 unx     1458 b- defN 23-May-17 09:50 sklearn2pmml/SelectorProxy.class
--rw-rw-r--  2.0 unx     2046 b- defN 23-May-17 09:50 sklearn2pmml/expression/ExpressionUtil.class
--rw-rw-r--  2.0 unx     3799 b- defN 23-May-17 09:50 sklearn2pmml/expression/ExpressionRegressor.class
--rw-rw-r--  2.0 unx      990 b- defN 23-May-17 09:50 sklearn2pmml/expression/ExpressionClassifier$1.class
--rw-rw-r--  2.0 unx     8759 b- defN 23-May-17 09:50 sklearn2pmml/expression/ExpressionClassifier.class
--rw-rw-r--  2.0 unx      948 b- defN 23-May-17 09:50 sklearn2pmml/expression/ExpressionUtil$1.class
--rw-rw-r--  2.0 unx     1774 b- defN 23-May-17 09:50 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest$1.class
--rw-rw-r--  2.0 unx     2764 b- defN 23-May-17 09:50 org/jpmml/sklearn/testing/SkLearnEncoderBatch.class
--rw-rw-r--  2.0 unx     3549 b- defN 23-May-17 09:50 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest.class
--rw-rw-r--  2.0 unx    13598 b- defN 23-May-17 09:50 org/jpmml/sklearn/SkLearnEncoder.class
--rw-rw-r--  2.0 unx      194 b- defN 23-May-17 09:50 org/jpmml/sklearn/FieldNames.class
--rw-rw-r--  2.0 unx      171 b- defN 23-May-17 09:50 org/jpmml/sklearn/HasSkLearnOptions.class
--rw-rw-r--  2.0 unx     1030 b- defN 23-May-17 09:50 org/jpmml/sklearn/SkLearnEncoder$1.class
--rw-rw-r--  2.0 unx     1822 b- defN 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn/pom.xml
--rw-rw-r--  2.0 unx       57 b- defN 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn/pom.properties
-403 files, 916820 bytes uncompressed, 404783 bytes compressed:  55.8%
+Zip file size: 467741 bytes, number of entries: 403
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-06 10:35 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn_pandas/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 chaid/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 stop_words/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/calibration/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/pipeline/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/dummy/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/svm/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/neural_network/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/impute/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/naive_bayes/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/linear_model/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/linear_model/logistic/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/linear_model/ridge/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/linear_model/glm/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/linear_model/stochastic_gradient/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/compose/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/model_selection/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/decomposition/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/neighbors/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/multioutput/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/isotonic/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/feature_extraction/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/feature_extraction/text/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/metrics/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/ensemble/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/ensemble/bagging/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/ensemble/stacking/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/ensemble/forest/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/ensemble/iforest/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/ensemble/voting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/ensemble/hist_gradient_boosting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/ensemble/weight_boosting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/feature_selection/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/loss/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/discriminant_analysis/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/preprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/tree/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/tree/visitors/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/cluster/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/multiclass/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/ruleset/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/pipeline/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/decoration/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/neural_network/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/util/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/feature_extraction/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/feature_extraction/text/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/ensemble/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/feature_selection/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/postprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/preprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/tree/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/expression/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 org/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 org/jpmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 org/jpmml/sklearn/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 org/jpmml/sklearn/testing/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/org.jpmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn/
+-rw-rw-r--  2.0 unx    16829 b- defN 23-Jun-06 10:35 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx     2287 b- defN 23-Jun-06 10:35 sklearn_pandas/CategoricalImputer.class
+-rw-rw-r--  2.0 unx      656 b- defN 23-Jun-06 10:35 sklearn_pandas/TransformerPipeline.class
+-rw-rw-r--  2.0 unx     1154 b- defN 23-Jun-06 10:35 sklearn_pandas/DataFrameMapper$2.class
+-rw-rw-r--  2.0 unx     6280 b- defN 23-Jun-06 10:35 sklearn_pandas/DataFrameMapper.class
+-rw-rw-r--  2.0 unx     1126 b- defN 23-Jun-06 10:35 sklearn_pandas/DataFrameMapper$1.class
+-rw-rw-r--  2.0 unx      609 b- defN 23-Jun-06 10:35 chaid/ContinuousColumn.class
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jun-06 10:35 chaid/Node.class
+-rw-rw-r--  2.0 unx      467 b- defN 23-Jun-06 10:35 chaid/Column.class
+-rw-rw-r--  2.0 unx     3283 b- defN 23-Jun-06 10:35 chaid/Split.class
+-rw-rw-r--  2.0 unx      401 b- defN 23-Jun-06 10:35 chaid/InvalidSplitReason.class
+-rw-rw-r--  2.0 unx      602 b- defN 23-Jun-06 10:35 chaid/NominalColumn.class
+-rw-rw-r--  2.0 unx     1912 b- defN 23-Jun-06 10:35 stop_words/english.txt
+-rw-rw-r--  2.0 unx      147 b- defN 23-Jun-06 10:35 sklearn/HasHead.class
+-rw-rw-r--  2.0 unx     1728 b- defN 23-Jun-06 10:35 sklearn/StepUtil.class
+-rw-rw-r--  2.0 unx    11453 b- defN 23-Jun-06 10:35 sklearn/calibration/CalibratedClassifier.class
+-rw-rw-r--  2.0 unx     2972 b- defN 23-Jun-06 10:35 sklearn/calibration/SigmoidCalibration.class
+-rw-rw-r--  2.0 unx      683 b- defN 23-Jun-06 10:35 sklearn/calibration/CalibratedClassifier$1.class
+-rw-rw-r--  2.0 unx     1475 b- defN 23-Jun-06 10:35 sklearn/calibration/CalibratedClassifierCV.class
+-rw-rw-r--  2.0 unx     1862 b- defN 23-Jun-06 10:35 sklearn/pipeline/PipelineTransformer.class
+-rw-rw-r--  2.0 unx     1671 b- defN 23-Jun-06 10:35 sklearn/pipeline/Pipeline$2.class
+-rw-rw-r--  2.0 unx     2536 b- defN 23-Jun-06 10:35 sklearn/pipeline/FeatureUnion.class
+-rw-rw-r--  2.0 unx     5062 b- defN 23-Jun-06 10:35 sklearn/pipeline/Pipeline.class
+-rw-rw-r--  2.0 unx     2003 b- defN 23-Jun-06 10:35 sklearn/pipeline/PipelineRegressor.class
+-rw-rw-r--  2.0 unx     1773 b- defN 23-Jun-06 10:35 sklearn/pipeline/Pipeline$1.class
+-rw-rw-r--  2.0 unx     1111 b- defN 23-Jun-06 10:35 sklearn/pipeline/PipelineUtil.class
+-rw-rw-r--  2.0 unx     2298 b- defN 23-Jun-06 10:35 sklearn/pipeline/PipelineClassifier.class
+-rw-rw-r--  2.0 unx     4913 b- defN 23-Jun-06 10:35 sklearn/dummy/DummyClassifier.class
+-rw-rw-r--  2.0 unx     2055 b- defN 23-Jun-06 10:35 sklearn/dummy/DummyRegressor.class
+-rw-rw-r--  2.0 unx      454 b- defN 23-Jun-06 10:35 sklearn/SkLearnFields.class
+-rw-rw-r--  2.0 unx     2293 b- defN 23-Jun-06 10:35 sklearn/SkLearnOutlierTransformation.class
+-rw-rw-r--  2.0 unx      240 b- defN 23-Jun-06 10:35 sklearn/HasEstimator.class
+-rw-rw-r--  2.0 unx     3456 b- defN 23-Jun-06 10:35 sklearn/OutlierDetectorUtil.class
+-rw-rw-r--  2.0 unx     1258 b- defN 23-Jun-06 10:35 sklearn/HasMultiApplyField.class
+-rw-rw-r--  2.0 unx      908 b- defN 23-Jun-06 10:35 sklearn/None.class
+-rw-rw-r--  2.0 unx     2393 b- defN 23-Jun-06 10:35 sklearn/svm/SupportVectorMachineUtil.class
+-rw-rw-r--  2.0 unx     1109 b- defN 23-Jun-06 10:35 sklearn/svm/LinearSVC.class
+-rw-rw-r--  2.0 unx     5037 b- defN 23-Jun-06 10:35 sklearn/svm/LibSVMClassifier.class
+-rw-rw-r--  2.0 unx      966 b- defN 23-Jun-06 10:35 sklearn/svm/SupportVectorMachineUtil$1.class
+-rw-rw-r--  2.0 unx     1305 b- defN 23-Jun-06 10:35 sklearn/svm/OneClassSVM.class
+-rw-rw-r--  2.0 unx     3594 b- defN 23-Jun-06 10:35 sklearn/svm/LibSVMRegressor.class
+-rw-rw-r--  2.0 unx     4114 b- defN 23-Jun-06 10:35 sklearn/InitializerUtil$1.class
+-rw-rw-r--  2.0 unx      735 b- defN 23-Jun-06 10:35 sklearn/Estimator$1.class
+-rw-rw-r--  2.0 unx      214 b- defN 23-Jun-06 10:35 sklearn/HasNumberOfFeatures.class
+-rw-rw-r--  2.0 unx      660 b- defN 23-Jun-06 10:35 sklearn/MultiTransformer.class
+-rw-rw-r--  2.0 unx     2110 b- defN 23-Jun-06 10:35 sklearn/neural_network/MLPRegressor.class
+-rw-rw-r--  2.0 unx     2555 b- defN 23-Jun-06 10:35 sklearn/neural_network/MLPClassifier.class
+-rw-rw-r--  2.0 unx      759 b- defN 23-Jun-06 10:35 sklearn/neural_network/MultilayerPerceptronUtil$1.class
+-rw-rw-r--  2.0 unx    11996 b- defN 23-Jun-06 10:35 sklearn/neural_network/MultilayerPerceptronUtil.class
+-rw-rw-r--  2.0 unx     1880 b- defN 23-Jun-06 10:35 sklearn/Step.class
+-rw-rw-r--  2.0 unx      168 b- defN 23-Jun-06 10:35 sklearn/HasDefaultValue.class
+-rw-rw-r--  2.0 unx     2936 b- defN 23-Jun-06 10:35 sklearn/impute/MissingIndicator.class
+-rw-rw-r--  2.0 unx     4027 b- defN 23-Jun-06 10:35 sklearn/impute/ImputerUtil.class
+-rw-rw-r--  2.0 unx     5703 b- defN 23-Jun-06 10:35 sklearn/impute/SimpleImputer.class
+-rw-rw-r--  2.0 unx     6948 b- defN 23-Jun-06 10:35 sklearn/naive_bayes/GaussianNB.class
+-rw-rw-r--  2.0 unx     4398 b- defN 23-Jun-06 10:35 sklearn/linear_model/LinearRegressor.class
+-rw-rw-r--  2.0 unx     5040 b- defN 23-Jun-06 10:35 sklearn/linear_model/LinearClassifier.class
+-rw-rw-r--  2.0 unx     7648 b- defN 23-Jun-06 10:35 sklearn/linear_model/logistic/LogisticRegression.class
+-rw-rw-r--  2.0 unx     1042 b- defN 23-Jun-06 10:35 sklearn/linear_model/ridge/RidgeClassifier.class
+-rw-rw-r--  2.0 unx      596 b- defN 23-Jun-06 10:35 sklearn/linear_model/glm/DistributionBoundary.class
+-rw-rw-r--  2.0 unx     1601 b- defN 23-Jun-06 10:35 sklearn/linear_model/glm/GeneralizedLinearRegressor.class
+-rw-rw-r--  2.0 unx      911 b- defN 23-Jun-06 10:35 sklearn/linear_model/stochastic_gradient/Hinge.class
+-rw-rw-r--  2.0 unx     2480 b- defN 23-Jun-06 10:35 sklearn/linear_model/stochastic_gradient/SGDOneClassSVM.class
+-rw-rw-r--  2.0 unx      461 b- defN 23-Jun-06 10:35 sklearn/linear_model/stochastic_gradient/LossFunction.class
+-rw-rw-r--  2.0 unx      452 b- defN 23-Jun-06 10:35 sklearn/linear_model/stochastic_gradient/Log.class
+-rw-rw-r--  2.0 unx     1165 b- defN 23-Jun-06 10:35 sklearn/linear_model/stochastic_gradient/SGDClassifier.class
+-rw-rw-r--  2.0 unx      482 b- defN 23-Jun-06 10:35 sklearn/linear_model/stochastic_gradient/ModifiedHuber.class
+-rw-rw-r--  2.0 unx      932 b- defN 23-Jun-06 10:35 sklearn/linear_model/stochastic_gradient/SquaredHinge.class
+-rw-rw-r--  2.0 unx     1720 b- defN 23-Jun-06 10:35 sklearn/compose/ColumnTransformer$1.class
+-rw-rw-r--  2.0 unx     3239 b- defN 23-Jun-06 10:35 sklearn/compose/TransformedTargetRegressor.class
+-rw-rw-r--  2.0 unx     3649 b- defN 23-Jun-06 10:35 sklearn/compose/ColumnTransformer.class
+-rw-rw-r--  2.0 unx     1534 b- defN 23-Jun-06 10:35 sklearn/compose/TransformedTargetRegressor$1.class
+-rw-rw-r--  2.0 unx     4089 b- defN 23-Jun-06 10:35 sklearn/Classifier.class
+-rw-rw-r--  2.0 unx     1457 b- defN 23-Jun-06 10:35 sklearn/model_selection/EstimatorSearcher.class
+-rw-rw-r--  2.0 unx     1685 b- defN 23-Jun-06 10:35 sklearn/Selector.class
+-rw-rw-r--  2.0 unx      419 b- defN 23-Jun-06 10:35 sklearn/decomposition/IncrementalPCA.class
+-rw-rw-r--  2.0 unx     3471 b- defN 23-Jun-06 10:35 sklearn/decomposition/TruncatedSVD.class
+-rw-rw-r--  2.0 unx     4759 b- defN 23-Jun-06 10:35 sklearn/decomposition/PCA.class
+-rw-rw-r--  2.0 unx      911 b- defN 23-Jun-06 10:35 sklearn/decomposition/BasePCA.class
+-rw-rw-r--  2.0 unx      336 b- defN 23-Jun-06 10:35 sklearn/HasPredictField.class
+-rw-rw-r--  2.0 unx     3018 b- defN 23-Jun-06 10:35 sklearn/neighbors/NearestNeighbors.class
+-rw-rw-r--  2.0 unx     4505 b- defN 23-Jun-06 10:35 sklearn/neighbors/KNeighborsClassifier.class
+-rw-rw-r--  2.0 unx     3794 b- defN 23-Jun-06 10:35 sklearn/neighbors/NearestCentroid.class
+-rw-rw-r--  2.0 unx     2025 b- defN 23-Jun-06 10:35 sklearn/neighbors/BinaryTree.class
+-rw-rw-r--  2.0 unx     1266 b- defN 23-Jun-06 10:35 sklearn/neighbors/KNeighborsUtil$1.class
+-rw-rw-r--  2.0 unx      181 b- defN 23-Jun-06 10:35 sklearn/neighbors/HasMetric.class
+-rw-rw-r--  2.0 unx    10748 b- defN 23-Jun-06 10:35 sklearn/neighbors/KNeighborsUtil.class
+-rw-rw-r--  2.0 unx     4387 b- defN 23-Jun-06 10:35 sklearn/neighbors/KNeighborsRegressor.class
+-rw-rw-r--  2.0 unx     1032 b- defN 23-Jun-06 10:35 sklearn/neighbors/DistanceMetric.class
+-rw-rw-r--  2.0 unx      351 b- defN 23-Jun-06 10:35 sklearn/neighbors/HasTrainingData.class
+-rw-rw-r--  2.0 unx      176 b- defN 23-Jun-06 10:35 sklearn/neighbors/HasNumberOfNeighbors.class
+-rw-rw-r--  2.0 unx     2235 b- defN 23-Jun-06 10:35 sklearn/multioutput/MultiOutputUtil.class
+-rw-rw-r--  2.0 unx     3383 b- defN 23-Jun-06 10:35 sklearn/multioutput/ChainUtil.class
+-rw-rw-r--  2.0 unx     1601 b- defN 23-Jun-06 10:35 sklearn/multioutput/RegressorChain.class
+-rw-rw-r--  2.0 unx     1316 b- defN 23-Jun-06 10:35 sklearn/multioutput/MultiOutputClassifier.class
+-rw-rw-r--  2.0 unx     1310 b- defN 23-Jun-06 10:35 sklearn/multioutput/MultiOutputRegressor.class
+-rw-rw-r--  2.0 unx     1745 b- defN 23-Jun-06 10:35 sklearn/multioutput/ClassifierChain.class
+-rw-rw-r--  2.0 unx     4469 b- defN 23-Jun-06 10:35 sklearn/isotonic/IsotonicRegression.class
+-rw-rw-r--  2.0 unx      326 b- defN 23-Jun-06 10:35 sklearn/HasApplyField.class
+-rw-rw-r--  2.0 unx      273 b- defN 23-Jun-06 10:35 sklearn/HasEstimatorEnsemble.class
+-rw-rw-r--  2.0 unx     1929 b- defN 23-Jun-06 10:35 sklearn/Transformer$1.class
+-rw-rw-r--  2.0 unx      953 b- defN 23-Jun-06 10:35 sklearn/LabelEncoderClassifier.class
+-rw-rw-r--  2.0 unx      937 b- defN 23-Jun-06 10:35 sklearn/PassThrough.class
+-rw-rw-r--  2.0 unx      181 b- defN 23-Jun-06 10:35 sklearn/HasPriorProbability.class
+-rw-rw-r--  2.0 unx     5693 b- defN 23-Jun-06 10:35 sklearn/feature_extraction/text/TfidfVectorizer.class
+-rw-rw-r--  2.0 unx      809 b- defN 23-Jun-06 10:35 sklearn/feature_extraction/text/TfidfVectorizer$1.class
+-rw-rw-r--  2.0 unx      675 b- defN 23-Jun-06 10:35 sklearn/feature_extraction/text/Tokenizer.class
+-rw-rw-r--  2.0 unx    13329 b- defN 23-Jun-06 10:35 sklearn/feature_extraction/text/CountVectorizer.class
+-rw-rw-r--  2.0 unx     2129 b- defN 23-Jun-06 10:35 sklearn/feature_extraction/text/CountVectorizer$1.class
+-rw-rw-r--  2.0 unx     1433 b- defN 23-Jun-06 10:35 sklearn/feature_extraction/text/TfidfTransformer.class
+-rw-rw-r--  2.0 unx     4031 b- defN 23-Jun-06 10:35 sklearn/feature_extraction/DictVectorizer.class
+-rw-rw-r--  2.0 unx      762 b- defN 23-Jun-06 10:35 sklearn/Clusterer.class
+-rw-rw-r--  2.0 unx     1375 b- defN 23-Jun-06 10:35 sklearn/metrics/DistanceMetric.class
+-rw-rw-r--  2.0 unx     1069 b- defN 23-Jun-06 10:35 sklearn/ensemble/EnsembleUtil.class
+-rw-rw-r--  2.0 unx     2112 b- defN 23-Jun-06 10:35 sklearn/ensemble/bagging/BaggingRegressor.class
+-rw-rw-r--  2.0 unx     3293 b- defN 23-Jun-06 10:35 sklearn/ensemble/bagging/BaggingUtil.class
+-rw-rw-r--  2.0 unx     3031 b- defN 23-Jun-06 10:35 sklearn/ensemble/bagging/BaggingClassifier.class
+-rw-rw-r--  2.0 unx     1409 b- defN 23-Jun-06 10:35 sklearn/ensemble/EnsembleRegressor.class
+-rw-rw-r--  2.0 unx     3485 b- defN 23-Jun-06 10:35 sklearn/ensemble/stacking/StackingClassifier.class
+-rw-rw-r--  2.0 unx      495 b- defN 23-Jun-06 10:35 sklearn/ensemble/stacking/StackingUtil$PredictFunction.class
+-rw-rw-r--  2.0 unx     3109 b- defN 23-Jun-06 10:35 sklearn/ensemble/stacking/StackingRegressor.class
+-rw-rw-r--  2.0 unx     3960 b- defN 23-Jun-06 10:35 sklearn/ensemble/stacking/StackingUtil.class
+-rw-rw-r--  2.0 unx     2524 b- defN 23-Jun-06 10:35 sklearn/ensemble/stacking/StackingClassifier$1.class
+-rw-rw-r--  2.0 unx     2254 b- defN 23-Jun-06 10:35 sklearn/ensemble/stacking/StackingRegressor$1.class
+-rw-rw-r--  2.0 unx      495 b- defN 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/ScaledLogOddsEstimator.class
+-rw-rw-r--  2.0 unx     1440 b- defN 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$GradientBoostingClassifierProxy.class
+-rw-rw-r--  2.0 unx     1862 b- defN 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/MultinomialDeviance.class
+-rw-rw-r--  2.0 unx     2563 b- defN 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/GradientBoostingRegressor.class
+-rw-rw-r--  2.0 unx      858 b- defN 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/LossFunction.class
+-rw-rw-r--  2.0 unx     1588 b- defN 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/ExponentialLoss.class
+-rw-rw-r--  2.0 unx     1317 b- defN 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/PriorProbabilityEstimator.class
+-rw-rw-r--  2.0 unx     7948 b- defN 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier.class
+-rw-rw-r--  2.0 unx     1288 b- defN 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/LogOddsEstimator.class
+-rw-rw-r--  2.0 unx      960 b- defN 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/MeanEstimator.class
+-rw-rw-r--  2.0 unx     1265 b- defN 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$1.class
+-rw-rw-r--  2.0 unx      980 b- defN 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/QuantileEstimator.class
+-rw-rw-r--  2.0 unx     1578 b- defN 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/BinomialDeviance.class
+-rw-rw-r--  2.0 unx      811 b- defN 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/ZeroEstimator.class
+-rw-rw-r--  2.0 unx     3003 b- defN 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/GradientBoostingUtil.class
+-rw-rw-r--  2.0 unx     1148 b- defN 23-Jun-06 10:35 sklearn/ensemble/EnsembleUtil$1.class
+-rw-rw-r--  2.0 unx     3059 b- defN 23-Jun-06 10:35 sklearn/ensemble/forest/ForestUtil.class
+-rw-rw-r--  2.0 unx     2311 b- defN 23-Jun-06 10:35 sklearn/ensemble/forest/ForestRegressor.class
+-rw-rw-r--  2.0 unx     2770 b- defN 23-Jun-06 10:35 sklearn/ensemble/forest/ForestClassifier.class
+-rw-rw-r--  2.0 unx     1752 b- defN 23-Jun-06 10:35 sklearn/ensemble/iforest/IsolationForest$3.class
+-rw-rw-r--  2.0 unx     2206 b- defN 23-Jun-06 10:35 sklearn/ensemble/iforest/IsolationForest$1.class
+-rw-rw-r--  2.0 unx     1716 b- defN 23-Jun-06 10:35 sklearn/ensemble/iforest/IsolationForest$2.class
+-rw-rw-r--  2.0 unx     8265 b- defN 23-Jun-06 10:35 sklearn/ensemble/iforest/IsolationForest.class
+-rw-rw-r--  2.0 unx     5055 b- defN 23-Jun-06 10:35 sklearn/ensemble/voting/VotingClassifier.class
+-rw-rw-r--  2.0 unx     3716 b- defN 23-Jun-06 10:35 sklearn/ensemble/voting/VotingRegressor.class
+-rw-rw-r--  2.0 unx     2814 b- defN 23-Jun-06 10:35 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingRegressor.class
+-rw-rw-r--  2.0 unx     1247 b- defN 23-Jun-06 10:35 sklearn/ensemble/hist_gradient_boosting/BinMapper$1.class
+-rw-rw-r--  2.0 unx     3041 b- defN 23-Jun-06 10:35 sklearn/ensemble/hist_gradient_boosting/TreePredictor.class
+-rw-rw-r--  2.0 unx     6152 b- defN 23-Jun-06 10:35 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingUtil.class
+-rw-rw-r--  2.0 unx      505 b- defN 23-Jun-06 10:35 sklearn/ensemble/hist_gradient_boosting/CategoricalCrossEntropy.class
+-rw-rw-r--  2.0 unx      490 b- defN 23-Jun-06 10:35 sklearn/ensemble/hist_gradient_boosting/BinaryCrossEntropy.class
+-rw-rw-r--  2.0 unx     1572 b- defN 23-Jun-06 10:35 sklearn/ensemble/hist_gradient_boosting/BinMapper.class
+-rw-rw-r--  2.0 unx     6377 b- defN 23-Jun-06 10:35 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingClassifier.class
+-rw-rw-r--  2.0 unx     8868 b- defN 23-Jun-06 10:35 sklearn/ensemble/hist_gradient_boosting/TreePredictorUtil.class
+-rw-rw-r--  2.0 unx      441 b- defN 23-Jun-06 10:35 sklearn/ensemble/hist_gradient_boosting/BaseLoss.class
+-rw-rw-r--  2.0 unx     1418 b- defN 23-Jun-06 10:35 sklearn/ensemble/EnsembleClassifier.class
+-rw-rw-r--  2.0 unx     3564 b- defN 23-Jun-06 10:35 sklearn/ensemble/weight_boosting/AdaBoostRegressor.class
+-rw-rw-r--  2.0 unx     5361 b- defN 23-Jun-06 10:35 sklearn/Transformer.class
+-rw-rw-r--  2.0 unx      859 b- defN 23-Jun-06 10:35 sklearn/Transformer$1$1.class
+-rw-rw-r--  2.0 unx      981 b- defN 23-Jun-06 10:35 sklearn/Drop.class
+-rw-rw-r--  2.0 unx     1772 b- defN 23-Jun-06 10:35 sklearn/feature_selection/SelectKBest$Entry.class
+-rw-rw-r--  2.0 unx     3486 b- defN 23-Jun-06 10:35 sklearn/feature_selection/SelectFromModel.class
+-rw-rw-r--  2.0 unx     2922 b- defN 23-Jun-06 10:35 sklearn/feature_selection/SelectKBest.class
+-rw-rw-r--  2.0 unx     1451 b- defN 23-Jun-06 10:35 sklearn/feature_selection/PySelector.class
+-rw-rw-r--  2.0 unx      607 b- defN 23-Jun-06 10:35 sklearn/Transformer$2.class
+-rw-rw-r--  2.0 unx     2216 b- defN 23-Jun-06 10:35 sklearn/SkLearnUtil.class
+-rw-rw-r--  2.0 unx      412 b- defN 23-Jun-06 10:35 sklearn/loss/HalfMultinomialLoss.class
+-rw-rw-r--  2.0 unx      602 b- defN 23-Jun-06 10:35 sklearn/loss/CyLossFunction.class
+-rw-rw-r--  2.0 unx      403 b- defN 23-Jun-06 10:35 sklearn/loss/HalfBinomialLoss.class
+-rw-rw-r--  2.0 unx      387 b- defN 23-Jun-06 10:35 sklearn/loss/BaseLoss.class
+-rw-rw-r--  2.0 unx      381 b- defN 23-Jun-06 10:35 sklearn/HasDecisionFunctionField.class
+-rw-rw-r--  2.0 unx      338 b- defN 23-Jun-06 10:35 sklearn/SkLearnMethods.class
+-rw-rw-r--  2.0 unx     3091 b- defN 23-Jun-06 10:35 sklearn/ScalarLabelUtil.class
+-rw-rw-r--  2.0 unx     1582 b- defN 23-Jun-06 10:35 sklearn/OutlierDetectorUtil$1.class
+-rw-rw-r--  2.0 unx      195 b- defN 23-Jun-06 10:35 sklearn/HasClasses.class
+-rw-rw-r--  2.0 unx     4685 b- defN 23-Jun-06 10:35 sklearn/discriminant_analysis/LinearDiscriminantAnalysis.class
+-rw-rw-r--  2.0 unx      696 b- defN 23-Jun-06 10:35 sklearn/EstimatorUtil$1.class
+-rw-rw-r--  2.0 unx     3311 b- defN 23-Jun-06 10:35 sklearn/Composite.class
+-rw-rw-r--  2.0 unx     1194 b- defN 23-Jun-06 10:35 sklearn/preprocessing/KBinsDiscretizer$1.class
+-rw-rw-r--  2.0 unx     4567 b- defN 23-Jun-06 10:35 sklearn/preprocessing/PowerTransformer.class
+-rw-rw-r--  2.0 unx     2381 b- defN 23-Jun-06 10:35 sklearn/preprocessing/LabelEncoder.class
+-rw-rw-r--  2.0 unx     4924 b- defN 23-Jun-06 10:35 sklearn/preprocessing/LabelBinarizer.class
+-rw-rw-r--  2.0 unx      729 b- defN 23-Jun-06 10:35 sklearn/preprocessing/EncoderUtil$3.class
+-rw-rw-r--  2.0 unx      389 b- defN 23-Jun-06 10:35 sklearn/preprocessing/Scaler.class
+-rw-rw-r--  2.0 unx     3242 b- defN 23-Jun-06 10:35 sklearn/preprocessing/MaxAbsScaler.class
+-rw-rw-r--  2.0 unx     2948 b- defN 23-Jun-06 10:35 sklearn/preprocessing/FunctionTransformer.class
+-rw-rw-r--  2.0 unx     3291 b- defN 23-Jun-06 10:35 sklearn/preprocessing/BaseEncoder.class
+-rw-rw-r--  2.0 unx     1270 b- defN 23-Jun-06 10:35 sklearn/preprocessing/EncoderUtil$1.class
+-rw-rw-r--  2.0 unx     4549 b- defN 23-Jun-06 10:35 sklearn/preprocessing/StandardScaler.class
+-rw-rw-r--  2.0 unx     6971 b- defN 23-Jun-06 10:35 sklearn/preprocessing/EncoderUtil.class
+-rw-rw-r--  2.0 unx     6343 b- defN 23-Jun-06 10:35 sklearn/preprocessing/PolynomialFeatures.class
+-rw-rw-r--  2.0 unx     8486 b- defN 23-Jun-06 10:35 sklearn/preprocessing/KBinsDiscretizer.class
+-rw-rw-r--  2.0 unx     4671 b- defN 23-Jun-06 10:35 sklearn/preprocessing/OneHotEncoder.class
+-rw-rw-r--  2.0 unx     2553 b- defN 23-Jun-06 10:35 sklearn/preprocessing/Binarizer.class
+-rw-rw-r--  2.0 unx     1054 b- defN 23-Jun-06 10:35 sklearn/preprocessing/EncoderUtil$2.class
+-rw-rw-r--  2.0 unx     3595 b- defN 23-Jun-06 10:35 sklearn/preprocessing/MinMaxScaler.class
+-rw-rw-r--  2.0 unx     4467 b- defN 23-Jun-06 10:35 sklearn/preprocessing/RobustScaler.class
+-rw-rw-r--  2.0 unx     3740 b- defN 23-Jun-06 10:35 sklearn/preprocessing/OrdinalEncoder.class
+-rw-rw-r--  2.0 unx      957 b- defN 23-Jun-06 10:35 sklearn/preprocessing/Imputer.class
+-rw-rw-r--  2.0 unx     2033 b- defN 23-Jun-06 10:35 sklearn/preprocessing/PolynomialFeatures$1.class
+-rw-rw-r--  2.0 unx     7408 b- defN 23-Jun-06 10:35 sklearn/preprocessing/MultiOneHotEncoder.class
+-rw-rw-r--  2.0 unx     2153 b- defN 23-Jun-06 10:35 sklearn/tree/TreeClassifier.class
+-rw-rw-r--  2.0 unx     3111 b- defN 23-Jun-06 10:35 sklearn/tree/TreeUtil$1.class
+-rw-rw-r--  2.0 unx     2664 b- defN 23-Jun-06 10:35 sklearn/tree/TreeUtil$4.class
+-rw-rw-r--  2.0 unx     4805 b- defN 23-Jun-06 10:35 sklearn/tree/visitors/TreeModelFlattener.class
+-rw-rw-r--  2.0 unx      739 b- defN 23-Jun-06 10:35 sklearn/tree/visitors/TreeModelCompactor$1.class
+-rw-rw-r--  2.0 unx     5431 b- defN 23-Jun-06 10:35 sklearn/tree/visitors/TreeModelCompactor.class
+-rw-rw-r--  2.0 unx     2988 b- defN 23-Jun-06 10:35 sklearn/tree/visitors/TreeModelPruner.class
+-rw-rw-r--  2.0 unx      739 b- defN 23-Jun-06 10:35 sklearn/tree/visitors/TreeModelFlattener$1.class
+-rw-rw-r--  2.0 unx      730 b- defN 23-Jun-06 10:35 sklearn/tree/visitors/TreeModelPruner$1.class
+-rw-rw-r--  2.0 unx     1489 b- defN 23-Jun-06 10:35 sklearn/tree/TreeUtil$8.class
+-rw-rw-r--  2.0 unx      879 b- defN 23-Jun-06 10:35 sklearn/tree/RegressionCriterion.class
+-rw-rw-r--  2.0 unx     1151 b- defN 23-Jun-06 10:35 sklearn/tree/TreeUtil$5.class
+-rw-rw-r--  2.0 unx      978 b- defN 23-Jun-06 10:35 sklearn/tree/PresortBestSplitter.class
+-rw-rw-r--  2.0 unx      955 b- defN 23-Jun-06 10:35 sklearn/tree/TreeUtil$6.class
+-rw-rw-r--  2.0 unx     1764 b- defN 23-Jun-06 10:35 sklearn/tree/TreeRegressor.class
+-rw-rw-r--  2.0 unx     1589 b- defN 23-Jun-06 10:35 sklearn/tree/TreeUtil$7.class
+-rw-rw-r--  2.0 unx    20072 b- defN 23-Jun-06 10:35 sklearn/tree/TreeUtil.class
+-rw-rw-r--  2.0 unx     1123 b- defN 23-Jun-06 10:35 sklearn/tree/TreeUtil$3.class
+-rw-rw-r--  2.0 unx     1373 b- defN 23-Jun-06 10:35 sklearn/tree/HasTreeOptions.class
+-rw-rw-r--  2.0 unx     2257 b- defN 23-Jun-06 10:35 sklearn/tree/Tree.class
+-rw-rw-r--  2.0 unx      754 b- defN 23-Jun-06 10:35 sklearn/tree/TreeUtil$2.class
+-rw-rw-r--  2.0 unx      150 b- defN 23-Jun-06 10:35 sklearn/tree/HasTree.class
+-rw-rw-r--  2.0 unx     1967 b- defN 23-Jun-06 10:35 sklearn/InitializerUtil.class
+-rw-rw-r--  2.0 unx      570 b- defN 23-Jun-06 10:35 sklearn/Regressor.class
+-rw-rw-r--  2.0 unx      211 b- defN 23-Jun-06 10:35 sklearn/HasNumberOfOutputs.class
+-rw-rw-r--  2.0 unx      381 b- defN 23-Jun-06 10:35 sklearn/OutlierDetector.class
+-rw-rw-r--  2.0 unx     2366 b- defN 23-Jun-06 10:35 sklearn/Calibrator.class
+-rw-rw-r--  2.0 unx      273 b- defN 23-Jun-06 10:35 sklearn/HasClassifierOptions.class
+-rw-rw-r--  2.0 unx     7075 b- defN 23-Jun-06 10:35 sklearn/EstimatorUtil.class
+-rw-rw-r--  2.0 unx      199 b- defN 23-Jun-06 10:35 sklearn/HasType.class
+-rw-rw-r--  2.0 unx      678 b- defN 23-Jun-06 10:35 sklearn/cluster/MiniBatchKMeans.class
+-rw-rw-r--  2.0 unx     5086 b- defN 23-Jun-06 10:35 sklearn/cluster/KMeans.class
+-rw-rw-r--  2.0 unx    12172 b- defN 23-Jun-06 10:35 sklearn/Estimator.class
+-rw-rw-r--  2.0 unx     1624 b- defN 23-Jun-06 10:35 sklearn/Initializer.class
+-rw-rw-r--  2.0 unx     4598 b- defN 23-Jun-06 10:35 sklearn/multiclass/OneVsRestClassifier.class
+-rw-rw-r--  2.0 unx     5157 b- defN 23-Jun-06 10:35 sklearn2pmml/ruleset/RuleSetClassifier.class
+-rw-rw-r--  2.0 unx     1023 b- defN 23-Jun-06 10:35 sklearn2pmml/pipeline/PMMLPipeline$3.class
+-rw-rw-r--  2.0 unx    28136 b- defN 23-Jun-06 10:35 sklearn2pmml/pipeline/PMMLPipeline.class
+-rw-rw-r--  2.0 unx      980 b- defN 23-Jun-06 10:35 sklearn2pmml/pipeline/PMMLPipeline$2.class
+-rw-rw-r--  2.0 unx     1421 b- defN 23-Jun-06 10:35 sklearn2pmml/pipeline/PMMLPipeline$1.class
+-rw-rw-r--  2.0 unx     1811 b- defN 23-Jun-06 10:35 sklearn2pmml/pipeline/Verification.class
+-rw-rw-r--  2.0 unx     2162 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/MultiDomain.class
+-rw-rw-r--  2.0 unx     1152 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/ContinuousDomainEraser.class
+-rw-rw-r--  2.0 unx     1654 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/Alias.class
+-rw-rw-r--  2.0 unx     1772 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/TemporalDomain.class
+-rw-rw-r--  2.0 unx      779 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/ContinuousDomain$1.class
+-rw-rw-r--  2.0 unx    11878 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/Domain.class
+-rw-rw-r--  2.0 unx     1416 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/MultiAlias.class
+-rw-rw-r--  2.0 unx     5055 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/DiscreteDomain.class
+-rw-rw-r--  2.0 unx     1952 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/CategoricalDomain.class
+-rw-rw-r--  2.0 unx     1453 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/DomainEraser.class
+-rw-rw-r--  2.0 unx      613 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/DateTimeDomain.class
+-rw-rw-r--  2.0 unx     7764 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/ContinuousDomain.class
+-rw-rw-r--  2.0 unx     1083 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/DiscreteDomainEraser.class
+-rw-rw-r--  2.0 unx     1590 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/TransformerWrapper.class
+-rw-rw-r--  2.0 unx     1045 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/Domain$2.class
+-rw-rw-r--  2.0 unx      596 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/DateDomain.class
+-rw-rw-r--  2.0 unx     3544 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/DomainUtil.class
+-rw-rw-r--  2.0 unx     1033 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/Domain$1.class
+-rw-rw-r--  2.0 unx     1577 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/OrdinalDomain.class
+-rw-rw-r--  2.0 unx      672 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/Domain$4.class
+-rw-rw-r--  2.0 unx      799 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/Domain$3.class
+-rw-rw-r--  2.0 unx     7862 b- defN 23-Jun-06 10:35 sklearn2pmml/neural_network/MLPTransformer.class
+-rw-rw-r--  2.0 unx      391 b- defN 23-Jun-06 10:35 sklearn2pmml/SkLearn2PMMLFields.class
+-rw-rw-r--  2.0 unx     1160 b- defN 23-Jun-06 10:35 sklearn2pmml/util/Evaluatable.class
+-rw-rw-r--  2.0 unx     1196 b- defN 23-Jun-06 10:35 sklearn2pmml/util/Expression.class
+-rw-rw-r--  2.0 unx     1189 b- defN 23-Jun-06 10:35 sklearn2pmml/util/Predicate.class
+-rw-rw-r--  2.0 unx     1434 b- defN 23-Jun-06 10:35 sklearn2pmml/util/Reshaper.class
+-rw-rw-r--  2.0 unx     3392 b- defN 23-Jun-06 10:35 sklearn2pmml/util/EvaluatableUtil.class
+-rw-rw-r--  2.0 unx     1658 b- defN 23-Jun-06 10:35 sklearn2pmml/util/Slicer.class
+-rw-rw-r--  2.0 unx     2418 b- defN 23-Jun-06 10:35 sklearn2pmml/feature_extraction/text/Splitter.class
+-rw-rw-r--  2.0 unx     3184 b- defN 23-Jun-06 10:35 sklearn2pmml/feature_extraction/text/Matcher.class
+-rw-rw-r--  2.0 unx     1262 b- defN 23-Jun-06 10:35 sklearn2pmml/ensemble/SelectFirstRegressor.class
+-rw-rw-r--  2.0 unx     2083 b- defN 23-Jun-06 10:35 sklearn2pmml/ensemble/GBDTUtil$2.class
+-rw-rw-r--  2.0 unx     1134 b- defN 23-Jun-06 10:35 sklearn2pmml/ensemble/EstimatorChain$1.class
+-rw-rw-r--  2.0 unx     1934 b- defN 23-Jun-06 10:35 sklearn2pmml/ensemble/GBDTLMRegressor.class
+-rw-rw-r--  2.0 unx      948 b- defN 23-Jun-06 10:35 sklearn2pmml/ensemble/GBDTUtil$1.class
+-rw-rw-r--  2.0 unx     7358 b- defN 23-Jun-06 10:35 sklearn2pmml/ensemble/EstimatorChain.class
+-rw-rw-r--  2.0 unx     6578 b- defN 23-Jun-06 10:35 sklearn2pmml/ensemble/GBDTUtil.class
+-rw-rw-r--  2.0 unx     3995 b- defN 23-Jun-06 10:35 sklearn2pmml/ensemble/Link.class
+-rw-rw-r--  2.0 unx     4360 b- defN 23-Jun-06 10:35 sklearn2pmml/ensemble/SelectFirstUtil.class
+-rw-rw-r--  2.0 unx     4252 b- defN 23-Jun-06 10:35 sklearn2pmml/ensemble/GBDTLRClassifier.class
+-rw-rw-r--  2.0 unx     2608 b- defN 23-Jun-06 10:35 sklearn2pmml/ensemble/SelectFirstClassifier.class
+-rw-rw-r--  2.0 unx     1438 b- defN 23-Jun-06 10:35 sklearn2pmml/EstimatorProxy$1.class
+-rw-rw-r--  2.0 unx      946 b- defN 23-Jun-06 10:35 sklearn2pmml/feature_selection/SelectUnique.class
+-rw-rw-r--  2.0 unx     6477 b- defN 23-Jun-06 10:35 sklearn2pmml/postprocessing/BusinessDecisionTransformer.class
+-rw-rw-r--  2.0 unx      791 b- defN 23-Jun-06 10:35 sklearn2pmml/postprocessing/BusinessDecisionTransformer$1.class
+-rw-rw-r--  2.0 unx     1197 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/PatternTransformer.class
+-rw-rw-r--  2.0 unx     2908 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/ReplaceTransformer.class
+-rw-rw-r--  2.0 unx     1844 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/WordCountTransformer.class
+-rw-rw-r--  2.0 unx      597 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/DateTimeFormatter.class
+-rw-rw-r--  2.0 unx     1288 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/PMMLLabelBinarizer.class
+-rw-rw-r--  2.0 unx     4621 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/DurationTransformer.class
+-rw-rw-r--  2.0 unx      444 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/PMMLLabelEncoder.class
+-rw-rw-r--  2.0 unx     2777 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/FilterLookupTransformer.class
+-rw-rw-r--  2.0 unx     2545 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/Formatter.class
+-rw-rw-r--  2.0 unx     3341 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/CastTransformer.class
+-rw-rw-r--  2.0 unx     2758 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/MatchesTransformer.class
+-rw-rw-r--  2.0 unx      589 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/NumberFormatter.class
+-rw-rw-r--  2.0 unx     4149 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/MultiLookupTransformer.class
+-rw-rw-r--  2.0 unx     3871 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/StringNormalizer.class
+-rw-rw-r--  2.0 unx     7145 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/ExpressionTransformer.class
+-rw-rw-r--  2.0 unx      635 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/DaysSinceYearTransformer.class
+-rw-rw-r--  2.0 unx     3604 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/DataFrameConstructor.class
+-rw-rw-r--  2.0 unx     2847 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/ConcatTransformer.class
+-rw-rw-r--  2.0 unx     5993 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/CutTransformer.class
+-rw-rw-r--  2.0 unx     7025 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/BSplineTransformer.class
+-rw-rw-r--  2.0 unx     6410 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/LookupTransformer.class
+-rw-rw-r--  2.0 unx     3236 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/SubstringTransformer.class
+-rw-rw-r--  2.0 unx     3181 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/SecondsSinceMidnightTransformer.class
+-rw-rw-r--  2.0 unx     2132 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/PowerFunctionTransformer.class
+-rw-rw-r--  2.0 unx     3328 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/Aggregator.class
+-rw-rw-r--  2.0 unx      647 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/SecondsSinceYearTransformer.class
+-rw-rw-r--  2.0 unx     1728 b- defN 23-Jun-06 10:35 sklearn2pmml/tree/CHAIDRegressor.class
+-rw-rw-r--  2.0 unx    10719 b- defN 23-Jun-06 10:35 sklearn2pmml/tree/CHAIDUtil.class
+-rw-rw-r--  2.0 unx     2121 b- defN 23-Jun-06 10:35 sklearn2pmml/tree/CHAIDClassifier.class
+-rw-rw-r--  2.0 unx     1417 b- defN 23-Jun-06 10:35 sklearn2pmml/tree/CHAIDUtil$1.class
+-rw-rw-r--  2.0 unx     3864 b- defN 23-Jun-06 10:35 sklearn2pmml/EstimatorProxy.class
+-rw-rw-r--  2.0 unx     1458 b- defN 23-Jun-06 10:35 sklearn2pmml/SelectorProxy.class
+-rw-rw-r--  2.0 unx     2046 b- defN 23-Jun-06 10:35 sklearn2pmml/expression/ExpressionUtil.class
+-rw-rw-r--  2.0 unx     3799 b- defN 23-Jun-06 10:35 sklearn2pmml/expression/ExpressionRegressor.class
+-rw-rw-r--  2.0 unx      990 b- defN 23-Jun-06 10:35 sklearn2pmml/expression/ExpressionClassifier$1.class
+-rw-rw-r--  2.0 unx     8687 b- defN 23-Jun-06 10:35 sklearn2pmml/expression/ExpressionClassifier.class
+-rw-rw-r--  2.0 unx      948 b- defN 23-Jun-06 10:35 sklearn2pmml/expression/ExpressionUtil$1.class
+-rw-rw-r--  2.0 unx     1774 b- defN 23-Jun-06 10:35 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest$1.class
+-rw-rw-r--  2.0 unx     2764 b- defN 23-Jun-06 10:35 org/jpmml/sklearn/testing/SkLearnEncoderBatch.class
+-rw-rw-r--  2.0 unx     3549 b- defN 23-Jun-06 10:35 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest.class
+-rw-rw-r--  2.0 unx    13608 b- defN 23-Jun-06 10:35 org/jpmml/sklearn/SkLearnEncoder.class
+-rw-rw-r--  2.0 unx      194 b- defN 23-Jun-06 10:35 org/jpmml/sklearn/FieldNames.class
+-rw-rw-r--  2.0 unx      171 b- defN 23-Jun-06 10:35 org/jpmml/sklearn/HasSkLearnOptions.class
+-rw-rw-r--  2.0 unx     1030 b- defN 23-Jun-06 10:35 org/jpmml/sklearn/SkLearnEncoder$1.class
+-rw-rw-r--  2.0 unx     1822 b- defN 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn/pom.xml
+-rw-rw-r--  2.0 unx       57 b- defN 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn/pom.properties
+403 files, 920905 bytes uncompressed, 405921 bytes compressed:  55.9%
```

#### zipnote «TEMP»/diffoscope__evcigd9_/tmp3zf5v7vp_.zip

```diff
@@ -285,29 +285,26 @@
 
 Filename: sklearn/SkLearnOutlierTransformation.class
 Comment: 
 
 Filename: sklearn/HasEstimator.class
 Comment: 
 
+Filename: sklearn/OutlierDetectorUtil.class
+Comment: 
+
 Filename: sklearn/HasMultiApplyField.class
 Comment: 
 
 Filename: sklearn/None.class
 Comment: 
 
 Filename: sklearn/svm/SupportVectorMachineUtil.class
 Comment: 
 
-Filename: sklearn/svm/OneClassSVMUtil.class
-Comment: 
-
-Filename: sklearn/svm/OneClassSVMUtil$1.class
-Comment: 
-
 Filename: sklearn/svm/LinearSVC.class
 Comment: 
 
 Filename: sklearn/svm/LibSVMClassifier.class
 Comment: 
 
 Filename: sklearn/svm/SupportVectorMachineUtil$1.class
@@ -627,17 +624,14 @@
 
 Filename: sklearn/ensemble/iforest/IsolationForest$3.class
 Comment: 
 
 Filename: sklearn/ensemble/iforest/IsolationForest$1.class
 Comment: 
 
-Filename: sklearn/ensemble/iforest/IsolationForest$4.class
-Comment: 
-
 Filename: sklearn/ensemble/iforest/IsolationForest$2.class
 Comment: 
 
 Filename: sklearn/ensemble/iforest/IsolationForest.class
 Comment: 
 
 Filename: sklearn/ensemble/voting/VotingClassifier.class
@@ -726,14 +720,17 @@
 
 Filename: sklearn/SkLearnMethods.class
 Comment: 
 
 Filename: sklearn/ScalarLabelUtil.class
 Comment: 
 
+Filename: sklearn/OutlierDetectorUtil$1.class
+Comment: 
+
 Filename: sklearn/HasClasses.class
 Comment: 
 
 Filename: sklearn/discriminant_analysis/LinearDiscriminantAnalysis.class
 Comment: 
 
 Filename: sklearn/EstimatorUtil$1.class
@@ -882,14 +879,17 @@
 
 Filename: sklearn/Regressor.class
 Comment: 
 
 Filename: sklearn/HasNumberOfOutputs.class
 Comment: 
 
+Filename: sklearn/OutlierDetector.class
+Comment: 
+
 Filename: sklearn/Calibrator.class
 Comment: 
 
 Filename: sklearn/HasClassifierOptions.class
 Comment: 
 
 Filename: sklearn/EstimatorUtil.class
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,6 +1,6 @@
 Manifest-Version: 1.0
 Implementation-Title: JPMML-SkLearn library
-Implementation-Version: 1.7.28
+Implementation-Version: 1.7.29
 Build-Jdk-Spec: 1.8
-Created-By: Maven JAR Plugin 3.2.2
+Created-By: Maven JAR Plugin 3.3.0
```

#### sklearn/calibration/CalibratedClassifier.class

##### procyon -ec {}

```diff
@@ -141,15 +141,15 @@
                 RegressionModel calibratorModel;
                 if (calibrators.size() == 1) {
                     SchemaUtil.checkSize(2, categoricalLabel);
                     final Calibrator calibrator = (Calibrator)calibrators.get(0);
                     final Model featureModel = (Model)models.get(0);
                     final Feature feature = (Feature)decisionFunctionFeatures.get(0);
                     final Feature calibratedFeature = calibrate(calibrator, featureModel, feature, encoder);
-                    calibratorModel = RegressionModelUtil.createBinaryLogisticClassification((List)Collections.singletonList(calibratedFeature), (List)Collections.singletonList(Double.valueOf(1.0)), (Number)null, RegressionModel.NormalizationMethod.NONE, true, schema);
+                    calibratorModel = RegressionModelUtil.createBinaryLogisticClassification((List)Collections.singletonList(calibratedFeature), (List)Collections.singletonList(Double.valueOf(1.0)), (Number)null, RegressionModel.NormalizationMethod.NONE, false, schema);
                 }
                 else {
                     if (calibrators.size() < 3) {
                         throw new IllegalArgumentException();
                     }
                     SchemaUtil.checkSize(calibrators.size(), categoricalLabel);
                     final List<RegressionTable> regressionTables = new ArrayList<RegressionTable>();
@@ -157,16 +157,17 @@
                         final Calibrator calibrator2 = (Calibrator)calibrators.get(i);
                         final Model featureModel2 = (models.size() == 1) ? ((Model)models.get(0)) : ((Model)models.get(i));
                         final Feature feature2 = (Feature)decisionFunctionFeatures.get(i);
                         final Feature calibratedFeature2 = calibrate(calibrator2, featureModel2, feature2, encoder);
                         final RegressionTable regressionTable2 = RegressionModelUtil.createRegressionTable((List)Collections.singletonList(calibratedFeature2), (List)Collections.singletonList(Double.valueOf(1.0)), (Number)null).setTargetCategory(categoricalLabel.getValue(i));
                         regressionTables.add(regressionTable2);
                     }
-                    calibratorModel = new RegressionModel(MiningFunction.CLASSIFICATION, ModelUtil.createMiningSchema((Label)categoricalLabel), (List)regressionTables).setNormalizationMethod(RegressionModel.NormalizationMethod.SIMPLEMAX).setOutput(ModelUtil.createProbabilityOutput(DataType.DOUBLE, categoricalLabel));
+                    calibratorModel = new RegressionModel(MiningFunction.CLASSIFICATION, ModelUtil.createMiningSchema((Label)categoricalLabel), (List)regressionTables).setNormalizationMethod(RegressionModel.NormalizationMethod.SIMPLEMAX);
                 }
+                this.encodePredictProbaOutput((Model)calibratorModel, DataType.DOUBLE, categoricalLabel);
                 models.add((Model)calibratorModel);
                 return (Model)MiningModelUtil.createModelChain((List)models, Segmentation.MissingPredictionTreatment.RETURN_MISSING);
             }
             default: {
                 throw new IllegalArgumentException(method);
             }
         }
```

#### sklearn/dummy/DummyClassifier.class

##### procyon -ec {}

```diff
@@ -1,13 +1,13 @@
 
 package sklearn.dummy;
 
-import org.dmg.pmml.Model;
 import com.google.common.primitives.Doubles;
 import org.dmg.pmml.tree.Node;
+import org.dmg.pmml.Model;
 import org.dmg.pmml.DataType;
 import org.jpmml.converter.Label;
 import org.jpmml.converter.ModelUtil;
 import org.dmg.pmml.MiningFunction;
 import org.dmg.pmml.PMMLObject;
 import org.dmg.pmml.Predicate;
 import org.dmg.pmml.tree.ClassifierNode;
@@ -110,15 +110,16 @@
             default: {
                 throw new IllegalArgumentException(strategy);
             }
         }
         final Node root = (Node)new ClassifierNode(categoricalLabel.getValue(maxIndex), (Predicate)True.INSTANCE);
         final ScoreDistributionManager scoreDistributionManager = new ScoreDistributionManager();
         scoreDistributionManager.addScoreDistributions((PMMLObject)root, categoricalLabel.getValues(), (List)null, (List)probabilities);
-        final TreeModel treeModel = new TreeModel(MiningFunction.CLASSIFICATION, ModelUtil.createMiningSchema((Label)categoricalLabel), root).setOutput(ModelUtil.createProbabilityOutput(DataType.DOUBLE, categoricalLabel));
+        final TreeModel treeModel = new TreeModel(MiningFunction.CLASSIFICATION, ModelUtil.createMiningSchema((Label)categoricalLabel), root);
+        this.encodePredictProbaOutput((Model)treeModel, DataType.DOUBLE, categoricalLabel);
         return treeModel;
     }
     
     public List<? extends Number> getClassPrior() {
         return this.getNumberArray("class_prior_");
     }
```

#### sklearn/HasMultiApplyField.class

##### procyon -ec {}

```diff
@@ -1,24 +1,24 @@
 
 package sklearn;
 
 import org.jpmml.converter.FieldNameUtil;
 import java.util.ArrayList;
 import java.util.List;
 
-public interface HasMultiApplyField
+public interface HasMultiApplyField extends HasApplyField
 {
     int getNumberOfApplyFields();
     
     default List<String> getApplyFields() {
         final List<String> result = new ArrayList<String>();
         for (int i = 0, max = this.getNumberOfApplyFields(); i < max; ++i) {
-            final String name = this.getApplyField(i);
+            final String name = this.getApplyField(Integer.valueOf(i + 1));
             result.add(name);
         }
         return result;
     }
     
-    default String getApplyField(final int index) {
-        return FieldNameUtil.create("apply", new Object[] { Integer.valueOf(index) });
+    default String getApplyField(final Object segmentId) {
+        return FieldNameUtil.create(this.getApplyField(), new Object[] { segmentId });
     }
 }
```

#### sklearn/svm/OneClassSVM.class

##### procyon -ec {}

```diff
@@ -1,24 +1,26 @@
 
 package sklearn.svm;
 
 import org.dmg.pmml.Model;
 import sklearn.Estimator;
+import sklearn.OutlierDetectorUtil;
 import org.dmg.pmml.support_vector_machine.SupportVectorMachineModel;
 import org.jpmml.converter.Schema;
+import sklearn.OutlierDetector;
 import sklearn.HasDecisionFunctionField;
 
-public class OneClassSVM extends LibSVMRegressor implements HasDecisionFunctionField
+public class OneClassSVM extends LibSVMRegressor implements HasDecisionFunctionField, OutlierDetector
 {
     public OneClassSVM(final String module, final String name) {
         super(module, name);
     }
     
     public boolean isSupervised() {
         return false;
     }
     
     public SupportVectorMachineModel encodeModel(final Schema schema) {
-        final SupportVectorMachineModel supportVectorMachineModel = super.encodeModel(schema).setOutput(OneClassSVMUtil.createPredictedOutput((Estimator)this));
+        final SupportVectorMachineModel supportVectorMachineModel = super.encodeModel(schema).setOutput(OutlierDetectorUtil.createPredictedOutput((Estimator)this));
         return supportVectorMachineModel;
     }
 }
```

#### sklearn/Estimator$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 54a50ab01ad8749f7400c08043594cccac92f45e6b47f577a015c927a6caf776
+  SHA-256 checksum 514424329a09acf594bae97a6fb982c696553a1aad76adf2458d561dfb7540d3
   Compiled from "Estimator.java"
 class sklearn.Estimator$1
   minor version: 0
   major version: 52
   flags: (0x1020) ACC_SUPER, ACC_SYNTHETIC
   this_class: #8                          // sklearn/Estimator$1
   super_class: #9                         // java/lang/Object
@@ -89,15 +89,15 @@
         54: return
       Exception table:
          from    to  target type
              9    20    23   Class java/lang/NoSuchFieldError
             24    35    38   Class java/lang/NoSuchFieldError
             39    50    53   Class java/lang/NoSuchFieldError
       LineNumberTable:
-        line 99: 0
+        line 106: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
       StackMapTable: number_of_entries = 6
         frame_type = 87 /* same_locals_1_stack_item */
           stack = [ class java/lang/NoSuchFieldError ]
         frame_type = 0 /* same */
         frame_type = 77 /* same_locals_1_stack_item */
```

#### sklearn/neural_network/MLPClassifier.class

##### procyon -ec {}

```diff
@@ -1,15 +1,14 @@
 
 package sklearn.neural_network;
 
 import org.dmg.pmml.Model;
-import org.jpmml.converter.ModelUtil;
-import org.jpmml.converter.CategoricalLabel;
 import org.dmg.pmml.DataType;
 import org.dmg.pmml.MiningFunction;
+import org.jpmml.converter.CategoricalLabel;
 import org.dmg.pmml.neural_network.NeuralNetwork;
 import org.jpmml.converter.Schema;
 import org.jpmml.python.HasArray;
 import java.util.List;
 import sklearn.Classifier;
 
 public class MLPClassifier extends Classifier
@@ -23,15 +22,17 @@
         return MultilayerPerceptronUtil.getNumberOfFeatures((List)coefs);
     }
     
     public NeuralNetwork encodeModel(final Schema schema) {
         final String activation = this.getActivation();
         final List<? extends HasArray> coefs = this.getCoefs();
         final List<? extends HasArray> intercepts = this.getIntercepts();
-        final NeuralNetwork neuralNetwork = MultilayerPerceptronUtil.encodeNeuralNetwork(MiningFunction.CLASSIFICATION, activation, (List)coefs, (List)intercepts, schema).setOutput(ModelUtil.createProbabilityOutput(DataType.DOUBLE, (CategoricalLabel)schema.getLabel()));
+        final CategoricalLabel categoricalLabel = (CategoricalLabel)schema.getLabel();
+        final NeuralNetwork neuralNetwork = MultilayerPerceptronUtil.encodeNeuralNetwork(MiningFunction.CLASSIFICATION, activation, (List)coefs, (List)intercepts, schema);
+        this.encodePredictProbaOutput((Model)neuralNetwork, DataType.DOUBLE, categoricalLabel);
         return neuralNetwork;
     }
     
     public String getActivation() {
         return this.getString("activation");
     }
```

#### sklearn/naive_bayes/GaussianNB.class

##### procyon -ec {}

```diff
@@ -1,20 +1,20 @@
 
 package sklearn.naive_bayes;
 
-import org.dmg.pmml.Model;
 import org.dmg.pmml.naive_bayes.TargetValueCount;
 import org.dmg.pmml.ContinuousDistribution;
 import org.dmg.pmml.naive_bayes.TargetValueStat;
 import org.dmg.pmml.GaussianDistribution;
 import org.jpmml.python.ClassDictUtil;
 import java.util.Collection;
 import org.dmg.pmml.naive_bayes.TargetValueStats;
 import org.jpmml.converter.ContinuousFeature;
 import org.jpmml.converter.Feature;
+import org.dmg.pmml.Model;
 import org.dmg.pmml.DataType;
 import org.jpmml.converter.Label;
 import org.jpmml.converter.ModelUtil;
 import org.dmg.pmml.MiningFunction;
 import org.dmg.pmml.naive_bayes.TargetValueCounts;
 import org.dmg.pmml.naive_bayes.BayesOutput;
 import org.dmg.pmml.naive_bayes.BayesInput;
@@ -51,15 +51,16 @@
             final List<? extends Number> variances = CMatrixUtil.getColumn((List)sigma, numberOfClasses, numberOfFeatures, i);
             final ContinuousFeature continuousFeature = feature.toContinuousFeature();
             final BayesInput bayesInput = new BayesInput(continuousFeature.getName(), encodeTargetValueStats(categoricalLabel.getValues(), means, variances), (List)null);
             bayesInputs.addBayesInputs(new BayesInput[] { bayesInput });
         }
         final List<Integer> classCount = this.getClassCount();
         final BayesOutput bayesOutput = new BayesOutput((TargetValueCounts)null).setTargetField(categoricalLabel.getName()).setTargetValueCounts(encodeTargetValueCounts((List<?>)categoricalLabel.getValues(), classCount));
-        final NaiveBayesModel naiveBayesModel = new NaiveBayesModel((Number)Double.valueOf(0.0), MiningFunction.CLASSIFICATION, ModelUtil.createMiningSchema((Label)categoricalLabel), bayesInputs, bayesOutput).setOutput(ModelUtil.createProbabilityOutput(DataType.DOUBLE, categoricalLabel));
+        final NaiveBayesModel naiveBayesModel = new NaiveBayesModel((Number)Double.valueOf(0.0), MiningFunction.CLASSIFICATION, ModelUtil.createMiningSchema((Label)categoricalLabel), bayesInputs, bayesOutput);
+        this.encodePredictProbaOutput((Model)naiveBayesModel, DataType.DOUBLE, categoricalLabel);
         return naiveBayesModel;
     }
     
     public List<Integer> getClassCount() {
         return this.getIntegerArray("class_count_");
     }
```

#### sklearn/linear_model/LinearRegressor.class

##### procyon -ec {}

```diff
@@ -1,18 +1,18 @@
 
 package sklearn.linear_model;
 
 import org.jpmml.converter.regression.RegressionModelUtil;
+import org.dmg.pmml.regression.RegressionModel;
 import org.jpmml.converter.Feature;
 import org.jpmml.converter.Label;
 import org.jpmml.converter.mining.MiningModelUtil;
 import org.dmg.pmml.mining.Segmentation;
 import java.util.List;
 import org.jpmml.converter.CMatrixUtil;
-import org.dmg.pmml.regression.RegressionModel;
 import java.util.ArrayList;
 import org.jpmml.python.ClassDictUtil;
 import java.util.Collection;
 import org.jpmml.converter.MultiLabel;
 import com.google.common.collect.Iterables;
 import org.dmg.pmml.Model;
 import org.jpmml.converter.Schema;
@@ -48,21 +48,21 @@
         final int numberOfOutputs = this.getNumberOfOutputs();
         if (numberOfOutputs == 1) {
             return (Model)this.createRegression(coef, (Number)Iterables.getOnlyElement((Iterable)intercept), schema);
         }
         if (numberOfOutputs >= 2) {
             final MultiLabel multiLabel = (MultiLabel)label;
             ClassDictUtil.checkSize(numberOfOutputs, new Collection[] { intercept, multiLabel.getLabels() });
-            final List<RegressionModel> regressionModels = new ArrayList<RegressionModel>();
+            final List<Model> models = new ArrayList<Model>();
             for (int i = 0, max = numberOfOutputs; i < max; ++i) {
                 final Schema segmentSchema = schema.toRelabeledSchema(multiLabel.getLabel(i));
-                final RegressionModel regressionModel = this.createRegression(CMatrixUtil.getRow((List)coef, numberOfOutputs, features.size(), i), (Number)intercept.get(i), segmentSchema);
-                regressionModels.add(regressionModel);
+                final Model model = (Model)this.createRegression(CMatrixUtil.getRow((List)coef, numberOfOutputs, features.size(), i), (Number)intercept.get(i), segmentSchema);
+                models.add(model);
             }
-            return (Model)MiningModelUtil.createMultiModelChain((List)regressionModels, Segmentation.MissingPredictionTreatment.CONTINUE);
+            return (Model)MiningModelUtil.createMultiModelChain((List)models, Segmentation.MissingPredictionTreatment.CONTINUE);
         }
         throw new IllegalArgumentException();
     }
     
     protected RegressionModel createRegression(final List<? extends Number> coef, final Number intercept, final Schema schema) {
         return RegressionModelUtil.createRegression(schema.getFeatures(), (List)coef, intercept, (RegressionModel.NormalizationMethod)null, schema);
     }
```

#### sklearn/linear_model/LinearClassifier.class

##### procyon -ec {}

```diff
@@ -1,10 +1,11 @@
 
 package sklearn.linear_model;
 
+import org.dmg.pmml.mining.MiningModel;
 import org.jpmml.converter.Feature;
 import org.jpmml.converter.mining.MiningModelUtil;
 import org.jpmml.converter.ModelUtil;
 import org.jpmml.converter.Transformation;
 import org.dmg.pmml.OpType;
 import org.jpmml.converter.FieldNameUtil;
 import java.util.ArrayList;
@@ -37,25 +38,33 @@
         final boolean hasProbabilityDistribution = this.hasProbabilityDistribution();
         final List<? extends Number> coef = this.getCoef();
         final List<? extends Number> intercept = this.getIntercept();
         final CategoricalLabel categoricalLabel = (CategoricalLabel)schema.getLabel();
         final List<? extends Feature> features = schema.getFeatures();
         if (numberOfClasses == 1) {
             SchemaUtil.checkSize(2, categoricalLabel);
-            return (Model)RegressionModelUtil.createBinaryLogisticClassification((List)features, CMatrixUtil.getRow((List)coef, numberOfClasses, numberOfFeatures, 0), (Number)intercept.get(0), RegressionModel.NormalizationMethod.LOGIT, hasProbabilityDistribution, schema);
+            final RegressionModel regressionModel = RegressionModelUtil.createBinaryLogisticClassification((List)features, CMatrixUtil.getRow((List)coef, numberOfClasses, numberOfFeatures, 0), (Number)intercept.get(0), RegressionModel.NormalizationMethod.LOGIT, false, schema);
+            if (hasProbabilityDistribution) {
+                this.encodePredictProbaOutput((Model)regressionModel, DataType.DOUBLE, categoricalLabel);
+            }
+            return (Model)regressionModel;
         }
         if (numberOfClasses >= 3) {
             SchemaUtil.checkSize(numberOfClasses, categoricalLabel);
             final Schema segmentSchema = schema.toAnonymousRegressorSchema(DataType.DOUBLE).toEmptySchema();
-            final List<RegressionModel> regressionModels = new ArrayList<RegressionModel>();
+            final List<Model> models = new ArrayList<Model>();
             for (int i = 0, rows = categoricalLabel.size(); i < rows; ++i) {
-                final RegressionModel regressionModel = RegressionModelUtil.createRegression((List)features, CMatrixUtil.getRow((List)coef, numberOfClasses, numberOfFeatures, i), (Number)intercept.get(i), RegressionModel.NormalizationMethod.LOGIT, segmentSchema).setOutput(ModelUtil.createPredictedOutput(FieldNameUtil.create("decisionFunction", new Object[] { categoricalLabel.getValue(i) }), OpType.CONTINUOUS, DataType.DOUBLE, new Transformation[0]));
-                regressionModels.add(regressionModel);
+                final Model model = (Model)RegressionModelUtil.createRegression((List)features, CMatrixUtil.getRow((List)coef, numberOfClasses, numberOfFeatures, i), (Number)intercept.get(i), RegressionModel.NormalizationMethod.LOGIT, segmentSchema).setOutput(ModelUtil.createPredictedOutput(FieldNameUtil.create("decisionFunction", new Object[] { categoricalLabel.getValue(i) }), OpType.CONTINUOUS, DataType.DOUBLE, new Transformation[0]));
+                models.add(model);
+            }
+            final MiningModel miningModel = MiningModelUtil.createClassification((List)models, RegressionModel.NormalizationMethod.SIMPLEMAX, false, schema);
+            if (hasProbabilityDistribution) {
+                this.encodePredictProbaOutput((Model)miningModel, DataType.DOUBLE, categoricalLabel);
             }
-            return (Model)MiningModelUtil.createClassification((List)regressionModels, RegressionModel.NormalizationMethod.SIMPLEMAX, hasProbabilityDistribution, schema);
+            return (Model)miningModel;
         }
         throw new IllegalArgumentException();
     }
     
     public List<? extends Number> getCoef() {
         return this.getNumberArray("coef_");
     }
```

#### sklearn/linear_model/logistic/LogisticRegression.class

##### procyon -ec {}

```diff
@@ -1,10 +1,11 @@
 
 package sklearn.linear_model.logistic;
 
+import org.dmg.pmml.mining.MiningModel;
 import org.jpmml.converter.Feature;
 import org.jpmml.converter.PMMLEncoder;
 import org.jpmml.converter.mining.MiningModelUtil;
 import org.dmg.pmml.mining.Segmentation;
 import java.util.Arrays;
 import org.dmg.pmml.MiningFunction;
 import org.dmg.pmml.regression.RegressionTable;
@@ -68,33 +69,36 @@
         if (numberOfClasses == 1) {
             SchemaUtil.checkSize(2, categoricalLabel);
             final boolean corrected = sklearnVersion != null && SkLearnUtil.compareVersion(sklearnVersion, "0.20") >= 0;
             if (!corrected) {
                 return this.encodeOvRModel(schema);
             }
             final Schema segmentSchema = schema.toRelabeledSchema((Label)null);
-            final RegressionModel firstRegressionModel = RegressionModelUtil.createRegression((List)features, CMatrixUtil.getRow((List)coef, 1, numberOfFeatures, 0), (Number)intercept.get(0), (RegressionModel.NormalizationMethod)null, segmentSchema).setOutput(ModelUtil.createPredictedOutput("decisionFunction", OpType.CONTINUOUS, DataType.DOUBLE, new Transformation[0]));
+            final Model firstModel = (Model)RegressionModelUtil.createRegression((List)features, CMatrixUtil.getRow((List)coef, 1, numberOfFeatures, 0), (Number)intercept.get(0), (RegressionModel.NormalizationMethod)null, segmentSchema).setOutput(ModelUtil.createPredictedOutput("decisionFunction", OpType.CONTINUOUS, DataType.DOUBLE, new Transformation[0]));
             final Feature feature = (Feature)new ContinuousFeature(encoder, "decisionFunction", DataType.DOUBLE);
             final RegressionTable passiveRegressionTable = RegressionModelUtil.createRegressionTable((List)Collections.singletonList(feature), (List)Collections.singletonList(Double.valueOf(-1.0)), (Number)Double.valueOf(0.0)).setTargetCategory(categoricalLabel.getValue(0));
             final RegressionTable activeRegressionTable = RegressionModelUtil.createRegressionTable((List)Collections.singletonList(feature), (List)Collections.singletonList(Double.valueOf(1.0)), (Number)Double.valueOf(0.0)).setTargetCategory(categoricalLabel.getValue(1));
             final List<RegressionTable> regressionTables = new ArrayList<RegressionTable>();
             regressionTables.add(passiveRegressionTable);
             regressionTables.add(activeRegressionTable);
-            final RegressionModel secondRegressionModel = new RegressionModel(MiningFunction.CLASSIFICATION, ModelUtil.createMiningSchema((Label)categoricalLabel), (List)regressionTables).setNormalizationMethod(RegressionModel.NormalizationMethod.SOFTMAX).setOutput(ModelUtil.createProbabilityOutput(DataType.DOUBLE, categoricalLabel));
-            return (Model)MiningModelUtil.createModelChain((List)Arrays.asList(firstRegressionModel, secondRegressionModel), Segmentation.MissingPredictionTreatment.RETURN_MISSING);
+            final Model secondModel = (Model)new RegressionModel(MiningFunction.CLASSIFICATION, ModelUtil.createMiningSchema((Label)categoricalLabel), (List)regressionTables).setNormalizationMethod(RegressionModel.NormalizationMethod.SOFTMAX);
+            final MiningModel miningModel = MiningModelUtil.createModelChain((List)Arrays.asList(firstModel, secondModel), Segmentation.MissingPredictionTreatment.RETURN_MISSING);
+            this.encodePredictProbaOutput((Model)miningModel, DataType.DOUBLE, categoricalLabel);
+            return (Model)miningModel;
         }
         else {
             if (numberOfClasses >= 3) {
                 SchemaUtil.checkSize(numberOfClasses, categoricalLabel);
                 final List<RegressionTable> regressionTables2 = new ArrayList<RegressionTable>();
                 for (int i = 0; i < categoricalLabel.size(); ++i) {
                     final RegressionTable regressionTable = RegressionModelUtil.createRegressionTable((List)features, CMatrixUtil.getRow((List)coef, numberOfClasses, numberOfFeatures, i), (Number)intercept.get(i)).setTargetCategory(categoricalLabel.getValue(i));
                     regressionTables2.add(regressionTable);
                 }
-                final RegressionModel regressionModel = new RegressionModel(MiningFunction.CLASSIFICATION, ModelUtil.createMiningSchema((Label)categoricalLabel), (List)regressionTables2).setNormalizationMethod(RegressionModel.NormalizationMethod.SOFTMAX).setOutput(ModelUtil.createProbabilityOutput(DataType.DOUBLE, categoricalLabel));
+                final RegressionModel regressionModel = new RegressionModel(MiningFunction.CLASSIFICATION, ModelUtil.createMiningSchema((Label)categoricalLabel), (List)regressionTables2).setNormalizationMethod(RegressionModel.NormalizationMethod.SOFTMAX);
+                this.encodePredictProbaOutput((Model)regressionModel, DataType.DOUBLE, categoricalLabel);
                 return (Model)regressionModel;
             }
             throw new IllegalArgumentException();
         }
     }
     
     private Model encodeOvRModel(final Schema schema) {
```

#### sklearn/linear_model/stochastic_gradient/SGDOneClassSVM.class

##### procyon -ec {}

```diff
@@ -1,35 +1,36 @@
 
 package sklearn.linear_model.stochastic_gradient;
 
 import org.dmg.pmml.Model;
 import sklearn.Estimator;
-import sklearn.svm.OneClassSVMUtil;
+import sklearn.OutlierDetectorUtil;
 import java.util.List;
 import org.jpmml.converter.regression.RegressionModelUtil;
 import com.google.common.collect.Iterables;
 import org.dmg.pmml.regression.RegressionModel;
 import org.jpmml.converter.Schema;
+import sklearn.OutlierDetector;
 import sklearn.HasDecisionFunctionField;
 import sklearn.Regressor;
 
-public class SGDOneClassSVM extends Regressor implements HasDecisionFunctionField
+public class SGDOneClassSVM extends Regressor implements HasDecisionFunctionField, OutlierDetector
 {
     public SGDOneClassSVM(final String module, final String name) {
         super(module, name);
     }
     
     public boolean isSupervised() {
         return false;
     }
     
     public RegressionModel encodeModel(final Schema schema) {
         final List<? extends Number> coef = this.getCoef();
         final List<? extends Number> offset = this.getOffset();
-        final RegressionModel regressionModel = RegressionModelUtil.createRegression(schema.getFeatures(), (List)coef, (Number)Double.valueOf(-1.0 * ((Number)Iterables.getOnlyElement((Iterable)offset)).doubleValue()), (RegressionModel.NormalizationMethod)null, schema).setOutput(OneClassSVMUtil.createPredictedOutput((Estimator)this));
+        final RegressionModel regressionModel = RegressionModelUtil.createRegression(schema.getFeatures(), (List)coef, (Number)Double.valueOf(-1.0 * ((Number)Iterables.getOnlyElement((Iterable)offset)).doubleValue()), (RegressionModel.NormalizationMethod)null, schema).setOutput(OutlierDetectorUtil.createPredictedOutput((Estimator)this));
         return regressionModel;
     }
     
     public List<? extends Number> getCoef() {
         return this.getNumberArray("coef_");
     }
```

#### sklearn/Classifier.class

##### procyon -ec {}

```diff
@@ -1,10 +1,19 @@
 
 package sklearn;
 
+import org.dmg.pmml.Output;
+import java.util.Collection;
+import org.jpmml.converter.ModelUtil;
+import org.jpmml.converter.mining.MiningModelUtil;
+import org.dmg.pmml.mining.MiningModel;
+import org.dmg.pmml.OutputField;
+import org.jpmml.converter.CategoricalLabel;
+import org.dmg.pmml.DataType;
+import org.dmg.pmml.Model;
 import java.util.stream.Collector;
 import java.util.stream.Collectors;
 import org.jpmml.python.HasArray;
 import java.util.List;
 import org.dmg.pmml.MiningFunction;
 
 public abstract class Classifier extends Estimator implements HasClasses
@@ -25,11 +34,22 @@
         return canonicalizeValues(values);
     }
     
     public boolean hasProbabilityDistribution() {
         return true;
     }
     
+    public List<OutputField> encodePredictProbaOutput(Model model, final DataType dataType, final CategoricalLabel categoricalLabel) {
+        final List<OutputField> predictProbaFields = this.createPredictProbaFields(dataType, categoricalLabel);
+        if (model instanceof MiningModel) {
+            final MiningModel miningModel = (MiningModel)model;
+            model = MiningModelUtil.getFinalModel(miningModel);
+        }
+        final Output output = ModelUtil.ensureOutput(model);
+        output.getOutputFields().addAll(predictProbaFields);
+        return predictProbaFields;
+    }
+    
     private static List<?> canonicalizeValues(final List<?> values) {
         return values.stream().map(value -> (value instanceof Long) ? Integer.valueOf(Math.toIntExact((long)value)) : value).collect((Collector<? super Object, ?, List<? super Object>>)Collectors.toList());
     }
 }
```

#### sklearn/ensemble/bagging/BaggingClassifier.class

##### procyon -ec {}

```diff
@@ -1,42 +1,43 @@
 
 package sklearn.ensemble.bagging;
 
-import org.dmg.pmml.Model;
 import sklearn.ensemble.EnsembleUtil;
 import org.jpmml.python.HasArray;
 import java.util.Iterator;
-import org.jpmml.converter.ModelUtil;
-import org.jpmml.converter.CategoricalLabel;
+import org.dmg.pmml.Model;
 import org.dmg.pmml.DataType;
 import java.util.List;
 import org.dmg.pmml.MiningFunction;
 import sklearn.Classifier;
 import org.dmg.pmml.mining.Segmentation;
+import org.jpmml.converter.CategoricalLabel;
 import org.dmg.pmml.mining.MiningModel;
 import org.jpmml.converter.Schema;
 import sklearn.ensemble.EnsembleClassifier;
 
 public class BaggingClassifier extends EnsembleClassifier
 {
     public BaggingClassifier(final String module, final String name) {
         super(module, name);
     }
     
     public MiningModel encodeModel(final Schema schema) {
         final List<? extends Classifier> estimators = this.getEstimators();
         final List<List<Integer>> estimatorsFeatures = this.getEstimatorsFeatures();
+        final CategoricalLabel categoricalLabel = (CategoricalLabel)schema.getLabel();
         Segmentation.MultipleModelMethod multipleModelMethod = Segmentation.MultipleModelMethod.AVERAGE;
         for (final Classifier estimator : estimators) {
             if (!estimator.hasProbabilityDistribution()) {
                 multipleModelMethod = Segmentation.MultipleModelMethod.MAJORITY_VOTE;
                 break;
             }
         }
-        final MiningModel miningModel = BaggingUtil.encodeBagging((List)estimators, (List)estimatorsFeatures, multipleModelMethod, MiningFunction.CLASSIFICATION, schema).setOutput(ModelUtil.createProbabilityOutput(DataType.DOUBLE, (CategoricalLabel)schema.getLabel()));
+        final MiningModel miningModel = BaggingUtil.encodeBagging((List)estimators, (List)estimatorsFeatures, multipleModelMethod, MiningFunction.CLASSIFICATION, schema);
+        this.encodePredictProbaOutput((Model)miningModel, DataType.DOUBLE, categoricalLabel);
         return miningModel;
     }
     
     public List<List<Integer>> getEstimatorsFeatures() {
         return EnsembleUtil.transformEstimatorsFeatures(this.getList("estimators_features_", (Class)HasArray.class));
     }
 }
```

#### sklearn/ensemble/stacking/StackingClassifier.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 771d4ad04e93683af3b7392a0c634045ed9fc10d6422f7ccf646bca15e33fc87
+  SHA-256 checksum 84f535de501c322f4d71d75914657d985114528c4598069f04d0343cb5abde6c
   Compiled from "StackingClassifier.java"
 public class sklearn.ensemble.stacking.StackingClassifier extends sklearn.Classifier implements sklearn.HasEstimatorEnsemble<sklearn.Classifier>
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #27                         // sklearn/ensemble/stacking/StackingClassifier
   super_class: #18                        // sklearn/Classifier
@@ -159,16 +159,16 @@
       stack=3, locals=3, args_size=3
          0: aload_0
          1: aload_1
          2: aload_2
          3: invokespecial #1                  // Method sklearn/Classifier."<init>":(Ljava/lang/String;Ljava/lang/String;)V
          6: return
       LineNumberTable:
-        line 45: 0
-        line 46: 6
+        line 40: 0
+        line 41: 6
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       7     0  this   Lsklearn/ensemble/stacking/StackingClassifier;
             0       7     1 module   Ljava/lang/String;
             0       7     2  name   Ljava/lang/String;
 
   public int getNumberOfFeatures();
@@ -179,16 +179,16 @@
          0: aload_0
          1: invokevirtual #2                  // Method getEstimators:()Ljava/util/List;
          4: astore_1
          5: aload_1
          6: invokestatic  #3                  // Method sklearn/StepUtil.getNumberOfFeatures:(Ljava/util/List;)I
          9: ireturn
       LineNumberTable:
-        line 50: 0
-        line 52: 5
+        line 45: 0
+        line 47: 5
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lsklearn/ensemble/stacking/StackingClassifier;
             5       5     1 estimators   Ljava/util/List;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
             5       5     1 estimators   Ljava/util/List<+Lsklearn/Classifier;>;
@@ -239,24 +239,24 @@
         78: aload_3
         79: aload         4
         81: invokevirtual #15                 // Method java/lang/Boolean.booleanValue:()Z
         84: aload_1
         85: invokestatic  #16                 // Method sklearn/ensemble/stacking/StackingUtil.encodeStacking:(Ljava/util/List;Ljava/util/List;Lsklearn/ensemble/stacking/StackingUtil$PredictFunction;Lsklearn/Estimator;ZLorg/jpmml/converter/Schema;)Lorg/dmg/pmml/mining/MiningModel;
         88: areturn
       LineNumberTable:
-        line 57: 0
-        line 58: 5
-        line 59: 10
-        line 60: 16
-        line 62: 22
-        line 66: 31
-        line 67: 40
-        line 71: 54
-        line 74: 61
-        line 119: 73
+        line 52: 0
+        line 53: 5
+        line 54: 10
+        line 55: 16
+        line 57: 22
+        line 61: 31
+        line 62: 40
+        line 66: 54
+        line 69: 61
+        line 93: 73
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            51       3     7 values   Ljava/util/List;
             0      89     0  this   Lsklearn/ensemble/stacking/StackingClassifier;
             0      89     1 schema   Lorg/jpmml/converter/Schema;
             5      84     2 estimators   Ljava/util/List;
            10      79     3 finalEstimator   Lsklearn/Classifier;
@@ -287,15 +287,15 @@
       stack=3, locals=1, args_size=1
          0: aload_0
          1: ldc           #17                 // String estimators_
          3: ldc           #18                 // class sklearn/Classifier
          5: invokevirtual #19                 // Method getList:(Ljava/lang/String;Ljava/lang/Class;)Ljava/util/List;
          8: areturn
       LineNumberTable:
-        line 124: 0
+        line 98: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       9     0  this   Lsklearn/ensemble/stacking/StackingClassifier;
     Signature: #74                          // ()Ljava/util/List<+Lsklearn/Classifier;>;
 
   public sklearn.Classifier getFinalEstimator();
     descriptor: ()Lsklearn/Classifier;
@@ -305,30 +305,30 @@
          0: aload_0
          1: ldc           #20                 // String final_estimator_
          3: ldc           #18                 // class sklearn/Classifier
          5: invokevirtual #21                 // Method get:(Ljava/lang/String;Ljava/lang/Class;)Ljava/lang/Object;
          8: checkcast     #18                 // class sklearn/Classifier
         11: areturn
       LineNumberTable:
-        line 128: 0
+        line 102: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      12     0  this   Lsklearn/ensemble/stacking/StackingClassifier;
 
   public java.lang.Boolean getPassthrough();
     descriptor: ()Ljava/lang/Boolean;
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=2, locals=1, args_size=1
          0: aload_0
          1: ldc           #22                 // String passthrough
          3: invokevirtual #23                 // Method getBoolean:(Ljava/lang/String;)Ljava/lang/Boolean;
          6: areturn
       LineNumberTable:
-        line 132: 0
+        line 106: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       7     0  this   Lsklearn/ensemble/stacking/StackingClassifier;
 
   public java.util.List<java.lang.String> getStackMethod();
     descriptor: ()Ljava/util/List;
     flags: (0x0001) ACC_PUBLIC
@@ -336,15 +336,15 @@
       stack=3, locals=1, args_size=1
          0: aload_0
          1: ldc           #24                 // String stack_method_
          3: ldc           #25                 // class java/lang/String
          5: invokevirtual #19                 // Method getList:(Ljava/lang/String;Ljava/lang/Class;)Ljava/util/List;
          8: areturn
       LineNumberTable:
-        line 136: 0
+        line 110: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       9     0  this   Lsklearn/ensemble/stacking/StackingClassifier;
     Signature: #80                          // ()Ljava/util/List<Ljava/lang/String;>;
 
   public org.dmg.pmml.Model encodeModel(org.jpmml.converter.Schema);
     descriptor: (Lorg/jpmml/converter/Schema;)Lorg/dmg/pmml/Model;
@@ -352,15 +352,15 @@
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: invokevirtual #26                 // Method encodeModel:(Lorg/jpmml/converter/Schema;)Lorg/dmg/pmml/mining/MiningModel;
          5: areturn
       LineNumberTable:
-        line 42: 0
+        line 37: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lsklearn/ensemble/stacking/StackingClassifier;
 }
 Signature: #82                          // Lsklearn/Classifier;Lsklearn/HasEstimatorEnsemble<Lsklearn/Classifier;>;
 SourceFile: "StackingClassifier.java"
 InnerClasses:
```

#### sklearn/ensemble/stacking/StackingUtil.class

##### procyon -ec {}

```diff
@@ -27,15 +27,22 @@
         final Label label = schema.getLabel();
         final List<? extends Feature> features = schema.getFeatures();
         final List<Feature> stackFeatures = new ArrayList<Feature>();
         final List<Model> models = new ArrayList<Model>();
         for (int i = 0; i < estimators.size(); ++i) {
             final E estimator = (E)estimators.get(i);
             final String stackMethod = (String)stackMethods.get(i);
-            final Model model = estimator.encode(schema);
+            estimator.setPMMLSegmentId((Object)Integer.valueOf(i + 1));
+            Model model;
+            try {
+                model = estimator.encode(schema);
+            }
+            finally {
+                estimator.setPMMLSegmentId((Object)null);
+            }
             final List<Feature> predictFeatures = predictFunction.apply(i, model, stackMethod, encoder);
             if (predictFeatures != null && !predictFeatures.isEmpty()) {
                 stackFeatures.addAll(predictFeatures);
             }
             models.add(model);
         }
         if (passthrough) {
```

#### sklearn/ensemble/stacking/StackingClassifier$1.class

##### procyon -ec {}

```diff
@@ -1,45 +1,32 @@
 
 package sklearn.ensemble.stacking;
 
-import org.dmg.pmml.ResultFeature;
 import java.util.Iterator;
-import org.dmg.pmml.OutputField;
-import org.dmg.pmml.Output;
 import org.jpmml.converter.FieldNameUtil;
 import java.util.ArrayList;
-import java.util.function.Predicate;
-import org.jpmml.converter.mining.MiningModelUtil;
 import org.jpmml.converter.Feature;
 import org.jpmml.sklearn.SkLearnEncoder;
 import org.dmg.pmml.Model;
 import java.util.List;
 
 class StackingClassifier$1 implements StackingUtil.PredictFunction {
-    private static final String PREFIX_PROBABILITY = "probability(";
-    
     public List<Feature> apply(final int index, final Model model, final String stackMethod, final SkLearnEncoder encoder) {
         int n = -1;
         switch (stackMethod.hashCode()) {
             case -1907484474: {
                 if (stackMethod.equals("predict_proba")) {
                     n = 0;
                     break;
                 }
                 break;
             }
         }
         switch (n) {
             case 0: {
-                final Model finalModel = MiningModelUtil.getFinalModel(model);
-                final Output output = finalModel.getOutput();
-                if (output != null && output.hasOutputFields()) {
-                    final List<OutputField> outputFields = output.getOutputFields();
-                    outputFields.stream().filter((Predicate<? super Object>)StackingClassifier$1::lambda$apply$0).forEach(StackingClassifier$1::lambda$apply$1);
-                }
                 final List<Feature> result = new ArrayList<Feature>();
                 for (final Object value : this.val$values) {
                     final Feature feature = encoder.exportProbability(model, FieldNameUtil.create(stackMethod, new Object[] { Integer.valueOf(index), value }), value);
                     result.add(feature);
                 }
                 return result;
             }
```

#### sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$GradientBoostingClassifierProxy.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum d719b9ae16871896eaeb6f6162f0134c412c69eee2814097b71273bd7a6ec4d0
+  SHA-256 checksum cea38d7ba92acf97062fcd652465fdb9641a552709c667da661ddc3f24f53653
   Compiled from "GradientBoostingClassifier.java"
 abstract class sklearn.ensemble.gradient_boosting.GradientBoostingClassifier$GradientBoostingClassifierProxy extends sklearn2pmml.EstimatorProxy implements sklearn.HasEstimatorEnsemble<sklearn.tree.TreeRegressor>, sklearn.tree.HasTreeOptions
   minor version: 0
   major version: 52
   flags: (0x0420) ACC_SUPER, ACC_ABSTRACT
   this_class: #4                          // sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$GradientBoostingClassifierProxy
   super_class: #5                         // sklearn2pmml/EstimatorProxy
@@ -61,44 +61,44 @@
          0: aload_0
          1: aload_1
          2: putfield      #2                  // Field this$0:Lsklearn/ensemble/gradient_boosting/GradientBoostingClassifier;
          5: aload_0
          6: invokespecial #3                  // Method sklearn2pmml/EstimatorProxy."<init>":()V
          9: return
       LineNumberTable:
-        line 157: 0
+        line 164: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lsklearn/ensemble/gradient_boosting/GradientBoostingClassifier$GradientBoostingClassifierProxy;
 
   public sklearn.Estimator getEstimator();
     descriptor: ()Lsklearn/Estimator;
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #2                  // Field this$0:Lsklearn/ensemble/gradient_boosting/GradientBoostingClassifier;
          4: areturn
       LineNumberTable:
-        line 161: 0
+        line 168: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lsklearn/ensemble/gradient_boosting/GradientBoostingClassifier$GradientBoostingClassifierProxy;
 
   sklearn.ensemble.gradient_boosting.GradientBoostingClassifier$GradientBoostingClassifierProxy(sklearn.ensemble.gradient_boosting.GradientBoostingClassifier, sklearn.ensemble.gradient_boosting.GradientBoostingClassifier$1);
     descriptor: (Lsklearn/ensemble/gradient_boosting/GradientBoostingClassifier;Lsklearn/ensemble/gradient_boosting/GradientBoostingClassifier$1;)V
     flags: (0x1000) ACC_SYNTHETIC
     Code:
       stack=2, locals=3, args_size=3
          0: aload_0
          1: aload_1
          2: invokespecial #1                  // Method "<init>":(Lsklearn/ensemble/gradient_boosting/GradientBoostingClassifier;)V
          5: return
       LineNumberTable:
-        line 157: 0
+        line 164: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lsklearn/ensemble/gradient_boosting/GradientBoostingClassifier$GradientBoostingClassifierProxy;
             0       6     1    x0   Lsklearn/ensemble/gradient_boosting/GradientBoostingClassifier;
             0       6     2    x1   Lsklearn/ensemble/gradient_boosting/GradientBoostingClassifier$1;
 }
 Signature: #27                          // Lsklearn2pmml/EstimatorProxy;Lsklearn/HasEstimatorEnsemble<Lsklearn/tree/TreeRegressor;>;Lsklearn/tree/HasTreeOptions;
```

#### sklearn/ensemble/gradient_boosting/GradientBoostingClassifier.class

##### procyon -ec {}

```diff
@@ -1,16 +1,16 @@
 
 package sklearn.ensemble.gradient_boosting;
 
 import java.util.function.IntFunction;
 import sklearn.HasPriorProbability;
 import java.util.List;
 import org.jpmml.converter.CMatrixUtil;
-import java.util.ArrayList;
 import org.dmg.pmml.Model;
+import java.util.ArrayList;
 import org.jpmml.converter.mining.MiningModelUtil;
 import org.dmg.pmml.regression.RegressionModel;
 import org.jpmml.converter.ModelUtil;
 import org.jpmml.converter.Transformation;
 import org.dmg.pmml.OpType;
 import org.jpmml.converter.FieldNameUtil;
 import sklearn.Estimator;
@@ -51,36 +51,41 @@
         IntFunction<Number> initialPredictions = init::getPriorProbability;
         if (sklearnVersion != null && SkLearnUtil.compareVersion(sklearnVersion, "0.21") >= 0) {
             final List<? extends Number> computedInitialPredictions = loss.computeInitialPredictions(init);
             initialPredictions = computedInitialPredictions::get;
         }
         final Schema segmentSchema = schema.toAnonymousRegressorSchema(DataType.DOUBLE);
         final CategoricalLabel categoricalLabel = (CategoricalLabel)schema.getLabel();
+        MiningModel miningModel;
         if (numberOfClasses == 1) {
             SchemaUtil.checkSize(2, categoricalLabel);
-            final MiningModel miningModel = GradientBoostingUtil.encodeGradientBoosting((Estimator)this, (Number)initialPredictions.apply(1), learningRate, segmentSchema).setOutput(ModelUtil.createPredictedOutput(FieldNameUtil.create("decisionFunction", new Object[] { categoricalLabel.getValue(1) }), OpType.CONTINUOUS, DataType.DOUBLE, new Transformation[] { loss.createTransformation() }));
-            return MiningModelUtil.createBinaryLogisticClassification((Model)miningModel, 1.0, 0.0, RegressionModel.NormalizationMethod.NONE, true, schema);
+            final Model model = (Model)GradientBoostingUtil.encodeGradientBoosting((Estimator)this, (Number)initialPredictions.apply(1), learningRate, segmentSchema).setOutput(ModelUtil.createPredictedOutput(FieldNameUtil.create("decisionFunction", new Object[] { categoricalLabel.getValue(1) }), OpType.CONTINUOUS, DataType.DOUBLE, new Transformation[] { loss.createTransformation() }));
+            miningModel = MiningModelUtil.createBinaryLogisticClassification(model, 1.0, 0.0, RegressionModel.NormalizationMethod.NONE, false, schema);
         }
-        if (numberOfClasses >= 3) {
+        else {
+            if (numberOfClasses < 3) {
+                throw new IllegalArgumentException();
+            }
             SchemaUtil.checkSize(numberOfClasses, categoricalLabel);
             final List<? extends TreeRegressor> estimators = this.getEstimators();
-            final List<MiningModel> miningModels = new ArrayList<MiningModel>();
+            final List<Model> models = new ArrayList<Model>();
             int i = 0;
             final int columns = categoricalLabel.size();
             final int rows = estimators.size() / columns;
             while (i < columns) {
                 final List<? extends TreeRegressor> columnEstimators = CMatrixUtil.getColumn((List)estimators, rows, columns, i);
                 final GradientBoostingClassifier.GradientBoostingClassifierProxy estimatorProxy = (GradientBoostingClassifier.GradientBoostingClassifierProxy)new GradientBoostingClassifier.GradientBoostingClassifier$1(this, (List)columnEstimators);
-                final MiningModel miningModel2 = GradientBoostingUtil.encodeGradientBoosting((Estimator)estimatorProxy, (Number)initialPredictions.apply(i), learningRate, segmentSchema).setOutput(ModelUtil.createPredictedOutput(FieldNameUtil.create("decisionFunction", new Object[] { categoricalLabel.getValue(i) }), OpType.CONTINUOUS, DataType.DOUBLE, new Transformation[] { loss.createTransformation() }));
-                miningModels.add(miningModel2);
+                final Model model2 = (Model)GradientBoostingUtil.encodeGradientBoosting((Estimator)estimatorProxy, (Number)initialPredictions.apply(i), learningRate, segmentSchema).setOutput(ModelUtil.createPredictedOutput(FieldNameUtil.create("decisionFunction", new Object[] { categoricalLabel.getValue(i) }), OpType.CONTINUOUS, DataType.DOUBLE, new Transformation[] { loss.createTransformation() }));
+                models.add(model2);
                 ++i;
             }
-            return MiningModelUtil.createClassification((List)miningModels, RegressionModel.NormalizationMethod.SIMPLEMAX, true, schema);
+            miningModel = MiningModelUtil.createClassification((List)models, RegressionModel.NormalizationMethod.SIMPLEMAX, false, schema);
         }
-        throw new IllegalArgumentException();
+        this.encodePredictProbaOutput((Model)miningModel, DataType.DOUBLE, categoricalLabel);
+        return miningModel;
     }
     
     public LossFunction getLoss() {
         if (this.containsKey((Object)"loss_")) {
             return (LossFunction)this.get("loss_", (Class)LossFunction.class);
         }
         return (LossFunction)this.get("_loss", (Class)LossFunction.class);
```

#### sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum e9513209386f68f43d2171b53ac1d9540bd2d8ff1dd609b4819f1942c8139ebe
+  SHA-256 checksum 1b70aa8cd40a5e132fd824952e2185f4d3c984aaf4b856479e513a2afbaabb3a
   Compiled from "GradientBoostingClassifier.java"
 class sklearn.ensemble.gradient_boosting.GradientBoostingClassifier$1 extends sklearn.ensemble.gradient_boosting.GradientBoostingClassifier$GradientBoostingClassifierProxy
   minor version: 0
   major version: 52
   flags: (0x0020) ACC_SUPER
   this_class: #4                          // sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$1
   super_class: #5                         // sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$GradientBoostingClassifierProxy
@@ -66,30 +66,30 @@
          7: putfield      #2                  // Field val$columnEstimators:Ljava/util/List;
         10: aload_0
         11: aload_1
         12: aconst_null
         13: invokespecial #3                  // Method sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$GradientBoostingClassifierProxy."<init>":(Lsklearn/ensemble/gradient_boosting/GradientBoostingClassifier;Lsklearn/ensemble/gradient_boosting/GradientBoostingClassifier$1;)V
         16: return
       LineNumberTable:
-        line 110: 0
+        line 113: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      17     0  this   Lsklearn/ensemble/gradient_boosting/GradientBoostingClassifier$1;
             0      17     1 this$0   Lsklearn/ensemble/gradient_boosting/GradientBoostingClassifier;
 
   public java.util.List<? extends sklearn.tree.TreeRegressor> getEstimators();
     descriptor: ()Ljava/util/List;
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #2                  // Field val$columnEstimators:Ljava/util/List;
          4: areturn
       LineNumberTable:
-        line 114: 0
+        line 117: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lsklearn/ensemble/gradient_boosting/GradientBoostingClassifier$1;
     Signature: #21                          // ()Ljava/util/List<+Lsklearn/tree/TreeRegressor;>;
 }
 SourceFile: "GradientBoostingClassifier.java"
 EnclosingMethod: #25.#26                // sklearn.ensemble.gradient_boosting.GradientBoostingClassifier.encodeModel
```

#### sklearn/ensemble/forest/ForestRegressor.class

##### procyon -ec {}

```diff
@@ -3,15 +3,14 @@
 
 import org.dmg.pmml.Model;
 import java.util.List;
 import org.dmg.pmml.MiningFunction;
 import org.dmg.pmml.mining.Segmentation;
 import org.dmg.pmml.mining.MiningModel;
 import org.jpmml.converter.Schema;
-import org.jpmml.converter.FieldNameUtil;
 import sklearn.Estimator;
 import org.dmg.pmml.DataType;
 import sklearn.tree.HasTreeOptions;
 import sklearn.HasMultiApplyField;
 import sklearn.tree.TreeRegressor;
 import sklearn.HasEstimatorEnsemble;
 import sklearn.Regressor;
@@ -26,16 +25,16 @@
         return DataType.FLOAT;
     }
     
     public int getNumberOfApplyFields() {
         return ForestUtil.getNumberOfEstimators((Estimator)this);
     }
     
-    public String getApplyField(final int index) {
-        return FieldNameUtil.create("nodeId", new Object[] { Integer.valueOf(index + 1) });
+    public String getApplyField() {
+        return "nodeId";
     }
     
     public MiningModel encodeModel(final Schema schema) {
         return ForestUtil.encodeBaseForest((Estimator)this, Segmentation.MultipleModelMethod.AVERAGE, MiningFunction.REGRESSION, schema);
     }
     
     public List<? extends TreeRegressor> getEstimators() {
```

#### sklearn/ensemble/forest/ForestClassifier.class

##### procyon -ec {}

```diff
@@ -1,19 +1,17 @@
 
 package sklearn.ensemble.forest;
 
-import org.dmg.pmml.Model;
 import java.util.List;
-import org.jpmml.converter.ModelUtil;
-import org.jpmml.converter.CategoricalLabel;
+import org.dmg.pmml.Model;
 import org.dmg.pmml.MiningFunction;
 import org.dmg.pmml.mining.Segmentation;
+import org.jpmml.converter.CategoricalLabel;
 import org.dmg.pmml.mining.MiningModel;
 import org.jpmml.converter.Schema;
-import org.jpmml.converter.FieldNameUtil;
 import sklearn.Estimator;
 import org.dmg.pmml.DataType;
 import sklearn.tree.HasTreeOptions;
 import sklearn.HasMultiApplyField;
 import sklearn.tree.TreeClassifier;
 import sklearn.HasEstimatorEnsemble;
 import sklearn.Classifier;
@@ -28,20 +26,22 @@
         return DataType.FLOAT;
     }
     
     public int getNumberOfApplyFields() {
         return ForestUtil.getNumberOfEstimators((Estimator)this);
     }
     
-    public String getApplyField(final int index) {
-        return FieldNameUtil.create("nodeId", new Object[] { Integer.valueOf(index + 1) });
+    public String getApplyField() {
+        return "nodeId";
     }
     
     public MiningModel encodeModel(final Schema schema) {
-        final MiningModel miningModel = ForestUtil.encodeBaseForest((Estimator)this, Segmentation.MultipleModelMethod.AVERAGE, MiningFunction.CLASSIFICATION, schema).setOutput(ModelUtil.createProbabilityOutput(DataType.DOUBLE, (CategoricalLabel)schema.getLabel()));
+        final CategoricalLabel categoricalLabel = (CategoricalLabel)schema.getLabel();
+        final MiningModel miningModel = ForestUtil.encodeBaseForest((Estimator)this, Segmentation.MultipleModelMethod.AVERAGE, MiningFunction.CLASSIFICATION, schema);
+        this.encodePredictProbaOutput((Model)miningModel, DataType.DOUBLE, categoricalLabel);
         return miningModel;
     }
     
     public List<? extends TreeClassifier> getEstimators() {
         return this.getList("estimators_", (Class)TreeClassifier.class);
     }
 }
```

#### sklearn/ensemble/iforest/IsolationForest$3.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 85a9fbd8ab137d7163e8ac1a43f19d4b5d6777cd8b8743bc3aa1ea3953faaf6c
+  SHA-256 checksum f910951941a382c5b16ae325f86c2815de76d82e5b76c48688b6e6ddbc744961
   Compiled from "IsolationForest.java"
 class sklearn.ensemble.iforest.IsolationForest$3 extends org.jpmml.converter.transformations.AbstractTransformation
   minor version: 0
   major version: 52
   flags: (0x0020) ACC_SUPER
   this_class: #18                         // sklearn/ensemble/iforest/IsolationForest$3
   super_class: #19                        // org/jpmml/converter/transformations/AbstractTransformation
@@ -102,15 +102,15 @@
          0: aload_0
          1: aload_1
          2: putfield      #1                  // Field this$0:Lsklearn/ensemble/iforest/IsolationForest;
          5: aload_0
          6: invokespecial #2                  // Method org/jpmml/converter/transformations/AbstractTransformation."<init>":()V
          9: return
       LineNumberTable:
-        line 166: 0
+        line 163: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lsklearn/ensemble/iforest/IsolationForest$3;
             0      10     1 this$0   Lsklearn/ensemble/iforest/IsolationForest;
 
   public java.lang.String getName(java.lang.String);
     descriptor: (Ljava/lang/String;)Ljava/lang/String;
@@ -118,29 +118,29 @@
     Code:
       stack=1, locals=2, args_size=2
          0: aload_0
          1: getfield      #1                  // Field this$0:Lsklearn/ensemble/iforest/IsolationForest;
          4: invokevirtual #3                  // Method sklearn/ensemble/iforest/IsolationForest.getDecisionFunctionField:()Ljava/lang/String;
          7: areturn
       LineNumberTable:
-        line 170: 0
+        line 167: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       8     0  this   Lsklearn/ensemble/iforest/IsolationForest$3;
             0       8     1  name   Ljava/lang/String;
 
   public boolean isFinalResult();
     descriptor: ()Z
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: iconst_1
          1: ireturn
       LineNumberTable:
-        line 175: 0
+        line 172: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       2     0  this   Lsklearn/ensemble/iforest/IsolationForest$3;
 
   public org.dmg.pmml.Expression createExpression(org.dmg.pmml.FieldRef);
     descriptor: (Lorg/dmg/pmml/FieldRef;)Lorg/dmg/pmml/Expression;
     flags: (0x0001) ACC_PUBLIC
@@ -190,16 +190,16 @@
         72: invokestatic  #17                 // Method org/jpmml/converter/PMMLUtil.createApply:(Ljava/lang/String;[Lorg/dmg/pmml/Expression;)Lorg/dmg/pmml/Apply;
         75: aastore
         76: invokestatic  #17                 // Method org/jpmml/converter/PMMLUtil.createApply:(Ljava/lang/String;[Lorg/dmg/pmml/Expression;)Lorg/dmg/pmml/Apply;
         79: aastore
         80: invokestatic  #17                 // Method org/jpmml/converter/PMMLUtil.createApply:(Ljava/lang/String;[Lorg/dmg/pmml/Expression;)Lorg/dmg/pmml/Apply;
         83: areturn
       LineNumberTable:
-        line 180: 0
-        line 182: 8
+        line 177: 0
+        line 179: 8
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      84     0  this   Lsklearn/ensemble/iforest/IsolationForest$3;
             0      84     1 fieldRef   Lorg/dmg/pmml/FieldRef;
             8      76     2 offset   Ljava/lang/Number;
 }
 SourceFile: "IsolationForest.java"
```

#### sklearn/ensemble/iforest/IsolationForest$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 28b27dec6f49ec869d9ebe26f56c84425ed43475d8a1a8ad5f8445a0ae710283
+  SHA-256 checksum d7cf65bf37f9b925e92f6be5ffd259fd44a6e727a765f22b447bf5b1128fe489
   Compiled from "IsolationForest.java"
 class sklearn.ensemble.iforest.IsolationForest$1 extends org.jpmml.model.visitors.AbstractVisitor
   minor version: 0
   major version: 52
   flags: (0x0020) ACC_SUPER
   this_class: #23                         // sklearn/ensemble/iforest/IsolationForest$1
   super_class: #24                        // org/jpmml/model/visitors/AbstractVisitor
@@ -175,16 +175,16 @@
         25: aload_0
         26: aload_0
         27: getfield      #2                  // Field val$tree:Lsklearn/tree/Tree;
         30: invokevirtual #6                  // Method sklearn/tree/Tree.getNodeSamples:()[I
         33: putfield      #7                  // Field nodeSamples:[I
         36: return
       LineNumberTable:
-        line 109: 0
-        line 111: 25
+        line 106: 0
+        line 108: 25
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      37     0  this   Lsklearn/ensemble/iforest/IsolationForest$1;
             0      37     1 this$0   Lsklearn/ensemble/iforest/IsolationForest;
 
   public org.dmg.pmml.VisitorAction visit(org.dmg.pmml.tree.Node);
     descriptor: (Lorg/dmg/pmml/tree/Node;)Lorg/dmg/pmml/VisitorAction;
@@ -246,26 +246,26 @@
        116: invokevirtual #21                 // Method org/dmg/pmml/tree/Node.setScore:(Ljava/lang/Object;)Lorg/dmg/pmml/tree/Node;
        119: pop
        120: aload_0
        121: aload_1
        122: invokespecial #22                 // Method org/jpmml/model/visitors/AbstractVisitor.visit:(Lorg/dmg/pmml/tree/Node;)Lorg/dmg/pmml/VisitorAction;
        125: areturn
       LineNumberTable:
-        line 117: 0
-        line 118: 7
-        line 120: 9
-        line 121: 15
-        line 123: 46
-        line 124: 54
-        line 127: 57
-        line 128: 61
-        line 130: 64
-        line 132: 82
-        line 134: 108
-        line 137: 120
+        line 114: 0
+        line 115: 7
+        line 117: 9
+        line 118: 15
+        line 120: 46
+        line 121: 54
+        line 124: 57
+        line 125: 61
+        line 127: 64
+        line 129: 82
+        line 131: 108
+        line 134: 120
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            46      15     6 parent   Lorg/dmg/pmml/PMMLObject;
             9     111     2 nodeDepth   D
            15     105     4 parents   Ljava/util/Deque;
            82      38     5 nodeSample   D
           108      12     7 averagePathLength   D
```

#### sklearn/ensemble/iforest/IsolationForest$2.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum bcb43e62e681027ac4640b316f394e4232572542b37a2410321bf26b0c8345fd
+  SHA-256 checksum f9b628588ece0aa30fea4df3177b1182efef9401b1f926367e7b73cf6da6555b
   Compiled from "IsolationForest.java"
 class sklearn.ensemble.iforest.IsolationForest$2 extends org.jpmml.converter.transformations.AbstractTransformation
   minor version: 0
   major version: 52
   flags: (0x0020) ACC_SUPER
   this_class: #15                         // sklearn/ensemble/iforest/IsolationForest$2
   super_class: #16                        // org/jpmml/converter/transformations/AbstractTransformation
@@ -117,29 +117,29 @@
         10: aload_0
         11: iload_3
         12: putfield      #3                  // Field val$nodeSampleCorrected:Z
         15: aload_0
         16: invokespecial #4                  // Method org/jpmml/converter/transformations/AbstractTransformation."<init>":()V
         19: return
       LineNumberTable:
-        line 148: 0
+        line 145: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      20     0  this   Lsklearn/ensemble/iforest/IsolationForest$2;
             0      20     1 this$0   Lsklearn/ensemble/iforest/IsolationForest;
 
   public java.lang.String getName(java.lang.String);
     descriptor: (Ljava/lang/String;)Ljava/lang/String;
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=2, args_size=2
          0: ldc           #5                  // String normalizedAnomalyScore
          2: areturn
       LineNumberTable:
-        line 152: 0
+        line 149: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       3     0  this   Lsklearn/ensemble/iforest/IsolationForest$2;
             0       3     1  name   Ljava/lang/String;
 
   public org.dmg.pmml.Expression createExpression(org.dmg.pmml.FieldRef);
     descriptor: (Lorg/dmg/pmml/FieldRef;)Lorg/dmg/pmml/Expression;
@@ -174,17 +174,17 @@
         45: dload         4
         47: invokestatic  #12                 // Method java/lang/Double.valueOf:(D)Ljava/lang/Double;
         50: invokestatic  #13                 // Method org/jpmml/converter/PMMLUtil.createConstant:(Ljava/lang/Number;)Lorg/dmg/pmml/Constant;
         53: aastore
         54: invokestatic  #14                 // Method org/jpmml/converter/PMMLUtil.createApply:(Ljava/lang/String;[Lorg/dmg/pmml/Expression;)Lorg/dmg/pmml/Apply;
         57: areturn
       LineNumberTable:
-        line 157: 0
-        line 159: 9
-        line 161: 33
+        line 154: 0
+        line 156: 9
+        line 158: 33
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      58     0  this   Lsklearn/ensemble/iforest/IsolationForest$2;
             0      58     1 fieldRef   Lorg/dmg/pmml/FieldRef;
             9      49     2 maxSamples   D
            33      25     4 averagePathLength   D
       StackMapTable: number_of_entries = 2
```

#### sklearn/ensemble/iforest/IsolationForest.class

##### procyon -ec {}

```diff
@@ -1,23 +1,20 @@
 
 package sklearn.ensemble.iforest;
 
 import sklearn.ensemble.EnsembleUtil;
 import org.jpmml.python.HasArray;
-import org.dmg.pmml.Output;
 import org.dmg.pmml.Visitor;
 import sklearn.tree.Tree;
 import org.dmg.pmml.Model;
+import sklearn.OutlierDetectorUtil;
+import org.jpmml.converter.Transformation;
 import org.jpmml.converter.mining.MiningModelUtil;
 import org.dmg.pmml.mining.Segmentation;
 import org.jpmml.converter.ModelUtil;
-import org.jpmml.converter.Transformation;
-import org.dmg.pmml.DataType;
-import org.dmg.pmml.OpType;
-import sklearn.SkLearnOutlierTransformation;
 import net.razorvine.pickle.objects.ClassDict;
 import org.jpmml.python.ClassDictUtil;
 import org.dmg.pmml.Visitable;
 import sklearn.Estimator;
 import sklearn.tree.TreeUtil;
 import org.dmg.pmml.MiningFunction;
 import sklearn.tree.TreeRegressor;
@@ -28,19 +25,20 @@
 import org.dmg.pmml.tree.TreeModel;
 import java.util.ArrayList;
 import org.jpmml.converter.ScoreDistributionManager;
 import org.jpmml.converter.PredicateManager;
 import sklearn.SkLearnUtil;
 import org.dmg.pmml.mining.MiningModel;
 import org.jpmml.converter.Schema;
+import sklearn.OutlierDetector;
 import sklearn.tree.HasTreeOptions;
 import sklearn.HasDecisionFunctionField;
 import sklearn.ensemble.EnsembleRegressor;
 
-public class IsolationForest extends EnsembleRegressor implements HasDecisionFunctionField, HasTreeOptions
+public class IsolationForest extends EnsembleRegressor implements HasDecisionFunctionField, HasTreeOptions, OutlierDetector
 {
     public IsolationForest(final String module, final String name) {
         super(module, name);
     }
     
     public boolean isSupervised() {
         return false;
@@ -67,21 +65,36 @@
             final Visitor visitor = (Visitor)new IsolationForest.IsolationForest$1(this, tree, corrected, nodeSampleCorrected);
             visitor.applyTo((Visitable)treeModel);
             ClassDictUtil.clearContent((ClassDict)tree);
             treeModels.add(treeModel);
         }
         final Transformation normalizedAnomalyScore = (Transformation)new IsolationForest.IsolationForest$2(this, corrected, nodeSampleCorrected);
         final Transformation decisionFunction = (Transformation)new IsolationForest.IsolationForest$3(this);
-        final Transformation outlier = (Transformation)new IsolationForest.IsolationForest$4(this);
-        final Transformation sklearnOutlier = (Transformation)new SkLearnOutlierTransformation();
-        final Output output = ModelUtil.createPredictedOutput("rawAnomalyScore", OpType.CONTINUOUS, DataType.DOUBLE, new Transformation[] { normalizedAnomalyScore, decisionFunction, outlier, sklearnOutlier });
-        final MiningModel miningModel = new MiningModel(MiningFunction.REGRESSION, ModelUtil.createMiningSchema(schema.getLabel())).setSegmentation(MiningModelUtil.createSegmentation(Segmentation.MultipleModelMethod.AVERAGE, Segmentation.MissingPredictionTreatment.RETURN_MISSING, (List)treeModels)).setOutput(output);
+        final MiningModel miningModel = new MiningModel(MiningFunction.REGRESSION, ModelUtil.createMiningSchema(schema.getLabel())).setSegmentation(MiningModelUtil.createSegmentation(Segmentation.MultipleModelMethod.AVERAGE, Segmentation.MissingPredictionTreatment.RETURN_MISSING, (List)treeModels)).setOutput(OutlierDetectorUtil.createPredictedOutput((Estimator)this, "rawAnomalyScore", new Transformation[] { normalizedAnomalyScore, decisionFunction }));
         return (MiningModel)TreeUtil.transform((Estimator)this, (Model)miningModel);
     }
     
+    public Number getDecisionFunctionThreshold() {
+        final String behaviour = this.getBehaviour();
+        Number threshold;
+        if (behaviour == null) {
+            threshold = this.getThreshold();
+        }
+        else if ("old".equals(behaviour)) {
+            threshold = this.getThreshold();
+        }
+        else {
+            if (!"new".equals(behaviour) && !"deprecated".equals(behaviour)) {
+                throw new IllegalArgumentException(behaviour);
+            }
+            threshold = Double.valueOf(0.0);
+        }
+        return threshold;
+    }
+    
     public List<List<Integer>> getEstimatorsFeatures() {
         return EnsembleUtil.transformEstimatorsFeatures(this.getList("estimators_features_", (Class)HasArray.class));
     }
     
     public String getBehaviour() {
         return this.getOptionalString("behaviour");
     }
```

#### sklearn/ensemble/voting/VotingClassifier.class

##### procyon -ec {}

```diff
@@ -1,21 +1,21 @@
 
 package sklearn.ensemble.voting;
 
 import java.util.Iterator;
 import org.dmg.pmml.DataType;
 import org.jpmml.converter.mining.MiningModelUtil;
 import org.dmg.pmml.mining.Segmentation;
-import org.dmg.pmml.mining.MiningModel;
 import org.jpmml.converter.Label;
 import org.jpmml.converter.ModelUtil;
 import org.dmg.pmml.MiningFunction;
+import org.dmg.pmml.Model;
 import java.util.ArrayList;
 import org.jpmml.converter.CategoricalLabel;
-import org.dmg.pmml.Model;
+import org.dmg.pmml.mining.MiningModel;
 import org.jpmml.converter.Schema;
 import java.util.List;
 import sklearn.StepUtil;
 import sklearn.HasEstimatorEnsemble;
 import sklearn.Classifier;
 
 public class VotingClassifier extends Classifier implements HasEstimatorEnsemble<Classifier>
@@ -25,27 +25,28 @@
     }
     
     public int getNumberOfFeatures() {
         final List<? extends Classifier> estimators = this.getEstimators();
         return StepUtil.getNumberOfFeatures((List)estimators);
     }
     
-    public Model encodeModel(final Schema schema) {
+    public MiningModel encodeModel(final Schema schema) {
         final List<? extends Classifier> estimators = this.getEstimators();
         final List<? extends Number> weights = this.getWeights();
         final CategoricalLabel categoricalLabel = (CategoricalLabel)schema.getLabel();
         final List<Model> models = new ArrayList<Model>();
         for (final Classifier estimator : estimators) {
             final Model model = estimator.encode(schema);
             models.add(model);
         }
         final String voting = this.getVoting();
         final Segmentation.MultipleModelMethod multipleModelMethod = parseVoting(voting, weights != null && !weights.isEmpty());
-        final MiningModel miningModel = new MiningModel(MiningFunction.CLASSIFICATION, ModelUtil.createMiningSchema((Label)categoricalLabel)).setSegmentation(MiningModelUtil.createSegmentation(multipleModelMethod, Segmentation.MissingPredictionTreatment.RETURN_MISSING, (List)models, (List)weights)).setOutput(ModelUtil.createProbabilityOutput(DataType.DOUBLE, categoricalLabel));
-        return (Model)miningModel;
+        final MiningModel miningModel = new MiningModel(MiningFunction.CLASSIFICATION, ModelUtil.createMiningSchema((Label)categoricalLabel)).setSegmentation(MiningModelUtil.createSegmentation(multipleModelMethod, Segmentation.MissingPredictionTreatment.RETURN_MISSING, (List)models, (List)weights));
+        this.encodePredictProbaOutput((Model)miningModel, DataType.DOUBLE, categoricalLabel);
+        return miningModel;
     }
     
     public List<? extends Classifier> getEstimators() {
         return this.getList("estimators_", (Class)Classifier.class);
     }
     
     public String getVoting() {
```

#### sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingClassifier.class

##### procyon -ec {}

```diff
@@ -1,14 +1,14 @@
 
 package sklearn.ensemble.hist_gradient_boosting;
 
 import org.jpmml.python.PythonObject;
+import org.dmg.pmml.Model;
 import java.util.ArrayList;
 import sklearn.loss.HalfMultinomialLoss;
-import org.dmg.pmml.Model;
 import org.jpmml.converter.mining.MiningModelUtil;
 import org.dmg.pmml.regression.RegressionModel;
 import org.jpmml.converter.ModelUtil;
 import org.jpmml.converter.Transformation;
 import org.dmg.pmml.OpType;
 import org.jpmml.converter.FieldNameUtil;
 import java.util.List;
@@ -35,37 +35,40 @@
         final int numberOfTreesPerIteration = (int)this.getNumberOfTreesPerIteration();
         final List<List<TreePredictor>> predictors = this.getPredictors();
         if (!predictors.isEmpty()) {
             ClassDictUtil.checkSize(numberOfTreesPerIteration, new Collection[] { (Collection)predictors.get(0), baselinePredictions });
         }
         final Schema segmentSchema = schema.toAnonymousRegressorSchema(DataType.DOUBLE);
         final CategoricalLabel categoricalLabel = (CategoricalLabel)schema.getLabel();
+        MiningModel miningModel;
         if (numberOfTreesPerIteration == 1) {
             SchemaUtil.checkSize(2, categoricalLabel);
             if (!(loss instanceof BinaryCrossEntropy) && !(loss instanceof HalfBinomialLoss)) {
                 throw new IllegalArgumentException();
             }
-            final MiningModel miningModel = HistGradientBoostingUtil.encodeHistGradientBoosting((List)predictors, binMapper, (List)baselinePredictions, 0, segmentSchema).setOutput(ModelUtil.createPredictedOutput(FieldNameUtil.create("decisionFunction", new Object[] { categoricalLabel.getValue(1) }), OpType.CONTINUOUS, DataType.DOUBLE, new Transformation[0]));
-            return MiningModelUtil.createBinaryLogisticClassification((Model)miningModel, 1.0, 0.0, RegressionModel.NormalizationMethod.LOGIT, true, schema);
+            final Model model = (Model)HistGradientBoostingUtil.encodeHistGradientBoosting((List)predictors, binMapper, (List)baselinePredictions, 0, segmentSchema).setOutput(ModelUtil.createPredictedOutput(FieldNameUtil.create("decisionFunction", new Object[] { categoricalLabel.getValue(1) }), OpType.CONTINUOUS, DataType.DOUBLE, new Transformation[0]));
+            miningModel = MiningModelUtil.createBinaryLogisticClassification(model, 1.0, 0.0, RegressionModel.NormalizationMethod.LOGIT, false, schema);
         }
         else {
             if (numberOfTreesPerIteration < 3) {
                 throw new IllegalArgumentException();
             }
             SchemaUtil.checkSize(numberOfTreesPerIteration, categoricalLabel);
             if (!(loss instanceof CategoricalCrossEntropy) && !(loss instanceof HalfMultinomialLoss)) {
                 throw new IllegalArgumentException();
             }
-            final List<MiningModel> miningModels = new ArrayList<MiningModel>();
+            final List<Model> models = new ArrayList<Model>();
             for (int i = 0, columns = categoricalLabel.size(); i < columns; ++i) {
-                final MiningModel miningModel2 = HistGradientBoostingUtil.encodeHistGradientBoosting((List)predictors, binMapper, (List)baselinePredictions, i, segmentSchema).setOutput(ModelUtil.createPredictedOutput(FieldNameUtil.create("decisionFunction", new Object[] { categoricalLabel.getValue(i) }), OpType.CONTINUOUS, DataType.DOUBLE, new Transformation[0]));
-                miningModels.add(miningModel2);
+                final Model model2 = (Model)HistGradientBoostingUtil.encodeHistGradientBoosting((List)predictors, binMapper, (List)baselinePredictions, i, segmentSchema).setOutput(ModelUtil.createPredictedOutput(FieldNameUtil.create("decisionFunction", new Object[] { categoricalLabel.getValue(i) }), OpType.CONTINUOUS, DataType.DOUBLE, new Transformation[0]));
+                models.add(model2);
             }
-            return MiningModelUtil.createClassification((List)miningModels, RegressionModel.NormalizationMethod.SOFTMAX, true, schema);
+            miningModel = MiningModelUtil.createClassification((List)models, RegressionModel.NormalizationMethod.SOFTMAX, false, schema);
         }
+        this.encodePredictProbaOutput((Model)miningModel, DataType.DOUBLE, categoricalLabel);
+        return miningModel;
     }
     
     public List<? extends Number> getBaselinePrediction() {
         return this.getNumberArray("_baseline_prediction");
     }
     
     public BinMapper getBinMapper() {
```

#### sklearn/discriminant_analysis/LinearDiscriminantAnalysis.class

##### procyon -ec {}

```diff
@@ -1,20 +1,21 @@
 
 package sklearn.discriminant_analysis;
 
+import org.dmg.pmml.mining.MiningModel;
 import org.jpmml.converter.Feature;
 import org.jpmml.converter.mining.MiningModelUtil;
 import org.jpmml.converter.ModelUtil;
 import org.jpmml.converter.Transformation;
 import org.dmg.pmml.OpType;
 import org.jpmml.converter.FieldNameUtil;
 import org.jpmml.converter.regression.RegressionModelUtil;
+import org.dmg.pmml.regression.RegressionModel;
 import java.util.List;
 import org.jpmml.converter.CMatrixUtil;
-import org.dmg.pmml.regression.RegressionModel;
 import java.util.ArrayList;
 import org.dmg.pmml.DataType;
 import org.jpmml.converter.SchemaUtil;
 import sklearn.SkLearnUtil;
 import org.jpmml.converter.CategoricalLabel;
 import org.dmg.pmml.Model;
 import org.jpmml.converter.Schema;
@@ -52,17 +53,19 @@
         final boolean corrected = sklearnVersion != null && SkLearnUtil.compareVersion(sklearnVersion, "0.21") >= 0;
         if (!corrected) {
             return super.encodeModel(schema);
         }
         if (numberOfClasses >= 3) {
             SchemaUtil.checkSize(numberOfClasses, categoricalLabel);
             final Schema segmentSchema = schema.toAnonymousRegressorSchema(DataType.DOUBLE).toEmptySchema();
-            final List<RegressionModel> regressionModels = new ArrayList<RegressionModel>();
+            final List<Model> models = new ArrayList<Model>();
             for (int i = 0, rows = categoricalLabel.size(); i < rows; ++i) {
-                final RegressionModel regressionModel = RegressionModelUtil.createRegression((List)features, CMatrixUtil.getRow((List)coef, numberOfClasses, numberOfFeatures, i), (Number)intercept.get(i), RegressionModel.NormalizationMethod.NONE, segmentSchema).setOutput(ModelUtil.createPredictedOutput(FieldNameUtil.create("decisionFunction", new Object[] { categoricalLabel.getValue(i) }), OpType.CONTINUOUS, DataType.DOUBLE, new Transformation[0]));
-                regressionModels.add(regressionModel);
+                final Model model = (Model)RegressionModelUtil.createRegression((List)features, CMatrixUtil.getRow((List)coef, numberOfClasses, numberOfFeatures, i), (Number)intercept.get(i), RegressionModel.NormalizationMethod.NONE, segmentSchema).setOutput(ModelUtil.createPredictedOutput(FieldNameUtil.create("decisionFunction", new Object[] { categoricalLabel.getValue(i) }), OpType.CONTINUOUS, DataType.DOUBLE, new Transformation[0]));
+                models.add(model);
             }
-            return (Model)MiningModelUtil.createClassification((List)regressionModels, RegressionModel.NormalizationMethod.SOFTMAX, true, schema);
+            final MiningModel miningModel = MiningModelUtil.createClassification((List)models, RegressionModel.NormalizationMethod.SOFTMAX, false, schema);
+            this.encodePredictProbaOutput((Model)miningModel, DataType.DOUBLE, categoricalLabel);
+            return (Model)miningModel;
         }
         throw new IllegalArgumentException();
     }
 }
```

#### sklearn/EstimatorUtil$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 38ff2e99f6cc92c81af5b3fc5cda405f7494cdeb50e2516caff5c6ac7cd486c9
+  SHA-256 checksum bdc04e6457f0ce0f4e894b3b61270c992ddfabb01986f9c0fe504eaa4a310fc5
   Compiled from "EstimatorUtil.java"
 class sklearn.EstimatorUtil$1
   minor version: 0
   major version: 52
   flags: (0x1020) ACC_SUPER, ACC_SYNTHETIC
   this_class: #7                          // sklearn/EstimatorUtil$1
   super_class: #8                         // java/lang/Object
@@ -78,15 +78,15 @@
         38: astore_0
         39: return
       Exception table:
          from    to  target type
              9    20    23   Class java/lang/NoSuchFieldError
             24    35    38   Class java/lang/NoSuchFieldError
       LineNumberTable:
-        line 114: 0
+        line 115: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
       StackMapTable: number_of_entries = 4
         frame_type = 87 /* same_locals_1_stack_item */
           stack = [ class java/lang/NoSuchFieldError ]
         frame_type = 0 /* same */
         frame_type = 77 /* same_locals_1_stack_item */
```

#### sklearn/tree/TreeClassifier.class

##### procyon -ec {}

```diff
@@ -1,15 +1,14 @@
 
 package sklearn.tree;
 
 import org.dmg.pmml.Model;
-import org.jpmml.converter.ModelUtil;
-import org.jpmml.converter.CategoricalLabel;
 import sklearn.Estimator;
 import org.dmg.pmml.MiningFunction;
+import org.jpmml.converter.CategoricalLabel;
 import org.dmg.pmml.tree.TreeModel;
 import org.jpmml.converter.Schema;
 import org.dmg.pmml.DataType;
 import sklearn.HasApplyField;
 import sklearn.Classifier;
 
 public class TreeClassifier extends Classifier implements HasApplyField, HasTree, HasTreeOptions
@@ -23,15 +22,17 @@
     }
     
     public String getApplyField() {
         return "nodeId";
     }
     
     public TreeModel encodeModel(final Schema schema) {
-        final TreeModel treeModel = TreeUtil.encodeTreeModel((Estimator)this, MiningFunction.CLASSIFICATION, schema).setOutput(ModelUtil.createProbabilityOutput(DataType.DOUBLE, (CategoricalLabel)schema.getLabel()));
+        final CategoricalLabel categoricalLabel = (CategoricalLabel)schema.getLabel();
+        final TreeModel treeModel = TreeUtil.encodeTreeModel((Estimator)this, MiningFunction.CLASSIFICATION, schema);
+        this.encodePredictProbaOutput((Model)treeModel, DataType.DOUBLE, categoricalLabel);
         return (TreeModel)TreeUtil.transform((Estimator)this, (Model)treeModel);
     }
     
     public Tree getTree() {
         return (Tree)this.get("tree_", (Class)Tree.class);
     }
 }
```

#### sklearn/tree/TreeUtil$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 5be3be3bbfd4dd66687ea14361b453d3b509056c202a3fc9db562bf135ddb40d
+  SHA-256 checksum 8be5aebcb04997f46dae0611df7ecd7cc6ed555a4c0a52f100b83e7bf3963273
   Compiled from "TreeUtil.java"
 final class sklearn.tree.TreeUtil$1 extends org.jpmml.converter.visitors.AbstractExtender
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #27                         // sklearn/tree/TreeUtil$1
   super_class: #28                        // org/jpmml/converter/visitors/AbstractExtender
@@ -180,16 +180,16 @@
          6: aload_1
          7: invokespecial #2                  // Method org/jpmml/converter/visitors/AbstractExtender."<init>":(Ljava/lang/String;)V
         10: aload_0
         11: getstatic     #3                  // Field org/dmg/pmml/tree/SimplifyingNodeTransformer.INSTANCE:Lorg/dmg/pmml/tree/SimplifyingNodeTransformer;
         14: putfield      #4                  // Field nodeTransformer:Lorg/dmg/pmml/tree/NodeTransformer;
         17: return
       LineNumberTable:
-        line 135: 0
-        line 137: 10
+        line 133: 0
+        line 135: 10
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      18     0  this   Lsklearn/tree/TreeUtil$1;
             0      18     1    x0   Ljava/lang/String;
 
   public org.dmg.pmml.VisitorAction visit(org.dmg.pmml.tree.TreeModel);
     descriptor: (Lorg/dmg/pmml/tree/TreeModel;)Lorg/dmg/pmml/VisitorAction;
@@ -204,16 +204,16 @@
          9: invokevirtual #7                  // Method org/dmg/pmml/tree/TreeModel.setNode:(Lorg/dmg/pmml/tree/Node;)Lorg/dmg/pmml/tree/TreeModel;
         12: pop
         13: aload_0
         14: aload_1
         15: invokespecial #8                  // Method org/jpmml/converter/visitors/AbstractExtender.visit:(Lorg/dmg/pmml/tree/TreeModel;)Lorg/dmg/pmml/VisitorAction;
         18: areturn
       LineNumberTable:
-        line 142: 0
-        line 144: 13
+        line 140: 0
+        line 142: 13
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      19     0  this   Lsklearn/tree/TreeUtil$1;
             0      19     1 treeModel   Lorg/dmg/pmml/tree/TreeModel;
 
   public org.dmg.pmml.VisitorAction visit(org.dmg.pmml.tree.Node);
     descriptor: (Lorg/dmg/pmml/tree/Node;)Lorg/dmg/pmml/VisitorAction;
@@ -257,23 +257,23 @@
         74: invokestatic  #19                 // Method org/jpmml/converter/ValueUtil.asString:(Ljava/lang/Object;)Ljava/lang/String;
         77: invokevirtual #20                 // Method addExtension:(Lorg/dmg/pmml/PMMLObject;Ljava/lang/String;)V
         80: aload_0
         81: aload_1
         82: invokespecial #21                 // Method org/jpmml/converter/visitors/AbstractExtender.visit:(Lorg/dmg/pmml/tree/Node;)Lorg/dmg/pmml/VisitorAction;
         85: areturn
       LineNumberTable:
-        line 150: 0
-        line 151: 7
-        line 153: 12
-        line 154: 28
-        line 158: 50
-        line 159: 56
-        line 160: 60
-        line 162: 65
-        line 165: 80
+        line 148: 0
+        line 149: 7
+        line 151: 12
+        line 152: 28
+        line 156: 50
+        line 157: 56
+        line 158: 60
+        line 160: 65
+        line 163: 80
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            19      31     3 childIt   Ljava/util/ListIterator;
            12      38     2 children   Ljava/util/List;
             0      86     0  this   Lsklearn/tree/TreeUtil$1;
             0      86     1  node   Lorg/dmg/pmml/tree/Node;
            56      30     2 value   Ljava/lang/Object;
@@ -311,20 +311,20 @@
         20: getfield      #4                  // Field nodeTransformer:Lorg/dmg/pmml/tree/NodeTransformer;
         23: aload_1
         24: invokeinterface #22,  2           // InterfaceMethod org/dmg/pmml/tree/NodeTransformer.toComplexNode:(Lorg/dmg/pmml/tree/Node;)Lorg/dmg/pmml/tree/ComplexNode;
         29: areturn
         30: aload_1
         31: areturn
       LineNumberTable:
-        line 170: 0
-        line 171: 7
-        line 174: 9
-        line 175: 15
-        line 176: 19
-        line 179: 30
+        line 168: 0
+        line 169: 7
+        line 172: 9
+        line 173: 15
+        line 174: 19
+        line 177: 30
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      32     0  this   Lsklearn/tree/TreeUtil$1;
             0      32     1  node   Lorg/dmg/pmml/tree/Node;
            15      17     2 value   Ljava/lang/Object;
       StackMapTable: number_of_entries = 2
         frame_type = 9 /* same */
@@ -344,16 +344,16 @@
         10: astore_2
         11: aload_0
         12: getfield      #1                  // Field val$values:Ljava/util/Map;
         15: aload_2
         16: invokeinterface #26,  2           // InterfaceMethod java/util/Map.get:(Ljava/lang/Object;)Ljava/lang/Object;
         21: areturn
       LineNumberTable:
-        line 183: 0
-        line 185: 11
+        line 181: 0
+        line 183: 11
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      22     0  this   Lsklearn/tree/TreeUtil$1;
             0      22     1  node   Lorg/dmg/pmml/tree/Node;
            11      11     2    id   Ljava/lang/Integer;
 }
 SourceFile: "TreeUtil.java"
```

#### sklearn/tree/TreeUtil$4.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 1cdd287704d917dc619157cb5ba6cafd0f528aea8070e36e6d0ad1b770e08bf8
+  SHA-256 checksum cd16e1b1849a751f6299f74a84e91d674062260cbfde1e1e3fe7e46a099e1799
   Compiled from "TreeUtil.java"
 final class sklearn.tree.TreeUtil$4 extends java.lang.Object implements java.util.function.Function<T, org.dmg.pmml.tree.TreeModel>
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #16                         // sklearn/tree/TreeUtil$4
   super_class: #17                        // java/lang/Object
@@ -146,15 +146,15 @@
         21: aload_0
         22: aload         5
         24: putfield      #5                  // Field val$scoreDistributionManager:Lorg/jpmml/converter/ScoreDistributionManager;
         27: aload_0
         28: invokespecial #6                  // Method java/lang/Object."<init>":()V
         31: return
       LineNumberTable:
-        line 253: 0
+        line 251: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      32     0  this   Lsklearn/tree/TreeUtil$4;
 
   public org.dmg.pmml.tree.TreeModel apply(T);
     descriptor: (Lsklearn/Estimator;)Lorg/dmg/pmml/tree/TreeModel;
     flags: (0x0001) ACC_PUBLIC
@@ -193,20 +193,20 @@
         61: aload_1
         62: aload_3
         63: aload         4
         65: invokevirtual #13                 // Method sklearn/Estimator.addFeatureImportances:(Lorg/dmg/pmml/Model;Lorg/jpmml/converter/Schema;)V
         68: aload_3
         69: areturn
       LineNumberTable:
-        line 257: 0
-        line 259: 19
-        line 262: 41
-        line 263: 48
-        line 265: 61
-        line 268: 68
+        line 255: 0
+        line 257: 19
+        line 260: 41
+        line 261: 48
+        line 263: 61
+        line 266: 68
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            61       7     4 featureImportanceSchema   Lorg/jpmml/converter/Schema;
             0      70     0  this   Lsklearn/tree/TreeUtil$4;
             0      70     1 estimator   Lsklearn/Estimator;
            19      51     2 treeModelSchema   Lorg/jpmml/converter/Schema;
            41      29     3 treeModel   Lorg/dmg/pmml/tree/TreeModel;
@@ -226,15 +226,15 @@
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: checkcast     #14                 // class sklearn/Estimator
          5: invokevirtual #15                 // Method apply:(Lsklearn/Estimator;)Lorg/dmg/pmml/tree/TreeModel;
          8: areturn
       LineNumberTable:
-        line 253: 0
+        line 251: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       9     0  this   Lsklearn/tree/TreeUtil$4;
 }
 Signature: #53                          // Ljava/lang/Object;Ljava/util/function/Function<TT;Lorg/dmg/pmml/tree/TreeModel;>;
 SourceFile: "TreeUtil.java"
 EnclosingMethod: #57.#58                // sklearn.tree.TreeUtil.encodeTreeModelEnsemble
```

#### sklearn/tree/TreeUtil$8.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum ab2e84e9976376a54353cfdcdf6fa8650051b63706c5a27e4f29f5c658434bfc
+  SHA-256 checksum cfa7dc034091c0eb7b66d429c4088ad3c6b48286f104d9da5c848b78b5bc0be0
   Compiled from "TreeUtil.java"
 final class sklearn.tree.TreeUtil$8 extends java.lang.Object implements java.util.function.Function<org.jpmml.converter.Feature, org.jpmml.converter.Feature>
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #8                          // sklearn/tree/TreeUtil$8
   super_class: #9                         // java/lang/Object
@@ -76,15 +76,15 @@
          0: aload_0
          1: iload_1
          2: putfield      #1                  // Field val$numeric:Z
          5: aload_0
          6: invokespecial #2                  // Method java/lang/Object."<init>":()V
          9: return
       LineNumberTable:
-        line 551: 0
+        line 555: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lsklearn/tree/TreeUtil$8;
 
   public org.jpmml.converter.Feature apply(org.jpmml.converter.Feature);
     descriptor: (Lorg/jpmml/converter/Feature;)Lorg/jpmml/converter/Feature;
     flags: (0x0001) ACC_PUBLIC
@@ -111,22 +111,22 @@
         34: areturn
         35: aload_1
         36: invokestatic  #5                  // Method sklearn/tree/TreeUtil.access$200:(Lorg/jpmml/converter/Feature;)Lorg/jpmml/converter/ContinuousFeature;
         39: astore_2
         40: aload_2
         41: areturn
       LineNumberTable:
-        line 556: 0
-        line 557: 7
-        line 559: 12
-        line 562: 14
-        line 563: 28
-        line 565: 33
-        line 569: 35
-        line 571: 40
+        line 560: 0
+        line 561: 7
+        line 563: 12
+        line 566: 14
+        line 567: 28
+        line 569: 33
+        line 573: 35
+        line 575: 40
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            12       2     2 binaryFeature   Lorg/jpmml/converter/BinaryFeature;
            33       2     2 thresholdFeature   Lorg/jpmml/converter/ThresholdFeature;
            40       2     2 continuousFeature   Lorg/jpmml/converter/ContinuousFeature;
             0      42     0  this   Lsklearn/tree/TreeUtil$8;
             0      42     1 feature   Lorg/jpmml/converter/Feature;
@@ -141,15 +141,15 @@
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: checkcast     #6                  // class org/jpmml/converter/Feature
          5: invokevirtual #7                  // Method apply:(Lorg/jpmml/converter/Feature;)Lorg/jpmml/converter/Feature;
          8: areturn
       LineNumberTable:
-        line 551: 0
+        line 555: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       9     0  this   Lsklearn/tree/TreeUtil$8;
 }
 Signature: #34                          // Ljava/lang/Object;Ljava/util/function/Function<Lorg/jpmml/converter/Feature;Lorg/jpmml/converter/Feature;>;
 SourceFile: "TreeUtil.java"
 EnclosingMethod: #38.#39                // sklearn.tree.TreeUtil.toTreeModelFeatureImportanceSchema
```

#### sklearn/tree/TreeUtil$5.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 0d6a3eeae2d43ec4fe41c638e0a01a41e5da5c2faa2ac39ebee507d85fe351ff
+  SHA-256 checksum df3560b0bb449738226a74dc63c33dc4b2ac8c225d9dbb269005159626286b47
   Compiled from "TreeUtil.java"
 final class sklearn.tree.TreeUtil$5 extends java.util.AbstractList<java.lang.Number>
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #5                          // sklearn/tree/TreeUtil$5
   super_class: #6                         // java/util/AbstractList
@@ -67,30 +67,30 @@
          0: aload_0
          1: aload_1
          2: putfield      #1                  // Field val$leafValues:[D
          5: aload_0
          6: invokespecial #2                  // Method java/util/AbstractList."<init>":()V
          9: return
       LineNumberTable:
-        line 413: 0
+        line 411: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lsklearn/tree/TreeUtil$5;
 
   public int size();
     descriptor: ()I
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #1                  // Field val$leafValues:[D
          4: arraylength
          5: ireturn
       LineNumberTable:
-        line 417: 0
+        line 415: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lsklearn/tree/TreeUtil$5;
 
   public java.lang.Number get(int);
     descriptor: (I)Ljava/lang/Number;
     flags: (0x0001) ACC_PUBLIC
@@ -101,16 +101,16 @@
          4: iload_1
          5: daload
          6: dstore_2
          7: dload_2
          8: invokestatic  #3                  // Method org/jpmml/converter/ValueUtil.narrow:(D)Ljava/lang/Number;
         11: areturn
       LineNumberTable:
-        line 422: 0
-        line 424: 7
+        line 420: 0
+        line 422: 7
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      12     0  this   Lsklearn/tree/TreeUtil$5;
             0      12     1 index   I
             7       5     2 leafValue   D
 
   public java.lang.Object get(int);
@@ -119,15 +119,15 @@
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: iload_1
          2: invokevirtual #4                  // Method get:(I)Ljava/lang/Number;
          5: areturn
       LineNumberTable:
-        line 413: 0
+        line 411: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lsklearn/tree/TreeUtil$5;
 }
 Signature: #27                          // Ljava/util/AbstractList<Ljava/lang/Number;>;
 SourceFile: "TreeUtil.java"
 EnclosingMethod: #31.#32                // sklearn.tree.TreeUtil.encodeNode
```

#### sklearn/tree/TreeUtil$6.class

##### procyon -ec {}

```diff
@@ -5,12 +5,12 @@
 import org.dmg.pmml.tree.Node;
 import java.util.List;
 import org.jpmml.model.visitors.AbstractVisitor;
 
 static final class TreeUtil$6 extends AbstractVisitor {
     public VisitorAction visit(final Node node) {
         if (!node.hasNodes()) {
-            this.val$values.add(node.getId());
+            this.val$result.add(node.getId());
         }
         return super.visit(node);
     }
 }
```

#### sklearn/tree/TreeUtil$7.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 9d0beb0c75dc4867daeabb187d76306396241962c6d2c86fe903f717aa61319e
+  SHA-256 checksum eb1f4571cbc22ea407d0c0d8972f0cef65cc2278ae4b0b997f7b9bb140e009e3
   Compiled from "TreeUtil.java"
 final class sklearn.tree.TreeUtil$7 extends java.lang.Object implements java.util.function.Function<org.jpmml.converter.Feature, org.jpmml.converter.Feature>
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #9                          // sklearn/tree/TreeUtil$7
   super_class: #10                        // java/lang/Object
@@ -87,15 +87,15 @@
          5: aload_0
          6: aload_2
          7: putfield      #2                  // Field val$dataType:Lorg/dmg/pmml/DataType;
         10: aload_0
         11: invokespecial #3                  // Method java/lang/Object."<init>":()V
         14: return
       LineNumberTable:
-        line 521: 0
+        line 525: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      15     0  this   Lsklearn/tree/TreeUtil$7;
 
   public org.jpmml.converter.Feature apply(org.jpmml.converter.Feature);
     descriptor: (Lorg/jpmml/converter/Feature;)Lorg/jpmml/converter/Feature;
     flags: (0x0001) ACC_PUBLIC
@@ -124,22 +124,22 @@
         36: aload_0
         37: getfield      #2                  // Field val$dataType:Lorg/dmg/pmml/DataType;
         40: invokevirtual #6                  // Method org/jpmml/converter/Feature.toContinuousFeature:(Lorg/dmg/pmml/DataType;)Lorg/jpmml/converter/ContinuousFeature;
         43: astore_2
         44: aload_2
         45: areturn
       LineNumberTable:
-        line 526: 0
-        line 527: 7
-        line 529: 12
-        line 532: 14
-        line 533: 28
-        line 535: 33
-        line 539: 35
-        line 541: 44
+        line 530: 0
+        line 531: 7
+        line 533: 12
+        line 536: 14
+        line 537: 28
+        line 539: 33
+        line 543: 35
+        line 545: 44
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            12       2     2 binaryFeature   Lorg/jpmml/converter/BinaryFeature;
            33       2     2 thresholdFeature   Lorg/jpmml/converter/ThresholdFeature;
            44       2     2 continuousFeature   Lorg/jpmml/converter/ContinuousFeature;
             0      46     0  this   Lsklearn/tree/TreeUtil$7;
             0      46     1 feature   Lorg/jpmml/converter/Feature;
@@ -154,15 +154,15 @@
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: checkcast     #7                  // class org/jpmml/converter/Feature
          5: invokevirtual #8                  // Method apply:(Lorg/jpmml/converter/Feature;)Lorg/jpmml/converter/Feature;
          8: areturn
       LineNumberTable:
-        line 521: 0
+        line 525: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       9     0  this   Lsklearn/tree/TreeUtil$7;
 }
 Signature: #37                          // Ljava/lang/Object;Ljava/util/function/Function<Lorg/jpmml/converter/Feature;Lorg/jpmml/converter/Feature;>;
 SourceFile: "TreeUtil.java"
 EnclosingMethod: #41.#42                // sklearn.tree.TreeUtil.toTreeModelSchema
```

#### sklearn/tree/TreeUtil.class

##### procyon -ec {}

```diff
@@ -1,17 +1,16 @@
 
 package sklearn.tree;
 
 import org.dmg.pmml.OutputField;
-import org.jpmml.converter.FieldNameUtil;
-import org.dmg.pmml.DataType;
 import org.dmg.pmml.mining.Segmentation;
-import org.dmg.pmml.Output;
+import org.dmg.pmml.DataType;
 import org.jpmml.model.UnsupportedElementException;
 import org.dmg.pmml.mining.Segment;
+import sklearn.HasMultiApplyField;
 import org.dmg.pmml.mining.MiningModel;
 import org.jpmml.converter.ContinuousFeature;
 import org.dmg.pmml.tree.LeafNode;
 import org.dmg.pmml.PMMLObject;
 import com.google.common.primitives.Doubles;
 import org.jpmml.converter.CategoricalLabel;
 import org.dmg.pmml.tree.BranchNode;
@@ -70,15 +69,15 @@
                 throw new IllegalArgumentException("Conflicting tree model options");
             }
             nodeExtensions = null;
             nodeId = winnerId;
             nodeScore = (((boolean)winnerId) ? Boolean.TRUE : null);
         }
         if (Boolean.TRUE.equals(winnerId)) {
-            encodeNodeId(model);
+            encodeNodeId(estimator, model);
         }
         final List<Visitor> visitors = new ArrayList<Visitor>();
         if (Boolean.TRUE.equals(prune)) {
             visitors.add((Visitor)new TreeModelPruner());
         }
         if (Boolean.TRUE.equals(compact)) {
             visitors.add((Visitor)new TreeModelCompactor());
@@ -222,44 +221,46 @@
             }
             final double value4 = values[index];
             result2 = (Node)new LeafNode((Object)Double.valueOf(value4), predicate).setId((Object)id);
         }
         return result2;
     }
     
-    private static void encodeNodeId(final Model model) {
-        final Output output = ModelUtil.ensureOutput(model);
+    private static void encodeNodeId(final Estimator estimator, final Model model) {
         if (model instanceof MiningModel) {
             final MiningModel miningModel = (MiningModel)model;
+            final HasMultiApplyField hasMultiApplyField = (HasMultiApplyField)estimator;
             final Segmentation segmentation = miningModel.requireSegmentation();
             final List<Segment> segments = segmentation.requireSegments();
             for (final Segment segment : segments) {
                 final TreeModel treeModel = (TreeModel)segment.requireModel((Class)TreeModel.class);
                 final String segmentId = segment.getId();
                 if (segmentId == null) {
                     throw new UnsupportedElementException((PMMLObject)segment);
                 }
-                encodeNodeId(output, treeModel, segmentId);
+                final List<Integer> nodeIds = collectNodeIds(treeModel);
+                final OutputField applyField = estimator.encodeApplyOutput((Model)miningModel, DataType.INTEGER, (List)nodeIds);
+                applyField.setName(hasMultiApplyField.getApplyField((Object)segmentId)).setSegmentId(segmentId);
             }
         }
         else {
+            if (!(model instanceof TreeModel)) {
+                throw new IllegalArgumentException();
+            }
             final TreeModel treeModel2 = (TreeModel)model;
-            encodeNodeId(output, treeModel2, null);
+            final List<Integer> nodeIds2 = collectNodeIds(treeModel2);
+            estimator.encodeApplyOutput((Model)treeModel2, DataType.INTEGER, (List)nodeIds2);
         }
     }
     
-    private static void encodeNodeId(final Output output, final TreeModel treeModel, final String segmentId) {
-        final List<Integer> values = new ArrayList<Integer>();
-        final Visitor nodeIdCollector = (Visitor)new TreeUtil.TreeUtil$6((List)values);
+    private static List<Integer> collectNodeIds(final TreeModel treeModel) {
+        final List<Integer> result = new ArrayList<Integer>();
+        final Visitor nodeIdCollector = (Visitor)new TreeUtil.TreeUtil$6((List)result);
         nodeIdCollector.applyTo((Visitable)treeModel);
-        final OutputField nodeIdField = ModelUtil.createEntityIdField("nodeId", DataType.INTEGER, (List)values);
-        if (segmentId != null) {
-            nodeIdField.setName(FieldNameUtil.create(nodeIdField.requireName(), new Object[] { segmentId })).setSegmentId(segmentId);
-        }
-        output.addOutputFields(new OutputField[] { nodeIdField });
+        return result;
     }
     
     private static Schema toTreeModelSchema(final DataType dataType, final boolean numeric, final Schema schema) {
         final Function<Feature, Feature> function = (Function<Feature, Feature>)new TreeUtil.TreeUtil$7(numeric, dataType);
         return schema.toTransformedSchema((Function)function);
     }
```

#### sklearn/tree/TreeUtil$3.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum e443cd81212d7b0bb862713490b8e16be17d86efd6c620b75f68d5a9b5bc9665
+  SHA-256 checksum dca8a72a335aaef426dcb04c7c019d964578eaac211e88ea6db9de4e8ac79921
   Compiled from "TreeUtil.java"
 final class sklearn.tree.TreeUtil$3 extends org.jpmml.model.visitors.AbstractVisitor
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #8                          // sklearn/tree/TreeUtil$3
   super_class: #9                         // org/jpmml/model/visitors/AbstractVisitor
@@ -69,15 +69,15 @@
     flags: (0x0000)
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #1                  // Method org/jpmml/model/visitors/AbstractVisitor."<init>":()V
          4: return
       LineNumberTable:
-        line 208: 0
+        line 206: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lsklearn/tree/TreeUtil$3;
 
   public org.dmg.pmml.VisitorAction visit(org.dmg.pmml.tree.Node);
     descriptor: (Lorg/dmg/pmml/tree/Node;)Lorg/dmg/pmml/VisitorAction;
     flags: (0x0001) ACC_PUBLIC
@@ -99,20 +99,20 @@
         25: aload_2
         26: invokeinterface #6,  1            // InterfaceMethod java/util/List.clear:()V
         31: aload_0
         32: aload_1
         33: invokespecial #7                  // Method org/jpmml/model/visitors/AbstractVisitor.visit:(Lorg/dmg/pmml/tree/Node;)Lorg/dmg/pmml/VisitorAction;
         36: areturn
       LineNumberTable:
-        line 213: 0
-        line 214: 7
-        line 216: 13
-        line 217: 20
-        line 219: 25
-        line 223: 31
+        line 211: 0
+        line 212: 7
+        line 214: 13
+        line 215: 20
+        line 217: 25
+        line 221: 31
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            25       6     2 scoreDistributions   Ljava/util/List;
             0      37     0  this   Lsklearn/tree/TreeUtil$3;
             0      37     1  node   Lorg/dmg/pmml/tree/Node;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
```

#### sklearn/tree/TreeUtil$2.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 982e44b7d9b59cbb6774bc178b486110a0779cbcab65a37e4af1a1f9150678cd
+  SHA-256 checksum aea5b8005680539aa288fe10864010d5a7b29fd4320d79a0c8abae8b311a0bd5
   Compiled from "TreeUtil.java"
 final class sklearn.tree.TreeUtil$2 extends org.jpmml.model.visitors.AbstractVisitor
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #4                          // sklearn/tree/TreeUtil$2
   super_class: #5                         // org/jpmml/model/visitors/AbstractVisitor
@@ -48,15 +48,15 @@
     flags: (0x0000)
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #1                  // Method org/jpmml/model/visitors/AbstractVisitor."<init>":()V
          4: return
       LineNumberTable:
-        line 194: 0
+        line 192: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lsklearn/tree/TreeUtil$2;
 
   public org.dmg.pmml.VisitorAction visit(org.dmg.pmml.tree.Node);
     descriptor: (Lorg/dmg/pmml/tree/Node;)Lorg/dmg/pmml/VisitorAction;
     flags: (0x0001) ACC_PUBLIC
@@ -67,16 +67,16 @@
          2: invokevirtual #2                  // Method org/dmg/pmml/tree/Node.setId:(Ljava/lang/Object;)Lorg/dmg/pmml/tree/Node;
          5: pop
          6: aload_0
          7: aload_1
          8: invokespecial #3                  // Method org/jpmml/model/visitors/AbstractVisitor.visit:(Lorg/dmg/pmml/tree/Node;)Lorg/dmg/pmml/VisitorAction;
         11: areturn
       LineNumberTable:
-        line 198: 0
-        line 200: 6
+        line 196: 0
+        line 198: 6
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      12     0  this   Lsklearn/tree/TreeUtil$2;
             0      12     1  node   Lorg/dmg/pmml/tree/Node;
 }
 SourceFile: "TreeUtil.java"
 EnclosingMethod: #21.#22                // sklearn.tree.TreeUtil.transform
```

#### sklearn/EstimatorUtil.class

##### procyon -ec {}

```diff
@@ -1,12 +1,13 @@
 
 package sklearn;
 
 import org.dmg.pmml.Output;
-import org.jpmml.converter.FieldNameUtil;
+import org.dmg.pmml.DataType;
+import org.jpmml.converter.CategoricalLabel;
 import org.dmg.pmml.OutputField;
 import java.util.Collections;
 import org.jpmml.converter.ScalarLabel;
 import org.jpmml.converter.Feature;
 import org.jpmml.sklearn.SkLearnEncoder;
 import org.dmg.pmml.Model;
 import org.jpmml.converter.Schema;
@@ -69,22 +70,22 @@
                     break;
                 }
                 break;
             }
         }
         switch (n) {
             case 0: {
-                if (estimator instanceof HasApplyField) {
-                    final HasApplyField hasApplyField = (HasApplyField)estimator;
-                    return encoder.export(model, hasApplyField.getApplyField());
-                }
                 if (estimator instanceof HasMultiApplyField) {
                     final HasMultiApplyField hasMultiApplyField = (HasMultiApplyField)estimator;
                     return encoder.export(model, hasMultiApplyField.getApplyFields());
                 }
+                if (estimator instanceof HasApplyField) {
+                    final HasApplyField hasApplyField = (HasApplyField)estimator;
+                    return encoder.export(model, hasApplyField.getApplyField());
+                }
                 throw new IllegalArgumentException();
             }
             case 1: {
                 if (estimator instanceof HasDecisionFunctionField) {
                     final HasDecisionFunctionField hasDecisionFunctionField = (HasDecisionFunctionField)estimator;
                     return encoder.export(model, hasDecisionFunctionField.getDecisionFunctionField());
                 }
@@ -123,16 +124,19 @@
                     outputField = (OutputField)Iterables.getLast((Iterable)predictionOutputFields);
                     return encoder.export(model, outputField.getName());
                 }
                 break;
             }
             case 3: {
                 if (estimator instanceof HasClasses) {
-                    final List<?> categories = getClasses(estimator);
-                    final List<String> names = (List<String>)categories.stream().map(category -> FieldNameUtil.create("probability", new Object[] { category })).collect((Collector<? super Object, ?, List<String>>)Collectors.toList());
+                    final HasClasses hasClasses = (HasClasses)estimator;
+                    final CategoricalLabel categoricalLabel = (CategoricalLabel)schema.getLabel();
+                    final List<OutputField> probabilityOutputFields = estimator.createPredictProbaFields(DataType.DOUBLE, categoricalLabel);
+                    final OutputField outputField;
+                    final List<String> names = (List<String>)probabilityOutputFields.stream().map(outputField -> outputField.requireName()).collect((Collector<? super Object, ?, List<String>>)Collectors.toList());
                     return encoder.export(model, (List)names);
                 }
                 throw new IllegalArgumentException();
             }
             default: {
                 throw new IllegalArgumentException(predictFunc);
             }
```

#### sklearn/Estimator.class

##### procyon -ec {}

```diff
@@ -1,11 +1,20 @@
 
 package sklearn;
 
 import org.slf4j.LoggerFactory;
+import org.dmg.pmml.Output;
+import org.dmg.pmml.Field;
+import org.jpmml.converter.PMMLUtil;
+import java.util.stream.Collector;
+import java.util.stream.Collectors;
+import org.jpmml.converter.ModelUtil;
+import org.jpmml.converter.FieldNameUtil;
+import org.dmg.pmml.OutputField;
+import org.jpmml.converter.CategoricalLabel;
 import numpy.core.NDArrayUtil;
 import java.util.LinkedHashMap;
 import java.util.Collections;
 import java.util.Map;
 import net.razorvine.pickle.objects.ClassDict;
 import org.jpmml.python.ClassDictUtil;
 import java.util.Collection;
@@ -190,15 +199,71 @@
     }
     
     public Estimator setPMMLOptions(final Map<String, ?> pmmlOptions) {
         this.put((Object)"pmml_options_", (Object)pmmlOptions);
         return this;
     }
     
+    public Object getPMMLSegmentId() {
+        return this.getOptionalScalar("pmml_segment_id_");
+    }
+    
+    public Estimator setPMMLSegmentId(final Object segmentId) {
+        if (segmentId != null) {
+            this.put((Object)"pmml_segment_id_", segmentId);
+        }
+        else {
+            this.remove((Object)"pmml_segment_id_");
+        }
+        return this;
+    }
+    
     public String getSkLearnVersion() {
         return this.getOptionalString("_sklearn_version");
     }
     
+    public List<OutputField> createPredictProbaFields(final DataType dataType, final CategoricalLabel categoricalLabel) {
+        final Object pmmlSegmentId = this.getPMMLSegmentId();
+        if (this instanceof HasClasses) {
+            final HasClasses hasClasses = (HasClasses)this;
+            final List<?> values = categoricalLabel.getValues();
+            return values.stream().map(value -> {
+                String name;
+                if (pmmlSegmentId != null) {
+                    name = FieldNameUtil.create("probability", new Object[] { pmmlSegmentId, value });
+                }
+                else {
+                    name = FieldNameUtil.create("probability", new Object[] { value });
+                }
+                return ModelUtil.createProbabilityField(name, dataType, value);
+            }).collect((Collector<? super Object, ?, List<OutputField>>)Collectors.toList());
+        }
+        throw new IllegalArgumentException();
+    }
+    
+    public OutputField createApplyField(final DataType dataType) {
+        final Object pmmlSegmentId = this.getPMMLSegmentId();
+        if (this instanceof HasApplyField) {
+            final HasApplyField hasApplyField = (HasApplyField)this;
+            String name = hasApplyField.getApplyField();
+            if (pmmlSegmentId != null) {
+                name = FieldNameUtil.create(name, new Object[] { pmmlSegmentId });
+            }
+            return ModelUtil.createEntityIdField(name, dataType);
+        }
+        throw new IllegalArgumentException();
+    }
+    
+    public OutputField encodeApplyOutput(final Model model, final DataType dataType, final List<?> values) {
+        final OutputField applyField = this.createApplyField(dataType);
+        if (values != null && !values.isEmpty()) {
+            PMMLUtil.addValues((Field)applyField, (List)values);
+        }
+        final Output output = ModelUtil.ensureOutput(model);
+        output.getOutputFields().add(applyField);
+        return applyField;
+    }
+    
     static {
         logger = LoggerFactory.getLogger((Class)Estimator.class);
     }
 }
```

#### sklearn2pmml/pipeline/PMMLPipeline$3.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 636779fe3174221315a98907318b48354103de9d90f5b95a5f92d26187e17e3b
+  SHA-256 checksum 100b5ac36b3092569b931572e64726fb0c168a5769e85768c0c3dc4ce642a52c
   Compiled from "PMMLPipeline.java"
 class sklearn2pmml.pipeline.PMMLPipeline$3
   minor version: 0
   major version: 52
   flags: (0x1020) ACC_SUPER, ACC_SYNTHETIC
   this_class: #13                         // sklearn2pmml/pipeline/PMMLPipeline$3
   super_class: #14                        // java/lang/Object
@@ -129,16 +129,16 @@
          from    to  target type
              9    20    23   Class java/lang/NoSuchFieldError
             24    35    38   Class java/lang/NoSuchFieldError
             39    50    53   Class java/lang/NoSuchFieldError
             63    74    77   Class java/lang/NoSuchFieldError
             78    89    92   Class java/lang/NoSuchFieldError
       LineNumberTable:
-        line 567: 0
-        line 333: 54
+        line 566: 0
+        line 332: 54
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
       StackMapTable: number_of_entries = 10
         frame_type = 87 /* same_locals_1_stack_item */
           stack = [ class java/lang/NoSuchFieldError ]
         frame_type = 0 /* same */
         frame_type = 77 /* same_locals_1_stack_item */
```

#### sklearn2pmml/pipeline/PMMLPipeline.class

##### procyon -ec {}

```diff
@@ -164,20 +164,20 @@
                     output.addOutputFields(new OutputField[] { predictField });
                     predictFields.add(predictField);
                 }
                 this.encodeOutput(output, predictFields, predictTransformer, encoder);
             }
             if (predictProbaTransformer != null) {
                 final CategoricalLabel categoricalLabel = (CategoricalLabel)label2;
-                final List<OutputField> predictProbaFields = ModelUtil.createProbabilityFields(DataType.DOUBLE, categoricalLabel.getValues());
+                final List<OutputField> predictProbaFields = estimator.createPredictProbaFields(DataType.DOUBLE, categoricalLabel);
                 this.encodeOutput(output, predictProbaFields, predictProbaTransformer, encoder);
             }
             if (applyTransformer != null) {
-                final OutputField nodeIdField = ModelUtil.createEntityIdField("nodeId", DataType.INTEGER);
-                this.encodeOutput(output, Collections.singletonList(nodeIdField), applyTransformer, encoder);
+                final OutputField applyField = estimator.createApplyField(DataType.INTEGER);
+                this.encodeOutput(output, Collections.singletonList(applyField), applyTransformer, encoder);
             }
             encoder.setModel(model);
         }
         if (estimator.isSupervised()) {
             if (verification == null) {
                 PMMLPipeline.logger.warn("Model verification data is not set. Use method '" + ClassDictUtil.formatMember((ClassDict)this, "verify(X)") + "' to correct this deficiency");
             }
```

#### sklearn2pmml/pipeline/PMMLPipeline$2.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum af07946ec47d92aa95ba36d975c10cfdbe818a96b0d5e2be8d4f4324261b1d6b
+  SHA-256 checksum 634ddfc2308d0370a574151a5617f14f9fd690611e67c2b146f4d32410146cb5
   Compiled from "PMMLPipeline.java"
 final class sklearn2pmml.pipeline.PMMLPipeline$2 extends java.lang.Object implements com.google.common.base.Function<java.lang.Object, java.lang.Object>
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #4                          // sklearn2pmml/pipeline/PMMLPipeline$2
   super_class: #5                         // java/lang/Object
@@ -56,15 +56,15 @@
     flags: (0x0000)
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #1                  // Method java/lang/Object."<init>":()V
          4: return
       LineNumberTable:
-        line 691: 0
+        line 690: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lsklearn2pmml/pipeline/PMMLPipeline$2;
 
   public java.lang.Object apply(java.lang.Object);
     descriptor: (Ljava/lang/Object;)Ljava/lang/Object;
     flags: (0x0001) ACC_PUBLIC
@@ -77,18 +77,18 @@
          6: invokestatic  #3                  // Method org/jpmml/converter/ValueUtil.isNaN:(Ljava/lang/Object;)Z
          9: ifeq          14
         12: aconst_null
         13: areturn
         14: aload_1
         15: areturn
       LineNumberTable:
-        line 695: 0
-        line 697: 5
-        line 698: 12
-        line 701: 14
+        line 694: 0
+        line 696: 5
+        line 697: 12
+        line 700: 14
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lsklearn2pmml/pipeline/PMMLPipeline$2;
             0      16     1 value   Ljava/lang/Object;
       StackMapTable: number_of_entries = 1
         frame_type = 14 /* same */
 }
```

#### sklearn2pmml/pipeline/PMMLPipeline$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum cb68a246d30686406bfc5b691bb4b248ba1d0d2076a6da1f6ab08c6a72ed4970
+  SHA-256 checksum 016ba14712410a3c7ed2cba46061783aaa01b81684490ee61d584ae12fce46ee
   Compiled from "PMMLPipeline.java"
 final class sklearn2pmml.pipeline.PMMLPipeline$1 extends org.jpmml.converter.visitors.AbstractExtender
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #9                          // sklearn2pmml/pipeline/PMMLPipeline$1
   super_class: #10                        // org/jpmml/converter/visitors/AbstractExtender
@@ -89,15 +89,15 @@
          1: aload_2
          2: putfield      #1                  // Field val$values:Ljava/util/Map;
          5: aload_0
          6: aload_1
          7: invokespecial #2                  // Method org/jpmml/converter/visitors/AbstractExtender."<init>":(Ljava/lang/String;)V
         10: return
       LineNumberTable:
-        line 642: 0
+        line 641: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      11     0  this   Lsklearn2pmml/pipeline/PMMLPipeline$1;
             0      11     1    x0   Ljava/lang/String;
 
   public org.dmg.pmml.VisitorAction visit(org.dmg.pmml.Value);
     descriptor: (Lorg/dmg/pmml/Value;)Lorg/dmg/pmml/VisitorAction;
@@ -121,19 +121,19 @@
         26: invokestatic  #6                  // Method org/jpmml/converter/ValueUtil.asString:(Ljava/lang/Object;)Ljava/lang/String;
         29: invokevirtual #7                  // Method addExtension:(Lorg/dmg/pmml/PMMLObject;Ljava/lang/String;)V
         32: aload_0
         33: aload_1
         34: invokespecial #8                  // Method org/jpmml/converter/visitors/AbstractExtender.visit:(Lorg/dmg/pmml/Value;)Lorg/dmg/pmml/VisitorAction;
         37: areturn
       LineNumberTable:
-        line 646: 0
-        line 648: 14
-        line 649: 18
-        line 651: 23
-        line 654: 32
+        line 645: 0
+        line 647: 14
+        line 648: 18
+        line 650: 23
+        line 653: 32
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      38     0  this   Lsklearn2pmml/pipeline/PMMLPipeline$1;
             0      38     1 pmmlValue   Lorg/dmg/pmml/Value;
            14      24     2 value   Ljava/lang/Object;
       StackMapTable: number_of_entries = 1
         frame_type = 252 /* append */
```

#### sklearn2pmml/SkLearn2PMMLFields.class

##### procyon -ec {}

```diff
@@ -2,8 +2,9 @@
 package sklearn2pmml;
 
 public interface SkLearn2PMMLFields
 {
     public static final String PMML_FEATURE_IMPORTANCES = "pmml_feature_importances_";
     public static final String PMML_NAME = "pmml_name_";
     public static final String PMML_OPTIONS = "pmml_options_";
+    public static final String PMML_SEGMENT_ID = "pmml_segment_id_";
 }
```

#### sklearn2pmml/ensemble/GBDTLRClassifier.class

##### procyon -ec {}

```diff
@@ -1,23 +1,23 @@
 
 package sklearn2pmml.ensemble;
 
-import org.dmg.pmml.mining.MiningModel;
 import sklearn.preprocessing.MultiOneHotEncoder;
+import org.dmg.pmml.Model;
 import org.jpmml.converter.mining.MiningModelUtil;
 import org.dmg.pmml.regression.RegressionModel;
 import org.jpmml.converter.ModelUtil;
 import org.jpmml.converter.Transformation;
 import org.dmg.pmml.DataType;
 import org.dmg.pmml.OpType;
 import sklearn.Estimator;
 import com.google.common.collect.Iterables;
 import org.jpmml.converter.SchemaUtil;
 import org.jpmml.converter.CategoricalLabel;
-import org.dmg.pmml.Model;
+import org.dmg.pmml.mining.MiningModel;
 import org.jpmml.converter.Schema;
 import sklearn.linear_model.LinearClassifier;
 import java.util.List;
 import sklearn.Classifier;
 
 public class GBDTLRClassifier extends Classifier
 {
@@ -31,25 +31,29 @@
     }
     
     public boolean hasProbabilityDistribution() {
         final LinearClassifier lr = this.getLR();
         return lr.hasProbabilityDistribution();
     }
     
-    public Model encodeModel(final Schema schema) {
+    public MiningModel encodeModel(final Schema schema) {
         final Classifier gbdt = this.getGBDT();
         final MultiOneHotEncoder ohe = this.getOHE();
         final LinearClassifier lr = this.getLR();
         final CategoricalLabel categoricalLabel = (CategoricalLabel)schema.getLabel();
         SchemaUtil.checkSize(2, categoricalLabel);
         final List<? extends Number> coef = lr.getCoef();
         final List<? extends Number> intercept = lr.getIntercept();
         final Schema segmentSchema = schema.toAnonymousSchema();
-        final MiningModel miningModel = GBDTUtil.encodeModel((Estimator)gbdt, ohe, (List)coef, (Number)Iterables.getOnlyElement((Iterable)intercept), segmentSchema).setOutput(ModelUtil.createPredictedOutput("decisionFunction", OpType.CONTINUOUS, DataType.DOUBLE, new Transformation[0]));
-        return (Model)MiningModelUtil.createBinaryLogisticClassification((Model)miningModel, 1.0, 0.0, RegressionModel.NormalizationMethod.LOGIT, lr.hasProbabilityDistribution(), schema);
+        final Model model = (Model)GBDTUtil.encodeModel((Estimator)gbdt, ohe, (List)coef, (Number)Iterables.getOnlyElement((Iterable)intercept), segmentSchema).setOutput(ModelUtil.createPredictedOutput("decisionFunction", OpType.CONTINUOUS, DataType.DOUBLE, new Transformation[0]));
+        final MiningModel miningModel = MiningModelUtil.createBinaryLogisticClassification(model, 1.0, 0.0, RegressionModel.NormalizationMethod.LOGIT, false, schema);
+        if (lr.hasProbabilityDistribution()) {
+            this.encodePredictProbaOutput((Model)miningModel, DataType.DOUBLE, categoricalLabel);
+        }
+        return miningModel;
     }
     
     public Classifier getGBDT() {
         return (Classifier)this.get("gbdt_", (Class)Classifier.class);
     }
     
     public LinearClassifier getLR() {
```

#### sklearn2pmml/tree/CHAIDRegressor.class

##### procyon -ec {}

```diff
@@ -1,24 +1,35 @@
 
 package sklearn2pmml.tree;
 
 import treelib.Tree;
-import org.dmg.pmml.MiningFunction;
+import java.util.List;
 import org.dmg.pmml.Model;
+import java.util.Collections;
+import org.dmg.pmml.DataType;
+import org.dmg.pmml.MiningFunction;
+import org.dmg.pmml.tree.TreeModel;
 import org.jpmml.converter.Schema;
+import sklearn.HasApplyField;
 import sklearn.Regressor;
 
-public class CHAIDRegressor extends Regressor
+public class CHAIDRegressor extends Regressor implements HasApplyField
 {
     public CHAIDRegressor(final String module, final String name) {
         super(module, name);
     }
     
-    public Model encodeModel(final Schema schema) {
+    public String getApplyField() {
+        return "nodeId";
+    }
+    
+    public TreeModel encodeModel(final Schema schema) {
         final Tree tree = this.getTree();
-        return (Model)CHAIDUtil.encodeModel(MiningFunction.REGRESSION, tree, schema);
+        final TreeModel treeModel = CHAIDUtil.encodeModel(MiningFunction.REGRESSION, tree, schema);
+        this.encodeApplyOutput((Model)treeModel, DataType.INTEGER, (List)Collections.emptyList());
+        return treeModel;
     }
     
     public Tree getTree() {
         return (Tree)this.get("treelib_tree_", (Class)Tree.class);
     }
 }
```

#### sklearn2pmml/tree/CHAIDUtil.class

##### procyon -ec {}

```diff
@@ -27,17 +27,14 @@
 import org.dmg.pmml.tree.ClassifierNode;
 import org.jpmml.converter.CategoricalLabel;
 import org.jpmml.converter.CategoricalFeature;
 import org.jpmml.python.ClassDictUtil;
 import java.util.Collection;
 import org.dmg.pmml.tree.Node;
 import org.jpmml.converter.ModelUtil;
-import org.dmg.pmml.DataType;
-import org.dmg.pmml.OutputField;
-import org.dmg.pmml.Output;
 import org.dmg.pmml.Predicate;
 import org.jpmml.converter.PredicateManager;
 import org.dmg.pmml.True;
 import org.dmg.pmml.tree.TreeModel;
 import org.jpmml.converter.Schema;
 import treelib.Tree;
 import org.dmg.pmml.MiningFunction;
@@ -45,17 +42,15 @@
 public class CHAIDUtil
 {
     private CHAIDUtil() {
     }
     
     public static TreeModel encodeModel(final MiningFunction miningFunction, final Tree tree, final Schema schema) {
         final Node root = encodeNode((Predicate)True.INSTANCE, tree.selectRoot(), tree, new PredicateManager(), schema);
-        final Output output = new Output().addOutputFields(new OutputField[] { ModelUtil.createEntityIdField("nodeId", DataType.INTEGER) });
-        final TreeModel treeModel = new TreeModel(miningFunction, ModelUtil.createMiningSchema(schema.getLabel()), root).setOutput(output);
-        return treeModel;
+        return new TreeModel(miningFunction, ModelUtil.createMiningSchema(schema.getLabel()), root);
     }
     
     private static Node encodeNode(final Predicate predicate, final treelib.Node node, final Tree tree, final PredicateManager predicateManager, final Schema schema) {
         final Label label = schema.getLabel();
         final chaid.Node tag = (chaid.Node)node.getTag((Class)chaid.Node.class);
         final List<treelib.Node> successors = node.selectSuccessors(tree);
         final Column depV = tag.getDepV();
```

#### sklearn2pmml/tree/CHAIDClassifier.class

##### procyon -ec {}

```diff
@@ -1,37 +1,38 @@
 
 package sklearn2pmml.tree;
 
-import java.util.List;
-import org.dmg.pmml.Output;
-import org.dmg.pmml.tree.TreeModel;
 import treelib.Tree;
-import org.dmg.pmml.OutputField;
-import java.util.Collection;
+import java.util.List;
+import java.util.Collections;
+import org.dmg.pmml.Model;
 import org.dmg.pmml.DataType;
-import org.jpmml.converter.ModelUtil;
 import org.dmg.pmml.MiningFunction;
 import org.jpmml.converter.CategoricalLabel;
-import org.dmg.pmml.Model;
+import org.dmg.pmml.tree.TreeModel;
 import org.jpmml.converter.Schema;
+import sklearn.HasApplyField;
 import sklearn.Classifier;
 
-public class CHAIDClassifier extends Classifier
+public class CHAIDClassifier extends Classifier implements HasApplyField
 {
     public CHAIDClassifier(final String module, final String name) {
         super(module, name);
     }
     
-    public Model encodeModel(final Schema schema) {
+    public String getApplyField() {
+        return "nodeId";
+    }
+    
+    public TreeModel encodeModel(final Schema schema) {
         final Tree tree = this.getTree();
         final CategoricalLabel categoricalLabel = (CategoricalLabel)schema.getLabel();
         final TreeModel treeModel = CHAIDUtil.encodeModel(MiningFunction.CLASSIFICATION, tree, schema);
-        final Output output = ModelUtil.ensureOutput((Model)treeModel);
-        final List<OutputField> outputFields = output.getOutputFields();
-        outputFields.addAll(ModelUtil.createProbabilityFields(DataType.DOUBLE, categoricalLabel.getValues()));
-        return (Model)treeModel;
+        this.encodePredictProbaOutput((Model)treeModel, DataType.DOUBLE, categoricalLabel);
+        this.encodeApplyOutput((Model)treeModel, DataType.INTEGER, (List)Collections.emptyList());
+        return treeModel;
     }
     
     public Tree getTree() {
         return (Tree)this.get("treelib_tree_", (Class)Tree.class);
     }
 }
```

#### sklearn2pmml/tree/CHAIDUtil$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum b007927b6c0eb491318f1d39348687790f3742497a65d3b0f9bd0dfc8bc046a7
+  SHA-256 checksum 2cca34795c37a2ce0f1fab08a7f97d55a3b2b0ca230dc969b194070fdae3e837
   Compiled from "CHAIDUtil.java"
 final class sklearn2pmml.tree.CHAIDUtil$1 extends java.lang.Object implements java.util.Comparator<treelib.Node>
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #9                          // sklearn2pmml/tree/CHAIDUtil$1
   super_class: #10                        // java/lang/Object
@@ -79,15 +79,15 @@
     flags: (0x0000)
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #1                  // Method java/lang/Object."<init>":()V
          4: return
       LineNumberTable:
-        line 103: 0
+        line 94: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lsklearn2pmml/tree/CHAIDUtil$1;
 
   public int compare(treelib.Node, treelib.Node);
     descriptor: (Ltreelib/Node;Ltreelib/Node;)I
     flags: (0x0001) ACC_PUBLIC
@@ -112,19 +112,19 @@
         34: aload         5
         36: invokeinterface #5,  1            // InterfaceMethod java/util/List.size:()I
         41: aload         6
         43: invokeinterface #5,  1            // InterfaceMethod java/util/List.size:()I
         48: invokestatic  #6                  // Method java/lang/Integer.compare:(II)I
         51: ireturn
       LineNumberTable:
-        line 107: 0
-        line 108: 10
-        line 110: 21
-        line 111: 27
-        line 113: 34
+        line 98: 0
+        line 99: 10
+        line 101: 21
+        line 102: 27
+        line 104: 34
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      52     0  this   Lsklearn2pmml/tree/CHAIDUtil$1;
             0      52     1  left   Ltreelib/Node;
             0      52     2 right   Ltreelib/Node;
            10      42     3 leftTag   Lchaid/Node;
            21      31     4 rightTag   Lchaid/Node;
@@ -144,15 +144,15 @@
          1: aload_1
          2: checkcast     #7                  // class treelib/Node
          5: aload_2
          6: checkcast     #7                  // class treelib/Node
          9: invokevirtual #8                  // Method compare:(Ltreelib/Node;Ltreelib/Node;)I
         12: ireturn
       LineNumberTable:
-        line 103: 0
+        line 94: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      13     0  this   Lsklearn2pmml/tree/CHAIDUtil$1;
 }
 Signature: #35                          // Ljava/lang/Object;Ljava/util/Comparator<Ltreelib/Node;>;
 SourceFile: "CHAIDUtil.java"
 EnclosingMethod: #39.#40                // sklearn2pmml.tree.CHAIDUtil.encodeNode
```

#### sklearn2pmml/expression/ExpressionClassifier.class

##### procyon -ec {}

```diff
@@ -1,15 +1,15 @@
 
 package sklearn2pmml.expression;
 
-import org.dmg.pmml.Model;
 import java.util.Iterator;
 import org.jpmml.python.Scope;
 import org.jpmml.converter.Feature;
 import org.jpmml.converter.PMMLEncoder;
+import org.dmg.pmml.Model;
 import org.dmg.pmml.DataType;
 import org.jpmml.converter.Label;
 import org.jpmml.converter.ModelUtil;
 import org.dmg.pmml.MiningFunction;
 import java.util.stream.Collector;
 import java.util.stream.Collectors;
 import java.util.Collection;
@@ -86,15 +86,16 @@
                 regressionTables = categories.stream().map(category -> ((RegressionTable)categoryRegressionTables.get(category)).setTargetCategory(category)).collect((Collector<? super Object, ?, List<RegressionTable>>)Collectors.toList());
                 break;
             }
             default: {
                 throw new IllegalArgumentException();
             }
         }
-        final RegressionModel regressionModel = new RegressionModel(MiningFunction.CLASSIFICATION, ModelUtil.createMiningSchema((Label)categoricalLabel), (List)regressionTables).setNormalizationMethod(normalizationMethod).setOutput(ModelUtil.createProbabilityOutput(DataType.DOUBLE, categoricalLabel));
+        final RegressionModel regressionModel = new RegressionModel(MiningFunction.CLASSIFICATION, ModelUtil.createMiningSchema((Label)categoricalLabel), (List)regressionTables).setNormalizationMethod(normalizationMethod);
+        this.encodePredictProbaOutput((Model)regressionModel, DataType.DOUBLE, categoricalLabel);
         return regressionModel;
     }
     
     public Map<?, Expression> getClassExprs() {
         return this.getDict("class_exprs");
     }
```

#### org/jpmml/sklearn/SkLearnEncoder.class

##### procyon -ec {}

```diff
@@ -66,14 +66,17 @@
     
     public List<Feature> export(final Model model, final String name) {
         return this.export(model, Collections.singletonList(name));
     }
     
     public List<Feature> export(final Model model, final List<String> names) {
         final Output output = model.getOutput();
+        if (output == null) {
+            throw new IllegalArgumentException();
+        }
         final List<OutputField> outputFields = output.getOutputFields();
         final List<Feature> result = new ArrayList<Feature>();
         for (final String name : names) {
             DerivedOutputField derivedOutputField = null;
             final List<OutputField> nameOutputFields = selectOutputFields(name, outputFields);
             for (final OutputField nameOutputField : nameOutputFields) {
                 derivedOutputField = this.createDerivedField(model, nameOutputField, true);
```

#### org/jpmml/sklearn/SkLearnEncoder$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum f47980d147b52839558c1ab373d26069d1fdb570cb6cb3ab1d213b517fbe3cb5
+  SHA-256 checksum a539c6cfab44503d3988e116c0d0cb1de9c662cb6a3e19237801f7c47a32f702
   Compiled from "SkLearnEncoder.java"
 class org.jpmml.sklearn.SkLearnEncoder$1
   minor version: 0
   major version: 52
   flags: (0x1020) ACC_SUPER, ACC_SYNTHETIC
   this_class: #13                         // org/jpmml/sklearn/SkLearnEncoder$1
   super_class: #14                        // java/lang/Object
@@ -129,16 +129,16 @@
          from    to  target type
              9    20    23   Class java/lang/NoSuchFieldError
             24    35    38   Class java/lang/NoSuchFieldError
             39    50    53   Class java/lang/NoSuchFieldError
             63    74    77   Class java/lang/NoSuchFieldError
             78    89    92   Class java/lang/NoSuchFieldError
       LineNumberTable:
-        line 302: 0
-        line 109: 54
+        line 305: 0
+        line 112: 54
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
       StackMapTable: number_of_entries = 10
         frame_type = 87 /* same_locals_1_stack_item */
           stack = [ class java/lang/NoSuchFieldError ]
         frame_type = 0 /* same */
         frame_type = 77 /* same_locals_1_stack_item */
```

#### META-INF/maven/org.jpmml/pmml-sklearn/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.28</version>
+    <version>1.7.29</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn converter</name>
   <description>JPMML Scikit-Learn to PMML converter</description>
   <licenses>
@@ -38,15 +38,15 @@
     </dependency>
   </dependencies>
   <build>
     <plugins>
       <plugin>
         <groupId>org.apache.maven.plugins</groupId>
         <artifactId>maven-jar-plugin</artifactId>
-        <version>3.2.2</version>
+        <version>3.3.0</version>
         <configuration>
           <archive>
             <manifestEntries>
               <Implementation-Title>JPMML-SkLearn library</Implementation-Title>
               <Implementation-Version>${project.version}</Implementation-Version>
             </manifestEntries>
           </archive>
```

#### META-INF/maven/org.jpmml/pmml-sklearn/pom.properties

```diff
@@ -1,3 +1,3 @@
 artifactId=pmml-sklearn
 groupId=org.jpmml
-version=1.7.28
+version=1.7.29
```

#### Comparing `sklearn/svm/OneClassSVMUtil$1.class` & `sklearn/OutlierDetectorUtil$1.class`

 * *Files 25% similar despite different names*

##### procyon -ec {}

```diff
@@ -1,18 +1,18 @@
 
-package sklearn.svm;
+package sklearn;
 
 import org.jpmml.converter.PMMLUtil;
 import org.dmg.pmml.Expression;
 import org.dmg.pmml.FieldRef;
-import sklearn.Estimator;
 import org.jpmml.converter.transformations.OutlierTransformation;
 
-static final class OneClassSVMUtil$1 extends OutlierTransformation {
+static final class OutlierDetectorUtil$1 extends OutlierTransformation {
     public String getName(final String name) {
         return this.val$estimator.createFieldName("outlier", new Object[0]);
     }
     
     public Expression createExpression(final FieldRef fieldRef) {
-        return (Expression)PMMLUtil.createApply("lessOrEqual", new Expression[] { (Expression)fieldRef, (Expression)PMMLUtil.createConstant((Number)Double.valueOf(0.0)) });
+        final Number threshold = ((OutlierDetector)this.val$estimator).getDecisionFunctionThreshold();
+        return (Expression)PMMLUtil.createApply("lessOrEqual", new Expression[] { (Expression)fieldRef, (Expression)PMMLUtil.createConstant(threshold) });
     }
 }
```

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-h2o-1.2.5.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-h2o-1.2.6.jar`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,39 +1,39 @@
-Zip file size: 46362 bytes, number of entries: 37
-drwxr-xr-x  2.0 unx        0 b- stor 22-Aug-31 16:41 META-INF/
--rw-r--r--  2.0 unx      154 b- defN 22-Aug-31 16:41 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 22-Aug-31 16:41 META-INF/services/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Aug-31 16:41 org/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Aug-31 16:41 org/jpmml/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Aug-31 16:41 org/jpmml/h2o/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Aug-31 16:41 org/jpmml/h2o/testing/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Aug-31 16:41 META-INF/maven/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Aug-31 16:41 META-INF/maven/org.jpmml/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Aug-31 16:41 META-INF/maven/org.jpmml/pmml-h2o/
--rw-rw-r--  2.0 unx       32 b- defN 22-Aug-31 16:41 META-INF/services/hex.genmodel.ModelMojoReader
--rw-rw-r--  2.0 unx     7639 b- defN 22-Aug-31 16:41 org/jpmml/h2o/GbmMojoModelConverter.class
--rw-rw-r--  2.0 unx     1798 b- defN 22-Aug-31 16:41 org/jpmml/h2o/IsolationForestMojoModelConverter$1.class
--rw-rw-r--  2.0 unx     4088 b- defN 22-Aug-31 16:41 org/jpmml/h2o/XGBoostMojoModelConverter.class
--rw-rw-r--  2.0 unx     2013 b- defN 22-Aug-31 16:41 org/jpmml/h2o/testing/H2OEncoderBatchTest.class
--rw-rw-r--  2.0 unx     2897 b- defN 22-Aug-31 16:41 org/jpmml/h2o/testing/H2OEncoderBatch.class
--rw-rw-r--  2.0 unx     1591 b- defN 22-Aug-31 16:41 org/jpmml/h2o/testing/H2OEncoderBatchTest$1.class
--rw-rw-r--  2.0 unx     8548 b- defN 22-Aug-31 16:41 org/jpmml/h2o/GlmMojoModelBaseConverter.class
--rw-rw-r--  2.0 unx     4387 b- defN 22-Aug-31 16:41 org/jpmml/h2o/IsolationForestMojoModelConverter.class
--rw-rw-r--  2.0 unx     3400 b- defN 22-Aug-31 16:41 org/jpmml/h2o/XGBoostMojoModelConverter$1.class
--rw-rw-r--  2.0 unx     4469 b- defN 22-Aug-31 16:41 org/jpmml/h2o/GlmMojoModelConverter.class
--rw-rw-r--  2.0 unx      664 b- defN 22-Aug-31 16:41 org/jpmml/h2o/H2OEncoder$1.class
--rw-rw-r--  2.0 unx     1344 b- defN 22-Aug-31 16:41 org/jpmml/h2o/MojoModelUtil$1.class
--rw-rw-r--  2.0 unx     3560 b- defN 22-Aug-31 16:41 org/jpmml/h2o/H2OEncoder.class
--rw-rw-r--  2.0 unx     1117 b- defN 22-Aug-31 16:41 org/jpmml/h2o/XGBoostMojoModel.class
--rw-rw-r--  2.0 unx    12570 b- defN 22-Aug-31 16:41 org/jpmml/h2o/SharedTreeMojoModelConverter.class
--rw-rw-r--  2.0 unx     4030 b- defN 22-Aug-31 16:41 org/jpmml/h2o/GlmMultinomialMojoModelConverter.class
--rw-rw-r--  2.0 unx     1586 b- defN 22-Aug-31 16:41 org/jpmml/h2o/XGBoostMojoReader.class
--rw-rw-r--  2.0 unx     1412 b- defN 22-Aug-31 16:41 org/jpmml/h2o/ImputerUtil.class
--rw-rw-r--  2.0 unx     7050 b- defN 22-Aug-31 16:41 org/jpmml/h2o/DrfMojoModelConverter.class
--rw-rw-r--  2.0 unx     5387 b- defN 22-Aug-31 16:41 org/jpmml/h2o/Converter.class
--rw-rw-r--  2.0 unx     1840 b- defN 22-Aug-31 16:41 org/jpmml/h2o/MojoModelUtil.class
--rw-rw-r--  2.0 unx     3179 b- defN 22-Aug-31 16:41 org/jpmml/h2o/GlmMojoModelBaseConverter$1.class
--rw-rw-r--  2.0 unx     7520 b- defN 22-Aug-31 16:41 org/jpmml/h2o/StackedEnsembleMojoModelConverter.class
--rw-rw-r--  2.0 unx     2304 b- defN 22-Aug-31 16:41 org/jpmml/h2o/ConverterFactory.class
--rw-rw-r--  2.0 unx     1952 b- defN 22-Aug-31 16:41 META-INF/maven/org.jpmml/pmml-h2o/pom.xml
--rw-rw-r--  2.0 unx       52 b- defN 22-Aug-31 16:41 META-INF/maven/org.jpmml/pmml-h2o/pom.properties
-37 files, 96583 bytes uncompressed, 40904 bytes compressed:  57.6%
+Zip file size: 46363 bytes, number of entries: 37
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-30 22:11 META-INF/
+-rw-r--r--  2.0 unx      154 b- defN 23-May-30 22:11 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 22:11 META-INF/services/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 22:11 org/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 22:11 org/jpmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 22:11 org/jpmml/h2o/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 22:11 org/jpmml/h2o/testing/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-30 22:11 META-INF/maven/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-30 22:11 META-INF/maven/org.jpmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-30 22:11 META-INF/maven/org.jpmml/pmml-h2o/
+-rw-rw-r--  2.0 unx       32 b- defN 23-May-30 22:11 META-INF/services/hex.genmodel.ModelMojoReader
+-rw-rw-r--  2.0 unx     7639 b- defN 23-May-30 22:11 org/jpmml/h2o/GbmMojoModelConverter.class
+-rw-rw-r--  2.0 unx     1798 b- defN 23-May-30 22:11 org/jpmml/h2o/IsolationForestMojoModelConverter$1.class
+-rw-rw-r--  2.0 unx     4088 b- defN 23-May-30 22:11 org/jpmml/h2o/XGBoostMojoModelConverter.class
+-rw-rw-r--  2.0 unx     2013 b- defN 23-May-30 22:11 org/jpmml/h2o/testing/H2OEncoderBatchTest.class
+-rw-rw-r--  2.0 unx     2897 b- defN 23-May-30 22:11 org/jpmml/h2o/testing/H2OEncoderBatch.class
+-rw-rw-r--  2.0 unx     1591 b- defN 23-May-30 22:11 org/jpmml/h2o/testing/H2OEncoderBatchTest$1.class
+-rw-rw-r--  2.0 unx     8548 b- defN 23-May-30 22:11 org/jpmml/h2o/GlmMojoModelBaseConverter.class
+-rw-rw-r--  2.0 unx     4387 b- defN 23-May-30 22:11 org/jpmml/h2o/IsolationForestMojoModelConverter.class
+-rw-rw-r--  2.0 unx     3400 b- defN 23-May-30 22:11 org/jpmml/h2o/XGBoostMojoModelConverter$1.class
+-rw-rw-r--  2.0 unx     4469 b- defN 23-May-30 22:11 org/jpmml/h2o/GlmMojoModelConverter.class
+-rw-rw-r--  2.0 unx      664 b- defN 23-May-30 22:11 org/jpmml/h2o/H2OEncoder$1.class
+-rw-rw-r--  2.0 unx     1344 b- defN 23-May-30 22:11 org/jpmml/h2o/MojoModelUtil$1.class
+-rw-rw-r--  2.0 unx     3560 b- defN 23-May-30 22:11 org/jpmml/h2o/H2OEncoder.class
+-rw-rw-r--  2.0 unx     1117 b- defN 23-May-30 22:11 org/jpmml/h2o/XGBoostMojoModel.class
+-rw-rw-r--  2.0 unx    12570 b- defN 23-May-30 22:11 org/jpmml/h2o/SharedTreeMojoModelConverter.class
+-rw-rw-r--  2.0 unx     4030 b- defN 23-May-30 22:11 org/jpmml/h2o/GlmMultinomialMojoModelConverter.class
+-rw-rw-r--  2.0 unx     1586 b- defN 23-May-30 22:11 org/jpmml/h2o/XGBoostMojoReader.class
+-rw-rw-r--  2.0 unx     1412 b- defN 23-May-30 22:11 org/jpmml/h2o/ImputerUtil.class
+-rw-rw-r--  2.0 unx     7050 b- defN 23-May-30 22:11 org/jpmml/h2o/DrfMojoModelConverter.class
+-rw-rw-r--  2.0 unx     5387 b- defN 23-May-30 22:11 org/jpmml/h2o/Converter.class
+-rw-rw-r--  2.0 unx     1840 b- defN 23-May-30 22:11 org/jpmml/h2o/MojoModelUtil.class
+-rw-rw-r--  2.0 unx     3179 b- defN 23-May-30 22:11 org/jpmml/h2o/GlmMojoModelBaseConverter$1.class
+-rw-rw-r--  2.0 unx     7520 b- defN 23-May-30 22:11 org/jpmml/h2o/StackedEnsembleMojoModelConverter.class
+-rw-rw-r--  2.0 unx     2304 b- defN 23-May-30 22:11 org/jpmml/h2o/ConverterFactory.class
+-rw-rw-r--  2.0 unx     1952 b- defN 23-May-30 22:11 META-INF/maven/org.jpmml/pmml-h2o/pom.xml
+-rw-rw-r--  2.0 unx       52 b- defN 23-May-30 22:11 META-INF/maven/org.jpmml/pmml-h2o/pom.properties
+37 files, 96583 bytes uncompressed, 40905 bytes compressed:  57.6%
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,6 +1,6 @@
 Manifest-Version: 1.0
 Implementation-Title: JPMML-H2O library
-Implementation-Version: 1.2.5
+Implementation-Version: 1.2.6
 Build-Jdk-Spec: 1.8
-Created-By: Maven JAR Plugin 3.2.2
+Created-By: Maven JAR Plugin 3.3.0
```

#### META-INF/maven/org.jpmml/pmml-h2o/pom.xml

##### META-INF/maven/org.jpmml/pmml-h2o/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-h2o</artifactId>
-    <version>1.2.5</version>
+    <version>1.2.6</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-h2o</artifactId>
   <packaging>jar</packaging>
   <name>JPMML H2O.ai converter</name>
   <description>JPMML H2O.ai to PMML converter</description>
   <licenses>
@@ -46,15 +46,15 @@
     </dependency>
   </dependencies>
   <build>
     <plugins>
       <plugin>
         <groupId>org.apache.maven.plugins</groupId>
         <artifactId>maven-jar-plugin</artifactId>
-        <version>3.2.2</version>
+        <version>3.3.0</version>
         <configuration>
           <archive>
             <manifestEntries>
               <Implementation-Title>JPMML-H2O library</Implementation-Title>
               <Implementation-Version>${project.version}</Implementation-Version>
             </manifestEntries>
           </archive>
```

#### META-INF/maven/org.jpmml/pmml-h2o/pom.properties

```diff
@@ -1,3 +1,3 @@
 artifactId=pmml-h2o
 groupId=org.jpmml
-version=1.2.5
+version=1.2.6
```

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-sklearn-extension-1.7.28.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-sklearn-extension-1.7.29.jar`

 * *Files 12% similar despite different names*

#### zipinfo {}

```diff
@@ -1,69 +1,69 @@
-Zip file size: 84308 bytes, number of entries: 67
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-May-17 09:50 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 mlxtend/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 mlxtend/preprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 pycaret/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 pycaret/preprocess/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 tpot/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 tpot/builtins/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 optbinning/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 optbinning/scorecard/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 imblearn/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 category_encoders/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklego/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklego/meta/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklego/preprocessing/
--rw-rw-r--  2.0 unx      913 b- defN 23-May-17 09:50 mlxtend/preprocessing/DenseTransformer.class
--rw-rw-r--  2.0 unx     4244 b- defN 23-May-17 09:50 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx      898 b- defN 23-May-17 09:50 pycaret/preprocess/FixImbalancer.class
--rw-rw-r--  2.0 unx     2818 b- defN 23-May-17 09:50 pycaret/preprocess/RemoveMulticollinearity.class
--rw-rw-r--  2.0 unx      907 b- defN 23-May-17 09:50 pycaret/preprocess/CleanColumnNames.class
--rw-rw-r--  2.0 unx     4017 b- defN 23-May-17 09:50 pycaret/preprocess/RareCategoryGrouping.class
--rw-rw-r--  2.0 unx     7434 b- defN 23-May-17 09:50 pycaret/preprocess/TransformerWrapper.class
--rw-rw-r--  2.0 unx     4951 b- defN 23-May-17 09:50 pycaret/preprocess/TransformerWrapperWithInverse.class
--rw-rw-r--  2.0 unx      720 b- defN 23-May-17 09:50 tpot/builtins/StackingEstimator$1.class
--rw-rw-r--  2.0 unx     4530 b- defN 23-May-17 09:50 tpot/builtins/StackingEstimator.class
--rw-rw-r--  2.0 unx     2433 b- defN 23-May-17 09:50 optbinning/BinnedFeature.class
--rw-rw-r--  2.0 unx     8560 b- defN 23-May-17 09:50 optbinning/scorecard/Scorecard.class
--rw-rw-r--  2.0 unx     2133 b- defN 23-May-17 09:50 optbinning/OptimalBinningUtil.class
--rw-rw-r--  2.0 unx     6372 b- defN 23-May-17 09:50 optbinning/BinningProcess.class
--rw-rw-r--  2.0 unx     2274 b- defN 23-May-17 09:50 optbinning/ContinuousOptimalBinning.class
--rw-rw-r--  2.0 unx     3917 b- defN 23-May-17 09:50 optbinning/MulticlassOptimalBinning.class
--rw-rw-r--  2.0 unx     1242 b- defN 23-May-17 09:50 optbinning/BinningProcess$1.class
--rw-rw-r--  2.0 unx    14050 b- defN 23-May-17 09:50 optbinning/OptimalBinning.class
--rw-rw-r--  2.0 unx      860 b- defN 23-May-17 09:50 imblearn/Sampler.class
--rw-rw-r--  2.0 unx     1916 b- defN 23-May-17 09:50 category_encoders/MapEncoder.class
--rw-rw-r--  2.0 unx     8449 b- defN 23-May-17 09:50 category_encoders/MapFeature.class
--rw-rw-r--  2.0 unx      527 b- defN 23-May-17 09:50 category_encoders/TargetEncoder.class
--rw-rw-r--  2.0 unx     1451 b- defN 23-May-17 09:50 category_encoders/CountEncoder$1.class
--rw-rw-r--  2.0 unx      515 b- defN 23-May-17 09:50 category_encoders/WOEEncoder.class
--rw-rw-r--  2.0 unx     9124 b- defN 23-May-17 09:50 category_encoders/MeanEncoder.class
--rw-rw-r--  2.0 unx     8520 b- defN 23-May-17 09:50 category_encoders/CountEncoder.class
--rw-rw-r--  2.0 unx    12815 b- defN 23-May-17 09:50 category_encoders/BaseNFeature.class
--rw-rw-r--  2.0 unx     1123 b- defN 23-May-17 09:50 category_encoders/MeanEncoder$2.class
--rw-rw-r--  2.0 unx     1481 b- defN 23-May-17 09:50 category_encoders/OrdinalMapEncoder$1.class
--rw-rw-r--  2.0 unx     1445 b- defN 23-May-17 09:50 category_encoders/MeanEncoder$1.class
--rw-rw-r--  2.0 unx     2119 b- defN 23-May-17 09:50 category_encoders/OrdinalEncoder$Mapping.class
--rw-rw-r--  2.0 unx     1323 b- defN 23-May-17 09:50 category_encoders/LeaveOneOutEncoder$1.class
--rw-rw-r--  2.0 unx     7967 b- defN 23-May-17 09:50 category_encoders/OrdinalMapEncoder.class
--rw-rw-r--  2.0 unx     9241 b- defN 23-May-17 09:50 category_encoders/BaseNEncoder.class
--rw-rw-r--  2.0 unx     1334 b- defN 23-May-17 09:50 category_encoders/BinaryEncoder.class
--rw-rw-r--  2.0 unx     3547 b- defN 23-May-17 09:50 category_encoders/OneHotEncoder.class
--rw-rw-r--  2.0 unx     1325 b- defN 23-May-17 09:50 category_encoders/CatBoostEncoder.class
--rw-rw-r--  2.0 unx     2062 b- defN 23-May-17 09:50 category_encoders/CategoryEncoderUtil.class
--rw-rw-r--  2.0 unx     1564 b- defN 23-May-17 09:50 category_encoders/OrdinalEncoder$1.class
--rw-rw-r--  2.0 unx     1047 b- defN 23-May-17 09:50 category_encoders/LeaveOneOutEncoder.class
--rw-rw-r--  2.0 unx     4690 b- defN 23-May-17 09:50 category_encoders/OrdinalEncoder.class
--rw-rw-r--  2.0 unx      742 b- defN 23-May-17 09:50 category_encoders/MeanEncoder$MeanFunction.class
--rw-rw-r--  2.0 unx     1378 b- defN 23-May-17 09:50 category_encoders/CatBoostEncoder$1.class
--rw-rw-r--  2.0 unx     2162 b- defN 23-May-17 09:50 category_encoders/CategoryEncoder.class
--rw-rw-r--  2.0 unx      725 b- defN 23-May-17 09:50 sklego/meta/EstimatorTransformer$1.class
--rw-rw-r--  2.0 unx     7272 b- defN 23-May-17 09:50 sklego/meta/EstimatorTransformer.class
--rw-rw-r--  2.0 unx      920 b- defN 23-May-17 09:50 sklego/preprocessing/IdentityTransformer.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn-extension/
--rw-rw-r--  2.0 unx     1226 b- defN 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml
--rw-rw-r--  2.0 unx      118 b- defN 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.properties
-67 files, 171531 bytes uncompressed, 74742 bytes compressed:  56.4%
+Zip file size: 84309 bytes, number of entries: 67
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Jun-06 10:35 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 mlxtend/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 mlxtend/preprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 pycaret/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 pycaret/preprocess/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 tpot/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 tpot/builtins/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 optbinning/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 optbinning/scorecard/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 imblearn/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 category_encoders/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklego/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklego/meta/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklego/preprocessing/
+-rw-rw-r--  2.0 unx      913 b- defN 23-Jun-06 10:35 mlxtend/preprocessing/DenseTransformer.class
+-rw-rw-r--  2.0 unx     4244 b- defN 23-Jun-06 10:35 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx      898 b- defN 23-Jun-06 10:35 pycaret/preprocess/FixImbalancer.class
+-rw-rw-r--  2.0 unx     2818 b- defN 23-Jun-06 10:35 pycaret/preprocess/RemoveMulticollinearity.class
+-rw-rw-r--  2.0 unx      907 b- defN 23-Jun-06 10:35 pycaret/preprocess/CleanColumnNames.class
+-rw-rw-r--  2.0 unx     4017 b- defN 23-Jun-06 10:35 pycaret/preprocess/RareCategoryGrouping.class
+-rw-rw-r--  2.0 unx     7434 b- defN 23-Jun-06 10:35 pycaret/preprocess/TransformerWrapper.class
+-rw-rw-r--  2.0 unx     4951 b- defN 23-Jun-06 10:35 pycaret/preprocess/TransformerWrapperWithInverse.class
+-rw-rw-r--  2.0 unx      720 b- defN 23-Jun-06 10:35 tpot/builtins/StackingEstimator$1.class
+-rw-rw-r--  2.0 unx     4530 b- defN 23-Jun-06 10:35 tpot/builtins/StackingEstimator.class
+-rw-rw-r--  2.0 unx     2433 b- defN 23-Jun-06 10:35 optbinning/BinnedFeature.class
+-rw-rw-r--  2.0 unx     8560 b- defN 23-Jun-06 10:35 optbinning/scorecard/Scorecard.class
+-rw-rw-r--  2.0 unx     2133 b- defN 23-Jun-06 10:35 optbinning/OptimalBinningUtil.class
+-rw-rw-r--  2.0 unx     6372 b- defN 23-Jun-06 10:35 optbinning/BinningProcess.class
+-rw-rw-r--  2.0 unx     2274 b- defN 23-Jun-06 10:35 optbinning/ContinuousOptimalBinning.class
+-rw-rw-r--  2.0 unx     3917 b- defN 23-Jun-06 10:35 optbinning/MulticlassOptimalBinning.class
+-rw-rw-r--  2.0 unx     1242 b- defN 23-Jun-06 10:35 optbinning/BinningProcess$1.class
+-rw-rw-r--  2.0 unx    14050 b- defN 23-Jun-06 10:35 optbinning/OptimalBinning.class
+-rw-rw-r--  2.0 unx      860 b- defN 23-Jun-06 10:35 imblearn/Sampler.class
+-rw-rw-r--  2.0 unx     1916 b- defN 23-Jun-06 10:35 category_encoders/MapEncoder.class
+-rw-rw-r--  2.0 unx     8449 b- defN 23-Jun-06 10:35 category_encoders/MapFeature.class
+-rw-rw-r--  2.0 unx      527 b- defN 23-Jun-06 10:35 category_encoders/TargetEncoder.class
+-rw-rw-r--  2.0 unx     1451 b- defN 23-Jun-06 10:35 category_encoders/CountEncoder$1.class
+-rw-rw-r--  2.0 unx      515 b- defN 23-Jun-06 10:35 category_encoders/WOEEncoder.class
+-rw-rw-r--  2.0 unx     9124 b- defN 23-Jun-06 10:35 category_encoders/MeanEncoder.class
+-rw-rw-r--  2.0 unx     8520 b- defN 23-Jun-06 10:35 category_encoders/CountEncoder.class
+-rw-rw-r--  2.0 unx    12815 b- defN 23-Jun-06 10:35 category_encoders/BaseNFeature.class
+-rw-rw-r--  2.0 unx     1123 b- defN 23-Jun-06 10:35 category_encoders/MeanEncoder$2.class
+-rw-rw-r--  2.0 unx     1481 b- defN 23-Jun-06 10:35 category_encoders/OrdinalMapEncoder$1.class
+-rw-rw-r--  2.0 unx     1445 b- defN 23-Jun-06 10:35 category_encoders/MeanEncoder$1.class
+-rw-rw-r--  2.0 unx     2119 b- defN 23-Jun-06 10:35 category_encoders/OrdinalEncoder$Mapping.class
+-rw-rw-r--  2.0 unx     1323 b- defN 23-Jun-06 10:35 category_encoders/LeaveOneOutEncoder$1.class
+-rw-rw-r--  2.0 unx     7967 b- defN 23-Jun-06 10:35 category_encoders/OrdinalMapEncoder.class
+-rw-rw-r--  2.0 unx     9241 b- defN 23-Jun-06 10:35 category_encoders/BaseNEncoder.class
+-rw-rw-r--  2.0 unx     1334 b- defN 23-Jun-06 10:35 category_encoders/BinaryEncoder.class
+-rw-rw-r--  2.0 unx     3547 b- defN 23-Jun-06 10:35 category_encoders/OneHotEncoder.class
+-rw-rw-r--  2.0 unx     1325 b- defN 23-Jun-06 10:35 category_encoders/CatBoostEncoder.class
+-rw-rw-r--  2.0 unx     2062 b- defN 23-Jun-06 10:35 category_encoders/CategoryEncoderUtil.class
+-rw-rw-r--  2.0 unx     1564 b- defN 23-Jun-06 10:35 category_encoders/OrdinalEncoder$1.class
+-rw-rw-r--  2.0 unx     1047 b- defN 23-Jun-06 10:35 category_encoders/LeaveOneOutEncoder.class
+-rw-rw-r--  2.0 unx     4690 b- defN 23-Jun-06 10:35 category_encoders/OrdinalEncoder.class
+-rw-rw-r--  2.0 unx      742 b- defN 23-Jun-06 10:35 category_encoders/MeanEncoder$MeanFunction.class
+-rw-rw-r--  2.0 unx     1378 b- defN 23-Jun-06 10:35 category_encoders/CatBoostEncoder$1.class
+-rw-rw-r--  2.0 unx     2162 b- defN 23-Jun-06 10:35 category_encoders/CategoryEncoder.class
+-rw-rw-r--  2.0 unx      725 b- defN 23-Jun-06 10:35 sklego/meta/EstimatorTransformer$1.class
+-rw-rw-r--  2.0 unx     7272 b- defN 23-Jun-06 10:35 sklego/meta/EstimatorTransformer.class
+-rw-rw-r--  2.0 unx      920 b- defN 23-Jun-06 10:35 sklego/preprocessing/IdentityTransformer.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn-extension/
+-rw-rw-r--  2.0 unx     1226 b- defN 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml
+-rw-rw-r--  2.0 unx      118 b- defN 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.properties
+67 files, 171531 bytes uncompressed, 74743 bytes compressed:  56.4%
```

#### META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.28</version>
+    <version>1.7.29</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-extension</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn extensions converter</name>
   <description>JPMML Scikit-Learn extension packages to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Wed May 17 09:50:30 EEST 2023
-version=1.7.28
+#Tue Jun 06 10:35:43 EEST 2023
+version=1.7.29
 groupId=org.jpmml
 artifactId=pmml-sklearn-extension
```

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/h2o-logger-3.40.0.4.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/h2o-logger-3.40.0.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar`

 * *Files 22% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 5703 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-17 09:56 META-INF/
--rw-r--r--  2.0 unx      158 b- defN 23-May-17 09:56 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:56 com/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:56 com/sklearn2pmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-17 09:56 META-INF/maven/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-17 09:56 META-INF/maven/com.sklearn2pmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-17 09:56 META-INF/maven/com.sklearn2pmml/sklearn2pmml/
--rw-rw-r--  2.0 unx     3741 b- defN 23-May-17 09:56 com/sklearn2pmml/Main.class
--rw-rw-r--  2.0 unx     1200 b- defN 23-May-17 09:56 com/sklearn2pmml/Main$1.class
--rw-rw-r--  2.0 unx     7844 b- defN 23-May-17 09:56 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.xml
--rw-rw-r--  2.0 unx       70 b- defN 23-May-17 09:56 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.properties
-11 files, 13013 bytes uncompressed, 4227 bytes compressed:  67.5%
+Zip file size: 5704 bytes, number of entries: 11
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 10:41 META-INF/
+-rw-r--r--  2.0 unx      158 b- defN 23-Jun-06 10:41 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:41 com/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:41 com/sklearn2pmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 10:41 META-INF/maven/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 10:41 META-INF/maven/com.sklearn2pmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 10:41 META-INF/maven/com.sklearn2pmml/sklearn2pmml/
+-rw-rw-r--  2.0 unx     3741 b- defN 23-Jun-06 10:41 com/sklearn2pmml/Main.class
+-rw-rw-r--  2.0 unx     1200 b- defN 23-Jun-06 10:41 com/sklearn2pmml/Main$1.class
+-rw-rw-r--  2.0 unx     7844 b- defN 23-Jun-06 10:40 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.xml
+-rw-rw-r--  2.0 unx       70 b- defN 23-Jun-06 10:41 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.properties
+11 files, 13013 bytes uncompressed, 4228 bytes compressed:  67.5%
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,6 +1,6 @@
 Manifest-Version: 1.0
 Implementation-Title: SkLearn2PMML package
-Implementation-Version: 0.92.2
+Implementation-Version: 0.93.0
 Build-Jdk-Spec: 1.8
 Created-By: Maven JAR Plugin 3.2.2
```

#### META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.xml

##### META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.xml

```diff
@@ -24,15 +24,15 @@
     <tag>HEAD</tag>
   </scm>
   <issueManagement>
     <system>GitHub</system>
     <url>https://github.com/jpmml/sklearn2pmml/issues</url>
   </issueManagement>
   <properties>
-    <jpmml-sklearn.version>1.7.28</jpmml-sklearn.version>
+    <jpmml-sklearn.version>1.7.29</jpmml-sklearn.version>
   </properties>
   <dependencies>
     <dependency>
       <groupId>org.jpmml</groupId>
       <artifactId>pmml-sklearn</artifactId>
       <version>${jpmml-sklearn.version}</version>
       <exclusions>
```

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.28.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.29.jar`

 * *Files 18% similar despite different names*

#### zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 6332 bytes, number of entries: 15
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-May-17 09:50 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 h2o/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 h2o/estimators/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/preprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 sklearn2pmml/preprocessing/h2o/
--rw-rw-r--  2.0 unx      679 b- defN 23-May-17 09:50 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx     5710 b- defN 23-May-17 09:50 h2o/estimators/H2OEstimator.class
--rw-rw-r--  2.0 unx     1694 b- defN 23-May-17 09:50 sklearn2pmml/preprocessing/h2o/H2OFrameConstructor.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn-h2o/
--rw-rw-r--  2.0 unx     1305 b- defN 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.xml
--rw-rw-r--  2.0 unx      112 b- defN 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.properties
-15 files, 9630 bytes uncompressed, 4316 bytes compressed:  55.2%
+Zip file size: 6333 bytes, number of entries: 15
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Jun-06 10:35 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 h2o/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 h2o/estimators/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/preprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/preprocessing/h2o/
+-rw-rw-r--  2.0 unx      679 b- defN 23-Jun-06 10:35 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx     5710 b- defN 23-Jun-06 10:35 h2o/estimators/H2OEstimator.class
+-rw-rw-r--  2.0 unx     1694 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/h2o/H2OFrameConstructor.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn-h2o/
+-rw-rw-r--  2.0 unx     1305 b- defN 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.xml
+-rw-rw-r--  2.0 unx      112 b- defN 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.properties
+15 files, 9630 bytes uncompressed, 4317 bytes compressed:  55.2%
```

#### META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.28</version>
+    <version>1.7.29</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-h2o</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn H2O.ai converter</name>
   <description>JPMML Scikit-Learn H2O.ai to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Wed May 17 09:50:31 EEST 2023
-version=1.7.28
+#Tue Jun 06 10:35:43 EEST 2023
+version=1.7.29
 groupId=org.jpmml
 artifactId=pmml-sklearn-h2o
```

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-xgboost-1.7.3.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-xgboost-1.7.3.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/serpent-1.40.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/serpent-1.40.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.28.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.29.jar`

 * *Files 15% similar despite different names*

#### zipinfo {}

```diff
@@ -1,17 +1,17 @@
 Zip file size: 7312 bytes, number of entries: 15
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-May-17 09:50 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 lightgbm/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 09:50 lightgbm/sklearn/
--rw-rw-r--  2.0 unx      177 b- defN 23-May-17 09:50 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx      170 b- defN 23-May-17 09:50 lightgbm/sklearn/HasBooster.class
--rw-rw-r--  2.0 unx     1953 b- defN 23-May-17 09:50 lightgbm/sklearn/Booster.class
--rw-rw-r--  2.0 unx     2102 b- defN 23-May-17 09:50 lightgbm/sklearn/LGBMRegressor.class
--rw-rw-r--  2.0 unx     2126 b- defN 23-May-17 09:50 lightgbm/sklearn/LGBMClassifier.class
--rw-rw-r--  2.0 unx     3298 b- defN 23-May-17 09:50 lightgbm/sklearn/BoosterUtil.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/
--rw-rw-r--  2.0 unx     1319 b- defN 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml
--rw-rw-r--  2.0 unx      117 b- defN 23-May-17 09:50 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.properties
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Jun-06 10:35 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 lightgbm/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 lightgbm/sklearn/
+-rw-rw-r--  2.0 unx      177 b- defN 23-Jun-06 10:35 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx      170 b- defN 23-Jun-06 10:35 lightgbm/sklearn/HasBooster.class
+-rw-rw-r--  2.0 unx     1953 b- defN 23-Jun-06 10:35 lightgbm/sklearn/Booster.class
+-rw-rw-r--  2.0 unx     2102 b- defN 23-Jun-06 10:35 lightgbm/sklearn/LGBMRegressor.class
+-rw-rw-r--  2.0 unx     2126 b- defN 23-Jun-06 10:35 lightgbm/sklearn/LGBMClassifier.class
+-rw-rw-r--  2.0 unx     3298 b- defN 23-Jun-06 10:35 lightgbm/sklearn/BoosterUtil.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/
+-rw-rw-r--  2.0 unx     1319 b- defN 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml
+-rw-rw-r--  2.0 unx      117 b- defN 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.properties
 15 files, 11392 bytes uncompressed, 5232 bytes compressed:  54.1%
```

#### META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.28</version>
+    <version>1.7.29</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-lightgbm</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn LightGBM converter</name>
   <description>JPMML Scikit-Learn LightGBM to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Wed May 17 09:50:31 EEST 2023
-version=1.7.28
+#Tue Jun 06 10:35:43 EEST 2023
+version=1.7.29
 groupId=org.jpmml
 artifactId=pmml-sklearn-lightgbm
```

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/jakarta.activation-2.0.1.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/jakarta.activation-2.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/resources/gson-2.10.jar` & `sklearn2pmml-0.93.0/sklearn2pmml/resources/gson-2.10.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/preprocessing/h2o.py` & `sklearn2pmml-0.93.0/sklearn2pmml/preprocessing/h2o.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/preprocessing/__init__.py` & `sklearn2pmml-0.93.0/sklearn2pmml/preprocessing/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -406,35 +406,43 @@
 		transform_dict = self._transform_dict()
 		# See https://stackoverflow.com/a/3460747
 		# See https://stackoverflow.com/a/3338368
 		func = lambda k: transform_dict[tuple(k) if isinstance(k, Hashable) else tuple(numpy.squeeze(numpy.asarray(k)))]
 		Xt = eval_rows(X, func)
 		return _col2d(Xt)
 
+def _make_index(values):
+	result = {}
+	for i, v in enumerate(list(values)):
+		result[v] = i
+	if len(result) != len(values):
+		raise ValueError()
+	return result
+
 class PMMLLabelBinarizer(BaseEstimator, TransformerMixin):
 	"""Binarize categorical data in a missing value-aware way."""
 
 	def __init__(self, sparse_output = False):
 		self.sparse_output = sparse_output
 
 	def fit(self, X, y = None):
 		X = ensure_1d(X)
 		self.classes_ = numpy.unique(X[~pandas.isnull(X)])
 		return self
 
 	def transform(self, X):
 		X = ensure_1d(X)
-		index = list(self.classes_)
+		mapping = _make_index(self.classes_)
 		if self.sparse_output:
-			Xt = lil_matrix((len(X), len(index)), dtype = int)
+			Xt = lil_matrix((len(X), len(mapping)), dtype = int)
 		else:
-			Xt = numpy.zeros((len(X), len(index)), dtype = int)
+			Xt = numpy.zeros((len(X), len(mapping)), dtype = int)
 		for i, v in enumerate(X):
-			if pandas.notnull(v):
-				Xt[i, index.index(v)] = 1
+			if (pandas.notnull(v)) and (v in mapping):
+				Xt[i, mapping[v]] = 1
 		if self.sparse_output:
 			Xt = Xt.tocsr()
 		return Xt
 
 class PMMLLabelEncoder(BaseEstimator, TransformerMixin):
 	"""Encode categorical data in a missing value-aware way."""
 
@@ -444,16 +452,16 @@
 	def fit(self, X, y = None):
 		X = ensure_1d(X)
 		self.classes_ = numpy.unique(X[~pandas.isnull(X)])
 		return self
 
 	def transform(self, X):
 		X = ensure_1d(X)
-		index = list(self.classes_)
-		Xt = numpy.array([self.missing_values if pandas.isnull(v) else index.index(v) for v in X])
+		mapping = _make_index(self.classes_)
+		Xt = numpy.array([self.missing_values if pandas.isnull(v) else mapping.get(v, self.missing_values) for v in X])
 		return _col2d(Xt)
 
 class PowerFunctionTransformer(BaseEstimator, TransformerMixin):
 	"""Raise numeric data to power."""
 
 	def __init__(self, power):
 		if not isinstance(power, int):
```

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/preprocessing/xgboost.py` & `sklearn2pmml-0.93.0/sklearn2pmml/preprocessing/xgboost.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/preprocessing/lightgbm.py` & `sklearn2pmml-0.93.0/sklearn2pmml/preprocessing/lightgbm.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/tree/chaid.py` & `sklearn2pmml-0.93.0/sklearn2pmml/tree/chaid.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.2/sklearn2pmml/expression/__init__.py` & `sklearn2pmml-0.93.0/sklearn2pmml/expression/__init__.py`

 * *Files identical despite different names*

