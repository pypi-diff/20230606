# Comparing `tmp/pycudwt-1.0.1.tar.gz` & `tmp/pycudwt-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycudwt-1.0.1.tar", last modified: Tue Mar 15 10:21:43 2022, max compression
+gzip compressed data, was "pycudwt-1.0.2.tar", last modified: Tue Jun  6 14:26:00 2023, max compression
```

## Comparing `pycudwt-1.0.1.tar` & `pycudwt-1.0.2.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2022-03-15 10:21:43.135565 pycudwt-1.0.1/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1484 2022-03-15 09:45:31.000000 pycudwt-1.0.1/LICENSE
--rw-r--r--   0 pierre    (1000) pierre    (1000)       52 2022-03-15 09:45:43.000000 pycudwt-1.0.1/MANIFEST.in
--rw-r--r--   0 pierre    (1000) pierre    (1000)      327 2022-03-15 10:21:43.135565 pycudwt-1.0.1/PKG-INFO
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1664 2022-03-15 10:19:07.000000 pycudwt-1.0.1/README.md
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2022-03-15 10:21:43.131565 pycudwt-1.0.1/pdwt/
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2022-03-15 10:21:43.131565 pycudwt-1.0.1/pdwt/src/
--rw-r--r--   0 pierre    (1000) pierre    (1000)    20444 2022-03-15 09:45:31.000000 pycudwt-1.0.1/pdwt/src/common.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4048 2022-03-15 09:45:31.000000 pycudwt-1.0.1/pdwt/src/common.h
--rw-r--r--   0 pierre    (1000) pierre    (1000)   136815 2022-03-15 09:45:31.000000 pycudwt-1.0.1/pdwt/src/filters.cpp
--rwxr-xr-x   0 pierre    (1000) pierre    (1000)    10442 2022-03-15 09:45:31.000000 pycudwt-1.0.1/pdwt/src/filters.h
--rw-r--r--   0 pierre    (1000) pierre    (1000)     8758 2022-03-15 09:45:31.000000 pycudwt-1.0.1/pdwt/src/haar.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)      789 2022-03-15 09:45:31.000000 pycudwt-1.0.1/pdwt/src/haar.h
--rw-r--r--   0 pierre    (1000) pierre    (1000)      190 2022-03-15 09:45:31.000000 pycudwt-1.0.1/pdwt/src/io.h
--rw-r--r--   0 pierre    (1000) pierre    (1000)    17734 2022-03-15 09:45:31.000000 pycudwt-1.0.1/pdwt/src/nonseparable.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1261 2022-03-15 09:45:31.000000 pycudwt-1.0.1/pdwt/src/nonseparable.h
--rw-r--r--   0 pierre    (1000) pierre    (1000)    27757 2022-03-15 09:45:31.000000 pycudwt-1.0.1/pdwt/src/separable.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2064 2022-03-15 09:45:31.000000 pycudwt-1.0.1/pdwt/src/separable.h
--rw-r--r--   0 pierre    (1000) pierre    (1000)      487 2022-03-15 09:45:31.000000 pycudwt-1.0.1/pdwt/src/utils.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)      667 2022-03-15 09:45:31.000000 pycudwt-1.0.1/pdwt/src/utils.h
--rwxr-xr-x   0 pierre    (1000) pierre    (1000)    22818 2022-03-15 09:45:31.000000 pycudwt-1.0.1/pdwt/src/wt.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3331 2022-03-15 09:45:31.000000 pycudwt-1.0.1/pdwt/src/wt.h
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2022-03-15 10:21:43.131565 pycudwt-1.0.1/pycudwt.egg-info/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      327 2022-03-15 10:21:42.000000 pycudwt-1.0.1/pycudwt.egg-info/PKG-INFO
--rw-r--r--   0 pierre    (1000) pierre    (1000)      612 2022-03-15 10:21:42.000000 pycudwt-1.0.1/pycudwt.egg-info/SOURCES.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2022-03-15 10:21:42.000000 pycudwt-1.0.1/pycudwt.egg-info/dependency_links.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2022-03-15 10:21:42.000000 pycudwt-1.0.1/pycudwt.egg-info/not-zip-safe
--rw-r--r--   0 pierre    (1000) pierre    (1000)       13 2022-03-15 10:21:42.000000 pycudwt-1.0.1/pycudwt.egg-info/requires.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)        8 2022-03-15 10:21:42.000000 pycudwt-1.0.1/pycudwt.egg-info/top_level.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)       38 2022-03-15 10:21:43.135565 pycudwt-1.0.1/setup.cfg
--rwxr-xr-x   0 pierre    (1000) pierre    (1000)     8800 2022-03-15 09:52:57.000000 pycudwt-1.0.1/setup.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2022-03-15 10:21:43.131565 pycudwt-1.0.1/src/
--rw-r--r--   0 pierre    (1000) pierre    (1000)    17531 2022-03-15 09:46:36.000000 pycudwt-1.0.1/src/pypwt.pyx
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2022-03-15 10:21:43.131565 pycudwt-1.0.1/test/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1764 2022-03-15 09:45:31.000000 pycudwt-1.0.1/test/test_all.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2270 2022-03-15 09:45:31.000000 pycudwt-1.0.1/test/test_single.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2580 2022-03-15 09:45:31.000000 pycudwt-1.0.1/test/test_sizes.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    24365 2022-03-15 09:45:31.000000 pycudwt-1.0.1/test/test_wavelets.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3662 2022-03-15 09:45:31.000000 pycudwt-1.0.1/test/testutils.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-06 14:26:00.279188 pycudwt-1.0.2/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1484 2022-03-15 09:45:31.000000 pycudwt-1.0.2/LICENSE
+-rw-r--r--   0 pierre    (1000) pierre    (1000)       52 2023-06-06 14:20:01.000000 pycudwt-1.0.2/MANIFEST.in
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      327 2023-06-06 14:26:00.279188 pycudwt-1.0.2/PKG-INFO
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1852 2023-06-06 14:22:09.000000 pycudwt-1.0.2/README.md
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-06 14:26:00.279188 pycudwt-1.0.2/pdwt/
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-06 14:26:00.279188 pycudwt-1.0.2/pdwt/src/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    20444 2022-03-15 09:45:31.000000 pycudwt-1.0.2/pdwt/src/common.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4048 2022-03-15 09:45:31.000000 pycudwt-1.0.2/pdwt/src/common.h
+-rw-r--r--   0 pierre    (1000) pierre    (1000)   136815 2022-03-15 09:45:31.000000 pycudwt-1.0.2/pdwt/src/filters.cpp
+-rwxr-xr-x   0 pierre    (1000) pierre    (1000)    10442 2022-03-15 09:45:31.000000 pycudwt-1.0.2/pdwt/src/filters.h
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     8758 2022-03-15 09:45:31.000000 pycudwt-1.0.2/pdwt/src/haar.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      789 2022-03-15 09:45:31.000000 pycudwt-1.0.2/pdwt/src/haar.h
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      190 2022-03-15 09:45:31.000000 pycudwt-1.0.2/pdwt/src/io.h
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    17734 2022-03-15 09:45:31.000000 pycudwt-1.0.2/pdwt/src/nonseparable.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1261 2022-03-15 09:45:31.000000 pycudwt-1.0.2/pdwt/src/nonseparable.h
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    27757 2022-03-15 09:45:31.000000 pycudwt-1.0.2/pdwt/src/separable.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2064 2022-03-15 09:45:31.000000 pycudwt-1.0.2/pdwt/src/separable.h
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      487 2022-03-15 09:45:31.000000 pycudwt-1.0.2/pdwt/src/utils.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      667 2022-03-15 09:45:31.000000 pycudwt-1.0.2/pdwt/src/utils.h
+-rwxr-xr-x   0 pierre    (1000) pierre    (1000)    22818 2022-03-15 09:45:31.000000 pycudwt-1.0.2/pdwt/src/wt.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3331 2022-03-15 09:45:31.000000 pycudwt-1.0.2/pdwt/src/wt.h
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-06 14:26:00.279188 pycudwt-1.0.2/pycudwt.egg-info/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      327 2023-06-06 14:26:00.000000 pycudwt-1.0.2/pycudwt.egg-info/PKG-INFO
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      627 2023-06-06 14:26:00.000000 pycudwt-1.0.2/pycudwt.egg-info/SOURCES.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2023-06-06 14:26:00.000000 pycudwt-1.0.2/pycudwt.egg-info/dependency_links.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2023-06-06 14:26:00.000000 pycudwt-1.0.2/pycudwt.egg-info/not-zip-safe
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        6 2023-06-06 14:26:00.000000 pycudwt-1.0.2/pycudwt.egg-info/requires.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        8 2023-06-06 14:26:00.000000 pycudwt-1.0.2/pycudwt.egg-info/top_level.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      127 2023-06-06 14:22:09.000000 pycudwt-1.0.2/pyproject.toml
+-rw-r--r--   0 pierre    (1000) pierre    (1000)       38 2023-06-06 14:26:00.279188 pycudwt-1.0.2/setup.cfg
+-rwxr-xr-x   0 pierre    (1000) pierre    (1000)     8767 2023-06-06 14:22:58.000000 pycudwt-1.0.2/setup.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-06 14:26:00.279188 pycudwt-1.0.2/src/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    17531 2023-06-06 14:23:29.000000 pycudwt-1.0.2/src/pypwt.pyx
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-06 14:26:00.279188 pycudwt-1.0.2/test/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1764 2022-03-15 09:45:31.000000 pycudwt-1.0.2/test/test_all.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2270 2022-03-15 09:45:31.000000 pycudwt-1.0.2/test/test_single.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2580 2022-03-15 09:45:31.000000 pycudwt-1.0.2/test/test_sizes.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    24365 2022-03-15 09:45:31.000000 pycudwt-1.0.2/test/test_wavelets.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3662 2022-03-15 09:45:31.000000 pycudwt-1.0.2/test/testutils.py
```

### Comparing `pycudwt-1.0.1/LICENSE` & `pycudwt-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycudwt-1.0.1/README.md` & `pycudwt-1.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -16,14 +16,24 @@
 
 ### Stable version (from pypi)
 
 ```bash
 pip install pycudwt
 ```
 
