# Comparing `tmp/CRYSTALpytools-2023.4.4.tar.gz` & `tmp/CRYSTALpytools-2023.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CRYSTALpytools-2023.4.4.tar", last modified: Tue Apr  4 07:53:14 2023, max compression
+gzip compressed data, was "CRYSTALpytools-2023.6.6.tar", last modified: Tue Jun  6 15:03:36 2023, max compression
```

## Comparing `CRYSTALpytools-2023.4.4.tar` & `CRYSTALpytools-2023.6.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 davidemitoli   (501) staff       (20)        0 2023-04-04 07:53:14.284404 CRYSTALpytools-2023.4.4/
-drwxr-xr-x   0 davidemitoli   (501) staff       (20)        0 2023-04-04 07:53:14.283324 CRYSTALpytools-2023.4.4/CRYSTALpytools/
--rw-r--r--   0 davidemitoli   (501) staff       (20)      173 2023-03-20 14:51:49.000000 CRYSTALpytools-2023.4.4/CRYSTALpytools/__init__.py
--rw-r--r--   0 davidemitoli   (501) staff       (20)      577 2023-03-20 14:51:49.000000 CRYSTALpytools-2023.4.4/CRYSTALpytools/adsorb.py
--rw-r--r--   0 davidemitoli   (501) staff       (20)      757 2023-03-20 14:51:49.000000 CRYSTALpytools-2023.4.4/CRYSTALpytools/calculate.py
--rw-r--r--   0 davidemitoli   (501) staff       (20)    12685 2023-03-20 14:51:49.000000 CRYSTALpytools-2023.4.4/CRYSTALpytools/convert.py
--rw-r--r--   0 davidemitoli   (501) staff       (20)   103327 2023-04-02 17:10:05.000000 CRYSTALpytools-2023.4.4/CRYSTALpytools/crystal_io.py
--rw-r--r--   0 davidemitoli   (501) staff       (20)     3613 2023-03-20 14:51:49.000000 CRYSTALpytools-2023.4.4/CRYSTALpytools/execute.py
--rw-r--r--   0 davidemitoli   (501) staff       (20)   121351 2023-04-02 17:10:05.000000 CRYSTALpytools-2023.4.4/CRYSTALpytools/plot.py
--rw-r--r--   0 davidemitoli   (501) staff       (20)    78480 2023-04-02 17:10:05.000000 CRYSTALpytools-2023.4.4/CRYSTALpytools/thermodynamics.py
--rw-r--r--   0 davidemitoli   (501) staff       (20)    12906 2023-03-20 14:51:49.000000 CRYSTALpytools-2023.4.4/CRYSTALpytools/unit_test.py
--rw-r--r--   0 davidemitoli   (501) staff       (20)      974 2023-03-20 14:51:49.000000 CRYSTALpytools-2023.4.4/CRYSTALpytools/units.py
--rw-r--r--   0 davidemitoli   (501) staff       (20)      693 2023-03-20 14:51:49.000000 CRYSTALpytools-2023.4.4/CRYSTALpytools/utils.py
-drwxr-xr-x   0 davidemitoli   (501) staff       (20)        0 2023-04-04 07:53:14.284071 CRYSTALpytools-2023.4.4/CRYSTALpytools.egg-info/
--rw-r--r--   0 davidemitoli   (501) staff       (20)      706 2023-04-04 07:53:14.000000 CRYSTALpytools-2023.4.4/CRYSTALpytools.egg-info/PKG-INFO
--rw-r--r--   0 davidemitoli   (501) staff       (20)      527 2023-04-04 07:53:14.000000 CRYSTALpytools-2023.4.4/CRYSTALpytools.egg-info/SOURCES.txt
--rw-r--r--   0 davidemitoli   (501) staff       (20)        1 2023-04-04 07:53:14.000000 CRYSTALpytools-2023.4.4/CRYSTALpytools.egg-info/dependency_links.txt
--rw-r--r--   0 davidemitoli   (501) staff       (20)       23 2023-04-04 07:53:14.000000 CRYSTALpytools-2023.4.4/CRYSTALpytools.egg-info/requires.txt
--rw-r--r--   0 davidemitoli   (501) staff       (20)       15 2023-04-04 07:53:14.000000 CRYSTALpytools-2023.4.4/CRYSTALpytools.egg-info/top_level.txt
--rw-r--r--   0 davidemitoli   (501) staff       (20)     1167 2023-03-20 14:51:49.000000 CRYSTALpytools-2023.4.4/LICENSE.txt
--rw-r--r--   0 davidemitoli   (501) staff       (20)      706 2023-04-04 07:53:14.284262 CRYSTALpytools-2023.4.4/PKG-INFO
--rw-r--r--   0 davidemitoli   (501) staff       (20)     6068 2023-03-20 14:51:49.000000 CRYSTALpytools-2023.4.4/README.md
--rw-r--r--   0 davidemitoli   (501) staff       (20)      105 2023-03-20 14:51:49.000000 CRYSTALpytools-2023.4.4/pyproject.toml
--rw-r--r--   0 davidemitoli   (501) staff       (20)       38 2023-04-04 07:53:14.284448 CRYSTALpytools-2023.4.4/setup.cfg
--rw-r--r--   0 davidemitoli   (501) staff       (20)     1034 2023-04-04 07:53:01.000000 CRYSTALpytools-2023.4.4/setup.py
+drwxr-xr-x   0 brunocamino   (501) staff       (20)        0 2023-06-06 15:03:36.914911 CRYSTALpytools-2023.6.6/
+drwxr-xr-x   0 brunocamino   (501) staff       (20)        0 2023-06-06 15:03:36.913292 CRYSTALpytools-2023.6.6/CRYSTALpytools/
+-rw-r--r--   0 brunocamino   (501) staff       (20)      289 2023-04-25 17:05:03.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools/__init__.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)      577 2022-09-15 16:48:47.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools/adsorb.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)      757 2022-09-15 16:48:47.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools/calculate.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)    12828 2023-06-06 14:59:42.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools/convert.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)   102276 2023-06-06 14:55:03.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools/crystal_io.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)     3613 2022-09-15 16:48:47.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools/execute.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)   121442 2023-04-25 17:05:03.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools/plot.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)    73581 2023-06-06 14:55:03.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools/thermodynamics.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)    12906 2023-01-02 18:39:56.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools/unit_test.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)      974 2023-02-10 08:58:41.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools/units.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)      693 2022-09-15 16:48:47.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools/utils.py
+drwxr-xr-x   0 brunocamino   (501) staff       (20)        0 2023-06-06 15:03:36.914611 CRYSTALpytools-2023.6.6/CRYSTALpytools.egg-info/
+-rw-r--r--   0 brunocamino   (501) staff       (20)      706 2023-06-06 15:03:36.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools.egg-info/PKG-INFO
+-rw-r--r--   0 brunocamino   (501) staff       (20)      527 2023-06-06 15:03:36.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools.egg-info/SOURCES.txt
+-rw-r--r--   0 brunocamino   (501) staff       (20)        1 2023-06-06 15:03:36.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools.egg-info/dependency_links.txt
+-rw-r--r--   0 brunocamino   (501) staff       (20)       23 2023-06-06 15:03:36.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools.egg-info/requires.txt
+-rw-r--r--   0 brunocamino   (501) staff       (20)       15 2023-06-06 15:03:36.000000 CRYSTALpytools-2023.6.6/CRYSTALpytools.egg-info/top_level.txt
+-rw-r--r--   0 brunocamino   (501) staff       (20)     1167 2022-09-15 16:48:47.000000 CRYSTALpytools-2023.6.6/LICENSE.txt
+-rw-r--r--   0 brunocamino   (501) staff       (20)      706 2023-06-06 15:03:36.914778 CRYSTALpytools-2023.6.6/PKG-INFO
+-rw-r--r--   0 brunocamino   (501) staff       (20)     3925 2023-06-06 14:55:03.000000 CRYSTALpytools-2023.6.6/README.md
+-rw-r--r--   0 brunocamino   (501) staff       (20)      105 2022-12-21 17:23:54.000000 CRYSTALpytools-2023.6.6/pyproject.toml
+-rw-r--r--   0 brunocamino   (501) staff       (20)       38 2023-06-06 15:03:36.914957 CRYSTALpytools-2023.6.6/setup.cfg
+-rw-r--r--   0 brunocamino   (501) staff       (20)     1043 2023-06-06 15:03:22.000000 CRYSTALpytools-2023.6.6/setup.py
```

### Comparing `CRYSTALpytools-2023.4.4/CRYSTALpytools/adsorb.py` & `CRYSTALpytools-2023.6.6/CRYSTALpytools/adsorb.py`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.4.4/CRYSTALpytools/calculate.py` & `CRYSTALpytools-2023.6.6/CRYSTALpytools/calculate.py`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.4.4/CRYSTALpytools/convert.py` & `CRYSTALpytools-2023.6.6/CRYSTALpytools/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,41 +272,45 @@
 
     gui.lattice = lattice_vectors
     gui.n_atoms = structure.num_sites
     gui.space_group = SpacegroupAnalyzer(structure).get_space_group_number()
     gui.symmops = []
     
     if symmetry == True:
+        n_symmops = 0
         if dimensionality == 3:
             symmops = SpacegroupAnalyzer(structure).get_symmetry_operations(cartesian=True)
 
             for symmop in symmops:
-                gui.symmops.extend(symmop.rotation_matrix.tolist())
-                gui.symmops.append(symmop.translation_vector.tolist())
+                if np.all(symmop.translation_vector == 0.):
+                    n_symmops += 1
+                    gui.symmops.extend(symmop.rotation_matrix.tolist())
+                    gui.symmops.append(symmop.translation_vector.tolist())
             
-            gui.n_symmops = int(len(symmops))
+            gui.n_symmops = n_symmops
 
         elif dimensionality == 2:
 
             #center the slab first
             structure = center_slab(structure)
 
             # Then center at z=0.0
             translation = np.array([0.0, 0.0, -0.5])
             structure.translate_sites(list(range(structure.num_sites)),
                                           translation, to_unit_cell=False)
             
             sg = SpacegroupAnalyzer(structure)
             ops = sg.get_symmetry_operations(cartesian=True)
             for op in ops:
-                if op.translation_vector[2] == 0.:
+                if np.all(op.translation_vector == 0.):
+                    n_symmops += 1
                     gui.symmops.extend(op.rotation_matrix.tolist())
                     gui.symmops.append(op.translation_vector.tolist())
          
-            gui.n_symmops = int(len(gui.symmops)/4)
+            gui.n_symmops = n_symmops
 
         elif dimensionality == 1:
             print('WARNING: check the polymer is correctly centered in the cell and that the correct symmops are used.')      
 
         elif dimensionality == 0:
             print('WARNING: 0D in development')
             sys.exit(1)
```

### Comparing `CRYSTALpytools-2023.4.4/CRYSTALpytools/crystal_io.py` & `CRYSTALpytools-2023.6.6/CRYSTALpytools/crystal_io.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,240 +1,180 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Fri Nov 19 18:28:28 2021
 """
 from CRYSTALpytools import units
+from CRYSTALpytools.base.crysd12 import Crystal_inputBASE
 
 
-class Crystal_input:
-    # This creates a crystal_input object
+class Crystal_input(Crystal_inputBASE):
+    """
+    Crystal input object inherited from Crystal_inputBASE.
 
-    def __init__(self):
-        # Initialise the object
+    **Note for users**
 
-        pass
+    ``Crystal_input`` object is strictly structured by 'blocks', which, in
+    general, is defined as keywords that are closed by 'END'. All the blocks
+    are organized in layers and each corresponds to a list of keywords that can
+    be called and set.The current structure of ``Crystal_input`` is listed
+    below:
 
-    def add_ghost(self, ghost_atoms):
-        # Add ghost functions to the input object
+    # Layer 1: ``geom``, ``basisset``, ``scf``
+    # Layer 2: ``optgeom``, ``freqcalc``, ``dft``, ``dftd3``, ``gcp``, ``fixindex``
+    # Layer 3: ``preoptgeom``, ``geom``, ``base``
 
-        if self.is_basisset == True:
-            self.bs_block.append('GHOSTS\n')
-            self.bs_block.append('%s\n' % len(ghost_atoms))
-            self.bs_block.append(' '.join([str(x) for x in ghost_atoms])+'\n')
-        else:
-            self.bs_block.insert(-1, 'GHOSTS\n')
-            self.bs_block.insert(-1, '%s\n' % len(ghost_atoms))
-            self.bs_block.insert(-1, ' '.join([str(x)
-                                               for x in ghost_atoms])+'\n')
-
-    def add_guessp(self):
-        # Add the GUESSP keyword functions to the input object
-
-        self.scf_block.insert(-1, 'GUESSP\n')
-
-    def from_blocks(self, geom_block, bs_block, func_block, scf_block, title='Input generated by CRYSTALpytools'):
-        # Build the input from blocks
-        # All the blocks are list of strings or lists
-
-        self.geom_block = geom_block
-        self.bs_block = bs_block
-        self.func_block = func_block
-        self.scf_block = scf_block
-        self.title = [title+'\n']
+    For example, to set force convergence threshold of a optimization run:
 
-        if 'BASISSET\n' in self.bs_block:
-            self.is_basisset = True
+    Usage::
 
-        return self
+        obj = Crystal_input()
+        obj.geom.optgeom.toldeg(0.0001)
 
-    def from_file(self, input_name):
-        # input_name: name of the input file
+    In principle, by calling the 'block-like' attribute, a 'block-like' object
+    will be automatically generated if the attribute is empty. The exception is
+    the 3rd layer attributes, which must be set by ``set_attr()`` method. A
+    warning message is printed to indicate the name of the opened sub-block
+    since it usually does not correspond to CRYSTAL keywords to avoid potential
+    conflicts.
 
-        import sys
+    Usage::
 
-        self.name = input_name
+        obj.geom.freqcalc.set_preoptgeom()
+        obj.geom.freqcalc.optgeom.toldeg(0.0003)
 
-        try:
-            if input_name[-3:] != 'd12':
-                input_name = input_name+'.d12'
-            file = open(input_name, 'r')
-            data = file.readlines()
-            file.close()
-        except:
-            print('EXITING: a .d12 file needs to be specified')
-            sys.exit(1)
+    Methods and sub-blocks of ``Crystal_input`` usually have the same name as
+    corresponding keywords. One can setup, change or clean the keyword by
+    calling the corresponding method.
 
-        # The first line is the title
-        self.title = [data[0]]
+    Usage::
 
-        # Check is the basis set is a built in one
-        if 'BASISSET\n' in data:
-            end_index = []
-            if 'OPTGEOM\n' in data:
-                end_index = [i for i, s in enumerate(data) if 'END' in s]
-                end_index.insert(1, data.index('BASISSET\n')+1)
-            else:
-                end_index.append(data.index('BASISSET\n')-1)
-                end_index.append(data.index('BASISSET\n')+1)
-                end_index.extend([i for i, s in enumerate(
-                    data[end_index[1]:]) if 'END' in s])
-            self.is_basisset = True
-        else:
-            end_index = [i for i, s in enumerate(data) if 'END' in s]
-            self.is_basisset = False
+        obj.scf.toldee(9) # Set SCF TOLDEE = 9
+        obj.scf.toldee('') # Clean the TOLDEE keyword and value
+        obj.scf.ppan() # Print PPAN keyword, without value
 
