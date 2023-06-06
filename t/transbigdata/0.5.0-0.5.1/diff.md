# Comparing `tmp/transbigdata-0.5.0.tar.gz` & `tmp/transbigdata-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transbigdata-0.5.0.tar", last modified: Thu May 25 14:49:01 2023, max compression
+gzip compressed data, was "transbigdata-0.5.1.tar", last modified: Tue Jun  6 08:32:09 2023, max compression
```

## Comparing `transbigdata-0.5.0.tar` & `transbigdata-0.5.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:49:01.961894 transbigdata-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-25 14:48:50.000000 transbigdata-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-25 14:48:50.000000 transbigdata-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-05-25 14:49:01.961894 transbigdata-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13991 2023-05-25 14:48:50.000000 transbigdata-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 14:49:01.961894 transbigdata-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-25 14:48:51.000000 transbigdata-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:49:01.957894 transbigdata-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:49:01.961894 transbigdata-0.5.0/src/transbigdata/
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/bikedata.py
--rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/busgps.py
--rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    13711 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/gisprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    49157 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/grids.py
--rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/metro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/mobilephonedata.py
--rw-r--r--   0 runner    (1001) docker     (123)    10775 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/odprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    22191 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/plotmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     9447 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/taxigps.py
--rw-r--r--   0 runner    (1001) docker     (123)    31808 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/traj.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25655 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:49:01.961894 transbigdata-0.5.0/transbigdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-05-25 14:49:01.000000 transbigdata-0.5.0/transbigdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-25 14:49:01.000000 transbigdata-0.5.0/transbigdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:49:01.000000 transbigdata-0.5.0/transbigdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-25 14:49:01.000000 transbigdata-0.5.0/transbigdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 14:49:01.000000 transbigdata-0.5.0/transbigdata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:09.661062 transbigdata-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-06 08:31:56.000000 transbigdata-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-06 08:31:56.000000 transbigdata-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15249 2023-06-06 08:32:09.661062 transbigdata-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14372 2023-06-06 08:31:56.000000 transbigdata-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 08:32:09.661062 transbigdata-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-06 08:31:57.000000 transbigdata-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:09.653062 transbigdata-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:09.657062 transbigdata-0.5.1/src/transbigdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/bikedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14076 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/busgps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13711 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/gisprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49157 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/grids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/metro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/mobilephonedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10775 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/odprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22191 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/plotmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9447 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/taxigps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31846 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/traj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25663 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:09.657062 transbigdata-0.5.1/transbigdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15249 2023-06-06 08:32:09.000000 transbigdata-0.5.1/transbigdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-06 08:32:09.000000 transbigdata-0.5.1/transbigdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 08:32:09.000000 transbigdata-0.5.1/transbigdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-06 08:32:09.000000 transbigdata-0.5.1/transbigdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-06 08:32:09.000000 transbigdata-0.5.1/transbigdata.egg-info/top_level.txt
```

### Comparing `transbigdata-0.5.0/LICENSE` & `transbigdata-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.0/PKG-INFO` & `transbigdata-0.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transbigdata
-Version: 0.5.0
+Version: 0.5.1
 Summary: A Python package developed for transportation spatio-temporal big data processing and analysis.
 Home-page: https://github.com/ni1o1/transbigdata
 Author: Qing Yu
 Author-email: qingyu0815@foxmail.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/ni1o1/transbigdata/issues
 Classifier: Operating System :: OS Independent
