# Comparing `tmp/python-sscha-1.3.tar.gz` & `tmp/python-sscha-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sscha-1.3.tar", last modified: Tue Jun  6 10:23:25 2023, max compression
+gzip compressed data, was "python-sscha-1.3.1.tar", last modified: Tue Jun  6 11:29:28 2023, max compression
```

## Comparing `python-sscha-1.3.tar` & `python-sscha-1.3.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 10:23:25.297097 python-sscha-1.3/
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    35149 2023-02-13 14:58:18.000000 python-sscha-1.3/LICENSE.txt
-drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 10:23:25.281097 python-sscha-1.3/Modules/
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    10879 2023-02-13 14:58:18.000000 python-sscha-1.3/Modules/AdvancedCalculations.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     4823 2023-02-13 14:58:18.000000 python-sscha-1.3/Modules/Calculator.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    66394 2023-05-16 12:51:43.000000 python-sscha-1.3/Modules/Cluster.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    10288 2023-02-13 14:58:18.000000 python-sscha-1.3/Modules/Dynamical.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)   132589 2023-02-23 10:36:25.000000 python-sscha-1.3/Modules/Ensemble.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    15683 2023-02-13 14:58:18.000000 python-sscha-1.3/Modules/Minimizer.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    15751 2023-02-13 14:58:18.000000 python-sscha-1.3/Modules/Optimizer.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     1173 2023-02-13 14:58:18.000000 python-sscha-1.3/Modules/Parallel.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    32819 2023-02-23 10:36:25.000000 python-sscha-1.3/Modules/Relax.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    76682 2023-02-23 10:37:43.000000 python-sscha-1.3/Modules/SchaMinimizer.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    18362 2023-02-13 14:58:18.000000 python-sscha-1.3/Modules/Tools.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    24140 2023-02-13 14:58:18.000000 python-sscha-1.3/Modules/Utilities.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)       80 2023-02-13 14:58:18.000000 python-sscha-1.3/Modules/__init__.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)      227 2023-06-06 10:23:25.297097 python-sscha-1.3/PKG-INFO
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     8066 2023-05-16 12:51:43.000000 python-sscha-1.3/README.md
-drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 10:23:25.285097 python-sscha-1.3/SCHAModules/
--rw-rw-r--   0 monacell  (1001) monacell  (1001)      870 2023-02-13 14:58:18.000000 python-sscha-1.3/SCHAModules/cell_force.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     3354 2023-02-13 14:58:18.000000 python-sscha-1.3/SCHAModules/get_cmat.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     1442 2023-02-13 14:58:18.000000 python-sscha-1.3/SCHAModules/get_emat.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     1333 2023-02-13 14:58:18.000000 python-sscha-1.3/SCHAModules/get_g.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    17132 2023-02-23 10:36:26.000000 python-sscha-1.3/SCHAModules/get_gradient_supercell.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    14175 2023-02-13 14:58:18.000000 python-sscha-1.3/SCHAModules/get_gradient_supercell_fast.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     5029 2023-02-13 14:58:18.000000 python-sscha-1.3/SCHAModules/get_odd_straight.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     4215 2023-02-13 14:58:18.000000 python-sscha-1.3/SCHAModules/get_odd_straight_with_v4.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    10186 2023-02-13 14:58:18.000000 python-sscha-1.3/SCHAModules/get_stress_tensor.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     1997 2023-02-13 14:58:18.000000 python-sscha-1.3/SCHAModules/get_upsilon_matrix.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     4044 2023-02-13 14:58:18.000000 python-sscha-1.3/SCHAModules/get_v3.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     3540 2023-02-13 14:58:18.000000 python-sscha-1.3/SCHAModules/get_v4.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     9696 2023-02-13 14:58:18.000000 python-sscha-1.3/SCHAModules/module_anharmonic.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     3172 2023-02-13 14:58:18.000000 python-sscha-1.3/SCHAModules/module_new_thermodynamic.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     8213 2023-02-13 14:58:18.000000 python-sscha-1.3/SCHAModules/module_stochastic.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     4547 2023-02-13 14:58:18.000000 python-sscha-1.3/SCHAModules/multiply_lambda_tensor.f90
-drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 10:23:25.285097 python-sscha-1.3/python_sscha.egg-info/
--rw-rw-r--   0 monacell  (1001) monacell  (1001)      227 2023-06-06 10:23:25.000000 python-sscha-1.3/python_sscha.egg-info/PKG-INFO
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     1126 2023-06-06 10:23:25.000000 python-sscha-1.3/python_sscha.egg-info/SOURCES.txt
--rw-rw-r--   0 monacell  (1001) monacell  (1001)        1 2023-06-06 10:23:25.000000 python-sscha-1.3/python_sscha.egg-info/dependency_links.txt
--rw-rw-r--   0 monacell  (1001) monacell  (1001)       18 2023-06-06 10:23:25.000000 python-sscha-1.3/python_sscha.egg-info/top_level.txt
-drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 10:23:25.297097 python-sscha-1.3/scripts/
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     3585 2023-02-13 14:58:18.000000 python-sscha-1.3/scripts/cluster_check.x
--rwxrwxr-x   0 monacell  (1001) monacell  (1001)      842 2023-02-13 14:58:18.000000 python-sscha-1.3/scripts/plot_frequencies.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     3565 2023-02-13 14:58:18.000000 python-sscha-1.3/scripts/read_incomplete_ensemble.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     4960 2023-02-13 14:58:18.000000 python-sscha-1.3/scripts/sscha
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     4715 2023-02-13 14:58:18.000000 python-sscha-1.3/scripts/sscha-plot-data.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     8052 2023-02-13 14:58:18.000000 python-sscha-1.3/scripts/static-vc-relax.pyx
--rw-rw-r--   0 monacell  (1001) monacell  (1001)       38 2023-06-06 10:23:25.297097 python-sscha-1.3/setup.cfg
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     6935 2023-06-06 10:23:07.000000 python-sscha-1.3/setup.py
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 11:29:28.528195 python-sscha-1.3.1/
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    35149 2023-02-13 14:58:18.000000 python-sscha-1.3.1/LICENSE.txt
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 11:29:28.520195 python-sscha-1.3.1/Modules/
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    10879 2023-02-13 14:58:18.000000 python-sscha-1.3.1/Modules/AdvancedCalculations.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     4823 2023-02-13 14:58:18.000000 python-sscha-1.3.1/Modules/Calculator.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    66394 2023-05-16 12:51:43.000000 python-sscha-1.3.1/Modules/Cluster.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    10288 2023-02-13 14:58:18.000000 python-sscha-1.3.1/Modules/Dynamical.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)   139737 2023-06-06 11:28:53.000000 python-sscha-1.3.1/Modules/Ensemble.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    15683 2023-02-13 14:58:18.000000 python-sscha-1.3.1/Modules/Minimizer.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    15751 2023-02-13 14:58:18.000000 python-sscha-1.3.1/Modules/Optimizer.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1173 2023-02-13 14:58:18.000000 python-sscha-1.3.1/Modules/Parallel.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    33103 2023-06-06 11:28:53.000000 python-sscha-1.3.1/Modules/Relax.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    82564 2023-06-06 11:28:53.000000 python-sscha-1.3.1/Modules/SchaMinimizer.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    18362 2023-02-13 14:58:18.000000 python-sscha-1.3.1/Modules/Tools.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    24140 2023-02-13 14:58:18.000000 python-sscha-1.3.1/Modules/Utilities.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)       80 2023-02-13 14:58:18.000000 python-sscha-1.3.1/Modules/__init__.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      229 2023-06-06 11:29:28.528195 python-sscha-1.3.1/PKG-INFO
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     8066 2023-05-16 12:51:43.000000 python-sscha-1.3.1/README.md
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 11:29:28.524195 python-sscha-1.3.1/SCHAModules/
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      870 2023-02-13 14:58:18.000000 python-sscha-1.3.1/SCHAModules/cell_force.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     3354 2023-02-13 14:58:18.000000 python-sscha-1.3.1/SCHAModules/get_cmat.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1442 2023-02-13 14:58:18.000000 python-sscha-1.3.1/SCHAModules/get_emat.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1333 2023-02-13 14:58:18.000000 python-sscha-1.3.1/SCHAModules/get_g.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    17136 2023-06-06 11:28:53.000000 python-sscha-1.3.1/SCHAModules/get_gradient_supercell.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    14175 2023-02-13 14:58:18.000000 python-sscha-1.3.1/SCHAModules/get_gradient_supercell_fast.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     5029 2023-02-13 14:58:18.000000 python-sscha-1.3.1/SCHAModules/get_odd_straight.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     4215 2023-02-13 14:58:18.000000 python-sscha-1.3.1/SCHAModules/get_odd_straight_with_v4.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    10186 2023-02-13 14:58:18.000000 python-sscha-1.3.1/SCHAModules/get_stress_tensor.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1997 2023-02-13 14:58:18.000000 python-sscha-1.3.1/SCHAModules/get_upsilon_matrix.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     4044 2023-02-13 14:58:18.000000 python-sscha-1.3.1/SCHAModules/get_v3.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     3540 2023-02-13 14:58:18.000000 python-sscha-1.3.1/SCHAModules/get_v4.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     9696 2023-02-13 14:58:18.000000 python-sscha-1.3.1/SCHAModules/module_anharmonic.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     3172 2023-02-13 14:58:18.000000 python-sscha-1.3.1/SCHAModules/module_new_thermodynamic.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     8213 2023-02-13 14:58:18.000000 python-sscha-1.3.1/SCHAModules/module_stochastic.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     4547 2023-02-13 14:58:18.000000 python-sscha-1.3.1/SCHAModules/multiply_lambda_tensor.f90
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 11:29:28.528195 python-sscha-1.3.1/python_sscha.egg-info/
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      229 2023-06-06 11:29:28.000000 python-sscha-1.3.1/python_sscha.egg-info/PKG-INFO
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1126 2023-06-06 11:29:28.000000 python-sscha-1.3.1/python_sscha.egg-info/SOURCES.txt
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)        1 2023-06-06 11:29:28.000000 python-sscha-1.3.1/python_sscha.egg-info/dependency_links.txt
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)       18 2023-06-06 11:29:28.000000 python-sscha-1.3.1/python_sscha.egg-info/top_level.txt
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 11:29:28.528195 python-sscha-1.3.1/scripts/
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     3585 2023-02-13 14:58:18.000000 python-sscha-1.3.1/scripts/cluster_check.x
+-rwxrwxr-x   0 monacell  (1001) monacell  (1001)      842 2023-02-13 14:58:18.000000 python-sscha-1.3.1/scripts/plot_frequencies.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     3565 2023-02-13 14:58:18.000000 python-sscha-1.3.1/scripts/read_incomplete_ensemble.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     4960 2023-02-13 14:58:18.000000 python-sscha-1.3.1/scripts/sscha
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     4715 2023-02-13 14:58:18.000000 python-sscha-1.3.1/scripts/sscha-plot-data.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     8052 2023-02-13 14:58:18.000000 python-sscha-1.3.1/scripts/static-vc-relax.pyx
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)       38 2023-06-06 11:29:28.528195 python-sscha-1.3.1/setup.cfg
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     6938 2023-06-06 11:29:12.000000 python-sscha-1.3.1/setup.py
```

### Comparing `python-sscha-1.3/LICENSE.txt` & `python-sscha-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/Modules/AdvancedCalculations.py` & `python-sscha-1.3.1/Modules/AdvancedCalculations.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/Modules/Calculator.py` & `python-sscha-1.3.1/Modules/Calculator.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/Modules/Cluster.py` & `python-sscha-1.3.1/Modules/Cluster.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/Modules/Dynamical.py` & `python-sscha-1.3.1/Modules/Dynamical.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/Modules/Ensemble.py` & `python-sscha-1.3.1/Modules/Ensemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -330,15 +330,16 @@
             raise NotImplementedError("Error, I do not know anything about this conversion")
 
 
         # Update the units flag
         self.units = new_units
 
 
