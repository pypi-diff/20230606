# Comparing `tmp/Python-PCG-0.1.1.tar.gz` & `tmp/Python-PCG-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Python-PCG-0.1.1.tar", last modified: Mon Dec 12 16:45:28 2022, max compression
+gzip compressed data, was "Python-PCG-0.2.tar", last modified: Tue Jun  6 11:52:50 2023, max compression
```

## Comparing `Python-PCG-0.1.1.tar` & `Python-PCG-0.2.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2022-12-12 16:45:28.430960 Python-PCG-0.1.1/
--rw-r--r--   0 matthijs   (501) staff       (20)     1061 2022-12-12 16:17:00.000000 Python-PCG-0.1.1/LICENSE
--rw-r--r--   0 matthijs   (501) staff       (20)       50 2022-12-12 16:22:24.000000 Python-PCG-0.1.1/MANIFEST.in
--rw-r--r--   0 matthijs   (501) staff       (20)      929 2022-12-12 16:45:28.431036 Python-PCG-0.1.1/PKG-INFO
--rw-r--r--   0 matthijs   (501) staff       (20)      399 2022-12-12 15:25:58.000000 Python-PCG-0.1.1/README.md
--rw-r--r--   0 matthijs   (501) staff       (20)      608 2022-12-12 16:44:56.000000 Python-PCG-0.1.1/pyproject.toml
--rw-r--r--   0 matthijs   (501) staff       (20)       89 2022-12-12 16:45:28.431303 Python-PCG-0.1.1/setup.cfg
--rw-r--r--   0 matthijs   (501) staff       (20)      383 2022-12-12 16:03:01.000000 Python-PCG-0.1.1/setup.py
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2022-12-12 16:45:28.426460 Python-PCG-0.1.1/src/
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2022-12-12 16:45:28.428290 Python-PCG-0.1.1/src/Python_PCG.egg-info/
--rw-r--r--   0 matthijs   (501) staff       (20)      929 2022-12-12 16:45:28.000000 Python-PCG-0.1.1/src/Python_PCG.egg-info/PKG-INFO
--rw-r--r--   0 matthijs   (501) staff       (20)      509 2022-12-12 16:45:28.000000 Python-PCG-0.1.1/src/Python_PCG.egg-info/SOURCES.txt
--rw-r--r--   0 matthijs   (501) staff       (20)        1 2022-12-12 16:45:28.000000 Python-PCG-0.1.1/src/Python_PCG.egg-info/dependency_links.txt
--rw-r--r--   0 matthijs   (501) staff       (20)       14 2022-12-12 16:45:28.000000 Python-PCG-0.1.1/src/Python_PCG.egg-info/top_level.txt
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2022-12-12 16:45:28.426374 Python-PCG-0.1.1/src/pcg-cpp/
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2022-12-12 16:45:28.428804 Python-PCG-0.1.1/src/pcg-cpp/include/
--rw-r--r--   0 matthijs   (501) staff       (20)    20333 2022-12-11 22:10:33.000000 Python-PCG-0.1.1/src/pcg-cpp/include/pcg_extras.hpp
--rw-r--r--   0 matthijs   (501) staff       (20)    73456 2022-12-11 22:10:33.000000 Python-PCG-0.1.1/src/pcg-cpp/include/pcg_random.hpp
--rw-r--r--   0 matthijs   (501) staff       (20)    28354 2022-12-11 22:10:33.000000 Python-PCG-0.1.1/src/pcg-cpp/include/pcg_uint128.hpp
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2022-12-12 16:45:28.430693 Python-PCG-0.1.1/src/py_pcg/
--rw-r--r--   0 matthijs   (501) staff       (20)       25 2022-12-12 15:25:58.000000 Python-PCG-0.1.1/src/py_pcg/__init__.py
--rw-r--r--   0 matthijs   (501) staff       (20)     1118 2022-12-12 15:49:18.000000 Python-PCG-0.1.1/src/py_pcg/normal_cdf.cpp
--rw-r--r--   0 matthijs   (501) staff       (20)      786 2022-12-12 15:49:23.000000 Python-PCG-0.1.1/src/py_pcg/normal_cdf.hpp
--rw-r--r--   0 matthijs   (501) staff       (20)     1646 2022-12-12 16:43:39.000000 Python-PCG-0.1.1/src/py_pcg/pcg32.py
--rw-r--r--   0 matthijs   (501) staff       (20)     3292 2022-12-12 16:00:22.000000 Python-PCG-0.1.1/src/py_pcg/pcg_wrapper.cpp
--rw-r--r--   0 matthijs   (501) staff       (20)     1718 2022-12-12 15:25:58.000000 Python-PCG-0.1.1/src/py_pcg/py_cpp_conversion.cpp
--rw-r--r--   0 matthijs   (501) staff       (20)      443 2022-12-12 15:25:58.000000 Python-PCG-0.1.1/src/py_pcg/py_cpp_conversion.hpp
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-06 11:52:50.159218 Python-PCG-0.2/
+-rw-r--r--   0 matthijs   (501) staff       (20)     1061 2023-02-01 09:53:33.000000 Python-PCG-0.2/LICENSE
+-rw-r--r--   0 matthijs   (501) staff       (20)       50 2023-02-01 09:53:33.000000 Python-PCG-0.2/MANIFEST.in
+-rw-r--r--   0 matthijs   (501) staff       (20)     1157 2023-06-06 11:52:50.159056 Python-PCG-0.2/PKG-INFO
+-rw-r--r--   0 matthijs   (501) staff       (20)      629 2023-02-01 09:53:33.000000 Python-PCG-0.2/README.md
+-rw-r--r--   0 matthijs   (501) staff       (20)      677 2023-06-06 11:50:51.000000 Python-PCG-0.2/pyproject.toml
+-rw-r--r--   0 matthijs   (501) staff       (20)       38 2023-06-06 11:52:50.159261 Python-PCG-0.2/setup.cfg
+-rw-r--r--   0 matthijs   (501) staff       (20)      385 2023-05-01 16:00:34.000000 Python-PCG-0.2/setup.py
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-06 11:52:50.147503 Python-PCG-0.2/src/
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-06 11:52:50.152900 Python-PCG-0.2/src/Python_PCG.egg-info/
+-rw-r--r--   0 matthijs   (501) staff       (20)     1157 2023-06-06 11:52:50.000000 Python-PCG-0.2/src/Python_PCG.egg-info/PKG-INFO
+-rw-r--r--   0 matthijs   (501) staff       (20)      537 2023-06-06 11:52:50.000000 Python-PCG-0.2/src/Python_PCG.egg-info/SOURCES.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)        1 2023-06-06 11:52:50.000000 Python-PCG-0.2/src/Python_PCG.egg-info/dependency_links.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)       14 2023-06-06 11:52:50.000000 Python-PCG-0.2/src/Python_PCG.egg-info/requires.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)       22 2023-06-06 11:52:50.000000 Python-PCG-0.2/src/Python_PCG.egg-info/top_level.txt
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-06 11:52:50.147371 Python-PCG-0.2/src/pcg-cpp/
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-06 11:52:50.153954 Python-PCG-0.2/src/pcg-cpp/include/
+-rw-r--r--   0 matthijs   (501) staff       (20)    20333 2023-02-01 09:53:41.000000 Python-PCG-0.2/src/pcg-cpp/include/pcg_extras.hpp
+-rw-r--r--   0 matthijs   (501) staff       (20)    73456 2023-02-01 09:53:41.000000 Python-PCG-0.2/src/pcg-cpp/include/pcg_random.hpp
+-rw-r--r--   0 matthijs   (501) staff       (20)    28354 2023-02-01 09:53:41.000000 Python-PCG-0.2/src/pcg-cpp/include/pcg_uint128.hpp
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-06 11:52:50.158710 Python-PCG-0.2/src/py_pcg/
+-rw-r--r--   0 matthijs   (501) staff       (20)      527 2023-06-06 10:57:13.000000 Python-PCG-0.2/src/py_pcg/PCGCPP.pyi
+-rw-r--r--   0 matthijs   (501) staff       (20)       25 2023-02-01 09:53:33.000000 Python-PCG-0.2/src/py_pcg/__init__.py
+-rw-r--r--   0 matthijs   (501) staff       (20)        0 2023-04-28 13:22:03.000000 Python-PCG-0.2/src/py_pcg/__init__.pyi
+-rw-r--r--   0 matthijs   (501) staff       (20)     1118 2023-02-01 09:53:33.000000 Python-PCG-0.2/src/py_pcg/normal_cdf.cpp
+-rw-r--r--   0 matthijs   (501) staff       (20)      786 2023-02-01 09:53:33.000000 Python-PCG-0.2/src/py_pcg/normal_cdf.hpp
+-rw-r--r--   0 matthijs   (501) staff       (20)     1911 2023-06-06 11:03:40.000000 Python-PCG-0.2/src/py_pcg/pcg32.py
+-rw-r--r--   0 matthijs   (501) staff       (20)      459 2023-06-06 10:56:42.000000 Python-PCG-0.2/src/py_pcg/pcg32.pyi
+-rw-r--r--   0 matthijs   (501) staff       (20)     3490 2023-05-01 13:59:00.000000 Python-PCG-0.2/src/py_pcg/pcg_wrapper.cpp
```

### Comparing `Python-PCG-0.1.1/LICENSE` & `Python-PCG-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Python-PCG-0.1.1/src/pcg-cpp/include/pcg_extras.hpp` & `Python-PCG-0.2/src/pcg-cpp/include/pcg_extras.hpp`

 * *Files identical despite different names*

### Comparing `Python-PCG-0.1.1/src/pcg-cpp/include/pcg_random.hpp` & `Python-PCG-0.2/src/pcg-cpp/include/pcg_random.hpp`

 * *Files identical despite different names*

### Comparing `Python-PCG-0.1.1/src/pcg-cpp/include/pcg_uint128.hpp` & `Python-PCG-0.2/src/pcg-cpp/include/pcg_uint128.hpp`

 * *Files identical despite different names*

### Comparing `Python-PCG-0.1.1/src/py_pcg/normal_cdf.cpp` & `Python-PCG-0.2/src/py_pcg/normal_cdf.cpp`

 * *Files identical despite different names*

### Comparing `Python-PCG-0.1.1/src/py_pcg/normal_cdf.hpp` & `Python-PCG-0.2/src/py_pcg/normal_cdf.hpp`

 * *Files identical despite different names*

### Comparing `Python-PCG-0.1.1/src/py_pcg/pcg32.py` & `Python-PCG-0.2/src/py_pcg/pcg32.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,68 @@
+from typing import Any, Optional, Union
 import PCGCPP
