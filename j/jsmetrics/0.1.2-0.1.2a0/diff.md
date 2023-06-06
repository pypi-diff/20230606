# Comparing `tmp/jsmetrics-0.1.2.tar.gz` & `tmp/jsmetrics-0.1.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsmetrics-0.1.2.tar", last modified: Tue Jun  6 16:08:41 2023, max compression
+gzip compressed data, was "jsmetrics-0.1.2a0.tar", last modified: Sat May 27 11:23:57 2023, max compression
```

## Comparing `jsmetrics-0.1.2.tar` & `jsmetrics-0.1.2a0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:08:41.128729 jsmetrics-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20495 2023-06-06 16:08:41.128729 jsmetrics-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12787 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:08:41.112729 jsmetrics-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:08:41.108729 jsmetrics-0.1.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:08:41.116729 jsmetrics-0.1.2/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)  1083764 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/docs/_static/images/all_jet_lats_stj_pfj_npac_maps_more_metrics.png
--rw-r--r--   0 runner    (1001) docker     (123)   279496 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/docs/_static/images/all_metrics_jetlat_circbar_w_errorbars.png
--rw-r--r--   0 runner    (1001) docker     (123)  1519071 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/docs/_static/images/jet_core_algorithm_comparions_NA_5_texas2021.png
--rw-r--r--   0 runner    (1001) docker     (123)   788211 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/docs/_static/images/jet_shift_violin.png
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/docs/metrics.rst
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/docs/statement.rst
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:08:41.120729 jsmetrics-0.1.2/jsmetrics/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/jsmetrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:08:41.120729 jsmetrics-0.1.2/jsmetrics/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/jsmetrics/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/jsmetrics/core/check_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/jsmetrics/details_for_all_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:08:41.120729 jsmetrics-0.1.2/jsmetrics/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/jsmetrics/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/jsmetrics/metrics/jet_core_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)    26250 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/jsmetrics/metrics/jet_core_algorithms_components.py
--rw-r--r--   0 runner    (1001) docker     (123)    22927 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/jsmetrics/metrics/jet_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    42201 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/jsmetrics/metrics/jet_statistics_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/jsmetrics/metrics/waviness_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/jsmetrics/metrics/waviness_metrics_components.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:08:41.124729 jsmetrics-0.1.2/jsmetrics/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/jsmetrics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/jsmetrics/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/jsmetrics/utils/spatial_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/jsmetrics/utils/windspeed_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:08:41.120729 jsmetrics-0.1.2/jsmetrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20495 2023-06-06 16:08:41.000000 jsmetrics-0.1.2/jsmetrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-06 16:08:41.000000 jsmetrics-0.1.2/jsmetrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 16:08:41.000000 jsmetrics-0.1.2/jsmetrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 16:08:41.000000 jsmetrics-0.1.2/jsmetrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-06 16:08:41.000000 jsmetrics-0.1.2/jsmetrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-06 16:08:41.000000 jsmetrics-0.1.2/jsmetrics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-06 16:08:41.128729 jsmetrics-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:08:41.124729 jsmetrics-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:08:41.128729 jsmetrics-0.1.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1262096 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/tests/data/ua_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
--rw-r--r--   0 runner    (1001) docker     (123)  1260860 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/tests/data/va_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
--rw-r--r--   0 runner    (1001) docker     (123)  1104721 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/tests/data/zg_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:08:41.128729 jsmetrics-0.1.2/tests/metric_verification/
--rw-r--r--   0 runner    (1001) docker     (123)    13017 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/tests/metric_verification/metric_verification.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:08:41.128729 jsmetrics-0.1.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/tests/unit/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/tests/unit/test_jet_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/tests/unit/test_jet_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/tests/unit/test_spatial_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/tests/unit/test_waviness_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-06 16:08:35.000000 jsmetrics-0.1.2/tests/unit/test_windspeed_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.124666 jsmetrics-0.1.2a0/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20337 2023-05-27 11:23:57.124666 jsmetrics-0.1.2a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12787 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.116666 jsmetrics-0.1.2a0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.112666 jsmetrics-0.1.2a0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.116666 jsmetrics-0.1.2a0/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)  1083764 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/_static/images/all_jet_lats_stj_pfj_npac_maps_more_metrics.png
+-rw-r--r--   0 runner    (1001) docker     (123)   279496 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/_static/images/all_metrics_jetlat_circbar_w_errorbars.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1519071 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/_static/images/jet_core_algorithm_comparions_NA_5_texas2021.png
+-rw-r--r--   0 runner    (1001) docker     (123)   788211 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/_static/images/jet_shift_violin.png
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/metrics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/statement.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.116666 jsmetrics-0.1.2a0/jsmetrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.120666 jsmetrics-0.1.2a0/jsmetrics/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/core/check_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/details_for_all_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.120666 jsmetrics-0.1.2a0/jsmetrics/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/metrics/jet_core_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26250 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/metrics/jet_core_algorithms_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22302 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/metrics/jet_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42201 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/metrics/jet_statistics_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/metrics/waviness_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/metrics/waviness_metrics_components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.120666 jsmetrics-0.1.2a0/jsmetrics/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/utils/spatial_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/utils/windspeed_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.120666 jsmetrics-0.1.2a0/jsmetrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20337 2023-05-27 11:23:57.000000 jsmetrics-0.1.2a0/jsmetrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-27 11:23:57.000000 jsmetrics-0.1.2a0/jsmetrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 11:23:57.000000 jsmetrics-0.1.2a0/jsmetrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 11:23:57.000000 jsmetrics-0.1.2a0/jsmetrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-27 11:23:57.000000 jsmetrics-0.1.2a0/jsmetrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-27 11:23:57.000000 jsmetrics-0.1.2a0/jsmetrics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-27 11:23:57.124666 jsmetrics-0.1.2a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.120666 jsmetrics-0.1.2a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.124666 jsmetrics-0.1.2a0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1262096 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/data/ua_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
+-rw-r--r--   0 runner    (1001) docker     (123)  1260860 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/data/va_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
+-rw-r--r--   0 runner    (1001) docker     (123)  1104721 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/data/zg_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.124666 jsmetrics-0.1.2a0/tests/metric_verification/
+-rw-r--r--   0 runner    (1001) docker     (123)    13017 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/metric_verification/metric_verification.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.124666 jsmetrics-0.1.2a0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/unit/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/unit/test_jet_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/unit/test_jet_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/unit/test_spatial_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/unit/test_waviness_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/unit/test_windspeed_utils.py
```

### Comparing `jsmetrics-0.1.2/CONTRIBUTING.rst` & `jsmetrics-0.1.2a0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/HISTORY.rst` & `jsmetrics-0.1.2a0/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,12 @@
 =======
 History
 =======
 
 