-    def load(self, data_dir, population, N, verbose = False, load_displacements = True, raise_error_on_not_found = False, load_noncomputed_ensemble = False):
+    def load(self, data_dir, population, N, verbose = False, load_displacements = True, raise_error_on_not_found = False, load_noncomputed_ensemble = False,
+             timer=None):
         """
         LOAD THE ENSEMBLE
         =================
 
         This function load the ensemble from a standard calculation.
 
         The files need to be organized as follows
@@ -411,63 +412,70 @@
         self.sscha_forces = np.zeros( (self.N, Nat_sc, 3), order = "F", dtype = np.float64)
 
         self.u_disps = np.zeros( (self.N, Nat_sc * 3), order = "F", dtype = np.float64)
 
         # Initialize the computation of energy and forces
         self.force_computed = np.zeros( self.N, dtype = bool)
         self.stress_computed = np.zeros(self.N, dtype = bool)
+        self.all_properties = [None] * self.N
 
         # Add a counter to check if all the stress tensors are present
         count_stress = 0
 
         # Superstructure
-        dyn_supercell = self.dyn_0.GenerateSupercellDyn(self.supercell)
-        super_structure = dyn_supercell.structure
-        super_fc = np.real(dyn_supercell.dynmats[0])
+        #dyn_supercell = self.dyn_0.GenerateSupercellDyn(self.supercell)
+        super_structure = self.dyn_0.structure.generate_supercell(self.supercell)
+        #super_fc = np.real(dyn_supercell.dynmats[0])
 
         self.structures = []
 
         total_t_for_loading = 0
         total_t_for_sscha_ef = 0
         t_before_for = time.time()
         for i in range(self.N):
             # Load the structure
             structure = CC.Structure.Structure()
             if os.path.exists(os.path.join(data_dir, "scf_population%d_%d.dat" % (population, i+1))) and not load_displacements:
-                t1 = time.time()
-                structure.read_scf(os.path.join(data_dir, "scf_population%d_%d.dat" % (population, i+1)), alat = self.dyn_0.alat)
-                t2 = time.time()
-                total_t_for_loading += t2 - t1
+                if timer:
+                    timer.execute_timed_function(structure.read_scf, os.path.join(data_dir, "scf_population%d_%d.dat" % (population, i+1)), alat = self.dyn_0.alat)
+                else:
+                    structure.read_scf(os.path.join(data_dir, "scf_population%d_%d.dat" % (population, i+1)), alat = self.dyn_0.alat)
 
                 structure.has_unit_cell = True
                 structure.unit_cell = super_structure.unit_cell
 
                 # Get the displacement [ANGSTROM]
-                self.u_disps[i,:] = structure.get_displacement(super_structure).reshape( 3 * Nat_sc)
+                if timer:
+                    self.u_disps[i,:] = timer.execute_timed_function(structure.get_displacement, super_structure).ravel()
+                else:
+                    self.u_disps[i,:] = structure.get_displacement(super_structure).ravel()
 
             else:
                 structure = super_structure.copy()
-                t1 = time.time()
-                disp =np.loadtxt(os.path.join(data_dir, "u_population%d_%d.dat" % (population, i+1))) /__A_TO_BOHR__
-                t2 = time.time()
-                total_t_for_loading += t2 - t1
+                if timer:
+                    disp = timer.execute_timed_function(np.loadtxt, os.path.join(data_dir, "u_population%d_%d.dat" % (population, i+1))) / A_TO_BOHR
+                else:
+                    disp =np.loadtxt(os.path.join(data_dir, "u_population%d_%d.dat" % (population, i+1))) /__A_TO_BOHR__
 
                 structure.coords += disp
                 self.u_disps[i, :] = disp.ravel()
 
             self.xats[i, :, :] = structure.coords
             self.structures.append(structure)
 
 
             # Load forces (Forces are in Ry/bohr, convert them in Ry /A)
             t1 = time.time()
             force_path = os.path.join(data_dir, "forces_population%d_%d.dat" % (population, i+1))
 
             if os.path.exists(force_path):
-                self.forces[i,:,:] = np.loadtxt(force_path) * A_TO_BOHR
+                if timer:
+                    self.forces[i,:,:] = timer.execute_timed_function(np.loadtxt, force_path) * A_TO_BOHR
+                else:
+                    self.forces[i,:,:] = np.loadtxt(force_path) * A_TO_BOHR
                 self.force_computed[i] = True
             else:
                 if raise_error_on_not_found:
                     ERROR_MSG = """
 Error, the file '{}' is missing from the ensemble
        data_dir = '{}'
        please, check better your data.
@@ -475,20 +483,22 @@
                     print(ERROR_MSG)
                     raise IOError(ERROR_MSG)
                 else:
                     self.force_computed[i] = False
 
             # Load stress
             if os.path.exists(os.path.join(data_dir, "pressures_population%d_%d.dat" % (population, i+1))):
-                self.stresses[i,:,:] =  np.loadtxt(os.path.join(data_dir, "pressures_population%d_%d.dat" % (population, i+1)))
+                if timer:
+                    self.stresses[i,:,:] =  timer.execute_timed_function(np.loadtxt, os.path.join(data_dir, "pressures_population%d_%d.dat" % (population, i+1)))
+                else:
+                    self.stresses[i,:,:] =  np.loadtxt(os.path.join(data_dir, "pressures_population%d_%d.dat" % (population, i+1)))
                 self.stress_computed[i] = True
             else:
                 self.stress_computed[i] = False
             t2 = time.time()
-            total_t_for_loading += t2 - t1
 
 
 
 #            print "Loading: config %d:" % i
 #            for j in range(structure.N_atoms):
 #                print "Atom %d" % j
 #                print "u_disp = ", structure.get_displacement(self.dyn_0.structure)[j,:]  *A_TO_BOHR
@@ -504,38 +514,36 @@
 
 
         if verbose:
             print( "[LOAD ENSEMBLE]: time elapsed for the cycle over the configurations:", time.time() - t_before_for)
 
         t1 = time.time()
         # Load the energy
-        total_energies = np.loadtxt(os.path.join(data_dir, "energies_supercell_population%d.dat" % (population)))
-        t2 = time.time()
-        total_t_for_sscha_ef += t2 - t1
+        if timer:
+            total_energies = timer.execute_timed_function(np.loadtxt, os.path.join(data_dir, "energies_supercell_population%d.dat" % (population)))
+        else:
+            total_energies = np.loadtxt(os.path.join(data_dir, "energies_supercell_population%d.dat" % (population)))
         self.energies = total_energies[:N]
 
         # Compute the SSCHA energies and forces
-        self.sscha_energies[:], self.sscha_forces[:,:,:] = self.dyn_0.GenerateSupercellDyn(self.supercell).get_energy_forces(None, displacement = self.u_disps)
+        if timer:
+            self.sscha_energies[:], self.sscha_forces[:,:,:] = timer.execute_timed_function(self.dyn_0.get_energy_forces, None, displacement = self.u_disps)
+        else:
+            self.sscha_energies[:], self.sscha_forces[:,:,:] = self.dyn_0.get_energy_forces(None, displacement = self.u_disps)
 
 
         # Setup the initial weight
         self.rho = np.ones(self.N, dtype = np.float64)
 
         # Initialize the q_start
 
         t1 = time.time()
-        self.q_start = CC.Manipulate.GetQ_vectors(self.structures, dyn_supercell, self.u_disps)
+        #self.q_start = CC.Manipulate.GetQ_vectors(self.structures, dyn_supercell, self.u_disps)
         t2 = time.time()
-        self.current_q = self.q_start.copy()
-
-        if verbose:
-            print( "[LOAD ENSEMBLE]: time elapsed to compute the current q vectors:", t2 - t1)
-            print( "[LOAD ENSEMBLE]: time elapsed while loading with numpy:", total_t_for_loading)
-            print( "[LOAD ENSEMBLE]: time elapsed for computing sscha energy and forces:", total_t_for_sscha_ef)
-
+        #self.current_q = self.q_start.copy()
 
         p_count = np.sum(self.stress_computed.astype(int))
         if p_count > 0:
             self.has_stress = True
         else:
             self.has_stress = False
 
@@ -1338,15 +1346,15 @@
         self.energies = energies_new
         self.forces = forces_new
         self.sscha_energies = sscha_energies_new
         self.sscha_forces = sscha_forces_new
 
 
 
