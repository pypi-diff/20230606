# Comparing `tmp/h5pydantic-0.3.0.tar.gz` & `tmp/h5pydantic-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h5pydantic-0.3.0.tar", max compression
+gzip compressed data, was "h5pydantic-0.3.1.tar", max compression
```

## Comparing `h5pydantic-0.3.0.tar` & `h5pydantic-0.3.1.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0      340 2023-05-13 03:54:48.206900 h5pydantic-0.3.0/README.md
--rw-r--r--   0        0        0     1219 2023-05-17 01:26:58.110102 h5pydantic-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      115 2023-05-17 00:29:12.901569 h5pydantic-0.3.0/src/h5pydantic/__init__.py
--rw-r--r--   0        0        0     5726 2023-05-17 01:27:57.055075 h5pydantic-0.3.0/src/h5pydantic/model.py
--rw-r--r--   0        0        0       12 2023-05-17 00:25:11.728066 h5pydantic-0.3.0/src/h5pydantic/newsfragments/.gitignore
--rw-r--r--   0        0        0     1266 1970-01-01 00:00:00.000000 h5pydantic-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      340 2023-06-05 10:27:55.276860 h5pydantic-0.3.1/README.md
+-rw-r--r--   0        0        0     1379 2023-06-06 09:26:09.304108 h5pydantic-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      146 2023-06-06 09:26:14.931979 h5pydantic-0.3.1/src/h5pydantic/__init__.py
+-rw-r--r--   0        0        0     6198 2023-06-06 09:26:14.931979 h5pydantic-0.3.1/src/h5pydantic/model.py
+-rw-r--r--   0        0        0       12 2023-06-05 10:27:55.276860 h5pydantic-0.3.1/src/h5pydantic/newsfragments/.gitignore
+-rw-r--r--   0        0        0      130 2023-06-06 10:22:56.486499 h5pydantic-0.3.1/src/h5pydantic/newsfragments/multi.feature
+-rw-r--r--   0        0        0      263 2023-06-05 10:27:55.276860 h5pydantic-0.3.1/src/h5pydantic/types.py
+-rw-r--r--   0        0        0     1367 1970-01-01 00:00:00.000000 h5pydantic-0.3.1/PKG-INFO
```

### Comparing `h5pydantic-0.3.0/pyproject.toml` & `h5pydantic-0.3.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "h5pydantic"
-version = "0.3.0"
+version = "0.3.1"
 description = "Pydantic models for HDF5 files."
 authors = ["Clinton Roy <clinton.roy@gmail.com>"]
 readme = "README.md"
 repository = "https://gitlab.com/clinton.roy/h5pydantic"
 documentation = "https://h5pydantic.readthedocs.io/"
 packages = [{include = "h5pydantic", from = "src"}]
 classifiers = [
@@ -13,22 +13,25 @@
             "Natural Language :: English",
 	    "Topic :: File Formats",
             "Topic :: Scientific/Engineering :: Information Analysis",
             "Intended Audience :: Science/Research",
             "License :: OSI Approved :: Python Software Foundation License",
 ]
 [tool.poetry.dependencies]
-python = "~3.9"
+python = "^3.9"
 h5py = "^3.8.0"
 pydantic = "^1.10.7"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 ruff = "^0.0.265"
 hypothesis = "^6.75.2"
+pytest-cov = "^4.0.0"
+coverage = "^7.2.5"
+mypy = "^1.3.0"
 
 [tool.poetry.group.doc.dependencies]
 sphinx-autodoc-typehints = "^1.23.0"
 sphinx-rtd-theme = "^1.2.0"
 sphinx = "6.2.1"
 towncrier = "^22.12.0"
 
@@ -39,7 +42,10 @@
 package = "h5pydantic"
 package_dir = "src"
 filename = "docs/news.rst"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poe.tasks]
+test = "pytest --verbose --cov --cov-fail-under=100 --cov-branch --cov-report=html"
```

### Comparing `h5pydantic-0.3.0/src/h5pydantic/model.py` & `h5pydantic-0.3.1/src/h5pydantic/model.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,37 @@
 import h5py
 from pydantic import BaseModel
 import numpy
 
-from abc import ABC
+from abc import ABC, abstractmethod
 from pathlib import Path, PurePosixPath
 import types
 
-from typing import Union
+from typing import Any, Union
 
 _H5Container = Union[h5py.Group, h5py.Dataset]
 
 
-class _H5Base(ABC):
+class _H5Base(ABC, BaseModel):
     """An implementation detail, to share the _load and _dump APIs."""
 
+    def __init__(self, **data: Any):
+        super().__init__(**data)
+        for key, field in self.__fields__.items():
+            if key.endswith("_"):
+                continue
+
+            if isinstance(field.outer_type_, types.GenericAlias):
+                # FIXME clearly I should not be looking at these attributes.
+                if not issubclass(field.outer_type_.__origin__, list):
+                    raise ValueError(f"h5pydantic only handles list containers, not '{field.outer_type_.__origin__}'")
+
+    @abstractmethod
     def _dump_container(self, h5file: h5py.File, prefix: PurePosixPath) -> _H5Container:
-        pass
+        """Dump the group/dataset container to the h5file."""
 
     def _dump_children(self, container: _H5Container, h5file: h5py.File, prefix: PurePosixPath):
         for key, field in self.__fields__.items():
             # FIXME I think I should be explicitly testing these keys against a known list, at init time though.
             if key.endswith("_"):
                 continue
             value = getattr(self, key)
