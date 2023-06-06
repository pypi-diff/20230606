# Comparing `tmp/CRYSTALpytools-2023.6.6.tar.gz` & `tmp/CRYSTALpytools-2023.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CRYSTALpytools-2023.6.6.tar", last modified: Tue Jun  6 15:03:36 2023, max compression
+gzip compressed data, was "CRYSTALpytools-2023.6.7.tar", last modified: Tue Jun  6 15:12:36 2023, max compression
```

## Comparing `CRYSTALpytools-2023.6.6.tar` & `CRYSTALpytools-2023.6.7.tar`

### file list

```diff
@@ -1,25 +1,30 @@
-drwxr-xr-x   0 brunocamino   (501) staff       (20)        0 2023-06-06 15:03:36.914911 CRYSTALpytools-2023.6.6/
-drwxr-xr-x   0 brunocamino   (501) staff       (20)        0 2023-06-06 15:03:36.913292 CRYSTALpytools-2023.6.6/CRYSTALpytools/
--rw-r--r--   0 brunocamino   (501) staff       (20)      289 2023-04-25 17:05:03.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools/__init__.py
--rw-r--r--   0 brunocamino   (501) staff       (20)      577 2022-09-15 16:48:47.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools/adsorb.py
--rw-r--r--   0 brunocamino   (501) staff       (20)      757 2022-09-15 16:48:47.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools/calculate.py
--rw-r--r--   0 brunocamino   (501) staff       (20)    12828 2023-06-06 14:59:42.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools/convert.py
--rw-r--r--   0 brunocamino   (501) staff       (20)   102276 2023-06-06 14:55:03.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools/crystal_io.py
--rw-r--r--   0 brunocamino   (501) staff       (20)     3613 2022-09-15 16:48:47.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools/execute.py
--rw-r--r--   0 brunocamino   (501) staff       (20)   121442 2023-04-25 17:05:03.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools/plot.py
--rw-r--r--   0 brunocamino   (501) staff       (20)    73581 2023-06-06 14:55:03.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools/thermodynamics.py
--rw-r--r--   0 brunocamino   (501) staff       (20)    12906 2023-01-02 18:39:56.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools/unit_test.py
--rw-r--r--   0 brunocamino   (501) staff       (20)      974 2023-02-10 08:58:41.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools/units.py
--rw-r--r--   0 brunocamino   (501) staff       (20)      693 2022-09-15 16:48:47.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools/utils.py
-drwxr-xr-x   0 brunocamino   (501) staff       (20)        0 2023-06-06 15:03:36.914611 CRYSTALpytools-2023.6.6/CRYSTALpytools.egg-info/
--rw-r--r--   0 brunocamino   (501) staff       (20)      706 2023-06-06 15:03:36.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools.egg-info/PKG-INFO
--rw-r--r--   0 brunocamino   (501) staff       (20)      527 2023-06-06 15:03:36.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools.egg-info/SOURCES.txt
--rw-r--r--   0 brunocamino   (501) staff       (20)        1 2023-06-06 15:03:36.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools.egg-info/dependency_links.txt
--rw-r--r--   0 brunocamino   (501) staff       (20)       23 2023-06-06 15:03:36.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools.egg-info/requires.txt
--rw-r--r--   0 brunocamino   (501) staff       (20)       15 2023-06-06 15:03:36.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools.egg-info/top_level.txt
--rw-r--r--   0 brunocamino   (501) staff       (20)     1167 2022-09-15 16:48:47.000000 CRYSTALpytools-2023.6.6/LICENSE.txt
--rw-r--r--   0 brunocamino   (501) staff       (20)      706 2023-06-06 15:03:36.914778 CRYSTALpytools-2023.6.6/PKG-INFO
--rw-r--r--   0 brunocamino   (501) staff       (20)     3925 2023-06-06 14:55:03.000000 CRYSTALpytools-2023.6.6/README.md
--rw-r--r--   0 brunocamino   (501) staff       (20)      105 2022-12-21 17:23:54.000000 CRYSTALpytools-2023.6.6/pyproject.toml
--rw-r--r--   0 brunocamino   (501) staff       (20)       38 2023-06-06 15:03:36.914957 CRYSTALpytools-2023.6.6/setup.cfg
--rw-r--r--   0 brunocamino   (501) staff       (20)     1043 2023-06-06 15:03:22.000000 CRYSTALpytools-2023.6.6/setup.py
+drwxr-xr-x   0 brunocamino   (501) staff       (20)        0 2023-06-06 15:12:36.795747 CRYSTALpytools-2023.6.7/
+drwxr-xr-x   0 brunocamino   (501) staff       (20)        0 2023-06-06 15:12:36.791361 CRYSTALpytools-2023.6.7/CRYSTALpytools/
+-rw-r--r--   0 brunocamino   (501) staff       (20)      467 2023-06-06 15:10:07.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools/__init__.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)      577 2022-09-15 16:48:47.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools/adsorb.py
+drwxr-xr-x   0 brunocamino   (501) staff       (20)        0 2023-06-06 15:12:36.795317 CRYSTALpytools-2023.6.7/CRYSTALpytools/base/
+-rw-r--r--   0 brunocamino   (501) staff       (20)      122 2023-06-06 15:10:07.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools/base/__init__.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)    11964 2023-06-06 15:10:07.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools/base/basisset.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)    47067 2023-06-06 15:10:07.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools/base/crysd12.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)     9266 2023-06-06 15:10:07.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools/base/inputbase.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)      757 2022-09-15 16:48:47.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools/calculate.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)    16727 2023-06-06 15:10:07.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools/convert.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)   103231 2023-06-06 15:10:07.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools/crystal_io.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)     3613 2022-09-15 16:48:47.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools/execute.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)   121442 2023-04-25 17:05:03.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools/plot.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)    73581 2023-06-06 14:55:03.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools/thermodynamics.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)    12902 2023-06-06 15:10:07.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools/unit_test.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)      974 2023-02-10 08:58:41.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools/units.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)      693 2022-09-15 16:48:47.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools/utils.py
+drwxr-xr-x   0 brunocamino   (501) staff       (20)        0 2023-06-06 15:12:36.793259 CRYSTALpytools-2023.6.7/CRYSTALpytools.egg-info/
+-rw-r--r--   0 brunocamino   (501) staff       (20)      706 2023-06-06 15:12:36.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools.egg-info/PKG-INFO
+-rw-r--r--   0 brunocamino   (501) staff       (20)      655 2023-06-06 15:12:36.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools.egg-info/SOURCES.txt
+-rw-r--r--   0 brunocamino   (501) staff       (20)        1 2023-06-06 15:12:36.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools.egg-info/dependency_links.txt
+-rw-r--r--   0 brunocamino   (501) staff       (20)       23 2023-06-06 15:12:36.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools.egg-info/requires.txt
+-rw-r--r--   0 brunocamino   (501) staff       (20)       15 2023-06-06 15:12:36.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools.egg-info/top_level.txt
+-rw-r--r--   0 brunocamino   (501) staff       (20)     1167 2022-09-15 16:48:47.000000 CRYSTALpytools-2023.6.7/LICENSE.txt
+-rw-r--r--   0 brunocamino   (501) staff       (20)      706 2023-06-06 15:12:36.795615 CRYSTALpytools-2023.6.7/PKG-INFO
+-rw-r--r--   0 brunocamino   (501) staff       (20)     3925 2023-06-06 14:55:03.000000 CRYSTALpytools-2023.6.7/README.md
+-rw-r--r--   0 brunocamino   (501) staff       (20)      105 2022-12-21 17:23:54.000000 CRYSTALpytools-2023.6.7/pyproject.toml
+-rw-r--r--   0 brunocamino   (501) staff       (20)       38 2023-06-06 15:12:36.795790 CRYSTALpytools-2023.6.7/setup.cfg
+-rw-r--r--   0 brunocamino   (501) staff       (20)     1043 2023-06-06 15:12:25.000000 CRYSTALpytools-2023.6.7/setup.py
```

### Comparing `CRYSTALpytools-2023.6.6/CRYSTALpytools/adsorb.py` & `CRYSTALpytools-2023.6.7/CRYSTALpytools/adsorb.py`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.6.6/CRYSTALpytools/calculate.py` & `CRYSTALpytools-2023.6.7/CRYSTALpytools/calculate.py`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.6.6/CRYSTALpytools/convert.py` & `CRYSTALpytools-2023.6.7/CRYSTALpytools/convert.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-Created on Fri Nov 19 18:29:16 2021
-
+Functions that do conversion between data / file formats
 """
 
-def cry_ase2gui(structure, dimensionality = 3, symmetry = True):
+def cry_ase2gui(structure, pbc=[True, True, True], symmetry=True):
+    """
+    Transform an ASE Structure object into a Pymatgen structure object and then
+    a CRYSTAL structure (gui) object.
+
+    Args:
+        structure (ASE Structure)
+        pbc (list[bool]): Periodic boundary conditions.
+        symmetry (bool)
+    """
     # First transform into pmg and then write the gui
 
     from pymatgen.io.ase import AseAtomsAdaptor
 
     pmg_structure = AseAtomsAdaptor().get_structure(structure)
 
-    return cry_pmg2gui(pmg_structure, dimensionality=dimensionality, symmetry=symmetry)
-    
+    return cry_pmg2gui(pmg_structure, pbc=pbc, symmetry=symmetry)
+
 
 def cry_bands2pmg(output, bands, labels=None):
     # WORK IN TRANSFORMATION
     #Transform a CRYSTAL bands object into a pymatgen bands object
 
     # output_file is a crystal output object
     # bands is a crystal bands object
@@ -76,24 +84,33 @@
     #gui_file is the CRYSTAL structure (gui) file
 
     from pymatgen.io.ase import AseAtomsAdaptor
 
     return AseAtomsAdaptor().get_atoms(cry_gui2pmg(gui_file))
 
 
-def cry_gui2cif(cif_file_name, gui):
-    #Read a CRYSTAL structure (gui) file and save a cif file
-    # cif_file_name: name (including path) of the cif file to be saved
-    # gui_file: CRYSTAL gui object
-
+def cry_gui2cif(cif_file_name, gui, symprec=0.01, angle_tolerance=5.0):
+    """
+    Read a CRYSTAL structure (gui) file and save a cif file. The CifWriter
+    object of PyMatGen is called.
+
+    Args:
+        cif_file_name (str): Name (including path) of the cif file to be saved
+        gui (Crystal_gui): CRYSTALpytools gui object
+        symprec (float): Refer to `CifWriter's manual <https://pymatgen.org/pymatgen.io.cif.html#pymatgen.io.cif.CifWriter>`_.
+            If none, CIF output without symmetry.
+        angle_tolerance (float): Refer to `CifWriter's manual <https://pymatgen.org/pymatgen.io.cif.html#pymatgen.io.cif.CifWriter>`_
+    """
     from pymatgen.io.cif import CifWriter
 
     structure = cry_gui2pmg(gui)
-    
-    CifWriter(structure).write_file(cif_file_name)
+
+    CifWriter(structure,
+              symprec=symprec,
+              angle_tolerance=angle_tolerance).write_file(cif_file_name)
 
 
 def cry_gui2pmg(gui, vacuum=10, molecule = True):
     #Transform a CRYSTAL structure (gui) object into a pymatgen Structure object
     #Vacuum needs to be included because pymatgen only includes 3D symmetry
     # molecule = True generates a Molecule pymatgen object for 0D structures
     # molecule = False generates a Molecule pymatgen with vacuum object for 0D structures
@@ -232,100 +249,154 @@
 
     structure = Structure(vectors, output.atom_numbers, 
                               atom_positions, coords_are_cartesian=True)
 
     return structure
 
 
-def cry_pmg2gui(structure, dimensionality = 3, symmetry = True):
-    #Transform a CRYSTAL structure (gui) object into a pymatgen Structure object
-    #Vacuum needs to be included because pymatgen only includes 3D symmetry
-    # molecule = True generates a Molecule pymatgen object for 0D structures
-    # molecule = False generates a Molecule pymatgen with vacuum object for 0D structures
-    
-    #from . import crystal_io
+def cry_pmg2gui(structure, pbc=[True, True, True], symmetry=True, zconv=None):
+    """
+    Transform a pymatgen Structure object into a CRYSTAL structure (gui) object.
+    Vacuum needs to be included because pymatgen only includes 3D symmetry.
+
+    Args:
+        structure (Structure | Molecule): Pymatgen Structure / Molecule object.
+        pbc (list[bool]): Periodic boundary conditions along the x, y, z directions.
+        symmetry (bool): Do symmetry analysis.
+        zconv (list[list[int, int]]): 1st element: The **index** of atom;
+                2nd element: The new conventional atomic number.
+    """
     from CRYSTALpytools.crystal_io import Crystal_gui
     from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
     from pymatgen.core.surface import center_slab
-    
+    from pymatgen.core.structure import Molecule
+
     import numpy as np
-    import sys
+    import warnings
     import copy
 
     gui = Crystal_gui()
+    dimensionality = pbc.count(True)
 
-    if dimensionality == 0 and 'Molecule' not in str(type(structure)):
-        print('WARNING: dimensionality is set to 0, but the structure is not a molecule')
-        sys.exit(1)
-    elif dimensionality == 0 and 'Molecule' in str(type(structure)):
-        lattice_vectors = np.identity(3)*500.
+    if dimensionality == 0 and 'Molecule' in str(type(structure)):
+        molecule = structure
+        is_molecule = True # 0D object called as molecule
     elif dimensionality > 0:
-        lattice_vectors = copy.deepcopy(structure.lattice.matrix)
-    
-    gui.dimensionality = dimensionality
-
-    if dimensionality == 2:
-        lattice_vectors[2][2] = 500.
-    
-    if dimensionality == 1:
-        lattice_vectors[1][1] = 500.
-        lattice_vectors[2][2] = 500.
-
-    gui.lattice = lattice_vectors
-    gui.n_atoms = structure.num_sites
-    gui.space_group = SpacegroupAnalyzer(structure).get_space_group_number()
-    gui.symmops = []
-    
-    if symmetry == True:
-        n_symmops = 0
-        if dimensionality == 3:
-            symmops = SpacegroupAnalyzer(structure).get_symmetry_operations(cartesian=True)
-
-            for symmop in symmops:
-                if np.all(symmop.translation_vector == 0.):
-                    n_symmops += 1
-                    gui.symmops.extend(symmop.rotation_matrix.tolist())
-                    gui.symmops.append(symmop.translation_vector.tolist())
-            
-            gui.n_symmops = n_symmops
+        is_molecule = False # >0D object called as structure
+    elif dimensionality == 0 and 'Molecule' not in str(type(structure)):
+        warnings.warn('Dimensionality is set to 0, but the structure is not a molecule. Periodicity will be removed.')
+        molecule = Molecule(structure.species,
+                            [i.coords for i in structure.sites],
+                            structure.charge,
+                            [i.properties for i in struc.sites]) 
+        is_molecule = True # 0D object called as molecule
+    elif dimensionality > 0 and 'Molecule' in str(type(structure)):
+        warnings.warn('Dimensionality is set to 1-3, but the structure is a molecule. Periodicity will be added.')
+        structure = structure.get_boxed_structure(500., 500., 500.)
+        is_molecule = False # >0D object called as structure
 
-        elif dimensionality == 2:
-
-            #center the slab first
-            structure = center_slab(structure)
-
-            # Then center at z=0.0
-            translation = np.array([0.0, 0.0, -0.5])
-            structure.translate_sites(list(range(structure.num_sites)),
-                                          translation, to_unit_cell=False)
-            
-            sg = SpacegroupAnalyzer(structure)
-            ops = sg.get_symmetry_operations(cartesian=True)
-            for op in ops:
-                if np.all(op.translation_vector == 0.):
-                    n_symmops += 1
-                    gui.symmops.extend(op.rotation_matrix.tolist())
-                    gui.symmops.append(op.translation_vector.tolist())
-         
-            gui.n_symmops = n_symmops
-
-        elif dimensionality == 1:
-            print('WARNING: check the polymer is correctly centered in the cell and that the correct symmops are used.')      
+    gui.dimensionality = dimensionality
 
-        elif dimensionality == 0:
-            print('WARNING: 0D in development')
-            sys.exit(1)
-     
-    else:
+    if is_molecule == True: # 0D
+        lattice_vectors = np.identity(3)*500.
+        gui.lattice = lattice_vectors
+        gui.n_atoms = molecule.num_sites
+        gui.space_group = 1
+        gui.symmops = []
         gui.n_symmops = 1
         gui.symmops.extend(np.identity(3).tolist())
         gui.symmops.append([0.0,0.0,0.0])
+        gui.atom_number = list(molecule.atomic_numbers)
+        gui.atom_positions = molecule.cart_coords.tolist()
+    else: # 1-3D
+        if dimensionality == 2:
+            if pbc[0] == False: # X no periodicity
+                warnings.warn('The non-periodic direction will be rotated to z axis.')
+                mx = structure.lattice.matrix
+                lattice_vectors = np.array([[mx[1, 1], mx[1, 2], 0.],
+                                            [mx[2, 1], mx[2, 2], 0.],
+                                            [0., 0., 500.]])
+            elif pbc[1] == False: # Y no periodicity
+                warnings.warn('The non-periodic direction will be rotated to z axis.')
+                mx = structure.lattice.matrix
+                lattice_vectors = np.array([[mx[0, 2], mx[0, 0], 0.],
+                                            [mx[2, 2], mx[2, 0], 0.],
+                                            [0., 0., 500.]])
+            else: # Z no periodicity
+                lattice_vectors = copy.deepcopy(structure.lattice.matrix)
+
+        elif dimensionality == 1:
+            if pbc[0] == True: # X periodic
+                lattice_vectors = copy.deepcopy(structure.lattice.matrix)
+            elif pbc[1] == True: # Y periodic
+                warnings.warn('The periodic direction will be rotated to x axis.')
+                mx = structure.lattice.matrix
+                lattice_vectors = np.array([[mx[1, 1], 0., 0.],
+                                            [0., 500., 0.],
+                                            [0., 0., 500.]])
+            else: # Z periodic
+                warnings.warn('The periodic direction will be rotated to x axis.')
+                mx = structure.lattice.matrix
+                lattice_vectors = np.array([[mx[2, 2], 0., 0.],
+                                            [0., 500., 0.],
+                                            [0., 0., 500.]])
+        else:
+            lattice_vectors = copy.deepcopy(structure.lattice.matrix)
+
+        gui.lattice = lattice_vectors
+        gui.n_atoms = structure.num_sites
+        gui.space_group = SpacegroupAnalyzer(structure).get_space_group_number()
+        gui.symmops = []
+
+        if symmetry == True:
+            n_symmops = 0
+            if dimensionality == 3:
+                symmops = SpacegroupAnalyzer(structure).get_symmetry_operations(cartesian=True)
+
+                for symmop in symmops:
+                    if np.all(symmop.translation_vector == 0.):
+                        n_symmops += 1
+                        gui.symmops.extend(symmop.rotation_matrix.tolist())
+                        gui.symmops.append(symmop.translation_vector.tolist())
+
+                gui.n_symmops = n_symmops
+
+            elif dimensionality == 2:
+
+                #center the slab first
+                structure = center_slab(structure)
+
+                # Then center at z=0.0
+                translation = np.array([0.0, 0.0, -0.5])
+                structure.translate_sites(list(range(structure.num_sites)),
+                                          translation, to_unit_cell=False)
 
-    gui.atom_number = list(structure.atomic_numbers)
-    gui.atom_positions = structure.cart_coords.tolist()
+                sg = SpacegroupAnalyzer(structure)
+                ops = sg.get_symmetry_operations(cartesian=True)
+                for op in ops:
+                    if np.all(op.translation_vector == 0.):
+                        n_symmops += 1
+                        gui.symmops.extend(op.rotation_matrix.tolist())
+                        gui.symmops.append(op.translation_vector.tolist())
+
+                gui.n_symmops = n_symmops
+
+            else:
+                warnings.warn('Check the polymer is correctly centered in the cell and that the correct symmops are used.')
+        else:
+            gui.n_symmops = 1
+            gui.symmops.extend(np.identity(3).tolist())
+            gui.symmops.append([0.0,0.0,0.0])
+
+        gui.atom_number = list(structure.atomic_numbers)
+        gui.atom_positions = structure.cart_coords.tolist()
+
+    if zconv != None:
+        for atom in zconv:
+            gui.atom_number[atom[0]] = atom[1]
 
     return gui
 
 
 def cry_out2xyz(xyz_file_name, output):
     #Transform a CRYSTAL structure (gui) file into an ASE bands object
     #The gui file is firt transfomed into a pymatgen object
```

### Comparing `CRYSTALpytools-2023.6.6/CRYSTALpytools/crystal_io.py` & `CRYSTALpytools-2023.6.7/CRYSTALpytools/crystal_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,128 +1,107 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-Created on Fri Nov 19 18:28:28 2021
+Objects of input / output files of CRYSTAL. Methods to edit or substract data
+from corresponding files are provided.
 """
 from CRYSTALpytools import units
 from CRYSTALpytools.base.crysd12 import Crystal_inputBASE
 
 
 class Crystal_input(Crystal_inputBASE):
     """
-    Crystal input object inherited from Crystal_inputBASE.
-
-    **Note for users**
-
-    ``Crystal_input`` object is strictly structured by 'blocks', which, in
-    general, is defined as keywords that are closed by 'END'. All the blocks
-    are organized in layers and each corresponds to a list of keywords that can
-    be called and set.The current structure of ``Crystal_input`` is listed
-    below:
-
-    # Layer 1: ``geom``, ``basisset``, ``scf``
-    # Layer 2: ``optgeom``, ``freqcalc``, ``dft``, ``dftd3``, ``gcp``, ``fixindex``
-    # Layer 3: ``preoptgeom``, ``geom``, ``base``
-
-    For example, to set force convergence threshold of a optimization run:
-
-    Usage::
-
-        obj = Crystal_input()
-        obj.geom.optgeom.toldeg(0.0001)
-
-    In principle, by calling the 'block-like' attribute, a 'block-like' object
-    will be automatically generated if the attribute is empty. The exception is
-    the 3rd layer attributes, which must be set by ``set_attr()`` method. A
-    warning message is printed to indicate the name of the opened sub-block
-    since it usually does not correspond to CRYSTAL keywords to avoid potential
-    conflicts.
-
-    Usage::
-
-        obj.geom.freqcalc.set_preoptgeom()
-        obj.geom.freqcalc.optgeom.toldeg(0.0003)
-
-    Methods and sub-blocks of ``Crystal_input`` usually have the same name as
-    corresponding keywords. One can setup, change or clean the keyword by
-    calling the corresponding method.
-
-    Usage::
-
-        obj.scf.toldee(9) # Set SCF TOLDEE = 9
-        obj.scf.toldee('') # Clean the TOLDEE keyword and value
-        obj.scf.ppan() # Print PPAN keyword, without value
-
-    Though one can set CRYSTAL input object by manually setting up all the
-    attributes, it is also possible to read a template d12 file and do
-    modifications.
-
-    Usage::
-
-        obj.from_file('opt.d12')
-        obj.geom.optgeom('') # Remove OPTGEOM block
-        obj.to_file('scf.d12') # Print it into file
+    Crystal input object inherited from the :ref:`Crystal_inputBASE <ref-base-crysd12>`
+    object. For the basic set-ups of keywords, please refer to manuals there.
+    """
+    def __init__(self):
+        super(Crystal_input, self).__init__()
 
