# Comparing `tmp/psifr-0.8.2.tar.gz` & `tmp/psifr-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psifr-0.8.2.tar", last modified: Thu Sep 15 23:05:53 2022, max compression
+gzip compressed data, was "psifr-0.9.0.tar", last modified: Mon Jun  5 23:14:17 2023, max compression
```

## Comparing `psifr-0.8.2.tar` & `psifr-0.9.0.tar`

### file list

```diff
@@ -1,25 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 23:05:53.189773 psifr-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-09-15 23:05:42.000000 psifr-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5637 2022-09-15 23:05:53.189773 psifr-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5051 2022-09-15 23:05:42.000000 psifr-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-09-15 23:05:42.000000 psifr-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      938 2022-09-15 23:05:53.189773 psifr-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-15 23:05:42.000000 psifr-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 23:05:53.173773 psifr-0.8.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 23:05:53.177773 psifr-0.8.2/src/psifr/
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-09-15 23:05:42.000000 psifr-0.8.2/src/psifr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2046 2022-09-15 23:05:42.000000 psifr-0.8.2/src/psifr/clustering.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 23:05:53.177773 psifr-0.8.2/src/psifr/data/
--rw-r--r--   0 runner    (1001) docker     (121)  4050433 2022-09-15 23:05:42.000000 psifr-0.8.2/src/psifr/data/Morton2013.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 23:05:53.181773 psifr-0.8.2/src/psifr/distances/
--rw-r--r--   0 runner    (1001) docker     (121)  4802050 2022-09-15 23:05:42.000000 psifr-0.8.2/src/psifr/distances/Morton2013.npz
--rw-r--r--   0 runner    (1001) docker     (121)    65171 2022-09-15 23:05:42.000000 psifr-0.8.2/src/psifr/fr.py
--rw-r--r--   0 runner    (1001) docker     (121)    12764 2022-09-15 23:05:42.000000 psifr-0.8.2/src/psifr/measures.py
--rw-r--r--   0 runner    (1001) docker     (121)     6020 2022-09-15 23:05:42.000000 psifr-0.8.2/src/psifr/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    38434 2022-09-15 23:05:42.000000 psifr-0.8.2/src/psifr/transitions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 23:05:53.177773 psifr-0.8.2/src/psifr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5637 2022-09-15 23:05:53.000000 psifr-0.8.2/src/psifr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-09-15 23:05:53.000000 psifr-0.8.2/src/psifr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-15 23:05:53.000000 psifr-0.8.2/src/psifr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-09-15 23:05:53.000000 psifr-0.8.2/src/psifr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-15 23:05:53.000000 psifr-0.8.2/src/psifr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:14:17.214196 psifr-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 23:14:05.000000 psifr-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-06-05 23:14:17.214196 psifr-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-06-05 23:14:05.000000 psifr-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-05 23:14:05.000000 psifr-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 23:14:17.214196 psifr-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:14:17.202195 psifr-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:14:17.202195 psifr-0.9.0/src/psifr/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-05 23:14:05.000000 psifr-0.9.0/src/psifr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:14:17.202195 psifr-0.9.0/src/psifr/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  4050433 2023-06-05 23:14:05.000000 psifr-0.9.0/src/psifr/data/Morton2013.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:14:17.210196 psifr-0.9.0/src/psifr/distances/
+-rw-r--r--   0 runner    (1001) docker     (123)  4802050 2023-06-05 23:14:05.000000 psifr-0.9.0/src/psifr/distances/Morton2013.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    65710 2023-06-05 23:14:05.000000 psifr-0.9.0/src/psifr/fr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13627 2023-06-05 23:14:05.000000 psifr-0.9.0/src/psifr/maskers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-06-05 23:14:05.000000 psifr-0.9.0/src/psifr/measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32940 2023-06-05 23:14:05.000000 psifr-0.9.0/src/psifr/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:14:17.202195 psifr-0.9.0/src/psifr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-06-05 23:14:17.000000 psifr-0.9.0/src/psifr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-05 23:14:17.000000 psifr-0.9.0/src/psifr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 23:14:17.000000 psifr-0.9.0/src/psifr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-05 23:14:17.000000 psifr-0.9.0/src/psifr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 23:14:17.000000 psifr-0.9.0/src/psifr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:14:17.214196 psifr-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-05 23:14:05.000000 psifr-0.9.0/tests/test_category_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-06-05 23:14:05.000000 psifr-0.9.0/tests/test_distance_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18899 2023-06-05 23:14:05.000000 psifr-0.9.0/tests/test_fr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-06-05 23:14:05.000000 psifr-0.9.0/tests/test_lag_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-06-05 23:14:05.000000 psifr-0.9.0/tests/test_maskers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-05 23:14:05.000000 psifr-0.9.0/tests/test_output_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-05 23:14:05.000000 psifr-0.9.0/tests/test_pair_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-06-05 23:14:05.000000 psifr-0.9.0/tests/test_plots.py
```

### Comparing `psifr-0.8.2/LICENSE` & `psifr-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `psifr-0.8.2/PKG-INFO` & `psifr-0.9.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: psifr
-Version: 0.8.2
+Version: 0.9.0
 Summary: Psifr: Analysis and visualization of free recall data
-Home-page: https://github.com/mortonne/psifr
-Author: Neal Morton
-Author-email: mortonne@gmail.com
+Author-email: Neal W Morton <mortonne@gmail.com>
 License: GPL-3.0-or-later
 Keywords: psychology,memory,free recall
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: perf
 License-File: LICENSE
 
 # Psifr
@@ -22,15 +21,21 @@
 [![Pytest](https://github.com/mortonne/psifr/actions/workflows/pytest.yml/badge.svg)](https://github.com/mortonne/psifr/actions/workflows/pytest.yml)
 [![codecov](https://codecov.io/gh/mortonne/psifr/branch/master/graph/badge.svg)](https://codecov.io/gh/mortonne/psifr)
 [![status](https://joss.theoj.org/papers/712d4452e465229d61d0e281d3d6f299/status.svg)](https://joss.theoj.org/papers/712d4452e465229d61d0e281d3d6f299)
 [![DOI](https://zenodo.org/badge/248593723.svg)](https://zenodo.org/badge/latestdoi/248593723)
 
 Advanced analysis and visualization of free recall data in Python.
 
-Psifr has tools to visualize recall sequences, to make it easier to see general trends in the data. Psifr also provides targeted analyses to examine factors that may affect recall, such as recency, primacy, temporal contiguity, stimulus category, and semantic relatedness. Analyses are customizable, allowing flexible filtering of included data to help answer precise questions. Extensive automated testing is used to ensure the consistency and correctness of analysis results. 
+Features:
+* A large library of advanced analyses, tested against published benchmarks
+* Flexible analysis customization and plotting
+* Tools for exploratory analysis of large datasets
+* Extensive automated testing to ensure analysis correctness
+* Based around a simple and flexible table-based data format
+* Comprehensive [documentation](https://psifr.readthedocs.io/en/stable/api/overview.html) and [user guide](https://psifr.readthedocs.io/en/stable/guide/overview.html)
 
 The name Psifr is pronounced "cipher". It's taken from Psi, in reference to the field of psychology, and FR for free recall.
 
 <div align="center">
   <div style="max-width:500px; margin:0 20px;">
     <img src="https://github.com/mortonne/psifr/blob/master/images/raster.png" alt="free recall visualization" width="500px">
     <div style="text-align:left; padding:10px 0;">
```

