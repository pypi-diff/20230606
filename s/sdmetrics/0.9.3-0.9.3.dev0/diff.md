# Comparing `tmp/sdmetrics-0.9.3.tar.gz` & `tmp/sdmetrics-0.9.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdmetrics-0.9.3.tar", last modified: Wed Apr 12 18:26:28 2023, max compression
+gzip compressed data, was "sdmetrics-0.9.3.dev0.tar", last modified: Tue Apr 11 17:54:06 2023, max compression
```

## Comparing `sdmetrics-0.9.3.tar` & `sdmetrics-0.9.3.dev0.tar`

### file list

```diff
@@ -1,213 +1,213 @@
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.170883 sdmetrics-0.9.3/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)      142 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/AUTHORS.rst
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     8364 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/CONTRIBUTING.rst
--rw-r--r--   0 romain_datacebo   (501) staff       (20)    18394 2023-04-12 18:26:18.000000 sdmetrics-0.9.3/HISTORY.md
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     1077 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/LICENSE
--rw-r--r--   0 romain_datacebo   (501) staff       (20)      295 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/MANIFEST.in
--rw-r--r--   0 romain_datacebo   (501) staff       (20)    24539 2023-04-12 18:26:28.171074 sdmetrics-0.9.3/PKG-INFO
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     5223 2023-04-12 09:05:56.000000 sdmetrics-0.9.3/README.md
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.134370 sdmetrics-0.9.3/docs/
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.142030 sdmetrics-0.9.3/docs/images/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)   181646 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/docs/images/column_comparison.png
--rw-r--r--   0 romain_datacebo   (501) staff       (20)   222559 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/docs/images/column_pairs.png
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.144143 sdmetrics-0.9.3/sdmetrics/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     2194 2023-04-12 18:26:18.000000 sdmetrics-0.9.3/sdmetrics/__init__.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)      825 2023-04-12 18:26:18.000000 sdmetrics-0.9.3/sdmetrics/_addons.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     3344 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/base.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.146497 sdmetrics-0.9.3/sdmetrics/column_pairs/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)      551 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/column_pairs/__init__.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     1867 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/column_pairs/base.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.147046 sdmetrics-0.9.3/sdmetrics/column_pairs/statistical/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)      480 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/column_pairs/statistical/__init__.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     3367 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/column_pairs/statistical/contingency_similarity.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     5256 2023-04-12 18:26:18.000000 sdmetrics-0.9.3/sdmetrics/column_pairs/statistical/correlation_similarity.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     4418 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/column_pairs/statistical/kl_divergence.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.148482 sdmetrics-0.9.3/sdmetrics/demos/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     8013 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/demos/multi_table.pkl
--rw-r--r--   0 romain_datacebo   (501) staff       (20)    48099 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/demos/single_table.pkl
--rw-r--r--   0 romain_datacebo   (501) staff       (20)    61272 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/demos/timeseries.pkl
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     2451 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/demos.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)      130 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/errors.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)      300 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/goal.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.150178 sdmetrics-0.9.3/sdmetrics/multi_table/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     1611 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/multi_table/__init__.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     1447 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/multi_table/base.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.150829 sdmetrics-0.9.3/sdmetrics/multi_table/detection/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)       71 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/multi_table/detection/__init__.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     2018 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/multi_table/detection/base.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     4619 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/multi_table/detection/parent_child.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)    10713 2023-04-12 18:26:18.000000 sdmetrics-0.9.3/sdmetrics/multi_table/multi_single_table.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.151256 sdmetrics-0.9.3/sdmetrics/multi_table/statistical/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)      352 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/multi_table/statistical/__init__.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     5932 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/multi_table/statistical/cardinality_shape_similarity.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     8484 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/multi_table/statistical/cardinality_statistic_similarity.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.151511 sdmetrics-0.9.3/sdmetrics/reports/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)      169 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/reports/__init__.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.152033 sdmetrics-0.9.3/sdmetrics/reports/multi_table/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)      250 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/reports/multi_table/__init__.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)    11069 2023-04-12 18:26:18.000000 sdmetrics-0.9.3/sdmetrics/reports/multi_table/diagnostic_report.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     2081 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/reports/multi_table/plot_utils.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)    14805 2023-04-12 18:26:18.000000 sdmetrics-0.9.3/sdmetrics/reports/multi_table/quality_report.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.152516 sdmetrics-0.9.3/sdmetrics/reports/single_table/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)      253 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/reports/single_table/__init__.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     9171 2023-04-12 18:26:18.000000 sdmetrics-0.9.3/sdmetrics/reports/single_table/diagnostic_report.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)    12880 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/reports/single_table/plot_utils.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)    10073 2023-04-12 18:26:18.000000 sdmetrics-0.9.3/sdmetrics/reports/single_table/quality_report.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)    24960 2023-04-12 18:26:18.000000 sdmetrics-0.9.3/sdmetrics/reports/utils.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.152766 sdmetrics-0.9.3/sdmetrics/single_column/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     1011 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_column/__init__.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     1938 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_column/base.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.153871 sdmetrics-0.9.3/sdmetrics/single_column/statistical/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)      878 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_column/statistical/__init__.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     2130 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_column/statistical/boundary_adherence.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     2805 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_column/statistical/category_coverage.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     2120 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_column/statistical/cstest.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     2483 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_column/statistical/kscomplement.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     2748 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_column/statistical/missing_value_similarity.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     2332 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_column/statistical/range_coverage.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     3694 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_column/statistical/statistic_similarity.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     2124 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_column/statistical/tv_complement.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.154733 sdmetrics-0.9.3/sdmetrics/single_table/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     3636 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_table/__init__.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     7241 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_table/base.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     8748 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_table/bayesian_network.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.155098 sdmetrics-0.9.3/sdmetrics/single_table/detection/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)      213 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_table/detection/__init__.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     4297 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_table/detection/base.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     2355 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_table/detection/sklearn.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.155818 sdmetrics-0.9.3/sdmetrics/single_table/efficacy/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     1059 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_table/efficacy/__init__.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     4848 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_table/efficacy/base.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     3062 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_table/efficacy/binary.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     3897 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_table/efficacy/mlefficacy.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     1816 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_table/efficacy/multiclass.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     1412 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_table/efficacy/regression.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     6597 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_table/gaussian_mixture.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     9447 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_table/multi_column_pairs.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     9136 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_table/multi_single_column.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     7518 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_table/new_row_synthesis.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.156933 sdmetrics-0.9.3/sdmetrics/single_table/privacy/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     1021 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_table/privacy/__init__.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)    13909 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_table/privacy/base.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     6127 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_table/privacy/cap.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     7982 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_table/privacy/categorical_sklearn.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     4255 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_table/privacy/ensemble.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     2703 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_table/privacy/loss.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     4151 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_table/privacy/numerical_sklearn.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     4733 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_table/privacy/radius_nearest_neighbor.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     3737 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/single_table/privacy/util.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.157409 sdmetrics-0.9.3/sdmetrics/timeseries/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)      615 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/timeseries/__init__.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     3048 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/timeseries/base.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     3919 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/timeseries/detection.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.157778 sdmetrics-0.9.3/sdmetrics/timeseries/efficacy/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)      380 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/timeseries/efficacy/__init__.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     4195 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/timeseries/efficacy/base.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)      526 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/timeseries/efficacy/classification.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     2138 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/sdmetrics/timeseries/ml_scorers.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     8766 2023-04-12 18:26:18.000000 sdmetrics-0.9.3/sdmetrics/utils.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)      306 2023-04-12 18:26:18.000000 sdmetrics-0.9.3/sdmetrics/warnings.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.146215 sdmetrics-0.9.3/sdmetrics.egg-info/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)    24539 2023-04-12 18:26:28.000000 sdmetrics-0.9.3/sdmetrics.egg-info/PKG-INFO
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     7062 2023-04-12 18:26:28.000000 sdmetrics-0.9.3/sdmetrics.egg-info/SOURCES.txt
--rw-r--r--   0 romain_datacebo   (501) staff       (20)        1 2023-04-12 18:26:28.000000 sdmetrics-0.9.3/sdmetrics.egg-info/dependency_links.txt
--rw-r--r--   0 romain_datacebo   (501) staff       (20)        1 2023-04-12 18:26:28.000000 sdmetrics-0.9.3/sdmetrics.egg-info/not-zip-safe
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     1636 2023-04-12 18:26:28.000000 sdmetrics-0.9.3/sdmetrics.egg-info/requires.txt
--rw-r--r--   0 romain_datacebo   (501) staff       (20)       10 2023-04-12 18:26:28.000000 sdmetrics-0.9.3/sdmetrics.egg-info/top_level.txt
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     1420 2023-04-12 18:26:28.171491 sdmetrics-0.9.3/setup.cfg
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     3712 2023-04-12 18:26:18.000000 sdmetrics-0.9.3/setup.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.158022 sdmetrics-0.9.3/tests/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)       33 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/__init__.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.158267 sdmetrics-0.9.3/tests/integration/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)       45 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/__init__.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.158387 sdmetrics-0.9.3/tests/integration/column_pairs/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)       65 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/column_pairs/__init__.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.158633 sdmetrics-0.9.3/tests/integration/column_pairs/statistical/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)       77 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/column_pairs/statistical/__init__.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     3736 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/column_pairs/statistical/test_kl_divergence.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.159242 sdmetrics-0.9.3/tests/integration/multi_table/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)       64 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/multi_table/__init__.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     2732 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/multi_table/test_multi_single_table.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)      581 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/multi_table/test_multi_table.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     3719 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/multi_table/test_parent_child.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     2932 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/multi_table/test_statistical_metrics.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.159364 sdmetrics-0.9.3/tests/integration/reports/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)       60 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/reports/__init__.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.159603 sdmetrics-0.9.3/tests/integration/reports/multi_table/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)       72 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/reports/multi_table/__init__.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     2578 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/reports/multi_table/test_multi_table_quality_report.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.160620 sdmetrics-0.9.3/tests/integration/reports/single_table/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)       73 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/reports/single_table/__init__.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     1823 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/reports/single_table/test_single_table_quality_report.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.160790 sdmetrics-0.9.3/tests/integration/single_column/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)       66 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/single_column/__init__.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.161790 sdmetrics-0.9.3/tests/integration/single_column/statistical/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)       66 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/single_column/statistical/__init__.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     1467 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/single_column/statistical/test_cstest.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     1509 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/single_column/statistical/test_kscomplement.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.162195 sdmetrics-0.9.3/tests/integration/single_table/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)       65 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/single_table/__init__.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.162704 sdmetrics-0.9.3/tests/integration/single_table/efficacy/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     2446 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/single_table/efficacy/test_binary.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     1283 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/single_table/efficacy/test_detection.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     1677 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/single_table/efficacy/test_multiclass.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     1898 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/single_table/efficacy/test_regression.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.162831 sdmetrics-0.9.3/tests/integration/single_table/privacy/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     6178 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/single_table/privacy/test_privacy.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     1717 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/single_table/test_gaussian_mixture.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     4308 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/single_table/test_single_table.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     1261 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/test_base.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.163082 sdmetrics-0.9.3/tests/integration/timeseries/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)       63 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/timeseries/__init__.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.163334 sdmetrics-0.9.3/tests/integration/timeseries/efficacy/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)       72 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/timeseries/efficacy/__init__.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)      778 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/timeseries/efficacy/test_classification.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     1354 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/integration/timeseries/test_timeseries.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.163959 sdmetrics-0.9.3/tests/unit/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)       38 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/unit/__init__.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.164210 sdmetrics-0.9.3/tests/unit/column_pairs/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)       46 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/unit/column_pairs/__init__.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.164603 sdmetrics-0.9.3/tests/unit/column_pairs/statistical/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)       59 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/unit/column_pairs/statistical/__init__.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     1515 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/unit/column_pairs/statistical/test_contingency_similarity.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     6305 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/unit/column_pairs/statistical/test_correlation_similarity.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)      818 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/unit/column_pairs/test_base.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.164734 sdmetrics-0.9.3/tests/unit/multi_table/
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.164990 sdmetrics-0.9.3/tests/unit/multi_table/statistical/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     6089 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/unit/multi_table/statistical/test_cardinality_shape_similarity.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     8127 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/unit/multi_table/statistical/test_cardinality_statistic_similarity.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     3642 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/unit/multi_table/test_multi_single_table.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.165114 sdmetrics-0.9.3/tests/unit/reports/
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.165547 sdmetrics-0.9.3/tests/unit/reports/multi_table/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)    24434 2023-04-12 18:26:18.000000 sdmetrics-0.9.3/tests/unit/reports/multi_table/test_multi_table_diagnostic_report.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     1881 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/unit/reports/multi_table/test_multi_table_plot_utils.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)    44827 2023-04-12 18:26:18.000000 sdmetrics-0.9.3/tests/unit/reports/multi_table/test_multi_table_quality_report.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.166851 sdmetrics-0.9.3/tests/unit/reports/single_table/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)    19753 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/unit/reports/single_table/test_single_table_diagnostic_report.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     8208 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/unit/reports/single_table/test_single_table_plot_utils.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)    31054 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/unit/reports/single_table/test_single_table_quality_report.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)    39408 2023-04-12 18:26:18.000000 sdmetrics-0.9.3/tests/unit/reports/test_utils.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.168242 sdmetrics-0.9.3/tests/unit/single_column/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)       47 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/unit/single_column/__init__.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.169311 sdmetrics-0.9.3/tests/unit/single_column/statistical/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)       60 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/unit/single_column/statistical/__init__.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     1361 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/unit/single_column/statistical/test_boundary_adherence.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     2848 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/unit/single_column/statistical/test_category_coverage.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     2378 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/unit/single_column/statistical/test_missing_value_similarity.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     2751 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/unit/single_column/statistical/test_range_coverage.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     3543 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/unit/single_column/statistical/test_statistic_similarity.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     1978 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/unit/single_column/statistical/test_tv_complement.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)      823 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/unit/single_column/test_base.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.170390 sdmetrics-0.9.3/tests/unit/single_table/
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.170614 sdmetrics-0.9.3/tests/unit/single_table/detection/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     2518 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/unit/single_table/detection/test_detection.py
-drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-12 18:26:28.170751 sdmetrics-0.9.3/tests/unit/single_table/privacy/
--rw-r--r--   0 romain_datacebo   (501) staff       (20)      749 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/unit/single_table/privacy/test_util.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     7987 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/unit/single_table/test_base.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     6834 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/unit/single_table/test_multi_single_column.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     6338 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/unit/single_table/test_new_row_synthesis.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     1383 2023-04-12 18:26:18.000000 sdmetrics-0.9.3/tests/unit/test__addons.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     1789 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/unit/test_base.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     1066 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/unit/test_demos.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)     6412 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/unit/test_utils.py
--rw-r--r--   0 romain_datacebo   (501) staff       (20)      735 2023-04-11 14:07:52.000000 sdmetrics-0.9.3/tests/utils.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.571921 sdmetrics-0.9.3.dev0/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      142 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/AUTHORS.rst
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     8364 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/CONTRIBUTING.rst
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    17346 2023-04-11 17:49:30.000000 sdmetrics-0.9.3.dev0/HISTORY.md
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1077 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/LICENSE
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      295 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/MANIFEST.in
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    23496 2023-04-11 17:54:06.572266 sdmetrics-0.9.3.dev0/PKG-INFO
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     5223 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/README.md
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.519190 sdmetrics-0.9.3.dev0/docs/
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.528219 sdmetrics-0.9.3.dev0/docs/images/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)   181646 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/docs/images/column_comparison.png
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)   222559 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/docs/images/column_pairs.png
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.530396 sdmetrics-0.9.3.dev0/sdmetrics/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2199 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      825 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/_addons.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     3344 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/base.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.531965 sdmetrics-0.9.3.dev0/sdmetrics/column_pairs/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      551 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/column_pairs/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1867 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/column_pairs/base.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.533379 sdmetrics-0.9.3.dev0/sdmetrics/column_pairs/statistical/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      480 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/column_pairs/statistical/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     3367 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/column_pairs/statistical/contingency_similarity.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     5256 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/column_pairs/statistical/correlation_similarity.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     4418 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/column_pairs/statistical/kl_divergence.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.534079 sdmetrics-0.9.3.dev0/sdmetrics/demos/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     8013 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/demos/multi_table.pkl
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    48099 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/demos/single_table.pkl
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    61272 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/demos/timeseries.pkl
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2451 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/demos.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      130 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/errors.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      300 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/goal.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.535168 sdmetrics-0.9.3.dev0/sdmetrics/multi_table/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1611 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/multi_table/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1447 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/multi_table/base.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.536255 sdmetrics-0.9.3.dev0/sdmetrics/multi_table/detection/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       71 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/multi_table/detection/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2018 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/multi_table/detection/base.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     4619 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/multi_table/detection/parent_child.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    10713 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/multi_table/multi_single_table.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.537179 sdmetrics-0.9.3.dev0/sdmetrics/multi_table/statistical/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      352 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/multi_table/statistical/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     5932 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/multi_table/statistical/cardinality_shape_similarity.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     8484 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/multi_table/statistical/cardinality_statistic_similarity.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.537651 sdmetrics-0.9.3.dev0/sdmetrics/reports/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      169 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/reports/__init__.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.538609 sdmetrics-0.9.3.dev0/sdmetrics/reports/multi_table/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      250 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/reports/multi_table/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    11069 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/reports/multi_table/diagnostic_report.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2081 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/reports/multi_table/plot_utils.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    14805 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/reports/multi_table/quality_report.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.539597 sdmetrics-0.9.3.dev0/sdmetrics/reports/single_table/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      253 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/reports/single_table/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     9171 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/reports/single_table/diagnostic_report.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    12880 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/reports/single_table/plot_utils.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    10073 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/reports/single_table/quality_report.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    24960 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/reports/utils.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.540383 sdmetrics-0.9.3.dev0/sdmetrics/single_column/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1011 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_column/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1938 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_column/base.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.543513 sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      878 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2130 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/boundary_adherence.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2805 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/category_coverage.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2120 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/cstest.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2483 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/kscomplement.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2748 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/missing_value_similarity.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2332 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/range_coverage.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     3694 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/statistic_similarity.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2124 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/tv_complement.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.546585 sdmetrics-0.9.3.dev0/sdmetrics/single_table/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     3636 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     7241 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/base.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     8748 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/bayesian_network.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.547152 sdmetrics-0.9.3.dev0/sdmetrics/single_table/detection/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      213 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/detection/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     4297 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/detection/base.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2355 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/detection/sklearn.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.548680 sdmetrics-0.9.3.dev0/sdmetrics/single_table/efficacy/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1059 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/efficacy/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     4848 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/efficacy/base.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     3062 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/efficacy/binary.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     3897 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/efficacy/mlefficacy.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1816 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/efficacy/multiclass.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1412 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/efficacy/regression.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     6597 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/gaussian_mixture.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     9447 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/multi_column_pairs.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     9136 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/multi_single_column.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     7518 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/new_row_synthesis.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.551896 sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1021 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    13909 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/base.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     6127 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/cap.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     7982 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/categorical_sklearn.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     4255 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/ensemble.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2703 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/loss.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     4151 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/numerical_sklearn.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     4733 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/radius_nearest_neighbor.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     3737 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/util.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.552682 sdmetrics-0.9.3.dev0/sdmetrics/timeseries/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      615 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/timeseries/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     3048 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/timeseries/base.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     3919 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/timeseries/detection.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.553977 sdmetrics-0.9.3.dev0/sdmetrics/timeseries/efficacy/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      380 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/timeseries/efficacy/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     4195 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/timeseries/efficacy/base.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      526 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/timeseries/efficacy/classification.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2138 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/timeseries/ml_scorers.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     8766 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/utils.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      306 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/warnings.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.531569 sdmetrics-0.9.3.dev0/sdmetrics.egg-info/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    23496 2023-04-11 17:54:06.000000 sdmetrics-0.9.3.dev0/sdmetrics.egg-info/PKG-INFO
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     7062 2023-04-11 17:54:06.000000 sdmetrics-0.9.3.dev0/sdmetrics.egg-info/SOURCES.txt
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)        1 2023-04-11 17:54:06.000000 sdmetrics-0.9.3.dev0/sdmetrics.egg-info/dependency_links.txt
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)        1 2023-04-11 17:54:06.000000 sdmetrics-0.9.3.dev0/sdmetrics.egg-info/not-zip-safe
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1636 2023-04-11 17:54:06.000000 sdmetrics-0.9.3.dev0/sdmetrics.egg-info/requires.txt
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       10 2023-04-11 17:54:06.000000 sdmetrics-0.9.3.dev0/sdmetrics.egg-info/top_level.txt
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1425 2023-04-11 17:54:06.572797 sdmetrics-0.9.3.dev0/setup.cfg
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     3717 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/setup.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.554422 sdmetrics-0.9.3.dev0/tests/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       33 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/__init__.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.554901 sdmetrics-0.9.3.dev0/tests/integration/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       45 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/__init__.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.555070 sdmetrics-0.9.3.dev0/tests/integration/column_pairs/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       65 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/column_pairs/__init__.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.555468 sdmetrics-0.9.3.dev0/tests/integration/column_pairs/statistical/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       77 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/column_pairs/statistical/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     3736 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/column_pairs/statistical/test_kl_divergence.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.556983 sdmetrics-0.9.3.dev0/tests/integration/multi_table/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       64 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/multi_table/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2732 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/multi_table/test_multi_single_table.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      581 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/multi_table/test_multi_table.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     3719 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/multi_table/test_parent_child.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2932 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/multi_table/test_statistical_metrics.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.557182 sdmetrics-0.9.3.dev0/tests/integration/reports/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       60 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/reports/__init__.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.557515 sdmetrics-0.9.3.dev0/tests/integration/reports/multi_table/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       72 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/reports/multi_table/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2578 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/reports/multi_table/test_multi_table_quality_report.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.557910 sdmetrics-0.9.3.dev0/tests/integration/reports/single_table/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       73 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/reports/single_table/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1823 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/reports/single_table/test_single_table_quality_report.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.558112 sdmetrics-0.9.3.dev0/tests/integration/single_column/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       66 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/single_column/__init__.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.558678 sdmetrics-0.9.3.dev0/tests/integration/single_column/statistical/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       66 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/single_column/statistical/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1467 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/single_column/statistical/test_cstest.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1509 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/single_column/statistical/test_kscomplement.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.559237 sdmetrics-0.9.3.dev0/tests/integration/single_table/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       65 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/single_table/__init__.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.560228 sdmetrics-0.9.3.dev0/tests/integration/single_table/efficacy/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2446 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/single_table/efficacy/test_binary.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1283 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/single_table/efficacy/test_detection.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1677 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/single_table/efficacy/test_multiclass.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1898 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/single_table/efficacy/test_regression.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.560494 sdmetrics-0.9.3.dev0/tests/integration/single_table/privacy/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     6178 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/single_table/privacy/test_privacy.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1717 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/single_table/test_gaussian_mixture.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     4308 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/single_table/test_single_table.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1261 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/test_base.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.561300 sdmetrics-0.9.3.dev0/tests/integration/timeseries/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       63 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/timeseries/__init__.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.561692 sdmetrics-0.9.3.dev0/tests/integration/timeseries/efficacy/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       72 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/timeseries/efficacy/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      778 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/timeseries/efficacy/test_classification.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1354 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/timeseries/test_timeseries.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.563610 sdmetrics-0.9.3.dev0/tests/unit/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       38 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/__init__.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.564674 sdmetrics-0.9.3.dev0/tests/unit/column_pairs/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       46 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/column_pairs/__init__.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.565449 sdmetrics-0.9.3.dev0/tests/unit/column_pairs/statistical/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       59 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/column_pairs/statistical/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1515 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/column_pairs/statistical/test_contingency_similarity.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     6305 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/column_pairs/statistical/test_correlation_similarity.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      818 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/column_pairs/test_base.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.565658 sdmetrics-0.9.3.dev0/tests/unit/multi_table/
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.566311 sdmetrics-0.9.3.dev0/tests/unit/multi_table/statistical/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     6089 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/multi_table/statistical/test_cardinality_shape_similarity.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     8127 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/multi_table/statistical/test_cardinality_statistic_similarity.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     3642 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/multi_table/test_multi_single_table.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.566515 sdmetrics-0.9.3.dev0/tests/unit/reports/
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.567220 sdmetrics-0.9.3.dev0/tests/unit/reports/multi_table/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    24434 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/reports/multi_table/test_multi_table_diagnostic_report.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1881 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/reports/multi_table/test_multi_table_plot_utils.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    44827 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/reports/multi_table/test_multi_table_quality_report.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.568151 sdmetrics-0.9.3.dev0/tests/unit/reports/single_table/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    19753 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/reports/single_table/test_single_table_diagnostic_report.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     8208 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/reports/single_table/test_single_table_plot_utils.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    31054 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/reports/single_table/test_single_table_quality_report.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    39408 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/reports/test_utils.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.568602 sdmetrics-0.9.3.dev0/tests/unit/single_column/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       47 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/single_column/__init__.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.570045 sdmetrics-0.9.3.dev0/tests/unit/single_column/statistical/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       60 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/single_column/statistical/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1361 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/single_column/statistical/test_boundary_adherence.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2848 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/single_column/statistical/test_category_coverage.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2378 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/single_column/statistical/test_missing_value_similarity.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2751 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/single_column/statistical/test_range_coverage.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     3543 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/single_column/statistical/test_statistic_similarity.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1978 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/single_column/statistical/test_tv_complement.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      823 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/single_column/test_base.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.570894 sdmetrics-0.9.3.dev0/tests/unit/single_table/
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.571116 sdmetrics-0.9.3.dev0/tests/unit/single_table/detection/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2518 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/single_table/detection/test_detection.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.571638 sdmetrics-0.9.3.dev0/tests/unit/single_table/privacy/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      749 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/single_table/privacy/test_util.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     7987 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/single_table/test_base.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     6834 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/single_table/test_multi_single_column.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     6338 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/single_table/test_new_row_synthesis.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1383 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/test__addons.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1789 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/test_base.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1066 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/test_demos.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     6412 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/test_utils.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      735 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/utils.py
```

### Comparing `sdmetrics-0.9.3/CONTRIBUTING.rst` & `sdmetrics-0.9.3.dev0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/HISTORY.md` & `sdmetrics-0.9.3.dev0/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,9 @@
 # History
 
