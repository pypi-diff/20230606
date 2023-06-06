# Comparing `tmp/PyMoosh-2.62.tar.gz` & `tmp/PyMoosh-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyMoosh-2.62.tar", last modified: Tue Jun  6 08:58:39 2023, max compression
+gzip compressed data, was "dist/PyMoosh-3.0.tar", last modified: Tue Jun  6 11:14:40 2023, max compression
```

## Comparing `PyMoosh-2.62.tar` & `PyMoosh-3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 moi       (1001) moi       (1001)        0 2023-06-06 08:58:39.000000 PyMoosh-2.62/
--rw-rw-r--   0 moi       (1001) moi       (1001)     3350 2023-06-06 08:58:39.000000 PyMoosh-2.62/PKG-INFO
-drwxrwxr-x   0 moi       (1001) moi       (1001)        0 2023-06-06 08:58:39.000000 PyMoosh-2.62/PyMoosh/
-drwxrwxr-x   0 moi       (1001) moi       (1001)        0 2023-06-06 08:58:39.000000 PyMoosh-2.62/PyMoosh/data/
--rw-rw-r--   0 moi       (1001) moi       (1001)    80345 2023-02-15 07:39:17.000000 PyMoosh-2.62/PyMoosh/data/solar.json
--rw-rw-r--   0 moi       (1001) moi       (1001)    11075 2023-02-15 07:39:17.000000 PyMoosh-2.62/PyMoosh/data/material_data.json
--rw-rw-r--   0 moi       (1001) moi       (1001)     1274 2023-06-06 08:58:14.000000 PyMoosh-2.62/PyMoosh/__init__.py
--rw-rw-r--   0 moi       (1001) moi       (1001)   188199 2023-06-06 08:48:44.000000 PyMoosh-2.62/PyMoosh/core.py
--rw-rw-r--   0 moi       (1001) moi       (1001)     4571 2023-06-05 14:15:08.000000 PyMoosh-2.62/PyMoosh/optim_algo.py
--rw-rw-r--   0 moi       (1001) moi       (1001)     4373 2023-04-06 22:06:11.000000 PyMoosh-2.62/PyMoosh/materials.py
--rw-rw-r--   0 moi       (1001) moi       (1001)    34502 2022-09-23 09:03:42.000000 PyMoosh-2.62/LICENSE.txt
-drwxrwxr-x   0 moi       (1001) moi       (1001)        0 2023-06-06 08:58:39.000000 PyMoosh-2.62/PyMoosh.egg-info/
--rw-rw-r--   0 moi       (1001) moi       (1001)     3350 2023-06-06 08:58:39.000000 PyMoosh-2.62/PyMoosh.egg-info/PKG-INFO
--rw-rw-r--   0 moi       (1001) moi       (1001)      425 2023-06-06 08:58:39.000000 PyMoosh-2.62/PyMoosh.egg-info/SOURCES.txt
--rw-rw-r--   0 moi       (1001) moi       (1001)        8 2023-06-06 08:58:39.000000 PyMoosh-2.62/PyMoosh.egg-info/top_level.txt
--rw-rw-r--   0 moi       (1001) moi       (1001)       23 2023-06-06 08:58:39.000000 PyMoosh-2.62/PyMoosh.egg-info/requires.txt
--rw-rw-r--   0 moi       (1001) moi       (1001)        1 2023-06-06 08:58:39.000000 PyMoosh-2.62/PyMoosh.egg-info/dependency_links.txt
--rw-rw-r--   0 moi       (1001) moi       (1001)      319 2023-02-15 08:19:19.000000 PyMoosh-2.62/PyMoosh.egg-info/SOURCES (SFConflict antoine.moreau@uca.fr 2023-05-29-10-11-16).txt
--rw-rw-r--   0 moi       (1001) moi       (1001)     2282 2023-02-15 07:39:17.000000 PyMoosh-2.62/setup.py
--rw-rw-r--   0 moi       (1001) moi       (1001)       34 2023-02-15 07:39:17.000000 PyMoosh-2.62/MANIFEST.in
--rw-rw-r--   0 moi       (1001) moi       (1001)      107 2023-06-06 08:58:39.000000 PyMoosh-2.62/setup.cfg
--rw-rw-r--   0 moi       (1001) moi       (1001)     2565 2023-02-15 07:39:17.000000 PyMoosh-2.62/README.md
+drwxrwxr-x   0 moi       (1001) moi       (1001)        0 2023-06-06 11:14:40.000000 PyMoosh-3.0/
+-rw-rw-r--   0 moi       (1001) moi       (1001)     3349 2023-06-06 11:14:40.000000 PyMoosh-3.0/PKG-INFO
+drwxrwxr-x   0 moi       (1001) moi       (1001)        0 2023-06-06 11:14:40.000000 PyMoosh-3.0/PyMoosh/
+drwxrwxr-x   0 moi       (1001) moi       (1001)        0 2023-06-06 11:14:40.000000 PyMoosh-3.0/PyMoosh/data/
+-rw-rw-r--   0 moi       (1001) moi       (1001)    80345 2023-02-15 07:39:17.000000 PyMoosh-3.0/PyMoosh/data/solar.json
+-rw-rw-r--   0 moi       (1001) moi       (1001)    11075 2023-02-15 07:39:17.000000 PyMoosh-3.0/PyMoosh/data/material_data.json
+-rw-rw-r--   0 moi       (1001) moi       (1001)     1273 2023-06-06 11:14:23.000000 PyMoosh-3.0/PyMoosh/__init__.py
+-rw-rw-r--   0 moi       (1001) moi       (1001)   188241 2023-06-06 10:59:05.000000 PyMoosh-3.0/PyMoosh/core.py
+-rw-rw-r--   0 moi       (1001) moi       (1001)     4571 2023-06-05 14:15:08.000000 PyMoosh-3.0/PyMoosh/optim_algo.py
+-rw-rw-r--   0 moi       (1001) moi       (1001)     4373 2023-04-06 22:06:11.000000 PyMoosh-3.0/PyMoosh/materials.py
+-rw-rw-r--   0 moi       (1001) moi       (1001)    34502 2022-09-23 09:03:42.000000 PyMoosh-3.0/LICENSE.txt
+drwxrwxr-x   0 moi       (1001) moi       (1001)        0 2023-06-06 11:14:40.000000 PyMoosh-3.0/PyMoosh.egg-info/
+-rw-rw-r--   0 moi       (1001) moi       (1001)     3349 2023-06-06 11:14:40.000000 PyMoosh-3.0/PyMoosh.egg-info/PKG-INFO
+-rw-rw-r--   0 moi       (1001) moi       (1001)      425 2023-06-06 11:14:40.000000 PyMoosh-3.0/PyMoosh.egg-info/SOURCES.txt
+-rw-rw-r--   0 moi       (1001) moi       (1001)        8 2023-06-06 11:14:40.000000 PyMoosh-3.0/PyMoosh.egg-info/top_level.txt
+-rw-rw-r--   0 moi       (1001) moi       (1001)       23 2023-06-06 11:14:40.000000 PyMoosh-3.0/PyMoosh.egg-info/requires.txt
+-rw-rw-r--   0 moi       (1001) moi       (1001)        1 2023-06-06 11:14:40.000000 PyMoosh-3.0/PyMoosh.egg-info/dependency_links.txt
+-rw-rw-r--   0 moi       (1001) moi       (1001)      319 2023-02-15 08:19:19.000000 PyMoosh-3.0/PyMoosh.egg-info/SOURCES (SFConflict antoine.moreau@uca.fr 2023-05-29-10-11-16).txt
+-rw-rw-r--   0 moi       (1001) moi       (1001)     2282 2023-02-15 07:39:17.000000 PyMoosh-3.0/setup.py
+-rw-rw-r--   0 moi       (1001) moi       (1001)       34 2023-02-15 07:39:17.000000 PyMoosh-3.0/MANIFEST.in
+-rw-rw-r--   0 moi       (1001) moi       (1001)      107 2023-06-06 11:14:40.000000 PyMoosh-3.0/setup.cfg
+-rw-rw-r--   0 moi       (1001) moi       (1001)     2565 2023-02-15 07:39:17.000000 PyMoosh-3.0/README.md
```

### Comparing `PyMoosh-2.62/PKG-INFO` & `PyMoosh-3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: PyMoosh
-Version: 2.62
+Version: 3.0
 Summary: A scattering matrix formalism to solve Maxwell's equations in a multilayered structure.
 Home-page: https://github.com/AnMoreau/PyMoosh
 Author: Antoine Moreau
 Author-email: antoine.moreau@uca.fr
 License: GPLv3+
 Description: # PyMoosh
