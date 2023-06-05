# Comparing `tmp/ipdw-1.0.0.tar.gz` & `tmp/ipdw-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipdw-1.0.0.tar", last modified: Wed May 31 23:10:05 2023, max compression
+gzip compressed data, was "ipdw-1.0.1.tar", last modified: Mon Jun  5 22:46:21 2023, max compression
```

## Comparing `ipdw-1.0.0.tar` & `ipdw-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:10:05.826115 ipdw-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-31 23:09:54.000000 ipdw-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-05-31 23:10:05.826115 ipdw-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-05-31 23:09:54.000000 ipdw-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:10:05.826115 ipdw-1.0.0/ipdw/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-31 23:09:54.000000 ipdw-1.0.0/ipdw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18179 2023-05-31 23:09:54.000000 ipdw-1.0.0/ipdw/interpolate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:10:05.826115 ipdw-1.0.0/ipdw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-05-31 23:10:05.000000 ipdw-1.0.0/ipdw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-31 23:10:05.000000 ipdw-1.0.0/ipdw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 23:10:05.000000 ipdw-1.0.0/ipdw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-31 23:10:05.000000 ipdw-1.0.0/ipdw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-31 23:10:05.000000 ipdw-1.0.0/ipdw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 23:10:05.826115 ipdw-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-31 23:09:54.000000 ipdw-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:10:05.826115 ipdw-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-31 23:09:54.000000 ipdw-1.0.0/tests/test_interpolate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:46:21.170766 ipdw-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-05 22:46:11.000000 ipdw-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-06-05 22:46:21.170766 ipdw-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-06-05 22:46:11.000000 ipdw-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:46:21.166766 ipdw-1.0.1/ipdw/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-05 22:46:11.000000 ipdw-1.0.1/ipdw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19022 2023-06-05 22:46:11.000000 ipdw-1.0.1/ipdw/interpolate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:46:21.170766 ipdw-1.0.1/ipdw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-06-05 22:46:21.000000 ipdw-1.0.1/ipdw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-05 22:46:21.000000 ipdw-1.0.1/ipdw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 22:46:21.000000 ipdw-1.0.1/ipdw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-05 22:46:21.000000 ipdw-1.0.1/ipdw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-05 22:46:21.000000 ipdw-1.0.1/ipdw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 22:46:21.170766 ipdw-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-05 22:46:11.000000 ipdw-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:46:21.170766 ipdw-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-05 22:46:11.000000 ipdw-1.0.1/tests/test_interpolate.py
```

### Comparing `ipdw-1.0.0/LICENSE` & `ipdw-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ipdw-1.0.0/PKG-INFO` & `ipdw-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 Metadata-Version: 2.1
 Name: ipdw
