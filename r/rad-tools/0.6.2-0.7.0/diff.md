# Comparing `tmp/rad-tools-0.6.2.tar.gz` & `tmp/rad-tools-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rad-tools-0.6.2.tar", last modified: Mon Jun  5 22:29:12 2023, max compression
+gzip compressed data, was "rad-tools-0.7.0.tar", last modified: Tue Jun  6 00:13:32 2023, max compression
```

## Comparing `rad-tools-0.6.2.tar` & `rad-tools-0.7.0.tar`

### file list

```diff
@@ -1,48 +1,56 @@
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-05 22:29:12.758428 rad-tools-0.6.2/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1071 2022-10-03 15:21:14.000000 rad-tools-0.6.2/LICENSE.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2829 2023-06-05 22:29:12.757679 rad-tools-0.6.2/PKG-INFO
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2122 2023-06-05 22:25:50.000000 rad-tools-0.6.2/README.rst
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-05 22:29:12.730801 rad-tools-0.6.2/rad_tools/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      561 2023-06-05 22:27:45.000000 rad-tools-0.6.2/rad_tools/__init__.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-05 22:29:12.737018 rad-tools-0.6.2/rad_tools/dos/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      183 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/dos/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    21722 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/dos/dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    22436 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/dos/pdos.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-05 22:29:12.741272 rad-tools-0.6.2/rad_tools/exchange/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      253 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/exchange/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     7700 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/exchange/bond.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    28094 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/exchange/model.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1198 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/exchange/template.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-05 22:29:12.742967 rad-tools-0.6.2/rad_tools/io/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      547 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/io/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1930 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/io/internal.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4054 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/io/tb2j.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-05 22:29:12.745403 rad-tools-0.6.2/rad_tools/kpoints/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      616 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/kpoints/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    30577 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/kpoints/high_symmetry_point.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3626 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/kpoints/kpoints.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1284 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/map.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3372 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/routines.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-05 22:29:12.751292 rad-tools-0.6.2/rad_tools/score/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1539 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/score/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4512 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/score/extract_tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3715 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/score/identify_wannier_centres.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4705 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/score/make_template.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    13248 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/score/plot_dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     9938 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/score/plot_tb2j.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-05 22:29:12.734930 rad-tools-0.6.2/rad_tools.egg-info/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2829 2023-06-05 22:29:12.000000 rad-tools-0.6.2/rad_tools.egg-info/PKG-INFO
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1008 2023-06-05 22:29:12.000000 rad-tools-0.6.2/rad_tools.egg-info/SOURCES.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)        1 2023-06-05 22:29:12.000000 rad-tools-0.6.2/rad_tools.egg-info/dependency_links.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       32 2023-06-05 22:29:12.000000 rad-tools-0.6.2/rad_tools.egg-info/requires.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       10 2023-06-05 22:29:12.000000 rad-tools-0.6.2/rad_tools.egg-info/top_level.txt
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-05 22:29:12.756896 rad-tools-0.6.2/scripts/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3225 2023-03-30 12:48:24.000000 rad-tools-0.6.2/scripts/compute-energies.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2933 2023-03-30 12:48:24.000000 rad-tools-0.6.2/scripts/phonopy-plotter.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      293 2023-06-05 22:25:14.000000 rad-tools-0.6.2/scripts/rad-extract-tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      305 2023-06-05 22:25:14.000000 rad-tools-0.6.2/scripts/rad-identify-wannier-centres.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      294 2023-06-05 22:25:14.000000 rad-tools-0.6.2/scripts/rad-make-template.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      289 2023-06-05 22:25:14.000000 rad-tools-0.6.2/scripts/rad-plot-dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      290 2023-06-05 22:25:14.000000 rad-tools-0.6.2/scripts/rad-plot-tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-05 22:29:12.758567 rad-tools-0.6.2/setup.cfg
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1403 2023-06-05 22:25:51.000000 rad-tools-0.6.2/setup.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-06 00:13:32.507400 rad-tools-0.7.0/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1071 2022-10-03 15:21:14.000000 rad-tools-0.7.0/LICENSE.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-06 00:13:32.506784 rad-tools-0.7.0/PKG-INFO
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2139 2023-06-05 23:32:40.000000 rad-tools-0.7.0/README.rst
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-06 00:13:32.455300 rad-tools-0.7.0/rad_tools.egg-info/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-06 00:13:32.000000 rad-tools-0.7.0/rad_tools.egg-info/PKG-INFO
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1203 2023-06-06 00:13:32.000000 rad-tools-0.7.0/rad_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)        1 2023-06-06 00:13:32.000000 rad-tools-0.7.0/rad_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-06 00:13:32.000000 rad-tools-0.7.0/rad_tools.egg-info/requires.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)        9 2023-06-06 00:13:32.000000 rad-tools-0.7.0/rad_tools.egg-info/top_level.txt
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-06 00:13:32.457785 rad-tools-0.7.0/radtools/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      624 2023-06-06 00:13:06.000000 rad-tools-0.7.0/radtools/__init__.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-06 00:13:32.467176 rad-tools-0.7.0/radtools/crystal/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      292 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/crystal/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     6865 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/crystal/atom.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1183 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/crystal/atom_types.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    87419 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/crystal/bravais_lattice.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     8896 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/crystal/crystal.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    23756 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/crystal/identify.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    36933 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/crystal/lattice.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-06 00:13:32.473734 rad-tools-0.7.0/radtools/dos/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      183 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/dos/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    21701 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/dos/dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    22428 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/dos/pdos.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-06 00:13:32.480558 rad-tools-0.7.0/radtools/exchange/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      299 2023-06-06 00:13:06.000000 rad-tools-0.7.0/radtools/exchange/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    45538 2023-06-06 00:13:06.000000 rad-tools-0.7.0/radtools/exchange/hamiltonian.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    12326 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/exchange/parameter.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1198 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/exchange/template.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-06 00:13:32.483348 rad-tools-0.7.0/radtools/io/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      421 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/io/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1929 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/io/internal.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     5458 2023-06-06 00:13:06.000000 rad-tools-0.7.0/radtools/io/tb2j.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-06 00:13:32.485986 rad-tools-0.7.0/radtools/kpoints/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      615 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/kpoints/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4280 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/kpoints/high_symmetry_point.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3625 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/kpoints/kpoints.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1284 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/map.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    18633 2023-06-06 00:13:06.000000 rad-tools-0.7.0/radtools/routines.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-06 00:13:32.492839 rad-tools-0.7.0/radtools/score/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1639 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/score/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4506 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/score/extract_tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3715 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/score/identify_wannier_centres.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4695 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/score/make_template.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    13280 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/score/plot_dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     9920 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/score/plot_tb2j.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-06 00:13:32.505099 rad-tools-0.7.0/scripts/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3225 2023-03-30 12:48:24.000000 rad-tools-0.7.0/scripts/compute-energies.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2933 2023-03-30 12:48:24.000000 rad-tools-0.7.0/scripts/phonopy-plotter.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      256 2023-06-05 23:32:40.000000 rad-tools-0.7.0/scripts/rad-extract-tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      268 2023-06-05 23:32:40.000000 rad-tools-0.7.0/scripts/rad-identify-wannier-centres.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      257 2023-06-05 23:32:40.000000 rad-tools-0.7.0/scripts/rad-make-template.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      252 2023-06-05 23:32:40.000000 rad-tools-0.7.0/scripts/rad-plot-dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      253 2023-06-05 23:32:40.000000 rad-tools-0.7.0/scripts/rad-plot-tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-06 00:13:32.507590 rad-tools-0.7.0/setup.cfg
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1411 2023-06-05 23:35:15.000000 rad-tools-0.7.0/setup.py
```

### Comparing `rad-tools-0.6.2/LICENSE.txt` & `rad-tools-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rad-tools-0.6.2/PKG-INFO` & `rad-tools-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad-tools
-Version: 0.6.2
+Version: 0.7.0
 Summary: Scripts for condense matter calculations and post-processing.
 Home-page: https://rad-tools.org/en/stable/
 Download-URL: https://github.com/adrybakov/rad-tools.git
 Author: Andrey Rybakov
 Author-email: rybakov.ad@icloud.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
