# Comparing `tmp/metricspace-0.5.0.tar.gz` & `tmp/metricspace-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metricspace-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "metricspace-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `metricspace-0.5.0.tar` & `metricspace-0.6.0.tar`

### file list

```diff
@@ -1,26 +1,32 @@
--rw-r--r--   0        0        0       15 2023-05-31 03:34:59.307740 metricspace-0.5.0/.gitattributes
--rw-r--r--   0        0        0      207 2023-06-03 20:32:15.687932 metricspace-0.5.0/.gitignore
--rw-r--r--   0        0        0     1092 2023-06-03 20:34:39.576899 metricspace-0.5.0/LICENSE
--rw-r--r--   0        0        0     4121 2023-06-04 00:01:05.996089 metricspace-0.5.0/README.md
--rw-r--r--   0        0        0        0 2023-06-02 23:54:22.575801 metricspace-0.5.0/examples/ex_distances.py
--rw-r--r--   0        0        0      368 2023-06-03 20:42:47.249595 metricspace-0.5.0/metricspace.egg-info/PKG-INFO
--rw-r--r--   0        0        0      625 2023-06-03 20:42:47.271461 metricspace-0.5.0/metricspace.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2023-06-03 20:42:47.250297 metricspace-0.5.0/metricspace.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       12 2023-06-03 20:42:47.250297 metricspace-0.5.0/metricspace.egg-info/top_level.txt
--rw-r--r--   0        0        0      175 2023-06-03 20:42:23.565089 metricspace-0.5.0/metricspace/__init__.py
--rw-r--r--   0        0        0      310 2023-06-03 20:32:56.972513 metricspace-0.5.0/metricspace/entropy/__init__.py
--rw-r--r--   0        0        0      898 2023-06-03 20:27:52.969199 metricspace-0.5.0/metricspace/entropy/histbi.py
--rw-r--r--   0        0        0      540 2023-06-03 20:27:52.969199 metricspace-0.5.0/metricspace/entropy/histinfo.py
--rw-r--r--   0        0        0      687 2023-06-03 20:27:52.969915 metricspace-0.5.0/metricspace/entropy/histjabi.py
--rw-r--r--   0        0        0      703 2023-06-03 20:27:52.969915 metricspace-0.5.0/metricspace/entropy/histtpbi.py
--rw-r--r--   0        0        0      987 2023-06-03 20:27:52.970909 metricspace-0.5.0/metricspace/entropy/tblxbi.py
--rw-r--r--   0        0        0      405 2023-06-03 20:27:52.970909 metricspace-0.5.0/metricspace/entropy/tblxinfo.py
--rw-r--r--   0        0        0     1322 2023-06-03 20:27:52.970909 metricspace-0.5.0/metricspace/entropy/tblxtpbi.py
--rw-r--r--   0        0        0      119 2023-06-03 20:27:52.971909 metricspace-0.5.0/metricspace/model/__init__.py
--rw-r--r--   0        0        0       74 2023-06-03 20:27:52.972909 metricspace-0.5.0/metricspace/model/calculate_spkd/__init__.py
--rw-r--r--   0        0        0     7378 2023-06-03 20:27:52.972909 metricspace-0.5.0/metricspace/model/calculate_spkd/spkd_functions.py
--rw-r--r--   0        0        0     6263 2023-06-03 20:27:52.972909 metricspace-0.5.0/metricspace/model/distclust.py
--rw-r--r--   0        0        0     1447 2023-06-03 20:27:52.973910 metricspace-0.5.0/metricspace/model/spkd.py
--rw-r--r--   0        0        0      853 2023-06-04 00:03:20.640991 metricspace-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       49 2023-06-03 19:43:56.794865 metricspace-0.5.0/requirements.txt
--rw-r--r--   0        0        0     4656 1970-01-01 00:00:00.000000 metricspace-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0       15 2023-05-31 03:34:59.307740 metricspace-0.6.0/.gitattributes
+-rw-r--r--   0        0        0     1351 2023-06-06 15:51:47.403236 metricspace-0.6.0/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      207 2023-06-03 20:32:15.687932 metricspace-0.6.0/.gitignore
+-rw-r--r--   0        0        0      260 2023-06-06 15:18:39.063233 metricspace-0.6.0/.vscode/settings.json
+-rw-r--r--   0        0        0     1092 2023-06-03 20:34:39.576899 metricspace-0.6.0/LICENSE
+-rw-r--r--   0        0        0     6111 2023-06-05 16:11:23.195528 metricspace-0.6.0/README.md
+-rwxr-xr-x   0        0        0       50 2023-06-05 14:52:22.100017 metricspace-0.6.0/bld.bat
+-rw-r--r--   0        0        0       24 2023-06-05 14:52:45.229190 metricspace-0.6.0/build.sh
+-rw-r--r--   0        0        0     1201 2023-06-05 15:18:54.100213 metricspace-0.6.0/examples/ex_distances.py
+-rw-r--r--   0        0        0      307 2023-06-06 15:54:05.576735 metricspace-0.6.0/meta.yaml
+-rw-r--r--   0        0        0      368 2023-06-03 20:42:47.249595 metricspace-0.6.0/metricspace.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      625 2023-06-03 20:42:47.271461 metricspace-0.6.0/metricspace.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2023-06-03 20:42:47.250297 metricspace-0.6.0/metricspace.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       12 2023-06-03 20:42:47.250297 metricspace-0.6.0/metricspace.egg-info/top_level.txt
+-rw-r--r--   0        0        0      175 2023-06-03 20:42:23.565089 metricspace-0.6.0/metricspace/__init__.py
+-rw-r--r--   0        0        0      310 2023-06-03 20:32:56.972513 metricspace-0.6.0/metricspace/entropy/__init__.py
+-rw-r--r--   0        0        0      898 2023-06-03 20:27:52.969199 metricspace-0.6.0/metricspace/entropy/histbi.py
+-rw-r--r--   0        0        0      540 2023-06-03 20:27:52.969199 metricspace-0.6.0/metricspace/entropy/histinfo.py
+-rw-r--r--   0        0        0      687 2023-06-03 20:27:52.969915 metricspace-0.6.0/metricspace/entropy/histjabi.py
+-rw-r--r--   0        0        0      703 2023-06-03 20:27:52.969915 metricspace-0.6.0/metricspace/entropy/histtpbi.py
+-rw-r--r--   0        0        0      987 2023-06-03 20:27:52.970909 metricspace-0.6.0/metricspace/entropy/tblxbi.py
+-rw-r--r--   0        0        0      405 2023-06-03 20:27:52.970909 metricspace-0.6.0/metricspace/entropy/tblxinfo.py
+-rw-r--r--   0        0        0     1322 2023-06-03 20:27:52.970909 metricspace-0.6.0/metricspace/entropy/tblxtpbi.py
+-rw-r--r--   0        0        0      119 2023-06-03 20:27:52.971909 metricspace-0.6.0/metricspace/model/__init__.py
+-rw-r--r--   0        0        0       74 2023-06-03 20:27:52.972909 metricspace-0.6.0/metricspace/model/calculate_spkd/__init__.py
+-rw-r--r--   0        0        0     7994 2023-06-06 15:48:04.959619 metricspace-0.6.0/metricspace/model/calculate_spkd/spkd_functions.py
+-rw-r--r--   0        0        0     6263 2023-06-03 20:27:52.972909 metricspace-0.6.0/metricspace/model/distclust.py
+-rw-r--r--   0        0        0     2065 2023-06-06 15:47:25.912947 metricspace-0.6.0/metricspace/model/spkd.py
+-rw-r--r--   0        0        0      386 2023-06-06 15:01:44.940811 metricspace-0.6.0/metricspace/validate/__init__.py
+-rw-r--r--   0        0        0      853 2023-06-06 15:53:12.149849 metricspace-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       49 2023-06-06 15:13:29.314097 metricspace-0.6.0/requirements.txt
+-rw-r--r--   0        0        0     6583 1970-01-01 00:00:00.000000 metricspace-0.6.0/PKG-INFO
```