+import numpy.typing as npt
 
 class PCG32:
     """Wrapper around the pcg32 class.
     
     >>> rng = PCG32(42)
     >>> rng.randint()
     589627368
     >>> rng.randint()
     2336806640
     """
-    def __init__(self, stream = None, state = None):
+    def __init__(self, stream: Optional[int] = None, state: Optional[int] = None):
         if stream and state:
             self.capsule = PCGCPP.construct(stream, state)
         elif stream:
             self.capsule = PCGCPP.construct(stream)
         else:
             self.capsule = PCGCPP.construct()
     
-    def randint(self, size = 1, bound = 0):
+    def randint(self, size: int = 1, bound: int = 0) -> Union[npt.NDArray[Any], int]:
         """Draw a random integer, with an optional upper bound.
         
         >>> rng = PCG32(42, 54)
-        >>> rng.randint(2)
+        >>> rng.randint(2).tolist()
         [1070908346, 3346215311]
-        >>> rng.randint(2, bound=100)
+        >>> rng.randint(2, bound=100).tolist()
         [67, 65]
         """
         result = PCGCPP.randint(self.capsule, size, bound)
 
         if size == 1:
             return result[0]
         
         return result
     
-    def rand(self, size = 1):
+    def rand(self, size: int = 1) -> Union[npt.NDArray[Any], float]:
         """Draw a uniform random number in the interval [0,1).
 
-        >>> rng = PCG32(42 ,54)
-        >>> rng.rand(2)
+        >>> rng = PCG32(42, 54)
+        >>> rng.rand(2).tolist()
         [0.24934027949348092, 0.7791014646645635]
         """
         result = PCGCPP.rand(self.capsule, size)
 
         if size == 1:
             return result[0]
         
         return result
     
