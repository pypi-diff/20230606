# Comparing `tmp/lazyearth-1.0.7.tar.gz` & `tmp/lazyearth-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyearth-1.0.7.tar", last modified: Tue Mar 21 04:22:05 2023, max compression
+gzip compressed data, was "lazyearth-1.0.8.tar", last modified: Tue Mar 21 04:34:11 2023, max compression
```

## Comparing `lazyearth-1.0.7.tar` & `lazyearth-1.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-21 04:22:05.074000 lazyearth-1.0.7/
--rw-rw-rw-   0        0        0     1068 2022-07-25 06:10:12.000000 lazyearth-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     1089 2022-07-25 06:10:12.000000 lazyearth-1.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0     1316 2023-03-21 04:22:05.052000 lazyearth-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      689 2022-07-27 03:46:26.000000 lazyearth-1.0.7/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-21 04:22:04.722000 lazyearth-1.0.7/lazyearth/
--rw-rw-rw-   0        0        0      324 2023-03-21 04:11:00.000000 lazyearth-1.0.7/lazyearth/__init__.py
--rw-rw-rw-   0        0        0    65307 2023-03-21 04:18:58.000000 lazyearth-1.0.7/lazyearth/mainfile.py
--rw-rw-rw-   0        0        0      394 2022-07-27 10:08:55.000000 lazyearth-1.0.7/lazyearth/test_mainfile.py
-drwxrwxrwx   0        0        0        0 2023-03-21 04:22:05.032000 lazyearth-1.0.7/lazyearth.egg-info/
--rw-rw-rw-   0        0        0     1316 2023-03-21 04:22:03.000000 lazyearth-1.0.7/lazyearth.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-03-21 04:22:03.000000 lazyearth-1.0.7/lazyearth.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-21 04:22:03.000000 lazyearth-1.0.7/lazyearth.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-03-21 04:22:03.000000 lazyearth-1.0.7/lazyearth.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-21 04:22:03.000000 lazyearth-1.0.7/lazyearth.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-03-21 04:22:05.069000 lazyearth-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1402 2023-03-21 04:21:40.000000 lazyearth-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-21 04:34:11.801000 lazyearth-1.0.8/
+-rw-rw-rw-   0        0        0     1068 2022-07-25 06:10:12.000000 lazyearth-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1089 2022-07-25 06:10:12.000000 lazyearth-1.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     1316 2023-03-21 04:34:11.748000 lazyearth-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      689 2022-07-27 03:46:26.000000 lazyearth-1.0.8/README.rst
+drwxrwxrwx   0        0        0        0 2023-03-21 04:34:11.411000 lazyearth-1.0.8/lazyearth/
+-rw-rw-rw-   0        0        0      324 2023-03-21 04:33:40.000000 lazyearth-1.0.8/lazyearth/__init__.py
+-rw-rw-rw-   0        0        0    65307 2023-03-21 04:18:58.000000 lazyearth-1.0.8/lazyearth/mainfile.py
+-rw-rw-rw-   0        0        0      394 2022-07-27 10:08:55.000000 lazyearth-1.0.8/lazyearth/test_mainfile.py
+drwxrwxrwx   0        0        0        0 2023-03-21 04:34:11.723000 lazyearth-1.0.8/lazyearth.egg-info/
+-rw-rw-rw-   0        0        0     1316 2023-03-21 04:34:09.000000 lazyearth-1.0.8/lazyearth.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-03-21 04:34:10.000000 lazyearth-1.0.8/lazyearth.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-21 04:34:09.000000 lazyearth-1.0.8/lazyearth.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-03-21 04:34:10.000000 lazyearth-1.0.8/lazyearth.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-03-21 04:34:10.000000 lazyearth-1.0.8/lazyearth.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-03-21 04:34:11.797000 lazyearth-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1402 2023-03-21 04:33:30.000000 lazyearth-1.0.8/setup.py
```

### Comparing `lazyearth-1.0.7/LICENSE` & `lazyearth-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lazyearth-1.0.7/LICENSE.txt` & `lazyearth-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lazyearth-1.0.7/PKG-INFO` & `lazyearth-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazyearth
-Version: 1.0.7
+Version: 1.0.8
 Summary: Library for earth science
 Home-page: https://github.com/Tun555/lazyearth
 Download-URL: https://github.com/Tun555/lazyearth/archive/refs/tags/v0.0.15.zip
 Author: Tun Kedsaro
 Author-email: Tun.k@ku.th
 License: MIT
 Keywords: geo,ODC,earth
```

### Comparing `lazyearth-1.0.7/README.rst` & `lazyearth-1.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `lazyearth-1.0.7/lazyearth/mainfile.py` & `lazyearth-1.0.8/lazyearth/mainfile.py`

 * *Files identical despite different names*

### Comparing `lazyearth-1.0.7/lazyearth.egg-info/PKG-INFO` & `lazyearth-1.0.8/lazyearth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazyearth
-Version: 1.0.7
+Version: 1.0.8
 Summary: Library for earth science
 Home-page: https://github.com/Tun555/lazyearth
 Download-URL: https://github.com/Tun555/lazyearth/archive/refs/tags/v0.0.15.zip
 Author: Tun Kedsaro
 Author-email: Tun.k@ku.th
 License: MIT
 Keywords: geo,ODC,earth
```

### Comparing `lazyearth-1.0.7/setup.py` & `lazyearth-1.0.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 DESCRIPTION = '\n\n'.join(LOAD_TEXT(_) for _ in [
     'README.rst'
 ])
 
 setup(
   name = 'lazyearth',                # Name project the same with folder
   packages = ['lazyearth'],          # Name project the same with folder
-  version = '1.0.7',                 # version
+  version = '1.0.8',                 # version
   license='MIT', 
   description = 'Library for earth science',    #Show on PyPi
   long_description=DESCRIPTION,
   author = 'Tun Kedsaro',            #          
   author_email = 'Tun.k@ku.th',      #
   url = 'https://github.com/Tun555/lazyearth',  #
   download_url = 'https://github.com/Tun555/lazyearth/archive/refs/tags/v0.0.15.zip',                                      #
```

