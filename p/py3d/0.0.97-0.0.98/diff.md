# Comparing `tmp/py3d-0.0.97.tar.gz` & `tmp/py3d-0.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3d-0.0.97.tar", last modified: Fri Jun  2 15:23:10 2023, max compression
+gzip compressed data, was "py3d-0.0.98.tar", last modified: Tue Jun  6 15:39:23 2023, max compression
```

## Comparing `py3d-0.0.97.tar` & `py3d-0.0.98.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 15:23:10.783317 py3d-0.0.97/
--rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-06-02 15:23:10.783317 py3d-0.0.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-06-02 15:22:45.000000 py3d-0.0.97/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 15:23:10.783317 py3d-0.0.97/py3d/
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-02 15:21:54.000000 py3d-0.0.97/py3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    28253 2023-06-02 15:21:54.000000 py3d-0.0.97/py3d/core.py
--rw-r--r--   0 runner    (1001) docker     (122)    22609 2023-06-02 15:21:54.000000 py3d-0.0.97/py3d/viewer.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 15:23:10.783317 py3d-0.0.97/py3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-06-02 15:23:10.000000 py3d-0.0.97/py3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-02 15:23:10.000000 py3d-0.0.97/py3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 15:23:10.000000 py3d-0.0.97/py3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-02 15:23:10.000000 py3d-0.0.97/py3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-02 15:23:10.000000 py3d-0.0.97/py3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-02 15:23:10.783317 py3d-0.0.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-02 15:21:54.000000 py3d-0.0.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:39:23.944769 py3d-0.0.98/
+-rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-06-06 15:39:23.944769 py3d-0.0.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-06-06 15:39:02.000000 py3d-0.0.98/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:39:23.940769 py3d-0.0.98/py3d/
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-06 15:38:18.000000 py3d-0.0.98/py3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28362 2023-06-06 15:38:18.000000 py3d-0.0.98/py3d/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22635 2023-06-06 15:38:18.000000 py3d-0.0.98/py3d/viewer.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:39:23.940769 py3d-0.0.98/py3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-06-06 15:39:23.000000 py3d-0.0.98/py3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-06 15:39:23.000000 py3d-0.0.98/py3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-06 15:39:23.000000 py3d-0.0.98/py3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-06 15:39:23.000000 py3d-0.0.98/py3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-06 15:39:23.000000 py3d-0.0.98/py3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-06 15:39:23.944769 py3d-0.0.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-06 15:38:18.000000 py3d-0.0.98/setup.py
```

### Comparing `py3d-0.0.97/PKG-INFO` & `py3d-0.0.98/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.0.97
+Version: 0.0.98
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.0.97/README.md` & `py3d-0.0.98/README.md`

 * *Files identical despite different names*

### Comparing `py3d-0.0.97/py3d/core.py` & `py3d-0.0.98/py3d/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) Tumiz.
 # Distributed under the terms of the GPL-3.0 License.
 from __future__ import annotations
 import numpy
 from IPython.display import display, HTML
-from typing import Dict
+from typing import Dict, Union
 import pathlib
 import uuid
 import json
 import struct
 
 pi = numpy.arccos(-1)
 __module__ = __import__(__name__)
@@ -222,35 +222,35 @@
         return self[..., 0:3].view(Vector3)
 
     @xyz.setter
     def xyz(self, v):
         self[..., 0:3] = v
 
     @property
-    def U(self) -> Vector:
+    def U(self) -> Union[Vector, Vector2, Vector3, Vector4]:
         '''
         unit vector, direction vector
         '''
         n = self.L
         return numpy.divide(self, n, where=n != 0)
 
     @property
-    def H(self) -> Vector:
+    def H(self) -> Union[Vector, Vector2, Vector3, Vector4]:
         '''
         Homogeneous vector
         '''
         ret = numpy.insert(self, self.shape[-1], 1, axis=self.ndim-1)
         w = ret.shape[-1]
         if w in [2, 3, 4]:
             return ret.view(getattr(__module__, f"Vector{w}"))
         else:
             return ret.view(Vector)
 
     @property
-    def M(self) -> Vector:
+    def M(self) -> Union[Vector, Vector2, Vector3, Vector4]:
         # mean vector
         return super().mean(axis=self.ndim-2)
 
     @property
     def L(self) -> Vector:
         # length
         return numpy.linalg.norm(self, axis=self.ndim - 1, keepdims=True)
```

### Comparing `py3d-0.0.97/py3d/viewer.html` & `py3d-0.0.98/py3d/viewer.html`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
             )
         }
     }
     class ToolBar {
         constructor(cache) {
             this.bar = document.createElement("div")
             this.cache = cache
-            this.ts = Object.keys(this.cache).sort()
+            this.ts = Object.keys(this.cache).sort((a, b) => { return a - b })
             this.ti = this.ts.length - 1
             this.slider = document.createElement("input")
             this.slider.type = "range"
             this.slider.style.width = "100%"
             this.slider.style.verticalAlign = "middle"
             this.slider.style.height = "3px"
             this.slider.min = this.ts[0] > 0 ? this.ts[0] : this.ts[1]
```

### Comparing `py3d-0.0.97/py3d.egg-info/PKG-INFO` & `py3d-0.0.98/py3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.0.97
+Version: 0.0.98
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.0.97/setup.py` & `py3d-0.0.98/setup.py`

 * *Files identical despite different names*

