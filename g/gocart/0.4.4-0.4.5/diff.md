# Comparing `tmp/gocart-0.4.4.tar.gz` & `tmp/gocart-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gocart-0.4.4.tar", last modified: Thu Jun  1 14:47:57 2023, max compression
+gzip compressed data, was "gocart-0.4.5.tar", last modified: Tue Jun  6 15:31:31 2023, max compression
```

## Comparing `gocart-0.4.4.tar` & `gocart-0.4.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-01 14:47:57.772820 gocart-0.4.4/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3841 2023-06-01 14:43:19.000000 gocart-0.4.4/CHANGES.md
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2023-06-01 14:43:19.000000 gocart-0.4.4/LICENSE
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      377 2023-06-01 14:43:19.000000 gocart-0.4.4/MANIFEST.in
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6460 2023-06-01 14:47:57.772820 gocart-0.4.4/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5894 2023-06-01 14:43:19.000000 gocart-0.4.4/README.md
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-01 14:47:57.768820 gocart-0.4.4/gocart/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      189 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/__version__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      738 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/advanced_settings.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10717 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/cl_utils.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-01 14:47:57.772820 gocart-0.4.4/gocart/commonutils/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      157 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/commonutils/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4510 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/commonutils/flatten_healpix_map.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3054 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/commonutils/generate_skymap_stats.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      358 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/commonutils/getpackagepath.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-01 14:47:57.772820 gocart-0.4.4/gocart/convert/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      204 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/convert/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    12776 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/convert/aitoff.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3397 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/convert/ascii.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6489 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/convert/healpix2cart.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3096 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/default_settings.yaml
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-01 14:47:57.772820 gocart-0.4.4/gocart/parsers/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       56 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/parsers/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    16286 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/parsers/lvk.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-01 14:47:57.760819 gocart-0.4.4/gocart/resources/
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-01 14:47:57.772820 gocart-0.4.4/gocart/resources/plugins/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3124 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/resources/plugins/gp_template.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9654 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2891 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/test_settings.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3387 2023-06-01 14:43:19.000000 gocart-0.4.4/gocart/utKit.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-01 14:47:57.768820 gocart-0.4.4/gocart.egg-info/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6460 2023-06-01 14:47:57.000000 gocart-0.4.4/gocart.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      788 2023-06-01 14:47:57.000000 gocart-0.4.4/gocart.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-06-01 14:47:57.000000 gocart-0.4.4/gocart.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       48 2023-06-01 14:47:57.000000 gocart-0.4.4/gocart.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-06-01 14:46:48.000000 gocart-0.4.4/gocart.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      109 2023-06-01 14:47:57.000000 gocart-0.4.4/gocart.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        7 2023-06-01 14:47:57.000000 gocart-0.4.4/gocart.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2023-06-01 14:47:57.772820 gocart-0.4.4/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1915 2023-06-01 14:43:19.000000 gocart-0.4.4/setup.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-06 15:31:31.127103 gocart-0.4.5/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4516 2023-06-06 15:25:02.000000 gocart-0.4.5/CHANGES.md
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2023-06-06 15:25:02.000000 gocart-0.4.5/LICENSE
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      377 2023-06-06 15:25:02.000000 gocart-0.4.5/MANIFEST.in
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6460 2023-06-06 15:31:31.127103 gocart-0.4.5/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5894 2023-06-06 15:25:02.000000 gocart-0.4.5/README.md
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-06 15:31:31.107102 gocart-0.4.5/gocart/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      189 2023-06-06 15:25:02.000000 gocart-0.4.5/gocart/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2023-06-06 15:25:02.000000 gocart-0.4.5/gocart/__version__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      738 2023-06-06 15:25:02.000000 gocart-0.4.5/gocart/advanced_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10717 2023-06-06 15:25:02.000000 gocart-0.4.5/gocart/cl_utils.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-06 15:31:31.115102 gocart-0.4.5/gocart/commonutils/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      157 2023-06-06 15:25:02.000000 gocart-0.4.5/gocart/commonutils/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4510 2023-06-06 15:25:02.000000 gocart-0.4.5/gocart/commonutils/flatten_healpix_map.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3054 2023-06-06 15:25:02.000000 gocart-0.4.5/gocart/commonutils/generate_skymap_stats.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      358 2023-06-06 15:25:02.000000 gocart-0.4.5/gocart/commonutils/getpackagepath.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-06 15:31:31.123103 gocart-0.4.5/gocart/convert/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      204 2023-06-06 15:25:02.000000 gocart-0.4.5/gocart/convert/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    14318 2023-06-06 15:25:02.000000 gocart-0.4.5/gocart/convert/aitoff.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3397 2023-06-06 15:25:02.000000 gocart-0.4.5/gocart/convert/ascii.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6489 2023-06-06 15:25:02.000000 gocart-0.4.5/gocart/convert/healpix2cart.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3096 2023-06-06 15:25:02.000000 gocart-0.4.5/gocart/default_settings.yaml
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-06 15:31:31.123103 gocart-0.4.5/gocart/parsers/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       56 2023-06-06 15:25:02.000000 gocart-0.4.5/gocart/parsers/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    16347 2023-06-06 15:25:02.000000 gocart-0.4.5/gocart/parsers/lvk.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-06 15:31:31.095102 gocart-0.4.5/gocart/resources/
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-06 15:31:31.127103 gocart-0.4.5/gocart/resources/plugins/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3124 2023-06-06 15:25:03.000000 gocart-0.4.5/gocart/resources/plugins/gp_template.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9654 2023-06-06 15:25:03.000000 gocart-0.4.5/gocart/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2891 2023-06-06 15:25:03.000000 gocart-0.4.5/gocart/test_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3387 2023-06-06 15:25:03.000000 gocart-0.4.5/gocart/utKit.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-06 15:31:31.111102 gocart-0.4.5/gocart.egg-info/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6460 2023-06-06 15:31:30.000000 gocart-0.4.5/gocart.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      788 2023-06-06 15:31:30.000000 gocart-0.4.5/gocart.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-06-06 15:31:30.000000 gocart-0.4.5/gocart.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       48 2023-06-06 15:31:30.000000 gocart-0.4.5/gocart.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-06-06 15:29:38.000000 gocart-0.4.5/gocart.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      109 2023-06-06 15:31:30.000000 gocart-0.4.5/gocart.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        7 2023-06-06 15:31:30.000000 gocart-0.4.5/gocart.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2023-06-06 15:31:31.127103 gocart-0.4.5/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1915 2023-06-06 15:25:03.000000 gocart-0.4.5/setup.py
```

### Comparing `gocart-0.4.4/CHANGES.md` & `gocart-0.4.5/CHANGES.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 
 ## Release Notes
 
