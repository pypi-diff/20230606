# Comparing `tmp/landmarkclassifier-2.0.6.tar.gz` & `tmp/landmarkclassifier-2.0.7.tar.gz`

## Comparing `landmarkclassifier-2.0.6.tar` & `landmarkclassifier-2.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/environment.yml
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     9153 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/LANDMark/LANDMark.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/LANDMark/__init__.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/LANDMark/lm_dtree_clfs.py
--rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/LANDMark/lm_linear_clfs.py
--rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/LANDMark/lm_nnet_clfs.py
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/LANDMark/lm_oracle_clfs.py
--rw-r--r--   0        0        0    24183 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/LANDMark/tree.py
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/LANDMark/utils.py
--rw-r--r--   0        0        0     5627 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/docs/API.md
--rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/notebooks/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/tests/__init__.py
--rw-r--r--   0        0        0     3468 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/tests/test_landmark.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/.gitignore
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/LICENSE
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/README.md
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/pyproject.toml
--rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/PKG-INFO
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/environment.yml
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     9351 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/LANDMark/LANDMark.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/LANDMark/__init__.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/LANDMark/lm_dtree_clfs.py
+-rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/LANDMark/lm_linear_clfs.py
+-rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/LANDMark/lm_nnet_clfs.py
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/LANDMark/lm_oracle_clfs.py
+-rw-r--r--   0        0        0    21548 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/LANDMark/tree.py
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/LANDMark/utils.py
+-rw-r--r--   0        0        0     5627 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/docs/API.md
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/notebooks/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/tests/__init__.py
+-rw-r--r--   0        0        0     3468 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/tests/test_landmark.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/.gitignore
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/LICENSE
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/README.md
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/pyproject.toml
+-rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/PKG-INFO
```

### Comparing `landmarkclassifier-2.0.6/.github/ISSUE_TEMPLATE/bug_report.md` & `landmarkclassifier-2.0.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.6/.github/ISSUE_TEMPLATE/feature_request.md` & `landmarkclassifier-2.0.7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.6/.github/workflows/ci.yml` & `landmarkclassifier-2.0.7/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.6/.github/workflows/python-publish.yml` & `landmarkclassifier-2.0.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.6/LANDMark/LANDMark.py` & `landmarkclassifier-2.0.7/LANDMark/LANDMark.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         use_lm_l1: bool = True,
         use_nnet: bool = True,
         nnet_min_samples: int = 32,
         use_etc: bool = True,
         etc_max_depth: int = 5,
         etc_max_trees: int = 128,
         resampler = None,
+        use_cascade: bool = False,
         n_jobs: int = 4
     ):
         # Tree construction parameters
         self.n_estimators = n_estimators
         self.min_samples_in_leaf = min_samples_in_leaf
         self.max_depth = max_depth
         self.max_features = max_features
@@ -48,14 +49,15 @@
         self.use_lm_l1 = use_lm_l1
         self.use_nnet = use_nnet
         self.nnet_min_samples = nnet_min_samples
         self.use_etc = use_etc
         self.etc_max_depth = etc_max_depth
         self.etc_max_trees = etc_max_trees
         self.resampler = resampler
