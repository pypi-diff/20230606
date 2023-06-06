# Comparing `tmp/bas_geoplot-0.0.17.tar.gz` & `tmp/bas_geoplot-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bas_geoplot-0.0.17.tar", last modified: Wed Apr 19 10:35:43 2023, max compression
+gzip compressed data, was "bas_geoplot-0.0.19.tar", last modified: Tue Jun  6 12:54:58 2023, max compression
```

## Comparing `bas_geoplot-0.0.17.tar` & `bas_geoplot-0.0.19.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-04-19 10:35:43.945830 bas_geoplot-0.0.17/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1081 2022-10-25 08:33:04.000000 bas_geoplot-0.0.17/LICENSE
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       92 2022-10-21 13:21:48.000000 bas_geoplot-0.0.17/MANIFEST.in
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2905 2023-04-19 10:35:43.949830 bas_geoplot-0.0.17/PKG-INFO
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2004 2022-10-21 13:21:48.000000 bas_geoplot-0.0.17/README.md
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-04-19 10:35:43.945830 bas_geoplot-0.0.17/bas_geoplot/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      194 2023-04-04 13:22:34.000000 bas_geoplot-0.0.17/bas_geoplot/__init__.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     4821 2023-04-19 10:35:00.000000 bas_geoplot-0.0.17/bas_geoplot/cli.py
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-04-19 10:35:43.945830 bas_geoplot-0.0.17/bas_geoplot/config/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     7165 2023-02-23 13:19:23.000000 bas_geoplot-0.0.17/bas_geoplot/config/interactive.json
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     4536 2023-01-24 13:37:08.000000 bas_geoplot-0.0.17/bas_geoplot/config/static.json
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    34647 2023-04-19 10:35:00.000000 bas_geoplot-0.0.17/bas_geoplot/interactive.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     9658 2022-10-21 13:21:48.000000 bas_geoplot-0.0.17/bas_geoplot/static.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2201 2022-10-21 13:21:48.000000 bas_geoplot-0.0.17/bas_geoplot/utils.py
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-04-19 10:35:43.945830 bas_geoplot-0.0.17/bas_geoplot.egg-info/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2905 2023-04-19 10:35:43.000000 bas_geoplot-0.0.17/bas_geoplot.egg-info/PKG-INFO
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      474 2023-04-19 10:35:43.000000 bas_geoplot-0.0.17/bas_geoplot.egg-info/SOURCES.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2023-04-19 10:35:43.000000 bas_geoplot-0.0.17/bas_geoplot.egg-info/dependency_links.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       61 2023-04-19 10:35:43.000000 bas_geoplot-0.0.17/bas_geoplot.egg-info/entry_points.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2022-10-21 13:36:47.000000 bas_geoplot-0.0.17/bas_geoplot.egg-info/not-zip-safe
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       71 2023-04-19 10:35:43.000000 bas_geoplot-0.0.17/bas_geoplot.egg-info/requires.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       12 2023-04-19 10:35:43.000000 bas_geoplot-0.0.17/bas_geoplot.egg-info/top_level.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      107 2023-04-19 10:35:43.949830 bas_geoplot-0.0.17/setup.cfg
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1540 2022-10-21 13:21:48.000000 bas_geoplot-0.0.17/setup.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-06-06 12:54:58.415331 bas_geoplot-0.0.19/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1081 2022-10-25 08:33:04.000000 bas_geoplot-0.0.19/LICENSE
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       92 2022-10-21 13:21:48.000000 bas_geoplot-0.0.19/MANIFEST.in
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2905 2023-06-06 12:54:58.415331 bas_geoplot-0.0.19/PKG-INFO
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2004 2022-10-21 13:21:48.000000 bas_geoplot-0.0.19/README.md
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-06-06 12:54:58.411331 bas_geoplot-0.0.19/bas_geoplot/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      194 2023-06-06 12:52:13.000000 bas_geoplot-0.0.19/bas_geoplot/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     5358 2023-06-06 12:53:52.000000 bas_geoplot-0.0.19/bas_geoplot/cli.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-06-06 12:54:58.415331 bas_geoplot-0.0.19/bas_geoplot/config/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     7342 2023-04-20 13:24:57.000000 bas_geoplot-0.0.19/bas_geoplot/config/interactive.json
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     4536 2023-01-24 13:37:08.000000 bas_geoplot-0.0.19/bas_geoplot/config/static.json
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    34748 2023-06-06 12:52:13.000000 bas_geoplot-0.0.19/bas_geoplot/interactive.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     9658 2022-10-21 13:21:48.000000 bas_geoplot-0.0.19/bas_geoplot/static.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2201 2022-10-21 13:21:48.000000 bas_geoplot-0.0.19/bas_geoplot/utils.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-06-06 12:54:58.415331 bas_geoplot-0.0.19/bas_geoplot.egg-info/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2905 2023-06-06 12:54:58.000000 bas_geoplot-0.0.19/bas_geoplot.egg-info/PKG-INFO
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      474 2023-06-06 12:54:58.000000 bas_geoplot-0.0.19/bas_geoplot.egg-info/SOURCES.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2023-06-06 12:54:58.000000 bas_geoplot-0.0.19/bas_geoplot.egg-info/dependency_links.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       61 2023-06-06 12:54:58.000000 bas_geoplot-0.0.19/bas_geoplot.egg-info/entry_points.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2022-10-21 13:36:47.000000 bas_geoplot-0.0.19/bas_geoplot.egg-info/not-zip-safe
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       71 2023-06-06 12:54:58.000000 bas_geoplot-0.0.19/bas_geoplot.egg-info/requires.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       12 2023-06-06 12:54:58.000000 bas_geoplot-0.0.19/bas_geoplot.egg-info/top_level.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      107 2023-06-06 12:54:58.415331 bas_geoplot-0.0.19/setup.cfg
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1540 2022-10-21 13:21:48.000000 bas_geoplot-0.0.19/setup.py
```

### Comparing `bas_geoplot-0.0.17/LICENSE` & `bas_geoplot-0.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `bas_geoplot-0.0.17/PKG-INFO` & `bas_geoplot-0.0.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bas_geoplot
-Version: 0.0.17
+Version: 0.0.19
 Summary: GeoPlot: BAS AI Lab plotting scripts built on Folium
 Home-page: https://github.com/antarctica/GeoPlot
 Author: BAS AI Lab
 Author-email: jonsmi@bas.ac.uk
 Maintainer: BAS AI Lab
 Maintainer-email: jonsmi@bas.ac.uk
 License: UNKNOWN
```

