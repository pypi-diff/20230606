# Comparing `tmp/foundation_cancer_image_biomarker-0.0.1a0.tar.gz` & `tmp/foundation_cancer_image_biomarker-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundation_cancer_image_biomarker-0.0.1a0.tar", max compression
+gzip compressed data, was "foundation_cancer_image_biomarker-0.0.1a1.tar", max compression
```

## Comparing `foundation_cancer_image_biomarker-0.0.1a0.tar` & `foundation_cancer_image_biomarker-0.0.1a1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1076 2023-06-04 18:03:55.694363 foundation_cancer_image_biomarker-0.0.1a0/LICENSE
--rw-r--r--   0        0        0     4918 2023-06-04 21:16:58.832951 foundation_cancer_image_biomarker-0.0.1a0/README.md
--rw-r--r--   0        0        0      516 2023-06-04 18:03:55.674363 foundation_cancer_image_biomarker-0.0.1a0/fmcib/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 21:18:23.348278 foundation_cancer_image_biomarker-0.0.1a0/fmcib/models/__init__.py
--rw-r--r--   0        0        0      676 2023-06-05 05:41:51.121939 foundation_cancer_image_biomarker-0.0.1a0/fmcib/models/resnet50.py
--rw-r--r--   0        0        0        0 2023-06-05 03:56:42.750721 foundation_cancer_image_biomarker-0.0.1a0/fmcib/preprocessing/__init__.py
--rw-r--r--   0        0        0     4319 2023-06-05 04:24:50.653868 foundation_cancer_image_biomarker-0.0.1a0/fmcib/preprocessing/seed_based_crop.py
--rw-r--r--   0        0        0       30 2023-06-05 04:21:20.431473 foundation_cancer_image_biomarker-0.0.1a0/fmcib/preprocessing/transforms.py
--rw-r--r--   0        0        0      356 2023-06-05 05:41:07.974276 foundation_cancer_image_biomarker-0.0.1a0/fmcib/utils/download_utils.py
--rw-r--r--   0        0        0      110 2023-06-05 04:47:02.627639 foundation_cancer_image_biomarker-0.0.1a0/fmcib/utils/idc_helper.py
--rw-r--r--   0        0        0        0 2023-06-05 03:57:32.526329 foundation_cancer_image_biomarker-0.0.1a0/fmcib/visualization/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 03:57:26.342378 foundation_cancer_image_biomarker-0.0.1a0/fmcib/visualization/verify_io.py
--rw-r--r--   0        0        0     4105 2023-06-05 05:58:34.602180 foundation_cancer_image_biomarker-0.0.1a0/pyproject.toml
--rw-r--r--   0        0        0     6055 1970-01-01 00:00:00.000000 foundation_cancer_image_biomarker-0.0.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-04 18:03:55.694363 foundation_cancer_image_biomarker-0.0.1a1/LICENSE
+-rw-r--r--   0        0        0     4911 2023-06-06 01:33:53.653635 foundation_cancer_image_biomarker-0.0.1a1/README.md
+-rw-r--r--   0        0        0      516 2023-06-04 18:03:55.674363 foundation_cancer_image_biomarker-0.0.1a1/fmcib/__init__.py
+-rw-r--r--   0        0        0       31 2023-06-06 01:43:30.477335 foundation_cancer_image_biomarker-0.0.1a1/fmcib/models/__init__.py
+-rw-r--r--   0        0        0      767 2023-06-06 01:43:30.497334 foundation_cancer_image_biomarker-0.0.1a1/fmcib/models/resnet50.py
+-rw-r--r--   0        0        0     1437 2023-06-06 01:43:30.521334 foundation_cancer_image_biomarker-0.0.1a1/fmcib/preprocessing/__init__.py
+-rw-r--r--   0        0        0     4283 2023-06-06 01:43:30.549334 foundation_cancer_image_biomarker-0.0.1a1/fmcib/preprocessing/seed_based_crop.py
+-rw-r--r--   0        0        0      943 2023-06-06 01:43:30.505334 foundation_cancer_image_biomarker-0.0.1a1/fmcib/run.py
+-rw-r--r--   0        0        0       67 2023-06-06 01:43:30.477335 foundation_cancer_image_biomarker-0.0.1a1/fmcib/utils/__init__.py
+-rw-r--r--   0        0        0      367 2023-06-06 01:43:30.485334 foundation_cancer_image_biomarker-0.0.1a1/fmcib/utils/download_utils.py
+-rw-r--r--   0        0        0     3436 2023-06-06 01:43:30.553334 foundation_cancer_image_biomarker-0.0.1a1/fmcib/utils/idc_helper.py
+-rw-r--r--   0        0        0       44 2023-06-06 01:43:30.477335 foundation_cancer_image_biomarker-0.0.1a1/fmcib/visualization/__init__.py
+-rw-r--r--   0        0        0      499 2023-06-06 01:41:36.682184 foundation_cancer_image_biomarker-0.0.1a1/fmcib/visualization/verify_io.py
+-rw-r--r--   0        0        0     4149 2023-06-06 02:04:37.523600 foundation_cancer_image_biomarker-0.0.1a1/pyproject.toml
+-rw-r--r--   0        0        0     6288 1970-01-01 00:00:00.000000 foundation_cancer_image_biomarker-0.0.1a1/PKG-INFO
```

### Comparing `foundation_cancer_image_biomarker-0.0.1a0/LICENSE` & `foundation_cancer_image_biomarker-0.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a0/README.md` & `foundation_cancer_image_biomarker-0.0.1a1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # Foundation Models for Quantitative Imaging Biomarker Discovery in Cancer Imaging
 