-    It is also possible to set individual blocks by a string. The ``set_block``
-    method should be used. The keyword for the block itself should not be
-    included.
+    def geom_from_cif(self, file, zconv=None, keyword='EXTERNAL',
+                      pbc=[True, True, True], gui_name='fort.34',
+                      symprec=0.01, angle_tolerance=5.0):
+        """
+        Read geometry from cif file and put infomation to geom block, either as
+        'EXTERNAL' or 'CRYSTAL'. CIF files with a single geometry only.
 
-    Usage::
+        CIF with Symmetry is required.
 
-        obj.scf.set_dft('SPIN\nEXCHANGE\nPBE\nCORRELAT\nP86\n')
+        .. note::
 
-    For basis set, it can be read from an external basis set file. '99 0' and
-    'END' should not be included.
+            CIF files should have the '.cif' extension.
 
-    Usage::
+        Args:
+            file (str): CIF file.
+            keyword (str): 'EXTERNAL' or 'CRYSTAL'.
+            zconv (list[list[int, int]]): 1st element: The **index** of atom;
+                2nd element: The new conventional atomic number. Atoms of the
+                irreducible unit is required.
+            pbc (list[bool]): *Limited to keyword = EXTERNAL*. Periodic boundary
+                conditions along x, y, z axis
+            gui_name (str): *Limited to keyword = EXTERNAL*. Gui file's name.
+            symprec (float): *Limited to keyword = CRYSTAL*. If not none,
+                finds the symmetry of the structure. See `pymatgen.symmetry.analyzer.SpacegroupAnalyzer <https://pymatgen.org/pymatgen.symmetry.analyzer.html#pymatgen.symmetry.analyzer.SpacegroupAnalyzer>`_
+            angle_tolerance (float): *Limited to keyword = CRYSTAL*. See `pymatgen.symmetry.analyzer.SpacegroupAnalyzer <https://pymatgen.org/pymatgen.symmetry.analyzer.html#pymatgen.symmetry.analyzer.SpacegroupAnalyzer>`_
+        """
+        import re
+        from pymatgen.core.structure import IStructure
 
