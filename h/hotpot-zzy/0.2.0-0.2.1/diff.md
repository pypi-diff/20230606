# Comparing `tmp/hotpot-zzy-0.2.0.tar.gz` & `tmp/hotpot-zzy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/zz1/hotpot/dist/.tmp-210l41vs/hotpot-zzy-0.2.0.tar", last modified: Sat Jun  3 08:23:43 2023, max compression
+gzip compressed data, was "/home/zz1/hotpot/dist/.tmp-i134ha33/hotpot-zzy-0.2.1.tar", last modified: Tue Jun  6 07:46:36 2023, max compression
```

## Comparing `hotpot-zzy-0.2.0.tar` & `hotpot-zzy-0.2.1.tar`

### file list

```diff
@@ -1,52 +1,45 @@
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-03 08:23:43.300421 hotpot-zzy-0.2.0/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       17 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.0/MANIFEST.in
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       54 2023-06-03 08:23:43.300421 hotpot-zzy-0.2.0/PKG-INFO
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-03 08:23:43.296421 hotpot-zzy-0.2.0/hotpot/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      398 2023-05-19 15:58:44.000000 hotpot-zzy-0.2.0/hotpot/__init__.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)    39992 2023-05-20 11:35:21.000000 hotpot-zzy-0.2.0/hotpot/_io.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)    15016 2023-05-21 10:40:23.000000 hotpot-zzy-0.2.0/hotpot/bundle.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)    81486 2023-05-21 05:08:08.000000 hotpot-zzy-0.2.0/hotpot/cheminfo.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-03 08:23:43.296421 hotpot-zzy-0.2.0/hotpot/data/
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-03 08:23:43.296421 hotpot-zzy-0.2.0/hotpot/data/force_field/
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-03 08:23:43.296421 hotpot-zzy-0.2.0/hotpot/data/force_field/UFF/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     4710 2023-05-04 02:36:48.000000 hotpot-zzy-0.2.0/hotpot/data/force_field/UFF/LJ.json
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-03 08:23:43.296421 hotpot-zzy-0.2.0/hotpot/data/force_field/aMaterials/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1742 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.0/hotpot/data/force_field/aMaterials/SiC.tersoff
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       88 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.0/hotpot/data/force_field/contents.json
--rw-rw-r--   0 zz1       (1005) zz1       (1008)   297275 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.0/hotpot/data/periodic_table.json
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      195 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.0/hotpot/data/units.json
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-03 08:23:43.300421 hotpot-zzy-0.2.0/hotpot/tanks/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      217 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.0/hotpot/tanks/__init__.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-03 08:23:43.300421 hotpot-zzy-0.2.0/hotpot/tanks/dl/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      133 2023-03-23 08:00:45.000000 hotpot-zzy-0.2.0/hotpot/tanks/dl/__init__.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      126 2023-03-23 08:00:45.000000 hotpot-zzy-0.2.0/hotpot/tanks/dl/bert.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      955 2023-03-23 08:00:45.000000 hotpot-zzy-0.2.0/hotpot/tanks/dl/datasets.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      134 2023-03-23 08:00:45.000000 hotpot-zzy-0.2.0/hotpot/tanks/dl/graph_learning.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-03 08:23:43.300421 hotpot-zzy-0.2.0/hotpot/tanks/dl/models/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      131 2023-03-30 08:04:59.000000 hotpot-zzy-0.2.0/hotpot/tanks/dl/models/__init__.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2512 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.0/hotpot/tanks/dl/models/dp.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      161 2023-03-23 08:00:45.000000 hotpot-zzy-0.2.0/hotpot/tanks/features.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-03 08:23:43.300421 hotpot-zzy-0.2.0/hotpot/tanks/lmp/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      284 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.0/hotpot/tanks/lmp/__init__.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     8118 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.0/hotpot/tanks/lmp/base.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     8704 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.0/hotpot/tanks/lmp/gcmc.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     9577 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.0/hotpot/tanks/lmp/materials.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     7857 2023-03-30 08:04:59.000000 hotpot-zzy-0.2.0/hotpot/tanks/quantum.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2949 2023-05-13 03:01:23.000000 hotpot-zzy-0.2.0/hotpot/tmo.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2882 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.0/hotpot/tools.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-03 08:23:43.300421 hotpot-zzy-0.2.0/hotpot/utils/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      134 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.0/hotpot/utils/__init__.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      669 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.0/hotpot/utils/units_convert.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-03 08:23:43.300421 hotpot-zzy-0.2.0/hotpot_zzy.egg-info/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       54 2023-06-03 08:23:43.000000 hotpot-zzy-0.2.0/hotpot_zzy.egg-info/PKG-INFO
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      972 2023-06-03 08:23:43.000000 hotpot-zzy-0.2.0/hotpot_zzy.egg-info/SOURCES.txt
--rw-rw-r--   0 zz1       (1005) zz1       (1008)        1 2023-06-03 08:23:43.000000 hotpot-zzy-0.2.0/hotpot_zzy.egg-info/dependency_links.txt
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       20 2023-06-03 08:23:43.000000 hotpot-zzy-0.2.0/hotpot_zzy.egg-info/requires.txt
--rw-rw-r--   0 zz1       (1005) zz1       (1008)        7 2023-06-03 08:23:43.000000 hotpot-zzy-0.2.0/hotpot_zzy.egg-info/top_level.txt
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      249 2023-06-03 08:23:13.000000 hotpot-zzy-0.2.0/pyproject.toml
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       38 2023-06-03 08:23:43.300421 hotpot-zzy-0.2.0/setup.cfg
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-03 08:23:43.300421 hotpot-zzy-0.2.0/test/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      550 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.0/test/test_amorphous_maker.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1162 2023-05-20 11:40:18.000000 hotpot-zzy-0.2.0/test/test_bundle.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1742 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.0/test/test_chemif.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     7081 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.0/test/test_lmp.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-06 07:46:36.324825 hotpot-zzy-0.2.1/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       17 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.1/MANIFEST.in
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       54 2023-06-06 07:46:36.324825 hotpot-zzy-0.2.1/PKG-INFO
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-06 07:46:36.324825 hotpot-zzy-0.2.1/hotpot/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      398 2023-05-19 15:58:44.000000 hotpot-zzy-0.2.1/hotpot/__init__.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    39992 2023-05-20 11:35:21.000000 hotpot-zzy-0.2.1/hotpot/_io.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    14731 2023-06-06 07:26:56.000000 hotpot-zzy-0.2.1/hotpot/bundle.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    83164 2023-06-06 07:13:56.000000 hotpot-zzy-0.2.1/hotpot/cheminfo.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-06 07:46:36.324825 hotpot-zzy-0.2.1/hotpot/data/
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-06 07:46:36.324825 hotpot-zzy-0.2.1/hotpot/data/force_field/
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-06 07:46:36.324825 hotpot-zzy-0.2.1/hotpot/data/force_field/UFF/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     4710 2023-05-04 02:36:48.000000 hotpot-zzy-0.2.1/hotpot/data/force_field/UFF/LJ.json
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-06 07:46:36.324825 hotpot-zzy-0.2.1/hotpot/data/force_field/aMaterials/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1742 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.1/hotpot/data/force_field/aMaterials/SiC.tersoff
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       88 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.1/hotpot/data/force_field/contents.json
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)   231681 2023-06-06 06:50:07.000000 hotpot-zzy-0.2.1/hotpot/data/periodic_table.json
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      195 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.1/hotpot/data/units.json
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-06 07:46:36.324825 hotpot-zzy-0.2.1/hotpot/tanks/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      217 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.1/hotpot/tanks/__init__.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      365 2023-06-05 01:59:39.000000 hotpot-zzy-0.2.1/hotpot/tanks/cc.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      161 2023-03-23 08:00:45.000000 hotpot-zzy-0.2.1/hotpot/tanks/features.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-06 07:46:36.324825 hotpot-zzy-0.2.1/hotpot/tanks/lmp/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      284 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.1/hotpot/tanks/lmp/__init__.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     8118 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.1/hotpot/tanks/lmp/base.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     8704 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.1/hotpot/tanks/lmp/gcmc.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     9577 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.1/hotpot/tanks/lmp/materials.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     7857 2023-03-30 08:04:59.000000 hotpot-zzy-0.2.1/hotpot/tanks/quantum.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2949 2023-05-13 03:01:23.000000 hotpot-zzy-0.2.1/hotpot/tmo.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2882 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.1/hotpot/tools.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-06 07:46:36.324825 hotpot-zzy-0.2.1/hotpot/utils/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      134 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.1/hotpot/utils/__init__.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      669 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.1/hotpot/utils/units_convert.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-06 07:46:36.324825 hotpot-zzy-0.2.1/hotpot_zzy.egg-info/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       54 2023-06-06 07:46:36.000000 hotpot-zzy-0.2.1/hotpot_zzy.egg-info/PKG-INFO
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      813 2023-06-06 07:46:36.000000 hotpot-zzy-0.2.1/hotpot_zzy.egg-info/SOURCES.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)        1 2023-06-06 07:46:36.000000 hotpot-zzy-0.2.1/hotpot_zzy.egg-info/dependency_links.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       26 2023-06-06 07:46:36.000000 hotpot-zzy-0.2.1/hotpot_zzy.egg-info/requires.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)        7 2023-06-06 07:46:36.000000 hotpot-zzy-0.2.1/hotpot_zzy.egg-info/top_level.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      263 2023-06-06 07:33:50.000000 hotpot-zzy-0.2.1/pyproject.toml
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       38 2023-06-06 07:46:36.324825 hotpot-zzy-0.2.1/setup.cfg
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-06 07:46:36.324825 hotpot-zzy-0.2.1/test/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      550 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.1/test/test_amorphous_maker.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1162 2023-05-20 11:40:18.000000 hotpot-zzy-0.2.1/test/test_bundle.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1932 2023-06-06 07:26:56.000000 hotpot-zzy-0.2.1/test/test_chemif.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     7081 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.1/test/test_lmp.py
```

### Comparing `hotpot-zzy-0.2.0/hotpot/_io.py` & `hotpot-zzy-0.2.1/hotpot/_io.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.0/hotpot/bundle.py` & `hotpot-zzy-0.2.1/hotpot/bundle.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,18 @@
 @Project: hotpot
 @File   : bundle.py
 @Author : Zhiyuan Zhang
 @Date   : 2023/3/22
 @Time   : 3:18
 """
 import copy
-import time
 from os import PathLike
 from typing import *
 from pathlib import Path
 import numpy as np
-import torch
 from tqdm import tqdm
 from openbabel import pybel as pb
 import hotpot.cheminfo as ci
 from hotpot.tools import check_path
 import multiprocessing as mp
 
 
@@ -202,26 +200,22 @@
         generator = mol_mp_generator() if num_proc else mol_generator()
 
         if generate:
             return cls(generator)
         else:
             return cls([m for m in tqdm(generator, 'reading molecules')])
 
-    def graph_represent(self, graph_fmt: GraphFormatName, *feature_type):
-        """ Transform molecules to the molecule to graph representation,
-        the transformed graph with 'numpy.ndarray' or 'PyTorch.Tensor' format """
+    def graph_represent(self, *feature_type):
+        """ Transform molecules to the molecule to graph representation """
         feature_matrices = []
         for mol in self.mols:
             feature_matrix = mol.feature_matrix(feature_names=feature_type)
             feature_matrices.append(feature_matrix)
 
-        if graph_fmt == 'numpy':
-            return feature_matrices
-        elif graph_fmt == 'Pytorch':
-            return [torch.tensor(matrix) for matrix in feature_matrices]
+        return feature_matrices
 
     def gaussian(
             self, g16root: Union[str, PathLike], dir_out: Union[str, PathLike],
             link0: Union[str, List[str]], route: Union[str, List[str]],
             dir_err: Optional[Union[str, PathLike]] = None,
             dir_chk: Optional[Union[str, PathLike]] = None,
             clean_configure: bool = True,
```

### Comparing `hotpot-zzy-0.2.0/hotpot/cheminfo.py` & `hotpot-zzy-0.2.1/hotpot/cheminfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,32 +3,36 @@
 @Project: hotpot
 @File   : cheminfo.py
 @Author : Zhiyuan Zhang
 @Date   : 2023/3/14
 @Time   : 4:09
 """
 import copy
