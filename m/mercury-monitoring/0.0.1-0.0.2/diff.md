# Comparing `tmp/mercury-monitoring-0.0.1.tar.gz` & `tmp/mercury-monitoring-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-monitoring-0.0.1.tar", last modified: Tue Apr 11 13:27:14 2023, max compression
+gzip compressed data, was "mercury-monitoring-0.0.2.tar", last modified: Tue Jun  6 08:53:08 2023, max compression
```

## Comparing `mercury-monitoring-0.0.1.tar` & `mercury-monitoring-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:27:14.565290 mercury-monitoring-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 13:27:00.000000 mercury-monitoring-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-11 13:27:14.565290 mercury-monitoring-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-11 13:27:00.000000 mercury-monitoring-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:27:14.561290 mercury-monitoring-0.0.1/mercury/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:27:14.561290 mercury-monitoring-0.0.1/mercury/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-11 13:27:00.000000 mercury-monitoring-0.0.1/mercury/monitoring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:27:14.565290 mercury-monitoring-0.0.1/mercury/monitoring/drift/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 13:27:00.000000 mercury-monitoring-0.0.1/mercury/monitoring/drift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-11 13:27:00.000000 mercury-monitoring-0.0.1/mercury/monitoring/drift/_resampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-11 13:27:00.000000 mercury-monitoring-0.0.1/mercury/monitoring/drift/_vae.py
--rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-04-11 13:27:00.000000 mercury-monitoring-0.0.1/mercury/monitoring/drift/auto_encoder_drift_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-04-11 13:27:00.000000 mercury-monitoring-0.0.1/mercury/monitoring/drift/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-04-11 13:27:00.000000 mercury-monitoring-0.0.1/mercury/monitoring/drift/chi2_drift_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-04-11 13:27:00.000000 mercury-monitoring-0.0.1/mercury/monitoring/drift/density_drift_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-04-11 13:27:00.000000 mercury-monitoring-0.0.1/mercury/monitoring/drift/domain_classifier_drift_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)    12285 2023-04-11 13:27:00.000000 mercury-monitoring-0.0.1/mercury/monitoring/drift/drift_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-04-11 13:27:00.000000 mercury-monitoring-0.0.1/mercury/monitoring/drift/histogram_distance_drift_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-04-11 13:27:00.000000 mercury-monitoring-0.0.1/mercury/monitoring/drift/ks_drift_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-04-11 13:27:00.000000 mercury-monitoring-0.0.1/mercury/monitoring/drift/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:27:14.565290 mercury-monitoring-0.0.1/mercury/monitoring/estimation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 13:27:00.000000 mercury-monitoring-0.0.1/mercury/monitoring/estimation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17440 2023-04-11 13:27:00.000000 mercury-monitoring-0.0.1/mercury/monitoring/estimation/performance_predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:27:14.565290 mercury-monitoring-0.0.1/mercury_monitoring.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-11 13:27:14.000000 mercury-monitoring-0.0.1/mercury_monitoring.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-11 13:27:14.000000 mercury-monitoring-0.0.1/mercury_monitoring.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 13:27:14.000000 mercury-monitoring-0.0.1/mercury_monitoring.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-11 13:27:14.000000 mercury-monitoring-0.0.1/mercury_monitoring.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 13:27:14.000000 mercury-monitoring-0.0.1/mercury_monitoring.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-11 13:27:00.000000 mercury-monitoring-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 13:27:14.565290 mercury-monitoring-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:53:08.955386 mercury-monitoring-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 08:52:59.000000 mercury-monitoring-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-06 08:53:08.955386 mercury-monitoring-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-06 08:52:59.000000 mercury-monitoring-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:53:08.955386 mercury-monitoring-0.0.2/mercury/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:53:08.955386 mercury-monitoring-0.0.2/mercury/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-06 08:52:59.000000 mercury-monitoring-0.0.2/mercury/monitoring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:53:08.955386 mercury-monitoring-0.0.2/mercury/monitoring/drift/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 08:52:59.000000 mercury-monitoring-0.0.2/mercury/monitoring/drift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-06 08:52:59.000000 mercury-monitoring-0.0.2/mercury/monitoring/drift/_resampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-06 08:52:59.000000 mercury-monitoring-0.0.2/mercury/monitoring/drift/_vae.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-06-06 08:52:59.000000 mercury-monitoring-0.0.2/mercury/monitoring/drift/auto_encoder_drift_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-06-06 08:52:59.000000 mercury-monitoring-0.0.2/mercury/monitoring/drift/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-06 08:52:59.000000 mercury-monitoring-0.0.2/mercury/monitoring/drift/chi2_drift_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-06-06 08:52:59.000000 mercury-monitoring-0.0.2/mercury/monitoring/drift/density_drift_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-06-06 08:52:59.000000 mercury-monitoring-0.0.2/mercury/monitoring/drift/domain_classifier_drift_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12285 2023-06-06 08:52:59.000000 mercury-monitoring-0.0.2/mercury/monitoring/drift/drift_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-06-06 08:52:59.000000 mercury-monitoring-0.0.2/mercury/monitoring/drift/histogram_distance_drift_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-06-06 08:52:59.000000 mercury-monitoring-0.0.2/mercury/monitoring/drift/ks_drift_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-06-06 08:52:59.000000 mercury-monitoring-0.0.2/mercury/monitoring/drift/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:53:08.955386 mercury-monitoring-0.0.2/mercury/monitoring/estimation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 08:52:59.000000 mercury-monitoring-0.0.2/mercury/monitoring/estimation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17440 2023-06-06 08:52:59.000000 mercury-monitoring-0.0.2/mercury/monitoring/estimation/performance_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:53:08.955386 mercury-monitoring-0.0.2/mercury_monitoring.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-06 08:53:08.000000 mercury-monitoring-0.0.2/mercury_monitoring.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-06 08:53:08.000000 mercury-monitoring-0.0.2/mercury_monitoring.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 08:53:08.000000 mercury-monitoring-0.0.2/mercury_monitoring.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-06 08:53:08.000000 mercury-monitoring-0.0.2/mercury_monitoring.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 08:53:08.000000 mercury-monitoring-0.0.2/mercury_monitoring.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-06 08:52:59.000000 mercury-monitoring-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 08:53:08.959387 mercury-monitoring-0.0.2/setup.cfg
```

### Comparing `mercury-monitoring-0.0.1/LICENSE` & `mercury-monitoring-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mercury-monitoring-0.0.1/mercury/monitoring/drift/_resampling.py` & `mercury-monitoring-0.0.2/mercury/monitoring/drift/_resampling.py`

 * *Files identical despite different names*

### Comparing `mercury-monitoring-0.0.1/mercury/monitoring/drift/_vae.py` & `mercury-monitoring-0.0.2/mercury/monitoring/drift/_vae.py`

 * *Files identical despite different names*

### Comparing `mercury-monitoring-0.0.1/mercury/monitoring/drift/auto_encoder_drift_detector.py` & `mercury-monitoring-0.0.2/mercury/monitoring/drift/auto_encoder_drift_detector.py`

 * *Files identical despite different names*

### Comparing `mercury-monitoring-0.0.1/mercury/monitoring/drift/base.py` & `mercury-monitoring-0.0.2/mercury/monitoring/drift/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -97,40 +97,72 @@
             if self.features is not None:
                 return self.features.index(name_feature)
             else:
                 raise ValueError("To use the name_feature the feature attribute of the class must be specified first")
 
         return idx_feature
 
