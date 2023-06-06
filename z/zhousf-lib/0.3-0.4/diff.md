# Comparing `tmp/zhousf-lib-0.3.tar.gz` & `tmp/zhousf-lib-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhousf-lib-0.3.tar", last modified: Tue Jun  6 05:47:20 2023, max compression
+gzip compressed data, was "zhousf-lib-0.4.tar", last modified: Tue Jun  6 06:06:45 2023, max compression
```

## Comparing `zhousf-lib-0.3.tar` & `zhousf-lib-0.4.tar`

### file list

```diff
@@ -1,48 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 05:47:20.944373 zhousf-lib-0.3/
--rw-rw-rw-   0        0        0     1086 2023-06-06 02:24:10.000000 zhousf-lib-0.3/LICENSE
--rw-rw-rw-   0        0        0      750 2023-06-06 05:47:20.943373 zhousf-lib-0.3/PKG-INFO
--rw-rw-rw-   0        0        0       36 2023-06-06 02:24:10.000000 zhousf-lib-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 05:47:20.903374 zhousf-lib-0.3/core/
--rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.3/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 05:47:20.904373 zhousf-lib-0.3/core/font/
--rw-rw-rw-   0        0        0      873 2023-06-06 02:39:11.000000 zhousf-lib-0.3/core/font/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 05:47:20.921374 zhousf-lib-0.3/core/util/
--rw-rw-rw-   0        0        0       84 2023-06-06 02:39:11.000000 zhousf-lib-0.3/core/util/__init__.py
--rw-rw-rw-   0        0        0     2795 2023-06-06 02:39:11.000000 zhousf-lib-0.3/core/util/calculater_util.py
--rw-rw-rw-   0        0        0      709 2023-06-06 02:39:10.000000 zhousf-lib-0.3/core/util/cv_util.py
--rw-rw-rw-   0        0        0     2220 2023-06-06 02:39:11.000000 zhousf-lib-0.3/core/util/encrypt_util.py
--rw-rw-rw-   0        0        0      492 2023-06-06 02:39:11.000000 zhousf-lib-0.3/core/util/except_util.py
--rw-rw-rw-   0        0        0     1359 2023-06-06 02:48:08.000000 zhousf-lib-0.3/core/util/img_util.py
--rw-rw-rw-   0        0        0     1116 2023-06-06 02:39:11.000000 zhousf-lib-0.3/core/util/interceptor_util.py
--rw-rw-rw-   0        0        0    12953 2023-06-06 02:39:11.000000 zhousf-lib-0.3/core/util/iou_util.py
--rw-rw-rw-   0        0        0     3129 2023-06-06 02:39:11.000000 zhousf-lib-0.3/core/util/log_util.py
--rw-rw-rw-   0        0        0     1812 2023-06-06 02:39:10.000000 zhousf-lib-0.3/core/util/pdf_util.py
--rw-rw-rw-   0        0        0     1385 2023-06-06 02:39:10.000000 zhousf-lib-0.3/core/util/permission_util.py
--rw-rw-rw-   0        0        0      658 2023-06-06 02:39:10.000000 zhousf-lib-0.3/core/util/re_util.py
--rw-rw-rw-   0        0        0      805 2023-06-06 02:39:11.000000 zhousf-lib-0.3/core/util/string_util.py
--rw-rw-rw-   0        0        0     4687 2023-06-06 02:39:10.000000 zhousf-lib-0.3/core/util/time_util.py
-drwxrwxrwx   0        0        0        0 2023-06-06 05:47:20.922372 zhousf-lib-0.3/datasets/
--rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.3/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 05:47:20.930372 zhousf-lib-0.3/datasets/coco/
--rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.3/datasets/coco/__init__.py
--rw-rw-rw-   0        0        0     8244 2023-06-06 02:42:48.000000 zhousf-lib-0.3/datasets/coco/coco_bbox_extract.py
--rw-rw-rw-   0        0        0     5813 2023-06-06 02:40:04.000000 zhousf-lib-0.3/datasets/coco/coco_bbox_update.py
--rw-rw-rw-   0        0        0     6557 2023-06-06 02:43:29.000000 zhousf-lib-0.3/datasets/coco/coco_bbox_vis.py
--rw-rw-rw-   0        0        0     2889 2023-06-06 02:42:48.000000 zhousf-lib-0.3/datasets/coco/coco_dataset_merge.py
--rw-rw-rw-   0        0        0     6077 2023-06-06 02:42:48.000000 zhousf-lib-0.3/datasets/coco/coco_dataset_split.py
-drwxrwxrwx   0        0        0        0 2023-06-06 05:47:20.934372 zhousf-lib-0.3/datasets/labelme/
--rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.3/datasets/labelme/__init__.py
--rw-rw-rw-   0        0        0     8110 2023-06-06 02:48:08.000000 zhousf-lib-0.3/datasets/labelme/labelme_convert_coco.py
--rw-rw-rw-   0        0        0     9583 2023-06-06 02:44:18.000000 zhousf-lib-0.3/datasets/labelme/labelme_convert_seg.py
--rw-rw-rw-   0        0        0     3842 2023-06-06 02:48:08.000000 zhousf-lib-0.3/datasets/labelme/labelme_dataset_clip.py
-drwxrwxrwx   0        0        0        0 2023-06-06 05:47:20.936371 zhousf-lib-0.3/datasets/segmentation/
--rw-rw-rw-   0        0        0       84 2023-06-06 02:48:08.000000 zhousf-lib-0.3/datasets/segmentation/__init__.py
--rw-rw-rw-   0        0        0     2723 2023-06-06 02:48:08.000000 zhousf-lib-0.3/datasets/segmentation/seg_dataset_split.py
--rw-rw-rw-   0        0        0       42 2023-06-06 05:47:20.944373 zhousf-lib-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1569 2023-06-06 05:46:26.000000 zhousf-lib-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 05:47:20.942373 zhousf-lib-0.3/zhousf_lib.egg-info/
--rw-rw-rw-   0        0        0      750 2023-06-06 05:47:20.000000 zhousf-lib-0.3/zhousf_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1020 2023-06-06 05:47:20.000000 zhousf-lib-0.3/zhousf_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 05:47:20.000000 zhousf-lib-0.3/zhousf_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-06 05:47:20.000000 zhousf-lib-0.3/zhousf_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-06-06 05:47:20.000000 zhousf-lib-0.3/zhousf_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 06:06:45.015116 zhousf-lib-0.4/
+-rw-rw-rw-   0        0        0     1086 2023-06-06 02:24:10.000000 zhousf-lib-0.4/LICENSE
+-rw-rw-rw-   0        0        0      672 2023-06-06 06:06:45.015116 zhousf-lib-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       36 2023-06-06 02:24:10.000000 zhousf-lib-0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 06:06:44.974086 zhousf-lib-0.4/core/
+-rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.4/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:06:44.975086 zhousf-lib-0.4/core/font/
+-rw-rw-rw-   0        0        0      873 2023-06-06 02:39:11.000000 zhousf-lib-0.4/core/font/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:06:44.989085 zhousf-lib-0.4/core/util/
+-rw-rw-rw-   0        0        0       84 2023-06-06 02:39:11.000000 zhousf-lib-0.4/core/util/__init__.py
+-rw-rw-rw-   0        0        0     2795 2023-06-06 02:39:11.000000 zhousf-lib-0.4/core/util/calculater_util.py
+-rw-rw-rw-   0        0        0      709 2023-06-06 02:39:10.000000 zhousf-lib-0.4/core/util/cv_util.py
+-rw-rw-rw-   0        0        0     2220 2023-06-06 02:39:11.000000 zhousf-lib-0.4/core/util/encrypt_util.py
+-rw-rw-rw-   0        0        0      492 2023-06-06 02:39:11.000000 zhousf-lib-0.4/core/util/except_util.py
+-rw-rw-rw-   0        0        0     1359 2023-06-06 02:48:08.000000 zhousf-lib-0.4/core/util/img_util.py
+-rw-rw-rw-   0        0        0     1116 2023-06-06 02:39:11.000000 zhousf-lib-0.4/core/util/interceptor_util.py
+-rw-rw-rw-   0        0        0    12953 2023-06-06 02:39:11.000000 zhousf-lib-0.4/core/util/iou_util.py
+-rw-rw-rw-   0        0        0     3129 2023-06-06 02:39:11.000000 zhousf-lib-0.4/core/util/log_util.py
+-rw-rw-rw-   0        0        0     1812 2023-06-06 02:39:10.000000 zhousf-lib-0.4/core/util/pdf_util.py
+-rw-rw-rw-   0        0        0     1385 2023-06-06 02:39:10.000000 zhousf-lib-0.4/core/util/permission_util.py
+-rw-rw-rw-   0        0        0      658 2023-06-06 02:39:10.000000 zhousf-lib-0.4/core/util/re_util.py
+-rw-rw-rw-   0        0        0      805 2023-06-06 02:39:11.000000 zhousf-lib-0.4/core/util/string_util.py
+-rw-rw-rw-   0        0        0     4687 2023-06-06 02:39:10.000000 zhousf-lib-0.4/core/util/time_util.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:06:44.992085 zhousf-lib-0.4/datasets/
+-rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.4/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:06:45.001085 zhousf-lib-0.4/datasets/coco/
+-rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.4/datasets/coco/__init__.py
+-rw-rw-rw-   0        0        0     8244 2023-06-06 02:42:48.000000 zhousf-lib-0.4/datasets/coco/coco_bbox_extract.py
+-rw-rw-rw-   0        0        0     5813 2023-06-06 02:40:04.000000 zhousf-lib-0.4/datasets/coco/coco_bbox_update.py
+-rw-rw-rw-   0        0        0     6557 2023-06-06 02:43:29.000000 zhousf-lib-0.4/datasets/coco/coco_bbox_vis.py
+-rw-rw-rw-   0        0        0     2889 2023-06-06 02:42:48.000000 zhousf-lib-0.4/datasets/coco/coco_dataset_merge.py
+-rw-rw-rw-   0        0        0     6077 2023-06-06 02:42:48.000000 zhousf-lib-0.4/datasets/coco/coco_dataset_split.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:06:45.006086 zhousf-lib-0.4/datasets/labelme/
+-rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.4/datasets/labelme/__init__.py
+-rw-rw-rw-   0        0        0     8110 2023-06-06 02:48:08.000000 zhousf-lib-0.4/datasets/labelme/labelme_convert_coco.py
+-rw-rw-rw-   0        0        0     9583 2023-06-06 02:44:18.000000 zhousf-lib-0.4/datasets/labelme/labelme_convert_seg.py
+-rw-rw-rw-   0        0        0     3842 2023-06-06 02:48:08.000000 zhousf-lib-0.4/datasets/labelme/labelme_dataset_clip.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:06:45.009086 zhousf-lib-0.4/datasets/segmentation/
+-rw-rw-rw-   0        0        0       84 2023-06-06 02:48:08.000000 zhousf-lib-0.4/datasets/segmentation/__init__.py
+-rw-rw-rw-   0        0        0     2723 2023-06-06 02:48:08.000000 zhousf-lib-0.4/datasets/segmentation/seg_dataset_split.py
+-rw-rw-rw-   0        0        0       42 2023-06-06 06:06:45.015116 zhousf-lib-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     5715 2023-06-06 06:06:08.000000 zhousf-lib-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:06:45.014086 zhousf-lib-0.4/zhousf_lib.egg-info/
+-rw-rw-rw-   0        0        0      672 2023-06-06 06:06:44.000000 zhousf-lib-0.4/zhousf_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      987 2023-06-06 06:06:44.000000 zhousf-lib-0.4/zhousf_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 06:06:44.000000 zhousf-lib-0.4/zhousf_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-06 06:06:44.000000 zhousf-lib-0.4/zhousf_lib.egg-info/top_level.txt
```

### Comparing `zhousf-lib-0.3/LICENSE` & `zhousf-lib-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.3/core/font/__init__.py` & `zhousf-lib-0.4/core/font/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.3/core/util/calculater_util.py` & `zhousf-lib-0.4/core/util/calculater_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.3/core/util/cv_util.py` & `zhousf-lib-0.4/core/util/cv_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.3/core/util/encrypt_util.py` & `zhousf-lib-0.4/core/util/encrypt_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.3/core/util/img_util.py` & `zhousf-lib-0.4/core/util/img_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.3/core/util/interceptor_util.py` & `zhousf-lib-0.4/core/util/interceptor_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.3/core/util/iou_util.py` & `zhousf-lib-0.4/core/util/iou_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.3/core/util/log_util.py` & `zhousf-lib-0.4/core/util/log_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.3/core/util/pdf_util.py` & `zhousf-lib-0.4/core/util/pdf_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.3/core/util/permission_util.py` & `zhousf-lib-0.4/core/util/permission_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.3/core/util/re_util.py` & `zhousf-lib-0.4/core/util/re_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.3/core/util/string_util.py` & `zhousf-lib-0.4/core/util/string_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.3/core/util/time_util.py` & `zhousf-lib-0.4/core/util/time_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.3/datasets/coco/coco_bbox_extract.py` & `zhousf-lib-0.4/datasets/coco/coco_bbox_extract.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.3/datasets/coco/coco_bbox_update.py` & `zhousf-lib-0.4/datasets/coco/coco_bbox_update.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.3/datasets/coco/coco_bbox_vis.py` & `zhousf-lib-0.4/datasets/coco/coco_bbox_vis.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.3/datasets/coco/coco_dataset_merge.py` & `zhousf-lib-0.4/datasets/coco/coco_dataset_merge.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.3/datasets/coco/coco_dataset_split.py` & `zhousf-lib-0.4/datasets/coco/coco_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.3/datasets/labelme/labelme_convert_coco.py` & `zhousf-lib-0.4/datasets/labelme/labelme_convert_coco.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.3/datasets/labelme/labelme_convert_seg.py` & `zhousf-lib-0.4/datasets/labelme/labelme_convert_seg.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.3/datasets/labelme/labelme_dataset_clip.py` & `zhousf-lib-0.4/datasets/labelme/labelme_dataset_clip.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.3/datasets/segmentation/seg_dataset_split.py` & `zhousf-lib-0.4/datasets/segmentation/seg_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.3/zhousf_lib.egg-info/SOURCES.txt` & `zhousf-lib-0.4/zhousf_lib.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -29,9 +29,8 @@
 datasets/labelme/labelme_convert_seg.py
 datasets/labelme/labelme_dataset_clip.py
 datasets/segmentation/__init__.py
 datasets/segmentation/seg_dataset_split.py
 zhousf_lib.egg-info/PKG-INFO
 zhousf_lib.egg-info/SOURCES.txt
 zhousf_lib.egg-info/dependency_links.txt
-zhousf_lib.egg-info/requires.txt
 zhousf_lib.egg-info/top_level.txt
```