-0.1.2 (2023-06-06)
--------------------------
-* Fix  Barnes & Polvani 2013 to better deal when min max jet lat is at edge data 
-* Add check for NoLeapDatetime
-
-
 0.1.2-alpha (2023-05-27)
 -------------------------
 * Add check for NoLeapDatetime
 
 
 0.1.1 (2023-05-26)
 -------------------------
```

### Comparing `jsmetrics-0.1.2/LICENSE` & `jsmetrics-0.1.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/PKG-INFO` & `jsmetrics-0.1.2a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsmetrics
-Version: 0.1.2
+Version: 0.1.2a0
 Summary: Library of algorithms and metrics used to characterise and/or identify jet-streams, based on xarray.
 Home-page: https://github.com/Thomasjkeel/jsmetrics
 Author: Thomas Keel
 Author-email: thomas.keel.18@ucl.ac.uk
 License: MIT License
 Keywords: jet-stream climate metrics algorithms xarray
 Platform: UNKNOWN
@@ -247,20 +247,14 @@
 
 
 =======
 History
 =======
 
 
-0.1.2 (2023-06-06)
--------------------------
-* Fix  Barnes & Polvani 2013 to better deal when min max jet lat is at edge data 
-* Add check for NoLeapDatetime
-
-
 0.1.2-alpha (2023-05-27)
 -------------------------
 * Add check for NoLeapDatetime
 
 
 0.1.1 (2023-05-26)
 -------------------------
