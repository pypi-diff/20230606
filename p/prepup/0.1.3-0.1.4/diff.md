# Comparing `tmp/prepup-0.1.3.tar.gz` & `tmp/prepup-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prepup-0.1.3.tar", last modified: Tue Jun  6 19:05:30 2023, max compression
+gzip compressed data, was "prepup-0.1.4.tar", last modified: Tue Jun  6 19:09:19 2023, max compression
```

## Comparing `prepup-0.1.3.tar` & `prepup-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 19:05:30.329564 prepup-0.1.3/
--rw-rw-rw-   0        0        0      188 2023-04-29 20:41:27.000000 prepup-0.1.3/AUTHORS.rst
--rw-rw-rw-   0        0        0     1100 2023-04-29 20:41:27.000000 prepup-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      129 2023-04-29 20:41:27.000000 prepup-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4255 2023-06-06 19:05:30.329564 prepup-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3719 2023-05-17 04:35:37.000000 prepup-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 19:05:30.321562 prepup-0.1.3/prepup/
--rw-rw-rw-   0        0        0     7949 2023-06-06 19:04:33.000000 prepup-0.1.3/prepup/__init__.py
--rw-rw-rw-   0        0        0    33833 2023-05-17 04:34:27.000000 prepup-0.1.3/prepup/common.py
-drwxrwxrwx   0        0        0        0 2023-06-06 19:05:30.329564 prepup-0.1.3/prepup.egg-info/
--rw-rw-rw-   0        0        0     4255 2023-06-06 19:05:30.000000 prepup-0.1.3/prepup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-06-06 19:05:30.000000 prepup-0.1.3/prepup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 19:05:30.000000 prepup-0.1.3/prepup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-06 19:05:30.000000 prepup-0.1.3/prepup.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      220 2023-06-06 19:05:30.000000 prepup-0.1.3/prepup.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-06 19:05:30.000000 prepup-0.1.3/prepup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      367 2023-05-17 04:35:39.000000 prepup-0.1.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 19:05:30.329564 prepup-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1488 2023-06-06 19:05:05.000000 prepup-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 19:09:19.503523 prepup-0.1.4/
+-rw-rw-rw-   0        0        0      188 2023-04-29 20:41:27.000000 prepup-0.1.4/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1100 2023-04-29 20:41:27.000000 prepup-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-04-29 20:41:27.000000 prepup-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4255 2023-06-06 19:09:19.503523 prepup-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3719 2023-05-17 04:35:37.000000 prepup-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 19:09:19.497331 prepup-0.1.4/prepup/
+-rw-rw-rw-   0        0        0     7949 2023-06-06 19:04:33.000000 prepup-0.1.4/prepup/__init__.py
+-rw-rw-rw-   0        0        0    33833 2023-05-17 04:34:27.000000 prepup-0.1.4/prepup/common.py
+drwxrwxrwx   0        0        0        0 2023-06-06 19:09:19.503523 prepup-0.1.4/prepup.egg-info/
+-rw-rw-rw-   0        0        0     4255 2023-06-06 19:09:19.000000 prepup-0.1.4/prepup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-06-06 19:09:19.000000 prepup-0.1.4/prepup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 19:09:19.000000 prepup-0.1.4/prepup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-06 19:09:19.000000 prepup-0.1.4/prepup.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      220 2023-06-06 19:09:19.000000 prepup-0.1.4/prepup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-06 19:09:19.000000 prepup-0.1.4/prepup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      367 2023-05-17 04:35:39.000000 prepup-0.1.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 19:09:19.503523 prepup-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1488 2023-06-06 19:09:11.000000 prepup-0.1.4/setup.py
```

### Comparing `prepup-0.1.3/LICENSE` & `prepup-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prepup-0.1.3/PKG-INFO` & `prepup-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prepup
-Version: 0.1.3
+Version: 0.1.4
 Summary: Prepup is a free, open-source package that lets you open, explore, visualize, and pre-process datasets in your Computer's Terminal.
 Author: Sudhanshu Mukherjee
 Author-email: sudhanshumukherjeexx@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
```

### Comparing `prepup-0.1.3/README.md` & `prepup-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `prepup-0.1.3/prepup/__init__.py` & `prepup-0.1.4/prepup/__init__.py`

 * *Files identical despite different names*

### Comparing `prepup-0.1.3/prepup/common.py` & `prepup-0.1.4/prepup/common.py`

 * *Files identical despite different names*

### Comparing `prepup-0.1.3/prepup.egg-info/PKG-INFO` & `prepup-0.1.4/prepup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prepup
-Version: 0.1.3
+Version: 0.1.4
 Summary: Prepup is a free, open-source package that lets you open, explore, visualize, and pre-process datasets in your Computer's Terminal.
 Author: Sudhanshu Mukherjee
 Author-email: sudhanshumukherjeexx@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
```

### Comparing `prepup-0.1.3/setup.py` & `prepup-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setuptools.setup(
     name="prepup",
-    version="0.1.3",
+    version="0.1.4",
     author="Sudhanshu Mukherjee",
     author_email="sudhanshumukherjeexx@gmail.com",
     description="Prepup is a free, open-source package that lets you open, explore, visualize, and pre-process datasets in your Computer's Terminal.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     entry_points={
```