-        obj.basisset.bs_from_file('mybasis.txt')
+        struc = IStructure.from_file(file)
+        self.geom_from_pmg(struc, zconv, keyword, pbc, gui_name, symprec, angle_tolerance)
 
-    To examine the data in a block object, including Crystal_input obj itself,
-    call the ``data`` attribute.
+        return
 
-    Usage::
+    def geom_from_pmg(self, struc, zconv=None, keyword='EXTERNAL',
+                      pbc=[True, True, True], gui_name='fort.34',
+                      symprec=0.01, angle_tolerance=5.0):
+        """
+        Read geometry defined by PyMatGen structure object and put infomation
+        into geom block, either as 'EXTERNAL' or 'CRYSTAL'.
 
-        obj.data
+        See ``geom_from_cif`` for definition of arguments.
+        """
+        import re
+        from CRYSTALpytools.convert import cry_pmg2gui
 
-    """
+        if re.match(r'^EXTERNAL$', keyword, re.IGNORECASE):
+            super(Crystal_input, self).geom.external()
+            gui = cry_pmg2gui(struc, pbc=pbc, symmetry=True, zconv=zconv)
+            gui.write_gui(gui_name, symm=True)
+        elif re.match(r'^CRYSTAL$', keyword, re.IGNORECASE):
+            self._pmg2input(struc, zconv, symprec=symprec, angle_tolerance=angle_tolerance)
+        else:
+            raise ValueError("Input keyword format error: {}".format(keyword))
 
-    def __init__(self):
-        super(Crystal_input, self).__init__()
+        return
 
-    def crystal_from_cif(self, file, symprec=0.01, angle_tolerance=5.0):
+    def _pmg2input(self, struc, zconv=None, symprec=0.01, angle_tolerance=5.0):
         """
