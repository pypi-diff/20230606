# Comparing `tmp/vrpSolver-0.0.8.tar.gz` & `tmp/vrpSolver-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vrpSolver-0.0.8.tar", last modified: Sun Jul 18 21:28:55 2021, max compression
+gzip compressed data, was "dist\vrpSolver-0.0.9.tar", last modified: Wed Jul 21 05:20:29 2021, max compression
```

## Comparing `vrpSolver-0.0.8.tar` & `vrpSolver-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2021-07-18 21:28:55.000000 vrpSolver-0.0.8/
--rw-rw-rw-   0        0        0      789 2021-07-18 21:28:55.000000 vrpSolver-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2021-07-18 21:28:55.000000 vrpSolver-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1008 2021-04-21 02:25:53.000000 vrpSolver-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-07-18 21:28:55.000000 vrpSolver-0.0.8/vrpSolver/
--rw-rw-rw-   0        0        0    36727 2021-07-18 21:21:55.000000 vrpSolver-0.0.8/vrpSolver/TSP.py
--rw-rw-rw-   0        0        0     1383 2021-07-18 21:26:47.000000 vrpSolver-0.0.8/vrpSolver/__init__.py
--rw-rw-rw-   0        0        0    11575 2021-07-18 20:40:56.000000 vrpSolver-0.0.8/vrpSolver/cgCVRPTW.py
--rw-rw-rw-   0        0        0      283 2021-07-18 20:59:04.000000 vrpSolver-0.0.8/vrpSolver/color.py
--rw-rw-rw-   0        0        0     7029 2021-07-18 20:59:22.000000 vrpSolver-0.0.8/vrpSolver/common.py
--rw-rw-rw-   0        0        0     7548 2021-07-18 20:43:15.000000 vrpSolver-0.0.8/vrpSolver/consVRP.py
--rw-rw-rw-   0        0        0       23 2020-11-03 06:30:13.000000 vrpSolver-0.0.8/vrpSolver/const.py
--rw-rw-rw-   0        0        0     7759 2021-07-18 20:43:42.000000 vrpSolver-0.0.8/vrpSolver/instance.py
--rw-rw-rw-   0        0        0    11680 2021-07-18 20:37:36.000000 vrpSolver-0.0.8/vrpSolver/ipCVRP.py
--rw-rw-rw-   0        0        0     2437 2021-07-18 20:54:11.000000 vrpSolver-0.0.8/vrpSolver/matching.py
--rw-rw-rw-   0        0        0     3036 2021-07-18 20:38:21.000000 vrpSolver-0.0.8/vrpSolver/msg.py
--rw-rw-rw-   0        0        0     3534 2021-07-18 20:40:18.000000 vrpSolver-0.0.8/vrpSolver/mst.py
--rw-rw-rw-   0        0        0    21713 2021-07-18 20:58:35.000000 vrpSolver-0.0.8/vrpSolver/plot.py
--rw-rw-rw-   0        0        0      773 2021-07-18 21:21:06.000000 vrpSolver-0.0.8/vrpSolver/shortestPath.py
--rw-rw-rw-   0        0        0     9050 2021-07-18 21:12:44.000000 vrpSolver-0.0.8/vrpSolver/timeWindows.py
--rw-rw-rw-   0        0        0     3015 2021-07-18 20:43:01.000000 vrpSolver-0.0.8/vrpSolver/traversal.py
-drwxrwxrwx   0        0        0        0 2021-07-18 21:28:55.000000 vrpSolver-0.0.8/vrpSolver.egg-info/
--rw-rw-rw-   0        0        0      789 2021-07-18 21:28:55.000000 vrpSolver-0.0.8/vrpSolver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      502 2021-07-18 21:28:55.000000 vrpSolver-0.0.8/vrpSolver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-07-18 21:28:55.000000 vrpSolver-0.0.8/vrpSolver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2021-07-18 21:28:55.000000 vrpSolver-0.0.8/vrpSolver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2021-07-18 21:28:55.000000 vrpSolver-0.0.8/vrpSolver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-07-21 05:20:29.000000 vrpSolver-0.0.9/
+-rw-rw-rw-   0        0        0      789 2021-07-21 05:20:29.000000 vrpSolver-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2021-07-21 05:20:29.000000 vrpSolver-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1008 2021-04-21 02:25:53.000000 vrpSolver-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-07-21 05:20:29.000000 vrpSolver-0.0.9/vrpSolver/
+-rw-rw-rw-   0        0        0    36667 2021-07-18 21:50:41.000000 vrpSolver-0.0.9/vrpSolver/TSP.py
+-rw-rw-rw-   0        0        0     1464 2021-07-21 05:20:07.000000 vrpSolver-0.0.9/vrpSolver/__init__.py
+-rw-rw-rw-   0        0        0    11575 2021-07-18 20:40:56.000000 vrpSolver-0.0.9/vrpSolver/cgCVRPTW.py
+-rw-rw-rw-   0        0        0      283 2021-07-18 20:59:04.000000 vrpSolver-0.0.9/vrpSolver/color.py
+-rw-rw-rw-   0        0        0     7882 2021-07-18 23:08:50.000000 vrpSolver-0.0.9/vrpSolver/common.py
+-rw-rw-rw-   0        0        0     7548 2021-07-18 20:43:15.000000 vrpSolver-0.0.9/vrpSolver/consVRP.py
+-rw-rw-rw-   0        0        0       23 2020-11-03 06:30:13.000000 vrpSolver-0.0.9/vrpSolver/const.py
+-rw-rw-rw-   0        0        0     7759 2021-07-18 20:43:42.000000 vrpSolver-0.0.9/vrpSolver/instance.py
+-rw-rw-rw-   0        0        0    11680 2021-07-18 20:37:36.000000 vrpSolver-0.0.9/vrpSolver/ipCVRP.py
+-rw-rw-rw-   0        0        0     2437 2021-07-18 20:54:11.000000 vrpSolver-0.0.9/vrpSolver/matching.py
+-rw-rw-rw-   0        0        0     3036 2021-07-18 20:38:21.000000 vrpSolver-0.0.9/vrpSolver/msg.py
+-rw-rw-rw-   0        0        0     3534 2021-07-18 20:40:18.000000 vrpSolver-0.0.9/vrpSolver/mst.py
+-rw-rw-rw-   0        0        0    22362 2021-07-21 05:18:25.000000 vrpSolver-0.0.9/vrpSolver/plot.py
+-rw-rw-rw-   0        0        0      773 2021-07-18 21:21:06.000000 vrpSolver-0.0.9/vrpSolver/shortestPath.py
+-rw-rw-rw-   0        0        0    12985 2021-07-20 21:08:32.000000 vrpSolver-0.0.9/vrpSolver/timeWindows.py
+-rw-rw-rw-   0        0        0     3015 2021-07-18 20:43:01.000000 vrpSolver-0.0.9/vrpSolver/traversal.py
+drwxrwxrwx   0        0        0        0 2021-07-21 05:20:29.000000 vrpSolver-0.0.9/vrpSolver.egg-info/
+-rw-rw-rw-   0        0        0      789 2021-07-21 05:20:28.000000 vrpSolver-0.0.9/vrpSolver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      502 2021-07-21 05:20:29.000000 vrpSolver-0.0.9/vrpSolver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-07-21 05:20:28.000000 vrpSolver-0.0.9/vrpSolver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2021-07-21 05:20:28.000000 vrpSolver-0.0.9/vrpSolver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2021-07-21 05:20:28.000000 vrpSolver-0.0.9/vrpSolver.egg-info/top_level.txt
```

### Comparing `vrpSolver-0.0.8/PKG-INFO` & `vrpSolver-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vrpSolver
-Version: 0.0.8
+Version: 0.0.9
 Summary: VRP Solver
 Home-page: https://github.com/isaac0821/vrpSolver
 Author: Lan Peng
 Author-email: lanpeng@buffalo.edu
 License: MIT
 Download-URL: https://github.com/isaac0821/vrpSolver
 Project-URL: Bug Tracker, https://github.com/isaac0821/vrpSolver/issues