```

### Comparing `jsmetrics-0.1.2/README.rst` & `jsmetrics-0.1.2a0/README.rst`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/docs/Makefile` & `jsmetrics-0.1.2a0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/docs/_static/images/all_jet_lats_stj_pfj_npac_maps_more_metrics.png` & `jsmetrics-0.1.2a0/docs/_static/images/all_jet_lats_stj_pfj_npac_maps_more_metrics.png`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/docs/_static/images/all_metrics_jetlat_circbar_w_errorbars.png` & `jsmetrics-0.1.2a0/docs/_static/images/all_metrics_jetlat_circbar_w_errorbars.png`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/docs/_static/images/jet_core_algorithm_comparions_NA_5_texas2021.png` & `jsmetrics-0.1.2a0/docs/_static/images/jet_core_algorithm_comparions_NA_5_texas2021.png`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/docs/_static/images/jet_shift_violin.png` & `jsmetrics-0.1.2a0/docs/_static/images/jet_shift_violin.png`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/docs/conf.py` & `jsmetrics-0.1.2a0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/docs/index.rst` & `jsmetrics-0.1.2a0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/docs/installation.rst` & `jsmetrics-0.1.2a0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/docs/make.bat` & `jsmetrics-0.1.2a0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/docs/metrics.rst` & `jsmetrics-0.1.2a0/docs/metrics.rst`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/jsmetrics/core/check_data.py` & `jsmetrics-0.1.2a0/jsmetrics/core/check_data.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/jsmetrics/details_for_all_metrics.py` & `jsmetrics-0.1.2a0/jsmetrics/details_for_all_metrics.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/jsmetrics/metrics/jet_core_algorithms.py` & `jsmetrics-0.1.2a0/jsmetrics/metrics/jet_core_algorithms.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/jsmetrics/metrics/jet_core_algorithms_components.py` & `jsmetrics-0.1.2a0/jsmetrics/metrics/jet_core_algorithms_components.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/jsmetrics/metrics/jet_statistics.py` & `jsmetrics-0.1.2a0/jsmetrics/metrics/jet_statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,27 +210,16 @@
                 scaled_ws,
             ) = jet_statistics_components.get_latitude_and_speed_where_max_ws_at_reduced_resolution(
                 max_lat_and_ws, lat_resolution=0.01
             )
             scaled_max_lats.append(scaled_max_lat)
             scaled_max_ws.append(scaled_ws)
         else:
