# Comparing `tmp/lazysdk-0.1.1.tar.gz` & `tmp/lazysdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazysdk-0.1.1.tar", last modified: Sat Feb 25 06:33:58 2023, max compression
+gzip compressed data, was "lazysdk-0.1.2.tar", last modified: Tue Jun  6 09:54:28 2023, max compression
```

## Comparing `lazysdk-0.1.1.tar` & `lazysdk-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-02-25 06:33:58.776487 lazysdk-0.1.1/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1369 2023-02-25 06:33:58.776364 lazysdk-0.1.1/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      993 2023-02-23 03:14:55.000000 lazysdk-0.1.1/README.md
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-02-25 06:33:58.775561 lazysdk-0.1.1/lazysdk/
--rw-r--r--   0 zeroseeker   (501) staff       (20)      402 2023-02-23 03:44:47.000000 lazysdk-0.1.1/lazysdk/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      555 2023-02-23 03:14:55.000000 lazysdk-0.1.1/lazysdk/lazybase64.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     6829 2023-02-23 03:14:55.000000 lazysdk-0.1.1/lazysdk/lazydict.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     3024 2023-02-23 03:14:55.000000 lazysdk-0.1.1/lazysdk/lazyenv.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    13091 2023-02-25 06:33:34.000000 lazysdk-0.1.1/lazysdk/lazyexcel.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    20267 2023-02-23 03:14:55.000000 lazysdk-0.1.1/lazysdk/lazyfile.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      727 2023-02-23 03:14:55.000000 lazysdk-0.1.1/lazysdk/lazyflask.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      607 2023-02-23 03:41:38.000000 lazysdk-0.1.1/lazysdk/lazyid.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      451 2023-02-23 03:14:55.000000 lazysdk-0.1.1/lazysdk/lazyip.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1112 2023-02-23 03:14:55.000000 lazysdk-0.1.1/lazysdk/lazymd5.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     4305 2023-02-23 03:14:55.000000 lazysdk-0.1.1/lazysdk/lazypath.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     5079 2023-02-23 03:14:55.000000 lazysdk-0.1.1/lazysdk/lazyprocess.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      546 2023-02-23 03:14:55.000000 lazysdk-0.1.1/lazysdk/lazyproxies.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1482 2023-02-23 03:14:55.000000 lazysdk-0.1.1/lazysdk/lazyrandom.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    37918 2023-02-23 03:14:55.000000 lazysdk-0.1.1/lazysdk/lazyredis.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     2511 2023-02-23 03:14:55.000000 lazysdk-0.1.1/lazysdk/lazyrequests.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1448 2023-02-23 03:14:55.000000 lazysdk-0.1.1/lazysdk/lazytext.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    23199 2023-02-23 03:14:55.000000 lazysdk-0.1.1/lazysdk/lazytime.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     3783 2023-02-23 03:14:55.000000 lazysdk-0.1.1/lazysdk/lazyua.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     8386 2023-02-23 03:14:55.000000 lazysdk-0.1.1/lazysdk/lazywebhook.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-02-25 06:33:58.776167 lazysdk-0.1.1/lazysdk.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1369 2023-02-25 06:33:58.000000 lazysdk-0.1.1/lazysdk.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      584 2023-02-25 06:33:58.000000 lazysdk-0.1.1/lazysdk.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-02-25 06:33:58.000000 lazysdk-0.1.1/lazysdk.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)      130 2023-02-25 06:33:58.000000 lazysdk-0.1.1/lazysdk.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        8 2023-02-25 06:33:58.000000 lazysdk-0.1.1/lazysdk.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-02-25 06:33:58.776535 lazysdk-0.1.1/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1066 2023-02-25 06:33:34.000000 lazysdk-0.1.1/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-06 09:54:28.022498 lazysdk-0.1.2/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1369 2023-06-06 09:54:28.022267 lazysdk-0.1.2/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      993 2023-02-23 03:14:55.000000 lazysdk-0.1.2/README.md
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-06 09:54:28.020119 lazysdk-0.1.2/lazysdk/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      402 2023-02-23 03:44:47.000000 lazysdk-0.1.2/lazysdk/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      389 2023-06-06 09:15:38.000000 lazysdk-0.1.2/lazysdk/lazyCrypto.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      555 2023-02-23 03:14:55.000000 lazysdk-0.1.2/lazysdk/lazybase64.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     6829 2023-02-23 03:14:55.000000 lazysdk-0.1.2/lazysdk/lazydict.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     3024 2023-02-23 03:14:55.000000 lazysdk-0.1.2/lazysdk/lazyenv.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    13091 2023-02-25 06:33:34.000000 lazysdk-0.1.2/lazysdk/lazyexcel.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    20267 2023-02-23 03:14:55.000000 lazysdk-0.1.2/lazysdk/lazyfile.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      727 2023-02-23 03:14:55.000000 lazysdk-0.1.2/lazysdk/lazyflask.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      607 2023-02-23 03:41:38.000000 lazysdk-0.1.2/lazysdk/lazyid.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      451 2023-02-23 03:14:55.000000 lazysdk-0.1.2/lazysdk/lazyip.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    28834 2023-06-06 09:53:35.000000 lazysdk-0.1.2/lazysdk/lazym3u8.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1112 2023-02-23 03:14:55.000000 lazysdk-0.1.2/lazysdk/lazymd5.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     4305 2023-02-23 03:14:55.000000 lazysdk-0.1.2/lazysdk/lazypath.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     5079 2023-02-23 03:14:55.000000 lazysdk-0.1.2/lazysdk/lazyprocess.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      546 2023-02-23 03:14:55.000000 lazysdk-0.1.2/lazysdk/lazyproxies.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1482 2023-02-23 03:14:55.000000 lazysdk-0.1.2/lazysdk/lazyrandom.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    37918 2023-02-23 03:14:55.000000 lazysdk-0.1.2/lazysdk/lazyredis.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     2511 2023-02-23 03:14:55.000000 lazysdk-0.1.2/lazysdk/lazyrequests.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1448 2023-02-23 03:14:55.000000 lazysdk-0.1.2/lazysdk/lazytext.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    23199 2023-02-23 03:14:55.000000 lazysdk-0.1.2/lazysdk/lazytime.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     3783 2023-02-23 03:14:55.000000 lazysdk-0.1.2/lazysdk/lazyua.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     8386 2023-02-23 03:14:55.000000 lazysdk-0.1.2/lazysdk/lazywebhook.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-06 09:54:28.021459 lazysdk-0.1.2/lazysdk.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1369 2023-06-06 09:54:27.000000 lazysdk-0.1.2/lazysdk.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      626 2023-06-06 09:54:27.000000 lazysdk-0.1.2/lazysdk.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-06-06 09:54:27.000000 lazysdk-0.1.2/lazysdk.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      163 2023-06-06 09:54:27.000000 lazysdk-0.1.2/lazysdk.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        8 2023-06-06 09:54:27.000000 lazysdk-0.1.2/lazysdk.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-06-06 09:54:28.022561 lazysdk-0.1.2/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1121 2023-06-06 09:01:19.000000 lazysdk-0.1.2/setup.py
```

### Comparing `lazysdk-0.1.1/PKG-INFO` & `lazysdk-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazysdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: 基于Python的懒人包
 Home-page: https://gitee.com/ZeroSeeker/lazysdk
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lazysdk-0.1.1/README.md` & `lazysdk-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.1/lazysdk/lazybase64.py` & `lazysdk-0.1.2/lazysdk/lazybase64.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.1/lazysdk/lazydict.py` & `lazysdk-0.1.2/lazysdk/lazydict.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.1/lazysdk/lazyenv.py` & `lazysdk-0.1.2/lazysdk/lazyenv.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.1/lazysdk/lazyexcel.py` & `lazysdk-0.1.2/lazysdk/lazyexcel.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.1/lazysdk/lazyfile.py` & `lazysdk-0.1.2/lazysdk/lazyfile.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.1/lazysdk/lazyflask.py` & `lazysdk-0.1.2/lazysdk/lazyflask.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.1/lazysdk/lazyid.py` & `lazysdk-0.1.2/lazysdk/lazyid.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.1/lazysdk/lazymd5.py` & `lazysdk-0.1.2/lazysdk/lazymd5.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.1/lazysdk/lazypath.py` & `lazysdk-0.1.2/lazysdk/lazypath.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.1/lazysdk/lazyprocess.py` & `lazysdk-0.1.2/lazysdk/lazyprocess.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.1/lazysdk/lazyproxies.py` & `lazysdk-0.1.2/lazysdk/lazyproxies.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.1/lazysdk/lazyrandom.py` & `lazysdk-0.1.2/lazysdk/lazyrandom.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.1/lazysdk/lazyredis.py` & `lazysdk-0.1.2/lazysdk/lazyredis.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.1/lazysdk/lazyrequests.py` & `lazysdk-0.1.2/lazysdk/lazyrequests.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.1/lazysdk/lazytext.py` & `lazysdk-0.1.2/lazysdk/lazytext.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.1/lazysdk/lazytime.py` & `lazysdk-0.1.2/lazysdk/lazytime.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.1/lazysdk/lazyua.py` & `lazysdk-0.1.2/lazysdk/lazyua.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.1/lazysdk/lazywebhook.py` & `lazysdk-0.1.2/lazysdk/lazywebhook.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.1/lazysdk.egg-info/PKG-INFO` & `lazysdk-0.1.2/lazysdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazysdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: 基于Python的懒人包
 Home-page: https://gitee.com/ZeroSeeker/lazysdk
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lazysdk-0.1.1/lazysdk.egg-info/SOURCES.txt` & `lazysdk-0.1.2/lazysdk.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 README.md
 setup.py
 lazysdk/__init__.py