-        Read geometry from cif file and put infomation under 'CRYSTAL' keyword.
-        3D structure only. CIF files with a single geometry only.
+        Pymatgen IStructure object to 'CRYSTAL' input block
 
         .. note::
 
             Coordinates of corresponding atoms may not consistent with the
             original CIF file, in which case coordinates of another symmetry
             equivalent atom is used.
 
-            When multiple choices of periodic cell exist (typically for
-            low-symmetric non-orthgonal systems such as monoclinic or trilinic
-            cells), this method might lead to errors due to the inconsistent
-            choice of periodic cell between CRYSTAL and pymatgen.
-
-        Args:
-            file (str): CIF file name
-            symprec (float): If not none, finds the symmetry of the structure.
-                See `pymatgen.symmetry.analyzer.SpacegroupAnalyzer <https://pymatgen.org/pymatgen.symmetry.analyzer.html#pymatgen.symmetry.analyzer.SpacegroupAnalyzer>`_
-            angle_tolerance (float): See `pymatgen.symmetry.analyzer.SpacegroupAnalyzer <https://pymatgen.org/pymatgen.symmetry.analyzer.html#pymatgen.symmetry.analyzer.SpacegroupAnalyzer>`_
+            When multiple choices of periodic cell exist, this method might
+            lead to errors due to the inconsistent choice of periodic cell
+            between CRYSTAL and pymatgen.
         """
         import numpy as np
         from pymatgen.core.structure import IStructure
         from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
 
-        struc = IStructure.from_file(file, primitive=True)
         analyzer = SpacegroupAnalyzer(
             struc, symprec=symprec, angle_tolerance=angle_tolerance)
-        struc_symm = analyzer.get_symmetrized_structure()
+        # Analyze the refined geometry
+        struc2 = analyzer.get_refined_structure()
+        analyzer2 = SpacegroupAnalyzer(
+            struc2, symprec=symprec, angle_tolerance=angle_tolerance)
+        struc_symm = analyzer2.get_symmetrized_structure()
 
         sg = analyzer.get_space_group_number()
         latt = []
         if sg >= 1 and sg < 3:  # trilinic
             for i in ['a', 'b', 'c', 'alpha', 'beta', 'gamma']:
                 latt.append(round(
                     getattr(struc_symm.lattice, i), 6
@@ -154,25 +133,40 @@
                 ))
         else:  # cubic
             latt.append(round(struc_sym.lattice.a, 6))
 
         natom = len(struc_symm.equivalent_sites)
         eq_atom = int(len(struc_symm.species) / natom)
         atominfo = []
+        if zconv != None:
+            z_atom_index = [i[0] for i in zconv]
         for i in range(natom):
             idx_eq = int(i * eq_atom)
+            if zconv == None:
+                z_input = struc_symm.species[idx_eq].Z
+            else:
+                try:
+                    atom_to_sub = z_atom_index.index(i)
+                    z_input = zconv[atom_to_sub][1]
+                except ValueError:
+                    z_input = struc_symm.species[idx_eq].Z
             atominfo.append([
-                int(struc_symm.species[idx_eq].Z),
-                round(struc_symm.equivalent_sites[i][0].frac_coords[0], 8),
-                round(struc_symm.equivalent_sites[i][0].frac_coords[1], 8),
-                round(struc_symm.equivalent_sites[i][0].frac_coords[2], 8)
+                '{:<3}'.format(z_input),
+                '{0:11.8f}'.format(
+                    round(struc_symm.equivalent_sites[i][0].frac_coords[0], 8)
+                ),
+                '{0:11.8f}'.format(
+                    round(struc_symm.equivalent_sites[i][0].frac_coords[1], 8)
+                ),
+                '{0:11.8f}'.format(
+                    round(struc_symm.equivalent_sites[i][0].frac_coords[2], 8)
+                )
             ])
 
-        super(Crystal_input, self).geom.crystal(
-            IGR=sg, latt=latt, atom=atominfo)
+        super(Crystal_input, self).geom.crystal(IGR=sg, latt=latt, atom=atominfo)
 
         return
 
 
 class Crystal_output:
     # This class reads a CRYSTAL output and generates an object
 
@@ -492,31 +486,31 @@
                     self.band_gap = np.array(band_gap_spin)
                     return self.band_gap
         if self.spin_pol == True and band_gap_spin == []:
             print(
                 'DEV WARNING: check this output and the band gap function in crystal_io')
 
     def get_last_geom(self, write_gui_file=True, symm_info='pymatgen'):
-        # Return the last optimised geometry
-
-        # write_gui_file == True writes the last geometry to the gui file
-        # symm_info == 'pymatgen' uses the symmetry info from a pymatgen object
-        # otherwise it is taken from the existing gui file
+        """
+        Return the last optimised geometry
 