@@ -43,41 +55,35 @@
     def _load_children(cls, h5file: h5py.File, prefix: PurePosixPath):
         d = {}
         for key, field in cls.__fields__.items():
             if key.endswith("_"):
                 continue
 
             if isinstance(field.outer_type_, types.GenericAlias):
-                # FIXME clearly I should not be looking at these attributes.
-                if not issubclass(field.outer_type_.__origin__, list):
-                    raise ValueError(f"h5pydantic only handles list containers, not '{field.outer_type_.__origin__}'")
-
                 d[key] = []
                 indexes = [int(i) for i in h5file[str(prefix / key)].keys()]
                 indexes.sort()
                 for i in indexes:
                     # FIXME This doesn't check a lot of cases.
                     d[key].insert(i, field.type_._load(h5file, prefix / key / str(i)))
             elif issubclass(field.type_, _H5Base):
                 d[key] = field.type_._load(h5file, prefix / key)
-            elif issubclass(field.type_, list):
-                pass
             else:
                 d[key] = h5file[str(prefix)].attrs[key]
 
         return d
 
     @classmethod
     def _load(cls, h5file: h5py.File, prefix: PurePosixPath) -> tuple["H5Group", list[str]]:
         d = cls._load_intrinsic(h5file, prefix)
         d.update(cls._load_children(h5file, prefix))
         return cls.parse_obj(d)
 
 
-class H5Dataset(_H5Base, BaseModel):
+class H5Dataset(_H5Base):
     """A pydantic Basemodel specifying a HDF5 Dataset."""
 
     class Config:
         # Allows numpy.ndarray (which doesn't have a validator).
         arbitrary_types_allowed = True
 
     # FIXME check that all underscore attributes are special attributes
@@ -87,45 +93,45 @@
     # FIXME test for attributes on datasets
     # FIXME I'm not comfortable with shadowing these fields like this,
     # but it's nice to have some ns to put config variables in.
     shape_: tuple[int, ...]
     dtype_: str = "f"
 
     # FIXME is it possible to initialise this after we've got shape_ and dtype_ in the instance?
-    data_: h5py.Dataset = None
+    data_: Union[h5py.Dataset, numpy.ndarray] = None
 
     def _dump_container(self, h5file: h5py.File, prefix: PurePosixPath) -> h5py.Dataset:
         # FIXME check that the shape of data matches
         # FIXME add in all the other flags
         dataset = h5file.require_dataset(str(prefix), shape=self.shape_, dtype=self.dtype_)
         dataset[:] = self.data_
         return dataset
 
     @classmethod
     def _load_intrinsic(cls: BaseModel, h5file: h5py.File, prefix: PurePosixPath):
         # Really should be verifying all of the details match the class.
-        data = h5file[str(prefix)]
+        data = h5file[str(prefix)][()]
         return {"shape_": data.shape, "dtype_": str(data.dtype), "data_": data}
 
+    def __eq__(self, other):
+        intrinsic = numpy.array_equal(self.data_, other.data_)
+        children = all([getattr(self, k) == getattr(other, k) for k in self.__fields__ if not k.endswith("_")])
+        return intrinsic and children
+
 
-class H5Group(_H5Base, BaseModel):
+class H5Group(_H5Base):
     """A pydantic BaseModel specifying a HDF5 Group."""
 
     class Config:
         # For the _h5file attribute.
         underscore_attrs_are_private = True
 
     _h5file: h5py.File = None
 
     @classmethod
-    def _load_container(cls, h5file: h5py.File, prefix: PurePosixPath) -> _H5Container:
-        group = h5file[str(prefix)]
-        return group
-
-    @classmethod
     def load(cls: BaseModel, filename: Path) -> "H5Group":
         """Load a file into a tree of H5Group models.
 
         Args:
             filename: Path of HDF5 to load.
 
         Returns:
@@ -139,16 +145,15 @@
 
     def close(self):
         """Close the underlying HDF5 file.
         """
         self._h5file.close()
 
     def __enter__(self):
-        if self._h5file:
-            return self
+        return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
     def _dump_container(self, h5file: h5py.File, prefix: PurePosixPath) -> h5py.Group:
         return h5file.require_group(str(prefix))
 
@@ -158,7 +163,10 @@
         Args:
             filename: Path to dump the the HDF5Group to.
 
         Returns: None
 """
         with h5py.File(filename, "w") as h5file:
             self._dump(h5file, PurePosixPath("/"))
+
+    def __eq__(self, other):
+        return all([getattr(self, k) == getattr(other, k) for k in self.__fields__ if not k.endswith("_")])
```

### Comparing `h5pydantic-0.3.0/PKG-INFO` & `h5pydantic-0.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: h5pydantic
-Version: 0.3.0
+Version: 0.3.1
 Summary: Pydantic models for HDF5 files.
 Home-page: https://gitlab.com/clinton.roy/h5pydantic
 Author: Clinton Roy
 Author-email: clinton.roy@gmail.com
-Requires-Python: >=3.9,<3.10
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Pydantic
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Python Software Foundation License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: File Formats
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Dist: h5py (>=3.8.0,<4.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Project-URL: Documentation, https://h5pydantic.readthedocs.io/
 Project-URL: Repository, https://gitlab.com/clinton.roy/h5pydantic
 Description-Content-Type: text/markdown
```

