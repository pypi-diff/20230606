# Comparing `tmp/datasieve-0.1.0.tar.gz` & `tmp/datasieve-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasieve-0.1.0.tar", max compression
+gzip compressed data, was "datasieve-0.1.1.tar", max compression
```

## Comparing `datasieve-0.1.0.tar` & `datasieve-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1059 2023-05-29 21:37:04.979482 datasieve-0.1.0/LICENSE
--rw-r--r--   0        0        0    11157 2023-05-29 21:37:04.979482 datasieve-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-29 21:37:04.979482 datasieve-0.1.0/datasieve/__init__.py
--rw-r--r--   0        0        0     7210 2023-05-29 21:37:04.979482 datasieve-0.1.0/datasieve/pipeline.py
--rw-r--r--   0        0        0      575 2023-05-29 21:37:04.979482 datasieve-0.1.0/datasieve/transforms/__init__.py
--rw-r--r--   0        0        0     5739 2023-05-29 21:37:04.979482 datasieve-0.1.0/datasieve/transforms/dbscan.py
--rw-r--r--   0        0        0     3137 2023-05-29 21:37:04.979482 datasieve-0.1.0/datasieve/transforms/dissimilarity_index.py
--rw-r--r--   0        0        0     1197 2023-05-29 21:37:04.979482 datasieve-0.1.0/datasieve/transforms/minmax_scaler.py
--rw-r--r--   0        0        0     1606 2023-05-29 21:37:04.979482 datasieve-0.1.0/datasieve/transforms/pca.py
--rw-r--r--   0        0        0     1725 2023-05-29 21:37:04.979482 datasieve-0.1.0/datasieve/transforms/svm_outlier_extractor.py
--rw-r--r--   0        0        0     1453 2023-05-29 21:37:04.979482 datasieve-0.1.0/datasieve/transforms/variance_threshold.py
--rw-r--r--   0        0        0     3058 2023-05-29 21:37:04.979482 datasieve-0.1.0/datasieve/utils.py
--rw-r--r--   0        0        0      544 2023-05-29 21:37:04.979482 datasieve-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    11783 1970-01-01 00:00:00.000000 datasieve-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-06-06 19:08:39.717257 datasieve-0.1.1/LICENSE
+-rw-r--r--   0        0        0    11439 2023-06-06 19:08:39.717257 datasieve-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-06 19:08:39.717257 datasieve-0.1.1/datasieve/__init__.py
+-rw-r--r--   0        0        0     7803 2023-06-06 19:08:39.717257 datasieve-0.1.1/datasieve/pipeline.py
+-rw-r--r--   0        0        0      563 2023-06-06 19:08:39.717257 datasieve-0.1.1/datasieve/transforms/__init__.py
+-rw-r--r--   0        0        0      706 2023-06-06 19:08:39.717257 datasieve-0.1.1/datasieve/transforms/base_transform.py
+-rw-r--r--   0        0        0     5896 2023-06-06 19:08:39.717257 datasieve-0.1.1/datasieve/transforms/dbscan.py
+-rw-r--r--   0        0        0     3214 2023-06-06 19:08:39.717257 datasieve-0.1.1/datasieve/transforms/dissimilarity_index.py
+-rw-r--r--   0        0        0     1693 2023-06-06 19:08:39.717257 datasieve-0.1.1/datasieve/transforms/pca.py
+-rw-r--r--   0        0        0     1553 2023-06-06 19:08:39.717257 datasieve-0.1.1/datasieve/transforms/sklearn_wrapper.py
+-rw-r--r--   0        0        0     1803 2023-06-06 19:08:39.717257 datasieve-0.1.1/datasieve/transforms/svm_outlier_extractor.py
+-rw-r--r--   0        0        0     1550 2023-06-06 19:08:39.717257 datasieve-0.1.1/datasieve/transforms/variance_threshold.py
+-rw-r--r--   0        0        0     3058 2023-06-06 19:08:39.717257 datasieve-0.1.1/datasieve/utils.py
+-rw-r--r--   0        0        0      544 2023-06-06 19:08:39.717257 datasieve-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    12065 1970-01-01 00:00:00.000000 datasieve-0.1.1/PKG-INFO
```

### Comparing `datasieve-0.1.0/LICENSE` & `datasieve-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.0/README.md` & `datasieve-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,88 +2,43 @@
 
 DataSieve is very similar to the SKlearn Pipeline in that it:
 
 - fits an arbitrary series of transformations to an array X
 - transforms subsequent arrays of the same dimension according to the fit from the original X
 - inverse transforms arrays by inverting the series of transformations
 
