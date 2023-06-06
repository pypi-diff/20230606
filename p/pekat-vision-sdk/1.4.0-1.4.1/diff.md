# Comparing `tmp/pekat_vision_sdk-1.4.0.tar.gz` & `tmp/pekat_vision_sdk-1.4.1.tar.gz`

## Comparing `pekat_vision_sdk-1.4.0.tar` & `pekat_vision_sdk-1.4.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.0/PekatVisionSDK/__about__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.0/PekatVisionSDK/__init__.py
--rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.0/PekatVisionSDK/pekat_vision_instance.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.0/LICENSE
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.0/README.md
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.1/PekatVisionSDK/__about__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.1/PekatVisionSDK/__init__.py
+-rw-r--r--   0        0        0    12186 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.1/PekatVisionSDK/pekat_vision_instance.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.1/LICENSE
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.1/README.md
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.1/PKG-INFO
```

### Comparing `pekat_vision_sdk-1.4.0/PekatVisionSDK/pekat_vision_instance.py` & `pekat_vision_sdk-1.4.1/PekatVisionSDK/pekat_vision_instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,15 @@
             response = requests.post(
                 url='{}/analyze_image?{}'.format(url, query),
                 data=image_data,
                 timeout=timeout,
                 headers={'Content-Type': 'application/octet-stream'}
             )
         elif numpy_image is not None:
-            height, width, _ = numpy_image.shape
+            height, width = numpy_image.shape[:2]
             response = requests.post(
                 url='{}/analyze_raw_image?width={}&height={}&{}'.format(url, width, height, query),
                 data=numpy_image.tobytes(),
                 headers={'Content-Type': 'application/octet-stream'},
                 timeout=timeout
             )
         else:
```

### Comparing `pekat_vision_sdk-1.4.0/LICENSE` & `pekat_vision_sdk-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pekat_vision_sdk-1.4.0/README.md` & `pekat_vision_sdk-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pekat_vision_sdk-1.4.0/pyproject.toml` & `pekat_vision_sdk-1.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pekat_vision_sdk-1.4.0/PKG-INFO` & `pekat_vision_sdk-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pekat-vision-sdk
-Version: 1.4.0
+Version: 1.4.1
 Summary: A Python module for communication with PEKAT VISION
 Project-URL: Homepage, https://github.com/pekat-vision/pekat-vision-sdk-python
 Project-URL: repository, https://github.com/pekat-vision/pekat-vision-sdk-python.git
 Author-email: developers@pekatvision.com
 Maintainer-email: developers@pekatvision.com
 License-Expression: MIT
 License-File: LICENSE
```