### Comparing `metricspace-0.5.0/LICENSE` & `metricspace-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metricspace-0.5.0/metricspace.egg-info/SOURCES.txt` & `metricspace-0.6.0/metricspace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metricspace-0.5.0/metricspace/entropy/histbi.py` & `metricspace-0.6.0/metricspace/entropy/histbi.py`

 * *Files identical despite different names*

### Comparing `metricspace-0.5.0/metricspace/entropy/histinfo.py` & `metricspace-0.6.0/metricspace/entropy/histinfo.py`

 * *Files identical despite different names*

### Comparing `metricspace-0.5.0/metricspace/entropy/histjabi.py` & `metricspace-0.6.0/metricspace/entropy/histjabi.py`

 * *Files identical despite different names*

### Comparing `metricspace-0.5.0/metricspace/entropy/histtpbi.py` & `metricspace-0.6.0/metricspace/entropy/histtpbi.py`

 * *Files identical despite different names*

### Comparing `metricspace-0.5.0/metricspace/entropy/tblxbi.py` & `metricspace-0.6.0/metricspace/entropy/tblxbi.py`

 * *Files identical despite different names*

### Comparing `metricspace-0.5.0/metricspace/entropy/tblxtpbi.py` & `metricspace-0.6.0/metricspace/entropy/tblxtpbi.py`

 * *Files identical despite different names*