-This means that it follows the SKLearn API very closely, and in fact most of the methods inherit directly from SKLearn methods.
+This means that it follows the SKLearn API very closely, and in fact users can use SKLearn transforms directly without making any modifications.
 
 The main **difference** is that DataSieve allows for the manipulation of the y and sample_weight arrays in addition to the X array. This is useful if you find yourself wishing to use the SKLearn pipeline for:
 
 - removing outliers across your X, y, and sample_weights arrays according to simple or complex criteria
 - remove feature columns based on arbitrary criteria (e.g. low variance features)
 - change feature column names at certain transformations (e.g. PCA)
 - needing outlier classification without removal (see `oulier_check`)
 - passing dynamic parameters to individual transforms of the pipeline
 - passing dataframes/arrays without worrying about converting to arrays and maintaining the proper feature columns
 - customizing backend for parallelization (e.g. Dask, Ray, loky, etc.)
 
 These improved flexibilities allow for more customized/creative transformations. For example, the included `DataSieveDBSCAN` has automated parameter fitting and outlier removal based on clustering. 
 
-An example would be someone who wants to use `SGDOneClassSVM` to detect and remove outliers from their data set before training:
-
-```python
-class SVMOutlierExtractor(SGDOneClassSVM):
-    """
-    A subclass of the SKLearn SGDOneClassSVM that adds a transform() method
-    for removing detected outliers from X (as well as the associated y and
-    sample_weight if they are also furnished.
-    """
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-
-    def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        self.fit(X, y, sample_weight=sample_weight)
-        return self.transform(X, y, sample_weight=sample_weight)
-
-    def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        super().fit(X, y=y, sample_weight=sample_weight)
-        return X, y, sample_weight, feature_list
 
-    def transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        y_pred = self.predict(X)
-
-        X, y, sample_weight = remove_outliers(X, y, sample_weight, y_pred)
-
-        num_tossed = len(y_pred) - len(X)
-        if num_tossed > 0:
-            logger.info(
-                f"SVM detected {num_tossed} data points "
-                "as outliers."
-            )
-
-        return X, y, sample_weight, feature_list
-
-    def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        """
-        Unused, pass through X, y, sample_weight, and feature_list
-        """
-        return X, y, sample_weight, feature_list
-```
-
-
-As shown here, the `fit()` method is actually identical to the SKLearn `fit()` method, but the `transform()` removes data points from X, y, and sample_weight for any outliers detected in the `X` array.
-
-
-# Usage
-The user builds the pipeline similarly to SKLearn:
+## Usage
+The user builds the pipeline similarly to SKLearn, and can even use SKLearn transforms directly with the `SKLearnWrapper`:
 
 ```python
     from datasieve.pipeline import Pipeline
     from datasieve.transforms import DataSieveMinMaxScaler, DataSievePCA, DataSieveVarianceThreshold, SVMOutlierExtractor
+    from datasieve.transforms import SKlearnWrapper
 
     feature_pipeline = Pipeline([
         ("detect_constants", DataSieveVarianceThreshold(threshold=0)),
-        ("pre_svm_scaler", DataSieveMinMaxScaler(feature_range=(-1, 1))),
+        ("pre_svm_scaler", SKlearnWrapper(MinMaxScaler(feature_range=(-1, 1)))),
         ("svm", SVMOutlierExtractor()),
-        ("pre_pca_scaler", DataSieveMinMaxScaler(feature_range=(-1, 1))),
-        ("pca", DataSievePCA(n_components=0.95),
-        ("post_pca_scaler", DataSieveMinMaxScaler(feature_range=(-1, 1)))
+        ("pca", DataSievePCA(n_components=0.95)),
+        ("post_pca_scaler", SKlearnWrapper(MinMaxScaler(feature_range=(-1, 1))))
     ])
 
 ```
 
 Once the pipeline is built, it can be fit and transformed similar to a SKLearn pipeline:
 
 ```python
@@ -92,23 +47,74 @@
 
 This pipeline demonstrates the various components of `DataSieve` which are missing from SKLearn's pipeline. A dataframe `X` (if desired, else users can input a simply array without column names) is input with its associated `y` and `sample_weight` arrays/vectors. The `VarianceThreshold` will first detect and remove any features that have zero variance in X, the `SVMOutlierExtractor` will fit `SGDOneClassSVM` to `X` and then remove the detected outliers in `X`, while also propagating those row removals from `y` and `sample_weight`. Finally, the `PCA` will be fit to the remaining `X` array with the features count changing and getting renamed. The returned `X` dataframe will have the correctly named column features/count, and equal row counts across the `X`, `y`, and `sample_weight` arrays.
 
 Next, the `feature_pipeline` can then be used to transform other datasets with the same input feature dimension:
 
 ```python
 X2, _, _ = feature_pipeline.transform(X2)
