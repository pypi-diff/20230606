# Comparing `tmp/neuron-image-denoise-0.0.2.tar.gz` & `tmp/neuron-image-denoise-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuron-image-denoise-0.0.2.tar", last modified: Tue Jun  6 10:17:25 2023, max compression
+gzip compressed data, was "neuron-image-denoise-0.0.3.tar", last modified: Tue Jun  6 11:45:17 2023, max compression
```

## Comparing `neuron-image-denoise-0.0.2.tar` & `neuron-image-denoise-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 10:17:25.366533 neuron-image-denoise-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-06-06 10:17:25.336611 neuron-image-denoise-0.0.2/.github/
--rw-rw-rw-   0        0        0        6 2023-06-04 10:12:59.000000 neuron-image-denoise-0.0.2/.github/python-version.txt
-drwxrwxrwx   0        0        0        0 2023-06-06 10:17:25.338606 neuron-image-denoise-0.0.2/.github/workflows/
--rw-rw-rw-   0        0        0     1451 2023-06-04 10:12:59.000000 neuron-image-denoise-0.0.2/.github/workflows/static.yml
--rw-rw-rw-   0        0        0     3258 2023-06-06 05:03:03.000000 neuron-image-denoise-0.0.2/.gitignore
--rw-rw-rw-   0        0        0     1096 2023-06-03 10:23:41.000000 neuron-image-denoise-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       22 2023-06-04 10:06:59.000000 neuron-image-denoise-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2612 2023-06-06 10:17:25.365534 neuron-image-denoise-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1929 2023-06-06 10:08:32.000000 neuron-image-denoise-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 10:17:25.354564 neuron-image-denoise-0.0.2/neuron_image_denoise/
--rw-rw-rw-   0        0        0      219 2023-06-05 16:25:08.000000 neuron-image-denoise-0.0.2/neuron_image_denoise/__init__.py
--rw-rw-rw-   0        0        0     3272 2023-06-06 10:06:27.000000 neuron-image-denoise-0.0.2/neuron_image_denoise/_filter.pyx
--rw-rw-rw-   0        0        0     2887 2023-06-06 10:15:01.000000 neuron-image-denoise-0.0.2/neuron_image_denoise/filter.py
-drwxrwxrwx   0        0        0        0 2023-06-06 10:17:25.362542 neuron-image-denoise-0.0.2/neuron_image_denoise.egg-info/
--rw-rw-rw-   0        0        0     2612 2023-06-06 10:17:25.000000 neuron-image-denoise-0.0.2/neuron_image_denoise.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-06-06 10:17:25.000000 neuron-image-denoise-0.0.2/neuron_image_denoise.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 10:17:25.000000 neuron-image-denoise-0.0.2/neuron_image_denoise.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-06 10:17:25.000000 neuron-image-denoise-0.0.2/neuron_image_denoise.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-06 10:17:25.000000 neuron-image-denoise-0.0.2/neuron_image_denoise.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      947 2023-06-06 08:02:29.000000 neuron-image-denoise-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-06 10:17:25.366533 neuron-image-denoise-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      437 2023-06-04 10:22:19.000000 neuron-image-denoise-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 10:17:25.364535 neuron-image-denoise-0.0.2/test/
--rw-rw-rw-   0        0        0      271 2023-06-06 10:13:29.000000 neuron-image-denoise-0.0.2/test/case1.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:45:17.196068 neuron-image-denoise-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-06-06 11:45:17.178118 neuron-image-denoise-0.0.3/.github/
+-rw-rw-rw-   0        0        0        6 2023-06-04 10:12:59.000000 neuron-image-denoise-0.0.3/.github/python-version.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 11:45:17.179113 neuron-image-denoise-0.0.3/.github/workflows/
+-rw-rw-rw-   0        0        0     1451 2023-06-04 10:12:59.000000 neuron-image-denoise-0.0.3/.github/workflows/static.yml
+-rw-rw-rw-   0        0        0     3258 2023-06-06 05:03:03.000000 neuron-image-denoise-0.0.3/.gitignore
+-rw-rw-rw-   0        0        0     1096 2023-06-03 10:23:41.000000 neuron-image-denoise-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       22 2023-06-04 10:06:59.000000 neuron-image-denoise-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2612 2023-06-06 11:45:17.196068 neuron-image-denoise-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1929 2023-06-06 10:08:32.000000 neuron-image-denoise-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 11:45:17.184101 neuron-image-denoise-0.0.3/neuron_image_denoise/
+-rw-rw-rw-   0        0        0      219 2023-06-05 16:25:08.000000 neuron-image-denoise-0.0.3/neuron_image_denoise/__init__.py
+-rw-rw-rw-   0        0        0     3272 2023-06-06 10:06:27.000000 neuron-image-denoise-0.0.3/neuron_image_denoise/_filter.pyx
+-rw-rw-rw-   0        0        0     3195 2023-06-06 11:33:17.000000 neuron-image-denoise-0.0.3/neuron_image_denoise/filter.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:45:17.192079 neuron-image-denoise-0.0.3/neuron_image_denoise.egg-info/
+-rw-rw-rw-   0        0        0     2612 2023-06-06 11:45:16.000000 neuron-image-denoise-0.0.3/neuron_image_denoise.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-06-06 11:45:17.000000 neuron-image-denoise-0.0.3/neuron_image_denoise.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 11:45:16.000000 neuron-image-denoise-0.0.3/neuron_image_denoise.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-06 11:45:16.000000 neuron-image-denoise-0.0.3/neuron_image_denoise.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-06 11:45:16.000000 neuron-image-denoise-0.0.3/neuron_image_denoise.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      947 2023-06-06 08:02:29.000000 neuron-image-denoise-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-06 11:45:17.197066 neuron-image-denoise-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      437 2023-06-04 10:22:19.000000 neuron-image-denoise-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:45:17.194098 neuron-image-denoise-0.0.3/test/
+-rw-rw-rw-   0        0        0      317 2023-06-06 11:35:31.000000 neuron-image-denoise-0.0.3/test/case1.py
```

### Comparing `neuron-image-denoise-0.0.2/.github/workflows/static.yml` & `neuron-image-denoise-0.0.3/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `neuron-image-denoise-0.0.2/.gitignore` & `neuron-image-denoise-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `neuron-image-denoise-0.0.2/LICENSE` & `neuron-image-denoise-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `neuron-image-denoise-0.0.2/PKG-INFO` & `neuron-image-denoise-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuron-image-denoise
-Version: 0.0.2
+Version: 0.0.3
 Summary: Fluorescent neuron image denoising tools
 Author-email: Zuohan Zhao <zzhmark@126.com>
 License: MIT License
 Project-URL: GitHub Project, https://github.com/SEU-ALLEN-codebase/neuron-image-denoise-py
 Project-URL: Documentation, https://SEU-ALLEN-codebase.github.io/neuron-image-denoise-py
 Keywords: vaa3d,neuron-morphology,image-processing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `neuron-image-denoise-0.0.2/README.md` & `neuron-image-denoise-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `neuron-image-denoise-0.0.2/neuron_image_denoise/_filter.pyx` & `neuron-image-denoise-0.0.3/neuron_image_denoise/_filter.pyx`

 * *Files identical despite different names*