### Comparing `metricspace-0.5.0/metricspace/model/calculate_spkd/spkd_functions.py` & `metricspace-0.6.0/metricspace/model/calculate_spkd/spkd_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,41 +5,54 @@
 
 They are private to clean up the public namespace, avoid circular imports, and prevent confusion about which
 spike distance function is being called.
 
 """
 import numpy as np
 import importlib.util
+import warnings
 from numba import jit
 
-rs_distances_spec = importlib.util.find_spec('rs_distances')
+rs_distances_spec = importlib.util.find_spec("rs_distances")
 
 if rs_distances_spec is not None:
     try:
         import rs_distances
     except ImportError:
-        print('Error during import of rs_distances. Fallback to spkd_v function.')
+        print("Error during import of rs_distances. Fallback to spkd.py.")
         rs_distances = None
 else:
+    print("rs_distances not installed. Fallback to spkd.py.")
     rs_distances = None
 
 
 # Outer Entrypoint -----------------------------------------------------------------------------------------------------
-def calculate_spkd(cspks: np.ndarray | list, qvals: list | np.ndarray, res: float | int | None = 1e-4):
+def calculate_spkd(
+    cspks: np.ndarray | list, qvals: list | np.ndarray, res: float | int | None = 1e-2
+):
     """
-       Internal function to compute pairwise spike train distances with variable time precision for multiple cost values.
+    Internal function to compute pairwise spike train distances with variable time precision for multiple cost values.
+
+    Args:
+        cspks (nested iterable[list | np.ndarray]): Each inner list contains spike times for a single spike train.
+        qvals (list of float | int): List of time precision values to use in the computation.
+        res (float, optional): The search resolution of the spike trains. Defaults to 1e-4.
+
+    Returns:
+        ndarray: A 3D array containing pairwise spike train distances for each time precision value.
+
+      Raises:
+             TypeError: If cspks is not a list or numpy array.
+    """
+    if res is not None and res < 0.1:
+        warnings.warn(
+            "Setting a small value for 'res' using the python implementation may result in long computation time.",
+            UserWarning,
+        )
 
-       Args:
-           cspks (nested iterable[list | np.ndarray]): Each inner list contains spike times for a single spike train.
-           qvals (list of float | int): List of time precision values to use in the computation.
-           res (float, optional): The search resolution of the spike trains. Defaults to 1e-4.
-
-       Returns:
-           ndarray: A 3D array containing pairwise spike train distances for each time precision value.
-       """
     if not isinstance(qvals, np.ndarray):
         # Check if qvals is a numpy array
         qvals = np.array(qvals)
 
     # Calculate the count of spikes in each spike train
     curcounts = [len(x) for x in cspks]
     numt = len(cspks)
@@ -55,31 +68,37 @@
                 spk_train_b = np.array(cspks[xj])
 
                 offsets = np.arange(-1, 1 + res, res) if res else [0]
                 for offset in offsets:
                     if res:
                         spk_train_a = spk_train_a + offset
 
-                    outer_diff = np.abs(spk_train_a.reshape(-1, 1) - spk_train_b.reshape(1, -1))
+                    outer_diff = np.abs(
+                        spk_train_a.reshape(-1, 1) - spk_train_b.reshape(1, -1)
+                    )
                     sd = qvals.reshape((-1, 1, 1)) * outer_diff
                     scr = np.zeros((len(qvals), curcounts[xi] + 1, curcounts[xj] + 1))
                     scr[:, 1:, 0] += np.arange(1, curcounts[xi] + 1)
                     scr[:, 0, 1:] += np.arange(1, curcounts[xj] + 1).reshape((1, -1))
 
                     d_current = _compute_spike_distance(scr, sd)
