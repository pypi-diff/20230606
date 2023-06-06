# Comparing `tmp/SPyOD-0.1.5.tar.gz` & `tmp/SPyOD-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPyOD-0.1.5.tar", last modified: Tue May  2 13:03:53 2023, max compression
+gzip compressed data, was "SPyOD-0.1.6.tar", last modified: Tue Jun  6 02:47:44 2023, max compression
```

## Comparing `SPyOD-0.1.5.tar` & `SPyOD-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:03:53.646647 SPyOD-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-02 13:03:44.000000 SPyOD-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-02 13:03:53.646647 SPyOD-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-02 13:03:44.000000 SPyOD-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-02 13:03:44.000000 SPyOD-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 13:03:53.646647 SPyOD-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:03:53.646647 SPyOD-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:03:53.646647 SPyOD-0.1.5/src/SPyOD.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-02 13:03:53.000000 SPyOD-0.1.5/src/SPyOD.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-02 13:03:53.000000 SPyOD-0.1.5/src/SPyOD.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 13:03:53.000000 SPyOD-0.1.5/src/SPyOD.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 13:03:53.000000 SPyOD-0.1.5/src/SPyOD.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:03:53.646647 SPyOD-0.1.5/src/spyod/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 13:03:44.000000 SPyOD-0.1.5/src/spyod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-02 13:03:44.000000 SPyOD-0.1.5/src/spyod/findpairs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-05-02 13:03:44.000000 SPyOD-0.1.5/src/spyod/spod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:47:44.210894 SPyOD-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-06 02:47:27.000000 SPyOD-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-06 02:47:44.210894 SPyOD-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-06-06 02:47:27.000000 SPyOD-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-06 02:47:28.000000 SPyOD-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 02:47:44.210894 SPyOD-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:47:44.206894 SPyOD-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:47:44.206894 SPyOD-0.1.6/src/SPyOD.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-06 02:47:44.000000 SPyOD-0.1.6/src/SPyOD.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-06 02:47:44.000000 SPyOD-0.1.6/src/SPyOD.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 02:47:44.000000 SPyOD-0.1.6/src/SPyOD.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-06 02:47:44.000000 SPyOD-0.1.6/src/SPyOD.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:47:44.210894 SPyOD-0.1.6/src/spyod/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 02:47:28.000000 SPyOD-0.1.6/src/spyod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-06-06 02:47:28.000000 SPyOD-0.1.6/src/spyod/findpairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16783 2023-06-06 02:47:28.000000 SPyOD-0.1.6/src/spyod/spod.py
```

### Comparing `SPyOD-0.1.5/LICENSE` & `SPyOD-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `SPyOD-0.1.5/PKG-INFO` & `SPyOD-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPyOD
-Version: 0.1.5
+Version: 0.1.6
 Summary: Spectral Proper Orthogonal Decomposition
 Author-email: Grigorios Hatzissawidis <grigorios.hatzissawidis@fst.tu-darmstadt.de>, Moritz Sieber <moritz.sieber@tu-berlin.de>
 Project-URL: Homepage, https://github.com/grigorishat/SPyOD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: SPyOD Version: 0.1.5 Summary: Spectral Proper
+Metadata-Version: 2.1 Name: SPyOD Version: 0.1.6 Summary: Spectral Proper
 Orthogonal Decomposition Author-email: Grigorios Hatzissawidis
 hatzissawidis@fst.tu-darmstadt.de>, Moritz Sieber
 sieber@tu-berlin.de> Project-URL: Homepage, https://github.com/grigorishat/
 SPyOD Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE # Spectral Proper Orthogonal Decomposition ## Table of contents *
```

