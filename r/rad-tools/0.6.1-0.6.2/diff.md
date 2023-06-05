# Comparing `tmp/rad-tools-0.6.1.tar.gz` & `tmp/rad-tools-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rad-tools-0.6.1.tar", last modified: Sat May 13 01:38:04 2023, max compression
+gzip compressed data, was "rad-tools-0.6.2.tar", last modified: Mon Jun  5 22:29:12 2023, max compression
```

## Comparing `rad-tools-0.6.1.tar` & `rad-tools-0.6.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-05-13 01:38:04.090298 rad-tools-0.6.1/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1071 2022-10-03 15:21:14.000000 rad-tools-0.6.1/LICENSE.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2859 2023-05-13 01:38:04.089830 rad-tools-0.6.1/PKG-INFO
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2142 2023-05-12 23:13:20.000000 rad-tools-0.6.1/README.rst
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-05-13 01:38:04.064351 rad-tools-0.6.1/rad_tools/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      561 2023-05-13 01:32:49.000000 rad-tools-0.6.1/rad_tools/__init__.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-05-13 01:38:04.070122 rad-tools-0.6.1/rad_tools/dos/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      183 2023-05-13 01:31:59.000000 rad-tools-0.6.1/rad_tools/dos/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    21722 2023-05-13 01:08:44.000000 rad-tools-0.6.1/rad_tools/dos/dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    22436 2023-05-13 01:11:24.000000 rad-tools-0.6.1/rad_tools/dos/pdos.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-05-13 01:38:04.074891 rad-tools-0.6.1/rad_tools/exchange/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      253 2023-05-09 00:12:40.000000 rad-tools-0.6.1/rad_tools/exchange/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     7700 2023-05-13 01:07:33.000000 rad-tools-0.6.1/rad_tools/exchange/bond.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    28094 2023-05-13 01:21:46.000000 rad-tools-0.6.1/rad_tools/exchange/model.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1198 2023-05-13 01:12:42.000000 rad-tools-0.6.1/rad_tools/exchange/template.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-05-13 01:38:04.077418 rad-tools-0.6.1/rad_tools/io/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      547 2023-05-13 01:31:59.000000 rad-tools-0.6.1/rad_tools/io/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1930 2023-05-13 01:23:59.000000 rad-tools-0.6.1/rad_tools/io/internal.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4054 2023-05-13 01:24:34.000000 rad-tools-0.6.1/rad_tools/io/tb2j.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-05-13 01:38:04.081169 rad-tools-0.6.1/rad_tools/kpoints/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      616 2023-05-09 00:12:40.000000 rad-tools-0.6.1/rad_tools/kpoints/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    30577 2023-05-12 23:13:20.000000 rad-tools-0.6.1/rad_tools/kpoints/high_symmetry_point.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3626 2023-05-09 00:12:40.000000 rad-tools-0.6.1/rad_tools/kpoints/kpoints.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1284 2023-03-30 12:48:24.000000 rad-tools-0.6.1/rad_tools/map.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3372 2023-05-13 01:31:59.000000 rad-tools-0.6.1/rad_tools/routines.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-05-13 01:38:04.084943 rad-tools-0.6.1/rad_tools/score/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1539 2023-05-13 01:31:59.000000 rad-tools-0.6.1/rad_tools/score/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4512 2023-05-13 00:20:50.000000 rad-tools-0.6.1/rad_tools/score/extract_tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3715 2023-05-13 00:12:08.000000 rad-tools-0.6.1/rad_tools/score/identify_wannier_centres.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4705 2023-05-13 00:23:29.000000 rad-tools-0.6.1/rad_tools/score/make_template.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    13248 2023-05-13 01:31:59.000000 rad-tools-0.6.1/rad_tools/score/plot_dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     9938 2023-05-13 01:31:55.000000 rad-tools-0.6.1/rad_tools/score/plot_tb2j.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-05-13 01:38:04.067139 rad-tools-0.6.1/rad_tools.egg-info/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2859 2023-05-13 01:38:03.000000 rad-tools-0.6.1/rad_tools.egg-info/PKG-INFO
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1008 2023-05-13 01:38:04.000000 rad-tools-0.6.1/rad_tools.egg-info/SOURCES.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)        1 2023-05-13 01:38:03.000000 rad-tools-0.6.1/rad_tools.egg-info/dependency_links.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       32 2023-05-13 01:38:03.000000 rad-tools-0.6.1/rad_tools.egg-info/requires.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       10 2023-05-13 01:38:03.000000 rad-tools-0.6.1/rad_tools.egg-info/top_level.txt
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-05-13 01:38:04.089275 rad-tools-0.6.1/scripts/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3225 2023-03-30 12:48:24.000000 rad-tools-0.6.1/scripts/compute-energies.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2933 2023-03-30 12:48:24.000000 rad-tools-0.6.1/scripts/phonopy-plotter.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      293 2023-05-13 01:31:59.000000 rad-tools-0.6.1/scripts/rad-extract-tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      305 2023-05-13 01:31:59.000000 rad-tools-0.6.1/scripts/rad-identify-wannier-centres.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      294 2023-05-13 01:31:59.000000 rad-tools-0.6.1/scripts/rad-make-template.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      289 2023-05-13 01:31:59.000000 rad-tools-0.6.1/scripts/rad-plot-dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      290 2023-05-13 01:31:59.000000 rad-tools-0.6.1/scripts/rad-plot-tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-05-13 01:38:04.090456 rad-tools-0.6.1/setup.cfg
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1413 2023-05-12 23:45:26.000000 rad-tools-0.6.1/setup.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-05 22:29:12.758428 rad-tools-0.6.2/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1071 2022-10-03 15:21:14.000000 rad-tools-0.6.2/LICENSE.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2829 2023-06-05 22:29:12.757679 rad-tools-0.6.2/PKG-INFO
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2122 2023-06-05 22:25:50.000000 rad-tools-0.6.2/README.rst
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-05 22:29:12.730801 rad-tools-0.6.2/rad_tools/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      561 2023-06-05 22:27:45.000000 rad-tools-0.6.2/rad_tools/__init__.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-05 22:29:12.737018 rad-tools-0.6.2/rad_tools/dos/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      183 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/dos/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    21722 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/dos/dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    22436 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/dos/pdos.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-05 22:29:12.741272 rad-tools-0.6.2/rad_tools/exchange/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      253 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/exchange/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     7700 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/exchange/bond.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    28094 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/exchange/model.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1198 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/exchange/template.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-05 22:29:12.742967 rad-tools-0.6.2/rad_tools/io/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      547 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/io/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1930 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/io/internal.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4054 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/io/tb2j.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-05 22:29:12.745403 rad-tools-0.6.2/rad_tools/kpoints/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      616 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/kpoints/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    30577 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/kpoints/high_symmetry_point.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3626 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/kpoints/kpoints.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1284 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/map.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3372 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/routines.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-05 22:29:12.751292 rad-tools-0.6.2/rad_tools/score/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1539 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/score/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4512 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/score/extract_tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3715 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/score/identify_wannier_centres.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4705 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/score/make_template.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    13248 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/score/plot_dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     9938 2023-06-05 22:25:14.000000 rad-tools-0.6.2/rad_tools/score/plot_tb2j.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-05 22:29:12.734930 rad-tools-0.6.2/rad_tools.egg-info/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2829 2023-06-05 22:29:12.000000 rad-tools-0.6.2/rad_tools.egg-info/PKG-INFO
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1008 2023-06-05 22:29:12.000000 rad-tools-0.6.2/rad_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)        1 2023-06-05 22:29:12.000000 rad-tools-0.6.2/rad_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       32 2023-06-05 22:29:12.000000 rad-tools-0.6.2/rad_tools.egg-info/requires.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       10 2023-06-05 22:29:12.000000 rad-tools-0.6.2/rad_tools.egg-info/top_level.txt
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-05 22:29:12.756896 rad-tools-0.6.2/scripts/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3225 2023-03-30 12:48:24.000000 rad-tools-0.6.2/scripts/compute-energies.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2933 2023-03-30 12:48:24.000000 rad-tools-0.6.2/scripts/phonopy-plotter.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      293 2023-06-05 22:25:14.000000 rad-tools-0.6.2/scripts/rad-extract-tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      305 2023-06-05 22:25:14.000000 rad-tools-0.6.2/scripts/rad-identify-wannier-centres.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      294 2023-06-05 22:25:14.000000 rad-tools-0.6.2/scripts/rad-make-template.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      289 2023-06-05 22:25:14.000000 rad-tools-0.6.2/scripts/rad-plot-dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      290 2023-06-05 22:25:14.000000 rad-tools-0.6.2/scripts/rad-plot-tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-05 22:29:12.758567 rad-tools-0.6.2/setup.cfg
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1403 2023-06-05 22:25:51.000000 rad-tools-0.6.2/setup.py
```

### Comparing `rad-tools-0.6.1/LICENSE.txt` & `rad-tools-0.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rad-tools-0.6.1/PKG-INFO` & `rad-tools-0.6.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: rad-tools
-Version: 0.6.1
+Version: 0.6.2
 Summary: Scripts for condense matter calculations and post-processing.
