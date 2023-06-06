# Comparing `tmp/dataset-tools-0.0.8.tar.gz` & `tmp/dataset-tools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset-tools-0.0.8.tar", last modified: Wed May 17 10:26:01 2023, max compression
+gzip compressed data, was "dataset-tools-0.0.9.tar", last modified: Mon Jun  5 13:38:22 2023, max compression
```

## Comparing `dataset-tools-0.0.8.tar` & `dataset-tools-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:26:01.432417 dataset-tools-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-17 10:26:01.432417 dataset-tools-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:26:01.428417 dataset-tools-0.0.8/dataset_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:26:01.432417 dataset-tools-0.0.8/dataset_tools/image/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:26:01.432417 dataset-tools-0.0.8/dataset_tools/image/renders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/image/renders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/image/renders/poster.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/image/renders/previews.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/image/renders/separated_anns_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/image/renders/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:26:01.432417 dataset-tools-0.0.8/dataset_tools/image/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/image/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/image/stats/basestats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/image/stats/class_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/image/stats/class_cooccurrence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/image/stats/classes_per_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/image/stats/heatmaps_for_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8325 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/image/stats/object_and_class_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/image/stats/objects_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/image/stats/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:26:01.432417 dataset-tools-0.0.8/dataset_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-17 10:26:01.000000 dataset-tools-0.0.8/dataset_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-17 10:26:01.000000 dataset-tools-0.0.8/dataset_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 10:26:01.000000 dataset-tools-0.0.8/dataset_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-17 10:26:01.000000 dataset-tools-0.0.8/dataset_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-17 10:26:01.000000 dataset-tools-0.0.8/dataset_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 10:26:01.432417 dataset-tools-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:38:22.035194 dataset-tools-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-05 13:38:22.035194 dataset-tools-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:38:22.023194 dataset-tools-0.0.9/dataset_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:38:22.027194 dataset-tools-0.0.9/dataset_tools/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/convert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:38:22.027194 dataset-tools-0.0.9/dataset_tools/convert/cityscapes/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/convert/cityscapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22156 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/convert/cityscapes/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:38:22.027194 dataset-tools-0.0.9/dataset_tools/convert/coco/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/convert/coco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18686 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/convert/coco/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:38:22.027194 dataset-tools-0.0.9/dataset_tools/convert/pascal/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/convert/pascal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19519 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/convert/pascal/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/download.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:38:22.027194 dataset-tools-0.0.9/dataset_tools/image/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:38:22.031194 dataset-tools-0.0.9/dataset_tools/image/renders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/renders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/renders/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/renders/horizontal_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/renders/poster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/renders/previews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/renders/separated_anns_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/renders/vertical_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/renders/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:38:22.031194 dataset-tools-0.0.9/dataset_tools/image/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/stats/basestats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/stats/class_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/stats/class_cooccurrence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/stats/classes_per_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/stats/heatmaps_for_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/stats/object_and_class_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/stats/objects_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14417 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/stats/preview_for_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/stats/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:38:22.031194 dataset-tools-0.0.9/dataset_tools/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:38:22.035194 dataset-tools-0.0.9/dataset_tools/text/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/text/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/text/summary/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:38:22.027194 dataset-tools-0.0.9/dataset_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-05 13:38:22.000000 dataset-tools-0.0.9/dataset_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-05 13:38:22.000000 dataset-tools-0.0.9/dataset_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:38:22.000000 dataset-tools-0.0.9/dataset_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-05 13:38:22.000000 dataset-tools-0.0.9/dataset_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 13:38:22.000000 dataset-tools-0.0.9/dataset_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 13:38:22.035194 dataset-tools-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/setup.py
```

### Comparing `dataset-tools-0.0.8/LICENSE` & `dataset-tools-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.8/PKG-INFO` & `dataset-tools-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset-tools
-Version: 0.0.8
+Version: 0.0.9
 Summary: Dataset tools for dataset ninja made by Supervisely team.
 Home-page: https://github.com/supervisely/dataset-tools
 Author: Supervisely
 Author-email: support@supervise.ly
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dataset-tools-0.0.8/dataset_tools/__init__.py` & `dataset-tools-0.0.9/dataset_tools/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,28 @@
-# from dataset_tools import image
+from dataset_tools.download import prepare_download_link, update_sly_url_dict
+
 from dataset_tools.image.stats.class_balance import ClassBalance
 from dataset_tools.image.stats.class_cooccurrence import ClassCooccurrence
 
 from dataset_tools.image.stats.classes_per_image import ClassesPerImage
 from dataset_tools.image.stats.heatmaps_for_classes import ClassesHeatmaps
+from dataset_tools.image.stats.preview_for_classes import ClassesPreview
 
 from dataset_tools.image.stats.objects_distribution import ObjectsDistribution
 from dataset_tools.image.stats.object_and_class_sizes import ObjectSizes, ClassSizes
 
 from dataset_tools.image.stats.wrapper import count_stats  # , initialize
 
 
 from dataset_tools.image.renders.wrapper import prepare_renders
 from dataset_tools.image.renders.separated_anns_grid import SideAnnotationsGrid
+from dataset_tools.image.renders.horizontal_grid import HorizontalGrid
+from dataset_tools.image.renders.vertical_grid import VerticalGrid
 from dataset_tools.image.renders.poster import Poster
+
+from dataset_tools.text.summary.generate import (
+    generate_summary_content,
+    get_summary_data,
+    get_summary_data_sly,
+)
+
+from dataset_tools.image.renders.convert import from_mp4_to_webm, compress_mp4, compress_png
```

### Comparing `dataset-tools-0.0.8/dataset_tools/image/renders/poster.py` & `dataset-tools-0.0.9/dataset_tools/image/renders/poster.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import os
 import random
 from typing import List, Union
 
 import cv2
 import numpy as np
-from PIL import Image, ImageDraw
 from tqdm import tqdm
 
 import supervisely as sly
+from dataset_tools.image.renders.convert import compress_png
 from supervisely.imaging import font as sly_font
 
 
 class Poster:
     def __init__(
         self,
         project: Union[str, int],
         project_meta: sly.ProjectMeta,
         api: sly.Api = None,
+        force: bool = False,
     ) -> None:
+        self.force = force
         self._project_meta = project_meta
         self._api = api if api is not None else sly.Api.from_env()  # ?
         self._project = None
         self._images_info = None
         self._items_count = 0
         self._total_labels = 0
         self._local = False
@@ -44,28 +46,32 @@
                 ]
                 for img in img_infos:
                     self._total_labels += img.labels_count
 
         else:
             raise Exception('Parameter "project" has to be one of `int` or `str` types.')
 
-        self._size = (540, 960)
+        self._size = (1080, 1960)
         self._GAP = 20
         self._size_line_1 = (
             (self._size[0] - 3 * self._GAP) // 5 * 3,
             (self._size[1] - 4 * self._GAP) // 3,
         )
         self._size_line_2 = (
             (self._size[0] - 3 * self._GAP) // 5 * 2,
             (self._size[1] - 5 * self._GAP) // 4,
         )
 
         self._poster = np.ones((*self._size, 4), dtype=np.uint8) * 255  # result poster
 
-        self._logo_text = "logo.png"
+        self._logo_path = "logo.png"
+
+    @property
+    def basename_stem(self) -> None:
+        return sly.utils.camel_to_snake(self.__class__.__name__)
 
     def update(self, data: tuple):
         np_images = []
         join_data = [(ds, img, ann) for ds, list1, list2 in data for img, ann in zip(list1, list2)]
         random.shuffle(join_data)
         i = 0
         with tqdm(desc="Downloading 7 sample images.", total=7) as pbar:
