# Comparing `tmp/scdef-0.0.8.tar.gz` & `tmp/scdef-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scdef-0.0.8.tar", max compression
+gzip compressed data, was "scdef-0.0.9.tar", max compression
```

## Comparing `scdef-0.0.8.tar` & `scdef-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      961 2023-06-05 12:00:48.737739 scdef-0.0.8/README.md
--rw-r--r--   0        0        0      660 2023-06-05 19:07:21.964725 scdef-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      141 2023-06-05 01:25:33.034355 scdef-0.0.8/scdef/__init__.py
--rw-r--r--   0        0        0    13737 2023-06-05 01:13:30.448424 scdef-0.0.8/scdef/bscdef.py
--rw-r--r--   0        0        0    10025 2023-06-05 01:13:30.354772 scdef-0.0.8/scdef/iscdef.py
--rw-r--r--   0        0        0     3113 2023-06-04 23:18:51.711931 scdef-0.0.8/scdef/main.py
--rw-r--r--   0        0        0     7584 2023-06-04 23:23:31.968859 scdef-0.0.8/scdef/models/integrated.py
--rw-r--r--   0        0        0     7548 2023-06-04 23:23:29.433437 scdef-0.0.8/scdef/models/joint.py
--rw-r--r--   0        0        0        0 2023-06-05 01:42:20.961736 scdef-0.0.8/scdef/models/single.py
--rw-r--r--   0        0        0    20159 2023-06-04 23:23:30.962929 scdef-0.0.8/scdef/models/spatial.py
--rw-r--r--   0        0        0    50586 2023-06-05 17:05:58.304170 scdef-0.0.8/scdef/scdef.py
--rw-r--r--   0        0        0     3328 2023-06-04 23:18:52.167043 scdef-0.0.8/scdef/util.py
--rw-r--r--   0        0        0     2072 1970-01-01 00:00:00.000000 scdef-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      961 2023-06-05 12:00:48.737739 scdef-0.0.9/README.md
+-rw-r--r--   0        0        0      660 2023-06-06 05:53:29.743713 scdef-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      141 2023-06-05 01:25:33.034355 scdef-0.0.9/scdef/__init__.py
+-rw-r--r--   0        0        0    13737 2023-06-05 01:13:30.448424 scdef-0.0.9/scdef/bscdef.py
+-rw-r--r--   0        0        0    10025 2023-06-05 01:13:30.354772 scdef-0.0.9/scdef/iscdef.py
+-rw-r--r--   0        0        0     3113 2023-06-04 23:18:51.711931 scdef-0.0.9/scdef/main.py
+-rw-r--r--   0        0        0     7584 2023-06-04 23:23:31.968859 scdef-0.0.9/scdef/models/integrated.py
+-rw-r--r--   0        0        0     7548 2023-06-04 23:23:29.433437 scdef-0.0.9/scdef/models/joint.py
+-rw-r--r--   0        0        0        0 2023-06-05 01:42:20.961736 scdef-0.0.9/scdef/models/single.py
+-rw-r--r--   0        0        0    20159 2023-06-04 23:23:30.962929 scdef-0.0.9/scdef/models/spatial.py
+-rw-r--r--   0        0        0    50571 2023-06-06 05:52:37.682855 scdef-0.0.9/scdef/scdef.py
+-rw-r--r--   0        0        0     3328 2023-06-04 23:18:52.167043 scdef-0.0.9/scdef/util.py
+-rw-r--r--   0        0        0     2072 1970-01-01 00:00:00.000000 scdef-0.0.9/PKG-INFO
```

### Comparing `scdef-0.0.8/README.md` & `scdef-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `scdef-0.0.8/pyproject.toml` & `scdef-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scdef"
-version = "0.0.8"
+version = "0.0.9"
 description = "Extract hierarchical signatures of cell state from single-cell data."
 license = "MIT"
 authors = ["pedrofale <pedro.miguel.ferreira.pf@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/cbg-ethz/scdef"
 
 [tool.poetry.dependencies]
```

### Comparing `scdef-0.0.8/scdef/bscdef.py` & `scdef-0.0.9/scdef/bscdef.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.8/scdef/iscdef.py` & `scdef-0.0.9/scdef/iscdef.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.8/scdef/main.py` & `scdef-0.0.9/scdef/main.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.8/scdef/models/integrated.py` & `scdef-0.0.9/scdef/models/integrated.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.8/scdef/models/joint.py` & `scdef-0.0.9/scdef/models/joint.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.8/scdef/models/spatial.py` & `scdef-0.0.9/scdef/models/spatial.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.8/scdef/scdef.py` & `scdef-0.0.9/scdef/scdef.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
         self.adata = adata.copy()
         self.adata.raw = self.adata
         X = self.adata.raw.X
         if layer is not None:
             X = self.adata.layers[layer]
 
         if isinstance(X, scipy.sparse.csr_matrix):
-            self.X = np.array(self.adata.raw.X.toarray())
+            self.X = np.array(X.toarray())
         else:
             self.X = np.array(X)
 
         self.batch_indices_onehot = np.ones((self.adata.shape[0], 1))
         self.batch_lib_sizes = np.sum(self.X, axis=1)
         self.batch_lib_ratio = (
             np.ones((self.X.shape[0], 1))
```

### Comparing `scdef-0.0.8/scdef/util.py` & `scdef-0.0.9/scdef/util.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.8/PKG-INFO` & `scdef-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scdef
-Version: 0.0.8
+Version: 0.0.9
 Summary: Extract hierarchical signatures of cell state from single-cell data.
 Home-page: https://github.com/cbg-ethz/scdef
 License: MIT
 Author: pedrofale
 Author-email: pedro.miguel.ferreira.pf@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

