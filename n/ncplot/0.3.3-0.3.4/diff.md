# Comparing `tmp/ncplot-0.3.3.tar.gz` & `tmp/ncplot-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncplot-0.3.3.tar", last modified: Thu Jun  1 16:22:48 2023, max compression
+gzip compressed data, was "ncplot-0.3.4.tar", last modified: Tue Jun  6 17:18:18 2023, max compression
```

## Comparing `ncplot-0.3.3.tar` & `ncplot-0.3.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:22:48.786610 ncplot-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-01 16:22:33.000000 ncplot-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-01 16:22:33.000000 ncplot-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-06-01 16:22:48.786610 ncplot-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-01 16:22:33.000000 ncplot-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:22:48.786610 ncplot-0.3.3/ncplot/
--rwxr-xr-x   0 runner    (1001) docker     (123)       29 2023-06-01 16:22:33.000000 ncplot-0.3.3/ncplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-01 16:22:33.000000 ncplot-0.3.3/ncplot/command_line.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:22:33.000000 ncplot-0.3.3/ncplot/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)    35379 2023-06-01 16:22:33.000000 ncplot-0.3.3/ncplot/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-06-01 16:22:33.000000 ncplot-0.3.3/ncplot/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-01 16:22:33.000000 ncplot-0.3.3/ncplot/xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:22:48.786610 ncplot-0.3.3/ncplot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-01 16:22:48.000000 ncplot-0.3.3/ncplot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-01 16:22:33.000000 ncplot-0.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 16:22:48.786610 ncplot-0.3.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1952 2023-06-01 16:22:33.000000 ncplot-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:18:18.293346 ncplot-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-06 17:18:08.000000 ncplot-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-06 17:18:08.000000 ncplot-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-06-06 17:18:18.293346 ncplot-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-06 17:18:08.000000 ncplot-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:18:18.293346 ncplot-0.3.4/ncplot/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       29 2023-06-06 17:18:08.000000 ncplot-0.3.4/ncplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-06 17:18:08.000000 ncplot-0.3.4/ncplot/command_line.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:18:08.000000 ncplot-0.3.4/ncplot/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35927 2023-06-06 17:18:08.000000 ncplot-0.3.4/ncplot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-06-06 17:18:08.000000 ncplot-0.3.4/ncplot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-06 17:18:08.000000 ncplot-0.3.4/ncplot/xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:18:18.293346 ncplot-0.3.4/ncplot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-06 17:18:18.000000 ncplot-0.3.4/ncplot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-06 17:18:08.000000 ncplot-0.3.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 17:18:18.293346 ncplot-0.3.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1952 2023-06-06 17:18:08.000000 ncplot-0.3.4/setup.py
```

### Comparing `ncplot-0.3.3/LICENSE` & `ncplot-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ncplot-0.3.3/MANIFEST.in` & `ncplot-0.3.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ncplot-0.3.3/PKG-INFO` & `ncplot-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncplot
-Version: 0.3.3
+Version: 0.3.4
 Summary: Interactive viewing of NetCDF data
 Home-page: https://github.com/pmlmodelling/ncplot
 Author: Robert Wilson
 Author-email: rwi@pml.ac.uk
 Maintainer: Robert Wilson
 Project-URL: Bug Tracker, https://github.com/pmlmodelling/ncplot/issues
 Project-URL: Documentation, https://ncplot.readthedocs.io/en/stable
```

### Comparing `ncplot-0.3.3/README.md` & `ncplot-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `ncplot-0.3.3/ncplot/command_line.py` & `ncplot-0.3.4/ncplot/command_line.py`

 * *Files identical despite different names*

### Comparing `ncplot-0.3.3/ncplot/plot.py` & `ncplot-0.3.4/ncplot/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,23 +157,21 @@
         return True
     if "ipykernel" in sys.modules:
         return True
 
     if "spyder" in sys.modules:
         return False
 
-    if 'debugpy' in sys.modules:
-        return False
-
     return "ipykernel" in sys.modules
 
 
 def view(x, vars=None, autoscale=True, out=None, **kwargs):
     """
     Plot the contents of a NetCDF out
+
     Parameters
     -------------
     x : object or str
         xarray object or file  path
     vars : list or str
         Variables you want to plot. Everything will be plotted if this is not supplied
 
@@ -213,18 +211,24 @@
         xr_file = False
 
     nc_vars = None
     if xr_file is False:
         try:
             try:
                 import nctoolkit as nc
+                warnings.warn("Checking if nctoolkit is available")
 
-                ds = nc.open_data(x)
-                nc_vars = ds.variables
-                ds = ds.to_xarray()
+                if os.path.exists(x):
+                    ds = nc.open_data(x)
+                    nc_vars = ds.variables
+                    ds = ds.to_xarray()
+                else:
+                    ds = nc.open_thredds(x)
+                    nc_vars = ds.variables
+                    ds = ds.to_xarray()
             except:
                 ds = xr.open_dataset(x)
         except:
             ds = xr.open_dataset(x, decode_times=False)
             warnings.warn("Warning: xarray could not decode times!")
     else:
         ds = x
@@ -260,14 +264,18 @@
         if "long_name" in ds[lon_name].attrs:
             if "rotate" in ds[lon_name].long_name:
                 coastline = False
 
             if "pole" in ds[lon_name].long_name:
                 coastline = False
 
+    bad = []
+
+
+
     if True:
         dims = list(ds.dims)
         coords = ds.coords
         coords_list = list(coords)
         selected = []
         for x in coords_list:
             selected += list(coords[x].dims)
@@ -286,14 +294,25 @@
                 if "long_name" in ds[lon_name].attrs:
                     if "rotate" in ds[lon_name].long_name:
                         coastline = False
 
                     if "pole" in ds[lon_name].long_name:
                         coastline = False
 
+    if lon_name is not None:
+        for vv in ds.variables:
+            if lon_name not in list(ds[vv].dims):
+                if lat_name not in list(ds[vv].dims):
+                    if "time" not in list(ds[vv].dims):
+                        bad += [vv]
+    
+        if len(bad) > 0:
+            ds = ds.drop(bad)
+
+
     if len([x for x in ds.coords if "lon" in x]) > len(
         [x for x in ds.dims if "lon" in x]
     ):
         coastline = False
 
     if quadmesh is False and lat_name is not None:
         lats = ds[lat_name].values
```

### Comparing `ncplot-0.3.3/ncplot/utils.py` & `ncplot-0.3.4/ncplot/utils.py`

 * *Files identical despite different names*

### Comparing `ncplot-0.3.3/setup.py` & `ncplot-0.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         ],
 }
 
 
 extras_require["complete"] = ["geoviews"]
 
 setup(name='ncplot',
-      version='0.3.3',
+      version='0.3.4',
       description=DESCRIPTION,
       long_description=long_description,
       long_description_content_type='text/markdown',
 
       python_requires='>=3.6.1',
 
       entry_points={
```