+        Args:
+            write_gui_file (bool): Whether to write the last geometry to gui
+                file.
+            symm_info (str): 'pymatgen' to use symmetry info from a pymatgen
+                object, otherwise it is taken from the existing gui file
+        """
         import re
         from mendeleev import element
         import numpy as np
-        import sys
         from pymatgen.core.structure import Structure, Molecule
         from CRYSTALpytools.convert import cry_pmg2gui
 
         dimensionality = self.get_dimensionality()
 
-        
-
         # Find the last geometry
         for i, line in enumerate(self.data):
             if re.match(r' TRANSFORMATION MATRIX PRIMITIVE-CRYSTALLOGRAPHIC CELL', line):
                 trans_matrix_flat = [float(x) for x in self.data[i+1].split()]
                 self.trans_matrix = []
                 for i in range(0, len(trans_matrix_flat), 3):
                     self.trans_matrix.append(trans_matrix_flat[i:i+3])
@@ -592,28 +586,34 @@
                         elif self.name[-4:] == 'outp':
                             gui_file = self.name[:-5]+'.gui'
                         else:
                             gui_file = self.name+'.gui'
 
                         structure = Structure(lattice, self.atom_numbers,
                                               self.atom_positions_cart, coords_are_cartesian=True)
-                        gui_object = cry_pmg2gui(structure)
+                        if dimensionality == 0:
+                            pbc = [False, False, False]
+                        elif dimensionality == 1:
+                            pbc = [True, False, False]
+                        elif dimensionality == 2:
+                            pbc = [True, True, False]
+                        else:
+                            pbc = [True, True, True]
+                        gui_object = cry_pmg2gui(structure, pbc=pbc)
 
-                        gui_object.write_crystal_gui(gui_file)
+                        gui_object.write_gui(gui_file)
                     else:
                         gui_file = symm_info
                         try:
                             file = open(gui_file, 'r')
                             gui_data = file.readlines()
                             file.close()
                         except:
-                            print(
-                                'EXITING: a .gui file with the same name as the input need to be present in the directory.')
-                            sys.exit(1)
-
+                            raise FileNotFoundError(
+                                'A .gui file with the same name as the input need to be present in the directory.')
                         # Replace the lattice vectors with the optimised ones
                         for i, vector in enumerate(lattice.tolist()):
                             gui_data[i+1] = ' '.join([str(x)
                                                       for x in vector])+'\n'
 
                         n_symmops = int(gui_data[4])
                         for i in range(len(self.atom_numbers)):
@@ -2160,38 +2160,37 @@
         self.datax = df.dist
         self.datay = df.rho
 
         return self
 
 
 class Crystal_gui:
-    # This class reads a CRYSTAL gui file and generates an object
-
+    """
+    This class can read a CRYSTAL gui file into an object or substrate
+    information of the object to generate a gui file.
+    """
     def __init__(self):
-        # Initialise the Crystal_gui
-
         pass
 
-    def read_cry_gui(self, gui_file):
-        # gui_filename: name of the gui file
-
-        # gui_file is the CRYSTAL structure (gui) file
-        # This is used mainly to convert the object into an ASE or pymatgen object
-
-        import sys
+    def read_gui(self, gui_file):
+        """
+        This is used mainly to convert the object into an ASE or pymatgen
+        object.
 