@@ -45,26 +45,28 @@
 
 It is expected to be used in two ways:
 
 * As Python library
 
 * Via scripts (i.e. usage from command line)
 
-For the detailed descriprion check
+For the detailed description check
 `documentation. <https://rad-tools.org>`_
 
 Installation
 ============
 
 Requirement for RAD-tools installation are:
 
 * Python itself (>=3.6)
 * NumPy
+* SciPy
 * matplotlib
 * tqdm
+* termcolor
 
 RAD-tools can be installed with ``pip`` or from source.
 
 pip
 ---
 
 To install RAD-tools, run (you may need to use ``pip3``):
@@ -97,12 +99,12 @@
 Additionally you may run the unit tests, 
 which requires pytest (requires Python 3.7+) to be installed:
 
 .. code-block:: console
 
    make test
 
-To install RAD-tools, run (you may need to use ``pip3``):
+To install pytest, run (you may need to use ``pip3``):
 
 .. code-block:: console
 
    pip install pytest
```

### Comparing `rad-tools-0.6.2/README.rst` & `rad-tools-0.7.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -26,26 +26,28 @@
 
 It is expected to be used in two ways:
 
 * As Python library
 
 * Via scripts (i.e. usage from command line)
 
-For the detailed descriprion check
+For the detailed description check
 `documentation. <https://rad-tools.org>`_
 
 Installation
 ============
 
 Requirement for RAD-tools installation are:
 
 * Python itself (>=3.6)
 * NumPy
