# Comparing `tmp/PCCanalyser-0.1.1.tar.gz` & `tmp/PCCanalyser-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PCCanalyser-0.1.1.tar", last modified: Sun May 14 21:37:34 2023, max compression
+gzip compressed data, was "PCCanalyser-0.5.0.tar", last modified: Tue Jun  6 20:11:56 2023, max compression
```

## Comparing `PCCanalyser-0.1.1.tar` & `PCCanalyser-0.5.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-05-14 21:37:34.951014 PCCanalyser-0.1.1/
--rw-r--r--   0 v94623eb2   (504) staff       (20)    35149 2022-09-08 11:03:35.000000 PCCanalyser-0.1.1/LICENSE
-drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-05-14 21:37:34.948017 PCCanalyser-0.1.1/PCCanalyser.egg-info/
--rw-r--r--   0 v94623eb2   (504) staff       (20)      130 2023-05-14 21:37:34.000000 PCCanalyser-0.1.1/PCCanalyser.egg-info/PKG-INFO
--rw-r--r--   0 v94623eb2   (504) staff       (20)      463 2023-05-14 21:37:34.000000 PCCanalyser-0.1.1/PCCanalyser.egg-info/SOURCES.txt
--rw-r--r--   0 v94623eb2   (504) staff       (20)        1 2023-05-14 21:37:34.000000 PCCanalyser-0.1.1/PCCanalyser.egg-info/dependency_links.txt
--rw-r--r--   0 v94623eb2   (504) staff       (20)      172 2023-05-14 21:37:34.000000 PCCanalyser-0.1.1/PCCanalyser.egg-info/entry_points.txt
--rw-r--r--   0 v94623eb2   (504) staff       (20)       39 2023-05-14 21:37:34.000000 PCCanalyser-0.1.1/PCCanalyser.egg-info/requires.txt
--rw-r--r--   0 v94623eb2   (504) staff       (20)       13 2023-05-14 21:37:34.000000 PCCanalyser-0.1.1/PCCanalyser.egg-info/top_level.txt
--rw-r--r--   0 v94623eb2   (504) staff       (20)      130 2023-05-14 21:37:34.950805 PCCanalyser-0.1.1/PKG-INFO
--rw-r--r--   0 v94623eb2   (504) staff       (20)    15312 2023-02-27 16:00:34.000000 PCCanalyser-0.1.1/README.md
-drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-05-14 21:37:34.949924 PCCanalyser-0.1.1/matgen/
--rw-r--r--   0 v94623eb2   (504) staff       (20)        0 2022-09-08 11:03:35.000000 PCCanalyser-0.1.1/matgen/__init__.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)    63479 2023-04-26 12:13:35.000000 PCCanalyser-0.1.1/matgen/base.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)     2368 2023-02-27 16:00:34.000000 PCCanalyser-0.1.1/matgen/characterise.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)    22427 2023-05-04 12:15:07.000000 PCCanalyser-0.1.1/matgen/matutils.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)     1567 2023-05-03 12:47:14.000000 PCCanalyser-0.1.1/matgen/ndisangles.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)     3034 2023-05-03 12:47:22.000000 PCCanalyser-0.1.1/matgen/ndisorientquat.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)    12073 2023-05-03 12:39:22.000000 PCCanalyser-0.1.1/matgen/sparsemat.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)     2145 2023-04-26 12:13:35.000000 PCCanalyser-0.1.1/matgen/utils.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)      680 2023-05-14 21:37:24.000000 PCCanalyser-0.1.1/pyproject.toml
--rw-r--r--   0 v94623eb2   (504) staff       (20)       38 2023-05-14 21:37:34.951065 PCCanalyser-0.1.1/setup.cfg
-drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-05-14 21:37:34.950592 PCCanalyser-0.1.1/tests/
--rw-r--r--   0 v94623eb2   (504) staff       (20)        0 2022-09-08 11:03:35.000000 PCCanalyser-0.1.1/tests/__init__.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)      298 2023-02-27 16:00:35.000000 PCCanalyser-0.1.1/tests/test_base.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)      466 2023-05-03 12:11:10.000000 PCCanalyser-0.1.1/tests/test_sparsemat.py
+drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-06-06 20:11:56.765819 PCCanalyser-0.5.0/
+-rw-r--r--   0 v94623eb2   (504) staff       (20)    35149 2022-09-08 11:03:35.000000 PCCanalyser-0.5.0/LICENSE
+drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-06-06 20:11:56.761885 PCCanalyser-0.5.0/PCCanalyser.egg-info/
+-rw-r--r--   0 v94623eb2   (504) staff       (20)    16261 2023-06-06 20:11:56.000000 PCCanalyser-0.5.0/PCCanalyser.egg-info/PKG-INFO
+-rw-r--r--   0 v94623eb2   (504) staff       (20)      482 2023-06-06 20:11:56.000000 PCCanalyser-0.5.0/PCCanalyser.egg-info/SOURCES.txt
+-rw-r--r--   0 v94623eb2   (504) staff       (20)        1 2023-06-06 20:11:56.000000 PCCanalyser-0.5.0/PCCanalyser.egg-info/dependency_links.txt
+-rw-r--r--   0 v94623eb2   (504) staff       (20)      172 2023-06-06 20:11:56.000000 PCCanalyser-0.5.0/PCCanalyser.egg-info/entry_points.txt
+-rw-r--r--   0 v94623eb2   (504) staff       (20)       76 2023-06-06 20:11:56.000000 PCCanalyser-0.5.0/PCCanalyser.egg-info/requires.txt
+-rw-r--r--   0 v94623eb2   (504) staff       (20)       13 2023-06-06 20:11:56.000000 PCCanalyser-0.5.0/PCCanalyser.egg-info/top_level.txt
+-rw-r--r--   0 v94623eb2   (504) staff       (20)    16261 2023-06-06 20:11:56.765569 PCCanalyser-0.5.0/PKG-INFO
+-rw-r--r--   0 v94623eb2   (504) staff       (20)    16117 2023-06-06 19:55:50.000000 PCCanalyser-0.5.0/README.md
+drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-06-06 20:11:56.764626 PCCanalyser-0.5.0/matgen/
+-rw-r--r--   0 v94623eb2   (504) staff       (20)        0 2022-09-08 11:03:35.000000 PCCanalyser-0.5.0/matgen/__init__.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)    65850 2023-06-06 19:55:50.000000 PCCanalyser-0.5.0/matgen/base.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)     1648 2023-06-06 19:55:50.000000 PCCanalyser-0.5.0/matgen/characterise.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)     5922 2023-06-06 19:55:50.000000 PCCanalyser-0.5.0/matgen/entropic.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)    19059 2023-06-06 19:55:50.000000 PCCanalyser-0.5.0/matgen/matutils.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)     1567 2023-06-06 19:55:50.000000 PCCanalyser-0.5.0/matgen/ndisangles.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)     3034 2023-06-06 19:55:50.000000 PCCanalyser-0.5.0/matgen/ndisorientquat.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)    12153 2023-06-06 19:55:50.000000 PCCanalyser-0.5.0/matgen/sparsemat.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)     2145 2023-06-06 19:55:50.000000 PCCanalyser-0.5.0/matgen/utils.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)      901 2023-06-06 20:11:05.000000 PCCanalyser-0.5.0/pyproject.toml
+-rw-r--r--   0 v94623eb2   (504) staff       (20)       38 2023-06-06 20:11:56.765872 PCCanalyser-0.5.0/setup.cfg
+drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-06-06 20:11:56.765314 PCCanalyser-0.5.0/tests/
+-rw-r--r--   0 v94623eb2   (504) staff       (20)        0 2022-09-08 11:03:35.000000 PCCanalyser-0.5.0/tests/__init__.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)      298 2023-02-27 16:00:35.000000 PCCanalyser-0.5.0/tests/test_base.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)      466 2023-06-06 19:55:50.000000 PCCanalyser-0.5.0/tests/test_sparsemat.py
```

### Comparing `PCCanalyser-0.1.1/LICENSE` & `PCCanalyser-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PCCanalyser-0.1.1/README.md` & `PCCanalyser-0.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,40 @@
-# Discrete Cell Complex (DCC) Generator tool
+# Polyhedral Cell Complex (PCC) Analyser
+
+## Quick start
+
+Installation:
+
+```
+pip install PCCanalyser
+```
+
+Using of classes:
+```
+from matgen.base import CellComplex
+from matgen.entropic import TripleJunctionSet
+```
+
+Command-line interface (CLI) tools:
+
+```
+# generate sparse matrices
+sparsemat --file complex.tess --dir path/to/target/directory
+
+# find disorientation angles between neighbouring grains of orders less than N
+ndisanples --file complex.tess --dir path/to/target/directory --max-order N
+
+# find disorientation angles between neighbouring grains of orders less than N in quaternions
+ndisorientquat --file complex.tess --dir path/to/target/directory --max-order N
+
+# characteristics of a cell complex
+characterise --dir path/to/files
+```
+
+For details see: [tutorial/Examples.ipynb](tutorial/Examples.ipynb)
 
 <p> The code addressed the practical needs of creating discrete (combinatorial) cell complexes (DCCs) 
 based on the both regular (cubic or octahedron) and Laguerre-Voronoi tessellations of space provided by the <a href="https://neper.info" target=”_blank”> Neper </a> software. In particular, Voronoi tessellations with the corresponding DCCs provide a very close representation of the real material microstructures and are widely used in molecular dynamics and other types of simulations. Such complexes arise from the tessellations of spatial domains around arbitrary sets of points, which ensure that each 1-cell is in the boundary of exactly three 2-cells and three 3-cells, and each 0-cell is in the boundary of exactly four 1-cells, six 2-cells and four 3-cells. </p>
 
 ## 1. DCC definition and algebraic representation
 An excellent simple introduction to the area of DCCs with their various applications is given in the <a href="https://link.springer.com/book/10.1007/978-1-84996-290-2" target="_blank"> book </a> of Leo Grady and Jonathan Polimeni _“Discrete Calculus. Applied Analysis on Graphs for Computational Science. (2010)_ Below are just a few notes necessary for understanding the output of the code.