@@ -345,13 +345,29 @@
 
 ![1648715064154.png](https://github.com/ni1o1/transbigdata/raw/main/image/README/1648715064154.png)
 
 See [This Example](https://github.com/ni1o1/transbigdata/blob/main/docs/source/gallery/Example%202-Grid-base%20processing%20framework%20of%20TransBigData.ipynb) for further details.
 
 ## Citation information [![DOI](https://zenodo.org/badge/419559811.svg)](https://zenodo.org/badge/latestdoi/419559811) [![status](https://joss.theoj.org/papers/d1055fe3105dfa2dcff4cb6c7688a79b/status.svg)](https://joss.theoj.org/papers/d1055fe3105dfa2dcff4cb6c7688a79b)
 
-Please cite [this](https://doi.org/10.21105/joss.04021) when using `TransBigData` in your research. Citation information can be found at [CITATION.cff](https://github.com/ni1o1/transbigdata/blob/main/CITATION.cff).
+Please cite [this](https://doi.org/10.21105/joss.04021) when using `TransBigData` in your research. Citation information is as follows:
+
+```bibtex
+@article{Yu2022,
+  doi       = {10.21105/joss.04021},
+  url       = {https://doi.org/10.21105/joss.04021},
+  year      = {2022},
+  publisher = {The Open Journal},
+  volume    = {7},
+  number    = {71},
+  pages     = {4021},
+  author    = {Qing Yu and Jian Yuan},
+  title     = {TransBigData: A Python package for transportation spatio-temporal big data processing, analysis and visualization},
+  journal   = {Journal of Open Source Software}
+}
+```
+
 
 ## Introducing Video (In Chinese) [![bilibili](https://img.shields.io/badge/bilibili-%E5%90%8C%E6%B5%8E%E5%B0%8F%E6%97%AD%E5%AD%A6%E9%95%BF-green.svg)](https://space.bilibili.com/3051484)
 
 * [Bilibili](https://www.bilibili.com/video/BV1na411i7sd/)
 * [Youtube](https://www.youtube.com/watch?v=ynqJ01WmPiQ)
```

### Comparing `transbigdata-0.5.0/README.md` & `transbigdata-0.5.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -323,13 +323,29 @@
 
 ![1648715064154.png](https://github.com/ni1o1/transbigdata/raw/main/image/README/1648715064154.png)
 
 See [This Example](https://github.com/ni1o1/transbigdata/blob/main/docs/source/gallery/Example%202-Grid-base%20processing%20framework%20of%20TransBigData.ipynb) for further details.
 
 ## Citation information [![DOI](https://zenodo.org/badge/419559811.svg)](https://zenodo.org/badge/latestdoi/419559811) [![status](https://joss.theoj.org/papers/d1055fe3105dfa2dcff4cb6c7688a79b/status.svg)](https://joss.theoj.org/papers/d1055fe3105dfa2dcff4cb6c7688a79b)
 
-Please cite [this](https://doi.org/10.21105/joss.04021) when using `TransBigData` in your research. Citation information can be found at [CITATION.cff](https://github.com/ni1o1/transbigdata/blob/main/CITATION.cff).
+Please cite [this](https://doi.org/10.21105/joss.04021) when using `TransBigData` in your research. Citation information is as follows:
+
+```bibtex
+@article{Yu2022,
+  doi       = {10.21105/joss.04021},
+  url       = {https://doi.org/10.21105/joss.04021},
+  year      = {2022},
+  publisher = {The Open Journal},
+  volume    = {7},
+  number    = {71},
+  pages     = {4021},
+  author    = {Qing Yu and Jian Yuan},
+  title     = {TransBigData: A Python package for transportation spatio-temporal big data processing, analysis and visualization},
+  journal   = {Journal of Open Source Software}
+}
+```
+
 
 ## Introducing Video (In Chinese) [![bilibili](https://img.shields.io/badge/bilibili-%E5%90%8C%E6%B5%8E%E5%B0%8F%E6%97%AD%E5%AD%A6%E9%95%BF-green.svg)](https://space.bilibili.com/3051484)
 
 * [Bilibili](https://www.bilibili.com/video/BV1na411i7sd/)
 * [Youtube](https://www.youtube.com/watch?v=ynqJ01WmPiQ)
```

### Comparing `transbigdata-0.5.0/setup.py` & `transbigdata-0.5.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="transbigdata",
-    version="0.5.0",
+    version="0.5.1",
     author="Qing Yu",
     author_email="qingyu0815@foxmail.com",
     description="A Python package developed for transportation spatio-temporal big data processing and analysis.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="BSD",
     url="https://github.com/ni1o1/transbigdata",
```

### Comparing `transbigdata-0.5.0/src/transbigdata/__init__.py` & `transbigdata-0.5.1/src/transbigdata/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 
-__version__ = '0.5.0'
+__version__ = '0.5.1'
 __author__ = 'Qing Yu <yuq@sustech.edu.cn>'
 
 # module level doc-string
 __doc__ = """
 TransBigData - A Python package develop for transportation spatio-temporal big
 data processing, analysis and visualization.
 =====================================================================
@@ -153,15 +153,15 @@
     traj_clean_redundant,
     traj_slice,
     traj_smooth,
     traj_segment,
     traj_densify,
     traj_sparsify,
     traj_stay_move,
-    points_to_traj,
+    traj_to_linestring,
 )
 
 from transbigdata.utils import (
     dumpjson
 )
 
 from transbigdata.quality import (
```

### Comparing `transbigdata-0.5.0/src/transbigdata/activity.py` & `transbigdata-0.5.1/src/transbigdata/activity.py`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.0/src/transbigdata/bikedata.py` & `transbigdata-0.5.1/src/transbigdata/bikedata.py`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.0/src/transbigdata/busgps.py` & `transbigdata-0.5.1/src/transbigdata/busgps.py`

 * *Files 21% similar despite different names*

```diff
@@ -40,18 +40,19 @@
     id_reindex
 )
 from .traj import(
     traj_clean_redundant
 )
 
 
+
 def busgps_arriveinfo(data, line, stop, col=[
         'VehicleId', 'GPSDateTime', 'lon', 'lat', 'stopname'],
-        stopbuffer=200, mintime=300, project_epsg=2416,
-        timegap=1800, method='project', projectoutput=False):
+        stopbuffer=200, mintime=300,    disgap = 200, project_epsg='auto',
+        timegap=1800,  projectoutput=False):
     '''
     Input bus GPS data, bus route and station GeoDataFrame, this
     method can identify the bus arrival and departure information
 
     Parameters
     -------
     data : DataFrame
@@ -67,163 +68,222 @@
         latitude, station name]
     stopbuffer : number
         Meter. When the vehicle approaches the station within this
         certain distance, it is considered to be arrive at the station.
     mintime : number
         Seconds. Within a short period of time that the bus arrive
         at bus station again, it will not be consider as another arrival
+    disgap : number
+        Meter. The distance between the front point and the back point
+        of the vehicle, which is used to determine whether the vehicle
+        is moving or not
     project_epsg : number
         The matching algorithm will convert the data into a projection
         coordinate system to calculate the distance, here the epsg code
         of the projection coordinate system is given
     timegap : number
         Seconds. For how long the vehicle does not appear, it will be
         considered as a new vehicle
-    method : str
-        The method of matching the bus, either ‘project’ or ‘dislimit’;
-        ‘project’ is to directly match the nearest point on the route,
-        which is fast. ‘dislimit’ needs to consider the front point position
-        with the distance limitation, the matching speed is slow.
     projectoutput : bool
         Whether to output the projected data
 
     Returns
     -------
     arrive_info : DataFrame
         Bus arrival and departure information
     '''
+    data = data.copy()
+    line = line.copy()
+    stop = stop.copy()
     VehicleId, GPSDateTime, lon, lat, stopcol = col
     # Clean data
     print('Cleaning data', end='')
-    line.set_crs(crs='epsg:4326', allow_override=True, inplace=True)
-    line = line.to_crs(epsg=project_epsg)
+
+    if project_epsg=='auto':
+        from pyproj import CRS
+        # 计算数据点的平均经纬度
+        meanlat = data[lat].mean()
+        meanlon = data[lon].mean()
+        project_epsg = CRS.from_proj4("+proj=aeqd +lat_0="+str(meanlat)+" +lon_0="+str(meanlon)+" +datum=WGS84")# 生成投影坐标系，等距方位投影
+
+    line.crs = {'init':'epsg:4326'}  
+    line = line.to_crs(project_epsg)
     line_buffer = line.copy()
     line_buffer['geometry'] = line_buffer.buffer(200)
     line_buffer = line_buffer.to_crs(epsg=4326)
     print('.', end='')
     data = traj_clean_redundant(data, col=[VehicleId, GPSDateTime, lon, lat])
     print('.', end='')
     data = clean_outofshape(data, line_buffer, col=[lon, lat], accuracy=500)
     print('.')
-    data = id_reindex(data, VehicleId, timegap=timegap,
-                      timecol=GPSDateTime, suffix='')
-
+    data = data.sort_values(by=[VehicleId, GPSDateTime])
+    # Reindex data
     print('Position matching', end='')
     # project data points onto bus LineString
     lineshp = line['geometry'].iloc[0]
     print('.', end='')
     data['geometry'] = gpd.points_from_xy(data[lon], data[lat])
     data = gpd.GeoDataFrame(data)
     data.set_crs(crs='epsg:4326', allow_override=True, inplace=True)
     print('.', end='')
-    data = data.to_crs(epsg=project_epsg)
+    data = data.to_crs(project_epsg)
     print('.', end='')
-    if method == 'project':
-        data['project'] = data['geometry'].apply(lineshp.project)
-    elif method == 'dislimit':
-        tmps = []
-        # Distance limit method
-        for vid in data[VehicleId].drop_duplicates():
-            print('.', end='')
-            tmp = data[data[VehicleId] == vid].copy()
-            i = 0
-            tmp = tmp.sort_values(
-                by=[VehicleId, GPSDateTime]).reset_index(drop=True)
-            tmp['project'] = 0
-            for i in range(len(tmp)-1):
-                if i == 0:
-                    proj = lineshp.project(tmp.iloc[i]['geometry'])
-                    tmp.loc[i, 'project'] = proj
-                else:
-                    proj = tmp['project'].iloc[i]
-                dis = tmp.iloc[i +
-                               1]['geometry'].distance(tmp.iloc[i]['geometry'])
-                if dis == 0:
-                    proj1 = proj
-                else:
-                    proj2 = lineshp.project(tmp.iloc[i+1]['geometry'])
-                    if abs(proj2-proj) > dis:
-                        proj1 = np.sign(proj2-proj)*dis+proj
-                    else:
-                        proj1 = proj2
-                tmp.loc[i+1, 'project'] = proj1
-            tmps.append(tmp)
-        data = pd.concat(tmps)
+
+    data['project'] = data['geometry'].apply(lineshp.project)
+    
+
+    # 设定时间与距离阈值阈值
+
+    # 比较相邻两条数据的信息
+    data[GPSDateTime+'_pre'] = data[GPSDateTime].shift()
+    data[VehicleId+'_pre'] = data[VehicleId].shift()
+    data['project_pre'] = data['project'].shift()
+    #定义三个条件
+    # 1.车辆位置发生了变化
+    condition1 = abs(data['project_pre']-data['project'])>disgap
+    # 2.相邻两条数据"时间间隔大于30分钟"
+    condition2 = (data[GPSDateTime]-data[GPSDateTime+'_pre']).dt.total_seconds()>timegap
+    # 3."本来这一条记录就是新车"
+    condition3 = data[VehicleId+'_pre']!=data[VehicleId]
+    data['condition1'] = condition1
+    data['condition2'] = condition2
+    data['condition3'] = condition3
+    # 标记新车辆
+    data['flag'] = (condition1 & condition2)|condition3
+    # 重新编号
+    data[VehicleId+'_new'] = data['flag'].cumsum()
+    # 重新编号后的车辆ID
+    reid = data[[VehicleId+'_new',VehicleId]].drop_duplicates()
+    
     print('.', end='')
     # Project bus stop to bus line
-    stop = stop.to_crs(epsg=project_epsg)
+    stop = stop.to_crs(project_epsg)
     stop['project'] = stop['geometry'].apply(lineshp.project)
     print('.', end='')
     starttime = data[GPSDateTime].min()
     data['time_st'] = (data[GPSDateTime]-starttime).dt.total_seconds()
     BUS_project = data
     print('.')
-
+    def get_arrive_info(
+            one_bus_data, 
+            position,
+            stopbuffer = 100
+    ):
+        '''
+        通过线与面的交集，识别到离站信息
+        输入：
+            one_bus_data：某一辆车的运行图数据
+            position：站点位置
+            stopbuffer：到站判定的缓冲区间隔
+        输出：
+            line_intersection：车辆轨迹与buffer的交集
+        '''
+        from shapely.geometry import LineString
+        #站点周边100米缓冲区
+        buffer_polygon = LineString([[0,position],
+                                    [24*3600,position]]).buffer(stopbuffer)
+        #生成车辆轨迹的linestring
+        bus_linestring = LineString(one_bus_data[['time_st','project']].values)
+        #提取车辆轨迹与buffer的交集
+        line_intersection = bus_linestring.intersection(buffer_polygon)
+        return line_intersection
+    #定义函数
+    def get_arrive_leave(line_intersection):
+        '''
+        从运行图中提取其中的到离站轨迹
+        输入：
+            line_intersection：车辆轨迹与buffer的交集
+        输出：
+            arrive：到站信息
+        '''
+        import shapely
+        # 如果没有到离站，则为空
+        arrive = []
+        if line_intersection.is_empty:
+            return pd.DataFrame()
+        # 如果只包含一次到离站，则类型为LineString
+        elif type(line_intersection) == shapely.geometry.linestring.LineString:
+            arrive = [line_intersection]
+        # 如果包含多次到离站，则类型为MultiLineString，需要将其拆分为多个LineString
+        elif type(line_intersection) == shapely.geometry.multilinestring.MultiLineString:
+            arrive = list(line_intersection.geoms)
+        #构建为DataFrame
+        arrive = pd.DataFrame(arrive)
+        #取每一次到离站时间戳
+        arrive['arrive_timestamp']= arrive[0].apply(lambda r:r.coords[0][0])
+        arrive['leave_timestamp']= arrive[0].apply(lambda r:r.coords[-1][0])
+        return arrive
+    def merge_arrive(arrive,stopname,vid,mintime = 300):
+        '''
+        本函数用于合并到离站信息
+        输入：
+            arrive：到离站信息
+            stopname：站点名
+            VehicleId：车辆ID
+            mintime：时间阈值
+        输出：
+            arrive_new：合并后的到离站信息
+        '''
+        #步骤①
+        a = arrive[['arrive_timestamp']]  
+        a.columns = ['time']  
+        a['flag'] = 1  
+        b = arrive[['leave_timestamp']]  
+        b.columns = ['time']  
+        b['flag'] = 0  
+        c = pd.concat([a,b]).sort_values(by = 'time')  
+        #步骤②
+        c['time1'] = c['time'].shift(-1)  
+        c['flag_1'] = ((c['time1']-c['time'])<mintime)&(c['flag']==0)  
+        c['flag_2'] = c['flag_1'].shift().fillna(False)  
+        c['flag_3'] = c['flag_1']|c['flag_2']  
+        #步骤③
+        c = c[-c['flag_3']]  
+        #步骤④
+        arrive_new = c[c['flag'] == 1][['time']]  
+        arrive_new.columns = ['arrive_timestamp']  
+        arrive_new['leave_timestamp'] = list(c[c['flag'] == 0]['time'])  
+        arrive_new[stopcol] = stopname  
+        arrive_new[VehicleId+'_new'] = vid 
+        return arrive_new 
+    #定义一个空的list存储识别结果
     ls = []
+    #对每一辆车遍历
     print('Matching arrival and leaving info...', end='')
-    for car in BUS_project[VehicleId].drop_duplicates():
+    for vid in BUS_project[VehicleId+'_new'].drop_duplicates():
         print('.', end='')
-        # Extract bus trajectory
-        tmp = BUS_project[BUS_project[VehicleId] == car]
-        if len(tmp) > 1:
+        #提取车辆运行图
+        one_bus_data = BUS_project[BUS_project[VehicleId+'_new'] == vid]
+        #如果车辆数据点少于等于1个，则无法构成轨迹
+        if len(one_bus_data)==1:
+            continue
+        else:
+            #对每一个站点识别
             for stopname in stop[stopcol].drop_duplicates():
-                # Get the stop position
+                #提取站点位置
                 position = stop[stop[stopcol] == stopname]['project'].iloc[0]
-                # Identify arrival and departure by intersection ofstop buffer
-                # and line segment
-                buffer_polygon = LineString([[0, position],
-                                             [data['time_st'].max(), position]
-                                             ]).buffer(stopbuffer)
-                bus_linestring = LineString(tmp[['time_st', 'project']].values)
-                line_intersection = bus_linestring.intersection(buffer_polygon)
-                # Extract leave time
-                if line_intersection.is_empty:
-                    # If empty, no bus arrive
+                #通过线与面的交集，识别到离站信息
+                line_intersection = get_arrive_info(one_bus_data,position,stopbuffer = stopbuffer)
+                arrive = get_arrive_leave(line_intersection)
+                if len(arrive)==0:
                     continue
-                else:
-                    if type(
-                        line_intersection
-                    ) == shapely.geometry.linestring.LineString:
-                        arrive = [line_intersection]
-                    else:
-                        arrive = list(line_intersection.geoms)
-                arrive = pd.DataFrame(arrive)
-                arrive['arrivetime'] = arrive[0].apply(
-                    lambda r: r.coords[0][0])
-                arrive['leavetime'] = arrive[0].apply(
-                    lambda r: r.coords[-1][0])
-                # Filtering arrival information through time threshold
-                a = arrive[['arrivetime']].copy()
-                a.columns = ['time']
-                a['flag'] = 1
-                b = arrive[['leavetime']].copy()
-                b.columns = ['time']
-                b['flag'] = 0
-                c = pd.concat([a, b]).sort_values(by='time')
-                c['time1'] = c['time'].shift(-1)
-                c['flag_1'] = ((c['time1']-c['time']) <
-                               mintime) & (c['flag'] == 0)
-                c['flag_2'] = c['flag_1'].shift().fillna(False)
-                c['flag_3'] = c['flag_1'] | c['flag_2']
-                c = c[-c['flag_3']]
-                arrive_new = c[c['flag'] == 1][['time']].copy()
-                arrive_new.columns = ['arrivetime']
-                arrive_new['leavetime'] = list(c[c['flag'] == 0]['time'])
-                arrive_new[stopcol] = stopname
-                arrive_new[VehicleId] = car
-                # Save data
+                arrive_new = merge_arrive(arrive,stopname,vid,mintime = mintime)
+                #合并数据
                 ls.append(arrive_new)
-    # Concat data
+    #将到离站信息合并
     arrive_info = pd.concat(ls)
+
     arrive_info['arrivetime'] = starttime + \
-        arrive_info['arrivetime'].apply(
+        arrive_info['arrive_timestamp'].apply(
             lambda r: pd.Timedelta(int(r), unit='s'))
     arrive_info['leavetime'] = starttime + \
-        arrive_info['leavetime'].apply(
+        arrive_info['leave_timestamp'].apply(
             lambda r: pd.Timedelta(int(r), unit='s'))
+    arrive_info = pd.merge(arrive_info, reid)
+    arrive_info = arrive_info.drop(['arrive_timestamp', 'leave_timestamp',VehicleId+'_new'], axis=1)
     if projectoutput:
         return arrive_info, data # pragma: no cover
     else:
         return arrive_info
 
 
 def busgps_onewaytime(arrive_info, start, end,
```

### Comparing `transbigdata-0.5.0/src/transbigdata/coordinates.py` & `transbigdata-0.5.1/src/transbigdata/coordinates.py`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.0/src/transbigdata/crawler.py` & `transbigdata-0.5.1/src/transbigdata/crawler.py`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.0/src/transbigdata/gisprocess.py` & `transbigdata-0.5.1/src/transbigdata/gisprocess.py`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.0/src/transbigdata/grids.py` & `transbigdata-0.5.1/src/transbigdata/grids.py`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.0/src/transbigdata/metro.py` & `transbigdata-0.5.1/src/transbigdata/metro.py`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.0/src/transbigdata/mobilephonedata.py` & `transbigdata-0.5.1/src/transbigdata/mobilephonedata.py`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.0/src/transbigdata/odprocess.py` & `transbigdata-0.5.1/src/transbigdata/odprocess.py`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.0/src/transbigdata/plotmap.py` & `transbigdata-0.5.1/src/transbigdata/plotmap.py`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.0/src/transbigdata/preprocess.py` & `transbigdata-0.5.1/src/transbigdata/preprocess.py`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.0/src/transbigdata/quality.py` & `transbigdata-0.5.1/src/transbigdata/quality.py`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.0/src/transbigdata/taxigps.py` & `transbigdata-0.5.1/src/transbigdata/taxigps.py`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.0/src/transbigdata/traj.py` & `transbigdata-0.5.1/src/transbigdata/traj.py`

 * *Files 1% similar despite different names*

```diff
@@ -455,14 +455,15 @@
     data_sliced['flag1'] = data_sliced.groupby(VehicleNum)['flag'].cumsum()
     data_sliced[VehicleNum] = data_sliced[VehicleNum].ffill()
     data_sliced = data_sliced[(data_sliced['flag1'] == 1) &
                               (data_sliced['flag'] == 0) &
                             (-data_sliced[VehicleNum].isnull())]
     data_sliced[SliceId] = data_sliced[SliceId].ffill()
     data_sliced.drop(['flag','flag1'], axis=1, inplace=True)
+    
     return data_sliced
 
 def traj_densify(data, col=['Vehicleid', 'Time', 'Lng', 'Lat'], timegap=15):
     '''
     Trajectory densification, ensure that there is a trajectory point each
     timegap seconds
 
@@ -680,15 +681,15 @@
     
     move['moveid'] = range(len(move))
     stay['stayid'] = range(len(stay))
     return stay, move
 
 
 
-def points_to_traj(traj_points, col=['Lng', 'Lat', 'ID'], timecol=None):
+def traj_to_linestring(traj_points, col=['Lng', 'Lat', 'ID'], timecol=None):
     '''
     Input trajectory, generate GeoDataFrame
 
     Parameters
     -------
     traj_points : DataFrame
         trajectory data
@@ -730,12 +731,12 @@
         traj_id = []
         for i in traj_points[ID].drop_duplicates():
             coords = traj_points[traj_points[ID] == i][[Lng, Lat]].values
             traj_id.append(i)
             if len(coords) >= 2:
                 geometry.append(LineString(coords))
             else:
-                geometry.append(None) # pragma: no cover
+                geometry.append(LineString([coords[0],coords[0]])) # pragma: no cover
         traj[ID] = traj_id
         traj['geometry'] = geometry
         traj = gpd.GeoDataFrame(traj)
     return traj
```

### Comparing `transbigdata-0.5.0/src/transbigdata/utils.py` & `transbigdata-0.5.1/src/transbigdata/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,16 +37,14 @@
     Input the json data and save it as a file. This method is suitable for
     sovling the problem that numpy cannot be compatiable with json package.
 
     Parameters
     -------
     data : json
         The json data to be saved
-
-
     path : str
         The storage path
 
     '''
     import json
 
     class NpEncoder(json.JSONEncoder):
```

### Comparing `transbigdata-0.5.0/src/transbigdata/visualization.py` & `transbigdata-0.5.1/src/transbigdata/visualization.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 '''
 
 import pandas as pd
 import numpy as np
 import geopandas as gpd
-from .traj import points_to_traj
+from .traj import traj_to_linestring
 from .grids import (
     area_to_params,
     GPS_to_grid,
     grid_to_polygon,
     grid_to_centre,
 )
 from .odprocess import (
@@ -79,15 +79,15 @@
         #clean data
     trajdata = trajdata[-((trajdata[Lng].isnull())|(trajdata[Lat].isnull()))]
     trajdata = trajdata[(trajdata[Lng]>=-180)&(trajdata[Lng]<=180)&(trajdata[Lat]>=-90)&(trajdata[Lat]<=90)]
     
     trajdata[timecol] = pd.to_datetime(trajdata[timecol])
 
     trajdata = trajdata.sort_values(by=[ID, timecol])
-    traj = points_to_traj(trajdata, col=[Lng, Lat, ID], timecol=timecol)
+    traj = traj_to_linestring(trajdata, col=[Lng, Lat, ID], timecol=timecol)
     ls = []
     for i in range(len(traj['features'])):
         ls.append(traj['features'][i]['geometry']['coordinates'][0])
         ls.append(traj['features'][i]['geometry']['coordinates'][-1])
     ls = pd.DataFrame(ls)
     lon_center, lat_center, starttime = ls[0].mean(), ls[1].mean(), ls[3].min()
     if zoom == 'auto':
```

### Comparing `transbigdata-0.5.0/transbigdata.egg-info/PKG-INFO` & `transbigdata-0.5.1/transbigdata.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transbigdata
-Version: 0.5.0
+Version: 0.5.1
 Summary: A Python package developed for transportation spatio-temporal big data processing and analysis.
 Home-page: https://github.com/ni1o1/transbigdata
 Author: Qing Yu
 Author-email: qingyu0815@foxmail.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/ni1o1/transbigdata/issues
 Classifier: Operating System :: OS Independent
@@ -345,13 +345,29 @@
 
 ![1648715064154.png](https://github.com/ni1o1/transbigdata/raw/main/image/README/1648715064154.png)
 
 See [This Example](https://github.com/ni1o1/transbigdata/blob/main/docs/source/gallery/Example%202-Grid-base%20processing%20framework%20of%20TransBigData.ipynb) for further details.
 
 ## Citation information [![DOI](https://zenodo.org/badge/419559811.svg)](https://zenodo.org/badge/latestdoi/419559811) [![status](https://joss.theoj.org/papers/d1055fe3105dfa2dcff4cb6c7688a79b/status.svg)](https://joss.theoj.org/papers/d1055fe3105dfa2dcff4cb6c7688a79b)
 
-Please cite [this](https://doi.org/10.21105/joss.04021) when using `TransBigData` in your research. Citation information can be found at [CITATION.cff](https://github.com/ni1o1/transbigdata/blob/main/CITATION.cff).
+Please cite [this](https://doi.org/10.21105/joss.04021) when using `TransBigData` in your research. Citation information is as follows:
+
+```bibtex
+@article{Yu2022,
+  doi       = {10.21105/joss.04021},
+  url       = {https://doi.org/10.21105/joss.04021},
+  year      = {2022},
+  publisher = {The Open Journal},
+  volume    = {7},
+  number    = {71},
+  pages     = {4021},
+  author    = {Qing Yu and Jian Yuan},
+  title     = {TransBigData: A Python package for transportation spatio-temporal big data processing, analysis and visualization},
+  journal   = {Journal of Open Source Software}
+}
+```
+
 
 ## Introducing Video (In Chinese) [![bilibili](https://img.shields.io/badge/bilibili-%E5%90%8C%E6%B5%8E%E5%B0%8F%E6%97%AD%E5%AD%A6%E9%95%BF-green.svg)](https://space.bilibili.com/3051484)
 
 * [Bilibili](https://www.bilibili.com/video/BV1na411i7sd/)
 * [Youtube](https://www.youtube.com/watch?v=ynqJ01WmPiQ)
```

### Comparing `transbigdata-0.5.0/transbigdata.egg-info/SOURCES.txt` & `transbigdata-0.5.1/transbigdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