-
 ```
 
 Finally, similar to SKLearn's pipeline, the `feature_pipeline` can be used to inverse_transform an array `X3` array that has the same dimensions as the returned `X` array from the pipeline:
 
 ```python
 Xinv, _ ,_ = feature_pipeline.inverse_transform(X)
 ```
 
+
+## Creating a custom transform
+
+An example would be someone who wants to use `SGDOneClassSVM` to detect and remove outliers from their data set before training:
+
+```python
+class SVMOutlierExtractor(BaseTransform):
+    """
+    A subclass of the SKLearn SGDOneClassSVM that adds a transform() method
+    for removing detected outliers from X (as well as the associated y and
+    sample_weight if they are also furnished.
+    """
+
+    def __init__(self, **kwargs):
+        self._skl = SGDOneClassSVM(**kwargs)
+
+    def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        self.fit(X, y, sample_weight=sample_weight)
+        return self.transform(X, y, sample_weight, feature_list)
+
+    def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        self._skl.fit(X, y=y, sample_weight=sample_weight)
+        return X, y, sample_weight, feature_list
+
+    def transform(self, X, y=None, sample_weight=None, feature_list=None,
+                  outlier_check=False, **kwargs):
+        y_pred = self._skl.predict(X)
+        y_pred = np.where(y_pred == -1, 0, y_pred)
+        if not outlier_check:
+            X, y, sample_weight = remove_outliers(X, y, sample_weight, y_pred)
+            num_tossed = len(y_pred) - len(X)
+            if num_tossed > 0:
+                logger.info(
+                    f"SVM detected {num_tossed} data points "
+                    "as outliers."
+                )
+        else:
+            y += y_pred
+            y -= 1
+
+        return X, y, sample_weight, feature_list
+
+    def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        """
+        Unused
+        """
+        return X, y, sample_weight, feature_list
+```
+
+
+As shown here, the `fit()` method is actually identical to the SKLearn `fit()` method, but the `transform()` removes data points from X, y, and sample_weight for any outliers detected in the `X` array.
+
 ## Data removal
 
 The command `feature_pipeline.fit_transform(X, y, sample_weight)` fits each pipeline step to `X`, and transforms `X` according to each step's `transform()` method. In some cases, this will not affect `y` or `sample_weight`. For example, `FlowdaptMinMaxScaler` simply scales `X` and saves the normalization information.  Meanwhile, in the `SVMOutlierExtractor`, `.fit()` will fit an SVM to `X` and `.transform()` will remove any detected outliers from `X`. Typical `Scikit-Learn` pipelines do not remove those data points from `y` and `sample_weight`. Luckily, the `FlowdaptPipeline` takes care of the "associated removal" of the same outlier data points from `y` and `sample_weight`. 
 
 ## Feature modification
 
 Another feature is demonstrated in the `FlowdaptPCA`, which fits a PCA transform to `X` and then transforms `X` to principal components. This dimensionality reduction means that the features are no longer the same, instead they are now `PC1`, `PC2` ... `PCX`. `FlowdaptPipeline` handles the feature renaming at that step (which is not a feature available in the `Scikit-Learn` pipeline). Similar to `FlowdaptPCA`, the `FlowdaptVarianceThreshold` subclasses the `Scikit-Learn` `VarianceThreshold` which is geared toward removing features that have a low variance. `FlowdaptVarianceThreshold` ensures that the removed features are properly handled when `X` passes through this part of the pipeline.
```