-        self.geom_block = []
-        self.bs_block = []
-        self.func_block = []
-        self.scf_block = []
-
-        if len(end_index) == 4:
-            self.geom_block = data[1:end_index[0]+1]
-            self.bs_block = data[end_index[0]+1:end_index[1]+1]
-            self.func_block = data[end_index[1]+1:end_index[2]+1]
-            for i in range(end_index[2]+1, end_index[-1]):
-                self.scf_block.append(data[i])
-                '''if data[i+1][0].isnumeric():
-                    self.scf_block.append([data[i], data[i+1]])
-                else:
-                    if data[i][0].isalpha():
-                        self.scf_block.append(data[i])
-                    else:
-                        pass'''
-            # The loop cannot go over the last element
-            self.scf_block.append('ENDSCF\n')
-
-        elif len(end_index) == 5:
-            self.geom_block = data[:end_index[1]+1]
-            self.bs_block = data[end_index[1]+1:end_index[2]+1]
-            self.func_block = data[end_index[2]+1:end_index[3]+1]
-
-            for i in range(end_index[3]+1, end_index[-1]):
-                if data[i+1][0].isnumeric():
-                    self.scf_block.append([data[i], data[i+1]])
-                else:
-                    if data[i][0].isalpha():
-                        self.scf_block.append(data[i])
-                    else:
-                        pass
-            # The loop cannot go over the last element
-            self.scf_block.append('ENDSCF\n')
+    Though one can set CRYSTAL input object by manually setting up all the
+    attributes, it is also possible to read a template d12 file and do
+    modifications.
 
-        return self
+    Usage::
 
-    def opt_to_sp(self):
-        # Make an optgeom calculation into single_point
+        obj.from_file('opt.d12')
+        obj.geom.optgeom('') # Remove OPTGEOM block
+        obj.to_file('scf.d12') # Print it into file
 
-        if 'OPTGEOM\n' in self.geom_block:
-            init = self.geom_block.index('OPTGEOM\n')
-            final = self.geom_block.index('END\n')
-            del self.geom_block[init:final+1]
+    It is also possible to set individual blocks by a string. The ``set_block``
+    method should be used. The keyword for the block itself should not be
+    included.
 
-    def print_input(self):
-        # Print the whole input file
+    Usage::
 
-        if len(self.__dict__) > 0:
+        obj.scf.set_dft('SPIN\nEXCHANGE\nPBE\nCORRELAT\nP86\n')
 
-            blocks = [self.geom_block, self.bs_block,
-                      self.func_block, self.scf_block]
+    For basis set, it can be read from an external basis set file. '99 0' and
+    'END' should not be included.
 
-            if self.title is not None:
-                print(self.title[0][:-1])
-            else:
-                print('CRYSTALpytools generated input')
-            for block in blocks:
-                for line in block:
-                    if type(line) == list:
-                        print(line[0][:-1])
-                        print(line[1][:-1])
-                    else:
-                        print(line[:-1])
-        else:
-            print('The input is initialised, but the blocks were not defined')
+    Usage::
 
-    def remove_ghost(self):
-        # Remove ghost functions from the input object
+        obj.basisset.bs_from_file('mybasis.txt')
 
-        if 'GHOST\n' in self.bs_block:
-            del self.bs_block[-3:-1]
+    To examine the data in a block object, including Crystal_input obj itself,
+    call the ``data`` attribute.
 
-    def sp_to_opt(self, opt_options=[]):
-        # Make a single point calculation into an optgeom
-
-        if 'OPTGEOM\n' not in self.geom_block:
-            if self.is_basisset == True:
-                self.geom_block.append('OPTGEOM\n')
-                self.geom_block.extend(opt_options)
-                self.geom_block.append('END\n')
-            else:
-                self.geom_block.insert(-1, 'OPTGEOM\n')
-                for option in opt_options:
-                    self.geom_block.insert(-1, option)
-                self.geom_block.insert(-1, 'END\n')
-
-    def write_crystal_input(self, input_name, external_obj=None):
-        # Write a CRYSTAL input file (to file)
-
-        # input_name is the name of the imput that is going to be written (.d12)
-        # crystal_input is an object belonging to the crystal_input Class.
-        # external_obj is the ASE or pymatgen object that is going to be written in the gui file
+    Usage::
 
-        import itertools
-        import sys
-        from pymatgen.io.ase import AseAtomsAdaptor
-        from CRYSTALpytools.convert import cry_pmg2gui
+        obj.data
 
-        geom_block = self.geom_block
-        bs_block = self.bs_block
-        func_block = self.func_block
-        scf_block = self.scf_block
+    """
 
-        if self.title is None:
-            title = ['Input generated using CRYSTALpytools\n']
-        else:
-            title = self.title
+    def __init__(self):
+        super(Crystal_input, self).__init__()
 
-        # if there is an external object, we want to have the EXTERNAL
-        # keyword in the geom_block. If it's not present, this means
-        # adding it and keeping the rest of the input
-        if external_obj != None:
-            if 'EXTERNAL\n' not in geom_block:
-                new_geom_block = []
-                new_geom_block.append('EXTERNAL\n')
-                for i, line in enumerate(geom_block[2:]):
-                    if line.split()[0].replace('.', '', 1).isdigit() == False:
-                        for line1 in geom_block[i+2:]:
-                            new_geom_block.append(line1)
-                        break
-                geom_block = new_geom_block
-            if 'ase.atoms' in str(type(external_obj)):
-                # Transform into a pymatgen object to use the extra tools pymatgen has
-                external_obj = AseAtomsAdaptor().get_structure(external_obj)
-
-                gui_file_name = input_name[:-4]+'.gui'
-                gui_obj = cry_pmg2gui(external_obj)
-                gui_obj.write_crystal_gui(gui_file_name)
-
-            elif 'pymatgen.core' in str(type(external_obj)):
-
-                gui_file_name = input_name[:-4]+'.gui'
-                gui_obj = cry_pmg2gui(external_obj)
-                gui_obj.write_crystal_gui(gui_file_name)
+    def crystal_from_cif(self, file, symprec=0.01, angle_tolerance=5.0):
+        """
+        Read geometry from cif file and put infomation under 'CRYSTAL' keyword.
+        3D structure only. CIF files with a single geometry only.
 
-            else:
-                print(
-                    'EXITING: external object format not recognised, please specfy an ASE or pymatgen object')
-                sys.exit(1)
-
-        with open(input_name, 'w') as file:
-            cry_input = list(itertools.chain(title, geom_block, bs_block,
-                                             func_block, scf_block))
-            for line in cry_input:
-                file.writelines(line)
+        .. note::
+
+            Coordinates of corresponding atoms may not consistent with the
+            original CIF file, in which case coordinates of another symmetry
+            equivalent atom is used.
+
+            When multiple choices of periodic cell exist (typically for
+            low-symmetric non-orthgonal systems such as monoclinic or trilinic
+            cells), this method might lead to errors due to the inconsistent
+            choice of periodic cell between CRYSTAL and pymatgen.
+
+        Args:
+            file (str): CIF file name
+            symprec (float): If not none, finds the symmetry of the structure.
+                See `pymatgen.symmetry.analyzer.SpacegroupAnalyzer <https://pymatgen.org/pymatgen.symmetry.analyzer.html#pymatgen.symmetry.analyzer.SpacegroupAnalyzer>`_
+            angle_tolerance (float): See `pymatgen.symmetry.analyzer.SpacegroupAnalyzer <https://pymatgen.org/pymatgen.symmetry.analyzer.html#pymatgen.symmetry.analyzer.SpacegroupAnalyzer>`_
+        """
+        import numpy as np
+        from pymatgen.core.structure import IStructure
+        from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
+
+        struc = IStructure.from_file(file, primitive=True)
+        analyzer = SpacegroupAnalyzer(
+            struc, symprec=symprec, angle_tolerance=angle_tolerance)
+        struc_symm = analyzer.get_symmetrized_structure()
+
+        sg = analyzer.get_space_group_number()
+        latt = []
+        if sg >= 1 and sg < 3:  # trilinic
+            for i in ['a', 'b', 'c', 'alpha', 'beta', 'gamma']:
+                latt.append(round(
+                    getattr(struc_symm.lattice, i), 6
+                ))
+        elif sg >= 3 and sg < 16:  # monoclinic
+            for i in ['a', 'b', 'c', 'beta']:
+                latt.append(round(
+                    getattr(struc_symm.lattice, i), 6
+                ))
+        elif sg >= 16 and sg < 75:  # orthorhombic
+            for i in ['a', 'b', 'c']:
+                latt.append(round(
+                    getattr(struc_symm.lattice, i), 6
+                ))
+        elif sg >= 75 and sg < 143:  # tetragonal
+            for i in ['a', 'c']:
+                latt.append(round(
+                    getattr(struc_symm.lattice, i), 6
+                ))
+        elif sg >= 143 and sg < 168:  # trigonal
+            for i in ['a', 'alpha']:
+                latt.append(round(
+                    getattr(struc_symm.lattice, i), 6
+                ))
+        elif sg >= 168 and sg < 195:  # hexagonal
+            for i in ['a', 'c']:
+                latt.append(round(
+                    getattr(struc_symm.lattice, i), 6
+                ))
+        else:  # cubic
+            latt.append(round(struc_sym.lattice.a, 6))
+
+        natom = len(struc_symm.equivalent_sites)
+        eq_atom = int(len(struc_symm.species) / natom)
+        atominfo = []
+        for i in range(natom):
+            idx_eq = int(i * eq_atom)
+            atominfo.append([
+                int(struc_symm.species[idx_eq].Z),
+                round(struc_symm.equivalent_sites[i][0].frac_coords[0], 8),
+                round(struc_symm.equivalent_sites[i][0].frac_coords[1], 8),
+                round(struc_symm.equivalent_sites[i][0].frac_coords[2], 8)
+            ])
+
+        super(Crystal_input, self).geom.crystal(
+            IGR=sg, latt=latt, atom=atominfo)
+
+        return
 
 
 class Crystal_output:
     # This class reads a CRYSTAL output and generates an object
 
     def __init__(self):
         # Initialise the Crystal_output
@@ -256,27 +196,42 @@
             file = open(output_name, 'r', errors='ignore')
             self.data = file.readlines()
             file.close()
         except:
             print('EXITING: a .out file needs to be specified')
             sys.exit(1)
 
-        # Check the calculation converged
-        self.converged = False
+        # Check the calculation terminated correctly
+        self.terminated = False
 
         for i, line in enumerate(self.data[::-1]):
             if re.match(r'^ EEEEEEEEEE TERMINATION', line):
-                self.converged = True
+                self.terminated = True
                 # This is the end of output
                 self.eoo = len(self.data)-1-i
                 break
 
-        if self.converged == False:
+        if self.terminated == False:
             self.eoo = len(self.data)
 
+        # Check if the scf converged
+        self.converged = False
+        for line in self.data:
+            if re.match(r'^ == SCF ENDED - CONVERGENCE ON ENERGY', line):
+                self.converged = True
+                break
+
+        # Check if the geometry optimisation converged
+        self.opt_converged = False
+
+        for line in self.data[::-1]:
+            if bool(re.search('OPT END - CONVERGED', line) ) == True:
+                self.opt_converged = True
+                break
+        
         return self
 
     def get_dielectric_tensor(self):
 
         import re
 
         for i, line in enumerate(self.data):
@@ -552,20 +507,15 @@
         import numpy as np
         import sys
         from pymatgen.core.structure import Structure, Molecule
         from CRYSTALpytools.convert import cry_pmg2gui
 
         dimensionality = self.get_dimensionality()
 
-        # Check if the geometry optimisation converged
-        self.opt_converged = False
-        for line in self.data:
-            if re.match(r'^  FINAL OPTIMIZED GEOMETRY', line):
-                self.opt_converged = True
-                break
+        
 
         # Find the last geometry
         for i, line in enumerate(self.data):
             if re.match(r' TRANSFORMATION MATRIX PRIMITIVE-CRYSTALLOGRAPHIC CELL', line):
                 trans_matrix_flat = [float(x) for x in self.data[i+1].split()]
                 self.trans_matrix = []
                 for i in range(0, len(trans_matrix_flat), 3):
@@ -834,147 +784,144 @@
                 [int(x) for x in config_list[atom2_begin[i]+1:atom2_end[i]]])
 
         self.atom_type1 = atom_type1
         self.atom_type2 = atom_type2
 
         return [self.atom_type1, self.atom_type2]
 
-    """
-    Thermodynamic-specific attributes, including:
-        self.edft: get_qpoint, DFT total energy at central point, with probable
-                   corrections. Unit: KJ / mol cell
-        self.nqpoint: get_qpoint, Number of q points
-        self.qpoint: get_qpoint, Fractional coordinates of qpoints
-        self.nmode: get_mode, Number of vibrational modes at all qpoints
-        self.frequency: get_mode, Frequencies of all modes at all qpoints.
-                        Unit: THz
-        self.eigenvector: get_phonon_eigenvector, Eigenvectors (classical amplitude)
-                          of all atoms all modes at all qpoints. Unit: Angstrom
-    """
-
-    def check_freq_file(self):
+    def _check_freq_file(self):
         """
-        Not a standalone method. Check if the output is specified and if it is
-        a frequency output. The identifier:
-        +++ SYMMETRY ADAPTION OF VIBRATIONAL MODES +++
-
-        Input:
-            -
-        Output:
-            is_freq: bool, True if the identifier is found.
+        Check if the output is specified and if it is a frequency output. 
+
+        .. note::
+
+            The identifier:
+
+            +++ SYMMETRY ADAPTION OF VIBRATIONAL MODES +++
+
+        Returns:
+            is_freq (bool): True if the file is a frequency output file.
+
+        :raise Exception: If the output file is not specified
         """
         import re
-        import sys
 
         if not hasattr(self, 'data'):
-            print('ERROR: Output file not specified.')
-            sys.exit(1)
+            raise Exception('Output file not specified.')
 
         is_freq = False
 
         for line in self.data:
             if re.match(r'^\s*\+\+\+\sSYMMETRY\sADAPTION\sOF\sVIBRATIONAL\sMODES\s\+\+\+', line):
                 is_freq = True
                 break
             else:
                 continue
 
         return is_freq
 
-    def get_qpoint(self):
+    def get_q_info(self):
         """
-        Get the lattice information, DFT total energy and qpoints at which the
-        phonon frequency is calculated.
+        Get DFT total energy and coordinates and weights of q points (where 
+        phonon frequencies are calculated).
+
+        Returns:
+            self.edft (array[float]): Energy (in kJ/mol) reported in 'CENTERAL 
+                POINT' line (DFT + corrected energy)
+            self.nqpoint (int): Number of q points
+            self.qpoint (list[list[array[float], float]]): A nqpoint list of
+                2\*1 list whose first element is a 3\*1 array of q point
+                fractional coordinates and the second is its weight.
+
+        .. note::
+
+            ``self.edft`` is an array commensurate with the number of qpoints
+            to ensure the compatibility with QHA output. DFT+HA calculations
+            with various volumes generated by the QHA module make ``self.edft``
+            an array of different numbers. Otherwise, it is the array of same
+            numbers.
 