### Comparing `SPyOD-0.1.5/README.md` & `SPyOD-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `SPyOD-0.1.5/pyproject.toml` & `SPyOD-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SPyOD"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Grigorios Hatzissawidis", email="grigorios.hatzissawidis@fst.tu-darmstadt.de" },
   { name="Moritz Sieber", email="moritz.sieber@tu-berlin.de" },
 ]
 description = "Spectral Proper Orthogonal Decomposition"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `SPyOD-0.1.5/src/SPyOD.egg-info/PKG-INFO` & `SPyOD-0.1.6/src/SPyOD.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPyOD
-Version: 0.1.5
+Version: 0.1.6
 Summary: Spectral Proper Orthogonal Decomposition
 Author-email: Grigorios Hatzissawidis <grigorios.hatzissawidis@fst.tu-darmstadt.de>, Moritz Sieber <moritz.sieber@tu-berlin.de>
 Project-URL: Homepage, https://github.com/grigorishat/SPyOD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: SPyOD Version: 0.1.5 Summary: Spectral Proper
+Metadata-Version: 2.1 Name: SPyOD Version: 0.1.6 Summary: Spectral Proper
 Orthogonal Decomposition Author-email: Grigorios Hatzissawidis
 hatzissawidis@fst.tu-darmstadt.de>, Moritz Sieber
 sieber@tu-berlin.de> Project-URL: Homepage, https://github.com/grigorishat/
 SPyOD Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE # Spectral Proper Orthogonal Decomposition ## Table of contents *
```

### Comparing `SPyOD-0.1.5/src/spyod/findpairs.py` & `SPyOD-0.1.6/src/spyod/findpairs.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,16 +26,16 @@
         mode['a']:   Analytic mode coefficient a[:,i] + 1j*a[:,i]
         mode['at']:  Derivative of analytic mode coefficient
         mode['K']:   Relative energy content of a single mode pair
         mode['f']:   Estimated frequency of the mode pair [1/sample]
     """
     Nsnap, Npod = np.shape(a)
     # relative energy content, without the part which is cut off 
-    lmbd = np.diag(np.dot(a.transpose(),a))
-    lmbd = lmbd/np.sum(lmbd)
+    lmbd = np.diag(np.dot(a.transpose(), a))
+    lmbd = lmbd / np.sum(lmbd)
 
     ag = np.gradient(a) # gradient
     ag = ag[0]
     # find combined modes from DMD
 
     T = np.linalg.lstsq(a[:Nsnap-1],a[1:Nsnap],rcond=-1)[0].conj().T
 
@@ -49,19 +49,27 @@
     # linked modes are only phase shifted -> correlate real and imaginary part
     # of DMD eigenvectors
     C = np.imag(V @ np.diag(np.sign(omega)) @ V.conj().T)/2
 
     # problem in relative mode energy: last mode is the first, so change
     Nmode = np.trunc(Npod/2)
     Nmode = Nmode.astype(int)
+
+    precision = a.dtype
+    if precision == np.float32:
+        precision_comp = np.complex64
+    elif precision == np.float64:
+        precision_comp = np.complex128
+    else:
+        precision_comp = np.complex128
     
-    mode = {'c' : np.zeros(Nmode),'ind' : np.zeros((Nmode,2)),
-            'a' : np.zeros((Nmode, Nsnap), dtype=complex),
-            'at': np.zeros((Nmode, Nsnap), dtype=complex),
-            'K' : np.zeros(Nmode),'f' : np.zeros(Nmode)}
+    mode = {'c' : np.zeros(Nmode, dtype=precision),'ind' : np.zeros((Nmode,2), dtype=int),
+            'a' : np.zeros((Nmode, Nsnap), dtype=precision_comp),
+            'at': np.zeros((Nmode, Nsnap), dtype=precision_comp),
+            'K' : np.zeros(Nmode, dtype=precision),'f' : np.zeros(Nmode, dtype=precision)}
 
     for i in range(Nmode):
         #pick maximum
         tmp = np.max(C)
         mode['c'][i] = tmp
         indij = np.unravel_index(np.argmax(C, axis=None),C.shape)
         # delete rows and column
```

### Comparing `SPyOD-0.1.5/src/spyod/spod.py` & `SPyOD-0.1.6/src/spyod/spod.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,28 +82,28 @@
                     np.diag(transpose(a)*a)/Nsnap = lambda.
     mode_norm:      Norm of the single spatial modes. 1D array of length Npod. For
                     classical POD (Nfilt=0) the norm is 1 for all modes.
                     sqrt(<Ui,Ui>_w + <Vi,Vi>_w + <Wi,Wi>_w + ...) = mode_norm.
     """
     t = time.time()
     # parse input arguments