```

### Comparing `vrpSolver-0.0.8/setup.py` & `vrpSolver-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `vrpSolver-0.0.8/vrpSolver/TSP.py` & `vrpSolver-0.0.9/vrpSolver/TSP.py`

 * *Files 0% similar despite different names*

```diff
@@ -601,21 +601,20 @@
     # Define nodeIDs ==========================================================
     if (type(nodeIDs) is not list):
         if (nodeIDs == 'All'):
             nodeIDs = []
             for i in nodes:
                 nodeIDs.append(i)
 
-    # Define edges ==============================================================
+    # Define edges ============================================================
     if (type(edges) is not dict):
-        lstNodeID = nodeIDs.copy()
         if (edges == 'Euclidean'):
-            edges = getTauEuclidean(nodes, lstNodeID)
+            edges = getTauEuclidean(nodes)
         elif (edges == 'SphereEuclidean'):
-            edges = getTauSphereEuclidean(nodes, lstNodeID)
+            edges = getTauSphereEuclidean(nodes)
         else:
             print("Error: Incorrect type `edges`")
             return None
 
     # Initialize ==============================================================
     k = 0
     u = [0 for i in range(len(nodeIDs))]
```

### Comparing `vrpSolver-0.0.8/vrpSolver/__init__.py` & `vrpSolver-0.0.9/vrpSolver/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 __author__ = "Lan Peng"
 
 # History =====================================================================
 # v0.0.1  - 04202021 - Initial upload
 # v0.0.2  - 04282021 - Add `plotGantt()` function to plot Gantt chart
 # v0.0.3  - 05022021 - `plotGantt()` add descriptions
 # v0.0.4  - 05042021 - Reorganize structure of package