-        Note: edft is a list to make the script compatible with QHA output. The
-              sampled HA calculations in QHA output are recognized as HA
-              calculations at various qpoints.
-
-              For other cases, self.edft is an array of the same numbers,
-              corresponding to the number of qpoints.
-
-        Input:
-            -
-        Output:
-            self.edft, nqpoint * 1 array, DFT total energy. Unit: KJ / mol cell
-            self.nqpoint, int, Number of q points where the frequencies are
-                          calculated.
-            self.qpoint, nq * 3 numpy float array, Fractional coordinates of
-                         qpoints.
+        :raise Exception: If the output does not include the 'FREQCALC' section.
         """
         import re
         import numpy as np
-        import sys
 
-        is_freq = self.check_freq_file()
+        is_freq = self._check_freq_file()
         if not is_freq:
-            print('ERROR: Not a frequency output.')
-            sys.exit(1)
+            raise Exception('Not a frequency calculation.')
 
         edft = np.array([], dtype=float)
         self.nqpoint = 0
-        self.qpoint = np.array([], dtype=float)
+        self.qpoint = []
 
         for i, line in enumerate(self.data):
             # Keywords in gradient calculation
             if re.match(r'\s*CENTRAL POINT', line):
                 edft = np.append(edft, units.H_to_kjmol(
                     float(line.strip().split()[2])))
 
             if re.search(r'EXPRESSED IN UNITS\s*OF DENOMINATOR', line):
                 shrink = int(line.strip().split()[-1])
 
 # Keywords in dipersion calculation
             if re.match(r'\s*DISPERSION K POINT NUMBER', line):
                 coord = np.array(line.strip().split()[7:10], dtype=float)
-                self.qpoint = np.append(self.qpoint, coord / shrink)
+                weight = float(line.strip().split()[-1])
+                self.qpoint.append([coord / shrink, weight])
                 self.nqpoint += 1
 
 # HA Gamma point calculation
         if self.nqpoint == 0 and len(edft) == 1:
             self.nqpoint = 1
-            self.qpoint = np.array([[0, 0, 0]], dtype=float)
+            self.qpoint = [[np.array([0, 0, 0], dtype=float), 1.]]
             self.edft = edft
 # QHA Gamma point calculation
         elif self.nqpoint == 0 and len(edft) > 1:
             self.nqpoint = len(edft)
-            self.qpoint = np.array([[0, 0, 0]
-                                   for i in range(self.nqpoint)], dtype=float)
+            for i in range(self.nqpoint):
+                self.qpoint.append(
+                    [np.array([0, 0, 0], dtype=float), 1.]
+                )
             self.edft = edft
 # HA dispersion calculation
         elif self.nqpoint > 0 and len(edft) == 1:
-            self.qpoint = np.reshape(self.qpoint, (-1, 3))
-            self.edft = edft
+            for i in range(self.nqpoint):
+                self.qpoint[i][1] /= self.nqpoint
+            self.edft = np.array([edft[0] for i in range(self.nqpoint)], dtype=float)
         else:
-            print(
-                'ERROR: Only support: 1. HA, Gamma point 2. QHA, gamma point 3. HA dispersion.')
-            sys.exit(1)
+            raise Exception('Only support: 1. HA, Gamma point 2. QHA, gamma point 3. HA dispersion.')
 
         return self.edft, self.nqpoint, self.qpoint
 
     def get_mode(self):
         """
-        Get corresponding vibrational frequencies and for all modes and
-        compute the total number of vibration modes (natoms * 3).
+        Get the number of modes at all q points and corresponding vibrational
+        frequencies and intensities.
 
-        Input:
-            -
-        Output:
-            self.nmode, nqpoint * 1 numpy int array, Number of vibration modes
-                        at each qpoints.
-            self.frequency: nqpoint * nmode numpy float array, Harmonic
-                            vibrational frequency. Unit: THz
+        Returns:
+            self.nmode (array[int]): Number of modes at q point.
+            self.frequency (array[float]): nqpoint \* nmode array of vibrational
+                frequency. Unit: THz
+            self.intens (array[float]): nqpoint \* nmode array of harmonic
+                intensiy. Unit: km/mol
+            self.IR (array[bool]): nqpoint \* nmode array of boolean values
+                specifying whether the mode is IR active
+            self.Raman (array[bool]): nqpoint \* nmode array of boolean values
+                specifying whether the mode is Raman active
         """
         import numpy as np
         import re
 
         if not hasattr(self, 'nqpoint'):
-            self.get_qpoint()
+            self.get_q_info()
 
         self.frequency = np.array([], dtype=float)
+        self.intens = np.array([], dtype=float)
+        self.IR = np.array([], dtype=bool)
+        self.Raman = np.array([], dtype=bool)
 
         countline = 0
         while countline < len(self.data):
             is_freq = False
             if re.match(r'\s*DISPERSION K POINT NUMBER\s*\d',
                         self.data[countline]):
                 countline += 2
@@ -982,45 +929,58 @@
 
             if re.match(r'\s*MODES\s*EIGV\s*FREQUENCIES\s*IRREP',
                         self.data[countline]):
                 countline += 2
                 is_freq = True
 
             while self.data[countline].strip() and is_freq:
-                line_data = re.findall(r'\-*[\d\.]+[E\d\-\+]*',
-                                       self.data[countline])
-                if line_data:
-                    nm_a = int(line_data[0].strip('-'))
-                    nm_b = int(line_data[1])
-                    freq = float(line_data[4])
+                line_data = self.data[countline].split()
+                nm_a = int(line_data[0].strip('-'))
+                nm_b = int(line_data[1])
+                freq = float(line_data[4])
+                has_spec = False
+                # IR/Raman analysis, closed by default in dispersion calcs
+                if 'A' in line_data or 'I' in line_data:
+                    has_spec = True
+                    intens = float(line_data[-2].strip(')'))
+                    IR = line_data[-4] == 'A'
+                    Raman = line_data[-1] == 'A'
+                    if (nm_b-nm_a == 1):
+                        intens = intens/2
+                    elif(nm_b-nm_a == 2):
+                        intens = intens/3
 
                 for mode in range(nm_a, nm_b + 1):
                     self.frequency = np.append(self.frequency, freq)
+                    if has_spec:
+                        self.intens = np.append(self.intens, intens)
+                        self.IR = np.append(self.IR, IR)
+                        self.Raman = np.append(self.Raman, Raman)
 
                 countline += 1
 
             countline += 1
 
         self.frequency = np.reshape(self.frequency, (self.nqpoint, -1))
         self.nmode = np.array([len(i) for i in self.frequency], dtype=int)
 
-        return self.nmode, self.frequency
+        if has_spec:
+            self.intens = np.reshape(self.intens, (self.nqpoint, -1))
+            self.IR = np.reshape(self.IR, (self.nqpoint, -1))
+            self.Raman = np.reshape(self.Raman, (self.nqpoint, -1))
+
+        return self.nmode, self.frequency, self.intens, self.IR, self.Raman
 
     def get_phonon_eigenvector(self):
         """
-        Get corresponding mode eigenvectors for all modes on all
-        atoms in the supercell.
+        Get corresponding mode eigenvectors.
 
-        Input:
-            -
-        Output:
-            self.eigenvector, nqpoint * nmode * natom * 3 numpy float array,
-                              Eigenvectors expressed in Cartesian coordinate,
-                              at all atoms, all modes and all qpoints.
-                              Classical amplitude. Unit: Angstrom
+        Returns:
+            self.eigenvector (array[float]): nqpoint\*nmode\*natom\*3 array of 
+                eigenvectors. Normalized to 1.
         """
         import numpy as np
         import re
 
         if not hasattr(self, 'nmode'):
             self.get_mode()
 
@@ -1091,40 +1051,38 @@
         return self.eigenvector
 
     def clean_imaginary(self):
         """
         Substitute imaginary modes and corresponding eigenvectors with numpy
         NaN format and print warning message.
 
-        Input:
-            -
-        Output:
-            cleaned attributes.
-            self.frequency
-            self.eigenvector
+        Returns:
+            self.frequency (array[float])
+            self.eigenvector (array[float])
         """
         import numpy as np
         import warnings
 
         for q, freq in enumerate(self.frequency):
-            if freq[0] > -1e-4:
+            if freq[0] > -1e-4 or np.isnan(freq[0]):
                 continue
 
             warnings.warn(
                 'Negative frequencies detected - Calculated thermodynamics might be inaccurate. Negative frequencies will be substituted by NaN.',
                 stacklevel=2
             )
 
             neg_rank = np.where(freq <= -1e-4)[0]
             self.frequency[q, neg_rank] = np.nan
 
             if hasattr(self, 'eigenvector'):
-                natom = int(self.nmode[q] / 3)
-                nan_eigvt = np.full([natom, 3], np.nan)
-                self.eigenvector[q, neg_rank] = nan_eigvt
+                if len(self.eigenvector) != 0:
+                    natom = int(self.nmode[q] / 3)
+                    nan_eigvt = np.full([natom, 3], np.nan)
+                    self.eigenvector[q, neg_rank] = nan_eigvt
 
         if hasattr(self, 'eigenvector'):
             return self.frequency, self.eigenvector
         else:
             return self.frequency
 
     def get_elatensor(self):
```

### Comparing `CRYSTALpytools-2023.4.4/CRYSTALpytools/execute.py` & `CRYSTALpytools-2023.6.6/CRYSTALpytools/execute.py`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.4.4/CRYSTALpytools/plot.py` & `CRYSTALpytools-2023.6.6/CRYSTALpytools/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -3153,15 +3153,16 @@
         return poisson_avg
     if poisson_choice == "min":
         return poisson_min
     if poisson_choice == "max":
         return poisson_max
 
 
-def plot_cry_ela(choose, ndeg, *args):
+def plot_cry_ela(choose, ndeg, *args, dpi=200, filetype=".png",
+                 transparency=False):
 
     import numpy as np
     import matplotlib.pyplot as plt
     import math
     import time
     import sys
     from mpl_toolkits.mplot3d import axes3d, Axes3D
@@ -3255,15 +3256,15 @@
         ax.set_ylabel("Y")
         ax.set_zlabel("Z")
 
         ax.set_box_aspect(aspect=(1, 1, 1))  # Fix aspect ratio
 
         plt.show()
         fig.savefig(choose + time.strftime("%Y-%m-%d_%H%M%S") +
-                    ".jpg", dpi=200)
+                    filetype, dpi=dpi, transparent=transparency)
 
         # <--
 
 
 def save_plot(path_to_file):
 
     from os import path
```

### Comparing `CRYSTALpytools-2023.4.4/CRYSTALpytools/thermodynamics.py` & `CRYSTALpytools-2023.6.6/CRYSTALpytools/thermodynamics.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,81 +1,63 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-A comprehensive module for lattice dynamics based on harmonic and quasiharmonic
-approximations.
+A post-processing module for DFT lattice dynamics by harmonic and quasiharmonic
+approximations (HA/QHA).
 """
 from CRYSTALpytools.crystal_io import Crystal_output
 from CRYSTALpytools import units
 
 
 class Mode:
     """
-    Class Mode - store important information for a given vibrational mode. Can
-    be used for a single harmonic phonon calculation and multiple calculations
-    on the same system.
-
-    Initialization:
-        self.rank, __init__, The rank of the mode object. Start from 1.
-        self.ncalc, __init__, The number of harmonic frequency calculations.
-        self.frequency, __init__, Frequencies of the mode. Unit: THz
-        self.volume, __init__, Cell volumes of harmonic calculations.
-                     Unit: Angstrom^3
-        self.eigenvector, __init__, Corresponding eigenvectors. Unit: Angstrom
-
-    Limited to ncalc = 1 cases:
-        self.zp_energy, get_zp_energy, Zero point energy of the mode.
-                        Unit: KJ/mol cell
-        self.U_vib, get_U_vib, Vibration contribution to internal energy,
-                    including zero-point energy. Unit: KJ/mol cell
-        self.entropy, get_entropy, Entropy of the mode. Unit: J/mol cell*K
-        self.C_v, get_C_v, Constant volume specific heat. Unit: J/mol cell*K
-
-    Limited to ncalc > 1 cases:
-        self.poly_fit, polynomial_fit, dictionary of numpy polynomial objects.
-                       Key: orders of power, Value: fitted polynomials
-        self.poly_fit_rsqaure, polynomial_fit, dictionary of the goodness o
-                               fittings, characterized by R^2.
+    Store important information for a given vibrational mode and do analysis at
+    mode-level. Not recommanded to be used individually.
+
+    Args:
+        rank (int): The rank of the mode object, from 1.
+        frequency (array[float] | list[float]): Frequencies of the mode
+            (Ncalc\*1). Unit: THz. Note: **NOT** angular frequency, which is 
+            frequency * 2pi.
+        volume (array[float] | list[float]): Lattice volumes of harmonic
+            calculations (Ncalc\*1). Unit: Angstrom^3
+        eigenvector (array[float] | list[float]): Corresponding normalized 
+            eigenvectors (Ncalc\*Natom\*3).
+
+    Returns:
+        self.rank (int)
+        self.ncalc (int): The number of harmonic calculations (typically at
+            different volumes)
+        self.frequency (array[float])
+        self.volume (array[float])
+        self.eigenvector (array[float])
     """
 
     def __init__(self, rank=0, frequency=[], volume=[], eigenvector=[]):
-        """
-        Input:
-            rank, int, The rank of the mode object, from 1.
-            frequency, ncalc * 1 array / list, Frequencies of the mode.
-                       Unit: THz. Note: Not angular frequency, which is
-                       frequency * 2pi
-            volume, ncalc * 1 array / list, Lattice volumes of harmonic
-                    calculations. Unit: Angstrom^3
-            eigenvector, ncalc * natom * 3 array / list, Corresponding
-                         eigenvectors. Unit: Angstrom
-        Output:
-            self.rank
-            self.ncalc, int, The number of harmonic calculations
-            self.frequency
-            self.volume
-            self.eigenvector
-        """
         import numpy as np
 
         self.rank = rank
         self.ncalc = len(frequency)
         self.frequency = np.array(frequency, dtype=float)
         self.volume = np.array(volume, dtype=float)
         self.eigenvector = np.array(eigenvector, dtype=float)
 
     def get_zp_energy(self):
         """
-        Get the zero-point energy of a single mode. Limited to ncalc = 1 cases.
+        Get the zero-point energy of a single mode with the following equation. 
+        Limited to ncalc = 1 cases.
+
+        .. math::
+
+            E^{zp}_{i,\\mathbf{q}}=\\frac{1}{2}\\hbar\\omega_{i,\\mathbf{q}}
 
-        Input:
-            -
-        Output:
-            self.zp_energy, float, Zero-point energy of a given mode.
-                            Unit: KJ/mol cell
+        Returns:
+            self.zp_energy (float): Zero-point energy. Unit: KJ/mol
+
+        :raise Exception: If ``self.ncalc`` > 1.
         """
         import numpy as np
         import scipy.constants as scst
 
         if self.ncalc > 1:
             raise Exception(
                 'This module is limited to a single frequency calculation.')
@@ -83,23 +65,34 @@
         hbar_freq = self.frequency[0] * scst.Avogadro * scst.h * 1e9
         self.zp_energy = 0.5 * hbar_freq
 
         return self.zp_energy
 
     def get_U_vib(self, temperature=298.15):
         """
-        Get the vibration contribution to internal energy of a single mode.
-        Limited to ncalc = 1 cases. U_vib includes zero-point energy.
+        Get the vibration contribution to internal energy (including zero-point
+        energy) of a single mode with the following equation. Limited to 
+        ncalc = 1 cases.
+
+        .. math::
 
-        Input:
-            temperature: float, the temperature where the thermal contribution
-                         is computed.
-        Output:
-            self.U_vib, float, Vibration contribution to internal energy of a
-                        given mode. Unit: KJ/mol cell
+            U^{vib}_{i,\\mathbf{q}}\\left(T\\right)=E^{zp}_{i,\\mathbf{q}}+
+            \\frac{\\hbar\\omega_{i,\\mathbf{q}}}{\\exp{\\left(
+                \\frac{\\hbar\\omega_{i,\\mathbf{q}}}{k_{B}T}
+            \\right)}-1}
+
+        Args:
+            temperature (float, optional): Temperature where the quantity is 
+                computed. Unit: K
+
+        Returns:
+            self.U_vib (float): Vibration contribution to internal energy. 
+                Unit: KJ/mol
+
+        :raise Exception: If ``self.ncalc`` > 1.
         """
         import numpy as np
         import scipy.constants as scst
 
         if self.ncalc > 1:
             raise Exception(
                 'This module is limited to a single frequency calculation.')
