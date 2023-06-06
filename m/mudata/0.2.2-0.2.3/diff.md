# Comparing `tmp/mudata-0.2.2.tar.gz` & `tmp/mudata-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mudata-0.2.2.tar", last modified: Thu Apr  6 16:29:08 2023, max compression
+gzip compressed data, was "mudata-0.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mudata-0.2.2.tar` & `mudata-0.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2694 2022-11-04 19:52:22.862864 mudata-0.2.2/README.md
--rw-r--r--   0        0        0      243 2023-04-06 16:24:48.986123 mudata-0.2.2/mudata/__init__.py
--rw-r--r--   0        0        0        0 2022-11-04 19:52:22.871585 mudata-0.2.2/mudata/_core/__init__.py
--rw-r--r--   0        0        0     1598 2022-11-04 19:52:22.871753 mudata-0.2.2/mudata/_core/config.py
--rw-r--r--   0        0        0     3540 2023-04-06 16:24:48.986840 mudata-0.2.2/mudata/_core/file_backing.py
--rw-r--r--   0        0        0    19483 2023-04-06 16:24:48.987829 mudata-0.2.2/mudata/_core/io.py
--rw-r--r--   0        0        0    51789 2023-04-06 16:24:48.988971 mudata-0.2.2/mudata/_core/mudata.py
--rw-r--r--   0        0        0     8343 2022-11-04 19:52:22.872892 mudata-0.2.2/mudata/_core/repr.py
--rw-r--r--   0        0        0      662 2022-11-04 19:52:22.873192 mudata-0.2.2/mudata/_core/utils.py
--rw-r--r--   0        0        0     1094 2023-04-06 16:24:48.990836 mudata-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3824 1970-01-01 00:00:00.000000 mudata-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     3554 2023-06-06 09:10:56.440148 mudata-0.2.3/README.md
+-rw-r--r--   0        0        0      243 2023-06-06 09:10:56.440635 mudata-0.2.3/mudata/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-04 19:52:22.871585 mudata-0.2.3/mudata/_core/__init__.py
+-rw-r--r--   0        0        0     1598 2022-11-04 19:52:22.871753 mudata-0.2.3/mudata/_core/config.py
+-rw-r--r--   0        0        0     3540 2023-04-06 16:24:48.986840 mudata-0.2.3/mudata/_core/file_backing.py
+-rw-r--r--   0        0        0    19503 2023-06-06 09:10:56.441334 mudata-0.2.3/mudata/_core/io.py
+-rw-r--r--   0        0        0    53761 2023-06-06 09:10:56.442640 mudata-0.2.3/mudata/_core/mudata.py
+-rw-r--r--   0        0        0     8956 2023-06-06 09:10:56.444061 mudata-0.2.3/mudata/_core/repr.py
+-rw-r--r--   0        0        0     1037 2023-06-06 09:10:56.444511 mudata-0.2.3/mudata/_core/utils.py
+-rw-r--r--   0        0        0     1094 2023-04-06 16:24:48.990836 mudata-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4684 1970-01-01 00:00:00.000000 mudata-0.2.3/PKG-INFO
```

### Comparing `mudata-0.2.2/README.md` & `mudata-0.2.3/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -74,7 +74,24 @@
 It allows to effectively use the hierarchical nature of HDF5 files and to read/write AnnData object directly from/to `.h5mu` files:
 
 ```py
 adata = md.read("pbmc_10k.h5mu/rna")
 md.write("pbmc_10k.h5mu/rna", adata)
 ```
 