+### From conda recipe
+
+Conda build for a specific *cudatoolkit* version that matches one in your conda environment, e.g.:
+
+```
+export CUDA_VERSION="10.1.243"
+conda build conda-recipe/
+```
+
+
 ### Development version (from github)
 
 ```bash
 git clone https://github.com/pierrepaleo/pypwt
 cd pypwt
 pip install .
 ```
@@ -65,9 +75,7 @@
 Running on device : GeForce GTX TITAN X
 --------------------------------------------------
 W.forward()
 W.soft_threshold(10)
 W.inverse()
 imshow(W.image)
 ```
-
-
```

### Comparing `pycudwt-1.0.1/pdwt/src/common.cu` & `pycudwt-1.0.2/pdwt/src/common.cu`

 * *Files identical despite different names*

### Comparing `pycudwt-1.0.1/pdwt/src/common.h` & `pycudwt-1.0.2/pdwt/src/common.h`

 * *Files identical despite different names*

### Comparing `pycudwt-1.0.1/pdwt/src/filters.cpp` & `pycudwt-1.0.2/pdwt/src/filters.cpp`

 * *Files identical despite different names*

### Comparing `pycudwt-1.0.1/pdwt/src/filters.h` & `pycudwt-1.0.2/pdwt/src/filters.h`

 * *Files identical despite different names*