+lazysdk/lazyCrypto.py
 lazysdk/lazybase64.py
 lazysdk/lazydict.py
 lazysdk/lazyenv.py
 lazysdk/lazyexcel.py
 lazysdk/lazyfile.py
 lazysdk/lazyflask.py
 lazysdk/lazyid.py
 lazysdk/lazyip.py
+lazysdk/lazym3u8.py
 lazysdk/lazymd5.py
 lazysdk/lazypath.py
 lazysdk/lazyprocess.py
 lazysdk/lazyproxies.py
 lazysdk/lazyrandom.py
 lazysdk/lazyredis.py
 lazysdk/lazyrequests.py
```

### Comparing `lazysdk-0.1.1/setup.py` & `lazysdk-0.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lazysdk",
-    version="0.1.1",
+    version="0.1.2",
     description="基于Python的懒人包",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ZeroSeeker",
     author_email="zeroseeker@foxmail.com",
     url="https://gitee.com/ZeroSeeker/lazysdk",
     packages=setuptools.find_packages(),
@@ -31,10 +31,12 @@
         'requests==2.27.1',
         'envx>=1.0.1',
         'pytz==2022.1',
         'redis==4.1.0',
         'ua_parser==0.10.0',
         'openpyxl==3.0.9',
         'xlrd==2.0.1',
-        'numpy==1.22.0'
+        'numpy==1.22.0',
+        'm3u8==3.5.0',
+        'pycryptodome==3.10.1'
     ]
 )
```