+* SciPy
 * matplotlib
 * tqdm
+* termcolor
 
 RAD-tools can be installed with ``pip`` or from source.
 
 pip
 ---
 
 To install RAD-tools, run (you may need to use ``pip3``):
@@ -78,12 +80,12 @@
 Additionally you may run the unit tests, 
 which requires pytest (requires Python 3.7+) to be installed:
 
 .. code-block:: console
 
    make test
 
-To install RAD-tools, run (you may need to use ``pip3``):
+To install pytest, run (you may need to use ``pip3``):
 
 .. code-block:: console
 
    pip install pytest
```

### Comparing `rad-tools-0.6.2/rad_tools/__init__.py` & `rad-tools-0.7.0/radtools/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 r"""
 All tools from the package.
 
 
 |version|
 """
 
-__version__ = "0.6.2"
+__version__ = "0.7.0"
 
-
-from . import dos, exchange, io, kpoints, score
+from . import crystal, dos, exchange, io, kpoints, score
+from .crystal import *
 from .dos import *
 from .exchange import *
 from .io import *
 from .kpoints import *
 from .routines import *
 from .score import *
 
 __all__ = []
 __all__.extend(score.__all__)
 __all__.extend(io.__all__)
 __all__.extend(exchange.__all__)
 __all__.extend(kpoints.__all__)
 __all__.extend(dos.__all__)
 __all__.extend(routines.__all__)
+__all__.extend(crystal.__all__)
 
 
 if __name__ == "__main__":
     local_variables = dict(locals())
     for i in local_variables:
         print(i)
```

### Comparing `rad-tools-0.6.2/rad_tools/dos/dos.py` & `rad-tools-0.7.0/radtools/dos/dos.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 import re
 from os import walk
 from os.path import join
 
 import matplotlib.pyplot as plt
 import numpy as np
 