```

#### html2text {}

```diff
@@ -1,8 +1,18 @@
-# Discrete Cell Complex (DCC) Generator tool
+# Polyhedral Cell Complex (PCC) Analyser ## Quick start Installation: ``` pip
+install PCCanalyser ``` Using of classes: ``` from matgen.base import
+CellComplex from matgen.entropic import TripleJunctionSet ``` Command-line
+interface (CLI) tools: ``` # generate sparse matrices sparsemat --file
+complex.tess --dir path/to/target/directory # find disorientation angles
+between neighbouring grains of orders less than N ndisanples --file
+complex.tess --dir path/to/target/directory --max-order N # find disorientation
+angles between neighbouring grains of orders less than N in quaternions
+ndisorientquat --file complex.tess --dir path/to/target/directory --max-order N
+# characteristics of a cell complex characterise --dir path/to/files ``` For
+details see: [tutorial/Examples.ipynb](tutorial/Examples.ipynb)
 The code addressed the practical needs of creating discrete (combinatorial)
 cell complexes (DCCs) based on the both regular (cubic or octahedron) and
 Laguerre-Voronoi tessellations of space provided by the Neper software. In
 particular, Voronoi tessellations with the corresponding DCCs provide a very
 close representation of the real material microstructures and are widely used
 in molecular dynamics and other types of simulations. Such complexes arise from
 the tessellations of spatial domains around arbitrary sets of points, which
```

### Comparing `PCCanalyser-0.1.1/matgen/base.py` & `PCCanalyser-0.5.0/matgen/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,30 @@
-"""Base classes for complex analysis.
+"""Base classes.
 
 """
-from __future__ import annotations # to avoid NameError in type hinting
+from __future__ import annotations
 import io
 import time
 from typing import Dict, Iterable, List, Tuple
 import logging
+logging.basicConfig(
+    format='%(asctime)s %(message)s',
+    datefmt='%H:%M:%S', level=logging.INFO
+)
 from tqdm import tqdm
 import numpy as np
 import random
 import math
-# import pandas as pd
 
 import matplotlib.pyplot as plt
 from matplotlib.axes import Axes
 from mpl_toolkits.mplot3d.art3d import Poly3DCollection
 
 from matgen import matutils
+from matgen.entropic import TripleJunctionSet
 
 
 class Cell:
     """
     Cell class.
 
     Parameters
