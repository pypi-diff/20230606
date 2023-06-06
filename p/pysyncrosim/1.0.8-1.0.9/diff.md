# Comparing `tmp/pysyncrosim-1.0.8.tar.gz` & `tmp/pysyncrosim-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pysyncrosim-1.0.8.tar", last modified: Tue Jan 18 23:23:16 2022, max compression
+gzip compressed data, was "pysyncrosim-1.0.9.tar", last modified: Tue Jan 18 23:37:24 2022, max compression
```

## Comparing `pysyncrosim-1.0.8.tar` & `pysyncrosim-1.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2022-01-18 23:23:16.334709 pysyncrosim-1.0.8/
--rw-rw-rw-   0        0        0     1087 2021-09-28 22:08:10.000000 pysyncrosim-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     6178 2022-01-18 23:23:16.333897 pysyncrosim-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     5889 2022-01-18 23:20:18.000000 pysyncrosim-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-01-18 23:23:16.298189 pysyncrosim-1.0.8/pysyncrosim/
--rw-rw-rw-   0        0        0      583 2022-01-13 00:19:20.000000 pysyncrosim-1.0.8/pysyncrosim/__init__.py
--rw-rw-rw-   0        0        0       23 2022-01-18 23:22:38.000000 pysyncrosim-1.0.8/pysyncrosim/_version.py
--rw-rw-rw-   0        0        0     5551 2022-01-13 22:05:26.000000 pysyncrosim-1.0.8/pysyncrosim/environment.py
--rw-rw-rw-   0        0        0     9845 2022-01-04 22:37:36.000000 pysyncrosim-1.0.8/pysyncrosim/helper.py
--rw-rw-rw-   0        0        0    47605 2022-01-13 22:15:31.000000 pysyncrosim-1.0.8/pysyncrosim/library.py
--rw-rw-rw-   0        0        0    10605 2022-01-13 22:15:40.000000 pysyncrosim-1.0.8/pysyncrosim/project.py
--rw-rw-rw-   0        0        0     4540 2022-01-13 22:15:57.000000 pysyncrosim-1.0.8/pysyncrosim/raster.py
--rw-rw-rw-   0        0        0    33008 2022-01-13 22:15:49.000000 pysyncrosim-1.0.8/pysyncrosim/scenario.py
--rw-rw-rw-   0        0        0    12876 2022-01-13 22:15:09.000000 pysyncrosim-1.0.8/pysyncrosim/session.py
-drwxrwxrwx   0        0        0        0 2022-01-18 23:23:16.330004 pysyncrosim-1.0.8/pysyncrosim.egg-info/
--rw-rw-rw-   0        0        0     6178 2022-01-18 23:23:16.000000 pysyncrosim-1.0.8/pysyncrosim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      422 2022-01-18 23:23:16.000000 pysyncrosim-1.0.8/pysyncrosim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-18 23:23:16.000000 pysyncrosim-1.0.8/pysyncrosim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2022-01-18 23:23:16.000000 pysyncrosim-1.0.8/pysyncrosim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-01-18 23:23:16.334709 pysyncrosim-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      787 2022-01-18 18:05:20.000000 pysyncrosim-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-01-18 23:23:16.332513 pysyncrosim-1.0.8/tests/
--rw-rw-rw-   0        0        0        4 2021-09-08 15:24:00.000000 pysyncrosim-1.0.8/tests/__init__.py
--rw-rw-rw-   0        0        0    35335 2022-01-07 21:03:50.000000 pysyncrosim-1.0.8/tests/test_pysyncrosim.py
+drwxrwxrwx   0        0        0        0 2022-01-18 23:37:24.549402 pysyncrosim-1.0.9/
+-rw-rw-rw-   0        0        0     1087 2021-09-28 22:08:10.000000 pysyncrosim-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     6169 2022-01-18 23:37:24.548903 pysyncrosim-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5880 2022-01-18 23:30:32.000000 pysyncrosim-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-01-18 23:37:24.510009 pysyncrosim-1.0.9/pysyncrosim/
+-rw-rw-rw-   0        0        0      583 2022-01-13 00:19:20.000000 pysyncrosim-1.0.9/pysyncrosim/__init__.py
+-rw-rw-rw-   0        0        0       23 2022-01-18 23:29:30.000000 pysyncrosim-1.0.9/pysyncrosim/_version.py
+-rw-rw-rw-   0        0        0     5551 2022-01-13 22:05:26.000000 pysyncrosim-1.0.9/pysyncrosim/environment.py
+-rw-rw-rw-   0        0        0     9845 2022-01-04 22:37:36.000000 pysyncrosim-1.0.9/pysyncrosim/helper.py
+-rw-rw-rw-   0        0        0    47605 2022-01-13 22:15:31.000000 pysyncrosim-1.0.9/pysyncrosim/library.py
+-rw-rw-rw-   0        0        0    10605 2022-01-13 22:15:40.000000 pysyncrosim-1.0.9/pysyncrosim/project.py
+-rw-rw-rw-   0        0        0     4540 2022-01-13 22:15:57.000000 pysyncrosim-1.0.9/pysyncrosim/raster.py
+-rw-rw-rw-   0        0        0    33008 2022-01-13 22:15:49.000000 pysyncrosim-1.0.9/pysyncrosim/scenario.py
+-rw-rw-rw-   0        0        0    12876 2022-01-13 22:15:09.000000 pysyncrosim-1.0.9/pysyncrosim/session.py
+drwxrwxrwx   0        0        0        0 2022-01-18 23:37:24.544647 pysyncrosim-1.0.9/pysyncrosim.egg-info/
+-rw-rw-rw-   0        0        0     6169 2022-01-18 23:37:24.000000 pysyncrosim-1.0.9/pysyncrosim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2022-01-18 23:37:24.000000 pysyncrosim-1.0.9/pysyncrosim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-01-18 23:37:24.000000 pysyncrosim-1.0.9/pysyncrosim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2022-01-18 23:37:24.000000 pysyncrosim-1.0.9/pysyncrosim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-01-18 23:37:24.550164 pysyncrosim-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      787 2022-01-18 18:05:20.000000 pysyncrosim-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-01-18 23:37:24.547570 pysyncrosim-1.0.9/tests/
+-rw-rw-rw-   0        0        0        4 2021-09-08 15:24:00.000000 pysyncrosim-1.0.9/tests/__init__.py
+-rw-rw-rw-   0        0        0    35335 2022-01-07 21:03:50.000000 pysyncrosim-1.0.9/tests/test_pysyncrosim.py
```

### Comparing `pysyncrosim-1.0.8/LICENSE` & `pysyncrosim-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pysyncrosim-1.0.8/PKG-INFO` & `pysyncrosim-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pysyncrosim
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python interface to SyncroSim
 Home-page: https://syncrosim.com/
 Author: ApexRMS
 Author-email: info@apexrms.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# pysyncrosim <img src="docs/logo.png" align="right" width=140/>