-    Nsnap, Ncomp, Ngrid, Nfilt, Npod, input_size, Wxyz, boundary, corr_type, f = parse_input(args, kwargs)
+    Nsnap, Ncomp, Ngrid, Nfilt, Npod, input_size, Wxyz, boundary, corr_type, f, precision = parse_input(args, kwargs)
 
     if Ncomp == 1:
         print("There is {} input component.".format(Ncomp)) #pylint: disable=consider-using-f-string
     elif Ncomp > 1:
         print("There are {} input components.".format(Ncomp)) #pylint: disable=consider-using-f-string
 
     if corr_type == 'temporal':
 
     # calculate temporal correlation matrix
-        R = np.zeros((Nsnap, Nsnap))
+        R = np.zeros((Nsnap, Nsnap), dtype=precision)
 
-        for ii in range(Ncomp):
-            U = np.transpose(args[ii]).reshape((Ngrid, Nsnap))
+        for i in range(Ncomp):
+            U = np.transpose(args[i]).reshape((Ngrid, Nsnap))
             R = R + U.transpose() * Wxyz @ U
         R = R / Nsnap / np.sum(Wxyz)
 
         # calculate filtered correlation matrix S
 
         if boundary == "periodic":
             # convolve periodically extended matrix with filtered diagonal matrix
@@ -113,16 +113,16 @@
             #S = convolve2d(R[np.ix_(ind, ind)], np.diag(f), mode = "valid")
             S = fftconvolve(R[np.ix_(ind, ind)], np.diag(f), mode = "valid")
 
 
         # dft case
         elif boundary == "DFTcase":
             rr = np.zeros(Nsnap)
-            for ii in range(Nsnap):
-                rr[ii] = np.sum(np.diag(R, ii)) * f[0]
+            for i in range(Nsnap):
+                rr[i] = np.sum(np.diag(R, i)) * f[0]
 
             # periodic boundary condition -> circulant matrix
             rr[1:] = rr[1:] + rr[:0:-1]
             S = toeplitz(rr)
 
         # convolve zero padded matrix with filter diagonal matrix
         # ("center" differs from matlab if number of rows/ columns is odd)
@@ -157,43 +157,43 @@
         # since correlation matrix is positive-definite or positive-semidefinite when mean flow field is subtracted
         Nrank = len(lmbd[lmbd > 0])
         if any(lmbd < 0) and Npod > Nrank:
             Npod = Nrank
             print('SPODrankDeficit: Correlation matrix rank is less than number of request POD modes. Npod is set to Nrank. Npod = '+ str(Nrank))
 
 # compute scaled temporal coefficients
-        a = np.multiply(v[:,:Npod],np.sqrt(Nsnap*lmbd[:Npod]))
+        a = np.multiply(v[:, :Npod],np.sqrt(Nsnap * lmbd[:Npod]))
 
 # calculate spatial modes for all components
-        a_proj = np.divide(v[:,:Npod],np.sqrt(Nsnap*lmbd[:Npod]))
+        a_proj = np.divide(v[:, :Npod],np.sqrt(Nsnap * lmbd[:Npod]))
         output_size = list(input_size)
         output_size[0] = Npod
-        mode_norm = np.zeros(Npod)
+        mode_norm = np.zeros(Npod, dtype=precision)
         Ui = list()
 
         for i in range(Ncomp):
 
-            U = np.transpose(args[i]).reshape((Ngrid,Nsnap))
+            U = np.transpose(args[i]).reshape((Ngrid, Nsnap))
             #Ui.append(np.dreshape(np.dot(U,a_proj),output_size))
             #Ui_vec = np.dot(U,a_proj)
-            mode_norm = mode_norm + np.sum(np.dot(U,a_proj).T**2 * Wxyz,axis=1)/np.sum(Wxyz)
+            mode_norm = mode_norm + np.sum(np.dot(U, a_proj).T**2 * Wxyz, axis=1) / np.sum(Wxyz)
             Ui.append(np.dot(U,a_proj).T.reshape(output_size, order = 'F'))
 
     if corr_type == "spatial":
         Nfilt2 = f.size
