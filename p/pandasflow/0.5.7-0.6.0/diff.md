# Comparing `tmp/pandasflow-0.5.7.tar.gz` & `tmp/pandasflow-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasflow-0.5.7.tar", last modified: Thu Jun  1 08:35:15 2023, max compression
+gzip compressed data, was "pandasflow-0.6.0.tar", last modified: Tue Jun  6 08:50:08 2023, max compression
```

## Comparing `pandasflow-0.5.7.tar` & `pandasflow-0.6.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 08:35:15.414077 pandasflow-0.5.7/
--rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.5.7/LICENCE
--rw-rw-rw-   0        0        0      869 2023-06-01 08:35:15.414077 pandasflow-0.5.7/PKG-INFO
--rw-rw-rw-   0        0        0      396 2023-05-15 11:35:26.000000 pandasflow-0.5.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 08:35:15.397489 pandasflow-0.5.7/pandasflow/
--rw-rw-rw-   0        0        0      391 2023-06-01 08:35:10.000000 pandasflow-0.5.7/pandasflow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 08:35:15.401479 pandasflow-0.5.7/pandasflow/dev/
--rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.5.7/pandasflow/dev/__init__.py
--rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.5.7/pandasflow/dev/err_mean_diff.py
--rw-rw-rw-   0        0        0      387 2023-05-30 09:54:40.000000 pandasflow-0.5.7/pandasflow/get_import.py
--rw-rw-rw-   0        0        0      480 2023-05-15 09:05:23.000000 pandasflow-0.5.7/pandasflow/get_psql.py
--rw-rw-rw-   0        0        0      208 2023-05-15 09:29:01.000000 pandasflow-0.5.7/pandasflow/get_sqlt.py
-drwxrwxrwx   0        0        0        0 2023-06-01 08:35:15.405148 pandasflow-0.5.7/pandasflow/metrics/
--rw-rw-rw-   0        0        0      324 2023-05-05 12:24:58.000000 pandasflow-0.5.7/pandasflow/metrics/__init__.py
--rw-rw-rw-   0        0        0      797 2023-06-01 08:27:10.000000 pandasflow-0.5.7/pandasflow/metrics/best_f1.py
--rw-rw-rw-   0        0        0     1132 2023-05-02 12:00:22.000000 pandasflow-0.5.7/pandasflow/metrics/conf_mat.py
--rw-rw-rw-   0        0        0     2173 2023-05-15 11:57:58.000000 pandasflow-0.5.7/pandasflow/metrics/lloss_up.py
--rw-rw-rw-   0        0        0      400 2023-04-26 15:19:05.000000 pandasflow-0.5.7/pandasflow/metrics/mean_error.py
--rw-rw-rw-   0        0        0      721 2023-05-07 08:19:28.000000 pandasflow-0.5.7/pandasflow/metrics/precision_recall.py
--rw-rw-rw-   0        0        0      654 2023-05-07 08:18:25.000000 pandasflow-0.5.7/pandasflow/metrics/roc.py
-drwxrwxrwx   0        0        0        0 2023-06-01 08:35:15.405148 pandasflow-0.5.7/pandasflow/model/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:16:13.000000 pandasflow-0.5.7/pandasflow/model/__init__.py
--rw-rw-rw-   0        0        0      622 2023-05-15 12:17:31.000000 pandasflow-0.5.7/pandasflow/reset_mi.py
-drwxrwxrwx   0        0        0        0 2023-06-01 08:35:15.406149 pandasflow-0.5.7/pandasflow/services/
--rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.5.7/pandasflow/services/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 08:35:15.407146 pandasflow-0.5.7/pandasflow/split/
--rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.5.7/pandasflow/split/__init__.py
--rw-rw-rw-   0        0        0     2835 2023-05-15 10:13:46.000000 pandasflow-0.5.7/pandasflow/split/train_test.py
--rw-rw-rw-   0        0        0     3944 2023-05-15 10:24:18.000000 pandasflow-0.5.7/pandasflow/split/train_valid_test.py
-drwxrwxrwx   0        0        0        0 2023-06-01 08:35:15.399484 pandasflow-0.5.7/pandasflow.egg-info/
--rw-rw-rw-   0        0        0      869 2023-06-01 08:35:15.000000 pandasflow-0.5.7/pandasflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      958 2023-06-01 08:35:15.000000 pandasflow-0.5.7/pandasflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 08:35:15.000000 pandasflow-0.5.7/pandasflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-01 08:35:15.000000 pandasflow-0.5.7/pandasflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-01 08:35:15.000000 pandasflow-0.5.7/pandasflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 08:35:15.414077 pandasflow-0.5.7/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-04-26 15:06:07.000000 pandasflow-0.5.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 08:35:15.413473 pandasflow-0.5.7/test/
--rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.5.7/test/__init__.py
--rw-rw-rw-   0        0        0      760 2023-05-02 12:24:07.000000 pandasflow-0.5.7/test/best_f1_test.py
--rw-rw-rw-   0        0        0      740 2023-05-02 12:00:40.000000 pandasflow-0.5.7/test/conf_mat_test.py
--rw-rw-rw-   0        0        0      620 2023-05-15 11:59:08.000000 pandasflow-0.5.7/test/lloss_up_test.py
--rw-rw-rw-   0        0        0      139 2023-04-26 14:30:22.000000 pandasflow-0.5.7/test/mean_error_test.py
--rw-rw-rw-   0        0        0     1296 2023-05-07 08:19:28.000000 pandasflow-0.5.7/test/precision_recall_test.py
--rw-rw-rw-   0        0        0     1249 2023-05-07 08:18:25.000000 pandasflow-0.5.7/test/roc_test.py
--rw-rw-rw-   0        0        0      498 2023-05-15 10:14:07.000000 pandasflow-0.5.7/test/split_tt_test.py
--rw-rw-rw-   0        0        0      782 2023-05-15 10:24:03.000000 pandasflow-0.5.7/test/split_tvt_test.py
+drwxrwxrwx   0        0        0        0 2023-06-06 08:50:08.995943 pandasflow-0.6.0/
+-rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.6.0/LICENCE
+-rw-rw-rw-   0        0        0      869 2023-06-06 08:50:08.995943 pandasflow-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2023-05-15 11:35:26.000000 pandasflow-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 08:50:08.975996 pandasflow-0.6.0/pandasflow/
+-rw-rw-rw-   0        0        0      391 2023-06-06 08:45:10.000000 pandasflow-0.6.0/pandasflow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 08:50:08.979986 pandasflow-0.6.0/pandasflow/dev/
+-rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.6.0/pandasflow/dev/__init__.py
+-rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.6.0/pandasflow/dev/err_mean_diff.py
+-rw-rw-rw-   0        0        0      387 2023-05-30 09:54:40.000000 pandasflow-0.6.0/pandasflow/get_import.py
+-rw-rw-rw-   0        0        0      480 2023-05-15 09:05:23.000000 pandasflow-0.6.0/pandasflow/get_psql.py
+-rw-rw-rw-   0        0        0      208 2023-05-15 09:29:01.000000 pandasflow-0.6.0/pandasflow/get_sqlt.py
+drwxrwxrwx   0        0        0        0 2023-06-06 08:50:08.985970 pandasflow-0.6.0/pandasflow/metrics/
+-rw-rw-rw-   0        0        0      340 2023-06-06 08:47:33.000000 pandasflow-0.6.0/pandasflow/metrics/__init__.py
+-rw-rw-rw-   0        0        0      801 2023-06-06 08:45:10.000000 pandasflow-0.6.0/pandasflow/metrics/best_thr_f1.py
+-rw-rw-rw-   0        0        0     1132 2023-05-02 12:00:22.000000 pandasflow-0.6.0/pandasflow/metrics/conf_mat.py
+-rw-rw-rw-   0        0        0     2173 2023-05-15 11:57:58.000000 pandasflow-0.6.0/pandasflow/metrics/lloss_up.py
+-rw-rw-rw-   0        0        0      400 2023-04-26 15:19:05.000000 pandasflow-0.6.0/pandasflow/metrics/mean_error.py
+-rw-rw-rw-   0        0        0      721 2023-05-07 08:19:28.000000 pandasflow-0.6.0/pandasflow/metrics/precision_recall.py
+-rw-rw-rw-   0        0        0      658 2023-06-06 08:47:33.000000 pandasflow-0.6.0/pandasflow/metrics/roc_auc.py
+drwxrwxrwx   0        0        0        0 2023-06-06 08:50:08.985970 pandasflow-0.6.0/pandasflow/model/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:16:13.000000 pandasflow-0.6.0/pandasflow/model/__init__.py
+-rw-rw-rw-   0        0        0      622 2023-05-15 12:17:31.000000 pandasflow-0.6.0/pandasflow/reset_mi.py
+drwxrwxrwx   0        0        0        0 2023-06-06 08:50:08.986967 pandasflow-0.6.0/pandasflow/services/
+-rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.6.0/pandasflow/services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 08:50:08.988962 pandasflow-0.6.0/pandasflow/split/
+-rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.6.0/pandasflow/split/__init__.py
+-rw-rw-rw-   0        0        0     2835 2023-05-15 10:13:46.000000 pandasflow-0.6.0/pandasflow/split/train_test.py
+-rw-rw-rw-   0        0        0     3944 2023-05-15 10:24:18.000000 pandasflow-0.6.0/pandasflow/split/train_valid_test.py
+drwxrwxrwx   0        0        0        0 2023-06-06 08:50:08.978989 pandasflow-0.6.0/pandasflow.egg-info/
+-rw-rw-rw-   0        0        0      869 2023-06-06 08:50:08.000000 pandasflow-0.6.0/pandasflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      974 2023-06-06 08:50:08.000000 pandasflow-0.6.0/pandasflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 08:50:08.000000 pandasflow-0.6.0/pandasflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-06 08:50:08.000000 pandasflow-0.6.0/pandasflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-06 08:50:08.000000 pandasflow-0.6.0/pandasflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 08:50:08.995943 pandasflow-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      738 2023-04-26 15:06:07.000000 pandasflow-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 08:50:08.994946 pandasflow-0.6.0/test/
+-rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.6.0/test/__init__.py
+-rw-rw-rw-   0        0        0      764 2023-06-06 08:45:10.000000 pandasflow-0.6.0/test/best_thr_f1_test.py
+-rw-rw-rw-   0        0        0      740 2023-05-02 12:00:40.000000 pandasflow-0.6.0/test/conf_mat_test.py
+-rw-rw-rw-   0        0        0      620 2023-05-15 11:59:08.000000 pandasflow-0.6.0/test/lloss_up_test.py
+-rw-rw-rw-   0        0        0      139 2023-04-26 14:30:22.000000 pandasflow-0.6.0/test/mean_error_test.py
+-rw-rw-rw-   0        0        0     1296 2023-05-07 08:19:28.000000 pandasflow-0.6.0/test/precision_recall_test.py
+-rw-rw-rw-   0        0        0     1261 2023-06-06 08:49:02.000000 pandasflow-0.6.0/test/roc_auc_test.py
+-rw-rw-rw-   0        0        0      498 2023-05-15 10:14:07.000000 pandasflow-0.6.0/test/split_tt_test.py
+-rw-rw-rw-   0        0        0      782 2023-05-15 10:24:03.000000 pandasflow-0.6.0/test/split_tvt_test.py
```

### Comparing `pandasflow-0.5.7/LICENCE` & `pandasflow-0.6.0/LICENCE`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.7/PKG-INFO` & `pandasflow-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.5.7
+Version: 0.6.0
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.5.7/pandasflow/dev/err_mean_diff.py` & `pandasflow-0.6.0/pandasflow/dev/err_mean_diff.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.7/pandasflow/metrics/best_f1.py` & `pandasflow-0.6.0/pandasflow/metrics/best_thr_f1.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import pandas as pd
 from sklearn.metrics import f1_score
 from tqdm.notebook import tqdm
 
 
-def best_f1(y_true:pd.Series, score:pd.Series, out:int=1, tqdm_:bool=True):
+def best_thr_f1(y_true:pd.Series, score:pd.Series, out:int=1, tqdm_:bool=True):
 	thrs = list(score.unique())
 	thrs = [max(min(thrs) - 0.000001, 0.000001)] + thrs
 	
 	df = pd.concat([y_true, score], axis=1)
 	
 	result = []
```