```

### Comparing `PyMoosh-2.62/PyMoosh/data/solar.json` & `PyMoosh-3.0/PyMoosh/data/solar.json`

 * *Files identical despite different names*

### Comparing `PyMoosh-2.62/PyMoosh/data/material_data.json` & `PyMoosh-3.0/PyMoosh/data/material_data.json`

 * *Files identical despite different names*

### Comparing `PyMoosh-2.62/PyMoosh/__init__.py` & `PyMoosh-3.0/PyMoosh/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     in a multilayered structure. This makes PyMoosh unconditionally stable,
     allowing to explore even advanced properties of such multilayers,
     find poles and zeros of the scattering matrix (and thus guided modes),
     and many other things...
 
 """
 __name__ = 'PyMoosh'
-__version__ = '2.62'
+__version__ = '3.0'
 __date__ = "06/06/2023"   # MM/DD/YYY
 __author__ = 'Antoine Moreau'
 
 
 ## make accessible everything from `core` directly from the PyMoosh base package
 from PyMoosh.core import *
 from PyMoosh.optim_algo import *
```

### Comparing `PyMoosh-2.62/PyMoosh/core.py` & `PyMoosh-3.0/PyMoosh/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 from PyMoosh.materials import *
 
 def conv_to_nm(length, unit):
     """ Converts a length from "unit"to nm, because everything has been coded
         in nm...
     """
     if (unit == "m"):
-        return length * 1e9
+        return np.array(length) * 1e9
     elif (unit == "um"):
-        return length * 1e3
+        return np.array(length) * 1e3
     elif (unit == "mm"):
-        return length * 1e6
+        return np.array(length) * 1e6
     elif (unit == "pm"):
-        return length * 1e-3
+        return np.array(length) * 1e-3
     elif (unit == "nm"):
     # Just in case we get here but didn't need to
-        return length
+        return np.array(length)
     else:
         print("Please provide lengths in m, mm or um")
 
 
 class Structure:
     """Each instance of Structure describes a multilayer completely.
     This includes the materials the multilayer is made of and the