@@ -79,177 +85,195 @@
                     continue
                 np_img = (
                     sly.image.read(ds.get_img_path(img_info.name))
                     if self._local
                     else self._api.image.download_np(img_info.id)
                 )
 
-                if len(np_images) % 2 == 0:
-                    h, w = np_img.shape[:2]
-                    background = np.ones((h, w, 3), dtype=np.uint8) * 255
-                    alpha = 0.5
-                    np_img = cv2.addWeighted(background, 1 - alpha, np_img, alpha, 0)
-                    ann.draw_pretty(np_img, thickness=0, opacity=0.3)
-                else:
-                    thickness = 7 if len(np_images) < 3 else 9
-                    ann.draw_contour(np_img, color=[253, 69, 133], thickness=thickness)
+                h, w = np_img.shape[:2]
+                background = np.ones((h, w, 3), dtype=np.uint8) * 255
+                ann.draw_pretty(np_img, thickness=0, opacity=0.7)
+                np_img = cv2.addWeighted(np_img, 0.8, background, 0.2, 0)
+
+                # backup
+                # if len(np_images) % 2 == 0:
+                #     h, w = np_img.shape[:2]
+                #     background = np.ones((h, w, 3), dtype=np.uint8) * 255
+                #     alpha = 0.5
+                #     np_img = cv2.addWeighted(background, 1 - alpha, np_img, alpha, 0)
+                #     ann.draw_pretty(np_img, thickness=0, opacity=0.6)
+                # else:
+                #     ann: sly.Annotation
+                #     thickness = 3
+                #     ann.draw_contour(np_img, thickness=thickness)
 
-                np_images.append(np_img)
+                np_images.append(self._resize_image(np_img, i))
                 i += 1
                 pbar.update(1)
 
-        self._resize_images(np_images)
         self._create_frame(np_images)
-        self._draw_text_and_bboxes()
-        self._put_watermark(self._logo_text)
+        self._draw_text_and_rectangles()
 
     def to_image(self, path: str = None):
+        path_part, ext = os.path.splitext(path)
+        tmp_path = f"{path_part}-o{ext}"
         if path is None:
             storage_dir = sly.app.get_data_dir()
-            sly.fs.clean_dir(storage_dir)
-            path = os.path.join(storage_dir, "poster.jpeg")
-        sly.image.write(path, self._poster)
+            path = os.path.join(storage_dir, "horizontal_grid.png")
+
+        sly.image.write(tmp_path, self._poster)
+        compress_png(tmp_path, path)
+        sly.fs.silent_remove(tmp_path)
         sly.logger.info(f"Poster saved to: {path}")
 