@@ -116,22 +109,38 @@
         expon = np.exp(hbar_freq / kb_t)
         self.U_vib = self.zp_energy + hbar_freq / (expon - 1)
 
         return self.U_vib
 
     def get_entropy(self, temperature):
         """
-        Get the entropy of a single mode. Limited to ncalc = 1 cases.
+        Get the entropy of a single mode with the following equation. Limited
+        to ncalc = 1 cases.
+
+        .. math::
 
-        Input:
-            temperature: float, the temperature where the thermal contribution
-                         is computed.
-        Output:
-            self.entropy, float, The entropy of a given mode.
-                          Unit: J/mol cell*K
+            S_{i,\\mathbf{q}}\\left(T\\right)=k_{B}\\left\\{
+                \\frac{\\hbar\\omega_{i,\\mathbf{q}}}{k_{B}T\\left[
+                    \\exp{\\left(
+                        \\frac{\\hbar\\omega_{i,\\mathbf{q}}}{k_{B}T}
+                    \\right)}-1
+                \\right]}-\\ln{\\left[
+                    1-\\exp{\\left(
+                        -\\frac{\\hbar\\omega_{i,\\mathbf{q}}}{k_{B}T}
+                    \\right)}
+                \\right]}
+            \\right\\}
+
+        Args:
+            temperature (float, optional): Unit: K
+
+        Returns:
+            self.entropy (float): Entropy. Unit: J/mol\*K
+
+        :raise Exception: If ``self.ncalc`` > 1.
         """
         import numpy as np
         import scipy.constants as scst
 
         if self.ncalc > 1:
             raise Exception(
                 'This module is limited to a single frequency calculation.')
@@ -146,23 +155,39 @@
         entS = kb_t * (hbar_freq / kb_t / (expon - 1) - np.log(1 - 1 / expon))
         self.entropy = entS / temperature
 
         return self.entropy
 
     def get_C_v(self, temperature):
         """
-        Get the constant volume specific heat of a single mode. Limited to
-        ncalc = 1 cases.
+        Get the constant volume specific heat of a single mode with the 
+        following equation. Limited to ncalc = 1 cases.
+
+        .. math::
 
-        Input:
-            temperature: float, the temperature where the thermal contribution
-                         is computed.
-        Output:
-            self.C_v, float, The constant volume specific heat of a given mode.
-            Unit: J/mol cell*K
+            C^{V}_{i,\\mathbf{q}}=
+            \\frac{\\left(\\hbar\\omega_{i,\\mathbf{q}}\\right)^{2}}{k_{B}T^{2}}
+            \\frac{\\exp{
+            \\left(
+                \\frac{\\hbar\\omega_{i,\\mathbf{q}}}{k_{B}T}
+            \\right)}
+            }{\\left[
+                \\exp{\\left(
+                    \\frac{\\hbar\\omega_{i,\\mathbf{q}}}{k_{B}T}
+                \\right)-1}
+            \\right]^{2}
+            }
+
+        Args:
+            temperature (float, optional): Unit: K
+
+        Returns:
+            self.C_v (float): Constant volume specific heat. Unit: J/mol\*K
+
+        :raise Exception: If ``self.ncalc`` > 1.
         """
         import numpy as np
         import scipy.constants as scst
 
         if self.ncalc > 1:
             raise Exception(
                 'This module is limited to a single frequency calculation.')
@@ -180,24 +205,27 @@
         return self.C_v
 
     def polynomial_fit(self, eq_point, order=[2, 3]):
         """
         Fit phonon frequency as the polynomial function of volume with
         perturbation theory. Limited to ncalc > 1 cases.
 
-        Input:
-            eq_point, int, The DFT total energy minimum point with equilibrium
-                           volume
-            order, norder * 1 list, The orders of polynomials to be fitted.
-        Output:
-            self.poly_fit, norder * 1 dictionary, the dictionary of numpy
-                           polynomial objects. Key: orders of power, Value:
-                           fitted polynomials
-            self.poly_fit_rsquare, norder * 1 dictionary, the dictionary of the
-                                   goodness of fittings, characterized by R^2.
+        Args:
+            eq_point (int): The index (not rank) corresponds to the DFT total
+                energy minimum (typically the unstrained geometry).
+            order (array[int] | list[int]], optional): Orders of
+                polynomials used.
+
+        Returns:
+            self.poly_fit (Dict[int, NumPy Polynomial]): Key - orders of power, 
+                Value - fitted NumPy polynomials
+            self.poly_fit_rsquare (Dict[int, float]): Key - orders of power, 
+                Value - goodness of fittings, characterized by R^2.
+
+        :raise Exception: If ``self.ncalc`` <= 1.
         """
         import numpy as np
         import warnings
 
         if self.ncalc <= 1:
             raise Exception(
                 'This modulus is limited to multiple frequency calculations.')
@@ -230,62 +258,42 @@
             self.poly_fit_rsqaure.update({i: r_square})
 
         return order, self.poly_fit, self.poly_fit_rsqaure
 
 
 class Harmonic(Crystal_output):
     """
-    Class Harmonic, inherited from the Crystal_output class, with thermodynamic
+    Inherited from the Crystal_output class and has thermodynamic-specific 
     attributes. Used for harmonic phonon calclulations. Harmonic object can be
     defined by either a harmonic phonon calculation output file or manually set
     the all the information (usually for QHA).
 
-    Inherited attributes:
-        self.edft (length should be 1)
-        self.nqpoint
-        self.qpoint
-        self.nmode
-        self.frequency
-        self.eigenvector
-
-    New attributes:
-        self.strucrure, The pymatgen Structure object of the calculation cell.
-        self.mode, The list of mode objects.
-        self.temperature, The temperature range for HA thermodynamics.
-        self.pressure, The pressure range for HA thermodynamics.
-        self.helmholtz, Helmholtz free energy of the cell, at HA level.
-                        Unit: KJ/mol cell
-        self.gibbs, Gibbs free energy of the cell, at HA level.
-                    Unit: KJ/mol cell
-        * Following attributes are the summed up values of corresponding
-          attributes of class Mode.
-        self.U_vib, thermodynamics
-        self.zp_energy, thermodynamics
-        self.entropy, thermodynamics
-        self.C_v, thermodynamics
+    Args:
+        temperature (array[float] | list[float], optional): Temperatures
+            where thermodynamic properties are computed. Unit: K
+        pressure (array[float] | list[float], optional): Pressures where
+            the thermodyanmic properties are calculated. Unit: GPa
+        write_out (bool, optional): Wheter to print out HA thermodynamic 
+            properties in a separate text file.
+        filename (str, optional): Name of the printed-out file, valid if
+            ``write_out`` = True.
+
+    **Note**
+
+    Temperatures and pressures can also be defined by ``self.thermodynamics``,
+    whose entries always cover the entries here.
+
+    Usage::
+
+        ha = Harmonic(temperature=[0, 100, 200, 300], pressure=[0.,])
+        ha.from_file('harmonic_phonon.out')
     """
 
     def __init__(self, temperature=[], pressure=[],
                  write_out=True, filename='HA-thermodynamics.dat'):
-        """
-        Initialization.
-
-        Input:
-            temperature, nTempt * 1 array / list, Temperatures where the
-                         thermodynamic properties are computed. Unit: K
-            pressure, npress * 1 array / list, Pressures where the
-                      thermodyanmic properties are calculated. Unit: GPa
-            write_out, bool, Wheter to print out HA thermodynamic properties.
-            filename, str, Name of the printed-out file, used only if
-                      write_out = True.
-        Note: Temperature can also be defined in 'thermodynamics' method, which
-              will cover the settings during initialisation.
-        Output: 
-            -
-        """
         import numpy as np
 
         if len(temperature) > 0:
             self.temperature = np.array(temperature, dtype=float)
 
         if len(pressure) > 0:
             self.pressure = np.array(pressure, dtype=float)
@@ -295,167 +303,130 @@
             self.filename = filename
         else:
             self.filename = 'no file'
 
     def from_file(self, output_name, scelphono=[], read_eigenvector=False,
                   auto_calc=True):
         """
-        Generate the Harominc object from a HA file.
+        Generate the Harominc object from a HA output file.
 
-        Input:
-            output_name, str, Name of the output file.
-            scellphono, ndimension * ndimension list, Supercell manipulation
-                        matrix used for vibrational properties. Should be the
-                        same as 'SCELPHONO' keyword in CRYSTAL input file. 3x3
-                        list is also allowed.
-            read_eigenvector, bool, Whether reading eigenvectors, i.e.,
-                              normalised modes from outputs.
-            auto_calc, bool, Whether to automatically launch thermodynamic
-                       calculations. Parameters defined during initialization
-                       will be used.
-        Output:
-            self.strucrure, pymatgen Structure object, the calculation cell,
-                            reduced by SCELPHONO.
-            self.natom, int, The number of atoms in the reduced calculation cell.
-            self.volume, float, The volume the reduced calculation cell.
-            self.mode, nqpoint * nmode array, List of mode objects at all
-                       qpoints.
+        Args:
+            output_name (str): Name of the output file.
+            scellphono (array[float] | list[float], optional):
+                Supercell manipulation matrix used for vibrational properties. 
+                Should be the same as 'SCELPHONO' keyword in CRYSTAL input file.
+                By default a 1\*1\*1 'SCELPHONO' is assumed.
+            read_eigenvector (bool, optional): Whether to read eigenvectors from
+                the output.
+            auto_calc (bool, optional): Whether to automatically launch
+                thermodynamic calculations. Parameters defined during
+                initialization will be used.
+
+        Returns:
+            self.strucrure (PyMatGen Structure): Cell reduced by SCELPHONO.
+            self.natom (int): Number of atoms in the reduced cell.
+            self.volume (float): Volume of the reduced cell. Unit: Angstrom^3
+            self.mode (list[Mode]): List of mode objects at all the qpoints.
+
+        :raise Exception: If computational data is stored in the object.
+        :raise Exception: If a QHA output file is read.
         """
         import numpy as np
         from CRYSTALpytools.thermodynamics import Mode
 
         if hasattr(self, "volume"):
             raise Exception(
-                "Data exists. Cannot overwriting the existing data.")
+                "Data exists. Cannot overwrite the existing data.")
 
         super(Harmonic, self).read_cry_output(output_name)
         super(Harmonic, self).get_mode()
-        super(Harmonic, self).clean_imaginary()
         self._generate_structure(scelphono=scelphono)
 
-        if len(self.edft) != 1:
+        if len(np.unique(self.edft)) != 1:
             raise Exception(
-                "Only a single frequency calculation is premitted.")
+                "Only the frequency calculations at constant volumes are premitted.")
         else:
             self.edft = self.edft[0]
 
         # Transfer the modes in self.freqency into lists of mode objects
         if read_eigenvector:
             super(Harmonic, self).get_phonon_eigenvector()
         else:
             self.eigenvector = []
 
-        self.from_frequency(self.edft, self.qpoint, self.frequency, self.eigenvector,
-                            structure=self.structure)
+        self.from_frequency(self.edft, self.qpoint, self.frequency, self.eigenvector)
 
         if auto_calc:
             self.thermodynamics(sumphonon=True)
             self.print_results()
 
         return self
 
-    def from_mode(self, edft, mode, **geometry):
+    def from_frequency(self, edft, qpoint, frequency, eigenvector, **kwargs):
         """
-        Generate a Harmonic object by specifying data. Not recommanded to be
-        used as a standalone method.
-
-        Input:
-            edft: float, Electron total energy
-            mode: nqpoint * nmode array, List of mode objects.
-            structure: Optional, Pymatgen structure object
-            natom: Optional, int, number of atoms
-            volume: Optional, float, volume of the simulation cell.
-                    Unit Angstrom^3
-        Output:
-            self.nqpoint, int, Number of qpoints.
-            self.nmode, nqpoint * 1 array, Number of modes at each q point.
-            self.mode, nqpoint * nmode array, List of mode objects at Gamma.
-            self.structure, pymatgen Structure object, the calculation cell,
-                            reduced by SCELPHONO.
-            self.natom, int, Number of atoms in the reduced calculation cell.
-            self.volume, float, The volume the reduced calculation cell.
-        """
-        import numpy as np
-
-        if hasattr(self, "volume"):
-            raise Exception(
-                "Data exists. The current command will be ignored.")
-
-        for key, value in geometry.items():
-            if key == 'structure':
-                self.structure = value
-                self.natom = len(value.species)
-                self.volume = value.lattice.volume
-                break
-            elif key == 'natom':
-                self.natom = int(value)
-            elif key == 'volume':
-                self.volume = float(value)
-
-        self.edft = edft
-        self.mode = mode
-        self.nqpoint = len(mode)
-        self.nmode = np.array([len(q) for q in self.mode])
+        Generate a Harmonic object by specifying frequency and eigenvector and
+        clean imaginary frequencies.
 
-        return self
-
-    def from_frequency(self, edft, qpoint, frequency, eigenvector, **geometry):
-        """
-        Generate a Harmonic object by specifying frequency and eigenvector. 
         Not recommanded to be used as a standalone method.
 
-        Input:
-            edft: float, Electron total energy
-            qpoint: nqpoint * 3 array, Fractional coordinates of qpoint
-            frequency: nqpoint * nmode array, Array of frequencies. Unit: THz
-            eigenvector: nqpoint * nmode * natom * 3 array / list, Corresponding
-                         normalized eigenvectors. 
-            structure: Optional, Pymatgen structure object
-            natom: Optional, int, number of atoms
-            volume: Optional, float, volume of the simulation cell.
-                    Unit Angstrom^3
-        Output:
-            self.nqpoint, int, Number of qpoints.
-            self.nmode, nqpoint * 1 array, Number of modes at each q point.
-            self.mode, nqpoint * nmode array, List of mode objects at Gamma.
-            self.structure, pymatgen Structure object, the calculation cell,
-                            reduced by SCELPHONO.
-            self.natom, int, Number of atoms in the reduced calculation cell.
-            self.volume, float, The volume the reduced calculation cell.
+        Args:
+            edft (float): Electron total energy
+            qpoint (list[list[array[float], float]]): Fractional coordinate 
+                and weight of qpoint
+            frequency (array[float]): Array of frequencies. Unit: THz
+            eigenvector (array[float]): Normalized eigenvectors. 
+            structure (PyMatGen Structure, optional)
+            natom (int, optional)
+            volume (float, optional)
+
+        **Note**: The user should define either 'structure' or 'natom' + 'volume'.
+
+        Returns:
+            self.nqpoint (int)
+            self.nmode (array[int])
+            self.mode (list[Mode])
+            self.structure (PyMatGen Structure, optional)
+            self.natom (int)
+            self.volume (float)
+
+        :raise Exception: If computational data is stored in the object.
+        :raise Exception: If the 1st dimension (nqpoint) of ``qpoint`` and ``frequency`` are not consistent.
+        :raise Exception: If the 2nd dimension (nfreq) of ``frequency`` and ``eigenvector`` are not consistent and ``eigenvector`` is not ``[]``.
         """
         import numpy as np
 
-        if hasattr(self, "volume"):
+        if hasattr(self, "mode"):
             raise Exception(
                 "Data exists. The current command will be ignored.")
 
-        for key, value in geometry.items():
+        for key, value in kwargs.items():
             if key == 'structure':
                 self.structure = value
                 self.natom = len(value.species)
                 self.volume = value.lattice.volume
                 break
             elif key == 'natom':
                 self.natom = int(value)
             elif key == 'volume':
                 self.volume = float(value)
 
