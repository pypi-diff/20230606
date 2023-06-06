# Comparing `tmp/moosez-2.0.0.tar.gz` & `tmp/moosez-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moosez-2.0.0.tar", last modified: Tue Jun  6 13:44:26 2023, max compression
+gzip compressed data, was "moosez-2.0.1.tar", last modified: Tue Jun  6 15:56:28 2023, max compression
```

## Comparing `moosez-2.0.0.tar` & `moosez-2.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 lalithsimac   (501) staff       (20)        0 2023-06-06 13:44:26.106353 moosez-2.0.0/
--rw-r--r--   0 lalithsimac   (501) staff       (20)    11357 2023-06-06 13:31:59.000000 moosez-2.0.0/LICENSE
--rw-r--r--   0 lalithsimac   (501) staff       (20)     1404 2023-06-06 13:44:26.105924 moosez-2.0.0/PKG-INFO
--rw-r--r--   0 lalithsimac   (501) staff       (20)    19071 2023-06-06 13:31:59.000000 moosez-2.0.0/README.md
-drwxr-xr-x   0 lalithsimac   (501) staff       (20)        0 2023-06-06 13:44:26.102499 moosez-2.0.0/moosez/
--rw-r--r--   0 lalithsimac   (501) staff       (20)      227 2023-06-06 13:31:59.000000 moosez-2.0.0/moosez/__init__.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     1362 2023-06-06 13:31:59.000000 moosez-2.0.0/moosez/constants.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     7161 2023-06-06 13:31:59.000000 moosez-2.0.0/moosez/display.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     3662 2023-06-06 13:31:59.000000 moosez-2.0.0/moosez/download.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     4119 2023-06-06 13:31:59.000000 moosez-2.0.0/moosez/file_utilities.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     4002 2023-06-06 13:31:59.000000 moosez-2.0.0/moosez/image_conversion.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     3414 2023-06-06 13:31:59.000000 moosez-2.0.0/moosez/image_processing.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     4163 2023-06-06 13:31:59.000000 moosez-2.0.0/moosez/input_validation.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     7744 2023-06-06 13:31:59.000000 moosez-2.0.0/moosez/moosez.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     5974 2023-06-06 13:31:59.000000 moosez-2.0.0/moosez/predict.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     3090 2023-06-06 13:31:59.000000 moosez-2.0.0/moosez/resources.py
-drwxr-xr-x   0 lalithsimac   (501) staff       (20)        0 2023-06-06 13:44:26.105317 moosez-2.0.0/moosez.egg-info/
--rw-r--r--   0 lalithsimac   (501) staff       (20)     1404 2023-06-06 13:44:26.000000 moosez-2.0.0/moosez.egg-info/PKG-INFO
--rw-r--r--   0 lalithsimac   (501) staff       (20)      445 2023-06-06 13:44:26.000000 moosez-2.0.0/moosez.egg-info/SOURCES.txt
--rw-r--r--   0 lalithsimac   (501) staff       (20)        1 2023-06-06 13:44:26.000000 moosez-2.0.0/moosez.egg-info/dependency_links.txt
--rw-r--r--   0 lalithsimac   (501) staff       (20)       47 2023-06-06 13:44:26.000000 moosez-2.0.0/moosez.egg-info/entry_points.txt
--rw-r--r--   0 lalithsimac   (501) staff       (20)      218 2023-06-06 13:44:26.000000 moosez-2.0.0/moosez.egg-info/requires.txt
--rw-r--r--   0 lalithsimac   (501) staff       (20)        7 2023-06-06 13:44:26.000000 moosez-2.0.0/moosez.egg-info/top_level.txt
--rw-r--r--   0 lalithsimac   (501) staff       (20)       38 2023-06-06 13:44:26.106636 moosez-2.0.0/setup.cfg
--rw-r--r--   0 lalithsimac   (501) staff       (20)     2151 2023-06-06 13:44:21.000000 moosez-2.0.0/setup.py
+drwxr-xr-x   0 lalithsimac   (501) staff       (20)        0 2023-06-06 15:56:28.567098 moosez-2.0.1/
+-rw-r--r--   0 lalithsimac   (501) staff       (20)    11357 2023-06-06 13:31:59.000000 moosez-2.0.1/LICENSE
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     1404 2023-06-06 15:56:28.566692 moosez-2.0.1/PKG-INFO
+-rw-r--r--   0 lalithsimac   (501) staff       (20)    19071 2023-06-06 13:31:59.000000 moosez-2.0.1/README.md
+drwxr-xr-x   0 lalithsimac   (501) staff       (20)        0 2023-06-06 15:56:28.563859 moosez-2.0.1/moosez/
+-rw-r--r--   0 lalithsimac   (501) staff       (20)      227 2023-06-06 13:31:59.000000 moosez-2.0.1/moosez/__init__.py
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     1362 2023-06-06 13:31:59.000000 moosez-2.0.1/moosez/constants.py
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     7161 2023-06-06 13:31:59.000000 moosez-2.0.1/moosez/display.py
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     3662 2023-06-06 13:31:59.000000 moosez-2.0.1/moosez/download.py
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     4119 2023-06-06 13:31:59.000000 moosez-2.0.1/moosez/file_utilities.py
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     4002 2023-06-06 13:31:59.000000 moosez-2.0.1/moosez/image_conversion.py
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     3416 2023-06-06 15:07:22.000000 moosez-2.0.1/moosez/image_processing.py
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     4163 2023-06-06 13:31:59.000000 moosez-2.0.1/moosez/input_validation.py
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     7781 2023-06-06 15:53:20.000000 moosez-2.0.1/moosez/moosez.py
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     5974 2023-06-06 13:31:59.000000 moosez-2.0.1/moosez/predict.py
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     3090 2023-06-06 13:31:59.000000 moosez-2.0.1/moosez/resources.py
+drwxr-xr-x   0 lalithsimac   (501) staff       (20)        0 2023-06-06 15:56:28.566188 moosez-2.0.1/moosez.egg-info/
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     1404 2023-06-06 15:56:28.000000 moosez-2.0.1/moosez.egg-info/PKG-INFO
+-rw-r--r--   0 lalithsimac   (501) staff       (20)      445 2023-06-06 15:56:28.000000 moosez-2.0.1/moosez.egg-info/SOURCES.txt
+-rw-r--r--   0 lalithsimac   (501) staff       (20)        1 2023-06-06 15:56:28.000000 moosez-2.0.1/moosez.egg-info/dependency_links.txt
+-rw-r--r--   0 lalithsimac   (501) staff       (20)       47 2023-06-06 15:56:28.000000 moosez-2.0.1/moosez.egg-info/entry_points.txt
+-rw-r--r--   0 lalithsimac   (501) staff       (20)      234 2023-06-06 15:56:28.000000 moosez-2.0.1/moosez.egg-info/requires.txt
+-rw-r--r--   0 lalithsimac   (501) staff       (20)        7 2023-06-06 15:56:28.000000 moosez-2.0.1/moosez.egg-info/top_level.txt
+-rw-r--r--   0 lalithsimac   (501) staff       (20)       38 2023-06-06 15:56:28.567244 moosez-2.0.1/setup.cfg
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     2178 2023-06-06 15:55:40.000000 moosez-2.0.1/setup.py
```

### Comparing `moosez-2.0.0/LICENSE` & `moosez-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `moosez-2.0.0/PKG-INFO` & `moosez-2.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.0.0
+Version: 2.0.1
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Platform: UNKNOWN
```