-from rad_tools.dos.pdos import PDOSQE
+from radtools.dos.pdos import PDOSQE
 
 
 class DOSQE:
     r"""
     Analyse the folder with the |QE|_ results and store all information.
 
     Parameters
     ----------
     seedname : str
         Seedname for the |QE|_ output files.
     input_folder : str
         Path to the folder with |QE|_ output files.
-    energy_window : tuple, default None
+    energy_window : tuple, optional
         Energy limits, necessary for correct plotting.
 
     Attributes
     ----------
     seedname : str
         Seedname for the |QE|_ output files.
     energy : array
@@ -416,15 +416,15 @@
         r"""
         Return list of wave function labels for particular atom.
 
         Parameters
         ----------
         atom : str
             Label of an atom.
-        atom_number : int, default None
+        atom_number : int, optional
             Number of an atom. If ``None`` then return wfc and wfc numbers of first atom.
 
         Returns
         -------
         wfcs : list
             List of wave function labels and numbers
 
@@ -447,15 +447,15 @@
         ----------
         atom : str
             Name of the atom type.
         wfc : str
             Name of the projector wave function.
         wfc_numbers : int
             Number of wave function projector.
-        atom_numbers : list or int, default None
+        atom_numbers : list or int, optional
             If ``None``, then PDOS summed over all atom numbers for ``atom``.
 
         Returns
         -------
         pdos : :py:class:`PDOSQE`
             Partial density of states, orbital-resolved.
         """
@@ -528,17 +528,17 @@
         ----------
         output_name : str
             Name of the output file.
         interactive : bool, default False
             Whether to plot in interactive |matplotlib|_ window.
         efermi : float, default 0
             Fermi energy. Zero of energy scale is shifted to it.
-        xlim : tuple, default None
+        xlim : tuple, optional
             Limits for energy scale.
-        ylim : tuple, default None
+        ylim : tuple, optional
             Limits for dos scale.
         save_pickle : bool, default False
             Whether to save figure as a .pickle file.
             Helps for custom modification of particular figures.
         """
         fig, ax = plt.subplots(figsize=(8, 4))
```

### Comparing `rad-tools-0.6.2/rad_tools/dos/pdos.py` & `rad-tools-0.7.0/radtools/dos/pdos.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     projectors : list
         Names of the projectors.
         If :py:attr:`projectors_group` has the form "l" or "l_j",
         where l is "s", "p", "d", "f" and j is the total angular momentum,
         the projectors are assigned automatically,
         otherwise it is necessary to provide :math:`n` projectors manually.
         The names of projectors are directly used in the plots.
-    ldos : |array_like|_, default None
+    ldos : |array_like|_, optional
         Local density of states. Sum of partial density of states over all projectors.
         Computed based on ``pdos`` if not provided.
         Shape is assumed to be:
 
         * Spin-polarized, k-resolved: :math:`(2, n_k, n_e)`
         * Spin-unpolarized, k-resolved: :math:`(n_k, n_e)`
         * Spin-polarized, non k-resolved: :math:`(2, n_e)`
@@ -528,15 +528,15 @@
     ----------
     pdos : :py:class:`.PDOS`
         PDOS for the plot.
     efermi : float, default 0
         Fermi energy.
     output_name : str, default "pdos"
         output_name for the plot file. Extension ".png" is added at the end.
-    title : str, default None
+    title : str, optional
         Title of the plot. Passed to the ``ax.set_title()``.
     xlim : tuple
         limits for the x (Energy) axis
     ylim : tuple
         limits for the y (PDOS) axis
     relative : bool, default False
         Relative plot style.
```

### Comparing `rad-tools-0.6.2/rad_tools/exchange/template.py` & `rad-tools-0.7.0/radtools/exchange/template.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.6.2/rad_tools/io/internal.py` & `rad-tools-0.7.0/radtools/io/internal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 r"""
 Input-output for the files related with this package.
 """
 
