# Comparing `tmp/pyseistr-0.0.4.3.1.tar.gz` & `tmp/pyseistr-0.0.4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyseistr-0.0.4.3.1.tar", last modified: Wed Apr 26 02:58:08 2023, max compression
+gzip compressed data, was "pyseistr-0.0.4.4.0.tar", last modified: Tue Jun  6 03:10:25 2023, max compression
```

## Comparing `pyseistr-0.0.4.3.1.tar` & `pyseistr-0.0.4.4.0.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-04-26 02:58:08.825459 pyseistr-0.0.4.3.1/
--rw-r--r--   0 chenyk     (501) staff       (20)    35149 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/LICENSE
--rw-r--r--   0 chenyk     (501) staff       (20)     1167 2023-04-26 02:58:08.825071 pyseistr-0.0.4.3.1/PKG-INFO
--rw-r--r--   0 chenyk     (501) staff       (20)     6520 2023-04-23 23:19:43.000000 pyseistr-0.0.4.3.1/README.md
-drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-04-26 02:58:08.812730 pyseistr-0.0.4.3.1/pyseistr/
--rw-r--r--   0 chenyk     (501) staff       (20)     1893 2023-04-22 20:38:05.000000 pyseistr-0.0.4.3.1/pyseistr/__init__.py
--rw-r--r--   0 chenyk     (501) staff       (20)     5563 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/bp.py
--rw-r--r--   0 chenyk     (501) staff       (20)     4852 2023-04-26 02:53:38.000000 pyseistr-0.0.4.3.1/pyseistr/dip2d.py
--rw-r--r--   0 chenyk     (501) staff       (20)     6636 2023-04-26 02:54:03.000000 pyseistr-0.0.4.3.1/pyseistr/dip3d.py
--rw-r--r--   0 chenyk     (501) staff       (20)     7494 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/divne.py
--rw-r--r--   0 chenyk     (501) staff       (20)     1044 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/fk.py
--rw-r--r--   0 chenyk     (501) staff       (20)     4464 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/mf.py
--rw-r--r--   0 chenyk     (501) staff       (20)     4557 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/operators.py
--rw-r--r--   0 chenyk     (501) staff       (20)      696 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/plot.py
--rw-r--r--   0 chenyk     (501) staff       (20)     6801 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/pwspray2d.py
--rw-r--r--   0 chenyk     (501) staff       (20)     9410 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/pwspray3d.py
--rw-r--r--   0 chenyk     (501) staff       (20)      657 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/ricker.py
--rw-r--r--   0 chenyk     (501) staff       (20)     1990 2023-04-23 18:14:53.000000 pyseistr-0.0.4.3.1/pyseistr/soint2d.py
--rw-r--r--   0 chenyk     (501) staff       (20)     2300 2023-04-22 20:42:00.000000 pyseistr-0.0.4.3.1/pyseistr/soint3d.py
--rw-r--r--   0 chenyk     (501) staff       (20)     7771 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/solvers.py
--rw-r--r--   0 chenyk     (501) staff       (20)     1263 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/somean2d.py
--rw-r--r--   0 chenyk     (501) staff       (20)     1496 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/somean3d.py
--rw-r--r--   0 chenyk     (501) staff       (20)     2823 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/somf2d.py
--rw-r--r--   0 chenyk     (501) staff       (20)     2932 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/somf3d.py
-drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-04-26 02:58:08.823427 pyseistr-0.0.4.3.1/pyseistr/src/
--rw-r--r--   0 chenyk     (501) staff       (20)    14513 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/src/bp_cfuns.c
--rw-r--r--   0 chenyk     (501) staff       (20)    42528 2023-04-23 21:14:48.000000 pyseistr-0.0.4.3.1/pyseistr/src/dip_cfuns.c
--rw-r--r--   0 chenyk     (501) staff       (20)    35389 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/src/sof3d_cfuns.c
--rw-r--r--   0 chenyk     (501) staff       (20)    34464 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/src/sof_cfuns.c
--rw-r--r--   0 chenyk     (501) staff       (20)    49126 2023-04-23 18:43:05.000000 pyseistr-0.0.4.3.1/pyseistr/src/soint2d_cfuns.c
--rw-r--r--   0 chenyk     (501) staff       (20)    31152 2023-04-22 19:39:19.000000 pyseistr-0.0.4.3.1/pyseistr/src/soint3d_cfuns.c
-drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-04-26 02:58:08.816476 pyseistr-0.0.4.3.1/pyseistr.egg-info/
--rw-r--r--   0 chenyk     (501) staff       (20)     1167 2023-04-26 02:58:08.000000 pyseistr-0.0.4.3.1/pyseistr.egg-info/PKG-INFO
--rw-r--r--   0 chenyk     (501) staff       (20)      737 2023-04-26 02:58:08.000000 pyseistr-0.0.4.3.1/pyseistr.egg-info/SOURCES.txt
--rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-04-26 02:58:08.000000 pyseistr-0.0.4.3.1/pyseistr.egg-info/dependency_links.txt
--rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-04-22 19:39:47.000000 pyseistr-0.0.4.3.1/pyseistr.egg-info/not-zip-safe
--rw-r--r--   0 chenyk     (501) staff       (20)       53 2023-04-26 02:58:08.000000 pyseistr-0.0.4.3.1/pyseistr.egg-info/requires.txt
--rw-r--r--   0 chenyk     (501) staff       (20)       66 2023-04-26 02:58:08.000000 pyseistr-0.0.4.3.1/pyseistr.egg-info/top_level.txt
--rw-r--r--   0 chenyk     (501) staff       (20)       38 2023-04-26 02:58:08.825597 pyseistr-0.0.4.3.1/setup.cfg
--rw-r--r--   0 chenyk     (501) staff       (20)     2668 2023-04-26 02:57:52.000000 pyseistr-0.0.4.3.1/setup.py
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-06-06 03:10:25.860363 pyseistr-0.0.4.4.0/
+-rw-r--r--   0 chenyk     (501) staff       (20)    35149 2022-10-30 03:00:33.000000 pyseistr-0.0.4.4.0/LICENSE
+-rw-r--r--   0 chenyk     (501) staff       (20)     1167 2023-06-06 03:10:25.859846 pyseistr-0.0.4.4.0/PKG-INFO
+-rw-r--r--   0 chenyk     (501) staff       (20)     6526 2023-06-06 03:09:12.000000 pyseistr-0.0.4.4.0/README.md
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-06-06 03:10:25.841239 pyseistr-0.0.4.4.0/pyseistr/
+-rw-r--r--   0 chenyk     (501) staff       (20)     1963 2023-04-26 17:23:07.000000 pyseistr-0.0.4.4.0/pyseistr/__init__.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     6443 2023-04-26 17:54:27.000000 pyseistr-0.0.4.4.0/pyseistr/bp.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     3370 2023-04-26 19:17:10.000000 pyseistr-0.0.4.4.0/pyseistr/das.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     4852 2023-04-26 02:53:38.000000 pyseistr-0.0.4.4.0/pyseistr/dip2d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     6636 2023-04-26 02:54:03.000000 pyseistr-0.0.4.4.0/pyseistr/dip3d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     7458 2023-04-26 18:24:49.000000 pyseistr-0.0.4.4.0/pyseistr/divne.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     1949 2023-04-26 18:00:54.000000 pyseistr-0.0.4.4.0/pyseistr/fk.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     4355 2023-04-26 18:21:58.000000 pyseistr-0.0.4.4.0/pyseistr/mf.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     4515 2023-04-26 18:20:04.000000 pyseistr-0.0.4.4.0/pyseistr/operators.py
+-rw-r--r--   0 chenyk     (501) staff       (20)      696 2022-10-30 03:00:33.000000 pyseistr-0.0.4.4.0/pyseistr/plot.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     6682 2023-04-26 18:18:58.000000 pyseistr-0.0.4.4.0/pyseistr/pwspray2d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     9161 2023-04-26 18:16:38.000000 pyseistr-0.0.4.4.0/pyseistr/pwspray3d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)      756 2023-04-26 18:01:43.000000 pyseistr-0.0.4.4.0/pyseistr/ricker.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     1946 2023-04-26 18:13:12.000000 pyseistr-0.0.4.4.0/pyseistr/soint2d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     2296 2023-04-26 18:12:30.000000 pyseistr-0.0.4.4.0/pyseistr/soint3d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     7702 2023-04-26 18:11:26.000000 pyseistr-0.0.4.4.0/pyseistr/solvers.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     1257 2023-04-26 18:04:24.000000 pyseistr-0.0.4.4.0/pyseistr/somean2d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     1310 2023-04-26 18:10:01.000000 pyseistr-0.0.4.4.0/pyseistr/somean3d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     2773 2023-04-26 18:09:39.000000 pyseistr-0.0.4.4.0/pyseistr/somf2d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     2877 2023-04-26 18:08:32.000000 pyseistr-0.0.4.4.0/pyseistr/somf3d.py
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-06-06 03:10:25.857978 pyseistr-0.0.4.4.0/pyseistr/src/
+-rw-r--r--   0 chenyk     (501) staff       (20)    14538 2023-04-26 17:07:57.000000 pyseistr-0.0.4.4.0/pyseistr/src/bp_cfuns.c
+-rw-r--r--   0 chenyk     (501) staff       (20)    13013 2023-04-26 19:16:45.000000 pyseistr-0.0.4.4.0/pyseistr/src/coh_cfuns.c
+-rw-r--r--   0 chenyk     (501) staff       (20)    42570 2023-04-26 17:15:11.000000 pyseistr-0.0.4.4.0/pyseistr/src/dip_cfuns.c
+-rw-r--r--   0 chenyk     (501) staff       (20)    35389 2022-10-30 03:00:33.000000 pyseistr-0.0.4.4.0/pyseistr/src/sof3d_cfuns.c
+-rw-r--r--   0 chenyk     (501) staff       (20)    34515 2023-04-26 17:27:47.000000 pyseistr-0.0.4.4.0/pyseistr/src/sof_cfuns.c
+-rw-r--r--   0 chenyk     (501) staff       (20)    49126 2023-04-23 18:43:05.000000 pyseistr-0.0.4.4.0/pyseistr/src/soint2d_cfuns.c
+-rw-r--r--   0 chenyk     (501) staff       (20)    31152 2023-04-22 19:39:19.000000 pyseistr-0.0.4.4.0/pyseistr/src/soint3d_cfuns.c
+-rw-r--r--   0 chenyk     (501) staff       (20)     1339 2023-04-26 18:02:10.000000 pyseistr-0.0.4.4.0/pyseistr/synthetics.py
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-06-06 03:10:25.845661 pyseistr-0.0.4.4.0/pyseistr.egg-info/
+-rw-r--r--   0 chenyk     (501) staff       (20)     1167 2023-06-06 03:10:25.000000 pyseistr-0.0.4.4.0/pyseistr.egg-info/PKG-INFO
+-rw-r--r--   0 chenyk     (501) staff       (20)      801 2023-06-06 03:10:25.000000 pyseistr-0.0.4.4.0/pyseistr.egg-info/SOURCES.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-06-06 03:10:25.000000 pyseistr-0.0.4.4.0/pyseistr.egg-info/dependency_links.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-04-22 19:39:47.000000 pyseistr-0.0.4.4.0/pyseistr.egg-info/not-zip-safe
+-rw-r--r--   0 chenyk     (501) staff       (20)       53 2023-06-06 03:10:25.000000 pyseistr-0.0.4.4.0/pyseistr.egg-info/requires.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)       74 2023-06-06 03:10:25.000000 pyseistr-0.0.4.4.0/pyseistr.egg-info/top_level.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)       38 2023-06-06 03:10:25.860500 pyseistr-0.0.4.4.0/setup.cfg
+-rw-r--r--   0 chenyk     (501) staff       (20)     2799 2023-06-06 03:10:08.000000 pyseistr-0.0.4.4.0/setup.py
```

### Comparing `pyseistr-0.0.4.3.1/LICENSE` & `pyseistr-0.0.4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3.1/PKG-INFO` & `pyseistr-0.0.4.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyseistr
-Version: 0.0.4.3.1
+Version: 0.0.4.4.0
 Summary: A python package for structural denoising and interpolation of multi-channel seismic data
 Home-page: https://github.com/aaspip/pyseistr
 Author: pyseistr developing team
 Author-email: chenyk2016@gmail.com
 License: GNU General Public License, Version 3 (GPLv3)
 Keywords: seismology,earthquake seismology,exploration seismology,array seismology,denoising,science,engineering,structure,local slope,filtering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyseistr-0.0.4.3.1/README.md` & `pyseistr-0.0.4.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 ======
 
 ## Description
 
 **Pyseistr** is a python package for structural denoising and interpolation of multi-channel seismic data. The latest version has incorporated both Python and C (hundreds of times faster) implementations of the embedded functions. We keep both implementations for both educational and production purposes. This package has a variety of applications in both exploration and earthquake seismology.
 
 ## Reference
