# Comparing `tmp/openmht-0.1.0.tar.gz` & `tmp/openmht-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\openmht-0.1.0.tar", last modified: Sat Feb  8 05:28:11 2020, max compression
+gzip compressed data, was "dist\openmht-1.0.0.tar", last modified: Tue Jun  6 00:47:58 2023, max compression
```

## Comparing `openmht-0.1.0.tar` & `openmht-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2020-02-08 05:28:11.000000 openmht-0.1.0/
-drwxrwxrwx   0        0        0        0 2020-02-08 05:28:11.000000 openmht-0.1.0/openmht/
--rw-rw-rw-   0        0        0     5207 2020-02-08 05:02:44.000000 openmht-0.1.0/openmht/cli.py
--rw-rw-rw-   0        0        0     3675 2020-02-08 03:44:16.000000 openmht-0.1.0/openmht/graph.py
--rw-rw-rw-   0        0        0     2476 2020-02-08 03:38:48.000000 openmht-0.1.0/openmht/kalman_filter.py
--rw-rw-rw-   0        0        0     5396 2020-02-08 03:38:34.000000 openmht-0.1.0/openmht/mht.py
--rw-rw-rw-   0        0        0     3328 2020-02-08 03:44:24.000000 openmht-0.1.0/openmht/weighted_graph.py
--rw-rw-rw-   0        0        0        0 2020-02-08 03:31:14.000000 openmht-0.1.0/openmht/__init__.py
--rw-rw-rw-   0        0        0      197 2020-02-08 05:03:40.000000 openmht-0.1.0/openmht/__main__.py
-drwxrwxrwx   0        0        0        0 2020-02-08 05:28:11.000000 openmht-0.1.0/openmht.egg-info/
--rw-rw-rw-   0        0        0        1 2020-02-08 05:28:11.000000 openmht-0.1.0/openmht.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2020-02-08 05:28:11.000000 openmht-0.1.0/openmht.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      569 2020-02-08 05:28:11.000000 openmht-0.1.0/openmht.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2020-02-08 05:28:11.000000 openmht-0.1.0/openmht.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2020-02-08 05:28:11.000000 openmht-0.1.0/openmht.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      569 2020-02-08 05:28:11.000000 openmht-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2793 2020-02-03 07:26:11.000000 openmht-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2020-02-08 05:28:11.000000 openmht-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      868 2020-02-08 05:27:46.000000 openmht-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 00:47:58.000000 openmht-1.0.0/
+-rw-rw-rw-   0        0        0      569 2023-06-06 00:47:58.000000 openmht-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2126 2023-06-06 00:37:53.000000 openmht-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 00:47:58.000000 openmht-1.0.0/openmht/
+-rw-rw-rw-   0        0        0        0 2020-02-08 03:31:14.000000 openmht-1.0.0/openmht/__init__.py
+-rw-rw-rw-   0        0        0      117 2023-06-06 00:37:53.000000 openmht-1.0.0/openmht/__main__.py
+-rw-rw-rw-   0        0        0     5209 2023-06-06 00:39:25.000000 openmht-1.0.0/openmht/cli.py
+-rw-rw-rw-   0        0        0     3675 2020-02-08 06:06:47.000000 openmht-1.0.0/openmht/graph.py
+-rw-rw-rw-   0        0        0     2476 2023-06-06 00:37:53.000000 openmht-1.0.0/openmht/kalman_filter.py
+-rw-rw-rw-   0        0        0     5396 2023-06-06 00:37:53.000000 openmht-1.0.0/openmht/mht.py
+-rw-rw-rw-   0        0        0     3328 2023-06-06 00:40:47.000000 openmht-1.0.0/openmht/weighted_graph.py
+drwxrwxrwx   0        0        0        0 2023-06-06 00:47:58.000000 openmht-1.0.0/openmht.egg-info/
+-rw-rw-rw-   0        0        0      569 2023-06-06 00:47:58.000000 openmht-1.0.0/openmht.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-06-06 00:47:58.000000 openmht-1.0.0/openmht.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 00:47:58.000000 openmht-1.0.0/openmht.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-06 00:47:58.000000 openmht-1.0.0/openmht.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2023-06-06 00:47:58.000000 openmht-1.0.0/openmht.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 00:47:58.000000 openmht-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      868 2023-06-06 00:45:54.000000 openmht-1.0.0/setup.py
```

### Comparing `openmht-0.1.0/openmht/cli.py` & `openmht-1.0.0/openmht/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python
 """CLI"""
 
+
 from .mht import MHT
 
 import os
 import sys
 import argparse
 import time
 import csv