-## v0.9.3 - 2023-04-12
-
-This release improves the clarity of warning/error messages. We also add a version add-on, update the workflow to optimize the runtime and fix a bug in the `NewRowSynthesis` metric when computing the `synthetic_sample_size` for multi-table.
-
-### New Features
-* Add functionality to find version add-on - Issue [#321](https://github.com/sdv-dev/SDMetrics/issues/321) by @frances-h
-* More detailed warning in QualityReport when there is a constant input - Issue [#316](https://github.com/sdv-dev/SDMetrics/issues/316) by @pvk-developer
-* Make error more informative in QualityReport when tables cannot be merged - Issue [#317](https://github.com/sdv-dev/SDMetrics/issues/317) by @frances-h
-* More detailed warning in QualityReport for unexpected category values - Issue [#315](https://github.com/sdv-dev/SDMetrics/issues/315) by @frances-h
-
-### Bug Fixes
-* Multi table DiagnosticReport sets synthetic_sample_size too low for NewRowSynthesis - Issue [#320](https://github.com/sdv-dev/SDMetrics/issues/320) by @pvk-developer
-
-
 ## v0.9.2 - 2023-03-08
 
 This release fixes bugs in the  `NewRowSynthesis` metric when too many columns were present. It also fixes bugs around datetime columns that are formatted as strings in both `get_column_pair_plot` and `get_column_plot`.
 
 ### Bug Fixes
 * Method get_column_pair_plot: Does not plot synthetic data if datetime column is formatted as a string - Issue [#310] (https://github.com/sdv-dev/SDMetrics/issues/310) by @frances-h
 * Method get_column_plot: ValueError if a datetime column is formatted as a string - Issue [#309](https://github.com/sdv-dev/SDMetrics/issues/309) by @frances-h
```

### Comparing `sdmetrics-0.9.3/LICENSE` & `sdmetrics-0.9.3.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/PKG-INFO` & `sdmetrics-0.9.3.dev0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdmetrics
-Version: 0.9.3
+Version: 0.9.3.dev0
 Summary: Metrics for Synthetic Data Generation Projects
 Home-page: https://github.com/sdv-dev/SDMetrics
 Author: MIT Data To AI Lab
 Author-email: dailabmit@gmail.com
 License: MIT license
 Keywords: sdmetrics sdmetrics SDMetrics
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -169,28 +169,14 @@
 [Get started using the SDV package](https://sdv.dev/SDV/getting_started/install.html) -- a fully
 integrated solution and your one-stop shop for synthetic data. Or, use the standalone libraries
 for specific needs.
 
 
 # History
 
-## v0.9.3 - 2023-04-12
-
-This release improves the clarity of warning/error messages. We also add a version add-on, update the workflow to optimize the runtime and fix a bug in the `NewRowSynthesis` metric when computing the `synthetic_sample_size` for multi-table.
-
-### New Features
-* Add functionality to find version add-on - Issue [#321](https://github.com/sdv-dev/SDMetrics/issues/321) by @frances-h
-* More detailed warning in QualityReport when there is a constant input - Issue [#316](https://github.com/sdv-dev/SDMetrics/issues/316) by @pvk-developer
-* Make error more informative in QualityReport when tables cannot be merged - Issue [#317](https://github.com/sdv-dev/SDMetrics/issues/317) by @frances-h
-* More detailed warning in QualityReport for unexpected category values - Issue [#315](https://github.com/sdv-dev/SDMetrics/issues/315) by @frances-h
-
-### Bug Fixes
-* Multi table DiagnosticReport sets synthetic_sample_size too low for NewRowSynthesis - Issue [#320](https://github.com/sdv-dev/SDMetrics/issues/320) by @pvk-developer
-
-
 ## v0.9.2 - 2023-03-08
 
 This release fixes bugs in the  `NewRowSynthesis` metric when too many columns were present. It also fixes bugs around datetime columns that are formatted as strings in both `get_column_pair_plot` and `get_column_plot`.
 
 ### Bug Fixes
 * Method get_column_pair_plot: Does not plot synthetic data if datetime column is formatted as a string - Issue [#310] (https://github.com/sdv-dev/SDMetrics/issues/310) by @frances-h
 * Method get_column_plot: ValueError if a datetime column is formatted as a string - Issue [#309](https://github.com/sdv-dev/SDMetrics/issues/309) by @frances-h
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sdmetrics Version: 0.9.3 Summary: Metrics for
+Metadata-Version: 2.1 Name: sdmetrics Version: 0.9.3.dev0 Summary: Metrics for
 Synthetic Data Generation Projects Home-page: https://github.com/sdv-dev/
 SDMetrics Author: MIT Data To AI Lab Author-email: dailabmit@gmail.com License:
 MIT license Keywords: sdmetrics sdmetrics SDMetrics Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
@@ -73,32 +73,18 @@
 including: * ð Data discovery & transformation. Reverse the transforms to
 reproduce realistic data. * ð§  Multiple machine learning models -- ranging
 from Copulas to Deep Learning -- to create tabular, multi table and time series
 data. * ð Measuring quality and privacy of synthetic data, and comparing
 different synthetic data generation models. [Get started using the SDV package]
 (https://sdv.dev/SDV/getting_started/install.html) -- a fully integrated
 solution and your one-stop shop for synthetic data. Or, use the standalone
-libraries for specific needs. # History ## v0.9.3 - 2023-04-12 This release
-improves the clarity of warning/error messages. We also add a version add-on,
-update the workflow to optimize the runtime and fix a bug in the
-`NewRowSynthesis` metric when computing the `synthetic_sample_size` for multi-
-table. ###Â New Features * Add functionality to find version add-on - Issue
-[#321](https://github.com/sdv-dev/SDMetrics/issues/321) by @frances-h * More
-detailed warning in QualityReport when there is a constant input - Issue [#316]
-(https://github.com/sdv-dev/SDMetrics/issues/316) by @pvk-developer * Make
-error more informative in QualityReport when tables cannot be merged - Issue
-[#317](https://github.com/sdv-dev/SDMetrics/issues/317) by @frances-h * More
-detailed warning in QualityReport for unexpected category values - Issue [#315]
-(https://github.com/sdv-dev/SDMetrics/issues/315) by @frances-h ### Bug Fixes *
-Multi table DiagnosticReport sets synthetic_sample_size too low for
-NewRowSynthesis - Issue [#320](https://github.com/sdv-dev/SDMetrics/issues/320)
-by @pvk-developer ## v0.9.2 - 2023-03-08 This release fixes bugs in the
-`NewRowSynthesis` metric when too many columns were present. It also fixes bugs
-around datetime columns that are formatted as strings in both
-`get_column_pair_plot` and `get_column_plot`. ### Bug Fixes * Method
+libraries for specific needs. # History ## v0.9.2 - 2023-03-08 This release
+fixes bugs in the `NewRowSynthesis` metric when too many columns were present.
+It also fixes bugs around datetime columns that are formatted as strings in
+both `get_column_pair_plot` and `get_column_plot`. ### Bug Fixes * Method
 get_column_pair_plot: Does not plot synthetic data if datetime column is
 formatted as a string - Issue [#310] (https://github.com/sdv-dev/SDMetrics/
 issues/310) by @frances-h * Method get_column_plot: ValueError if a datetime
 column is formatted as a string - Issue [#309](https://github.com/sdv-dev/
 SDMetrics/issues/309) by @frances-h * Fix ValueError in the NewRowSynthesis
 metric (also impacts DiagnosticReport) - Issue [#307](https://github.com/sdv-
 dev/SDMetrics/issues/307) by @frances-h ## v0.9.1 - 2023-02-17 This release
```

### Comparing `sdmetrics-0.9.3/README.md` & `sdmetrics-0.9.3.dev0/README.md`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/docs/images/column_comparison.png` & `sdmetrics-0.9.3.dev0/docs/images/column_comparison.png`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/docs/images/column_pairs.png` & `sdmetrics-0.9.3.dev0/docs/images/column_pairs.png`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/__init__.py` & `sdmetrics-0.9.3.dev0/sdmetrics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for SDMetrics."""
 
 __author__ = 'MIT Data To AI Lab'
 __email__ = 'dailabmit@gmail.com'
-__version__ = '0.9.3'
+__version__ = '0.9.3.dev0'
 
 import pandas as pd
 
 from sdmetrics import (
     column_pairs, demos, goal, multi_table, single_column, single_table, timeseries)
 from sdmetrics._addons import _find_addons
 from sdmetrics.demos import load_demo
```

### Comparing `sdmetrics-0.9.3/sdmetrics/_addons.py` & `sdmetrics-0.9.3.dev0/sdmetrics/_addons.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/base.py` & `sdmetrics-0.9.3.dev0/sdmetrics/base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/column_pairs/__init__.py` & `sdmetrics-0.9.3.dev0/sdmetrics/column_pairs/__init__.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/column_pairs/base.py` & `sdmetrics-0.9.3.dev0/sdmetrics/column_pairs/base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/column_pairs/statistical/contingency_similarity.py` & `sdmetrics-0.9.3.dev0/sdmetrics/column_pairs/statistical/contingency_similarity.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/column_pairs/statistical/correlation_similarity.py` & `sdmetrics-0.9.3.dev0/sdmetrics/column_pairs/statistical/correlation_similarity.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/column_pairs/statistical/kl_divergence.py` & `sdmetrics-0.9.3.dev0/sdmetrics/column_pairs/statistical/kl_divergence.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/demos/multi_table.pkl` & `sdmetrics-0.9.3.dev0/sdmetrics/demos/multi_table.pkl`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/demos/single_table.pkl` & `sdmetrics-0.9.3.dev0/sdmetrics/demos/single_table.pkl`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/demos/timeseries.pkl` & `sdmetrics-0.9.3.dev0/sdmetrics/demos/timeseries.pkl`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/demos.py` & `sdmetrics-0.9.3.dev0/sdmetrics/demos.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/multi_table/__init__.py` & `sdmetrics-0.9.3.dev0/sdmetrics/multi_table/__init__.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/multi_table/base.py` & `sdmetrics-0.9.3.dev0/sdmetrics/multi_table/base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/multi_table/detection/base.py` & `sdmetrics-0.9.3.dev0/sdmetrics/multi_table/detection/base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/multi_table/detection/parent_child.py` & `sdmetrics-0.9.3.dev0/sdmetrics/multi_table/detection/parent_child.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/multi_table/multi_single_table.py` & `sdmetrics-0.9.3.dev0/sdmetrics/multi_table/multi_single_table.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/multi_table/statistical/cardinality_shape_similarity.py` & `sdmetrics-0.9.3.dev0/sdmetrics/multi_table/statistical/cardinality_shape_similarity.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/multi_table/statistical/cardinality_statistic_similarity.py` & `sdmetrics-0.9.3.dev0/sdmetrics/multi_table/statistical/cardinality_statistic_similarity.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/reports/multi_table/diagnostic_report.py` & `sdmetrics-0.9.3.dev0/sdmetrics/reports/multi_table/diagnostic_report.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/reports/multi_table/plot_utils.py` & `sdmetrics-0.9.3.dev0/sdmetrics/reports/multi_table/plot_utils.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/reports/multi_table/quality_report.py` & `sdmetrics-0.9.3.dev0/sdmetrics/reports/multi_table/quality_report.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/reports/single_table/diagnostic_report.py` & `sdmetrics-0.9.3.dev0/sdmetrics/reports/single_table/diagnostic_report.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/reports/single_table/plot_utils.py` & `sdmetrics-0.9.3.dev0/sdmetrics/reports/single_table/plot_utils.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/reports/single_table/quality_report.py` & `sdmetrics-0.9.3.dev0/sdmetrics/reports/single_table/quality_report.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/reports/utils.py` & `sdmetrics-0.9.3.dev0/sdmetrics/reports/utils.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_column/__init__.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_column/__init__.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_column/base.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_column/base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_column/statistical/__init__.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/__init__.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_column/statistical/boundary_adherence.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/boundary_adherence.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_column/statistical/category_coverage.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/category_coverage.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_column/statistical/cstest.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/cstest.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_column/statistical/kscomplement.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/kscomplement.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_column/statistical/missing_value_similarity.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/missing_value_similarity.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_column/statistical/range_coverage.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/range_coverage.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_column/statistical/statistic_similarity.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/statistic_similarity.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_column/statistical/tv_complement.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/tv_complement.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_table/__init__.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/__init__.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_table/base.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_table/bayesian_network.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/bayesian_network.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_table/detection/base.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/detection/base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_table/detection/sklearn.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/detection/sklearn.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_table/efficacy/__init__.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/efficacy/__init__.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_table/efficacy/base.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/efficacy/base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_table/efficacy/binary.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/efficacy/binary.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_table/efficacy/mlefficacy.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/efficacy/mlefficacy.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_table/efficacy/multiclass.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/efficacy/multiclass.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_table/efficacy/regression.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/efficacy/regression.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_table/gaussian_mixture.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/gaussian_mixture.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_table/multi_column_pairs.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/multi_column_pairs.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_table/multi_single_column.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/multi_single_column.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_table/new_row_synthesis.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/new_row_synthesis.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_table/privacy/__init__.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/__init__.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_table/privacy/base.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_table/privacy/cap.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/cap.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_table/privacy/categorical_sklearn.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/categorical_sklearn.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_table/privacy/ensemble.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/ensemble.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_table/privacy/loss.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/loss.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_table/privacy/numerical_sklearn.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/numerical_sklearn.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_table/privacy/radius_nearest_neighbor.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/radius_nearest_neighbor.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/single_table/privacy/util.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/util.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/timeseries/__init__.py` & `sdmetrics-0.9.3.dev0/sdmetrics/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/timeseries/base.py` & `sdmetrics-0.9.3.dev0/sdmetrics/timeseries/base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/timeseries/detection.py` & `sdmetrics-0.9.3.dev0/sdmetrics/timeseries/detection.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/timeseries/efficacy/base.py` & `sdmetrics-0.9.3.dev0/sdmetrics/timeseries/efficacy/base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/timeseries/efficacy/classification.py` & `sdmetrics-0.9.3.dev0/sdmetrics/timeseries/efficacy/classification.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/timeseries/ml_scorers.py` & `sdmetrics-0.9.3.dev0/sdmetrics/timeseries/ml_scorers.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics/utils.py` & `sdmetrics-0.9.3.dev0/sdmetrics/utils.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics.egg-info/PKG-INFO` & `sdmetrics-0.9.3.dev0/sdmetrics.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdmetrics
-Version: 0.9.3
+Version: 0.9.3.dev0
 Summary: Metrics for Synthetic Data Generation Projects
 Home-page: https://github.com/sdv-dev/SDMetrics
 Author: MIT Data To AI Lab
 Author-email: dailabmit@gmail.com
 License: MIT license
 Keywords: sdmetrics sdmetrics SDMetrics
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -169,28 +169,14 @@
 [Get started using the SDV package](https://sdv.dev/SDV/getting_started/install.html) -- a fully
 integrated solution and your one-stop shop for synthetic data. Or, use the standalone libraries
 for specific needs.
 
 
 # History
 
-## v0.9.3 - 2023-04-12
-
-This release improves the clarity of warning/error messages. We also add a version add-on, update the workflow to optimize the runtime and fix a bug in the `NewRowSynthesis` metric when computing the `synthetic_sample_size` for multi-table.
-
-### New Features
-* Add functionality to find version add-on - Issue [#321](https://github.com/sdv-dev/SDMetrics/issues/321) by @frances-h
-* More detailed warning in QualityReport when there is a constant input - Issue [#316](https://github.com/sdv-dev/SDMetrics/issues/316) by @pvk-developer
-* Make error more informative in QualityReport when tables cannot be merged - Issue [#317](https://github.com/sdv-dev/SDMetrics/issues/317) by @frances-h
-* More detailed warning in QualityReport for unexpected category values - Issue [#315](https://github.com/sdv-dev/SDMetrics/issues/315) by @frances-h
-
-### Bug Fixes
-* Multi table DiagnosticReport sets synthetic_sample_size too low for NewRowSynthesis - Issue [#320](https://github.com/sdv-dev/SDMetrics/issues/320) by @pvk-developer
-
-
 ## v0.9.2 - 2023-03-08
 
 This release fixes bugs in the  `NewRowSynthesis` metric when too many columns were present. It also fixes bugs around datetime columns that are formatted as strings in both `get_column_pair_plot` and `get_column_plot`.
 
 ### Bug Fixes
 * Method get_column_pair_plot: Does not plot synthetic data if datetime column is formatted as a string - Issue [#310] (https://github.com/sdv-dev/SDMetrics/issues/310) by @frances-h
 * Method get_column_plot: ValueError if a datetime column is formatted as a string - Issue [#309](https://github.com/sdv-dev/SDMetrics/issues/309) by @frances-h
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sdmetrics Version: 0.9.3 Summary: Metrics for
+Metadata-Version: 2.1 Name: sdmetrics Version: 0.9.3.dev0 Summary: Metrics for
 Synthetic Data Generation Projects Home-page: https://github.com/sdv-dev/
 SDMetrics Author: MIT Data To AI Lab Author-email: dailabmit@gmail.com License:
 MIT license Keywords: sdmetrics sdmetrics SDMetrics Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
@@ -73,32 +73,18 @@
 including: * ð Data discovery & transformation. Reverse the transforms to
 reproduce realistic data. * ð§  Multiple machine learning models -- ranging
 from Copulas to Deep Learning -- to create tabular, multi table and time series
 data. * ð Measuring quality and privacy of synthetic data, and comparing
 different synthetic data generation models. [Get started using the SDV package]
 (https://sdv.dev/SDV/getting_started/install.html) -- a fully integrated
 solution and your one-stop shop for synthetic data. Or, use the standalone
-libraries for specific needs. # History ## v0.9.3 - 2023-04-12 This release
-improves the clarity of warning/error messages. We also add a version add-on,
-update the workflow to optimize the runtime and fix a bug in the
-`NewRowSynthesis` metric when computing the `synthetic_sample_size` for multi-
-table. ###Â New Features * Add functionality to find version add-on - Issue
-[#321](https://github.com/sdv-dev/SDMetrics/issues/321) by @frances-h * More
-detailed warning in QualityReport when there is a constant input - Issue [#316]
-(https://github.com/sdv-dev/SDMetrics/issues/316) by @pvk-developer * Make
-error more informative in QualityReport when tables cannot be merged - Issue
-[#317](https://github.com/sdv-dev/SDMetrics/issues/317) by @frances-h * More
-detailed warning in QualityReport for unexpected category values - Issue [#315]
-(https://github.com/sdv-dev/SDMetrics/issues/315) by @frances-h ### Bug Fixes *
-Multi table DiagnosticReport sets synthetic_sample_size too low for
-NewRowSynthesis - Issue [#320](https://github.com/sdv-dev/SDMetrics/issues/320)
-by @pvk-developer ## v0.9.2 - 2023-03-08 This release fixes bugs in the
-`NewRowSynthesis` metric when too many columns were present. It also fixes bugs
-around datetime columns that are formatted as strings in both
-`get_column_pair_plot` and `get_column_plot`. ### Bug Fixes * Method
+libraries for specific needs. # History ## v0.9.2 - 2023-03-08 This release
+fixes bugs in the `NewRowSynthesis` metric when too many columns were present.
+It also fixes bugs around datetime columns that are formatted as strings in
+both `get_column_pair_plot` and `get_column_plot`. ### Bug Fixes * Method
 get_column_pair_plot: Does not plot synthetic data if datetime column is
 formatted as a string - Issue [#310] (https://github.com/sdv-dev/SDMetrics/
 issues/310) by @frances-h * Method get_column_plot: ValueError if a datetime
 column is formatted as a string - Issue [#309](https://github.com/sdv-dev/
 SDMetrics/issues/309) by @frances-h * Fix ValueError in the NewRowSynthesis
 metric (also impacts DiagnosticReport) - Issue [#307](https://github.com/sdv-
 dev/SDMetrics/issues/307) by @frances-h ## v0.9.1 - 2023-02-17 This release
```

### Comparing `sdmetrics-0.9.3/sdmetrics.egg-info/SOURCES.txt` & `sdmetrics-0.9.3.dev0/sdmetrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/sdmetrics.egg-info/requires.txt` & `sdmetrics-0.9.3.dev0/sdmetrics.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/setup.cfg` & `sdmetrics-0.9.3.dev0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.9.3
+current_version = 0.9.3.dev0
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `sdmetrics-0.9.3/setup.py` & `sdmetrics-0.9.3.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,10 +121,10 @@
     name='sdmetrics',
     packages=find_packages(include=['sdmetrics', 'sdmetrics.*']),
     python_requires='>=3.7,<3.11',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sdv-dev/SDMetrics',
-    version='0.9.3',
+    version='0.9.3.dev0',
     zip_safe=False,
 )
```

### Comparing `sdmetrics-0.9.3/tests/integration/column_pairs/statistical/test_kl_divergence.py` & `sdmetrics-0.9.3.dev0/tests/integration/column_pairs/statistical/test_kl_divergence.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/integration/multi_table/test_multi_single_table.py` & `sdmetrics-0.9.3.dev0/tests/integration/multi_table/test_multi_single_table.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/integration/multi_table/test_multi_table.py` & `sdmetrics-0.9.3.dev0/tests/integration/multi_table/test_multi_table.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/integration/multi_table/test_parent_child.py` & `sdmetrics-0.9.3.dev0/tests/integration/multi_table/test_parent_child.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/integration/multi_table/test_statistical_metrics.py` & `sdmetrics-0.9.3.dev0/tests/integration/multi_table/test_statistical_metrics.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/integration/reports/multi_table/test_multi_table_quality_report.py` & `sdmetrics-0.9.3.dev0/tests/integration/reports/multi_table/test_multi_table_quality_report.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/integration/reports/single_table/test_single_table_quality_report.py` & `sdmetrics-0.9.3.dev0/tests/integration/reports/single_table/test_single_table_quality_report.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/integration/single_column/statistical/test_cstest.py` & `sdmetrics-0.9.3.dev0/tests/integration/single_column/statistical/test_cstest.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/integration/single_column/statistical/test_kscomplement.py` & `sdmetrics-0.9.3.dev0/tests/integration/single_column/statistical/test_kscomplement.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/integration/single_table/efficacy/test_binary.py` & `sdmetrics-0.9.3.dev0/tests/integration/single_table/efficacy/test_binary.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/integration/single_table/efficacy/test_detection.py` & `sdmetrics-0.9.3.dev0/tests/integration/single_table/efficacy/test_detection.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/integration/single_table/efficacy/test_multiclass.py` & `sdmetrics-0.9.3.dev0/tests/integration/single_table/efficacy/test_multiclass.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/integration/single_table/efficacy/test_regression.py` & `sdmetrics-0.9.3.dev0/tests/integration/single_table/efficacy/test_regression.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/integration/single_table/privacy/test_privacy.py` & `sdmetrics-0.9.3.dev0/tests/integration/single_table/privacy/test_privacy.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/integration/single_table/test_gaussian_mixture.py` & `sdmetrics-0.9.3.dev0/tests/integration/single_table/test_gaussian_mixture.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/integration/single_table/test_single_table.py` & `sdmetrics-0.9.3.dev0/tests/integration/single_table/test_single_table.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/integration/test_base.py` & `sdmetrics-0.9.3.dev0/tests/integration/test_base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/integration/timeseries/efficacy/test_classification.py` & `sdmetrics-0.9.3.dev0/tests/integration/timeseries/efficacy/test_classification.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/integration/timeseries/test_timeseries.py` & `sdmetrics-0.9.3.dev0/tests/integration/timeseries/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/unit/column_pairs/statistical/test_contingency_similarity.py` & `sdmetrics-0.9.3.dev0/tests/unit/column_pairs/statistical/test_contingency_similarity.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/unit/column_pairs/statistical/test_correlation_similarity.py` & `sdmetrics-0.9.3.dev0/tests/unit/column_pairs/statistical/test_correlation_similarity.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/unit/column_pairs/test_base.py` & `sdmetrics-0.9.3.dev0/tests/unit/column_pairs/test_base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/unit/multi_table/statistical/test_cardinality_shape_similarity.py` & `sdmetrics-0.9.3.dev0/tests/unit/multi_table/statistical/test_cardinality_shape_similarity.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/unit/multi_table/statistical/test_cardinality_statistic_similarity.py` & `sdmetrics-0.9.3.dev0/tests/unit/multi_table/statistical/test_cardinality_statistic_similarity.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/unit/multi_table/test_multi_single_table.py` & `sdmetrics-0.9.3.dev0/tests/unit/multi_table/test_multi_single_table.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/unit/reports/multi_table/test_multi_table_diagnostic_report.py` & `sdmetrics-0.9.3.dev0/tests/unit/reports/multi_table/test_multi_table_diagnostic_report.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/unit/reports/multi_table/test_multi_table_plot_utils.py` & `sdmetrics-0.9.3.dev0/tests/unit/reports/multi_table/test_multi_table_plot_utils.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/unit/reports/multi_table/test_multi_table_quality_report.py` & `sdmetrics-0.9.3.dev0/tests/unit/reports/multi_table/test_multi_table_quality_report.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/unit/reports/single_table/test_single_table_diagnostic_report.py` & `sdmetrics-0.9.3.dev0/tests/unit/reports/single_table/test_single_table_diagnostic_report.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/unit/reports/single_table/test_single_table_plot_utils.py` & `sdmetrics-0.9.3.dev0/tests/unit/reports/single_table/test_single_table_plot_utils.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/unit/reports/single_table/test_single_table_quality_report.py` & `sdmetrics-0.9.3.dev0/tests/unit/reports/single_table/test_single_table_quality_report.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/unit/reports/test_utils.py` & `sdmetrics-0.9.3.dev0/tests/unit/reports/test_utils.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/unit/single_column/statistical/test_boundary_adherence.py` & `sdmetrics-0.9.3.dev0/tests/unit/single_column/statistical/test_boundary_adherence.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/unit/single_column/statistical/test_category_coverage.py` & `sdmetrics-0.9.3.dev0/tests/unit/single_column/statistical/test_category_coverage.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/unit/single_column/statistical/test_missing_value_similarity.py` & `sdmetrics-0.9.3.dev0/tests/unit/single_column/statistical/test_missing_value_similarity.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/unit/single_column/statistical/test_range_coverage.py` & `sdmetrics-0.9.3.dev0/tests/unit/single_column/statistical/test_range_coverage.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/unit/single_column/statistical/test_statistic_similarity.py` & `sdmetrics-0.9.3.dev0/tests/unit/single_column/statistical/test_statistic_similarity.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/unit/single_column/statistical/test_tv_complement.py` & `sdmetrics-0.9.3.dev0/tests/unit/single_column/statistical/test_tv_complement.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/unit/single_column/test_base.py` & `sdmetrics-0.9.3.dev0/tests/unit/single_column/test_base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/unit/single_table/detection/test_detection.py` & `sdmetrics-0.9.3.dev0/tests/unit/single_table/detection/test_detection.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/unit/single_table/privacy/test_util.py` & `sdmetrics-0.9.3.dev0/tests/unit/single_table/privacy/test_util.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/unit/single_table/test_base.py` & `sdmetrics-0.9.3.dev0/tests/unit/single_table/test_base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/unit/single_table/test_multi_single_column.py` & `sdmetrics-0.9.3.dev0/tests/unit/single_table/test_multi_single_column.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/unit/single_table/test_new_row_synthesis.py` & `sdmetrics-0.9.3.dev0/tests/unit/single_table/test_new_row_synthesis.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/unit/test__addons.py` & `sdmetrics-0.9.3.dev0/tests/unit/test__addons.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/unit/test_base.py` & `sdmetrics-0.9.3.dev0/tests/unit/test_base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/unit/test_demos.py` & `sdmetrics-0.9.3.dev0/tests/unit/test_demos.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/unit/test_utils.py` & `sdmetrics-0.9.3.dev0/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.3/tests/utils.py` & `sdmetrics-0.9.3.dev0/tests/utils.py`

 * *Files identical despite different names*