-Home-page: https://rad-tools.adrybakov.com/en/stable/
+Home-page: https://rad-tools.org/en/stable/
 Download-URL: https://github.com/adrybakov/rad-tools.git
 Author: Andrey Rybakov
 Author-email: rybakov.ad@icloud.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -22,15 +22,15 @@
 *********
 Various scripts for condense matter calculations and post-processing.
 
 .. image:: https://badge.fury.io/py/rad-tools.svg
     :target: https://badge.fury.io/py/rad-tools
     
 .. image:: https://readthedocs.org/projects/rad-tools/badge/?version=stable
-    :target: https://rad-tools.adrybakov.com/en/stable/?badge=stable
+    :target: https://rad-tools.org/en/stable/?badge=stable
     :alt: Documentation Status
    
 .. image:: https://static.pepy.tech/personalized-badge/rad-tools?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads
  :target: https://pepy.tech/project/rad-tools
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
@@ -46,15 +46,15 @@
 It is expected to be used in two ways:
 
 * As Python library
 
 * Via scripts (i.e. usage from command line)
 
 For the detailed descriprion check
-`documentation. <https://rad-tools.adrybakov.com>`_
+`documentation. <https://rad-tools.org>`_
 
 Installation
 ============
 
 Requirement for RAD-tools installation are:
 
 * Python itself (>=3.6)
