# Comparing `tmp/ssptools-0.3.3.tar.gz` & `tmp/ssptools-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssptools-0.3.3.tar", last modified: Fri Jan 20 15:25:17 2023, max compression
+gzip compressed data, was "ssptools-0.4.0.tar", last modified: Tue Jun  6 14:36:27 2023, max compression
```

## Comparing `ssptools-0.3.3.tar` & `ssptools-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 15:25:17.827983 ssptools-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-20 15:25:06.000000 ssptools-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-01-20 15:25:17.827983 ssptools-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-01-20 15:25:06.000000 ssptools-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-01-20 15:25:06.000000 ssptools-0.3.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 15:25:17.827983 ssptools-0.3.3/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-01-20 15:25:06.000000 ssptools-0.3.3/scripts/2POS.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-01-20 15:25:06.000000 ssptools-0.3.3/scripts/appendKPaths.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-01-20 15:25:06.000000 ssptools-0.3.3/scripts/compareEV.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-01-20 15:25:06.000000 ssptools-0.3.3/scripts/plotBS.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-01-20 15:25:06.000000 ssptools-0.3.3/scripts/sortPOS.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-01-20 15:25:17.827983 ssptools-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-01-20 15:25:06.000000 ssptools-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 15:25:17.827983 ssptools-0.3.3/ssptools/
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-01-20 15:25:06.000000 ssptools-0.3.3/ssptools/BSData.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 15:25:06.000000 ssptools-0.3.3/ssptools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-01-20 15:25:06.000000 ssptools-0.3.3/ssptools/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-01-20 15:25:06.000000 ssptools-0.3.3/ssptools/eigenvalues.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 15:25:17.827983 ssptools-0.3.3/ssptools/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 15:25:06.000000 ssptools-0.3.3/ssptools/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-01-20 15:25:06.000000 ssptools-0.3.3/ssptools/io/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-01-20 15:25:06.000000 ssptools-0.3.3/ssptools/kpaths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 15:25:17.827983 ssptools-0.3.3/ssptools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-01-20 15:25:17.000000 ssptools-0.3.3/ssptools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-01-20 15:25:17.000000 ssptools-0.3.3/ssptools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 15:25:17.000000 ssptools-0.3.3/ssptools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-01-20 15:25:17.000000 ssptools-0.3.3/ssptools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-20 15:25:17.000000 ssptools-0.3.3/ssptools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:36:27.988789 ssptools-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-06 14:36:15.000000 ssptools-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-06 14:36:27.988789 ssptools-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-06-06 14:36:15.000000 ssptools-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-06 14:36:15.000000 ssptools-0.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:36:27.988789 ssptools-0.4.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-06 14:36:15.000000 ssptools-0.4.0/scripts/2POS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-06 14:36:15.000000 ssptools-0.4.0/scripts/appendKPaths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-06 14:36:15.000000 ssptools-0.4.0/scripts/compareEV.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-06 14:36:15.000000 ssptools-0.4.0/scripts/plotBS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-06 14:36:15.000000 ssptools-0.4.0/scripts/sortPOS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-06 14:36:27.992789 ssptools-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-06 14:36:15.000000 ssptools-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:36:27.988789 ssptools-0.4.0/ssptools/
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-06-06 14:36:15.000000 ssptools-0.4.0/ssptools/BSData.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:36:15.000000 ssptools-0.4.0/ssptools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-06 14:36:15.000000 ssptools-0.4.0/ssptools/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-06 14:36:15.000000 ssptools-0.4.0/ssptools/eigenvalues.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:36:27.988789 ssptools-0.4.0/ssptools/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:36:15.000000 ssptools-0.4.0/ssptools/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-06 14:36:15.000000 ssptools-0.4.0/ssptools/io/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-06 14:36:15.000000 ssptools-0.4.0/ssptools/kpaths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:36:27.988789 ssptools-0.4.0/ssptools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-06 14:36:27.000000 ssptools-0.4.0/ssptools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-06 14:36:27.000000 ssptools-0.4.0/ssptools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:36:27.000000 ssptools-0.4.0/ssptools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-06 14:36:27.000000 ssptools-0.4.0/ssptools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-06 14:36:27.000000 ssptools-0.4.0/ssptools.egg-info/top_level.txt
```

### Comparing `ssptools-0.3.3/LICENSE` & `ssptools-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ssptools-0.3.3/PKG-INFO` & `ssptools-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssptools
-Version: 0.3.3
+Version: 0.4.0
 Summary: Various specialized tools for working with the input and output of VASP
 Home-page: https://github.com/martin-eom/ssptools
 Author: Martin Keller
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
```

### Comparing `ssptools-0.3.3/README.md` & `ssptools-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ssptools-0.3.3/scripts/appendKPaths.py` & `ssptools-0.4.0/scripts/appendKPaths.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python
 
 import sys
 from ssptools.kpaths import read, makeCoordList
 
-pointList, numList, nameList = read(sys.argv[1])
-coordList = makeCoordList(pointList, numList, nameList)
+pointList, numList, nameList, rest = read(sys.argv[1])
+coordList = makeCoordList(pointList, numList, nameList, rest)
+
 with open(sys.argv[2], 'a') as file:
     for kpoint in coordList:
         file.write("\t%f\t%f\t%f\t%d\n" % (kpoint[0], kpoint[1], kpoint[2], 0))
 with open(sys.argv[2], 'r') as file:
     lines = file.readlines()
 nk_old = int(lines[1])
 nk_new = nk_old + sum(numList)
```

### Comparing `ssptools-0.3.3/scripts/plotBS.py` & `ssptools-0.4.0/scripts/plotBS.py`

 * *Files identical despite different names*

### Comparing `ssptools-0.3.3/setup.cfg` & `ssptools-0.4.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ssptools
-version = 0.3.3
+version = 0.4.0
 url = https://github.com/martin-eom/ssptools
 author = Martin Keller
 description = Various specialized tools for working with the input and output of VASP
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `ssptools-0.3.3/setup.py` & `ssptools-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 site.ENABLE_USER_SITE = "--user" in sys.argv[1:]
 
 with open("README.md", 'r', encoding="utf-8") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="ssptools",
-	version="0.3.3",
+	version="0.4.0",
 	url="https://github.com/martin-eom/ssptools",
 	author="Martin Keller",
 	description="Various specialized tools for working with the input and output of VASP",
         long_description=long_description,
         classifiers=[
                 "Programming Language :: Python :: 3",
                 "License :: OSI Approved :: MIT License",
```

### Comparing `ssptools-0.3.3/ssptools/BSData.py` & `ssptools-0.4.0/ssptools/BSData.py`

 * *Files identical despite different names*

### Comparing `ssptools-0.3.3/ssptools/compare.py` & `ssptools-0.4.0/ssptools/compare.py`

 * *Files identical despite different names*

### Comparing `ssptools-0.3.3/ssptools/eigenvalues.py` & `ssptools-0.4.0/ssptools/eigenvalues.py`

 * *Files identical despite different names*

### Comparing `ssptools-0.3.3/ssptools/io/main.py` & `ssptools-0.4.0/ssptools/io/main.py`

 * *Files identical despite different names*

### Comparing `ssptools-0.3.3/ssptools.egg-info/PKG-INFO` & `ssptools-0.4.0/ssptools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssptools
-Version: 0.3.3
+Version: 0.4.0
 Summary: Various specialized tools for working with the input and output of VASP
 Home-page: https://github.com/martin-eom/ssptools
 Author: Martin Keller
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
```

