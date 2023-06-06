# Comparing `tmp/a2-0.3.6.tar.gz` & `tmp/a2-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a2-0.3.6.tar", max compression
+gzip compressed data, was "a2-0.3.7.tar", max compression
```

## Comparing `a2-0.3.6.tar` & `a2-0.3.7.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     3941 2023-06-06 16:29:51.630832 a2-0.3.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-20 15:29:54.345253 a2-0.3.6/src/a2/__init__.py
--rw-r--r--   0        0        0       45 2023-01-13 09:43:31.404482 a2-0.3.6/src/a2/cli/__init__.py
--rw-r--r--   0        0        0       39 2023-01-13 09:45:19.522669 a2-0.3.6/src/a2/cli/cli_plotting/__init__.py
--rw-r--r--   0        0        0      107 2023-01-13 09:46:23.599985 a2-0.3.6/src/a2/cli/cli_plotting/plot.py
--rw-r--r--   0        0        0     2056 2023-02-16 10:12:08.320539 a2-0.3.6/src/a2/cli/cli_plotting/single_plots.py
--rw-r--r--   0        0        0       66 2023-01-13 09:36:10.235731 a2-0.3.6/src/a2/cli/main.py
--rw-r--r--   0        0        0        0 2022-11-01 14:44:14.720032 a2-0.3.6/src/a2/data/__init__.py
--rw-r--r--   0        0        0        0 2022-11-01 14:44:14.720032 a2-0.3.6/src/a2/data/emoji/__init__.py
--rw-r--r--   0        0        0   379747 2022-11-01 14:44:14.724032 a2-0.3.6/src/a2/data/emoji/emoji_df.csv
--rw-r--r--   0        0        0        0 2022-11-01 14:44:14.724032 a2-0.3.6/src/a2/data/vocabularies/__init__.py
--rw-r--r--   0        0        0     2789 2023-02-21 08:27:21.563839 a2-0.3.6/src/a2/data/vocabularies/weather_vocab_enchanted_learning_com.txt
--rw-r--r--   0        0        0      236 2023-02-21 08:27:21.563869 a2-0.3.6/src/a2/data/vocabularies/weather_vocab_enchanted_precipitation.txt
--rw-r--r--   0        0        0      188 2023-02-21 14:04:17.568649 a2-0.3.6/src/a2/dataset/__init__.py
--rw-r--r--   0        0        0      556 2023-01-30 14:59:51.635141 a2-0.3.6/src/a2/dataset/emojis.py
--rw-r--r--   0        0        0     8227 2023-06-06 16:23:55.890263 a2-0.3.6/src/a2/dataset/load_dataset.py
--rw-r--r--   0        0        0    50068 2023-01-30 14:59:51.635141 a2-0.3.6/src/a2/dataset/radar.py
--rw-r--r--   0        0        0    10354 2023-01-30 14:59:51.635141 a2-0.3.6/src/a2/dataset/stations.py
--rw-r--r--   0        0        0      699 2023-02-20 13:53:30.152744 a2-0.3.6/src/a2/dataset/tweets.py
--rw-r--r--   0        0        0     1464 2022-12-14 09:36:33.150856 a2-0.3.6/src/a2/dataset/units.py
--rw-r--r--   0        0        0    17623 2023-06-06 13:09:51.493718 a2-0.3.6/src/a2/dataset/utils_dataset.py
--rw-r--r--   0        0        0      191 2022-12-14 09:36:33.150856 a2-0.3.6/src/a2/plotting/__init__.py
--rw-r--r--   0        0        0     8164 2023-05-12 12:06:36.401113 a2-0.3.6/src/a2/plotting/analysis.py
--rw-r--r--   0        0        0     1964 2023-02-14 14:11:41.262470 a2-0.3.6/src/a2/plotting/axes_utils.py
--rw-r--r--   0        0        0    30638 2023-05-16 11:22:03.945363 a2-0.3.6/src/a2/plotting/histograms.py
--rw-r--r--   0        0        0     3007 2022-12-14 09:36:33.154856 a2-0.3.6/src/a2/plotting/parallel_plotting.py
--rw-r--r--   0        0        0     2809 2022-12-14 09:36:33.154856 a2-0.3.6/src/a2/plotting/timeseries.py
--rw-r--r--   0        0        0    16218 2023-05-12 12:06:36.401113 a2-0.3.6/src/a2/plotting/utils_plotting.py
--rw-r--r--   0        0        0    34741 2023-02-20 13:53:30.156744 a2-0.3.6/src/a2/plotting/weather_maps.py
--rw-r--r--   0        0        0       67 2022-11-01 14:44:14.724032 a2-0.3.6/src/a2/preprocess/__init__.py
--rw-r--r--   0        0        0     3645 2022-12-06 08:38:01.708129 a2-0.3.6/src/a2/preprocess/embedding.py
--rw-r--r--   0        0        0    30389 2023-05-12 12:06:33.277030 a2-0.3.6/src/a2/preprocess/normalize_text.py
--rw-r--r--   0        0        0      172 2023-05-12 12:06:13.512505 a2-0.3.6/src/a2/training/__init__.py
--rw-r--r--   0        0        0     3889 2023-05-12 12:12:57.271066 a2-0.3.6/src/a2/training/benchmarks.py
--rw-r--r--   0        0        0     2863 2023-06-06 15:14:17.260894 a2-0.3.6/src/a2/training/dataset_hugging.py
--rw-r--r--   0        0        0     4213 2023-06-06 15:45:58.319253 a2-0.3.6/src/a2/training/evaluate_hugging.py
--rw-r--r--   0        0        0     4563 2023-06-06 15:48:04.766178 a2-0.3.6/src/a2/training/tracking.py
--rw-r--r--   0        0        0     1780 2023-05-12 12:06:13.512505 a2-0.3.6/src/a2/training/tracking_hugging.py
--rw-r--r--   0        0        0     6390 2023-05-12 12:06:13.512505 a2-0.3.6/src/a2/training/training_deep500.py
--rw-r--r--   0        0        0    11299 2023-06-06 14:58:39.420340 a2-0.3.6/src/a2/training/training_hugging.py
--rw-r--r--   0        0        0     6821 2023-05-12 12:06:33.277030 a2-0.3.6/src/a2/training/training_performance.py
--rw-r--r--   0        0        0       73 2023-01-30 14:59:51.639141 a2-0.3.6/src/a2/training/utils_training.py
--rw-r--r--   0        0        0       87 2022-11-01 14:44:14.728032 a2-0.3.6/src/a2/twitter/__init__.py
--rw-r--r--   0        0        0     4570 2023-02-20 13:53:30.156744 a2-0.3.6/src/a2/twitter/downloader.py
--rw-r--r--   0        0        0    11489 2023-06-06 13:55:59.732319 a2-0.3.6/src/a2/twitter/locations.py
--rw-r--r--   0        0        0     6765 2023-02-20 13:53:30.156744 a2-0.3.6/src/a2/twitter/twitter_api.py
--rw-r--r--   0        0        0      196 2023-06-06 12:24:26.982480 a2-0.3.6/src/a2/utils/__init__.py
--rw-r--r--   0        0        0     8658 2023-06-06 16:22:16.123856 a2-0.3.6/src/a2/utils/argparse.py
--rw-r--r--   0        0        0      518 2023-05-11 10:46:59.965258 a2-0.3.6/src/a2/utils/checks.py
--rw-r--r--   0        0        0      362 2023-02-20 15:01:52.076201 a2-0.3.6/src/a2/utils/constants.py
--rw-r--r--   0        0        0     9361 2023-06-06 14:01:17.485564 a2-0.3.6/src/a2/utils/file_handling.py
--rw-r--r--   0        0        0       90 2023-05-12 12:06:33.277030 a2-0.3.6/src/a2/utils/strings.py
--rw-r--r--   0        0        0     5327 2023-05-12 12:06:33.277030 a2-0.3.6/src/a2/utils/testing.py
--rw-r--r--   0        0        0      394 2022-12-14 09:36:33.154856 a2-0.3.6/src/a2/utils/times.py
--rw-r--r--   0        0        0     6088 2023-05-12 12:06:36.405113 a2-0.3.6/src/a2/utils/utils.py
--rw-r--r--   0        0        0     1918 1970-01-01 00:00:00.000000 a2-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     3941 2023-06-06 16:39:04.054525 a2-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-20 15:29:54.345253 a2-0.3.7/src/a2/__init__.py
+-rw-r--r--   0        0        0       45 2023-01-13 09:43:31.404482 a2-0.3.7/src/a2/cli/__init__.py
+-rw-r--r--   0        0        0       39 2023-01-13 09:45:19.522669 a2-0.3.7/src/a2/cli/cli_plotting/__init__.py
+-rw-r--r--   0        0        0      107 2023-01-13 09:46:23.599985 a2-0.3.7/src/a2/cli/cli_plotting/plot.py
+-rw-r--r--   0        0        0     2056 2023-02-16 10:12:08.320539 a2-0.3.7/src/a2/cli/cli_plotting/single_plots.py
+-rw-r--r--   0        0        0       66 2023-01-13 09:36:10.235731 a2-0.3.7/src/a2/cli/main.py
+-rw-r--r--   0        0        0        0 2022-11-01 14:44:14.720032 a2-0.3.7/src/a2/data/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-01 14:44:14.720032 a2-0.3.7/src/a2/data/emoji/__init__.py
+-rw-r--r--   0        0        0   379747 2022-11-01 14:44:14.724032 a2-0.3.7/src/a2/data/emoji/emoji_df.csv
+-rw-r--r--   0        0        0        0 2022-11-01 14:44:14.724032 a2-0.3.7/src/a2/data/vocabularies/__init__.py
+-rw-r--r--   0        0        0     2789 2023-02-21 08:27:21.563839 a2-0.3.7/src/a2/data/vocabularies/weather_vocab_enchanted_learning_com.txt
+-rw-r--r--   0        0        0      236 2023-02-21 08:27:21.563869 a2-0.3.7/src/a2/data/vocabularies/weather_vocab_enchanted_precipitation.txt
+-rw-r--r--   0        0        0      188 2023-02-21 14:04:17.568649 a2-0.3.7/src/a2/dataset/__init__.py
+-rw-r--r--   0        0        0      556 2023-01-30 14:59:51.635141 a2-0.3.7/src/a2/dataset/emojis.py
+-rw-r--r--   0        0        0     8227 2023-06-06 16:23:55.890263 a2-0.3.7/src/a2/dataset/load_dataset.py
+-rw-r--r--   0        0        0    50068 2023-01-30 14:59:51.635141 a2-0.3.7/src/a2/dataset/radar.py
+-rw-r--r--   0        0        0    10354 2023-01-30 14:59:51.635141 a2-0.3.7/src/a2/dataset/stations.py
+-rw-r--r--   0        0        0      699 2023-02-20 13:53:30.152744 a2-0.3.7/src/a2/dataset/tweets.py
+-rw-r--r--   0        0        0     1464 2022-12-14 09:36:33.150856 a2-0.3.7/src/a2/dataset/units.py
+-rw-r--r--   0        0        0    17623 2023-06-06 13:09:51.493718 a2-0.3.7/src/a2/dataset/utils_dataset.py
+-rw-r--r--   0        0        0      191 2022-12-14 09:36:33.150856 a2-0.3.7/src/a2/plotting/__init__.py
+-rw-r--r--   0        0        0     8164 2023-05-12 12:06:36.401113 a2-0.3.7/src/a2/plotting/analysis.py
+-rw-r--r--   0        0        0     1964 2023-02-14 14:11:41.262470 a2-0.3.7/src/a2/plotting/axes_utils.py
+-rw-r--r--   0        0        0    30638 2023-05-16 11:22:03.945363 a2-0.3.7/src/a2/plotting/histograms.py
+-rw-r--r--   0        0        0     3007 2022-12-14 09:36:33.154856 a2-0.3.7/src/a2/plotting/parallel_plotting.py
+-rw-r--r--   0        0        0     2809 2022-12-14 09:36:33.154856 a2-0.3.7/src/a2/plotting/timeseries.py
+-rw-r--r--   0        0        0    16218 2023-05-12 12:06:36.401113 a2-0.3.7/src/a2/plotting/utils_plotting.py
+-rw-r--r--   0        0        0    34741 2023-02-20 13:53:30.156744 a2-0.3.7/src/a2/plotting/weather_maps.py
+-rw-r--r--   0        0        0       67 2022-11-01 14:44:14.724032 a2-0.3.7/src/a2/preprocess/__init__.py
+-rw-r--r--   0        0        0     3645 2022-12-06 08:38:01.708129 a2-0.3.7/src/a2/preprocess/embedding.py
+-rw-r--r--   0        0        0    30389 2023-05-12 12:06:33.277030 a2-0.3.7/src/a2/preprocess/normalize_text.py
+-rw-r--r--   0        0        0      172 2023-05-12 12:06:13.512505 a2-0.3.7/src/a2/training/__init__.py
+-rw-r--r--   0        0        0     3889 2023-05-12 12:12:57.271066 a2-0.3.7/src/a2/training/benchmarks.py
+-rw-r--r--   0        0        0     2863 2023-06-06 15:14:17.260894 a2-0.3.7/src/a2/training/dataset_hugging.py
+-rw-r--r--   0        0        0     4213 2023-06-06 15:45:58.319253 a2-0.3.7/src/a2/training/evaluate_hugging.py
+-rw-r--r--   0        0        0     4563 2023-06-06 15:48:04.766178 a2-0.3.7/src/a2/training/tracking.py
+-rw-r--r--   0        0        0     1780 2023-05-12 12:06:13.512505 a2-0.3.7/src/a2/training/tracking_hugging.py
+-rw-r--r--   0        0        0     6390 2023-05-12 12:06:13.512505 a2-0.3.7/src/a2/training/training_deep500.py
+-rw-r--r--   0        0        0    11299 2023-06-06 14:58:39.420340 a2-0.3.7/src/a2/training/training_hugging.py
+-rw-r--r--   0        0        0     6821 2023-05-12 12:06:33.277030 a2-0.3.7/src/a2/training/training_performance.py
+-rw-r--r--   0        0        0       73 2023-01-30 14:59:51.639141 a2-0.3.7/src/a2/training/utils_training.py
+-rw-r--r--   0        0        0       87 2022-11-01 14:44:14.728032 a2-0.3.7/src/a2/twitter/__init__.py
+-rw-r--r--   0        0        0     4570 2023-02-20 13:53:30.156744 a2-0.3.7/src/a2/twitter/downloader.py
+-rw-r--r--   0        0        0    11489 2023-06-06 13:55:59.732319 a2-0.3.7/src/a2/twitter/locations.py
+-rw-r--r--   0        0        0     6765 2023-02-20 13:53:30.156744 a2-0.3.7/src/a2/twitter/twitter_api.py
+-rw-r--r--   0        0        0      196 2023-06-06 12:24:26.982480 a2-0.3.7/src/a2/utils/__init__.py
+-rw-r--r--   0        0        0     8662 2023-06-06 16:36:35.562037 a2-0.3.7/src/a2/utils/argparse.py
+-rw-r--r--   0        0        0      518 2023-05-11 10:46:59.965258 a2-0.3.7/src/a2/utils/checks.py
+-rw-r--r--   0        0        0      362 2023-02-20 15:01:52.076201 a2-0.3.7/src/a2/utils/constants.py
+-rw-r--r--   0        0        0     9361 2023-06-06 14:01:17.485564 a2-0.3.7/src/a2/utils/file_handling.py
+-rw-r--r--   0        0        0       90 2023-05-12 12:06:33.277030 a2-0.3.7/src/a2/utils/strings.py
+-rw-r--r--   0        0        0     5327 2023-05-12 12:06:33.277030 a2-0.3.7/src/a2/utils/testing.py
+-rw-r--r--   0        0        0      394 2022-12-14 09:36:33.154856 a2-0.3.7/src/a2/utils/times.py
+-rw-r--r--   0        0        0     6088 2023-05-12 12:06:36.405113 a2-0.3.7/src/a2/utils/utils.py
+-rw-r--r--   0        0        0     1918 1970-01-01 00:00:00.000000 a2-0.3.7/PKG-INFO
```

### Comparing `a2-0.3.6/pyproject.toml` & `a2-0.3.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "a2"
-version = "0.3.6"
+version = "0.3.7"
 description = "Package for predicting information about the weather from social media data as application 2 for maelstrom project"
 authors = ["Kristian Ehlert <kristian.ehlert@4-cast.de>"]
 packages = [{ include = "a2", from = "src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 jupyterlab = "^3.4.3"
```

### Comparing `a2-0.3.6/src/a2/cli/cli_plotting/single_plots.py` & `a2-0.3.7/src/a2/cli/cli_plotting/single_plots.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/data/emoji/emoji_df.csv` & `a2-0.3.7/src/a2/data/emoji/emoji_df.csv`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/data/vocabularies/weather_vocab_enchanted_learning_com.txt` & `a2-0.3.7/src/a2/data/vocabularies/weather_vocab_enchanted_learning_com.txt`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/dataset/emojis.py` & `a2-0.3.7/src/a2/dataset/emojis.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/dataset/load_dataset.py` & `a2-0.3.7/src/a2/dataset/load_dataset.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/dataset/radar.py` & `a2-0.3.7/src/a2/dataset/radar.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/dataset/stations.py` & `a2-0.3.7/src/a2/dataset/stations.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/dataset/tweets.py` & `a2-0.3.7/src/a2/dataset/tweets.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/dataset/units.py` & `a2-0.3.7/src/a2/dataset/units.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/dataset/utils_dataset.py` & `a2-0.3.7/src/a2/dataset/utils_dataset.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/plotting/analysis.py` & `a2-0.3.7/src/a2/plotting/analysis.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/plotting/axes_utils.py` & `a2-0.3.7/src/a2/plotting/axes_utils.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/plotting/histograms.py` & `a2-0.3.7/src/a2/plotting/histograms.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/plotting/parallel_plotting.py` & `a2-0.3.7/src/a2/plotting/parallel_plotting.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/plotting/timeseries.py` & `a2-0.3.7/src/a2/plotting/timeseries.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/plotting/utils_plotting.py` & `a2-0.3.7/src/a2/plotting/utils_plotting.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/plotting/weather_maps.py` & `a2-0.3.7/src/a2/plotting/weather_maps.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/preprocess/embedding.py` & `a2-0.3.7/src/a2/preprocess/embedding.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/preprocess/normalize_text.py` & `a2-0.3.7/src/a2/preprocess/normalize_text.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/training/benchmarks.py` & `a2-0.3.7/src/a2/training/benchmarks.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/training/dataset_hugging.py` & `a2-0.3.7/src/a2/training/dataset_hugging.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/training/evaluate_hugging.py` & `a2-0.3.7/src/a2/training/evaluate_hugging.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/training/tracking.py` & `a2-0.3.7/src/a2/training/tracking.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/training/tracking_hugging.py` & `a2-0.3.7/src/a2/training/tracking_hugging.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/training/training_deep500.py` & `a2-0.3.7/src/a2/training/training_deep500.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/training/training_hugging.py` & `a2-0.3.7/src/a2/training/training_hugging.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/training/training_performance.py` & `a2-0.3.7/src/a2/training/training_performance.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/twitter/downloader.py` & `a2-0.3.7/src/a2/twitter/downloader.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/twitter/locations.py` & `a2-0.3.7/src/a2/twitter/locations.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/twitter/twitter_api.py` & `a2-0.3.7/src/a2/twitter/twitter_api.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/utils/argparse.py` & `a2-0.3.7/src/a2/utils/argparse.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,17 +115,17 @@
         "--data_filename_irrelevant",
         type=str,
         default="2017_2020_tweets_rain_sun_vocab_emojis_locations_bba_Tp_era5_no_bots_normalized_filtered.nc",
         help="Filename of training data.",
     )
     parser.add_argument(
         "--n_tweets_irrelevant",
-        type=tuple[int, str],
-        default="all",
-        help='Number of irrelevant tweets used to create dataset, use all irrelevant tweets by default ("all").',
+        type=int,
+        default=-1,
+        help='Number of irrelevant tweets used to create dataset, use all irrelevant tweets by default (`n_tweets_irrelevant=-1`).',
     )
 
     parser.add_argument(
         "--key_relevance",
         type=str,
         default="relevant",
         help="Filename of training data.",
```

### Comparing `a2-0.3.6/src/a2/utils/checks.py` & `a2-0.3.7/src/a2/utils/checks.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/utils/file_handling.py` & `a2-0.3.7/src/a2/utils/file_handling.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/utils/testing.py` & `a2-0.3.7/src/a2/utils/testing.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/src/a2/utils/utils.py` & `a2-0.3.7/src/a2/utils/utils.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.6/PKG-INFO` & `a2-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a2
-Version: 0.3.6
+Version: 0.3.7
 Summary: Package for predicting information about the weather from social media data as application 2 for maelstrom project
 Author: Kristian Ehlert
 Author-email: kristian.ehlert@4-cast.de
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