### Comparing `moosez-2.0.0/README.md` & `moosez-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `moosez-2.0.0/moosez/constants.py` & `moosez-2.0.1/moosez/constants.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.0/moosez/display.py` & `moosez-2.0.1/moosez/display.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.0/moosez/download.py` & `moosez-2.0.1/moosez/download.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.0/moosez/file_utilities.py` & `moosez-2.0.1/moosez/file_utilities.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.0/moosez/image_conversion.py` & `moosez-2.0.1/moosez/image_conversion.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.0/moosez/image_processing.py` & `moosez-2.0.1/moosez/image_processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     sitk_input_image.SetSpacing([spacing.item() for spacing in original_spacing])
     axis_flip_matrix = np.diag([-1, -1, 1])
     sitk_input_image.SetOrigin(np.dot(axis_flip_matrix, translation_vector))
     sitk_input_image.SetDirection((np.dot(axis_flip_matrix, rotation_matrix) / np.absolute(original_spacing)).ravel())
 
     # Resample the image to the desired spacing
     desired_spacing = np.array(desired_spacing)
-    new_size = [int(original_size[i] * (original_spacing[i] / desired_spacing[i])) for i in range(len(original_size))]
+    new_size = [round(original_size[i] * (original_spacing[i] / desired_spacing[i])) for i in range(len(original_size))]
     resampled_sitk_image = SimpleITK.Resample(sitk_input_image, new_size, SimpleITK.Transform(), interpolation_method,
                                               sitk_input_image.GetOrigin(), desired_spacing.tolist(),
                                               sitk_input_image.GetDirection(), 0.0, sitk_input_image.GetPixelIDValue())
 
     # Save the resampled image to disk
     SimpleITK.WriteImage(resampled_sitk_image, output_image_path)
