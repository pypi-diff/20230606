# Comparing `tmp/ccdt-2.1.7.tar.gz` & `tmp/ccdt-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccdt-2.1.7.tar", last modified: Fri Jun  2 09:13:31 2023, max compression
+gzip compressed data, was "ccdt-2.1.8.tar", last modified: Tue Jun  6 03:09:34 2023, max compression
```

## Comparing `ccdt-2.1.7.tar` & `ccdt-2.1.8.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 09:13:31.125148 ccdt-2.1.7/
--rw-rw-rw-   0        0        0    35823 2023-05-23 02:06:29.000000 ccdt-2.1.7/LICENSE
--rw-rw-rw-   0        0        0     4309 2023-06-02 09:13:31.123179 ccdt-2.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     3785 2023-05-23 02:44:28.000000 ccdt-2.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 09:13:31.076279 ccdt-2.1.7/ccdt/
--rw-rw-rw-   0        0        0      150 2023-06-01 09:39:39.000000 ccdt-2.1.7/ccdt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:13:31.095227 ccdt-2.1.7/ccdt/dataset/
--rw-rw-rw-   0        0        0      216 2023-05-17 01:52:32.000000 ccdt-2.1.7/ccdt/dataset/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:13:31.099217 ccdt-2.1.7/ccdt/dataset/base_coco/
--rw-rw-rw-   0        0        0      171 2023-05-17 01:51:28.000000 ccdt-2.1.7/ccdt/dataset/base_coco/__init__.py
--rw-rw-rw-   0        0        0    22572 2023-05-25 05:57:25.000000 ccdt-2.1.7/ccdt/dataset/base_coco/base_coco.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:13:31.107194 ccdt-2.1.7/ccdt/dataset/base_labelme/
--rw-rw-rw-   0        0        0      180 2023-05-17 01:47:52.000000 ccdt-2.1.7/ccdt/dataset/base_labelme/__init__.py
--rw-rw-rw-   0        0        0     7497 2023-06-02 09:12:57.000000 ccdt-2.1.7/ccdt/dataset/base_labelme/async_io_task.py
--rw-rw-rw-   0        0        0    63498 2023-05-25 02:57:06.000000 ccdt-2.1.7/ccdt/dataset/base_labelme/base_labelme.py
--rw-rw-rw-   0        0        0    14420 2023-05-25 03:24:49.000000 ccdt-2.1.7/ccdt/dataset/main.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:13:31.114197 ccdt-2.1.7/ccdt/dataset/utils/
--rw-rw-rw-   0        0        0      221 2023-05-17 01:56:42.000000 ccdt-2.1.7/ccdt/dataset/utils/__init__.py
--rw-rw-rw-   0        0        0      562 2023-05-17 01:54:00.000000 ccdt-2.1.7/ccdt/dataset/utils/encoder.py
--rw-rw-rw-   0        0        0    17029 2023-05-25 06:27:22.000000 ccdt-2.1.7/ccdt/dataset/utils/labelme_load.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:13:31.121159 ccdt-2.1.7/ccdt/video_tool/
--rw-rw-rw-   0        0        0      172 2023-05-25 06:30:32.000000 ccdt-2.1.7/ccdt/video_tool/__init__.py
--rw-rw-rw-   0        0        0     1382 2023-05-25 06:23:23.000000 ccdt-2.1.7/ccdt/video_tool/split.py
--rw-rw-rw-   0        0        0     4845 2023-05-25 06:30:32.000000 ccdt-2.1.7/ccdt/video_tool/video_main.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:13:31.090241 ccdt-2.1.7/ccdt.egg-info/
--rw-rw-rw-   0        0        0     4309 2023-06-02 09:13:31.000000 ccdt-2.1.7/ccdt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      632 2023-06-02 09:13:31.000000 ccdt-2.1.7/ccdt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 09:13:31.000000 ccdt-2.1.7/ccdt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-06-02 09:13:31.000000 ccdt-2.1.7/ccdt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       80 2023-06-02 09:13:31.000000 ccdt-2.1.7/ccdt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-02 09:13:31.000000 ccdt-2.1.7/ccdt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 09:13:31.125148 ccdt-2.1.7/setup.cfg
--rw-rw-rw-   0        0        0     2401 2023-06-02 09:12:57.000000 ccdt-2.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 03:09:34.171066 ccdt-2.1.8/
+-rw-rw-rw-   0        0        0    35823 2023-05-23 02:06:29.000000 ccdt-2.1.8/LICENSE
+-rw-rw-rw-   0        0        0     4309 2023-06-06 03:09:34.169071 ccdt-2.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3785 2023-05-23 02:44:28.000000 ccdt-2.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 03:09:34.032437 ccdt-2.1.8/ccdt/
+-rw-rw-rw-   0        0        0      150 2023-06-01 09:39:39.000000 ccdt-2.1.8/ccdt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 03:09:34.051386 ccdt-2.1.8/ccdt/dataset/
+-rw-rw-rw-   0        0        0      216 2023-05-17 01:52:32.000000 ccdt-2.1.8/ccdt/dataset/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 03:09:34.079310 ccdt-2.1.8/ccdt/dataset/base_coco/
+-rw-rw-rw-   0        0        0      171 2023-05-17 01:51:28.000000 ccdt-2.1.8/ccdt/dataset/base_coco/__init__.py
+-rw-rw-rw-   0        0        0    22572 2023-05-25 05:57:25.000000 ccdt-2.1.8/ccdt/dataset/base_coco/base_coco.py
+drwxrwxrwx   0        0        0        0 2023-06-06 03:09:34.102249 ccdt-2.1.8/ccdt/dataset/base_labelme/
+-rw-rw-rw-   0        0        0      180 2023-05-17 01:47:52.000000 ccdt-2.1.8/ccdt/dataset/base_labelme/__init__.py
+-rw-rw-rw-   0        0        0     7523 2023-06-06 03:07:09.000000 ccdt-2.1.8/ccdt/dataset/base_labelme/async_io_task.py
+-rw-rw-rw-   0        0        0    63537 2023-06-06 03:07:09.000000 ccdt-2.1.8/ccdt/dataset/base_labelme/base_labelme.py
+-rw-rw-rw-   0        0        0    14420 2023-05-25 03:24:49.000000 ccdt-2.1.8/ccdt/dataset/main.py
+drwxrwxrwx   0        0        0        0 2023-06-06 03:09:34.110255 ccdt-2.1.8/ccdt/dataset/utils/
+-rw-rw-rw-   0        0        0      221 2023-05-17 01:56:42.000000 ccdt-2.1.8/ccdt/dataset/utils/__init__.py
+-rw-rw-rw-   0        0        0      562 2023-05-17 01:54:00.000000 ccdt-2.1.8/ccdt/dataset/utils/encoder.py
+-rw-rw-rw-   0        0        0    17029 2023-05-25 06:27:22.000000 ccdt-2.1.8/ccdt/dataset/utils/labelme_load.py
+drwxrwxrwx   0        0        0        0 2023-06-06 03:09:34.154133 ccdt-2.1.8/ccdt/video_tool/
+-rw-rw-rw-   0        0        0      172 2023-05-25 06:30:32.000000 ccdt-2.1.8/ccdt/video_tool/__init__.py
+-rw-rw-rw-   0        0        0     1382 2023-05-25 06:23:23.000000 ccdt-2.1.8/ccdt/video_tool/split.py
+-rw-rw-rw-   0        0        0     4845 2023-05-25 06:30:32.000000 ccdt-2.1.8/ccdt/video_tool/video_main.py
+drwxrwxrwx   0        0        0        0 2023-06-06 03:09:34.046398 ccdt-2.1.8/ccdt.egg-info/
+-rw-rw-rw-   0        0        0     4309 2023-06-06 03:09:33.000000 ccdt-2.1.8/ccdt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      645 2023-06-06 03:09:34.000000 ccdt-2.1.8/ccdt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 03:09:33.000000 ccdt-2.1.8/ccdt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-06-06 03:09:33.000000 ccdt-2.1.8/ccdt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       80 2023-06-06 03:09:33.000000 ccdt-2.1.8/ccdt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-06 03:09:33.000000 ccdt-2.1.8/ccdt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 03:09:34.171066 ccdt-2.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     2401 2023-06-06 03:07:09.000000 ccdt-2.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 03:09:34.166078 ccdt-2.1.8/test/
+-rw-rw-rw-   0        0        0     8106 2023-06-05 05:36:13.000000 ccdt-2.1.8/test/test.py
```

### Comparing `ccdt-2.1.7/LICENSE` & `ccdt-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.7/PKG-INFO` & `ccdt-2.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.1.7
+Version: 2.1.8
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ccdt-2.1.7/README.md` & `ccdt-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.7/ccdt/dataset/base_coco/base_coco.py` & `ccdt-2.1.8/ccdt/dataset/base_coco/base_coco.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.7/ccdt/dataset/base_labelme/async_io_task.py` & `ccdt-2.1.8/ccdt/dataset/base_labelme/async_io_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # 计算机登录用户: jk
 # 系统日期: 2023/5/18 15:58
 # 项目名称: async_ccdt
 # 开发者: zhanyong
