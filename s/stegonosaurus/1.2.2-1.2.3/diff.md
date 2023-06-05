# Comparing `tmp/stegonosaurus-1.2.2.tar.gz` & `tmp/stegonosaurus-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stegonosaurus-1.2.2.tar", last modified: Sun Jun  4 18:59:07 2023, max compression
+gzip compressed data, was "stegonosaurus-1.2.3.tar", last modified: Mon Jun  5 23:25:27 2023, max compression
```

## Comparing `stegonosaurus-1.2.2.tar` & `stegonosaurus-1.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:59:07.454248 stegonosaurus-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-04 18:59:07.454248 stegonosaurus-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-04 18:58:56.000000 stegonosaurus-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 18:59:07.454248 stegonosaurus-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-04 18:58:56.000000 stegonosaurus-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:59:07.454248 stegonosaurus-1.2.2/stegonosaurus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 18:58:56.000000 stegonosaurus-1.2.2/stegonosaurus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-04 18:58:56.000000 stegonosaurus-1.2.2/stegonosaurus/stegoexceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-06-04 18:58:56.000000 stegonosaurus-1.2.2/stegonosaurus/stegofunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-04 18:58:56.000000 stegonosaurus-1.2.2/stegonosaurus/stegoutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:59:07.454248 stegonosaurus-1.2.2/stegonosaurus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-04 18:59:07.000000 stegonosaurus-1.2.2/stegonosaurus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-04 18:59:07.000000 stegonosaurus-1.2.2/stegonosaurus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 18:59:07.000000 stegonosaurus-1.2.2/stegonosaurus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-04 18:59:07.000000 stegonosaurus-1.2.2/stegonosaurus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:59:07.454248 stegonosaurus-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    23550 2023-06-04 18:58:56.000000 stegonosaurus-1.2.2/tests/test_stegofunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9142 2023-06-04 18:58:56.000000 stegonosaurus-1.2.2/tests/test_stegoutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:25:27.989738 stegonosaurus-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-05 23:25:27.989738 stegonosaurus-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-05 23:25:15.000000 stegonosaurus-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 23:25:27.989738 stegonosaurus-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-05 23:25:15.000000 stegonosaurus-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:25:27.985738 stegonosaurus-1.2.3/stegonosaurus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:25:15.000000 stegonosaurus-1.2.3/stegonosaurus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-05 23:25:15.000000 stegonosaurus-1.2.3/stegonosaurus/stegoexceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-06-05 23:25:15.000000 stegonosaurus-1.2.3/stegonosaurus/stegofunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-05 23:25:15.000000 stegonosaurus-1.2.3/stegonosaurus/stegoutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:25:27.989738 stegonosaurus-1.2.3/stegonosaurus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-05 23:25:27.000000 stegonosaurus-1.2.3/stegonosaurus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-05 23:25:27.000000 stegonosaurus-1.2.3/stegonosaurus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 23:25:27.000000 stegonosaurus-1.2.3/stegonosaurus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 23:25:27.000000 stegonosaurus-1.2.3/stegonosaurus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:25:27.989738 stegonosaurus-1.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    23550 2023-06-05 23:25:15.000000 stegonosaurus-1.2.3/tests/test_stegofunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9142 2023-06-05 23:25:15.000000 stegonosaurus-1.2.3/tests/test_stegoutils.py
```

### Comparing `stegonosaurus-1.2.2/PKG-INFO` & `stegonosaurus-1.2.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 Metadata-Version: 2.1
 Name: stegonosaurus
-Version: 1.2.2
+Version: 1.2.3
 Summary: Stegonography utilities
 Home-page: https://github.com/Geada734/stegonosaurus
 Author: Geada734
 License: MIT
 Keywords: steganography
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
 # stegonosaurus
 
