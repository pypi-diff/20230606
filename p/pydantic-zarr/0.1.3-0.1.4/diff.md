# Comparing `tmp/pydantic_zarr-0.1.3.tar.gz` & `tmp/pydantic_zarr-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_zarr-0.1.3.tar", max compression
+gzip compressed data, was "pydantic_zarr-0.1.4.tar", max compression
```

## Comparing `pydantic_zarr-0.1.3.tar` & `pydantic_zarr-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1070 2023-05-30 21:01:34.647934 pydantic_zarr-0.1.3/LICENSE
--rw-r--r--   0        0        0      505 2023-05-31 17:55:46.852124 pydantic_zarr-0.1.3/README.md
--rw-r--r--   0        0        0      489 2023-06-05 13:59:26.020614 pydantic_zarr-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       85 2023-06-03 15:04:37.431488 pydantic_zarr-0.1.3/src/pydantic_zarr/__init__.py
--rw-r--r--   0        0        0     9934 2023-06-05 13:57:00.113260 pydantic_zarr-0.1.3/src/pydantic_zarr/core.py
--rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 pydantic_zarr-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-30 21:01:34.647934 pydantic_zarr-0.1.4/LICENSE
+-rw-r--r--   0        0        0      505 2023-05-31 17:55:46.852124 pydantic_zarr-0.1.4/README.md
+-rw-r--r--   0        0        0      489 2023-06-06 17:15:04.490352 pydantic_zarr-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       85 2023-06-03 15:04:37.431488 pydantic_zarr-0.1.4/src/pydantic_zarr/__init__.py
+-rw-r--r--   0        0        0    10205 2023-06-06 02:43:26.838747 pydantic_zarr-0.1.4/src/pydantic_zarr/core.py
+-rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 pydantic_zarr-0.1.4/PKG-INFO
```

### Comparing `pydantic_zarr-0.1.3/LICENSE` & `pydantic_zarr-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_zarr-0.1.3/src/pydantic_zarr/core.py` & `pydantic_zarr-0.1.4/src/pydantic_zarr/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from pydantic.generics import GenericModel
 from zarr.storage import init_group, BaseStore
 import numcodecs
 import zarr
 import os
 import numpy as np
+from numcodecs.abc import Codec
 
 TAttrs = TypeVar("TAttrs", bound=Mapping[str, Any])
 TItem = TypeVar("TItem", bound=Union["GroupSpec", "ArraySpec"])
 
 DimensionSeparator = Union[Literal["."], Literal["/"]]
 ZarrVersion = Union[Literal[2], Literal[3]]
 ArrayOrder = Union[Literal["C"], Literal["F"]]
@@ -29,27 +30,27 @@
 class NodeSpec(GenericModel, Generic[TAttrs]):
     """
     The base class for ArraySpec and GroupSpec. Generic with respect to the type of
     attrs.
     """
 
     zarr_version: ZarrVersion = 2
-    attrs: TAttrs
 
     class Config:
         extra = "forbid"
 
 
 class ArraySpec(NodeSpec, Generic[TAttrs]):
     """
     This pydantic model represents the structural properties of a zarr array.
     It does not represent the data contained in the array. It is generic with respect to
     the type of attrs.
     """
 
+    attrs: TAttrs
     shape: tuple[int, ...]
     chunks: tuple[int, ...]
     dtype: str
     fill_value: Union[None, int, float] = 0
     order: ArrayOrder = "C"
     filters: Optional[list[dict[str, Any]]] = None
     dimension_separator: DimensionSeparator = "/"
@@ -60,14 +61,30 @@
         """
         Convert a np.dtype object into a string
         """
         if isinstance(v, np.dtype):
             return str(v)
         return v
 
+    @validator("compressor", pre=True)
+    def jsonify_compressor(cls, v):
+        if isinstance(v, Codec):
+            v = v.get_config()
+        return v
+
+    @validator("filters", pre=True)
+    def jsonify_filters(cls, v):
+        if v is not None:
+            try:
+                v = [element.get_config() for element in v]
+                return v
+            except AttributeError:
+                pass
+        return v
+
     @root_validator
     def check_ndim(cls, values):
         if (lshape := len(values["shape"])) != (lchunks := len(values["chunks"])):
             msg = f"""
             Length of shape must match length of chunks. Got {lshape} elements
             for shape and {lchunks} elements for chunks.
             """
@@ -85,31 +102,23 @@
 
         Returns
         -------
         An instance of ArraySpec with properties derived from the provided zarr
         array.
 
         """
-
-        filters = zarray.filters
-        if filters is not None:
-            filters = [f.get_config() for f in filters]
-
-        compressor = zarray.compressor
-        if compressor is not None:
-            compressor = compressor.get_config()
         return cls(
             shape=zarray.shape,
             chunks=zarray.chunks,
             dtype=str(zarray.dtype),
             fill_value=zarray.fill_value,
             order=zarray.order,
-            filters=filters,
+            filters=zarray.filters,
             dimension_separator=zarray._dimension_separator,
-            compressor=compressor,
+            compressor=zarray.compressor,
             attrs=dict(zarray.attrs),
         )
 
     def to_zarr(
         self, store: BaseStore, path: str, overwrite: bool = False
     ) -> zarr.Array:
         """
@@ -143,18 +152,19 @@
             ]
         result = zarr.create(store=store, path=path, **spec_dict, overwrite=overwrite)
         result.attrs.put(attrs)
         return result
 
 
 class GroupSpec(NodeSpec, Generic[TAttrs, TItem]):
+    attrs: TAttrs
     items: dict[str, TItem] = {}
 
     @classmethod
-    def from_zarr(cls, zgroup: zarr.Group) -> "GroupSpec":
+    def from_zarr(cls, zgroup: zarr.Group) -> "GroupSpec[TAttrs, TItem]":
         """
         Create a GroupSpec from a zarr group. Subgroups and arrays contained in the zarr
         group will be converted to instances of GroupSpec and ArraySpec, respectively,
         and these spec instances will be stored in the .items attribute of the parent
         GroupSpec. This occurs recursively, so the entire zarr hierarchy below a given
         group can be represented as a GroupSpec.
 
@@ -162,30 +172,31 @@
         ----------
         zgroup : zarr group
 
         Returns
         -------
         An instance of GroupSpec that represents the structure of the zarr hierarchy.
         """
-        result: GroupSpec
+
+        result: GroupSpec[TAttrs, TItem]
         items = {}
         for name, item in zgroup.items():
             if isinstance(item, zarr.Array):
                 _item = ArraySpec.from_zarr(item)
             elif isinstance(item, zarr.Group):
                 _item = cls.from_zarr(item)
             else:
                 msg = f"""
                 Unparseable object encountered: {type(item)}. Expected zarr.Array or
                 zarr.Group.
                 """
                 raise ValueError(msg)
             items[name] = _item
 
-        result = GroupSpec(attrs=dict(zgroup.attrs), items=items)
+        result = cls(attrs=dict(zgroup.attrs), items=items)
         return result
 
     def to_zarr(self, store: BaseStore, path: str, overwrite: bool = False):
         """
         Serialize a GroupSpec to a zarr group at a specific path in a zarr store.
 
         Parameters
```

### Comparing `pydantic_zarr-0.1.3/PKG-INFO` & `pydantic_zarr-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-zarr
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Davis Vann Bennett
 Author-email: davis.v.bennett@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