### Comparing `pandasflow-0.5.7/pandasflow/metrics/conf_mat.py` & `pandasflow-0.6.0/pandasflow/metrics/conf_mat.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.7/pandasflow/metrics/lloss_up.py` & `pandasflow-0.6.0/pandasflow/metrics/lloss_up.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.7/pandasflow/metrics/precision_recall.py` & `pandasflow-0.6.0/pandasflow/metrics/precision_recall.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.7/pandasflow/metrics/roc.py` & `pandasflow-0.6.0/pandasflow/metrics/roc_auc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pandasflow as pdf
 import pandas as pd
 from sklearn.metrics import roc_curve, roc_auc_score
 from matplotlib import pyplot
 
 
-def roc(target, score, plot=False, marker='', round_=2):
+def roc_auc(target, score, plot=False, marker='', round_=2):
 	if type(score) == pd.Series:
 		score_ = []
 		score_.append(score)
 	else:
 		score_ = score
 	
 	for sc in score_:
```

### Comparing `pandasflow-0.5.7/pandasflow/reset_mi.py` & `pandasflow-0.6.0/pandasflow/reset_mi.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.7/pandasflow/split/train_test.py` & `pandasflow-0.6.0/pandasflow/split/train_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.7/pandasflow/split/train_valid_test.py` & `pandasflow-0.6.0/pandasflow/split/train_valid_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.7/pandasflow.egg-info/PKG-INFO` & `pandasflow-0.6.0/pandasflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.5.7
+Version: 0.6.0
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.5.7/pandasflow.egg-info/SOURCES.txt` & `pandasflow-0.6.0/pandasflow.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 pandasflow.egg-info/SOURCES.txt
 pandasflow.egg-info/dependency_links.txt
 pandasflow.egg-info/requires.txt
 pandasflow.egg-info/top_level.txt
 pandasflow/dev/__init__.py
 pandasflow/dev/err_mean_diff.py
 pandasflow/metrics/__init__.py