@@ -12,15 +13,15 @@
 import logging
 logging.basicConfig(level=logging.INFO,
                     format='%(asctime)s %(message)s',
                     datefmt='%Y-%m-%d %H:%M:%S')
 
 __author__ = "Jon Perdomo"
 __license__ = "GPL-3.0"
-__version__ = "0.0.2"
+__version__ = "0.1.0"
 
 
 def read_uv_csv(file_path, frame_max=100):
     """
     Read detections from a CSV.
     Expected column headers are:
     Frame number, U, V
```

### Comparing `openmht-0.1.0/openmht/graph.py` & `openmht-1.0.0/openmht/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 """Graph"""
 
 import numpy as np
 
 __author__ = "Jon Perdomo"
 __license__ = "GPL-3.0"
-__version__ = "0.0.2"
+__version__ = "0.1.0"
 
 class Graph(object):
     def __init__(self, graph_dict=None):
         """ initializes a graph object
             If no dictionary or None is given,
             an empty dictionary will be used
         """
```

### Comparing `openmht-0.1.0/openmht/kalman_filter.py` & `openmht-1.0.0/openmht/kalman_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 """Kalman Filter"""
 
 import numpy as np
 
 __author__ = "Jon Perdomo"
 __license__ = "GPL-3.0"
-__version__ = "0.0.2"
+__version__ = "0.1.0"
 
 
 class KalmanFilter:
     """
     Kalman filter for 2D & 3D vectors.
     """
     def __init__(self, initial_observation, image_area=307200, gating_area=1000, k=0, q=1e-5, r=0.01):
```

### Comparing `openmht-0.1.0/openmht/mht.py` & `openmht-1.0.0/openmht/mht.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import logging
 logging.basicConfig(level=logging.INFO,
                     format='%(asctime)s %(message)s',
                     datefmt='%Y-%m-%d %H:%M:%S')
 
 __author__ = "Jon Perdomo"
 __license__ = "GPL-3.0"
-__version__ = "0.0.2"
+__version__ = "0.1.0"
 
 
 class MHT:
     """
     Multiple hypothesis tracking.
     """
     def __init__(self, detections, params):
```

### Comparing `openmht-0.1.0/openmht/weighted_graph.py` & `openmht-1.0.0/openmht/weighted_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import operator
 import random
 
 from .graph import Graph
 
 __author__ = "Jon Perdomo"
 __license__ = "GPL-3.0"
-__version__ = "0.0.2"
+__version__ = "0.1.0"
 
 
 class WeightedGraph(Graph):
     """
     A graph with weighted vertices.
     """
     def __init__(self, graph_dict=None):
@@ -77,19 +77,19 @@
             self.__bron_kerbosch(R | {v}, P & N_v, X & N_v, g, results)
 
             P = P - {v}
             X = X | {v}
 
     def __degeneracy_ordering(self, g):
         """Order such that each vertex has d or fewer neighbors that come later in the ordering."""
-        v_ordered = set()
+        v_ordered = []
         degrees = list(enumerate(self.vertex_degrees(g)))
         while degrees:
             min_index, min_value = min(degrees, key=operator.itemgetter(1))
-            v_ordered.add(min_index)
+            v_ordered.append(min_index)
             degrees.remove((min_index, min_value))
 
         return v_ordered
 
     def __n(self, v, g):
         return set([i for i, n_v in enumerate(g[v]) if n_v])
```

### Comparing `openmht-0.1.0/openmht.egg-info/PKG-INFO` & `openmht-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmht
-Version: 0.1.0
+Version: 1.0.0
 Summary: OpenMHT
 Home-page: https://github.com/jonperdomo/openmht
 Author: Jonathan Elliot Perdomo
 Author-email: jonperdomodb@gmail.com
 License: UNKNOWN
 Description: An implementation of the multiple hypothesis tracking algorithm for data association.
 Platform: UNKNOWN
```

### Comparing `openmht-0.1.0/PKG-INFO` & `openmht-1.0.0/openmht.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmht
-Version: 0.1.0
+Version: 1.0.0
 Summary: OpenMHT
 Home-page: https://github.com/jonperdomo/openmht
 Author: Jonathan Elliot Perdomo
 Author-email: jonperdomodb@gmail.com
 License: UNKNOWN
 Description: An implementation of the multiple hypothesis tracking algorithm for data association.
 Platform: UNKNOWN
```

### Comparing `openmht-0.1.0/setup.py` & `openmht-1.0.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="openmht",
-    version="0.1.0",
+    version="1.0.0",
     author="Jonathan Elliot Perdomo",
     author_email="jonperdomodb@gmail.com",
     description="OpenMHT",
     long_description="An implementation of the multiple hypothesis tracking algorithm for data association.",
     long_description_content_type="text/markdown",
     url="https://github.com/jonperdomo/openmht",
     packages=setuptools.find_packages(),
```