### Comparing `neuron-image-denoise-0.0.2/neuron_image_denoise/filter.py` & `neuron-image-denoise-0.0.3/neuron_image_denoise/filter.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,24 +41,28 @@
     if type(lower) is float:
         lower = np.quantile(img, lower)
     if type(upper) is float:
         upper = np.quantile(img, upper)
     return ((img.clip(lower, upper) - lower) / (upper - lower) * 255).astype(np.uint8)
 
 
-def gauss_attenuation_filter(img: np.ndarray, sigma=32, attenuation=.1, truncate=2.):
+def gauss_attenuation_filter(img: np.ndarray, sigma=32, attenuation=.1, truncate=2., warmup=32):
     """
     Fast and stable flare cancelling and overall denoising.
 
     :param img: 3D image array.
     :param sigma: gaussian sigma, scalar or a tuple of 2 scalar.
     :param attenuation: cancel weight of each z slice, the bigger the more removal.
     :param truncate: this many times of sigma will be truncated to speed up gaussian.
+    :param warmup: the times that the gaussian is repeated on the init slice to warm up the filter.
     :return: image with flare removed
     """
 
     gpool = np.zeros([img.shape[1], img.shape[2]], dtype=float)
     out = np.zeros_like(img)
+    for i in range(warmup):
+        out[-1] = (img[-1] - gpool * attenuation).clip(0).astype(np.uint16)
+        gpool = gaussian(gpool + out[-1], sigma, preserve_range=True, truncate=truncate)
     for i in range(img.shape[0] - 1, -1, -1):
         out[i] = (img[i] - gpool * attenuation).clip(0).astype(np.uint16)
         gpool = gaussian(gpool + out[i], sigma, preserve_range=True, truncate=truncate)
     return out
```

### Comparing `neuron-image-denoise-0.0.2/neuron_image_denoise.egg-info/PKG-INFO` & `neuron-image-denoise-0.0.3/neuron_image_denoise.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuron-image-denoise
-Version: 0.0.2
+Version: 0.0.3
 Summary: Fluorescent neuron image denoising tools
 Author-email: Zuohan Zhao <zzhmark@126.com>
 License: MIT License
 Project-URL: GitHub Project, https://github.com/SEU-ALLEN-codebase/neuron-image-denoise-py
 Project-URL: Documentation, https://SEU-ALLEN-codebase.github.io/neuron-image-denoise-py
 Keywords: vaa3d,neuron-morphology,image-processing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `neuron-image-denoise-0.0.2/pyproject.toml` & `neuron-image-denoise-0.0.3/pyproject.toml`

 * *Files identical despite different names*

