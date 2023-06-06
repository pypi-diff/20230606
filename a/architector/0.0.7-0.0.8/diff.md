# Comparing `tmp/architector-0.0.7.tar.gz` & `tmp/architector-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "architector-0.0.7.tar", last modified: Mon Mar 20 22:14:41 2023, max compression
+gzip compressed data, was "architector-0.0.8.tar", last modified: Tue Jun  6 16:25:27 2023, max compression
```

## Comparing `architector-0.0.7.tar` & `architector-0.0.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:14:41.760993 architector-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-03-20 22:14:38.000000 architector-0.0.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-20 22:14:38.000000 architector-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-03-20 22:14:41.760993 architector-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-03-20 22:14:38.000000 architector-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:14:41.760993 architector-0.0.7/architector/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-20 22:14:38.000000 architector-0.0.7/architector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 22:14:38.000000 architector-0.0.7/architector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-20 22:14:41.760993 architector-0.0.7/architector/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-03-20 22:14:38.000000 architector-0.0.7/architector/arch_context_manage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-03-20 22:14:38.000000 architector-0.0.7/architector/ase_db_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    41433 2023-03-20 22:14:38.000000 architector-0.0.7/architector/complex_construction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:14:41.760993 architector-0.0.7/architector/data/
--rw-r--r--   0 runner    (1001) docker     (123) 27596793 2023-03-20 22:14:38.000000 architector-0.0.7/architector/data/angle_stats_datasource.csv
--rw-r--r--   0 runner    (1001) docker     (123)    18350 2023-03-20 22:14:38.000000 architector-0.0.7/architector/data/ligtype_angle_reference.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13997 2023-03-20 22:14:38.000000 architector-0.0.7/architector/geometries.py
--rw-r--r--   0 runner    (1001) docker     (123)    20628 2023-03-20 22:14:38.000000 architector-0.0.7/architector/io_align_mol.py
--rw-r--r--   0 runner    (1001) docker     (123)    16600 2023-03-20 22:14:38.000000 architector-0.0.7/architector/io_calc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18848 2023-03-20 22:14:38.000000 architector-0.0.7/architector/io_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-03-20 22:14:38.000000 architector-0.0.7/architector/io_crest.py
--rw-r--r--   0 runner    (1001) docker     (123)    79274 2023-03-20 22:14:38.000000 architector-0.0.7/architector/io_lig.py
--rw-r--r--   0 runner    (1001) docker     (123)    44449 2023-03-20 22:14:38.000000 architector-0.0.7/architector/io_molecule.py
--rw-r--r--   0 runner    (1001) docker     (123)    30242 2023-03-20 22:14:38.000000 architector-0.0.7/architector/io_obabel.py
--rw-r--r--   0 runner    (1001) docker     (123)    68314 2023-03-20 22:14:38.000000 architector-0.0.7/architector/io_process_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    39950 2023-03-20 22:14:38.000000 architector-0.0.7/architector/io_ptable.py
--rw-r--r--   0 runner    (1001) docker     (123)    14894 2023-03-20 22:14:38.000000 architector-0.0.7/architector/io_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)    20602 2023-03-20 22:14:38.000000 architector-0.0.7/architector/io_xtb_calc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-03-20 22:14:38.000000 architector-0.0.7/architector/vibrations_free_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-03-20 22:14:38.000000 architector-0.0.7/architector/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:14:41.724990 architector-0.0.7/architector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-03-20 22:14:41.000000 architector-0.0.7/architector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-20 22:14:41.000000 architector-0.0.7/architector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 22:14:41.000000 architector-0.0.7/architector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-20 22:14:41.000000 architector-0.0.7/architector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-20 22:14:41.000000 architector-0.0.7/architector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-20 22:14:41.760993 architector-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-03-20 22:14:38.000000 architector-0.0.7/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-03-20 22:14:38.000000 architector-0.0.7/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:25:27.165297 architector-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-06 16:25:23.000000 architector-0.0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-06 16:25:23.000000 architector-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-06-06 16:25:27.165297 architector-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14077 2023-06-06 16:25:23.000000 architector-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:25:27.165297 architector-0.0.8/architector/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-06 16:25:23.000000 architector-0.0.8/architector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 16:25:23.000000 architector-0.0.8/architector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-06 16:25:27.165297 architector-0.0.8/architector/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-06 16:25:23.000000 architector-0.0.8/architector/arch_context_manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-06-06 16:25:23.000000 architector-0.0.8/architector/ase_db_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42356 2023-06-06 16:25:23.000000 architector-0.0.8/architector/complex_construction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:25:27.165297 architector-0.0.8/architector/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 27596793 2023-06-06 16:25:23.000000 architector-0.0.8/architector/data/angle_stats_datasource.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    18350 2023-06-06 16:25:23.000000 architector-0.0.8/architector/data/ligtype_angle_reference.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13997 2023-06-06 16:25:23.000000 architector-0.0.8/architector/geometries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20628 2023-06-06 16:25:23.000000 architector-0.0.8/architector/io_align_mol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16875 2023-06-06 16:25:23.000000 architector-0.0.8/architector/io_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18848 2023-06-06 16:25:23.000000 architector-0.0.8/architector/io_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-06-06 16:25:23.000000 architector-0.0.8/architector/io_crest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79274 2023-06-06 16:25:23.000000 architector-0.0.8/architector/io_lig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44449 2023-06-06 16:25:23.000000 architector-0.0.8/architector/io_molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31158 2023-06-06 16:25:23.000000 architector-0.0.8/architector/io_obabel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68735 2023-06-06 16:25:23.000000 architector-0.0.8/architector/io_process_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39950 2023-06-06 16:25:23.000000 architector-0.0.8/architector/io_ptable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14894 2023-06-06 16:25:23.000000 architector-0.0.8/architector/io_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20602 2023-06-06 16:25:23.000000 architector-0.0.8/architector/io_xtb_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-06 16:25:23.000000 architector-0.0.8/architector/vibrations_free_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-06-06 16:25:23.000000 architector-0.0.8/architector/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:25:27.117297 architector-0.0.8/architector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-06-06 16:25:27.000000 architector-0.0.8/architector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-06 16:25:27.000000 architector-0.0.8/architector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 16:25:27.000000 architector-0.0.8/architector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-06 16:25:27.000000 architector-0.0.8/architector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-06 16:25:27.000000 architector-0.0.8/architector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-06 16:25:27.165297 architector-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-06 16:25:23.000000 architector-0.0.8/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-06 16:25:23.000000 architector-0.0.8/versioneer.py
```

### Comparing `architector-0.0.7/LICENSE.txt` & `architector-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `architector-0.0.7/PKG-INFO` & `architector-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: architector
-Version: 0.0.7
+Version: 0.0.8
 Summary: The architector python package - for 3D inorganometallic complex design.
 Author: Michael G. Taylor et al.
 License: BSD 3-Clause License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Chemistry
@@ -12,14 +12,20 @@
 License-File: LICENSE.txt
 
 # Architector
 
 Architector is a 3D chemical structure generation software package designed to take minimal 2D information about ligands and metal centers and generates chemically sensible 3D conformers and stereochemistry of the organometallic compounds.
 It is capable of high-throughput in-silico construction of s-, p-, d-, and f-block organometallic complexes. Architector represents a transformative step towards cross-periodic table computational design of metal complex chemistry.
 
+### If you use this package for your work please cite the manuscript and code:
+
+1. Manuscript: Taylor, M.G., Burrill, D.J., Janssen, J., Batsita, E.R., Perez, D., and Yang. P. Architector for high-throughput cross-periodic table 3D complex building. Nat Commun 14, 2786 (2023). https://doi.org/10.1038/s41467-023-38169-2
+
+2. Code: https://www.github.com/lanl/Architector 
+
 ## Installation
 
 Conda installation recommended. The conda-forge distribution can be installed via: 
 
 ```bash
 conda install -c conda-forge architector
 ```
@@ -33,16 +39,17 @@
 ```
 
 ## Useful Tools/Examples:
 
 1. See tutorials for basic introduction to capabilties and code examples: `documentation/tutorials/`
 2. Reference for core and ligand geometry labels see: `documentation/view_default_core_ligand_types.ipynb`
 3. Utility for aiding in determining ligand coordination sites see: `utils/ligand_viewing_coordinating_atom_selecting.ipynb`
