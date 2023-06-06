# Comparing `tmp/crossroads-schematization-0.0.9.tar.gz` & `tmp/crossroads-schematization-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossroads-schematization-0.0.9.tar", last modified: Tue May 16 13:44:59 2023, max compression
+gzip compressed data, was "crossroads-schematization-0.1.0.tar", last modified: Tue Jun  6 13:14:31 2023, max compression
```

## Comparing `crossroads-schematization-0.0.9.tar` & `crossroads-schematization-0.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-05-16 13:44:59.007081 crossroads-schematization-0.0.9/
--rw-r--r--   0 jm        (1000) jm        (1000)      107 2022-11-30 16:15:16.000000 crossroads-schematization-0.0.9/MANIFEST.in
--rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-05-16 13:44:59.007081 crossroads-schematization-0.0.9/PKG-INFO
--rw-r--r--   0 jm        (1000) jm        (1000)     2897 2022-11-30 16:53:52.000000 crossroads-schematization-0.0.9/README.md
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-05-16 13:44:59.003081 crossroads-schematization-0.0.9/crossroads_schematization.egg-info/
--rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-05-16 13:44:58.000000 crossroads-schematization-0.0.9/crossroads_schematization.egg-info/PKG-INFO
--rw-r--r--   0 jm        (1000) jm        (1000)      794 2023-05-16 13:44:58.000000 crossroads-schematization-0.0.9/crossroads_schematization.egg-info/SOURCES.txt
--rw-r--r--   0 jm        (1000) jm        (1000)        1 2023-05-16 13:44:58.000000 crossroads-schematization-0.0.9/crossroads_schematization.egg-info/dependency_links.txt
--rw-r--r--   0 jm        (1000) jm        (1000)       98 2023-05-16 13:44:58.000000 crossroads-schematization-0.0.9/crossroads_schematization.egg-info/entry_points.txt
--rw-r--r--   0 jm        (1000) jm        (1000)        8 2023-05-16 13:44:58.000000 crossroads-schematization-0.0.9/crossroads_schematization.egg-info/top_level.txt
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-05-16 13:44:59.003081 crossroads-schematization-0.0.9/crschem/
--rw-r--r--   0 jm        (1000) jm        (1000)       22 2023-05-16 13:44:31.000000 crossroads-schematization-0.0.9/crschem/__init__.py
--rw-r--r--   0 jm        (1000) jm        (1000)     5853 2022-12-02 09:57:06.000000 crossroads-schematization-0.0.9/crschem/cmd.py
--rw-r--r--   0 jm        (1000) jm        (1000)    37904 2023-05-16 13:20:22.000000 crossroads-schematization-0.0.9/crschem/crossroad.py
--rw-r--r--   0 jm        (1000) jm        (1000)    21474 2023-05-16 13:43:40.000000 crossroads-schematization-0.0.9/crschem/crossroad_schematization.py
--rw-r--r--   0 jm        (1000) jm        (1000)     5393 2023-05-12 08:32:50.000000 crossroads-schematization-0.0.9/crschem/processing.py
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-05-16 13:44:59.007081 crossroads-schematization-0.0.9/crschem/resources/
--rw-r--r--   0 jm        (1000) jm        (1000)     2425 2022-10-28 13:53:49.000000 crossroads-schematization-0.0.9/crschem/resources/crossing.svg
--rw-r--r--   0 jm        (1000) jm        (1000)    23130 2023-02-06 15:35:04.000000 crossroads-schematization-0.0.9/crschem/resources/rendering-areas.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    29217 2023-01-16 14:33:05.000000 crossroads-schematization-0.0.9/crschem/resources/rendering-nodes-crossings.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    22244 2023-01-16 15:35:19.000000 crossroads-schematization-0.0.9/crschem/resources/rendering-nodes-islands.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    22752 2023-02-06 15:36:47.000000 crossroads-schematization-0.0.9/crschem/resources/rendering-nodes-space.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    35242 2023-01-16 09:30:00.000000 crossroads-schematization-0.0.9/crschem/resources/rendering-nodes.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    28654 2023-02-06 15:35:25.000000 crossroads-schematization-0.0.9/crschem/resources/rendering-polylines-space.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    28635 2023-01-16 09:29:31.000000 crossroads-schematization-0.0.9/crschem/resources/rendering-polylines.qml
--rw-r--r--   0 jm        (1000) jm        (1000)     7371 2022-11-10 14:22:27.000000 crossroads-schematization-0.0.9/crschem/resources/tactile-a5.qpt
--rw-r--r--   0 jm        (1000) jm        (1000)     7350 2023-05-16 08:27:12.000000 crossroads-schematization-0.0.9/crschem/utils.py
--rw-r--r--   0 jm        (1000) jm        (1000)       36 2023-05-15 13:14:07.000000 crossroads-schematization-0.0.9/requirements.txt
--rw-r--r--   0 jm        (1000) jm        (1000)       38 2023-05-16 13:44:59.007081 crossroads-schematization-0.0.9/setup.cfg
--rw-r--r--   0 jm        (1000) jm        (1000)     1207 2022-11-30 16:14:11.000000 crossroads-schematization-0.0.9/setup.py
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-06 13:14:31.214410 crossroads-schematization-0.1.0/
+-rw-r--r--   0 jm        (1000) jm        (1000)      107 2022-11-30 16:15:16.000000 crossroads-schematization-0.1.0/MANIFEST.in
+-rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-06-06 13:14:31.210410 crossroads-schematization-0.1.0/PKG-INFO
+-rw-r--r--   0 jm        (1000) jm        (1000)     2897 2022-11-30 16:53:52.000000 crossroads-schematization-0.1.0/README.md
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-06 13:14:31.210410 crossroads-schematization-0.1.0/crossroads_schematization.egg-info/
+-rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-06-06 13:14:31.000000 crossroads-schematization-0.1.0/crossroads_schematization.egg-info/PKG-INFO
+-rw-r--r--   0 jm        (1000) jm        (1000)      794 2023-06-06 13:14:31.000000 crossroads-schematization-0.1.0/crossroads_schematization.egg-info/SOURCES.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)        1 2023-06-06 13:14:31.000000 crossroads-schematization-0.1.0/crossroads_schematization.egg-info/dependency_links.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)       98 2023-06-06 13:14:31.000000 crossroads-schematization-0.1.0/crossroads_schematization.egg-info/entry_points.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)        8 2023-06-06 13:14:31.000000 crossroads-schematization-0.1.0/crossroads_schematization.egg-info/top_level.txt
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-06 13:14:31.210410 crossroads-schematization-0.1.0/crschem/
+-rw-r--r--   0 jm        (1000) jm        (1000)       22 2023-06-06 13:11:18.000000 crossroads-schematization-0.1.0/crschem/__init__.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     6727 2023-06-06 12:30:02.000000 crossroads-schematization-0.1.0/crschem/cmd.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    51224 2023-06-06 12:40:32.000000 crossroads-schematization-0.1.0/crschem/crossroad.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    23404 2023-06-06 12:28:22.000000 crossroads-schematization-0.1.0/crschem/crossroad_schematization.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     5393 2023-05-12 08:32:50.000000 crossroads-schematization-0.1.0/crschem/processing.py
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-06 13:14:31.210410 crossroads-schematization-0.1.0/crschem/resources/
+-rw-r--r--   0 jm        (1000) jm        (1000)     2425 2022-10-28 13:53:49.000000 crossroads-schematization-0.1.0/crschem/resources/crossing.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)    23130 2023-02-06 15:35:04.000000 crossroads-schematization-0.1.0/crschem/resources/rendering-areas.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    29214 2023-05-19 13:30:46.000000 crossroads-schematization-0.1.0/crschem/resources/rendering-nodes-crossings.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    22244 2023-05-19 13:29:18.000000 crossroads-schematization-0.1.0/crschem/resources/rendering-nodes-islands.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    22753 2023-05-19 13:31:32.000000 crossroads-schematization-0.1.0/crschem/resources/rendering-nodes-space.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    35238 2023-05-19 13:31:15.000000 crossroads-schematization-0.1.0/crschem/resources/rendering-nodes.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    28654 2023-02-06 15:35:25.000000 crossroads-schematization-0.1.0/crschem/resources/rendering-polylines-space.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    28635 2023-01-16 09:29:31.000000 crossroads-schematization-0.1.0/crschem/resources/rendering-polylines.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)     7371 2022-11-10 14:22:27.000000 crossroads-schematization-0.1.0/crschem/resources/tactile-a5.qpt
+-rw-r--r--   0 jm        (1000) jm        (1000)     7843 2023-06-05 15:25:19.000000 crossroads-schematization-0.1.0/crschem/utils.py
+-rw-r--r--   0 jm        (1000) jm        (1000)       36 2023-05-15 13:14:07.000000 crossroads-schematization-0.1.0/requirements.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)       38 2023-06-06 13:14:31.214410 crossroads-schematization-0.1.0/setup.cfg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1207 2022-11-30 16:14:11.000000 crossroads-schematization-0.1.0/setup.py
```

### Comparing `crossroads-schematization-0.0.9/PKG-INFO` & `crossroads-schematization-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossroads-schematization
-Version: 0.0.9
+Version: 0.1.0
 Summary: Crossroads schematization is a python tool that produces automatic schematization of intersections from OpenStreetMap.
 Home-page: https://github.com/jmtrivial/crossroads-schematization/
 Author: Jean-Marie Favreau
 Author-email: j-marie.favreau@uca.fr
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crossroads-schematization-0.0.9/README.md` & `crossroads-schematization-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.0.9/crossroads_schematization.egg-info/PKG-INFO` & `crossroads-schematization-0.1.0/crossroads_schematization.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossroads-schematization
-Version: 0.0.9
+Version: 0.1.0
 Summary: Crossroads schematization is a python tool that produces automatic schematization of intersections from OpenStreetMap.
 Home-page: https://github.com/jmtrivial/crossroads-schematization/
 Author: Jean-Marie Favreau
 Author-email: j-marie.favreau@uca.fr
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crossroads-schematization-0.0.9/crossroads_schematization.egg-info/SOURCES.txt` & `crossroads-schematization-0.1.0/crossroads_schematization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.0.9/crschem/cmd.py` & `crossroads-schematization-0.1.0/crschem/cmd.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,18 @@
     group_input.add_argument('--ignore-cache', help='Ignore local cache', action='store_true')
 
     group_preprocess = parser.add_argument_group('Preprocessing', "Parameters of the preprocesses (crseg, crdesc)")
     group_preprocess.add_argument('--c0', help='Initial intersection size (distance between boundaries and middle of the initial intersection). Default: 2.', type=float, default=2)
     group_preprocess.add_argument('--c1', help='Intersection size (aggregation by adjacency). Default: 2.', type=float, default=2)
     group_preprocess.add_argument('--c2', help='Intersection size (aggregation by cycle detection). Default: 4.', type=float, default=4)
 
+    group_process = parser.add_argument_group("Processing", "Parameters of the processing")
+    group_process.add_argument('--ignore-crossings-for-sidewalks', help='Do not use crossings to shape the sidewalks', action='store_true')
+    group_process.add_argument('--use-fixed-width-on-branches', help='Use a fixed width on each branch (do not evaluate the width adjustment)', action='store_true')
+    group_process.add_argument('--turn-shape', help='Turn shape.', type=lambda s: c.TurningSidewalk.TurnShape[s], choices=list(c.TurningSidewalk.TurnShape))
 
     group_output = parser.add_argument_group("Output", "Display, log or save results")
     group_output.add_argument('-l', '--log-files', help='keep intermediate files and give their name in output', action='store_true')
     group_output.add_argument('-d', '--display-all', help='display all steps', action='store_true')
     group_output.add_argument('--display-preview', help='display a preview of the crossroad schematization', action='store_true')
     group_output.add_argument('-o', '--output', help='output file (supported format: geojson, pdf, tif)', type=FileOpener('w'))
 
@@ -66,14 +70,17 @@
             crschem = cs.CrossroadSchematization(cr_input, G_init)
         else:
             latitude = args.by_coordinates[0]
             longitude = args.by_coordinates[1]
             crschem = cs.CrossroadSchematization.build(latitude, longitude,
                                                     args.c0, args.c1, args.c2,
                                                     verbose = True,
+                                                    ignore_crossings_for_sidewalks = args.ignore_crossings_for_sidewalks,
+                                                    use_fixed_width_on_branches = args.use_fixed_width_on_branches,
+                                                    turn_shape = args.turn_shape,
                                                     ignore_cache = args.ignore_cache,
                                                     overpass = args.overpass,
                                                     log_files = args.log_files)
 
         '''if not crschem.is_valid_model():
             print("Error: the model is not valid")
             exit(1)'''
```

### Comparing `crossroads-schematization-0.0.9/crschem/crossroad.py` & `crossroads-schematization-0.1.0/crschem/crossroad.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,32 +4,31 @@
 from numpy import linalg
 import copy
 import math
 import shapely.ops
 import osmnx
 from more_itertools import locate
 import geopandas
+from enum import Enum
 
 from . import utils as u
 from . import processing as p
 
 
 class SimpleWay:
     
     # parameters (and attributes)
     # - n1 is the interior node, n2 is the exterior node  (centripetal orientation)
     # - edge_tags: tags from crdesc
     # - same_osm_orientation: boolean (is the OSM orientation similar)
-    # - is_crossing_interior_node: return true if the first node is a crossing
-    def __init__(self, n1, n2, edge_tags, same_osm_orientation, is_crossing_interior_node):
+    def __init__(self, n1, n2, edge_tags, same_osm_orientation):
         self.n1 = n1
         self.n2 = n2
         self.same_osm_orientation = same_osm_orientation
         self.edge_tags = edge_tags
-        self.is_crossing_interior_node = is_crossing_interior_node
 
 
     def has_sidewalk(self):
         return SimpleWay.is_number(self.edge_tags["left_sidewalk"]) or SimpleWay.is_number(self.edge_tags["right_sidewalk"])
 
 
     def is_number(value):
@@ -46,18 +45,14 @@
         else:
             return ""
 
     def has_sidewalks_both_sides(self):
         return SimpleWay.is_number(self.edge_tags["left_sidewalk"]) and SimpleWay.is_number(self.edge_tags["right_sidewalk"])
 
 
-    def is_crossing_inner_node(self):
-        return self.is_crossing_interior_node
-
-
     def get_initial_edge_id(self):
         if self.same_osm_orientation:
             return self.get_edge_id()
         else:
             return self.get_edge_id_reverse()
 
 
@@ -70,25 +65,26 @@
 
 
 class StraightWay(SimpleWay):
     
     # parameters (and attributes)
     # - a simpleway (defined by nodes n1, n2)
     # - polybranch: an extended path from n1, n2
-    def __init__(self, sw, polybranch):
-        super().__init__(sw.n1, sw.n2, sw.edge_tags, sw.same_osm_orientation, sw.is_crossing_interior_node)
+    def __init__(self, sw, polybranch, G):
+        super().__init__(sw.n1, sw.n2, sw.edge_tags, sw.same_osm_orientation)
         self.polybranch = polybranch
         self.edge = None
         self.array = None
+        self.G = G
         self.lz = p.Linearization()
         self.maximal_removal = 20 # meters
 
 
     def build_from_simpleway(sw, G, left_first):
-        result = StraightWay(sw, p.Expander.extend_branch(G, sw.n1, sw.n2, left_first)) 
+        result = StraightWay(sw, p.Expander.extend_branch(G, sw.n1, sw.n2, left_first), G) 
         result.compute_linear_edge(G)
         return result
 
 
     def compute_linear_edge(self, G):
         self.consolidated_polybranch = p.Expander.remove_non_straight_parts(G, self.polybranch, self.maximal_removal)
         self.edge = self.lz.process(p.Expander.convert_to_linestring(G, self.consolidated_polybranch))
@@ -135,33 +131,49 @@
         # plt.plot([c[0] for c in sw2.array], [c[1] for c in sw2.array])
 
         # plt.plot([sw1.osm_input.nodes[sw1.n1]["x"], sw1.osm_input.nodes[sw1.n2]["x"]], [sw1.osm_input.nodes[sw1.n1]["y"], sw1.osm_input.nodes[sw1.n2]["y"]])
         # plt.plot([sw2.osm_input.nodes[sw2.n1]["x"], sw2.osm_input.nodes[sw2.n2]["x"]], [sw2.osm_input.nodes[sw2.n1]["y"], sw2.osm_input.nodes[sw2.n2]["y"]])
         # plt.show()
                 
         return LineString([LineString([e1_1, e2_1]).centroid, LineString([e1_2, e2_2]).centroid])
-    
-    
-    # basic evaluation of the width using number of lanes, and type of highway
-    def evaluate_width_way(self, osm_graph):
-        return u.Utils.evaluate_width_way(osm_graph[self.polybranch[-1]][self.polybranch[-2]][0])
 
 
+    def get_projection_on_polybranch(self, point):
+        line = [(self.G.nodes[x]["x"], self.G.nodes[x]["y"]) for x in self.polybranch]
+        nearest = shapely.ops.nearest_points(LineString(line), Point(point))
+        pt = nearest[0]
+
+        edges = []
+        for e1, e2 in zip(self.polybranch, self.polybranch[1:]):
+            if u.Utils.is_in_edge(pt, self.G.nodes[e1], self.G.nodes[e2]):
+                edges.append((e1, e2))
+
+        if len(edges) == 0:
+            return pt, None
+        elif len(edges) == 1:
+            return pt, edges[0]
+        else:
+            # find the edge with the largest estimated width
+            ewidths = [(e, u.Utils.evaluate_width_way(self.G[e[0]][e[1]][0])) for e in edges]
+            return pt, max(ewidths, key=lambda x: x[1])[0]
+        
+
 class StraightSidewalk:
 
-    def __init__(self, edge, description, same_orientation, side, is_crossing_inner_node):
+    def __init__(self, edge, straightway, side):
         self.edge = edge
-        self.description = description
-        self.same_orientation = same_orientation
+        self.straightway = straightway
+        self.description = straightway.edge_tags
+        self.same_orientation = straightway.same_osm_orientation
         self.side = side
-        if is_crossing_inner_node:
-            # extends the sidewalk in the inner direction if the inner point is a crossing
-            self.extends_start()
 
 
+    def get_polybranch(self):
+        return self.straightway.polybranch
+
     def __str__(self):
         return str(self.edge) + "; side: " + str(self.side) + "; same orientation: " + str(self.same_orientation)
 
 
     def update_first_node(self, coords):
         self.edge = LineString([coords, self.edge.coords[1]])
 
@@ -206,54 +218,239 @@
 
     def getOSMIds(self):
         return ";".join(self.description["osm_node_ids"])
 
 
 class TurningSidewalk:
 
-    # TODO: add a supplementary point of pedestrian crossings in the turn (./example-pdf.sh 10)
+    class TurnShape(Enum):
+        BEVELED = 0
+        STRAIGHT_ANGLE = 1
+        ADJUSTED_ANGLE = 2
+
+        def __str__(self):
+                return self.name
+
+        @staticmethod
+        def from_string(s):
+            try:
+                return TurnShape[s]
+            except KeyError:
+                raise ValueError()
+                
+    class Point:
+        def __init__(self, coord, curvPos = None):
+            if isinstance(coord, Point):
+                self.coord = (coord.x, coord.y)
+            else:
+                self.coord = coord
+            self.curvPos = curvPos
+        
+        def set_curvilign_position(self, curvPos):
+            self.curvPos = curvPos
 
-    def __init__(self, str_sidewalks, osm_input, distance_kerb_footway):
-        self.distance_kerb_footway = distance_kerb_footway
+    class FlexiblePoint(Point):
+        def __init__(self, coord, curvPos = None):
+            super().__init__(coord, curvPos)
+            self.flexible = True
+
+    class FixedPoint(Point):
+        def __init__(self, coord, curvPos = None):
+            super().__init__(coord, curvPos)
+            self.flexible = False
 
+    class CrossingPoint(FixedPoint):
+        pass
+
+        
+
+    def __init__(self, id, str_sidewalks, crossings, 
+                 osm_input, cr_input,
+                 distance_kerb_footway, ignore_crossings_for_sidewalks,
+                 turn_shape = TurnShape.ADJUSTED_ANGLE):
+        self.id = id
+
+        self.distance_kerb_footway = distance_kerb_footway
+        self.turn_shape = turn_shape
         self.str_sidewalks = str_sidewalks
+
+        self.crossings = crossings
         
         self.osm_input = osm_input
+        self.cr_input = cr_input
 
-        self.build_simple_turn()
+        self.epsilon_for_merging = 2
 
-        if self.way is None or self.way.is_empty:
-            self.build_beveled_turn()
-        else:
-            if self.is_flexible_way:
-                self.adjust_intersection()
+        self.build_initial_turn()
 
+        if not ignore_crossings_for_sidewalks:
+            self.add_crossings()
 
-    def get_middle_bevel(self):
-        p1 = self.str_sidewalks[0].edge.coords[0]
-        p2 = self.str_sidewalks[1].edge.coords[0]
-        return [(x + y) / 2 for x, y in zip(p1, p2)]
+        self.adjust_flexible_points()
 
 
-    def adjust_intersection(self):
-        middle_sw = self.way.coords[1]
-        buffered_osm = u.Utils.get_buffered_osm(self.osm_input, self.distance_kerb_footway)
+    def build_initial_turn_basic(self):
+        self.way = [TurningSidewalk.FixedPoint(c) for c in self.str_sidewalks[0].edge.coords][::-1] + [TurningSidewalk.FixedPoint(c) for c in self.str_sidewalks[1].edge.coords]
+
+
+    def add_intersection_point_in_turn(self):
+        if TurningSidewalk.is_before_end_of_edge(self.str_sidewalks[0].edge.coords, self.intersection) and \
+            TurningSidewalk.is_before_end_of_edge(self.str_sidewalks[1].edge.coords, self.intersection):
+            # if the intersection point is within the two end points
+            
+            if not TurningSidewalk.is_before_begin_of_edge(self.str_sidewalks[0].edge.coords, self.intersection):
+                # if the intersection point is within the first edge
+                self.way[1] = TurningSidewalk.FixedPoint(self.intersection)
+                # if it is also inside the second edge, we remove the supplementary point
+                if not TurningSidewalk.is_before_begin_of_edge(self.str_sidewalks[1].edge.coords, self.intersection):
+                    del self.way[2]
+            else:
+                if not TurningSidewalk.is_before_begin_of_edge(self.str_sidewalks[1].edge.coords, self.intersection):
+                    # if the intersection point is within the second edge
+                    self.way[2] = TurningSidewalk.FixedPoint(self.intersection)
+                else:
+                    if self.turn_shape == TurningSidewalk.TurnShape.STRAIGHT_ANGLE:
+                        # we add a fixed point
+                        self.way.insert(2, TurningSidewalk.FixedPoint(self.intersection))
+                    else:
+                        # we add a flexible point
+                        self.way.insert(2, TurningSidewalk.FlexiblePoint(self.intersection))
+
+
+    def is_sidewalk_edge(self, node1, node2):
+        tags = u.Utils.get_initial_edge_tags(self.cr_input, node1, node2, True)
+        return tags != None and (tags["left_sidewalk"] == str(self.id) or tags["right_sidewalk"] == str(self.id))
+
+    def find_next_point_on_original_path(self, path):
+        last = path[-1]
+        previous = path[-2]
+
+        # for all neighbour of the last point
+        for nb in self.osm_input[last]:
+            if nb != previous and self.is_sidewalk_edge(nb, last):
+                return nb
+        
+        print("Error: cannot found a point along the sidewalk")
+        return None
+
+
+    def compute_original_path(self):
+        # find all edges of the original graph that are part of the sidewalk
+        polybranch1 = self.str_sidewalks[0].get_polybranch()
+        polybranch2 = self.str_sidewalks[1].get_polybranch()
+        
+        # initialize the final path with the first polybranch
+        self.original_path = polybranch1[::-1]
+        while self.original_path[-1] != polybranch2[0]:
+            self.original_path.append(self.find_next_point_on_original_path(self.original_path))
+            if self.original_path[-1] == None:
+                # error: no continuity (should not be possible)
+                self.original_path = None
+                return
+        
+        # add the final part
+        self.original_path += polybranch2[1:]
+        self.original_path_linestring = [(self.osm_input.nodes[x]["x"], self.osm_input.nodes[x]["y"]) for x in self.original_path]
 
-        # first check for basic interesction
-        middle_bevel = Point(self.get_middle_bevel())
-        if buffered_osm.intersects(middle_bevel):
-            self.build_beveled_turn()
+
+    def project_on_original_path(self, point):
+        if isinstance(point, TurningSidewalk.Point):
+            p = point.coord
         else:
-            # otherwise build a more complex turn
-            edge = LineString((middle_bevel, middle_sw))
+            p = point
+        nearest = shapely.ops.nearest_points(LineString(self.original_path_linestring), Point(p))
+        return nearest[0]
+
+
+    def estimate_curvilign_location_by_projection(self, point):
+        proj = self.project_on_original_path(point)
+
+        location = 0.0
+
+        for x, y in zip(self.original_path_linestring, self.original_path_linestring[1:]):
+            if u.Utils.is_in_edge(proj, x, y):
+                location += u.Utils.edge_length(x, proj)
+                break
+            else:
+                location += u.Utils.edge_length(x, y)
+
+        return location
+
+
+    def compute_curvilign_locations(self):
+        for idp, current in enumerate(self.way):
+            self.way[idp].set_curvilign_position(self.estimate_curvilign_location_by_projection(current))
+
+
+    def build_initial_turn(self):
+        # create turn with the 4 initial points
+        self.build_initial_turn_basic()
+
+        if self.turn_shape != TurningSidewalk.TurnShape.BEVELED:
+            # compute middle point
+            self.intersection = self.get_intersection()
+
+            # create the initial turn
+            if not self.intersection.is_empty:
+                # if there is an intersection point
+                self.add_intersection_point_in_turn()
+
+
+        # compute the corresponding path in the OSM graph
+        self.compute_original_path()
+
+        # compute curvilign locations
+        self.compute_curvilign_locations()
+
+    def add_crossings(self):
+        # for each sidewalk point
+        for c in self.crossings:
+            # identify its curvilign coordinate in the OSM path
+            curvPos = self.estimate_curvilign_location_by_projection(c.get_location())
+            # get location on the sidewalk
+            location = c.get_location_on_sidewalk(self.id)
+            # create the crossing point
+            p = TurningSidewalk.CrossingPoint(location, curvPos)
+
+            # find the good location along the way
+            cid = 0
+            while self.way[cid].curvPos < curvPos:
+                cid += 1
+                if cid >= len(self.way):
+                    break
             
-            elements = buffered_osm.boundary.intersection(edge)
-            if not elements.is_empty:
-                nearest = shapely.ops.nearest_points(middle_bevel, elements)
-                self.build_beveled_turn(nearest[1])
+            if cid != 0 and abs(curvPos - self.way[cid - 1].curvPos) < self.epsilon_for_merging:
+                # replace the existing node by the crossing
+                self.way[cid - 1] = p
+            elif cid < len(self.way) and abs(curvPos - self.way[cid].curvPos) < self.epsilon_for_merging:
+                # replace the existing node by the crossing
+                self.way[cid] = p
+            else:
+                # add it to the sidewalk
+                self.way.insert(cid, p)
+
+
+    def adjust_flexible_points(self):
+        buffered_osm = u.Utils.get_buffered_osm(self.osm_input, self.distance_kerb_footway)
+
+        for pred, point, next in zip(self.way, self.way[1:], self.way[2:]):
+            if point.flexible:
+                middle_sw = point.coord
+                
+                # first check for basic intersection
+                middle_bevel = Point([(x + y) / 2 for x, y in zip(pred.coord, next.coord)])
+
+                if not buffered_osm.intersects(middle_bevel):
+                    # build a more complex turn
+                    edge = LineString((middle_bevel, middle_sw))
+                    
+                    elements = buffered_osm.boundary.intersection(edge)
+                    if not elements.is_empty:
+                        nearest = shapely.ops.nearest_points(middle_bevel, elements)
+                        point.coord = (nearest[1].x, nearest[1].y)
 
 
     def branch_ids(self):
         return [x.description["id"] for x in self.str_sidewalks]
     
 
     def sidewalk_id(self):
@@ -268,61 +465,38 @@
         return u.Utils.norm_and_dot(u.Utils.vector(edge[0], edge[1]), u.Utils.vector(edge[1], node)) < 0
 
 
     def is_before_begin_of_edge(edge, node):
         return u.Utils.norm_and_dot(u.Utils.vector(edge[0], edge[1]), u.Utils.vector(edge[0], node)) < 0
 
 
-    def build_simple_turn(self):
-        sw1 = np.asarray(self.str_sidewalks[0].edge.coords)
-        sw2 = np.asarray(self.str_sidewalks[1].edge.coords)
-        self.intersection = self.get_intersection()
-        if not self.intersection.is_empty and (TurningSidewalk.is_before_end_of_edge(self.str_sidewalks[0].edge.coords, self.intersection) and \
-           TurningSidewalk.is_before_end_of_edge(self.str_sidewalks[1].edge.coords, self.intersection)) :
-            self.way = LineString([sw1[1], self.intersection, sw2[1]])
-            self.is_flexible_way = TurningSidewalk.is_before_begin_of_edge(self.str_sidewalks[0].edge.coords, self.intersection) and \
-                                    TurningSidewalk.is_before_begin_of_edge(self.str_sidewalks[1].edge.coords, self.intersection)
-        else:
-            self.way = None
-            self.is_flexible_way = True
-
-
-    def build_beveled_turn(self, middle = None):
-        sw1 = np.asarray(self.str_sidewalks[0].edge.coords)
-        sw2 = np.asarray(self.str_sidewalks[1].edge.coords)
-        if middle is None:
-            self.way = LineString(np.concatenate((sw1[::-1], sw2)))
-        else:
-            self.way = LineString(np.concatenate((sw1[::-1], [middle.coords[0]], sw2)))
-
-
     def as_array(self):
-        return np.asarray(self.way.coords)
+        return np.asarray([x.coord for x in self.way])
 
 
     def buffer(self, size):
         return self.way.buffer(size)
 
 
     def getGeometry(self):
-        return self.way
+        return LineString([x.coord for x in self.way])
 
 
     def getOSMIds(self):
         return ";".join([x.getOSMIds() for x in self.str_sidewalks])
 
     def toGDFSidewalks(sidewalks):
         d = {'type': [], 'osm_id': [], 'geometry': []}
 
         for s in sidewalks:
             d["type"].append("sidewalk")
             d["osm_id"].append(s.getOSMIds())
             d["geometry"].append(s.getGeometry())
 
-        return geopandas.GeoDataFrame(d, crs=2154)
+        return geopandas.GeoDataFrame(d, crs=2154, geometry="geometry")
 
 
 class TrafficIsland:
 
     def __init__(self, edgelist, osm_input, cr_input):
         self.edgelist = [list(map(int, x.split(";"))) for x in edgelist]
         self.osm_input = osm_input
@@ -489,16 +663,14 @@
 
     def build_polylines_from_section(self, section):
 
         edges = [e for e in zip(section, section[1:]) if e[0] != e[1]]
         outside = list(locate(edges, lambda e: not u.Utils.edge_in_osm(e[0], e[1], self.osm_input)))
 
         if len(outside) != 0:
-            print(outside)
-            print(section)
             side1 = section[0:outside[0] + 1]
             side2 = section[outside[-1] + 1:]
             side2.reverse()
             return u.Utils.pathid_to_pathcoords(side1, self.osm_input), u.Utils.pathid_to_pathcoords(side2, self.osm_input)
         else:
             # use length to split
             path = LineString(u.Utils.pathid_to_pathcoords(section, self.osm_input))
@@ -618,125 +790,288 @@
                     d["geometry"].append(g)
 
         return geopandas.GeoDataFrame(d, crs=2154)
 
 
 class Crossing:
 
-    def __init__(self, node_id, osm_input):
+    # The crossing will be oriented such that it goes from the sidewalk
+    # with the smallest ID to the sidewalk with the largest one.
+    # If there is an island in one side, this sidewalk comes first.
+    # If there are two islands, they are ordered in increasing ID order.
+
+    def __init__(self, node_id, osm_input, cr_input, osm_input_oriented, distance_kerb_footway):
 
         self.node_id = node_id
+
         self.osm_input = osm_input
+        self.cr_input = cr_input
+        self.osm_input_oriented = osm_input_oriented
+        self.distance_kerb_footway = distance_kerb_footway
 
         self.island_width = 0.50 # cm
 
         self.compute_location()
-        self.compute_orientation()
+
+        self.compute_way_orientations()
+
+        if len(self.roadway_nodes) > 0:
+
+            self.compute_footway_orientations()
+
+            self.flip_orientation_if_required()
+
+            self.compute_final_orientation()
+
+            # split adjacent ways in two groups
+            self.compute_adjacent_ways_ditribution()
+
 
         self.compute_crossing_profile()
 
+
+    def get_adjacent_border_from_way(self, tags, side):
+        sidewalk_key = side + "_sidewalk"
+        island_key = side + "_island"
+
+        if sidewalk_key in tags and isinstance(tags[sidewalk_key], str) and tags[sidewalk_key] != "":
+            return tags[sidewalk_key], "sidewalk"
+        elif island_key in tags and isinstance(tags[island_key], str) and tags[island_key] != "":
+            return tags[island_key], "island"
+        else:
+            return None, ""
+
+    def get_adjacent_border(self, crossing_orientation):
+        # for each adjacent way, compute the angle with the crossing orientation
+        orientations = [math.atan2(-x[1], x[0]) for x in self.build_vectors(self.roadway_nodes)]
+        angles = [x - crossing_orientation for x in orientations]
+        positive_angles = [x if x > 0 else x + 2 * math.pi if x > - 2 * math.pi else x + 4 * math.pi for x in angles]
+        # find next way by orientation
+        idx = positive_angles.index(min(positive_angles))
+        next_node = self.roadway_nodes[idx]
+        
+        # get tags
+        tags = u.Utils.get_initial_edge_tags(self.cr_input, self.node_id, next_node, True)
+
+        if tags is None:
+            # if tags are not defined, the crossing is located in border of the input segmentation, we choose the 
+            # opposite direction to get sidewalk information
+
+            idx = positive_angles.index(max(positive_angles))
+            next_node = self.roadway_nodes[idx]
+
+            tags = u.Utils.get_initial_edge_tags(self.cr_input, self.node_id, next_node, True)
+
+            side = "left" if str(next_node) != str(tags["osm_node_ids"][0]) else "right"
+
+            return self.get_adjacent_border_from_way(tags, side)
+        else:
+            
+            # identify the adjacent border
+            side = "right" if str(next_node) != str(tags["osm_node_ids"][0]) else "left"
+
+            return self.get_adjacent_border_from_way(tags, side)
+
+
+    def flip_orientation_if_required(self):
+        # compute the island or sidewalk for the two footways_orientations
+        id1, type1 = self.get_adjacent_border(self.footways_orientations[0])
+        id2, type2 = self.get_adjacent_border(self.footways_orientations[1])
+
+        self.sides = [(id1, type1), (id2, type2)]
+        if (self.sides[0] == self.sides[1]):
+            print("ERROR: two sides with the same sidewalk or island")
+        # check if oriented in the inverted direction
+        if type1 == type2:
+            inverted = int(id1) > int(id2)
+        else:
+            inverted = type1 == "island"
+
+        # if required, invert the orientations
+        if inverted:
+            self.footways_orientations = self.footways_orientations[::-1]
+            self.sides = self.sides[::-1]
+
+    # get ID of the sidewalks adjacent to this crossing
+    def get_sidewalk_ids(self):
+        return [x[0] for x in self.sides if x[1] == "sidewalk"]
+
+
+    def compute_way_orientations(self):
+        self.roadway_nodes = self.get_adjacent_roadways_nodes()
+
+        vectors = self.build_vectors(self.roadway_nodes)
+        self.way_orientations = sorted([math.atan2(-x[1], x[0]) for x in vectors])
+
+
+    def compute_footway_orientations(self):
+        self.footway_nodes = self.get_adjacent_footways_nodes()
+
+        if len(self.footway_nodes) > 2:
+            print("Error: bad number of footways:", len(self.footway_nodes))
+            self.footway_orientations = []
+        if len(self.footway_nodes) != 0:
+            vector_footways = self.build_vectors(self.footway_nodes)
+            self.footways_orientations = sorted([math.atan2(-x[1], x[0]) for x in vector_footways])
+        else:
+            # guess the correct split a maximum angle heuristic
+            angle_with_pred = [ a - b for a, b in zip(self.way_orientations, [self.way_orientations[-1]- 2 * math.pi] + self.way_orientations)]
+            max_id = angle_with_pred.index(max(angle_with_pred))
+            pred = max_id - 1
+            if pred < 0:
+                pred = len(self.way_orientations) - 1
+            self.footways_orientations = [u.Utils.angle_mean(self.way_orientations[max_id], self.way_orientations[pred])]
+        
+        # if required, add the opposite orientation
+        if len(self.footways_orientations) == 1:
+            opposite = self.footways_orientations[0] + math.pi
+            if opposite > math.pi:
+                opposite -= 2 * math.pi
+            self.footways_orientations.append(opposite)
+
+    def compute_adjacent_ways_ditribution(self):
+        # set angles up to angle1 using modulo 2pi 
+        angle1 = self.footways_orientations[0]
+        angle2 = self.footways_orientations[1] 
+        if angle2 < angle1:
+            angle2 += 2 * math.pi
+        way_orientations_unfold = [a if a > angle1 else a + 2 * math.pi for a in self.way_orientations]
+
+        # identify the side of each way wrt the two footways
+        way_side = [0 if a < angle2 else 1 for a in way_orientations_unfold]
+        ways_and_orientations = list(zip(self.roadway_nodes, way_side))
+
+        # shift list to reach the angle1 orientation
+        while ways_and_orientations[0][1] == ways_and_orientations[-1][1]:
+            ways_and_orientations = ways_and_orientations[1:] + ways_and_orientations[:1]
+
+        # finally build the ordered list of ways on each side of the footways
+        self.ways_side1 = [w for w, s in ways_and_orientations if s == 0]
+        self.ways_side2 = [w for w, s in ways_and_orientations if s == 1]
+        
+
+    def compute_crossing_profile_oneside(self, ways, invert):
+        # TODO: improve this naive merge where the sequence is not really computed
+        # assuming that there is only one set of backward lanes and one set of forward lanes
+        nb_backward = 0
+        nb_forward = 0
+        total_width = 0
+        for nw in ways:
+            if nw in self.osm_input[self.node_id]:
+                edge = self.osm_input[self.node_id][nw][0]
+                nb_b, nb_f, w = u.Utils.evaluate_way_composition(edge)
+            else:
+                edge = self.osm_input[nw][self.node_id][0]
+                nb_f, nb_b, w = u.Utils.evaluate_way_composition(edge)
+            nb_backward += nb_b
+            nb_forward += nb_f
+            total_width += w * (nb_f + nb_b)
+
+
+        if invert:
+            return nb_forward, nb_backward, total_width / (nb_forward + nb_backward)
+        else:
+            return nb_backward, nb_forward, total_width / (nb_forward + nb_backward)
+
+
     def compute_crossing_profile(self):
+        # TODO: improve this naive approach implemented in this fonction
+        # where there is only two directions (island being only between both directions)
+
         self.has_island = "crossing:island" in self.osm_input.nodes[self.node_id] and self.osm_input.nodes[self.node_id]["crossing:island"] == "yes"
-        car_way = u.Utils.get_adjacent_road_edge(self.node_id, self.osm_input)
-        if car_way != None:
-            nb_backward, nb_forward, width = u.Utils.evaluate_way_composition(car_way)
-            self.nb_lanes_backward = nb_backward
-            self.nb_lanes_forward = nb_forward
-            self.lane_width = width
-        else:
-            self.nb_lanes_backward = 0
-            self.nb_lanes_forward = 0
-            self.lane_width = 0
+
+        # for each side, compute the distribution
+        profile1 = self.compute_crossing_profile_oneside(self.ways_side1, False)
+        profile2 = self.compute_crossing_profile_oneside(self.ways_side2, True)
+
+        # choose the largest side as the final profile
+        nbside1 = profile1[0] + profile1[1]
+        nbside2 = profile2[0] + profile2[1]
+
+        if nbside1 > nbside2:
+            self.nb_lanes_backward = profile1[0]
+            self.nb_lanes_forward = profile1[1]
+        else:
+            self.nb_lanes_backward = profile2[0]
+            self.nb_lanes_forward = profile2[1]
+
+        # use the maximum width
+        self.lane_width = max(profile1[2], profile2[2])
+
 
     def compute_location(self):
         self.x = self.osm_input.nodes[self.node_id]["x"]
         self.y = self.osm_input.nodes[self.node_id]["y"]
 
 
-    def compute_orientation(self):
-        footways = self.get_adjacent_footways_nodes()
-        if len(footways) != 0:
-            self.bearing = self.compute_parallel_orientation(footways)
-            self.bearing_confidence = False
-        else:
-            roadways = self.get_adjacent_roadways_nodes()
-            if len(roadways) == 0:
-                print("Error: no adjacent road")
-                for x in self.osm_input[self.node_id]:
-                    print(" ", self.osm_input[self.node_id][x][0])
-                self.bearing_confidence = Fakse
-                self.bearing = 0
-            else:
-                self.bearing = self.compute_orthogonal_orientation(roadways)
-                self.bearing_confidence = True
-
+    def compute_final_orientation(self):
+        self.bearing = u.Utils.angle_mean(self.footways_orientations[0], math.pi + self.footways_orientations[1])
+        self.bearing_confidence = len(self.footway_nodes) != 0
 
     def get_adjacent_roadways_nodes(self):
-        # TODO: est-ce qu'on n'essayerait pas de prendre des nodes un peu plus loin sur les ways?
         return [x for x in self.osm_input[self.node_id] if u.Utils.is_roadway_edge(self.osm_input[self.node_id][x][0])]
 
 
     def get_adjacent_footways_nodes(self):
         return [x for x in self.osm_input[self.node_id] if u.Utils.is_footway_edge(self.osm_input[self.node_id][x][0])]
 
 
-    def compute_parallel_orientation(self, nodes):
-        vectors = self.build_vectors(nodes)
-        if len(vectors) == 1:
-            return math.atan2(vectors[0][1], vectors[0][0])
-        elif len(vectors) == 2:
-            return math.atan2(vectors[0][1] - vectors[1][1], vectors[0][0] - vectors[1][0])
-        elif len(vectors) == 3:
-            # compute the orientations (in gradient) and sort them
-            orientations = sorted([math.atan2(x[1], x[0]) for x in vectors])
-            # compute the difference between consecutive orientations
-            diff = [o[1] - o[0] for o in zip(orientations, orientations[1:] + orientations[:1])]
-            diff = [ o + 2 * math.pi if o < 0 else o for o in diff]
-            # identify the pair of branches with the smallest difference
-            branchID1 = diff.index(min(diff))
-            branchID2 = (branchID1 + 1) % len(vectors)
-            # identify the other one
-            otherBranchID = (branchID2 + 1) % len(vectors)
-            # compute a mean of the global orientation, considering the other branch as an opposite one
-            return u.Utils.angle_mean(u.Utils.angle_mean(orientations[branchID1], orientations[branchID2]), orientations[otherBranchID] + math.pi)
-        else:
-            print(vectors, [math.atan2(x[1], x[0]) for x in vectors])
-            print("Error: bad number of edges to compute a direction", len(vectors))
-
-    def compute_orthogonal_orientation(self, nodes):
-        bearing = self.compute_parallel_orientation(nodes)
-        bearing += math.pi / 2
-        if bearing > 2 * math.pi:
-            bearing -= 2 * math.pi
-        return bearing
-
     def build_vectors(self, nodes):
         return [u.Utils.normalized_vector(self.osm_input.nodes[self.node_id], self.osm_input.nodes[n]) for n in nodes]
 
     
-    def create_crossings(osm_input, cr_input, region = None):
-        return dict([(n, Crossing(n, osm_input)) for n in osm_input.nodes if 
-                      (region is None or region.contains(Point(osm_input.nodes[n]["x"], osm_input.nodes[n]["y"]))) and
+    def create_crossings(osm_input, cr_input, osm_input_oriented, distance_kerb_footway):
+        return dict([(n, Crossing(n, osm_input, cr_input, osm_input_oriented, distance_kerb_footway)) for n in osm_input.nodes if 
                       osm_input.nodes[n]["type"] == "input" and Crossing.is_crossing(n, cr_input)])
 
 
+    def is_inside(self, region):
+        return region.contains(Point(Point(self.osm_input.nodes[self.node_id]["x"], self.osm_input.nodes[self.node_id]["y"])))
 
     def is_crossing(node, cr_input):
         tags = u.Utils.get_initial_node_tags(cr_input, node)
         return tags and tags["type"] == "crosswalk"
 
 
     def get_line_representation(self, length = 1):
         x = self.osm_input.nodes[self.node_id]["x"]
         y = self.osm_input.nodes[self.node_id]["y"]
-        shiftx = math.cos(self.bearing) * length
+        shiftx = -math.cos(self.bearing) * length
         shifty = math.sin(self.bearing) * length
         return [(x - shiftx, y - shifty), (x, y), (x + shiftx, y + shifty)]
 
 
+    def get_location(self):
+        x = self.osm_input.nodes[self.node_id]["x"]
+        y = self.osm_input.nodes[self.node_id]["y"]
+        return (x, y)
+
+    
+    def is_first_side(self, id_sidewalk):
+        if self.sides[0][1] != "sidewalk":
+            return False
+        else:
+            return str(self.sides[0][0]) == str(id_sidewalk)
+
+
+    def get_location_on_sidewalk(self, id_sidewalk):
+        x = self.osm_input.nodes[self.node_id]["x"]
+        y = self.osm_input.nodes[self.node_id]["y"]
+
+        nb = self.nb_lanes_backward + self.nb_lanes_forward
+        length = nb * self.lane_width / 2 + self.distance_kerb_footway
+
+        bearing = self.footways_orientations[0 if self.is_first_side(id_sidewalk) else 1]
+
+        shiftx = -math.cos(bearing) * length
+        shifty = math.sin(bearing) * length
+        return (x + shiftx, y + shifty)
+
+ 
+
     def getGeometry(self):
         return Point(self.osm_input.nodes[self.node_id]["x"], self.osm_input.nodes[self.node_id]["y"])
 
     def getCrossingElements(self):
         nb = self.nb_lanes_backward + self.nb_lanes_forward
         start_shift = (nb - 1) * self.lane_width / 2
         total_width = nb * self.lane_width
@@ -748,15 +1083,15 @@
         elements = []
         x = self.osm_input.nodes[self.node_id]["x"]
         y = self.osm_input.nodes[self.node_id]["y"]
 
         # crossings
         for i in range(nb):
             shift = -start_shift + i * lane_width_effective + (self.island_width if self.has_island and i >= self.nb_lanes_forward else 0)
-            shiftx = math.cos(self.bearing) * shift
+            shiftx = -math.cos(self.bearing) * shift
             shifty = math.sin(self.bearing) * shift
             elements.append({ "type": "crossing",
                               "geometry": Point(x + shiftx, y + shifty),
                               "lane_orientation": "forward" if i < self.nb_lanes_forward else "backward",
                               "lane_width": lane_width_effective })
 
         # separators
@@ -764,15 +1099,15 @@
         for i in range(nb - 1):
             shift = -start_shift + i * lane_width_effective
             if self.has_island:
                 if i + 1== self.nb_lanes_forward:
                     shift += self.island_width / 2
                 elif i + 1 > self.nb_lanes_forward:
                     shift += self.island_width
-            shiftx = math.cos(self.bearing) * shift
+            shiftx = -math.cos(self.bearing) * shift
             shifty = math.sin(self.bearing) * shift
             island = self.has_island and i + 1 == self.nb_lanes_backward
             elements.append({ "type": "traffic_island" if island else "lane_separator",
                               "geometry": Point(x + shiftx, y + shifty),
                               "lane_orientation": None,
                               "lane_width": self.island_width if island else 0 })
 
@@ -797,21 +1132,21 @@
         for cid in crossings:
             c = crossings[cid]
             if details:
                 for e in c.getCrossingElements():
                     d["type"].append(e["type"])
                     d["osm_id"].append(c.node_id)
                     d["geometry"].append(e["geometry"])
-                    d["orientation"].append(c.bearing)
+                    d["orientation"].append(-c.bearing + math.pi / 2)
                     d['lane_orientation'].append(e["lane_orientation"])
                     d["orientation_confidence"].append(c.bearing_confidence)
                     d["lane_width"].append(e["lane_width"])
             else:
                 d["type"].append("crossing")
-                d["orientation"].append(c.bearing)
+                d["orientation"].append(-c.bearing + math.pi / 2)
                 d["orientation_confidence"].append(c.bearing_confidence)
                 d["osm_id"].append(c.node_id)
                 d["geometry"].append(c.getGeometry())
                 d["has_island"].append(c.has_island)
                 d["nb_lanes_backward"].append(c.nb_lanes_backward)
                 d["nb_lanes_forward"].append(c.nb_lanes_forward)
                 d["lane_width"].append(c.lane_width)
@@ -845,37 +1180,43 @@
         for index, elem in self.cr_input.iterrows():
             if elem["type"] in ["branch", "way"] and elem["name"] != self.name:
                 ids = list(map(int, elem["osm_node_ids"]))
                 result.append(ids)
         return result
 
 
-    def build_two_sidewalks(self):
-        # the shift corresponds to half the width of the street
-        shift = self.width / 2
+    def shift_middle_line(self, shifts, direction):
+        edges = [self.middle_line.parallel_offset(s, direction) for s in shifts]
+        return LineString([edges[0].coords[0], edges[1].coords[1]])
+
+    def build_two_sidewalks(self, use_fixed_width_on_branches):
+        from statistics import mean
+        # the shifts corresponds to half the widths of the street
+        shifts = [x / 2 for x in self.widths]
+
+        if use_fixed_width_on_branches:
+            shifts = [mean(shifts) for x in shifts]
         
         # compute the two lines (one in each side)
-        result = [StraightSidewalk(self.middle_line.parallel_offset(shift, "left"),
-                                   self.sides[0].edge_tags,
-                                   self.sides[0].same_osm_orientation,
-                                   "left",
-                                   self.sides[0].is_crossing_inner_node()),
-                   StraightSidewalk(self.middle_line.parallel_offset(shift, "right"),
-                                   self.sides[1].edge_tags,
-                                   self.sides[1].same_osm_orientation,
-                                   "right",
-                                   self.sides[1].is_crossing_inner_node())]
+        result = [StraightSidewalk(self.shift_middle_line(shifts, "left"),
+                                   self.sides[0],
+                                   "left"),
+                   StraightSidewalk(self.shift_middle_line(shifts, "right"),
+                                   self.sides[1],
+                                   "right")]
+
+        # shift them if required
         buf = u.Utils.get_edges_buffered_by_osm(self.get_other_edges(), self.osm_input, self.distance_kerb_footway).boundary
         for i, s in enumerate(result):
             if s.edge.intersects(buf):
                 intersections = s.edge.intersection(buf)
                 if not intersections.is_empty and isinstance(intersections, Point):
                     result[i].update_first_node(intersections)
 
-        return result
+        self.sidewalks = result
 
 
 
     # maximum distance between two extremity points of the ways
     def get_initial_branche_width(self):
         edges = []
         distance = 0
@@ -890,21 +1231,34 @@
                         distance = d
             edges.append(emeters)
 
         return distance
 
 
     def build_middle_way(self):
-            self.middle_line = StraightWay.build_middle_line(self.sides[0], self.sides[1])
+        self.middle_line = StraightWay.build_middle_line(self.sides[0], self.sides[1])
             
     
-    def compute_width(self):
-        self.width = self.sides[0].evaluate_width_way(self.osm_input) / 2 + \
-                    self.sides[1].evaluate_width_way(self.osm_input) / 2 + \
-                    self.get_initial_branche_width() + 2 * self.distance_kerb_footway
+    def compute_widths(self):
+        # for each extremity of the middle line
+        self.widths = []
+        for p in self.middle_line.coords:
+
+            # project it on each polybranches and select two furthest points
+            p1, e1 = self.sides[0].get_projection_on_polybranch(p)
+            p2, e2 = self.sides[1].get_projection_on_polybranch(p)
+
+            # for each point estimate the width of the way
+            interdistance = u.Utils.edge_length(p1, p2)
+            w1 = u.Utils.evaluate_width_way(self.osm_input[e1[0]][e1[1]][0]) / 2 + self.distance_kerb_footway
+            w2 = u.Utils.evaluate_width_way(self.osm_input[e2[0]][e2[1]][0]) / 2 + self.distance_kerb_footway
+
+            # compute the final width
+            self.widths.append(interdistance + w1 + w2)
+
 
     def build_sidewalk_straightways(self):
         # get the external simple ways (they are bordered by a sidewalk)
         self.simple_sides = [ w for w in self.ways if w.has_sidewalk()]
 
         if len(self.simple_sides) > 2:
             print("ERROR: more than two ways with a sidewalk (", self.name, ")")
@@ -927,26 +1281,25 @@
 
         # build their extension as straightline
         self.sides = [StraightWay.build_from_simpleway(self.simple_sides[0], self.osm_input, True), # always choose the left
                        StraightWay.build_from_simpleway(self.simple_sides[1], self.osm_input, False)] # always choose the right
 
 
 
-    def get_sidewalks(self):
+    def get_sidewalks(self, use_fixed_width_on_branches):
 
         self.build_sidewalk_straightways()
 
         # TODO: shift each extremity of each sidewalk wrt the estimated width of each extremity
 
-        # TODO: remove this
         self.build_middle_way()
 
-        self.compute_width()
+        self.compute_widths()
 
-        self.sidewalks = self.build_two_sidewalks()
+        self.build_two_sidewalks(use_fixed_width_on_branches)
 
         return self.sidewalks
 
     
     def getGeometry(self):
         return self.middle_line
```

### Comparing `crossroads-schematization-0.0.9/crschem/crossroad_schematization.py` & `crossroads-schematization-0.1.0/crschem/crossroad_schematization.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,27 +34,36 @@
         'foot'
     ]
 
     # If the OSM data has been previously loaded, do not load it again
     def __init__(self, cr_input, 
                  osm_oriented = None,
                  osm_unoriented = None,
+                 ignore_crossings_for_sidewalks = False,
+                 use_fixed_width_on_branches = False,
+                 turn_shape = c.TurningSidewalk.TurnShape.ADJUSTED_ANGLE,
                  osm_buffer_size_meters = 200, 
                  distance_kerb_footway = 0.5,
                  white_space_meter = 1.5):
         self.osm_buffer_size_meters = osm_buffer_size_meters
         self.distance_kerb_footway = distance_kerb_footway
         self.white_space_meter = white_space_meter
         self.cr_input = cr_input
+        self.ignore_crossings_for_sidewalks = ignore_crossings_for_sidewalks
+        self.use_fixed_width_on_branches = use_fixed_width_on_branches
+        self.turn_shape = turn_shape
 
         self.load_osm(osm_oriented, osm_unoriented)
 
 
     def build(latitude, longitude,
               C0, C1, C2,
+              ignore_crossings_for_sidewalks = False,
+              use_fixed_width_on_branches = False,
+              turn_shape = c.TurningSidewalk.TurnShape.ADJUSTED_ANGLE,
               verbose = True,
               ignore_cache = False,
               overpass = False,
               log_files = False):
 
         import crseg.segmentation as cseg
         import crseg.utils as cru
@@ -106,15 +115,18 @@
         cr_input = geopandas.read_file(tmp2.name)
 
         if log_files:
             print("Model:", tmp2.name)
         else:
             os.unlink(tmp2.name)
 
-        return CrossroadSchematization(cr_input, G_init)
+        return CrossroadSchematization(cr_input, G_init, 
+                                        ignore_crossings_for_sidewalks=ignore_crossings_for_sidewalks, 
+                                        use_fixed_width_on_branches=use_fixed_width_on_branches,
+                                        turn_shape=turn_shape)
 
     def is_valid_model(self):
         for index, elem in self.cr_input.iterrows():
             if elem["type"] in ["branch", "way"]:                
                 for side in ["left", "right"]:
                     for obj in ["_island", "_sidewalk"]:
                         key = side + obj
@@ -127,41 +139,52 @@
         return True
 
 
     def process(self):
         self.label_osm_from_input()
         
         # grouping ways by branch
+        print("Creating branches")
         self.build_branches()
 
         # compute for each branch two long edges *S1* and *S2* corresponding to the sidewalks:
+        print("Creating sidewalks")
         self.build_sidewalks()
 
+        # add pedestrian crossings
+        print("Creating crossings")
+        self.crossings = c.Crossing.create_crossings(self.osm_input, self.cr_input, 
+                                                     self.osm_input_oriented,
+                                                     self.distance_kerb_footway)
+
         # assemble sidewalks
+        print("Assembling sidewalks")
         self.assemble_sidewalks()
 
         # compute inner region 
+        print("Computing inner region")
         self.build_inner_region()
 
+        # filtering crossings
+        print("Filtering crossings")
+        self.filter_crossings()
         # build traffic islands
+        print("Building traffic islands")
         self.build_traffic_islands()
 
-        # add pedestrian crossings
-        print("Creating crossings")
-        self.crossings = c.Crossing.create_crossings(self.osm_input, self.cr_input, self.inner_region)
-
         print("Computing traffic island shape")
         # compute traffic island shape
         for island in self.traffic_islands:
             island.compute_generalization(self.crossings, self.inner_region)
 
-        # add a supplementary point on the sidewalks where a crossing is reaching it
-        # to preserve the estimated distance
-        # TODO
 
+    def filter_crossings(self):
+        def function_is_inside(pair):
+            return pair[1].is_inside(self.inner_region)
+        self.crossings = dict(filter(function_is_inside, self.crossings.items()))
 
     def load_osm(self, osm_oriented, osm_unoriented):
         # load OSM data from the same crossroad (osmnx:graph)
         bounds = self.cr_input.total_bounds
         center = [(bounds[1] + bounds[3]) / 2, (bounds[0] + bounds[2]) / 2]
 
         if osm_oriented is None:
@@ -223,24 +246,22 @@
                 n2 = osm_n2 if n1 == osm_n1 else osm_n1
                 e = u.Utils.get_initial_edge_tags(self.cr_input, osm_n1, osm_n2)
                 if e is not None:
                     id = e["id"]
                     bname = e["name"]
                     if not id in self.branches:
                         self.branches[id] = c.Branch(bname, id, self.osm_input, self.cr_input, self.distance_kerb_footway)
-                    self.branches[id].add_way(c.SimpleWay(n1, n2, e, osm_n1 == n1,
-                                                        c.Crossing.is_crossing(n1, self.cr_input)))
+                    self.branches[id].add_way(c.SimpleWay(n1, n2, e, osm_n1 == n1))
 
 
     def build_sidewalks(self):
-        print("Building sidewalks")
         self.sidewalks = {}
         
         for bid in self.branches:
-            self.sidewalks[bid] = self.branches[bid].get_sidewalks()
+            self.sidewalks[bid] = self.branches[bid].get_sidewalks(self.use_fixed_width_on_branches)
 
     
     def get_sidewalk_ids(self):
         result = set()
         for bid in self.sidewalks:
             if self.sidewalks[bid]:
                 for sw in self.sidewalks[bid]:
@@ -253,26 +274,40 @@
         for bid in self.sidewalks:
             if self.sidewalks[bid]:
                 for sw in self.sidewalks[bid]:
                     if sw.sidewalk_id() == sid:
                         result.append(sw)
         return result
 
+    def get_crossings_by_sidewalks_ids(self, sid):
+        result = []
+        for cid in self.crossings:
+            if str(sid) in self.crossings[cid].get_sidewalk_ids():
+                result.append(self.crossings[cid])
+        return result
+
+
     def assemble_sidewalks(self):
-        print("Assembling sidewalks")
         self.cr_input.replace('', np.nan, inplace=True)
         original_sidewalks_ids = self.get_sidewalk_ids()
         self.merged_sidewalks = []
 
+        # TODO: find crossings that should be part of the sidewalks and
+        # integrate them to the final shape
+
         for sid in original_sidewalks_ids:
-            self.merged_sidewalks.append(c.TurningSidewalk(self.get_sidewalks_by_id(sid), self.osm_input, self.distance_kerb_footway))
+            self.merged_sidewalks.append(c.TurningSidewalk(sid,
+                                                            self.get_sidewalks_by_id(sid), 
+                                                            self.get_crossings_by_sidewalks_ids(sid),
+                                                            self.osm_input, self.cr_input, self.distance_kerb_footway,
+                                                            self.ignore_crossings_for_sidewalks,
+                                                            self.turn_shape))
 
 
     def build_inner_region(self):
-        print("Building inner region")
         open_sides = copy.copy(self.merged_sidewalks)
 
         # order sidewalks
         final_shape = [(open_sides.pop(), True)]
         while len(open_sides) != 0:
             cid = final_shape[-1][0].branch_ids()[1 if final_shape[-1][1] else 0]
             found = False
@@ -294,15 +329,14 @@
         final_shape = list(itertools.chain(*[list(x) for x in final_shape]))
         final_shape.append(final_shape[0])
 
         self.inner_region = Polygon(final_shape)
 
 
     def build_traffic_islands(self):
-        print("Building traffic island")
         traffic_islands_edges = {}
 
         # first group edges by island id
         for index, elem in self.cr_input.iterrows():
             if elem["type"] in ["branch", "way"]:
                 for side in ["left", "right"]:
                     id = u.Utils.get_number_from_label(elem[side + "_island"])
@@ -492,15 +526,16 @@
                     x, y = sw.edge.xy
 
                     plt.plot(x, y, color = colors[sw.sidewalk_id() % len(colors)])
                     plt.plot(x[0],y[0],'ok')
 
         if merged_sidewalks:
             for sw in self.merged_sidewalks:
-                x, y = sw.way.xy
+                x = [p.coord[0] for p in sw.way]
+                y = [p.coord[1] for p in sw.way]
                 plt.plot(x, y, color = colors[sw.sidewalk_id() % len(colors)], linewidth=3)
 
         if exact_islands:
             for i, sw in enumerate(self.traffic_islands):
                 if sw.is_reachable or not only_reachable_islands:
                     x, y = sw.get_linearring().xy
                     plt.plot(x, y, color = colors[i % len(colors)], linewidth=1)
```

### Comparing `crossroads-schematization-0.0.9/crschem/processing.py` & `crossroads-schematization-0.1.0/crschem/processing.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.0.9/crschem/resources/crossing.svg` & `crossroads-schematization-0.1.0/crschem/resources/crossing.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.0.9/crschem/resources/rendering-areas.qml` & `crossroads-schematization-0.1.0/crschem/resources/rendering-areas.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.0.9/crschem/resources/rendering-nodes-crossings.qml` & `crossroads-schematization-0.1.0/crschem/resources/rendering-nodes-crossings.qml`

 * *Files 1% similar despite different names*

```diff
@@ -687,1141 +687,1140 @@
 00002ae0: 653d 224d 6170 223e 0a20 2020 2020 2020  e="Map">.       
 00002af0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
 00002b00: 6f6e 206e 616d 653d 2261 6374 6976 6522  on name="active"
 00002b10: 2076 616c 7565 3d22 7472 7565 2220 7479   value="true" ty
 00002b20: 7065 3d22 626f 6f6c 222f 3e0a 2020 2020  pe="bool"/>.    
 00002b30: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
 00002b40: 7074 696f 6e20 6e61 6d65 3d22 6578 7072  ption name="expr
-00002b50: 6573 7369 6f6e 2220 7661 6c75 653d 2231  ession" value="1
-00002b60: 3830 202b 2028 2d26 7175 6f74 3b6f 7269  80 + (-&quot;ori
-00002b70: 656e 7461 7469 6f6e 2671 756f 743b 202f  entation&quot; /
-00002b80: 2070 6928 2929 202a 2031 3830 2220 7479   pi()) * 180" ty
-00002b90: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+00002b50: 6573 7369 6f6e 2220 7661 6c75 653d 2239  ession" value="9
+00002b60: 3020 2b20 282d 2671 756f 743b 6f72 6965  0 + (-&quot;orie
+00002b70: 6e74 6174 696f 6e26 7175 6f74 3b20 2f20  ntation&quot; / 
+00002b80: 7069 2829 2920 2a20 3138 3022 2074 7970  pi()) * 180" typ
+00002b90: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
 00002ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bb0: 203c 4f70 7469 6f6e 206e 616d 653d 2274   <Option name="t
-00002bc0: 7970 6522 2076 616c 7565 3d22 3322 2074  ype" value="3" t
-00002bd0: 7970 653d 2269 6e74 222f 3e0a 2020 2020  ype="int"/>.    
-00002be0: 2020 2020 2020 2020 2020 2020 3c2f 4f70              </Op
-00002bf0: 7469 6f6e 3e0a 2020 2020 2020 2020 2020  tion>.          
-00002c00: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
-00002c10: 6d65 3d22 6f75 746c 696e 6557 6964 7468  me="outlineWidth
-00002c20: 2220 7479 7065 3d22 4d61 7022 3e0a 2020  " type="Map">.  
-00002c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c40: 3c4f 7074 696f 6e20 6e61 6d65 3d22 6163  <Option name="ac
-00002c50: 7469 7665 2220 7661 6c75 653d 2274 7275  tive" value="tru
-00002c60: 6522 2074 7970 653d 2262 6f6f 6c22 2f3e  e" type="bool"/>
-00002c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002c80: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
-00002c90: 2265 7870 7265 7373 696f 6e22 2076 616c  "expression" val
-00002ca0: 7565 3d22 2671 756f 743b 6c61 6e65 5f77  ue="&quot;lane_w
-00002cb0: 6964 7468 2671 756f 743b 202a 2030 2e37  idth&quot; * 0.7
-00002cc0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00002cd0: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
-00002ce0: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
-00002cf0: 653d 2274 7970 6522 2076 616c 7565 3d22  e="type" value="
-00002d00: 3322 2074 7970 653d 2269 6e74 222f 3e0a  3" type="int"/>.
-00002d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d20: 3c2f 4f70 7469 6f6e 3e0a 2020 2020 2020  </Option>.      
-00002d30: 2020 2020 2020 2020 3c2f 4f70 7469 6f6e          </Option
-00002d40: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00002d50: 3c4f 7074 696f 6e20 6e61 6d65 3d22 7479  <Option name="ty
-00002d60: 7065 2220 7661 6c75 653d 2263 6f6c 6c65  pe" value="colle
-00002d70: 6374 696f 6e22 2074 7970 653d 2251 5374  ction" type="QSt
-00002d80: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-00002d90: 2020 2020 3c2f 4f70 7469 6f6e 3e0a 2020      </Option>.  
-00002da0: 2020 2020 2020 2020 3c2f 6461 7461 5f64          </data_d
-00002db0: 6566 696e 6564 5f70 726f 7065 7274 6965  efined_propertie
-00002dc0: 733e 0a20 2020 2020 2020 203c 2f6c 6179  s>.        </lay
-00002dd0: 6572 3e0a 2020 2020 2020 3c2f 7379 6d62  er>.      </symb
-00002de0: 6f6c 3e0a 2020 2020 2020 3c73 796d 626f  ol>.      <symbo
-00002df0: 6c20 6e61 6d65 3d22 3122 2066 6f72 6365  l name="1" force
-00002e00: 5f72 6872 3d22 3022 2066 7261 6d65 5f72  _rhr="0" frame_r
-00002e10: 6174 653d 2231 3022 2061 6c70 6861 3d22  ate="10" alpha="
-00002e20: 3122 2063 6c69 705f 746f 5f65 7874 656e  1" clip_to_exten
-00002e30: 743d 2231 2220 6973 5f61 6e69 6d61 7465  t="1" is_animate
-00002e40: 643d 2230 2220 7479 7065 3d22 6d61 726b  d="0" type="mark
-00002e50: 6572 223e 0a20 2020 2020 2020 203c 6461  er">.        <da
-00002e60: 7461 5f64 6566 696e 6564 5f70 726f 7065  ta_defined_prope
-00002e70: 7274 6965 733e 0a20 2020 2020 2020 2020  rties>.         
-00002e80: 203c 4f70 7469 6f6e 2074 7970 653d 224d   <Option type="M
-00002e90: 6170 223e 0a20 2020 2020 2020 2020 2020  ap">.           
-00002ea0: 203c 4f70 7469 6f6e 206e 616d 653d 226e   <Option name="n
-00002eb0: 616d 6522 2076 616c 7565 3d22 2220 7479  ame" value="" ty
-00002ec0: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
-00002ed0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00002ee0: 6f6e 206e 616d 653d 2270 726f 7065 7274  on name="propert
-00002ef0: 6965 7322 2f3e 0a20 2020 2020 2020 2020  ies"/>.         
-00002f00: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
-00002f10: 2274 7970 6522 2076 616c 7565 3d22 636f  "type" value="co
-00002f20: 6c6c 6563 7469 6f6e 2220 7479 7065 3d22  llection" type="
-00002f30: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-00002f40: 2020 2020 203c 2f4f 7074 696f 6e3e 0a20       </Option>. 
-00002f50: 2020 2020 2020 203c 2f64 6174 615f 6465         </data_de
-00002f60: 6669 6e65 645f 7072 6f70 6572 7469 6573  fined_properties
-00002f70: 3e0a 2020 2020 2020 2020 3c6c 6179 6572  >.        <layer
-00002f80: 2070 6173 733d 2230 2220 6c6f 636b 6564   pass="0" locked
-00002f90: 3d22 3022 2065 6e61 626c 6564 3d22 3122  ="0" enabled="1"
-00002fa0: 2063 6c61 7373 3d22 5369 6d70 6c65 4d61   class="SimpleMa
-00002fb0: 726b 6572 223e 0a20 2020 2020 2020 2020  rker">.         
-00002fc0: 203c 4f70 7469 6f6e 2074 7970 653d 224d   <Option type="M
-00002fd0: 6170 223e 0a20 2020 2020 2020 2020 2020  ap">.           
-00002fe0: 203c 4f70 7469 6f6e 206e 616d 653d 2261   <Option name="a
-00002ff0: 6e67 6c65 2220 7661 6c75 653d 2230 2220  ngle" value="0" 
-00003000: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
-00003010: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
-00003020: 7469 6f6e 206e 616d 653d 2263 6170 5f73  tion name="cap_s
-00003030: 7479 6c65 2220 7661 6c75 653d 2266 6c61  tyle" value="fla
-00003040: 7422 2074 7970 653d 2251 5374 7269 6e67  t" type="QString
-00003050: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00003060: 3c4f 7074 696f 6e20 6e61 6d65 3d22 636f  <Option name="co
-00003070: 6c6f 7222 2076 616c 7565 3d22 3233 322c  lor" value="232,
-00003080: 3835 2c30 2c32 3535 2220 7479 7065 3d22  85,0,255" type="
-00003090: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-000030a0: 2020 2020 2020 203c 4f70 7469 6f6e 206e         <Option n
-000030b0: 616d 653d 2268 6f72 697a 6f6e 7461 6c5f  ame="horizontal_
-000030c0: 616e 6368 6f72 5f70 6f69 6e74 2220 7661  anchor_point" va
-000030d0: 6c75 653d 2231 2220 7479 7065 3d22 5153  lue="1" type="QS
-000030e0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-000030f0: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
-00003100: 653d 226a 6f69 6e73 7479 6c65 2220 7661  e="joinstyle" va
-00003110: 6c75 653d 2262 6576 656c 2220 7479 7065  lue="bevel" type
-00003120: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-00003130: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-00003140: 206e 616d 653d 226e 616d 6522 2076 616c   name="name" val
-00003150: 7565 3d22 6c69 6e65 2220 7479 7065 3d22  ue="line" type="
-00003160: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-00003170: 2020 2020 2020 203c 4f70 7469 6f6e 206e         <Option n
-00003180: 616d 653d 226f 6666 7365 7422 2076 616c  ame="offset" val
-00003190: 7565 3d22 302c 3022 2074 7970 653d 2251  ue="0,0" type="Q
-000031a0: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
-000031b0: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
-000031c0: 6d65 3d22 6f66 6673 6574 5f6d 6170 5f75  me="offset_map_u
-000031d0: 6e69 745f 7363 616c 6522 2076 616c 7565  nit_scale" value
-000031e0: 3d22 3378 3a30 2c30 2c30 2c30 2c30 2c30  ="3x:0,0,0,0,0,0
-000031f0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00003200: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-00003210: 4f70 7469 6f6e 206e 616d 653d 226f 6666  Option name="off
-00003220: 7365 745f 756e 6974 2220 7661 6c75 653d  set_unit" value=
-00003230: 224d 4d22 2074 7970 653d 2251 5374 7269  "MM" type="QStri
-00003240: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
-00003250: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
-00003260: 6f75 746c 696e 655f 636f 6c6f 7222 2076  outline_color" v
-00003270: 616c 7565 3d22 3235 352c 3235 352c 3235  alue="255,255,25
-00003280: 352c 3235 3522 2074 7970 653d 2251 5374  5,255" type="QSt
-00003290: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-000032a0: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
-000032b0: 3d22 6f75 746c 696e 655f 7374 796c 6522  ="outline_style"
-000032c0: 2076 616c 7565 3d22 736f 6c69 6422 2074   value="solid" t
-000032d0: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
-000032e0: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-000032f0: 696f 6e20 6e61 6d65 3d22 6f75 746c 696e  ion name="outlin
-00003300: 655f 7769 6474 6822 2076 616c 7565 3d22  e_width" value="
-00003310: 3222 2074 7970 653d 2251 5374 7269 6e67  2" type="QString
-00003320: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00003330: 3c4f 7074 696f 6e20 6e61 6d65 3d22 6f75  <Option name="ou
-00003340: 746c 696e 655f 7769 6474 685f 6d61 705f  tline_width_map_
-00003350: 756e 6974 5f73 6361 6c65 2220 7661 6c75  unit_scale" valu
-00003360: 653d 2233 783a 302c 302c 302c 302c 302c  e="3x:0,0,0,0,0,
-00003370: 3022 2074 7970 653d 2251 5374 7269 6e67  0" type="QString
-00003380: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00003390: 3c4f 7074 696f 6e20 6e61 6d65 3d22 6f75  <Option name="ou
-000033a0: 746c 696e 655f 7769 6474 685f 756e 6974  tline_width_unit
-000033b0: 2220 7661 6c75 653d 2252 656e 6465 724d  " value="RenderM
-000033c0: 6574 6572 7349 6e4d 6170 556e 6974 7322  etersInMapUnits"
-000033d0: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-000033e0: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
-000033f0: 7074 696f 6e20 6e61 6d65 3d22 7363 616c  ption name="scal
-00003400: 655f 6d65 7468 6f64 2220 7661 6c75 653d  e_method" value=
-00003410: 2264 6961 6d65 7465 7222 2074 7970 653d  "diameter" type=
-00003420: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-00003430: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00003440: 6e61 6d65 3d22 7369 7a65 2220 7661 6c75  name="size" valu
-00003450: 653d 2233 2220 7479 7065 3d22 5153 7472  e="3" type="QStr
-00003460: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-00003470: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
-00003480: 2273 697a 655f 6d61 705f 756e 6974 5f73  "size_map_unit_s
-00003490: 6361 6c65 2220 7661 6c75 653d 2233 783a  cale" value="3x:
-000034a0: 302c 302c 302c 302c 302c 3022 2074 7970  0,0,0,0,0,0" typ
-000034b0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-000034c0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-000034d0: 6e20 6e61 6d65 3d22 7369 7a65 5f75 6e69  n name="size_uni
-000034e0: 7422 2076 616c 7565 3d22 5265 6e64 6572  t" value="Render
-000034f0: 4d65 7465 7273 496e 4d61 7055 6e69 7473  MetersInMapUnits
-00003500: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00003510: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-00003520: 4f70 7469 6f6e 206e 616d 653d 2276 6572  Option name="ver
-00003530: 7469 6361 6c5f 616e 6368 6f72 5f70 6f69  tical_anchor_poi
-00003540: 6e74 2220 7661 6c75 653d 2231 2220 7479  nt" value="1" ty
-00003550: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
-00003560: 2020 2020 2020 2020 203c 2f4f 7074 696f           </Optio
-00003570: 6e3e 0a20 2020 2020 2020 2020 203c 6461  n>.          <da
-00003580: 7461 5f64 6566 696e 6564 5f70 726f 7065  ta_defined_prope
-00003590: 7274 6965 733e 0a20 2020 2020 2020 2020  rties>.         
-000035a0: 2020 203c 4f70 7469 6f6e 2074 7970 653d     <Option type=
-000035b0: 224d 6170 223e 0a20 2020 2020 2020 2020  "Map">.         
-000035c0: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
-000035d0: 653d 226e 616d 6522 2076 616c 7565 3d22  e="name" value="
-000035e0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-000035f0: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
-00003600: 203c 4f70 7469 6f6e 206e 616d 653d 2270   <Option name="p
-00003610: 726f 7065 7274 6965 7322 2074 7970 653d  roperties" type=
-00003620: 224d 6170 223e 0a20 2020 2020 2020 2020  "Map">.         
-00003630: 2020 2020 2020 203c 4f70 7469 6f6e 206e         <Option n
-00003640: 616d 653d 2261 6e67 6c65 2220 7479 7065  ame="angle" type
-00003650: 3d22 4d61 7022 3e0a 2020 2020 2020 2020  ="Map">.        
-00003660: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00003670: 6e20 6e61 6d65 3d22 6163 7469 7665 2220  n name="active" 
-00003680: 7661 6c75 653d 2274 7275 6522 2074 7970  value="true" typ
-00003690: 653d 2262 6f6f 6c22 2f3e 0a20 2020 2020  e="bool"/>.     
-000036a0: 2020 2020 2020 2020 2020 2020 203c 4f70               <Op
-000036b0: 7469 6f6e 206e 616d 653d 2265 7870 7265  tion name="expre
-000036c0: 7373 696f 6e22 2076 616c 7565 3d22 3138  ssion" value="18
-000036d0: 3020 2b20 282d 2671 756f 743b 6f72 6965  0 + (-&quot;orie
-000036e0: 6e74 6174 696f 6e26 7175 6f74 3b20 2f20  ntation&quot; / 
-000036f0: 7069 2829 2920 2a20 3138 3022 2074 7970  pi()) * 180" typ
-00003700: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00003710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003720: 3c4f 7074 696f 6e20 6e61 6d65 3d22 7479  <Option name="ty
-00003730: 7065 2220 7661 6c75 653d 2233 2220 7479  pe" value="3" ty
-00003740: 7065 3d22 696e 7422 2f3e 0a20 2020 2020  pe="int"/>.     
-00003750: 2020 2020 2020 2020 2020 203c 2f4f 7074             </Opt
-00003760: 696f 6e3e 0a20 2020 2020 2020 2020 2020  ion>.           
-00003770: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
-00003780: 653d 226f 7574 6c69 6e65 5769 6474 6822  e="outlineWidth"
-00003790: 2074 7970 653d 224d 6170 223e 0a20 2020   type="Map">.   
-000037a0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000037b0: 4f70 7469 6f6e 206e 616d 653d 2261 6374  Option name="act
-000037c0: 6976 6522 2076 616c 7565 3d22 7472 7565  ive" value="true
-000037d0: 2220 7479 7065 3d22 626f 6f6c 222f 3e0a  " type="bool"/>.
+00002bb0: 3c4f 7074 696f 6e20 6e61 6d65 3d22 7479  <Option name="ty
+00002bc0: 7065 2220 7661 6c75 653d 2233 2220 7479  pe" value="3" ty
+00002bd0: 7065 3d22 696e 7422 2f3e 0a20 2020 2020  pe="int"/>.     
+00002be0: 2020 2020 2020 2020 2020 203c 2f4f 7074             </Opt
+00002bf0: 696f 6e3e 0a20 2020 2020 2020 2020 2020  ion>.           
+00002c00: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
+00002c10: 653d 226f 7574 6c69 6e65 5769 6474 6822  e="outlineWidth"
+00002c20: 2074 7970 653d 224d 6170 223e 0a20 2020   type="Map">.   
+00002c30: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00002c40: 4f70 7469 6f6e 206e 616d 653d 2261 6374  Option name="act
+00002c50: 6976 6522 2076 616c 7565 3d22 7472 7565  ive" value="true
+00002c60: 2220 7479 7065 3d22 626f 6f6c 222f 3e0a  " type="bool"/>.
+00002c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c80: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
+00002c90: 6578 7072 6573 7369 6f6e 2220 7661 6c75  expression" valu
+00002ca0: 653d 2226 7175 6f74 3b6c 616e 655f 7769  e="&quot;lane_wi
+00002cb0: 6474 6826 7175 6f74 3b20 2a20 302e 3722  dth&quot; * 0.7"
+00002cc0: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+00002cd0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00002ce0: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
+00002cf0: 3d22 7479 7065 2220 7661 6c75 653d 2233  ="type" value="3
+00002d00: 2220 7479 7065 3d22 696e 7422 2f3e 0a20  " type="int"/>. 
+00002d10: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00002d20: 2f4f 7074 696f 6e3e 0a20 2020 2020 2020  /Option>.       
+00002d30: 2020 2020 2020 203c 2f4f 7074 696f 6e3e         </Option>
+00002d40: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+00002d50: 4f70 7469 6f6e 206e 616d 653d 2274 7970  Option name="typ
+00002d60: 6522 2076 616c 7565 3d22 636f 6c6c 6563  e" value="collec
+00002d70: 7469 6f6e 2220 7479 7065 3d22 5153 7472  tion" type="QStr
+00002d80: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+00002d90: 2020 203c 2f4f 7074 696f 6e3e 0a20 2020     </Option>.   
+00002da0: 2020 2020 2020 203c 2f64 6174 615f 6465         </data_de
+00002db0: 6669 6e65 645f 7072 6f70 6572 7469 6573  fined_properties
+00002dc0: 3e0a 2020 2020 2020 2020 3c2f 6c61 7965  >.        </laye
+00002dd0: 723e 0a20 2020 2020 203c 2f73 796d 626f  r>.      </symbo
+00002de0: 6c3e 0a20 2020 2020 203c 7379 6d62 6f6c  l>.      <symbol
+00002df0: 206e 616d 653d 2231 2220 666f 7263 655f   name="1" force_
+00002e00: 7268 723d 2230 2220 6672 616d 655f 7261  rhr="0" frame_ra
+00002e10: 7465 3d22 3130 2220 616c 7068 613d 2231  te="10" alpha="1
+00002e20: 2220 636c 6970 5f74 6f5f 6578 7465 6e74  " clip_to_extent
+00002e30: 3d22 3122 2069 735f 616e 696d 6174 6564  ="1" is_animated
+00002e40: 3d22 3022 2074 7970 653d 226d 6172 6b65  ="0" type="marke
+00002e50: 7222 3e0a 2020 2020 2020 2020 3c64 6174  r">.        <dat
+00002e60: 615f 6465 6669 6e65 645f 7072 6f70 6572  a_defined_proper
+00002e70: 7469 6573 3e0a 2020 2020 2020 2020 2020  ties>.          
+00002e80: 3c4f 7074 696f 6e20 7479 7065 3d22 4d61  <Option type="Ma
+00002e90: 7022 3e0a 2020 2020 2020 2020 2020 2020  p">.            
+00002ea0: 3c4f 7074 696f 6e20 6e61 6d65 3d22 6e61  <Option name="na
+00002eb0: 6d65 2220 7661 6c75 653d 2222 2074 7970  me" value="" typ
+00002ec0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00002ed0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00002ee0: 6e20 6e61 6d65 3d22 7072 6f70 6572 7469  n name="properti
+00002ef0: 6573 222f 3e0a 2020 2020 2020 2020 2020  es"/>.          
+00002f00: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
+00002f10: 7479 7065 2220 7661 6c75 653d 2263 6f6c  type" value="col
+00002f20: 6c65 6374 696f 6e22 2074 7970 653d 2251  lection" type="Q
+00002f30: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+00002f40: 2020 2020 3c2f 4f70 7469 6f6e 3e0a 2020      </Option>.  
+00002f50: 2020 2020 2020 3c2f 6461 7461 5f64 6566        </data_def
+00002f60: 696e 6564 5f70 726f 7065 7274 6965 733e  ined_properties>
+00002f70: 0a20 2020 2020 2020 203c 6c61 7965 7220  .        <layer 
+00002f80: 7061 7373 3d22 3022 206c 6f63 6b65 643d  pass="0" locked=
+00002f90: 2230 2220 656e 6162 6c65 643d 2231 2220  "0" enabled="1" 
+00002fa0: 636c 6173 733d 2253 696d 706c 654d 6172  class="SimpleMar
+00002fb0: 6b65 7222 3e0a 2020 2020 2020 2020 2020  ker">.          
+00002fc0: 3c4f 7074 696f 6e20 7479 7065 3d22 4d61  <Option type="Ma
+00002fd0: 7022 3e0a 2020 2020 2020 2020 2020 2020  p">.            
+00002fe0: 3c4f 7074 696f 6e20 6e61 6d65 3d22 616e  <Option name="an
+00002ff0: 676c 6522 2076 616c 7565 3d22 3022 2074  gle" value="0" t
+00003000: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
+00003010: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00003020: 696f 6e20 6e61 6d65 3d22 6361 705f 7374  ion name="cap_st
+00003030: 796c 6522 2076 616c 7565 3d22 666c 6174  yle" value="flat
+00003040: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00003050: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
+00003060: 4f70 7469 6f6e 206e 616d 653d 2263 6f6c  Option name="col
+00003070: 6f72 2220 7661 6c75 653d 2232 3332 2c38  or" value="232,8
+00003080: 352c 302c 3235 3522 2074 7970 653d 2251  5,0,255" type="Q
+00003090: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+000030a0: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
+000030b0: 6d65 3d22 686f 7269 7a6f 6e74 616c 5f61  me="horizontal_a
+000030c0: 6e63 686f 725f 706f 696e 7422 2076 616c  nchor_point" val
+000030d0: 7565 3d22 3122 2074 7970 653d 2251 5374  ue="1" type="QSt
+000030e0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+000030f0: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
+00003100: 3d22 6a6f 696e 7374 796c 6522 2076 616c  ="joinstyle" val
+00003110: 7565 3d22 6265 7665 6c22 2074 7970 653d  ue="bevel" type=
+00003120: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00003130: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00003140: 6e61 6d65 3d22 6e61 6d65 2220 7661 6c75  name="name" valu
+00003150: 653d 226c 696e 6522 2074 7970 653d 2251  e="line" type="Q
+00003160: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+00003170: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
+00003180: 6d65 3d22 6f66 6673 6574 2220 7661 6c75  me="offset" valu
+00003190: 653d 2230 2c30 2220 7479 7065 3d22 5153  e="0,0" type="QS
+000031a0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+000031b0: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
+000031c0: 653d 226f 6666 7365 745f 6d61 705f 756e  e="offset_map_un
+000031d0: 6974 5f73 6361 6c65 2220 7661 6c75 653d  it_scale" value=
+000031e0: 2233 783a 302c 302c 302c 302c 302c 3022  "3x:0,0,0,0,0,0"
+000031f0: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+00003200: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
+00003210: 7074 696f 6e20 6e61 6d65 3d22 6f66 6673  ption name="offs
+00003220: 6574 5f75 6e69 7422 2076 616c 7565 3d22  et_unit" value="
+00003230: 4d4d 2220 7479 7065 3d22 5153 7472 696e  MM" type="QStrin
+00003240: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00003250: 203c 4f70 7469 6f6e 206e 616d 653d 226f   <Option name="o
+00003260: 7574 6c69 6e65 5f63 6f6c 6f72 2220 7661  utline_color" va
+00003270: 6c75 653d 2232 3535 2c32 3535 2c32 3535  lue="255,255,255
+00003280: 2c32 3535 2220 7479 7065 3d22 5153 7472  ,255" type="QStr
+00003290: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+000032a0: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
+000032b0: 226f 7574 6c69 6e65 5f73 7479 6c65 2220  "outline_style" 
+000032c0: 7661 6c75 653d 2273 6f6c 6964 2220 7479  value="solid" ty
+000032d0: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+000032e0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+000032f0: 6f6e 206e 616d 653d 226f 7574 6c69 6e65  on name="outline
+00003300: 5f77 6964 7468 2220 7661 6c75 653d 2232  _width" value="2
+00003310: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00003320: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
+00003330: 4f70 7469 6f6e 206e 616d 653d 226f 7574  Option name="out
+00003340: 6c69 6e65 5f77 6964 7468 5f6d 6170 5f75  line_width_map_u
+00003350: 6e69 745f 7363 616c 6522 2076 616c 7565  nit_scale" value
+00003360: 3d22 3378 3a30 2c30 2c30 2c30 2c30 2c30  ="3x:0,0,0,0,0,0
+00003370: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00003380: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
+00003390: 4f70 7469 6f6e 206e 616d 653d 226f 7574  Option name="out
+000033a0: 6c69 6e65 5f77 6964 7468 5f75 6e69 7422  line_width_unit"
+000033b0: 2076 616c 7565 3d22 5265 6e64 6572 4d65   value="RenderMe
+000033c0: 7465 7273 496e 4d61 7055 6e69 7473 2220  tersInMapUnits" 
+000033d0: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+000033e0: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
+000033f0: 7469 6f6e 206e 616d 653d 2273 6361 6c65  tion name="scale
+00003400: 5f6d 6574 686f 6422 2076 616c 7565 3d22  _method" value="
+00003410: 6469 616d 6574 6572 2220 7479 7065 3d22  diameter" type="
+00003420: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+00003430: 2020 2020 2020 203c 4f70 7469 6f6e 206e         <Option n
+00003440: 616d 653d 2273 697a 6522 2076 616c 7565  ame="size" value
+00003450: 3d22 3322 2074 7970 653d 2251 5374 7269  ="3" type="QStri
+00003460: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+00003470: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
+00003480: 7369 7a65 5f6d 6170 5f75 6e69 745f 7363  size_map_unit_sc
+00003490: 616c 6522 2076 616c 7565 3d22 3378 3a30  ale" value="3x:0
+000034a0: 2c30 2c30 2c30 2c30 2c30 2220 7479 7065  ,0,0,0,0,0" type
+000034b0: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+000034c0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+000034d0: 206e 616d 653d 2273 697a 655f 756e 6974   name="size_unit
+000034e0: 2220 7661 6c75 653d 2252 656e 6465 724d  " value="RenderM
+000034f0: 6574 6572 7349 6e4d 6170 556e 6974 7322  etersInMapUnits"
+00003500: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+00003510: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
+00003520: 7074 696f 6e20 6e61 6d65 3d22 7665 7274  ption name="vert
+00003530: 6963 616c 5f61 6e63 686f 725f 706f 696e  ical_anchor_poin
+00003540: 7422 2076 616c 7565 3d22 3122 2074 7970  t" value="1" typ
+00003550: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00003560: 2020 2020 2020 2020 3c2f 4f70 7469 6f6e          </Option
+00003570: 3e0a 2020 2020 2020 2020 2020 3c64 6174  >.          <dat
+00003580: 615f 6465 6669 6e65 645f 7072 6f70 6572  a_defined_proper
+00003590: 7469 6573 3e0a 2020 2020 2020 2020 2020  ties>.          
+000035a0: 2020 3c4f 7074 696f 6e20 7479 7065 3d22    <Option type="
+000035b0: 4d61 7022 3e0a 2020 2020 2020 2020 2020  Map">.          
+000035c0: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
+000035d0: 3d22 6e61 6d65 2220 7661 6c75 653d 2222  ="name" value=""
+000035e0: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+000035f0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00003600: 3c4f 7074 696f 6e20 6e61 6d65 3d22 7072  <Option name="pr
+00003610: 6f70 6572 7469 6573 2220 7479 7065 3d22  operties" type="
+00003620: 4d61 7022 3e0a 2020 2020 2020 2020 2020  Map">.          
+00003630: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
+00003640: 6d65 3d22 616e 676c 6522 2074 7970 653d  me="angle" type=
+00003650: 224d 6170 223e 0a20 2020 2020 2020 2020  "Map">.         
+00003660: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00003670: 206e 616d 653d 2261 6374 6976 6522 2076   name="active" v
+00003680: 616c 7565 3d22 7472 7565 2220 7479 7065  alue="true" type
+00003690: 3d22 626f 6f6c 222f 3e0a 2020 2020 2020  ="bool"/>.      
+000036a0: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+000036b0: 696f 6e20 6e61 6d65 3d22 6578 7072 6573  ion name="expres
+000036c0: 7369 6f6e 2220 7661 6c75 653d 2239 3020  sion" value="90 
+000036d0: 2b20 282d 2671 756f 743b 6f72 6965 6e74  + (-&quot;orient
+000036e0: 6174 696f 6e26 7175 6f74 3b20 2f20 7069  ation&quot; / pi
+000036f0: 2829 2920 2a20 3138 3022 2074 7970 653d  ()) * 180" type=
+00003700: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00003710: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
+00003720: 7074 696f 6e20 6e61 6d65 3d22 7479 7065  ption name="type
+00003730: 2220 7661 6c75 653d 2233 2220 7479 7065  " value="3" type
+00003740: 3d22 696e 7422 2f3e 0a20 2020 2020 2020  ="int"/>.       
+00003750: 2020 2020 2020 2020 203c 2f4f 7074 696f           </Optio
+00003760: 6e3e 0a20 2020 2020 2020 2020 2020 2020  n>.             
+00003770: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
+00003780: 226f 7574 6c69 6e65 5769 6474 6822 2074  "outlineWidth" t
+00003790: 7970 653d 224d 6170 223e 0a20 2020 2020  ype="Map">.     
+000037a0: 2020 2020 2020 2020 2020 2020 203c 4f70               <Op
+000037b0: 7469 6f6e 206e 616d 653d 2261 6374 6976  tion name="activ
+000037c0: 6522 2076 616c 7565 3d22 7472 7565 2220  e" value="true" 
+000037d0: 7479 7065 3d22 626f 6f6c 222f 3e0a 2020  type="bool"/>.  
 000037e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037f0: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
-00003800: 6578 7072 6573 7369 6f6e 2220 7661 6c75  expression" valu
-00003810: 653d 2226 7175 6f74 3b6c 616e 655f 7769  e="&quot;lane_wi
-00003820: 6474 6826 7175 6f74 3b22 2074 7970 653d  dth&quot;" type=
-00003830: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-00003840: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
-00003850: 7074 696f 6e20 6e61 6d65 3d22 7479 7065  ption name="type
-00003860: 2220 7661 6c75 653d 2233 2220 7479 7065  " value="3" type
-00003870: 3d22 696e 7422 2f3e 0a20 2020 2020 2020  ="int"/>.       
-00003880: 2020 2020 2020 2020 203c 2f4f 7074 696f           </Optio
-00003890: 6e3e 0a20 2020 2020 2020 2020 2020 2020  n>.             
-000038a0: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
-000038b0: 2273 697a 6522 2074 7970 653d 224d 6170  "size" type="Map
-000038c0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-000038d0: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
-000038e0: 653d 2261 6374 6976 6522 2076 616c 7565  e="active" value
-000038f0: 3d22 7472 7565 2220 7479 7065 3d22 626f  ="true" type="bo
-00003900: 6f6c 222f 3e0a 2020 2020 2020 2020 2020  ol"/>.          
-00003910: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00003920: 6e61 6d65 3d22 6578 7072 6573 7369 6f6e  name="expression
-00003930: 2220 7661 6c75 653d 2233 202d 2032 202a  " value="3 - 2 *
-00003940: 2030 2e30 3031 202a 2040 6d61 705f 7363   0.001 * @map_sc
-00003950: 616c 6522 2074 7970 653d 2251 5374 7269  ale" type="QStri
-00003960: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
-00003970: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00003980: 6e61 6d65 3d22 7479 7065 2220 7661 6c75  name="type" valu
-00003990: 653d 2233 2220 7479 7065 3d22 696e 7422  e="3" type="int"
-000039a0: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
-000039b0: 2020 203c 2f4f 7074 696f 6e3e 0a20 2020     </Option>.   
-000039c0: 2020 2020 2020 2020 2020 203c 2f4f 7074             </Opt
-000039d0: 696f 6e3e 0a20 2020 2020 2020 2020 2020  ion>.           
-000039e0: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
-000039f0: 2274 7970 6522 2076 616c 7565 3d22 636f  "type" value="co
-00003a00: 6c6c 6563 7469 6f6e 2220 7479 7065 3d22  llection" type="
-00003a10: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-00003a20: 2020 2020 2020 203c 2f4f 7074 696f 6e3e         </Option>
-00003a30: 0a20 2020 2020 2020 2020 203c 2f64 6174  .          </dat
-00003a40: 615f 6465 6669 6e65 645f 7072 6f70 6572  a_defined_proper
-00003a50: 7469 6573 3e0a 2020 2020 2020 2020 3c2f  ties>.        </
-00003a60: 6c61 7965 723e 0a20 2020 2020 203c 2f73  layer>.      </s
-00003a70: 796d 626f 6c3e 0a20 2020 2020 203c 7379  ymbol>.      <sy
-00003a80: 6d62 6f6c 206e 616d 653d 2232 2220 666f  mbol name="2" fo
-00003a90: 7263 655f 7268 723d 2230 2220 6672 616d  rce_rhr="0" fram
-00003aa0: 655f 7261 7465 3d22 3130 2220 616c 7068  e_rate="10" alph
-00003ab0: 613d 2231 2220 636c 6970 5f74 6f5f 6578  a="1" clip_to_ex
-00003ac0: 7465 6e74 3d22 3122 2069 735f 616e 696d  tent="1" is_anim
-00003ad0: 6174 6564 3d22 3022 2074 7970 653d 226d  ated="0" type="m
-00003ae0: 6172 6b65 7222 3e0a 2020 2020 2020 2020  arker">.        
-00003af0: 3c64 6174 615f 6465 6669 6e65 645f 7072  <data_defined_pr
-00003b00: 6f70 6572 7469 6573 3e0a 2020 2020 2020  operties>.      
-00003b10: 2020 2020 3c4f 7074 696f 6e20 7479 7065      <Option type
-00003b20: 3d22 4d61 7022 3e0a 2020 2020 2020 2020  ="Map">.        
-00003b30: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
-00003b40: 3d22 6e61 6d65 2220 7661 6c75 653d 2222  ="name" value=""
-00003b50: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-00003b60: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
-00003b70: 7074 696f 6e20 6e61 6d65 3d22 7072 6f70  ption name="prop
-00003b80: 6572 7469 6573 222f 3e0a 2020 2020 2020  erties"/>.      
-00003b90: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
-00003ba0: 6d65 3d22 7479 7065 2220 7661 6c75 653d  me="type" value=
-00003bb0: 2263 6f6c 6c65 6374 696f 6e22 2074 7970  "collection" typ
-00003bc0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00003bd0: 2020 2020 2020 2020 3c2f 4f70 7469 6f6e          </Option
-00003be0: 3e0a 2020 2020 2020 2020 3c2f 6461 7461  >.        </data
-00003bf0: 5f64 6566 696e 6564 5f70 726f 7065 7274  _defined_propert
-00003c00: 6965 733e 0a20 2020 2020 2020 203c 6c61  ies>.        <la
-00003c10: 7965 7220 7061 7373 3d22 3022 206c 6f63  yer pass="0" loc
-00003c20: 6b65 643d 2230 2220 656e 6162 6c65 643d  ked="0" enabled=
-00003c30: 2231 2220 636c 6173 733d 2253 696d 706c  "1" class="Simpl
-00003c40: 654d 6172 6b65 7222 3e0a 2020 2020 2020  eMarker">.      
-00003c50: 2020 2020 3c4f 7074 696f 6e20 7479 7065      <Option type
-00003c60: 3d22 4d61 7022 3e0a 2020 2020 2020 2020  ="Map">.        
-00003c70: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
-00003c80: 3d22 616e 676c 6522 2076 616c 7565 3d22  ="angle" value="
-00003c90: 3022 2074 7970 653d 2251 5374 7269 6e67  0" type="QString
-00003ca0: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00003cb0: 3c4f 7074 696f 6e20 6e61 6d65 3d22 6361  <Option name="ca
-00003cc0: 705f 7374 796c 6522 2076 616c 7565 3d22  p_style" value="
-00003cd0: 666c 6174 2220 7479 7065 3d22 5153 7472  flat" type="QStr
-00003ce0: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-00003cf0: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
-00003d00: 2263 6f6c 6f72 2220 7661 6c75 653d 2232  "color" value="2
-00003d10: 3332 2c38 352c 302c 3235 3522 2074 7970  32,85,0,255" typ
-00003d20: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00003d30: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00003d40: 6e20 6e61 6d65 3d22 686f 7269 7a6f 6e74  n name="horizont
-00003d50: 616c 5f61 6e63 686f 725f 706f 696e 7422  al_anchor_point"
-00003d60: 2076 616c 7565 3d22 3122 2074 7970 653d   value="1" type=
-00003d70: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-00003d80: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00003d90: 6e61 6d65 3d22 6a6f 696e 7374 796c 6522  name="joinstyle"
-00003da0: 2076 616c 7565 3d22 6265 7665 6c22 2074   value="bevel" t
-00003db0: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
-00003dc0: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00003dd0: 696f 6e20 6e61 6d65 3d22 6e61 6d65 2220  ion name="name" 
-00003de0: 7661 6c75 653d 226c 696e 6522 2074 7970  value="line" typ
-00003df0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00003e00: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00003e10: 6e20 6e61 6d65 3d22 6f66 6673 6574 2220  n name="offset" 
-00003e20: 7661 6c75 653d 2230 2c30 2220 7479 7065  value="0,0" type
-00003e30: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-00003e40: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-00003e50: 206e 616d 653d 226f 6666 7365 745f 6d61   name="offset_ma
-00003e60: 705f 756e 6974 5f73 6361 6c65 2220 7661  p_unit_scale" va
-00003e70: 6c75 653d 2233 783a 302c 302c 302c 302c  lue="3x:0,0,0,0,
-00003e80: 302c 3022 2074 7970 653d 2251 5374 7269  0,0" type="QStri
-00003e90: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
-00003ea0: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
-00003eb0: 6f66 6673 6574 5f75 6e69 7422 2076 616c  offset_unit" val
-00003ec0: 7565 3d22 4d4d 2220 7479 7065 3d22 5153  ue="MM" type="QS
-00003ed0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00003ee0: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
-00003ef0: 653d 226f 7574 6c69 6e65 5f63 6f6c 6f72  e="outline_color
-00003f00: 2220 7661 6c75 653d 2232 3535 2c32 3535  " value="255,255
-00003f10: 2c32 3535 2c32 3535 2220 7479 7065 3d22  ,255,255" type="
-00003f20: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-00003f30: 2020 2020 2020 203c 4f70 7469 6f6e 206e         <Option n
-00003f40: 616d 653d 226f 7574 6c69 6e65 5f73 7479  ame="outline_sty
-00003f50: 6c65 2220 7661 6c75 653d 2273 6f6c 6964  le" value="solid
-00003f60: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00003f70: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-00003f80: 4f70 7469 6f6e 206e 616d 653d 226f 7574  Option name="out
-00003f90: 6c69 6e65 5f77 6964 7468 2220 7661 6c75  line_width" valu
-00003fa0: 653d 2232 2220 7479 7065 3d22 5153 7472  e="2" type="QStr
-00003fb0: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-00003fc0: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
-00003fd0: 226f 7574 6c69 6e65 5f77 6964 7468 5f6d  "outline_width_m
-00003fe0: 6170 5f75 6e69 745f 7363 616c 6522 2076  ap_unit_scale" v
-00003ff0: 616c 7565 3d22 3378 3a30 2c30 2c30 2c30  alue="3x:0,0,0,0
-00004000: 2c30 2c30 2220 7479 7065 3d22 5153 7472  ,0,0" type="QStr
-00004010: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-00004020: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
-00004030: 226f 7574 6c69 6e65 5f77 6964 7468 5f75  "outline_width_u
-00004040: 6e69 7422 2076 616c 7565 3d22 5265 6e64  nit" value="Rend
-00004050: 6572 4d65 7465 7273 496e 4d61 7055 6e69  erMetersInMapUni
-00004060: 7473 2220 7479 7065 3d22 5153 7472 696e  ts" type="QStrin
-00004070: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
-00004080: 203c 4f70 7469 6f6e 206e 616d 653d 2273   <Option name="s
-00004090: 6361 6c65 5f6d 6574 686f 6422 2076 616c  cale_method" val
-000040a0: 7565 3d22 6469 616d 6574 6572 2220 7479  ue="diameter" ty
-000040b0: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
-000040c0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-000040d0: 6f6e 206e 616d 653d 2273 697a 6522 2076  on name="size" v
-000040e0: 616c 7565 3d22 3322 2074 7970 653d 2251  alue="3" type="Q
-000040f0: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
-00004100: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
-00004110: 6d65 3d22 7369 7a65 5f6d 6170 5f75 6e69  me="size_map_uni
-00004120: 745f 7363 616c 6522 2076 616c 7565 3d22  t_scale" value="
-00004130: 3378 3a30 2c30 2c30 2c30 2c30 2c30 2220  3x:0,0,0,0,0,0" 
-00004140: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
-00004150: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
-00004160: 7469 6f6e 206e 616d 653d 2273 697a 655f  tion name="size_
-00004170: 756e 6974 2220 7661 6c75 653d 2252 656e  unit" value="Ren
-00004180: 6465 724d 6574 6572 7349 6e4d 6170 556e  derMetersInMapUn
-00004190: 6974 7322 2074 7970 653d 2251 5374 7269  its" type="QStri
-000041a0: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
-000041b0: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
-000041c0: 7665 7274 6963 616c 5f61 6e63 686f 725f  vertical_anchor_
-000041d0: 706f 696e 7422 2076 616c 7565 3d22 3122  point" value="1"
-000041e0: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-000041f0: 3e0a 2020 2020 2020 2020 2020 3c2f 4f70  >.          </Op
-00004200: 7469 6f6e 3e0a 2020 2020 2020 2020 2020  tion>.          
-00004210: 3c64 6174 615f 6465 6669 6e65 645f 7072  <data_defined_pr
-00004220: 6f70 6572 7469 6573 3e0a 2020 2020 2020  operties>.      
-00004230: 2020 2020 2020 3c4f 7074 696f 6e20 7479        <Option ty
-00004240: 7065 3d22 4d61 7022 3e0a 2020 2020 2020  pe="Map">.      
-00004250: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00004260: 6e61 6d65 3d22 6e61 6d65 2220 7661 6c75  name="name" valu
-00004270: 653d 2222 2074 7970 653d 2251 5374 7269  e="" type="QStri
-00004280: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
-00004290: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
-000042a0: 3d22 7072 6f70 6572 7469 6573 2220 7479  ="properties" ty
-000042b0: 7065 3d22 4d61 7022 3e0a 2020 2020 2020  pe="Map">.      
-000042c0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-000042d0: 6e20 6e61 6d65 3d22 616e 676c 6522 2074  n name="angle" t
-000042e0: 7970 653d 224d 6170 223e 0a20 2020 2020  ype="Map">.     
-000042f0: 2020 2020 2020 2020 2020 2020 203c 4f70               <Op
-00004300: 7469 6f6e 206e 616d 653d 2261 6374 6976  tion name="activ
-00004310: 6522 2076 616c 7565 3d22 7472 7565 2220  e" value="true" 
-00004320: 7479 7065 3d22 626f 6f6c 222f 3e0a 2020  type="bool"/>.  
-00004330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004340: 3c4f 7074 696f 6e20 6e61 6d65 3d22 6578  <Option name="ex
-00004350: 7072 6573 7369 6f6e 2220 7661 6c75 653d  pression" value=
-00004360: 2231 3830 202b 2028 2d26 7175 6f74 3b6f  "180 + (-&quot;o
-00004370: 7269 656e 7461 7469 6f6e 2671 756f 743b  rientation&quot;
-00004380: 202f 2070 6928 2929 202a 2031 3830 2220   / pi()) * 180" 
-00004390: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
-000043a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000043b0: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
-000043c0: 2274 7970 6522 2076 616c 7565 3d22 3322  "type" value="3"
-000043d0: 2074 7970 653d 2269 6e74 222f 3e0a 2020   type="int"/>.  
-000043e0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-000043f0: 4f70 7469 6f6e 3e0a 2020 2020 2020 2020  Option>.        
-00004400: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00004410: 6e61 6d65 3d22 6f75 746c 696e 6557 6964  name="outlineWid
-00004420: 7468 2220 7479 7065 3d22 4d61 7022 3e0a  th" type="Map">.
-00004430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004440: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
-00004450: 6163 7469 7665 2220 7661 6c75 653d 2274  active" value="t
-00004460: 7275 6522 2074 7970 653d 2262 6f6f 6c22  rue" type="bool"
-00004470: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
-00004480: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
-00004490: 653d 2265 7870 7265 7373 696f 6e22 2076  e="expression" v
-000044a0: 616c 7565 3d22 2671 756f 743b 6c61 6e65  alue="&quot;lane
-000044b0: 5f77 6964 7468 2671 756f 743b 2220 7479  _width&quot;" ty
-000044c0: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
-000044d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044e0: 203c 4f70 7469 6f6e 206e 616d 653d 2274   <Option name="t
-000044f0: 7970 6522 2076 616c 7565 3d22 3322 2074  ype" value="3" t
-00004500: 7970 653d 2269 6e74 222f 3e0a 2020 2020  ype="int"/>.    
-00004510: 2020 2020 2020 2020 2020 2020 3c2f 4f70              </Op
-00004520: 7469 6f6e 3e0a 2020 2020 2020 2020 2020  tion>.          
-00004530: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
-00004540: 6d65 3d22 7369 7a65 2220 7479 7065 3d22  me="size" type="
-00004550: 4d61 7022 3e0a 2020 2020 2020 2020 2020  Map">.          
-00004560: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00004570: 6e61 6d65 3d22 6163 7469 7665 2220 7661  name="active" va
-00004580: 6c75 653d 2274 7275 6522 2074 7970 653d  lue="true" type=
-00004590: 2262 6f6f 6c22 2f3e 0a20 2020 2020 2020  "bool"/>.       
-000045a0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-000045b0: 6f6e 206e 616d 653d 2265 7870 7265 7373  on name="express
-000045c0: 696f 6e22 2076 616c 7565 3d22 3320 2d20  ion" value="3 - 
-000045d0: 3220 2a20 302e 3030 3220 2a20 406d 6170  2 * 0.002 * @map
-000045e0: 5f73 6361 6c65 2220 7479 7065 3d22 5153  _scale" type="QS
-000045f0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00004600: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00004610: 6f6e 206e 616d 653d 2274 7970 6522 2076  on name="type" v
-00004620: 616c 7565 3d22 3322 2074 7970 653d 2269  alue="3" type="i
-00004630: 6e74 222f 3e0a 2020 2020 2020 2020 2020  nt"/>.          
-00004640: 2020 2020 2020 3c2f 4f70 7469 6f6e 3e0a        </Option>.
-00004650: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00004660: 4f70 7469 6f6e 3e0a 2020 2020 2020 2020  Option>.        
-00004670: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
-00004680: 6d65 3d22 7479 7065 2220 7661 6c75 653d  me="type" value=
-00004690: 2263 6f6c 6c65 6374 696f 6e22 2074 7970  "collection" typ
-000046a0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-000046b0: 2020 2020 2020 2020 2020 3c2f 4f70 7469            </Opti
-000046c0: 6f6e 3e0a 2020 2020 2020 2020 2020 3c2f  on>.          </
-000046d0: 6461 7461 5f64 6566 696e 6564 5f70 726f  data_defined_pro
-000046e0: 7065 7274 6965 733e 0a20 2020 2020 2020  perties>.       
-000046f0: 203c 2f6c 6179 6572 3e0a 2020 2020 2020   </layer>.      
-00004700: 3c2f 7379 6d62 6f6c 3e0a 2020 2020 3c2f  </symbol>.    </
-00004710: 7379 6d62 6f6c 733e 0a20 203c 2f72 656e  symbols>.  </ren
-00004720: 6465 7265 722d 7632 3e0a 2020 3c63 7573  derer-v2>.  <cus
-00004730: 746f 6d70 726f 7065 7274 6965 733e 0a20  tomproperties>. 
-00004740: 2020 203c 4f70 7469 6f6e 2074 7970 653d     <Option type=
-00004750: 224d 6170 223e 0a20 2020 2020 203c 4f70  "Map">.      <Op
-00004760: 7469 6f6e 206e 616d 653d 2264 7561 6c76  tion name="dualv
-00004770: 6965 772f 7072 6576 6965 7745 7870 7265  iew/previewExpre
-00004780: 7373 696f 6e73 2220 7479 7065 3d22 4c69  ssions" type="Li
-00004790: 7374 223e 0a20 2020 2020 2020 203c 4f70  st">.        <Op
-000047a0: 7469 6f6e 2076 616c 7565 3d22 2671 756f  tion value="&quo
-000047b0: 743b 7479 7065 2671 756f 743b 2220 7479  t;type&quot;" ty
-000047c0: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
-000047d0: 2020 2020 203c 2f4f 7074 696f 6e3e 0a20       </Option>. 
-000047e0: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
-000047f0: 653d 2265 6d62 6564 6465 6457 6964 6765  e="embeddedWidge
-00004800: 7473 2f63 6f75 6e74 2220 7661 6c75 653d  ts/count" value=
-00004810: 2230 2220 7479 7065 3d22 696e 7422 2f3e  "0" type="int"/>
-00004820: 0a20 2020 2020 203c 4f70 7469 6f6e 206e  .      <Option n
-00004830: 616d 653d 2276 6172 6961 626c 654e 616d  ame="variableNam
-00004840: 6573 222f 3e0a 2020 2020 2020 3c4f 7074  es"/>.      <Opt
-00004850: 696f 6e20 6e61 6d65 3d22 7661 7269 6162  ion name="variab
-00004860: 6c65 5661 6c75 6573 222f 3e0a 2020 2020  leValues"/>.    
-00004870: 3c2f 4f70 7469 6f6e 3e0a 2020 3c2f 6375  </Option>.  </cu
-00004880: 7374 6f6d 7072 6f70 6572 7469 6573 3e0a  stomproperties>.
-00004890: 2020 3c62 6c65 6e64 4d6f 6465 3e30 3c2f    <blendMode>0</
-000048a0: 626c 656e 644d 6f64 653e 0a20 203c 6665  blendMode>.  <fe
-000048b0: 6174 7572 6542 6c65 6e64 4d6f 6465 3e30  atureBlendMode>0
-000048c0: 3c2f 6665 6174 7572 6542 6c65 6e64 4d6f  </featureBlendMo
-000048d0: 6465 3e0a 2020 3c6c 6179 6572 4f70 6163  de>.  <layerOpac
-000048e0: 6974 793e 313c 2f6c 6179 6572 4f70 6163  ity>1</layerOpac
-000048f0: 6974 793e 0a20 203c 5369 6e67 6c65 4361  ity>.  <SingleCa
-00004900: 7465 676f 7279 4469 6167 7261 6d52 656e  tegoryDiagramRen
-00004910: 6465 7265 7220 6174 7472 6962 7574 654c  derer attributeL
-00004920: 6567 656e 643d 2231 2220 6469 6167 7261  egend="1" diagra
-00004930: 6d54 7970 653d 2248 6973 746f 6772 616d  mType="Histogram
-00004940: 223e 0a20 2020 203c 4469 6167 7261 6d43  ">.    <DiagramC
-00004950: 6174 6567 6f72 7920 7065 6e41 6c70 6861  ategory penAlpha
-00004960: 3d22 3235 3522 2068 6569 6768 743d 2231  ="255" height="1
-00004970: 3522 2073 7061 6369 6e67 556e 6974 5363  5" spacingUnitSc
-00004980: 616c 653d 2233 783a 302c 302c 302c 302c  ale="3x:0,0,0,0,
-00004990: 302c 3022 206f 7061 6369 7479 3d22 3122  0,0" opacity="1"
-000049a0: 206d 6178 5363 616c 6544 656e 6f6d 696e   maxScaleDenomin
-000049b0: 6174 6f72 3d22 3165 2b30 3822 206c 6162  ator="1e+08" lab
-000049c0: 656c 506c 6163 656d 656e 744d 6574 686f  elPlacementMetho
-000049d0: 643d 2258 4865 6967 6874 2220 6469 7265  d="XHeight" dire
-000049e0: 6374 696f 6e3d 2230 2220 6c69 6e65 5369  ction="0" lineSi
-000049f0: 7a65 5363 616c 653d 2233 783a 302c 302c  zeScale="3x:0,0,
-00004a00: 302c 302c 302c 3022 2064 6961 6772 616d  0,0,0,0" diagram
-00004a10: 4f72 6965 6e74 6174 696f 6e3d 2255 7022  Orientation="Up"
-00004a20: 2073 7061 6369 6e67 556e 6974 3d22 4d4d   spacingUnit="MM
-00004a30: 2220 7369 7a65 5363 616c 653d 2233 783a  " sizeScale="3x:
-00004a40: 302c 302c 302c 302c 302c 3022 2073 6361  0,0,0,0,0,0" sca
-00004a50: 6c65 4465 7065 6e64 656e 6379 3d22 4172  leDependency="Ar
-00004a60: 6561 2220 6d69 6e69 6d75 6d53 697a 653d  ea" minimumSize=
-00004a70: 2230 2220 656e 6162 6c65 643d 2230 2220  "0" enabled="0" 
-00004a80: 7369 7a65 5479 7065 3d22 4d4d 2220 6d69  sizeType="MM" mi
-00004a90: 6e53 6361 6c65 4465 6e6f 6d69 6e61 746f  nScaleDenominato
-00004aa0: 723d 2230 2220 726f 7461 7469 6f6e 4f66  r="0" rotationOf
-00004ab0: 6673 6574 3d22 3237 3022 2070 656e 436f  fset="270" penCo
-00004ac0: 6c6f 723d 2223 3030 3030 3030 2220 6261  lor="#000000" ba
-00004ad0: 636b 6772 6f75 6e64 416c 7068 613d 2232  ckgroundAlpha="2
-00004ae0: 3535 2220 6261 7257 6964 7468 3d22 3522  55" barWidth="5"
-00004af0: 2062 6163 6b67 726f 756e 6443 6f6c 6f72   backgroundColor
-00004b00: 3d22 2366 6666 6666 6622 206c 696e 6553  ="#ffffff" lineS
-00004b10: 697a 6554 7970 653d 224d 4d22 2073 6361  izeType="MM" sca
-00004b20: 6c65 4261 7365 6456 6973 6962 696c 6974  leBasedVisibilit
-00004b30: 793d 2230 2220 7368 6f77 4178 6973 3d22  y="0" showAxis="
-00004b40: 3122 2073 7061 6369 6e67 3d22 3522 2070  1" spacing="5" p
-00004b50: 656e 5769 6474 683d 2230 2220 7769 6474  enWidth="0" widt
-00004b60: 683d 2231 3522 3e0a 2020 2020 2020 3c66  h="15">.      <f
-00004b70: 6f6e 7450 726f 7065 7274 6965 7320 7374  ontProperties st
-00004b80: 7269 6b65 7468 726f 7567 683d 2230 2220  rikethrough="0" 
-00004b90: 6465 7363 7269 7074 696f 6e3d 224e 6f74  description="Not
-00004ba0: 6f20 5361 6e73 2c31 302c 2d31 2c30 2c35  o Sans,10,-1,0,5
-00004bb0: 302c 302c 302c 302c 302c 3022 2069 7461  0,0,0,0,0,0" ita
-00004bc0: 6c69 633d 2230 2220 756e 6465 726c 696e  lic="0" underlin
-00004bd0: 653d 2230 2220 7374 796c 653d 2222 2062  e="0" style="" b
-00004be0: 6f6c 643d 2230 222f 3e0a 2020 2020 2020  old="0"/>.      
-00004bf0: 3c61 7474 7269 6275 7465 2063 6f6c 6f72  <attribute color
-00004c00: 3d22 2330 3030 3030 3022 2066 6965 6c64  ="#000000" field
-00004c10: 3d22 2220 636f 6c6f 724f 7061 6369 7479  ="" colorOpacity
-00004c20: 3d22 3122 206c 6162 656c 3d22 222f 3e0a  ="1" label=""/>.
-00004c30: 2020 2020 2020 3c61 7869 7353 796d 626f        <axisSymbo
-00004c40: 6c3e 0a20 2020 2020 2020 203c 7379 6d62  l>.        <symb
-00004c50: 6f6c 206e 616d 653d 2222 2066 6f72 6365  ol name="" force
-00004c60: 5f72 6872 3d22 3022 2066 7261 6d65 5f72  _rhr="0" frame_r
-00004c70: 6174 653d 2231 3022 2061 6c70 6861 3d22  ate="10" alpha="
-00004c80: 3122 2063 6c69 705f 746f 5f65 7874 656e  1" clip_to_exten
-00004c90: 743d 2231 2220 6973 5f61 6e69 6d61 7465  t="1" is_animate
-00004ca0: 643d 2230 2220 7479 7065 3d22 6c69 6e65  d="0" type="line
-00004cb0: 223e 0a20 2020 2020 2020 2020 203c 6461  ">.          <da
-00004cc0: 7461 5f64 6566 696e 6564 5f70 726f 7065  ta_defined_prope
-00004cd0: 7274 6965 733e 0a20 2020 2020 2020 2020  rties>.         
-00004ce0: 2020 203c 4f70 7469 6f6e 2074 7970 653d     <Option type=
-00004cf0: 224d 6170 223e 0a20 2020 2020 2020 2020  "Map">.         
-00004d00: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
-00004d10: 653d 226e 616d 6522 2076 616c 7565 3d22  e="name" value="
-00004d20: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00004d30: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
-00004d40: 203c 4f70 7469 6f6e 206e 616d 653d 2270   <Option name="p
-00004d50: 726f 7065 7274 6965 7322 2f3e 0a20 2020  roperties"/>.   
-00004d60: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00004d70: 6f6e 206e 616d 653d 2274 7970 6522 2076  on name="type" v
-00004d80: 616c 7565 3d22 636f 6c6c 6563 7469 6f6e  alue="collection
-00004d90: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00004da0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-00004db0: 2f4f 7074 696f 6e3e 0a20 2020 2020 2020  /Option>.       
-00004dc0: 2020 203c 2f64 6174 615f 6465 6669 6e65     </data_define
-00004dd0: 645f 7072 6f70 6572 7469 6573 3e0a 2020  d_properties>.  
-00004de0: 2020 2020 2020 2020 3c6c 6179 6572 2070          <layer p
-00004df0: 6173 733d 2230 2220 6c6f 636b 6564 3d22  ass="0" locked="
-00004e00: 3022 2065 6e61 626c 6564 3d22 3122 2063  0" enabled="1" c
-00004e10: 6c61 7373 3d22 5369 6d70 6c65 4c69 6e65  lass="SimpleLine
-00004e20: 223e 0a20 2020 2020 2020 2020 2020 203c  ">.            <
-00004e30: 4f70 7469 6f6e 2074 7970 653d 224d 6170  Option type="Map
-00004e40: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00004e50: 203c 4f70 7469 6f6e 206e 616d 653d 2261   <Option name="a
-00004e60: 6c69 676e 5f64 6173 685f 7061 7474 6572  lign_dash_patter
-00004e70: 6e22 2076 616c 7565 3d22 3022 2074 7970  n" value="0" typ
-00004e80: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00004e90: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00004ea0: 696f 6e20 6e61 6d65 3d22 6361 7073 7479  ion name="capsty
-00004eb0: 6c65 2220 7661 6c75 653d 2273 7175 6172  le" value="squar
-00004ec0: 6522 2074 7970 653d 2251 5374 7269 6e67  e" type="QString
-00004ed0: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00004ee0: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
-00004ef0: 6375 7374 6f6d 6461 7368 2220 7661 6c75  customdash" valu
-00004f00: 653d 2235 3b32 2220 7479 7065 3d22 5153  e="5;2" type="QS
-00004f10: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00004f20: 2020 2020 2020 203c 4f70 7469 6f6e 206e         <Option n
-00004f30: 616d 653d 2263 7573 746f 6d64 6173 685f  ame="customdash_
-00004f40: 6d61 705f 756e 6974 5f73 6361 6c65 2220  map_unit_scale" 
-00004f50: 7661 6c75 653d 2233 783a 302c 302c 302c  value="3x:0,0,0,
-00004f60: 302c 302c 3022 2074 7970 653d 2251 5374  0,0,0" type="QSt
-00004f70: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-00004f80: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
-00004f90: 6d65 3d22 6375 7374 6f6d 6461 7368 5f75  me="customdash_u
-00004fa0: 6e69 7422 2076 616c 7565 3d22 4d4d 2220  nit" value="MM" 
-00004fb0: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
-00004fc0: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-00004fd0: 4f70 7469 6f6e 206e 616d 653d 2264 6173  Option name="das
-00004fe0: 685f 7061 7474 6572 6e5f 6f66 6673 6574  h_pattern_offset
-00004ff0: 2220 7661 6c75 653d 2230 2220 7479 7065  " value="0" type
-00005000: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-00005010: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00005020: 6f6e 206e 616d 653d 2264 6173 685f 7061  on name="dash_pa
-00005030: 7474 6572 6e5f 6f66 6673 6574 5f6d 6170  ttern_offset_map
-00005040: 5f75 6e69 745f 7363 616c 6522 2076 616c  _unit_scale" val
-00005050: 7565 3d22 3378 3a30 2c30 2c30 2c30 2c30  ue="3x:0,0,0,0,0
-00005060: 2c30 2220 7479 7065 3d22 5153 7472 696e  ,0" type="QStrin
-00005070: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
-00005080: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
-00005090: 2264 6173 685f 7061 7474 6572 6e5f 6f66  "dash_pattern_of
-000050a0: 6673 6574 5f75 6e69 7422 2076 616c 7565  fset_unit" value
-000050b0: 3d22 4d4d 2220 7479 7065 3d22 5153 7472  ="MM" type="QStr
-000050c0: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-000050d0: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
-000050e0: 653d 2264 7261 775f 696e 7369 6465 5f70  e="draw_inside_p
-000050f0: 6f6c 7967 6f6e 2220 7661 6c75 653d 2230  olygon" value="0
-00005100: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00005110: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
-00005120: 203c 4f70 7469 6f6e 206e 616d 653d 226a   <Option name="j
-00005130: 6f69 6e73 7479 6c65 2220 7661 6c75 653d  oinstyle" value=
-00005140: 2262 6576 656c 2220 7479 7065 3d22 5153  "bevel" type="QS
-00005150: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00005160: 2020 2020 2020 203c 4f70 7469 6f6e 206e         <Option n
-00005170: 616d 653d 226c 696e 655f 636f 6c6f 7222  ame="line_color"
-00005180: 2076 616c 7565 3d22 3335 2c33 352c 3335   value="35,35,35
-00005190: 2c32 3535 2220 7479 7065 3d22 5153 7472  ,255" type="QStr
-000051a0: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-000051b0: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
-000051c0: 653d 226c 696e 655f 7374 796c 6522 2076  e="line_style" v
-000051d0: 616c 7565 3d22 736f 6c69 6422 2074 7970  alue="solid" typ
-000051e0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-000051f0: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00005200: 696f 6e20 6e61 6d65 3d22 6c69 6e65 5f77  ion name="line_w
-00005210: 6964 7468 2220 7661 6c75 653d 2230 2e32  idth" value="0.2
-00005220: 3622 2074 7970 653d 2251 5374 7269 6e67  6" type="QString
-00005230: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00005240: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
-00005250: 6c69 6e65 5f77 6964 7468 5f75 6e69 7422  line_width_unit"
-00005260: 2076 616c 7565 3d22 4d4d 2220 7479 7065   value="MM" type
-00005270: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-00005280: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00005290: 6f6e 206e 616d 653d 226f 6666 7365 7422  on name="offset"
-000052a0: 2076 616c 7565 3d22 3022 2074 7970 653d   value="0" type=
-000052b0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-000052c0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-000052d0: 6e20 6e61 6d65 3d22 6f66 6673 6574 5f6d  n name="offset_m
-000052e0: 6170 5f75 6e69 745f 7363 616c 6522 2076  ap_unit_scale" v
-000052f0: 616c 7565 3d22 3378 3a30 2c30 2c30 2c30  alue="3x:0,0,0,0
-00005300: 2c30 2c30 2220 7479 7065 3d22 5153 7472  ,0,0" type="QStr
-00005310: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-00005320: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
-00005330: 653d 226f 6666 7365 745f 756e 6974 2220  e="offset_unit" 
-00005340: 7661 6c75 653d 224d 4d22 2074 7970 653d  value="MM" type=
-00005350: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-00005360: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00005370: 6e20 6e61 6d65 3d22 7269 6e67 5f66 696c  n name="ring_fil
-00005380: 7465 7222 2076 616c 7565 3d22 3022 2074  ter" value="0" t
-00005390: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
-000053a0: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
-000053b0: 7074 696f 6e20 6e61 6d65 3d22 7472 696d  ption name="trim
-000053c0: 5f64 6973 7461 6e63 655f 656e 6422 2076  _distance_end" v
-000053d0: 616c 7565 3d22 3022 2074 7970 653d 2251  alue="0" type="Q
-000053e0: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
-000053f0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00005400: 6e61 6d65 3d22 7472 696d 5f64 6973 7461  name="trim_dista
-00005410: 6e63 655f 656e 645f 6d61 705f 756e 6974  nce_end_map_unit
-00005420: 5f73 6361 6c65 2220 7661 6c75 653d 2233  _scale" value="3
-00005430: 783a 302c 302c 302c 302c 302c 3022 2074  x:0,0,0,0,0,0" t
-00005440: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
-00005450: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
-00005460: 7074 696f 6e20 6e61 6d65 3d22 7472 696d  ption name="trim
-00005470: 5f64 6973 7461 6e63 655f 656e 645f 756e  _distance_end_un
-00005480: 6974 2220 7661 6c75 653d 224d 4d22 2074  it" value="MM" t
-00005490: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
-000054a0: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
-000054b0: 7074 696f 6e20 6e61 6d65 3d22 7472 696d  ption name="trim
-000054c0: 5f64 6973 7461 6e63 655f 7374 6172 7422  _distance_start"
-000054d0: 2076 616c 7565 3d22 3022 2074 7970 653d   value="0" type=
-000054e0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-000054f0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00005500: 6e20 6e61 6d65 3d22 7472 696d 5f64 6973  n name="trim_dis
-00005510: 7461 6e63 655f 7374 6172 745f 6d61 705f  tance_start_map_
-00005520: 756e 6974 5f73 6361 6c65 2220 7661 6c75  unit_scale" valu
-00005530: 653d 2233 783a 302c 302c 302c 302c 302c  e="3x:0,0,0,0,0,
-00005540: 3022 2074 7970 653d 2251 5374 7269 6e67  0" type="QString
-00005550: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00005560: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
-00005570: 7472 696d 5f64 6973 7461 6e63 655f 7374  trim_distance_st
-00005580: 6172 745f 756e 6974 2220 7661 6c75 653d  art_unit" value=
-00005590: 224d 4d22 2074 7970 653d 2251 5374 7269  "MM" type="QStri
-000055a0: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
-000055b0: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
-000055c0: 3d22 7477 6561 6b5f 6461 7368 5f70 6174  ="tweak_dash_pat
-000055d0: 7465 726e 5f6f 6e5f 636f 726e 6572 7322  tern_on_corners"
-000055e0: 2076 616c 7565 3d22 3022 2074 7970 653d   value="0" type=
-000055f0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-00005600: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00005610: 6e20 6e61 6d65 3d22 7573 655f 6375 7374  n name="use_cust
-00005620: 6f6d 5f64 6173 6822 2076 616c 7565 3d22  om_dash" value="
-00005630: 3022 2074 7970 653d 2251 5374 7269 6e67  0" type="QString
-00005640: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00005650: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
-00005660: 7769 6474 685f 6d61 705f 756e 6974 5f73  width_map_unit_s
-00005670: 6361 6c65 2220 7661 6c75 653d 2233 783a  cale" value="3x:
-00005680: 302c 302c 302c 302c 302c 3022 2074 7970  0,0,0,0,0,0" typ
-00005690: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-000056a0: 2020 2020 2020 2020 2020 3c2f 4f70 7469            </Opti
-000056b0: 6f6e 3e0a 2020 2020 2020 2020 2020 2020  on>.            
-000056c0: 3c64 6174 615f 6465 6669 6e65 645f 7072  <data_defined_pr
-000056d0: 6f70 6572 7469 6573 3e0a 2020 2020 2020  operties>.      
-000056e0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-000056f0: 7479 7065 3d22 4d61 7022 3e0a 2020 2020  type="Map">.    
-00005700: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00005710: 696f 6e20 6e61 6d65 3d22 6e61 6d65 2220  ion name="name" 
-00005720: 7661 6c75 653d 2222 2074 7970 653d 2251  value="" type="Q
-00005730: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
-00005740: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00005750: 6e20 6e61 6d65 3d22 7072 6f70 6572 7469  n name="properti
-00005760: 6573 222f 3e0a 2020 2020 2020 2020 2020  es"/>.          
-00005770: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
-00005780: 6d65 3d22 7479 7065 2220 7661 6c75 653d  me="type" value=
-00005790: 2263 6f6c 6c65 6374 696f 6e22 2074 7970  "collection" typ
-000057a0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-000057b0: 2020 2020 2020 2020 2020 2020 3c2f 4f70              </Op
-000057c0: 7469 6f6e 3e0a 2020 2020 2020 2020 2020  tion>.          
-000057d0: 2020 3c2f 6461 7461 5f64 6566 696e 6564    </data_defined
-000057e0: 5f70 726f 7065 7274 6965 733e 0a20 2020  _properties>.   
-000057f0: 2020 2020 2020 203c 2f6c 6179 6572 3e0a         </layer>.
-00005800: 2020 2020 2020 2020 3c2f 7379 6d62 6f6c          </symbol
-00005810: 3e0a 2020 2020 2020 3c2f 6178 6973 5379  >.      </axisSy
-00005820: 6d62 6f6c 3e0a 2020 2020 3c2f 4469 6167  mbol>.    </Diag
-00005830: 7261 6d43 6174 6567 6f72 793e 0a20 203c  ramCategory>.  <
-00005840: 2f53 696e 676c 6543 6174 6567 6f72 7944  /SingleCategoryD
-00005850: 6961 6772 616d 5265 6e64 6572 6572 3e0a  iagramRenderer>.
-00005860: 2020 3c44 6961 6772 616d 4c61 7965 7253    <DiagramLayerS
-00005870: 6574 7469 6e67 7320 6469 7374 3d22 3022  ettings dist="0"
-00005880: 2073 686f 7741 6c6c 3d22 3122 206f 6273   showAll="1" obs
-00005890: 7461 636c 653d 2230 2220 706c 6163 656d  tacle="0" placem
-000058a0: 656e 743d 2230 2220 7a49 6e64 6578 3d22  ent="0" zIndex="
-000058b0: 3022 2070 7269 6f72 6974 793d 2230 2220  0" priority="0" 
-000058c0: 6c69 6e65 506c 6163 656d 656e 7446 6c61  linePlacementFla
-000058d0: 6773 3d22 3138 223e 0a20 2020 203c 7072  gs="18">.    <pr
-000058e0: 6f70 6572 7469 6573 3e0a 2020 2020 2020  operties>.      
-000058f0: 3c4f 7074 696f 6e20 7479 7065 3d22 4d61  <Option type="Ma
-00005900: 7022 3e0a 2020 2020 2020 2020 3c4f 7074  p">.        <Opt
-00005910: 696f 6e20 6e61 6d65 3d22 6e61 6d65 2220  ion name="name" 
-00005920: 7661 6c75 653d 2222 2074 7970 653d 2251  value="" type="Q
-00005930: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
-00005940: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
-00005950: 7072 6f70 6572 7469 6573 222f 3e0a 2020  properties"/>.  
-00005960: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
-00005970: 6d65 3d22 7479 7065 2220 7661 6c75 653d  me="type" value=
-00005980: 2263 6f6c 6c65 6374 696f 6e22 2074 7970  "collection" typ
-00005990: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-000059a0: 2020 2020 3c2f 4f70 7469 6f6e 3e0a 2020      </Option>.  
-000059b0: 2020 3c2f 7072 6f70 6572 7469 6573 3e0a    </properties>.
-000059c0: 2020 3c2f 4469 6167 7261 6d4c 6179 6572    </DiagramLayer
-000059d0: 5365 7474 696e 6773 3e0a 2020 3c67 656f  Settings>.  <geo
-000059e0: 6d65 7472 794f 7074 696f 6e73 2072 656d  metryOptions rem
-000059f0: 6f76 6544 7570 6c69 6361 7465 4e6f 6465  oveDuplicateNode
-00005a00: 733d 2230 2220 6765 6f6d 6574 7279 5072  s="0" geometryPr
-00005a10: 6563 6973 696f 6e3d 2230 223e 0a20 2020  ecision="0">.   
-00005a20: 203c 6163 7469 7665 4368 6563 6b73 2f3e   <activeChecks/>
-00005a30: 0a20 2020 203c 6368 6563 6b43 6f6e 6669  .    <checkConfi
-00005a40: 6775 7261 7469 6f6e 2f3e 0a20 203c 2f67  guration/>.  </g
-00005a50: 656f 6d65 7472 794f 7074 696f 6e73 3e0a  eometryOptions>.
-00005a60: 2020 3c6c 6567 656e 6420 7368 6f77 4c61    <legend showLa
-00005a70: 6265 6c4c 6567 656e 643d 2230 2220 7479  belLegend="0" ty
-00005a80: 7065 3d22 6465 6661 756c 742d 7665 6374  pe="default-vect
-00005a90: 6f72 222f 3e0a 2020 3c72 6566 6572 656e  or"/>.  <referen
-00005aa0: 6365 644c 6179 6572 732f 3e0a 2020 3c66  cedLayers/>.  <f
-00005ab0: 6965 6c64 436f 6e66 6967 7572 6174 696f  ieldConfiguratio
-00005ac0: 6e3e 0a20 2020 203c 6669 656c 6420 6e61  n>.    <field na
-00005ad0: 6d65 3d22 7479 7065 2220 636f 6e66 6967  me="type" config
-00005ae0: 7572 6174 696f 6e46 6c61 6773 3d22 4e6f  urationFlags="No
-00005af0: 6e65 223e 0a20 2020 2020 203c 6564 6974  ne">.      <edit
-00005b00: 5769 6467 6574 2074 7970 653d 2254 6578  Widget type="Tex
-00005b10: 7445 6469 7422 3e0a 2020 2020 2020 2020  tEdit">.        
-00005b20: 3c63 6f6e 6669 673e 0a20 2020 2020 2020  <config>.       
-00005b30: 2020 203c 4f70 7469 6f6e 2f3e 0a20 2020     <Option/>.   
-00005b40: 2020 2020 203c 2f63 6f6e 6669 673e 0a20       </config>. 
-00005b50: 2020 2020 203c 2f65 6469 7457 6964 6765       </editWidge
-00005b60: 743e 0a20 2020 203c 2f66 6965 6c64 3e0a  t>.    </field>.
-00005b70: 2020 2020 3c66 6965 6c64 206e 616d 653d      <field name=
-00005b80: 226f 736d 5f69 6422 2063 6f6e 6669 6775  "osm_id" configu
-00005b90: 7261 7469 6f6e 466c 6167 733d 224e 6f6e  rationFlags="Non
-00005ba0: 6522 3e0a 2020 2020 2020 3c65 6469 7457  e">.      <editW
-00005bb0: 6964 6765 7420 7479 7065 3d22 5465 7874  idget type="Text
-00005bc0: 4564 6974 223e 0a20 2020 2020 2020 203c  Edit">.        <
-00005bd0: 636f 6e66 6967 3e0a 2020 2020 2020 2020  config>.        
-00005be0: 2020 3c4f 7074 696f 6e2f 3e0a 2020 2020    <Option/>.    
-00005bf0: 2020 2020 3c2f 636f 6e66 6967 3e0a 2020      </config>.  
-00005c00: 2020 2020 3c2f 6564 6974 5769 6467 6574      </editWidget
-00005c10: 3e0a 2020 2020 3c2f 6669 656c 643e 0a20  >.    </field>. 
-00005c20: 2020 203c 6669 656c 6420 6e61 6d65 3d22     <field name="
-00005c30: 6f72 6965 6e74 6174 696f 6e22 2063 6f6e  orientation" con
-00005c40: 6669 6775 7261 7469 6f6e 466c 6167 733d  figurationFlags=
-00005c50: 224e 6f6e 6522 3e0a 2020 2020 2020 3c65  "None">.      <e
-00005c60: 6469 7457 6964 6765 7420 7479 7065 3d22  ditWidget type="
-00005c70: 5465 7874 4564 6974 223e 0a20 2020 2020  TextEdit">.     
-00005c80: 2020 203c 636f 6e66 6967 3e0a 2020 2020     <config>.    
-00005c90: 2020 2020 2020 3c4f 7074 696f 6e2f 3e0a        <Option/>.
-00005ca0: 2020 2020 2020 2020 3c2f 636f 6e66 6967          </config
-00005cb0: 3e0a 2020 2020 2020 3c2f 6564 6974 5769  >.      </editWi
-00005cc0: 6467 6574 3e0a 2020 2020 3c2f 6669 656c  dget>.    </fiel
-00005cd0: 643e 0a20 2020 203c 6669 656c 6420 6e61  d>.    <field na
-00005ce0: 6d65 3d22 6f72 6965 6e74 6174 696f 6e5f  me="orientation_
-00005cf0: 636f 6e66 6964 656e 6365 2220 636f 6e66  confidence" conf
-00005d00: 6967 7572 6174 696f 6e46 6c61 6773 3d22  igurationFlags="
-00005d10: 4e6f 6e65 223e 0a20 2020 2020 203c 6564  None">.      <ed
-00005d20: 6974 5769 6467 6574 2074 7970 653d 2254  itWidget type="T
-00005d30: 6578 7445 6469 7422 3e0a 2020 2020 2020  extEdit">.      
-00005d40: 2020 3c63 6f6e 6669 673e 0a20 2020 2020    <config>.     
-00005d50: 2020 2020 203c 4f70 7469 6f6e 2f3e 0a20       <Option/>. 
-00005d60: 2020 2020 2020 203c 2f63 6f6e 6669 673e         </config>
-00005d70: 0a20 2020 2020 203c 2f65 6469 7457 6964  .      </editWid
-00005d80: 6765 743e 0a20 2020 203c 2f66 6965 6c64  get>.    </field
-00005d90: 3e0a 2020 2020 3c66 6965 6c64 206e 616d  >.    <field nam
-00005da0: 653d 226c 616e 655f 7769 6474 6822 2063  e="lane_width" c
-00005db0: 6f6e 6669 6775 7261 7469 6f6e 466c 6167  onfigurationFlag
-00005dc0: 733d 224e 6f6e 6522 3e0a 2020 2020 2020  s="None">.      
-00005dd0: 3c65 6469 7457 6964 6765 7420 7479 7065  <editWidget type
-00005de0: 3d22 5465 7874 4564 6974 223e 0a20 2020  ="TextEdit">.   
-00005df0: 2020 2020 203c 636f 6e66 6967 3e0a 2020       <config>.  
-00005e00: 2020 2020 2020 2020 3c4f 7074 696f 6e2f          <Option/
-00005e10: 3e0a 2020 2020 2020 2020 3c2f 636f 6e66  >.        </conf
-00005e20: 6967 3e0a 2020 2020 2020 3c2f 6564 6974  ig>.      </edit
-00005e30: 5769 6467 6574 3e0a 2020 2020 3c2f 6669  Widget>.    </fi
-00005e40: 656c 643e 0a20 2020 203c 6669 656c 6420  eld>.    <field 
-00005e50: 6e61 6d65 3d22 6c61 6e65 5f6f 7269 656e  name="lane_orien
-00005e60: 7461 7469 6f6e 2220 636f 6e66 6967 7572  tation" configur
-00005e70: 6174 696f 6e46 6c61 6773 3d22 4e6f 6e65  ationFlags="None
-00005e80: 223e 0a20 2020 2020 203c 6564 6974 5769  ">.      <editWi
-00005e90: 6467 6574 2074 7970 653d 2254 6578 7445  dget type="TextE
-00005ea0: 6469 7422 3e0a 2020 2020 2020 2020 3c63  dit">.        <c
-00005eb0: 6f6e 6669 673e 0a20 2020 2020 2020 2020  onfig>.         
-00005ec0: 203c 4f70 7469 6f6e 2f3e 0a20 2020 2020   <Option/>.     
-00005ed0: 2020 203c 2f63 6f6e 6669 673e 0a20 2020     </config>.   
-00005ee0: 2020 203c 2f65 6469 7457 6964 6765 743e     </editWidget>
-00005ef0: 0a20 2020 203c 2f66 6965 6c64 3e0a 2020  .    </field>.  
-00005f00: 3c2f 6669 656c 6443 6f6e 6669 6775 7261  </fieldConfigura
-00005f10: 7469 6f6e 3e0a 2020 3c61 6c69 6173 6573  tion>.  <aliases
-00005f20: 3e0a 2020 2020 3c61 6c69 6173 206e 616d  >.    <alias nam
-00005f30: 653d 2222 2069 6e64 6578 3d22 3022 2066  e="" index="0" f
-00005f40: 6965 6c64 3d22 7479 7065 222f 3e0a 2020  ield="type"/>.  
-00005f50: 2020 3c61 6c69 6173 206e 616d 653d 2222    <alias name=""
-00005f60: 2069 6e64 6578 3d22 3122 2066 6965 6c64   index="1" field
-00005f70: 3d22 6f73 6d5f 6964 222f 3e0a 2020 2020  ="osm_id"/>.    
-00005f80: 3c61 6c69 6173 206e 616d 653d 2222 2069  <alias name="" i
-00005f90: 6e64 6578 3d22 3222 2066 6965 6c64 3d22  ndex="2" field="
-00005fa0: 6f72 6965 6e74 6174 696f 6e22 2f3e 0a20  orientation"/>. 
-00005fb0: 2020 203c 616c 6961 7320 6e61 6d65 3d22     <alias name="
-00005fc0: 2220 696e 6465 783d 2233 2220 6669 656c  " index="3" fiel
-00005fd0: 643d 226f 7269 656e 7461 7469 6f6e 5f63  d="orientation_c
-00005fe0: 6f6e 6669 6465 6e63 6522 2f3e 0a20 2020  onfidence"/>.   
-00005ff0: 203c 616c 6961 7320 6e61 6d65 3d22 2220   <alias name="" 
-00006000: 696e 6465 783d 2234 2220 6669 656c 643d  index="4" field=
-00006010: 226c 616e 655f 7769 6474 6822 2f3e 0a20  "lane_width"/>. 
-00006020: 2020 203c 616c 6961 7320 6e61 6d65 3d22     <alias name="
-00006030: 2220 696e 6465 783d 2235 2220 6669 656c  " index="5" fiel
-00006040: 643d 226c 616e 655f 6f72 6965 6e74 6174  d="lane_orientat
-00006050: 696f 6e22 2f3e 0a20 203c 2f61 6c69 6173  ion"/>.  </alias
-00006060: 6573 3e0a 2020 3c64 6566 6175 6c74 733e  es>.  <defaults>
-00006070: 0a20 2020 203c 6465 6661 756c 7420 6669  .    <default fi
-00006080: 656c 643d 2274 7970 6522 2061 7070 6c79  eld="type" apply
-00006090: 4f6e 5570 6461 7465 3d22 3022 2065 7870  OnUpdate="0" exp
-000060a0: 7265 7373 696f 6e3d 2222 2f3e 0a20 2020  ression=""/>.   
-000060b0: 203c 6465 6661 756c 7420 6669 656c 643d   <default field=
-000060c0: 226f 736d 5f69 6422 2061 7070 6c79 4f6e  "osm_id" applyOn
-000060d0: 5570 6461 7465 3d22 3022 2065 7870 7265  Update="0" expre
-000060e0: 7373 696f 6e3d 2222 2f3e 0a20 2020 203c  ssion=""/>.    <
-000060f0: 6465 6661 756c 7420 6669 656c 643d 226f  default field="o
-00006100: 7269 656e 7461 7469 6f6e 2220 6170 706c  rientation" appl
-00006110: 794f 6e55 7064 6174 653d 2230 2220 6578  yOnUpdate="0" ex
-00006120: 7072 6573 7369 6f6e 3d22 222f 3e0a 2020  pression=""/>.  
-00006130: 2020 3c64 6566 6175 6c74 2066 6965 6c64    <default field
-00006140: 3d22 6f72 6965 6e74 6174 696f 6e5f 636f  ="orientation_co
-00006150: 6e66 6964 656e 6365 2220 6170 706c 794f  nfidence" applyO
-00006160: 6e55 7064 6174 653d 2230 2220 6578 7072  nUpdate="0" expr
-00006170: 6573 7369 6f6e 3d22 222f 3e0a 2020 2020  ession=""/>.    
-00006180: 3c64 6566 6175 6c74 2066 6965 6c64 3d22  <default field="
-00006190: 6c61 6e65 5f77 6964 7468 2220 6170 706c  lane_width" appl
-000061a0: 794f 6e55 7064 6174 653d 2230 2220 6578  yOnUpdate="0" ex
-000061b0: 7072 6573 7369 6f6e 3d22 222f 3e0a 2020  pression=""/>.  
-000061c0: 2020 3c64 6566 6175 6c74 2066 6965 6c64    <default field
-000061d0: 3d22 6c61 6e65 5f6f 7269 656e 7461 7469  ="lane_orientati
-000061e0: 6f6e 2220 6170 706c 794f 6e55 7064 6174  on" applyOnUpdat
-000061f0: 653d 2230 2220 6578 7072 6573 7369 6f6e  e="0" expression
-00006200: 3d22 222f 3e0a 2020 3c2f 6465 6661 756c  =""/>.  </defaul
-00006210: 7473 3e0a 2020 3c63 6f6e 7374 7261 696e  ts>.  <constrain
-00006220: 7473 3e0a 2020 2020 3c63 6f6e 7374 7261  ts>.    <constra
-00006230: 696e 7420 6e6f 746e 756c 6c5f 7374 7265  int notnull_stre
-00006240: 6e67 7468 3d22 3022 2063 6f6e 7374 7261  ngth="0" constra
-00006250: 696e 7473 3d22 3022 2075 6e69 7175 655f  ints="0" unique_
-00006260: 7374 7265 6e67 7468 3d22 3022 2066 6965  strength="0" fie
-00006270: 6c64 3d22 7479 7065 2220 6578 705f 7374  ld="type" exp_st
-00006280: 7265 6e67 7468 3d22 3022 2f3e 0a20 2020  rength="0"/>.   
-00006290: 203c 636f 6e73 7472 6169 6e74 206e 6f74   <constraint not
-000062a0: 6e75 6c6c 5f73 7472 656e 6774 683d 2230  null_strength="0
-000062b0: 2220 636f 6e73 7472 6169 6e74 733d 2230  " constraints="0
-000062c0: 2220 756e 6971 7565 5f73 7472 656e 6774  " unique_strengt
-000062d0: 683d 2230 2220 6669 656c 643d 226f 736d  h="0" field="osm
-000062e0: 5f69 6422 2065 7870 5f73 7472 656e 6774  _id" exp_strengt
-000062f0: 683d 2230 222f 3e0a 2020 2020 3c63 6f6e  h="0"/>.    <con
-00006300: 7374 7261 696e 7420 6e6f 746e 756c 6c5f  straint notnull_
-00006310: 7374 7265 6e67 7468 3d22 3022 2063 6f6e  strength="0" con
-00006320: 7374 7261 696e 7473 3d22 3022 2075 6e69  straints="0" uni
-00006330: 7175 655f 7374 7265 6e67 7468 3d22 3022  que_strength="0"
-00006340: 2066 6965 6c64 3d22 6f72 6965 6e74 6174   field="orientat
-00006350: 696f 6e22 2065 7870 5f73 7472 656e 6774  ion" exp_strengt
-00006360: 683d 2230 222f 3e0a 2020 2020 3c63 6f6e  h="0"/>.    <con
-00006370: 7374 7261 696e 7420 6e6f 746e 756c 6c5f  straint notnull_
-00006380: 7374 7265 6e67 7468 3d22 3022 2063 6f6e  strength="0" con
-00006390: 7374 7261 696e 7473 3d22 3022 2075 6e69  straints="0" uni
-000063a0: 7175 655f 7374 7265 6e67 7468 3d22 3022  que_strength="0"
-000063b0: 2066 6965 6c64 3d22 6f72 6965 6e74 6174   field="orientat
-000063c0: 696f 6e5f 636f 6e66 6964 656e 6365 2220  ion_confidence" 
-000063d0: 6578 705f 7374 7265 6e67 7468 3d22 3022  exp_strength="0"
-000063e0: 2f3e 0a20 2020 203c 636f 6e73 7472 6169  />.    <constrai
-000063f0: 6e74 206e 6f74 6e75 6c6c 5f73 7472 656e  nt notnull_stren
-00006400: 6774 683d 2230 2220 636f 6e73 7472 6169  gth="0" constrai
-00006410: 6e74 733d 2230 2220 756e 6971 7565 5f73  nts="0" unique_s
-00006420: 7472 656e 6774 683d 2230 2220 6669 656c  trength="0" fiel
-00006430: 643d 226c 616e 655f 7769 6474 6822 2065  d="lane_width" e
-00006440: 7870 5f73 7472 656e 6774 683d 2230 222f  xp_strength="0"/
-00006450: 3e0a 2020 2020 3c63 6f6e 7374 7261 696e  >.    <constrain
-00006460: 7420 6e6f 746e 756c 6c5f 7374 7265 6e67  t notnull_streng
-00006470: 7468 3d22 3022 2063 6f6e 7374 7261 696e  th="0" constrain
-00006480: 7473 3d22 3022 2075 6e69 7175 655f 7374  ts="0" unique_st
-00006490: 7265 6e67 7468 3d22 3022 2066 6965 6c64  rength="0" field
-000064a0: 3d22 6c61 6e65 5f6f 7269 656e 7461 7469  ="lane_orientati
-000064b0: 6f6e 2220 6578 705f 7374 7265 6e67 7468  on" exp_strength
-000064c0: 3d22 3022 2f3e 0a20 203c 2f63 6f6e 7374  ="0"/>.  </const
-000064d0: 7261 696e 7473 3e0a 2020 3c63 6f6e 7374  raints>.  <const
-000064e0: 7261 696e 7445 7870 7265 7373 696f 6e73  raintExpressions
-000064f0: 3e0a 2020 2020 3c63 6f6e 7374 7261 696e  >.    <constrain
-00006500: 7420 6578 703d 2222 2064 6573 633d 2222  t exp="" desc=""
-00006510: 2066 6965 6c64 3d22 7479 7065 222f 3e0a   field="type"/>.
-00006520: 2020 2020 3c63 6f6e 7374 7261 696e 7420      <constraint 
-00006530: 6578 703d 2222 2064 6573 633d 2222 2066  exp="" desc="" f
-00006540: 6965 6c64 3d22 6f73 6d5f 6964 222f 3e0a  ield="osm_id"/>.
-00006550: 2020 2020 3c63 6f6e 7374 7261 696e 7420      <constraint 
-00006560: 6578 703d 2222 2064 6573 633d 2222 2066  exp="" desc="" f
-00006570: 6965 6c64 3d22 6f72 6965 6e74 6174 696f  ield="orientatio
-00006580: 6e22 2f3e 0a20 2020 203c 636f 6e73 7472  n"/>.    <constr
-00006590: 6169 6e74 2065 7870 3d22 2220 6465 7363  aint exp="" desc
-000065a0: 3d22 2220 6669 656c 643d 226f 7269 656e  ="" field="orien
-000065b0: 7461 7469 6f6e 5f63 6f6e 6669 6465 6e63  tation_confidenc
-000065c0: 6522 2f3e 0a20 2020 203c 636f 6e73 7472  e"/>.    <constr
-000065d0: 6169 6e74 2065 7870 3d22 2220 6465 7363  aint exp="" desc
-000065e0: 3d22 2220 6669 656c 643d 226c 616e 655f  ="" field="lane_
-000065f0: 7769 6474 6822 2f3e 0a20 2020 203c 636f  width"/>.    <co
-00006600: 6e73 7472 6169 6e74 2065 7870 3d22 2220  nstraint exp="" 
-00006610: 6465 7363 3d22 2220 6669 656c 643d 226c  desc="" field="l
-00006620: 616e 655f 6f72 6965 6e74 6174 696f 6e22  ane_orientation"
-00006630: 2f3e 0a20 203c 2f63 6f6e 7374 7261 696e  />.  </constrain
-00006640: 7445 7870 7265 7373 696f 6e73 3e0a 2020  tExpressions>.  
-00006650: 3c65 7870 7265 7373 696f 6e66 6965 6c64  <expressionfield
-00006660: 732f 3e0a 2020 3c61 7474 7269 6275 7465  s/>.  <attribute
-00006670: 6163 7469 6f6e 733e 0a20 2020 203c 6465  actions>.    <de
-00006680: 6661 756c 7441 6374 696f 6e20 6b65 793d  faultAction key=
-00006690: 2243 616e 7661 7322 2076 616c 7565 3d22  "Canvas" value="
-000066a0: 7b30 3030 3030 3030 302d 3030 3030 2d30  {00000000-0000-0
-000066b0: 3030 302d 3030 3030 2d30 3030 3030 3030  000-0000-0000000
-000066c0: 3030 3030 307d 222f 3e0a 2020 3c2f 6174  00000}"/>.  </at
-000066d0: 7472 6962 7574 6561 6374 696f 6e73 3e0a  tributeactions>.
-000066e0: 2020 3c61 7474 7269 6275 7465 7461 626c    <attributetabl
-000066f0: 6563 6f6e 6669 6720 736f 7274 4578 7072  econfig sortExpr
-00006700: 6573 7369 6f6e 3d22 2220 736f 7274 4f72  ession="" sortOr
-00006710: 6465 723d 2230 2220 6163 7469 6f6e 5769  der="0" actionWi
-00006720: 6467 6574 5374 796c 653d 2264 726f 7044  dgetStyle="dropD
-00006730: 6f77 6e22 3e0a 2020 2020 3c63 6f6c 756d  own">.    <colum
-00006740: 6e73 3e0a 2020 2020 2020 3c63 6f6c 756d  ns>.      <colum
-00006750: 6e20 6e61 6d65 3d22 7479 7065 2220 7769  n name="type" wi
-00006760: 6474 683d 222d 3122 2068 6964 6465 6e3d  dth="-1" hidden=
-00006770: 2230 2220 7479 7065 3d22 6669 656c 6422  "0" type="field"
-00006780: 2f3e 0a20 2020 2020 203c 636f 6c75 6d6e  />.      <column
-00006790: 206e 616d 653d 226f 736d 5f69 6422 2077   name="osm_id" w
-000067a0: 6964 7468 3d22 3137 3122 2068 6964 6465  idth="171" hidde
-000067b0: 6e3d 2230 2220 7479 7065 3d22 6669 656c  n="0" type="fiel
-000067c0: 6422 2f3e 0a20 2020 2020 203c 636f 6c75  d"/>.      <colu
-000067d0: 6d6e 206e 616d 653d 226f 7269 656e 7461  mn name="orienta
-000067e0: 7469 6f6e 2220 7769 6474 683d 2232 3932  tion" width="292
-000067f0: 2220 6869 6464 656e 3d22 3022 2074 7970  " hidden="0" typ
-00006800: 653d 2266 6965 6c64 222f 3e0a 2020 2020  e="field"/>.    
-00006810: 2020 3c63 6f6c 756d 6e20 6e61 6d65 3d22    <column name="
-00006820: 6f72 6965 6e74 6174 696f 6e5f 636f 6e66  orientation_conf
-00006830: 6964 656e 6365 2220 7769 6474 683d 222d  idence" width="-
-00006840: 3122 2068 6964 6465 6e3d 2230 2220 7479  1" hidden="0" ty
-00006850: 7065 3d22 6669 656c 6422 2f3e 0a20 2020  pe="field"/>.   
-00006860: 2020 203c 636f 6c75 6d6e 206e 616d 653d     <column name=
-00006870: 226c 616e 655f 6f72 6965 6e74 6174 696f  "lane_orientatio
-00006880: 6e22 2077 6964 7468 3d22 2d31 2220 6869  n" width="-1" hi
-00006890: 6464 656e 3d22 3022 2074 7970 653d 2266  dden="0" type="f
-000068a0: 6965 6c64 222f 3e0a 2020 2020 2020 3c63  ield"/>.      <c
-000068b0: 6f6c 756d 6e20 6e61 6d65 3d22 6c61 6e65  olumn name="lane
-000068c0: 5f77 6964 7468 2220 7769 6474 683d 222d  _width" width="-
-000068d0: 3122 2068 6964 6465 6e3d 2230 2220 7479  1" hidden="0" ty
-000068e0: 7065 3d22 6669 656c 6422 2f3e 0a20 2020  pe="field"/>.   
-000068f0: 2020 203c 636f 6c75 6d6e 2077 6964 7468     <column width
-00006900: 3d22 2d31 2220 6869 6464 656e 3d22 3122  ="-1" hidden="1"
-00006910: 2074 7970 653d 2261 6374 696f 6e73 222f   type="actions"/
-00006920: 3e0a 2020 2020 3c2f 636f 6c75 6d6e 733e  >.    </columns>
-00006930: 0a20 203c 2f61 7474 7269 6275 7465 7461  .  </attributeta
-00006940: 626c 6563 6f6e 6669 673e 0a20 203c 636f  bleconfig>.  <co
-00006950: 6e64 6974 696f 6e61 6c73 7479 6c65 733e  nditionalstyles>
-00006960: 0a20 2020 203c 726f 7773 7479 6c65 732f  .    <rowstyles/
-00006970: 3e0a 2020 2020 3c66 6965 6c64 7374 796c  >.    <fieldstyl
-00006980: 6573 2f3e 0a20 203c 2f63 6f6e 6469 7469  es/>.  </conditi
-00006990: 6f6e 616c 7374 796c 6573 3e0a 2020 3c73  onalstyles>.  <s
-000069a0: 746f 7265 6465 7870 7265 7373 696f 6e73  toredexpressions
-000069b0: 2f3e 0a20 203c 6564 6974 666f 726d 2074  />.  <editform t
-000069c0: 6f6c 6572 616e 743d 2231 223e 3c2f 6564  olerant="1"></ed
-000069d0: 6974 666f 726d 3e0a 2020 3c65 6469 7466  itform>.  <editf
-000069e0: 6f72 6d69 6e69 742f 3e0a 2020 3c65 6469  orminit/>.  <edi
-000069f0: 7466 6f72 6d69 6e69 7463 6f64 6573 6f75  tforminitcodesou
-00006a00: 7263 653e 303c 2f65 6469 7466 6f72 6d69  rce>0</editformi
-00006a10: 6e69 7463 6f64 6573 6f75 7263 653e 0a20  nitcodesource>. 
-00006a20: 203c 6564 6974 666f 726d 696e 6974 6669   <editforminitfi
-00006a30: 6c65 7061 7468 3e3c 2f65 6469 7466 6f72  lepath></editfor
-00006a40: 6d69 6e69 7466 696c 6570 6174 683e 0a20  minitfilepath>. 
-00006a50: 203c 6564 6974 666f 726d 696e 6974 636f   <editforminitco
-00006a60: 6465 3e3c 215b 4344 4154 415b 2320 2d2a  de><![CDATA[# -*
-00006a70: 2d20 636f 6469 6e67 3a20 7574 662d 3820  - coding: utf-8 
-00006a80: 2d2a 2d0a 2222 220a 4c65 7320 666f 726d  -*-.""".Les form
-00006a90: 756c 6169 7265 7320 5147 4953 2070 6575  ulaires QGIS peu
-00006aa0: 7665 6e74 2061 766f 6972 2075 6e65 2066  vent avoir une f
-00006ab0: 6f6e 6374 696f 6e20 5079 7468 6f6e 2071  onction Python q
-00006ac0: 7569 2065 7374 2061 7070 656c c3a9 6520  ui est appel..e 
-00006ad0: 6c6f 7273 7175 6520 6c65 2066 6f72 6d75  lorsque le formu
-00006ae0: 6c61 6972 6520 6573 740a 6f75 7665 7274  laire est.ouvert
-00006af0: 2e0a 0a55 7469 6c69 7365 7a20 6365 7474  ...Utilisez cett
-00006b00: 6520 666f 6e63 7469 6f6e 2070 6f75 7220  e fonction pour 
-00006b10: 616a 6f75 7465 7220 756e 6520 6c6f 6769  ajouter une logi
-00006b20: 7175 6520 7375 7070 6cc3 a96d 656e 7461  que suppl..menta
-00006b30: 6972 6520 c3a0 2076 6f73 2066 6f72 6d75  ire .. vos formu
-00006b40: 6c61 6972 6573 2e0a 0a45 6e74 7265 7a20  laires...Entrez 
-00006b50: 6c65 206e 6f6d 2064 6520 6c61 2066 6f6e  le nom de la fon
-00006b60: 6374 696f 6e20 6461 6e73 206c 6520 6368  ction dans le ch
-00006b70: 616d 7020 0a22 466f 6e63 7469 6f6e 2064  amp ."Fonction d
-00006b80: 2769 6e69 7469 616c 6973 6174 696f 6e20  'initialisation 
-00006b90: 5079 7468 6f6e 222e 0a56 6f69 6369 2075  Python"..Voici u
-00006ba0: 6e20 6578 656d 706c 653a 0a22 2222 0a66  n exemple:.""".f
-00006bb0: 726f 6d20 7167 6973 2e50 7951 742e 5174  rom qgis.PyQt.Qt
-00006bc0: 5769 6467 6574 7320 696d 706f 7274 2051  Widgets import Q
-00006bd0: 5769 6467 6574 0a0a 6465 6620 6d79 5f66  Widget..def my_f
-00006be0: 6f72 6d5f 6f70 656e 2864 6961 6c6f 672c  orm_open(dialog,
-00006bf0: 206c 6179 6572 2c20 6665 6174 7572 6529   layer, feature)
-00006c00: 3a0a 2020 2020 6765 6f6d 203d 2066 6561  :.    geom = fea
-00006c10: 7475 7265 2e67 656f 6d65 7472 7928 290a  ture.geometry().
-00006c20: 2020 2020 636f 6e74 726f 6c20 3d20 6469      control = di
-00006c30: 616c 6f67 2e66 696e 6443 6869 6c64 2851  alog.findChild(Q
-00006c40: 5769 6467 6574 2c20 224d 794c 696e 6545  Widget, "MyLineE
-00006c50: 6469 7422 290a 5d5d 3e3c 2f65 6469 7466  dit").]]></editf
-00006c60: 6f72 6d69 6e69 7463 6f64 653e 0a20 203c  orminitcode>.  <
-00006c70: 6665 6174 666f 726d 7375 7070 7265 7373  featformsuppress
-00006c80: 3e30 3c2f 6665 6174 666f 726d 7375 7070  >0</featformsupp
-00006c90: 7265 7373 3e0a 2020 3c65 6469 746f 726c  ress>.  <editorl
-00006ca0: 6179 6f75 743e 6765 6e65 7261 7465 646c  ayout>generatedl
-00006cb0: 6179 6f75 743c 2f65 6469 746f 726c 6179  ayout</editorlay
-00006cc0: 6f75 743e 0a20 203c 6564 6974 6162 6c65  out>.  <editable
-00006cd0: 3e0a 2020 2020 3c66 6965 6c64 206e 616d  >.    <field nam
-00006ce0: 653d 2261 6e67 6c65 2220 6564 6974 6162  e="angle" editab
-00006cf0: 6c65 3d22 3122 2f3e 0a20 2020 203c 6669  le="1"/>.    <fi
-00006d00: 656c 6420 6e61 6d65 3d22 6669 6422 2065  eld name="fid" e
-00006d10: 6469 7461 626c 653d 2231 222f 3e0a 2020  ditable="1"/>.  
-00006d20: 2020 3c66 6965 6c64 206e 616d 653d 226c    <field name="l
-00006d30: 616e 655f 6f72 6965 6e74 6174 696f 6e22  ane_orientation"
-00006d40: 2065 6469 7461 626c 653d 2231 222f 3e0a   editable="1"/>.
-00006d50: 2020 2020 3c66 6965 6c64 206e 616d 653d      <field name=
-00006d60: 226c 616e 655f 7769 6474 6822 2065 6469  "lane_width" edi
-00006d70: 7461 626c 653d 2231 222f 3e0a 2020 2020  table="1"/>.    
-00006d80: 3c66 6965 6c64 206e 616d 653d 226f 7269  <field name="ori
-00006d90: 656e 7461 7469 6f6e 2220 6564 6974 6162  entation" editab
-00006da0: 6c65 3d22 3122 2f3e 0a20 2020 203c 6669  le="1"/>.    <fi
-00006db0: 656c 6420 6e61 6d65 3d22 6f72 6965 6e74  eld name="orient
-00006dc0: 6174 696f 6e5f 636f 6e66 6964 656e 6365  ation_confidence
-00006dd0: 2220 6564 6974 6162 6c65 3d22 3122 2f3e  " editable="1"/>
-00006de0: 0a20 2020 203c 6669 656c 6420 6e61 6d65  .    <field name
-00006df0: 3d22 6f73 6d5f 6964 2220 6564 6974 6162  ="osm_id" editab
-00006e00: 6c65 3d22 3122 2f3e 0a20 2020 203c 6669  le="1"/>.    <fi
-00006e10: 656c 6420 6e61 6d65 3d22 7479 7065 2220  eld name="type" 
-00006e20: 6564 6974 6162 6c65 3d22 3122 2f3e 0a20  editable="1"/>. 
-00006e30: 203c 2f65 6469 7461 626c 653e 0a20 203c   </editable>.  <
-00006e40: 6c61 6265 6c4f 6e54 6f70 3e0a 2020 2020  labelOnTop>.    
-00006e50: 3c66 6965 6c64 206e 616d 653d 2261 6e67  <field name="ang
-00006e60: 6c65 2220 6c61 6265 6c4f 6e54 6f70 3d22  le" labelOnTop="
-00006e70: 3022 2f3e 0a20 2020 203c 6669 656c 6420  0"/>.    <field 
-00006e80: 6e61 6d65 3d22 6669 6422 206c 6162 656c  name="fid" label
-00006e90: 4f6e 546f 703d 2230 222f 3e0a 2020 2020  OnTop="0"/>.    
-00006ea0: 3c66 6965 6c64 206e 616d 653d 226c 616e  <field name="lan
-00006eb0: 655f 6f72 6965 6e74 6174 696f 6e22 206c  e_orientation" l
-00006ec0: 6162 656c 4f6e 546f 703d 2230 222f 3e0a  abelOnTop="0"/>.
-00006ed0: 2020 2020 3c66 6965 6c64 206e 616d 653d      <field name=
-00006ee0: 226c 616e 655f 7769 6474 6822 206c 6162  "lane_width" lab
-00006ef0: 656c 4f6e 546f 703d 2230 222f 3e0a 2020  elOnTop="0"/>.  
-00006f00: 2020 3c66 6965 6c64 206e 616d 653d 226f    <field name="o
-00006f10: 7269 656e 7461 7469 6f6e 2220 6c61 6265  rientation" labe
-00006f20: 6c4f 6e54 6f70 3d22 3022 2f3e 0a20 2020  lOnTop="0"/>.   
-00006f30: 203c 6669 656c 6420 6e61 6d65 3d22 6f72   <field name="or
-00006f40: 6965 6e74 6174 696f 6e5f 636f 6e66 6964  ientation_confid
-00006f50: 656e 6365 2220 6c61 6265 6c4f 6e54 6f70  ence" labelOnTop
-00006f60: 3d22 3022 2f3e 0a20 2020 203c 6669 656c  ="0"/>.    <fiel
-00006f70: 6420 6e61 6d65 3d22 6f73 6d5f 6964 2220  d name="osm_id" 
-00006f80: 6c61 6265 6c4f 6e54 6f70 3d22 3022 2f3e  labelOnTop="0"/>
-00006f90: 0a20 2020 203c 6669 656c 6420 6e61 6d65  .    <field name
-00006fa0: 3d22 7479 7065 2220 6c61 6265 6c4f 6e54  ="type" labelOnT
-00006fb0: 6f70 3d22 3022 2f3e 0a20 203c 2f6c 6162  op="0"/>.  </lab
-00006fc0: 656c 4f6e 546f 703e 0a20 203c 7265 7573  elOnTop>.  <reus
-00006fd0: 654c 6173 7456 616c 7565 3e0a 2020 2020  eLastValue>.    
-00006fe0: 3c66 6965 6c64 206e 616d 653d 2261 6e67  <field name="ang
-00006ff0: 6c65 2220 7265 7573 654c 6173 7456 616c  le" reuseLastVal
-00007000: 7565 3d22 3022 2f3e 0a20 2020 203c 6669  ue="0"/>.    <fi
-00007010: 656c 6420 6e61 6d65 3d22 6669 6422 2072  eld name="fid" r
-00007020: 6575 7365 4c61 7374 5661 6c75 653d 2230  euseLastValue="0
-00007030: 222f 3e0a 2020 2020 3c66 6965 6c64 206e  "/>.    <field n
-00007040: 616d 653d 226c 616e 655f 6f72 6965 6e74  ame="lane_orient
-00007050: 6174 696f 6e22 2072 6575 7365 4c61 7374  ation" reuseLast
-00007060: 5661 6c75 653d 2230 222f 3e0a 2020 2020  Value="0"/>.    
-00007070: 3c66 6965 6c64 206e 616d 653d 226c 616e  <field name="lan
-00007080: 655f 7769 6474 6822 2072 6575 7365 4c61  e_width" reuseLa
-00007090: 7374 5661 6c75 653d 2230 222f 3e0a 2020  stValue="0"/>.  
-000070a0: 2020 3c66 6965 6c64 206e 616d 653d 226f    <field name="o
-000070b0: 7269 656e 7461 7469 6f6e 2220 7265 7573  rientation" reus
-000070c0: 654c 6173 7456 616c 7565 3d22 3022 2f3e  eLastValue="0"/>
-000070d0: 0a20 2020 203c 6669 656c 6420 6e61 6d65  .    <field name
-000070e0: 3d22 6f72 6965 6e74 6174 696f 6e5f 636f  ="orientation_co
-000070f0: 6e66 6964 656e 6365 2220 7265 7573 654c  nfidence" reuseL
-00007100: 6173 7456 616c 7565 3d22 3022 2f3e 0a20  astValue="0"/>. 
-00007110: 2020 203c 6669 656c 6420 6e61 6d65 3d22     <field name="
-00007120: 6f73 6d5f 6964 2220 7265 7573 654c 6173  osm_id" reuseLas
-00007130: 7456 616c 7565 3d22 3022 2f3e 0a20 2020  tValue="0"/>.   
-00007140: 203c 6669 656c 6420 6e61 6d65 3d22 7479   <field name="ty
-00007150: 7065 2220 7265 7573 654c 6173 7456 616c  pe" reuseLastVal
-00007160: 7565 3d22 3022 2f3e 0a20 203c 2f72 6575  ue="0"/>.  </reu
-00007170: 7365 4c61 7374 5661 6c75 653e 0a20 203c  seLastValue>.  <
-00007180: 6461 7461 4465 6669 6e65 6446 6965 6c64  dataDefinedField
-00007190: 5072 6f70 6572 7469 6573 2f3e 0a20 203c  Properties/>.  <
-000071a0: 7769 6467 6574 732f 3e0a 2020 3c70 7265  widgets/>.  <pre
-000071b0: 7669 6577 4578 7072 6573 7369 6f6e 3e22  viewExpression>"
-000071c0: 7479 7065 223c 2f70 7265 7669 6577 4578  type"</previewEx
-000071d0: 7072 6573 7369 6f6e 3e0a 2020 3c6d 6170  pression>.  <map
-000071e0: 5469 703e 3c2f 6d61 7054 6970 3e0a 2020  Tip></mapTip>.  
-000071f0: 3c6c 6179 6572 4765 6f6d 6574 7279 5479  <layerGeometryTy
-00007200: 7065 3e30 3c2f 6c61 7965 7247 656f 6d65  pe>0</layerGeome
-00007210: 7472 7954 7970 653e 0a3c 2f71 6769 733e  tryType>.</qgis>
-00007220: 0a                                       .
+000037f0: 3c4f 7074 696f 6e20 6e61 6d65 3d22 6578  <Option name="ex
+00003800: 7072 6573 7369 6f6e 2220 7661 6c75 653d  pression" value=
+00003810: 2226 7175 6f74 3b6c 616e 655f 7769 6474  "&quot;lane_widt
+00003820: 6826 7175 6f74 3b22 2074 7970 653d 2251  h&quot;" type="Q
+00003830: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+00003840: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00003850: 696f 6e20 6e61 6d65 3d22 7479 7065 2220  ion name="type" 
+00003860: 7661 6c75 653d 2233 2220 7479 7065 3d22  value="3" type="
+00003870: 696e 7422 2f3e 0a20 2020 2020 2020 2020  int"/>.         
+00003880: 2020 2020 2020 203c 2f4f 7074 696f 6e3e         </Option>
+00003890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000038a0: 203c 4f70 7469 6f6e 206e 616d 653d 2273   <Option name="s
+000038b0: 697a 6522 2074 7970 653d 224d 6170 223e  ize" type="Map">
+000038c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000038d0: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
+000038e0: 2261 6374 6976 6522 2076 616c 7565 3d22  "active" value="
+000038f0: 7472 7565 2220 7479 7065 3d22 626f 6f6c  true" type="bool
+00003900: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00003910: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
+00003920: 6d65 3d22 6578 7072 6573 7369 6f6e 2220  me="expression" 
+00003930: 7661 6c75 653d 2233 202d 2032 202a 2030  value="3 - 2 * 0
+00003940: 2e30 3031 202a 2040 6d61 705f 7363 616c  .001 * @map_scal
+00003950: 6522 2074 7970 653d 2251 5374 7269 6e67  e" type="QString
+00003960: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00003970: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
+00003980: 6d65 3d22 7479 7065 2220 7661 6c75 653d  me="type" value=
+00003990: 2233 2220 7479 7065 3d22 696e 7422 2f3e  "3" type="int"/>
+000039a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000039b0: 203c 2f4f 7074 696f 6e3e 0a20 2020 2020   </Option>.     
+000039c0: 2020 2020 2020 2020 203c 2f4f 7074 696f           </Optio
+000039d0: 6e3e 0a20 2020 2020 2020 2020 2020 2020  n>.             
+000039e0: 203c 4f70 7469 6f6e 206e 616d 653d 2274   <Option name="t
+000039f0: 7970 6522 2076 616c 7565 3d22 636f 6c6c  ype" value="coll
+00003a00: 6563 7469 6f6e 2220 7479 7065 3d22 5153  ection" type="QS
+00003a10: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+00003a20: 2020 2020 203c 2f4f 7074 696f 6e3e 0a20       </Option>. 
+00003a30: 2020 2020 2020 2020 203c 2f64 6174 615f           </data_
+00003a40: 6465 6669 6e65 645f 7072 6f70 6572 7469  defined_properti
+00003a50: 6573 3e0a 2020 2020 2020 2020 3c2f 6c61  es>.        </la
+00003a60: 7965 723e 0a20 2020 2020 203c 2f73 796d  yer>.      </sym
+00003a70: 626f 6c3e 0a20 2020 2020 203c 7379 6d62  bol>.      <symb
+00003a80: 6f6c 206e 616d 653d 2232 2220 666f 7263  ol name="2" forc
+00003a90: 655f 7268 723d 2230 2220 6672 616d 655f  e_rhr="0" frame_
+00003aa0: 7261 7465 3d22 3130 2220 616c 7068 613d  rate="10" alpha=
+00003ab0: 2231 2220 636c 6970 5f74 6f5f 6578 7465  "1" clip_to_exte
+00003ac0: 6e74 3d22 3122 2069 735f 616e 696d 6174  nt="1" is_animat
+00003ad0: 6564 3d22 3022 2074 7970 653d 226d 6172  ed="0" type="mar
+00003ae0: 6b65 7222 3e0a 2020 2020 2020 2020 3c64  ker">.        <d
+00003af0: 6174 615f 6465 6669 6e65 645f 7072 6f70  ata_defined_prop
+00003b00: 6572 7469 6573 3e0a 2020 2020 2020 2020  erties>.        
+00003b10: 2020 3c4f 7074 696f 6e20 7479 7065 3d22    <Option type="
+00003b20: 4d61 7022 3e0a 2020 2020 2020 2020 2020  Map">.          
+00003b30: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
+00003b40: 6e61 6d65 2220 7661 6c75 653d 2222 2074  name" value="" t
+00003b50: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
+00003b60: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00003b70: 696f 6e20 6e61 6d65 3d22 7072 6f70 6572  ion name="proper
+00003b80: 7469 6573 222f 3e0a 2020 2020 2020 2020  ties"/>.        
+00003b90: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
+00003ba0: 3d22 7479 7065 2220 7661 6c75 653d 2263  ="type" value="c
+00003bb0: 6f6c 6c65 6374 696f 6e22 2074 7970 653d  ollection" type=
+00003bc0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00003bd0: 2020 2020 2020 3c2f 4f70 7469 6f6e 3e0a        </Option>.
+00003be0: 2020 2020 2020 2020 3c2f 6461 7461 5f64          </data_d
+00003bf0: 6566 696e 6564 5f70 726f 7065 7274 6965  efined_propertie
+00003c00: 733e 0a20 2020 2020 2020 203c 6c61 7965  s>.        <laye
+00003c10: 7220 7061 7373 3d22 3022 206c 6f63 6b65  r pass="0" locke
+00003c20: 643d 2230 2220 656e 6162 6c65 643d 2231  d="0" enabled="1
+00003c30: 2220 636c 6173 733d 2253 696d 706c 654d  " class="SimpleM
+00003c40: 6172 6b65 7222 3e0a 2020 2020 2020 2020  arker">.        
+00003c50: 2020 3c4f 7074 696f 6e20 7479 7065 3d22    <Option type="
+00003c60: 4d61 7022 3e0a 2020 2020 2020 2020 2020  Map">.          
+00003c70: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
+00003c80: 616e 676c 6522 2076 616c 7565 3d22 3022  angle" value="0"
+00003c90: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+00003ca0: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
+00003cb0: 7074 696f 6e20 6e61 6d65 3d22 6361 705f  ption name="cap_
+00003cc0: 7374 796c 6522 2076 616c 7565 3d22 666c  style" value="fl
+00003cd0: 6174 2220 7479 7065 3d22 5153 7472 696e  at" type="QStrin
+00003ce0: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00003cf0: 203c 4f70 7469 6f6e 206e 616d 653d 2263   <Option name="c
+00003d00: 6f6c 6f72 2220 7661 6c75 653d 2232 3332  olor" value="232
+00003d10: 2c38 352c 302c 3235 3522 2074 7970 653d  ,85,0,255" type=
+00003d20: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00003d30: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00003d40: 6e61 6d65 3d22 686f 7269 7a6f 6e74 616c  name="horizontal
+00003d50: 5f61 6e63 686f 725f 706f 696e 7422 2076  _anchor_point" v
+00003d60: 616c 7565 3d22 3122 2074 7970 653d 2251  alue="1" type="Q
+00003d70: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+00003d80: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
+00003d90: 6d65 3d22 6a6f 696e 7374 796c 6522 2076  me="joinstyle" v
+00003da0: 616c 7565 3d22 6265 7665 6c22 2074 7970  alue="bevel" typ
+00003db0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00003dc0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00003dd0: 6e20 6e61 6d65 3d22 6e61 6d65 2220 7661  n name="name" va
+00003de0: 6c75 653d 226c 696e 6522 2074 7970 653d  lue="line" type=
+00003df0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00003e00: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00003e10: 6e61 6d65 3d22 6f66 6673 6574 2220 7661  name="offset" va
+00003e20: 6c75 653d 2230 2c30 2220 7479 7065 3d22  lue="0,0" type="
+00003e30: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+00003e40: 2020 2020 2020 203c 4f70 7469 6f6e 206e         <Option n
+00003e50: 616d 653d 226f 6666 7365 745f 6d61 705f  ame="offset_map_
+00003e60: 756e 6974 5f73 6361 6c65 2220 7661 6c75  unit_scale" valu
+00003e70: 653d 2233 783a 302c 302c 302c 302c 302c  e="3x:0,0,0,0,0,
+00003e80: 3022 2074 7970 653d 2251 5374 7269 6e67  0" type="QString
+00003e90: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00003ea0: 3c4f 7074 696f 6e20 6e61 6d65 3d22 6f66  <Option name="of
+00003eb0: 6673 6574 5f75 6e69 7422 2076 616c 7565  fset_unit" value
+00003ec0: 3d22 4d4d 2220 7479 7065 3d22 5153 7472  ="MM" type="QStr
+00003ed0: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+00003ee0: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
+00003ef0: 226f 7574 6c69 6e65 5f63 6f6c 6f72 2220  "outline_color" 
+00003f00: 7661 6c75 653d 2232 3535 2c32 3535 2c32  value="255,255,2
+00003f10: 3535 2c32 3535 2220 7479 7065 3d22 5153  55,255" type="QS
+00003f20: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+00003f30: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
+00003f40: 653d 226f 7574 6c69 6e65 5f73 7479 6c65  e="outline_style
+00003f50: 2220 7661 6c75 653d 2273 6f6c 6964 2220  " value="solid" 
+00003f60: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00003f70: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
+00003f80: 7469 6f6e 206e 616d 653d 226f 7574 6c69  tion name="outli
+00003f90: 6e65 5f77 6964 7468 2220 7661 6c75 653d  ne_width" value=
+00003fa0: 2232 2220 7479 7065 3d22 5153 7472 696e  "2" type="QStrin
+00003fb0: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00003fc0: 203c 4f70 7469 6f6e 206e 616d 653d 226f   <Option name="o
+00003fd0: 7574 6c69 6e65 5f77 6964 7468 5f6d 6170  utline_width_map
+00003fe0: 5f75 6e69 745f 7363 616c 6522 2076 616c  _unit_scale" val
+00003ff0: 7565 3d22 3378 3a30 2c30 2c30 2c30 2c30  ue="3x:0,0,0,0,0
+00004000: 2c30 2220 7479 7065 3d22 5153 7472 696e  ,0" type="QStrin
+00004010: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00004020: 203c 4f70 7469 6f6e 206e 616d 653d 226f   <Option name="o
+00004030: 7574 6c69 6e65 5f77 6964 7468 5f75 6e69  utline_width_uni
+00004040: 7422 2076 616c 7565 3d22 5265 6e64 6572  t" value="Render
+00004050: 4d65 7465 7273 496e 4d61 7055 6e69 7473  MetersInMapUnits
+00004060: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00004070: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
+00004080: 4f70 7469 6f6e 206e 616d 653d 2273 6361  Option name="sca
+00004090: 6c65 5f6d 6574 686f 6422 2076 616c 7565  le_method" value
+000040a0: 3d22 6469 616d 6574 6572 2220 7479 7065  ="diameter" type
+000040b0: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+000040c0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+000040d0: 206e 616d 653d 2273 697a 6522 2076 616c   name="size" val
+000040e0: 7565 3d22 3322 2074 7970 653d 2251 5374  ue="3" type="QSt
+000040f0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+00004100: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
+00004110: 3d22 7369 7a65 5f6d 6170 5f75 6e69 745f  ="size_map_unit_
+00004120: 7363 616c 6522 2076 616c 7565 3d22 3378  scale" value="3x
+00004130: 3a30 2c30 2c30 2c30 2c30 2c30 2220 7479  :0,0,0,0,0,0" ty
+00004140: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+00004150: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00004160: 6f6e 206e 616d 653d 2273 697a 655f 756e  on name="size_un
+00004170: 6974 2220 7661 6c75 653d 2252 656e 6465  it" value="Rende
+00004180: 724d 6574 6572 7349 6e4d 6170 556e 6974  rMetersInMapUnit
+00004190: 7322 2074 7970 653d 2251 5374 7269 6e67  s" type="QString
+000041a0: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+000041b0: 3c4f 7074 696f 6e20 6e61 6d65 3d22 7665  <Option name="ve
+000041c0: 7274 6963 616c 5f61 6e63 686f 725f 706f  rtical_anchor_po
+000041d0: 696e 7422 2076 616c 7565 3d22 3122 2074  int" value="1" t
+000041e0: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
+000041f0: 2020 2020 2020 2020 2020 3c2f 4f70 7469            </Opti
+00004200: 6f6e 3e0a 2020 2020 2020 2020 2020 3c64  on>.          <d
+00004210: 6174 615f 6465 6669 6e65 645f 7072 6f70  ata_defined_prop
+00004220: 6572 7469 6573 3e0a 2020 2020 2020 2020  erties>.        
+00004230: 2020 2020 3c4f 7074 696f 6e20 7479 7065      <Option type
+00004240: 3d22 4d61 7022 3e0a 2020 2020 2020 2020  ="Map">.        
+00004250: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
+00004260: 6d65 3d22 6e61 6d65 2220 7661 6c75 653d  me="name" value=
+00004270: 2222 2074 7970 653d 2251 5374 7269 6e67  "" type="QString
+00004280: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00004290: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
+000042a0: 7072 6f70 6572 7469 6573 2220 7479 7065  properties" type
+000042b0: 3d22 4d61 7022 3e0a 2020 2020 2020 2020  ="Map">.        
+000042c0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+000042d0: 6e61 6d65 3d22 616e 676c 6522 2074 7970  name="angle" typ
+000042e0: 653d 224d 6170 223e 0a20 2020 2020 2020  e="Map">.       
+000042f0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00004300: 6f6e 206e 616d 653d 2261 6374 6976 6522  on name="active"
+00004310: 2076 616c 7565 3d22 7472 7565 2220 7479   value="true" ty
+00004320: 7065 3d22 626f 6f6c 222f 3e0a 2020 2020  pe="bool"/>.    
+00004330: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
+00004340: 7074 696f 6e20 6e61 6d65 3d22 6578 7072  ption name="expr
+00004350: 6573 7369 6f6e 2220 7661 6c75 653d 2239  ession" value="9
+00004360: 3020 2b20 282d 2671 756f 743b 6f72 6965  0 + (-&quot;orie
+00004370: 6e74 6174 696f 6e26 7175 6f74 3b20 2f20  ntation&quot; / 
+00004380: 7069 2829 2920 2a20 3138 3022 2074 7970  pi()) * 180" typ
+00004390: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+000043a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000043b0: 3c4f 7074 696f 6e20 6e61 6d65 3d22 7479  <Option name="ty
+000043c0: 7065 2220 7661 6c75 653d 2233 2220 7479  pe" value="3" ty
+000043d0: 7065 3d22 696e 7422 2f3e 0a20 2020 2020  pe="int"/>.     
+000043e0: 2020 2020 2020 2020 2020 203c 2f4f 7074             </Opt
+000043f0: 696f 6e3e 0a20 2020 2020 2020 2020 2020  ion>.           
+00004400: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
+00004410: 653d 226f 7574 6c69 6e65 5769 6474 6822  e="outlineWidth"
+00004420: 2074 7970 653d 224d 6170 223e 0a20 2020   type="Map">.   
+00004430: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00004440: 4f70 7469 6f6e 206e 616d 653d 2261 6374  Option name="act
+00004450: 6976 6522 2076 616c 7565 3d22 7472 7565  ive" value="true
+00004460: 2220 7479 7065 3d22 626f 6f6c 222f 3e0a  " type="bool"/>.
+00004470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004480: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
+00004490: 6578 7072 6573 7369 6f6e 2220 7661 6c75  expression" valu
+000044a0: 653d 2226 7175 6f74 3b6c 616e 655f 7769  e="&quot;lane_wi
+000044b0: 6474 6826 7175 6f74 3b22 2074 7970 653d  dth&quot;" type=
+000044c0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+000044d0: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
+000044e0: 7074 696f 6e20 6e61 6d65 3d22 7479 7065  ption name="type
+000044f0: 2220 7661 6c75 653d 2233 2220 7479 7065  " value="3" type
+00004500: 3d22 696e 7422 2f3e 0a20 2020 2020 2020  ="int"/>.       
+00004510: 2020 2020 2020 2020 203c 2f4f 7074 696f           </Optio
+00004520: 6e3e 0a20 2020 2020 2020 2020 2020 2020  n>.             
+00004530: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
+00004540: 2273 697a 6522 2074 7970 653d 224d 6170  "size" type="Map
+00004550: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00004560: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
+00004570: 653d 2261 6374 6976 6522 2076 616c 7565  e="active" value
+00004580: 3d22 7472 7565 2220 7479 7065 3d22 626f  ="true" type="bo
+00004590: 6f6c 222f 3e0a 2020 2020 2020 2020 2020  ol"/>.          
+000045a0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+000045b0: 6e61 6d65 3d22 6578 7072 6573 7369 6f6e  name="expression
+000045c0: 2220 7661 6c75 653d 2233 202d 2032 202a  " value="3 - 2 *
+000045d0: 2030 2e30 3032 202a 2040 6d61 705f 7363   0.002 * @map_sc
+000045e0: 616c 6522 2074 7970 653d 2251 5374 7269  ale" type="QStri
+000045f0: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+00004600: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00004610: 6e61 6d65 3d22 7479 7065 2220 7661 6c75  name="type" valu
+00004620: 653d 2233 2220 7479 7065 3d22 696e 7422  e="3" type="int"
+00004630: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+00004640: 2020 203c 2f4f 7074 696f 6e3e 0a20 2020     </Option>.   
+00004650: 2020 2020 2020 2020 2020 203c 2f4f 7074             </Opt
+00004660: 696f 6e3e 0a20 2020 2020 2020 2020 2020  ion>.           
+00004670: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
+00004680: 2274 7970 6522 2076 616c 7565 3d22 636f  "type" value="co
+00004690: 6c6c 6563 7469 6f6e 2220 7479 7065 3d22  llection" type="
+000046a0: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+000046b0: 2020 2020 2020 203c 2f4f 7074 696f 6e3e         </Option>
+000046c0: 0a20 2020 2020 2020 2020 203c 2f64 6174  .          </dat
+000046d0: 615f 6465 6669 6e65 645f 7072 6f70 6572  a_defined_proper
+000046e0: 7469 6573 3e0a 2020 2020 2020 2020 3c2f  ties>.        </
+000046f0: 6c61 7965 723e 0a20 2020 2020 203c 2f73  layer>.      </s
+00004700: 796d 626f 6c3e 0a20 2020 203c 2f73 796d  ymbol>.    </sym
+00004710: 626f 6c73 3e0a 2020 3c2f 7265 6e64 6572  bols>.  </render
+00004720: 6572 2d76 323e 0a20 203c 6375 7374 6f6d  er-v2>.  <custom
+00004730: 7072 6f70 6572 7469 6573 3e0a 2020 2020  properties>.    
+00004740: 3c4f 7074 696f 6e20 7479 7065 3d22 4d61  <Option type="Ma
+00004750: 7022 3e0a 2020 2020 2020 3c4f 7074 696f  p">.      <Optio
+00004760: 6e20 6e61 6d65 3d22 6475 616c 7669 6577  n name="dualview
+00004770: 2f70 7265 7669 6577 4578 7072 6573 7369  /previewExpressi
+00004780: 6f6e 7322 2074 7970 653d 224c 6973 7422  ons" type="List"
+00004790: 3e0a 2020 2020 2020 2020 3c4f 7074 696f  >.        <Optio
+000047a0: 6e20 7661 6c75 653d 2226 7175 6f74 3b74  n value="&quot;t
+000047b0: 7970 6526 7175 6f74 3b22 2074 7970 653d  ype&quot;" type=
+000047c0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+000047d0: 2020 3c2f 4f70 7469 6f6e 3e0a 2020 2020    </Option>.    
+000047e0: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
+000047f0: 656d 6265 6464 6564 5769 6467 6574 732f  embeddedWidgets/
+00004800: 636f 756e 7422 2076 616c 7565 3d22 3022  count" value="0"
+00004810: 2074 7970 653d 2269 6e74 222f 3e0a 2020   type="int"/>.  
+00004820: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
+00004830: 3d22 7661 7269 6162 6c65 4e61 6d65 7322  ="variableNames"
+00004840: 2f3e 0a20 2020 2020 203c 4f70 7469 6f6e  />.      <Option
+00004850: 206e 616d 653d 2276 6172 6961 626c 6556   name="variableV
+00004860: 616c 7565 7322 2f3e 0a20 2020 203c 2f4f  alues"/>.    </O
+00004870: 7074 696f 6e3e 0a20 203c 2f63 7573 746f  ption>.  </custo
+00004880: 6d70 726f 7065 7274 6965 733e 0a20 203c  mproperties>.  <
+00004890: 626c 656e 644d 6f64 653e 303c 2f62 6c65  blendMode>0</ble
+000048a0: 6e64 4d6f 6465 3e0a 2020 3c66 6561 7475  ndMode>.  <featu
+000048b0: 7265 426c 656e 644d 6f64 653e 303c 2f66  reBlendMode>0</f
+000048c0: 6561 7475 7265 426c 656e 644d 6f64 653e  eatureBlendMode>
+000048d0: 0a20 203c 6c61 7965 724f 7061 6369 7479  .  <layerOpacity
+000048e0: 3e31 3c2f 6c61 7965 724f 7061 6369 7479  >1</layerOpacity
+000048f0: 3e0a 2020 3c53 696e 676c 6543 6174 6567  >.  <SingleCateg
+00004900: 6f72 7944 6961 6772 616d 5265 6e64 6572  oryDiagramRender
+00004910: 6572 2061 7474 7269 6275 7465 4c65 6765  er attributeLege
+00004920: 6e64 3d22 3122 2064 6961 6772 616d 5479  nd="1" diagramTy
+00004930: 7065 3d22 4869 7374 6f67 7261 6d22 3e0a  pe="Histogram">.
+00004940: 2020 2020 3c44 6961 6772 616d 4361 7465      <DiagramCate
+00004950: 676f 7279 2070 656e 416c 7068 613d 2232  gory penAlpha="2
+00004960: 3535 2220 6865 6967 6874 3d22 3135 2220  55" height="15" 
+00004970: 7370 6163 696e 6755 6e69 7453 6361 6c65  spacingUnitScale
+00004980: 3d22 3378 3a30 2c30 2c30 2c30 2c30 2c30  ="3x:0,0,0,0,0,0
+00004990: 2220 6f70 6163 6974 793d 2231 2220 6d61  " opacity="1" ma
+000049a0: 7853 6361 6c65 4465 6e6f 6d69 6e61 746f  xScaleDenominato
+000049b0: 723d 2231 652b 3038 2220 6c61 6265 6c50  r="1e+08" labelP
+000049c0: 6c61 6365 6d65 6e74 4d65 7468 6f64 3d22  lacementMethod="
+000049d0: 5848 6569 6768 7422 2064 6972 6563 7469  XHeight" directi
+000049e0: 6f6e 3d22 3022 206c 696e 6553 697a 6553  on="0" lineSizeS
+000049f0: 6361 6c65 3d22 3378 3a30 2c30 2c30 2c30  cale="3x:0,0,0,0
+00004a00: 2c30 2c30 2220 6469 6167 7261 6d4f 7269  ,0,0" diagramOri
+00004a10: 656e 7461 7469 6f6e 3d22 5570 2220 7370  entation="Up" sp
+00004a20: 6163 696e 6755 6e69 743d 224d 4d22 2073  acingUnit="MM" s
+00004a30: 697a 6553 6361 6c65 3d22 3378 3a30 2c30  izeScale="3x:0,0
+00004a40: 2c30 2c30 2c30 2c30 2220 7363 616c 6544  ,0,0,0,0" scaleD
+00004a50: 6570 656e 6465 6e63 793d 2241 7265 6122  ependency="Area"
+00004a60: 206d 696e 696d 756d 5369 7a65 3d22 3022   minimumSize="0"
+00004a70: 2065 6e61 626c 6564 3d22 3022 2073 697a   enabled="0" siz
+00004a80: 6554 7970 653d 224d 4d22 206d 696e 5363  eType="MM" minSc
+00004a90: 616c 6544 656e 6f6d 696e 6174 6f72 3d22  aleDenominator="
+00004aa0: 3022 2072 6f74 6174 696f 6e4f 6666 7365  0" rotationOffse
+00004ab0: 743d 2232 3730 2220 7065 6e43 6f6c 6f72  t="270" penColor
+00004ac0: 3d22 2330 3030 3030 3022 2062 6163 6b67  ="#000000" backg
+00004ad0: 726f 756e 6441 6c70 6861 3d22 3235 3522  roundAlpha="255"
+00004ae0: 2062 6172 5769 6474 683d 2235 2220 6261   barWidth="5" ba
+00004af0: 636b 6772 6f75 6e64 436f 6c6f 723d 2223  ckgroundColor="#
+00004b00: 6666 6666 6666 2220 6c69 6e65 5369 7a65  ffffff" lineSize
+00004b10: 5479 7065 3d22 4d4d 2220 7363 616c 6542  Type="MM" scaleB
+00004b20: 6173 6564 5669 7369 6269 6c69 7479 3d22  asedVisibility="
+00004b30: 3022 2073 686f 7741 7869 733d 2231 2220  0" showAxis="1" 
+00004b40: 7370 6163 696e 673d 2235 2220 7065 6e57  spacing="5" penW
+00004b50: 6964 7468 3d22 3022 2077 6964 7468 3d22  idth="0" width="
+00004b60: 3135 223e 0a20 2020 2020 203c 666f 6e74  15">.      <font
+00004b70: 5072 6f70 6572 7469 6573 2073 7472 696b  Properties strik
+00004b80: 6574 6872 6f75 6768 3d22 3022 2064 6573  ethrough="0" des
+00004b90: 6372 6970 7469 6f6e 3d22 4e6f 746f 2053  cription="Noto S
+00004ba0: 616e 732c 3130 2c2d 312c 302c 3530 2c30  ans,10,-1,0,50,0
+00004bb0: 2c30 2c30 2c30 2c30 2220 6974 616c 6963  ,0,0,0,0" italic
+00004bc0: 3d22 3022 2075 6e64 6572 6c69 6e65 3d22  ="0" underline="
+00004bd0: 3022 2073 7479 6c65 3d22 2220 626f 6c64  0" style="" bold
+00004be0: 3d22 3022 2f3e 0a20 2020 2020 203c 6174  ="0"/>.      <at
+00004bf0: 7472 6962 7574 6520 636f 6c6f 723d 2223  tribute color="#
+00004c00: 3030 3030 3030 2220 6669 656c 643d 2222  000000" field=""
+00004c10: 2063 6f6c 6f72 4f70 6163 6974 793d 2231   colorOpacity="1
+00004c20: 2220 6c61 6265 6c3d 2222 2f3e 0a20 2020  " label=""/>.   
+00004c30: 2020 203c 6178 6973 5379 6d62 6f6c 3e0a     <axisSymbol>.
+00004c40: 2020 2020 2020 2020 3c73 796d 626f 6c20          <symbol 
+00004c50: 6e61 6d65 3d22 2220 666f 7263 655f 7268  name="" force_rh
+00004c60: 723d 2230 2220 6672 616d 655f 7261 7465  r="0" frame_rate
+00004c70: 3d22 3130 2220 616c 7068 613d 2231 2220  ="10" alpha="1" 
+00004c80: 636c 6970 5f74 6f5f 6578 7465 6e74 3d22  clip_to_extent="
+00004c90: 3122 2069 735f 616e 696d 6174 6564 3d22  1" is_animated="
+00004ca0: 3022 2074 7970 653d 226c 696e 6522 3e0a  0" type="line">.
+00004cb0: 2020 2020 2020 2020 2020 3c64 6174 615f            <data_
+00004cc0: 6465 6669 6e65 645f 7072 6f70 6572 7469  defined_properti
+00004cd0: 6573 3e0a 2020 2020 2020 2020 2020 2020  es>.            
+00004ce0: 3c4f 7074 696f 6e20 7479 7065 3d22 4d61  <Option type="Ma
+00004cf0: 7022 3e0a 2020 2020 2020 2020 2020 2020  p">.            
+00004d00: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
+00004d10: 6e61 6d65 2220 7661 6c75 653d 2222 2074  name" value="" t
+00004d20: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
+00004d30: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
+00004d40: 7074 696f 6e20 6e61 6d65 3d22 7072 6f70  ption name="prop
+00004d50: 6572 7469 6573 222f 3e0a 2020 2020 2020  erties"/>.      
+00004d60: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00004d70: 6e61 6d65 3d22 7479 7065 2220 7661 6c75  name="type" valu
+00004d80: 653d 2263 6f6c 6c65 6374 696f 6e22 2074  e="collection" t
+00004d90: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
+00004da0: 2020 2020 2020 2020 2020 2020 3c2f 4f70              </Op
+00004db0: 7469 6f6e 3e0a 2020 2020 2020 2020 2020  tion>.          
+00004dc0: 3c2f 6461 7461 5f64 6566 696e 6564 5f70  </data_defined_p
+00004dd0: 726f 7065 7274 6965 733e 0a20 2020 2020  roperties>.     
+00004de0: 2020 2020 203c 6c61 7965 7220 7061 7373       <layer pass
+00004df0: 3d22 3022 206c 6f63 6b65 643d 2230 2220  ="0" locked="0" 
+00004e00: 656e 6162 6c65 643d 2231 2220 636c 6173  enabled="1" clas
+00004e10: 733d 2253 696d 706c 654c 696e 6522 3e0a  s="SimpleLine">.
+00004e20: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00004e30: 696f 6e20 7479 7065 3d22 4d61 7022 3e0a  ion type="Map">.
+00004e40: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
+00004e50: 7074 696f 6e20 6e61 6d65 3d22 616c 6967  ption name="alig
+00004e60: 6e5f 6461 7368 5f70 6174 7465 726e 2220  n_dash_pattern" 
+00004e70: 7661 6c75 653d 2230 2220 7479 7065 3d22  value="0" type="
+00004e80: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+00004e90: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00004ea0: 206e 616d 653d 2263 6170 7374 796c 6522   name="capstyle"
+00004eb0: 2076 616c 7565 3d22 7371 7561 7265 2220   value="square" 
+00004ec0: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00004ed0: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+00004ee0: 4f70 7469 6f6e 206e 616d 653d 2263 7573  Option name="cus
+00004ef0: 746f 6d64 6173 6822 2076 616c 7565 3d22  tomdash" value="
+00004f00: 353b 3222 2074 7970 653d 2251 5374 7269  5;2" type="QStri
+00004f10: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+00004f20: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
+00004f30: 3d22 6375 7374 6f6d 6461 7368 5f6d 6170  ="customdash_map
+00004f40: 5f75 6e69 745f 7363 616c 6522 2076 616c  _unit_scale" val
+00004f50: 7565 3d22 3378 3a30 2c30 2c30 2c30 2c30  ue="3x:0,0,0,0,0
+00004f60: 2c30 2220 7479 7065 3d22 5153 7472 696e  ,0" type="QStrin
+00004f70: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00004f80: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
+00004f90: 2263 7573 746f 6d64 6173 685f 756e 6974  "customdash_unit
+00004fa0: 2220 7661 6c75 653d 224d 4d22 2074 7970  " value="MM" typ
+00004fb0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00004fc0: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00004fd0: 696f 6e20 6e61 6d65 3d22 6461 7368 5f70  ion name="dash_p
+00004fe0: 6174 7465 726e 5f6f 6666 7365 7422 2076  attern_offset" v
+00004ff0: 616c 7565 3d22 3022 2074 7970 653d 2251  alue="0" type="Q
+00005000: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+00005010: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00005020: 6e61 6d65 3d22 6461 7368 5f70 6174 7465  name="dash_patte
+00005030: 726e 5f6f 6666 7365 745f 6d61 705f 756e  rn_offset_map_un
+00005040: 6974 5f73 6361 6c65 2220 7661 6c75 653d  it_scale" value=
+00005050: 2233 783a 302c 302c 302c 302c 302c 3022  "3x:0,0,0,0,0,0"
+00005060: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+00005070: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00005080: 3c4f 7074 696f 6e20 6e61 6d65 3d22 6461  <Option name="da
+00005090: 7368 5f70 6174 7465 726e 5f6f 6666 7365  sh_pattern_offse
+000050a0: 745f 756e 6974 2220 7661 6c75 653d 224d  t_unit" value="M
+000050b0: 4d22 2074 7970 653d 2251 5374 7269 6e67  M" type="QString
+000050c0: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+000050d0: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
+000050e0: 6472 6177 5f69 6e73 6964 655f 706f 6c79  draw_inside_poly
+000050f0: 676f 6e22 2076 616c 7565 3d22 3022 2074  gon" value="0" t
+00005100: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
+00005110: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
+00005120: 7074 696f 6e20 6e61 6d65 3d22 6a6f 696e  ption name="join
+00005130: 7374 796c 6522 2076 616c 7565 3d22 6265  style" value="be
+00005140: 7665 6c22 2074 7970 653d 2251 5374 7269  vel" type="QStri
+00005150: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+00005160: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
+00005170: 3d22 6c69 6e65 5f63 6f6c 6f72 2220 7661  ="line_color" va
+00005180: 6c75 653d 2233 352c 3335 2c33 352c 3235  lue="35,35,35,25
+00005190: 3522 2074 7970 653d 2251 5374 7269 6e67  5" type="QString
+000051a0: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+000051b0: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
+000051c0: 6c69 6e65 5f73 7479 6c65 2220 7661 6c75  line_style" valu
+000051d0: 653d 2273 6f6c 6964 2220 7479 7065 3d22  e="solid" type="
+000051e0: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+000051f0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00005200: 206e 616d 653d 226c 696e 655f 7769 6474   name="line_widt
+00005210: 6822 2076 616c 7565 3d22 302e 3236 2220  h" value="0.26" 
+00005220: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00005230: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+00005240: 4f70 7469 6f6e 206e 616d 653d 226c 696e  Option name="lin
+00005250: 655f 7769 6474 685f 756e 6974 2220 7661  e_width_unit" va
+00005260: 6c75 653d 224d 4d22 2074 7970 653d 2251  lue="MM" type="Q
+00005270: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+00005280: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00005290: 6e61 6d65 3d22 6f66 6673 6574 2220 7661  name="offset" va
+000052a0: 6c75 653d 2230 2220 7479 7065 3d22 5153  lue="0" type="QS
+000052b0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+000052c0: 2020 2020 2020 203c 4f70 7469 6f6e 206e         <Option n
+000052d0: 616d 653d 226f 6666 7365 745f 6d61 705f  ame="offset_map_
+000052e0: 756e 6974 5f73 6361 6c65 2220 7661 6c75  unit_scale" valu
+000052f0: 653d 2233 783a 302c 302c 302c 302c 302c  e="3x:0,0,0,0,0,
+00005300: 3022 2074 7970 653d 2251 5374 7269 6e67  0" type="QString
+00005310: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00005320: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
+00005330: 6f66 6673 6574 5f75 6e69 7422 2076 616c  offset_unit" val
+00005340: 7565 3d22 4d4d 2220 7479 7065 3d22 5153  ue="MM" type="QS
+00005350: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+00005360: 2020 2020 2020 203c 4f70 7469 6f6e 206e         <Option n
+00005370: 616d 653d 2272 696e 675f 6669 6c74 6572  ame="ring_filter
+00005380: 2220 7661 6c75 653d 2230 2220 7479 7065  " value="0" type
+00005390: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+000053a0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+000053b0: 6f6e 206e 616d 653d 2274 7269 6d5f 6469  on name="trim_di
+000053c0: 7374 616e 6365 5f65 6e64 2220 7661 6c75  stance_end" valu
+000053d0: 653d 2230 2220 7479 7065 3d22 5153 7472  e="0" type="QStr
+000053e0: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+000053f0: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
+00005400: 653d 2274 7269 6d5f 6469 7374 616e 6365  e="trim_distance
+00005410: 5f65 6e64 5f6d 6170 5f75 6e69 745f 7363  _end_map_unit_sc
+00005420: 616c 6522 2076 616c 7565 3d22 3378 3a30  ale" value="3x:0
+00005430: 2c30 2c30 2c30 2c30 2c30 2220 7479 7065  ,0,0,0,0,0" type
+00005440: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+00005450: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00005460: 6f6e 206e 616d 653d 2274 7269 6d5f 6469  on name="trim_di
+00005470: 7374 616e 6365 5f65 6e64 5f75 6e69 7422  stance_end_unit"
+00005480: 2076 616c 7565 3d22 4d4d 2220 7479 7065   value="MM" type
+00005490: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+000054a0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+000054b0: 6f6e 206e 616d 653d 2274 7269 6d5f 6469  on name="trim_di
+000054c0: 7374 616e 6365 5f73 7461 7274 2220 7661  stance_start" va
+000054d0: 6c75 653d 2230 2220 7479 7065 3d22 5153  lue="0" type="QS
+000054e0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+000054f0: 2020 2020 2020 203c 4f70 7469 6f6e 206e         <Option n
+00005500: 616d 653d 2274 7269 6d5f 6469 7374 616e  ame="trim_distan
+00005510: 6365 5f73 7461 7274 5f6d 6170 5f75 6e69  ce_start_map_uni
+00005520: 745f 7363 616c 6522 2076 616c 7565 3d22  t_scale" value="
+00005530: 3378 3a30 2c30 2c30 2c30 2c30 2c30 2220  3x:0,0,0,0,0,0" 
+00005540: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00005550: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+00005560: 4f70 7469 6f6e 206e 616d 653d 2274 7269  Option name="tri
+00005570: 6d5f 6469 7374 616e 6365 5f73 7461 7274  m_distance_start
+00005580: 5f75 6e69 7422 2076 616c 7565 3d22 4d4d  _unit" value="MM
+00005590: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+000055a0: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+000055b0: 203c 4f70 7469 6f6e 206e 616d 653d 2274   <Option name="t
+000055c0: 7765 616b 5f64 6173 685f 7061 7474 6572  weak_dash_patter
+000055d0: 6e5f 6f6e 5f63 6f72 6e65 7273 2220 7661  n_on_corners" va
+000055e0: 6c75 653d 2230 2220 7479 7065 3d22 5153  lue="0" type="QS
+000055f0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+00005600: 2020 2020 2020 203c 4f70 7469 6f6e 206e         <Option n
+00005610: 616d 653d 2275 7365 5f63 7573 746f 6d5f  ame="use_custom_
+00005620: 6461 7368 2220 7661 6c75 653d 2230 2220  dash" value="0" 
+00005630: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00005640: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+00005650: 4f70 7469 6f6e 206e 616d 653d 2277 6964  Option name="wid
+00005660: 7468 5f6d 6170 5f75 6e69 745f 7363 616c  th_map_unit_scal
+00005670: 6522 2076 616c 7565 3d22 3378 3a30 2c30  e" value="3x:0,0
+00005680: 2c30 2c30 2c30 2c30 2220 7479 7065 3d22  ,0,0,0,0" type="
+00005690: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+000056a0: 2020 2020 2020 203c 2f4f 7074 696f 6e3e         </Option>
+000056b0: 0a20 2020 2020 2020 2020 2020 203c 6461  .            <da
+000056c0: 7461 5f64 6566 696e 6564 5f70 726f 7065  ta_defined_prope
+000056d0: 7274 6965 733e 0a20 2020 2020 2020 2020  rties>.         
+000056e0: 2020 2020 203c 4f70 7469 6f6e 2074 7970       <Option typ
+000056f0: 653d 224d 6170 223e 0a20 2020 2020 2020  e="Map">.       
+00005700: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00005710: 206e 616d 653d 226e 616d 6522 2076 616c   name="name" val
+00005720: 7565 3d22 2220 7479 7065 3d22 5153 7472  ue="" type="QStr
+00005730: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+00005740: 2020 2020 2020 203c 4f70 7469 6f6e 206e         <Option n
+00005750: 616d 653d 2270 726f 7065 7274 6965 7322  ame="properties"
+00005760: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+00005770: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
+00005780: 2274 7970 6522 2076 616c 7565 3d22 636f  "type" value="co
+00005790: 6c6c 6563 7469 6f6e 2220 7479 7065 3d22  llection" type="
+000057a0: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+000057b0: 2020 2020 2020 2020 203c 2f4f 7074 696f           </Optio
+000057c0: 6e3e 0a20 2020 2020 2020 2020 2020 203c  n>.            <
+000057d0: 2f64 6174 615f 6465 6669 6e65 645f 7072  /data_defined_pr
+000057e0: 6f70 6572 7469 6573 3e0a 2020 2020 2020  operties>.      
+000057f0: 2020 2020 3c2f 6c61 7965 723e 0a20 2020      </layer>.   
+00005800: 2020 2020 203c 2f73 796d 626f 6c3e 0a20       </symbol>. 
+00005810: 2020 2020 203c 2f61 7869 7353 796d 626f       </axisSymbo
+00005820: 6c3e 0a20 2020 203c 2f44 6961 6772 616d  l>.    </Diagram
+00005830: 4361 7465 676f 7279 3e0a 2020 3c2f 5369  Category>.  </Si
+00005840: 6e67 6c65 4361 7465 676f 7279 4469 6167  ngleCategoryDiag
+00005850: 7261 6d52 656e 6465 7265 723e 0a20 203c  ramRenderer>.  <
+00005860: 4469 6167 7261 6d4c 6179 6572 5365 7474  DiagramLayerSett
+00005870: 696e 6773 2064 6973 743d 2230 2220 7368  ings dist="0" sh
+00005880: 6f77 416c 6c3d 2231 2220 6f62 7374 6163  owAll="1" obstac
+00005890: 6c65 3d22 3022 2070 6c61 6365 6d65 6e74  le="0" placement
+000058a0: 3d22 3022 207a 496e 6465 783d 2230 2220  ="0" zIndex="0" 
+000058b0: 7072 696f 7269 7479 3d22 3022 206c 696e  priority="0" lin
+000058c0: 6550 6c61 6365 6d65 6e74 466c 6167 733d  ePlacementFlags=
+000058d0: 2231 3822 3e0a 2020 2020 3c70 726f 7065  "18">.    <prope
+000058e0: 7274 6965 733e 0a20 2020 2020 203c 4f70  rties>.      <Op
+000058f0: 7469 6f6e 2074 7970 653d 224d 6170 223e  tion type="Map">
+00005900: 0a20 2020 2020 2020 203c 4f70 7469 6f6e  .        <Option
+00005910: 206e 616d 653d 226e 616d 6522 2076 616c   name="name" val
+00005920: 7565 3d22 2220 7479 7065 3d22 5153 7472  ue="" type="QStr
+00005930: 696e 6722 2f3e 0a20 2020 2020 2020 203c  ing"/>.        <
+00005940: 4f70 7469 6f6e 206e 616d 653d 2270 726f  Option name="pro
+00005950: 7065 7274 6965 7322 2f3e 0a20 2020 2020  perties"/>.     
+00005960: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
+00005970: 2274 7970 6522 2076 616c 7565 3d22 636f  "type" value="co
+00005980: 6c6c 6563 7469 6f6e 2220 7479 7065 3d22  llection" type="
+00005990: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+000059a0: 203c 2f4f 7074 696f 6e3e 0a20 2020 203c   </Option>.    <
+000059b0: 2f70 726f 7065 7274 6965 733e 0a20 203c  /properties>.  <
+000059c0: 2f44 6961 6772 616d 4c61 7965 7253 6574  /DiagramLayerSet
+000059d0: 7469 6e67 733e 0a20 203c 6765 6f6d 6574  tings>.  <geomet
+000059e0: 7279 4f70 7469 6f6e 7320 7265 6d6f 7665  ryOptions remove
+000059f0: 4475 706c 6963 6174 654e 6f64 6573 3d22  DuplicateNodes="
+00005a00: 3022 2067 656f 6d65 7472 7950 7265 6369  0" geometryPreci
+00005a10: 7369 6f6e 3d22 3022 3e0a 2020 2020 3c61  sion="0">.    <a
+00005a20: 6374 6976 6543 6865 636b 732f 3e0a 2020  ctiveChecks/>.  
+00005a30: 2020 3c63 6865 636b 436f 6e66 6967 7572    <checkConfigur
+00005a40: 6174 696f 6e2f 3e0a 2020 3c2f 6765 6f6d  ation/>.  </geom
+00005a50: 6574 7279 4f70 7469 6f6e 733e 0a20 203c  etryOptions>.  <
+00005a60: 6c65 6765 6e64 2073 686f 774c 6162 656c  legend showLabel
+00005a70: 4c65 6765 6e64 3d22 3022 2074 7970 653d  Legend="0" type=
+00005a80: 2264 6566 6175 6c74 2d76 6563 746f 7222  "default-vector"
+00005a90: 2f3e 0a20 203c 7265 6665 7265 6e63 6564  />.  <referenced
+00005aa0: 4c61 7965 7273 2f3e 0a20 203c 6669 656c  Layers/>.  <fiel
+00005ab0: 6443 6f6e 6669 6775 7261 7469 6f6e 3e0a  dConfiguration>.
+00005ac0: 2020 2020 3c66 6965 6c64 206e 616d 653d      <field name=
+00005ad0: 2274 7970 6522 2063 6f6e 6669 6775 7261  "type" configura
+00005ae0: 7469 6f6e 466c 6167 733d 224e 6f6e 6522  tionFlags="None"
+00005af0: 3e0a 2020 2020 2020 3c65 6469 7457 6964  >.      <editWid
+00005b00: 6765 7420 7479 7065 3d22 5465 7874 4564  get type="TextEd
+00005b10: 6974 223e 0a20 2020 2020 2020 203c 636f  it">.        <co
+00005b20: 6e66 6967 3e0a 2020 2020 2020 2020 2020  nfig>.          
+00005b30: 3c4f 7074 696f 6e2f 3e0a 2020 2020 2020  <Option/>.      
+00005b40: 2020 3c2f 636f 6e66 6967 3e0a 2020 2020    </config>.    
+00005b50: 2020 3c2f 6564 6974 5769 6467 6574 3e0a    </editWidget>.
+00005b60: 2020 2020 3c2f 6669 656c 643e 0a20 2020      </field>.   
+00005b70: 203c 6669 656c 6420 6e61 6d65 3d22 6f73   <field name="os
+00005b80: 6d5f 6964 2220 636f 6e66 6967 7572 6174  m_id" configurat
+00005b90: 696f 6e46 6c61 6773 3d22 4e6f 6e65 223e  ionFlags="None">
+00005ba0: 0a20 2020 2020 203c 6564 6974 5769 6467  .      <editWidg
+00005bb0: 6574 2074 7970 653d 2254 6578 7445 6469  et type="TextEdi
+00005bc0: 7422 3e0a 2020 2020 2020 2020 3c63 6f6e  t">.        <con
+00005bd0: 6669 673e 0a20 2020 2020 2020 2020 203c  fig>.          <
+00005be0: 4f70 7469 6f6e 2f3e 0a20 2020 2020 2020  Option/>.       
+00005bf0: 203c 2f63 6f6e 6669 673e 0a20 2020 2020   </config>.     
+00005c00: 203c 2f65 6469 7457 6964 6765 743e 0a20   </editWidget>. 
+00005c10: 2020 203c 2f66 6965 6c64 3e0a 2020 2020     </field>.    
+00005c20: 3c66 6965 6c64 206e 616d 653d 226f 7269  <field name="ori
+00005c30: 656e 7461 7469 6f6e 2220 636f 6e66 6967  entation" config
+00005c40: 7572 6174 696f 6e46 6c61 6773 3d22 4e6f  urationFlags="No
+00005c50: 6e65 223e 0a20 2020 2020 203c 6564 6974  ne">.      <edit
+00005c60: 5769 6467 6574 2074 7970 653d 2254 6578  Widget type="Tex
+00005c70: 7445 6469 7422 3e0a 2020 2020 2020 2020  tEdit">.        
+00005c80: 3c63 6f6e 6669 673e 0a20 2020 2020 2020  <config>.       
+00005c90: 2020 203c 4f70 7469 6f6e 2f3e 0a20 2020     <Option/>.   
+00005ca0: 2020 2020 203c 2f63 6f6e 6669 673e 0a20       </config>. 
+00005cb0: 2020 2020 203c 2f65 6469 7457 6964 6765       </editWidge
+00005cc0: 743e 0a20 2020 203c 2f66 6965 6c64 3e0a  t>.    </field>.
+00005cd0: 2020 2020 3c66 6965 6c64 206e 616d 653d      <field name=
+00005ce0: 226f 7269 656e 7461 7469 6f6e 5f63 6f6e  "orientation_con
+00005cf0: 6669 6465 6e63 6522 2063 6f6e 6669 6775  fidence" configu
+00005d00: 7261 7469 6f6e 466c 6167 733d 224e 6f6e  rationFlags="Non
+00005d10: 6522 3e0a 2020 2020 2020 3c65 6469 7457  e">.      <editW
+00005d20: 6964 6765 7420 7479 7065 3d22 5465 7874  idget type="Text
+00005d30: 4564 6974 223e 0a20 2020 2020 2020 203c  Edit">.        <
+00005d40: 636f 6e66 6967 3e0a 2020 2020 2020 2020  config>.        
+00005d50: 2020 3c4f 7074 696f 6e2f 3e0a 2020 2020    <Option/>.    
+00005d60: 2020 2020 3c2f 636f 6e66 6967 3e0a 2020      </config>.  
+00005d70: 2020 2020 3c2f 6564 6974 5769 6467 6574      </editWidget
+00005d80: 3e0a 2020 2020 3c2f 6669 656c 643e 0a20  >.    </field>. 
+00005d90: 2020 203c 6669 656c 6420 6e61 6d65 3d22     <field name="
+00005da0: 6c61 6e65 5f77 6964 7468 2220 636f 6e66  lane_width" conf
+00005db0: 6967 7572 6174 696f 6e46 6c61 6773 3d22  igurationFlags="
+00005dc0: 4e6f 6e65 223e 0a20 2020 2020 203c 6564  None">.      <ed
+00005dd0: 6974 5769 6467 6574 2074 7970 653d 2254  itWidget type="T
+00005de0: 6578 7445 6469 7422 3e0a 2020 2020 2020  extEdit">.      
+00005df0: 2020 3c63 6f6e 6669 673e 0a20 2020 2020    <config>.     
+00005e00: 2020 2020 203c 4f70 7469 6f6e 2f3e 0a20       <Option/>. 
+00005e10: 2020 2020 2020 203c 2f63 6f6e 6669 673e         </config>
+00005e20: 0a20 2020 2020 203c 2f65 6469 7457 6964  .      </editWid
+00005e30: 6765 743e 0a20 2020 203c 2f66 6965 6c64  get>.    </field
+00005e40: 3e0a 2020 2020 3c66 6965 6c64 206e 616d  >.    <field nam
+00005e50: 653d 226c 616e 655f 6f72 6965 6e74 6174  e="lane_orientat
+00005e60: 696f 6e22 2063 6f6e 6669 6775 7261 7469  ion" configurati
+00005e70: 6f6e 466c 6167 733d 224e 6f6e 6522 3e0a  onFlags="None">.
+00005e80: 2020 2020 2020 3c65 6469 7457 6964 6765        <editWidge
+00005e90: 7420 7479 7065 3d22 5465 7874 4564 6974  t type="TextEdit
+00005ea0: 223e 0a20 2020 2020 2020 203c 636f 6e66  ">.        <conf
+00005eb0: 6967 3e0a 2020 2020 2020 2020 2020 3c4f  ig>.          <O
+00005ec0: 7074 696f 6e2f 3e0a 2020 2020 2020 2020  ption/>.        
+00005ed0: 3c2f 636f 6e66 6967 3e0a 2020 2020 2020  </config>.      
+00005ee0: 3c2f 6564 6974 5769 6467 6574 3e0a 2020  </editWidget>.  
+00005ef0: 2020 3c2f 6669 656c 643e 0a20 203c 2f66    </field>.  </f
+00005f00: 6965 6c64 436f 6e66 6967 7572 6174 696f  ieldConfiguratio
+00005f10: 6e3e 0a20 203c 616c 6961 7365 733e 0a20  n>.  <aliases>. 
+00005f20: 2020 203c 616c 6961 7320 6e61 6d65 3d22     <alias name="
+00005f30: 2220 696e 6465 783d 2230 2220 6669 656c  " index="0" fiel
+00005f40: 643d 2274 7970 6522 2f3e 0a20 2020 203c  d="type"/>.    <
+00005f50: 616c 6961 7320 6e61 6d65 3d22 2220 696e  alias name="" in
+00005f60: 6465 783d 2231 2220 6669 656c 643d 226f  dex="1" field="o
+00005f70: 736d 5f69 6422 2f3e 0a20 2020 203c 616c  sm_id"/>.    <al
+00005f80: 6961 7320 6e61 6d65 3d22 2220 696e 6465  ias name="" inde
+00005f90: 783d 2232 2220 6669 656c 643d 226f 7269  x="2" field="ori
+00005fa0: 656e 7461 7469 6f6e 222f 3e0a 2020 2020  entation"/>.    
+00005fb0: 3c61 6c69 6173 206e 616d 653d 2222 2069  <alias name="" i
+00005fc0: 6e64 6578 3d22 3322 2066 6965 6c64 3d22  ndex="3" field="
+00005fd0: 6f72 6965 6e74 6174 696f 6e5f 636f 6e66  orientation_conf
+00005fe0: 6964 656e 6365 222f 3e0a 2020 2020 3c61  idence"/>.    <a
+00005ff0: 6c69 6173 206e 616d 653d 2222 2069 6e64  lias name="" ind
+00006000: 6578 3d22 3422 2066 6965 6c64 3d22 6c61  ex="4" field="la
+00006010: 6e65 5f77 6964 7468 222f 3e0a 2020 2020  ne_width"/>.    
+00006020: 3c61 6c69 6173 206e 616d 653d 2222 2069  <alias name="" i
+00006030: 6e64 6578 3d22 3522 2066 6965 6c64 3d22  ndex="5" field="
+00006040: 6c61 6e65 5f6f 7269 656e 7461 7469 6f6e  lane_orientation
+00006050: 222f 3e0a 2020 3c2f 616c 6961 7365 733e  "/>.  </aliases>
+00006060: 0a20 203c 6465 6661 756c 7473 3e0a 2020  .  <defaults>.  
+00006070: 2020 3c64 6566 6175 6c74 2066 6965 6c64    <default field
+00006080: 3d22 7479 7065 2220 6170 706c 794f 6e55  ="type" applyOnU
+00006090: 7064 6174 653d 2230 2220 6578 7072 6573  pdate="0" expres
+000060a0: 7369 6f6e 3d22 222f 3e0a 2020 2020 3c64  sion=""/>.    <d
+000060b0: 6566 6175 6c74 2066 6965 6c64 3d22 6f73  efault field="os
+000060c0: 6d5f 6964 2220 6170 706c 794f 6e55 7064  m_id" applyOnUpd
+000060d0: 6174 653d 2230 2220 6578 7072 6573 7369  ate="0" expressi
+000060e0: 6f6e 3d22 222f 3e0a 2020 2020 3c64 6566  on=""/>.    <def
+000060f0: 6175 6c74 2066 6965 6c64 3d22 6f72 6965  ault field="orie
+00006100: 6e74 6174 696f 6e22 2061 7070 6c79 4f6e  ntation" applyOn
+00006110: 5570 6461 7465 3d22 3022 2065 7870 7265  Update="0" expre
+00006120: 7373 696f 6e3d 2222 2f3e 0a20 2020 203c  ssion=""/>.    <
+00006130: 6465 6661 756c 7420 6669 656c 643d 226f  default field="o
+00006140: 7269 656e 7461 7469 6f6e 5f63 6f6e 6669  rientation_confi
+00006150: 6465 6e63 6522 2061 7070 6c79 4f6e 5570  dence" applyOnUp
+00006160: 6461 7465 3d22 3022 2065 7870 7265 7373  date="0" express
+00006170: 696f 6e3d 2222 2f3e 0a20 2020 203c 6465  ion=""/>.    <de
+00006180: 6661 756c 7420 6669 656c 643d 226c 616e  fault field="lan
+00006190: 655f 7769 6474 6822 2061 7070 6c79 4f6e  e_width" applyOn
+000061a0: 5570 6461 7465 3d22 3022 2065 7870 7265  Update="0" expre
+000061b0: 7373 696f 6e3d 2222 2f3e 0a20 2020 203c  ssion=""/>.    <
+000061c0: 6465 6661 756c 7420 6669 656c 643d 226c  default field="l
+000061d0: 616e 655f 6f72 6965 6e74 6174 696f 6e22  ane_orientation"
+000061e0: 2061 7070 6c79 4f6e 5570 6461 7465 3d22   applyOnUpdate="
+000061f0: 3022 2065 7870 7265 7373 696f 6e3d 2222  0" expression=""
+00006200: 2f3e 0a20 203c 2f64 6566 6175 6c74 733e  />.  </defaults>
+00006210: 0a20 203c 636f 6e73 7472 6169 6e74 733e  .  <constraints>
+00006220: 0a20 2020 203c 636f 6e73 7472 6169 6e74  .    <constraint
+00006230: 206e 6f74 6e75 6c6c 5f73 7472 656e 6774   notnull_strengt
+00006240: 683d 2230 2220 636f 6e73 7472 6169 6e74  h="0" constraint
+00006250: 733d 2230 2220 756e 6971 7565 5f73 7472  s="0" unique_str
+00006260: 656e 6774 683d 2230 2220 6669 656c 643d  ength="0" field=
+00006270: 2274 7970 6522 2065 7870 5f73 7472 656e  "type" exp_stren
+00006280: 6774 683d 2230 222f 3e0a 2020 2020 3c63  gth="0"/>.    <c
+00006290: 6f6e 7374 7261 696e 7420 6e6f 746e 756c  onstraint notnul
+000062a0: 6c5f 7374 7265 6e67 7468 3d22 3022 2063  l_strength="0" c
+000062b0: 6f6e 7374 7261 696e 7473 3d22 3022 2075  onstraints="0" u
+000062c0: 6e69 7175 655f 7374 7265 6e67 7468 3d22  nique_strength="
+000062d0: 3022 2066 6965 6c64 3d22 6f73 6d5f 6964  0" field="osm_id
+000062e0: 2220 6578 705f 7374 7265 6e67 7468 3d22  " exp_strength="
+000062f0: 3022 2f3e 0a20 2020 203c 636f 6e73 7472  0"/>.    <constr
+00006300: 6169 6e74 206e 6f74 6e75 6c6c 5f73 7472  aint notnull_str
+00006310: 656e 6774 683d 2230 2220 636f 6e73 7472  ength="0" constr
+00006320: 6169 6e74 733d 2230 2220 756e 6971 7565  aints="0" unique
+00006330: 5f73 7472 656e 6774 683d 2230 2220 6669  _strength="0" fi
+00006340: 656c 643d 226f 7269 656e 7461 7469 6f6e  eld="orientation
+00006350: 2220 6578 705f 7374 7265 6e67 7468 3d22  " exp_strength="
+00006360: 3022 2f3e 0a20 2020 203c 636f 6e73 7472  0"/>.    <constr
+00006370: 6169 6e74 206e 6f74 6e75 6c6c 5f73 7472  aint notnull_str
+00006380: 656e 6774 683d 2230 2220 636f 6e73 7472  ength="0" constr
+00006390: 6169 6e74 733d 2230 2220 756e 6971 7565  aints="0" unique
+000063a0: 5f73 7472 656e 6774 683d 2230 2220 6669  _strength="0" fi
+000063b0: 656c 643d 226f 7269 656e 7461 7469 6f6e  eld="orientation
+000063c0: 5f63 6f6e 6669 6465 6e63 6522 2065 7870  _confidence" exp
+000063d0: 5f73 7472 656e 6774 683d 2230 222f 3e0a  _strength="0"/>.
+000063e0: 2020 2020 3c63 6f6e 7374 7261 696e 7420      <constraint 
+000063f0: 6e6f 746e 756c 6c5f 7374 7265 6e67 7468  notnull_strength
+00006400: 3d22 3022 2063 6f6e 7374 7261 696e 7473  ="0" constraints
+00006410: 3d22 3022 2075 6e69 7175 655f 7374 7265  ="0" unique_stre
+00006420: 6e67 7468 3d22 3022 2066 6965 6c64 3d22  ngth="0" field="
+00006430: 6c61 6e65 5f77 6964 7468 2220 6578 705f  lane_width" exp_
+00006440: 7374 7265 6e67 7468 3d22 3022 2f3e 0a20  strength="0"/>. 
+00006450: 2020 203c 636f 6e73 7472 6169 6e74 206e     <constraint n
+00006460: 6f74 6e75 6c6c 5f73 7472 656e 6774 683d  otnull_strength=
+00006470: 2230 2220 636f 6e73 7472 6169 6e74 733d  "0" constraints=
+00006480: 2230 2220 756e 6971 7565 5f73 7472 656e  "0" unique_stren
+00006490: 6774 683d 2230 2220 6669 656c 643d 226c  gth="0" field="l
+000064a0: 616e 655f 6f72 6965 6e74 6174 696f 6e22  ane_orientation"
+000064b0: 2065 7870 5f73 7472 656e 6774 683d 2230   exp_strength="0
+000064c0: 222f 3e0a 2020 3c2f 636f 6e73 7472 6169  "/>.  </constrai
+000064d0: 6e74 733e 0a20 203c 636f 6e73 7472 6169  nts>.  <constrai
+000064e0: 6e74 4578 7072 6573 7369 6f6e 733e 0a20  ntExpressions>. 
+000064f0: 2020 203c 636f 6e73 7472 6169 6e74 2065     <constraint e
+00006500: 7870 3d22 2220 6465 7363 3d22 2220 6669  xp="" desc="" fi
+00006510: 656c 643d 2274 7970 6522 2f3e 0a20 2020  eld="type"/>.   
+00006520: 203c 636f 6e73 7472 6169 6e74 2065 7870   <constraint exp
+00006530: 3d22 2220 6465 7363 3d22 2220 6669 656c  ="" desc="" fiel
+00006540: 643d 226f 736d 5f69 6422 2f3e 0a20 2020  d="osm_id"/>.   
+00006550: 203c 636f 6e73 7472 6169 6e74 2065 7870   <constraint exp
+00006560: 3d22 2220 6465 7363 3d22 2220 6669 656c  ="" desc="" fiel
+00006570: 643d 226f 7269 656e 7461 7469 6f6e 222f  d="orientation"/
+00006580: 3e0a 2020 2020 3c63 6f6e 7374 7261 696e  >.    <constrain
+00006590: 7420 6578 703d 2222 2064 6573 633d 2222  t exp="" desc=""
+000065a0: 2066 6965 6c64 3d22 6f72 6965 6e74 6174   field="orientat
+000065b0: 696f 6e5f 636f 6e66 6964 656e 6365 222f  ion_confidence"/
+000065c0: 3e0a 2020 2020 3c63 6f6e 7374 7261 696e  >.    <constrain
+000065d0: 7420 6578 703d 2222 2064 6573 633d 2222  t exp="" desc=""
+000065e0: 2066 6965 6c64 3d22 6c61 6e65 5f77 6964   field="lane_wid
+000065f0: 7468 222f 3e0a 2020 2020 3c63 6f6e 7374  th"/>.    <const
+00006600: 7261 696e 7420 6578 703d 2222 2064 6573  raint exp="" des
+00006610: 633d 2222 2066 6965 6c64 3d22 6c61 6e65  c="" field="lane
+00006620: 5f6f 7269 656e 7461 7469 6f6e 222f 3e0a  _orientation"/>.
+00006630: 2020 3c2f 636f 6e73 7472 6169 6e74 4578    </constraintEx
+00006640: 7072 6573 7369 6f6e 733e 0a20 203c 6578  pressions>.  <ex
+00006650: 7072 6573 7369 6f6e 6669 656c 6473 2f3e  pressionfields/>
+00006660: 0a20 203c 6174 7472 6962 7574 6561 6374  .  <attributeact
+00006670: 696f 6e73 3e0a 2020 2020 3c64 6566 6175  ions>.    <defau
+00006680: 6c74 4163 7469 6f6e 206b 6579 3d22 4361  ltAction key="Ca
+00006690: 6e76 6173 2220 7661 6c75 653d 227b 3030  nvas" value="{00
+000066a0: 3030 3030 3030 2d30 3030 302d 3030 3030  000000-0000-0000
+000066b0: 2d30 3030 302d 3030 3030 3030 3030 3030  -0000-0000000000
+000066c0: 3030 7d22 2f3e 0a20 203c 2f61 7474 7269  00}"/>.  </attri
+000066d0: 6275 7465 6163 7469 6f6e 733e 0a20 203c  buteactions>.  <
+000066e0: 6174 7472 6962 7574 6574 6162 6c65 636f  attributetableco
+000066f0: 6e66 6967 2073 6f72 7445 7870 7265 7373  nfig sortExpress
+00006700: 696f 6e3d 2222 2073 6f72 744f 7264 6572  ion="" sortOrder
+00006710: 3d22 3022 2061 6374 696f 6e57 6964 6765  ="0" actionWidge
+00006720: 7453 7479 6c65 3d22 6472 6f70 446f 776e  tStyle="dropDown
+00006730: 223e 0a20 2020 203c 636f 6c75 6d6e 733e  ">.    <columns>
+00006740: 0a20 2020 2020 203c 636f 6c75 6d6e 206e  .      <column n
+00006750: 616d 653d 2274 7970 6522 2077 6964 7468  ame="type" width
+00006760: 3d22 2d31 2220 6869 6464 656e 3d22 3022  ="-1" hidden="0"
+00006770: 2074 7970 653d 2266 6965 6c64 222f 3e0a   type="field"/>.
+00006780: 2020 2020 2020 3c63 6f6c 756d 6e20 6e61        <column na
+00006790: 6d65 3d22 6f73 6d5f 6964 2220 7769 6474  me="osm_id" widt
+000067a0: 683d 2231 3731 2220 6869 6464 656e 3d22  h="171" hidden="
+000067b0: 3022 2074 7970 653d 2266 6965 6c64 222f  0" type="field"/
+000067c0: 3e0a 2020 2020 2020 3c63 6f6c 756d 6e20  >.      <column 
+000067d0: 6e61 6d65 3d22 6f72 6965 6e74 6174 696f  name="orientatio
+000067e0: 6e22 2077 6964 7468 3d22 3239 3222 2068  n" width="292" h
+000067f0: 6964 6465 6e3d 2230 2220 7479 7065 3d22  idden="0" type="
+00006800: 6669 656c 6422 2f3e 0a20 2020 2020 203c  field"/>.      <
+00006810: 636f 6c75 6d6e 206e 616d 653d 226f 7269  column name="ori
+00006820: 656e 7461 7469 6f6e 5f63 6f6e 6669 6465  entation_confide
+00006830: 6e63 6522 2077 6964 7468 3d22 2d31 2220  nce" width="-1" 
+00006840: 6869 6464 656e 3d22 3022 2074 7970 653d  hidden="0" type=
+00006850: 2266 6965 6c64 222f 3e0a 2020 2020 2020  "field"/>.      
+00006860: 3c63 6f6c 756d 6e20 6e61 6d65 3d22 6c61  <column name="la
+00006870: 6e65 5f6f 7269 656e 7461 7469 6f6e 2220  ne_orientation" 
+00006880: 7769 6474 683d 222d 3122 2068 6964 6465  width="-1" hidde
+00006890: 6e3d 2230 2220 7479 7065 3d22 6669 656c  n="0" type="fiel
+000068a0: 6422 2f3e 0a20 2020 2020 203c 636f 6c75  d"/>.      <colu
+000068b0: 6d6e 206e 616d 653d 226c 616e 655f 7769  mn name="lane_wi
+000068c0: 6474 6822 2077 6964 7468 3d22 2d31 2220  dth" width="-1" 
+000068d0: 6869 6464 656e 3d22 3022 2074 7970 653d  hidden="0" type=
+000068e0: 2266 6965 6c64 222f 3e0a 2020 2020 2020  "field"/>.      
+000068f0: 3c63 6f6c 756d 6e20 7769 6474 683d 222d  <column width="-
+00006900: 3122 2068 6964 6465 6e3d 2231 2220 7479  1" hidden="1" ty
+00006910: 7065 3d22 6163 7469 6f6e 7322 2f3e 0a20  pe="actions"/>. 
+00006920: 2020 203c 2f63 6f6c 756d 6e73 3e0a 2020     </columns>.  
+00006930: 3c2f 6174 7472 6962 7574 6574 6162 6c65  </attributetable
+00006940: 636f 6e66 6967 3e0a 2020 3c63 6f6e 6469  config>.  <condi
+00006950: 7469 6f6e 616c 7374 796c 6573 3e0a 2020  tionalstyles>.  
+00006960: 2020 3c72 6f77 7374 796c 6573 2f3e 0a20    <rowstyles/>. 
+00006970: 2020 203c 6669 656c 6473 7479 6c65 732f     <fieldstyles/
+00006980: 3e0a 2020 3c2f 636f 6e64 6974 696f 6e61  >.  </conditiona
+00006990: 6c73 7479 6c65 733e 0a20 203c 7374 6f72  lstyles>.  <stor
+000069a0: 6564 6578 7072 6573 7369 6f6e 732f 3e0a  edexpressions/>.
+000069b0: 2020 3c65 6469 7466 6f72 6d20 746f 6c65    <editform tole
+000069c0: 7261 6e74 3d22 3122 3e3c 2f65 6469 7466  rant="1"></editf
+000069d0: 6f72 6d3e 0a20 203c 6564 6974 666f 726d  orm>.  <editform
+000069e0: 696e 6974 2f3e 0a20 203c 6564 6974 666f  init/>.  <editfo
+000069f0: 726d 696e 6974 636f 6465 736f 7572 6365  rminitcodesource
+00006a00: 3e30 3c2f 6564 6974 666f 726d 696e 6974  >0</editforminit
+00006a10: 636f 6465 736f 7572 6365 3e0a 2020 3c65  codesource>.  <e
+00006a20: 6469 7466 6f72 6d69 6e69 7466 696c 6570  ditforminitfilep
+00006a30: 6174 683e 3c2f 6564 6974 666f 726d 696e  ath></editformin
+00006a40: 6974 6669 6c65 7061 7468 3e0a 2020 3c65  itfilepath>.  <e
+00006a50: 6469 7466 6f72 6d69 6e69 7463 6f64 653e  ditforminitcode>
+00006a60: 3c21 5b43 4441 5441 5b23 202d 2a2d 2063  <![CDATA[# -*- c
+00006a70: 6f64 696e 673a 2075 7466 2d38 202d 2a2d  oding: utf-8 -*-
+00006a80: 0a22 2222 0a4c 6573 2066 6f72 6d75 6c61  .""".Les formula
+00006a90: 6972 6573 2051 4749 5320 7065 7576 656e  ires QGIS peuven
+00006aa0: 7420 6176 6f69 7220 756e 6520 666f 6e63  t avoir une fonc
+00006ab0: 7469 6f6e 2050 7974 686f 6e20 7175 6920  tion Python qui 
+00006ac0: 6573 7420 6170 7065 6cc3 a965 206c 6f72  est appel..e lor
+00006ad0: 7371 7565 206c 6520 666f 726d 756c 6169  sque le formulai
+00006ae0: 7265 2065 7374 0a6f 7576 6572 742e 0a0a  re est.ouvert...
+00006af0: 5574 696c 6973 657a 2063 6574 7465 2066  Utilisez cette f
+00006b00: 6f6e 6374 696f 6e20 706f 7572 2061 6a6f  onction pour ajo
+00006b10: 7574 6572 2075 6e65 206c 6f67 6971 7565  uter une logique
+00006b20: 2073 7570 706c c3a9 6d65 6e74 6169 7265   suppl..mentaire
+00006b30: 20c3 a020 766f 7320 666f 726d 756c 6169   .. vos formulai
+00006b40: 7265 732e 0a0a 456e 7472 657a 206c 6520  res...Entrez le 
+00006b50: 6e6f 6d20 6465 206c 6120 666f 6e63 7469  nom de la foncti
+00006b60: 6f6e 2064 616e 7320 6c65 2063 6861 6d70  on dans le champ
+00006b70: 200a 2246 6f6e 6374 696f 6e20 6427 696e   ."Fonction d'in
+00006b80: 6974 6961 6c69 7361 7469 6f6e 2050 7974  itialisation Pyt
+00006b90: 686f 6e22 2e0a 566f 6963 6920 756e 2065  hon"..Voici un e
+00006ba0: 7865 6d70 6c65 3a0a 2222 220a 6672 6f6d  xemple:.""".from
+00006bb0: 2071 6769 732e 5079 5174 2e51 7457 6964   qgis.PyQt.QtWid
+00006bc0: 6765 7473 2069 6d70 6f72 7420 5157 6964  gets import QWid
+00006bd0: 6765 740a 0a64 6566 206d 795f 666f 726d  get..def my_form
+00006be0: 5f6f 7065 6e28 6469 616c 6f67 2c20 6c61  _open(dialog, la
+00006bf0: 7965 722c 2066 6561 7475 7265 293a 0a20  yer, feature):. 
+00006c00: 2020 2067 656f 6d20 3d20 6665 6174 7572     geom = featur
+00006c10: 652e 6765 6f6d 6574 7279 2829 0a20 2020  e.geometry().   
+00006c20: 2063 6f6e 7472 6f6c 203d 2064 6961 6c6f   control = dialo
+00006c30: 672e 6669 6e64 4368 696c 6428 5157 6964  g.findChild(QWid
+00006c40: 6765 742c 2022 4d79 4c69 6e65 4564 6974  get, "MyLineEdit
+00006c50: 2229 0a5d 5d3e 3c2f 6564 6974 666f 726d  ").]]></editform
+00006c60: 696e 6974 636f 6465 3e0a 2020 3c66 6561  initcode>.  <fea
+00006c70: 7466 6f72 6d73 7570 7072 6573 733e 303c  tformsuppress>0<
+00006c80: 2f66 6561 7466 6f72 6d73 7570 7072 6573  /featformsuppres
+00006c90: 733e 0a20 203c 6564 6974 6f72 6c61 796f  s>.  <editorlayo
+00006ca0: 7574 3e67 656e 6572 6174 6564 6c61 796f  ut>generatedlayo
+00006cb0: 7574 3c2f 6564 6974 6f72 6c61 796f 7574  ut</editorlayout
+00006cc0: 3e0a 2020 3c65 6469 7461 626c 653e 0a20  >.  <editable>. 
+00006cd0: 2020 203c 6669 656c 6420 6e61 6d65 3d22     <field name="
+00006ce0: 616e 676c 6522 2065 6469 7461 626c 653d  angle" editable=
+00006cf0: 2231 222f 3e0a 2020 2020 3c66 6965 6c64  "1"/>.    <field
+00006d00: 206e 616d 653d 2266 6964 2220 6564 6974   name="fid" edit
+00006d10: 6162 6c65 3d22 3122 2f3e 0a20 2020 203c  able="1"/>.    <
+00006d20: 6669 656c 6420 6e61 6d65 3d22 6c61 6e65  field name="lane
+00006d30: 5f6f 7269 656e 7461 7469 6f6e 2220 6564  _orientation" ed
+00006d40: 6974 6162 6c65 3d22 3122 2f3e 0a20 2020  itable="1"/>.   
+00006d50: 203c 6669 656c 6420 6e61 6d65 3d22 6c61   <field name="la
+00006d60: 6e65 5f77 6964 7468 2220 6564 6974 6162  ne_width" editab
+00006d70: 6c65 3d22 3122 2f3e 0a20 2020 203c 6669  le="1"/>.    <fi
+00006d80: 656c 6420 6e61 6d65 3d22 6f72 6965 6e74  eld name="orient
+00006d90: 6174 696f 6e22 2065 6469 7461 626c 653d  ation" editable=
+00006da0: 2231 222f 3e0a 2020 2020 3c66 6965 6c64  "1"/>.    <field
+00006db0: 206e 616d 653d 226f 7269 656e 7461 7469   name="orientati
+00006dc0: 6f6e 5f63 6f6e 6669 6465 6e63 6522 2065  on_confidence" e
+00006dd0: 6469 7461 626c 653d 2231 222f 3e0a 2020  ditable="1"/>.  
+00006de0: 2020 3c66 6965 6c64 206e 616d 653d 226f    <field name="o
+00006df0: 736d 5f69 6422 2065 6469 7461 626c 653d  sm_id" editable=
+00006e00: 2231 222f 3e0a 2020 2020 3c66 6965 6c64  "1"/>.    <field
+00006e10: 206e 616d 653d 2274 7970 6522 2065 6469   name="type" edi
+00006e20: 7461 626c 653d 2231 222f 3e0a 2020 3c2f  table="1"/>.  </
+00006e30: 6564 6974 6162 6c65 3e0a 2020 3c6c 6162  editable>.  <lab
+00006e40: 656c 4f6e 546f 703e 0a20 2020 203c 6669  elOnTop>.    <fi
+00006e50: 656c 6420 6e61 6d65 3d22 616e 676c 6522  eld name="angle"
+00006e60: 206c 6162 656c 4f6e 546f 703d 2230 222f   labelOnTop="0"/
+00006e70: 3e0a 2020 2020 3c66 6965 6c64 206e 616d  >.    <field nam
+00006e80: 653d 2266 6964 2220 6c61 6265 6c4f 6e54  e="fid" labelOnT
+00006e90: 6f70 3d22 3022 2f3e 0a20 2020 203c 6669  op="0"/>.    <fi
+00006ea0: 656c 6420 6e61 6d65 3d22 6c61 6e65 5f6f  eld name="lane_o
+00006eb0: 7269 656e 7461 7469 6f6e 2220 6c61 6265  rientation" labe
+00006ec0: 6c4f 6e54 6f70 3d22 3022 2f3e 0a20 2020  lOnTop="0"/>.   
+00006ed0: 203c 6669 656c 6420 6e61 6d65 3d22 6c61   <field name="la
+00006ee0: 6e65 5f77 6964 7468 2220 6c61 6265 6c4f  ne_width" labelO
+00006ef0: 6e54 6f70 3d22 3022 2f3e 0a20 2020 203c  nTop="0"/>.    <
+00006f00: 6669 656c 6420 6e61 6d65 3d22 6f72 6965  field name="orie
+00006f10: 6e74 6174 696f 6e22 206c 6162 656c 4f6e  ntation" labelOn
+00006f20: 546f 703d 2230 222f 3e0a 2020 2020 3c66  Top="0"/>.    <f
+00006f30: 6965 6c64 206e 616d 653d 226f 7269 656e  ield name="orien
+00006f40: 7461 7469 6f6e 5f63 6f6e 6669 6465 6e63  tation_confidenc
+00006f50: 6522 206c 6162 656c 4f6e 546f 703d 2230  e" labelOnTop="0
+00006f60: 222f 3e0a 2020 2020 3c66 6965 6c64 206e  "/>.    <field n
+00006f70: 616d 653d 226f 736d 5f69 6422 206c 6162  ame="osm_id" lab
+00006f80: 656c 4f6e 546f 703d 2230 222f 3e0a 2020  elOnTop="0"/>.  
+00006f90: 2020 3c66 6965 6c64 206e 616d 653d 2274    <field name="t
+00006fa0: 7970 6522 206c 6162 656c 4f6e 546f 703d  ype" labelOnTop=
+00006fb0: 2230 222f 3e0a 2020 3c2f 6c61 6265 6c4f  "0"/>.  </labelO
+00006fc0: 6e54 6f70 3e0a 2020 3c72 6575 7365 4c61  nTop>.  <reuseLa
+00006fd0: 7374 5661 6c75 653e 0a20 2020 203c 6669  stValue>.    <fi
+00006fe0: 656c 6420 6e61 6d65 3d22 616e 676c 6522  eld name="angle"
+00006ff0: 2072 6575 7365 4c61 7374 5661 6c75 653d   reuseLastValue=
+00007000: 2230 222f 3e0a 2020 2020 3c66 6965 6c64  "0"/>.    <field
+00007010: 206e 616d 653d 2266 6964 2220 7265 7573   name="fid" reus
+00007020: 654c 6173 7456 616c 7565 3d22 3022 2f3e  eLastValue="0"/>
+00007030: 0a20 2020 203c 6669 656c 6420 6e61 6d65  .    <field name
+00007040: 3d22 6c61 6e65 5f6f 7269 656e 7461 7469  ="lane_orientati
+00007050: 6f6e 2220 7265 7573 654c 6173 7456 616c  on" reuseLastVal
+00007060: 7565 3d22 3022 2f3e 0a20 2020 203c 6669  ue="0"/>.    <fi
+00007070: 656c 6420 6e61 6d65 3d22 6c61 6e65 5f77  eld name="lane_w
+00007080: 6964 7468 2220 7265 7573 654c 6173 7456  idth" reuseLastV
+00007090: 616c 7565 3d22 3022 2f3e 0a20 2020 203c  alue="0"/>.    <
+000070a0: 6669 656c 6420 6e61 6d65 3d22 6f72 6965  field name="orie
+000070b0: 6e74 6174 696f 6e22 2072 6575 7365 4c61  ntation" reuseLa
+000070c0: 7374 5661 6c75 653d 2230 222f 3e0a 2020  stValue="0"/>.  
+000070d0: 2020 3c66 6965 6c64 206e 616d 653d 226f    <field name="o
+000070e0: 7269 656e 7461 7469 6f6e 5f63 6f6e 6669  rientation_confi
+000070f0: 6465 6e63 6522 2072 6575 7365 4c61 7374  dence" reuseLast
+00007100: 5661 6c75 653d 2230 222f 3e0a 2020 2020  Value="0"/>.    
+00007110: 3c66 6965 6c64 206e 616d 653d 226f 736d  <field name="osm
+00007120: 5f69 6422 2072 6575 7365 4c61 7374 5661  _id" reuseLastVa
+00007130: 6c75 653d 2230 222f 3e0a 2020 2020 3c66  lue="0"/>.    <f
+00007140: 6965 6c64 206e 616d 653d 2274 7970 6522  ield name="type"
+00007150: 2072 6575 7365 4c61 7374 5661 6c75 653d   reuseLastValue=
+00007160: 2230 222f 3e0a 2020 3c2f 7265 7573 654c  "0"/>.  </reuseL
+00007170: 6173 7456 616c 7565 3e0a 2020 3c64 6174  astValue>.  <dat
+00007180: 6144 6566 696e 6564 4669 656c 6450 726f  aDefinedFieldPro
+00007190: 7065 7274 6965 732f 3e0a 2020 3c77 6964  perties/>.  <wid
+000071a0: 6765 7473 2f3e 0a20 203c 7072 6576 6965  gets/>.  <previe
+000071b0: 7745 7870 7265 7373 696f 6e3e 2274 7970  wExpression>"typ
+000071c0: 6522 3c2f 7072 6576 6965 7745 7870 7265  e"</previewExpre
+000071d0: 7373 696f 6e3e 0a20 203c 6d61 7054 6970  ssion>.  <mapTip
+000071e0: 3e3c 2f6d 6170 5469 703e 0a20 203c 6c61  ></mapTip>.  <la
+000071f0: 7965 7247 656f 6d65 7472 7954 7970 653e  yerGeometryType>
+00007200: 303c 2f6c 6179 6572 4765 6f6d 6574 7279  0</layerGeometry
+00007210: 5479 7065 3e0a 3c2f 7167 6973 3e0a       Type>.</qgis>.
```

### Comparing `crossroads-schematization-0.0.9/crschem/resources/rendering-nodes-islands.qml` & `crossroads-schematization-0.1.0/crschem/resources/rendering-nodes-islands.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.0.9/crschem/resources/rendering-nodes-space.qml` & `crossroads-schematization-0.1.0/crschem/resources/rendering-nodes-space.qml`

 * *Files 0% similar despite different names*

```diff
@@ -666,757 +666,758 @@
 00002990: 616e 676c 6522 2074 7970 653d 224d 6170  angle" type="Map
 000029a0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
 000029b0: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
 000029c0: 7565 3d22 7472 7565 2220 6e61 6d65 3d22  ue="true" name="
 000029d0: 6163 7469 7665 2220 7479 7065 3d22 626f  active" type="bo
 000029e0: 6f6c 222f 3e0a 2020 2020 2020 2020 2020  ol"/>.          
 000029f0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00002a00: 7661 6c75 653d 2231 3830 202b 2028 2d26  value="180 + (-&
-00002a10: 7175 6f74 3b6f 7269 656e 7461 7469 6f6e  quot;orientation
-00002a20: 2671 756f 743b 202f 2070 6928 2929 202a  &quot; / pi()) *
-00002a30: 2031 3830 2220 6e61 6d65 3d22 6578 7072   180" name="expr
-00002a40: 6573 7369 6f6e 2220 7479 7065 3d22 5153  ession" type="QS
-00002a50: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00002a60: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00002a70: 6f6e 2076 616c 7565 3d22 3322 206e 616d  on value="3" nam
-00002a80: 653d 2274 7970 6522 2074 7970 653d 2269  e="type" type="i
-00002a90: 6e74 222f 3e0a 2020 2020 2020 2020 2020  nt"/>.          
-00002aa0: 2020 2020 2020 3c2f 4f70 7469 6f6e 3e0a        </Option>.
-00002ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ac0: 3c4f 7074 696f 6e20 6e61 6d65 3d22 6f75  <Option name="ou
-00002ad0: 746c 696e 6557 6964 7468 2220 7479 7065  tlineWidth" type
-00002ae0: 3d22 4d61 7022 3e0a 2020 2020 2020 2020  ="Map">.        
-00002af0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00002b00: 6e20 7661 6c75 653d 2274 7275 6522 206e  n value="true" n
-00002b10: 616d 653d 2261 6374 6976 6522 2074 7970  ame="active" typ
-00002b20: 653d 2262 6f6f 6c22 2f3e 0a20 2020 2020  e="bool"/>.     
-00002b30: 2020 2020 2020 2020 2020 2020 203c 4f70               <Op
-00002b40: 7469 6f6e 2076 616c 7565 3d22 2671 756f  tion value="&quo
-00002b50: 743b 6c61 6e65 5f77 6964 7468 2671 756f  t;lane_width&quo
-00002b60: 743b 202a 2031 2e33 2220 6e61 6d65 3d22  t; * 1.3" name="
-00002b70: 6578 7072 6573 7369 6f6e 2220 7479 7065  expression" type
-00002b80: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-00002b90: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002ba0: 4f70 7469 6f6e 2076 616c 7565 3d22 3322  Option value="3"
-00002bb0: 206e 616d 653d 2274 7970 6522 2074 7970   name="type" typ
-00002bc0: 653d 2269 6e74 222f 3e0a 2020 2020 2020  e="int"/>.      
-00002bd0: 2020 2020 2020 2020 2020 3c2f 4f70 7469            </Opti
-00002be0: 6f6e 3e0a 2020 2020 2020 2020 2020 2020  on>.            
-00002bf0: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
-00002c00: 3d22 7369 7a65 2220 7479 7065 3d22 4d61  ="size" type="Ma
-00002c10: 7022 3e0a 2020 2020 2020 2020 2020 2020  p">.            
-00002c20: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
-00002c30: 6c75 653d 2274 7275 6522 206e 616d 653d  lue="true" name=
-00002c40: 2261 6374 6976 6522 2074 7970 653d 2262  "active" type="b
-00002c50: 6f6f 6c22 2f3e 0a20 2020 2020 2020 2020  ool"/>.         
-00002c60: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-00002c70: 2076 616c 7565 3d22 3320 2b20 3220 2a20   value="3 + 2 * 
-00002c80: 302e 3030 3220 2a20 2040 6d61 705f 7363  0.002 *  @map_sc
-00002c90: 616c 6522 206e 616d 653d 2265 7870 7265  ale" name="expre
-00002ca0: 7373 696f 6e22 2074 7970 653d 2251 5374  ssion" type="QSt
-00002cb0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-00002cc0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00002cd0: 6e20 7661 6c75 653d 2233 2220 6e61 6d65  n value="3" name
-00002ce0: 3d22 7479 7065 2220 7479 7065 3d22 696e  ="type" type="in
-00002cf0: 7422 2f3e 0a20 2020 2020 2020 2020 2020  t"/>.           
-00002d00: 2020 2020 203c 2f4f 7074 696f 6e3e 0a20       </Option>. 
-00002d10: 2020 2020 2020 2020 2020 2020 203c 2f4f               </O
-00002d20: 7074 696f 6e3e 0a20 2020 2020 2020 2020  ption>.         
-00002d30: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00002d40: 7565 3d22 636f 6c6c 6563 7469 6f6e 2220  ue="collection" 
-00002d50: 6e61 6d65 3d22 7479 7065 2220 7479 7065  name="type" type
-00002d60: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-00002d70: 2020 2020 2020 2020 203c 2f4f 7074 696f           </Optio
-00002d80: 6e3e 0a20 2020 2020 2020 2020 203c 2f64  n>.          </d
-00002d90: 6174 615f 6465 6669 6e65 645f 7072 6f70  ata_defined_prop
-00002da0: 6572 7469 6573 3e0a 2020 2020 2020 2020  erties>.        
-00002db0: 3c2f 6c61 7965 723e 0a20 2020 2020 203c  </layer>.      <
-00002dc0: 2f73 796d 626f 6c3e 0a20 2020 203c 2f73  /symbol>.    </s
-00002dd0: 796d 626f 6c73 3e0a 2020 3c2f 7265 6e64  ymbols>.  </rend
-00002de0: 6572 6572 2d76 323e 0a20 203c 6375 7374  erer-v2>.  <cust
-00002df0: 6f6d 7072 6f70 6572 7469 6573 3e0a 2020  omproperties>.  
-00002e00: 2020 3c4f 7074 696f 6e20 7479 7065 3d22    <Option type="
-00002e10: 4d61 7022 3e0a 2020 2020 2020 3c4f 7074  Map">.      <Opt
-00002e20: 696f 6e20 6e61 6d65 3d22 6475 616c 7669  ion name="dualvi
-00002e30: 6577 2f70 7265 7669 6577 4578 7072 6573  ew/previewExpres
-00002e40: 7369 6f6e 7322 2074 7970 653d 224c 6973  sions" type="Lis
-00002e50: 7422 3e0a 2020 2020 2020 2020 3c4f 7074  t">.        <Opt
-00002e60: 696f 6e20 7661 6c75 653d 2226 7175 6f74  ion value="&quot
-00002e70: 3b74 7970 6526 7175 6f74 3b22 2074 7970  ;type&quot;" typ
-00002e80: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00002e90: 2020 2020 3c2f 4f70 7469 6f6e 3e0a 2020      </Option>.  
-00002ea0: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-00002eb0: 653d 2230 2220 6e61 6d65 3d22 656d 6265  e="0" name="embe
-00002ec0: 6464 6564 5769 6467 6574 732f 636f 756e  ddedWidgets/coun
-00002ed0: 7422 2074 7970 653d 2269 6e74 222f 3e0a  t" type="int"/>.
-00002ee0: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
-00002ef0: 6d65 3d22 7661 7269 6162 6c65 4e61 6d65  me="variableName
-00002f00: 7322 2f3e 0a20 2020 2020 203c 4f70 7469  s"/>.      <Opti
-00002f10: 6f6e 206e 616d 653d 2276 6172 6961 626c  on name="variabl
-00002f20: 6556 616c 7565 7322 2f3e 0a20 2020 203c  eValues"/>.    <
-00002f30: 2f4f 7074 696f 6e3e 0a20 203c 2f63 7573  /Option>.  </cus
-00002f40: 746f 6d70 726f 7065 7274 6965 733e 0a20  tomproperties>. 
-00002f50: 203c 626c 656e 644d 6f64 653e 303c 2f62   <blendMode>0</b
-00002f60: 6c65 6e64 4d6f 6465 3e0a 2020 3c66 6561  lendMode>.  <fea
-00002f70: 7475 7265 426c 656e 644d 6f64 653e 303c  tureBlendMode>0<
-00002f80: 2f66 6561 7475 7265 426c 656e 644d 6f64  /featureBlendMod
-00002f90: 653e 0a20 203c 6c61 7965 724f 7061 6369  e>.  <layerOpaci
-00002fa0: 7479 3e31 3c2f 6c61 7965 724f 7061 6369  ty>1</layerOpaci
-00002fb0: 7479 3e0a 2020 3c53 696e 676c 6543 6174  ty>.  <SingleCat
-00002fc0: 6567 6f72 7944 6961 6772 616d 5265 6e64  egoryDiagramRend
-00002fd0: 6572 6572 2064 6961 6772 616d 5479 7065  erer diagramType
-00002fe0: 3d22 4869 7374 6f67 7261 6d22 2061 7474  ="Histogram" att
-00002ff0: 7269 6275 7465 4c65 6765 6e64 3d22 3122  ributeLegend="1"
-00003000: 3e0a 2020 2020 3c44 6961 6772 616d 4361  >.    <DiagramCa
-00003010: 7465 676f 7279 2070 656e 436f 6c6f 723d  tegory penColor=
-00003020: 2223 3030 3030 3030 2220 7065 6e57 6964  "#000000" penWid
-00003030: 7468 3d22 3022 2077 6964 7468 3d22 3135  th="0" width="15
-00003040: 2220 7369 7a65 5479 7065 3d22 4d4d 2220  " sizeType="MM" 
-00003050: 6469 7265 6374 696f 6e3d 2230 2220 6c61  direction="0" la
-00003060: 6265 6c50 6c61 6365 6d65 6e74 4d65 7468  belPlacementMeth
-00003070: 6f64 3d22 5848 6569 6768 7422 2065 6e61  od="XHeight" ena
-00003080: 626c 6564 3d22 3022 2062 6172 5769 6474  bled="0" barWidt
-00003090: 683d 2235 2220 6d61 7853 6361 6c65 4465  h="5" maxScaleDe
-000030a0: 6e6f 6d69 6e61 746f 723d 2231 652b 3038  nominator="1e+08
-000030b0: 2220 7370 6163 696e 6755 6e69 7453 6361  " spacingUnitSca
-000030c0: 6c65 3d22 3378 3a30 2c30 2c30 2c30 2c30  le="3x:0,0,0,0,0
-000030d0: 2c30 2220 6f70 6163 6974 793d 2231 2220  ,0" opacity="1" 
-000030e0: 7363 616c 6544 6570 656e 6465 6e63 793d  scaleDependency=
-000030f0: 2241 7265 6122 2062 6163 6b67 726f 756e  "Area" backgroun
-00003100: 6441 6c70 6861 3d22 3235 3522 206d 696e  dAlpha="255" min
-00003110: 5363 616c 6544 656e 6f6d 696e 6174 6f72  ScaleDenominator
-00003120: 3d22 3022 2073 7061 6369 6e67 556e 6974  ="0" spacingUnit
-00003130: 3d22 4d4d 2220 6d69 6e69 6d75 6d53 697a  ="MM" minimumSiz
-00003140: 653d 2230 2220 6261 636b 6772 6f75 6e64  e="0" background
-00003150: 436f 6c6f 723d 2223 6666 6666 6666 2220  Color="#ffffff" 
-00003160: 6c69 6e65 5369 7a65 5479 7065 3d22 4d4d  lineSizeType="MM
-00003170: 2220 6c69 6e65 5369 7a65 5363 616c 653d  " lineSizeScale=
-00003180: 2233 783a 302c 302c 302c 302c 302c 3022  "3x:0,0,0,0,0,0"
-00003190: 2073 697a 6553 6361 6c65 3d22 3378 3a30   sizeScale="3x:0
-000031a0: 2c30 2c30 2c30 2c30 2c30 2220 7363 616c  ,0,0,0,0,0" scal
-000031b0: 6542 6173 6564 5669 7369 6269 6c69 7479  eBasedVisibility
-000031c0: 3d22 3022 2073 7061 6369 6e67 3d22 3522  ="0" spacing="5"
-000031d0: 2072 6f74 6174 696f 6e4f 6666 7365 743d   rotationOffset=
-000031e0: 2232 3730 2220 6865 6967 6874 3d22 3135  "270" height="15
-000031f0: 2220 7368 6f77 4178 6973 3d22 3122 2064  " showAxis="1" d
-00003200: 6961 6772 616d 4f72 6965 6e74 6174 696f  iagramOrientatio
-00003210: 6e3d 2255 7022 2070 656e 416c 7068 613d  n="Up" penAlpha=
-00003220: 2232 3535 223e 0a20 2020 2020 203c 666f  "255">.      <fo
-00003230: 6e74 5072 6f70 6572 7469 6573 2062 6f6c  ntProperties bol
-00003240: 643d 2230 2220 7374 7269 6b65 7468 726f  d="0" strikethro
-00003250: 7567 683d 2230 2220 7374 796c 653d 2222  ugh="0" style=""
-00003260: 2075 6e64 6572 6c69 6e65 3d22 3022 2064   underline="0" d
-00003270: 6573 6372 6970 7469 6f6e 3d22 4e6f 746f  escription="Noto
-00003280: 2053 616e 732c 3130 2c2d 312c 302c 3530   Sans,10,-1,0,50
-00003290: 2c30 2c30 2c30 2c30 2c30 2220 6974 616c  ,0,0,0,0,0" ital
-000032a0: 6963 3d22 3022 2f3e 0a20 2020 2020 203c  ic="0"/>.      <
-000032b0: 6174 7472 6962 7574 6520 636f 6c6f 724f  attribute colorO
-000032c0: 7061 6369 7479 3d22 3122 2063 6f6c 6f72  pacity="1" color
-000032d0: 3d22 2330 3030 3030 3022 2066 6965 6c64  ="#000000" field
-000032e0: 3d22 2220 6c61 6265 6c3d 2222 2f3e 0a20  ="" label=""/>. 
-000032f0: 2020 2020 203c 6178 6973 5379 6d62 6f6c       <axisSymbol
-00003300: 3e0a 2020 2020 2020 2020 3c73 796d 626f  >.        <symbo
-00003310: 6c20 6672 616d 655f 7261 7465 3d22 3130  l frame_rate="10
-00003320: 2220 6e61 6d65 3d22 2220 616c 7068 613d  " name="" alpha=
-00003330: 2231 2220 6973 5f61 6e69 6d61 7465 643d  "1" is_animated=
-00003340: 2230 2220 636c 6970 5f74 6f5f 6578 7465  "0" clip_to_exte
-00003350: 6e74 3d22 3122 2074 7970 653d 226c 696e  nt="1" type="lin
-00003360: 6522 2066 6f72 6365 5f72 6872 3d22 3022  e" force_rhr="0"
-00003370: 3e0a 2020 2020 2020 2020 2020 3c64 6174  >.          <dat
-00003380: 615f 6465 6669 6e65 645f 7072 6f70 6572  a_defined_proper
-00003390: 7469 6573 3e0a 2020 2020 2020 2020 2020  ties>.          
-000033a0: 2020 3c4f 7074 696f 6e20 7479 7065 3d22    <Option type="
-000033b0: 4d61 7022 3e0a 2020 2020 2020 2020 2020  Map">.          
-000033c0: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-000033d0: 653d 2222 206e 616d 653d 226e 616d 6522  e="" name="name"
-000033e0: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-000033f0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00003400: 3c4f 7074 696f 6e20 6e61 6d65 3d22 7072  <Option name="pr
-00003410: 6f70 6572 7469 6573 222f 3e0a 2020 2020  operties"/>.    
-00003420: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00003430: 6e20 7661 6c75 653d 2263 6f6c 6c65 6374  n value="collect
-00003440: 696f 6e22 206e 616d 653d 2274 7970 6522  ion" name="type"
-00003450: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-00003460: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
-00003470: 4f70 7469 6f6e 3e0a 2020 2020 2020 2020  Option>.        
-00003480: 2020 3c2f 6461 7461 5f64 6566 696e 6564    </data_defined
-00003490: 5f70 726f 7065 7274 6965 733e 0a20 2020  _properties>.   
-000034a0: 2020 2020 2020 203c 6c61 7965 7220 636c         <layer cl
-000034b0: 6173 733d 2253 696d 706c 654c 696e 6522  ass="SimpleLine"
-000034c0: 2070 6173 733d 2230 2220 656e 6162 6c65   pass="0" enable
-000034d0: 643d 2231 2220 6c6f 636b 6564 3d22 3022  d="1" locked="0"
-000034e0: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
-000034f0: 7074 696f 6e20 7479 7065 3d22 4d61 7022  ption type="Map"
-00003500: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00003510: 3c4f 7074 696f 6e20 7661 6c75 653d 2230  <Option value="0
-00003520: 2220 6e61 6d65 3d22 616c 6967 6e5f 6461  " name="align_da
-00003530: 7368 5f70 6174 7465 726e 2220 7479 7065  sh_pattern" type
-00003540: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-00003550: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00003560: 6f6e 2076 616c 7565 3d22 7371 7561 7265  on value="square
-00003570: 2220 6e61 6d65 3d22 6361 7073 7479 6c65  " name="capstyle
-00003580: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00003590: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
-000035a0: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-000035b0: 353b 3222 206e 616d 653d 2263 7573 746f  5;2" name="custo
-000035c0: 6d64 6173 6822 2074 7970 653d 2251 5374  mdash" type="QSt
-000035d0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-000035e0: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
-000035f0: 6c75 653d 2233 783a 302c 302c 302c 302c  lue="3x:0,0,0,0,
-00003600: 302c 3022 206e 616d 653d 2263 7573 746f  0,0" name="custo
-00003610: 6d64 6173 685f 6d61 705f 756e 6974 5f73  mdash_map_unit_s
-00003620: 6361 6c65 2220 7479 7065 3d22 5153 7472  cale" type="QStr
-00003630: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-00003640: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00003650: 7565 3d22 4d4d 2220 6e61 6d65 3d22 6375  ue="MM" name="cu
-00003660: 7374 6f6d 6461 7368 5f75 6e69 7422 2074  stomdash_unit" t
-00003670: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
-00003680: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
-00003690: 7074 696f 6e20 7661 6c75 653d 2230 2220  ption value="0" 
-000036a0: 6e61 6d65 3d22 6461 7368 5f70 6174 7465  name="dash_patte
-000036b0: 726e 5f6f 6666 7365 7422 2074 7970 653d  rn_offset" type=
-000036c0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-000036d0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-000036e0: 6e20 7661 6c75 653d 2233 783a 302c 302c  n value="3x:0,0,
-000036f0: 302c 302c 302c 3022 206e 616d 653d 2264  0,0,0,0" name="d
-00003700: 6173 685f 7061 7474 6572 6e5f 6f66 6673  ash_pattern_offs
-00003710: 6574 5f6d 6170 5f75 6e69 745f 7363 616c  et_map_unit_scal
-00003720: 6522 2074 7970 653d 2251 5374 7269 6e67  e" type="QString
-00003730: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00003740: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
-00003750: 224d 4d22 206e 616d 653d 2264 6173 685f  "MM" name="dash_
-00003760: 7061 7474 6572 6e5f 6f66 6673 6574 5f75  pattern_offset_u
-00003770: 6e69 7422 2074 7970 653d 2251 5374 7269  nit" type="QStri
-00003780: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
-00003790: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-000037a0: 653d 2230 2220 6e61 6d65 3d22 6472 6177  e="0" name="draw
-000037b0: 5f69 6e73 6964 655f 706f 6c79 676f 6e22  _inside_polygon"
-000037c0: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-000037d0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000037e0: 3c4f 7074 696f 6e20 7661 6c75 653d 2262  <Option value="b
-000037f0: 6576 656c 2220 6e61 6d65 3d22 6a6f 696e  evel" name="join
-00003800: 7374 796c 6522 2074 7970 653d 2251 5374  style" type="QSt
-00003810: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-00003820: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
-00003830: 6c75 653d 2233 352c 3335 2c33 352c 3235  lue="35,35,35,25
-00003840: 3522 206e 616d 653d 226c 696e 655f 636f  5" name="line_co
-00003850: 6c6f 7222 2074 7970 653d 2251 5374 7269  lor" type="QStri
-00003860: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
-00003870: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-00003880: 653d 2273 6f6c 6964 2220 6e61 6d65 3d22  e="solid" name="
-00003890: 6c69 6e65 5f73 7479 6c65 2220 7479 7065  line_style" type
-000038a0: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-000038b0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-000038c0: 6f6e 2076 616c 7565 3d22 302e 3236 2220  on value="0.26" 
-000038d0: 6e61 6d65 3d22 6c69 6e65 5f77 6964 7468  name="line_width
-000038e0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-000038f0: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
-00003900: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-00003910: 4d4d 2220 6e61 6d65 3d22 6c69 6e65 5f77  MM" name="line_w
-00003920: 6964 7468 5f75 6e69 7422 2074 7970 653d  idth_unit" type=
-00003930: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-00003940: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00003950: 6e20 7661 6c75 653d 2230 2220 6e61 6d65  n value="0" name
-00003960: 3d22 6f66 6673 6574 2220 7479 7065 3d22  ="offset" type="
-00003970: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-00003980: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-00003990: 2076 616c 7565 3d22 3378 3a30 2c30 2c30   value="3x:0,0,0
-000039a0: 2c30 2c30 2c30 2220 6e61 6d65 3d22 6f66  ,0,0,0" name="of
-000039b0: 6673 6574 5f6d 6170 5f75 6e69 745f 7363  fset_map_unit_sc
-000039c0: 616c 6522 2074 7970 653d 2251 5374 7269  ale" type="QStri
-000039d0: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
-000039e0: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-000039f0: 653d 224d 4d22 206e 616d 653d 226f 6666  e="MM" name="off
-00003a00: 7365 745f 756e 6974 2220 7479 7065 3d22  set_unit" type="
-00003a10: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-00003a20: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-00003a30: 2076 616c 7565 3d22 3022 206e 616d 653d   value="0" name=
-00003a40: 2272 696e 675f 6669 6c74 6572 2220 7479  "ring_filter" ty
-00003a50: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
-00003a60: 2020 2020 2020 2020 2020 2020 203c 4f70               <Op
-00003a70: 7469 6f6e 2076 616c 7565 3d22 3022 206e  tion value="0" n
-00003a80: 616d 653d 2274 7269 6d5f 6469 7374 616e  ame="trim_distan
-00003a90: 6365 5f65 6e64 2220 7479 7065 3d22 5153  ce_end" type="QS
-00003aa0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00003ab0: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-00003ac0: 616c 7565 3d22 3378 3a30 2c30 2c30 2c30  alue="3x:0,0,0,0
-00003ad0: 2c30 2c30 2220 6e61 6d65 3d22 7472 696d  ,0,0" name="trim
-00003ae0: 5f64 6973 7461 6e63 655f 656e 645f 6d61  _distance_end_ma
-00003af0: 705f 756e 6974 5f73 6361 6c65 2220 7479  p_unit_scale" ty
-00003b00: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
-00003b10: 2020 2020 2020 2020 2020 2020 203c 4f70               <Op
-00003b20: 7469 6f6e 2076 616c 7565 3d22 4d4d 2220  tion value="MM" 
-00003b30: 6e61 6d65 3d22 7472 696d 5f64 6973 7461  name="trim_dista
-00003b40: 6e63 655f 656e 645f 756e 6974 2220 7479  nce_end_unit" ty
-00003b50: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
-00003b60: 2020 2020 2020 2020 2020 2020 203c 4f70               <Op
-00003b70: 7469 6f6e 2076 616c 7565 3d22 3022 206e  tion value="0" n
-00003b80: 616d 653d 2274 7269 6d5f 6469 7374 616e  ame="trim_distan
-00003b90: 6365 5f73 7461 7274 2220 7479 7065 3d22  ce_start" type="
-00003ba0: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-00003bb0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-00003bc0: 2076 616c 7565 3d22 3378 3a30 2c30 2c30   value="3x:0,0,0
-00003bd0: 2c30 2c30 2c30 2220 6e61 6d65 3d22 7472  ,0,0,0" name="tr
-00003be0: 696d 5f64 6973 7461 6e63 655f 7374 6172  im_distance_star
-00003bf0: 745f 6d61 705f 756e 6974 5f73 6361 6c65  t_map_unit_scale
-00003c00: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00003c10: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
-00003c20: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-00003c30: 4d4d 2220 6e61 6d65 3d22 7472 696d 5f64  MM" name="trim_d
-00003c40: 6973 7461 6e63 655f 7374 6172 745f 756e  istance_start_un
-00003c50: 6974 2220 7479 7065 3d22 5153 7472 696e  it" type="QStrin
-00003c60: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
-00003c70: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
-00003c80: 3d22 3022 206e 616d 653d 2274 7765 616b  ="0" name="tweak
-00003c90: 5f64 6173 685f 7061 7474 6572 6e5f 6f6e  _dash_pattern_on
-00003ca0: 5f63 6f72 6e65 7273 2220 7479 7065 3d22  _corners" type="
-00003cb0: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-00003cc0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-00003cd0: 2076 616c 7565 3d22 3022 206e 616d 653d   value="0" name=
-00003ce0: 2275 7365 5f63 7573 746f 6d5f 6461 7368  "use_custom_dash
-00003cf0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00003d00: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
-00003d10: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-00003d20: 3378 3a30 2c30 2c30 2c30 2c30 2c30 2220  3x:0,0,0,0,0,0" 
-00003d30: 6e61 6d65 3d22 7769 6474 685f 6d61 705f  name="width_map_
-00003d40: 756e 6974 5f73 6361 6c65 2220 7479 7065  unit_scale" type
-00003d50: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-00003d60: 2020 2020 2020 2020 203c 2f4f 7074 696f           </Optio
-00003d70: 6e3e 0a20 2020 2020 2020 2020 2020 203c  n>.            <
-00003d80: 6461 7461 5f64 6566 696e 6564 5f70 726f  data_defined_pro
-00003d90: 7065 7274 6965 733e 0a20 2020 2020 2020  perties>.       
-00003da0: 2020 2020 2020 203c 4f70 7469 6f6e 2074         <Option t
-00003db0: 7970 653d 224d 6170 223e 0a20 2020 2020  ype="Map">.     
-00003dc0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00003dd0: 6f6e 2076 616c 7565 3d22 2220 6e61 6d65  on value="" name
-00003de0: 3d22 6e61 6d65 2220 7479 7065 3d22 5153  ="name" type="QS
-00003df0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00003e00: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-00003e10: 206e 616d 653d 2270 726f 7065 7274 6965   name="propertie
-00003e20: 7322 2f3e 0a20 2020 2020 2020 2020 2020  s"/>.           
-00003e30: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00003e40: 7565 3d22 636f 6c6c 6563 7469 6f6e 2220  ue="collection" 
-00003e50: 6e61 6d65 3d22 7479 7065 2220 7479 7065  name="type" type
-00003e60: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-00003e70: 2020 2020 2020 2020 2020 203c 2f4f 7074             </Opt
-00003e80: 696f 6e3e 0a20 2020 2020 2020 2020 2020  ion>.           
-00003e90: 203c 2f64 6174 615f 6465 6669 6e65 645f   </data_defined_
-00003ea0: 7072 6f70 6572 7469 6573 3e0a 2020 2020  properties>.    
-00003eb0: 2020 2020 2020 3c2f 6c61 7965 723e 0a20        </layer>. 
-00003ec0: 2020 2020 2020 203c 2f73 796d 626f 6c3e         </symbol>
-00003ed0: 0a20 2020 2020 203c 2f61 7869 7353 796d  .      </axisSym
-00003ee0: 626f 6c3e 0a20 2020 203c 2f44 6961 6772  bol>.    </Diagr
-00003ef0: 616d 4361 7465 676f 7279 3e0a 2020 3c2f  amCategory>.  </
-00003f00: 5369 6e67 6c65 4361 7465 676f 7279 4469  SingleCategoryDi
-00003f10: 6167 7261 6d52 656e 6465 7265 723e 0a20  agramRenderer>. 
-00003f20: 203c 4469 6167 7261 6d4c 6179 6572 5365   <DiagramLayerSe
-00003f30: 7474 696e 6773 207a 496e 6465 783d 2230  ttings zIndex="0
-00003f40: 2220 7368 6f77 416c 6c3d 2231 2220 706c  " showAll="1" pl
-00003f50: 6163 656d 656e 743d 2230 2220 6c69 6e65  acement="0" line
-00003f60: 506c 6163 656d 656e 7446 6c61 6773 3d22  PlacementFlags="
-00003f70: 3138 2220 6f62 7374 6163 6c65 3d22 3022  18" obstacle="0"
-00003f80: 2064 6973 743d 2230 2220 7072 696f 7269   dist="0" priori
-00003f90: 7479 3d22 3022 3e0a 2020 2020 3c70 726f  ty="0">.    <pro
-00003fa0: 7065 7274 6965 733e 0a20 2020 2020 203c  perties>.      <
-00003fb0: 4f70 7469 6f6e 2074 7970 653d 224d 6170  Option type="Map
-00003fc0: 223e 0a20 2020 2020 2020 203c 4f70 7469  ">.        <Opti
-00003fd0: 6f6e 2076 616c 7565 3d22 2220 6e61 6d65  on value="" name
-00003fe0: 3d22 6e61 6d65 2220 7479 7065 3d22 5153  ="name" type="QS
-00003ff0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00004000: 203c 4f70 7469 6f6e 206e 616d 653d 2270   <Option name="p
-00004010: 726f 7065 7274 6965 7322 2f3e 0a20 2020  roperties"/>.   
-00004020: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00004030: 7565 3d22 636f 6c6c 6563 7469 6f6e 2220  ue="collection" 
-00004040: 6e61 6d65 3d22 7479 7065 2220 7479 7065  name="type" type
-00004050: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-00004060: 2020 203c 2f4f 7074 696f 6e3e 0a20 2020     </Option>.   
-00004070: 203c 2f70 726f 7065 7274 6965 733e 0a20   </properties>. 
-00004080: 203c 2f44 6961 6772 616d 4c61 7965 7253   </DiagramLayerS
-00004090: 6574 7469 6e67 733e 0a20 203c 6765 6f6d  ettings>.  <geom
-000040a0: 6574 7279 4f70 7469 6f6e 7320 7265 6d6f  etryOptions remo
-000040b0: 7665 4475 706c 6963 6174 654e 6f64 6573  veDuplicateNodes
-000040c0: 3d22 3022 2067 656f 6d65 7472 7950 7265  ="0" geometryPre
-000040d0: 6369 7369 6f6e 3d22 3022 3e0a 2020 2020  cision="0">.    
-000040e0: 3c61 6374 6976 6543 6865 636b 732f 3e0a  <activeChecks/>.
-000040f0: 2020 2020 3c63 6865 636b 436f 6e66 6967      <checkConfig
-00004100: 7572 6174 696f 6e2f 3e0a 2020 3c2f 6765  uration/>.  </ge
-00004110: 6f6d 6574 7279 4f70 7469 6f6e 733e 0a20  ometryOptions>. 
-00004120: 203c 6c65 6765 6e64 2073 686f 774c 6162   <legend showLab
-00004130: 656c 4c65 6765 6e64 3d22 3022 2074 7970  elLegend="0" typ
-00004140: 653d 2264 6566 6175 6c74 2d76 6563 746f  e="default-vecto
-00004150: 7222 2f3e 0a20 203c 7265 6665 7265 6e63  r"/>.  <referenc
-00004160: 6564 4c61 7965 7273 2f3e 0a20 203c 6669  edLayers/>.  <fi
-00004170: 656c 6443 6f6e 6669 6775 7261 7469 6f6e  eldConfiguration
-00004180: 3e0a 2020 2020 3c66 6965 6c64 206e 616d  >.    <field nam
-00004190: 653d 2274 7970 6522 2063 6f6e 6669 6775  e="type" configu
-000041a0: 7261 7469 6f6e 466c 6167 733d 224e 6f6e  rationFlags="Non
-000041b0: 6522 3e0a 2020 2020 2020 3c65 6469 7457  e">.      <editW
-000041c0: 6964 6765 7420 7479 7065 3d22 5465 7874  idget type="Text
-000041d0: 4564 6974 223e 0a20 2020 2020 2020 203c  Edit">.        <
-000041e0: 636f 6e66 6967 3e0a 2020 2020 2020 2020  config>.        
-000041f0: 2020 3c4f 7074 696f 6e2f 3e0a 2020 2020    <Option/>.    
-00004200: 2020 2020 3c2f 636f 6e66 6967 3e0a 2020      </config>.  
-00004210: 2020 2020 3c2f 6564 6974 5769 6467 6574      </editWidget
-00004220: 3e0a 2020 2020 3c2f 6669 656c 643e 0a20  >.    </field>. 
-00004230: 2020 203c 6669 656c 6420 6e61 6d65 3d22     <field name="
-00004240: 6f73 6d5f 6964 2220 636f 6e66 6967 7572  osm_id" configur
-00004250: 6174 696f 6e46 6c61 6773 3d22 4e6f 6e65  ationFlags="None
-00004260: 223e 0a20 2020 2020 203c 6564 6974 5769  ">.      <editWi
-00004270: 6467 6574 2074 7970 653d 2254 6578 7445  dget type="TextE
-00004280: 6469 7422 3e0a 2020 2020 2020 2020 3c63  dit">.        <c
-00004290: 6f6e 6669 673e 0a20 2020 2020 2020 2020  onfig>.         
-000042a0: 203c 4f70 7469 6f6e 2f3e 0a20 2020 2020   <Option/>.     
-000042b0: 2020 203c 2f63 6f6e 6669 673e 0a20 2020     </config>.   
-000042c0: 2020 203c 2f65 6469 7457 6964 6765 743e     </editWidget>
-000042d0: 0a20 2020 203c 2f66 6965 6c64 3e0a 2020  .    </field>.  
-000042e0: 2020 3c66 6965 6c64 206e 616d 653d 226f    <field name="o
-000042f0: 7269 656e 7461 7469 6f6e 2220 636f 6e66  rientation" conf
-00004300: 6967 7572 6174 696f 6e46 6c61 6773 3d22  igurationFlags="
-00004310: 4e6f 6e65 223e 0a20 2020 2020 203c 6564  None">.      <ed
-00004320: 6974 5769 6467 6574 2074 7970 653d 2254  itWidget type="T
-00004330: 6578 7445 6469 7422 3e0a 2020 2020 2020  extEdit">.      
-00004340: 2020 3c63 6f6e 6669 673e 0a20 2020 2020    <config>.     
-00004350: 2020 2020 203c 4f70 7469 6f6e 2f3e 0a20       <Option/>. 
-00004360: 2020 2020 2020 203c 2f63 6f6e 6669 673e         </config>
-00004370: 0a20 2020 2020 203c 2f65 6469 7457 6964  .      </editWid
-00004380: 6765 743e 0a20 2020 203c 2f66 6965 6c64  get>.    </field
-00004390: 3e0a 2020 2020 3c66 6965 6c64 206e 616d  >.    <field nam
-000043a0: 653d 226f 7269 656e 7461 7469 6f6e 5f63  e="orientation_c
-000043b0: 6f6e 6669 6465 6e63 6522 2063 6f6e 6669  onfidence" confi
-000043c0: 6775 7261 7469 6f6e 466c 6167 733d 224e  gurationFlags="N
-000043d0: 6f6e 6522 3e0a 2020 2020 2020 3c65 6469  one">.      <edi
-000043e0: 7457 6964 6765 7420 7479 7065 3d22 5465  tWidget type="Te
-000043f0: 7874 4564 6974 223e 0a20 2020 2020 2020  xtEdit">.       
-00004400: 203c 636f 6e66 6967 3e0a 2020 2020 2020   <config>.      
-00004410: 2020 2020 3c4f 7074 696f 6e2f 3e0a 2020      <Option/>.  
-00004420: 2020 2020 2020 3c2f 636f 6e66 6967 3e0a        </config>.
-00004430: 2020 2020 2020 3c2f 6564 6974 5769 6467        </editWidg
-00004440: 6574 3e0a 2020 2020 3c2f 6669 656c 643e  et>.    </field>
-00004450: 0a20 2020 203c 6669 656c 6420 6e61 6d65  .    <field name
-00004460: 3d22 6c61 6e65 5f77 6964 7468 2220 636f  ="lane_width" co
-00004470: 6e66 6967 7572 6174 696f 6e46 6c61 6773  nfigurationFlags
-00004480: 3d22 4e6f 6e65 223e 0a20 2020 2020 203c  ="None">.      <
-00004490: 6564 6974 5769 6467 6574 2074 7970 653d  editWidget type=
-000044a0: 2254 6578 7445 6469 7422 3e0a 2020 2020  "TextEdit">.    
-000044b0: 2020 2020 3c63 6f6e 6669 673e 0a20 2020      <config>.   
-000044c0: 2020 2020 2020 203c 4f70 7469 6f6e 2f3e         <Option/>
-000044d0: 0a20 2020 2020 2020 203c 2f63 6f6e 6669  .        </confi
-000044e0: 673e 0a20 2020 2020 203c 2f65 6469 7457  g>.      </editW
-000044f0: 6964 6765 743e 0a20 2020 203c 2f66 6965  idget>.    </fie
-00004500: 6c64 3e0a 2020 2020 3c66 6965 6c64 206e  ld>.    <field n
-00004510: 616d 653d 226c 616e 655f 6f72 6965 6e74  ame="lane_orient
-00004520: 6174 696f 6e22 2063 6f6e 6669 6775 7261  ation" configura
-00004530: 7469 6f6e 466c 6167 733d 224e 6f6e 6522  tionFlags="None"
-00004540: 3e0a 2020 2020 2020 3c65 6469 7457 6964  >.      <editWid
-00004550: 6765 7420 7479 7065 3d22 5465 7874 4564  get type="TextEd
-00004560: 6974 223e 0a20 2020 2020 2020 203c 636f  it">.        <co
-00004570: 6e66 6967 3e0a 2020 2020 2020 2020 2020  nfig>.          
-00004580: 3c4f 7074 696f 6e2f 3e0a 2020 2020 2020  <Option/>.      
-00004590: 2020 3c2f 636f 6e66 6967 3e0a 2020 2020    </config>.    
-000045a0: 2020 3c2f 6564 6974 5769 6467 6574 3e0a    </editWidget>.
-000045b0: 2020 2020 3c2f 6669 656c 643e 0a20 203c      </field>.  <
-000045c0: 2f66 6965 6c64 436f 6e66 6967 7572 6174  /fieldConfigurat
-000045d0: 696f 6e3e 0a20 203c 616c 6961 7365 733e  ion>.  <aliases>
-000045e0: 0a20 2020 203c 616c 6961 7320 6e61 6d65  .    <alias name
-000045f0: 3d22 2220 696e 6465 783d 2230 2220 6669  ="" index="0" fi
-00004600: 656c 643d 2274 7970 6522 2f3e 0a20 2020  eld="type"/>.   
-00004610: 203c 616c 6961 7320 6e61 6d65 3d22 2220   <alias name="" 
-00004620: 696e 6465 783d 2231 2220 6669 656c 643d  index="1" field=
-00004630: 226f 736d 5f69 6422 2f3e 0a20 2020 203c  "osm_id"/>.    <
-00004640: 616c 6961 7320 6e61 6d65 3d22 2220 696e  alias name="" in
-00004650: 6465 783d 2232 2220 6669 656c 643d 226f  dex="2" field="o
-00004660: 7269 656e 7461 7469 6f6e 222f 3e0a 2020  rientation"/>.  
-00004670: 2020 3c61 6c69 6173 206e 616d 653d 2222    <alias name=""
-00004680: 2069 6e64 6578 3d22 3322 2066 6965 6c64   index="3" field
-00004690: 3d22 6f72 6965 6e74 6174 696f 6e5f 636f  ="orientation_co
-000046a0: 6e66 6964 656e 6365 222f 3e0a 2020 2020  nfidence"/>.    
-000046b0: 3c61 6c69 6173 206e 616d 653d 2222 2069  <alias name="" i
-000046c0: 6e64 6578 3d22 3422 2066 6965 6c64 3d22  ndex="4" field="
-000046d0: 6c61 6e65 5f77 6964 7468 222f 3e0a 2020  lane_width"/>.  
-000046e0: 2020 3c61 6c69 6173 206e 616d 653d 2222    <alias name=""
-000046f0: 2069 6e64 6578 3d22 3522 2066 6965 6c64   index="5" field
-00004700: 3d22 6c61 6e65 5f6f 7269 656e 7461 7469  ="lane_orientati
-00004710: 6f6e 222f 3e0a 2020 3c2f 616c 6961 7365  on"/>.  </aliase
-00004720: 733e 0a20 203c 6465 6661 756c 7473 3e0a  s>.  <defaults>.
-00004730: 2020 2020 3c64 6566 6175 6c74 2066 6965      <default fie
-00004740: 6c64 3d22 7479 7065 2220 6578 7072 6573  ld="type" expres
-00004750: 7369 6f6e 3d22 2220 6170 706c 794f 6e55  sion="" applyOnU
-00004760: 7064 6174 653d 2230 222f 3e0a 2020 2020  pdate="0"/>.    
-00004770: 3c64 6566 6175 6c74 2066 6965 6c64 3d22  <default field="
-00004780: 6f73 6d5f 6964 2220 6578 7072 6573 7369  osm_id" expressi
-00004790: 6f6e 3d22 2220 6170 706c 794f 6e55 7064  on="" applyOnUpd
-000047a0: 6174 653d 2230 222f 3e0a 2020 2020 3c64  ate="0"/>.    <d
-000047b0: 6566 6175 6c74 2066 6965 6c64 3d22 6f72  efault field="or
-000047c0: 6965 6e74 6174 696f 6e22 2065 7870 7265  ientation" expre
-000047d0: 7373 696f 6e3d 2222 2061 7070 6c79 4f6e  ssion="" applyOn
-000047e0: 5570 6461 7465 3d22 3022 2f3e 0a20 2020  Update="0"/>.   
-000047f0: 203c 6465 6661 756c 7420 6669 656c 643d   <default field=
-00004800: 226f 7269 656e 7461 7469 6f6e 5f63 6f6e  "orientation_con
-00004810: 6669 6465 6e63 6522 2065 7870 7265 7373  fidence" express
-00004820: 696f 6e3d 2222 2061 7070 6c79 4f6e 5570  ion="" applyOnUp
-00004830: 6461 7465 3d22 3022 2f3e 0a20 2020 203c  date="0"/>.    <
-00004840: 6465 6661 756c 7420 6669 656c 643d 226c  default field="l
-00004850: 616e 655f 7769 6474 6822 2065 7870 7265  ane_width" expre
-00004860: 7373 696f 6e3d 2222 2061 7070 6c79 4f6e  ssion="" applyOn
-00004870: 5570 6461 7465 3d22 3022 2f3e 0a20 2020  Update="0"/>.   
-00004880: 203c 6465 6661 756c 7420 6669 656c 643d   <default field=
-00004890: 226c 616e 655f 6f72 6965 6e74 6174 696f  "lane_orientatio
-000048a0: 6e22 2065 7870 7265 7373 696f 6e3d 2222  n" expression=""
-000048b0: 2061 7070 6c79 4f6e 5570 6461 7465 3d22   applyOnUpdate="
-000048c0: 3022 2f3e 0a20 203c 2f64 6566 6175 6c74  0"/>.  </default
-000048d0: 733e 0a20 203c 636f 6e73 7472 6169 6e74  s>.  <constraint
-000048e0: 733e 0a20 2020 203c 636f 6e73 7472 6169  s>.    <constrai
-000048f0: 6e74 2075 6e69 7175 655f 7374 7265 6e67  nt unique_streng
-00004900: 7468 3d22 3022 206e 6f74 6e75 6c6c 5f73  th="0" notnull_s
-00004910: 7472 656e 6774 683d 2230 2220 6578 705f  trength="0" exp_
-00004920: 7374 7265 6e67 7468 3d22 3022 2066 6965  strength="0" fie
-00004930: 6c64 3d22 7479 7065 2220 636f 6e73 7472  ld="type" constr
-00004940: 6169 6e74 733d 2230 222f 3e0a 2020 2020  aints="0"/>.    
-00004950: 3c63 6f6e 7374 7261 696e 7420 756e 6971  <constraint uniq
-00004960: 7565 5f73 7472 656e 6774 683d 2230 2220  ue_strength="0" 
-00004970: 6e6f 746e 756c 6c5f 7374 7265 6e67 7468  notnull_strength
-00004980: 3d22 3022 2065 7870 5f73 7472 656e 6774  ="0" exp_strengt
-00004990: 683d 2230 2220 6669 656c 643d 226f 736d  h="0" field="osm
-000049a0: 5f69 6422 2063 6f6e 7374 7261 696e 7473  _id" constraints
-000049b0: 3d22 3022 2f3e 0a20 2020 203c 636f 6e73  ="0"/>.    <cons
-000049c0: 7472 6169 6e74 2075 6e69 7175 655f 7374  traint unique_st
-000049d0: 7265 6e67 7468 3d22 3022 206e 6f74 6e75  rength="0" notnu
-000049e0: 6c6c 5f73 7472 656e 6774 683d 2230 2220  ll_strength="0" 
-000049f0: 6578 705f 7374 7265 6e67 7468 3d22 3022  exp_strength="0"
-00004a00: 2066 6965 6c64 3d22 6f72 6965 6e74 6174   field="orientat
-00004a10: 696f 6e22 2063 6f6e 7374 7261 696e 7473  ion" constraints
-00004a20: 3d22 3022 2f3e 0a20 2020 203c 636f 6e73  ="0"/>.    <cons
-00004a30: 7472 6169 6e74 2075 6e69 7175 655f 7374  traint unique_st
-00004a40: 7265 6e67 7468 3d22 3022 206e 6f74 6e75  rength="0" notnu
-00004a50: 6c6c 5f73 7472 656e 6774 683d 2230 2220  ll_strength="0" 
-00004a60: 6578 705f 7374 7265 6e67 7468 3d22 3022  exp_strength="0"
-00004a70: 2066 6965 6c64 3d22 6f72 6965 6e74 6174   field="orientat
-00004a80: 696f 6e5f 636f 6e66 6964 656e 6365 2220  ion_confidence" 
-00004a90: 636f 6e73 7472 6169 6e74 733d 2230 222f  constraints="0"/
-00004aa0: 3e0a 2020 2020 3c63 6f6e 7374 7261 696e  >.    <constrain
-00004ab0: 7420 756e 6971 7565 5f73 7472 656e 6774  t unique_strengt
-00004ac0: 683d 2230 2220 6e6f 746e 756c 6c5f 7374  h="0" notnull_st
-00004ad0: 7265 6e67 7468 3d22 3022 2065 7870 5f73  rength="0" exp_s
-00004ae0: 7472 656e 6774 683d 2230 2220 6669 656c  trength="0" fiel
-00004af0: 643d 226c 616e 655f 7769 6474 6822 2063  d="lane_width" c
-00004b00: 6f6e 7374 7261 696e 7473 3d22 3022 2f3e  onstraints="0"/>
-00004b10: 0a20 2020 203c 636f 6e73 7472 6169 6e74  .    <constraint
-00004b20: 2075 6e69 7175 655f 7374 7265 6e67 7468   unique_strength
-00004b30: 3d22 3022 206e 6f74 6e75 6c6c 5f73 7472  ="0" notnull_str
-00004b40: 656e 6774 683d 2230 2220 6578 705f 7374  ength="0" exp_st
-00004b50: 7265 6e67 7468 3d22 3022 2066 6965 6c64  rength="0" field
-00004b60: 3d22 6c61 6e65 5f6f 7269 656e 7461 7469  ="lane_orientati
-00004b70: 6f6e 2220 636f 6e73 7472 6169 6e74 733d  on" constraints=
-00004b80: 2230 222f 3e0a 2020 3c2f 636f 6e73 7472  "0"/>.  </constr
-00004b90: 6169 6e74 733e 0a20 203c 636f 6e73 7472  aints>.  <constr
-00004ba0: 6169 6e74 4578 7072 6573 7369 6f6e 733e  aintExpressions>
-00004bb0: 0a20 2020 203c 636f 6e73 7472 6169 6e74  .    <constraint
-00004bc0: 2064 6573 633d 2222 2065 7870 3d22 2220   desc="" exp="" 
-00004bd0: 6669 656c 643d 2274 7970 6522 2f3e 0a20  field="type"/>. 
-00004be0: 2020 203c 636f 6e73 7472 6169 6e74 2064     <constraint d
-00004bf0: 6573 633d 2222 2065 7870 3d22 2220 6669  esc="" exp="" fi
-00004c00: 656c 643d 226f 736d 5f69 6422 2f3e 0a20  eld="osm_id"/>. 
-00004c10: 2020 203c 636f 6e73 7472 6169 6e74 2064     <constraint d
-00004c20: 6573 633d 2222 2065 7870 3d22 2220 6669  esc="" exp="" fi
-00004c30: 656c 643d 226f 7269 656e 7461 7469 6f6e  eld="orientation
-00004c40: 222f 3e0a 2020 2020 3c63 6f6e 7374 7261  "/>.    <constra
-00004c50: 696e 7420 6465 7363 3d22 2220 6578 703d  int desc="" exp=
-00004c60: 2222 2066 6965 6c64 3d22 6f72 6965 6e74  "" field="orient
-00004c70: 6174 696f 6e5f 636f 6e66 6964 656e 6365  ation_confidence
-00004c80: 222f 3e0a 2020 2020 3c63 6f6e 7374 7261  "/>.    <constra
-00004c90: 696e 7420 6465 7363 3d22 2220 6578 703d  int desc="" exp=
-00004ca0: 2222 2066 6965 6c64 3d22 6c61 6e65 5f77  "" field="lane_w
-00004cb0: 6964 7468 222f 3e0a 2020 2020 3c63 6f6e  idth"/>.    <con
-00004cc0: 7374 7261 696e 7420 6465 7363 3d22 2220  straint desc="" 
-00004cd0: 6578 703d 2222 2066 6965 6c64 3d22 6c61  exp="" field="la
-00004ce0: 6e65 5f6f 7269 656e 7461 7469 6f6e 222f  ne_orientation"/
-00004cf0: 3e0a 2020 3c2f 636f 6e73 7472 6169 6e74  >.  </constraint
-00004d00: 4578 7072 6573 7369 6f6e 733e 0a20 203c  Expressions>.  <
-00004d10: 6578 7072 6573 7369 6f6e 6669 656c 6473  expressionfields
-00004d20: 2f3e 0a20 203c 6174 7472 6962 7574 6561  />.  <attributea
-00004d30: 6374 696f 6e73 3e0a 2020 2020 3c64 6566  ctions>.    <def
-00004d40: 6175 6c74 4163 7469 6f6e 2076 616c 7565  aultAction value
-00004d50: 3d22 7b30 3030 3030 3030 302d 3030 3030  ="{00000000-0000
-00004d60: 2d30 3030 302d 3030 3030 2d30 3030 3030  -0000-0000-00000
-00004d70: 3030 3030 3030 307d 2220 6b65 793d 2243  0000000}" key="C
-00004d80: 616e 7661 7322 2f3e 0a20 203c 2f61 7474  anvas"/>.  </att
-00004d90: 7269 6275 7465 6163 7469 6f6e 733e 0a20  ributeactions>. 
-00004da0: 203c 6174 7472 6962 7574 6574 6162 6c65   <attributetable
-00004db0: 636f 6e66 6967 2061 6374 696f 6e57 6964  config actionWid
-00004dc0: 6765 7453 7479 6c65 3d22 6472 6f70 446f  getStyle="dropDo
-00004dd0: 776e 2220 736f 7274 4f72 6465 723d 2230  wn" sortOrder="0
-00004de0: 2220 736f 7274 4578 7072 6573 7369 6f6e  " sortExpression
-00004df0: 3d22 223e 0a20 2020 203c 636f 6c75 6d6e  ="">.    <column
-00004e00: 733e 0a20 2020 2020 203c 636f 6c75 6d6e  s>.      <column
-00004e10: 206e 616d 653d 2274 7970 6522 2077 6964   name="type" wid
-00004e20: 7468 3d22 2d31 2220 6869 6464 656e 3d22  th="-1" hidden="
-00004e30: 3022 2074 7970 653d 2266 6965 6c64 222f  0" type="field"/
-00004e40: 3e0a 2020 2020 2020 3c63 6f6c 756d 6e20  >.      <column 
-00004e50: 6e61 6d65 3d22 6f73 6d5f 6964 2220 7769  name="osm_id" wi
-00004e60: 6474 683d 2231 3731 2220 6869 6464 656e  dth="171" hidden
-00004e70: 3d22 3022 2074 7970 653d 2266 6965 6c64  ="0" type="field
-00004e80: 222f 3e0a 2020 2020 2020 3c63 6f6c 756d  "/>.      <colum
-00004e90: 6e20 6e61 6d65 3d22 6f72 6965 6e74 6174  n name="orientat
-00004ea0: 696f 6e22 2077 6964 7468 3d22 3239 3222  ion" width="292"
-00004eb0: 2068 6964 6465 6e3d 2230 2220 7479 7065   hidden="0" type
-00004ec0: 3d22 6669 656c 6422 2f3e 0a20 2020 2020  ="field"/>.     
-00004ed0: 203c 636f 6c75 6d6e 206e 616d 653d 226f   <column name="o
-00004ee0: 7269 656e 7461 7469 6f6e 5f63 6f6e 6669  rientation_confi
-00004ef0: 6465 6e63 6522 2077 6964 7468 3d22 2d31  dence" width="-1
-00004f00: 2220 6869 6464 656e 3d22 3022 2074 7970  " hidden="0" typ
-00004f10: 653d 2266 6965 6c64 222f 3e0a 2020 2020  e="field"/>.    
-00004f20: 2020 3c63 6f6c 756d 6e20 6e61 6d65 3d22    <column name="
-00004f30: 6c61 6e65 5f6f 7269 656e 7461 7469 6f6e  lane_orientation
-00004f40: 2220 7769 6474 683d 222d 3122 2068 6964  " width="-1" hid
-00004f50: 6465 6e3d 2230 2220 7479 7065 3d22 6669  den="0" type="fi
-00004f60: 656c 6422 2f3e 0a20 2020 2020 203c 636f  eld"/>.      <co
-00004f70: 6c75 6d6e 206e 616d 653d 226c 616e 655f  lumn name="lane_
-00004f80: 7769 6474 6822 2077 6964 7468 3d22 2d31  width" width="-1
-00004f90: 2220 6869 6464 656e 3d22 3022 2074 7970  " hidden="0" typ
-00004fa0: 653d 2266 6965 6c64 222f 3e0a 2020 2020  e="field"/>.    
-00004fb0: 2020 3c63 6f6c 756d 6e20 7769 6474 683d    <column width=
-00004fc0: 222d 3122 2068 6964 6465 6e3d 2231 2220  "-1" hidden="1" 
-00004fd0: 7479 7065 3d22 6163 7469 6f6e 7322 2f3e  type="actions"/>
-00004fe0: 0a20 2020 203c 2f63 6f6c 756d 6e73 3e0a  .    </columns>.
-00004ff0: 2020 3c2f 6174 7472 6962 7574 6574 6162    </attributetab
-00005000: 6c65 636f 6e66 6967 3e0a 2020 3c63 6f6e  leconfig>.  <con
-00005010: 6469 7469 6f6e 616c 7374 796c 6573 3e0a  ditionalstyles>.
-00005020: 2020 2020 3c72 6f77 7374 796c 6573 2f3e      <rowstyles/>
-00005030: 0a20 2020 203c 6669 656c 6473 7479 6c65  .    <fieldstyle
-00005040: 732f 3e0a 2020 3c2f 636f 6e64 6974 696f  s/>.  </conditio
-00005050: 6e61 6c73 7479 6c65 733e 0a20 203c 7374  nalstyles>.  <st
-00005060: 6f72 6564 6578 7072 6573 7369 6f6e 732f  oredexpressions/
-00005070: 3e0a 2020 3c65 6469 7466 6f72 6d20 746f  >.  <editform to
-00005080: 6c65 7261 6e74 3d22 3122 3e3c 2f65 6469  lerant="1"></edi
-00005090: 7466 6f72 6d3e 0a20 203c 6564 6974 666f  tform>.  <editfo
-000050a0: 726d 696e 6974 2f3e 0a20 203c 6564 6974  rminit/>.  <edit
-000050b0: 666f 726d 696e 6974 636f 6465 736f 7572  forminitcodesour
-000050c0: 6365 3e30 3c2f 6564 6974 666f 726d 696e  ce>0</editformin
-000050d0: 6974 636f 6465 736f 7572 6365 3e0a 2020  itcodesource>.  
-000050e0: 3c65 6469 7466 6f72 6d69 6e69 7466 696c  <editforminitfil
-000050f0: 6570 6174 683e 3c2f 6564 6974 666f 726d  epath></editform
-00005100: 696e 6974 6669 6c65 7061 7468 3e0a 2020  initfilepath>.  
-00005110: 3c65 6469 7466 6f72 6d69 6e69 7463 6f64  <editforminitcod
-00005120: 653e 3c21 5b43 4441 5441 5b23 202d 2a2d  e><![CDATA[# -*-
-00005130: 2063 6f64 696e 673a 2075 7466 2d38 202d   coding: utf-8 -
-00005140: 2a2d 0a22 2222 0a4c 6573 2066 6f72 6d75  *-.""".Les formu
-00005150: 6c61 6972 6573 2051 4749 5320 7065 7576  laires QGIS peuv
-00005160: 656e 7420 6176 6f69 7220 756e 6520 666f  ent avoir une fo
-00005170: 6e63 7469 6f6e 2050 7974 686f 6e20 7175  nction Python qu
-00005180: 6920 6573 7420 6170 7065 6cc3 a965 206c  i est appel..e l
-00005190: 6f72 7371 7565 206c 6520 666f 726d 756c  orsque le formul
-000051a0: 6169 7265 2065 7374 0a6f 7576 6572 742e  aire est.ouvert.
-000051b0: 0a0a 5574 696c 6973 657a 2063 6574 7465  ..Utilisez cette
-000051c0: 2066 6f6e 6374 696f 6e20 706f 7572 2061   fonction pour a
-000051d0: 6a6f 7574 6572 2075 6e65 206c 6f67 6971  jouter une logiq
-000051e0: 7565 2073 7570 706c c3a9 6d65 6e74 6169  ue suppl..mentai
-000051f0: 7265 20c3 a020 766f 7320 666f 726d 756c  re .. vos formul
-00005200: 6169 7265 732e 0a0a 456e 7472 657a 206c  aires...Entrez l
-00005210: 6520 6e6f 6d20 6465 206c 6120 666f 6e63  e nom de la fonc
-00005220: 7469 6f6e 2064 616e 7320 6c65 2063 6861  tion dans le cha
-00005230: 6d70 200a 2246 6f6e 6374 696f 6e20 6427  mp ."Fonction d'
-00005240: 696e 6974 6961 6c69 7361 7469 6f6e 2050  initialisation P
-00005250: 7974 686f 6e22 2e0a 566f 6963 6920 756e  ython"..Voici un
-00005260: 2065 7865 6d70 6c65 3a0a 2222 220a 6672   exemple:.""".fr
-00005270: 6f6d 2071 6769 732e 5079 5174 2e51 7457  om qgis.PyQt.QtW
-00005280: 6964 6765 7473 2069 6d70 6f72 7420 5157  idgets import QW
-00005290: 6964 6765 740a 0a64 6566 206d 795f 666f  idget..def my_fo
-000052a0: 726d 5f6f 7065 6e28 6469 616c 6f67 2c20  rm_open(dialog, 
-000052b0: 6c61 7965 722c 2066 6561 7475 7265 293a  layer, feature):
-000052c0: 0a20 2020 2067 656f 6d20 3d20 6665 6174  .    geom = feat
-000052d0: 7572 652e 6765 6f6d 6574 7279 2829 0a20  ure.geometry(). 
-000052e0: 2020 2063 6f6e 7472 6f6c 203d 2064 6961     control = dia
-000052f0: 6c6f 672e 6669 6e64 4368 696c 6428 5157  log.findChild(QW
-00005300: 6964 6765 742c 2022 4d79 4c69 6e65 4564  idget, "MyLineEd
-00005310: 6974 2229 0a5d 5d3e 3c2f 6564 6974 666f  it").]]></editfo
-00005320: 726d 696e 6974 636f 6465 3e0a 2020 3c66  rminitcode>.  <f
-00005330: 6561 7466 6f72 6d73 7570 7072 6573 733e  eatformsuppress>
-00005340: 303c 2f66 6561 7466 6f72 6d73 7570 7072  0</featformsuppr
-00005350: 6573 733e 0a20 203c 6564 6974 6f72 6c61  ess>.  <editorla
-00005360: 796f 7574 3e67 656e 6572 6174 6564 6c61  yout>generatedla
-00005370: 796f 7574 3c2f 6564 6974 6f72 6c61 796f  yout</editorlayo
-00005380: 7574 3e0a 2020 3c65 6469 7461 626c 653e  ut>.  <editable>
-00005390: 0a20 2020 203c 6669 656c 6420 6e61 6d65  .    <field name
-000053a0: 3d22 616e 676c 6522 2065 6469 7461 626c  ="angle" editabl
-000053b0: 653d 2231 222f 3e0a 2020 2020 3c66 6965  e="1"/>.    <fie
-000053c0: 6c64 206e 616d 653d 2266 6964 2220 6564  ld name="fid" ed
-000053d0: 6974 6162 6c65 3d22 3122 2f3e 0a20 2020  itable="1"/>.   
-000053e0: 203c 6669 656c 6420 6e61 6d65 3d22 6c61   <field name="la
-000053f0: 6e65 5f6f 7269 656e 7461 7469 6f6e 2220  ne_orientation" 
-00005400: 6564 6974 6162 6c65 3d22 3122 2f3e 0a20  editable="1"/>. 
-00005410: 2020 203c 6669 656c 6420 6e61 6d65 3d22     <field name="
-00005420: 6c61 6e65 5f77 6964 7468 2220 6564 6974  lane_width" edit
-00005430: 6162 6c65 3d22 3122 2f3e 0a20 2020 203c  able="1"/>.    <
-00005440: 6669 656c 6420 6e61 6d65 3d22 6f72 6965  field name="orie
-00005450: 6e74 6174 696f 6e22 2065 6469 7461 626c  ntation" editabl
-00005460: 653d 2231 222f 3e0a 2020 2020 3c66 6965  e="1"/>.    <fie
-00005470: 6c64 206e 616d 653d 226f 7269 656e 7461  ld name="orienta
-00005480: 7469 6f6e 5f63 6f6e 6669 6465 6e63 6522  tion_confidence"
-00005490: 2065 6469 7461 626c 653d 2231 222f 3e0a   editable="1"/>.
-000054a0: 2020 2020 3c66 6965 6c64 206e 616d 653d      <field name=
-000054b0: 226f 736d 5f69 6422 2065 6469 7461 626c  "osm_id" editabl
-000054c0: 653d 2231 222f 3e0a 2020 2020 3c66 6965  e="1"/>.    <fie
-000054d0: 6c64 206e 616d 653d 2274 7970 6522 2065  ld name="type" e
-000054e0: 6469 7461 626c 653d 2231 222f 3e0a 2020  ditable="1"/>.  
-000054f0: 3c2f 6564 6974 6162 6c65 3e0a 2020 3c6c  </editable>.  <l
-00005500: 6162 656c 4f6e 546f 703e 0a20 2020 203c  abelOnTop>.    <
-00005510: 6669 656c 6420 6e61 6d65 3d22 616e 676c  field name="angl
-00005520: 6522 206c 6162 656c 4f6e 546f 703d 2230  e" labelOnTop="0
-00005530: 222f 3e0a 2020 2020 3c66 6965 6c64 206e  "/>.    <field n
-00005540: 616d 653d 2266 6964 2220 6c61 6265 6c4f  ame="fid" labelO
-00005550: 6e54 6f70 3d22 3022 2f3e 0a20 2020 203c  nTop="0"/>.    <
-00005560: 6669 656c 6420 6e61 6d65 3d22 6c61 6e65  field name="lane
-00005570: 5f6f 7269 656e 7461 7469 6f6e 2220 6c61  _orientation" la
-00005580: 6265 6c4f 6e54 6f70 3d22 3022 2f3e 0a20  belOnTop="0"/>. 
-00005590: 2020 203c 6669 656c 6420 6e61 6d65 3d22     <field name="
-000055a0: 6c61 6e65 5f77 6964 7468 2220 6c61 6265  lane_width" labe
-000055b0: 6c4f 6e54 6f70 3d22 3022 2f3e 0a20 2020  lOnTop="0"/>.   
-000055c0: 203c 6669 656c 6420 6e61 6d65 3d22 6f72   <field name="or
-000055d0: 6965 6e74 6174 696f 6e22 206c 6162 656c  ientation" label
-000055e0: 4f6e 546f 703d 2230 222f 3e0a 2020 2020  OnTop="0"/>.    
-000055f0: 3c66 6965 6c64 206e 616d 653d 226f 7269  <field name="ori
-00005600: 656e 7461 7469 6f6e 5f63 6f6e 6669 6465  entation_confide
-00005610: 6e63 6522 206c 6162 656c 4f6e 546f 703d  nce" labelOnTop=
-00005620: 2230 222f 3e0a 2020 2020 3c66 6965 6c64  "0"/>.    <field
-00005630: 206e 616d 653d 226f 736d 5f69 6422 206c   name="osm_id" l
-00005640: 6162 656c 4f6e 546f 703d 2230 222f 3e0a  abelOnTop="0"/>.
-00005650: 2020 2020 3c66 6965 6c64 206e 616d 653d      <field name=
-00005660: 2274 7970 6522 206c 6162 656c 4f6e 546f  "type" labelOnTo
-00005670: 703d 2230 222f 3e0a 2020 3c2f 6c61 6265  p="0"/>.  </labe
-00005680: 6c4f 6e54 6f70 3e0a 2020 3c72 6575 7365  lOnTop>.  <reuse
-00005690: 4c61 7374 5661 6c75 653e 0a20 2020 203c  LastValue>.    <
-000056a0: 6669 656c 6420 6e61 6d65 3d22 616e 676c  field name="angl
-000056b0: 6522 2072 6575 7365 4c61 7374 5661 6c75  e" reuseLastValu
-000056c0: 653d 2230 222f 3e0a 2020 2020 3c66 6965  e="0"/>.    <fie
-000056d0: 6c64 206e 616d 653d 2266 6964 2220 7265  ld name="fid" re
-000056e0: 7573 654c 6173 7456 616c 7565 3d22 3022  useLastValue="0"
-000056f0: 2f3e 0a20 2020 203c 6669 656c 6420 6e61  />.    <field na
-00005700: 6d65 3d22 6c61 6e65 5f6f 7269 656e 7461  me="lane_orienta
-00005710: 7469 6f6e 2220 7265 7573 654c 6173 7456  tion" reuseLastV
-00005720: 616c 7565 3d22 3022 2f3e 0a20 2020 203c  alue="0"/>.    <
-00005730: 6669 656c 6420 6e61 6d65 3d22 6c61 6e65  field name="lane
-00005740: 5f77 6964 7468 2220 7265 7573 654c 6173  _width" reuseLas
-00005750: 7456 616c 7565 3d22 3022 2f3e 0a20 2020  tValue="0"/>.   
-00005760: 203c 6669 656c 6420 6e61 6d65 3d22 6f72   <field name="or
-00005770: 6965 6e74 6174 696f 6e22 2072 6575 7365  ientation" reuse
-00005780: 4c61 7374 5661 6c75 653d 2230 222f 3e0a  LastValue="0"/>.
-00005790: 2020 2020 3c66 6965 6c64 206e 616d 653d      <field name=
-000057a0: 226f 7269 656e 7461 7469 6f6e 5f63 6f6e  "orientation_con
-000057b0: 6669 6465 6e63 6522 2072 6575 7365 4c61  fidence" reuseLa
-000057c0: 7374 5661 6c75 653d 2230 222f 3e0a 2020  stValue="0"/>.  
-000057d0: 2020 3c66 6965 6c64 206e 616d 653d 226f    <field name="o
-000057e0: 736d 5f69 6422 2072 6575 7365 4c61 7374  sm_id" reuseLast
-000057f0: 5661 6c75 653d 2230 222f 3e0a 2020 2020  Value="0"/>.    
-00005800: 3c66 6965 6c64 206e 616d 653d 2274 7970  <field name="typ
-00005810: 6522 2072 6575 7365 4c61 7374 5661 6c75  e" reuseLastValu
-00005820: 653d 2230 222f 3e0a 2020 3c2f 7265 7573  e="0"/>.  </reus
-00005830: 654c 6173 7456 616c 7565 3e0a 2020 3c64  eLastValue>.  <d
-00005840: 6174 6144 6566 696e 6564 4669 656c 6450  ataDefinedFieldP
-00005850: 726f 7065 7274 6965 732f 3e0a 2020 3c77  roperties/>.  <w
-00005860: 6964 6765 7473 2f3e 0a20 203c 7072 6576  idgets/>.  <prev
-00005870: 6965 7745 7870 7265 7373 696f 6e3e 2274  iewExpression>"t
-00005880: 7970 6522 3c2f 7072 6576 6965 7745 7870  ype"</previewExp
-00005890: 7265 7373 696f 6e3e 0a20 203c 6d61 7054  ression>.  <mapT
-000058a0: 6970 3e3c 2f6d 6170 5469 703e 0a20 203c  ip></mapTip>.  <
-000058b0: 6c61 7965 7247 656f 6d65 7472 7954 7970  layerGeometryTyp
-000058c0: 653e 303c 2f6c 6179 6572 4765 6f6d 6574  e>0</layerGeomet
-000058d0: 7279 5479 7065 3e0a 3c2f 7167 6973 3e0a  ryType>.</qgis>.
+00002a00: 7661 6c75 653d 2239 3020 2b20 282d 2671  value="90 + (-&q
+00002a10: 756f 743b 6f72 6965 6e74 6174 696f 6e26  uot;orientation&
+00002a20: 7175 6f74 3b20 2f20 7069 2829 2920 2a20  quot; / pi()) * 
+00002a30: 3138 3022 206e 616d 653d 2265 7870 7265  180" name="expre
+00002a40: 7373 696f 6e22 2074 7970 653d 2251 5374  ssion" type="QSt
+00002a50: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+00002a60: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00002a70: 6e20 7661 6c75 653d 2233 2220 6e61 6d65  n value="3" name
+00002a80: 3d22 7479 7065 2220 7479 7065 3d22 696e  ="type" type="in
+00002a90: 7422 2f3e 0a20 2020 2020 2020 2020 2020  t"/>.           
+00002aa0: 2020 2020 203c 2f4f 7074 696f 6e3e 0a20       </Option>. 
+00002ab0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00002ac0: 4f70 7469 6f6e 206e 616d 653d 226f 7574  Option name="out
+00002ad0: 6c69 6e65 5769 6474 6822 2074 7970 653d  lineWidth" type=
+00002ae0: 224d 6170 223e 0a20 2020 2020 2020 2020  "Map">.         
+00002af0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00002b00: 2076 616c 7565 3d22 7472 7565 2220 6e61   value="true" na
+00002b10: 6d65 3d22 6163 7469 7665 2220 7479 7065  me="active" type
+00002b20: 3d22 626f 6f6c 222f 3e0a 2020 2020 2020  ="bool"/>.      
+00002b30: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00002b40: 696f 6e20 7661 6c75 653d 2226 7175 6f74  ion value="&quot
+00002b50: 3b6c 616e 655f 7769 6474 6826 7175 6f74  ;lane_width&quot
+00002b60: 3b20 2a20 312e 3322 206e 616d 653d 2265  ; * 1.3" name="e
+00002b70: 7870 7265 7373 696f 6e22 2074 7970 653d  xpression" type=
+00002b80: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00002b90: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
+00002ba0: 7074 696f 6e20 7661 6c75 653d 2233 2220  ption value="3" 
+00002bb0: 6e61 6d65 3d22 7479 7065 2220 7479 7065  name="type" type
+00002bc0: 3d22 696e 7422 2f3e c2b2 0a20 2020 2020  ="int"/>...     
+00002bd0: 2020 2020 2020 2020 2020 203c 2f4f 7074             </Opt
+00002be0: 696f 6e3e 0a20 2020 2020 2020 2020 2020  ion>.           
+00002bf0: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
+00002c00: 653d 2273 697a 6522 2074 7970 653d 224d  e="size" type="M
+00002c10: 6170 223e 0a20 2020 2020 2020 2020 2020  ap">.           
+00002c20: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
+00002c30: 616c 7565 3d22 7472 7565 2220 6e61 6d65  alue="true" name
+00002c40: 3d22 6163 7469 7665 2220 7479 7065 3d22  ="active" type="
+00002c50: 626f 6f6c 222f 3e0a 2020 2020 2020 2020  bool"/>.        
+00002c60: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00002c70: 6e20 7661 6c75 653d 2233 202b 2032 202a  n value="3 + 2 *
+00002c80: 2030 2e30 3032 202a 2020 406d 6170 5f73   0.002 *  @map_s
+00002c90: 6361 6c65 2220 6e61 6d65 3d22 6578 7072  cale" name="expr
+00002ca0: 6573 7369 6f6e 2220 7479 7065 3d22 5153  ession" type="QS
+00002cb0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+00002cc0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00002cd0: 6f6e 2076 616c 7565 3d22 3322 206e 616d  on value="3" nam
+00002ce0: 653d 2274 7970 6522 2074 7970 653d 2269  e="type" type="i
+00002cf0: 6e74 222f 3e0a 2020 2020 2020 2020 2020  nt"/>.          
+00002d00: 2020 2020 2020 3c2f 4f70 7469 6f6e 3e0a        </Option>.
+00002d10: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00002d20: 4f70 7469 6f6e 3e0a 2020 2020 2020 2020  Option>.        
+00002d30: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
+00002d40: 6c75 653d 2263 6f6c 6c65 6374 696f 6e22  lue="collection"
+00002d50: 206e 616d 653d 2274 7970 6522 2074 7970   name="type" typ
+00002d60: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00002d70: 2020 2020 2020 2020 2020 3c2f 4f70 7469            </Opti
+00002d80: 6f6e 3e0a 2020 2020 2020 2020 2020 3c2f  on>.          </
+00002d90: 6461 7461 5f64 6566 696e 6564 5f70 726f  data_defined_pro
+00002da0: 7065 7274 6965 733e 0a20 2020 2020 2020  perties>.       
+00002db0: 203c 2f6c 6179 6572 3e0a 2020 2020 2020   </layer>.      
+00002dc0: 3c2f 7379 6d62 6f6c 3e0a 2020 2020 3c2f  </symbol>.    </
+00002dd0: 7379 6d62 6f6c 733e 0a20 203c 2f72 656e  symbols>.  </ren
+00002de0: 6465 7265 722d 7632 3e0a 2020 3c63 7573  derer-v2>.  <cus
+00002df0: 746f 6d70 726f 7065 7274 6965 733e 0a20  tomproperties>. 
+00002e00: 2020 203c 4f70 7469 6f6e 2074 7970 653d     <Option type=
+00002e10: 224d 6170 223e 0a20 2020 2020 203c 4f70  "Map">.      <Op
+00002e20: 7469 6f6e 206e 616d 653d 2264 7561 6c76  tion name="dualv
+00002e30: 6965 772f 7072 6576 6965 7745 7870 7265  iew/previewExpre
+00002e40: 7373 696f 6e73 2220 7479 7065 3d22 4c69  ssions" type="Li
+00002e50: 7374 223e 0a20 2020 2020 2020 203c 4f70  st">.        <Op
+00002e60: 7469 6f6e 2076 616c 7565 3d22 2671 756f  tion value="&quo
+00002e70: 743b 7479 7065 2671 756f 743b 2220 7479  t;type&quot;" ty
+00002e80: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+00002e90: 2020 2020 203c 2f4f 7074 696f 6e3e 0a20       </Option>. 
+00002ea0: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
+00002eb0: 7565 3d22 3022 206e 616d 653d 2265 6d62  ue="0" name="emb
+00002ec0: 6564 6465 6457 6964 6765 7473 2f63 6f75  eddedWidgets/cou
+00002ed0: 6e74 2220 7479 7065 3d22 696e 7422 2f3e  nt" type="int"/>
+00002ee0: 0a20 2020 2020 203c 4f70 7469 6f6e 206e  .      <Option n
+00002ef0: 616d 653d 2276 6172 6961 626c 654e 616d  ame="variableNam
+00002f00: 6573 222f 3e0a 2020 2020 2020 3c4f 7074  es"/>.      <Opt
+00002f10: 696f 6e20 6e61 6d65 3d22 7661 7269 6162  ion name="variab
+00002f20: 6c65 5661 6c75 6573 222f 3e0a 2020 2020  leValues"/>.    
+00002f30: 3c2f 4f70 7469 6f6e 3e0a 2020 3c2f 6375  </Option>.  </cu
+00002f40: 7374 6f6d 7072 6f70 6572 7469 6573 3e0a  stomproperties>.
+00002f50: 2020 3c62 6c65 6e64 4d6f 6465 3e30 3c2f    <blendMode>0</
+00002f60: 626c 656e 644d 6f64 653e 0a20 203c 6665  blendMode>.  <fe
+00002f70: 6174 7572 6542 6c65 6e64 4d6f 6465 3e30  atureBlendMode>0
+00002f80: 3c2f 6665 6174 7572 6542 6c65 6e64 4d6f  </featureBlendMo
+00002f90: 6465 3e0a 2020 3c6c 6179 6572 4f70 6163  de>.  <layerOpac
+00002fa0: 6974 793e 313c 2f6c 6179 6572 4f70 6163  ity>1</layerOpac
+00002fb0: 6974 793e 0a20 203c 5369 6e67 6c65 4361  ity>.  <SingleCa
+00002fc0: 7465 676f 7279 4469 6167 7261 6d52 656e  tegoryDiagramRen
+00002fd0: 6465 7265 7220 6469 6167 7261 6d54 7970  derer diagramTyp
+00002fe0: 653d 2248 6973 746f 6772 616d 2220 6174  e="Histogram" at
+00002ff0: 7472 6962 7574 654c 6567 656e 643d 2231  tributeLegend="1
+00003000: 223e 0a20 2020 203c 4469 6167 7261 6d43  ">.    <DiagramC
+00003010: 6174 6567 6f72 7920 7065 6e43 6f6c 6f72  ategory penColor
+00003020: 3d22 2330 3030 3030 3022 2070 656e 5769  ="#000000" penWi
+00003030: 6474 683d 2230 2220 7769 6474 683d 2231  dth="0" width="1
+00003040: 3522 2073 697a 6554 7970 653d 224d 4d22  5" sizeType="MM"
+00003050: 2064 6972 6563 7469 6f6e 3d22 3022 206c   direction="0" l
+00003060: 6162 656c 506c 6163 656d 656e 744d 6574  abelPlacementMet
+00003070: 686f 643d 2258 4865 6967 6874 2220 656e  hod="XHeight" en
+00003080: 6162 6c65 643d 2230 2220 6261 7257 6964  abled="0" barWid
+00003090: 7468 3d22 3522 206d 6178 5363 616c 6544  th="5" maxScaleD
+000030a0: 656e 6f6d 696e 6174 6f72 3d22 3165 2b30  enominator="1e+0
+000030b0: 3822 2073 7061 6369 6e67 556e 6974 5363  8" spacingUnitSc
+000030c0: 616c 653d 2233 783a 302c 302c 302c 302c  ale="3x:0,0,0,0,
+000030d0: 302c 3022 206f 7061 6369 7479 3d22 3122  0,0" opacity="1"
+000030e0: 2073 6361 6c65 4465 7065 6e64 656e 6379   scaleDependency
+000030f0: 3d22 4172 6561 2220 6261 636b 6772 6f75  ="Area" backgrou
+00003100: 6e64 416c 7068 613d 2232 3535 2220 6d69  ndAlpha="255" mi
+00003110: 6e53 6361 6c65 4465 6e6f 6d69 6e61 746f  nScaleDenominato
+00003120: 723d 2230 2220 7370 6163 696e 6755 6e69  r="0" spacingUni
+00003130: 743d 224d 4d22 206d 696e 696d 756d 5369  t="MM" minimumSi
+00003140: 7a65 3d22 3022 2062 6163 6b67 726f 756e  ze="0" backgroun
+00003150: 6443 6f6c 6f72 3d22 2366 6666 6666 6622  dColor="#ffffff"
+00003160: 206c 696e 6553 697a 6554 7970 653d 224d   lineSizeType="M
+00003170: 4d22 206c 696e 6553 697a 6553 6361 6c65  M" lineSizeScale
+00003180: 3d22 3378 3a30 2c30 2c30 2c30 2c30 2c30  ="3x:0,0,0,0,0,0
+00003190: 2220 7369 7a65 5363 616c 653d 2233 783a  " sizeScale="3x:
+000031a0: 302c 302c 302c 302c 302c 3022 2073 6361  0,0,0,0,0,0" sca
+000031b0: 6c65 4261 7365 6456 6973 6962 696c 6974  leBasedVisibilit
+000031c0: 793d 2230 2220 7370 6163 696e 673d 2235  y="0" spacing="5
+000031d0: 2220 726f 7461 7469 6f6e 4f66 6673 6574  " rotationOffset
+000031e0: 3d22 3237 3022 2068 6569 6768 743d 2231  ="270" height="1
+000031f0: 3522 2073 686f 7741 7869 733d 2231 2220  5" showAxis="1" 
+00003200: 6469 6167 7261 6d4f 7269 656e 7461 7469  diagramOrientati
+00003210: 6f6e 3d22 5570 2220 7065 6e41 6c70 6861  on="Up" penAlpha
+00003220: 3d22 3235 3522 3e0a 2020 2020 2020 3c66  ="255">.      <f
+00003230: 6f6e 7450 726f 7065 7274 6965 7320 626f  ontProperties bo
+00003240: 6c64 3d22 3022 2073 7472 696b 6574 6872  ld="0" strikethr
+00003250: 6f75 6768 3d22 3022 2073 7479 6c65 3d22  ough="0" style="
+00003260: 2220 756e 6465 726c 696e 653d 2230 2220  " underline="0" 
+00003270: 6465 7363 7269 7074 696f 6e3d 224e 6f74  description="Not
+00003280: 6f20 5361 6e73 2c31 302c 2d31 2c30 2c35  o Sans,10,-1,0,5
+00003290: 302c 302c 302c 302c 302c 3022 2069 7461  0,0,0,0,0,0" ita
+000032a0: 6c69 633d 2230 222f 3e0a 2020 2020 2020  lic="0"/>.      
+000032b0: 3c61 7474 7269 6275 7465 2063 6f6c 6f72  <attribute color
+000032c0: 4f70 6163 6974 793d 2231 2220 636f 6c6f  Opacity="1" colo
+000032d0: 723d 2223 3030 3030 3030 2220 6669 656c  r="#000000" fiel
+000032e0: 643d 2222 206c 6162 656c 3d22 222f 3e0a  d="" label=""/>.
+000032f0: 2020 2020 2020 3c61 7869 7353 796d 626f        <axisSymbo
+00003300: 6c3e 0a20 2020 2020 2020 203c 7379 6d62  l>.        <symb
+00003310: 6f6c 2066 7261 6d65 5f72 6174 653d 2231  ol frame_rate="1
+00003320: 3022 206e 616d 653d 2222 2061 6c70 6861  0" name="" alpha
+00003330: 3d22 3122 2069 735f 616e 696d 6174 6564  ="1" is_animated
+00003340: 3d22 3022 2063 6c69 705f 746f 5f65 7874  ="0" clip_to_ext
+00003350: 656e 743d 2231 2220 7479 7065 3d22 6c69  ent="1" type="li
+00003360: 6e65 2220 666f 7263 655f 7268 723d 2230  ne" force_rhr="0
+00003370: 223e 0a20 2020 2020 2020 2020 203c 6461  ">.          <da
+00003380: 7461 5f64 6566 696e 6564 5f70 726f 7065  ta_defined_prope
+00003390: 7274 6965 733e 0a20 2020 2020 2020 2020  rties>.         
+000033a0: 2020 203c 4f70 7469 6f6e 2074 7970 653d     <Option type=
+000033b0: 224d 6170 223e 0a20 2020 2020 2020 2020  "Map">.         
+000033c0: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
+000033d0: 7565 3d22 2220 6e61 6d65 3d22 6e61 6d65  ue="" name="name
+000033e0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+000033f0: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+00003400: 203c 4f70 7469 6f6e 206e 616d 653d 2270   <Option name="p
+00003410: 726f 7065 7274 6965 7322 2f3e 0a20 2020  roperties"/>.   
+00003420: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00003430: 6f6e 2076 616c 7565 3d22 636f 6c6c 6563  on value="collec
+00003440: 7469 6f6e 2220 6e61 6d65 3d22 7479 7065  tion" name="type
+00003450: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00003460: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
+00003470: 2f4f 7074 696f 6e3e 0a20 2020 2020 2020  /Option>.       
+00003480: 2020 203c 2f64 6174 615f 6465 6669 6e65     </data_define
+00003490: 645f 7072 6f70 6572 7469 6573 3e0a 2020  d_properties>.  
+000034a0: 2020 2020 2020 2020 3c6c 6179 6572 2063          <layer c
+000034b0: 6c61 7373 3d22 5369 6d70 6c65 4c69 6e65  lass="SimpleLine
+000034c0: 2220 7061 7373 3d22 3022 2065 6e61 626c  " pass="0" enabl
+000034d0: 6564 3d22 3122 206c 6f63 6b65 643d 2230  ed="1" locked="0
+000034e0: 223e 0a20 2020 2020 2020 2020 2020 203c  ">.            <
+000034f0: 4f70 7469 6f6e 2074 7970 653d 224d 6170  Option type="Map
+00003500: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00003510: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+00003520: 3022 206e 616d 653d 2261 6c69 676e 5f64  0" name="align_d
+00003530: 6173 685f 7061 7474 6572 6e22 2074 7970  ash_pattern" typ
+00003540: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00003550: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00003560: 696f 6e20 7661 6c75 653d 2273 7175 6172  ion value="squar
+00003570: 6522 206e 616d 653d 2263 6170 7374 796c  e" name="capstyl
+00003580: 6522 2074 7970 653d 2251 5374 7269 6e67  e" type="QString
+00003590: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+000035a0: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+000035b0: 2235 3b32 2220 6e61 6d65 3d22 6375 7374  "5;2" name="cust
+000035c0: 6f6d 6461 7368 2220 7479 7065 3d22 5153  omdash" type="QS
+000035d0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+000035e0: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
+000035f0: 616c 7565 3d22 3378 3a30 2c30 2c30 2c30  alue="3x:0,0,0,0
+00003600: 2c30 2c30 2220 6e61 6d65 3d22 6375 7374  ,0,0" name="cust
+00003610: 6f6d 6461 7368 5f6d 6170 5f75 6e69 745f  omdash_map_unit_
+00003620: 7363 616c 6522 2074 7970 653d 2251 5374  scale" type="QSt
+00003630: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+00003640: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
+00003650: 6c75 653d 224d 4d22 206e 616d 653d 2263  lue="MM" name="c
+00003660: 7573 746f 6d64 6173 685f 756e 6974 2220  ustomdash_unit" 
+00003670: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00003680: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+00003690: 4f70 7469 6f6e 2076 616c 7565 3d22 3022  Option value="0"
+000036a0: 206e 616d 653d 2264 6173 685f 7061 7474   name="dash_patt
+000036b0: 6572 6e5f 6f66 6673 6574 2220 7479 7065  ern_offset" type
+000036c0: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+000036d0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+000036e0: 6f6e 2076 616c 7565 3d22 3378 3a30 2c30  on value="3x:0,0
+000036f0: 2c30 2c30 2c30 2c30 2220 6e61 6d65 3d22  ,0,0,0,0" name="
+00003700: 6461 7368 5f70 6174 7465 726e 5f6f 6666  dash_pattern_off
+00003710: 7365 745f 6d61 705f 756e 6974 5f73 6361  set_map_unit_sca
+00003720: 6c65 2220 7479 7065 3d22 5153 7472 696e  le" type="QStrin
+00003730: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00003740: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
+00003750: 3d22 4d4d 2220 6e61 6d65 3d22 6461 7368  ="MM" name="dash
+00003760: 5f70 6174 7465 726e 5f6f 6666 7365 745f  _pattern_offset_
+00003770: 756e 6974 2220 7479 7065 3d22 5153 7472  unit" type="QStr
+00003780: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+00003790: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
+000037a0: 7565 3d22 3022 206e 616d 653d 2264 7261  ue="0" name="dra
+000037b0: 775f 696e 7369 6465 5f70 6f6c 7967 6f6e  w_inside_polygon
+000037c0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+000037d0: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+000037e0: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+000037f0: 6265 7665 6c22 206e 616d 653d 226a 6f69  bevel" name="joi
+00003800: 6e73 7479 6c65 2220 7479 7065 3d22 5153  nstyle" type="QS
+00003810: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+00003820: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
+00003830: 616c 7565 3d22 3335 2c33 352c 3335 2c32  alue="35,35,35,2
+00003840: 3535 2220 6e61 6d65 3d22 6c69 6e65 5f63  55" name="line_c
+00003850: 6f6c 6f72 2220 7479 7065 3d22 5153 7472  olor" type="QStr
+00003860: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+00003870: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
+00003880: 7565 3d22 736f 6c69 6422 206e 616d 653d  ue="solid" name=
+00003890: 226c 696e 655f 7374 796c 6522 2074 7970  "line_style" typ
+000038a0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+000038b0: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+000038c0: 696f 6e20 7661 6c75 653d 2230 2e32 3622  ion value="0.26"
+000038d0: 206e 616d 653d 226c 696e 655f 7769 6474   name="line_widt
+000038e0: 6822 2074 7970 653d 2251 5374 7269 6e67  h" type="QString
+000038f0: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00003900: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+00003910: 224d 4d22 206e 616d 653d 226c 696e 655f  "MM" name="line_
+00003920: 7769 6474 685f 756e 6974 2220 7479 7065  width_unit" type
+00003930: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+00003940: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00003950: 6f6e 2076 616c 7565 3d22 3022 206e 616d  on value="0" nam
+00003960: 653d 226f 6666 7365 7422 2074 7970 653d  e="offset" type=
+00003970: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00003980: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00003990: 6e20 7661 6c75 653d 2233 783a 302c 302c  n value="3x:0,0,
+000039a0: 302c 302c 302c 3022 206e 616d 653d 226f  0,0,0,0" name="o
+000039b0: 6666 7365 745f 6d61 705f 756e 6974 5f73  ffset_map_unit_s
+000039c0: 6361 6c65 2220 7479 7065 3d22 5153 7472  cale" type="QStr
+000039d0: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+000039e0: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
+000039f0: 7565 3d22 4d4d 2220 6e61 6d65 3d22 6f66  ue="MM" name="of
+00003a00: 6673 6574 5f75 6e69 7422 2074 7970 653d  fset_unit" type=
+00003a10: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00003a20: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00003a30: 6e20 7661 6c75 653d 2230 2220 6e61 6d65  n value="0" name
+00003a40: 3d22 7269 6e67 5f66 696c 7465 7222 2074  ="ring_filter" t
+00003a50: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
+00003a60: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
+00003a70: 7074 696f 6e20 7661 6c75 653d 2230 2220  ption value="0" 
+00003a80: 6e61 6d65 3d22 7472 696d 5f64 6973 7461  name="trim_dista
+00003a90: 6e63 655f 656e 6422 2074 7970 653d 2251  nce_end" type="Q
+00003aa0: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+00003ab0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00003ac0: 7661 6c75 653d 2233 783a 302c 302c 302c  value="3x:0,0,0,
+00003ad0: 302c 302c 3022 206e 616d 653d 2274 7269  0,0,0" name="tri
+00003ae0: 6d5f 6469 7374 616e 6365 5f65 6e64 5f6d  m_distance_end_m
+00003af0: 6170 5f75 6e69 745f 7363 616c 6522 2074  ap_unit_scale" t
+00003b00: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
+00003b10: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
+00003b20: 7074 696f 6e20 7661 6c75 653d 224d 4d22  ption value="MM"
+00003b30: 206e 616d 653d 2274 7269 6d5f 6469 7374   name="trim_dist
+00003b40: 616e 6365 5f65 6e64 5f75 6e69 7422 2074  ance_end_unit" t
+00003b50: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
+00003b60: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
+00003b70: 7074 696f 6e20 7661 6c75 653d 2230 2220  ption value="0" 
+00003b80: 6e61 6d65 3d22 7472 696d 5f64 6973 7461  name="trim_dista
+00003b90: 6e63 655f 7374 6172 7422 2074 7970 653d  nce_start" type=
+00003ba0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00003bb0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00003bc0: 6e20 7661 6c75 653d 2233 783a 302c 302c  n value="3x:0,0,
+00003bd0: 302c 302c 302c 3022 206e 616d 653d 2274  0,0,0,0" name="t
+00003be0: 7269 6d5f 6469 7374 616e 6365 5f73 7461  rim_distance_sta
+00003bf0: 7274 5f6d 6170 5f75 6e69 745f 7363 616c  rt_map_unit_scal
+00003c00: 6522 2074 7970 653d 2251 5374 7269 6e67  e" type="QString
+00003c10: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00003c20: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+00003c30: 224d 4d22 206e 616d 653d 2274 7269 6d5f  "MM" name="trim_
+00003c40: 6469 7374 616e 6365 5f73 7461 7274 5f75  distance_start_u
+00003c50: 6e69 7422 2074 7970 653d 2251 5374 7269  nit" type="QStri
+00003c60: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+00003c70: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
+00003c80: 653d 2230 2220 6e61 6d65 3d22 7477 6561  e="0" name="twea
+00003c90: 6b5f 6461 7368 5f70 6174 7465 726e 5f6f  k_dash_pattern_o
+00003ca0: 6e5f 636f 726e 6572 7322 2074 7970 653d  n_corners" type=
+00003cb0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00003cc0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00003cd0: 6e20 7661 6c75 653d 2230 2220 6e61 6d65  n value="0" name
+00003ce0: 3d22 7573 655f 6375 7374 6f6d 5f64 6173  ="use_custom_das
+00003cf0: 6822 2074 7970 653d 2251 5374 7269 6e67  h" type="QString
+00003d00: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00003d10: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+00003d20: 2233 783a 302c 302c 302c 302c 302c 3022  "3x:0,0,0,0,0,0"
+00003d30: 206e 616d 653d 2277 6964 7468 5f6d 6170   name="width_map
+00003d40: 5f75 6e69 745f 7363 616c 6522 2074 7970  _unit_scale" typ
+00003d50: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00003d60: 2020 2020 2020 2020 2020 3c2f 4f70 7469            </Opti
+00003d70: 6f6e 3e0a 2020 2020 2020 2020 2020 2020  on>.            
+00003d80: 3c64 6174 615f 6465 6669 6e65 645f 7072  <data_defined_pr
+00003d90: 6f70 6572 7469 6573 3e0a 2020 2020 2020  operties>.      
+00003da0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00003db0: 7479 7065 3d22 4d61 7022 3e0a 2020 2020  type="Map">.    
+00003dc0: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00003dd0: 696f 6e20 7661 6c75 653d 2222 206e 616d  ion value="" nam
+00003de0: 653d 226e 616d 6522 2074 7970 653d 2251  e="name" type="Q
+00003df0: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+00003e00: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00003e10: 6e20 6e61 6d65 3d22 7072 6f70 6572 7469  n name="properti
+00003e20: 6573 222f 3e0a 2020 2020 2020 2020 2020  es"/>.          
+00003e30: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
+00003e40: 6c75 653d 2263 6f6c 6c65 6374 696f 6e22  lue="collection"
+00003e50: 206e 616d 653d 2274 7970 6522 2074 7970   name="type" typ
+00003e60: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00003e70: 2020 2020 2020 2020 2020 2020 3c2f 4f70              </Op
+00003e80: 7469 6f6e 3e0a 2020 2020 2020 2020 2020  tion>.          
+00003e90: 2020 3c2f 6461 7461 5f64 6566 696e 6564    </data_defined
+00003ea0: 5f70 726f 7065 7274 6965 733e 0a20 2020  _properties>.   
+00003eb0: 2020 2020 2020 203c 2f6c 6179 6572 3e0a         </layer>.
+00003ec0: 2020 2020 2020 2020 3c2f 7379 6d62 6f6c          </symbol
+00003ed0: 3e0a 2020 2020 2020 3c2f 6178 6973 5379  >.      </axisSy
+00003ee0: 6d62 6f6c 3e0a 2020 2020 3c2f 4469 6167  mbol>.    </Diag
+00003ef0: 7261 6d43 6174 6567 6f72 793e 0a20 203c  ramCategory>.  <
+00003f00: 2f53 696e 676c 6543 6174 6567 6f72 7944  /SingleCategoryD
+00003f10: 6961 6772 616d 5265 6e64 6572 6572 3e0a  iagramRenderer>.
+00003f20: 2020 3c44 6961 6772 616d 4c61 7965 7253    <DiagramLayerS
+00003f30: 6574 7469 6e67 7320 7a49 6e64 6578 3d22  ettings zIndex="
+00003f40: 3022 2073 686f 7741 6c6c 3d22 3122 2070  0" showAll="1" p
+00003f50: 6c61 6365 6d65 6e74 3d22 3022 206c 696e  lacement="0" lin
+00003f60: 6550 6c61 6365 6d65 6e74 466c 6167 733d  ePlacementFlags=
+00003f70: 2231 3822 206f 6273 7461 636c 653d 2230  "18" obstacle="0
+00003f80: 2220 6469 7374 3d22 3022 2070 7269 6f72  " dist="0" prior
+00003f90: 6974 793d 2230 223e 0a20 2020 203c 7072  ity="0">.    <pr
+00003fa0: 6f70 6572 7469 6573 3e0a 2020 2020 2020  operties>.      
+00003fb0: 3c4f 7074 696f 6e20 7479 7065 3d22 4d61  <Option type="Ma
+00003fc0: 7022 3e0a 2020 2020 2020 2020 3c4f 7074  p">.        <Opt
+00003fd0: 696f 6e20 7661 6c75 653d 2222 206e 616d  ion value="" nam
+00003fe0: 653d 226e 616d 6522 2074 7970 653d 2251  e="name" type="Q
+00003ff0: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+00004000: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
+00004010: 7072 6f70 6572 7469 6573 222f 3e0a 2020  properties"/>.  
+00004020: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
+00004030: 6c75 653d 2263 6f6c 6c65 6374 696f 6e22  lue="collection"
+00004040: 206e 616d 653d 2274 7970 6522 2074 7970   name="type" typ
+00004050: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00004060: 2020 2020 3c2f 4f70 7469 6f6e 3e0a 2020      </Option>.  
+00004070: 2020 3c2f 7072 6f70 6572 7469 6573 3e0a    </properties>.
+00004080: 2020 3c2f 4469 6167 7261 6d4c 6179 6572    </DiagramLayer
+00004090: 5365 7474 696e 6773 3e0a 2020 3c67 656f  Settings>.  <geo
+000040a0: 6d65 7472 794f 7074 696f 6e73 2072 656d  metryOptions rem
+000040b0: 6f76 6544 7570 6c69 6361 7465 4e6f 6465  oveDuplicateNode
+000040c0: 733d 2230 2220 6765 6f6d 6574 7279 5072  s="0" geometryPr
+000040d0: 6563 6973 696f 6e3d 2230 223e 0a20 2020  ecision="0">.   
+000040e0: 203c 6163 7469 7665 4368 6563 6b73 2f3e   <activeChecks/>
+000040f0: 0a20 2020 203c 6368 6563 6b43 6f6e 6669  .    <checkConfi
+00004100: 6775 7261 7469 6f6e 2f3e 0a20 203c 2f67  guration/>.  </g
+00004110: 656f 6d65 7472 794f 7074 696f 6e73 3e0a  eometryOptions>.
+00004120: 2020 3c6c 6567 656e 6420 7368 6f77 4c61    <legend showLa
+00004130: 6265 6c4c 6567 656e 643d 2230 2220 7479  belLegend="0" ty
+00004140: 7065 3d22 6465 6661 756c 742d 7665 6374  pe="default-vect
+00004150: 6f72 222f 3e0a 2020 3c72 6566 6572 656e  or"/>.  <referen
+00004160: 6365 644c 6179 6572 732f 3e0a 2020 3c66  cedLayers/>.  <f
+00004170: 6965 6c64 436f 6e66 6967 7572 6174 696f  ieldConfiguratio
+00004180: 6e3e 0a20 2020 203c 6669 656c 6420 6e61  n>.    <field na
+00004190: 6d65 3d22 7479 7065 2220 636f 6e66 6967  me="type" config
+000041a0: 7572 6174 696f 6e46 6c61 6773 3d22 4e6f  urationFlags="No
+000041b0: 6e65 223e 0a20 2020 2020 203c 6564 6974  ne">.      <edit
+000041c0: 5769 6467 6574 2074 7970 653d 2254 6578  Widget type="Tex
+000041d0: 7445 6469 7422 3e0a 2020 2020 2020 2020  tEdit">.        
+000041e0: 3c63 6f6e 6669 673e 0a20 2020 2020 2020  <config>.       
+000041f0: 2020 203c 4f70 7469 6f6e 2f3e 0a20 2020     <Option/>.   
+00004200: 2020 2020 203c 2f63 6f6e 6669 673e 0a20       </config>. 
+00004210: 2020 2020 203c 2f65 6469 7457 6964 6765       </editWidge
+00004220: 743e 0a20 2020 203c 2f66 6965 6c64 3e0a  t>.    </field>.
+00004230: 2020 2020 3c66 6965 6c64 206e 616d 653d      <field name=
+00004240: 226f 736d 5f69 6422 2063 6f6e 6669 6775  "osm_id" configu
+00004250: 7261 7469 6f6e 466c 6167 733d 224e 6f6e  rationFlags="Non
+00004260: 6522 3e0a 2020 2020 2020 3c65 6469 7457  e">.      <editW
+00004270: 6964 6765 7420 7479 7065 3d22 5465 7874  idget type="Text
+00004280: 4564 6974 223e 0a20 2020 2020 2020 203c  Edit">.        <
+00004290: 636f 6e66 6967 3e0a 2020 2020 2020 2020  config>.        
+000042a0: 2020 3c4f 7074 696f 6e2f 3e0a 2020 2020    <Option/>.    
+000042b0: 2020 2020 3c2f 636f 6e66 6967 3e0a 2020      </config>.  
+000042c0: 2020 2020 3c2f 6564 6974 5769 6467 6574      </editWidget
+000042d0: 3e0a 2020 2020 3c2f 6669 656c 643e 0a20  >.    </field>. 
+000042e0: 2020 203c 6669 656c 6420 6e61 6d65 3d22     <field name="
+000042f0: 6f72 6965 6e74 6174 696f 6e22 2063 6f6e  orientation" con
+00004300: 6669 6775 7261 7469 6f6e 466c 6167 733d  figurationFlags=
+00004310: 224e 6f6e 6522 3e0a 2020 2020 2020 3c65  "None">.      <e
+00004320: 6469 7457 6964 6765 7420 7479 7065 3d22  ditWidget type="
+00004330: 5465 7874 4564 6974 223e 0a20 2020 2020  TextEdit">.     
+00004340: 2020 203c 636f 6e66 6967 3e0a 2020 2020     <config>.    
+00004350: 2020 2020 2020 3c4f 7074 696f 6e2f 3e0a        <Option/>.
+00004360: 2020 2020 2020 2020 3c2f 636f 6e66 6967          </config
+00004370: 3e0a 2020 2020 2020 3c2f 6564 6974 5769  >.      </editWi
+00004380: 6467 6574 3e0a 2020 2020 3c2f 6669 656c  dget>.    </fiel
+00004390: 643e 0a20 2020 203c 6669 656c 6420 6e61  d>.    <field na
+000043a0: 6d65 3d22 6f72 6965 6e74 6174 696f 6e5f  me="orientation_
+000043b0: 636f 6e66 6964 656e 6365 2220 636f 6e66  confidence" conf
+000043c0: 6967 7572 6174 696f 6e46 6c61 6773 3d22  igurationFlags="
+000043d0: 4e6f 6e65 223e 0a20 2020 2020 203c 6564  None">.      <ed
+000043e0: 6974 5769 6467 6574 2074 7970 653d 2254  itWidget type="T
+000043f0: 6578 7445 6469 7422 3e0a 2020 2020 2020  extEdit">.      
+00004400: 2020 3c63 6f6e 6669 673e 0a20 2020 2020    <config>.     
+00004410: 2020 2020 203c 4f70 7469 6f6e 2f3e 0a20       <Option/>. 
+00004420: 2020 2020 2020 203c 2f63 6f6e 6669 673e         </config>
+00004430: 0a20 2020 2020 203c 2f65 6469 7457 6964  .      </editWid
+00004440: 6765 743e 0a20 2020 203c 2f66 6965 6c64  get>.    </field
+00004450: 3e0a 2020 2020 3c66 6965 6c64 206e 616d  >.    <field nam
+00004460: 653d 226c 616e 655f 7769 6474 6822 2063  e="lane_width" c
+00004470: 6f6e 6669 6775 7261 7469 6f6e 466c 6167  onfigurationFlag
+00004480: 733d 224e 6f6e 6522 3e0a 2020 2020 2020  s="None">.      
+00004490: 3c65 6469 7457 6964 6765 7420 7479 7065  <editWidget type
+000044a0: 3d22 5465 7874 4564 6974 223e 0a20 2020  ="TextEdit">.   
+000044b0: 2020 2020 203c 636f 6e66 6967 3e0a 2020       <config>.  
+000044c0: 2020 2020 2020 2020 3c4f 7074 696f 6e2f          <Option/
+000044d0: 3e0a 2020 2020 2020 2020 3c2f 636f 6e66  >.        </conf
+000044e0: 6967 3e0a 2020 2020 2020 3c2f 6564 6974  ig>.      </edit
+000044f0: 5769 6467 6574 3e0a 2020 2020 3c2f 6669  Widget>.    </fi
+00004500: 656c 643e 0a20 2020 203c 6669 656c 6420  eld>.    <field 
+00004510: 6e61 6d65 3d22 6c61 6e65 5f6f 7269 656e  name="lane_orien
+00004520: 7461 7469 6f6e 2220 636f 6e66 6967 7572  tation" configur
+00004530: 6174 696f 6e46 6c61 6773 3d22 4e6f 6e65  ationFlags="None
+00004540: 223e 0a20 2020 2020 203c 6564 6974 5769  ">.      <editWi
+00004550: 6467 6574 2074 7970 653d 2254 6578 7445  dget type="TextE
+00004560: 6469 7422 3e0a 2020 2020 2020 2020 3c63  dit">.        <c
+00004570: 6f6e 6669 673e 0a20 2020 2020 2020 2020  onfig>.         
+00004580: 203c 4f70 7469 6f6e 2f3e 0a20 2020 2020   <Option/>.     
+00004590: 2020 203c 2f63 6f6e 6669 673e 0a20 2020     </config>.   
+000045a0: 2020 203c 2f65 6469 7457 6964 6765 743e     </editWidget>
+000045b0: 0a20 2020 203c 2f66 6965 6c64 3e0a 2020  .    </field>.  
+000045c0: 3c2f 6669 656c 6443 6f6e 6669 6775 7261  </fieldConfigura
+000045d0: 7469 6f6e 3e0a 2020 3c61 6c69 6173 6573  tion>.  <aliases
+000045e0: 3e0a 2020 2020 3c61 6c69 6173 206e 616d  >.    <alias nam
+000045f0: 653d 2222 2069 6e64 6578 3d22 3022 2066  e="" index="0" f
+00004600: 6965 6c64 3d22 7479 7065 222f 3e0a 2020  ield="type"/>.  
+00004610: 2020 3c61 6c69 6173 206e 616d 653d 2222    <alias name=""
+00004620: 2069 6e64 6578 3d22 3122 2066 6965 6c64   index="1" field
+00004630: 3d22 6f73 6d5f 6964 222f 3e0a 2020 2020  ="osm_id"/>.    
+00004640: 3c61 6c69 6173 206e 616d 653d 2222 2069  <alias name="" i
+00004650: 6e64 6578 3d22 3222 2066 6965 6c64 3d22  ndex="2" field="
+00004660: 6f72 6965 6e74 6174 696f 6e22 2f3e 0a20  orientation"/>. 
+00004670: 2020 203c 616c 6961 7320 6e61 6d65 3d22     <alias name="
+00004680: 2220 696e 6465 783d 2233 2220 6669 656c  " index="3" fiel
+00004690: 643d 226f 7269 656e 7461 7469 6f6e 5f63  d="orientation_c
+000046a0: 6f6e 6669 6465 6e63 6522 2f3e 0a20 2020  onfidence"/>.   
+000046b0: 203c 616c 6961 7320 6e61 6d65 3d22 2220   <alias name="" 
+000046c0: 696e 6465 783d 2234 2220 6669 656c 643d  index="4" field=
+000046d0: 226c 616e 655f 7769 6474 6822 2f3e 0a20  "lane_width"/>. 
+000046e0: 2020 203c 616c 6961 7320 6e61 6d65 3d22     <alias name="
+000046f0: 2220 696e 6465 783d 2235 2220 6669 656c  " index="5" fiel
+00004700: 643d 226c 616e 655f 6f72 6965 6e74 6174  d="lane_orientat
+00004710: 696f 6e22 2f3e 0a20 203c 2f61 6c69 6173  ion"/>.  </alias
+00004720: 6573 3e0a 2020 3c64 6566 6175 6c74 733e  es>.  <defaults>
+00004730: 0a20 2020 203c 6465 6661 756c 7420 6669  .    <default fi
+00004740: 656c 643d 2274 7970 6522 2065 7870 7265  eld="type" expre
+00004750: 7373 696f 6e3d 2222 2061 7070 6c79 4f6e  ssion="" applyOn
+00004760: 5570 6461 7465 3d22 3022 2f3e 0a20 2020  Update="0"/>.   
+00004770: 203c 6465 6661 756c 7420 6669 656c 643d   <default field=
+00004780: 226f 736d 5f69 6422 2065 7870 7265 7373  "osm_id" express
+00004790: 696f 6e3d 2222 2061 7070 6c79 4f6e 5570  ion="" applyOnUp
+000047a0: 6461 7465 3d22 3022 2f3e 0a20 2020 203c  date="0"/>.    <
+000047b0: 6465 6661 756c 7420 6669 656c 643d 226f  default field="o
+000047c0: 7269 656e 7461 7469 6f6e 2220 6578 7072  rientation" expr
+000047d0: 6573 7369 6f6e 3d22 2220 6170 706c 794f  ession="" applyO
+000047e0: 6e55 7064 6174 653d 2230 222f 3e0a 2020  nUpdate="0"/>.  
+000047f0: 2020 3c64 6566 6175 6c74 2066 6965 6c64    <default field
+00004800: 3d22 6f72 6965 6e74 6174 696f 6e5f 636f  ="orientation_co
+00004810: 6e66 6964 656e 6365 2220 6578 7072 6573  nfidence" expres
+00004820: 7369 6f6e 3d22 2220 6170 706c 794f 6e55  sion="" applyOnU
+00004830: 7064 6174 653d 2230 222f 3e0a 2020 2020  pdate="0"/>.    
+00004840: 3c64 6566 6175 6c74 2066 6965 6c64 3d22  <default field="
+00004850: 6c61 6e65 5f77 6964 7468 2220 6578 7072  lane_width" expr
+00004860: 6573 7369 6f6e 3d22 2220 6170 706c 794f  ession="" applyO
+00004870: 6e55 7064 6174 653d 2230 222f 3e0a 2020  nUpdate="0"/>.  
+00004880: 2020 3c64 6566 6175 6c74 2066 6965 6c64    <default field
+00004890: 3d22 6c61 6e65 5f6f 7269 656e 7461 7469  ="lane_orientati
+000048a0: 6f6e 2220 6578 7072 6573 7369 6f6e 3d22  on" expression="
+000048b0: 2220 6170 706c 794f 6e55 7064 6174 653d  " applyOnUpdate=
+000048c0: 2230 222f 3e0a 2020 3c2f 6465 6661 756c  "0"/>.  </defaul
+000048d0: 7473 3e0a 2020 3c63 6f6e 7374 7261 696e  ts>.  <constrain
+000048e0: 7473 3e0a 2020 2020 3c63 6f6e 7374 7261  ts>.    <constra
+000048f0: 696e 7420 756e 6971 7565 5f73 7472 656e  int unique_stren
+00004900: 6774 683d 2230 2220 6e6f 746e 756c 6c5f  gth="0" notnull_
+00004910: 7374 7265 6e67 7468 3d22 3022 2065 7870  strength="0" exp
+00004920: 5f73 7472 656e 6774 683d 2230 2220 6669  _strength="0" fi
+00004930: 656c 643d 2274 7970 6522 2063 6f6e 7374  eld="type" const
+00004940: 7261 696e 7473 3d22 3022 2f3e 0a20 2020  raints="0"/>.   
+00004950: 203c 636f 6e73 7472 6169 6e74 2075 6e69   <constraint uni
+00004960: 7175 655f 7374 7265 6e67 7468 3d22 3022  que_strength="0"
+00004970: 206e 6f74 6e75 6c6c 5f73 7472 656e 6774   notnull_strengt
+00004980: 683d 2230 2220 6578 705f 7374 7265 6e67  h="0" exp_streng
+00004990: 7468 3d22 3022 2066 6965 6c64 3d22 6f73  th="0" field="os
+000049a0: 6d5f 6964 2220 636f 6e73 7472 6169 6e74  m_id" constraint
+000049b0: 733d 2230 222f 3e0a 2020 2020 3c63 6f6e  s="0"/>.    <con
+000049c0: 7374 7261 696e 7420 756e 6971 7565 5f73  straint unique_s
+000049d0: 7472 656e 6774 683d 2230 2220 6e6f 746e  trength="0" notn
+000049e0: 756c 6c5f 7374 7265 6e67 7468 3d22 3022  ull_strength="0"
+000049f0: 2065 7870 5f73 7472 656e 6774 683d 2230   exp_strength="0
+00004a00: 2220 6669 656c 643d 226f 7269 656e 7461  " field="orienta
+00004a10: 7469 6f6e 2220 636f 6e73 7472 6169 6e74  tion" constraint
+00004a20: 733d 2230 222f 3e0a 2020 2020 3c63 6f6e  s="0"/>.    <con
+00004a30: 7374 7261 696e 7420 756e 6971 7565 5f73  straint unique_s
+00004a40: 7472 656e 6774 683d 2230 2220 6e6f 746e  trength="0" notn
+00004a50: 756c 6c5f 7374 7265 6e67 7468 3d22 3022  ull_strength="0"
+00004a60: 2065 7870 5f73 7472 656e 6774 683d 2230   exp_strength="0
+00004a70: 2220 6669 656c 643d 226f 7269 656e 7461  " field="orienta
+00004a80: 7469 6f6e 5f63 6f6e 6669 6465 6e63 6522  tion_confidence"
+00004a90: 2063 6f6e 7374 7261 696e 7473 3d22 3022   constraints="0"
+00004aa0: 2f3e 0a20 2020 203c 636f 6e73 7472 6169  />.    <constrai
+00004ab0: 6e74 2075 6e69 7175 655f 7374 7265 6e67  nt unique_streng
+00004ac0: 7468 3d22 3022 206e 6f74 6e75 6c6c 5f73  th="0" notnull_s
+00004ad0: 7472 656e 6774 683d 2230 2220 6578 705f  trength="0" exp_
+00004ae0: 7374 7265 6e67 7468 3d22 3022 2066 6965  strength="0" fie
+00004af0: 6c64 3d22 6c61 6e65 5f77 6964 7468 2220  ld="lane_width" 
+00004b00: 636f 6e73 7472 6169 6e74 733d 2230 222f  constraints="0"/
+00004b10: 3e0a 2020 2020 3c63 6f6e 7374 7261 696e  >.    <constrain
+00004b20: 7420 756e 6971 7565 5f73 7472 656e 6774  t unique_strengt
+00004b30: 683d 2230 2220 6e6f 746e 756c 6c5f 7374  h="0" notnull_st
+00004b40: 7265 6e67 7468 3d22 3022 2065 7870 5f73  rength="0" exp_s
+00004b50: 7472 656e 6774 683d 2230 2220 6669 656c  trength="0" fiel
+00004b60: 643d 226c 616e 655f 6f72 6965 6e74 6174  d="lane_orientat
+00004b70: 696f 6e22 2063 6f6e 7374 7261 696e 7473  ion" constraints
+00004b80: 3d22 3022 2f3e 0a20 203c 2f63 6f6e 7374  ="0"/>.  </const
+00004b90: 7261 696e 7473 3e0a 2020 3c63 6f6e 7374  raints>.  <const
+00004ba0: 7261 696e 7445 7870 7265 7373 696f 6e73  raintExpressions
+00004bb0: 3e0a 2020 2020 3c63 6f6e 7374 7261 696e  >.    <constrain
+00004bc0: 7420 6465 7363 3d22 2220 6578 703d 2222  t desc="" exp=""
+00004bd0: 2066 6965 6c64 3d22 7479 7065 222f 3e0a   field="type"/>.
+00004be0: 2020 2020 3c63 6f6e 7374 7261 696e 7420      <constraint 
+00004bf0: 6465 7363 3d22 2220 6578 703d 2222 2066  desc="" exp="" f
+00004c00: 6965 6c64 3d22 6f73 6d5f 6964 222f 3e0a  ield="osm_id"/>.
+00004c10: 2020 2020 3c63 6f6e 7374 7261 696e 7420      <constraint 
+00004c20: 6465 7363 3d22 2220 6578 703d 2222 2066  desc="" exp="" f
+00004c30: 6965 6c64 3d22 6f72 6965 6e74 6174 696f  ield="orientatio
+00004c40: 6e22 2f3e 0a20 2020 203c 636f 6e73 7472  n"/>.    <constr
+00004c50: 6169 6e74 2064 6573 633d 2222 2065 7870  aint desc="" exp
+00004c60: 3d22 2220 6669 656c 643d 226f 7269 656e  ="" field="orien
+00004c70: 7461 7469 6f6e 5f63 6f6e 6669 6465 6e63  tation_confidenc
+00004c80: 6522 2f3e 0a20 2020 203c 636f 6e73 7472  e"/>.    <constr
+00004c90: 6169 6e74 2064 6573 633d 2222 2065 7870  aint desc="" exp
+00004ca0: 3d22 2220 6669 656c 643d 226c 616e 655f  ="" field="lane_
+00004cb0: 7769 6474 6822 2f3e 0a20 2020 203c 636f  width"/>.    <co
+00004cc0: 6e73 7472 6169 6e74 2064 6573 633d 2222  nstraint desc=""
+00004cd0: 2065 7870 3d22 2220 6669 656c 643d 226c   exp="" field="l
+00004ce0: 616e 655f 6f72 6965 6e74 6174 696f 6e22  ane_orientation"
+00004cf0: 2f3e 0a20 203c 2f63 6f6e 7374 7261 696e  />.  </constrain
+00004d00: 7445 7870 7265 7373 696f 6e73 3e0a 2020  tExpressions>.  
+00004d10: 3c65 7870 7265 7373 696f 6e66 6965 6c64  <expressionfield
+00004d20: 732f 3e0a 2020 3c61 7474 7269 6275 7465  s/>.  <attribute
+00004d30: 6163 7469 6f6e 733e 0a20 2020 203c 6465  actions>.    <de
+00004d40: 6661 756c 7441 6374 696f 6e20 7661 6c75  faultAction valu
+00004d50: 653d 227b 3030 3030 3030 3030 2d30 3030  e="{00000000-000
+00004d60: 302d 3030 3030 2d30 3030 302d 3030 3030  0-0000-0000-0000
+00004d70: 3030 3030 3030 3030 7d22 206b 6579 3d22  00000000}" key="
+00004d80: 4361 6e76 6173 222f 3e0a 2020 3c2f 6174  Canvas"/>.  </at
+00004d90: 7472 6962 7574 6561 6374 696f 6e73 3e0a  tributeactions>.
+00004da0: 2020 3c61 7474 7269 6275 7465 7461 626c    <attributetabl
+00004db0: 6563 6f6e 6669 6720 6163 7469 6f6e 5769  econfig actionWi
+00004dc0: 6467 6574 5374 796c 653d 2264 726f 7044  dgetStyle="dropD
+00004dd0: 6f77 6e22 2073 6f72 744f 7264 6572 3d22  own" sortOrder="
+00004de0: 3022 2073 6f72 7445 7870 7265 7373 696f  0" sortExpressio
+00004df0: 6e3d 2222 3e0a 2020 2020 3c63 6f6c 756d  n="">.    <colum
+00004e00: 6e73 3e0a 2020 2020 2020 3c63 6f6c 756d  ns>.      <colum
+00004e10: 6e20 6e61 6d65 3d22 7479 7065 2220 7769  n name="type" wi
+00004e20: 6474 683d 222d 3122 2068 6964 6465 6e3d  dth="-1" hidden=
+00004e30: 2230 2220 7479 7065 3d22 6669 656c 6422  "0" type="field"
+00004e40: 2f3e 0a20 2020 2020 203c 636f 6c75 6d6e  />.      <column
+00004e50: 206e 616d 653d 226f 736d 5f69 6422 2077   name="osm_id" w
+00004e60: 6964 7468 3d22 3137 3122 2068 6964 6465  idth="171" hidde
+00004e70: 6e3d 2230 2220 7479 7065 3d22 6669 656c  n="0" type="fiel
+00004e80: 6422 2f3e 0a20 2020 2020 203c 636f 6c75  d"/>.      <colu
+00004e90: 6d6e 206e 616d 653d 226f 7269 656e 7461  mn name="orienta
+00004ea0: 7469 6f6e 2220 7769 6474 683d 2232 3932  tion" width="292
+00004eb0: 2220 6869 6464 656e 3d22 3022 2074 7970  " hidden="0" typ
+00004ec0: 653d 2266 6965 6c64 222f 3e0a 2020 2020  e="field"/>.    
+00004ed0: 2020 3c63 6f6c 756d 6e20 6e61 6d65 3d22    <column name="
+00004ee0: 6f72 6965 6e74 6174 696f 6e5f 636f 6e66  orientation_conf
+00004ef0: 6964 656e 6365 2220 7769 6474 683d 222d  idence" width="-
+00004f00: 3122 2068 6964 6465 6e3d 2230 2220 7479  1" hidden="0" ty
+00004f10: 7065 3d22 6669 656c 6422 2f3e 0a20 2020  pe="field"/>.   
+00004f20: 2020 203c 636f 6c75 6d6e 206e 616d 653d     <column name=
+00004f30: 226c 616e 655f 6f72 6965 6e74 6174 696f  "lane_orientatio
+00004f40: 6e22 2077 6964 7468 3d22 2d31 2220 6869  n" width="-1" hi
+00004f50: 6464 656e 3d22 3022 2074 7970 653d 2266  dden="0" type="f
+00004f60: 6965 6c64 222f 3e0a 2020 2020 2020 3c63  ield"/>.      <c
+00004f70: 6f6c 756d 6e20 6e61 6d65 3d22 6c61 6e65  olumn name="lane
+00004f80: 5f77 6964 7468 2220 7769 6474 683d 222d  _width" width="-
+00004f90: 3122 2068 6964 6465 6e3d 2230 2220 7479  1" hidden="0" ty
+00004fa0: 7065 3d22 6669 656c 6422 2f3e 0a20 2020  pe="field"/>.   
+00004fb0: 2020 203c 636f 6c75 6d6e 2077 6964 7468     <column width
+00004fc0: 3d22 2d31 2220 6869 6464 656e 3d22 3122  ="-1" hidden="1"
+00004fd0: 2074 7970 653d 2261 6374 696f 6e73 222f   type="actions"/
+00004fe0: 3e0a 2020 2020 3c2f 636f 6c75 6d6e 733e  >.    </columns>
+00004ff0: 0a20 203c 2f61 7474 7269 6275 7465 7461  .  </attributeta
+00005000: 626c 6563 6f6e 6669 673e 0a20 203c 636f  bleconfig>.  <co
+00005010: 6e64 6974 696f 6e61 6c73 7479 6c65 733e  nditionalstyles>
+00005020: 0a20 2020 203c 726f 7773 7479 6c65 732f  .    <rowstyles/
+00005030: 3e0a 2020 2020 3c66 6965 6c64 7374 796c  >.    <fieldstyl
+00005040: 6573 2f3e 0a20 203c 2f63 6f6e 6469 7469  es/>.  </conditi
+00005050: 6f6e 616c 7374 796c 6573 3e0a 2020 3c73  onalstyles>.  <s
+00005060: 746f 7265 6465 7870 7265 7373 696f 6e73  toredexpressions
+00005070: 2f3e 0a20 203c 6564 6974 666f 726d 2074  />.  <editform t
+00005080: 6f6c 6572 616e 743d 2231 223e 3c2f 6564  olerant="1"></ed
+00005090: 6974 666f 726d 3e0a 2020 3c65 6469 7466  itform>.  <editf
+000050a0: 6f72 6d69 6e69 742f 3e0a 2020 3c65 6469  orminit/>.  <edi
+000050b0: 7466 6f72 6d69 6e69 7463 6f64 6573 6f75  tforminitcodesou
+000050c0: 7263 653e 303c 2f65 6469 7466 6f72 6d69  rce>0</editformi
+000050d0: 6e69 7463 6f64 6573 6f75 7263 653e 0a20  nitcodesource>. 
+000050e0: 203c 6564 6974 666f 726d 696e 6974 6669   <editforminitfi
+000050f0: 6c65 7061 7468 3e3c 2f65 6469 7466 6f72  lepath></editfor
+00005100: 6d69 6e69 7466 696c 6570 6174 683e 0a20  minitfilepath>. 
+00005110: 203c 6564 6974 666f 726d 696e 6974 636f   <editforminitco
+00005120: 6465 3e3c 215b 4344 4154 415b 2320 2d2a  de><![CDATA[# -*
+00005130: 2d20 636f 6469 6e67 3a20 7574 662d 3820  - coding: utf-8 
+00005140: 2d2a 2d0a 2222 220a 4c65 7320 666f 726d  -*-.""".Les form
+00005150: 756c 6169 7265 7320 5147 4953 2070 6575  ulaires QGIS peu
+00005160: 7665 6e74 2061 766f 6972 2075 6e65 2066  vent avoir une f
+00005170: 6f6e 6374 696f 6e20 5079 7468 6f6e 2071  onction Python q
+00005180: 7569 2065 7374 2061 7070 656c c3a9 6520  ui est appel..e 
+00005190: 6c6f 7273 7175 6520 6c65 2066 6f72 6d75  lorsque le formu
+000051a0: 6c61 6972 6520 6573 740a 6f75 7665 7274  laire est.ouvert
+000051b0: 2e0a 0a55 7469 6c69 7365 7a20 6365 7474  ...Utilisez cett
+000051c0: 6520 666f 6e63 7469 6f6e 2070 6f75 7220  e fonction pour 
+000051d0: 616a 6f75 7465 7220 756e 6520 6c6f 6769  ajouter une logi
+000051e0: 7175 6520 7375 7070 6cc3 a96d 656e 7461  que suppl..menta
+000051f0: 6972 6520 c3a0 2076 6f73 2066 6f72 6d75  ire .. vos formu
+00005200: 6c61 6972 6573 2e0a 0a45 6e74 7265 7a20  laires...Entrez 
+00005210: 6c65 206e 6f6d 2064 6520 6c61 2066 6f6e  le nom de la fon
+00005220: 6374 696f 6e20 6461 6e73 206c 6520 6368  ction dans le ch
+00005230: 616d 7020 0a22 466f 6e63 7469 6f6e 2064  amp ."Fonction d
+00005240: 2769 6e69 7469 616c 6973 6174 696f 6e20  'initialisation 
+00005250: 5079 7468 6f6e 222e 0a56 6f69 6369 2075  Python"..Voici u
+00005260: 6e20 6578 656d 706c 653a 0a22 2222 0a66  n exemple:.""".f
+00005270: 726f 6d20 7167 6973 2e50 7951 742e 5174  rom qgis.PyQt.Qt
+00005280: 5769 6467 6574 7320 696d 706f 7274 2051  Widgets import Q
+00005290: 5769 6467 6574 0a0a 6465 6620 6d79 5f66  Widget..def my_f
+000052a0: 6f72 6d5f 6f70 656e 2864 6961 6c6f 672c  orm_open(dialog,
+000052b0: 206c 6179 6572 2c20 6665 6174 7572 6529   layer, feature)
+000052c0: 3a0a 2020 2020 6765 6f6d 203d 2066 6561  :.    geom = fea
+000052d0: 7475 7265 2e67 656f 6d65 7472 7928 290a  ture.geometry().
+000052e0: 2020 2020 636f 6e74 726f 6c20 3d20 6469      control = di
+000052f0: 616c 6f67 2e66 696e 6443 6869 6c64 2851  alog.findChild(Q
+00005300: 5769 6467 6574 2c20 224d 794c 696e 6545  Widget, "MyLineE
+00005310: 6469 7422 290a 5d5d 3e3c 2f65 6469 7466  dit").]]></editf
+00005320: 6f72 6d69 6e69 7463 6f64 653e 0a20 203c  orminitcode>.  <
+00005330: 6665 6174 666f 726d 7375 7070 7265 7373  featformsuppress
+00005340: 3e30 3c2f 6665 6174 666f 726d 7375 7070  >0</featformsupp
+00005350: 7265 7373 3e0a 2020 3c65 6469 746f 726c  ress>.  <editorl
+00005360: 6179 6f75 743e 6765 6e65 7261 7465 646c  ayout>generatedl
+00005370: 6179 6f75 743c 2f65 6469 746f 726c 6179  ayout</editorlay
+00005380: 6f75 743e 0a20 203c 6564 6974 6162 6c65  out>.  <editable
+00005390: 3e0a 2020 2020 3c66 6965 6c64 206e 616d  >.    <field nam
+000053a0: 653d 2261 6e67 6c65 2220 6564 6974 6162  e="angle" editab
+000053b0: 6c65 3d22 3122 2f3e 0a20 2020 203c 6669  le="1"/>.    <fi
+000053c0: 656c 6420 6e61 6d65 3d22 6669 6422 2065  eld name="fid" e
+000053d0: 6469 7461 626c 653d 2231 222f 3e0a 2020  ditable="1"/>.  
+000053e0: 2020 3c66 6965 6c64 206e 616d 653d 226c    <field name="l
+000053f0: 616e 655f 6f72 6965 6e74 6174 696f 6e22  ane_orientation"
+00005400: 2065 6469 7461 626c 653d 2231 222f 3e0a   editable="1"/>.
+00005410: 2020 2020 3c66 6965 6c64 206e 616d 653d      <field name=
+00005420: 226c 616e 655f 7769 6474 6822 2065 6469  "lane_width" edi
+00005430: 7461 626c 653d 2231 222f 3e0a 2020 2020  table="1"/>.    
+00005440: 3c66 6965 6c64 206e 616d 653d 226f 7269  <field name="ori
+00005450: 656e 7461 7469 6f6e 2220 6564 6974 6162  entation" editab
+00005460: 6c65 3d22 3122 2f3e 0a20 2020 203c 6669  le="1"/>.    <fi
+00005470: 656c 6420 6e61 6d65 3d22 6f72 6965 6e74  eld name="orient
+00005480: 6174 696f 6e5f 636f 6e66 6964 656e 6365  ation_confidence
+00005490: 2220 6564 6974 6162 6c65 3d22 3122 2f3e  " editable="1"/>
+000054a0: 0a20 2020 203c 6669 656c 6420 6e61 6d65  .    <field name
+000054b0: 3d22 6f73 6d5f 6964 2220 6564 6974 6162  ="osm_id" editab
+000054c0: 6c65 3d22 3122 2f3e 0a20 2020 203c 6669  le="1"/>.    <fi
+000054d0: 656c 6420 6e61 6d65 3d22 7479 7065 2220  eld name="type" 
+000054e0: 6564 6974 6162 6c65 3d22 3122 2f3e 0a20  editable="1"/>. 
+000054f0: 203c 2f65 6469 7461 626c 653e 0a20 203c   </editable>.  <
+00005500: 6c61 6265 6c4f 6e54 6f70 3e0a 2020 2020  labelOnTop>.    
+00005510: 3c66 6965 6c64 206e 616d 653d 2261 6e67  <field name="ang
+00005520: 6c65 2220 6c61 6265 6c4f 6e54 6f70 3d22  le" labelOnTop="
+00005530: 3022 2f3e 0a20 2020 203c 6669 656c 6420  0"/>.    <field 
+00005540: 6e61 6d65 3d22 6669 6422 206c 6162 656c  name="fid" label
+00005550: 4f6e 546f 703d 2230 222f 3e0a 2020 2020  OnTop="0"/>.    
+00005560: 3c66 6965 6c64 206e 616d 653d 226c 616e  <field name="lan
+00005570: 655f 6f72 6965 6e74 6174 696f 6e22 206c  e_orientation" l
+00005580: 6162 656c 4f6e 546f 703d 2230 222f 3e0a  abelOnTop="0"/>.
+00005590: 2020 2020 3c66 6965 6c64 206e 616d 653d      <field name=
+000055a0: 226c 616e 655f 7769 6474 6822 206c 6162  "lane_width" lab
+000055b0: 656c 4f6e 546f 703d 2230 222f 3e0a 2020  elOnTop="0"/>.  
+000055c0: 2020 3c66 6965 6c64 206e 616d 653d 226f    <field name="o
+000055d0: 7269 656e 7461 7469 6f6e 2220 6c61 6265  rientation" labe
+000055e0: 6c4f 6e54 6f70 3d22 3022 2f3e 0a20 2020  lOnTop="0"/>.   
+000055f0: 203c 6669 656c 6420 6e61 6d65 3d22 6f72   <field name="or
+00005600: 6965 6e74 6174 696f 6e5f 636f 6e66 6964  ientation_confid
+00005610: 656e 6365 2220 6c61 6265 6c4f 6e54 6f70  ence" labelOnTop
+00005620: 3d22 3022 2f3e 0a20 2020 203c 6669 656c  ="0"/>.    <fiel
+00005630: 6420 6e61 6d65 3d22 6f73 6d5f 6964 2220  d name="osm_id" 
+00005640: 6c61 6265 6c4f 6e54 6f70 3d22 3022 2f3e  labelOnTop="0"/>
+00005650: 0a20 2020 203c 6669 656c 6420 6e61 6d65  .    <field name
+00005660: 3d22 7479 7065 2220 6c61 6265 6c4f 6e54  ="type" labelOnT
+00005670: 6f70 3d22 3022 2f3e 0a20 203c 2f6c 6162  op="0"/>.  </lab
+00005680: 656c 4f6e 546f 703e 0a20 203c 7265 7573  elOnTop>.  <reus
+00005690: 654c 6173 7456 616c 7565 3e0a 2020 2020  eLastValue>.    
+000056a0: 3c66 6965 6c64 206e 616d 653d 2261 6e67  <field name="ang
+000056b0: 6c65 2220 7265 7573 654c 6173 7456 616c  le" reuseLastVal
+000056c0: 7565 3d22 3022 2f3e 0a20 2020 203c 6669  ue="0"/>.    <fi
+000056d0: 656c 6420 6e61 6d65 3d22 6669 6422 2072  eld name="fid" r
+000056e0: 6575 7365 4c61 7374 5661 6c75 653d 2230  euseLastValue="0
+000056f0: 222f 3e0a 2020 2020 3c66 6965 6c64 206e  "/>.    <field n
+00005700: 616d 653d 226c 616e 655f 6f72 6965 6e74  ame="lane_orient
+00005710: 6174 696f 6e22 2072 6575 7365 4c61 7374  ation" reuseLast
+00005720: 5661 6c75 653d 2230 222f 3e0a 2020 2020  Value="0"/>.    
+00005730: 3c66 6965 6c64 206e 616d 653d 226c 616e  <field name="lan
+00005740: 655f 7769 6474 6822 2072 6575 7365 4c61  e_width" reuseLa
+00005750: 7374 5661 6c75 653d 2230 222f 3e0a 2020  stValue="0"/>.  
+00005760: 2020 3c66 6965 6c64 206e 616d 653d 226f    <field name="o
+00005770: 7269 656e 7461 7469 6f6e 2220 7265 7573  rientation" reus
+00005780: 654c 6173 7456 616c 7565 3d22 3022 2f3e  eLastValue="0"/>
+00005790: 0a20 2020 203c 6669 656c 6420 6e61 6d65  .    <field name
+000057a0: 3d22 6f72 6965 6e74 6174 696f 6e5f 636f  ="orientation_co
+000057b0: 6e66 6964 656e 6365 2220 7265 7573 654c  nfidence" reuseL
+000057c0: 6173 7456 616c 7565 3d22 3022 2f3e 0a20  astValue="0"/>. 
+000057d0: 2020 203c 6669 656c 6420 6e61 6d65 3d22     <field name="
+000057e0: 6f73 6d5f 6964 2220 7265 7573 654c 6173  osm_id" reuseLas
+000057f0: 7456 616c 7565 3d22 3022 2f3e 0a20 2020  tValue="0"/>.   
+00005800: 203c 6669 656c 6420 6e61 6d65 3d22 7479   <field name="ty
+00005810: 7065 2220 7265 7573 654c 6173 7456 616c  pe" reuseLastVal
+00005820: 7565 3d22 3022 2f3e 0a20 203c 2f72 6575  ue="0"/>.  </reu
+00005830: 7365 4c61 7374 5661 6c75 653e 0a20 203c  seLastValue>.  <
+00005840: 6461 7461 4465 6669 6e65 6446 6965 6c64  dataDefinedField
+00005850: 5072 6f70 6572 7469 6573 2f3e 0a20 203c  Properties/>.  <
+00005860: 7769 6467 6574 732f 3e0a 2020 3c70 7265  widgets/>.  <pre
+00005870: 7669 6577 4578 7072 6573 7369 6f6e 3e22  viewExpression>"
+00005880: 7479 7065 223c 2f70 7265 7669 6577 4578  type"</previewEx
+00005890: 7072 6573 7369 6f6e 3e0a 2020 3c6d 6170  pression>.  <map
+000058a0: 5469 703e 3c2f 6d61 7054 6970 3e0a 2020  Tip></mapTip>.  
+000058b0: 3c6c 6179 6572 4765 6f6d 6574 7279 5479  <layerGeometryTy
+000058c0: 7065 3e30 3c2f 6c61 7965 7247 656f 6d65  pe>0</layerGeome
+000058d0: 7472 7954 7970 653e 0a3c 2f71 6769 733e  tryType>.</qgis>
+000058e0: 0a                                       .
```

### Comparing `crossroads-schematization-0.0.9/crschem/resources/rendering-nodes.qml` & `crossroads-schematization-0.1.0/crschem/resources/rendering-nodes.qml`

 * *Files 0% similar despite different names*

```diff
@@ -698,1506 +698,1506 @@
 00002b90: 616d 653d 2261 6e67 6c65 2220 7479 7065  ame="angle" type
 00002ba0: 3d22 4d61 7022 3e0a 2020 2020 2020 2020  ="Map">.        
 00002bb0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
 00002bc0: 6e20 7661 6c75 653d 2274 7275 6522 206e  n value="true" n
 00002bd0: 616d 653d 2261 6374 6976 6522 2074 7970  ame="active" typ
 00002be0: 653d 2262 6f6f 6c22 2f3e 0a20 2020 2020  e="bool"/>.     
 00002bf0: 2020 2020 2020 2020 2020 2020 203c 4f70               <Op
-00002c00: 7469 6f6e 2076 616c 7565 3d22 3138 3020  tion value="180 
-00002c10: 2b20 282d 2671 756f 743b 6f72 6965 6e74  + (-&quot;orient
-00002c20: 6174 696f 6e26 7175 6f74 3b20 2f20 7069  ation&quot; / pi
-00002c30: 2829 2920 2a20 3138 3022 206e 616d 653d  ()) * 180" name=
-00002c40: 2265 7870 7265 7373 696f 6e22 2074 7970  "expression" typ
-00002c50: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00002c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c70: 3c4f 7074 696f 6e20 7661 6c75 653d 2233  <Option value="3
-00002c80: 2220 6e61 6d65 3d22 7479 7065 2220 7479  " name="type" ty
-00002c90: 7065 3d22 696e 7422 2f3e 0a20 2020 2020  pe="int"/>.     
-00002ca0: 2020 2020 2020 2020 2020 203c 2f4f 7074             </Opt
-00002cb0: 696f 6e3e 0a20 2020 2020 2020 2020 2020  ion>.           
-00002cc0: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
-00002cd0: 653d 226f 7574 6c69 6e65 5769 6474 6822  e="outlineWidth"
-00002ce0: 2074 7970 653d 224d 6170 223e 0a20 2020   type="Map">.   
-00002cf0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002d00: 4f70 7469 6f6e 2076 616c 7565 3d22 7472  Option value="tr
-00002d10: 7565 2220 6e61 6d65 3d22 6163 7469 7665  ue" name="active
-00002d20: 2220 7479 7065 3d22 626f 6f6c 222f 3e0a  " type="bool"/>.
+00002c00: 7469 6f6e 2076 616c 7565 3d22 3930 202b  tion value="90 +
+00002c10: 2028 2d26 7175 6f74 3b6f 7269 656e 7461   (-&quot;orienta
+00002c20: 7469 6f6e 2671 756f 743b 202f 2070 6928  tion&quot; / pi(
+00002c30: 2929 202a 2031 3830 2220 6e61 6d65 3d22  )) * 180" name="
+00002c40: 6578 7072 6573 7369 6f6e 2220 7479 7065  expression" type
+00002c50: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+00002c60: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00002c70: 4f70 7469 6f6e 2076 616c 7565 3d22 3322  Option value="3"
+00002c80: 206e 616d 653d 2274 7970 6522 2074 7970   name="type" typ
+00002c90: 653d 2269 6e74 222f 3e0a 2020 2020 2020  e="int"/>.      
+00002ca0: 2020 2020 2020 2020 2020 3c2f 4f70 7469            </Opti
+00002cb0: 6f6e 3e0a 2020 2020 2020 2020 2020 2020  on>.            
+00002cc0: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
+00002cd0: 3d22 6f75 746c 696e 6557 6964 7468 2220  ="outlineWidth" 
+00002ce0: 7479 7065 3d22 4d61 7022 3e0a 2020 2020  type="Map">.    
+00002cf0: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
+00002d00: 7074 696f 6e20 7661 6c75 653d 2274 7275  ption value="tru
+00002d10: 6522 206e 616d 653d 2261 6374 6976 6522  e" name="active"
+00002d20: 2074 7970 653d 2262 6f6f 6c22 2f3e 0a20   type="bool"/>. 
 00002d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d40: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
-00002d50: 2226 7175 6f74 3b6c 616e 655f 7769 6474  "&quot;lane_widt
-00002d60: 6826 7175 6f74 3b20 2a20 312e 3122 206e  h&quot; * 1.1" n
-00002d70: 616d 653d 2265 7870 7265 7373 696f 6e22  ame="expression"
-00002d80: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-00002d90: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00002da0: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-00002db0: 653d 2233 2220 6e61 6d65 3d22 7479 7065  e="3" name="type
-00002dc0: 2220 7479 7065 3d22 696e 7422 2f3e 0a20  " type="int"/>. 
-00002dd0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002de0: 2f4f 7074 696f 6e3e 0a20 2020 2020 2020  /Option>.       
-00002df0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-00002e00: 206e 616d 653d 2273 697a 6522 2074 7970   name="size" typ
-00002e10: 653d 224d 6170 223e 0a20 2020 2020 2020  e="Map">.       
-00002e20: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00002e30: 6f6e 2076 616c 7565 3d22 7472 7565 2220  on value="true" 
-00002e40: 6e61 6d65 3d22 6163 7469 7665 2220 7479  name="active" ty
-00002e50: 7065 3d22 626f 6f6c 222f 3e0a 2020 2020  pe="bool"/>.    
-00002e60: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
-00002e70: 7074 696f 6e20 7661 6c75 653d 2233 202b  ption value="3 +
-00002e80: 2032 202a 2030 2e30 3034 202a 2020 406d   2 * 0.004 *  @m
-00002e90: 6170 5f73 6361 6c65 2220 6e61 6d65 3d22  ap_scale" name="
-00002ea0: 6578 7072 6573 7369 6f6e 2220 7479 7065  expression" type
-00002eb0: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-00002ec0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002ed0: 4f70 7469 6f6e 2076 616c 7565 3d22 3322  Option value="3"
-00002ee0: 206e 616d 653d 2274 7970 6522 2074 7970   name="type" typ
-00002ef0: 653d 2269 6e74 222f 3e0a 2020 2020 2020  e="int"/>.      
-00002f00: 2020 2020 2020 2020 2020 3c2f 4f70 7469            </Opti
-00002f10: 6f6e 3e0a 2020 2020 2020 2020 2020 2020  on>.            
-00002f20: 2020 3c2f 4f70 7469 6f6e 3e0a 2020 2020    </Option>.    
-00002f30: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00002f40: 6e20 7661 6c75 653d 2263 6f6c 6c65 6374  n value="collect
-00002f50: 696f 6e22 206e 616d 653d 2274 7970 6522  ion" name="type"
-00002f60: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-00002f70: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
-00002f80: 4f70 7469 6f6e 3e0a 2020 2020 2020 2020  Option>.        
-00002f90: 2020 3c2f 6461 7461 5f64 6566 696e 6564    </data_defined
-00002fa0: 5f70 726f 7065 7274 6965 733e 0a20 2020  _properties>.   
-00002fb0: 2020 2020 203c 2f6c 6179 6572 3e0a 2020       </layer>.  
-00002fc0: 2020 2020 3c2f 7379 6d62 6f6c 3e0a 2020      </symbol>.  
-00002fd0: 2020 2020 3c73 796d 626f 6c20 6672 616d      <symbol fram
-00002fe0: 655f 7261 7465 3d22 3130 2220 6973 5f61  e_rate="10" is_a
-00002ff0: 6e69 6d61 7465 643d 2230 2220 6e61 6d65  nimated="0" name
-00003000: 3d22 3122 2061 6c70 6861 3d22 3122 2066  ="1" alpha="1" f
-00003010: 6f72 6365 5f72 6872 3d22 3022 2063 6c69  orce_rhr="0" cli
-00003020: 705f 746f 5f65 7874 656e 743d 2231 2220  p_to_extent="1" 
-00003030: 7479 7065 3d22 6d61 726b 6572 223e 0a20  type="marker">. 
-00003040: 2020 2020 2020 203c 6461 7461 5f64 6566         <data_def
-00003050: 696e 6564 5f70 726f 7065 7274 6965 733e  ined_properties>
-00003060: 0a20 2020 2020 2020 2020 203c 4f70 7469  .          <Opti
-00003070: 6f6e 2074 7970 653d 224d 6170 223e 0a20  on type="Map">. 
-00003080: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00003090: 6f6e 2076 616c 7565 3d22 2220 6e61 6d65  on value="" name
-000030a0: 3d22 6e61 6d65 2220 7479 7065 3d22 5153  ="name" type="QS
-000030b0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-000030c0: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
-000030d0: 653d 2270 726f 7065 7274 6965 7322 2f3e  e="properties"/>
-000030e0: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
-000030f0: 7469 6f6e 2076 616c 7565 3d22 636f 6c6c  tion value="coll
-00003100: 6563 7469 6f6e 2220 6e61 6d65 3d22 7479  ection" name="ty
-00003110: 7065 2220 7479 7065 3d22 5153 7472 696e  pe" type="QStrin
-00003120: 6722 2f3e 0a20 2020 2020 2020 2020 203c  g"/>.          <
-00003130: 2f4f 7074 696f 6e3e 0a20 2020 2020 2020  /Option>.       
-00003140: 203c 2f64 6174 615f 6465 6669 6e65 645f   </data_defined_
-00003150: 7072 6f70 6572 7469 6573 3e0a 2020 2020  properties>.    
-00003160: 2020 2020 3c6c 6179 6572 2065 6e61 626c      <layer enabl
-00003170: 6564 3d22 3122 2063 6c61 7373 3d22 5369  ed="1" class="Si
-00003180: 6d70 6c65 4d61 726b 6572 2220 6c6f 636b  mpleMarker" lock
-00003190: 6564 3d22 3022 2070 6173 733d 2230 223e  ed="0" pass="0">
-000031a0: 0a20 2020 2020 2020 2020 203c 4f70 7469  .          <Opti
-000031b0: 6f6e 2074 7970 653d 224d 6170 223e 0a20  on type="Map">. 
-000031c0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-000031d0: 6f6e 2076 616c 7565 3d22 3022 206e 616d  on value="0" nam
-000031e0: 653d 2261 6e67 6c65 2220 7479 7065 3d22  e="angle" type="
-000031f0: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-00003200: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-00003210: 616c 7565 3d22 666c 6174 2220 6e61 6d65  alue="flat" name
-00003220: 3d22 6361 705f 7374 796c 6522 2074 7970  ="cap_style" typ
-00003230: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00003240: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00003250: 6e20 7661 6c75 653d 2231 3435 2c38 322c  n value="145,82,
-00003260: 3435 2c32 3535 2220 6e61 6d65 3d22 636f  45,255" name="co
-00003270: 6c6f 7222 2074 7970 653d 2251 5374 7269  lor" type="QStri
-00003280: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
-00003290: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
-000032a0: 2231 2220 6e61 6d65 3d22 686f 7269 7a6f  "1" name="horizo
-000032b0: 6e74 616c 5f61 6e63 686f 725f 706f 696e  ntal_anchor_poin
-000032c0: 7422 2074 7970 653d 2251 5374 7269 6e67  t" type="QString
-000032d0: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-000032e0: 3c4f 7074 696f 6e20 7661 6c75 653d 226d  <Option value="m
-000032f0: 6974 6572 2220 6e61 6d65 3d22 6a6f 696e  iter" name="join
-00003300: 7374 796c 6522 2074 7970 653d 2251 5374  style" type="QSt
-00003310: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-00003320: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-00003330: 653d 226c 696e 6522 206e 616d 653d 226e  e="line" name="n
-00003340: 616d 6522 2074 7970 653d 2251 5374 7269  ame" type="QStri
-00003350: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
-00003360: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
-00003370: 2230 2c30 2220 6e61 6d65 3d22 6f66 6673  "0,0" name="offs
-00003380: 6574 2220 7479 7065 3d22 5153 7472 696e  et" type="QStrin
-00003390: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
-000033a0: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-000033b0: 3378 3a30 2c30 2c30 2c30 2c30 2c30 2220  3x:0,0,0,0,0,0" 
-000033c0: 6e61 6d65 3d22 6f66 6673 6574 5f6d 6170  name="offset_map
-000033d0: 5f75 6e69 745f 7363 616c 6522 2074 7970  _unit_scale" typ
-000033e0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-000033f0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00003400: 6e20 7661 6c75 653d 224d 4d22 206e 616d  n value="MM" nam
-00003410: 653d 226f 6666 7365 745f 756e 6974 2220  e="offset_unit" 
-00003420: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
-00003430: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
-00003440: 7469 6f6e 2076 616c 7565 3d22 302c 302c  tion value="0,0,
-00003450: 302c 3235 3522 206e 616d 653d 226f 7574  0,255" name="out
-00003460: 6c69 6e65 5f63 6f6c 6f72 2220 7479 7065  line_color" type
-00003470: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-00003480: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-00003490: 2076 616c 7565 3d22 736f 6c69 6422 206e   value="solid" n
-000034a0: 616d 653d 226f 7574 6c69 6e65 5f73 7479  ame="outline_sty
-000034b0: 6c65 2220 7479 7065 3d22 5153 7472 696e  le" type="QStrin
-000034c0: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
-000034d0: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-000034e0: 3222 206e 616d 653d 226f 7574 6c69 6e65  2" name="outline
-000034f0: 5f77 6964 7468 2220 7479 7065 3d22 5153  _width" type="QS
-00003500: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00003510: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00003520: 7565 3d22 3378 3a30 2c30 2c30 2c30 2c30  ue="3x:0,0,0,0,0
-00003530: 2c30 2220 6e61 6d65 3d22 6f75 746c 696e  ,0" name="outlin
-00003540: 655f 7769 6474 685f 6d61 705f 756e 6974  e_width_map_unit
-00003550: 5f73 6361 6c65 2220 7479 7065 3d22 5153  _scale" type="QS
-00003560: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00003570: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00003580: 7565 3d22 5265 6e64 6572 4d65 7465 7273  ue="RenderMeters
-00003590: 496e 4d61 7055 6e69 7473 2220 6e61 6d65  InMapUnits" name
-000035a0: 3d22 6f75 746c 696e 655f 7769 6474 685f  ="outline_width_
-000035b0: 756e 6974 2220 7479 7065 3d22 5153 7472  unit" type="QStr
-000035c0: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-000035d0: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
-000035e0: 3d22 6469 616d 6574 6572 2220 6e61 6d65  ="diameter" name
-000035f0: 3d22 7363 616c 655f 6d65 7468 6f64 2220  ="scale_method" 
-00003600: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
-00003610: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
-00003620: 7469 6f6e 2076 616c 7565 3d22 3322 206e  tion value="3" n
-00003630: 616d 653d 2273 697a 6522 2074 7970 653d  ame="size" type=
-00003640: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-00003650: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00003660: 7661 6c75 653d 2233 783a 302c 302c 302c  value="3x:0,0,0,
-00003670: 302c 302c 3022 206e 616d 653d 2273 697a  0,0,0" name="siz
-00003680: 655f 6d61 705f 756e 6974 5f73 6361 6c65  e_map_unit_scale
-00003690: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-000036a0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-000036b0: 4f70 7469 6f6e 2076 616c 7565 3d22 5265  Option value="Re
-000036c0: 6e64 6572 4d65 7465 7273 496e 4d61 7055  nderMetersInMapU
-000036d0: 6e69 7473 2220 6e61 6d65 3d22 7369 7a65  nits" name="size
-000036e0: 5f75 6e69 7422 2074 7970 653d 2251 5374  _unit" type="QSt
-000036f0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-00003700: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-00003710: 653d 2231 2220 6e61 6d65 3d22 7665 7274  e="1" name="vert
-00003720: 6963 616c 5f61 6e63 686f 725f 706f 696e  ical_anchor_poin
-00003730: 7422 2074 7970 653d 2251 5374 7269 6e67  t" type="QString
-00003740: 222f 3e0a 2020 2020 2020 2020 2020 3c2f  "/>.          </
-00003750: 4f70 7469 6f6e 3e0a 2020 2020 2020 2020  Option>.        
-00003760: 2020 3c64 6174 615f 6465 6669 6e65 645f    <data_defined_
-00003770: 7072 6f70 6572 7469 6573 3e0a 2020 2020  properties>.    
-00003780: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00003790: 7479 7065 3d22 4d61 7022 3e0a 2020 2020  type="Map">.    
-000037a0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-000037b0: 6e20 7661 6c75 653d 2222 206e 616d 653d  n value="" name=
-000037c0: 226e 616d 6522 2074 7970 653d 2251 5374  "name" type="QSt
-000037d0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-000037e0: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
-000037f0: 6d65 3d22 7072 6f70 6572 7469 6573 2220  me="properties" 
-00003800: 7479 7065 3d22 4d61 7022 3e0a 2020 2020  type="Map">.    
-00003810: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00003820: 696f 6e20 6e61 6d65 3d22 616e 676c 6522  ion name="angle"
-00003830: 2074 7970 653d 224d 6170 223e 0a20 2020   type="Map">.   
-00003840: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00003850: 4f70 7469 6f6e 2076 616c 7565 3d22 7472  Option value="tr
-00003860: 7565 2220 6e61 6d65 3d22 6163 7469 7665  ue" name="active
-00003870: 2220 7479 7065 3d22 626f 6f6c 222f 3e0a  " type="bool"/>.
+00002d40: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+00002d50: 2671 756f 743b 6c61 6e65 5f77 6964 7468  &quot;lane_width
+00002d60: 2671 756f 743b 202a 2031 2e31 2220 6e61  &quot; * 1.1" na
+00002d70: 6d65 3d22 6578 7072 6573 7369 6f6e 2220  me="expression" 
+00002d80: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00002d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002da0: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
+00002db0: 3d22 3322 206e 616d 653d 2274 7970 6522  ="3" name="type"
+00002dc0: 2074 7970 653d 2269 6e74 222f 3e0a 2020   type="int"/>.  
+00002dd0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00002de0: 4f70 7469 6f6e 3e0a 2020 2020 2020 2020  Option>.        
+00002df0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00002e00: 6e61 6d65 3d22 7369 7a65 2220 7479 7065  name="size" type
+00002e10: 3d22 4d61 7022 3e0a 2020 2020 2020 2020  ="Map">.        
+00002e20: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00002e30: 6e20 7661 6c75 653d 2274 7275 6522 206e  n value="true" n
+00002e40: 616d 653d 2261 6374 6976 6522 2074 7970  ame="active" typ
+00002e50: 653d 2262 6f6f 6c22 2f3e 0a20 2020 2020  e="bool"/>.     
+00002e60: 2020 2020 2020 2020 2020 2020 203c 4f70               <Op
+00002e70: 7469 6f6e 2076 616c 7565 3d22 3320 2b20  tion value="3 + 
+00002e80: 3220 2a20 302e 3030 3420 2a20 2040 6d61  2 * 0.004 *  @ma
+00002e90: 705f 7363 616c 6522 206e 616d 653d 2265  p_scale" name="e
+00002ea0: 7870 7265 7373 696f 6e22 2074 7970 653d  xpression" type=
+00002eb0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00002ec0: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
+00002ed0: 7074 696f 6e20 7661 6c75 653d 2233 2220  ption value="3" 
+00002ee0: 6e61 6d65 3d22 7479 7065 2220 7479 7065  name="type" type
+00002ef0: 3d22 696e 7422 2f3e 0a20 2020 2020 2020  ="int"/>.       
+00002f00: 2020 2020 2020 2020 203c 2f4f 7074 696f           </Optio
+00002f10: 6e3e 0a20 2020 2020 2020 2020 2020 2020  n>.             
+00002f20: 203c 2f4f 7074 696f 6e3e 0a20 2020 2020   </Option>.     
+00002f30: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00002f40: 2076 616c 7565 3d22 636f 6c6c 6563 7469   value="collecti
+00002f50: 6f6e 2220 6e61 6d65 3d22 7479 7065 2220  on" name="type" 
+00002f60: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00002f70: 0a20 2020 2020 2020 2020 2020 203c 2f4f  .            </O
+00002f80: 7074 696f 6e3e 0a20 2020 2020 2020 2020  ption>.         
+00002f90: 203c 2f64 6174 615f 6465 6669 6e65 645f   </data_defined_
+00002fa0: 7072 6f70 6572 7469 6573 3e0a 2020 2020  properties>.    
+00002fb0: 2020 2020 3c2f 6c61 7965 723e 0a20 2020      </layer>.   
+00002fc0: 2020 203c 2f73 796d 626f 6c3e 0a20 2020     </symbol>.   
+00002fd0: 2020 203c 7379 6d62 6f6c 2066 7261 6d65     <symbol frame
+00002fe0: 5f72 6174 653d 2231 3022 2069 735f 616e  _rate="10" is_an
+00002ff0: 696d 6174 6564 3d22 3022 206e 616d 653d  imated="0" name=
+00003000: 2231 2220 616c 7068 613d 2231 2220 666f  "1" alpha="1" fo
+00003010: 7263 655f 7268 723d 2230 2220 636c 6970  rce_rhr="0" clip
+00003020: 5f74 6f5f 6578 7465 6e74 3d22 3122 2074  _to_extent="1" t
+00003030: 7970 653d 226d 6172 6b65 7222 3e0a 2020  ype="marker">.  
+00003040: 2020 2020 2020 3c64 6174 615f 6465 6669        <data_defi
+00003050: 6e65 645f 7072 6f70 6572 7469 6573 3e0a  ned_properties>.
+00003060: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00003070: 6e20 7479 7065 3d22 4d61 7022 3e0a 2020  n type="Map">.  
+00003080: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00003090: 6e20 7661 6c75 653d 2222 206e 616d 653d  n value="" name=
+000030a0: 226e 616d 6522 2074 7970 653d 2251 5374  "name" type="QSt
+000030b0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+000030c0: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
+000030d0: 3d22 7072 6f70 6572 7469 6573 222f 3e0a  ="properties"/>.
+000030e0: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+000030f0: 696f 6e20 7661 6c75 653d 2263 6f6c 6c65  ion value="colle
+00003100: 6374 696f 6e22 206e 616d 653d 2274 7970  ction" name="typ
+00003110: 6522 2074 7970 653d 2251 5374 7269 6e67  e" type="QString
+00003120: 222f 3e0a 2020 2020 2020 2020 2020 3c2f  "/>.          </
+00003130: 4f70 7469 6f6e 3e0a 2020 2020 2020 2020  Option>.        
+00003140: 3c2f 6461 7461 5f64 6566 696e 6564 5f70  </data_defined_p
+00003150: 726f 7065 7274 6965 733e 0a20 2020 2020  roperties>.     
+00003160: 2020 203c 6c61 7965 7220 656e 6162 6c65     <layer enable
+00003170: 643d 2231 2220 636c 6173 733d 2253 696d  d="1" class="Sim
+00003180: 706c 654d 6172 6b65 7222 206c 6f63 6b65  pleMarker" locke
+00003190: 643d 2230 2220 7061 7373 3d22 3022 3e0a  d="0" pass="0">.
+000031a0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+000031b0: 6e20 7479 7065 3d22 4d61 7022 3e0a 2020  n type="Map">.  
+000031c0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+000031d0: 6e20 7661 6c75 653d 2230 2220 6e61 6d65  n value="0" name
+000031e0: 3d22 616e 676c 6522 2074 7970 653d 2251  ="angle" type="Q
+000031f0: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+00003200: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
+00003210: 6c75 653d 2266 6c61 7422 206e 616d 653d  lue="flat" name=
+00003220: 2263 6170 5f73 7479 6c65 2220 7479 7065  "cap_style" type
+00003230: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+00003240: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00003250: 2076 616c 7565 3d22 3134 352c 3832 2c34   value="145,82,4
+00003260: 352c 3235 3522 206e 616d 653d 2263 6f6c  5,255" name="col
+00003270: 6f72 2220 7479 7065 3d22 5153 7472 696e  or" type="QStrin
+00003280: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00003290: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+000032a0: 3122 206e 616d 653d 2268 6f72 697a 6f6e  1" name="horizon
+000032b0: 7461 6c5f 616e 6368 6f72 5f70 6f69 6e74  tal_anchor_point
+000032c0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+000032d0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
+000032e0: 4f70 7469 6f6e 2076 616c 7565 3d22 6d69  Option value="mi
+000032f0: 7465 7222 206e 616d 653d 226a 6f69 6e73  ter" name="joins
+00003300: 7479 6c65 2220 7479 7065 3d22 5153 7472  tyle" type="QStr
+00003310: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+00003320: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
+00003330: 3d22 6c69 6e65 2220 6e61 6d65 3d22 6e61  ="line" name="na
+00003340: 6d65 2220 7479 7065 3d22 5153 7472 696e  me" type="QStrin
+00003350: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00003360: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+00003370: 302c 3022 206e 616d 653d 226f 6666 7365  0,0" name="offse
+00003380: 7422 2074 7970 653d 2251 5374 7269 6e67  t" type="QString
+00003390: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+000033a0: 3c4f 7074 696f 6e20 7661 6c75 653d 2233  <Option value="3
+000033b0: 783a 302c 302c 302c 302c 302c 3022 206e  x:0,0,0,0,0,0" n
+000033c0: 616d 653d 226f 6666 7365 745f 6d61 705f  ame="offset_map_
+000033d0: 756e 6974 5f73 6361 6c65 2220 7479 7065  unit_scale" type
+000033e0: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+000033f0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00003400: 2076 616c 7565 3d22 4d4d 2220 6e61 6d65   value="MM" name
+00003410: 3d22 6f66 6673 6574 5f75 6e69 7422 2074  ="offset_unit" t
+00003420: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
+00003430: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00003440: 696f 6e20 7661 6c75 653d 2230 2c30 2c30  ion value="0,0,0
+00003450: 2c32 3535 2220 6e61 6d65 3d22 6f75 746c  ,255" name="outl
+00003460: 696e 655f 636f 6c6f 7222 2074 7970 653d  ine_color" type=
+00003470: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00003480: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00003490: 7661 6c75 653d 2273 6f6c 6964 2220 6e61  value="solid" na
+000034a0: 6d65 3d22 6f75 746c 696e 655f 7374 796c  me="outline_styl
+000034b0: 6522 2074 7970 653d 2251 5374 7269 6e67  e" type="QString
+000034c0: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+000034d0: 3c4f 7074 696f 6e20 7661 6c75 653d 2232  <Option value="2
+000034e0: 2220 6e61 6d65 3d22 6f75 746c 696e 655f  " name="outline_
+000034f0: 7769 6474 6822 2074 7970 653d 2251 5374  width" type="QSt
+00003500: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+00003510: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
+00003520: 653d 2233 783a 302c 302c 302c 302c 302c  e="3x:0,0,0,0,0,
+00003530: 3022 206e 616d 653d 226f 7574 6c69 6e65  0" name="outline
+00003540: 5f77 6964 7468 5f6d 6170 5f75 6e69 745f  _width_map_unit_
+00003550: 7363 616c 6522 2074 7970 653d 2251 5374  scale" type="QSt
+00003560: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+00003570: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
+00003580: 653d 2252 656e 6465 724d 6574 6572 7349  e="RenderMetersI
+00003590: 6e4d 6170 556e 6974 7322 206e 616d 653d  nMapUnits" name=
+000035a0: 226f 7574 6c69 6e65 5f77 6964 7468 5f75  "outline_width_u
+000035b0: 6e69 7422 2074 7970 653d 2251 5374 7269  nit" type="QStri
+000035c0: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+000035d0: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+000035e0: 2264 6961 6d65 7465 7222 206e 616d 653d  "diameter" name=
+000035f0: 2273 6361 6c65 5f6d 6574 686f 6422 2074  "scale_method" t
+00003600: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
+00003610: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00003620: 696f 6e20 7661 6c75 653d 2233 2220 6e61  ion value="3" na
+00003630: 6d65 3d22 7369 7a65 2220 7479 7065 3d22  me="size" type="
+00003640: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+00003650: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
+00003660: 616c 7565 3d22 3378 3a30 2c30 2c30 2c30  alue="3x:0,0,0,0
+00003670: 2c30 2c30 2220 6e61 6d65 3d22 7369 7a65  ,0,0" name="size
+00003680: 5f6d 6170 5f75 6e69 745f 7363 616c 6522  _map_unit_scale"
+00003690: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+000036a0: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
+000036b0: 7074 696f 6e20 7661 6c75 653d 2252 656e  ption value="Ren
+000036c0: 6465 724d 6574 6572 7349 6e4d 6170 556e  derMetersInMapUn
+000036d0: 6974 7322 206e 616d 653d 2273 697a 655f  its" name="size_
+000036e0: 756e 6974 2220 7479 7065 3d22 5153 7472  unit" type="QStr
+000036f0: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+00003700: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
+00003710: 3d22 3122 206e 616d 653d 2276 6572 7469  ="1" name="verti
+00003720: 6361 6c5f 616e 6368 6f72 5f70 6f69 6e74  cal_anchor_point
+00003730: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00003740: 2f3e 0a20 2020 2020 2020 2020 203c 2f4f  />.          </O
+00003750: 7074 696f 6e3e 0a20 2020 2020 2020 2020  ption>.         
+00003760: 203c 6461 7461 5f64 6566 696e 6564 5f70   <data_defined_p
+00003770: 726f 7065 7274 6965 733e 0a20 2020 2020  roperties>.     
+00003780: 2020 2020 2020 203c 4f70 7469 6f6e 2074         <Option t
+00003790: 7970 653d 224d 6170 223e 0a20 2020 2020  ype="Map">.     
+000037a0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+000037b0: 2076 616c 7565 3d22 2220 6e61 6d65 3d22   value="" name="
+000037c0: 6e61 6d65 2220 7479 7065 3d22 5153 7472  name" type="QStr
+000037d0: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+000037e0: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
+000037f0: 653d 2270 726f 7065 7274 6965 7322 2074  e="properties" t
+00003800: 7970 653d 224d 6170 223e 0a20 2020 2020  ype="Map">.     
+00003810: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00003820: 6f6e 206e 616d 653d 2261 6e67 6c65 2220  on name="angle" 
+00003830: 7479 7065 3d22 4d61 7022 3e0a 2020 2020  type="Map">.    
+00003840: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
+00003850: 7074 696f 6e20 7661 6c75 653d 2274 7275  ption value="tru
+00003860: 6522 206e 616d 653d 2261 6374 6976 6522  e" name="active"
+00003870: 2074 7970 653d 2262 6f6f 6c22 2f3e 0a20   type="bool"/>. 
 00003880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003890: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
-000038a0: 2231 3830 202b 2028 2d26 7175 6f74 3b6f  "180 + (-&quot;o
-000038b0: 7269 656e 7461 7469 6f6e 2671 756f 743b  rientation&quot;
-000038c0: 202f 2070 6928 2929 202a 2031 3830 2220   / pi()) * 180" 
-000038d0: 6e61 6d65 3d22 6578 7072 6573 7369 6f6e  name="expression
-000038e0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-000038f0: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
-00003900: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00003910: 7565 3d22 3322 206e 616d 653d 2274 7970  ue="3" name="typ
-00003920: 6522 2074 7970 653d 2269 6e74 222f 3e0a  e" type="int"/>.
-00003930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003940: 3c2f 4f70 7469 6f6e 3e0a 2020 2020 2020  </Option>.      
-00003950: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00003960: 6e20 6e61 6d65 3d22 6f75 746c 696e 6557  n name="outlineW
-00003970: 6964 7468 2220 7479 7065 3d22 4d61 7022  idth" type="Map"
-00003980: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00003990: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-000039a0: 653d 2274 7275 6522 206e 616d 653d 2261  e="true" name="a
-000039b0: 6374 6976 6522 2074 7970 653d 2262 6f6f  ctive" type="boo
-000039c0: 6c22 2f3e 0a20 2020 2020 2020 2020 2020  l"/>.           
-000039d0: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-000039e0: 616c 7565 3d22 2671 756f 743b 6c61 6e65  alue="&quot;lane
-000039f0: 5f77 6964 7468 2671 756f 743b 202a 2030  _width&quot; * 0
-00003a00: 2e37 2220 6e61 6d65 3d22 6578 7072 6573  .7" name="expres
-00003a10: 7369 6f6e 2220 7479 7065 3d22 5153 7472  sion" type="QStr
-00003a20: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-00003a30: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-00003a40: 2076 616c 7565 3d22 3322 206e 616d 653d   value="3" name=
-00003a50: 2274 7970 6522 2074 7970 653d 2269 6e74  "type" type="int
-00003a60: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00003a70: 2020 2020 3c2f 4f70 7469 6f6e 3e0a 2020      </Option>.  
-00003a80: 2020 2020 2020 2020 2020 2020 3c2f 4f70              </Op
-00003a90: 7469 6f6e 3e0a 2020 2020 2020 2020 2020  tion>.          
-00003aa0: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-00003ab0: 653d 2263 6f6c 6c65 6374 696f 6e22 206e  e="collection" n
-00003ac0: 616d 653d 2274 7970 6522 2074 7970 653d  ame="type" type=
-00003ad0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-00003ae0: 2020 2020 2020 2020 3c2f 4f70 7469 6f6e          </Option
-00003af0: 3e0a 2020 2020 2020 2020 2020 3c2f 6461  >.          </da
-00003b00: 7461 5f64 6566 696e 6564 5f70 726f 7065  ta_defined_prope
-00003b10: 7274 6965 733e 0a20 2020 2020 2020 203c  rties>.        <
-00003b20: 2f6c 6179 6572 3e0a 2020 2020 2020 3c2f  /layer>.      </
-00003b30: 7379 6d62 6f6c 3e0a 2020 2020 2020 3c73  symbol>.      <s
-00003b40: 796d 626f 6c20 6672 616d 655f 7261 7465  ymbol frame_rate
-00003b50: 3d22 3130 2220 6973 5f61 6e69 6d61 7465  ="10" is_animate
-00003b60: 643d 2230 2220 6e61 6d65 3d22 3222 2061  d="0" name="2" a
-00003b70: 6c70 6861 3d22 3122 2066 6f72 6365 5f72  lpha="1" force_r
-00003b80: 6872 3d22 3022 2063 6c69 705f 746f 5f65  hr="0" clip_to_e
-00003b90: 7874 656e 743d 2231 2220 7479 7065 3d22  xtent="1" type="
-00003ba0: 6d61 726b 6572 223e 0a20 2020 2020 2020  marker">.       
-00003bb0: 203c 6461 7461 5f64 6566 696e 6564 5f70   <data_defined_p
-00003bc0: 726f 7065 7274 6965 733e 0a20 2020 2020  roperties>.     
-00003bd0: 2020 2020 203c 4f70 7469 6f6e 2074 7970       <Option typ
-00003be0: 653d 224d 6170 223e 0a20 2020 2020 2020  e="Map">.       
-00003bf0: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00003c00: 7565 3d22 2220 6e61 6d65 3d22 6e61 6d65  ue="" name="name
-00003c10: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00003c20: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-00003c30: 4f70 7469 6f6e 206e 616d 653d 2270 726f  Option name="pro
-00003c40: 7065 7274 6965 7322 2f3e 0a20 2020 2020  perties"/>.     
-00003c50: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-00003c60: 616c 7565 3d22 636f 6c6c 6563 7469 6f6e  alue="collection
-00003c70: 2220 6e61 6d65 3d22 7479 7065 2220 7479  " name="type" ty
-00003c80: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
-00003c90: 2020 2020 2020 2020 203c 2f4f 7074 696f           </Optio
-00003ca0: 6e3e 0a20 2020 2020 2020 203c 2f64 6174  n>.        </dat
-00003cb0: 615f 6465 6669 6e65 645f 7072 6f70 6572  a_defined_proper
-00003cc0: 7469 6573 3e0a 2020 2020 2020 2020 3c6c  ties>.        <l
-00003cd0: 6179 6572 2065 6e61 626c 6564 3d22 3122  ayer enabled="1"
-00003ce0: 2063 6c61 7373 3d22 5369 6d70 6c65 4d61   class="SimpleMa
-00003cf0: 726b 6572 2220 6c6f 636b 6564 3d22 3022  rker" locked="0"
-00003d00: 2070 6173 733d 2230 223e 0a20 2020 2020   pass="0">.     
-00003d10: 2020 2020 203c 4f70 7469 6f6e 2074 7970       <Option typ
-00003d20: 653d 224d 6170 223e 0a20 2020 2020 2020  e="Map">.       
-00003d30: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00003d40: 7565 3d22 3022 206e 616d 653d 2261 6e67  ue="0" name="ang
-00003d50: 6c65 2220 7479 7065 3d22 5153 7472 696e  le" type="QStrin
-00003d60: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
-00003d70: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-00003d80: 666c 6174 2220 6e61 6d65 3d22 6361 705f  flat" name="cap_
-00003d90: 7374 796c 6522 2074 7970 653d 2251 5374  style" type="QSt
-00003da0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-00003db0: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-00003dc0: 653d 2232 3332 2c38 352c 302c 3235 3522  e="232,85,0,255"
-00003dd0: 206e 616d 653d 2263 6f6c 6f72 2220 7479   name="color" ty
-00003de0: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
-00003df0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00003e00: 6f6e 2076 616c 7565 3d22 3122 206e 616d  on value="1" nam
-00003e10: 653d 2268 6f72 697a 6f6e 7461 6c5f 616e  e="horizontal_an
-00003e20: 6368 6f72 5f70 6f69 6e74 2220 7479 7065  chor_point" type
-00003e30: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-00003e40: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-00003e50: 2076 616c 7565 3d22 6265 7665 6c22 206e   value="bevel" n
-00003e60: 616d 653d 226a 6f69 6e73 7479 6c65 2220  ame="joinstyle" 
-00003e70: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
-00003e80: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
-00003e90: 7469 6f6e 2076 616c 7565 3d22 6c69 6e65  tion value="line
-00003ea0: 2220 6e61 6d65 3d22 6e61 6d65 2220 7479  " name="name" ty
-00003eb0: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
-00003ec0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00003ed0: 6f6e 2076 616c 7565 3d22 302c 3022 206e  on value="0,0" n
-00003ee0: 616d 653d 226f 6666 7365 7422 2074 7970  ame="offset" typ
-00003ef0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00003f00: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00003f10: 6e20 7661 6c75 653d 2233 783a 302c 302c  n value="3x:0,0,
-00003f20: 302c 302c 302c 3022 206e 616d 653d 226f  0,0,0,0" name="o
-00003f30: 6666 7365 745f 6d61 705f 756e 6974 5f73  ffset_map_unit_s
-00003f40: 6361 6c65 2220 7479 7065 3d22 5153 7472  cale" type="QStr
-00003f50: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-00003f60: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
-00003f70: 3d22 4d4d 2220 6e61 6d65 3d22 6f66 6673  ="MM" name="offs
-00003f80: 6574 5f75 6e69 7422 2074 7970 653d 2251  et_unit" type="Q
-00003f90: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
-00003fa0: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
-00003fb0: 6c75 653d 2232 3535 2c32 3535 2c32 3535  lue="255,255,255
-00003fc0: 2c32 3535 2220 6e61 6d65 3d22 6f75 746c  ,255" name="outl
-00003fd0: 696e 655f 636f 6c6f 7222 2074 7970 653d  ine_color" type=
-00003fe0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-00003ff0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00004000: 7661 6c75 653d 2273 6f6c 6964 2220 6e61  value="solid" na
-00004010: 6d65 3d22 6f75 746c 696e 655f 7374 796c  me="outline_styl
-00004020: 6522 2074 7970 653d 2251 5374 7269 6e67  e" type="QString
-00004030: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00004040: 3c4f 7074 696f 6e20 7661 6c75 653d 2232  <Option value="2
-00004050: 2220 6e61 6d65 3d22 6f75 746c 696e 655f  " name="outline_
-00004060: 7769 6474 6822 2074 7970 653d 2251 5374  width" type="QSt
-00004070: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-00004080: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-00004090: 653d 2233 783a 302c 302c 302c 302c 302c  e="3x:0,0,0,0,0,
-000040a0: 3022 206e 616d 653d 226f 7574 6c69 6e65  0" name="outline
-000040b0: 5f77 6964 7468 5f6d 6170 5f75 6e69 745f  _width_map_unit_
-000040c0: 7363 616c 6522 2074 7970 653d 2251 5374  scale" type="QSt
-000040d0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-000040e0: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-000040f0: 653d 2252 656e 6465 724d 6574 6572 7349  e="RenderMetersI
-00004100: 6e4d 6170 556e 6974 7322 206e 616d 653d  nMapUnits" name=
-00004110: 226f 7574 6c69 6e65 5f77 6964 7468 5f75  "outline_width_u
-00004120: 6e69 7422 2074 7970 653d 2251 5374 7269  nit" type="QStri
-00004130: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
-00004140: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
-00004150: 2264 6961 6d65 7465 7222 206e 616d 653d  "diameter" name=
-00004160: 2273 6361 6c65 5f6d 6574 686f 6422 2074  "scale_method" t
-00004170: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
-00004180: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00004190: 696f 6e20 7661 6c75 653d 2233 2220 6e61  ion value="3" na
-000041a0: 6d65 3d22 7369 7a65 2220 7479 7065 3d22  me="size" type="
-000041b0: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-000041c0: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-000041d0: 616c 7565 3d22 3378 3a30 2c30 2c30 2c30  alue="3x:0,0,0,0
-000041e0: 2c30 2c30 2220 6e61 6d65 3d22 7369 7a65  ,0,0" name="size
-000041f0: 5f6d 6170 5f75 6e69 745f 7363 616c 6522  _map_unit_scale"
-00004200: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-00004210: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
-00004220: 7074 696f 6e20 7661 6c75 653d 2252 656e  ption value="Ren
-00004230: 6465 724d 6574 6572 7349 6e4d 6170 556e  derMetersInMapUn
-00004240: 6974 7322 206e 616d 653d 2273 697a 655f  its" name="size_
-00004250: 756e 6974 2220 7479 7065 3d22 5153 7472  unit" type="QStr
-00004260: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-00004270: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
-00004280: 3d22 3122 206e 616d 653d 2276 6572 7469  ="1" name="verti
-00004290: 6361 6c5f 616e 6368 6f72 5f70 6f69 6e74  cal_anchor_point
-000042a0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-000042b0: 2f3e 0a20 2020 2020 2020 2020 203c 2f4f  />.          </O
-000042c0: 7074 696f 6e3e 0a20 2020 2020 2020 2020  ption>.         
-000042d0: 203c 6461 7461 5f64 6566 696e 6564 5f70   <data_defined_p
-000042e0: 726f 7065 7274 6965 733e 0a20 2020 2020  roperties>.     
-000042f0: 2020 2020 2020 203c 4f70 7469 6f6e 2074         <Option t
-00004300: 7970 653d 224d 6170 223e 0a20 2020 2020  ype="Map">.     
-00004310: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-00004320: 2076 616c 7565 3d22 2220 6e61 6d65 3d22   value="" name="
-00004330: 6e61 6d65 2220 7479 7065 3d22 5153 7472  name" type="QStr
-00004340: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-00004350: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
-00004360: 653d 2270 726f 7065 7274 6965 7322 2074  e="properties" t
-00004370: 7970 653d 224d 6170 223e 0a20 2020 2020  ype="Map">.     
-00004380: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00004390: 6f6e 206e 616d 653d 2261 6e67 6c65 2220  on name="angle" 
-000043a0: 7479 7065 3d22 4d61 7022 3e0a 2020 2020  type="Map">.    
-000043b0: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
-000043c0: 7074 696f 6e20 7661 6c75 653d 2274 7275  ption value="tru
-000043d0: 6522 206e 616d 653d 2261 6374 6976 6522  e" name="active"
-000043e0: 2074 7970 653d 2262 6f6f 6c22 2f3e 0a20   type="bool"/>. 
-000043f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004400: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-00004410: 3138 3020 2b20 282d 2671 756f 743b 6f72  180 + (-&quot;or
-00004420: 6965 6e74 6174 696f 6e26 7175 6f74 3b20  ientation&quot; 
-00004430: 2f20 7069 2829 2920 2a20 3138 3022 206e  / pi()) * 180" n
-00004440: 616d 653d 2265 7870 7265 7373 696f 6e22  ame="expression"
-00004450: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-00004460: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00004470: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-00004480: 653d 2233 2220 6e61 6d65 3d22 7479 7065  e="3" name="type
-00004490: 2220 7479 7065 3d22 696e 7422 2f3e 0a20  " type="int"/>. 
-000044a0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000044b0: 2f4f 7074 696f 6e3e 0a20 2020 2020 2020  /Option>.       
-000044c0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-000044d0: 206e 616d 653d 226f 7574 6c69 6e65 5769   name="outlineWi
-000044e0: 6474 6822 2074 7970 653d 224d 6170 223e  dth" type="Map">
-000044f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004500: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
-00004510: 3d22 7472 7565 2220 6e61 6d65 3d22 6163  ="true" name="ac
-00004520: 7469 7665 2220 7479 7065 3d22 626f 6f6c  tive" type="bool
-00004530: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00004540: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
-00004550: 6c75 653d 2226 7175 6f74 3b6c 616e 655f  lue="&quot;lane_
-00004560: 7769 6474 6826 7175 6f74 3b22 206e 616d  width&quot;" nam
-00004570: 653d 2265 7870 7265 7373 696f 6e22 2074  e="expression" t
-00004580: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
-00004590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045a0: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
-000045b0: 2233 2220 6e61 6d65 3d22 7479 7065 2220  "3" name="type" 
-000045c0: 7479 7065 3d22 696e 7422 2f3e 0a20 2020  type="int"/>.   
-000045d0: 2020 2020 2020 2020 2020 2020 203c 2f4f               </O
-000045e0: 7074 696f 6e3e 0a20 2020 2020 2020 2020  ption>.         
-000045f0: 2020 2020 2020 203c 4f70 7469 6f6e 206e         <Option n
-00004600: 616d 653d 2273 697a 6522 2074 7970 653d  ame="size" type=
-00004610: 224d 6170 223e 0a20 2020 2020 2020 2020  "Map">.         
-00004620: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-00004630: 2076 616c 7565 3d22 7472 7565 2220 6e61   value="true" na
-00004640: 6d65 3d22 6163 7469 7665 2220 7479 7065  me="active" type
-00004650: 3d22 626f 6f6c 222f 3e0a 2020 2020 2020  ="bool"/>.      
-00004660: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00004670: 696f 6e20 7661 6c75 653d 2233 202d 2032  ion value="3 - 2
-00004680: 202a 2030 2e30 3031 202a 2040 6d61 705f   * 0.001 * @map_
-00004690: 7363 616c 6522 206e 616d 653d 2265 7870  scale" name="exp
-000046a0: 7265 7373 696f 6e22 2074 7970 653d 2251  ression" type="Q
-000046b0: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
-000046c0: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-000046d0: 696f 6e20 7661 6c75 653d 2233 2220 6e61  ion value="3" na
-000046e0: 6d65 3d22 7479 7065 2220 7479 7065 3d22  me="type" type="
-000046f0: 696e 7422 2f3e 0a20 2020 2020 2020 2020  int"/>.         
-00004700: 2020 2020 2020 203c 2f4f 7074 696f 6e3e         </Option>
-00004710: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-00004720: 2f4f 7074 696f 6e3e 0a20 2020 2020 2020  /Option>.       
-00004730: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-00004740: 616c 7565 3d22 636f 6c6c 6563 7469 6f6e  alue="collection
-00004750: 2220 6e61 6d65 3d22 7479 7065 2220 7479  " name="type" ty
-00004760: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
-00004770: 2020 2020 2020 2020 2020 203c 2f4f 7074             </Opt
-00004780: 696f 6e3e 0a20 2020 2020 2020 2020 203c  ion>.          <
-00004790: 2f64 6174 615f 6465 6669 6e65 645f 7072  /data_defined_pr
-000047a0: 6f70 6572 7469 6573 3e0a 2020 2020 2020  operties>.      
-000047b0: 2020 3c2f 6c61 7965 723e 0a20 2020 2020    </layer>.     
-000047c0: 203c 2f73 796d 626f 6c3e 0a20 2020 2020   </symbol>.     
-000047d0: 203c 7379 6d62 6f6c 2066 7261 6d65 5f72   <symbol frame_r
-000047e0: 6174 653d 2231 3022 2069 735f 616e 696d  ate="10" is_anim
-000047f0: 6174 6564 3d22 3022 206e 616d 653d 2233  ated="0" name="3
-00004800: 2220 616c 7068 613d 2231 2220 666f 7263  " alpha="1" forc
-00004810: 655f 7268 723d 2230 2220 636c 6970 5f74  e_rhr="0" clip_t
-00004820: 6f5f 6578 7465 6e74 3d22 3122 2074 7970  o_extent="1" typ
-00004830: 653d 226d 6172 6b65 7222 3e0a 2020 2020  e="marker">.    
-00004840: 2020 2020 3c64 6174 615f 6465 6669 6e65      <data_define
-00004850: 645f 7072 6f70 6572 7469 6573 3e0a 2020  d_properties>.  
-00004860: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00004870: 7479 7065 3d22 4d61 7022 3e0a 2020 2020  type="Map">.    
-00004880: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00004890: 7661 6c75 653d 2222 206e 616d 653d 226e  value="" name="n
-000048a0: 616d 6522 2074 7970 653d 2251 5374 7269  ame" type="QStri
-000048b0: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
-000048c0: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
-000048d0: 7072 6f70 6572 7469 6573 222f 3e0a 2020  properties"/>.  
-000048e0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-000048f0: 6e20 7661 6c75 653d 2263 6f6c 6c65 6374  n value="collect
-00004900: 696f 6e22 206e 616d 653d 2274 7970 6522  ion" name="type"
-00004910: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-00004920: 3e0a 2020 2020 2020 2020 2020 3c2f 4f70  >.          </Op
-00004930: 7469 6f6e 3e0a 2020 2020 2020 2020 3c2f  tion>.        </
-00004940: 6461 7461 5f64 6566 696e 6564 5f70 726f  data_defined_pro
-00004950: 7065 7274 6965 733e 0a20 2020 2020 2020  perties>.       
-00004960: 203c 6c61 7965 7220 656e 6162 6c65 643d   <layer enabled=
-00004970: 2231 2220 636c 6173 733d 2253 696d 706c  "1" class="Simpl
-00004980: 654d 6172 6b65 7222 206c 6f63 6b65 643d  eMarker" locked=
-00004990: 2230 2220 7061 7373 3d22 3022 3e0a 2020  "0" pass="0">.  
-000049a0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-000049b0: 7479 7065 3d22 4d61 7022 3e0a 2020 2020  type="Map">.    
-000049c0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-000049d0: 7661 6c75 653d 2230 2220 6e61 6d65 3d22  value="0" name="
-000049e0: 616e 676c 6522 2074 7970 653d 2251 5374  angle" type="QSt
-000049f0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-00004a00: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-00004a10: 653d 2266 6c61 7422 206e 616d 653d 2263  e="flat" name="c
-00004a20: 6170 5f73 7479 6c65 2220 7479 7065 3d22  ap_style" type="
-00004a30: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-00004a40: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-00004a50: 616c 7565 3d22 3233 322c 3835 2c30 2c32  alue="232,85,0,2
-00004a60: 3535 2220 6e61 6d65 3d22 636f 6c6f 7222  55" name="color"
-00004a70: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-00004a80: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
-00004a90: 7074 696f 6e20 7661 6c75 653d 2231 2220  ption value="1" 
-00004aa0: 6e61 6d65 3d22 686f 7269 7a6f 6e74 616c  name="horizontal
-00004ab0: 5f61 6e63 686f 725f 706f 696e 7422 2074  _anchor_point" t
-00004ac0: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
-00004ad0: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00004ae0: 696f 6e20 7661 6c75 653d 2262 6576 656c  ion value="bevel
-00004af0: 2220 6e61 6d65 3d22 6a6f 696e 7374 796c  " name="joinstyl
-00004b00: 6522 2074 7970 653d 2251 5374 7269 6e67  e" type="QString
-00004b10: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00004b20: 3c4f 7074 696f 6e20 7661 6c75 653d 226c  <Option value="l
-00004b30: 696e 6522 206e 616d 653d 226e 616d 6522  ine" name="name"
-00004b40: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-00004b50: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
-00004b60: 7074 696f 6e20 7661 6c75 653d 2230 2c30  ption value="0,0
-00004b70: 2220 6e61 6d65 3d22 6f66 6673 6574 2220  " name="offset" 
-00004b80: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
-00004b90: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
-00004ba0: 7469 6f6e 2076 616c 7565 3d22 3378 3a30  tion value="3x:0
-00004bb0: 2c30 2c30 2c30 2c30 2c30 2220 6e61 6d65  ,0,0,0,0,0" name
-00004bc0: 3d22 6f66 6673 6574 5f6d 6170 5f75 6e69  ="offset_map_uni
-00004bd0: 745f 7363 616c 6522 2074 7970 653d 2251  t_scale" type="Q
-00004be0: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
-00004bf0: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
-00004c00: 6c75 653d 224d 4d22 206e 616d 653d 226f  lue="MM" name="o
-00004c10: 6666 7365 745f 756e 6974 2220 7479 7065  ffset_unit" type
-00004c20: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-00004c30: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-00004c40: 2076 616c 7565 3d22 3235 352c 3235 352c   value="255,255,
-00004c50: 3235 352c 3235 3522 206e 616d 653d 226f  255,255" name="o
-00004c60: 7574 6c69 6e65 5f63 6f6c 6f72 2220 7479  utline_color" ty
-00004c70: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
-00004c80: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00004c90: 6f6e 2076 616c 7565 3d22 736f 6c69 6422  on value="solid"
-00004ca0: 206e 616d 653d 226f 7574 6c69 6e65 5f73   name="outline_s
-00004cb0: 7479 6c65 2220 7479 7065 3d22 5153 7472  tyle" type="QStr
-00004cc0: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-00004cd0: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
-00004ce0: 3d22 3222 206e 616d 653d 226f 7574 6c69  ="2" name="outli
-00004cf0: 6e65 5f77 6964 7468 2220 7479 7065 3d22  ne_width" type="
-00004d00: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-00004d10: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-00004d20: 616c 7565 3d22 3378 3a30 2c30 2c30 2c30  alue="3x:0,0,0,0
-00004d30: 2c30 2c30 2220 6e61 6d65 3d22 6f75 746c  ,0,0" name="outl
-00004d40: 696e 655f 7769 6474 685f 6d61 705f 756e  ine_width_map_un
-00004d50: 6974 5f73 6361 6c65 2220 7479 7065 3d22  it_scale" type="
-00004d60: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-00004d70: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-00004d80: 616c 7565 3d22 5265 6e64 6572 4d65 7465  alue="RenderMete
-00004d90: 7273 496e 4d61 7055 6e69 7473 2220 6e61  rsInMapUnits" na
-00004da0: 6d65 3d22 6f75 746c 696e 655f 7769 6474  me="outline_widt
-00004db0: 685f 756e 6974 2220 7479 7065 3d22 5153  h_unit" type="QS
-00004dc0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00004dd0: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00004de0: 7565 3d22 6469 616d 6574 6572 2220 6e61  ue="diameter" na
-00004df0: 6d65 3d22 7363 616c 655f 6d65 7468 6f64  me="scale_method
-00004e00: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00004e10: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-00004e20: 4f70 7469 6f6e 2076 616c 7565 3d22 3322  Option value="3"
-00004e30: 206e 616d 653d 2273 697a 6522 2074 7970   name="size" typ
-00004e40: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00004e50: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00004e60: 6e20 7661 6c75 653d 2233 783a 302c 302c  n value="3x:0,0,
-00004e70: 302c 302c 302c 3022 206e 616d 653d 2273  0,0,0,0" name="s
-00004e80: 697a 655f 6d61 705f 756e 6974 5f73 6361  ize_map_unit_sca
-00004e90: 6c65 2220 7479 7065 3d22 5153 7472 696e  le" type="QStrin
-00004ea0: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
-00004eb0: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-00004ec0: 5265 6e64 6572 4d65 7465 7273 496e 4d61  RenderMetersInMa
-00004ed0: 7055 6e69 7473 2220 6e61 6d65 3d22 7369  pUnits" name="si
-00004ee0: 7a65 5f75 6e69 7422 2074 7970 653d 2251  ze_unit" type="Q
-00004ef0: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
-00004f00: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
-00004f10: 6c75 653d 2231 2220 6e61 6d65 3d22 7665  lue="1" name="ve
-00004f20: 7274 6963 616c 5f61 6e63 686f 725f 706f  rtical_anchor_po
-00004f30: 696e 7422 2074 7970 653d 2251 5374 7269  int" type="QStri
-00004f40: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
-00004f50: 3c2f 4f70 7469 6f6e 3e0a 2020 2020 2020  </Option>.      
-00004f60: 2020 2020 3c64 6174 615f 6465 6669 6e65      <data_define
-00004f70: 645f 7072 6f70 6572 7469 6573 3e0a 2020  d_properties>.  
-00004f80: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00004f90: 6e20 7479 7065 3d22 4d61 7022 3e0a 2020  n type="Map">.  
-00004fa0: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00004fb0: 696f 6e20 7661 6c75 653d 2222 206e 616d  ion value="" nam
-00004fc0: 653d 226e 616d 6522 2074 7970 653d 2251  e="name" type="Q
-00004fd0: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
-00004fe0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00004ff0: 6e61 6d65 3d22 7072 6f70 6572 7469 6573  name="properties
-00005000: 2220 7479 7065 3d22 4d61 7022 3e0a 2020  " type="Map">.  
-00005010: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
-00005020: 7074 696f 6e20 6e61 6d65 3d22 616e 676c  ption name="angl
-00005030: 6522 2074 7970 653d 224d 6170 223e 0a20  e" type="Map">. 
-00005040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005050: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-00005060: 7472 7565 2220 6e61 6d65 3d22 6163 7469  true" name="acti
-00005070: 7665 2220 7479 7065 3d22 626f 6f6c 222f  ve" type="bool"/
-00005080: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00005090: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-000050a0: 653d 2231 3830 202b 2028 2d26 7175 6f74  e="180 + (-&quot
-000050b0: 3b6f 7269 656e 7461 7469 6f6e 2671 756f  ;orientation&quo
-000050c0: 743b 202f 2070 6928 2929 202a 2031 3830  t; / pi()) * 180
-000050d0: 2220 6e61 6d65 3d22 6578 7072 6573 7369  " name="expressi
-000050e0: 6f6e 2220 7479 7065 3d22 5153 7472 696e  on" type="QStrin
-000050f0: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
-00005100: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-00005110: 616c 7565 3d22 3322 206e 616d 653d 2274  alue="3" name="t
-00005120: 7970 6522 2074 7970 653d 2269 6e74 222f  ype" type="int"/
-00005130: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00005140: 2020 3c2f 4f70 7469 6f6e 3e0a 2020 2020    </Option>.    
-00005150: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00005160: 696f 6e20 6e61 6d65 3d22 6f75 746c 696e  ion name="outlin
-00005170: 6557 6964 7468 2220 7479 7065 3d22 4d61  eWidth" type="Ma
-00005180: 7022 3e0a 2020 2020 2020 2020 2020 2020  p">.            
-00005190: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
-000051a0: 6c75 653d 2274 7275 6522 206e 616d 653d  lue="true" name=
-000051b0: 2261 6374 6976 6522 2074 7970 653d 2262  "active" type="b
-000051c0: 6f6f 6c22 2f3e 0a20 2020 2020 2020 2020  ool"/>.         
-000051d0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-000051e0: 2076 616c 7565 3d22 2671 756f 743b 6c61   value="&quot;la
-000051f0: 6e65 5f77 6964 7468 2671 756f 743b 2220  ne_width&quot;" 
-00005200: 6e61 6d65 3d22 6578 7072 6573 7369 6f6e  name="expression
-00005210: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00005220: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
-00005230: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00005240: 7565 3d22 3322 206e 616d 653d 2274 7970  ue="3" name="typ
-00005250: 6522 2074 7970 653d 2269 6e74 222f 3e0a  e" type="int"/>.
-00005260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005270: 3c2f 4f70 7469 6f6e 3e0a 2020 2020 2020  </Option>.      
-00005280: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00005290: 6e20 6e61 6d65 3d22 7369 7a65 2220 7479  n name="size" ty
-000052a0: 7065 3d22 4d61 7022 3e0a 2020 2020 2020  pe="Map">.      
-000052b0: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-000052c0: 696f 6e20 7661 6c75 653d 2274 7275 6522  ion value="true"
-000052d0: 206e 616d 653d 2261 6374 6976 6522 2074   name="active" t
-000052e0: 7970 653d 2262 6f6f 6c22 2f3e 0a20 2020  ype="bool"/>.   
-000052f0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00005300: 4f70 7469 6f6e 2076 616c 7565 3d22 3320  Option value="3 
-00005310: 2d20 3220 2a20 302e 3030 3220 2a20 406d  - 2 * 0.002 * @m
-00005320: 6170 5f73 6361 6c65 2220 6e61 6d65 3d22  ap_scale" name="
-00005330: 6578 7072 6573 7369 6f6e 2220 7479 7065  expression" type
-00005340: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-00005350: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00005360: 4f70 7469 6f6e 2076 616c 7565 3d22 3322  Option value="3"
-00005370: 206e 616d 653d 2274 7970 6522 2074 7970   name="type" typ
-00005380: 653d 2269 6e74 222f 3e0a 2020 2020 2020  e="int"/>.      
-00005390: 2020 2020 2020 2020 2020 3c2f 4f70 7469            </Opti
-000053a0: 6f6e 3e0a 2020 2020 2020 2020 2020 2020  on>.            
-000053b0: 2020 3c2f 4f70 7469 6f6e 3e0a 2020 2020    </Option>.    
-000053c0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-000053d0: 6e20 7661 6c75 653d 2263 6f6c 6c65 6374  n value="collect
-000053e0: 696f 6e22 206e 616d 653d 2274 7970 6522  ion" name="type"
-000053f0: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-00005400: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
-00005410: 4f70 7469 6f6e 3e0a 2020 2020 2020 2020  Option>.        
-00005420: 2020 3c2f 6461 7461 5f64 6566 696e 6564    </data_defined
-00005430: 5f70 726f 7065 7274 6965 733e 0a20 2020  _properties>.   
-00005440: 2020 2020 203c 2f6c 6179 6572 3e0a 2020       </layer>.  
-00005450: 2020 2020 3c2f 7379 6d62 6f6c 3e0a 2020      </symbol>.  
-00005460: 2020 2020 3c73 796d 626f 6c20 6672 616d      <symbol fram
-00005470: 655f 7261 7465 3d22 3130 2220 6973 5f61  e_rate="10" is_a
-00005480: 6e69 6d61 7465 643d 2230 2220 6e61 6d65  nimated="0" name
-00005490: 3d22 3422 2061 6c70 6861 3d22 3122 2066  ="4" alpha="1" f
-000054a0: 6f72 6365 5f72 6872 3d22 3022 2063 6c69  orce_rhr="0" cli
-000054b0: 705f 746f 5f65 7874 656e 743d 2231 2220  p_to_extent="1" 
-000054c0: 7479 7065 3d22 6d61 726b 6572 223e 0a20  type="marker">. 
-000054d0: 2020 2020 2020 203c 6461 7461 5f64 6566         <data_def
-000054e0: 696e 6564 5f70 726f 7065 7274 6965 733e  ined_properties>
-000054f0: 0a20 2020 2020 2020 2020 203c 4f70 7469  .          <Opti
-00005500: 6f6e 2074 7970 653d 224d 6170 223e 0a20  on type="Map">. 
-00005510: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00005520: 6f6e 2076 616c 7565 3d22 2220 6e61 6d65  on value="" name
-00005530: 3d22 6e61 6d65 2220 7479 7065 3d22 5153  ="name" type="QS
-00005540: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00005550: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
-00005560: 653d 2270 726f 7065 7274 6965 7322 2f3e  e="properties"/>
-00005570: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
-00005580: 7469 6f6e 2076 616c 7565 3d22 636f 6c6c  tion value="coll
-00005590: 6563 7469 6f6e 2220 6e61 6d65 3d22 7479  ection" name="ty
-000055a0: 7065 2220 7479 7065 3d22 5153 7472 696e  pe" type="QStrin
-000055b0: 6722 2f3e 0a20 2020 2020 2020 2020 203c  g"/>.          <
-000055c0: 2f4f 7074 696f 6e3e 0a20 2020 2020 2020  /Option>.       
-000055d0: 203c 2f64 6174 615f 6465 6669 6e65 645f   </data_defined_
-000055e0: 7072 6f70 6572 7469 6573 3e0a 2020 2020  properties>.    
-000055f0: 2020 2020 3c6c 6179 6572 2065 6e61 626c      <layer enabl
-00005600: 6564 3d22 3122 2063 6c61 7373 3d22 5369  ed="1" class="Si
-00005610: 6d70 6c65 4d61 726b 6572 2220 6c6f 636b  mpleMarker" lock
-00005620: 6564 3d22 3022 2070 6173 733d 2230 223e  ed="0" pass="0">
-00005630: 0a20 2020 2020 2020 2020 203c 4f70 7469  .          <Opti
-00005640: 6f6e 2074 7970 653d 224d 6170 223e 0a20  on type="Map">. 
-00005650: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00005660: 6f6e 2076 616c 7565 3d22 3022 206e 616d  on value="0" nam
-00005670: 653d 2261 6e67 6c65 2220 7479 7065 3d22  e="angle" type="
-00005680: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-00005690: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-000056a0: 616c 7565 3d22 7371 7561 7265 2220 6e61  alue="square" na
-000056b0: 6d65 3d22 6361 705f 7374 796c 6522 2074  me="cap_style" t
-000056c0: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
-000056d0: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-000056e0: 696f 6e20 7661 6c75 653d 2230 2c30 2c30  ion value="0,0,0
-000056f0: 2c32 3535 2220 6e61 6d65 3d22 636f 6c6f  ,255" name="colo
-00005700: 7222 2074 7970 653d 2251 5374 7269 6e67  r" type="QString
-00005710: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00005720: 3c4f 7074 696f 6e20 7661 6c75 653d 2231  <Option value="1
-00005730: 2220 6e61 6d65 3d22 686f 7269 7a6f 6e74  " name="horizont
-00005740: 616c 5f61 6e63 686f 725f 706f 696e 7422  al_anchor_point"
-00005750: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-00005760: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
-00005770: 7074 696f 6e20 7661 6c75 653d 226d 6974  ption value="mit
-00005780: 6572 2220 6e61 6d65 3d22 6a6f 696e 7374  er" name="joinst
-00005790: 796c 6522 2074 7970 653d 2251 5374 7269  yle" type="QStri
-000057a0: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
-000057b0: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
-000057c0: 2263 6972 636c 6522 206e 616d 653d 226e  "circle" name="n
-000057d0: 616d 6522 2074 7970 653d 2251 5374 7269  ame" type="QStri
-000057e0: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
-000057f0: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
-00005800: 2230 2c30 2220 6e61 6d65 3d22 6f66 6673  "0,0" name="offs
-00005810: 6574 2220 7479 7065 3d22 5153 7472 696e  et" type="QStrin
-00005820: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
-00005830: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-00005840: 3378 3a30 2c30 2c30 2c30 2c30 2c30 2220  3x:0,0,0,0,0,0" 
-00005850: 6e61 6d65 3d22 6f66 6673 6574 5f6d 6170  name="offset_map
-00005860: 5f75 6e69 745f 7363 616c 6522 2074 7970  _unit_scale" typ
-00005870: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00005880: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00005890: 6e20 7661 6c75 653d 2252 656e 6465 724d  n value="RenderM
-000058a0: 6574 6572 7349 6e4d 6170 556e 6974 7322  etersInMapUnits"
-000058b0: 206e 616d 653d 226f 6666 7365 745f 756e   name="offset_un
-000058c0: 6974 2220 7479 7065 3d22 5153 7472 696e  it" type="QStrin
-000058d0: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
-000058e0: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-000058f0: 3335 2c33 352c 3335 2c32 3535 2220 6e61  35,35,35,255" na
-00005900: 6d65 3d22 6f75 746c 696e 655f 636f 6c6f  me="outline_colo
-00005910: 7222 2074 7970 653d 2251 5374 7269 6e67  r" type="QString
-00005920: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00005930: 3c4f 7074 696f 6e20 7661 6c75 653d 2273  <Option value="s
-00005940: 6f6c 6964 2220 6e61 6d65 3d22 6f75 746c  olid" name="outl
-00005950: 696e 655f 7374 796c 6522 2074 7970 653d  ine_style" type=
-00005960: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-00005970: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00005980: 7661 6c75 653d 2230 2220 6e61 6d65 3d22  value="0" name="
-00005990: 6f75 746c 696e 655f 7769 6474 6822 2074  outline_width" t
-000059a0: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
-000059b0: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-000059c0: 696f 6e20 7661 6c75 653d 2233 783a 302c  ion value="3x:0,
-000059d0: 302c 302c 302c 302c 3022 206e 616d 653d  0,0,0,0,0" name=
-000059e0: 226f 7574 6c69 6e65 5f77 6964 7468 5f6d  "outline_width_m
-000059f0: 6170 5f75 6e69 745f 7363 616c 6522 2074  ap_unit_scale" t
-00005a00: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
-00005a10: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00005a20: 696f 6e20 7661 6c75 653d 2252 656e 6465  ion value="Rende
-00005a30: 724d 6574 6572 7349 6e4d 6170 556e 6974  rMetersInMapUnit
-00005a40: 7322 206e 616d 653d 226f 7574 6c69 6e65  s" name="outline
-00005a50: 5f77 6964 7468 5f75 6e69 7422 2074 7970  _width_unit" typ
-00005a60: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00005a70: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00005a80: 6e20 7661 6c75 653d 2264 6961 6d65 7465  n value="diamete
-00005a90: 7222 206e 616d 653d 2273 6361 6c65 5f6d  r" name="scale_m
-00005aa0: 6574 686f 6422 2074 7970 653d 2251 5374  ethod" type="QSt
-00005ab0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-00005ac0: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-00005ad0: 653d 2236 2220 6e61 6d65 3d22 7369 7a65  e="6" name="size
-00005ae0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00005af0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-00005b00: 4f70 7469 6f6e 2076 616c 7565 3d22 3378  Option value="3x
-00005b10: 3a30 2c30 2c30 2c30 2c30 2c30 2220 6e61  :0,0,0,0,0,0" na
-00005b20: 6d65 3d22 7369 7a65 5f6d 6170 5f75 6e69  me="size_map_uni
-00005b30: 745f 7363 616c 6522 2074 7970 653d 2251  t_scale" type="Q
-00005b40: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
-00005b50: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
-00005b60: 6c75 653d 2252 656e 6465 724d 6574 6572  lue="RenderMeter
-00005b70: 7349 6e4d 6170 556e 6974 7322 206e 616d  sInMapUnits" nam
-00005b80: 653d 2273 697a 655f 756e 6974 2220 7479  e="size_unit" ty
-00005b90: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
-00005ba0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00005bb0: 6f6e 2076 616c 7565 3d22 3122 206e 616d  on value="1" nam
-00005bc0: 653d 2276 6572 7469 6361 6c5f 616e 6368  e="vertical_anch
-00005bd0: 6f72 5f70 6f69 6e74 2220 7479 7065 3d22  or_point" type="
-00005be0: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-00005bf0: 2020 2020 203c 2f4f 7074 696f 6e3e 0a20       </Option>. 
-00005c00: 2020 2020 2020 2020 203c 6461 7461 5f64           <data_d
-00005c10: 6566 696e 6564 5f70 726f 7065 7274 6965  efined_propertie
-00005c20: 733e 0a20 2020 2020 2020 2020 2020 203c  s>.            <
-00005c30: 4f70 7469 6f6e 2074 7970 653d 224d 6170  Option type="Map
-00005c40: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00005c50: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-00005c60: 2220 6e61 6d65 3d22 6e61 6d65 2220 7479  " name="name" ty
-00005c70: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
-00005c80: 2020 2020 2020 2020 2020 2020 203c 4f70               <Op
-00005c90: 7469 6f6e 206e 616d 653d 2270 726f 7065  tion name="prope
-00005ca0: 7274 6965 7322 2074 7970 653d 224d 6170  rties" type="Map
-00005cb0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00005cc0: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
-00005cd0: 2273 697a 6522 2074 7970 653d 224d 6170  "size" type="Map
-00005ce0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00005cf0: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00005d00: 7565 3d22 7472 7565 2220 6e61 6d65 3d22  ue="true" name="
-00005d10: 6163 7469 7665 2220 7479 7065 3d22 626f  active" type="bo
-00005d20: 6f6c 222f 3e0a 2020 2020 2020 2020 2020  ol"/>.          
-00005d30: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00005d40: 7661 6c75 653d 2226 7175 6f74 3b6c 616e  value="&quot;lan
-00005d50: 655f 7769 6474 6826 7175 6f74 3b22 206e  e_width&quot;" n
-00005d60: 616d 653d 2265 7870 7265 7373 696f 6e22  ame="expression"
-00005d70: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-00005d80: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00005d90: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-00005da0: 653d 2233 2220 6e61 6d65 3d22 7479 7065  e="3" name="type
-00005db0: 2220 7479 7065 3d22 696e 7422 2f3e 0a20  " type="int"/>. 
-00005dc0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00005dd0: 2f4f 7074 696f 6e3e 0a20 2020 2020 2020  /Option>.       
-00005de0: 2020 2020 2020 203c 2f4f 7074 696f 6e3e         </Option>
-00005df0: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-00005e00: 4f70 7469 6f6e 2076 616c 7565 3d22 636f  Option value="co
-00005e10: 6c6c 6563 7469 6f6e 2220 6e61 6d65 3d22  llection" name="
-00005e20: 7479 7065 2220 7479 7065 3d22 5153 7472  type" type="QStr
-00005e30: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-00005e40: 2020 203c 2f4f 7074 696f 6e3e 0a20 2020     </Option>.   
-00005e50: 2020 2020 2020 203c 2f64 6174 615f 6465         </data_de
-00005e60: 6669 6e65 645f 7072 6f70 6572 7469 6573  fined_properties
-00005e70: 3e0a 2020 2020 2020 2020 3c2f 6c61 7965  >.        </laye
-00005e80: 723e 0a20 2020 2020 203c 2f73 796d 626f  r>.      </symbo
-00005e90: 6c3e 0a20 2020 203c 2f73 796d 626f 6c73  l>.    </symbols
-00005ea0: 3e0a 2020 3c2f 7265 6e64 6572 6572 2d76  >.  </renderer-v
-00005eb0: 323e 0a20 203c 6375 7374 6f6d 7072 6f70  2>.  <customprop
-00005ec0: 6572 7469 6573 3e0a 2020 2020 3c4f 7074  erties>.    <Opt
-00005ed0: 696f 6e20 7479 7065 3d22 4d61 7022 3e0a  ion type="Map">.
-00005ee0: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
-00005ef0: 6d65 3d22 6475 616c 7669 6577 2f70 7265  me="dualview/pre
-00005f00: 7669 6577 4578 7072 6573 7369 6f6e 7322  viewExpressions"
-00005f10: 2074 7970 653d 224c 6973 7422 3e0a 2020   type="List">.  
-00005f20: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
-00005f30: 6c75 653d 2226 7175 6f74 3b74 7970 6526  lue="&quot;type&
-00005f40: 7175 6f74 3b22 2074 7970 653d 2251 5374  quot;" type="QSt
-00005f50: 7269 6e67 222f 3e0a 2020 2020 2020 3c2f  ring"/>.      </
-00005f60: 4f70 7469 6f6e 3e0a 2020 2020 2020 3c4f  Option>.      <O
-00005f70: 7074 696f 6e20 7661 6c75 653d 2230 2220  ption value="0" 
-00005f80: 6e61 6d65 3d22 656d 6265 6464 6564 5769  name="embeddedWi
-00005f90: 6467 6574 732f 636f 756e 7422 2074 7970  dgets/count" typ
-00005fa0: 653d 2269 6e74 222f 3e0a 2020 2020 2020  e="int"/>.      
-00005fb0: 3c4f 7074 696f 6e20 6e61 6d65 3d22 7661  <Option name="va
-00005fc0: 7269 6162 6c65 4e61 6d65 7322 2f3e 0a20  riableNames"/>. 
-00005fd0: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
-00005fe0: 653d 2276 6172 6961 626c 6556 616c 7565  e="variableValue
-00005ff0: 7322 2f3e 0a20 2020 203c 2f4f 7074 696f  s"/>.    </Optio
-00006000: 6e3e 0a20 203c 2f63 7573 746f 6d70 726f  n>.  </custompro
-00006010: 7065 7274 6965 733e 0a20 203c 626c 656e  perties>.  <blen
-00006020: 644d 6f64 653e 303c 2f62 6c65 6e64 4d6f  dMode>0</blendMo
-00006030: 6465 3e0a 2020 3c66 6561 7475 7265 426c  de>.  <featureBl
-00006040: 656e 644d 6f64 653e 303c 2f66 6561 7475  endMode>0</featu
-00006050: 7265 426c 656e 644d 6f64 653e 0a20 203c  reBlendMode>.  <
-00006060: 6c61 7965 724f 7061 6369 7479 3e31 3c2f  layerOpacity>1</
-00006070: 6c61 7965 724f 7061 6369 7479 3e0a 2020  layerOpacity>.  
-00006080: 3c53 696e 676c 6543 6174 6567 6f72 7944  <SingleCategoryD
-00006090: 6961 6772 616d 5265 6e64 6572 6572 2061  iagramRenderer a
-000060a0: 7474 7269 6275 7465 4c65 6765 6e64 3d22  ttributeLegend="
-000060b0: 3122 2064 6961 6772 616d 5479 7065 3d22  1" diagramType="
-000060c0: 4869 7374 6f67 7261 6d22 3e0a 2020 2020  Histogram">.    
-000060d0: 3c44 6961 6772 616d 4361 7465 676f 7279  <DiagramCategory
-000060e0: 2062 6163 6b67 726f 756e 6441 6c70 6861   backgroundAlpha
-000060f0: 3d22 3235 3522 206c 6162 656c 506c 6163  ="255" labelPlac
-00006100: 656d 656e 744d 6574 686f 643d 2258 4865  ementMethod="XHe
-00006110: 6967 6874 2220 7369 7a65 5363 616c 653d  ight" sizeScale=
-00006120: 2233 783a 302c 302c 302c 302c 302c 3022  "3x:0,0,0,0,0,0"
-00006130: 206c 696e 6553 697a 6553 6361 6c65 3d22   lineSizeScale="
-00006140: 3378 3a30 2c30 2c30 2c30 2c30 2c30 2220  3x:0,0,0,0,0,0" 
-00006150: 7065 6e43 6f6c 6f72 3d22 2330 3030 3030  penColor="#00000
-00006160: 3022 206d 696e 5363 616c 6544 656e 6f6d  0" minScaleDenom
-00006170: 696e 6174 6f72 3d22 3022 2073 6361 6c65  inator="0" scale
-00006180: 4261 7365 6456 6973 6962 696c 6974 793d  BasedVisibility=
-00006190: 2230 2220 6f70 6163 6974 793d 2231 2220  "0" opacity="1" 
-000061a0: 6261 7257 6964 7468 3d22 3522 2064 6972  barWidth="5" dir
-000061b0: 6563 7469 6f6e 3d22 3022 2070 656e 416c  ection="0" penAl
-000061c0: 7068 613d 2232 3535 2220 7769 6474 683d  pha="255" width=
-000061d0: 2231 3522 2073 6361 6c65 4465 7065 6e64  "15" scaleDepend
-000061e0: 656e 6379 3d22 4172 6561 2220 7369 7a65  ency="Area" size
-000061f0: 5479 7065 3d22 4d4d 2220 7370 6163 696e  Type="MM" spacin
-00006200: 6755 6e69 743d 224d 4d22 2073 7061 6369  gUnit="MM" spaci
-00006210: 6e67 556e 6974 5363 616c 653d 2233 783a  ngUnitScale="3x:
-00006220: 302c 302c 302c 302c 302c 3022 2073 686f  0,0,0,0,0,0" sho
-00006230: 7741 7869 733d 2231 2220 6865 6967 6874  wAxis="1" height
-00006240: 3d22 3135 2220 6469 6167 7261 6d4f 7269  ="15" diagramOri
-00006250: 656e 7461 7469 6f6e 3d22 5570 2220 7065  entation="Up" pe
-00006260: 6e57 6964 7468 3d22 3022 206c 696e 6553  nWidth="0" lineS
-00006270: 697a 6554 7970 653d 224d 4d22 206d 696e  izeType="MM" min
-00006280: 696d 756d 5369 7a65 3d22 3022 2065 6e61  imumSize="0" ena
-00006290: 626c 6564 3d22 3022 2062 6163 6b67 726f  bled="0" backgro
-000062a0: 756e 6443 6f6c 6f72 3d22 2366 6666 6666  undColor="#fffff
-000062b0: 6622 2073 7061 6369 6e67 3d22 3522 206d  f" spacing="5" m
-000062c0: 6178 5363 616c 6544 656e 6f6d 696e 6174  axScaleDenominat
-000062d0: 6f72 3d22 3165 2b30 3822 2072 6f74 6174  or="1e+08" rotat
-000062e0: 696f 6e4f 6666 7365 743d 2232 3730 223e  ionOffset="270">
-000062f0: 0a20 2020 2020 203c 666f 6e74 5072 6f70  .      <fontProp
-00006300: 6572 7469 6573 2064 6573 6372 6970 7469  erties descripti
-00006310: 6f6e 3d22 4e6f 746f 2053 616e 732c 3130  on="Noto Sans,10
-00006320: 2c2d 312c 302c 3530 2c30 2c30 2c30 2c30  ,-1,0,50,0,0,0,0
-00006330: 2c30 2220 7374 796c 653d 2222 2073 7472  ,0" style="" str
-00006340: 696b 6574 6872 6f75 6768 3d22 3022 2075  ikethrough="0" u
-00006350: 6e64 6572 6c69 6e65 3d22 3022 2069 7461  nderline="0" ita
-00006360: 6c69 633d 2230 2220 626f 6c64 3d22 3022  lic="0" bold="0"
-00006370: 2f3e 0a20 2020 2020 203c 6174 7472 6962  />.      <attrib
-00006380: 7574 6520 6669 656c 643d 2222 2063 6f6c  ute field="" col
-00006390: 6f72 3d22 2330 3030 3030 3022 206c 6162  or="#000000" lab
-000063a0: 656c 3d22 2220 636f 6c6f 724f 7061 6369  el="" colorOpaci
-000063b0: 7479 3d22 3122 2f3e 0a20 2020 2020 203c  ty="1"/>.      <
-000063c0: 6178 6973 5379 6d62 6f6c 3e0a 2020 2020  axisSymbol>.    
-000063d0: 2020 2020 3c73 796d 626f 6c20 6672 616d      <symbol fram
-000063e0: 655f 7261 7465 3d22 3130 2220 6973 5f61  e_rate="10" is_a
-000063f0: 6e69 6d61 7465 643d 2230 2220 6e61 6d65  nimated="0" name
-00006400: 3d22 2220 616c 7068 613d 2231 2220 666f  ="" alpha="1" fo
-00006410: 7263 655f 7268 723d 2230 2220 636c 6970  rce_rhr="0" clip
-00006420: 5f74 6f5f 6578 7465 6e74 3d22 3122 2074  _to_extent="1" t
-00006430: 7970 653d 226c 696e 6522 3e0a 2020 2020  ype="line">.    
-00006440: 2020 2020 2020 3c64 6174 615f 6465 6669        <data_defi
-00006450: 6e65 645f 7072 6f70 6572 7469 6573 3e0a  ned_properties>.
-00006460: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00006470: 696f 6e20 7479 7065 3d22 4d61 7022 3e0a  ion type="Map">.
-00006480: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
-00006490: 7074 696f 6e20 7661 6c75 653d 2222 206e  ption value="" n
-000064a0: 616d 653d 226e 616d 6522 2074 7970 653d  ame="name" type=
-000064b0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-000064c0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-000064d0: 6e20 6e61 6d65 3d22 7072 6f70 6572 7469  n name="properti
-000064e0: 6573 222f 3e0a 2020 2020 2020 2020 2020  es"/>.          
-000064f0: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-00006500: 653d 2263 6f6c 6c65 6374 696f 6e22 206e  e="collection" n
-00006510: 616d 653d 2274 7970 6522 2074 7970 653d  ame="type" type=
-00006520: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-00006530: 2020 2020 2020 2020 3c2f 4f70 7469 6f6e          </Option
-00006540: 3e0a 2020 2020 2020 2020 2020 3c2f 6461  >.          </da
-00006550: 7461 5f64 6566 696e 6564 5f70 726f 7065  ta_defined_prope
-00006560: 7274 6965 733e 0a20 2020 2020 2020 2020  rties>.         
-00006570: 203c 6c61 7965 7220 656e 6162 6c65 643d   <layer enabled=
-00006580: 2231 2220 636c 6173 733d 2253 696d 706c  "1" class="Simpl
-00006590: 654c 696e 6522 206c 6f63 6b65 643d 2230  eLine" locked="0
-000065a0: 2220 7061 7373 3d22 3022 3e0a 2020 2020  " pass="0">.    
-000065b0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-000065c0: 7479 7065 3d22 4d61 7022 3e0a 2020 2020  type="Map">.    
-000065d0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-000065e0: 6e20 7661 6c75 653d 2230 2220 6e61 6d65  n value="0" name
-000065f0: 3d22 616c 6967 6e5f 6461 7368 5f70 6174  ="align_dash_pat
-00006600: 7465 726e 2220 7479 7065 3d22 5153 7472  tern" type="QStr
-00006610: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-00006620: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00006630: 7565 3d22 7371 7561 7265 2220 6e61 6d65  ue="square" name
-00006640: 3d22 6361 7073 7479 6c65 2220 7479 7065  ="capstyle" type
-00006650: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-00006660: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00006670: 6f6e 2076 616c 7565 3d22 353b 3222 206e  on value="5;2" n
-00006680: 616d 653d 2263 7573 746f 6d64 6173 6822  ame="customdash"
-00006690: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-000066a0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000066b0: 3c4f 7074 696f 6e20 7661 6c75 653d 2233  <Option value="3
-000066c0: 783a 302c 302c 302c 302c 302c 3022 206e  x:0,0,0,0,0,0" n
-000066d0: 616d 653d 2263 7573 746f 6d64 6173 685f  ame="customdash_
-000066e0: 6d61 705f 756e 6974 5f73 6361 6c65 2220  map_unit_scale" 
-000066f0: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
-00006700: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-00006710: 4f70 7469 6f6e 2076 616c 7565 3d22 4d4d  Option value="MM
-00006720: 2220 6e61 6d65 3d22 6375 7374 6f6d 6461  " name="customda
-00006730: 7368 5f75 6e69 7422 2074 7970 653d 2251  sh_unit" type="Q
-00006740: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
-00006750: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00006760: 7661 6c75 653d 2230 2220 6e61 6d65 3d22  value="0" name="
-00006770: 6461 7368 5f70 6174 7465 726e 5f6f 6666  dash_pattern_off
-00006780: 7365 7422 2074 7970 653d 2251 5374 7269  set" type="QStri
-00006790: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
-000067a0: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-000067b0: 653d 2233 783a 302c 302c 302c 302c 302c  e="3x:0,0,0,0,0,
-000067c0: 3022 206e 616d 653d 2264 6173 685f 7061  0" name="dash_pa
-000067d0: 7474 6572 6e5f 6f66 6673 6574 5f6d 6170  ttern_offset_map
-000067e0: 5f75 6e69 745f 7363 616c 6522 2074 7970  _unit_scale" typ
-000067f0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00006800: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00006810: 696f 6e20 7661 6c75 653d 224d 4d22 206e  ion value="MM" n
-00006820: 616d 653d 2264 6173 685f 7061 7474 6572  ame="dash_patter
-00006830: 6e5f 6f66 6673 6574 5f75 6e69 7422 2074  n_offset_unit" t
-00006840: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
-00006850: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
-00006860: 7074 696f 6e20 7661 6c75 653d 2230 2220  ption value="0" 
-00006870: 6e61 6d65 3d22 6472 6177 5f69 6e73 6964  name="draw_insid
-00006880: 655f 706f 6c79 676f 6e22 2074 7970 653d  e_polygon" type=
-00006890: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-000068a0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-000068b0: 6e20 7661 6c75 653d 2262 6576 656c 2220  n value="bevel" 
-000068c0: 6e61 6d65 3d22 6a6f 696e 7374 796c 6522  name="joinstyle"
-000068d0: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-000068e0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000068f0: 3c4f 7074 696f 6e20 7661 6c75 653d 2233  <Option value="3
-00006900: 352c 3335 2c33 352c 3235 3522 206e 616d  5,35,35,255" nam
-00006910: 653d 226c 696e 655f 636f 6c6f 7222 2074  e="line_color" t
-00006920: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
-00006930: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
-00006940: 7074 696f 6e20 7661 6c75 653d 2273 6f6c  ption value="sol
-00006950: 6964 2220 6e61 6d65 3d22 6c69 6e65 5f73  id" name="line_s
-00006960: 7479 6c65 2220 7479 7065 3d22 5153 7472  tyle" type="QStr
-00006970: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-00006980: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00006990: 7565 3d22 302e 3236 2220 6e61 6d65 3d22  ue="0.26" name="
-000069a0: 6c69 6e65 5f77 6964 7468 2220 7479 7065  line_width" type
-000069b0: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-000069c0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-000069d0: 6f6e 2076 616c 7565 3d22 4d4d 2220 6e61  on value="MM" na
-000069e0: 6d65 3d22 6c69 6e65 5f77 6964 7468 5f75  me="line_width_u
-000069f0: 6e69 7422 2074 7970 653d 2251 5374 7269  nit" type="QStri
-00006a00: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
-00006a10: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-00006a20: 653d 2230 2220 6e61 6d65 3d22 6f66 6673  e="0" name="offs
-00006a30: 6574 2220 7479 7065 3d22 5153 7472 696e  et" type="QStrin
-00006a40: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
-00006a50: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
-00006a60: 3d22 3378 3a30 2c30 2c30 2c30 2c30 2c30  ="3x:0,0,0,0,0,0
-00006a70: 2220 6e61 6d65 3d22 6f66 6673 6574 5f6d  " name="offset_m
-00006a80: 6170 5f75 6e69 745f 7363 616c 6522 2074  ap_unit_scale" t
-00006a90: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
-00006aa0: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
-00006ab0: 7074 696f 6e20 7661 6c75 653d 224d 4d22  ption value="MM"
-00006ac0: 206e 616d 653d 226f 6666 7365 745f 756e   name="offset_un
-00006ad0: 6974 2220 7479 7065 3d22 5153 7472 696e  it" type="QStrin
-00006ae0: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
-00006af0: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
-00006b00: 3d22 3022 206e 616d 653d 2272 696e 675f  ="0" name="ring_
-00006b10: 6669 6c74 6572 2220 7479 7065 3d22 5153  filter" type="QS
-00006b20: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00006b30: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-00006b40: 616c 7565 3d22 3022 206e 616d 653d 2274  alue="0" name="t
-00006b50: 7269 6d5f 6469 7374 616e 6365 5f65 6e64  rim_distance_end
-00006b60: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00006b70: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
-00006b80: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-00006b90: 3378 3a30 2c30 2c30 2c30 2c30 2c30 2220  3x:0,0,0,0,0,0" 
-00006ba0: 6e61 6d65 3d22 7472 696d 5f64 6973 7461  name="trim_dista
-00006bb0: 6e63 655f 656e 645f 6d61 705f 756e 6974  nce_end_map_unit
-00006bc0: 5f73 6361 6c65 2220 7479 7065 3d22 5153  _scale" type="QS
-00006bd0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00006be0: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-00006bf0: 616c 7565 3d22 4d4d 2220 6e61 6d65 3d22  alue="MM" name="
-00006c00: 7472 696d 5f64 6973 7461 6e63 655f 656e  trim_distance_en
-00006c10: 645f 756e 6974 2220 7479 7065 3d22 5153  d_unit" type="QS
-00006c20: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00006c30: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-00006c40: 616c 7565 3d22 3022 206e 616d 653d 2274  alue="0" name="t
-00006c50: 7269 6d5f 6469 7374 616e 6365 5f73 7461  rim_distance_sta
-00006c60: 7274 2220 7479 7065 3d22 5153 7472 696e  rt" type="QStrin
-00006c70: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
-00006c80: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
-00006c90: 3d22 3378 3a30 2c30 2c30 2c30 2c30 2c30  ="3x:0,0,0,0,0,0
-00006ca0: 2220 6e61 6d65 3d22 7472 696d 5f64 6973  " name="trim_dis
-00006cb0: 7461 6e63 655f 7374 6172 745f 6d61 705f  tance_start_map_
-00006cc0: 756e 6974 5f73 6361 6c65 2220 7479 7065  unit_scale" type
-00006cd0: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-00006ce0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00006cf0: 6f6e 2076 616c 7565 3d22 4d4d 2220 6e61  on value="MM" na
-00006d00: 6d65 3d22 7472 696d 5f64 6973 7461 6e63  me="trim_distanc
-00006d10: 655f 7374 6172 745f 756e 6974 2220 7479  e_start_unit" ty
-00006d20: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
-00006d30: 2020 2020 2020 2020 2020 2020 203c 4f70               <Op
-00006d40: 7469 6f6e 2076 616c 7565 3d22 3022 206e  tion value="0" n
-00006d50: 616d 653d 2274 7765 616b 5f64 6173 685f  ame="tweak_dash_
-00006d60: 7061 7474 6572 6e5f 6f6e 5f63 6f72 6e65  pattern_on_corne
-00006d70: 7273 2220 7479 7065 3d22 5153 7472 696e  rs" type="QStrin
-00006d80: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
-00006d90: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
-00006da0: 3d22 3022 206e 616d 653d 2275 7365 5f63  ="0" name="use_c
-00006db0: 7573 746f 6d5f 6461 7368 2220 7479 7065  ustom_dash" type
-00006dc0: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-00006dd0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00006de0: 6f6e 2076 616c 7565 3d22 3378 3a30 2c30  on value="3x:0,0
-00006df0: 2c30 2c30 2c30 2c30 2220 6e61 6d65 3d22  ,0,0,0,0" name="
-00006e00: 7769 6474 685f 6d61 705f 756e 6974 5f73  width_map_unit_s
-00006e10: 6361 6c65 2220 7479 7065 3d22 5153 7472  cale" type="QStr
-00006e20: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-00006e30: 2020 203c 2f4f 7074 696f 6e3e 0a20 2020     </Option>.   
-00006e40: 2020 2020 2020 2020 203c 6461 7461 5f64           <data_d
-00006e50: 6566 696e 6564 5f70 726f 7065 7274 6965  efined_propertie
-00006e60: 733e 0a20 2020 2020 2020 2020 2020 2020  s>.             
-00006e70: 203c 4f70 7469 6f6e 2074 7970 653d 224d   <Option type="M
-00006e80: 6170 223e 0a20 2020 2020 2020 2020 2020  ap">.           
-00006e90: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00006ea0: 7565 3d22 2220 6e61 6d65 3d22 6e61 6d65  ue="" name="name
-00006eb0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00006ec0: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
-00006ed0: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
-00006ee0: 2270 726f 7065 7274 6965 7322 2f3e 0a20  "properties"/>. 
-00006ef0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00006f00: 4f70 7469 6f6e 2076 616c 7565 3d22 636f  Option value="co
-00006f10: 6c6c 6563 7469 6f6e 2220 6e61 6d65 3d22  llection" name="
-00006f20: 7479 7065 2220 7479 7065 3d22 5153 7472  type" type="QStr
-00006f30: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-00006f40: 2020 2020 203c 2f4f 7074 696f 6e3e 0a20       </Option>. 
-00006f50: 2020 2020 2020 2020 2020 203c 2f64 6174             </dat
-00006f60: 615f 6465 6669 6e65 645f 7072 6f70 6572  a_defined_proper
-00006f70: 7469 6573 3e0a 2020 2020 2020 2020 2020  ties>.          
-00006f80: 3c2f 6c61 7965 723e 0a20 2020 2020 2020  </layer>.       
-00006f90: 203c 2f73 796d 626f 6c3e 0a20 2020 2020   </symbol>.     
-00006fa0: 203c 2f61 7869 7353 796d 626f 6c3e 0a20   </axisSymbol>. 
-00006fb0: 2020 203c 2f44 6961 6772 616d 4361 7465     </DiagramCate
-00006fc0: 676f 7279 3e0a 2020 3c2f 5369 6e67 6c65  gory>.  </Single
-00006fd0: 4361 7465 676f 7279 4469 6167 7261 6d52  CategoryDiagramR
-00006fe0: 656e 6465 7265 723e 0a20 203c 4469 6167  enderer>.  <Diag
-00006ff0: 7261 6d4c 6179 6572 5365 7474 696e 6773  ramLayerSettings
-00007000: 2064 6973 743d 2230 2220 7368 6f77 416c   dist="0" showAl
-00007010: 6c3d 2231 2220 6c69 6e65 506c 6163 656d  l="1" linePlacem
-00007020: 656e 7446 6c61 6773 3d22 3138 2220 6f62  entFlags="18" ob
-00007030: 7374 6163 6c65 3d22 3022 2070 7269 6f72  stacle="0" prior
-00007040: 6974 793d 2230 2220 706c 6163 656d 656e  ity="0" placemen
-00007050: 743d 2230 2220 7a49 6e64 6578 3d22 3022  t="0" zIndex="0"
-00007060: 3e0a 2020 2020 3c70 726f 7065 7274 6965  >.    <propertie
-00007070: 733e 0a20 2020 2020 203c 4f70 7469 6f6e  s>.      <Option
-00007080: 2074 7970 653d 224d 6170 223e 0a20 2020   type="Map">.   
-00007090: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-000070a0: 7565 3d22 2220 6e61 6d65 3d22 6e61 6d65  ue="" name="name
-000070b0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-000070c0: 2f3e 0a20 2020 2020 2020 203c 4f70 7469  />.        <Opti
-000070d0: 6f6e 206e 616d 653d 2270 726f 7065 7274  on name="propert
-000070e0: 6965 7322 2f3e 0a20 2020 2020 2020 203c  ies"/>.        <
-000070f0: 4f70 7469 6f6e 2076 616c 7565 3d22 636f  Option value="co
-00007100: 6c6c 6563 7469 6f6e 2220 6e61 6d65 3d22  llection" name="
-00007110: 7479 7065 2220 7479 7065 3d22 5153 7472  type" type="QStr
-00007120: 696e 6722 2f3e 0a20 2020 2020 203c 2f4f  ing"/>.      </O
-00007130: 7074 696f 6e3e 0a20 2020 203c 2f70 726f  ption>.    </pro
-00007140: 7065 7274 6965 733e 0a20 203c 2f44 6961  perties>.  </Dia
-00007150: 6772 616d 4c61 7965 7253 6574 7469 6e67  gramLayerSetting
-00007160: 733e 0a20 203c 6765 6f6d 6574 7279 4f70  s>.  <geometryOp
-00007170: 7469 6f6e 7320 6765 6f6d 6574 7279 5072  tions geometryPr
-00007180: 6563 6973 696f 6e3d 2230 2220 7265 6d6f  ecision="0" remo
-00007190: 7665 4475 706c 6963 6174 654e 6f64 6573  veDuplicateNodes
-000071a0: 3d22 3022 3e0a 2020 2020 3c61 6374 6976  ="0">.    <activ
-000071b0: 6543 6865 636b 732f 3e0a 2020 2020 3c63  eChecks/>.    <c
-000071c0: 6865 636b 436f 6e66 6967 7572 6174 696f  heckConfiguratio
-000071d0: 6e2f 3e0a 2020 3c2f 6765 6f6d 6574 7279  n/>.  </geometry
-000071e0: 4f70 7469 6f6e 733e 0a20 203c 6c65 6765  Options>.  <lege
-000071f0: 6e64 2073 686f 774c 6162 656c 4c65 6765  nd showLabelLege
-00007200: 6e64 3d22 3022 2074 7970 653d 2264 6566  nd="0" type="def
-00007210: 6175 6c74 2d76 6563 746f 7222 2f3e 0a20  ault-vector"/>. 
-00007220: 203c 7265 6665 7265 6e63 6564 4c61 7965   <referencedLaye
-00007230: 7273 2f3e 0a20 203c 6669 656c 6443 6f6e  rs/>.  <fieldCon
-00007240: 6669 6775 7261 7469 6f6e 3e0a 2020 2020  figuration>.    
-00007250: 3c66 6965 6c64 206e 616d 653d 2274 7970  <field name="typ
-00007260: 6522 2063 6f6e 6669 6775 7261 7469 6f6e  e" configuration
-00007270: 466c 6167 733d 224e 6f6e 6522 3e0a 2020  Flags="None">.  
-00007280: 2020 2020 3c65 6469 7457 6964 6765 7420      <editWidget 
-00007290: 7479 7065 3d22 5465 7874 4564 6974 223e  type="TextEdit">
-000072a0: 0a20 2020 2020 2020 203c 636f 6e66 6967  .        <config
-000072b0: 3e0a 2020 2020 2020 2020 2020 3c4f 7074  >.          <Opt
-000072c0: 696f 6e2f 3e0a 2020 2020 2020 2020 3c2f  ion/>.        </
-000072d0: 636f 6e66 6967 3e0a 2020 2020 2020 3c2f  config>.      </
-000072e0: 6564 6974 5769 6467 6574 3e0a 2020 2020  editWidget>.    
-000072f0: 3c2f 6669 656c 643e 0a20 2020 203c 6669  </field>.    <fi
-00007300: 656c 6420 6e61 6d65 3d22 6f73 6d5f 6964  eld name="osm_id
-00007310: 2220 636f 6e66 6967 7572 6174 696f 6e46  " configurationF
-00007320: 6c61 6773 3d22 4e6f 6e65 223e 0a20 2020  lags="None">.   
-00007330: 2020 203c 6564 6974 5769 6467 6574 2074     <editWidget t
-00007340: 7970 653d 2254 6578 7445 6469 7422 3e0a  ype="TextEdit">.
-00007350: 2020 2020 2020 2020 3c63 6f6e 6669 673e          <config>
-00007360: 0a20 2020 2020 2020 2020 203c 4f70 7469  .          <Opti
-00007370: 6f6e 2f3e 0a20 2020 2020 2020 203c 2f63  on/>.        </c
-00007380: 6f6e 6669 673e 0a20 2020 2020 203c 2f65  onfig>.      </e
-00007390: 6469 7457 6964 6765 743e 0a20 2020 203c  ditWidget>.    <
-000073a0: 2f66 6965 6c64 3e0a 2020 2020 3c66 6965  /field>.    <fie
-000073b0: 6c64 206e 616d 653d 226f 7269 656e 7461  ld name="orienta
-000073c0: 7469 6f6e 2220 636f 6e66 6967 7572 6174  tion" configurat
-000073d0: 696f 6e46 6c61 6773 3d22 4e6f 6e65 223e  ionFlags="None">
-000073e0: 0a20 2020 2020 203c 6564 6974 5769 6467  .      <editWidg
-000073f0: 6574 2074 7970 653d 2254 6578 7445 6469  et type="TextEdi
-00007400: 7422 3e0a 2020 2020 2020 2020 3c63 6f6e  t">.        <con
-00007410: 6669 673e 0a20 2020 2020 2020 2020 203c  fig>.          <
-00007420: 4f70 7469 6f6e 2f3e 0a20 2020 2020 2020  Option/>.       
-00007430: 203c 2f63 6f6e 6669 673e 0a20 2020 2020   </config>.     
-00007440: 203c 2f65 6469 7457 6964 6765 743e 0a20   </editWidget>. 
-00007450: 2020 203c 2f66 6965 6c64 3e0a 2020 2020     </field>.    
-00007460: 3c66 6965 6c64 206e 616d 653d 226f 7269  <field name="ori
-00007470: 656e 7461 7469 6f6e 5f63 6f6e 6669 6465  entation_confide
-00007480: 6e63 6522 2063 6f6e 6669 6775 7261 7469  nce" configurati
-00007490: 6f6e 466c 6167 733d 224e 6f6e 6522 3e0a  onFlags="None">.
-000074a0: 2020 2020 2020 3c65 6469 7457 6964 6765        <editWidge
-000074b0: 7420 7479 7065 3d22 5465 7874 4564 6974  t type="TextEdit
-000074c0: 223e 0a20 2020 2020 2020 203c 636f 6e66  ">.        <conf
-000074d0: 6967 3e0a 2020 2020 2020 2020 2020 3c4f  ig>.          <O
-000074e0: 7074 696f 6e2f 3e0a 2020 2020 2020 2020  ption/>.        
-000074f0: 3c2f 636f 6e66 6967 3e0a 2020 2020 2020  </config>.      
-00007500: 3c2f 6564 6974 5769 6467 6574 3e0a 2020  </editWidget>.  
-00007510: 2020 3c2f 6669 656c 643e 0a20 2020 203c    </field>.    <
-00007520: 6669 656c 6420 6e61 6d65 3d22 6c61 6e65  field name="lane
-00007530: 5f77 6964 7468 2220 636f 6e66 6967 7572  _width" configur
-00007540: 6174 696f 6e46 6c61 6773 3d22 4e6f 6e65  ationFlags="None
-00007550: 223e 0a20 2020 2020 203c 6564 6974 5769  ">.      <editWi
-00007560: 6467 6574 2074 7970 653d 2254 6578 7445  dget type="TextE
-00007570: 6469 7422 3e0a 2020 2020 2020 2020 3c63  dit">.        <c
-00007580: 6f6e 6669 673e 0a20 2020 2020 2020 2020  onfig>.         
-00007590: 203c 4f70 7469 6f6e 2f3e 0a20 2020 2020   <Option/>.     
-000075a0: 2020 203c 2f63 6f6e 6669 673e 0a20 2020     </config>.   
-000075b0: 2020 203c 2f65 6469 7457 6964 6765 743e     </editWidget>
-000075c0: 0a20 2020 203c 2f66 6965 6c64 3e0a 2020  .    </field>.  
-000075d0: 2020 3c66 6965 6c64 206e 616d 653d 226c    <field name="l
-000075e0: 616e 655f 6f72 6965 6e74 6174 696f 6e22  ane_orientation"
-000075f0: 2063 6f6e 6669 6775 7261 7469 6f6e 466c   configurationFl
-00007600: 6167 733d 224e 6f6e 6522 3e0a 2020 2020  ags="None">.    
-00007610: 2020 3c65 6469 7457 6964 6765 7420 7479    <editWidget ty
-00007620: 7065 3d22 5465 7874 4564 6974 223e 0a20  pe="TextEdit">. 
-00007630: 2020 2020 2020 203c 636f 6e66 6967 3e0a         <config>.
-00007640: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00007650: 6e2f 3e0a 2020 2020 2020 2020 3c2f 636f  n/>.        </co
-00007660: 6e66 6967 3e0a 2020 2020 2020 3c2f 6564  nfig>.      </ed
-00007670: 6974 5769 6467 6574 3e0a 2020 2020 3c2f  itWidget>.    </
-00007680: 6669 656c 643e 0a20 203c 2f66 6965 6c64  field>.  </field
-00007690: 436f 6e66 6967 7572 6174 696f 6e3e 0a20  Configuration>. 
-000076a0: 203c 616c 6961 7365 733e 0a20 2020 203c   <aliases>.    <
-000076b0: 616c 6961 7320 6669 656c 643d 2274 7970  alias field="typ
-000076c0: 6522 206e 616d 653d 2222 2069 6e64 6578  e" name="" index
-000076d0: 3d22 3022 2f3e 0a20 2020 203c 616c 6961  ="0"/>.    <alia
-000076e0: 7320 6669 656c 643d 226f 736d 5f69 6422  s field="osm_id"
-000076f0: 206e 616d 653d 2222 2069 6e64 6578 3d22   name="" index="
-00007700: 3122 2f3e 0a20 2020 203c 616c 6961 7320  1"/>.    <alias 
-00007710: 6669 656c 643d 226f 7269 656e 7461 7469  field="orientati
-00007720: 6f6e 2220 6e61 6d65 3d22 2220 696e 6465  on" name="" inde
-00007730: 783d 2232 222f 3e0a 2020 2020 3c61 6c69  x="2"/>.    <ali
-00007740: 6173 2066 6965 6c64 3d22 6f72 6965 6e74  as field="orient
-00007750: 6174 696f 6e5f 636f 6e66 6964 656e 6365  ation_confidence
-00007760: 2220 6e61 6d65 3d22 2220 696e 6465 783d  " name="" index=
-00007770: 2233 222f 3e0a 2020 2020 3c61 6c69 6173  "3"/>.    <alias
-00007780: 2066 6965 6c64 3d22 6c61 6e65 5f77 6964   field="lane_wid
-00007790: 7468 2220 6e61 6d65 3d22 2220 696e 6465  th" name="" inde
-000077a0: 783d 2234 222f 3e0a 2020 2020 3c61 6c69  x="4"/>.    <ali
-000077b0: 6173 2066 6965 6c64 3d22 6c61 6e65 5f6f  as field="lane_o
-000077c0: 7269 656e 7461 7469 6f6e 2220 6e61 6d65  rientation" name
-000077d0: 3d22 2220 696e 6465 783d 2235 222f 3e0a  ="" index="5"/>.
-000077e0: 2020 3c2f 616c 6961 7365 733e 0a20 203c    </aliases>.  <
-000077f0: 6465 6661 756c 7473 3e0a 2020 2020 3c64  defaults>.    <d
-00007800: 6566 6175 6c74 2066 6965 6c64 3d22 7479  efault field="ty
-00007810: 7065 2220 6170 706c 794f 6e55 7064 6174  pe" applyOnUpdat
-00007820: 653d 2230 2220 6578 7072 6573 7369 6f6e  e="0" expression
-00007830: 3d22 222f 3e0a 2020 2020 3c64 6566 6175  =""/>.    <defau
-00007840: 6c74 2066 6965 6c64 3d22 6f73 6d5f 6964  lt field="osm_id
-00007850: 2220 6170 706c 794f 6e55 7064 6174 653d  " applyOnUpdate=
-00007860: 2230 2220 6578 7072 6573 7369 6f6e 3d22  "0" expression="
-00007870: 222f 3e0a 2020 2020 3c64 6566 6175 6c74  "/>.    <default
-00007880: 2066 6965 6c64 3d22 6f72 6965 6e74 6174   field="orientat
-00007890: 696f 6e22 2061 7070 6c79 4f6e 5570 6461  ion" applyOnUpda
-000078a0: 7465 3d22 3022 2065 7870 7265 7373 696f  te="0" expressio
-000078b0: 6e3d 2222 2f3e 0a20 2020 203c 6465 6661  n=""/>.    <defa
-000078c0: 756c 7420 6669 656c 643d 226f 7269 656e  ult field="orien
-000078d0: 7461 7469 6f6e 5f63 6f6e 6669 6465 6e63  tation_confidenc
-000078e0: 6522 2061 7070 6c79 4f6e 5570 6461 7465  e" applyOnUpdate
-000078f0: 3d22 3022 2065 7870 7265 7373 696f 6e3d  ="0" expression=
-00007900: 2222 2f3e 0a20 2020 203c 6465 6661 756c  ""/>.    <defaul
-00007910: 7420 6669 656c 643d 226c 616e 655f 7769  t field="lane_wi
-00007920: 6474 6822 2061 7070 6c79 4f6e 5570 6461  dth" applyOnUpda
-00007930: 7465 3d22 3022 2065 7870 7265 7373 696f  te="0" expressio
-00007940: 6e3d 2222 2f3e 0a20 2020 203c 6465 6661  n=""/>.    <defa
-00007950: 756c 7420 6669 656c 643d 226c 616e 655f  ult field="lane_
-00007960: 6f72 6965 6e74 6174 696f 6e22 2061 7070  orientation" app
-00007970: 6c79 4f6e 5570 6461 7465 3d22 3022 2065  lyOnUpdate="0" e
-00007980: 7870 7265 7373 696f 6e3d 2222 2f3e 0a20  xpression=""/>. 
-00007990: 203c 2f64 6566 6175 6c74 733e 0a20 203c   </defaults>.  <
-000079a0: 636f 6e73 7472 6169 6e74 733e 0a20 2020  constraints>.   
-000079b0: 203c 636f 6e73 7472 6169 6e74 2066 6965   <constraint fie
-000079c0: 6c64 3d22 7479 7065 2220 636f 6e73 7472  ld="type" constr
-000079d0: 6169 6e74 733d 2230 2220 6578 705f 7374  aints="0" exp_st
-000079e0: 7265 6e67 7468 3d22 3022 2075 6e69 7175  rength="0" uniqu
-000079f0: 655f 7374 7265 6e67 7468 3d22 3022 206e  e_strength="0" n
-00007a00: 6f74 6e75 6c6c 5f73 7472 656e 6774 683d  otnull_strength=
-00007a10: 2230 222f 3e0a 2020 2020 3c63 6f6e 7374  "0"/>.    <const
-00007a20: 7261 696e 7420 6669 656c 643d 226f 736d  raint field="osm
-00007a30: 5f69 6422 2063 6f6e 7374 7261 696e 7473  _id" constraints
-00007a40: 3d22 3022 2065 7870 5f73 7472 656e 6774  ="0" exp_strengt
-00007a50: 683d 2230 2220 756e 6971 7565 5f73 7472  h="0" unique_str
-00007a60: 656e 6774 683d 2230 2220 6e6f 746e 756c  ength="0" notnul
-00007a70: 6c5f 7374 7265 6e67 7468 3d22 3022 2f3e  l_strength="0"/>
-00007a80: 0a20 2020 203c 636f 6e73 7472 6169 6e74  .    <constraint
-00007a90: 2066 6965 6c64 3d22 6f72 6965 6e74 6174   field="orientat
-00007aa0: 696f 6e22 2063 6f6e 7374 7261 696e 7473  ion" constraints
-00007ab0: 3d22 3022 2065 7870 5f73 7472 656e 6774  ="0" exp_strengt
-00007ac0: 683d 2230 2220 756e 6971 7565 5f73 7472  h="0" unique_str
-00007ad0: 656e 6774 683d 2230 2220 6e6f 746e 756c  ength="0" notnul
-00007ae0: 6c5f 7374 7265 6e67 7468 3d22 3022 2f3e  l_strength="0"/>
-00007af0: 0a20 2020 203c 636f 6e73 7472 6169 6e74  .    <constraint
-00007b00: 2066 6965 6c64 3d22 6f72 6965 6e74 6174   field="orientat
-00007b10: 696f 6e5f 636f 6e66 6964 656e 6365 2220  ion_confidence" 
-00007b20: 636f 6e73 7472 6169 6e74 733d 2230 2220  constraints="0" 
-00007b30: 6578 705f 7374 7265 6e67 7468 3d22 3022  exp_strength="0"
-00007b40: 2075 6e69 7175 655f 7374 7265 6e67 7468   unique_strength
-00007b50: 3d22 3022 206e 6f74 6e75 6c6c 5f73 7472  ="0" notnull_str
-00007b60: 656e 6774 683d 2230 222f 3e0a 2020 2020  ength="0"/>.    
-00007b70: 3c63 6f6e 7374 7261 696e 7420 6669 656c  <constraint fiel
-00007b80: 643d 226c 616e 655f 7769 6474 6822 2063  d="lane_width" c
-00007b90: 6f6e 7374 7261 696e 7473 3d22 3022 2065  onstraints="0" e
-00007ba0: 7870 5f73 7472 656e 6774 683d 2230 2220  xp_strength="0" 
-00007bb0: 756e 6971 7565 5f73 7472 656e 6774 683d  unique_strength=
-00007bc0: 2230 2220 6e6f 746e 756c 6c5f 7374 7265  "0" notnull_stre
-00007bd0: 6e67 7468 3d22 3022 2f3e 0a20 2020 203c  ngth="0"/>.    <
-00007be0: 636f 6e73 7472 6169 6e74 2066 6965 6c64  constraint field
-00007bf0: 3d22 6c61 6e65 5f6f 7269 656e 7461 7469  ="lane_orientati
-00007c00: 6f6e 2220 636f 6e73 7472 6169 6e74 733d  on" constraints=
-00007c10: 2230 2220 6578 705f 7374 7265 6e67 7468  "0" exp_strength
-00007c20: 3d22 3022 2075 6e69 7175 655f 7374 7265  ="0" unique_stre
-00007c30: 6e67 7468 3d22 3022 206e 6f74 6e75 6c6c  ngth="0" notnull
-00007c40: 5f73 7472 656e 6774 683d 2230 222f 3e0a  _strength="0"/>.
-00007c50: 2020 3c2f 636f 6e73 7472 6169 6e74 733e    </constraints>
-00007c60: 0a20 203c 636f 6e73 7472 6169 6e74 4578  .  <constraintEx
-00007c70: 7072 6573 7369 6f6e 733e 0a20 2020 203c  pressions>.    <
-00007c80: 636f 6e73 7472 6169 6e74 2066 6965 6c64  constraint field
-00007c90: 3d22 7479 7065 2220 6578 703d 2222 2064  ="type" exp="" d
-00007ca0: 6573 633d 2222 2f3e 0a20 2020 203c 636f  esc=""/>.    <co
-00007cb0: 6e73 7472 6169 6e74 2066 6965 6c64 3d22  nstraint field="
-00007cc0: 6f73 6d5f 6964 2220 6578 703d 2222 2064  osm_id" exp="" d
-00007cd0: 6573 633d 2222 2f3e 0a20 2020 203c 636f  esc=""/>.    <co
-00007ce0: 6e73 7472 6169 6e74 2066 6965 6c64 3d22  nstraint field="
-00007cf0: 6f72 6965 6e74 6174 696f 6e22 2065 7870  orientation" exp
-00007d00: 3d22 2220 6465 7363 3d22 222f 3e0a 2020  ="" desc=""/>.  
-00007d10: 2020 3c63 6f6e 7374 7261 696e 7420 6669    <constraint fi
-00007d20: 656c 643d 226f 7269 656e 7461 7469 6f6e  eld="orientation
-00007d30: 5f63 6f6e 6669 6465 6e63 6522 2065 7870  _confidence" exp
-00007d40: 3d22 2220 6465 7363 3d22 222f 3e0a 2020  ="" desc=""/>.  
-00007d50: 2020 3c63 6f6e 7374 7261 696e 7420 6669    <constraint fi
-00007d60: 656c 643d 226c 616e 655f 7769 6474 6822  eld="lane_width"
-00007d70: 2065 7870 3d22 2220 6465 7363 3d22 222f   exp="" desc=""/
-00007d80: 3e0a 2020 2020 3c63 6f6e 7374 7261 696e  >.    <constrain
-00007d90: 7420 6669 656c 643d 226c 616e 655f 6f72  t field="lane_or
-00007da0: 6965 6e74 6174 696f 6e22 2065 7870 3d22  ientation" exp="
-00007db0: 2220 6465 7363 3d22 222f 3e0a 2020 3c2f  " desc=""/>.  </
-00007dc0: 636f 6e73 7472 6169 6e74 4578 7072 6573  constraintExpres
-00007dd0: 7369 6f6e 733e 0a20 203c 6578 7072 6573  sions>.  <expres
-00007de0: 7369 6f6e 6669 656c 6473 2f3e 0a20 203c  sionfields/>.  <
-00007df0: 6174 7472 6962 7574 6561 6374 696f 6e73  attributeactions
-00007e00: 3e0a 2020 2020 3c64 6566 6175 6c74 4163  >.    <defaultAc
-00007e10: 7469 6f6e 2076 616c 7565 3d22 7b30 3030  tion value="{000
-00007e20: 3030 3030 302d 3030 3030 2d30 3030 302d  00000-0000-0000-
-00007e30: 3030 3030 2d30 3030 3030 3030 3030 3030  0000-00000000000
-00007e40: 307d 2220 6b65 793d 2243 616e 7661 7322  0}" key="Canvas"
-00007e50: 2f3e 0a20 203c 2f61 7474 7269 6275 7465  />.  </attribute
-00007e60: 6163 7469 6f6e 733e 0a20 203c 6174 7472  actions>.  <attr
-00007e70: 6962 7574 6574 6162 6c65 636f 6e66 6967  ibutetableconfig
-00007e80: 2061 6374 696f 6e57 6964 6765 7453 7479   actionWidgetSty
-00007e90: 6c65 3d22 6472 6f70 446f 776e 2220 736f  le="dropDown" so
-00007ea0: 7274 4f72 6465 723d 2230 2220 736f 7274  rtOrder="0" sort
-00007eb0: 4578 7072 6573 7369 6f6e 3d22 223e 0a20  Expression="">. 
-00007ec0: 2020 203c 636f 6c75 6d6e 733e 0a20 2020     <columns>.   
-00007ed0: 2020 203c 636f 6c75 6d6e 2068 6964 6465     <column hidde
-00007ee0: 6e3d 2230 2220 6e61 6d65 3d22 7479 7065  n="0" name="type
-00007ef0: 2220 7769 6474 683d 222d 3122 2074 7970  " width="-1" typ
-00007f00: 653d 2266 6965 6c64 222f 3e0a 2020 2020  e="field"/>.    
-00007f10: 2020 3c63 6f6c 756d 6e20 6869 6464 656e    <column hidden
-00007f20: 3d22 3022 206e 616d 653d 226f 736d 5f69  ="0" name="osm_i
-00007f30: 6422 2077 6964 7468 3d22 3137 3122 2074  d" width="171" t
-00007f40: 7970 653d 2266 6965 6c64 222f 3e0a 2020  ype="field"/>.  
-00007f50: 2020 2020 3c63 6f6c 756d 6e20 6869 6464      <column hidd
-00007f60: 656e 3d22 3022 206e 616d 653d 226f 7269  en="0" name="ori
-00007f70: 656e 7461 7469 6f6e 2220 7769 6474 683d  entation" width=
-00007f80: 2232 3932 2220 7479 7065 3d22 6669 656c  "292" type="fiel
-00007f90: 6422 2f3e 0a20 2020 2020 203c 636f 6c75  d"/>.      <colu
-00007fa0: 6d6e 2068 6964 6465 6e3d 2230 2220 6e61  mn hidden="0" na
-00007fb0: 6d65 3d22 6f72 6965 6e74 6174 696f 6e5f  me="orientation_
-00007fc0: 636f 6e66 6964 656e 6365 2220 7769 6474  confidence" widt
-00007fd0: 683d 222d 3122 2074 7970 653d 2266 6965  h="-1" type="fie
-00007fe0: 6c64 222f 3e0a 2020 2020 2020 3c63 6f6c  ld"/>.      <col
-00007ff0: 756d 6e20 6869 6464 656e 3d22 3022 206e  umn hidden="0" n
-00008000: 616d 653d 226c 616e 655f 6f72 6965 6e74  ame="lane_orient
-00008010: 6174 696f 6e22 2077 6964 7468 3d22 2d31  ation" width="-1
-00008020: 2220 7479 7065 3d22 6669 656c 6422 2f3e  " type="field"/>
-00008030: 0a20 2020 2020 203c 636f 6c75 6d6e 2068  .      <column h
-00008040: 6964 6465 6e3d 2230 2220 6e61 6d65 3d22  idden="0" name="
-00008050: 6c61 6e65 5f77 6964 7468 2220 7769 6474  lane_width" widt
-00008060: 683d 222d 3122 2074 7970 653d 2266 6965  h="-1" type="fie
-00008070: 6c64 222f 3e0a 2020 2020 2020 3c63 6f6c  ld"/>.      <col
-00008080: 756d 6e20 6869 6464 656e 3d22 3122 2077  umn hidden="1" w
-00008090: 6964 7468 3d22 2d31 2220 7479 7065 3d22  idth="-1" type="
-000080a0: 6163 7469 6f6e 7322 2f3e 0a20 2020 203c  actions"/>.    <
-000080b0: 2f63 6f6c 756d 6e73 3e0a 2020 3c2f 6174  /columns>.  </at
-000080c0: 7472 6962 7574 6574 6162 6c65 636f 6e66  tributetableconf
-000080d0: 6967 3e0a 2020 3c63 6f6e 6469 7469 6f6e  ig>.  <condition
-000080e0: 616c 7374 796c 6573 3e0a 2020 2020 3c72  alstyles>.    <r
-000080f0: 6f77 7374 796c 6573 2f3e 0a20 2020 203c  owstyles/>.    <
-00008100: 6669 656c 6473 7479 6c65 732f 3e0a 2020  fieldstyles/>.  
-00008110: 3c2f 636f 6e64 6974 696f 6e61 6c73 7479  </conditionalsty
-00008120: 6c65 733e 0a20 203c 7374 6f72 6564 6578  les>.  <storedex
-00008130: 7072 6573 7369 6f6e 732f 3e0a 2020 3c65  pressions/>.  <e
-00008140: 6469 7466 6f72 6d20 746f 6c65 7261 6e74  ditform tolerant
-00008150: 3d22 3122 3e3c 2f65 6469 7466 6f72 6d3e  ="1"></editform>
-00008160: 0a20 203c 6564 6974 666f 726d 696e 6974  .  <editforminit
-00008170: 2f3e 0a20 203c 6564 6974 666f 726d 696e  />.  <editformin
-00008180: 6974 636f 6465 736f 7572 6365 3e30 3c2f  itcodesource>0</
-00008190: 6564 6974 666f 726d 696e 6974 636f 6465  editforminitcode
-000081a0: 736f 7572 6365 3e0a 2020 3c65 6469 7466  source>.  <editf
-000081b0: 6f72 6d69 6e69 7466 696c 6570 6174 683e  orminitfilepath>
-000081c0: 3c2f 6564 6974 666f 726d 696e 6974 6669  </editforminitfi
-000081d0: 6c65 7061 7468 3e0a 2020 3c65 6469 7466  lepath>.  <editf
-000081e0: 6f72 6d69 6e69 7463 6f64 653e 3c21 5b43  orminitcode><![C
-000081f0: 4441 5441 5b23 202d 2a2d 2063 6f64 696e  DATA[# -*- codin
-00008200: 673a 2075 7466 2d38 202d 2a2d 0a22 2222  g: utf-8 -*-."""
-00008210: 0a4c 6573 2066 6f72 6d75 6c61 6972 6573  .Les formulaires
-00008220: 2051 4749 5320 7065 7576 656e 7420 6176   QGIS peuvent av
-00008230: 6f69 7220 756e 6520 666f 6e63 7469 6f6e  oir une fonction
-00008240: 2050 7974 686f 6e20 7175 6920 6573 7420   Python qui est 
-00008250: 6170 7065 6cc3 a965 206c 6f72 7371 7565  appel..e lorsque
-00008260: 206c 6520 666f 726d 756c 6169 7265 2065   le formulaire e
-00008270: 7374 0a6f 7576 6572 742e 0a0a 5574 696c  st.ouvert...Util
-00008280: 6973 657a 2063 6574 7465 2066 6f6e 6374  isez cette fonct
-00008290: 696f 6e20 706f 7572 2061 6a6f 7574 6572  ion pour ajouter
-000082a0: 2075 6e65 206c 6f67 6971 7565 2073 7570   une logique sup
-000082b0: 706c c3a9 6d65 6e74 6169 7265 20c3 a020  pl..mentaire .. 
-000082c0: 766f 7320 666f 726d 756c 6169 7265 732e  vos formulaires.
-000082d0: 0a0a 456e 7472 657a 206c 6520 6e6f 6d20  ..Entrez le nom 
-000082e0: 6465 206c 6120 666f 6e63 7469 6f6e 2064  de la fonction d
-000082f0: 616e 7320 6c65 2063 6861 6d70 200a 2246  ans le champ ."F
-00008300: 6f6e 6374 696f 6e20 6427 696e 6974 6961  onction d'initia
-00008310: 6c69 7361 7469 6f6e 2050 7974 686f 6e22  lisation Python"
-00008320: 2e0a 566f 6963 6920 756e 2065 7865 6d70  ..Voici un exemp
-00008330: 6c65 3a0a 2222 220a 6672 6f6d 2071 6769  le:.""".from qgi
-00008340: 732e 5079 5174 2e51 7457 6964 6765 7473  s.PyQt.QtWidgets
-00008350: 2069 6d70 6f72 7420 5157 6964 6765 740a   import QWidget.
-00008360: 0a64 6566 206d 795f 666f 726d 5f6f 7065  .def my_form_ope
-00008370: 6e28 6469 616c 6f67 2c20 6c61 7965 722c  n(dialog, layer,
-00008380: 2066 6561 7475 7265 293a 0a20 2020 2067   feature):.    g
-00008390: 656f 6d20 3d20 6665 6174 7572 652e 6765  eom = feature.ge
-000083a0: 6f6d 6574 7279 2829 0a20 2020 2063 6f6e  ometry().    con
-000083b0: 7472 6f6c 203d 2064 6961 6c6f 672e 6669  trol = dialog.fi
-000083c0: 6e64 4368 696c 6428 5157 6964 6765 742c  ndChild(QWidget,
-000083d0: 2022 4d79 4c69 6e65 4564 6974 2229 0a5d   "MyLineEdit").]
-000083e0: 5d3e 3c2f 6564 6974 666f 726d 696e 6974  ]></editforminit
-000083f0: 636f 6465 3e0a 2020 3c66 6561 7466 6f72  code>.  <featfor
-00008400: 6d73 7570 7072 6573 733e 303c 2f66 6561  msuppress>0</fea
-00008410: 7466 6f72 6d73 7570 7072 6573 733e 0a20  tformsuppress>. 
-00008420: 203c 6564 6974 6f72 6c61 796f 7574 3e67   <editorlayout>g
-00008430: 656e 6572 6174 6564 6c61 796f 7574 3c2f  eneratedlayout</
-00008440: 6564 6974 6f72 6c61 796f 7574 3e0a 2020  editorlayout>.  
-00008450: 3c65 6469 7461 626c 653e 0a20 2020 203c  <editable>.    <
-00008460: 6669 656c 6420 6e61 6d65 3d22 616e 676c  field name="angl
-00008470: 6522 2065 6469 7461 626c 653d 2231 222f  e" editable="1"/
-00008480: 3e0a 2020 2020 3c66 6965 6c64 206e 616d  >.    <field nam
-00008490: 653d 2266 6964 2220 6564 6974 6162 6c65  e="fid" editable
-000084a0: 3d22 3122 2f3e 0a20 2020 203c 6669 656c  ="1"/>.    <fiel
-000084b0: 6420 6e61 6d65 3d22 6c61 6e65 5f6f 7269  d name="lane_ori
-000084c0: 656e 7461 7469 6f6e 2220 6564 6974 6162  entation" editab
-000084d0: 6c65 3d22 3122 2f3e 0a20 2020 203c 6669  le="1"/>.    <fi
-000084e0: 656c 6420 6e61 6d65 3d22 6c61 6e65 5f77  eld name="lane_w
-000084f0: 6964 7468 2220 6564 6974 6162 6c65 3d22  idth" editable="
-00008500: 3122 2f3e 0a20 2020 203c 6669 656c 6420  1"/>.    <field 
-00008510: 6e61 6d65 3d22 6f72 6965 6e74 6174 696f  name="orientatio
-00008520: 6e22 2065 6469 7461 626c 653d 2231 222f  n" editable="1"/
-00008530: 3e0a 2020 2020 3c66 6965 6c64 206e 616d  >.    <field nam
-00008540: 653d 226f 7269 656e 7461 7469 6f6e 5f63  e="orientation_c
-00008550: 6f6e 6669 6465 6e63 6522 2065 6469 7461  onfidence" edita
-00008560: 626c 653d 2231 222f 3e0a 2020 2020 3c66  ble="1"/>.    <f
-00008570: 6965 6c64 206e 616d 653d 226f 736d 5f69  ield name="osm_i
-00008580: 6422 2065 6469 7461 626c 653d 2231 222f  d" editable="1"/
-00008590: 3e0a 2020 2020 3c66 6965 6c64 206e 616d  >.    <field nam
-000085a0: 653d 2274 7970 6522 2065 6469 7461 626c  e="type" editabl
-000085b0: 653d 2231 222f 3e0a 2020 3c2f 6564 6974  e="1"/>.  </edit
-000085c0: 6162 6c65 3e0a 2020 3c6c 6162 656c 4f6e  able>.  <labelOn
-000085d0: 546f 703e 0a20 2020 203c 6669 656c 6420  Top>.    <field 
-000085e0: 6c61 6265 6c4f 6e54 6f70 3d22 3022 206e  labelOnTop="0" n
-000085f0: 616d 653d 2261 6e67 6c65 222f 3e0a 2020  ame="angle"/>.  
-00008600: 2020 3c66 6965 6c64 206c 6162 656c 4f6e    <field labelOn
-00008610: 546f 703d 2230 2220 6e61 6d65 3d22 6669  Top="0" name="fi
-00008620: 6422 2f3e 0a20 2020 203c 6669 656c 6420  d"/>.    <field 
-00008630: 6c61 6265 6c4f 6e54 6f70 3d22 3022 206e  labelOnTop="0" n
-00008640: 616d 653d 226c 616e 655f 6f72 6965 6e74  ame="lane_orient
-00008650: 6174 696f 6e22 2f3e 0a20 2020 203c 6669  ation"/>.    <fi
-00008660: 656c 6420 6c61 6265 6c4f 6e54 6f70 3d22  eld labelOnTop="
-00008670: 3022 206e 616d 653d 226c 616e 655f 7769  0" name="lane_wi
-00008680: 6474 6822 2f3e 0a20 2020 203c 6669 656c  dth"/>.    <fiel
-00008690: 6420 6c61 6265 6c4f 6e54 6f70 3d22 3022  d labelOnTop="0"
-000086a0: 206e 616d 653d 226f 7269 656e 7461 7469   name="orientati
-000086b0: 6f6e 222f 3e0a 2020 2020 3c66 6965 6c64  on"/>.    <field
-000086c0: 206c 6162 656c 4f6e 546f 703d 2230 2220   labelOnTop="0" 
-000086d0: 6e61 6d65 3d22 6f72 6965 6e74 6174 696f  name="orientatio
-000086e0: 6e5f 636f 6e66 6964 656e 6365 222f 3e0a  n_confidence"/>.
-000086f0: 2020 2020 3c66 6965 6c64 206c 6162 656c      <field label
-00008700: 4f6e 546f 703d 2230 2220 6e61 6d65 3d22  OnTop="0" name="
-00008710: 6f73 6d5f 6964 222f 3e0a 2020 2020 3c66  osm_id"/>.    <f
-00008720: 6965 6c64 206c 6162 656c 4f6e 546f 703d  ield labelOnTop=
-00008730: 2230 2220 6e61 6d65 3d22 7479 7065 222f  "0" name="type"/
-00008740: 3e0a 2020 3c2f 6c61 6265 6c4f 6e54 6f70  >.  </labelOnTop
-00008750: 3e0a 2020 3c72 6575 7365 4c61 7374 5661  >.  <reuseLastVa
-00008760: 6c75 653e 0a20 2020 203c 6669 656c 6420  lue>.    <field 
-00008770: 6e61 6d65 3d22 616e 676c 6522 2072 6575  name="angle" reu
-00008780: 7365 4c61 7374 5661 6c75 653d 2230 222f  seLastValue="0"/
-00008790: 3e0a 2020 2020 3c66 6965 6c64 206e 616d  >.    <field nam
-000087a0: 653d 2266 6964 2220 7265 7573 654c 6173  e="fid" reuseLas
-000087b0: 7456 616c 7565 3d22 3022 2f3e 0a20 2020  tValue="0"/>.   
-000087c0: 203c 6669 656c 6420 6e61 6d65 3d22 6c61   <field name="la
-000087d0: 6e65 5f6f 7269 656e 7461 7469 6f6e 2220  ne_orientation" 
-000087e0: 7265 7573 654c 6173 7456 616c 7565 3d22  reuseLastValue="
-000087f0: 3022 2f3e 0a20 2020 203c 6669 656c 6420  0"/>.    <field 
-00008800: 6e61 6d65 3d22 6c61 6e65 5f77 6964 7468  name="lane_width
-00008810: 2220 7265 7573 654c 6173 7456 616c 7565  " reuseLastValue
-00008820: 3d22 3022 2f3e 0a20 2020 203c 6669 656c  ="0"/>.    <fiel
-00008830: 6420 6e61 6d65 3d22 6f72 6965 6e74 6174  d name="orientat
-00008840: 696f 6e22 2072 6575 7365 4c61 7374 5661  ion" reuseLastVa
-00008850: 6c75 653d 2230 222f 3e0a 2020 2020 3c66  lue="0"/>.    <f
-00008860: 6965 6c64 206e 616d 653d 226f 7269 656e  ield name="orien
-00008870: 7461 7469 6f6e 5f63 6f6e 6669 6465 6e63  tation_confidenc
-00008880: 6522 2072 6575 7365 4c61 7374 5661 6c75  e" reuseLastValu
-00008890: 653d 2230 222f 3e0a 2020 2020 3c66 6965  e="0"/>.    <fie
-000088a0: 6c64 206e 616d 653d 226f 736d 5f69 6422  ld name="osm_id"
-000088b0: 2072 6575 7365 4c61 7374 5661 6c75 653d   reuseLastValue=
-000088c0: 2230 222f 3e0a 2020 2020 3c66 6965 6c64  "0"/>.    <field
-000088d0: 206e 616d 653d 2274 7970 6522 2072 6575   name="type" reu
-000088e0: 7365 4c61 7374 5661 6c75 653d 2230 222f  seLastValue="0"/
-000088f0: 3e0a 2020 3c2f 7265 7573 654c 6173 7456  >.  </reuseLastV
-00008900: 616c 7565 3e0a 2020 3c64 6174 6144 6566  alue>.  <dataDef
-00008910: 696e 6564 4669 656c 6450 726f 7065 7274  inedFieldPropert
-00008920: 6965 732f 3e0a 2020 3c77 6964 6765 7473  ies/>.  <widgets
-00008930: 2f3e 0a20 203c 7072 6576 6965 7745 7870  />.  <previewExp
-00008940: 7265 7373 696f 6e3e 2274 7970 6522 3c2f  ression>"type"</
-00008950: 7072 6576 6965 7745 7870 7265 7373 696f  previewExpressio
-00008960: 6e3e 0a20 203c 6d61 7054 6970 3e3c 2f6d  n>.  <mapTip></m
-00008970: 6170 5469 703e 0a20 203c 6c61 7965 7247  apTip>.  <layerG
-00008980: 656f 6d65 7472 7954 7970 653e 303c 2f6c  eometryType>0</l
-00008990: 6179 6572 4765 6f6d 6574 7279 5479 7065  ayerGeometryType
-000089a0: 3e0a 3c2f 7167 6973 3e0a                 >.</qgis>.
+00003890: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+000038a0: 3930 202b 2028 2d26 7175 6f74 3b6f 7269  90 + (-&quot;ori
+000038b0: 656e 7461 7469 6f6e 2671 756f 743b 202f  entation&quot; /
+000038c0: 2070 6928 2929 202a 2031 3830 2220 6e61   pi()) * 180" na
+000038d0: 6d65 3d22 6578 7072 6573 7369 6f6e 2220  me="expression" 
+000038e0: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+000038f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003900: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
+00003910: 3d22 3322 206e 616d 653d 2274 7970 6522  ="3" name="type"
+00003920: 2074 7970 653d 2269 6e74 222f 3e0a 2020   type="int"/>.  
+00003930: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00003940: 4f70 7469 6f6e 3e0a 2020 2020 2020 2020  Option>.        
+00003950: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00003960: 6e61 6d65 3d22 6f75 746c 696e 6557 6964  name="outlineWid
+00003970: 7468 2220 7479 7065 3d22 4d61 7022 3e0a  th" type="Map">.
+00003980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003990: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+000039a0: 2274 7275 6522 206e 616d 653d 2261 6374  "true" name="act
+000039b0: 6976 6522 2074 7970 653d 2262 6f6f 6c22  ive" type="bool"
+000039c0: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+000039d0: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
+000039e0: 7565 3d22 2671 756f 743b 6c61 6e65 5f77  ue="&quot;lane_w
+000039f0: 6964 7468 2671 756f 743b 202a 2030 2e37  idth&quot; * 0.7
+00003a00: 2220 6e61 6d65 3d22 6578 7072 6573 7369  " name="expressi
+00003a10: 6f6e 2220 7479 7065 3d22 5153 7472 696e  on" type="QStrin
+00003a20: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00003a30: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
+00003a40: 616c 7565 3d22 3322 206e 616d 653d 2274  alue="3" name="t
+00003a50: 7970 6522 2074 7970 653d 2269 6e74 222f  ype" type="int"/
+00003a60: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00003a70: 2020 3c2f 4f70 7469 6f6e 3e0a 2020 2020    </Option>.    
+00003a80: 2020 2020 2020 2020 2020 3c2f 4f70 7469            </Opti
+00003a90: 6f6e 3e0a 2020 2020 2020 2020 2020 2020  on>.            
+00003aa0: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+00003ab0: 2263 6f6c 6c65 6374 696f 6e22 206e 616d  "collection" nam
+00003ac0: 653d 2274 7970 6522 2074 7970 653d 2251  e="type" type="Q
+00003ad0: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+00003ae0: 2020 2020 2020 3c2f 4f70 7469 6f6e 3e0a        </Option>.
+00003af0: 2020 2020 2020 2020 2020 3c2f 6461 7461            </data
+00003b00: 5f64 6566 696e 6564 5f70 726f 7065 7274  _defined_propert
+00003b10: 6965 733e 0a20 2020 2020 2020 203c 2f6c  ies>.        </l
+00003b20: 6179 6572 3e0a 2020 2020 2020 3c2f 7379  ayer>.      </sy
+00003b30: 6d62 6f6c 3e0a 2020 2020 2020 3c73 796d  mbol>.      <sym
+00003b40: 626f 6c20 6672 616d 655f 7261 7465 3d22  bol frame_rate="
+00003b50: 3130 2220 6973 5f61 6e69 6d61 7465 643d  10" is_animated=
+00003b60: 2230 2220 6e61 6d65 3d22 3222 2061 6c70  "0" name="2" alp
+00003b70: 6861 3d22 3122 2066 6f72 6365 5f72 6872  ha="1" force_rhr
+00003b80: 3d22 3022 2063 6c69 705f 746f 5f65 7874  ="0" clip_to_ext
+00003b90: 656e 743d 2231 2220 7479 7065 3d22 6d61  ent="1" type="ma
+00003ba0: 726b 6572 223e 0a20 2020 2020 2020 203c  rker">.        <
+00003bb0: 6461 7461 5f64 6566 696e 6564 5f70 726f  data_defined_pro
+00003bc0: 7065 7274 6965 733e 0a20 2020 2020 2020  perties>.       
+00003bd0: 2020 203c 4f70 7469 6f6e 2074 7970 653d     <Option type=
+00003be0: 224d 6170 223e 0a20 2020 2020 2020 2020  "Map">.         
+00003bf0: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
+00003c00: 3d22 2220 6e61 6d65 3d22 6e61 6d65 2220  ="" name="name" 
+00003c10: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00003c20: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
+00003c30: 7469 6f6e 206e 616d 653d 2270 726f 7065  tion name="prope
+00003c40: 7274 6965 7322 2f3e 0a20 2020 2020 2020  rties"/>.       
+00003c50: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
+00003c60: 7565 3d22 636f 6c6c 6563 7469 6f6e 2220  ue="collection" 
+00003c70: 6e61 6d65 3d22 7479 7065 2220 7479 7065  name="type" type
+00003c80: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+00003c90: 2020 2020 2020 203c 2f4f 7074 696f 6e3e         </Option>
+00003ca0: 0a20 2020 2020 2020 203c 2f64 6174 615f  .        </data_
+00003cb0: 6465 6669 6e65 645f 7072 6f70 6572 7469  defined_properti
+00003cc0: 6573 3e0a 2020 2020 2020 2020 3c6c 6179  es>.        <lay
+00003cd0: 6572 2065 6e61 626c 6564 3d22 3122 2063  er enabled="1" c
+00003ce0: 6c61 7373 3d22 5369 6d70 6c65 4d61 726b  lass="SimpleMark
+00003cf0: 6572 2220 6c6f 636b 6564 3d22 3022 2070  er" locked="0" p
+00003d00: 6173 733d 2230 223e 0a20 2020 2020 2020  ass="0">.       
+00003d10: 2020 203c 4f70 7469 6f6e 2074 7970 653d     <Option type=
+00003d20: 224d 6170 223e 0a20 2020 2020 2020 2020  "Map">.         
+00003d30: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
+00003d40: 3d22 3022 206e 616d 653d 2261 6e67 6c65  ="0" name="angle
+00003d50: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00003d60: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
+00003d70: 4f70 7469 6f6e 2076 616c 7565 3d22 666c  Option value="fl
+00003d80: 6174 2220 6e61 6d65 3d22 6361 705f 7374  at" name="cap_st
+00003d90: 796c 6522 2074 7970 653d 2251 5374 7269  yle" type="QStri
+00003da0: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+00003db0: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+00003dc0: 2232 3332 2c38 352c 302c 3235 3522 206e  "232,85,0,255" n
+00003dd0: 616d 653d 2263 6f6c 6f72 2220 7479 7065  ame="color" type
+00003de0: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+00003df0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00003e00: 2076 616c 7565 3d22 3122 206e 616d 653d   value="1" name=
+00003e10: 2268 6f72 697a 6f6e 7461 6c5f 616e 6368  "horizontal_anch
+00003e20: 6f72 5f70 6f69 6e74 2220 7479 7065 3d22  or_point" type="
+00003e30: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+00003e40: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
+00003e50: 616c 7565 3d22 6265 7665 6c22 206e 616d  alue="bevel" nam
+00003e60: 653d 226a 6f69 6e73 7479 6c65 2220 7479  e="joinstyle" ty
+00003e70: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+00003e80: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00003e90: 6f6e 2076 616c 7565 3d22 6c69 6e65 2220  on value="line" 
+00003ea0: 6e61 6d65 3d22 6e61 6d65 2220 7479 7065  name="name" type
+00003eb0: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+00003ec0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00003ed0: 2076 616c 7565 3d22 302c 3022 206e 616d   value="0,0" nam
+00003ee0: 653d 226f 6666 7365 7422 2074 7970 653d  e="offset" type=
+00003ef0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00003f00: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00003f10: 7661 6c75 653d 2233 783a 302c 302c 302c  value="3x:0,0,0,
+00003f20: 302c 302c 3022 206e 616d 653d 226f 6666  0,0,0" name="off
+00003f30: 7365 745f 6d61 705f 756e 6974 5f73 6361  set_map_unit_sca
+00003f40: 6c65 2220 7479 7065 3d22 5153 7472 696e  le" type="QStrin
+00003f50: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00003f60: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+00003f70: 4d4d 2220 6e61 6d65 3d22 6f66 6673 6574  MM" name="offset
+00003f80: 5f75 6e69 7422 2074 7970 653d 2251 5374  _unit" type="QSt
+00003f90: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+00003fa0: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
+00003fb0: 653d 2232 3535 2c32 3535 2c32 3535 2c32  e="255,255,255,2
+00003fc0: 3535 2220 6e61 6d65 3d22 6f75 746c 696e  55" name="outlin
+00003fd0: 655f 636f 6c6f 7222 2074 7970 653d 2251  e_color" type="Q
+00003fe0: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+00003ff0: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
+00004000: 6c75 653d 2273 6f6c 6964 2220 6e61 6d65  lue="solid" name
+00004010: 3d22 6f75 746c 696e 655f 7374 796c 6522  ="outline_style"
+00004020: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+00004030: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
+00004040: 7074 696f 6e20 7661 6c75 653d 2232 2220  ption value="2" 
+00004050: 6e61 6d65 3d22 6f75 746c 696e 655f 7769  name="outline_wi
+00004060: 6474 6822 2074 7970 653d 2251 5374 7269  dth" type="QStri
+00004070: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+00004080: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+00004090: 2233 783a 302c 302c 302c 302c 302c 3022  "3x:0,0,0,0,0,0"
+000040a0: 206e 616d 653d 226f 7574 6c69 6e65 5f77   name="outline_w
+000040b0: 6964 7468 5f6d 6170 5f75 6e69 745f 7363  idth_map_unit_sc
+000040c0: 616c 6522 2074 7970 653d 2251 5374 7269  ale" type="QStri
+000040d0: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+000040e0: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+000040f0: 2252 656e 6465 724d 6574 6572 7349 6e4d  "RenderMetersInM
+00004100: 6170 556e 6974 7322 206e 616d 653d 226f  apUnits" name="o
+00004110: 7574 6c69 6e65 5f77 6964 7468 5f75 6e69  utline_width_uni
+00004120: 7422 2074 7970 653d 2251 5374 7269 6e67  t" type="QString
+00004130: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00004140: 3c4f 7074 696f 6e20 7661 6c75 653d 2264  <Option value="d
+00004150: 6961 6d65 7465 7222 206e 616d 653d 2273  iameter" name="s
+00004160: 6361 6c65 5f6d 6574 686f 6422 2074 7970  cale_method" typ
+00004170: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00004180: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00004190: 6e20 7661 6c75 653d 2233 2220 6e61 6d65  n value="3" name
+000041a0: 3d22 7369 7a65 2220 7479 7065 3d22 5153  ="size" type="QS
+000041b0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+000041c0: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
+000041d0: 7565 3d22 3378 3a30 2c30 2c30 2c30 2c30  ue="3x:0,0,0,0,0
+000041e0: 2c30 2220 6e61 6d65 3d22 7369 7a65 5f6d  ,0" name="size_m
+000041f0: 6170 5f75 6e69 745f 7363 616c 6522 2074  ap_unit_scale" t
+00004200: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
+00004210: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00004220: 696f 6e20 7661 6c75 653d 2252 656e 6465  ion value="Rende
+00004230: 724d 6574 6572 7349 6e4d 6170 556e 6974  rMetersInMapUnit
+00004240: 7322 206e 616d 653d 2273 697a 655f 756e  s" name="size_un
+00004250: 6974 2220 7479 7065 3d22 5153 7472 696e  it" type="QStrin
+00004260: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00004270: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+00004280: 3122 206e 616d 653d 2276 6572 7469 6361  1" name="vertica
+00004290: 6c5f 616e 6368 6f72 5f70 6f69 6e74 2220  l_anchor_point" 
+000042a0: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+000042b0: 0a20 2020 2020 2020 2020 203c 2f4f 7074  .          </Opt
+000042c0: 696f 6e3e 0a20 2020 2020 2020 2020 203c  ion>.          <
+000042d0: 6461 7461 5f64 6566 696e 6564 5f70 726f  data_defined_pro
+000042e0: 7065 7274 6965 733e 0a20 2020 2020 2020  perties>.       
+000042f0: 2020 2020 203c 4f70 7469 6f6e 2074 7970       <Option typ
+00004300: 653d 224d 6170 223e 0a20 2020 2020 2020  e="Map">.       
+00004310: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
+00004320: 616c 7565 3d22 2220 6e61 6d65 3d22 6e61  alue="" name="na
+00004330: 6d65 2220 7479 7065 3d22 5153 7472 696e  me" type="QStrin
+00004340: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00004350: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
+00004360: 2270 726f 7065 7274 6965 7322 2074 7970  "properties" typ
+00004370: 653d 224d 6170 223e 0a20 2020 2020 2020  e="Map">.       
+00004380: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00004390: 206e 616d 653d 2261 6e67 6c65 2220 7479   name="angle" ty
+000043a0: 7065 3d22 4d61 7022 3e0a 2020 2020 2020  pe="Map">.      
+000043b0: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+000043c0: 696f 6e20 7661 6c75 653d 2274 7275 6522  ion value="true"
+000043d0: 206e 616d 653d 2261 6374 6976 6522 2074   name="active" t
+000043e0: 7970 653d 2262 6f6f 6c22 2f3e 0a20 2020  ype="bool"/>.   
+000043f0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00004400: 4f70 7469 6f6e 2076 616c 7565 3d22 3930  Option value="90
+00004410: 202b 2028 2d26 7175 6f74 3b6f 7269 656e   + (-&quot;orien
+00004420: 7461 7469 6f6e 2671 756f 743b 202f 2070  tation&quot; / p
+00004430: 6928 2929 202a 2031 3830 2220 6e61 6d65  i()) * 180" name
+00004440: 3d22 6578 7072 6573 7369 6f6e 2220 7479  ="expression" ty
+00004450: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+00004460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004470: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+00004480: 3322 206e 616d 653d 2274 7970 6522 2074  3" name="type" t
+00004490: 7970 653d 2269 6e74 222f 3e0a 2020 2020  ype="int"/>.    
+000044a0: 2020 2020 2020 2020 2020 2020 3c2f 4f70              </Op
+000044b0: 7469 6f6e 3e0a 2020 2020 2020 2020 2020  tion>.          
+000044c0: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
+000044d0: 6d65 3d22 6f75 746c 696e 6557 6964 7468  me="outlineWidth
+000044e0: 2220 7479 7065 3d22 4d61 7022 3e0a 2020  " type="Map">.  
+000044f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004500: 3c4f 7074 696f 6e20 7661 6c75 653d 2274  <Option value="t
+00004510: 7275 6522 206e 616d 653d 2261 6374 6976  rue" name="activ
+00004520: 6522 2074 7970 653d 2262 6f6f 6c22 2f3e  e" type="bool"/>
+00004530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004540: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
+00004550: 3d22 2671 756f 743b 6c61 6e65 5f77 6964  ="&quot;lane_wid
+00004560: 7468 2671 756f 743b 2220 6e61 6d65 3d22  th&quot;" name="
+00004570: 6578 7072 6573 7369 6f6e 2220 7479 7065  expression" type
+00004580: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+00004590: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000045a0: 4f70 7469 6f6e 2076 616c 7565 3d22 3322  Option value="3"
+000045b0: 206e 616d 653d 2274 7970 6522 2074 7970   name="type" typ
+000045c0: 653d 2269 6e74 222f 3e0a 2020 2020 2020  e="int"/>.      
+000045d0: 2020 2020 2020 2020 2020 3c2f 4f70 7469            </Opti
+000045e0: 6f6e 3e0a 2020 2020 2020 2020 2020 2020  on>.            
+000045f0: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
+00004600: 3d22 7369 7a65 2220 7479 7065 3d22 4d61  ="size" type="Ma
+00004610: 7022 3e0a 2020 2020 2020 2020 2020 2020  p">.            
+00004620: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
+00004630: 6c75 653d 2274 7275 6522 206e 616d 653d  lue="true" name=
+00004640: 2261 6374 6976 6522 2074 7970 653d 2262  "active" type="b
+00004650: 6f6f 6c22 2f3e 0a20 2020 2020 2020 2020  ool"/>.         
+00004660: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00004670: 2076 616c 7565 3d22 3320 2d20 3220 2a20   value="3 - 2 * 
+00004680: 302e 3030 3120 2a20 406d 6170 5f73 6361  0.001 * @map_sca
+00004690: 6c65 2220 6e61 6d65 3d22 6578 7072 6573  le" name="expres
+000046a0: 7369 6f6e 2220 7479 7065 3d22 5153 7472  sion" type="QStr
+000046b0: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+000046c0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+000046d0: 2076 616c 7565 3d22 3322 206e 616d 653d   value="3" name=
+000046e0: 2274 7970 6522 2074 7970 653d 2269 6e74  "type" type="int
+000046f0: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00004700: 2020 2020 3c2f 4f70 7469 6f6e 3e0a 2020      </Option>.  
+00004710: 2020 2020 2020 2020 2020 2020 3c2f 4f70              </Op
+00004720: 7469 6f6e 3e0a 2020 2020 2020 2020 2020  tion>.          
+00004730: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
+00004740: 653d 2263 6f6c 6c65 6374 696f 6e22 206e  e="collection" n
+00004750: 616d 653d 2274 7970 6522 2074 7970 653d  ame="type" type=
+00004760: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00004770: 2020 2020 2020 2020 3c2f 4f70 7469 6f6e          </Option
+00004780: 3e0a 2020 2020 2020 2020 2020 3c2f 6461  >.          </da
+00004790: 7461 5f64 6566 696e 6564 5f70 726f 7065  ta_defined_prope
+000047a0: 7274 6965 733e 0a20 2020 2020 2020 203c  rties>.        <
+000047b0: 2f6c 6179 6572 3e0a 2020 2020 2020 3c2f  /layer>.      </
+000047c0: 7379 6d62 6f6c 3e0a 2020 2020 2020 3c73  symbol>.      <s
+000047d0: 796d 626f 6c20 6672 616d 655f 7261 7465  ymbol frame_rate
+000047e0: 3d22 3130 2220 6973 5f61 6e69 6d61 7465  ="10" is_animate
+000047f0: 643d 2230 2220 6e61 6d65 3d22 3322 2061  d="0" name="3" a
+00004800: 6c70 6861 3d22 3122 2066 6f72 6365 5f72  lpha="1" force_r
+00004810: 6872 3d22 3022 2063 6c69 705f 746f 5f65  hr="0" clip_to_e
+00004820: 7874 656e 743d 2231 2220 7479 7065 3d22  xtent="1" type="
+00004830: 6d61 726b 6572 223e 0a20 2020 2020 2020  marker">.       
+00004840: 203c 6461 7461 5f64 6566 696e 6564 5f70   <data_defined_p
+00004850: 726f 7065 7274 6965 733e 0a20 2020 2020  roperties>.     
+00004860: 2020 2020 203c 4f70 7469 6f6e 2074 7970       <Option typ
+00004870: 653d 224d 6170 223e 0a20 2020 2020 2020  e="Map">.       
+00004880: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
+00004890: 7565 3d22 2220 6e61 6d65 3d22 6e61 6d65  ue="" name="name
+000048a0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+000048b0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
+000048c0: 4f70 7469 6f6e 206e 616d 653d 2270 726f  Option name="pro
+000048d0: 7065 7274 6965 7322 2f3e 0a20 2020 2020  perties"/>.     
+000048e0: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
+000048f0: 616c 7565 3d22 636f 6c6c 6563 7469 6f6e  alue="collection
+00004900: 2220 6e61 6d65 3d22 7479 7065 2220 7479  " name="type" ty
+00004910: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+00004920: 2020 2020 2020 2020 203c 2f4f 7074 696f           </Optio
+00004930: 6e3e 0a20 2020 2020 2020 203c 2f64 6174  n>.        </dat
+00004940: 615f 6465 6669 6e65 645f 7072 6f70 6572  a_defined_proper
+00004950: 7469 6573 3e0a 2020 2020 2020 2020 3c6c  ties>.        <l
+00004960: 6179 6572 2065 6e61 626c 6564 3d22 3122  ayer enabled="1"
+00004970: 2063 6c61 7373 3d22 5369 6d70 6c65 4d61   class="SimpleMa
+00004980: 726b 6572 2220 6c6f 636b 6564 3d22 3022  rker" locked="0"
+00004990: 2070 6173 733d 2230 223e 0a20 2020 2020   pass="0">.     
+000049a0: 2020 2020 203c 4f70 7469 6f6e 2074 7970       <Option typ
+000049b0: 653d 224d 6170 223e 0a20 2020 2020 2020  e="Map">.       
+000049c0: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
+000049d0: 7565 3d22 3022 206e 616d 653d 2261 6e67  ue="0" name="ang
+000049e0: 6c65 2220 7479 7065 3d22 5153 7472 696e  le" type="QStrin
+000049f0: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00004a00: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+00004a10: 666c 6174 2220 6e61 6d65 3d22 6361 705f  flat" name="cap_
+00004a20: 7374 796c 6522 2074 7970 653d 2251 5374  style" type="QSt
+00004a30: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+00004a40: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
+00004a50: 653d 2232 3332 2c38 352c 302c 3235 3522  e="232,85,0,255"
+00004a60: 206e 616d 653d 2263 6f6c 6f72 2220 7479   name="color" ty
+00004a70: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+00004a80: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00004a90: 6f6e 2076 616c 7565 3d22 3122 206e 616d  on value="1" nam
+00004aa0: 653d 2268 6f72 697a 6f6e 7461 6c5f 616e  e="horizontal_an
+00004ab0: 6368 6f72 5f70 6f69 6e74 2220 7479 7065  chor_point" type
+00004ac0: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+00004ad0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00004ae0: 2076 616c 7565 3d22 6265 7665 6c22 206e   value="bevel" n
+00004af0: 616d 653d 226a 6f69 6e73 7479 6c65 2220  ame="joinstyle" 
+00004b00: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00004b10: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
+00004b20: 7469 6f6e 2076 616c 7565 3d22 6c69 6e65  tion value="line
+00004b30: 2220 6e61 6d65 3d22 6e61 6d65 2220 7479  " name="name" ty
+00004b40: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+00004b50: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00004b60: 6f6e 2076 616c 7565 3d22 302c 3022 206e  on value="0,0" n
+00004b70: 616d 653d 226f 6666 7365 7422 2074 7970  ame="offset" typ
+00004b80: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00004b90: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00004ba0: 6e20 7661 6c75 653d 2233 783a 302c 302c  n value="3x:0,0,
+00004bb0: 302c 302c 302c 3022 206e 616d 653d 226f  0,0,0,0" name="o
+00004bc0: 6666 7365 745f 6d61 705f 756e 6974 5f73  ffset_map_unit_s
+00004bd0: 6361 6c65 2220 7479 7065 3d22 5153 7472  cale" type="QStr
+00004be0: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+00004bf0: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
+00004c00: 3d22 4d4d 2220 6e61 6d65 3d22 6f66 6673  ="MM" name="offs
+00004c10: 6574 5f75 6e69 7422 2074 7970 653d 2251  et_unit" type="Q
+00004c20: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+00004c30: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
+00004c40: 6c75 653d 2232 3535 2c32 3535 2c32 3535  lue="255,255,255
+00004c50: 2c32 3535 2220 6e61 6d65 3d22 6f75 746c  ,255" name="outl
+00004c60: 696e 655f 636f 6c6f 7222 2074 7970 653d  ine_color" type=
+00004c70: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00004c80: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00004c90: 7661 6c75 653d 2273 6f6c 6964 2220 6e61  value="solid" na
+00004ca0: 6d65 3d22 6f75 746c 696e 655f 7374 796c  me="outline_styl
+00004cb0: 6522 2074 7970 653d 2251 5374 7269 6e67  e" type="QString
+00004cc0: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00004cd0: 3c4f 7074 696f 6e20 7661 6c75 653d 2232  <Option value="2
+00004ce0: 2220 6e61 6d65 3d22 6f75 746c 696e 655f  " name="outline_
+00004cf0: 7769 6474 6822 2074 7970 653d 2251 5374  width" type="QSt
+00004d00: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+00004d10: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
+00004d20: 653d 2233 783a 302c 302c 302c 302c 302c  e="3x:0,0,0,0,0,
+00004d30: 3022 206e 616d 653d 226f 7574 6c69 6e65  0" name="outline
+00004d40: 5f77 6964 7468 5f6d 6170 5f75 6e69 745f  _width_map_unit_
+00004d50: 7363 616c 6522 2074 7970 653d 2251 5374  scale" type="QSt
+00004d60: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+00004d70: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
+00004d80: 653d 2252 656e 6465 724d 6574 6572 7349  e="RenderMetersI
+00004d90: 6e4d 6170 556e 6974 7322 206e 616d 653d  nMapUnits" name=
+00004da0: 226f 7574 6c69 6e65 5f77 6964 7468 5f75  "outline_width_u
+00004db0: 6e69 7422 2074 7970 653d 2251 5374 7269  nit" type="QStri
+00004dc0: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+00004dd0: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+00004de0: 2264 6961 6d65 7465 7222 206e 616d 653d  "diameter" name=
+00004df0: 2273 6361 6c65 5f6d 6574 686f 6422 2074  "scale_method" t
+00004e00: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
+00004e10: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00004e20: 696f 6e20 7661 6c75 653d 2233 2220 6e61  ion value="3" na
+00004e30: 6d65 3d22 7369 7a65 2220 7479 7065 3d22  me="size" type="
+00004e40: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+00004e50: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
+00004e60: 616c 7565 3d22 3378 3a30 2c30 2c30 2c30  alue="3x:0,0,0,0
+00004e70: 2c30 2c30 2220 6e61 6d65 3d22 7369 7a65  ,0,0" name="size
+00004e80: 5f6d 6170 5f75 6e69 745f 7363 616c 6522  _map_unit_scale"
+00004e90: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+00004ea0: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
+00004eb0: 7074 696f 6e20 7661 6c75 653d 2252 656e  ption value="Ren
+00004ec0: 6465 724d 6574 6572 7349 6e4d 6170 556e  derMetersInMapUn
+00004ed0: 6974 7322 206e 616d 653d 2273 697a 655f  its" name="size_
+00004ee0: 756e 6974 2220 7479 7065 3d22 5153 7472  unit" type="QStr
+00004ef0: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+00004f00: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
+00004f10: 3d22 3122 206e 616d 653d 2276 6572 7469  ="1" name="verti
+00004f20: 6361 6c5f 616e 6368 6f72 5f70 6f69 6e74  cal_anchor_point
+00004f30: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00004f40: 2f3e 0a20 2020 2020 2020 2020 203c 2f4f  />.          </O
+00004f50: 7074 696f 6e3e 0a20 2020 2020 2020 2020  ption>.         
+00004f60: 203c 6461 7461 5f64 6566 696e 6564 5f70   <data_defined_p
+00004f70: 726f 7065 7274 6965 733e 0a20 2020 2020  roperties>.     
+00004f80: 2020 2020 2020 203c 4f70 7469 6f6e 2074         <Option t
+00004f90: 7970 653d 224d 6170 223e 0a20 2020 2020  ype="Map">.     
+00004fa0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00004fb0: 2076 616c 7565 3d22 2220 6e61 6d65 3d22   value="" name="
+00004fc0: 6e61 6d65 2220 7479 7065 3d22 5153 7472  name" type="QStr
+00004fd0: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+00004fe0: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
+00004ff0: 653d 2270 726f 7065 7274 6965 7322 2074  e="properties" t
+00005000: 7970 653d 224d 6170 223e 0a20 2020 2020  ype="Map">.     
+00005010: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00005020: 6f6e 206e 616d 653d 2261 6e67 6c65 2220  on name="angle" 
+00005030: 7479 7065 3d22 4d61 7022 3e0a 2020 2020  type="Map">.    
+00005040: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
+00005050: 7074 696f 6e20 7661 6c75 653d 2274 7275  ption value="tru
+00005060: 6522 206e 616d 653d 2261 6374 6976 6522  e" name="active"
+00005070: 2074 7970 653d 2262 6f6f 6c22 2f3e 0a20   type="bool"/>. 
+00005080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005090: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+000050a0: 3930 202b 2028 2d26 7175 6f74 3b6f 7269  90 + (-&quot;ori
+000050b0: 656e 7461 7469 6f6e 2671 756f 743b 202f  entation&quot; /
+000050c0: 2070 6928 2929 202a 2031 3830 2220 6e61   pi()) * 180" na
+000050d0: 6d65 3d22 6578 7072 6573 7369 6f6e 2220  me="expression" 
+000050e0: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+000050f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005100: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
+00005110: 3d22 3322 206e 616d 653d 2274 7970 6522  ="3" name="type"
+00005120: 2074 7970 653d 2269 6e74 222f 3e0a 2020   type="int"/>.  
+00005130: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00005140: 4f70 7469 6f6e 3e0a 2020 2020 2020 2020  Option>.        
+00005150: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00005160: 6e61 6d65 3d22 6f75 746c 696e 6557 6964  name="outlineWid
+00005170: 7468 2220 7479 7065 3d22 4d61 7022 3e0a  th" type="Map">.
+00005180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005190: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+000051a0: 2274 7275 6522 206e 616d 653d 2261 6374  "true" name="act
+000051b0: 6976 6522 2074 7970 653d 2262 6f6f 6c22  ive" type="bool"
+000051c0: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+000051d0: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
+000051e0: 7565 3d22 2671 756f 743b 6c61 6e65 5f77  ue="&quot;lane_w
+000051f0: 6964 7468 2671 756f 743b 2220 6e61 6d65  idth&quot;" name
+00005200: 3d22 6578 7072 6573 7369 6f6e 2220 7479  ="expression" ty
+00005210: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+00005220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005230: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+00005240: 3322 206e 616d 653d 2274 7970 6522 2074  3" name="type" t
+00005250: 7970 653d 2269 6e74 222f 3e0a 2020 2020  ype="int"/>.    
+00005260: 2020 2020 2020 2020 2020 2020 3c2f 4f70              </Op
+00005270: 7469 6f6e 3e0a 2020 2020 2020 2020 2020  tion>.          
+00005280: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
+00005290: 6d65 3d22 7369 7a65 2220 7479 7065 3d22  me="size" type="
+000052a0: 4d61 7022 3e0a 2020 2020 2020 2020 2020  Map">.          
+000052b0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+000052c0: 7661 6c75 653d 2274 7275 6522 206e 616d  value="true" nam
+000052d0: 653d 2261 6374 6976 6522 2074 7970 653d  e="active" type=
+000052e0: 2262 6f6f 6c22 2f3e 0a20 2020 2020 2020  "bool"/>.       
+000052f0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00005300: 6f6e 2076 616c 7565 3d22 3320 2d20 3220  on value="3 - 2 
+00005310: 2a20 302e 3030 3220 2a20 406d 6170 5f73  * 0.002 * @map_s
+00005320: 6361 6c65 2220 6e61 6d65 3d22 6578 7072  cale" name="expr
+00005330: 6573 7369 6f6e 2220 7479 7065 3d22 5153  ession" type="QS
+00005340: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+00005350: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00005360: 6f6e 2076 616c 7565 3d22 3322 206e 616d  on value="3" nam
+00005370: 653d 2274 7970 6522 2074 7970 653d 2269  e="type" type="i
+00005380: 6e74 222f 3e0a 2020 2020 2020 2020 2020  nt"/>.          
+00005390: 2020 2020 2020 3c2f 4f70 7469 6f6e 3e0a        </Option>.
+000053a0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+000053b0: 4f70 7469 6f6e 3e0a 2020 2020 2020 2020  Option>.        
+000053c0: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
+000053d0: 6c75 653d 2263 6f6c 6c65 6374 696f 6e22  lue="collection"
+000053e0: 206e 616d 653d 2274 7970 6522 2074 7970   name="type" typ
+000053f0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00005400: 2020 2020 2020 2020 2020 3c2f 4f70 7469            </Opti
+00005410: 6f6e 3e0a 2020 2020 2020 2020 2020 3c2f  on>.          </
+00005420: 6461 7461 5f64 6566 696e 6564 5f70 726f  data_defined_pro
+00005430: 7065 7274 6965 733e 0a20 2020 2020 2020  perties>.       
+00005440: 203c 2f6c 6179 6572 3e0a 2020 2020 2020   </layer>.      
+00005450: 3c2f 7379 6d62 6f6c 3e0a 2020 2020 2020  </symbol>.      
+00005460: 3c73 796d 626f 6c20 6672 616d 655f 7261  <symbol frame_ra
+00005470: 7465 3d22 3130 2220 6973 5f61 6e69 6d61  te="10" is_anima
+00005480: 7465 643d 2230 2220 6e61 6d65 3d22 3422  ted="0" name="4"
+00005490: 2061 6c70 6861 3d22 3122 2066 6f72 6365   alpha="1" force
+000054a0: 5f72 6872 3d22 3022 2063 6c69 705f 746f  _rhr="0" clip_to
+000054b0: 5f65 7874 656e 743d 2231 2220 7479 7065  _extent="1" type
+000054c0: 3d22 6d61 726b 6572 223e 0a20 2020 2020  ="marker">.     
+000054d0: 2020 203c 6461 7461 5f64 6566 696e 6564     <data_defined
+000054e0: 5f70 726f 7065 7274 6965 733e 0a20 2020  _properties>.   
+000054f0: 2020 2020 2020 203c 4f70 7469 6f6e 2074         <Option t
+00005500: 7970 653d 224d 6170 223e 0a20 2020 2020  ype="Map">.     
+00005510: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
+00005520: 616c 7565 3d22 2220 6e61 6d65 3d22 6e61  alue="" name="na
+00005530: 6d65 2220 7479 7065 3d22 5153 7472 696e  me" type="QStrin
+00005540: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00005550: 203c 4f70 7469 6f6e 206e 616d 653d 2270   <Option name="p
+00005560: 726f 7065 7274 6965 7322 2f3e 0a20 2020  roperties"/>.   
+00005570: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00005580: 2076 616c 7565 3d22 636f 6c6c 6563 7469   value="collecti
+00005590: 6f6e 2220 6e61 6d65 3d22 7479 7065 2220  on" name="type" 
+000055a0: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+000055b0: 0a20 2020 2020 2020 2020 203c 2f4f 7074  .          </Opt
+000055c0: 696f 6e3e 0a20 2020 2020 2020 203c 2f64  ion>.        </d
+000055d0: 6174 615f 6465 6669 6e65 645f 7072 6f70  ata_defined_prop
+000055e0: 6572 7469 6573 3e0a 2020 2020 2020 2020  erties>.        
+000055f0: 3c6c 6179 6572 2065 6e61 626c 6564 3d22  <layer enabled="
+00005600: 3122 2063 6c61 7373 3d22 5369 6d70 6c65  1" class="Simple
+00005610: 4d61 726b 6572 2220 6c6f 636b 6564 3d22  Marker" locked="
+00005620: 3022 2070 6173 733d 2230 223e 0a20 2020  0" pass="0">.   
+00005630: 2020 2020 2020 203c 4f70 7469 6f6e 2074         <Option t
+00005640: 7970 653d 224d 6170 223e 0a20 2020 2020  ype="Map">.     
+00005650: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
+00005660: 616c 7565 3d22 3022 206e 616d 653d 2261  alue="0" name="a
+00005670: 6e67 6c65 2220 7479 7065 3d22 5153 7472  ngle" type="QStr
+00005680: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+00005690: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
+000056a0: 3d22 7371 7561 7265 2220 6e61 6d65 3d22  ="square" name="
+000056b0: 6361 705f 7374 796c 6522 2074 7970 653d  cap_style" type=
+000056c0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+000056d0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+000056e0: 7661 6c75 653d 2230 2c30 2c30 2c32 3535  value="0,0,0,255
+000056f0: 2220 6e61 6d65 3d22 636f 6c6f 7222 2074  " name="color" t
+00005700: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
+00005710: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00005720: 696f 6e20 7661 6c75 653d 2231 2220 6e61  ion value="1" na
+00005730: 6d65 3d22 686f 7269 7a6f 6e74 616c 5f61  me="horizontal_a
+00005740: 6e63 686f 725f 706f 696e 7422 2074 7970  nchor_point" typ
+00005750: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00005760: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00005770: 6e20 7661 6c75 653d 226d 6974 6572 2220  n value="miter" 
+00005780: 6e61 6d65 3d22 6a6f 696e 7374 796c 6522  name="joinstyle"
+00005790: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+000057a0: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
+000057b0: 7074 696f 6e20 7661 6c75 653d 2263 6972  ption value="cir
+000057c0: 636c 6522 206e 616d 653d 226e 616d 6522  cle" name="name"
+000057d0: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+000057e0: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
+000057f0: 7074 696f 6e20 7661 6c75 653d 2230 2c30  ption value="0,0
+00005800: 2220 6e61 6d65 3d22 6f66 6673 6574 2220  " name="offset" 
+00005810: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00005820: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
+00005830: 7469 6f6e 2076 616c 7565 3d22 3378 3a30  tion value="3x:0
+00005840: 2c30 2c30 2c30 2c30 2c30 2220 6e61 6d65  ,0,0,0,0,0" name
+00005850: 3d22 6f66 6673 6574 5f6d 6170 5f75 6e69  ="offset_map_uni
+00005860: 745f 7363 616c 6522 2074 7970 653d 2251  t_scale" type="Q
+00005870: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+00005880: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
+00005890: 6c75 653d 2252 656e 6465 724d 6574 6572  lue="RenderMeter
+000058a0: 7349 6e4d 6170 556e 6974 7322 206e 616d  sInMapUnits" nam
+000058b0: 653d 226f 6666 7365 745f 756e 6974 2220  e="offset_unit" 
+000058c0: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+000058d0: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
+000058e0: 7469 6f6e 2076 616c 7565 3d22 3335 2c33  tion value="35,3
+000058f0: 352c 3335 2c32 3535 2220 6e61 6d65 3d22  5,35,255" name="
+00005900: 6f75 746c 696e 655f 636f 6c6f 7222 2074  outline_color" t
+00005910: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
+00005920: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00005930: 696f 6e20 7661 6c75 653d 2273 6f6c 6964  ion value="solid
+00005940: 2220 6e61 6d65 3d22 6f75 746c 696e 655f  " name="outline_
+00005950: 7374 796c 6522 2074 7970 653d 2251 5374  style" type="QSt
+00005960: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+00005970: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
+00005980: 653d 2230 2220 6e61 6d65 3d22 6f75 746c  e="0" name="outl
+00005990: 696e 655f 7769 6474 6822 2074 7970 653d  ine_width" type=
+000059a0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+000059b0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+000059c0: 7661 6c75 653d 2233 783a 302c 302c 302c  value="3x:0,0,0,
+000059d0: 302c 302c 3022 206e 616d 653d 226f 7574  0,0,0" name="out
+000059e0: 6c69 6e65 5f77 6964 7468 5f6d 6170 5f75  line_width_map_u
+000059f0: 6e69 745f 7363 616c 6522 2074 7970 653d  nit_scale" type=
+00005a00: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00005a10: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00005a20: 7661 6c75 653d 2252 656e 6465 724d 6574  value="RenderMet
+00005a30: 6572 7349 6e4d 6170 556e 6974 7322 206e  ersInMapUnits" n
+00005a40: 616d 653d 226f 7574 6c69 6e65 5f77 6964  ame="outline_wid
+00005a50: 7468 5f75 6e69 7422 2074 7970 653d 2251  th_unit" type="Q
+00005a60: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+00005a70: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
+00005a80: 6c75 653d 2264 6961 6d65 7465 7222 206e  lue="diameter" n
+00005a90: 616d 653d 2273 6361 6c65 5f6d 6574 686f  ame="scale_metho
+00005aa0: 6422 2074 7970 653d 2251 5374 7269 6e67  d" type="QString
+00005ab0: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00005ac0: 3c4f 7074 696f 6e20 7661 6c75 653d 2236  <Option value="6
+00005ad0: 2220 6e61 6d65 3d22 7369 7a65 2220 7479  " name="size" ty
+00005ae0: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+00005af0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00005b00: 6f6e 2076 616c 7565 3d22 3378 3a30 2c30  on value="3x:0,0
+00005b10: 2c30 2c30 2c30 2c30 2220 6e61 6d65 3d22  ,0,0,0,0" name="
+00005b20: 7369 7a65 5f6d 6170 5f75 6e69 745f 7363  size_map_unit_sc
+00005b30: 616c 6522 2074 7970 653d 2251 5374 7269  ale" type="QStri
+00005b40: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+00005b50: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+00005b60: 2252 656e 6465 724d 6574 6572 7349 6e4d  "RenderMetersInM
+00005b70: 6170 556e 6974 7322 206e 616d 653d 2273  apUnits" name="s
+00005b80: 697a 655f 756e 6974 2220 7479 7065 3d22  ize_unit" type="
+00005b90: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+00005ba0: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
+00005bb0: 616c 7565 3d22 3122 206e 616d 653d 2276  alue="1" name="v
+00005bc0: 6572 7469 6361 6c5f 616e 6368 6f72 5f70  ertical_anchor_p
+00005bd0: 6f69 6e74 2220 7479 7065 3d22 5153 7472  oint" type="QStr
+00005be0: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+00005bf0: 203c 2f4f 7074 696f 6e3e 0a20 2020 2020   </Option>.     
+00005c00: 2020 2020 203c 6461 7461 5f64 6566 696e       <data_defin
+00005c10: 6564 5f70 726f 7065 7274 6965 733e 0a20  ed_properties>. 
+00005c20: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00005c30: 6f6e 2074 7970 653d 224d 6170 223e 0a20  on type="Map">. 
+00005c40: 2020 2020 2020 2020 2020 2020 203c 4f70               <Op
+00005c50: 7469 6f6e 2076 616c 7565 3d22 2220 6e61  tion value="" na
+00005c60: 6d65 3d22 6e61 6d65 2220 7479 7065 3d22  me="name" type="
+00005c70: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+00005c80: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00005c90: 206e 616d 653d 2270 726f 7065 7274 6965   name="propertie
+00005ca0: 7322 2074 7970 653d 224d 6170 223e 0a20  s" type="Map">. 
+00005cb0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00005cc0: 4f70 7469 6f6e 206e 616d 653d 2273 697a  Option name="siz
+00005cd0: 6522 2074 7970 653d 224d 6170 223e 0a20  e" type="Map">. 
+00005ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005cf0: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+00005d00: 7472 7565 2220 6e61 6d65 3d22 6163 7469  true" name="acti
+00005d10: 7665 2220 7479 7065 3d22 626f 6f6c 222f  ve" type="bool"/
+00005d20: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00005d30: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
+00005d40: 653d 2226 7175 6f74 3b6c 616e 655f 7769  e="&quot;lane_wi
+00005d50: 6474 6826 7175 6f74 3b22 206e 616d 653d  dth&quot;" name=
+00005d60: 2265 7870 7265 7373 696f 6e22 2074 7970  "expression" typ
+00005d70: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00005d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d90: 3c4f 7074 696f 6e20 7661 6c75 653d 2233  <Option value="3
+00005da0: 2220 6e61 6d65 3d22 7479 7065 2220 7479  " name="type" ty
+00005db0: 7065 3d22 696e 7422 2f3e 0a20 2020 2020  pe="int"/>.     
+00005dc0: 2020 2020 2020 2020 2020 203c 2f4f 7074             </Opt
+00005dd0: 696f 6e3e 0a20 2020 2020 2020 2020 2020  ion>.           
+00005de0: 2020 203c 2f4f 7074 696f 6e3e 0a20 2020     </Option>.   
+00005df0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00005e00: 6f6e 2076 616c 7565 3d22 636f 6c6c 6563  on value="collec
+00005e10: 7469 6f6e 2220 6e61 6d65 3d22 7479 7065  tion" name="type
+00005e20: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00005e30: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
+00005e40: 2f4f 7074 696f 6e3e 0a20 2020 2020 2020  /Option>.       
+00005e50: 2020 203c 2f64 6174 615f 6465 6669 6e65     </data_define
+00005e60: 645f 7072 6f70 6572 7469 6573 3e0a 2020  d_properties>.  
+00005e70: 2020 2020 2020 3c2f 6c61 7965 723e 0a20        </layer>. 
+00005e80: 2020 2020 203c 2f73 796d 626f 6c3e 0a20       </symbol>. 
+00005e90: 2020 203c 2f73 796d 626f 6c73 3e0a 2020     </symbols>.  
+00005ea0: 3c2f 7265 6e64 6572 6572 2d76 323e 0a20  </renderer-v2>. 
+00005eb0: 203c 6375 7374 6f6d 7072 6f70 6572 7469   <customproperti
+00005ec0: 6573 3e0a 2020 2020 3c4f 7074 696f 6e20  es>.    <Option 
+00005ed0: 7479 7065 3d22 4d61 7022 3e0a 2020 2020  type="Map">.    
+00005ee0: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
+00005ef0: 6475 616c 7669 6577 2f70 7265 7669 6577  dualview/preview
+00005f00: 4578 7072 6573 7369 6f6e 7322 2074 7970  Expressions" typ
+00005f10: 653d 224c 6973 7422 3e0a 2020 2020 2020  e="List">.      
+00005f20: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+00005f30: 2226 7175 6f74 3b74 7970 6526 7175 6f74  "&quot;type&quot
+00005f40: 3b22 2074 7970 653d 2251 5374 7269 6e67  ;" type="QString
+00005f50: 222f 3e0a 2020 2020 2020 3c2f 4f70 7469  "/>.      </Opti
+00005f60: 6f6e 3e0a 2020 2020 2020 3c4f 7074 696f  on>.      <Optio
+00005f70: 6e20 7661 6c75 653d 2230 2220 6e61 6d65  n value="0" name
+00005f80: 3d22 656d 6265 6464 6564 5769 6467 6574  ="embeddedWidget
+00005f90: 732f 636f 756e 7422 2074 7970 653d 2269  s/count" type="i
+00005fa0: 6e74 222f 3e0a 2020 2020 2020 3c4f 7074  nt"/>.      <Opt
+00005fb0: 696f 6e20 6e61 6d65 3d22 7661 7269 6162  ion name="variab
+00005fc0: 6c65 4e61 6d65 7322 2f3e 0a20 2020 2020  leNames"/>.     
+00005fd0: 203c 4f70 7469 6f6e 206e 616d 653d 2276   <Option name="v
+00005fe0: 6172 6961 626c 6556 616c 7565 7322 2f3e  ariableValues"/>
+00005ff0: 0a20 2020 203c 2f4f 7074 696f 6e3e 0a20  .    </Option>. 
+00006000: 203c 2f63 7573 746f 6d70 726f 7065 7274   </custompropert
+00006010: 6965 733e 0a20 203c 626c 656e 644d 6f64  ies>.  <blendMod
+00006020: 653e 303c 2f62 6c65 6e64 4d6f 6465 3e0a  e>0</blendMode>.
+00006030: 2020 3c66 6561 7475 7265 426c 656e 644d    <featureBlendM
+00006040: 6f64 653e 303c 2f66 6561 7475 7265 426c  ode>0</featureBl
+00006050: 656e 644d 6f64 653e 0a20 203c 6c61 7965  endMode>.  <laye
+00006060: 724f 7061 6369 7479 3e31 3c2f 6c61 7965  rOpacity>1</laye
+00006070: 724f 7061 6369 7479 3e0a 2020 3c53 696e  rOpacity>.  <Sin
+00006080: 676c 6543 6174 6567 6f72 7944 6961 6772  gleCategoryDiagr
+00006090: 616d 5265 6e64 6572 6572 2061 7474 7269  amRenderer attri
+000060a0: 6275 7465 4c65 6765 6e64 3d22 3122 2064  buteLegend="1" d
+000060b0: 6961 6772 616d 5479 7065 3d22 4869 7374  iagramType="Hist
+000060c0: 6f67 7261 6d22 3e0a 2020 2020 3c44 6961  ogram">.    <Dia
+000060d0: 6772 616d 4361 7465 676f 7279 2062 6163  gramCategory bac
+000060e0: 6b67 726f 756e 6441 6c70 6861 3d22 3235  kgroundAlpha="25
+000060f0: 3522 206c 6162 656c 506c 6163 656d 656e  5" labelPlacemen
+00006100: 744d 6574 686f 643d 2258 4865 6967 6874  tMethod="XHeight
+00006110: 2220 7369 7a65 5363 616c 653d 2233 783a  " sizeScale="3x:
+00006120: 302c 302c 302c 302c 302c 3022 206c 696e  0,0,0,0,0,0" lin
+00006130: 6553 697a 6553 6361 6c65 3d22 3378 3a30  eSizeScale="3x:0
+00006140: 2c30 2c30 2c30 2c30 2c30 2220 7065 6e43  ,0,0,0,0,0" penC
+00006150: 6f6c 6f72 3d22 2330 3030 3030 3022 206d  olor="#000000" m
+00006160: 696e 5363 616c 6544 656e 6f6d 696e 6174  inScaleDenominat
+00006170: 6f72 3d22 3022 2073 6361 6c65 4261 7365  or="0" scaleBase
+00006180: 6456 6973 6962 696c 6974 793d 2230 2220  dVisibility="0" 
+00006190: 6f70 6163 6974 793d 2231 2220 6261 7257  opacity="1" barW
+000061a0: 6964 7468 3d22 3522 2064 6972 6563 7469  idth="5" directi
+000061b0: 6f6e 3d22 3022 2070 656e 416c 7068 613d  on="0" penAlpha=
+000061c0: 2232 3535 2220 7769 6474 683d 2231 3522  "255" width="15"
+000061d0: 2073 6361 6c65 4465 7065 6e64 656e 6379   scaleDependency
+000061e0: 3d22 4172 6561 2220 7369 7a65 5479 7065  ="Area" sizeType
+000061f0: 3d22 4d4d 2220 7370 6163 696e 6755 6e69  ="MM" spacingUni
+00006200: 743d 224d 4d22 2073 7061 6369 6e67 556e  t="MM" spacingUn
+00006210: 6974 5363 616c 653d 2233 783a 302c 302c  itScale="3x:0,0,
+00006220: 302c 302c 302c 3022 2073 686f 7741 7869  0,0,0,0" showAxi
+00006230: 733d 2231 2220 6865 6967 6874 3d22 3135  s="1" height="15
+00006240: 2220 6469 6167 7261 6d4f 7269 656e 7461  " diagramOrienta
+00006250: 7469 6f6e 3d22 5570 2220 7065 6e57 6964  tion="Up" penWid
+00006260: 7468 3d22 3022 206c 696e 6553 697a 6554  th="0" lineSizeT
+00006270: 7970 653d 224d 4d22 206d 696e 696d 756d  ype="MM" minimum
+00006280: 5369 7a65 3d22 3022 2065 6e61 626c 6564  Size="0" enabled
+00006290: 3d22 3022 2062 6163 6b67 726f 756e 6443  ="0" backgroundC
+000062a0: 6f6c 6f72 3d22 2366 6666 6666 6622 2073  olor="#ffffff" s
+000062b0: 7061 6369 6e67 3d22 3522 206d 6178 5363  pacing="5" maxSc
+000062c0: 616c 6544 656e 6f6d 696e 6174 6f72 3d22  aleDenominator="
+000062d0: 3165 2b30 3822 2072 6f74 6174 696f 6e4f  1e+08" rotationO
+000062e0: 6666 7365 743d 2232 3730 223e 0a20 2020  ffset="270">.   
+000062f0: 2020 203c 666f 6e74 5072 6f70 6572 7469     <fontProperti
+00006300: 6573 2064 6573 6372 6970 7469 6f6e 3d22  es description="
+00006310: 4e6f 746f 2053 616e 732c 3130 2c2d 312c  Noto Sans,10,-1,
+00006320: 302c 3530 2c30 2c30 2c30 2c30 2c30 2220  0,50,0,0,0,0,0" 
+00006330: 7374 796c 653d 2222 2073 7472 696b 6574  style="" striket
+00006340: 6872 6f75 6768 3d22 3022 2075 6e64 6572  hrough="0" under
+00006350: 6c69 6e65 3d22 3022 2069 7461 6c69 633d  line="0" italic=
+00006360: 2230 2220 626f 6c64 3d22 3022 2f3e 0a20  "0" bold="0"/>. 
+00006370: 2020 2020 203c 6174 7472 6962 7574 6520       <attribute 
+00006380: 6669 656c 643d 2222 2063 6f6c 6f72 3d22  field="" color="
+00006390: 2330 3030 3030 3022 206c 6162 656c 3d22  #000000" label="
+000063a0: 2220 636f 6c6f 724f 7061 6369 7479 3d22  " colorOpacity="
+000063b0: 3122 2f3e 0a20 2020 2020 203c 6178 6973  1"/>.      <axis
+000063c0: 5379 6d62 6f6c 3e0a 2020 2020 2020 2020  Symbol>.        
+000063d0: 3c73 796d 626f 6c20 6672 616d 655f 7261  <symbol frame_ra
+000063e0: 7465 3d22 3130 2220 6973 5f61 6e69 6d61  te="10" is_anima
+000063f0: 7465 643d 2230 2220 6e61 6d65 3d22 2220  ted="0" name="" 
+00006400: 616c 7068 613d 2231 2220 666f 7263 655f  alpha="1" force_
+00006410: 7268 723d 2230 2220 636c 6970 5f74 6f5f  rhr="0" clip_to_
+00006420: 6578 7465 6e74 3d22 3122 2074 7970 653d  extent="1" type=
+00006430: 226c 696e 6522 3e0a 2020 2020 2020 2020  "line">.        
+00006440: 2020 3c64 6174 615f 6465 6669 6e65 645f    <data_defined_
+00006450: 7072 6f70 6572 7469 6573 3e0a 2020 2020  properties>.    
+00006460: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00006470: 7479 7065 3d22 4d61 7022 3e0a 2020 2020  type="Map">.    
+00006480: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00006490: 6e20 7661 6c75 653d 2222 206e 616d 653d  n value="" name=
+000064a0: 226e 616d 6522 2074 7970 653d 2251 5374  "name" type="QSt
+000064b0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+000064c0: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
+000064d0: 6d65 3d22 7072 6f70 6572 7469 6573 222f  me="properties"/
+000064e0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000064f0: 3c4f 7074 696f 6e20 7661 6c75 653d 2263  <Option value="c
+00006500: 6f6c 6c65 6374 696f 6e22 206e 616d 653d  ollection" name=
+00006510: 2274 7970 6522 2074 7970 653d 2251 5374  "type" type="QSt
+00006520: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+00006530: 2020 2020 3c2f 4f70 7469 6f6e 3e0a 2020      </Option>.  
+00006540: 2020 2020 2020 2020 3c2f 6461 7461 5f64          </data_d
+00006550: 6566 696e 6564 5f70 726f 7065 7274 6965  efined_propertie
+00006560: 733e 0a20 2020 2020 2020 2020 203c 6c61  s>.          <la
+00006570: 7965 7220 656e 6162 6c65 643d 2231 2220  yer enabled="1" 
+00006580: 636c 6173 733d 2253 696d 706c 654c 696e  class="SimpleLin
+00006590: 6522 206c 6f63 6b65 643d 2230 2220 7061  e" locked="0" pa
+000065a0: 7373 3d22 3022 3e0a 2020 2020 2020 2020  ss="0">.        
+000065b0: 2020 2020 3c4f 7074 696f 6e20 7479 7065      <Option type
+000065c0: 3d22 4d61 7022 3e0a 2020 2020 2020 2020  ="Map">.        
+000065d0: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
+000065e0: 6c75 653d 2230 2220 6e61 6d65 3d22 616c  lue="0" name="al
+000065f0: 6967 6e5f 6461 7368 5f70 6174 7465 726e  ign_dash_pattern
+00006600: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00006610: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+00006620: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+00006630: 7371 7561 7265 2220 6e61 6d65 3d22 6361  square" name="ca
+00006640: 7073 7479 6c65 2220 7479 7065 3d22 5153  pstyle" type="QS
+00006650: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+00006660: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
+00006670: 616c 7565 3d22 353b 3222 206e 616d 653d  alue="5;2" name=
+00006680: 2263 7573 746f 6d64 6173 6822 2074 7970  "customdash" typ
+00006690: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+000066a0: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+000066b0: 696f 6e20 7661 6c75 653d 2233 783a 302c  ion value="3x:0,
+000066c0: 302c 302c 302c 302c 3022 206e 616d 653d  0,0,0,0,0" name=
+000066d0: 2263 7573 746f 6d64 6173 685f 6d61 705f  "customdash_map_
+000066e0: 756e 6974 5f73 6361 6c65 2220 7479 7065  unit_scale" type
+000066f0: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+00006700: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00006710: 6f6e 2076 616c 7565 3d22 4d4d 2220 6e61  on value="MM" na
+00006720: 6d65 3d22 6375 7374 6f6d 6461 7368 5f75  me="customdash_u
+00006730: 6e69 7422 2074 7970 653d 2251 5374 7269  nit" type="QStri
+00006740: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+00006750: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
+00006760: 653d 2230 2220 6e61 6d65 3d22 6461 7368  e="0" name="dash
+00006770: 5f70 6174 7465 726e 5f6f 6666 7365 7422  _pattern_offset"
+00006780: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+00006790: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000067a0: 3c4f 7074 696f 6e20 7661 6c75 653d 2233  <Option value="3
+000067b0: 783a 302c 302c 302c 302c 302c 3022 206e  x:0,0,0,0,0,0" n
+000067c0: 616d 653d 2264 6173 685f 7061 7474 6572  ame="dash_patter
+000067d0: 6e5f 6f66 6673 6574 5f6d 6170 5f75 6e69  n_offset_map_uni
+000067e0: 745f 7363 616c 6522 2074 7970 653d 2251  t_scale" type="Q
+000067f0: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+00006800: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00006810: 7661 6c75 653d 224d 4d22 206e 616d 653d  value="MM" name=
+00006820: 2264 6173 685f 7061 7474 6572 6e5f 6f66  "dash_pattern_of
+00006830: 6673 6574 5f75 6e69 7422 2074 7970 653d  fset_unit" type=
+00006840: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00006850: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00006860: 6e20 7661 6c75 653d 2230 2220 6e61 6d65  n value="0" name
+00006870: 3d22 6472 6177 5f69 6e73 6964 655f 706f  ="draw_inside_po
+00006880: 6c79 676f 6e22 2074 7970 653d 2251 5374  lygon" type="QSt
+00006890: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+000068a0: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
+000068b0: 6c75 653d 2262 6576 656c 2220 6e61 6d65  lue="bevel" name
+000068c0: 3d22 6a6f 696e 7374 796c 6522 2074 7970  ="joinstyle" typ
+000068d0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+000068e0: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+000068f0: 696f 6e20 7661 6c75 653d 2233 352c 3335  ion value="35,35
+00006900: 2c33 352c 3235 3522 206e 616d 653d 226c  ,35,255" name="l
+00006910: 696e 655f 636f 6c6f 7222 2074 7970 653d  ine_color" type=
+00006920: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00006930: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00006940: 6e20 7661 6c75 653d 2273 6f6c 6964 2220  n value="solid" 
+00006950: 6e61 6d65 3d22 6c69 6e65 5f73 7479 6c65  name="line_style
+00006960: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00006970: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+00006980: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+00006990: 302e 3236 2220 6e61 6d65 3d22 6c69 6e65  0.26" name="line
+000069a0: 5f77 6964 7468 2220 7479 7065 3d22 5153  _width" type="QS
+000069b0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+000069c0: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
+000069d0: 616c 7565 3d22 4d4d 2220 6e61 6d65 3d22  alue="MM" name="
+000069e0: 6c69 6e65 5f77 6964 7468 5f75 6e69 7422  line_width_unit"
+000069f0: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+00006a00: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00006a10: 3c4f 7074 696f 6e20 7661 6c75 653d 2230  <Option value="0
+00006a20: 2220 6e61 6d65 3d22 6f66 6673 6574 2220  " name="offset" 
+00006a30: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00006a40: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+00006a50: 4f70 7469 6f6e 2076 616c 7565 3d22 3378  Option value="3x
+00006a60: 3a30 2c30 2c30 2c30 2c30 2c30 2220 6e61  :0,0,0,0,0,0" na
+00006a70: 6d65 3d22 6f66 6673 6574 5f6d 6170 5f75  me="offset_map_u
+00006a80: 6e69 745f 7363 616c 6522 2074 7970 653d  nit_scale" type=
+00006a90: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00006aa0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00006ab0: 6e20 7661 6c75 653d 224d 4d22 206e 616d  n value="MM" nam
+00006ac0: 653d 226f 6666 7365 745f 756e 6974 2220  e="offset_unit" 
+00006ad0: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00006ae0: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+00006af0: 4f70 7469 6f6e 2076 616c 7565 3d22 3022  Option value="0"
+00006b00: 206e 616d 653d 2272 696e 675f 6669 6c74   name="ring_filt
+00006b10: 6572 2220 7479 7065 3d22 5153 7472 696e  er" type="QStrin
+00006b20: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00006b30: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
+00006b40: 3d22 3022 206e 616d 653d 2274 7269 6d5f  ="0" name="trim_
+00006b50: 6469 7374 616e 6365 5f65 6e64 2220 7479  distance_end" ty
+00006b60: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+00006b70: 2020 2020 2020 2020 2020 2020 203c 4f70               <Op
+00006b80: 7469 6f6e 2076 616c 7565 3d22 3378 3a30  tion value="3x:0
+00006b90: 2c30 2c30 2c30 2c30 2c30 2220 6e61 6d65  ,0,0,0,0,0" name
+00006ba0: 3d22 7472 696d 5f64 6973 7461 6e63 655f  ="trim_distance_
+00006bb0: 656e 645f 6d61 705f 756e 6974 5f73 6361  end_map_unit_sca
+00006bc0: 6c65 2220 7479 7065 3d22 5153 7472 696e  le" type="QStrin
+00006bd0: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00006be0: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
+00006bf0: 3d22 4d4d 2220 6e61 6d65 3d22 7472 696d  ="MM" name="trim
+00006c00: 5f64 6973 7461 6e63 655f 656e 645f 756e  _distance_end_un
+00006c10: 6974 2220 7479 7065 3d22 5153 7472 696e  it" type="QStrin
+00006c20: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00006c30: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
+00006c40: 3d22 3022 206e 616d 653d 2274 7269 6d5f  ="0" name="trim_
+00006c50: 6469 7374 616e 6365 5f73 7461 7274 2220  distance_start" 
+00006c60: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00006c70: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+00006c80: 4f70 7469 6f6e 2076 616c 7565 3d22 3378  Option value="3x
+00006c90: 3a30 2c30 2c30 2c30 2c30 2c30 2220 6e61  :0,0,0,0,0,0" na
+00006ca0: 6d65 3d22 7472 696d 5f64 6973 7461 6e63  me="trim_distanc
+00006cb0: 655f 7374 6172 745f 6d61 705f 756e 6974  e_start_map_unit
+00006cc0: 5f73 6361 6c65 2220 7479 7065 3d22 5153  _scale" type="QS
+00006cd0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+00006ce0: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
+00006cf0: 616c 7565 3d22 4d4d 2220 6e61 6d65 3d22  alue="MM" name="
+00006d00: 7472 696d 5f64 6973 7461 6e63 655f 7374  trim_distance_st
+00006d10: 6172 745f 756e 6974 2220 7479 7065 3d22  art_unit" type="
+00006d20: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+00006d30: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00006d40: 2076 616c 7565 3d22 3022 206e 616d 653d   value="0" name=
+00006d50: 2274 7765 616b 5f64 6173 685f 7061 7474  "tweak_dash_patt
+00006d60: 6572 6e5f 6f6e 5f63 6f72 6e65 7273 2220  ern_on_corners" 
+00006d70: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00006d80: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+00006d90: 4f70 7469 6f6e 2076 616c 7565 3d22 3022  Option value="0"
+00006da0: 206e 616d 653d 2275 7365 5f63 7573 746f   name="use_custo
+00006db0: 6d5f 6461 7368 2220 7479 7065 3d22 5153  m_dash" type="QS
+00006dc0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+00006dd0: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
+00006de0: 616c 7565 3d22 3378 3a30 2c30 2c30 2c30  alue="3x:0,0,0,0
+00006df0: 2c30 2c30 2220 6e61 6d65 3d22 7769 6474  ,0,0" name="widt
+00006e00: 685f 6d61 705f 756e 6974 5f73 6361 6c65  h_map_unit_scale
+00006e10: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00006e20: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
+00006e30: 2f4f 7074 696f 6e3e 0a20 2020 2020 2020  /Option>.       
+00006e40: 2020 2020 203c 6461 7461 5f64 6566 696e       <data_defin
+00006e50: 6564 5f70 726f 7065 7274 6965 733e 0a20  ed_properties>. 
+00006e60: 2020 2020 2020 2020 2020 2020 203c 4f70               <Op
+00006e70: 7469 6f6e 2074 7970 653d 224d 6170 223e  tion type="Map">
+00006e80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006e90: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+00006ea0: 2220 6e61 6d65 3d22 6e61 6d65 2220 7479  " name="name" ty
+00006eb0: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+00006ec0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00006ed0: 4f70 7469 6f6e 206e 616d 653d 2270 726f  Option name="pro
+00006ee0: 7065 7274 6965 7322 2f3e 0a20 2020 2020  perties"/>.     
+00006ef0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00006f00: 6f6e 2076 616c 7565 3d22 636f 6c6c 6563  on value="collec
+00006f10: 7469 6f6e 2220 6e61 6d65 3d22 7479 7065  tion" name="type
+00006f20: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00006f30: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+00006f40: 203c 2f4f 7074 696f 6e3e 0a20 2020 2020   </Option>.     
+00006f50: 2020 2020 2020 203c 2f64 6174 615f 6465         </data_de
+00006f60: 6669 6e65 645f 7072 6f70 6572 7469 6573  fined_properties
+00006f70: 3e0a 2020 2020 2020 2020 2020 3c2f 6c61  >.          </la
+00006f80: 7965 723e 0a20 2020 2020 2020 203c 2f73  yer>.        </s
+00006f90: 796d 626f 6c3e 0a20 2020 2020 203c 2f61  ymbol>.      </a
+00006fa0: 7869 7353 796d 626f 6c3e 0a20 2020 203c  xisSymbol>.    <
+00006fb0: 2f44 6961 6772 616d 4361 7465 676f 7279  /DiagramCategory
+00006fc0: 3e0a 2020 3c2f 5369 6e67 6c65 4361 7465  >.  </SingleCate
+00006fd0: 676f 7279 4469 6167 7261 6d52 656e 6465  goryDiagramRende
+00006fe0: 7265 723e 0a20 203c 4469 6167 7261 6d4c  rer>.  <DiagramL
+00006ff0: 6179 6572 5365 7474 696e 6773 2064 6973  ayerSettings dis
+00007000: 743d 2230 2220 7368 6f77 416c 6c3d 2231  t="0" showAll="1
+00007010: 2220 6c69 6e65 506c 6163 656d 656e 7446  " linePlacementF
+00007020: 6c61 6773 3d22 3138 2220 6f62 7374 6163  lags="18" obstac
+00007030: 6c65 3d22 3022 2070 7269 6f72 6974 793d  le="0" priority=
+00007040: 2230 2220 706c 6163 656d 656e 743d 2230  "0" placement="0
+00007050: 2220 7a49 6e64 6578 3d22 3022 3e0a 2020  " zIndex="0">.  
+00007060: 2020 3c70 726f 7065 7274 6965 733e 0a20    <properties>. 
+00007070: 2020 2020 203c 4f70 7469 6f6e 2074 7970       <Option typ
+00007080: 653d 224d 6170 223e 0a20 2020 2020 2020  e="Map">.       
+00007090: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+000070a0: 2220 6e61 6d65 3d22 6e61 6d65 2220 7479  " name="name" ty
+000070b0: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+000070c0: 2020 2020 2020 203c 4f70 7469 6f6e 206e         <Option n
+000070d0: 616d 653d 2270 726f 7065 7274 6965 7322  ame="properties"
+000070e0: 2f3e 0a20 2020 2020 2020 203c 4f70 7469  />.        <Opti
+000070f0: 6f6e 2076 616c 7565 3d22 636f 6c6c 6563  on value="collec
+00007100: 7469 6f6e 2220 6e61 6d65 3d22 7479 7065  tion" name="type
+00007110: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00007120: 2f3e 0a20 2020 2020 203c 2f4f 7074 696f  />.      </Optio
+00007130: 6e3e 0a20 2020 203c 2f70 726f 7065 7274  n>.    </propert
+00007140: 6965 733e 0a20 203c 2f44 6961 6772 616d  ies>.  </Diagram
+00007150: 4c61 7965 7253 6574 7469 6e67 733e 0a20  LayerSettings>. 
+00007160: 203c 6765 6f6d 6574 7279 4f70 7469 6f6e   <geometryOption
+00007170: 7320 6765 6f6d 6574 7279 5072 6563 6973  s geometryPrecis
+00007180: 696f 6e3d 2230 2220 7265 6d6f 7665 4475  ion="0" removeDu
+00007190: 706c 6963 6174 654e 6f64 6573 3d22 3022  plicateNodes="0"
+000071a0: 3e0a 2020 2020 3c61 6374 6976 6543 6865  >.    <activeChe
+000071b0: 636b 732f 3e0a 2020 2020 3c63 6865 636b  cks/>.    <check
+000071c0: 436f 6e66 6967 7572 6174 696f 6e2f 3e0a  Configuration/>.
+000071d0: 2020 3c2f 6765 6f6d 6574 7279 4f70 7469    </geometryOpti
+000071e0: 6f6e 733e 0a20 203c 6c65 6765 6e64 2073  ons>.  <legend s
+000071f0: 686f 774c 6162 656c 4c65 6765 6e64 3d22  howLabelLegend="
+00007200: 3022 2074 7970 653d 2264 6566 6175 6c74  0" type="default
+00007210: 2d76 6563 746f 7222 2f3e 0a20 203c 7265  -vector"/>.  <re
+00007220: 6665 7265 6e63 6564 4c61 7965 7273 2f3e  ferencedLayers/>
+00007230: 0a20 203c 6669 656c 6443 6f6e 6669 6775  .  <fieldConfigu
+00007240: 7261 7469 6f6e 3e0a 2020 2020 3c66 6965  ration>.    <fie
+00007250: 6c64 206e 616d 653d 2274 7970 6522 2063  ld name="type" c
+00007260: 6f6e 6669 6775 7261 7469 6f6e 466c 6167  onfigurationFlag
+00007270: 733d 224e 6f6e 6522 3e0a 2020 2020 2020  s="None">.      
+00007280: 3c65 6469 7457 6964 6765 7420 7479 7065  <editWidget type
+00007290: 3d22 5465 7874 4564 6974 223e 0a20 2020  ="TextEdit">.   
+000072a0: 2020 2020 203c 636f 6e66 6967 3e0a 2020       <config>.  
+000072b0: 2020 2020 2020 2020 3c4f 7074 696f 6e2f          <Option/
+000072c0: 3e0a 2020 2020 2020 2020 3c2f 636f 6e66  >.        </conf
+000072d0: 6967 3e0a 2020 2020 2020 3c2f 6564 6974  ig>.      </edit
+000072e0: 5769 6467 6574 3e0a 2020 2020 3c2f 6669  Widget>.    </fi
+000072f0: 656c 643e 0a20 2020 203c 6669 656c 6420  eld>.    <field 
+00007300: 6e61 6d65 3d22 6f73 6d5f 6964 2220 636f  name="osm_id" co
+00007310: 6e66 6967 7572 6174 696f 6e46 6c61 6773  nfigurationFlags
+00007320: 3d22 4e6f 6e65 223e 0a20 2020 2020 203c  ="None">.      <
+00007330: 6564 6974 5769 6467 6574 2074 7970 653d  editWidget type=
+00007340: 2254 6578 7445 6469 7422 3e0a 2020 2020  "TextEdit">.    
+00007350: 2020 2020 3c63 6f6e 6669 673e 0a20 2020      <config>.   
+00007360: 2020 2020 2020 203c 4f70 7469 6f6e 2f3e         <Option/>
+00007370: 0a20 2020 2020 2020 203c 2f63 6f6e 6669  .        </confi
+00007380: 673e 0a20 2020 2020 203c 2f65 6469 7457  g>.      </editW
+00007390: 6964 6765 743e 0a20 2020 203c 2f66 6965  idget>.    </fie
+000073a0: 6c64 3e0a 2020 2020 3c66 6965 6c64 206e  ld>.    <field n
+000073b0: 616d 653d 226f 7269 656e 7461 7469 6f6e  ame="orientation
+000073c0: 2220 636f 6e66 6967 7572 6174 696f 6e46  " configurationF
+000073d0: 6c61 6773 3d22 4e6f 6e65 223e 0a20 2020  lags="None">.   
+000073e0: 2020 203c 6564 6974 5769 6467 6574 2074     <editWidget t
+000073f0: 7970 653d 2254 6578 7445 6469 7422 3e0a  ype="TextEdit">.
+00007400: 2020 2020 2020 2020 3c63 6f6e 6669 673e          <config>
+00007410: 0a20 2020 2020 2020 2020 203c 4f70 7469  .          <Opti
+00007420: 6f6e 2f3e 0a20 2020 2020 2020 203c 2f63  on/>.        </c
+00007430: 6f6e 6669 673e 0a20 2020 2020 203c 2f65  onfig>.      </e
+00007440: 6469 7457 6964 6765 743e 0a20 2020 203c  ditWidget>.    <
+00007450: 2f66 6965 6c64 3e0a 2020 2020 3c66 6965  /field>.    <fie
+00007460: 6c64 206e 616d 653d 226f 7269 656e 7461  ld name="orienta
+00007470: 7469 6f6e 5f63 6f6e 6669 6465 6e63 6522  tion_confidence"
+00007480: 2063 6f6e 6669 6775 7261 7469 6f6e 466c   configurationFl
+00007490: 6167 733d 224e 6f6e 6522 3e0a 2020 2020  ags="None">.    
+000074a0: 2020 3c65 6469 7457 6964 6765 7420 7479    <editWidget ty
+000074b0: 7065 3d22 5465 7874 4564 6974 223e 0a20  pe="TextEdit">. 
+000074c0: 2020 2020 2020 203c 636f 6e66 6967 3e0a         <config>.
+000074d0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+000074e0: 6e2f 3e0a 2020 2020 2020 2020 3c2f 636f  n/>.        </co
+000074f0: 6e66 6967 3e0a 2020 2020 2020 3c2f 6564  nfig>.      </ed
+00007500: 6974 5769 6467 6574 3e0a 2020 2020 3c2f  itWidget>.    </
+00007510: 6669 656c 643e 0a20 2020 203c 6669 656c  field>.    <fiel
+00007520: 6420 6e61 6d65 3d22 6c61 6e65 5f77 6964  d name="lane_wid
+00007530: 7468 2220 636f 6e66 6967 7572 6174 696f  th" configuratio
+00007540: 6e46 6c61 6773 3d22 4e6f 6e65 223e 0a20  nFlags="None">. 
+00007550: 2020 2020 203c 6564 6974 5769 6467 6574       <editWidget
+00007560: 2074 7970 653d 2254 6578 7445 6469 7422   type="TextEdit"
+00007570: 3e0a 2020 2020 2020 2020 3c63 6f6e 6669  >.        <confi
+00007580: 673e 0a20 2020 2020 2020 2020 203c 4f70  g>.          <Op
+00007590: 7469 6f6e 2f3e 0a20 2020 2020 2020 203c  tion/>.        <
+000075a0: 2f63 6f6e 6669 673e 0a20 2020 2020 203c  /config>.      <
+000075b0: 2f65 6469 7457 6964 6765 743e 0a20 2020  /editWidget>.   
+000075c0: 203c 2f66 6965 6c64 3e0a 2020 2020 3c66   </field>.    <f
+000075d0: 6965 6c64 206e 616d 653d 226c 616e 655f  ield name="lane_
+000075e0: 6f72 6965 6e74 6174 696f 6e22 2063 6f6e  orientation" con
+000075f0: 6669 6775 7261 7469 6f6e 466c 6167 733d  figurationFlags=
+00007600: 224e 6f6e 6522 3e0a 2020 2020 2020 3c65  "None">.      <e
+00007610: 6469 7457 6964 6765 7420 7479 7065 3d22  ditWidget type="
+00007620: 5465 7874 4564 6974 223e 0a20 2020 2020  TextEdit">.     
+00007630: 2020 203c 636f 6e66 6967 3e0a 2020 2020     <config>.    
+00007640: 2020 2020 2020 3c4f 7074 696f 6e2f 3e0a        <Option/>.
+00007650: 2020 2020 2020 2020 3c2f 636f 6e66 6967          </config
+00007660: 3e0a 2020 2020 2020 3c2f 6564 6974 5769  >.      </editWi
+00007670: 6467 6574 3e0a 2020 2020 3c2f 6669 656c  dget>.    </fiel
+00007680: 643e 0a20 203c 2f66 6965 6c64 436f 6e66  d>.  </fieldConf
+00007690: 6967 7572 6174 696f 6e3e 0a20 203c 616c  iguration>.  <al
+000076a0: 6961 7365 733e 0a20 2020 203c 616c 6961  iases>.    <alia
+000076b0: 7320 6669 656c 643d 2274 7970 6522 206e  s field="type" n
+000076c0: 616d 653d 2222 2069 6e64 6578 3d22 3022  ame="" index="0"
+000076d0: 2f3e 0a20 2020 203c 616c 6961 7320 6669  />.    <alias fi
+000076e0: 656c 643d 226f 736d 5f69 6422 206e 616d  eld="osm_id" nam
+000076f0: 653d 2222 2069 6e64 6578 3d22 3122 2f3e  e="" index="1"/>
+00007700: 0a20 2020 203c 616c 6961 7320 6669 656c  .    <alias fiel
+00007710: 643d 226f 7269 656e 7461 7469 6f6e 2220  d="orientation" 
+00007720: 6e61 6d65 3d22 2220 696e 6465 783d 2232  name="" index="2
+00007730: 222f 3e0a 2020 2020 3c61 6c69 6173 2066  "/>.    <alias f
+00007740: 6965 6c64 3d22 6f72 6965 6e74 6174 696f  ield="orientatio
+00007750: 6e5f 636f 6e66 6964 656e 6365 2220 6e61  n_confidence" na
+00007760: 6d65 3d22 2220 696e 6465 783d 2233 222f  me="" index="3"/
+00007770: 3e0a 2020 2020 3c61 6c69 6173 2066 6965  >.    <alias fie
+00007780: 6c64 3d22 6c61 6e65 5f77 6964 7468 2220  ld="lane_width" 
+00007790: 6e61 6d65 3d22 2220 696e 6465 783d 2234  name="" index="4
+000077a0: 222f 3e0a 2020 2020 3c61 6c69 6173 2066  "/>.    <alias f
+000077b0: 6965 6c64 3d22 6c61 6e65 5f6f 7269 656e  ield="lane_orien
+000077c0: 7461 7469 6f6e 2220 6e61 6d65 3d22 2220  tation" name="" 
+000077d0: 696e 6465 783d 2235 222f 3e0a 2020 3c2f  index="5"/>.  </
+000077e0: 616c 6961 7365 733e 0a20 203c 6465 6661  aliases>.  <defa
+000077f0: 756c 7473 3e0a 2020 2020 3c64 6566 6175  ults>.    <defau
+00007800: 6c74 2066 6965 6c64 3d22 7479 7065 2220  lt field="type" 
+00007810: 6170 706c 794f 6e55 7064 6174 653d 2230  applyOnUpdate="0
+00007820: 2220 6578 7072 6573 7369 6f6e 3d22 222f  " expression=""/
+00007830: 3e0a 2020 2020 3c64 6566 6175 6c74 2066  >.    <default f
+00007840: 6965 6c64 3d22 6f73 6d5f 6964 2220 6170  ield="osm_id" ap
+00007850: 706c 794f 6e55 7064 6174 653d 2230 2220  plyOnUpdate="0" 
+00007860: 6578 7072 6573 7369 6f6e 3d22 222f 3e0a  expression=""/>.
+00007870: 2020 2020 3c64 6566 6175 6c74 2066 6965      <default fie
+00007880: 6c64 3d22 6f72 6965 6e74 6174 696f 6e22  ld="orientation"
+00007890: 2061 7070 6c79 4f6e 5570 6461 7465 3d22   applyOnUpdate="
+000078a0: 3022 2065 7870 7265 7373 696f 6e3d 2222  0" expression=""
+000078b0: 2f3e 0a20 2020 203c 6465 6661 756c 7420  />.    <default 
+000078c0: 6669 656c 643d 226f 7269 656e 7461 7469  field="orientati
+000078d0: 6f6e 5f63 6f6e 6669 6465 6e63 6522 2061  on_confidence" a
+000078e0: 7070 6c79 4f6e 5570 6461 7465 3d22 3022  pplyOnUpdate="0"
+000078f0: 2065 7870 7265 7373 696f 6e3d 2222 2f3e   expression=""/>
+00007900: 0a20 2020 203c 6465 6661 756c 7420 6669  .    <default fi
+00007910: 656c 643d 226c 616e 655f 7769 6474 6822  eld="lane_width"
+00007920: 2061 7070 6c79 4f6e 5570 6461 7465 3d22   applyOnUpdate="
+00007930: 3022 2065 7870 7265 7373 696f 6e3d 2222  0" expression=""
+00007940: 2f3e 0a20 2020 203c 6465 6661 756c 7420  />.    <default 
+00007950: 6669 656c 643d 226c 616e 655f 6f72 6965  field="lane_orie
+00007960: 6e74 6174 696f 6e22 2061 7070 6c79 4f6e  ntation" applyOn
+00007970: 5570 6461 7465 3d22 3022 2065 7870 7265  Update="0" expre
+00007980: 7373 696f 6e3d 2222 2f3e 0a20 203c 2f64  ssion=""/>.  </d
+00007990: 6566 6175 6c74 733e 0a20 203c 636f 6e73  efaults>.  <cons
+000079a0: 7472 6169 6e74 733e 0a20 2020 203c 636f  traints>.    <co
+000079b0: 6e73 7472 6169 6e74 2066 6965 6c64 3d22  nstraint field="
+000079c0: 7479 7065 2220 636f 6e73 7472 6169 6e74  type" constraint
+000079d0: 733d 2230 2220 6578 705f 7374 7265 6e67  s="0" exp_streng
+000079e0: 7468 3d22 3022 2075 6e69 7175 655f 7374  th="0" unique_st
+000079f0: 7265 6e67 7468 3d22 3022 206e 6f74 6e75  rength="0" notnu
+00007a00: 6c6c 5f73 7472 656e 6774 683d 2230 222f  ll_strength="0"/
+00007a10: 3e0a 2020 2020 3c63 6f6e 7374 7261 696e  >.    <constrain
+00007a20: 7420 6669 656c 643d 226f 736d 5f69 6422  t field="osm_id"
+00007a30: 2063 6f6e 7374 7261 696e 7473 3d22 3022   constraints="0"
+00007a40: 2065 7870 5f73 7472 656e 6774 683d 2230   exp_strength="0
+00007a50: 2220 756e 6971 7565 5f73 7472 656e 6774  " unique_strengt
+00007a60: 683d 2230 2220 6e6f 746e 756c 6c5f 7374  h="0" notnull_st
+00007a70: 7265 6e67 7468 3d22 3022 2f3e 0a20 2020  rength="0"/>.   
+00007a80: 203c 636f 6e73 7472 6169 6e74 2066 6965   <constraint fie
+00007a90: 6c64 3d22 6f72 6965 6e74 6174 696f 6e22  ld="orientation"
+00007aa0: 2063 6f6e 7374 7261 696e 7473 3d22 3022   constraints="0"
+00007ab0: 2065 7870 5f73 7472 656e 6774 683d 2230   exp_strength="0
+00007ac0: 2220 756e 6971 7565 5f73 7472 656e 6774  " unique_strengt
+00007ad0: 683d 2230 2220 6e6f 746e 756c 6c5f 7374  h="0" notnull_st
+00007ae0: 7265 6e67 7468 3d22 3022 2f3e 0a20 2020  rength="0"/>.   
+00007af0: 203c 636f 6e73 7472 6169 6e74 2066 6965   <constraint fie
+00007b00: 6c64 3d22 6f72 6965 6e74 6174 696f 6e5f  ld="orientation_
+00007b10: 636f 6e66 6964 656e 6365 2220 636f 6e73  confidence" cons
+00007b20: 7472 6169 6e74 733d 2230 2220 6578 705f  traints="0" exp_
+00007b30: 7374 7265 6e67 7468 3d22 3022 2075 6e69  strength="0" uni
+00007b40: 7175 655f 7374 7265 6e67 7468 3d22 3022  que_strength="0"
+00007b50: 206e 6f74 6e75 6c6c 5f73 7472 656e 6774   notnull_strengt
+00007b60: 683d 2230 222f 3e0a 2020 2020 3c63 6f6e  h="0"/>.    <con
+00007b70: 7374 7261 696e 7420 6669 656c 643d 226c  straint field="l
+00007b80: 616e 655f 7769 6474 6822 2063 6f6e 7374  ane_width" const
+00007b90: 7261 696e 7473 3d22 3022 2065 7870 5f73  raints="0" exp_s
+00007ba0: 7472 656e 6774 683d 2230 2220 756e 6971  trength="0" uniq
+00007bb0: 7565 5f73 7472 656e 6774 683d 2230 2220  ue_strength="0" 
+00007bc0: 6e6f 746e 756c 6c5f 7374 7265 6e67 7468  notnull_strength
+00007bd0: 3d22 3022 2f3e 0a20 2020 203c 636f 6e73  ="0"/>.    <cons
+00007be0: 7472 6169 6e74 2066 6965 6c64 3d22 6c61  traint field="la
+00007bf0: 6e65 5f6f 7269 656e 7461 7469 6f6e 2220  ne_orientation" 
+00007c00: 636f 6e73 7472 6169 6e74 733d 2230 2220  constraints="0" 
+00007c10: 6578 705f 7374 7265 6e67 7468 3d22 3022  exp_strength="0"
+00007c20: 2075 6e69 7175 655f 7374 7265 6e67 7468   unique_strength
+00007c30: 3d22 3022 206e 6f74 6e75 6c6c 5f73 7472  ="0" notnull_str
+00007c40: 656e 6774 683d 2230 222f 3e0a 2020 3c2f  ength="0"/>.  </
+00007c50: 636f 6e73 7472 6169 6e74 733e 0a20 203c  constraints>.  <
+00007c60: 636f 6e73 7472 6169 6e74 4578 7072 6573  constraintExpres
+00007c70: 7369 6f6e 733e 0a20 2020 203c 636f 6e73  sions>.    <cons
+00007c80: 7472 6169 6e74 2066 6965 6c64 3d22 7479  traint field="ty
+00007c90: 7065 2220 6578 703d 2222 2064 6573 633d  pe" exp="" desc=
+00007ca0: 2222 2f3e 0a20 2020 203c 636f 6e73 7472  ""/>.    <constr
+00007cb0: 6169 6e74 2066 6965 6c64 3d22 6f73 6d5f  aint field="osm_
+00007cc0: 6964 2220 6578 703d 2222 2064 6573 633d  id" exp="" desc=
+00007cd0: 2222 2f3e 0a20 2020 203c 636f 6e73 7472  ""/>.    <constr
+00007ce0: 6169 6e74 2066 6965 6c64 3d22 6f72 6965  aint field="orie
+00007cf0: 6e74 6174 696f 6e22 2065 7870 3d22 2220  ntation" exp="" 
+00007d00: 6465 7363 3d22 222f 3e0a 2020 2020 3c63  desc=""/>.    <c
+00007d10: 6f6e 7374 7261 696e 7420 6669 656c 643d  onstraint field=
+00007d20: 226f 7269 656e 7461 7469 6f6e 5f63 6f6e  "orientation_con
+00007d30: 6669 6465 6e63 6522 2065 7870 3d22 2220  fidence" exp="" 
+00007d40: 6465 7363 3d22 222f 3e0a 2020 2020 3c63  desc=""/>.    <c
+00007d50: 6f6e 7374 7261 696e 7420 6669 656c 643d  onstraint field=
+00007d60: 226c 616e 655f 7769 6474 6822 2065 7870  "lane_width" exp
+00007d70: 3d22 2220 6465 7363 3d22 222f 3e0a 2020  ="" desc=""/>.  
+00007d80: 2020 3c63 6f6e 7374 7261 696e 7420 6669    <constraint fi
+00007d90: 656c 643d 226c 616e 655f 6f72 6965 6e74  eld="lane_orient
+00007da0: 6174 696f 6e22 2065 7870 3d22 2220 6465  ation" exp="" de
+00007db0: 7363 3d22 222f 3e0a 2020 3c2f 636f 6e73  sc=""/>.  </cons
+00007dc0: 7472 6169 6e74 4578 7072 6573 7369 6f6e  traintExpression
+00007dd0: 733e 0a20 203c 6578 7072 6573 7369 6f6e  s>.  <expression
+00007de0: 6669 656c 6473 2f3e 0a20 203c 6174 7472  fields/>.  <attr
+00007df0: 6962 7574 6561 6374 696f 6e73 3e0a 2020  ibuteactions>.  
+00007e00: 2020 3c64 6566 6175 6c74 4163 7469 6f6e    <defaultAction
+00007e10: 2076 616c 7565 3d22 7b30 3030 3030 3030   value="{0000000
+00007e20: 302d 3030 3030 2d30 3030 302d 3030 3030  0-0000-0000-0000
+00007e30: 2d30 3030 3030 3030 3030 3030 307d 2220  -000000000000}" 
+00007e40: 6b65 793d 2243 616e 7661 7322 2f3e 0a20  key="Canvas"/>. 
+00007e50: 203c 2f61 7474 7269 6275 7465 6163 7469   </attributeacti
+00007e60: 6f6e 733e 0a20 203c 6174 7472 6962 7574  ons>.  <attribut
+00007e70: 6574 6162 6c65 636f 6e66 6967 2061 6374  etableconfig act
+00007e80: 696f 6e57 6964 6765 7453 7479 6c65 3d22  ionWidgetStyle="
+00007e90: 6472 6f70 446f 776e 2220 736f 7274 4f72  dropDown" sortOr
+00007ea0: 6465 723d 2230 2220 736f 7274 4578 7072  der="0" sortExpr
+00007eb0: 6573 7369 6f6e 3d22 223e 0a20 2020 203c  ession="">.    <
+00007ec0: 636f 6c75 6d6e 733e 0a20 2020 2020 203c  columns>.      <
+00007ed0: 636f 6c75 6d6e 2068 6964 6465 6e3d 2230  column hidden="0
+00007ee0: 2220 6e61 6d65 3d22 7479 7065 2220 7769  " name="type" wi
+00007ef0: 6474 683d 222d 3122 2074 7970 653d 2266  dth="-1" type="f
+00007f00: 6965 6c64 222f 3e0a 2020 2020 2020 3c63  ield"/>.      <c
+00007f10: 6f6c 756d 6e20 6869 6464 656e 3d22 3022  olumn hidden="0"
+00007f20: 206e 616d 653d 226f 736d 5f69 6422 2077   name="osm_id" w
+00007f30: 6964 7468 3d22 3137 3122 2074 7970 653d  idth="171" type=
+00007f40: 2266 6965 6c64 222f 3e0a 2020 2020 2020  "field"/>.      
+00007f50: 3c63 6f6c 756d 6e20 6869 6464 656e 3d22  <column hidden="
+00007f60: 3022 206e 616d 653d 226f 7269 656e 7461  0" name="orienta
+00007f70: 7469 6f6e 2220 7769 6474 683d 2232 3932  tion" width="292
+00007f80: 2220 7479 7065 3d22 6669 656c 6422 2f3e  " type="field"/>
+00007f90: 0a20 2020 2020 203c 636f 6c75 6d6e 2068  .      <column h
+00007fa0: 6964 6465 6e3d 2230 2220 6e61 6d65 3d22  idden="0" name="
+00007fb0: 6f72 6965 6e74 6174 696f 6e5f 636f 6e66  orientation_conf
+00007fc0: 6964 656e 6365 2220 7769 6474 683d 222d  idence" width="-
+00007fd0: 3122 2074 7970 653d 2266 6965 6c64 222f  1" type="field"/
+00007fe0: 3e0a 2020 2020 2020 3c63 6f6c 756d 6e20  >.      <column 
+00007ff0: 6869 6464 656e 3d22 3022 206e 616d 653d  hidden="0" name=
+00008000: 226c 616e 655f 6f72 6965 6e74 6174 696f  "lane_orientatio
+00008010: 6e22 2077 6964 7468 3d22 2d31 2220 7479  n" width="-1" ty
+00008020: 7065 3d22 6669 656c 6422 2f3e 0a20 2020  pe="field"/>.   
+00008030: 2020 203c 636f 6c75 6d6e 2068 6964 6465     <column hidde
+00008040: 6e3d 2230 2220 6e61 6d65 3d22 6c61 6e65  n="0" name="lane
+00008050: 5f77 6964 7468 2220 7769 6474 683d 222d  _width" width="-
+00008060: 3122 2074 7970 653d 2266 6965 6c64 222f  1" type="field"/
+00008070: 3e0a 2020 2020 2020 3c63 6f6c 756d 6e20  >.      <column 
+00008080: 6869 6464 656e 3d22 3122 2077 6964 7468  hidden="1" width
+00008090: 3d22 2d31 2220 7479 7065 3d22 6163 7469  ="-1" type="acti
+000080a0: 6f6e 7322 2f3e 0a20 2020 203c 2f63 6f6c  ons"/>.    </col
+000080b0: 756d 6e73 3e0a 2020 3c2f 6174 7472 6962  umns>.  </attrib
+000080c0: 7574 6574 6162 6c65 636f 6e66 6967 3e0a  utetableconfig>.
+000080d0: 2020 3c63 6f6e 6469 7469 6f6e 616c 7374    <conditionalst
+000080e0: 796c 6573 3e0a 2020 2020 3c72 6f77 7374  yles>.    <rowst
+000080f0: 796c 6573 2f3e 0a20 2020 203c 6669 656c  yles/>.    <fiel
+00008100: 6473 7479 6c65 732f 3e0a 2020 3c2f 636f  dstyles/>.  </co
+00008110: 6e64 6974 696f 6e61 6c73 7479 6c65 733e  nditionalstyles>
+00008120: 0a20 203c 7374 6f72 6564 6578 7072 6573  .  <storedexpres
+00008130: 7369 6f6e 732f 3e0a 2020 3c65 6469 7466  sions/>.  <editf
+00008140: 6f72 6d20 746f 6c65 7261 6e74 3d22 3122  orm tolerant="1"
+00008150: 3e3c 2f65 6469 7466 6f72 6d3e 0a20 203c  ></editform>.  <
+00008160: 6564 6974 666f 726d 696e 6974 2f3e 0a20  editforminit/>. 
+00008170: 203c 6564 6974 666f 726d 696e 6974 636f   <editforminitco
+00008180: 6465 736f 7572 6365 3e30 3c2f 6564 6974  desource>0</edit
+00008190: 666f 726d 696e 6974 636f 6465 736f 7572  forminitcodesour
+000081a0: 6365 3e0a 2020 3c65 6469 7466 6f72 6d69  ce>.  <editformi
+000081b0: 6e69 7466 696c 6570 6174 683e 3c2f 6564  nitfilepath></ed
+000081c0: 6974 666f 726d 696e 6974 6669 6c65 7061  itforminitfilepa
+000081d0: 7468 3e0a 2020 3c65 6469 7466 6f72 6d69  th>.  <editformi
+000081e0: 6e69 7463 6f64 653e 3c21 5b43 4441 5441  nitcode><![CDATA
+000081f0: 5b23 202d 2a2d 2063 6f64 696e 673a 2075  [# -*- coding: u
+00008200: 7466 2d38 202d 2a2d 0a22 2222 0a4c 6573  tf-8 -*-.""".Les
+00008210: 2066 6f72 6d75 6c61 6972 6573 2051 4749   formulaires QGI
+00008220: 5320 7065 7576 656e 7420 6176 6f69 7220  S peuvent avoir 
+00008230: 756e 6520 666f 6e63 7469 6f6e 2050 7974  une fonction Pyt
+00008240: 686f 6e20 7175 6920 6573 7420 6170 7065  hon qui est appe
+00008250: 6cc3 a965 206c 6f72 7371 7565 206c 6520  l..e lorsque le 
+00008260: 666f 726d 756c 6169 7265 2065 7374 0a6f  formulaire est.o
+00008270: 7576 6572 742e 0a0a 5574 696c 6973 657a  uvert...Utilisez
+00008280: 2063 6574 7465 2066 6f6e 6374 696f 6e20   cette fonction 
+00008290: 706f 7572 2061 6a6f 7574 6572 2075 6e65  pour ajouter une
+000082a0: 206c 6f67 6971 7565 2073 7570 706c c3a9   logique suppl..
+000082b0: 6d65 6e74 6169 7265 20c3 a020 766f 7320  mentaire .. vos 
+000082c0: 666f 726d 756c 6169 7265 732e 0a0a 456e  formulaires...En
+000082d0: 7472 657a 206c 6520 6e6f 6d20 6465 206c  trez le nom de l
+000082e0: 6120 666f 6e63 7469 6f6e 2064 616e 7320  a fonction dans 
+000082f0: 6c65 2063 6861 6d70 200a 2246 6f6e 6374  le champ ."Fonct
+00008300: 696f 6e20 6427 696e 6974 6961 6c69 7361  ion d'initialisa
+00008310: 7469 6f6e 2050 7974 686f 6e22 2e0a 566f  tion Python"..Vo
+00008320: 6963 6920 756e 2065 7865 6d70 6c65 3a0a  ici un exemple:.
+00008330: 2222 220a 6672 6f6d 2071 6769 732e 5079  """.from qgis.Py
+00008340: 5174 2e51 7457 6964 6765 7473 2069 6d70  Qt.QtWidgets imp
+00008350: 6f72 7420 5157 6964 6765 740a 0a64 6566  ort QWidget..def
+00008360: 206d 795f 666f 726d 5f6f 7065 6e28 6469   my_form_open(di
+00008370: 616c 6f67 2c20 6c61 7965 722c 2066 6561  alog, layer, fea
+00008380: 7475 7265 293a 0a20 2020 2067 656f 6d20  ture):.    geom 
+00008390: 3d20 6665 6174 7572 652e 6765 6f6d 6574  = feature.geomet
+000083a0: 7279 2829 0a20 2020 2063 6f6e 7472 6f6c  ry().    control
+000083b0: 203d 2064 6961 6c6f 672e 6669 6e64 4368   = dialog.findCh
+000083c0: 696c 6428 5157 6964 6765 742c 2022 4d79  ild(QWidget, "My
+000083d0: 4c69 6e65 4564 6974 2229 0a5d 5d3e 3c2f  LineEdit").]]></
+000083e0: 6564 6974 666f 726d 696e 6974 636f 6465  editforminitcode
+000083f0: 3e0a 2020 3c66 6561 7466 6f72 6d73 7570  >.  <featformsup
+00008400: 7072 6573 733e 303c 2f66 6561 7466 6f72  press>0</featfor
+00008410: 6d73 7570 7072 6573 733e 0a20 203c 6564  msuppress>.  <ed
+00008420: 6974 6f72 6c61 796f 7574 3e67 656e 6572  itorlayout>gener
+00008430: 6174 6564 6c61 796f 7574 3c2f 6564 6974  atedlayout</edit
+00008440: 6f72 6c61 796f 7574 3e0a 2020 3c65 6469  orlayout>.  <edi
+00008450: 7461 626c 653e 0a20 2020 203c 6669 656c  table>.    <fiel
+00008460: 6420 6e61 6d65 3d22 616e 676c 6522 2065  d name="angle" e
+00008470: 6469 7461 626c 653d 2231 222f 3e0a 2020  ditable="1"/>.  
+00008480: 2020 3c66 6965 6c64 206e 616d 653d 2266    <field name="f
+00008490: 6964 2220 6564 6974 6162 6c65 3d22 3122  id" editable="1"
+000084a0: 2f3e 0a20 2020 203c 6669 656c 6420 6e61  />.    <field na
+000084b0: 6d65 3d22 6c61 6e65 5f6f 7269 656e 7461  me="lane_orienta
+000084c0: 7469 6f6e 2220 6564 6974 6162 6c65 3d22  tion" editable="
+000084d0: 3122 2f3e 0a20 2020 203c 6669 656c 6420  1"/>.    <field 
+000084e0: 6e61 6d65 3d22 6c61 6e65 5f77 6964 7468  name="lane_width
+000084f0: 2220 6564 6974 6162 6c65 3d22 3122 2f3e  " editable="1"/>
+00008500: 0a20 2020 203c 6669 656c 6420 6e61 6d65  .    <field name
+00008510: 3d22 6f72 6965 6e74 6174 696f 6e22 2065  ="orientation" e
+00008520: 6469 7461 626c 653d 2231 222f 3e0a 2020  ditable="1"/>.  
+00008530: 2020 3c66 6965 6c64 206e 616d 653d 226f    <field name="o
+00008540: 7269 656e 7461 7469 6f6e 5f63 6f6e 6669  rientation_confi
+00008550: 6465 6e63 6522 2065 6469 7461 626c 653d  dence" editable=
+00008560: 2231 222f 3e0a 2020 2020 3c66 6965 6c64  "1"/>.    <field
+00008570: 206e 616d 653d 226f 736d 5f69 6422 2065   name="osm_id" e
+00008580: 6469 7461 626c 653d 2231 222f 3e0a 2020  ditable="1"/>.  
+00008590: 2020 3c66 6965 6c64 206e 616d 653d 2274    <field name="t
+000085a0: 7970 6522 2065 6469 7461 626c 653d 2231  ype" editable="1
+000085b0: 222f 3e0a 2020 3c2f 6564 6974 6162 6c65  "/>.  </editable
+000085c0: 3e0a 2020 3c6c 6162 656c 4f6e 546f 703e  >.  <labelOnTop>
+000085d0: 0a20 2020 203c 6669 656c 6420 6c61 6265  .    <field labe
+000085e0: 6c4f 6e54 6f70 3d22 3022 206e 616d 653d  lOnTop="0" name=
+000085f0: 2261 6e67 6c65 222f 3e0a 2020 2020 3c66  "angle"/>.    <f
+00008600: 6965 6c64 206c 6162 656c 4f6e 546f 703d  ield labelOnTop=
+00008610: 2230 2220 6e61 6d65 3d22 6669 6422 2f3e  "0" name="fid"/>
+00008620: 0a20 2020 203c 6669 656c 6420 6c61 6265  .    <field labe
+00008630: 6c4f 6e54 6f70 3d22 3022 206e 616d 653d  lOnTop="0" name=
+00008640: 226c 616e 655f 6f72 6965 6e74 6174 696f  "lane_orientatio
+00008650: 6e22 2f3e 0a20 2020 203c 6669 656c 6420  n"/>.    <field 
+00008660: 6c61 6265 6c4f 6e54 6f70 3d22 3022 206e  labelOnTop="0" n
+00008670: 616d 653d 226c 616e 655f 7769 6474 6822  ame="lane_width"
+00008680: 2f3e 0a20 2020 203c 6669 656c 6420 6c61  />.    <field la
+00008690: 6265 6c4f 6e54 6f70 3d22 3022 206e 616d  belOnTop="0" nam
+000086a0: 653d 226f 7269 656e 7461 7469 6f6e 222f  e="orientation"/
+000086b0: 3e0a 2020 2020 3c66 6965 6c64 206c 6162  >.    <field lab
+000086c0: 656c 4f6e 546f 703d 2230 2220 6e61 6d65  elOnTop="0" name
+000086d0: 3d22 6f72 6965 6e74 6174 696f 6e5f 636f  ="orientation_co
+000086e0: 6e66 6964 656e 6365 222f 3e0a 2020 2020  nfidence"/>.    
+000086f0: 3c66 6965 6c64 206c 6162 656c 4f6e 546f  <field labelOnTo
+00008700: 703d 2230 2220 6e61 6d65 3d22 6f73 6d5f  p="0" name="osm_
+00008710: 6964 222f 3e0a 2020 2020 3c66 6965 6c64  id"/>.    <field
+00008720: 206c 6162 656c 4f6e 546f 703d 2230 2220   labelOnTop="0" 
+00008730: 6e61 6d65 3d22 7479 7065 222f 3e0a 2020  name="type"/>.  
+00008740: 3c2f 6c61 6265 6c4f 6e54 6f70 3e0a 2020  </labelOnTop>.  
+00008750: 3c72 6575 7365 4c61 7374 5661 6c75 653e  <reuseLastValue>
+00008760: 0a20 2020 203c 6669 656c 6420 6e61 6d65  .    <field name
+00008770: 3d22 616e 676c 6522 2072 6575 7365 4c61  ="angle" reuseLa
+00008780: 7374 5661 6c75 653d 2230 222f 3e0a 2020  stValue="0"/>.  
+00008790: 2020 3c66 6965 6c64 206e 616d 653d 2266    <field name="f
+000087a0: 6964 2220 7265 7573 654c 6173 7456 616c  id" reuseLastVal
+000087b0: 7565 3d22 3022 2f3e 0a20 2020 203c 6669  ue="0"/>.    <fi
+000087c0: 656c 6420 6e61 6d65 3d22 6c61 6e65 5f6f  eld name="lane_o
+000087d0: 7269 656e 7461 7469 6f6e 2220 7265 7573  rientation" reus
+000087e0: 654c 6173 7456 616c 7565 3d22 3022 2f3e  eLastValue="0"/>
+000087f0: 0a20 2020 203c 6669 656c 6420 6e61 6d65  .    <field name
+00008800: 3d22 6c61 6e65 5f77 6964 7468 2220 7265  ="lane_width" re
+00008810: 7573 654c 6173 7456 616c 7565 3d22 3022  useLastValue="0"
+00008820: 2f3e 0a20 2020 203c 6669 656c 6420 6e61  />.    <field na
+00008830: 6d65 3d22 6f72 6965 6e74 6174 696f 6e22  me="orientation"
+00008840: 2072 6575 7365 4c61 7374 5661 6c75 653d   reuseLastValue=
+00008850: 2230 222f 3e0a 2020 2020 3c66 6965 6c64  "0"/>.    <field
+00008860: 206e 616d 653d 226f 7269 656e 7461 7469   name="orientati
+00008870: 6f6e 5f63 6f6e 6669 6465 6e63 6522 2072  on_confidence" r
+00008880: 6575 7365 4c61 7374 5661 6c75 653d 2230  euseLastValue="0
+00008890: 222f 3e0a 2020 2020 3c66 6965 6c64 206e  "/>.    <field n
+000088a0: 616d 653d 226f 736d 5f69 6422 2072 6575  ame="osm_id" reu
+000088b0: 7365 4c61 7374 5661 6c75 653d 2230 222f  seLastValue="0"/
+000088c0: 3e0a 2020 2020 3c66 6965 6c64 206e 616d  >.    <field nam
+000088d0: 653d 2274 7970 6522 2072 6575 7365 4c61  e="type" reuseLa
+000088e0: 7374 5661 6c75 653d 2230 222f 3e0a 2020  stValue="0"/>.  
+000088f0: 3c2f 7265 7573 654c 6173 7456 616c 7565  </reuseLastValue
+00008900: 3e0a 2020 3c64 6174 6144 6566 696e 6564  >.  <dataDefined
+00008910: 4669 656c 6450 726f 7065 7274 6965 732f  FieldProperties/
+00008920: 3e0a 2020 3c77 6964 6765 7473 2f3e 0a20  >.  <widgets/>. 
+00008930: 203c 7072 6576 6965 7745 7870 7265 7373   <previewExpress
+00008940: 696f 6e3e 2274 7970 6522 3c2f 7072 6576  ion>"type"</prev
+00008950: 6965 7745 7870 7265 7373 696f 6e3e 0a20  iewExpression>. 
+00008960: 203c 6d61 7054 6970 3e3c 2f6d 6170 5469   <mapTip></mapTi
+00008970: 703e 0a20 203c 6c61 7965 7247 656f 6d65  p>.  <layerGeome
+00008980: 7472 7954 7970 653e 303c 2f6c 6179 6572  tryType>0</layer
+00008990: 4765 6f6d 6574 7279 5479 7065 3e0a 3c2f  GeometryType>.</
+000089a0: 7167 6973 3e0a                           qgis>.
```

### Comparing `crossroads-schematization-0.0.9/crschem/resources/rendering-polylines-space.qml` & `crossroads-schematization-0.1.0/crschem/resources/rendering-polylines-space.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.0.9/crschem/resources/rendering-polylines.qml` & `crossroads-schematization-0.1.0/crschem/resources/rendering-polylines.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.0.9/crschem/resources/tactile-a5.qpt` & `crossroads-schematization-0.1.0/crschem/resources/tactile-a5.qpt`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.0.9/crschem/utils.py` & `crossroads-schematization-0.1.0/crschem/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,14 +52,27 @@
         return v / norm
 
 
     def edge_length(n1, n2):
         v = Utils.vector(n1, n2)
         return linalg.norm(np.array(v), 2)
 
+    # return true if p is a point in the edge (n1, n2)
+    def is_in_edge(p, n1, n2):
+        v = Utils.vector(n1, n2)
+        vp = Utils.vector(n1, p)
+
+        # first check if they are colinear
+        if abs(np.cross(v, vp)) > 1e-6:
+            return False
+
+        dot = np.dot(v, vp)
+        dotv = np.dot(v, v)
+        return dot >= 0 and dot <= dotv
+
 
     def reverse_geom(geom):
         def _reverse(x, y, z=None):
             if z:
                 return x[::-1], y[::-1], z[::-1]
             return x[::-1], y[::-1]
 
@@ -87,15 +100,15 @@
 
     def angle_mean(a1, a2):
         a1 = Utils.angle_modulo(a1)
         a2 = Utils.angle_modulo(a2)
 
         m1 = (a1 + a2) / 2
         if m1 > math.pi:
-            return m1 - math.pi
+            return m1 - 2 * math.pi
         else:
             return m1
 
     
     def turn_angle(G, middle, n2, n3):
         c1 = (G.nodes[middle]["x"], G.nodes[middle]["y"])
         c2 = (G.nodes[n2]["x"], G.nodes[n2]["y"])
@@ -206,28 +219,32 @@
         if ("cycleway:right" in gEdge and gEdge["cycleway:right"] == "lane") or \
            ("cycleway:left" in gEdge and gEdge["cycleway:left"] == "lane"):
             result += 1 # one meter per cycle lane
 
         return result
 
     def get_initial_node_tags(cr_input, osm_n1):
-        is_n = cr_input["osm_node_id"] == str(osm_n1)
-        filtered = cr_input[is_n]
-        if len(filtered) > 0:
-            return filtered.iloc[0, :].to_dict()
+        if "osm_node_id" in cr_input.columns.tolist():
+            is_n = cr_input["osm_node_id"] == str(osm_n1)
+            filtered = cr_input[is_n]
+            if len(filtered) > 0:
+                return filtered.iloc[0, :].to_dict()
+            else:
+                return None
         else:
-            return None
+                return None
+        
 
 
     def get_initial_edge_tags(cr_input, osm_n1, osm_n2, inverse = False):
         for index, row in cr_input.iterrows():
             if row["osm_node_ids"] == [str(osm_n1), str(osm_n2)]:
                 return row.to_dict()
         if inverse:
-            return Utils.get_initial_edge_tags(cr_input, osm_n1, osm_n2, False)
+            return Utils.get_initial_edge_tags(cr_input, osm_n2, osm_n1, False)
         else:
             return None
 
 
     def pathid_to_pathcoords(path, osm):
         return [(osm.nodes[n]["x"], osm.nodes[n]["y"]) for n in path]
```

### Comparing `crossroads-schematization-0.0.9/setup.py` & `crossroads-schematization-0.1.0/setup.py`

 * *Files identical despite different names*

