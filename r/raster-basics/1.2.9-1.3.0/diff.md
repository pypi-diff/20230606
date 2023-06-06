# Comparing `tmp/raster_basics-1.2.9.tar.gz` & `tmp/raster_basics-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raster_basics-1.2.9.tar", last modified: Tue Jun  6 14:08:19 2023, max compression
+gzip compressed data, was "raster_basics-1.3.0.tar", last modified: Tue Jun  6 14:11:21 2023, max compression
```

## Comparing `raster_basics-1.2.9.tar` & `raster_basics-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-06 14:08:19.691390 raster_basics-1.2.9/
--rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-06 14:08:19.691454 raster_basics-1.2.9/PKG-INFO
-drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-06 14:08:19.690417 raster_basics-1.2.9/raster_basics/
--rw-rw-r--   0 albinwells   (501) staff       (20)     8661 2023-02-27 17:09:17.000000 raster_basics-1.2.9/raster_basics/BaseFunctions.py
--rw-rw-r--   0 albinwells   (501) staff       (20)    42097 2023-06-01 21:15:30.000000 raster_basics-1.2.9/raster_basics/DataPlots.py
--rw-rw-r--   0 albinwells   (501) staff       (20)    17690 2023-06-02 17:27:11.000000 raster_basics-1.2.9/raster_basics/GlacierFunctions.py
--rw-rw-r--   0 albinwells   (501) staff       (20)    12235 2023-03-23 16:41:47.000000 raster_basics-1.2.9/raster_basics/RasterBasics.py
--rwxrwxrwx   0 albinwells   (501) staff       (20)    12012 2023-06-06 14:07:38.000000 raster_basics-1.2.9/raster_basics/SmoothingFunctions.py
--rw-rw-r--   0 albinwells   (501) staff       (20)      574 2023-02-03 15:09:59.000000 raster_basics-1.2.9/raster_basics/__init__.py
-drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-06 14:08:19.691264 raster_basics-1.2.9/raster_basics.egg-info/
--rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-06 14:08:19.000000 raster_basics-1.2.9/raster_basics.egg-info/PKG-INFO
--rw-r--r--   0 albinwells   (501) staff       (20)      386 2023-06-06 14:08:19.000000 raster_basics-1.2.9/raster_basics.egg-info/SOURCES.txt
--rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-06 14:08:19.000000 raster_basics-1.2.9/raster_basics.egg-info/dependency_links.txt
--rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-06 14:08:19.000000 raster_basics-1.2.9/raster_basics.egg-info/not-zip-safe
--rw-r--r--   0 albinwells   (501) staff       (20)       14 2023-06-06 14:08:19.000000 raster_basics-1.2.9/raster_basics.egg-info/top_level.txt
--rw-rw-r--   0 albinwells   (501) staff       (20)       38 2023-06-06 14:08:19.691722 raster_basics-1.2.9/setup.cfg
--rw-rw-r--   0 albinwells   (501) staff       (20)      421 2023-06-06 14:07:49.000000 raster_basics-1.2.9/setup.py
+drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-06 14:11:21.015007 raster_basics-1.3.0/
+-rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-06 14:11:21.015071 raster_basics-1.3.0/PKG-INFO
+drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-06 14:11:21.014164 raster_basics-1.3.0/raster_basics/
+-rw-rw-r--   0 albinwells   (501) staff       (20)     8661 2023-02-27 17:09:17.000000 raster_basics-1.3.0/raster_basics/BaseFunctions.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)    42097 2023-06-01 21:15:30.000000 raster_basics-1.3.0/raster_basics/DataPlots.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)    17690 2023-06-02 17:27:11.000000 raster_basics-1.3.0/raster_basics/GlacierFunctions.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)    12235 2023-03-23 16:41:47.000000 raster_basics-1.3.0/raster_basics/RasterBasics.py
+-rwxrwxrwx   0 albinwells   (501) staff       (20)    12008 2023-06-06 14:10:42.000000 raster_basics-1.3.0/raster_basics/SmoothingFunctions.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)      574 2023-02-03 15:09:59.000000 raster_basics-1.3.0/raster_basics/__init__.py
+drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-06 14:11:21.014876 raster_basics-1.3.0/raster_basics.egg-info/
+-rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-06 14:11:20.000000 raster_basics-1.3.0/raster_basics.egg-info/PKG-INFO
+-rw-r--r--   0 albinwells   (501) staff       (20)      386 2023-06-06 14:11:20.000000 raster_basics-1.3.0/raster_basics.egg-info/SOURCES.txt
+-rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-06 14:11:20.000000 raster_basics-1.3.0/raster_basics.egg-info/dependency_links.txt
+-rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-06 14:11:20.000000 raster_basics-1.3.0/raster_basics.egg-info/not-zip-safe
+-rw-r--r--   0 albinwells   (501) staff       (20)       14 2023-06-06 14:11:20.000000 raster_basics-1.3.0/raster_basics.egg-info/top_level.txt
+-rw-rw-r--   0 albinwells   (501) staff       (20)       38 2023-06-06 14:11:21.015323 raster_basics-1.3.0/setup.cfg
+-rw-rw-r--   0 albinwells   (501) staff       (20)      421 2023-06-06 14:11:01.000000 raster_basics-1.3.0/setup.py
```

### Comparing `raster_basics-1.2.9/raster_basics/BaseFunctions.py` & `raster_basics-1.3.0/raster_basics/BaseFunctions.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.2.9/raster_basics/DataPlots.py` & `raster_basics-1.3.0/raster_basics/DataPlots.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.2.9/raster_basics/GlacierFunctions.py` & `raster_basics-1.3.0/raster_basics/GlacierFunctions.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.2.9/raster_basics/RasterBasics.py` & `raster_basics-1.3.0/raster_basics/RasterBasics.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.2.9/raster_basics/SmoothingFunctions.py` & `raster_basics-1.3.0/raster_basics/SmoothingFunctions.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         r = np.linalg.pinv(A)[2].reshape((window_size, -1))
         return scipy.signal.fftconvolve(Z, -r, mode='valid')
     elif derivative == 'both':
         c = np.linalg.pinv(A)[1].reshape((window_size, -1))
         r = np.linalg.pinv(A)[2].reshape((window_size, -1))
         return scipy.signal.fftconvolve(Z, -r, mode='valid'), scipy.signal.fftconvolve(Z, -c, mode='valid')
 
-def gaussianFilter(z, st_dev, truncate=4, fill_mode=‘constant’, fill_val=0):
+def gaussianFilter(z, st_dev, truncate=4, fill_mode='constant', fill_val=0):
     '''
     Gaussian smoothing filter
     :param z: input file (open, read raster file; array-like)
     :param st_dev: standard deviation for filter. higher value indicates greater blur
     :param fill_mode: parameter that determines how the input array is extended when the filter overlaps a border.
     :param fill_val: value to fill past edges of input if mode is ‘constant’. Default is 0.0.
     :return: new, smoothed array
```

### Comparing `raster_basics-1.2.9/raster_basics/__init__.py` & `raster_basics-1.3.0/raster_basics/__init__.py`

 * *Files identical despite different names*