-    def randn(self, size = 1):
+    def randn(self, size: int = 1) -> Union[npt.NDArray[Any], float]:
         """Draw a random number following a standard normal PDF.
 
-        >>> rng = PCG32(42 ,54)
-        >>> rng.randn(2)
+        >>> rng = PCG32(42, 54)
+        >>> rng.randn(2).tolist()
         [-0.6765672580042227, 0.7691621258667373]
         """
         result = PCGCPP.randn(self.capsule, size)
 
         if size == 1:
             return result[0]
         
         return result
 
 if __name__ == "__main__":
     import doctest
-    doctest.testmod()
+    doctest.testmod(verbose=True)
```

### Comparing `Python-PCG-0.1.1/src/py_pcg/pcg_wrapper.cpp` & `Python-PCG-0.2/src/py_pcg/pcg_wrapper.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,117 +1,120 @@
 #include <random>
 #include <stdio.h>
-#include <vector>
 
-#include "Python.h"
+#include <Python.h>
+#define NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION
+#include <numpy/arrayobject.h>
 
 #include "normal_cdf.hpp"
 #include "pcg_random.hpp"
-#include "py_cpp_conversion.hpp"
 
 using namespace std;
 
 #define PCG32_MAX1 (double)4294967296.0
 
 // ------------------- Class wrappers -------------------
 
 PyObject *construct32(PyObject *self, PyObject *args) {
     uint64_t stream = 0xda3e39cb94b95bdbULL; // Taken from the minimal C implementation
-    uint64_t state = 0x853c49e6748fea9bULL;
+    uint64_t state  = 0x853c49e6748fea9bULL;
 
     PyArg_ParseTuple(args, "|kk", &stream, &state);
-    
+
     pcg32 *rng;
 
     if (stream == 0xda3e39cb94b95bdbULL) {
         rng = new pcg32();
         rng->seed(pcg_extras::seed_seq_from<std::random_device>());
     } else {
         rng = new pcg32(state, stream);
     }
-    
+
     PyObject *rngCapsule = PyCapsule_New((void *)rng, "rngPtr", NULL);
     PyCapsule_SetPointer(rngCapsule, (void *)rng);
-    
+
     return Py_BuildValue("O", rngCapsule);
 }
 
 PyObject *randint32(PyObject *self, PyObject *args) {
-    vector<uint32_t> result;
+    uint32_t *result;
     uint32_t size = 1;
     uint32_t bound = 0;
-    
+
     PyObject *rngCapsule = NULL;
     PyArg_ParseTuple(args, "O|II", &rngCapsule, &size, &bound);
-    
+
     pcg32 *rng = (pcg32 *)PyCapsule_GetPointer(rngCapsule, "rngPtr");
-    result.reserve(size);
+    result = (uint32_t *)malloc(size * sizeof(uint32_t));
 
     if (bound > 0) {
         for (uint32_t i = 0; i < size; i++) {
-            result.push_back(rng->operator()(bound));
+            result[i] = rng->operator()(bound);
         }
     } else {
         for (uint32_t i = 0; i < size; i++) {
-            result.push_back(rng->operator()());
+            result[i] = rng->operator()();
         }
     }
-    
-    return vectorUint32ToListInt(result);
+
+    npy_intp dims[1] = {size};
+    return PyArray_SimpleNewFromData(1, dims, NPY_UINT32, result);
 }
 
 PyObject *rand32(PyObject *self, PyObject *args) {
-    vector<double> result;
+    double *result;
     uint32_t size = 1;
-    
+
     PyObject *rngCapsule = NULL;
     PyArg_ParseTuple(args, "O|I", &rngCapsule, &size);
-    
+
     pcg32 *rng = (pcg32 *)PyCapsule_GetPointer(rngCapsule, "rngPtr");
-    result.reserve(size);
+    result = (double *)malloc(size * sizeof(double));
 
     for (uint32_t i = 0; i < size; i++) {
-        result.push_back(rng->operator()() / PCG32_MAX1);
+        result[i] = rng->operator()() / PCG32_MAX1;
     }
-    
-    return vectorDoubleToListFloat(result);
+
+    npy_intp dims[1] = {size};
+    return PyArray_SimpleNewFromData(1, dims, NPY_DOUBLE, result);
 }
 
 PyObject *randn32(PyObject *self, PyObject *args) {
-    vector<double> result;
+    double *result;
     uint32_t size = 1;
-    
+
     PyObject *rngCapsule = NULL;
     PyArg_ParseTuple(args, "O|I", &rngCapsule, &size);
-    
+
     pcg32 *rng = (pcg32 *)PyCapsule_GetPointer(rngCapsule, "rngPtr");
-    result.reserve(size);
+    result = (double *)malloc(size * sizeof(double));
 
     for (uint32_t i = 0; i < size; i++) {
-        result.push_back(inverse_normal_cdf(rng->operator()() / PCG32_MAX1));
+        result[i] = inverse_normal_cdf(rng->operator()() / PCG32_MAX1);
     }
-    
-    return vectorDoubleToListFloat(result);
+
+    npy_intp dims[1] = {size};
+    return PyArray_SimpleNewFromData(1, dims, NPY_DOUBLE, result);
 }
 
 // --------------------- Module definitions ---------------------
 
 PyMethodDef PCGCPPFunctions[] = {
     {"construct",
       construct32, METH_VARARGS,
      "Create `PCGCPP` object."},
-    
+
     {"randint",
       randint32, METH_VARARGS,
      "Obtain 1 or more random integers, with an optional bound."},
-    
+
     {"rand",
       rand32, METH_VARARGS,
      "Obtain 1 or more random doubles in the range [0,1)."},
-    
+
     {"randn",
       randn32, METH_VARARGS,
      "Obtain 1 or more random doubles following a standard normal PDF."},
 
     {NULL, NULL, 0, NULL}
 };
 
@@ -121,9 +124,10 @@
    "Python wrapper around the pcg-cpp library.", 
    -1,
    PCGCPPFunctions
 };
 
 
 PyMODINIT_FUNC PyInit_PCGCPP(void) {
+    import_array();
     return PyModule_Create(&PCGCPPModule);
 }
```