+        Args:
+            gui_file (str): The CRYSTAL structure (gui) file
+        """
         try:
             if gui_file[-3:] != 'gui' and gui_file[-3:] != 'f34' and 'optc' not in gui_file:
                 gui_file = gui_file + '.gui'
             file = open(gui_file, 'r')
             data = file.readlines()
             file.close()
         except:
-            print('EXITING: a .gui file needs to be specified')
-            sys.exit(1)
+            raise FileNotFoundError('A .gui file needs to be specified')
 
         self.dimensionality = int(data[0].split()[0])
         self.lattice = []
         self.symmops = []
         for i in range(1, 4):
             self.lattice.append([float(x) for x in data[i].split()])
         self.n_symmops = int(data[4].split()[0])
@@ -2204,59 +2203,69 @@
             atom_line = data[i].split()
             self.atom_number.append(str(atom_line[0]))
             self.atom_positions.append([float(x) for x in atom_line[1:]])
         self.space_group = int(data[-1].split()[0])
 
         return self
 
-    def write_crystal_gui(self, gui_file, symm=True, pseudo_atoms=[]):
-        # Write a CRYSTAL gui file (to file)
-        # gui_file is the name of the gui that is going to be written (including .gui)
-        # ext_structure is the structure object from ase or pymatgen
-        # dimensionality is the dimensionality of the system
-        # symm == True includes the symmops
-        # pseudo_atoms is a list of atoms whose core is described by a pseudopotential
+    def write_gui(self, gui_file, symm=True, pseudo_atoms=[]):
+        """
+        Write a CRYSTAL gui file (to file)
 