-    def update_weights(self, new_dynamical_matrix, newT, update_q = False):
+    def update_weights(self, new_dynamical_matrix, newT, update_q = False, timer=None):
         """
         IMPORTANCE SAMPLING
         ===================
 
 
         This function updates the importance sampling for the given dynamical matrix.
         The result is written in the self.rho variable
@@ -1377,25 +1385,32 @@
         old_disps = np.zeros(np.shape(self.u_disps), dtype = np.double)
         Nat_sc = super_structure.N_atoms
 
         self.u_disps[:,:] = self.xats.reshape((self.N, 3*Nat_sc)) - np.tile(super_structure.coords.ravel(), (self.N,1))
         old_disps[:,:] = self.xats.reshape((self.N, 3*Nat_sc)) - np.tile(super_struct0.coords.ravel(), (self.N,1))
 
         if changed_dyn:
-            w_new, pols = new_dynamical_matrix.DiagonalizeSupercell()#new_super_dyn.DyagDinQ(0)
+            if timer:
+                w_new, pols = timer.execute_timed_function(new_dynamical_matrix.DiagonalizeSupercell)
+            else:
+                w_new, pols = new_dynamical_matrix.DiagonalizeSupercell()#new_super_dyn.DyagDinQ(0)
             self.current_w = w_new.copy()
             self.current_pols = pols.copy()
         else:
             w_new = self.current_w.copy()
             pols  = self.current_pols.copy()
             #w_new, pols = new_dynamical_matrix.DiagonalizeSupercell()#new_super_dyn.DyagDinQ(0)
             #self.current_w = w_new.copy()
             #self.current_pols = pols.copy()
         # Update sscha energies and forces
-        self.sscha_energies[:], self.sscha_forces[:,:,:] = new_dynamical_matrix.get_energy_forces(None, displacement = self.u_disps, w_pols = (w_new, pols))
+        if timer:
+            self.sscha_energies[:], self.sscha_forces[:,:,:] = timer.execute_timed_function(new_dynamical_matrix.get_energy_forces,
+                                                                                            None, displacement = self.u_disps, w_pols = (w_new, pols))
+        else:
+            self.sscha_energies[:], self.sscha_forces[:,:,:] = new_dynamical_matrix.get_energy_forces(None, displacement = self.u_disps, w_pols = (w_new, pols))
 
 
         t1 = time.time()
         # Get the frequencies of the original dynamical matrix
         #super_dyn = self.dyn_0.GenerateSupercellDyn(self.supercell)
 
         w_original = self.w_0.copy()
@@ -1451,23 +1466,24 @@
 
         w= w_new[~trans_mask]
         w = np.array(w/2, dtype = np.float64)
         new_a = SCHAModules.thermodynamic.w_to_a(w, newT)
 
 
         # Get the new displacements in the supercell
-        t3 = time.time()
+        t2 = time.time()
+        if timer:
+            timer.add_timer("update preparation", t2-t1)
         # for i in range(self.N):
         #     self.u_disps[i, :] = (self.xats[i, :, :] - super_structure.coords).reshape( 3*Nat_sc )
 
         #     old_disps[i,:] = (self.xats[i, :, :] - super_dyn.structure.coords).reshape( 3*Nat_sc )
 
         #     # TODO: this method recomputes the displacements, it is useless since we already have them in self.u_disps
 
-        t4 = time.time()
 
 
         # Convert the q vectors in the Hartree units
         #old_q = self.q_start * np.sqrt(np.float64(2)) * __A_TO_BOHR__
         #new_q = self.current_q * np.sqrt(np.float64(2)) * __A_TO_BOHR__
 
 
@@ -1479,30 +1495,31 @@
             print( " ==== [UPDATE RHO DEBUGGING] ==== ")
             print( " INPUT INFO: ")
             np.savetxt("rho_%05d.dat" % self.__debug_index__, self.rho)
             print( " rho saved in ", "rho_%05d.dat" % self.__debug_index__)
 
 
         # Get the covariance matrices of the ensemble
-        ups_new = np.real(new_dynamical_matrix.GetUpsilonMatrix(self.current_T, w_pols = (w_new, pols)))
-        ups_old = np.real(self.dyn_0.GetUpsilonMatrix(self.T0, w_pols = (w_original, pols_original)))
+        if timer:
+            ups_new = np.real(timer.execute_timed_function(new_dynamical_matrix.GetUpsilonMatrix, self.current_T, w_pols = (w_new, pols)))
+            ups_old = np.real(timer.execute_timed_function(self.dyn_0.GetUpsilonMatrix, self.T0, w_pols = (w_original, pols_original)))
+        else:
+            ups_new = np.real(new_dynamical_matrix.GetUpsilonMatrix(self.current_T, w_pols = (w_new, pols)))
+            ups_old = np.real(self.dyn_0.GetUpsilonMatrix(self.T0, w_pols = (w_original, pols_original)))
 
         # Get the normalization ratio
         #norm = np.sqrt(np.abs(np.linalg.det(ups_new) / np.linalg.det(ups_old)))
         norm = np.prod( old_a / new_a)
 
         t2 = time.time()
-        print( "Time elapsed to prepare the rho update:", t2 - t1, "s")
-        print (" (of which to diagonalize and prepare the structure: %.4f s)" % (t3-t1))
-        print ( "(of which to update sscha energies and forces: %.4f s)" % (t4-t3))
-        print ( "(of which computing the Upsilon matrix: %.4f s)" % (t2 - t4))
 
         rho_tmp = np.ones( self.N, dtype = np.float64) * norm
         if __DEBUG_RHO__:
             print("Norm factor:", norm)
+
         for i in range(self.N):
             v_new = self.u_disps[i, :].dot(ups_new.dot(self.u_disps[i, :])) * __A_TO_BOHR__**2
             v_old = old_disps[i, :].dot(ups_old.dot(old_disps[i, :])) * __A_TO_BOHR__**2
 
             if __DEBUG_RHO__:
                 print("CONF {} | displacement = {}".format(i, v_new - v_old))
             rho_tmp[i] *= np.exp(-0.5 * (v_new - v_old) )
@@ -1520,19 +1537,20 @@
         #print "RHO:", self.rho
 
         #for i in range(self.N):
             # Get the new displacement
             #self.u_disps[i, :] = self.structures[i].get_displacement(new_super_dyn.structure).reshape(3 * new_super_dyn.structure.N_atoms)
             #self.u_disps[i, :] = (self.xats[i, :, :] - super_structure.coords).reshape( 3*Nat_sc )
         t1 = time.time()
+        if timer:
+            timer.add_timer("<u| Y |u> and weights update (TODO: parallelizable)", t1-t2)
+            self.current_dyn = timer.execute_timed_function(new_dynamical_matrix.Copy)
         #print( "Time elapsed to update weights the sscha energies, forces and displacements:", t1 - t3, "s")
-        print( "(of which to update the weights):", t1 - t2, "s")
-        self.current_dyn = new_dynamical_matrix.Copy()
-        t2 = time.time()
-        print(" | to copy the dynamical matrix: {} s".format(t2-t1))
+        else:
+            self.current_dyn = new_dynamical_matrix.Copy()
 
 
         if __DEBUG_RHO__:
             new_dynamical_matrix.save_qe("ud_%05d" % self.__debug_index__)
             print( " new_dynmat saved in ud_%05d " % self.__debug_index__)
             print( " new_T : ", newT)
             print( " old_T : ", self.T0)
@@ -1874,30 +1892,78 @@
             delta_new_phi = (delta_new_phi + np.transpose(delta_new_phi)) * .5
             delta_new_phi -= new_phi**2
             delta_new_phi = np.sqrt(delta_new_phi)
             return new_phi, delta_new_phi
 
         return new_phi
 
+    def get_preconditioned_gradient_parallel(self, *args, timer=None, **kwargs):
+        """
+        Compute the gradient using multiprocessing.
+        For documentation, see get_preconditioned_gradient
+        """
+
+        print("force length:", len(self.force_computed))
+
+        def work_function(argument, timer=None):
+            print("force length [inside]:", len(self.force_computed))
+            ensemble_start_config, ensemble_end_config = argument
+            mask = np.zeros(self.N, dtype = bool)
+            mask[ensemble_start_config : ensemble_end_config] = True
+            print("mask length:", np.sum(mask.astype(int))," total N:", len(mask))
+            new_ensemble = self.split(mask)
+
+            gradient, _ = new_ensemble.get_preconditioned_gradient(*args, timer=timer, **kwargs)
+
+            av_ensemble = np.sum(new_ensemble.rho)
+            
+            return gradient * av_ensemble
+
+        nproc = CC.Settings.GetNProc()
+        list_of_inputs = []
+        index = 0
+        for i in range(nproc):
+            start_config = index
+            index += self.N // nproc
+            if i < self.N % nproc:
+                index += 1
+            end_config = index
+            
+            list_of_inputs.append( (start_config, end_config) )
+
+        if timer:
+            gradient = timer.execute_timed_function(CC.Settings.GoParallel, work_function, list_of_inputs, "+")
+        else:
+            gradient = CC.Settings.GoParallel(work_function, list_of_inputs, "+")
+
+        gradient /= np.sum(self.rho)
+
+        return gradient, np.zeros_like(gradient) + 1
+
+        
+
+        
+    
+
     def get_preconditioned_gradient(self, subtract_sscha = True, return_error = False,
                                     use_ups_supercell = True, preconditioned = 1,
-                                    fast_grad = False, verbose = True):
+                                    fast_grad = False, verbose = True, timer=None):
         """
         SELF CONSISTENT SCHA EQUATION
         =============================
 
         This function evaluate the self consistent scha equation. This can be used
         to evaluate the goodness of the minimization procedure, as well as an
         independent minimizer. This is the same as get_fc_from_self_consistency,
         but works also with supercell
 
 
         .. math::
 
-            \\Phi_{ab} = \\sum_c \\upsilon_{ac} \\left< u_c f_a\\right>_{\\Phi}
+            \\Phi_{ab} = \\sum_c \\Upsilon_{ac} \\left< u_c f_a\\right>_{\\Phi}
 
         The previous equation is true only if the :math:`\\Phi` matrix is the solution
         of the SCHA theory. Here :math:`\\vec u` are the displacements of the configurations
         and :math:`f` are the forces of the real system acting on the simulation.
 
         NOTE: It does not takes into account for the symmetrization.
 
@@ -1922,20 +1988,22 @@
         Results
         -------
             fc : ndarray (nq x 3*nat x 3*nat)
                 The real space force constant matrix obtained by the
                 self-consistent equation.
         """
 
-        t1 = time.time()
         super_struct = self.current_dyn.structure.generate_supercell(self.supercell)
         #supercell_dyn = self.current_dyn.GenerateSupercellDyn(self.supercell)
         
         # Dyagonalize
-        w, pols = self.current_dyn.DiagonalizeSupercell()#supercell_dyn.DyagDinQ(0)
+        if timer:
+            w, pols = timer.execute_timed_function(self.current_dyn.DiagonalizeSupercell)
+        else:
+            w, pols = self.current_dyn.DiagonalizeSupercell()#supercell_dyn.DyagDinQ(0)
 
         if not self.ignore_small_w:
             trans = CC.Methods.get_translations(pols, super_struct.get_masses_array())
         else:
             trans = np.abs(w) < CC.Phonons.__EPSILON_W__
 
         ityp = super_struct.get_ityp() + 1 # Py to fortran convertion
@@ -1945,80 +2013,106 @@
 
         mass *= 2
         w /= 2
 
         nat = super_struct.N_atoms
         eforces = np.zeros((self.N, nat, 3), dtype = np.float64, order = "F")
         u_disp = np.zeros((self.N, nat, 3), dtype = np.float64, order = "F")
+
+        t1 = time.time()
         #print nat
         if subtract_sscha:
             eforces[:,:,:] = self.forces - self.sscha_forces
         else:
             eforces[:,:,:] = self.forces
         for i in range(self.N):
             u_disp[i, :, :] = np.reshape(self.u_disps[i,:], (nat, 3))
 
 
         # TODO: This may be dangerous
         pols = np.real(pols)
 
         t2 = time.time()
-        if verbose:
-            print( " [GRADIENT] Time to prepare the gradient calculation:", t2 -t1,"s")
+        if timer:
+            timer.add_timer("Preparation of the gradient", t2 - t1)
 
 
-        t1 = time.time()
         if fast_grad or not preconditioned:
-            grad, grad_err = SCHAModules.get_gradient_supercell(self.rho, u_disp, eforces, w, pols, trans,
+            if timer:
+                grad, grad_err = timer.execute_timed_function(SCHAModules.get_gradient_supercell, 
+                                                              self.rho, u_disp, eforces, w, pols, trans,
+                                                              self.current_T, mass, ityp, log_err, self.N,
+                                                              nat, 3*nat, len(mass), preconditioned,
+                                                              override_name = "get_gradient_supercell")
+            else:
+                grad, grad_err = SCHAModules.get_gradient_supercell(self.rho, u_disp, eforces, w, pols, trans,
                                                                 self.current_T, mass, ityp, log_err, self.N,
                                                                 nat, 3*nat, len(mass), preconditioned)
         else:
-            grad, grad_err = SCHAModules.get_gradient_supercell_new(self.rho, u_disp, eforces, w, pols, trans,
+            if timer:
+                grad, grad_err = timer.execute_timed_function(SCHAModules.get_gradient_supercell_new,
+                                                              self.rho, u_disp, eforces, w, pols, trans,
+                                                                     self.current_T, mass, ityp, log_err, self.N,
+                                                                     nat, 3*nat, len(mass),
+                                                                     override_name = "get_gradient_supercell_new")
+            else:
+                grad, grad_err = SCHAModules.get_gradient_supercell_new(self.rho, u_disp, eforces, w, pols, trans,
                                                                      self.current_T, mass, ityp, log_err, self.N,
                                                                      nat, 3*nat, len(mass))
 
 
-        t2 = time.time()
-        if verbose:
-            print (" [GRADIENT] Time to call the fortran code:", t2 - t1, "s")
-
         # If we are at gamma, we can skip this part
         # Which makes the code faster
         if np.prod(self.dyn_0.GetSupercell()) > 1:
 
             # Perform the fourier transform
             if return_error:
                 # Check if a multiprocessing function can be exploited
                 if hasattr(CC.Phonons, 'GetDynQFromFCSupercell_parallel') and CC.Settings.GetNProc() > 1:  
-                    q_grad,q_grad_err = CC.Phonons.GetDynQFromFCSupercell_parallel(grad, np.array(self.current_dyn.q_tot),
+                    if timer:
+                        q_grad,q_grad_err = timer.execute_timed_function(CC.Phonons.GetDynQFromFCSupercell_parallel,
+                                                                         grad, np.array(self.current_dyn.q_tot),
+                                                        self.current_dyn.structure, super_struct,fc2=grad_err)
+                    else:
+                        q_grad,q_grad_err = CC.Phonons.GetDynQFromFCSupercell_parallel(grad, np.array(self.current_dyn.q_tot),
                                                         self.current_dyn.structure, super_struct,fc2=grad_err)
                 else:
-                    q_grad,q_grad_err = CC.Phonons.GetDynQFromFCSupercell(grad, np.array(self.current_dyn.q_tot),
+                    if timer:
+                        q_grad,q_grad_err = timer.execute_timed_function(CC.Phonons.GetDynQFromFCSupercell,
+                                                                         grad, np.array(self.current_dyn.q_tot),
+                                                        self.current_dyn.structure, super_struct,fc2=grad_err)
+                    else:
+                        q_grad,q_grad_err = CC.Phonons.GetDynQFromFCSupercell(grad, np.array(self.current_dyn.q_tot),
                                                         self.current_dyn.structure, super_struct,fc2=grad_err)
             else:
                 if hasattr(CC.Phonons, 'GetDynQFromFCSupercell_parallel'):
-                    q_grad = CC.Phonons.GetDynQFromFCSupercell_parallel(grad, np.array(self.current_dyn.q_tot),
+                    if timer:
+                        q_grad = timer.execute_timed_function(CC.Phonons.GetDynQFromFCSupercell_parallel,
+                                                              grad, np.array(self.current_dyn.q_tot),
+                                                        self.current_dyn.structure, super_struct)
+                    else:
+                        q_grad = CC.Phonons.GetDynQFromFCSupercell_parallel(grad, np.array(self.current_dyn.q_tot),
                                                         self.current_dyn.structure, super_struct)
                 else:
-                    q_grad = CC.Phonons.GetDynQFromFCSupercell(grad, np.array(self.current_dyn.q_tot),
+                    if timer:
+                        q_grad = timer.execute_timed_function(CC.Phonons.GetDynQFromFCSupercell, 
+                                                              grad, np.array(self.current_dyn.q_tot),
+                                                        self.current_dyn.structure, super_struct)
+                    else:
+                        q_grad = CC.Phonons.GetDynQFromFCSupercell(grad, np.array(self.current_dyn.q_tot),
                                                         self.current_dyn.structure, super_struct)
             #q_grad_err = CC.Phonons.GetDynQFromFCSupercell(grad_err, np.array(self.current_dyn.q_tot),
              #                                           self.current_dyn.structure, supercell_dyn.structure)
         else:
             nat3, _ = grad.shape
             q_grad = np.zeros( (1, nat3, nat3), dtype = np.double)
             q_grad_err = np.zeros_like(q_grad)
             q_grad[0, :, :] = grad
             q_grad_err[0, :, :] = grad_err
 
-        t1 = time.time()
-        if verbose:
-            print (" [GRADIENT] Time to get back in fourier space:", t1 - t2, "s")
-
-
         if return_error:
             return q_grad, q_grad_err
         else:
             return q_grad
 
 #
 #        nat = self.current_dyn.structure.N_atoms
@@ -2104,15 +2198,15 @@
 
         # A C style matrix of double precision real values
         cov_mat = np.einsum("i, ij, ik", self.rho, self.u_disps, self.u_disps) / np.sum(self.rho)
 
         return cov_mat
 
 
-    def get_stress_tensor(self, offset_stress = None, add_centroid_contrib = False, use_spglib = False):
+    def get_stress_tensor(self, offset_stress = None, use_spglib = False):
 
         """
         GET STRESS TENSOR
         =================
 
         The following subroutine computes the anharmonic stress tensor
         calling the fortran code get_stress_tensor.
