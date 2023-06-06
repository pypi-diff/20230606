# Comparing `tmp/geopandas-0.8.2.tar.gz` & `tmp/geopandas-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geopandas-0.8.2.tar", last modified: Mon Jan 25 20:51:19 2021, max compression
+gzip compressed data, was "geopandas-0.9.0.tar", last modified: Sun Feb 28 21:10:40 2021, max compression
```

## Comparing `geopandas-0.8.2.tar` & `geopandas-0.9.0.tar`

### file list

```diff
@@ -1,87 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-25 20:51:19.116649 geopandas-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (116)     1504 2021-01-25 20:51:12.000000 geopandas-0.8.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (116)       72 2021-01-25 20:51:12.000000 geopandas-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)      890 2021-01-25 20:51:19.116649 geopandas-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     6436 2021-01-25 20:51:12.000000 geopandas-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-25 20:51:19.116649 geopandas-0.8.2/geopandas/
--rw-r--r--   0 runner    (1001) docker     (116)      969 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4511 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/_compat.py
--rw-r--r--   0 runner    (1001) docker     (116)     4083 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/_config.py
--rw-r--r--   0 runner    (1001) docker     (116)    25247 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/_vectorized.py
--rw-r--r--   0 runner    (1001) docker     (116)      471 2021-01-25 20:51:19.116649 geopandas-0.8.2/geopandas/_version.py
--rw-r--r--   0 runner    (1001) docker     (116)    33557 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/array.py
--rw-r--r--   0 runner    (1001) docker     (116)    32027 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/base.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-25 20:51:19.108649 geopandas-0.8.2/geopandas/datasets/
--rw-r--r--   0 runner    (1001) docker     (116)      958 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-25 20:51:19.112649 geopandas-0.8.2/geopandas/datasets/naturalearth_cities/
--rw-r--r--   0 runner    (1001) docker     (116)    32111 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/datasets/naturalearth_cities/naturalearth_cities.README.html
--rw-r--r--   0 runner    (1001) docker     (116)        5 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/datasets/naturalearth_cities/naturalearth_cities.VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (116)       10 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/datasets/naturalearth_cities/naturalearth_cities.cpg
--rw-r--r--   0 runner    (1001) docker     (116)    16427 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/datasets/naturalearth_cities/naturalearth_cities.dbf
--rw-r--r--   0 runner    (1001) docker     (116)      143 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/datasets/naturalearth_cities/naturalearth_cities.prj
--rw-r--r--   0 runner    (1001) docker     (116)     5756 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/datasets/naturalearth_cities/naturalearth_cities.shp
--rw-r--r--   0 runner    (1001) docker     (116)     1716 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/datasets/naturalearth_cities/naturalearth_cities.shx
--rw-r--r--   0 runner    (1001) docker     (116)      736 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/datasets/naturalearth_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-25 20:51:19.112649 geopandas-0.8.2/geopandas/datasets/naturalearth_lowres/
--rw-r--r--   0 runner    (1001) docker     (116)       10 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/datasets/naturalearth_lowres/naturalearth_lowres.cpg
--rw-r--r--   0 runner    (1001) docker     (116)    48869 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/datasets/naturalearth_lowres/naturalearth_lowres.dbf
--rw-r--r--   0 runner    (1001) docker     (116)      143 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/datasets/naturalearth_lowres/naturalearth_lowres.prj
--rw-r--r--   0 runner    (1001) docker     (116)   180924 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/datasets/naturalearth_lowres/naturalearth_lowres.shp
--rw-r--r--   0 runner    (1001) docker     (116)     1516 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/datasets/naturalearth_lowres/naturalearth_lowres.shx
--rw-r--r--   0 runner    (1001) docker     (116)   661032 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/datasets/nybb_16a.zip
--rw-r--r--   0 runner    (1001) docker     (116)    43017 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/geodataframe.py
--rw-r--r--   0 runner    (1001) docker     (116)    21730 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/geoseries.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-25 20:51:19.112649 geopandas-0.8.2/geopandas/io/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    14660 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/io/arrow.py
--rw-r--r--   0 runner    (1001) docker     (116)    12624 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/io/file.py
--rw-r--r--   0 runner    (1001) docker     (116)    12813 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/io/sql.py
--rw-r--r--   0 runner    (1001) docker     (116)    32150 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/plotting.py
--rw-r--r--   0 runner    (1001) docker     (116)    18590 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/sindex.py
--rw-r--r--   0 runner    (1001) docker     (116)     7222 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-25 20:51:19.116649 geopandas-0.8.2/geopandas/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1069 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    24032 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tests/test_array.py
--rw-r--r--   0 runner    (1001) docker     (116)      923 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tests/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (116)      781 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (116)    20610 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tests/test_crs.py
--rw-r--r--   0 runner    (1001) docker     (116)      312 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (116)     3039 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tests/test_dissolve.py
--rw-r--r--   0 runner    (1001) docker     (116)    14614 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tests/test_extension_array.py
--rw-r--r--   0 runner    (1001) docker     (116)     4989 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tests/test_geocode.py
--rw-r--r--   0 runner    (1001) docker     (116)    31856 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tests/test_geodataframe.py
--rw-r--r--   0 runner    (1001) docker     (116)    29386 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tests/test_geom_methods.py
--rw-r--r--   0 runner    (1001) docker     (116)    12680 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tests/test_geoseries.py
--rw-r--r--   0 runner    (1001) docker     (116)     2105 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tests/test_merge.py
--rw-r--r--   0 runner    (1001) docker     (116)    17733 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tests/test_overlay.py
--rw-r--r--   0 runner    (1001) docker     (116)    15381 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tests/test_pandas_methods.py
--rw-r--r--   0 runner    (1001) docker     (116)    55179 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (116)     1171 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tests/test_show_versions.py
--rw-r--r--   0 runner    (1001) docker     (116)    22394 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tests/test_sindex.py
--rw-r--r--   0 runner    (1001) docker     (116)     3268 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (116)     2504 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (116)     4235 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tests/util.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-25 20:51:19.116649 geopandas-0.8.2/geopandas/tools/
--rw-r--r--   0 runner    (1001) docker     (116)      329 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3289 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tools/_show_versions.py
--rw-r--r--   0 runner    (1001) docker     (116)     8129 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tools/clip.py
--rw-r--r--   0 runner    (1001) docker     (116)     1489 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tools/crs.py
--rw-r--r--   0 runner    (1001) docker     (116)     5757 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tools/geocoding.py
--rw-r--r--   0 runner    (1001) docker     (116)     8533 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tools/overlay.py
--rw-r--r--   0 runner    (1001) docker     (116)     6799 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tools/sjoin.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-25 20:51:19.116649 geopandas-0.8.2/geopandas/tools/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    13758 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tools/tests/test_clip.py
--rw-r--r--   0 runner    (1001) docker     (116)    18491 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tools/tests/test_sjoin.py
--rw-r--r--   0 runner    (1001) docker     (116)     2954 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tools/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (116)     1454 2021-01-25 20:51:12.000000 geopandas-0.8.2/geopandas/tools/util.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-25 20:51:19.108649 geopandas-0.8.2/geopandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      890 2021-01-25 20:51:19.000000 geopandas-0.8.2/geopandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2523 2021-01-25 20:51:19.000000 geopandas-0.8.2/geopandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-25 20:51:19.000000 geopandas-0.8.2/geopandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       43 2021-01-25 20:51:19.000000 geopandas-0.8.2/geopandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       10 2021-01-25 20:51:19.000000 geopandas-0.8.2/geopandas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      562 2021-01-25 20:51:19.116649 geopandas-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1940 2021-01-25 20:51:12.000000 geopandas-0.8.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)    65747 2021-01-25 20:51:12.000000 geopandas-0.8.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-28 21:10:40.387239 geopandas-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (116)     1504 2021-02-28 21:10:37.000000 geopandas-0.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       72 2021-02-28 21:10:37.000000 geopandas-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)      890 2021-02-28 21:10:40.387239 geopandas-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     6296 2021-02-28 21:10:37.000000 geopandas-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-28 21:10:40.391239 geopandas-0.9.0/geopandas/
+-rw-r--r--   0 runner    (1001) docker     (116)      969 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6385 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4083 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/_config.py
+-rw-r--r--   0 runner    (1001) docker     (116)    27301 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/_vectorized.py
+-rw-r--r--   0 runner    (1001) docker     (116)      471 2021-02-28 21:10:40.391239 geopandas-0.9.0/geopandas/_version.py
+-rw-r--r--   0 runner    (1001) docker     (116)    43316 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/array.py
+-rw-r--r--   0 runner    (1001) docker     (116)   111554 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/base.py
+-rw-r--r--   0 runner    (1001) docker     (116)      694 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-28 21:10:40.383239 geopandas-0.9.0/geopandas/datasets/
+-rw-r--r--   0 runner    (1001) docker     (116)     1161 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-28 21:10:40.383239 geopandas-0.9.0/geopandas/datasets/naturalearth_cities/
+-rw-r--r--   0 runner    (1001) docker     (116)    32111 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/datasets/naturalearth_cities/naturalearth_cities.README.html
+-rw-r--r--   0 runner    (1001) docker     (116)        5 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/datasets/naturalearth_cities/naturalearth_cities.VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       10 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/datasets/naturalearth_cities/naturalearth_cities.cpg
+-rw-r--r--   0 runner    (1001) docker     (116)    16427 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/datasets/naturalearth_cities/naturalearth_cities.dbf
+-rw-r--r--   0 runner    (1001) docker     (116)      143 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/datasets/naturalearth_cities/naturalearth_cities.prj
+-rw-r--r--   0 runner    (1001) docker     (116)     5756 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/datasets/naturalearth_cities/naturalearth_cities.shp
+-rw-r--r--   0 runner    (1001) docker     (116)     1716 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/datasets/naturalearth_cities/naturalearth_cities.shx
+-rw-r--r--   0 runner    (1001) docker     (116)      736 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/datasets/naturalearth_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-28 21:10:40.383239 geopandas-0.9.0/geopandas/datasets/naturalearth_lowres/
+-rw-r--r--   0 runner    (1001) docker     (116)       10 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/datasets/naturalearth_lowres/naturalearth_lowres.cpg
+-rw-r--r--   0 runner    (1001) docker     (116)    48869 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/datasets/naturalearth_lowres/naturalearth_lowres.dbf
+-rw-r--r--   0 runner    (1001) docker     (116)      143 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/datasets/naturalearth_lowres/naturalearth_lowres.prj
+-rw-r--r--   0 runner    (1001) docker     (116)   180924 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/datasets/naturalearth_lowres/naturalearth_lowres.shp
+-rw-r--r--   0 runner    (1001) docker     (116)     1516 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/datasets/naturalearth_lowres/naturalearth_lowres.shx
+-rw-r--r--   0 runner    (1001) docker     (116)   661032 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/datasets/nybb_16a.zip
+-rw-r--r--   0 runner    (1001) docker     (116)    64184 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/geodataframe.py
+-rw-r--r--   0 runner    (1001) docker     (116)    40294 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/geoseries.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-28 21:10:40.383239 geopandas-0.9.0/geopandas/io/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14773 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/io/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13697 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/io/file.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14124 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/io/sql.py
+-rw-r--r--   0 runner    (1001) docker     (116)    36526 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (116)    21858 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/sindex.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9486 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-28 21:10:40.387239 geopandas-0.9.0/geopandas/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-28 21:10:40.387239 geopandas-0.9.0/geopandas/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (116)      506 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/data/null_geom.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)     1153 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    26836 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (116)      923 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (116)      781 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (116)    21680 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_crs.py
+-rw-r--r--   0 runner    (1001) docker     (116)      312 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9283 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_dissolve.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15258 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_extension_array.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5410 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_geocode.py
+-rw-r--r--   0 runner    (1001) docker     (116)    35283 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_geodataframe.py
+-rw-r--r--   0 runner    (1001) docker     (116)    37334 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_geom_methods.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16325 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_geoseries.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2105 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_merge.py
+-rw-r--r--   0 runner    (1001) docker     (116)    20148 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17336 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_pandas_methods.py
+-rw-r--r--   0 runner    (1001) docker     (116)    64812 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1171 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_show_versions.py
+-rw-r--r--   0 runner    (1001) docker     (116)    27341 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_sindex.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3774 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2504 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4235 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-28 21:10:40.387239 geopandas-0.9.0/geopandas/tools/
+-rw-r--r--   0 runner    (1001) docker     (116)      329 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3307 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tools/_show_versions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8098 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tools/clip.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1489 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tools/crs.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5897 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tools/geocoding.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13373 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tools/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11220 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tools/sjoin.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-28 21:10:40.387239 geopandas-0.9.0/geopandas/tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14652 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tools/tests/test_clip.py
+-rw-r--r--   0 runner    (1001) docker     (116)    18421 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tools/tests/test_sjoin.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2954 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tools/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1454 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tools/util.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-28 21:10:40.383239 geopandas-0.9.0/geopandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      890 2021-02-28 21:10:40.000000 geopandas-0.9.0/geopandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2584 2021-02-28 21:10:40.000000 geopandas-0.9.0/geopandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-28 21:10:40.000000 geopandas-0.9.0/geopandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       53 2021-02-28 21:10:40.000000 geopandas-0.9.0/geopandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       10 2021-02-28 21:10:40.000000 geopandas-0.9.0/geopandas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      562 2021-02-28 21:10:40.387239 geopandas-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1993 2021-02-28 21:10:37.000000 geopandas-0.9.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (116)    65747 2021-02-28 21:10:37.000000 geopandas-0.9.0/versioneer.py
```

### Comparing `geopandas-0.8.2/LICENSE.txt` & `geopandas-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geopandas-0.8.2/PKG-INFO` & `geopandas-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: geopandas
-Version: 0.8.2
+Version: 0.9.0
 Summary: Geographic pandas extensions
 Home-page: http://geopandas.org
 Author: GeoPandas contributors
 Author-email: kjordahl@alum.mit.edu
 License: BSD
 Description: GeoPandas is a project to add support for geographic data to
         `pandas`_ objects.
@@ -16,8 +16,8 @@
         operations in python that would otherwise require a spatial database
         such as PostGIS.
         
         .. _pandas: http://pandas.pydata.org
         .. _shapely: http://shapely.readthedocs.io/en/latest/
         
 Platform: UNKNOWN
-Requires-Python: >=3.5
+Requires-Python: >=3.6
```

### Comparing `geopandas-0.8.2/README.md` & `geopandas-0.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-GeoPandas [![build status](https://secure.travis-ci.org/geopandas/geopandas.png?branch=master)](https://travis-ci.org/geopandas/geopandas) [![Coverage Status](https://codecov.io/gh/geopandas/geopandas/branch/master/graph/badge.svg)](https://codecov.io/gh/geopandas/geopandas) [![Join the chat at https://gitter.im/geopandas/geopandas](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/geopandas/geopandas?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/geopandas/geopandas/master) [![DOI](https://zenodo.org/badge/11002815.svg)](https://zenodo.org/badge/latestdoi/11002815)
+GeoPandas [![Actions Status](https://github.com/geopandas/geopandas/workflows/Tests/badge.svg)](https://github.com/geopandas/geopandas/actions?query=workflow%3ATests) [![Coverage Status](https://codecov.io/gh/geopandas/geopandas/branch/master/graph/badge.svg)](https://codecov.io/gh/geopandas/geopandas) [![Join the chat at https://gitter.im/geopandas/geopandas](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/geopandas/geopandas?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/geopandas/geopandas/master) [![DOI](https://zenodo.org/badge/11002815.svg)](https://zenodo.org/badge/latestdoi/11002815)
 =========
 
 Python tools for geographic data
 
 Introduction
 ------------
 
@@ -32,15 +32,15 @@
 for all details. GeoPandas depends on the following packages:
 
 - ``pandas``
 - ``shapely``
 - ``fiona``
 - ``pyproj``
 
-Further, ``descartes`` and ``matplotlib`` are optional dependencies, required
+Further, ``matplotlib`` is an optional dependency, required
 for plotting, and [``rtree``](https://github.com/Toblerity/rtree) is an optional
 dependency, required for spatial joins. ``rtree`` requires the C library [``libspatialindex``](https://github.com/libspatialindex/libspatialindex).
 
 Those packages depend on several low-level libraries for geospatial analysis, which can be a challenge to install. Therefore, we recommend to install GeoPandas using the [conda package manager](https://conda.io/en/latest/). See the [installation docs](https://geopandas.readthedocs.io/en/latest/install.html) for more details.
 
 
 Get in touch
@@ -63,15 +63,15 @@
     >>> g = geopandas.GeoSeries([p1, p2, p3])
     >>> g
     0         POLYGON ((0 0, 1 0, 1 1, 0 0))
     1    POLYGON ((0 0, 1 0, 1 1, 0 1, 0 0))
     2    POLYGON ((2 0, 3 0, 3 1, 2 1, 2 0))
     dtype: geometry
 
-![Example 1](examples/test.png)
+![Example 1](doc/source/gallery/test.png)
 
 Some geographic operations return normal pandas object.  The `area` property of a `GeoSeries` will return a `pandas.Series` containing the area of each item in the `GeoSeries`:
 
     >>> print(g.area)
     0    0.5
     1    1.0
     2    1.0
@@ -81,48 +81,50 @@
 
     >>> g.buffer(0.5)
     0    POLYGON ((-0.3535533905932737 0.35355339059327...
     1    POLYGON ((-0.5 0, -0.5 1, -0.4975923633360985 ...
     2    POLYGON ((1.5 0, 1.5 1, 1.502407636663901 1.04...
     dtype: geometry
 
-![Example 2](examples/test_buffer.png)
+![Example 2](doc/source/gallery/test_buffer.png)
 
-GeoPandas objects also know how to plot themselves.  GeoPandas uses [descartes](https://pypi.python.org/pypi/descartes) to generate a [matplotlib](http://matplotlib.org) plot. To generate a plot of our GeoSeries, use:
+GeoPandas objects also know how to plot themselves. GeoPandas uses
+[matplotlib](http://matplotlib.org) for plotting. To generate a plot of our
+GeoSeries, use:
 
     >>> g.plot()
 
 GeoPandas also implements alternate constructors that can read any data format recognized by [fiona](http://fiona.readthedocs.io/en/latest/). To read a zip file containing an ESRI shapefile with the [boroughs boundaries of New York City](https://data.cityofnewyork.us/City-Government/Borough-Boundaries/tqmj-j8zm) (GeoPandas includes this as an example dataset):
 
     >>> nybb_path = geopandas.datasets.get_path('nybb')
     >>> boros = geopandas.read_file(nybb_path)
     >>> boros.set_index('BoroCode', inplace=True)
     >>> boros.sort_index(inplace=True)
     >>> boros
                    BoroName     Shape_Leng    Shape_Area  \
-    BoroCode                                               
-    1             Manhattan  359299.096471  6.364715e+08   
-    2                 Bronx  464392.991824  1.186925e+09   
-    3              Brooklyn  741080.523166  1.937479e+09   
-    4                Queens  896344.047763  3.045213e+09   
-    5         Staten Island  330470.010332  1.623820e+09   
-    
-                                                       geometry  
-    BoroCode                                                     
-    1         MULTIPOLYGON (((981219.0557861328 188655.31579...  
-    2         MULTIPOLYGON (((1012821.805786133 229228.26458...  
-    3         MULTIPOLYGON (((1021176.479003906 151374.79699...  
-    4         MULTIPOLYGON (((1029606.076599121 156073.81420...  
-    5         MULTIPOLYGON (((970217.0223999023 145643.33221...  
+    BoroCode
+    1             Manhattan  359299.096471  6.364715e+08
+    2                 Bronx  464392.991824  1.186925e+09
+    3              Brooklyn  741080.523166  1.937479e+09
+    4                Queens  896344.047763  3.045213e+09
+    5         Staten Island  330470.010332  1.623820e+09
+
+                                                       geometry
+    BoroCode
+    1         MULTIPOLYGON (((981219.0557861328 188655.31579...
+    2         MULTIPOLYGON (((1012821.805786133 229228.26458...
+    3         MULTIPOLYGON (((1021176.479003906 151374.79699...
+    4         MULTIPOLYGON (((1029606.076599121 156073.81420...
+    5         MULTIPOLYGON (((970217.0223999023 145643.33221...
 
-![New York City boroughs](examples/nyc.png)
+![New York City boroughs](doc/source/gallery/nyc.png)
 
     >>> boros['geometry'].convex_hull
     BoroCode
     1    POLYGON ((977855.4451904297 188082.3223876953,...
     2    POLYGON ((1017949.977600098 225426.8845825195,...
     3    POLYGON ((988872.8212280273 146772.0317993164,...
     4    POLYGON ((1000721.531799316 136681.776184082, ...
     5    POLYGON ((915517.6877458114 120121.8812543372,...
     dtype: geometry
 
-![Convex hulls of New York City boroughs](examples/nyc_hull.png)
+![Convex hulls of New York City boroughs](doc/source/gallery/nyc_hull.png)
```

### Comparing `geopandas-0.8.2/geopandas/__init__.py` & `geopandas-0.9.0/geopandas/__init__.py`

 * *Files identical despite different names*

### Comparing `geopandas-0.8.2/geopandas/_config.py` & `geopandas-0.9.0/geopandas/_config.py`

 * *Files identical despite different names*

### Comparing `geopandas-0.8.2/geopandas/_vectorized.py` & `geopandas-0.9.0/geopandas/_vectorized.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,15 +98,16 @@
     """
     # First try a fast path for pygeos if possible, but do this in a try-except
     # block because pygeos.from_shapely only handles Shapely objects, while
     # the rest of this function is more forgiving (also __geo_interface__).
     if compat.USE_PYGEOS and compat.PYGEOS_SHAPELY_COMPAT:
         if not isinstance(data, np.ndarray):
             arr = np.empty(len(data), dtype=object)
-            arr[:] = data
+            with compat.ignore_shapely2_warnings():
+                arr[:] = data
         else:
             arr = data
         try:
             return pygeos.from_shapely(arr)
         except TypeError:
             pass
 
@@ -117,18 +118,15 @@
             out.append(geom)
         elif isinstance(geom, BaseGeometry):
             if compat.USE_PYGEOS:
                 out.append(_shapely_to_pygeos(geom))
             else:
                 out.append(geom)
         elif hasattr(geom, "__geo_interface__"):
-            geom = shapely.geometry.asShape(geom)
-            # asShape returns GeometryProxy -> trigger actual materialization
-            # with one of its methods
-            geom.wkb
+            geom = shapely.geometry.shape(geom)
             if compat.USE_PYGEOS:
                 out.append(_shapely_to_pygeos(geom))
             else:
                 out.append(geom)
         elif _isna(geom):
             out.append(None)
         else:
@@ -136,22 +134,24 @@
 
     if compat.USE_PYGEOS:
         return np.array(out, dtype=object)
     else:
         # numpy can expand geometry collections into 2D arrays, use this
         # two-step construction to avoid this
         aout = np.empty(len(data), dtype=object)
-        aout[:] = out
+        with compat.ignore_shapely2_warnings():
+            aout[:] = out
         return aout
 
 
 def to_shapely(data):
     if compat.USE_PYGEOS:
         out = np.empty(len(data), dtype=object)
-        out[:] = [_pygeos_to_shapely(geom) for geom in data]
+        with compat.ignore_shapely2_warnings():
+            out[:] = [_pygeos_to_shapely(geom) for geom in data]
         return out
     else:
         return data
 
 
 def from_wkb(data):
     """
@@ -168,21 +168,22 @@
         if geom is not None and len(geom):
             geom = shapely.wkb.loads(geom)
         else:
             geom = None
         out.append(geom)
 
     aout = np.empty(len(data), dtype=object)
-    aout[:] = out
+    with compat.ignore_shapely2_warnings():
+        aout[:] = out
     return aout
 
 
-def to_wkb(data, hex=False):
+def to_wkb(data, hex=False, **kwargs):
     if compat.USE_PYGEOS:
-        return pygeos.to_wkb(data, hex=hex)
+        return pygeos.to_wkb(data, hex=hex, **kwargs)
     else:
         if hex:
             out = [geom.wkb_hex if geom is not None else None for geom in data]
         else:
             out = [geom.wkb if geom is not None else None for geom in data]
         return np.array(out, dtype=object)
 
@@ -204,15 +205,16 @@
                 geom = geom.decode("utf-8")
             geom = shapely.wkt.loads(geom)
         else:
             geom = None
         out.append(geom)
 
     aout = np.empty(len(data), dtype=object)
-    aout[:] = out
+    with compat.ignore_shapely2_warnings():
+        aout[:] = out
     return aout
 
 
 def to_wkt(data, **kwargs):
     if compat.USE_PYGEOS:
         return pygeos.to_wkt(data, **kwargs)
     else:
@@ -259,15 +261,15 @@
     if isinstance(right, BaseGeometry):
         right = from_shapely([right])[0]
     return getattr(pygeos, op)(left, right, **kwargs)
 
 
 def _binary_geo(op, left, right):
     # type: (str, np.array[geoms], [np.array[geoms]/BaseGeometry]) -> np.array[geoms]
-    """ Apply geometry-valued operation
+    """Apply geometry-valued operation
 
     Supports:
 
     -   difference
     -   symmetric_difference
     -   intersection
     -   union
@@ -277,32 +279,34 @@
     op: string
     right: np.array[geoms] or single shapely BaseGeoemtry
     """
     if isinstance(right, BaseGeometry):
         # intersection can return empty GeometryCollections, and if the
         # result are only those, numpy will coerce it to empty 2D array
         data = np.empty(len(left), dtype=object)
-        data[:] = [
-            getattr(s, op)(right) if s is not None and right is not None else None
-            for s in left
-        ]
+        with compat.ignore_shapely2_warnings():
+            data[:] = [
+                getattr(s, op)(right) if s is not None and right is not None else None
+                for s in left
+            ]
         return data
     elif isinstance(right, np.ndarray):
         if len(left) != len(right):
             msg = "Lengths of inputs do not match. Left: {0}, Right: {1}".format(
                 len(left), len(right)
             )
             raise ValueError(msg)
         data = np.empty(len(left), dtype=object)
-        data[:] = [
-            getattr(this_elem, op)(other_elem)
-            if this_elem is not None and other_elem is not None
-            else None
-            for this_elem, other_elem in zip(left, right)
-        ]
+        with compat.ignore_shapely2_warnings():
+            data[:] = [
+                getattr(this_elem, op)(other_elem)
+                if this_elem is not None and other_elem is not None
+                else None
+                for this_elem, other_elem in zip(left, right)
+            ]
         return data
     else:
         raise TypeError("Type not known: {0} vs {1}".format(type(left), type(right)))
 
 
 def _binary_predicate(op, left, right, *args, **kwargs):
     # type: (str, np.array[geoms], np.array[geoms]/BaseGeometry, args/kwargs)
@@ -428,15 +432,16 @@
     for geom in left:
         if geom is None or geom.is_empty:
             res = geom
         else:
             res = getattr(shapely.affinity, op)(geom, *args, **kwargs)
         out.append(res)
     data = np.empty(len(left), dtype=object)
-    data[:] = out
+    with compat.ignore_shapely2_warnings():
+        data[:] = out
     return from_shapely(data)
 
 
 # -----------------------------------------------------------------------------
 # Vectorized operations
 # -----------------------------------------------------------------------------
 
@@ -471,31 +476,36 @@
     if compat.USE_PYGEOS:
         return pygeos.is_simple(data)
     else:
         return _unary_op("is_simple", data, null_value=False)
 
 
 def is_ring(data):
+    if "Polygon" in geom_type(data):
+        warnings.warn(
+            "is_ring currently returns True for Polygons, which is not correct. "
+            "This will be corrected to False in a future release.",
+            FutureWarning,
+            stacklevel=3,
+        )
     if compat.USE_PYGEOS:
-        return pygeos.is_ring(pygeos.get_exterior_ring(data))
+        return pygeos.is_ring(data) | pygeos.is_ring(pygeos.get_exterior_ring(data))
     else:
-        # operates on the exterior, so can't use _unary_op()
-        # XXX needed to change this because there is now a geometry collection
-        # in the shapely ones that was something else before?
-        return np.array(
-            [
-                geom.exterior.is_ring
-                if geom is not None
-                and hasattr(geom, "exterior")
-                and geom.exterior is not None
-                else False
-                for geom in data
-            ],
-            dtype=bool,
-        )
+        # for polygons operates on the exterior, so can't use _unary_op()
+        results = []
+        for geom in data:
+            if geom is None:
+                results.append(False)
+            elif geom.type == "Polygon":
+                results.append(geom.exterior.is_ring)
+            elif geom.type in ["LineString", "LinearRing"]:
+                results.append(geom.is_ring)
+            else:
+                results.append(False)
+        return np.array(results, dtype=bool)
 
 
 def is_closed(data):
     if compat.USE_PYGEOS:
         return pygeos.is_closed(data)
     else:
         return _unary_op("is_closed", data, null_value=False)
@@ -536,15 +546,16 @@
 
 
 def _unary_geo(op, left, *args, **kwargs):
     # type: (str, np.array[geoms]) -> np.array[geoms]
     """Unary operation that returns new geometries"""
     # ensure 1D output, see note above
     data = np.empty(len(left), dtype=object)
-    data[:] = [getattr(geom, op, None) for geom in left]
+    with compat.ignore_shapely2_warnings():
+        data[:] = [getattr(geom, op, None) for geom in left]
     return data
 
 
 def boundary(data):
     if compat.USE_PYGEOS:
         return pygeos.boundary(data)
     else:
@@ -758,24 +769,30 @@
         if isinstance(distance, np.ndarray):
             if len(distance) != len(data):
                 raise ValueError(
                     "Length of distance sequence does not match "
                     "length of the GeoSeries"
                 )
 
-            out[:] = [
-                geom.buffer(dist, resolution, **kwargs) if geom is not None else None
-                for geom, dist in zip(data, distance)
-            ]
+            with compat.ignore_shapely2_warnings():
+                out[:] = [
+                    geom.buffer(dist, resolution, **kwargs)
+                    if geom is not None
+                    else None
+                    for geom, dist in zip(data, distance)
+                ]
             return out
 
-        out[:] = [
-            geom.buffer(distance, resolution, **kwargs) if geom is not None else None
-            for geom in data
-        ]
+        with compat.ignore_shapely2_warnings():
+            out[:] = [
+                geom.buffer(distance, resolution, **kwargs)
+                if geom is not None
+                else None
+                for geom in data
+            ]
         return out
 
 
 def interpolate(data, distance, normalized=False):
     if compat.USE_PYGEOS:
         return pygeos.line_interpolate_point(data, distance, normalize=normalized)
     else:
@@ -799,18 +816,47 @@
 def simplify(data, tolerance, preserve_topology=True):
     if compat.USE_PYGEOS:
         # preserve_topology has different default as pygeos!
         return pygeos.simplify(data, tolerance, preserve_topology=preserve_topology)
     else:
         # method and not a property -> can't use _unary_geo
         out = np.empty(len(data), dtype=object)
-        out[:] = [
-            geom.simplify(tolerance, preserve_topology=preserve_topology)
-            for geom in data
-        ]
+        with compat.ignore_shapely2_warnings():
+            out[:] = [
+                geom.simplify(tolerance, preserve_topology=preserve_topology)
+                for geom in data
+            ]
+        return out
+
+
+def _shapely_normalize(geom):
+    """
+    Small helper function for now because it is not yet available in Shapely.
+    """
+    from shapely.geos import lgeos
+    from shapely.geometry.base import geom_factory
+    from ctypes import c_void_p, c_int
+
+    lgeos._lgeos.GEOSNormalize_r.restype = c_int
+    lgeos._lgeos.GEOSNormalize_r.argtypes = [c_void_p, c_void_p]
+
+    geom_cloned = lgeos.GEOSGeom_clone(geom._geom)
+    lgeos._lgeos.GEOSNormalize_r(lgeos.geos_handle, geom_cloned)
+    return geom_factory(geom_cloned)
+
+
+def normalize(data):
+    if compat.USE_PYGEOS:
+        return pygeos.normalize(data)
+    else:
+        out = np.empty(len(data), dtype=object)
+        with compat.ignore_shapely2_warnings():
+            out[:] = [
+                _shapely_normalize(geom) if geom is not None else None for geom in data
+            ]
         return out
 
 
 def project(data, other, normalized=False):
     if compat.USE_PYGEOS:
         return pygeos.line_locate_point(data, other, normalize=normalized)
     else:
@@ -846,14 +892,22 @@
 def get_y(data):
     if compat.USE_PYGEOS:
         return pygeos.get_y(data)
     else:
         return _unary_op("y", data, null_value=np.nan)
 
 
+def get_z(data):
+    if compat.USE_PYGEOS:
+        return pygeos.get_z(data)
+    else:
+        data = [geom.z if geom.has_z else np.nan for geom in data]
+        return np.array(data, dtype=np.dtype(float))
+
+
 def bounds(data):
     if compat.USE_PYGEOS:
         return pygeos.bounds(data)
     # ensure that for empty arrays, the result has the correct shape
     if len(data) == 0:
         return np.empty((0, 4), dtype="float64")
     # need to explicitly check for empty (in addition to missing) geometries,
@@ -883,10 +937,13 @@
     else:
         from shapely.ops import transform
 
         n = len(data)
         result = np.empty(n, dtype=object)
         for i in range(n):
             geom = data[i]
-            result[i] = transform(func, geom)
+            if _isna(geom):
+                result[i] = geom
+            else:
+                result[i] = transform(func, geom)
 
         return result
```

### Comparing `geopandas-0.8.2/geopandas/array.py` & `geopandas-0.9.0/geopandas/array.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,31 +2,36 @@
 import numbers
 import operator
 import warnings
 import inspect
 
 import numpy as np
 import pandas as pd
-from pandas.api.extensions import ExtensionArray, ExtensionDtype
+from pandas.api.extensions import (
+    ExtensionArray,
+    ExtensionDtype,
+    register_extension_dtype,
+)
 
 import shapely
 import shapely.affinity
 import shapely.geometry
 from shapely.geometry.base import BaseGeometry
 import shapely.ops
 import shapely.wkt
-from pyproj import CRS
+from pyproj import CRS, Transformer
 
 try:
     import pygeos
 except ImportError:
     geos = None
 
 from . import _compat as compat
 from . import _vectorized as vectorized
+from .sindex import _get_sindex_class
 
 
 class GeometryDtype(ExtensionDtype):
     type = BaseGeometry
     name = "geometry"
     na_value = np.nan
 
@@ -44,18 +49,15 @@
             )
 
     @classmethod
     def construct_array_type(cls):
         return GeometryArray
 
 
-if compat.PANDAS_GE_024:
-    from pandas.api.extensions import register_extension_dtype
-
-    register_extension_dtype(GeometryDtype)
+register_extension_dtype(GeometryDtype)
 
 
 def _isna(value):
     """
     Check if scalar value is NA-like (None, np.nan or pd.NA).
 
     Custom version that only works for scalars (returning True or False),
@@ -138,15 +140,15 @@
         return geom
     else:
         return vectorized._shapely_to_pygeos(geom)
 
 
 def _is_scalar_geometry(geom):
     if compat.USE_PYGEOS:
-        return isinstance(geom, pygeos.Geometry)
+        return isinstance(geom, (pygeos.Geometry, BaseGeometry))
     else:
         return isinstance(geom, BaseGeometry)
 
 
 def from_shapely(data, crs=None):
     """
     Convert a list or array of shapely objects to a GeometryArray.
@@ -188,21 +190,21 @@
         :meth:`pyproj.CRS.from_user_input() <pyproj.crs.CRS.from_user_input>`,
         such as an authority string (eg "EPSG:4326") or a WKT string.
 
     """
     return GeometryArray(vectorized.from_wkb(data), crs=crs)
 
 
-def to_wkb(geoms, hex=False):
+def to_wkb(geoms, hex=False, **kwargs):
     """
     Convert GeometryArray to a numpy object array of WKB objects.
     """
     if not isinstance(geoms, GeometryArray):
         raise ValueError("'geoms' must be a GeometryArray")
-    return vectorized.to_wkb(geoms.data, hex=hex)
+    return vectorized.to_wkb(geoms.data, hex=hex, **kwargs)
 
 
 def from_wkt(data, crs=None):
     """
     Convert a list or array of WKT objects to a GeometryArray.
 
     Parameters
@@ -227,28 +229,48 @@
     return vectorized.to_wkt(geoms.data, **kwargs)
 
 
 def points_from_xy(x, y, z=None, crs=None):
     """
     Generate GeometryArray of shapely Point geometries from x, y(, z) coordinates.
 
+    In case of geographic coordinates, it is assumed that longitude is captured by
+    ``x`` coordinates and latitude by ``y``.
+
     Parameters
     ----------
     x, y, z : iterable
     crs : value, optional
         Coordinate Reference System of the geometry objects. Can be anything accepted by
         :meth:`pyproj.CRS.from_user_input() <pyproj.crs.CRS.from_user_input>`,
         such as an authority string (eg "EPSG:4326") or a WKT string.
 
     Examples
     --------
+    >>> import pandas as pd
+    >>> df = pd.DataFrame({'x': [0, 1, 2], 'y': [0, 1, 2], 'z': [0, 1, 2]})
+    >>> df
+       x  y  z
+    0  0  0  0
+    1  1  1  1
+    2  2  2  2
     >>> geometry = geopandas.points_from_xy(x=[1, 0], y=[0, 1])
     >>> geometry = geopandas.points_from_xy(df['x'], df['y'], df['z'])
     >>> gdf = geopandas.GeoDataFrame(
-            df, geometry=geopandas.points_from_xy(df['x'], df['y']))
+    ...     df, geometry=geopandas.points_from_xy(df['x'], df['y']))
+
+    Having geographic coordinates:
+
+    >>> df = pd.DataFrame({'longitude': [-140, 0, 123], 'latitude': [-65, 1, 48]})
+    >>> df
+       longitude  latitude
+    0       -140       -65
+    1          0         1
+    2        123        48
+    >>> geometry = geopandas.points_from_xy(df.longitude, df.latitude, crs="EPSG:4326")
 
     Returns
     -------
     output : GeometryArray
     """
     return GeometryArray(vectorized.points_from_xy(x, y, z), crs=crs)
 
@@ -275,14 +297,45 @@
             raise ValueError(
                 "'data' should be a 1-dimensional array of geometry objects."
             )
         self.data = data
 
         self._crs = None
         self.crs = crs
+        self._sindex = None
+
+    @property
+    def sindex(self):
+        if self._sindex is None:
+            self._sindex = _get_sindex_class()(self.data)
+        return self._sindex
+
+    @property
+    def has_sindex(self):
+        """Check the existence of the spatial index without generating it.
+
+        Use the `.sindex` attribute on a GeoDataFrame or GeoSeries
+        to generate a spatial index if it does not yet exist,
+        which may take considerable time based on the underlying index
+        implementation.
+
+        Note that the underlying spatial index may not be fully
+        initialized until the first use.
+
+        See Also
+        ---------
+        GeoDataFrame.has_sindex
+
+        Returns
+        -------
+        bool
+            `True` if the spatial index has been generated or
+            `False` if not.
+        """
+        return self._sindex is not None
 
     @property
     def crs(self):
         """
         The Coordinate Reference System (CRS) represented as a ``pyproj.CRS``
         object.
 
@@ -352,45 +405,49 @@
                 value = None
             elif isinstance(value, BaseGeometry):
                 value = from_shapely([value]).data[0]
             else:
                 raise TypeError("should be valid geometry")
             if isinstance(key, (slice, list, np.ndarray)):
                 value_array = np.empty(1, dtype=object)
-                value_array[:] = [value]
+                with compat.ignore_shapely2_warnings():
+                    value_array[:] = [value]
                 self.data[key] = value_array
             else:
                 self.data[key] = value
         else:
             raise TypeError(
                 "Value should be either a BaseGeometry or None, got %s" % str(value)
             )
 
+        # invalidate spatial index
+        self._sindex = None
+
         # TODO: use this once pandas-dev/pandas#33457 is fixed
         # if hasattr(value, "crs"):
         #     if value.crs and (value.crs != self.crs):
         #         raise ValueError(
         #             "CRS mismatch between CRS of the passed geometries "
         #             "and CRS of existing geometries."
         #         )
 
-    if compat.USE_PYGEOS:
-
-        def __getstate__(self):
+    def __getstate__(self):
+        if compat.USE_PYGEOS:
             return (pygeos.to_wkb(self.data), self._crs)
+        else:
+            return self.__dict__
 
-        def __setstate__(self, state):
+    def __setstate__(self, state):
+        if compat.USE_PYGEOS:
             geoms = pygeos.from_wkb(state[0])
             self._crs = state[1]
+            self._sindex = None  # pygeos.STRtree could not be pickled yet
             self.data = geoms
             self.base = None
-
-    else:
-
-        def __setstate__(self, state):
+        else:
             if "_crs" not in state:
                 state["_crs"] = None
             self.__dict__.update(state)
 
     # -------------------------------------------------------------------------
     # Geometry related methods
     # -------------------------------------------------------------------------
@@ -647,14 +704,176 @@
         return GeometryArray(
             vectorized._affinity_method(
                 "skew", self.data, xs, ys, origin=origin, use_radians=use_radians
             ),
             crs=self.crs,
         )
 
+    def to_crs(self, crs=None, epsg=None):
+        """Returns a ``GeometryArray`` with all geometries transformed to a new
+        coordinate reference system.
+
+        Transform all geometries in a GeometryArray to a different coordinate
+        reference system.  The ``crs`` attribute on the current GeometryArray must
+        be set.  Either ``crs`` or ``epsg`` may be specified for output.
+
+        This method will transform all points in all objects.  It has no notion
+        or projecting entire geometries.  All segments joining points are
+        assumed to be lines in the current projection, not geodesics.  Objects
+        crossing the dateline (or other projection boundary) will have
+        undesirable behavior.
+
+        Parameters
+        ----------
+        crs : pyproj.CRS, optional if `epsg` is specified
+            The value can be anything accepted
+            by :meth:`pyproj.CRS.from_user_input() <pyproj.crs.CRS.from_user_input>`,
+            such as an authority string (eg "EPSG:4326") or a WKT string.
+        epsg : int, optional if `crs` is specified
+            EPSG code specifying output projection.
+
+        Returns
+        -------
+        GeometryArray
+
+        Examples
+        --------
+        >>> from shapely.geometry import Point
+        >>> from geopandas.array import from_shapely, to_wkt
+        >>> a = from_shapely([Point(1, 1), Point(2, 2), Point(3, 3)], crs=4326)
+        >>> to_wkt(a)
+        array(['POINT (1 1)', 'POINT (2 2)', 'POINT (3 3)'], dtype=object)
+        >>> a.crs  # doctest: +SKIP
+        <Geographic 2D CRS: EPSG:4326>
+        Name: WGS 84
+        Axis Info [ellipsoidal]:
+        - Lat[north]: Geodetic latitude (degree)
+        - Lon[east]: Geodetic longitude (degree)
+        Area of Use:
+        - name: World
+        - bounds: (-180.0, -90.0, 180.0, 90.0)
+        Datum: World Geodetic System 1984
+        - Ellipsoid: WGS 84
+        - Prime Meridian: Greenwich
+
+        >>> a = a.to_crs(3857)
+        >>> to_wkt(a)
+        array(['POINT (111319 111325)', 'POINT (222639 222684)',
+               'POINT (333958 334111)'], dtype=object)
+        >>> a.crs  # doctest: +SKIP
+        <Projected CRS: EPSG:3857>
+        Name: WGS 84 / Pseudo-Mercator
+        Axis Info [cartesian]:
+        - X[east]: Easting (metre)
+        - Y[north]: Northing (metre)
+        Area of Use:
+        - name: World - 85°S to 85°N
+        - bounds: (-180.0, -85.06, 180.0, 85.06)
+        Coordinate Operation:
+        - name: Popular Visualisation Pseudo-Mercator
+        - method: Popular Visualisation Pseudo Mercator
+        Datum: World Geodetic System 1984
+        - Ellipsoid: WGS 84
+        - Prime Meridian: Greenwich
+
+        """
+        if self.crs is None:
+            raise ValueError(
+                "Cannot transform naive geometries.  "
+                "Please set a crs on the object first."
+            )
+        if crs is not None:
+            crs = CRS.from_user_input(crs)
+        elif epsg is not None:
+            crs = CRS.from_epsg(epsg)
+        else:
+            raise ValueError("Must pass either crs or epsg.")
+
+        # skip if the input CRS and output CRS are the exact same
+        if self.crs.is_exact_same(crs):
+            return self
+
+        transformer = Transformer.from_crs(self.crs, crs, always_xy=True)
+
+        new_data = vectorized.transform(self.data, transformer.transform)
+        return GeometryArray(new_data, crs=crs)
+
+    def estimate_utm_crs(self, datum_name="WGS 84"):
+        """Returns the estimated UTM CRS based on the bounds of the dataset.
+
+        .. versionadded:: 0.9
+
+        .. note:: Requires pyproj 3+
+
+        Parameters
+        ----------
+        datum_name : str, optional
+            The name of the datum to use in the query. Default is WGS 84.
+
+        Returns
+        -------
+        pyproj.CRS
+
+        Examples
+        --------
+        >>> world = geopandas.read_file(
+        ...     geopandas.datasets.get_path("naturalearth_lowres")
+        ... )
+        >>> germany = world.loc[world.name == "Germany"]
+        >>> germany.geometry.values.estimate_utm_crs()  # doctest: +SKIP
+        <Projected CRS: EPSG:32632>
+        Name: WGS 84 / UTM zone 32N
+        Axis Info [cartesian]:
+        - E[east]: Easting (metre)
+        - N[north]: Northing (metre)
+        Area of Use:
+        - name: World - N hemisphere - 6°E to 12°E - by country
+        - bounds: (6.0, 0.0, 12.0, 84.0)
+        Coordinate Operation:
+        - name: UTM zone 32N
+        - method: Transverse Mercator
+        Datum: World Geodetic System 1984
+        - Ellipsoid: WGS 84
+        - Prime Meridian: Greenwich
+        """
+        try:
+            from pyproj.aoi import AreaOfInterest
+            from pyproj.database import query_utm_crs_info
+        except ImportError:
+            raise RuntimeError("pyproj 3+ required for estimate_utm_crs.")
+
+        if not self.crs:
+            raise RuntimeError("crs must be set to estimate UTM CRS.")
+
+        minx, miny, maxx, maxy = self.total_bounds
+        # ensure using geographic coordinates
+        if not self.crs.is_geographic:
+            lon, lat = Transformer.from_crs(
+                self.crs, "EPSG:4326", always_xy=True
+            ).transform((minx, maxx, minx, maxx), (miny, miny, maxy, maxy))
+            x_center = np.mean(lon)
+            y_center = np.mean(lat)
+        else:
+            x_center = np.mean([minx, maxx])
+            y_center = np.mean([miny, maxy])
+
+        utm_crs_list = query_utm_crs_info(
+            datum_name=datum_name,
+            area_of_interest=AreaOfInterest(
+                west_lon_degree=x_center,
+                south_lat_degree=y_center,
+                east_lon_degree=x_center,
+                north_lat_degree=y_center,
+            ),
+        )
+        try:
+            return CRS.from_epsg(utm_crs_list[0].code)
+        except IndexError:
+            raise RuntimeError("Unable to determine UTM CRS")
+
     #
     # Coordinate related properties
     #
 
     @property
     def x(self):
         """Return the x location of point geometries in a GeoSeries"""
@@ -670,14 +889,23 @@
         if (self.geom_type[~self.isna()] == "Point").all():
             return vectorized.get_y(self.data)
         else:
             message = "y attribute access only provided for Point geometries"
             raise ValueError(message)
 
     @property
+    def z(self):
+        """Return the z location of point geometries in a GeoSeries"""
+        if (self.geom_type[~self.isna()] == "Point").all():
+            return vectorized.get_z(self.data)
+        else:
+            message = "z attribute access only provided for Point geometries"
+            raise ValueError(message)
+
+    @property
     def bounds(self):
         return vectorized.bounds(self.data)
 
     @property
     def total_bounds(self):
         if len(self) == 0:
             # numpy 'min' cannot handle empty arrays
@@ -726,28 +954,30 @@
 
         result = take(self.data, indices, allow_fill=allow_fill, fill_value=fill_value)
         if allow_fill and fill_value is None:
             result[pd.isna(result)] = None
         return GeometryArray(result, crs=self.crs)
 
     def _fill(self, idx, value):
-        """ Fill index locations with value
+        """Fill index locations with value
 
         Value should be a BaseGeometry
         """
         if not (_is_scalar_geometry(value) or value is None):
             raise TypeError(
                 "Value should be either a BaseGeometry or None, got %s" % str(value)
             )
         # self.data[idx] = value
-        self.data[idx] = np.array([value], dtype=object)
+        value_arr = np.empty(1, dtype=object)
+        value_arr[:] = [value]
+        self.data[idx] = value_arr
         return self
 
     def fillna(self, value=None, method=None, limit=None):
-        """ Fill NA/NaN values using the specified method.
+        """Fill NA/NaN values using the specified method.
 
         Parameters
         ----------
         value : scalar, array-like
             If a scalar value is passed it is used to fill all missing values.
             Alternatively, an array-like 'value' can be given. It's expected
             that the array-like have the same length as 'self'.
@@ -843,14 +1073,49 @@
         _, uniques = factorize(self)
         return uniques
 
     @property
     def nbytes(self):
         return self.data.nbytes
 
+    def shift(self, periods=1, fill_value=None):
+        """
+        Shift values by desired number.
+
+        Newly introduced missing values are filled with
+        ``self.dtype.na_value``.
+
+        Parameters
+        ----------
+        periods : int, default 1
+            The number of periods to shift. Negative values are allowed
+            for shifting backwards.
+
+        fill_value : object, optional (default None)
+            The scalar value to use for newly introduced missing values.
+            The default is ``self.dtype.na_value``.
+
+        Returns
+        -------
+        GeometryArray
+            Shifted.
+
+        Notes
+        -----
+        If ``self`` is empty or ``periods`` is 0, a copy of ``self`` is
+        returned.
+
+        If ``periods > len(self)``, then an array of size
+        len(self) is returned, with all values filled with
+        ``self.dtype.na_value``.
+        """
+        shifted = super(GeometryArray, self).shift(periods, fill_value)
+        shifted.crs = self.crs
+        return shifted
+
     # -------------------------------------------------------------------------
     # ExtensionArray specific
     # -------------------------------------------------------------------------
 
     @classmethod
     def _from_sequence(cls, scalars, dtype=None, copy=False):
         """
@@ -908,15 +1173,15 @@
             The original ExtensionArray that factorize was called on.
 
         See Also
         --------
         pandas.factorize
         ExtensionArray.factorize
         """
-        return from_wkb(values)
+        return from_wkb(values, crs=original.crs)
 
     def _values_for_argsort(self):
         # type: () -> np.ndarray
         """Return values for sorting.
 
         Returns
         -------
@@ -957,15 +1222,17 @@
         if boxed:
             import geopandas
 
             precision = geopandas.options.display_precision
             if precision is None:
                 # dummy heuristic based on 10 first geometries that should
                 # work in most cases
-                xmin, ymin, xmax, ymax = self[~self.isna()][:10].total_bounds
+                with warnings.catch_warnings():
+                    warnings.simplefilter("ignore", category=RuntimeWarning)
+                    xmin, ymin, xmax, ymax = self[~self.isna()][:10].total_bounds
                 if (
                     (-180 <= xmin <= 180)
                     and (-180 <= xmax <= 180)
                     and (-90 <= ymin <= 90)
                     and (-90 <= ymax <= 90)
                 ):
                     # geographic coordinates
@@ -1013,21 +1280,23 @@
         -------
         values : numpy array
         """
         return to_shapely(self)
 
     def _binop(self, other, op):
         def convert_values(param):
-            if isinstance(param, ExtensionArray) or pd.api.types.is_list_like(param):
+            if not _is_scalar_geometry(param) and (
+                isinstance(param, ExtensionArray) or pd.api.types.is_list_like(param)
+            ):
                 ovalues = param
             else:  # Assume its an object
                 ovalues = [param] * len(self)
             return ovalues
 
-        if isinstance(other, (pd.Series, pd.Index)):
+        if isinstance(other, (pd.Series, pd.Index, pd.DataFrame)):
             # rely on pandas to unbox and dispatch to us
             return NotImplemented
 
         lvalues = self
         rvalues = convert_values(other)
 
         if len(lvalues) != len(rvalues):
@@ -1041,7 +1310,22 @@
         return res
 
     def __eq__(self, other):
         return self._binop(other, operator.eq)
 
     def __ne__(self, other):
         return self._binop(other, operator.ne)
+
+    def __contains__(self, item):
+        """
+        Return for `item in self`.
+        """
+        if _isna(item):
+            if (
+                item is self.dtype.na_value
+                or isinstance(item, self.dtype.type)
+                or item is None
+            ):
+                return self.isna().any()
+            else:
+                return False
+        return (self == item).any()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `geopandas-0.8.2/geopandas/datasets/__init__.py` & `geopandas-0.9.0/geopandas/datasets/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,20 @@
 
     Parameters
     ----------
     dataset : str
         The name of the dataset. See ``geopandas.datasets.available`` for
         all options.
 
+    Examples
+    --------
+    >>> geopandas.datasets.get_path("naturalearth_lowres")  # doctest: +SKIP
+    '.../python3.8/site-packages/geopandas/datasets/\
+naturalearth_lowres/naturalearth_lowres.shp'
+
     """
     if dataset in _available_dir:
         return os.path.abspath(os.path.join(_module_path, dataset, dataset + ".shp"))
     elif dataset in _available_zip:
         fpath = os.path.abspath(os.path.join(_module_path, _available_zip[dataset]))
         return "zip://" + fpath
     else:
```

### Comparing `geopandas-0.8.2/geopandas/datasets/naturalearth_cities/naturalearth_cities.README.html` & `geopandas-0.9.0/geopandas/datasets/naturalearth_cities/naturalearth_cities.README.html`

 * *Files identical despite different names*

### Comparing `geopandas-0.8.2/geopandas/datasets/naturalearth_cities/naturalearth_cities.dbf` & `geopandas-0.9.0/geopandas/datasets/naturalearth_cities/naturalearth_cities.dbf`

 * *Files identical despite different names*

### Comparing `geopandas-0.8.2/geopandas/datasets/naturalearth_cities/naturalearth_cities.shp` & `geopandas-0.9.0/geopandas/datasets/naturalearth_cities/naturalearth_cities.shp`

 * *Files identical despite different names*

### Comparing `geopandas-0.8.2/geopandas/datasets/naturalearth_cities/naturalearth_cities.shx` & `geopandas-0.9.0/geopandas/datasets/naturalearth_cities/naturalearth_cities.shx`

 * *Files identical despite different names*

### Comparing `geopandas-0.8.2/geopandas/datasets/naturalearth_creation.py` & `geopandas-0.9.0/geopandas/datasets/naturalearth_creation.py`

 * *Files identical despite different names*

### Comparing `geopandas-0.8.2/geopandas/datasets/naturalearth_lowres/naturalearth_lowres.dbf` & `geopandas-0.9.0/geopandas/datasets/naturalearth_lowres/naturalearth_lowres.dbf`

 * *Files identical despite different names*

### Comparing `geopandas-0.8.2/geopandas/datasets/naturalearth_lowres/naturalearth_lowres.shp` & `geopandas-0.9.0/geopandas/datasets/naturalearth_lowres/naturalearth_lowres.shp`

 * *Files identical despite different names*

### Comparing `geopandas-0.8.2/geopandas/datasets/naturalearth_lowres/naturalearth_lowres.shx` & `geopandas-0.9.0/geopandas/datasets/naturalearth_lowres/naturalearth_lowres.shx`

 * *Files identical despite different names*

### Comparing `geopandas-0.8.2/geopandas/datasets/nybb_16a.zip` & `geopandas-0.9.0/geopandas/datasets/nybb_16a.zip`

 * *Files identical despite different names*

### Comparing `geopandas-0.8.2/geopandas/geodataframe.py` & `geopandas-0.9.0/geopandas/geodataframe.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 
 from shapely.geometry import mapping, shape
 from shapely.geometry.base import BaseGeometry
 
 
 from pyproj import CRS
 
-from geopandas.array import GeometryArray, from_shapely, GeometryDtype
+from geopandas.array import GeometryArray, GeometryDtype, from_shapely, to_wkb, to_wkt
 from geopandas.base import GeoPandasBase, is_geometry_type
-from geopandas.geoseries import GeoSeries
+from geopandas.geoseries import GeoSeries, inherit_doc
 import geopandas.io
 from geopandas.plotting import plot_dataframe
+from . import _compat as compat
 
 
 DEFAULT_GEO_COLUMN_NAME = "geometry"
 
 
 def _ensure_geometry(data, crs=None):
     """
@@ -60,41 +61,56 @@
         column on GeoDataFrame.
 
     Examples
     --------
     Constructing GeoDataFrame from a dictionary.
 
     >>> from shapely.geometry import Point
-    >>> d = {'col1': ['name1', 'name2'], 'geometry': [Point(1,2), Point(2,1)]}
-    >>> gdf = gpd.GeoDataFrame(d, crs="EPSG:4326")
+    >>> d = {'col1': ['name1', 'name2'], 'geometry': [Point(1, 2), Point(2, 1)]}
+    >>> gdf = geopandas.GeoDataFrame(d, crs="EPSG:4326")
     >>> gdf
         col1                 geometry
     0  name1  POINT (1.00000 2.00000)
     1  name2  POINT (2.00000 1.00000)
 
     Notice that the inferred dtype of 'geometry' columns is geometry.
 
     >>> gdf.dtypes
     col1          object
     geometry    geometry
     dtype: object
+
+    Constructing GeoDataFrame from a pandas DataFrame with a column of WKT geometries:
+
+    >>> import pandas as pd
+    >>> d = {'col1': ['name1', 'name2'], 'wkt': ['POINT (1 2)', 'POINT (2 1)']}
+    >>> df = pd.DataFrame(d)
+    >>> gs = geopandas.GeoSeries.from_wkt(df['wkt'])
+    >>> gdf = geopandas.GeoDataFrame(df, geometry=gs, crs="EPSG:4326")
+    >>> gdf
+        col1          wkt                 geometry
+    0  name1  POINT (1 2)  POINT (1.00000 2.00000)
+    1  name2  POINT (2 1)  POINT (2.00000 1.00000)
+
+    See also
+    --------
+    GeoSeries : Series object designed to store shapely geometry objects
     """
 
     _metadata = ["_crs", "_geometry_column_name"]
 
     _geometry_column_name = DEFAULT_GEO_COLUMN_NAME
 
-    def __init__(self, *args, **kwargs):
-        crs = kwargs.pop("crs", None)
-        geometry = kwargs.pop("geometry", None)
-        super(GeoDataFrame, self).__init__(*args, **kwargs)
+    def __init__(self, *args, geometry=None, crs=None, **kwargs):
+        with compat.ignore_shapely2_warnings():
+            super(GeoDataFrame, self).__init__(*args, **kwargs)
 
         # need to set this before calling self['geometry'], because
         # getitem accesses crs
-        self._crs = crs if crs is not None else None
+        self._crs = CRS.from_user_input(crs) if crs else None
 
         # set_geometry ensures the geometry data have the proper dtype,
         # but is not called if `geometry=None` ('geometry' column present
         # in the data), so therefore need to ensure it here manually
         # but within a try/except because currently non-geometries are
         # allowed in that case
         # TODO do we want to raise / return normal DataFrame in this case?
@@ -145,15 +161,14 @@
                     "CRS mismatch will raise an error in the future versions "
                     "of GeoPandas.",
                     FutureWarning,
                     stacklevel=2,
                 )
                 # TODO: raise error in 0.9 or 0.10.
             self.set_geometry(geometry, inplace=True)
-        self._invalidate_sindex()
 
         if geometry is None and crs:
             warnings.warn(
                 "Assigning CRS to a GeoDataFrame without a geometry column is now "
                 "deprecated and will not be supported in the future.",
                 FutureWarning,
                 stacklevel=2,
@@ -189,33 +204,59 @@
         the specified input. By default yields a new object.
 
         The original geometry column is replaced with the input.
 
         Parameters
         ----------
         col : column label or array
-        drop : boolean, default True
+        drop : boolean, default False
             Delete column to be used as the new geometry
         inplace : boolean, default False
             Modify the GeoDataFrame in place (do not create a new object)
         crs : pyproj.CRS, optional
             Coordinate system to use. The value can be anything accepted
             by :meth:`pyproj.CRS.from_user_input() <pyproj.crs.CRS.from_user_input>`,
             such as an authority string (eg "EPSG:4326") or a WKT string.
             If passed, overrides both DataFrame and col's crs.
             Otherwise, tries to get crs from passed col values or DataFrame.
 
         Examples
         --------
-        >>> df1 = df.set_geometry([Point(0,0), Point(1,1), Point(2,2)])
-        >>> df2 = df.set_geometry('geom1')
+        >>> from shapely.geometry import Point
+        >>> d = {'col1': ['name1', 'name2'], 'geometry': [Point(1, 2), Point(2, 1)]}
+        >>> gdf = geopandas.GeoDataFrame(d, crs="EPSG:4326")
+        >>> gdf
+            col1                 geometry
+        0  name1  POINT (1.00000 2.00000)
+        1  name2  POINT (2.00000 1.00000)
+
+        Passing an array:
+
+        >>> df1 = gdf.set_geometry([Point(0,0), Point(1,1)])
+        >>> df1
+            col1                 geometry
+        0  name1  POINT (0.00000 0.00000)
+        1  name2  POINT (1.00000 1.00000)
+
+        Using existing column:
+
+        >>> gdf["buffered"] = gdf.buffer(2)
+        >>> df2 = gdf.set_geometry("buffered")
+        >>> df2.geometry
+        0    POLYGON ((3.00000 2.00000, 2.99037 1.80397, 2....
+        1    POLYGON ((4.00000 1.00000, 3.99037 0.80397, 3....
+        Name: buffered, dtype: geometry
 
         Returns
         -------
         GeoDataFrame
+
+        See also
+        --------
+        GeoDataFrame.rename_geometry : rename an active geometry column
         """
         # Most of the code here is taken from DataFrame.set_index()
         if inplace:
             frame = self
         else:
             frame = self.copy()
 
@@ -256,15 +297,14 @@
         frame[geo_column_name] = level
         if frame.index is not index and len(frame.index) == len(index):
             # With pandas < 1.0 and an empty frame (no rows), the index gets reset
             # to a default RangeIndex -> set back the original index if needed
             frame.index = index
         frame._geometry_column_name = geo_column_name
         frame.crs = crs
-        frame._invalidate_sindex()
         if not inplace:
             return frame
 
     def rename_geometry(self, col, inplace=False):
         """
         Renames the GeoDataFrame geometry column to
         the specified name. By default yields a new object.
@@ -275,42 +315,76 @@
         ----------
         col : new geometry column label
         inplace : boolean, default False
             Modify the GeoDataFrame in place (do not create a new object)
 
         Examples
         --------
+        >>> from shapely.geometry import Point
+        >>> d = {'col1': ['name1', 'name2'], 'geometry': [Point(1, 2), Point(2, 1)]}
+        >>> df = geopandas.GeoDataFrame(d, crs="EPSG:4326")
         >>> df1 = df.rename_geometry('geom1')
         >>> df1.geometry.name
         'geom1'
         >>> df.rename_geometry('geom1', inplace=True)
         >>> df.geometry.name
         'geom1'
 
         Returns
         -------
         geodataframe : GeoDataFrame
+
+        See also
+        --------
+        GeoDataFrame.set_geometry : set the active geometry
         """
         geometry_col = self.geometry.name
-        if not inplace:
-            return self.rename(columns={geometry_col: col}).set_geometry(col, inplace)
-        self.rename(columns={geometry_col: col}, inplace=inplace)
-        self.set_geometry(col, inplace=inplace)
+        if col in self.columns:
+            raise ValueError(f"Column named {col} already exists")
+        else:
+            if not inplace:
+                return self.rename(columns={geometry_col: col}).set_geometry(
+                    col, inplace
+                )
+            self.rename(columns={geometry_col: col}, inplace=inplace)
+            self.set_geometry(col, inplace=inplace)
 
     @property
     def crs(self):
         """
         The Coordinate Reference System (CRS) represented as a ``pyproj.CRS``
         object.
 
         Returns None if the CRS is not set, and to set the value it
         :getter: Returns a ``pyproj.CRS`` or None. When setting, the value
         can be anything accepted by
         :meth:`pyproj.CRS.from_user_input() <pyproj.crs.CRS.from_user_input>`,
         such as an authority string (eg "EPSG:4326") or a WKT string.
+
+        Examples
+        --------
+
+        >>> gdf.crs  # doctest: +SKIP
+        <Geographic 2D CRS: EPSG:4326>
+        Name: WGS 84
+        Axis Info [ellipsoidal]:
+        - Lat[north]: Geodetic latitude (degree)
+        - Lon[east]: Geodetic longitude (degree)
+        Area of Use:
+        - name: World
+        - bounds: (-180.0, -90.0, 180.0, 90.0)
+        Datum: World Geodetic System 1984
+        - Ellipsoid: WGS 84
+        - Prime Meridian: Greenwich
+
+        See also
+        --------
+        GeoDataFrame.set_crs : assign CRS
+        GeoDataFrame.to_crs : re-project to another CRS
+
         """
         return self._crs
 
     @crs.setter
     def crs(self, value):
         """Sets the value of the crs"""
         if self._geometry_column_name not in self:
@@ -348,17 +422,45 @@
             if self.crs is not None:
                 if self.geometry.values.crs is None:
                     self.crs = self.crs
         except Exception:
             pass
 
     @classmethod
+    def from_dict(cls, data, geometry=None, crs=None, **kwargs):
+        """
+        Construct GeoDataFrame from dict of array-like or dicts by
+        overiding DataFrame.from_dict method with geometry and crs
+
+        Parameters
+        ----------
+        data : dict
+            Of the form {field : array-like} or {field : dict}.
+        geometry : str or array (optional)
+            If str, column to use as geometry. If array, will be set as 'geometry'
+            column on GeoDataFrame.
+        crs : str or dict (optional)
+            Coordinate reference system to set on the resulting frame.
+        kwargs : key-word arguments
+            These arguments are passed to DataFrame.from_dict
+
+        Returns
+        -------
+        GeoDataFrame
+
+        """
+        dataframe = super().from_dict(data, **kwargs)
+        return GeoDataFrame(dataframe, geometry=geometry, crs=crs)
+
+    @classmethod
     def from_file(cls, filename, **kwargs):
         """Alternate constructor to create a ``GeoDataFrame`` from a file.
 
+        It is recommended to use :func:`geopandas.read_file` instead.
+
         Can load a ``GeoDataFrame`` from a file in any format recognized by
         `fiona`. See http://fiona.readthedocs.io/en/latest/manual.html for details.
 
         Parameters
         ----------
         filename : str
             File path or file handle to read from. Depending on which kwargs
@@ -367,15 +469,40 @@
         kwargs : key-word arguments
             These arguments are passed to fiona.open, and can be used to
             access multi-layer data, data stored within archives (zip files),
             etc.
 
         Examples
         --------
-        >>> df = geopandas.GeoDataFrame.from_file('nybb.shp')
+
+        >>> path = geopandas.datasets.get_path('nybb')
+        >>> gdf = geopandas.GeoDataFrame.from_file(path)
+        >>> gdf  # doctest: +SKIP
+           BoroCode       BoroName     Shape_Leng    Shape_Area                 \
+                          geometry
+        0         5  Staten Island  330470.010332  1.623820e+09  MULTIPOLYGON ((\
+(970217.022 145643.332, 970227....
+        1         4         Queens  896344.047763  3.045213e+09  MULTIPOLYGON ((\
+(1029606.077 156073.814, 102957...
+        2         3       Brooklyn  741080.523166  1.937479e+09  MULTIPOLYGON ((\
+(1021176.479 151374.797, 102100...
+        3         1      Manhattan  359299.096471  6.364715e+08  MULTIPOLYGON ((\
+(981219.056 188655.316, 980940....
+        4         2          Bronx  464392.991824  1.186925e+09  MULTIPOLYGON ((\
+(1012821.806 229228.265, 101278...
+
+        The recommended method of reading files is :func:`geopandas.read_file`:
+
+        >>> gdf = geopandas.read_file(path)
+
+        See also
+        --------
+        read_file : read file to GeoDataFame
+        GeoDataFrame.to_file : write GeoDataFrame to file
+
         """
         return geopandas.io.file._read_file(filename, **kwargs)
 
     @classmethod
     def from_features(cls, features, crs=None, columns=None):
         """
         Alternate constructor to create GeoDataFrame from an iterable of
@@ -402,14 +529,42 @@
         GeoDataFrame
 
         Notes
         -----
         For more information about the ``__geo_interface__``, see
         https://gist.github.com/sgillies/2217756
 
+        Examples
+        --------
+        >>> feature_coll = {
+        ...     "type": "FeatureCollection",
+        ...     "features": [
+        ...         {
+        ...             "id": "0",
+        ...             "type": "Feature",
+        ...             "properties": {"col1": "name1"},
+        ...             "geometry": {"type": "Point", "coordinates": (1.0, 2.0)},
+        ...             "bbox": (1.0, 2.0, 1.0, 2.0),
+        ...         },
+        ...         {
+        ...             "id": "1",
+        ...             "type": "Feature",
+        ...             "properties": {"col1": "name2"},
+        ...             "geometry": {"type": "Point", "coordinates": (2.0, 1.0)},
+        ...             "bbox": (2.0, 1.0, 2.0, 1.0),
+        ...         },
+        ...     ],
+        ...     "bbox": (1.0, 1.0, 2.0, 2.0),
+        ... }
+        >>> df = geopandas.GeoDataFrame.from_features(feature_coll)
+        >>> df
+                          geometry   col1
+        0  POINT (1.00000 2.00000)  name1
+        1  POINT (2.00000 1.00000)  name2
+
         """
         # Handle feature collections
         if hasattr(features, "__geo_interface__"):
             fs = features.__geo_interface__
         else:
             fs = features
 
@@ -447,15 +602,15 @@
         """
         Alternate constructor to create a ``GeoDataFrame`` from a sql query
         containing a geometry column in WKB representation.
 
         Parameters
         ----------
         sql : string
-        con : DB connection object or SQLAlchemy engine
+        con : sqlalchemy.engine.Connection or sqlalchemy.engine.Engine
         geom_col : string, default 'geom'
             column name to convert to shapely geometries
         crs : optional
             Coordinate reference system to use for the returned GeoDataFrame
         index_col : string or list of strings, optional, default: None
             Column(s) to set as index(MultiIndex)
         coerce_float : boolean, default True
@@ -474,18 +629,35 @@
             List of parameters to pass to execute method.
         chunksize : int, default None
             If specified, return an iterator where chunksize is the number
             of rows to include in each chunk.
 
         Examples
         --------
+        PostGIS
+
+        >>> from sqlalchemy import create_engine  # doctest: +SKIP
+        >>> db_connection_url = "postgres://myusername:mypassword@myhost:5432/mydb"
+        >>> con = create_engine(db_connection_url)  # doctest: +SKIP
         >>> sql = "SELECT geom, highway FROM roads"
+        >>> df = geopandas.GeoDataFrame.from_postgis(sql, con)  # doctest: +SKIP
+
         SpatiaLite
+
         >>> sql = "SELECT ST_Binary(geom) AS geom, highway FROM roads"
-        >>> df = geopandas.GeoDataFrame.from_postgis(sql, con)
+        >>> df = geopandas.GeoDataFrame.from_postgis(sql, con)  # doctest: +SKIP
+
+        The recommended method of reading from PostGIS is
+        :func:`geopandas.read_postgis`:
+
+        >>> df = geopandas.read_postgis(sql, con)  # doctest: +SKIP
+
+        See also
+        --------
+        geopandas.read_postgis : read PostGIS database to GeoDataFrame
         """
 
         df = geopandas.io.sql._read_postgis(
             sql,
             con,
             geom_col=geom_col,
             crs=crs,
@@ -494,68 +666,141 @@
             parse_dates=parse_dates,
             params=params,
             chunksize=chunksize,
         )
 
         return df
 
-    def to_json(self, na="null", show_bbox=False, **kwargs):
+    def to_json(self, na="null", show_bbox=False, drop_id=False, **kwargs):
         """
         Returns a GeoJSON representation of the ``GeoDataFrame`` as a string.
 
         Parameters
         ----------
         na : {'null', 'drop', 'keep'}, default 'null'
             Indicates how to output missing (NaN) values in the GeoDataFrame.
             See below.
         show_bbox : bool, optional, default: False
             Include bbox (bounds) in the geojson
+        drop_id : bool, default: False
+            Whether to retain the index of the GeoDataFrame as the id property
+            in the generated GeoJSON. Default is False, but may want True
+            if the index is just arbitrary row numbers.
 
         Notes
         -----
         The remaining *kwargs* are passed to json.dumps().
 
         Missing (NaN) values in the GeoDataFrame can be represented as follows:
 
         - ``null``: output the missing entries as JSON null.
         - ``drop``: remove the property from the feature. This applies to each
           feature individually so that features may have different properties.
         - ``keep``: output the missing entries as NaN.
+
+        Examples
+        --------
+
+        >>> from shapely.geometry import Point
+        >>> d = {'col1': ['name1', 'name2'], 'geometry': [Point(1, 2), Point(2, 1)]}
+        >>> gdf = geopandas.GeoDataFrame(d, crs="EPSG:4326")
+        >>> gdf
+            col1                 geometry
+        0  name1  POINT (1.00000 2.00000)
+        1  name2  POINT (2.00000 1.00000)
+
+        >>> gdf.to_json()
+        '{"type": "FeatureCollection", "features": [{"id": "0", "type": "Feature", \
+"properties": {"col1": "name1"}, "geometry": {"type": "Point", "coordinates": [1.0,\
+ 2.0]}}, {"id": "1", "type": "Feature", "properties": {"col1": "name2"}, "geometry"\
+: {"type": "Point", "coordinates": [2.0, 1.0]}}]}'
+
+        Alternatively, you can write GeoJSON to file:
+
+        >>> gdf.to_file(path, driver="GeoJSON")  # doctest: +SKIP
+
+        See also
+        --------
+        GeoDataFrame.to_file : write GeoDataFrame to file
+
         """
-        return json.dumps(self._to_geo(na=na, show_bbox=show_bbox), **kwargs)
+        return json.dumps(
+            self._to_geo(na=na, show_bbox=show_bbox, drop_id=drop_id), **kwargs
+        )
 
     @property
     def __geo_interface__(self):
         """Returns a ``GeoDataFrame`` as a python feature collection.
 
         Implements the `geo_interface`. The returned python data structure
         represents the ``GeoDataFrame`` as a GeoJSON-like
         ``FeatureCollection``.
 
         This differs from `_to_geo()` only in that it is a property with
         default args instead of a method
+
+        Examples
+        --------
+
+        >>> from shapely.geometry import Point
+        >>> d = {'col1': ['name1', 'name2'], 'geometry': [Point(1, 2), Point(2, 1)]}
+        >>> gdf = geopandas.GeoDataFrame(d, crs="EPSG:4326")
+        >>> gdf
+            col1                 geometry
+        0  name1  POINT (1.00000 2.00000)
+        1  name2  POINT (2.00000 1.00000)
+
+        >>> gdf.__geo_interface__
+        {'type': 'FeatureCollection', 'features': [{'id': '0', 'type': 'Feature', \
+'properties': {'col1': 'name1'}, 'geometry': {'type': 'Point', 'coordinates': (1.0\
+, 2.0)}, 'bbox': (1.0, 2.0, 1.0, 2.0)}, {'id': '1', 'type': 'Feature', 'properties\
+': {'col1': 'name2'}, 'geometry': {'type': 'Point', 'coordinates': (2.0, 1.0)}, 'b\
+box': (2.0, 1.0, 2.0, 1.0)}], 'bbox': (1.0, 1.0, 2.0, 2.0)}
+
+
         """
-        return self._to_geo(na="null", show_bbox=True)
+        return self._to_geo(na="null", show_bbox=True, drop_id=False)
 
-    def iterfeatures(self, na="null", show_bbox=False):
+    def iterfeatures(self, na="null", show_bbox=False, drop_id=False):
         """
         Returns an iterator that yields feature dictionaries that comply with
         __geo_interface__
 
         Parameters
         ----------
-        na : {'null', 'drop', 'keep'}, default 'null'
+        na : str, optional
+            Options are {'null', 'drop', 'keep'}, default 'null'.
             Indicates how to output missing (NaN) values in the GeoDataFrame
             * null: ouput the missing entries as JSON null
             * drop: remove the property from the feature. This applies to
                     each feature individually so that features may have
                     different properties
             * keep: output the missing entries as NaN
+        show_bbox : bool, optional
+            Include bbox (bounds) in the geojson. Default False.
+        drop_id : bool, default: False
+            Whether to retain the index of the GeoDataFrame as the id property
+            in the generated GeoJSON. Default is False, but may want True
+            if the index is just arbitrary row numbers.
 
-        show_bbox : include bbox (bounds) in the geojson. default False
+        Examples
+        --------
+
+        >>> from shapely.geometry import Point
+        >>> d = {'col1': ['name1', 'name2'], 'geometry': [Point(1, 2), Point(2, 1)]}
+        >>> gdf = geopandas.GeoDataFrame(d, crs="EPSG:4326")
+        >>> gdf
+            col1                 geometry
+        0  name1  POINT (1.00000 2.00000)
+        1  name2  POINT (2.00000 1.00000)
+
+        >>> feature = next(gdf.iterfeatures())
+        >>> feature
+        {'id': '0', 'type': 'Feature', 'properties': {'col1': 'name1'}, 'geometry': {\
+'type': 'Point', 'coordinates': (1.0, 2.0)}}
         """
         if na not in ["null", "drop", "keep"]:
             raise ValueError("Unknown na method {0}".format(na))
 
         if self._geometry_column_name not in self:
             raise AttributeError(
                 "No geometry data set (expected in"
@@ -579,35 +824,43 @@
                 if na == "drop":
                     properties_items = {
                         k: v for k, v in zip(properties_cols, row) if not pd.isnull(v)
                     }
                 else:
                     properties_items = {k: v for k, v in zip(properties_cols, row)}
 
-                feature = {
-                    "id": str(ids[i]),
-                    "type": "Feature",
-                    "properties": properties_items,
-                    "geometry": mapping(geom) if geom else None,
-                }
+                if drop_id:
+                    feature = {}
+                else:
+                    feature = {"id": str(ids[i])}
+
+                feature["type"] = "Feature"
+                feature["properties"] = properties_items
+                feature["geometry"] = mapping(geom) if geom else None
 
                 if show_bbox:
                     feature["bbox"] = geom.bounds if geom else None
+
                 yield feature
 
         else:
             for fid, geom in zip(ids, geometries):
-                feature = {
-                    "id": str(fid),
-                    "type": "Feature",
-                    "properties": {},
-                    "geometry": mapping(geom) if geom else None,
-                }
+
+                if drop_id:
+                    feature = {}
+                else:
+                    feature = {"id": str(fid)}
+
+                feature["type"] = "Feature"
+                feature["properties"] = {}
+                feature["geometry"] = mapping(geom) if geom else None
+
                 if show_bbox:
                     feature["bbox"] = geom.bounds if geom else None
+
                 yield feature
 
     def _to_geo(self, **kwargs):
         """
         Returns a python feature collection (i.e. the geointerface)
         representation of the GeoDataFrame.
 
@@ -618,14 +871,65 @@
         }
 
         if kwargs.get("show_bbox", False):
             geo["bbox"] = tuple(self.total_bounds)
 
         return geo
 
+    def to_wkb(self, hex=False, **kwargs):
+        """
+        Encode all geometry columns in the GeoDataFrame to WKB.
+
+        Parameters
+        ----------
+        hex : bool
+            If true, export the WKB as a hexadecimal string.
+            The default is to return a binary bytes object.
+        kwargs
+            Additional keyword args will be passed to
+            :func:`pygeos.to_wkb` if pygeos is installed.
+
+        Returns
+        -------
+        DataFrame
+            geometry columns are encoded to WKB
+        """
+
+        df = DataFrame(self.copy())
+
+        # Encode all geometry columns to WKB
+        for col in df.columns[df.dtypes == "geometry"]:
+            df[col] = to_wkb(df[col].values, hex=hex, **kwargs)
+
+        return df
+
+    def to_wkt(self, **kwargs):
+        """
+        Encode all geometry columns in the GeoDataFrame to WKT.
+
+        Parameters
+        ----------
+        kwargs
+            Keyword args will be passed to :func:`pygeos.to_wkt`
+            if pygeos is installed.
+
+        Returns
+        -------
+        DataFrame
+            geometry columns are encoded to WKT
+        """
+
+        df = DataFrame(self.copy())
+
+        # Encode all geometry columns to WKT
+        for col in df.columns[df.dtypes == "geometry"]:
+            df[col] = to_wkt(df[col].values, **kwargs)
+
+        return df
+
     def to_parquet(self, path, index=None, compression="snappy", **kwargs):
         """Write a GeoDataFrame to the Parquet format.
 
         Any geometry columns present are serialized to WKB format in the file.
 
         Requires 'pyarrow'.
 
@@ -649,14 +953,24 @@
             If ``False``, the index(es) will not be written to the file.
             If ``None``, the index(ex) will be included as columns in the file
             output except `RangeIndex` which is stored as metadata only.
         compression : {'snappy', 'gzip', 'brotli', None}, default 'snappy'
             Name of the compression to use. Use ``None`` for no compression.
         kwargs
             Additional keyword arguments passed to to pyarrow.parquet.write_table().
+
+        Examples
+        --------
+
+        >>> gdf.to_parquet('data.parquet')  # doctest: +SKIP
+
+        See also
+        --------
+        GeoDataFrame.to_feather : write GeoDataFrame to feather
+        GeoDataFrame.to_file : write GeoDataFrame to file
         """
 
         from geopandas.io.arrow import _to_parquet
 
         _to_parquet(self, path, compression=compression, index=index, **kwargs)
 
     def to_feather(self, path, index=None, compression=None, **kwargs):
@@ -687,14 +1001,24 @@
             If ``None``, the index(ex) will be included as columns in the file
             output except `RangeIndex` which is stored as metadata only.
         compression : {'zstd', 'lz4', 'uncompressed'}, optional
             Name of the compression to use. Use ``"uncompressed"`` for no
             compression. By default uses LZ4 if available, otherwise uncompressed.
         kwargs
             Additional keyword arguments passed to to pyarrow.feather.write_feather().
+
+        Examples
+        --------
+
+        >>> gdf.to_feather('data.feather')  # doctest: +SKIP
+
+        See also
+        --------
+        GeoDataFrame.to_parquet : write GeoDataFrame to parquet
+        GeoDataFrame.to_file : write GeoDataFrame to file
         """
 
         from geopandas.io.arrow import _to_feather
 
         _to_feather(self, path, index=index, compression=compression, **kwargs)
 
     def to_file(
@@ -703,15 +1027,15 @@
         """Write the ``GeoDataFrame`` to a file.
 
         By default, an ESRI shapefile is written, but any OGR data source
         supported by Fiona can be written. A dictionary of supported OGR
         providers is available via:
 
         >>> import fiona
-        >>> fiona.supported_drivers
+        >>> fiona.supported_drivers  # doctest: +SKIP
 
         Parameters
         ----------
         filename : string
             File path or file handle to write to.
         driver : string, default: 'ESRI Shapefile'
             The OGR format driver used to write the vector file.
@@ -736,14 +1060,30 @@
         The format drivers will attempt to detect the encoding of your data, but
         may fail. In this case, the proper encoding can be specified explicitly
         by using the encoding keyword parameter, e.g. ``encoding='utf-8'``.
 
         See Also
         --------
         GeoSeries.to_file
+        GeoDataFrame.to_postgis : write GeoDataFrame to PostGIS database
+        GeoDataFrame.to_parquet : write GeoDataFrame to parquet
+        GeoDataFrame.to_feather : write GeoDataFrame to feather
+
+        Examples
+        --------
+
+        >>> gdf.to_file('dataframe.shp')  # doctest: +SKIP
+
+        >>> gdf.to_file('dataframe.gpkg', driver='GPKG', layer='name')  # doctest: +SKIP
+
+        >>> gdf.to_file('dataframe.geojson', driver='GeoJSON')  # doctest: +SKIP
+
+        With selected drivers you can also append to a file with `mode="a"`:
+
+        >>> gdf.to_file('dataframe.shp', mode="a")  # doctest: +SKIP
         """
         from geopandas.io.file import _to_file
 
         _to_file(self, filename, driver, schema, index, **kwargs)
 
     def set_crs(self, crs=None, epsg=None, inplace=False, allow_override=False):
         """
@@ -766,14 +1106,58 @@
         inplace : bool, default False
             If True, the CRS of the GeoDataFrame will be changed in place
             (while still returning the result) instead of making a copy of
             the GeoDataFrame.
         allow_override : bool, default False
             If the the GeoDataFrame already has a CRS, allow to replace the
             existing CRS, even when both are not equal.
+
+        Examples
+        --------
+        >>> from shapely.geometry import Point
+        >>> d = {'col1': ['name1', 'name2'], 'geometry': [Point(1, 2), Point(2, 1)]}
+        >>> gdf = geopandas.GeoDataFrame(d)
+        >>> gdf
+            col1                 geometry
+        0  name1  POINT (1.00000 2.00000)
+        1  name2  POINT (2.00000 1.00000)
+
+        Setting CRS to a GeoDataFrame without one:
+
+        >>> gdf.crs is None
+        True
+
+        >>> gdf = gdf.set_crs('epsg:3857')
+        >>> gdf.crs  # doctest: +SKIP
+        <Projected CRS: EPSG:3857>
+        Name: WGS 84 / Pseudo-Mercator
+        Axis Info [cartesian]:
+        - X[east]: Easting (metre)
+        - Y[north]: Northing (metre)
+        Area of Use:
+        - name: World - 85°S to 85°N
+        - bounds: (-180.0, -85.06, 180.0, 85.06)
+        Coordinate Operation:
+        - name: Popular Visualisation Pseudo-Mercator
+        - method: Popular Visualisation Pseudo Mercator
+        Datum: World Geodetic System 1984
+        - Ellipsoid: WGS 84
+        - Prime Meridian: Greenwich
+
+        Overriding existing CRS:
+
+        >>> gdf = gdf.set_crs(4326, allow_override=True)
+
+        Without ``allow_override=True``, ``set_crs`` returns an error if you try to
+        override CRS.
+
+        See also
+        --------
+        GeoDataFrame.to_crs : re-project to another CRS
+
         """
         if not inplace:
             df = self.copy()
         else:
             df = self
         df.geometry = df.geometry.set_crs(
             crs=crs, epsg=epsg, allow_override=allow_override, inplace=True
@@ -804,40 +1188,125 @@
         inplace : bool, optional, default: False
             Whether to return a new GeoDataFrame or do the transformation in
             place.
 
         Returns
         -------
         GeoDataFrame
+
+        Examples
+        --------
+        >>> from shapely.geometry import Point
+        >>> d = {'col1': ['name1', 'name2'], 'geometry': [Point(1, 2), Point(2, 1)]}
+        >>> gdf = geopandas.GeoDataFrame(d, crs=4326)
+        >>> gdf
+            col1                 geometry
+        0  name1  POINT (1.00000 2.00000)
+        1  name2  POINT (2.00000 1.00000)
+        >>> gdf.crs  # doctest: +SKIP
+        <Geographic 2D CRS: EPSG:4326>
+        Name: WGS 84
+        Axis Info [ellipsoidal]:
+        - Lat[north]: Geodetic latitude (degree)
+        - Lon[east]: Geodetic longitude (degree)
+        Area of Use:
+        - name: World
+        - bounds: (-180.0, -90.0, 180.0, 90.0)
+        Datum: World Geodetic System 1984
+        - Ellipsoid: WGS 84
+        - Prime Meridian: Greenwich
+
+        >>> gdf = gdf.to_crs(3857)
+        >>> gdf
+            col1                       geometry
+        0  name1  POINT (111319.491 222684.209)
+        1  name2  POINT (222638.982 111325.143)
+        >>> gdf.crs  # doctest: +SKIP
+        <Projected CRS: EPSG:3857>
+        Name: WGS 84 / Pseudo-Mercator
+        Axis Info [cartesian]:
+        - X[east]: Easting (metre)
+        - Y[north]: Northing (metre)
+        Area of Use:
+        - name: World - 85°S to 85°N
+        - bounds: (-180.0, -85.06, 180.0, 85.06)
+        Coordinate Operation:
+        - name: Popular Visualisation Pseudo-Mercator
+        - method: Popular Visualisation Pseudo Mercator
+        Datum: World Geodetic System 1984
+        - Ellipsoid: WGS 84
+        - Prime Meridian: Greenwich
+
+        See also
+        --------
+        GeoDataFrame.set_crs : assign CRS without re-projection
         """
         if inplace:
             df = self
         else:
             df = self.copy()
         geom = df.geometry.to_crs(crs=crs, epsg=epsg)
         df.geometry = geom
         df.crs = geom.crs
         if not inplace:
             return df
 
+    def estimate_utm_crs(self, datum_name="WGS 84"):
+        """Returns the estimated UTM CRS based on the bounds of the dataset.
+
+        .. versionadded:: 0.9
+
+        .. note:: Requires pyproj 3+
+
+        Parameters
+        ----------
+        datum_name : str, optional
+            The name of the datum to use in the query. Default is WGS 84.
+
+        Returns
+        -------
+        pyproj.CRS
+
+        Examples
+        --------
+        >>> world = geopandas.read_file(
+        ...     geopandas.datasets.get_path("naturalearth_lowres")
+        ... )
+        >>> germany = world.loc[world.name == "Germany"]
+        >>> germany.estimate_utm_crs()  # doctest: +SKIP
+        <Projected CRS: EPSG:32632>
+        Name: WGS 84 / UTM zone 32N
+        Axis Info [cartesian]:
+        - E[east]: Easting (metre)
+        - N[north]: Northing (metre)
+        Area of Use:
+        - name: World - N hemisphere - 6°E to 12°E - by country
+        - bounds: (6.0, 0.0, 12.0, 84.0)
+        Coordinate Operation:
+        - name: UTM zone 32N
+        - method: Transverse Mercator
+        Datum: World Geodetic System 1984
+        - Ellipsoid: WGS 84
+        - Prime Meridian: Greenwich
+        """
+        return self.geometry.estimate_utm_crs(datum_name=datum_name)
+
     def __getitem__(self, key):
         """
         If the result is a column containing only 'geometry', return a
         GeoSeries. If it's a DataFrame with a 'geometry' column, return a
         GeoDataFrame.
         """
         result = super(GeoDataFrame, self).__getitem__(key)
         geo_col = self._geometry_column_name
         if isinstance(result, Series) and isinstance(result.dtype, GeometryDtype):
             result.__class__ = GeoSeries
-            result._invalidate_sindex()
         elif isinstance(result, DataFrame) and geo_col in result:
             result.__class__ = GeoDataFrame
             result._geometry_column_name = geo_col
-            result._invalidate_sindex()
         elif isinstance(result, DataFrame) and geo_col not in result:
             result.__class__ = DataFrame
         return result
 
     def __setitem__(self, key, value):
         """
         Overwritten to preserve CRS of GeometryArray in cases like
@@ -879,103 +1348,176 @@
         """
         result = DataFrame.merge(self, *args, **kwargs)
         geo_col = self._geometry_column_name
         if isinstance(result, DataFrame) and geo_col in result:
             result.__class__ = GeoDataFrame
             result.crs = self.crs
             result._geometry_column_name = geo_col
-            result._invalidate_sindex()
         elif isinstance(result, DataFrame) and geo_col not in result:
             result.__class__ = DataFrame
         return result
 
+    @inherit_doc(pd.DataFrame)
+    def apply(self, func, axis=0, raw=False, result_type=None, args=(), **kwargs):
+        result = super().apply(
+            func, axis=axis, raw=raw, result_type=result_type, args=args, **kwargs
+        )
+        if (
+            isinstance(result, GeoDataFrame)
+            and self._geometry_column_name in result.columns
+            and any(isinstance(t, GeometryDtype) for t in result.dtypes)
+        ):
+            if self.crs is not None and result.crs is None:
+                result.set_crs(self.crs, inplace=True)
+        return result
+
     @property
     def _constructor(self):
         return GeoDataFrame
 
     def __finalize__(self, other, method=None, **kwargs):
         """propagate metadata from other to self """
+        self = super().__finalize__(other, method=method, **kwargs)
+
         # merge operation: using metadata of the left object
         if method == "merge":
             for name in self._metadata:
                 object.__setattr__(self, name, getattr(other.left, name, None))
         # concat operation: using metadata of the first object
         elif method == "concat":
             for name in self._metadata:
                 object.__setattr__(self, name, getattr(other.objs[0], name, None))
-        else:
-            for name in self._metadata:
-                object.__setattr__(self, name, getattr(other, name, None))
 
         return self
 
-    def plot(self, *args, **kwargs):
-        """Generate a plot of the geometries in the ``GeoDataFrame``.
-
-        If the ``column`` parameter is given, colors plot according to values
-        in that column, otherwise calls ``GeoSeries.plot()`` on the
-        ``geometry`` column.
-
-        Wraps the ``plot_dataframe()`` function, and documentation is copied
-        from there.
-        """
-        return plot_dataframe(self, *args, **kwargs)
-
-    plot.__doc__ = plot_dataframe.__doc__
-
-    def dissolve(self, by=None, aggfunc="first", as_index=True):
+    def dissolve(
+        self,
+        by=None,
+        aggfunc="first",
+        as_index=True,
+        level=None,
+        sort=True,
+        observed=False,
+        dropna=True,
+    ):
         """
         Dissolve geometries within `groupby` into single observation.
         This is accomplished by applying the `unary_union` method
         to all geometries within a groupself.
 
         Observations associated with each `groupby` group will be aggregated
         using the `aggfunc`.
 
         Parameters
         ----------
         by : string, default None
-            Column whose values define groups to be dissolved
+            Column whose values define groups to be dissolved. If None,
+            whole GeoDataFrame is considered a single group.
         aggfunc : function or string, default "first"
             Aggregation function for manipulation of data associated
             with each group. Passed to pandas `groupby.agg` method.
         as_index : boolean, default True
             If true, groupby columns become index of result.
+        level : int or str or sequence of int or sequence of str, default None
+            If the axis is a MultiIndex (hierarchical), group by a
+            particular level or levels.
+
+            .. versionadded:: 0.9.0
+        sort : bool, default True
+            Sort group keys. Get better performance by turning this off.
+            Note this does not influence the order of observations within
+            each group. Groupby preserves the order of rows within each group.
+
+            .. versionadded:: 0.9.0
+        observed : bool, default False
+            This only applies if any of the groupers are Categoricals.
+            If True: only show observed values for categorical groupers.
+            If False: show all values for categorical groupers.
+
+            .. versionadded:: 0.9.0
+        dropna : bool, default True
+            If True, and if group keys contain NA values, NA values
+            together with row/column will be dropped. If False, NA
+            values will also be treated as the key in groups.
+
+            This parameter is not supported for pandas < 1.1.0.
+            A warning will be emitted for earlier pandas versions
+            if a non-default value is given for this parameter.
+
+            .. versionadded:: 0.9.0
 
         Returns
         -------
         GeoDataFrame
+
+        Examples
+        --------
+        >>> from shapely.geometry import Point
+        >>> d = {
+        ...     "col1": ["name1", "name2", "name1"],
+        ...     "geometry": [Point(1, 2), Point(2, 1), Point(0, 1)],
+        ... }
+        >>> gdf = geopandas.GeoDataFrame(d, crs=4326)
+        >>> gdf
+            col1                 geometry
+        0  name1  POINT (1.00000 2.00000)
+        1  name2  POINT (2.00000 1.00000)
+        2  name1  POINT (0.00000 1.00000)
+
+        >>> dissolved = gdf.dissolve('col1')
+        >>> dissolved  # doctest: +SKIP
+                                                    geometry
+        col1
+        name1  MULTIPOINT (0.00000 1.00000, 1.00000 2.00000)
+        name2                        POINT (2.00000 1.00000)
+
+        See also
+        --------
+        GeoDataFrame.explode : explode muti-part geometries into single geometries
+
         """
 
+        if by is None and level is None:
+            by = np.zeros(len(self), dtype="int64")
+
+        groupby_kwargs = dict(
+            by=by, level=level, sort=sort, observed=observed, dropna=dropna
+        )
+        if not compat.PANDAS_GE_11:
+            groupby_kwargs.pop("dropna")
+
+            if not dropna:  # If they passed a non-default dropna value
+                warnings.warn("dropna kwarg is not supported for pandas < 1.1.0")
+
         # Process non-spatial component
         data = self.drop(labels=self.geometry.name, axis=1)
-        aggregated_data = data.groupby(by=by).agg(aggfunc)
+        aggregated_data = data.groupby(**groupby_kwargs).agg(aggfunc)
 
         # Process spatial component
         def merge_geometries(block):
             merged_geom = block.unary_union
             return merged_geom
 
-        g = self.groupby(by=by, group_keys=False)[self.geometry.name].agg(
+        g = self.groupby(group_keys=False, **groupby_kwargs)[self.geometry.name].agg(
             merge_geometries
         )
 
         # Aggregate
         aggregated_geometry = GeoDataFrame(g, geometry=self.geometry.name, crs=self.crs)
         # Recombine
         aggregated = aggregated_geometry.join(aggregated_data)
 
         # Reset if requested
         if not as_index:
             aggregated = aggregated.reset_index()
 
         return aggregated
 
-    # overrides GeoPandasBase method
-    def explode(self):
+    # overrides the pandas native explode method to break up features geometrically
+    def explode(self, column=None, **kwargs):
         """
         Explode muti-part geometries into multiple single geometries.
 
         Each row containing a multi-part geometry will be split into
         multiple rows with single geometries, thereby increasing the vertical
         size of the GeoDataFrame.
 
@@ -986,15 +1528,53 @@
 
         Returns
         -------
         GeoDataFrame
             Exploded geodataframe with each single geometry
             as a separate entry in the geodataframe.
 
+        Examples
+        --------
+
+        >>> from shapely.geometry import MultiPoint
+        >>> d = {
+        ...     "col1": ["name1", "name2"],
+        ...     "geometry": [
+        ...         MultiPoint([(1, 2), (3, 4)]),
+        ...         MultiPoint([(2, 1), (0, 0)]),
+        ...     ],
+        ... }
+        >>> gdf = geopandas.GeoDataFrame(d, crs=4326)
+        >>> gdf
+            col1                                       geometry
+        0  name1  MULTIPOINT (1.00000 2.00000, 3.00000 4.00000)
+        1  name2  MULTIPOINT (2.00000 1.00000, 0.00000 0.00000)
+
+        >>> exploded = gdf.explode()
+        >>> exploded
+              col1                 geometry
+        0 0  name1  POINT (1.00000 2.00000)
+          1  name1  POINT (3.00000 4.00000)
+        1 0  name2  POINT (2.00000 1.00000)
+          1  name2  POINT (0.00000 0.00000)
+
+        See also
+        --------
+        GeoDataFrame.dissolve : dissolve geometries into a single observation.
+
         """
+
+        # If no column is specified then default to the active geometry column
+        if column is None:
+            column = self.geometry.name
+        # If the specified column is not a geometry dtype use pandas explode
+        if not isinstance(self[column].dtype, GeometryDtype):
+            return super(GeoDataFrame, self).explode(column, **kwargs)
+            # TODO: make sure index behaviour is consistent
+
         df_copy = self.copy()
 
         if "level_1" in df_copy.columns:  # GH1393
             df_copy = df_copy.rename(columns={"level_1": "__level_1"})
 
         exploded_geom = df_copy.geometry.explode().reset_index(level=-1)
         exploded_index = exploded_geom.columns[0]
@@ -1057,15 +1637,15 @@
         This method requires SQLAlchemy and GeoAlchemy2, and a PostgreSQL
         Python driver (e.g. psycopg2) to be installed.
 
         Parameters
         ----------
         name : str
             Name of the target table.
-        con : sqlalchemy.engine.Engine
+        con : sqlalchemy.engine.Connection or sqlalchemy.engine.Engine
             Active connection to the PostGIS database.
         if_exists : {'fail', 'replace', 'append'}, default 'fail'
             How to behave if the table already exists:
 
             - fail: Raise a ValueError.
             - replace: Drop the table before inserting new values.
             - append: Insert new values to the existing table.
@@ -1087,16 +1667,22 @@
             should be the SQLAlchemy types.
 
         Examples
         --------
 
         >>> from sqlalchemy import create_engine
         >>> engine = create_engine("postgres://myusername:mypassword@myhost:5432\
-/mydatabase";)
-        >>> gdf.to_postgis("my_table", engine)
+/mydatabase")  # doctest: +SKIP
+        >>> gdf.to_postgis("my_table", engine)  # doctest: +SKIP
+
+        See also
+        --------
+        GeoDataFrame.to_file : write GeoDataFrame to file
+        read_postgis : read PostGIS database to GeoDataFrame
+
         """
         geopandas.io.sql._write_postgis(
             self, name, con, schema, if_exists, index, index_label, chunksize, dtype
         )
 
         #
         # Implement standard operators for GeoSeries
@@ -1135,14 +1721,32 @@
         warnings.warn(
             "'-' operator will be deprecated. Use the 'difference' method instead.",
             DeprecationWarning,
             stacklevel=2,
         )
         return self.geometry.difference(other)
 
+    if compat.PANDAS_GE_025:
+        from pandas.core.accessor import CachedAccessor
+
+        plot = CachedAccessor("plot", geopandas.plotting.GeoplotAccessor)
+    else:
+
+        def plot(self, *args, **kwargs):
+            """Generate a plot of the geometries in the ``GeoDataFrame``.
+            If the ``column`` parameter is given, colors plot according to values
+            in that column, otherwise calls ``GeoSeries.plot()`` on the
+            ``geometry`` column.
+            Wraps the ``plot_dataframe()`` function, and documentation is copied
+            from there.
+            """
+            return plot_dataframe(self, *args, **kwargs)
+
+    plot.__doc__ = plot_dataframe.__doc__
+
 
 def _dataframe_set_geometry(self, col, drop=False, inplace=False, crs=None):
     if inplace:
         raise ValueError(
             "Can't do inplace setting when converting from DataFrame to GeoDataFrame"
         )
     gf = GeoDataFrame(self)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `geopandas-0.8.2/geopandas/io/arrow.py` & `geopandas-0.9.0/geopandas/io/arrow.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.version import LooseVersion
 import json
 import warnings
 
 from pandas import DataFrame
 
 from geopandas._compat import import_optional_dependency
-from geopandas.array import from_wkb, to_wkb
+from geopandas.array import from_wkb
 from geopandas import GeoDataFrame
 import geopandas
 
 
 METADATA_VERSION = "0.1.0"
 # reference: https://github.com/geopandas/geo-arrow-spec
 
@@ -72,36 +72,14 @@
     Returns
     -------
     UTF-8 encoded JSON string
     """
     return json.dumps(metadata).encode("utf-8")
 
 
-def _encode_wkb(df):
-    """Encode all geometry columns in the GeoDataFrame to WKB.
-
-    Parameters
-    ----------
-    df : GeoDataFrame
-
-    Returns
-    -------
-    DataFrame
-        geometry columns are encoded to WKB
-    """
-
-    df = DataFrame(df.copy())
-
-    # Encode all geometry columns to WKB
-    for col in df.columns[df.dtypes == "geometry"]:
-        df[col] = to_wkb(df[col].values)
-
-    return df
-
-
 def _decode_metadata(metadata_str):
     """Decode a UTF-8 encoded JSON string to dict
 
     Parameters
     ----------
     metadata_str : string (UTF-8 encoded)
 
@@ -204,15 +182,15 @@
     )
 
     _validate_dataframe(df)
 
     # create geo metadata before altering incoming data frame
     geo_metadata = _create_metadata(df)
 
-    df = _encode_wkb(df)
+    df = df.to_wkb()
 
     table = Table.from_pandas(df, preserve_index=index)
 
     # Store geopandas specific file-level metadata
     # This must be done AFTER creating the table or it is not persisted
     metadata = table.schema.metadata
     metadata.update({b"geo": _encode_metadata(geo_metadata)})
@@ -390,14 +368,25 @@
         a ``ValueError`` will be raised.
     **kwargs
         Any additional kwargs passed to pyarrow.parquet.read_table().
 
     Returns
     -------
     GeoDataFrame
+
+    Examples
+    --------
+    >>> df = geopandas.read_parquet("data.parquet")  # doctest: +SKIP
+
+    Specifying columns to read:
+
+    >>> df = geopandas.read_parquet(
+    ...     "data.parquet",
+    ...     columns=["geometry", "pop_est"]
+    ... )  # doctest: +SKIP
     """
 
     parquet = import_optional_dependency(
         "pyarrow.parquet", extra="pyarrow is required for Parquet support."
     )
 
     kwargs["use_pandas_metadata"] = True
@@ -435,14 +424,25 @@
         a ``ValueError`` will be raised.
     **kwargs
         Any additional kwargs passed to pyarrow.feather.read_table().
 
     Returns
     -------
     GeoDataFrame
+
+    Examples
+    --------
+    >>> df = geopandas.read_feather("data.feather")  # doctest: +SKIP
+
+    Specifying columns to read:
+
+    >>> df = geopandas.read_feather(
+    ...     "data.feather",
+    ...     columns=["geometry", "pop_est"]
+    ... )  # doctest: +SKIP
     """
 
     feather = import_optional_dependency(
         "pyarrow.feather", extra="pyarrow is required for Feather support."
     )
     # TODO move this into `import_optional_dependency`
     import pyarrow
```

### Comparing `geopandas-0.8.2/geopandas/io/file.py` & `geopandas-0.9.0/geopandas/io/file.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,72 @@
 from distutils.version import LooseVersion
 
-import io
+import warnings
 import numpy as np
 import pandas as pd
 
-import fiona
 import pyproj
 from shapely.geometry import mapping
 from shapely.geometry.base import BaseGeometry
 
 try:
+    import fiona
+
+    fiona_import_error = None
+except ImportError as err:
+    fiona = None
+    fiona_import_error = str(err)
+
+try:
     from fiona import Env as fiona_env
 except ImportError:
-    from fiona import drivers as fiona_env
+    try:
+        from fiona import drivers as fiona_env
+    except ImportError:
+        fiona_env = None
 
 from geopandas import GeoDataFrame, GeoSeries
 
 
 # Adapted from pandas.io.common
 from urllib.request import urlopen as _urlopen
 from urllib.parse import urlparse as parse_url
 from urllib.parse import uses_netloc, uses_params, uses_relative
 
 
-_FIONA18 = LooseVersion(fiona.__version__) >= LooseVersion("1.8")
 _VALID_URLS = set(uses_relative + uses_netloc + uses_params)
 _VALID_URLS.discard("")
 
 
+def _check_fiona(func):
+    if fiona is None:
+        raise ImportError(
+            f"the {func} requires the 'fiona' package, but it is not installed or does "
+            f"not import correctly.\nImporting fiona resulted in: {fiona_import_error}"
+        )
+
+
 def _is_url(url):
     """Check to see if *url* has a valid protocol."""
     try:
         return parse_url(url).scheme in _VALID_URLS
     except Exception:
         return False
 
 
+def _is_zip(path):
+    """Check if a given path is a zipfile"""
+    parsed = fiona.path.ParsedPath.from_uri(path)
+    return (
+        parsed.archive.endswith(".zip")
+        if parsed.archive
+        else parsed.path.endswith(".zip")
+    )
+
+
 def _read_file(filename, bbox=None, mask=None, rows=None, **kwargs):
     """
     Returns a GeoDataFrame from a file or URL.
 
     .. versionadded:: 0.7.0 mask, rows
 
     Parameters
@@ -64,35 +91,72 @@
         Keyword args to be passed to the `open` or `BytesCollection` method
         in the fiona library when opening the file. For more information on
         possible keywords, type:
         ``import fiona; help(fiona.open)``
 
     Examples
     --------
-    >>> df = geopandas.read_file("nybb.shp")
+    >>> df = geopandas.read_file("nybb.shp")  # doctest: +SKIP
+
+    Specifying layer of GPKG:
+
+    >>> df = geopandas.read_file("file.gpkg", layer='cities')  # doctest: +SKIP
+
+    Reading only first 10 rows:
+
+    >>> df = geopandas.read_file("nybb.shp", rows=10)  # doctest: +SKIP
+
+    Reading only geometries intersecting ``mask``:
+
+    >>> df = geopandas.read_file("nybb.shp", mask=polygon)  # doctest: +SKIP
+
+    Reading only geometries intersecting ``bbox``:
+
+    >>> df = geopandas.read_file("nybb.shp", bbox=(0, 10, 0, 20))  # doctest: +SKIP
 
     Returns
     -------
     :obj:`geopandas.GeoDataFrame` or :obj:`pandas.DataFrame` :
         If `ignore_geometry=True` a :obj:`pandas.DataFrame` will be returned.
 
     Notes
     -----
     The format drivers will attempt to detect the encoding of your data, but
     may fail. In this case, the proper encoding can be specified explicitly
     by using the encoding keyword parameter, e.g. ``encoding='utf-8'``.
     """
+    _check_fiona("'read_file' function")
     if _is_url(filename):
         req = _urlopen(filename)
         path_or_bytes = req.read()
         reader = fiona.BytesCollection
-    elif isinstance(filename, io.TextIOBase):
-        path_or_bytes = filename.read()
-        reader = fiona.open
+    elif pd.api.types.is_file_like(filename):
+        data = filename.read()
+        path_or_bytes = data.encode("utf-8") if isinstance(data, str) else data
+        reader = fiona.BytesCollection
     else:
+        # Opening a file via URL or file-like-object above automatically detects a
+        # zipped file. In order to match that behavior, attempt to add a zip scheme
+        # if missing.
+        if _is_zip(str(filename)):
+            parsed = fiona.parse_path(str(filename))
+            if isinstance(parsed, fiona.path.ParsedPath):
+                # If fiona is able to parse the path, we can safely look at the scheme
+                # and update it to have a zip scheme if necessary.
+                schemes = (parsed.scheme or "").split("+")
+                if "zip" not in schemes:
+                    parsed.scheme = "+".join(["zip"] + schemes)
+                filename = parsed.name
+            elif isinstance(parsed, fiona.path.UnparsedPath) and not str(
+                filename
+            ).startswith("/vsi"):
+                # If fiona is unable to parse the path, it might have a Windows drive
+                # scheme. Try adding zip:// to the front. If the path starts with "/vsi"
+                # it is a legacy GDAL path type, so let it pass unmodified.
+                filename = "zip://" + parsed.name
         path_or_bytes = filename
         reader = fiona.open
 
     with fiona_env():
         with reader(path_or_bytes, **kwargs) as features:
 
             # In a future Fiona release the crs attribute of features will
@@ -172,22 +236,22 @@
     df,
     filename,
     driver="ESRI Shapefile",
     schema=None,
     index=None,
     mode="w",
     crs=None,
-    **kwargs
+    **kwargs,
 ):
     """
     Write this GeoDataFrame to an OGR data source
 
     A dictionary of supported OGR providers is available via:
     >>> import fiona
-    >>> fiona.supported_drivers
+    >>> fiona.supported_drivers  # doctest: +SKIP
 
     Parameters
     ----------
     df : GeoDataFrame to be written
     filename : string
         File path or file handle to write to.
     driver : string, default 'ESRI Shapefile'
@@ -223,28 +287,37 @@
 
     Notes
     -----
     The format drivers will attempt to detect the encoding of your data, but
     may fail. In this case, the proper encoding can be specified explicitly
     by using the encoding keyword parameter, e.g. ``encoding='utf-8'``.
     """
+    _check_fiona("'to_file' method")
     if index is None:
         # Determine if index attribute(s) should be saved to file
         index = list(df.index.names) != [None] or type(df.index) not in (
             pd.RangeIndex,
             pd.Int64Index,
         )
     if index:
         df = df.reset_index(drop=False)
     if schema is None:
         schema = infer_schema(df)
     if crs:
         crs = pyproj.CRS.from_user_input(crs)
     else:
         crs = df.crs
+
+    if driver == "ESRI Shapefile" and any([len(c) > 10 for c in df.columns.tolist()]):
+        warnings.warn(
+            "Column names longer than 10 characters will be truncated when saved to "
+            "ESRI Shapefile.",
+            stacklevel=3,
+        )
+
     with fiona_env():
         crs_wkt = None
         try:
             gdal_version = fiona.env.get_gdal_release_name()
         except AttributeError:
             gdal_version = "2.0.0"  # just assume it is not the latest
         if LooseVersion(gdal_version) >= LooseVersion("3.0.0") and crs:
@@ -271,20 +344,14 @@
             return "datetime"
         if str(in_type) in types:
             out_type = types[str(in_type)]
         else:
             out_type = type(np.zeros(1, in_type).item()).__name__
         if out_type == "long":
             out_type = "int"
-        if not _FIONA18 and out_type == "bool":
-            raise ValueError(
-                'column "{}" is boolean type, '.format(column)
-                + "which is unsupported in file writing with fiona "
-                "< 1.8. Consider casting the column to int type."
-            )
         return out_type
 
     properties = OrderedDict(
         [
             (col, convert_type(col, _type))
             for col, _type in zip(df.columns, df.dtypes)
             if col != df._geometry_column_name
@@ -303,57 +370,22 @@
     return schema
 
 
 def _geometry_types(df):
     """
     Determine the geometry types in the GeoDataFrame for the schema.
     """
-    if _FIONA18:
-        # Starting from Fiona 1.8, schema submitted to fiona to write a gdf
-        # can have mixed geometries:
-        # - 3D and 2D shapes can coexist in inferred schema
-        # - Shape and MultiShape types can (and must) coexist in inferred
-        #   schema
-        geom_types_2D = df[~df.geometry.has_z].geometry.geom_type.unique()
-        geom_types_2D = [gtype for gtype in geom_types_2D if gtype is not None]
-        geom_types_3D = df[df.geometry.has_z].geometry.geom_type.unique()
-        geom_types_3D = ["3D " + gtype for gtype in geom_types_3D if gtype is not None]
-        geom_types = geom_types_3D + geom_types_2D
-
-    else:
-        # Before Fiona 1.8, schema submitted to write a gdf should have
-        # one single geometry type whenever possible:
-        # - 3D and 2D shapes cannot coexist in inferred schema
-        # - Shape and MultiShape can not coexist in inferred schema
-        geom_types = _geometry_types_back_compat(df)
+    geom_types_2D = df[~df.geometry.has_z].geometry.geom_type.unique()
+    geom_types_2D = [gtype for gtype in geom_types_2D if gtype is not None]
+    geom_types_3D = df[df.geometry.has_z].geometry.geom_type.unique()
+    geom_types_3D = ["3D " + gtype for gtype in geom_types_3D if gtype is not None]
+    geom_types = geom_types_3D + geom_types_2D
 
     if len(geom_types) == 0:
         # Default geometry type supported by Fiona
         # (Since https://github.com/Toblerity/Fiona/issues/446 resolution)
         return "Unknown"
 
     if len(geom_types) == 1:
         geom_types = geom_types[0]
 
     return geom_types
-
-
-def _geometry_types_back_compat(df):
-    """
-    for backward compatibility with Fiona<1.8 only
-    """
-    unique_geom_types = df.geometry.geom_type.unique()
-    unique_geom_types = [gtype for gtype in unique_geom_types if gtype is not None]
-
-    # merge single and Multi types (eg Polygon and MultiPolygon)
-    unique_geom_types = [
-        gtype
-        for gtype in unique_geom_types
-        if not gtype.startswith("Multi") or gtype[5:] not in unique_geom_types
-    ]
-
-    if df.geometry.has_z.any():
-        # declare all geometries as 3D geometries
-        unique_geom_types = ["3D " + type for type in unique_geom_types]
-    # by default, all geometries are 2D geometries
-
-    return unique_geom_types
```

### Comparing `geopandas-0.8.2/geopandas/io/sql.py` & `geopandas-0.9.0/geopandas/io/sql.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,48 @@
 import warnings
+from contextlib import contextmanager
 
 import pandas as pd
 
 import shapely.wkb
 
 from geopandas import GeoDataFrame
 
 from .. import _compat as compat
 
 
+@contextmanager
+def _get_conn(conn_or_engine):
+    """
+    Yield a connection within a transaction context.
+
+    Engine.begin() returns a Connection with an implicit Transaction while
+    Connection.begin() returns the Transaction. This helper will always return a
+    Connection with an implicit (possibly nested) Transaction.
+
+    Parameters
+    ----------
+    conn_or_engine : Connection or Engine
+        A sqlalchemy Connection or Engine instance
+    Returns
+    -------
+    Connection
+    """
+    from sqlalchemy.engine.base import Engine, Connection
+
+    if isinstance(conn_or_engine, Connection):
+        with conn_or_engine.begin():
+            yield conn_or_engine
+    elif isinstance(conn_or_engine, Engine):
+        with conn_or_engine.begin() as conn:
+            yield conn
+    else:
+        raise ValueError(f"Unknown Connectable: {conn_or_engine}")
+
+
 def _df_to_geodf(df, geom_col="geom", crs=None):
     """
     Transforms a pandas DataFrame into a GeoDataFrame.
     The column 'geom_col' must be a geometry column in WKB representation.
     To be used to convert df based on pd.read_sql to gdf.
     Parameters
     ----------
@@ -79,15 +109,15 @@
     string, which must contain a geometry column in WKB representation.
 
     Parameters
     ----------
     sql : string
         SQL query to execute in selecting entries from database, or name
         of the table to read from the database.
-    con : DB connection object or SQLAlchemy engine
+    con : sqlalchemy.engine.Connection or sqlalchemy.engine.Engine
         Active connection to the database to query.
     geom_col : string, default 'geom'
         column name to convert to shapely geometries
     crs : dict or str, optional
         CRS to use for the returned GeoDataFrame; if not set, tries to
         determine CRS from the SRID associated with the first geometry in
         the database, and assigns that to all geometries.
@@ -102,18 +132,25 @@
     Returns
     -------
     GeoDataFrame
 
     Examples
     --------
     PostGIS
-    >>> sql = "SELECT geom, kind FROM polygons"
+
+    >>> from sqlalchemy import create_engine  # doctest: +SKIP
+    >>> db_connection_url = "postgres://myusername:mypassword@myhost:5432/mydatabase"
+    >>> con = create_engine(db_connection_url)  # doctest: +SKIP
+    >>> sql = "SELECT geom, highway FROM roads"
+    >>> df = geopandas.read_postgis(sql, con)  # doctest: +SKIP
+
     SpatiaLite
-    >>> sql = "SELECT ST_AsBinary(geom) AS geom, kind FROM polygons"
-    >>> df = geopandas.read_postgis(sql, con)
+
+    >>> sql = "SELECT ST_Binary(geom) AS geom, highway FROM roads"
+    >>> df = geopandas.read_postgis(sql, con)  # doctest: +SKIP
     """
 
     if chunksize is None:
         # read all in one chunk and return a single GeoDataFrame
         df = pd.read_sql(
             sql,
             con,
@@ -166,15 +203,15 @@
      - in all other cases, geometries will be inserted with type GEOMETRY:
         - a mix of Polygons and MultiPolygons in GeoSeries
         - a mix of Points and LineStrings in GeoSeries
         - geometry is of type GeometryCollection,
           such as GeometryCollection([Point, LineStrings])
      - if any of the geometries has Z-coordinate, all records will
        be written with 3D.
-     """
+    """
     geom_types = list(gdf.geometry.geom_type.unique())
     has_curve = False
 
     for gt in geom_types:
         if gt is None:
             continue
         elif "LinearRing" in gt:
@@ -265,15 +302,17 @@
     writer.writerows(data_iter)
     s_buf.seek(0)
 
     columns = ", ".join('"{}"'.format(k) for k in keys)
 
     dbapi_conn = conn.connection
     with dbapi_conn.cursor() as cur:
-        sql = "COPY {} ({}) FROM STDIN WITH CSV".format(tbl.table.fullname, columns)
+        sql = 'COPY "{}"."{}" ({}) FROM STDIN WITH CSV'.format(
+            tbl.table.schema, tbl.table.name, columns
+        )
         cur.copy_expert(sql=sql, file=s_buf)
 
 
 def _write_postgis(
     gdf,
     name,
     con,
@@ -290,15 +329,15 @@
     This method requires SQLAlchemy and GeoAlchemy2, and a PostgreSQL
     Python driver (e.g. psycopg2) to be installed.
 
     Parameters
     ----------
     name : str
         Name of the target table.
-    con : sqlalchemy.engine.Engine
+    con : sqlalchemy.engine.Connection or sqlalchemy.engine.Engine
         Active connection to the PostGIS database.
     if_exists : {'fail', 'replace', 'append'}, default 'fail'
         How to behave if the table already exists:
 
         - fail: Raise a ValueError.
         - replace: Drop the table before inserting new values.
         - append: Insert new values to the existing table.
@@ -318,18 +357,18 @@
         Specifying the datatype for columns.
         The keys should be the column names and the values
         should be the SQLAlchemy types.
 
     Examples
     --------
 
-    >>> from sqlalchemy import create_engine
+    >>> from sqlalchemy import create_engine  # doctest: +SKIP
     >>> engine = create_engine("postgres://myusername:mypassword@myhost:5432\
-/mydatabase";)
-    >>> gdf.to_postgis("my_table", engine)
+/mydatabase";)  # doctest: +SKIP
+    >>> gdf.to_postgis("my_table", engine)  # doctest: +SKIP
     """
     try:
         from geoalchemy2 import Geometry
     except ImportError:
         raise ImportError("'to_postgis()' requires geoalchemy2 package. ")
 
     if not compat.SHAPELY_GE_17:
@@ -358,24 +397,24 @@
     # Convert LinearRing geometries to LineString
     if has_curve:
         gdf = _convert_linearring_to_linestring(gdf, geom_name)
 
     # Convert geometries to EWKB
     gdf = _convert_to_ewkb(gdf, geom_name, srid)
 
+    if schema is not None:
+        schema_name = schema
+    else:
+        schema_name = "public"
+
     if if_exists == "append":
         # Check that the geometry srid matches with the current GeoDataFrame
-        with con.begin() as connection:
-            if schema is not None:
-                schema_name = schema
-            else:
-                schema_name = "public"
-
+        with _get_conn(con) as connection:
             # Only check SRID if table exists
-            if connection.run_callable(connection.dialect.has_table, name, schema):
+            if connection.dialect.has_table(connection, name, schema):
                 target_srid = connection.execute(
                     "SELECT Find_SRID('{schema}', '{table}', '{geom_col}');".format(
                         schema=schema_name, table=name, geom_col=geom_name
                     )
                 ).fetchone()[0]
 
                 if target_srid != srid:
@@ -383,20 +422,20 @@
                         "The CRS of the target table (EPSG:{epsg_t}) differs from the "
                         "CRS of current GeoDataFrame (EPSG:{epsg_src}).".format(
                             epsg_t=target_srid, epsg_src=srid
                         )
                     )
                     raise ValueError(msg)
 
-    with con.begin() as connection:
+    with _get_conn(con) as connection:
 
         gdf.to_sql(
             name,
             connection,
-            schema=schema,
+            schema=schema_name,
             if_exists=if_exists,
             index=index,
             index_label=index_label,
             chunksize=chunksize,
             dtype=dtype,
             method=_psql_insert_copy,
         )
```

### Comparing `geopandas-0.8.2/geopandas/plotting.py` & `geopandas-0.9.0/geopandas/plotting.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,16 +41,16 @@
     """
     components, component_index = [], []
 
     if not geoms.geom_type.str.startswith(prefix).any():
         return geoms, np.arange(len(geoms))
 
     for ix, geom in enumerate(geoms):
-        if geom.type.startswith(prefix):
-            for poly in geom:
+        if geom is not None and geom.type.startswith(prefix) and not geom.is_empty:
+            for poly in geom.geoms:
                 components.append(poly)
                 component_index.append(ix)
         else:
             components.append(geom)
             component_index.append(ix)
 
     return components, np.array(component_index)
@@ -59,37 +59,71 @@
 def _expand_kwargs(kwargs, multiindex):
     """
     Most arguments to the plot functions must be a (single) value, or a sequence
     of values. This function checks each key-value pair in 'kwargs' and expands
     it (in place) to the correct length/formats with help of 'multiindex', unless
     the value appears to already be a valid (single) value for the key.
     """
+    import matplotlib
     from matplotlib.colors import is_color_like
     from typing import Iterable
 
+    mpl = matplotlib.__version__
+    if mpl >= LooseVersion("3.4") or (mpl > LooseVersion("3.3.2") and "+" in mpl):
+        # alpha is supported as array argument with matplotlib 3.4+
+        scalar_kwargs = ["marker"]
+    else:
+        scalar_kwargs = ["marker", "alpha"]
+
     for att, value in kwargs.items():
         if "color" in att:  # color(s), edgecolor(s), facecolor(s)
             if is_color_like(value):
                 continue
         elif "linestyle" in att:  # linestyle(s)
             # A single linestyle can be 2-tuple of a number and an iterable.
             if (
                 isinstance(value, tuple)
                 and len(value) == 2
                 and isinstance(value[1], Iterable)
             ):
                 continue
-        elif att in ["marker", "alpha"]:
+        elif att in scalar_kwargs:
             # For these attributes, only a single value is allowed, so never expand.
             continue
 
         if pd.api.types.is_list_like(value):
             kwargs[att] = np.take(value, multiindex, axis=0)
 
 
+def _PolygonPatch(polygon, **kwargs):
+    """Constructs a matplotlib patch from a Polygon geometry
+
+    The `kwargs` are those supported by the matplotlib.patches.PathPatch class
+    constructor. Returns an instance of matplotlib.patches.PathPatch.
+
+    Example (using Shapely Point and a matplotlib axes)::
+
+        b = shapely.geometry.Point(0, 0).buffer(1.0)
+        patch = _PolygonPatch(b, fc='blue', ec='blue', alpha=0.5)
+        ax.add_patch(patch)
+
+    GeoPandas originally relied on the descartes package by Sean Gillies
+    (BSD license, https://pypi.org/project/descartes) for PolygonPatch, but
+    this dependency was removed in favor of the below matplotlib code.
+    """
+    from matplotlib.patches import PathPatch
+    from matplotlib.path import Path
+
+    path = Path.make_compound_path(
+        Path(np.asarray(polygon.exterior.coords)[:, :2]),
+        *[Path(np.asarray(ring.coords)[:, :2]) for ring in polygon.interiors],
+    )
+    return PathPatch(path, **kwargs)
+
+
 def _plot_polygon_collection(
     ax, geoms, values=None, color=None, cmap=None, vmin=None, vmax=None, **kwargs
 ):
     """
     Plots a collection of Polygon and MultiPolygon geometries to `ax`
 
     Parameters
@@ -111,23 +145,14 @@
     **kwargs
         Additional keyword arguments passed to the collection
 
     Returns
     -------
     collection : matplotlib.collections.Collection that was plotted
     """
-
-    try:
-        from descartes.patch import PolygonPatch
-    except ImportError:
-        raise ImportError(
-            "The descartes package is required for plotting polygons in geopandas. "
-            "You can install it using 'conda install -c conda-forge descartes' or "
-            "'pip install descartes'."
-        )
     from matplotlib.collections import PatchCollection
 
     geoms, multiindex = _flatten_multi_geoms(geoms)
     if values is not None:
         values = np.take(values, multiindex, axis=0)
 
     # PatchCollection does not accept some kwargs.
@@ -139,15 +164,17 @@
 
     # Add to kwargs for easier checking below.
     if color is not None:
         kwargs["color"] = color
 
     _expand_kwargs(kwargs, multiindex)
 
-    collection = PatchCollection([PolygonPatch(poly) for poly in geoms], **kwargs)
+    collection = PatchCollection(
+        [_PolygonPatch(poly) for poly in geoms if not poly.is_empty], **kwargs
+    )
 
     if values is not None:
         collection.set_array(np.asarray(values))
         collection.set_cmap(cmap)
         if "norm" not in kwargs:
             collection.set_clim(vmin, vmax)
 
@@ -196,15 +223,15 @@
 
     # Add to kwargs for easier checking below.
     if color is not None:
         kwargs["color"] = color
 
     _expand_kwargs(kwargs, multiindex)
 
-    segments = [np.array(linestring)[:, :2] for linestring in geoms]
+    segments = [np.array(linestring.coords)[:, :2] for linestring in geoms]
     collection = LineCollection(segments, **kwargs)
 
     if values is not None:
         collection.set_array(np.asarray(values))
         collection.set_cmap(cmap)
         if "norm" not in kwargs:
             collection.set_clim(vmin, vmax)
@@ -223,15 +250,15 @@
     values=None,
     color=None,
     cmap=None,
     vmin=None,
     vmax=None,
     marker="o",
     markersize=None,
-    **kwargs
+    **kwargs,
 ):
     """
     Plots a collection of Point and MultiPoint geometries to `ax`
 
     Parameters
     ----------
     ax : matplotlib.axes.Axes
@@ -250,19 +277,18 @@
     -------
     collection : matplotlib.collections.Collection that was plotted
     """
     if values is not None and color is not None:
         raise ValueError("Can only specify one of 'values' and 'color' kwargs")
 
     geoms, multiindex = _flatten_multi_geoms(geoms)
-    if values is not None:
-        values = np.take(values, multiindex, axis=0)
+    # values are expanded below as kwargs["c"]
 
-    x = [p.x for p in geoms]
-    y = [p.y for p in geoms]
+    x = [p.x if not p.is_empty else None for p in geoms]
+    y = [p.y if not p.is_empty else None for p in geoms]
 
     # matplotlib 1.4 does not support c=None, and < 2.0 does not support s=None
     if values is not None:
         kwargs["c"] = values
     if markersize is not None:
         kwargs["s"] = markersize
 
@@ -309,22 +335,22 @@
     color : str (default None)
         If specified, all objects will be colored uniformly.
     ax : matplotlib.pyplot.Artist (default None)
         axes on which to draw the plot
     figsize : pair of floats (default None)
         Size of the resulting matplotlib.figure.Figure. If the argument
         ax is given explicitly, figsize is ignored.
-    aspect : 'auto', 'equal' or float (default 'auto')
+    aspect : 'auto', 'equal', None or float (default 'auto')
         Set aspect of axis. If 'auto', the default aspect for map plots is 'equal'; if
         however data are not projected (coordinates are long/lat), the aspect is by
         default set to 1/cos(s_y * pi/180) with s_y the y coordinate of the middle of
         the GeoSeries (the mean of the y range of bounding box) so that a long/lat
         square appears square in the middle of the plot. This implies an
-        Equirectangular projection. It can also be set manually (float) as the ratio
-        of y-unit to x-unit.
+        Equirectangular projection. If None, the aspect of `ax` won't be changed. It can
+        also be set manually (float) as the ratio of y-unit to x-unit.
     **style_kwds : dict
         Color options to be passed on to the actual plot function, such
         as ``edgecolor``, ``facecolor``, ``linewidth``, ``markersize``,
         ``alpha``.
 
     Returns
     -------
@@ -362,25 +388,33 @@
             bounds = s.total_bounds
             y_coord = np.mean([bounds[1], bounds[3]])
             ax.set_aspect(1 / np.cos(y_coord * np.pi / 180))
             # formula ported from R package sp
             # https://github.com/edzer/sp/blob/master/R/mapasp.R
         else:
             ax.set_aspect("equal")
-    else:
+    elif aspect is not None:
         ax.set_aspect(aspect)
 
     if s.empty:
         warnings.warn(
             "The GeoSeries you are attempting to plot is "
             "empty. Nothing has been displayed.",
             UserWarning,
         )
         return ax
 
+    if s.is_empty.all():
+        warnings.warn(
+            "The GeoSeries you are attempting to plot is "
+            "composed of empty geometries. Nothing has been displayed.",
+            UserWarning,
+        )
+        return ax
+
     # if cmap is specified, create range of colors based on cmap
     values = None
     if cmap is not None:
         values = np.arange(len(s))
         if hasattr(cmap, "N"):
             values = values % cmap.N
         style_kwds["vmin"] = style_kwds.get("vmin", values.min())
@@ -450,34 +484,45 @@
     markersize=None,
     figsize=None,
     legend_kwds=None,
     categories=None,
     classification_kwds=None,
     missing_kwds=None,
     aspect="auto",
-    **style_kwds
+    **style_kwds,
 ):
     """
     Plot a GeoDataFrame.
 
     Generate a plot of a GeoDataFrame with matplotlib.  If a
     column is specified, the plot coloring will be based on values
     in that column.
 
     Parameters
     ----------
-    df : GeoDataFrame
-        The GeoDataFrame to be plotted.  Currently Polygon,
-        MultiPolygon, LineString, MultiLineString and Point
-        geometries can be plotted.
     column : str, np.array, pd.Series (default None)
         The name of the dataframe column, np.array, or pd.Series to be plotted.
         If np.array or pd.Series are used then it must have same length as
         dataframe. Values are used to color the plot. Ignored if `color` is
         also set.
+    kind: str
+        The kind of plots to produce:
+         - 'geo': Map (default)
+         Pandas Kinds
+         - 'line' : line plot
+         - 'bar' : vertical bar plot
+         - 'barh' : horizontal bar plot
+         - 'hist' : histogram
+         - 'box' : BoxPlot
+         - 'kde' : Kernel Density Estimation plot
+         - 'density' : same as 'kde'
+         - 'area' : area plot
+         - 'pie' : pie plot
+         - 'scatter' : scatter plot
+         - 'hexbin' : hexbin plot.
     cmap : str (default None)
         The name of a colormap recognized by matplotlib.
     color : str (default None)
         If specified, all objects will be colored uniformly.
     ax : matplotlib.pyplot.Artist (default None)
         axes on which to draw the plot
     cax : matplotlib.pyplot Artist (default None)
@@ -522,41 +567,65 @@
         fmt : string
             A formatting specification for the bin edges of the classes in the
             legend. For example, to have no decimals: ``{"fmt": "{:.0f}"}``.
         labels : list-like
             A list of legend labels to override the auto-generated labels.
             Needs to have the same number of elements as the number of
             classes (`k`).
+        interval : boolean (default False)
+            An option to control brackets from mapclassify legend.
+            If True, open/closed interval brackets are shown in the legend.
     categories : list-like
         Ordered list-like object of categories to be used for categorical plot.
     classification_kwds : dict (default None)
         Keyword arguments to pass to mapclassify
     missing_kwds : dict (default None)
         Keyword arguments specifying color options (as style_kwds)
         to be passed on to geometries with missing values in addition to
         or overwriting other style kwds. If None, geometries with missing
         values are not plotted.
-    aspect : 'auto', 'equal' or float (default 'auto')
+    aspect : 'auto', 'equal', None or float (default 'auto')
         Set aspect of axis. If 'auto', the default aspect for map plots is 'equal'; if
         however data are not projected (coordinates are long/lat), the aspect is by
         default set to 1/cos(df_y * pi/180) with df_y the y coordinate of the middle of
         the GeoDataFrame (the mean of the y range of bounding box) so that a long/lat
         square appears square in the middle of the plot. This implies an
-        Equirectangular projection. It can also be set manually (float) as the ratio
-        of y-unit to x-unit.
+        Equirectangular projection. If None, the aspect of `ax` won't be changed. It can
+        also be set manually (float) as the ratio of y-unit to x-unit.
 
     **style_kwds : dict
         Style options to be passed on to the actual plot function, such
         as ``edgecolor``, ``facecolor``, ``linewidth``, ``markersize``,
         ``alpha``.
 
     Returns
     -------
     ax : matplotlib axes instance
 
+    Examples
+    --------
+    >>> df = geopandas.read_file(geopandas.datasets.get_path("naturalearth_lowres"))
+    >>> df.head()  # doctest: +SKIP
+        pop_est      continent                      name iso_a3  \
+gdp_md_est                                           geometry
+    0     920938        Oceania                      Fiji    FJI      8374.0  MULTIPOLY\
+GON (((180.00000 -16.06713, 180.00000...
+    1   53950935         Africa                  Tanzania    TZA    150600.0  POLYGON (\
+(33.90371 -0.95000, 34.07262 -1.05982...
+    2     603253         Africa                 W. Sahara    ESH       906.5  POLYGON (\
+(-8.66559 27.65643, -8.66512 27.58948...
+    3   35623680  North America                    Canada    CAN   1674000.0  MULTIPOLY\
+GON (((-122.84000 49.00000, -122.9742...
+    4  326625791  North America  United States of America    USA  18560000.0  MULTIPOLY\
+GON (((-122.84000 49.00000, -120.0000...
+
+    >>> df.plot("pop_est", cmap="Blues")  # doctest: +SKIP
+
+    See the User Guide page :doc:`../../user_guide/mapping` for details.
+
     """
     if "colormap" in style_kwds:
         warnings.warn(
             "'colormap' is deprecated, please use 'cmap' instead "
             "(for consistency with matplotlib)",
             FutureWarning,
         )
@@ -593,17 +662,22 @@
             bounds = df.total_bounds
             y_coord = np.mean([bounds[1], bounds[3]])
             ax.set_aspect(1 / np.cos(y_coord * np.pi / 180))
             # formula ported from R package sp
             # https://github.com/edzer/sp/blob/master/R/mapasp.R
         else:
             ax.set_aspect("equal")
-    else:
+    elif aspect is not None:
         ax.set_aspect(aspect)
 
+    # GH 1555
+    # if legend_kwds set, copy so we don't update it in place
+    if legend_kwds is not None:
+        legend_kwds = legend_kwds.copy()
+
     if df.empty:
         warnings.warn(
             "The GeoDataFrame you are attempting to plot is "
             "empty. Nothing has been displayed.",
             UserWarning,
         )
         return ax
@@ -616,25 +690,29 @@
             df.geometry,
             cmap=cmap,
             color=color,
             ax=ax,
             figsize=figsize,
             markersize=markersize,
             aspect=aspect,
-            **style_kwds
+            **style_kwds,
         )
 
     # To accept pd.Series and np.arrays as column
     if isinstance(column, (np.ndarray, pd.Series)):
         if column.shape[0] != df.shape[0]:
             raise ValueError(
                 "The dataframe and given column have different number of rows."
             )
         else:
             values = column
+
+            # Make sure index of a Series matches index of df
+            if isinstance(values, pd.Series):
+                values = values.reindex(df.index)
     else:
         values = df[column]
 
     if pd.api.types.is_categorical_dtype(values.dtype):
         if categories is not None:
             raise ValueError(
                 "Cannot specify 'categories' when column has categorical dtype"
@@ -684,15 +762,22 @@
                 )
             else:
                 categories = list(legend_kwds.pop("labels"))
         else:
             fmt = "{:.2f}"
             if legend_kwds is not None and "fmt" in legend_kwds:
                 fmt = legend_kwds.pop("fmt")
+
             categories = binning.get_legend_classes(fmt)
+            if legend_kwds is not None:
+                show_interval = legend_kwds.pop("interval", False)
+            else:
+                show_interval = False
+            if not show_interval:
+                categories = [c[1:-1] for c in categories]
         values = np.array(binning.yb)
 
     # fill values with placeholder where were NaNs originally to map them properly
     # (after removing them in categorical or scheme)
     if categorical:
         for n in np.where(nan_idx)[0]:
             values = np.insert(values, n, values[0])
@@ -742,18 +827,18 @@
             ax,
             points,
             subset,
             vmin=mn,
             vmax=mx,
             markersize=markersize,
             cmap=cmap,
-            **style_kwds
+            **style_kwds,
         )
 
-    if missing_kwds is not None:
+    if missing_kwds is not None and not expl_series[nan_idx].empty:
         if color:
             if "color" not in missing_kwds:
                 missing_kwds["color"] = color
 
         merged_kwds = style_kwds.copy()
         merged_kwds.update(missing_kwds)
 
@@ -821,14 +906,38 @@
             n_cmap.set_array([])
             ax.get_figure().colorbar(n_cmap, **legend_kwds)
 
     plt.draw()
     return ax
 
 
+if geopandas._compat.PANDAS_GE_025:
+    from pandas.plotting import PlotAccessor
+
+    class GeoplotAccessor(PlotAccessor):
+
+        __doc__ = plot_dataframe.__doc__
+        _pandas_kinds = PlotAccessor._all_kinds
+
+        def __call__(self, *args, **kwargs):
+            data = self._parent.copy()
+            kind = kwargs.pop("kind", "geo")
+            if kind == "geo":
+                return plot_dataframe(data, *args, **kwargs)
+            if kind in self._pandas_kinds:
+                # Access pandas plots
+                return PlotAccessor(data)(kind=kind, **kwargs)
+            else:
+                # raise error
+                raise ValueError(f"{kind} is not a valid plot kind")
+
+        def geo(self, *args, **kwargs):
+            return self(kind="geo", *args, **kwargs)
+
+
 def _mapclassify_choro(values, scheme, **classification_kwds):
     """
     Wrapper for choropleth schemes from mapclassify for use with plot_dataframe
 
     Parameters
     ----------
     values
@@ -840,15 +949,15 @@
         JenksCaspallForced, JenksCaspallSampled, MaxP,
         MaximumBreaks, NaturalBreaks, Quantiles, Percentiles, StdMean,
         UserDefined
 
     **classification_kwds : dict
         Keyword arguments for classification scheme
         For details see mapclassify documentation:
-        https://mapclassify.readthedocs.io/en/latest/api.html
+        https://pysal.org/mapclassify/api.html
 
     Returns
     -------
     binning
         Binning objects that holds the Series with values replaced with
         class identifier and the bins.
     """
```

### Comparing `geopandas-0.8.2/geopandas/sindex.py` & `geopandas-0.9.0/geopandas/tools/tests/test_sjoin.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,481 +1,490 @@
-from collections import namedtuple
-from warnings import warn
+from distutils.version import LooseVersion
 
-from shapely.geometry.base import BaseGeometry
-import pandas as pd
 import numpy as np
+import pandas as pd
 
-from . import _compat as compat
-
-
-VALID_QUERY_PREDICATES = {
-    None,
-    "intersects",
-    "within",
-    "contains",
-    "overlaps",
-    "crosses",
-    "touches",
-}
-
-
-def has_sindex():
-    """Dynamically checks for ability to generate spatial index.
-    """
-    try:
-        get_sindex_class()
-        return True
-    except ImportError:
-        return False
-
-
-def get_sindex_class():
-    """Dynamically chooses a spatial indexing backend.
-
-    Required to comply with _compat.USE_PYGEOS.
-    The selection order goes PyGEOS > RTree > Error.
-    """
-    if compat.USE_PYGEOS:
-        return PyGEOSSTRTreeIndex
-    if compat.HAS_RTREE:
-        return RTreeIndex
-    raise ImportError(
-        "Spatial indexes require either `rtree` or `pygeos`. "
-        "See installation instructions at https://geopandas.org/install.html"
-    )
+from shapely.geometry import Point, Polygon, GeometryCollection
 
+import geopandas
+from geopandas import GeoDataFrame, GeoSeries, read_file, sjoin
 
-if compat.HAS_RTREE:
+from pandas.testing import assert_frame_equal
+import pytest
 
-    import rtree.index  # noqa
-    from rtree.core import RTreeError  # noqa
-    from shapely.prepared import prep  # noqa
-
-    class SpatialIndex(rtree.index.Index):
-        """Original rtree wrapper, kept for backwards compatibility.
-        """
-
-        def __init__(self, *args):
-            super().__init__(self, *args)
-
-        @property
-        def size(self):
-            return len(self.leaves()[0][1])
-
-        @property
-        def is_empty(self):
-            if len(self.leaves()) > 1:
-                return False
-            return self.size < 1
-
-    class RTreeIndex(rtree.index.Index):
-        """A simple wrapper around rtree's RTree Index
-
-        Parameters
-        ----------
-        geometry : GeoSeries
-            GeoSeries from which to build the spatial index.
-        """
-
-        # set of valid predicates for this spatial index
-        # by default, the global set
-        valid_query_predicates = VALID_QUERY_PREDICATES
-
-        def __init__(self, geometry):
-            stream = (
-                (i, item.bounds, idx)
-                for i, (idx, item) in enumerate(geometry.iteritems())
-                if pd.notnull(item) and not item.is_empty
-            )
-            try:
-                super().__init__(stream)
-            except RTreeError:
-                # What we really want here is an empty generator error, or
-                # for the bulk loader to log that the generator was empty
-                # and move on.
-                # See https://github.com/Toblerity/rtree/issues/20.
-                super().__init__()
-
-            # store reference to geometries for predicate queries
-            self.geometries = geometry.geometry.values
-            # create a prepared geometry cache
-            self._prepared_geometries = np.array(
-                [None] * self.geometries.size, dtype=object
-            )
 
-        def query(self, geometry, predicate=None, sort=False):
-            """Compatibility layer for pygeos.query.
+pytestmark = pytest.mark.skip_no_sindex
 
-            This is not a vectorized function, if speed is important,
-            please use PyGEOS.
 
-            Parameters
-            ----------
-            geometry : shapely geometry
-                A single shapely geometry to query against the spatial index.
-            predicate : {None, 'intersects', 'within', 'contains', \
-'overlaps', 'crosses', 'touches'}, optional
-                If predicate is provided, the input geometry is
-                tested using the predicate function against each item
-                in the tree whose extent intersects the envelope of the
-                input geometry: predicate(input_geometry, tree_geometry).
-                If possible, prepared geometries are used to help
-                speed up the predicate operation.
-            sort : bool, default False
-                If True, the results will be sorted in ascending order.
-                If False, results are often sorted but there is no guarantee.
-
-            Returns
-            -------
-            matches : ndarray of shape (n_results, )
-                Integer indices for matching geometries from the spatial index.
-            """
-
-            # handle invalid predicates
-            if predicate not in self.valid_query_predicates:
-                raise ValueError(
-                    "Got `predicate` = `{}`, `predicate` must be one of {}".format(
-                        predicate, self.valid_query_predicates
-                    )
-                )
-
-            # handle empty / invalid geometries
-            if geometry is None:
-                # return an empty integer array, similar to pygeys.STRtree.query.
-                return np.array([], dtype=np.intp)
-
-            if not isinstance(geometry, BaseGeometry):
-                raise TypeError(
-                    "Got `geometry` of type `{}`, `geometry` must be ".format(
-                        type(geometry)
-                    )
-                    + "a shapely geometry."
-                )
-
-            if geometry.is_empty:
-                return np.array([], dtype=np.intp)
+@pytest.fixture()
+def dfs(request):
+    polys1 = GeoSeries(
+        [
+            Polygon([(0, 0), (5, 0), (5, 5), (0, 5)]),
+            Polygon([(5, 5), (6, 5), (6, 6), (5, 6)]),
+            Polygon([(6, 0), (9, 0), (9, 3), (6, 3)]),
+        ]
+    )
 
-            # query tree
-            bounds = geometry.bounds  # rtree operates on bounds
-            tree_idx = list(self.intersection(bounds, objects=False))
-
-            if not tree_idx:
-                return np.array([], dtype=np.intp)
-
-            # Check predicate
-            # This is checked as input_geometry.predicate(tree_geometry)
-            # When possible, we use prepared geometries.
-            # Prepared geometries only support "intersects" and "contains"
-            # For the special case of "within", we are able to flip the
-            # comparison and check if tree_geometry.contains(input_geometry)
-            # to still take advantage of prepared geometries.
-            if predicate == "within":
-                # To use prepared geometries for within,
-                # we compare tree_geom.contains(input_geom)
-                # Since we are preparing the tree geometries,
-                # we cache them for multiple comparisons.
-                res = []
-                for index_in_tree in tree_idx:
-                    if self._prepared_geometries[index_in_tree] is None:
-                        # if not already prepared, prepare and cache
-                        self._prepared_geometries[index_in_tree] = prep(
-                            self.geometries[index_in_tree]
-                        )
-                    if self._prepared_geometries[index_in_tree].contains(geometry):
-                        res.append(index_in_tree)
-                tree_idx = res
-            elif predicate is not None:
-                # For the remaining predicates,
-                # we compare input_geom.predicate(tree_geom)
-                if predicate in ("contains", "intersects"):
-                    # prepare this input geometry
-                    geometry = prep(geometry)
-                tree_idx = [
-                    index_in_tree
-                    for index_in_tree in tree_idx
-                    if getattr(geometry, predicate)(self.geometries[index_in_tree])
-                ]
-
-            # sort if requested
-            if sort:
-                # sorted
-                return np.sort(np.array(tree_idx, dtype=np.intp))
-
-            # unsorted
-            return np.array(tree_idx, dtype=np.intp)
-
-        def query_bulk(self, geometry, predicate=None, sort=False):
-            """Compatibility layer for pygeos.query_bulk.
-
-            Iterates over `geometry` and queries index.
-            This operation is not vectorized and may be slow.
-            Use PyGEOS with `query_bulk` for speed.
-
-            Parameters
-            ----------
-            geometry : {GeoSeries, GeometryArray, numpy.array of PyGEOS geometries}
-                Accepts GeoPandas geometry iterables (GeoSeries, GeometryArray)
-                or a numpy array of PyGEOS geometries.
-            predicate : {None, 'intersects', 'within', 'contains', 'overlaps', \
-'crosses', 'touches'}, optional
-                If predicate is provided, the input geometries are tested using
-                the predicate function against each item in the tree whose extent
-                intersects the envelope of the each input geometry:
-                predicate(input_geometry, tree_geometry).  If possible, prepared
-                geometries are used to help speed up the predicate operation.
-            sort : bool, default False
-                If True, results sorted lexicographically using
-                geometry's indexes as the primary key and the sindex's indexes as the
-                secondary key. If False, no additional sorting is applied.
-
-            Returns
-            -------
-            ndarray with shape (2, n)
-                The first subarray contains input geometry integer indexes.
-                The second subarray contains tree geometry integer indexes.
-            """
-            # Iterates over geometry, applying func.
-            tree_index = []
-            input_geometry_index = []
-
-            for i, geo in enumerate(geometry):
-                res = self.query(geo, predicate=predicate, sort=sort)
-                tree_index.extend(res)
-                input_geometry_index.extend([i] * len(res))
-            return np.vstack([input_geometry_index, tree_index])
-
-        def intersection(self, coordinates, objects=False):
-            """Find tree geometries that intersect the input coordinates.
-
-            Parameters
-            ----------
-            coordinates : sequence or array
-                Sequence of the form (min_x, min_y, max_x, max_y)
-                to query a rectangle or (x, y) to query a point.
-            objects : boolean, default False
-                If True, return the label based indexes. If False, integer indexes
-                are returned.
-            """
-            if objects:
-                warn(
-                    "`objects` is deprecated and will be removed in a future version. "
-                    "Instead, use `iloc` to index your GeoSeries/GeoDataFrame using "
-                    "integer indexes returned by `intersection`.",
-                    FutureWarning,
-                )
-            return super().intersection(coordinates, objects)
+    polys2 = GeoSeries(
+        [
+            Polygon([(1, 1), (4, 1), (4, 4), (1, 4)]),
+            Polygon([(4, 4), (7, 4), (7, 7), (4, 7)]),
+            Polygon([(7, 7), (10, 7), (10, 10), (7, 10)]),
+        ]
+    )
 
-        @property
-        def size(self):
-            return len(self.leaves()[0][1])
-
-        @property
-        def is_empty(self):
-            return self.size == 0
-
-        def __len__(self):
-            return self.size
-
-
-if compat.HAS_PYGEOS:
-
-    from . import geoseries  # noqa
-    from .array import GeometryArray, _shapely_to_geom  # noqa
-    import pygeos  # noqa
-
-    class PyGEOSSTRTreeIndex(pygeos.STRtree):
-        """A simple wrapper around pygeos's STRTree.
-
-
-        Parameters
-        ----------
-        geometry : GeoSeries
-            GeoSeries from which to build the spatial index.
-        """
-
-        # helper for loc/label based indexing in `intersection` method
-        with_objects = namedtuple("with_objects", "object id")
-
-        # set of valid predicates for this spatial index
-        # by default, the global set
-        valid_query_predicates = VALID_QUERY_PREDICATES
-
-        def __init__(self, geometry):
-            # for compatibility with old RTree implementation, store ids/indexes
-            original_indexes = geometry.index
-            # set empty geometries to None to avoid segfault on GEOS <= 3.6
-            # see:
-            # https://github.com/pygeos/pygeos/issues/146
-            # https://github.com/pygeos/pygeos/issues/147
-            non_empty = geometry.values.data.copy()
-            non_empty[pygeos.is_empty(non_empty)] = None
-            # set empty geometries to None to mantain indexing
-            self.objects = self.ids = original_indexes
-            super().__init__(non_empty)
-            # store geometries, including empty geometries for user access
-            self.geometries = geometry.values.data.copy()
-
-        def query(self, geometry, predicate=None, sort=False):
-            """Wrapper for pygeos.query.
-
-            This also ensures a deterministic (sorted) order for the results.
-
-            Parameters
-            ----------
-            geometry : single PyGEOS geometry
-            predicate : {None, 'intersects', 'within', 'contains', \
-'overlaps', 'crosses', 'touches'}, optional
-                If predicate is provided, the input geometry is tested
-                using the predicate function against each item in the
-                tree whose extent intersects the envelope of the input
-                geometry: predicate(input_geometry, tree_geometry).
-            sort : bool, default False
-                If True, the results will be sorted in ascending order.
-                If False, results are often sorted but there is no guarantee.
-
-            Returns
-            -------
-            matches : ndarray of shape (n_results, )
-                Integer indices for matching geometries from the spatial index.
-
-            See also
-            --------
-            See PyGEOS.strtree documentation for more information.
-            """
-
-            if predicate not in self.valid_query_predicates:
-                raise ValueError(
-                    "Got `predicate` = `{}`; ".format(predicate)
-                    + "`predicate` must be one of {}".format(
-                        self.valid_query_predicates
-                    )
-                )
+    df1 = GeoDataFrame({"geometry": polys1, "df1": [0, 1, 2]})
+    df2 = GeoDataFrame({"geometry": polys2, "df2": [3, 4, 5]})
 
-            if isinstance(geometry, BaseGeometry):
-                geometry = _shapely_to_geom(geometry)
+    if request.param == "string-index":
+        df1.index = ["a", "b", "c"]
+        df2.index = ["d", "e", "f"]
+
+    if request.param == "named-index":
+        df1.index.name = "df1_ix"
+        df2.index.name = "df2_ix"
+
+    if request.param == "multi-index":
+        i1 = ["a", "b", "c"]
+        i2 = ["d", "e", "f"]
+        df1 = df1.set_index([i1, i2])
+        df2 = df2.set_index([i2, i1])
+
+    if request.param == "named-multi-index":
+        i1 = ["a", "b", "c"]
+        i2 = ["d", "e", "f"]
+        df1 = df1.set_index([i1, i2])
+        df2 = df2.set_index([i2, i1])
+        df1.index.names = ["df1_ix1", "df1_ix2"]
+        df2.index.names = ["df2_ix1", "df2_ix2"]
+
+    # construction expected frames
+    expected = {}
+
+    part1 = df1.copy().reset_index().rename(columns={"index": "index_left"})
+    part2 = (
+        df2.copy()
+        .iloc[[0, 1, 1, 2]]
+        .reset_index()
+        .rename(columns={"index": "index_right"})
+    )
+    part1["_merge"] = [0, 1, 2]
+    part2["_merge"] = [0, 0, 1, 3]
+    exp = pd.merge(part1, part2, on="_merge", how="outer")
+    expected["intersects"] = exp.drop("_merge", axis=1).copy()
+
+    part1 = df1.copy().reset_index().rename(columns={"index": "index_left"})
+    part2 = df2.copy().reset_index().rename(columns={"index": "index_right"})
+    part1["_merge"] = [0, 1, 2]
+    part2["_merge"] = [0, 3, 3]
+    exp = pd.merge(part1, part2, on="_merge", how="outer")
+    expected["contains"] = exp.drop("_merge", axis=1).copy()
+
+    part1["_merge"] = [0, 1, 2]
+    part2["_merge"] = [3, 1, 3]
+    exp = pd.merge(part1, part2, on="_merge", how="outer")
+    expected["within"] = exp.drop("_merge", axis=1).copy()
+
+    return [request.param, df1, df2, expected]
+
+
+class TestSpatialJoin:
+    @pytest.mark.parametrize("dfs", ["default-index", "string-index"], indirect=True)
+    def test_crs_mismatch(self, dfs):
+        index, df1, df2, expected = dfs
+        df1.crs = "epsg:4326"
+        with pytest.warns(UserWarning, match="CRS mismatch between the CRS"):
+            sjoin(df1, df2)
+
+    @pytest.mark.parametrize(
+        "dfs",
+        [
+            "default-index",
+            "string-index",
+            "named-index",
+            "multi-index",
+            "named-multi-index",
+        ],
+        indirect=True,
+    )
+    @pytest.mark.parametrize("op", ["intersects", "contains", "within"])
+    def test_inner(self, op, dfs):
+        index, df1, df2, expected = dfs
+
+        res = sjoin(df1, df2, how="inner", op=op)
+
+        exp = expected[op].dropna().copy()
+        exp = exp.drop("geometry_y", axis=1).rename(columns={"geometry_x": "geometry"})
+        exp[["df1", "df2"]] = exp[["df1", "df2"]].astype("int64")
+        if index == "default-index":
+            exp[["index_left", "index_right"]] = exp[
+                ["index_left", "index_right"]
+            ].astype("int64")
+        if index == "named-index":
+            exp[["df1_ix", "df2_ix"]] = exp[["df1_ix", "df2_ix"]].astype("int64")
+            exp = exp.set_index("df1_ix").rename(columns={"df2_ix": "index_right"})
+        if index in ["default-index", "string-index"]:
+            exp = exp.set_index("index_left")
+            exp.index.name = None
+        if index == "multi-index":
+            exp = exp.set_index(["level_0_x", "level_1_x"]).rename(
+                columns={"level_0_y": "index_right0", "level_1_y": "index_right1"}
+            )
+            exp.index.names = df1.index.names
+        if index == "named-multi-index":
+            exp = exp.set_index(["df1_ix1", "df1_ix2"]).rename(
+                columns={"df2_ix1": "index_right0", "df2_ix2": "index_right1"}
+            )
+            exp.index.names = df1.index.names
 
-            matches = super().query(geometry=geometry, predicate=predicate)
+        assert_frame_equal(res, exp)
 
-            if sort:
-                return np.sort(matches)
+    @pytest.mark.parametrize(
+        "dfs",
+        [
+            "default-index",
+            "string-index",
+            "named-index",
+            "multi-index",
+            "named-multi-index",
+        ],
+        indirect=True,
+    )
+    @pytest.mark.parametrize("op", ["intersects", "contains", "within"])
+    def test_left(self, op, dfs):
+        index, df1, df2, expected = dfs
+
+        res = sjoin(df1, df2, how="left", op=op)
+
+        if index in ["default-index", "string-index"]:
+            exp = expected[op].dropna(subset=["index_left"]).copy()
+        elif index == "named-index":
+            exp = expected[op].dropna(subset=["df1_ix"]).copy()
+        elif index == "multi-index":
+            exp = expected[op].dropna(subset=["level_0_x"]).copy()
+        elif index == "named-multi-index":
+            exp = expected[op].dropna(subset=["df1_ix1"]).copy()
+        exp = exp.drop("geometry_y", axis=1).rename(columns={"geometry_x": "geometry"})
+        exp["df1"] = exp["df1"].astype("int64")
+        if index == "default-index":
+            exp["index_left"] = exp["index_left"].astype("int64")
+            # TODO: in result the dtype is object
+            res["index_right"] = res["index_right"].astype(float)
+        elif index == "named-index":
+            exp[["df1_ix"]] = exp[["df1_ix"]].astype("int64")
+            exp = exp.set_index("df1_ix").rename(columns={"df2_ix": "index_right"})
+        if index in ["default-index", "string-index"]:
+            exp = exp.set_index("index_left")
+            exp.index.name = None
+        if index == "multi-index":
+            exp = exp.set_index(["level_0_x", "level_1_x"]).rename(
+                columns={"level_0_y": "index_right0", "level_1_y": "index_right1"}
+            )
+            exp.index.names = df1.index.names
+        if index == "named-multi-index":
+            exp = exp.set_index(["df1_ix1", "df1_ix2"]).rename(
+                columns={"df2_ix1": "index_right0", "df2_ix2": "index_right1"}
+            )
+            exp.index.names = df1.index.names
 
-            return matches
-
-        def query_bulk(self, geometry, predicate=None, sort=False):
-            """Wrapper to expose underlaying pygeos objects to pygeos.query_bulk.
-
-            This also allows a deterministic (sorted) order for the results.
-
-
-            Parameters
-            ----------
-            geometry : {GeoSeries, GeometryArray, numpy.array of PyGEOS geometries}
-                Accepts GeoPandas geometry iterables (GeoSeries, GeometryArray)
-                or a numpy array of PyGEOS geometries.
-            predicate : {None, 'intersects', 'within', 'contains', \
-'overlaps', 'crosses', 'touches'}, optional
-                If predicate is provided, the input geometry is tested
-                using the predicate function against each item in the
-                index whose extent intersects the envelope of the input geometry:
-                predicate(input_geometry, tree_geometry).
-            sort : bool, default False
-                If True, results sorted lexicographically using
-                geometry's indexes as the primary key and the sindex's indexes as the
-                secondary key. If False, no additional sorting is applied.
-
-            Returns
-            -------
-            ndarray with shape (2, n)
-                The first subarray contains input geometry integer indexes.
-                The second subarray contains tree geometry integer indexes.
-
-            See also
-            --------
-            See PyGEOS.strtree documentation for more information.
-            """
-
-            if predicate not in self.valid_query_predicates:
-                raise ValueError(
-                    "Got `predicate` = `{}`, `predicate` must be one of {}".format(
-                        predicate, self.valid_query_predicates
-                    )
-                )
-            if isinstance(geometry, geoseries.GeoSeries):
-                geometry = geometry.values.data
-            elif isinstance(geometry, GeometryArray):
-                geometry = geometry.data
-            elif not isinstance(geometry, np.ndarray):
-                geometry = np.asarray(geometry)
-
-            res = super().query_bulk(geometry, predicate)
-
-            if sort:
-                # sort by first array (geometry) and then second (tree)
-                geo_res, tree_res = res
-                indexing = np.lexsort((tree_res, geo_res))
-                return np.vstack((geo_res[indexing], tree_res[indexing]))
-
-            return res
-
-        def intersection(self, coordinates, objects=False):
-            """Wrapper for pygeos.query that uses the RTree API.
-
-            Parameters
-            ----------
-            coordinates : sequence or array
-                Sequence of the form (min_x, min_y, max_x, max_y)
-                to query a rectangle or (x, y) to query a point.
-            objects : boolean, default False
-                If True, return the label based indexes. If False, integer indexes
-                are returned.
-            """
-            if objects:
-                warn(
-                    "`objects` is deprecated and will be removed in a future version. "
-                    "Instead, use `iloc` to index your GeoSeries/GeoDataFrame using "
-                    "integer indexes returned by `intersection`.",
-                    FutureWarning,
-                )
+        assert_frame_equal(res, exp)
 
-            # convert bounds to geometry
-            # the old API uses tuples of bound, but pygeos uses geometries
-            try:
-                iter(coordinates)
-            except TypeError:
-                # likely not an iterable
-                # this is a check that rtree does, we mimic it
-                # to ensure a useful failure message
-                raise TypeError(
-                    "Invalid coordinates, must be iterable in format "
-                    "(minx, miny, maxx, maxy) (for bounds) or (x, y) (for points). "
-                    "Got `coordinates` = {}.".format(coordinates)
-                )
+    def test_empty_join(self):
+        # Check joins resulting in empty gdfs.
+        polygons = geopandas.GeoDataFrame(
+            {
+                "col2": [1, 2],
+                "geometry": [
+                    Polygon([(0, 0), (1, 0), (1, 1), (0, 1)]),
+                    Polygon([(1, 0), (2, 0), (2, 1), (1, 1)]),
+                ],
+            }
+        )
+        not_in = geopandas.GeoDataFrame({"col1": [1], "geometry": [Point(-0.5, 0.5)]})
+        empty = sjoin(not_in, polygons, how="left", op="intersects")
+        assert empty.index_right.isnull().all()
+        empty = sjoin(not_in, polygons, how="right", op="intersects")
+        assert empty.index_left.isnull().all()
+        empty = sjoin(not_in, polygons, how="inner", op="intersects")
+        assert empty.empty
+
+    @pytest.mark.parametrize("op", ["intersects", "contains", "within"])
+    @pytest.mark.parametrize(
+        "empty",
+        [
+            GeoDataFrame(geometry=[GeometryCollection(), GeometryCollection()]),
+            GeoDataFrame(geometry=GeoSeries()),
+        ],
+    )
+    def test_join_with_empty(self, op, empty):
+        # Check joins with empty geometry columns/dataframes.
+        polygons = geopandas.GeoDataFrame(
+            {
+                "col2": [1, 2],
+                "geometry": [
+                    Polygon([(0, 0), (1, 0), (1, 1), (0, 1)]),
+                    Polygon([(1, 0), (2, 0), (2, 1), (1, 1)]),
+                ],
+            }
+        )
+        result = sjoin(empty, polygons, how="left", op=op)
+        assert result.index_right.isnull().all()
+        result = sjoin(empty, polygons, how="right", op=op)
+        assert result.index_left.isnull().all()
+        result = sjoin(empty, polygons, how="inner", op=op)
+        assert result.empty
+
+    @pytest.mark.parametrize("dfs", ["default-index", "string-index"], indirect=True)
+    def test_sjoin_invalid_args(self, dfs):
+        index, df1, df2, expected = dfs
+
+        with pytest.raises(ValueError, match="'left_df' should be GeoDataFrame"):
+            sjoin(df1.geometry, df2)
+
+        with pytest.raises(ValueError, match="'right_df' should be GeoDataFrame"):
+            sjoin(df1, df2.geometry)
+
+    @pytest.mark.parametrize(
+        "dfs",
+        [
+            "default-index",
+            "string-index",
+            "named-index",
+            "multi-index",
+            "named-multi-index",
+        ],
+        indirect=True,
+    )
+    @pytest.mark.parametrize("op", ["intersects", "contains", "within"])
+    def test_right(self, op, dfs):
+        index, df1, df2, expected = dfs
+
+        res = sjoin(df1, df2, how="right", op=op)
+
+        if index in ["default-index", "string-index"]:
+            exp = expected[op].dropna(subset=["index_right"]).copy()
+        elif index == "named-index":
+            exp = expected[op].dropna(subset=["df2_ix"]).copy()
+        elif index == "multi-index":
+            exp = expected[op].dropna(subset=["level_0_y"]).copy()
+        elif index == "named-multi-index":
+            exp = expected[op].dropna(subset=["df2_ix1"]).copy()
+        exp = exp.drop("geometry_x", axis=1).rename(columns={"geometry_y": "geometry"})
+        exp["df2"] = exp["df2"].astype("int64")
+        if index == "default-index":
+            exp["index_right"] = exp["index_right"].astype("int64")
+            res["index_left"] = res["index_left"].astype(float)
+        elif index == "named-index":
+            exp[["df2_ix"]] = exp[["df2_ix"]].astype("int64")
+            exp = exp.set_index("df2_ix").rename(columns={"df1_ix": "index_left"})
+        if index in ["default-index", "string-index"]:
+            exp = exp.set_index("index_right")
+            exp = exp.reindex(columns=res.columns)
+            exp.index.name = None
+        if index == "multi-index":
+            exp = exp.set_index(["level_0_y", "level_1_y"]).rename(
+                columns={"level_0_x": "index_left0", "level_1_x": "index_left1"}
+            )
+            exp.index.names = df2.index.names
+        if index == "named-multi-index":
+            exp = exp.set_index(["df2_ix1", "df2_ix2"]).rename(
+                columns={"df1_ix1": "index_left0", "df1_ix2": "index_left1"}
+            )
+            exp.index.names = df2.index.names
 
-            # need to convert tuple of bounds to a geometry object
-            if len(coordinates) == 4:
-                indexes = super().query(pygeos.box(*coordinates))
-            elif len(coordinates) == 2:
-                indexes = super().query(pygeos.points(*coordinates))
-            else:
-                raise TypeError(
-                    "Invalid coordinates, must be iterable in format "
-                    "(minx, miny, maxx, maxy) (for bounds) or (x, y) (for points). "
-                    "Got `coordinates` = {}.".format(coordinates)
+        # GH 1364 fix of behaviour was done in pandas 1.1.0
+        if op == "within" and str(pd.__version__) >= LooseVersion("1.1.0"):
+            exp = exp.sort_index()
+
+        assert_frame_equal(res, exp, check_index_type=False)
+
+
+class TestSpatialJoinNYBB:
+    def setup_method(self):
+        nybb_filename = geopandas.datasets.get_path("nybb")
+        self.polydf = read_file(nybb_filename)
+        self.crs = self.polydf.crs
+        N = 20
+        b = [int(x) for x in self.polydf.total_bounds]
+        self.pointdf = GeoDataFrame(
+            [
+                {"geometry": Point(x, y), "pointattr1": x + y, "pointattr2": x - y}
+                for x, y in zip(
+                    range(b[0], b[2], int((b[2] - b[0]) / N)),
+                    range(b[1], b[3], int((b[3] - b[1]) / N)),
                 )
-
-            if objects:
-                objs = self.objects[indexes].values
-                ids = self.ids[indexes]
-                return [
-                    self.with_objects(id=id, object=obj) for id, obj in zip(ids, objs)
-                ]
-            else:
-                return indexes
-
-        @property
-        def size(self):
-            return len(self)
-
-        @property
-        def is_empty(self):
-            return len(self) == 0
+            ],
+            crs=self.crs,
+        )
+
+    def test_geometry_name(self):
+        # test sjoin is working with other geometry name
+        polydf_original_geom_name = self.polydf.geometry.name
+        self.polydf = self.polydf.rename(columns={"geometry": "new_geom"}).set_geometry(
+            "new_geom"
+        )
+        assert polydf_original_geom_name != self.polydf.geometry.name
+        res = sjoin(self.polydf, self.pointdf, how="left")
+        assert self.polydf.geometry.name == res.geometry.name
+
+    def test_sjoin_left(self):
+        df = sjoin(self.pointdf, self.polydf, how="left")
+        assert df.shape == (21, 8)
+        for i, row in df.iterrows():
+            assert row.geometry.type == "Point"
+        assert "pointattr1" in df.columns
+        assert "BoroCode" in df.columns
+
+    def test_sjoin_right(self):
+        # the inverse of left
+        df = sjoin(self.pointdf, self.polydf, how="right")
+        df2 = sjoin(self.polydf, self.pointdf, how="left")
+        assert df.shape == (12, 8)
+        assert df.shape == df2.shape
+        for i, row in df.iterrows():
+            assert row.geometry.type == "MultiPolygon"
+        for i, row in df2.iterrows():
+            assert row.geometry.type == "MultiPolygon"
+
+    def test_sjoin_inner(self):
+        df = sjoin(self.pointdf, self.polydf, how="inner")
+        assert df.shape == (11, 8)
+
+    def test_sjoin_op(self):
+        # points within polygons
+        df = sjoin(self.pointdf, self.polydf, how="left", op="within")
+        assert df.shape == (21, 8)
+        assert df.loc[1]["BoroName"] == "Staten Island"
+
+        # points contain polygons? never happens so we should have nulls
+        df = sjoin(self.pointdf, self.polydf, how="left", op="contains")
+        assert df.shape == (21, 8)
+        assert np.isnan(df.loc[1]["Shape_Area"])
+
+    def test_sjoin_bad_op(self):
+        # AttributeError: 'Point' object has no attribute 'spandex'
+        with pytest.raises(ValueError):
+            sjoin(self.pointdf, self.polydf, how="left", op="spandex")
+
+    def test_sjoin_duplicate_column_name(self):
+        pointdf2 = self.pointdf.rename(columns={"pointattr1": "Shape_Area"})
+        df = sjoin(pointdf2, self.polydf, how="left")
+        assert "Shape_Area_left" in df.columns
+        assert "Shape_Area_right" in df.columns
+
+    @pytest.mark.parametrize("how", ["left", "right", "inner"])
+    def test_sjoin_named_index(self, how):
+        # original index names should be unchanged
+        pointdf2 = self.pointdf.copy()
+        pointdf2.index.name = "pointid"
+        polydf = self.polydf.copy()
+        polydf.index.name = "polyid"
+
+        res = sjoin(pointdf2, polydf, how=how)
+        assert pointdf2.index.name == "pointid"
+        assert polydf.index.name == "polyid"
+
+        # original index name should pass through to result
+        if how == "right":
+            assert res.index.name == "polyid"
+        else:  # how == "left", how == "inner"
+            assert res.index.name == "pointid"
+
+    def test_sjoin_values(self):
+        # GH190
+        self.polydf.index = [1, 3, 4, 5, 6]
+        df = sjoin(self.pointdf, self.polydf, how="left")
+        assert df.shape == (21, 8)
+        df = sjoin(self.polydf, self.pointdf, how="left")
+        assert df.shape == (12, 8)
+
+    @pytest.mark.xfail
+    def test_no_overlapping_geometry(self):
+        # Note: these tests are for correctly returning GeoDataFrame
+        # when result of the join is empty
+
+        df_inner = sjoin(self.pointdf.iloc[17:], self.polydf, how="inner")
+        df_left = sjoin(self.pointdf.iloc[17:], self.polydf, how="left")
+        df_right = sjoin(self.pointdf.iloc[17:], self.polydf, how="right")
+
+        expected_inner_df = pd.concat(
+            [
+                self.pointdf.iloc[:0],
+                pd.Series(name="index_right", dtype="int64"),
+                self.polydf.drop("geometry", axis=1).iloc[:0],
+            ],
+            axis=1,
+        )
+
+        expected_inner = GeoDataFrame(expected_inner_df)
+
+        expected_right_df = pd.concat(
+            [
+                self.pointdf.drop("geometry", axis=1).iloc[:0],
+                pd.concat(
+                    [
+                        pd.Series(name="index_left", dtype="int64"),
+                        pd.Series(name="index_right", dtype="int64"),
+                    ],
+                    axis=1,
+                ),
+                self.polydf,
+            ],
+            axis=1,
+        )
+
+        expected_right = GeoDataFrame(expected_right_df).set_index("index_right")
+
+        expected_left_df = pd.concat(
+            [
+                self.pointdf.iloc[17:],
+                pd.Series(name="index_right", dtype="int64"),
+                self.polydf.iloc[:0].drop("geometry", axis=1),
+            ],
+            axis=1,
+        )
+
+        expected_left = GeoDataFrame(expected_left_df)
+
+        assert expected_inner.equals(df_inner)
+        assert expected_right.equals(df_right)
+        assert expected_left.equals(df_left)
+
+    @pytest.mark.skip("Not implemented")
+    def test_sjoin_outer(self):
+        df = sjoin(self.pointdf, self.polydf, how="outer")
+        assert df.shape == (21, 8)
+
+    def test_sjoin_empty_geometries(self):
+        # https://github.com/geopandas/geopandas/issues/944
+        empty = GeoDataFrame(geometry=[GeometryCollection()] * 3)
+        df = sjoin(self.pointdf.append(empty), self.polydf, how="left")
+        assert df.shape == (24, 8)
+        df2 = sjoin(self.pointdf, self.polydf.append(empty), how="left")
+        assert df2.shape == (21, 8)
+
+    @pytest.mark.parametrize("op", ["intersects", "within", "contains"])
+    def test_sjoin_no_valid_geoms(self, op):
+        """Tests a completely empty GeoDataFrame."""
+        empty = GeoDataFrame(geometry=[], crs=self.pointdf.crs)
+        assert sjoin(self.pointdf, empty, how="inner", op=op).empty
+        assert sjoin(self.pointdf, empty, how="right", op=op).empty
+        assert sjoin(empty, self.pointdf, how="inner", op=op).empty
+        assert sjoin(empty, self.pointdf, how="left", op=op).empty
+
+
+class TestSpatialJoinNaturalEarth:
+    def setup_method(self):
+        world_path = geopandas.datasets.get_path("naturalearth_lowres")
+        cities_path = geopandas.datasets.get_path("naturalearth_cities")
+        self.world = read_file(world_path)
+        self.cities = read_file(cities_path)
+
+    def test_sjoin_inner(self):
+        # GH637
+        countries = self.world[["geometry", "name"]]
+        countries = countries.rename(columns={"name": "country"})
+        cities_with_country = sjoin(
+            self.cities, countries, how="inner", op="intersects"
+        )
+        assert cities_with_country.shape == (172, 4)
```

### Comparing `geopandas-0.8.2/geopandas/testing.py` & `geopandas-0.9.0/geopandas/testing.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 import warnings
 
 import pandas as pd
 
 from geopandas import GeoDataFrame, GeoSeries
 from geopandas.array import GeometryDtype
+from geopandas import _vectorized
 
 
 def _isna(this):
     """isna version that works for both scalars and (Geo)Series"""
     if hasattr(this, "isna"):
         return this.isna()
     elif hasattr(this, "isnull"):
@@ -63,14 +64,15 @@
     right,
     check_dtype=True,
     check_index_type=False,
     check_series_type=True,
     check_less_precise=False,
     check_geom_type=False,
     check_crs=True,
+    normalize=False,
 ):
     """
     Test util for checking that two GeoSeries are equal.
 
     Parameters
     ----------
     left, right : two GeoSeries
@@ -85,14 +87,18 @@
     check_less_precise : bool, default False
         If True, use geom_almost_equals. if False, use geom_equals.
     check_geom_type : bool, default False
         If True, check that all the geom types are equal.
     check_crs: bool, default True
         If `check_series_type` is True, then also check that the
         crs matches.
+    normalize: bool, default False
+        If True, normalize the geometries before comparing equality.
+        Typically useful with ``check_less_precise=True``, which uses
+        ``geom_almost_equals`` and requires exact coordinate order.
     """
     assert len(left) == len(right), "%d != %d" % (len(left), len(right))
 
     if check_dtype:
         msg = "dtype should be a GeometryDtype, got {0}"
         assert isinstance(left.dtype, GeometryDtype), msg.format(left.dtype)
         assert isinstance(right.dtype, GeometryDtype), msg.format(left.dtype)
@@ -116,39 +122,87 @@
 
     if check_geom_type:
         assert (left.type == right.type).all(), "type: %s != %s" % (
             left.type,
             right.type,
         )
 
+    if normalize:
+        left = GeoSeries(_vectorized.normalize(left.array.data))
+        right = GeoSeries(_vectorized.normalize(right.array.data))
+
     if not check_crs:
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", "CRS mismatch", UserWarning)
-            if check_less_precise:
-                assert geom_almost_equals(left, right)
-            else:
-                assert geom_equals(left, right)
+            _check_equality(left, right, check_less_precise)
+    else:
+        _check_equality(left, right, check_less_precise)
+
+
+def _truncated_string(geom):
+    """Truncated WKT repr of geom"""
+    s = str(geom)
+    if len(s) > 100:
+        return s[:100] + "..."
+    else:
+        return s
+
+
+def _check_equality(left, right, check_less_precise):
+    assert_error_message = (
+        "{0} out of {1} geometries are not {3}equal.\n"
+        "Indices where geometries are not {3}equal: {2} \n"
+        "The first not {3}equal geometry:\n"
+        "Left: {4}\n"
+        "Right: {5}\n"
+    )
+    if check_less_precise:
+        precise = "almost "
+        if not geom_almost_equals(left, right):
+            unequal_left_geoms = left[~left.geom_almost_equals(right)]
+            unequal_right_geoms = right[~left.geom_almost_equals(right)]
+            raise AssertionError(
+                assert_error_message.format(
+                    len(unequal_left_geoms),
+                    len(left),
+                    unequal_left_geoms.index.to_list(),
+                    precise,
+                    _truncated_string(unequal_left_geoms.iloc[0]),
+                    _truncated_string(unequal_right_geoms.iloc[0]),
+                )
+            )
     else:
-        if check_less_precise:
-            assert geom_almost_equals(left, right)
-        else:
-            assert geom_equals(left, right)
+        precise = ""
+        if not geom_equals(left, right):
+            unequal_left_geoms = left[~left.geom_almost_equals(right)]
+            unequal_right_geoms = right[~left.geom_almost_equals(right)]
+            raise AssertionError(
+                assert_error_message.format(
+                    len(unequal_left_geoms),
+                    len(left),
+                    unequal_left_geoms.index.to_list(),
+                    precise,
+                    _truncated_string(unequal_left_geoms.iloc[0]),
+                    _truncated_string(unequal_right_geoms.iloc[0]),
+                )
+            )
 
 
 def assert_geodataframe_equal(
     left,
     right,
     check_dtype=True,
     check_index_type="equiv",
     check_column_type="equiv",
     check_frame_type=True,
     check_like=False,
     check_less_precise=False,
     check_geom_type=False,
     check_crs=True,
+    normalize=False,
 ):
     """
     Check that two GeoDataFrames are equal/
 
     Parameters
     ----------
     left, right : two GeoDataFrames
@@ -164,14 +218,18 @@
     check_less_precise : bool, default False
         If True, use geom_almost_equals. if False, use geom_equals.
     check_geom_type : bool, default False
         If True, check that all the geom types are equal.
     check_crs: bool, default True
         If `check_frame_type` is True, then also check that the
         crs matches.
+    normalize: bool, default False
+        If True, normalize the geometries before comparing equality.
+        Typically useful with ``check_less_precise=True``, which uses
+        ``geom_almost_equals`` and requires exact coordinate order.
     """
     try:
         # added from pandas 0.20
         from pandas.testing import assert_frame_equal, assert_index_equal
     except ImportError:
         from pandas.util.testing import assert_frame_equal, assert_index_equal
 
@@ -191,20 +249,17 @@
             left = GeoDataFrame(left)
         if not isinstance(right, GeoDataFrame):
             right = GeoDataFrame(right)
 
     # shape comparison
     assert left.shape == right.shape, (
         "GeoDataFrame shape mismatch, left: {lshape!r}, right: {rshape!r}.\n"
-        "Left columns: {lcols!r}, right columns: {rcols!r}".format(
-            lshape=left.shape,
-            rshape=right.shape,
-            lcols=left.columns,
-            rcols=right.columns,
-        )
+        "Left columns: {lcols!r}, right columns: {rcols!r}"
+    ).format(
+        lshape=left.shape, rshape=right.shape, lcols=left.columns, rcols=right.columns
     )
 
     if check_like:
         left, right = left.reindex_like(right), right
 
     # column comparison
     assert_index_equal(
@@ -213,14 +268,15 @@
 
     # geometry comparison
     for col, dtype in left.dtypes.iteritems():
         if isinstance(dtype, GeometryDtype):
             assert_geoseries_equal(
                 left[col],
                 right[col],
+                normalize=normalize,
                 check_dtype=check_dtype,
                 check_less_precise=check_less_precise,
                 check_geom_type=check_geom_type,
                 check_crs=check_crs,
             )
 
     # drop geometries and check remaining columns
```

### Comparing `geopandas-0.8.2/geopandas/tests/test_api.py` & `geopandas-0.9.0/geopandas/tests/test_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 def test_no_additional_imports():
     # test that 'import geopandas' does not import any of the optional or
     # development dependencies
     blacklist = {
         "pytest",
         "py",
         "ipython",
-        # 'matplotlib',  # matplotlib gets imported by pandas, see below
-        "descartes",
+        # fiona actually gets imported if installed (but error suppressed until used)
+        # "fiona",
+        # "matplotlib",  # matplotlib gets imported by pandas, see below
         "mapclassify",
         # 'rtree',  # rtree actually gets imported if installed
         "sqlalchemy",
         "psycopg2",
         "geopy",
         "geoalchemy2",
     }
```

### Comparing `geopandas-0.8.2/geopandas/tests/test_array.py` & `geopandas-0.9.0/geopandas/tests/test_array.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import random
 
 import numpy as np
 import pandas as pd
 import six
 
+from pyproj import CRS
 import shapely
 import shapely.affinity
 import shapely.geometry
 from shapely.geometry.base import CAP_STYLE, JOIN_STYLE
 import shapely.wkb
 from shapely._buildcfg import geos_version
 
@@ -48,16 +49,16 @@
                 return False
         elif not r.equals(e):
             return False
     return True
 
 
 def test_points():
-    x = np.arange(10).astype(np.float)
-    y = np.arange(10).astype(np.float) ** 2
+    x = np.arange(10).astype(np.float64)
+    y = np.arange(10).astype(np.float64) ** 2
 
     points = points_from_xy(x, y)
     assert isinstance(points, GeometryArray)
 
     for i in range(10):
         assert isinstance(points[i], shapely.geometry.Point)
         assert points[i].x == x[i]
@@ -113,17 +114,19 @@
             self.y = y
 
         @property
         def __geo_interface__(self):
             return {"type": "Point", "coordinates": (self.x, self.y)}
 
     result = from_shapely([Point(1.0, 2.0), Point(3.0, 4.0)])
+
     expected = from_shapely(
         [shapely.geometry.Point(1.0, 2.0), shapely.geometry.Point(3.0, 4.0)]
     )
+
     assert all(v.equals(t) for v, t in zip(result, expected))
 
 
 def test_from_wkb():
     # list
     L_wkb = [p.wkb for p in points_no_missing]
     res = from_wkb(L_wkb)
@@ -322,15 +325,15 @@
                 getattr(a, attr if "geom" not in attr else attr[5:])(b, *args)
             )
 
     assert result.tolist() == expected
 
 
 @pytest.mark.parametrize(
-    "attr,args", [("equals_exact", (0.1,)), ("almost_equals", (3,))],
+    "attr,args", [("equals_exact", (0.1,)), ("almost_equals", (3,))]
 )
 def test_equals_deprecation(attr, args):
     point = points[0]
     tri = triangles[0]
 
     for other in [point, tri, shapely.geometry.Polygon()]:
         with pytest.warns(FutureWarning):
@@ -475,20 +478,36 @@
             for t in vals
         ]
     else:
         expected = [getattr(t, attr) if t is not None else na_value for t in vals]
     assert result.tolist() == expected
 
 
+def test_is_ring():
+    g = [
+        shapely.geometry.LinearRing([(0, 0), (1, 1), (1, -1)]),
+        shapely.geometry.LineString([(0, 0), (1, 1), (1, -1)]),
+        shapely.geometry.LineString([(0, 0), (1, 1), (1, -1), (0, 0)]),
+        shapely.geometry.Polygon([(0, 0), (1, 1), (1, -1)]),
+        shapely.geometry.Polygon(),
+        None,
+    ]
+    expected = [True, False, True, True, False, False]
+
+    result = from_shapely(g).is_ring
+
+    assert result.tolist() == expected
+
+
 @pytest.mark.parametrize("attr", ["area", "length"])
 def test_unary_float(attr):
     na_value = np.nan
     result = getattr(T, attr)
     assert isinstance(result, np.ndarray)
-    assert result.dtype == np.float
+    assert result.dtype == np.dtype("float64")
     expected = [getattr(t, attr) if t is not None else na_value for t in triangles]
     np.testing.assert_allclose(result, expected)
 
 
 def test_geom_types():
     cat = T.geom_type
     # empty polygon has GeometryCollection type
@@ -749,14 +768,23 @@
 
     res = a1 == a2
     assert res.tolist() == [True, False, True]
 
     res = a1 != a2
     assert res.tolist() == [False, True, False]
 
+    # check the correct expansion of list-like geometry
+    multi_poly = shapely.geometry.MultiPolygon(
+        [shapely.geometry.box(0, 0, 1, 1), shapely.geometry.box(3, 3, 4, 4)]
+    )
+    a3 = from_shapely([points[1], points[2], points[3], multi_poly])
+
+    res = a3 == multi_poly
+    assert res.tolist() == [False, False, False, True]
+
 
 def test_dir():
     assert "contains" in dir(P)
     assert "data" in dir(P)
 
 
 def test_chaining():
@@ -852,7 +880,59 @@
 
 
 @pytest.mark.skipif(not compat.PANDAS_GE_10, reason="pd.NA introduced in pandas 1.0")
 def test_isna_pdNA():
     t1 = T.copy()
     t1[0] = pd.NA
     assert t1[0] is None
+
+
+def test_shift_has_crs():
+    t = T.copy()
+    t.crs = 4326
+    assert t.shift(1).crs == t.crs
+    assert t.shift(0).crs == t.crs
+    assert t.shift(-1).crs == t.crs
+
+
+@pytest.mark.skipif(
+    not compat.PANDAS_GE_115, reason="crs only preserved in unique after pandas 1.1.5"
+)
+def test_unique_has_crs():
+    t = T.copy()
+    t.crs = 4326
+    assert t.unique().crs == t.crs
+
+
+class TestEstimateUtmCrs:
+    def setup_method(self):
+        self.esb = shapely.geometry.Point(-73.9847, 40.7484)
+        self.sol = shapely.geometry.Point(-74.0446, 40.6893)
+        self.landmarks = from_shapely([self.esb, self.sol], crs="epsg:4326")
+
+    def test_estimate_utm_crs__geographic(self):
+        if compat.PYPROJ_LT_3:
+            with pytest.raises(RuntimeError, match=r"pyproj 3\+ required"):
+                self.landmarks.estimate_utm_crs()
+        else:
+            assert self.landmarks.estimate_utm_crs() == CRS("EPSG:32618")
+            assert self.landmarks.estimate_utm_crs("NAD83") == CRS("EPSG:26918")
+
+    @pytest.mark.skipif(compat.PYPROJ_LT_3, reason="requires pyproj 3 or higher")
+    def test_estimate_utm_crs__projected(self):
+        assert self.landmarks.to_crs("EPSG:3857").estimate_utm_crs() == CRS(
+            "EPSG:32618"
+        )
+
+    @pytest.mark.skipif(compat.PYPROJ_LT_3, reason="requires pyproj 3 or higher")
+    def test_estimate_utm_crs__out_of_bounds(self):
+        with pytest.raises(RuntimeError, match="Unable to determine UTM CRS"):
+            from_shapely(
+                [shapely.geometry.Polygon([(0, 90), (1, 90), (2, 90)])], crs="EPSG:4326"
+            ).estimate_utm_crs()
+
+    @pytest.mark.skipif(compat.PYPROJ_LT_3, reason="requires pyproj 3 or higher")
+    def test_estimate_utm_crs__missing_crs(self):
+        with pytest.raises(RuntimeError, match="crs must be set"):
+            from_shapely(
+                [shapely.geometry.Polygon([(0, 90), (1, 90), (2, 90)])]
+            ).estimate_utm_crs()
```

### Comparing `geopandas-0.8.2/geopandas/tests/test_compat.py` & `geopandas-0.9.0/geopandas/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `geopandas-0.8.2/geopandas/tests/test_config.py` & `geopandas-0.9.0/geopandas/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `geopandas-0.8.2/geopandas/tests/test_crs.py` & `geopandas-0.9.0/geopandas/tests/test_crs.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,23 @@
 def test_to_crs_transform():
     df = df_epsg26918()
     lonlat = df.to_crs(epsg=4326)
     utm = lonlat.to_crs(epsg=26918)
     assert_geodataframe_equal(df, utm, check_less_precise=True)
 
 
+def test_to_crs_transform__missing_data():
+    # https://github.com/geopandas/geopandas/issues/1573
+    df = df_epsg26918()
+    df.loc[3, "geometry"] = None
+    lonlat = df.to_crs(epsg=4326)
+    utm = lonlat.to_crs(epsg=26918)
+    assert_geodataframe_equal(df, utm, check_less_precise=True)
+
+
 def test_to_crs_inplace():
     df = df_epsg26918()
     lonlat = df.to_crs(epsg=4326)
     df.to_crs(epsg=4326, inplace=True)
     assert_geodataframe_equal(df, lonlat, check_less_precise=True)
 
 
@@ -379,15 +388,15 @@
         assert df.geometry.crs == self.osgb
         assert df.geometry.values.crs == self.osgb
 
         df = df.rename(columns={"col1": "column1"})
         assert df.column1.crs == self.wgs
         assert df.column1.values.crs == self.wgs
 
-    def test_to_crs(self):
+    def test_geoseries_to_crs(self):
         s = GeoSeries(self.geoms, crs=27700)
         s = s.to_crs(4326)
         assert s.crs == self.wgs
         assert s.values.crs == self.wgs
 
         df = GeoDataFrame(geometry=s)
         assert df.crs == self.wgs
@@ -399,14 +408,19 @@
         # make sure that only active geometry is transformed
         arr = from_shapely(self.geoms, crs=4326)
         df["col1"] = arr
         df = df.to_crs(3857)
         assert df.col1.crs == self.wgs
         assert df.col1.values.crs == self.wgs
 
+    def test_array_to_crs(self):
+        arr = from_shapely(self.geoms, crs=27700)
+        arr = arr.to_crs(4326)
+        assert arr.crs == self.wgs
+
     def test_from_shapely(self):
         arr = from_shapely(self.geoms, crs=27700)
         assert arr.crs == self.osgb
 
     def test_from_wkb(self):
         L_wkb = [p.wkb for p in self.geoms]
         arr = from_wkb(L_wkb, crs=27700)
@@ -525,20 +539,26 @@
         assert merged.col2.values.crs == self.wgs
         assert merged.geom.values.crs == self.osgb
         assert merged.crs == self.osgb
 
     # CRS should be assigned to geometry
     def test_deprecation(self):
         with pytest.warns(FutureWarning):
-            GeoDataFrame([], crs=27700)
+            df = GeoDataFrame([], crs=27700)
+
+        # https://github.com/geopandas/geopandas/issues/1548
+        # ensure we still have converted the crs value to a CRS object
+        assert isinstance(df.crs, pyproj.CRS)
 
         with pytest.warns(FutureWarning):
             df = GeoDataFrame([])
             df.crs = 27700
 
+        assert isinstance(df.crs, pyproj.CRS)
+
     # make sure that geometry column from list has CRS (__setitem__)
     def test_setitem_geometry(self):
         arr = from_shapely(self.geoms, crs=27700)
         df = GeoDataFrame({"col1": [0, 1]}, geometry=arr)
 
         df["geometry"] = [g for g in df.geometry]
         assert df.geometry.values.crs == self.osgb
@@ -557,14 +577,24 @@
         s = GeoSeries(self.arr)
         assert s.crs == 27700
 
         # apply preserves the CRS if the result is a GeoSeries
         result = s.apply(lambda x: x.centroid)
         assert result.crs == 27700
 
+    def test_apply_geodataframe(self):
+        df = GeoDataFrame({"col1": [0, 1]}, geometry=self.geoms, crs=27700)
+        assert df.crs == 27700
+
+        # apply preserves the CRS if the result is a GeoDataFrame
+        result = df.apply(lambda col: col, axis=0)
+        assert result.crs == 27700
+        result = df.apply(lambda row: row, axis=1)
+        assert result.crs == 27700
+
 
 class TestSetCRS:
     @pytest.mark.parametrize(
         "constructor",
         [
             lambda geoms, crs: GeoSeries(geoms, crs=crs),
             lambda geoms, crs: GeoDataFrame(geometry=geoms, crs=crs),
```

### Comparing `geopandas-0.8.2/geopandas/tests/test_extension_array.py` & `geopandas-0.9.0/geopandas/tests/test_extension_array.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,59 +12,47 @@
 A set of fixtures are defined to provide data for the tests (the fixtures
 expected to be available to pytest by the inherited pandas tests).
 
 """
 import operator
 
 import numpy as np
+from numpy.testing import assert_array_equal
 import pandas as pd
 from pandas.tests.extension import base as extension_tests
 
 import shapely.geometry
 
-from geopandas._compat import PANDAS_GE_024
 from geopandas.array import GeometryArray, GeometryDtype, from_shapely
 
 import pytest
 
 # -----------------------------------------------------------------------------
 # Compat with extension tests in older pandas versions
 # -----------------------------------------------------------------------------
 
 
-if not PANDAS_GE_024:
-    # pandas 0.23.4 doesn't have those tests yet, so adding dummy classes
-    # to derive from here
-    extension_tests.BaseNoReduceTests = object
-    extension_tests.BaseArithmeticOpsTests = object
-    extension_tests.BaseComparisonOpsTests = object
-    extension_tests.BasePrintingTests = object
-    extension_tests.BaseParsingTests = object
-
-
 not_yet_implemented = pytest.mark.skip(reason="Not yet implemented")
 no_sorting = pytest.mark.skip(reason="Sorting not supported")
-skip_pandas_below_024 = pytest.mark.skipif(
-    not PANDAS_GE_024, reason="Sorting not supported"
-)
 
 
 # -----------------------------------------------------------------------------
 # Required fixtures
 # -----------------------------------------------------------------------------
 
 
 @pytest.fixture
 def dtype():
     """A fixture providing the ExtensionDtype to validate."""
     return GeometryDtype()
 
 
 def make_data():
-    a = np.array([shapely.geometry.Point(i, i) for i in range(100)], dtype=object)
+    a = np.empty(100, dtype=object)
+    a[:] = [shapely.geometry.Point(i, i) for i in range(100)]
     ga = from_shapely(a)
     return ga
 
 
 @pytest.fixture
 def data():
     """Length-100 array for this type.
@@ -288,25 +276,51 @@
 class TestDtype(extension_tests.BaseDtypeTests):
 
     # additional tests
 
     def test_array_type_with_arg(self, data, dtype):
         assert dtype.construct_array_type() is GeometryArray
 
-    @skip_pandas_below_024
     def test_registry(self, data, dtype):
         s = pd.Series(np.asarray(data), dtype=object)
         result = s.astype("geometry")
         assert isinstance(result.array, GeometryArray)
         expected = pd.Series(data)
         self.assert_series_equal(result, expected)
 
 
 class TestInterface(extension_tests.BaseInterfaceTests):
-    pass
+    def test_array_interface(self, data):
+        # we are overriding this base test because the creation of `expected`
+        # potentionally doesn't work for shapely geometries
+        # TODO can be removed with Shapely 2.0
+        result = np.array(data)
+        assert result[0] == data[0]
+
+        result = np.array(data, dtype=object)
+        # expected = np.array(list(data), dtype=object)
+        expected = np.empty(len(data), dtype=object)
+        expected[:] = list(data)
+        assert_array_equal(result, expected)
+
+    def test_contains(self, data, data_missing):
+        # overrided due to the inconsistency between
+        # GeometryDtype.na_value = np.nan
+        # and None being used as NA in array
+
+        # ensure data without missing values
+        data = data[~data.isna()]
+
+        # first elements are non-missing
+        assert data[0] in data
+        assert data_missing[0] in data_missing
+
+        assert None in data_missing
+        assert None not in data
+        assert pd.NaT not in data_missing
 
 
 class TestConstructors(extension_tests.BaseConstructorsTests):
     pass
 
 
 class TestReshaping(extension_tests.BaseReshapingTests):
@@ -399,21 +413,19 @@
 class TestComparisonOps(extension_tests.BaseComparisonOpsTests):
     def _compare_other(self, s, data, op_name, other):
         op = getattr(operator, op_name.strip("_"))
         result = op(s, other)
         expected = s.combine(other, op)
         self.assert_series_equal(result, expected)
 
-    @skip_pandas_below_024
     def test_compare_scalar(self, data, all_compare_operators):  # noqa
         op_name = all_compare_operators
         s = pd.Series(data)
         self._compare_other(s, data, op_name, data[0])
 
-    @skip_pandas_below_024
     def test_compare_array(self, data, all_compare_operators):  # noqa
         op_name = all_compare_operators
         s = pd.Series(data)
         other = pd.Series([data[0]] * len(data))
         self._compare_other(s, data, op_name, other)
 
 
@@ -505,14 +517,22 @@
     def test_argmin_argmax_empty_array(self):
         pass
 
     @no_sorting
     def test_argmin_argmax_all_na(self):
         pass
 
+    @no_sorting
+    def test_argreduce_series(self):
+        pass
+
+    @no_sorting
+    def test_argmax_argmin_no_skipna_notimplemented(self):
+        pass
+
 
 class TestCasting(extension_tests.BaseCastingTests):
     pass
 
 
 class TestGroupby(extension_tests.BaseGroupbyTests):
     @no_sorting
```

### Comparing `geopandas-0.8.2/geopandas/tests/test_geocode.py` & `geopandas-0.9.0/geopandas/tests/test_geocode.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-import numpy as np
 import pandas as pd
 
 from shapely.geometry import Point
 
 from geopandas import GeoDataFrame, GeoSeries
 from geopandas.tools import geocode, reverse_geocode
 from geopandas.tools.geocoding import _prepare_geocode_result
 
 from geopandas.tests.util import assert_geoseries_equal, mock
 from pandas.testing import assert_series_equal
+from geopandas.testing import assert_geodataframe_equal
 import pytest
 
 geopy = pytest.importorskip("geopy")
 
 
 class ForwardMock(mock.MagicMock):
     """
@@ -102,15 +102,29 @@
     # gets converted to that in conversion to pygeos. When converting back
     # on access, you now get a GeometryCollection object instead of Point,
     # which has no coords
     # see https://github.com/Toblerity/Shapely/issues/742/#issuecomment-545296708
     # TODO we should probably replace this with a missing value instead of point?
     # assert len(row["geometry"].coords) == 0
     assert row["geometry"].is_empty
-    assert np.isnan(row["address"])
+    assert row["address"] is None
+
+
+@pytest.mark.parametrize("geocode_result", (None, (None, None)))
+def test_prepare_geocode_result_when_result_is(geocode_result):
+
+    result = {0: geocode_result}
+    expected_output = GeoDataFrame(
+        {"geometry": [Point()], "address": [None]},
+        crs="EPSG:4326",
+    )
+
+    output = _prepare_geocode_result(result)
+
+    assert_geodataframe_equal(output, expected_output)
 
 
 def test_bad_provider_forward():
     from geopy.exc import GeocoderNotFound
 
     with pytest.raises(GeocoderNotFound):
         geocode(["cambridge, ma"], "badprovider")
```

### Comparing `geopandas-0.8.2/geopandas/tests/test_geodataframe.py` & `geopandas-0.9.0/geopandas/tests/test_geodataframe.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 import json
 import os
 import shutil
 import tempfile
+from distutils.version import LooseVersion
 
 import numpy as np
 import pandas as pd
 
-import fiona
+import pyproj
+from pyproj import CRS
 from pyproj.exceptions import CRSError
 from shapely.geometry import Point
 
 import geopandas
 from geopandas import GeoDataFrame, GeoSeries, read_file
 from geopandas.array import GeometryArray, GeometryDtype, from_shapely
 
 from geopandas.testing import assert_geodataframe_equal, assert_geoseries_equal
 from geopandas.tests.util import PACKAGE_DIR, validate_boro_df
 from pandas.testing import assert_frame_equal, assert_index_equal, assert_series_equal
 import pytest
 
 
+PYPROJ_LT_3 = LooseVersion(pyproj.__version__) < LooseVersion("3")
+
+
 class TestDataFrame:
     def setup_method(self):
         N = 10
 
         nybb_filename = geopandas.datasets.get_path("nybb")
         self.df = read_file(nybb_filename)
         self.tempdir = tempfile.mkdtemp()
@@ -31,15 +36,17 @@
         self.df2 = GeoDataFrame(
             [
                 {"geometry": Point(x, y), "value1": x + y, "value2": x * y}
                 for x, y in zip(range(N), range(N))
             ],
             crs=self.crs,
         )
-        self.df3 = read_file(os.path.join(PACKAGE_DIR, "examples", "null_geom.geojson"))
+        self.df3 = read_file(
+            os.path.join(PACKAGE_DIR, "geopandas", "tests", "data", "null_geom.geojson")
+        )
 
     def teardown_method(self):
         shutil.rmtree(self.tempdir)
 
     def test_df_init(self):
         assert type(self.df2) is GeoDataFrame
         assert self.df2.crs == self.crs
@@ -205,14 +212,21 @@
         assert self.df.geometry.name == "geometry"
         df2 = self.df.rename_geometry("new_name")
         assert df2.geometry.name == "new_name"
         df2 = self.df.rename_geometry("new_name", inplace=True)
         assert df2 is None
         assert self.df.geometry.name == "new_name"
 
+        # existing column error
+        msg = "Column named Shape_Area already exists"
+        with pytest.raises(ValueError, match=msg):
+            df2 = self.df.rename_geometry("Shape_Area")
+        with pytest.raises(ValueError, match=msg):
+            self.df.rename_geometry("Shape_Area", inplace=True)
+
     def test_set_geometry(self):
         geom = GeoSeries([Point(x, y) for x, y in zip(range(5), range(5))])
         original_geom = self.df.geometry
 
         df2 = self.df.set_geometry(geom)
         assert self.df is not df2
         assert_geoseries_equal(df2.geometry, geom, check_crs=False)
@@ -347,26 +361,33 @@
         assert_frame_equal(res2, exp2_nogeom)
 
     def test_to_json(self):
         text = self.df.to_json()
         data = json.loads(text)
         assert data["type"] == "FeatureCollection"
         assert len(data["features"]) == 5
+        assert "id" in data["features"][0].keys()
 
     def test_to_json_geom_col(self):
         df = self.df.copy()
         df["geom"] = df["geometry"]
         df["geometry"] = np.arange(len(df))
         df.set_geometry("geom", inplace=True)
 
         text = df.to_json()
         data = json.loads(text)
         assert data["type"] == "FeatureCollection"
         assert len(data["features"]) == 5
 
+    def test_to_json_only_geom_column(self):
+        text = self.df[["geometry"]].to_json()
+        data = json.loads(text)
+        assert len(data["features"]) == 5
+        assert "id" in data["features"][0].keys()
+
     def test_to_json_na(self):
         # Set a value as nan and make sure it's written
         self.df.loc[self.df["BoroName"] == "Queens", "Shape_Area"] = np.nan
 
         text = self.df.to_json()
         data = json.loads(text)
         assert len(data["features"]) == 5
@@ -418,14 +439,28 @@
                 # Just make sure setting it to nan in a different row
                 # doesn't affect this one
                 assert "Shape_Leng" in props
             elif props["BoroName"] == "Bronx":
                 assert np.isnan(props["Shape_Leng"])
                 assert "Shape_Area" in props
 
+    def test_to_json_drop_id(self):
+        text = self.df.to_json(drop_id=True)
+        data = json.loads(text)
+        assert len(data["features"]) == 5
+        for f in data["features"]:
+            assert "id" not in f.keys()
+
+    def test_to_json_drop_id_only_geom_column(self):
+        text = self.df[["geometry"]].to_json(drop_id=True)
+        data = json.loads(text)
+        assert len(data["features"]) == 5
+        for f in data["features"]:
+            assert "id" not in f.keys()
+
     def test_copy(self):
         df2 = self.df.copy()
         assert type(df2) is GeoDataFrame
         assert self.df.crs == df2.crs
 
     def test_to_file_crs(self):
         """
@@ -462,15 +497,26 @@
     def test_coord_slice_points(self):
         assert self.df2.cx[-2:-1, -2:-1].empty
         assert_frame_equal(self.df2, self.df2.cx[:, :])
         assert_frame_equal(self.df2.loc[5:], self.df2.cx[5:, :])
         assert_frame_equal(self.df2.loc[5:], self.df2.cx[:, 5:])
         assert_frame_equal(self.df2.loc[5:], self.df2.cx[5:, 5:])
 
+    def test_from_dict(self):
+        data = {"A": [1], "geometry": [Point(0.0, 0.0)]}
+        df = GeoDataFrame.from_dict(data, crs=3857)
+        assert df.crs == "epsg:3857"
+        assert df._geometry_column_name == "geometry"
+
+        data = {"B": [1], "location": [Point(0.0, 0.0)]}
+        df = GeoDataFrame.from_dict(data, geometry="location")
+        assert df._geometry_column_name == "location"
+
     def test_from_features(self):
+        fiona = pytest.importorskip("fiona")
         nybb_filename = geopandas.datasets.get_path("nybb")
         with fiona.open(nybb_filename) as f:
             features = list(f)
             crs = f.crs_wkt
 
         df = GeoDataFrame.from_features(features, crs=crs)
         validate_boro_df(df, case_sensitive=True)
@@ -546,15 +592,15 @@
 
         # test __geo_interface__ attribute (a GeoDataFrame has one)
         res = GeoDataFrame.from_features(gdf)
         assert_frame_equal(res, expected)
 
     def test_dataframe_to_geodataframe(self):
         df = pd.DataFrame(
-            {"A": range(len(self.df)), "location": list(self.df.geometry)},
+            {"A": range(len(self.df)), "location": np.array(self.df.geometry)},
             index=self.df.index,
         )
         gf = df.set_geometry("location", crs=self.df.crs)
         assert isinstance(df, pd.DataFrame)
         assert isinstance(gf, GeoDataFrame)
         assert_geoseries_equal(gf.geometry, self.df.geometry)
         assert gf.geometry.name == "location"
@@ -648,14 +694,60 @@
     def test_pickle_method(self):
         filename = os.path.join(self.tempdir, "df.pkl")
         self.df.to_pickle(filename)
         unpickled = pd.read_pickle(filename)
         assert_frame_equal(self.df, unpickled)
         assert self.df.crs == unpickled.crs
 
+    def test_estimate_utm_crs(self):
+        if PYPROJ_LT_3:
+            with pytest.raises(RuntimeError, match=r"pyproj 3\+ required"):
+                self.df.estimate_utm_crs()
+        else:
+            assert self.df.estimate_utm_crs() == CRS("EPSG:32618")
+            assert self.df.estimate_utm_crs("NAD83") == CRS("EPSG:26918")
+
+    def test_to_wkb(self):
+        wkbs0 = [
+            (
+                b"\x01\x01\x00\x00\x00\x00\x00\x00\x00\x00\x00"
+                b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"
+            ),  # POINT (0 0)
+            (
+                b"\x01\x01\x00\x00\x00\x00\x00\x00\x00\x00"
+                b"\x00\xf0?\x00\x00\x00\x00\x00\x00\xf0?"
+            ),  # POINT (1 1)
+        ]
+        wkbs1 = [
+            (
+                b"\x01\x01\x00\x00\x00\x00\x00\x00\x00\x00"
+                b"\x00\x00@\x00\x00\x00\x00\x00\x00\x00@"
+            ),  # POINT (2 2)
+            (
+                b"\x01\x01\x00\x00\x00\x00\x00\x00\x00\x00"
+                b"\x00\x08@\x00\x00\x00\x00\x00\x00\x08@"
+            ),  # POINT (3 3)
+        ]
+        gs0 = GeoSeries.from_wkb(wkbs0)
+        gs1 = GeoSeries.from_wkb(wkbs1)
+        gdf = GeoDataFrame({"geom_col0": gs0, "geom_col1": gs1})
+
+        expected_df = pd.DataFrame({"geom_col0": wkbs0, "geom_col1": wkbs1})
+        assert_frame_equal(expected_df, gdf.to_wkb())
+
+    def test_to_wkt(self):
+        wkts0 = ["POINT (0 0)", "POINT (1 1)"]
+        wkts1 = ["POINT (2 2)", "POINT (3 3)"]
+        gs0 = GeoSeries.from_wkt(wkts0)
+        gs1 = GeoSeries.from_wkt(wkts1)
+        gdf = GeoDataFrame({"gs0": gs0, "gs1": gs1})
+
+        expected_df = pd.DataFrame({"gs0": wkts0, "gs1": wkts1})
+        assert_frame_equal(expected_df, gdf.to_wkt())
+
 
 def check_geodataframe(df, geometry_column="geometry"):
     assert isinstance(df, GeoDataFrame)
     assert isinstance(df.geometry, GeoSeries)
     assert isinstance(df[geometry_column], GeoSeries)
     assert df._geometry_column_name == geometry_column
     assert df.geometry.name == geometry_column
```

### Comparing `geopandas-0.8.2/geopandas/tests/test_geom_methods.py` & `geopandas-0.9.0/geopandas/tests/test_geom_methods.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from shapely.geometry import LinearRing, LineString, MultiPoint, Point, Polygon
 from shapely.geometry.collection import GeometryCollection
 from shapely.ops import unary_union
 
 from geopandas import GeoDataFrame, GeoSeries
 from geopandas.base import GeoPandasBase
 
+from geopandas.testing import assert_geodataframe_equal
 from geopandas.tests.util import assert_geoseries_equal, geom_almost_equals, geom_equals
 from geopandas import _compat as compat
 from pandas.testing import assert_frame_equal, assert_series_equal
 import pytest
 
 
 def assert_array_dtype_equal(a, b, *args, **kwargs):
@@ -25,15 +26,18 @@
 
 
 class TestGeomMethods:
     def setup_method(self):
         self.t1 = Polygon([(0, 0), (1, 0), (1, 1)])
         self.t2 = Polygon([(0, 0), (1, 1), (0, 1)])
         self.t3 = Polygon([(2, 0), (3, 0), (3, 1)])
+        self.tz = Polygon([(1, 1, 1), (2, 2, 2), (3, 3, 3)])
+        self.tz1 = Polygon([(2, 2, 2), (1, 1, 1), (3, 3, 3)])
         self.sq = Polygon([(0, 0), (1, 0), (1, 1), (0, 1)])
+        self.sqz = Polygon([(1, 1, 1), (2, 2, 2), (3, 3, 3), (4, 4, 4)])
         self.t4 = Polygon([(0, 0), (3, 0), (3, 3), (0, 2)])
         self.t5 = Polygon([(2, 0), (3, 0), (3, 3), (2, 3)])
         self.inner_sq = Polygon(
             [(0.25, 0.25), (0.75, 0.25), (0.75, 0.75), (0.25, 0.75)]
         )
         self.nested_squares = Polygon(self.sq.boundary, [self.inner_sq.boundary])
         self.p0 = Point(5, 5)
@@ -48,36 +52,40 @@
                 self.p0,
                 None,
             ]
         )
         self.g1 = GeoSeries([self.t1, self.sq])
         self.g2 = GeoSeries([self.sq, self.t1])
         self.g3 = GeoSeries([self.t1, self.t2])
+        self.gz = GeoSeries([self.tz, self.sqz, self.tz1])
         self.g3.crs = "epsg:4326"
         self.g4 = GeoSeries([self.t2, self.t1])
         self.g4.crs = "epsg:4326"
         self.g_3d = GeoSeries([self.p0, self.p3d])
         self.na = GeoSeries([self.t1, self.t2, Polygon()])
         self.na_none = GeoSeries([self.t1, None])
         self.a1 = self.g1.copy()
         self.a1.index = ["A", "B"]
         self.a2 = self.g2.copy()
         self.a2.index = ["B", "C"]
-        self.esb = Point(-73.9847, 40.7484)
-        self.sol = Point(-74.0446, 40.6893)
+        self.esb = Point(-73.9847, 40.7484, 30.3244)
+        self.sol = Point(-74.0446, 40.6893, 31.2344)
         self.landmarks = GeoSeries([self.esb, self.sol], crs="epsg:4326")
+        self.pt2d = Point(-73.9847, 40.7484)
+        self.landmarks_mixed = GeoSeries([self.esb, self.sol, self.pt2d], crs=4326)
         self.l1 = LineString([(0, 0), (0, 1), (1, 1)])
         self.l2 = LineString([(0, 0), (1, 0), (1, 1), (0, 1)])
         self.g5 = GeoSeries([self.l1, self.l2])
         self.g6 = GeoSeries([self.p0, self.t3])
         self.g7 = GeoSeries([self.sq, self.t4])
         self.g8 = GeoSeries([self.t1, self.t5])
         self.empty = GeoSeries([])
         self.all_none = GeoSeries([None, None])
         self.empty_poly = Polygon()
+        self.g9 = GeoSeries(self.g0, index=range(1, 8))
 
         # Crossed lines
         self.l3 = LineString([(0, 0), (1, 1)])
         self.l4 = LineString([(0, 1), (1, 0)])
         self.crossed_lines = GeoSeries([self.l3, self.l4])
 
         # Placeholder for testing, will just drop in different geometries
@@ -87,14 +95,17 @@
         )
         self.gdf2 = GeoDataFrame(
             {"geometry": self.g1, "col3": [4, 5], "col4": ["rand", "string"]}
         )
         self.gdf3 = GeoDataFrame(
             {"geometry": self.g3, "col3": [4, 5], "col4": ["rand", "string"]}
         )
+        self.gdfz = GeoDataFrame(
+            {"geometry": self.gz, "col3": [4, 5, 6], "col4": ["rand", "string", "geo"]}
+        )
 
     def _test_unary_real(self, op, expected, a):
         """ Tests for 'area', 'length', 'is_valid', etc. """
         fcmp = assert_series_equal
         self._test_unary(op, expected, a, fcmp)
 
     def _test_unary_topological(self, op, expected, a):
@@ -230,33 +241,45 @@
     def test_intersection(self):
         self._test_binary_topological("intersection", self.t1, self.g1, self.g2)
         with pytest.warns(UserWarning, match="The indices .+ different"):
             self._test_binary_topological(
                 "intersection", self.all_none, self.g1, self.empty
             )
 
+        assert len(self.g0.intersection(self.g9, align=True) == 8)
+        assert len(self.g0.intersection(self.g9, align=False) == 7)
+
     def test_union_series(self):
         self._test_binary_topological("union", self.sq, self.g1, self.g2)
 
+        assert len(self.g0.union(self.g9, align=True) == 8)
+        assert len(self.g0.union(self.g9, align=False) == 7)
+
     def test_union_polygon(self):
         self._test_binary_topological("union", self.sq, self.g1, self.t2)
 
     def test_symmetric_difference_series(self):
         self._test_binary_topological("symmetric_difference", self.sq, self.g3, self.g4)
 
+        assert len(self.g0.symmetric_difference(self.g9, align=True) == 8)
+        assert len(self.g0.symmetric_difference(self.g9, align=False) == 7)
+
     def test_symmetric_difference_poly(self):
         expected = GeoSeries([GeometryCollection(), self.sq], crs=self.g3.crs)
         self._test_binary_topological(
             "symmetric_difference", expected, self.g3, self.t1
         )
 
     def test_difference_series(self):
         expected = GeoSeries([GeometryCollection(), self.t2])
         self._test_binary_topological("difference", expected, self.g1, self.g2)
 
+        assert len(self.g0.difference(self.g9, align=True) == 8)
+        assert len(self.g0.difference(self.g9, align=False) == 7)
+
     def test_difference_poly(self):
         expected = GeoSeries([self.t1, self.t1])
         self._test_binary_topological("difference", expected, self.g1, self.t2)
 
     def test_geo_op_empty_result(self):
         l1 = LineString([(0, 0), (1, 1)])
         l2 = LineString([(2, 2), (3, 3)])
@@ -327,14 +350,20 @@
 
         self._test_unary_topological("unary_union", expected, g)
 
     def test_contains(self):
         expected = [True, False, True, False, False, False, False]
         assert_array_dtype_equal(expected, self.g0.contains(self.t1))
 
+        expected = [False, True, True, True, True, True, False, False]
+        assert_array_dtype_equal(expected, self.g0.contains(self.g9, align=True))
+
+        expected = [False, False, True, False, False, False, False]
+        assert_array_dtype_equal(expected, self.g0.contains(self.g9, align=False))
+
     def test_length(self):
         expected = Series(np.array([2 + np.sqrt(2), 4]), index=self.g1.index)
         self._test_unary_real("length", expected, self.g1)
 
         expected = Series(np.array([2 + np.sqrt(2), np.nan]), index=self.na_none.index)
         self._test_unary_real("length", expected, self.na_none)
 
@@ -345,18 +374,30 @@
     def test_crosses(self):
         expected = [False, False, False, False, False, False, False]
         assert_array_dtype_equal(expected, self.g0.crosses(self.t1))
 
         expected = [False, True]
         assert_array_dtype_equal(expected, self.crossed_lines.crosses(self.l3))
 
+        expected = [False] * 8
+        assert_array_dtype_equal(expected, self.g0.crosses(self.g9, align=True))
+
+        expected = [False] * 7
+        assert_array_dtype_equal(expected, self.g0.crosses(self.g9, align=False))
+
     def test_disjoint(self):
         expected = [False, False, False, False, False, True, False]
         assert_array_dtype_equal(expected, self.g0.disjoint(self.t1))
 
+        expected = [False] * 8
+        assert_array_dtype_equal(expected, self.g0.disjoint(self.g9, align=True))
+
+        expected = [False, False, False, False, True, False, False]
+        assert_array_dtype_equal(expected, self.g0.disjoint(self.g9, align=False))
+
     def test_relate(self):
         expected = Series(
             [
                 "212101212",
                 "212101212",
                 "212FF1FF2",
                 "2FFF1FFF2",
@@ -367,23 +408,60 @@
             index=self.g0.index,
         )
         assert_array_dtype_equal(expected, self.g0.relate(self.inner_sq))
 
         expected = Series(["FF0FFF212", None], index=self.g6.index)
         assert_array_dtype_equal(expected, self.g6.relate(self.na_none))
 
+        expected = Series(
+            [
+                None,
+                "2FFF1FFF2",
+                "2FFF1FFF2",
+                "2FFF1FFF2",
+                "2FFF1FFF2",
+                "0FFFFFFF2",
+                None,
+                None,
+            ],
+            index=range(8),
+        )
+
+        assert_array_dtype_equal(expected, self.g0.relate(self.g9, align=True))
+
+        expected = Series(
+            [
+                "FF2F11212",
+                "2FF11F212",
+                "212FF1FF2",
+                "FF2F1F212",
+                "FF2FF10F2",
+                None,
+                None,
+            ],
+            index=self.g0.index,
+        )
+        assert_array_dtype_equal(expected, self.g0.relate(self.g9, align=False))
+
     def test_distance(self):
         expected = Series(
             np.array([np.sqrt((5 - 1) ** 2 + (5 - 1) ** 2), np.nan]), self.na_none.index
         )
         assert_array_dtype_equal(expected, self.na_none.distance(self.p0))
 
         expected = Series(np.array([np.sqrt(4 ** 2 + 4 ** 2), np.nan]), self.g6.index)
         assert_array_dtype_equal(expected, self.g6.distance(self.na_none))
 
+        expected = Series(np.array([np.nan, 0, 0, 0, 0, 0, np.nan, np.nan]), range(8))
+        assert_array_dtype_equal(expected, self.g0.distance(self.g9, align=True))
+
+        val = self.g0.iloc[4].distance(self.g9.iloc[4])
+        expected = Series(np.array([0, 0, 0, 0, val, np.nan, np.nan]), self.g0.index)
+        assert_array_dtype_equal(expected, self.g0.distance(self.g9, align=False))
+
     def test_distance_crs_warning(self):
         with pytest.warns(UserWarning, match="Geometry is in a geographic CRS"):
             self.g4.distance(self.p0)
 
     def test_intersects(self):
         expected = [True, True, True, True, True, False, False]
         assert_array_dtype_equal(expected, self.g0.intersects(self.t1))
@@ -396,57 +474,93 @@
 
         expected = np.array([], dtype=bool)
         assert_array_dtype_equal(expected, self.empty.intersects(self.empty_poly))
 
         expected = [False] * 7
         assert_array_dtype_equal(expected, self.g0.intersects(self.empty_poly))
 
+        expected = [False, True, True, True, True, True, False, False]
+        assert_array_dtype_equal(expected, self.g0.intersects(self.g9, align=True))
+
+        expected = [True, True, True, True, False, False, False]
+        assert_array_dtype_equal(expected, self.g0.intersects(self.g9, align=False))
+
     def test_overlaps(self):
         expected = [True, True, False, False, False, False, False]
         assert_array_dtype_equal(expected, self.g0.overlaps(self.inner_sq))
 
         expected = [False, False]
         assert_array_dtype_equal(expected, self.g4.overlaps(self.t1))
 
+        expected = [False] * 8
+        assert_array_dtype_equal(expected, self.g0.overlaps(self.g9, align=True))
+
+        expected = [False] * 7
+        assert_array_dtype_equal(expected, self.g0.overlaps(self.g9, align=False))
+
     def test_touches(self):
         expected = [False, True, False, False, False, False, False]
         assert_array_dtype_equal(expected, self.g0.touches(self.t1))
 
+        expected = [False] * 8
+        assert_array_dtype_equal(expected, self.g0.touches(self.g9, align=True))
+
+        expected = [True, False, False, True, False, False, False]
+        assert_array_dtype_equal(expected, self.g0.touches(self.g9, align=False))
+
     def test_within(self):
         expected = [True, False, False, False, False, False, False]
         assert_array_dtype_equal(expected, self.g0.within(self.t1))
 
         expected = [True, True, True, True, True, False, False]
         assert_array_dtype_equal(expected, self.g0.within(self.sq))
 
+        expected = [False, True, True, True, True, True, False, False]
+        assert_array_dtype_equal(expected, self.g0.within(self.g9, align=True))
+
+        expected = [False, True, False, False, False, False, False]
+        assert_array_dtype_equal(expected, self.g0.within(self.g9, align=False))
+
     def test_covers_itself(self):
         # Each polygon in a Series covers itself
         res = self.g1.covers(self.g1)
         exp = Series([True, True])
         assert_series_equal(res, exp)
 
     def test_covers(self):
         res = self.g7.covers(self.g8)
         exp = Series([True, False])
         assert_series_equal(res, exp)
 
+        expected = [False, True, True, True, True, True, False, False]
+        assert_array_dtype_equal(expected, self.g0.covers(self.g9, align=True))
+
+        expected = [False, False, True, False, False, False, False]
+        assert_array_dtype_equal(expected, self.g0.covers(self.g9, align=False))
+
     def test_covers_inverse(self):
         res = self.g8.covers(self.g7)
         exp = Series([False, False])
         assert_series_equal(res, exp)
 
     @pytest.mark.skipif(
         not compat.USE_PYGEOS,
         reason="covered_by is only implemented for pygeos, not shapely",
     )
     def test_covered_by(self):
         res = self.g1.covered_by(self.g1)
         exp = Series([True, True])
         assert_series_equal(res, exp)
 
+        expected = [False, True, True, True, True, True, False, False]
+        assert_array_dtype_equal(expected, self.g0.covered_by(self.g9, align=True))
+
+        expected = [False, True, False, False, False, False, False]
+        assert_array_dtype_equal(expected, self.g0.covered_by(self.g9, align=False))
+
     def test_is_valid(self):
         expected = Series(np.array([True] * len(self.g1)), self.g1.index)
         self._test_unary_real("is_valid", expected, self.g1)
 
     def test_is_empty(self):
         expected = Series(np.array([False] * len(self.g1)), self.g1.index)
         self._test_unary_real("is_empty", expected, self.g1)
@@ -459,28 +573,37 @@
         expected = Series(np.array([True] * len(self.g1)), self.g1.index)
         self._test_unary_real("is_simple", expected, self.g1)
 
     def test_has_z(self):
         expected = Series([False, True], self.g_3d.index)
         self._test_unary_real("has_z", expected, self.g_3d)
 
-    def test_xy_points(self):
+    def test_xyz_points(self):
         expected_x = [-73.9847, -74.0446]
         expected_y = [40.7484, 40.6893]
+        expected_z = [30.3244, 31.2344]
 
         assert_array_dtype_equal(expected_x, self.landmarks.geometry.x)
         assert_array_dtype_equal(expected_y, self.landmarks.geometry.y)
+        assert_array_dtype_equal(expected_z, self.landmarks.geometry.z)
 
-    def test_xy_polygons(self):
+        # mixed dimensions
+        expected_z = [30.3244, 31.2344, np.nan]
+        assert_array_dtype_equal(expected_z, self.landmarks_mixed.geometry.z)
+
+    def test_xyz_polygons(self):
         # accessing x attribute in polygon geoseries should raise an error
         with pytest.raises(ValueError):
             _ = self.gdf1.geometry.x
         # and same for accessing y attribute in polygon geoseries
         with pytest.raises(ValueError):
             _ = self.gdf1.geometry.y
+        # and same for accessing z attribute in polygon geoseries
+        with pytest.raises(ValueError):
+            _ = self.gdfz.geometry.z
 
     def test_centroid(self):
         polygon = Polygon([(-1, -1), (1, -1), (1, 1), (-1, 1)])
         point = Point(0, 0)
         polygons = GeoSeries([polygon for i in range(3)])
         points = GeoSeries([point for i in range(3)])
         assert_geoseries_equal(polygons.centroid, points)
@@ -549,14 +672,21 @@
         expected = Series([2.0, 1.5], index=self.g5.index)
         p = Point(1.0, 0.5)
         self._test_binary_real("project", expected, self.g5, p)
 
         expected = Series([1.0, 0.5], index=self.g5.index)
         self._test_binary_real("project", expected, self.g5, p, normalized=True)
 
+        s = GeoSeries([Point(2, 2), Point(0.5, 0.5)], index=[1, 2])
+        expected = Series([np.nan, 2.0, np.nan])
+        assert_series_equal(self.g5.project(s), expected)
+
+        expected = Series([2.0, 0.5], index=self.g5.index)
+        assert_series_equal(self.g5.project(s, align=False), expected)
+
     def test_affine_transform(self):
         # 45 degree reflection matrix
         matrix = [0, 1, 1, 0, 0, 0]
         expected = self.g4
 
         res = self.g3.affine_transform(matrix)
         assert_geoseries_equal(expected, res)
@@ -667,15 +797,16 @@
         with pytest.warns(UserWarning, match="Geometry is in a geographic CRS"):
             self.g4.buffer(1)
 
         with pytest.warns(None) as record:
             # do not warn for 0
             self.g4.buffer(0)
 
-        assert len(record) == 0
+        for r in record:
+            assert "Geometry is in a geographic CRS." not in str(r.message)
 
     def test_envelope(self):
         e = self.g3.envelope
         assert np.all(e.geom_equals(self.sq))
         assert isinstance(e, GeoSeries)
         assert self.g3.crs == e.crs
 
@@ -687,22 +818,24 @@
         df = GeoDataFrame(
             {"geometry": self.landmarks, "col1": range(len(self.landmarks))}
         )
         assert tuple(df.total_bounds) == bbox
 
     def test_explode_geoseries(self):
         s = GeoSeries(
-            [MultiPoint([(0, 0), (1, 1)]), MultiPoint([(2, 2), (3, 3), (4, 4)])]
+            [MultiPoint([(0, 0), (1, 1)]), MultiPoint([(2, 2), (3, 3), (4, 4)])],
+            crs=4326,
         )
         s.index.name = "test_index_name"
         expected_index_name = ["test_index_name", None]
         index = [(0, 0), (0, 1), (1, 0), (1, 1), (1, 2)]
         expected = GeoSeries(
             [Point(0, 0), Point(1, 1), Point(2, 2), Point(3, 3), Point(4, 4)],
             index=MultiIndex.from_tuples(index, names=expected_index_name),
+            crs=4326,
         )
         assert_geoseries_equal(expected, s.explode())
 
     @pytest.mark.parametrize("index_name", [None, "test"])
     def test_explode_geodataframe(self, index_name):
         s = GeoSeries([MultiPoint([Point(1, 2), Point(2, 3)]), Point(5, 5)])
         df = GeoDataFrame({"col": [1, 2], "geometry": s})
@@ -733,18 +866,85 @@
         expected_df = GeoDataFrame({"level_1": [1, 1, 2], "geometry": expected_s})
         expected_index = MultiIndex(
             [[0, 1], [0, 1]],  # levels
             [[0, 0, 1], [0, 1, 0]],  # labels/codes
             names=[index_name, None],
         )
         expected_df = expected_df.set_index(expected_index)
-        if not compat.PANDAS_GE_024:
-            expected_df = expected_df[["level_1", "geometry"]]
         assert_frame_equal(test_df, expected_df)
 
+    @pytest.mark.skipif(
+        not compat.PANDAS_GE_025,
+        reason="pandas explode introduced in pandas 0.25",
+    )
+    def test_explode_pandas_fallback(self):
+        d = {
+            "col1": [["name1", "name2"], ["name3", "name4"]],
+            "geometry": [
+                MultiPoint([(1, 2), (3, 4)]),
+                MultiPoint([(2, 1), (0, 0)]),
+            ],
+        }
+        gdf = GeoDataFrame(d, crs=4326)
+        expected_df = GeoDataFrame(
+            {
+                "col1": ["name1", "name2", "name3", "name4"],
+                "geometry": [
+                    MultiPoint([(1, 2), (3, 4)]),
+                    MultiPoint([(1, 2), (3, 4)]),
+                    MultiPoint([(2, 1), (0, 0)]),
+                    MultiPoint([(2, 1), (0, 0)]),
+                ],
+            },
+            index=[0, 0, 1, 1],
+            crs=4326,
+        )
+
+        # Test with column provided as arg
+        exploded_df = gdf.explode("col1")
+        assert_geodataframe_equal(exploded_df, expected_df)
+
+        # Test with column provided as kwarg
+        exploded_df = gdf.explode(column="col1")
+        assert_geodataframe_equal(exploded_df, expected_df)
+
+    @pytest.mark.skipif(
+        not compat.PANDAS_GE_11,
+        reason="ignore_index keyword introduced in pandas 1.1.0",
+    )
+    def test_explode_pandas_fallback_ignore_index(self):
+        d = {
+            "col1": [["name1", "name2"], ["name3", "name4"]],
+            "geometry": [
+                MultiPoint([(1, 2), (3, 4)]),
+                MultiPoint([(2, 1), (0, 0)]),
+            ],
+        }
+        gdf = GeoDataFrame(d, crs=4326)
+        expected_df = GeoDataFrame(
+            {
+                "col1": ["name1", "name2", "name3", "name4"],
+                "geometry": [
+                    MultiPoint([(1, 2), (3, 4)]),
+                    MultiPoint([(1, 2), (3, 4)]),
+                    MultiPoint([(2, 1), (0, 0)]),
+                    MultiPoint([(2, 1), (0, 0)]),
+                ],
+            },
+            crs=4326,
+        )
+
+        # Test with column provided as arg
+        exploded_df = gdf.explode("col1", ignore_index=True)
+        assert_geodataframe_equal(exploded_df, expected_df)
+
+        # Test with column provided as kwarg
+        exploded_df = gdf.explode(column="col1", ignore_index=True)
+        assert_geodataframe_equal(exploded_df, expected_df)
+
     #
     # Test '&', '|', '^', and '-'
     #
     def test_intersection_operator(self):
         with pytest.warns(DeprecationWarning):
             self._test_binary_operator("__and__", self.t1, self.g1, self.g2)
         with pytest.warns(DeprecationWarning):
```

### Comparing `geopandas-0.8.2/geopandas/tests/test_geoseries.py` & `geopandas-0.9.0/geopandas/tests/test_geoseries.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,26 +4,29 @@
 import shutil
 import tempfile
 
 import numpy as np
 from numpy.testing import assert_array_equal
 import pandas as pd
 
+from pyproj import CRS
 from shapely.geometry import (
     LineString,
     MultiLineString,
     MultiPoint,
     MultiPolygon,
     Point,
     Polygon,
 )
 from shapely.geometry.base import BaseGeometry
 
 from geopandas import GeoSeries, GeoDataFrame
+from geopandas._compat import PYPROJ_LT_3
 from geopandas.array import GeometryArray, GeometryDtype
+from geopandas.testing import assert_geoseries_equal
 
 from geopandas.tests.util import geom_equals
 from pandas.testing import assert_series_equal
 import pytest
 
 
 class TestSeries:
@@ -126,28 +129,46 @@
 
     def test_geom_equals(self):
         assert np.all(self.g1.geom_equals(self.g1))
         assert_array_equal(self.g1.geom_equals(self.sq), [False, True])
 
     def test_geom_equals_align(self):
         with pytest.warns(UserWarning, match="The indices .+ different"):
-            a = self.a1.geom_equals(self.a2)
+            a = self.a1.geom_equals(self.a2, align=True)
         exp = pd.Series([False, True, False], index=["A", "B", "C"])
         assert_series_equal(a, exp)
 
+        a = self.a1.geom_equals(self.a2, align=False)
+        exp = pd.Series([False, False], index=["A", "B"])
+        assert_series_equal(a, exp)
+
     def test_geom_almost_equals(self):
         # TODO: test decimal parameter
         assert np.all(self.g1.geom_almost_equals(self.g1))
         assert_array_equal(self.g1.geom_almost_equals(self.sq), [False, True])
 
+        assert_array_equal(
+            self.a1.geom_almost_equals(self.a2, align=True), [False, True, False]
+        )
+        assert_array_equal(
+            self.a1.geom_almost_equals(self.a2, align=False), [False, False]
+        )
+
     def test_geom_equals_exact(self):
         # TODO: test tolerance parameter
         assert np.all(self.g1.geom_equals_exact(self.g1, 0.001))
         assert_array_equal(self.g1.geom_equals_exact(self.sq, 0.001), [False, True])
 
+        assert_array_equal(
+            self.a1.geom_equals_exact(self.a2, 0.001, align=True), [False, True, False]
+        )
+        assert_array_equal(
+            self.a1.geom_equals_exact(self.a2, 0.001, align=False), [False, False]
+        )
+
     def test_equal_comp_op(self):
         s = GeoSeries([Point(x, x) for x in range(3)])
         res = s == Point(1, 1)
         exp = pd.Series([False, True, False])
         assert_series_equal(res, exp)
 
     def test_to_file(self):
@@ -178,14 +199,40 @@
         lonlat = utm18n.to_crs(epsg=4326)
         assert np.all(self.landmarks.geom_almost_equals(lonlat))
         with pytest.raises(ValueError):
             self.g1.to_crs(epsg=4326)
         with pytest.raises(ValueError):
             self.landmarks.to_crs(crs=None, epsg=None)
 
+    def test_estimate_utm_crs__geographic(self):
+        if PYPROJ_LT_3:
+            with pytest.raises(RuntimeError, match=r"pyproj 3\+ required"):
+                self.landmarks.estimate_utm_crs()
+        else:
+            assert self.landmarks.estimate_utm_crs() == CRS("EPSG:32618")
+            assert self.landmarks.estimate_utm_crs("NAD83") == CRS("EPSG:26918")
+
+    @pytest.mark.skipif(PYPROJ_LT_3, reason="requires pyproj 3 or higher")
+    def test_estimate_utm_crs__projected(self):
+        assert self.landmarks.to_crs("EPSG:3857").estimate_utm_crs() == CRS(
+            "EPSG:32618"
+        )
+
+    @pytest.mark.skipif(PYPROJ_LT_3, reason="requires pyproj 3 or higher")
+    def test_estimate_utm_crs__out_of_bounds(self):
+        with pytest.raises(RuntimeError, match="Unable to determine UTM CRS"):
+            GeoSeries(
+                [Polygon([(0, 90), (1, 90), (2, 90)])], crs="EPSG:4326"
+            ).estimate_utm_crs()
+
+    @pytest.mark.skipif(PYPROJ_LT_3, reason="requires pyproj 3 or higher")
+    def test_estimate_utm_crs__missing_crs(self):
+        with pytest.raises(RuntimeError, match="crs must be set"):
+            GeoSeries([Polygon([(0, 90), (1, 90), (2, 90)])]).estimate_utm_crs()
+
     def test_fillna(self):
         # default is to fill with empty geometry
         na = self.na_none.fillna()
         assert isinstance(na[2], BaseGeometry)
         assert na[2].is_empty
         assert geom_equals(self.na_none[:2], na[:2])
         # XXX: method works inconsistently for different pandas versions
@@ -232,14 +279,53 @@
         assert np.all(self.g3.geom_almost_equals(reprojected_back))
 
         # Conversions by different format
         reprojected_string = self.g3.to_crs("+proj=utm +zone=30N")
         reprojected_dict = self.g3.to_crs({"proj": "utm", "zone": "30N"})
         assert np.all(reprojected_string.geom_almost_equals(reprojected_dict))
 
+    def test_from_wkb(self):
+        assert_geoseries_equal(self.g1, GeoSeries.from_wkb([self.t1.wkb, self.sq.wkb]))
+
+    def test_from_wkb_series(self):
+        s = pd.Series([self.t1.wkb, self.sq.wkb], index=[1, 2])
+        expected = self.g1.copy()
+        expected.index = pd.Index([1, 2])
+        assert_geoseries_equal(expected, GeoSeries.from_wkb(s))
+
+    def test_from_wkb_series_with_index(self):
+        index = [0]
+        s = pd.Series([self.t1.wkb, self.sq.wkb], index=[0, 2])
+        expected = self.g1.reindex(index)
+        assert_geoseries_equal(expected, GeoSeries.from_wkb(s, index=index))
+
+    def test_from_wkt(self):
+        assert_geoseries_equal(self.g1, GeoSeries.from_wkt([self.t1.wkt, self.sq.wkt]))
+
+    def test_from_wkt_series(self):
+        s = pd.Series([self.t1.wkt, self.sq.wkt], index=[1, 2])
+        expected = self.g1.copy()
+        expected.index = pd.Index([1, 2])
+        assert_geoseries_equal(expected, GeoSeries.from_wkt(s))
+
+    def test_from_wkt_series_with_index(self):
+        index = [0]
+        s = pd.Series([self.t1.wkt, self.sq.wkt], index=[0, 2])
+        expected = self.g1.reindex(index)
+        assert_geoseries_equal(expected, GeoSeries.from_wkt(s, index=index))
+
+    def test_to_wkb(self):
+        assert_series_equal(pd.Series([self.t1.wkb, self.sq.wkb]), self.g1.to_wkb())
+        assert_series_equal(
+            pd.Series([self.t1.wkb_hex, self.sq.wkb_hex]), self.g1.to_wkb(hex=True)
+        )
+
+    def test_to_wkt(self):
+        assert_series_equal(pd.Series([self.t1.wkt, self.sq.wkt]), self.g1.to_wkt())
+
 
 def test_missing_values_empty_warning():
     s = GeoSeries([Point(1, 1), None, np.nan, BaseGeometry(), Polygon()])
     with pytest.warns(UserWarning):
         s.isna()
 
     with pytest.warns(UserWarning):
@@ -340,14 +426,18 @@
     def test_empty(self):
         s = GeoSeries([])
         check_geoseries(s)
 
         s = GeoSeries()
         check_geoseries(s)
 
+    def test_data_is_none(self):
+        s = GeoSeries(index=range(3))
+        check_geoseries(s)
+
     def test_from_series(self):
         shapes = [
             Polygon([(random.random(), random.random()) for _ in range(3)])
             for _ in range(10)
         ]
         s = pd.Series(shapes, index=list("abcdefghij"), name="foo")
         g = GeoSeries(s)
```

### Comparing `geopandas-0.8.2/geopandas/tests/test_merge.py` & `geopandas-0.9.0/geopandas/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `geopandas-0.8.2/geopandas/tests/test_overlay.py` & `geopandas-0.9.0/geopandas/tests/test_overlay.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import os
 
 import pandas as pd
 
-from shapely.geometry import Point, Polygon, LineString, GeometryCollection
+from shapely.geometry import Point, Polygon, LineString, GeometryCollection, box
 from fiona.errors import DriverError
 
 import geopandas
 from geopandas import GeoDataFrame, GeoSeries, overlay, read_file
 
 from geopandas.testing import assert_geodataframe_equal, assert_geoseries_equal
 import pytest
 
 DATA = os.path.join(os.path.abspath(os.path.dirname(__file__)), "data", "overlay")
 
 
-pytestmark = pytest.mark.skipif(
-    not geopandas.sindex.has_sindex(), reason="overlay requires spatial index"
-)
+pytestmark = pytest.mark.skip_no_sindex
 
 
 @pytest.fixture
 def dfs(request):
     s1 = GeoSeries(
         [
             Polygon([(0, 0), (2, 0), (2, 2), (0, 2)]),
@@ -105,27 +103,31 @@
         assert_geodataframe_equal(result, expected, check_column_type=False)
 
 
 @pytest.mark.filterwarnings("ignore:GeoSeries crs mismatch:UserWarning")
 def test_overlay_nybb(how):
     polydf = read_file(geopandas.datasets.get_path("nybb"))
 
-    # construct circles dataframe
-    N = 10
-    b = [int(x) for x in polydf.total_bounds]
-    polydf2 = GeoDataFrame(
-        [
-            {"geometry": Point(x, y).buffer(10000), "value1": x + y, "value2": x - y}
-            for x, y in zip(
-                range(b[0], b[2], int((b[2] - b[0]) / N)),
-                range(b[1], b[3], int((b[3] - b[1]) / N)),
-            )
-        ],
-        crs=polydf.crs,
-    )
+    # The circles have been constructed and saved at the time the expected
+    # results were created (exact output of buffer algorithm can slightly
+    # change over time -> use saved ones)
+    # # construct circles dataframe
+    # N = 10
+    # b = [int(x) for x in polydf.total_bounds]
+    # polydf2 = GeoDataFrame(
+    #     [
+    #         {"geometry": Point(x, y).buffer(10000), "value1": x + y, "value2": x - y}
+    #         for x, y in zip(
+    #             range(b[0], b[2], int((b[2] - b[0]) / N)),
+    #             range(b[1], b[3], int((b[3] - b[1]) / N)),
+    #         )
+    #     ],
+    #     crs=polydf.crs,
+    # )
+    polydf2 = read_file(os.path.join(DATA, "nybb_qgis", "polydf2.shp"))
 
     result = overlay(polydf, polydf2, how=how)
 
     cols = ["BoroCode", "BoroName", "Shape_Leng", "Shape_Area", "value1", "value2"]
     if how == "difference":
         cols = cols[:-2]
 
@@ -184,20 +186,31 @@
     pd.testing.assert_series_equal(
         result.geometry.area, expected.geometry.area, check_less_precise=True
     )
     pd.testing.assert_frame_equal(
         result.geometry.bounds, expected.geometry.bounds, check_less_precise=True
     )
 
-    # now drop multipolygons
-    result.geometry[result.geometry.geom_type == "MultiPolygon"] = None
-    expected.geometry[expected.geometry.geom_type == "MultiPolygon"] = None
+    # There are two cases where the multipolygon have a different number
+    # of sub-geometries -> not solved by normalize (and thus drop for now)
+    if how == "symmetric_difference":
+        expected.loc[9, "geometry"] = None
+        result.loc[9, "geometry"] = None
+
+    if how == "union":
+        expected.loc[24, "geometry"] = None
+        result.loc[24, "geometry"] = None
 
     assert_geodataframe_equal(
-        result, expected, check_crs=False, check_column_type=False
+        result,
+        expected,
+        normalize=True,
+        check_crs=False,
+        check_column_type=False,
+        check_less_precise=True,
     )
 
 
 def test_overlay_overlap(how):
     """
     Overlay test with overlapping geometries in both dataframes.
     Test files are created with::
@@ -242,15 +255,19 @@
 
     # TODO needed adaptations to result
     result = result.reset_index(drop=True)
     if how == "union":
         result = result.sort_values(["col1", "col2"]).reset_index(drop=True)
 
     assert_geodataframe_equal(
-        result, expected, check_column_type=False, check_less_precise=True
+        result,
+        expected,
+        normalize=True,
+        check_column_type=False,
+        check_less_precise=True,
     )
 
 
 @pytest.mark.parametrize("other_geometry", [False, True])
 def test_geometry_not_named_geometry(dfs, how, other_geometry):
     # Issue #306
     # Add points and flip names
@@ -361,18 +378,34 @@
     )
     df3 = GeoDataFrame({"geometry": polys3, "col3": [1, 2, 3]})
     i1 = Polygon([(1, 1), (1, 3), (3, 3), (3, 1), (1, 1)])
     i2 = Polygon([(3, 3), (3, 5), (5, 5), (5, 3), (3, 3)])
     expected = GeoDataFrame(
         [[1, 1, i1], [3, 2, i2]], columns=["col3", "col2", "geometry"]
     )
-    result = overlay(df3, df2)
+    result = overlay(df3, df2, keep_geom_type=True)
     assert_geodataframe_equal(result, expected)
 
 
+def test_warn_on_keep_geom_type(dfs):
+
+    df1, df2 = dfs
+    polys3 = GeoSeries(
+        [
+            Polygon([(1, 1), (3, 1), (3, 3), (1, 3)]),
+            Polygon([(-1, 1), (1, 1), (1, 3), (-1, 3)]),
+            Polygon([(3, 3), (5, 3), (5, 5), (3, 5)]),
+        ]
+    )
+    df3 = GeoDataFrame({"geometry": polys3})
+
+    with pytest.warns(UserWarning, match="`keep_geom_type=True` in overlay"):
+        overlay(df2, df3, keep_geom_type=None)
+
+
 @pytest.mark.parametrize(
     "geom_types", ["polys", "poly_line", "poly_point", "line_poly", "point_poly"]
 )
 def test_overlay_strict(how, keep_geom_type, geom_types):
     """
     Test of mixed geometry types on input and output. Expected results initially
     generated using following snippet.
@@ -467,14 +500,15 @@
         cols = list(set(result.columns) - set(["geometry"]))
         expected = expected.sort_values(cols, axis=0).reset_index(drop=True)
         result = result.sort_values(cols, axis=0).reset_index(drop=True)
 
         assert_geodataframe_equal(
             result,
             expected,
+            normalize=True,
             check_column_type=False,
             check_less_precise=True,
             check_crs=False,
             check_dtype=False,
         )
 
     except DriverError:  # fiona >= 1.8
@@ -518,7 +552,43 @@
             Polygon([(1, 1), (3, 1), (3, 3), (1, 3)]),
             Polygon([(3, 3), (5, 3), (5, 5), (3, 5)]),
         ]
     )
     df1 = GeoDataFrame({"col1": [1, 2], "geometry": polys1})
     with pytest.raises(TypeError):
         overlay(dfcol, df1, keep_geom_type=True)
+
+
+def test_keep_geom_type_geometry_collection():
+    # GH 1581
+
+    df1 = read_file(os.path.join(DATA, "geom_type", "df1.geojson"))
+    df2 = read_file(os.path.join(DATA, "geom_type", "df2.geojson"))
+
+    intersection = overlay(df1, df2, keep_geom_type=True)
+    assert len(intersection) == 1
+    assert (intersection.geom_type == "Polygon").all()
+
+    intersection = overlay(df1, df2, keep_geom_type=False)
+    assert len(intersection) == 1
+    assert (intersection.geom_type == "GeometryCollection").all()
+
+
+@pytest.mark.parametrize("make_valid", [True, False])
+def test_overlap_make_valid(make_valid):
+    bowtie = Polygon([(1, 1), (9, 9), (9, 1), (1, 9), (1, 1)])
+    assert not bowtie.is_valid
+    fixed_bowtie = bowtie.buffer(0)
+    assert fixed_bowtie.is_valid
+
+    df1 = GeoDataFrame({"col1": ["region"], "geometry": GeoSeries([box(0, 0, 10, 10)])})
+    df_bowtie = GeoDataFrame(
+        {"col1": ["invalid", "valid"], "geometry": GeoSeries([bowtie, fixed_bowtie])}
+    )
+
+    if make_valid:
+        df_overlay_bowtie = overlay(df1, df_bowtie, make_valid=make_valid)
+        assert df_overlay_bowtie.at[0, "geometry"].equals(fixed_bowtie)
+        assert df_overlay_bowtie.at[1, "geometry"].equals(fixed_bowtie)
+    else:
+        with pytest.raises(ValueError, match="1 invalid input geometries"):
+            overlay(df1, df_bowtie, make_valid=make_valid)
```

### Comparing `geopandas-0.8.2/geopandas/tests/test_pandas_methods.py` & `geopandas-0.9.0/geopandas/tests/test_pandas_methods.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pandas as pd
 
 import shapely
 from shapely.geometry import Point, GeometryCollection
 
 import geopandas
 from geopandas import GeoDataFrame, GeoSeries
-from geopandas._compat import PANDAS_GE_024, PANDAS_GE_025, PANDAS_GE_11
+import geopandas._compat as compat
 from geopandas.array import from_shapely
 
 from geopandas.testing import assert_geodataframe_equal, assert_geoseries_equal
 from pandas.testing import assert_frame_equal, assert_series_equal
 import pytest
 
 
@@ -35,17 +35,14 @@
 
 def test_repr(s, df):
     assert "POINT" in repr(s)
     assert "POINT" in repr(df)
     assert "POINT" in df._repr_html_()
 
 
-@pytest.mark.skipif(
-    not PANDAS_GE_024, reason="formatting for EA only implemented in 0.24.0"
-)
 def test_repr_boxed_display_precision():
     # geographic coordinates
     p1 = Point(10.123456789, 50.123456789)
     p2 = Point(4.123456789, 20.123456789)
     s1 = GeoSeries([p1, p2, None])
     assert "POINT (10.12346 50.12346)" in repr(s1)
 
@@ -70,15 +67,15 @@
     assert "None" in repr(df)
     assert "geometry" in df._repr_html_()
 
 
 def test_repr_empty():
     # https://github.com/geopandas/geopandas/issues/1195
     s = GeoSeries([])
-    if PANDAS_GE_025:
+    if compat.PANDAS_GE_025:
         # repr with correct name fixed in pandas 0.25
         assert repr(s) == "GeoSeries([], dtype: geometry)"
     else:
         assert repr(s) == "Series([], dtype: geometry)"
     df = GeoDataFrame({"a": [], "geometry": s})
     assert "Empty GeoDataFrame" in repr(df)
     # https://github.com/geopandas/geopandas/issues/1184
@@ -271,22 +268,23 @@
 
 def test_numerical_operations(s, df):
 
     # df methods ignore the geometry column
     exp = pd.Series([3, 4], index=["value1", "value2"])
     assert_series_equal(df.sum(), exp)
 
-    # series methods raise error
+    # series methods raise error (not supported for geometry)
     with pytest.raises(TypeError):
         s.sum()
 
     with pytest.raises(TypeError):
         s.max()
 
-    with pytest.raises(TypeError):
+    with pytest.raises((TypeError, ValueError)):
+        # TODO: remove ValueError after pandas-dev/pandas#32749
         s.idxmax()
 
     # numerical ops raise an error
     with pytest.raises(TypeError):
         df + 1
 
     with pytest.raises((TypeError, AssertionError)):
@@ -295,17 +293,14 @@
 
     # boolean comparisons work
     res = df == 100
     exp = pd.DataFrame(False, index=df.index, columns=df.columns)
     assert_frame_equal(res, exp)
 
 
-@pytest.mark.skipif(
-    not PANDAS_GE_024, reason="where for EA only implemented in 0.24.0 (GH24114)"
-)
 def test_where(s):
     res = s.where(np.array([True, False, True]))
     exp = GeoSeries([Point(0, 0), None, Point(2, 2)])
     assert_series_equal(res, exp)
 
 
 def test_select_dtypes(df):
@@ -456,15 +451,15 @@
     exp = pd.DataFrame({"value1": [2, 1], "value2": [1, 2]}, dtype="int64").set_index(
         "value2"
     )
     assert_frame_equal(res, exp)
 
     # applying on the geometry column
     res = df.groupby("value2")["geometry"].apply(lambda x: x.cascaded_union)
-    if PANDAS_GE_11:
+    if compat.PANDAS_GE_11:
         exp = GeoSeries(
             [shapely.geometry.MultiPoint([(0, 0), (2, 2)]), Point(1, 1)],
             index=pd.Index([1, 2], name="value2"),
             name="geometry",
         )
     else:
         exp = pd.Series(
@@ -513,7 +508,69 @@
     # subset of len 1 with loc -> bug in pandas with inconsistent Block ndim
     # resulting in bug in apply
     # https://github.com/geopandas/geopandas/issues/1078
     subset = df.loc[[0], "geometry"]
     result = subset.apply(lambda geom: geom.is_empty)
     expected = subset.is_empty
     np.testing.assert_allclose(result, expected)
+
+
+def test_apply_convert_dtypes_keyword(s):
+    # ensure the convert_dtypes keyword is accepted
+    res = s.apply(lambda x: x, convert_dtype=True, args=())
+    assert_geoseries_equal(res, s)
+
+
+@pytest.mark.parametrize("crs", [None, "EPSG:4326"])
+def test_apply_no_geometry_result(df, crs):
+    if crs:
+        df = df.set_crs(crs)
+    result = df.apply(lambda col: col.astype(str), axis=0)
+    # TODO this should actually not return a GeoDataFrame
+    assert isinstance(result, GeoDataFrame)
+    expected = df.astype(str)
+    assert_frame_equal(result, expected)
+
+    result = df.apply(lambda col: col.astype(str), axis=1)
+    assert isinstance(result, GeoDataFrame)
+    assert_frame_equal(result, expected)
+
+
+@pytest.mark.skipif(not compat.PANDAS_GE_10, reason="attrs introduced in pandas 1.0")
+def test_preserve_attrs(df):
+    # https://github.com/geopandas/geopandas/issues/1654
+    df.attrs["name"] = "my_name"
+    attrs = {"name": "my_name"}
+    assert df.attrs == attrs
+
+    # preserve attrs in indexing operations
+    for subset in [df[:2], df[df["value1"] > 2], df[["value2", "geometry"]]]:
+        assert df.attrs == attrs
+
+    # preserve attrs in methods
+    df2 = df.reset_index()
+    assert df2.attrs == attrs
+
+
+@pytest.mark.skipif(not compat.PANDAS_GE_12, reason="attrs introduced in pandas 1.0")
+def test_preserve_flags(df):
+    # https://github.com/geopandas/geopandas/issues/1654
+    df = df.set_flags(allows_duplicate_labels=False)
+    assert df.flags.allows_duplicate_labels is False
+
+    # preserve flags in indexing operations
+    for subset in [df[:2], df[df["value1"] > 2], df[["value2", "geometry"]]]:
+        assert df.flags.allows_duplicate_labels is False
+
+    # preserve attrs in methods
+    df2 = df.reset_index()
+    assert df2.flags.allows_duplicate_labels is False
+
+    # it is honored for operations that introduce duplicate labels
+    with pytest.raises(ValueError):
+        df.reindex([0, 0, 1])
+
+    with pytest.raises(ValueError):
+        df[["value1", "value1", "geometry"]]
+
+    with pytest.raises(ValueError):
+        pd.concat([df, df])
```

### Comparing `geopandas-0.8.2/geopandas/tests/test_plotting.py` & `geopandas-0.9.0/geopandas/tests/test_plotting.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from distutils.version import LooseVersion
 import itertools
 import warnings
 
 import numpy as np
 import pandas as pd
 
+from shapely import wkt
 from shapely.affinity import rotate
 from shapely.geometry import (
     MultiPolygon,
     Polygon,
     LineString,
     LinearRing,
     Point,
@@ -15,34 +17,44 @@
     MultiLineString,
     GeometryCollection,
 )
 
 
 from geopandas import GeoDataFrame, GeoSeries, read_file
 from geopandas.datasets import get_path
+import geopandas._compat as compat
 
 import pytest
 
 matplotlib = pytest.importorskip("matplotlib")
 matplotlib.use("Agg")
 import matplotlib.pyplot as plt  # noqa
 
+try:  # skipif and importorskip do not work for decorators
+    from matplotlib.testing.decorators import check_figures_equal
+
+    MPL_DECORATORS = True
+except ImportError:
+    MPL_DECORATORS = False
+
 
 @pytest.fixture(autouse=True)
 def close_figures(request):
     yield
     plt.close("all")
 
 
 try:
     cycle = matplotlib.rcParams["axes.prop_cycle"].by_key()
     MPL_DFT_COLOR = cycle["color"][0]
 except KeyError:
     MPL_DFT_COLOR = matplotlib.rcParams["axes.color_cycle"][0]
 
+plt.rcParams.update({"figure.max_open_warning": 0})
+
 
 class TestPointPlotting:
     def setup_method(self):
         self.N = 10
         self.points = GeoSeries(Point(i, i) for i in range(self.N))
 
         values = np.arange(self.N)
@@ -82,14 +94,51 @@
 
         # # with specifying values -> different colors for all 10 values
         ax = self.df.plot(column="values")
         cmap = plt.get_cmap()
         expected_colors = cmap(np.arange(self.N) / (self.N - 1))
         _check_colors(self.N, ax.collections[0].get_facecolors(), expected_colors)
 
+    def test_series_color_no_index(self):
+
+        # Color order with ordered index
+        colors_ord = pd.Series(["a", "b", "c", "a", "b", "c", "a", "b", "c", "a"])
+
+        # Plot using Series as color
+        ax1 = self.df.plot(colors_ord)
+
+        # Correct answer: Add as column to df and plot
+        self.df["colors_ord"] = colors_ord
+        ax2 = self.df.plot("colors_ord")
+
+        # Confirm out-of-order index re-sorted
+        point_colors1 = ax1.collections[0].get_facecolors()
+        point_colors2 = ax2.collections[0].get_facecolors()
+        np.testing.assert_array_equal(point_colors1[1], point_colors2[1])
+
+    def test_series_color_index(self):
+
+        # Color order with out-of-order index
+        colors_ord = pd.Series(
+            ["a", "a", "a", "a", "b", "b", "b", "c", "c", "c"],
+            index=[0, 3, 6, 9, 1, 4, 7, 2, 5, 8],
+        )
+
+        # Plot using Series as color
+        ax1 = self.df.plot(colors_ord)
+
+        # Correct answer: Add as column to df and plot
+        self.df["colors_ord"] = colors_ord
+        ax2 = self.df.plot("colors_ord")
+
+        # Confirm out-of-order index re-sorted
+        point_colors1 = ax1.collections[0].get_facecolors()
+        point_colors2 = ax2.collections[0].get_facecolors()
+        np.testing.assert_array_equal(point_colors1[1], point_colors2[1])
+
     def test_colormap(self):
 
         # without specifying values but cmap specified -> no uniform color
         # but different colors for all points
 
         # GeoSeries
         ax = self.points.plot(cmap="RdYlGn")
@@ -105,15 +154,15 @@
         cmap = plt.get_cmap("RdYlGn")
         _check_colors(self.N, ax.collections[0].get_facecolors(), exp_colors)
 
         # when using a cmap with specified lut -> limited number of different
         # colors
         ax = self.points.plot(cmap=plt.get_cmap("Set1", lut=5))
         cmap = plt.get_cmap("Set1", lut=5)
-        exp_colors = cmap(list(range(5)) * 3)
+        exp_colors = cmap(list(range(5)) * 2)
         _check_colors(self.N, ax.collections[0].get_facecolors(), exp_colors)
 
     def test_single_color(self):
 
         ax = self.points.plot(color="green")
         _check_colors(self.N, ax.collections[0].get_facecolors(), ["green"] * self.N)
 
@@ -167,16 +216,23 @@
 
         ax = self.points.plot(edgecolors="k")
         assert (ax.collections[0].get_edgecolor() == [0, 0, 0, 1]).all()
 
     def test_style_kwargs_alpha(self):
         ax = self.df.plot(alpha=0.7)
         np.testing.assert_array_equal([0.7], ax.collections[0].get_alpha())
-        with pytest.raises(TypeError):  # no list allowed for alpha
-            ax = self.df.plot(alpha=[0.7, 0.2])
+        try:
+            ax = self.df.plot(alpha=np.linspace(0, 0.0, 1.0, self.N))
+        except TypeError:
+            # no list allowed for alpha up to matplotlib 3.3
+            pass
+        else:
+            np.testing.assert_array_equal(
+                np.linspace(0, 0.0, 1.0, self.N), ax.collections[0].get_alpha()
+            )
 
     def test_legend(self):
         with warnings.catch_warnings(record=True) as _:  # don't print warning
             # legend ignored if color is given.
             ax = self.df.plot(column="values", color="green", legend=True)
             assert len(ax.get_figure().axes) == 1  # no separate legend axis
 
@@ -184,38 +240,38 @@
         ax = self.df.plot(legend=True)
         assert len(ax.get_figure().axes) == 1  # no separate legend axis
 
         # # Continuous legend
         # the colorbar matches the Point colors
         ax = self.df.plot(column="values", cmap="RdYlGn", legend=True)
         point_colors = ax.collections[0].get_facecolors()
-        cbar_colors = ax.get_figure().axes[1].collections[0].get_facecolors()
+        cbar_colors = _get_colorbar_ax(ax.get_figure()).collections[-1].get_facecolors()
         # first point == bottom of colorbar
         np.testing.assert_array_equal(point_colors[0], cbar_colors[0])
         # last point == top of colorbar
         np.testing.assert_array_equal(point_colors[-1], cbar_colors[-1])
 
         # # Categorical legend
         # the colorbar matches the Point colors
         ax = self.df.plot(column="values", categorical=True, legend=True)
         point_colors = ax.collections[0].get_facecolors()
-        cbar_colors = ax.get_legend().axes.collections[0].get_facecolors()
+        cbar_colors = ax.get_legend().axes.collections[-1].get_facecolors()
         # first point == bottom of colorbar
         np.testing.assert_array_equal(point_colors[0], cbar_colors[0])
         # last point == top of colorbar
         np.testing.assert_array_equal(point_colors[-1], cbar_colors[-1])
 
         # # Normalized legend
         # the colorbar matches the Point colors
         norm = matplotlib.colors.LogNorm(
             vmin=self.df[1:].exp.min(), vmax=self.df[1:].exp.max()
         )
         ax = self.df[1:].plot(column="exp", cmap="RdYlGn", legend=True, norm=norm)
         point_colors = ax.collections[0].get_facecolors()
-        cbar_colors = ax.get_figure().axes[1].collections[0].get_facecolors()
+        cbar_colors = _get_colorbar_ax(ax.get_figure()).collections[-1].get_facecolors()
         # first point == bottom of colorbar
         np.testing.assert_array_equal(point_colors[0], cbar_colors[0])
         # last point == top of colorbar
         np.testing.assert_array_equal(point_colors[-1], cbar_colors[-1])
         # colorbar generated proper long transition
         assert cbar_colors.shape == (256, 4)
 
@@ -229,43 +285,81 @@
         np.testing.assert_array_equal(exp_colors, actual_colors_orig)
         fig, ax = plt.subplots()
         self.df[1:].plot(column="values", ax=ax, norm=norm, cmap=cmap)
         actual_colors_sub = ax.collections[0].get_facecolors()
         np.testing.assert_array_equal(actual_colors_orig[1], actual_colors_sub[0])
 
     def test_empty_plot(self):
+
+        s = GeoSeries([Polygon()])
+        with pytest.warns(UserWarning):
+            ax = s.plot()
+        assert len(ax.collections) == 0
         s = GeoSeries([])
         with pytest.warns(UserWarning):
             ax = s.plot()
         assert len(ax.collections) == 0
         df = GeoDataFrame([])
         with pytest.warns(UserWarning):
             ax = df.plot()
         assert len(ax.collections) == 0
 
+    def test_empty_geometry(self):
+
+        if compat.USE_PYGEOS:
+            s = GeoSeries([wkt.loads("POLYGON EMPTY")])
+            s = GeoSeries(
+                [Polygon([(0, 0), (1, 0), (1, 1)]), wkt.loads("POLYGON EMPTY")]
+            )
+            ax = s.plot()
+            assert len(ax.collections) == 1
+        if not compat.USE_PYGEOS:
+            s = GeoSeries([Polygon([(0, 0), (1, 0), (1, 1)]), Polygon()])
+            ax = s.plot()
+            assert len(ax.collections) == 1
+
+        # more complex case with GEOMETRYCOLLECTION EMPTY, POINT EMPTY and NONE
+        poly = Polygon([(-1, -1), (-1, 2), (2, 2), (2, -1), (-1, -1)])
+        point = Point(0, 1)
+        point_ = Point(10, 10)
+        empty_point = Point()
+
+        gdf = GeoDataFrame(geometry=[point, empty_point, point_])
+        gdf["geometry"] = gdf.intersection(poly)
+        gdf.loc[3] = [None]
+        ax = gdf.plot()
+        assert len(ax.collections) == 1
+
     def test_multipoints(self):
 
         # MultiPoints
         ax = self.df2.plot()
         _check_colors(4, ax.collections[0].get_facecolors(), [MPL_DFT_COLOR] * 4)
 
         ax = self.df2.plot(column="values")
-        cmap = plt.get_cmap()
+        cmap = plt.get_cmap(lut=2)
         expected_colors = [cmap(0)] * self.N + [cmap(1)] * self.N
-        _check_colors(2, ax.collections[0].get_facecolors(), expected_colors)
+        _check_colors(20, ax.collections[0].get_facecolors(), expected_colors)
 
         ax = self.df2.plot(color=["r", "b"])
         # colors are repeated for all components within a MultiPolygon
-        _check_colors(2, ax.collections[0].get_facecolors(), ["r"] * 10 + ["b"] * 10)
+        _check_colors(20, ax.collections[0].get_facecolors(), ["r"] * 10 + ["b"] * 10)
 
     def test_multipoints_alpha(self):
         ax = self.df2.plot(alpha=0.7)
         np.testing.assert_array_equal([0.7], ax.collections[0].get_alpha())
-        with pytest.raises(TypeError):  # no list allowed for alpha
+        try:
             ax = self.df2.plot(alpha=[0.7, 0.2])
+        except TypeError:
+            # no list allowed for alpha up to matplotlib 3.3
+            pass
+        else:
+            np.testing.assert_array_equal(
+                [0.7] * 10 + [0.2] * 10, ax.collections[0].get_alpha()
+            )
 
     def test_categories(self):
         self.df["cats_object"] = ["cat1", "cat2"] * 5
         self.df["nums"] = [1, 2] * 5
         self.df["singlecat_object"] = ["cat2"] * 10
         self.df["cats"] = pd.Categorical(["cat1", "cat2"] * 5)
         self.df["singlecat"] = pd.Categorical(
@@ -437,16 +531,23 @@
             self.df.plot(column="values", linewidth=lw),
         ]:
             np.testing.assert_array_equal(lw, ax.collections[0].get_linewidths())
 
     def test_style_kwargs_alpha(self):
         ax = self.df.plot(alpha=0.7)
         np.testing.assert_array_equal([0.7], ax.collections[0].get_alpha())
-        with pytest.raises(TypeError):  # no list allowed for alpha
-            ax = self.df.plot(alpha=[0.7, 0.2])
+        try:
+            ax = self.df.plot(alpha=np.linspace(0, 0.0, 1.0, self.N))
+        except TypeError:
+            # no list allowed for alpha up to matplotlib 3.3
+            pass
+        else:
+            np.testing.assert_array_equal(
+                np.linspace(0, 0.0, 1.0, self.N), ax.collections[0].get_alpha()
+            )
 
     def test_subplots_norm(self):
         # colors of subplots are the same as for plot (norm is applied)
         cmap = matplotlib.cm.viridis_r
         norm = matplotlib.colors.Normalize(vmin=0, vmax=20)
         ax = self.df.plot(column="values", cmap=cmap, norm=norm)
         actual_colors_orig = ax.collections[0].get_edgecolors()
@@ -458,25 +559,25 @@
         np.testing.assert_array_equal(actual_colors_orig[1], actual_colors_sub[0])
 
     def test_multilinestrings(self):
 
         # MultiLineStrings
         ax = self.df2.plot()
         assert len(ax.collections[0].get_paths()) == 4
-        _check_colors(4, ax.collections[0].get_facecolors(), [MPL_DFT_COLOR] * 4)
+        _check_colors(4, ax.collections[0].get_edgecolors(), [MPL_DFT_COLOR] * 4)
 
         ax = self.df2.plot("values")
         cmap = plt.get_cmap(lut=2)
         # colors are repeated for all components within a MultiLineString
         expected_colors = [cmap(0), cmap(0), cmap(1), cmap(1)]
-        _check_colors(4, ax.collections[0].get_facecolors(), expected_colors)
+        _check_colors(4, ax.collections[0].get_edgecolors(), expected_colors)
 
         ax = self.df2.plot(color=["r", "b"])
         # colors are repeated for all components within a MultiLineString
-        _check_colors(4, ax.collections[0].get_facecolors(), ["r", "r", "b", "b"])
+        _check_colors(4, ax.collections[0].get_edgecolors(), ["r", "r", "b", "b"])
 
 
 class TestPolygonPlotting:
     def setup_method(self):
 
         t1 = Polygon([(0, 0), (1, 0), (1, 1)])
         t2 = Polygon([(1, 0), (2, 0), (2, 1)])
@@ -494,19 +595,19 @@
         self.df3 = self.df.append(df_nan)
 
     def test_single_color(self):
 
         ax = self.polys.plot(color="green")
         _check_colors(2, ax.collections[0].get_facecolors(), ["green"] * 2)
         # color only sets facecolor
-        _check_colors(2, ax.collections[0].get_edgecolors(), ["k"] * 2)
+        assert len(ax.collections[0].get_edgecolors()) == 0
 
         ax = self.df.plot(color="green")
         _check_colors(2, ax.collections[0].get_facecolors(), ["green"] * 2)
-        _check_colors(2, ax.collections[0].get_edgecolors(), ["k"] * 2)
+        assert len(ax.collections[0].get_edgecolors()) == 0
 
         # check rgba tuple GH1178
         ax = self.df.plot(color=(0.5, 0.5, 0.5))
         _check_colors(2, ax.collections[0].get_facecolors(), [(0.5, 0.5, 0.5)] * 2)
         ax = self.df.plot(color=(0.5, 0.5, 0.5, 0.5))
         _check_colors(2, ax.collections[0].get_facecolors(), [(0.5, 0.5, 0.5, 0.5)] * 2)
         with pytest.raises((TypeError, ValueError)):
@@ -598,16 +699,21 @@
         #   multiple
         for ax in [self.df.plot(linewidth=[2, 4]), self.df.plot(linewidths=[2, 4])]:
             np.testing.assert_array_equal([2, 4], ax.collections[0].get_linewidths())
 
         # alpha
         ax = self.df.plot(alpha=0.7)
         np.testing.assert_array_equal([0.7], ax.collections[0].get_alpha())
-        with pytest.raises(TypeError):  # no list allowed for alpha
+        try:
             ax = self.df.plot(alpha=[0.7, 0.2])
+        except TypeError:
+            # no list allowed for alpha up to matplotlib 3.3
+            pass
+        else:
+            np.testing.assert_array_equal([0.7, 0.2], ax.collections[0].get_alpha())
 
     def test_legend_kwargs(self):
 
         ax = self.df.plot(
             column="values",
             categorical=True,
             legend=True,
@@ -622,25 +728,26 @@
 
         ax = self.df.plot(
             column="values",
             categorical=False,
             legend=True,
             legend_kwds={"label": label_txt},
         )
-
-        assert ax.get_figure().axes[1].get_ylabel() == label_txt
+        cax = _get_colorbar_ax(ax.get_figure())
+        assert cax.get_ylabel() == label_txt
 
         ax = self.df.plot(
             column="values",
             categorical=False,
             legend=True,
             legend_kwds={"label": label_txt, "orientation": "horizontal"},
         )
 
-        assert ax.get_figure().axes[1].get_xlabel() == label_txt
+        cax = _get_colorbar_ax(ax.get_figure())
+        assert cax.get_xlabel() == label_txt
 
     def test_fmt_ignore(self):
         # test if fmt is removed if scheme is not passed (it would raise Error)
         # GH #1253
 
         self.df.plot(
             column="values",
@@ -696,16 +803,23 @@
             np.testing.assert_array_equal(
                 [2, 2, 4, 4], ax.collections[0].get_linewidths()
             )
 
     def test_multipolygons_alpha(self):
         ax = self.df2.plot(alpha=0.7)
         np.testing.assert_array_equal([0.7], ax.collections[0].get_alpha())
-        with pytest.raises(TypeError):  # no list allowed for alpha
+        try:
             ax = self.df2.plot(alpha=[0.7, 0.2])
+        except TypeError:
+            # no list allowed for alpha up to matplotlib 3.3
+            pass
+        else:
+            np.testing.assert_array_equal(
+                [0.7, 0.7, 0.2, 0.2], ax.collections[0].get_alpha()
+            )
 
     def test_subplots_norm(self):
         # colors of subplots are the same as for plot (norm is applied)
         cmap = matplotlib.cm.viridis_r
         norm = matplotlib.colors.Normalize(vmin=0, vmax=10)
         ax = self.df.plot(column="values", cmap=cmap, norm=norm)
         actual_colors_orig = ax.collections[0].get_facecolors()
@@ -750,25 +864,31 @@
 
         self.series = GeoSeries([coll1, coll2])
         self.df = GeoDataFrame({"geometry": self.series, "values": [1, 2]})
 
     def test_colors(self):
         # default uniform color
         ax = self.series.plot()
-        _check_colors(1, ax.collections[0].get_facecolors(), [MPL_DFT_COLOR])  # poly
-        _check_colors(2, ax.collections[1].get_edgecolors(), [MPL_DFT_COLOR])  # line
-        _check_colors(2, ax.collections[2].get_facecolors(), [MPL_DFT_COLOR])  # point
+        _check_colors(
+            2, ax.collections[0].get_facecolors(), [MPL_DFT_COLOR] * 2
+        )  # poly
+        _check_colors(
+            2, ax.collections[1].get_edgecolors(), [MPL_DFT_COLOR] * 2
+        )  # line
+        _check_colors(1, ax.collections[2].get_facecolors(), [MPL_DFT_COLOR])  # point
 
     def test_values(self):
         ax = self.df.plot("values")
         cmap = plt.get_cmap()
-        exp_colors = cmap(np.arange(2) / 1)
-        _check_colors(1, ax.collections[0].get_facecolors(), exp_colors)  # poly
-        _check_colors(2, ax.collections[1].get_edgecolors(), [exp_colors[0]])  # line
-        _check_colors(2, ax.collections[2].get_facecolors(), [exp_colors[1]])  # point
+        exp_colors = cmap([0.0, 1.0])
+        _check_colors(2, ax.collections[0].get_facecolors(), exp_colors)  # poly
+        _check_colors(
+            2, ax.collections[1].get_edgecolors(), [exp_colors[0]] * 2
+        )  # line
+        _check_colors(1, ax.collections[2].get_facecolors(), [exp_colors[1]])  # point
 
 
 class TestNonuniformGeometryPlotting:
     def setup_method(self):
         pytest.importorskip("matplotlib", "1.5.0")
 
         poly = Polygon([(1, 0), (2, 0), (2, 1)])
@@ -842,16 +962,25 @@
             np.testing.assert_array_equal(
                 [2, 4, 5.5], ax.collections[0].get_linewidths()
             )
 
     def test_style_kwargs_alpha(self):
         ax = self.df.plot(alpha=0.7)
         np.testing.assert_array_equal([0.7], ax.collections[0].get_alpha())
-        with pytest.raises(TypeError):  # no list allowed for alpha
-            ax = self.df.plot(alpha=[0.7, 0.2, 0.9])
+        # TODO splitting array-like arguments for the different plot types
+        # is not yet supported - https://github.com/geopandas/geopandas/issues/1379
+        # try:
+        #     ax = self.df.plot(alpha=[0.7, 0.2, 0.9])
+        # except TypeError:
+        #     # no list allowed for alpha up to matplotlib 3.3
+        #     pass
+        # else:
+        #     np.testing.assert_array_equal(
+        #         [0.7, 0.2, 0.9], ax.collections[0].get_alpha()
+        #     )
 
 
 class TestGeographicAspect:
     def setup_class(self):
         pth = get_path("naturalearth_lowres")
         df = read_file(pth)
         self.north = df.loc[df.continent == "North America"]
@@ -873,30 +1002,48 @@
         assert ax3.get_aspect() == self.exp
         ax4 = self.north_proj.plot("pop_est")
         assert ax4.get_aspect() in ["equal", 1.0]
 
     def test_manual(self):
         ax = self.north.geometry.plot(aspect="equal")
         assert ax.get_aspect() in ["equal", 1.0]
+        self.north.geometry.plot(ax=ax, aspect=None)
+        assert ax.get_aspect() in ["equal", 1.0]
         ax2 = self.north.geometry.plot(aspect=0.5)
         assert ax2.get_aspect() == 0.5
+        self.north.geometry.plot(ax=ax2, aspect=None)
+        assert ax2.get_aspect() == 0.5
         ax3 = self.north_proj.geometry.plot(aspect=0.5)
         assert ax3.get_aspect() == 0.5
+        self.north_proj.geometry.plot(ax=ax3, aspect=None)
+        assert ax3.get_aspect() == 0.5
         ax = self.north.plot(aspect="equal")
         assert ax.get_aspect() in ["equal", 1.0]
+        self.north.plot(ax=ax, aspect=None)
+        assert ax.get_aspect() in ["equal", 1.0]
         ax2 = self.north.plot(aspect=0.5)
         assert ax2.get_aspect() == 0.5
+        self.north.plot(ax=ax2, aspect=None)
+        assert ax2.get_aspect() == 0.5
         ax3 = self.north_proj.plot(aspect=0.5)
         assert ax3.get_aspect() == 0.5
+        self.north_proj.plot(ax=ax3, aspect=None)
+        assert ax3.get_aspect() == 0.5
         ax = self.north.plot("pop_est", aspect="equal")
         assert ax.get_aspect() in ["equal", 1.0]
+        self.north.plot("pop_est", ax=ax, aspect=None)
+        assert ax.get_aspect() in ["equal", 1.0]
         ax2 = self.north.plot("pop_est", aspect=0.5)
         assert ax2.get_aspect() == 0.5
+        self.north.plot("pop_est", ax=ax2, aspect=None)
+        assert ax2.get_aspect() == 0.5
         ax3 = self.north_proj.plot("pop_est", aspect=0.5)
         assert ax3.get_aspect() == 0.5
+        self.north_proj.plot("pop_est", ax=ax3, aspect=None)
+        assert ax3.get_aspect() == 0.5
 
 
 class TestMapclassifyPlotting:
     @classmethod
     def setup_class(cls):
         try:
             import mapclassify  # noqa
@@ -912,17 +1059,17 @@
         with warnings.catch_warnings(record=True) as _:  # don't print warning
             # warning coming from scipy.stats
             ax = self.df.plot(
                 column="pop_est", scheme="QUANTILES", k=3, cmap="OrRd", legend=True
             )
         labels = [t.get_text() for t in ax.get_legend().get_texts()]
         expected = [
-            u"[       140.00,    5217064.00]",
-            u"(   5217064.00,   19532732.33]",
-            u"(  19532732.33, 1379302771.00]",
+            u"       140.00,    5217064.00",
+            u"   5217064.00,   19532732.33",
+            u"  19532732.33, 1379302771.00",
         ]
         assert labels == expected
 
     def test_bin_labels(self):
         ax = self.df.plot(
             column="pop_est",
             scheme="QUANTILES",
@@ -947,28 +1094,41 @@
             )
 
     def test_negative_legend(self):
         ax = self.df.plot(
             column="NEGATIVES", scheme="FISHER_JENKS", k=3, cmap="OrRd", legend=True
         )
         labels = [t.get_text() for t in ax.get_legend().get_texts()]
-        expected = [u"[-10.00,  -3.41]", u"( -3.41,   3.30]", u"(  3.30,  10.00]"]
+        expected = [u"-10.00,  -3.41", u" -3.41,   3.30", u"  3.30,  10.00"]
         assert labels == expected
 
     def test_fmt(self):
         ax = self.df.plot(
             column="NEGATIVES",
             scheme="FISHER_JENKS",
             k=3,
             cmap="OrRd",
             legend=True,
             legend_kwds={"fmt": "{:.0f}"},
         )
         labels = [t.get_text() for t in ax.get_legend().get_texts()]
-        expected = [u"[-10,  -3]", u"( -3,   3]", u"(  3,  10]"]
+        expected = [u"-10,  -3", u" -3,   3", u"  3,  10"]
+        assert labels == expected
+
+    def test_interval(self):
+        ax = self.df.plot(
+            column="NEGATIVES",
+            scheme="FISHER_JENKS",
+            k=3,
+            cmap="OrRd",
+            legend=True,
+            legend_kwds={"interval": True},
+        )
+        labels = [t.get_text() for t in ax.get_legend().get_texts()]
+        expected = [u"[-10.00,  -3.41]", u"( -3.41,   3.30]", u"(  3.30,  10.00]"]
         assert labels == expected
 
     @pytest.mark.parametrize("scheme", ["FISHER_JENKS", "FISHERJENKS"])
     def test_scheme_name_compat(self, scheme):
         ax = self.df.plot(column="NEGATIVES", scheme=scheme, k=3, legend=True)
         assert len(ax.get_legend().get_texts()) == 3
 
@@ -983,15 +1143,15 @@
             scheme="percentiles",
             k=3,
             classification_kwds={"pct": [50, 100]},
             cmap="OrRd",
             legend=True,
         )
         labels = [t.get_text() for t in ax.get_legend().get_texts()]
-        expected = ["[       140.00,    9961396.00]", "(   9961396.00, 1379302771.00]"]
+        expected = ["       140.00,    9961396.00", "   9961396.00, 1379302771.00"]
         assert labels == expected
 
     def test_invalid_scheme(self):
         with pytest.raises(ValueError):
             scheme = "invalid_scheme_*#&)(*#"
             self.df.plot(
                 column="gdp_md_est", scheme=scheme, k=3, cmap="OrRd", legend=True
@@ -1013,29 +1173,29 @@
     def test_cax_legend_height(self):
         """Pass a cax argument to 'df.plot(.)', the legend location must be
         aligned with those of main plot
         """
         # base case
         with warnings.catch_warnings(record=True) as _:  # don't print warning
             ax = self.df.plot(column="pop_est", cmap="OrRd", legend=True)
-        plot_height = ax.get_figure().get_axes()[0].get_position().height
-        legend_height = ax.get_figure().get_axes()[1].get_position().height
+        plot_height = _get_ax(ax.get_figure(), "").get_position().height
+        legend_height = _get_ax(ax.get_figure(), "<colorbar>").get_position().height
         assert abs(plot_height - legend_height) >= 1e-6
         # fix heights with cax argument
-        ax2 = plt.axes()
+        fig, ax2 = plt.subplots()
         from mpl_toolkits.axes_grid1 import make_axes_locatable
 
         divider = make_axes_locatable(ax2)
-        cax = divider.append_axes("right", size="5%", pad=0.1)
+        cax = divider.append_axes("right", size="5%", pad=0.1, label="fixed_colorbar")
         with warnings.catch_warnings(record=True) as _:
             ax2 = self.df.plot(
                 column="pop_est", cmap="OrRd", legend=True, cax=cax, ax=ax2
             )
-        plot_height = ax2.get_figure().get_axes()[0].get_position().height
-        legend_height = ax2.get_figure().get_axes()[1].get_position().height
+        plot_height = _get_ax(fig, "").get_position().height
+        legend_height = _get_ax(fig, "fixed_colorbar").get_position().height
         assert abs(plot_height - legend_height) < 1e-6
 
 
 class TestPlotCollections:
     def setup_method(self):
         self.N = 3
         self.values = np.arange(self.N)
@@ -1203,31 +1363,31 @@
         _check_colors(self.N, coll.get_color(), expected_colors)
         ax.cla()
 
         # specify vmin/vmax
         coll = _plot_linestring_collection(ax, self.lines, self.values, vmin=3, vmax=5)
         fig.canvas.draw_idle()
         cmap = plt.get_cmap()
-        expected_colors = cmap([0])
-        _check_colors(self.N, coll.get_color(), expected_colors)
+        expected_colors = [cmap(0)]
+        _check_colors(self.N, coll.get_color(), expected_colors * 3)
         ax.cla()
 
     def test_polygons(self):
         from geopandas.plotting import _plot_polygon_collection, plot_polygon_collection
         from matplotlib.collections import PatchCollection
 
         fig, ax = plt.subplots()
         coll = _plot_polygon_collection(ax, self.polygons)
         assert isinstance(coll, PatchCollection)
         ax.cla()
 
         # default: single default matplotlib color
         coll = _plot_polygon_collection(ax, self.polygons)
         _check_colors(self.N, coll.get_facecolor(), [MPL_DFT_COLOR] * self.N)
-        _check_colors(self.N, coll.get_edgecolor(), ["k"] * self.N)
+        assert len(coll.get_edgecolor()) == 0
         ax.cla()
 
         # default: color sets both facecolor and edgecolor
         coll = _plot_polygon_collection(ax, self.polygons, color="g")
         _check_colors(self.N, coll.get_facecolor(), ["g"] * self.N)
         _check_colors(self.N, coll.get_edgecolor(), ["g"] * self.N)
         ax.cla()
@@ -1254,15 +1414,15 @@
             [(0.5, 0.5, 0.5, 0.5), (0.1, 0.2, 0.3, 0.5), (0.4, 0.5, 0.6, 0.5)],
         )
         ax.cla()
 
         # only setting facecolor keeps default for edgecolor
         coll = _plot_polygon_collection(ax, self.polygons, facecolor="g")
         _check_colors(self.N, coll.get_facecolor(), ["g"] * self.N)
-        _check_colors(self.N, coll.get_edgecolor(), ["k"] * self.N)
+        assert len(coll.get_edgecolor()) == 0
         ax.cla()
 
         # custom facecolor and edgecolor
         coll = _plot_polygon_collection(ax, self.polygons, facecolor="g", edgecolor="r")
         _check_colors(self.N, coll.get_facecolor(), ["g"] * self.N)
         _check_colors(self.N, coll.get_edgecolor(), ["r"] * self.N)
         ax.cla()
@@ -1297,28 +1457,103 @@
         _check_colors(self.N, coll.get_facecolor(), exp_colors)
         ax.cla()
 
         # specify vmin/vmax
         coll = _plot_polygon_collection(ax, self.polygons, self.values, vmin=3, vmax=5)
         fig.canvas.draw_idle()
         cmap = plt.get_cmap()
-        exp_colors = cmap([0])
-        _check_colors(self.N, coll.get_facecolor(), exp_colors)
+        exp_colors = [cmap(0)]
+        _check_colors(self.N, coll.get_facecolor(), exp_colors * 3)
         ax.cla()
 
         # override edgecolor
         coll = _plot_polygon_collection(ax, self.polygons, self.values, edgecolor="g")
         fig.canvas.draw_idle()
         cmap = plt.get_cmap()
         exp_colors = cmap(np.arange(self.N) / (self.N - 1))
         _check_colors(self.N, coll.get_facecolor(), exp_colors)
         _check_colors(self.N, coll.get_edgecolor(), ["g"] * self.N)
         ax.cla()
 
 
+@pytest.mark.skipif(not compat.PANDAS_GE_025, reason="requires pandas > 0.24")
+class TestGeoplotAccessor:
+    def setup_method(self):
+        geometries = [Polygon([(0, 0), (1, 0), (1, 1)]), Point(1, 3)]
+        x = [1, 2]
+        y = [10, 20]
+        self.gdf = GeoDataFrame(
+            {"geometry": geometries, "x": x, "y": y}, crs="EPSG:4326"
+        )
+        self.df = pd.DataFrame({"x": x, "y": y})
+
+    def compare_figures(self, kind, fig_test, fig_ref, kwargs):
+        """Compare Figures."""
+        ax_pandas_1 = fig_test.subplots()
+        self.df.plot(kind=kind, ax=ax_pandas_1, **kwargs)
+        ax_geopandas_1 = fig_ref.subplots()
+        self.gdf.plot(kind=kind, ax=ax_geopandas_1, **kwargs)
+
+        ax_pandas_2 = fig_test.subplots()
+        getattr(self.df.plot, kind)(ax=ax_pandas_2, **kwargs)
+        ax_geopandas_2 = fig_ref.subplots()
+        getattr(self.gdf.plot, kind)(ax=ax_geopandas_2, **kwargs)
+
+    _pandas_kinds = []
+    if compat.PANDAS_GE_025:
+        from geopandas.plotting import GeoplotAccessor
+
+        _pandas_kinds = GeoplotAccessor._pandas_kinds
+
+    if MPL_DECORATORS:
+
+        @pytest.mark.parametrize("kind", _pandas_kinds)
+        @check_figures_equal(extensions=["png", "pdf"])
+        def test_pandas_kind(self, kind, fig_test, fig_ref):
+            """Test Pandas kind."""
+            import importlib
+
+            _scipy_dependent_kinds = ["kde", "density"]  # Needs scipy
+            _y_kinds = ["pie"]  # Needs y
+            _xy_kinds = ["scatter", "hexbin"]  # Needs x & y
+            kwargs = {}
+            if kind in _scipy_dependent_kinds:
+                if not importlib.util.find_spec("scipy"):
+                    with pytest.raises(
+                        ModuleNotFoundError, match="No module named 'scipy'"
+                    ):
+                        self.gdf.plot(kind=kind)
+            elif kind in _y_kinds:
+                kwargs = {"y": "y"}
+            elif kind in _xy_kinds:
+                kwargs = {"x": "x", "y": "y"}
+
+            self.compare_figures(kind, fig_test, fig_ref, kwargs)
+            plt.close("all")
+
+        @check_figures_equal(extensions=["png", "pdf"])
+        def test_geo_kind(self, fig_test, fig_ref):
+            """Test Geo kind."""
+            ax1 = fig_test.subplots()
+            self.gdf.plot(ax=ax1)
+            ax2 = fig_ref.subplots()
+            getattr(self.gdf.plot, "geo")(ax=ax2)
+            plt.close("all")
+
+    def test_invalid_kind(self):
+        """Test invalid kinds."""
+        with pytest.raises(ValueError, match="error is not a valid plot kind"):
+            self.gdf.plot(kind="error")
+        with pytest.raises(
+            AttributeError,
+            match="'GeoplotAccessor' object has no attribute 'error'",
+        ):
+            self.gdf.plot.error()
+
+
 def test_column_values():
     """
     Check that the dataframe plot method returns same values with an
     input string (column in df), pd.Series, or np.array
     """
     # Build test data
     t1 = Polygon([(0, 0), (1, 0), (1, 1)])
@@ -1347,14 +1582,33 @@
     np.testing.assert_array_equal(colors, colors_array)
 
     # Check raised error: is df rows number equal to column legth?
     with pytest.raises(ValueError, match="different number of rows"):
         ax = df.plot(column=np.array([1, 2, 3]))
 
 
+def test_polygon_patch():
+    # test adapted from descartes by Sean Gillies
+    # (BSD license, https://pypi.org/project/descartes).
+    from geopandas.plotting import _PolygonPatch
+    from matplotlib.patches import PathPatch
+
+    polygon = (
+        Point(0, 0).buffer(10.0).difference(MultiPoint([(-5, 0), (5, 0)]).buffer(3.0))
+    )
+
+    patch = _PolygonPatch(polygon)
+    assert isinstance(patch, PathPatch)
+    path = patch.get_path()
+    if compat.GEOS_GE_390:
+        assert len(path.vertices) == len(path.codes) == 195
+    else:
+        assert len(path.vertices) == len(path.codes) == 198
+
+
 def _check_colors(N, actual_colors, expected_colors, alpha=None):
     """
     Asserts that the members of `collection` match the `expected_colors`
     (in order)
 
     Parameters
     ----------
@@ -1377,28 +1631,54 @@
 
     conv = colors.colorConverter
 
     # Convert 2D numpy array to a list of RGBA tuples.
     actual_colors = map(tuple, actual_colors)
     all_actual_colors = list(itertools.islice(itertools.cycle(actual_colors), N))
 
+    assert len(all_actual_colors) == len(expected_colors), (
+        "Different " "lengths of actual and expected colors!"
+    )
+
     for actual, expected in zip(all_actual_colors, expected_colors):
         assert actual == conv.to_rgba(expected, alpha=alpha), "{} != {}".format(
             actual, conv.to_rgba(expected, alpha=alpha)
         )
 
 
 def _style_to_linestring_onoffseq(linestyle, linewidth):
-    """ Converts a linestyle string representation, namely one of:
-            ['dashed',  'dotted', 'dashdot', 'solid'],
-        documented in `Collections.set_linestyle`,
-        to the form `onoffseq`.
+    """Converts a linestyle string representation, namely one of:
+        ['dashed',  'dotted', 'dashdot', 'solid'],
+    documented in `Collections.set_linestyle`,
+    to the form `onoffseq`.
     """
     offset, dashes = matplotlib.lines._get_dash_pattern(linestyle)
     return matplotlib.lines._scale_dashes(offset, dashes, linewidth)
 
 
 def _style_to_vertices(markerstyle):
     """ Converts a markerstyle string to a path. """
     # TODO: Vertices values are twice the actual path; unclear, why.
     path = matplotlib.markers.MarkerStyle(markerstyle).get_path()
     return path.vertices / 2
+
+
+def _get_ax(fig, label):
+    """
+    Helper function to not rely on the order of `fig.axes`.
+    Previously, we did `fig.axes[1]`, but in matplotlib 3.4 the order switched
+    and the colorbar ax was first and subplot ax second.
+    """
+    if matplotlib.__version__ < LooseVersion("3.0.0"):
+        if label == "<colorbar>":
+            return fig.axes[1]
+        elif label == "":
+            return fig.axes[0]
+    for ax in fig.axes:
+        if ax.get_label() == label:
+            return ax
+    else:
+        raise ValueError("no ax found with label {0}".format(label))
+
+
+def _get_colorbar_ax(fig):
+    return _get_ax(fig, "<colorbar>")
```

### Comparing `geopandas-0.8.2/geopandas/tests/test_show_versions.py` & `geopandas-0.9.0/geopandas/tests/test_show_versions.py`

 * *Files identical despite different names*

### Comparing `geopandas-0.8.2/geopandas/tests/test_sindex.py` & `geopandas-0.9.0/geopandas/tests/test_sindex.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,68 +8,65 @@
     GeometryCollection,
     LineString,
 )
 from numpy.testing import assert_array_equal
 
 import geopandas
 from geopandas import _compat as compat
-from geopandas import GeoDataFrame, GeoSeries, read_file, sindex, datasets
+from geopandas import GeoDataFrame, GeoSeries, read_file, datasets
 
 import pytest
 import numpy as np
 
 
-class TestNoSindex:
-    @pytest.mark.skipif(sindex.has_sindex(), reason="Spatial index present, skipping")
-    def test_no_sindex_installed(self):
-        """Checks that an error is raised when no spatial index is present."""
-        with pytest.raises(ImportError):
-            sindex.get_sindex_class()
-
-    @pytest.mark.skipif(
-        compat.HAS_RTREE or not compat.HAS_PYGEOS,
-        reason="rtree cannot be disabled via flags",
-    )
-    def test_no_sindex_active(self):
-        """Checks that an error is given when rtree is not installed
-        and compat.USE_PYGEOS is False.
-        """
-        state = compat.USE_PYGEOS  # try to save state
-        compat.set_use_pygeos(False)
-        with pytest.raises(ImportError):
-            sindex.get_sindex_class()
-        compat.set_use_pygeos(state)  # try to restore state
-
-
 @pytest.mark.skipif(sys.platform.startswith("win"), reason="fails on AppVeyor")
-@pytest.mark.skipif(not sindex.has_sindex(), reason="Spatial index absent, skipping")
+@pytest.mark.skip_no_sindex
 class TestSeriesSindex:
+    def test_has_sindex(self):
+        """Test the has_sindex method."""
+        t1 = Polygon([(0, 0), (1, 0), (1, 1)])
+        t2 = Polygon([(0, 0), (1, 1), (0, 1)])
+
+        d = GeoDataFrame({"geom": [t1, t2]}, geometry="geom")
+        assert not d.has_sindex
+        d.sindex
+        assert d.has_sindex
+        d.geometry.values._sindex = None
+        assert not d.has_sindex
+        d.sindex
+        assert d.has_sindex
+
+        s = GeoSeries([t1, t2])
+        assert not s.has_sindex
+        s.sindex
+        assert s.has_sindex
+        s.values._sindex = None
+        assert not s.has_sindex
+        s.sindex
+        assert s.has_sindex
+
     def test_empty_geoseries(self):
         """Tests creating a spatial index from an empty GeoSeries."""
-        with pytest.warns(FutureWarning, match="Generated spatial index is empty"):
-            # TODO: add checking len(GeoSeries().sindex) == 0 once deprecated
-            assert not GeoSeries(dtype=object).sindex
+        s = GeoSeries(dtype=object)
+        assert not s.sindex
+        assert len(s.sindex) == 0
 
     def test_point(self):
         s = GeoSeries([Point(0, 0)])
         assert s.sindex.size == 1
         hits = s.sindex.intersection((-1, -1, 1, 1))
         assert len(list(hits)) == 1
         hits = s.sindex.intersection((-2, -2, -1, -1))
         assert len(list(hits)) == 0
 
     def test_empty_point(self):
         """Tests that a single empty Point results in an empty tree."""
         s = GeoSeries([Point()])
-
-        with pytest.warns(FutureWarning, match="Generated spatial index is empty"):
-            # TODO: add checking len(s) == 0 once deprecated
-            assert not s.sindex
-
-        assert s._sindex_generated is True
+        assert not s.sindex
+        assert len(s.sindex) == 0
 
     def test_polygons(self):
         t1 = Polygon([(0, 0), (1, 0), (1, 1)])
         t2 = Polygon([(0, 0), (1, 1), (0, 1)])
         sq = Polygon([(0, 0), (1, 0), (1, 1), (0, 1)])
         s = GeoSeries([t1, t2, sq])
         assert s.sindex.size == 3
@@ -82,108 +79,152 @@
         t = GeoSeries([t1, t2, sq], [3, 4, 5])
         s = s.append(t)
         assert len(s) == 6
         assert s.sindex.size == 6
 
     def test_lazy_build(self):
         s = GeoSeries([Point(0, 0)])
-        assert s._sindex is None
+        assert s.values._sindex is None
         assert s.sindex.size == 1
-        assert s._sindex is not None
+        assert s.values._sindex is not None
+
+    def test_rebuild_on_item_change(self):
+        s = GeoSeries([Point(0, 0)])
+        original_index = s.sindex
+        s.iloc[0] = Point(0, 0)
+        assert s.sindex is not original_index
+
+    def test_rebuild_on_slice(self):
+        s = GeoSeries([Point(0, 0), Point(0, 0)])
+        original_index = s.sindex
+        # Select a couple of rows
+        sliced = s.iloc[:1]
+        assert sliced.sindex is not original_index
+        # Select all rows
+        sliced = s.iloc[:]
+        assert sliced.sindex is original_index
+        # Select all rows and flip
+        sliced = s.iloc[::-1]
+        assert sliced.sindex is not original_index
 
 
 @pytest.mark.skipif(sys.platform.startswith("win"), reason="fails on AppVeyor")
-@pytest.mark.skipif(not sindex.has_sindex(), reason="Spatial index absent, skipping")
+@pytest.mark.skip_no_sindex
 class TestFrameSindex:
     def setup_method(self):
         data = {
             "A": range(5),
             "B": range(-5, 0),
-            "location": [Point(x, y) for x, y in zip(range(5), range(5))],
+            "geom": [Point(x, y) for x, y in zip(range(5), range(5))],
         }
-        self.df = GeoDataFrame(data, geometry="location")
+        self.df = GeoDataFrame(data, geometry="geom")
 
     def test_sindex(self):
         self.df.crs = "epsg:4326"
         assert self.df.sindex.size == 5
-        with pytest.warns(FutureWarning, match="`objects` is deprecated"):
-            # TODO: remove warning check once deprecated
-            hits = list(self.df.sindex.intersection((2.5, 2.5, 4, 4), objects=True))
+        hits = list(self.df.sindex.intersection((2.5, 2.5, 4, 4)))
         assert len(hits) == 2
-        assert hits[0].object == 3
+        assert hits[0] == 3
 
     def test_lazy_build(self):
-        assert self.df._sindex is None
+        assert self.df.geometry.values._sindex is None
         assert self.df.sindex.size == 5
-        assert self.df._sindex is not None
+        assert self.df.geometry.values._sindex is not None
 
     def test_sindex_rebuild_on_set_geometry(self):
         # First build the sindex
         assert self.df.sindex is not None
+        original_index = self.df.sindex
         self.df.set_geometry(
             [Point(x, y) for x, y in zip(range(5, 10), range(5, 10))], inplace=True
         )
-        assert self.df._sindex_generated is False
+        assert self.df.sindex is not original_index
+
+    def test_rebuild_on_row_slice(self):
+        # Select a subset of rows rebuilds
+        original_index = self.df.sindex
+        sliced = self.df.iloc[:1]
+        assert sliced.sindex is not original_index
+        # Slicing all does not rebuild
+        original_index = self.df.sindex
+        sliced = self.df.iloc[:]
+        assert sliced.sindex is original_index
+        # Re-ordering rebuilds
+        sliced = self.df.iloc[::-1]
+        assert sliced.sindex is not original_index
+
+    def test_rebuild_on_single_col_selection(self):
+        """Selecting a single column should not rebuild the spatial index."""
+        # Selecting geometry column preserves the index
+        original_index = self.df.sindex
+        geometry_col = self.df["geom"]
+        assert geometry_col.sindex is original_index
+        geometry_col = self.df.geometry
+        assert geometry_col.sindex is original_index
+
+    @pytest.mark.skipif(
+        not compat.PANDAS_GE_10, reason="Column selection returns a copy on pd<=1.0.0"
+    )
+    def test_rebuild_on_multiple_col_selection(self):
+        """Selecting a subset of columns preserves the index."""
+        original_index = self.df.sindex
+        # Selecting a subset of columns preserves the index
+        subset1 = self.df[["geom", "A"]]
+        assert subset1.sindex is original_index
+        subset2 = self.df[["A", "geom"]]
+        assert subset2.sindex is original_index
 
 
 # Skip to accommodate Shapely geometries being unhashable
 @pytest.mark.skip
 class TestJoinSindex:
     def setup_method(self):
         nybb_filename = geopandas.datasets.get_path("nybb")
         self.boros = read_file(nybb_filename)
 
     def test_merge_geo(self):
         # First check that we gets hits from the boros frame.
         tree = self.boros.sindex
-        with pytest.warns(FutureWarning, match="`objects` is deprecated"):
-            # TODO: remove warning check once deprecated
-            hits = tree.intersection((1012821.80, 229228.26), objects=True)
-        res = [self.boros.loc[hit.object]["BoroName"] for hit in hits]
+        hits = tree.intersection((1012821.80, 229228.26))
+        res = [self.boros.iloc[hit]["BoroName"] for hit in hits]
         assert res == ["Bronx", "Queens"]
 
         # Check that we only get the Bronx from this view.
         first = self.boros[self.boros["BoroCode"] < 3]
         tree = first.sindex
-        with pytest.warns(FutureWarning, match="`objects` is deprecated"):
-            # TODO: remove warning check once deprecated
-            hits = tree.intersection((1012821.80, 229228.26), objects=True)
-        res = [first.loc[hit.object]["BoroName"] for hit in hits]
+        hits = tree.intersection((1012821.80, 229228.26))
+        res = [first.iloc[hit]["BoroName"] for hit in hits]
         assert res == ["Bronx"]
 
         # Check that we only get Queens from this view.
         second = self.boros[self.boros["BoroCode"] >= 3]
         tree = second.sindex
-        with pytest.warns(FutureWarning, match="`objects` is deprecated"):
-            # TODO: remove warning check once deprecated
-            hits = tree.intersection((1012821.80, 229228.26), objects=True)
-        res = ([second.loc[hit.object]["BoroName"] for hit in hits],)
+        hits = tree.intersection((1012821.80, 229228.26))
+        res = ([second.iloc[hit]["BoroName"] for hit in hits],)
         assert res == ["Queens"]
 
         # Get both the Bronx and Queens again.
         merged = first.merge(second, how="outer")
         assert len(merged) == 5
         assert merged.sindex.size == 5
         tree = merged.sindex
-        with pytest.warns(FutureWarning, match="`objects` is deprecated"):
-            # TODO: remove warning check once deprecated
-            hits = tree.intersection((1012821.80, 229228.26), objects=True)
-        res = [merged.loc[hit.object]["BoroName"] for hit in hits]
+        hits = tree.intersection((1012821.80, 229228.26))
+        res = [merged.iloc[hit]["BoroName"] for hit in hits]
         assert res == ["Bronx", "Queens"]
 
 
-@pytest.mark.skipif(not sindex.has_sindex(), reason="Spatial index absent, skipping")
+@pytest.mark.skip_no_sindex
 class TestPygeosInterface:
     def setup_method(self):
         data = {
-            "location": [Point(x, y) for x, y in zip(range(5), range(5))]
+            "geom": [Point(x, y) for x, y in zip(range(5), range(5))]
             + [box(10, 10, 20, 20)]  # include a box geometry
         }
-        self.df = GeoDataFrame(data, geometry="location")
-        self.expected_size = len(data["location"])
+        self.df = GeoDataFrame(data, geometry="geom")
+        self.expected_size = len(data["geom"])
 
     # --------------------------- `intersection` tests -------------------------- #
     @pytest.mark.parametrize(
         "test_geom, expected",
         (
             ((-1, -1, -0.5, -0.5), []),
             ((-0.5, -0.5, 0.5, 0.5), [0]),
@@ -252,46 +293,93 @@
             ),  # intersects but not contains
             ("touches", box(-1, -1, 0, 0), [0]),  # bbox intersects and touches
             (
                 "touches",
                 box(-0.5, -0.5, 1.5, 1.5),
                 [],
             ),  # bbox intersects but geom does not touch
+            (
+                "contains",
+                box(10, 10, 20, 20),
+                [5],
+            ),  # contains but does not contains_properly
+            (
+                "covers",
+                box(-0.5, -0.5, 1, 1),
+                [0, 1],
+            ),  # covers (0, 0) and (1, 1)
+            (
+                "covers",
+                box(0.001, 0.001, 0.99, 0.99),
+                [],
+            ),  # does not cover any
+            (
+                "covers",
+                box(0, 0, 1, 1),
+                [0, 1],
+            ),  # covers but does not contain
+            (
+                "contains_properly",
+                box(0, 0, 1, 1),
+                [],
+            ),  # intersects but does not contain
+            (
+                "contains_properly",
+                box(0, 0, 1.001, 1.001),
+                [1],
+            ),  # intersects 2 and contains 1
+            (
+                "contains_properly",
+                box(0.5, 0.5, 1.001, 1.001),
+                [1],
+            ),  # intersects 1 and contains 1
+            (
+                "contains_properly",
+                box(0.5, 0.5, 1.5, 1.5),
+                [1],
+            ),  # intersects and contains
+            (
+                "contains_properly",
+                box(-1, -1, 2, 2),
+                [0, 1],
+            ),  # intersects and contains multiple
+            (
+                "contains_properly",
+                box(10, 10, 20, 20),
+                [],
+            ),  # contains but does not contains_properly
         ),
     )
     def test_query(self, predicate, test_geom, expected):
         """Tests the `query` method with valid inputs and valid predicates."""
         res = self.df.sindex.query(test_geom, predicate=predicate)
         assert_array_equal(res, expected)
 
     def test_query_invalid_geometry(self):
-        """Tests the `query` method with invalid geometry.
-        """
+        """Tests the `query` method with invalid geometry."""
         with pytest.raises(TypeError):
             self.df.sindex.query("notavalidgeom")
 
     @pytest.mark.parametrize(
         "test_geom, expected_value",
         [
             (None, []),
             (GeometryCollection(), []),
             (Point(), []),
             (MultiPolygon(), []),
             (Polygon(), []),
         ],
     )
     def test_query_empty_geometry(self, test_geom, expected_value):
-        """Tests the `query` method with empty geometry.
-        """
+        """Tests the `query` method with empty geometry."""
         res = self.df.sindex.query(test_geom)
         assert_array_equal(res, expected_value)
 
     def test_query_invalid_predicate(self):
-        """Tests the `query` method with invalid predicates.
-        """
+        """Tests the `query` method with invalid predicates."""
         test_geom = box(-1, -1, -0.5, -0.5)
         with pytest.raises(ValueError):
             self.df.sindex.query(test_geom, predicate="test")
 
     @pytest.mark.parametrize(
         "sort, expected",
         (
@@ -320,18 +408,22 @@
         # pass through GeoSeries to have GeoPandas
         # determine if it should use shapely or pygeos geometry objects
         tree_df = geopandas.GeoDataFrame(geometry=tree_polys)
         test_df = geopandas.GeoDataFrame(geometry=test_polys)
 
         test_geo = test_df.geometry.values.data[0]
         res = tree_df.sindex.query(test_geo, sort=sort)
+
+        # asserting the same elements
+        assert sorted(res) == sorted(expected)
+        # asserting the exact array can fail if sort=False
         try:
             assert_array_equal(res, expected)
         except AssertionError as e:
-            if not compat.USE_PYGEOS and sort is False:
+            if sort is False:
                 pytest.xfail(
                     "rtree results are known to be unordered, see "
                     "https://github.com/geopandas/geopandas/issues/1337\n"
                     "Expected:\n {}\n".format(expected)
                     + "Got:\n {}\n".format(res.tolist())
                 )
             raise e
@@ -353,15 +445,19 @@
                 "intersects",
                 [(-1, -1, 1, 1), (-0.5, -0.5, 0.5, 0.5)],
                 [[0, 0, 1], [0, 1, 0]],
             ),
             ("within", [(0.25, 0.28, 0.75, 0.75)], [[], []]),  # does not intersect
             ("within", [(0, 0, 10, 10)], [[], []]),  # intersects but is not within
             ("within", [(11, 11, 12, 12)], [[0], [5]]),  # intersects and is within
-            ("contains", [(0, 0, 1, 1)], [[], []]),  # intersects but does not contain
+            (
+                "contains",
+                [(0, 0, 1, 1)],
+                [[], []],
+            ),  # intersects and covers, but does not contain
             (
                 "contains",
                 [(0, 0, 1.001, 1.001)],
                 [[0], [1]],
             ),  # intersects 2 and contains 1
             (
                 "contains",
@@ -370,14 +466,70 @@
             ),  # intersects 1 and contains 1
             ("contains", [(0.5, 0.5, 1.5, 1.5)], [[0], [1]]),  # intersects and contains
             (
                 "contains",
                 [(-1, -1, 2, 2)],
                 [[0, 0], [0, 1]],
             ),  # intersects and contains multiple
+            (
+                "contains",
+                [(10, 10, 20, 20)],
+                [[0], [5]],
+            ),  # contains but does not contains_properly
+            ("touches", [(-1, -1, 0, 0)], [[0], [0]]),  # bbox intersects and touches
+            (
+                "touches",
+                [(-0.5, -0.5, 1.5, 1.5)],
+                [[], []],
+            ),  # bbox intersects but geom does not touch
+            (
+                "covers",
+                [(-0.5, -0.5, 1, 1)],
+                [[0, 0], [0, 1]],
+            ),  # covers (0, 0) and (1, 1)
+            (
+                "covers",
+                [(0.001, 0.001, 0.99, 0.99)],
+                [[], []],
+            ),  # does not cover any
+            (
+                "covers",
+                [(0, 0, 1, 1)],
+                [[0, 0], [0, 1]],
+            ),  # covers but does not contain
+            (
+                "contains_properly",
+                [(0, 0, 1, 1)],
+                [[], []],
+            ),  # intersects but does not contain
+            (
+                "contains_properly",
+                [(0, 0, 1.001, 1.001)],
+                [[0], [1]],
+            ),  # intersects 2 and contains 1
+            (
+                "contains_properly",
+                [(0.5, 0.5, 1.001, 1.001)],
+                [[0], [1]],
+            ),  # intersects 1 and contains 1
+            (
+                "contains_properly",
+                [(0.5, 0.5, 1.5, 1.5)],
+                [[0], [1]],
+            ),  # intersects and contains
+            (
+                "contains_properly",
+                [(-1, -1, 2, 2)],
+                [[0, 0], [0, 1]],
+            ),  # intersects and contains multiple
+            (
+                "contains_properly",
+                [(10, 10, 20, 20)],
+                [[], []],
+            ),  # contains but does not contains_properly
         ),
     )
     def test_query_bulk(self, predicate, test_geom, expected):
         """Tests the `query_bulk` method with valid
         inputs and valid predicates.
         """
         # pass through GeoSeries to have GeoPandas
@@ -396,41 +548,39 @@
             # None should be skipped
             ([GeometryCollection(), None], [[], []]),
             ([None], [[], []]),
             ([None, box(-0.5, -0.5, 0.5, 0.5), None], [[1], [0]]),
         ],
     )
     def test_query_bulk_empty_geometry(self, test_geoms, expected_value):
-        """Tests the `query_bulk` method with an empty geometry.
-        """
+        """Tests the `query_bulk` method with an empty geometry."""
         # pass through GeoSeries to have GeoPandas
         # determine if it should use shapely or pygeos geometry objects
         # note: for this test, test_geoms (note plural) is a list already
         test_geoms = geopandas.GeoSeries(test_geoms, index=range(len(test_geoms)))
         res = self.df.sindex.query_bulk(test_geoms)
         assert_array_equal(res, expected_value)
 
     def test_query_bulk_empty_input_array(self):
-        """Tests the `query_bulk` method with an empty input array.
-        """
+        """Tests the `query_bulk` method with an empty input array."""
         test_array = np.array([], dtype=object)
         expected_value = [[], []]
         res = self.df.sindex.query_bulk(test_array)
         assert_array_equal(res, expected_value)
 
     def test_query_bulk_invalid_input_geometry(self):
-        """Tests the `query_bulk` method with invalid input for the `geometry` parameter.
+        """
+        Tests the `query_bulk` method with invalid input for the `geometry` parameter.
         """
         test_array = "notanarray"
         with pytest.raises(TypeError):
             self.df.sindex.query_bulk(test_array)
 
     def test_query_bulk_invalid_predicate(self):
-        """Tests the `query_bulk` method with invalid predicates.
-        """
+        """Tests the `query_bulk` method with invalid predicates."""
         test_geom_bounds = (-1, -1, -0.5, -0.5)
         test_predicate = "test"
 
         # pass through GeoSeries to have GeoPandas
         # determine if it should use shapely or pygeos geometry objects
         test_geom = geopandas.GeoSeries([box(*test_geom_bounds)], index=["0"])
 
@@ -499,31 +649,35 @@
 
         # pass through GeoSeries to have GeoPandas
         # determine if it should use shapely or pygeos geometry objects
         tree_df = geopandas.GeoDataFrame(geometry=tree_polys)
         test_df = geopandas.GeoDataFrame(geometry=test_polys)
 
         res = tree_df.sindex.query_bulk(test_df.geometry, sort=sort)
+
+        # asserting the same elements
+        assert sorted(res[0]) == sorted(expected[0])
+        assert sorted(res[1]) == sorted(expected[1])
+        # asserting the exact array can fail if sort=False
         try:
             assert_array_equal(res, expected)
         except AssertionError as e:
-            if not compat.USE_PYGEOS and sort is False:
+            if sort is False:
                 pytest.xfail(
                     "rtree results are known to be unordered, see "
                     "https://github.com/geopandas/geopandas/issues/1337\n"
                     "Expected:\n {}\n".format(expected)
                     + "Got:\n {}\n".format(res.tolist())
                 )
             raise e
 
     # --------------------------- misc tests ---------------------------- #
 
     def test_empty_tree_geometries(self):
-        """Tests building sindex with interleaved empty geometries.
-        """
+        """Tests building sindex with interleaved empty geometries."""
         geoms = [Point(0, 0), None, Point(), Point(1, 1), Point()]
         df = geopandas.GeoDataFrame(geometry=geoms)
         assert df.sindex.query(Point(1, 1))[0] == 3
 
     def test_size(self):
         """Tests the `size` property."""
         assert self.df.sindex.size == self.expected_size
@@ -531,22 +685,23 @@
     def test_len(self):
         """Tests the `__len__` method of spatial indexes."""
         assert len(self.df.sindex) == self.expected_size
 
     def test_is_empty(self):
         """Tests the `is_empty` property."""
         # create empty tree
-        cls_ = sindex.get_sindex_class()
-        empty = geopandas.GeoSeries(dtype=object)
-        tree = cls_(empty)
-        assert tree.is_empty
+        empty = geopandas.GeoSeries([], dtype=object)
+        assert empty.sindex.is_empty
+        empty = geopandas.GeoSeries([None])
+        assert empty.sindex.is_empty
+        empty = geopandas.GeoSeries([Point()])
+        assert empty.sindex.is_empty
         # create a non-empty tree
         non_empty = geopandas.GeoSeries([Point(0, 0)])
-        tree = cls_(non_empty)
-        assert not tree.is_empty
+        assert not non_empty.sindex.is_empty
 
     @pytest.mark.parametrize(
         "predicate, expected_shape",
         [
             (None, (2, 396)),
             ("intersects", (2, 172)),
             ("within", (2, 172)),
@@ -559,7 +714,20 @@
     def test_integration_natural_earth(self, predicate, expected_shape):
         """Tests output sizes for the naturalearth datasets."""
         world = read_file(datasets.get_path("naturalearth_lowres"))
         capitals = read_file(datasets.get_path("naturalearth_cities"))
 
         res = world.sindex.query_bulk(capitals.geometry, predicate)
         assert res.shape == expected_shape
+
+
+@pytest.mark.skipif(not compat.HAS_RTREE, reason="no rtree installed")
+def test_old_spatial_index_deprecated():
+    t1 = Polygon([(0, 0), (1, 0), (1, 1)])
+    t2 = Polygon([(0, 0), (1, 1), (0, 1)])
+
+    stream = ((i, item.bounds, None) for i, item in enumerate([t1, t2]))
+
+    with pytest.warns(FutureWarning):
+        idx = geopandas.sindex.SpatialIndex(stream)
+
+    assert list(idx.intersection((0, 0, 1, 1))) == [0, 1]
```

### Comparing `geopandas-0.8.2/geopandas/tests/test_testing.py` & `geopandas-0.9.0/geopandas/tests/test_testing.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,14 +42,22 @@
 df1 = GeoDataFrame({"col1": [1, 2], "geometry": s1})
 df2 = GeoDataFrame({"col1": [1, 2], "geometry": s2})
 
 s4 = s1.copy()
 s4.crs = 4326
 s5 = s2.copy()
 s5.crs = 27700
+
+s6 = GeoSeries(
+    [
+        Polygon([(0, 3), (0, 0), (2, 0), (2, 2)]),
+        Polygon([(2, 2), (4, 2), (4, 4), (2, 4)]),
+    ]
+)
+
 df4 = GeoDataFrame(
     {"col1": [1, 2], "geometry": s1.copy(), "geom2": s4.copy(), "geom3": s5.copy()},
     crs=3857,
 )
 df5 = GeoDataFrame(
     {"col1": [1, 2], "geometry": s1.copy(), "geom3": s5.copy(), "geom2": s4.copy()},
     crs=3857,
@@ -59,16 +67,23 @@
 @pytest.mark.filterwarnings("ignore::UserWarning")
 def test_geoseries():
     assert_geoseries_equal(s1, s2)
     assert_geoseries_equal(s1, s3, check_series_type=False, check_dtype=False)
     assert_geoseries_equal(s3, s2, check_series_type=False, check_dtype=False)
     assert_geoseries_equal(s1, s4, check_series_type=False)
 
-    with pytest.raises(AssertionError):
+    with pytest.raises(AssertionError) as error:
         assert_geoseries_equal(s1, s2, check_less_precise=True)
+    assert "1 out of 2 geometries are not almost equal" in str(error.value)
+    assert "not almost equal: [0]" in str(error.value)
+
+    with pytest.raises(AssertionError) as error:
+        assert_geoseries_equal(s2, s6, check_less_precise=False)
+    assert "1 out of 2 geometries are not equal" in str(error.value)
+    assert "not equal: [0]" in str(error.value)
 
 
 def test_geodataframe():
     assert_geodataframe_equal(df1, df2)
 
     with pytest.raises(AssertionError):
         assert_geodataframe_equal(df1, df2, check_less_precise=True)
```

### Comparing `geopandas-0.8.2/geopandas/tests/test_types.py` & `geopandas-0.9.0/geopandas/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `geopandas-0.8.2/geopandas/tests/util.py` & `geopandas-0.9.0/geopandas/tests/util.py`

 * *Files identical despite different names*

### Comparing `geopandas-0.8.2/geopandas/tools/_show_versions.py` & `geopandas-0.9.0/geopandas/tools/_show_versions.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,15 @@
         "pyproj",
         "matplotlib",
         "mapclassify",
         "geopy",
         "psycopg2",
         "geoalchemy2",
         "pyarrow",
+        "pygeos",
     ]
 
     def get_version(module):
         return module.__version__
 
     deps_info = {}
```

### Comparing `geopandas-0.8.2/geopandas/tools/clip.py` & `geopandas-0.9.0/geopandas/tools/clip.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         that intersects with poly.
     """
     gdf_sub = gdf.iloc[gdf.sindex.query(poly, predicate="intersects")]
 
     # Clip the data with the polygon
     if isinstance(gdf_sub, GeoDataFrame):
         clipped = gdf_sub.copy()
-        clipped["geometry"] = gdf_sub.intersection(poly)
+        clipped[gdf.geometry.name] = gdf_sub.intersection(poly)
     else:
         # GeoSeries
         clipped = gdf_sub.intersection(poly)
 
     return clipped
 
 
@@ -102,36 +102,35 @@
          Vector data (points, lines, polygons) from `gdf` clipped to
          polygon boundary from mask.
 
     Examples
     --------
     Clip points (global cities) with a polygon (the South American continent):
 
-    >>> import geopandas
-    >>> path =
     >>> world = geopandas.read_file(
     ...     geopandas.datasets.get_path('naturalearth_lowres'))
     >>> south_america = world[world['continent'] == "South America"]
     >>> capitals = geopandas.read_file(
     ...     geopandas.datasets.get_path('naturalearth_cities'))
     >>> capitals.shape
     (202, 2)
+
     >>> sa_capitals = geopandas.clip(capitals, south_america)
     >>> sa_capitals.shape
     (12, 2)
     """
     if not isinstance(gdf, (GeoDataFrame, GeoSeries)):
         raise TypeError(
             "'gdf' should be GeoDataFrame or GeoSeries, got {}".format(type(gdf))
         )
 
     if not isinstance(mask, (GeoDataFrame, GeoSeries, Polygon, MultiPolygon)):
         raise TypeError(
             "'mask' should be GeoDataFrame, GeoSeries or"
-            "(Multi)Polygon, got {}".format(type(gdf))
+            "(Multi)Polygon, got {}".format(type(mask))
         )
 
     if isinstance(mask, (GeoDataFrame, GeoSeries)):
         if not _check_crs(gdf, mask):
             _crs_mismatch_warn(gdf, mask, stacklevel=3)
 
     if isinstance(mask, (GeoDataFrame, GeoSeries)):
```

### Comparing `geopandas-0.8.2/geopandas/tools/crs.py` & `geopandas-0.9.0/geopandas/tools/crs.py`

 * *Files identical despite different names*

### Comparing `geopandas-0.8.2/geopandas/tools/geocoding.py` & `geopandas-0.9.0/geopandas/tools/geocoding.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from collections import defaultdict
 import time
 
-import numpy as np
 import pandas as pd
 
 from shapely.geometry import Point
 
 import geopandas
 
 
@@ -49,22 +48,21 @@
     your provider.
 
     Geocoding requires geopy. Install it using 'pip install geopy'. See also
     https://github.com/geopy/geopy
 
     Examples
     --------
-    >>> df = geocode(['boston, ma', '1600 pennsylvania ave. washington, dc'])
-    >>> df
-                                                 address  \\
-    0                                    Boston, MA, USA
-    1  1600 Pennsylvania Avenue Northwest, President'...
-                             geometry
-    0  POINT (-71.0597732 42.3584308)
-    1  POINT (-77.0365305 38.8977332)
+    >>> df = geopandas.tools.geocode(  # doctest: +SKIP
+    ...         ["boston, ma", "1600 pennsylvania ave. washington, dc"]
+    ...     )
+    >>> df  # doctest: +SKIP
+                        geometry                                            address
+    0  POINT (-71.05863 42.35899)                          Boston, MA, United States
+    1  POINT (-77.03651 38.89766)  1600 Pennsylvania Ave NW, Washington, DC 20006...
     """
 
     if provider is None:
         # https://geocode.farm/geocoding/free-api-documentation/
         provider = "geocodefarm"
         throttle_time = 0.25
     else:
@@ -104,23 +102,22 @@
     your provider.
 
     Reverse geocoding requires geopy. Install it using 'pip install geopy'.
     See also https://github.com/geopy/geopy
 
     Examples
     --------
-    >>> df = reverse_geocode([Point(-71.0594869, 42.3584697),
-                              Point(-77.0365305, 38.8977332)])
-    >>> df
-                                             address  \\
-    0             29 Court Square, Boston, MA 02108, USA
-    1  1600 Pennsylvania Avenue Northwest, President'...
-                             geometry
-    0  POINT (-71.0594869 42.3584697)
-    1  POINT (-77.0365305 38.8977332)
+    >>> from shapely.geometry import Point
+    >>> df = geopandas.tools.reverse_geocode(  # doctest: +SKIP
+    ...     [Point(-71.0594869, 42.3584697), Point(-77.0365305, 38.8977332)]
+    ... )
+    >>> df  # doctest: +SKIP
+                         geometry                                            address
+    0  POINT (-71.05941 42.35837)       29 Court Sq, Boston, MA 02108, United States
+    1  POINT (-77.03641 38.89766)  1600 Pennsylvania Ave NW, Washington, DC 20006...
     """
 
     if provider is None:
         # https://geocode.farm/geocoding/free-api-documentation/
         provider = "geocodefarm"
         throttle_time = 0.25
     else:
@@ -165,24 +162,27 @@
 
     """
     # Prepare the data for the DataFrame as a dict of lists
     d = defaultdict(list)
     index = []
 
     for i, s in results.items():
-        address, loc = s
 
-        # loc is lat, lon and we want lon, lat
-        if loc is None:
+        if s is None:
             p = Point()
+            address = None
+
         else:
-            p = Point(loc[1], loc[0])
+            address, loc = s
 
-        if address is None:
-            address = np.nan
+            # loc is lat, lon and we want lon, lat
+            if loc is None:
+                p = Point()
+            else:
+                p = Point(loc[1], loc[0])
 
         d["geometry"].append(p)
         d["address"].append(address)
         index.append(i)
 
     df = geopandas.GeoDataFrame(d, index=index, crs="EPSG:4326")
```

### Comparing `geopandas-0.8.2/geopandas/tools/tests/test_clip.py` & `geopandas-0.9.0/geopandas/tools/tests/test_clip.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 import geopandas
 from geopandas import GeoDataFrame, GeoSeries, clip
 
 from geopandas.testing import assert_geodataframe_equal, assert_geoseries_equal
 import pytest
 
 
-pytestmark = pytest.mark.skipif(
-    not geopandas.sindex.has_sindex(), reason="clip requires spatial index"
-)
+pytestmark = pytest.mark.skip_no_sindex
 
 
 @pytest.fixture
 def point_gdf():
     """Create a point GeoDataFrame."""
     pts = np.array([[2, 2], [3, 4], [9, 8], [-12, -15]])
     gdf = GeoDataFrame([Point(xy) for xy in pts], columns=["geometry"], crs="EPSG:4326")
@@ -199,21 +197,45 @@
     """Test clipping a points GDF with a generic polygon geometry."""
     clip_pts = clip(point_gdf, single_rectangle_gdf)
     pts = np.array([[2, 2], [3, 4], [9, 8]])
     exp = GeoDataFrame([Point(xy) for xy in pts], columns=["geometry"], crs="EPSG:4326")
     assert_geodataframe_equal(clip_pts, exp)
 
 
+def test_clip_points_geom_col_rename(point_gdf, single_rectangle_gdf):
+    """Test clipping a points GDF with a generic polygon geometry."""
+    point_gdf_geom_col_rename = point_gdf.rename_geometry("geometry2")
+    clip_pts = clip(point_gdf_geom_col_rename, single_rectangle_gdf)
+    pts = np.array([[2, 2], [3, 4], [9, 8]])
+    exp = GeoDataFrame(
+        [Point(xy) for xy in pts],
+        columns=["geometry2"],
+        crs="EPSG:4326",
+        geometry="geometry2",
+    )
+    assert_geodataframe_equal(clip_pts, exp)
+
+
 def test_clip_poly(buffered_locations, single_rectangle_gdf):
     """Test clipping a polygon GDF with a generic polygon geometry."""
     clipped_poly = clip(buffered_locations, single_rectangle_gdf)
     assert len(clipped_poly.geometry) == 3
     assert all(clipped_poly.geom_type == "Polygon")
 
 
+def test_clip_poly_geom_col_rename(buffered_locations, single_rectangle_gdf):
+    """Test clipping a polygon GDF with a generic polygon geometry."""
+
+    poly_gdf_geom_col_rename = buffered_locations.rename_geometry("geometry2")
+    clipped_poly = clip(poly_gdf_geom_col_rename, single_rectangle_gdf)
+    assert len(clipped_poly.geometry) == 3
+    assert "geometry" not in clipped_poly.keys()
+    assert "geometry2" in clipped_poly.keys()
+
+
 def test_clip_poly_series(buffered_locations, single_rectangle_gdf):
     """Test clipping a polygon GDF with a generic polygon geometry."""
     clipped_poly = clip(buffered_locations.geometry, single_rectangle_gdf)
     assert len(clipped_poly) == 3
     assert all(clipped_poly.geom_type == "Polygon")
```

### Comparing `geopandas-0.8.2/geopandas/tools/tests/test_tools.py` & `geopandas-0.9.0/geopandas/tools/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `geopandas-0.8.2/geopandas/tools/util.py` & `geopandas-0.9.0/geopandas/tools/util.py`

 * *Files identical despite different names*

### Comparing `geopandas-0.8.2/geopandas.egg-info/PKG-INFO` & `geopandas-0.9.0/geopandas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: geopandas
-Version: 0.8.2
+Version: 0.9.0
 Summary: Geographic pandas extensions
 Home-page: http://geopandas.org
 Author: GeoPandas contributors
 Author-email: kjordahl@alum.mit.edu
 License: BSD
 Description: GeoPandas is a project to add support for geographic data to
         `pandas`_ objects.
@@ -16,8 +16,8 @@
         operations in python that would otherwise require a spatial database
         such as PostGIS.
         
         .. _pandas: http://pandas.pydata.org
         .. _shapely: http://shapely.readthedocs.io/en/latest/
         
 Platform: UNKNOWN
-Requires-Python: >=3.5
+Requires-Python: >=3.6
```

### Comparing `geopandas-0.8.2/geopandas.egg-info/SOURCES.txt` & `geopandas-0.9.0/geopandas.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 geopandas/__init__.py
 geopandas/_compat.py
 geopandas/_config.py
 geopandas/_vectorized.py
 geopandas/_version.py
 geopandas/array.py
 geopandas/base.py
+geopandas/conftest.py
 geopandas/geodataframe.py
 geopandas/geoseries.py
 geopandas/plotting.py
 geopandas/sindex.py
 geopandas/testing.py
 geopandas.egg-info/PKG-INFO
 geopandas.egg-info/SOURCES.txt
@@ -58,14 +59,15 @@
 geopandas/tests/test_pandas_methods.py
 geopandas/tests/test_plotting.py
 geopandas/tests/test_show_versions.py
 geopandas/tests/test_sindex.py
 geopandas/tests/test_testing.py
 geopandas/tests/test_types.py
 geopandas/tests/util.py
+geopandas/tests/data/null_geom.geojson
 geopandas/tools/__init__.py
 geopandas/tools/_show_versions.py
 geopandas/tools/clip.py
 geopandas/tools/crs.py
 geopandas/tools/geocoding.py
 geopandas/tools/overlay.py
 geopandas/tools/sjoin.py
```

### Comparing `geopandas-0.8.2/setup.cfg` & `geopandas-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `geopandas-0.8.2/setup.py` & `geopandas-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,20 @@
 .. _pandas: http://pandas.pydata.org
 .. _shapely: http://shapely.readthedocs.io/en/latest/
 """
 
 if os.environ.get("READTHEDOCS", False) == "True":
     INSTALL_REQUIRES = []
 else:
-    INSTALL_REQUIRES = ["pandas >= 0.23.0", "shapely", "fiona", "pyproj >= 2.2.0"]
+    INSTALL_REQUIRES = [
+        "pandas >= 0.24.0",
+        "shapely >= 1.6",
+        "fiona >= 1.8",
+        "pyproj >= 2.2.0",
+    ]
 
 # get all data dirs in the datasets module
 data_files = []
 
 for item in os.listdir("geopandas/datasets"):
     if not item.startswith("__"):
         if os.path.isdir(os.path.join("geopandas/datasets/", item)):
@@ -58,11 +63,11 @@
         "geopandas.io",
         "geopandas.tools",
         "geopandas.datasets",
         "geopandas.tests",
         "geopandas.tools.tests",
     ],
     package_data={"geopandas": data_files},
-    python_requires=">=3.5",
+    python_requires=">=3.6",
     install_requires=INSTALL_REQUIRES,
     cmdclass=versioneer.get_cmdclass(),
 )
```

### Comparing `geopandas-0.8.2/versioneer.py` & `geopandas-0.9.0/versioneer.py`

 * *Files identical despite different names*

