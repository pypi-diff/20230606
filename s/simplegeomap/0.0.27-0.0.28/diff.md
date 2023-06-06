# Comparing `tmp/simplegeomap-0.0.27.tar.gz` & `tmp/simplegeomap-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/simplegeomap-0.0.27.tar", last modified: Thu Jun  1 06:36:19 2023, max compression
+gzip compressed data, was "dist/simplegeomap-0.0.28.tar", last modified: Tue Jun  6 06:14:38 2023, max compression
```

## Comparing `simplegeomap-0.0.27.tar` & `simplegeomap-0.0.28.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-06-01 06:36:19.000000 simplegeomap-0.0.27/
--rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-06-01 06:36:19.000000 simplegeomap-0.0.27/PKG-INFO
--rw-rw-r--   0 burak     (1000) burak     (1000)     2189 2023-01-06 09:35:10.000000 simplegeomap-0.0.27/README.md
-drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-06-01 06:36:19.000000 simplegeomap-0.0.27/simplegeomap.egg-info/
--rw-rw-r--   0 burak     (1000) burak     (1000)        1 2023-06-01 06:36:18.000000 simplegeomap-0.0.27/simplegeomap.egg-info/dependency_links.txt
--rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-06-01 06:36:18.000000 simplegeomap-0.0.27/simplegeomap.egg-info/PKG-INFO
--rw-rw-r--   0 burak     (1000) burak     (1000)       13 2023-06-01 06:36:18.000000 simplegeomap-0.0.27/simplegeomap.egg-info/top_level.txt
--rw-rw-r--   0 burak     (1000) burak     (1000)       51 2023-06-01 06:36:18.000000 simplegeomap-0.0.27/simplegeomap.egg-info/requires.txt
--rw-rw-r--   0 burak     (1000) burak     (1000)      272 2023-06-01 06:36:18.000000 simplegeomap-0.0.27/simplegeomap.egg-info/SOURCES.txt
-drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-06-01 06:36:19.000000 simplegeomap-0.0.27/simplegeomap/
--rw-rw-r--   0 burak     (1000) burak     (1000)       28 2023-02-11 07:38:13.000000 simplegeomap-0.0.27/simplegeomap/__init__.py
--rw-rw-r--   0 burak     (1000) burak     (1000)     6876 2023-05-31 12:04:11.000000 simplegeomap-0.0.27/simplegeomap/simplegeomap.py
--rw-rw-r--   0 burak     (1000) burak     (1000)     6386 2023-05-31 11:57:38.000000 simplegeomap-0.0.27/simplegeomap/util.py
--rw-rw-r--   0 burak     (1000) burak     (1000)      626 2023-06-01 06:34:42.000000 simplegeomap-0.0.27/setup.py
--rw-rw-r--   0 burak     (1000) burak     (1000)       38 2023-06-01 06:36:19.000000 simplegeomap-0.0.27/setup.cfg
+drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-06-06 06:14:38.000000 simplegeomap-0.0.28/
+-rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-06-06 06:14:38.000000 simplegeomap-0.0.28/PKG-INFO
+-rw-rw-r--   0 burak     (1000) burak     (1000)     2189 2023-01-06 09:35:10.000000 simplegeomap-0.0.28/README.md
+drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-06-06 06:14:38.000000 simplegeomap-0.0.28/simplegeomap.egg-info/
+-rw-rw-r--   0 burak     (1000) burak     (1000)        1 2023-06-06 06:14:38.000000 simplegeomap-0.0.28/simplegeomap.egg-info/dependency_links.txt
+-rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-06-06 06:14:38.000000 simplegeomap-0.0.28/simplegeomap.egg-info/PKG-INFO
+-rw-rw-r--   0 burak     (1000) burak     (1000)       13 2023-06-06 06:14:38.000000 simplegeomap-0.0.28/simplegeomap.egg-info/top_level.txt
+-rw-rw-r--   0 burak     (1000) burak     (1000)       45 2023-06-06 06:14:38.000000 simplegeomap-0.0.28/simplegeomap.egg-info/requires.txt
+-rw-rw-r--   0 burak     (1000) burak     (1000)      272 2023-06-06 06:14:38.000000 simplegeomap-0.0.28/simplegeomap.egg-info/SOURCES.txt
+drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-06-06 06:14:38.000000 simplegeomap-0.0.28/simplegeomap/
+-rw-rw-r--   0 burak     (1000) burak     (1000)       28 2023-02-11 07:38:13.000000 simplegeomap-0.0.28/simplegeomap/__init__.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)     7699 2023-06-06 06:11:05.000000 simplegeomap-0.0.28/simplegeomap/simplegeomap.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)     6386 2023-05-31 11:57:38.000000 simplegeomap-0.0.28/simplegeomap/util.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)      618 2023-06-06 06:13:01.000000 simplegeomap-0.0.28/setup.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)       38 2023-06-06 06:14:38.000000 simplegeomap-0.0.28/setup.cfg
```

### Comparing `simplegeomap-0.0.27/PKG-INFO` & `simplegeomap-0.0.28/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplegeomap
-Version: 0.0.27
+Version: 0.0.28
 Summary: Simple offline map plot utility, for country borders, elevation, water
 Home-page: https://github.com/burakbayramli/simplegeomap
 Author: Burak Bayramli
 License: UNKNOWN
 Description: # SimpleGeoMap
         
         Given a center latitude, longitude and a zoom level simply plot all