-        if np.size(qpoint, 0) != np.size(frequency, 0):
+        if len(qpoint) != np.size(frequency, 0):
             raise Exception(
                 "The 1st dimension (n qpoint) of 'qpoint' and 'frequency' are not consistent.")
         if len(eigenvector) != 0 and np.size(eigenvector, 1) != np.size(frequency, 1):
             raise Exception(
                 "The 2nd dimension (n mode) of 'frequency' and 'eigenvector' are not consistent.")
 
         self.edft = edft
-        self.nqpoint = np.size(qpoint, 0)
+        self.nqpoint = len(qpoint)
         self.qpoint = qpoint
         self.frequency = frequency
         if len(eigenvector) != 0:
             self.eigenvector = eigenvector
+        super(Harmonic, self).clean_imaginary()
 
         # Transfer the modes in self.freqency into lists of mode objects
         self.mode = []
         for q, qpoint_freq in enumerate(frequency):
             qmode = []
             for m, mode_freq in enumerate(qpoint_freq):
                 if len(eigenvector) != 0:
@@ -474,25 +445,25 @@
         self.nmode = np.array([len(q) for q in self.mode])
 
         return self
 
     def _generate_structure(self, scelphono):
         """
         Eliminate the influences of the keyword 'SCELPHONO' and generate the
-        pymatgen 'structure' object of the actual cell used for phonon
+        PyMatGen Structure object of the actual cell used for phonon 
         calculation. Not a standalone method.
 
-        Input:
-            scellphono, ndimension * ndimension list. 3*3 list is also allowed.
-        Output:
-            self.structure, pymatgen Structure object. The calculation cell
-                            without 'SCELPHONO' expansion.
-            self.natom, int, Number of atoms in the cell.
-            self.volume, float, pymatgen structure.volume. Cell volume.
-                         Unit: Angstrom^3
+        Args:
+            scellphono (list[int] | array[int]): ndimension\*ndimension or 
+                3\*3 matrix corresponds to the 'SCELPHONO' keyword.
+
+        Returns:
+            self.structure (PyMatGen Structure)
+            self.natom (int)
+            self.volume (float)
         """
         from CRYSTALpytools.convert import cry_out2pmg
         from pymatgen.core.structure import Structure
         import numpy as np
 
         ndimen = self.get_dimensionality()
 
@@ -533,45 +504,43 @@
         self.volume = self.structure.volume
 
         return self
 
     def _phonon_sumup(self, temperature, calculate_zp):
         """
         Summing up inidival phonon modes at each q point. Translational modes
-        with frequencies = 0 are skipped.
-
-        Not a standalone method. For thermodynamics, use 'self.thermodyanmics'
+        with frequencies = 0 are skipped. Not a standalone method. For 
+        thermodynamics, use 'self.thermodyanmics'
         instead.
 
-        Input:
-            temperature, float, The temperature where the U_vib, entropy and
-                         C_v are calculated.
-            calculate_zp, bool, Calculate zero-point energy or temperature
-                          dependent properties.
-        Output:
-            zp_energy, nqpoint * 1 array, Zero-point energy at a given q point.
-                       Returned if temperature = None.
-            U_vib, nqpoint * 1 array, Vibrational contribution to internal
-                   energy at constant temperature and all q points. Returned
-                   if temperature is given.
-            entropy, nqpoint * 1 array, Entropy at constant temperature and
-                     given q point. Returned if temperature is given.
-            C_v, nqpoint * 1 array, Constant volume specific heat at constant
-                 temperature and given q point. Returned if temperature is
-                 given.
+        Args:
+            temperature (float)
+            calculate_zp (bool): Calculate zero-point energy or temperature
+                dependent properties.
+
+        Returns:
+            zp_energy (array[float]): Zero-point energy at a q point. Returned
+                if ``calculate_zp = True``.
+            U_vib (array[float]): Vibrational contribution to internal energy 
+                at constant temperature and a q point. Returned if 
+                ``calculate_zp = False``.
+            entropy (array[float]): Entropy at constant temperature and a q 
+                point. Returned if ``calculate_zp = False``.
+            C_v (array[float]): Constant volume specific heat at constant
+                 temperature and a q point. Returned if ``calculate_zp = False``.
         """
         import numpy as np
 
         if calculate_zp:
-            zp_energy = np.array([], dtype=float)
+            zp_energy = []
         else:
             T = temperature
-            U_vib = np.array([], dtype=float)
-            entropy = np.array([], dtype=float)
-            C_v = np.array([], dtype=float)
+            U_vib = []
+            entropy = []
+            C_v = []
 
         for qpoint in self.mode:
             if calculate_zp:
                 zp_energy_q = 0.
             else:
                 U_vib_q = 0.
                 entropy_q = 0.
@@ -585,152 +554,151 @@
                     zp_energy_q += mode.get_zp_energy()
                 else:
                     U_vib_q += mode.get_U_vib(temperature=T)
                     entropy_q += mode.get_entropy(temperature=T)
                     C_v_q += mode.get_C_v(temperature=T)
 
             if calculate_zp:
-                zp_energy = np.append(zp_energy, zp_energy_q)
+                zp_energy.append(zp_energy_q)
             else:
-                U_vib = np.append(U_vib, U_vib_q)
-                entropy = np.append(entropy, entropy_q)
-                C_v = np.append(C_v, C_v_q)
+                U_vib.append(U_vib_q)
+                entropy.append(entropy_q)
+                C_v.append(C_v_q)
 
         if calculate_zp:
+            zp_energy = np.array(zp_energy, dtype=float)
             return zp_energy
         else:
+            U_vib = np.array(U_vib, dtype=float)
+            entropy = np.array(entropy, dtype=float)
+            C_v = np.array(C_v, dtype=float)
             return U_vib, entropy, C_v
 
-    def thermodynamics(self, sumphonon=True, mutewarning=False, **temptpress):
+    def thermodynamics(self, sumphonon=True, mutewarning=False, **kwargs):
         """
         Calculate the thermodynamic properties (zp_energy, U_vib, entropy, C_v
         and Helmholtz free energy) of the given system, at all qpoints and the
         whole temperature range.
 
-        Input:
-            temperature, Optional, nTempt * 1 array / list, Temperatures where
-                         the thermodynamic properties are computed. Unit: K
-            pressure, Optional, npress * 1 array / list, Pressures where the
-                      thermodyanmic properties are calculated. Unit: GPa
-            sumphonon, bool, Whether summing up the phonon contributions across
-                       the first Brillouin zone and take average.
-            mutewarning, bool, Whether print out warning messages of updating
-                               temperature and pressure.
-        Output:
-            self.helmholtz, nqpoint * nTempt numpy array, Helmholtz free
-                            energy. Unit: KJ/mol cell
-            self.gibbs, nqpoint * nTempt * npress numpy array, Gibbs free 
-                        energy. Unit: KJ/mol cell
-            self.zp_energy, nqpoint * 1 numpy array, Zero-point energy.
-                            Unit: KJ/mol cell
-            self.U_vib, nqpoint * nTempt numpy array, Vibrational contribute to
-                        internal energy. Unit: KJ/mol cell
-            self.entropy, nqpoint * nTempt numpy array, Entropy.
-                          Unit: J/mol cell*K
-            self.C_v, nqpoint * nTempt numpy array, Constant volume specific
-                      heat. Unit: J/mol cell*K
-
-        Generated, not returned output:
-            self.temperature, nTempt * 1 array / list, Temperature range.
-                              Unit: K
-            self.pressure, nPress * 1 array / list, Pressure range.
-                              Unit: K
-
-        Note: If sumphonon = True, the thermodyanmic properties of phonon 
-              dispersion are summed. In this case, nqpoint = 1 but the
-              dimension is kept.
+        The Helmholtz free energy is defined as:
+
+        .. math::
+
+            F(p,V) = E_{DFT} + F_{vib}(T) = E_{DFT} + U_{vib}(T) - TS(T)
+
+        Args:
+            temperature (array[float] | list[float], optional): 
+                Temperature. Unit: K
+            pressure (array[float] | list[float], optional):
+                Pressure. Unit: GPa
+            sumphonon (bool): Whether to sum up the phonon contributions across
+                the sampled q points and take weighted-average.
+            mutewarning (bool): Whether print out warning messages of updated
+                temperature and pressure (For QHA).
+
+        Returns:
+            self.helmholtz (array[float]): Helmholtz free energy 
+                (nqpoint\*ntemperature). Unit: KJ/mol
+            self.gibbs (array[float]): Gibbs free energy 
+                (nqpoint\*ntemperature\*npressure). Unit: KJ/mol
+            self.zp_energy (array[float]): Zero-point energy. (nqpoint\*1). 
+                Unit: KJ/mol
+            self.U_vib (array[float]): Vibrational contribution to internal 
+                energy (nqpoint\*ntemperature). Unit: KJ/mol
+            self.entropy (array[float]): Entropy (nqpoint\*ntemperature)
+                Unit: J/mol\*K
+            self.C_v (array[float]): Constant volume specific heat 
+                (nqpoint\*ntemperature). Unit: J/mol\*K
+
+
+        **Note**: If ``sumphonon = True``, nqpoint = 1.
+
+        :raise ValueError: If temperature and pressure are defined neither here nor during initialization
         """
         import warnings
         import numpy as np
         import scipy.constants as scst
 
         # Generate temperature and pressure series
-        if temptpress:
-            if 'temperature' in temptpress:
+        if kwargs:
+            if 'temperature' in kwargs:
                 if hasattr(self, 'temperature') and not mutewarning:
                     warnings.warn(
                         'Temperature attribute exists. Input temperatures will be used to update the attribute.')
 
-                self.temperature = np.array(
-                    temptpress['temperature'], dtype=float)
+                self.temperature = np.array(kwargs['temperature'], dtype=float)
 
-            if 'pressure' in temptpress:
+            if 'pressure' in kwargs:
                 if hasattr(self, 'pressure') and not mutewarning:
                     warnings.warn(
                         'Pressure attribute exists. Input pressures will be used to update the attribute.')
 
-                self.pressure = np.array(temptpress['pressure'], dtype=float)
+                self.pressure = np.array(kwargs['pressure'], dtype=float)
         else:
             if not hasattr(self, 'temperature') or \
                not hasattr(self, 'pressure'):
                 raise ValueError(
                     'Temperature and pressure should be specified.')
 
-        self.zp_energy = self._phonon_sumup(temperature=0., calculate_zp=True)
+        zp_energy = self._phonon_sumup(temperature=0., calculate_zp=True)
         U_vib = []
         entropy = []
         C_v = []
         helmholtz = []
         gibbs = []
 
         for T in self.temperature:
             gibbs_t = []
-            U_vib_t, entropy_t, C_v_t = self._phonon_sumup(
-                temperature=T, calculate_zp=False)
+            U_vib_t, entropy_t, C_v_t = self._phonon_sumup(temperature=T,
+                                                           calculate_zp=False)
             helm_t = -entropy_t * T * 1e-3 + U_vib_t + self.edft
 
             for p in self.pressure:
                 gibbs_tp = p * self.volume * scst.Avogadro * 1e-24 + helm_t
                 gibbs_t.append(gibbs_tp)
 
             # nTemp * nqpoint
             U_vib.append(U_vib_t)
             entropy.append(entropy_t)
             C_v.append(C_v_t)
             helmholtz.append(helm_t)
             # nTemp * npress * nqpoint
             gibbs.append(gibbs_t)
 
-        U_vib = np.transpose(np.array(U_vib, dtype=float))
-        entropy = np.transpose(np.array(entropy, dtype=float))
-        C_v = np.transpose(np.array(C_v, dtype=float))
-        helmholtz = np.transpose(np.array(helmholtz, dtype=float))
-        gibbs = np.transpose(np.array(gibbs, dtype=float), (2, 0, 1))
-
         if sumphonon:
-            self.U_vib = np.array([np.sum(U_vib, axis=0)]) / self.nqpoint
-            self.entropy = np.array([np.sum(entropy, axis=0)]) / self.nqpoint
-            self.C_v = np.array([np.sum(C_v, axis=0)]) / self.nqpoint
-            self.helmholtz = np.array(
-                [np.sum(helmholtz, axis=0)]) / self.nqpoint
-            self.gibbs = np.array([np.sum(gibbs, axis=0)]) / self.nqpoint
+            wt = np.array([qp[1] for qp in self.qpoint])
             self.nqpoint = 1
-            self.qpoint = np.array([[0., 0., 0.]], dtype=float)
+            self.qpoint = [[np.array([0., 0., 0.]), 1.]]
+            self.zp_energy = np.array([np.dot(zp_energy, wt)])
+            self.U_vib = np.array([np.dot(U_vib, wt)])
+            self.entropy = np.array([np.dot(entropy, wt)])
+            self.C_v = np.array([np.dot(C_v, wt)])
+            self.helmholtz = np.array([np.dot(helmholtz, wt)])
+            self.gibbs = np.array([np.dot(gibbs, wt)])
         else:
-            self.U_vib = U_vib
-            self.entropy = entropy
-            self.C_v = C_v
-            self.helmholtz = helmholtz
-            self.gibbs = gibbs
+            self.zp_energy = zp_energy
+            self.U_vib = np.transpose(np.array(U_vib, dtype=float))
+            self.entropy = np.transpose(np.array(entropy, dtype=float))
+            self.C_v = np.transpose(np.array(C_v, dtype=float))
+            self.helmholtz = np.transpose(np.array(helmholtz, dtype=float))
+            self.gibbs = np.transpose(np.array(gibbs, dtype=float), (2, 0, 1))
 
         return self.helmholtz, self.gibbs, self.zp_energy, self.U_vib,\
             self.entropy, self.C_v
 
     def print_results(self):
         """
-        Print a single output file for HA thermodynamics. Used if write_out=True.
+        Print HA thermodynamic results into an external file. Used if 
+        ``write_out = True``.
 
-        Note: Phonon dispersions are forced to be summed to keep the output
-        succinct if the automatic scheme (write_out=True) is launched. To get
-        verbose outputs, directly use this attribute.
+        **Note**
 
-        Input:
-            -
-        Output:
-            filename, text file.
+        Phonon dispersions are forced to be summed to keep the output
+        succinct if the automatic scheme (write_out=True) is launched. To get
+        verbose outputs, directly call this method.
         """
         import scipy.constants as scst
         from CRYSTALpytools.units import eV_to_H
 
         if not self.write_out:
             print('Harmonic.write_out = False, return to empty.')
             return
@@ -775,59 +743,45 @@
 
             for gibbs_t in self.gibbs[q]:
                 file.write('\n%4s' % '')
                 for gibbs_p in gibbs_t:
                     file.write('%18.6e%2s' % (gibbs_p, ''))
 
             file.write('\n\n\n')