@@ -2121,17 +2215,14 @@
         NOTE: unit of measure is Ry/bohr^3 to match the quantum espresso one
 
         Parameters
         ----------
             offset_stress : 3x3 matrix, optional
                 An offset stress to be subtracted to the real stress tensor.
                 Usefull if you want to compute just the anharmonic contribution.
-            add_centroid_contrib : bool, optional
-                If true the contribution of the centroid is added. This is always zero when
-                the system is relaxed.
             use_spglib : bool
                 If true use the spglib library to perform the symmetrization
 
 
         Results
         -------
             stress_tensor : 3x3 matrix
@@ -2142,29 +2233,30 @@
         """
 
         if not self.has_stress:
             raise ValueError("Error, the stress tensors are not present in the current ensemble.")
 
 
         # Get frequencies and polarization vectors
-        super_dyn = self.current_dyn.GenerateSupercellDyn(self.supercell)
-        wr, pols = super_dyn.DyagDinQ(0)
+        super_structure = self.current_dyn.structure.generate_supercell(self.supercell)
+        #super_dyn = self.current_dyn.GenerateSupercellDyn(self.supercell)
+        wr, pols = self.current_dyn.DiagonalizeSupercell()
 
         if not self.ignore_small_w:
-            trans = ~ CC.Methods.get_translations(pols, super_dyn.structure.get_masses_array())
+            trans = ~ CC.Methods.get_translations(pols, super_structure.get_masses_array())
         else:
             trans = np.abs(wr) > CC.Phonons.__EPSILON_W__
 
         wr = np.real( wr[trans])
         pols = np.real( pols[:, trans])
 
-        nat = super_dyn.structure.N_atoms
+        nat = super_structure.N_atoms
 
         # Volume bohr^3
-        volume = super_dyn.structure.get_volume() * __A_TO_BOHR__**3
+        volume = super_structure.get_volume() * __A_TO_BOHR__**3
 
 
         # Get the correctly shaped polarization vectors
         er = np.zeros( (nat, len(wr), 3), dtype = np.float64, order = "F")
 
         for i in range(len(wr)):
             for j in range(nat):
@@ -2180,58 +2272,47 @@
         abinit_stress = np.einsum("abc -> cba", self.stresses, order = "F")
 
         stress, err_stress = SCHAModules.get_stress_tensor(volume, self.forces / __A_TO_BOHR__, u_disps * __A_TO_BOHR__,
                                                            abinit_stress, wr, er, self.current_T, self.rho, "err_yesrho",
                                                            self.N, nat, len(wr))
 
         # Correct the stress adding the centroid contribution
-        if add_centroid_contrib:
+        # if add_centroid_contrib:
+
+        #     eforces = self.forces - self.sscha_forces
 
-            eforces = self.forces - self.sscha_forces
+        #     if not np.prod(self.supercell) == 1:
+        #         # Refold the forces in the unit cell
+        #         itau = super_structure.get_itau(self.current_dyn.structure) - 1 # Fort -> Py
+        #         nat = self.dyn_0.structure.N_atoms
+        #         new_forces = np.zeros((self.N, nat, 3), dtype  =np.float64, order = "C")
+
+        #         # Project in the unit cell the forces
+        #         for i in range(nat):
+        #             #print "%d) ITAU LIST:" % i, itau == i
+        #             new_forces[:, i, :] = np.sum(eforces[:, itau==i,:], axis = 1) / np.prod(self.supercell)
+        #             #new_forces[:, i, :] =
+
+        #         eforces = new_forces
+
+        #     stress_centr = np.zeros( (3,3), dtype = np.float64)
+        #     error_centr = np.zeros( (3,3), dtype = np.float64)
+        #     for i in range(0, 3):
+        #         for j in range(i, 3):
+        #             av_array = 0.5 * np.einsum("h, ah", self.current_dyn.structure.coords[:, i],
+        #                                        eforces[:,:,j])
+        #             av_array += 0.5 * np.einsum("h, ah", self.current_dyn.structure.coords[:, j],
+        #                                         eforces[:,:,i])
+        #             stress_centr[i,j], error_centr[i,j] = SCHAModules.stochastic.average_error_weight(av_array, self.rho, "err_yesrho")
+        #             stress_centr[j,i] = stress_centr[i,j]
+        #             error_centr[j,i] = error_centr[i,j]
 
-            if not np.prod(self.supercell) == 1:
-                # Refold the forces in the unit cell
-                super_structure = self.current_dyn.structure.generate_supercell(self.supercell)
-                itau = super_structure.get_itau(self.current_dyn.structure) - 1 # Fort -> Py
-                nat = self.dyn_0.structure.N_atoms
-                new_forces = np.zeros((self.N, nat, 3), dtype  =np.float64, order = "C")
-
-                # Project in the unit cell the forces
-                for i in range(nat):
-                    #print "%d) ITAU LIST:" % i, itau == i
-                    new_forces[:, i, :] = np.sum(eforces[:, itau==i,:], axis = 1) / np.prod(self.supercell)
-                    #new_forces[:, i, :] =
-
-                eforces = new_forces
-
-            stress_centr = np.zeros( (3,3), dtype = np.float64)
-            error_centr = np.zeros( (3,3), dtype = np.float64)
-            for i in range(0, 3):
-                for j in range(i, 3):
-                    av_array = 0.5 * np.einsum("h, ah", self.current_dyn.structure.coords[:, i],
-                                               eforces[:,:,j])
-                    av_array += 0.5 * np.einsum("h, ah", self.current_dyn.structure.coords[:, j],
-                                                eforces[:,:,i])
-                    stress_centr[i,j], error_centr[i,j] = SCHAModules.stochastic.average_error_weight(av_array, self.rho, "err_yesrho")
-                    stress_centr[j,i] = stress_centr[i,j]
-                    error_centr[j,i] = error_centr[i,j]
-
-
-#            f, err_f = self.get_average_forces(True)
-#            stress_centroid = 0.5 * np.einsum( "ai,aj", self.current_dyn.structure.coords * __A_TO_BOHR__, f) / volume
-#            stress_centroid += np.transpose(stress_centroid)
-#            err_stress_centroid = np.einsum( "ai,aj", self.current_dyn.structure.coords**2 , err_f**2)
-#            err_stress_centroid = np.sqrt(err_stress_centroid) * __A_TO_BOHR__ / volume
-#            err_stress_centroid = np.sqrt( err_stress_centroid**2 + np.transpose(err_stress_centroid**2))
-#            divideby = np.ones( (3,3)) * 2
-#            divideby[np.eye(3) == 1] = np.sqrt(2)
-#            err_stress_centroid /= divideby
 
-            stress += stress_centr
-            err_stress = np.sqrt(err_stress**2 + error_centr**2)
+        #   stress += stress_centr
+        #   err_stress = np.sqrt(err_stress**2 + error_centr**2)
 
 
 
         # Check the offset
         if not offset_stress is None:
             stress -= offset_stress
 
@@ -2805,15 +2886,15 @@
 
     #     if N_w > 1:
     #         return sigmas
     #     return sigma
 
 
     def get_free_energy_hessian(self, include_v4 = False, get_full_hessian = True, verbose = False, \
-        use_symmetries = True, return_d3 = False):
+        use_symmetries = True, return_d3 = False, w_pols = None, timer=None):
         """
         GET THE FREE ENERGY ODD CORRECTION
         ==================================
 
         This subroutines computes the odd correction
         to the free energy hessian using the fortran subroutines, as describe in the
         Bianco paper ...
@@ -2832,14 +2913,16 @@
                 If true, the third order force constant tensor is written in output [Ha/bohr^3 units].
                 This can be used to interpolate the result on a bigger mesh with cellconstructor.
             use_symmetries : bool
                 If true, the d3 and d4 are symmetrized in real space.
                 It requires that spglib is installed to detect symmetries in the supercell correctly.
             return_d3 : bool
                 If true, returns also the tensor of three phonon scattering.