-    def plot_distribution_feature(self, idx_feature=None, name_feature=None, ax=None, figsize=(8, 4)):
+    def plot_distribution_feature(
+        self,
+        idx_feature=None,
+        name_feature=None,
+        ax=None,
+        figsize=(8, 4),
+        kde=True,
+        stat='density',
+        common_bins=True,
+        common_norm=False,
+        **kwargs
+    ):
         """
         Plots the distribution of a given feature for the source and the target datasets.
         The feature can be indicated by the index using the `idx_feature` parameter, or by the name using the
         `name_feature` parameter (only possible if attribute `features` was specified.
         Args:
             idx_feature (int):
                 index of the feature
             name_feature (string):
                 name of the feature
             ax (matplotlib.axes._subplots.AxesSubplot):
                 Axes object on which the data will be plotted. If not specified it creates one.
             figsize (tuple):
                 figsize to use if `ax` is not specified.
+            kde (bool):
+                whether to show the smoothed distribution. Default is True
+            stat (str):
+                Aggregate statistic to compute in each bin. By default is 'density'. Valid values can be checked in
+                seaborn documentation
+            common_bins (bool):
+                If True, use the same bins for the target and source dataset. By default is True
+            common_norm (bool):
+                If True and using a normalized statistic, the normalization will apply over the full dataset (src and target).
+                Otherwise, the normalization is applied to each set independently. Default is False.
+            kwargs:
+                Extra key arguments that can be passed to seaborn `histplot`.
         Returns:
             The axes
         """
         self._check_datasets()
         idx_feature = self._get_index_feature(idx_feature, name_feature)
         if ax is None:
             fig, ax = plt.subplots(1, 1, figsize=figsize)
 