-            file.close()
+        file.close()
 
         return
 
 
 class Quasi_harmonic:
     """
-    Class Quasi_haromic - Generate and arrange harmonic phonons, store the
-    fitted, volume dependent QHA phonon information and obtain the QHA
-    thermodynamic properties.
-
-    self.ncalc, from_HA_files, The number of phonon calculations.
-    self.combined_phonon, from_HA_files, Sampled calculation as Harmonic object
-    self.combined_volume, from_HA_files, A list of volumes.
-    self.combined_edft, from_HA_files, A list of DFT total energies.
-    self.combined_mode, from_HA_files, A list of mode objects.
-    self.eos_method, edft_eos_fit, Fitting method of equation of states
-    self.eos, edft_eos_fit, Fitted equation of states
-    self.fit_order, freq_polynomial_fit, The optimal order of polynomial fit
-    self.temerature, thermo_freq / thermo_eos, Temperature series. Unit: K
-    self.pressure, thermo_freq / thermo_eos, Pressure series. Unit: GPa
-    self.equilibrium_volume, thermo_freq / thermo_eos, V(T, p). Unit: Angstrom^3
-    self.helmholtz, thermo_freq / thermo_eos, F(T, V). Unit: kJ/mol
-    self.gibbs, thermo_freq / thermo_eos, G(T, p). Unit: kJ/mol
-    self.entropy, thermo_freq / thermo_eos, S(T, V). Unit: J/mol*K
+    Generate and rearrange harmonic phonons, store the fitted, volume-dependent
+    QHA phonon information and obtain the QHA thermodynamic properties.
+
+    Args:
+        temperature (array[float] | list[float], optional): Unit: K
+        pressure (array[float] | list[float], optional): Unit: GPa
+        write_out (bool): Whether to print the key information into a file.
+        filename (str): Name of the output file. Valid if 
+                ``write_out = True``.
+
+    **Note**
+
+    Temperatures and pressures can also be defined by ``self.thermodynamics``,
+    whose entries always cover the entries here.
+
+    Usage::
+
+        qha = Quasi_harmonic()
+        qha.from_QHA_file('qha_phonon.out')
+        qha.thermo_freq(eos_method='birch_murnaghan', temperature=[0, 100, 200, 300], pressure=[0., 0.5, 1.]):
     """
 
     def __init__(self, temperature=[], pressure=[],
                  write_out=True, filename='QHA-Fit.dat'):
-        """
-        Initialization.
-
-        Input:
-            temperature, nTempt * 1 array / list, Temperatures where the
-                         thermodynamic properties are computed. Unit: K
-            pressure, npress * 1 array / list, Pressures where the
-                      thermodyanmic properties are calculated. Unit: GPa
-            write_out, bool, Whether to record the key information into a file.
-            filename, str, Name of the printed-out file, used only if
-                      write_out = True.
-        Note: Temperature can also be defined in 'thermodynamics' method, which
-              will cover the settings during initialisation.
-        Output: 
-            -
-        """
         import numpy as np
 
         if len(temperature) > 0:
             self.temperature = np.array(temperature, dtype=float)
 
         if len(pressure) > 0:
             self.pressure = np.array(pressure, dtype=float)
@@ -838,24 +792,29 @@
         else:
             self.filename = 'no file'
 
     def from_HA_files(self, input_files, scelphono=[], overlap=0.4, sort_phonon=True):
         """
         Read data from individual HA calculation outputs.
 
-        Input:
-            input_files, ncalc*1 list, List of phonon output filenames.
-            scelphono, ndimen*ndimen or 3*3 list / array, Same to the
-                       'SCELPHONO' keyword of CRYSTAL17 input.
-            overlap, float, The threshold of close mode overlaps
-            sort_phonon, bool, Whether to check phonon continuity. 
-        Output:
-            self.ncalc, int, Number of HA phonon calculations.
-            self.combined_phonon, self.combined_volume, self.combined_edft,
-            self.combined_mode, refer the method 'combine_data'
+        Args:
+            input_files (list[str]): List of phonon output filenames.
+            scelphono (array[float] | list[float]], optional): Corresponds
+                to the 'SCELPHONO' keyword in CRYSTAL. Either 3\*3 or 
+                ndimension\*ndimension. By default a 1\*1\*1 'SCELPHONO' is 
+                assumed.
+            overlap (float, optional): The threshold of close mode overlaps.
+            sort_phonon (bool, optional): Whether to check phonon continuity.
+
+        Returns:
+            self.ncalc (int): Number of HA phonon calculations.
+            self.combined_phonon (list[Harmonic]): List of Harmonic objects.
+            self.combined_volume (list[float]): Volumes. Unit: Angstrom^3
+            self.combined_edft (list[float]): DFT total energies. Unit: KJ/mol
+            self.combined_mode (list[Mode]): List of mode objects.
         """
         from CRYSTALpytools.thermodynamics import Harmonic
         import warnings
 
         if hasattr(self, "ncalc"):
             warnings.warn('Data exists. The current command will be ignored.')
 
@@ -874,26 +833,37 @@
                 auto_calc=False
             ) for file in input_files
         ]
 
         self.combined_phonon, self.combined_volume, self.combined_edft, \
             self.combined_mode = self._combine_data(ha_list, overlap=overlap,
                                                     sort_phonon=sort_phonon)
+        self.nqpoint = ha_list[0].nqpoint
+        self.qpoint = ha_list[0].qpoint # consistency of nqpoint is checked, but not qpoint.
 
         return self
 
     def from_QHA_file(self, input_file, scelphono=[], overlap=0.4, sort_phonon=True):
         """
         Read data from a single QHA calculation at Gamma point.
 
-        Input:
-            input_file, string or 1*1 list, Name of QHA output file. Only 1
-                        file is permitted
+        Args:
+            input_files (str | list[str]): Only 1 QHA file is permitted.
+            scelphono (array[float] | list[float], optional)
+            overlap (float, optional)
+            sort_phonon (bool, optional)
+
+        Returns:
+            self.ncalc (int)
+            self.combined_phonon (list[Harmonic])
+            self.combined_volume (list[float])
+            self.combined_edft (list[float])
+            self.combined_mode (list[Mode])
 
-        Other Input/output are consistent with 'from_HA_files'
+        :raise Exception: If multiple files are defined.
         """
         from CRYSTALpytools.crystal_io import Crystal_output
         from CRYSTALpytools.thermodynamics import Harmonic
         from CRYSTALpytools.thermodynamics import Mode
         import warnings
         import re
         import numpy as np
@@ -985,42 +955,36 @@
                               np.array([file.eigenvector[idx_c]]),
                               structure=structures[idx_c + 1])  # The first one is pre-opt geom
             ha_list.append(ha)
 
         self.combined_phonon, self.combined_volume, self.combined_edft, \
             self.combined_mode = self._combine_data(ha_list, overlap=overlap,
                                                     sort_phonon=sort_phonon)
+        self.nqpoint = 1
+        self.qpoint = [[np.array([0., 0., 0.]), 1.]]
 
         return self
 
     def _combine_data(self, ha_list, overlap, sort_phonon):
         """
-        Combine the HA calculation data and rearrange it according to modes.
-        Not a standalone method.
+        Combine the HA calculation data and rearrange it in the ascending order 
+        of volumes. Not a standalone method.
 
-        NOTE: All the input data will be rearranged in the low-to-high sequence
-              according to volumes.
+        Args:
+            ha_list (list[Harmonic]): List of harmonic objects.
+            overlap (float)
+            sort_phonon (bool)
+
+        Returns:
+            combined_phonon (list[Harmonic])
+            combined_volume (list[float])
+            combined_edft (list[float])
+            combined_mode (list[Mode])
 
-        Input:
-            ha_list, ncalc * 1 list, The list of harmonic objects.
-            overlap, float, The threshold of close mode overlaps
-            sort_phonon, bool, Whether to check phonon continuity. 
-        Output:
-            combined_phonon, list of Harmonic objects, Sampled calculations
-            combined_volume, ncalc * 1 list, A list of volumes.
-                             Unit: Angstrom^3
-            combined_edft, ncalc * 1 list, A list of DFT total energies.
-                           Unit: KJ / mol cell
-            combined_mode, nqpoint * nmode list, A list of mode objects. Each
-                           mode object stands for a vibrational mode at the
-                           given q point and stores ncalc HA values for volume,
-                           frequency and eigenvector.
-                           mode.volume: ncalc * 1 array
-                           mode.frequency: ncalc * 1 array
-                           mode.eigenvector: ncalc * natom * 3 array
+        :raise Exception: If number of q points, modes or atoms are not consistent across the HA calculations.
         """
         import numpy as np
         import warnings
         from CRYSTALpytools.thermodynamics import Mode
 
         # Sorting data according to volumes
         sorted_vol = np.zeros([self.ncalc, 2])
@@ -1158,38 +1122,41 @@
 
                     file.write('\n')
 
             file.close()
 
         return combined_phonon, combined_volume, combined_edft, combined_mode
 
-    def _phonon_continuity(self, freq, eigvt, symm=None, overlap=0.4):
+    @staticmethod
+    def _phonon_continuity(freq, eigvt, symm=None, overlap=0.4):
         """
         Rearrange phonon modes by their continuity. If the difference between
-        the maximum scalar product of correspondin eigenvectors (normalized to 
+        the maximum scalar product of corresponding eigenvectors (normalized to 
         1) and scalar products of other modes is less than 0.4, warning is
-        printed due to the potential overlap of modes. Adopted from CRYSTAL17,
+        printed due to the potential overlap of modes. Adopted from CRYSTAL17.
+
+        .. note::
 
-        Erba A. J. Chem. Phys., 2014 141 124115.
+            A. Erba, *J. Chem. Phys.*, 2014, **141**, 124115.
 
         Not a standalone method.
 
-        Input:
-            freq, ncalc * nmode array, Phonon frequencies.
-            eigvt, ncalc * nmode * natom * 3 array, Eigenvectores normalized to
-                   1 of corresponding modes
-            symm, ncalc * nmode array, Sub-group numbers of corresponding modes
-                  (Not supported at the current implementation)
-            overlap, float, The threshold of close mode overlaps
-        Output:
-            freq, ncalc * nmode array, Sorted phonon frequencies
-            eigvt, ncalc * nmode * natom * 3 array, Sorted eigenvectores
-            close_overlap, ncalc * nmode * nmode boolian array, Whether close
-                           overlap is identified at previous calculation (2nd 
-                           dimension) and the current calculation (3rd).
+        Args:
+            freq (array[float]): Phonon frequencies. Unit: THz
+            eigvt (array[float]): Eigenvectores normalized to 1
+            symm (array[float]): Sub-group numbers of corresponding modes.
+                *Not implemented*
+            overlap (float): The threshold of close mode overlaps.
+
+        Returns:
+            freq (array[float]): Sorted phonon frequencies
+            eigvt (array[float]): Sorted eigenvectores
+            close_overlap (array[bool]):ncalc\*nmode\*nmode. Whether close 
+                overlap is identified between the previous calculation (2nd 
+                dimension) and the current one (3rd).
         """
         import numpy as np
 
         # Exclude negative and 0 frequencies
         ncalc = len(freq)
         nmode = len(freq[0])
         ng_mode = 0
@@ -1254,31 +1221,28 @@
                         eigvt[ref_c, ref_m] * eigvt[sort_c, sort_m]
                     ))
                     if ref_pdt - sort_pdt < overlap:
                         close_overlap[ref_c, ref_m, sort_m] = 1
 
         return freq, eigvt, close_overlap
 
-    def edft_eos_fit(self, method, **fitargs):
+    def edft_eos_fit(self, method, **kwargs):
         """
-        Fit electron total energy according to equation of states. Not a
-        standalone method.
+        Fit electron total energy according to equation of states. 
 
-        Input:
-            method: string, Name of EoS used. Consistent with requirements of
-                    pymatgen (https://pymatgen.org/pymatgen.analysis.eos.html).
-
-        Optional Inputs:
-            order: int, limited to the DeltaFactor method
-            min_ndata_factor, max_poly_order_factor, min_poly_order_factor:
-                int, limited to the NumericalEOS method
-
-        Output:
-            self.eos_method, string, Equation of State used
-            self.eos, pymatgen EOS object, Fitted equation of state.
+        Args:
+            method (str): Name of EoS used. Consistent with
+                `PyMatGen <https://pymatgen.org/pymatgen.analysis.eos.html>`_.
+            order (int): For the DeltaFactor method. *Not implemented*
+            min_ndata_factor, max_poly_order_factor, min_poly_order_factor (int):
+                For the NumericalEOS method. *Not implemented*
+
+        Returns:
+            self.eos_method (string): Name of the fitted equation of state
+            self.eos (PyMatGen EOS): The fitted equation of state.
         """
         import re
         from pymatgen.analysis.eos import EOS
         import scipy.constants as scst
 
         self.eos_method = method
 # Commented due to the inhierant problem of pymatgen EOS object
@@ -1313,25 +1277,24 @@
             file.write('\n')
             file.close()
 
         return self.eos
 
     def freq_polynomial_fit(self, order):
         """
-        Fit phonon frequencies as polynomial functions of volumes. Not a
-        standalone method.
+        Fit phonon frequencies as polynomial functions of volumes. 
 
-        Input:
-            order, list/array, List of the highest order of polynomials to be
-                   fitted. Default: [2, 3] (quadratic, cubic)
-        Output:
-            self.fit_order, int, The optimal order of polynomial fit.
+        Args:
+            order (list[int] | array[int]): The order of polynomials used.
 
-        Also see 'self.poly_fit' and 'self.poly_fit_rsquare' attributes of mode
-        object
+        Returns:
+            self.fit_order (int): The optimal order of polynomial fit.
+
+        Please also refer to ``self.poly_fit`` and ``self.poly_fit_rsquare`` 
+        attributes of Mode class.
         """
         import numpy as np
 
         rsquare_tot = np.array([[od, 0] for od in order], dtype=float)
         eq_point = np.argmin(self.combined_edft)
 
         if self.write_out:
@@ -1392,157 +1355,155 @@
         return self
 
     def _get_harmonic_phonon(self, volume):
         """
         Get numerical phonon frequencies from fitted analytical expressions and
         generate harmonic phonon objects. Not a standalone method.
 
-        Input:
-            volume, float, The volume of harmonic lattice. Unit: Angstrom^3
-        Output:
-            ha, Harmonic, Harmonic phonon object with numerical data.
+        Args:
+            volume (float): Unit: Angstrom^3
+
+        Returns:
+            ha (Harmonic): Harmonic phonon object with numerical data.
+
+        :raise Exception: If frequency is not fitted as function of volumes.
         """
         import numpy as np
         from CRYSTALpytools.thermodynamics import Harmonic
         from CRYSTALpytools.thermodynamics import Mode
 
         if not hasattr(self, 'fit_order') or not hasattr(self, 'eos'):
             raise Exception('ERROR: Analytical expressions unavailable.')
 
         eq_point = np.argmin(self.combined_edft)
         num_mode = []
         for mode_q in self.combined_mode:
             num_mode_q = []
             for idx_m, mode in enumerate(mode_q):
                 d_vol = volume - self.combined_volume[eq_point]
-                freq = mode.poly_fit[self.fit_order](d_vol) \
-                    + mode_q[idx_m].frequency[eq_point]
-                num_mode_q.append(
-                    Mode(rank=idx_m + 1, frequency=[freq], volume=[volume])
-                )
-
+                freq = mode.poly_fit[self.fit_order](d_vol) + mode_q[idx_m].frequency[eq_point]
+                num_mode_q.append(freq)
             num_mode.append(num_mode_q)
 