-pandasflow/metrics/best_f1.py
+pandasflow/metrics/best_thr_f1.py
 pandasflow/metrics/conf_mat.py
 pandasflow/metrics/lloss_up.py
 pandasflow/metrics/mean_error.py
 pandasflow/metrics/precision_recall.py
-pandasflow/metrics/roc.py
+pandasflow/metrics/roc_auc.py
 pandasflow/model/__init__.py
 pandasflow/services/__init__.py
 pandasflow/split/__init__.py
 pandasflow/split/train_test.py
 pandasflow/split/train_valid_test.py
 test/__init__.py
-test/best_f1_test.py
+test/best_thr_f1_test.py
 test/conf_mat_test.py
 test/lloss_up_test.py
 test/mean_error_test.py
 test/precision_recall_test.py
-test/roc_test.py
+test/roc_auc_test.py
 test/split_tt_test.py
 test/split_tvt_test.py
```

### Comparing `pandasflow-0.5.7/setup.py` & `pandasflow-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.7/test/best_f1_test.py` & `pandasflow-0.6.0/test/best_thr_f1_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,9 +11,9 @@
 model = model.rename({'Exited': 'score_prod_age'}, axis=1)
 train = train.merge(model, how='left', on=['NumOfProducts', 'age_group'])
 test['age_group'] = pd.cut(test['Age'], [0, 31, 35, 40, 45, float('inf')])
 test = test.merge(model, how='left', on=['NumOfProducts', 'age_group'])
 test['y_pred'] = (test['score_prod_age'] > 0.5) * 1
 
 
