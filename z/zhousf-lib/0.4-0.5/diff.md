# Comparing `tmp/zhousf-lib-0.4.tar.gz` & `tmp/zhousf-lib-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhousf-lib-0.4.tar", last modified: Tue Jun  6 06:06:45 2023, max compression
+gzip compressed data, was "zhousf-lib-0.5.tar", last modified: Tue Jun  6 06:13:24 2023, max compression
```

## Comparing `zhousf-lib-0.4.tar` & `zhousf-lib-0.5.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 06:06:45.015116 zhousf-lib-0.4/
--rw-rw-rw-   0        0        0     1086 2023-06-06 02:24:10.000000 zhousf-lib-0.4/LICENSE
--rw-rw-rw-   0        0        0      672 2023-06-06 06:06:45.015116 zhousf-lib-0.4/PKG-INFO
--rw-rw-rw-   0        0        0       36 2023-06-06 02:24:10.000000 zhousf-lib-0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 06:06:44.974086 zhousf-lib-0.4/core/
--rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.4/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 06:06:44.975086 zhousf-lib-0.4/core/font/
--rw-rw-rw-   0        0        0      873 2023-06-06 02:39:11.000000 zhousf-lib-0.4/core/font/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 06:06:44.989085 zhousf-lib-0.4/core/util/
--rw-rw-rw-   0        0        0       84 2023-06-06 02:39:11.000000 zhousf-lib-0.4/core/util/__init__.py
--rw-rw-rw-   0        0        0     2795 2023-06-06 02:39:11.000000 zhousf-lib-0.4/core/util/calculater_util.py
--rw-rw-rw-   0        0        0      709 2023-06-06 02:39:10.000000 zhousf-lib-0.4/core/util/cv_util.py
--rw-rw-rw-   0        0        0     2220 2023-06-06 02:39:11.000000 zhousf-lib-0.4/core/util/encrypt_util.py
--rw-rw-rw-   0        0        0      492 2023-06-06 02:39:11.000000 zhousf-lib-0.4/core/util/except_util.py
--rw-rw-rw-   0        0        0     1359 2023-06-06 02:48:08.000000 zhousf-lib-0.4/core/util/img_util.py
--rw-rw-rw-   0        0        0     1116 2023-06-06 02:39:11.000000 zhousf-lib-0.4/core/util/interceptor_util.py
--rw-rw-rw-   0        0        0    12953 2023-06-06 02:39:11.000000 zhousf-lib-0.4/core/util/iou_util.py
--rw-rw-rw-   0        0        0     3129 2023-06-06 02:39:11.000000 zhousf-lib-0.4/core/util/log_util.py
--rw-rw-rw-   0        0        0     1812 2023-06-06 02:39:10.000000 zhousf-lib-0.4/core/util/pdf_util.py
--rw-rw-rw-   0        0        0     1385 2023-06-06 02:39:10.000000 zhousf-lib-0.4/core/util/permission_util.py
--rw-rw-rw-   0        0        0      658 2023-06-06 02:39:10.000000 zhousf-lib-0.4/core/util/re_util.py
--rw-rw-rw-   0        0        0      805 2023-06-06 02:39:11.000000 zhousf-lib-0.4/core/util/string_util.py
--rw-rw-rw-   0        0        0     4687 2023-06-06 02:39:10.000000 zhousf-lib-0.4/core/util/time_util.py
-drwxrwxrwx   0        0        0        0 2023-06-06 06:06:44.992085 zhousf-lib-0.4/datasets/
--rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.4/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 06:06:45.001085 zhousf-lib-0.4/datasets/coco/
--rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.4/datasets/coco/__init__.py
--rw-rw-rw-   0        0        0     8244 2023-06-06 02:42:48.000000 zhousf-lib-0.4/datasets/coco/coco_bbox_extract.py
--rw-rw-rw-   0        0        0     5813 2023-06-06 02:40:04.000000 zhousf-lib-0.4/datasets/coco/coco_bbox_update.py
--rw-rw-rw-   0        0        0     6557 2023-06-06 02:43:29.000000 zhousf-lib-0.4/datasets/coco/coco_bbox_vis.py
--rw-rw-rw-   0        0        0     2889 2023-06-06 02:42:48.000000 zhousf-lib-0.4/datasets/coco/coco_dataset_merge.py
--rw-rw-rw-   0        0        0     6077 2023-06-06 02:42:48.000000 zhousf-lib-0.4/datasets/coco/coco_dataset_split.py
-drwxrwxrwx   0        0        0        0 2023-06-06 06:06:45.006086 zhousf-lib-0.4/datasets/labelme/
--rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.4/datasets/labelme/__init__.py
--rw-rw-rw-   0        0        0     8110 2023-06-06 02:48:08.000000 zhousf-lib-0.4/datasets/labelme/labelme_convert_coco.py
--rw-rw-rw-   0        0        0     9583 2023-06-06 02:44:18.000000 zhousf-lib-0.4/datasets/labelme/labelme_convert_seg.py
--rw-rw-rw-   0        0        0     3842 2023-06-06 02:48:08.000000 zhousf-lib-0.4/datasets/labelme/labelme_dataset_clip.py
-drwxrwxrwx   0        0        0        0 2023-06-06 06:06:45.009086 zhousf-lib-0.4/datasets/segmentation/
--rw-rw-rw-   0        0        0       84 2023-06-06 02:48:08.000000 zhousf-lib-0.4/datasets/segmentation/__init__.py
--rw-rw-rw-   0        0        0     2723 2023-06-06 02:48:08.000000 zhousf-lib-0.4/datasets/segmentation/seg_dataset_split.py
--rw-rw-rw-   0        0        0       42 2023-06-06 06:06:45.015116 zhousf-lib-0.4/setup.cfg
--rw-rw-rw-   0        0        0     5715 2023-06-06 06:06:08.000000 zhousf-lib-0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 06:06:45.014086 zhousf-lib-0.4/zhousf_lib.egg-info/
--rw-rw-rw-   0        0        0      672 2023-06-06 06:06:44.000000 zhousf-lib-0.4/zhousf_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      987 2023-06-06 06:06:44.000000 zhousf-lib-0.4/zhousf_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 06:06:44.000000 zhousf-lib-0.4/zhousf_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-06 06:06:44.000000 zhousf-lib-0.4/zhousf_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 06:13:24.073225 zhousf-lib-0.5/
+-rw-rw-rw-   0        0        0     1086 2023-06-06 02:24:10.000000 zhousf-lib-0.5/LICENSE
+-rw-rw-rw-   0        0        0      672 2023-06-06 06:13:24.071253 zhousf-lib-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       36 2023-06-06 02:24:10.000000 zhousf-lib-0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-06 06:13:24.073225 zhousf-lib-0.5/setup.cfg
+-rw-rw-rw-   0        0        0     4098 2023-06-06 06:13:20.000000 zhousf-lib-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:13:24.038249 zhousf-lib-0.5/zhousf_lib.egg-info/
+-rw-rw-rw-   0        0        0      672 2023-06-06 06:13:23.000000 zhousf-lib-0.5/zhousf_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1299 2023-06-06 06:13:23.000000 zhousf-lib-0.5/zhousf_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 06:13:23.000000 zhousf-lib-0.5/zhousf_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-06 06:13:23.000000 zhousf-lib-0.5/zhousf_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 06:13:24.039251 zhousf-lib-0.5/zhousflib/
+-rw-rw-rw-   0        0        0       84 2023-06-06 06:12:25.000000 zhousf-lib-0.5/zhousflib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:13:24.040251 zhousf-lib-0.5/zhousflib/core/
+-rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.5/zhousflib/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:13:24.041220 zhousf-lib-0.5/zhousflib/core/font/
+-rw-rw-rw-   0        0        0      873 2023-06-06 02:39:11.000000 zhousf-lib-0.5/zhousflib/core/font/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:13:24.056221 zhousf-lib-0.5/zhousflib/core/util/
+-rw-rw-rw-   0        0        0       84 2023-06-06 02:39:11.000000 zhousf-lib-0.5/zhousflib/core/util/__init__.py
+-rw-rw-rw-   0        0        0     2795 2023-06-06 02:39:11.000000 zhousf-lib-0.5/zhousflib/core/util/calculater_util.py
+-rw-rw-rw-   0        0        0      709 2023-06-06 02:39:10.000000 zhousf-lib-0.5/zhousflib/core/util/cv_util.py
+-rw-rw-rw-   0        0        0     2220 2023-06-06 02:39:11.000000 zhousf-lib-0.5/zhousflib/core/util/encrypt_util.py
+-rw-rw-rw-   0        0        0      492 2023-06-06 02:39:11.000000 zhousf-lib-0.5/zhousflib/core/util/except_util.py
+-rw-rw-rw-   0        0        0     1359 2023-06-06 02:48:08.000000 zhousf-lib-0.5/zhousflib/core/util/img_util.py
+-rw-rw-rw-   0        0        0     1116 2023-06-06 02:39:11.000000 zhousf-lib-0.5/zhousflib/core/util/interceptor_util.py
+-rw-rw-rw-   0        0        0    12953 2023-06-06 02:39:11.000000 zhousf-lib-0.5/zhousflib/core/util/iou_util.py
+-rw-rw-rw-   0        0        0     3129 2023-06-06 02:39:11.000000 zhousf-lib-0.5/zhousflib/core/util/log_util.py
+-rw-rw-rw-   0        0        0     1812 2023-06-06 02:39:10.000000 zhousf-lib-0.5/zhousflib/core/util/pdf_util.py
+-rw-rw-rw-   0        0        0     1385 2023-06-06 02:39:10.000000 zhousf-lib-0.5/zhousflib/core/util/permission_util.py
+-rw-rw-rw-   0        0        0      658 2023-06-06 02:39:10.000000 zhousf-lib-0.5/zhousflib/core/util/re_util.py
+-rw-rw-rw-   0        0        0      805 2023-06-06 02:39:11.000000 zhousf-lib-0.5/zhousflib/core/util/string_util.py
+-rw-rw-rw-   0        0        0     4687 2023-06-06 02:39:10.000000 zhousf-lib-0.5/zhousflib/core/util/time_util.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:13:24.057221 zhousf-lib-0.5/zhousflib/datasets/
+-rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.5/zhousflib/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:13:24.064222 zhousf-lib-0.5/zhousflib/datasets/coco/
+-rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.5/zhousflib/datasets/coco/__init__.py
+-rw-rw-rw-   0        0        0     8244 2023-06-06 02:42:48.000000 zhousf-lib-0.5/zhousflib/datasets/coco/coco_bbox_extract.py
+-rw-rw-rw-   0        0        0     5813 2023-06-06 02:40:04.000000 zhousf-lib-0.5/zhousflib/datasets/coco/coco_bbox_update.py
+-rw-rw-rw-   0        0        0     6567 2023-06-06 06:12:25.000000 zhousf-lib-0.5/zhousflib/datasets/coco/coco_bbox_vis.py
+-rw-rw-rw-   0        0        0     2889 2023-06-06 02:42:48.000000 zhousf-lib-0.5/zhousflib/datasets/coco/coco_dataset_merge.py
+-rw-rw-rw-   0        0        0     6077 2023-06-06 02:42:48.000000 zhousf-lib-0.5/zhousflib/datasets/coco/coco_dataset_split.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:13:24.068221 zhousf-lib-0.5/zhousflib/datasets/labelme/
+-rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.5/zhousflib/datasets/labelme/__init__.py
+-rw-rw-rw-   0        0        0     8120 2023-06-06 06:12:25.000000 zhousf-lib-0.5/zhousflib/datasets/labelme/labelme_convert_coco.py
+-rw-rw-rw-   0        0        0     9583 2023-06-06 02:44:18.000000 zhousf-lib-0.5/zhousflib/datasets/labelme/labelme_convert_seg.py
+-rw-rw-rw-   0        0        0     3862 2023-06-06 06:12:25.000000 zhousf-lib-0.5/zhousflib/datasets/labelme/labelme_dataset_clip.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:13:24.070221 zhousf-lib-0.5/zhousflib/datasets/segmentation/
+-rw-rw-rw-   0        0        0       84 2023-06-06 02:48:08.000000 zhousf-lib-0.5/zhousflib/datasets/segmentation/__init__.py
+-rw-rw-rw-   0        0        0     2723 2023-06-06 02:48:08.000000 zhousf-lib-0.5/zhousflib/datasets/segmentation/seg_dataset_split.py
```

### Comparing `zhousf-lib-0.4/LICENSE` & `zhousf-lib-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.4/PKG-INFO` & `zhousf-lib-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhousf-lib
-Version: 0.4
+Version: 0.5
 Summary: a python library of zhousf
 Home-page: https://github.com/MrZhousf/ZhousfLib
 Author: zhousf
 Author-email: 442553199@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `zhousf-lib-0.4/core/font/__init__.py` & `zhousf-lib-0.5/zhousflib/core/font/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.4/core/util/calculater_util.py` & `zhousf-lib-0.5/zhousflib/core/util/calculater_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.4/core/util/cv_util.py` & `zhousf-lib-0.5/zhousflib/core/util/cv_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.4/core/util/encrypt_util.py` & `zhousf-lib-0.5/zhousflib/core/util/encrypt_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.4/core/util/img_util.py` & `zhousf-lib-0.5/zhousflib/core/util/img_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.4/core/util/interceptor_util.py` & `zhousf-lib-0.5/zhousflib/core/util/interceptor_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.4/core/util/iou_util.py` & `zhousf-lib-0.5/zhousflib/core/util/iou_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.4/core/util/log_util.py` & `zhousf-lib-0.5/zhousflib/core/util/log_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.4/core/util/pdf_util.py` & `zhousf-lib-0.5/zhousflib/core/util/pdf_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.4/core/util/permission_util.py` & `zhousf-lib-0.5/zhousflib/core/util/permission_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.4/core/util/re_util.py` & `zhousf-lib-0.5/zhousflib/core/util/re_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.4/core/util/string_util.py` & `zhousf-lib-0.5/zhousflib/core/util/string_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.4/core/util/time_util.py` & `zhousf-lib-0.5/zhousflib/core/util/time_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.4/datasets/coco/coco_bbox_extract.py` & `zhousf-lib-0.5/zhousflib/datasets/coco/coco_bbox_extract.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.4/datasets/coco/coco_bbox_update.py` & `zhousf-lib-0.5/zhousflib/datasets/coco/coco_bbox_update.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.4/datasets/coco/coco_bbox_vis.py` & `zhousf-lib-0.5/zhousflib/datasets/coco/coco_bbox_vis.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Date:    2023-03-15
 # Description:
 import json
 import random
 import colorsys
 from pathlib import Path
 from PIL import Image, ImageDraw, ImageFont
-from core.font import Font_SimSun
+from zhousflib.core.font import Font_SimSun
 FONT = ImageFont.truetype(font=str(Font_SimSun), size=15)
 
 
 def coco_convert_bbox(box_coco: list):
     _x, _y, _width, _height = tuple(box_coco)
     _bbox = (_x, _y, _x + _width, _y + _height)
     return _bbox
```

