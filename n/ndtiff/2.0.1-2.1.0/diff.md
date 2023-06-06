# Comparing `tmp/ndtiff-2.0.1.tar.gz` & `tmp/ndtiff-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndtiff-2.0.1.tar", last modified: Fri Jun  2 21:18:31 2023, max compression
+gzip compressed data, was "ndtiff-2.1.0.tar", last modified: Tue Jun  6 20:39:08 2023, max compression
```

## Comparing `ndtiff-2.0.1.tar` & `ndtiff-2.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:18:31.840706 ndtiff-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-02 21:18:31.840706 ndtiff-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-02 21:18:15.000000 ndtiff-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:18:31.836706 ndtiff-2.0.1/ndtiff/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-02 21:18:15.000000 ndtiff-2.0.1/ndtiff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-02 21:18:15.000000 ndtiff-2.0.1/ndtiff/_superclass.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-02 21:18:15.000000 ndtiff-2.0.1/ndtiff/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-02 21:18:15.000000 ndtiff-2.0.1/ndtiff/file_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    42655 2023-06-02 21:18:15.000000 ndtiff-2.0.1/ndtiff/nd_tiff_current.py
--rw-r--r--   0 runner    (1001) docker     (123)    28211 2023-06-02 21:18:15.000000 ndtiff-2.0.1/ndtiff/nd_tiff_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    44915 2023-06-02 21:18:15.000000 ndtiff-2.0.1/ndtiff/ndtiff_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:18:31.840706 ndtiff-2.0.1/ndtiff/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 21:18:15.000000 ndtiff-2.0.1/ndtiff/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-02 21:18:15.000000 ndtiff-2.0.1/ndtiff/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-06-02 21:18:15.000000 ndtiff-2.0.1/ndtiff/test/data_loading_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-02 21:18:15.000000 ndtiff-2.0.1/ndtiff/test/test_custom_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:18:31.840706 ndtiff-2.0.1/ndtiff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-02 21:18:31.000000 ndtiff-2.0.1/ndtiff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-02 21:18:31.000000 ndtiff-2.0.1/ndtiff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 21:18:31.000000 ndtiff-2.0.1/ndtiff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-02 21:18:31.000000 ndtiff-2.0.1/ndtiff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 21:18:31.000000 ndtiff-2.0.1/ndtiff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-02 21:18:15.000000 ndtiff-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 21:18:31.840706 ndtiff-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-02 21:18:15.000000 ndtiff-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:39:08.480429 ndtiff-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-06 20:39:08.480429 ndtiff-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-06 20:38:58.000000 ndtiff-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:39:08.476429 ndtiff-2.1.0/ndtiff/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-06 20:38:58.000000 ndtiff-2.1.0/ndtiff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-06 20:38:58.000000 ndtiff-2.1.0/ndtiff/_superclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-06 20:38:58.000000 ndtiff-2.1.0/ndtiff/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-06 20:38:58.000000 ndtiff-2.1.0/ndtiff/file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42655 2023-06-06 20:38:58.000000 ndtiff-2.1.0/ndtiff/nd_tiff_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28685 2023-06-06 20:38:58.000000 ndtiff-2.1.0/ndtiff/nd_tiff_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44915 2023-06-06 20:38:58.000000 ndtiff-2.1.0/ndtiff/ndtiff_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:39:08.480429 ndtiff-2.1.0/ndtiff/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:38:58.000000 ndtiff-2.1.0/ndtiff/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-06 20:38:58.000000 ndtiff-2.1.0/ndtiff/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-06-06 20:38:58.000000 ndtiff-2.1.0/ndtiff/test/data_loading_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-06 20:38:58.000000 ndtiff-2.1.0/ndtiff/test/test_custom_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:39:08.480429 ndtiff-2.1.0/ndtiff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-06 20:39:08.000000 ndtiff-2.1.0/ndtiff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-06 20:39:08.000000 ndtiff-2.1.0/ndtiff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 20:39:08.000000 ndtiff-2.1.0/ndtiff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-06 20:39:08.000000 ndtiff-2.1.0/ndtiff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-06 20:39:08.000000 ndtiff-2.1.0/ndtiff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-06 20:38:58.000000 ndtiff-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 20:39:08.480429 ndtiff-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-06 20:38:58.000000 ndtiff-2.1.0/setup.py
```

### Comparing `ndtiff-2.0.1/PKG-INFO` & `ndtiff-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndtiff
-Version: 2.0.1
+Version: 2.1.0
 Summary: Python libraries for NDTiff datasets
 Home-page: https://github.com/micro-manager/NDTiffStorage
 Author: Henry Pinkard
 Author-email: henry.pinkard@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ndtiff-2.0.1/ndtiff/_superclass.py` & `ndtiff-2.1.0/ndtiff/_superclass.py`

 * *Files identical despite different names*

### Comparing `ndtiff-2.0.1/ndtiff/file_io.py` & `ndtiff-2.1.0/ndtiff/file_io.py`

 * *Files identical despite different names*

### Comparing `ndtiff-2.0.1/ndtiff/nd_tiff_current.py` & `ndtiff-2.1.0/ndtiff/nd_tiff_current.py`

 * *Files identical despite different names*

### Comparing `ndtiff-2.0.1/ndtiff/nd_tiff_v2.py` & `ndtiff-2.1.0/ndtiff/nd_tiff_v2.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,35 @@
 import json
 import dask.array as da
 import warnings
 import struct
 import threading
 from ndtiff.file_io import NDTiffFileIO, BUILTIN_FILE_IO
 