+4. Reference for debugging cases where no structures are generated see: `documentation/Debugging_Guide.ipynb`
 
-* Note that ligands used in (3) can even be drawn in [Avogadro](https://avogadro.cc/) and copied as SMILES strings into this analysis.
+* Note that ligands used in (3) can even be drawn in [Avogadro](https://avogadro.cc/) and or most other 2D molecular editors (e.g. ChemDraw) and copied as SMILES strings into this analysis.
 * If other analyses are used to determine the coordinating atom indices we can't guarantee the generated structure will match what was input. If generating complexes with new ligands we HIGHLY recommend using the utility in (3)
 
 ## XTB (backend) Potentially Useful References:
 * [Available Solvents](https://xtb-docs.readthedocs.io/en/latest/gbsa.html)
 * [Available Methods](https://xtb-python.readthedocs.io/en/latest/general-api.html)
 * [ASE Calculator](https://xtb-python.readthedocs.io/en/latest/ase-calculator.html)
 * [XTB Documentation](https://xtb-docs.readthedocs.io/en/latest/contents.html)
@@ -118,14 +125,19 @@
     # for the "full_method", or turn "relaxation" off.
     "xtb_solvent": 'none', # Add any named XTB solvent!
     "xtb_accuracy": 1.0, # Numerical Accuracy for XTB calculations
     "xtb_electronic_temperature": 300, # In K -> fermi smearing - increase for convergence on harder systems
     "xtb_max_iterations": 250, # Max iterations for xtb SCF.
     "force_generation":False, # Whether to force the construction to proceed without xtb energies - defaults to UFF evaluation
     # in cases of XTB outright failure. Will still enforce sanity checks on output structures.
+    "ff_preopt":False, # Whether to force forcefield (FF) pre-optimization of fully-built complexes before final xtb evalulation.
+    # FF preoptimization helps especially in cases where longer carbon chains are present that tend to overlap.
+    # This option will also decrease the maximum force tolerance for xtb relaxation to 0.2 and set assemble_method='GFN-FF'
+    # By default for acceleration.
+
 
     # Covalent radii and vdw radii of the metal if nonstandard radii requested.
     "vdwrad_metal": vdwrad_metal,
     "covrad_metal": covrad_metal,
 
     ####### Conformer parameters and information stored ########
     "n_conformers": 1, # Number of metal-core symmetries at each core to save / relax
```

### Comparing `architector-0.0.7/README.md` & `architector-0.0.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # Architector
 
 Architector is a 3D chemical structure generation software package designed to take minimal 2D information about ligands and metal centers and generates chemically sensible 3D conformers and stereochemistry of the organometallic compounds.
 It is capable of high-throughput in-silico construction of s-, p-, d-, and f-block organometallic complexes. Architector represents a transformative step towards cross-periodic table computational design of metal complex chemistry.
 
+### If you use this package for your work please cite the manuscript and code:
+
+1. Manuscript: Taylor, M.G., Burrill, D.J., Janssen, J., Batsita, E.R., Perez, D., and Yang. P. Architector for high-throughput cross-periodic table 3D complex building. Nat Commun 14, 2786 (2023). https://doi.org/10.1038/s41467-023-38169-2
+
+2. Code: https://www.github.com/lanl/Architector 
+
 ## Installation
 
 Conda installation recommended. The conda-forge distribution can be installed via: 
 
 ```bash
 conda install -c conda-forge architector
 ```
@@ -20,16 +26,17 @@
 ```
 
 ## Useful Tools/Examples:
 
 1. See tutorials for basic introduction to capabilties and code examples: `documentation/tutorials/`
 2. Reference for core and ligand geometry labels see: `documentation/view_default_core_ligand_types.ipynb`
 3. Utility for aiding in determining ligand coordination sites see: `utils/ligand_viewing_coordinating_atom_selecting.ipynb`
+4. Reference for debugging cases where no structures are generated see: `documentation/Debugging_Guide.ipynb`
 
-* Note that ligands used in (3) can even be drawn in [Avogadro](https://avogadro.cc/) and copied as SMILES strings into this analysis.
+* Note that ligands used in (3) can even be drawn in [Avogadro](https://avogadro.cc/) and or most other 2D molecular editors (e.g. ChemDraw) and copied as SMILES strings into this analysis.
 * If other analyses are used to determine the coordinating atom indices we can't guarantee the generated structure will match what was input. If generating complexes with new ligands we HIGHLY recommend using the utility in (3)
 
 ## XTB (backend) Potentially Useful References:
 * [Available Solvents](https://xtb-docs.readthedocs.io/en/latest/gbsa.html)
 * [Available Methods](https://xtb-python.readthedocs.io/en/latest/general-api.html)
 * [ASE Calculator](https://xtb-python.readthedocs.io/en/latest/ase-calculator.html)
 * [XTB Documentation](https://xtb-docs.readthedocs.io/en/latest/contents.html)
@@ -105,14 +112,19 @@
     # for the "full_method", or turn "relaxation" off.
     "xtb_solvent": 'none', # Add any named XTB solvent!
     "xtb_accuracy": 1.0, # Numerical Accuracy for XTB calculations
     "xtb_electronic_temperature": 300, # In K -> fermi smearing - increase for convergence on harder systems
     "xtb_max_iterations": 250, # Max iterations for xtb SCF.
     "force_generation":False, # Whether to force the construction to proceed without xtb energies - defaults to UFF evaluation
     # in cases of XTB outright failure. Will still enforce sanity checks on output structures.
+    "ff_preopt":False, # Whether to force forcefield (FF) pre-optimization of fully-built complexes before final xtb evalulation.
+    # FF preoptimization helps especially in cases where longer carbon chains are present that tend to overlap.
+    # This option will also decrease the maximum force tolerance for xtb relaxation to 0.2 and set assemble_method='GFN-FF'
+    # By default for acceleration.
+
 
     # Covalent radii and vdw radii of the metal if nonstandard radii requested.
     "vdwrad_metal": vdwrad_metal,
     "covrad_metal": covrad_metal,
 
     ####### Conformer parameters and information stored ########
     "n_conformers": 1, # Number of metal-core symmetries at each core to save / relax
@@ -238,8 +250,8 @@
 This program was produced under U.S. Government contract 89233218CNA000001 for Los Alamos
 National Laboratory (LANL), which is operated by Triad National Security, LLC for the U.S.
 Department of Energy/National Nuclear Security Administration. All rights in the program are
 reserved by Triad National Security, LLC, and the U.S. Department of Energy/National Nuclear
 Security Administration. The Government is granted for itself and others acting on its behalf a
 nonexclusive, paid-up, irrevocable worldwide license in this material to reproduce, prepare
 derivative works, distribute copies to the public, perform publicly and display publicly, and to permit
-others to do so.
+others to do so.
```

### Comparing `architector-0.0.7/architector/arch_context_manage.py` & `architector-0.0.8/architector/arch_context_manage.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.7/architector/ase_db_utilities.py` & `architector-0.0.8/architector/ase_db_utilities.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.7/architector/complex_construction.py` & `architector-0.0.8/architector/complex_construction.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import architector.io_obabel as io_obabel
 import architector.io_lig as io_lig
 import architector.io_ptable as io_ptable
 import architector.io_molecule as io_molecule
 import architector.io_align_mol as io_align_mol
 import architector.io_crest as io_crest
 import architector.io_symmetry as io_symmetry
-
 from architector.io_calc import CalcExecutor
 
 class Ligand:
     """Class to contain all information about a ligand including conformers."""
 
     def __init__(self, smiles, ligcoordList, corecoordList, core, ligGeo, ligcharge,
                 covrad_metal=None, vdwrad_metal=None, debug=False):
@@ -236,19 +235,33 @@
         single_point : bool, optional
             Perform only a singlepoint calculation?, by default False
         """
         self.final_start_time = time.time()
         self.initMol.dist_sanity_checks(params=self.parameters,assembly=single_point)
         self.initMol.graph_sanity_checks(params=self.parameters,assembly=single_point)
         if self.assembled:
+            if self.parameters['ff_preopt'] and (not single_point):
+                if self.parameters['debug']:
+                    print('Doing UFF - pre-optimization before final evaluation.')
+                calculator = CalcExecutor(self.complexMol, parameters=self.parameters,
+                                final_sanity_check=False,
+                                relax=True, assembly=single_point, 
+                                ff_preopt_run=self.parameters['ff_preopt'])
+                if calculator:
+                    self.complexMol.ase_atoms.set_positions(calculator.mol.ase_atoms.get_positions())
             if self.parameters['debug']:
                 print("Final Evaluation - Opt Molecule/Single point")
-            self.calculator = CalcExecutor(self.complexMol,parameters=self.parameters,
-                                            final_sanity_check=self.parameters['full_sanity_checks'],
-                                            relax=single_point,assembly=single_point)
+            self.calculator = CalcExecutor(self.complexMol,
+                                           parameters=self.parameters,
+                                           final_sanity_check=self.parameters['full_sanity_checks'],
+                                           relax=single_point,
+                                           assembly=single_point)
+            if (self.parameters['debug']) and (self.calculator):
+                print('Finished method: {} {}.'.format(self.calculator.method,
+                                                    self.calculator.relax))
             if self.parameters['debug'] and (not self.calculator.successful):
                 print('Failed final relaxation. - Retrying with UFF/XTB')
                 print(self.initMol.write_mol2('cool.mol2', writestring=True))
             # Retry with 2 step optimization -> first do UFF -> then do the requested method.
             if (not self.calculator.successful):
                 tmp_relax = CalcExecutor(self.complexMol,method='UFF',fix_m_neighbors=False,relax=single_point)
                 self.calculator = CalcExecutor(tmp_relax.mol,parameters=self.parameters,
```

### Comparing `architector-0.0.7/architector/data/angle_stats_datasource.csv` & `architector-0.0.8/architector/data/angle_stats_datasource.csv`

 * *Files identical despite different names*

### Comparing `architector-0.0.7/architector/data/ligtype_angle_reference.csv` & `architector-0.0.8/architector/data/ligtype_angle_reference.csv`

 * *Files identical despite different names*

### Comparing `architector-0.0.7/architector/geometries.py` & `architector-0.0.8/architector/geometries.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.7/architector/io_align_mol.py` & `architector-0.0.8/architector/io_align_mol.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.7/architector/io_calc.py` & `architector-0.0.8/architector/io_calc.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 }
 
 class CalcExecutor:
     def __init__(self, structure, parameters={}, init_sanity_check=False,
                 final_sanity_check=False, relax=False, assembly=False,
                 method='GFN2-xTB', xtb_solvent='none', xtb_accuracy=1.0,
                 xtb_electronic_temperature=300, xtb_max_iterations=250,
-                fmax=0.1, maxsteps=1000,
+                fmax=0.1, maxsteps=1000, ff_preopt_run=False,
                 detect_spin_charge=False, fix_m_neighbors=False,
                 default_params=params, ase_opt_method=None,
                 calculator=None):
         """CalcExecutor is the class handling all calculations of full metal-ligand complexes.
 
         Parameters
         ----------
@@ -103,14 +103,16 @@
             Electronic temp for smearing, default 300 K
         xtb_max_iterations : float, optional
             Maximum iterations for xtb SCF convergence, default 250.
         fmax : float, optional
             Max force in eV/Angstrom, by default 0.1
         maxsteps : int, optional
             Total number of optimization steps to take, by default 1000
+        ff_preopt_run : bool, optional
+            Perform forcefield pre-optimization?, by default False
         detect_spin_charge : bool, optional
             Detect the charge and spin with openbabel routines?, by default False
         fix_m_neighbors : bool, optional
             Set the metal neighbors as fixed, by default False
         default_params :dict, optional
             default parameters to evaluate to, by default params
         ase_opt_method : ase.optimize Optimizer, optional
@@ -126,14 +128,15 @@
         default_params.update(parameters)
         self.parameters = default_params
         self.init_sanity_check = init_sanity_check
         self.final_sanity_check = final_sanity_check
         self.calculator = calculator
         self.relax = relax
         self.assembly = assembly
+        self.ff_preopt_run = ff_preopt_run
         self.xtb_solvent = xtb_solvent
         self.xtb_accuracy = xtb_accuracy
         self.xtb_electronic_temperature = xtb_electronic_temperature
         self.xtb_max_iterations = xtb_max_iterations
         self.fmax = fmax
         self.fix_m_neighbors = fix_m_neighbors
         self.maxsteps = maxsteps
@@ -144,15 +147,18 @@
             for key,val in parameters.items():
                 setattr(self,key,val)
             if assembly:
                 self.init_sanity_check = True
                 self.relax = False
                 self.method = self.assemble_method
             else:
-                self.method = self.full_method
+                if self.ff_preopt_run:
+                    self.method = 'UFF'
+                else:
+                    self.method = self.full_method
         if ase_opt_method is None: # Default to LBFGSLineSearch
             self.opt_method = LBFGSLineSearch
         else:
             self.opt_method = ase_opt_method
         # Temporary logfile or not for ase optimizer
         if self.parameters['debug']: # Set logfile to suppress stdout output.
             self.logfile = None
```

### Comparing `architector-0.0.7/architector/io_core.py` & `architector-0.0.8/architector/io_core.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.7/architector/io_crest.py` & `architector-0.0.8/architector/io_crest.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.7/architector/io_lig.py` & `architector-0.0.8/architector/io_lig.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.7/architector/io_molecule.py` & `architector-0.0.8/architector/io_molecule.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.7/architector/io_obabel.py` & `architector-0.0.8/architector/io_obabel.py`

 * *Files 2% similar despite different names*

```diff
@@ -375,15 +375,16 @@
     # Optimize energy
     FF.ConjugateGradients(2000,1e-6)
     FF.GetCoordinates(OBmol)
     return OBmol
 
 
 def generate_obmol_conformers(smiles, rmsd_cutoff=0.4, conf_cutoff=3000, energy_cutoff=50.0, 
-        confab_verbose = False, output_format='mol2', neutralize=False, functionalizations=None):
+        confab_verbose = False, output_format='mol2', neutralize=False, functionalizations=None,
+        return_energies = False):
     """generate_obmol_conformers 
     generate conformers with openbabel for given smiles
     using confab conformer generation routine
     O'Boyle NM, Vandermeersch T, Flynn CJ, Maguire AR, Hutchison GR. Confab 
     - Systematic generation of diverse low-energy conformers. Journal of Cheminformatics. 
     2011;3:8. doi:10.1186/1758-2946-3-8.
 
@@ -401,40 +402,62 @@
         give more detailed output, by default False
     output_format : str, optional
         which format to output , by default 'mol2'
     neutralize : bool, optional
         neutralize smiles?, by default False
     functionalizations : dict, optional
         add functionalizations?, by default None
+    return_energies : bool, optional
+        return the FF energies in addition to the conformers generated
 
     Returns
     -------
     output_strings : list (str)
         list of conformers generated as whatever format desired
+    output_energies : list (float)
+        forcefield energies
     """
     obmol = get_obmol_smiles(smiles,
                              neutralize=neutralize,
                              functionalizations=functionalizations)
     mmff94_ok = check_mmff_okay(obmol)
     if mmff94_ok:
         FF = ob.OBForceField.FindForceField("MMFF94")
         FF.Setup(obmol) # Make sure setup works OK
     else:
-        FF = ob.OBForceField.FindForceField("MMFF94")
+        FF = ob.OBForceField.FindForceField("UFF")
         FF.Setup(obmol) # Make sure setup works OK
+    # Run Diverse conformer generation
     FF.DiverseConfGen(rmsd_cutoff, conf_cutoff, energy_cutoff, confab_verbose)
     FF.GetConformers(obmol)
     confs_to_write = obmol.NumConformers()
     obconversion = ob.OBConversion()
     obconversion.SetOutFormat(output_format)
     output_strings = []
+    output_energies = []
     for conf_num in range(confs_to_write):
         obmol.SetConformer(conf_num)
+        if return_energies: # Calculate FF energies
+            if mmff94_ok:
+                FF = ob.OBForceField.FindForceField("MMFF94")
+                FF.Setup(obmol) # Make sure setup works OK
+            else:
+                FF = ob.OBForceField.FindForceField("UFF")
+                FF.Setup(obmol) # Make sure setup works OK
+            energy = FF.Energy()
+            if mmff94_ok:
+                energy = energy * units.kcal / units.mol
+            else:
+                energy = energy * units.kJ / units.mol
+            output_energies.append(energy)
         output_strings.append(obconversion.WriteString(obmol))
-    return output_strings
+    if return_energies:
+        return output_strings,output_energies
+    else:
+        return output_strings
 
 
 def functionalize(OBmol,functional_group='C',smiles_inds=[0]):
     """functionalize functionalization routine
 
     Parameters
     ----------
```

### Comparing `architector-0.0.7/architector/io_process_input.py` & `architector-0.0.8/architector/io_process_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -740,14 +740,15 @@
             "full_spin": None, # Assign spin to the full complex (overrides metal_spin)
             "full_charge": None, # Assign charge to the complex (overrides ligand charges and metal_ox)!
             "full_method":"GFN2-xTB", # Which method to use for final cleaning/evaulating conformers.
             "assemble_method":"GFN2-xTB", # Which method to use for assembling conformers. 
             "fmax":0.1, # eV/Angstrom - max force for relaxation.
             "maxsteps":1000, # Steps involved in relaxation
             "force_generation":False, # Whether to force the construction to proceed without xtb energies - defaults to UFF
+            "ff_preopt":False, # Perform forcefield pre-optimization of full complex? - default False.
             # In cases of XTB outright failure.
             # For very large speedup - use GFN-FF, though this is much less stable (especially for Lanthanides)
             # Or UFF
 
             "skip_duplicate_tests":False, # Skip the duplicate tests (return all generated/relaxed configurations)
             
             # Covalent radii and vdw radii of the metal if deviations requested.
@@ -849,14 +850,20 @@
             outparams['ase_db'] = None
 
         # Screen out non-trans geos if requested
         if outparams['force_trans_oxos']:
             coreTypes = [x for x in newinpDict['coreTypes'] if x in core_geo_class.trans_geos]
             newinpDict['coreTypes'] = coreTypes
 
+        # FF-preoptimization shifts
+        if outparams['ff_preopt']:
+            outparams['assemble_method'] = 'GFN-FF'
+            outparams['assemble_sanity_checks'] = False # Allow for close/overlapping atoms 
+            outparams['fmax'] = 0.2 # Slightly decrease accuracy to encourage difficult convergence
+ 
         # # Load logger
         # if outparams['logg']
         newinpDict['parameters'] = outparams
 
         # Initialize seed.
         if isinstance(newinpDict['parameters']['seed'],(int,float,np.float64,np.int64)):
             np.random.seed(int(newinpDict['parameters']['seed']))
```

### Comparing `architector-0.0.7/architector/io_ptable.py` & `architector-0.0.8/architector/io_ptable.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.7/architector/io_symmetry.py` & `architector-0.0.8/architector/io_symmetry.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.7/architector/io_xtb_calc.py` & `architector-0.0.8/architector/io_xtb_calc.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.7/architector/vibrations_free_energy.py` & `architector-0.0.8/architector/vibrations_free_energy.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.7/architector/visualization.py` & `architector-0.0.8/architector/visualization.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.7/architector.egg-info/PKG-INFO` & `architector-0.0.8/architector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: architector
-Version: 0.0.7
+Version: 0.0.8
 Summary: The architector python package - for 3D inorganometallic complex design.
 Author: Michael G. Taylor et al.
 License: BSD 3-Clause License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Chemistry
@@ -12,14 +12,20 @@
 License-File: LICENSE.txt
 
 # Architector
 
 Architector is a 3D chemical structure generation software package designed to take minimal 2D information about ligands and metal centers and generates chemically sensible 3D conformers and stereochemistry of the organometallic compounds.
 It is capable of high-throughput in-silico construction of s-, p-, d-, and f-block organometallic complexes. Architector represents a transformative step towards cross-periodic table computational design of metal complex chemistry.
 
+### If you use this package for your work please cite the manuscript and code:
+
+1. Manuscript: Taylor, M.G., Burrill, D.J., Janssen, J., Batsita, E.R., Perez, D., and Yang. P. Architector for high-throughput cross-periodic table 3D complex building. Nat Commun 14, 2786 (2023). https://doi.org/10.1038/s41467-023-38169-2
+
+2. Code: https://www.github.com/lanl/Architector 
+
 ## Installation
 
 Conda installation recommended. The conda-forge distribution can be installed via: 
 
 ```bash
 conda install -c conda-forge architector
 ```
@@ -33,16 +39,17 @@
 ```
 
 ## Useful Tools/Examples:
 
 1. See tutorials for basic introduction to capabilties and code examples: `documentation/tutorials/`
 2. Reference for core and ligand geometry labels see: `documentation/view_default_core_ligand_types.ipynb`
 3. Utility for aiding in determining ligand coordination sites see: `utils/ligand_viewing_coordinating_atom_selecting.ipynb`
+4. Reference for debugging cases where no structures are generated see: `documentation/Debugging_Guide.ipynb`
 
-* Note that ligands used in (3) can even be drawn in [Avogadro](https://avogadro.cc/) and copied as SMILES strings into this analysis.
+* Note that ligands used in (3) can even be drawn in [Avogadro](https://avogadro.cc/) and or most other 2D molecular editors (e.g. ChemDraw) and copied as SMILES strings into this analysis.
 * If other analyses are used to determine the coordinating atom indices we can't guarantee the generated structure will match what was input. If generating complexes with new ligands we HIGHLY recommend using the utility in (3)
 
 ## XTB (backend) Potentially Useful References:
 * [Available Solvents](https://xtb-docs.readthedocs.io/en/latest/gbsa.html)
 * [Available Methods](https://xtb-python.readthedocs.io/en/latest/general-api.html)
 * [ASE Calculator](https://xtb-python.readthedocs.io/en/latest/ase-calculator.html)
 * [XTB Documentation](https://xtb-docs.readthedocs.io/en/latest/contents.html)
@@ -118,14 +125,19 @@
     # for the "full_method", or turn "relaxation" off.
     "xtb_solvent": 'none', # Add any named XTB solvent!
     "xtb_accuracy": 1.0, # Numerical Accuracy for XTB calculations
     "xtb_electronic_temperature": 300, # In K -> fermi smearing - increase for convergence on harder systems
     "xtb_max_iterations": 250, # Max iterations for xtb SCF.
     "force_generation":False, # Whether to force the construction to proceed without xtb energies - defaults to UFF evaluation
     # in cases of XTB outright failure. Will still enforce sanity checks on output structures.
+    "ff_preopt":False, # Whether to force forcefield (FF) pre-optimization of fully-built complexes before final xtb evalulation.
+    # FF preoptimization helps especially in cases where longer carbon chains are present that tend to overlap.
+    # This option will also decrease the maximum force tolerance for xtb relaxation to 0.2 and set assemble_method='GFN-FF'
+    # By default for acceleration.
+
 
     # Covalent radii and vdw radii of the metal if nonstandard radii requested.
     "vdwrad_metal": vdwrad_metal,
     "covrad_metal": covrad_metal,
 
     ####### Conformer parameters and information stored ########
     "n_conformers": 1, # Number of metal-core symmetries at each core to save / relax
```

### Comparing `architector-0.0.7/architector.egg-info/SOURCES.txt` & `architector-0.0.8/architector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `architector-0.0.7/setup.py` & `architector-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.7/versioneer.py` & `architector-0.0.8/versioneer.py`

 * *Files identical despite different names*