-        ha = Harmonic(write_out=False).from_mode(self.eos(volume),
-                                                 num_mode, volume=volume)
+        num_mode = np.array(num_mode)
+        ha = Harmonic(write_out=False).from_frequency(
+            self.eos(volume), self.qpoint, num_mode, [], volume=volume
+        )
 
         return ha
 
     def _minimize_gibbs(self, volume, temperature, pressure):
         """
         Get Gibbs free energy from the Harmonic phonon object. Used only for
         minimizing G(V; T, p) by SciPy. Not a standalone method.
 
-        Input:
-            volume, float, The volume of lattice (V). Unit: Angstrom^3
-            temperature, float, T, argument. Unit: K
-            pressure, float, p, argument. Unit: GPa
+        Args:
+            volume (float)
+            temperature (float)
+            pressure (float)
+
+        Returns:
+            ha.gibbs (float): Gibbs free energy. Unit: KJ/mol
         """
         ha = self._get_harmonic_phonon(volume)
         ha.thermodynamics(temperature=[temperature], pressure=[pressure])
 
         return ha.gibbs[0, 0, 0]
 
     def thermo_freq(self, eos_method='birch_murnaghan', poly_order=[2, 3],
                     min_method='BFGS', volume_bound=None, mutewarning=False,
-                    **temptpress):
+                    **kwargs):
         """
-        1. Fit E_DFT and frequencies (if that has not been done) according to
-        methods specified. 
-        2. Calculate the 0 pressure equilibrium volume and pressure-independent
-        properties (Helmholtz free energy, Entropy and Constant-volume specific
-        heat) at given temperatures.
-        3. Calculate pressure-dependent proerties (Gibbs free energy)
-
-        Input:
-            eos_method: string, Equation of state used to fit E_DFT. For EOSs
-                        supported, refer https://pymatgen.org/pymatgen.analysis.eos.html
-            poly_order: list/array, List of the highest order of polynomials to
-                        be fitted.
-            min_method: string, Minimisation algorithms. Parameterized and
-                        tested algos: 
-                        * BFGS(no boundary)
-                        * L-BFGS-B(with boundary)
-            volume_bound: turple-like, Boundary conditions of equilibrium
-                          volumes. Unit: Angstrom^3
-            mutewarning, bool, Whether print out warning messages.
-
-        Optional Inputs:
-            temperature: Optional, nTempt*1 list/array, Temperatures. Unit: K
-            pressure: Optional, nPress*1 list/array, Pressures. Unit: GPa
-            order: int, limited to the DeltaFactor method
-            min_ndata_factor, max_poly_order_factor, min_poly_order_factor:
-                int, limited to the NumericalEOS method
-
-        Output:
-            self.temperature, nTempt*1 array, List of temperatures. Unit: K
-            self.pressure, nPress*1 array, List of pressures. Unit: GPa
-            self.equilibrium_volume, nPress*nTempt array, Equilibrium volumes
-                                     at given temperature and pressure. Unit:
-                                     Angstrom^3
-            self.helmholtz, nPress*nTempt array, Helmholtz free energy at given
-                            volume. Unit: kJ/mol
-            self.gibbs, nPress*nTempt array, Gibbs free energy at given volume.
-                        Unit: kJ/mol
-            self.entropy, nPress*nTempt array, Entropy at given volume. Unit:
-                          J/mol*K
+        Obtain thermodynamic properties by explicitly fitting phonon 
+        frequencies as polynomial functions of volume. DFT total energies are
+        fitted as a function of volume by equation of states (EOS).
+
+        Args:
+            eos_method (str, optional): EOS used to fit DFT total energies. 
+            poly_order (array[int] | list[int], optional): The order of 
+                polynomials used to fit frequency as the function of volumes.
+            min_method (string, optional): Minimisation algorithms. 
+            volume_bound (tuple-like, optional), Boundary conditions of 
+                equilibrium volumes. Unit: Angstrom^3
+            mutewarning (bool, optional): Whether print out warning messages.
+            temperature (array[float], optional): Unit: K
+            pressure (array[float], optional): Unit: GPa
+            order (int, optional): For DeltaFactor EOS. *Not implemented*
+            min_ndata_factor, max_poly_order_factor, min_poly_order_factor (int, optional):
+                For Numerical EOS. *Not implemented*
+
+        **Notes**
+
+        1. EOS supported by ``eos_method`` are consistent with `PyMatGen <https://pymatgen.org/pymatgen.analysis.eos.html>`_.
+        2. Parameterized and tested algorithms for ``min_method``: 
+            * BFGS(no boundary)
+            * L-BFGS-B(with boundary)
+
+        Returns:
+            self (Quasi_harmonic)
+
+        **New Attributes**
+
+        * ``self.temperature`` in K and ``self.pressure`` in GPa.
+        * ``self.equilibrium_volume``, nPressure\*nTemperature. Equilibrium volumes. Unit: Angstrom^3
+        * ``self.helmholtz`` and ``self.gibbs``, nPressure\*nTemperature. Helmholtz and Gibbs free energies. Unit: kJ/mol
+        * ``self.entropy``, nPressure\*nTemperature, Entropy. Unit: J/mol\*K
 
-        Optional outputs, see comments in edft_eos_fit, freq_polynomial_fit
+        :raise ValueError: If temperature or pressure is defined neither here nor during initialization.
         """
         import numpy as np
         import warnings
         import re
         from scipy.optimize import minimize
 
         # Generate temperature and pressure series
-        if temptpress:
-            if 'temperature' in temptpress:
+        if kwargs:
+            if 'temperature' in kwargs:
                 if hasattr(self, 'temperature') and not mutewarning:
                     warnings.warn(
                         'Temperature attribute exists. Input temperatures will be used to update the attribute.', stacklevel=2)
 
-                self.temperature = np.array(
-                    temptpress['temperature'], dtype=float)
+                self.temperature = np.array(kwargs['temperature'], dtype=float)
 
-            if 'pressure' in temptpress:
+            if 'pressure' in kwargs:
                 if hasattr(self, 'pressure') and not mutewarning:
                     warnings.warn(
                         'Pressure attribute exists. Input pressures will be used to update the attribute.', stacklevel=2)
 
-                self.pressure = np.array(temptpress['pressure'], dtype=float)
+                self.pressure = np.array(kwargs['pressure'], dtype=float)
 
         if not hasattr(self, 'temperature') or not hasattr(self, 'pressure'):
             raise ValueError('Temperature and pressure should be specified.')
 
         # Fit DFT total energy, if not done yet. Otherwise, fitted values will not be covered.
         if hasattr(self, 'eos') and not mutewarning:
             warnings.warn(
                 'DFT total energy is already fitted. To keep the consistency, it will not be updated.', stacklevel=2)
         else:
             # Commented due to the inhierant problem of pymatgen EOS object
             #             if re.findall(r'deltafactor', eos_method, re.I):
-            #                 if 'order' not in temptpress.keys():
-            #                     temptpress.update({'order' : 3})
+            #                 if 'order' not in kwargs.keys():
+            #                     kwargs.update({'order' : 3})
 
-            #                 self.edft_eos_fit(method=eos_method, order=temptpress['order'])
+            #                 self.edft_eos_fit(method=eos_method, order=kwargs['order'])
 
             #             elif re.findall(r'numerical_eos', eos_method, re.I):
-            #                 if 'min_ndata_factor' not in temptpress.keys():
-            #                     temptpress.update({'min_ndata_factor' : 3})
+            #                 if 'min_ndata_factor' not in kwargs.keys():
+            #                     kwargs.update({'min_ndata_factor' : 3})
 
-            #                 if 'max_poly_order_factor' not in temptpress.keys():
-            #                     temptpress.update({'max_poly_order_factor' : 5})
+            #                 if 'max_poly_order_factor' not in kwargs.keys():
+            #                     kwargs.update({'max_poly_order_factor' : 5})
 
-            #                 if 'min_poly_order_factor' not in temptpress.keys():
-            #                     temptpress.update({'min_poly_order_factor' : 2})
+            #                 if 'min_poly_order_factor' not in kwargs.keys():
+            #                     kwargs.update({'min_poly_order_factor' : 2})
 
             #                 self.edft_eos_fit(method=eos_method,
-            #                                   min_ndata_factor=temptpress['min_ndata_factor'],
-            #                                   max_poly_order_factor=temptpress['max_poly_order_factor'],
-            #                                   min_poly_order_factor=temptpress['min_poly_order_factor'])
+            #                                   min_ndata_factor=kwargs['min_ndata_factor'],
+            #                                   max_poly_order_factor=kwargs['max_poly_order_factor'],
+            #                                   min_poly_order_factor=kwargs['min_poly_order_factor'])
 
             #             else:
             #                 self.edft_eos_fit(method=eos_method)
             self.edft_eos_fit(method=eos_method)
 
         # Fit frequencies, if not done yet. Otherwise, fitted values will not be covered.
         if hasattr(self, 'fit_order') and not mutewarning:
@@ -1646,75 +1607,70 @@
 
             file.write('\n')
             file.close()
 
         return self
 
     def thermo_eos(self, eos_method='birch_murnaghan', poly_order=[2, 3],
-                   mutewarning=False, **temptpress):
+                   mutewarning=False, **kwargs):
         """
-        Obtain thermodynamic properties by fitting equation of states F(V). 
-        Exact sorting and fitting of frequency-volume relationship is disabled,
-        EoSs are fitted according to the Helmholtz free energy of sampled 
-        harmonic phonons. 
-
-        Input:
-
-            eos_method: string, Equation of state used to fit F. For EOSs 
-                        supported, refer https://pymatgen.org/pymatgen.analysis.eos.html
-            poly_order: list/array, List of the highest order of polynomials to
-                        be fitted (G(T) for entropy).
-            mutewarning, bool, Whether print out warning messages.
-
-        Optional Inputs:
-            temperature: Optional, nTempt*1 list/array, Temperatures. Unit: K
-            pressure: Optional, nPress*1 list/array, Pressures. Unit: GPa
-            order: int, limited to the DeltaFactor method
-            min_ndata_factor, max_poly_order_factor, min_poly_order_factor:
-                int, limited to the NumericalEOS method
-
-        Output:
-            self.thermo_eos_method: string, Equation of state used to fit F.
-            self.thermo_eos: nTempt*1 list, List of adiabatic EoS at given
-                             temperatures
-
-        self.temperature, self.pressure, self.equilibrium_volume, 
-        self.helmholtz, self.gibbs, self.entropy are consistent with method
-        'thermodynamics'.
+        Obtain thermodynamic properties by fitting EOS, which is fitted by the 
+        Helmholtz free energies of sampled harmonic phonons. The explicit 
+        sorting and fitting of frequency-volume relationship is disabled.
+
+        Args:
+
+            eos_method (str, optional)
+            poly_order (array[int] | list[int], optional): Order of 
+                polynomials used to fit Gibbs free energy to get entropy.
+            mutewarning (bool, optional)
+            temperature (array[float] | list[float], optional): Unit: K
+            pressure (array[float] | list[float], optional): Unit: GPa
+            order (int, optional): For DeltaFactor EOS. *Not implemented*
+            min_ndata_factor, max_poly_order_factor, min_poly_order_factor (int, optional):
+                For Numerical EOS. *Not implemented*
+
+        Returns:
+            self (Quasi_harmonic)
+
+        New Attributes are consistent with the ``thermo_freq`` method
+
+        :raise Exception: If the number of HA calculations is less than 4.
+        :raise ValueError: If temperature or pressure is defined neither here nor during initialization.
         """
         import numpy as np
         import warnings
         import re
         from CRYSTALpytools.thermodynamics import Harmonic
         from pymatgen.analysis.eos import EOS
         from scipy.optimize import fmin
         from sympy import diff, lambdify, symbols
 
         # Check the number of calculations
         if self.ncalc < 4:
             raise Exception('Insufficient database. Increase HA phonons')
 
         # Generate temperature and pressure series
-        if temptpress:
-            if 'temperature' in temptpress:
+        if kwargs:
+            if 'temperature' in kwargs:
                 if hasattr(self, 'temperature') and not mutewarning:
                     warnings.warn(
                         'Temperature attribute exists. Input temperatures will be used to update the attribute.',
                         stacklevel=2)
 
                 self.temperature = np.array(
-                    temptpress['temperature'], dtype=float)
+                    kwargs['temperature'], dtype=float)
 
-            if 'pressure' in temptpress:
+            if 'pressure' in kwargs:
                 if hasattr(self, 'pressure') and not mutewarning:
                     warnings.warn(
                         'Pressure attribute exists. Input pressures will be used to update the attribute.',
                         stacklevel=2)
 
-                self.pressure = np.array(temptpress['pressure'], dtype=float)
+                self.pressure = np.array(kwargs['pressure'], dtype=float)
 
         if not hasattr(self, 'temperature') or not hasattr(self, 'pressure'):
             raise ValueError('Temperature and pressure should be specified.')
 
         # Data for fitting
         helmholtz = np.zeros([len(self.temperature), self.ncalc], dtype=float)
         for idx_c, calc in enumerate(self.combined_phonon):
@@ -1734,33 +1690,33 @@
             [len(self.pressure), len(self.temperature)], dtype=float)
         self.entropy = np.zeros(
             [len(self.pressure), len(self.temperature)], dtype=float)
         v = symbols('v')
         for idx_t, t in enumerate(self.temperature):
             # Commented due to the inhierant problem of pymatgen EOS object
             #             if re.findall(r'deltafactor', eos_method, re.I):
-            #                 if 'order' not in temptpress.keys():
-            #                     temptpress.update({'order' : 3})
+            #                 if 'order' not in kwargs.keys():
+            #                     kwargs.update({'order' : 3})
 
-            #                 hfe_t = EOS(eos_method).fit(self.combined_volume, helmholtz[idx_t], order=temptpress['order'])
+            #                 hfe_t = EOS(eos_method).fit(self.combined_volume, helmholtz[idx_t], order=kwargs['order'])
 
             #             elif re.findall(r'numerical_eos', eos_method, re.I):
-            #                 if 'min_ndata_factor' not in temptpress.keys():
-            #                     temptpress.update({'min_ndata_factor' : 3})
+            #                 if 'min_ndata_factor' not in kwargs.keys():
+            #                     kwargs.update({'min_ndata_factor' : 3})
 
-            #                 if 'max_poly_order_factor' not in temptpress.keys():
-            #                     temptpress.update({'max_poly_order_factor' : 5})
+            #                 if 'max_poly_order_factor' not in kwargs.keys():
+            #                     kwargs.update({'max_poly_order_factor' : 5})
 
-            #                 if 'min_poly_order_factor' not in temptpress.keys():
-            #                     temptpress.update({'min_poly_order_factor' : 2})
+            #                 if 'min_poly_order_factor' not in kwargs.keys():
+            #                     kwargs.update({'min_poly_order_factor' : 2})
 
             #                 hfe_t = EOS(eos_method).fit(self.combined_volume, helmholtz[idx_t],
-            #                                             min_ndata_factor=temptpress['min_ndata_factor'],
-            #                                             max_poly_order_factor=temptpress['max_poly_order_factor'],
-            #                                             min_poly_order_factor=temptpress['min_poly_order_factor'])
+            #                                             min_ndata_factor=kwargs['min_ndata_factor'],
+            #                                             max_poly_order_factor=kwargs['max_poly_order_factor'],
+            #                                             min_poly_order_factor=kwargs['min_poly_order_factor'])
 
             #             else:
             #                 hfe_t = EOS(eos_method).fit(self.combined_volume, helmholtz[idx_t])
             hfe_t = EOS(eos_method).fit(self.combined_volume, helmholtz[idx_t])
             self.thermo_eos.append(hfe_t(v))
             press_t = -diff(hfe_t(v), v)
             for idx_p, p in enumerate(self.pressure):
```

### Comparing `CRYSTALpytools-2023.4.4/CRYSTALpytools/unit_test.py` & `CRYSTALpytools-2023.6.6/CRYSTALpytools/unit_test.py`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.4.4/CRYSTALpytools/units.py` & `CRYSTALpytools-2023.6.6/CRYSTALpytools/units.py`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.4.4/CRYSTALpytools/utils.py` & `CRYSTALpytools-2023.6.6/CRYSTALpytools/utils.py`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.4.4/CRYSTALpytools.egg-info/PKG-INFO` & `CRYSTALpytools-2023.6.6/CRYSTALpytools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CRYSTALpytools
-Version: 2023.4.4
+Version: 2023.6.6
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
-Metadata-Version: 2.1 Name: CRYSTALpytools Version: 2023.4.4 Summary: Python
+Metadata-Version: 2.1 Name: CRYSTALpytools Version: 2023.6.6 Summary: Python
 tools for the CRYSTAL code developed and mantained by the CRYSTAL code
 developers. Home-page: https://github.com/crystal-code-tools/CRYSTALpytools
 Author-email: crystalcodetools@gmail.com Project-URL: Bug Tracker, https://
 github.com/crystal-code-tools/CRYSTALpytools/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown License-File: LICENSE.txt Python tools for the CRYSTAL_code developed
```