### Comparing `zhousf-lib-0.4/datasets/coco/coco_dataset_merge.py` & `zhousf-lib-0.5/zhousflib/datasets/coco/coco_dataset_merge.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.4/datasets/coco/coco_dataset_split.py` & `zhousf-lib-0.5/zhousflib/datasets/coco/coco_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.4/datasets/labelme/labelme_convert_coco.py` & `zhousf-lib-0.5/zhousflib/datasets/labelme/labelme_convert_coco.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # @Date    : 2023/4/23 
 # @Function: labelme convert coco | coco conver labelme
 import json
 import numpy
 import shutil
 import colorsys
 from pathlib import Path
-from core.util.img_util import get_file_base64
+from zhousflib.core.util.img_util import get_file_base64
 
 
 def coco_convert_bbox(box_coco: list):
     _x, _y, _width, _height = tuple(box_coco)
     _bbox = (_x, _y, _x + _width, _y + _height)
     return _bbox
```

### Comparing `zhousf-lib-0.4/datasets/labelme/labelme_convert_seg.py` & `zhousf-lib-0.5/zhousflib/datasets/labelme/labelme_convert_seg.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.4/datasets/labelme/labelme_dataset_clip.py` & `zhousf-lib-0.5/zhousflib/datasets/labelme/labelme_dataset_clip.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 # @Author  : zhousf
 # @Date    : 2023/5/17 
 # @Function: labelme标注数据裁剪工具
 import json
 import numpy as np
 from pathlib import Path
 from PIL import Image, ImageDraw, ImageFont
