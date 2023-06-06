# Comparing `tmp/pydantic_zarr-0.1.4.tar.gz` & `tmp/pydantic_zarr-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_zarr-0.1.4.tar", max compression
+gzip compressed data, was "pydantic_zarr-0.2.0.tar", max compression
```

## Comparing `pydantic_zarr-0.1.4.tar` & `pydantic_zarr-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1070 2023-05-30 21:01:34.647934 pydantic_zarr-0.1.4/LICENSE
--rw-r--r--   0        0        0      505 2023-05-31 17:55:46.852124 pydantic_zarr-0.1.4/README.md
--rw-r--r--   0        0        0      489 2023-06-06 17:15:04.490352 pydantic_zarr-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       85 2023-06-03 15:04:37.431488 pydantic_zarr-0.1.4/src/pydantic_zarr/__init__.py
--rw-r--r--   0        0        0    10205 2023-06-06 02:43:26.838747 pydantic_zarr-0.1.4/src/pydantic_zarr/core.py
--rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 pydantic_zarr-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-30 21:01:34.647934 pydantic_zarr-0.2.0/LICENSE
+-rw-r--r--   0        0        0      505 2023-05-31 17:55:46.852124 pydantic_zarr-0.2.0/README.md
+-rw-r--r--   0        0        0      489 2023-06-06 19:15:25.723765 pydantic_zarr-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       85 2023-06-03 15:04:37.431488 pydantic_zarr-0.2.0/src/pydantic_zarr/__init__.py
+-rw-r--r--   0        0        0    10522 2023-06-06 19:14:28.300772 pydantic_zarr-0.2.0/src/pydantic_zarr/core.py
+-rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 pydantic_zarr-0.2.0/PKG-INFO
```

### Comparing `pydantic_zarr-0.1.4/LICENSE` & `pydantic_zarr-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_zarr-0.1.4/src/pydantic_zarr/core.py` & `pydantic_zarr-0.2.0/src/pydantic_zarr/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from pydantic.generics import GenericModel
 from zarr.storage import init_group, BaseStore
 import numcodecs
 import zarr
 import os
 import numpy as np
+import numpy.typing as npt
 from numcodecs.abc import Codec
 
 TAttrs = TypeVar("TAttrs", bound=Mapping[str, Any])
 TItem = TypeVar("TItem", bound=Union["GroupSpec", "ArraySpec"])
 
 DimensionSeparator = Union[Literal["."], Literal["/"]]
 ZarrVersion = Union[Literal[2], Literal[3]]
@@ -88,14 +89,25 @@
             Length of shape must match length of chunks. Got {lshape} elements
             for shape and {lchunks} elements for chunks.
             """
             raise ValueError(msg)
         return values
 
     @classmethod
+    def from_array(cls, array: npt.NDArray[Any], **kwargs):
+
+        return cls(
+            shape=array.shape,
+            dtype=array.dtype,
+            chunks=kwargs.pop("chunks", array.shape),
+            attrs=kwargs.pop("attrs", {}),
+            **kwargs,
+        )
+
+    @classmethod
     def from_zarr(cls, zarray: zarr.Array):
         """
         Create an ArraySpec from a zarr array.
 
         Parameters
         ----------
         zarray : zarr array
```

### Comparing `pydantic_zarr-0.1.4/PKG-INFO` & `pydantic_zarr-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-zarr
-Version: 0.1.4
+Version: 0.2.0
 Summary: 
 Author: Davis Vann Bennett
 Author-email: davis.v.bennett@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

