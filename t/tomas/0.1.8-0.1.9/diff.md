# Comparing `tmp/tomas-0.1.8.tar.gz` & `tmp/tomas-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tomas-0.1.8.tar", last modified: Tue Jan  3 13:22:07 2023, max compression
+gzip compressed data, was "dist/tomas-0.1.9.tar", last modified: Tue Jan  3 18:38:50 2023, max compression
```

## Comparing `tomas-0.1.8.tar` & `tomas-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 qy        (1000) qy        (1000)        0 2023-01-03 13:22:07.597991 tomas-0.1.8/
--rw-rw-r--   0 qy        (1000) qy        (1000)     1517 2022-12-06 15:08:18.000000 tomas-0.1.8/LICENSE
--rw-rw-r--   0 qy        (1000) qy        (1000)      304 2023-01-03 13:22:07.597991 tomas-0.1.8/PKG-INFO
--rw-rw-r--   0 qy        (1000) qy        (1000)        0 2022-12-06 15:08:18.000000 tomas-0.1.8/README.md
--rw-rw-r--   0 qy        (1000) qy        (1000)       38 2023-01-03 13:22:07.597991 tomas-0.1.8/setup.cfg
--rw-rw-r--   0 qy        (1000) qy        (1000)      761 2023-01-03 13:21:18.000000 tomas-0.1.8/setup.py
-drwxrwxr-x   0 qy        (1000) qy        (1000)        0 2023-01-03 13:22:07.597991 tomas-0.1.8/tomas/
--rw-rw-r--   0 qy        (1000) qy        (1000)      156 2022-12-14 06:55:26.000000 tomas-0.1.8/tomas/__init__.py
--rwxrwxr-x   0 qy        (1000) qy        (1000)    10280 2022-12-06 15:08:05.000000 tomas-0.1.8/tomas/auxi.py
--rwxrwxr-x   0 qy        (1000) qy        (1000)    12057 2022-12-15 05:25:38.000000 tomas-0.1.8/tomas/fit.py
--rwxrwxr-x   0 qy        (1000) qy        (1000)    41547 2023-01-03 13:11:36.000000 tomas-0.1.8/tomas/infer.py
--rw-rw-r--   0 qy        (1000) qy        (1000)    12277 2022-12-06 15:08:01.000000 tomas-0.1.8/tomas/lrt.py
--rwxrwxr-x   0 qy        (1000) qy        (1000)    20665 2022-12-29 12:20:48.000000 tomas-0.1.8/tomas/vis.py
-drwxrwxr-x   0 qy        (1000) qy        (1000)        0 2023-01-03 13:22:07.597991 tomas-0.1.8/tomas.egg-info/
--rw-rw-r--   0 qy        (1000) qy        (1000)      304 2023-01-03 13:22:07.000000 tomas-0.1.8/tomas.egg-info/PKG-INFO
--rw-rw-r--   0 qy        (1000) qy        (1000)      256 2023-01-03 13:22:07.000000 tomas-0.1.8/tomas.egg-info/SOURCES.txt
--rw-rw-r--   0 qy        (1000) qy        (1000)        1 2023-01-03 13:22:07.000000 tomas-0.1.8/tomas.egg-info/dependency_links.txt
--rw-rw-r--   0 qy        (1000) qy        (1000)       28 2023-01-03 13:22:07.000000 tomas-0.1.8/tomas.egg-info/requires.txt
--rw-rw-r--   0 qy        (1000) qy        (1000)        6 2023-01-03 13:22:07.000000 tomas-0.1.8/tomas.egg-info/top_level.txt
+drwxrwxr-x   0 qy        (1000) qy        (1000)        0 2023-01-03 18:38:50.226029 tomas-0.1.9/
+-rw-rw-r--   0 qy        (1000) qy        (1000)     1517 2022-12-06 15:08:18.000000 tomas-0.1.9/LICENSE
+-rw-rw-r--   0 qy        (1000) qy        (1000)      304 2023-01-03 18:38:50.226029 tomas-0.1.9/PKG-INFO
+-rw-rw-r--   0 qy        (1000) qy        (1000)        0 2022-12-06 15:08:18.000000 tomas-0.1.9/README.md
+-rw-rw-r--   0 qy        (1000) qy        (1000)       38 2023-01-03 18:38:50.226029 tomas-0.1.9/setup.cfg
+-rw-rw-r--   0 qy        (1000) qy        (1000)      761 2023-01-03 18:38:43.000000 tomas-0.1.9/setup.py
+drwxrwxr-x   0 qy        (1000) qy        (1000)        0 2023-01-03 18:38:50.226029 tomas-0.1.9/tomas/
+-rw-rw-r--   0 qy        (1000) qy        (1000)      156 2022-12-14 06:55:26.000000 tomas-0.1.9/tomas/__init__.py
+-rwxrwxr-x   0 qy        (1000) qy        (1000)    10280 2022-12-06 15:08:05.000000 tomas-0.1.9/tomas/auxi.py
+-rwxrwxr-x   0 qy        (1000) qy        (1000)    12057 2022-12-15 05:25:38.000000 tomas-0.1.9/tomas/fit.py
+-rwxrwxr-x   0 qy        (1000) qy        (1000)    41547 2023-01-03 13:11:36.000000 tomas-0.1.9/tomas/infer.py
+-rw-rw-r--   0 qy        (1000) qy        (1000)    12277 2022-12-06 15:08:01.000000 tomas-0.1.9/tomas/lrt.py
+-rwxrwxr-x   0 qy        (1000) qy        (1000)    20664 2023-01-03 18:38:19.000000 tomas-0.1.9/tomas/vis.py
+drwxrwxr-x   0 qy        (1000) qy        (1000)        0 2023-01-03 18:38:50.226029 tomas-0.1.9/tomas.egg-info/
+-rw-rw-r--   0 qy        (1000) qy        (1000)      304 2023-01-03 18:38:50.000000 tomas-0.1.9/tomas.egg-info/PKG-INFO
+-rw-rw-r--   0 qy        (1000) qy        (1000)      256 2023-01-03 18:38:50.000000 tomas-0.1.9/tomas.egg-info/SOURCES.txt
+-rw-rw-r--   0 qy        (1000) qy        (1000)        1 2023-01-03 18:38:50.000000 tomas-0.1.9/tomas.egg-info/dependency_links.txt
+-rw-rw-r--   0 qy        (1000) qy        (1000)       28 2023-01-03 18:38:50.000000 tomas-0.1.9/tomas.egg-info/requires.txt
+-rw-rw-r--   0 qy        (1000) qy        (1000)        6 2023-01-03 18:38:50.000000 tomas-0.1.9/tomas.egg-info/top_level.txt
```

### Comparing `tomas-0.1.8/LICENSE` & `tomas-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tomas-0.1.8/setup.py` & `tomas-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="tomas",
-    version="0.1.8",
+    version="0.1.9",
     license='BSD-3',
     author="Qiuyu Lian",
     author_email="qiuyu.lian@sjtu.edu.cn",
     description="A tool for TOtal-MRNA-Aware Single-cell RNA-seq data analysis",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
