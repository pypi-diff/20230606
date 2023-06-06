# Comparing `tmp/error-parity-0.1.1.tar.gz` & `tmp/error-parity-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "error-parity-0.1.1.tar", last modified: Tue Jun  6 11:07:27 2023, max compression
+gzip compressed data, was "error-parity-0.1.2.tar", last modified: Tue Jun  6 12:00:15 2023, max compression
```

## Comparing `error-parity-0.1.1.tar` & `error-parity-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:07:27.726400 error-parity-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-06 11:07:14.000000 error-parity-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-06 11:07:14.000000 error-parity-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-06 11:07:27.726400 error-parity-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-06 11:07:14.000000 error-parity-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:07:27.722401 error-parity-0.1.1/error_parity/
--rwxr-xr-x   0 runner    (1001) docker     (123)       93 2023-06-06 11:07:14.000000 error-parity-0.1.1/error_parity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-06 11:07:14.000000 error-parity-0.1.1/error_parity/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16548 2023-06-06 11:07:14.000000 error-parity-0.1.1/error_parity/classifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16492 2023-06-06 11:07:14.000000 error-parity-0.1.1/error_parity/cvxpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15143 2023-06-06 11:07:14.000000 error-parity-0.1.1/error_parity/equal_odds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-06-06 11:07:14.000000 error-parity-0.1.1/error_parity/roc_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:07:27.726400 error-parity-0.1.1/error_parity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-06 11:07:27.000000 error-parity-0.1.1/error_parity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-06 11:07:27.000000 error-parity-0.1.1/error_parity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 11:07:27.000000 error-parity-0.1.1/error_parity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-06 11:07:27.000000 error-parity-0.1.1/error_parity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-06 11:07:27.000000 error-parity-0.1.1/error_parity.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:07:27.726400 error-parity-0.1.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-06 11:07:14.000000 error-parity-0.1.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-06 11:07:14.000000 error-parity-0.1.1/requirements/main.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-06 11:07:14.000000 error-parity-0.1.1/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 11:07:27.726400 error-parity-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-06 11:07:14.000000 error-parity-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:07:27.726400 error-parity-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 11:07:14.000000 error-parity-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-06 11:07:14.000000 error-parity-0.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-06 11:07:14.000000 error-parity-0.1.1/tests/test_equal_odds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:00:15.044356 error-parity-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-06 12:00:05.000000 error-parity-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-06 12:00:05.000000 error-parity-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-06 12:00:15.040356 error-parity-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-06 12:00:05.000000 error-parity-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:00:15.040356 error-parity-0.1.2/error_parity/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       93 2023-06-06 12:00:05.000000 error-parity-0.1.2/error_parity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-06 12:00:05.000000 error-parity-0.1.2/error_parity/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16548 2023-06-06 12:00:05.000000 error-parity-0.1.2/error_parity/classifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16486 2023-06-06 12:00:05.000000 error-parity-0.1.2/error_parity/cvxpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15448 2023-06-06 12:00:05.000000 error-parity-0.1.2/error_parity/equal_odds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-06-06 12:00:05.000000 error-parity-0.1.2/error_parity/roc_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:00:15.040356 error-parity-0.1.2/error_parity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-06 12:00:15.000000 error-parity-0.1.2/error_parity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-06 12:00:15.000000 error-parity-0.1.2/error_parity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 12:00:15.000000 error-parity-0.1.2/error_parity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-06 12:00:15.000000 error-parity-0.1.2/error_parity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-06 12:00:15.000000 error-parity-0.1.2/error_parity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:00:15.040356 error-parity-0.1.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-06 12:00:05.000000 error-parity-0.1.2/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-06 12:00:05.000000 error-parity-0.1.2/requirements/main.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-06 12:00:05.000000 error-parity-0.1.2/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 12:00:15.044356 error-parity-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-06 12:00:05.000000 error-parity-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:00:15.040356 error-parity-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:00:05.000000 error-parity-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-06 12:00:05.000000 error-parity-0.1.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-06 12:00:05.000000 error-parity-0.1.2/tests/test_equal_odds.py
```

### Comparing `error-parity-0.1.1/LICENSE` & `error-parity-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `error-parity-0.1.1/PKG-INFO` & `error-parity-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-parity
-Version: 0.1.1
+Version: 0.1.2
 Summary: Achieve error-rate parity between protected groups for any predictor
 Home-page: https://github.com/AndreFCruz/error-parity
 Author: AndreFCruz
 License: MIT
 Keywords: ml,optimization,fairness,error-parity,equal-odds
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `error-parity-0.1.1/README.md` & `error-parity-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `error-parity-0.1.1/error_parity/classifiers.py` & `error-parity-0.1.2/error_parity/classifiers.py`

 * *Files identical despite different names*

### Comparing `error-parity-0.1.1/error_parity/cvxpy_utils.py` & `error-parity-0.1.2/error_parity/cvxpy_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -148,15 +148,15 @@
             cvxpy_point,
         )
         for i in range(len(polygon_vertices))
     ]
 
 
 