```

### Comparing `rad-tools-0.6.1/README.rst` & `rad-tools-0.6.2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 *********
 Various scripts for condense matter calculations and post-processing.
 
 .. image:: https://badge.fury.io/py/rad-tools.svg
     :target: https://badge.fury.io/py/rad-tools
     
 .. image:: https://readthedocs.org/projects/rad-tools/badge/?version=stable
-    :target: https://rad-tools.adrybakov.com/en/stable/?badge=stable
+    :target: https://rad-tools.org/en/stable/?badge=stable
     :alt: Documentation Status
    
 .. image:: https://static.pepy.tech/personalized-badge/rad-tools?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads
  :target: https://pepy.tech/project/rad-tools
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
@@ -27,15 +27,15 @@
 It is expected to be used in two ways:
 
 * As Python library
 
 * Via scripts (i.e. usage from command line)
 
 For the detailed descriprion check
-`documentation. <https://rad-tools.adrybakov.com>`_
+`documentation. <https://rad-tools.org>`_
 
 Installation
 ============
 
 Requirement for RAD-tools installation are:
 
 * Python itself (>=3.6)
```

### Comparing `rad-tools-0.6.1/rad_tools/__init__.py` & `rad-tools-0.6.2/rad_tools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 r"""
 All tools from the package.
 
 
 |version|
 """
 
-__version__ = "0.6.1"
+__version__ = "0.6.2"
 
 
 from . import dos, exchange, io, kpoints, score
 from .dos import *
 from .exchange import *
 from .io import *
 from .kpoints import *