### Comparing `datasieve-0.1.0/datasieve/pipeline.py` & `datasieve-0.1.1/datasieve/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         matches the str used to name the step in the steps list.
         """
         self.steps: List[Tuple] = steps
         self.fitparams: Dict[str, dict] = self._validate_fitparams(fitparams, steps)
         self.pandas_types: bool = False
         self.feature_list: list = []
         self.label_list: list = []
+        self.step_strings: list = []
 
     def _validate_fitparams(self, fitparams: Dict[str, dict], steps: List[Tuple]):
         for _, (name, _) in enumerate(steps):
             if name not in fitparams.keys():
                 fitparams[name] = {}  # add an empty dict
 
         return fitparams
@@ -34,14 +35,27 @@
     def __getitem__(self, name: str):
         for _, (step_name, step) in enumerate(self.steps):
             if step_name == name:
                 return step
 
         logger.warning(f"Could not find step {name} in pipeline, returning None")
         return None
+    
+    def append(self, step: Tuple[str, object], fitparams: dict = {}):
+        """
+        Append a step to the pipeline
+        :param step: tuple of (str, transform())
+        :param fitparams: dictionary of parameters to pass to fit
+        """
+        if step[0] in self.step_strings:
+            raise ValueError(f"Step name {step[0]} already exists in pipeline."
+                             "Ensure each step has a unique name.")
+        self.step_strings.append(step[0])
+        self.steps += [step]
+        self.fitparams[step[0]] = fitparams
 
     def fit_transform(self, X, y=None, sample_weight=None) -> Tuple[npt.ArrayLike,
                                                                     npt.ArrayLike,
                                                                     npt.ArrayLike]:
         """
         Iterate through the pipeline calling fit_transform() on each of the
         transformations
```

### Comparing `datasieve-0.1.0/datasieve/transforms/__init__.py` & `datasieve-0.1.1/datasieve/transforms/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datasieve.transforms.dissimilarity_index import DissimilarityIndex
 from datasieve.transforms.svm_outlier_extractor import SVMOutlierExtractor
 from datasieve.transforms.pca import DataSievePCA
 from datasieve.transforms.dbscan import DataSieveDBSCAN
-from datasieve.transforms.minmax_scaler import DataSieveMinMaxScaler
 from datasieve.transforms.variance_threshold import DataSieveVarianceThreshold
+from datasieve.transforms.sklearn_wrapper import SKLearnWrapper
 
 __all__ = (
     "DissimilarityIndex",
     "SVMOutlierExtractor",
     "DataSievePCA",
     "DataSieveDBSCAN",
-    "DataSieveMinMaxScaler",
     "DataSieveVarianceThreshold",
+    "SKLearnWrapper",
 )
```

### Comparing `datasieve-0.1.0/datasieve/transforms/dbscan.py` & `datasieve-0.1.1/datasieve/transforms/dbscan.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import logging
 import numpy as np
 import numpy.typing as npt
 from joblib import parallel_backend
 from sklearn.cluster import DBSCAN
 from sklearn.neighbors import NearestNeighbors
 from datasieve.utils import remove_outliers
+from datasieve.transforms.base_transform import BaseTransform
 
 logger = logging.getLogger('datasieve.pipeline')
 
 
-class DataSieveDBSCAN(DBSCAN):
+class DataSieveDBSCAN(BaseTransform):
     """
     A subclass of the SKLearn DBSCAN that ensures fit, transform, fit_transform and
     inverse_transform all take the full set of params X, y, sample_weight (even if they
     are unused) to follow the FlowdaptPipeline API.
 
     fit() automatically finds the optimal epsilon and min_samples for a set of train_features
     transform() appends datapoints to the train_features, using the same epsilon and
     min_samples as computed in fit, to then determing if any of the appended data points
     are outliers.
     """
 
     def __init__(self, backend="loky", n_jobs=-1, **kwargs) -> None:
-        super().__init__(**kwargs)
+        self._skl: DBSCAN = DBSCAN(**kwargs)
         self.train_features: npt.ArrayLike = np.array([])
         self.backend = backend
         self.n_jobs = n_jobs
 
     def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         self.fit(X, y, sample_weight)
 
@@ -34,35 +35,35 @@
         # to get the outliers assocciated with the train_features.
         # In contrast, a user in the future wants to use the
         # "fit" dbscan to check for outliers on incoming points
         # which makes use of self.transform(). However, self.transform()
         # appends X to the self.train_features in order to determine
         # outliers, so we avoid that duplication by ensuring that
         # fit_transform simply uses the primary train_features only.
-        inliers = np.where(self.labels_ == -1, 0, 1)
+        inliers = np.where(self._skl.labels_ == -1, 0, 1)
 
         X, y, sample_weight = remove_outliers(X, y, sample_weight, inliers)
 
         logger.info(
             f"DBSCAN tossed {len(inliers) - X.shape[0]}"
-            f" train points from {len(self.labels_)} in fit_transform()"
+            f" train points from {len(self._skl.labels_)} in fit_transform()"
         )
 
         return X, y, sample_weight, feature_list
 
     def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         """
         Given a set of training features, find the best
         epsilond and min_samples
         """