-        palette = itertools.cycle(sns.color_palette())
-        axes = sns.histplot(self.X_src[:, idx_feature], kde=True, color=next(palette), ax=ax, label="dataset source")
-        axes = sns.histplot(self.X_target[:, idx_feature], kde=True, color=next(palette), ax=ax, label="dataset target")
-        axes.legend()
+        data_plot = np.concatenate((self.X_src[:, idx_feature], self.X_target[:, idx_feature]))
+        n_samples_src = len(self.X_src[:, idx_feature])
+        n_samples_target = len(self.X_target[:, idx_feature])
+        axes = sns.histplot(
+            x=data_plot,
+            hue=["dataset source"] * n_samples_src + ["dataset target"] * n_samples_target,
+            kde=kde,
+            stat=stat,
+            common_bins=common_bins,
+            common_norm=common_norm,
+            **kwargs
+        )
+
         return axes
 
     def plot_histograms_feature(self, idx_feature=None, name_feature=None, figsize=(8, 4)):
         """
         Plots the histograms of a given feature for the source and the target distributions.
         The feature can be indicated by the index using the `idx_feature` parameter, or by the name using the
         `name_feature` parameter (only possible if attribute `features` was specified.
@@ -152,28 +184,50 @@
 
         axes[0].bar(range(len(self.distr_src[idx_feature])), self.distr_src[idx_feature], width=0.8)
         axes[1].bar(range(len(self.distr_target[idx_feature])), self.distr_target[idx_feature], width=0.8)
         axes[0].set_title("histogram source")
         axes[1].set_title("histogram target")
         return axes
 
-    def plot_distribution_drifted_features(self, figsize=(8, 4)):
+    def plot_distribution_drifted_features(
+        self,
+        figsize=(8, 4),
+        kde=True,
+        stat='density',
+        common_bins=True,
+        common_norm=False,
+        **kwargs
+    ):
         """
         Plots the distributions of the features that are considered to have drift. The method `calculate_drift`
         needs to be called first.
 
         Args:
             figsize (tuple):
                 figsize to use if `ax` is not specified.
+            kde (bool):
+                whether to show the smoothed distribution. Default is True
+            stat (str):
+                Aggregate statistic to compute in each bin. By default is 'density'. Valid values can be checked in
+                seaborn documentation
+            common_bins (bool):
+                If True, use the same bins for the target and source dataset. By default is True
+            common_norm (bool):
+                If True and using a normalized statistic, the normalization will apply over the full dataset (src and target).
+                Otherwise, the normalization is applied to each set independently. Default is False.
+            kwargs:
+                Extra key arguments that can be passed to seaborn `histplot`.
 
         """
 
         drifted_features = self.get_drifted_features(return_as_indices=True)
         for idx in drifted_features:
-            ax = self.plot_distribution_feature(idx_feature=idx, figsize=figsize)
+            ax = self.plot_distribution_feature(
+                idx_feature=idx, figsize=figsize, kde=kde, common_bins=common_bins, common_norm=common_norm, stat=stat, **kwargs
+            )
             if self.features:
                 ax.set_title(self.features[idx])
             else:
                 ax.set_title(idx)
 
     def plot_histograms_drifted_features(self, figsize=(8, 4)):
         """
```

### Comparing `mercury-monitoring-0.0.1/mercury/monitoring/drift/chi2_drift_detector.py` & `mercury-monitoring-0.0.2/mercury/monitoring/drift/chi2_drift_detector.py`

 * *Files identical despite different names*

### Comparing `mercury-monitoring-0.0.1/mercury/monitoring/drift/density_drift_detector.py` & `mercury-monitoring-0.0.2/mercury/monitoring/drift/density_drift_detector.py`

 * *Files identical despite different names*

### Comparing `mercury-monitoring-0.0.1/mercury/monitoring/drift/domain_classifier_drift_detector.py` & `mercury-monitoring-0.0.2/mercury/monitoring/drift/domain_classifier_drift_detector.py`

 * *Files identical despite different names*

### Comparing `mercury-monitoring-0.0.1/mercury/monitoring/drift/drift_simulation.py` & `mercury-monitoring-0.0.2/mercury/monitoring/drift/drift_simulation.py`

 * *Files identical despite different names*

### Comparing `mercury-monitoring-0.0.1/mercury/monitoring/drift/histogram_distance_drift_detector.py` & `mercury-monitoring-0.0.2/mercury/monitoring/drift/histogram_distance_drift_detector.py`

 * *Files identical despite different names*

### Comparing `mercury-monitoring-0.0.1/mercury/monitoring/drift/ks_drift_detector.py` & `mercury-monitoring-0.0.2/mercury/monitoring/drift/ks_drift_detector.py`

 * *Files identical despite different names*

### Comparing `mercury-monitoring-0.0.1/mercury/monitoring/drift/metrics.py` & `mercury-monitoring-0.0.2/mercury/monitoring/drift/metrics.py`

 * *Files identical despite different names*

### Comparing `mercury-monitoring-0.0.1/mercury/monitoring/estimation/performance_predictor.py` & `mercury-monitoring-0.0.2/mercury/monitoring/estimation/performance_predictor.py`

 * *Files identical despite different names*

### Comparing `mercury-monitoring-0.0.1/mercury_monitoring.egg-info/SOURCES.txt` & `mercury-monitoring-0.0.2/mercury_monitoring.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mercury-monitoring-0.0.1/pyproject.toml` & `mercury-monitoring-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mercury-monitoring"
 license = {file = "LICENSE.txt"}
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Mercury Team", email="mercury.group@bbva.com" },
 ]
 description = "Mercury's monitoring is a library to perform monitoring testing on models and/or datasets.."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

