# Comparing `tmp/meow-sim-0.4.1.tar.gz` & `tmp/meow-sim-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow-sim-0.4.1.tar", last modified: Mon Jun  5 20:45:35 2023, max compression
+gzip compressed data, was "meow-sim-0.4.2.tar", last modified: Tue Jun  6 03:45:49 2023, max compression
```

## Comparing `meow-sim-0.4.1.tar` & `meow-sim-0.4.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:45:35.636978 meow-sim-0.4.1/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-06-05 20:45:31.000000 meow-sim-0.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3078 2023-06-05 20:45:35.636978 meow-sim-0.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2060 2023-06-05 20:45:31.000000 meow-sim-0.4.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:45:35.636978 meow-sim-0.4.1/meow/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:45:35.636978 meow-sim-0.4.1/meow/assets/
--rw-r--r--   0 root         (0) root         (0)    10307 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/assets/silicon.csv
--rw-r--r--   0 root         (0) root         (0)     8535 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/assets/silicon_oxide.csv
--rw-r--r--   0 root         (0) root         (0)     8019 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/base_model.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/cache.py
--rw-r--r--   0 root         (0) root         (0)     4844 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/cell.py
--rw-r--r--   0 root         (0) root         (0)     2797 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/cross_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:45:35.636978 meow-sim-0.4.1/meow/eme/
--rw-r--r--   0 root         (0) root         (0)      623 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/eme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5354 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/eme/common.py
--rw-r--r--   0 root         (0) root         (0)     3810 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/eme/sax.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:45:35.636978 meow-sim-0.4.1/meow/fde/
--rw-r--r--   0 root         (0) root         (0)      324 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/fde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4621 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/fde/lumerical.py
--rw-r--r--   0 root         (0) root         (0)     2907 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/fde/tidy3d.py
--rw-r--r--   0 root         (0) root         (0)     2318 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/gds_structures.py
--rw-r--r--   0 root         (0) root         (0)    10642 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/geometries.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/integrate.py
--rw-r--r--   0 root         (0) root         (0)    10798 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/materials.py
--rw-r--r--   0 root         (0) root         (0)     3579 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/mesh.py
--rw-r--r--   0 root         (0) root         (0)    12184 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/mode.py
--rw-r--r--   0 root         (0) root         (0)     1876 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/structures.py
--rw-r--r--   0 root         (0) root         (0)     5962 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:45:35.636978 meow-sim-0.4.1/meow_sim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3078 2023-06-05 20:45:35.000000 meow-sim-0.4.1/meow_sim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-06-05 20:45:35.000000 meow-sim-0.4.1/meow_sim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 20:45:35.000000 meow-sim-0.4.1/meow_sim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-05 20:45:35.000000 meow-sim-0.4.1/meow_sim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-05 20:45:35.000000 meow-sim-0.4.1/meow_sim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1819 2023-06-05 20:45:31.000000 meow-sim-0.4.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 20:45:35.636978 meow-sim-0.4.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:45:35.636978 meow-sim-0.4.1/tests/
--rw-r--r--   0 root         (0) root         (0)     3931 2023-06-05 20:45:31.000000 meow-sim-0.4.1/tests/test_deserialization.py
--rw-r--r--   0 root         (0) root         (0)     3767 2023-06-05 20:45:31.000000 meow-sim-0.4.1/tests/test_mode_operators.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-06-05 20:45:31.000000 meow-sim-0.4.1/tests/test_nbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 03:45:49.285664 meow-sim-0.4.2/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-06-06 03:45:44.000000 meow-sim-0.4.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-06-06 03:45:49.281664 meow-sim-0.4.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-06-06 03:45:44.000000 meow-sim-0.4.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 03:45:49.281664 meow-sim-0.4.2/meow/
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 03:45:49.281664 meow-sim-0.4.2/meow/assets/
+-rw-r--r--   0 root         (0) root         (0)    10307 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/assets/silicon.csv
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/assets/silicon_oxide.csv
+-rw-r--r--   0 root         (0) root         (0)     8019 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4844 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/cell.py
+-rw-r--r--   0 root         (0) root         (0)     2797 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/cross_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 03:45:49.281664 meow-sim-0.4.2/meow/eme/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/eme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5354 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/eme/common.py
+-rw-r--r--   0 root         (0) root         (0)     3810 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/eme/sax.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 03:45:49.281664 meow-sim-0.4.2/meow/fde/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/fde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4621 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/fde/lumerical.py
+-rw-r--r--   0 root         (0) root         (0)     2969 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/fde/tidy3d.py
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/gds_structures.py
+-rw-r--r--   0 root         (0) root         (0)    10642 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/geometries.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/integrate.py
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/materials.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/mesh.py
+-rw-r--r--   0 root         (0) root         (0)    12184 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/mode.py
+-rw-r--r--   0 root         (0) root         (0)     1876 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/structures.py
+-rw-r--r--   0 root         (0) root         (0)     5962 2023-06-06 03:45:44.000000 meow-sim-0.4.2/meow/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 03:45:49.281664 meow-sim-0.4.2/meow_sim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-06-06 03:45:49.000000 meow-sim-0.4.2/meow_sim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-06-06 03:45:49.000000 meow-sim-0.4.2/meow_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 03:45:49.000000 meow-sim-0.4.2/meow_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-06 03:45:49.000000 meow-sim-0.4.2/meow_sim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-06 03:45:49.000000 meow-sim-0.4.2/meow_sim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-06-06 03:45:44.000000 meow-sim-0.4.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 03:45:49.285664 meow-sim-0.4.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 03:45:49.281664 meow-sim-0.4.2/tests/
+-rw-r--r--   0 root         (0) root         (0)     3931 2023-06-06 03:45:44.000000 meow-sim-0.4.2/tests/test_deserialization.py
+-rw-r--r--   0 root         (0) root         (0)     3767 2023-06-06 03:45:44.000000 meow-sim-0.4.2/tests/test_mode_operators.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-06-06 03:45:44.000000 meow-sim-0.4.2/tests/test_nbs.py
```

### Comparing `meow-sim-0.4.1/LICENSE` & `meow-sim-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.1/PKG-INFO` & `meow-sim-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.4.1
+Version: 0.4.2
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.4.1/README.md` & `meow-sim-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.1/meow/__init__.py` & `meow-sim-0.4.2/meow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ MEOW: Modeling of Eigenmodes and Overlaps in Waveguides """
 
 __author__ = "Floris Laporte"
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 
 import warnings
 
 # Silence Excessive Logging...
 
 try:
     from loguru import logger
```

### Comparing `meow-sim-0.4.1/meow/assets/silicon.csv` & `meow-sim-0.4.2/meow/assets/silicon.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.1/meow/assets/silicon_oxide.csv` & `meow-sim-0.4.2/meow/assets/silicon_oxide.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.1/meow/base_model.py` & `meow-sim-0.4.2/meow/base_model.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.1/meow/cache.py` & `meow-sim-0.4.2/meow/cache.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.1/meow/cell.py` & `meow-sim-0.4.2/meow/cell.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.1/meow/cross_section.py` & `meow-sim-0.4.2/meow/cross_section.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.1/meow/eme/__init__.py` & `meow-sim-0.4.2/meow/eme/__init__.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.1/meow/eme/common.py` & `meow-sim-0.4.2/meow/eme/common.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.1/meow/eme/sax.py` & `meow-sim-0.4.2/meow/eme/sax.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.1/meow/environment.py` & `meow-sim-0.4.2/meow/environment.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.1/meow/fde/lumerical.py` & `meow-sim-0.4.2/meow/fde/lumerical.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.1/meow/fde/tidy3d.py` & `meow-sim-0.4.2/meow/fde/tidy3d.py`

 * *Files 22% similar despite different names*

```diff
@@ -31,34 +31,40 @@
     """
 
     if num_modes < 1:
         raise ValueError("You need to request at least 1 mode.")
 
     od = np.zeros_like(cs.nx)  # off diagonal entry
     new_tidy3d = version.parse(tidy3d.__version__) >= version.parse("2.2.0")