-        Ncorr = Ngrid*Nfilt2*Ncomp
-        R = np.zeros((Ngrid,Nfilt2,Ncomp,Ngrid,Nfilt2,Ncomp))
+        Ncorr = Ngrid * Nfilt2 * Ncomp
+        R = np.zeros((Ngrid, Nfilt2, Ncomp, Ngrid, Nfilt2, Ncomp))
 
         # first loop over input component
         for k in range(Ncomp):
-            Uk = np.transpose(args[k]).reshape((Ngrid,Nsnap))* np.sqrt(Wxyz)[:,None]
+            Uk = np.transpose(args[k]).reshape((Ngrid, Nsnap))* np.sqrt(Wxyz)[:,None]
 
             # second loop over input component
             for l in range(Ncomp):
-                Ul = np.transpose(args[l]).reshape((Ngrid,Nsnap))* np.sqrt(Wxyz)[:,None]
+                Ul = np.transpose(args[l]).reshape((Ngrid, Nsnap))* np.sqrt(Wxyz)[:,None]
 
                 # first loop over filter coefficient
                 for i in range(-Nfilt, Nfilt + 1, 1):
                     for j in range(-Nfilt, Nfilt + 1, 1):
                         indi = i + Nfilt
                         indj = j + Nfilt
                         ij_shift = i-j
@@ -231,26 +231,26 @@
         if any(lmbd < 0) and Npod > Nrank:
             Npod = Nrank
             print('SPODrankDeficit: Correlation matrix rank is less than number of request POD modes. Npod is set to Nrank. Npod = '+ str(Nrank))
 
         # compute scaled temporal coefficients
         output_size = np.array(input_size)
         output_size[0] = Npod
-        a = np.zeros((Nsnap,Npod),dtype = 'complex_')
-        mode_norm = np.zeros((1,Npod))
+        a = np.zeros((Nsnap, Npod),dtype = 'complex_')
+        mode_norm = np.zeros((1, Npod), dtype=precision)
         Nconvfilt = Ngrid * Nfilt2
         Ui = list()
         for j in range(Ncomp):
-            U = np.transpose(args[j]).reshape((Ngrid,Nsnap))
+            U = np.transpose(args[j]).reshape((Ngrid, Nsnap))
             if boundary == "periodic":
                 # create periodically extended time series
-                Uext = np.concatenate((U[:,-Nfilt:], U, U[:,0:Nfilt]),1)
+                Uext = np.concatenate((U[:,-Nfilt:], U, U[:,0:Nfilt]), 1)
             else: 
                 # create zero padded time series
-                Uext = np.concatenate((np.zeros((Ngrid,Nfilt)),U,np.zeros((Ngrid,Nfilt))),1)
+                Uext = np.concatenate((np.zeros((Ngrid,Nfilt)), U, np.zeros((Ngrid, Nfilt))), 1)
 
             idx = j * Nconvfilt + range(Nconvfilt) 
 
             for i in range(Npod):
                 # pick apropriate spatial mode
                 f_proj = v[idx,i].reshape(Ngrid,Nfilt2, order = 'F')
                 # apply spatial weihting
@@ -266,35 +266,47 @@
             idx = j * Nconvfilt + Nfilt * Ngrid + range(Ngrid)
             scale = np.sqrt(np.sum(Wxyz)/ f[Nfilt+1]/ Wxyz)
             scale[Wxyz==0] = 1 # avoid singularities
             Ui_vec = v[idx,:Npod] * scale[:,None]
             mode_norm = mode_norm + np.sum(Ui_vec**2 * Wxyz[:,None])/np.sum(Wxyz)
             Ui.append(Ui_vec.T.reshape(output_size, order = 'F'))
 
-    print("Elapsed: %.2f min" %(np.double((time.time() - t))/60)) #pylint: disable=consider-using-f-string
+    print("Elapsed: %.2f min" %(np.double((time.time() - t)) / 60)) #pylint: disable=consider-using-f-string
 
     return lmbd, a, mode_norm, Ui
 
