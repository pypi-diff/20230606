# Comparing `tmp/pipiyiTools-0.0.1.tar.gz` & `tmp/pipiyiTools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pipiyiTools-0.0.1.tar", last modified: Tue May 30 10:09:46 2023, max compression
+gzip compressed data, was "dist/pipiyiTools-0.0.3.tar", last modified: Tue Jun  6 09:02:38 2023, max compression
```

## Comparing `pipiyiTools-0.0.1.tar` & `pipiyiTools-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 xiaopipi   (501) staff       (20)        0 2023-05-30 10:09:46.000000 pipiyiTools-0.0.1/
--rw-r--r--   0 xiaopipi   (501) staff       (20)      917 2023-05-30 10:09:46.000000 pipiyiTools-0.0.1/PKG-INFO
--rw-r--r--   0 xiaopipi   (501) staff       (20)      288 2023-05-30 08:07:51.000000 pipiyiTools-0.0.1/README.md
-drwxr-xr-x   0 xiaopipi   (501) staff       (20)        0 2023-05-30 10:09:46.000000 pipiyiTools-0.0.1/pipiyiTools/
--rw-r--r--   0 xiaopipi   (501) staff       (20)     2589 2023-05-23 08:46:36.000000 pipiyiTools-0.0.1/pipiyiTools/EpubSpliter.py
--rw-r--r--   0 xiaopipi   (501) staff       (20)     1058 2023-05-25 05:43:31.000000 pipiyiTools-0.0.1/pipiyiTools/FileOperation.py
--rw-r--r--   0 xiaopipi   (501) staff       (20)     1134 2023-05-26 09:22:54.000000 pipiyiTools-0.0.1/pipiyiTools/ListQueue.py
--rw-r--r--   0 xiaopipi   (501) staff       (20)     1928 2023-05-26 09:49:22.000000 pipiyiTools-0.0.1/pipiyiTools/Log.py
--rw-r--r--   0 xiaopipi   (501) staff       (20)     2070 2023-05-23 06:29:36.000000 pipiyiTools-0.0.1/pipiyiTools/MyRequest.py
--rw-r--r--   0 xiaopipi   (501) staff       (20)     6711 2023-05-28 14:14:08.000000 pipiyiTools-0.0.1/pipiyiTools/PooledBase.py
--rw-r--r--   0 xiaopipi   (501) staff       (20)      972 2023-05-23 04:18:08.000000 pipiyiTools-0.0.1/pipiyiTools/Storage.py
--rw-r--r--   0 xiaopipi   (501) staff       (20)        0 2023-05-30 10:06:54.000000 pipiyiTools-0.0.1/pipiyiTools/__init__.py
-drwxr-xr-x   0 xiaopipi   (501) staff       (20)        0 2023-05-30 10:09:46.000000 pipiyiTools-0.0.1/pipiyiTools.egg-info/
--rw-r--r--   0 xiaopipi   (501) staff       (20)      917 2023-05-30 10:09:46.000000 pipiyiTools-0.0.1/pipiyiTools.egg-info/PKG-INFO
--rw-r--r--   0 xiaopipi   (501) staff       (20)      390 2023-05-30 10:09:46.000000 pipiyiTools-0.0.1/pipiyiTools.egg-info/SOURCES.txt
--rw-r--r--   0 xiaopipi   (501) staff       (20)        1 2023-05-30 10:09:46.000000 pipiyiTools-0.0.1/pipiyiTools.egg-info/dependency_links.txt
--rw-r--r--   0 xiaopipi   (501) staff       (20)       43 2023-05-30 10:09:46.000000 pipiyiTools-0.0.1/pipiyiTools.egg-info/requires.txt
--rw-r--r--   0 xiaopipi   (501) staff       (20)       12 2023-05-30 10:09:46.000000 pipiyiTools-0.0.1/pipiyiTools.egg-info/top_level.txt
--rw-r--r--   0 xiaopipi   (501) staff       (20)       38 2023-05-30 10:09:46.000000 pipiyiTools-0.0.1/setup.cfg
--rw-r--r--   0 xiaopipi   (501) staff       (20)     1002 2023-05-30 10:09:22.000000 pipiyiTools-0.0.1/setup.py
+drwxr-xr-x   0 xiaopipi   (501) staff       (20)        0 2023-06-06 09:02:38.000000 pipiyiTools-0.0.3/
+-rw-r--r--   0 xiaopipi   (501) staff       (20)      975 2023-06-06 09:02:38.000000 pipiyiTools-0.0.3/PKG-INFO
+-rw-r--r--   0 xiaopipi   (501) staff       (20)      314 2023-06-06 08:59:34.000000 pipiyiTools-0.0.3/README.md
+drwxr-xr-x   0 xiaopipi   (501) staff       (20)        0 2023-06-06 09:02:38.000000 pipiyiTools-0.0.3/pipiyiTools/
+-rw-r--r--   0 xiaopipi   (501) staff       (20)     2589 2023-05-23 08:46:36.000000 pipiyiTools-0.0.3/pipiyiTools/EpubSpliter.py
+-rw-r--r--   0 xiaopipi   (501) staff       (20)     1058 2023-05-25 05:43:31.000000 pipiyiTools-0.0.3/pipiyiTools/FileOperation.py
+-rw-r--r--   0 xiaopipi   (501) staff       (20)     1385 2023-06-06 09:02:18.000000 pipiyiTools-0.0.3/pipiyiTools/ListQueue.py
+-rw-r--r--   0 xiaopipi   (501) staff       (20)     1928 2023-05-26 09:49:22.000000 pipiyiTools-0.0.3/pipiyiTools/Log.py
+-rw-r--r--   0 xiaopipi   (501) staff       (20)     2070 2023-05-23 06:29:36.000000 pipiyiTools-0.0.3/pipiyiTools/MyRequest.py
+-rw-r--r--   0 xiaopipi   (501) staff       (20)     6711 2023-05-28 14:14:08.000000 pipiyiTools-0.0.3/pipiyiTools/PooledBase.py
+-rw-r--r--   0 xiaopipi   (501) staff       (20)      972 2023-05-23 04:18:08.000000 pipiyiTools-0.0.3/pipiyiTools/Storage.py
+-rw-r--r--   0 xiaopipi   (501) staff       (20)        0 2023-05-30 10:06:54.000000 pipiyiTools-0.0.3/pipiyiTools/__init__.py
+drwxr-xr-x   0 xiaopipi   (501) staff       (20)        0 2023-06-06 09:02:38.000000 pipiyiTools-0.0.3/pipiyiTools.egg-info/
+-rw-r--r--   0 xiaopipi   (501) staff       (20)      975 2023-06-06 09:02:38.000000 pipiyiTools-0.0.3/pipiyiTools.egg-info/PKG-INFO
+-rw-r--r--   0 xiaopipi   (501) staff       (20)      390 2023-06-06 09:02:38.000000 pipiyiTools-0.0.3/pipiyiTools.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaopipi   (501) staff       (20)        1 2023-06-06 09:02:38.000000 pipiyiTools-0.0.3/pipiyiTools.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaopipi   (501) staff       (20)       43 2023-06-06 09:02:38.000000 pipiyiTools-0.0.3/pipiyiTools.egg-info/requires.txt
+-rw-r--r--   0 xiaopipi   (501) staff       (20)       12 2023-06-06 09:02:38.000000 pipiyiTools-0.0.3/pipiyiTools.egg-info/top_level.txt
+-rw-r--r--   0 xiaopipi   (501) staff       (20)       38 2023-06-06 09:02:38.000000 pipiyiTools-0.0.3/setup.cfg
+-rw-r--r--   0 xiaopipi   (501) staff       (20)     1005 2023-06-06 09:02:25.000000 pipiyiTools-0.0.3/setup.py
```

### Comparing `pipiyiTools-0.0.1/PKG-INFO` & `pipiyiTools-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: pipiyiTools
-Version: 0.0.1
+Version: 0.0.3
 Summary: Personal tool library
 Home-page: UNKNOWN
 Author: pipiyi
 Author-email: smallpoliao@gmail.com
 License: UNKNOWN
 Description: 
         # 一个小工具合集
         