+## Citation
+
+If you use `mudata` in your work, please cite the `muon/mudata` publication as follows:
+
+> **MUON: multimodal omics analysis framework**
+> 
+> Danila Bredikhin, Ilia Kats, Oliver Stegle
+>
+> _Genome Biology_ 2022 Feb 01. doi: [10.1186/s13059-021-02577-8](https://doi.org/10.1186/s13059-021-02577-8).
+
+You can cite the scverse publication as follows:
+
+> **The scverse project provides a computational ecosystem for single-cell omics data analysis**
+>
+> Isaac Virshup, Danila Bredikhin, Lukas Heumos, Giovanni Palla, Gregor Sturm, Adam Gayoso, Ilia Kats, Mikaela Koutrouli, Scverse Community, Bonnie Berger, Dana Pe’er, Aviv Regev, Sarah A. Teichmann, Francesca Finotello, F. Alexander Wolf, Nir Yosef, Oliver Stegle & Fabian J. Theis
+>
+> _Nat Biotechnol._ 2022 Apr 10. doi: [10.1038/s41587-023-01733-8](https://doi.org/10.1038/s41587-023-01733-8).
```

### Comparing `mudata-0.2.2/mudata/_core/config.py` & `mudata-0.2.3/mudata/_core/config.py`

 * *Files identical despite different names*

### Comparing `mudata-0.2.2/mudata/_core/file_backing.py` & `mudata-0.2.3/mudata/_core/file_backing.py`

 * *Files identical despite different names*

### Comparing `mudata-0.2.2/mudata/_core/io.py` & `mudata-0.2.3/mudata/_core/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
         adata = mdata.mod[k]
 
         adata.strings_to_categoricals()
         if adata.raw is not None:
             adata.strings_to_categoricals(adata.raw.var)
 
-        if write_data:
+        if write_data or not adata.isbacked:
             write_elem(group, "X", adata.X, dataset_kwargs=kwargs)
         if adata.raw is not None:
             write_elem(group, "raw", adata.raw)
 
         write_elem(group, "obs", adata.obs, dataset_kwargs=kwargs)
         write_elem(group, "var", adata.var, dataset_kwargs=kwargs)
         write_elem(group, "obsm", dict(adata.obsm), dataset_kwargs=kwargs)
@@ -154,15 +154,15 @@
 
             adata = mdata.mod[k]
 
             adata.strings_to_categoricals()
             if adata.raw is not None:
                 adata.strings_to_categoricals(adata.raw.var)
 
-            if write_data:
+            if write_data or not adata.isbacked:
                 if chunks is not None and not isinstance(adata.X, sparse.spmatrix):
                     write_elem(group, "X", adata.X, dataset_kwargs=dict(chunks=chunks, **kwargs))
                 else:
                     write_elem(group, "X", adata.X, dataset_kwargs=kwargs)
             if adata.raw is not None:
                 write_elem(group, "raw", adata.raw)
 
@@ -302,15 +302,15 @@
         ), "Can only save MuData object to .h5mu file"
 
         write_h5mu(filename, data)
 
     else:
         assert isinstance(data, AnnData), "Only MuData and AnnData objects are accepted"
 
-        m = re.search("^(.+)\.(h5mu)[/]?([A-Za-z]*)[/]?([/A-Za-z]*)$", str(filename))
+        m = re.search("^(.+)\.(h5mu)[/]?([^/]*)[/]?(.*)$", str(filename))
         if m is not None:
             m = m.groups()
         else:
             raise ValueError("Expected non-empty .h5ad or .h5mu file name")
 
         filepath = ".".join([m[0], m[1]])
 
@@ -578,15 +578,15 @@
       - FILE.h5mu
       - FILE.h5mu/MODALITY
       - FILE.h5mu/mod/MODALITY
       - FILE.h5ad
     """
     import re
 
-    m = re.search("^(.+)\.(h5mu)[/]?([A-Za-z]*)[/]?([/A-Za-z]*)$", str(filename))
+    m = re.search("^(.+)\.(h5mu)[/]?([^/]*)[/]?(.*)$", str(filename))
     if m is not None:
         m = m.groups()
     else:
         if filename.endswith(".h5ad"):
             m = [filename[:-5], "h5ad", "", ""]
         else:
             raise ValueError("Expected non-empty .h5ad or .h5mu file name")
```

### Comparing `mudata-0.2.2/mudata/_core/mudata.py` & `mudata-0.2.3/mudata/_core/mudata.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     AxisArraysBase,
     PairwiseArrays,
     PairwiseArraysView,
 )
 from anndata._core.views import DataFrameView
 
 from .file_backing import MuDataFileManager
-from .utils import _make_index_unique, _restore_index
+from .utils import _make_index_unique, _restore_index, _maybe_coerce_to_boolean
 
 from .repr import *
 from .config import OPTIONS
 
 
 class MuAxisArraysView(AlignedViewMixin, AxisArraysBase):
     def __init__(self, parent_mapping: AxisArraysBase, parent_view: "MuData", subset_idx: Any):
@@ -186,41 +186,66 @@
             varidx = slice(varidx, varidx + 1)
 
         self.mod = dict()
         for m, a in mudata_ref.mod.items():
             cobsidx, cvaridx = mudata_ref.obsmap[m][obsidx], mudata_ref.varmap[m][varidx]
             cobsidx, cvaridx = cobsidx[cobsidx > 0] - 1, cvaridx[cvaridx > 0] - 1
             if len(cobsidx) > 0 and len(cvaridx) > 0:
-                if len(cobsidx) == a.n_obs and np.all(np.diff(cobsidx) == 1):
-                    cobsidx = slice(None)
-                if len(cvaridx) == a.n_vars and np.all(np.diff(cvaridx) == 1):
-                    cvaridx = slice(None)
-            self.mod[m] = a[cobsidx, cvaridx]
+                if np.all(np.diff(cobsidx) == 1):
+                    if a.is_view:
+                        if (
+                            isinstance(a, MuData)
+                            and len(cobsidx) == a._mudata_ref.n_obs
+                            or isinstance(a, AnnData)
+                            and len(cobsidx) == a._adata_ref.n_obs
+                        ):
+                            cobsidx = slice(None)
+                    elif len(cobsidx) == a.n_obs:
+                        cobsidx = slice(None)
+                if np.all(np.diff(cvaridx) == 1):
+                    if a.is_view:
+                        if (
+                            isinstance(a, MuData)
+                            and len(cvaridx) == a._mudata_ref.n_vars
+                            or isinstance(a, AnnData)
+                            and len(cvaridx) == a._adata_ref.n_vars
+                        ):
+                            cvaridx = slice(None)
+                    elif len(cvaridx) == a.n_vars:
+                        cvaridx = slice(None)
+            if a.is_view:
+                if isinstance(a, MuData):
+                    self.mod[m] = a._mudata_ref[cobsidx, cvaridx]
+                else:
+                    self.mod[m] = a._adata_ref[cobsidx, cvaridx]
+            else:
+                self.mod[m] = a[cobsidx, cvaridx]
 
         self._obs = DataFrameView(mudata_ref.obs.iloc[obsidx, :], view_args=(self, "obs"))
         self._obsm = mudata_ref.obsm._view(self, (obsidx,))
         self._obsp = mudata_ref.obsp._view(self, obsidx)
         self._var = DataFrameView(mudata_ref.var.iloc[varidx, :], view_args=(self, "var"))
         self._varm = mudata_ref.varm._view(self, (varidx,))
         self._varp = mudata_ref.varp._view(self, varidx)
 
         for attr, idx in (("obs", obsidx), ("var", varidx)):
             posmap = {}
             for mod, mapping in getattr(mudata_ref, attr + "map").items():
-                newmap = mapping[idx]
-                nz = newmap > 0
-                newmap[nz] = np.nonzero(nz)[0] + np.uint(1)
-                posmap[mod] = newmap
+                posmap[mod] = mapping[idx].copy()
             setattr(self, "_" + attr + "map", posmap)
 
         self.is_view = True
         self.file = mudata_ref.file
-        self._mudata_ref = mudata_ref
         self._axis = mudata_ref._axis
 
+        if mudata_ref.is_view:
+            self._mudata_ref = mudata_ref._mudata_ref
+        else:
+            self._mudata_ref = mudata_ref
+
     def _init_as_actual(self, data: "MuData"):
         self._init_common()
         self.mod = data.mod
         self._obs = data.obs
         self._var = data.var
         self._obsm = MuAxisArrays(self, 0, convert_to_dict(data.obsm))
         self._obsp = PairwiseArrays(self, 0, convert_to_dict(data.obsp))
@@ -243,15 +268,24 @@
         obsp: Optional[Union[np.ndarray, Mapping[str, Sequence[Any]]]] = None,
         varp: Optional[Union[np.ndarray, Mapping[str, Sequence[Any]]]] = None,
         obsmap: Optional[Mapping[str, Sequence[int]]] = None,
         varmap: Optional[Mapping[str, Sequence[int]]] = None,
         axis: Literal[0, 1] = 0,
     ):
         return cls(
-            data={k: (v if isinstance(v, AnnData) else AnnData(**v)) for k, v in mod.items()},
+            data={
+                k: (
+                    v
+                    if isinstance(v, AnnData) or isinstance(v, MuData)
+                    else MuData(**v)
+                    if "mod" in v
+                    else AnnData(**v)
+                )
+                for k, v in mod.items()
+            },
             obs=obs,
             var=var,
             uns=uns,
             obsm=obsm,
             varm=varm,
             obsp=obsp,
             varp=varp,
@@ -537,15 +571,18 @@
                             for m, a in self.mod.items()
                         ],
                         join="outer",
                         axis=0,
                         sort=False,
                     )
                     data_common = pd.concat(
-                        [getattr(a, attr)[columns_common] for m, a in self.mod.items()],
+                        [
+                            _maybe_coerce_to_boolean(getattr(a, attr)[columns_common])
+                            for m, a in self.mod.items()
+                        ],
                         join="outer",
                         axis=0,
                         sort=False,
                     )
                     data_mod = data_mod.join(data_common, how="left", sort=False)
 
                     # this occurs when join_common=True and we already have a global data frame, e.g. after reading from H5MU
@@ -567,51 +604,54 @@
                     )
 
             for mod, amod in self.mod.items():
                 colname = mod + ":" + rowcol
                 # use 0 as special value for missing
                 # we could use a pandas.array, which has missing values support, but then we get an Exception upon hdf5 write
                 # also, this is compatible to Muon.jl
-                col = data_mod.loc[:, colname] + 1
+                col = data_mod[colname] + 1
                 col.replace(np.NaN, 0, inplace=True)
-                col = col.astype(np.uint32)
-                data_mod.loc[:, colname] = col
+                data_mod[colname] = col.astype(np.uint32)
 
             if len(data_global.columns) > 0:
                 # TODO: if there were intersecting attrnames between modalities,
                 #       this will increase the size of the index
                 # Should we use attrmap to figure the index out?
                 data_mod = data_mod.join(data_global, how="left", sort=False)
 
         #
         # General case: with duplicates and/or intersections
         #
         else:
             if join_common:
                 dfs = [
-                    _make_index_unique(
-                        getattr(a, attr)
-                        .drop(columns_common, axis=1)
-                        .assign(**{rowcol: np.arange(getattr(a, attr).shape[0])})
-                        .add_prefix(m + ":")
+                    _maybe_coerce_to_boolean(
+                        _make_index_unique(
+                            getattr(a, attr)
+                            .drop(columns_common, axis=1)
+                            .assign(**{rowcol: np.arange(getattr(a, attr).shape[0])})
+                            .add_prefix(m + ":")
+                        )
                     )
                     for m, a in self.mod.items()
                 ]
 
                 # Here, attr_names are guaranteed to be unique and are safe to be used for joins
                 data_mod = pd.concat(
                     dfs,
                     join="outer",
                     axis=axis,
                     sort=False,
                 )
 
                 data_common = pd.concat(
                     [
-                        _make_index_unique(getattr(a, attr)[columns_common])
+                        _maybe_coerce_to_boolean(
+                            _make_index_unique(getattr(a, attr)[columns_common])
+                        )
                         for m, a in self.mod.items()
                     ],
                     join="outer",
                     axis=0,
                     sort=False,
                 )
                 data_mod = data_mod.join(data_common, how="left", sort=False)
@@ -1191,15 +1231,16 @@
         """
         Write MuData object to a Zarr store
         """
         from .io import write_zarr
 
         write_zarr(store, self, **kwargs)
 
-    def _gen_repr(self, n_obs, n_vars, extensive: bool = False) -> str:
+    def _gen_repr(self, n_obs, n_vars, extensive: bool = False, nest_level: int = 0) -> str:
+        indent = "    " * nest_level
         backed_at = f" backed at {str(self.filename)!r}" if self.isbacked else ""
         view_of = "View of " if self.is_view else ""
         descr = f"{view_of}MuData object with n_obs × n_vars = {n_obs} × {n_vars}{backed_at}"
         for attr in ["obs", "var", "uns", "obsm", "varm", "obsp", "varp"]:
             if hasattr(self, attr) and getattr(self, attr) is not None:
                 keys = list(getattr(self, attr).keys())
                 if len(keys) > 0:
@@ -1217,31 +1258,40 @@
                                         for mod in self.mod
                                     ]
                                 )
                             ),
                         )
                     )
                     if any(global_keys):
-                        descr += f"\n  {attr}:\t{str([keys[i] for i in range(len(keys)) if global_keys[i]])[1:-1]}"
-        descr += f"\n  {len(self.mod)} modalit{'y' if len(self.mod) == 1 else 'ies'}"
+                        descr += f"\n{indent}  {attr}:\t{str([keys[i] for i in range(len(keys)) if global_keys[i]])[1:-1]}"
+        descr += f"\n{indent}  {len(self.mod)} modalit{'y' if len(self.mod) == 1 else 'ies'}"
         for k, v in self.mod.items():
-            descr += f"\n    {k}:\t{v.n_obs} x {v.n_vars}"
+            mod_indent = "    " * (nest_level + 1)
+            if isinstance(v, MuData):
+                descr += f"\n{mod_indent}{k}:\t" + v._gen_repr(
+                    n_obs, n_vars, extensive, nest_level + 1
+                )
+                continue
+            descr += f"\n{mod_indent}{k}:\t{v.n_obs} x {v.n_vars}"
             for attr in [
                 "obs",
                 "var",
                 "uns",
                 "obsm",
                 "varm",
                 "layers",
                 "obsp",
                 "varp",
             ]:
-                keys = getattr(v, attr).keys()
-                if len(keys) > 0:
-                    descr += f"\n      {attr}:\t{str(list(keys))[1:-1]}"
+                try:
+                    keys = getattr(v, attr).keys()
+                    if len(keys) > 0:
+                        descr += f"\n{mod_indent}  {attr}:\t{str(list(keys))[1:-1]}"
+                except AttributeError:
+                    pass
         return descr
 
     def __repr__(self) -> str:
         return self._gen_repr(self.n_obs, self.n_vars, extensive=True)
 
     def _repr_html_(self, expand=None):
         """
```

### Comparing `mudata-0.2.2/mudata/_core/repr.py` & `mudata-0.2.3/mudata/_core/repr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #
 # Utility functions for MuData._repr_html_()
 #
 
 from typing import Tuple, Iterable
-from numbers import Integral, Real, Complex
+from numbers import Number, Integral, Real, Complex
 from warnings import warn
 import numpy as np
 import pandas as pd
 
 
 def maybe_module_class(obj, sep=".", builtins=False) -> Tuple[str, str]:
     m, cl = "", obj.__class__.__name__
@@ -34,34 +34,52 @@
             vs = ",".join(map(format_values, x.values()))
             s += ks + ": " + vs
         else:
             s += ks
     elif isinstance(x, str):
         s += x
     else:
+        if not len(x):
+            return s
         x = x[: min(100, len(x))]
+        testval = None
         if hasattr(x, "shape"):
             if isinstance(x, np.ndarray):
-                x = x.flat
+                x = x.reshape(-1)
             elif isinstance(x, pd.Series):
                 x = x.to_numpy()
             else:
                 warn(f"got unknown array type {type(x)}, don't know how handle it.")
                 return type(x)
-        if isinstance(x[0], Integral):
+            if x.dtype == object:
+                try:
+                    testval = next(
+                        filter(
+                            lambda y: ~np.isnan(y) if isinstance(y, Number) else x is not None,
+                            x,
+                        )
+                    )
+                except StopIteration:
+                    pass
+        if testval is None:
+            testval = x[0]
+        if (
+            isinstance(testval, Integral)
+            or isinstance(testval, np.bool_)
+            or isinstance(testval, bool)
+        ):
             s += ",".join([f"{i}" for i in x])
-        elif isinstance(x[0], Real):
+        elif isinstance(testval, Real):
             s += ",".join([f"{i:.2f}" for i in x])
-        elif isinstance(x[0], Complex):
+        elif isinstance(testval, Complex):
             warn("got complex number, don't know how to handle it")
-        elif isinstance(x[0], Iterable):
+        elif isinstance(testval, Iterable):
             s += ",".join(map(format_values, x))
-        s = s[:50]
-        while s[-1] != ",":
-            s = s[:-1]
+        lastidx = max(50, s.find(","))
+        s = s[:lastidx]
         s += "..."
     return s
 
 
 def block_matrix(data, attr, name):
     obj = getattr(data, attr)
     s = ""
```

### Comparing `mudata-0.2.2/pyproject.toml` & `mudata-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mudata-0.2.2/PKG-INFO` & `mudata-0.2.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mudata
-Version: 0.2.2
+Version: 0.2.3
 Summary: Multimodal omics analysis framework
 Home-page: https://github.com/scverse/mudata
 Author: Danila Bredikhin
 Author-email: danila.bredikhin@embl.de
 Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
@@ -104,8 +104,25 @@
 It allows to effectively use the hierarchical nature of HDF5 files and to read/write AnnData object directly from/to `.h5mu` files:
 
 ```py
 adata = md.read("pbmc_10k.h5mu/rna")
 md.write("pbmc_10k.h5mu/rna", adata)
 ```
 
+## Citation
+
+If you use `mudata` in your work, please cite the `muon/mudata` publication as follows:
+
+> **MUON: multimodal omics analysis framework**
+> 
+> Danila Bredikhin, Ilia Kats, Oliver Stegle
+>
+> _Genome Biology_ 2022 Feb 01. doi: [10.1186/s13059-021-02577-8](https://doi.org/10.1186/s13059-021-02577-8).
+
+You can cite the scverse publication as follows:
+
+> **The scverse project provides a computational ecosystem for single-cell omics data analysis**
+>
+> Isaac Virshup, Danila Bredikhin, Lukas Heumos, Giovanni Palla, Gregor Sturm, Adam Gayoso, Ilia Kats, Mikaela Koutrouli, Scverse Community, Bonnie Berger, Dana Pe’er, Aviv Regev, Sarah A. Teichmann, Francesca Finotello, F. Alexander Wolf, Nir Yosef, Oliver Stegle & Fabian J. Theis
+>
+> _Nat Biotechnol._ 2022 Apr 10. doi: [10.1038/s41587-023-01733-8](https://doi.org/10.1038/s41587-023-01733-8).
```