-def parse_input(in_data,in_set):
+def parse_input(in_data, in_set):
     """
     this function checks the data for validity
 
     inputs: in_data is a non-keyworded variable-length argument list of the data to be analysed
             in_set is a keyworded, variable-length argument list of the SPOD settings
 
     output: Nsnap, Ncomp, Ngrid, Nfilt, Npod, input_size, Wxyz, boundary, corr_type, f
     """
+
+    if 'precision' in in_set:
+        if in_set.get('precision') == 'double':
+            precision = np.float64
+        elif in_set.get('precision') == 'single':
+            precision = np.float32
+        else:
+            print('Invalid input for precision. Precision must be "single" or "double". Set to "double".')
+            precision = np.float64
+    else: 
+        precision = np.float64
+
     Ncomp = len(in_data)
     assert not Ncomp < 1, 'Input components U,V,W,.. are missing.'
 
     # determine size of input data
-    for ii in range(Ncomp):
-        U = in_data[ii]
+    for i in range(Ncomp):
+        U = in_data[i]
 
-        if ii == 0:
+        if i == 0:
             input_size = U.shape
             Nsnap = input_size[0]
         else:
             if U.shape[0] != Nsnap:
                 raise Exception('Number of snapshots in additional component is not consistent with first component.')
     Ngrid = np.prod(input_size[1:])
 
@@ -337,15 +349,15 @@
     if 'Wxyz' in in_set:
         if in_set.get('Wxyz').size == Ngrid:
             Wxyz = in_set.get('Wxyz')
             Wxyz = np.concatenate(Wxyz.transpose())
         else:
             raise Exception('dimension of weighting does not match the input data.')
     else:
-        Wxyz = np.ones(Ngrid)
+        Wxyz = np.ones(Ngrid, dtype=precision)
 
 
     if 'boundary' in in_set:
         if in_set.get('boundary') == "zeros" or in_set.get('boundary') == "periodic":
             boundary = in_set.get('boundary')
 
         else:
@@ -361,46 +373,46 @@
             raise Exception('correlation type must be temporal or spatial.')  
     else:
         corr_type = 'temporal'
 
     # define filter
     if Nfilt == Nsnap and corr_type == 'temporal':
     # choose box filter to obtain DFT
-        f = filter_coefficient(Nfilt, 'box')
+        f = filter_coefficient(Nfilt, 'box', precision)
         boundary = "DFTcase"
     else:
-        f = filter_coefficient(Nfilt, 'gauss')
+        f = filter_coefficient(Nfilt, 'gauss', precision)
 
 
 
     # check problem size and display appropriate warning
     if corr_type == 'temporal':
         Ncorr = Nsnap
     else: # spatial
-        Ncorr = Ngrid*len(f)
+        Ncorr = Ngrid * len(f)
     if Ncorr > 10000:
         warnings.warn('SPOD:LargeProblem computation takes long time >1 hour')
     elif Ncorr > 2000:
         warnings.warn('SPOD:LargeProblem computation takes some time >1 min')
     elif Ncorr > 1000:
         warnings.warn('SPOD:LargeProblem computation may take some time')
 
-    #print(Nsnap, Ncomp, Ngrid, Nfilt, Npod, input_size, Wxyz, boundary, corr_type, f)
+
     print('Input parameter checked.')
-    return Nsnap, Ncomp, Ngrid, Nfilt, Npod, input_size, Wxyz, boundary, corr_type, f
+    return Nsnap, Ncomp, Ngrid, Nfilt, Npod, input_size, Wxyz, boundary, corr_type, f, precision
 
 
-def filter_coefficient(N_filt, filt_type):
+def filter_coefficient(N_filt, filt_type, precision):
     """
     calculates the filter coefficient for a box or a gaussian filter
 
     input: filter size N_filt and filt_type
     output: filter coefficient f
     """
     if filt_type == 'box':
-        f = np.ones(N_filt)
+        f = np.ones(N_filt, dtype=precision)
     elif filt_type == 'gauss':
-        f = np.exp(-np.linspace(-2.285,2.285,2*N_filt+1)**2)
+        f = np.exp(-np.linspace(-2.285, 2.285, 2 * N_filt + 1)**2, dtype=precision)
     else:
         raise Exception('unknown filter type.')
-    f = f/np.sum(f)
+    f = f / np.sum(f)
     return f
```