@@ -11,14 +11,15 @@
 #                      with time windows
 # v0.0.5  - 05042021 - Minor fixes
 # v0.0.6  - 05052021 - Add `timePin` option to `plotGantt()` function
 # v0.0.7  - 05262021 - Gantt enables force drawing time window
 # v0.0.8  - 07182021 - Massive change of structure
 #                    - Add `heuTSP()` for TSP heuristic
 #                    - Add time window functions
+# v0.0.9  - 07212021 - Fix some functions in `timeWindows.py` and `plotGantt()`
 # =============================================================================
 
 # Constants and messages
 from .const import *
 from .msg import *
 
 # Basic modules
```

### Comparing `vrpSolver-0.0.8/vrpSolver/cgCVRPTW.py` & `vrpSolver-0.0.9/vrpSolver/cgCVRPTW.py`

 * *Files identical despite different names*

### Comparing `vrpSolver-0.0.8/vrpSolver/common.py` & `vrpSolver-0.0.9/vrpSolver/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -204,7 +204,29 @@
         if (arcs[i][1] not in neighbors):
             neighbors[arcs[i][1]] = [arcs[i][0]]
         else:
             neighbors[arcs[i][1]].append(arcs[i][0])
 
     return neighbors
 
+def insideInterval(
+    val:            "The value to be compared with the interval" = None,
+    interval:   "List, in the format of [start, end], None if no constraint on that side" = [None, None]    
+    ) -> "Given a value `val`, returns true if `val` is inside the interval (or on the edge), false else wise.":
+
+    # Initialize ==============================================================
+    insideFlag = True
+    [s, e] = interval
+
+    # Check left side =========================================================
+    if (s != None):
+        if (val < s):
+            insideFlag = False
+            return insideFlag
+
+    # Check right side ========================================================
+    if (e != None):
+        if (val > e):
+            insideFlag = False
+            return insideFlag
+
+    return insideFlag
```

### Comparing `vrpSolver-0.0.8/vrpSolver/consVRP.py` & `vrpSolver-0.0.9/vrpSolver/consVRP.py`

 * *Files identical despite different names*

### Comparing `vrpSolver-0.0.8/vrpSolver/instance.py` & `vrpSolver-0.0.9/vrpSolver/instance.py`

 * *Files identical despite different names*

### Comparing `vrpSolver-0.0.8/vrpSolver/ipCVRP.py` & `vrpSolver-0.0.9/vrpSolver/ipCVRP.py`

 * *Files identical despite different names*

### Comparing `vrpSolver-0.0.8/vrpSolver/matching.py` & `vrpSolver-0.0.9/vrpSolver/matching.py`

 * *Files identical despite different names*

### Comparing `vrpSolver-0.0.8/vrpSolver/msg.py` & `vrpSolver-0.0.9/vrpSolver/msg.py`

 * *Files identical despite different names*

### Comparing `vrpSolver-0.0.8/vrpSolver/mst.py` & `vrpSolver-0.0.9/vrpSolver/mst.py`

 * *Files identical despite different names*

### Comparing `vrpSolver-0.0.8/vrpSolver/plot.py` & `vrpSolver-0.0.9/vrpSolver/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,18 +29,20 @@
                         'timePin': timePin, \
                         'desc': desc, \
                         'color': (optional, default as 'Random') color \
                     }]\
                 " = None,
     gridFlag:   "True if turn on the grid as background" = True,
     labelFlag:  "True if add label of entities on Gantt chart" = True,