### Comparing `pycudwt-1.0.1/pdwt/src/haar.cu` & `pycudwt-1.0.2/pdwt/src/haar.cu`

 * *Files identical despite different names*

### Comparing `pycudwt-1.0.1/pdwt/src/haar.h` & `pycudwt-1.0.2/pdwt/src/haar.h`

 * *Files identical despite different names*

### Comparing `pycudwt-1.0.1/pdwt/src/nonseparable.cu` & `pycudwt-1.0.2/pdwt/src/nonseparable.cu`

 * *Files identical despite different names*

### Comparing `pycudwt-1.0.1/pdwt/src/nonseparable.h` & `pycudwt-1.0.2/pdwt/src/nonseparable.h`

 * *Files identical despite different names*

### Comparing `pycudwt-1.0.1/pdwt/src/separable.cu` & `pycudwt-1.0.2/pdwt/src/separable.cu`

 * *Files identical despite different names*

### Comparing `pycudwt-1.0.1/pdwt/src/separable.h` & `pycudwt-1.0.2/pdwt/src/separable.h`

 * *Files identical despite different names*

### Comparing `pycudwt-1.0.1/pdwt/src/utils.h` & `pycudwt-1.0.2/pdwt/src/utils.h`

 * *Files identical despite different names*

### Comparing `pycudwt-1.0.1/pdwt/src/wt.cu` & `pycudwt-1.0.2/pdwt/src/wt.cu`

 * *Files identical despite different names*