-pdf.metrics.best_f1(test['Exited'], test['score_prod_age'], tqdm_=False)
+pdf.metrics.best_thr_f1(test['Exited'], test['score_prod_age'], tqdm_=False)
```

### Comparing `pandasflow-0.5.7/test/conf_mat_test.py` & `pandasflow-0.6.0/test/conf_mat_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.7/test/lloss_up_test.py` & `pandasflow-0.6.0/test/lloss_up_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.7/test/precision_recall_test.py` & `pandasflow-0.6.0/test/precision_recall_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.7/test/roc_test.py` & `pandasflow-0.6.0/test/roc_auc_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,12 +19,12 @@
 t['y_score3'] = np.concatenate([np.random.uniform(0, 0.2, size=850), #TN
                                 np.random.uniform(0.8, 1, size=140), #FP
                                 np.random.uniform(0, 0.2, size=2),   #FN
                                 np.random.uniform(0.8, 1, size=8)])  #TP
 
 
 
-pdf.metrics.roc(t['y_true'], score=t['y_score1'], plot=True)
+# pdf.metrics.roc_auc(t['y_true'], score=t['y_score1'], plot=True)
 
-# pdf.metrics.roc(t['y_true'], score=[t['y_score1'], t['y_score2']])
+# pdf.metrics.roc_auc(t['y_true'], score=[t['y_score1'], t['y_score2']])
 
-# pdf.metrics.roc(t['y_true'], score=[t['y_score1'], t['y_score2'], t['y_score3']], plot=True)
+pdf.metrics.roc_auc(t['y_true'], score=[t['y_score1'], t['y_score2'], t['y_score3']], plot=True)
```

### Comparing `pandasflow-0.5.7/test/split_tvt_test.py` & `pandasflow-0.6.0/test/split_tvt_test.py`

 * *Files identical despite different names*

