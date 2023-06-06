# Comparing `tmp/m3u8_XZ-0.0.2.tar.gz` & `tmp/m3u8_XZ-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "H:\PythonProject\XZlib\packaging_m3u8\dist\.tmp-bg_ye6g2\m3u8_XZ-0.0.2.tar", last modified: Sat May  6 04:17:13 2023, max compression
+gzip compressed data, was "H:\PythonProject\XZlib\packaging_m3u8\dist\.tmp-yudo51hc\m3u8_XZ-0.0.4.tar", last modified: Tue Jun  6 11:54:37 2023, max compression
```

## Comparing `m3u8_XZ-0.0.2.tar` & `m3u8_XZ-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 04:17:13.608021 m3u8_XZ-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-03-23 03:00:43.000000 m3u8_XZ-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      736 2023-05-06 04:17:13.607023 m3u8_XZ-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      393 2023-05-06 04:16:16.000000 m3u8_XZ-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 04:17:13.594062 m3u8_XZ-0.0.2/m3u8_XZ/
--rw-rw-rw-   0        0        0      120 2023-03-23 03:49:25.000000 m3u8_XZ-0.0.2/m3u8_XZ/__init__.py
--rw-rw-rw-   0        0        0      678 2023-05-05 05:15:21.000000 m3u8_XZ-0.0.2/m3u8_XZ/cryptoModel.py
--rw-rw-rw-   0        0        0     6790 2023-05-06 03:59:07.000000 m3u8_XZ-0.0.2/m3u8_XZ/xz.py
-drwxrwxrwx   0        0        0        0 2023-05-06 04:17:13.604035 m3u8_XZ-0.0.2/m3u8_XZ.egg-info/
--rw-rw-rw-   0        0        0      736 2023-05-06 04:17:13.000000 m3u8_XZ-0.0.2/m3u8_XZ.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-05-06 04:17:13.000000 m3u8_XZ-0.0.2/m3u8_XZ.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 04:17:13.000000 m3u8_XZ-0.0.2/m3u8_XZ.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-05-06 04:17:13.000000 m3u8_XZ-0.0.2/m3u8_XZ.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-06 04:17:13.000000 m3u8_XZ-0.0.2/m3u8_XZ.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      522 2023-03-23 11:30:25.000000 m3u8_XZ-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 04:17:13.608021 m3u8_XZ-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      716 2023-05-06 04:04:36.000000 m3u8_XZ-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 04:17:13.606026 m3u8_XZ-0.0.2/test/
--rw-rw-rw-   0        0        0       98 2023-05-06 03:29:10.000000 m3u8_XZ-0.0.2/test/__init__.py
--rw-rw-rw-   0        0        0      365 2023-05-06 04:16:49.000000 m3u8_XZ-0.0.2/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:54:37.357859 m3u8_XZ-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-03-23 03:00:43.000000 m3u8_XZ-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      835 2023-06-06 11:54:37.356866 m3u8_XZ-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      458 2023-06-06 11:17:28.000000 m3u8_XZ-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 11:54:37.348883 m3u8_XZ-0.0.4/m3u8_XZ/
+-rw-rw-rw-   0        0        0      177 2023-06-06 11:01:44.000000 m3u8_XZ-0.0.4/m3u8_XZ/__init__.py
+-rw-rw-rw-   0        0        0      678 2023-05-05 05:15:21.000000 m3u8_XZ-0.0.4/m3u8_XZ/cryptoModel.py
+-rw-rw-rw-   0        0        0     6810 2023-06-06 10:41:28.000000 m3u8_XZ-0.0.4/m3u8_XZ/xz.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:54:37.355868 m3u8_XZ-0.0.4/m3u8_XZ.egg-info/
+-rw-rw-rw-   0        0        0      835 2023-06-06 11:54:37.000000 m3u8_XZ-0.0.4/m3u8_XZ.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-06-06 11:54:37.000000 m3u8_XZ-0.0.4/m3u8_XZ.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 11:54:37.000000 m3u8_XZ-0.0.4/m3u8_XZ.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-06-06 11:54:37.000000 m3u8_XZ-0.0.4/m3u8_XZ.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 11:54:37.000000 m3u8_XZ-0.0.4/m3u8_XZ.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      522 2023-03-23 11:30:25.000000 m3u8_XZ-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-06 11:54:37.357859 m3u8_XZ-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      785 2023-06-06 11:54:18.000000 m3u8_XZ-0.0.4/setup.py
```

### Comparing `m3u8_XZ-0.0.2/LICENSE` & `m3u8_XZ-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `m3u8_XZ-0.0.2/m3u8_XZ/cryptoModel.py` & `m3u8_XZ-0.0.4/m3u8_XZ/cryptoModel.py`

 * *Files identical despite different names*

### Comparing `m3u8_XZ-0.0.2/m3u8_XZ/xz.py` & `m3u8_XZ-0.0.4/m3u8_XZ/xz.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 # IED:PyCharm
 import time
 import aiohttp
 import asyncio
 import requests as req
 import re
 import os
-from ..m3u8_XZ.cryptoModel import DecodeByte
+from .cryptoModel import DecodeByte
 
 
 class M3U8:
     """
         url: m3u8文件的url
         folder: 下载文件后存储的名字
         run(): 执行下载
     """
-    def __init__(self, url=None, folder='test', m3u8_file=None):
+    def __init__(self, url=None, folder='m3u8_XZ_test', m3u8_file=None):
         # 下载文件名
         self.file_name = folder + '.mp4'
         # 下载存储文件夹
         self.path = './down_load/' + folder + '/'
         if not os.path.exists(self.path):
             os.makedirs(self.path)
         # 缓存文件夹
@@ -97,15 +97,15 @@
         cry_obj = dict()
         if len(x_key) > 0:
             # 提取
             for item in x_key[0].split(','):
                 cry_obj[item.split('=')[0]] = item.split('=')[1].replace('"', '')
             # format
             if cry_obj['URI'] and not cry_obj['URI'].startswith('http'):
-                cry_obj['URI'] = url + cry_obj['URI']
+                cry_obj['URI'] = self.get_full_ts_url(url, cry_obj['URI'])
             # 获取key
             res = req.get(cry_obj['URI'], headers=self.headers)
             self.cry['key'] = res.content
             # 加密方式
             self.cry['method'] = cry_obj['METHOD']
             # iv值
             if cry_obj.get('IV'):
```

### Comparing `m3u8_XZ-0.0.2/pyproject.toml` & `m3u8_XZ-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `m3u8_XZ-0.0.2/setup.py` & `m3u8_XZ-0.0.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -- coding:utf-8 --
 # Time:2023-03-23 14:44
 # Author:XZ
 # File:setup.py
 # IED:PyCharm
 import setuptools
 
-with open("README.md", "r") as fh:
+with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="m3u8_XZ",
-    version="0.0.2",
+    version="0.0.4",
     author="XZ",
     author_email="345841407@qq.com",
-    description="download m3u8 video",
+    description="download m3u8 video by m3u8 url or by local m3u8 file",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    packages=setuptools.find_packages(),
+    packages=setuptools.find_packages(where="./m3u8_XZ"),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=["requests", "aiohttp", "pycryptodome"],
 )
```