-<div align="center">
+<!-- <div align="center">
 
 [![Build status](https://github.com/foundation_image_biomarker/foundation-image-biomarker/workflows/build/badge.svg?branch=master&event=push)](https://github.com/foundation_image_biomarker/foundation-image-biomarker/actions?query=workflow%3Abuild)
 [![Python Version](https://img.shields.io/pypi/pyversions/foundation-image-biomarker.svg)](https://pypi.org/project/foundation-image-biomarker/)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/foundation_image_biomarker/foundation-image-biomarker/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/foundation_image_biomarker/foundation-image-biomarker/blob/master/.pre-commit-config.yaml)
 [![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/foundation_image_biomarker/foundation-image-biomarker/releases)
 [![License](https://img.shields.io/github/license/foundation_image_biomarker/foundation-image-biomarker)](https://github.com/foundation_image_biomarker/foundation-image-biomarker/blob/master/LICENSE)
 ![Coverage Report](assets/images/coverage.svg)
 
-</div>
+</div> -->
 
 ## Overview
 This is the the official repository for the paper <i> Foundation Models for Quantitative Imaging Biomarker Discovery for Cancer Imaging </i> <br/>
  Suraj Pai, Dennis Bontempi, Vasco Prudente, Ibrahim Hadzic, Mateo Sokač, Tafadzwa L. Chaunzwa, Simon Bernatz, Ahmed Hosny, Raymond H Mak, Nicolai J Birkbak, Hugo JWL Aerts
 
 ![](assets/images/overview.png)
  <b>General overview of the study.</b><b> a. Foundation model pre-training.</b> A foundation model, specifically a deep convolutional encoder model, was pre-trained by contrasting volumes with and without lesions. <b> b. </b> Clinical application of the foundation model. The foundation model was used to extract biomarkers and then evaluated for three classification tasks on diverse datasets. <b>c. Foundation model implementation approaches </b>  The foundation model was adapted to specific use cases by extracting features or through fine-tuning (left). <b> d. Evaluation against supervised models with selected performance metrics. </b> We compared the performance of the foundation models against conventional supervised implementations, trained from scratch (left) and fine-tuned from a different task (right). The comparison was made through several criteria for the different use cases, including quantitative performance, stability, and biological analysis. Biological, clinical, and stability analyses are limited to use case 2 due to the availability of associated data. 
@@ -49,17 +49,17 @@
 
 ## Re-running all the experiments outlined in the paper
 You can find detailed instructions for this [here](experiments/README.md)
 
 
 ## 🛡 License
 
-[![License](https://img.shields.io/github/license/foundation_image_biomarker/foundation-image-biomarker)](https://github.com/foundation_image_biomarker/foundation-image-biomarker/blob/master/LICENSE)
+[![License](https://img.shields.io/github/license/foundation_image_biomarker/foundation-image-biomarker)](https://github.com/AIM-Harvard/foundation-cancer-image-biomarker/blob/master/LICENSE)
 
-This project is licensed under the terms of the `MIT` license. See [LICENSE](https://github.com/foundation_image_biomarker/foundation-image-biomarker/blob/master/LICENSE) for more details.
+This project is licensed under the terms of the `MIT` license. See [LICENSE](https://github.com/AIM-Harvard/foundation-cancer-image-biomarker/blob/master/LICENSE) for more details.
 
 ## 📃 Citation
 
 ```bibtex
 @misc{foundation-image-biomarker,
   author = {AIM-Harvard},
   title = {Official repo for "Foundation Models for Quantitative Biomarker Discovery in Cancer Imaging"},
```

### Comparing `foundation_cancer_image_biomarker-0.0.1a0/fmcib/__init__.py` & `foundation_cancer_image_biomarker-0.0.1a1/fmcib/__init__.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a0/fmcib/preprocessing/seed_based_crop.py` & `foundation_cancer_image_biomarker-0.0.1a1/fmcib/preprocessing/seed_based_crop.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 Author: Suraj Pai
 Email: bspai@bwh.harvard.edu
 This script contains two classes:
 1. SeedBasedPatchCropd
 2. SeedBasedPatchCrop
 """
 
-from typing import Any, Tuple, Mapping, Hashable, Dict
-from monai.transforms import MapTransform, Transform
-from monai.config.type_definitions import NdarrayOrTensor
+from typing import Any, Dict, Hashable, Mapping, Tuple
+
 import numpy as np
+from monai.config.type_definitions import NdarrayOrTensor
+from monai.transforms import MapTransform, Transform
 
 
 class SeedBasedPatchCropd(MapTransform):
     def __init__(self, keys, roi_size, allow_missing_keys=False, coord_orientation="RAS", global_coordinates=True) -> None:
         """
         Initialize SeedBasedPatchCropd class.
 
@@ -23,17 +24,15 @@
             allow_missing_keys: If True, do not raise an error if some keys in the input data dictionary are missing.
             coord_orientation: Coordinate system (RAS or LPS) of input coordinates.
             global_coordinates: If True, coordinates are in global coordinates; otherwise, local coordinates.
         """
         super().__init__(keys=keys, allow_missing_keys=allow_missing_keys)
         self.coord_orientation = coord_orientation
         self.global_coordinates = global_coordinates
-        self.cropper = SeedBasedPatchCrop(
-            roi_size=roi_size
-        )
+        self.cropper = SeedBasedPatchCrop(roi_size=roi_size)
 
     def __call__(self, data: Mapping[Hashable, NdarrayOrTensor]) -> Dict[Hashable, NdarrayOrTensor]:
         """
         Apply transformation to given data.
 
         Args:
             data: Dictionary with image keys and required center coordinates.
@@ -42,15 +41,15 @@
             Dictionary with cropped patches for each key in the input data dictionary.
         """
         d = dict(data)
 
         assert "coordX" in d.keys(), "coordX not found in data"
         assert "coordY" in d.keys(), "coordY not found in data"
         assert "coordZ" in d.keys(), "coordZ not found in data"
-        
+
         # Convert coordinates to RAS orientation to match image orientation
         if self.coord_orientation == "RAS":
             center = (d["coordX"], d["coordY"], d["coordZ"])
         elif self.coord_orientation == "LPS":
             center = (-d["coordX"], -d["coordY"], d["coordZ"])
 
         for key in self.key_iterator(d):
@@ -95,12 +94,12 @@
         min_w, max_w = max(center[1] - Pw // 2, 0), min(center[1] + Pw // 2, W)
         min_d, max_d = max(center[2] - Pd // 2, 0), min(center[2] + Pd // 2, D)
 
         # Check if coordinates are valid
         assert min_h < max_h, "Invalid coordinates: min_h >= max_h"
         assert min_w < max_w, "Invalid coordinates: min_w >= max_w"
         assert min_d < max_d, "Invalid coordinates: min_d >= max_d"
-        
+
         # Crop the patch from the image
         patch = img[:, min_h:max_h, min_w:max_w, min_d:max_d]
 
-        return patch
+        return patch
```

### Comparing `foundation_cancer_image_biomarker-0.0.1a0/pyproject.toml` & `foundation_cancer_image_biomarker-0.0.1a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "foundation-cancer-image-biomarker"
-version = "0.0.1a0"
+version = "0.0.1a1"
 description = "Official repo for Foundation Models for Quantitative Biomarker Discovery in Cancer Imaging [INSERT DOI]"
 readme = "README.md"
 authors = ["Suraj Pai <bspai@bwh.harvard.edu>"]
 license = "MIT"
 repository = "https://github.com/AIM-Harvard/foundation-cancer-image-biomarker"
 homepage = "https://aim.hms.harvard.edu/foundation-cancer-image-biomarker"
 
 # Keywords description https://python-poetry.org/docs/pyproject/#keywords
 keywords = []  #! Update me
 packages = [
     { include = "fmcib" },
 ]
-include = ["fmcib/files/gcs_lung1_paths.txt"]
 
 # Pypi classifiers: https://pypi.org/classifiers/
 classifiers = [  #! Update me
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Topic :: Software Development :: Libraries :: Python Modules",
@@ -35,14 +34,20 @@
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 project-lighter = {version = "^0.0.2a2", allow-prereleases = true}
 wget = "^3.2"
 google-cloud-storage = "^2.9.0"
+thedicomsort = "^1.0.1"
+dcmrtstruct2nii = "^5"
+nibabel = "^5.1.0"
+matplotlib = "^3.7.1"
+platipy = "0.4.1"
+pynrrd = "^1.0.0"
 
 [tool.poetry.dev-dependencies]
 bandit = "^1.7.1"
 black = {version = "^21.10b0", allow-prereleases = true}
 isort = {extras = ["colors"], version = "^5.10.1"}
 mypy = "^0.910"
 mypy-extensions = "^0.4.3"
@@ -160,8 +165,8 @@
     no-else-return,
 """
 generated-members = "torch.*"
 
 [tool.pylint.master]
 fail-under=8
 
-[tool.poetry_bumpversion.file."foundation-cancer-image-biomarker/version.py"]
+[tool.poetry_bumpversion.file."version.py"]
```

### Comparing `foundation_cancer_image_biomarker-0.0.1a0/PKG-INFO` & `foundation_cancer_image_biomarker-0.0.1a1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundation-cancer-image-biomarker
-Version: 0.0.1a0
+Version: 0.0.1a1
 Summary: Official repo for Foundation Models for Quantitative Biomarker Discovery in Cancer Imaging [INSERT DOI]
 Home-page: https://aim.hms.harvard.edu/foundation-cancer-image-biomarker
 License: MIT
 Author: Suraj Pai
 Author-email: bspai@bwh.harvard.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -13,36 +13,42 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: dcmrtstruct2nii (>=5,<6)
 Requires-Dist: google-cloud-storage (>=2.9.0,<3.0.0)
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
+Requires-Dist: nibabel (>=5.1.0,<6.0.0)
+Requires-Dist: platipy (==0.4.1)
 Requires-Dist: project-lighter (>=0.0.2a2,<0.0.3)
+Requires-Dist: pynrrd (>=1.0.0,<2.0.0)
+Requires-Dist: thedicomsort (>=1.0.1,<2.0.0)
 Requires-Dist: wget (>=3.2,<4.0)
 Project-URL: Repository, https://github.com/AIM-Harvard/foundation-cancer-image-biomarker
 Description-Content-Type: text/markdown
 
 # Foundation Models for Quantitative Imaging Biomarker Discovery in Cancer Imaging
 
-<div align="center">
+<!-- <div align="center">
 
 [![Build status](https://github.com/foundation_image_biomarker/foundation-image-biomarker/workflows/build/badge.svg?branch=master&event=push)](https://github.com/foundation_image_biomarker/foundation-image-biomarker/actions?query=workflow%3Abuild)
 [![Python Version](https://img.shields.io/pypi/pyversions/foundation-image-biomarker.svg)](https://pypi.org/project/foundation-image-biomarker/)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/foundation_image_biomarker/foundation-image-biomarker/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/foundation_image_biomarker/foundation-image-biomarker/blob/master/.pre-commit-config.yaml)
 [![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/foundation_image_biomarker/foundation-image-biomarker/releases)
 [![License](https://img.shields.io/github/license/foundation_image_biomarker/foundation-image-biomarker)](https://github.com/foundation_image_biomarker/foundation-image-biomarker/blob/master/LICENSE)
 ![Coverage Report](assets/images/coverage.svg)
 
-</div>
+</div> -->
 
 ## Overview
 This is the the official repository for the paper <i> Foundation Models for Quantitative Imaging Biomarker Discovery for Cancer Imaging </i> <br/>
  Suraj Pai, Dennis Bontempi, Vasco Prudente, Ibrahim Hadzic, Mateo Sokač, Tafadzwa L. Chaunzwa, Simon Bernatz, Ahmed Hosny, Raymond H Mak, Nicolai J Birkbak, Hugo JWL Aerts
 
 ![](assets/images/overview.png)
  <b>General overview of the study.</b><b> a. Foundation model pre-training.</b> A foundation model, specifically a deep convolutional encoder model, was pre-trained by contrasting volumes with and without lesions. <b> b. </b> Clinical application of the foundation model. The foundation model was used to extract biomarkers and then evaluated for three classification tasks on diverse datasets. <b>c. Foundation model implementation approaches </b>  The foundation model was adapted to specific use cases by extracting features or through fine-tuning (left). <b> d. Evaluation against supervised models with selected performance metrics. </b> We compared the performance of the foundation models against conventional supervised implementations, trained from scratch (left) and fine-tuned from a different task (right). The comparison was made through several criteria for the different use cases, including quantitative performance, stability, and biological analysis. Biological, clinical, and stability analyses are limited to use case 2 due to the availability of associated data. 
@@ -74,17 +80,17 @@
 
 ## Re-running all the experiments outlined in the paper
 You can find detailed instructions for this [here](experiments/README.md)
 
 
 ## 🛡 License
 
-[![License](https://img.shields.io/github/license/foundation_image_biomarker/foundation-image-biomarker)](https://github.com/foundation_image_biomarker/foundation-image-biomarker/blob/master/LICENSE)
+[![License](https://img.shields.io/github/license/foundation_image_biomarker/foundation-image-biomarker)](https://github.com/AIM-Harvard/foundation-cancer-image-biomarker/blob/master/LICENSE)
 
-This project is licensed under the terms of the `MIT` license. See [LICENSE](https://github.com/foundation_image_biomarker/foundation-image-biomarker/blob/master/LICENSE) for more details.
+This project is licensed under the terms of the `MIT` license. See [LICENSE](https://github.com/AIM-Harvard/foundation-cancer-image-biomarker/blob/master/LICENSE) for more details.
 
 ## 📃 Citation
 
 ```bibtex
 @misc{foundation-image-biomarker,
   author = {AIM-Harvard},
   title = {Official repo for "Foundation Models for Quantitative Biomarker Discovery in Cancer Imaging"},
```