-Chen et al., 2023, Pyseistr: a python package for structural denoising and interpolation of multi-channel seismic data, Seismological Research Letters, 94(1), 457-472. 
+Chen et al., 2023, Pyseistr: a python package for structural denoising and interpolation of multi-channel seismic data, Seismological Research Letters, 94(3), 1703-1714. 
 
 BibTeX:
 
 	@article{pyseistr,
 	  title={Pyseistr: a python package for structural denoising and interpolation of multi-channel seismic data},
 	  author={Yangkang Chen and Alexandros Savvaidis and Sergey Fomel and Yunfeng Chen and Omar M. Saad and Yapo Abol{\'e} Serge Innocent Obou{\'e} and Quan Zhang and Wei Chen},
 	  journal={Seismological Research Letters},
 	  volume={94},
-	  number={1},
-	  pages={457-472},
+	  number={3},
+	  pages={1703–1714},
 	  year={2023}
 	}
 
 -----------
 ## Copyright
     The pyseistr developing team, 2021-present
 -----------
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyseistr-0.0.4.3.1/pyseistr/__init__.py` & `pyseistr-0.0.4.4.0/pyseistr/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 :copyright:
-    Yangkang Chen (chenyk2016@gmail.com), 2021-2022   
+    Yangkang Chen (chenyk2016@gmail.com), 2021-2023   
 :license:
     GNU General Public License, Version 3
     (http://www.gnu.org/copyleft/gpl.html)
 """
 from __future__ import (absolute_import, division, print_function,
                         unicode_literals)
 
@@ -53,15 +53,18 @@
 from .soint2d import soint2d #structure-oriented interpolation for 2D data
 from .soint3d import soint3d #structure-oriented interpolation for 3D data
 from .ricker import ricker
 from .bp import bandpass
 from .fk import fkdip
 from .plot import cseis
 
+from .das import coh 
+from .das import cohc
 
+from .synthetics import *
 
 ## C versions
 from .dip2d import dip2dc
 from .dip3d import dip3dc
 from .somean2d import somean2dc
 from .somean3d import somean3dc
 from .somf2d import somf2dc
```

### Comparing `pyseistr-0.0.4.3.1/pyseistr/bp.py` & `pyseistr-0.0.4.4.0/pyseistr/bp.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,54 @@
 import numpy as np
 from bpcfun import *
 
 def bandpass(din,dt,flo=0,fhi=0.5,nplo=6,nphi=6,phase=0,verb=1):
-	# bandpass: Bandpass filtering.
-	#
-	# Aug, 05, 2020
-	# by Yangkang Chen
-	#
-	# INPUT
-	# din:	  input data
-	# dt:       sampling
-	# flo:      Low frequency in band, default is 0
-	# fhi:      High frequency in band, default is Nyquist
-	# nplo=6:   number of poles for low cutoff
-	# nphi=6:   number of poles for high cutoff
-	# phase=0:  y: minimum phase, n: zero phase
-	# verb=0:   verbosity flag
-	#
-	# OUTPUT
-	# dout:     output data
-	#
-	# RFERENCE
-	# November 2012 program of the month: http://ahay.org/blog/2012/11/03/program-of-the-month-sfbandpass/
-	#
-	# Example
-	# demos/test_xxx_das.py
-	#
+	'''
+	bandpass: Bandpass filtering.
 	
+	Aug, 05, 2020
+	by Yangkang Chen
+	
+	INPUT
+	din:	  input data
+	dt:       sampling
+	flo:      Low frequency in band, default is 0
+	fhi:      High frequency in band, default is Nyquist
+	nplo=6:   number of poles for low cutoff
+	nphi=6:   number of poles for high cutoff
+	phase=0:  y: minimum phase, n: zero phase
+	verb=0:   verbosity flag
+	
+	OUTPUT
+	dout:     output data
+	
+	RFERENCE
+	November 2012 program of the month: http://ahay.org/blog/2012/11/03/program-of-the-month-sfbandpass/
+	
+	EXAMPLE 1
+	demos/test_pyseistr_das.py
+	
+	EXAMPLE 2
+	from pyseistr import ricker;
+	wav,tw=ricker(20,0.004,2);
+	from pyseistr import bandpass;
+	wav2=bandpass(wav,0.004,flo=0,fhi=20);
+	
+	import matplotlib.pyplot as plt;
+	plt.subplot(2,1,1);
+	plt.plot(tw,wav);plt.ylabel('Amplitude');plt.gca().set_ylim([-0.5,1]);
+	plt.subplot(2,1,2);
+	plt.plot(tw,wav2);plt.xlabel('Time (s)');plt.ylabel('Amplitude');plt.gca().set_ylim([-0.5,1]);
+	plt.show();
+
+	
+	'''
+	if din.ndim==1:	#for 1D problems
+		din=np.expand_dims(din, axis=1)
+		
 	if din.ndim==2:	#for 2D problems
 		din=np.expand_dims(din, axis=2)
 		
 	if din.shape[0]==1 and din.shape[1]>1 and din.shape[2]==1: #row vector
 		din=din.flatten();
 	
 	[n1,n22,n33]=din.shape;
@@ -68,17 +86,16 @@
 		nphi=1;
 
 	if nphi>1 and not phase:
 		nphi=nphi/2;
 
 
 	if verb:
-		print("flo=%g fhi=%g nplo=%d nphi=%d\n",flo,fhi,nplo,nphi);
+		print("flo=%g fhi=%g nplo=%d nphi=%d\n"%(flo,fhi,nplo,nphi));
 	
-
 	if flo>eps:
 		blo=butter_init(0,flo,nplo);
 	else:
 		blo='NULL';
 
 	if fhi<0.5-eps:
 		bhi=butter_init(1,fhi,nphi);
@@ -105,69 +122,89 @@
 
 	dout=dout.reshape(n1,n22,n33);
 
 	dout=np.squeeze(dout);
 	return dout
 
 def bandpassc(din,dt,flo=0,fhi=0.5,nplo=6,nphi=6,phase=0,verb=1):
-	# bandpass: Bandpass filtering.
-	#
-	# Aug, 05, 2020
-	# by Yangkang Chen
-	#
-	# INPUT
-	# din:	  input data
-	# dt:       sampling
-	# flo:      Low frequency in band, default is 0
-	# fhi:      High frequency in band, default is Nyquist
-	# nplo=6:   number of poles for low cutoff
-	# nphi=6:   number of poles for high cutoff
-	# phase=0:  y: minimum phase, n: zero phase
-	# verb=0:   verbosity flag
-	#
-	# OUTPUT
-	# dout:     output data
-	#
-	# RFERENCE
-	# November 2012 program of the month: http://ahay.org/blog/2012/11/03/program-of-the-month-sfbandpass/
-	#
-	# Example
-	# demos/test_xxx_das.py
-	#
+	'''
+	bandpass: Bandpass filtering.
+	
+	Aug, 05, 2020
+	by Yangkang Chen
+	
+	INPUT
+	din:	  input data
+	dt:       sampling
+	flo:      Low frequency in band, default is 0
+	fhi:      High frequency in band, default is Nyquist
+	nplo=6:   number of poles for low cutoff
+	nphi=6:   number of poles for high cutoff
+	phase=0:  y: minimum phase, n: zero phase
+	verb=0:   verbosity flag
+	
+	OUTPUT
+	dout:     output data
+	
+	RFERENCE
+	November 2012 program of the month: http://ahay.org/blog/2012/11/03/program-of-the-month-sfbandpass/
+	
+	EXAMPLE 1
+	demos/test_pyseistr_das.py
+	
+	EXAMPLE 2
+	from pyseistr import ricker;
+	wav,tw=ricker(20,0.004,2);
+	from pyseistr import bandpassc;
+	wav2=bandpassc(wav,0.004,flo=0,fhi=20);
 	
+	import matplotlib.pyplot as plt;
+	figsize=(8, 8)
+	plt.subplot(2,1,1);
+	plt.plot(tw,wav);plt.ylabel('Amplitude');plt.gca().set_ylim([-0.5,1]);
+	plt.subplot(2,1,2);
+	plt.plot(tw,wav2);plt.xlabel('Time (s)');plt.ylabel('Amplitude');plt.gca().set_ylim([-0.5,1]);
+	plt.show();
+	
+	'''
+	if din.ndim==1:	#for 1D problems
+		din=np.expand_dims(din, axis=1)
+		
 	if din.ndim==2:	#for 2D problems
 		din=np.expand_dims(din, axis=2)
 		
 	if din.shape[0]==1 and din.shape[1]>1 and din.shape[2]==1: #row vector
 		din=din.flatten();
-	
-	[n1,n2,n3]=din.shape;
 
+	[n1,n2,n3]=din.shape;
+		
 	din=np.float32(din).flatten(order='F');
 	dout=cbp(din,n1,n2,n3,dt,flo,fhi,nplo,nphi,phase,verb);
 	dout=dout.reshape(n1,n2,n3,order='F');
 
 	if n3==1:
 		dout=np.squeeze(dout);
 	return dout
 	
 def butter_init(low,cutoff,nn):
-	# butter_init: initialize
-	# Aug, 5, 2020
-	# Yangkang Chen
-	# 
-	# INPUT
-	# low:	  low-pass (or high-pass)
-	# cutoff:   cut off frequency
-	# nn:	   number of poles
-	# 
-	# OUTPUT
-	# bw:	   butterworth struct
-	# 
-# 	bw=struct;
+	'''
+	butter_init: initialize
+	Aug, 5, 2020
+	Yangkang Chen
+	
+	INPUT
+	low:	  low-pass (or high-pass)
+	cutoff:   cut off frequency
+	nn:	   number of poles
+	
+	OUTPUT
+	bw:	   butterworth struct
+	
+	'''
+
 	arg=2*np.pi*cutoff;
 	sinw=np.sin(arg);
 	cosw=np.cos(arg);
 
 	bw={'nn':nn,'low':low,'den':np.zeros([2,int(np.floor((nn+1)/2))])};
 	
 	if np.mod(nn,2)>0:
@@ -190,29 +227,31 @@
 		bw['den'][1,j]=(1-ss)/fact;
 
 	bw['mid']=-2.*cosw/fact;
 	return bw
 
 
 def butter_apply(bw,nx,x):
-	# butter_apply: filter the data (in place)
-	# 
-	#Implementation is inspired by D. Hale and J.F. Claerbout, 1983, Butterworth
-	#dip filters: Geophysics, 48, 1033-1038.
-	#
-	# Aug, 5, 2020
-	# Yangkang Chen
-	# 
-	# INPUT
-	# bw: butterworth struct
-	# nx: size of x
-	# x: input data
-	# 
-	# OUTPUT
-	# x: output data
+	'''
+	butter_apply: filter the data (in place)
+	
+	Implementation is inspired by D. Hale and J.F. Claerbout, 1983, Butterworth
+	dip filters: Geophysics, 48, 1033-1038.
+	
+	Aug, 5, 2020
+	Yangkang Chen
+	
+	INPUT
+	bw: butterworth struct
+	nx: size of x
+	x: input data
+	
+	OUTPUT
+	x: output data
+	'''
 	d1=bw['mid'];
 	nn=bw['nn'];
 	if np.mod(nn,2)>0:
 		d0=bw['den'][0,int(np.floor(nn/2))];
 		d2=bw['den'][1,int(np.floor(nn/2))];
 		x0=0;
 		y1=0;
@@ -228,26 +267,29 @@
 		for ix in range(0,nx):
 			x2=x1;x1=x0;x0=x[ix].copy();#This bug is striking, .copy is necessary because otherwise x0 will automatically change according to y0.
 			y0=ifnot(bw['low'],(x0 + 2*x1 + x2 - d1 * y1 - d2 * y2)*d0,(x0 - 2*x1 + x2 - d1 * y1 - d2 * y2)*d0);
 			y2=y1;x[ix]=y0;y1=y0;
 	return x
 
 def reverse(n1,trace):
-	# reverse a trace (in place)
+	'''
+	reverse a trace (in place)
+	'''
 	for i1 in range(0,int(np.floor(n1/2))):
 		t=trace[i1].copy();#This bug is striking, .copy is necessary because otherwise x0 will automatically change according to y0.
 		trace[i1]=trace[n1-i1-1];
 		trace[n1-i1-1]=t;
 	return trace
 
 
 def ifnot(yes, v1, v2):
-	# ifnot: equivalent to C grammar (v=yes?v1:v2)
-	# Yangkang Chen
-	# July, 22, 2020
-
+	'''
+	ifnot: equivalent to C grammar (v=yes?v1:v2)
+	Yangkang Chen
+	July, 22, 2020
+	'''
 	if yes:
 		v=v1;
 	else:
 		v=v2;
 
 	return v
```

### Comparing `pyseistr-0.0.4.3.1/pyseistr/dip2d.py` & `pyseistr-0.0.4.4.0/pyseistr/dip2d.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3.1/pyseistr/dip3d.py` & `pyseistr-0.0.4.4.0/pyseistr/dip3d.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3.1/pyseistr/divne.py` & `pyseistr-0.0.4.4.0/pyseistr/divne.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import numpy as np
 def divne(num, den, Niter, rect, ndat, eps_dv, eps_cg, tol_cg,verb):
-	#divne: N-dimensional smooth division rat=num/den		  
-	#This is a subroutine from the seistr package (https://github.com/chenyk1990/seistr)
-	#
-	#by Yangkang Chen, 2022, verified to be exactly the same as the Matlab version
-	#
-	#INPUT
-	#num: numerator
-	#den: denominator
-	#Niter: number of iterations
-	#rect: triangle radius [ndim], e.g., [5,5,1]
-	#ndat: data dimensions [ndim], e.g., [n1,n2,1]
-	#eps_dv: eps for divn  (default: 0.01)
-	#eps_cg: eps for CG	(default: 1)
-	#tol_cg: tolerence for CG (default: 0.000001)
-	#verb: verbosity flag
-	#
-	#OUTPUT
-	#rat: output ratio
-	# 
-	#Reference
-	#H. Wang, Y. Chen, O. Saad, W. Chen, Y. Oboue, L. Yang, S. Fomel, and Y. Chen, 2022, A Matlab code package for 2D/3D local slope estimation and structural filtering. Geophysics, 87(3), F1–F14, doi: 10.1190/geo2021-0266.1. 
+	'''
+	divne: N-dimensional smooth division rat=num/den		  
+	This is a subroutine from the seistr package (https://github.com/chenyk1990/seistr)
+	
+	by Yangkang Chen, 2022, verified to be exactly the same as the Matlab version
+	
+	INPUT
+	num: numerator
+	den: denominator
+	Niter: number of iterations
+	rect: triangle radius [ndim], e.g., [5,5,1]
+	ndat: data dimensions [ndim], e.g., [n1,n2,1]
+	eps_dv: eps for divn  (default: 0.01)
+	eps_cg: eps for CG	(default: 1)
+	tol_cg: tolerence for CG (default: 0.000001)
+	verb: verbosity flag
+	
+	OUTPUT
+	rat: output ratio
+	 
+	REFERENCE
+	H. Wang, Y. Chen, O. Saad, W. Chen, Y. Oboue, L. Yang, S. Fomel, and Y. Chen, 2022, A Matlab code package for 2D/3D local slope estimation and structural filtering. Geophysics, 87(3), F1–F14, doi: 10.1190/geo2021-0266.1. 
+	'''
 	n=num.size
 	
 	ifhasp0=0
 	p=np.zeros(n)
 	
 	num=num.reshape(n,order='F')
 	den=den.reshape(n,order='F')
@@ -49,26 +51,28 @@
 	rat = conjgrad(None, weight_lop, trianglen_lop, p, None, num, eps_cg, tol_cg, Niter,ifhasp0,[],par_L,par_S,verb);
 	rat=rat.reshape(ndat[0],ndat[1],ndat[2],order='F')
 
 	return rat
 
 
 def weight_lop(din,par,adj,add):
-	# weight_lop: Weighting operator (verified)
-	# 
-	# Ported to Python by Yangkang Chen, 2022
-	# 
-	# INPUT
-	# din: model/data
-	# par: parameter
-	# adj: adj flag
-	# add: add flag
-	# OUTPUT
-	# dout: data/model
-	# 
+	'''
+	weight_lop: Weighting operator (verified)
+	
+	Ported to Python by Yangkang Chen, 2022
+	
+	INPUT
+	din: model/data
+	par: parameter
+	adj: adj flag
+	add: add flag
+	
+	OUTPUT
+	dout: data/model
+	'''
 	nm=par['nm'];
 	nd=par['nd'];
 	w=par['w'];
 
 	if adj==1:
 		d=din;
 		if 'm' in par and add==1:
@@ -92,25 +96,28 @@
 		dout=m;
 	else:
 		dout=d;
 
 	return dout
 	
 def trianglen_lop(din,par,adj,add ):
-	# trianglen_lop: N-D triangle smoothing operator (verified)
-	# 
-	# Ported to Python by Yangkang Chen, 2022
-	# 
-	# INPUT
-	# din: model/data
-	# par: parameter
-	# adj: adj flag
-	# add: add flag
-	# OUTPUT
-	# dout: data/model
+	'''
+	trianglen_lop: N-D triangle smoothing operator (verified)
+	
+	Ported to Python by Yangkang Chen, 2022
+	
+	INPUT
+	din: model/data
+	par: parameter
+	adj: adj flag
+	add: add flag
+	
+	OUTPUT
+	dout: data/model
+	'''
 	if adj==1:
 		d=din;
 		if 'm' in par and add==1:
 			m=par['m'];
 		else:
 			m=np.zeros(par['nm']);
 	else:
@@ -162,78 +169,87 @@
 	else:
 		dout=d;
 
 	return dout
 
 
 def first_index( i, j, dim, n, s ):
-	#first_index: Find first index for multidimensional transforms
-	#Ported to Python by Yangkang Chen, 2022
-	#
-	#INPUT
-	#i:	dimension [0...dim-1]
-	#j:	line coordinate
-	#dim:  number of dimensions
-	#n:	box size [dim], vector
-	#s:	step [dim], vector
-	#OUTPUT
-	#i0:   first index
+	'''
+	first_index: Find first index for multidimensional transforms
+	Ported to Python by Yangkang Chen, 2022
+	
+	INPUT
+	i:	dimension [0...dim-1]
+	j:	line coordinate
+	dim:  number of dimensions
+	n:	box size [dim], vector
+	s:	step [dim], vector
+	
+	OUTPUT
+	i0:   first index
+	'''
 
 	n123 = 1;
 	i0 = 0;
 	for k in range(0,dim):
 		if (k == i):
 			continue;
 		ii = np.floor(np.mod((j/n123), n[k]));
 		n123 = n123 * n[k];
 		i0 = i0 + ii * s[k];
 
 	return int(i0)
 
 
 def smooth2( tr, o, d, der, x):
-	#smooth2: apply triangle smoothing
-	#
-	#Ported to Python by Yangkang Chen, 2022
-	#
-	#INPUT
-	#tr:   smoothing object
-	#o:	trace sampling
-	#d:	trace sampling
-	#x:	data (smoothed in place)
-	#der:  if derivative
-	#OUTPUT
-	#x: smoothed result
-	#tr: triangle struct
+	'''
+	smooth2: apply triangle smoothing
+	
+	Ported to Python by Yangkang Chen, 2022
+	
+	INPUT
+	tr:   smoothing object
+	o:	trace sampling
+	d:	trace sampling
+	x:	data (smoothed in place)
+	der:  if derivative
+	
+	OUTPUT
+	x: smoothed result
+	tr: triangle struct
+	'''
 
 	tr['tmp'] = triple2(o, d, tr['nx'], tr['nb'], x, tr['tmp'], tr['box'], tr['wt']);
 	tr['tmp'] = doubint2(tr['np'], tr['tmp'], (tr['box'] or der));
 	x = fold2(o, d, tr['nx'], tr['nb'], tr['np'], x, tr['tmp']);
 
 	return x,tr
 
 
 def triple2( o, d, nx, nb, x, tmp, box, wt ):
-	#BY Yangkang Chen, Nov, 04, 2019
-
+	'''
+	BY Yangkang Chen, Nov, 04, 2019
+	'''
 	for i in range(0,nx+2*nb):
 		tmp[i] = 0;
 
 	if box:
 		tmp[1:]	 = cblas_saxpy(nx,  +wt,x[o:],d,tmp[1:],   1); 	#y += a*x
 		tmp[2*nb:]  = cblas_saxpy(nx,  -wt,x[o:],d,tmp[2*nb:],1);
 	else:
 		tmp		 = cblas_saxpy(nx,  -wt,x[o:],d,tmp,	   1); 	#y += a*x
 		tmp[nb:]	= cblas_saxpy(nx,2.*wt,x[o:],d,tmp[nb:],  1);
 		tmp[2*nb:]  = cblas_saxpy(nx,  -wt,x[o:],d,tmp[2*nb:],1);
 
 	return tmp
 
 def doubint2( nx, xx, der ):
-	#Modified by Yangkang Chen, Nov, 04, 2019
+	'''
+	Modified by Yangkang Chen, Nov, 04, 2019
+	'''
 	#integrate forward
 	t = 0.0;
 	for i in range(0,nx):
 		t = t + xx[i];
 		xx[i] = t;
 
 	if der:
@@ -246,27 +262,29 @@
 		xx[i] = t
 
 	return xx
 
 
 
 def cblas_saxpy( n, a, x, sx, y, sy ):
-	#y += a*x
-	#Modified by Yangkang Chen, Nov, 04, 2019
-
+	'''
+	y += a*x
+	Modified by Yangkang Chen, Nov, 04, 2019
+	'''
 	for i in range(0,n):
 		ix = i * sx;
 		iy = i * sy;
 		y[iy] = y[iy] + a * x[ix];
 
 	return y
 
 def fold2(o, d, nx, nb, np, x, tmp):
-	#Modified by Yangkang Chen, Nov, 04, 2019
-
+	'''
+	Modified by Yangkang Chen, Nov, 04, 2019
+	'''
 	#copy middle
 	for i in range(0,nx):
 		x[o+i*d] = tmp[i+nb];
 
 	#reflections from the right side
 	for j in range(nb+nx,np+1,nx):
 		if (nx <= np-j):
@@ -297,32 +315,34 @@
 				x[o+(nx-1-i)*d] = x[o+(nx-1-i)*d] + tmp[j-1-i];
 		else:
 			for i in range(0,j):
 				x[o+(nx-1-i)*d] = x[o+(nx-1-i)*d] + tmp[j-1-i];
 	return x
 
 def adjnull( adj,add,nm,nd,m,d ):
-	#Claerbout-style adjoint zeroing Zeros out the output (unless add is true). 
-	#Useful first step for and linear operator.
-	# 
-	#  This program is free software; you can redistribute it and/or modify
-	#  it under the terms of the GNU General Public License as published by
-	#  the Free Software Foundation; either version 2 of the License, or
-	#  (at your option) and later version.
-	#  
-	#  This program is distributed in the hope that it will be useful,
-	#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-	#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-	#  GNU General Public License for more details.
-	#  
-	#  You should have received a copy of the GNU General Public License
-	#  along with this program; if not, write to the Free Software
-	#  Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
-	#adj : adjoint flag; add: addition flag; nm: size of m; nd: size of d
-
+	'''
+	Claerbout-style adjoint zeroing Zeros out the output (unless add is true). 
+	Useful first step for and linear operator.
+	
+	This program is free software; you can redistribute it and/or modify
+	it under the terms of the GNU General Public License as published by
+	the Free Software Foundation; either version 2 of the License, or
+	(at your option) and later version.
+	
+	This program is distributed in the hope that it will be useful,
+	but WITHOUT ANY WARRANTY; without even the implied warranty of
+	MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+	GNU General Public License for more details.
+	
+	You should have received a copy of the GNU General Public License
+	along with this program; if not, write to the Free Software
+	Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
+	adj : adjoint flag; add: addition flag; nm: size of m; nd: size of d
+	'''
+	
 	if add:
 		return m,d
 
 	if adj:
 		m=np.zeros(nm);
 		for i in range(0,nm):
 			m[i] = 0.0;
```

### Comparing `pyseistr-0.0.4.3.1/pyseistr/mf.py` & `pyseistr-0.0.4.4.0/pyseistr/mf.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 def mf(D,nfw=7,ifb=1,axis=2):
-	#MF: median filter along first or second axis for 2D profile
-	#  IN   D:   	intput data 
-	#       nfw:    window size 
-	#       ifb:    if use padded boundary (if not, zero will be padded)
-	#       axis:   along the vertical (1) or horizontal (2) axis
-	#      
-	#  OUT   D1:  	output data
-	# 
-	#  Copyright (C) 2014 The University of Texas at Austin
-	#  Copyright (C) 2014 Yangkang Chen
-	#  Ported to python in Apr, 17, 2022
-	#
-	#  This program is free software: you can redistribute it and/or modify
-	#  it under the terms of the GNU General Public License as published
-	#  by the Free Software Foundation, either version 3 of the License, or
-	#  any later version.
-	#
-	#  This program is distributed in the hope that it will be useful,
-	#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-	#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-	#  GNU General Public License for more details: http://www.gnu.org/licenses/
-	#  
-	# References
-	# Huang et al., 2021, Erratic noise suppression using iterative structure-oriented space-varying median filtering with sparsity constraint, Geophysical Prospecting, 69, 101-121.
-	# Chen et al., 2020, Deblending of simultaneous-source data using a structure-oriented space-varying median filter, Geophysical Journal International, 222, 1805–1823.
-	# Gan et al., 2016, Separation of simultaneous sources using a structural-oriented median filter in the flattened dimension, Computers & Geosciences, 86, 46-54.
-	# Chen, Y., 2015, Deblending using a space-varying median filter, Exploration Geophysics, 46, 332-341.
+	'''
+	MF: median filter along first or second axis for 2D profile
+	
+	INPUT 
+	D:   	intput data 
+	nfw:    window size 
+	ifb:    if use padded boundary (if not, zero will be padded)
+	axis:   along the vertical (1) or horizontal (2) axis
+	    
+	OUTPUT 
+	D1:  	output data
+	
+	Copyright (C) 2014 The University of Texas at Austin
+	Copyright (C) 2014 Yangkang Chen
+	Ported to python in Apr, 17, 2022
+	
+	This program is free software: you can redistribute it and/or modify
+	it under the terms of the GNU General Public License as published
+	by the Free Software Foundation, either version 3 of the License, or
+	any later version.
+	
+	This program is distributed in the hope that it will be useful,
+	but WITHOUT ANY WARRANTY; without even the implied warranty of
+	MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+	GNU General Public License for more details: http://www.gnu.org/licenses/
+	
+	References
+	Huang et al., 2021, Erratic noise suppression using iterative structure-oriented space-varying median filtering with sparsity constraint, Geophysical Prospecting, 69, 101-121.
+	Chen et al., 2020, Deblending of simultaneous-source data using a structure-oriented space-varying median filter, Geophysical Journal International, 222, 1805–1823.
+	Gan et al., 2016, Separation of simultaneous sources using a structural-oriented median filter in the flattened dimension, Computers & Geosciences, 86, 46-54.
+	Chen, Y., 2015, Deblending using a space-varying median filter, Exploration Geophysics, 46, 332-341.
+	'''
 	import numpy as np
 
 	# nfw should be odd
 	if np.mod(nfw,2)==0:
 		nfw=nfw+1;
 
 	if axis==2:
@@ -51,34 +56,39 @@
 	if axis==2:
 		D1=D1.transpose();
 		
 	return D1
 
 
 def svmf(D,nfw=7,ifb=1,axis=2,l1=2,l2=0,l3=2,l4=4):
-	#SVMF: space-varying median filter along first or second axis for 2D profile
-	#  IN   D:   	intput data 
-	#       nfw:    window size
-	#       ifb:    if use padded boundary (if not, zero will be padded)
-	#       axis:   along the vertical (1) or horizontal (2) axis
-	#      
-	#  OUT   D1:  	output data
+	'''
+	SVMF: space-varying median filter along first or second axis for 2D profile
+	
+	INPUT   
+	D:   	intput data 
+	nfw:    window size
+	ifb:    if use padded boundary (if not, zero will be padded)
+	axis:   along the vertical (1) or horizontal (2) axis
+	    
+	OUTPUT  
+	D1:  	output data
 	# 		 win_len: window length distribution
-	#  Copyright (C) 2019 Yangkang Chen
-	#
-	#  This program is free software: you can redistribute it and/or modify
-	#  it under the terms of the GNU General Public License as published
-	#  by the Free Software Foundation, either version 3 of the License, or
-	#  any later version.
-	#
-	#  This program is distributed in the hope that it will be useful,
-	#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-	#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-	#  GNU General Public License for more details: http://www.gnu.org/licenses/
-	#
+	
+	Copyright (C) 2019 Yangkang Chen
+	
+	This program is free software: you can redistribute it and/or modify
+	it under the terms of the GNU General Public License as published
+	by the Free Software Foundation, either version 3 of the License, or
+	any later version.
+	
+	This program is distributed in the hope that it will be useful,
+	but WITHOUT ANY WARRANTY; without even the implied warranty of
+	MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+	GNU General Public License for more details: http://www.gnu.org/licenses/
+	'''
 	import numpy as np
 	n1=D.shape[0];
 	n2=D.shape[1];
 	
 	
 	Dtmp=mf(D,nfw,ifb,axis);
 	medianv=np.sum(np.abs(Dtmp.flatten()))/(n1*n2);
```

### Comparing `pyseistr-0.0.4.3.1/pyseistr/operators.py` & `pyseistr-0.0.4.4.0/pyseistr/operators.py`

 * *Files 16% similar despite different names*

```diff
@@ -107,24 +107,26 @@
 	else:
 		dout=yy;
 
 	return dout
 
 
 def passfilter(p,nw):
-	# passfilter: find filter coefficients£®verfied)
-	# All-pass plane-wave destruction filter coefficients
-	#
-	# INPUT
-	# p: slope
-	# nw: filter order
-	#
-	# OUTPUT
-	# a: output filter (n+1) (1D array)
-	#
+	'''
+	passfilter: find filter coefficients£®verfied)
+	All-pass plane-wave destruction filter coefficients
+	
+	INPUT
+	p: slope
+	nw: filter order
+	
+	OUTPUT
+	a: output filter (n+1) (1D array)
+	
+	'''
 	n=nw*2;
 	b=np.zeros([n+1,1]);
 	a=np.zeros([n+1,1]);
 	
 	for k in range(0,n+1):
 		bk=1;
 		for j in range(0,n):
@@ -144,32 +146,33 @@
 				ak=ak*(p+j+1);
 		a[k]=ak;
 
 	return a,b
 
 
 def adjnull( adj,add,nm,nd,m,d ):
-	#Claerbout-style adjoint zeroing Zeros out the output (unless add is true). 
-	#Useful first step for and linear operator.
-	# 
-	#  This program is free software; you can redistribute it and/or modify
-	#  it under the terms of the GNU General Public License as published by
-	#  the Free Software Foundation; either version 2 of the License, or
-	#  (at your option) and later version.
-	#  
-	#  This program is distributed in the hope that it will be useful,
-	#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-	#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-	#  GNU General Public License for more details.
-	#  
-	#  You should have received a copy of the GNU General Public License
-	#  along with this program; if not, write to the Free Software
-	#  Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
-	#adj : adjoint flag; add: addition flag; nm: size of m; nd: size of d
-
+	'''
+	Claerbout-style adjoint zeroing Zeros out the output (unless add is true). 
+	Useful first step for and linear operator.
+	
+	This program is free software; you can redistribute it and/or modify
+	it under the terms of the GNU General Public License as published by
+	the Free Software Foundation; either version 2 of the License, or
+	(at your option) and later version.
+	
+	This program is distributed in the hope that it will be useful,
+	but WITHOUT ANY WARRANTY; without even the implied warranty of
+	MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+	GNU General Public License for more details.
+	
+	You should have received a copy of the GNU General Public License
+	along with this program; if not, write to the Free Software
+	Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
+	adj : adjoint flag; add: addition flag; nm: size of m; nd: size of d
+	'''
 	if add:
 		return m,d
 
 	if adj:
 		m=np.zeros(nm);
 		for i in range(0,nm):
 			m[i] = 0.0;
```

### Comparing `pyseistr-0.0.4.3.1/pyseistr/plot.py` & `pyseistr-0.0.4.4.0/pyseistr/plot.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3.1/pyseistr/pwspray2d.py` & `pyseistr-0.0.4.4.0/pyseistr/pwspray2d.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import numpy as np
 def pwspray2d(u1,dip,nr,order,eps):
-	# pwspray2d: 2D plane-wave spray operator
-	#
-	# INPUT:
-	# u1: noisy data  
-	# dip: slope 
-	# nr: spray radius
-	# order: PWD order
-	# eps: regularization (default:0.01);
-	#
-	# OUTPUT:
-	# u: smooth data
-   
+	'''
+	pwspray2d: 2D plane-wave spray operator
+	
+	INPUT
+	u1: noisy data  
+	dip: slope 
+	nr: spray radius
+	order: PWD order
+	eps: regularization (default:0.01);
+	
+	OUTPUT
+	u: smooth data
+   	'''
 	[n1,n2]=u1.shape;
 	ns=nr;	 	#spray radius
 	ns2=2*ns+1;	#spray diameter
 
 	n=n1*n2;nu=n1*n2*ns2;
 
 	u=np.zeros(n1*ns2*n2);
@@ -63,29 +64,30 @@
 			[w,diag,offd,trace] = predict_step(e,nw,1,p[:,ip-1],trace);
 			for i1 in range(0,n1):
 				u[j*n1+i1]= u[j*n1+i1]+trace[i1];
 
 	return u
 
 def predict_step(e,nw,forw,pp,trace1):
-	# predict_step: prediction step
-	#
-	# INPUT:
-	# e: regularization parameter (default, 0.01*0.01);
-	# nw: accuracy order
-	# forw: forward or backward
-	# n1: trace length
-	# pp: slope
-	# trace: input trace
-	# 
-	# OUTPUT:
-	# w: PWD object
-	# diag,offd: diagonal/offdiagonals of the banded matrix
-	# trace: output trace
-	#
+	'''
+	predict_step: prediction step
+	
+	INPUT
+	e: regularization parameter (default, 0.01*0.01);
+	nw: accuracy order
+	forw: forward or backward
+	n1: trace length
+	pp: slope
+	trace: input trace
+	
+	OUTPUT
+	w: PWD object
+	diag,offd: diagonal/offdiagonals of the banded matrix
+	trace: output trace
+	'''
 	n1=trace1.shape[0];
 	nb=2*nw;
 	eps=e;
 	eps2=e;
 
 	diag=np.zeros(n1);
 	offd=np.zeros([n1,nb]);
@@ -116,27 +118,29 @@
 
 	trace = banded_solve(n1,nb,diag,offd,trace);   
 
 	return w,diag,offd,trace
 
 
 def regularization(diag,offd,nw,eps,eps2):
-	# fill diag and offd using regularization 
-	# 
-	# INPUT:
-	# diag: defined diagonal .   (1D array)
-	# offd: defined off-diagonal (2D array)
-	# eps: regularization parameter (default: e*e, e=0.01);
-	# eps2: second regularization parameter (default, same as eps)
-	# nw: accuracy order (nb=2*nw)
-	#
-	# OUTPUT:
-	# diag: defined diagonal .   (1D array)
-	# offd: defined off-diagonal (2D array)
+	'''
+	fill diag and offd using regularization 
+	
+	INPUT
+	diag: defined diagonal .   (1D array)
+	offd: defined off-diagonal (2D array)
+	eps: regularization parameter (default: e*e, e=0.01);
+	eps2: second regularization parameter (default, same as eps)
+	nw: accuracy order (nb=2*nw)
+	
+	OUTPUT
+	diag: defined diagonal .   (1D array)
+	offd: defined off-diagonal (2D array)
 	#
+	'''
 
 	nb=2*nw;
 	n1=diag.size;
 
 	for i1 in range(0,n1):
 		diag[i1]=6*eps;
 		offd[i1,0]=-4*eps;
@@ -153,30 +157,31 @@
 	
 		offd[0,0]=-2*eps;
 		offd[n1-2,0]=-2*eps;
 
 	return diag,offd
 
 def pwd_define(forw,diag,offd,n1,nw,pp):
-	# pwd_define: matrix multiplication
-	# 
-	# INPUT:
-	# forw:forward or backward
-	# diag: defined diagonal .   (1D array)
-	# offd: defined off-diagonal (2D array)
-	# n1: trace length
-	# nw: PWD filter(accuracy) order (default nw=1)
-	# pp: slope				  (1D array)
-	#
-	# OUTPUT:
-	# diag: defined diagonal .   (1D array)
-	# offd: defined off-diagonal (2D array)
-	# w: PWD object(struct)
-	#
-	#
+	'''
+	pwd_define: matrix multiplication
+	
+	INPUT
+	forw:forward or backward
+	diag: defined diagonal .   (1D array)
+	offd: defined off-diagonal (2D array)
+	n1: trace length
+	nw: PWD filter(accuracy) order (default nw=1)
+	pp: slope				  (1D array)
+	
+	OUTPUT
+	diag: defined diagonal .   (1D array)
+	offd: defined off-diagonal (2D array)
+	w: PWD object(struct)
+	
+	'''
 	
 	#define PWD object(struct)
 	w={'n':n1,'na':2*nw+1,'a':np.zeros([n1,2*nw+1]),'b':np.zeros(2*nw+1)}
 	
 	n=w['n'];
 	nb=2*nw;
 
@@ -201,26 +206,27 @@
 					aj=w['a'][k,j];
 					am=w['a'][k,j-m-1];
 					offd[i,m]=offd[i,m]+am*aj;
 	return w,diag,offd
 
 
 def passfilter(p,nw):
-	# passfilter: find filter coefficients 
-	# All-pass plane-wave destruction filter coefficients
-	# 
-	# INPUT:
-	# p: slope
-	# nw: PWD filter(accuracy) order
-	#
-	# OUTPUT:
-	# a: output filter (n+1) (1D array)
-	# b: temp variable of a
-	#
-
+	'''
+	passfilter: find filter coefficients 
+	All-pass plane-wave destruction filter coefficients
+	
+	INPUT
+	p: slope
+	nw: PWD filter(accuracy) order
+	
+	OUTPUT
+	a: output filter (n+1) (1D array)
+	b: temp variable of a
+	
+	'''
 	n=nw*2;
 	b=np.zeros(n+1);
 	a=np.zeros(n+1);
 	for k in range(0,n+1):
 		bk=1;
 		for j in range(0,n):
 			if j<n-k:
@@ -235,32 +241,34 @@
 				ak=ak*(n-j-p);
 			else:
 				ak=ak*(p+j+1);
 		a[k]=ak;
 	return a,b
 
 def pwd_set(adj,w,diag,offd,pp,inp):
-	# pwd_set: matrix multiplication
-	# 
-	# INPUT:
-	# adj:adjoint flag
-	# w: PWD object(struct)
-	# diag: defined diagonal .   (1D array)
-	# offd: defined off-diagonal (2D array)
-	# pp: slope				  (1D array)
-	# inp: model
-	#
-	# OUTPUT:
-	# out: data 
-	#
+	'''
+	pwd_set: matrix multiplication
+	
+	INPUT
+	adj:adjoint flag
+	w: PWD object(struct)
+	diag: defined diagonal .   (1D array)
+	offd: defined off-diagonal (2D array)
+	pp: slope				  (1D array)
+	inp: model
+	
+	OUTPUT
+	out: data 
+	
+	'''
 
 	n=w['n'];
 	nw=np.int((w['na']-1)/2);
 
-	#	# pwd_set
+	#	pwd_set
 	tmp=np.zeros(n);
 	out=np.zeros(n);
 	if adj:
 		for i in range(0,n):
 			tmp[i]=0.0;
 
 		for i in range(0,n):
@@ -287,26 +295,28 @@
 			for j in range(0,w['na']):
 				k=i+j-nw;
 				if k>=nw and k<n-nw:
 					out[i]=out[i]+w['a'][k,j]*tmp[k];
 	return out
 
 def banded_solve(n,band,diag,offd,b):
-	# banded_solve: Banded matrix solver
-	# 
-	# INPUT:
-	# n:	matrix size
-	# band: band size
-	# diag: defined diagonal .   (1D array)
-	# offd: defined off-diagonal (2D array)
-	# b: input trace
-	#
-	# OUTPUT:
-	# b: trace solution
-	#
+	'''
+	banded_solve: Banded matrix solver
+	
+	INPUT
+	n:	matrix size
+	band: band size
+	diag: defined diagonal .   (1D array)
+	offd: defined off-diagonal (2D array)
+	b: input trace
+	
+	OUTPUT
+	b: trace solution
+	
+	'''
 
 	#define Band object(struct)
 	slv={'n':n,'band':band,'d':np.zeros(n),'o':np.zeros([n-1,band])}
 
 	# define the banded matrix
 	for k in range(0,slv['n']):
 		t=diag[k];
@@ -320,15 +330,14 @@
 			t=offd[k,n];
 			m1=np.min([k,slv['band']-n-1]);
 			for m in range(0,m1):
 				t=t-slv['o'][k-m-1,m]*slv['o'][k-m-1,n+m+1]*slv['d'][k-m-1];
 
 			slv['o'][k,n]=t/slv['d'][k];
 
-
 	# the solver 
 	for k in range(1,slv['n']):
 		t=b[k];
 		m1=np.min([k,slv['band']]);
 		for m in range(0,m1):
 			t=t-slv['o'][k-m-1,m]*b[k-m-1];
 		b[k]=t;
```

### Comparing `pyseistr-0.0.4.3.1/pyseistr/pwspray3d.py` & `pyseistr-0.0.4.4.0/pyseistr/pwspray3d.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import numpy as np
 def pwspray3d(din,dipi,dipx,ns2,ns3,order,eps):
-	#pwspray3d: 3D plane-wave spray operator 
-	# 
-	# by Yangkang Chen, 2022
-	#
-	# INPUT:
-	# din: input
-	# dipi: inline slope
-	# dipx: xline slope
-	# ns2/3: smoothing radius
-	# order: PWD order
-	# eps: regularization (default:0.01);
-	# 
-	# OUTPUT:
-	# dout: result
-	# 
+	'''
+	pwspray3d: 3D plane-wave spray operator 
+	
+	by Yangkang Chen, 2022
+	
+	INPUT
+	din: input
+	dipi: inline slope
+	dipx: xline slope
+	ns2/3: smoothing radius
+	order: PWD order
+	eps: regularization (default:0.01);
+	
+	OUTPUT
+	dout: result
+	
+	'''
 	[n1,n2,n3]=din.shape;
 	n23=n2*n3;
 
 	np2=2*ns2+1;	#spray diameter
 	np3=2*ns3+1;	#spray diameter
 	nnp=np2*np3;
 
@@ -103,47 +105,44 @@
 					u[:,jp,j] = predict2_step(e,nw,up2,up3,q2,q3,u[:,k2,j2],u[:,k3,j3]);
 		
 	dout=u.reshape(n1,nnp,n2,n3,order='F');
 
 	return dout
 
 def get_update(ii, n1,n2, t, visit):
-	# forward or backward options
-	# 
-	# INPUT
-	# ii: loop number
-	# n1:   [n1,n2]=size(t)
-	# n2:   [n1,n2]=size(t)
-	# t:	traveltime
-	# visit: sorted sequence of t
-	# 
-	# OUTPUT
-	# jj: local linear index
-	# up: prediction type
-	# up1: forward or backward
-	# up2: forward or backward
+	'''
+	forward or backward options
+	
+	INPUT
+	ii: loop number
+	n1:   [n1,n2]=size(t)
+	n2:   [n1,n2]=size(t)
+	t:	traveltime
+	visit: sorted sequence of t
+	
+	OUTPUT
+	jj: local linear index
+	up: prediction type
+	up1: forward or backward
+	up2: forward or backward
+	'''
 
 
 	n12=n1*n2;
 	jj=visit[ii];
 	t1=t[jj];
 
 	i1=np.mod(jj,n1);
 	i2=np.floor(jj/n1);
 
 	up=0;
 	if n1>1:
 		a1=jj-1;
 		b1=jj+1;
 		
-# 		print(ii)
-# 		print(visit.shape)
-# 		print(jj)
-# 		print(a1)
-# 		print((t[a1]>t[b1]))
 		up1= (i1 and ((i1==n1-1) or (1!= (t[a1]>t[b1]))));
 		if up1:
 			c1=a1;
 		else:
 			c1=b1;
 
 		if t1>t[c1]:
@@ -161,26 +160,28 @@
 
 		if t1>t[c2]:
 			up = up | 2; 	#Bit-wise OR.
 
 	return up, jj, up1, up2
 
 def predict1_step(e,nw,forw,pp,trace1):
-	# predict1_step: prediction step from one trace
-	# 
-	# INPUT:
-	# e: regularization parameter (default, 0.01*0.01);
-	# nw: accuracy order
-	# forw: forward or backward
-	# pp: slope
-	# trace1: input trace
-	# 
-	# OUTPUT:
-	# trace: output trace
-	#
+	'''
+	predict1_step: prediction step from one trace
+	
+	INPUT
+	e: regularization parameter (default, 0.01*0.01);
+	nw: accuracy order
+	forw: forward or backward
+	pp: slope
+	trace1: input trace
+	
+	OUTPUT
+	trace: output trace
+	
+	'''
 	n1=trace1.shape[0];
 	nb=2*nw;
 	eps=e;
 	eps2=e;
 
 	diag=np.zeros(n1);
 	offd=np.zeros([n1,nb]);
@@ -206,27 +207,28 @@
 
 	trace = banded_solve(n1,nb,diag,offd,trace);   
 
 	return trace
 
 
 def regularization(diag,offd,nw,eps,eps2):
-	# fill diag and offd using regularization 
-	# 
-	# INPUT:
-	# diag: defined diagonal .   (1D array)
-	# offd: defined off-diagonal (2D array)
-	# eps: regularization parameter (default: e*e, e=0.01);
-	# eps2: second regularization parameter (default, same as eps)
-	# nw: accuracy order (nb=2*nw)
-	#
-	# OUTPUT:
-	# diag: defined diagonal .   (1D array)
-	# offd: defined off-diagonal (2D array)
-	#
+	'''
+	fill diag and offd using regularization 
+	
+	INPUT
+	diag: defined diagonal .   (1D array)
+	offd: defined off-diagonal (2D array)
+	eps: regularization parameter (default: e*e, e=0.01);
+	eps2: second regularization parameter (default, same as eps)
+	nw: accuracy order (nb=2*nw)
+	
+	OUTPUT
+	diag: defined diagonal .   (1D array)
+	offd: defined off-diagonal (2D array)
+	'''
 
 	nb=2*nw;
 	n1=diag.size;
 
 	for i1 in range(0,n1):
 		diag[i1]=6*eps;
 		offd[i1,0]=-4*eps;
@@ -243,30 +245,31 @@
 	
 		offd[0,0]=-2*eps;
 		offd[n1-2,0]=-2*eps;
 
 	return diag,offd
 
 def pwd_define(forw,diag,offd,n1,nw,pp):
-	# pwd_define: matrix multiplication
-	# 
-	# INPUT:
-	# forw:forward or backward
-	# diag: defined diagonal .   (1D array)
-	# offd: defined off-diagonal (2D array)
-	# n1: trace length
-	# nw: PWD filter(accuracy) order (default nw=1)
-	# pp: slope				  (1D array)
-	#
-	# OUTPUT:
-	# diag: defined diagonal .   (1D array)
-	# offd: defined off-diagonal (2D array)
-	# w: PWD object(struct)
-	#
-	#
+	'''
+	pwd_define: matrix multiplication
+	
+	INPUT
+	forw:forward or backward
+	diag: defined diagonal .   (1D array)
+	offd: defined off-diagonal (2D array)
+	n1: trace length
+	nw: PWD filter(accuracy) order (default nw=1)
+	pp: slope				  (1D array)
+	
+	OUTPUT
+	diag: defined diagonal .   (1D array)
+	offd: defined off-diagonal (2D array)
+	w: PWD object(struct)
+	
+	'''
 	
 	#define PWD object(struct)
 	w={'n':n1,'na':2*nw+1,'a':np.zeros([n1,2*nw+1]),'b':np.zeros(2*nw+1)}
 	
 	n=w['n'];
 	nb=2*nw;
 
@@ -291,25 +294,27 @@
 					aj=w['a'][k,j];
 					am=w['a'][k,j-m-1];
 					offd[i,m]=offd[i,m]+am*aj;
 	return w,diag,offd
 
 
 def passfilter(p,nw):
-	# passfilter: find filter coefficients 
-	# All-pass plane-wave destruction filter coefficients
-	# 
-	# INPUT:
-	# p: slope
-	# nw: PWD filter(accuracy) order
-	#
-	# OUTPUT:
-	# a: output filter (n+1) (1D array)
-	# b: temp variable of a
-	#
+	'''
+	passfilter: find filter coefficients 
+	All-pass plane-wave destruction filter coefficients
+	
+	INPUT
+	p: slope
+	nw: PWD filter(accuracy) order
+	
+	OUTPUT
+	a: output filter (n+1) (1D array)
+	b: temp variable of a
+	
+	'''
 
 	n=nw*2;
 	b=np.zeros(n+1);
 	a=np.zeros(n+1);
 	for k in range(0,n+1):
 		bk=1;
 		for j in range(0,n):
@@ -326,28 +331,29 @@
 			else:
 				ak=ak*(p+j+1);
 		a[k]=ak;
 	return a,b
 
 
 def pwd_set(adj,w,diag,offd,pp,inp):
-	# pwd_set: matrix multiplication
-	# 
-	# INPUT:
-	# adj:adjoint flag
-	# w: PWD object(struct)
-	# diag: defined diagonal .   (1D array)
-	# offd: defined off-diagonal (2D array)
-	# pp: slope				  (1D array)
-	# inp: model
-	#
-	# OUTPUT:
-	# out: data 
-	#
-
+	'''
+	pwd_set: matrix multiplication
+	
+	INPUT
+	adj:adjoint flag
+	w: PWD object(struct)
+	diag: defined diagonal .   (1D array)
+	offd: defined off-diagonal (2D array)
+	pp: slope				  (1D array)
+	inp: model
+	
+	OUTPUT
+	out: data 
+	
+	'''
 	n=w['n'];
 	nw=np.int((w['na']-1)/2);
 
 	#	# pwd_set
 	tmp=np.zeros(n);
 	out=np.zeros(n);
 	if adj:
@@ -379,27 +385,28 @@
 				k=i+j-nw;
 				if k>=nw and k<n-nw:
 					out[i]=out[i]+w['a'][k,j]*tmp[k];
 	return out
 
 
 def banded_solve(n,band,diag,offd,b):
-	# banded_solve: Banded matrix solver
-	# 
-	# INPUT:
-	# n:	matrix size
-	# band: band size
-	# diag: defined diagonal .   (1D array)
-	# offd: defined off-diagonal (2D array)
-	# b: input trace
-	#
-	# OUTPUT:
-	# b: trace solution
-	#
-
+	'''
+	banded_solve: Banded matrix solver
+	
+	INPUT
+	n:	matrix size
+	band: band size
+	diag: defined diagonal .   (1D array)
+	offd: defined off-diagonal (2D array)
+	b: input trace
+	
+	OUTPUT
+	b: trace solution
+	
+	'''
 	#define Band object(struct)
 	slv={'n':n,'band':band,'d':np.zeros(n),'o':np.zeros([n-1,band])}
 
 	# define the banded matrix
 	for k in range(0,slv['n']):
 		t=diag[k];
 		m1=np.min([k,slv['band']]);
@@ -434,29 +441,31 @@
 		b[k]=t;
 
 
 	return b
 
 
 def predict2_step(e,nw,forw1,forw2,pp1,pp2,trace1,trace2):
-	# predict2_step: prediction step from two trace
-	# 
-	# INPUT:
-	# e: regularization parameter (default, 0.01*0.01);
-	# nw: accuracy order
-	# forw1: forward or backward
-	# forw2: forward or backward
-	# pp1: slope
-	# pp2: slope
-	# trace1: input trace
-	# trace2: input trace
-	# 
-	# OUTPUT:
-	# trace: output trace
-	#
+	'''
+	predict2_step: prediction step from two trace
+	
+	INPUT
+	e: regularization parameter (default, 0.01*0.01);
+	nw: accuracy order
+	forw1: forward or backward
+	forw2: forward or backward
+	pp1: slope
+	pp2: slope
+	trace1: input trace
+	trace2: input trace
+	
+	OUTPUT
+	trace: output trace
+	
+	'''
 	n1=trace1.shape[0];
 	nb=2*nw;
 	eps=e;
 	eps2=e;
 
 	diag=np.zeros(n1);
 	offd=np.zeros([n1,nb]);
```

### Comparing `pyseistr-0.0.4.3.1/pyseistr/soint2d.py` & `pyseistr-0.0.4.4.0/pyseistr/soint2d.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from soint2dcfun import *
 
 def soint2d(din,mask,dip,order=1,niter=100,njs=[1,1],drift=0,verb=1):
-	# soint2d: 2D structure-oriented interpolation
-	# 
-	# by Yangkang Chen, 2022
-	#
-	# INPUT:
-	# dn: model  noisy data
-	# dip: slope
-	# order:    PWD order
-	# eps: regularization (default:0.01);
-	# 
-	# OUTPUT:
-	# ds: filtered data 
-	#
-	# Demo
-	# demos/test_pyseistr_soint2d.py
+	'''
+	soint2d: 2D structure-oriented interpolation
 	
+	by Yangkang Chen, 2022
+	
+	INPUT
+	dn: model  noisy data
+	dip: slope
+	order:    PWD order
+	eps: regularization (default:0.01);
+	
+	OUTPUT
+	ds: filtered data 
+	
+	EXAMPLE
+	demos/test_pyseistr_soint2d.py
+	'''
 	from .solvers import solver
 	from .solvers import cgstep
 	from .operators import allpass3_lop
 	import numpy as np
 	
 	nw=order;
 	nj1=njs[0];
@@ -47,33 +48,34 @@
 	
 	dout=din
 
 	return dout
 	
 	
 def soint2dc(din,mask,dip,order=1,niter=100,njs=[1,1],drift=0,hasmask=1,twoplane=0,prec=0,verb=1):
-	# soint2d: 3D structure-oriented interpolation
-	# 
-	# by Yangkang Chen, 2022
-	#
-	# INPUT:
-	# dn: model  noisy data
-	# dipi: inline slope
-	# dipx: xline slope
-	# r1,r2:    spray radius
-	# order:    PWD order
-	# eps: regularization (default:0.01);
-	# hasmask: if 1, using the provided mask; if 0, using the data itself to determine
-	# 
-	# OUTPUT:
-	# ds: filtered data 
-	#
-	# Demo
-	# demos/test_pyseistr_soint3d.py
+	'''
+	soint2d: 3D structure-oriented interpolation
+	
+	by Yangkang Chen, 2022
 	
+	INPUT
+	dn: model  noisy data
+	dipi: inline slope
+	dipx: xline slope
+	r1,r2:    spray radius
+	order:    PWD order
+	eps: regularization (default:0.01);
+	hasmask: if 1, using the provided mask; if 0, using the data itself to determine
+	
+	OUTPUT
+	ds: filtered data 
+	
+	EXAMPLE
+	demos/test_pyseistr_soint3d.py
+	'''
 	from .solvers import solver
 	from .solvers import cgstep
 	from .operators import allpass3_lop
 	import numpy as np
 	
 	nw=order;
 	nj1=njs[0];
```

### Comparing `pyseistr-0.0.4.3.1/pyseistr/soint3d.py` & `pyseistr-0.0.4.4.0/pyseistr/soint3d.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 def soint3d(din,mask,dipi,dipx,order=1,niter=100,njs=[1,1],drift=0,verb=1):
 	'''
 	soint3d: 3D structure-oriented interpolation
 	
 	by Yangkang Chen, 2022
 	
-	INPUT:
+	INPUT
 	dn: model  noisy data
 	dipi: inline slope
 	dipx: xline slope
 	order:    PWD order
 	
-	OUTPUT:
+	OUTPUT
 	dout: filtered data 
 
-	Demo
-	demos/test_xxx_soint3d.py
+	EXAMPLE
+	demos/test_pyseistr_soint3d.py
 	'''
 	from .solvers import solver
 	from .solvers import cgstep
 	from .operators import allpass3_lop
 	import numpy as np
 	
 	nw=order;
@@ -60,32 +60,32 @@
 	dout=mm2.reshape(n1,n2,n3,order='F');
 
 	return dout
 	
 	
 def soint3dc(din,mask,dipi,dipx,order=1,niter=100,njs=[1,1],drift=0,seed=202223,hasmask=1,var=0,verb=1):
 	'''
-	# soint3d: 3D structure-oriented interpolation
-	# 
-	# by Yangkang Chen, 2022
-	#
-	# INPUT:
-	# dn: model  noisy data
-	# dipi: inline slope
-	# dipx: xline slope
-	# r1,r2:    spray radius
-	# order:    PWD order
-	# eps: regularization (default:0.01);
-	# hasmask: if 1, using the provided mask; if 0, using the data itself to determine
-	# 
-	# OUTPUT:
-	# dout: filtered data 
-	#
-	# Demo
-	# demos/test_xxx_soint3d.py
+	soint3dc: 3D structure-oriented interpolation implemented in C
+	
+	by Yangkang Chen, 2022
+	
+	INPUT
+	dn: model  noisy data
+	dipi: inline slope
+	dipx: xline slope
+	r1,r2:    spray radius
+	order:    PWD order
+	eps: regularization (default:0.01);
+	hasmask: if 1, using the provided mask; if 0, using the data itself to determine
+	
+	OUTPUT
+	dout: filtered data 
+	
+	EXAMPLE
+	demos/test_pyseistr_soint3d.py
 	'''
 	
 	from .solvers import solver
 	from .solvers import cgstep
 	from .operators import allpass3_lop
 	import numpy as np
```

### Comparing `pyseistr-0.0.4.3.1/pyseistr/solvers.py` & `pyseistr-0.0.4.4.0/pyseistr/solvers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 import numpy as np
 def solver(opL,solv,nx,ny,x,dat,niter,par_L,par):
-	#Generic linear solver. (same as Madagascar function: sf_solver)
-	#
-	#Solves
-	#L{x}    =~ dat
-	#
-	#Yangkang Chen
-	#Aug, 05, 2020
-	#Ported to Python in Apr, 25, 2022
-	#
-	#INPUT
-	#opL: forward/linear operator
-	#solv: stepping function
-	#nx:   size of x   (1D vector)
-	#ny:   size of dat (1D vector)
-	#x:    estimated model
-	#dat:  data
-	#niter:number of iterations
-	#
-	#par. (parameter struct)
-	#  "wt":     float*:         weight      
-	#  "wght":   sf_weight wght: weighting function
-	#  "x0":     float*:         initial model
-	#  "nloper": sf_operator:    nonlinear operator
-	#  "mwt":    float*:         model weight
-	#  "verb":   bool:           verbosity flag
-	#  "known":  bool*:          known model mask
-	#  "nmem":   int:            iteration memory
-	#  "nfreq":  int:            periodic restart
-	#  "xmov":   float**:        model iteration
-	#  "rmov":   float**:        residual iteration
-	#  "err":    float*:         final error
-	#  "res":    float*:         final residual
-	#
-	#OUPUT
-	#x: estimated model
-	#
-	#
+	'''
+	Generic linear solver. (same as Madagascar function: sf_solver)
+	
+	Solves
+	L{x}    =~ dat
+	
+	Yangkang Chen
+	Aug, 05, 2020
+	Ported to Python in Apr, 25, 2022
+	
+	INPUT
+	opL: forward/linear operator
+	solv: stepping function
+	nx:   size of x   (1D vector)
+	ny:   size of dat (1D vector)
+	x:    estimated model
+	dat:  data
+	niter:number of iterations
+	
+	par. (parameter struct)
+	  "wt":     float*:         weight      
+	  "wght":   sf_weight wght: weighting function
+	  "x0":     float*:         initial model
+	  "nloper": sf_operator:    nonlinear operator
+	  "mwt":    float*:         model weight
+	  "verb":   bool:           verbosity flag
+	  "known":  bool*:          known model mask
+	  "nmem":   int:            iteration memory
+	  "nfreq":  int:            periodic restart
+	  "xmov":   float**:        model iteration
+	  "rmov":   float**:        residual iteration
+	  "err":    float*:         final error
+	  "res":    float*:         final residual
+	
+	OUPUT
+	x: estimated model
+	
+	'''
 	
 	TOLERANCE=1.e-12;
 	forget=0;
 	x=x.flatten(order='F');
 	dat=dat.flatten(order='F');
 	xmov=None;
 	rmov=None;
@@ -232,37 +233,39 @@
 	if res  is not None:
 		res=rr;
 		par['res']=res;
 		
 	return x,par
 
 def conjgrad(opP,opL,opS, p, x, dat, eps_cg, tol_cg, N,ifhasp0,par_P,par_L,par_S,verb):
-	#conjgrad: conjugate gradient with shaping
-	#
-	#by Yangkang Chen, 2022
-	#
-	#Modified by Yangkang Chen, Nov, 09, 2019 (fix the "adding" for each oper)
-	#
-	#INPUT
-	#opP: preconditioning operator
-	#opL: forward/linear operator
-	#opS: shaping operator
-	#d:  data
-	#N:  number of iterations
-	#eps_cg:  scaling
-	#tol_cg:  tolerance
-	#ifhasp0: flag indicating if has initial model
-	#par_P: parameters for P
-	#par_L: parameters for L
-	#par_S: parameters for S
-	#verb: verbosity flag
-	#
-	#OUPUT
-	#x: estimated model
-	#
+	'''
+	conjgrad: conjugate gradient with shaping
+	
+	by Yangkang Chen, 2022
+	
+	Modified by Yangkang Chen, Nov, 09, 2019 (fix the "adding" for each oper)
+	
+	INPUT
+	opP: preconditioning operator
+	opL: forward/linear operator
+	opS: shaping operator
+	d:  data
+	N:  number of iterations
+	eps_cg:  scaling
+	tol_cg:  tolerance
+	ifhasp0: flag indicating if has initial model
+	par_P: parameters for P
+	par_L: parameters for L
+	par_S: parameters for S
+	verb: verbosity flag
+	
+	OUPUT
+	x: estimated model
+	
+	'''
 
 	nnp=p.size;
 	nx=par_L['nm'];	#model size
 	nd=par_L['nd'];	#data size
 
 	if opP  is not None:
 		d=-dat; #nd*1
@@ -351,33 +354,34 @@
 	
 		gnp=gn;
 
 	return x
 
 
 def cgstep(forget,nx,ny,x,g,rr,gg):
-	#Step of conjugate-gradient iteration.
-	# Yangkang Chen
-	# Aug, 05, 2020
-	# 
-	# INPUT
-	# forget:restart flag
-	# nx:   model size
-	# ny:   data size
-	# x:    current model [nx]
-	# g:    gradient [nx]
-	# rr:   data residual [ny]
-	# gg:   conjugate gradient [ny]
-	# 
-	# OUTPUT
-	# x:    current model [nx]
-	# g:    gradient [nx]
-	# rr:   data residual [ny]
-	# gg:   conjugate gradient [ny]
-	
+	'''
+	Step of conjugate-gradient iteration.
+	Yangkang Chen
+	Aug, 05, 2020
+	
+	INPUT
+	forget:restart flag
+	nx:   model size
+	ny:   data size
+	x:    current model [nx]
+	g:    gradient [nx]
+	rr:   data residual [ny]
+	gg:   conjugate gradient [ny]
+	
+	OUTPUT
+	x:    current model [nx]
+	g:    gradient [nx]
+	rr:   data residual [ny]
+	gg:   conjugate gradient [ny]
+	'''
 	EPSILON=1.e-12;
 	Allocated=0;
 	if not Allocated:
 		Allocated =1;
 		forget=1;
 		S=np.zeros(nx);
 		Ss=np.zeros(ny);
```

### Comparing `pyseistr-0.0.4.3.1/pyseistr/somf2d.py` & `pyseistr-0.0.4.4.0/pyseistr/somf3d.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,95 +1,98 @@
-from sofcfun import *
+from sof3dcfun import *
 
-def somf2d(dn,dip,ns,order,eps,option=1):
-	# somf2d: structure-oriented median filter
-	#
-	# INPUT:
-	# dn: model   noisy data
-	# dip: slope (2D array)
-	# ns:       spray radius
-	# order:    PWD order
-	# eps: regularization (default:0.01);
-	# option=1 or 2: (1 for MF; 2 for SVMF)
-	#
-	# OUTPUT:
-	# ds:  filtered data
-	#  
-	# References
-	# Huang et al., 2021, Erratic noise suppression using iterative structure-oriented space-varying median filtering with sparsity constraint, Geophysical Prospecting, 69, 101-121.
-	# Chen et al., 2020, Deblending of simultaneous-source data using a structure-oriented space-varying median filter, Geophysical Journal International, 222, 1805–1823.
-	# Gan et al., 2016, Separation of simultaneous sources using a structural-oriented median filter in the flattened dimension, Computers & Geosciences, 86, 46-54.
-	# Chen, Y., 2015, Deblending using a space-varying median filter, Exploration Geophysics, 46, 332-341.
-	#
-	# Demo
-	# demos/test_xxx_somf2d.py
-	
+def somf3d(dn,dipi,dipx,r1,r2,eps,order,option=1):
+	'''
+	somf3d: 3D structure-oriented median filter
+	
+	by Yangkang Chen, 2022
+	
+	INPUT
+	dn: model  noisy data
+	dipi: inline slope
+	dipx: xline slope
+	r1,r2:    spray radius
+	order:    PWD order
+	eps: regularization (default:0.01);
+	
+	OUTPUT
+	ds: filtered data
+	 
+	REFERENCES
+	Huang et al., 2021, Erratic noise suppression using iterative structure-oriented space-varying median filtering with sparsity constraint, Geophysical Prospecting, 69, 101-121.
+	Chen et al., 2020, Deblending of simultaneous-source data using a structure-oriented space-varying median filter, Geophysical Journal International, 222, 1805–1823.
+	Gan et al., 2016, Separation of simultaneous sources using a structural-oriented median filter in the flattened dimension, Computers & Geosciences, 86, 46-54.
+	Chen, Y., 2015, Deblending using a space-varying median filter, Exploration Geophysics, 46, 332-341.
+	
+	EXAMPLE
+	demos/test_pyseistr_somf3d.py
+	'''
 	import numpy as np
-	from .pwspray2d import pwspray2d
+	nnp=(2*r1+1)*(2*r2+1);
+	
+	#flattening
+	from .pwspray3d import pwspray3d
 	from .mf import mf
 	from .mf import svmf
 	
-	n1=dn.shape[0];
-	n2=dn.shape[1];
-	ns2=2*ns+1;	#spray diameter
-
-	#flattening
-	utmp=pwspray2d(dn,dip,ns,order,eps);
-	u=utmp.reshape(n1,ns2,n2,order='F')
-
+	u = pwspray3d(dn,dipi,dipx,r1,r2,order,eps);
 
-	for i2 in range(0,n2):
-		if option==1:
-			u[:,:,i2]=mf(u[:,:,i2],ns2,1,2);
-		else:
-			u[:,:,i2],win_tmp=svmf(u[:,:,i2],ns2,1,2);
-	
-	ds=u[:,ns,:];
+	n3=dn.shape[2];
+	n2=dn.shape[1];
+	ns2=2*r1*r2+1;
+	for i3 in range(0,n3):
+		for i2 in range(0,n2):
+			if option==1:
+				u[:,:,i2,i3]=mf(u[:,:,i2,i3],ns2,1,2);
+			else:
+				u[:,:,i2,i3],win_tmp=svmf(u[:,:,i2,i3],ns2,1,2);
 	
+	ds=u[:,int(nnp/2),:,:];
+
 	return ds
 
-def somf2dc(dn,dip,ns,order,eps,option=1,verb=1):
-	# somf2dc: structure-oriented median filter in C
-	#
-	# INPUT:
-	# dn: model   noisy data
-	# dip: slope (2D array)
-	# ns:       spray radius
-	# order:    PWD order
-	# eps: regularization (default:0.01);
-	# option=1 or 2: (1 for MF; 2 for SVMF)
-	#
-	# OUTPUT:
-	# ds:  filtered data
-	#  
-	# References
-	# Huang et al., 2021, Erratic noise suppression using iterative structure-oriented space-varying median filtering with sparsity constraint, Geophysical Prospecting, 69, 101-121.
-	# Chen et al., 2020, Deblending of simultaneous-source data using a structure-oriented space-varying median filter, Geophysical Journal International, 222, 1805–1823.
-	# Gan et al., 2016, Separation of simultaneous sources using a structural-oriented median filter in the flattened dimension, Computers & Geosciences, 86, 46-54.
-	# Chen, Y., 2015, Deblending using a space-varying median filter, Exploration Geophysics, 46, 332-341.
-	#
-	# Demo
-	# demos/test_xxx_somf2d.py
-	
+
+def somf3dc(dn,dipi,dipx,r1,r2,eps,order,option=1,verb=1):
+	'''
+	somf3dc: 3D structure-oriented median filter implemented in C
+	
+	by Yangkang Chen, 2022
+	
+	INPUT
+	dn: model  noisy data
+	dipi: inline slope
+	dipx: xline slope
+	r1,r2:    spray radius
+	order:    PWD order
+	eps: regularization (default:0.01);
+	
+	OUTPUT
+	ds: filtered data
+	 
+	REFERENCES
+	Huang et al., 2021, Erratic noise suppression using iterative structure-oriented space-varying median filtering with sparsity constraint, Geophysical Prospecting, 69, 101-121.
+	Chen et al., 2020, Deblending of simultaneous-source data using a structure-oriented space-varying median filter, Geophysical Journal International, 222, 1805–1823.
+	Gan et al., 2016, Separation of simultaneous sources using a structural-oriented median filter in the flattened dimension, Computers & Geosciences, 86, 46-54.
+	Chen, Y., 2015, Deblending using a space-varying median filter, Exploration Geophysics, 46, 332-341.
+	
+	EXAMPLE
+	demos/test_pyseistr_somf3d.py
+	'''
 	import numpy as np
-	ns2=2*ns+1;	#spray diameter
-	
+	nnp=(2*r1+1)*(2*r2+1);
+
 	if dn.ndim==2:
 		[n1,n2]=dn.shape;
 		n3=1;
 	else: #assuming ndim=3;
 		[n1,n2,n3]=dn.shape;
-	
+		
 	dn=np.float32(dn).flatten(order='F');
-	dip=np.float32(dip).flatten(order='F');
+	dipi=np.float32(dipi).flatten(order='F');
+	dipx=np.float32(dipx).flatten(order='F');
 	
-	ds=csomf2d(dn,dip,n1,n2,n3,ns,2*ns+1,option,order,eps,verb);
-	ds=ds.reshape(n1,n2,n3,order='F')
-	
-	if n3==1:	#for 2D problems
-		ds=np.squeeze(ds)
+	rmf=2*r1*r2+1; #median filter length
+	ds=csomf3d(dn,dipi,dipx,n1,n2,n3,r1,r2,rmf,option,order,eps,verb);
+	ds=ds.reshape([n1,n2,n3],order='F');
+
 	return ds
-	
 
-	
-	
-
```

### Comparing `pyseistr-0.0.4.3.1/pyseistr/somf3d.py` & `pyseistr-0.0.4.4.0/pyseistr/somf2d.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,94 +1,99 @@
-from sof3dcfun import *
+from sofcfun import *
 
-def somf3d(dn,dipi,dipx,r1,r2,eps,order,option=1):
-	# somf3d: 3D structure-oriented median filter
-	# 
-	# by Yangkang Chen, 2022
-	#
-	# INPUT:
-	# dn: model  noisy data
-	# dipi: inline slope
-	# dipx: xline slope
-	# r1,r2:    spray radius
-	# order:    PWD order
-	# eps: regularization (default:0.01);
-	# 
-	# OUTPUT:
-	# ds: filtered data
-	#  
-	# References
-	# Huang et al., 2021, Erratic noise suppression using iterative structure-oriented space-varying median filtering with sparsity constraint, Geophysical Prospecting, 69, 101-121.
-	# Chen et al., 2020, Deblending of simultaneous-source data using a structure-oriented space-varying median filter, Geophysical Journal International, 222, 1805–1823.
-	# Gan et al., 2016, Separation of simultaneous sources using a structural-oriented median filter in the flattened dimension, Computers & Geosciences, 86, 46-54.
-	# Chen, Y., 2015, Deblending using a space-varying median filter, Exploration Geophysics, 46, 332-341.
-	#
-	# Demo
-	# demos/test_xxx_somf3d.py
-	import numpy as np
-	nnp=(2*r1+1)*(2*r2+1);
+def somf2d(dn,dip,ns,order,eps,option=1):
+	'''
+	somf2d: structure-oriented median filter
 	
-	#flattening
-	from .pwspray3d import pwspray3d
+	INPUT:
+	dn: model   noisy data
+	dip: slope (2D array)
+	ns:       spray radius
+	order:    PWD order
+	eps: regularization (default:0.01);
+	option=1 or 2: (1 for MF; 2 for SVMF)
+	
+	OUTPUT
+	ds:  filtered data
+	 
+	REFERENCES
+	Huang et al., 2021, Erratic noise suppression using iterative structure-oriented space-varying median filtering with sparsity constraint, Geophysical Prospecting, 69, 101-121.
+	Chen et al., 2020, Deblending of simultaneous-source data using a structure-oriented space-varying median filter, Geophysical Journal International, 222, 1805–1823.
+	Gan et al., 2016, Separation of simultaneous sources using a structural-oriented median filter in the flattened dimension, Computers & Geosciences, 86, 46-54.
+	Chen, Y., 2015, Deblending using a space-varying median filter, Exploration Geophysics, 46, 332-341.
+	
+	EXAMPLE
+	demos/test_xxx_somf2d.py
+	'''
+	
+	import numpy as np
+	from .pwspray2d import pwspray2d
 	from .mf import mf
 	from .mf import svmf
 	
-	u = pwspray3d(dn,dipi,dipx,r1,r2,order,eps);
-
-	n3=dn.shape[2];
+	n1=dn.shape[0];
 	n2=dn.shape[1];
-	ns2=2*r1*r2+1;
-	for i3 in range(0,n3):
-		for i2 in range(0,n2):
-			if option==1:
-				u[:,:,i2,i3]=mf(u[:,:,i2,i3],ns2,1,2);
-			else:
-				u[:,:,i2,i3],win_tmp=svmf(u[:,:,i2,i3],ns2,1,2);
-	
-	ds=u[:,int(nnp/2),:,:];
+	ns2=2*ns+1;	#spray diameter
 
-	return ds
+	#flattening
+	utmp=pwspray2d(dn,dip,ns,order,eps);
+	u=utmp.reshape(n1,ns2,n2,order='F')
 
 
-def somf3dc(dn,dipi,dipx,r1,r2,eps,order,option=1,verb=1):
-	# somf3d: 3D structure-oriented median filter implemented in C
-	# 
-	# by Yangkang Chen, 2022
-	#
-	# INPUT:
-	# dn: model  noisy data
-	# dipi: inline slope
-	# dipx: xline slope
-	# r1,r2:    spray radius
-	# order:    PWD order
-	# eps: regularization (default:0.01);
-	# 
-	# OUTPUT:
-	# ds: filtered data
-	#  
-	# References
-	# Huang et al., 2021, Erratic noise suppression using iterative structure-oriented space-varying median filtering with sparsity constraint, Geophysical Prospecting, 69, 101-121.
-	# Chen et al., 2020, Deblending of simultaneous-source data using a structure-oriented space-varying median filter, Geophysical Journal International, 222, 1805–1823.
-	# Gan et al., 2016, Separation of simultaneous sources using a structural-oriented median filter in the flattened dimension, Computers & Geosciences, 86, 46-54.
-	# Chen, Y., 2015, Deblending using a space-varying median filter, Exploration Geophysics, 46, 332-341.
-	#
-	# Demo
-	# demos/test_xxx_somf3d.py
-	import numpy as np
-	nnp=(2*r1+1)*(2*r2+1);
+	for i2 in range(0,n2):
+		if option==1:
+			u[:,:,i2]=mf(u[:,:,i2],ns2,1,2);
+		else:
+			u[:,:,i2],win_tmp=svmf(u[:,:,i2],ns2,1,2);
+	
+	ds=u[:,ns,:];
+	
+	return ds
 
+def somf2dc(dn,dip,ns,order,eps,option=1,verb=1):
+	'''
+	somf2dc: structure-oriented median filter in C
+	
+	INPUT
+	dn: model   noisy data
+	dip: slope (2D array)
+	ns:       spray radius
+	order:    PWD order
+	eps: regularization (default:0.01);
+	option=1 or 2: (1 for MF; 2 for SVMF)
+	
+	OUTPUT
+	ds:  filtered data
+	 
+	REFERENCES
+	Huang et al., 2021, Erratic noise suppression using iterative structure-oriented space-varying median filtering with sparsity constraint, Geophysical Prospecting, 69, 101-121.
+	Chen et al., 2020, Deblending of simultaneous-source data using a structure-oriented space-varying median filter, Geophysical Journal International, 222, 1805–1823.
+	Gan et al., 2016, Separation of simultaneous sources using a structural-oriented median filter in the flattened dimension, Computers & Geosciences, 86, 46-54.
+	Chen, Y., 2015, Deblending using a space-varying median filter, Exploration Geophysics, 46, 332-341.
+	
+	EXAMPLE
+	demos/test_pyseistr_somf2d.py
+	'''
+	
+	import numpy as np
+	ns2=2*ns+1;	#spray diameter
+	
 	if dn.ndim==2:
 		[n1,n2]=dn.shape;
 		n3=1;
 	else: #assuming ndim=3;
 		[n1,n2,n3]=dn.shape;
-		
+	
 	dn=np.float32(dn).flatten(order='F');
-	dipi=np.float32(dipi).flatten(order='F');
-	dipx=np.float32(dipx).flatten(order='F');
+	dip=np.float32(dip).flatten(order='F');
 	
-	rmf=2*r1*r2+1; #median filter length
-	ds=csomf3d(dn,dipi,dipx,n1,n2,n3,r1,r2,rmf,option,order,eps,verb);
-	ds=ds.reshape([n1,n2,n3],order='F');
-
+	ds=csomf2d(dn,dip,n1,n2,n3,ns,2*ns+1,option,order,eps,verb);
+	ds=ds.reshape(n1,n2,n3,order='F')
+	
+	if n3==1:	#for 2D problems
+		ds=np.squeeze(ds)
 	return ds
+	
 
+	
+	
+
```

### Comparing `pyseistr-0.0.4.3.1/pyseistr/src/bp_cfuns.c` & `pyseistr-0.0.4.4.0/pyseistr/src/bp_cfuns.c`

 * *Files 1% similar despite different names*

```diff
@@ -535,18 +535,18 @@
     
     PyObject *f1=NULL;
     PyObject *arrf1=NULL;
 
     
 	PyArg_ParseTuple(args, "Oiiifffiiii", &f1, &n1, &n2, &n3, &d1, &flo, &fhi, &nplo, &nphi, &phase, &verb);
 
-	
-	verb=1;
 	n123=n1*n2*n3;
-	printf("nplo=%d,n123=%d\n",nplo,n123);
+	
+	if(verb)
+		printf("nplo=%d,n123=%d\n",nplo,n123);
 	
     arrf1 = PyArray_FROM_OTF(f1, NPY_FLOAT, NPY_IN_ARRAY);
 
     nd2=PyArray_NDIM(arrf1);
     npy_intp *sp=PyArray_SHAPE(arrf1);
 
 	if(flo<0)
@@ -630,14 +630,16 @@
 	/* Parse tuples separately since args will differ between C fcns */
 	/* Make a new double vector of same dimension */
 	vecout=(PyArrayObject *) PyArray_SimpleNew(1,dims,NPY_FLOAT);
 	for(i=0;i<dims[0];i++)
 		(*((float*)PyArray_GETPTR1(vecout,i))) = trace[i];
 
     free(trace);
+    free(trace1);
+    
 	return PyArray_Return(vecout);
 	
 }
```

### Comparing `pyseistr-0.0.4.3.1/pyseistr/src/dip_cfuns.c` & `pyseistr-0.0.4.4.0/pyseistr/src/dip_cfuns.c`

 * *Files 0% similar despite different names*

```diff
@@ -1796,33 +1796,34 @@
 	eps=f8;
 	
     rect[0]=f11;
     rect[1]=f12;
     rect[2]=f13;
 	hasmask=f14;
 	verb=f15;
-// 	verb=true;
 	
     arrf1 = PyArray_FROM_OTF(f1, NPY_FLOAT, NPY_IN_ARRAY);
     
     nd2=PyArray_NDIM(arrf1);
     npy_intp *sp=PyArray_SHAPE(arrf1);
 
 	
 	if(hasmask==0)
     	if (*sp != n123)
     	{
     		printf("Dimension mismatch, N_input = %d, N_data = %d\n", *sp, n123);
     		return NULL;
     	}
+    if(verb)
+    {
     printf("rect1=%d,rect2=%d,rect3=%d\n",rect[0],rect[1],rect[2]);
 	printf("both=%d,hasmask=%d,verb=%d\n",both,hasmask,verb);
 	printf("n123=%d\n",n123);
 	printf("eps_dv=%f\n",eps);
-
+	} 
 
 	if(n[2]==1)
 	{
 	n4=0;
 	p = ps_floatalloc(n123);
 	}
 	else
@@ -1974,14 +1975,19 @@
 	/* Parse tuples separately since args will differ between C fcns */
 	/* Make a new double vector of same dimension */
 	vecout=(PyArrayObject *) PyArray_SimpleNew(1,dims,NPY_FLOAT);
 	for(i=0;i<dims[0];i++)
 		(*((float*)PyArray_GETPTR1(vecout,i))) = p[i];
 
 	
+	free(p);
+	free(u);
+	free(um);
+	
+	
 	return PyArray_Return(vecout);
 	
 }
```

### Comparing `pyseistr-0.0.4.3.1/pyseistr/src/sof3d_cfuns.c` & `pyseistr-0.0.4.4.0/pyseistr/src/sof3d_cfuns.c`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3.1/pyseistr/src/sof_cfuns.c` & `pyseistr-0.0.4.4.0/pyseistr/src/sof_cfuns.c`

 * *Files 1% similar despite different names*

```diff
@@ -1617,25 +1617,23 @@
 	
 
 	    
 	/*below is MF/SVMF*/
     if(option==1)
     {
     mf_init(n1, np, nmf, 2, 1);
-    	printf("running MF\n");
+    	if (verb) printf("running MF\n");
     }
     else
     {
     svmf_init(n1, np, nmf, 2, 1);
-    	printf("running SVMF\n");
+    	if (verb) printf("running SVMF\n");
     }
     
 
-
-
     for(i=0;i<n2;i++)
     {
     	sum=0;
     	for(j=0;j<n1*np;j++)
     	{tt[j]=u[i][0][j];sum=sum+tt[j];}
     	
     	if(option==1)
@@ -1650,27 +1648,28 @@
 	for(k=0;k<n1;k++)
 	smooth[i*n1+k+i3*n1*n2] = u[i][(np-1)/2][k];
     }
     
 
     }
 
-    
-    
 
     /*Below is the output part*/
     PyArrayObject *vecout;
 	npy_intp dims[2];
 	dims[0]=n123;dims[1]=1;
 	/* Parse tuples separately since args will differ between C fcns */
 	/* Make a new double vector of same dimension */
 	vecout=(PyArrayObject *) PyArray_SimpleNew(1,dims,NPY_FLOAT);
 	for(i=0;i<dims[0];i++)
 		(*((float*)PyArray_GETPTR1(vecout,i))) = smooth[i];
 
+	free(smooth);
+	free(input);
+	free(slope);
 
 	return PyArray_Return(vecout);
 	
 }
```

### Comparing `pyseistr-0.0.4.3.1/pyseistr/src/soint2d_cfuns.c` & `pyseistr-0.0.4.4.0/pyseistr/src/soint2d_cfuns.c`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3.1/pyseistr/src/soint3d_cfuns.c` & `pyseistr-0.0.4.4.0/pyseistr/src/soint3d_cfuns.c`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3.1/pyseistr.egg-info/PKG-INFO` & `pyseistr-0.0.4.4.0/pyseistr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyseistr
-Version: 0.0.4.3.1
+Version: 0.0.4.4.0
 Summary: A python package for structural denoising and interpolation of multi-channel seismic data
 Home-page: https://github.com/aaspip/pyseistr
 Author: pyseistr developing team
 Author-email: chenyk2016@gmail.com
 License: GNU General Public License, Version 3 (GPLv3)
 Keywords: seismology,earthquake seismology,exploration seismology,array seismology,denoising,science,engineering,structure,local slope,filtering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyseistr-0.0.4.3.1/pyseistr.egg-info/SOURCES.txt` & `pyseistr-0.0.4.4.0/pyseistr.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.py
 pyseistr/__init__.py
 pyseistr/bp.py
+pyseistr/das.py
 pyseistr/dip2d.py
 pyseistr/dip3d.py
 pyseistr/divne.py
 pyseistr/fk.py
 pyseistr/mf.py
 pyseistr/operators.py
 pyseistr/plot.py
@@ -16,19 +17,21 @@
 pyseistr/soint2d.py
 pyseistr/soint3d.py
 pyseistr/solvers.py
 pyseistr/somean2d.py
 pyseistr/somean3d.py
 pyseistr/somf2d.py
 pyseistr/somf3d.py
+pyseistr/synthetics.py
 pyseistr.egg-info/PKG-INFO
 pyseistr.egg-info/SOURCES.txt
 pyseistr.egg-info/dependency_links.txt
 pyseistr.egg-info/not-zip-safe
 pyseistr.egg-info/requires.txt
 pyseistr.egg-info/top_level.txt
 pyseistr/src/bp_cfuns.c
+pyseistr/src/coh_cfuns.c
 pyseistr/src/dip_cfuns.c
 pyseistr/src/sof3d_cfuns.c
 pyseistr/src/sof_cfuns.c
 pyseistr/src/soint2d_cfuns.c
 pyseistr/src/soint3d_cfuns.c
```

### Comparing `pyseistr-0.0.4.3.1/setup.py` & `pyseistr-0.0.4.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,25 +25,26 @@
 										include_dirs=[numpy.get_include()])
 sointc3d_module = Extension('soint3dcfun', sources=['pyseistr/src/soint3d_cfuns.c'], 
 										include_dirs=[numpy.get_include()])
 sointc2d_module = Extension('soint2dcfun', sources=['pyseistr/src/soint2d_cfuns.c'], 
 										include_dirs=[numpy.get_include()])
 bpc_module = Extension('bpcfun', sources=['pyseistr/src/bp_cfuns.c'], 
 										include_dirs=[numpy.get_include()])
-
+cohc_module = Extension('cohcfun', sources=['pyseistr/src/coh_cfuns.c'], 
+										include_dirs=[numpy.get_include()])
 setup(
     name="pyseistr",
-    version="0.0.4.3.1",
+    version="0.0.4.4.0",
     license='GNU General Public License, Version 3 (GPLv3)',
     description="A python package for structural denoising and interpolation of multi-channel seismic data",
     long_description=long_description,
     author="pyseistr developing team",
     author_email="chenyk2016@gmail.com",
     url="https://github.com/aaspip/pyseistr",
-    ext_modules=[dipc_module,sofc_module,sofc3d_module,sointc2d_module,sointc3d_module,bpc_module],
+    ext_modules=[dipc_module,sofc_module,sofc3d_module,sointc2d_module,sointc3d_module,bpc_module,cohc_module],
     packages=['pyseistr'],
     include_package_data=True,
     zip_safe=False,
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
```

