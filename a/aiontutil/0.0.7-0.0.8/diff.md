# Comparing `tmp/aiontutil-0.0.7.tar.gz` & `tmp/aiontutil-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiontutil-0.0.7.tar", max compression
+gzip compressed data, was "aiontutil-0.0.8.tar", max compression
```

## Comparing `aiontutil-0.0.7.tar` & `aiontutil-0.0.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      283 2023-05-08 08:27:47.285958 aiontutil-0.0.7/README.md
--rw-r--r--   0        0        0       22 2023-05-08 07:09:03.272254 aiontutil-0.0.7/aiontutil/__init__.py
--rw-r--r--   0        0        0     7874 2023-06-06 06:15:36.062162 aiontutil-0.0.7/aiontutil/signal.py
--rw-r--r--   0        0        0      355 2023-06-06 06:17:50.317571 aiontutil-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 aiontutil-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      283 2023-05-08 08:27:47.285958 aiontutil-0.0.8/README.md
+-rw-r--r--   0        0        0       22 2023-05-08 07:09:03.272254 aiontutil-0.0.8/aiontutil/__init__.py
+-rw-r--r--   0        0        0     8302 2023-06-06 08:50:40.368893 aiontutil-0.0.8/aiontutil/signal.py
+-rw-r--r--   0        0        0      355 2023-06-06 08:51:30.105264 aiontutil-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 aiontutil-0.0.8/PKG-INFO
```

### Comparing `aiontutil-0.0.7/aiontutil/signal.py` & `aiontutil-0.0.8/aiontutil/signal.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import List, Optional
+from typing import Callable, Dict, List, Optional, Set, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import scipy as sp
 from scipy import stats
 
 
 def list_all_feature_names() -> List[str]:
     """
     Returns a list of available feature names.
     """
     return list(name_dict.keys())
 
 
-def get_freq_amp(x: np.ndarray, fs: int):
+def get_freq_amp(x: np.ndarray, fs: int) -> Tuple[np.ndarray, np.ndarray]:
     """
     Examples
     --------
     >>> n_secs = 5
     >>> fs = 256
     >>> true_freqs = np.array([11, 23, 31, 41])
     >>> true_amps = np.array([13, 29, 37, 43])
@@ -31,15 +31,15 @@
     freq = sp.fft.fftfreq(n, d=1 / fs)
     fhat = sp.fft.fft(x)
     amp = 2 * np.abs(fhat) / n
     amp[..., 0] = 0
     return freq[: n // 2].copy(), amp[..., : n // 2].copy()
 
 
-def get_ratio_max_upper_fence(x: np.ndarray, axis=-1, keepdims=False):
+def get_ratio_max_upper_fence(x: np.ndarray, axis=-1, keepdims=False) -> np.ndarray:
     """
     Examples
     --------
     >>> feat = get_ratio_max_upper_fence(np.random.randn(10, 1024))
     >>> feat.shape
     (10,)
     >>> feat = get_ratio_max_upper_fence(np.random.randn(10, 1024), keepdims=True)
@@ -50,39 +50,39 @@
     if np.ndim(x) == 1:
         x = x[np.newaxis, ...]
     _max = np.max(x, axis=axis, keepdims=keepdims)
     _upper_fence = get_upper_fence(x, axis=axis, keepdims=keepdims)
     return _max / _upper_fence
 
 
-def get_rmeds(x: np.ndarray, axis=-1, keepdims=False):
+def get_rmeds(x: np.ndarray, axis=-1, keepdims=False) -> np.ndarray:
     """
     Examples
     --------
     >>> rmeds = get_rmeds(np.random.randn(10, 1024))
     """
     x = x.copy()
     if np.ndim(x) == 1:
         x = x[np.newaxis, ...]
     return np.sqrt(np.median(x**2, axis=axis, keepdims=keepdims))
 
 
-def get_rms(x: np.ndarray, axis=-1, keepdims=False):
+def get_rms(x: np.ndarray, axis=-1, keepdims=False) -> np.ndarray:
     """
     Examples
     --------
     >>> rms = get_rms(np.random.randn(10, 1024))
     """
     x = x.copy()
     if np.ndim(x) == 1:
         x = x[np.newaxis, ...]
     return np.sqrt(np.mean(x**2, axis=axis, keepdims=keepdims))
 
 
