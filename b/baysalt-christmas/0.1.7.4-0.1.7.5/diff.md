# Comparing `tmp/baysalt_christmas-0.1.7.4.tar.gz` & `tmp/baysalt_christmas-0.1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baysalt_christmas-0.1.7.4.tar", last modified: Thu May 25 08:49:35 2023, max compression
+gzip compressed data, was "baysalt_christmas-0.1.7.5.tar", last modified: Tue Jun  6 09:11:06 2023, max compression
```

## Comparing `baysalt_christmas-0.1.7.4.tar` & `baysalt_christmas-0.1.7.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-05-25 08:49:35.910997 baysalt_christmas-0.1.7.4/
--rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-05-18 11:12:41.000000 baysalt_christmas-0.1.7.4/.DS_Store
--rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.7.4/MANIFEST.in
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-05-25 08:49:35.910856 baysalt_christmas-0.1.7.4/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.7.4/README.md
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-05-25 08:49:35.905585 baysalt_christmas-0.1.7.4/baysalt_christmas.egg-info/
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-05-25 08:49:35.000000 baysalt_christmas-0.1.7.4/baysalt_christmas.egg-info/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)      729 2023-05-25 08:49:35.000000 baysalt_christmas-0.1.7.4/baysalt_christmas.egg-info/SOURCES.txt
--rw-r--r--   0 christmas   (501) staff       (20)        1 2023-05-25 08:49:35.000000 baysalt_christmas-0.1.7.4/baysalt_christmas.egg-info/dependency_links.txt
--rw-r--r--   0 christmas   (501) staff       (20)       30 2023-05-25 08:49:35.000000 baysalt_christmas-0.1.7.4/baysalt_christmas.egg-info/requires.txt
--rw-r--r--   0 christmas   (501) staff       (20)       10 2023-05-25 08:49:35.000000 baysalt_christmas-0.1.7.4/baysalt_christmas.egg-info/top_level.txt
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-05-25 08:49:35.907886 baysalt_christmas-0.1.7.4/christmas/
--rw-r--r--   0 christmas   (501) staff       (20)    20844 2023-05-25 08:49:22.000000 baysalt_christmas-0.1.7.4/christmas/Blogging.py
--rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.7.4/christmas/S_DateTime.py
--rw-r--r--   0 christmas   (501) staff       (20)      445 2023-04-23 12:43:18.000000 baysalt_christmas-0.1.7.4/christmas/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     4676 2023-05-17 09:02:10.000000 baysalt_christmas-0.1.7.4/christmas/commonCode.py
--rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.7.4/christmas/cprintf.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-05-25 08:49:35.909709 baysalt_christmas-0.1.7.4/christmas/mncPy/
--rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.4/christmas/mncPy/.gitignore
--rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.4/christmas/mncPy/LICENSE
--rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.7.4/christmas/mncPy/__init__.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-05-25 08:49:35.910511 baysalt_christmas-0.1.7.4/christmas/mncPy/__pycache__/
--rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.7.4/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.4/christmas/mncPy/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.4/christmas/mncPy/__pycache__/compress.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.7.4/christmas/mncPy/common.py
--rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.7.4/christmas/mncPy/compress.py
--rw-r--r--   0 christmas   (501) staff       (20)     3554 2023-03-29 02:58:20.000000 baysalt_christmas-0.1.7.4/christmas/processBar.py
--rw-r--r--   0 christmas   (501) staff       (20)     3473 2023-04-13 06:21:12.000000 baysalt_christmas-0.1.7.4/christmas/read_conf.py
--rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.7.4/christmas/server_info.py
--rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.7.4/run_twine.py
--rw-r--r--   0 christmas   (501) staff       (20)       38 2023-05-25 08:49:35.911051 baysalt_christmas-0.1.7.4/setup.cfg
--rw-r--r--   0 christmas   (501) staff       (20)      796 2023-05-25 08:49:31.000000 baysalt_christmas-0.1.7.4/setup.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-06 09:11:06.855027 baysalt_christmas-0.1.7.5/
+-rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-05-18 11:12:41.000000 baysalt_christmas-0.1.7.5/.DS_Store
+-rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.7.5/MANIFEST.in
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-06-06 09:11:06.854866 baysalt_christmas-0.1.7.5/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.7.5/README.md
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-06 09:11:06.848504 baysalt_christmas-0.1.7.5/baysalt_christmas.egg-info/
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-06-06 09:11:06.000000 baysalt_christmas-0.1.7.5/baysalt_christmas.egg-info/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)      729 2023-06-06 09:11:06.000000 baysalt_christmas-0.1.7.5/baysalt_christmas.egg-info/SOURCES.txt
+-rw-r--r--   0 christmas   (501) staff       (20)        1 2023-06-06 09:11:06.000000 baysalt_christmas-0.1.7.5/baysalt_christmas.egg-info/dependency_links.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       30 2023-06-06 09:11:06.000000 baysalt_christmas-0.1.7.5/baysalt_christmas.egg-info/requires.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       10 2023-06-06 09:11:06.000000 baysalt_christmas-0.1.7.5/baysalt_christmas.egg-info/top_level.txt
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-06 09:11:06.850903 baysalt_christmas-0.1.7.5/christmas/
+-rw-r--r--   0 christmas   (501) staff       (20)    20844 2023-05-25 08:49:22.000000 baysalt_christmas-0.1.7.5/christmas/Blogging.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.7.5/christmas/S_DateTime.py
+-rw-r--r--   0 christmas   (501) staff       (20)      445 2023-04-23 12:43:18.000000 baysalt_christmas-0.1.7.5/christmas/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4676 2023-05-17 09:02:10.000000 baysalt_christmas-0.1.7.5/christmas/commonCode.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.7.5/christmas/cprintf.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-06 09:11:06.853590 baysalt_christmas-0.1.7.5/christmas/mncPy/
+-rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.5/christmas/mncPy/.gitignore
+-rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.5/christmas/mncPy/LICENSE
+-rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.7.5/christmas/mncPy/__init__.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-06 09:11:06.854434 baysalt_christmas-0.1.7.5/christmas/mncPy/__pycache__/
+-rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.7.5/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.5/christmas/mncPy/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.5/christmas/mncPy/__pycache__/compress.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.7.5/christmas/mncPy/common.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.7.5/christmas/mncPy/compress.py
+-rw-r--r--   0 christmas   (501) staff       (20)     3554 2023-03-29 02:58:20.000000 baysalt_christmas-0.1.7.5/christmas/processBar.py
+-rw-r--r--   0 christmas   (501) staff       (20)     3473 2023-04-13 06:21:12.000000 baysalt_christmas-0.1.7.5/christmas/read_conf.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.7.5/christmas/server_info.py
+-rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.7.5/run_twine.py
+-rw-r--r--   0 christmas   (501) staff       (20)       38 2023-06-06 09:11:06.855071 baysalt_christmas-0.1.7.5/setup.cfg
+-rw-r--r--   0 christmas   (501) staff       (20)      796 2023-06-06 09:11:05.000000 baysalt_christmas-0.1.7.5/setup.py
```

### Comparing `baysalt_christmas-0.1.7.4/.DS_Store` & `baysalt_christmas-0.1.7.5/.DS_Store`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.4/PKG-INFO` & `baysalt_christmas-0.1.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt_christmas
-Version: 0.1.7.4
+Version: 0.1.7.5
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.7.4/README.md` & `baysalt_christmas-0.1.7.5/README.md`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.4/baysalt_christmas.egg-info/PKG-INFO` & `baysalt_christmas-0.1.7.5/baysalt_christmas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt-christmas
-Version: 0.1.7.4
+Version: 0.1.7.5
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.7.4/baysalt_christmas.egg-info/SOURCES.txt` & `baysalt_christmas-0.1.7.5/baysalt_christmas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.4/christmas/Blogging.py` & `baysalt_christmas-0.1.7.5/christmas/Blogging.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.4/christmas/S_DateTime.py` & `baysalt_christmas-0.1.7.5/christmas/S_DateTime.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.4/christmas/commonCode.py` & `baysalt_christmas-0.1.7.5/christmas/commonCode.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.4/christmas/cprintf.py` & `baysalt_christmas-0.1.7.5/christmas/cprintf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.4/christmas/mncPy/.gitignore` & `baysalt_christmas-0.1.7.5/christmas/mncPy/.gitignore`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.4/christmas/mncPy/LICENSE` & `baysalt_christmas-0.1.7.5/christmas/mncPy/LICENSE`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.4/christmas/mncPy/__pycache__/common.cpython-39.pyc` & `baysalt_christmas-0.1.7.5/christmas/mncPy/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.4/christmas/mncPy/__pycache__/compress.cpython-39.pyc` & `baysalt_christmas-0.1.7.5/christmas/mncPy/__pycache__/compress.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.4/christmas/mncPy/common.py` & `baysalt_christmas-0.1.7.5/christmas/mncPy/common.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.4/christmas/mncPy/compress.py` & `baysalt_christmas-0.1.7.5/christmas/mncPy/compress.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.4/christmas/processBar.py` & `baysalt_christmas-0.1.7.5/christmas/processBar.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.4/christmas/read_conf.py` & `baysalt_christmas-0.1.7.5/christmas/read_conf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.4/christmas/server_info.py` & `baysalt_christmas-0.1.7.5/christmas/server_info.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.4/setup.py` & `baysalt_christmas-0.1.7.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="baysalt_christmas",
-    version="0.1.7.4",
+    version="0.1.7.5",
     author="Christmas",
     author_email="273519355@qq.com",
     description="Some simple tools for Christmas",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     include_package_data=True,
```

