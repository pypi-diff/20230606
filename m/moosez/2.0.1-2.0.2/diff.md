# Comparing `tmp/moosez-2.0.1.tar.gz` & `tmp/moosez-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moosez-2.0.1.tar", last modified: Tue Jun  6 15:56:28 2023, max compression
+gzip compressed data, was "moosez-2.0.2.tar", last modified: Tue Jun  6 16:03:40 2023, max compression
```

## Comparing `moosez-2.0.1.tar` & `moosez-2.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 lalithsimac   (501) staff       (20)        0 2023-06-06 15:56:28.567098 moosez-2.0.1/
--rw-r--r--   0 lalithsimac   (501) staff       (20)    11357 2023-06-06 13:31:59.000000 moosez-2.0.1/LICENSE
--rw-r--r--   0 lalithsimac   (501) staff       (20)     1404 2023-06-06 15:56:28.566692 moosez-2.0.1/PKG-INFO
--rw-r--r--   0 lalithsimac   (501) staff       (20)    19071 2023-06-06 13:31:59.000000 moosez-2.0.1/README.md
-drwxr-xr-x   0 lalithsimac   (501) staff       (20)        0 2023-06-06 15:56:28.563859 moosez-2.0.1/moosez/
--rw-r--r--   0 lalithsimac   (501) staff       (20)      227 2023-06-06 13:31:59.000000 moosez-2.0.1/moosez/__init__.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     1362 2023-06-06 13:31:59.000000 moosez-2.0.1/moosez/constants.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     7161 2023-06-06 13:31:59.000000 moosez-2.0.1/moosez/display.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     3662 2023-06-06 13:31:59.000000 moosez-2.0.1/moosez/download.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     4119 2023-06-06 13:31:59.000000 moosez-2.0.1/moosez/file_utilities.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     4002 2023-06-06 13:31:59.000000 moosez-2.0.1/moosez/image_conversion.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     3416 2023-06-06 15:07:22.000000 moosez-2.0.1/moosez/image_processing.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     4163 2023-06-06 13:31:59.000000 moosez-2.0.1/moosez/input_validation.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     7781 2023-06-06 15:53:20.000000 moosez-2.0.1/moosez/moosez.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     5974 2023-06-06 13:31:59.000000 moosez-2.0.1/moosez/predict.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     3090 2023-06-06 13:31:59.000000 moosez-2.0.1/moosez/resources.py
-drwxr-xr-x   0 lalithsimac   (501) staff       (20)        0 2023-06-06 15:56:28.566188 moosez-2.0.1/moosez.egg-info/
--rw-r--r--   0 lalithsimac   (501) staff       (20)     1404 2023-06-06 15:56:28.000000 moosez-2.0.1/moosez.egg-info/PKG-INFO
--rw-r--r--   0 lalithsimac   (501) staff       (20)      445 2023-06-06 15:56:28.000000 moosez-2.0.1/moosez.egg-info/SOURCES.txt
--rw-r--r--   0 lalithsimac   (501) staff       (20)        1 2023-06-06 15:56:28.000000 moosez-2.0.1/moosez.egg-info/dependency_links.txt
--rw-r--r--   0 lalithsimac   (501) staff       (20)       47 2023-06-06 15:56:28.000000 moosez-2.0.1/moosez.egg-info/entry_points.txt
--rw-r--r--   0 lalithsimac   (501) staff       (20)      234 2023-06-06 15:56:28.000000 moosez-2.0.1/moosez.egg-info/requires.txt
--rw-r--r--   0 lalithsimac   (501) staff       (20)        7 2023-06-06 15:56:28.000000 moosez-2.0.1/moosez.egg-info/top_level.txt
--rw-r--r--   0 lalithsimac   (501) staff       (20)       38 2023-06-06 15:56:28.567244 moosez-2.0.1/setup.cfg
--rw-r--r--   0 lalithsimac   (501) staff       (20)     2178 2023-06-06 15:55:40.000000 moosez-2.0.1/setup.py
+drwxr-xr-x   0 lalithsimac   (501) staff       (20)        0 2023-06-06 16:03:40.591980 moosez-2.0.2/
+-rw-r--r--   0 lalithsimac   (501) staff       (20)    11357 2023-06-06 13:31:59.000000 moosez-2.0.2/LICENSE
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     1404 2023-06-06 16:03:40.591772 moosez-2.0.2/PKG-INFO
+-rw-r--r--   0 lalithsimac   (501) staff       (20)    19071 2023-06-06 13:31:59.000000 moosez-2.0.2/README.md
+drwxr-xr-x   0 lalithsimac   (501) staff       (20)        0 2023-06-06 16:03:40.590163 moosez-2.0.2/moosez/
+-rw-r--r--   0 lalithsimac   (501) staff       (20)      227 2023-06-06 13:31:59.000000 moosez-2.0.2/moosez/__init__.py
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     1362 2023-06-06 13:31:59.000000 moosez-2.0.2/moosez/constants.py
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     7161 2023-06-06 13:31:59.000000 moosez-2.0.2/moosez/display.py
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     3662 2023-06-06 13:31:59.000000 moosez-2.0.2/moosez/download.py
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     4119 2023-06-06 13:31:59.000000 moosez-2.0.2/moosez/file_utilities.py
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     4002 2023-06-06 13:31:59.000000 moosez-2.0.2/moosez/image_conversion.py
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     3416 2023-06-06 15:07:22.000000 moosez-2.0.2/moosez/image_processing.py
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     4163 2023-06-06 13:31:59.000000 moosez-2.0.2/moosez/input_validation.py
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     7781 2023-06-06 15:53:20.000000 moosez-2.0.2/moosez/moosez.py
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     5974 2023-06-06 13:31:59.000000 moosez-2.0.2/moosez/predict.py
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     3090 2023-06-06 13:31:59.000000 moosez-2.0.2/moosez/resources.py
+drwxr-xr-x   0 lalithsimac   (501) staff       (20)        0 2023-06-06 16:03:40.591475 moosez-2.0.2/moosez.egg-info/
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     1404 2023-06-06 16:03:40.000000 moosez-2.0.2/moosez.egg-info/PKG-INFO
+-rw-r--r--   0 lalithsimac   (501) staff       (20)      445 2023-06-06 16:03:40.000000 moosez-2.0.2/moosez.egg-info/SOURCES.txt
+-rw-r--r--   0 lalithsimac   (501) staff       (20)        1 2023-06-06 16:03:40.000000 moosez-2.0.2/moosez.egg-info/dependency_links.txt
+-rw-r--r--   0 lalithsimac   (501) staff       (20)       47 2023-06-06 16:03:40.000000 moosez-2.0.2/moosez.egg-info/entry_points.txt
+-rw-r--r--   0 lalithsimac   (501) staff       (20)      234 2023-06-06 16:03:40.000000 moosez-2.0.2/moosez.egg-info/requires.txt
+-rw-r--r--   0 lalithsimac   (501) staff       (20)        7 2023-06-06 16:03:40.000000 moosez-2.0.2/moosez.egg-info/top_level.txt
+-rw-r--r--   0 lalithsimac   (501) staff       (20)       38 2023-06-06 16:03:40.592056 moosez-2.0.2/setup.cfg
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     2178 2023-06-06 16:03:09.000000 moosez-2.0.2/setup.py
```

### Comparing `moosez-2.0.1/LICENSE` & `moosez-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `moosez-2.0.1/PKG-INFO` & `moosez-2.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.0.1
+Version: 2.0.2
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Platform: UNKNOWN
```