-def compute_error_parity_optimum(
+def compute_equal_odds_optimum(
         groupwise_roc_hulls: Dict[int, np.ndarray],
         fairness_tolerance: float,
         group_sizes_label_pos: np.ndarray,
         group_sizes_label_neg: np.ndarray,
         global_prevalence: float,
         false_positive_cost: float = 1.,
         false_negative_cost: float = 1.,
@@ -279,15 +279,15 @@
         groupwise_label_neg_weight=group_sizes_label_neg,
     )
     assert all(np.isclose(global_roc_from_groupwise, global_roc_point))
 
     return groupwise_roc_points, global_roc_point
 
 
-def compute_error_parity_unfair_optimum(
+def compute_equal_odds_unfair_optimum(
         groupwise_roc_hulls: Dict[int, np.ndarray],
         fairness_tolerance: float,
         group_sizes_label_pos: np.ndarray,
         group_sizes_label_neg: np.ndarray,
         global_prevalence: float,
         false_positive_cost: float = 1.,
         false_negative_cost: float = 1.,
@@ -322,15 +322,15 @@
     (groupwise_roc_points, global_roc_point) : tuple[np.ndarray, np.ndarray]
         A pair tuple, (<1>, <2>), containing:
         1: an array with the group-wise ROC points for the solution.
         2: an array with the single global ROC point for the solution.
     """
     raise NotImplementedError("Not currently implemented; the problem is not convex!")
 
-    logging.warning("> compute_error_parity_unfair_optimum :: USE WITH CARE!")
+    logging.warning("> compute_equal_odds_unfair_optimum :: USE WITH CARE!")
     n_groups = len(groupwise_roc_hulls)
     assert n_groups == len(group_sizes_label_neg) == len(group_sizes_label_pos)
 
     # Group-wise ROC points
     groupwise_roc_points_vars = [
         cp.Variable(shape=2, name=f"ROC point for group {i}", nonneg=True)
         for i in range(n_groups)
```

### Comparing `error-parity-0.1.1/error_parity/equal_odds.py` & `error-parity-0.1.2/error_parity/equal_odds.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import logging
 from itertools import product
 from typing import Callable
 
 import numpy as np
 from sklearn.metrics import roc_curve
 
-from .cvxpy_utils import compute_error_parity_optimum
+from .cvxpy_utils import compute_equal_odds_optimum
 from .roc_utils import (
     roc_convex_hull,
     plot_polygon_edges,
     calc_cost_of_point,
 )
 from .classifiers import (
     Classifier,
@@ -119,23 +119,34 @@
             fpr=global_fpr,
             fnr=1 - global_tpr,
             prevalence=self._global_prevalence,
             false_pos_cost=self.false_pos_cost or false_pos_cost,
             false_neg_cost=self.false_neg_cost or false_neg_cost,
         )
     
-    def error_parity_violation(self) -> float:
+    def constraint_violation(self) -> float:
+        """This method should be part of a common interface between different
+        relaxed-constraint classes.
+
+        Returns
+        -------
+        float
+            The fairness constraint violation.
+        """
+        return self.equal_odds_violation()
+
+    def equal_odds_violation(self) -> float:
         """Computes the theoretical violation of the equal odds constraint 
         (i.e., the maximum l-inf distance between the ROC point of any pair
         of groups).
 
         Returns
         -------
         float
-            The fairness constraint violation.
+            The equal-odds constraint violation.
         """
         self._check_fit_status()
 
         n_groups = len(self.groupwise_roc_points)
 
         # Compute l-inf distance between each pair of groups
         linf_constraint_violation = [
@@ -235,15 +246,15 @@
 
             curr_roc_points = np.stack((group_fpr, group_tpr), axis=1)
             curr_roc_points = np.vstack((curr_roc_points, [1, 0]))  # Add point (1, 0) to ROC curve
 
             self._all_roc_hulls[g] = roc_convex_hull(curr_roc_points)
 
         # Find the group-wise optima that fulfill the fairness criteria
-        self._groupwise_roc_points, self._global_roc_point = compute_error_parity_optimum(
+        self._groupwise_roc_points, self._global_roc_point = compute_equal_odds_optimum(
             groupwise_roc_hulls=self._all_roc_hulls,
             fairness_tolerance=self.tolerance,
             group_sizes_label_pos=group_sizes_label_pos,
             group_sizes_label_neg=group_sizes_label_neg,
             global_prevalence=self._global_prevalence,
             false_positive_cost=self.false_pos_cost,
             false_negative_cost=self.false_neg_cost,
```

### Comparing `error-parity-0.1.1/error_parity/roc_utils.py` & `error-parity-0.1.2/error_parity/roc_utils.py`

 * *Files identical despite different names*

### Comparing `error-parity-0.1.1/error_parity.egg-info/PKG-INFO` & `error-parity-0.1.2/error_parity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-parity
-Version: 0.1.1
+Version: 0.1.2
 Summary: Achieve error-rate parity between protected groups for any predictor
 Home-page: https://github.com/AndreFCruz/error-parity
 Author: AndreFCruz
 License: MIT
 Keywords: ml,optimization,fairness,error-parity,equal-odds
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `error-parity-0.1.1/setup.py` & `error-parity-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `error-parity-0.1.1/tests/conftest.py` & `error-parity-0.1.2/tests/conftest.py`

 * *Files identical despite different names*