-                    d[xi, xj, :] = np.minimum(d[xi, xj, :], d_current) if offset != -1 else d_current
+                    d[xi, xj, :] = (
+                        np.minimum(d[xi, xj, :], d_current)
+                        if offset != -1
+                        else d_current
+                    )
             else:
                 d[xi, xj, :] = max(curcounts[xi], curcounts[xj])
     return np.maximum(d, np.transpose(d, [1, 0, 2]))
 
 
 # Check if rs_distances is installed -----------------------------------------------------------------------------------
 def _compute_spike_distance(scr, sd):
     """
-    Compute spike-time distance, using either the rs_distances module (if installed and importable) or
+    Internal. Compute spike-time distance, using either the rs_distances module (if installed and importable) or
     the fallback iterate_spiketrains @jit decorated function.
 
     Args:
         scr, sd: Input arguments for the distance computation function.
 
     Returns:
         numpy.ndarray: The result of the spike-time distance computation.
@@ -88,17 +107,18 @@
         return _spkd_v_rs(scr, sd)
     else:
         return _spkd_v(scr, sd)
 
 
 # If rs_distances is installed -----------------------------------------------------------------------------------------
 def _spkd_v_rs(scr, sd):
+    """ This is called if calculate_spkd is run in python, but the vectorization is done in rust."""
     scr = rs_distances.iterate_spiketrains_impl(scr, sd)
     # The last column represents the final values of the accumulated cost of aligning the two spike trains
-    d = np.squeeze(scr[:, -1, -1]).astype('float32')
+    d = np.squeeze(scr[:, -1, -1]).astype("float32")
     return d
 
 
 # If rs_distances not installed ----------------------------------------------------------------------------------------
 def _spkd_v(scr, sd):
     """
     Compute spike-time distance.
@@ -116,15 +136,15 @@
     Returns:
         numpy.ndarray: A 1D array representing the spike-time distances.
     """
     # Need to separate this iteration for compatibility with numba
     scr = _iterate_spiketrains(scr, sd)
 
     # The last column represents the final values of the accumulated cost of aligning the two spike trains
-    d = np.squeeze(scr[:, -1, -1]).astype('float32')
+    d = np.squeeze(scr[:, -1, -1]).astype("float32")
 
     return d
 
 
 @jit(nopython=True, fastmath=True)
 def _iterate_spiketrains(scr, sd):
     """
```

### Comparing `metricspace-0.5.0/metricspace/model/distclust.py` & `metricspace-0.6.0/metricspace/model/distclust.py`

 * *Files identical despite different names*

### Comparing `metricspace-0.5.0/metricspace/model/spkd.py` & `metricspace-0.6.0/metricspace/model/spkd.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,38 @@
 import numpy as np
 from .calculate_spkd import spkd_functions
+import importlib
+rs_distances_spec = importlib.util.find_spec('rs_distances')
 
+if rs_distances_spec is not None:
+    try:
+        import rs_distances
+    except ImportError:
+        print('Error during import of rs_distances. Fallback to spkd_v function.')
+        rs_distances = None
+else:
+    rs_distances = None
 
-def spkd(cspks: np.ndarray | list, qvals: list | np.ndarray):
+def spkd(cspks: np.ndarray | list, qvals: list | np.ndarray, use_rs: bool = True):
     """
     Compute pairwise spike train distances with variable time precision for multiple cost values.
 
     Args:
         cspks (nested iterable[list | np.ndarray]): Each inner list contains spike times for a single spike train.
         qvals (list of float | int): List of time precision values to use in the computation.
+        use_rs (bool, optional): Whether to use the rs_distances implementation. Defaults to True.
 
     Returns:
         ndarray: A 3D array containing pairwise spike train distances for each time precision value.
     """