+# pysyncrosim <img src="docs/img/logo.png" align="right" width=140/>
 
 The Python interface to [SyncroSim](https://syncrosim.com/)
 
 ## Installation
 
 `pysyncrosim` can be installed using either the `conda` or `pip` package managers. `conda` is a general package manager capable of installing packages from many sources, but `pip` is strictly a Python package manager. While the installation instructions below are based on a Windows 10 operating system, similar steps can be used to install `pysyncrosim` for Linux.
 
@@ -106,15 +106,15 @@
 spyder
 ```
 
 *Note: you may get a pop-up saying you have a missing dependency, `rtree`. You can safely ignore this warning.*
 
 3. Within the IDE, change the working directory to the directory containing your `pysyncrosim` scripts (e.g. [spatial_demo.py](https://github.com/syncrosim/pysyncrosim/blob/main/examples/spatial_demo.py) and [input-raster.tif](https://github.com/syncrosim/pysyncrosim/blob/main/examples/input-raster.tif))
 
-![Using pysyncrosim in Spyder](https://github.com/syncrosim/pysyncrosim/raw/main/docs/img/pysyncrosim-with-UI.PNG)
+![Using pysyncrosim in Spyder](https://github.com/syncrosim/pysyncrosim/raw/main/docs/img/spyder.PNG)
 
 4. Open and run your `pysyncrosim` scripts from the left-hand window. You can run scripts line-by-line in `spyder` by selecting the line(s) you want to run and pressing F9.
 
 ### SyncroSim Package Development
 
 If you wish to design SyncroSim packages using python and `pysyncrosim`, you can follow the [Creating a Package](http://docs.syncrosim.com/how_to_guides/package_create_overview.html) and [Enhancing a Package](http://docs.syncrosim.com/how_to_guides/package_enhance_overview.html) tutorials on the [SyncroSim documentation website](http://docs.syncrosim.com/). Note that [SyncroSim v2.3.6](https://syncrosim.com/download/) is required to develop python-based SyncroSim packages.
```

### Comparing `pysyncrosim-1.0.8/README.md` & `pysyncrosim-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pysyncrosim <img src="docs/logo.png" align="right" width=140/>
+# pysyncrosim <img src="docs/img/logo.png" align="right" width=140/>
 
 The Python interface to [SyncroSim](https://syncrosim.com/)
 
 ## Installation
 
 `pysyncrosim` can be installed using either the `conda` or `pip` package managers. `conda` is a general package manager capable of installing packages from many sources, but `pip` is strictly a Python package manager. While the installation instructions below are based on a Windows 10 operating system, similar steps can be used to install `pysyncrosim` for Linux.
 
@@ -94,14 +94,14 @@
 spyder
 ```
 
 *Note: you may get a pop-up saying you have a missing dependency, `rtree`. You can safely ignore this warning.*
 
 3. Within the IDE, change the working directory to the directory containing your `pysyncrosim` scripts (e.g. [spatial_demo.py](https://github.com/syncrosim/pysyncrosim/blob/main/examples/spatial_demo.py) and [input-raster.tif](https://github.com/syncrosim/pysyncrosim/blob/main/examples/input-raster.tif))
 
-![Using pysyncrosim in Spyder](https://github.com/syncrosim/pysyncrosim/raw/main/docs/img/pysyncrosim-with-UI.PNG)
+![Using pysyncrosim in Spyder](https://github.com/syncrosim/pysyncrosim/raw/main/docs/img/spyder.PNG)
 
 4. Open and run your `pysyncrosim` scripts from the left-hand window. You can run scripts line-by-line in `spyder` by selecting the line(s) you want to run and pressing F9.
 
 ### SyncroSim Package Development
 
 If you wish to design SyncroSim packages using python and `pysyncrosim`, you can follow the [Creating a Package](http://docs.syncrosim.com/how_to_guides/package_create_overview.html) and [Enhancing a Package](http://docs.syncrosim.com/how_to_guides/package_enhance_overview.html) tutorials on the [SyncroSim documentation website](http://docs.syncrosim.com/). Note that [SyncroSim v2.3.6](https://syncrosim.com/download/) is required to develop python-based SyncroSim packages.
```

### Comparing `pysyncrosim-1.0.8/pysyncrosim/__init__.py` & `pysyncrosim-1.0.9/pysyncrosim/__init__.py`

 * *Files identical despite different names*

### Comparing `pysyncrosim-1.0.8/pysyncrosim/environment.py` & `pysyncrosim-1.0.9/pysyncrosim/environment.py`

 * *Files identical despite different names*

### Comparing `pysyncrosim-1.0.8/pysyncrosim/helper.py` & `pysyncrosim-1.0.9/pysyncrosim/helper.py`

 * *Files identical despite different names*

### Comparing `pysyncrosim-1.0.8/pysyncrosim/library.py` & `pysyncrosim-1.0.9/pysyncrosim/library.py`

 * *Files identical despite different names*

### Comparing `pysyncrosim-1.0.8/pysyncrosim/project.py` & `pysyncrosim-1.0.9/pysyncrosim/project.py`

 * *Files identical despite different names*

### Comparing `pysyncrosim-1.0.8/pysyncrosim/raster.py` & `pysyncrosim-1.0.9/pysyncrosim/raster.py`

 * *Files identical despite different names*

### Comparing `pysyncrosim-1.0.8/pysyncrosim/scenario.py` & `pysyncrosim-1.0.9/pysyncrosim/scenario.py`

 * *Files identical despite different names*

### Comparing `pysyncrosim-1.0.8/pysyncrosim/session.py` & `pysyncrosim-1.0.9/pysyncrosim/session.py`

 * *Files identical despite different names*

### Comparing `pysyncrosim-1.0.8/pysyncrosim.egg-info/PKG-INFO` & `pysyncrosim-1.0.9/pysyncrosim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pysyncrosim
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python interface to SyncroSim
 Home-page: https://syncrosim.com/
 Author: ApexRMS
 Author-email: info@apexrms.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# pysyncrosim <img src="docs/logo.png" align="right" width=140/>
+# pysyncrosim <img src="docs/img/logo.png" align="right" width=140/>
 
 The Python interface to [SyncroSim](https://syncrosim.com/)
 
 ## Installation
 
 `pysyncrosim` can be installed using either the `conda` or `pip` package managers. `conda` is a general package manager capable of installing packages from many sources, but `pip` is strictly a Python package manager. While the installation instructions below are based on a Windows 10 operating system, similar steps can be used to install `pysyncrosim` for Linux.
 
@@ -106,15 +106,15 @@
 spyder
 ```
 
 *Note: you may get a pop-up saying you have a missing dependency, `rtree`. You can safely ignore this warning.*
 
 3. Within the IDE, change the working directory to the directory containing your `pysyncrosim` scripts (e.g. [spatial_demo.py](https://github.com/syncrosim/pysyncrosim/blob/main/examples/spatial_demo.py) and [input-raster.tif](https://github.com/syncrosim/pysyncrosim/blob/main/examples/input-raster.tif))
 
-![Using pysyncrosim in Spyder](https://github.com/syncrosim/pysyncrosim/raw/main/docs/img/pysyncrosim-with-UI.PNG)
+![Using pysyncrosim in Spyder](https://github.com/syncrosim/pysyncrosim/raw/main/docs/img/spyder.PNG)
 
 4. Open and run your `pysyncrosim` scripts from the left-hand window. You can run scripts line-by-line in `spyder` by selecting the line(s) you want to run and pressing F9.
 
 ### SyncroSim Package Development
 
 If you wish to design SyncroSim packages using python and `pysyncrosim`, you can follow the [Creating a Package](http://docs.syncrosim.com/how_to_guides/package_create_overview.html) and [Enhancing a Package](http://docs.syncrosim.com/how_to_guides/package_enhance_overview.html) tutorials on the [SyncroSim documentation website](http://docs.syncrosim.com/). Note that [SyncroSim v2.3.6](https://syncrosim.com/download/) is required to develop python-based SyncroSim packages.
```

### Comparing `pysyncrosim-1.0.8/setup.py` & `pysyncrosim-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `pysyncrosim-1.0.8/tests/test_pysyncrosim.py` & `pysyncrosim-1.0.9/tests/test_pysyncrosim.py`

 * *Files identical despite different names*

