# Comparing `tmp/neuron-image-denoise-0.0.1.tar.gz` & `tmp/neuron-image-denoise-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuron-image-denoise-0.0.1.tar", last modified: Mon Jun  5 16:33:06 2023, max compression
+gzip compressed data, was "neuron-image-denoise-0.0.2.tar", last modified: Tue Jun  6 10:17:25 2023, max compression
```

## Comparing `neuron-image-denoise-0.0.1.tar` & `neuron-image-denoise-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 16:33:06.819250 neuron-image-denoise-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-06-05 16:33:06.775855 neuron-image-denoise-0.0.1/.github/
--rw-rw-rw-   0        0        0        6 2023-06-04 10:12:59.000000 neuron-image-denoise-0.0.1/.github/python-version.txt
-drwxrwxrwx   0        0        0        0 2023-06-05 16:33:06.776851 neuron-image-denoise-0.0.1/.github/workflows/
--rw-rw-rw-   0        0        0     1451 2023-06-04 10:12:59.000000 neuron-image-denoise-0.0.1/.github/workflows/static.yml
--rw-rw-rw-   0        0        0     3252 2023-06-04 10:26:02.000000 neuron-image-denoise-0.0.1/.gitignore
--rw-rw-rw-   0        0        0     1096 2023-06-03 10:23:41.000000 neuron-image-denoise-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       22 2023-06-04 10:06:59.000000 neuron-image-denoise-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2565 2023-06-05 16:33:06.819250 neuron-image-denoise-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1882 2023-06-05 16:29:08.000000 neuron-image-denoise-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 16:33:06.810307 neuron-image-denoise-0.0.1/neuron_image_denoise/
--rw-rw-rw-   0        0        0      219 2023-06-05 16:25:08.000000 neuron-image-denoise-0.0.1/neuron_image_denoise/__init__.py
--rw-rw-rw-   0        0        0     3272 2023-06-05 16:25:08.000000 neuron-image-denoise-0.0.1/neuron_image_denoise/_filter.pyx
--rw-rw-rw-   0        0        0     2041 2023-06-05 16:25:08.000000 neuron-image-denoise-0.0.1/neuron_image_denoise/filter.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:33:06.817257 neuron-image-denoise-0.0.1/neuron_image_denoise.egg-info/
--rw-rw-rw-   0        0        0     2565 2023-06-05 16:33:06.000000 neuron-image-denoise-0.0.1/neuron_image_denoise.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      436 2023-06-05 16:33:06.000000 neuron-image-denoise-0.0.1/neuron_image_denoise.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 16:33:06.000000 neuron-image-denoise-0.0.1/neuron_image_denoise.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-05 16:33:06.000000 neuron-image-denoise-0.0.1/neuron_image_denoise.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-05 16:33:06.000000 neuron-image-denoise-0.0.1/neuron_image_denoise.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      926 2023-06-04 09:59:33.000000 neuron-image-denoise-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-05 16:33:06.820249 neuron-image-denoise-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      437 2023-06-04 10:22:19.000000 neuron-image-denoise-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:17:25.366533 neuron-image-denoise-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-06-06 10:17:25.336611 neuron-image-denoise-0.0.2/.github/
+-rw-rw-rw-   0        0        0        6 2023-06-04 10:12:59.000000 neuron-image-denoise-0.0.2/.github/python-version.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 10:17:25.338606 neuron-image-denoise-0.0.2/.github/workflows/
+-rw-rw-rw-   0        0        0     1451 2023-06-04 10:12:59.000000 neuron-image-denoise-0.0.2/.github/workflows/static.yml
+-rw-rw-rw-   0        0        0     3258 2023-06-06 05:03:03.000000 neuron-image-denoise-0.0.2/.gitignore
+-rw-rw-rw-   0        0        0     1096 2023-06-03 10:23:41.000000 neuron-image-denoise-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       22 2023-06-04 10:06:59.000000 neuron-image-denoise-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2612 2023-06-06 10:17:25.365534 neuron-image-denoise-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1929 2023-06-06 10:08:32.000000 neuron-image-denoise-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 10:17:25.354564 neuron-image-denoise-0.0.2/neuron_image_denoise/
+-rw-rw-rw-   0        0        0      219 2023-06-05 16:25:08.000000 neuron-image-denoise-0.0.2/neuron_image_denoise/__init__.py
+-rw-rw-rw-   0        0        0     3272 2023-06-06 10:06:27.000000 neuron-image-denoise-0.0.2/neuron_image_denoise/_filter.pyx
+-rw-rw-rw-   0        0        0     2887 2023-06-06 10:15:01.000000 neuron-image-denoise-0.0.2/neuron_image_denoise/filter.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:17:25.362542 neuron-image-denoise-0.0.2/neuron_image_denoise.egg-info/
+-rw-rw-rw-   0        0        0     2612 2023-06-06 10:17:25.000000 neuron-image-denoise-0.0.2/neuron_image_denoise.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-06-06 10:17:25.000000 neuron-image-denoise-0.0.2/neuron_image_denoise.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 10:17:25.000000 neuron-image-denoise-0.0.2/neuron_image_denoise.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-06 10:17:25.000000 neuron-image-denoise-0.0.2/neuron_image_denoise.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-06 10:17:25.000000 neuron-image-denoise-0.0.2/neuron_image_denoise.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      947 2023-06-06 08:02:29.000000 neuron-image-denoise-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-06 10:17:25.366533 neuron-image-denoise-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      437 2023-06-04 10:22:19.000000 neuron-image-denoise-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:17:25.364535 neuron-image-denoise-0.0.2/test/
+-rw-rw-rw-   0        0        0      271 2023-06-06 10:13:29.000000 neuron-image-denoise-0.0.2/test/case1.py
```

### Comparing `neuron-image-denoise-0.0.1/.github/workflows/static.yml` & `neuron-image-denoise-0.0.2/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `neuron-image-denoise-0.0.1/.gitignore` & `neuron-image-denoise-0.0.2/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -156,7 +156,8 @@
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 .idea/
 *.html
 *.cpp
+data
```

