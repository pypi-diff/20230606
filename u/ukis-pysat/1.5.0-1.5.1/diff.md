# Comparing `tmp/ukis-pysat-1.5.0.tar.gz` & `tmp/ukis-pysat-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ukis-pysat-1.5.0.tar", last modified: Thu May  4 08:19:39 2023, max compression
+gzip compressed data, was "ukis-pysat-1.5.1.tar", last modified: Tue Jun  6 05:53:22 2023, max compression
```

## Comparing `ukis-pysat-1.5.0.tar` & `ukis-pysat-1.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:19:39.905615 ukis-pysat-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-05-04 08:19:24.000000 ukis-pysat-1.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-04 08:19:24.000000 ukis-pysat-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-05-04 08:19:39.905615 ukis-pysat-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-05-04 08:19:24.000000 ukis-pysat-1.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-04 08:19:24.000000 ukis-pysat-1.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 08:19:39.905615 ukis-pysat-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-04 08:19:24.000000 ukis-pysat-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:19:39.905615 ukis-pysat-1.5.0/ukis_pysat/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 08:19:24.000000 ukis-pysat-1.5.0/ukis_pysat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10909 2023-05-04 08:19:24.000000 ukis-pysat-1.5.0/ukis_pysat/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-04 08:19:24.000000 ukis-pysat-1.5.0/ukis_pysat/members.py
--rw-r--r--   0 runner    (1001) docker     (123)    22369 2023-05-04 08:19:24.000000 ukis-pysat-1.5.0/ukis_pysat/raster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:19:39.905615 ukis-pysat-1.5.0/ukis_pysat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-05-04 08:19:39.000000 ukis-pysat-1.5.0/ukis_pysat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-04 08:19:39.000000 ukis-pysat-1.5.0/ukis_pysat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:19:39.000000 ukis-pysat-1.5.0/ukis_pysat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:19:39.000000 ukis-pysat-1.5.0/ukis_pysat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-04 08:19:39.000000 ukis-pysat-1.5.0/ukis_pysat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 08:19:39.000000 ukis-pysat-1.5.0/ukis_pysat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:53:22.334442 ukis-pysat-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-06-06 05:53:13.000000 ukis-pysat-1.5.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-06 05:53:13.000000 ukis-pysat-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-06-06 05:53:22.334442 ukis-pysat-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-06-06 05:53:13.000000 ukis-pysat-1.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-06 05:53:13.000000 ukis-pysat-1.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 05:53:22.334442 ukis-pysat-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-06 05:53:13.000000 ukis-pysat-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:53:22.334442 ukis-pysat-1.5.1/ukis_pysat/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-06 05:53:13.000000 ukis-pysat-1.5.1/ukis_pysat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10909 2023-06-06 05:53:13.000000 ukis-pysat-1.5.1/ukis_pysat/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-06 05:53:13.000000 ukis-pysat-1.5.1/ukis_pysat/members.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24848 2023-06-06 05:53:13.000000 ukis-pysat-1.5.1/ukis_pysat/raster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:53:22.334442 ukis-pysat-1.5.1/ukis_pysat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-06-06 05:53:22.000000 ukis-pysat-1.5.1/ukis_pysat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-06 05:53:22.000000 ukis-pysat-1.5.1/ukis_pysat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 05:53:22.000000 ukis-pysat-1.5.1/ukis_pysat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 05:53:22.000000 ukis-pysat-1.5.1/ukis_pysat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-06 05:53:22.000000 ukis-pysat-1.5.1/ukis_pysat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-06 05:53:22.000000 ukis-pysat-1.5.1/ukis_pysat.egg-info/top_level.txt
```

### Comparing `ukis-pysat-1.5.0/LICENSE.txt` & `ukis-pysat-1.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ukis-pysat-1.5.0/PKG-INFO` & `ukis-pysat-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ukis-pysat
-Version: 1.5.0
+Version: 1.5.1
 Summary: generic classes and functions to query, access and process multi-spectral and SAR satellite images
 Home-page: https://github.com/dlr-eoc/ukis-pysat
 Author: German Aerospace Center (DLR)
 Author-email: ukis-helpdesk@dlr.de
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -18,15 +18,15 @@
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 [![UKIS](https://raw.githubusercontent.com/dlr-eoc/ukis-pysat/master/docs/ukis-logo.png)](https://www.dlr.de/eoc/en/desktopdefault.aspx/tabid-5413/10560_read-21914/) UKIS-pysat
 ==============
 
 ![ukis-pysat](https://github.com/dlr-eoc/ukis-pysat/workflows/ukis-pysat/badge.svg)
-[![codecov](https://codecov.io/gh/dlr-eoc/ukis-pysat/branch/master/graph/badge.svg)](https://codecov.io/gh/dlr-eoc/ukis-pysat)
+[![codecov](https://codecov.io/gh/dlr-eoc/ukis-pysat/branch/main/graph/badge.svg)](https://codecov.io/gh/dlr-eoc/ukis-pysat)
 ![Upload Python Package](https://github.com/dlr-eoc/ukis-pysat/workflows/Upload%20Python%20Package/badge.svg)
 [![PyPI version](https://img.shields.io/pypi/v/ukis-pysat)](https://pypi.python.org/pypi/ukis-pysat/)
 [![Documentation Status](https://readthedocs.org/projects/ukis-pysat/badge/?version=latest)](https://ukis-pysat.readthedocs.io/en/latest/?badge=latest)
 [![GitHub license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE.txt)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://black.readthedocs.io/en/stable/)
 [![DOI](https://zenodo.org/badge/259635994.svg)](https://zenodo.org/badge/latestdoi/259635994)
```

### Comparing `ukis-pysat-1.5.0/README.md` & `ukis-pysat-1.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [![UKIS](https://raw.githubusercontent.com/dlr-eoc/ukis-pysat/master/docs/ukis-logo.png)](https://www.dlr.de/eoc/en/desktopdefault.aspx/tabid-5413/10560_read-21914/) UKIS-pysat
 ==============
 
 ![ukis-pysat](https://github.com/dlr-eoc/ukis-pysat/workflows/ukis-pysat/badge.svg)
-[![codecov](https://codecov.io/gh/dlr-eoc/ukis-pysat/branch/master/graph/badge.svg)](https://codecov.io/gh/dlr-eoc/ukis-pysat)
+[![codecov](https://codecov.io/gh/dlr-eoc/ukis-pysat/branch/main/graph/badge.svg)](https://codecov.io/gh/dlr-eoc/ukis-pysat)
 ![Upload Python Package](https://github.com/dlr-eoc/ukis-pysat/workflows/Upload%20Python%20Package/badge.svg)
 [![PyPI version](https://img.shields.io/pypi/v/ukis-pysat)](https://pypi.python.org/pypi/ukis-pysat/)
 [![Documentation Status](https://readthedocs.org/projects/ukis-pysat/badge/?version=latest)](https://ukis-pysat.readthedocs.io/en/latest/?badge=latest)
 [![GitHub license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE.txt)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://black.readthedocs.io/en/stable/)
 [![DOI](https://zenodo.org/badge/259635994.svg)](https://zenodo.org/badge/latestdoi/259635994)
```

### Comparing `ukis-pysat-1.5.0/setup.py` & `ukis-pysat-1.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `ukis-pysat-1.5.0/ukis_pysat/file.py` & `ukis-pysat-1.5.1/ukis_pysat/file.py`

 * *Files identical despite different names*

### Comparing `ukis-pysat-1.5.0/ukis_pysat/raster.py` & `ukis-pysat-1.5.1/ukis_pysat/raster.py`

 * *Files 7% similar despite different names*

```diff
@@ -208,15 +208,23 @@
 
         memfile = MemoryFile()
         with memfile.open(**meta) as ds:
             ds.write(self.__arr)
         self.dataset = memfile.open()
         memfile.close()
 
-    def warp(self, dst_crs, resampling_method=0, num_threads=4, resolution=None, nodata=None, target_align=None):
+    def warp(
+        self,
+        dst_crs,
+        resampling_method=0,
+        num_threads=4,
+        resolution=None,
+        nodata=None,
+        target_align=None,
+    ):
         """Reproject a source raster to a destination raster.
 
         :param dst_crs: CRS or dict, Target coordinate reference system.
         :param resampling_method: Resampling algorithm, int, defaults to 0 (Nearest)
             numbers: https://github.com/mapbox/rasterio/blob/master/rasterio/enums.py#L28
         :param num_threads: int, number of workers, optional (default: 4)
         :param resolution: tuple (x resolution, y resolution) or float, optional.
@@ -280,46 +288,96 @@
             Platform.Landsat8,
         ]:
             if mtl_file is None:
                 raise AttributeError(f"'mtl_file' has to be set if platform is {platform}.")
             else:
                 # get rescale factors from mtl file
                 mtl = toa_utils._load_mtl(str(mtl_file))  # no obvious reason not to call this
-                metadata = mtl["L1_METADATA_FILE"]
+
+                # search for collection number in MTL metadata file
+                def iterate_mtl(mtl_obj):
+                    for key, value in mtl_obj.items():
+                        if isinstance(value, dict):
+                            for pair in iterate_mtl(value):
+                                yield (key, *pair)
+                        else:
+                            yield (key, value)
+
+                COLLECTION_NUMBER = next(
+                    (
+                        pair[pair.index("COLLECTION_NUMBER") + 1]
+                        for pair in iterate_mtl(mtl)
+                        if "COLLECTION_NUMBER" in pair
+                    ),
+                    None,
+                )
+                if not "COLLECTION_NUMBER":
+                    raise AttributeError("Cannot find COLLECTION_NUMBER in MTL metadata file")
+
+                # define collection specific group names
+                if COLLECTION_NUMBER == 1:
+                    # Landsat collection 1 naming convention
+                    mtl_group_main = "L1_METADATA_FILE"
+                    mtl_group_radiometric_rescaling = "RADIOMETRIC_RESCALING"
+                    if platform == Platform.Landsat8:
+                        mtl_group_thermal_constants = "TIRS_THERMAL_CONSTANTS"
+                    else:
+                        mtl_group_thermal_constants = "THERMAL_CONSTANTS"
+                elif COLLECTION_NUMBER == 2:
+                    # Landsat collection 2 naming convention
+                    mtl_group_main = "LANDSAT_METADATA_FILE"
+                    mtl_group_radiometric_rescaling = "LEVEL1_RADIOMETRIC_RESCALING"
+                    mtl_group_thermal_constants = "LEVEL1_THERMAL_CONSTANTS"
+                else:
+                    raise AttributeError(f"COLLECTION_NUMBER {COLLECTION_NUMBER} in metadata file is not supported")
+
+                metadata = mtl[mtl_group_main]
                 sun_elevation = metadata["IMAGE_ATTRIBUTES"]["SUN_ELEVATION"]
                 toa = []
 
                 for idx, b in enumerate(self._lookup_bands(platform, wavelengths)):
                     if (platform == Platform.Landsat8 and b in ["10", "11"]) or (
                         platform != Platform.Landsat8 and b.startswith("6")
                     ):
                         if platform == Platform.Landsat8:
-                            thermal_conversion_constant1 = metadata["TIRS_THERMAL_CONSTANTS"][f"K1_CONSTANT_BAND_{b}"]
-                            thermal_conversion_constant2 = metadata["TIRS_THERMAL_CONSTANTS"][f"K2_CONSTANT_BAND_{b}"]
+                            thermal_conversion_constant1 = metadata[mtl_group_thermal_constants][
+                                f"K1_CONSTANT_BAND_{b}"
+                            ]
+                            thermal_conversion_constant2 = metadata[mtl_group_thermal_constants][
+                                f"K2_CONSTANT_BAND_{b}"
+                            ]
                         else:
-                            thermal_conversion_constant1 = metadata["THERMAL_CONSTANTS"][f"K1_CONSTANT_BAND_{b}"]
-                            thermal_conversion_constant2 = metadata["THERMAL_CONSTANTS"][f"K2_CONSTANT_BAND_{b}"]
-                        multiplicative_rescaling_factors = metadata["RADIOMETRIC_RESCALING"][f"RADIANCE_MULT_BAND_{b}"]
-                        additive_rescaling_factors = metadata["RADIOMETRIC_RESCALING"][f"RADIANCE_ADD_BAND_{b}"]
+                            thermal_conversion_constant1 = metadata[mtl_group_thermal_constants][
+                                f"K1_CONSTANT_BAND_{b}"
+                            ]
+                            thermal_conversion_constant2 = metadata[mtl_group_thermal_constants][
+                                f"K2_CONSTANT_BAND_{b}"
+                            ]
+                        multiplicative_rescaling_factors = metadata[mtl_group_radiometric_rescaling][
+                            f"RADIANCE_MULT_BAND_{b}"
+                        ]
+                        additive_rescaling_factors = metadata[mtl_group_radiometric_rescaling][f"RADIANCE_ADD_BAND_{b}"]
 
                         # rescale thermal bands
                         toa.append(
                             brightness_temp.brightness_temp(
                                 self.__arr[idx, :, :],
                                 ML=multiplicative_rescaling_factors,
                                 AL=additive_rescaling_factors,
                                 K1=thermal_conversion_constant1,
                                 K2=thermal_conversion_constant2,
                             )
                         )
                         continue
 
                     # rescale reflectance bands
-                    multiplicative_rescaling_factors = metadata["RADIOMETRIC_RESCALING"][f"REFLECTANCE_MULT_BAND_{b}"]
-                    additive_rescaling_factors = metadata["RADIOMETRIC_RESCALING"][f"REFLECTANCE_ADD_BAND_{b}"]
+                    multiplicative_rescaling_factors = metadata[mtl_group_radiometric_rescaling][
+                        f"REFLECTANCE_MULT_BAND_{b}"
+                    ]
+                    additive_rescaling_factors = metadata[mtl_group_radiometric_rescaling][f"REFLECTANCE_ADD_BAND_{b}"]
                     toa.append(
                         reflectance.reflectance(
                             self.__arr[idx, :, :],
                             MR=multiplicative_rescaling_factors,
                             AR=additive_rescaling_factors,
                             E=sun_elevation,
                         )
@@ -451,15 +509,18 @@
 
         :param tile: rasterio.windows.Window tile from get_tiles().
         :param band: Band number (default: 0).
         :return: Sliced numpy array, bounding box of array slice.
         """
         # access window bounds
         bounds = rasterio.windows.bounds(tile, self.dataset.transform)
-        return self.__arr[(band,) + tile.toslices()], bounds  # Shape of array is announced with (bands, height, width)
+        return (
+            self.__arr[(band,) + tile.toslices()],
+            bounds,
+        )  # Shape of array is announced with (bands, height, width)
 
     def to_dask_array(self, chunk_size=(1, 6000, 6000)):
         """transforms numpy to dask array
 
         :param chunk_size: tuple, size of chunk, optional (default: (1, 6000, 6000))
         :return: dask array
         """
@@ -467,15 +528,23 @@
             import dask.array as da
         except ImportError:
             raise ImportError("to_dask_array requires optional dependency dask[array].")
 
         self.da_arr = da.from_array(self.__arr, chunks=chunk_size)
         return self.da_arr
 
-    def write_to_file(self, path_to_file, dtype, driver="GTiff", nodata=None, compress=None, kwargs=None):
+    def write_to_file(
+        self,
+        path_to_file,
+        dtype,
+        driver="GTiff",
+        nodata=None,
+        compress=None,
+        kwargs=None,
+    ):
         """
         Write a dataset to file.
         :param path_to_file: str, path to new file
         :param dtype: datatype, like np.uint16, 'float32' or 'min' to use the minimum type to represent values
 
         :param driver: str, optional (default: 'GTiff')
         :param nodata: nodata value, e.g. 255 (default: None, means nodata value of dataset will be used)
```

### Comparing `ukis-pysat-1.5.0/ukis_pysat.egg-info/PKG-INFO` & `ukis-pysat-1.5.1/ukis_pysat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ukis-pysat
-Version: 1.5.0
+Version: 1.5.1
 Summary: generic classes and functions to query, access and process multi-spectral and SAR satellite images
 Home-page: https://github.com/dlr-eoc/ukis-pysat
 Author: German Aerospace Center (DLR)
 Author-email: ukis-helpdesk@dlr.de
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -18,15 +18,15 @@
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 [![UKIS](https://raw.githubusercontent.com/dlr-eoc/ukis-pysat/master/docs/ukis-logo.png)](https://www.dlr.de/eoc/en/desktopdefault.aspx/tabid-5413/10560_read-21914/) UKIS-pysat
 ==============
 
 ![ukis-pysat](https://github.com/dlr-eoc/ukis-pysat/workflows/ukis-pysat/badge.svg)
-[![codecov](https://codecov.io/gh/dlr-eoc/ukis-pysat/branch/master/graph/badge.svg)](https://codecov.io/gh/dlr-eoc/ukis-pysat)
+[![codecov](https://codecov.io/gh/dlr-eoc/ukis-pysat/branch/main/graph/badge.svg)](https://codecov.io/gh/dlr-eoc/ukis-pysat)
 ![Upload Python Package](https://github.com/dlr-eoc/ukis-pysat/workflows/Upload%20Python%20Package/badge.svg)
 [![PyPI version](https://img.shields.io/pypi/v/ukis-pysat)](https://pypi.python.org/pypi/ukis-pysat/)
 [![Documentation Status](https://readthedocs.org/projects/ukis-pysat/badge/?version=latest)](https://ukis-pysat.readthedocs.io/en/latest/?badge=latest)
 [![GitHub license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE.txt)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://black.readthedocs.io/en/stable/)
 [![DOI](https://zenodo.org/badge/259635994.svg)](https://zenodo.org/badge/latestdoi/259635994)
```