+            w_pols : list of ndarray
+                If provided, it avoids the diagonalization of the dynamical matrix to speedup the time.
 
         Returns
         -------
             phi_sc : Phonons()
                 The dynamical matrix of the free energy hessian in (Ry/bohr^2)
             d3 : ndarray (size = (3*nat_sc, 3*nat_sc, 3*nat_sc), Optional
                 Return the three-phonon-scattering tensor (in Ry atomic units).
@@ -2853,16 +2936,24 @@
         #         raise NotImplementedError(ERROR_MSG)
 
         # Convert anything into the Ha units
         # This is needed for the Fortran subroutines
         self.convert_units(UNITS_HARTREE)
 
         # Get the dynamical matrix in the supercell
-        dyn_supercell = self.current_dyn.GenerateSupercellDyn(self.supercell)
-        w, pols = dyn_supercell.DyagDinQ(0)
+        #dyn_supercell = self.current_dyn.GenerateSupercellDyn(self.supercell)
+        super_structure = self.current_dyn.structure.generate_supercell(self.supercell)
+        if w_pols is None:
+            if timer:
+                w, pols = timer.execute_timed_function(self.current_dyn.DiagonalizeSupercell)
+            else:
+                w, pols = self.current_dyn.DiagonalizeSupercell()
+        else:
+            w, pols = w_pols
+
         a = SCHAModules.thermodynamic.w_to_a(w, self.current_T)
 
 
         n_modes = len(w)
         nat_sc = int(np.shape(pols)[0] / 3)
 
         # Get the polarization vectors in the correct format
@@ -2870,21 +2961,21 @@
         for i in range(nat_sc):
             for j in range(n_modes):
                 new_pol[i, j, :] = pols[3*i : 3*(i+1), j]
 
 
         # Get the translational modes
         if not self.ignore_small_w:
-            trans = CC.Methods.get_translations(pols, dyn_supercell.structure.get_masses_array())
+            trans = CC.Methods.get_translations(pols, super_structure.get_masses_array())
         else:
             trans = np.abs(w) < CC.Phonons.__EPSILON_W__
 
 
         # Get the atomic types
-        ityp = dyn_supercell.structure.get_ityp() + 1 #Py to Fortran indexing
+        ityp = super_structure.get_ityp() + 1 #Py to Fortran indexing
         n_typ = len(self.current_dyn.structure.masses)
 
         amass = np.zeros(n_typ, dtype = np.double)
 
         for at_type in self.current_dyn.structure.masses:
             index = ityp[self.current_dyn.structure.atoms.index(at_type)] - 1
             amass[index] = self.current_dyn.structure.masses[at_type]
@@ -2894,80 +2985,107 @@
         u = self.u_disps.reshape((self.N, nat_sc, 3), order = "C") #/ Bohr
 
         log_err = "err_yesrho"
 
         # Lets call the Fortran subroutine to compute the v3
         if verbose:
             print ("Going into d3")
-        d3 = SCHAModules.get_v3(a, new_pol, trans, amass, ityp,
-                                f, u, self.rho, log_err)
+        if timer:
+            d3 = timer.execute_timed_function(SCHAModules.get_v3, a, new_pol, trans, amass, ityp,
+                                    f, u, self.rho, log_err, override_name="SCHAModules.get_v3")
+        else:
+            d3 = SCHAModules.get_v3(a, new_pol, trans, amass, ityp,
+                                    f, u, self.rho, log_err)
         if verbose:
             print("Outside d3")
 
 
         # Symmetrize the d3
         if use_symmetries:
             if verbose:
                 print("Symmetrizing the d3")
                 np.save("d3_realspace_nosym.npy", d3)
-            qe_sym = CC.symmetries.QE_Symmetry(dyn_supercell.structure)
-            qe_sym.SetupFromSPGLIB()
-            qe_sym.ApplySymmetryToTensor3(d3)
+
+            qe_sym = CC.symmetries.QE_Symmetry(super_structure)
+            if timer:
+                timer.execute_timed_function(qe_sym.SetupFromSPGLIB)
+                timer.execute_timed_function(qe_sym.ApplySymmetryToTensor3, d3)
+            else:
+                qe_sym.SetupFromSPGLIB()
+                qe_sym.ApplySymmetryToTensor3(d3)
+            
 
         if verbose:
             print("Saving the third order force constants as d3_realspace_sym.npy [Ha units]")
             np.save("d3_realspace_sym.npy", d3)
 
         # Check if the v4 must be included
         if include_v4:
             print("Computing the v4, this requires some time...")
             t1 = time.time()
-            d4 = SCHAModules.get_v4(a, new_pol, trans, amass, ityp, \
-                f, u, self.rho, log_err)
+            if timer:
+                d4 = timer.execute_timed_function(SCHAModules.get_v4, a, new_pol, trans, amass, ityp, \
+                    f, u, self.rho, log_err, override_name="SCHAModules.get_v4")
+            else:
+                d4 = SCHAModules.get_v4(a, new_pol, trans, amass, ityp, \
+                    f, u, self.rho, log_err)
             t2 = time.time()
             print("Time elapsed to compute the v4: {} s".format(t2-t1))
 
             # Symmetrize the v4
             if use_symmetries:
-                qe_sym = CC.symmetries.QE_Symmetry(dyn_supercell.structure)
-                qe_sym.SetupFromSPGLIB()
-                qe_sym.ApplySymmetryToTensor4(d4)
+                if timer:
+                    timer.execute_timed_function(qe_sym.ApplySymmetryToTensor4, d4)
+                else:
+                    qe_sym.ApplySymmetryToTensor4(d4)
 
             if verbose: print("Inside odd straight")
-            phi_sc_odd = SCHAModules.get_odd_straight_with_v4(a, w, new_pol, trans, \
-                amass, ityp, self.current_T, d3, d4)
+            if timer:
+                phi_sc_odd = timer.execute_timed_function(SCHAModules.get_odd_straight_with_v4, a, w, new_pol, trans, \
+                    amass, ityp, self.current_T, d3, d4, override_name="SCHAModules.get_odd_straight_with_v4")
+            else:
+                phi_sc_odd = SCHAModules.get_odd_straight_with_v4(a, w, new_pol, trans, \
+                    amass, ityp, self.current_T, d3, d4)
             if verbose : print("Outside odd straight")
         else:
             # Only v3
             # Get the odd correction (In Ha/bohr^2)
             if verbose:
                 print ("Inside odd straight")
                 print (" A = ", a)
                 print (" W = ", w)
                 print (" TRANS = ", trans)
                 print (" AMASS = ", amass)
                 print (" ITYP = ", ityp)
                 print (" T = ", self.current_T)
-            phi_sc_odd = SCHAModules.get_odd_straight(a, w, new_pol, trans, amass, ityp,
-                                                    self.current_T, d3)
+            if timer:
+                phi_sc_odd = timer.execute_timed_function(SCHAModules.get_odd_straight, a, w, new_pol, trans, amass, ityp,
+                                                        self.current_T, d3)
+            else:
+                phi_sc_odd = SCHAModules.get_odd_straight(a, w, new_pol, trans, amass, ityp,
+                                                        self.current_T, d3)
 
             if verbose:
                 print ("Outside odd straight.")
                 print ("Saving the odd correction (Ha) as phi_odd.npy")
                 np.save("phi_odd.npy", phi_sc_odd)
 
                 # Try to save this matrix
-                dyn_supercell.dynmats[0] = phi_sc_odd
-                dyn_supercell.save_qe("SupercellOddDynHa")
+                #dyn_supercell.dynmats[0] = phi_sc_odd
+                #dyn_supercell.save_qe("SupercellOddDynHa")
 
 
 
         # Lets fourier transform
-        dynq_odd = CC.Phonons.GetDynQFromFCSupercell(phi_sc_odd, np.array(self.current_dyn.q_tot),
-                                                     self.current_dyn.structure, dyn_supercell.structure)
+        if timer:
+            dynq_odd = timer.execute_timed_function(CC.Phonons.GetDynQFromFCSupercell, phi_sc_odd, np.array(self.current_dyn.q_tot),
+                                                     self.current_dyn.structure, super_structure)
+        else:
+            dynq_odd = CC.Phonons.GetDynQFromFCSupercell(phi_sc_odd, np.array(self.current_dyn.q_tot),
+                                                        self.current_dyn.structure, super_structure)
 
 
         # Convert back the ensemble in Default units
         self.convert_units(UNITS_DEFAULT)
         dynq_odd *= 2 # Ha/bohr^2 -> Ry/bohr^2
 
         # Generate the Phonon structure by including the odd correction
@@ -3036,17 +3154,20 @@
         if is_cluster:
             print("BEFORE COMPUTING:", self.all_properties)
             cluster.compute_ensemble(computing_ensemble, calculator, compute_stress)
 
         else:
             computing_ensemble.get_energy_forces(calculator, compute_stress, stress_numerical, verbose = verbose)
 
+        print("CE BEFORE MERGE:", len(self.force_computed))
+
         if should_i_merge:
             # Remove the noncomputed ensemble from here, and merge
             self.merge(computing_ensemble)
+        print("CE AFTER MERGE:", len(self.force_computed))
 
         print('ENSEMBLE ALL PROPERTIES:', self.all_properties)
 
     def merge(self, other):
         """
         MERGE TWO ENSEMBLES
         ===================
@@ -3104,14 +3225,19 @@
         """
 
         structs = [self.structures[x] for x in np.arange(len(split_mask))[split_mask]]
 
         N = np.sum(split_mask.astype(int))
         ens = Ensemble(self.dyn_0, self.T0, self.dyn_0.GetSupercell())
         ens.init_from_structures(structs)
+        print("Split length:", len(split_mask))
+        print("original force legnth:", len(self.force_computed))
+        print("Expected length:", len(ens.force_computed))
+        print("Splitting force length:", len(self.force_computed[split_mask]))
+
         ens.force_computed[:] = self.force_computed[split_mask]
         ens.stress_computed[:] = self.stress_computed[split_mask]
         ens.energies[:] = self.energies[split_mask]
         ens.forces[:, :, :] = self.forces[split_mask, :, :]
         ens.has_stress = self.has_stress
         ens.ignore_small_w = self.ignore_small_w
         if self.has_stress:
@@ -3126,26 +3252,28 @@
 
     def remove_noncomputed(self):
         """
         Removed all the incomplete calculation from the ensemble.
         It may be used to run a minimization even if the ensemble was not completely calculated.
         """
 
-        good_mask = self.force_computed
+        good_mask = np.copy(self.force_computed)
         if self.has_stress:
             good_mask = good_mask & self.stress_computed
 
         self.N = np.sum( good_mask.astype(int))
         self.forces = self.forces[good_mask, :, :]
         self.sscha_forces = self.sscha_forces[good_mask, :, :]
         self.stresses = self.stresses[good_mask, :, :]
         self.energies = self.energies[good_mask]
         self.sscha_energies = self.sscha_energies[good_mask]
         self.xats = self.xats[good_mask, :, :]
         self.u_disps = self.u_disps[good_mask, :]
+        self.force_computed = self.force_computed[good_mask]
+        self.stress_computed = self.stress_computed[good_mask]
 
         self.structures = [self.structures[x] for x in np.arange(len(good_mask))[good_mask]]
         self.all_properties = [self.all_properties[x] for x in np.arange(len(good_mask))[good_mask]]
 
 
         self.rho = self.rho[good_mask]
 
@@ -3190,14 +3318,15 @@
                 If true the configurations already computed will be skipped.
                 Usefull if the calculation crashed for some reason.
 
         """
 
         # Setup the calculator for each structure
         parallel = False
+        print("Force computed shape:", len(self.force_computed))
         if __MPI__:
             comm = MPI.COMM_WORLD
             size = comm.Get_size()
             rank = comm.Get_rank()
 
             if size > 1:
                 parallel = True
@@ -3346,14 +3475,15 @@
             total_forces = forces
             if compute_stress:
                 total_stress = stress
 
         # Reshape the arrays
         self.forces[:, :, :] = np.reshape(total_forces, (N_rand, self.current_dyn.structure.N_atoms*np.prod(self.supercell), 3), order = "C")
         self.force_computed[:] = True
+        print("Force computed shape:", len(self.force_computed))
 
         if compute_stress:
             self.stresses[:,:,:] = np.reshape(total_stress, (N_rand, 3, 3), order = "C")
             self.has_stress = True
             self.stress_computed[:] = True
         else:
             self.has_stress = False
```

### Comparing `python-sscha-1.3/Modules/Minimizer.py` & `python-sscha-1.3.1/Modules/Minimizer.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/Modules/Optimizer.py` & `python-sscha-1.3.1/Modules/Optimizer.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/Modules/Parallel.py` & `python-sscha-1.3.1/Modules/Parallel.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/Modules/Relax.py` & `python-sscha-1.3.1/Modules/Relax.py`

 * *Files 2% similar despite different names*

```diff
@@ -572,23 +572,28 @@
                 #    self.minim.ensemble.save_bin(ensemble_loc, pop)
 
                 # Compute energies and forces
                 self.minim.ensemble.compute_ensemble(self.calc, True, stress_numerical,
                                                  cluster = self.cluster)
                 #self.minim.ensemble.get_energy_forces(self.calc, True, stress_numerical = stress_numerical)
 
+                print("RELAX force length:", len(self.minim.ensemble.force_computed))
+                
                 if ensemble_loc is not None and self.save_ensemble:
                     self.minim.ensemble.save_bin(ensemble_loc, pop)
+                print("RELAX force length:", len(self.minim.ensemble.force_computed))
 
             self.minim.population = pop
             self.minim.init(delete_previous_data = False)
 
+            print("RELAX force length:", len(self.minim.ensemble.force_computed))
             self.minim.run(custom_function_pre = self.__cfpre__,
                            custom_function_post = self.__cfpost__,
                            custom_function_gradient = self.__cfg__)
+            
 
 
             self.minim.finalize()
 
             # Get the stress tensor [ev/A^3]
             stress_tensor, stress_err = self.minim.get_stress_tensor()
             stress_tensor *= sscha.SchaMinimizer.__RyBohr3_to_evA3__
```

### Comparing `python-sscha-1.3/Modules/SchaMinimizer.py` & `python-sscha-1.3.1/Modules/SchaMinimizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,20 @@
     __MATPLOTLIB__ = False
 import cellconstructor as CC
 import cellconstructor.Methods
 import time
 import warnings
 import sys, os
 
+__SPGLIB__ = True
+try:
+    import spglib
+except:
+    __SPGLIB__ = False
+
 import sscha.Ensemble as Ensemble
 import sscha.Minimizer
 
 from sscha.Parallel import pprint as print
 
 # Rydberg to cm-1 and meV conversion factor
 __RyToCm__  = 109691.40235
@@ -101,15 +107,16 @@
 __MAX_DIAG_ERROR_COUNTER__ = 5
 __MAX_IMAG_ERROR_COUNTER__ = 50
 
 class SSCHA_Minimizer(object):
 
     def __init__(self, ensemble = None, root_representation = "normal",
                  kong_liu_ratio = 0.5, meaningful_factor = 0.2,
-                 minimization_algorithm = "sdes", lambda_a = 1, **kwargs):
+                 minimization_algorithm = "sdes", lambda_a = 1, 
+                 timer=None, **kwargs):
         """
         This class create a minimizer to perform the sscha minimization.
         It performs the sscha minimization.
 
         Parameters
         ----------
             ensemble : Ensemble.Ensemble()
@@ -137,14 +144,16 @@
                 The force constant minimization step.
             **kwargs : any other attribute of this class
         """
 
         self.ensemble = ensemble
         self.root_representation = root_representation
 
+        self.timer=timer
+
 
         # The symmetries
         self.symmetries = None
 
         # The minimization step
         self.min_step_dyn = lambda_a
         self.min_step_struc = 1
@@ -287,49 +296,60 @@
     def set_ensemble(self, ensemble):
         """Provide an ensemble to the minimizer object"""
 
         self.ensemble = ensemble
         if self.dyn is None:
             self.dyn = self.ensemble.current_dyn.Copy()
 
-    def minimization_step(self, custom_function_gradient = None):
+    def minimization_step(self, custom_function_gradient = None, timer=None):
         """
         Perform the single minimization step.
         This modify the self.dyn matrix and updates the ensemble
 
         Parameters
         ----------
             custom_function_gradient : pointer to function ( ndarray(nq x 3nat x 3nat), ndarray(nat, 3))
                 A function that can be used both to print particular component of the gradient
                 or to impose some constraints on the minimization (like lock the position of some atoms).
                 It takes as input the two gradient (the dynamical matrix one and the structure one), and
                 modifies them (or does some I/O on it).
         """
+        print("Minimization step, force computed:", len(self.ensemble.force_computed))
 
         # Setup the symmetries
+        t1 = time.time()
         qe_sym = CC.symmetries.QE_Symmetry(self.dyn.structure)
 
         if self.use_spglib:
             qe_sym.SetupFromSPGLIB()
             self.N_symmetries = qe_sym.QE_nsym
         else:
             qe_sym.SetupQPoint(verbose = False)
             self.N_symmetries = qe_sym.QE_nsym
+        t2 = time.time()
+        if timer is not None:
+            timer.add_timer("Setup symmetries", t2 - t1)
 
 
 
         # Get the gradient of the free-energy respect to the dynamical matrix
         #dyn_grad, err = self.ensemble.get_free_energy_gradient_respect_to_dyn()
         #dyn_grad, err = self.ensemble.get_fc_from_self_consistency(True, True)
         #dyn_grad, err = self.ensemble.get_fc_from_self_consistency(True, True)
         if self.minim_dyn:
             if self.precond_dyn:
-                dyn_grad, err = self.ensemble.get_preconditioned_gradient(True, True, preconditioned=1)
+                if timer is not None:
+                    dyn_grad, err = timer.execute_timed_function(self.ensemble.get_preconditioned_gradient_parallel, True, True, preconditioned=1)
+                else:
+                    dyn_grad, err = self.ensemble.get_preconditioned_gradient_parallel(True, True, preconditioned=1)
             else:
-                dyn_grad, err = self.ensemble.get_preconditioned_gradient(True, True, preconditioned=0)
+                if timer is not None:
+                    dyn_grad, err = timer.execute_timed_function(self.ensemble.get_preconditioned_gradient_parallel, True, True, preconditioned=0)
+                else:
+                    dyn_grad, err = self.ensemble.get_preconditioned_gradient_parallel(True, True, preconditioned=0)
         else:
             dyn_grad = np.zeros( (len(self.dyn.q_tot), 3 * self.dyn.structure.N_atoms, 3 * self.dyn.structure.N_atoms), dtype = np.complex128)
             err = np.zeros_like(dyn_grad)
 
 
         # Perform the symmetrization
 #        qe_sym.ImposeSumRule(dyn_grad)
@@ -342,57 +362,89 @@
                 # Check if the symmetries must be applied in the supercell
                 if self.use_spglib:
                     # Check if we have a supercell
                     supercell = self.dyn.GetSupercell()
                     n_cell = np.prod(supercell)
                     if n_cell == 1:
                         # Only gamma, apply the symmetries
-                        qe_sym.ApplySymmetriesToV2(dyn_grad[0, :, :])
+                        if timer is not None:
+                            timer.execute_timed_function(qe_sym.ApplySymmetriesToV2, dyn_grad[0, :, :])
+                        else:
+                            qe_sym.ApplySymmetriesToV2(dyn_grad[0, :, :])
 
                         #qe_sym.ApplySymmetriesToV2(err)
                         #CC.symmetries.CustomASR(err)
                     else:
                         # We have a supercell, we must generate the dynamical matrix in the supercell
+                        if timer is not None:
+                            timer_prepare = timer.spawn_child()
+                            timer_apply = timer.spawn_child()
+                            timer_return = timer.spawn_child()
+
+
                         t_5 = time.time()
                         super_structure = self.dyn.structure.generate_supercell(supercell)
-                        fc_supercell = CC.Phonons.GetSupercellFCFromDyn(dyn_grad, np.array(self.dyn.q_tot), \
-                            self.dyn.structure, super_structure)
+                        if timer is not None:
+                            timer_prepare.execute_timed_function(CC.Phonons.GetSupercellFCFromDyn, dyn_grad, np.array(self.dyn.q_tot), \
+                                self.dyn.structure, super_structure)
+                        else:
+                            fc_supercell = CC.Phonons.GetSupercellFCFromDyn(dyn_grad, np.array(self.dyn.q_tot), \
+                                self.dyn.structure, super_structure)
 
                         # Lets generate a new symmetries for the supercell
                         qe_sym_supcell = CC.symmetries.QE_Symmetry(super_structure)
                         qe_sym_supcell.SetupFromSPGLIB()
 
                         t_6 = time.time()
 
                         # Apply the symmetries to the fc_supercell matrix
-                        qe_sym_supcell.ApplySymmetriesToV2(fc_supercell)
+                        if timer is not None:
+                            timer_apply.execute_timed_function(qe_sym_supcell.ApplySymmetriesToV2, fc_supercell)
+                        else:
+                            qe_sym_supcell.ApplySymmetriesToV2(fc_supercell)
 
                         t_7 = time.time()
                         # Convert back to Q space
-                        dyn_grad = CC.Phonons.GetDynQFromFCSupercell_parallel(fc_supercell, np.array(self.dyn.q_tot), \
-                            self.dyn.structure, super_structure)
+                        if timer:
+                            dyn_grad = timer_return.execute_timed_function(CC.Phonons.GetDynQFromFCSupercell_parallel, fc_supercell, \
+                                                                           np.array(self.dyn.q_tot), self.dyn.structure, super_structure)
+                        else:
+                            dyn_grad = CC.Phonons.GetDynQFromFCSupercell(fc_supercell, np.array(self.dyn.q_tot), \
+                                self.dyn.structure, super_structure)
 
                         t_8 = time.time()
 
-                        print('    [symmetrization]  Time to prepare the suprecell dyn   : {:.6f} s'.format(t_6 - t_5))
-                        print('    [symmetrization]  Time to symmetrize in the supercell : {:.6f} s'.format(t_7 - t_6))
-                        print('    [symmetrization]  Time to return in fourier space     : {:.6f} s'.format(t_8 - t_7))
+                        if timer is not None:
+                            timer.add_timer("Prepare the suprecell dyn", t_6 - t_5, timer=timer_prepare)
+                            timer.add_timer("Symmetrize in the supercell", t_7 - t_6, timer=timer_apply)
+                            timer.add_timer("Return in fourier space", t_8 - t_7, timer=timer_return)
+
                     
                     # Apply the sum rule at gamma
-                    CC.symmetries.CustomASR(dyn_grad[0,:,:])
+                    if timer is not None:
+                        timer.execute_timed_function(CC.symmetries.CustomASR, dyn_grad[0,:,:])
+                    else:
+                        CC.symmetries.CustomASR(dyn_grad[0,:,:])
                 else:
-                    qe_sym.SymmetrizeFCQ(dyn_grad, self.dyn.q_stars, asr = "custom")
+                    if timer is not None:
+                        timer.execute_timed_function(qe_sym.SymmetrizeFCQ, dyn_grad, self.dyn.q_stars, asr = "custom")
+                    else:
+                        qe_sym.SymmetrizeFCQ(dyn_grad, self.dyn.q_stars, asr = "custom")
+
                     #qe_sym.SymmetrizeFCQ(err, np.array(self.dyn.q_stars), asr = "custom")
 
                 # Just divide the error by the square root the number of symmetries
                 err /= np.sqrt(qe_sym.QE_nsym * np.prod(self.ensemble.supercell))
             else:
-                CC.symmetries.CustomASR(dyn_grad[0, :,:])
-        t2 = time.time()
-        print ("Time elapsed to symmetrize the gradient:", t2 - t1, "s")
+                # Apply the sum rule at gamma
+                if timer is not None:
+                    timer.execute_timed_function(CC.symmetries.CustomASR, dyn_grad[0,:,:])
+                else:
+                    CC.symmetries.CustomASR(dyn_grad[0,:,:])
+
 
 #        # get the gradient in the supercell
 #        new_grad_tmp = CC.Phonons.GetSupercellFCFromDyn(dyn_grad, np.array(self.dyn.q_tot),
 #                                                        self.dyn.structure,
 #                                                        self.dyn.structure.generate_supercell(self.ensemble.supercell))
 #
 #        #np.savetxt("NewGradSC.dat", np.real(new_grad_tmp))
@@ -429,33 +481,41 @@
 
 
             # Preconditionate the gradient for the wyckoff minimization
             if self.precond_wyck:
                 w_pols = None
                 if len(self.dyn.q_tot) == 1:
                     w_pols = (self.ensemble.current_w, self.ensemble.current_pols)
-                struct_precond = GetStructPrecond(self.ensemble.current_dyn, ignore_small_w = self.ensemble.ignore_small_w, w_pols = w_pols)
+
+                if timer:
+                    struct_precond = timer.execute_timed_function(GetStructPrecond, self.ensemble.current_dyn, ignore_small_w = self.ensemble.ignore_small_w, w_pols = w_pols)
+                else:
+                    struct_precond = GetStructPrecond(self.ensemble.current_dyn, ignore_small_w = self.ensemble.ignore_small_w, w_pols = w_pols)
                 struct_grad_precond = struct_precond.dot(struct_grad_reshaped)
                 struct_grad = struct_grad_precond.reshape( (self.dyn.structure.N_atoms, 3))
             t2 = time.time()
 
-            print ("Time elapsed to compute the structure gradient:", t2 - t1, "s")
+            if timer:
+                timer.add_timer("Compute the structure gradient", t2 - t1)
 
 
             # Apply the symmetries to the forces
             if not self.neglect_symmetries:
                 if not self.use_spglib:
                     qe_sym.SetupQPoint()
-                qe_sym.SymmetrizeVector(struct_grad)
+                if timer:
+                    timer.execute_timed_function(qe_sym.SymmetrizeVector, struct_grad)
+                else:
+                    qe_sym.SymmetrizeVector(struct_grad)
                 #qe_sym.SymmetrizeVector(struct_grad_err)
                 struct_grad_err /= np.sqrt(qe_sym.QE_nsym)
 
 
                 #print "applying sum rule and symmetries:"
-                #qe_sym.SymmetrizeFCQ(dyn_grad, np.array(self.dyn.q_stars), asr = "custom")
+                #qe_sym.SymmetrizeFCQ(dyn_grad, self.dyn.q_stars, asr = "custom")
                 #print "SECOND DIAG:", np.linalg.eigvalsh(dyn_grad[0, :, :])
 
 
             # Perform the step for the structure
             #print "min step:", self.min_step_struc
             #self.dyn.structure.coords -= self.min_step_struc * struct_grad
 
@@ -484,17 +544,23 @@
     - [Optional] The minimizer (self) object
 
       The function you provided accepts {} arguments instead.
 '''.format(len(sig))
                 raise ValueError(MSG)
 
             if len(sig) == 3:
-                custom_function_gradient(dyn_grad, struct_grad, self)
+                if timer:
+                    timer.execute_timed_function(custom_function_gradient, dyn_grad, struct_grad, self)
+                else:
+                    custom_function_gradient(dyn_grad, struct_grad, self)
             else:
-                custom_function_gradient(dyn_grad, struct_grad)
+                if timer:
+                    timer.execute_timed_function(custom_function_gradient, dyn_grad, struct_grad)
+                else:
+                    custom_function_gradient(dyn_grad, struct_grad)
 
 
         # Append the gradient modulus to the minimization info
         if self.minim_struct:
             self.__gw__.append(np.sqrt( np.sum(struct_grad**2)))
             self.__gw_err__.append(np.sqrt( np.einsum("ij, ij", struct_grad_err, struct_grad_err) / qe_sym.QE_nsymq))
         else:
@@ -503,28 +569,35 @@
 
 
         # Store the gradient in the minimization
         self.__gc__.append( np.sqrt(np.sum( np.abs(dyn_grad)**2)))
         self.__gc_err__.append( np.sqrt(np.sum( np.abs(err)**2)))
 
         # Perform the minimization step (with the chosen minimization algorithm)
-        new_kl_ratio = self.ensemble.get_effective_sample_size() / self.ensemble.N
+        if timer:
+            new_kl_ratio = timer.execute_timed_function(self.ensemble.get_effective_sample_size) / self.ensemble.N
+        else:
+            new_kl_ratio = self.ensemble.get_effective_sample_size() / self.ensemble.N
 
         # Here a cycle to avoid diagonalization issues
         is_diag_ok = False
         diag_error_counter = 0
         imag_freq_counter = 0
         while not is_diag_ok:
             is_diag_ok = True
-            self.minimizer.update_dyn(new_kl_ratio, dyn_grad, struct_grad)
+            if timer:
+                timer.execute_timed_function(self.minimizer.update_dyn, new_kl_ratio, dyn_grad, struct_grad)
+                new_dyn, new_struct = timer.execute_timed_function(self.minimizer.get_dyn_struct)
+            else:
+                self.minimizer.update_dyn(new_kl_ratio, dyn_grad, struct_grad)        
+                new_dyn, new_struct = self.minimizer.get_dyn_struct()
 
 
 
             # Get the new dynamical matrix and strucure after the step
-            new_dyn, new_struct = self.minimizer.get_dyn_struct()
 
             # Perform the step for the dynamical matrix respecting the root representation
             #new_dyn = PerformRootStep(np.array(self.dyn.dynmats, order = "C"), dyn_grad,
             #                          self.min_step_dyn, root_representation = self.root_representation,
             #                          minimization_algorithm = self.minimization_algorithm)
 
             # Update the dynamical matrix
@@ -534,31 +607,42 @@
 
             # Update the structure
             if self.minim_struct:
                 self.dyn.structure.coords[:,:] = new_struct
 
             # Check if we must enforce the symmetries and the sum rule:
             if self.enforce_sum_rule and (not self.neglect_symmetries):
-                self.dyn.Symmetrize(use_spglib = self.use_spglib)
+                if timer:
+                    timer.execute_timed_function(self.dyn.Symmetrize, use_spglib = self.use_spglib)
+                else:
+                    self.dyn.Symmetrize(use_spglib = self.use_spglib)
 
 
             # If we have imaginary frequencies, force the kl ratio to zero
 
             # Update the ensemble
             try:
-                self.update()
+                if timer:
+                    timer.execute_timed_function(self.update)
+                else:
+                    self.update()
             except np.linalg.LinAlgError as error:
                 print("Diagonalization error:")
                 print(error)
                 print("Reducing the minimization step...")
                 new_kl_ratio = 0 # Force step reduction
                 is_diag_ok = False
                 diag_error_counter += 1
 
-            if self.check_imaginary_frequencies():
+            if timer:
+                check_imag = timer.execute_timed_function(self.check_imaginary_frequencies)
+            else:
+                check_imag = self.check_imaginary_frequencies()
+
+            if check_imag:
                 print("Immaginary frequencies found! Redoing the step.")
                 new_kl_ratio = 0
                 is_diag_ok = False
                 imag_freq_counter += 1
 
             if diag_error_counter >= self.max_diag_error_counter:
                 ERROR_MSG = """
@@ -874,29 +958,32 @@
         Result
         ------
             bool :
                 True if the simulation ended for converging.
         """
         return self.__converged__
 
-    def update(self):
+    def update(self, timer=None):
         """
         UPDATE IMPORTANCE SAMPLING
         ==========================
 
 
         This methods makes the self.dyn coincide with self.ensemble.current_dyn, and overwrites the stochastic
         weights of the current_dyn.
 
         Call this method each time you modify the dynamical matrix of the minimization to avoid errors.
 
         NOTE: it is equivalent to call self.ensemble.update_weights(self.dyn, self.ensemble.current_T)
         """
 
-        self.ensemble.update_weights(self.dyn, self.ensemble.current_T)
+        if timer:
+            timer.execute_timed_function(self.ensemble.update_weights, self.dyn, self.ensemble.current_T)
+        else:
+            self.ensemble.update_weights(self.dyn, self.ensemble.current_T)
 
 
     def get_free_energy(self, return_error = False):
         """
         SSCHA FREE ENERGY
         =================
 
@@ -929,29 +1016,36 @@
         #TODO: CHECK THE CONSISTENCY BETWEEN THE DYNAMICAL MATRICES
         # Check if the dynamical matrix has correctly been updated
         #if np.sum( self.dyn != self.ensemble.current_dyn):
         #    raise ValueError("Error, the ensemble dynamical matrix has not been updated. You forgot to call self.update() before")
 
         return self.ensemble.get_free_energy(return_error = return_error) / np.prod(self.ensemble.supercell)
 
-    def init(self, verbosity = False, delete_previous_data = True):
+    def init(self, verbosity = False, delete_previous_data = True, init_timer = True):
         """
         INITIALIZE THE MINIMIZATION
         ===========================
 
         This subroutine initialize the variables needed by the minimization.
         Call this before the first time you invoke the run function.
 
         Parameters
         ----------
             verbosity : bool
                 If true prints some debugging information
             delete_previous_data : bool
                 If true, it will clean previous minimizations from the free energies, gradients...
+            init_timer : bool
+                If true, it will initialize the timer for timing the function.
+                This can slightly slowdown the minimization, 
+                however enables the use of the timer to check the time spent in each step.
+
         """
+        if self.timer is None and init_timer:
+            self.timer = CC.Timer.Timer(active=True)
 
         if (not self.minim_dyn) and (not self.minim_struct):
             raise ValueError("Error, either one of minim_dyn or minim_struct should be True.")
 
         # Check the ensemble size
         if not self.ensemble.structures:
             s = """The ensemble has not been initialized.
@@ -1082,15 +1176,15 @@
         if not self.precond_wyck:
             if verbosity:
                 print ("Get wickoff best step...")
             self.min_step_struc *= GetBestWykoffStep(self.dyn)
 
 
     def run(self, verbose = 1, custom_function_pre = None, custom_function_post = None,
-            custom_function_gradient = None):
+            custom_function_gradient = None, timer=None):
         """
         RUN THE SSCHA MINIMIZATION
         ==========================
 
         This function uses all the setted up parameters to run the minimization
 
         The minimization is stopped only when one of the stopping criteria are met.
@@ -1118,14 +1212,16 @@
                 the minimization step has been perfomed. The data about free energy,
                 gradient and effective sample size have been updated.
             custom_function_gradient : pointer to function (ndarray(NQ, 3*nat, 3*nat), ndarray(nat, 3))
                 A pointer to a function that takes as an input the two gradients, and modifies them.
                 It is called after the two gradients have been computed, and it is used to
                 impose some constraint on the minimization.
         """
+        if timer is None:
+            timer = self.timer
 
 
         # Eliminate the convergence flag
         self.__converged__ = False
 
         # TODO: Activate a new pipe to avoid to stop the execution of the python
         #       code when running the minimization. This allows for interactive plots
@@ -1147,55 +1243,66 @@
 
         while running:
             # Invoke the custom fuction if any
             if custom_function_pre is not None:
                 custom_function_pre(self)
 
             # Store the original dynamical matrix
-            old_dyn = self.dyn.Copy()
+            if timer is not None:
+                old_dyn = timer.execute_timed_function(self.dyn.Copy)
+            else:
+                old_dyn = self.dyn.Copy()
 
             if verbose >= 1:
                 print ()
                 print (" # ---------------- NEW MINIMIZATION STEP --------------------")
                 print ("Step ka = ", len(self.__fe__))
 
             # Perform the minimization step
-            t1 = time.time()
-            self.minimization_step(custom_function_gradient)
-            t2 = time.time()
-            if verbose >=1:
-                print ("Time elapsed to perform the minimization step:", t2 - t1, "s")
+            if timer is not None:
+                timer.execute_timed_function(self.minimization_step, custom_function_gradient) 
+                im_freqs = timer.execute_timed_function(self.check_imaginary_frequencies)
+            else:
+                self.minimization_step(custom_function_gradient)
+                im_freqs = self.check_imaginary_frequencies()
 
 
-            if self.check_imaginary_frequencies():
+            if im_freqs:
                 print ("Immaginary frequencies found.")
                 print ("Minimization aborted.")
                 break
 
             # Compute the free energy and its error
             fe, err = self.get_free_energy(True)
             fe -= self.eq_energy
             self.__fe__.append(np.real(fe))
             self.__fe_err__.append(np.real(err))
 
-            harm_fe = self.dyn.GetHarmonicFreeEnergy(self.ensemble.current_T, w_pols = (self.ensemble.current_w, self.ensemble.current_pols)) / np.prod(self.ensemble.supercell)
+            if timer is not None:
+                harm_fe = timer.execute_timed_function(self.dyn.GetHarmonicFreeEnergy, self.ensemble.current_T, w_pols = (self.ensemble.current_w, self.ensemble.current_pols)) / np.prod(self.ensemble.supercell)
+            else:
+                harm_fe = self.dyn.GetHarmonicFreeEnergy(self.ensemble.current_T, w_pols = (self.ensemble.current_w, self.ensemble.current_pols)) / np.prod(self.ensemble.supercell)
             anharm_fe = np.real(fe - harm_fe)
 
             # Compute the KL ratio
             #print "SAVE RHO BEFORE PRINT:"
             #np.savetxt("LAST_RHO_BEFORE_PRINT.dat", self.ensemble.rho)
-            self.__KL__.append(self.ensemble.get_effective_sample_size())
+            if timer is not None:
+                kl_sample_size = timer.execute_timed_function(self.ensemble.get_effective_sample_size)
+            else:
+                kl_sample_size = self.ensemble.get_effective_sample_size()
+
+            self.__KL__.append(kl_sample_size)
 
             # Print the step
             if verbose >= 1:
                 print ()
                 print ("")
                 print("Number of symmetries before the step: ", self.N_symmetries)
                 if self.use_spglib:
-                    import spglib
                     print("Group space: ", spglib.get_spacegroup(self.dyn.structure.get_ase_atoms()))
                 print ("Harmonic contribution to free energy = %16.8f meV" % (harm_fe * __RyTomev__))
                 print ("Anharmonic contribution to free energy = %16.8f +- %16.8f meV" % (anharm_fe * __RyTomev__,
                                                                                          np.real(err) * __RyTomev__))
                 print ("Free energy = %16.8f +- %16.8f meV" % (self.__fe__[-1] * __RyTomev__,
                                                               self.__fe_err__[-1] * __RyTomev__))
 
@@ -1209,25 +1316,38 @@
             if verbose >= 2:
                 # Print the dynamical matrix at each step
                 ka = len(self.__fe__)
                 self.dyn.save_qe("minim_dyn_step%d_" % ka)
 
 
             # Get the stopping criteria
-            running = not self.check_stop()
-            print ("Check the stopping criteria: Running = ", running)
+            if timer is not None:
+                running = not timer.execute_timed_function(self.check_stop)
+            else:
+                running = not self.check_stop()
+
+            if verbose >= 1:
+                print ("Check the stopping criteria: Running = ", running)
 
 
             if len(self.__fe__) > self.max_ka and self.max_ka > 0:
-                print ("Maximum number of steps reached.")
+                if verbose >= 1:
+                    print ("Maximum number of steps reached.")
                 running = False
 
             # Invoke the custom function (if any)
             if custom_function_post is not None:
-                custom_function_post(self)
+                if timer is not None:
+                    timer.execute_timed_function(custom_function_post, self)
+                else:
+                    custom_function_post(self)
+
+
+            if verbose >= 2:
+                timer.print_report(is_master = True)
 
             # Flush the output to avoid asyncronous printing
             sys.stdout.flush()
 
         # If your stopped not for convergence then
         # restore the last dynamical matrix
         if not self.is_converged():
@@ -1236,29 +1356,31 @@
             self.dyn = old_dyn
 
             print ("Updating the importance sampling...")
             self.update()
             print ()
 
 
-    def finalize(self, verbose = 1):
+    def finalize(self, verbose = 1, timer=None):
         """
         FINALIZE
         ========
 
         This method finalizes the minimization, and prints on stdout the
         results of the current minimization.
 
         Parameters
         ----------
             verbose : int, optional
                 The verbosity level. If 0 only the final free energy and gradient is printed.
                 If 1 the stress tensor is also printed. If 2 also the final structure and frequencies
                 are printed.
         """
+        if timer is None:
+            timer = self.timer
 
 
 
         print ()
         print (" * * * * * * * * ")
         print (" *             * ")
         print (" *   RESULTS   * ")
@@ -1347,14 +1469,17 @@
             trans = CC.Methods.get_translations(pols, super_struct.get_masses_array())
 
             for i in range(len(w)):
                 print ("Mode %5d:   freq %16.8f cm-1  | is translation? " % (i+1, w[i] * __RyToCm__), trans[i])
 
             print ()
 
+        if timer is not None:
+            timer.print_report(is_master=True)
+
 
     def check_imaginary_frequencies(self):
         """
         The following subroutine check if the current matrix has imaginary frequency. In this case
         the minimization is stopped.
         """
```

### Comparing `python-sscha-1.3/Modules/Tools.py` & `python-sscha-1.3.1/Modules/Tools.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/Modules/Utilities.py` & `python-sscha-1.3.1/Modules/Utilities.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/README.md` & `python-sscha-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/SCHAModules/cell_force.f90` & `python-sscha-1.3.1/SCHAModules/cell_force.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/SCHAModules/get_cmat.f90` & `python-sscha-1.3.1/SCHAModules/get_cmat.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/SCHAModules/get_emat.f90` & `python-sscha-1.3.1/SCHAModules/get_emat.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/SCHAModules/get_g.f90` & `python-sscha-1.3.1/SCHAModules/get_g.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/SCHAModules/get_gradient_supercell.f90` & `python-sscha-1.3.1/SCHAModules/get_gradient_supercell.f90`

 * *Files 0% similar despite different names*

```diff
@@ -391,15 +391,15 @@
 ! Compute the upsilon matrix in the supercell
 call cpu_time(t1)
 call get_upsilon_matrix(n_modes, natsc, ntyp_sc, wr_sc, epols_sc, trans, mass, ityp_sc, T, ups_mat)
 call cpu_time(t2)
 !print *, "Time to compute the upsilon matrix:", t2 - t1
 
 
-!$OMP PARALLEL DO PRIVATE(ical, jcal)
+!!$OMP PARALLEL DO PRIVATE(ical, jcal)
 do i_r = 1, n_random
    do alpha = 1, 3
       do i = 1, natsc
          ical = alpha + (i-1)*3
          v_disp(i_r, i, alpha) = 0.0d0
 
          ! Sum up
@@ -408,34 +408,34 @@
                jcal = beta + (j-1)*3
                v_disp(i_r, i, alpha) = v_disp(i_r, i, alpha) + u_disp(i_r, j, beta) * ups_mat(jcal, ical)
             enddo
          enddo
       enddo
    enddo
 enddo
-!$OMP END PARALLEL DO
+!!$OMP END PARALLEL DO
 
 
 call cpu_time(t1)
-!$OMP PARALLEL DO COLLAPSE(4) PRIVATE(ical, jcal)
+!!$OMP PARALLEL DO COLLAPSE(4) PRIVATE(ical, jcal)
 do alpha = 1, 3
    do beta = 1, 3
       do i = 1, natsc
          do j = 1, natsc
             ical = alpha + (i-1)*3
             jcal = beta + (j-1)*3
             call average_error_weight(v_disp(:, i, alpha) * eforces(:,  j, beta), &
                  rho, log_err, grad(ical, jcal), grad_err(ical, jcal))
             !print *, "Terra di mezzo:", ical, jcal, "UF:", uf_mat(ical, jcal), &
             !     sum(u_disp(:, i, alpha) * eforces(:, j, beta)) / sum(rho)
          end do
       end do
    end do
 end do
-!$OMP END PARALLEL DO
+!!$OMP END PARALLEL DO
 
 ! Impose the hermitianity
 ! do ical = 1, 3*natsc
 !    do jcal = ical, 3*natsc
 !       uf_mat(ical, jcal) = 0.5d0 * (uf_mat(ical, jcal) + uf_mat(jcal, ical))
 !       err_uf_mat(ical, jcal) = 0.5d0 *dsqrt(err_uf_mat(ical, jcal)**2 + err_uf_mat(ical, jcal)**2)
 !       if (ical /= jcal) then
```

### Comparing `python-sscha-1.3/SCHAModules/get_gradient_supercell_fast.f90` & `python-sscha-1.3.1/SCHAModules/get_gradient_supercell_fast.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/SCHAModules/get_odd_straight.f90` & `python-sscha-1.3.1/SCHAModules/get_odd_straight.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/SCHAModules/get_odd_straight_with_v4.f90` & `python-sscha-1.3.1/SCHAModules/get_odd_straight_with_v4.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/SCHAModules/get_stress_tensor.f90` & `python-sscha-1.3.1/SCHAModules/get_stress_tensor.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/SCHAModules/get_upsilon_matrix.f90` & `python-sscha-1.3.1/SCHAModules/get_upsilon_matrix.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/SCHAModules/get_v3.f90` & `python-sscha-1.3.1/SCHAModules/get_v3.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/SCHAModules/get_v4.f90` & `python-sscha-1.3.1/SCHAModules/get_v4.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/SCHAModules/module_anharmonic.f90` & `python-sscha-1.3.1/SCHAModules/module_anharmonic.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/SCHAModules/module_new_thermodynamic.f90` & `python-sscha-1.3.1/SCHAModules/module_new_thermodynamic.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/SCHAModules/module_stochastic.f90` & `python-sscha-1.3.1/SCHAModules/module_stochastic.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/SCHAModules/multiply_lambda_tensor.f90` & `python-sscha-1.3.1/SCHAModules/multiply_lambda_tensor.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/python_sscha.egg-info/SOURCES.txt` & `python-sscha-1.3.1/python_sscha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/scripts/cluster_check.x` & `python-sscha-1.3.1/scripts/cluster_check.x`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/scripts/plot_frequencies.py` & `python-sscha-1.3.1/scripts/plot_frequencies.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/scripts/read_incomplete_ensemble.py` & `python-sscha-1.3.1/scripts/read_incomplete_ensemble.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/scripts/sscha` & `python-sscha-1.3.1/scripts/sscha`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/scripts/sscha-plot-data.py` & `python-sscha-1.3.1/scripts/sscha-plot-data.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/scripts/static-vc-relax.pyx` & `python-sscha-1.3.1/scripts/static-vc-relax.pyx`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3/setup.py` & `python-sscha-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import numpy 
 
 extra_flags_c = ["-fopenmp"]
 extra_link_args_c = ["-fopenmp"]
 mpi_compile_args = []
 mpi_link_args = []
 
+
 # If true, do not check for parallel
 avoid_parallel_test = True 
 
 # Get the MPI from environmental variables
 parallel = False 
 if "MPICC" in  os.environ:
         mpicc = os.environ["MPICC"]
@@ -84,15 +85,15 @@
 #                   extra_link_args = mpi_link_args + extra_link_args_c
 #                   )
 
 
 
 # Prepare the compilation of the Python Conde
 setup( name = "python-sscha",
-       version = "1.3",
+       version = "1.3.1",
        description = "Python implementation of the sscha code",
        author = "Lorenzo Monacelli",
        url = "https://github.com/mesonepigreco/python-sscha",
        packages = ["sscha"],
        package_dir = {"sscha": "Modules"},
        setup_requires = ["numpy", "ase", "scipy", "cellconstructor", "spglib", "matplotlib"],
        ext_modules = [SCHAModules], # odd_HP
```