@@ -47,15 +51,14 @@
     set_external(is_external=True)
     set_measure(measure)
     """
 
     def __init__(self, id: int):
         self.id = id
         self.n_ids = [] # neighbour ids
-        # self.nn_ids = [] # neighbour of neighbor ids
         self.is_external = False
 
     def __str__(self):
         cell_str = self.__class__.__name__ + "(id=%d)" % self.id
         return cell_str
     
     def __repr__(self) -> str:
@@ -91,22 +94,14 @@
         own identifier.
         """
         self.n_ids += n_ids
         s = set(self.n_ids) # eliminate duplicates
         s.difference_update([self.id]) # eliminate self.id
         self.n_ids = list(s)
 
-    # def add_neighbors_neighbors(self, nn_ids: Iterable):
-    #     """
-    #     """
-    #     self.nn_ids += nn_ids
-    #     s = set(self.nn_ids) # eliminate duplicates
-    #     s.difference_update([self.id] + self.n_ids) # eliminate id and n_ids
-    #     self.nn_ids = list(s)
-
     def set_external(self, is_external: bool = True) -> None:
         """Make the cell external (is_external=True) or internal
         (is_external=False).
 
         Parameters
         ----------
         is_external
@@ -250,75 +245,84 @@
     
     def add_incident_cell(self, signed_incident_id: int):
         """Add a signed incident cell identifier to signed incident cells
         list.
         """
         if abs(signed_incident_id) not in self.incident_ids:
             self.signed_incident_ids.append(signed_incident_id)
-    
-    # def add_incident_cells(self, incident_ids: Iterable):
-    #     """
-    #     FIXME: incident_ids may be signed?
-    #     """
-    #     self.incident_ids += incident_ids
-    #     self.incident_ids = list(set(self.incident_ids))
 
     @property
     def degree(self) -> int:
         """Number of incident cells of the given cell.
         """
         return len(self.signed_incident_ids)
 
 
-class TripleJunction(LowerOrderCell):
-    """
+class GrainBoundary(LowerOrderCell):
     """
-    def __init__(self, id: int):
-        super().__init__(id)
-        self.junction_type = None
+    Grain Boundary (GB). 
+    2D: 1-cells (edges) are considered to be grain biundaries.
+    3D: 2-cells (faces) are considered to be grain boundaries.
 
-    def set_junction_type(self, junction_type: int):
-        """
-        junction_type equals number of special incident cells
-        check consistency: external has type None
-        """
-        if not self.is_external:
-            self.junction_type = junction_type
-        elif self.is_external:
-            raise ValueError(
-                'External junction cannot have a type other than None'
-            )
+    Parameters
+    ----------
+    id : int
+        Identifier of the grain boundary.
+    
+    Attributes
+    ----------
+    id : int
+        Identifier of the grain boundary.
+    is_special: bool
+        Is the grain boundary special?
+    theta: float
+        Disorientation angle between incident grains (in degrees).
+        Theta = -1 for external grain boundaries.
+    gb_index: int
+        Grain boundary index.
 
+    Methods
+    -------
+    set_special(is_special)
+    set_theta(theta, lower_thrd, upper_thrd)
+    set_external(is_external)
+    set_gb_index(gb_index)
+    get_new_seed_prob(critical_size)
 
-class GrainBoundary(LowerOrderCell):
-    """
+    References
+    ---------
+    Discrete model for discontinuous dynamic recrystallisation in its
+    application to post-dynamic recrystallisation in adiabatic shear
+    bands
     """
     def __init__(self, id: int):
         super().__init__(id)
         self.is_special = False
         self.theta = None
         self.gb_index = None
 
     def set_special(self, is_special: bool = True):
         """
-        External cannot be set special
+        Some grain boundaries can be set special.
+        External cells cannot be set special.
         """
         if is_special and not self.is_external:
             self.is_special = is_special
         elif not is_special:
             self.is_special = is_special
         elif self.is_external:
             raise ValueError('External cannot be set special')
     
     def _reset_theta_thrds(
         self,
         lower_thrd: float = None,
         upper_thrd: float = None
     ):
         """
+        Reset is_special with respect to new thresholds for theta.
         """
         if not self.is_external and self.theta:
             if lower_thrd and upper_thrd:
                 if  self.theta >= lower_thrd and self.theta <= upper_thrd:
                     self.set_special(True)
                 else:
                     self.set_special(False)
@@ -341,29 +345,28 @@
         lower_thrd: float = None,
         upper_thrd: float = None
     ):
         """
         disorientation angle (in degrees)
         theta must be >= 0 ?
         for external cells theta = -1
-        TODO: check if theta is changed
         """
         if theta < 0:
             self.set_external(True)
             return
         elif self.is_external:
             raise ValueError(
                 f"External (id={self.id}) doesn't have theta other than -1")
         
         self.theta = theta
         self._reset_theta_thrds(lower_thrd, upper_thrd)
 
     def set_external(self, is_external: bool = True):
         """
-        When set external, it is set not special with theta = -1
+        When set external, it is set non-special and theta = -1
         """
         self.is_external = is_external
         if is_external:
             self.theta = -1
             self.set_special(False)
         elif self.theta == -1:
             self.theta = None
@@ -378,30 +381,84 @@
         elif self.is_external:
             raise ValueError(
                 'External GB cannot have a GB index other than None'
             )
 
     def get_new_seed_prob(self, critical_size=0):
         """
-        without coefficient etha0
+        The probability for nucleation of a new grain on the GB.
+        Without the coefficient of initial probability etha0.
         """
-
-        if self.eq_diam > critical_size:
-            coeff = (1 - (critical_size / self.eq_diam)**3)
-        else:
-            coeff = 0
+        try:
+            if self.eq_diam > critical_size:
+                coeff = (1 - (critical_size / self.eq_diam)**3)
+            else:
+                coeff = 0
+        except:
+            coeff = 1
 
         if self.is_external:
             return 0
         else:
             return (2 * self.gb_index) / (3 * len(self.n_ids) * coeff)