### Comparing `pycudwt-1.0.1/pdwt/src/wt.h` & `pycudwt-1.0.2/pdwt/src/wt.h`

 * *Files identical despite different names*

### Comparing `pycudwt-1.0.1/pycudwt.egg-info/SOURCES.txt` & `pycudwt-1.0.2/pycudwt.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.py
 pdwt/src/common.cu
 pdwt/src/common.h
 pdwt/src/filters.cpp
 pdwt/src/filters.h
 pdwt/src/haar.cu
 pdwt/src/haar.h
```

### Comparing `pycudwt-1.0.1/setup.py` & `pycudwt-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,22 +231,19 @@
         customize_compiler_for_nvcc(self.compiler)
         build_ext.build_extensions(self)
 
 
 setup(
     name="pycudwt",
     author="Pierre Paleo",
-    version="1.0.1",
+    version="1.0.2",
     author_email="pierre.paleo@esrf.fr",
     maintainer="Pierre Paleo",
     maintainer_email="pierre.paleo@esrf.fr",
-    install_requires=[
-        "Cython",
-        "numpy",
-    ],
+    install_requires=["numpy"],
     long_description="""
     Python Wrapper for Cuda Discrete Wavelet Transform
     """,
     ext_modules=[ext],
     # inject our custom trigger
     cmdclass={"build_ext": custom_build_ext},
     # since the package has c code, the egg cannot be zipped
```

### Comparing `pycudwt-1.0.1/src/pypwt.pyx` & `pycudwt-1.0.2/src/pypwt.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -515,8 +515,8 @@
     @classmethod
     def version(cls):
         """
         Return the current version of the pypwt library
 
         This mechanism is not so elegant and will be replaced in the future
         """
-        return "1.0.1"
+        return "1.0.2"
```

### Comparing `pycudwt-1.0.1/test/test_all.py` & `pycudwt-1.0.2/test/test_all.py`

 * *Files identical despite different names*

### Comparing `pycudwt-1.0.1/test/test_single.py` & `pycudwt-1.0.2/test/test_single.py`

 * *Files identical despite different names*

### Comparing `pycudwt-1.0.1/test/test_sizes.py` & `pycudwt-1.0.2/test/test_sizes.py`

 * *Files identical despite different names*

### Comparing `pycudwt-1.0.1/test/test_wavelets.py` & `pycudwt-1.0.2/test/test_wavelets.py`

 * *Files identical despite different names*

### Comparing `pycudwt-1.0.1/test/testutils.py` & `pycudwt-1.0.2/test/testutils.py`

 * *Files identical despite different names*