+**v0.4.5 - June 6, 2023**
+
+- **FEATURE**: added ability to plot square footprints on to the aitoff skymaps  
+- **ENHANCEMENT**: significance explicitly added to RHS sidebar of maps  
+- **REFACTOR**: colours of map contours adjusted to pastel colours  
+- **REFACTOR**: transparency of sun, moon, galactic plane adjusted for greater clarity  
+- **FIXED**: contours often getting tangled at the poles of the aitoff maps and rendering incorrectly. Solved by 'chunking' the filled contours with matplotlib  
+
 **v0.4.4 - June 1, 2023**
 
+- **REFACTOR**: `get_moon` has being depreciated in astropy, moving to get_body("moon")
+- **FIXED**: bilby now correctly reported as localisation on RHS of aitoff skymaps
 - **FIXED**: fix in prob calculations in flattened maps
 - **FIXED**: allowing symlinks in plugin folder
 
 **v0.4.2 - May 28, 2023**
 
 - **ENHANCEMENT**: added a `burst` filtering parameter. If set to True, burst event alerts will pass the filter, otherwise they filtered out (default).
 - **REFACTOR**: maps with `CREATOR: ligo-skymap-from-samples` now named on file as `bilby.multiorder.fits`.
```

### Comparing `gocart-0.4.4/LICENSE` & `gocart-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gocart-0.4.4/PKG-INFO` & `gocart-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: gocart
-Version: 0.4.4
+Version: 0.4.5
 Summary: Listen for, collect and convert multimessenger skymaps
 Home-page: https://github.com/thespacedoctor/gocart
-Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.4.4.zip
+Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.4.5.zip
 Author: David Young
 Author-email: d.r.young@qub.ac.uk
 License: MIT
 Keywords: astronomy
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `gocart-0.4.4/README.md` & `gocart-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `gocart-0.4.4/gocart/advanced_settings.yaml` & `gocart-0.4.5/gocart/advanced_settings.yaml`

 * *Files identical despite different names*

### Comparing `gocart-0.4.4/gocart/cl_utils.py` & `gocart-0.4.5/gocart/cl_utils.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.4/gocart/commonutils/flatten_healpix_map.py` & `gocart-0.4.5/gocart/commonutils/flatten_healpix_map.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.4/gocart/commonutils/generate_skymap_stats.py` & `gocart-0.4.5/gocart/commonutils/generate_skymap_stats.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.4/gocart/convert/aitoff.py` & `gocart-0.4.5/gocart/convert/aitoff.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 
     **Key Arguments:**
         - ``log`` -- logger
         - ``mapPath`` -- path to the multiorder FITS file
         - ``outputFolder`` -- path to output the results to
         - ``settings`` -- the settings dictionary
         - ``meta`` -- extra meta data to present on plots. Default: {}
+        - ``plotName`` -- the filename of the plot
+        - ``patches`` -- a patch collect to add to the plot
+        - ``patchesColor`` -- colour of the patches. Default '#859900'
+        - ``patchesLabel`` -- label for patches in the legend. Default None
 
     **Usage:**
 
     To setup your logger and settings, please use the ``fundamentals`` package (`see tutorial here <http://fundamentals.readthedocs.io/en/latest/#tutorial>`_).
 
     To print the healpix map as an aitoff projection, use the following:
 
@@ -46,22 +50,30 @@
 
     def __init__(
             self,
             log,
             mapPath,
             outputFolder,
             settings=False,
-            meta={}
+            meta={},
+            plotName="skymap.png",
+            patches=None,
+            patchesColor='#859900',
+            patchesLabel=None
     ):
         self.log = log
-        log.debug("instansiating a new 'aitoff' object")
+        log.debug("instantiating a new 'aitoff' object")
         self.settings = settings
         self.mapPath = mapPath
         self.outputFolder = outputFolder
         self.meta = meta