### Comparing `bas_geoplot-0.0.17/README.md` & `bas_geoplot-0.0.19/README.md`

 * *Files identical despite different names*

### Comparing `bas_geoplot-0.0.17/bas_geoplot/cli.py` & `bas_geoplot-0.0.19/bas_geoplot/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 import argparse
 import json
 import inspect
 import logging
 import numpy as np
+import pandas as pd
 
 from bas_geoplot import __version__ as version
 from bas_geoplot.utils import setup_logging, timed_call
+from bas_geoplot.interactive import Map
+
 
 @setup_logging
 def get_args(default_output: str):
     ap = argparse.ArgumentParser()
     ap.add_argument("-o", "--output",default=default_output,help="Output file")
     ap.add_argument("-v", "--verbose",default=False,action="store_true",help="Turn on DEBUG level logging")
     ap.add_argument("-s", "--static",default=False,action="store_true",help="Save the plot as a static .PNG")           
     ap.add_argument("-c", "--currents_paths",default='',help="Path to currents file")
     ap.add_argument("-l", "--coastlines",default='',help="Loading Offline Coastlines")
     ap.add_argument("-j", "--offline_filepath",default='',help="Location of Offline File Information")
-    ap.add_argument("-p", "--plot_sectors",default=False,action="store_true",help="Plot array values as separate polygons")
+    ap.add_argument("-p", "--plot_sectors",default=False,action="store_true",
+                    help="Plot array values as separate polygons")
     ap.add_argument("mesh", type=argparse.FileType('r'),help="file location of mesh to be plot")
+    ap.add_argument('--version', action='version',
+                    version='%(prog)s {version}'.format(version=version))
+    ap.add_argument("-t", "--rm_titlebar",default=False, action="store_true", help="Remove titlebar from html")
+
     return ap.parse_args()
 
 @timed_call
 def plot_mesh_cli():
-    from bas_geoplot.interactive import Map
-    import pandas as pd
 
     args = get_args("interactive_plot.html")
     logging.info("{} {}".format(inspect.stack()[0][3][:-4], version))
     info = json.load(args.mesh)
     mesh = pd.DataFrame(info['cellboxes'])
     region = info['config']['Mesh_info']['Region']
 
-    output = ' '.join(args.output.split('/')[-1].split('.')[:-1])
-    output = '{} | Start Date: {}, End Date: {}'.format(output, region['startTime'], region['endTime'])
+    if args.rm_titlebar:
+        output = None
+    else:
+        output = ' '.join(args.output.split('/')[-1].split('.')[:-1])
+        output = '{} | Start Date: {}, End Date: {}'.format(output, region['startTime'], region['endTime'])
 
     mesh_bounds = [[region["latMin"], region["longMin"]], [region["latMax"], region["longMax"]]]
 
 
     if args.offline_filepath != '':
         logging.debug("offline .js & .css datastore - {}".format(args.offline_filepath))
         if args.coastlines != '':
@@ -71,14 +80,18 @@
         logging.debug('plotting currents')
         if args.currents_paths != '':
             logging.debug('plotting currents from file')
             currents = pd.read_csv(args.currents_paths)
             currents = currents[(currents['cx'] >=  info['config']['Mesh_info']['Region']['longMin']) & (currents['cx'] <=  info['config']['Mesh_info']['Region']['longMax']) & (currents['cy'] >=  info['config']['Mesh_info']['Region']['latMin']) & (currents['cy'] <=  info['config']['Mesh_info']['Region']['latMax'] )].reset_index(drop=True)
             mp.Vectors(currents,'Currents - Raw Data', show=False, predefined='Currents')
         mp.Vectors(mesh,'Currents - Mesh', show=False, predefined='Currents')
