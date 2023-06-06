# Comparing `tmp/zhousf_lib-0.1.tar.gz` & `tmp/zhousf-lib-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhousf_lib-0.1.tar", last modified: Tue Jun  6 03:05:45 2023, max compression
+gzip compressed data, was "zhousf-lib-0.3.tar", last modified: Tue Jun  6 05:47:20 2023, max compression
```

## Comparing `zhousf_lib-0.1.tar` & `zhousf-lib-0.3.tar`

### file list

```diff
@@ -1,12 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 03:05:45.946777 zhousf_lib-0.1/
--rw-rw-rw-   0        0        0     1086 2023-06-06 02:24:10.000000 zhousf_lib-0.1/LICENSE
--rw-rw-rw-   0        0        0      750 2023-06-06 03:05:45.945777 zhousf_lib-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       36 2023-06-06 02:24:10.000000 zhousf_lib-0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-06 03:05:45.946777 zhousf_lib-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1418 2023-06-06 03:05:43.000000 zhousf_lib-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 03:05:45.943777 zhousf_lib-0.1/zhousf_lib.egg-info/
--rw-rw-rw-   0        0        0      750 2023-06-06 03:05:45.000000 zhousf_lib-0.1/zhousf_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-06-06 03:05:45.000000 zhousf_lib-0.1/zhousf_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 03:05:45.000000 zhousf_lib-0.1/zhousf_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-06 03:05:45.000000 zhousf_lib-0.1/zhousf_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-06 03:05:45.000000 zhousf_lib-0.1/zhousf_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 05:47:20.944373 zhousf-lib-0.3/
+-rw-rw-rw-   0        0        0     1086 2023-06-06 02:24:10.000000 zhousf-lib-0.3/LICENSE
+-rw-rw-rw-   0        0        0      750 2023-06-06 05:47:20.943373 zhousf-lib-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       36 2023-06-06 02:24:10.000000 zhousf-lib-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 05:47:20.903374 zhousf-lib-0.3/core/
+-rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.3/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:47:20.904373 zhousf-lib-0.3/core/font/
+-rw-rw-rw-   0        0        0      873 2023-06-06 02:39:11.000000 zhousf-lib-0.3/core/font/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:47:20.921374 zhousf-lib-0.3/core/util/
+-rw-rw-rw-   0        0        0       84 2023-06-06 02:39:11.000000 zhousf-lib-0.3/core/util/__init__.py
+-rw-rw-rw-   0        0        0     2795 2023-06-06 02:39:11.000000 zhousf-lib-0.3/core/util/calculater_util.py
+-rw-rw-rw-   0        0        0      709 2023-06-06 02:39:10.000000 zhousf-lib-0.3/core/util/cv_util.py
+-rw-rw-rw-   0        0        0     2220 2023-06-06 02:39:11.000000 zhousf-lib-0.3/core/util/encrypt_util.py
+-rw-rw-rw-   0        0        0      492 2023-06-06 02:39:11.000000 zhousf-lib-0.3/core/util/except_util.py
+-rw-rw-rw-   0        0        0     1359 2023-06-06 02:48:08.000000 zhousf-lib-0.3/core/util/img_util.py
+-rw-rw-rw-   0        0        0     1116 2023-06-06 02:39:11.000000 zhousf-lib-0.3/core/util/interceptor_util.py
+-rw-rw-rw-   0        0        0    12953 2023-06-06 02:39:11.000000 zhousf-lib-0.3/core/util/iou_util.py
+-rw-rw-rw-   0        0        0     3129 2023-06-06 02:39:11.000000 zhousf-lib-0.3/core/util/log_util.py
+-rw-rw-rw-   0        0        0     1812 2023-06-06 02:39:10.000000 zhousf-lib-0.3/core/util/pdf_util.py
+-rw-rw-rw-   0        0        0     1385 2023-06-06 02:39:10.000000 zhousf-lib-0.3/core/util/permission_util.py
+-rw-rw-rw-   0        0        0      658 2023-06-06 02:39:10.000000 zhousf-lib-0.3/core/util/re_util.py
+-rw-rw-rw-   0        0        0      805 2023-06-06 02:39:11.000000 zhousf-lib-0.3/core/util/string_util.py
+-rw-rw-rw-   0        0        0     4687 2023-06-06 02:39:10.000000 zhousf-lib-0.3/core/util/time_util.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:47:20.922372 zhousf-lib-0.3/datasets/
+-rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.3/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:47:20.930372 zhousf-lib-0.3/datasets/coco/
+-rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.3/datasets/coco/__init__.py
+-rw-rw-rw-   0        0        0     8244 2023-06-06 02:42:48.000000 zhousf-lib-0.3/datasets/coco/coco_bbox_extract.py
+-rw-rw-rw-   0        0        0     5813 2023-06-06 02:40:04.000000 zhousf-lib-0.3/datasets/coco/coco_bbox_update.py
+-rw-rw-rw-   0        0        0     6557 2023-06-06 02:43:29.000000 zhousf-lib-0.3/datasets/coco/coco_bbox_vis.py
+-rw-rw-rw-   0        0        0     2889 2023-06-06 02:42:48.000000 zhousf-lib-0.3/datasets/coco/coco_dataset_merge.py
+-rw-rw-rw-   0        0        0     6077 2023-06-06 02:42:48.000000 zhousf-lib-0.3/datasets/coco/coco_dataset_split.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:47:20.934372 zhousf-lib-0.3/datasets/labelme/
+-rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.3/datasets/labelme/__init__.py
+-rw-rw-rw-   0        0        0     8110 2023-06-06 02:48:08.000000 zhousf-lib-0.3/datasets/labelme/labelme_convert_coco.py
+-rw-rw-rw-   0        0        0     9583 2023-06-06 02:44:18.000000 zhousf-lib-0.3/datasets/labelme/labelme_convert_seg.py
+-rw-rw-rw-   0        0        0     3842 2023-06-06 02:48:08.000000 zhousf-lib-0.3/datasets/labelme/labelme_dataset_clip.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:47:20.936371 zhousf-lib-0.3/datasets/segmentation/
+-rw-rw-rw-   0        0        0       84 2023-06-06 02:48:08.000000 zhousf-lib-0.3/datasets/segmentation/__init__.py
+-rw-rw-rw-   0        0        0     2723 2023-06-06 02:48:08.000000 zhousf-lib-0.3/datasets/segmentation/seg_dataset_split.py
+-rw-rw-rw-   0        0        0       42 2023-06-06 05:47:20.944373 zhousf-lib-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1569 2023-06-06 05:46:26.000000 zhousf-lib-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:47:20.942373 zhousf-lib-0.3/zhousf_lib.egg-info/
+-rw-rw-rw-   0        0        0      750 2023-06-06 05:47:20.000000 zhousf-lib-0.3/zhousf_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1020 2023-06-06 05:47:20.000000 zhousf-lib-0.3/zhousf_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 05:47:20.000000 zhousf-lib-0.3/zhousf_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-06 05:47:20.000000 zhousf-lib-0.3/zhousf_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-06 05:47:20.000000 zhousf-lib-0.3/zhousf_lib.egg-info/top_level.txt
```

### Comparing `zhousf_lib-0.1/LICENSE` & `zhousf-lib-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zhousf_lib-0.1/PKG-INFO` & `zhousf-lib-0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: zhousf_lib
-Version: 0.1
+Name: zhousf-lib
+Version: 0.3
 Summary: a python library of zhousf
 Home-page: https://github.com/MrZhousf/ZhousfLib
 Author: zhousf
 Author-email: 442553199@qq.com
 License: MIT
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
```

### Comparing `zhousf_lib-0.1/setup.py` & `zhousf-lib-0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,36 +8,39 @@
 python -m pip install --user --upgrade setuptools wheel
 上传文件至Pypi
 python -m pip install --user --upgrade twine
 检查语法是否正确
 python setup.py check
 构建项目
 python setup.py sdist bdist_wheel
+cmd中输入Pypi的账户与密码
+twine upload --repository-url https://upload.pypi.org/legacy/ dist/*
 
 
 """
 
 from __future__ import print_function
-from setuptools import setup
+from setuptools import setup, find_packages
 import version
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
-    name="zhousf_lib",
+    name="zhousf-lib",
     version=version.__version__,
     author="zhousf",
     author_email="442553199@qq.com",
     description="a python library of zhousf",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/MrZhousf/ZhousfLib",
-    py_modules=['zhousf_lib'],
+    packages=find_packages(),
+    py_modules=['zhousflib'],
     install_requires=[
         "numpy <= 1.24.3",
         ],
     classifiers=[
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
```

### Comparing `zhousf_lib-0.1/zhousf_lib.egg-info/PKG-INFO` & `zhousf-lib-0.3/zhousf_lib.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhousf-lib
-Version: 0.1
+Version: 0.3
 Summary: a python library of zhousf
 Home-page: https://github.com/MrZhousf/ZhousfLib
 Author: zhousf
 Author-email: 442553199@qq.com
 License: MIT
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
```