-import json
 import shutil
 import asyncio
 import os
 from concurrent.futures import ThreadPoolExecutor
 from tqdm import tqdm
 from pathlib import Path
 import argparse
 import json
 import aiofiles
+from ccdt.dataset.utils.encoder import Encoder
 
 
 class AsyncIoTask(object):
     """
     asyncio.get_running_loop().run_in_executor函数的作用是将指定函数在线程池中异步执行，返回异步任务future。这样我们可以在多个任务之间切换，并且不需要等待文件写入、文件复制和文件移动操作完成，从而实现异步高并发和非阻塞操作。
     run_in_executor(None)，None参数表示开启默认线程执行，异步执行 CPU 密集型任务或 I/O 密集型任务
     """
 
     @staticmethod
     async def write_file(file_path: str, content: dict):
         # 通过aiofiles.open(),实现异步方式进行文件的读写操作
         async with aiofiles.open(file_path, 'w') as f:
             # cls=json.JSONEncoder不是必须的，因为json.dumps() 函数会自动选择适当的编码器来对 Python 对象进行编码
-            await f.write(json.dumps(content, indent=2, cls=json.JSONEncoder))
+            await f.write(json.dumps(content, indent=2, cls=Encoder))
 
     @staticmethod
     async def copy_file(src_file_path: str, dst_file_path: str):
         # 异步复制文件
         # with open(src_file_path, 'rb') as src_file, open(dst_file_path, 'wb') as dst_file:
         await asyncio.get_running_loop().run_in_executor(None, shutil.copy, src_file_path, dst_file_path)