```

### Comparing `rad-tools-0.6.1/rad_tools/dos/dos.py` & `rad-tools-0.6.2/rad_tools/dos/dos.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.6.1/rad_tools/dos/pdos.py` & `rad-tools-0.6.2/rad_tools/dos/pdos.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.6.1/rad_tools/exchange/bond.py` & `rad-tools-0.6.2/rad_tools/exchange/bond.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.6.1/rad_tools/exchange/model.py` & `rad-tools-0.6.2/rad_tools/exchange/model.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.6.1/rad_tools/exchange/template.py` & `rad-tools-0.6.2/rad_tools/exchange/template.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.6.1/rad_tools/io/__init__.py` & `rad-tools-0.6.2/rad_tools/io/__init__.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.6.1/rad_tools/io/internal.py` & `rad-tools-0.6.2/rad_tools/io/internal.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.6.1/rad_tools/io/tb2j.py` & `rad-tools-0.6.2/rad_tools/io/tb2j.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.6.1/rad_tools/kpoints/__init__.py` & `rad-tools-0.6.2/rad_tools/kpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.6.1/rad_tools/kpoints/high_symmetry_point.py` & `rad-tools-0.6.2/rad_tools/kpoints/high_symmetry_point.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.6.1/rad_tools/kpoints/kpoints.py` & `rad-tools-0.6.2/rad_tools/kpoints/kpoints.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.6.1/rad_tools/map.py` & `rad-tools-0.6.2/rad_tools/map.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.6.1/rad_tools/routines.py` & `rad-tools-0.6.2/rad_tools/routines.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.6.1/rad_tools/score/__init__.py` & `rad-tools-0.6.2/rad_tools/score/__init__.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.6.1/rad_tools/score/extract_tb2j.py` & `rad-tools-0.6.2/rad_tools/score/extract_tb2j.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.6.1/rad_tools/score/identify_wannier_centres.py` & `rad-tools-0.6.2/rad_tools/score/identify_wannier_centres.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.6.1/rad_tools/score/make_template.py` & `rad-tools-0.6.2/rad_tools/score/make_template.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.6.1/rad_tools/score/plot_dos.py` & `rad-tools-0.6.2/rad_tools/score/plot_dos.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.6.1/rad_tools/score/plot_tb2j.py` & `rad-tools-0.6.2/rad_tools/score/plot_tb2j.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.6.1/rad_tools.egg-info/PKG-INFO` & `rad-tools-0.6.2/rad_tools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: rad-tools
-Version: 0.6.1
+Version: 0.6.2
 Summary: Scripts for condense matter calculations and post-processing.
-Home-page: https://rad-tools.adrybakov.com/en/stable/
+Home-page: https://rad-tools.org/en/stable/
 Download-URL: https://github.com/adrybakov/rad-tools.git
 Author: Andrey Rybakov
 Author-email: rybakov.ad@icloud.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -22,15 +22,15 @@
 *********
 Various scripts for condense matter calculations and post-processing.
 
 .. image:: https://badge.fury.io/py/rad-tools.svg
     :target: https://badge.fury.io/py/rad-tools
     
 .. image:: https://readthedocs.org/projects/rad-tools/badge/?version=stable
-    :target: https://rad-tools.adrybakov.com/en/stable/?badge=stable
+    :target: https://rad-tools.org/en/stable/?badge=stable
     :alt: Documentation Status
    
 .. image:: https://static.pepy.tech/personalized-badge/rad-tools?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads
  :target: https://pepy.tech/project/rad-tools
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
@@ -46,15 +46,15 @@
 It is expected to be used in two ways:
 
 * As Python library
 
 * Via scripts (i.e. usage from command line)
 
 For the detailed descriprion check
-`documentation. <https://rad-tools.adrybakov.com>`_
+`documentation. <https://rad-tools.org>`_
 
 Installation
 ============
 
 Requirement for RAD-tools installation are:
 
 * Python itself (>=3.6)
```

### Comparing `rad-tools-0.6.1/rad_tools.egg-info/SOURCES.txt` & `rad-tools-0.6.2/rad_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rad-tools-0.6.1/scripts/compute-energies.py` & `rad-tools-0.6.2/scripts/compute-energies.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.6.1/scripts/phonopy-plotter.py` & `rad-tools-0.6.2/scripts/phonopy-plotter.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.6.1/setup.py` & `rad-tools-0.6.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     name="rad-tools",
     version=__version__,
     description="Scripts for condense matter calculations and post-processing.",
     long_description=long_description,
     author="Andrey Rybakov",
     author_email="rybakov.ad@icloud.com",
     license="MIT license",
-    url="https://rad-tools.adrybakov.com/en/stable/",
+    url="https://rad-tools.org/en/stable/",
     download_url="https://github.com/adrybakov/rad-tools.git",
     packages=find_packages(),
     scripts=[
         "scripts/rad-plot-tb2j.py",
         "scripts/phonopy-plotter.py",
         "scripts/rad-extract-tb2j.py",
         "scripts/rad-make-template.py",
```