-from rad_tools.exchange.template import ExchangeTemplate
+from radtools.exchange.template import ExchangeTemplate
 
 
 def read_template(filename):
     r"""
     Read template from the template file.
```

### Comparing `rad-tools-0.6.2/rad_tools/kpoints/__init__.py` & `rad-tools-0.7.0/radtools/kpoints/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Module for constructing the k-points paths and high-symmetry k-points [1]_. 
 
 Examples
 --------
 
 .. code-block:: python
 
-    from rad_tools.kpoints import HighSymmetryPoints
+    from radtools.kpoints import HighSymmetryPoints
 
     hexagonal = HighSymmetryPoints().hex()
 
 References
 ----------
 .. [1] 
     Setyawan, W. and Curtarolo, S., 2010.
```

### Comparing `rad-tools-0.6.2/rad_tools/kpoints/kpoints.py` & `rad-tools-0.7.0/radtools/kpoints/kpoints.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from math import sqrt
 
 import numpy as np
 
-from rad_tools.kpoints.high_symmetry_point import HighSymmetryPoints
+from radtools.kpoints.high_symmetry_point import HighSymmetryPoints
 
 
 class KPoints(HighSymmetryPoints):
     r"""
     K-points
     """
```

### Comparing `rad-tools-0.6.2/rad_tools/map.py` & `rad-tools-0.7.0/radtools/map.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.6.2/rad_tools/score/__init__.py` & `rad-tools-0.7.0/radtools/score/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 r"""
 Most of the scripts are moved to the library and could be called through 
-the corresponding ``manager`` function, which results in the behaviour 
-analogous to the command line interface.
+the corresponding function, which results in the behaviour 
+analogous to the command line interface. The common logic for the name: 
+If script is called "rad-script-name", then the function is called "script-name".
 
 .. hint::
     Long names of the arguments have to be used, i.e. ``input_path``, not ``ip``.
 
 .. admonition:: Example
 
     Identifying Wannier centres from the file "seedname_centres.xyz"
     with increased span of 0.2, saving the result in the file 
     "identified_centres" of the current directory:
 
     .. code-block:: python
 
-        from rad_tools import identify_wannier_centres
+        from radtools import identify_wannier_centres
         
         identify_wannier_centres("seedname_centres.xyz", 
             span = 0.2, 
             output_path = ".", 
             output_name="identified_centres",
             no_colour=False)
 
     Makings template based on the "exchange.out" TB2J file, 
     filtering by maximum distance of 5, saving the output in 
     the file "template.txt" of the current folder:
 
     .. code-block:: python
 