### Comparing `moosez-2.0.1/README.md` & `moosez-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `moosez-2.0.1/moosez/constants.py` & `moosez-2.0.2/moosez/constants.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.1/moosez/display.py` & `moosez-2.0.2/moosez/display.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.1/moosez/download.py` & `moosez-2.0.2/moosez/download.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.1/moosez/file_utilities.py` & `moosez-2.0.2/moosez/file_utilities.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.1/moosez/image_conversion.py` & `moosez-2.0.2/moosez/image_conversion.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.1/moosez/image_processing.py` & `moosez-2.0.2/moosez/image_processing.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.1/moosez/input_validation.py` & `moosez-2.0.2/moosez/input_validation.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.1/moosez/moosez.py` & `moosez-2.0.2/moosez/moosez.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.1/moosez/predict.py` & `moosez-2.0.2/moosez/predict.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.1/moosez/resources.py` & `moosez-2.0.2/moosez/resources.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.1/moosez.egg-info/PKG-INFO` & `moosez-2.0.2/moosez.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.0.1
+Version: 2.0.2
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Platform: UNKNOWN
```

### Comparing `moosez-2.0.1/setup.py` & `moosez-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='moosez',
-    version='2.0.1',
+    version='2.0.2',
     author='Lalith Kumar Shiyam Sundar',
     author_email='Lalith.shiyamsundar@meduniwien.ac.at',
     description='An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks',
     long_description='mooseZ is an AI-inference engine based on nnUNet, designed for 3D clinical and preclinical'
                      ' whole-body segmentation tasks. It serves models tailored towards different modalities such'
                      ' as PET, CT, and MR. mooseZ provides fast and accurate segmentation results, making it a '
                      'reliable tool for medical imaging applications.',
```