-        ----------
+        ---
+        
+        - EpubSpliter 创建 epub 电子书
+        - FileOperation 操作文件
+        - ListQueue list 队列
+        - Log 日志
+        - MyRequest 一个带随机 header 的 requests
+        - PooledBase 数据库操作
+        - Storage 基于 heapq 队列
+        
+        > 编译:python3 setup.py sdist bdist_wheel
+        > 上传:twine upload dist/\*
         
-        - EpubSpliter      创建epub电子书
-        - FileOperation    操作文件
-        - ListQueue        list 队列
-        - Log              日志
-        - MyRequest        一个带随机header的requests
-        - PooledBase       数据库操作
-        - Storage          基于heapq队列
 Keywords: python
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `pipiyiTools-0.0.1/pipiyiTools/EpubSpliter.py` & `pipiyiTools-0.0.3/pipiyiTools/EpubSpliter.py`

 * *Files identical despite different names*

### Comparing `pipiyiTools-0.0.1/pipiyiTools/FileOperation.py` & `pipiyiTools-0.0.3/pipiyiTools/FileOperation.py`

 * *Files identical despite different names*

### Comparing `pipiyiTools-0.0.1/pipiyiTools/ListQueue.py` & `pipiyiTools-0.0.3/pipiyiTools/ListQueue.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 """
 @Project ：内容队列
 @File    ：ListQueue.py
 @Author  ：Pipiyi