-        self.eps, self.min_samples = self.compute_epsilon_and_minpts(X)
-        logger.info(f"Found eps {self.eps} and min_samples {self.min_samples} in fit")
+        self._skl.eps, self._skl.min_samples = self.compute_epsilon_and_minpts(X)
+        logger.info(f"Found eps {self._skl.eps} and min_samples {self._skl.eps} in fit")
 
         with parallel_backend(self.backend, n_jobs=self.n_jobs):
-            super().fit(X)
+            self._skl.fit(X)
 
         self.train_features = X
 
         return X, y, sample_weight, feature_list
 
     def transform(self, X, y=None, sample_weight=None, feature_list=None,
                   outlier_check=False, **kwargs):
@@ -71,36 +72,37 @@
         train_features and determine if they are inliers.
         """
 
         num_X = X.shape[0]
         fullX = np.concatenate([self.train_features, X], axis=0)
 
         with parallel_backend(self.backend, n_jobs=self.n_jobs):
-            logger.info(f"Using eps {self.eps} and min_samples {self.min_samples} to transform")
-            clustering = super().fit(fullX)
+            logger.info(f"Using eps {self._skl.eps} and min_samples"
+                        f"{self._skl.min_samples} to transform")
+            clustering = self._skl.fit(fullX)
 
         inliers = np.where(clustering.labels_[-num_X:] == -1, 0, 1)
 
         if not outlier_check:
             X, y, sample_weight = remove_outliers(X, y, sample_weight, inliers=inliers)
             logger.info(
                 f"DBSCAN tossed {len(inliers) - X.shape[0]}"
-                f" train points from {len(self.labels_)} in transform()"
+                f" train points from {len(self._skl.labels_)} in transform()"
             )
         else:
             y += inliers
             y -= 1
 
         return X, y, sample_weight, feature_list
 
-    def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        """
-        Unused
-        """
-        return X, y, sample_weight, feature_list
+    # def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+    #     """
+    #     Unused
+    #     """
+    #     return X, y, sample_weight, feature_list
 
     def compute_epsilon_and_minpts(self, X):
         """
         Automatically compute the epsilon and min_samples for
         "fitting" the DBSCAN.
         """
         def normalise_distances(distances):
```

### Comparing `datasieve-0.1.0/datasieve/transforms/dissimilarity_index.py` & `datasieve-0.1.1/datasieve/transforms/dissimilarity_index.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import logging
 from sklearn.metrics.pairwise import pairwise_distances
+from datasieve.transforms.base_transform import BaseTransform
 import numpy as np
 import numpy.typing as npt
 from joblib import parallel_backend
 from datasieve.utils import remove_outliers
 
 logger = logging.getLogger('datasieve.pipeline')
 
 
-class DissimilarityIndex:
+class DissimilarityIndex(BaseTransform):
     """
     Object designed for computing the dissimilarity index for a set of training data and
     prediction points. fit() computes the avg_mean distance for the training data and
     stores the data for future "transforms" transform() uses the `di_threshold` to
     identify and remove outliers
     """
```

### Comparing `datasieve-0.1.0/datasieve/transforms/minmax_scaler.py` & `datasieve-0.1.1/datasieve/transforms/svm_outlier_extractor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,50 @@
-from sklearn.preprocessing import MinMaxScaler
+from sklearn.linear_model import SGDOneClassSVM
+from datasieve.transforms.base_transform import BaseTransform
+from datasieve.utils import remove_outliers
 import logging
+import numpy as np
 
 logger = logging.getLogger('datasieve.pipeline')
 
 
-class DataSieveMinMaxScaler(MinMaxScaler):
+class SVMOutlierExtractor(BaseTransform):
     """
-    A subclass of the SKLearn MinMaxScaler that ensures fit, transform, fit_transform and
-    inverse_transform all take the full set of params X, y, sample_weight (even if they
-    are unused) to follow the FlowdaptPipeline API.
+    A subclass of the SKLearn SGDOneClassSVM that adds a transform() method
+    for removing detected outliers from X (as well as the associated y and
+    sample_weight if they are also furnished.
     """
 
     def __init__(self, **kwargs):
-        super().__init__(**kwargs)
+        self._skl = SGDOneClassSVM(**kwargs)
 
     def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        super().fit(X)
-        X = super().transform(X)
-        return X, y, sample_weight, feature_list
+        self.fit(X, y, sample_weight=sample_weight)
+        return self.transform(X, y, sample_weight, feature_list)
 
     def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        super().fit(X)
+        self._skl.fit(X, y=y, sample_weight=sample_weight)
         return X, y, sample_weight, feature_list
 