-*Ver 1.2.2*
+*Ver 1.2.3*
 
 Steganography functions packed in a convenient wheel. This library helps encode and decode messages into and out of multi-band .png images. Works with the [Image](https://pillow.readthedocs.io/en/stable/reference/Image.html) module of the Pillow library.
 
 ## Requirements
 - Python3
 
 ## Installing
 
 A simple pip install will do:
 
 `pip install stegonosaurus`
 
 ## Functions
 
-### inspect:
+**inspect** *(img: PIL.Image) -> str:*
 
 Returns a string that contains the values of each pixel in the image along with other relevant info such as image size, format, file name, mode, and whether it can be used with the other functions in the library or not.
 
-### black:
+**black** *(img: PIL.Image) -> PIL.Image:*
 
 Return an all black copy of a provided image. This helps create a template for images with coded messages used for encoding.
 
-### encode:
-
-Takes two images, a black image with a message in contrasting colors, and the image where the message will be encoded. The image where the message is going to be hidden in is first "flattened" (all pixels with an odd value on their blue component are changed so their blue component's value is even). Afterwards, the image that contains the message is processed, so the same pixels that contain the bright red letters are changed in the other image to pixels where the blue value is odd (harder to express in theory than practice). The image with the bright message has to be smaller or equal in size to the image where the message is going to be hidden in on either axis.
-
-### decode:
+**decode** *(img: PIL.Image, mode: str) -> PIL.Image:*
 
 Decodes an image with a hidden message. This functions looks for pixels where the blue value is odd, and paints those pixels bright red. This function operates on two modes:
 
 -B,b (for "black"): pixels with an even blue value are colored black, displaying the message in red letters on a black background.
 -T,t (for "transparent"): pixels with an odd blue value are colored red, the other pixels remain the same so the message can be displayed on top of the original image.
 
-### Exceptions:
+**encode** *(coded: PIL.Image, img: PIL.Image) -> PIL.Image:*
+
+Takes two images, a black image with a message in contrasting colors, and the image where the message will be encoded. The image where the message is going to be hidden in is first "flattened" (all pixels with an odd value on their blue component are changed so their blue component's value is even). Afterwards, the image that contains the message is processed, so the same pixels that contain the bright red letters are changed in the other image to pixels where the blue value is odd (harder to express in theory than practice). The image with the bright message has to be smaller or equal in size to the image where the message is going to be hidden in on either axis.
+
+## Exceptions:
 
 - StegonosaurusIncorrectFormatError: 
 
   Raised when a function receives a file that isn't a .PNG multiband image.
 - StegonosaurusIncorrectSizeError: 
 
   Raised when the image with the coded message is larger than the image where the message will be hidden.
```

### Comparing `stegonosaurus-1.2.2/README.md` & `stegonosaurus-1.2.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 # stegonosaurus
 
-*Ver 1.2.2*
+*Ver 1.2.3*
 
 Steganography functions packed in a convenient wheel. This library helps encode and decode messages into and out of multi-band .png images. Works with the [Image](https://pillow.readthedocs.io/en/stable/reference/Image.html) module of the Pillow library.
 
 ## Requirements
 - Python3
 
 ## Installing
 
 A simple pip install will do:
 
 `pip install stegonosaurus`
 
 ## Functions
 
-### inspect:
+**inspect** *(img: PIL.Image) -> str:*
 
 Returns a string that contains the values of each pixel in the image along with other relevant info such as image size, format, file name, mode, and whether it can be used with the other functions in the library or not.
 
-### black:
+**black** *(img: PIL.Image) -> PIL.Image:*
 
 Return an all black copy of a provided image. This helps create a template for images with coded messages used for encoding.
 
-### encode:
-
-Takes two images, a black image with a message in contrasting colors, and the image where the message will be encoded. The image where the message is going to be hidden in is first "flattened" (all pixels with an odd value on their blue component are changed so their blue component's value is even). Afterwards, the image that contains the message is processed, so the same pixels that contain the bright red letters are changed in the other image to pixels where the blue value is odd (harder to express in theory than practice). The image with the bright message has to be smaller or equal in size to the image where the message is going to be hidden in on either axis.
-
-### decode:
+**decode** *(img: PIL.Image, mode: str) -> PIL.Image:*
 
 Decodes an image with a hidden message. This functions looks for pixels where the blue value is odd, and paints those pixels bright red. This function operates on two modes:
 
 -B,b (for "black"): pixels with an even blue value are colored black, displaying the message in red letters on a black background.
 -T,t (for "transparent"): pixels with an odd blue value are colored red, the other pixels remain the same so the message can be displayed on top of the original image.
 
-### Exceptions:
+**encode** *(coded: PIL.Image, img: PIL.Image) -> PIL.Image:*
+
+Takes two images, a black image with a message in contrasting colors, and the image where the message will be encoded. The image where the message is going to be hidden in is first "flattened" (all pixels with an odd value on their blue component are changed so their blue component's value is even). Afterwards, the image that contains the message is processed, so the same pixels that contain the bright red letters are changed in the other image to pixels where the blue value is odd (harder to express in theory than practice). The image with the bright message has to be smaller or equal in size to the image where the message is going to be hidden in on either axis.
+
+## Exceptions:
 
 - StegonosaurusIncorrectFormatError: 
 
   Raised when a function receives a file that isn't a .PNG multiband image.
 - StegonosaurusIncorrectSizeError: 
 
   Raised when the image with the coded message is larger than the image where the message will be hidden.
```

### Comparing `stegonosaurus-1.2.2/setup.py` & `stegonosaurus-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='stegonosaurus',
     packages=find_packages(include=["stegonosaurus"]),
-    version='1.2.2',
+    version='1.2.3',
     description='Stegonography utilities',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Geada734',
     license='MIT',
     classifiers=classifiers,
     keywords='steganography',
```

### Comparing `stegonosaurus-1.2.2/stegonosaurus/stegoexceptions.py` & `stegonosaurus-1.2.3/stegonosaurus/stegoexceptions.py`

 * *Files identical despite different names*

### Comparing `stegonosaurus-1.2.2/stegonosaurus/stegofunctions.py` & `stegonosaurus-1.2.3/stegonosaurus/stegofunctions.py`

 * *Files identical despite different names*

### Comparing `stegonosaurus-1.2.2/stegonosaurus/stegoutils.py` & `stegonosaurus-1.2.3/stegonosaurus/stegoutils.py`

 * *Files identical despite different names*

### Comparing `stegonosaurus-1.2.2/stegonosaurus.egg-info/PKG-INFO` & `stegonosaurus-1.2.3/stegonosaurus.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 Metadata-Version: 2.1
 Name: stegonosaurus
-Version: 1.2.2
+Version: 1.2.3
 Summary: Stegonography utilities
 Home-page: https://github.com/Geada734/stegonosaurus
 Author: Geada734
 License: MIT
 Keywords: steganography
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
 # stegonosaurus
 
-*Ver 1.2.2*
+*Ver 1.2.3*
 
 Steganography functions packed in a convenient wheel. This library helps encode and decode messages into and out of multi-band .png images. Works with the [Image](https://pillow.readthedocs.io/en/stable/reference/Image.html) module of the Pillow library.
 
 ## Requirements
 - Python3
 
 ## Installing
 
 A simple pip install will do:
 
 `pip install stegonosaurus`
 
 ## Functions
 
-### inspect:
+**inspect** *(img: PIL.Image) -> str:*
 
 Returns a string that contains the values of each pixel in the image along with other relevant info such as image size, format, file name, mode, and whether it can be used with the other functions in the library or not.
 
-### black:
+**black** *(img: PIL.Image) -> PIL.Image:*
 
 Return an all black copy of a provided image. This helps create a template for images with coded messages used for encoding.
 
-### encode:
-
-Takes two images, a black image with a message in contrasting colors, and the image where the message will be encoded. The image where the message is going to be hidden in is first "flattened" (all pixels with an odd value on their blue component are changed so their blue component's value is even). Afterwards, the image that contains the message is processed, so the same pixels that contain the bright red letters are changed in the other image to pixels where the blue value is odd (harder to express in theory than practice). The image with the bright message has to be smaller or equal in size to the image where the message is going to be hidden in on either axis.
-
-### decode:
+**decode** *(img: PIL.Image, mode: str) -> PIL.Image:*
 
 Decodes an image with a hidden message. This functions looks for pixels where the blue value is odd, and paints those pixels bright red. This function operates on two modes:
 
 -B,b (for "black"): pixels with an even blue value are colored black, displaying the message in red letters on a black background.
 -T,t (for "transparent"): pixels with an odd blue value are colored red, the other pixels remain the same so the message can be displayed on top of the original image.
 
-### Exceptions:
+**encode** *(coded: PIL.Image, img: PIL.Image) -> PIL.Image:*
+
+Takes two images, a black image with a message in contrasting colors, and the image where the message will be encoded. The image where the message is going to be hidden in is first "flattened" (all pixels with an odd value on their blue component are changed so their blue component's value is even). Afterwards, the image that contains the message is processed, so the same pixels that contain the bright red letters are changed in the other image to pixels where the blue value is odd (harder to express in theory than practice). The image with the bright message has to be smaller or equal in size to the image where the message is going to be hidden in on either axis.
+
+## Exceptions:
 
 - StegonosaurusIncorrectFormatError: 
 
   Raised when a function receives a file that isn't a .PNG multiband image.
 - StegonosaurusIncorrectSizeError: 
 
   Raised when the image with the coded message is larger than the image where the message will be hidden.
```

### Comparing `stegonosaurus-1.2.2/tests/test_stegofunctions.py` & `stegonosaurus-1.2.3/tests/test_stegofunctions.py`

 * *Files identical despite different names*

### Comparing `stegonosaurus-1.2.2/tests/test_stegoutils.py` & `stegonosaurus-1.2.3/tests/test_stegoutils.py`

 * *Files identical despite different names*