### Comparing `neuron-image-denoise-0.0.1/LICENSE` & `neuron-image-denoise-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `neuron-image-denoise-0.0.1/PKG-INFO` & `neuron-image-denoise-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuron-image-denoise
-Version: 0.0.1
+Version: 0.0.2
 Summary: Fluorescent neuron image denoising tools
 Author-email: Zuohan Zhao <zzhmark@126.com>
 License: MIT License
 Project-URL: GitHub Project, https://github.com/SEU-ALLEN-codebase/neuron-image-denoise-py
 Project-URL: Documentation, https://SEU-ALLEN-codebase.github.io/neuron-image-denoise-py
 Keywords: vaa3d,neuron-morphology,image-processing
 Classifier: Programming Language :: Python :: 3
@@ -40,14 +40,16 @@
     'flare_x':True, 
     'flare_y': True
 }
 
 out = adaptive_denoise(img, **params)
 
 out = adaptive_denoise_16to8(img, **params)   # 16bit to 8bit
+
+out = gauss_attenuation_filter(img, 32, .1)
 ```
 
 ## Algorithm Explanation
 
 Neurons are illuminated by the fluorescent proteins, which can be seen as dots in the space. Measuring the signal is to 
 locate where the dots are, but the problem is, these dots can diffuse to outside of neurons and their light can be
 spreaded far away due to refraction and microcopy aberration.
```

### Comparing `neuron-image-denoise-0.0.1/README.md` & `neuron-image-denoise-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     'flare_x':True, 
     'flare_y': True
 }
 
 out = adaptive_denoise(img, **params)
 
 out = adaptive_denoise_16to8(img, **params)   # 16bit to 8bit
+
+out = gauss_attenuation_filter(img, 32, .1)
 ```
 
 ## Algorithm Explanation
 
 Neurons are illuminated by the fluorescent proteins, which can be seen as dots in the space. Measuring the signal is to 
 locate where the dots are, but the problem is, these dots can diffuse to outside of neurons and their light can be
 spreaded far away due to refraction and microcopy aberration.
```

### Comparing `neuron-image-denoise-0.0.1/neuron_image_denoise/_filter.pyx` & `neuron-image-denoise-0.0.2/neuron_image_denoise/_filter.pyx`

 * *Files identical despite different names*

### Comparing `neuron-image-denoise-0.0.1/neuron_image_denoise.egg-info/PKG-INFO` & `neuron-image-denoise-0.0.2/neuron_image_denoise.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuron-image-denoise
-Version: 0.0.1
+Version: 0.0.2
 Summary: Fluorescent neuron image denoising tools
 Author-email: Zuohan Zhao <zzhmark@126.com>
 License: MIT License
 Project-URL: GitHub Project, https://github.com/SEU-ALLEN-codebase/neuron-image-denoise-py
 Project-URL: Documentation, https://SEU-ALLEN-codebase.github.io/neuron-image-denoise-py
 Keywords: vaa3d,neuron-morphology,image-processing
 Classifier: Programming Language :: Python :: 3
@@ -40,14 +40,16 @@
     'flare_x':True, 
     'flare_y': True
 }
 
 out = adaptive_denoise(img, **params)
 
 out = adaptive_denoise_16to8(img, **params)   # 16bit to 8bit
+
+out = gauss_attenuation_filter(img, 32, .1)
 ```
 
 ## Algorithm Explanation
 
 Neurons are illuminated by the fluorescent proteins, which can be seen as dots in the space. Measuring the signal is to 
 locate where the dots are, but the problem is, these dots can diffuse to outside of neurons and their light can be
 spreaded far away due to refraction and microcopy aberration.
```

### Comparing `neuron-image-denoise-0.0.1/pyproject.toml` & `neuron-image-denoise-0.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 dynamic = [ "version" ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
-    "numpy"
+    "numpy",
+    "scikit-image"
 ]
 
 [project.urls]
 "GitHub Project" = "https://github.com/SEU-ALLEN-codebase/neuron-image-denoise-py"
 "Documentation" = "https://SEU-ALLEN-codebase.github.io/neuron-image-denoise-py"
 
 [project.optional-dependencies]
```