-    def transform(self, X, y=None, sample_weight=None,
-                  feature_list=None, outlier_check=False, **kwargs):
-        X = super().transform(X)
+    def transform(self, X, y=None, sample_weight=None, feature_list=None,
+                  outlier_check=False, **kwargs):
+        y_pred = self._skl.predict(X)
+        y_pred = np.where(y_pred == -1, 0, y_pred)
+        if not outlier_check:
+            X, y, sample_weight = remove_outliers(X, y, sample_weight, y_pred)
+            num_tossed = len(y_pred) - len(X)
+            if num_tossed > 0:
+                logger.info(
+                    f"SVM detected {num_tossed} data points "
+                    "as outliers."
+                )
+        else:
+            y += y_pred
+            y -= 1
+
         return X, y, sample_weight, feature_list
 
     def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        return super().inverse_transform(X), y, sample_weight, feature_list
+        """
+        Unused
+        """
+        return X, y, sample_weight, feature_list
```

### Comparing `datasieve-0.1.0/datasieve/transforms/pca.py` & `datasieve-0.1.1/datasieve/transforms/pca.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 from sklearn.decomposition import PCA
+from datasieve.transforms.base_transform import BaseTransform
 import logging
 import numpy as np
 
 logger = logging.getLogger('datasieve.pipeline')
 
 
-class DataSievePCA(PCA):
+class DataSievePCA(BaseTransform):
     """
     A subclass of the SKLearn PCA that ensures fit, transform, fit_transform and
     inverse_transform all take the full set of params X, y, sample_weight (even if they
     are unused) to follow the FlowdaptPipeline API.
     """
 
     def __init__(self, n_components=0.9999, **kwargs):
-        super().__init__(n_components=n_components, **kwargs)
+        self._skl = PCA(n_components=n_components, **kwargs)
 
     def fit_transform(self, X, y=None, sample_weight=None, feature_list=None):
         X, y, sample_weight, feature_list = self.fit(X, y, sample_weight, feature_list)
         return self.transform(X, y, sample_weight, feature_list)
 
     def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         n_components = X.shape[1]
-        super().fit(X)
+        self._skl.fit(X)
 
-        n_keep_components = self.n_components_
+        n_keep_components = self._skl.n_components_
         self.feature_list = [f"PC{i}" for i in range(0, n_keep_components)]
         logger.info(f"reduced feature dimension by {n_components - n_keep_components}")
-        logger.info(f"explained variance {np.sum(self.explained_variance_ratio_)}")
+        logger.info(f"explained variance {np.sum(self._skl.explained_variance_ratio_)}")
         return X, y, sample_weight, self.feature_list
 
     def transform(self, X, y=None, sample_weight=None,
                   outlier_check=False, feature_list=None, **kwargs):
-        X = super().transform(X)
+        X = self._skl.transform(X)
         return X, y, sample_weight, self.feature_list
 
     def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        return super().inverse_transform(X), y, sample_weight, feature_list
+        return self._skl.inverse_transform(X), y, sample_weight, feature_list
```

### Comparing `datasieve-0.1.0/datasieve/transforms/variance_threshold.py` & `datasieve-0.1.1/datasieve/transforms/variance_threshold.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import logging
 import numpy as np
 from sklearn.feature_selection import VarianceThreshold
+from datasieve.transforms.base_transform import BaseTransform
 
 logger = logging.getLogger('datasieve.pipeline')
 
 
-class DataSieveVarianceThreshold(VarianceThreshold):
+class DataSieveVarianceThreshold(BaseTransform):
 
     def __init__(self, **kwargs) -> None:
-        super().__init__(**kwargs)
+        self._skl: VarianceThreshold = VarianceThreshold(**kwargs)
         self.feature_list: list = []
         self.mask = None
 
     def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         self.fit(X, y, sample_weight, feature_list)
         return self.transform(X, y, sample_weight, feature_list)
 
     def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        super().fit(X)
-        self.mask = self.get_support()
+        self._skl.fit(X)
+        self.mask = self._skl.get_support()
         if feature_list is not None:
             self.feature_list = np.array(feature_list)[self.mask]
             logger.info("Variance will remove features "
                         f"{len(feature_list) - len(self.feature_list)} "
                         f"on transform. {np.array(feature_list)[~self.mask]}")
         else:
             self.feature_list = None