+    if new_tidy3d:
+        eps_cross = [cs.nx**2, od, od, od, cs.ny**2, od, od, od, cs.nz**2]
+    else:
+        eps_cross = [cs.nx**2, cs.ny**2, cs.nz**2]
+
+    mode_spec = SimpleNamespace(  # tidy3d.ModeSpec alternative (prevents type checking)
+        num_modes=num_modes,
+        target_neff=target_neff,
+        num_pml=cs.cell.mesh.num_pml,
+        filter_pol=None,
+        angle_theta=cs.cell.mesh.angle_theta,
+        angle_phi=cs.cell.mesh.angle_phi,
+        bend_radius=cs.cell.mesh.bend_radius,
+        precision=precision,
+        bend_axis=cs.cell.mesh.bend_axis,
+        track_freq="central",
+        group_index_step=False,
+    )
+
     ((Ex, Ey, Ez), (Hx, Hy, Hz)), neffs = (
         x.squeeze()
         for x in _compute_modes(
-            eps_cross=[cs.nx**2, od, od, od, cs.ny**2, od, od, od, cs.nz**2]
-            if new_tidy3d
-            else [cs.nx**2, cs.ny**2, cs.nz**2],
+            eps_cross=eps_cross,
             coords=[cs.mesh.x, cs.mesh.y],
             freq=c / (cs.env.wl * 1e-6),
-            mode_spec=SimpleNamespace(
-                num_modes=num_modes,
-                angle_theta=cs.cell.mesh.angle_theta,
-                angle_phi=cs.cell.mesh.angle_phi,
-                bend_radius=cs.cell.mesh.bend_radius,
-                bend_axis=cs.cell.mesh.bend_axis,
-                target_neff=target_neff,
-                num_pml=cs.cell.mesh.num_pml,
-                sort_by="largest_neff",
-                filter_pol=None,
-                precision=precision,
-            ),
+            mode_spec=mode_spec,
         )
     )
 
     if num_modes == 1:
         modes = [
             Mode(
                 cs=cs,
```

### Comparing `meow-sim-0.4.1/meow/gds_structures.py` & `meow-sim-0.4.2/meow/gds_structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.1/meow/geometries.py` & `meow-sim-0.4.2/meow/geometries.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.1/meow/integrate.py` & `meow-sim-0.4.2/meow/integrate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.1/meow/materials.py` & `meow-sim-0.4.2/meow/materials.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.1/meow/mesh.py` & `meow-sim-0.4.2/meow/mesh.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.1/meow/mode.py` & `meow-sim-0.4.2/meow/mode.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.1/meow/structures.py` & `meow-sim-0.4.2/meow/structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.1/meow/visualize.py` & `meow-sim-0.4.2/meow/visualize.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.1/meow_sim.egg-info/PKG-INFO` & `meow-sim-0.4.2/meow_sim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.4.1
+Version: 0.4.2
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.4.1/meow_sim.egg-info/SOURCES.txt` & `meow-sim-0.4.2/meow_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.1/pyproject.toml` & `meow-sim-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["build", "pip", "setuptools", "wheel", "pybind11"]
 
 [project]
 name = "meow-sim"
-version = "0.4.1"
+version = "0.4.2"
 authors = [
 { name = "Rockley Photonics" },
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Modeling of Eigenmodes and Overlaps in Waveguide Structures"
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `meow-sim-0.4.1/tests/test_deserialization.py` & `meow-sim-0.4.2/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.1/tests/test_mode_operators.py` & `meow-sim-0.4.2/tests/test_mode_operators.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.1/tests/test_nbs.py` & `meow-sim-0.4.2/tests/test_nbs.py`

 * *Files identical despite different names*