```

### Comparing `ccdt-2.1.7/ccdt/dataset/base_labelme/base_labelme.py` & `ccdt-2.1.8/ccdt/dataset/base_labelme/base_labelme.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import random
 from shapely.geometry import Polygon, Point, box
 import cv2
 import numpy as np
 from pathlib import Path
 import copy
 import json
+from ccdt.dataset.utils.encoder import Encoder
 
 
 def my_sort(item):
     """
     自定义标注形状排序，把标注形状为矩形框的排序在列表第一位
     :param item:
     :return:
@@ -685,15 +686,15 @@
                         rebuild_img_dir = os.path.join(dataset.get('output_dir'), dataset.get('image_dir'))
                         rebuild_json_dir = os.path.join(dataset.get('output_dir'), dataset.get('labelme_dir'))
                         os.makedirs(rebuild_img_dir, exist_ok=True)
                         os.makedirs(rebuild_json_dir, exist_ok=True)
                         # 重写json文件
                         final_json_path = os.path.join(rebuild_json_dir, rebuild_json_name)
                         with open(final_json_path, "w", encoding='UTF-8', ) as labelme_fp:  # 以写入模式打开这个文件
-                            json.dump(rebuild_json, labelme_fp, indent=2, cls=json.JSONEncoder)
+                            json.dump(rebuild_json, labelme_fp, indent=2, cls=Encoder)
                         # 保存截取到的图像
                         final_image_path = os.path.join(rebuild_img_dir, rebuild_img_name)
                         cv2.imwrite(final_image_path, roi)
                     else:
                         self.error_dataset_handle(dataset)
                         if shapes_value[0]['shape_type'] != 'rectangle':
                             print(f'存在一个标注时不为矩形框，请核对{file_path}')
```

### Comparing `ccdt-2.1.7/ccdt/dataset/main.py` & `ccdt-2.1.8/ccdt/dataset/main.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.7/ccdt/dataset/utils/encoder.py` & `ccdt-2.1.8/ccdt/dataset/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.7/ccdt/dataset/utils/labelme_load.py` & `ccdt-2.1.8/ccdt/dataset/utils/labelme_load.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.7/ccdt/video_tool/split.py` & `ccdt-2.1.8/ccdt/video_tool/split.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.7/ccdt/video_tool/video_main.py` & `ccdt-2.1.8/ccdt/video_tool/video_main.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.7/ccdt.egg-info/PKG-INFO` & `ccdt-2.1.8/ccdt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.1.7
+Version: 2.1.8
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ccdt-2.1.7/ccdt.egg-info/SOURCES.txt` & `ccdt-2.1.8/ccdt.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 ccdt/dataset/base_labelme/async_io_task.py
 ccdt/dataset/base_labelme/base_labelme.py
 ccdt/dataset/utils/__init__.py
 ccdt/dataset/utils/encoder.py
 ccdt/dataset/utils/labelme_load.py
 ccdt/video_tool/__init__.py
 ccdt/video_tool/split.py
-ccdt/video_tool/video_main.py
+ccdt/video_tool/video_main.py
+test/test.py
```

### Comparing `ccdt-2.1.7/setup.py` & `ccdt-2.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     ]
     return install_requires
 
 
 setup(
     # 取名不能够用_会自动变-   ccdt
     name='ccdt',
-    version='2.1.7',
+    version='2.1.8',
     packages=find_packages(exclude=['data']),
     install_requires=get_install_requires(),
     author='zhanyong',
     author_email='zhan.yong@chipeak.com',
     description='AI数据转换工具箱',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