-        from rad_tools import make_template
+        from radtools import make_template
         
         make_template(output_name="template",
             input_filename="exchange.out",
             max_distance=5)
 """
 
 from .extract_tb2j import manager as extract_tb2j
```

### Comparing `rad-tools-0.6.2/rad_tools/score/extract_tb2j.py` & `rad-tools-0.7.0/radtools/score/extract_tb2j.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from calendar import month_name
 from datetime import datetime
 from os import makedirs
 from os.path import abspath, join
 
 from termcolor import cprint
 
-from rad_tools import __version__ as version
-from rad_tools.io import read_tb2j_model
-from rad_tools.io.internal import read_template
+from radtools import __version__ as version
+from radtools.io.internal import read_template
+from radtools.io.tb2j import read_tb2j_model
 
 
 def manager(
     input_filename,
     template_file,
     output_path=".",
     output_name=None,
@@ -51,16 +51,16 @@
     template = read_template(template_file)
     summary_txt = model.summary_as_txt(
         template=template,
         decimals=decimals,
         force_symmetry=force_symmetry,
         isotropic=isotropic,
         anisotropic=anisotropic,
-        out_matrix=matrix,
-        out_dmi=dmi,
+        matrix=matrix,
+        dmi=dmi,
     )
 
     if output_name is not None:
         with open(join(output_path, output_name + ".txt"), "w") as out_file:
             out_file.write(
                 f"Exchange values are extracted from: {input_filename}\n"
                 + f"on {cd.day} {month_name[cd.month]} {cd.year}"
```

### Comparing `rad-tools-0.6.2/rad_tools/score/identify_wannier_centres.py` & `rad-tools-0.7.0/radtools/score/identify_wannier_centres.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.6.2/rad_tools/score/make_template.py` & `rad-tools-0.7.0/radtools/score/make_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from datetime import datetime
 from os import makedirs
 from os.path import abspath, split
 
 import numpy as np
 from termcolor import cprint
 
-from rad_tools import __version__ as version
-from rad_tools.io.tb2j import read_exchange_model
+from radtools import __version__ as version
+from radtools.io.tb2j import read_tb2j_model
 
 
 def manager(
     output_name="template",
     input_filename=None,
     R_vector=None,
     max_distance=None,
@@ -79,15 +79,15 @@
         else:
             file.write(
                 f"Template is created based on the file: {input_filename}\n"
                 + f"on {cd.day} {month_name[cd.month]} {cd.year}"
                 + f" at {cd.hour}:{cd.minute}:{cd.second} by rad-tools {version}\n\n"
             )
 
-            model = read_exchange_model(input_filename, quiet=not verbose)
+            model = read_tb2j_model(input_filename, quiet=not verbose)
             model.filter(
                 min_distance=min_distance, max_distance=max_distance, R_vector=R_vector
             )
             file.write(
                 "=" * 20
                 + "\n"
                 + "Neighbors template:\n"
```

### Comparing `rad-tools-0.6.2/rad_tools/score/plot_dos.py` & `rad-tools-0.7.0/radtools/score/plot_dos.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from argparse import ArgumentParser
 from os import makedirs, walk
 from os.path import abspath, join
 
 from termcolor import cprint
 from tqdm import tqdm
 
-from rad_tools.dos import DOSQE, PDOS, plot_projected
+from radtools.dos.dos import DOSQE
+from radtools.dos.pdos import PDOS, plot_projected
 
 
 def detect_seednames(input_path):
     r"""
     Analyze input folder, detects seednames for the dos output files.
 
     Parameters
```

### Comparing `rad-tools-0.6.2/rad_tools/score/plot_tb2j.py` & `rad-tools-0.7.0/radtools/score/plot_tb2j.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from os import makedirs
 from os.path import abspath, join
 
 import numpy as np
 from matplotlib import pyplot as plt
 from termcolor import cprint
 