```

### Comparing `tomas-0.1.8/tomas/auxi.py` & `tomas-0.1.9/tomas/auxi.py`

 * *Files identical despite different names*

### Comparing `tomas-0.1.8/tomas/fit.py` & `tomas-0.1.9/tomas/fit.py`

 * *Files identical despite different names*

### Comparing `tomas-0.1.8/tomas/infer.py` & `tomas-0.1.9/tomas/infer.py`

 * *Files identical despite different names*

### Comparing `tomas-0.1.8/tomas/lrt.py` & `tomas-0.1.9/tomas/lrt.py`

 * *Files identical despite different names*

### Comparing `tomas-0.1.8/tomas/vis.py` & `tomas-0.1.9/tomas/vis.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     
     x = np.log2(r_list)
     
     xy_lim = [math.floor(np.min(x)), math.ceil(np.max(x))] #[np.log2(1)-6, np.log2(1)+6] #[np.floor(v_min), np.floor(v_max)]
     x_m = round(np.mean(x))
     x_margin = np.max(np.array(xy_lim)-x_m)
     #xy_ticks = np.arange(xy_lim[0]+2, xy_lim[1], step=2)
-    xy_ticks = np.arrange(x_m-x_margin, x_m+x_margin+1, step=1)
+    xy_ticks = np.arange(x_m-x_margin, x_m+x_margin+1, step=1)
     xy_ticks = xy_ticks[xy_ticks>0]
     
     if rm_outlier:
         x_shrinkage = rm_outliers(x)
     else:
         x_shrinkage = x
```