+        self.plotName = plotName
+        self.patches = patches
+        self.patchesColor = patchesColor
+        self.patchesLabel = patchesLabel
         # xt-self-arg-tmpx
 
         return None
 
     def convert(
         self,
         contours=True,
@@ -83,23 +95,25 @@
         """
         self.log.debug('starting the ``convert`` method')
 
         import matplotlib.pyplot as plt
         from . import healpix2cart
         import astropy.units as u
         import numpy as np
-        from astropy.coordinates import SkyCoord, Galactic, get_sun, get_moon
+        from astropy.coordinates import SkyCoord, Galactic, get_sun, get_body
         from matplotlib.projections.geo import GeoAxes
         from matplotlib.cm import get_cmap
         import matplotlib.patches as mpatches
         from matplotlib.lines import Line2D
         from astropy.time import Time
+        from matplotlib.collections import PatchCollection
 
         import matplotlib
-        matplotlib.use('PDF')
+        # matplotlib.use('PDF')
+        # plt.ion()
 
         class ThetaFormatterShiftPi(GeoAxes.ThetaFormatter):
             """SHIFTS LABELLING BY PI
             SHIFTS LABELLING FROM -180,180 TO 360-0"""
 
             def __call__(self, x, pos=None):
                 x -= np.pi
@@ -110,14 +124,17 @@
         converter = healpix2cart(
             log=self.log,
             mapPath=self.mapPath,
             settings=self.settings
         )
         wcs, mapDF, header = converter.convert()
 
+        # DROP MISSING VALUES
+        mapDF.dropna(axis='index', how='any', subset=['PROB'], inplace=True)
+
         xsize = mapDF["PIXEL_X"].max() - mapDF["PIXEL_X"].min() + 1
         ysize = mapDF["PIXEL_Y"].max() - mapDF["PIXEL_Y"].min() + 1
 
         # RA RANGES FROM 0-360 ... NEED TO FLIP 360-0, AND THEN SHIFT BY 180 TO MATCH MATPLOTLIB FRAME
         mapDF = mapDF.iloc[::-1].reset_index()
         mapDF["RASHIFTED"] = -mapDF["RA"] + 180
         data = mapDF["PROB"].values.reshape((ysize, xsize))
@@ -128,15 +145,15 @@
         # lat = mapDF["DEC"].values.reshape((ysize, xsize))
 
         # MATPLOTLIB IS DOING THE PROJECTION
         cmap = get_cmap("hot_r")
         fig = plt.figure()
 
         # AITOFF DOES NOT PLAY WELL WITH ADDING LABELS - USE HAMMER PROJECTION INSTEAD
-        ax = fig.add_subplot(111, projection='hammer')
+        ax = fig.add_subplot(111, projection='hammer', zorder=60)
 
         # RASTERIZED MAKES THE MAP BITMAP WHILE THE LABELS REMAIN VECTORIAL
         std = data.std()
         mean = data.mean()
         # image = ax.pcolormesh(long, lat, data, rasterized=False, cmap=cmap, vmin=mean, vmax=mean + 5 * std)
 
         # GRATICULE
@@ -164,19 +181,19 @@
             lats2 = np.linspace(-np.pi / 2, np.pi / 2, int(nlats))
             lons2, lats2 = np.meshgrid(lons2, lats2)
             sunlight = np.ones(lons2.shape)
             raSep = sun.ra.radian - lons2
             raSep[raSep > np.pi] = 2 * np.pi - raSep[raSep > np.pi]
             separation = ((raSep * np.cos((sun.dec.radian + lats2) / 2))**2 + (sun.dec.radian - lats2)**2)**0.5
             sunlight[separation < np.radians(33)] = 0
-            sunyellow = matplotlib.colors.colorConverter.to_rgba('#b58900', alpha=0.2)
-            ax.contourf(lons2, lats2, sunlight, 1, colors=[sunyellow, (0.0, 0.0, 0.0, 0.0)], zorder=3)
+            sunyellow = matplotlib.colors.colorConverter.to_rgba('#ffc202', alpha=0.15)
+            ax.contourf(lons2, lats2, sunlight, 1, colors=[sunyellow, (0.0, 0.0, 0.0, 0.0)], zorder=30)
 
             # PLOT THE MOON
-            moon = get_moon(t)
+            moon = get_body("moon", t)
             moon.ra.degree = -moon.ra.degree + 180
             if moon.ra.degree > 180.:
                 moon.ra.degree -= 360
             moon.ra.radian = np.deg2rad(moon.ra.degree)
 
             # COMPUTE LONS AND LATS OF DAY/NIGHT TERMINATOR.
             nlons = 1441
@@ -188,15 +205,15 @@
             lons2, lats2 = np.meshgrid(lons2, lats2)
             moonlight = np.ones(lons2.shape)
             raSep = moon.ra.radian - lons2
             raSep[raSep > np.pi] = 2 * np.pi - raSep[raSep > np.pi]
             separation = ((raSep * np.cos((moon.dec.radian + lats2) / 2))**2 + (moon.dec.radian - lats2)**2)**0.5
             moonlight[separation < np.radians(20)] = 0
             moonblue = matplotlib.colors.colorConverter.to_rgba('#268bd2', alpha=0.2)
-            ax.contourf(lons2, lats2, moonlight, 1, colors=[moonblue, (0.0, 0.0, 0.0, 0.0)], zorder=3)
+            ax.contourf(lons2, lats2, moonlight, 1, colors=[moonblue, (0.0, 0.0, 0.0, 0.0)], zorder=29)
 
         # PLOT THE SUN
         if sunmoon:
             t = Time(header['DATE-OBS'], scale='utc')
 
             # FIND SUN AND PLACE ON CORRECT PLOT COORDINATE
             sun = get_sun(t)
@@ -204,18 +221,18 @@
             if sun.ra.degree > 180.:
                 sun.ra.degree -= 360
             sun.ra.radian = np.deg2rad(sun.ra.degree)
 
             label = "Sun"
             if sunmoonContour:
                 label += " (within $33^o$)"
-            ax.scatter(sun.ra.radian, sun.dec.radian, color="#b58900", alpha=0.8, s=20, marker="o", edgecolors="#cb4b16", linewidths=0.5, label=label, zorder=30)
+            ax.scatter(sun.ra.radian, sun.dec.radian, color="#ffc202", alpha=0.8, s=20, marker="o", edgecolors="#cb4b16", linewidths=0.5, label=label, zorder=30)
 
             # PLOT THE MOON
-            moon = get_moon(t)
+            moon = get_body("moon", t)
             moon.ra.degree = -moon.ra.degree + 180
             if moon.ra.degree > 180.:
                 moon.ra.degree -= 360
             moon.ra.radian = np.deg2rad(moon.ra.degree)
 
             label = "Moon"
             if sunmoonContour:
@@ -237,34 +254,38 @@
             # SCALE CONVERSION TO [-180, 180] & FLIP RA
             ind = gx > 180
             gx[ind] -= 360
             gx = -gx
             planeColour = "#dc322f"
             ax.scatter(np.radians(gx), np.radians(gDec),
                        color=planeColour, alpha=1, s=1)
+            ax.scatter(np.radians(gx), np.radians(gDec),
+                       color=planeColour, alpha=0.1, s=1, zorder=30)
             line = Line2D([0], [0], label='Galactic Plane', color=planeColour)
             handles.append(line)
 
         if contours:
             mapDF.sort_values(["PROBDENSITY"],
                               ascending=[False], inplace=True)
             mapDF["CUMPROB"] = np.cumsum(mapDF['PROB'])
             mapDF["CUMPROB"] = mapDF["CUMPROB"] * 100. * mapDF["PROB"].sum()
+
             mapDF.sort_index(inplace=True)
+
             contours = mapDF["CUMPROB"].values.reshape((ysize, xsize))
 
-            colors = ['#474973', '#a69cac', '#03F7EB']
-            levels = [90, 50, 10]
+            colors = ['#a2a4c6', '#cdc2d3', '#8bfdf8']
+            levels = [90.0, 50.0, 10.0]
 
             z = 10
 
             for c, l in zip(colors, levels):
                 z += 1
                 ax.contourf(long, lat,
-                            contours, levels=[0, l], colors=c, zorder=z, alpha=0.8)
+                            contours, levels=[-1, l], colors=c, zorder=z, alpha=1., nchunk=10, antialiased=False)
                 if "EXTRA" in self.meta and f"area{l}" in self.meta["EXTRA"]:
                     area = self.meta["EXTRA"][f"area{l}"]
                     label = f"{l}%: {area:.1f} deg$^2$"
                 else:
                     label = f"{l}%"
                 patch = mpatches.Patch(color=c, label=label)
                 handles.append(patch)
@@ -272,14 +293,20 @@
         if len(self.meta):
             data = ""
             data += f"Event: {self.meta['ALERT']['superevent_id']} ({self.meta['ALERT']['event']['group']})\n"
             eventDate = Time(self.meta['HEADER']['DATE-OBS'], scale='utc').to_datetime().strftime("%Y-%m-%d %H:%M:%S")
             data += f"Event time: {eventDate}\n"
 
             data += "\n"
+            if "significant" in self.meta['ALERT']['event']:
+                if self.meta['ALERT']['event']["significant"]:
+                    data += f"Significance: HIGH\n"
+                else:
+                    data += f"Significance: LOW\n"
+
             data += f"Alert: {self.meta['ALERT']['alert_type'].replace('_',' ')}\n"
             alertDate = Time(self.meta['ALERT']['time_created'], scale='utc').to_datetime().strftime("%Y-%m-%d %H:%M:%S")
             data += f"Alert time: {alertDate}\n"
             instruments = (",").join(self.meta['ALERT']['event']['instruments'])
             data += f"Instruments: {instruments}\n"
             data += f"Localisation: {self.meta['HEADER']['CREATOR']}\n"
 
@@ -309,20 +336,29 @@
                 for k, v in self.meta['ALERT']['event']['properties'].items():
                     data += f"{k}: {v:.2f}\n"
 
             plt.text(3.42, 0.2, data, ha='left', va='top', fontsize=5, linespacing=1.8)
 
         # this = ax.clabel(line_c, inline=True, fontsize=6, colors=['#93a1a1'], fmt='{:.0f} '.format)
 
+        if self.patches:
+            ax.add_collection(PatchCollection(self.patches, alpha=0.4,
+                                              color=self.patchesColor, zorder=27))
+            if self.patchesLabel:
+                patch = mpatches.Patch(color=self.patchesColor, label=self.patchesLabel)
+                handles.append(patch)
+
         ax.tick_params(axis='x', labelsize=12)
         ax.tick_params(axis='y', labelsize=12)
-        ax.grid(color='#657b83', alpha=0.2, linestyle='dotted')
-        plt.grid(True)
+        ax.grid(color='#657b83', alpha=0.4, linestyle='dotted')
         plt.legend(handles=handles, loc='upper left', scatterpoints=1, bbox_to_anchor=(1.01, 1), fontsize=6)
         ax.xaxis.zorder = 40
+        ax.yaxis.zorder = 40
+
+        plt.grid(True)
 
-        plt.savefig(self.outputFolder + "/skymap.png", bbox_inches='tight', dpi=300)
+        plt.savefig(self.outputFolder + f"/{self.plotName}", bbox_inches='tight', dpi=300)
 
         plt.close()
 
         self.log.debug('completed the ``convert`` method')
         return None
```

### Comparing `gocart-0.4.4/gocart/convert/ascii.py` & `gocart-0.4.5/gocart/convert/ascii.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.4/gocart/convert/healpix2cart.py` & `gocart-0.4.5/gocart/convert/healpix2cart.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.4/gocart/default_settings.yaml` & `gocart-0.4.5/gocart/default_settings.yaml`

 * *Files identical despite different names*

### Comparing `gocart-0.4.4/gocart/parsers/lvk.py` & `gocart-0.4.5/gocart/parsers/lvk.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,14 +169,17 @@
             skymap_str = self.record.get('event', {}).pop('skymap')
 
             if skymap_str:
                 # Decode, parse skymap, and print most probable sky location
                 skymap_bytes = b64decode(skymap_str)
                 skymap = Table.read(BytesIO(skymap_bytes))
                 localisation = skymap.meta["CREATOR"].lower()
+                if localisation == "ligo-skymap-from-samples":
+                    skymap.meta["CREATOR"] = "bilby"
+                    localisation = "bilby"
                 header = {k: v for k, v in skymap.meta.items() if k != "HISTORY"}
                 # GENERATE SOME EXTRA STATS
                 extras = generate_skymap_stats(
                     log=self.log,
                     skymap=skymap,
                 )
 
@@ -221,16 +224,14 @@
             # DUMP JSON TO FILE
             writeFile = open(jsonPath, "w")
             json.dump(self.record, writeFile, indent=4)
             writeFile.close()
 
         # WRITE SKY MAP
         if localisation:
-            if localisation == "ligo-skymap-from-samples":
-                localisation = "bilby"
             fitsPath = f"{alertDir}/{localisation}.multiorder.fits"
             with open(fitsPath, "wb") as f:
                 f.write(skymap_bytes)
 
         # WRITE META
         with open(alertDir + "/meta.yaml", 'w') as stream:
             yaml.dump(meta, stream, default_flow_style=False)
```

### Comparing `gocart-0.4.4/gocart/resources/plugins/gp_template.py` & `gocart-0.4.5/gocart/resources/plugins/gp_template.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.4/gocart/setup.cfg` & `gocart-0.4.5/gocart/setup.cfg`

 * *Files identical despite different names*

### Comparing `gocart-0.4.4/gocart/test_settings.yaml` & `gocart-0.4.5/gocart/test_settings.yaml`

 * *Files identical despite different names*

### Comparing `gocart-0.4.4/gocart/utKit.py` & `gocart-0.4.5/gocart/utKit.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.4/gocart.egg-info/PKG-INFO` & `gocart-0.4.5/gocart.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: gocart
-Version: 0.4.4
+Version: 0.4.5
 Summary: Listen for, collect and convert multimessenger skymaps
 Home-page: https://github.com/thespacedoctor/gocart
-Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.4.4.zip
+Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.4.5.zip
 Author: David Young
 Author-email: d.r.young@qub.ac.uk
 License: MIT
 Keywords: astronomy
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `gocart-0.4.4/gocart.egg-info/SOURCES.txt` & `gocart-0.4.5/gocart.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gocart-0.4.4/setup.py` & `gocart-0.4.5/setup.py`

 * *Files identical despite different names*