-from rad_tools.io.internal import read_template
-from rad_tools.io.tb2j import read_exchange_model
-from rad_tools.routines import atom_mark_to_latex, rot_angle
+from radtools.io.internal import read_template
+from radtools.io.tb2j import read_tb2j_model
+from radtools.routines import atom_mark_to_latex, rot_angle
 
 
 def manager(
     input_filename,
     output_path=".",
     output_name="exchange",
     what_to_plot="iso",
@@ -52,15 +52,15 @@
 
     if R_vector is not None:
         R_vector = np.array(R_vector[: len(R_vector) // 3 * 3], dtype=int).reshape(
             (len(R_vector) // 3, 3)
         )
         R_vector = list(map(tuple, R_vector.tolist()))
 
-    model = read_exchange_model(input_filename, quiet=not verbose)
+    model = read_tb2j_model(input_filename, quiet=not verbose)
     if template_file is not None:
         template = read_template(template_file)
     else:
         template = None
 
     if force_symmetry:
         model.force_symmetry(template=template)
@@ -91,48 +91,47 @@
         else:
             fig = plt.figure(figsize=(6.4, 4.8 * Y / X))
         ax = fig.add_axes([0.1, 0.1, 0.8, 0.8])
         ax.set_aspect("equal")
         ax.set_xlabel("x, Angstroms")
         ax.set_ylabel("y, Angstroms")
 
-        for atom1, atom2, R in model:
-            bond = model[(atom1, atom2, R)]
-            dis = model.get_distance(atom1, atom2, R)
-            x1, y1, z1 = model.get_atom_coordinates(atom1)
-            x2, y2, z2 = model.get_atom_coordinates(atom2, R)
+        for atom1, atom2, R, J in model:
+            dis = model.crystal.get_distance(atom1, atom2, R)
+            x1, y1, z1 = model.crystal.get_atom_coordinates(atom1)
+            x2, y2, z2 = model.crystal.get_atom_coordinates(atom2, R)
             xm = (x1 + x2) / 2
             ym = (y1 + y2) / 2
             zm = (z1 + z2) / 2
 
             ax.scatter(x1, y1, s=100 * fig.dpi / 72.0, c="white")
             ax.scatter(x2, y2, s=100 * fig.dpi / 72.0, c="white")
 
             ax.text(
                 x2,
                 y2,
-                atom_mark_to_latex(atom2),
+                atom_mark_to_latex(atom2.literal),
                 va="center",
                 ha="center",
                 fontsize=1.5 * fontsize * scale_atoms,
             )
             ax.text(
                 x1,
                 y1,
-                atom_mark_to_latex(atom1),
+                atom_mark_to_latex(atom1.literal),
                 va="center",
                 ha="center",
                 fontsize=1.5 * fontsize * scale_atoms,
                 color="#A04F4D",
             )
             if wtp == "iso":
                 ax.text(
                     xm,
                     ym,
-                    str(round(bond.iso, 4)),
+                    str(round(J.iso, 4)),
                     va="bottom",
                     ha=ha,
                     rotation_mode="anchor",
                     rotation=rot_angle(x2 - x1, y2 - y1, dummy=dummy),
                     fontsize=fontsize * scale_data,
                 )
             elif wtp == "distance":
@@ -146,15 +145,15 @@
                     rotation=rot_angle(x2 - x1, y2 - y1, dummy=dummy),
                     fontsize=fontsize * scale_data,
                 )
             elif wtp == "dmi":
                 ax.text(
                     xm,
                     ym,
-                    str(round(sqrt(np.sum(bond.dmi**2)), 4)),
+                    str(round(sqrt(np.sum(J.dmi**2)), 4)),
                     va="bottom",
                     ha=ha,
                     rotation_mode="anchor",
                     rotation=rot_angle(x2 - x1, y2 - y1, dummy=dummy),
                     fontsize=fontsize * scale_data,
                 )
```

### Comparing `rad-tools-0.6.2/rad_tools.egg-info/PKG-INFO` & `rad-tools-0.7.0/rad_tools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad-tools
-Version: 0.6.2
+Version: 0.7.0
 Summary: Scripts for condense matter calculations and post-processing.
 Home-page: https://rad-tools.org/en/stable/
 Download-URL: https://github.com/adrybakov/rad-tools.git
 Author: Andrey Rybakov
 Author-email: rybakov.ad@icloud.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
@@ -45,26 +45,28 @@
 
 It is expected to be used in two ways:
 
 * As Python library
 
 * Via scripts (i.e. usage from command line)
 
-For the detailed descriprion check
+For the detailed description check
 `documentation. <https://rad-tools.org>`_
 
 Installation
 ============
 
 Requirement for RAD-tools installation are:
 
 * Python itself (>=3.6)
 * NumPy
+* SciPy
 * matplotlib
 * tqdm
+* termcolor
 
 RAD-tools can be installed with ``pip`` or from source.
 
 pip
 ---
 
 To install RAD-tools, run (you may need to use ``pip3``):
@@ -97,12 +99,12 @@
 Additionally you may run the unit tests, 
 which requires pytest (requires Python 3.7+) to be installed:
 
 .. code-block:: console
 
    make test
 
-To install RAD-tools, run (you may need to use ``pip3``):
+To install pytest, run (you may need to use ``pip3``):
 
 .. code-block:: console
 
    pip install pytest
```

### Comparing `rad-tools-0.6.2/rad_tools.egg-info/SOURCES.txt` & `rad-tools-0.7.0/rad_tools.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 LICENSE.txt
 README.rst
 setup.py
-rad_tools/__init__.py
-rad_tools/map.py
-rad_tools/routines.py
 rad_tools.egg-info/PKG-INFO
 rad_tools.egg-info/SOURCES.txt
 rad_tools.egg-info/dependency_links.txt
 rad_tools.egg-info/requires.txt
 rad_tools.egg-info/top_level.txt
-rad_tools/dos/__init__.py
-rad_tools/dos/dos.py
-rad_tools/dos/pdos.py
-rad_tools/exchange/__init__.py
-rad_tools/exchange/bond.py
-rad_tools/exchange/model.py
-rad_tools/exchange/template.py
-rad_tools/io/__init__.py
-rad_tools/io/internal.py
-rad_tools/io/tb2j.py
-rad_tools/kpoints/__init__.py
-rad_tools/kpoints/high_symmetry_point.py
-rad_tools/kpoints/kpoints.py
-rad_tools/score/__init__.py
-rad_tools/score/extract_tb2j.py
-rad_tools/score/identify_wannier_centres.py
-rad_tools/score/make_template.py
-rad_tools/score/plot_dos.py
-rad_tools/score/plot_tb2j.py
+radtools/__init__.py
+radtools/map.py
+radtools/routines.py
+radtools/crystal/__init__.py
+radtools/crystal/atom.py
+radtools/crystal/atom_types.py
+radtools/crystal/bravais_lattice.py
+radtools/crystal/crystal.py
+radtools/crystal/identify.py
+radtools/crystal/lattice.py
+radtools/dos/__init__.py
+radtools/dos/dos.py
+radtools/dos/pdos.py
+radtools/exchange/__init__.py
+radtools/exchange/hamiltonian.py
+radtools/exchange/parameter.py
+radtools/exchange/template.py
+radtools/io/__init__.py
+radtools/io/internal.py
+radtools/io/tb2j.py
+radtools/kpoints/__init__.py
+radtools/kpoints/high_symmetry_point.py
+radtools/kpoints/kpoints.py
+radtools/score/__init__.py
+radtools/score/extract_tb2j.py
+radtools/score/identify_wannier_centres.py
+radtools/score/make_template.py
+radtools/score/plot_dos.py
+radtools/score/plot_tb2j.py
 scripts/compute-energies.py
 scripts/phonopy-plotter.py
 scripts/rad-extract-tb2j.py
 scripts/rad-identify-wannier-centres.py
 scripts/rad-make-template.py
 scripts/rad-plot-dos.py
 scripts/rad-plot-tb2j.py
```

### Comparing `rad-tools-0.6.2/scripts/compute-energies.py` & `rad-tools-0.7.0/scripts/compute-energies.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.6.2/scripts/phonopy-plotter.py` & `rad-tools-0.7.0/scripts/phonopy-plotter.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.6.2/setup.py` & `rad-tools-0.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-from rad_tools import __version__
+from radtools import __version__
 
 __version__ = __version__
 
 with open("README.rst", "r") as file:
     long_description = ""
     for line in file:
         long_description += line
@@ -25,15 +25,15 @@
         "scripts/phonopy-plotter.py",
         "scripts/rad-extract-tb2j.py",
         "scripts/rad-make-template.py",
         "scripts/rad-plot-dos.py",
         "scripts/rad-identify-wannier-centres.py",
         "scripts/compute-energies.py",
     ],
-    install_requires=["numpy", "matplotlib", "tqdm", "termcolor"],
+    install_requires=["numpy", "matplotlib", "scipy", "tqdm", "termcolor"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Chemistry",
         "Topic :: Scientific/Engineering :: Physics",
```