-    def _resize_images(self, images):
-        for i, img in enumerate(images):
-            h, w = (self._size_line_1) if i < 3 else (self._size_line_2)
-            img_h, img_w = img.shape[1], img.shape[0]
-            src_ratio = w / h
-            img_ratio = img_w / img_h
-            if img_ratio != src_ratio:
-                if img_ratio > src_ratio:
-                    img_h, img_w = int(w * img_ratio), w
-                    img = sly.image.resize_inter_nearest(img, (img_h, img_w))
-                else:
-                    img_h, img_w = h, int(h / img_ratio)
-                    img = sly.image.resize_inter_nearest(img, (img_h, img_w))
-                rect = ((img_h - h) // 2, (img_w - w) // 2, (img_h + h) // 2, (img_w + w) // 2)
-                img = sly.image.crop_with_padding(img, sly.Rectangle(*rect))
-            else:
-                img = sly.image.resize(img, (h, w))
-
-            rgba_image = np.zeros((img.shape[0], img.shape[1], 4), dtype=np.uint8)
-            rgba_image[:, :, :3] = img
-            images[i] = rgba_image
-        sly.logger.info(f"Resized {len(images)} sample images.")
+    def _resize_image(self, image: np.ndarray, image_num: int):
+        h, w = self._size_line_1 if image_num < 3 else self._size_line_2
+        img_h, img_w = image.shape[:2]
+        scale_ratio = max(h / img_h, w / img_w)
+        img_h, img_w = int(img_h * scale_ratio), int(img_w * scale_ratio)
+        image = sly.image.resize(image, (img_h, img_w))
+        start_h = (img_h - h) // 2
+        start_w = (img_w - w) // 2
+        rect = (start_h, start_w, start_h + h, start_w + w)
+        image = sly.image.crop_with_padding(image, sly.Rectangle(*rect))
+
+        rgba_image = np.zeros((h, w, 4), dtype=np.uint8)
+        rgba_image[:h, :w, :3] = image[:h, :w, :3]
+        return rgba_image
 
-    def _draw_text_and_bboxes(self):
+    def _draw_text_and_rectangles(self):
         base_font_size = sly_font.get_readable_font_size(self._size)
-        fonts = [
-            sly_font.get_font(font_size=int(base_font_size * 6)),  # title
-            sly_font.get_font(font_size=int(base_font_size * 1.5)),  # images count
-            sly_font.get_font(font_size=int(base_font_size * 1.3)),  # classes count
-            sly_font.get_font(font_size=int(base_font_size * 1)),  # labels count
-        ]
-        texts = self._get_text_from_project()
-
-        h, w = self._size
-
-        bg_image = np.zeros((h, w, 3), dtype=np.uint8)
-
-        def _get_text_bbox(text, font):
-            if text is None:
-                return None
-            left, top, right, bottom = font.getbbox(text)
-            text_w, text_h = right - left, bottom
-            while text_w > w * 0.9:
-                font_size *= 0.96
-                left, top, right, bottom = font.getbbox(text)
-                text_w, text_h = right - left, bottom
-            return text_w, text_h
-
-        text_sizes = [_get_text_bbox(t, f) for t, f in zip(texts, fonts)]
-
-        x1, y1 = (w - text_sizes[0][0]) // 2, (h - text_sizes[0][1]) // 2
-        text_coords = [
-            (x1, y1),
-            (x1, (y1 - text_sizes[1][1])),
-            (x1 + text_sizes[0][0] - text_sizes[2][0], (y1 - text_sizes[2][1])),
-        ]
-        if text_sizes[3] is not None:
-            text_coords.append((w // 2 - text_sizes[3][0], (y1 + text_sizes[0][1])))
-
-        bg_image = self._gradient(bg_image, x1, 0, x1 + text_sizes[0][0], h)
-
-        for idx, (t, c, s, f) in enumerate(zip(texts, text_coords, text_sizes, fonts)):
-            if c is False:
-                continue
-            left, top, right, bottom = c[0], c[1], c[0] + s[0], c[1] + s[1]
-            if idx == 0:
-                offset = self._GAP // 5
-                bg_image[top + offset : bottom - offset, left + offset : right - offset] = 255
-            offs_x = (right - left - f.getlength(t)) // 2
-            offs_y = f.getbbox(t)[1] // 2
-            sly.image.draw_text(
-                bg_image, t, (top - offs_y, left + offs_x), font=f, fill_background=False
-            )
+        font_name_title = "FiraSans-Regular.ttf"
+        font_name_subs = "FiraSans-Thin.ttf"
+        font_title = sly_font.get_font(font_name_title, int(base_font_size * 6))
+        font_subs = sly_font.get_font(font_name_subs, int(base_font_size * 1.8))
+        title, *subs = self._get_text_from_project()
+        _, _, _, subs_height = font_subs.getbbox("".join(subs))
+
+        poster_h, poster_w = self._size
+
+        bg_image = np.zeros((poster_h, poster_w, 3), dtype=np.uint8)
+
+        title_bottom = self._draw_title(bg_image, font_title, title)
+        sub_imgs = [self._draw_subtitles(font_subs, text, subs_height) for text in subs]
+        logo = self._draw_logo(subs_height)
+
+        image = np.hstack(sub_imgs)
+        subs_h, subs_w = image.shape[:2]
+        subs_x = (poster_w - subs_w - logo.shape[1]) // 2
+        subs_y = title_bottom + self._GAP
+
+        bg = bg_image[subs_y : subs_y + subs_h, subs_x : subs_x + subs_w, :3]
+
+        alpha_channel = np.where(np.all(image == 0, axis=-1), 0, 255).astype(np.uint8)
+        text_image_bw = cv2.cvtColor(image, cv2.COLOR_BGRA2GRAY)
+        _, text_mask = cv2.threshold(text_image_bw, 255, 255, cv2.THRESH_BINARY)
+        inverse_text_mask = cv2.bitwise_not(text_mask)
+        background_masked = cv2.bitwise_and(bg, bg, mask=inverse_text_mask)
+        text_image_alpha = cv2.merge(
+            (image[:, :, 0], image[:, :, 1], image[:, :, 2], alpha_channel)
+        )
+        text_image_alpha = cv2.cvtColor(text_image_alpha, cv2.COLOR_BGRA2BGR)
+        result = cv2.add(background_masked, text_image_alpha)
+        result = np.hstack([result, logo])
+
+        h, w = result.shape[:2]
+        cv2.rectangle(result, (0, 0), (w - 1, h - 1), (255, 255, 255), 2)
+        self._poster[subs_y : subs_y + h, subs_x : subs_x + w, :3] = result
+
+    def _draw_title(self, image, font, text):
+        poster_h, poster_w = self._size
+        l, t, r, b = font.getbbox(text)
+        title_w, title_h = r - l, b
+        while title_w > poster_w * 0.9:
+            font = font.font_variant(size=int(font.size * 0.96))
+            l, t, r, b = font.getbbox(text)
+            title_w, title_h = r - l, b
+        title_x, title_y = (poster_w - title_w) // 2, (poster_h - title_h) // 2
+        left, top, right, bottom = title_x, title_y, title_x + title_w, title_y + title_h
+
+        self._gradient(image, title_x, 0, title_x + title_w, poster_h)
+        p = self._GAP // 3
+        image[top + p : bottom - p, left + p : right - p] = 255
+
+        sly.image.draw_text(
+            image,
+            text,
+            (top - t // 2, left),
+            font=font,
+            fill_background=False,
+            color=(0, 0, 0, 210),
+        )
+
+        self._poster[top:bottom, left:right, :3] = image[top:bottom, left:right, :3]
+        return bottom + p
 
-            self._poster[top:bottom, left:right, :3] = bg_image[top:bottom, left:right, :3]
+    def _draw_subtitles(self, font, text, height):
+        _, t, r, _ = font.getbbox(text)
+        pad = self._GAP // 4
+        w = r + self._GAP
+        image = np.ones((height, w, 3), dtype=np.uint8) * 255
+        sly.image.draw_text(
+            image,
+            text,
+            (-t // 2, pad * 2),
+            font=font,
+            fill_background=False,
+        )
+        image[:, r + 3 * pad :, :3] = 0
+        image = np.dstack((image, np.ones((*image.shape[:2], 1), dtype=np.uint8) * 255))
+        return 255 - image
+
+    def _draw_logo(self, height):
+        logo = sly.image.read(self._logo_path)
+        logo_h, logo_w = logo.shape[:2]
+        scale_factor = height / logo_h
+        logo_h, logo_w = height, int(logo_w * scale_factor)
+
+        logo = sly.image.resize(logo, (logo_h, logo_w))
+        image = np.zeros((logo_h, logo_w, 4), dtype=np.uint8)
+        image[:, :, :3] = logo[:, :, :3]
+        return logo
 
     def _get_text_from_project(self):
-        title = (
+        texts = []
+        texts.append(
             self._project.name.upper()
             if len(self._project.name.split(" ")) < 4
             else " ".join(self._project.name.split(" ")[:3]).upper()
         )
-        images_text = f"{self._items_count} IMAGES"
-        classes_text = f"{len(self._project_meta.obj_classes)} CLASSES"
-        labels_text = f"{self._total_labels} LABELS" if self._total_labels else None
 
-        return title, images_text, classes_text, labels_text
+        texts.append(f"{self._items_count} IMAGES")
+        texts.append(f"{len(self._project_meta.obj_classes)} CLASSES")
+        if self._total_labels:
+            texts.append(f"{self._total_labels} LABELS")
+
+        return texts
 
     def _gradient(self, img, left, top, right, bottom):
-        c1 = np.array((210, 95, 144))  # rgb (253, 69, 133)
-        c2 = np.array((234, 197, 77))  # (254, 208, 0)
+        c1 = np.array((225, 181, 62))  # rgb
+        c2 = np.array((219, 84, 150))  # rgb
         im = np.zeros((bottom - top, right - left, 3), dtype=np.uint8)
         row = np.linspace(0, 1, right - left)
         kernel_1d = np.tile(row, (bottom - top, 1))
         kernel = cv2.merge((kernel_1d, kernel_1d, kernel_1d))
         im = kernel * c1 + (1 - kernel) * c2
         im = im.astype(np.uint8)
         img[top:bottom, left:right, :3] = im
         return img
 
     def _create_frame(self, images: List[np.ndarray]):
         x, y = self._GAP, self._GAP
+        x_end, y_end = x, y
+
         for img in images[:3]:
             x_end, y_end = x + img.shape[1], y + img.shape[0]
             self._poster[y:y_end, x:x_end] = img
             x = x_end + self._GAP
 
         y = y_end + self._GAP
         x = self._GAP
+
         for img in images[3:]:
             x_end, y_end = x + img.shape[1], y + img.shape[0]
             self._poster[y:y_end, x:x_end] = img
             x = x_end + self._GAP
-
-    def _put_watermark(self, path):
-        img = sly.image.read(path)
-        poster_h, poster_w = self._size
-
-        # resize logo to poster size
-        mark_w = int(self._size_line_2[0] * 0.9)
-        mark_h = mark_w * img.shape[0] // img.shape[1]
-        img = cv2.resize(img, (mark_w, mark_h), interpolation=cv2.INTER_NEAREST)
-        # img = sly.image.resize_inter_nearest(img, (mark_h, mark_w))
-        img_h, img_w = img.shape[:2]
-
-        # calculate coords
-        offset_x = (self._size_line_2[1] - img_w) // 2
-        x = 3 * self._size_line_2[1] + 4 * self._GAP + offset_x
-        y = int(poster_h - 1.2 * self._GAP - img_h)
-
-        # add logo
-        logo = np.zeros((poster_h, poster_w, 4), dtype=np.uint8)
-        logo[y : y + img_h, x : x + img.shape[1], :3] = img[:, :, :3]
-        logo[y : y + img_h, x : x + img.shape[1], 3] = 255
-
-        self._poster = cv2.addWeighted(self._poster, 0.9, logo, 0.5, 0)
-
-        # or
-        # background = Image.fromarray(self._poster, mode="RGBA")
-        # overlay = Image.fromarray(logo, mode="RGBA")
-        # overlay = overlay.resize(background.size)
-        # new_image = Image.blend(background, overlay, alpha=0.15)
-        # self._poster = np.array(new_image, dtype=np.uint8)
```

### Comparing `dataset-tools-0.0.8/dataset_tools/image/renders/previews.py` & `dataset-tools-0.0.9/dataset_tools/image/renders/previews.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.8/dataset_tools/image/renders/separated_anns_grid.py` & `dataset-tools-0.0.9/dataset_tools/image/renders/separated_anns_grid.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,144 +1,175 @@
 import os
 import random
 from typing import Union
 
+import cv2
 import numpy as np
 from tqdm import tqdm
 
 import supervisely as sly
+from dataset_tools.image.renders.convert import compress_png
 
 
 class SideAnnotationsGrid:
     def __init__(
         self,
         project: Union[str, int],
         project_meta: sly.ProjectMeta,
         api: sly.Api = None,
         rows: int = 3,
         cols: int = 3,
+        side_overlay_path: str = "side_logo_overlay.png",
+        force: bool = False,
     ):
+        self.force = force
         self.project_meta = project_meta
 
-        self._max_size = 1920
+        self._img_height = 1080
         self._rows = rows
         self._cols = cols
-        self._aspect_ratio = 9 / 16
+        self._row_width = 0
+        self._gap = 15
+        self._bg_color = (221, 210, 230)  # rgb(221, 210, 230)
+        self._side_overlay_path = side_overlay_path
 
-        height, width, piece_h, piece_w = self._calculate_shapes()
-        self._grid_size = (height, width)
-        self._piece_size = (piece_h, piece_w)
+        self._local = False if isinstance(project, int) else True
+        self._api = api if api is not None else sly.Api.from_env()
 
-        self._all_image_infos = []
-        self._all_anns = []
         self.np_images = []
-        self.original_masks = []
-        self._grid = None
+        self._img_array = None
+        self._row_height = int((self._img_height - self._gap * (self._rows + 1)) / self._rows)
 
-        self._local = False if isinstance(project, int) else True
-        self._api = api if api is not None else sly.Api.from_env()
+    @property
+    def basename_stem(self) -> None:
+        return sly.utils.camel_to_snake(self.__class__.__name__)
 
     def update(self, data: tuple):
         cnt = self._cols * self._rows
         join_data = [(ds, img, ann) for ds, list1, list2 in data for img, ann in zip(list1, list2)]
 
         random.shuffle(join_data)
         with tqdm(desc="Downloading images", total=cnt) as p:
             for ds, img_info, ann in join_data[:cnt]:
-                self._all_image_infos.append(img_info)
-                self._all_anns.append(ann)
-                self.np_images.append(
+                img = (
                     sly.image.read(ds.get_img_path(img_info.name))
                     if self._local
                     else self._api.image.download_np(img_info.id)
                 )
-                p.update(1)
-
-                self.original_masks.append(self._draw_masks_on_single_image(ann, img_info))
-
-        resized_images = self._resize_images(self.np_images)
-        resized_masks = self._resize_images(self.original_masks)
+                mask = self._draw_masks_on_single_image(ann, img_info)
 
-        img = self._create_image_grid(
-            [i for pair in zip(resized_images, resized_masks) for i in pair]
-        )
-        self._grid = img
+                img = self._resize_image(img)
+                mask = self._resize_image(mask)
+                join_image = np.hstack([img, mask])
+                self.np_images.append(join_image)
 
-    def to_image(self, path: str = None):
-        if path is None:
-            storage_dir = sly.app.get_data_dir()
-            sly.fs.clean_dir(storage_dir)
-            path = os.path.join(storage_dir, "separated_images_grid.jpeg")
-        sly.image.write(path, self._grid)
-        sly.logger.info(f"Result grid saved to: {path}")
-
-    def _calculate_shapes(
-        self,
-    ):
-        height = width = self._max_size
-        if self._rows > self._cols * 2:
-            piece_h = height // self._rows
-            piece_w = int(max(1, piece_h / self._aspect_ratio))
-        else:
-            piece_w = width // (self._cols * 2)
-            piece_h = int(max(1, piece_w * self._aspect_ratio))
-        height, width = piece_h * self._rows, piece_w * self._cols * 2
-
-        sly.logger.info(f"Result image size is ({height}, {width})")
-        return height, width, piece_h, piece_w
-
-    def _resize_images(self, images):
-        h, w = self._piece_size
-        resized_images = []
-
-        for img in images:
-            img_h, img_w = img.shape[:2]
-            src_ratio = w / h
-            img_ratio = img_w / img_h
-            if img_ratio == src_ratio:
-                img = sly.image.resize(img, (h, w))
-            else:
-                if img_ratio < src_ratio:
-                    img_h, img_w = int((w * img_h) // img_w), w
-                else:
-                    img_h, img_w = h, int((h * img_w) // img_h)
-                img = sly.image.resize(img, (img_h, img_w))
-                crop_rect = sly.Rectangle(
-                    top=(img_h - h) // 2,
-                    left=(img_w - w) // 2,
-                    bottom=(img_h + h) // 2,
-                    right=(img_w + w) // 2,
-                )
-                img = sly.image.crop_with_padding(img, crop_rect)
-                img = sly.image.resize(img, (h, w))
-
-            resized_images.append(img)
-
-        sly.logger.info(f"{len(resized_images)} images resized to {self._piece_size}")
-        return resized_images
+                p.update(1)
 
     def _draw_masks_on_single_image(self, ann: sly.Annotation, image: sly.ImageInfo):
         height, width = image.height, image.width
         mask_img = np.zeros((height, width, 3), dtype=np.uint8)
-        mask_img[:, :, 0:3] = (165, 180, 180)  # rgb(165, 180, 180)
+        mask_img[:, :, 0:3] = self._bg_color  # rgb(221, 210, 230)
 
         for label in ann.labels:
-            random_rgb = sly.color.random_rgb()
-            label.geometry.draw(mask_img, random_rgb, thickness=3)
+            label.geometry.draw(mask_img, color=label.obj_class.color, thickness=3)
 
         return mask_img
 
-    def _create_image_grid(self, images):
-        img_h, img_w = images[0].shape[:2]
-        num = len(images)
-        grid_h, grid_w = self._grid_size
-
-        grid = np.zeros(
-            [grid_h, grid_w, 3],
-            dtype=np.uint8,
-        )
-        for idx in range(num):
-            x = (idx % (self._cols * 2)) * img_w
-            y = (idx // (self._cols * 2)) * img_h
-            grid[y : y + img_h, x : x + img_w, ...] = images[idx][:, :, ...]
+    def to_image(self, path: str = None):
+        path_part, ext = os.path.splitext(path)
+        tmp_path = f"{path_part}-o{ext}"
+        if path is None:
+            storage_dir = sly.app.get_data_dir()
+            path = os.path.join(storage_dir, "horizontal_grid.png")
+
+        self._merge_canvas_with_images()
+        self._add_overlay_with_logo()
+
+        sly.image.write(tmp_path, self._img_array)
+        compress_png(tmp_path, path)
+        sly.fs.silent_remove(tmp_path)
+        sly.logger.info(f"Result grid saved to: {path}")
+
+    def _create_image_canvas(self):
+        self._img_array = np.ones([self._img_height, self._row_width, 3], dtype=np.uint8) * 255
 
-        return grid
+    def _merge_canvas_with_images(self):
+        rows = self._create_rows()
+        self._create_image_canvas()
+        rows = self._merge_img_in_rows(rows)
+        for i, image in enumerate(rows):
+            if image.shape[1] > self._img_array.shape[1]:
+                image = image[:, : self._img_array.shape[1] - self._gap]
+
+            row_start = i * (self._row_height + self._gap) + self._gap
+            row_end = row_start + self._row_height
+            column_start = self._gap
+            column_end = self._img_array.shape[1]
+
+            self._img_array[row_start:row_end, column_start:column_end] = image
+
+    def _create_rows(self):
+        num_images = len(self.np_images)
+        image_widths = [image.shape[1] for image in self.np_images]
+
+        one_big_row_width = sum(image_widths) + (num_images - 1) * self._gap
+        self._row_width = one_big_row_width // self._rows
+
+        rows = []
+        row_images = []
+        current_width = 0
+
+        for image, width in zip(self.np_images, image_widths):
+            if current_width + width > self._row_width:
+                row_images.append(image)
+                rows.append(row_images)
+
+                row_images = []
+                current_width = 0
+
+            row_images.append(image)
+            current_width += width + self._gap
+
+        if len(rows) == self._rows:
+            return rows
+        return rows
+
+    def _merge_img_in_rows(self, rows):
+        combined_rows = []
+        separator = np.ones((self._row_height, 15, 3), dtype=np.uint8) * 255
+        for row in rows:
+            combined_images = []
+
+            for image in row:
+                combined_images.append(image)
+                combined_images.append(separator)
+            combined_images.pop()
+            combined_image = np.hstack(combined_images)
+            combined_rows.append(combined_image)
+
+        return combined_rows
+
+    def _resize_image(self, image):
+        img_h, img_w = image.shape[:2]
+        img_aspect_ratio = self._row_height / img_h
+        img_h = int(self._row_height)
+        img_w = int(img_aspect_ratio * img_w)
+
+        image = sly.image.resize(image, (img_h, img_w))
+
+        return image
+
+    def _add_overlay_with_logo(self):
+        image2 = cv2.imread(self._side_overlay_path, cv2.IMREAD_UNCHANGED)
+        image2 = cv2.cvtColor(image2, cv2.COLOR_BGRA2RGBA)
+
+        _, width1 = self._img_array.shape[:2]
+        height2, width2 = image2.shape[:2]
+
+        alpha_channel = image2[:, :, 3] / 255.0
+
+        x = width1 - width2
+
+        region = self._img_array[:height2, x : x + width2]
+        self._img_array[:height2, x : x + width2, :3] = (
+            1 - alpha_channel[:, :, np.newaxis]
+        ) * region + alpha_channel[:, :, np.newaxis] * image2[:, :, :3]
```

### Comparing `dataset-tools-0.0.8/dataset_tools/image/renders/wrapper.py` & `dataset-tools-0.0.9/dataset_tools/image/renders/wrapper.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,42 +18,49 @@
         dataset: sly.Dataset
         k = min(
             sample_cnt // len(datasets),
             (dataset.items_count if isinstance(project, int) else len(os.listdir(dataset.ann_dir))),
         )
 
         ds_images = (
-            api.image.get_list(dataset.id)
+            api.image.get_list(
+                dataset.id,
+                filters=[{"field": "labelsCount", "operator": ">", "value": 0}],
+            )
             if isinstance(project, int)
             else [
                 dataset.get_image_info(sly.fs.get_file_name(img))
                 for img in os.listdir(dataset.ann_dir)
+                if dataset.get_image_info(sly.fs.get_file_name(img)).labels_count > 0
             ]
         )
 
         s = random.sample(ds_images, min(k, len(ds_images)))
         anns = (
             [
-                sly.Annotation.from_json(ann.annotation, meta)
-                for ann in api.annotation.get_list(
+                sly.Annotation.from_json(ann_json, meta)
+                for ann_json in api.annotation.download_json_batch(
                     dataset.id,
-                    filters=[{"field": "imageId", "operator": "in", "value": [item.id for item in s]}],
+                    [item.id for item in s],
                 )
             ]
             if isinstance(project, int)
             else [dataset.get_ann(img.name, meta) for img in s]
         )
         samples.append((dataset, s, anns))
         total += k
     return samples, total
 
 
 def prepare_renders(
     project: Union[int, str], renderers: list, sample_cnt: int = 25, api: sly.Api = None
 ) -> None:
+    if len(renderers) == 0:
+        print("Passed 'renderers' parameter is empty. Enable 'force' flag to overwrite renderers output file. Skipping renderers preparation...")
+        return
     if api is None:
         api = sly.Api.from_env()
     if isinstance(project, int):
         project_meta = sly.ProjectMeta.from_json(api.project.get_meta(project))
         datasets = api.dataset.get_list(project)
     elif isinstance(project, str):
         project_fs = sly.Project(project, sly.OpenMode.READ)
```

### Comparing `dataset-tools-0.0.8/dataset_tools/image/stats/class_balance.py` & `dataset-tools-0.0.9/dataset_tools/image/stats/class_balance.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,39 @@
-import itertools
-import os
-import random
-from collections import defaultdict
-from copy import deepcopy
 from typing import Dict
 
-import dataframe_image as dfi
 import numpy as np
-import pandas as pd
 import supervisely as sly
 
 from dataset_tools.image.stats.basestats import BaseStats
 
 UNLABELED_COLOR = [0, 0, 0]
 
 
 class ClassBalance(BaseStats):
     """
     Columns:
-        class name
-        images
-        objects
-        avg count per image
-        avg area per image
+        Class
+        Images
+        Objects
+        Avg count per image
+        Avg area per image
     """
 
-    def __init__(self, project_meta: sly.ProjectMeta) -> None:
+    def __init__(self, project_meta: sly.ProjectMeta, force:bool=False) -> None:
         self._meta = project_meta
         self._stats = {}
+        self.force = force
 
-        self._class_names = []  # ["unlabeled"]
-        class_colors = []  # [UNLABELED_COLOR]
-        class_indices_colors = []  # [UNLABELED_COLOR]
+        self._class_names = []
+        class_colors = []
+        class_indices_colors = []
         self._name_to_index = {}
         for idx, obj_class in enumerate(self._meta.obj_classes):
             self._class_names.append(obj_class.name)
             class_colors.append(obj_class.color)
-            # class_index = idx + 1 # unlabeled
             class_indices_colors.append([idx, idx, idx])
             self._name_to_index[obj_class.name] = idx
 
         self._stats["class_names"] = self._class_names
         self._stats["class_indices_colors"] = class_indices_colors
         self._stats["_name_to_index"] = self._name_to_index
 
@@ -61,17 +54,14 @@
         ann.draw_class_idx_rgb(render_idx_rgb, self._stats["_name_to_index"])
 
         stat_area = sly.Annotation.stat_area(
             render_idx_rgb, self._stats["class_names"], self._stats["class_indices_colors"]
         )
         stat_count = ann.stat_class_count(self._stats["class_names"])
 
-        # if stat_area["unlabeled"] > 0:
-        # stat_count["unlabeled"] = 1
-
         for idx, class_name in enumerate(self._stats["class_names"]):
             cur_area = stat_area[class_name] if not np.isnan(stat_area[class_name]) else 0
             cur_count = stat_count[class_name] if not np.isnan(stat_count[class_name]) else 0
 
             self._stats["sum_class_area_per_image"][idx] += cur_area
             self._stats["objects_count"][idx] += cur_count
             self._stats["images_count"][idx] += 1 if stat_count[class_name] > 0 else 0
@@ -80,26 +70,23 @@
                 self._stats["avg_nonzero_area"][idx] = (
                     self._stats["sum_class_area_per_image"][idx] / self._stats["images_count"][idx]
                 )
                 self._stats["avg_nonzero_count"][idx] = (
                     self._stats["objects_count"][idx] / self._stats["images_count"][idx]
                 )
 
-            # if class_name == "unlabeled":
-            #     continue
-            # elif stat_count[class_name] > 0:
             if stat_count[class_name] > 0:
                 self._stats["image_counts_filter_by_id"][idx].append(image.id)
 
             # TODO: implement later
             # if stat_count[class_name] > 0:
             # obj_ids = [obj[0] for obj in ann_objects if obj[1] == class_name]
             # self._stats["object_counts_filter_by_id"][idx].extend(obj_ids)
 
-    def to_json(self) -> dict:
+    def to_json(self) -> Dict:
         columns = [
             "Class",
             "Images",
             "Objects",
             "Count on image",
             "Area on image",
         ]
```

### Comparing `dataset-tools-0.0.8/dataset_tools/image/stats/class_cooccurrence.py` & `dataset-tools-0.0.9/dataset_tools/image/stats/class_cooccurrence.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,85 +1,89 @@
-import itertools
-import os
-import random
 from collections import defaultdict
-from copy import deepcopy
 from typing import Dict
 
-import dataframe_image as dfi
 import numpy as np
-import pandas as pd
 import supervisely as sly
 
 from dataset_tools.image.stats.basestats import BaseStats
-from supervisely.app.widgets import ConfusionMatrix
+
+# from supervisely.app.widgets import ConfusionMatrix
 
 
 class ClassCooccurrence(BaseStats):
     """
     Columns:
-        class name
+        Class
         class 1
         class 2
         etc.
     """
 
-    def __init__(self, project_meta: sly.ProjectMeta) -> None:
+    def __init__(self, project_meta: sly.ProjectMeta, force:bool = False) -> None:
         self._meta = project_meta
         self._stats = {}
+        self.force = force
+
+        self._name_to_index = {}
+
+        for idx, obj_class in enumerate(self._meta.obj_classes):
+            self._name_to_index[obj_class.name] = idx
 
         self._class_names = [cls.name for cls in project_meta.obj_classes]
         self._references = defaultdict(lambda: defaultdict(list))
 
         num_classes = len(self._class_names)
         self.co_occurrence_matrix = np.zeros((num_classes, num_classes), dtype=int)
 
-    def update(self, image: sly.ImageInfo, ann: sly.Annotation):
+    def update(self, image: sly.ImageInfo, ann: sly.Annotation) -> None:
         classes = set()
         for label in ann.labels:
             classes.add(label.obj_class.name)
 
-        classes = list(classes)
         for class_ in classes:
-            idx = self._class_names.index(class_)
+            idx = self._name_to_index[class_]
             self.co_occurrence_matrix[idx][idx] += 1
             self._references[idx][idx].append(image.id)
 
+        classes = list(classes)
         for i in range(len(classes)):
             for j in range(i + 1, len(classes)):
                 class_i = classes[i]
                 class_j = classes[j]
-                idx_i = list(self._class_names).index(class_i)
-                idx_j = list(self._class_names).index(class_j)
+                idx_i = self._name_to_index[class_i]
+                idx_j = self._name_to_index[class_j]
                 self.co_occurrence_matrix[idx_i][idx_j] += 1
                 self.co_occurrence_matrix[idx_j][idx_i] += 1
 
                 self._references[idx_i][idx_j].append(image.id)
                 self._references[idx_j][idx_i].append(image.id)
 
-    def to_json(self):
-        options = {"fixColumns": 1}
+    def to_json(self) -> Dict:
+        options = {
+            "fixColumns": 1,  # not used in Web
+            "cellTooltip": "Click to preview. {currentCell} images have objects of both classes {firstCell} and {currentColumn} at the same time",
+        }
         colomns_options = [None] * (len(self._class_names) + 1)
-        colomns_options[0] = {"type": "class"}
+        colomns_options[0] = {"type": "class"}  # not used in Web
 
         for idx in range(1, len(colomns_options)):
             colomns_options[idx] = {"maxValue": int(np.max(self.co_occurrence_matrix[:, idx - 1]))}
 
         data = [
             [value] + sublist
             for value, sublist in zip(self._class_names, self.co_occurrence_matrix.tolist())
         ]
 
         res = {
-            "columns": ["class name"] + self._class_names,
+            "columns": ["Class"] + self._class_names,
             "data": data,
-            "referencesRow": self._references,
+            "referencesCell": self._references,  # row - col
             "options": options,
             "colomnsOptions": colomns_options,
         }
         return res
 
-    def get_widget(self) -> ConfusionMatrix:
-        df = pd.DataFrame(data=self.co_occurrence_matrix.tolist(), columns=self._class_names)
-        confusion_matrix = ConfusionMatrix()
-        confusion_matrix.read_pandas(df)
-        return confusion_matrix
+    # def get_widget(self) -> ConfusionMatrix:
+    #     df = pd.DataFrame(data=self.co_occurrence_matrix.tolist(), columns=self._class_names)
+    #     confusion_matrix = ConfusionMatrix()
+    #     confusion_matrix.read_pandas(df)
+    #     return confusion_matrix
```

### Comparing `dataset-tools-0.0.8/dataset_tools/image/stats/object_and_class_sizes.py` & `dataset-tools-0.0.9/dataset_tools/image/stats/object_and_class_sizes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,92 +1,128 @@
+from typing import Dict, List
 from collections import defaultdict
 
 import supervisely as sly
+from supervisely.app.widgets import TreemapChart
 
 from dataset_tools.image.stats.basestats import BaseStats
 
 
 class ObjectSizes(BaseStats):
     """
     Columns:
-        Class name
+        Object ID
+        Class
         Dataset ID
         Image name
         Image size
         Height px
         Height %
         Width px
         Width %
-        Area px
         Area %
     """
 
-    def __init__(self, project_meta: sly.ProjectMeta):
+    def __init__(
+        self,
+        project_meta: sly.ProjectMeta,
+        datasets: List[sly.DatasetInfo] = None,
+        force: bool = False,
+    ):
+        self.force = force
         self.project_meta = project_meta
+        self._dataset_id_to_name = None
+        if datasets is not None:
+            self._dataset_id_to_name = {ds.id: ds.name for ds in datasets}
         self._stats = []
+        self._object_id = 1
 
-    def update(self, image: sly.ImageInfo, ann: sly.Annotation):
+    def update(self, image: sly.ImageInfo, ann: sly.Annotation) -> None:
         image_height, image_width = ann.img_size
 
         for label in ann.labels:
             if type(label.geometry) not in [sly.Bitmap, sly.Rectangle, sly.Polygon]:
                 continue
 
+            object_id = self._object_id
+            self._object_id += 1
+
             object_data = {
-                "class_name": label.obj_class.name,
-                "dataset_id": image.dataset_id,
+                "object_id": object_id,
+                "class": label.obj_class.name,
                 "image_name": image.name,
-                "image_size_hw": f"{image_height}x{image_width}",
             }
 
+            if self._dataset_id_to_name:
+                dataset_name = self._dataset_id_to_name[image.dataset_id]
+                object_data["dataset_name"] = dataset_name
+
+            object_data["image_size_hw"] = f"{image_height} x {image_width}"
+
             object_data.update(calculate_obj_sizes(label, image_height, image_width))
 
             object_data = list(object_data.values())
 
-            self._stats.append(object_data)
+            self._stats.append((object_data, [image.id]))
+
+    def to_json(self) -> Dict:
+        options = {
+            "sort": {"columnIndex": 0, "order": "asc"},
+        }
+
+        columns = [
+            "Object ID",
+            "Class",
+            "Image name",
+            "Image size",
+            "Height",
+            "Height",
+            "Width",
+            "Width",
+            "Area",
+        ]
+
+        columns_options = [
+            {"tooltip": "ID of the object in instance"},
+            {"type": "class"},
+            {"subtitle": "click row to open"},
+            {"subtitle": "height x width"},
+            {"postfix": "px"},
+            {"postfix": "%"},
+            {"postfix": "px"},
+            {"postfix": "%"},
+            {"postfix": "%"},
+        ]
+
+        if self._dataset_id_to_name:
+            columns.insert(3, "Split")
+            columns_options.insert(
+                3,
+                {
+                    "subtitle": "folder name",
+                },
+            )
 
-    def to_json(self):
-        options = {"fixColumns": 1}
+        data, references_row = zip(*self._stats)
 
         res = {
-            "columns": [
-                "Class name",
-                "Dataset ID",
-                "Image name",
-                "Image size",
-                "Height",
-                "Height",
-                "Width",
-                "Width",
-                "Area",
-                "Area",
-            ],
-            "columnsOptions": [
-                {},
-                {},
-                {},
-                {},
-                {"postfix": "px"},
-                {"postfix": "%"},
-                {"postfix": "px"},
-                {"postfix": "%"},
-                {"postfix": "px"},
-                {"postfix": "%"},
-            ],
-            "data": self._stats,
+            "columns": columns,
+            "columnsOptions": columns_options,
+            "data": data,
             "options": options,
+            "referencesRow": references_row,
         }
 
         return res
 
 
 class ClassSizes(BaseStats):
     """
     Columns:
-        Class name
+        Class
         Object count
         Min height px
         Min height %
         Max height px
         Max height %
         Avg height px
         Avg height %
@@ -100,31 +136,31 @@
         Min area %
         Max area px
         Max area %
         Avg area px
         Avg area %
     """
 
-    def __init__(self, project_meta):
+    def __init__(self, project_meta: sly.ProjectMeta, force: bool = False):
+        self.force = force
         self.project_meta = project_meta
         self._class_titles = [obj_class.name for obj_class in project_meta.obj_classes]
 
         self._data = []
 
-    def update(self, image: sly.ImageInfo, ann: sly.Annotation):
+    def update(self, image: sly.ImageInfo, ann: sly.Annotation) -> None:
         self._data.append(ann)
 
-    def to_json(self):
+    def to_json(self) -> Dict:
         stats = []
 
         class_heights_px = defaultdict(list)
         class_heights_pc = defaultdict(list)
         class_widths_px = defaultdict(list)
         class_widths_pc = defaultdict(list)
-        class_areas_px = defaultdict(list)
         class_areas_pc = defaultdict(list)
         class_object_counts = defaultdict(int)
 
         for ann in self._data:
             image_height, image_width = ann.img_size
             for label in ann.labels:
                 if type(label.geometry) not in [sly.Bitmap, sly.Rectangle, sly.Polygon]:
@@ -134,123 +170,177 @@
 
                 obj_sizes = calculate_obj_sizes(label, image_height, image_width)
 
                 class_heights_px[label.obj_class.name].append(obj_sizes["height_px"])
                 class_heights_pc[label.obj_class.name].append(obj_sizes["height_pc"])
                 class_widths_px[label.obj_class.name].append(obj_sizes["width_px"])
                 class_widths_pc[label.obj_class.name].append(obj_sizes["width_pc"])
-                class_areas_px[label.obj_class.name].append(obj_sizes["area_px"])
                 class_areas_pc[label.obj_class.name].append(obj_sizes["area_pc"])
 
         for class_title in self._class_titles:
             object_count = class_object_counts[class_title]
 
             if object_count < 1:
                 continue
 
             class_data = {
                 "class_name": class_title,
                 "object_count": object_count,
+                "avg_area_pc": round(
+                    sum(class_areas_pc[class_title]) / len(class_areas_pc[class_title]),
+                    2,
+                ),
+                "max_area_pc": max(class_areas_pc[class_title]),
+                "min_area_pc": min(class_areas_pc[class_title]),
                 "min_height_px": min(class_heights_px[class_title]),
                 "min_height_pc": min(class_heights_pc[class_title]),
                 "max_height_px": max(class_heights_px[class_title]),
                 "max_height_pc": max(class_heights_pc[class_title]),
                 "avg_height_px": round(
                     sum(class_heights_px[class_title]) / len(class_heights_px[class_title]),
-                    2,
                 ),
                 "avg_height_pc": round(
                     sum(class_heights_pc[class_title]) / len(class_heights_pc[class_title]),
                     2,
                 ),
                 "min_width_px": min(class_widths_px[class_title]),
                 "min_width_pc": min(class_widths_pc[class_title]),
                 "max_width_px": max(class_widths_px[class_title]),
                 "max_width_pc": max(class_widths_pc[class_title]),
                 "avg_width_px": round(
                     sum(class_widths_px[class_title]) / len(class_widths_px[class_title]),
-                    2,
                 ),
                 "avg_width_pc": round(
                     sum(class_widths_pc[class_title]) / len(class_widths_pc[class_title]),
                     2,
                 ),
-                "min_area_px": min(class_areas_px[class_title]),
-                "min_area_pc": min(class_areas_pc[class_title]),
-                "max_area_px": max(class_areas_px[class_title]),
-                "max_area_pc": max(class_areas_pc[class_title]),
-                "avg_area_px": round(
-                    sum(class_areas_px[class_title]) / len(class_areas_px[class_title]),
-                    2,
-                ),
-                "avg_area_pc": round(
-                    sum(class_areas_pc[class_title]) / len(class_areas_pc[class_title]),
-                    2,
-                ),
             }
 
             class_data = list(class_data.values())
 
             stats.append(class_data)
 
-        options = {"fixColumns": 1}
+        options = {
+            "fixColumns": 1,
+            "sort": {"columnIndex": 1, "order": "desc"},
+            "pageSize": len(self._class_titles),
+        }
 
         res = {
             "columns": [
-                "Class name",
+                "Class",
                 "Object count",
+                "Avg area",
+                "Max area",
+                "Min area",
                 "Min height",
                 "Min height",
                 "Max height",
                 "Max height",
                 "Avg height",
                 "Avg height",
                 "Min width",
                 "Min width",
                 "Max width",
                 "Max width",
                 "Avg width",
                 "Avg width",
-                "Min area",
-                "Min area",
-                "Max area",
-                "Max area",
-                "Avg area",
-                "Avg area",
             ],
             "columnsOptions": [
-                {},
-                {},
-                {"postfix": "px"},
-                {"postfix": "%"},
-                {"postfix": "px"},
-                {"postfix": "%"},
+                {"type": "class"},
+                {"maxValue": max([class_data[1] for class_data in stats])},
+                {"postfix": "%", "tooltip": "Average object area in percents of all image."},
+                {"postfix": "%", "tooltip": "Maximum object area in percents of all image."},
+                {"postfix": "%", "tooltip": "Minimum object area in percents of all image."},
                 {"postfix": "px"},
-                {"postfix": "%"},
+                {"postfix": "%", "tooltip": "Minimum object height in percents of image height."},
                 {"postfix": "px"},
-                {"postfix": "%"},
+                {"postfix": "%", "tooltip": "Maximum object height in percents of image height."},
                 {"postfix": "px"},
-                {"postfix": "%"},
+                {"postfix": "%", "tooltip": "Average object height in percents of image height."},
                 {"postfix": "px"},
-                {"postfix": "%"},
+                {"postfix": "%", "tooltip": "Minimum object width in percents of image width."},
                 {"postfix": "px"},
-                {"postfix": "%"},
+                {"postfix": "%", "tooltip": "Maximum object width in percents of image width."},
                 {"postfix": "px"},
-                {"postfix": "%"},
-                {"postfix": "px"},
-                {"postfix": "%"},
+                {"postfix": "%", "tooltip": "Average object width in percents of image width."},
             ],
             "data": stats,
             "options": options,
         }
 
         return res
 
 
-def calculate_obj_sizes(label, image_height, image_width):
+class ClassTreemap(BaseStats):
+    def __init__(self, project_meta: sly.ProjectMeta, force: bool = False):
+        self.force = force
+        self.project_meta = project_meta
+        self._class_titles = [obj_class.name for obj_class in project_meta.obj_classes]
+        self._class_rgbs = [obj_class.color for obj_class in project_meta.obj_classes]
+        self._class_colors = [rgb_to_hex(rgb) for rgb in self._class_rgbs]
+
+        self._data = []
+
+    def update(self, image: sly.ImageInfo, ann: sly.Annotation) -> None:
+        self._data.append(ann)
+
+    def to_json(self) -> Dict:
+        tooltip = "Average area of class objects on image is {y}%"
+        colors = self._class_colors
+        names = []
+        values = []
+
+        class_areas_pc = defaultdict(list)
+        class_object_counts = defaultdict(int)
+
+        for ann in self._data:
+            image_height, image_width = ann.img_size
+            for label in ann.labels:
+                if type(label.geometry) not in [sly.Bitmap, sly.Rectangle, sly.Polygon]:
+                    continue
+
+                class_object_counts[label.obj_class.name] += 1
+
+                obj_sizes = calculate_obj_sizes(label, image_height, image_width)
+
+                class_areas_pc[label.obj_class.name].append(obj_sizes["area_pc"])
+
+        for class_title in self._class_titles:
+            object_count = class_object_counts[class_title]
+
+            if object_count < 1:
+                continue
+
+            names.append(class_title)
+            values.append(
+                round(
+                    sum(class_areas_pc[class_title]) / len(class_areas_pc[class_title]),
+                    2,
+                )
+            )
+
+        tc = TreemapChart(
+            title="Average area of class objects on image",
+            colors=colors,
+            tooltip=tooltip,
+        )
+
+        tc.set_series(names, values)
+
+        res = tc.get_json_data()
+
+        return res
+
+
+def rgb_to_hex(rgb: List[int]) -> str:
+    return "#{:02x}{:02x}{:02x}".format(*rgb)
+
+
+def calculate_obj_sizes(label: sly.Label, image_height: int, image_width: int) -> Dict:
     image_area = image_height * image_width
 
     rect_geometry = label.geometry.to_bbox()
 
     height_px = rect_geometry.height
     height_pc = round(height_px * 100.0 / image_height, 2)
 
@@ -261,10 +351,9 @@
     area_pc = round(area_px * 100.0 / image_area, 2)
 
     return {
         "height_px": height_px,
         "height_pc": height_pc,
         "width_px": width_px,
         "width_pc": width_pc,
-        "area_px": area_px,
         "area_pc": area_pc,
     }
```

### Comparing `dataset-tools-0.0.8/dataset_tools.egg-info/PKG-INFO` & `dataset-tools-0.0.9/dataset_tools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset-tools
-Version: 0.0.8
+Version: 0.0.9
 Summary: Dataset tools for dataset ninja made by Supervisely team.
 Home-page: https://github.com/supervisely/dataset-tools
 Author: Supervisely
 Author-email: support@supervise.ly
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dataset-tools-0.0.8/dataset_tools.egg-info/SOURCES.txt` & `dataset-tools-0.0.9/dataset_tools.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,40 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 dataset_tools/__init__.py
+dataset_tools/download.py
 dataset_tools.egg-info/PKG-INFO
 dataset_tools.egg-info/SOURCES.txt
 dataset_tools.egg-info/dependency_links.txt
 dataset_tools.egg-info/requires.txt
 dataset_tools.egg-info/top_level.txt
+dataset_tools/convert/__init__.py
+dataset_tools/convert/cityscapes/__init__.py
+dataset_tools/convert/cityscapes/main.py
+dataset_tools/convert/coco/__init__.py
+dataset_tools/convert/coco/main.py
+dataset_tools/convert/pascal/__init__.py
+dataset_tools/convert/pascal/main.py
 dataset_tools/image/__init__.py
 dataset_tools/image/renders/__init__.py
+dataset_tools/image/renders/convert.py
+dataset_tools/image/renders/horizontal_grid.py
 dataset_tools/image/renders/poster.py
 dataset_tools/image/renders/previews.py
 dataset_tools/image/renders/separated_anns_grid.py
+dataset_tools/image/renders/vertical_grid.py
 dataset_tools/image/renders/wrapper.py
 dataset_tools/image/stats/__init__.py
 dataset_tools/image/stats/basestats.py
 dataset_tools/image/stats/class_balance.py
 dataset_tools/image/stats/class_cooccurrence.py
 dataset_tools/image/stats/classes_per_image.py
 dataset_tools/image/stats/heatmaps_for_classes.py
 dataset_tools/image/stats/object_and_class_sizes.py
 dataset_tools/image/stats/objects_distribution.py
-dataset_tools/image/stats/wrapper.py
+dataset_tools/image/stats/preview_for_classes.py
+dataset_tools/image/stats/wrapper.py
+dataset_tools/text/__init__.py
+dataset_tools/text/summary/__init__.py
+dataset_tools/text/summary/generate.py
```

### Comparing `dataset-tools-0.0.8/setup.py` & `dataset-tools-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     # "MarkupSafe>=2.1.1, <3.0.0",
     # "arel>=0.2.0, <1.0.0",
     "tqdm>=4.62.3, <5.0.0",
     "pandas>=1.1.3, <=1.5.2",  # For compatibility with Python3.7
     "matplotlib>=3.3.2, <4.0.0",
     "scikit-image>=0.17.1, <1.0.0",
     "dataframe_image>=0.1.11, <1.0.0",
+    "inflect>=6.0.0",
     # "async_asgi_testclient",
     # "PyYAML",
     # "distinctipy",
     # "beautifulsoup4",
     # "numerize",
     # "ffmpeg-python==0.2.0",
     # "python-multipart==0.0.5",
```