+    linewidth:  "The width of Gantt block borders" = 1,
     entities:   "The Gantt chart will be drawn in this order, if None, takes the entities in `gantt`" = None,
     forceStartEndFlag: "Force the start time and end time of gantt" = False,
     startTime:  "Start time of Gantt, default to be 0, if None, use the earliest time in `gantt`" = 0,
     endTime:    "End time of Gantt, default to be None, if None, use the latest time in `gantt`" = None,
+    showTail:   "Show the latest time of all gantt blocks" = True,
     width:      "Width of the figure" = 12,
     height:     "Height of the figure" = 5,
     pinWidth:   "Width for pins" = 2,
     saveFigPath:"1) None, if not exporting image, or \
                  2) String, the path for exporting image" = None
     ) -> "Given a Gantt dictionary, plot Gantt":
 
@@ -129,73 +131,81 @@
     # Grids ===================================================================
     if (gridFlag):
         ax.grid(b = True, linestyle=':')
 
     # Loop through `gantt` and draw gantt =====================================
     for g in gantt:
         if (g['entityID'] in entities):
-            
-
             bottom = len(entities) - entities.index(g['entityID']) - 0.9
             top = 0
             if (labelFlag == True):
                 top = len(entities) - entities.index(g['entityID']) - 0.5
             else:
                 top = len(entities) - entities.index(g['entityID']) - 0.25
             if ('timeWindow' in g):
                 s = g['timeWindow'][0]
                 e = g['timeWindow'][1]
                 x = [s, s, e, e, s]
                 y = [bottom, top, top, bottom, bottom]
-                ax.plot(x, y, color = 'black', linewidth = 1)
+                ax.plot(x, y, color = 'black', linewidth = linewidth)
                 if (g['color'] != 'random'):
-                    ax.fill(x, y, color = g['color'])
+                    ax.fill(x, y, color = g['color'], linewidth = linewidth)
                 else:
                     rndColor = colorRandom()
-                    ax.fill(x, y, color = rndColor)
+                    ax.fill(x, y, color = rndColor, linewidth = linewidth)
                 if (labelFlag == True):
                     ax.annotate(g['desc'], (s, top + 0.1))
                 if (g['style'] != 'solid'):
-                    ax.fill(x, y, hatch = g['style'], fill=False)
+                    ax.fill(x, y, hatch = g['style'], fill=False, linewidth = linewidth)
             elif ('timeStamps' in g):
                 for i in range(len(g['timeStamps']) - 1):
                     s = g['timeStamps'][i]
                     e = g['timeStamps'][i + 1]
                     x = [s, s, e, e, s]
                     y = [bottom, top, top, bottom, bottom]
-                    ax.plot(x, y, color = 'black', linewidth = 1)
+                    ax.plot(x, y, color = 'black', linewidth = linewidth)
                     ax.annotate(g['desc'][i], (s, top + 0.1))
                     if (g['color'] != 'random'):
-                        ax.fill(x, y, color = g['color'])
+                        ax.fill(x, y, color = g['color'], linewidth = linewidth)
                     else:
                         rndColor = colorRandom()
-                        ax.fill(x, y, color = rndColor)
+                        ax.fill(x, y, color = rndColor, linewidth = linewidth)
                     if (g['style'] != 'solid'):
-                        ax.fill(x, y, hatch = g['style'], fill=False)
+                        ax.fill(x, y, hatch = g['style'], fill=False, linewidth = linewidth)
                 if (labelFlag == True):
                     ax.annotate(g['desc'][-1], (g['timeStamps'][-1], top + 0.1))
             elif ('timePin' in g):
                 s = g['timePin'] - pinWidth
                 m = g['timePin']
                 e = g['timePin'] + pinWidth
                 x = [m, s, e, m]
                 y1 = [top, top + 0.1, top + 0.1, top]
                 y2 = [bottom, bottom - 0.1, bottom - 0.1, bottom]
                 if (g['color'] != 'random'):
                     ax.fill(x, y1, color = g['color'])
                     ax.fill(x, y2, color = g['color'])