+_POSITION_AXIS = "position"
+_ROW_AXIS = "row"
+_COLUMN_AXIS = "column"
+_Z_AXIS = "z"
+_TIME_AXIS = "time"
+_CHANNEL_AXIS = "channel"
+
+_AXIS_ORDER = {_ROW_AXIS: 7,
+               _COLUMN_AXIS: 6,
+               _POSITION_AXIS: 5, 
+               _TIME_AXIS: 4, 
+               _CHANNEL_AXIS:3, 
+               _Z_AXIS:2}
+
+def _get_axis_order_key(dict_item):
+    axis_name = dict_item[0]
+    if axis_name in _AXIS_ORDER.keys():
+        return _AXIS_ORDER[axis_name]
+    else:
+        return 3  # stack next to channel axes
+
 class _MultipageTiffReader:
     """
     Class corresponsing to a single multipage tiff file in a Micro-Magellan dataset.
     Pass the full path of the TIFF to instantiate and call close() when finished
     """
 
     # file format constants
@@ -266,21 +287,14 @@
 
 ### This function outside class to prevent problems with pickling when running them in differnet process
 
 
 class NDTiff_v2_0():
     """Class that opens a single NDTiffStorage dataset"""
 
-    _POSITION_AXIS = "position"
-    _ROW_AXIS = "row"
-    _COLUMN_AXIS = "column"
-    _Z_AXIS = "z"
-    _TIME_AXIS = "time"
-    _CHANNEL_AXIS = "channel"
-
     def __init__(self, dataset_path=None, full_res_only=True, remote_storage_monitor=None, file_io: NDTiffFileIO = BUILTIN_FILE_IO):
         """
         Creat a Object providing access to and NDTiffStorage dataset, either one currently being acquired or one on disk
 
         Parameters
         ----------
         dataset_path : str
@@ -365,14 +379,16 @@
 
                 self.axes = {}
                 for axes_combo in res_level.index.keys():
                     for axis, position in axes_combo:
                         if axis not in self.axes.keys():
                             self.axes[axis] = set()
                         self.axes[axis].add(position)
+                # Sort axes according to _AXIS_ORDER
+                self.axes = dict(sorted(self.axes.items(), key=_get_axis_order_key, reverse=True))
 
                 # figure out the mapping of channel name to position by reading image metadata
                 print("\rReading channel names...", end="")
                 self._read_channel_names()
                 print("\rFinished reading channel names", end="")
 
                 # remove axes with no variation
@@ -389,25 +405,25 @@
         with self._lock:
             first_index = list(self.res_levels[0].index.values())[0]
         self._parse_first_index(first_index)
 
         print("\rDataset opened                ")
 
     def _read_channel_names(self):
-        if self._CHANNEL_AXIS in self.axes.keys():
+        if _CHANNEL_AXIS in self.axes.keys():
             self._channel_names = {}
             for key in self.res_levels[0].index.keys():
                 axes = {axis: position for axis, position in key}
                 if (
-                    self._CHANNEL_AXIS in axes.keys()
-                    and axes[self._CHANNEL_AXIS] not in self._channel_names.values()
+                    _CHANNEL_AXIS in axes.keys()
+                    and axes[_CHANNEL_AXIS] not in self._channel_names.values()
                 ):
                     channel_name = self.res_levels[0].read_metadata(axes)["Channel"]
-                    self._channel_names[channel_name] = axes[self._CHANNEL_AXIS]
-                if len(self._channel_names.values()) == len(self.axes[self._CHANNEL_AXIS]):
+                    self._channel_names[channel_name] = axes[_CHANNEL_AXIS]
+                if len(self._channel_names.values()) == len(self.axes[_CHANNEL_AXIS]):
                     break
 
     def _parse_first_index(self, first_index):
         """
         Read through first index to get some global data about images (assuming it is same for all)
         """
         if first_index["pixel_type"] == _MultipageTiffReader.EIGHT_BIT_RGB:
@@ -464,16 +480,16 @@
 
         To convert data into a numpy array, call np.asarray() on the returned result. However, doing so will bring the
         data into RAM, so it may be better to do this on only a slice of the array at a time.
 
         Parameters
         ----------
         axes : list
-            list of axes names over which to iterate and merge into a stacked array. If None, all axes will be used.
-            The order of axes supplied in this list will be the order of the axes of the returned dask array
+            list of axes names over which to iterate and merge into a stacked array. The order of axes supplied in this 
+            list will be the order of the axes of the returned dask array. If None, all axes will be used in PTCZYX order.
         stitched : bool
             If true and tiles were acquired in a grid, lay out adjacent tiles next to one another (Default value = False)
         **kwargs :
             names and integer positions of axes on which to slice data
         Returns
         -------
         dataset : dask array
@@ -718,23 +734,23 @@
     def get_channel_names(self):
         with self._lock:
             return self._channel_names.keys()
 
     def _consolidate_axes(self, channel, channel_name, z, position, time, row, col, kwargs):
         axes = {}
         if channel is not None:
-            axes[self._CHANNEL_AXIS] = channel
+            axes[_CHANNEL_AXIS] = channel
         if channel_name is not None:
-            axes[self._CHANNEL_AXIS] = self._channel_names[channel_name]
+            axes[_CHANNEL_AXIS] = self._channel_names[channel_name]
         if z is not None:
-            axes[self._Z_AXIS] = z
+            axes[_Z_AXIS] = z
         if position is not None:
-            axes[self._POSITION_AXIS] = position
+            axes[_POSITION_AXIS] = position
         if time is not None:
-            axes[self._TIME_AXIS] = time
+            axes[_TIME_AXIS] = time
         if row is not None:
-            axes[self._ROW_AXIS] = row
+            axes[_ROW_AXIS] = row
         if col is not None:
-            axes[self._COLUMN_AXIS] = col
+            axes[_COLUMN_AXIS] = col
         for other_axis_name in kwargs.keys():
             axes[other_axis_name] = kwargs[other_axis_name]
         return axes
```

### Comparing `ndtiff-2.0.1/ndtiff/ndtiff_v1.py` & `ndtiff-2.1.0/ndtiff/ndtiff_v1.py`

 * *Files identical despite different names*

### Comparing `ndtiff-2.0.1/ndtiff/test/data_loading_test.py` & `ndtiff-2.1.0/ndtiff/test/data_loading_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,22 @@
 
 
 def test_v2_data(test_data_path):
     data_path = os.path.join(test_data_path, "v2", "ndtiffv2.0_test")
     dataset = Dataset(data_path)
     assert(np.mean(dataset.as_array()) > 0)
 
+def test_v2_data_axis_sorting(test_data_path):
+    data_path = os.path.join(test_data_path, "v2", "ndtiffv2.0_test")
+    dataset = Dataset(data_path)
+    num_timepoints = len(dataset.axes['time'])
+    num_channels = len(dataset.axes['channel'])
+    data = dataset.as_array(axes=None)
+    assert data.shape[:-2] == (num_timepoints, num_channels)
+
 def test_v3_data(test_data_path):
     data_path = os.path.join(test_data_path, 'v3', 'ndtiffv3.0_test')
     dataset = Dataset(data_path)
     assert(np.mean(dataset.as_array()) > 0)
     for channel_name, correct_channel_name in zip(dataset.get_channel_names(), ['DAPI', 'FITC']):
         assert(channel_name == correct_channel_name)
```

### Comparing `ndtiff-2.0.1/ndtiff/test/test_custom_io.py` & `ndtiff-2.1.0/ndtiff/test/test_custom_io.py`

 * *Files identical despite different names*

### Comparing `ndtiff-2.0.1/ndtiff.egg-info/PKG-INFO` & `ndtiff-2.1.0/ndtiff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndtiff
-Version: 2.0.1
+Version: 2.1.0
 Summary: Python libraries for NDTiff datasets
 Home-page: https://github.com/micro-manager/NDTiffStorage
 Author: Henry Pinkard
 Author-email: henry.pinkard@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ndtiff-2.0.1/setup.py` & `ndtiff-2.1.0/setup.py`

 * *Files identical despite different names*