+import json
 import os
 import re
+from abc import ABC, abstractmethod
 from io import IOBase
 from os import PathLike
 from os.path import join as ptj
 from pathlib import Path
-from abc import ABC, abstractmethod
-import json
 from typing import *
+
 import numpy as np
 from openbabel import openbabel as ob, pybel as pb
+
 from hotpot import data_root
-from hotpot.tanks.quantum import Gaussian
 from hotpot.tanks import lmp
+from hotpot.tanks.quantum import Gaussian
 
-periodic_table = json.load(open(ptj(data_root, 'periodic_table.json'), encoding='utf-8'))['elements']
-periodic_table = {d['symbol']: d for d in periodic_table}
+periodic_table = json.load(open(ptj(data_root, 'periodic_table.json'), encoding='utf-8'))
+# periodic_table = {d['symbol']: d for d in periodic_table}
 _symbols = ['unknown'] + list(periodic_table.keys())
+_max_valences = {n: v['max_valence'] for n, v in periodic_table.items()}
+_max_total_bond_order = {n: v['max_total_bond_order'] for n, v in periodic_table.items()}
 
 _bond_type = {
     'Unknown': 0,
     'Single': 1,
     'Double': 2,
     'Triple': 3,
     'Aromatic': 5,
@@ -289,15 +293,19 @@
         to_pop_atom_idx = set_atoms_idx.difference(set_ob_atoms_idx)
 
         # Pop redundant stored atoms
         for pop_idx in to_pop_atom_idx:
             atoms.pop(pop_idx)
 
         # Add create new atoms, its corresponding obBond in the obMol but lacking in atom repository
-        atoms = {i: atoms.get(i, Atom(self.ob_mol.GetAtomById(i), mol=self)) for i in set_ob_atoms_idx}
+        for oba in ob.OBMolAtomIter(self.ob_mol):
+            atom = atoms.setdefault(oba.GetId(), Atom(oba, mol=self))
+            atom.ob_atom = oba
+
+        # atoms = {i: atoms.get(i, Atom(self.ob_mol.GetAtomById(i), mol=self)) for i in set_ob_atoms_idx}
 
         self._data['atoms'] = atoms
 
         return atoms
 
     def _load_bonds(self) -> Dict[int, 'Bond']:
         """
@@ -587,43 +595,43 @@
     def add_bond(
             self,
             atom1: Union[str, int, 'Atom'],
             atom2: Union[str, int, 'Atom'],
             bond_type: Union[str, int],
     ):
         """ Add a new bond into the molecule """
-        atoms = (atom1, atom2)
-        atom_idx = []
-        for a in atoms:
+        inputs = (atom1, atom2)
+        atoms: List[Atom] = []
+        for a in inputs:
             if isinstance(a, int):
-                atom_idx.append(a)
+                atoms.append(self.atoms[a])
             if isinstance(a, Atom):
-                atom_idx.append(a.ob_id)
+                atoms.append(a)
             if isinstance(a, str):
-                atom_idx.append(self.atom(a).ob_id)
+                atoms.append(self.atom(a))
 
         # Represent the bond type by int, refer to _bond_type dict
         bond_type = bond_type if isinstance(bond_type, int) else _bond_type[bond_type]
 
         # Try to add new OBMol
         # 'openbabel' has an odd behave that `index` of the `OBAtom` with various origin in the `OBMol`.
         # the `Id` of `OBAtom` from 0; but the `Idx` of `OBAtom` from 1.
         # To meet the convention, the `Id` is selected to be the unique `index` to specify `Atom`.
         # However, when try to add a `OBBond` to link each two `OBAtoms`, the `Idx` is the only method
         # to specify the atoms, so our `index` in `Atom` are added 1 to match the 'Idx'
-        success = self.ob_mol.AddBond(atom_idx[0] + 1, atom_idx[1] + 1, bond_type)
+        success = self.ob_mol.AddBond(atoms[0].ob_idx, atoms[1].ob_idx, bond_type)
 
         if success:
-            new_ob_bond_idx = [i for i in (ob.OBMolBondIter(self.ob_mol))][-1].GetIdx()
+            new_ob_bond_idx = [obb for obb in (ob.OBMolBondIter(self.ob_mol))][-1].GetIdx()
             bond = self._load_bonds()[new_ob_bond_idx]  # the new atoms should place in the terminal of the bond list
 
-        elif atom_idx[0] not in self.atom_indices:
+        elif atoms[0] not in self.atom_indices:
             raise KeyError("the start atom1 doesn't exist in molecule")
 
-        elif atom_idx[1] not in self.atom_indices:
+        elif atoms[1] not in self.atom_indices:
             raise KeyError("the end atom2 doesn't exist in molecule")
 
         else:
             raise RuntimeError('add bond not successful!')
 
         # Return the bond have add into the molecule
         return bond
@@ -666,25 +674,25 @@
     @property
     def angles(self):
         return [Angle(self, a_idx) for a_idx in ob.OBMolAngleIter(self.ob_mol)]
 
     def assign_bond_types(self):
         self.ob_mol.PerceiveBondOrders()
 
-    def atom(self, idx_label: Union[int, str]) -> 'Atom':
+    def atom(self, id_label: Union[int, str]) -> 'Atom':
         """ get atom by label or idx """
         if not self.is_labels_unique:
             print(AttributeError('the molecule atoms labels are not unique!'))
 
-        if isinstance(idx_label, str):
-            return self.atoms[self.labels.index(idx_label)]
-        elif isinstance(idx_label, int):
-            return self.atoms[idx_label]
+        if isinstance(id_label, str):
+            return self.atoms[self.labels.index(id_label)]
+        elif isinstance(id_label, int):
+            return self.atoms[id_label]
         else:
-            raise TypeError(f'the given idx_label is expected to be int or string, but given {type(idx_label)}')
+            raise TypeError(f'the given idx_label is expected to be int or string, but given {type(id_label)}')
         
     @property
     def atom_num(self):
         return self.ob_mol.NumAtoms()
 
     @property
     def atoms(self) -> List['Atom']:
@@ -902,15 +910,16 @@
 
         # generate Bonds in new Molecule with same graph pattern in this Molecule
         for bond in self.bonds:
             clone_mol.add_bond(*bond.atoms, bond_type=bond.type)
 
         return clone_mol
 
-    def copy_data(self):
+    @property
+    def data(self):
         return copy.copy(self._data)
 
     def compact_crystal(self, inplace=False):
         """"""
         mol = self if inplace else self.copy()
         lattice_params = np.concatenate((self.xyz_diff, [90., 90., 90.]))
 
@@ -1148,14 +1157,24 @@
     @property
     def is_labels_unique(self):
         """ Determine whether all atom labels are unique """
         labels = set(self.labels)
         return len(labels) == self.atom_num
 
     @property
+    def is_organic(self):
+        """ To judge whether the molecule is organic, an organic compound is with carbon atoms and without metal """
+        if any(a.is_metal for a in self.atoms):
+            return False
+        elif any(a.symbol == 'C' for a in self.atoms):
+            return True
+
+        return False
+
+    @property
     def ob_mol(self):
         return self._data['ob_mol']
 
     def ob_mol_pop(self):
         data = self._data
 
         atoms: Dict[int, Atom] = data.get('atoms')
@@ -1549,15 +1568,15 @@
             elif isinstance(value, np.ndarray):
                 np.save(set_root.joinpath(f'{name}.npy'), value)
 
     def to_mix_mol(self):
         return MixSameAtomMol(_data=self._data)
 
     def to_mol(self):
-        return Molecule(self.copy_data())
+        return Molecule(self.data)
 
     @property
     def unique_all_atoms(self):
         return self.unique_atoms + self.unique_pseudo_atoms
 
     @property
     def unique_atoms(self):
@@ -1661,14 +1680,18 @@
     def __hash__(self):
         return hash(f'Atom({self.atomic_number})')
 
     @property
     def ob_atom(self):
         return self._data['ob_atom']
 
+    @ob_atom.setter
+    def ob_atom(self, oba):
+        self._data['ob_atom'] = oba
+
     def ob_atom_pop(self):
         return self._data.pop('ob_atom')
 
     def ob_atom_rewrap(self, ob_atom):
         self._data['ob_atom'] = ob_atom
 
     @property
@@ -1856,46 +1879,65 @@
         return tuple(self._attr_setters.keys())
 
     @property
     def ob_id(self):
         return self.ob_atom.GetId()
 
     @property
-    def is_aromatic(self):
-        return self.ob_atom.IsAromatic()
+    def ob_idx(self):
+        return self.ob_atom.GetIdx()
 
     @property
-    def is_metal(self):
-        return self.ob_atom.IsMetal()
+    def is_aromatic(self):
+        return self.ob_atom.IsAromatic()
 
     @property
     def is_chiral(self):
         return self.ob_atom.IsChiral()
 
     @property
+    def is_polar_hydrogen(self) -> bool:
+        """ Is this atom a hydrogen connected to a polar atom """
+        return self.ob_atom.IsPolarHydrogen()
+
+    @property
+    def is_metal(self):
+        return self.ob_atom.IsMetal()
+
+    @property
     def label(self):
         return self._data.get('label', self.symbol)
 
     @label.setter
     def label(self, value):
         self._set_label(value)
 
     @property
+    def link_degree(self) -> int:
+        """ the degree of the atom in their parent molecule """
+        return self.ob_atom.GetTotalDegree()
+
+    @property
     def mass(self):
         return self.ob_atom.GetAtomicMass()
 
     @property
+    def max_total_bond_order(self):
+        return _max_total_bond_order[self.symbol]
+
+    @property
     def molecule(self) -> Molecule:
         return self.mol
 
     @property
     def neighbours(self):
         """ Get all atoms bond with this atom in same molecule """
         if self.mol:
-            return [self.mol.atoms[ob_atom.GetId()] for ob_atom in ob.OBAtomAtomIter(self.ob_atom)]
+            _ = self.mol.atoms  # update the atoms dict
+            return [self.mol.data.get('atoms')[ob_atom.GetId()] for ob_atom in ob.OBAtomAtomIter(self.ob_atom)]
         else:
             return []
 
     @property
     def partial_charge(self):
         return self.ob_atom.GetPartialCharge()
 
@@ -1914,14 +1956,24 @@
     def spin_density(self, spin_density: float):
         self._set_spin_density(spin_density)
 
     @property
     def symbol(self):
         return _symbols[self.atomic_number]
 
+    @property
+    def valence(self) -> int:
+        """ The current number of explicit connections """
+        return self.ob_atom.GetTotalValence()
+
+    @property
+    def valence_max(self):
+        """ The implicit valence of this atom type (i.e. maximum number of connections expected) """
+        return _max_valences[self.symbol]
+
 
 class PseudoAtom(Wrapper, ABC):
     """ A data wrapper for pseudo atom """
     def __init__(self, symbol: str, mass: float, coordinates: Union[Sequence, np.ndarray], **kwargs):
         if isinstance(coordinates, Sequence):
             coordinates = np.array(coordinates)
```

### Comparing `hotpot-zzy-0.2.0/hotpot/data/force_field/UFF/LJ.json` & `hotpot-zzy-0.2.1/hotpot/data/force_field/UFF/LJ.json`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.0/hotpot/data/force_field/aMaterials/SiC.tersoff` & `hotpot-zzy-0.2.1/hotpot/data/force_field/aMaterials/SiC.tersoff`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.0/hotpot/tanks/lmp/base.py` & `hotpot-zzy-0.2.1/hotpot/tanks/lmp/base.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.0/hotpot/tanks/lmp/gcmc.py` & `hotpot-zzy-0.2.1/hotpot/tanks/lmp/gcmc.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.0/hotpot/tanks/lmp/materials.py` & `hotpot-zzy-0.2.1/hotpot/tanks/lmp/materials.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.0/hotpot/tanks/quantum.py` & `hotpot-zzy-0.2.1/hotpot/tanks/quantum.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.0/hotpot/tmo.py` & `hotpot-zzy-0.2.1/hotpot/tmo.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.0/hotpot/tools.py` & `hotpot-zzy-0.2.1/hotpot/tools.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.0/hotpot/utils/units_convert.py` & `hotpot-zzy-0.2.1/hotpot/utils/units_convert.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.0/hotpot_zzy.egg-info/SOURCES.txt` & `hotpot-zzy-0.2.1/hotpot_zzy.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -8,22 +8,17 @@
 hotpot/tools.py
 hotpot/data/periodic_table.json
 hotpot/data/units.json
 hotpot/data/force_field/contents.json
 hotpot/data/force_field/UFF/LJ.json
 hotpot/data/force_field/aMaterials/SiC.tersoff
 hotpot/tanks/__init__.py
+hotpot/tanks/cc.py
 hotpot/tanks/features.py
 hotpot/tanks/quantum.py
-hotpot/tanks/dl/__init__.py
-hotpot/tanks/dl/bert.py
-hotpot/tanks/dl/datasets.py
-hotpot/tanks/dl/graph_learning.py
-hotpot/tanks/dl/models/__init__.py
-hotpot/tanks/dl/models/dp.py
 hotpot/tanks/lmp/__init__.py
 hotpot/tanks/lmp/base.py
 hotpot/tanks/lmp/gcmc.py
 hotpot/tanks/lmp/materials.py
 hotpot/utils/__init__.py
 hotpot/utils/units_convert.py
 hotpot_zzy.egg-info/PKG-INFO
```

### Comparing `hotpot-zzy-0.2.0/test/test_amorphous_maker.py` & `hotpot-zzy-0.2.1/test/test_amorphous_maker.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.0/test/test_bundle.py` & `hotpot-zzy-0.2.1/test/test_bundle.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.0/test/test_lmp.py` & `hotpot-zzy-0.2.1/test/test_lmp.py`

 * *Files identical despite different names*