```

### Comparing `moosez-2.0.0/moosez/input_validation.py` & `moosez-2.0.1/moosez/input_validation.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.0/moosez/moosez.py` & `moosez-2.0.1/moosez/moosez.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,21 +27,24 @@
 from moosez import input_validation
 from moosez import predict
 from moosez import constants
 from moosez import image_conversion
 from threading import Thread
 import tqdm
 import time
+import colorama
 
 logging.basicConfig(format='%(asctime)s %(levelname)-8s [%(filename)s:%(lineno)d] %(message)s', level=logging.INFO,
                     filename=datetime.now().strftime('moosez-v.2.0.0.%H-%M-%d-%m-%Y.log'),
                     filemode='w')
 
 
 def main():
+    colorama.init()
+
     parser = argparse.ArgumentParser()
 
     parser.add_argument("-d", "--main_directory", type=str, help="Main directory containing subject folders",
                         required=True)
 
     parser.add_argument("-m", "--model_name", type=str, help="Name of the model to use for segmentation",
                         choices=["clin_ct_bones",
```

### Comparing `moosez-2.0.0/moosez/predict.py` & `moosez-2.0.1/moosez/predict.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.0/moosez/resources.py` & `moosez-2.0.1/moosez/resources.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.0/moosez.egg-info/PKG-INFO` & `moosez-2.0.1/moosez.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.0.0
+Version: 2.0.1
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Platform: UNKNOWN
```

### Comparing `moosez-2.0.0/setup.py` & `moosez-2.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='moosez',
-    version='2.0.0',
+    version='2.0.1',
     author='Lalith Kumar Shiyam Sundar',
     author_email='Lalith.shiyamsundar@meduniwien.ac.at',
     description='An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks',
     long_description='mooseZ is an AI-inference engine based on nnUNet, designed for 3D clinical and preclinical'
                      ' whole-body segmentation tasks. It serves models tailored towards different modalities such'
                      ' as PET, CT, and MR. mooseZ provides fast and accurate segmentation results, making it a '
                      'reliable tool for medical imaging applications.',
@@ -41,15 +41,16 @@
         'imageio~=2.16.1',
         'numpy~=1.22.3',
         'mpire~=2.3.3',
         'openpyxl~=3.0.9',
         'matplotlib',
         'pyfiglet~=0.8.post1',
         'natsort~=8.1.0',
-        'pillow>=9.2.0'
+        'pillow>=9.2.0',
+        'colorama~=0.4.6'
     ],
     entry_points={
         'console_scripts': [
             'moosez=moosez.moosez:main',
         ],
     },
 )
```