+    if ('u10' in mesh.columns) and ('v10' in mesh.columns):
+        mesh['mW'] = np.sqrt(mesh['u10'] ** 2 + mesh['v10'] ** 2)
+        mp.Vectors(mesh, 'Winds', predefined='Winds')
+        logging.debug('plotting winds')
 
     if 'paths' in info.keys():
         logging.debug('plotting paths')
         paths = info['paths']
         mp.Paths(paths,'Routes - Traveltimes',predefined='Traveltime (Days)')
         mp.Paths(paths,'Routes - Distance',predefined='Distance (Nautical miles)',show=False)
         mp.Paths(paths,'Routes - Max Speed',predefined='Max Speed (knots)',show=False)
```

### Comparing `bas_geoplot-0.0.17/bas_geoplot/config/interactive.json` & `bas_geoplot-0.0.19/bas_geoplot/config/interactive.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9968487394957982%*

 * *Differences: {"'MeshInfo'": "{'PolarRoute': {'fields': {insert: [(7, OrderedDict([('Name', 'Wind Magnitude "*

 * *               "(m/s)'), ('data', 'mW')])), (8, OrderedDict([('Name', 'Wind Component X (m/s)'), "*

 * *               "('data', 'u10')])), (9, OrderedDict([('Name', 'Wind Component Y (m/s)'), ('data', "*

 * *               "'v10')]))]}}}"}*

```diff
@@ -145,14 +145,26 @@
                     "data": "uC"
                 },
                 {
                     "Name": "Current Component Y (m/s)",
                     "data": "vC"
                 },
                 {
+                    "Name": "Wind Magnitude (m/s)",
+                    "data": "mW"
+                },
+                {
+                    "Name": "Wind Component X (m/s)",
+                    "data": "u10"
+                },
+                {
+                    "Name": "Wind Component Y (m/s)",
+                    "data": "v10"
+                },
+                {
                     "Name": "Minimum Depth (m)",
                     "data": "elevation",
                     "scaling_factor": -1
                 },
                 {
                     "Name": "Ice Resistance (kN)",
                     "data": "ice resistance",
```

### Comparing `bas_geoplot-0.0.17/bas_geoplot/config/static.json` & `bas_geoplot-0.0.19/bas_geoplot/config/static.json`

 * *Files identical despite different names*

### Comparing `bas_geoplot-0.0.17/bas_geoplot/interactive.py` & `bas_geoplot-0.0.19/bas_geoplot/interactive.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
             folium.GeoJson(antarctica,
                     style_function=lambda feature: {
                         'color': 'black',
                         'weight': 0.5,
                     }, name="geojson").add_to(bsmap)
             bsmap.add_to(self.map)
 
-        if p['plot_title']:
+        if (p['plot_title']) and (p['title'] is not None):
             self.map.get_root().html.add_child(folium.Element(title_html))
 
 
     def _layer(self,name,show=False):
         if name not in self._layer_info:
             lyr = folium.FeatureGroup(name='{}'.format(name),show=show)
             self._layer_info[name] = lyr
@@ -511,15 +511,16 @@
                     config/interactive.json of the package files
         """
 
 
         p = paramsObject('Vectors',predefined=predefined,**kwargs)
 
         Vectors = mesh
-        Vectors = Vectors[(Vectors[p['V']]!=0.0)&(Vectors[p['U']]!=0.0)].reset_index(drop=True)
+        # Filter out empty vectors but allow single component vectors
+        Vectors = Vectors[(Vectors[p['V']]!=0.0)|(Vectors[p['U']]!=0.0)].reset_index(drop=True)
         Vectors = Vectors.dropna(subset=[p['U'], p['V']]).reset_index(drop=True)
 
         if 'land' in Vectors.keys():
             Vectors = Vectors[Vectors['land']==False].reset_index(drop=True)
 
         vcts = self._layer(name,show=show)
         for idx,vec in Vectors.iterrows():
```

### Comparing `bas_geoplot-0.0.17/bas_geoplot/static.py` & `bas_geoplot-0.0.19/bas_geoplot/static.py`

 * *Files identical despite different names*

### Comparing `bas_geoplot-0.0.17/bas_geoplot/utils.py` & `bas_geoplot-0.0.19/bas_geoplot/utils.py`

 * *Files identical despite different names*

### Comparing `bas_geoplot-0.0.17/bas_geoplot.egg-info/PKG-INFO` & `bas_geoplot-0.0.19/bas_geoplot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bas-geoplot
-Version: 0.0.17
+Version: 0.0.19
 Summary: GeoPlot: BAS AI Lab plotting scripts built on Folium
 Home-page: https://github.com/antarctica/GeoPlot
 Author: BAS AI Lab
 Author-email: jonsmi@bas.ac.uk
 Maintainer: BAS AI Lab
 Maintainer-email: jonsmi@bas.ac.uk
 License: UNKNOWN
```

### Comparing `bas_geoplot-0.0.17/setup.py` & `bas_geoplot-0.0.19/setup.py`

 * *Files identical despite different names*

