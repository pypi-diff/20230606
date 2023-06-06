# Comparing `tmp/PyMoosh-2.61.tar.gz` & `tmp/PyMoosh-2.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyMoosh-2.61.tar", last modified: Tue Jun  6 08:01:36 2023, max compression
+gzip compressed data, was "dist/PyMoosh-2.62.tar", last modified: Tue Jun  6 08:58:39 2023, max compression
```

## Comparing `PyMoosh-2.61.tar` & `PyMoosh-2.62.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 moi       (1001) moi       (1001)        0 2023-06-06 08:01:36.000000 PyMoosh-2.61/
--rw-rw-r--   0 moi       (1001) moi       (1001)     3350 2023-06-06 08:01:36.000000 PyMoosh-2.61/PKG-INFO
-drwxrwxr-x   0 moi       (1001) moi       (1001)        0 2023-06-06 08:01:36.000000 PyMoosh-2.61/PyMoosh/
-drwxrwxr-x   0 moi       (1001) moi       (1001)        0 2023-06-06 08:01:36.000000 PyMoosh-2.61/PyMoosh/data/
--rw-rw-r--   0 moi       (1001) moi       (1001)    80345 2023-02-15 07:39:17.000000 PyMoosh-2.61/PyMoosh/data/solar.json
--rw-rw-r--   0 moi       (1001) moi       (1001)    11075 2023-02-15 07:39:17.000000 PyMoosh-2.61/PyMoosh/data/material_data.json
--rw-rw-r--   0 moi       (1001) moi       (1001)     1274 2023-06-06 08:00:56.000000 PyMoosh-2.61/PyMoosh/__init__.py
--rw-rw-r--   0 moi       (1001) moi       (1001)   189816 2023-06-06 07:59:22.000000 PyMoosh-2.61/PyMoosh/core.py
--rw-rw-r--   0 moi       (1001) moi       (1001)     4571 2023-06-05 14:15:08.000000 PyMoosh-2.61/PyMoosh/optim_algo.py
--rw-rw-r--   0 moi       (1001) moi       (1001)     4373 2023-04-06 22:06:11.000000 PyMoosh-2.61/PyMoosh/materials.py
--rw-rw-r--   0 moi       (1001) moi       (1001)    34502 2022-09-23 09:03:42.000000 PyMoosh-2.61/LICENSE.txt
-drwxrwxr-x   0 moi       (1001) moi       (1001)        0 2023-06-06 08:01:36.000000 PyMoosh-2.61/PyMoosh.egg-info/
--rw-rw-r--   0 moi       (1001) moi       (1001)     3350 2023-06-06 08:01:36.000000 PyMoosh-2.61/PyMoosh.egg-info/PKG-INFO
--rw-rw-r--   0 moi       (1001) moi       (1001)      425 2023-06-06 08:01:36.000000 PyMoosh-2.61/PyMoosh.egg-info/SOURCES.txt
--rw-rw-r--   0 moi       (1001) moi       (1001)        8 2023-06-06 08:01:36.000000 PyMoosh-2.61/PyMoosh.egg-info/top_level.txt
--rw-rw-r--   0 moi       (1001) moi       (1001)       23 2023-06-06 08:01:36.000000 PyMoosh-2.61/PyMoosh.egg-info/requires.txt
--rw-rw-r--   0 moi       (1001) moi       (1001)        1 2023-06-06 08:01:36.000000 PyMoosh-2.61/PyMoosh.egg-info/dependency_links.txt
--rw-rw-r--   0 moi       (1001) moi       (1001)      319 2023-02-15 08:19:19.000000 PyMoosh-2.61/PyMoosh.egg-info/SOURCES (SFConflict antoine.moreau@uca.fr 2023-05-29-10-11-16).txt
--rw-rw-r--   0 moi       (1001) moi       (1001)     2282 2023-02-15 07:39:17.000000 PyMoosh-2.61/setup.py
--rw-rw-r--   0 moi       (1001) moi       (1001)       34 2023-02-15 07:39:17.000000 PyMoosh-2.61/MANIFEST.in
--rw-rw-r--   0 moi       (1001) moi       (1001)      107 2023-06-06 08:01:36.000000 PyMoosh-2.61/setup.cfg
--rw-rw-r--   0 moi       (1001) moi       (1001)     2565 2023-02-15 07:39:17.000000 PyMoosh-2.61/README.md
+drwxrwxr-x   0 moi       (1001) moi       (1001)        0 2023-06-06 08:58:39.000000 PyMoosh-2.62/
+-rw-rw-r--   0 moi       (1001) moi       (1001)     3350 2023-06-06 08:58:39.000000 PyMoosh-2.62/PKG-INFO
+drwxrwxr-x   0 moi       (1001) moi       (1001)        0 2023-06-06 08:58:39.000000 PyMoosh-2.62/PyMoosh/
+drwxrwxr-x   0 moi       (1001) moi       (1001)        0 2023-06-06 08:58:39.000000 PyMoosh-2.62/PyMoosh/data/
+-rw-rw-r--   0 moi       (1001) moi       (1001)    80345 2023-02-15 07:39:17.000000 PyMoosh-2.62/PyMoosh/data/solar.json
+-rw-rw-r--   0 moi       (1001) moi       (1001)    11075 2023-02-15 07:39:17.000000 PyMoosh-2.62/PyMoosh/data/material_data.json
+-rw-rw-r--   0 moi       (1001) moi       (1001)     1274 2023-06-06 08:58:14.000000 PyMoosh-2.62/PyMoosh/__init__.py
+-rw-rw-r--   0 moi       (1001) moi       (1001)   188199 2023-06-06 08:48:44.000000 PyMoosh-2.62/PyMoosh/core.py
+-rw-rw-r--   0 moi       (1001) moi       (1001)     4571 2023-06-05 14:15:08.000000 PyMoosh-2.62/PyMoosh/optim_algo.py
+-rw-rw-r--   0 moi       (1001) moi       (1001)     4373 2023-04-06 22:06:11.000000 PyMoosh-2.62/PyMoosh/materials.py
+-rw-rw-r--   0 moi       (1001) moi       (1001)    34502 2022-09-23 09:03:42.000000 PyMoosh-2.62/LICENSE.txt
+drwxrwxr-x   0 moi       (1001) moi       (1001)        0 2023-06-06 08:58:39.000000 PyMoosh-2.62/PyMoosh.egg-info/
+-rw-rw-r--   0 moi       (1001) moi       (1001)     3350 2023-06-06 08:58:39.000000 PyMoosh-2.62/PyMoosh.egg-info/PKG-INFO
+-rw-rw-r--   0 moi       (1001) moi       (1001)      425 2023-06-06 08:58:39.000000 PyMoosh-2.62/PyMoosh.egg-info/SOURCES.txt
+-rw-rw-r--   0 moi       (1001) moi       (1001)        8 2023-06-06 08:58:39.000000 PyMoosh-2.62/PyMoosh.egg-info/top_level.txt
+-rw-rw-r--   0 moi       (1001) moi       (1001)       23 2023-06-06 08:58:39.000000 PyMoosh-2.62/PyMoosh.egg-info/requires.txt
+-rw-rw-r--   0 moi       (1001) moi       (1001)        1 2023-06-06 08:58:39.000000 PyMoosh-2.62/PyMoosh.egg-info/dependency_links.txt
+-rw-rw-r--   0 moi       (1001) moi       (1001)      319 2023-02-15 08:19:19.000000 PyMoosh-2.62/PyMoosh.egg-info/SOURCES (SFConflict antoine.moreau@uca.fr 2023-05-29-10-11-16).txt
+-rw-rw-r--   0 moi       (1001) moi       (1001)     2282 2023-02-15 07:39:17.000000 PyMoosh-2.62/setup.py
+-rw-rw-r--   0 moi       (1001) moi       (1001)       34 2023-02-15 07:39:17.000000 PyMoosh-2.62/MANIFEST.in
+-rw-rw-r--   0 moi       (1001) moi       (1001)      107 2023-06-06 08:58:39.000000 PyMoosh-2.62/setup.cfg
+-rw-rw-r--   0 moi       (1001) moi       (1001)     2565 2023-02-15 07:39:17.000000 PyMoosh-2.62/README.md
```

### Comparing `PyMoosh-2.61/PKG-INFO` & `PyMoosh-2.62/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: PyMoosh
-Version: 2.61
+Version: 2.62
 Summary: A scattering matrix formalism to solve Maxwell's equations in a multilayered structure.
 Home-page: https://github.com/AnMoreau/PyMoosh
 Author: Antoine Moreau
 Author-email: antoine.moreau@uca.fr
 License: GPLv3+
 Description: # PyMoosh
