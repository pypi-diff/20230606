# Comparing `tmp/Image_filtering-0.0.1.tar.gz` & `tmp/Image_filtering-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Image_filtering-0.0.1.tar", last modified: Mon Jun  5 12:31:15 2023, max compression
+gzip compressed data, was "Image_filtering-0.0.2.tar", last modified: Tue Jun  6 05:51:08 2023, max compression
```

## Comparing `Image_filtering-0.0.1.tar` & `Image_filtering-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 12:31:15.057313 Image_filtering-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-06-05 12:31:15.041689 Image_filtering-0.0.1/Image_filtering.egg-info/
--rw-rw-rw-   0        0        0      163 2023-06-05 12:31:14.000000 Image_filtering-0.0.1/Image_filtering.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2023-06-05 12:31:14.000000 Image_filtering-0.0.1/Image_filtering.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 12:31:14.000000 Image_filtering-0.0.1/Image_filtering.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-05 12:31:14.000000 Image_filtering-0.0.1/Image_filtering.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      163 2023-06-05 12:31:15.057313 Image_filtering-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-05 12:31:15.041689 Image_filtering-0.0.1/noise_filter/
--rw-rw-rw-   0        0        0     7106 2023-06-05 05:46:56.000000 Image_filtering-0.0.1/noise_filter/PIL_filter.py
--rw-rw-rw-   0        0        0     1665 2023-06-05 02:47:07.000000 Image_filtering-0.0.1/noise_filter/__init__.py
--rw-rw-rw-   0        0        0     3900 2023-06-05 02:34:59.000000 Image_filtering-0.0.1/noise_filter/opencv_filter.py
--rw-rw-rw-   0        0        0     2795 2023-06-05 02:58:51.000000 Image_filtering-0.0.1/noise_filter/skimage_filter.py
--rw-rw-rw-   0        0        0       42 2023-06-05 12:31:15.057313 Image_filtering-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      288 2023-06-05 12:31:08.000000 Image_filtering-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:51:08.555725 Image_filtering-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-06-06 05:51:08.540102 Image_filtering-0.0.2/Image_filtering.egg-info/
+-rw-rw-rw-   0        0        0      163 2023-06-06 05:51:08.000000 Image_filtering-0.0.2/Image_filtering.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2023-06-06 05:51:08.000000 Image_filtering-0.0.2/Image_filtering.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 05:51:08.000000 Image_filtering-0.0.2/Image_filtering.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-06 05:51:08.000000 Image_filtering-0.0.2/Image_filtering.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      163 2023-06-06 05:51:08.555725 Image_filtering-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-06 05:51:08.540102 Image_filtering-0.0.2/noise_filter/
+-rw-rw-rw-   0        0        0     7106 2023-06-05 05:46:56.000000 Image_filtering-0.0.2/noise_filter/PIL_filter.py
+-rw-rw-rw-   0        0        0     1665 2023-06-05 02:47:07.000000 Image_filtering-0.0.2/noise_filter/__init__.py
+-rw-rw-rw-   0        0        0     3900 2023-06-05 02:34:59.000000 Image_filtering-0.0.2/noise_filter/opencv_filter.py
+-rw-rw-rw-   0        0        0     2795 2023-06-05 02:58:51.000000 Image_filtering-0.0.2/noise_filter/skimage_filter.py
+-rw-rw-rw-   0        0        0       42 2023-06-06 05:51:08.555725 Image_filtering-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      288 2023-06-06 05:49:54.000000 Image_filtering-0.0.2/setup.py
```

### Comparing `Image_filtering-0.0.1/noise_filter/PIL_filter.py` & `Image_filtering-0.0.2/noise_filter/PIL_filter.py`

 * *Files identical despite different names*

### Comparing `Image_filtering-0.0.1/noise_filter/__init__.py` & `Image_filtering-0.0.2/noise_filter/__init__.py`

 * *Files identical despite different names*

### Comparing `Image_filtering-0.0.1/noise_filter/opencv_filter.py` & `Image_filtering-0.0.2/noise_filter/opencv_filter.py`

 * *Files identical despite different names*

### Comparing `Image_filtering-0.0.1/noise_filter/skimage_filter.py` & `Image_filtering-0.0.2/noise_filter/skimage_filter.py`

 * *Files identical despite different names*