-Version: 1.0.0
+Version: 1.0.1
 Summary: Inverse-Path-Distance-Weighted Interpolation for Python
 Home-page: https://github.com/wrightky/ipdw
 Author: Kyle Wright
 Author-email: Kyle.Wright@twdb.texas.gov
 License: MIT
 Keywords: interpolation ipdw idw
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: GIS
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![codecov](https://codecov.io/gh/wrightky/ipdw/branch/main/graph/badge.svg?token=KQTT88DN6E)](https://codecov.io/gh/wrightky/ipdw)
+[![PyPi](https://img.shields.io/pypi/v/ipdw)](https://pypi.org/project/ipdw/)
+[![Python Version](https://img.shields.io/pypi/pyversions/ipdw)](https://pypi.org/project/ipdw/)
+[![Downloads](https://img.shields.io/pypi/dm/ipdw)](https://pypi.org/project/ipdw)
 # Inverse Path-Distance Weighted Interpolation
 
 `ipdw` is a Python package for performing [inverse-distance-weighted interpolation](https://en.wikipedia.org/wiki/Inverse_distance_weighting) using **path distances** instead of Euclidean distances. In other words, interpolation weights account for domain geometry and obstacles, which is often preferred in geophysical contexts in which "in water" distances are often more relevant to the process at hand than Euclidean distances. For example, this package allows you to quickly and easily interpolate inside a water body, accounting for complex coastlines, islands, and other barriers.
 
 This package is inspired by [Stachelek & Madden (2015)](doi.org/10.1080/13658816.2015.1018833) and is a Python alternative to the original `R` package [`ipdw`](https://github.com/jsta/ipdw), although likely using different methodology under the hood. We rely heavily on the fast-marching approach of [`scikit-fmm`](https://github.com/scikit-fmm/scikit-fmm) to compute path distances, and rely exclusively on `matplotlib.path` and `numpy` to make sense of domain geometry information, which can be specified in either raster or vector format. _No geospatial packages are required._ Due to the use of fast-marching, vectorization, and a reliance on more efficient packages for the compututationally-expensive steps, this package should be quite fast and computationally efficient relative to the complexity of the underlying algorithm.
 
 ## Installation
 
-Install the latest stable release from PyPi with pip:
+Install the latest stable release from [PyPi](https://pypi.org/project/ipdw/) with pip:
 ```
 pip install ipdw
 ```
 If you want to install from source, clone this repository, navigate to the new directory, and run `python setup.py`.
 
 **Requirements**: `numpy`, `matplotlib`, and `scikit-fmm`
 
@@ -88,13 +94,13 @@
 ```
 in which `output` is an array with interpolated values in all viable cells, and `NaN` everywhere else. That's it! 
 Also, note that there exists another function, `Gridded.reinterpolate`, which can be used to perform additional interpolations using new `input_values` from the same locations (and with the same parameter settings), which is faster than re-running `interpolate`.
 
 A few example interpolation outputs using different parameter choices are shown below.
 
 <div class="nav3" style="width:800px;">
-    <img src="example.jpeg" alt="Example" width="100%"></a>
+    <img src="https://raw.githubusercontent.com/wrightky/ipdw/main/example.jpeg" alt="Image" width="100%"></a>
 </div>
 
 ## Contributing
 
 Please feel free to open an issue or a pull request!
```

### Comparing `ipdw-1.0.0/README.md` & `ipdw-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+[![codecov](https://codecov.io/gh/wrightky/ipdw/branch/main/graph/badge.svg?token=KQTT88DN6E)](https://codecov.io/gh/wrightky/ipdw)
+[![PyPi](https://img.shields.io/pypi/v/ipdw)](https://pypi.org/project/ipdw/)
+[![Python Version](https://img.shields.io/pypi/pyversions/ipdw)](https://pypi.org/project/ipdw/)
+[![Downloads](https://img.shields.io/pypi/dm/ipdw)](https://pypi.org/project/ipdw)
 # Inverse Path-Distance Weighted Interpolation
 
 `ipdw` is a Python package for performing [inverse-distance-weighted interpolation](https://en.wikipedia.org/wiki/Inverse_distance_weighting) using **path distances** instead of Euclidean distances. In other words, interpolation weights account for domain geometry and obstacles, which is often preferred in geophysical contexts in which "in water" distances are often more relevant to the process at hand than Euclidean distances. For example, this package allows you to quickly and easily interpolate inside a water body, accounting for complex coastlines, islands, and other barriers.
 
 This package is inspired by [Stachelek & Madden (2015)](doi.org/10.1080/13658816.2015.1018833) and is a Python alternative to the original `R` package [`ipdw`](https://github.com/jsta/ipdw), although likely using different methodology under the hood. We rely heavily on the fast-marching approach of [`scikit-fmm`](https://github.com/scikit-fmm/scikit-fmm) to compute path distances, and rely exclusively on `matplotlib.path` and `numpy` to make sense of domain geometry information, which can be specified in either raster or vector format. _No geospatial packages are required._ Due to the use of fast-marching, vectorization, and a reliance on more efficient packages for the compututationally-expensive steps, this package should be quite fast and computationally efficient relative to the complexity of the underlying algorithm.
 
 ## Installation
 
-Install the latest stable release from PyPi with pip:
+Install the latest stable release from [PyPi](https://pypi.org/project/ipdw/) with pip:
 ```
 pip install ipdw
 ```
 If you want to install from source, clone this repository, navigate to the new directory, and run `python setup.py`.
 
 **Requirements**: `numpy`, `matplotlib`, and `scikit-fmm`
 
@@ -71,13 +75,13 @@
 ```
 in which `output` is an array with interpolated values in all viable cells, and `NaN` everywhere else. That's it! 
 Also, note that there exists another function, `Gridded.reinterpolate`, which can be used to perform additional interpolations using new `input_values` from the same locations (and with the same parameter settings), which is faster than re-running `interpolate`.
 
 A few example interpolation outputs using different parameter choices are shown below.
 
 <div class="nav3" style="width:800px;">
-    <img src="example.jpeg" alt="Example" width="100%"></a>
+    <img src="https://raw.githubusercontent.com/wrightky/ipdw/main/example.jpeg" alt="Image" width="100%"></a>
 </div>
 
 ## Contributing
 
 Please feel free to open an issue or a pull request!
```

### Comparing `ipdw-1.0.0/ipdw/interpolate.py` & `ipdw-1.0.1/ipdw/interpolate.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,16 +193,24 @@
             extent[0]+0.5*self.cellsize,
             extent[1]-0.5*self.cellsize,
             extent[2]+0.5*self.cellsize,
             extent[3]-0.5*self.cellsize,
         ]
         return
 
-    def interpolate(self, input_locations, input_values, n_nearest=3,
-                    power=1, offsets=None, buffer=0, regularization=1e-8):
+    def interpolate(self,
+                    input_locations,
+                    input_values,
+                    n_nearest=3,
+                    power=1,
+                    offsets=None,
+                    buffer=0,
+                    regularization=1e-8,
+                    allow_outside=False
+                    ):
         """
         Method performs inverse-path-distance-weighted interpolation from
         input data locations onto target raster, using the number of neighbor
         points specified in the function call.
         
         This function relies heavily on scikit-fmm to compute geodesic
         distances within the domain topology. The speed of this function is
@@ -238,14 +246,18 @@
                 enclosed domain (or it will return a ValueError), so
                 increasing the buffer by a few cells can be helpful if any
                 inputs are very close to a boundary/hole. Applied uniformly to
                 all locations, so does not affect weighting.
             regularization (float, default=1e-8) : Very small regularization
                 parameter used to avoid dividing by zero when computing
                 the inverse of distance.
+            allow_outside (bool, default=False) : If any "input_locations"
+                are not within the interpolation domain, this boolean flag
+                controls whether to raise an error or simply ignore that
+                location during interpolation.
         **Outputs**
             output (array) : Raster of interpolated values.
         """
         # Do some type checks on input values
         self.n_nearest = int(n_nearest)
         self.power = float(power)
         self.regularization = regularization
@@ -280,17 +292,27 @@
                 phi[iy-buffer:iy+buffer,ix-buffer:ix+buffer] = 1
             else:
                 phi[iy,ix] = 1
             try:
                 # Actually compute distances
                 dist = np.abs(skfmm.distance(phi)*self.cellsize) + offsets[n]
             except ValueError:
-                raise ValueError("One or more locations are not within the "+\
-                                 "enclosed boundary. Check locations or try "+\
-                                 "increasing the buffer size")
+                if not allow_outside:
+                    raise ValueError(
+                        "One or more locations are not within the "+\
+                        "interpolation domain. Check locations, try "+\
+                        "increasing the buffer, or set allow_outside=True"
+                    )
+                else:
+                    print(
+                        "Warning: Input location %s" % input_locations[n,:]+\
+                        " not found within interpolation domain. " +\
+                        "Skipping this location."
+                    )
+                    continue
             dist[mask] = np.nan # Mask out locations outside domain
             self.dist_from_each[:,:,n] = dist # Store result
 
         # For each cell, find indices of N nearest input locations
         self.arg_n_min = np.argsort(self.dist_from_each)[:,:,:n_nearest]
 
         # Perform inverse-path-distance-weighted interpolation
```

### Comparing `ipdw-1.0.0/ipdw.egg-info/PKG-INFO` & `ipdw-1.0.1/ipdw.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 Metadata-Version: 2.1
 Name: ipdw
-Version: 1.0.0
+Version: 1.0.1
 Summary: Inverse-Path-Distance-Weighted Interpolation for Python
 Home-page: https://github.com/wrightky/ipdw
 Author: Kyle Wright
 Author-email: Kyle.Wright@twdb.texas.gov
 License: MIT
 Keywords: interpolation ipdw idw
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: GIS
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![codecov](https://codecov.io/gh/wrightky/ipdw/branch/main/graph/badge.svg?token=KQTT88DN6E)](https://codecov.io/gh/wrightky/ipdw)
+[![PyPi](https://img.shields.io/pypi/v/ipdw)](https://pypi.org/project/ipdw/)
+[![Python Version](https://img.shields.io/pypi/pyversions/ipdw)](https://pypi.org/project/ipdw/)
+[![Downloads](https://img.shields.io/pypi/dm/ipdw)](https://pypi.org/project/ipdw)
 # Inverse Path-Distance Weighted Interpolation
 
 `ipdw` is a Python package for performing [inverse-distance-weighted interpolation](https://en.wikipedia.org/wiki/Inverse_distance_weighting) using **path distances** instead of Euclidean distances. In other words, interpolation weights account for domain geometry and obstacles, which is often preferred in geophysical contexts in which "in water" distances are often more relevant to the process at hand than Euclidean distances. For example, this package allows you to quickly and easily interpolate inside a water body, accounting for complex coastlines, islands, and other barriers.
 
 This package is inspired by [Stachelek & Madden (2015)](doi.org/10.1080/13658816.2015.1018833) and is a Python alternative to the original `R` package [`ipdw`](https://github.com/jsta/ipdw), although likely using different methodology under the hood. We rely heavily on the fast-marching approach of [`scikit-fmm`](https://github.com/scikit-fmm/scikit-fmm) to compute path distances, and rely exclusively on `matplotlib.path` and `numpy` to make sense of domain geometry information, which can be specified in either raster or vector format. _No geospatial packages are required._ Due to the use of fast-marching, vectorization, and a reliance on more efficient packages for the compututationally-expensive steps, this package should be quite fast and computationally efficient relative to the complexity of the underlying algorithm.
 
 ## Installation
 
-Install the latest stable release from PyPi with pip:
+Install the latest stable release from [PyPi](https://pypi.org/project/ipdw/) with pip:
 ```
 pip install ipdw
 ```
 If you want to install from source, clone this repository, navigate to the new directory, and run `python setup.py`.
 
 **Requirements**: `numpy`, `matplotlib`, and `scikit-fmm`
 
@@ -88,13 +94,13 @@
 ```
 in which `output` is an array with interpolated values in all viable cells, and `NaN` everywhere else. That's it! 
 Also, note that there exists another function, `Gridded.reinterpolate`, which can be used to perform additional interpolations using new `input_values` from the same locations (and with the same parameter settings), which is faster than re-running `interpolate`.
 
 A few example interpolation outputs using different parameter choices are shown below.
 
 <div class="nav3" style="width:800px;">
-    <img src="example.jpeg" alt="Example" width="100%"></a>
+    <img src="https://raw.githubusercontent.com/wrightky/ipdw/main/example.jpeg" alt="Image" width="100%"></a>
 </div>
 
 ## Contributing
 
 Please feel free to open an issue or a pull request!
```

### Comparing `ipdw-1.0.0/setup.py` & `ipdw-1.0.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name = 'ipdw',
-    version = '1.0.0',
+    version = '1.0.1',
     license = 'MIT',
     description = 'Inverse-Path-Distance-Weighted Interpolation for Python',
     long_description=LONG_DESCRIPTION,
     long_description_content_type = 'text/markdown',
     author = 'Kyle Wright',
     author_email = 'Kyle.Wright@twdb.texas.gov',
     url = 'https://github.com/wrightky/ipdw',
     packages = find_packages(),
     keywords='interpolation ipdw idw',
     classifiers = [
         'Programming Language :: Python',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Topic :: Scientific/Engineering :: GIS'
     ],
     install_requires = ['numpy','matplotlib','scikit-fmm'],
 )
```

### Comparing `ipdw-1.0.0/tests/test_interpolate.py` & `ipdw-1.0.1/tests/test_interpolate.py`

 * *Files identical despite different names*