-def get_upper_fence(x: np.ndarray, axis=-1, keepdims=False):
+def get_upper_fence(x: np.ndarray, axis=-1, keepdims=False) -> np.ndarray:
     """
     Examples
     --------
     >>> upper_fence = get_upper_fence(np.random.randn(3, 1024))
     >>> upper_fence.shape
     (3,)
     >>> upper_fence = get_upper_fence(np.random.randn(3, 1024), keepdims=True)
@@ -94,28 +94,28 @@
         x = x[np.newaxis, ...]
 
     _q3 = np.quantile(x, axis=axis, q=0.75, keepdims=keepdims)
     _iqr = stats.iqr(x, axis=axis, keepdims=keepdims)
     return _q3 + 1.5 * _iqr
 
 
-def get_zcr(x: np.ndarray, axis=-1, keepdims=False):
+def get_zcr(x: np.ndarray, axis=-1, keepdims=False) -> np.ndarray:
     """
     Examples
     --------
     >>> zcr = get_zcr(np.random.randn(10, 1024))
     """
     x = x.copy()
     if np.ndim(x) == 1:
         x = x[np.newaxis, ...]
     zc = np.abs(np.diff(np.sign(x), axis=axis)).sum(axis, keepdims=keepdims) / 2
     return zc / x.shape[1]
 
 
-name_dict = {
+name_dict: Dict[str, Callable[..., np.ndarray]] = {
     "entropy": stats.entropy,
     "kurtosis": stats.kurtosis,
     "mad": stats.median_abs_deviation,
     "max": np.max,
     "mean": np.mean,
     "median": np.median,
     "ratio_max_upper_fence": get_ratio_max_upper_fence,
@@ -124,15 +124,18 @@
     "skew": stats.skew,
     "std": np.std,
     "upper_fence": get_upper_fence,
     "zcr": get_zcr,
 }
 
 
-def get_feature(x: np.ndarray, names=None) -> pd.DataFrame:
+def get_feature(
+    x: np.ndarray,
+    names: Union[str, List[str], None] = None,
+) -> pd.DataFrame:
     """
     Examples
     --------
     >>> n_samples = 4
     >>> n_size = 1024
     >>> x = np.random.randn(n_samples, n_size)
     >>> feats = get_feature(x)
@@ -172,18 +175,18 @@
 
 
 def get_spectral_feature(
     x: np.ndarray,
     *,
     fs: int,
     freq_intervals: Optional[List[List[int]]] = None,
-    names=None,
-    major_freq=None,
-    ratio_major_orders=None,
-    eps=None,
+    names: Union[str, List[str], None] = None,
+    major_freq: Union[int, None] = None,
+    ratio_major_orders: Optional[List[List[int]]] = None,
+    eps: Union[int, None] = None,
 ) -> pd.DataFrame:
     """
     Get features from spectra.
 
     Examples
     --------
     >>> n_samples = 10
@@ -207,14 +210,15 @@
     ... )
     >>> features.shape
     (10, 4)
     >>> features.columns
     Index(['entropy_50_70', 'entropy_110_130', 'kurtosis_50_70',
            'kurtosis_110_130'],
           dtype='object')
+    >>> features = get_spectral_feature(x=x, fs=fs, major_freq=60, ratio_major_orders=[[1, 3], [2, 3]], eps=10)
     """
     x = x.copy()
     if np.ndim(x) == 1:
         x = x[np.newaxis, ...]
 
     if names is None:
         names = list_all_feature_names()
@@ -224,32 +228,34 @@
 
     if not set(names).issubset(names):
         raise TypeError("Unsupported provided name.")
 
     if freq_intervals is None:
         freq_intervals = [[0, fs // 2]]
 
+    new_column_to_dict = {}
     if major_freq is not None:
         if ratio_major_orders is None:
             raise ValueError("The argument ratio_major_orders should not be None.")
 
         if eps is None:
             raise ValueError("The argument eps should be of integer or of float type.")
 
         if "max" not in names:
             names.append("max")
 
-        seen = set()
+        seen: Set[int] = set()
         for interval in ratio_major_orders:
             for order in interval:
                 if order not in seen:
                     seen.add(order)
                     left = order * major_freq - eps
                     right = order * major_freq + eps
                     freq_intervals.append([left, right])
+                    new_column_to_dict[f"max_{left}_{right}"] = f"max_{order}x"
 
     freq, amps = get_freq_amp(x=x, fs=fs)
 
     feats = []
     for name in names:
         feats_given_name = []
         for interval in freq_intervals:
@@ -261,25 +267,21 @@
             feats_given_name.append(partial_feats.values.ravel())
         feats_given_name = np.array(feats_given_name).T
         feats.append(feats_given_name)
     feats = np.concatenate(feats, axis=1)
 
     columns = [f"{n}_{seg[0]}_{seg[1]}" for n in names for seg in freq_intervals]
     feats = pd.DataFrame(feats, columns=columns)
+    feats = feats.rename(columns=new_column_to_dict)
 
-    if major_freq is not None and ratio_major_orders is not None:
+    if major_freq is not None and ratio_major_orders is not None and eps is not None:
         for order in ratio_major_orders:
             o1, o2 = order
-            left1 = o1 * major_freq - eps
-            right1 = o1 * major_freq + eps
-
-            left2 = o2 * major_freq - eps
-            right2 = o2 * major_freq + eps
-            col1 = f"max_{left1}_{right1}"
-            col2 = f"max_{left2}_{right2}"
+            col1 = f"max_{o1}x"
+            col2 = f"max_{o2}x"
             ratio_col = f"ratio_order_{o1}x_{o2}x"
 
             feats[ratio_col] = feats[col1] / feats[col2]
             columns.append(ratio_col)
 
     assert feats.shape == (x.shape[0], len(columns))
```

### Comparing `aiontutil-0.0.7/PKG-INFO` & `aiontutil-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiontutil
-Version: 0.0.7
+Version: 0.0.8
 Summary: aiont utility package
 Author: jlan
 Author-email: jlan@aiont.io
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

