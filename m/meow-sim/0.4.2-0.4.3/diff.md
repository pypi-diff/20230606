# Comparing `tmp/meow-sim-0.4.2.tar.gz` & `tmp/meow-sim-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow-sim-0.4.2.tar", last modified: Tue Jun  6 03:45:49 2023, max compression
+gzip compressed data, was "meow-sim-0.4.3.tar", last modified: Tue Jun  6 21:21:53 2023, max compression
```

## Comparing `meow-sim-0.4.2.tar` & `meow-sim-0.4.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 03:45:49.285664 meow-sim-0.4.2/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-06-06 03:45:44.000000 meow-sim-0.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3078 2023-06-06 03:45:49.281664 meow-sim-0.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2060 2023-06-06 03:45:44.000000 meow-sim-0.4.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 03:45:49.281664 meow-sim-0.4.2/meow/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 03:45:49.281664 meow-sim-0.4.2/meow/assets/
--rw-r--r--   0 root         (0) root         (0)    10307 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/assets/silicon.csv
--rw-r--r--   0 root         (0) root         (0)     8535 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/assets/silicon_oxide.csv
--rw-r--r--   0 root         (0) root         (0)     8019 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/base_model.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/cache.py
--rw-r--r--   0 root         (0) root         (0)     4844 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/cell.py
--rw-r--r--   0 root         (0) root         (0)     2797 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/cross_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 03:45:49.281664 meow-sim-0.4.2/meow/eme/
--rw-r--r--   0 root         (0) root         (0)      623 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/eme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5354 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/eme/common.py
--rw-r--r--   0 root         (0) root         (0)     3810 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/eme/sax.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 03:45:49.281664 meow-sim-0.4.2/meow/fde/
--rw-r--r--   0 root         (0) root         (0)      324 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/fde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4621 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/fde/lumerical.py
--rw-r--r--   0 root         (0) root         (0)     2969 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/fde/tidy3d.py
--rw-r--r--   0 root         (0) root         (0)     2318 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/gds_structures.py
--rw-r--r--   0 root         (0) root         (0)    10642 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/geometries.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/integrate.py
--rw-r--r--   0 root         (0) root         (0)    10798 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/materials.py
--rw-r--r--   0 root         (0) root         (0)     3579 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/mesh.py
--rw-r--r--   0 root         (0) root         (0)    12184 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/mode.py
--rw-r--r--   0 root         (0) root         (0)     1876 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/structures.py
--rw-r--r--   0 root         (0) root         (0)     5962 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 03:45:49.281664 meow-sim-0.4.2/meow_sim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3078 2023-06-06 03:45:49.000000 meow-sim-0.4.2/meow_sim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-06-06 03:45:49.000000 meow-sim-0.4.2/meow_sim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 03:45:49.000000 meow-sim-0.4.2/meow_sim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-06 03:45:49.000000 meow-sim-0.4.2/meow_sim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-06 03:45:49.000000 meow-sim-0.4.2/meow_sim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1819 2023-06-06 03:45:44.000000 meow-sim-0.4.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 03:45:49.285664 meow-sim-0.4.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 03:45:49.281664 meow-sim-0.4.2/tests/
--rw-r--r--   0 root         (0) root         (0)     3931 2023-06-06 03:45:44.000000 meow-sim-0.4.2/tests/test_deserialization.py
--rw-r--r--   0 root         (0) root         (0)     3767 2023-06-06 03:45:44.000000 meow-sim-0.4.2/tests/test_mode_operators.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-06-06 03:45:44.000000 meow-sim-0.4.2/tests/test_nbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 21:21:53.194868 meow-sim-0.4.3/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-06-06 21:21:47.000000 meow-sim-0.4.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-06-06 21:21:53.194868 meow-sim-0.4.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-06-06 21:21:47.000000 meow-sim-0.4.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 21:21:53.190868 meow-sim-0.4.3/meow/
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 21:21:53.190868 meow-sim-0.4.3/meow/assets/
+-rw-r--r--   0 root         (0) root         (0)    10307 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/assets/silicon.csv
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/assets/silicon_oxide.csv
+-rw-r--r--   0 root         (0) root         (0)     8019 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4844 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/cell.py
+-rw-r--r--   0 root         (0) root         (0)     2797 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/cross_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 21:21:53.190868 meow-sim-0.4.3/meow/eme/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/eme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5354 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/eme/common.py
+-rw-r--r--   0 root         (0) root         (0)     3810 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/eme/sax.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 21:21:53.194868 meow-sim-0.4.3/meow/fde/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/fde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4621 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/fde/lumerical.py
+-rw-r--r--   0 root         (0) root         (0)     2969 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/fde/tidy3d.py
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/gds_structures.py
+-rw-r--r--   0 root         (0) root         (0)    10642 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/geometries.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/integrate.py
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/materials.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/mesh.py
+-rw-r--r--   0 root         (0) root         (0)    12184 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/mode.py
+-rw-r--r--   0 root         (0) root         (0)     1876 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/structures.py
+-rw-r--r--   0 root         (0) root         (0)     5962 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 21:21:53.194868 meow-sim-0.4.3/meow_sim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-06-06 21:21:53.000000 meow-sim-0.4.3/meow_sim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-06-06 21:21:53.000000 meow-sim-0.4.3/meow_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 21:21:53.000000 meow-sim-0.4.3/meow_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-06 21:21:53.000000 meow-sim-0.4.3/meow_sim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-06 21:21:53.000000 meow-sim-0.4.3/meow_sim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-06-06 21:21:47.000000 meow-sim-0.4.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 21:21:53.194868 meow-sim-0.4.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 21:21:53.194868 meow-sim-0.4.3/tests/
+-rw-r--r--   0 root         (0) root         (0)     3931 2023-06-06 21:21:47.000000 meow-sim-0.4.3/tests/test_deserialization.py
+-rw-r--r--   0 root         (0) root         (0)     3767 2023-06-06 21:21:47.000000 meow-sim-0.4.3/tests/test_mode_operators.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-06-06 21:21:47.000000 meow-sim-0.4.3/tests/test_nbs.py
```

### Comparing `meow-sim-0.4.2/LICENSE` & `meow-sim-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.2/PKG-INFO` & `meow-sim-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.4.2
+Version: 0.4.3
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.4.2/README.md` & `meow-sim-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.2/meow/__init__.py` & `meow-sim-0.4.3/meow/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ MEOW: Modeling of Eigenmodes and Overlaps in Waveguides """
 
 __author__ = "Floris Laporte"
-__version__ = "0.4.2"
+__version__ = "0.4.3"
 
 import warnings
 
 # Silence Excessive Logging...
 
 try:
     from loguru import logger
```

### Comparing `meow-sim-0.4.2/meow/assets/silicon.csv` & `meow-sim-0.4.3/meow/assets/silicon.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.2/meow/assets/silicon_oxide.csv` & `meow-sim-0.4.3/meow/assets/silicon_oxide.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.2/meow/base_model.py` & `meow-sim-0.4.3/meow/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 def _serialize_array(arr):
     if np.iscomplexobj(arr):
         return {
             "real": _serialize_array(np.real(arr)),
             "imag": _serialize_array(np.imag(arr)),
         }
     else:
-        return np.round(arr, 12).tolist()
+        return np.round(arr, 16).tolist()
 
 
 def _parse_array_type_info(annotation) -> Tuple[Any, Any]:
     try:
         type_info = annotation.__args__
     except AttributeError:
         type_info = tuple()
@@ -143,15 +143,15 @@
     When using this _ModelMetaclass, the BaseModel will automatically try to cast the arrays according to the given array type-hint.
 
     Moreover, the following config will be injected (added to the config class that might already be present)::
 
         Config:
             arbitrary_types_allowed = True
             json_encoders = {
-                np.ndarray: lambda arr: np.round(arr, 12).tolist()
+                np.ndarray: lambda arr: np.round(arr, 16).tolist()
             }
 
     """
 
     def __new__(cls, name, bases, dct, **kwargs):
         # Inject sensible default Configuration (Config class)
         extra_config = {
```

### Comparing `meow-sim-0.4.2/meow/cache.py` & `meow-sim-0.4.3/meow/cache.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.2/meow/cell.py` & `meow-sim-0.4.3/meow/cell.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.2/meow/cross_section.py` & `meow-sim-0.4.3/meow/cross_section.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.2/meow/eme/__init__.py` & `meow-sim-0.4.3/meow/eme/__init__.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.2/meow/eme/common.py` & `meow-sim-0.4.3/meow/eme/common.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.2/meow/eme/sax.py` & `meow-sim-0.4.3/meow/eme/sax.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.2/meow/environment.py` & `meow-sim-0.4.3/meow/environment.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.2/meow/fde/lumerical.py` & `meow-sim-0.4.3/meow/fde/lumerical.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.2/meow/fde/tidy3d.py` & `meow-sim-0.4.3/meow/fde/tidy3d.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.2/meow/gds_structures.py` & `meow-sim-0.4.3/meow/gds_structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.2/meow/geometries.py` & `meow-sim-0.4.3/meow/geometries.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.2/meow/integrate.py` & `meow-sim-0.4.3/meow/integrate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.2/meow/materials.py` & `meow-sim-0.4.3/meow/materials.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.2/meow/mesh.py` & `meow-sim-0.4.3/meow/mesh.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.2/meow/mode.py` & `meow-sim-0.4.3/meow/mode.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.2/meow/structures.py` & `meow-sim-0.4.3/meow/structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.2/meow/visualize.py` & `meow-sim-0.4.3/meow/visualize.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.2/meow_sim.egg-info/PKG-INFO` & `meow-sim-0.4.3/meow_sim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.4.2
+Version: 0.4.3
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.4.2/meow_sim.egg-info/SOURCES.txt` & `meow-sim-0.4.3/meow_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.2/pyproject.toml` & `meow-sim-0.4.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["build", "pip", "setuptools", "wheel", "pybind11"]
 
 [project]
 name = "meow-sim"
-version = "0.4.2"
+version = "0.4.3"
 authors = [
 { name = "Rockley Photonics" },
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Modeling of Eigenmodes and Overlaps in Waveguide Structures"
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `meow-sim-0.4.2/tests/test_deserialization.py` & `meow-sim-0.4.3/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.2/tests/test_mode_operators.py` & `meow-sim-0.4.3/tests/test_mode_operators.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.2/tests/test_nbs.py` & `meow-sim-0.4.3/tests/test_nbs.py`

 * *Files identical despite different names*