### Comparing `CRYSTALpytools-2023.4.4/CRYSTALpytools.egg-info/SOURCES.txt` & `CRYSTALpytools-2023.6.6/CRYSTALpytools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.4.4/LICENSE.txt` & `CRYSTALpytools-2023.6.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.4.4/PKG-INFO` & `CRYSTALpytools-2023.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CRYSTALpytools
-Version: 2023.4.4
+Version: 2023.6.6
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
-Metadata-Version: 2.1 Name: CRYSTALpytools Version: 2023.4.4 Summary: Python
+Metadata-Version: 2.1 Name: CRYSTALpytools Version: 2023.6.6 Summary: Python
 tools for the CRYSTAL code developed and mantained by the CRYSTAL code
 developers. Home-page: https://github.com/crystal-code-tools/CRYSTALpytools
 Author-email: crystalcodetools@gmail.com Project-URL: Bug Tracker, https://
 github.com/crystal-code-tools/CRYSTALpytools/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown License-File: LICENSE.txt Python tools for the CRYSTAL_code developed
```

### Comparing `CRYSTALpytools-2023.4.4/README.md` & `CRYSTALpytools-2023.6.6/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,128 +1,81 @@
 # CRYSTALpytools
-This repository contains functions that allow the user to access the
-<a href="https://www.crystal.unito.it/index.php">CRYSTAL code</a>,
-input, output and execution from a python infrastructure, such as
-Jupyter Notebooks. Although they can achieve this goal on their own,
-they achieve their full potential when used together with
-<a href="https://pymatgen.org/index.html">pymatgen</a>. In this latter scenario, the CRYSTALpytools could be seen as
+This repository contains functions that allow the user to access the <a href="https://www.crystal.unito.it/index.php">CRYSTAL code</a>, input, output and execution from a python infrastructure, such as Jupyter Notebooks. Although they can achieve this goal on their own, they achieve their full potential when used together with <a href="https://pymatgen.org/index.html">pymatgen</a>. In this latter scenario, the CRYSTALpytools could be seen as
 a layer between CRYSTAL and pymatgen.
 
 In January 2022 the first stable version (v2022.1.10) was released.
 
 ## Installation
 
 ### Create a conda/anaconda environment
-This step is not mandatory, but it makes using CRYSTALpytools very smooth.
-It is, therefore, very recommended.
-If you are new to anaconda, please follow <a href="https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html">these steps</a> to install it on your computer.
+This step is not mandatory, but it makes using CRYSTALpytools very smooth. It is, therefore, very recommended. If you are new to anaconda, please follow <a href="https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html">these steps</a> to install it on your computer.
 
 Create a new conda environment:
-```console
+``` console
 conda create --name crystal python=3.9
 ```
 
 In the line above, “crystal” is the name of the environment and can be set to any you like. The “python=3.9” ensures that the suitable python distribution is installed.
 
 Activate the conda environment:
-```console
+``` console
 conda activate crystal
 ```
 
 ### Install CRYSTALpytools
 
 The CRYSTALpytools package can be installed from pip. Pip is a package-management system written in Python and is used to install and manage software packages (called modules in python).
 
-```console
+``` console
 pip install --upgrade CRYSTALpytools
 ```
 
 Windows users might need to install windows-curses. This can be done by using:
 
-```console
+``` console
 pip install windows-curses
 ```
 
 To check that CRYSTALpytools was install please type
 
-```console
+``` console
 conda list
 ```
 
-This will return a list of all the modules installed in the environment. Here there should be crystal-functions. If this was not the case, something went wrong during the installation. Please check the location of the environment that is being displayed. This appears at the beginning of the “conda list” command. The most common mistake at this stage is that the environment was not activated as described above.
+This will return a list of all the modules installed in the environment. Here there should be crystalpytools. If this was not the case, something went wrong during the installation. Please check the location of the environment that is being displayed. This appears at the beginning of the “conda list” command. The most common mistake at this stage is that the environment was not activated as described above.
 
 
 Please note that pip will only install the functions and not the example notebooks. This decision was taken in order to reduce the volume of data transferred when installing. If you are interested in the example notebooks please read the section below.
 
 ### Set the path to runcry and runprop
 
-If you intend to run CRYSTAL on the machine where you are running
-the CRYSTALpytools, the path to your local runcry amd runprop needs to be specified. To do so, please run the set_runcry_path and set_runprop_path functions:
-```console
+If you intend to run CRYSTAL on the machine where you are running the CRYSTALpytools, the path to your local runcry amd runprop needs to be specified. To do so, please run the set_runcry_path and set_runprop_path functions:
+``` console
 python 3
 from CRYSTALpytools.execute import set_runcry_path, set_runprop_path
 set_runcry_path('path_to_your_runcry')
 set_runprop_path('path_to_your_runcry')
 ```
 
 ## Examples
-Each function is documented in Jupyter Notebooks that can be found in the  [example folder](example/). There is one notebook per function file (e.g. the functions contained in crystal_io.py are explained in the example/crystal_io.ipynb notebook).
+Each function is documented in Jupyter Notebooks that can be found in the  [example folder](examples/). There is one notebook per function file (e.g. the functions contained in crystal_io.py are explained in the example/crystal_io.ipynb notebook).
 
 
 ## Tutorials
 Tutorials can be found in the [tutorial folder](tutorial/)
 ## Usage
 
-The CRYSTALpytools module aims at providing the user
-a python interface to the CRYSTAL code. The central data structure, called Crystal_object is created by the crystal_io by parsing CRYSTAL input/output files. The flowchart below is aimed at showing how different parts of the module interact with the Crystal_objects.
+The CRYSTALpytools module aims at providing the user a python interface to the CRYSTAL code. The central data structure, called Crystal_object is created by the crystal_io by parsing CRYSTAL input/output files. The flowchart below is aimed at showing how different parts of the module interact with the Crystal_objects.
 
-![crystal_object](doc/crystal_object.jpg)
-
-The following flowcharts cover a wide range of workflows where
-CRYSTALpytools can be used. In order to run the CRYSTAL
-calculation, input data needs to be written to file. Nonetheless,
-crystal_function offers a much more approach flexible to do so.
-
-Despite trying to be as comprehensive as possible, these
-flowcharts will not cover all possible scenarios. Should you have
-any question please feel free to contact the maintainers of
-this repository.
-
-### Start from a pymatgen object
-This is the most flexible approach. Pymatgen gives the user the option to
-<a href="https://pymatgen.org/pymatgen.ext.matproj.html?highlight=mprester#pymatgen.ext.matproj.MPRester">download structures</a>
-from the Materials Project database.
-
-![pymatgen_start](doc/pymatgen_start.png)
-
-### Start from CRYSTAL input file or manually prepare the input
-In some instances, for example when studying a material for which
-you already have an input file, it might be easier to create a Crystal_input object by reading the information from file. Some researchers might find it easier to manually prepare the input. This means that the input lines are specified as lists in python and then written to file using the wry_cry_input function.
-
-![crystal_start](doc/crystal_start.png)
-
-### Output analysis only
-This case applied to when the calculations were run on a different machine and the user might be interested in analysing the output. The inputs can be generated from any of the two workflows above by stopping before execution.
-
-![output_analysis](doc/output_analysis.png)
-
-The functions are divided into files depending on their ultimate goal. For example, all the i/o functions are saved in CRYSTALpytools/crystal_io.py. To access them, please use:
-
-```console
-from CRYSTALpytools.crystal_io import Crystal_output
-
-Crystal_output('output_name.out')
-```
-
-Each individual function contains either 'crystal' or 'cry' in its name. This was chosen, despite making the names of the functions longer, in order to avoid ambiguity. This means that when calling a function, you will know that it refers to a CRYSTALpytools function and not, for example, a pymatgen one with a similar name.
+![crystal_object](docs_source/_static/crystal_object.png)
 
 ## Testing
 To test the CRYSTALpytools please run the test notebook that can be found in the [unit_test folder](unit_test/). Alternatively, please run the following command:
 
-```console
+``` python
 from CRYSTALpytools.unit_test import *
 
 test_all('./data_test/')
 ```
 where './data_test/' is the path to the test folder.
 
 All values should return True if the test is passed.
```

#### html2text {}

```diff
@@ -4,74 +4,47 @@
 on their own, they achieve their full potential when used together with
 pymatgen. In this latter scenario, the CRYSTALpytools could be seen as a layer
 between CRYSTAL and pymatgen. In January 2022 the first stable version
 (v2022.1.10) was released. ## Installation ### Create a conda/anaconda
 environment This step is not mandatory, but it makes using CRYSTALpytools very
 smooth. It is, therefore, very recommended. If you are new to anaconda, please
 follow these_steps to install it on your computer. Create a new conda
-environment: ```console conda create --name crystal python=3.9 ``` In the line
+environment: ``` console conda create --name crystal python=3.9 ``` In the line
 above, âcrystalâ is the name of the environment and can be set to any you
 like. The âpython=3.9â ensures that the suitable python distribution is
-installed. Activate the conda environment: ```console conda activate crystal
+installed. Activate the conda environment: ``` console conda activate crystal
 ``` ### Install CRYSTALpytools The CRYSTALpytools package can be installed from
 pip. Pip is a package-management system written in Python and is used to
-install and manage software packages (called modules in python). ```console pip
-install --upgrade CRYSTALpytools ``` Windows users might need to install
-windows-curses. This can be done by using: ```console pip install windows-
-curses ``` To check that CRYSTALpytools was install please type ```console
+install and manage software packages (called modules in python). ``` console
+pip install --upgrade CRYSTALpytools ``` Windows users might need to install
+windows-curses. This can be done by using: ``` console pip install windows-
+curses ``` To check that CRYSTALpytools was install please type ``` console
 conda list ``` This will return a list of all the modules installed in the
-environment. Here there should be crystal-functions. If this was not the case,
+environment. Here there should be crystalpytools. If this was not the case,
 something went wrong during the installation. Please check the location of the
 environment that is being displayed. This appears at the beginning of the
 âconda listâ command. The most common mistake at this stage is that the
 environment was not activated as described above. Please note that pip will
 only install the functions and not the example notebooks. This decision was
 taken in order to reduce the volume of data transferred when installing. If you
 are interested in the example notebooks please read the section below. ### Set
 the path to runcry and runprop If you intend to run CRYSTAL on the machine
 where you are running the CRYSTALpytools, the path to your local runcry amd
 runprop needs to be specified. To do so, please run the set_runcry_path and
-set_runprop_path functions: ```console python 3 from CRYSTALpytools.execute
+set_runprop_path functions: ``` console python 3 from CRYSTALpytools.execute
 import set_runcry_path, set_runprop_path set_runcry_path('path_to_your_runcry')
 set_runprop_path('path_to_your_runcry') ``` ## Examples Each function is
 documented in Jupyter Notebooks that can be found in the [example folder]
-(example/). There is one notebook per function file (e.g. the functions
+(examples/). There is one notebook per function file (e.g. the functions
 contained in crystal_io.py are explained in the example/crystal_io.ipynb
 notebook). ## Tutorials Tutorials can be found in the [tutorial folder]
 (tutorial/) ## Usage The CRYSTALpytools module aims at providing the user a
 python interface to the CRYSTAL code. The central data structure, called
 Crystal_object is created by the crystal_io by parsing CRYSTAL input/output
 files. The flowchart below is aimed at showing how different parts of the
-module interact with the Crystal_objects. ![crystal_object](doc/
-crystal_object.jpg) The following flowcharts cover a wide range of workflows
-where CRYSTALpytools can be used. In order to run the CRYSTAL calculation,
-input data needs to be written to file. Nonetheless, crystal_function offers a
-much more approach flexible to do so. Despite trying to be as comprehensive as
-possible, these flowcharts will not cover all possible scenarios. Should you
-have any question please feel free to contact the maintainers of this
-repository. ### Start from a pymatgen object This is the most flexible
-approach. Pymatgen gives the user the option to download_structures from the
-Materials Project database. ![pymatgen_start](doc/pymatgen_start.png) ### Start
-from CRYSTAL input file or manually prepare the input In some instances, for
-example when studying a material for which you already have an input file, it
-might be easier to create a Crystal_input object by reading the information
-from file. Some researchers might find it easier to manually prepare the input.
-This means that the input lines are specified as lists in python and then
-written to file using the wry_cry_input function. ![crystal_start](doc/
-crystal_start.png) ### Output analysis only This case applied to when the
-calculations were run on a different machine and the user might be interested
-in analysing the output. The inputs can be generated from any of the two
-workflows above by stopping before execution. ![output_analysis](doc/
-output_analysis.png) The functions are divided into files depending on their
-ultimate goal. For example, all the i/o functions are saved in CRYSTALpytools/
-crystal_io.py. To access them, please use: ```console from
-CRYSTALpytools.crystal_io import Crystal_output Crystal_output
-('output_name.out') ``` Each individual function contains either 'crystal' or
-'cry' in its name. This was chosen, despite making the names of the functions
-longer, in order to avoid ambiguity. This means that when calling a function,
-you will know that it refers to a CRYSTALpytools function and not, for example,
-a pymatgen one with a similar name. ## Testing To test the CRYSTALpytools
-please run the test notebook that can be found in the [unit_test folder]
-(unit_test/). Alternatively, please run the following command: ```console from
+module interact with the Crystal_objects. ![crystal_object](docs_source/
+_static/crystal_object.png) ## Testing To test the CRYSTALpytools please run
+the test notebook that can be found in the [unit_test folder](unit_test/).
+Alternatively, please run the following command: ``` python from
 CRYSTALpytools.unit_test import * test_all('./data_test/') ``` where './
 data_test/' is the path to the test folder. All values should return True if
 the test is passed.
```

### Comparing `CRYSTALpytools-2023.4.4/setup.py` & `CRYSTALpytools-2023.6.6/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 long_description = 'Python tools for the <a href="https://www.crystal.unito.it/index.php">CRYSTAL code</a> developed and mantained by the CRYSTAL code developers'
 
 setuptools.setup(
     name="CRYSTALpytools",        
-    version="2023.04.04",
+    version="2023.06.06",
     author_email="crystalcodetools@gmail.com",
     description="Python tools for the CRYSTAL code developed and mantained by the CRYSTAL code developers.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/crystal-code-tools/CRYSTALpytools",
     project_urls={
         "Bug Tracker": "https://github.com/crystal-code-tools/CRYSTALpytools/issues",
@@ -17,12 +17,12 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=setuptools.find_packages(include=['CRYSTALpytools', 'CRYSTALpytools.*']),
     #python_requires=">=3.8",
     install_requires=[
-	"pymatgen",
-	"mendeleev",
-	"ase"
+    "pymatgen",
+    "mendeleev",
+    "ase"
     ]
 )
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 import setuptools long_description = 'Python tools for the CRYSTAL_code
 developed and mantained by the CRYSTAL code developers' setuptools.setup
-( name="CRYSTALpytools", version="2023.04.04",
+( name="CRYSTALpytools", version="2023.06.06",
 author_email="crystalcodetools@gmail.com", description="Python tools for the
 CRYSTAL code developed and mantained by the CRYSTAL code developers.",
 long_description=long_description, long_description_content_type="text/
 markdown", url="https://github.com/crystal-code-tools/CRYSTALpytools",
 project_urls={ "Bug Tracker": "https://github.com/crystal-code-tools/
 CRYSTALpytools/issues", }, classifiers=[ "Programming Language :: Python :: 3",
 "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",
```