-            if np.isnan(max_lat_and_ws).all():
-                scaled_max_lats.append(np.nan)
-                scaled_max_ws.append(np.nan)
-            else:
-                if np.nanmax(max_lat_and_ws[0]) == data["lat"].max():
-                    scaled_max_lats.append(np.nanmax(max_lat_and_ws[0]))
-                    scaled_max_ws.append(np.nanmax(max_lat_and_ws[1]))
-                elif np.nanmin(max_lat_and_ws[0]) == data["lat"].min():
-                    scaled_max_lats.append(np.nanmin(max_lat_and_ws[0]))
-                    scaled_max_ws.append(np.nanmin(max_lat_and_ws[1]))
-                else:
-                    scaled_max_lats.append(np.nan)
-                    scaled_max_ws.append(np.nan)
+            scaled_max_lats.append(np.nan)
+            scaled_max_ws.append(np.nan)
 
     #  Step 6. Get jet-widths using scaled windspeed and usual jet-lat
     max_lats = all_max_lats_and_ws[::, 0, 1]
     jet_widths = list(
         map(
             lambda zm, la, wa: jet_statistics_components.calc_jet_width_for_one_day(
                 zm, la, wa
```

### Comparing `jsmetrics-0.1.2/jsmetrics/metrics/jet_statistics_components.py` & `jsmetrics-0.1.2a0/jsmetrics/metrics/jet_statistics_components.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/jsmetrics/metrics/waviness_metrics.py` & `jsmetrics-0.1.2a0/jsmetrics/metrics/waviness_metrics.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/jsmetrics/metrics/waviness_metrics_components.py` & `jsmetrics-0.1.2a0/jsmetrics/metrics/waviness_metrics_components.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/jsmetrics/utils/data_utils.py` & `jsmetrics-0.1.2a0/jsmetrics/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/jsmetrics/utils/spatial_utils.py` & `jsmetrics-0.1.2a0/jsmetrics/utils/spatial_utils.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/jsmetrics/utils/windspeed_utils.py` & `jsmetrics-0.1.2a0/jsmetrics/utils/windspeed_utils.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/jsmetrics.egg-info/PKG-INFO` & `jsmetrics-0.1.2a0/jsmetrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsmetrics
-Version: 0.1.2
+Version: 0.1.2a0
 Summary: Library of algorithms and metrics used to characterise and/or identify jet-streams, based on xarray.
 Home-page: https://github.com/Thomasjkeel/jsmetrics
 Author: Thomas Keel
 Author-email: thomas.keel.18@ucl.ac.uk
 License: MIT License
 Keywords: jet-stream climate metrics algorithms xarray
 Platform: UNKNOWN
@@ -247,20 +247,14 @@
 
 
 =======
 History
 =======
 
 
-0.1.2 (2023-06-06)
--------------------------
-* Fix  Barnes & Polvani 2013 to better deal when min max jet lat is at edge data 
-* Add check for NoLeapDatetime
-
-
 0.1.2-alpha (2023-05-27)
 -------------------------
 * Add check for NoLeapDatetime
 
 
 0.1.1 (2023-05-26)
 -------------------------
```

### Comparing `jsmetrics-0.1.2/jsmetrics.egg-info/SOURCES.txt` & `jsmetrics-0.1.2a0/jsmetrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/setup.cfg` & `jsmetrics-0.1.2a0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.2
+current_version = 0.1.2-alpha
 commit = True
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+).(?P<patch>\d+)(\-(?P<release>[a-z]+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}
 	{major}.{minor}.{patch}
```

### Comparing `jsmetrics-0.1.2/setup.py` & `jsmetrics-0.1.2a0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 NAME = "jsmetrics"
 DESCRIPTION = "Library of algorithms and metrics used to characterise and/or identify jet-streams, based on xarray."
 URL = "https://github.com/Thomasjkeel/jsmetrics"
 AUTHOR = "Thomas Keel"
 AUTHOR_EMAIL = "thomas.keel.18@ucl.ac.uk"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "0.1.2"
+VERSION = "0.1.2-alpha"
 LICENSE = "MIT License"
 
 KEYWORDS = "jet-stream climate metrics algorithms xarray"
 
 with open("README.rst") as file:
     readme = file.read()
```

### Comparing `jsmetrics-0.1.2/tests/data/ua_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc` & `jsmetrics-0.1.2a0/tests/data/ua_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/tests/data/va_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc` & `jsmetrics-0.1.2a0/tests/data/va_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/tests/data/zg_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc` & `jsmetrics-0.1.2a0/tests/data/zg_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/tests/metric_verification/metric_verification.ipynb` & `jsmetrics-0.1.2a0/tests/metric_verification/metric_verification.ipynb`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/tests/unit/__init__.py` & `jsmetrics-0.1.2a0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/tests/unit/test_data_utils.py` & `jsmetrics-0.1.2a0/tests/unit/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/tests/unit/test_jet_algorithms.py` & `jsmetrics-0.1.2a0/tests/unit/test_jet_algorithms.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/tests/unit/test_jet_statistics.py` & `jsmetrics-0.1.2a0/tests/unit/test_jet_statistics.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/tests/unit/test_spatial_utils.py` & `jsmetrics-0.1.2a0/tests/unit/test_spatial_utils.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/tests/unit/test_waviness_metrics.py` & `jsmetrics-0.1.2a0/tests/unit/test_waviness_metrics.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2/tests/unit/test_windspeed_utils.py` & `jsmetrics-0.1.2a0/tests/unit/test_windspeed_utils.py`

 * *Files identical despite different names*

