# Comparing `tmp/ehrapy-0.3.0.tar.gz` & `tmp/ehrapy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehrapy-0.3.0.tar", max compression
+gzip compressed data, was "ehrapy-0.4.0.tar", max compression
```

## Comparing `ehrapy-0.3.0.tar` & `ehrapy-0.4.0.tar`

### file list

```diff
@@ -1,47 +1,45 @@
--rw-r--r--   0        0        0    11310 2022-12-09 08:59:23.706569 ehrapy-0.3.0/LICENSE
--rw-r--r--   0        0        0     2303 2022-12-09 08:59:23.706569 ehrapy-0.3.0/README.md
--rw-r--r--   0        0        0     1539 2022-12-09 08:59:23.738569 ehrapy-0.3.0/ehrapy/SCANPY_LICENSE
--rw-r--r--   0        0        0      668 2022-12-09 08:59:23.738569 ehrapy-0.3.0/ehrapy/__init__.py
--rw-r--r--   0        0        0    15880 2022-12-09 08:59:23.738569 ehrapy-0.3.0/ehrapy/_settings.py
--rw-r--r--   0        0        0      175 2022-12-09 08:59:23.738569 ehrapy-0.3.0/ehrapy/anndata/__init__.py
--rw-r--r--   0        0        0    32064 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/anndata/anndata_ext.py
--rw-r--r--   0        0        0        0 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/core/__init__.py
--rw-r--r--   0        0        0     2192 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/core/meta_information.py
--rw-r--r--   0        0        0     3841 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/core/str_matching.py
--rw-r--r--   0        0        0     1082 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/core/tool_available.py
--rw-r--r--   0        0        0      460 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/data/__init__.py
--rw-r--r--   0        0        0     2274 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/data/_dataloader.py
--rw-r--r--   0        0        0    21476 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/data/_datasets.py
--rw-r--r--   0        0        0       98 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/io/__init__.py
--rw-r--r--   0        0        0    29628 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/io/_read.py
--rw-r--r--   0        0        0      675 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/io/_utility_io.py
--rw-r--r--   0        0        0     3541 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/io/_write.py
--rw-r--r--   0        0        0     6650 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/logging.py
--rw-r--r--   0        0        0      265 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/plot/__init__.py
--rw-r--r--   0        0        0    10483 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/plot/_missingno_pl_api.py
--rw-r--r--   0        0        0     2068 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/plot/_qc.py
--rw-r--r--   0        0        0   102065 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/plot/_scanpy_pl_api.py
--rw-r--r--   0        0        0    10091 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/plot/_survival_analysis.py
--rw-r--r--   0        0        0      795 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/plot/_util.py
--rw-r--r--   0        0        0      855 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/preprocessing/__init__.py
--rw-r--r--   0        0        0    43480 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/preprocessing/_data_imputation.py
--rw-r--r--   0        0        0    46230 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/preprocessing/_encode.py
--rw-r--r--   0        0        0     2863 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/preprocessing/_highly_variable_features.py
--rw-r--r--   0        0        0    15877 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/preprocessing/_normalization.py
--rw-r--r--   0        0        0     3994 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/preprocessing/_outliers.py
--rw-r--r--   0        0        0    15631 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/preprocessing/_quality_control.py
--rw-r--r--   0        0        0    11787 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/preprocessing/_scanpy_pp_api.py
--rw-r--r--   0        0        0    29649 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/preprocessing/laboratory_reference_tables/laposata.tsv
--rw-r--r--   0        0        0        0 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/py.typed
--rw-r--r--   0        0        0      374 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/tools/__init__.py
--rw-r--r--   0        0        0     9808 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/tools/_sa.py
--rw-r--r--   0        0        0    49230 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/tools/_scanpy_tl_api.py
--rw-r--r--   0        0        0        0 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/tools/nlp/__init__.py
--rw-r--r--   0        0        0     3911 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/tools/nlp/_hpo.py
--rw-r--r--   0        0        0    17580 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/tools/nlp/_medcat.py
--rw-r--r--   0        0        0    19792 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/tools/nlp/_translators.py
--rw-r--r--   0        0        0        0 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/util/__init__.py
--rw-r--r--   0        0        0    14707 2022-12-09 08:59:23.742569 ehrapy-0.3.0/ehrapy/util/_doc_util.py
--rw-r--r--   0        0        0     3544 2022-12-09 08:59:23.746569 ehrapy-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4068 1970-01-01 00:00:00.000000 ehrapy-0.3.0/setup.py
--rw-r--r--   0        0        0     4373 1970-01-01 00:00:00.000000 ehrapy-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11310 2023-06-06 12:43:14.081286 ehrapy-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2316 2023-06-06 12:43:14.081286 ehrapy-0.4.0/README.md
+-rw-r--r--   0        0        0     1539 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/SCANPY_LICENSE
+-rw-r--r--   0        0        0      668 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/__init__.py
+-rw-r--r--   0        0        0    15880 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/_settings.py
+-rw-r--r--   0        0        0      259 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/anndata/__init__.py
+-rw-r--r--   0        0        0    35753 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/anndata/anndata_ext.py
+-rw-r--r--   0        0        0        0 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/core/__init__.py
+-rw-r--r--   0        0        0     1091 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/core/_tool_available.py
+-rw-r--r--   0        0        0     2271 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/core/meta_information.py
+-rw-r--r--   0        0        0      509 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/data/__init__.py
+-rw-r--r--   0        0        0     2283 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/data/_dataloader.py
+-rw-r--r--   0        0        0    22780 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/data/_datasets.py
+-rw-r--r--   0        0        0      109 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/io/__init__.py
+-rw-r--r--   0        0        0    33563 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/io/_read.py
+-rw-r--r--   0        0        0      676 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/io/_utility_io.py
+-rw-r--r--   0        0        0     3192 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/io/_write.py
+-rw-r--r--   0        0        0     6614 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/logging.py
+-rw-r--r--   0        0        0      265 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/plot/__init__.py
+-rw-r--r--   0        0        0    10390 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/plot/_missingno_pl_api.py
+-rw-r--r--   0        0        0     2191 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/plot/_qc.py
+-rw-r--r--   0        0        0   101572 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/plot/_scanpy_pl_api.py
+-rw-r--r--   0        0        0    10214 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/plot/_survival_analysis.py
+-rw-r--r--   0        0        0      795 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/plot/_util.py
+-rw-r--r--   0        0        0      855 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/preprocessing/__init__.py
+-rw-r--r--   0        0        0    47405 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/preprocessing/_data_imputation.py
+-rw-r--r--   0        0        0    46268 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/preprocessing/_encode.py
+-rw-r--r--   0        0        0     2825 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/preprocessing/_highly_variable_features.py
+-rw-r--r--   0        0        0    16013 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/preprocessing/_normalization.py
+-rw-r--r--   0        0        0     4299 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/preprocessing/_outliers.py
+-rw-r--r--   0        0        0    17121 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/preprocessing/_quality_control.py
+-rw-r--r--   0        0        0    11810 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/preprocessing/_scanpy_pp_api.py
+-rw-r--r--   0        0        0    29649 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/preprocessing/laboratory_reference_tables/laposata.tsv
+-rw-r--r--   0        0        0        0 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/py.typed
+-rw-r--r--   0        0        0      437 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/tools/__init__.py
+-rw-r--r--   0        0        0    11546 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/tools/_sa.py
+-rw-r--r--   0        0        0    49254 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/tools/_scanpy_tl_api.py
+-rw-r--r--   0        0        0        0 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/tools/nlp/__init__.py
+-rw-r--r--   0        0        0     3911 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/tools/nlp/_hpo.py
+-rw-r--r--   0        0        0    17561 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/tools/nlp/_medcat.py
+-rw-r--r--   0        0        0    19793 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/tools/nlp/_translators.py
+-rw-r--r--   0        0        0        0 2023-06-06 12:43:14.121285 ehrapy-0.4.0/ehrapy/util/__init__.py
+-rw-r--r--   0        0        0    14707 2023-06-06 12:43:14.121285 ehrapy-0.4.0/ehrapy/util/_doc_util.py
+-rw-r--r--   0        0        0     3791 2023-06-06 12:43:14.121285 ehrapy-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4214 1970-01-01 00:00:00.000000 ehrapy-0.4.0/PKG-INFO
```

### Comparing `ehrapy-0.3.0/LICENSE` & `ehrapy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ehrapy-0.3.0/README.md` & `ehrapy-0.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 [![Test](https://github.com/theislab/ehrapy/workflows/Run%20ehrapy%20Tests/badge.svg)](https://github.com/theislab/ehrapy/actions?workflow=Tests)
 [![PyPI](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 <img src="https://user-images.githubusercontent.com/21954664/156930990-0d668468-0cd9-496e-995a-96d2c2407cf5.png" alt="ehrapy logo">
 
 # ehrapy overview
 
-<img src="https://user-images.githubusercontent.com/21954664/183865403-a2d61033-413e-4ae8-82cd-a9b6daa4fc18.png" alt="ehrapy overview">
+<img src="https://user-images.githubusercontent.com/99650244/217562449-e05ab1dd-9c04-44fc-a042-b993dd9d4eea.png" alt="ehrapy overview">
 
 ## Features
 
--   Exploratory analysis of Electronic Health Records
+-   Exploratory and targeted analysis of Electronic Health Records
 -   Quality control & preprocessing
--   Clustering & trajectory inference
 -   Visualization & Exploration
+-   Clustering & trajectory inference
 
 ## Installation
 
 You can install _ehrapy_ via [pip] from [PyPI]:
 
 ```console
 $ pip install ehrapy
```

### Comparing `ehrapy-0.3.0/ehrapy/SCANPY_LICENSE` & `ehrapy-0.4.0/ehrapy/SCANPY_LICENSE`

 * *Files identical despite different names*

### Comparing `ehrapy-0.3.0/ehrapy/__init__.py` & `ehrapy-0.4.0/ehrapy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for ehrapy."""
 
 __author__ = "Lukas Heumos"
 __email__ = "lukas.heumos@posteo.net"
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 
 from pypi_latest import PypiLatest
 from rich import traceback
 
 ehrapy_pypi_latest = PypiLatest("ehrapy", __version__)
 ehrapy_pypi_latest.check_latest()
```

### Comparing `ehrapy-0.3.0/ehrapy/_settings.py` & `ehrapy-0.4.0/ehrapy/_settings.py`

 * *Files identical despite different names*

### Comparing `ehrapy-0.3.0/ehrapy/anndata/anndata_ext.py` & `ehrapy-0.4.0/ehrapy/anndata/anndata_ext.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import annotations
 
 import random
 from collections import OrderedDict
 from string import ascii_letters
-from typing import Collection, NamedTuple
+from typing import Collection, Iterable, NamedTuple
 
 import numpy as np
 import pandas as pd
 from anndata import AnnData, concat
 from mudata import MuData
 from rich import print
 from rich.text import Text
 from rich.tree import Tree
+from scanpy.get import obs_df, rank_genes_groups_df, var_df
 from scipy import sparse
 from scipy.sparse import issparse
 
 from ehrapy import logging as logg
 
 
 class BaseDataframes(NamedTuple):
@@ -34,14 +35,26 @@
     Args:
         df: The pandas dataframe to be transformed
         columns_obs_only: An optional list of column names that should belong to obs only and not X
         index_column: The index column of obs. This can be either a column name (or its numerical index in the dataframe) or the index of the dataframe
 
     Returns:
         An AnnData object created from the given pandas dataframe
+
+    Examples:
+        >>> import ehrapy as ep
+        >>> import pandas as pd
+        >>> df = pd.DataFrame(
+        ...     {
+        ...         "patient_id": ["0", "1", "2", "3", "4"],
+        ...         "age": [65, 72, 58, 78, 82],
+        ...         "sex": ["M", "F", "F", "M", "F"],
+        ...     }
+        ... )
+        >>> adata = ep.df_to_anndata(df, index_column="patient_id")
     """
     # allow index 0
     if index_column is not None:
         df_columns = list(df.columns)
         # if the index of the dataframe is the index_column leave it as it is
         if index_column == df.index.name:
             pass
@@ -49,21 +62,34 @@
         elif isinstance(index_column, int) or index_column != df.index.name:
             if isinstance(index_column, str) and index_column in df_columns:
                 df = df.set_index(index_column)
             # also ensure that the index is in range
             elif isinstance(index_column, int) and index_column < len(df_columns):
                 df = df.set_index(df_columns[index_column])
             else:
-                raise IndexNotFoundError(f"Did not find column {index_column} in neither index or columns!")
+                raise ValueError(f"Did not find column {index_column} in neither index or columns!")
         # index_column is neither in the index or in the columns or passed as some value that could not be understood
-        else:
-            raise IndexNotFoundError(f"Did not find column {index_column} in neither index or columns!")
+        else:  # pragma: no cover
+            raise ValueError(f"Did not find column {index_column} in neither index or columns!")
 
-    # move columns from the input dataframe to later obs
-    dataframes = _move_columns_to_obs(df, columns_obs_only)
+    # move columns from the input dataframe to obs
+    if columns_obs_only:
+        try:
+            obs = df[columns_obs_only].copy()
+            obs = obs.set_index(df.index.map(str))
+            df = df.drop(columns_obs_only, axis=1)
+        except KeyError as e:
+            raise ValueError(
+                "One or more column names passed to column_obs_only were not found in the input data. "
+                "Are the column names spelled correctly?"
+            ) from e
+    else:
+        obs = pd.DataFrame(index=df.index.map(str))
+        logg.info("Added all columns to `obs`.")
+    dataframes = BaseDataframes(obs, df)
     numerical_columns = list(dataframes.df.select_dtypes("number").columns)
     # if data is numerical only, short-circuit AnnData creation to have float dtype instead of object
     all_num = True if len(numerical_columns) == len(list(dataframes.df.columns)) else False
     X = dataframes.df.to_numpy(copy=True)
 
     # initializing an OrderedDict with a non-empty dict might not be intended,
     # see: https://stackoverflow.com/questions/25480089/right-way-to-initialize-an-ordereddict-using-its-constructor-such-that-it-retain/25480206
@@ -86,80 +112,55 @@
     logg.info(
         f"Transformed passed dataframe into an AnnData object with n_obs x n_vars = `{adata.n_obs}` x `{adata.n_vars}`."
     )
 
     return adata
 
 
-def _move_columns_to_obs(df: pd.DataFrame, columns_obs_only: list[str] | None) -> BaseDataframes:
-    """Move the given columns from the original dataframe (and therefore X) to obs.
-
-    By moving these values will not get lost and will be stored in obs, but will not appear in X.
-    This may be useful for textual values like free text.
-
-    Args:
-        df: Pandas Dataframe to move the columns for
-        columns_obs_only: Columns to move to obs only
-
-    Returns:
-        A modified :class:`~pd.DataFrame` object
-    """
-    if columns_obs_only:
-        try:
-            obs = df[columns_obs_only].copy()
-            obs = obs.set_index(df.index.map(str))
-            df = df.drop(columns_obs_only, axis=1)
-        except KeyError as e:
-            raise ColumnNotFoundError(
-                "One or more column names passed to column_obs_only were not found in the input data. "
-                "Are the column names spelled correctly?"
-            ) from e
-    else:
-        obs = pd.DataFrame(index=df.index.map(str))
-        logg.info("Added all columns to `obs`.")
-
-    return BaseDataframes(obs, df)
-
-
 def anndata_to_df(
     adata: AnnData, layer: str = None, obs_cols: list[str] | str | None = None, var_cols: list[str] | str | None = None
 ) -> pd.DataFrame:
     """Transform an AnnData object to a pandas dataframe.
 
     Args:
         adata: The AnnData object to be transformed into a pandas Dataframe
         layer: The layer to use for X.
         obs_cols: List of obs columns to add to X.
         var_cols: List of var columns to add to X.
 
     Returns:
         The AnnData object as a pandas Dataframe
+
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.mimic_2(encoded=True)
+        >>> df = ep.ad.anndata_to_df(adata)
     """
     if layer is not None:
         X = adata.layers[layer]
     else:
         X = adata.X
-    if issparse(X):
+    if issparse(X):  # pragma: no cover
         X = X.toarray()
 
     df = pd.DataFrame(X, columns=list(adata.var_names))
     if obs_cols:
         if len(adata.obs.columns) == 0:
-            raise ObsEmptyError("Cannot slice columns from empty obs!")
+            raise ValueError("Cannot slice columns from empty obs!")
         if isinstance(obs_cols, str):
             obs_cols = list(obs_cols)
-        if isinstance(obs_cols, list):
+        if isinstance(obs_cols, list):  # pragma: no cover
             obs_slice = adata.obs[obs_cols]
         # reset index needed since we slice all or at least some columns from obs DataFrame
         obs_slice = obs_slice.reset_index(drop=True)
         df = pd.concat([df, obs_slice], axis=1)
         logg.info(f"Added `{obs_cols}` columns to `X`.")
     if var_cols:
         if len(adata.var.columns) == 0:
-            raise VarEmptyError("Cannot slice columns from empty var!")
+            raise ValueError("Cannot slice columns from empty var!")
         if isinstance(var_cols, str):
             var_cols = list(var_cols)
         if isinstance(var_cols, list):
             var_slice = adata.var[var_cols]
         # reset index needed since we slice all or at least some columns from var DataFrame
         var_slice = var_slice.reset_index(drop=True)
         df = pd.concat([df, var_slice], axis=1)
@@ -177,22 +178,26 @@
     Args:
         adata: The AnnData object
         to_obs: The columns to move to obs
         copy_obs: The values are copied to obs (and therefore kept in X) instead of moved completely
 
     Returns:
         The original AnnData object with moved or copied columns from X to obs
-    """
 
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.mimic_2(encoded=True)
+        >>> ep.ad.move_to_obs(adata, ['age'], copy_obs=False)
+    """
     if isinstance(to_obs, str):  # pragma: no cover
         to_obs = [to_obs]
 
     # don't allow moving encoded columns as this could lead to inconsistent data in X and obs
     if any(column.startswith("ehrapycat") for column in to_obs):
-        raise ObsMoveError(
+        raise ValueError(
             "Cannot move encoded columns from X to obs. Either undo encoding or remove them from the list!"
         )
 
     if not all(elem in adata.var_names.values for elem in to_obs):
         raise ValueError(
             f"Columns `{[col for col in to_obs if col not in adata.var_names.values]}` are not in var_names."
         )
@@ -233,16 +238,21 @@
 
     Args:
         adata: The AnnData object
         to_delete: The columns to delete from obs
 
     Returns:
         The original AnnData object with deleted columns from obs.
-    """
 
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.mimic_2(encoded=True)
+        >>> ep.ad.move_to_obs(adata, ['age'], copy_obs=True)
+        >>> ep.ad.delete_from_obs(adata, ['age'])
+    """
     if isinstance(to_delete, str):  # pragma: no cover
         to_delete = [to_delete]
 
     if not all(elem in adata.obs.columns.values for elem in to_delete):
         raise ValueError(
             f"Columns `{[col for col in to_delete if col not in adata.obs.columns.values]}` are not in obs."
         )
@@ -250,32 +260,37 @@
     adata.obs = adata.obs[adata.obs.columns[~adata.obs.columns.isin(to_delete)]]
 
     logg.info(f"Removed `{to_delete}` from `obs`.")
 
     return adata
 
 
-def move_to_x(adata: AnnData, to_x: list[str] | str, copy: bool = False) -> AnnData:
+def move_to_x(adata: AnnData, to_x: list[str] | str) -> AnnData:
     """Move features from obs to X inplace.
 
     Args:
         adata: The AnnData object
         to_x: The columns to move to X
         copy: Whether to return a copy or not
 
     Returns:
         A new AnnData object with moved columns from obs to X. This should not be used for datetime columns currently.
+
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.mimic_2(encoded=True)
+        >>> ep.ad.move_to_obs(adata, ['age'], copy_obs=False)
+        >>> new_adata = ep.ad.move_to_x(adata, ['age'])
     """
+    if isinstance(to_x, str):  # pragma: no cover
+        to_x = [to_x]
 
     if not all(elem in adata.obs.columns.values for elem in to_x):
         raise ValueError(f"Columns `{[col for col in to_x if col not in adata.obs.columns.values]}` are not in obs.")
 
-    if isinstance(to_x, str):  # pragma: no cover
-        to_x = [to_x]
-
     cols_present_in_x = []
     cols_not_in_x = []
 
     for col in to_x:
         if col in set(adata.var_names):
             cols_present_in_x.append(col)
         else:
@@ -307,27 +322,32 @@
 
     Args:
         adata: :class:`~anndata.AnnData` object
         col_names: Column names to extract the indices for
 
     Returns:
         Set of column indices
+
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.mimic_2(encoded=True)
+        >>> ep.ad.get_column_indices(adata, ['age', 'gender_num', 'bmi'])
     """
     if isinstance(col_names, str):  # pragma: no cover
         col_names = [col_names]
 
     indices = list()
     for idx, col in enumerate(adata.var_names):
         if col in col_names:
             indices.append(idx)
 
     return indices
 
 
-def get_column_values(adata: AnnData, indices: int | list[int]) -> np.ndarray:
+def _get_column_values(adata: AnnData, indices: int | list[int]) -> np.ndarray:
     """Fetches the column values for a specific index from X
 
     Args:
         adata: :class:`~anndata.AnnData` object
         indices: The index to extract the values for
 
     Returns:
@@ -343,33 +363,28 @@
 
     Output could be printed in sorted format by using one of `dtype`, `order`, `num_cats` or `None`, which sorts by data type, lexicographical order,
     number of unique values (excluding NaN's) and unsorted respectively. Note that sorting by `num_cats` only affects
     encoded variables currently and will display unencoded vars unsorted.
 
     Args:
         data: :class:`~anndata.AnnData` or :class:`~mudata.MuData` object to display
-        sort_by: How the tree output should be sorted. One of `dtype`, `order`, `num_cats` or None (defaults to None -> unsorted)
+        sort_by: How the tree output should be sorted. One of `dtype`, `order`, `num_cats` or None (Defaults to None -> unsorted)
         sort_reversed: Whether to sort in reversed order or not
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.dt.mimic_2(encode=True)
-            ep.anndata_ext.type_overview(adata)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.mimic_2(encoded=True)
+        >>> ep.ad.type_overview(adata)
     """
     if isinstance(data, AnnData):
         _adata_type_overview(data, sort_by, sort_reversed)
     elif isinstance(data, MuData):
         _mudata_type_overview(data, sort_by, sort_reversed)
     else:
-        raise EhrapyRepresentationError(
-            f"Unable to present object of type {type(data)}. Can only display AnnData or MuData objects!"
-        )
+        raise ValueError(f"Unable to present object of type {type(data)}. Can only display AnnData or MuData objects!")
 
 
 def _adata_type_overview(
     adata: AnnData, sort_by: str | None = None, sort_reversed: bool = False
 ) -> None:  # pragma: no cover
     """Display the :class:`~anndata.AnnData object in its current state (encoded and unencoded variables, obs)
 
@@ -571,15 +586,15 @@
         adata = adata.copy()
 
     vars_idx = get_column_indices(adata, vars)
 
     for i in range(n_values):
         adata.X[:, vars_idx[i]] = values[:, i]
 
-    logg.info(f"Column names for numeric variables {vars} were replaced.")
+    logg.info(f"Column names for numeric variables {vars} were replaced by {values}.")
 
     return adata
 
 
 def _update_uns(
     adata: AnnData, moved_columns: list[str], to_x: bool = False
 ) -> tuple[list[str], list[str], list[str] | None]:
@@ -591,15 +606,14 @@
     Args:
         adata: class:`~anndata.AnnData` object
         moved_columns: List of column names to be moved
         to_x: Whether to move from `obs` to `X` or vice versa
 
     Returns:
         :class:`~anndata.AnnData` object with updated .uns
-
     """
     moved_columns_set = set(moved_columns)
     if not to_x:  # moving from `X` to `obs`, delete it from the corresponding entry in `uns`.
         num_set = set(adata.uns["numerical_columns"].copy())
         non_num_set = set(adata.uns["non_numerical_columns"].copy())
         var_num = []
         for var in moved_columns_set:
@@ -653,15 +667,15 @@
         if not set(pd.unique(obs_name)).issubset({False, True, np.NaN})
         else obs_name.astype("bool"),
         axis=0,
     )
     return obs
 
 
-def generate_anndata(
+def generate_anndata(  # pragma: no cover
     shape: tuple[int, int],
     X_type=sparse.csr_matrix,
     X_dtype=np.float32,
     obsm_types: Collection = (sparse.csr_matrix, np.ndarray, pd.DataFrame),
     varm_types: Collection = (sparse.csr_matrix, np.ndarray, pd.DataFrame),
     layers_types: Collection = (sparse.csr_matrix, np.ndarray, pd.DataFrame),
     include_nlp: bool = False,
@@ -677,20 +691,17 @@
         layers_types: Types of additional layers.
         include_nlp: Whether to include diseases for NLP in all of X, obs and var.
                      Sets the X_dtype to object by default and overwrites the passed X_dtype.
 
     Returns:
         A specified AnnData object.
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.ad.generate_anndata((2, 2), include_nlp=True)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.ad.generate_anndata((2, 2), include_nlp=True)
     """
     example_diseases: list[str] = ["diabetes melitus", "breast cancer", "dementia", "pneumonia"]
 
     M, N = shape
     obs_names = pd.Index(f"patient{i}" for i in range(shape[0]))
     var_names = pd.Index(f"feature{i}" for i in range(shape[1]))
 
@@ -793,33 +804,106 @@
     )
 
     logg.info(f"Generated an AnnData object with n_obs x n_vars = `{adata.n_obs}` x `{adata.n_vars}`.")
 
     return adata
 
 
-class NotEncodedError(AssertionError):
-    pass
-
-
-class ColumnNotFoundError(Exception):
-    pass
-
-
-class IndexNotFoundError(Exception):
-    pass
-
-
-class ObsEmptyError(Exception):
-    pass
-
-
-class VarEmptyError(Exception):
-    pass
-
-
-class ObsMoveError(Exception):
-    pass
+def get_obs_df(  # pragma: no cover
+    adata: AnnData,
+    keys: Iterable[str] = (),
+    obsm_keys: Iterable[tuple[str, int]] = (),
+    *,
+    layer: str = None,
+    features: str = None,
+):
+    """Return values for observations in adata.
+
+    Args:
+        adata: AnnData object to get values from.
+        keys: Keys from either `.var_names`, `.var[gene_symbols]`, or `.obs.columns`.
+        obsm_keys: Tuple of `(key from obsm, column index of obsm[key])`.
+        layer: Layer of `adata`.
+        features: Column of `adata.var` to search for `keys` in.
+
+    Returns:
+        A dataframe with `adata.obs_names` as index, and values specified by `keys` and `obsm_keys`.
+
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.mimic_2(encoded=True)
+        >>> ages = ep.ad.get_obs_df(adata, keys = ['age'])
+    """
+    return obs_df(adata=adata, keys=keys, obsm_keys=obsm_keys, layer=layer, gene_symbols=features)
+
+
+def get_var_df(  # pragma: no cover
+    adata: AnnData,
+    keys: Iterable[str] = (),
+    varm_keys: Iterable[tuple[str, int]] = (),
+    *,
+    layer: str = None,
+):
+    """Return values for observations in adata.
+
+    Args:
+        adata: AnnData object to get values from.
+        keys: Keys from either `.obs_names`, or `.var.columns`.
+        varm_keys: Tuple of `(key from varm, column index of varm[key])`.
+        layer: Layer of `adata`.
+
+    Returns:
+        A dataframe with `adata.var_names` as index, and values specified by `keys` and `varm_keys`.
+
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.mimic_2(encoded=True)
+        >>> four_patients = ep.ad.get_var_df(adata, keys = ['0', '1', '2', '3'])
+    """
+    return var_df(adata=adata, keys=keys, varm_keys=varm_keys, layer=layer)
+
+
+def get_rank_features_df(
+    adata: AnnData,
+    group: str | Iterable[str],
+    *,
+    key: str = "rank_features_groups",
+    pval_cutoff: float | None = None,
+    log2fc_min: float | None = None,
+    log2fc_max: float | None = None,
+    features: str | None = None,
+):
+    """:func:`ehrapy.tl.rank_features_groups` results in the form of a :class:`~pandas.DataFrame`.
+
+    Args:
+        adata: AnnData object to get values from.
+        group: Which group (as in :func:`ehrapy.tl.rank_genes_groups`'s `groupby` argument)
+               to return results from. Can be a list. All groups are returned if groups is `None`.
+        key: Key differential groups were stored under.
+        pval_cutoff: Return only adjusted p-values below the  cutoff.
+        log2fc_min: Minimum logfc to return.
+        log2fc_max: Maximum logfc to return.
+        features: Column name in `.var` DataFrame that stores gene symbols.
+                  Specifying this will add that column to the returned DataFrame.
+
+    Returns:
+        A Pandas DataFrame of all rank genes groups results.
+
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.mimic_2(encoded=True)
+        >>> ep.tl.rank_features_groups(adata, "service_unit")
+        >>> df = ep.ad.get_rank_features_df(adata, group="FICU")
+    """
+    return rank_genes_groups_df(
+        adata=adata,
+        group=group,
+        key=key,
+        pval_cutoff=pval_cutoff,
+        log2fc_min=log2fc_min,
+        log2fc_max=log2fc_max,
+        gene_symbols=features,
+    )
 
 
-class EhrapyRepresentationError(ValueError):
+class NotEncodedError(AssertionError):
     pass
```

### Comparing `ehrapy-0.3.0/ehrapy/core/meta_information.py` & `ehrapy-0.4.0/ehrapy/core/meta_information.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 
 
 def print_versions(*, output_file=None) -> None:  # pragma: no cover
     """Print print versions of imported packages.
 
     Args:
         output_file: Path to output file
+
+    Examples:
+        >>> import ehrapy as ep
+        >>> ep.print_versions()
     """
     stdout = sys.stdout
     try:
         buf = sys.stdout = StringIO()
         session_info.show(
             dependencies=True,
             excludes=[
```

### Comparing `ehrapy-0.3.0/ehrapy/core/tool_available.py` & `ehrapy-0.4.0/ehrapy/core/_tool_available.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from __future__ import annotations
 
-import importlib
+import importlib.util
 from subprocess import PIPE, Popen
 
 
-def check_module_importable(package: str) -> bool:  # pragma: no cover
+def _check_module_importable(package: str) -> bool:  # pragma: no cover
     """Checks whether a module is installed and can be loaded.
 
     Args:
         package: The package to check.
 
     Returns:
-        True if the package is installed, false elsewise
+        True if the package is installed, False otherweise
     """
     module_information = importlib.util.find_spec(package)
     module_available = module_information is not None
 
     return module_available
 
 
-def shell_command_accessible(command: list[str]) -> bool:  # pragma: no cover
+def _shell_command_accessible(command: list[str]) -> bool:  # pragma: no cover
     """Checks whether the provided command is accessible in the current shell.
 
     Args:
         command: The command to check. Spaces are separated as list elements.
 
     Returns:
-        True if the command is accessible, false otherwise.
+        True if the command is accessible, False otherwise.
     """
     command_accessible = Popen(command, stdout=PIPE, stderr=PIPE, universal_newlines=True, shell=True)
     (commmand_stdout, command_stderr) = command_accessible.communicate()
     if command_accessible.returncode != 0:
         return False
 
     return True
```

### Comparing `ehrapy-0.3.0/ehrapy/data/_dataloader.py` & `ehrapy-0.4.0/ehrapy/data/_dataloader.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,18 +22,18 @@
     is_archived: bool = False,
 ) -> None:  # pragma: no cover
     """Downloads a dataset irrespective of the format.
 
     Args:
         url: URL to download
         output_file_name: Name of the downloaded file
-        output_path: Path to download/extract the files to (default: OS tmpdir)
-        block_size: Block size for downloads in bytes (default: 1024)
-        overwrite: Whether to overwrite existing files (default: False)
-        is_archived: Whether the downloaded file needs to be unarchived (default: False)
+        output_path: Path to download/extract the files to. Defaults to 'OS tmpdir'
+        block_size: Block size for downloads in bytes.Defaults to 1024
+        overwrite: Whether to overwrite existing files. Defaults to False
+        is_archived: Whether the downloaded file needs to be unarchived. Defaults to False
     """
     if output_file_name is None:
         letters = ascii_lowercase
         output_file_name = f"ehrapy_tmp_{''.join(choice(letters) for _ in range(10))}"
 
     if output_path is None:
         output_path = tempfile.gettempdir()
```

### Comparing `ehrapy-0.3.0/ehrapy/data/_datasets.py` & `ehrapy-0.4.0/ehrapy/data/_datasets.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import pandas as pd
 from anndata import AnnData
 
 from ehrapy import ehrapy_settings
-from ehrapy.io._read import read_csv
+from ehrapy.io._read import read_csv, read_fhir, read_h5ad
 from ehrapy.preprocessing._encode import encode
 
 
 def mimic_2(
     encoded: bool = False,
     columns_obs_only: dict[str, list[str]] | list[str] | None = None,
 ) -> AnnData:
@@ -19,58 +19,75 @@
     Args:
         encoded: Whether to return an already encoded object
         columns_obs_only: Columns to include in obs only and not X.
 
     Returns:
         :class:`~anndata.AnnData` object of the MIMIC-II dataset
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.dt.mimic_2(encoded=True)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.mimic_2(encoded=True)
     """
     adata = read_csv(
         dataset_path=f"{ehrapy_settings.datasetdir}/ehrapy_mimic2.csv",
         download_dataset_name="ehrapy_mimic2.csv",
         backup_url="https://www.physionet.org/files/mimic2-iaccd/1.0/full_cohort_data.csv?download",
         columns_obs_only=columns_obs_only,
     )
     if encoded:
         return encode(adata, autodetect=True)
 
     return adata
 
 
+def mimic_2_preprocessed() -> AnnData:
+    """Loads the preprocessed MIMIC-II dataset.
+
+    More details: https://physionet.org/content/mimic2-iaccd/1.0/
+    The dataset was preprocessed according to: https://github.com/theislab/ehrapy-datasets/tree/main/mimic_2
+
+    Returns:
+        :class:`~anndata.AnnData` object of the prprocessed MIMIC-II dataset
+
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.mimic_2_preprocessed()
+    """
+    adata = read_h5ad(
+        dataset_path=f"{ehrapy_settings.datasetdir}/ehrapy_mimic2.csv",
+        download_dataset_name="ehrapy_mimic_2_preprocessed.h5ad",
+        backup_url="https://figshare.com/ndownloader/files/39727936",
+    )
+
+    return adata
+
+
 def mimic_3_demo(
     encoded: bool = False,
     anndata: bool = False,
     columns_obs_only: dict[str, list[str]] | list[str] | None = None,
 ) -> dict[str, AnnData] | dict[str, pd.DataFrame]:
     """Loads the MIMIC-III demo dataset as a dictionary of Pandas DataFrames.
 
     The MIMIC-III dataset comes in the form of 26 CSV tables. Although, it is possible to return one AnnData object per
     csv table, it might be easier to start with Pandas DataFrames to aggregate the desired measurements with Pandas SQL.
     https://github.com/yhat/pandasql/ might be useful.
     The resulting DataFrame can then be transformed into an AnnData object with :func:`~ehrapy.anndata.df_to_anndata`.
 
     Args:
-        encoded: Whether to return an already encoded object
-        anndata: Whether to return one AnnData object per CSV file (default: False)
+        encoded: Whether to return an already encoded object.
+        anndata: Whether to return one AnnData object per CSV file. Defaults to False
+        columns_obs_only: Columns to include in obs only and not X.
 
     Returns:
         A dictionary of AnnData objects or a dictionary of Pandas DataFrames
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            dfs = ep.dt.mimic_3_demo()
+    Examples:
+        >>> import ehrapy as ep
+        >>> dfs = ep.dt.mimic_3_demo()
     """
     data = read_csv(
         dataset_path=f"{ehrapy_settings.datasetdir}/ehrapy_mimic_3",
         download_dataset_name="ehrapy_mimic_3",
         backup_url="https://physionet.org/static/published-projects/mimiciii-demo/mimic-iii-clinical-database-demo-1.4.zip",
         return_mudata=False,
         return_dfs=False if anndata else True,
@@ -94,20 +111,17 @@
     Args:
         encoded: Whether to return an already encoded object
         columns_obs_only: Columns to include in obs only and not X.
 
     Returns:
         :class:`~anndata.AnnData` object of the MIMIC-II dataset
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.dt.heart_failure(encoded=True)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.heart_failure(encoded=True)
     """
     adata = read_csv(
         dataset_path=f"{ehrapy_settings.datasetdir}/heart_failure.csv",
         download_dataset_name="heart_failure.csv",
         backup_url="https://figshare.com/ndownloader/files/33952934",
         columns_obs_only=columns_obs_only,
         index_column="patient_id",
@@ -130,20 +144,17 @@
     Args:
         encoded: Whether to return an already encoded object
         columns_obs_only: Columns to include in obs only and not X.
 
     Returns:
         :class:`~anndata.AnnData` object of the Diabetes 130 dataset
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.dt.diabetes_130(encoded=True)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.diabetes_130(encoded=True)
     """
     adata = read_csv(
         dataset_path=f"{ehrapy_settings.datasetdir}/diabetes_130.csv",
         download_dataset_name="diabetes_130.csv",
         backup_url="https://figshare.com/ndownloader/files/33950546",
         columns_obs_only=columns_obs_only,
         index_column="encounter_id",
@@ -166,20 +177,17 @@
     Args:
         encoded: Whether to return an already encoded object
         columns_obs_only: Columns to include in obs only and not X.
 
     Returns:
         :class:`~anndata.AnnData` object of the Chronic Kidney Disease dataset
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.data.chronic_kidney_disease(encoded=True)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.chronic_kidney_disease(encoded=True)
     """
     adata = read_csv(
         dataset_path=f"{ehrapy_settings.datasetdir}/chronic_kidney_disease_precessed.csv",
         download_dataset_name="chronic_kidney_disease.csv",
         backup_url="https://figshare.com/ndownloader/files/33989261",
         columns_obs_only=columns_obs_only,
         index_column="Patient_id",
@@ -202,20 +210,17 @@
     Args:
         encoded: Whether to return an already encoded object
         columns_obs_only: Columns to include in obs only and not X.
 
     Returns:
         :class:`~anndata.AnnData` object of the Breast Tissue Data Set
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.dt.breast_tissue(encoded=True)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.breast_tissue(encoded=True)
     """
     adata = read_csv(
         dataset_path=f"{ehrapy_settings.datasetdir}/breast_tissue.csv",
         download_dataset_name="breast_tissue.csv",
         backup_url="https://figshare.com/ndownloader/files/34179264",
         columns_obs_only=columns_obs_only,
         index_column="patient_id",
@@ -238,20 +243,17 @@
     Args:
         encoded: Whether to return an already encoded object
         columns_obs_only: Columns to include in obs only and not X.
 
     Returns:
         :class:`~anndata.AnnData` object of the Cervical cancer (Risk Factors) Data Set
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.dt.cervical_cancer_risk_factors(encoded=True)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.cervical_cancer_risk_factors(encoded=True)
     """
     adata = read_csv(
         dataset_path=f"{ehrapy_settings.datasetdir}/cervical_cancer_risk_factors.csv",
         download_dataset_name="cervical_cancer_risk_factors.csv",
         backup_url="https://figshare.com/ndownloader/files/34179291",
         columns_obs_only=columns_obs_only,
         index_column="patient_id",
@@ -274,20 +276,17 @@
     Args:
         encoded: Whether to return an already encoded object
         columns_obs_only: Columns to include in obs only and not X.
 
     Returns:
         :class:`~anndata.AnnData` object of the Dermatology Data Set
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.dt.dermatology(encoded=True)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.dermatology(encoded=True)
     """
     adata = read_csv(
         dataset_path=f"{ehrapy_settings.datasetdir}/dermatology.csv",
         download_dataset_name="dermatology.csv",
         backup_url="https://figshare.com/ndownloader/files/34179300",
         columns_obs_only=columns_obs_only,
         index_column="patient_id",
@@ -310,20 +309,17 @@
     Args:
         encoded: Whether to return an already encoded object
         columns_obs_only: Columns to include in obs only and not X.
 
     Returns:
         :class:`~anndata.AnnData` object of the Echocardiogram Data Set
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.dt.echocardiogram(encoded=True)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.echocardiogram(encoded=True)
     """
     adata = read_csv(
         dataset_path=f"{ehrapy_settings.datasetdir}/echocardiogram.csv",
         download_dataset_name="echocardiogram.csv",
         backup_url="https://figshare.com/ndownloader/files/34179306",
         columns_obs_only=columns_obs_only,
         index_column="patient_id",
@@ -346,20 +342,17 @@
     Args:
         encoded: Whether to return an already encoded object
         columns_obs_only: Columns to include in obs only and not X.
 
     Returns:
         :class:`~anndata.AnnData` object of the Hepatitis Data Set
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.dt.hepatitis(encoded=True)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.hepatitis(encoded=True)
     """
     adata = read_csv(
         dataset_path=f"{ehrapy_settings.datasetdir}/hepatitis.csv",
         download_dataset_name="hepatitis.csv",
         backup_url="https://figshare.com/ndownloader/files/34179318",
         columns_obs_only=columns_obs_only,
         index_column="patient_id",
@@ -382,20 +375,17 @@
     Args:
         encoded: Whether to return an already encoded object
         columns_obs_only: Columns to include in obs only and not X.
 
     Returns:
         :class:`~anndata.AnnData` object of the Statlog (Heart) Data Set
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.dt.statlog_heart(encoded=True)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.statlog_heart(encoded=True)
     """
     adata = read_csv(
         dataset_path=f"{ehrapy_settings.datasetdir}/statlog_heart.csv",
         download_dataset_name="statlog_heart.csv",
         backup_url="https://figshare.com/ndownloader/files/34179327",
         columns_obs_only=columns_obs_only,
         index_column="patient_id",
@@ -418,20 +408,17 @@
     Args:
         encoded: Whether to return an already encoded object.
         columns_obs_only: Columns to include in obs only and not X.
 
     Returns:
         :class:`~anndata.AnnData` object of the Thyroid Data Set
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.dt.thyroid(encoded=True)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.thyroid(encoded=True)
     """
     adata: AnnData = read_csv(
         dataset_path=f"{ehrapy_settings.datasetdir}/thyroid.csv",
         download_dataset_name="thyroid.csv",
         backup_url="https://figshare.com/ndownloader/files/34179333",
         columns_obs_only=columns_obs_only,
         index_column="patient_id",
@@ -454,20 +441,17 @@
     Args:
         encoded: Whether to return an already encoded object.
         columns_obs_only: Columns to include in obs only and not X.
 
     Returns:
         :class:`~anndata.AnnData` object of the Breast Cancer Coimbra Data Set
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.dt.breast_cancer_coimbra(encoded=True)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.breast_cancer_coimbra(encoded=True)
     """
     adata: AnnData = read_csv(
         dataset_path=f"{ehrapy_settings.datasetdir}/breast_cancer_coimbra.csv",
         download_dataset_name="breast_cancer_coimbra.csv",
         backup_url="https://figshare.com/ndownloader/files/34439681",
         columns_obs_only=columns_obs_only,
         index_column="patient_id",
@@ -490,20 +474,17 @@
     Args:
         encoded: Whether to return an already encoded object.
         columns_obs_only: Columns to include in obs only and not X.
 
     Returns:
         :class:`~anndata.AnnData` object of the Parkinsons Data Set
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.dt.parkinsons(columns_obs_only=['name'], encoded=True)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.parkinsons(columns_obs_only=['name'], encoded=True)
     """
     adata: AnnData = read_csv(
         dataset_path=f"{ehrapy_settings.datasetdir}/parkinsons.csv",
         download_dataset_name="parkinsons.csv",
         backup_url="https://figshare.com/ndownloader/files/34439684",
         columns_obs_only=columns_obs_only,
         index_column="measurement_id",
@@ -526,20 +507,17 @@
     Args:
         encoded: Whether to return an already encoded object.
         columns_obs_only: Columns to include in obs only and not X.
 
     Returns:
         :class:`~anndata.AnnData` object of the Parkinsons Telemonitoring Data Set
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.dt.parkinsons_telemonitoring(encoded=True)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.parkinsons_telemonitoring(encoded=True)
     """
     adata: AnnData = read_csv(
         dataset_path=f"{ehrapy_settings.datasetdir}/parkinsons_telemonitoring.csv",
         download_dataset_name="parkinsons_telemonitoring.csv",
         backup_url="https://figshare.com/ndownloader/files/34439708",
         columns_obs_only=columns_obs_only,
         index_column="measurement_id",
@@ -562,20 +540,17 @@
     Args:
         encoded: Whether to return an already encoded object.
         columns_obs_only: Columns to include in obs only and not X.
 
     Returns:
         :class:`~anndata.AnnData` object of the Parkinson's Disease Classification Data Set
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.dt.parkinsons_disease_classification(encoded=True)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.parkinsons_disease_classification(encoded=True)
     """
     adata: AnnData = read_csv(
         dataset_path=f"{ehrapy_settings.datasetdir}/parkinson's_disease_classification_prepared.csv",
         download_dataset_name="parkinson's_disease_classification_prepared.csv",
         backup_url="https://figshare.com/ndownloader/files/34439714",
         columns_obs_only=columns_obs_only,
         index_column="measurement_id",
@@ -598,20 +573,17 @@
     Args:
         encoded: Whether to return an already encoded object.
         columns_obs_only: Columns to include in obs only and not X.
 
     Returns:
         :class:`~anndata.AnnData` object of the Parkinson Dataset with replicated acoustic features Data Set
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.dt.parkinson_dataset_with_replicated_acoustic_features(columns_obs_only=['ID'], encoded=True)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.parkinson_dataset_with_replicated_acoustic_features(columns_obs_only=['ID'], encoded=True)
     """
     adata: AnnData = read_csv(
         dataset_path=f"{ehrapy_settings.datasetdir}/parkinson_dataset_with_replicated_acoustic_features.csv",
         download_dataset_name="parkinson_dataset_with_replicated_acoustic_features.csv",
         backup_url="https://figshare.com/ndownloader/files/34439801",
         columns_obs_only=columns_obs_only,
         index_column="measurement_id",
@@ -634,25 +606,56 @@
     Args:
         encoded: Whether to return an already encoded object.
         columns_obs_only: Columns to include in obs only and not X.
 
     Returns:
         :class:`~anndata.AnnData` object of the Heart Disease Data Set
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.dt.heart_disease(encoded=True)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.heart_disease(encoded=True)
     """
     adata: AnnData = read_csv(
         dataset_path=f"{ehrapy_settings.datasetdir}/processed_heart_disease.csv",
         download_dataset_name="processed_heart_disease.csv",
         backup_url="https://figshare.com/ndownloader/files/34906647",
         columns_obs_only=columns_obs_only,
         index_column="patient_id",
     )
     if encoded:
         return encode(adata, autodetect=True)
 
     return adata
+
+
+def synthea_1k_sample(
+    encoded: bool = False,
+    columns_obs_only: list[str] | None = None,
+) -> AnnData:
+    """Loads the 1K Sample Synthetic Patient Records Data Set
+
+    More details: https://synthea.mitre.org/downloads
+    Preprocessing: TODO: add preprocessing link
+
+    Args:
+        encoded: Whether to return an already encoded object.
+        columns_obs_only: Columns to include in obs only and not X.
+
+    Returns:
+        :class:`~anndata.AnnData` object of the 1K Sample Synthetic Patient Records Data Set
+
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.synthea_1k_sample(encoded=True)
+    """
+    adata: AnnData = read_fhir(
+        dataset_path=f"{ehrapy_settings.datasetdir}/synthea_sample",
+        download_dataset_name="synthea_sample",
+        backup_url="https://synthetichealth.github.io/synthea-sample-data/downloads/synthea_sample_data_fhir_dstu2_sep2019.zip",
+        columns_obs_only=columns_obs_only,
+        index_column="id",
+    )
+
+    if encoded:
+        return encode(adata, autodetect=True)
+
+    return adata
```

### Comparing `ehrapy-0.3.0/ehrapy/io/_read.py` & `ehrapy-0.4.0/ehrapy/io/_read.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import shutil
 from pathlib import Path
-from typing import Iterator
+from typing import Iterator, Literal
 
+import fhiry.parallel as fp
 import numpy as np
 import pandas as pd
 from _collections import OrderedDict
 from anndata import AnnData
 from anndata import read as read_h5
 from mudata import MuData
 from rich import print
@@ -31,169 +32,157 @@
     download_dataset_name: str | None = None,
     **kwargs,
 ) -> AnnData | dict[str, AnnData] | MuData:
     """Reads or downloads a desired directory of csv/tsv files or a single csv/tsv file.
 
     Args:
         dataset_path: Path to the file or directory to read.
-        sep: Separator in the file; either , (default) or \t.
+        sep: Separator in the file. One of either , (comma) or \t (tab). Defaults to , (comma)
         index_column: The index column of obs. Usually the patient visit ID or the patient ID.
         columns_obs_only: These columns will be added to obs only and not X.
-        columns_x_only: These columns will be added to X only and all remaining columns to obs. Note that datetime columns will always be added to .obs though.
+        columns_x_only: These columns will be added to X only and all remaining columns to obs.
+                        Note that datetime columns will always be added to .obs though.
         return_dfs: Whether to return one or several Pandas DataFrames.
-        return_mudata: Whether to create and return a MuData object. This is primarily used for complex datasets which require several AnnData files.
-        cache: Whether to write to cache when reading or not. (default: False)
-        download_dataset_name: Name of the file or directory in case the dataset is downloaded
+        return_mudata: Whether to create and return a MuData object.
+                       This is primarily used for complex datasets which require several AnnData files.
+        cache: Whether to write to cache when reading or not. Defaults to False .
+        download_dataset_name: Name of the file or directory in case the dataset is downloaded.
         backup_url: URL to download the data file(s) from if not yet existing.
 
     Returns:
         An :class:`~anndata.AnnData` object, a :class:`~mudata.MuData` object or a dict with an identifier (the filename, without extension)
         for each :class:`~anndata.AnnData` object in the dict
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-            adata = ep.io.read_csv("myfile.csv")
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.io.read_csv("myfile.csv")
     """
     _check_columns_only_params(columns_obs_only, columns_x_only)
     file: Path = Path(dataset_path)
     if not file.exists():
         file = _get_non_existing_files(file, download_dataset_name, backup_url)
 
     adata = _read_csv(
-        filename=file,
+        file_path=file,
         sep=sep,
         index_column=index_column,
         columns_obs_only=columns_obs_only,
         columns_x_only=columns_x_only,
         return_dfs=return_dfs,
         return_mudata=return_mudata,
         cache=cache,
         **kwargs,
     )
     return adata
 
 
-def read_h5ad(
-    dataset_path: Path | str,
-    backup_url: str | None = None,
-    download_dataset_name: str | None = None,
-) -> AnnData | dict[str, AnnData] | MuData:
-    """Reads or downloads a desired directory of h5ad files or a single h5ad file.
-
-    Args:
-        dataset_path: Path to the file or directory to read.
-        download_dataset_name: Name of the file or directory in case the dataset is downloaded
-        backup_url: URL to download the data file(s) from if not yet existing.
-
-    Returns:
-        An :class:`~anndata.AnnData` object or a dict with an identifier (the filename, without extension)
-        for each :class:`~anndata.AnnData` object in the dict
-
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = eh.data.mimic_2(encode=True)
-            ep.io.write("mimic_2.h5ad", adata)
-            adata_2 = ep.io.read_h5ad("mimic_2.h5ad")
-    """
-    file: Path = Path(dataset_path)
-    if not file.exists():
-        file = _get_non_existing_files(file, download_dataset_name, backup_url)
-
-    adata = _read_h5ad(filename=file)
-    return adata
-
-
 def _read_csv(
-    filename: Path,
+    file_path: Path,
     sep: str,
     index_column: dict[str, str | int] | str | int | None,
     columns_obs_only: dict[str, list[str]] | list[str] | None,
     columns_x_only: dict[str, list[str]] | list[str] | None,
     return_dfs: bool = False,
     return_mudata: bool = False,
     cache: bool = False,
     **kwargs,
 ) -> AnnData | dict[str, AnnData] | MuData:
     """Internal interface of the read_csv method."""
     if cache and (return_mudata or return_dfs):
-        _cache_not_supported()
+        raise CachingNotSupported("Caching is currently not supported for MuData or Pandas DataFrame objects.")
     if return_dfs and (columns_x_only or columns_obs_only):
         raise Warning(
             "Parameters columns_x_only and columns_obs_only are not supported when returning Pandas DataFrames."
         )
-    path_cache = settings.cachedir / filename
+    path_cache = settings.cachedir / file_path
     # reading from (cache) file is separated in the read_h5ad function
     if cache and (path_cache.is_dir() or path_cache.is_file()):
         raise CacheExistsException(
             f"{path_cache} already exists. Use the read_h5ad function instead to read from cache!"
         )
-    # If the filename is a directory, assume it is a dataset with multiple files
-    elif filename.is_dir():
+    # If the the file path is a directory, assume it is a dataset with multiple files
+    elif file_path.is_dir():
         return _read_from_directory(
-            filename,
+            file_path,
             cache,
             path_cache,
             extension=sep,
             index_column=index_column,
             columns_obs_only=columns_obs_only,
             columns_x_only=columns_x_only,
             return_dfs=return_dfs,
             return_mudata=return_mudata,  # type: ignore
         )
     # input is a single file
     else:
         if sep not in {",", "\t"}:
             raise ValueError("Please provide one of the available separators , or tab")
         adata, columns_obs_only = _do_read_csv(
-            filename, sep, index_column, columns_obs_only, columns_x_only, cache, **kwargs  # type: ignore
+            file_path, sep, index_column, columns_obs_only, columns_x_only, cache, **kwargs  # type: ignore
         )
         # cache results if desired
         if cache:
             if not path_cache.parent.is_dir():
                 path_cache.parent.mkdir(parents=True)
             return _write_cache(adata, path_cache, columns_obs_only)  # type: ignore
         return adata
 
 
-def _read_h5ad(
-    filename: Path,
-) -> AnnData | dict[str, AnnData]:
-    """Internal interface of the read_h5ad method."""
-
-    # If the filename is a directory, assume it is a dataset with h5ad multiple files
-    if filename.is_dir():
-        return _read_from_directory(filename, False, None, "h5ad")
-    # dataset is a single h5ad file
+def read_h5ad(
+    dataset_path: Path | str,
+    backup_url: str | None = None,
+    download_dataset_name: str | None = None,
+) -> AnnData | dict[str, AnnData] | MuData:
+    """Reads or downloads a desired directory of h5ad files or a single h5ad file.
+
+    Args:
+        dataset_path: Path to the file or directory to read.
+        download_dataset_name: Name of the file or directory in case the dataset is downloaded
+        backup_url: URL to download the data file(s) from if not yet existing.
+
+    Returns:
+        An :class:`~anndata.AnnData` object or a dict with an identifier (the filename, without extension)
+        for each :class:`~anndata.AnnData` object in the dict
+
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.mimic_2(encoded=True)
+        >>> ep.io.write("mimic_2.h5ad", adata)
+        >>> adata_2 = ep.io.read_h5ad("mimic_2.h5ad")
+    """
+    file_path: Path = Path(dataset_path)
+    if not file_path.exists():
+        file_path = _get_non_existing_files(file_path, download_dataset_name, backup_url)
+
+    if file_path.is_dir():
+        adata = _read_from_directory(file_path, False, None, "h5ad")
     else:
-        return _do_read_h5ad(filename)
+        adata = _do_read_h5ad(file_path)
+
+    return adata
 
 
 def _read_from_directory(
-    filename: Path,
+    file_path: Path,
     cache: bool,
     path_cache_dir: Path | None,
     extension: str,
     index_column: dict[str, str | int] | str | int | None = None,
     columns_obs_only: dict[str, list[str]] | list[str] | None = None,
     columns_x_only: dict[str, list[str]] | list[str] | None = None,
     return_dfs: bool = False,
     return_mudata: bool = False,
 ) -> dict[str, AnnData] | dict[str, pd.DataFrame]:
     """Parse AnnData objects or Pandas DataFrames from a directory containing the data files"""
     if return_dfs:
-        dfs = _read_multiple_csv(filename, sep=extension, return_dfs=True)
+        dfs = _read_multiple_csv(file_path, sep=extension, return_dfs=True)
         return dfs  # type: ignore
     if extension in {",", "\t"}:
         adata_objects, columns_obs_only = _read_multiple_csv(  # type: ignore
-            filename,
+            file_path,
             sep=extension,
             index_column=index_column,
             columns_obs_only=columns_obs_only,
             columns_x_only=columns_x_only,
             return_dfs=False,
             return_mudata=return_mudata,
         )
@@ -201,34 +190,34 @@
         if cache:
             if not path_cache_dir.parent.is_dir():
                 path_cache_dir.parent.mkdir(parents=True)
             path_cache_dir.mkdir()
             return _write_cache_dir(adata_objects, path_cache_dir, columns_obs_only, index_column)  # type: ignore
         return adata_objects  # type: ignore
     elif extension == "h5ad":
-        return _read_multiple_h5ad(filename)
+        return _read_multiple_h5ad(file_path)
     else:
         raise NotImplementedError(f"Reading from directory with .{extension} files is not implemented yet!")
 
 
 def _read_multiple_csv(  # noqa: N802
-    filename: Path,
+    file_path: Path,
     sep: str,
     index_column: dict[str, str | int] | str | int | None = None,
     columns_obs_only: dict[str, list[str]] | list[str] | None = None,
     columns_x_only: dict[str, list[str]] | list[str] | None = None,
     return_dfs: bool = False,
     return_mudata_object: bool = False,
     cache: bool = False,
     **kwargs,
 ) -> tuple[dict[str, AnnData], dict[str, list[str] | None]] | MuData | dict[str, pd.DataFrame]:
     """Read a dataset containing multiple .csv/.tsv files.
 
     Args:
-        filename: File path to the directory containing multiple .csv/.tsv files.
+        file_path: File path to the directory containing multiple .csv/.tsv files.
         sep: Either , or \t to determine which files to read.
         index_column: Column names of the index columns for obs
         columns_obs_only: List of columns per file (AnnData object) which should only be stored in .obs, but not in X. Useful for free text annotations.
         columns_x_only: List of columns per file (AnnData object) which should only be stored in .X, but not in obs. Datetime columns will be added to .obs regardless.
         return_dfs: When set to True, return a dictionary of Pandas DataFrames.
         return_mudata_object: When set to True, return a :class:`~mudata.MuData` object, otherwise a dict of :class:`~anndata.AnnData` objects
         cache: Whether to cache results or not
@@ -241,15 +230,15 @@
     obs_only_all = {}
     if not return_mudata_object and not return_dfs:
         anndata_dict = {}
     elif return_dfs:
         df_dict: dict[str, pd.DataFrame] = {}
     elif return_mudata_object:
         mudata = None
-    for file in filename.iterdir():
+    for file in file_path.iterdir():
         if file.is_file() and file.suffix in {".csv", ".tsv"}:
             # slice off the file suffix .csv or .tsv for a clean file name
             file_identifier = file.name[:-4]
             if return_dfs:
                 df = pd.read_csv(file, sep=sep, **kwargs)
                 df_dict[file_identifier] = df
                 continue
@@ -275,48 +264,27 @@
         return mudata
     elif return_dfs:
         return df_dict
     else:
         return anndata_dict, obs_only_all
 
 
-def _read_multiple_h5ad(  # noqa: N802
-    filename: Path,
-) -> dict[str, AnnData]:
-    """Read a dataset containing multiple .h5ad files.
-
-    Args:
-        filename: File path to the directory containing multiple .csv/.tsv files.
-
-    Returns:
-        A dict mapping the filename (object name) to the corresponding :class:`~anndata.AnnData` object
-    """
-    anndata_dict = {}
-    for file in filename.iterdir():
-        if file.is_file() and file.suffix == ".h5ad":
-            # slice off the file suffix .h5ad
-            adata_identifier = file.name[:-5]
-            adata = _do_read_h5ad(file)
-            anndata_dict[adata_identifier] = adata
-    return anndata_dict
-
-
 def _do_read_csv(
-    filename: Path | Iterator[str],
+    file_path: Path | Iterator[str],
     delimiter: str | None = ",",
     index_column: str | int | None = None,
     columns_obs_only: list[str] | None = None,
     columns_x_only: list[str] | None = None,
     cache: bool = False,
     **kwargs,
 ) -> tuple[AnnData, list[str] | None]:
     """Read `.csv` and `.tsv` file.
 
     Args:
-        filename: File path to the csv file.
+        file_path: File path to the csv file.
         delimiter: Delimiter separating the csv data within the file.
         index_column: Index or column name of the index column (obs)
         columns_obs_only: List of columns which only be stored in .obs, but not in X. Useful for free text annotations.
         columns_x_only: List of columns which only be stored in X, but not in .obs.
 
         cache: Whether the data should be written to cache or not
 
@@ -326,43 +294,161 @@
     try:
         if index_column and columns_obs_only and index_column in columns_obs_only:
             print(
                 f"[bold yellow]Index column [blue]{index_column} [yellow]is also used as a column "
                 f"for obs only. Using default indices instead and moving [blue]{index_column} [yellow]to column_obs_only."
             )
             index_column = None
-        initial_df = pd.read_csv(filename, delimiter=delimiter, index_col=index_column, **kwargs)
+        initial_df = pd.read_csv(file_path, delimiter=delimiter, index_col=index_column, **kwargs)
     # in case the index column is misspelled or does not exist
     except ValueError:
         raise IndexNotFoundError(
-            f"Could not create AnnData object while reading file {filename}. Does index_column named {index_column} "
-            f"exist in {filename}?"
+            f"Could not create AnnData object while reading file {file_path}. Does index_column named {index_column} "
+            f"exist in {file_path}?"
         ) from None
 
     initial_df, columns_obs_only = _prepare_dataframe(initial_df, columns_obs_only, columns_x_only, cache)
+
     return df_to_anndata(initial_df, columns_obs_only), columns_obs_only
 
 
-def _do_read_h5ad(filename: Path | Iterator[str]) -> AnnData:
+def _read_multiple_h5ad(  # noqa: N802
+    file_path: Path,
+) -> dict[str, AnnData]:
+    """Read a dataset containing multiple .h5ad files.
+
+    Args:
+        file_path: File path to the directory containing multiple .csv/.tsv files.
+
+    Returns:
+        A dict mapping the filename (object name) to the corresponding :class:`~anndata.AnnData` object
+    """
+    anndata_dict = {}
+    for file in file_path.iterdir():
+        if file.is_file() and file.suffix == ".h5ad":
+            # slice off the file suffix .h5ad
+            adata_identifier = file.name[:-5]
+            adata = _do_read_h5ad(file)
+            anndata_dict[adata_identifier] = adata
+    return anndata_dict
+
+
+def _do_read_h5ad(file_path: Path | Iterator[str]) -> AnnData:
     """Read from a h5ad file.
     Args:
-        filename: Path to the h5ad file
+        file_path: Path to the h5ad file
 
     Returns:
         An AnnData object.
     """
-    adata = read_h5(filename)
+    adata = read_h5(file_path)
     if "ehrapy_dummy_encoding" in adata.uns.keys():
         # if dummy encoding was needed, the original dtype of X could not be numerical, so cast it to object
         adata.X = adata.X.astype("object")
         decoded_adata = _decode_cached_adata(adata, list(adata.uns["columns_obs_only"]))
         return decoded_adata
     return adata
 
 
+def read_fhir(
+    dataset_path: str,
+    format: Literal["json", "ndjson"] = "json",
+    columns_obs_only: list[str] | None = None,
+    columns_x_only: list[str] | None = None,
+    return_df: bool = False,
+    cache: bool = False,
+    backup_url: str | None = None,
+    index_column: str | int | None = None,
+    download_dataset_name: str | None = None,
+) -> pd.DataFrame | AnnData:
+    """Reads one or multiple FHIR files using fhiry.
+
+    Uses https://github.com/dermatologist/fhiry to read the FHIR file into a Pandas DataFrame
+    which is subsequently transformed into an AnnData object.
+
+    Args:
+        dataset_path: Path to one or multiple FHIR files.
+        format: The file format of the FHIR data. One of 'json' or 'ndjson'. Defaults to 'json'.
+        columns_obs_only: These columns will be added to obs only and not X.
+        columns_x_only: These columns will be added to X only and all remaining columns to obs. Note that datetime columns will always be added to .obs though.
+        return_df: Whether to return one or several Pandas DataFrames.
+        cache: Whether to write to cache when reading or not. Defaults to False.
+        download_dataset_name: Name of the file or directory in case the dataset is downloaded
+        index_column: The index column for the generated object. Usually the patient or visit ID.
+        backup_url: URL to download the data file(s) from if not yet existing.
+
+    Returns:
+        A Pandas DataFrame or AnnData object of the read in FHIR file(s).
+
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.io.read_fhir("/path/to/fhir/resources")
+    """
+    _check_columns_only_params(columns_obs_only, columns_x_only)
+    file_path: Path = Path(dataset_path)
+    if not file_path.exists():
+        file_path = _get_non_existing_files(file_path, download_dataset_name, backup_url)
+
+    adata = _read_fhir(
+        file_path=str(file_path.resolve()),
+        format=format,
+        index_column=index_column,
+        columns_obs_only=columns_obs_only,
+        columns_x_only=columns_x_only,
+        return_df=return_df,
+        cache=cache,
+    )
+    return adata
+
+
+def _read_fhir(
+    file_path: str,
+    format: Literal["json", "ndjson"],
+    index_column: dict[str, str | int] | str | int | None,
+    columns_obs_only: list[str] | None,
+    columns_x_only: list[str] | None,
+    return_df: bool = False,
+    cache: bool = False,
+) -> AnnData | dict[str, AnnData] | MuData:
+    """Internal interface of the read_fhir method."""
+    if cache and return_df:
+        raise CachingNotSupported("Caching is currently not supported for MuData or Pandas DataFrame objects.")
+    if return_df and (columns_x_only or columns_obs_only):
+        raise Warning(
+            "Parameters columns_x_only and columns_obs_only are not supported when returning Pandas DataFrames."
+        )
+    path_cache = settings.cachedir / file_path
+    if cache and (path_cache.is_dir() or path_cache.is_file()):
+        raise CacheExistsException(
+            f"{path_cache} already exists. Use the read_h5ad function instead to read from cache!"
+        )
+    if format == "json":
+        df = fp.process(file_path)
+    elif format == "ndjson":
+        df = fp.ndjson(file_path)
+    else:
+        raise ValueError("Only folders containing json and ndjson in FHIR format are supported.")
+
+    df, columns_obs_only = _prepare_dataframe(df, columns_obs_only, columns_x_only, cache)
+    if index_column:
+        df.set_index(index_column)
+
+    if return_df:
+        return df
+    else:
+        adata = df_to_anndata(df, columns_obs_only)
+
+    if cache:
+        if not path_cache.parent.is_dir():
+            path_cache.parent.mkdir(parents=True)
+        return _write_cache(adata, path_cache, columns_obs_only)  # type: ignore
+
+    return adata
+
+
 def _get_non_existing_files(file: Path, download_dataset_name: str, backup_url: str) -> Path:
     """Handle non existing files or directories by trying to download from a backup_url and moving them
     in the correct directory.
 
     Args:
         backup_url: Backup URL to lookup for the datafile(s)
 
@@ -389,16 +475,24 @@
         is_archived=is_archived,
     )
     # if archived, remove archive suffix
     archive_extension = download_default_name[-4:]
     output_path_name = download_default_name.replace(archive_extension, "") if is_archived else download_default_name
     output_file_or_dir = ehrapy_settings.datasetdir / output_path_name
     moved_path = Path(str(output_file_or_dir)[: str(output_file_or_dir).rfind("/") + 1]) / download_dataset_name
-    shutil.move(output_file_or_dir, moved_path)  # type: ignore
-    file = moved_path
+    if moved_path.exists():
+        shutil.move(output_file_or_dir, moved_path)  # type: ignore
+        file = moved_path
+    elif (
+        not moved_path.exists()
+    ):  # some zip files change their name when unzipped. Hence, we look for the latest created file in datasetdir
+        list_of_paths = [path for path in ehrapy_settings.datasetdir.glob("*/") if not path.name.startswith(".")]
+        latest_path = max(list_of_paths, key=lambda path: path.stat().st_ctime)
+        shutil.move(latest_path, moved_path)  # type: ignore
+        file = moved_path
 
     return file
 
 
 def _read_from_cache_dir(cache_dir: Path) -> dict[str, AnnData]:
     """Read AnnData objects from the cache directory."""
     adata_objects = {}
@@ -555,16 +649,15 @@
     adata.uns["numerical_columns"] = numerical_columns
     adata.uns["non_numerical_columns"] = list(set(adata.var_names) ^ set(numerical_columns))
 
     return adata
 
 
 def _extract_index_and_columns_obs_only(identifier: str, index_columns, columns_obs_only, columns_x_only=None):
-    """
-    Extract the index column (if any) and the columns, for obs only (if any) from the given user input.
+    """Extract the index column (if any) and the columns, for obs only (if any) from the given user input.
 
     For each file, `index_columns` and `columns_obs_only` can provide three cases:
         1.) The filename (thus the identifier) is not present as a key and no default key is provided or one or both dicts are empty:
             --> No index column will be set and/or no columns are obs only (based on user input)
 
             .. code-block:: python
                    # some setup code here
@@ -670,33 +763,25 @@
             raise ValueError(
                 "Can not use columns_obs_only together with columns_x_only for a single AnnData object. "
                 "The following anndata identifiers where found"
                 f"in both: {','.join(key for key in common_keys)}!"
             )
 
 
-def _cache_not_supported():
-    raise MudataCachingNotSupportedError("Caching is currently not supported for MuData or Pandas DataFrame objects.")
-
-
 class IndexNotFoundError(Exception):
     pass
 
 
 class BackupURLNotProvidedError(Exception):
     pass
 
 
-class MudataCachingNotSupportedError(Exception):
+class CachingNotSupported(Exception):
     pass
 
 
 class ExtensionMissingError(Exception):
     pass
 
 
-class UnsupportedDirectoryParsingFormatException(Exception):
-    pass
-
-
 class CacheExistsException(Exception):
     pass
```

### Comparing `ehrapy-0.3.0/ehrapy/io/_utility_io.py` & `ehrapy-0.4.0/ehrapy/io/_utility_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 supported_extensions = {"csv", "tsv", "h5ad"}
 
 
 def _get_file_extension(file_path: Path) -> str:
     """Check whether the argument is a filename.
 
     Args:
-        file_path: Path to the file
+        file_path: Path to the file.
 
     Returns:
         File extension of the specified file
     """
     ext = file_path.suffixes
 
     if len(ext) > 2:
```

### Comparing `ehrapy-0.3.0/ehrapy/logging.py` & `ehrapy-0.4.0/ehrapy/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,21 +81,20 @@
 class _LogFormatter(logging.Formatter):
     def __init__(self, auto_colorized=True):
         super().__init__()
         self.auto_colorized = auto_colorized
         self.FORMATS = self.define_format()
 
     def define_format(self):
-        grey = "\x1b[0;37m"
+        grey = "\x1b[1;30m"
         green = "\x1b[1;32m"
         yellow = "\x1b[1;33m"
         red = "\x1b[1;31m"
         purple = "\x1b[1;35m"
         blue = "\x1b[1;34m"
-        # light_blue = "\x1b[1;36m"
         reset = "\x1b[0m"
         blink_red = "\x1b[5m\x1b[1;31m"
 
         format_prefix = f"{purple}%(asctime)s{reset} - " f"{blue}%(name)s{reset} "
 
         # format_prefix = f"{purple}%(asctime)s{reset} " \
         #                 f"{blue}%(name)s{reset} " \
```

### Comparing `ehrapy-0.3.0/ehrapy/plot/_missingno_pl_api.py` & `ehrapy-0.4.0/ehrapy/plot/_missingno_pl_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     sparkline: bool = True,
     categoricals: bool = False,
 ):  # pragma: no cover
     """A matrix visualization of the nullity of the given AnnData object.
 
     Args:
         adata: :class:`~anndata.AnnData` object object containing all observations.
-        filter: The filter to apply to the matrix. Should be one of "top", "bottom", or None (default).
+        filter: The filter to apply to the matrix. Should be one of "top", "bottom", or None. Defaults to None .
         max_cols: The max number of columns from the AnnData object to include.
         max_percentage: The max percentage fill of the columns from the AnnData object.
         sort: The row sort order to apply. Can be "ascending", "descending", or None.
         figsize: The size of the figure to display.
         width_ratios: The ratio of the width of the matrix to the width of the sparkline.
         color: The color of the filled columns.
         fontsize: The figure's font size.
@@ -39,21 +39,18 @@
         label_rotation: What angle to rotate the text labels to.
         sparkline: Whether or not to display the sparkline.
         categoricals: Whether to include "ehrapycat" columns to the plot.
 
     Returns:
         The plot axis.
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.data.mimic_2(encoded=True)
-            ep.pl.missing_values_matrix(adata, filter='bottom', max_cols=15, max_percentage=0.999)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> ep.pl.missing_values_matrix(adata, filter='bottom', max_cols=15, max_percentage=0.999)
 
     Preview:
         .. image:: /_static/docstring_previews/missingno_matrix.png
     """
     df = ae.anndata_to_df(adata)
 
     if not categoricals:
@@ -105,36 +102,33 @@
     categoricals: bool = False,
 ):  # pragma: no cover
     """A bar chart visualization of the nullity of the given AnnData object.
 
     Args:
         adata: :class:`~anndata.AnnData` object object containing all observations.
         log: Whether or not to display a logarithmic plot.
-        filter: The filter to apply to the barplot. Should be one of "top", "bottom", or None (default).
+        filter: The filter to apply to the barplot. Should be one of "top", "bottom", or None. Defaults to None .
         max_cols: The max number of columns from the AnnData object to include.
         max_percentage: The max percentage fill of the columns from the AnnData object.
         sort: The row sort order to apply. Can be "ascending", "descending", or None.
         figsize: The size of the figure to display.
         color: The color of the filled columns.
         fontsize: The figure's font size.
         labels: Whether or not to display the column names.
         label_rotation: What angle to rotate the text labels to.
         orientation: The way the bar plot is oriented.
         categoricals: Whether to include "ehrapycat" columns to the plot.
 
     Returns:
         The plot axis.
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.data.mimic_2(encoded=True)
-            ep.pl.missing_values_barplot(adata, filter='bottom', max_cols=15, max_percentage=0.999)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> ep.pl.missing_values_barplot(adata, filter='bottom', max_cols=15, max_percentage=0.999)
 
     Preview:
         .. image:: /_static/docstring_previews/missingno_barplot.png
     """
     df = ae.anndata_to_df(adata)
 
     if not categoricals:
@@ -188,15 +182,15 @@
 ):  # pragma: no cover
     """Presents a `seaborn` heatmap visualization of nullity correlation in the given AnnData object.
 
     Note that this visualization has no special support for large datasets. For those, try the dendrogram instead.
 
     Args:
         adata: :class:`~anndata.AnnData` object object containing all observations.
-        filter: The filter to apply to the heatmap. Should be one of "top", "bottom", or None (default).
+        filter: The filter to apply to the heatmap. Should be one of "top", "bottom", or None. Defaults to None .
         max_cols: The max number of columns from the AnnData object to include.
         max_percentage: The max percentage fill of the columns from the AnnData object.
         sort: The row sort order to apply. Can be "ascending", "descending", or None.
         figsize: The size of the figure to display.
         fontsize: The figure's font size.
         labels: Whether or not to display the column names.
         label_rotation: What angle to rotate the text labels to.
@@ -205,21 +199,18 @@
         vmax: The normalized colormap threshold.
         cbar: Whether to draw a colorbar.
         categoricals: Whether to include "ehrapycat" columns to the plot.
 
     Returns:
         The plot axis.
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.data.mimic_2(encoded=True)
-            ep.pl.missing_values_heatmap(adata, filter='bottom', max_cols=15, max_percentage=0.999)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> ep.pl.missing_values_heatmap(adata, filter='bottom', max_cols=15, max_percentage=0.999)
 
     Preview:
         .. image:: /_static/docstring_previews/missingno_heatmap.png
     """
     df = ae.anndata_to_df(adata)
 
     if not categoricals:
@@ -274,33 +265,30 @@
 
     The default vertical display will fit up to 50 columns. If more than 50 columns are specified and orientation is
     left unspecified the dendrogram will automatically swap to a horizontal display to fit the additional variables.
 
     Args:
         adata: :class:`~anndata.AnnData` object object containing all observations.
         method: The distance measure being used for clustering. This parameter is passed to `scipy.hierarchy`.
-        filter: The filter to apply to the dendrogram. Should be one of "top", "bottom", or None (default).
+        filter: The filter to apply to the dendrogram. Should be one of "top", "bottom", or None. Defaults to None .
         max_cols: The max number of columns from the AnnData object to include.
         max_percentage: The max percentage fill of the columns from the AnnData object.
         figsize: The size of the figure to display.
         fontsize: The figure's font size.
         orientation: The way the dendrogram is oriented.
         label_rotation: What angle to rotate the text labels to. .
         categoricals: Whether to include "ehrapycat" columns to the plot.
 
     Returns:
         The plot axis.
 
     Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.data.mimic_2(encoded=True)
-            ep.pl.missing_values_dendrogram(adata, filter='bottom', max_cols=15, max_percentage=0.999)
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> ep.pl.missing_values_dendrogram(adata, filter='bottom', max_cols=15, max_percentage=0.999)
 
     Preview:
         .. image:: /_static/docstring_previews/missingno_dendrogram.png
     """
     df = ae.anndata_to_df(adata)
 
     if not categoricals:
```

### Comparing `ehrapy-0.3.0/ehrapy/plot/_qc.py` & `ehrapy-0.4.0/ehrapy/plot/_qc.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 
        Per default this will display the following features:
        ``missing_values_abs``, ``missing_values_pct``, ``mean``, ``median``, ``standard_deviation``, ``max``, ``min``.
 
     Args:
         adata: Annotated data matrix.
         extra_columns: List of custom (qc) var columns to be displayed additionally.
+
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.mimic_2(encoded=True)
+        >>> ep.pp.qc_metrics(adata)
+        >>> ep.pl.qc_metrics(adata)
     """
     table = Table(title="[bold blue]Ehrapy qc metrics of var")
     # add special column header for the column name
     table.add_column("[bold blue]Column name", justify="right", style="bold green")
     var_names = list(adata.var_names)
     # default qc columns added to var
     fixed_qc_columns = [
@@ -29,24 +35,20 @@
         "min",
         "max",
     ]
     # update columns to display with extra columns (if any)
     columns_to_display = fixed_qc_columns if not extra_columns else fixed_qc_columns + extra_columns
     # check whether all columns exist (qc has been executed before and extra columns are var columns)
     if (set(columns_to_display) & set(adata.var.columns)) != set(columns_to_display):
-        raise QCDisplayError(
+        raise AttributeError(
             "Cannot display QC metrics of current AnnData object. Either QC has not been executed before or "
             "some column(s) of the extra_columns parameter are not in var!"
         )
     vars_to_display = adata.var[columns_to_display]
     # add column headers
     for col in vars_to_display:
         table.add_column(f"[bold blue]{col}", justify="right", style="bold green")
     for var in range(len(vars_to_display)):
         table.add_row(var_names[var], *map(str, list(vars_to_display.iloc[var])))
 
     console = Console()
     console.print(table)
-
-
-class QCDisplayError(Exception):
-    pass
```

### Comparing `ehrapy-0.3.0/ehrapy/plot/_scanpy_pl_api.py` & `ehrapy-0.4.0/ehrapy/plot/_scanpy_pl_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     Example:
         .. code-block:: python
 
             import ehrapy as ep
 
             adata = ep.data.mimic_2(encoded=True)
             ep.pp.knn_impute(adata)
-            ep.pp.norm_log(adata, offset=1)
+            ep.pp.log_norm(adata, offset=1)
             ep.pp.neighbors(adata)
             ep.pl.scatter(adata, x='age', y='icu_los_day', color='icu_los_day')
 
     Preview:
         .. image:: /_static/docstring_previews/scatter.png
     """
     scatter_partial = partial(
@@ -213,15 +213,15 @@
     Example:
         .. code-block:: python
 
             import ehrapy as ep
 
             adata = ep.data.mimic_2(encoded=True)
             ep.pp.knn_impute(adata)
-            ep.pp.norm_log(adata, offset=1)
+            ep.pp.log_norm(adata, offset=1)
             ep.pp.neighbors(adata)
             ep.tl.leiden(adata, resolution=0.5, key_added="leiden_0_5")
             ep.pl.heatmap(adata, var_names=['map_1st', 'hr_1st', 'temp_1st', 'spo2_1st',
                 'abg_count', 'wbc_first', 'hgb_first', 'platelet_first', 'sodium_first',
                 'potassium_first', 'tco2_first', 'chloride_first', 'bun_first',
                 'creatinine_first', 'po2_first', 'pco2_first', 'iv_day_1'], groupby="leiden_0_5")
 
@@ -547,15 +547,15 @@
     Example:
         .. code-block:: python
 
             import ehrapy as ep
 
             adata = ep.data.mimic_2(encoded=True)
             ep.pp.knn_impute(adata)
-            ep.pp.norm_log(adata, offset=1)
+            ep.pp.log_norm(adata, offset=1)
             ep.pp.neighbors(adata)
             ep.tl.leiden(adata, resolution=0.5, key_added="leiden_0_5")
             ep.pl.violin(adata, keys=['age'], groupby="leiden_0_5")
 
     Preview:
         .. image:: /_static/docstring_previews/violin.png
     """
@@ -677,15 +677,15 @@
     Example:
         .. code-block:: python
 
             import ehrapy as ep
 
             adata = ep.data.mimic_2(encoded=True)
             ep.pp.knn_impute(adata)
-            ep.pp.norm_log(adata, offset=1)
+            ep.pp.log_norm(adata, offset=1)
             ep.pp.neighbors(adata)
             ep.tl.leiden(adata, resolution=0.5, key_added="leiden_0_5")
             ep.pl.stacked_violin(adata, var_names=['icu_los_day',
                 'hospital_los_day', 'age', 'gender_num', 'weight_first', 'bmi',
                 'sapsi_first', 'sofa_first', 'service_num', 'day_icu_intime_num',
                 'hour_icu_intime'], groupby="leiden_0_5")
 
@@ -802,15 +802,15 @@
     Example:
         .. code-block:: python
 
             import ehrapy as ep
 
             adata = ep.data.mimic_2(encoded=True)
             ep.pp.knn_impute(adata)
-            ep.pp.norm_log(adata, offset=1)
+            ep.pp.log_norm(adata, offset=1)
             ep.pp.neighbors(adata)
             ep.tl.leiden(adata, resolution=0.5, key_added="leiden_0_5")
             ep.pl.matrixplot(adata, var_names=[
                 'abg_count', 'wbc_first', 'hgb_first', 'platelet_first', 'sodium_first',
                 'potassium_first', 'tco2_first', 'chloride_first', 'bun_first',
                 'creatinine_first', 'po2_first', 'pco2_first', 'iv_day_1'], groupby="leiden_0_5")
 
@@ -890,15 +890,15 @@
     Example:
         .. code-block:: python
 
             import ehrapy as ep
 
             adata = ep.data.mimic_2(encoded=True)
             ep.pp.knn_impute(adata)
-            ep.pp.norm_log(adata, offset=1)
+            ep.pp.log_norm(adata, offset=1)
             ep.pp.neighbors(adata)
             ep.tl.leiden(adata, resolution=0.5, key_added="leiden_0_5")
             ep.pl.clustermap(adata)
 
     Preview:
         .. image:: /_static/docstring_previews/clustermap.png
     """
@@ -933,15 +933,15 @@
     n_points=30,
     log=False,
     include_lowest=False,
     show=None,
 ):  # pragma: no cover
     """Plot rankings.
 
-    See, for example, how this is used in pl.pca_ranking.
+    See, for example, how this is used in pl.pca_loadings.
 
     Args:
         adata: :class:`~anndata.AnnData` object object containing all observations.
         attr: The attribute of AnnData that contains the score.
         keys: The scores to look up an array from the attribute of adata.
         dictionary: Optional key dictionary.
         indices: Optional dictionary indices.
@@ -956,14 +956,20 @@
         Returns matplotlib gridspec with access to the axes.
 
     Example:
         .. code-block:: python
 
             import ehrapy as ep
 
+            adata = ep.data.mimic_2(encoded=True)
+            ep.pp.knn_impute(adata)
+            ep.pp.log_norm(adata, offset=1)
+            ep.pp.neighbors(adata)
+            ep.pp.pca(adata)
+            TODO: ep.pl.ranking(adata)
     """
     return sc.pl.ranking(
         adata=adata,
         attr=attr,
         keys=keys,
         dictionary=dictionary,
         indices=indices,
@@ -1007,15 +1013,15 @@
     Example:
         .. code-block:: python
 
             import ehrapy as ep
 
             adata = ep.data.mimic_2(encoded=True)
             ep.pp.knn_impute(adata)
-            ep.pp.norm_log(adata, offset=1)
+            ep.pp.log_norm(adata, offset=1)
             ep.pp.neighbors(adata)
             ep.tl.leiden(adata, resolution=0.5, key_added="leiden_0_5")
             ep.pl.dendrogram(adata, groupby="leiden_0_5")
 
     Preview:
         .. image:: /_static/docstring_previews/dendrogram.png
     """
@@ -1067,25 +1073,22 @@
         annotate_var_explained: Whether to only annotate the explained variables.
         {scatter_bulk}
         {show_save_ax}
 
     Returns:
         If `show==False` a :class:`~matplotlib.axes.Axes` or a list of it.
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.data.mimic_2(encoded=True)
-            ep.pp.knn_impute(adata)
-            ep.pp.norm_log(adata, offset=1)
-            ep.pp.neighbors(adata)
-            ep.tl.pca(adata)
-            ep.pl.pca(adata, color="service_unit)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> ep.pp.knn_impute(adata)
+        >>> ep.pp.log_norm(adata, offset=1)
+        >>> ep.pp.neighbors(adata)
+        >>> ep.tl.pca(adata)
+        >>> ep.pl.pca(adata, color="service_unit")
 
     Preview:
         .. image:: /_static/docstring_previews/pca.png
     """
     pca_partial = partial(
         sc.pl.pca, annotate_var_explained=annotate_var_explained, show=show, return_fig=return_fig, save=save
     )
@@ -1129,25 +1132,22 @@
         show: Show the plot, do not return axis.
         save: If `True` or a `str`, save the figure. A string is appended to the default filename.
               Infer the filetype if ending on {`'.pdf'`, `'.png'`, `'.svg'`}.
 
     Returns:
         If `show==False` a :class:`~matplotlib.axes.Axes` or a list of it.
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.data.mimic_2(encoded=True)
-            ep.pp.knn_impute(adata)
-            ep.pp.norm_log(adata, offset=1)
-            ep.pp.neighbors(adata)
-            ep.pp.pca(adata)
-            ep.pl.pca_loadings(adata, components='1,2,3')
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> ep.pp.knn_impute(adata)
+        >>> ep.pp.log_norm(adata, offset=1)
+        >>> ep.pp.neighbors(adata)
+        >>> ep.pp.pca(adata)
+        >>> ep.pl.pca_loadings(adata, components='1,2,3')
 
     Preview:
         .. image:: /_static/docstring_previews/pca_loadings.png
     """
     return sc.pl.pca_loadings(adata=adata, components=components, include_lowest=include_lowest, show=show, save=save)
 
 
@@ -1168,25 +1168,22 @@
         save: If `True` or a `str`, save the figure.
               A string is appended to the default filename.
               Infer the filetype if ending on {`'.pdf'`, `'.png'`, `'.svg'`}.
 
     Returns:
         If `show==False` a :class:`~matplotlib.axes.Axes` or a list of it.
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.data.mimic_2(encoded=True)
-            ep.pp.knn_impute(adata)
-            ep.pp.norm_log(adata, offset=1)
-            ep.pp.neighbors(adata)
-            ep.pp.pca(adata)
-            ep.pl.pca_variance_ratio(adata, n_pcs=8)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> ep.pp.knn_impute(adata)
+        >>> ep.pp.log_norm(adata, offset=1)
+        >>> ep.pp.neighbors(adata)
+        >>> ep.pp.pca(adata)
+        >>> ep.pl.pca_variance_ratio(adata, n_pcs=8)
 
     Preview:
         .. image:: /_static/docstring_previews/pca_variance_ratio.png
     """
     return sc.pl.pca_variance_ratio(adata=adata, n_pcs=n_pcs, log=log, show=show, save=save)
 
 
@@ -1202,25 +1199,22 @@
         {scatter_bulk}
         {show_save_ax}
         **params: Scatterplot parameters
 
     Returns:
         If `show==False` a :class:`~matplotlib.axes.Axes` or a list of it.
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.data.mimic_2(encoded=True)
-            ep.pp.knn_impute(adata)
-            ep.pp.norm_log(adata, offset=1)
-            ep.pp.neighbors(adata)
-            ep.pp.pca(adata)
-            ep.pl.pca_overview(adata, components='1,2,3', color="service_unit")
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> ep.pp.knn_impute(adata)
+        >>> ep.pp.log_norm(adata, offset=1)
+        >>> ep.pp.neighbors(adata)
+        >>> ep.pp.pca(adata)
+        >>> ep.pl.pca_overview(adata, components='1,2,3', color="service_unit")
 
     Preview:
         .. image:: /_static/docstring_previews/pca_overview_1.png
 
         .. image:: /_static/docstring_previews/pca_overview_2.png
 
         .. image:: /_static/docstring_previews/pca_overview_3.png
@@ -1243,38 +1237,31 @@
         {edges_arrows}
         {scatter_bulk}
         {show_save_ax}
 
     Returns:
         If `show==False` a :class:`~matplotlib.axes.Axes` or a list of it.
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.data.mimic_2(encoded=True)
-            ep.pp.knn_impute(adata)
-            ep.pp.norm_log(adata, offset=1)
-            ep.pp.neighbors(adata)
-            ep.tl.tsne(adata)
-            ep.pl.tsne(adata)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> ep.pp.knn_impute(adata)
+        >>> ep.pp.log_norm(adata, offset=1)
+        >>> ep.pp.neighbors(adata)
+        >>> ep.tl.tsne(adata)
+        >>> ep.pl.tsne(adata)
 
         .. image:: /_static/docstring_previews/tsne_1.png
 
-        .. code-block:: python
-
-            ep.pl.tsne(adata, color=["day_icu_intime", "service_unit"], wspace=0.5, title=["Day of ICU admission", "Service unit"])
+        >>> ep.pl.tsne(adata, color=["day_icu_intime", "service_unit"], wspace=0.5, title=["Day of ICU admission", "Service unit"])
 
         .. image:: /_static/docstring_previews/tsne_2.png
 
-        .. code-block:: python
-
-            ep.tl.leiden(adata, resolution=0.5, key_added="leiden_0_5")
-            ep.pl.tsne(adata, color=["leiden_0_5"], title="Leiden 0.5")
+        >>> ep.tl.leiden(adata, resolution=0.5, key_added="leiden_0_5")
+        >>> ep.pl.tsne(adata, color=["leiden_0_5"], title="Leiden 0.5")
 
         .. image:: /_static/docstring_previews/tsne_3.png
     """
     if isinstance(adata, MedCAT):
         if kwargs.get("color"):
             if isinstance(kwargs["color"], str):
                 kwargs["color"] = [kwargs["color"]]
@@ -1312,38 +1299,31 @@
         {edges_arrows}
         {scatter_bulk}
         {show_save_ax}
 
     Returns:
         If `show==False` a :class:`~matplotlib.axes.Axes` or a list of it.
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.data.mimic_2(encoded=True)
-            ep.pp.knn_impute(adata)
-            ep.pp.norm_log(adata, offset=1)
-            ep.pp.neighbors(adata)
-            ep.tl.umap(adata)
-            ep.pl.umap(adata)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> ep.pp.knn_impute(adata)
+        >>> ep.pp.log_norm(adata, offset=1)
+        >>> ep.pp.neighbors(adata)
+        >>> ep.tl.umap(adata)
+        >>> ep.pl.umap(adata)
 
         .. image:: /_static/docstring_previews/umap_1.png
 
-        .. code-block:: python
-
-            ep.pl.umap(adata, color=["day_icu_intime", "service_unit"], wspace=0.5, title=["Day of ICU admission", "Service unit"])
+        >>> ep.pl.umap(adata, color=["day_icu_intime", "service_unit"], wspace=0.5, title=["Day of ICU admission", "Service unit"])
 
         .. image:: /_static/docstring_previews/umap_2.png
 
-        .. code-block:: python
-
-            ep.tl.leiden(adata, resolution=0.5, key_added="leiden_0_5")
-            ep.pl.umap(adata, color=["leiden_0_5"], title="Leiden 0.5")
+        >>> ep.tl.leiden(adata, resolution=0.5, key_added="leiden_0_5")
+        >>> ep.pl.umap(adata, color=["leiden_0_5"], title="Leiden 0.5")
 
         .. image:: /_static/docstring_previews/umap_3.png
     """
     if isinstance(adata, MedCAT):
         if kwargs.get("color"):
             if isinstance(kwargs["color"], str):
                 kwargs["color"] = [kwargs["color"]]
@@ -1379,25 +1359,22 @@
         {adata_color_etc}
         {scatter_bulk}
         {show_save_ax}
 
     Returns:
         If `show==False` a :class:`~matplotlib.axes.Axes` or a list of it.
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.data.mimic_2(encoded=True)
-            ep.pp.knn_impute(adata)
-            ep.pp.norm_log(adata, offset=1)
-            ep.pp.neighbors(adata)
-            ep.tl.diffmap(adata)
-            ep.pl.diffmap(adata, color='day_icu_intime')
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> ep.pp.knn_impute(adata)
+        >>> ep.pp.log_norm(adata, offset=1)
+        >>> ep.pp.neighbors(adata)
+        >>> ep.tl.diffmap(adata)
+        >>> ep.pl.diffmap(adata, color='day_icu_intime')
 
     Preview:
         .. image:: /_static/docstring_previews/diffmap.png
     """
     if isinstance(adata, MedCAT):
         if kwargs.get("color"):
             if isinstance(kwargs["color"], str):
@@ -1440,33 +1417,30 @@
         {edges_arrows}
         {scatter_bulk}
         {show_save_ax}
 
     Returns:
         If `show==False` a :class:`~matplotlib.axes.Axes` or a list of it.
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.data.mimic_2(encoded=True)
-            ep.pp.knn_impute(adata)
-            ep.pp.norm_log(adata, offset=1)
-            ep.pp.neighbors(adata)
-            ep.tl.leiden(adata, resolution=0.5, key_added="leiden_0_5")
-            ep.tl.paga(adata, groups="leiden_0_5")
-            ep.pl.paga(
-                adata,
-                color=["leiden_0_5", "day_28_flg"],
-                cmap=ep.pl.Colormaps.grey_red.value,
-                title=["Leiden 0.5", "Died in less than 28 days"],
-            )
-            ep.tl.draw_graph(adata, init_pos="paga")
-            ep.pl.draw_graph(adata, color=["leiden_0_5", "icu_exp_flg"], legend_loc="on data")
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> ep.pp.knn_impute(adata)
+        >>> ep.pp.log_norm(adata, offset=1)
+        >>> ep.pp.neighbors(adata)
+        >>> ep.tl.leiden(adata, resolution=0.5, key_added="leiden_0_5")
+        >>> ep.tl.paga(adata, groups="leiden_0_5")
+        >>> ep.pl.paga(
+        ...     adata,
+        ...     color=["leiden_0_5", "day_28_flg"],
+        ...     cmap=ep.pl.Colormaps.grey_red.value,
+        ...     title=["Leiden 0.5", "Died in less than 28 days"],
+        ... )
+        >>> ep.tl.draw_graph(adata, init_pos="paga")
+        >>> ep.pl.draw_graph(adata, color=["leiden_0_5", "icu_exp_flg"], legend_loc="on data")
 
     Preview:
         .. image:: /_static/docstring_previews/draw_graph_1.png
 
         .. image:: /_static/docstring_previews/draw_graph_2.png
     """
     draw_graph_part = partial(sc.pl.draw_graph, layout=layout)
@@ -1636,25 +1610,22 @@
         {edges_arrows}
         {scatter_bulk}
         {show_save_ax}
 
     Returns:
         If `show==False` a :class:`~matplotlib.axes.Axes` or a list of it.
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.data.mimic_2(encoded=True)
-            ep.pp.knn_impute(adata)
-            ep.pp.norm_log(adata, offset=1)
-            ep.pp.neighbors(adata)
-            ep.tl.umap(adata)
-            ep.pl.embedding(adata, 'X_umap', color='icu_exp_flg')
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> ep.pp.knn_impute(adata)
+        >>> ep.pp.log_norm(adata, offset=1)
+        >>> ep.pp.neighbors(adata)
+        >>> ep.tl.umap(adata)
+        >>> ep.pl.embedding(adata, 'X_umap', color='icu_exp_flg')
 
     Preview:
         .. image:: /_static/docstring_previews/embedding.png
     """
     embedding_partial = partial(
         sc.pl.embedding,
         basis=basis,
@@ -1784,27 +1755,24 @@
         hspace: Adjust the height of the space between multiple panels.
         return_fig: Return the matplotlib figure.\
         {show_save_ax}
 
     Returns:
         If `show==False` a :class:`~matplotlib.axes.Axes` or a list of it.
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.data.mimic_2(encoded=True)
-            ep.pp.knn_impute(adata)
-            ep.pp.norm_log(adata, offset=1)
-            ep.pp.neighbors(adata)
-            ep.tl.umap(adata)
-            ep.tl.leiden(adata, resolution=0.5, key_added="leiden_0_5")
-            ep.tl.embedding_density(adata, groupby='leiden_0_5', key_added='icu_exp_flg')
-            ep.pl.embedding_density(adata, key='icu_exp_flg')
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> ep.pp.knn_impute(adata)
+        >>> ep.pp.log_norm(adata, offset=1)
+        >>> ep.pp.neighbors(adata)
+        >>> ep.tl.umap(adata)
+        >>> ep.tl.leiden(adata, resolution=0.5, key_added="leiden_0_5")
+        >>> ep.tl.embedding_density(adata, groupby='leiden_0_5', key_added='icu_exp_flg')
+        >>> ep.pl.embedding_density(adata, key='icu_exp_flg')
 
     Preview:
         .. image:: /_static/docstring_previews/embedding_density.png
     """
     return sc.pl.embedding_density(
         adata=adata,
         basis=basis,
@@ -1842,29 +1810,26 @@
     Args:
         adata: :class:`~anndata.AnnData` object object containing all observations.
         color_map: Matplotlib Colormap
         palette: Matplotlib color Palette
         show: Whether to show the plot.
         save: Whether to save the plot or a path to save the plot.
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-            import numpy as np
-
-            adata = ep.data.mimic_2(encoded=True)
-            ep.pp.knn_impute(adata)
-            ep.pp.norm_log(adata, offset=1)
-            ep.pp.neighbors(adata, method='gauss')
-            ep.tl.leiden(adata, resolution=0.5, key_added="leiden_0_5")
-            ep.tl.diffmap(adata, n_comps=10)
-            adata.uns['iroot'] = np.flatnonzero(adata.obs['leiden_0_5'] == '0')[0]
-            ep.tl.dpt(adata, n_branchings=3)
-            ep.pl.dpt_groups_pseudotime(adata)
+    Examples:
+        >>> import ehrapy as ep
+        >>> import numpy as np
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> ep.pp.knn_impute(adata)
+        >>> ep.pp.log_norm(adata, offset=1)
+        >>> ep.pp.neighbors(adata, method='gauss')
+        >>> ep.tl.leiden(adata, resolution=0.5, key_added="leiden_0_5")
+        >>> ep.tl.diffmap(adata, n_comps=10)
+        >>> adata.uns['iroot'] = np.flatnonzero(adata.obs['leiden_0_5'] == '0')[0]
+        >>> ep.tl.dpt(adata, n_branchings=3)
+        >>> ep.pl.dpt_groups_pseudotime(adata)
 
     Preview:
         .. image:: /_static/docstring_previews/dpt_groups_pseudotime.png
     """
     sc.pl.dpt_groups_pseudotime(adata=adata, color_map=color_map, palette=palette, show=show, save=save)
 
 
@@ -1880,29 +1845,26 @@
     Args:
         adata: :class:`~anndata.AnnData` object object containing all observations.
         color_map: Matplotlib Colormap
         as_heatmap: Whether to render the plot a heatmap
         show: Whether to show the plot.
         save: Whether to save the plot or a path to save the plot.
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            import numpy as np
-            adata = ep.data.mimic_2(encoded=True)
-            ep.pp.knn_impute(adata)
-            ep.pp.norm_log(adata, offset=1)
-            ep.pp.neighbors(adata, method='gauss')
-            ep.tl.leiden(adata, resolution=0.5, key_added="leiden_0_5")
-            ep.tl.diffmap(adata, n_comps=10)
-            adata.uns['iroot'] = np.flatnonzero(adata.obs['leiden_0_5'] == '0')[0]
-            ep.tl.dpt(adata, n_branchings=3)
-            ep.pl.dpt_timeseries(adata)
+    Examples:
+        >>> import ehrapy as ep
+        >>> import numpy as np
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> ep.pp.knn_impute(adata)
+        >>> ep.pp.log_norm(adata, offset=1)
+        >>> ep.pp.neighbors(adata, method='gauss')
+        >>> ep.tl.leiden(adata, resolution=0.5, key_added="leiden_0_5")
+        >>> ep.tl.diffmap(adata, n_comps=10)
+        >>> adata.uns['iroot'] = np.flatnonzero(adata.obs['leiden_0_5'] == '0')[0]
+        >>> ep.tl.dpt(adata, n_branchings=3)
+        >>> ep.pl.dpt_timeseries(adata)
 
     Preview:
         .. image:: /_static/docstring_previews/dpt_timeseries.png
     """
     sc.pl.dpt_timeseries(adata=adata, color_map=color_map, show=show, save=save, as_heatmap=as_heatmap)
 
 
@@ -2012,31 +1974,28 @@
         show: Whether to show the plot.
         save: Whether or where to save the plot.
 
     Returns:
         A :class:`~matplotlib.axes.Axes` object, if `ax` is `None`, else `None`.
         If `return_data`, return the timeseries data in addition to an axes.
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.data.mimic_2(encoded=True)
-            ep.pp.knn_impute(adata)
-            ep.pp.norm_log(adata, offset=1)
-            ep.pp.neighbors(adata)
-            ep.tl.leiden(adata, resolution=0.5, key_added="leiden_0_5")
-            ep.tl.paga(adata, groups="leiden_0_5")
-            ep.pl.paga(
-                adata,
-                color=["leiden_0_5", "day_28_flg"],
-                cmap=ep.pl.Colormaps.grey_red.value,
-                title=["Leiden 0.5", "Died in less than 28 days"],
-            )
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> ep.pp.knn_impute(adata)
+        >>> ep.pp.log_norm(adata, offset=1)
+        >>> ep.pp.neighbors(adata)
+        >>> ep.tl.leiden(adata, resolution=0.5, key_added="leiden_0_5")
+        >>> ep.tl.paga(adata, groups="leiden_0_5")
+        >>> ep.pl.paga(
+        ...     adata,
+        ...     color=["leiden_0_5", "day_28_flg"],
+        ...     cmap=ep.pl.Colormaps.grey_red.value,
+        ...     title=["Leiden 0.5", "Died in less than 28 days"],
+        ... )
 
     Preview:
         .. image:: /_static/docstring_previews/paga.png
     """
     return sc.pl.paga(
         adata=adata,
         threshold=threshold,
@@ -2288,26 +2247,23 @@
         key: The key of the calculated feature group rankings (default: 'rank_features_groups').
         fontsize: Fontsize for feature names.
         ncols: Number of panels shown per row.
         share_y: Controls if the y-axis of each panels should be shared.
                  But passing `sharey=False`, each panel has its own y-axis range.
         {show_save_ax}
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.data.mimic_2(encoded=True)
-            ep.pp.knn_impute(adata)
-            ep.pp.norm_log(adata, offset=1)
-            ep.pp.neighbors(adata)
-            ep.tl.leiden(adata, resolution=0.15, key_added="leiden_0_5")
-            ep.tl.rank_features_groups(adata, groupby="leiden_0_5")
-            ep.pl.rank_features_groups(adata, key="rank_features_groups")
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.mimic_2(encoded=True)
+        >>> ep.pp.knn_impute(adata)
+        >>> ep.pp.log_norm(adata, offset=1)
+        >>> ep.pp.neighbors(adata)
+        >>> ep.tl.leiden(adata, resolution=0.15, key_added="leiden_0_5")
+        >>> ep.tl.rank_features_groups(adata, groupby="leiden_0_5")
+        >>> ep.pl.rank_features_groups(adata, key="rank_features_groups")
 
     Preview:
         .. image:: /_static/docstring_previews/rank_features_groups.png
     """
     return sc.pl.rank_genes_groups(
         adata=adata,
         groups=groups,
@@ -2355,26 +2311,23 @@
         split: Whether to split the violins or not.
         scale: See :func:`~seaborn.violinplot`.
         strip: Show a strip plot on top of the violin plot.
         jitter: If set to 0, no points are drawn. See :func:`~seaborn.stripplot`.
         size: Size of the jitter points.
         {show_save_ax}
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.data.mimic_2(encoded=True)
-            ep.pp.knn_impute(adata)
-            ep.pp.norm_log(adata, offset=1)
-            ep.pp.neighbors(adata)
-            ep.tl.leiden(adata, resolution=0.15, key_added="leiden_0_5")
-            ep.tl.rank_features_groups(adata, groupby="leiden_0_5")
-            ep.pl.rank_features_groups_violin(adata, key="rank_features_groups", n_features=5)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.mimic_2(encoded=True)
+        >>> ep.pp.knn_impute(adata)
+        >>> ep.pp.log_norm(adata, offset=1)
+        >>> ep.pp.neighbors(adata)
+        >>> ep.tl.leiden(adata, resolution=0.15, key_added="leiden_0_5")
+        >>> ep.tl.rank_features_groups(adata, groupby="leiden_0_5")
+        >>> ep.pl.rank_features_groups_violin(adata, key="rank_features_groups", n_features=5)
 
     Preview:
         .. image:: /_static/docstring_previews/rank_features_groups_violin_1.png
 
         .. image:: /_static/docstring_previews/rank_features_groups_violin_2.png
 
         .. image:: /_static/docstring_previews/rank_features_groups_violin_3.png
@@ -2433,26 +2386,23 @@
         return_fig: Returns :class:`StackedViolin` object. Useful for fine-tuning the plot.
                     Takes precedence over `show=False`.
 
     Returns:
         If `return_fig` is `True`, returns a :class:`StackedViolin` object,
         else if `show` is false, return axes dict
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.data.mimic_2(encoded=True)
-            ep.pp.knn_impute(adata)
-            ep.pp.norm_log(adata, offset=1)
-            ep.pp.neighbors(adata)
-            ep.tl.leiden(adata, resolution=0.15, key_added="leiden_0_5")
-            ep.tl.rank_features_groups(adata, groupby="leiden_0_5")
-            ep.pl.rank_features_groups_stacked_violin(adata, key="rank_features_groups", n_features=5)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> ep.pp.knn_impute(adata)
+        >>> ep.pp.log_norm(adata, offset=1)
+        >>> ep.pp.neighbors(adata)
+        >>> ep.tl.leiden(adata, resolution=0.15, key_added="leiden_0_5")
+        >>> ep.tl.rank_features_groups(adata, groupby="leiden_0_5")
+        >>> ep.pl.rank_features_groups_stacked_violin(adata, key="rank_features_groups", n_features=5)
 
     Preview:
         .. image:: /_static/docstring_previews/rank_features_groups_stacked_violin.png
     """
     return sc.pl.rank_genes_groups_stacked_violin(
         adata=adata,
         groups=groups,
@@ -2493,26 +2443,23 @@
                          use `.var_names` displayed in the plot.
         var_names: Feature names.
         min_logfoldchange: Minimum log fold change to consider.
         key: The key of the calculated feature group rankings (default: 'rank_features_groups').
         show: Whether to show the plot.
         save: Where to save the plot.
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.data.mimic_2(encoded=True)
-            ep.pp.knn_impute(adata)
-            ep.pp.norm_log(adata, offset=1)
-            ep.pp.neighbors(adata)
-            ep.tl.leiden(adata, resolution=0.15, key_added="leiden_0_5")
-            ep.tl.rank_features_groups(adata, groupby="leiden_0_5")
-            ep.pl.rank_features_groups_heatmap(adata, key="rank_features_groups")
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> ep.pp.knn_impute(adata)
+        >>> ep.pp.log_norm(adata, offset=1)
+        >>> ep.pp.neighbors(adata)
+        >>> ep.tl.leiden(adata, resolution=0.15, key_added="leiden_0_5")
+        >>> ep.tl.rank_features_groups(adata, groupby="leiden_0_5")
+        >>> ep.pl.rank_features_groups_heatmap(adata, key="rank_features_groups")
 
     Preview:
         .. image:: /_static/docstring_previews/rank_features_groups_heatmap.png
     """
     return sc.pl.rank_genes_groups_heatmap(
         adata=adata,
         groups=groups,
@@ -2573,24 +2520,21 @@
                     Takes precedence over `show=False`.
 
     Returns:
         If `return_fig` is `True`, returns a :class:`StackedViolin` object,
         else if `show` is false, return axes dict
 
     Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.data.mimic_2(encoded=True)
-            ep.pp.knn_impute(adata)
-            ep.pp.neighbors(adata)
-            ep.tl.leiden(adata, resolution=0.5, key_added="leiden_0_5")
-            ep.tl.rank_features_groups(adata, groupby="leiden_0_5")
-            ep.pl.rank_features_groups_dotplot(adata, key="rank_features_groups", groupby="leiden_0_5")
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> ep.pp.knn_impute(adata)
+        >>> ep.pp.neighbors(adata)
+        >>> ep.tl.leiden(adata, resolution=0.5, key_added="leiden_0_5")
+        >>> ep.tl.rank_features_groups(adata, groupby="leiden_0_5")
+        >>> ep.pl.rank_features_groups_dotplot(adata, key="rank_features_groups", groupby="leiden_0_5")
 
     Preview:
         .. image:: /_static/docstring_previews/rank_features_groups_dotplot.png
     """
     return sc.pl.rank_genes_groups_dotplot(
         adata=adata,
         groups=groups,
@@ -2600,14 +2544,15 @@
         var_names=var_names,
         gene_symbols=feature_symbols,
         min_logfoldchange=min_logfoldchange,
         key=key,
         show=show,
         save=save,
         return_fig=return_fig,
+        colorbar_title="Mean value in group",
         **kwds,
     )
 
 
 def rank_features_groups_matrixplot(
     adata: AnnData,
     groups: str | Sequence[str] = None,
@@ -2653,24 +2598,21 @@
                     Takes precedence over `show=False`.
 
     Returns:
         If `return_fig` is `True`, returns a :class:`MatrixPlot` object,
         else if `show` is false, return axes dict
 
     Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.data.mimic_2(encoded=True)
-            ep.pp.knn_impute(adata)
-            ep.pp.neighbors(adata)
-            ep.tl.leiden(adata, resolution=0.5, key_added="leiden_0_5")
-            ep.tl.rank_features_groups(adata, groupby="leiden_0_5")
-            ep.pl.rank_features_groups_matrixplot(adata, key="rank_features_groups", groupby="leiden_0_5")
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> ep.pp.knn_impute(adata)
+        >>> ep.pp.neighbors(adata)
+        >>> ep.tl.leiden(adata, resolution=0.5, key_added="leiden_0_5")
+        >>> ep.tl.rank_features_groups(adata, groupby="leiden_0_5")
+        >>> ep.pl.rank_features_groups_matrixplot(adata, key="rank_features_groups", groupby="leiden_0_5")
 
     Preview:
         .. image:: /_static/docstring_previews/rank_features_groups_matrixplot.png
 
     """
     return sc.pl.rank_genes_groups_matrixplot(
         adata=adata,
@@ -2713,26 +2655,23 @@
                          use `.var_names` displayed in the plot.
         var_names: Feature names.
         min_logfoldchange: Minimum log fold change to consider.
         key: The key of the calculated feature group rankings (default: 'rank_features_groups').
         show: Whether to show the plot.
         save: Where to save the plot.
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.data.mimic_2(encoded=True)
-            ep.pp.knn_impute(adata)
-            ep.pp.norm_log(adata, offset=1)
-            ep.pp.neighbors(adata)
-            ep.tl.leiden(adata, resolution=0.15, key_added="leiden_0_5")
-            ep.tl.rank_features_groups(adata, groupby="leiden_0_5")
-            ep.pl.rank_features_groups_tracksplot(adata, key="rank_features_groups")
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> ep.pp.knn_impute(adata)
+        >>> ep.pp.log_norm(adata, offset=1)
+        >>> ep.pp.neighbors(adata)
+        >>> ep.tl.leiden(adata, resolution=0.15, key_added="leiden_0_5")
+        >>> ep.tl.rank_features_groups(adata, groupby="leiden_0_5")
+        >>> ep.pl.rank_features_groups_tracksplot(adata, key="rank_features_groups")
 
     Preview:
         .. image:: /_static/docstring_previews/rank_features_groups_tracksplot.png
     """
     return sc.pl.rank_genes_groups_tracksplot(
         adata=adata,
         groups=groups,
```

### Comparing `ehrapy-0.3.0/ehrapy/plot/_survival_analysis.py` & `ehrapy-0.4.0/ehrapy/plot/_survival_analysis.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+from typing import Sequence
 from xmlrpc.client import Boolean
 
 import matplotlib.pyplot as plt
 import numpy as np
 from anndata import AnnData
 from lifelines import KaplanMeierFitter
 from matplotlib.axes import Axes
@@ -27,61 +28,58 @@
     lines_color: list[str] | None | None = None,
     lines_style: list[str] | None | None = None,
     lines_label: list[str] | None | None = None,
     xlim: tuple[float, float] | None = None,
     ylim: tuple[float, float] | None = None,
     show: bool | None = None,
     ax: Axes | None = None,
+    title: str | None = None,
     **kwds,
 ):
     """Plots a Ordinary Least Squares (OLS) Model result, scatter plot, and line plot.
 
     Args:
         adata: :class:`~anndata.AnnData` object object containing all observations.
-        x: x coordinate, for scatter plotting
-        y: y coordinate, for scatter plotting
-        scatter_plot: If True, show scatter plot (default: True)
+        x: x coordinate, for scatter plotting.
+        y: y coordinate, for scatter plotting.
+        scatter_plot: If True, show scatter plot. Defaults to True.
         ols_results: List of RegressionResults from ehrapy.tl.ols. Example: [result_1, result_2]
-        ols_color: List of colors for each ols_results. Example: ['red', 'blue']
-        xlabel: The x-axis label text
-        ylabel: The y-axis label text
-        figsize: Width, height in inches (default: None)
-        lines: List of Tuples of (slope, intercept) or (x, y). Plot lines by slope and intercept or data points. Example: plot two lines (y = x + 2 and y = 2*x + 1): [(1, 2), (2, 1)]
+        ols_color: List of colors for each ols_results. Example: ['red', 'blue'].
+        xlabel: The x-axis label text.
+        ylabel: The y-axis label text.
+        figsize: Width, height in inches. Defaults to None.
+        lines: List of Tuples of (slope, intercept) or (x, y). Plot lines by slope and intercept or data points.
+               Example: plot two lines (y = x + 2 and y = 2*x + 1): [(1, 2), (2, 1)]
         lines_color: List of colors for each line. Example: ['red', 'blue']
         lines_style: List of line styles for each line. Example: ['-', '--']
         lines_label: List of line labels for each line. Example: ['Line1', 'Line2']
-        xlim: Set the x-axis view limits. Required for only ploting lines using slope and intercept.
-        ylim: Set the y-axis view limits. Required for only ploting lines using slope and intercept.
+        xlim: Set the x-axis view limits. Required for only plotting lines using slope and intercept.
+        ylim: Set the y-axis view limits. Required for only plotting lines using slope and intercept.
         show: Show the plot, do not return axis.
         ax: A matplotlib axes object. Only works if plotting a single component.
-    Example:
-        .. code-block:: python
+        title: Set the title of the plot.
 
-            # Scatter plot and OLS regression plot
-            import ehrapy as ep
-            adata = ep.data.mimic_2(encoded=False)
-            co2_lm_result = ep.tl.ols(adata, var_names=['pco2_first', 'tco2_first'], formula='tco2_first ~ pco2_first', missing="drop").fit()
-            ep.pl.ols(adata, x='pco2_first', y='tco2_first', ols_results=[co2_lm_result], ols_color=['red'], xlabel="PCO2", ylabel="TCO2")
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.mimic_2(encoded=False)
+        >>> co2_lm_result = ep.tl.ols(adata, var_names=['pco2_first', 'tco2_first'], formula='tco2_first ~ pco2_first', missing="drop").fit()
+        >>> ep.pl.ols(adata, x='pco2_first', y='tco2_first', ols_results=[co2_lm_result], ols_color=['red'], xlabel="PCO2", ylabel="TCO2")
 
         .. image:: /_static/docstring_previews/ols_plot_1.png
 
-        .. code-block:: python
-
-            # Scatter plot and line plot
-            import ehrapy as ep
-            adata = ep.data.mimic_2(encoded=False)
-            ep.pl.ols(adata, x='pco2_first', y='tco2_first', lines=[(0.25, 10), (0.3, 20)], lines_color=['red', 'blue'], lines_style=['-', ':'], lines_label=['Line1', 'Line2'])
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.mimic_2(encoded=False)
+        >>> ep.pl.ols(adata, x='pco2_first', y='tco2_first', lines=[(0.25, 10), (0.3, 20)],
+        >>>           lines_color=['red', 'blue'], lines_style=['-', ':'], lines_label=['Line1', 'Line2'])
 
         .. image:: /_static/docstring_previews/ols_plot_2.png
 
-        .. code-block:: python
-
-            # Line plot only
-            import ehrapy as ep
-            ep.pl.ols(lines=[(0.25, 10), (0.3, 20)], lines_color=['red', 'blue'], lines_style=['-', ':'], lines_label=['Line1', 'Line2'], xlim=(0, 150), ylim=(0, 50))
+        >>> import ehrapy as ep
+        >>> ep.pl.ols(lines=[(0.25, 10), (0.3, 20)], lines_color=['red', 'blue'], lines_style=['-', ':'],
+        >>>           lines_label=['Line1', 'Line2'], xlim=(0, 150), ylim=(0, 50))
 
         .. image:: /_static/docstring_previews/ols_plot_3.png
     """
     if ax is None:
         _, ax = plt.subplots(figsize=figsize)
     if xlim is not None:
         plt.xlim(xlim)
@@ -111,83 +109,89 @@
                 line_x = np.array(ax.get_xlim())
                 line_y = a * line_x + b
                 ax.plot(line_x, line_y, linestyle=lines_style[i], color=lines_color[i], label=lines_label[i])
             else:
                 ax.plot(a, b, lines_style[i], color=lines_color[i], label=lines_label[i])
     plt.xlabel(xlabel)
     plt.ylabel(ylabel)
+    if title:
+        plt.title(title)
     if lines_label is not None and lines_label[0] is not None:
         plt.legend()
+
     if not show:
         return ax
 
 
 def kmf(
-    kmfs: list[KaplanMeierFitter] = None,
+    kmfs: Sequence[KaplanMeierFitter] = None,
     ci_alpha: list[float] | None = None,
     ci_force_lines: list[Boolean] | None = None,
     ci_show: list[Boolean] | None = None,
     ci_legend: list[Boolean] | None = None,
     at_risk_counts: list[Boolean] | None = None,
     color: list[str] | None | None = None,
     grid: Boolean | None = False,
     xlim: tuple[float, float] | None = None,
     ylim: tuple[float, float] | None = None,
     xlabel: str | None = None,
     ylabel: str | None = None,
     figsize: tuple[float, float] | None = None,
     show: bool | None = None,
+    title: str | None = None,
 ):
     """Plots a pretty figure of the Fitted KaplanMeierFitter model
 
     See https://lifelines.readthedocs.io/en/latest/fitters/univariate/KaplanMeierFitter.html
 
     Args:
-        kmfs: Lists of fitted KaplanMeierFitter object.
-        ci_alpha: The transparency level of the confidence interval. If more than one kmfs, this should be a list (default: 0.3).
-        ci_force_lines: Force the confidence intervals to be line plots (versus default shaded areas). If more than one kmfs, this should be a list (default: False).
-        ci_show: Show confidence intervals. If more than one kmfs, this should be a list (default: True).
-        ci_legend: If ci_force_lines is True, this is a boolean flag to add the lines' labels to the legend. If more than one kmfs, this should be a list (default: False).
-        at_risk_counts: Show group sizes at time points. If more than one kmfs, this should be a list (default: False).
+        kmfs: Iterables of fitted KaplanMeierFitter objects.
+        ci_alpha: The transparency level of the confidence interval. If more than one kmfs, this should be a list. Defaults to 0.3.
+        ci_force_lines: Force the confidence intervals to be line plots (versus default shaded areas).
+                        If more than one kmfs, this should be a list. Defaults to False .
+        ci_show: Show confidence intervals. If more than one kmfs, this should be a list. Defaults to True .
+        ci_legend: If ci_force_lines is True, this is a boolean flag to add the lines' labels to the legend.
+                   If more than one kmfs, this should be a list. Defaults to False .
+        at_risk_counts: Show group sizes at time points. If more than one kmfs, this should be a list. Defaults to False.
         color: List of colors for each kmf. If more than one kmfs, this should be a list.
         grid: If True, plot grid lines.
         xlim: Set the x-axis view limits.
         ylim: Set the y-axis view limits.
         xlabel: The x-axis label text.
         ylabel: The y-axis label text.
-        figsize: Width, height in inches (default: None).
+        figsize: Width, height in inches. Defaults to None .
         show: Show the plot, do not return axis.
+        title: Set the title of the plot.
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-            import numpy as np
-            adata = ep.dt.mimic_2(encoded=False)
-            # Because in MIMIC-II database, `censor_fl` is censored or death (binary: 0 = death, 1 = censored).
-            # While in KaplanMeierFitter, `event_observed` is True if the the death was observed, False if the event was lost (right-censored).
-            # So we need to flip `censor_fl` when pass `censor_fl` to KaplanMeierFitter
-            adata[:, ['censor_flg']].X = np.where(adata[:, ['censor_flg']].X == 0, 1, 0)
-            kmf = ep.tl.kmf(adata[:, ['mort_day_censored']].X, adata[:, ['censor_flg']].X)
-            ep.pl.kmf([kmf], color=['r'], xlim=[0, 700], ylim=[0, 1], xlabel="Days", ylabel="Proportion Survived", show=True)
+    Examples:
+        >>> import ehrapy as ep
+        >>> import numpy as np
+        >>> adata = ep.dt.mimic_2(encoded=False)
+
+        # Because in MIMIC-II database, `censor_fl` is censored or death (binary: 0 = death, 1 = censored).
+        # While in KaplanMeierFitter, `event_observed` is True if the the death was observed, False if the event was lost (right-censored).
+        # So we need to flip `censor_fl` when pass `censor_fl` to KaplanMeierFitter
+
+        >>> adata[:, ['censor_flg']].X = np.where(adata[:, ['censor_flg']].X == 0, 1, 0)
+        >>> kmf = ep.tl.kmf(adata[:, ['mort_day_censored']].X, adata[:, ['censor_flg']].X)
+        >>> ep.pl.kmf([kmf], color=['r'], xlim=[0, 700], ylim=[0, 1], xlabel="Days", ylabel="Proportion Survived", show=True)
 
         .. image:: /_static/docstring_previews/kmf_plot_1.png
 
-        .. code-block:: python
-
-            T = adata[:, ['mort_day_censored']].X
-            E = adata[:, ['censor_flg']].X
-            groups = adata[:, ['service_unit']].X
-            ix1 = (groups == 'FICU')
-            ix2 = (groups == 'MICU')
-            ix3 = (groups == 'SICU')
-            kmf_1 = ep.tl.kmf(T[ix1], E[ix1], label='FICU')
-            kmf_2 = ep.tl.kmf(T[ix2], E[ix2], label='MICU')
-            kmf_3 = ep.tl.kmf(T[ix3], E[ix3], label='SICU')
-            ep.pl.kmf([kmf_1, kmf_2, kmf_3], ci_show=[False,False,False], color=['k','r', 'g'], xlim=[0, 750], ylim=[0, 1], xlabel="Days", ylabel="Proportion Survived")
+        >>> T = adata[:, ['mort_day_censored']].X
+        >>> E = adata[:, ['censor_flg']].X
+        >>> groups = adata[:, ['service_unit']].X
+        >>> ix1 = (groups == 'FICU')
+        >>> ix2 = (groups == 'MICU')
+        >>> ix3 = (groups == 'SICU')
+        >>> kmf_1 = ep.tl.kmf(T[ix1], E[ix1], label='FICU')
+        >>> kmf_2 = ep.tl.kmf(T[ix2], E[ix2], label='MICU')
+        >>> kmf_3 = ep.tl.kmf(T[ix3], E[ix3], label='SICU')
+        >>> ep.pl.kmf([kmf_1, kmf_2, kmf_3], ci_show=[False,False,False], color=['k','r', 'g'],
+        >>>           xlim=[0, 750], ylim=[0, 1], xlabel="Days", ylabel="Proportion Survived")
 
         .. image:: /_static/docstring_previews/kmf_plot_2.png
     """
     if ci_alpha is None:
         ci_alpha = [0.3] * len(kmfs)
     if ci_force_lines is None:
         ci_force_lines = [False] * len(kmfs)
@@ -196,14 +200,15 @@
     if ci_legend is None:
         ci_legend = [False] * len(kmfs)
     if at_risk_counts is None:
         at_risk_counts = [False] * len(kmfs)
     if color is None:
         color = [None] * len(kmfs)
     plt.figure(figsize=figsize)
+
     for i, kmf in enumerate(kmfs):
         if i == 0:
             ax = kmf.plot_survival_function(
                 ci_alpha=ci_alpha[i],
                 ci_force_lines=ci_force_lines[i],
                 ci_show=ci_show[i],
                 ci_legend=ci_legend[i],
@@ -221,9 +226,12 @@
                 color=color[i],
             )
     ax.grid(grid)
     plt.xlim(xlim)
     plt.ylim(ylim)
     plt.xlabel(xlabel)
     plt.ylabel(ylabel)
+    if title:
+        plt.title(title)
+
     if not show:
         return ax
```

### Comparing `ehrapy-0.3.0/ehrapy/plot/_util.py` & `ehrapy-0.4.0/ehrapy/plot/_util.py`

 * *Files identical despite different names*

### Comparing `ehrapy-0.3.0/ehrapy/preprocessing/__init__.py` & `ehrapy-0.4.0/ehrapy/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `ehrapy-0.3.0/ehrapy/preprocessing/_data_imputation.py` & `ehrapy-0.4.0/ehrapy/preprocessing/_data_imputation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,57 @@
 from __future__ import annotations
 
+from typing import Iterable, Literal
+
 import numpy as np
 import pandas as pd
 from anndata import AnnData
 from rich import print
 from rich.progress import Progress, SpinnerColumn
 from sklearn.experimental import enable_iterative_imputer  # noqa: F401
 from sklearn.impute import SimpleImputer
 from sklearn.preprocessing import OrdinalEncoder
 
 from ehrapy import logging as logg
 from ehrapy import settings
 from ehrapy.anndata.anndata_ext import get_column_indices
-from ehrapy.core.tool_available import check_module_importable
+from ehrapy.core._tool_available import _check_module_importable
 
 
 def explicit_impute(
     adata: AnnData,
     replacement: (str | int) | (dict[str, str | int]),
     impute_empty_strings: bool = True,
     warning_threshold: int = 30,
     copy: bool = False,
 ) -> AnnData:
-    """Replaces all missing values in all or the specified columns with the passed value
+    """Replaces all missing values in all columns or a subset of columns specified by the user with the passed replacement value.
 
     There are two scenarios to cover:
     1. Replace all missing values with the specified value.
     2. Replace all missing values in a subset of columns with a specified value per column.
 
     Args:
         adata: :class:`~anndata.AnnData` object containing X to impute values in.
-        replacement: Value to use as replacement or optionally keys to indicate which columns to replace with which value.
-        impute_empty_strings: Whether to also impute empty strings.
-        warning_threshold: Threshold of percentage of missing values to display a warning for (default: 30)
-        copy: Whether to return a copy with the imputed data.
+        replacement: The value to replace missing values with. If a dictionary is provided, the keys represent column
+                     names and the values represent replacement values for those columns.
+        impute_empty_strings: If True, empty strings are also replaced. Defaults to True.
+        warning_threshold: Threshold of percentage of missing values to display a warning for. Defaults to 30.
+        copy: If True, returns a modified copy of the original AnnData object. If False, modifies the object in place.
 
     Returns:
-        :class:`~anndata.AnnData` object with imputed X
-
-    Example:
-        .. code-block:: python
+        If copy is True, a modified copy of the original AnnData object with imputed X.
+        If copy is False, the original AnnData object is modified in place.
 
-            import ehrapy as ep
+    Examples:
+        Replace all missing values in adata with the value 0:
 
-            adata = ep.dt.mimic_2(encoded=True)
-            ep.pp.explicit_impute(adata, replacement=0)
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.mimic_2(encoded=True)
+        >>> ep.pp.explicit_impute(adata, replacement=0)
     """
     if copy:  # pragma: no cover
         adata = adata.copy()
 
     if isinstance(replacement, int) or isinstance(replacement, str):
         _warn_imputation_threshold(adata, var_names=list(adata.var_names), threshold=warning_threshold)
     else:
@@ -74,15 +77,15 @@
                     _replace_explicit(adata.X[:, idx : idx + 1], imputation_value, impute_empty_strings)
                 else:
                     print(f"[bold yellow]No replace value passed and found for var [not bold green]{column_name}.")
             logg.debug(
                 f"Imputed missing values in columns `{replacement.keys()}` by `{replacement.values()}` respectively."
             )
         else:
-            raise ReplacementDatatypeError(  # pragma: no cover
+            raise ValueError(  # pragma: no cover
                 f"Type {type(replacement)} is not a valid datatype for replacement parameter. Either use int, str or a dict!"
             )
 
     if copy:
         return adata
 
 
@@ -109,43 +112,43 @@
     imputation_value = replacement.get("default")
     if imputation_value:  # pragma: no cover
         return imputation_value
     else:
         return None
 
 
-# ===================== Simple Imputation =========================
-
-
 def simple_impute(
     adata: AnnData,
-    var_names: list[str] | None = None,
-    strategy: str = "mean",
+    var_names: Iterable[str] | None = None,
+    strategy: Literal["mean", "median", "most_frequent"] = "mean",
     copy: bool = False,
     warning_threshold: int = 30,
 ) -> AnnData:
-    """Impute AnnData object using mean/median/most frequent imputation. This works for numerical data only.
+    """Impute missing values in numerical data using mean/median/most frequent imputation.
 
     Args:
-        adata: The AnnData object to use mean Imputation on
-        var_names: A list of var names indicating which columns to use mean imputation on (if None -> all columns)
-        strategy: Any of mean/median/most_frequent to indicate which strategy to use for simple imputation
-        warning_threshold: Threshold of percentage of missing values to display a warning for (default: 30)
-        copy: Whether to return a copy or act in place
+        adata: The annotated data matrix to impute missing values on.
+        var_names: A list of column names to apply imputation on (if None, impute all columns).
+        strategy: Imputation strategy to use. One of {'mean', 'median', 'most_frequent'}.
+        warning_threshold: Display a warning message if percentage of missing values exceeds this threshold. Defaults to 30.
+        copy:Whether to return a copy of `adata` or modify it inplace. Defaults to False.
 
     Returns:
-        The imputed AnnData object
+        An updated AnnData object with imputed values.
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.dt.mimic_2(encoded=True)
-            ep.pp.simple_impute(adata, strategy="median")
+    Raises:
+        ValueError:
+            If the selected imputation strategy is not applicable to the data.
+        ValueError:
+            If an unknown imputation strategy is provided.
+
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.mimic_2(encoded=True)
+        >>> ep.pp.simple_impute(adata, strategy="median")
     """
     if copy:
         adata = adata.copy()
 
     _warn_imputation_threshold(adata, var_names, threshold=warning_threshold)
 
     with Progress(
@@ -156,83 +159,82 @@
         progress.add_task(f"[blue]Running simple imputation with {strategy}", total=1)
         # Imputation using median and mean strategy works with numerical data only
         if strategy in {"median", "mean"}:
             try:
                 _simple_impute(adata, var_names, strategy)
                 logg.debug(f"Imputed the AnnData object using `{strategy}` Imputation.")
             except ValueError:
-                raise ImputeStrategyNotAvailableError(
+                raise ValueError(
                     f"Can only impute numerical data using {strategy} strategy. Try to restrict imputation"
                     "to certain columns using var_names parameter or use a different mode."
                 )
         # most_frequent imputation works with non numerical data as well
         elif strategy == "most_frequent":
             _simple_impute(adata, var_names, strategy)
             logg.debug("Imputed the AnnData object using `most_frequent` Imputation.")
         # unknown simple imputation strategy
         else:
-            raise UnknownImputeStrategyError(  # pragma: no cover
+            raise ValueError(  # pragma: no cover
                 f"Unknown impute strategy {strategy} for simple Imputation. Choose any of mean, median or most_frequent."
             )
 
     if copy:
         return adata
 
 
-def _simple_impute(adata: AnnData, var_names: list[str] | None, strategy: str) -> None:
+def _simple_impute(adata: AnnData, var_names: Iterable[str] | None, strategy: str) -> None:
     imputer = SimpleImputer(strategy=strategy)
     # impute a subset of columns
     if isinstance(var_names, list):
         column_indices = get_column_indices(adata, var_names)
         adata.X[::, column_indices] = imputer.fit_transform(adata.X[::, column_indices])
     # impute all columns if None passed
     else:
         adata.X = imputer.fit_transform(adata.X)
 
 
-# ===================== KNN Imputation =========================
-
-
 def knn_impute(
     adata: AnnData,
-    var_names: list[str] | None = None,
+    var_names: Iterable[str] | None = None,
     n_neighbours: int = 5,
     copy: bool = False,
     warning_threshold: int = 30,
 ) -> AnnData:
-    """Impute data using the KNN-Imputer.
+    """Imputes missing values in the input AnnData object using K-nearest neighbor imputation.
 
     When using KNN Imputation with mixed data (non-numerical and numerical), encoding using ordinal encoding is required
     since KNN Imputation can only work on numerical data. The encoding itself is just a utility and will be undone once
     imputation ran successfully.
 
-    Args:
-        adata: The AnnData object to use KNN Imputation on
-        var_names: A list of var names indicating which columns to use median imputation on (if None -> all columns)
-        n_neighbours: Number of neighbours to consider while imputing (default: 5)
-        warning_threshold: Threshold of percentage of missing values to display a warning for (default: 30)
-        copy: Whether to return a copy or act in place
-
-    Returns:
-        The imputed (but unencoded) AnnData object
-
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.dt.mimic_2(encoded=True)
-            ep.pp.knn_impute(adata)
+        Args:
+            adata: An annotated data matrix containing gene expression values.
+            var_names: A list of variable names indicating which columns to impute.
+                       If `None`, all columns are imputed. Default is `None`.
+            n_neighbours: Number of neighbors to use when performing the imputation. Defaults to 5.
+            copy: Whether to perform the imputation on a copy of the original `AnnData` object.
+                  If `True`, the original object remains unmodified. Defaults to `False`.
+            warning_threshold: Percentage of missing values above which a warning is issued. Defaults to 30.
+
+        Returns:
+            An updated AnnData object with imputed values.
+
+        Raises:
+            ValueError: If the input data matrix contains only categorical (non-numeric) values.
+
+        Examples:
+            >>> import ehrapy as ep
+            >>> adata = ep.dt.mimic_2(encoded=True)
+            >>> ep.pp.knn_impute(adata)
     """
     if copy:
         adata = adata.copy()
 
     _warn_imputation_threshold(adata, var_names, threshold=warning_threshold)
 
-    if check_module_importable("sklearnex"):  # pragma: no cover
+    if _check_module_importable("sklearnex"):  # pragma: no cover
         from sklearnex import patch_sklearn, unpatch_sklearn
 
         patch_sklearn()
     else:
         print(
             "[bold yellow]scikit-learn-intelex is not available. Install via [blue]pip install scikit-learn-intelex [yellow] for faster imputations."
         )
@@ -257,15 +259,15 @@
             # cast them to int to ensure they can be decoded
             adata.X[::, column_indices] = np.rint(adata.X[::, column_indices]).astype(int)
             # knn imputer transforms X dtype to numerical (encoded), but object is needed for decoding
             adata.X = adata.X.astype("object")
             # decode ordinal encoding to obtain imputed original data
             adata.X[::, column_indices] = enc.inverse_transform(adata.X[::, column_indices])
 
-    if check_module_importable("sklearnex"):  # pragma: no cover
+    if _check_module_importable("sklearnex"):  # pragma: no cover
         unpatch_sklearn()
 
     if var_names:
         logg.debug(
             f"Imputed the columns `{var_names}` in the AnnData object using kNN Imputation with {n_neighbours} neighbours considered."
         )
     elif not var_names:
@@ -273,81 +275,79 @@
             f"Imputed the data in the AnnData object using kNN Imputation with {n_neighbours} neighbours considered."
         )
 
     if copy:
         return adata
 
 
-def _knn_impute(adata: AnnData, var_names: list[str] | None, n_neighbours: int) -> None:
+def _knn_impute(adata: AnnData, var_names: Iterable[str] | None, n_neighbours: int) -> None:
     """Utility function to impute data using KNN-Imputer"""
     from sklearn.impute import KNNImputer
 
     imputer = KNNImputer(n_neighbors=n_neighbours)
 
     if isinstance(var_names, list):
         column_indices = get_column_indices(adata, var_names)
         adata.X[::, column_indices] = imputer.fit_transform(adata.X[::, column_indices])
         # this is required since X dtype has to be numerical in order to correctly round floats
         adata.X = adata.X.astype("float64")
     else:
         adata.X = imputer.fit_transform(adata.X)
 
 
-# ======================  MissForest Impuation =======================
-
-
 def miss_forest_impute(
     adata: AnnData,
     var_names: dict[str, list[str]] | list[str] | None = None,
-    num_initial_strategy: str = "mean",
+    num_initial_strategy: Literal["mean", "median", "most_frequent", "constant"] = "mean",
     max_iter: int = 10,
     n_estimators=100,
     random_state: int = 0,
     warning_threshold: int = 30,
     copy: bool = False,
 ) -> AnnData:
     """Impute data using the MissForest strategy.
 
+    This function uses the MissForest strategy to impute missing values in the data matrix of an AnnData object.
+    The strategy works by fitting a random forest model on each feature containing missing values,
+    and using the trained model to predict the missing values.
+
     See https://academic.oup.com/bioinformatics/article/28/1/112/219101.
     This requires the computation of which columns in X contain numerical only (including NaNs) and which contain non-numerical data.
 
     Args:
         adata: The AnnData object to use MissForest Imputation on.
         var_names: List of columns to impute or a dict with two keys ('numerical' and 'non_numerical') indicating which var
                    contain mixed data and which numerical data only.
-        num_initial_strategy: The initial strategy to replace all missing values with (default: 'mean').
+        num_initial_strategy: The initial strategy to replace all missing numerical values with. Defaults to 'mean'.
         max_iter: The maximum number of iterations if the stop criterion has not been met yet.
         n_estimators: The number of trees to fit for every missing variable. Has a big effect on the run time.
-                      Decrease for faster computations (default: 100).
-        random_state: The random seed for the initialization.
-        warning_threshold: Threshold of percentage of missing values to display a warning for (default: 30).
-        copy: Whether to return a copy or act in place.
+                      Decrease for faster computations. Defaults to 100.
+        random_state: The random seed for the initialization. Defaults to 0.
+        warning_threshold: Threshold of percentage of missing values to display a warning for. Defaults to 30 .
+        copy: Whether to return a copy or act in place. Defaults to False.
 
     Returns:
         The imputed (but unencoded) AnnData object.
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.dt.mimic_2(encoded=True)
-            ep.pp.miss_forest_impute(adata)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.mimic_2(encoded=True)
+        >>> ep.pp.miss_forest_impute(adata)
     """
     if copy:  # pragma: no cover
         adata = adata.copy()
 
     if var_names is None:
         _warn_imputation_threshold(adata, list(adata.var_names), threshold=warning_threshold)
     elif isinstance(var_names, dict):
         _warn_imputation_threshold(adata, var_names.keys(), threshold=warning_threshold)  # type: ignore
     elif isinstance(var_names, list):
         _warn_imputation_threshold(adata, var_names, threshold=warning_threshold)
 
-    if check_module_importable("sklearnex"):  # pragma: no cover
+    if _check_module_importable("sklearnex"):  # pragma: no cover
         from sklearnex import patch_sklearn, unpatch_sklearn
 
         patch_sklearn()
     else:
         print(
             "[bold yellow]scikit-learn-intelex is not available. Install via [blue]pip install scikit-learn-intelex [yellow] for faster imputations."
         )
@@ -384,15 +384,15 @@
             adata.X[::, var_indices] = imp_num.fit_transform(adata.X[::, var_indices])
         elif isinstance(var_names, dict) or var_names is None:
             if var_names:
                 try:
                     non_num_vars = var_names["non_numerical"]
                     num_vars = var_names["numerical"]
                 except KeyError:  # pragma: no cover
-                    raise MissForestKeyError(
+                    raise ValueError(
                         "One or both of your keys provided for var_names are unknown. Only "
                         "numerical and non_numerical are available!"
                     )
                 non_num_indices = get_column_indices(adata, non_num_vars)
                 num_indices = get_column_indices(adata, num_vars)
 
             # infer non numerical and numerical indices automatically
@@ -408,78 +408,73 @@
             # this step is the most expensive one and might extremely slow down the impute process
             if num_indices:
                 adata.X[::, num_indices] = imp_num.fit_transform(adata.X[::, num_indices])
             if non_num_indices:
                 adata.X[::, non_num_indices] = imp_cat.fit_transform(adata.X[::, non_num_indices])
                 adata.X[::, non_num_indices] = enc.inverse_transform(adata.X[::, non_num_indices])
 
-    if check_module_importable("sklearnex"):  # pragma: no cover
+    if _check_module_importable("sklearnex"):  # pragma: no cover
         unpatch_sklearn()
 
     if var_names:
         logg.debug(
             f"Imputed the columns `{var_names}` in the AnnData object with MissForest Imputation using {num_initial_strategy} strategy."
         )
     elif not var_names:
         logg.debug("Imputed the data in the AnnData object using MissForest Imputation.")
 
     if copy:
         return adata
 
 
-# ===================== SoftImpute =========================
-
-
 def soft_impute(
     adata: AnnData,
-    var_names: list[str] | None = None,
+    var_names: Iterable[str] | None = None,
     copy: bool = False,
     warning_threshold: int = 30,
     shrinkage_value: float | None = None,
     convergence_threshold: float = 0.001,
     max_iters: int = 100,
     max_rank: int | None = None,
     n_power_iterations: int = 1,
     init_fill_method: str = "zero",
     min_value: float | None = None,
     max_value: float | None = None,
     normalizer: object | None = None,
-    verbose: bool = True,
+    verbose: bool = False,
 ) -> AnnData:
     """Impute data using the SoftImpute.
 
     See https://github.com/iskandr/fancyimpute/blob/master/fancyimpute/soft_impute.py
     Matrix completion by iterative soft thresholding of SVD decompositions.
 
     Args:
-        adata: The AnnData object to use SoftImpute on.
+        adata: The AnnData object to impute missing values for.
         var_names: A list of var names indicating which columns to impute (if None -> all columns).
         copy: Whether to return a copy or act in place.
-        warning_threshold: Threshold of percentage of missing values to display a warning for (default: 30).
-        shrinkage_value : Value by which we shrink singular values on each iteration. If omitted then the default value will be the maximum singular value of the initialized matrix (zeros for missing values) divided by 50.
+        warning_threshold: Threshold of percentage of missing values to display a warning for. Defaults to 30 .
+        shrinkage_value : Value by which we shrink singular values on each iteration.
+                          If omitted then the default value will be the maximum singular value of the initialized matrix (zeros for missing values) divided by 50.
         convergence_threshold : Minimum ration difference between iterations (as a fraction of the Frobenius norm of the current solution) before stopping.
-        max_iters: Maximum number of SVD iterations.
-        max_rank: Perform a truncated SVD on each iteration with this value as its rank.
-        n_power_iterations: Number of power iterations to perform with randomized SVD.
+        max_iters: Maximum number of SVD iterations. Defaults to 100.
+        max_rank: Perform a truncated SVD on each iteration with this value as its rank. Defaults to None.
+        n_power_iterations: Number of power iterations to perform with randomized SVD. Defaults to 1.
         init_fill_method: How to initialize missing values of data matrix, default is to fill them with zeros.
         min_value: Smallest allowable value in the solution.
         max_value: Largest allowable value in the solution.
         normalizer: Any object (such as BiScaler) with fit() and transform() methods.
-        verbose: Print debugging info.
+        verbose: Print debugging info. Defaults to False.
 
     Returns:
-        The imputed AnnData object
+        The AnnData object with imputed missing values.
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.dt.mimic_2(encoded=True)
-            ep.pp.soft_impute(adata)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.mimic_2(encoded=True)
+        >>> ep.pp.soft_impute(adata)
     """
     if copy:
         adata = adata.copy()
 
     _warn_imputation_threshold(adata, var_names, threshold=warning_threshold)
 
     with Progress(
@@ -537,15 +532,15 @@
         )
 
     return adata
 
 
 def _soft_impute(
     adata: AnnData,
-    var_names: list[str] | None,
+    var_names: Iterable[str] | None,
     shrinkage_value,
     convergence_threshold,
     max_iters,
     max_rank,
     n_power_iterations,
     init_fill_method,
     min_value,
@@ -572,53 +567,71 @@
     if isinstance(var_names, list):
         column_indices = get_column_indices(adata, var_names)
         adata.X[::, column_indices] = imputer.fit_transform(adata.X[::, column_indices])
     else:
         adata.X = imputer.fit_transform(adata.X)
 
 
-# ===================== IterativeSVD =========================
-
-
 def iterative_svd_impute(
     adata: AnnData,
-    var_names: list[str] | None = None,
+    var_names: Iterable[str] | None = None,
     copy: bool = False,
     warning_threshold: int = 30,
     rank: int = 10,
     convergence_threshold: float = 0.00001,
     max_iters: int = 200,
     gradual_rank_increase: bool = True,
-    svd_algorithm: str = "arpack",
-    init_fill_method: str = "zero",
+    svd_algorithm: Literal["arpack", "randomized"] = "arpack",
+    init_fill_method: Literal["zero", "mean", "median"] = "mean",
     min_value: float | None = None,
     max_value: float | None = None,
-    verbose: bool = True,
+    verbose: bool = False,
 ) -> AnnData:
-    """Impute data using the IterativeSVD.
+    """Impute missing values in an AnnData object using the IterativeSVD algorithm.
 
-    See https://github.com/iskandr/fancyimpute/blob/master/fancyimpute/iterative_svd.py
-    Matrix completion by iterative low-rank SVD decomposition.
+    The IterativeSVD algorithm is a matrix completion method based on iterative low-rank singular value decomposition (SVD).
+    This function can impute missing values for numerical and ordinal-encoded data.
 
     Args:
-        adata: The AnnData object to use IterativeSVD on.
-        var_names: A list of var names indicating which columns to impute (if None -> all columns).
-        copy: Whether to return a copy or act in place.
-        warning_threshold: Threshold of percentage of missing values to display a warning for (default: 30).
+        adata: An AnnData object to impute missing values in.
+        var_names: A list of var names indicating which columns to impute. If `None`, all columns will be imputed.
+                   Defaults to None.
+        copy: Whether to return a copy of the AnnData object or act in place. Defaults to False.
+        warning_threshold: Threshold of percentage of missing values to display a warning for. Defaults to 30.
+        rank: Rank of the SVD decomposition. Defaults to 10.
+        convergence_threshold: Convergence threshold for the iterative algorithm.
+                               The algorithm stops when the relative difference in
+                               Frobenius norm between two iterations is less than `convergence_threshold`.
+                               Defaults to 0.00001.
+        max_iters: Maximum number of iterations. The algorithm stops after `max_iters` iterations if it does not converge.
+                   Defaults to 200.
+        gradual_rank_increase: Whether to increase the rank gradually or to use the rank value immediately.
+                               Defaults to True.
+        svd_algorithm: The SVD algorithm to use. Can be one of {'arpack', 'randomized'}. Defaults to `arpack`.
+        init_fill_method: The fill method to use for initializing missing values. Can be one of `{'zero', 'mean', 'median'}`.
+                          Defaults to `mean`.
+        min_value: The minimum value allowed for the imputed data. Any imputed value less than `min_value` is clipped to `min_value`.
+                   Defaults to None.
+        max_value: The maximum value allowed for the imputed data. Any imputed value greater than `max_value` is clipped to `max_value`.
+                   Defaults to None.
+        verbose: Whether to print progress messages during the imputation. Defaults to False.
 
     Returns:
-        The imputed AnnData object
-
-    Example:
-        .. code-block:: python
+        An AnnData object with imputed values.
 
-            import ehrapy as ep
-
-            adata = ep.dt.mimic_2(encoded=True)
-            ep.pp.iterative_svd_impute(adata)
+    Raises:
+        ValueError:
+            If `svd_algorithm` is not one of `{'arpack', 'randomized'}`.
+        ValueError:
+            If `init_fill_method` is not one of `{'zero', 'mean', 'median'}`.
+
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.mimic_2(encoded=True)
+        >>> ep.pp.iterative_svd_impute(adata)
     """
     if copy:
         adata = adata.copy()
 
     _warn_imputation_threshold(adata, var_names, threshold=warning_threshold)
 
     with Progress(
@@ -703,58 +716,65 @@
     if isinstance(var_names, list):
         column_indices = get_column_indices(adata, var_names)
         adata.X[::, column_indices] = imputer.fit_transform(adata.X[::, column_indices])
     else:
         adata.X = imputer.fit_transform(adata.X)
 
 
-# ===================== MatrixFactorization =========================
-
-
 def matrix_factorization_impute(
     adata: AnnData,
-    var_names: list[str] | None = None,
-    copy: bool = False,
+    var_names: Iterable[str] | None = None,
     warning_threshold: int = 30,
     rank: int = 40,
     learning_rate: float = 0.01,
     max_iters: int = 50,
     shrinkage_value: float = 0,
     min_value: float | None = None,
     max_value: float | None = None,
-    verbose: bool = True,
+    verbose: bool = False,
+    copy: bool = False,
 ) -> AnnData:
     """Impute data using the MatrixFactorization.
 
     See https://github.com/iskandr/fancyimpute/blob/master/fancyimpute/matrix_factorization.py
     Train a matrix factorization model to predict empty entries in a matrix.
 
     Args:
+
         adata: The AnnData object to use MatrixFactorization on.
         var_names: A list of var names indicating which columns to impute (if None -> all columns).
-        copy: Whether to return a copy or act in place.
-        warning_threshold: Threshold of percentage of missing values to display a warning for (default: 30).
-        rank: Number of latent factors to use in matrix factorization model
-        learning_rate: Learning rate for optimizer
-        max_iters: Number of max_iters to train for
-        shrinkage_value: Regularization term for sgd penalty
-        min_value: Smallest possible imputed value
-        max_value: Largest possible imputed value
-        verbose: Whether or not to printout training progress
+        warning_threshold: Threshold of percentage of missing values to display a warning for. Defaults to 30 .
+        rank: Number of latent factors to use in the matrix factorization model.
+              It determines the size of the latent feature space that will be used to estimate the missing values.
+              A higher rank will allow for more complex relationships between the features, but it can also lead to overfitting.
+              Defaults to 40.
+        learning_rate: The learning rate is the step size at which the optimization algorithm updates the model parameters during training.
+                       A larger learning rate can lead to faster convergence, but if it is set too high, the optimization can become unstable.
+                       Defaults to 0.01.
+        max_iters: Maximum number of iterations to train the matrix factorization model for.
+                   The algorithm stops once this number of iterations is reached, or if convergence is achieved earlier.
+                   Defaults to 50.
+        shrinkage_value: The shrinkage value is a regularization parameter that controls the amount of shrinkage applied to the estimated values during optimization.
+                         This term is added to the loss function and serves to penalize large values in the estimated matrix.
+                         A higher shrinkage value can help prevent overfitting, but can also lead to underfitting if set too high.
+                         Defaults to 0.
+        min_value: The minimum value allowed for the imputed data. Any imputed value less than `min_value` is clipped to `min_value`.
+                   Defaults to None.
+        max_value: The maximum value allowed for the imputed data. Any imputed value greater than `max_value` is clipped to `max_value`.
+                   Defaults to None.
+        verbose: Whether or not to printout training progress. Defaults to False.
+        copy: Whether to return a copy or act in place. Defaults to False.
 
     Returns:
         The imputed AnnData object
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.dt.mimic_2(encoded=True)
-            ep.pp.matrix_factorization_impute(adata)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.mimic_2(encoded=True)
+        >>> ep.pp.matrix_factorization_impute(adata)
     """
     if copy:
         adata = adata.copy()
 
     _warn_imputation_threshold(adata, var_names, threshold=warning_threshold)
 
     with Progress(
@@ -835,56 +855,50 @@
     if isinstance(var_names, list):
         column_indices = get_column_indices(adata, var_names)
         adata.X[::, column_indices] = imputer.fit_transform(adata.X[::, column_indices])
     else:
         adata.X = imputer.fit_transform(adata.X)
 
 
-# ===================== NuclearNormMinimization =========================
-
-
 def nuclear_norm_minimization_impute(
     adata: AnnData,
-    var_names: list[str] | None = None,
-    copy: bool = False,
+    var_names: Iterable[str] | None = None,
     warning_threshold: int = 30,
     require_symmetric_solution: bool = False,
     min_value: float | None = None,
     max_value: float | None = None,
     error_tolerance: float = 0.0001,
     max_iters: int = 50000,
-    verbose: bool = True,
+    verbose: bool = False,
+    copy: bool = False,
 ) -> AnnData:
     """Impute data using the NuclearNormMinimization.
 
     See https://github.com/iskandr/fancyimpute/blob/master/fancyimpute/nuclear_norm_minimization.py
     Simple implementation of "Exact Matrix Completion via Convex Optimization" by Emmanuel Candes and Benjamin Recht using cvxpy.
 
     Args:
-        adata: The AnnData object to use NuclearNormMinimization on.
-        var_names: A list of var names indicating which columns to impute (if None -> all columns).
-        copy: Whether to return a copy or act in place.
-        warning_threshold: Threshold of percentage of missing values to display a warning for (default: 30).
-        require_symmetric_solution: Add symmetry constraint to convex problem
-        min_value: Smallest possible imputed value
-        max_value: Largest possible imputed value
-        error_tolerance: Degree of error allowed on reconstructed values. If omitted then defaults to 0.0001
-        max_iters: Maximum number of iterations for the convex solver
-        verbose: Print debug info
+        adata: The AnnData object to apply NuclearNormMinimization on.
+        var_names: Var names indicating which columns to impute (if None -> all columns).
+        warning_threshold: Threshold of percentage of missing values to display a warning for. Defaults to 30.
+        require_symmetric_solution: Whether to add a symmetry constraint to the convex problem. Defaults to False.
+        min_value: Smallest possible imputed value. Defaults to None (no minimum value constraint).
+        max_value: Largest possible imputed value. Defaults to None (no maximum value constraint).
+        error_tolerance: Degree of error allowed on reconstructed values. Defaults to 0.0001.
+        max_iters: Maximum number of iterations for the convex solver. Defaults to 50000.
+        verbose: Whether to print debug information. Defaults to False.
+        copy: Whether to return a copy of the AnnData object or act in place. Defaults to False (act in place).
 
     Returns:
-        The imputed AnnData object
-
-    Example:
-        .. code-block:: python
+        The imputed AnnData object.
 
-            import ehrapy as ep
-
-            adata = ep.dt.mimic_2(encoded=True)
-            ep.pp.nuclear_norm_minimization_impute(adata)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.mimic_2(encoded=True)
+        >>> ep.pp.nuclear_norm_minimization_impute(adata)
     """
     if copy:
         adata = adata.copy()
 
     _warn_imputation_threshold(adata, var_names, threshold=warning_threshold)
 
     with Progress(
@@ -961,55 +975,56 @@
     if isinstance(var_names, list):
         column_indices = get_column_indices(adata, var_names)
         adata.X[::, column_indices] = imputer.fit_transform(adata.X[::, column_indices])
     else:
         adata.X = imputer.fit_transform(adata.X)
 
 
-# ===================== miceforest =========================
-
-
 def mice_forest_impute(
     adata: AnnData,
-    var_names: list[str] | None = None,
-    copy: bool = False,
+    var_names: Iterable[str] | None = None,
     warning_threshold: int = 30,
     save_all_iterations: bool = True,
     random_state: int | None = None,
     inplace: bool = False,
     iterations: int = 5,
     variable_parameters: dict | None = None,
     verbose: bool = False,
+    copy: bool = False,
 ) -> AnnData:
     """Impute data using the miceforest.
 
     See https://github.com/AnotherSamWilson/miceforest
     Fast, memory efficient Multiple Imputation by Chained Equations (MICE) with lightgbm.
 
     Args:
-        adata: The AnnData object to use miceforest on.
-        var_names: A list of var names indicating which columns to impute (if None -> all columns).
-        copy: Whether to return a copy or act in place.
-        warning_threshold: Threshold of percentage of missing values to display a warning for (default: 30).
-        save_all_iterations: Save all the imputation values from all iterations, or just the latest. Saving all iterations allows for additional plotting, but may take more memory.
-        random_state: The random_state ensures script reproducibility. It only ensures reproducible results if the same script is called multiple times. It does not guarantee reproducible results at the record level, if a record is imputed multiple different times. If reproducible record-results are desired, a seed must be passed for each record in the random_seed_array parameter.
-        inplace: Using inplace=False returns a copy of the completed data. Since the raw data is already stored in kernel.working_data, you can set inplace=True to complete the data without returning a copy.
-        iterations: The number of iterations to run.
-        variable_parameters: Model parameters can be specified by variable here. Keys should be variable names or indices, and values should be a dict of parameter which should apply to that variable only.
-        verbose: Should information about the process be printed.
-    Returns:
-        The imputed AnnData object
-
-    Example:
-        .. code-block:: python
+        adata: The AnnData object containing the data to impute.
+        var_names: A list of variable names to impute. If None, impute all variables.
+        warning_threshold: Threshold of percentage of missing values to display a warning for.
+                           Defaults to 30.
+        save_all_iterations: Whether to save all imputed values from all iterations or just the latest.
+                             Saving all iterations allows for additional plotting, but may take more memory. Defaults to True.
+        random_state: The random state ensures script reproducibility.
+                      Defaults to None.
+        inplace: If True, modify the input AnnData object in-place and return None.
+                 If False, return a copy of the modified AnnData object. Default is False.
+        iterations: The number of iterations to run. Defaults to 5.
+        variable_parameters: Model parameters can be specified by variable here.
+                             Keys should be variable names or indices, and values should be a dict of parameter which should apply to that variable only.
+                             Defaults to None.
+        verbose: Whether to print information about the imputation process. Defaults to False.
+        copy: Whether to return a copy of the AnnData object or modify it in-place. Defaults to False.
 
-            import ehrapy as ep
+    Returns:
+        The imputed AnnData object.
 
-            adata = ep.dt.mimic_2(encoded=True)
-            ep.pp.miceforest_impute(adata)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.mimic_2(encoded=True)
+        >>> ep.pp.mice_forest_impute(adata)
     """
     if copy:
         adata = adata.copy()
 
     _warn_imputation_threshold(adata, var_names, threshold=warning_threshold)
 
     with Progress(
@@ -1062,26 +1077,25 @@
         )
 
         kernel.mice(iterations=iterations, variable_parameters=variable_parameters, verbose=verbose)
 
         adata.X[::, column_indices] = kernel.complete_data(dataset=0, inplace=inplace)
 
     else:
-
         # Create kernel.
         kernel = mf.ImputationKernel(
             adata.X, datasets=1, save_all_iterations=save_all_iterations, random_state=random_state
         )
 
         kernel.mice(iterations=iterations, variable_parameters=variable_parameters, verbose=verbose)
 
         adata.X = kernel.complete_data(dataset=0, inplace=inplace)
 
 
-def _warn_imputation_threshold(adata: AnnData, var_names: list[str] | None, threshold: int = 30) -> dict[str, int]:
+def _warn_imputation_threshold(adata: AnnData, var_names: Iterable[str] | None, threshold: int = 30) -> dict[str, int]:
     """Warns the user if the more than $threshold percent had to be imputed.
 
     Args:
         adata: The AnnData object to check
         var_names: The var names which were imputed.
         threshold: A percentage value from 0 to 100 used as minimum.
     """
@@ -1126,31 +1140,7 @@
             return True
         return False
     else:
         if not isinstance(val, bool):
             return True
         else:
             return False
-
-
-class MissingImputeValuesError(Exception):
-    pass
-
-
-class ReplacementDatatypeError(Exception):
-    pass
-
-
-class MissingImputationValue(Exception):
-    pass
-
-
-class ImputeStrategyNotAvailableError(Exception):
-    pass
-
-
-class UnknownImputeStrategyError(Exception):
-    pass
-
-
-class MissForestKeyError(Exception):
-    pass
```

### Comparing `ehrapy-0.3.0/ehrapy/preprocessing/_encode.py` & `ehrapy-0.4.0/ehrapy/preprocessing/_encode.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,40 +50,31 @@
         autodetect: Whether to autodetect categorical values that will be encoded.
         encodings: Only needed if autodetect set to False (or False for some columns in case of a :class:`~mudata.MuData` object).
         A dict containing the encoding mode and categorical name for the respective column (for each AnnData object in case of MuData object).
 
     Returns:
         An :class:`~anndata.AnnData` object with the encoded values in X or None (in case of :class:`~mudata.MuData` object).
 
-    Example using autodetect with default label encoding:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.io.read(...)
-            # encode all autodetected (non numerical) columns using label encoding
-            adata_encoded = ep.pp.encode(adata, autodetect=True)
-
-    Example using autodetect with non-default encoding mode:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.io.read(...)
-            # encode all autodetected (non numerical) columns using one hot encoding (this only works for single column encoding modes, not hash encoding)
-            adata_encoded = ep.pp.encode(adata, autodetect=True, 'one_hot_encoding')
-
-    Example using custom encodings per columns:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.io.read(...)
-            # encode col1 and col2 using label encoding and encode col3 using one hot encoding
-            adata_encoded = ep.pp.encode(adata, autodetect=False, {'label_encoding': ['col1', 'col2'], 'one_hot_encoding': ['col3']})
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.io.read(...)
+        >>> # encode all autodetected (non numerical) columns using label encoding
+        >>> adata_encoded = ep.pp.encode(adata, autodetect=True)
+
+    # Example using autodetect with non-default encoding mode:
+        >>> import ehrapy as ep
+        >>> adata = ep.io.read(...)
+        >>> # encode all autodetected (non numerical) columns using one hot encoding (this only works for single column encoding modes, not hash encoding)
+        >>> adata_encoded = ep.pp.encode(adata, autodetect=True, 'one_hot_encoding')
+
+    # Example using custom encodings per columns:
+        >>> import ehrapy as ep
+        >>> adata = ep.io.read(...)
+        >>> # encode col1 and col2 using label encoding and encode col3 using one hot encoding
+        >>> adata_encoded = ep.pp.encode(adata, autodetect=False, {'label_encoding': ['col1', 'col2'], 'one_hot_encoding': ['col3']})
     """
     if isinstance(data, AnnData):
         # basic type checking for passed parameters when encoding a single AnnData object
         if not _check_anndata_input_type(autodetect, encodings):
             raise EncodingInputValueError
         return _encode(adata=data, autodetect=autodetect, encodings=encodings)
     elif isinstance(data, MuData):
@@ -123,21 +114,18 @@
     Args:
         data: The :class:`~anndata.AnnData` or MuData object
         columns: The names of the columns to reset encoding for. Defaults to all columns.
 
     Returns:
         A (partially) encoding reset :class:`~anndata.AnnData` or MuData object
 
-    Example:
-       .. code-block:: python
-
-           import ehrapy as ep
-
-           # adata_encoded is an encoded AnnData object
-           adata_undone = ep.encode.undo_encoding(adata_encoded)
+    Examples:
+        >>> import ehrapy as ep
+        >>> # adata_encoded is an encoded AnnData object
+        >>> adata_undone = ep.encode.undo_encoding(adata_encoded)
     """
     if isinstance(data, AnnData):
         return _undo_encoding(data, columns)
     elif isinstance(data, MuData):
         for adata in data.mod.keys():
             reset_adata = _undo_encoding(data.mod[adata], columns)
             if reset_adata:
@@ -221,29 +209,31 @@
                 encoded_var_names,
                 categoricals_names,
                 progress,
                 task,
             )
             progress.update(task, description="Updating layer originals ...")
             # update layer content with the latest categorical encoding and the old other values
+            logg.info("Encoding strings in X to save to .h5ad. Loading the file will reverse the encoding.")
             updated_layer = _update_layer_after_encoding(
                 adata.layers["original"],
                 encoded_x,
                 encoded_var_names,
                 adata.var_names.to_list(),
                 categoricals_names,
             )
-            progress.update(task, description=f"Finished {encode_mode} of autodetected columns.")
+            progress.update(task, description=f"[bold blue]Finished {encode_mode} of autodetected columns.")
 
             encoded_ann_data = AnnData(
                 encoded_x,
                 obs=adata.obs.copy(),
                 var=dict(var_names=encoded_var_names),
                 uns=orig_uns_copy,
                 layers={"original": updated_layer},
+                dtype=np.float32,
             )
             encoded_ann_data.uns["var_to_encoding"] = {categorical: encode_mode for categorical in categoricals_names}
             encoded_ann_data.uns["encoding_to_var"] = {encode_mode: categoricals_names}
 
             encoded_ann_data.uns["numerical_columns"] = adata.uns["numerical_columns"].copy()
             encoded_ann_data.uns["non_numerical_columns"] = []
 
@@ -296,15 +286,14 @@
         encoded_var_names = adata.var_names.to_list()
         with Progress(
             "[progress.description]{task.description}",
             BarColumn(),
             "[progress.percentage]{task.percentage:>3.0f}%",
             refresh_per_second=1500,
         ) as progress:
-
             for encoding_mode in encodings.keys():  # type: ignore
                 task = progress.add_task(f"[red]Setting up {encoding_mode}", total=1)
                 encode_mode_switcher = {
                     "one_hot_encoding": _one_hot_encoding,
                     "label_encoding": _label_encoding,
                     "count_encoding": _count_encoding,
                     "hash_encoding": _hash_encoding,
@@ -332,14 +321,15 @@
         try:
             encoded_ann_data = AnnData(
                 encoded_x,
                 obs=adata.obs.copy(),
                 var=dict(var_names=encoded_var_names),
                 uns=orig_uns_copy,
                 layers={"original": updated_layer},
+                dtype=np.float32,
             )
             # update current encodings in uns
             encoded_ann_data.uns["var_to_encoding"] = var_to_encoding
 
         # if the user did not pass every non numerical column for encoding, a Anndata object cannot be created
         except ValueError:
             print(
@@ -728,15 +718,15 @@
     logg.debug("Encoding of the AnnData object was reset.")
 
     return AnnData(
         new_x,
         obs=new_obs,
         var=pd.DataFrame(index=new_var_names),
         uns=uns,
-        dtype="object",
+        dtype=np.dtype(object),
         layers={"original": new_x.copy()},
     )
 
 
 def _delete_all_encodings(adata: AnnData) -> tuple[np.ndarray | None, list | None]:
     """Delete all encoded columns and keep track of their indices.
 
@@ -875,15 +865,15 @@
         new: The new AnnData object
         categorical_names: Name of each categorical column
     """
     for idx, var_name in enumerate(original.var_names):
         if var_name in new.obs.columns:
             continue
         elif var_name in categorical_names:
-            new.obs[var_name] = original.X[::, idx : idx + 1]
+            new.obs[var_name] = original.X[::, idx : idx + 1].flatten()
             # note: this will count binary columns (0 and 1 only) as well
             # needed for writing to .h5ad files
             if set(pd.unique(new.obs[var_name])).issubset({False, True, np.NaN}):
                 new.obs[var_name] = new.obs[var_name].astype("bool")
     # get all non bool object columns and cast the to category dtype
     object_columns = list(new.obs.select_dtypes(include="object").columns)
     new.obs[object_columns] = new.obs[object_columns].astype("category")
```

### Comparing `ehrapy-0.3.0/ehrapy/preprocessing/_highly_variable_features.py` & `ehrapy-0.4.0/ehrapy/preprocessing/_highly_variable_features.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,44 @@
-from typing import Literal, Optional
+from __future__ import annotations
 
 import pandas as pd
 import scanpy as sc
 from anndata import AnnData
 
 
 def highly_variable_features(
     adata: AnnData,
-    layer: Optional[str] = None,
+    layer: str | None = None,
     top_features_percentage: float = 0.2,
-    span: Optional[float] = 0.3,
+    span: float | None = 0.3,
     n_bins: int = 20,
-    flavor: Literal["normalized_variance"] = "normalized_variance",
     subset: bool = False,
     inplace: bool = True,
     check_values: bool = True,
-) -> Optional[pd.DataFrame]:
+) -> pd.DataFrame | None:
     """Annotate highly variable features.
 
     Expects count data. A normalized variance for each feature is computed. First, the data
     are standardized (i.e., z-score normalization per feature) with a regularized
     standard deviation. Next, the normalized variance is computed as the variance
     of each feature after the transformation. Features are ranked by the normalized variance.
 
     Args:
         adata: The annotated data matrix of shape `n_obs` × `n_vars`.
-        layer: If provided, use `adata.layers[layer]` for expression values instead of `adata.X`.
-        top_features_percentage: Percentage of highly-variable features to keep.
-        span: The fraction of the data used when estimating the variance in the loess model fit.
-        n_bins: Number of bins for binning. Normalization is done with respect to each bin. If just a single observation falls into a bin, the normalized dispersion is artificially set to 1. You'll be informed about this if you set `settings.verbosity = 4`.
-        flavor: Choose the flavor for identifying highly variable features.
+        layer: If provided, use `adata.layers[layer]` for expression values instead of `adata.X`. Defaults to None .
+        top_features_percentage: Percentage of highly-variable features to keep. Defaults to 0.2 .
+        span: The fraction of the data used when estimating the variance in the loess model fit. Defaults to 0.3 .
+        n_bins: Number of bins for binning. Normalization is done with respect to each bin.
+                If just a single observation falls into a bin, the normalized dispersion is artificially set to 1.
+                You'll be informed about this if you set `settings.verbosity = 4`. Defaults to 20 .
         subset: Inplace subset to highly-variable features if `True` otherwise merely indicate highly variable features.
-        inplace: Whether to place calculated metrics in `.var` or return them.
+                Defaults to False .
+        inplace: Whether to place calculated metrics in `.var` or return them. Defaults to True .
         check_values: Check if counts in selected layer are integers. A Warning is returned if set to True.
+                      Defaults to True .
 
     Returns:
         Depending on `inplace` returns calculated metrics (:class:`~pandas.DataFrame`) or
         updates `.var` with the following fields
 
     highly_variable : bool
         boolean indicator of highly-variable features
@@ -46,19 +48,19 @@
         variance per feature
     **variances_norm**
         normalized variance per feature, averaged in the case of multiple batches
     highly_variable_rank : float
         rank of the feature according to normalized variance, median rank in the case of multiple batches
     """
     n_top_features = int(top_features_percentage * len(adata.var))
-    if flavor == "normalized_variance":
-        return sc.pp.highly_variable_genes(
-            adata=adata,
-            layer=layer,
-            n_top_genes=n_top_features,
-            span=span,
-            n_bins=n_bins,
-            flavor="seurat_v3",
-            subset=subset,
-            inplace=inplace,
-            check_values=check_values,
-        )
+
+    return sc.pp.highly_variable_genes(
+        adata=adata,
+        layer=layer,
+        n_top_genes=n_top_features,
+        span=span,
+        n_bins=n_bins,
+        flavor="seurat_v3",
+        subset=subset,
+        inplace=inplace,
+        check_values=check_values,
+    )
```

### Comparing `ehrapy-0.3.0/ehrapy/preprocessing/_normalization.py` & `ehrapy-0.4.0/ehrapy/preprocessing/_normalization.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,55 +2,53 @@
 
 import numpy as np
 from anndata import AnnData
 from sklearn.preprocessing import maxabs_scale, minmax_scale, power_transform, quantile_transform, robust_scale, scale
 
 from ehrapy import logging as logg
 from ehrapy.anndata.anndata_ext import (
+    _get_column_values,
     assert_numeric_vars,
     get_column_indices,
-    get_column_values,
     get_numeric_vars,
     set_numeric_vars,
 )
 
 
 def scale_norm(adata: AnnData, vars: str | list[str] | None = None, copy: bool = False, **kwargs) -> AnnData | None:
     """Apply scaling normalization.
 
     Functionality is provided by :func:`~sklearn.preprocessing.scale`, see https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.scale.html for details.
 
     Args:
         adata: :class:`~anndata.AnnData` object containing X to normalize values in. Must already be encoded using :func:`~ehrapy.preprocessing.encode`.
-        vars: List of the names of the numeric variables to normalize. If None (default) all numeric variables will be normalized.
-        copy: Whether to return a copy or act in place (default: False)
+        vars: List of the names of the numeric variables to normalize.
+              If None all numeric variables will be normalized. Defaults to None .
+        copy: Whether to return a copy or act in place . Defaults to False .
         **kwargs: Additional arguments passed to :func:`~sklearn.preprocessing.scale`
 
     Returns:
         :class:`~anndata.AnnData` object with normalized X. Also stores a record of applied normalizations as a dictionary in adata.uns["normalization"].
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.data.mimic_2(encode=True)
-            adata_norm = ep.pp.scale_norm(adata, copy=True)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> adata_norm = ep.pp.scale_norm(adata, copy=True)
     """
     if isinstance(vars, str):
         vars = [vars]
     if vars is None:
         vars = get_numeric_vars(adata)
     else:
         assert_numeric_vars(adata, vars)
 
     adata = _prep_adata_norm(adata, copy)
 
     var_idx = get_column_indices(adata, vars)
-    var_values = get_column_values(adata, var_idx)
+    var_values = _get_column_values(adata, var_idx)
 
     var_values = scale(var_values, **kwargs)
 
     set_numeric_vars(adata, var_values, vars)
 
     _record_norm(adata, vars, "scale")
 
@@ -58,44 +56,45 @@
 
     return adata
 
 
 def minmax_norm(adata: AnnData, vars: str | list[str] | None = None, copy: bool = False, **kwargs) -> AnnData | None:
     """Apply min-max normalization.
 
-    Functionality is provided by :func:`~sklearn.preprocessing.minmax_scale`, see https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.minmax_scale.html for details.
+    Functionality is provided by :func:`~sklearn.preprocessing.minmax_scale`,
+    see https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.minmax_scale.html for details.
 
     Args:
-        adata: :class:`~anndata.AnnData` object containing X to normalize values in. Must already be encoded using :func:`~ehrapy.preprocessing.encode`.
-        vars: List of the names of the numeric variables to normalize. If None (default) all numeric variables will be normalized.
-        copy: Whether to return a copy or act in place (default: False)
+        adata: :class:`~anndata.AnnData` object containing X to normalize values in.
+               Must already be encoded using :func:`~ehrapy.preprocessing.encode`.
+        vars: List of the names of the numeric variables to normalize.
+              If None all numeric variables will be normalized. Defaults to False .
+        copy: Whether to return a copy or act in place. Defaults to False .
         **kwargs: Additional arguments passed to :func:`~sklearn.preprocessing.minmax_scale`
 
     Returns:
-        :class:`~anndata.AnnData` object with normalized X. Also stores a record of applied normalizations as a dictionary in adata.uns["normalization"].
+        :class:`~anndata.AnnData` object with normalized X.
+        Also stores a record of applied normalizations as a dictionary in adata.uns["normalization"].
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.data.mimic_2(encode=True)
-            adata_norm = ep.pp.minmax_norm(adata, copy=True)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> adata_norm = ep.pp.minmax_norm(adata, copy=True)
     """
     if isinstance(vars, str):
         vars = [vars]
     if vars is None:
         vars = get_numeric_vars(adata)
     else:
         assert_numeric_vars(adata, vars)
 
     adata = _prep_adata_norm(adata, copy)
 
     var_idx = get_column_indices(adata, vars)
-    var_values = get_column_values(adata, var_idx)
+    var_values = _get_column_values(adata, var_idx)
 
     var_values = minmax_scale(var_values, **kwargs)
 
     set_numeric_vars(adata, var_values, vars)
 
     _record_norm(adata, vars, "minmax")
 
@@ -103,43 +102,44 @@
 
     return adata
 
 
 def maxabs_norm(adata: AnnData, vars: str | list[str] | None = None, copy: bool = False) -> AnnData | None:
     """Apply max-abs normalization.
 
-    Functionality is provided by :func:`~sklearn.preprocessing.maxabs_scale`, see https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.maxabs_scale.html for details.
+    Functionality is provided by :func:`~sklearn.preprocessing.maxabs_scale`,
+    see https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.maxabs_scale.html for details.
 
     Args:
-        adata: :class:`~anndata.AnnData` object containing X to normalize values in. Must already be encoded using :func:`~ehrapy.preprocessing.encode`.
-        vars: List of the names of the numeric variables to normalize. If None (default) all numeric variables will be normalized.
-        copy: Whether to return a copy or act in place (default: False)
+        adata: :class:`~anndata.AnnData` object containing X to normalize values in.
+               Must already be encoded using :func:`~ehrapy.preprocessing.encode`.
+        vars: List of the names of the numeric variables to normalize.
+              If None all numeric variables will be normalized. Defaults to None .
+        copy: Whether to return a copy or act in place. Defaults to False .
 
     Returns:
-        :class:`~anndata.AnnData` object with normalized X. Also stores a record of applied normalizations as a dictionary in adata.uns["normalization"].
-
-    Example:
-        .. code-block:: python
+        :class:`~anndata.AnnData` object with normalized X.
+        Also stores a record of applied normalizations as a dictionary in adata.uns["normalization"].
 
-            import ehrapy as ep
-
-            adata = ep.data.mimic_2(encode=True)
-            adata_norm = ep.pp.maxabs_norm(adata, copy=True)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> adata_norm = ep.pp.maxabs_norm(adata, copy=True)
     """
     if isinstance(vars, str):
         vars = [vars]
     if vars is None:
         vars = get_numeric_vars(adata)
     else:
         assert_numeric_vars(adata, vars)
 
     adata = _prep_adata_norm(adata, copy)
 
     var_idx = get_column_indices(adata, vars)
-    var_values = get_column_values(adata, var_idx)
+    var_values = _get_column_values(adata, var_idx)
 
     var_values = maxabs_scale(var_values)
 
     set_numeric_vars(adata, var_values, vars)
 
     _record_norm(adata, vars, "maxabs")
 
@@ -149,44 +149,45 @@
 
 
 def robust_scale_norm(
     adata: AnnData, vars: str | list[str] | None = None, copy: bool = False, **kwargs
 ) -> AnnData | None:
     """Apply robust scaling normalization.
 
-    Functionality is provided by :func:`~sklearn.preprocessing.robust_scale`, see https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.robust_scale.html for details.
+    Functionality is provided by :func:`~sklearn.preprocessing.robust_scale`,
+    see https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.robust_scale.html for details.
 
     Args:
-        adata: :class:`~anndata.AnnData` object containing X to normalize values in. Must already be encoded using :func:`~ehrapy.preprocessing.encode`.
-        vars: List of the names of the numeric variables to normalize. If None (default) all numeric variables will be normalized.
-        copy: Whether to return a copy or act in place (default: False)
+        adata: :class:`~anndata.AnnData` object containing X to normalize values in.
+               Must already be encoded using :func:`~ehrapy.preprocessing.encode`.
+        vars: List of the names of the numeric variables to normalize.
+              If None all numeric variables will be normalized. Defaults to None .
+        copy: Whether to return a copy or act in place. Defaults to False .
         **kwargs: Additional arguments passed to :func:`~sklearn.preprocessing.robust_scale`
 
     Returns:
-        :class:`~anndata.AnnData` object with normalized X. Also stores a record of applied normalizations as a dictionary in adata.uns["normalization"].
-
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
+        :class:`~anndata.AnnData` object with normalized X.
+        Also stores a record of applied normalizations as a dictionary in adata.uns["normalization"].
 
-            adata = ep.data.mimic_2(encode=True)
-            adata_norm = ep.pp.robust_scale_norm(adata, copy=True)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> adata_norm = ep.pp.robust_scale_norm(adata, copy=True)
     """
     if isinstance(vars, str):
         vars = [vars]
     if vars is None:
         vars = get_numeric_vars(adata)
     else:
         assert_numeric_vars(adata, vars)
 
     adata = _prep_adata_norm(adata, copy)
 
     var_idx = get_column_indices(adata, vars)
-    var_values = get_column_values(adata, var_idx)
+    var_values = _get_column_values(adata, var_idx)
 
     var_values = robust_scale(var_values, **kwargs)
 
     set_numeric_vars(adata, var_values, vars)
 
     _record_norm(adata, vars, "robust_scale")
 
@@ -194,44 +195,44 @@
 
     return adata
 
 
 def quantile_norm(adata: AnnData, vars: str | list[str] | None = None, copy: bool = False, **kwargs) -> AnnData | None:
     """Apply quantile normalization.
 
-    Functionality is provided by ~sklearn.preprocessing.quantile_transform, see https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.quantile_transform.html for details.
+    Functionality is provided by ~sklearn.preprocessing.quantile_transform,
+    see https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.quantile_transform.html for details.
 
     Args:
         adata: :class:`~anndata.AnnData` object containing X to normalize values in. Must already be encoded using ~ehrapy.preprocessing.encode.encode.
-        vars: List of the names of the numeric variables to normalize. If None (default) all numeric variables will be normalized.
-        copy: Whether to return a copy or act in place (default: False)
+        vars: List of the names of the numeric variables to normalize.
+              If None all numeric variables will be normalized. Defaults to None .
+        copy: Whether to return a copy or act in place. Defaults to False .
         **kwargs: Additional arguments passed to :func:`~sklearn.preprocessing.quantile_transform`
 
     Returns:
-        :class:`~anndata.AnnData` object with normalized X. Also stores a record of applied normalizations as a dictionary in adata.uns["normalization"].
-
-    Example:
-        .. code-block:: python
+        :class:`~anndata.AnnData` object with normalized X.
+        Also stores a record of applied normalizations as a dictionary in adata.uns["normalization"].
 
-            import ehrapy as ep
-
-            adata = ep.data.mimic_2(encode=True)
-            adata_norm = ep.pp.quantile_norm(adata, copy=True)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> adata_norm = ep.pp.quantile_norm(adata, copy=True)
     """
     if isinstance(vars, str):
         vars = [vars]
     if vars is None:
         vars = get_numeric_vars(adata)
     else:
         assert_numeric_vars(adata, vars)
 
     adata = _prep_adata_norm(adata, copy)
 
     var_idx = get_column_indices(adata, vars)
-    var_values = get_column_values(adata, var_idx)
+    var_values = _get_column_values(adata, var_idx)
 
     var_values = quantile_transform(var_values, **kwargs)
 
     set_numeric_vars(adata, var_values, vars)
 
     _record_norm(adata, vars, "quantile")
 
@@ -239,44 +240,45 @@
 
     return adata
 
 
 def power_norm(adata: AnnData, vars: str | list[str] | None = None, copy: bool = False, **kwargs) -> AnnData | None:
     """Apply power transformation normalization.
 
-    Functionality is provided by :func:`~sklearn.preprocessing.power_transform`, see https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.power_transform.html for details.
+    Functionality is provided by :func:`~sklearn.preprocessing.power_transform`,
+    see https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.power_transform.html for details.
 
     Args:
-        adata: :class:`~anndata.AnnData` object containing X to normalize values in. Must already be encoded using :func:`~ehrapy.preprocessing.encode`.
-        vars: List of the names of the numeric variables to normalize. If None (default) all numeric variables will be normalized.
-        copy: Whether to return a copy or act in place (default: False)
+        adata: :class:`~anndata.AnnData` object containing X to normalize values in.
+               Must already be encoded using :func:`~ehrapy.preprocessing.encode`.
+        vars: List of the names of the numeric variables to normalize.
+              If None all numeric variables will be normalized. Defaults to None .
+        copy: Whether to return a copy or act in place. Defaults to False .
         **kwargs: Additional arguments passed to :func:`~sklearn.preprocessing.power_transform`
 
     Returns:
-        :class:`~anndata.AnnData` object with normalized X. Also stores a record of applied normalizations as a dictionary in adata.uns["normalization"].
-
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
+        :class:`~anndata.AnnData` object with normalized X.
+        Also stores a record of applied normalizations as a dictionary in adata.uns["normalization"].
 
-            adata = ep.data.mimic_2(encode=True)
-            adata_norm = ep.pp.power_norm(adata, copy=True)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> adata_norm = ep.pp.power_norm(adata, copy=True)
     """
     if isinstance(vars, str):
         vars = [vars]
     if vars is None:
         vars = get_numeric_vars(adata)
     else:
         assert_numeric_vars(adata, vars)
 
     adata = _prep_adata_norm(adata, copy)
 
     var_idx = get_column_indices(adata, vars)
-    var_values = get_column_values(adata, var_idx)
+    var_values = _get_column_values(adata, var_idx)
 
     var_values = power_transform(var_values, **kwargs)
 
     set_numeric_vars(adata, var_values, vars)
 
     _record_norm(adata, vars, "power")
 
@@ -290,33 +292,33 @@
     vars: str | list[str] | None = None,
     base: int | float | None = None,
     offset: int | float = 1,
     copy: bool = False,
 ) -> AnnData | None:
     """Apply log normalization.
 
-    Computes :math:`x = \\log(x + offset)`, where :math:`log` denotes the natural logarithm unless a different base is given and the default :math:`offset` is :math:`1`
+    Computes :math:`x = \\log(x + offset)`, where :math:`log` denotes the natural logarithm
+    unless a different base is given and the default :math:`offset` is :math:`1`
 
     Args:
         adata: :class:`~anndata.AnnData` object containing X to normalize values in. Must already be encoded using :func:`~ehrapy.preprocessing.encode`.
-        vars: List of the names of the numeric variables to normalize. If None (default) all numeric variables will be normalized.
+        vars: List of the names of the numeric variables to normalize.
+              If None all numeric variables will be normalized. Defaults to None.
         base: Numeric base for logarithm. If None the natural logarithm is used.
-        offset: Offset added to values before computing the logarithm. (default: 1)
-        copy: Whether to return a copy or act in place (default: False)
+        offset: Offset added to values before computing the logarithm. Defaults to 1 .
+        copy: Whether to return a copy or act in place. Defaults to False .
 
     Returns:
-        :class:`~anndata.AnnData` object with normalized X. Also stores a record of applied normalizations as a dictionary in adata.uns["normalization"].
-
-    Example:
-        .. code-block:: python
+        :class:`~anndata.AnnData` object with normalized X.
+        Also stores a record of applied normalizations as a dictionary in adata.uns["normalization"].
 
-            import ehrapy as ep
-
-            adata = ep.data.mimic_2(encode=True)
-            adata_norm = ep.pp.log_norm(adata, copy=True)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> adata_norm = ep.pp.log_norm(adata, copy=True)
     """
     if isinstance(vars, str):
         vars = [vars]
     if vars is None:
         vars = get_numeric_vars(adata)
     else:
         assert_numeric_vars(adata, vars)
@@ -327,15 +329,15 @@
         raise ValueError(
             "Matrix of X contains negative values. "
             "Undefined behavior for log normalization. "
             "Please offset negative values with ep.pp.offset_negative_values()."
         )
 
     var_idx = get_column_indices(adata, vars)
-    var_values = get_column_values(adata, var_idx)
+    var_values = _get_column_values(adata, var_idx)
 
     if offset == 1:
         np.log1p(var_values, out=var_values)
     else:
         var_values = var_values + offset
         np.log(var_values, out=var_values)
 
@@ -353,40 +355,40 @@
 
 def sqrt_norm(adata: AnnData, vars: str | list[str] | None = None, copy: bool = False) -> AnnData | None:
     """Apply square root normalization.
 
     Take the square root of all values.
 
     Args:
-        adata: :class:`~anndata.AnnData` object containing X to normalize values in. Must already be encoded using :func:`~ehrapy.preprocessing.encode`.
-        vars: List of the names of the numeric variables to normalize. If None (default) all numeric variables will be normalized.
-        copy: Whether to return a copy or act in place (default: False)
+        adata: :class:`~anndata.AnnData` object containing X to normalize values in.
+               Must already be encoded using :func:`~ehrapy.preprocessing.encode`.
+        vars: List of the names of the numeric variables to normalize.
+              If None all numeric variables will be normalized. Defaults to None .
+        copy: Whether to return a copy or act in place. Defaults to False .
 
     Returns:
-        :class:`~anndata.AnnData` object with normalized X. Also stores a record of applied normalizations as a dictionary in adata.uns["normalization"].
-
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
+        :class:`~anndata.AnnData` object with normalized X.
+        Also stores a record of applied normalizations as a dictionary in adata.uns["normalization"].
 
-            adata = ep.data.mimic_2(encode=True)
-            adata_norm = ep.pp.sqrt_norm(adata, copy=True)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> adata_norm = ep.pp.sqrt_norm(adata, copy=True)
     """
     if isinstance(vars, str):
         vars = [vars]
     if vars is None:
         vars = get_numeric_vars(adata)
     else:
         assert_numeric_vars(adata, vars)
 
     adata = _prep_adata_norm(adata, copy)
 
     var_idx = get_column_indices(adata, vars)
-    var_values = get_column_values(adata, var_idx)
+    var_values = _get_column_values(adata, var_idx)
 
     var_values = np.sqrt(var_values)
 
     set_numeric_vars(adata, var_values, vars)
 
     _record_norm(adata, vars, "sqrt")
```

### Comparing `ehrapy-0.3.0/ehrapy/preprocessing/_outliers.py` & `ehrapy-0.4.0/ehrapy/preprocessing/_outliers.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,22 +16,28 @@
 ) -> AnnData:
     """Returns a Winsorized version of the input array.
 
     The implementation is based on https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.mstats.winsorize.html
 
     Args:
         adata: AnnData object to winsorize
-        vars: The features to winsorize
-        obs_cols: Columns in obs with features to winsorize
-        limits: Tuple of the percentages to cut on each side of the array as floats between 0. and 1. (default: 0.01 and 0.99)
+        vars: The features to winsorize.
+        obs_cols: Columns in obs with features to winsorize.
+        limits: Tuple of the percentages to cut on each side of the array as floats between 0. and 1.
+                Defaults to (0.01, 0.99)
         copy: Whether to return a copy or not
         **kwargs: Keywords arguments get passed to scipy.stats.mstats.winsorize
 
     Returns:
-        Winsorized AnnData object if copy is True
+        Winsorized AnnData object if copy is True.
+
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> ep.pp.winsorize(adata, ['bmi'])
     """
     _validate_outlier_input(adata, obs_cols, vars)
 
     if copy:  # pragma: no cover
         adata = adata.copy()
 
     if limits is None:
@@ -70,14 +76,19 @@
         vars: Columns in var with features to clip
         obs_cols: Columns in obs with features to clip
         limits: Interval, values outside of which are clipped to the interval edges
         copy: Whether to return a copy of AnnData or not
 
     Returns:
         A copy of original AnnData object with clipped features.
+
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> ep.pp.clip_quantile(adata, ['bmi'])
     """
     obs_cols, vars = _validate_outlier_input(adata, obs_cols, vars)  # type: ignore
 
     if vars:
         for var in vars:
             adata[:, var].X = np.clip(adata[:, var].X, limits[0], limits[1])
```

### Comparing `ehrapy-0.3.0/ehrapy/preprocessing/_quality_control.py` & `ehrapy-0.4.0/ehrapy/preprocessing/_quality_control.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from pathlib import Path
 from typing import Collection, Literal
 
 import numpy as np
 import pandas as pd
 from anndata import AnnData
 from rich import print
+from thefuzz import process
 
 from ehrapy import logging as logg
-from ehrapy.core.str_matching import StrMatcher
 
 
 def qc_metrics(
     adata: AnnData, qc_vars: Collection[str] = (), layer: str = None, inplace: bool = True
 ) -> pd.DataFrame | None:
     """Calculates various quality control metrics.
 
@@ -50,25 +50,22 @@
         `std`
             Standard deviation of the features.
         `min`
             Minimum value of the features.
         `max`
             Maximum value of the features.
 
-        Example:
-            .. code-block:: python
-
-                import ehrapy as ep
-                import seaborn as sns
-                import matplotlib.pyplot as plt
-
-                adata = ep.dt.mimic_2(encode=True)
-                ep.pp.qc_metrics(adata)
-                sns.displot(adata.obs["missing_values_abs"])
-                plt.show()
+        Examples:
+            >>> import ehrapy as ep
+            >>> import seaborn as sns
+            >>> import matplotlib.pyplot as plt
+            >>> adata = ep.dt.mimic_2(encoded=True)
+            >>> ep.pp.qc_metrics(adata)
+            >>> sns.displot(adata.obs["missing_values_abs"])
+            >>> plt.show()
     """
     obs_metrics = _obs_qc_metrics(adata, layer, qc_vars)
     var_metrics = _var_qc_metrics(adata, layer)
 
     if inplace:
         adata.obs[obs_metrics.columns] = obs_metrics
         adata.var[var_metrics.columns] = var_metrics
@@ -81,15 +78,15 @@
     arr: np.ndarray, shape: tuple[int, int] = None, df_type: Literal["obs", "var"] = "obs"
 ) -> np.ndarray:
     """Calculates the absolute or relative amount of missing values.
 
     Args:
         arr: Numpy array containing a data row which is a subset of X (mtx).
         shape: Shape of X (mtx).
-        df_type: Whether to calculate the proportions for obs or var. One of 'obs' or 'var' (default: 'obs').
+        df_type: Whether to calculate the proportions for obs or var. One of 'obs' or 'var'. Defaults to 'obs' .
 
     Returns:
         Absolute or relative amount of missing values.
     """
     # Absolute number of missing values
     if shape is None:
         return pd.isnull(arr).sum()
@@ -159,53 +156,70 @@
         layer: Layer containing the matrix to calculate the metrics for.
 
     Returns:
         Pandas DataFrame with the calculated metrics.
     """
     var_metrics = pd.DataFrame(index=adata.var_names)
     mtx = adata.X if layer is None else adata.layers[layer]
+    categorical_indices = np.ndarray([0], dtype=int)
     if "original_values_categoricals" in adata.uns:
         for original_values_categorical in list(adata.uns["original_values_categoricals"]):
             mtx = copy.deepcopy(mtx.astype(object))
-            index = np.where(var_metrics.index.str.contains(original_values_categorical))[0]
+            index = np.where(var_metrics.index.str.startswith("ehrapycat_" + original_values_categorical))[0]
             mtx[:, index] = np.tile(
                 np.where(
                     adata.uns["original_values_categoricals"][original_values_categorical].astype(object) == "nan",
                     np.nan,
                     adata.uns["original_values_categoricals"][original_values_categorical].astype(object),
                 ),
                 mtx[:, index].shape[1],
             )
-
+            categorical_indices = np.concatenate([categorical_indices, index])
+    non_categorical_indices = np.ones(mtx.shape[1], dtype=bool)
+    non_categorical_indices[categorical_indices] = False
     var_metrics["missing_values_abs"] = np.apply_along_axis(_missing_values, 0, mtx)
     var_metrics["missing_values_pct"] = np.apply_along_axis(_missing_values, 0, mtx, shape=mtx.shape, df_type="var")
+
+    var_metrics["mean"] = np.nan
+    var_metrics["median"] = np.nan
+    var_metrics["standard_deviation"] = np.nan
+    var_metrics["min"] = np.nan
+    var_metrics["max"] = np.nan
+
     try:
-        var_metrics["mean"] = np.nanmean(mtx, axis=0)
-        var_metrics["median"] = np.nanmedian(mtx, axis=0)
-        var_metrics["standard_deviation"] = np.nanstd(mtx, axis=0)
-        var_metrics["min"] = np.nanmin(mtx, axis=0)
-        var_metrics["max"] = np.nanmax(mtx, axis=0)
+        var_metrics.loc[non_categorical_indices, "mean"] = np.nanmean(
+            np.array(mtx[:, non_categorical_indices], dtype=np.float64), axis=0
+        )
+        var_metrics.loc[non_categorical_indices, "median"] = np.nanmedian(
+            np.array(mtx[:, non_categorical_indices], dtype=np.float64), axis=0
+        )
+        var_metrics.loc[non_categorical_indices, "standard_deviation"] = np.nanstd(
+            np.array(mtx[:, non_categorical_indices], dtype=np.float64), axis=0
+        )
+        var_metrics.loc[non_categorical_indices, "min"] = np.nanmin(
+            np.array(mtx[:, non_categorical_indices], dtype=np.float64), axis=0
+        )
+        var_metrics.loc[non_categorical_indices, "max"] = np.nanmax(
+            np.array(mtx[:, non_categorical_indices], dtype=np.float64), axis=0
+        )
     except TypeError:
         print("[bold yellow]TypeError! Setting quality control metrics to nan. Did you encode your data?")
-        var_metrics["mean"] = np.nan
-        var_metrics["median"] = np.nan
-        var_metrics["standard_deviation"] = np.nan
-        var_metrics["min"] = np.nan
-        var_metrics["max"] = np.nan
+    except ValueError:
+        print("[bold yellow]ValueError! Setting quality control metrics to nan. Did you encode your data?")
 
     return var_metrics
 
 
 def qc_lab_measurements(
     adata: AnnData,
     reference_table: pd.DataFrame = None,
     measurements: list[str] = None,
     unit: Literal["traditional", "SI"] = None,
     layer: str = None,
-    threshold: float = 0.2,
+    threshold: int = 20,
     age_col: str = None,
     age_range: str = None,
     sex_col: str = None,
     sex: str = None,
     ethnicity_col: str = None,
     ethnicity: str = None,
     copy: bool = False,
@@ -242,51 +256,49 @@
     Ethnicity and age columns can be added.
     https://github.com/theislab/ehrapy/ehrapy/preprocessing/laboratory_reference_tables/laposata.tsv
 
     Args:
         adata: Annotated data matrix.
         reference_table: A custom DataFrame with reference values. Defaults to the laposata table if not specified.
         measurements: A list of measurements to check.
-        unit: The unit of the measurements. (default: SI)
+        unit: The unit of the measurements. Defaults to 'traditional'.
         layer: Layer containing the matrix to calculate the metrics for.
-        threshold: Minimum required matching confidence score of the bigrams.
-                   0 = low requirements, 1 = high requirements.
+        threshold: Minimum required matching confidence score of the fuzzysearch.
+                   0 = no matches, 100 = all must match. Defaults to 20.
         age_col: Column containing age values.
         age_range: The inclusive age-range to filter for. e.g. 5-99
-        sex_col: Column containing sex values.
+        sex_col: Column containing sex values. Column must contain 'U', 'M' or 'F'.
         sex: Sex to filter the reference values for. Use U for unisex which uses male values when male and female conflict.
-             (default: U|M)
+             Defaults to 'U|M'
         ethnicity_col: Column containing ethnicity values.
         ethnicity: Ethnicity to filter for.
-        copy: Whether to return a copy (default: False).
-        verbose: Whether to have verbose stdout. Notifes user of matched columns and value ranges.
+        copy: Whether to return a copy. Defaults to False .
+        verbose: Whether to have verbose stdout. Notifies user of matched columns and value ranges.
 
     Returns:
         A modified AnnData object (copy if specified).
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            ep.pp.qc_lab_measurements(adata, measurements=["Interleukin-6[pg/ml]"], verbose=True)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.mimic_2(encoded=True)
+        >>> ep.pp.qc_lab_measurements(adata, measurements=["potassium_first"], verbose=True)
     """
     if copy:
         adata = adata.copy()
 
     preprocessing_dir = Path(__file__).parent.resolve()
     if reference_table is None:
         reference_table = pd.read_csv(
             f"{preprocessing_dir}/laboratory_reference_tables/laposata.tsv", sep="\t", index_col="Measurement"
         )
 
-    str_matcher = StrMatcher(list(reference_table.index))
-
     for measurement in measurements:
-        score, best_column_match = str_matcher.best_match(query=measurement, threshold=threshold)
+        best_column_match, score = process.extractOne(
+            query=measurement, choices=reference_table.index, score_cutoff=threshold
+        )
         if best_column_match is None:
             print(f"[bold yellow]Unable to find a match for {measurement}")
             continue
         if verbose:
             print(
                 f"[bold blue]Detected [green]{best_column_match}[blue] for [green]{measurement}[blue] with score [green]{score}."
             )
@@ -294,14 +306,25 @@
         reference_column = "SI Reference Interval" if unit == "SI" else "Traditional Reference Interval"
 
         # Fetch all non None columns from the reference measures
         not_none_columns = [col for col in [sex_col, age_col, ethnicity_col] if col is not None]
         not_none_columns.append(reference_column)
         reference_values = reference_table.loc[[best_column_match], not_none_columns]
 
+        additional_columns = False
+        if sex_col or age_col or ethnicity_col:  # check if additional columns were provided
+            additional_columns = True
+
+        # Check if multiple reference values occur and no additional information is available:
+        if reference_values.shape[0] > 1 and additional_columns is False:
+            raise ValueError(
+                f"Several options for {best_column_match} reference value are available. Please specify sex, age or "
+                f"ethnicity columns and their values."
+            )
+
         # Fetch reference values
         try:
             if age_col:
                 min_age, max_age = age_range.split("-")
                 reference_values = reference_values[
                     (reference_values[age_col].str.split("-").str[0].astype(int) >= int(min_age))
                     and (reference_values[age_col].str.split("-").str[1].astype(int) <= int(max_age))
```

### Comparing `ehrapy-0.3.0/ehrapy/preprocessing/_scanpy_pp_api.py` & `ehrapy-0.4.0/ehrapy/preprocessing/_scanpy_pp_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,32 +22,33 @@
 ) -> Union[AnnData, np.ndarray, spmatrix]:  # pragma: no cover
     """Computes a principal component analysis.
 
     Computes PCA coordinates, loadings and variance decomposition. Uses the implementation of *scikit-learn*.
 
     Args:
         data: The (annotated) data matrix of shape `n_obs` × `n_vars`. Rows correspond to observations and columns to features.
-        n_comps: Number of principal components to compute. Defaults to 50, or 1 - minimum dimension size of selected representation.
+        n_comps: Number of principal components to compute.
+                 Defaults to 50, or 1 - minimum dimension size of selected representation.
         zero_center: If `True`, compute standard PCA from covariance matrix.
                      If `False`, omit zero-centering variables (uses :class:`~sklearn.decomposition.TruncatedSVD`), which allows to handle sparse input efficiently.
                      Passing `None` decides automatically based on sparseness of the data.
         svd_solver: SVD solver to use:
 
                     * `'arpack'` (the default) for the ARPACK wrapper in SciPy (:func:`~scipy.sparse.linalg.svds`)
 
                     * `'randomized'` for the randomized algorithm due to Halko (2009).
 
                     * `'auto'` chooses automatically depending on the size of the problem.
 
                     * `'lobpcg'` An alternative SciPy solver.
 
                     Efficient computation of the principal components of a sparse matrix currently only works with the `'arpack`' or `'lobpcg'` solvers.
-        random_state: Change to use different initial states for the optimization. (default: 0)
+        random_state: Change to use different initial states for the optimization. Defaults to 0 .
         return_info: Only relevant when not passing an :class:`~anndata.AnnData`: see “**Returns**”.
-        dtype: Numpy data type string to which to convert the result. (default: float32)
+        dtype: Numpy data type string to which to convert the result. Defaults to float32 .
         copy: If an :class:`~anndata.AnnData` is passed, determines whether a copy is returned. Is ignored otherwise.
         chunked: If `True`, perform an incremental PCA on segments of `chunk_size`.
                   The incremental PCA automatically zero centers and ignores settings of
                   `random_seed` and `svd_solver`. If `False`, perform a full PCA.
         chunk_size: Number of observations to include in each chunk. Required if `chunked=True` was passed.
 
     Returns:
```

### Comparing `ehrapy-0.3.0/ehrapy/preprocessing/laboratory_reference_tables/laposata.tsv` & `ehrapy-0.4.0/ehrapy/preprocessing/laboratory_reference_tables/laposata.tsv`

 * *Files identical despite different names*

### Comparing `ehrapy-0.3.0/ehrapy/tools/_sa.py` & `ehrapy-0.4.0/ehrapy/tools/_sa.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
-from typing import Literal
+from typing import Iterable, Literal
 
 import numpy as np  # noqa: F401 # This package is implicitly used
 import pandas as pd
 import statsmodels.api as sm
 import statsmodels.formula.api as smf
 from anndata import AnnData
 from lifelines import KaplanMeierFitter
+from lifelines.statistics import StatisticalResult, logrank_test
 from scipy import stats
 from statsmodels.genmod.generalized_linear_model import GLMResultsWrapper
 
 
 def ols(
     adata: AnnData,
     var_names: list[str] | None | None = None,
@@ -28,138 +29,125 @@
         var_names: A list of var names indicating which columns are for the OLS model.
         formula: The formula specifying the model.
         missing: Available options are 'none', 'drop', and 'raise'. If 'none', no nan checking is done. If 'drop', any observations with nans are dropped. If 'raise', an error is raised. Default is 'none'.
 
     Returns:
         The OLS model instance.
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.dt.mimic_2(encoded=False)
-            formula = 'tco2_first ~ pco2_first'
-            var_names = ['tco2_first', 'pco2_first']
-            ols = ep.tl.ols(adata, var_names, formula, missing = 'drop')
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.mimic_2(encoded=False)
+        >>> formula = 'tco2_first ~ pco2_first'
+        >>> var_names = ['tco2_first', 'pco2_first']
+        >>> ols = ep.tl.ols(adata, var_names, formula, missing = 'drop')
     """
     if isinstance(var_names, list):
         data = pd.DataFrame(adata[:, var_names].X, columns=var_names).astype(float)
     else:
         data = pd.DataFrame(adata.X, columns=adata.var_names)
     ols = smf.ols(formula, data=data, missing=missing)
+
     return ols
 
 
 def glm(
     adata: AnnData,
-    var_names: list[str] | None = None,
+    var_names: Iterable[str] | None = None,
     formula: str | None = None,
     family: Literal["Gaussian", "Binomial", "Gamma", "Gaussian", "InverseGaussian"] = "Gaussian",
     missing: Literal["none", "drop", "raise"] = "none",
-    ascontinus: list[str] | None | None = None,
+    as_continuous: Iterable[str] | None | None = None,
 ) -> sm.GLM:
     """Create a Generalized Linear Model (GLM) from a formula, a distribution, and AnnData.
 
     See https://www.statsmodels.org/stable/generated/statsmodels.formula.api.glm.html#statsmodels.formula.api.glm
     Internally use the statsmodel to create a GLM Model from a formula, a distribution, and dataframe.
 
     Args:
         adata: The AnnData object for the GLM model.
         var_names: A list of var names indicating which columns are for the GLM model.
         formula: The formula specifying the model.
-        family: The distribution families. Available options are 'Gaussian', 'Binomial', 'Gamma', and 'InverseGaussian', (default: 'Gaussian').
-        missing: Available options are 'none', 'drop', and 'raise'. If 'none', no nan checking is done. If 'drop', any observations with nans are dropped. If 'raise', an error is raised (default: 'none').
-        ascontinus: A list of var names indicating which columns are continus rather than categorical. The corresponding columns will be set as type float.
+        family: The distribution families. Available options are 'Gaussian', 'Binomial', 'Gamma', and 'InverseGaussian'.
+                Defaults to 'Gaussian'.
+        missing: Available options are 'none', 'drop', and 'raise'. If 'none', no nan checking is done.
+                 If 'drop', any observations with nans are dropped. If 'raise', an error is raised (default: 'none').
+        ascontinus: A list of var names indicating which columns are continuous rather than categorical.
+                    The corresponding columns will be set as type float.
 
     Returns:
         The GLM model instance.
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.dt.mimic_2(encoded=False)
-            formula = 'day_28_flg ~ age'
-            var_names = ['day_28_flg', 'age']
-            family = 'Binomial'
-            glm = ep.tl.glmglm(adata, var_names, formula, family, missing = 'drop', ascontinus = ['age'])
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.mimic_2(encoded=False)
+        >>> formula = 'day_28_flg ~ age'
+        >>> var_names = ['day_28_flg', 'age']
+        >>> family = 'Binomial'
+        >>> glm = ep.tl.glmglm(adata, var_names, formula, family, missing = 'drop', ascontinus = ['age'])
     """
     family_dict = {
         "Gaussian": sm.families.Gaussian(),
         "Binomial": sm.families.Binomial(),
         "Gamma": sm.families.Gamma(),
         "InverseGaussian": sm.families.InverseGaussian(),
     }
     if family in ["Gaussian", "Binomial", "Gamma", "Gaussian", "InverseGaussian"]:
         family = family_dict[family]
     if isinstance(var_names, list):
         data = pd.DataFrame(adata[:, var_names].X, columns=var_names)
     else:
         data = pd.DataFrame(adata.X, columns=adata.var_names)
-    if ascontinus is not None:
-        data[ascontinus] = data[ascontinus].astype(float)
+    if as_continuous is not None:
+        data[as_continuous] = data[as_continuous].astype(float)
     glm = smf.glm(formula, data=data, family=family, missing=missing)
 
     return glm
 
 
 def kmf(
-    durations,
-    event_observed=None,
-    timeline=None,
-    entry=None,
-    label=None,
-    alpha=None,
-    ci_labels=None,
-    weights=None,
-    censoring=None,
+    durations: Iterable,
+    event_observed: Iterable | None = None,
+    timeline: Iterable = None,
+    entry: Iterable | None = None,
+    label: str | None = None,
+    alpha: float | None = None,
+    ci_labels: tuple[str, str] = None,
+    weights: Iterable | None = None,
+    censoring: Literal["right", "left"] = None,
 ) -> KaplanMeierFitter:
     """Fit the Kaplan-Meier estimate for the survival function.
 
     See https://lifelines.readthedocs.io/en/latest/fitters/univariate/KaplanMeierFitter.html#module-lifelines.fitters.kaplan_meier_fitter
     Class for fitting the Kaplan-Meier estimate for the survival function.
 
     Args:
-        durations: an array, list, pd.DataFrame or pd.Series
-            length n -- duration (relative to subject's birth) the subject was alive for.
-        event_observed: an array, list, pd.DataFrame, or pd.Series, optional
-            True if the the death was observed, False if the event was lost (right-censored) (default: all True if event_observed==None).
-        timeline: an array, list, pd.DataFrame, or pd.Series, optional
-            return the best estimate at the values in timelines (positively increasing)
-        entry: an array, list, pd.DataFrame, or pd.Series, optional
-            relative time when a subject entered the study. This is useful for left-truncated (not left-censored) observations. If None, all members of the population
-            entered study when they were "born".
-        label: string, optional
-            a string to name the column of the estimate.
-        alpha: float, optional
-            the alpha value in the confidence intervals. Overrides the initializing alpha for this call to fit only.
-        ci_labels: tuple, optional
-            add custom column names to the generated confidence intervals as a length-2 list: [<lower-bound name>, <upper-bound name>] (default: <label>_lower_<1-alpha/2>).
-        weights: an array, list, pd.DataFrame, or pd.Series, optional
-            if providing a weighted dataset. For example, instead
-            of providing every subject as a single element of `durations` and `event_observed`, one could
-            weigh subject differently.
-        censoring: string, optional. One of ('right', 'left)
-            'right' for fitting the model to a right-censored dataset. 'left' for fitting the model to a left-censored dataset (default: fit the model to a right-censored dataset).
+        durations: length n -- duration (relative to subject's birth) the subject was alive for.
+        event_observed: True if the the death was observed, False if the event was lost (right-censored). Defaults to all True if event_observed==None.
+        timeline: return the best estimate at the values in timelines (positively increasing)
+        entry: Relative time when a subject entered the study. This is useful for left-truncated (not left-censored) observations.
+         If None, all members of the population entered study when they were "born".
+        label: A string to name the column of the estimate.
+        alpha: The alpha value in the confidence intervals. Overrides the initializing alpha for this call to fit only.
+        ci_labels: Add custom column names to the generated confidence intervals as a length-2 list: [<lower-bound name>, <upper-bound name>] (default: <label>_lower_<1-alpha/2>).
+        weights: If providing a weighted dataset. For example, instead of providing every subject
+                 as a single element of `durations` and `event_observed`, one could weigh subject differently.
+        censoring: 'right' for fitting the model to a right-censored dataset.
+                   'left' for fitting the model to a left-censored dataset (default: fit the model to a right-censored dataset).
 
     Returns:
         Fitted KaplanMeierFitter
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-            adata = ep.dt.mimic_2(encoded=False)
-            # Because in MIMIC-II database, `censor_fl` is censored or death (binary: 0 = death, 1 = censored).
-            # While in KaplanMeierFitter, `event_observed` is True if the the death was observed, False if the event was lost (right-censored).
-            # So we need to flip `censor_fl` when pass `censor_fl` to KaplanMeierFitter
-            adata[:, ['censor_flg']].X = np.where(adata[:, ['censor_flg']].X == 0, 1, 0)
-            kmf = ep.tl.kmf(adata[:, ['mort_day_censored']].X, adata[:, ['censor_flg']].X)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.mimic_2(encoded=False)
+        >>> # Because in MIMIC-II database, `censor_fl` is censored or death (binary: 0 = death, 1 = censored).
+        >>> # While in KaplanMeierFitter, `event_observed` is True if the the death was observed, False if the event was lost (right-censored).
+        >>> # So we need to flip `censor_fl` when pass `censor_fl` to KaplanMeierFitter
+        >>> adata[:, ['censor_flg']].X = np.where(adata[:, ['censor_flg']].X == 0, 1, 0)
+        >>> kmf = ep.tl.kmf(adata[:, ['mort_day_censored']].X, adata[:, ['censor_flg']].X)
     """
     kmf = KaplanMeierFitter()
     if censoring == "None" or "right":
         kmf.fit(
             durations=durations,
             event_observed=event_observed,
             timeline=timeline,
@@ -180,16 +168,57 @@
             ci_labels=ci_labels,
             weights=weights,
         )
 
     return kmf
 
 
-def calculate_nested_f_statistic(small_model: GLMResultsWrapper, big_model: GLMResultsWrapper) -> float:
-    """Given two fitted GLMs, the larger of which contains the parameter space of the smaller, return the P value corresponding to the larger model adding explanatory power
+def test_kmf_logrank(
+    kmf_A: KaplanMeierFitter,
+    kmf_B: KaplanMeierFitter,
+    t_0: float | None = -1,
+    weightings: Literal["wilcoxon", "tarone-ware", "peto", "fleming-harrington"] | None = None,
+) -> StatisticalResult:
+    """Calculates the p-value for the logrank test comparing the survival functions of two groups.
+
+    See https://lifelines.readthedocs.io/en/latest/lifelines.statistics.html
+
+    Measures and reports on whether two intensity processes are different.
+    That is, given two event series, determines whether the data generating processes are statistically different.
+    The test-statistic is chi-squared under the null hypothesis.
+
+    Args:
+        kmf_A: The first KaplanMeierFitter object containing the durations and events.
+        kmf_B: The second KaplanMeierFitter object containing the durations and events.
+        t_0: The final time period under observation, and subjects who experience the event after this time are set to be censored.
+             Specify -1 to use all time. Defaults to -1.
+        weightings: Apply a weighted logrank test: options are "wilcoxon" for Wilcoxon (also known as Breslow), "tarone-ware"
+                    for Tarone-Ware, "peto" for Peto test and "fleming-harrington" for Fleming-Harrington test.
+                    These are useful for testing for early or late differences in the survival curve. For the Fleming-Harrington
+                    test, keyword arguments p and q must also be provided with non-negative values.
+
+    Returns:
+        The p-value for the logrank test comparing the survival functions of the two groups.
+    """
+    results_pairwise = logrank_test(
+        durations_A=kmf_A.durations,
+        durations_B=kmf_B.durations,
+        event_observed_A=kmf_A.event_observed,
+        event_observed_B=kmf_B.event_observed,
+        weights_A=kmf_A.weights,
+        weights_B=kmf_B.weights,
+        t_0=t_0,
+        weightings=weightings,
+    )
+
+    return results_pairwise
+
+
+def test_nested_f_statistic(small_model: GLMResultsWrapper, big_model: GLMResultsWrapper) -> float:
+    """Given two fitted GLMs, the larger of which contains the parameter space of the smaller, return the P value corresponding to the larger model adding explanatory power.
 
     See https://stackoverflow.com/questions/27328623/anova-test-for-glm-in-python/60769343#60769343
 
     Args:
         small_model (GLMResultsWrapper): fitted generalized linear models.
         big_model (GLMResultsWrapper): fitted generalized linear models.
 
@@ -213,15 +242,15 @@
         result_2 (GLMResultsWrapper): fitted generalized linear models.
         formula_1 (str): The formula specifying the model.
         formula_2 (str): The formula specifying the model.
 
     Returns:
         pd.DataFrame: Anova table.
     """
-    p_value = calculate_nested_f_statistic(result_1, result_2)
+    p_value = test_nested_f_statistic(result_1, result_2)
 
     table = {
         "Model": [1, 2],
         "formula": [formula_1, formula_2],
         "Df Resid.": [result_1.df_resid, result_2.df_resid],
         "Dev.": [result_1.deviance, result_2.deviance],
         "Df_diff": [None, result_2.df_model - result_1.df_model],
```

### Comparing `ehrapy-0.3.0/ehrapy/tools/_scanpy_tl_api.py` & `ehrapy-0.4.0/ehrapy/tools/_scanpy_tl_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,17 @@
                       If `None`, the initial state is not reproducible.
         n_jobs: Number of jobs for parallel computation.
                 `None` means using :attr:`scanpy._settings.ScanpyConfig.n_jobs`.
         copy: Return a copy instead of writing to `adata`.
         metric: Distance metric calculate neighbors on.
 
     Returns:
+        Depending on `copy`, returns or updates `adata` with the following fields.
 
+        **X_tsne** : `np.ndarray` (`adata.obs`, dtype `float`) tSNE coordinates of data.
     """
     return sc.tl.tsne(
         adata=adata,
         n_pcs=n_pcs,
         use_rep=use_rep,
         perplexity=perplexity,
         early_exaggeration=early_exaggeration,
@@ -337,23 +339,20 @@
     Returns:
         Updates `adata.obs` with an additional field specified by the `key_added`
         parameter. This parameter defaults to `[basis]_density_[groupby]`, where
         where `[basis]` is one of `umap`, `diffmap`, `pca`, `tsne`, or `draw_graph_fa`
         and `[groupby]` denotes the parameter input.
         Updates `adata.uns` with an additional field `[key_added]_params`.
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            adata = ep.data.mimic_2(encode=True)
-            ep.tl.umap(adata)
-            ep.tl.embedding_density(adata, basis='umap', groupby='phase')
-            ep.pl.embedding_density(adata, basis='umap', key='umap_density_phase', group='G1')
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> ep.tl.umap(adata)
+        >>> ep.tl.embedding_density(adata, basis='umap', groupby='phase')
+        >>> ep.pl.embedding_density(adata, basis='umap', key='umap_density_phase', group='G1')
     """
     sc.tl.embedding_density(adata=adata, basis=basis, groupby=groupby, key_added=key_added, components=components)
 
 
 def leiden(
     adata: AnnData,
     resolution: float = 1,
@@ -550,21 +549,19 @@
                    `.uns[f'dendrogram_{{groupby}}']`.
                    Notice that the `groupby` information is added to the dendrogram.
         inplace: If `True`, adds dendrogram information to `adata.uns[key_added]`,
                  else this function returns the information.
     Returns:
         If `inplace=False`, returns dendrogram information, else `adata.uns[key_added]` is updated with it.
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-            adata = ep.data.mimic_2(encode=True)
-            ep.tl.dendrogram(adata, groupby='service_unit')
-            ep.pl.dendrogram(adata)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> ep.tl.dendrogram(adata, groupby='service_unit')
+        >>> ep.pl.dendrogram(adata)
     """
     return sc.tl.dendrogram(
         adata=adata,
         groupby=groupby,
         n_pcs=n_pcs,
         use_rep=use_rep,
         var_names=var_names,
@@ -741,22 +738,19 @@
                  Add labels and embeddings to the passed `adata` (if `True`) or return a copy of `adata` with mapped embeddings and labels.
         **kwargs: Further keyword arguments for the Neighbor calculation
 
     Returns:
         * if `inplace=False` returns a copy of `adata` with mapped embeddings and labels in `obsm` and `obs` correspondingly
         * if `inplace=True` returns `None` and updates `adata.obsm` and `adata.obs` with mapped embeddings and labels
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-
-            ep.pp.neighbors(adata_ref)
-            ep.tl.umap(adata_ref)
-            ep.tl.ingest(adata, adata_ref, obs="service_unit")
+    Examples:
+        >>> import ehrapy as ep
+        >>> ep.pp.neighbors(adata_ref)
+        >>> ep.tl.umap(adata_ref)
+        >>> ep.tl.ingest(adata, adata_ref, obs="service_unit")
     """
     return sc.tl.ingest(
         adata=adata,
         adata_ref=adata_ref,
         obs=obs,
         embedding_method=embedding_method,
         labeling_method=labeling_method,
@@ -835,21 +829,19 @@
                       Corrected p-values.
         *pts*: `pandas.DataFrame` (`.uns['rank_features_groups']`)
                Fraction of cells expressing the genes for each group.
         *pts_rest*: `pandas.DataFrame` (`.uns['rank_features_groups']`)
                     Only if `reference` is set to `'rest'`.
                     Fraction of observations from the union of the rest of each group containing the features.
 
-     Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-            adata = eh.dt.mimic_2(encode=True)
-            ep.tl.rank_features_groups(adata, "service_unit")
-            ep.pl.rank_features_groups(adata)
+     Examples:
+         >>> import ehrapy as ep
+         >>> adata = ep.dt.mimic_2(encoded=True)
+         >>> ep.tl.rank_features_groups(adata, "service_unit")
+         >>> ep.pl.rank_features_groups(adata)
     """
     return sc.tl.rank_genes_groups(
         adata=adata,
         groupby=groupby,
         use_raw=False,
         groups=groups,
         reference=reference,
@@ -893,21 +885,19 @@
         min_in_group_fraction: Minimum in group fraction (default: 0.25).
         min_fold_change: Miniumum fold change (default: 1).
         max_out_group_fraction: Maximum out group fraction (default: 0.5).
 
     Returns:
         Same output as :func:`ehrapy.tl.rank_features_groups` but with filtered feature names set to `nan`
 
-    Example:
-        .. code-block:: python
-
-            import ehrapy as ep
-            adata = eh.dt.mimic_2(encode=True)
-            ep.tl.rank_features_groups(adata, "service_unit")
-            ep.pl.rank_features_groups(adata)
+    Examples:
+        >>> import ehrapy as ep
+        >>> adata = ep.dt.mimic_2(encoded=True)
+        >>> ep.tl.rank_features_groups(adata, "service_unit")
+        >>> ep.pl.rank_features_groups(adata)
     """
     return sc.tl.filter_rank_genes_groups(
         adata=adata,
         key=key,
         groupby=groupby,
         use_raw=False,
         key_added=key_added,
@@ -961,15 +951,15 @@
         inplace: Return a marker gene dataframe or store it inplace in `adata.uns`.
 
     Returns:
         A pandas dataframe with the marker gene overlap scores if `inplace=False`.
         For `inplace=True` `adata.uns` is updated with an additional field
         specified by the `key_added` parameter (default = 'marker_gene_overlap').
 
-    Example:
+    Examples:
         TODO
     """
     return sc.tl.marker_gene_overlap(
         adata=adata,
         reference_markers=reference_markers,
         key=key,
         method=method,
```

### Comparing `ehrapy-0.3.0/ehrapy/tools/nlp/_hpo.py` & `ehrapy-0.4.0/ehrapy/tools/nlp/_hpo.py`

 * *Files identical despite different names*

### Comparing `ehrapy-0.3.0/ehrapy/tools/nlp/_medcat.py` & `ehrapy-0.4.0/ehrapy/tools/nlp/_medcat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import pandas as pd
 from anndata import AnnData
+from thefuzz import process
 
-from ehrapy.core.str_matching import StrMatcher
-from ehrapy.core.tool_available import check_module_importable
+from ehrapy.core._tool_available import _check_module_importable
 
 try:
     from medcat.cat import CAT
     from medcat.cdb import CDB
     from medcat.cdb_maker import CDBMaker
     from medcat.config import Config
     from medcat.vocab import Vocab
@@ -21,15 +21,15 @@
 
 class MedCAT:
     """Wrapper class for Medcat. This class will hold references to the current AnnData object, which holds the data, the current model (with vocab and concept database) and should be
     passed to all functions exposed to the ehrapy nlp API when required.
     """
 
     def __init__(self, anndata: AnnData, vocabulary: Vocab = None, concept_db: CDB = None, model_pack_path=None):
-        if not check_module_importable("medcat"):
+        if not _check_module_importable("medcat"):
             raise RuntimeError("Package medcat is not importable. Please install via pip install medcat")
         self.anndata = anndata
         self.vocabulary = vocabulary
         self.concept_db = concept_db
         if self.vocabulary is not None and self.concept_db is not None:
             self.cat = CAT(cdb=concept_db, config=concept_db.config, vocab=vocabulary)
         elif model_pack_path is not None:
@@ -266,19 +266,19 @@
         """
         # only extract affirmed entities
         df = EhrapyMedcat._filter_df_by_status(medcat_obj.annotated_results, "Affirmed")
         # check whether the name is in the extracted entities to handle possible typos to a certain extend
         # currently, only the pretty_name column is supported
         # _list_replace(color, colored_column, colored_column_tmp)
         if name not in df["pretty_name"].values:
-            str_matcher = StrMatcher(references=df["pretty_name"].unique())
-            _, new_name = str_matcher.best_match(name, 0.5)
+            new_name, _ = process.extractOne(query=name, choices=df["pretty_name"].unique(), score_cutoff=50)
             if new_name:
                 print(
-                    f"[bold yellow]Did not find [blue]{name} [yellow]in MedCAT's extracted entities. Will use best match {new_name}!"
+                    f"[bold yellow]Did not find [blue]{name} [yellow]in MedCAT's extracted entities. "
+                    f"Will use best match {new_name}!"
                 )
 
                 def _list_replace(lst, old: str, new: str):
                     """replace list elements (inplace)"""
                     i = -1
                     try:
                         while True:
```

### Comparing `ehrapy-0.3.0/ehrapy/tools/nlp/_translators.py` & `ehrapy-0.4.0/ehrapy/tools/nlp/_translators.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,24 +16,23 @@
         YandexTranslator,
     )
 except ConnectionError:  # pragma: no cover
     print("[bold red]Unable to import GoogleTranslator. Do you have an internet connection?")
 from deepl import Formality, GlossaryInfo, TextResult
 from rich import print
 
-from ehrapy.anndata.anndata_ext import get_column_indices, get_column_values
+from ehrapy.anndata.anndata_ext import _get_column_values, get_column_indices
 
 
 class Translator:
     """Class providing an interface to all translation functions. Requires a flavour."""
 
     def __init__(
         self, flavour: str = "deepl", source: str = "de", target: str = "en", token: str = None
     ) -> None:  # pragma: no cover
-
         self.translator: DeepL | GoogleTranslate | LibreTranslate | MyMemoryTranslate | MicrosoftTranslate | YandexTranslate = (
             None
         )
         if flavour == "deepl":
             self.translator = DeepL(token)
         elif flavour == "googletranslate":
             self.translator = GoogleTranslate(source, target)  # type: ignore
@@ -151,15 +150,15 @@
         if isinstance(columns, str):  # pragma: no cover
             columns = [columns]
 
         translate_text = self.translate_text
         indices = get_column_indices(adata, columns)
 
         for column, index in zip(columns, indices):
-            column_values = get_column_values(adata, index)
+            column_values = _get_column_values(adata, index)
 
             if column_values.dtype != str and column_values.dtype != object:  # pragma: no cover
                 raise ValueError("Attempted to translate column {column} which does not only contain strings.")
 
             if translate_column_name:  # TODO This requires a test
                 translated_column_name = translate_text(column)
                 index_values = adata.var_names.tolist()
```

### Comparing `ehrapy-0.3.0/ehrapy/util/_doc_util.py` & `ehrapy-0.4.0/ehrapy/util/_doc_util.py`

 * *Files identical despite different names*

### Comparing `ehrapy-0.3.0/pyproject.toml` & `ehrapy-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,101 +1,109 @@
 [tool.poetry]
 name = "ehrapy"
-version = "0.3.0"  # <<COOKIETEMPLE_FORCE_BUMP>>
+version = "0.4.0"  # <<COOKIETEMPLE_FORCE_BUMP>>
 description = "Electronic Health Record Analysis with Python."
 authors = ["Lukas Heumos <lukas.heumos@posteo.net>", "Philipp Ehmele <philipp_ehm@protonmail.com>"]
 license = "Apache2.0"
 readme = "README.md"
 homepage = "https://github.com/theislab/ehrapy"
 repository = "https://github.com/theislab/ehrapy"
 documentation = "https://ehrapy.readthedocs.io"
 packages = [
     { include = "ehrapy" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.0,<4"
-click = ">=7.0.0"
 rich = ">=10.12.0"
 PyYAML = ">=5.4.1"
-Jinja2 = ">=3.0.1"
 questionary = ">=1.10.0"
 requests = ">=2.26.0"
-pandas = ">=1.3.3"
+pandas = "^2.0.1"
 mudata = ">=0.1.1"
 pypi-latest = ">=0.1.1"
 scikit-learn = ">=1.0"
 category_encoders = ">=2.2.2"
 leidenalg = ">=0.8.7"
 deepl = ">=1.2.0"
 pynndescent = ">=0.5.4"
-scanpy = ">=1.8.2"
+scanpy = "^1.9.1"
 ipython = ">=7.30.1"
 pyhpo = {extras = ["all"], version = ">=3.0.0"}
 deep-translator = ">=1.6.1"
 scikit-learn-intelex = {version = ">=2021.5.3", optional = true}
-medcat = {version = ">=1.2.6", optional = true}
+medcat = {version = "^1.5.0", optional = true}
 anndata = ">=0.7.8"
 fancyimpute = ">=0.7.0"
 miceforest = ">=5.3.0"
 scikit-misc = ">=0.1.4"
 session-info = ">=1.0.0"
-lifelines = "^0.27.0"
-ipywidgets = "^8.0.2"
-missingno = "^0.5.1"
-tabulate = "^0.9.0"
+lifelines = ">=0.27.0"
+missingno = ">=0.5.1"
+thefuzz = {extras = ["speedup"], version = "^0.19.0"}
+tabulate = ">=0.9.0"
+fhiry = ">=2.1,<4.0"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=6.2.5"
 coverage = {extras = ["toml"], version = ">=6.0"}
 safety = ">=1.9.0"
 mypy = ">=0.930"
 typeguard = ">=2.13.3"
 xdoctest = {extras = ["colors"], version = ">=0.15.10"}
-sphinx = ">=4.3.2"
-sphinx-autobuild = ">=2021.3.14"
 pre-commit = ">=2.16.0"
 flake8 = ">=4.0.1"
 black = {extras = ["jupyter"], version = ">=21.12b0"}
 flake8-bandit = ">=2.1.2"
 flake8-bugbear = ">=21.11.29"
 flake8-docstrings = ">=1.5.0"
 flake8-rst-docstrings = ">=0.2.5"
 pep8-naming = ">=0.12.1"
 pre-commit-hooks = ">=4.0.1"
-sphinx-click = ">=3.0.0"
 Pygments = ">=2.10.0"
 types-pkg-resources = ">=0.1.3"
 types-requests = ">=2.26.2"
 types-attrs = ">=19.1.0"
 pyenchant = ">=3.2.1"
+pyupgrade = ">=2.30.1"
+
+[tool.poetry.extras]
+en-core-web-md = ["en-core-web-md"]
+scikit-learn-intelex = ["scikit-learn-intelex"]
+medcat = ["medcat"]
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+sphinx_gallery = "<0.11"
+sphinx = ">=4.3.2"
+sphinx-autobuild = ">=2021.3.14"
 sphinx-gallery = ">0.6,<0.11"
 sphinx-autodoc-typehints = ">=1.12.0"
 sphinx-last-updated-by-git = ">=0.3.0"
 nbsphinx = ">=0.8.7"
 sphinxcontrib-bibtex = ">=2.4.1"
 sphinx-automodapi = ">=0.14"
 nbsphinx-link = ">=1.3.0"
 sphinx-copybutton = ">=0.4.0"
-pyupgrade = ">=2.30.1"
-furo = ">=2022.3.4"
 myst-parser = ">=0.17.0"
 sphinx-remove-toctrees = ">=0.0.3"
 sphinx-design = ">=0.0.13"
 sphinxext-opengraph = ">=0.6.2"
-
-[tool.poetry.extras]
-en-core-web-md = ["en-core-web-md"]
-scikit-learn-intelex = ["scikit-learn-intelex"]
-medcat = ["medcat"]
+sphinx-click = ">=3.0.0"
+furo = ">=2022.3.4"
+sphinx-autodoc-annotation = "^1.0.post1"
+sphinxcontrib-spelling = ">=7.7,<9.0"
 
 [tool.poetry.scripts]
 ehrapy = "ehrapy.__main__:main"
 
 [tool.black]
 line-length = 120
```

### Comparing `ehrapy-0.3.0/PKG-INFO` & `ehrapy-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,57 +1,53 @@
 Metadata-Version: 2.1
 Name: ehrapy
-Version: 0.3.0
+Version: 0.4.0
 Summary: Electronic Health Record Analysis with Python.
 Home-page: https://github.com/theislab/ehrapy
 License: Apache2.0
 Author: Lukas Heumos
 Author-email: lukas.heumos@posteo.net
 Requires-Python: >=3.8.0,<4
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: en-core-web-md
 Provides-Extra: medcat
 Provides-Extra: scikit-learn-intelex
-Requires-Dist: Jinja2 (>=3.0.1)
 Requires-Dist: PyYAML (>=5.4.1)
 Requires-Dist: anndata (>=0.7.8)
 Requires-Dist: category_encoders (>=2.2.2)
-Requires-Dist: click (>=7.0.0)
 Requires-Dist: deep-translator (>=1.6.1)
 Requires-Dist: deepl (>=1.2.0)
 Requires-Dist: fancyimpute (>=0.7.0)
+Requires-Dist: fhiry (>=2.1,<4.0)
 Requires-Dist: ipython (>=7.30.1)
-Requires-Dist: ipywidgets (>=8.0.2,<9.0.0)
 Requires-Dist: leidenalg (>=0.8.7)
-Requires-Dist: lifelines (>=0.27.0,<0.28.0)
-Requires-Dist: medcat (>=1.2.6); extra == "medcat"
+Requires-Dist: lifelines (>=0.27.0)
+Requires-Dist: medcat (>=1.5.0,<2.0.0) ; extra == "medcat"
 Requires-Dist: miceforest (>=5.3.0)
-Requires-Dist: missingno (>=0.5.1,<0.6.0)
+Requires-Dist: missingno (>=0.5.1)
 Requires-Dist: mudata (>=0.1.1)
-Requires-Dist: pandas (>=1.3.3)
+Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: pyhpo[all] (>=3.0.0)
 Requires-Dist: pynndescent (>=0.5.4)
 Requires-Dist: pypi-latest (>=0.1.1)
 Requires-Dist: questionary (>=1.10.0)
 Requires-Dist: requests (>=2.26.0)
 Requires-Dist: rich (>=10.12.0)
-Requires-Dist: scanpy (>=1.8.2)
+Requires-Dist: scanpy (>=1.9.1,<2.0.0)
 Requires-Dist: scikit-learn (>=1.0)
-Requires-Dist: scikit-learn-intelex (>=2021.5.3); extra == "scikit-learn-intelex"
+Requires-Dist: scikit-learn-intelex (>=2021.5.3) ; extra == "scikit-learn-intelex"
 Requires-Dist: scikit-misc (>=0.1.4)
 Requires-Dist: session-info (>=1.0.0)
-Requires-Dist: tabulate (>=0.9.0,<0.10.0)
+Requires-Dist: tabulate (>=0.9.0)
+Requires-Dist: thefuzz[speedup] (>=0.19.0,<0.20.0)
 Project-URL: Documentation, https://ehrapy.readthedocs.io
 Project-URL: Repository, https://github.com/theislab/ehrapy
 Description-Content-Type: text/markdown
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Build](https://github.com/theislab/ehrapy/workflows/Build%20ehrapy%20Package/badge.svg)](https://github.com/theislab/ehrapy/actions?workflow=Package)
 [![Codecov](https://codecov.io/gh/theislab/ehrapy/branch/master/graph/badge.svg)](https://codecov.io/gh/theislab/ehrapy)
@@ -62,22 +58,22 @@
 [![Test](https://github.com/theislab/ehrapy/workflows/Run%20ehrapy%20Tests/badge.svg)](https://github.com/theislab/ehrapy/actions?workflow=Tests)
 [![PyPI](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 <img src="https://user-images.githubusercontent.com/21954664/156930990-0d668468-0cd9-496e-995a-96d2c2407cf5.png" alt="ehrapy logo">
 
 # ehrapy overview
 
-<img src="https://user-images.githubusercontent.com/21954664/183865403-a2d61033-413e-4ae8-82cd-a9b6daa4fc18.png" alt="ehrapy overview">
+<img src="https://user-images.githubusercontent.com/99650244/217562449-e05ab1dd-9c04-44fc-a042-b993dd9d4eea.png" alt="ehrapy overview">
 
 ## Features
 
--   Exploratory analysis of Electronic Health Records
+-   Exploratory and targeted analysis of Electronic Health Records
 -   Quality control & preprocessing
--   Clustering & trajectory inference
 -   Visualization & Exploration
+-   Clustering & trajectory inference
 
 ## Installation
 
 You can install _ehrapy_ via [pip] from [PyPI]:
 
 ```console
 $ pip install ehrapy
```