-@Date    ：24/5/23 21:35 
+@Date    ：24 /5/23 21:35 
 """
 
 
 class ListQueue:
     def __init__(self):
         self.data = {}
 
     def get_all(self, key):
         return self.data.get(key, [])
 
+    def set_items(self, key, value):
+        """写入内容,如果有指定key则覆盖，没有则写入
+
+        Args:
+            key (_type_): _description_
+            value (_type_): _description_
+        """
+        self.data["key"] = value
+
     def put(self, key, item):
         """
         压入内容
         :param key:
         :param item:
         :return:
         """
```

### Comparing `pipiyiTools-0.0.1/pipiyiTools/Log.py` & `pipiyiTools-0.0.3/pipiyiTools/Log.py`

 * *Files identical despite different names*

### Comparing `pipiyiTools-0.0.1/pipiyiTools/MyRequest.py` & `pipiyiTools-0.0.3/pipiyiTools/MyRequest.py`

 * *Files identical despite different names*

### Comparing `pipiyiTools-0.0.1/pipiyiTools/PooledBase.py` & `pipiyiTools-0.0.3/pipiyiTools/PooledBase.py`

 * *Files identical despite different names*

### Comparing `pipiyiTools-0.0.1/pipiyiTools/Storage.py` & `pipiyiTools-0.0.3/pipiyiTools/Storage.py`

 * *Files identical despite different names*

### Comparing `pipiyiTools-0.0.1/pipiyiTools.egg-info/PKG-INFO` & `pipiyiTools-0.0.3/pipiyiTools.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: pipiyiTools
-Version: 0.0.1
+Version: 0.0.3
 Summary: Personal tool library
 Home-page: UNKNOWN
 Author: pipiyi
 Author-email: smallpoliao@gmail.com
 License: UNKNOWN
 Description: 
         # 一个小工具合集
         
-        ----------
+        ---
+        
+        - EpubSpliter 创建 epub 电子书
+        - FileOperation 操作文件
+        - ListQueue list 队列
+        - Log 日志
+        - MyRequest 一个带随机 header 的 requests
+        - PooledBase 数据库操作
+        - Storage 基于 heapq 队列
+        
+        > 编译:python3 setup.py sdist bdist_wheel
+        > 上传:twine upload dist/\*
         
-        - EpubSpliter      创建epub电子书
-        - FileOperation    操作文件
-        - ListQueue        list 队列
-        - Log              日志
-        - MyRequest        一个带随机header的requests
-        - PooledBase       数据库操作
-        - Storage          基于heapq队列
 Keywords: python
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `pipiyiTools-0.0.1/setup.py` & `pipiyiTools-0.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
-DESCRIPTION = 'Personal tool library'
+VERSION = "0.0.3"
+DESCRIPTION = "Personal tool library"
 
 # Setting up
 setup(
     name="pipiyiTools",
     version=VERSION,
     author="pipiyi",
     author_email="smallpoliao@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['requests', 'ebooklib', 'colorlog','dbutils','pymysql'],
-    keywords=['python'],
-    setup_requires=['wheel'],
+    install_requires=["requests", "ebooklib", "colorlog", "dbutils", "pymysql"],
+    keywords=["python"],
+    setup_requires=["wheel"],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
-    ]
+    ],
 )
```