### Comparing `psifr-0.8.2/README.md` & `psifr-0.9.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,21 @@
 [![Pytest](https://github.com/mortonne/psifr/actions/workflows/pytest.yml/badge.svg)](https://github.com/mortonne/psifr/actions/workflows/pytest.yml)
 [![codecov](https://codecov.io/gh/mortonne/psifr/branch/master/graph/badge.svg)](https://codecov.io/gh/mortonne/psifr)
 [![status](https://joss.theoj.org/papers/712d4452e465229d61d0e281d3d6f299/status.svg)](https://joss.theoj.org/papers/712d4452e465229d61d0e281d3d6f299)
 [![DOI](https://zenodo.org/badge/248593723.svg)](https://zenodo.org/badge/latestdoi/248593723)
 
 Advanced analysis and visualization of free recall data in Python.
 
-Psifr has tools to visualize recall sequences, to make it easier to see general trends in the data. Psifr also provides targeted analyses to examine factors that may affect recall, such as recency, primacy, temporal contiguity, stimulus category, and semantic relatedness. Analyses are customizable, allowing flexible filtering of included data to help answer precise questions. Extensive automated testing is used to ensure the consistency and correctness of analysis results. 
+Features:
+* A large library of advanced analyses, tested against published benchmarks
+* Flexible analysis customization and plotting
+* Tools for exploratory analysis of large datasets
+* Extensive automated testing to ensure analysis correctness
+* Based around a simple and flexible table-based data format
+* Comprehensive [documentation](https://psifr.readthedocs.io/en/stable/api/overview.html) and [user guide](https://psifr.readthedocs.io/en/stable/guide/overview.html)
 
 The name Psifr is pronounced "cipher". It's taken from Psi, in reference to the field of psychology, and FR for free recall.
 
 <div align="center">
   <div style="max-width:500px; margin:0 20px;">
     <img src="https://github.com/mortonne/psifr/blob/master/images/raster.png" alt="free recall visualization" width="500px">
     <div style="text-align:left; padding:10px 0;">
```

### Comparing `psifr-0.8.2/src/psifr/data/Morton2013.csv` & `psifr-0.9.0/src/psifr/data/Morton2013.csv`

 * *Files identical despite different names*

### Comparing `psifr-0.8.2/src/psifr/distances/Morton2013.npz` & `psifr-0.9.0/src/psifr/distances/Morton2013.npz`

 * *Files identical despite different names*

### Comparing `psifr-0.8.2/src/psifr/fr.py` & `psifr-0.9.0/src/psifr/fr.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from pkg_resources import resource_filename
 import warnings
 import numpy as np
 import pandas as pd
 import seaborn as sns
 
+from psifr import stats
 from psifr import measures
-from psifr import clustering
 
 
 def sample_data(study):
     """Read sample data."""
     data_file = resource_filename('psifr', f'data/{study}.csv')
     df = pd.read_csv(data_file)
     return df
@@ -826,58 +826,54 @@
     Parameters
     ----------
     df : pandas.DataFrame
         Merged study and recall data. See merge_lists.
 
     Returns
     -------
-    recall : pandas.Series
-        Index includes:
-
+    recall : pandas.DataFrame
         subject : hashable
             Subject identifier.
 
         input : int
             Serial position in the list.
 
-        Values are:
-
         recall : float
             Recall probability for each serial position.
 
     See Also
     --------
     plot_spc : Plot serial position curve results.
     pnr : Probability of nth recall.
 
     Examples
     --------
     >>> from psifr import fr
     >>> raw = fr.sample_data('Morton2013')
     >>> data = fr.merge_free_recall(raw)
     >>> fr.spc(data)
-                     recall
-    subject input          
-    1       1.0    0.541667
-            2.0    0.458333
-            3.0    0.625000
-            4.0    0.333333
-            5.0    0.437500
-    ...                 ...
-    47      20.0   0.500000
-            21.0   0.770833
-            22.0   0.729167
-            23.0   0.895833
-            24.0   0.958333
+         subject  input    recall
+    0          1    1.0  0.541667
+    1          1    2.0  0.458333
+    2          1    3.0  0.625000
+    3          1    4.0  0.333333
+    4          1    5.0  0.437500
+    ..       ...    ...       ...
+    955       47   20.0  0.500000
+    956       47   21.0  0.770833
+    957       47   22.0  0.729167
+    958       47   23.0  0.895833
+    959       47   24.0  0.958333
     <BLANKLINE>
-    [960 rows x 1 columns]
+    [960 rows x 3 columns]
     """
     clean = df.query('study')
     recall = clean.groupby(['subject', 'input'])['recall'].mean()
-    return pd.DataFrame(recall)
+    recall = pd.DataFrame(recall).reset_index()
+    return recall
 
 
 def pnr(df, item_query=None, test_key=None, test=None):
     """
     Probability of recall by serial position and output position.
 
     Calculate probability of Nth recall, where N is each output
@@ -924,29 +920,28 @@
 
     Examples
     --------
     >>> from psifr import fr
     >>> raw = fr.sample_data('Morton2013')
     >>> data = fr.merge_free_recall(raw)
     >>> fr.pnr(data)
-                              prob  actual  possible
-    subject output input                            
-    1       1      1      0.000000       0        48
-                   2      0.020833       1        48
-                   3      0.000000       0        48
-                   4      0.000000       0        48
-                   5      0.000000       0        48
-    ...                        ...     ...       ...
-    47      24     20          NaN       0         0
-                   21          NaN       0         0
-                   22          NaN       0         0
-                   23          NaN       0         0
-                   24          NaN       0         0
+           subject  output  input      prob  actual  possible
+    0            1       1      1  0.000000       0        48
+    1            1       1      2  0.020833       1        48
+    2            1       1      3  0.000000       0        48
+    3            1       1      4  0.000000       0        48
+    4            1       1      5  0.000000       0        48
+    ...        ...     ...    ...       ...     ...       ...
+    23035       47      24     20       NaN       0         0
+    23036       47      24     21       NaN       0         0
+    23037       47      24     22       NaN       0         0
+    23038       47      24     23       NaN       0         0
+    23039       47      24     24       NaN       0         0
     <BLANKLINE>
-    [23040 rows x 3 columns]
+    [23040 rows x 6 columns]
     """
     list_length = int(df['input'].max())
     measure = measures.TransitionOutputs(
         list_length, item_query=item_query, test_key=test_key, test=test
     )
     prob = measure.analyze(df)
     return prob
@@ -996,31 +991,31 @@
 
     Examples
     --------
     >>> from psifr import fr
     >>> raw = fr.sample_data('Morton2013')
     >>> data = fr.merge_free_recall(raw)
     >>> fr.pli_list_lag(data, 3)
-                      count  per_list      prob
-    subject list_lag                           
-    1       1             7  0.155556  0.259259
-            2             5  0.111111  0.185185
-            3             0  0.000000  0.000000
-    2       1             9  0.200000  0.191489
-            2             2  0.044444  0.042553
-    ...                 ...       ...       ...
-    46      2             1  0.022222  0.100000
-            3             0  0.000000  0.000000
-    47      1             5  0.111111  0.277778
-            2             1  0.022222  0.055556
-            3             0  0.000000  0.000000
+         subject  list_lag  count  per_list      prob
+    0          1         1      7  0.155556  0.259259
+    1          1         2      5  0.111111  0.185185
+    2          1         3      0  0.000000  0.000000
+    3          2         1      9  0.200000  0.191489
+    4          2         2      2  0.044444  0.042553
+    ..       ...       ...    ...       ...       ...
+    115       46         2      1  0.022222  0.100000
+    116       46         3      0  0.000000  0.000000
+    117       47         1      5  0.111111  0.277778
+    118       47         2      1  0.022222  0.055556
+    119       47         3      0  0.000000  0.000000
     <BLANKLINE>
-    [120 rows x 3 columns]
+    [120 rows x 5 columns]
     """
     result = df.groupby('subject').apply(_subject_pli_list_lag, max_lag)
+    result = result.reset_index()
     return result
 
 
 def lag_crp(
     df, lag_key='input', count_unique=False, item_query=None, test_key=None, test=None
 ):
     """
@@ -1082,29 +1077,28 @@
 
     Examples
     --------
     >>> from psifr import fr
     >>> raw = fr.sample_data('Morton2013')
     >>> data = fr.merge_free_recall(raw)
     >>> fr.lag_crp(data)
-                       prob  actual  possible
-    subject lag                              
-    1       -23.0  0.020833       1        48
-            -22.0  0.035714       3        84
-            -21.0  0.026316       3       114
-            -20.0  0.024000       3       125
-            -19.0  0.014388       2       139
-    ...                 ...     ...       ...
-    47       19.0  0.061224       3        49
-             20.0  0.055556       2        36
-             21.0  0.045455       1        22
-             22.0  0.071429       1        14
-             23.0  0.000000       0         6
+          subject   lag      prob  actual  possible
+    0           1 -23.0  0.020833       1        48
+    1           1 -22.0  0.035714       3        84
+    2           1 -21.0  0.026316       3       114
+    3           1 -20.0  0.024000       3       125
+    4           1 -19.0  0.014388       2       139
+    ...       ...   ...       ...     ...       ...
+    1875       47  19.0  0.061224       3        49
+    1876       47  20.0  0.055556       2        36
+    1877       47  21.0  0.045455       1        22
+    1878       47  22.0  0.071429       1        14
+    1879       47  23.0  0.000000       0         6
     <BLANKLINE>
-    [1880 rows x 3 columns]
+    [1880 rows x 5 columns]
     """
     list_length = df[lag_key].max()
     measure = measures.TransitionLag(
         list_length,
         lag_key=lag_key,
         count_unique=count_unique,
         item_query=item_query,
@@ -1184,58 +1178,61 @@
     >>> subjects = [1]
     >>> study = [['absence', 'hollow', 'pupil', 'fountain']]
     >>> recall = [['fountain', 'hollow', 'absence']]
     >>> raw = fr.table_from_lists(subjects, study, recall)
     >>> data = fr.merge_free_recall(raw)
     >>> crp = fr.lag_crp_compound(data)
     >>> crp.head(14)
-                              prob  actual  possible
-    subject previous current                        
-    1       -3       -3        NaN       0         0
-                     -2        NaN       0         0
-                     -1        NaN       0         0
-                      0        NaN       0         0
-                      1        NaN       0         0
-                      2        NaN       0         0
-                      3        NaN       0         0
-            -2       -3        NaN       0         0
-                     -2        NaN       0         0
-                     -1        1.0       1         1
-                      0        NaN       0         0
-                      1        0.0       0         1
-                      2        NaN       0         0
-                      3        NaN       0         0
+        subject  previous  current  prob  actual  possible
+    0         1        -3       -3   NaN       0         0
+    1         1        -3       -2   NaN       0         0
+    2         1        -3       -1   NaN       0         0
+    3         1        -3        0   NaN       0         0
+    4         1        -3        1   NaN       0         0
+    5         1        -3        2   NaN       0         0
+    6         1        -3        3   NaN       0         0
+    7         1        -2       -3   NaN       0         0
+    8         1        -2       -2   NaN       0         0
+    9         1        -2       -1   1.0       1         1
+    10        1        -2        0   NaN       0         0
+    11        1        -2        1   0.0       0         1
+    12        1        -2        2   NaN       0         0
+    13        1        -2        3   NaN       0         0
     """
     list_length = df[lag_key].max()
     measure = measures.TransitionLag(
         list_length,
         lag_key=lag_key,
         count_unique=count_unique,
         item_query=item_query,
         test_key=test_key,
         test=test,
-        compound=True
+        compound=True,
     )
     crp = measure.analyze(df)
     return crp
 
 
-def lag_rank(df, item_query=None, test_key=None, test=None):
+def lag_rank(df, lag_key='input', item_query=None, test_key=None, test=None):
     """
     Calculate rank of the absolute lags in free recall lists.
 
     Parameters
     ----------
     df : pandas.DataFrame
         Merged study and recall data. See merge_lists. List length is
         assumed to be the same for all lists within each subject.
         Must have fields: subject, list, input, output, recalled.
         Input position must be defined such that the first serial
         position is 1, not 0.
 
+    lag_key : str, optional
+        Name of column to use when calculating lag between recalled
+        items. Default is to calculate lag based on input position.
+
     item_query : str, optional
         Query string to select items to include in the pool of possible
         recalls to be examined. See `pandas.DataFrame.query` for
         allowed format.
 
     test_key : str, optional
         Name of column with labels to use when testing transitions for
@@ -1257,24 +1254,23 @@
     Examples
     --------
     >>> from psifr import fr
     >>> raw = fr.sample_data('Morton2013')
     >>> data = fr.merge_free_recall(raw)
     >>> lag_rank = fr.lag_rank(data)
     >>> lag_rank.head()
-                 rank
-    subject          
-    1        0.610953
-    2        0.635676
-    3        0.612607
-    4        0.667090
-    5        0.643923
+       subject      rank
+    0        1  0.610953
+    1        2  0.635676
+    2        3  0.612607
+    3        4  0.667090
+    4        5  0.643923
     """
     measure = measures.TransitionLagRank(
-        item_query=item_query, test_key=test_key, test=test
+        lag_key=lag_key, item_query=item_query, test_key=test_key, test=test
     )
     rank = measure.analyze(df)
     return rank
 
 
 def distance_crp(
     df,
@@ -1282,14 +1278,15 @@
     distances,
     edges,
     centers=None,
     count_unique=False,
     item_query=None,
     test_key=None,
     test=None,
+    drop_bin=False,
 ):
     """
     Conditional response probability by distance bin.
 
     Parameters
     ----------
     df : pandas.DataFrame
@@ -1361,41 +1358,42 @@
     >>> from psifr import fr
     >>> raw = fr.sample_data('Morton2013')
     >>> data = fr.merge_free_recall(raw)
     >>> items, distances = fr.sample_distances('Morton2013')
     >>> data['item_index'] = fr.pool_index(data['item'], items)
     >>> edges = np.percentile(squareform(distances), np.linspace(1, 99, 10))
     >>> fr.distance_crp(data, 'item_index', distances, edges)
-                                 bin      prob  actual  possible
-    subject center                                              
-    1       0.467532  (0.352, 0.583]  0.085456     151      1767
-            0.617748  (0.583, 0.653]  0.067916      87      1281
-            0.673656  (0.653, 0.695]  0.062500      65      1040
-            0.711075  (0.695, 0.727]  0.051836      48       926
-            0.742069  (0.727, 0.757]  0.050633      44       869
-    ...                          ...       ...     ...       ...
-    47      0.742069  (0.727, 0.757]  0.062822      61       971
-            0.770867  (0.757, 0.785]  0.030682      27       880
-            0.800404  (0.785, 0.816]  0.040749      37       908
-            0.834473  (0.816, 0.853]  0.046651      39       836
-            0.897275  (0.853, 0.941]  0.028868      25       866
+         subject    center             bin      prob  actual  possible
+    0          1  0.467532  (0.352, 0.583]  0.085456     151      1767
+    1          1  0.617748  (0.583, 0.653]  0.067916      87      1281
+    2          1  0.673656  (0.653, 0.695]  0.062500      65      1040
+    3          1  0.711075  (0.695, 0.727]  0.051836      48       926
+    4          1  0.742069  (0.727, 0.757]  0.050633      44       869
+    ..       ...       ...             ...       ...     ...       ...
+    355       47  0.742069  (0.727, 0.757]  0.062822      61       971
+    356       47  0.770867  (0.757, 0.785]  0.030682      27       880
+    357       47  0.800404  (0.785, 0.816]  0.040749      37       908
+    358       47  0.834473  (0.816, 0.853]  0.046651      39       836
+    359       47  0.897275  (0.853, 0.941]  0.028868      25       866
     <BLANKLINE>
-    [360 rows x 4 columns]
+    [360 rows x 6 columns]
     """
     measure = measures.TransitionDistance(
         index_key,
         distances,
         edges,
         centers=centers,
         count_unique=count_unique,
         item_query=item_query,
         test_key=test_key,
         test=test,
     )
     crp = measure.analyze(df)
+    if drop_bin:
+        crp = crp.drop(columns=['bin'])
     return crp
 
 
 def distance_rank(df, index_key, distances, item_query=None, test_key=None, test=None):
     """
     Calculate rank of transition distances in free recall lists.
 
@@ -1445,21 +1443,20 @@
     >>> from psifr import fr
     >>> raw = fr.sample_data('Morton2013')
     >>> data = fr.merge_free_recall(raw)
     >>> items, distances = fr.sample_distances('Morton2013')
     >>> data['item_index'] = fr.pool_index(data['item'], items)
     >>> dist_rank = fr.distance_rank(data, 'item_index', distances)
     >>> dist_rank.head()
-                 rank
-    subject          
-    1        0.635571
-    2        0.571457
-    3        0.627282
-    4        0.637596
-    5        0.646181
+       subject      rank
+    0        1  0.635571
+    1        2  0.571457
+    2        3  0.627282
+    3        4  0.637596
+    4        5  0.646181
     """
     measure = measures.TransitionDistanceRank(
         index_key, distances, item_query=item_query, test_key=test_key, test=test
     )
     rank = measure.analyze(df)
     return rank
 
@@ -1520,32 +1517,36 @@
     >>> from psifr import fr
     >>> raw = fr.sample_data('Morton2013')
     >>> data = fr.merge_free_recall(raw)
     >>> items, distances = fr.sample_distances('Morton2013')
     >>> data['item_index'] = fr.pool_index(data['item'], items)
     >>> dist_rank = fr.distance_rank_shifted(data, 'item_index', distances, 3)
     >>> dist_rank
-                       rank
-    subject shift          
-    1       -3     0.523426
-            -2     0.559199
-            -1     0.634392
-    2       -3     0.475931
-            -2     0.507574
-    ...                 ...
-    46      -2     0.515332
-            -1     0.603304
-    47      -3     0.542951
-            -2     0.565001
-            -1     0.635415
+         subject  shift      rank
+    0          1     -3  0.523426
+    1          1     -2  0.559199
+    2          1     -1  0.634392
+    3          2     -3  0.475931
+    4          2     -2  0.507574
+    ..       ...    ...       ...
+    115       46     -2  0.515332
+    116       46     -1  0.603304
+    117       47     -3  0.542951
+    118       47     -2  0.565001
+    119       47     -1  0.635415
     <BLANKLINE>
-    [120 rows x 1 columns]
+    [120 rows x 3 columns]
     """
     measure = measures.TransitionDistanceRankShifted(
-        index_key, distances, max_shift, item_query=item_query, test_key=test_key, test=test
+        index_key,
+        distances,
+        max_shift,
+        item_query=item_query,
+        test_key=test_key,
+        test=test,
     )
     rank = measure.analyze(df)
     return rank
 
 
 def distance_rank_window(
     df, index_key, distances, window_lags, item_query=None, test_key=None, test=None
@@ -1655,37 +1656,36 @@
     Examples
     --------
     >>> from psifr import fr
     >>> raw = fr.sample_data('Morton2013')
     >>> data = fr.merge_free_recall(raw, study_keys=['category'])
     >>> cat_crp = fr.category_crp(data, 'category')
     >>> cat_crp.head()
-                 prob  actual  possible
-    subject                            
-    1        0.801147     419       523
-    2        0.733456     399       544
-    3        0.763158     377       494
-    4        0.814882     449       551
-    5        0.877273     579       660
+       subject      prob  actual  possible
+    0        1  0.801147     419       523
+    1        2  0.733456     399       544
+    2        3  0.763158     377       494
+    3        4  0.814882     449       551
+    4        5  0.877273     579       660
     """
     measure = measures.TransitionCategory(
         category_key, item_query=item_query, test_key=test_key, test=test
     )
     crp = measure.analyze(df)
     return crp
 
 
 def _subject_category_clustering(df, category_key):
     """Subject category clustering."""
     study = split_lists(df, 'study', keys=[category_key])
     recall = split_lists(df, 'recall', keys=[category_key])
-    lbc = clustering.lbc(study[category_key], recall[category_key])
-    arc = clustering.arc(recall[category_key])
-    stats = pd.Series({'lbc': np.nanmean(lbc), 'arc': np.nanmean(arc)})
-    return stats
+    lbc = stats.lbc(study[category_key], recall[category_key])
+    arc = stats.arc(recall[category_key])
+    clust = pd.Series({'lbc': np.nanmean(lbc), 'arc': np.nanmean(arc)})
+    return clust
 
 
 def category_clustering(df, category_key):
     """
     Category clustering of recall sequences.
 
     Calculates ARC (adjusted ratio of clustering) and LBC (list-based
@@ -1721,26 +1721,26 @@
     --------
     >>> from psifr import fr
     >>> raw = fr.sample_data('Morton2013')
     >>> mixed = raw.query('list_type == "mixed"')
     >>> data = fr.merge_free_recall(mixed, list_keys=['category'])
     >>> stats = fr.category_clustering(data, 'category')
     >>> stats.head()
-                  lbc       arc
-    subject                    
-    1        3.657971  0.614545
-    2        2.953623  0.407839
-    3        3.363768  0.627371
-    4        4.444928  0.688761
-    5        7.530435  0.873755
+       subject       lbc       arc
+    0        1  3.657971  0.614545
+    1        2  2.953623  0.407839
+    2        3  3.363768  0.627371
+    3        4  4.444928  0.688761
+    4        5  7.530435  0.873755
     """
     # these analyses are undefined when there are repeats and
     # intrusions, so strip them out
     clean = df.query('~intrusion and repeat == 0')
     stats = clean.groupby('subject').apply(_subject_category_clustering, category_key)
+    stats = stats.reset_index()
     return stats
 
 
 def plot_spc(recall, **facet_kws):
     """
     Plot a serial position curve.
 
@@ -1864,17 +1864,15 @@
     facet_kws
         Additional keywords for the FacetGrid.
     """
     g = sns.FacetGrid(data=data.reset_index(), dropna=False, **facet_kws)
     g.map_dataframe(
         sns.swarmplot, x=x, y=y, color=swarm_color, size=swarm_size, zorder=1
     )
-    g.map_dataframe(
-        sns.pointplot, x=x, y=y, color=point_color, join=False, capsize=0.5
-    )
+    g.map_dataframe(sns.pointplot, x=x, y=y, color=point_color, join=False, capsize=0.5)
     return g
 
 
 def plot_raster(
     df,
     hue='input',
     palette=None,
```

### Comparing `psifr-0.8.2/src/psifr/measures.py` & `psifr-0.9.0/src/psifr/measures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Classes for defining recall measures."""
 
 import abc
 
 import numpy as np
 import pandas as pd
 
+from psifr import stats
 from psifr import fr
-from psifr import transitions
-from psifr import outputs
 
 
 class TransitionMeasure(object):
     """
     Measure of free recall dataset with multiple subjects.
 
     Parameters
@@ -115,29 +114,29 @@
         """
         subj_results = []
         for subject, subject_data in data.groupby('subject'):
             pool_lists = self.split_lists(subject_data, 'study', self.item_query)
             recall_lists = self.split_lists(subject_data, 'recall')
             results = self.analyze_subject(subject, pool_lists, recall_lists)
             subj_results.append(results)
-        stat = pd.concat(subj_results, axis=0)
+        stat = pd.concat(subj_results, axis=0).reset_index()
         return stat
 
 
 class TransitionOutputs(TransitionMeasure):
     """Measure recall probability by input and output position."""
 
     def __init__(self, list_length, item_query=None, test_key=None, test=None):
         super().__init__(
             'input', 'input', item_query=item_query, test_key=test_key, test=test
         )
         self.list_length = list_length
 
     def analyze_subject(self, subject, pool, recall):
-        actual, possible = outputs.count_outputs(
+        actual, possible = stats.count_outputs(
             self.list_length,
             pool['items'],
             recall['items'],
             pool['label'],
             recall['label'],
             pool['test'],
             recall['test'],
@@ -180,17 +179,17 @@
         self.list_length = list_length
         self.count_unique = count_unique
         self.compound = compound
 
     def analyze_subject(self, subject, pool, recall):
 
         if self.compound:
-            counter = transitions.count_lags_compound
+            counter = stats.count_lags_compound
         else:
-            counter = transitions.count_lags
+            counter = stats.count_lags
 
         actual, possible = counter(
             self.list_length,
             pool['items'],
             recall['items'],
             pool['label'],
             recall['label'],
@@ -201,35 +200,36 @@
         )
         crp = pd.DataFrame(
             {
                 'subject': subject,
                 'prob': actual / possible,
                 'actual': actual,
                 'possible': possible,
-            }, index=actual.index
+            },
+            index=actual.index,
         )
         if self.compound:
             crp = crp.set_index('subject', append=True)
             crp = crp.reorder_levels(['subject', 'previous', 'current'])
         else:
             crp = crp.set_index('subject', append=True)
             crp = crp.reorder_levels(['subject', 'lag'])
         return crp
 
 
 class TransitionLagRank(TransitionMeasure):
     """Measure lag rank of transitions."""
 
-    def __init__(self, item_query=None, test_key=None, test=None):
+    def __init__(self, lag_key='input', item_query=None, test_key=None, test=None):
         super().__init__(
-            'input', 'input', item_query=item_query, test_key=test_key, test=test
+            'input', lag_key, item_query=item_query, test_key=test_key, test=test
         )
 
     def analyze_subject(self, subject, pool, recall):
-        ranks = transitions.rank_lags(
+        ranks = stats.rank_lags(
             pool['items'],
             recall['items'],
             pool['label'],
             recall['label'],
             pool['test'],
             recall['test'],
             self.test,
@@ -264,15 +264,15 @@
             # if no explicit centers, use halfway between edges
             centers = edges[:-1] + (np.diff(edges) / 2)
         self.centers = centers
         self.count_unique = count_unique
 
     def analyze_subject(self, subject, pool, recall):
 
-        actual, possible = transitions.count_distance(
+        actual, possible = stats.count_distance(
             self.distances,
             self.edges,
             pool['items'],
             recall['items'],
             pool['label'],
             recall['label'],
             pool['test'],
@@ -300,15 +300,15 @@
     def __init__(self, index_key, distances, item_query=None, test_key=None, test=None):
         super().__init__(
             index_key, index_key, item_query=item_query, test_key=test_key, test=test
         )
         self.distances = distances
 
     def analyze_subject(self, subject, pool, recall):
-        ranks = transitions.rank_distance(
+        ranks = stats.rank_distance(
             self.distances,
             pool['items'],
             recall['items'],
             pool['label'],
             recall['label'],
             pool['test'],
             recall['test'],
@@ -327,18 +327,18 @@
     def __init__(
         self, index_key, distances, max_shift, item_query=None, test_key=None, test=None
     ):
         super().__init__(
             index_key, index_key, item_query=item_query, test_key=test_key, test=test
         )
         self.distances = distances
-        self.max_shift = max_shift
+        self.max_shift = int(max_shift)
 
     def analyze_subject(self, subject, pool, recall):
-        ranks = transitions.rank_distance_shifted(
+        ranks = stats.rank_distance_shifted(
             self.distances,
             self.max_shift,
             pool['items'],
             recall['items'],
             pool['label'],
             recall['label'],
             pool['test'],
@@ -370,15 +370,15 @@
             'input', index_key, item_query=item_query, test_key=test_key, test=test
         )
         self.distances = distances
         self.list_length = list_length
         self.window_lags = window_lags
 
     def analyze_subject(self, subject, pool, recall):
-        ranks = transitions.rank_distance_window(
+        ranks = stats.rank_distance_window(
             self.distances,
             self.list_length,
             self.window_lags,
             pool['items'],
             recall['items'],
             pool['label'],
             recall['label'],
@@ -399,15 +399,15 @@
 
     def __init__(self, category_key, item_query=None, test_key=None, test=None):
         super().__init__(
             'input', category_key, item_query=item_query, test_key=test_key, test=test
         )
 
     def analyze_subject(self, subject, pool, recall):
-        actual, possible = transitions.count_category(
+        actual, possible = stats.count_category(
             pool['items'],
             recall['items'],
             pool['label'],
             recall['label'],
             pool['test'],
             recall['test'],
             self.test,
```

### Comparing `psifr-0.8.2/src/psifr/transitions.py` & `psifr-0.9.0/src/psifr/stats.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-"""Module to analyze transitions during free recall."""
-
+"""Calculate statistics of list recall."""
 import itertools
+
+import numpy
 import numpy as np
-from scipy import stats
 import pandas as pd
+import scipy.stats
+
+from psifr import maskers
 
 
 def percentile_rank(actual, possible):
     """
     Get percentile rank of a score compared to possible scores.
 
     Parameters
@@ -21,390 +24,142 @@
     Returns
     -------
     rank : float
         Rank scaled to range from 0 (low score) to 1 (high score).
 
     Examples
     --------
-    >>> from psifr import transitions
+    >>> from psifr import stats
     >>> actual = 3
     >>> possible = [1, 2, 2, 2, 3]
-    >>> transitions.percentile_rank(actual, possible)
+    >>> stats.percentile_rank(actual, possible)
     1.0
     """
-    possible_rank = stats.rankdata(possible)
+    possible_rank = scipy.stats.rankdata(possible)
     actual_rank = possible_rank[actual == np.asarray(possible)]
     possible_count = np.count_nonzero(~np.isnan(possible))
     if possible_count == 1:
         return np.nan
     rank = (actual_rank - 1) / (possible_count - 1)
     return rank[0]
 
 
-def transitions_masker(
-    pool_items,
-    recall_items,
-    pool_output,
-    recall_output,
-    pool_test=None,
-    recall_test=None,
-    test=None,
-):
-    """
-    Iterate over transitions with masking.
-
-    Transitions are between a "previous" item and a "current" item.
-    Non-included transitions will be skipped. A transition is yielded
-    only if it matches the following conditions:
-
-    (1) Each item involved in the transition is in the pool. Items are
-    removed from the pool after they appear as the previous item.
-
-    (2) Optionally, an additional check is run based on test values
-    associated with the items in the transition. For example, this
-    could be used to only include transitions where the category of
-    the previous and current items is the same.
-
-    The masker will yield "output" values, which may be distinct from
-    the item identifiers used to determine item repeats.
-
-    Parameters
-    ----------
-    pool_items : list
-        Items available for recall. Order does not matter. May contain
-        repeated values. Item identifiers must be unique within pool.
-
-    recall_items : list
-        Recalled items in output position order.
-
-    pool_output : list
-        Output values for pool items. Must be the same order as pool.
-
-    recall_output : list
-        Output values in output position order.
-
-    pool_test : list, optional
-        Test values for items available for recall. Must be the same
-        order as pool.
-
-    recall_test : list, optional
-        Test values for items in output position order.
-
-    test : callable, optional
-        Used to test whether individual transitions should be included,
-        based on test values.
-
-            test(prev, curr) - test for included transition
-
-            test(prev, poss) - test for included possible transition
-
-    Yields
-    ------
-    output : int
-        Output position of this transition. The first transition is 1.
-
-    prev : object
-        Output value for the "from" item on this transition.
-
-    curr : object
-        Output value for the "to" item.
-
-    poss : numpy.array
-        Output values for all possible valid "to" items.
-
-    Examples
-    --------
-    >>> from psifr import transitions
-    >>> pool = [1, 2, 3, 4, 5, 6]
-    >>> recs = [6, 2, 3, 6, 1, 4]
-    >>> masker = transitions.transitions_masker(
-    ...     pool_items=pool, recall_items=recs, pool_output=pool, recall_output=recs
-    ... )
-    >>> for output, prev, curr, poss in masker:
-    ...     print(output, prev, curr, poss)
-    1 6 2 [1 2 3 4 5]
-    2 2 3 [1 3 4 5]
-    5 1 4 [4 5]
-    """
-    pool_items = pool_items.copy()
-    pool_output = pool_output.copy()
-    if test is not None:
-        pool_test = pool_test.copy()
-
-    for n in range(len(recall_items) - 1):
-        # test if the previous item is in the pool
-        if pd.isnull(recall_items[n]) or (recall_items[n] not in pool_items):
-            continue
-
-        # remove the item from the pool
-        ind = pool_items.index(recall_items[n])
-        del pool_items[ind]
-        del pool_output[ind]
-        if test is not None:
-            del pool_test[ind]
-
-        # test if the current item is in the pool
-        if pd.isnull(recall_items[n + 1]) or (recall_items[n + 1] not in pool_items):
-            continue
-
-        prev = recall_output[n]
-        curr = recall_output[n + 1]
-        poss = np.array(pool_output)
-        if test is not None:
-            # test if this transition is included
-            if not test(recall_test[n], recall_test[n + 1]):
-                continue
-
-            # get included possible items
-            ind = test(recall_test[n], np.array(pool_test))
-            if not isinstance(ind, np.ndarray):
-                ind = np.repeat(ind, poss.shape)
-            poss = poss[ind]
-        yield n + 1, prev, curr, poss
-
-
-def sequences_masker(
-    n_transitions,
-    pool_items,
-    recall_items,
-    pool_output,
-    recall_output,
-    pool_test=None,
-    recall_test=None,
-    test=None,
-):
-    """
-    Yield sequences of adjacent included transitions.
-
-    Parameters
-    ----------
-    n_transitions : int
-        Number of transitions to include in yielded sequences.
-
-    pool_items : list
-        Items available for recall. Order does not matter. May contain
-        repeated values. Item identifiers must be unique within pool.
-
-    recall_items : list
-        Recalled items in output position order.
-
-    pool_output : list
-        Output values for pool items. Must be the same order as pool.
-
-    recall_output : list
-        Output values in output position order.
-
-    pool_test : list, optional
-        Test values for items available for recall. Must be the same
-        order as pool.
-
-    recall_test : list, optional
-        Test values for items in output position order.
-
-    test : callable, optional
-        Used to test whether individual transitions should be included,
-        based on test values.
-
-            test(prev, curr) - test for included transition
-
-            test(prev, poss) - test for included possible transition
-
-    Yields
-    ------
-    output : int
-        Output positions of included transitions. The first transition
-        is 1.
-
-    prev : list
-        Output values for the "from" item in included transitions.
-
-    curr : list
-        Output values for the "to" item in included transitions.
-
-    poss : list of numpy.ndarray
-        Output values for all possible valid "to" items in included
-        transitions.
-
-    See Also
-    --------
-    transitions_masker : Yield included transitions.
-
-    Examples
-    --------
-    >>> from psifr import transitions
-    >>> pool = [1, 2, 3, 4, 5, 6]
-    >>> recs = [6, 2, 3, 6, 1, 4, 5]
-    >>> masker = transitions.sequences_masker(
-    ...     2, pool_items=pool, recall_items=recs, pool_output=pool, recall_output=recs
-    ... )
-    >>> for output, prev, curr, poss in masker:
-    ...     print(output, prev, curr, poss)
-    [1, 2] [6, 2] [2, 3] [array([1, 2, 3, 4, 5]), array([1, 3, 4, 5])]
-    [5, 6] [1, 4] [4, 5] [array([4, 5]), array([5])]
-
-    >>> pool = [1, 2, 3, 4]
-    >>> recs = [4, 3, 1, 2]
-    >>> masker = transitions.sequences_masker(
-    ...     3, pool_items=pool, recall_items=recs, pool_output=pool, recall_output=recs
-    ... )
-    >>> for output, prev, curr, poss in masker:
-    ...     print(output, prev, curr, poss)
-    [1, 2, 3] [4, 3, 1] [3, 1, 2] [array([1, 2, 3]), array([1, 2]), array([2])]
-    """
-    masker = transitions_masker(
-        pool_items,
-        recall_items,
-        pool_output,
-        recall_output,
-        pool_test=pool_test,
-        recall_test=recall_test,
-        test=test,
-    )
-    s_output = []
-    s_prev = []
-    s_curr = []
-    s_poss = []
-    prev_output = 0
-    sequence_len = 0
-    for output, prev, curr, poss in masker:
-        if (output - prev_output) == 1:
-            s_output.append(output)
-            s_prev.append(prev)
-            s_curr.append(curr)
-            s_poss.append(poss)
-            sequence_len += 1
-        else:
-            # a break in the chain
-            s_output = [output]
-            s_prev = [prev]
-            s_curr = [curr]
-            s_poss = [poss]
-            sequence_len = 1
-        prev_output = output
-
-        if sequence_len >= n_transitions:
-            ind = slice(sequence_len - n_transitions, None)
-            yield s_output[ind], s_prev[ind], s_curr[ind], s_poss[ind]
-
-
-def windows_masker(
+def count_outputs(
     list_length,
-    window_lags,
     pool_items,
     recall_items,
-    pool_output,
-    recall_output,
+    pool_label,
+    recall_label,
     pool_test=None,
     recall_test=None,
     test=None,
+    count_unique=False,
 ):
     """
-    Yield windows around previous items in the input list.
+    Count actual and possible recalls for each output position.
 
     Parameters
     ----------
     list_length : int
         Number of items in each list.
 
-    window_lags : array_like
-        Serial position lags to include in the window.
-
     pool_items : list
-        Input position of items available for recall.
+        List of the serial positions available for recall in each list.
+        Must match the serial position codes used in `recall_items`.
 
     recall_items : list
-        Input position of recalled items, in output position order.
+        List indicating the serial position of each recall in output
+        order (NaN for intrusions).
 
-    pool_output : list
-        Output values for pool items. Must be the same order as pool.
+    pool_label : list
+        List of the positions to use for calculating lag. Default is to
+        use `pool_items`.
 
-    recall_output : list
-        Output values in output position order.
+    recall_label : list
+        List of position labels in recall order. Default is to use
+        `recall_items`.
 
     pool_test : list, optional
-        Test values for items available for recall. Must be the same
-        order as pool.
+         List of some test value for each item in the pool.
 
     recall_test : list, optional
-        Test values for items in output position order.
-
-    test : callable, optional
-        Used to test whether individual transitions should be included,
-        based on test values.
-
-            test(prev, curr) - test for included transition
+        List of some test value for each recall attempt by output
+        position.
 
-            test(prev, poss) - test for included possible transition
+    test : callable
+        Callable that evaluates each transition between items n and
+        n+1. Must take test values for items n and n+1 and return True
+        if a given transition should be included.
 
-    Yields
-    ------
-    output : int
-        Output positions of included transitions. The first transition
-        is 1.
+    count_unique : bool
+        If true, possible recalls with the same label will only be
+        counted once.
 
-    prev : list
-        Output values for the "from" item in included transitions.
+    Returns
+    -------
+    actual : numpy.ndarray
+        [outputs x inputs] array of actual recall counts.
 
-    curr : list
-        Output values for the "to" item in included transitions.
+    possible : numpy.ndarray
+        [outputs x inputs] array of possible recall counts.
 
-    poss : list of numpy.ndarray
-        Output values for all possible valid "to" items in included
-        transitions.
+    Examples
+    --------
+    >>> from psifr import stats
+    >>> pool_items = [[1, 2, 3, 4]]
+    >>> recall_items = [[4, 2, 3, 1]]
+    >>> actual, possible = stats.count_outputs(
+    ...     4, pool_items, recall_items, pool_items, recall_items
+    ... )
+    >>> actual
+    array([[0, 0, 0, 1],
+           [0, 1, 0, 0],
+           [0, 0, 1, 0],
+           [1, 0, 0, 0]])
+    >>> possible
+    array([[1, 1, 1, 1],
+           [1, 1, 1, 0],
+           [1, 0, 1, 0],
+           [1, 0, 0, 0]])
     """
-    # pool items include all items in presentation order; poss items
-    # include only items that have not been recalled yet
-    poss_items = pool_items.copy()
-    poss_output = pool_output.copy()
-    pool_output = np.asarray(pool_output)
-    if test is not None:
-        poss_test = pool_test.copy()
-        pool_test = np.asarray(pool_test)
-    window_lags = np.asarray(window_lags)
-
-    for n in range(len(recall_items) - 1):
-        # test if the previous item is in the pool
-        if pd.isnull(recall_items[n]) or (recall_items[n] not in poss_items):
-            continue
-
-        # remove the item from the pool
-        ind = poss_items.index(recall_items[n])
-        del poss_items[ind]
-        del poss_output[ind]
-        if test is not None:
-            del poss_test[ind]
+    if pool_label is None:
+        pool_label = pool_items
 
-        # test if the current item is in the pool
-        if pd.isnull(recall_items[n + 1]) or (recall_items[n + 1] not in poss_items):
-            continue
+    if recall_label is None:
+        recall_label = recall_items
 
-        # get windowed items in the input list
-        prev = int(recall_items[n]) + window_lags
+    count_actual = np.zeros((list_length, list_length), dtype=int)
+    count_possible = np.zeros((list_length, list_length), dtype=int)
+    for i, recall_items_list in enumerate(recall_items):
+        # set up masker to filter outputs
+        pool_test_list = None if pool_test is None else pool_test[i]
+        recall_test_list = None if recall_test is None else recall_test[i]
+        masker = maskers.outputs_masker(
+            pool_items[i],
+            recall_items_list,
+            pool_label[i],
+            recall_label[i],
+            pool_test_list,
+            recall_test_list,
+            test,
+        )
 
-        # exclude if any windowed items do not exist or fail test
-        if np.any(prev < 1) or np.any(prev > list_length):
-            continue
+        for curr, poss, op in masker:
+            curr = int(curr)
+            poss = poss.astype(int)
 
-        # exclude current/possible items in the window
-        curr = int(recall_items[n + 1])
-        if curr in prev:
-            continue
-        poss = np.asarray(poss_items, int)
-        include_poss = ~np.isin(poss, prev)
-        poss = poss[include_poss]
-
-        if test is not None:
-            # test if this transition is included
-            if np.any(~test(pool_test[prev - 1], recall_test[n + 1])):
-                continue
-
-            # get included possible items
-            include = test(pool_test[prev - 1][:, np.newaxis], pool_test[poss - 1])
-            poss = poss[np.all(include, axis=0)]
-        yield n + 1, pool_output[prev - 1], pool_output[curr - 1], pool_output[poss - 1]
+            # for this step, calculate actual input position and
+            # possible input positions
+            count_actual[op - 1, curr - 1] += 1
+            if count_unique:
+                for j in poss:
+                    count_possible[op - 1, j - 1] += 1
+            else:
+                count_possible[op - 1, poss - 1] += 1
+    return count_actual, count_possible
 
 
 def count_lags(
     list_length,
     pool_items,
     recall_items,
     pool_label=None,
@@ -467,18 +222,18 @@
 
     See Also
     --------
     rank_lags : Rank of serial position lags.
 
     Examples
     --------
-    >>> from psifr import transitions
+    >>> from psifr import stats
     >>> pool_items = [[1, 2, 3, 4]]
     >>> recall_items = [[4, 2, 3, 1]]
-    >>> actual, possible = transitions.count_lags(4, pool_items, recall_items)
+    >>> actual, possible = stats.count_lags(4, pool_items, recall_items)
     >>> actual
     lag
     -3    0
     -2    2
     -1    0
      0    0
      1    1
@@ -504,15 +259,15 @@
 
     list_actual = []
     list_possible = []
     for i, recall_items_list in enumerate(recall_items):
         # set up masker to filter transitions
         pool_test_list = None if pool_test is None else pool_test[i]
         recall_test_list = None if recall_test is None else recall_test[i]
-        masker = transitions_masker(
+        masker = maskers.transitions_masker(
             pool_items[i],
             recall_items_list,
             pool_label[i],
             recall_label[i],
             pool_test_list,
             recall_test_list,
             test,
@@ -599,18 +354,18 @@
 
     See Also
     --------
     count_lags : Count of individual transitions.
 
     Examples
     --------
-    >>> from psifr import transitions
+    >>> from psifr import stats
     >>> pool_items = [[1, 2, 3]]
     >>> recall_items = [[3, 1, 2]]
-    >>> actual, possible = transitions.count_lags_compound(3, pool_items, recall_items)
+    >>> actual, possible = stats.count_lags_compound(3, pool_items, recall_items)
     >>> (actual == possible).all()
     True
     >>> actual
     previous  current
     -2        -2         0
               -1         0
                0         0
@@ -648,15 +403,15 @@
     prev_possible = []
     curr_actual = []
     curr_possible = []
     for i, recall_items_list in enumerate(recall_items):
         # set up masker to filter pairs of transitions
         pool_test_list = None if pool_test is None else pool_test[i]
         recall_test_list = None if recall_test is None else recall_test[i]
-        masker = sequences_masker(
+        masker = maskers.sequences_masker(
             2,
             pool_items[i],
             recall_items_list,
             pool_label[i],
             recall_label[i],
             pool_test_list,
             recall_test_list,
@@ -747,32 +502,32 @@
 
     See Also
     --------
     count_lags : Count actual and possible serial position lags.
 
     Examples
     --------
-    >>> from psifr import transitions
+    >>> from psifr import stats
     >>> pool_items = [[1, 2, 3, 4]]
     >>> recall_items = [[4, 2, 3, 1]]
-    >>> transitions.rank_lags(pool_items, recall_items)
+    >>> stats.rank_lags(pool_items, recall_items)
     [0.5, 0.5, nan]
     """
     if pool_label is None:
         pool_label = pool_items
 
     if recall_label is None:
         recall_label = recall_items
 
     rank = []
     for i, recall_items_list in enumerate(recall_items):
         # set up masker to filter transitions
         pool_test_list = None if pool_test is None else pool_test[i]
         recall_test_list = None if recall_test is None else recall_test[i]
-        masker = transitions_masker(
+        masker = maskers.transitions_masker(
             pool_items[i],
             recall_items_list,
             pool_label[i],
             recall_label[i],
             pool_test_list,
             recall_test_list,
             test,
@@ -848,42 +603,42 @@
     See Also
     --------
     rank_distance : Calculate percentile rank of transition distances.
 
     Examples
     --------
     >>> import numpy as np
-    >>> from psifr import transitions
+    >>> from psifr import stats
     >>> distances = np.array([[0, 1, 2, 2], [1, 0, 2, 2], [2, 2, 0, 3], [2, 2, 3, 0]])
     >>> edges = np.array([0.5, 1.5, 2.5, 3.5])
     >>> pool_items = [[1, 2, 3, 4]]
     >>> recall_items = [[4, 2, 3, 1]]
     >>> pool_index = [[0, 1, 2, 3]]
     >>> recall_index = [[3, 1, 2, 0]]
-    >>> actual, possible = transitions.count_distance(
+    >>> actual, possible = stats.count_distance(
     ...     distances, edges, pool_items, recall_items, pool_index, recall_index
     ... )
     >>> actual
     (0.5, 1.5]    0
     (1.5, 2.5]    3
     (2.5, 3.5]    0
-    dtype: int64
+    Name: count, dtype: int64
     >>> possible
     (0.5, 1.5]    1
     (1.5, 2.5]    4
     (2.5, 3.5]    1
-    dtype: int64
+    Name: count, dtype: int64
     """
     list_actual = []
     list_possible = []
     centers = edges[:-1] + np.diff(edges) / 2
     for i in range(len(recall_items)):
         pool_test_list = None if pool_test is None else pool_test[i]
         recall_test_list = None if recall_test is None else recall_test[i]
-        masker = transitions_masker(
+        masker = maskers.transitions_masker(
             pool_items[i],
             recall_items[i],
             pool_index[i],
             recall_index[i],
             pool_test_list,
             recall_test_list,
             test,
@@ -960,30 +715,30 @@
     See Also
     --------
     count_distance : Count transitions within distance bins.
 
     Examples
     --------
     >>> import numpy as np
-    >>> from psifr import transitions
+    >>> from psifr import stats
     >>> distances = np.array([[0, 1, 2, 2], [1, 0, 2, 2], [2, 2, 0, 3], [2, 2, 3, 0]])
     >>> pool_items = [[1, 2, 3, 4]]
     >>> recall_items = [[4, 2, 3, 1]]
     >>> pool_index = [[0, 1, 2, 3]]
     >>> recall_index = [[3, 1, 2, 0]]
-    >>> transitions.rank_distance(
+    >>> stats.rank_distance(
     ...     distances, pool_items, recall_items, pool_index, recall_index
     ... )
     [0.75, 0.0, nan]
     """
     rank = []
     for i in range(len(recall_items)):
         pool_test_list = None if pool_test is None else pool_test[i]
         recall_test_list = None if recall_test is None else recall_test[i]
-        masker = transitions_masker(
+        masker = maskers.transitions_masker(
             pool_items[i],
             recall_items[i],
             pool_index[i],
             recall_index[i],
             pool_test_list,
             recall_test_list,
             test,
@@ -1054,39 +809,39 @@
     --------
     rank_distance - Percentile rank of transition distances relative
         to the immediately preceding item only.
 
     Examples
     --------
     >>> import numpy as np
-    >>> from psifr import transitions
+    >>> from psifr import stats
     >>> distances = np.array(
     ...     [
     ...         [0, 1, 2, 2, 2],
     ...         [1, 0, 2, 2, 2],
     ...         [2, 2, 0, 3, 3],
     ...         [2, 2, 3, 0, 2],
     ...         [2, 2, 3, 2, 0],
     ...     ]
     ... )
     >>> pool_items = [[1, 2, 3, 4, 5]]
     >>> recall_items = [[4, 2, 3, 1]]
     >>> pool_index = [[0, 1, 2, 3, 4]]
     >>> recall_index = [[3, 1, 2, 0]]
-    >>> transitions.rank_distance_shifted(
+    >>> stats.rank_distance_shifted(
     ...     distances, 2, pool_items, recall_items, pool_index, recall_index
     ... )
     array([[0.  , 0.25],
            [1.  , 1.  ]])
     """
     rank = []
     for i in range(len(recall_items)):
         pool_test_list = None if pool_test is None else pool_test[i]
         recall_test_list = None if recall_test is None else recall_test[i]
-        masker = sequences_masker(
+        masker = maskers.sequences_masker(
             max_shift,
             pool_items[i],
             recall_items[i],
             pool_index[i],
             recall_index[i],
             pool_test_list,
             recall_test_list,
@@ -1163,28 +918,31 @@
         transitions, and 1 if the distance was the smallest. Ties are
         assigned to the average percentile rank.
     """
     rank = []
     for i in range(len(recall_items)):
         pool_test_list = None if pool_test is None else pool_test[i]
         recall_test_list = None if recall_test is None else recall_test[i]
-        masker = windows_masker(
+        masker = maskers.windows_masker(
             list_length,
             window_lags,
             pool_items[i],
             recall_items[i],
             pool_index[i],
             recall_index[i],
             pool_test_list,
             recall_test_list,
             test,
         )
         for output, w_prev, curr, poss in masker:
+            curr = int(curr)
             rank_lag = []
             for prev in w_prev:
+                prev = int(prev)
+                poss = poss.astype(int)
                 actual = distances[prev, curr]
                 possible = distances[prev, poss]
                 rank_lag.append(1 - percentile_rank(actual, possible))
             rank.append(rank_lag)
     rank = np.array(rank)
     return rank
 
@@ -1235,31 +993,31 @@
         Count of actual within-category transitions.
 
     possible : int
         Count of possible within-category transitions.
 
     Examples
     --------
-    >>> from psifr import transitions
+    >>> from psifr import stats
     >>> pool_items = [[1, 2, 3, 4]]
     >>> recall_items = [[4, 3, 1, 2]]
     >>> pool_category = [[1, 1, 2, 2]]
     >>> recall_category = [[2, 2, 1, 1]]
-    >>> transitions.count_category(
+    >>> stats.count_category(
     ...     pool_items, recall_items, pool_category, recall_category
     ... )
     (2, 2)
     """
     actual = 0
     possible = 0
     for i in range(len(recall_items)):
         # set up masker to filter transitions
         pool_test_list = None if pool_test is None else pool_test[i]
         recall_test_list = None if recall_test is None else recall_test[i]
-        masker = transitions_masker(
+        masker = maskers.transitions_masker(
             pool_items[i],
             recall_items[i],
             pool_category[i],
             recall_category[i],
             pool_test_list,
             recall_test_list,
             test,
@@ -1279,21 +1037,76 @@
     """Count transitions between pairs of specific items."""
     actual = np.zeros((n_item, n_item), dtype=int)
     possible = np.zeros((n_item, n_item), dtype=int)
     for i, recall_items_list in enumerate(recall_items):
         # set up masker to filter transitions
         pool_test_list = None if pool_test is None else pool_test[i]
         recall_test_list = None if recall_test is None else recall_test[i]
-        masker = transitions_masker(
+        masker = maskers.transitions_masker(
             pool_items[i],
             recall_items_list,
             pool_items[i],
             recall_items_list,
             pool_test_list,
             recall_test_list,
             test,
         )
 
         for output, prev, curr, poss in masker:
             actual[prev, curr] += 1
             possible[prev, poss] += 1
     return actual, possible
+
+
+def lbc(study_category, recall_category):
+    """Calculate list-based clustering (LBC) for a set of lists."""
+    lbc_scores = np.zeros(len(study_category))
+    for i, (study, recall) in enumerate(zip(study_category, recall_category)):
+        study = np.asarray(study)
+        recall = np.asarray(recall)
+        if np.any(pd.isna(study)):
+            raise ValueError('Study category contains N/A values.')
+        if np.any(pd.isna(recall)):
+            raise ValueError('Recall category contains N/A values.')
+
+        # number of correct recalls
+        r = len(recall)
+
+        # number of items per category
+        m = len(study) / len(np.unique(study))
+
+        # list length
+        nl = len(study)
+
+        # observed and expected clustering
+        observed = np.count_nonzero(recall[:-1] == recall[1:])
+        expected = ((r - 1) * (m - 1)) / (nl - 1)
+        lbc_scores[i] = observed - expected
+    return lbc_scores
+
+
+def arc(recall_category):
+    """Calculate adjusted ratio of clustering for a set of lists."""
+    arc_scores = np.zeros(len(recall_category))
+    for i, recall in enumerate(recall_category):
+        recall = np.asarray(recall)
+        if np.any(pd.isna(recall)):
+            raise ValueError('Recall category contains N/A values.')
+
+        # number of categories and correct recalls from each category
+        categories = np.unique(recall)
+        n = np.array([np.count_nonzero(recall == c) for c in categories])
+        c = len(categories)
+
+        # number of correct recalls
+        r = len(recall)
+
+        # observed, expected, and maximum clustering
+        expected = np.sum((n * (n - 1)) / r)
+        observed = np.count_nonzero(recall[:-1] == recall[1:])
+        maximum = r - c
+        if maximum == expected:
+            # when maximum is the same as expected, ARC is undefined
+            arc_scores[i] = np.nan
+            continue
+        arc_scores[i] = (observed - expected) / (maximum - expected)
+    return arc_scores
```

### Comparing `psifr-0.8.2/src/psifr.egg-info/PKG-INFO` & `psifr-0.9.0/src/psifr.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: psifr
-Version: 0.8.2
+Version: 0.9.0
 Summary: Psifr: Analysis and visualization of free recall data
-Home-page: https://github.com/mortonne/psifr
-Author: Neal Morton
-Author-email: mortonne@gmail.com
+Author-email: Neal W Morton <mortonne@gmail.com>
 License: GPL-3.0-or-later
 Keywords: psychology,memory,free recall
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: perf
 License-File: LICENSE
 
 # Psifr
@@ -22,15 +21,21 @@
 [![Pytest](https://github.com/mortonne/psifr/actions/workflows/pytest.yml/badge.svg)](https://github.com/mortonne/psifr/actions/workflows/pytest.yml)
 [![codecov](https://codecov.io/gh/mortonne/psifr/branch/master/graph/badge.svg)](https://codecov.io/gh/mortonne/psifr)
 [![status](https://joss.theoj.org/papers/712d4452e465229d61d0e281d3d6f299/status.svg)](https://joss.theoj.org/papers/712d4452e465229d61d0e281d3d6f299)
 [![DOI](https://zenodo.org/badge/248593723.svg)](https://zenodo.org/badge/latestdoi/248593723)
 
 Advanced analysis and visualization of free recall data in Python.
 
-Psifr has tools to visualize recall sequences, to make it easier to see general trends in the data. Psifr also provides targeted analyses to examine factors that may affect recall, such as recency, primacy, temporal contiguity, stimulus category, and semantic relatedness. Analyses are customizable, allowing flexible filtering of included data to help answer precise questions. Extensive automated testing is used to ensure the consistency and correctness of analysis results. 
+Features:
+* A large library of advanced analyses, tested against published benchmarks
+* Flexible analysis customization and plotting
+* Tools for exploratory analysis of large datasets
+* Extensive automated testing to ensure analysis correctness
+* Based around a simple and flexible table-based data format
+* Comprehensive [documentation](https://psifr.readthedocs.io/en/stable/api/overview.html) and [user guide](https://psifr.readthedocs.io/en/stable/guide/overview.html)
 
 The name Psifr is pronounced "cipher". It's taken from Psi, in reference to the field of psychology, and FR for free recall.
 
 <div align="center">
   <div style="max-width:500px; margin:0 20px;">
     <img src="https://github.com/mortonne/psifr/blob/master/images/raster.png" alt="free recall visualization" width="500px">
     <div style="text-align:left; padding:10px 0;">
```

