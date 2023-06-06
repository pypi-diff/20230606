# Comparing `tmp/easylsb-1.0.5.tar.gz` & `tmp/easylsb-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\easylsb-1.0.5.tar", last modified: Tue Jun  6 06:26:27 2023, max compression
+gzip compressed data, was "dist\easylsb-1.0.6.tar", last modified: Tue Jun  6 06:28:45 2023, max compression
```

## Comparing `easylsb-1.0.5.tar` & `easylsb-1.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 06:26:27.000000 easylsb-1.0.5/
--rw-rw-rw-   0        0        0     1255 2023-06-06 06:26:27.000000 easylsb-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1108 2023-06-06 06:23:38.000000 easylsb-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 06:26:27.000000 easylsb-1.0.5/easylsb.egg-info/
--rw-rw-rw-   0        0        0     1255 2023-06-06 06:26:27.000000 easylsb-1.0.5/easylsb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-06-06 06:26:27.000000 easylsb-1.0.5/easylsb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 06:26:27.000000 easylsb-1.0.5/easylsb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-06-06 06:26:27.000000 easylsb-1.0.5/easylsb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2023-06-06 06:26:27.000000 easylsb-1.0.5/easylsb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-06 06:26:27.000000 easylsb-1.0.5/easylsb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13569 2023-06-06 06:21:21.000000 easylsb-1.0.5/lsb.py
--rw-rw-rw-   0        0        0       42 2023-06-06 06:26:27.000000 easylsb-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      721 2023-06-06 06:26:19.000000 easylsb-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:28:45.000000 easylsb-1.0.6/
+-rw-rw-rw-   0        0        0     1259 2023-06-06 06:28:45.000000 easylsb-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1112 2023-06-06 06:28:23.000000 easylsb-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 06:28:45.000000 easylsb-1.0.6/easylsb.egg-info/
+-rw-rw-rw-   0        0        0     1259 2023-06-06 06:28:44.000000 easylsb-1.0.6/easylsb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2023-06-06 06:28:45.000000 easylsb-1.0.6/easylsb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 06:28:44.000000 easylsb-1.0.6/easylsb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-06-06 06:28:44.000000 easylsb-1.0.6/easylsb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2023-06-06 06:28:44.000000 easylsb-1.0.6/easylsb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-06 06:28:44.000000 easylsb-1.0.6/easylsb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13569 2023-06-06 06:21:21.000000 easylsb-1.0.6/lsb.py
+-rw-rw-rw-   0        0        0       42 2023-06-06 06:28:45.000000 easylsb-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      721 2023-06-06 06:28:41.000000 easylsb-1.0.6/setup.py
```

### Comparing `easylsb-1.0.5/PKG-INFO` & `easylsb-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: easylsb
-Version: 1.0.5
+Version: 1.0.6
 Summary: Simple Python package for steganography
 Description-Content-Type: text/markdown
 
 <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
 
 ### This is a simple Python package for steganography
+
 Now this package can automatically detect the encoding of the hidden text using the '-a' argument.
+
 Code to hide information in the given image:
 ```python
 import lsb
 from PIL import Image
 import numpy as np
 img=Image.open('test.png')
 img=np.array(img)
```

### Comparing `easylsb-1.0.5/README.md` & `easylsb-1.0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
 
 ### This is a simple Python package for steganography
+
 Now this package can automatically detect the encoding of the hidden text using the '-a' argument.
+
 Code to hide information in the given image:
 ```python
 import lsb
 from PIL import Image
 import numpy as np
 img=Image.open('test.png')
 img=np.array(img)
```

### Comparing `easylsb-1.0.5/easylsb.egg-info/PKG-INFO` & `easylsb-1.0.6/easylsb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: easylsb
-Version: 1.0.5
+Version: 1.0.6
 Summary: Simple Python package for steganography
 Description-Content-Type: text/markdown
 
 <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
 
 ### This is a simple Python package for steganography
+
 Now this package can automatically detect the encoding of the hidden text using the '-a' argument.
+
 Code to hide information in the given image:
 ```python
 import lsb
 from PIL import Image
 import numpy as np
 img=Image.open('test.png')
 img=np.array(img)
```

### Comparing `easylsb-1.0.5/lsb.py` & `easylsb-1.0.6/lsb.py`

 * *Files identical despite different names*