-    return spkd_functions.calculate_spkd(cspks, qvals, None)
+    if rs_distances is not None and use_rs:
+        d = rs_distances.calculate_spkd(cspks, qvals)
+        return np.maximum(d, np.transpose(d, [1, 0, 2]))
+    else:
+        return spkd_functions.calculate_spkd(cspks, qvals, None)
 
 
 def spkd_slide(cspks: np.ndarray | list, qvals: list | np.ndarray, res: float | int = 1e-3):
     """
     Compute pairwise spike train distances with variable time precision for multiple cost values,
     incorporating sliding of one spike train along the time axis.
```

### Comparing `metricspace-0.5.0/pyproject.toml` & `metricspace-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "metricspace"
-version = "0.5.0"
+version = "0.6.0"
 description = "A python translation of code originally theorized in: Metric-space analysis of spike trains: theory, algorithms, and application Jonathan D. Victor and Keith Purpura Network 8, 127-164 (1997)"
 authors = [
     {name = "Flynn OConnell", email = "flynnoconnell@gmail.com"},
     {name = "Jonathan D Victor", email = "jdvicto@med.cornell.edu"}
 ]
 
 readme = "README.md"
```

### Comparing `metricspace-0.5.0/PKG-INFO` & `metricspace-0.6.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,104 @@
 Metadata-Version: 2.1
 Name: metricspace
-Version: 0.5.0
+Version: 0.6.0
 Summary: A python translation of code originally theorized in: Metric-space analysis of spike trains: theory, algorithms, and application Jonathan D. Victor and Keith Purpura Network 8, 127-164 (1997)
 Author-email: Flynn OConnell <flynnoconnell@gmail.com>, Jonathan D Victor <jdvicto@med.cornell.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 
 
-## Metric Space Analysis - A Python Implementation 
+# Metric Space Analysis - A Python Implementation 
 
 ![Python](https://img.shields.io/badge/python-3670A0?style=?style=plastic&logo=python&logoColor=ffdd54)
-![C++](https://img.shields.io/badge/c++-%2300599C.svg?style=plastic&logo=c%2B%2B&logoColor=white)
-![Rust](https://img.shields.io/badge/rust-%23000000.svg?style=plastic&logo=rust&logoColor=white)
+![Rust](https://img.shields.io/badge/rust-000000?style=?style=plastic&logo=rust&logoColor=white)
 [![GitHub license](https://badgen.net/github/license/Naereen/Strapdown.js)](https://github.com/NeuroPyPy/metricspace/blob/master/LICENSE)
 
 * <a href=https://journals.physiology.org/doi/abs/10.1152/jn.1996.76.2.1310> Nature and precision of temporal coding in visual cortex: a metric-space analysis. Victor & Purpura (1996)</a>
 * <a href="https://www.tandfonline.com/doi/abs/10.1088/0954-898X_8_2_003"> Metric space analysis of spike trains: theory, algorithms and application. Victor & Purpura (1997) </a>
-For a full walkthrough of cost-based metrics, see Dr. Jonathon Victor's <a href="http://www-users.med.cornell.edu/~jdvicto/metricdf.html#introduction"> website: </a> 
+
+<br>
+
+For a full walkthrough of cost-based metrics, see Jonathon Victor's <a href="http://www-users.med.cornell.edu/~jdvicto/metricdf.html#introduction"> website: </a> 
+
 > Spike trains are considered to be points in an abstract topological space. A spike train metric is a rule which assigns a non-negative number D(Sa,Sb) to pairs of spike trains Sa and Sb which expresses how dissimilar they are.
+ 
+<br>
 
 This repository hosts a Python implementation of the metric space analysis algorithms with several optimizations:
-* The more computationally intensive functions are implemented in Rust and compiled into a shared library that can be utilized within Python.
-* Vectorized array computation leveraging the power of numpy.
-* Parallelization of independent spike-trains using the multiprocessing library.
+* The more computationally intensive functions are <a href="http://github.com/NeuroPyPy/rs-distances"> implemented in Rust (with benchmarks for matlab, python and rust)</a> and compiled into a shared library that can be utilized within Python.
+* Spike train loops are vectorized, limiting the "auto-vectorization" safety and leveraging th epower of modern AVX2 vector instructions.
+* Parallelization of independent spike-trains using the multiprocessing library (multithreading in the works).
+
+<br>
 
 In addition to the standard approach for spike-distance calculations, this package exposes a modified "sliding window" approach that can be used to calculate spike distances for spike trains of unequal length.
 
+<br>
+
+----
+
 ## Installation
+
+<br>
+
 To install this package, run the following command:
 ```bash
 pip install metricspace
 ```
-or with conda package manager:
-```bash
-conda install -c  metricspace
-```
-**Note**: Be sure to activate your virtual environment with Python 3.7 or higher before installing this package via pip or anaconda so that the Rust library can be compiled correctly and has access to your python interpreter.
+**Note**: Be sure to activate a vertual env (penv or conda env) with Python 3.7 or higher before installing this package so that the Rust library can be compiled correctly and has access to your python interpreter.
+
+<br>
+
+### Installation with pipenv
+
+**Ensure your pip is up-to-date, and confirm activated venv**
+
+| MacOS/Unix                                      | Windows                                            |
+|:------------------------------------------------|:---------------------------------------------------|
+| `python3 -m pip install --upgrade pip`          | `py -m pip install --upgrade pip`                  |
+| `python3 -m pip --version`                      | `py -m pip --version`                              |
+| `python3 -m pip install --user virtualenv`      | `py -m pip install --user virtualenv`              |
+| `python3 -m venv env`                           | `py -m env_metricspace env`                       |
+| `source env/bin/activate`                       | `.\env\Scripts\activate`                           |
+| `.../env/bin/python`                            |                                                     |
+
+**Validate your active interpreter is in your venv and install metricspace**
+
+| MacOS/Unix                                      | Windows                                            |
+|:------------------------------------------------|:---------------------------------------------------|
+| `which python`                                  | `where python`                                     |
+| `.../env/bin/python`                            | `...\env_metricspace\Scripts\python.exe`           |
+| `python3 -m pip install metricspace`            | `py -m pip install metricspace`                    |
 
-## Exposed Functions
+<br>
+
+----
+
+
+## Usage
+
+<br>
+
+### Exposed Functions
 The following functions are exposed by this package:
 * `spkd` - Calculates the spike distance between two or more spike trains.
 * `spkd_slide` - Calculates the spike distance between two or more spike trains using a sliding window approach.
 * `distclust` - Uses spike distance to cluster spike trains for entropy calculations.
 * `tblxinfo` -  Uses the distclust confusion matrix output (probability, not count) to calculate mutual information.
 * `tblxtpbi` - Similar to tblxinfo but with Treves and Panzeri's bias correction.
-* `tblxjabi` - Similar to tblxinfo but with jacknife bias correction.
+* `tblxbi` - Similar to tblxinfo but with jacknife or tp bias correction.
+
+<br>
+
+### Example
 
-## Usage
 ```python
 import metricspace as ms
 import numpy as np
 
 # Generate random spike trains
 spike_train_A = np.sort(np.random.uniform(low=0.0, high=2, size=100))
 spike_train_B = np.sort(np.random.uniform(low=0.0, high=2, size=100))
@@ -67,14 +112,32 @@
 spike_distance = ms.spkd(spike_trains, costs)  # Standard approach
 spike_distance_slide = ms.spkd_slide(spike_trains, costs, 10e-3)  # Sliding window approach with search window of 1ms
 
 # Cluster spike trains using spike distance and the number of samples in each class
 spike_train_class_labels = np.concatenate((np.zeros(100), np.ones(100))) # 100 samples in each class, randomly generated
 _, nsam = np.unique(spike_train_class_labels, return_counts=True)
 clustered = ms.distclust(spike_distance, nsam)
+
+# Calculate entropy from the confusion matrix output of distclust
+mi = ms.tblxinfo(clustered)
+mj = ms.tblxjabi(clustered)
+mt = ms.tblxtpbi(clustered)
+mij = mi + mj
+mit = mi + mt
+
 ```
 
+<br>
+
+----
+
+<br>
+
+## Contributions
+
+Any contributions, improvements or suggestions are welcome. 
 
 ### Original Developers
 Jonathan D. Victor: jdvicto@med.cornell.edu
 Keith P. Purpura: kpurpura@med.cornell.edu
 Dmitriy Aronov: aronov@mit.edu 
+
```

#### html2text {}

```diff
@@ -1,61 +1,81 @@
-Metadata-Version: 2.1 Name: metricspace Version: 0.5.0 Summary: A python
+Metadata-Version: 2.1 Name: metricspace Version: 0.6.0 Summary: A python
 translation of code originally theorized in: Metric-space analysis of spike
 trains: theory, algorithms, and application Jonathan D. Victor and Keith
 Purpura Network 8, 127-164 (1997) Author-email: Flynn OConnell
 gmail.com>, Jonathan D Victor
 med.cornell.edu> Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Rust Classifier: Programming Language ::
 Python :: Implementation :: CPython Classifier: Programming Language :: Python
-:: Implementation :: PyPy ## Metric Space Analysis - A Python Implementation !
+:: Implementation :: PyPy # Metric Space Analysis - A Python Implementation !
 [Python](https://img.shields.io/badge/python-
-3670A0?style=?style=plastic&logo=python&logoColor=ffdd54) ![C++](https://
-img.shields.io/badge/c++-
-%2300599C.svg?style=plastic&logo=c%2B%2B&logoColor=white) ![Rust](https://
+3670A0?style=?style=plastic&logo=python&logoColor=ffdd54) ![Rust](https://
 img.shields.io/badge/rust-
-%23000000.svg?style=plastic&logo=rust&logoColor=white) [![GitHub license]
+000000?style=?style=plastic&logo=rust&logoColor=white) [![GitHub license]
 (https://badgen.net/github/license/Naereen/Strapdown.js)](https://github.com/
 NeuroPyPy/metricspace/blob/master/LICENSE) * Nature_and_precision_of_temporal
 coding_in_visual_cortex:_a_metric-space_analysis._Victor_&_Purpura_(1996) *
 Metric_space_analysis_of_spike_trains:_theory,_algorithms_and_application.
-Victor_&_Purpura_(1997) For a full walkthrough of cost-based metrics, see Dr.
-Jonathon Victor's website: > Spike trains are considered to be points in an
-abstract topological space. A spike train metric is a rule which assigns a non-
-negative number D(Sa,Sb) to pairs of spike trains Sa and Sb which expresses how
-dissimilar they are. This repository hosts a Python implementation of the
-metric space analysis algorithms with several optimizations: * The more
-computationally intensive functions are implemented in Rust and compiled into a
-shared library that can be utilized within Python. * Vectorized array
-computation leveraging the power of numpy. * Parallelization of independent
-spike-trains using the multiprocessing library. In addition to the standard
-approach for spike-distance calculations, this package exposes a modified
-"sliding window" approach that can be used to calculate spike distances for
-spike trains of unequal length. ## Installation To install this package, run
-the following command: ```bash pip install metricspace ``` or with conda
-package manager: ```bash conda install -c metricspace ``` **Note**: Be sure to
-activate your virtual environment with Python 3.7 or higher before installing
-this package via pip or anaconda so that the Rust library can be compiled
-correctly and has access to your python interpreter. ## Exposed Functions The
-following functions are exposed by this package: * `spkd` - Calculates the
-spike distance between two or more spike trains. * `spkd_slide` - Calculates
-the spike distance between two or more spike trains using a sliding window
-approach. * `distclust` - Uses spike distance to cluster spike trains for
-entropy calculations. * `tblxinfo` - Uses the distclust confusion matrix output
-(probability, not count) to calculate mutual information. * `tblxtpbi` -
-Similar to tblxinfo but with Treves and Panzeri's bias correction. * `tblxjabi`
-- Similar to tblxinfo but with jacknife bias correction. ## Usage ```python
-import metricspace as ms import numpy as np # Generate random spike trains
-spike_train_A = np.sort(np.random.uniform(low=0.0, high=2, size=100))
-spike_train_B = np.sort(np.random.uniform(low=0.0, high=2, size=100)) # Input
-spike trains into a list or array (as many or few as you want) spike_trains =
-[spike_train_A, spike_train_B] # Make array of cost values to be used in the
-spike-distance calculation (here we get 0 to 512) costs = np.concatenate(([0],
-2 ** np.arange(-4, 9.5, 0.5))) spike_distance = ms.spkd(spike_trains, costs) #
-Standard approach spike_distance_slide = ms.spkd_slide(spike_trains, costs,
-10e-3) # Sliding window approach with search window of 1ms # Cluster spike
-trains using spike distance and the number of samples in each class
-spike_train_class_labels = np.concatenate((np.zeros(100), np.ones(100))) # 100
-samples in each class, randomly generated _, nsam = np.unique
+Victor_&_Purpura_(1997)
+For a full walkthrough of cost-based metrics, see Jonathon Victor's website: >
+Spike trains are considered to be points in an abstract topological space. A
+spike train metric is a rule which assigns a non-negative number D(Sa,Sb) to
+pairs of spike trains Sa and Sb which expresses how dissimilar they are.
+This repository hosts a Python implementation of the metric space analysis
+algorithms with several optimizations: * The more computationally intensive
+functions are implemented_in_Rust_(with_benchmarks_for_matlab,_python_and_rust)
+and compiled into a shared library that can be utilized within Python. * Spike
+train loops are vectorized, limiting the "auto-vectorization" safety and
+leveraging th epower of modern AVX2 vector instructions. * Parallelization of
+independent spike-trains using the multiprocessing library (multithreading in
+the works).
+In addition to the standard approach for spike-distance calculations, this
+package exposes a modified "sliding window" approach that can be used to
+calculate spike distances for spike trains of unequal length.
+---- ## Installation
+To install this package, run the following command: ```bash pip install
+metricspace ``` **Note**: Be sure to activate a vertual env (penv or conda env)
+with Python 3.7 or higher before installing this package so that the Rust
+library can be compiled correctly and has access to your python interpreter.
+### Installation with pipenv **Ensure your pip is up-to-date, and confirm
+activated venv** | MacOS/Unix | Windows | |:-----------------------------------
+-------------|:---------------------------------------------------| | `python3
+-m pip install --upgrade pip` | `py -m pip install --upgrade pip` | | `python3
+-m pip --version` | `py -m pip --version` | | `python3 -m pip install --user
+virtualenv` | `py -m pip install --user virtualenv` | | `python3 -m venv env` |
+`py -m env_metricspace env` | | `source env/bin/activate` |
+`.\env\Scripts\activate` | | `.../env/bin/python` | | **Validate your active
+interpreter is in your venv and install metricspace** | MacOS/Unix | Windows |
+|:------------------------------------------------|:---------------------------
+------------------------| | `which python` | `where python` | | `.../env/bin/
+python` | `...\env_metricspace\Scripts\python.exe` | | `python3 -m pip install
+metricspace` | `py -m pip install metricspace` |
+---- ## Usage
+### Exposed Functions The following functions are exposed by this package: *
+`spkd` - Calculates the spike distance between two or more spike trains. *
+`spkd_slide` - Calculates the spike distance between two or more spike trains
+using a sliding window approach. * `distclust` - Uses spike distance to cluster
+spike trains for entropy calculations. * `tblxinfo` - Uses the distclust
+confusion matrix output (probability, not count) to calculate mutual
+information. * `tblxtpbi` - Similar to tblxinfo but with Treves and Panzeri's
+bias correction. * `tblxbi` - Similar to tblxinfo but with jacknife or tp bias
+correction.
+### Example ```python import metricspace as ms import numpy as np # Generate
+random spike trains spike_train_A = np.sort(np.random.uniform(low=0.0, high=2,
+size=100)) spike_train_B = np.sort(np.random.uniform(low=0.0, high=2,
+size=100)) # Input spike trains into a list or array (as many or few as you
+want) spike_trains = [spike_train_A, spike_train_B] # Make array of cost values
+to be used in the spike-distance calculation (here we get 0 to 512) costs =
+np.concatenate(([0], 2 ** np.arange(-4, 9.5, 0.5))) spike_distance = ms.spkd
+(spike_trains, costs) # Standard approach spike_distance_slide = ms.spkd_slide
+(spike_trains, costs, 10e-3) # Sliding window approach with search window of
+1ms # Cluster spike trains using spike distance and the number of samples in
+each class spike_train_class_labels = np.concatenate((np.zeros(100), np.ones
+(100))) # 100 samples in each class, randomly generated _, nsam = np.unique
 (spike_train_class_labels, return_counts=True) clustered = ms.distclust
-(spike_distance, nsam) ``` ### Original Developers Jonathan D. Victor:
-jdvicto@med.cornell.edu Keith P. Purpura: kpurpura@med.cornell.edu Dmitriy
-Aronov: aronov@mit.edu
+(spike_distance, nsam) # Calculate entropy from the confusion matrix output of
+distclust mi = ms.tblxinfo(clustered) mj = ms.tblxjabi(clustered) mt =
+ms.tblxtpbi(clustered) mij = mi + mj mit = mi + mt ```
+----
+## Contributions Any contributions, improvements or suggestions are welcome.
+### Original Developers Jonathan D. Victor: jdvicto@med.cornell.edu Keith P.
+Purpura: kpurpura@med.cornell.edu Dmitriy Aronov: aronov@mit.edu
```