```

### Comparing `datasieve-0.1.0/datasieve/utils.py` & `datasieve-0.1.1/datasieve/utils.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.0/pyproject.toml` & `datasieve-0.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "datasieve"
-version = "0.1.0"
+version = "0.1.1"
 description = "This package implements a flexible data pipeline to help organize row removal (e.g. outlier removal) and feature modification (e.g. PCA)"
 authors = ['Robert Caulk']
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 scikit-learn = ">=1.1.3"
 pandas = ">=1.3.3"
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.2.1"
+pytest = "^7.3.1"
 autopep8 = "1.6.0"
 flake8 = "^6.0.0"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `datasieve-0.1.0/PKG-INFO` & `datasieve-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasieve
-Version: 0.1.0
+Version: 0.1.1
 Summary: This package implements a flexible data pipeline to help organize row removal (e.g. outlier removal) and feature modification (e.g. PCA)
 License: MIT
 Author: Robert Caulk
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -18,88 +18,43 @@
 
 DataSieve is very similar to the SKlearn Pipeline in that it:
 
 - fits an arbitrary series of transformations to an array X
 - transforms subsequent arrays of the same dimension according to the fit from the original X
 - inverse transforms arrays by inverting the series of transformations
 
-This means that it follows the SKLearn API very closely, and in fact most of the methods inherit directly from SKLearn methods.
+This means that it follows the SKLearn API very closely, and in fact users can use SKLearn transforms directly without making any modifications.
 
 The main **difference** is that DataSieve allows for the manipulation of the y and sample_weight arrays in addition to the X array. This is useful if you find yourself wishing to use the SKLearn pipeline for:
 
 - removing outliers across your X, y, and sample_weights arrays according to simple or complex criteria
 - remove feature columns based on arbitrary criteria (e.g. low variance features)
 - change feature column names at certain transformations (e.g. PCA)
 - needing outlier classification without removal (see `oulier_check`)
 - passing dynamic parameters to individual transforms of the pipeline
 - passing dataframes/arrays without worrying about converting to arrays and maintaining the proper feature columns
 - customizing backend for parallelization (e.g. Dask, Ray, loky, etc.)
 
 These improved flexibilities allow for more customized/creative transformations. For example, the included `DataSieveDBSCAN` has automated parameter fitting and outlier removal based on clustering. 
 
-An example would be someone who wants to use `SGDOneClassSVM` to detect and remove outliers from their data set before training:
-
-```python
-class SVMOutlierExtractor(SGDOneClassSVM):
-    """
-    A subclass of the SKLearn SGDOneClassSVM that adds a transform() method
-    for removing detected outliers from X (as well as the associated y and
-    sample_weight if they are also furnished.
-    """
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-
-    def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        self.fit(X, y, sample_weight=sample_weight)
-        return self.transform(X, y, sample_weight=sample_weight)
-
-    def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        super().fit(X, y=y, sample_weight=sample_weight)
-        return X, y, sample_weight, feature_list
 
-    def transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        y_pred = self.predict(X)
-
-        X, y, sample_weight = remove_outliers(X, y, sample_weight, y_pred)
-
-        num_tossed = len(y_pred) - len(X)
-        if num_tossed > 0:
-            logger.info(
-                f"SVM detected {num_tossed} data points "
-                "as outliers."
-            )
-
-        return X, y, sample_weight, feature_list
-
-    def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        """
-        Unused, pass through X, y, sample_weight, and feature_list
-        """
-        return X, y, sample_weight, feature_list
-```
-
-
-As shown here, the `fit()` method is actually identical to the SKLearn `fit()` method, but the `transform()` removes data points from X, y, and sample_weight for any outliers detected in the `X` array.
-
-
-# Usage
-The user builds the pipeline similarly to SKLearn:
+## Usage
+The user builds the pipeline similarly to SKLearn, and can even use SKLearn transforms directly with the `SKLearnWrapper`:
 
 ```python
     from datasieve.pipeline import Pipeline
     from datasieve.transforms import DataSieveMinMaxScaler, DataSievePCA, DataSieveVarianceThreshold, SVMOutlierExtractor