+        Args:
+            gui_file (str): The name of the gui that is going to be written (
+                including .gui).
+            symm (bool): Whether to include symmetry operations.
+            pseudo_atoms (list[int]): A list of atoms whose core is described
+                by a pseudopotential
+        """
         import numpy as np
 
         with open(gui_file, 'w') as file:
 
             # First line
-            file.writelines('%s   1   1\n' % self.dimensionality)
+            file.writelines('%4s   1   1\n' % self.dimensionality)
             # Cell vectors
             for vector in self.lattice:
-                file.writelines(
-                    ' '.join((format(np.round(n, 12), '.12E')) for n in vector)+'\n')
+                file.writelines('{}\n'.format(
+                    ''.join(['{0: 20.12E}'.format(np.round(n, 12)) for n in vector])
+                ))
             # N symm ops
-            file.writelines('{}\n'.format(str(self.n_symmops)))
+            file.writelines('{:5d}\n'.format(self.n_symmops))
 
             # symm ops
             for symmops in self.symmops:
                 file.writelines('{}\n'.format(
-                    # ' '.join(str(np.around(n, 8)) for n in symmops)))
-                    ' '.join(str(format(np.round(n, 12), '.12E')) for n in symmops)))
-
+                    ''.join(['{0: 20.12f}'.format(np.round(n, 12)) for n in symmops])
+                ))
             # N atoms
-            file.writelines('{}\n'.format(self.n_atoms))
+            file.writelines('{:5d}\n'.format(self.n_atoms))
 
             # atom number (including pseudopotentials) + coordinates cart
             for i in range(self.n_atoms):
                 if self.atom_number[i] in pseudo_atoms:
-                    file.writelines('{} {}\n'.format(int(self.atom_number[i])+200,
-                                                     ' '.join([str(x) for x in self.atom_positions[i]])))
+                    file.writelines('{:5d}{}\n'.format(
+                        int(self.atom_number[i])+200,
+                        ''.join(['{0: 20.12E}'.format(np.round(x, 12)) for x in self.atom_positions[i]])
+                    ))
                 else:
-                    file.writelines('{} {}\n'.format(self.atom_number[i],
-                                                     ' '.join([str(format(np.round(x, 12), '.12E')) for x in self.atom_positions[i]])))
+                    file.writelines('{:5d}{}\n'.format(
+                        int(self.atom_number[i]),
+                        ''.join(['{0: 20.12E}'.format(np.round(x, 12)) for x in self.atom_positions[i]])
+                    ))
 
             # space group + n symm ops
             if symm == True:
-                file.writelines('{} {}'.format(
-                    self.space_group, self.n_symmops))
+                file.writelines('{:5d}{:5d}\n'.format(
+                    self.space_group, self.n_symmops
+                ))
             else:
-                file.writelines('1 1')
+                file.writelines('{:5d}{:5d}\n'.format(1, 1))
+
+        file.close()
 
 
 class Crystal_density():
     # WORK IN PROGRESS
     # Returns a crystal_density object
 
     def __init__(self):
```

### Comparing `CRYSTALpytools-2023.6.6/CRYSTALpytools/execute.py` & `CRYSTALpytools-2023.6.7/CRYSTALpytools/execute.py`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.6.6/CRYSTALpytools/plot.py` & `CRYSTALpytools-2023.6.7/CRYSTALpytools/plot.py`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.6.6/CRYSTALpytools/thermodynamics.py` & `CRYSTALpytools-2023.6.7/CRYSTALpytools/thermodynamics.py`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.6.6/CRYSTALpytools/unit_test.py` & `CRYSTALpytools-2023.6.7/CRYSTALpytools/unit_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -383,15 +383,15 @@
     else:
         test_result.append(False)
 
     # CRY_GUI2PMG
 
     test_attr.append('cry_gui2pmg')
     mgo_gui = Crystal_gui()
-    mgo_gui.read_cry_gui(gui_file)
+    mgo_gui.read_gui(gui_file)
     pmg_obj = cry_gui2pmg(mgo_gui)
     
     lattice_matrix = np.round(np.array([[-1.29819297e-16,  2.12011001e+00,  2.12011001e+00],
        [ 2.12011001e+00,  0.00000000e+00,  2.12011001e+00],
        [ 2.12011001e+00,  2.12011001e+00,  2.59638594e-16]]),8)
     
     cart_coord = np.round(np.array([[0.     , 0.     , 0.     ],
```

### Comparing `CRYSTALpytools-2023.6.6/CRYSTALpytools/units.py` & `CRYSTALpytools-2023.6.7/CRYSTALpytools/units.py`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.6.6/CRYSTALpytools/utils.py` & `CRYSTALpytools-2023.6.7/CRYSTALpytools/utils.py`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.6.6/CRYSTALpytools.egg-info/PKG-INFO` & `CRYSTALpytools-2023.6.7/CRYSTALpytools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CRYSTALpytools
-Version: 2023.6.6
+Version: 2023.6.7
 Summary: Python tools for the CRYSTAL code developed and mantained by the CRYSTAL code developers.
 Home-page: https://github.com/crystal-code-tools/CRYSTALpytools
 Author-email: crystalcodetools@gmail.com
 Project-URL: Bug Tracker, https://github.com/crystal-code-tools/CRYSTALpytools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: CRYSTALpytools Version: 2023.6.6 Summary: Python
+Metadata-Version: 2.1 Name: CRYSTALpytools Version: 2023.6.7 Summary: Python
 tools for the CRYSTAL code developed and mantained by the CRYSTAL code
 developers. Home-page: https://github.com/crystal-code-tools/CRYSTALpytools
 Author-email: crystalcodetools@gmail.com Project-URL: Bug Tracker, https://
 github.com/crystal-code-tools/CRYSTALpytools/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown License-File: LICENSE.txt Python tools for the CRYSTAL_code developed
```

### Comparing `CRYSTALpytools-2023.6.6/CRYSTALpytools.egg-info/SOURCES.txt` & `CRYSTALpytools-2023.6.7/CRYSTALpytools.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -13,8 +13,12 @@
 CRYSTALpytools/unit_test.py
 CRYSTALpytools/units.py
 CRYSTALpytools/utils.py
 CRYSTALpytools.egg-info/PKG-INFO
 CRYSTALpytools.egg-info/SOURCES.txt
 CRYSTALpytools.egg-info/dependency_links.txt
 CRYSTALpytools.egg-info/requires.txt
-CRYSTALpytools.egg-info/top_level.txt
+CRYSTALpytools.egg-info/top_level.txt
+CRYSTALpytools/base/__init__.py
+CRYSTALpytools/base/basisset.py
+CRYSTALpytools/base/crysd12.py
+CRYSTALpytools/base/inputbase.py
```

### Comparing `CRYSTALpytools-2023.6.6/LICENSE.txt` & `CRYSTALpytools-2023.6.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.6.6/PKG-INFO` & `CRYSTALpytools-2023.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CRYSTALpytools
-Version: 2023.6.6
+Version: 2023.6.7
 Summary: Python tools for the CRYSTAL code developed and mantained by the CRYSTAL code developers.
 Home-page: https://github.com/crystal-code-tools/CRYSTALpytools
 Author-email: crystalcodetools@gmail.com
 Project-URL: Bug Tracker, https://github.com/crystal-code-tools/CRYSTALpytools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: CRYSTALpytools Version: 2023.6.6 Summary: Python
+Metadata-Version: 2.1 Name: CRYSTALpytools Version: 2023.6.7 Summary: Python
 tools for the CRYSTAL code developed and mantained by the CRYSTAL code
 developers. Home-page: https://github.com/crystal-code-tools/CRYSTALpytools
 Author-email: crystalcodetools@gmail.com Project-URL: Bug Tracker, https://
 github.com/crystal-code-tools/CRYSTALpytools/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown License-File: LICENSE.txt Python tools for the CRYSTAL_code developed
```

### Comparing `CRYSTALpytools-2023.6.6/README.md` & `CRYSTALpytools-2023.6.7/README.md`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.6.6/setup.py` & `CRYSTALpytools-2023.6.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 long_description = 'Python tools for the <a href="https://www.crystal.unito.it/index.php">CRYSTAL code</a> developed and mantained by the CRYSTAL code developers'
 
 setuptools.setup(
     name="CRYSTALpytools",        
-    version="2023.06.06",
+    version="2023.06.07",
     author_email="crystalcodetools@gmail.com",
     description="Python tools for the CRYSTAL code developed and mantained by the CRYSTAL code developers.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/crystal-code-tools/CRYSTALpytools",
     project_urls={
         "Bug Tracker": "https://github.com/crystal-code-tools/CRYSTALpytools/issues",
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 import setuptools long_description = 'Python tools for the CRYSTAL_code
 developed and mantained by the CRYSTAL code developers' setuptools.setup
-( name="CRYSTALpytools", version="2023.06.06",
+( name="CRYSTALpytools", version="2023.06.07",
 author_email="crystalcodetools@gmail.com", description="Python tools for the
 CRYSTAL code developed and mantained by the CRYSTAL code developers.",
 long_description=long_description, long_description_content_type="text/
 markdown", url="https://github.com/crystal-code-tools/CRYSTALpytools",
 project_urls={ "Bug Tracker": "https://github.com/crystal-code-tools/
 CRYSTALpytools/issues", }, classifiers=[ "Programming Language :: Python :: 3",
 "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",
```