-                    ax.plot([m, m], [bottom, top], linewidth = 2, color = g['color'])
+                    ax.plot([m, m], [bottom, top], linewidth = pinWidth, color = g['color'])
                 else:
                     rndColor = colorRandom()
                     ax.fill(x, y1, color = rndColor)
                     ax.fill(x, y2, color = rndColor)
-                    ax.plot([m, m], [bottom, top], linewidth = 2, color = rndColor)
+                    ax.plot([m, m], [bottom, top], linewidth = pinWidth, color = rndColor)
                 if (labelFlag == True):
                     ax.annotate(g['desc'], (m, top + 0.15))
 
+    # Show time span ==========================================================
+    if (showTail):
+        xTicks = list(ax.get_xticks())
+        xTicks.append(realEnd)
+        ax.set_xticks(xTicks)
+
+    # Fix height if fig, ax are not provided ==================================
+    if (fig == None or ax == None):
+        fig.set_figheight(5 * len(entities))
+
     # Save figure =============================================================
     if (saveFigPath != None):
         fig.savefig(saveFigPath)
 
     return fig, ax
 
 def plotNodes(
```

### Comparing `vrpSolver-0.0.8/vrpSolver/shortestPath.py` & `vrpSolver-0.0.9/vrpSolver/shortestPath.py`

 * *Files identical despite different names*

### Comparing `vrpSolver-0.0.8/vrpSolver/timeWindows.py` & `vrpSolver-0.0.9/vrpSolver/timeWindows.py`

 * *Files 17% similar despite different names*

```diff
@@ -32,14 +32,87 @@
     # Check overlapping again =================================================
     for i in range(len(sortedTW) - 1):
         if (sortedTW[i][1] > sortedTW[i + 1][0]):
             return None 
 
     return sortedTW
 
+def mergeTimeWindows(
+    tws:        "List of time windows, might be overlapping" = None,
+    ) -> "Given a list of time windows, which might be overlapping, merge the time windows that are overlapping":
+
+    # Initialize ==============================================================
+    mergedTWs = []
+
+    # Merge tws ===============================================================
+    for tw in tws:
+        # Find the index of tw that involves the s/e of tw, if there is any
+        sIndex = None
+        eIndex = None
+        for bgTwIndex in range(len(mergedTWs)):
+            if (insideInterval(tw[0], mergedTWs[bgTwIndex])):
+                sIndex = bgTwIndex
+            if (insideInterval(tw[1], mergedTWs[bgTwIndex])):
+                eIndex = bgTwIndex
+            if (sIndex != None and eIndex != None):
+                break
+        # Find the s/e of merged tw
+        ts = None
+        te = None
+        if (sIndex != None):
+            ts = mergedTWs[sIndex][0]
+        else:
+            ts = tw[0]
+        if (eIndex != None):
+            te = mergedTWs[eIndex][1]
+        else:
+            te = tw[1]
+        mergedTWs.append([ts, te])
+
+        # Remove the tws that partially covered by [ts, te], remove them
+        tmpMergedTWs = [i for i in mergedTWs]
+        mergedTWs = [[ts, te]] # merged tw should be included
+        for newTW in tmpMergedTWs:
+            # For existed tws, both s and e should not inside the [ts, te]
+            if (not insideInterval(newTW[0], [ts, te]) and not insideInterval(newTW[1], [ts, te])):
+                mergedTWs.append(newTW)
+        
+        # Sort tws
+        mergedTWs = sortTimeWindows(mergedTWs)
+
+    return mergedTWs
+
+def lenTWOverlap(
+    tw1:        "The first time window" = None,
+    tw2:        "The second time window" = None
+    ) -> "Given two time windows, returns the length of time that these two time windows are overlapping":
+
+    # Initialize ==============================================================
+    overlapTime = 0
+
+    # Case by case ============================================================
+    if (not insideInterval(tw2[0], tw1) and not insideInterval(tw2[1], tw1)):
+        # Case 1: tw1 is entirely inside tw2
+        if (tw2[0] < tw1[0] and tw1[1] < tw2[1]):
+            overlapTime = tw1[1] - tw1[0]
+        # Case 2: No overlapping
+        else:
+            overlapTime = 0
+    elif (insideInterval(tw2[0], tw1) and not insideInterval(tw2[1], tw1)):
+        # Case 3: First half of tw2 is inside tw1
+        overlapTime = tw1[1] - tw2[0]
+    elif (not insideInterval(tw2[0], tw1) and insideInterval(tw2[1], tw1)):
+        # Case 4: Last half of tw2 is inside tw1
+        overlapTime = tw2[1] - tw[0]
+    else:
+        # Case 5: tw2 is entirely inside tw1
+        overlapTime = tw2[1] - tw2[0]
+
+    return overlapTime
+
 # [Done]
 def reverseTimeWindows(
     tws:        "List of existing time windows" = None,
     epoch:      "Another time window that we wanna find opposite time windows of `tws` inside `epoch`" = None
     ) -> "Given a list of time windows `tws`, given another time window `epoch`, returns the opposite time windows of `tws` in `epoch":
 
     # Initialize ==============================================================
@@ -49,15 +122,15 @@
     # Start with epoch, using `blockTimeWindows` to reverse time windows
     for tw in tws:
         oppTws = blockTimeWindows(oppTws, tw)
     return oppTws
 
 # [Done]
 def blockTimeWindows(
-    tws:        "List of existing time windows" = None,
+    tws:        "List of existing available time windows" = None,
     block:      "A piece of time make part of tws unavailable" = None,
     ) -> "Given a list of non-overlapping time windows, use a time window to block the existing `tws`":
     newTWs = []
     for tw in tws:
         # Use '<' in this section
         # Case 1: Block entirely inside the time window
         if (tw[0] < block[0] and block[1] < tw[1]):
@@ -103,14 +176,36 @@
             if (t < bgTws[i][0]):
                 if (earliestNext is None or earliestNext > bgTws[i][0]):
                     earliestNext = bgTws[i][0]
         else:
             return t
     return earliestNext
 
+def getAvailStartTW(
+    bgTws:      "List of non-overlapping time windows as background (CANNOT be covered by inserting time window)" = None,
+    epoch:      "The outer epoch of `bgTws` time windows" = None,
+    twLen:      "Length of time window that trying to add into bgTws (within epoch)" = None
+    ) -> "Given a list of background time windows and an outer epoch, given the length of a new time window, \
+          return a list of time windows that can start the tw with the length of `twLen`":
+
+    # Initialize ==============================================================
+    startTws = []
+
+    # Get the list of time windows that can insert new time window ============
+    availTws = reverseTimeWindows(bgTws, epoch)
+    print(availTws)
+
+    # For each available time windows, try to see if it is long enough ========
+    for tw in availTws:
+        bgTwLen = tw[1] - tw[0]
+        if (bgTwLen >= twLen):
+            startTws.append([tw[0], tw[0] + (bgTwLen - twLen)])
+
+    return startTws
+
 # [Done] NOTICE: this is for sorted and non-overlapping time windows
 def getTWInsertFlexibility(
     bgTws:      "List of non-overlapping time windows as background (CANNOT be covered by inserting time window)" = None,
     epoch:      "The outer epoch of `bgTws` time windows" = None,
     tw:         "The time windows to be inserted" = None,
     tdRange:    "This is for time-dependent tw, which is the time that the tw can move advance/delay without \
                  changing length. Also, tdRange[0] <= 0 and tdRange[1] >= 0" = [None, None]
@@ -192,7 +287,8 @@
                         minAdvanceNeeded = tw[1] - gap[1]
 
         return {
             'canInsertFlag': False,
             'minAdvanceNeeded': minAdvanceNeeded,
             'minDelayNeeded': minDelayNeeded
         }
+
```

### Comparing `vrpSolver-0.0.8/vrpSolver/traversal.py` & `vrpSolver-0.0.9/vrpSolver/traversal.py`

 * *Files identical despite different names*

### Comparing `vrpSolver-0.0.8/vrpSolver.egg-info/PKG-INFO` & `vrpSolver-0.0.9/vrpSolver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vrpSolver
-Version: 0.0.8
+Version: 0.0.9
 Summary: VRP Solver
 Home-page: https://github.com/isaac0821/vrpSolver
 Author: Lan Peng
 Author-email: lanpeng@buffalo.edu
 License: MIT
 Download-URL: https://github.com/isaac0821/vrpSolver
 Project-URL: Bug Tracker, https://github.com/isaac0821/vrpSolver/issues
```