```

### Comparing `simplegeomap-0.0.27/README.md` & `simplegeomap-0.0.28/README.md`

 * *Files identical despite different names*

### Comparing `simplegeomap-0.0.27/simplegeomap.egg-info/PKG-INFO` & `simplegeomap-0.0.28/simplegeomap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplegeomap
-Version: 0.0.27
+Version: 0.0.28
 Summary: Simple offline map plot utility, for country borders, elevation, water
 Home-page: https://github.com/burakbayramli/simplegeomap
 Author: Burak Bayramli
 License: UNKNOWN
 Description: # SimpleGeoMap
         
         Given a center latitude, longitude and a zoom level simply plot all
```

### Comparing `simplegeomap-0.0.27/simplegeomap/simplegeomap.py` & `simplegeomap-0.0.28/simplegeomap/simplegeomap.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,14 +60,37 @@
             if geo.shape[0] > 0:
                 if iso3 in country_color: 
                     ax.fill(geo[:,0],geo[:,1],country_color[iso3],alpha=0.5)
                 else:
                     ax.fill(geo[:,0],geo[:,1],incolor,alpha=0.5)
                 ax.plot(geo[:,0],geo[:,1],'b')
 
+def plot_continents(clat,clon,zoom=7,incolor='lightyellow',outcolor='lightblue',len_thres=10,ax=None):
+    if not ax: fig, ax = plt.subplots()
+    data_dir = os.path.dirname(__file__)
+    zip_file    = zipfile.ZipFile(data_dir + "/continents.zip")
+    fin  = zip_file.open('continents.json')
+    res = json.loads(fin.read())
+
+    MAX = 20    
+    CENTER_DIST = (40000. / MAX)*(zoom+1)
+    xlims = (clon+(-180./MAX)*zoom, clon+(180./MAX)*zoom)
+    ylims = (clat+(-90./MAX)*zoom, clat+(90./MAX)*zoom)
+    
+    ax.set_facecolor(color=outcolor)
+    ax.set_xlim(xlims)
+    ax.set_ylim(ylims)
+    
+    for i in range(8):
+        for x in res['features'][i]['geometry']['coordinates']:
+            if len(x[0]) > len_thres:
+                arr = np.array(x[0])
+                ax.fill(arr[:,0],arr[:,1],incolor)
+
+                
 def create_grid(clat,clon,dist):    
     p1 = LatLon(clat,clon)
     EARTH_RAD = 6371
     upright = p1.destination (dist, bearing=45, radius=EARTH_RAD)
     lowleft = p1.destination (dist, bearing=225, radius=EARTH_RAD)
 
     minlat = np.min([upright.lat,lowleft.lat])
```

### Comparing `simplegeomap-0.0.27/simplegeomap/util.py` & `simplegeomap-0.0.28/simplegeomap/util.py`

 * *Files identical despite different names*

### Comparing `simplegeomap-0.0.27/setup.py` & `simplegeomap-0.0.28/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 readme=open("README.md").read()
 
 setuptools.setup(
     name='simplegeomap',    
-    version='0.0.27',
+    version='0.0.28',
     description="Simple offline map plot utility, for country borders, elevation, water",
     long_description=readme,
     long_description_content_type="text/markdown",    
-    install_requires=['pandas','pygeodesy','matplotlib','numpy','pyshp','scipy','zarr'],
+    install_requires=['pandas','pygeodesy','matplotlib','numpy','pyshp','zarr'],
     include_package_data=True,
     url="https://github.com/burakbayramli/simplegeomap",
     author="Burak Bayramli",
     package_data={
         "": ["*.dbf", "*.shp","*.zip","*.npz","*.csv"]
     },
     packages=setuptools.find_packages(),
```