+        
+
+class TripleJunction(LowerOrderCell):
+    """
+    Triple junction (TJ). 
+    2D: 0-cells (vertices) are considered to be triple junctions.
+    3D: 1-cells (edges) are considered to be triple junctions.
+
+    Parameters
+    ----------
+    id : int
+        Identifier of the triple junction.
+    
+    Attributes
+    ----------
+    id : int
+        Identifier of the triple junction.
+    junction type: int
+        Junction_type equals the number of special incident grain boundaries.
+
+    Methods
+    -------
+    set_junction_type(junction_type)
+    
+    Notes
+    -----
+    Any binary classification of grain boundaries induces four distinct
+    TJs types: J0, J1, J2 and J3, where Jk is the index enumerating the number
+    of special GBs joint at a specific triple line. The corresponding TJ fractions of
+    different types j0, j1, j2 and j3 are the probabilities that a randomly chosen
+    TJ will possess with the corresponding type.
+
+    References
+    ---------
+    """
+    def __init__(self, id: int):
+        super().__init__(id)
+        self.junction_type = None
+
+    def set_junction_type(self, junction_type: int):
+        """
+        Junction type equals number of special incident cells.
+        External has type None.
+        """
+        if not self.is_external:
+            self.junction_type = junction_type
+        elif self.is_external:
+            raise ValueError(
+                'External junction cannot have a type other than None'
+            )
 
     
 def _create_ax(dim: int = 2, figsize: Tuple = (8,8)) -> Axes:
     """
+    Create axis.
     """
     if dim == 2:
         projection = None
         # xlim = ylim = (-0.1, 1.1)
     elif dim == 3:
         projection = '3d'
         # xlim = ylim = zlim = (0, 1)
