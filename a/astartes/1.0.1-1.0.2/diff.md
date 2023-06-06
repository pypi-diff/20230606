# Comparing `tmp/astartes-1.0.1.tar.gz` & `tmp/astartes-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astartes-1.0.1.tar", last modified: Sun Jun  4 23:52:07 2023, max compression
+gzip compressed data, was "astartes-1.0.2.tar", last modified: Tue Jun  6 01:01:23 2023, max compression
```

## Comparing `astartes-1.0.1.tar` & `astartes-1.0.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:52:07.686536 astartes-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-04 23:51:56.000000 astartes-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-06-04 23:52:07.686536 astartes-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17390 2023-06-04 23:51:56.000000 astartes-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:52:07.682536 astartes-1.0.1/astartes/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17874 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/molecules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:52:07.682536 astartes-1.0.1/astartes/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/samplers/abstract_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:52:07.682536 astartes-1.0.1/astartes/samplers/extrapolation/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/samplers/extrapolation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/samplers/extrapolation/dbscan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/samplers/extrapolation/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/samplers/extrapolation/optisim.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/samplers/extrapolation/scaffold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/samplers/extrapolation/sphere_exclusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/samplers/extrapolation/time_based.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:52:07.686536 astartes-1.0.1/astartes/samplers/interpolation/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/samplers/interpolation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/samplers/interpolation/kennardstone.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/samplers/interpolation/mtsd.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/samplers/interpolation/random_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/samplers/interpolation/spxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:52:07.686536 astartes-1.0.1/astartes/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/utils/convert_to_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/utils/sampler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/utils/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:52:07.682536 astartes-1.0.1/astartes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-06-04 23:52:07.000000 astartes-1.0.1/astartes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-04 23:52:07.000000 astartes-1.0.1/astartes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 23:52:07.000000 astartes-1.0.1/astartes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-04 23:52:07.000000 astartes-1.0.1/astartes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-04 23:52:07.000000 astartes-1.0.1/astartes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-04 23:51:56.000000 astartes-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 23:52:07.686536 astartes-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:01:23.773871 astartes-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-06 01:01:10.000000 astartes-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-06-06 01:01:23.773871 astartes-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17390 2023-06-06 01:01:10.000000 astartes-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:01:23.765871 astartes-1.0.2/astartes/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17874 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/molecules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:01:23.765871 astartes-1.0.2/astartes/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/samplers/abstract_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:01:23.769871 astartes-1.0.2/astartes/samplers/extrapolation/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/samplers/extrapolation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/samplers/extrapolation/dbscan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/samplers/extrapolation/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/samplers/extrapolation/optisim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/samplers/extrapolation/scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/samplers/extrapolation/sphere_exclusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/samplers/extrapolation/time_based.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:01:23.769871 astartes-1.0.2/astartes/samplers/interpolation/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/samplers/interpolation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/samplers/interpolation/kennardstone.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/samplers/interpolation/mtsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/samplers/interpolation/random_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/samplers/interpolation/spxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:01:23.769871 astartes-1.0.2/astartes/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/utils/convert_to_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/utils/sampler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/utils/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:01:23.765871 astartes-1.0.2/astartes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-06-06 01:01:23.000000 astartes-1.0.2/astartes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-06 01:01:23.000000 astartes-1.0.2/astartes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 01:01:23.000000 astartes-1.0.2/astartes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-06 01:01:23.000000 astartes-1.0.2/astartes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-06 01:01:23.000000 astartes-1.0.2/astartes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-06 01:01:10.000000 astartes-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 01:01:23.773871 astartes-1.0.2/setup.cfg
```

### Comparing `astartes-1.0.1/LICENSE` & `astartes-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `astartes-1.0.1/PKG-INFO` & `astartes-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astartes
-Version: 1.0.1
+Version: 1.0.2
 Summary: Train:Test Algorithmic Sampling for Molecules and Arbitrary Arrays
 Author-email: Jackson Burns <jwburns@mit.edu>, Himaghna Bhattacharjee <himaghna@udel.edu>, Kevin Spiekermann <kspieker@mit.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/JacksonBurns/astartes
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `astartes-1.0.1/README.md` & `astartes-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `astartes-1.0.1/astartes/main.py` & `astartes-1.0.2/astartes/main.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.1/astartes/molecules.py` & `astartes-1.0.2/astartes/molecules.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.1/astartes/samplers/__init__.py` & `astartes-1.0.2/astartes/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.1/astartes/samplers/abstract_sampler.py` & `astartes-1.0.2/astartes/samplers/abstract_sampler.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.1/astartes/samplers/extrapolation/dbscan.py` & `astartes-1.0.2/astartes/samplers/extrapolation/dbscan.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.1/astartes/samplers/extrapolation/kmeans.py` & `astartes-1.0.2/astartes/samplers/extrapolation/kmeans.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.1/astartes/samplers/extrapolation/optisim.py` & `astartes-1.0.2/astartes/samplers/extrapolation/optisim.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.1/astartes/samplers/extrapolation/scaffold.py` & `astartes-1.0.2/astartes/samplers/extrapolation/scaffold.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.1/astartes/samplers/extrapolation/sphere_exclusion.py` & `astartes-1.0.2/astartes/samplers/extrapolation/sphere_exclusion.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.1/astartes/samplers/extrapolation/time_based.py` & `astartes-1.0.2/astartes/samplers/extrapolation/time_based.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.1/astartes/samplers/interpolation/random_split.py` & `astartes-1.0.2/astartes/samplers/interpolation/random_split.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.1/astartes/samplers/interpolation/spxy.py` & `astartes-1.0.2/astartes/samplers/interpolation/kennardstone.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,74 +1,43 @@
-"""
-Implements the Sample set Partitioning based on join X-Y distances
-algorithm as originally described by Saldanha and coworkers in
-"A method for calibration and validation subset partitioning"
-doi:10.1016/j.talanta.2005.03.025
-
-This implementation has been validated against their original source
-code implementation, which can be found in the paper linked above.
-The corresponding unit tests reflect the expected output from
-the original implemenation. The breaking of ties is different
-compared to the original, but this is ultimately a minor and
-likely inconsequential difference.
-"""
 import numpy as np
 from scipy.spatial.distance import pdist, squareform
 
 from astartes.samplers import AbstractSampler
-from astartes.utils.exceptions import InvalidConfigurationError
 
 
-class SPXY(AbstractSampler):
+class KennardStone(AbstractSampler):
     def __init__(self, *args):
-        if args[1] is None:
-            raise InvalidConfigurationError(
-                "SPXY sampler requires both X and y arrays. Provide y or switch to kennard_stone."
-            )
         super().__init__(*args)
 
     def _sample(self):
         """
-        Implements the SPXY algorithm as described by Saldahna et al.
+        Implements the Kennard-Stone algorithm
         """
         n_samples = len(self.X)
 
         distance_metric = self.get_config("metric", "euclidean")
-
-        y_2d = self.y[:, np.newaxis]
-
-        y_pdist = pdist(y_2d, metric=distance_metric)
-        y_pdist = np.divide(y_pdist, np.amax(y_pdist))
-
         X_dist = pdist(self.X, metric=distance_metric)
-        X_dist = np.divide(X_dist, np.amax(X_dist))
-
-        # sum the distances as per eq. 3 of Saldahna, set diagonal to nan
-        spxy_distance = squareform(y_pdist + X_dist)
-        np.fill_diagonal(spxy_distance, -np.inf)
+        ks_distance = squareform(X_dist)
+        # when searching for max distance, disregard self
+        np.fill_diagonal(ks_distance, -np.inf)
 
         # get the row/col of maximum (greatest distance)
-        max_idx = np.nanargmax(spxy_distance)
-        max_coords = np.unravel_index(max_idx, spxy_distance.shape)
+        max_idx = np.nanargmax(ks_distance)
+        max_coords = np.unravel_index(max_idx, ks_distance.shape)
 
-        # -np.inf these points to trick numpy later on
-        spxy_distance[max_coords[0], :] = -np.inf
-        spxy_distance[max_coords[1], :] = -np.inf
-
-        # list of indices which have been selected, for use in the below loop
-        alread_selected = list()
-        alread_selected.append(max_coords[0])
-        alread_selected.append(max_coords[1])
+        # list of indices which have been selected
+        # - used to mask ks_distance
+        # - also tracks order of kennard-stone selection
+        already_selected = list(max_coords)
 
-        # iterate through the rest
+        # minimum distance of all unselected samples to the two selected samples
+        min_distances = np.min(ks_distance[:, already_selected], axis=1)
         for _ in range(n_samples - 2):
             # find the next sample with the largest minimum distance to any sample already selected
-            # get out the columns for the data already selected
-            select_spxy_distance = spxy_distance[:, alread_selected]
-            # find which member of the selected data each of the unselected data is closest to
-            min_distances_vals = np.nanmin(select_spxy_distance, axis=1)
-            # pick the largest of those values
-            max_min_idx = np.nanargmax(min_distances_vals)
-            spxy_distance[max_min_idx, :] = -np.inf
-            alread_selected.append(max_min_idx)
+            already_selected.append(
+                np.argmax(min_distances),
+            )
+            # get minimum distance of unselected samples to that sample only
+            new_distances = np.min(ks_distance[:, [already_selected[-1]]], axis=1)
+            min_distances = np.minimum(min_distances, new_distances)
 
-        self._samples_idxs = np.array(alread_selected, dtype=int)
+        self._samples_idxs = np.array(already_selected, dtype=int)
```