@@ -187,37 +187,37 @@
             material = self.materials[k]
             epsilon[k] = material.get_permittivity(wavelength)
             mu[k] = material.get_permeability(wavelength)
 
         return epsilon, mu
 
 
-    def plot_stack(struct, wavelength=None, lim_eps_colors=[1.5, 4]):
+    def plot_stack(self, wavelength=None, lim_eps_colors=[1.5, 4]):
         """plot layerstack
 
         evaluate materials at given wavelength for labels
         """
         if wavelength is None:
             wavelength=500.0
         elif(self.unit != "nm"):
             wavelength = conv_to_nm(wavelength, self.unit)
 
         _mats = []
         _mats_names = []
         _index_diff = []
-        for i, mat in enumerate(np.array(struct.materials)[struct.layer_type]):
+        for i, mat in enumerate(np.array(self.materials)[self.layer_type]):
             if hasattr(mat, 'name') and len(mat.name)>0:
                 # Named materials
                 _mats_names.append(mat.name)
                 _index_diff.append(i)
             # Simply using the permittivity at a given wavelength (default is 500 nm)
             _mats.append(mat.get_permittivity(wavelength))
         _index_diff = np.array(_index_diff)
 
-        _thick = struct.thickness
+        _thick = self.thickness
 
         ## give sub- and superstrate a finite thickness
         if _thick[0] == 0: _thick[0] = 50
         if _thick[-1] == 0: _thick[-1] = 50
 
 
         ## define colors for layers of different ref.indices
```

### Comparing `PyMoosh-2.62/PyMoosh/optim_algo.py` & `PyMoosh-3.0/PyMoosh/optim_algo.py`

 * *Files identical despite different names*

### Comparing `PyMoosh-2.62/PyMoosh/materials.py` & `PyMoosh-3.0/PyMoosh/materials.py`

 * *Files identical despite different names*

### Comparing `PyMoosh-2.62/LICENSE.txt` & `PyMoosh-3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyMoosh-2.62/PyMoosh.egg-info/PKG-INFO` & `PyMoosh-3.0/PyMoosh.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: PyMoosh
-Version: 2.62
+Version: 3.0
 Summary: A scattering matrix formalism to solve Maxwell's equations in a multilayered structure.
 Home-page: https://github.com/AnMoreau/PyMoosh
 Author: Antoine Moreau
 Author-email: antoine.moreau@uca.fr
 License: GPLv3+
 Description: # PyMoosh
```

### Comparing `PyMoosh-2.62/setup.py` & `PyMoosh-3.0/setup.py`

 * *Files identical despite different names*

### Comparing `PyMoosh-2.62/README.md` & `PyMoosh-3.0/README.md`

 * *Files identical despite different names*