```

### Comparing `PyMoosh-2.61/PyMoosh/data/solar.json` & `PyMoosh-2.62/PyMoosh/data/solar.json`

 * *Files identical despite different names*

### Comparing `PyMoosh-2.61/PyMoosh/data/material_data.json` & `PyMoosh-2.62/PyMoosh/data/material_data.json`

 * *Files identical despite different names*

### Comparing `PyMoosh-2.61/PyMoosh/__init__.py` & `PyMoosh-2.62/PyMoosh/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     in a multilayered structure. This makes PyMoosh unconditionally stable,
     allowing to explore even advanced properties of such multilayers,
     find poles and zeros of the scattering matrix (and thus guided modes),
     and many other things...
 
 """
 __name__ = 'PyMoosh'
-__version__ = '2.61'
+__version__ = '2.62'
 __date__ = "06/06/2023"   # MM/DD/YYY
 __author__ = 'Antoine Moreau'
 
 
 ## make accessible everything from `core` directly from the PyMoosh base package
 from PyMoosh.core import *
 from PyMoosh.optim_algo import *
```

### Comparing `PyMoosh-2.61/PyMoosh/core.py` & `PyMoosh-2.62/PyMoosh/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1401,73 +1401,45 @@
         Ampl = np.zeros((2 * g + 2, 2), dtype=complex)
 
 # -----------------------------> Above the source
 # calculation of the scattering matrices above the source (*_up)
         H_up = np.zeros((2*source_interface, 2, 2), dtype=complex)
         A_up = np.zeros((2*source_interface, 2, 2), dtype=complex)
 
-
-
-        # print("------------------  T ------------------------------")
-        # print(T)
-        # print("------------------  T ------------------------------")
-
-
         # T[2*source_interface] should be a neutral matrix for cascading
         # if the two media are the same on each side of the source.
 
         H_up[0] = [[0, 1], [1, 0]]
         A_up[0] = [[0, 1], [1, 0]]
 
         for k in range(2*source_interface-1):
             A_up[k + 1] = cascade(A_up[k], T[k + 1])
             H_up[k + 1] = cascade(T[2*source_interface-1-k], H_up[k])
 
-        # print("A_up")
-        # print(A_up)
-        # print("_________________________")
-        #
-        # print("H_up")
-        # print(H_up)
-        # print("_________________________")
-
         I_up = np.zeros((2*source_interface, 2, 2), dtype=complex)
         for k in range(2*source_interface-1):
             I_up[k] = np.array(
                 [[A_up[k][1, 0], A_up[k][1, 1] * H_up[2*source_interface-1-k][0, 1]],
                  [A_up[k][1, 0] * H_up[2*source_interface-1-k][0, 0],
                   H_up[2*source_interface-1-k][0, 1]]] / (
                         1 - A_up[k][1, 1] * H_up[2*source_interface-1-k][0, 0]))
-            print(k,2*source_interface-1-k)
-        print('//////////////////////////////////// I-up ////////////////////////////')
-        print(I_up)
-        print('//////////////////////////////////// I_up ////////////////////////////')
 
 # ----------------------------> Below the source
 # Calculation of the scattering matrices below the source (*_d)
 
         H_d = np.zeros((-2*source_interface+2*g+2, 2, 2), dtype=complex)
         A_d = np.zeros((-2*source_interface+2*g+2, 2, 2), dtype=complex)
 
         H_d[0] = [[0, 1], [1, 0]]
         A_d[0] = [[0, 1], [1, 0]]
 
         for k in range(2*g+1-2*source_interface):
             A_d[k + 1] = cascade(A_d[k], T[2*source_interface + k + 1])
             H_d[k + 1] = cascade(T[2*g+1-k], H_d[k])
 
-        # print('+++++++++++++++++++ A_d +++++++++++++++++')
-        # print(A_d)
-        # print('+++++++++++++++++++ A_d +++++++++++++++++')
-        #
-        # print('+++++++++++++++++++ H_d +++++++++++++++++')
-        # print(H_d)
-        # print('+++++++++++++++++++ H_d +++++++++++++++++')
-
-
         I_d = np.zeros((-2*source_interface+2*g+2, 2, 2), dtype=complex)
         for k in range(2*g+1-2*source_interface):
             I_d[k] = np.array(
                 [[A_d[k][1, 0], A_d[k][1, 1] * H_d[2*(g-source_interface)+1-k][0, 1]],
                  [A_d[k][1, 0] * H_d[2*(g-source_interface)+1-k][0, 0],
                   H_d[2*(g-source_interface)+1-k][0, 1]]] / (
                         1 - A_d[k][1, 1] * H_d[2*(g-source_interface)+1-k][0, 0]))
@@ -1480,36 +1452,24 @@
         M = ex / (1 - r_up + (1 + r_up) * (1- r_d) / (1 + r_d)) \
         / gamma[source_interface]
         D = ex / (1 - r_d + (1-r_up)/(1 + r_up)*(1 + r_d)) \
         / gamma[source_interface]
 
 # Starting with the intermediary matrices, compute the right coefficients
 
-        # print('//////////////////////////////////// I-up ////////////////////////////')
-        # print(I_up)
-        # print('//////////////////////////////////// I_up ////////////////////////////')
-
-
         Ampl = np.zeros(2*g+2, dtype=complex)
-        # print("Amplitudes up")
         for k in range(source_interface):
-            print(k,"Pff")
-            # Ampl[2*k] = I_up[2*k][1,1] * M
-            # Ampl[2*k+1] = I_up[2*k+1][0,1] * M
             # Celui qui descend.
             Ampl[2*k] = I_up[2*k][0,1] * M
             # Celui qui monte.
             Ampl[2*k+1] = I_up[2*k+1][1,1] * M
-            # print(k,Ampl[2*k]/M,Ampl[2*k+1]/M)
 
-        print("Amplitudes down")
         for k in range(source_interface,g+1):
             Ampl[2*k] = I_d[2*(k-source_interface)][0,0] * D
             Ampl[2*k+1] = I_d[2*(k-source_interface)+1][1,0] * D
-            # print(Ampl[2*k]/D,Ampl[2*k+1]/D)
 
         Ampl[2*source_interface-1] = M
         Ampl[2*source_interface] = D
 
 
 # >>> Calculation of the fields <<<
 
@@ -2037,17 +1997,14 @@
     opp = np.imag(n_s) > 0
     n_s = n_s - 2* n_s * (opp)
 
     n_p = n[Type]**2 / n_s
     delta = 2*np.pi*thickness*n_s/wavelength
     #cos_theta = np.cos(np.arcsin(sin_theta))
     temp = -1.j*np.tan(delta)
-    #print(sin_theta)
-    #print(cos_theta)
-    #print(temp)
 
     if polarization == 0:
         admittance = n_s
     else:
         admittance = n_p
 
     Y = admittance[-1]
@@ -2321,17 +2278,14 @@
         A[0] = np.array([[1, 0],
                          [0, 1]])
         B[0] = np.array([[1, 0],
                          [0, 1]])
         for i in range(1, T.shape[0]+1):
             A[i] =  A[i - 1] @ T[i-1]
             B[i] = T[-i] @ B[i-1]
-        #print(T)
-        #print(A)
-        # reflection coefficient of the whole structure
         r = -A[-1][1,0]/A[-1][0,0]
         # transmission coefficient of the whole structure
         t = A[-1][1,1] - (A[-1][1,0] * A[-1][0,1])/A[-1][0,0]
         # Energy reflexion coefficient;
         R = np.real(abs(r) ** 2)
         # Energy transmission coefficient;
         T = np.real(
@@ -2343,16 +2297,14 @@
         A, B = saved_mat
 
         if (0 < i_change):
             T = np.zeros(((3, 2, 2)), dtype=complex)
 
             sum = gamma[i_change-1]/f[Type[i_change-1]] + gamma[i_change]/f[Type[i_change]]
             dif = gamma[i_change-1]/f[Type[i_change-1]] - gamma[i_change]/f[Type[i_change]]
-            # print("pop", gamma[k], gamma[k+1])
-            # print(sum, dif)
             # Layer transfer matrix
             T[0] = f[Type[i_change]]/(2*gamma[i_change]) * np.array([[sum, -dif],
                                                                      [-dif, sum]])
 
             phase = 1.j* gamma[i_change] * thickness[i_change]
             # Layer propagation matrix
             T[1] = [[np.exp(-phase), 0],
```

### Comparing `PyMoosh-2.61/PyMoosh/optim_algo.py` & `PyMoosh-2.62/PyMoosh/optim_algo.py`

 * *Files identical despite different names*

### Comparing `PyMoosh-2.61/PyMoosh/materials.py` & `PyMoosh-2.62/PyMoosh/materials.py`

 * *Files identical despite different names*

### Comparing `PyMoosh-2.61/LICENSE.txt` & `PyMoosh-2.62/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyMoosh-2.61/PyMoosh.egg-info/PKG-INFO` & `PyMoosh-2.62/PyMoosh.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: PyMoosh
-Version: 2.61
+Version: 2.62
 Summary: A scattering matrix formalism to solve Maxwell's equations in a multilayered structure.
 Home-page: https://github.com/AnMoreau/PyMoosh
 Author: Antoine Moreau
 Author-email: antoine.moreau@uca.fr
 License: GPLv3+
 Description: # PyMoosh
```

### Comparing `PyMoosh-2.61/setup.py` & `PyMoosh-2.62/setup.py`

 * *Files identical despite different names*

### Comparing `PyMoosh-2.61/README.md` & `PyMoosh-2.62/README.md`

 * *Files identical despite different names*