### Comparing `astartes-1.0.1/astartes/utils/convert_to_array.py` & `astartes-1.0.2/astartes/utils/convert_to_array.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.1/astartes/utils/exceptions.py` & `astartes-1.0.2/astartes/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.1/astartes/utils/sampler_factory.py` & `astartes-1.0.2/astartes/utils/sampler_factory.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.1/astartes/utils/warnings.py` & `astartes-1.0.2/astartes/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.1/astartes.egg-info/PKG-INFO` & `astartes-1.0.2/astartes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astartes
-Version: 1.0.1
+Version: 1.0.2
 Summary: Train:Test Algorithmic Sampling for Molecules and Arbitrary Arrays
 Author-email: Jackson Burns <jwburns@mit.edu>, Himaghna Bhattacharjee <himaghna@udel.edu>, Kevin Spiekermann <kspieker@mit.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/JacksonBurns/astartes
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `astartes-1.0.1/astartes.egg-info/SOURCES.txt` & `astartes-1.0.2/astartes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astartes-1.0.1/pyproject.toml` & `astartes-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "astartes"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
     { name = "Jackson Burns", email = "jwburns@mit.edu" },
     { name = "Himaghna Bhattacharjee", email = "himaghna@udel.edu" },
     { name = "Kevin Spiekermann", email = "kspieker@mit.edu" },
 ]
 license = { text = "MIT" }
 description = "Train:Test Algorithmic Sampling for Molecules and Arbitrary Arrays"
```