@@ -502,14 +559,43 @@
         """A tuple of x-, y-, z-coordinates.
         """
         return (self.x, self.y, self.z)
 
 
 class Vertex2D(Vertex, TripleJunction):
     """
+    Vertex (0-cell) of a 2D cell complex.
+
+    Parameters
+    ----------
+    id : int
+        Identifier of the vertex.
+    x: float
+        Vertex x-coordinate.
+    y: float
+        Vertex y-coordinate.
+    z: float, optional
+        Vertex z-coordinate. Default is 0.
+    
+    Attributes
+    ----------
+    id : int
+        Identifier of the vertex.
+    x: float
+        Vertex x-coordinate.
+    y: float
+        Vertex y-coordinate.
+    z: float, optional
+        Vertex z-coordinate.
+    coord: Tuple[float]
+        A tuple of x-, y-, z-coordinates.
+
+    Methods
+    -------
+    plot(ax, figsize, **kwargs)
     """
     def __init__(self, id: int, x: float, y: float, z: float = 0):
         super().__init__(id, x, y, z)
         self.junction_type = None
 
     def __str__(self) -> str:
         v_str = self.__class__.__name__ + "(id=%d, x=%.3f, y=%.3f)" % (
@@ -534,14 +620,19 @@
             ax = _create_ax(dim=2, figsize=figsize)
         ax.scatter(self.x, self.y, **kwargs)
         return ax
 
 
 class Vertex3D(Vertex):
     """
+    Vertex (0-cell) of a 3D cell complex.
+
+    Methods
+    -------
+    plot(ax, figsize, **kwargs)
     """
     def plot(
             self,
             ax: Axes = None,
             figsize: Tuple = (8,8),
             **kwargs) -> Axes:
         """
@@ -570,15 +661,15 @@
     v_ids : list
         A list of two vertex identifiers of the edge.
     length : float, optional
         Length of the edge.
 
     Methods
     -------
-    from_tess_file(file)
+    from_tess_file(file, _vertices)
     """
     def __init__(self, id: int, v_ids: list):
         super().__init__(id)
         self.v_ids = v_ids
 
     @classmethod
     def from_tess_file(
@@ -636,14 +727,31 @@
             return self.measure
         except AttributeError:
             return None 
 
 
 class Edge2D(Edge, GrainBoundary):
     """
+    Edge (1-cell) of a 2D cell complex is a grain boundary.
+
+    Parameters
+    ----------
+    id : int
+        Identifier of the edge.
+    v_ids: list
+        A list of two vertex identifiers of the edge.
+    
+    Additional Attributes
+    ----------
+    tj_ids : list
+        Alias for the list of two vertex identifiers of the edge.
+    eq_diam: float
+        Alias for the edge's length.
+
+
     """
     def __init__(self, id: int, v_ids: list):
         super().__init__(id, v_ids)
         self.is_special = False
 
     @property
     def tj_ids(self):
@@ -652,14 +760,15 @@
     @property
     def eq_diam(self):
         return self.length
 
 
 class Edge3D(Edge, TripleJunction):
     """
+    Edge (1-cell) of a 3D cell complex is a triple junction.
     """
     def __init__(self, id: int, v_ids: list):
         super().__init__(id, v_ids)
         self.junction_type = None
 
 
 class Face(Cell):
@@ -678,32 +787,38 @@
     id : int
         Identifier of the face.
     v_ids: list
         A list of vertex identifiers of the face.
     e_ids : list
         A list of edge identifiers of the face.
     d : float
-
+        Parameter of the equation of the face (see Notes).
     a : float
-
+        Parameter of the equation of the face (see Notes).
     b : float
-
+        Parameter of the equation of the face (see Notes).
     c : float
-
+        Parameter of the equation of the face (see Notes).
     normal : Tuple[float]
-
+        Normal vector of the face (a, b, c).
     area : float, optional
         Area of the face.
 
     Methods
     -------
-    from_tess_file(file)
+    from_tess_file(file, _edges)
     add_edge(e_id)
     add_edges(e_ids)
     add_equation(d, a, b, c)
+
+    Notes
+    -----
+    Parameters d, a, b, c are the parameters of the equation of a face
+    :math:`ax + by + cz = d` with :math:`a^2 + b^2 + c^2 = 1`. See details
+    https://neper.info/doc/fileformat.html
     """
     def __init__(self, id: int, v_ids: list):
         super().__init__(id)
         self.v_ids = v_ids
         self.e_ids = []
 
     @classmethod
@@ -807,14 +922,15 @@
             return self.measure
         except AttributeError:
             return None 
 
 
 class Face2D(Face, Grain):
     """
+    Face (2-cell) of a 2D cell complex is a grain.
     """
     def __init__(self, id: int, v_ids: list):
         super().__init__(id, v_ids)
         self.seed = None
         self.ori = None
         self.oridesc = None
 
@@ -889,14 +1005,15 @@
                     face.set_seed(seeds[f_id])
                     _faces[f_id] = face
                 return _faces
 
 
 class Face3D(Face, GrainBoundary):
     """
+    Face (2-cell) of a 3D cell complex is a grain boundary.
     """
     def __init__(self, id: int, v_ids: list):
         super().__init__(id, v_ids)
         self.is_special = False
 
     @property
     def tj_ids(self):
@@ -930,15 +1047,15 @@
     f_ids : list
         A list of face identifiers of the polyhedron.
     vol : float, optional
         Volume of the polyhedron.
 
     Methods
     -------
-    from_tess_file(file)
+    from_tess_file(file, _faces)
     add_vertex(v_id)
     add_vertices(v_ids):
     add_edge(e_id)
     add_edges(e_ids)
     """
     def __init__(self, id: int, f_ids: list):
         super().__init__(id)
@@ -1026,207 +1143,41 @@
         """
         self.e_ids += e_ids
         self.e_ids = list(set(self.e_ids))
 
     @property
     def vol(self) -> float:
         """
+        Polyhedron volume.
         """
         try:
             return self.measure
         except AttributeError:
             return None
     
     @property
     def gb_ids(self):
         return self.f_ids
 
 
-class TripleJunctionSet:
-    """
-    """
-
-    def __init__(self, p, j_tuple) -> None:
-        """
-        """
-        self.p = p
-        self.j0, self.j1, self.j2, self.j3 = j_tuple
-
-    @property
-    def q(self):
-        """
-        """
-        return 1 - self.p
-
-    @property
-    def j_tuple(self):
-        """
-        """
-        return (self.j0, self.j1, self.j2, self.j3)
-
-    @property
-    def Sp(self):
-        """
-        """
-        if self.p == 0 or self.p == 1:
-            return 0
-        else:
-            return matutils.entropy(self.p)
-
-    @property
-    def Sp_m(self):
-        """
-        """
-        if self.p == 0:
-            return np.inf
-        else:
-            return matutils.entropy_m(self.p)
-
-    @property
-    def Sp_s(self):
-        """
-        """
-        if self.p == 0:
-            return - np.inf
-        else:
-            return matutils.entropy_s(self.p)
-
-    @property
-    def p_expected(self):
-        """
-        """
-        return (self.j1 + 2*self.j2 + 3*self.j3) / 3
-        
-    @property
-    def delta_p(self):
-        """
-        """
-        return abs(self.p_expected - self.p)
-
-    @property
-    def S(self):
-        """
-        """
-        return matutils.entropy(*self.j_tuple)
-
-    @property
-    def S_m(self):
-        """
-        """
-        if np.any(np.array(self.j_tuple) == 0):
-            return np.inf
-        else:
-            return matutils.entropy_m(*self.j_tuple)
-
-    @property
-    def S_s(self):
-        """
-        """
-        if np.any(np.array(self.j_tuple) == 0):
-            return - np.inf
-        else:
-            return matutils.entropy_s(*self.j_tuple)
-
-    @property
-    def kappa(self):
-        """
-        """
-        if self.S_s == 0:
-            return 0
-        else:
-            return self.S_m / self.S_s
-
-    @property
-    def delta_S(self):
-        """
-        """
-        return self.Sp - self.S
-
-    @property
-    def d_tuple(self):
-        """
-        """
-        return matutils.get_d_tuple(self.j_tuple)
-
-    @property
-    def d1(self):
-        """
-        """
-        return self.d_tuple[0]
-
-    @property
-    def d2(self):
-        """
-        """
-        return self.d_tuple[1]
-
-    @property
-    def d3(self):
-        """
-        """
-        return self.d_tuple[2]
-
-    def get_property(self, attr):
-        """
-        """
-        return getattr(self, attr)
-    
-    def get_properties(self, attr_list: list = []) -> Dict:
-        """
-        """
-        if not attr_list:
-            attr_list = [
-                'p',
-                'q',
-                'Sp',
-                'Sp_m',
-                'Sp_s',
-                'S',
-                'S_m',
-                'S_s',
-                'kappa',
-                'delta_S',
-                'd1',
-                'd2',
-                'd3'
-            ]
-
-        try:
-            return {attr_name: getattr(self, attr_name) for attr_name in attr_list}
-        except:
-            logging.exception('Check properties!')
-
-        # values = [getattr(self, attr_name) for attr_name in attr_list]
-        # return pd.DataFrame([values], columns = attr_list)
-
-
 def _add_neighbors(_cells: Dict, _incident_cells: Dict):
     """
     Add neighbors to incident_cells from common cells
     _vertices, _edges
     _edges, _faces
     _faces, _polyhedra
     """ 
     for cell in _cells.values():
         for inc_cell_id in cell.incident_ids:
             _incident_cells[inc_cell_id].add_neighbors(cell.incident_ids)
 
 
-# def _add_neighbors_neighbors(_cells: Dict):
-#     """
-#     """
-#     for cell in _cells.values():
-#         nn_ids = []
-#         for n_id in cell.n_ids:
-#             nn_ids += _cells[n_id].n_ids
-#         cell.add_neighbors_neighbors(nn_ids)
-
-
 def _add_measures(_cells: Dict, measures: list):
     """
+    Add measures to the dict of cells from the list of measures.
     """
     n = len(_cells.keys())
     if n != len(measures):
         raise ValueError(
             'Number of cells must be equal to number of measures'
         )
     
@@ -1237,14 +1188,17 @@
 def _add_thetas(
     _cells: Dict,
     thetas: Iterable,
     lower_thrd: float = None,
     upper_thrd: float = None
 ):
     """
+    Add thetas to the dict of cells from the list of thetas.
+    Parameters `lower_thrd` and `upper_thrd` can be used to
+    set special GBs from theta values.
     """
     n = len(_cells.keys())
     if n != len(thetas):
         raise ValueError(
             'Number of cells must be equal to number of theta'
         )
     
@@ -1280,41 +1234,96 @@
     _vertices: Dict
     _edges: Dict
     _faces: Dict
     _polyhedra: Dict, optional
     
     Attributes
     ----------
-    dim: int
-    _vertices: Dict
-    _edges: Dict
-    _faces: Dict
-    _polyhedra: Dict, optional
+    dim : int
+        Cell complex dimension (2 or 3).
+    _vertices : dict
+    vertices : list
+    _edges : dict
+    edges : list
+    _faces : dict
+    faces : list
+    _polyhedra : dict
+    polyhedra : list
     crysym : str
-    load_time: float
-
-
+    load_time : float
+    vernb : int
+        Number of vertices.
+    edgenb : int
+        Number of edges.
+    facenb : int
+        Number of faces.
+    polynb : int
+        Number of polyhedra.
+    grainnb : int
+        Number of grains.
+    _GBs : dict
+        Grain boundaries. Keys are grain ids, values are the cells of
+        the corresponding class (edges for 2D, faces for 3D).
+    _TJs : dict
+        Triple junctions. Keys are grain ids, values are the cells of
+        the corresponding class (vertices for 2D, edges for 3D).
+    _grains : dict
+        Grains. Keys are grain ids, values are the cells of
+        the corresponding class (faces for 2D, polyhedra for 3D).
+    _three_sided_grains : dict
+        Grains with 3 sides in 2D cell complex.
+    p : float
+        Special GB fraction.
+    j_tuple : tuple
+        TJ fractions (j0, j1, j2, j3).
+    n_max_order : int
+    
     Methods
     -------
-    from_tess_file(file)
-    add_vertex(v_id)
-    add_vertices(v_ids):
-    add_edge(e_id)
-    add_edges(e_ids)
+    from_tess_file(file, with_cell_size, with_measures, 
+                    with_theta, theta_file, lower_thrd, upper_thrd)
+    get_one(cell_type, cell_id)
+    get_many(cell_type, cell_ids)
+    get_external_ids(cell_type)
+    get_internal_ids(cell_type)
+    get_special_ids()
+    get_nonspecial_internal_ids()
+    plot_vertices(v_ids, ax, figsize, labels, **kwargs)
+    plot_edges(e_ids, ax, figsize, labels, **kwargs)
+    plot_faces(f_ids, ax, figsize, labels, **kwargs)
+    plot_polyhedra(p_ids, ax, figsize, **kwargs)
+    plot_seeds(cell_ids, ax, figsize, **kwargs)
+    get_junction_ids_of_type(junction_type)
+    get_spec_fraction()
+    get_ext_fraction(cell_type)
+    get_j_fraction(junction_type)
+    get_three_sided_distribution()
+    set_measures_from_coo()
+    set_junction_types()
+    set_gb_indexes()
+    set_three_sided_types()
+    reset_special(lower_thrd, upper_thrd, special_ids, warn_external)
+    to_TJset()
+    describe(attr_list)
+    set_theta_from_ori(lower_thrd, upper_thrd)
+    set_thetas(thetas, lower_thrd, upper_thrd)
+    set_theta_from_file(file, lower_thrd, upper_thrd)
+    find_neighbors_of_order(max_order)
+    get_neighbor_dis_angles(order)
+    get_neighbor_counts_of_order(order)
+    get_new_random_seeds(k, critical_size, spec_prob, exclusion_list, replace)
     """
     def __init__(
         self,
         dim: int,
         _vertices: Dict,
         _edges: Dict,
         _faces: Dict,
         _polyhedra: Dict = None
     ):
-        """
-        """
         self.dim = dim
         self._vertices = _vertices
         self._edges = _edges
         self._faces = _faces
         if _polyhedra:
             self._polyhedra = _polyhedra
 
@@ -1358,29 +1367,25 @@
 
         if dim == 2:
             _edges = Edge2D.from_tess_file(file, _vertices)
         elif dim == 3:
             _edges = Edge3D.from_tess_file(file, _vertices)
                     
         _add_neighbors(_vertices, _edges)
-        # _add_neighbors_neighbors(_vertices)
-        # _add_neighbors_neighbors(_edges)
 
         if dim == 2:
             _faces = Face2D.from_tess_file(file, _edges)
         elif dim == 3:
             _faces = Face3D.from_tess_file(file, _edges)
         
         _add_neighbors(_edges, _faces)
-        # _add_neighbors_neighbors(_faces)
 
         if dim == 3:
             _polyhedra = Poly.from_tess_file(file, _faces)
             _add_neighbors(_faces, _polyhedra)
-            # _add_neighbors_neighbors(_polyhedra)
         
         # Set external
         if dim == 2:
             for e in _edges.values():
                 if e.degree == 1:
                     e.set_external(True)
                     for v_id in e.v_ids:
@@ -1481,27 +1486,23 @@
                 cellcomplex.set_three_sided_types()
 
         cellcomplex.load_time = round(time.time() - start, 1)
         # print('Complex loaded:', cellcomplex.load_time, 's')
         return cellcomplex
 
     def __str__(self):
-        """
-        """
         cc_str = f"<class {self.__class__.__name__}> {self.dim}D" +\
         f"\n{self.vernb} vertices" + f"\n{self.edgenb} edges" +\
         f"\n{self.facenb} faces" 
         
         if self.dim == 3:
             cc_str += f"\n{self.polynb} polyhedra"
         return cc_str
 
-    def __repr__(self) -> str:
-        """
-        """
+    def __repr__(self):
         return self.__str__()
 
     @property
     def vertices(self):
         """
         """
         return [v for v in self._vertices.values()]
@@ -1518,48 +1519,57 @@
         """
         return [f for f in self._faces.values()]
 
     @property
     def polyhedra(self):
         """
         """
-        return [p for p in self._polyhedra.values()]
+        if self.dim == 3:
+            return [p for p in self._polyhedra.values()]
 
     @property
     def vernb(self):
         """
+        Number of vertices.
         """
         return len(self._vertices)
 
     @property
     def edgenb(self):
         """
+        Number of edges.
         """
         return len(self._edges)
 
     @property
     def facenb(self):
         """
+        Number of faces.
         """
         return len(self._faces)
 
     @property
     def polynb(self):
         """
+        Number of polyhedra.
         """
-        return len(self._polyhedra)
+        if self.dim == 3:
+            return len(self._polyhedra)
 
     @property
     def grainnb(self):
         """
+        Number of grains.
         """
         return len(self._grains)
 
     def _choose_cell_type(self, cell_type: str | int):
         """
+        Returns a dict with cells corresponding to the cell type.
+        cell_type may be of str or int data type.
         """
         if cell_type in ['v', 'vertex', 0, '0']:
             _cells = self._vertices
         elif cell_type in ['e', 'edge', 1, '1']:
             _cells = self._edges
         elif cell_type in ['f', 'face', 2, '2']:
             _cells = self._faces
@@ -1568,54 +1578,59 @@
         else:
             raise TypeError('Unknown cell type')
         return _cells
 
     @property
     def _GBs(self):
         """
+        Grain boundaries.
         """
         if self.dim == 2:
             _cells = self._choose_cell_type('edge')
         elif self.dim == 3:
             _cells = self._choose_cell_type('face')
         return _cells
 
     @property
     def _TJs(self):
         """
+        Triple junctions.
         """
         if self.dim == 2:
             _cells = self._choose_cell_type('vertex')
         elif self.dim == 3:
             _cells = self._choose_cell_type('edge')
         return _cells
 
     @property
     def _grains(self):
         """
+        Grains.
         """
         if self.dim == 2:
             _cells = self._choose_cell_type('face')
         elif self.dim == 3:
             _cells = self._choose_cell_type('poly')
         return _cells
 
     @property
     def _three_sided_grains(self):
         """
+        Grains with 3 sides in 2D cell complex.
         """
         if self.dim == 2:
             three_sided = {}
             for f_id, face in self._faces.items():
                 if len(face.e_ids) == 3 and not face.is_external:
                     three_sided[f_id] = face
         return three_sided
 
     def get_one(self, cell_type: str | int, cell_id: int):
         """
+        Get one cell of chosen type with chosen id.
         """
         _cells = self._choose_cell_type(cell_type)
         return _cells[cell_id]
     
     def get_many(self, cell_type: str | int, cell_ids: list):
         """
         """
@@ -1640,15 +1655,15 @@
         3D - faces can be special
         only internal GBs may be special
         """
         return [cell.id for cell in self._GBs.values() if cell.is_special]
 
     def get_nonspecial_internal_ids(self):
         """
-        internal and external can be special
+        internal and external can be nonspecial
         """
         cell_ids = []
         for cell in self._GBs.values():
             if not cell.is_special and not cell.is_external:
                 cell_ids.append(cell.id)
         return cell_ids
 
@@ -1894,32 +1909,16 @@
                     points.append(self._vertices[v_id].coord)
                 face.set_measure(matutils.polygon_area_2D(points))
             for edge in self._edges.values():
                 points = []
                 for v_id in edge.v_ids:
                     points.append(self._vertices[v_id].coord)
                 edge.set_measure(matutils.edge_length_2D(points))
-            
-            #     v_ids = c.get_one('f', f_id).v_ids
-#     vs = c.get_many('v', v_ids)
-#     points = np.array([v.coord2D for v in vs])
-#     d = Delaunay(points)
-#     area = 0
-#     for t in d.simplices:
-#         area += _tri_area_2D(points[t])
-#     return area
-
 
-
-    def to_TJset(self):
-        """
-        """
-        return TripleJunctionSet(self.p, self.j_tuple)
-
-    def set_junction_types(self) -> None:
+    def set_junction_types(self):
         """
         external has None junction type
         """
         if self.dim == 2:
             for v in self._vertices.values():
                 v.n_spec_edges = 0
                 if not v.is_external:
@@ -1956,15 +1955,15 @@
                     j_type = self._TJs[tj_id].junction_type
                     # j_type may be None, 0, 1, 2, 3
                     if j_type:
                         counter[j_type] += 1
                 gb_index = counter[1] + 2*counter[2] + 3*counter[3]
                 gb.set_gb_index(gb_index=gb_index)
 
-    def set_three_sided_types(self) -> None:
+    def set_three_sided_types(self):
         """
         T_{i + j}
         i - the number of special GBs (0...6)
         j - the number of triple junctions with two or more special
         boundaries (0...4) 
         i + j = 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10
         """
@@ -2004,15 +2003,15 @@
             upper_thrd: float = None,
             special_ids: list | set = None,
             warn_external: bool = True):
         """
         two options for reset:
         1. Specify new thresholds if theta is known
         2. Specify explicitly the list of special GBs
-        Options cannot be combained together.
+        Options cannot be combined together.
         If special_ids specified, then thresholds are ignored.
         GBs that are in special_ids becomes special, that aren't
         becomes not special. 
         """
         external_ids = []
         if special_ids is not None:
             for cell in self._GBs.values():
@@ -2034,14 +2033,19 @@
                     raise ValueError('Set theta first!')
                 cell._reset_theta_thrds(lower_thrd, upper_thrd)
         self.set_junction_types()
         self.set_gb_indexes()
         if self.dim == 2:
             self.set_three_sided_types()
 
+    def to_TJset(self):
+        """
+        """
+        return TripleJunctionSet(self.p, self.j_tuple)
+    
     def describe(self, attr_list: list = []):
         """
         """
         state = self.to_TJset()
         return state.get_properties(attr_list)
 
     def set_theta_from_ori(
```

### Comparing `PCCanalyser-0.1.1/matgen/matutils.py` & `PCCanalyser-0.5.0/matgen/matutils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 """
 import math
 from typing import Dict, Iterable, List, Tuple
 import numpy as np
 import random
 from scipy import sparse, linalg, stats, spatial
-import logging
+
 
 def _get_IJV_from_neighbors(_cells: Dict) -> Tuple[List]:
     """Get I, J, V lists of the adjacency matrix from a dictionary of cells.
 
     Cells can be vertices, edges, faces or polyhedra of a corresponding
     base class.
 
@@ -75,15 +75,14 @@
                 V.append(-1)
     
     return (I, J, V)
 
 
 def load_matrix_coo(filename, matrix_shape=None) -> sparse.coo_matrix:
     """
-    
     """
     M_sparse = np.loadtxt(filename, dtype='int')
     I = np.array([row[0] for row in M_sparse])
     J = np.array([row[1] for row in M_sparse])
     V = np.array([row[2] for row in M_sparse])
 
     M_coo = sparse.coo_matrix((V,(I,J)), shape=matrix_shape)
@@ -93,121 +92,14 @@
 
 def calculate_L(B1: sparse.coo_matrix, B2: sparse.coo_matrix):
     """
     """
     return B1.transpose() @ B1 + B2 @ B2.transpose()
 
 
-def entropy(*args):
-    """
-    S
-    """
-    # input arguments may be a scalar, a tuple or several scalars
-    if len(args) == 1 and isinstance(args[0], Iterable):
-        j_array = np.array(args[0])
-    else:
-        j_array = np.array(args)
-
-    # check sum of input parameters
-    if len(j_array) > 1 and not math.isclose(j_array.sum(), 1):
-        logging.warning('Sum is not equal to 1')
-
-    # calculate entropy
-    if len(j_array) == 1:
-        p = j_array[0]
-        if p == 0 or p == 1:
-            return 0
-        elif p > 0 and p < 1:
-            return - (p * math.log2(p) + (1 - p) * math.log2(1 - p))
-    elif len(j_array) > 1:
-        nonzeros = j_array[j_array > 0]
-        return - np.sum(nonzeros * np.log2(nonzeros))
-
-
-def entropy_m(*args):
-    """
-    mean part of S
-    """
-    # input arguments may be a scalar, a tuple or several scalars
-    if len(args) == 1 and isinstance(args[0], Iterable):
-        j_array = np.array(args[0])
-    else:
-        j_array = np.array(args)
-
-    # check sum of input parameters
-    if len(j_array) > 1 and not math.isclose(j_array.sum(), 1):
-        logging.warning('Sum is not equal to 1')
-
-    # check zero elements
-    if np.any(j_array == 0):
-        logging.warning('One or more j is equal to 0')
-        return np.inf
-
-    # calculate mean entropy
-    if len(j_array) == 1:
-        p = j_array[0]
-        if p == 1:
-            return np.inf
-        elif p > 0 and p < 1:
-            return - math.log2(p * (1 - p)) / 2
-    elif len(j_array) > 1:
-        return - np.log2(np.prod(j_array)) / len(j_array)
-
-
-def entropy_s(*args):
-    """
-    deviatoric part of S
-    """
-    # input arguments may be a scalar, a tuple or several scalars
-    if len(args) == 1 and isinstance(args[0], Iterable):
-        j_array = np.array(args[0])
-    else:
-        j_array = np.array(args)
-
-    # check sum of input parameters
-    if len(j_array) > 1 and not math.isclose(j_array.sum(), 1):
-        logging.warning('Sum is not equal to 1')
-
-    # check zero elements
-    if np.any(j_array == 0):
-        logging.warning('One or more j is equal to 0')
-        return - np.inf
-    
-    # calculate deviatoric entropy
-    if len(j_array) == 1:
-        p = j_array[0]
-        if p == 1:
-            return - np.inf
-        elif p > 0 and p < 1:
-            q = 1 - p
-            return - (p - q) / 2 * math.log2(p / q)
-    elif len(j_array) > 1:
-        Ss = 0
-        for k in range(len(j_array)):
-            jk = j_array[k]
-            for l in range(k + 1, len(j_array)):
-                jl = j_array[l]
-                Ss += (jk - jl) * math.log2(jk / jl)
-        Ss = Ss / len(j_array)
-        return - Ss
-
-
-def get_d_tuple(j_tuple: tuple) -> tuple:
-    """
-    """
-    if j_tuple[0] == 1:
-        return 0, 0, 0
-    else:
-        denom = 1 - j_tuple[0]
-        d1 = j_tuple[1] / denom
-        d2 = j_tuple[2] / denom
-        d3 = j_tuple[3] / denom
-        return d1, d2, d3
-
-
 def ori_mat(ori: tuple, oridesc: str ='euler-bunge:active') -> np.ndarray:
     """
     returns orientation matrix
     """
     
     if oridesc == 'euler-bunge:active':
         f1 = math.radians(ori[0])
@@ -875,34 +767,14 @@
     xs = points_coo[:, 0]
     ys = points_coo[:, 1]
 
     l2 = (xs[0] - xs[1])*(xs[0] - xs[1]) + (ys[0] - ys[1])*(ys[0] - ys[1])
     return math.sqrt(l2)
 
 
-# def metastability(S, Smax, Smin, Srand):
-#     """
-#     """    
-#     if S >= Srand and Smax != Srand:
-#         return (S - Srand) / (Smax - Srand)
-#     elif S < Srand and Smin != Srand:
-#         return (S - Srand) / (Srand - Smin)
-
-
-# def S_rand(p):
-#     """
-#     """
-#     jr0 = (1 - p)**3
-#     jr1 = 3 * p * (1 - p)**2
-#     jr2 = 3 * p**2 * (1 - p)
-#     jr3 = p**3
-
-#     return entropy(jr0, jr1, jr2, jr3)
-
-
 # def get_vor_entropy(vor):
 #     """
 #     S = - sum(Pn * log(Pn))
 #     """
 #     regions = vor.regions
 #     n_sides = np.array([len(r) for r in regions])
 #     inner_regions = [-1 not in r and len(r) >= 3 for r in regions]
```

### Comparing `PCCanalyser-0.1.1/matgen/ndisangles.py` & `PCCanalyser-0.5.0/matgen/ndisangles.py`

 * *Files identical despite different names*

### Comparing `PCCanalyser-0.1.1/matgen/ndisorientquat.py` & `PCCanalyser-0.5.0/matgen/ndisorientquat.py`

 * *Files identical despite different names*

### Comparing `PCCanalyser-0.1.1/matgen/sparsemat.py` & `PCCanalyser-0.5.0/matgen/sparsemat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 """Module to create sparse matrices from Neper output.
 
 Examples
 
     $ python sparsemat.py --file filename.tess --dir my_dir
 
+CLI tool
+
+    $ sparsemat --file filename.tess --dir my_dir
+
 """
 
 import argparse
 import os
 import time
 from typing import Dict, Tuple
 import numpy as np
@@ -148,16 +152,15 @@
                     f_id = int(row[0])
                     v_ids = []
                     for k in range(2, int(row[1]) + 2):
                         v_ids.append(int(row[k]))
                     if dim == 2:
                         face = base.Face2D(f_id, v_ids)
                     else:
-                        face = base.Face3D(f_id, v_ids)
-
+                        face = base.Face3D(f_id, v_ids)                    
                     row = file.readline().split()
                     e_ids = []
                     for k in range(1, int(row[0]) + 1):
                         e_id = int(row[k])
                         e_ids.append(abs(e_id))
                         if e_id > 0:
                             _edges[abs(e_id)].add_incident_cell(f_id)
```

### Comparing `PCCanalyser-0.1.1/matgen/utils.py` & `PCCanalyser-0.5.0/matgen/utils.py`

 * *Files identical despite different names*

### Comparing `PCCanalyser-0.1.1/pyproject.toml` & `PCCanalyser-0.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PCCanalyser"
-version = "0.1.1"
+version = "0.5.0"
 dependencies = [
-    "numpy", "scipy", "tqdm", "jupyterlab", 
-    "matplotlib",
+    "numpy >= 1.21.5", "scipy >= 1.7.3", "tqdm >= 4.64.1",
+    "jupyterlab >= 3.4.4", "matplotlib >= 3.5.2",
 ]
-description = "Polyhedral Cell Complex (PCC) Analysis tool"
+description = "Polyhedral Cell Complex (PCC) Analysis tools"
+readme = "README.md"
+
+[project.urls]
+documentation = "https://github.com/PRISBteam/Voronoi_PCC_Analyser"
+repository = "https://github.com/PRISBteam/Voronoi_PCC_Analyser.git"
 
 [tool.setuptools.packages.find]
 # All the following settings are optional:
 where = ["."]  # ["."] by default
 include = ["*"]  # ["*"] by default
 exclude = ["tutorial"]  # empty by default
 namespaces = false  # true by default
```