-from core.util.img_util import get_file_base64
-from core.font import Font_SimSun
+from zhousflib.core.util.img_util import get_file_base64
+from zhousflib.core.font import Font_SimSun
 
 FONT = ImageFont.truetype(font=str(Font_SimSun), size=15)
 
 
 def clip_img(labelme_dir: Path, dst_dir: Path, clip_labels: list, show=False):
     """
     裁剪
```

### Comparing `zhousf-lib-0.4/datasets/segmentation/seg_dataset_split.py` & `zhousf-lib-0.5/zhousflib/datasets/segmentation/seg_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.4/setup.py` & `zhousf-lib-0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,30 @@
 # -*- coding: utf-8 -*-
 # @Author  : zhousf
 # @Date    : 2023/6/6 
 # @Function:
-"""
-
-构建项目
-python -m pip install --user --upgrade setuptools wheel
-上传文件至Pypi
-python -m pip install --user --upgrade twine
-检查语法是否正确
-python setup.py check
-构建项目
-python setup.py sdist bdist_wheel
-Anaconda prompt中输入Pypi的账户与密码
-twine upload --repository-url https://upload.pypi.org/legacy/ dist/*
-
-
-"""
-
-# !/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 # Note: To use the 'upload' functionality of this file, you must:
 #   $ pipenv install twine --dev
 
 import io
 import os
 import sys
 from shutil import rmtree
 
 from setuptools import find_packages, setup, Command
 
-
+# python setup.py upload
 NAME = 'zhousf-lib'
 DESCRIPTION = 'a python library of zhousf'
 URL = 'https://github.com/MrZhousf/ZhousfLib'
 EMAIL = '442553199@qq.com'
 AUTHOR = 'zhousf'
 REQUIRES_PYTHON = '>=3.6.13'
-VERSION = '0.4'
+VERSION = '0.5'
 
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 # What packages are required for this module to be executed?
 REQUIRED = [
@@ -152,44 +134,9 @@
     ],
     # $ setup.py publish support.
     cmdclass={
         'upload': UploadCommand,
     },
 )
 
-# from __future__ import print_function
-# from setuptools import setup, find_packages
-# import version
-#
-# with open("README.md", "r", encoding='utf-8') as fh:
-#     long_description = fh.read()
-#
-# setup(
-#     name="zhousf-lib",
-#     version=version.__version__,
-#     author="zhousf",
-#     author_email="442553199@qq.com",
-#     description="a python library of zhousf",
-#     long_description=long_description,
-#     long_description_content_type="text/markdown",
-#     license="MIT",
-#     url="https://github.com/MrZhousf/ZhousfLib",
-#     packages=find_packages(),
-#     include_package_data=True,
-#     py_modules=['zhousflib'],
-#     install_requires=[
-#         "numpy <= 1.24.3",
-#         ],
-#     classifiers=[
-#         "Topic :: Software Development :: Libraries :: Python Modules",
-#         "Programming Language :: Python",
-#         "Programming Language :: Python :: 3",
-#         "Programming Language :: Python :: 3.5",
-#         "Programming Language :: Python :: 3.5",
-#         "Programming Language :: Python :: 3.6",
-#         "Programming Language :: Python :: 3.7",
-#         'Programming Language :: Python :: Implementation :: CPython',
-#     ],
-# )
-#
```

### Comparing `zhousf-lib-0.4/zhousf_lib.egg-info/PKG-INFO` & `zhousf-lib-0.5/zhousf_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhousf-lib
-Version: 0.4
+Version: 0.5
 Summary: a python library of zhousf
 Home-page: https://github.com/MrZhousf/ZhousfLib
 Author: zhousf
 Author-email: 442553199@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