+    from datasieve.transforms import SKlearnWrapper
 
     feature_pipeline = Pipeline([
         ("detect_constants", DataSieveVarianceThreshold(threshold=0)),
-        ("pre_svm_scaler", DataSieveMinMaxScaler(feature_range=(-1, 1))),
+        ("pre_svm_scaler", SKlearnWrapper(MinMaxScaler(feature_range=(-1, 1)))),
         ("svm", SVMOutlierExtractor()),
-        ("pre_pca_scaler", DataSieveMinMaxScaler(feature_range=(-1, 1))),
-        ("pca", DataSievePCA(n_components=0.95),
-        ("post_pca_scaler", DataSieveMinMaxScaler(feature_range=(-1, 1)))
+        ("pca", DataSievePCA(n_components=0.95)),
+        ("post_pca_scaler", SKlearnWrapper(MinMaxScaler(feature_range=(-1, 1))))
     ])
 
 ```
 
 Once the pipeline is built, it can be fit and transformed similar to a SKLearn pipeline:
 
 ```python
@@ -108,23 +63,74 @@
 
 This pipeline demonstrates the various components of `DataSieve` which are missing from SKLearn's pipeline. A dataframe `X` (if desired, else users can input a simply array without column names) is input with its associated `y` and `sample_weight` arrays/vectors. The `VarianceThreshold` will first detect and remove any features that have zero variance in X, the `SVMOutlierExtractor` will fit `SGDOneClassSVM` to `X` and then remove the detected outliers in `X`, while also propagating those row removals from `y` and `sample_weight`. Finally, the `PCA` will be fit to the remaining `X` array with the features count changing and getting renamed. The returned `X` dataframe will have the correctly named column features/count, and equal row counts across the `X`, `y`, and `sample_weight` arrays.
 
 Next, the `feature_pipeline` can then be used to transform other datasets with the same input feature dimension:
 
 ```python
 X2, _, _ = feature_pipeline.transform(X2)
-
 ```
 
 Finally, similar to SKLearn's pipeline, the `feature_pipeline` can be used to inverse_transform an array `X3` array that has the same dimensions as the returned `X` array from the pipeline:
 
 ```python
 Xinv, _ ,_ = feature_pipeline.inverse_transform(X)
 ```
 
+
+## Creating a custom transform
+
+An example would be someone who wants to use `SGDOneClassSVM` to detect and remove outliers from their data set before training:
+
+```python
+class SVMOutlierExtractor(BaseTransform):
+    """
+    A subclass of the SKLearn SGDOneClassSVM that adds a transform() method
+    for removing detected outliers from X (as well as the associated y and
+    sample_weight if they are also furnished.
+    """
+
+    def __init__(self, **kwargs):
+        self._skl = SGDOneClassSVM(**kwargs)
+
+    def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        self.fit(X, y, sample_weight=sample_weight)
+        return self.transform(X, y, sample_weight, feature_list)
+
+    def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        self._skl.fit(X, y=y, sample_weight=sample_weight)
+        return X, y, sample_weight, feature_list
+
+    def transform(self, X, y=None, sample_weight=None, feature_list=None,
+                  outlier_check=False, **kwargs):
+        y_pred = self._skl.predict(X)
+        y_pred = np.where(y_pred == -1, 0, y_pred)
+        if not outlier_check:
+            X, y, sample_weight = remove_outliers(X, y, sample_weight, y_pred)
+            num_tossed = len(y_pred) - len(X)
+            if num_tossed > 0:
+                logger.info(
+                    f"SVM detected {num_tossed} data points "
+                    "as outliers."
+                )
+        else:
+            y += y_pred
+            y -= 1
+
+        return X, y, sample_weight, feature_list
+
+    def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        """
+        Unused
+        """
+        return X, y, sample_weight, feature_list
+```
+
+
+As shown here, the `fit()` method is actually identical to the SKLearn `fit()` method, but the `transform()` removes data points from X, y, and sample_weight for any outliers detected in the `X` array.
+
 ## Data removal
 
 The command `feature_pipeline.fit_transform(X, y, sample_weight)` fits each pipeline step to `X`, and transforms `X` according to each step's `transform()` method. In some cases, this will not affect `y` or `sample_weight`. For example, `FlowdaptMinMaxScaler` simply scales `X` and saves the normalization information.  Meanwhile, in the `SVMOutlierExtractor`, `.fit()` will fit an SVM to `X` and `.transform()` will remove any detected outliers from `X`. Typical `Scikit-Learn` pipelines do not remove those data points from `y` and `sample_weight`. Luckily, the `FlowdaptPipeline` takes care of the "associated removal" of the same outlier data points from `y` and `sample_weight`. 
 
 ## Feature modification
 
 Another feature is demonstrated in the `FlowdaptPCA`, which fits a PCA transform to `X` and then transforms `X` to principal components. This dimensionality reduction means that the features are no longer the same, instead they are now `PC1`, `PC2` ... `PCX`. `FlowdaptPipeline` handles the feature renaming at that step (which is not a feature available in the `Scikit-Learn` pipeline). Similar to `FlowdaptPCA`, the `FlowdaptVarianceThreshold` subclasses the `Scikit-Learn` `VarianceThreshold` which is geared toward removing features that have a low variance. `FlowdaptVarianceThreshold` ensures that the removed features are properly handled when `X` passes through this part of the pipeline.
```