+        self.use_cascade = use_cascade
 
         self.n_jobs = n_jobs
 
     def fit(self, X: np.ndarray, y: np.ndarray) -> LANDMarkClassifier:
         """
         Parameters
         -----------
@@ -84,15 +86,15 @@
                 use_lm_l2=self.use_lm_l2,
                 use_lm_l1=self.use_lm_l1,
                 use_nnet=self.use_nnet,
                 nnet_min_samples=self.nnet_min_samples,
                 use_etc=self.use_etc,
                 etc_max_depth=self.etc_max_depth,
                 etc_max_trees=self.etc_max_trees,
-                resampler=self.resampler,
+                resampler=self.resampler
             ),
             n_estimators=self.n_estimators,
             class_names=self.classes_,
             n_jobs=self.n_jobs,
         )
 
         self.estimators_.fit(X_checked, y_checked)
@@ -218,14 +220,17 @@
 
         if not isinstance(self.use_nnet, bool):
             raise TypeError("'use_nnet' must be True or False.")
 
         if not isinstance(self.nnet_min_samples, int):
             raise TypeError("'nnet_min_samples' must be an integer.")
 
+        if not isinstance(self.use_cascade, bool):
+            raise TypeError("'use_cascade' must be True or False.")
+
         if isinstance(self.nnet_min_samples, int):
             if self.nnet_min_samples <= 0:
                 raise ValueError("'nnet_min_samples' must be greater than zero.")
 
         if not isinstance(self.use_etc, bool):
             raise TypeError("'use_etc' must be True or False.")
```

### Comparing `landmarkclassifier-2.0.6/LANDMark/lm_dtree_clfs.py` & `landmarkclassifier-2.0.7/LANDMark/lm_dtree_clfs.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,10 +38,17 @@
         self.clf_model = clf_1.fit(X_re, y_re)
 
         return self, self.decision_function(X)
 
     def predict(self, X):
         return self.clf_model.predict(X[:, self.features])
 
-    def decision_function(self, X):
+    def predict_proba(self, X):
+
         return self.clf_model.predict_proba(X[:, self.features])
 
+    def decision_function(self, X):
+        D = self.clf_model.predict_proba(X[:, self.features])
+
+        return np.where(D > 0.5, 1, -1)
+
+
```

### Comparing `landmarkclassifier-2.0.6/LANDMark/lm_linear_clfs.py` & `landmarkclassifier-2.0.7/LANDMark/lm_linear_clfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,8 +113,10 @@
 
     def decision_function(self, X):
         
         if self.y_min > 6:
             return self.clf.decision_function(X[:, self.features])
 
         else:
-            return self.clf.predict_proba(X[:, self.features])
+            D = self.clf.predict_proba(X[:, self.features])
+
+            return np.where(D > 0.5, 1, -1)
```

### Comparing `landmarkclassifier-2.0.6/LANDMark/lm_nnet_clfs.py` & `landmarkclassifier-2.0.7/LANDMark/lm_nnet_clfs.py`

 * *Files 10% similar despite different names*

```diff
@@ -93,14 +93,16 @@
         clf.fit(X_trf, y_trf)
         
         self.params = clf.module.state_dict()
 
         with pyt.inference_mode():
             D = clf.predict_proba(X[:, self.features].astype(np.float32))
 
+            D = np.where(D > 0.5, 1, -1)
+
         return self, D
 
     def predict_proba(self, X):
 
         if pyt.cuda.is_available():
             device = "cuda"
         else:
@@ -119,14 +121,20 @@
         clf.initialize()
 
         with pyt.inference_mode():
             predictions = clf.predict_proba(X[:, self.features].astype(np.float32))
 
         return predictions
 
+    def decision_function(self, X):
+
+        D = self.predict_proba(X)
+
+        return np.where(D > 0.5, 1, -1)
+
     def predict(self, X):
 
         predictions = self.predict_proba(X)
 
         predictions = np.argmax(predictions, axis = 1)
 
         return self.y_transformer.inverse_transform(predictions)
```

### Comparing `landmarkclassifier-2.0.6/LANDMark/lm_oracle_clfs.py` & `landmarkclassifier-2.0.7/LANDMark/lm_oracle_clfs.py`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.6/LANDMark/tree.py` & `landmarkclassifier-2.0.7/LANDMark/tree.py`

 * *Files 19% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         use_nnet,
         nnet_min_samples,
         use_etc,
         etc_max_depth,
         etc_max_trees,
         N,
         current_depth,
-        use_oracle,
+        use_oracle
     ):
         # Get the ID of the node
         self.node_id = id(self)
 
         # Prepare the list of hyperplanes, gains, and model types
         hyperplane_list = []
         gains = []
@@ -250,21 +250,16 @@
                         LMClassifier(model_type="lsvc", n_feat=max_features),
                     ]:
                         model, D = clf.fit(X, y)
 
                         if D.ndim > 1:
                             D = D[:, self.c_choice]
 
-                        if model.y_min > 6:
-                            L = np.where(D > 0, True, False)
-                            R = np.where(D <= 0, True, False)
-
-                        else:
-                            L = np.where(D > 0.5, True, False)
-                            R = np.where(D <= 0.5, True, False)
+                        L = np.where(D > 0, True, False)
+                        R = np.where(D <= 0, True, False)
 
                         X_L_n = X[L].shape[0]
                         X_R_n = X[R].shape[0]
 
                         # Calculate Information Gain
                         if X_L_n > 0 and X_R_n > 0:
                             IG = purity_function(
@@ -282,21 +277,16 @@
                         LMClassifier(model_type="sgd_l1", n_feat=max_features),
                     ]:
                         model, D = clf.fit(X, y)
 
                         if D.ndim > 1:
                             D = D[:, self.c_choice]
 
-                        if model.y_min > 6:
-                            L = np.where(D > 0, True, False)
-                            R = np.where(D <= 0, True, False)
-
-                        else:
-                            L = np.where(D > 0.5, True, False)
-                            R = np.where(D <= 0.5, True, False)
+                        L = np.where(D > 0, True, False)
+                        R = np.where(D <= 0, True, False)
 
                         X_L_n = X[L].shape[0]
                         X_R_n = X[R].shape[0]
 
                         # Calculate Information Gain
                         if X_L_n > 0 and X_R_n > 0:
                             IG = purity_function(
@@ -312,16 +302,16 @@
                     if X.shape[0] >= nnet_min_samples:
                         for clf in [ANNClassifier(n_feat=max_features)]:
                             model, D = clf.fit(X, y)
 
                             if D.ndim > 1:
                                 D = D[:, self.c_choice]
 
-                            L = np.where(D > 0.5, True, False)
-                            R = np.where(D <= 0.5, True, False)
+                            L = np.where(D > 0, True, False)
+                            R = np.where(D <= 0, True, False)
 
                             X_L_n = X[L].shape[0]
                             X_R_n = X[R].shape[0]
 
                             # Calculate Information Gain
                             if X_L_n > 0 and X_R_n > 0:
                                 IG = purity_function(
@@ -342,16 +332,16 @@
                         )
                     ]:
                         model, D = clf.fit(X, y)
 
                         if D.ndim > 1:
                             D = D[:, self.c_choice]
 
-                        L = np.where(D > 0.5, True, False)
-                        R = np.where(D <= 0.5, True, False)
+                        L = np.where(D > 0, True, False)
+                        R = np.where(D <= 0, True, False)
 
                         X_L_n = X[L].shape[0]
                         X_R_n = X[R].shape[0]
 
                         # Calculate Information Gain
                         if X_L_n > 0 and X_R_n > 0:
                             IG = purity_function(
@@ -528,92 +518,52 @@
             ids.extend(self._get_node_ids(node.right))
 
         else:
             ids.append(node.node_id)
 
         return ids
 
-    def _predict(self, X, current_node=None, root=True, sample_index=None):
+    def _predict(self, X, current_node=None, samp_idx=None):
         final_predictions = []
 
-        true_index = None
-        if root:
-            true_index = np.asarray([i for i in range(X.shape[0])])
+        # Get a list of sample IDs if sample_index is not provided and set the node to the root of the tree
+        if isinstance(samp_idx, type(None)):
+            samp_idx = np.asarray([i for i in range(X.shape[0])])
 
-        else:
-            true_index = sample_index
+            current_node = self.LMTree
 
-        node = None
-        if not (current_node):
-            node = self.LMTree
+        if current_node.terminal is False:
 
-        else:
-            node = current_node
+            D = current_node.splitter.decision_function(X)
 
-        if node.terminal is False:
-            if type(node.splitter) == ANNClassifier:
-                D = node.splitter.predict_proba(X)
+            if D.ndim > 1:
+                D = D[:, current_node.c_choice]
 
-                if D.ndim > 1:
-                    D = D[:, node.c_choice]
-
-                L = np.where(D > 0.5, True, False)
-                R = np.where(D <= 0.5, True, False)
-
-            elif type(node.splitter) == ETClassifier:
-                D = node.splitter.decision_function(X)
-
-                if D.ndim > 1:
-                    D = D[:, node.c_choice]
-
-                L = np.where(D > 0.5, True, False)
-                R = np.where(D <= 0.5, True, False)
-
-            elif type(node.splitter) == LMClassifier:
-                D = node.splitter.decision_function(X)
-
-                if D.ndim > 1:
-                    D = D[:, node.c_choice]
-
-                if node.splitter.y_min > 6:
-                    L = np.where(D > 0, True, False)
-                    R = np.where(D <= 0, True, False)
-
-                else:
-                    L = np.where(D > 0.5, True, False)
-                    R = np.where(D <= 0.5, True, False)
-
-            else:
-                D = node.splitter.decision_function(X)
-
-                if D.ndim > 1:
-                    D = D[:, node.c_choice]
-
-                L = np.where(D > 0, True, False)
-                R = np.where(D <= 0, True, False)
+            L = np.where(D > 0, True, False)
+            R = np.where(D <= 0, True, False)
 
             X_L = X[L]
-            left = true_index[L]
+            left = samp_idx[L]
 
             X_R = X[R]
-            right = true_index[R]
+            right = samp_idx[R]
 
             if left.shape[0] > 0:
-                predictions_left = self._predict(X_L, node.left, False, left)
+                predictions_left = self._predict(X_L, current_node.left, left)
                 final_predictions.extend(predictions_left)
 
             if right.shape[0] > 0:
-                predictions_right = self._predict(X_R, node.right, False, right)
+                predictions_right = self._predict(X_R, current_node.right, right)
                 final_predictions.extend(predictions_right)
 
-        elif node.terminal:
-            predictions = node.label(X)
+        elif current_node.terminal:
+            predictions = current_node.label(X)
             predictions = np.asarray(
                 [
-                    (true_index[i], prediction)
+                    (samp_idx[i], prediction)
                     for i, prediction in enumerate(predictions)
                 ]
             )
 
             return predictions
 
         return final_predictions
@@ -633,89 +583,51 @@
         return np.asarray(tree_predictions)[:, 1]
 
     def score(self, X, y):
         score = balanced_accuracy_score(y, self.predict(X))
 
         return score
 
-    def _proximity(self, X, current_node=None, root=True, sample_index=None):
+    def _proximity(self, X, current_node=None, samp_idx=None):
         final_predictions = []
 
-        true_index = None
-        if root:
-            true_index = np.asarray([i for i in range(X.shape[0])])
-
-        else:
-            true_index = sample_index
-
-        node = None
-        if not (current_node):
-            node = self.LMTree
-
-        else:
-            node = current_node
-
-        if node.terminal is False:
-            if type(node.splitter) == ANNClassifier:
-                D = node.splitter.predict_proba(X)
-
-                if D.ndim > 1:
-                    D = D[:, node.c_choice]
-
-                L = np.where(D > 0.5, True, False)
-                R = np.where(D <= 0.5, True, False)
-
-            elif type(node.splitter) == ETClassifier:
-                D = node.splitter.decision_function(X)
+        # Get a list of sample IDs if sample_index is not provided and set the node to the root of the tree
+        if isinstance(samp_idx, type(None)):
+            samp_idx = np.asarray([i for i in range(X.shape[0])])
 
-                if D.ndim > 1:
-                    D = D[:, node.c_choice]
+            current_node = self.LMTree
 
-                L = np.where(D > 0.5, True, False)
-                R = np.where(D <= 0.5, True, False)
+        # Check if the node is a terminal node
+        if current_node.terminal is False:
 
-            elif type(node.splitter) == LMClassifier:
-                D = node.splitter.decision_function(X)
+            # Determine splits
+            D = current_node.splitter.decision_function(X)
 
-                if D.ndim > 1:
-                    D = D[:, node.c_choice]
-
-                if node.splitter.y_min > 6:
-                    L = np.where(D > 0, True, False)
-                    R = np.where(D <= 0, True, False)
-
-                else:
-                    L = np.where(D > 0.5, True, False)
-                    R = np.where(D <= 0.5, True, False)
+            if D.ndim > 1:
+                D = D[:, current_node.c_choice]
 
-            else:
-                D = node.splitter.decision_function(X)
-
-                if D.ndim > 1:
-                    D = D[:, node.c_choice]
-
-                L = np.where(D > 0, True, False)
-                R = np.where(D <= 0, True, False)
+            L = np.where(D > 0, True, False)
+            R = np.where(D <= 0, True, False)
 
             X_L = X[L]
-            left = true_index[L]
+            left = samp_idx[L]
 
             X_R = X[R]
-            right = true_index[R]
+            right = samp_idx[R]
 
             if left.shape[0] > 0:
-                predictions_left = self._proximity(X_L, node.left, False, left)
+                predictions_left = self._proximity(X_L, current_node.left, left)
                 final_predictions.extend(predictions_left)
 
             if right.shape[0] > 0:
-                predictions_right = self._proximity(X_R, node.right, False, right)
+                predictions_right = self._proximity(X_R, current_node.right, right)
                 final_predictions.extend(predictions_right)
 
-        elif node.terminal:
-            return [(entry, node.node_id) for entry in true_index]
+        elif current_node.terminal:
+            return [(entry, current_node.node_id) for entry in samp_idx]
 
         return final_predictions
 
     def proximity(self, X):
         if hasattr(self.resampler, "transform"):
             X_trf = self.resampler.transform(X)
```

### Comparing `landmarkclassifier-2.0.6/LANDMark/utils.py` & `landmarkclassifier-2.0.7/LANDMark/utils.py`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.6/docs/API.md` & `landmarkclassifier-2.0.7/docs/API.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.6/docs/CONTRIBUTING.md` & `landmarkclassifier-2.0.7/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.6/tests/test_landmark.py` & `landmarkclassifier-2.0.7/tests/test_landmark.py`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.6/.gitignore` & `landmarkclassifier-2.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.6/LICENSE` & `landmarkclassifier-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.6/README.md` & `landmarkclassifier-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.6/pyproject.toml` & `landmarkclassifier-2.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "LANDMarkClassifier"
-version = "2.0.6"
+version = "2.0.7"
 authors = [
     {name = "Josip Rudar", email = "rudarj@uoguelph.ca"},
     {name = "Teresita M. Porter"},
     {name = "Michael Wright"},
     {name = "G. Brian Golding"},
     {name = "Mehrdad Hajibabaei", email = "mhajibab@uoguelph.ca"}
 ]
```

### Comparing `landmarkclassifier-2.0.6/PKG-INFO` & `landmarkclassifier-2.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LANDMarkClassifier
-Version: 2.0.6
+Version: 2.0.7
 Summary: LANDMark: An ensemble approach to the supervised selection of biomarkers in high-throughput sequencing data
 Project-URL: Homepage, https://github.com/jrudar/LANDMark
 Project-URL: Repository, https://github.com/jrudar/LANDMark.git
 Project-URL: Bug Tracker, https://github.com/jrudar/LANDMark/issues
 Author: Teresita M. Porter, Michael Wright, G. Brian Golding
 Author-email: Josip Rudar <rudarj@uoguelph.ca>, Mehrdad Hajibabaei <mhajibab@uoguelph.ca>
 License: MIT License
```

