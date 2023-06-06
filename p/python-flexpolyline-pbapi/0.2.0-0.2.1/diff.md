# Comparing `tmp/python-flexpolyline-pbapi-0.2.0.tar.gz` & `tmp/python-flexpolyline-pbapi-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-flexpolyline-pbapi-0.2.0.tar", last modified: Tue Apr  5 09:50:31 2022, max compression
+gzip compressed data, was "python-flexpolyline-pbapi-0.2.1.tar", last modified: Tue Jun  6 15:53:32 2023, max compression
```

## Comparing `python-flexpolyline-pbapi-0.2.0.tar` & `python-flexpolyline-pbapi-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 decitre    (501) staff       (20)        0 2022-04-05 09:50:31.243936 python-flexpolyline-pbapi-0.2.0/
--rw-r--r--   0 decitre    (501) staff       (20)     1055 2022-04-01 15:46:35.000000 python-flexpolyline-pbapi-0.2.0/LICENSE
--rw-r--r--   0 decitre    (501) staff       (20)       33 2022-04-01 15:46:35.000000 python-flexpolyline-pbapi-0.2.0/MANIFEST.in
--rw-r--r--   0 decitre    (501) staff       (20)     3540 2022-04-05 09:50:31.243691 python-flexpolyline-pbapi-0.2.0/PKG-INFO
--rw-r--r--   0 decitre    (501) staff       (20)     2759 2022-04-05 09:50:27.000000 python-flexpolyline-pbapi-0.2.0/README.md
-drwxr-xr-x   0 decitre    (501) staff       (20)        0 2022-04-05 09:50:31.242122 python-flexpolyline-pbapi-0.2.0/flexpolyline_pbapi/
--rw-r--r--   0 decitre    (501) staff       (20)     3097 2022-04-05 09:44:12.000000 python-flexpolyline-pbapi-0.2.0/flexpolyline_pbapi/__init__.py
--rw-r--r--   0 decitre    (501) staff       (20)     4659 2022-04-05 09:27:24.000000 python-flexpolyline-pbapi-0.2.0/flexpolyline_pbapi/decoding.py
--rw-r--r--   0 decitre    (501) staff       (20)     4356 2022-04-05 09:44:12.000000 python-flexpolyline-pbapi-0.2.0/flexpolyline_pbapi/encoding.py
-drwxr-xr-x   0 decitre    (501) staff       (20)        0 2022-04-05 09:50:31.243341 python-flexpolyline-pbapi-0.2.0/python_flexpolyline_pbapi.egg-info/
--rw-r--r--   0 decitre    (501) staff       (20)     3540 2022-04-05 09:50:31.000000 python-flexpolyline-pbapi-0.2.0/python_flexpolyline_pbapi.egg-info/PKG-INFO
--rw-r--r--   0 decitre    (501) staff       (20)      327 2022-04-05 09:50:31.000000 python-flexpolyline-pbapi-0.2.0/python_flexpolyline_pbapi.egg-info/SOURCES.txt
--rw-r--r--   0 decitre    (501) staff       (20)        1 2022-04-05 09:50:31.000000 python-flexpolyline-pbapi-0.2.0/python_flexpolyline_pbapi.egg-info/dependency_links.txt
--rw-r--r--   0 decitre    (501) staff       (20)       19 2022-04-05 09:50:31.000000 python-flexpolyline-pbapi-0.2.0/python_flexpolyline_pbapi.egg-info/top_level.txt
--rw-r--r--   0 decitre    (501) staff       (20)       38 2022-04-05 09:50:31.244034 python-flexpolyline-pbapi-0.2.0/setup.cfg
--rw-r--r--   0 decitre    (501) staff       (20)     1163 2022-04-05 09:23:00.000000 python-flexpolyline-pbapi-0.2.0/setup.py
+drwxr-xr-x   0 decitre    (501) staff       (20)        0 2023-06-06 15:53:32.046284 python-flexpolyline-pbapi-0.2.1/
+-rw-r--r--   0 decitre    (501) staff       (20)     1055 2023-06-06 15:41:42.000000 python-flexpolyline-pbapi-0.2.1/LICENSE
+-rw-r--r--   0 decitre    (501) staff       (20)       33 2023-06-06 15:41:42.000000 python-flexpolyline-pbapi-0.2.1/MANIFEST.in
+-rw-r--r--   0 decitre    (501) staff       (20)     3628 2023-06-06 15:53:32.045823 python-flexpolyline-pbapi-0.2.1/PKG-INFO
+-rw-r--r--   0 decitre    (501) staff       (20)     2886 2023-06-06 15:49:35.000000 python-flexpolyline-pbapi-0.2.1/README.md
+drwxr-xr-x   0 decitre    (501) staff       (20)        0 2023-06-06 15:53:32.042089 python-flexpolyline-pbapi-0.2.1/flexpolyline_pbapi/
+-rw-r--r--   0 decitre    (501) staff       (20)     3097 2023-06-06 15:41:42.000000 python-flexpolyline-pbapi-0.2.1/flexpolyline_pbapi/__init__.py
+-rw-r--r--   0 decitre    (501) staff       (20)     4659 2023-06-06 15:41:42.000000 python-flexpolyline-pbapi-0.2.1/flexpolyline_pbapi/decoding.py
+-rw-r--r--   0 decitre    (501) staff       (20)     4356 2023-06-06 15:41:42.000000 python-flexpolyline-pbapi-0.2.1/flexpolyline_pbapi/encoding.py
+drwxr-xr-x   0 decitre    (501) staff       (20)        0 2023-06-06 15:53:32.044200 python-flexpolyline-pbapi-0.2.1/python_flexpolyline_pbapi.egg-info/
+-rw-r--r--   0 decitre    (501) staff       (20)     3628 2023-06-06 15:53:32.000000 python-flexpolyline-pbapi-0.2.1/python_flexpolyline_pbapi.egg-info/PKG-INFO
+-rw-r--r--   0 decitre    (501) staff       (20)      354 2023-06-06 15:53:32.000000 python-flexpolyline-pbapi-0.2.1/python_flexpolyline_pbapi.egg-info/SOURCES.txt
+-rw-r--r--   0 decitre    (501) staff       (20)        1 2023-06-06 15:53:32.000000 python-flexpolyline-pbapi-0.2.1/python_flexpolyline_pbapi.egg-info/dependency_links.txt
+-rw-r--r--   0 decitre    (501) staff       (20)       19 2023-06-06 15:53:32.000000 python-flexpolyline-pbapi-0.2.1/python_flexpolyline_pbapi.egg-info/top_level.txt
+-rw-r--r--   0 decitre    (501) staff       (20)       38 2023-06-06 15:53:32.046385 python-flexpolyline-pbapi-0.2.1/setup.cfg
+-rw-r--r--   0 decitre    (501) staff       (20)     1163 2023-06-06 15:51:09.000000 python-flexpolyline-pbapi-0.2.1/setup.py
+drwxr-xr-x   0 decitre    (501) staff       (20)        0 2023-06-06 15:53:32.044901 python-flexpolyline-pbapi-0.2.1/tests/
+-rw-r--r--   0 decitre    (501) staff       (20)    11162 2023-06-06 15:41:42.000000 python-flexpolyline-pbapi-0.2.1/tests/test_flexpolyline.py
```

### Comparing `python-flexpolyline-pbapi-0.2.0/LICENSE` & `python-flexpolyline-pbapi-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-flexpolyline-pbapi-0.2.0/PKG-INFO` & `python-flexpolyline-pbapi-0.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: python-flexpolyline-pbapi
-Version: 0.2.0
+Version: 0.2.1
 Summary: Flexible Polyline encoding (PBAPI extension)
-Home-page: UNKNOWN
 Author: decitre
 License: MIT
 Project-URL: Source, https://github.com/decitre/python-flexpolyline-pbapi.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![workflow](https://github.com/decitre/python-flexpolyline-pbapi/actions/workflows/test.yml/badge.svg)
 
-# FlexPolyline and HERE Polyline
+# This project is deprecated. Please check [here-polyline-converter](https://github.com/heremaps/here-polyline-converter)
+
+## FlexPolyline and HERE Polyline
 
 This is Python extension of the [Flexible Polyline](https://github.com/heremaps/flexible-polyline) 
 codec library to support the HERE polyline format used by 
 [HERE Places (Search) API](https://developer.here.com/documentation/places/dev_guide/topics/guide.html)
 for the [`compressedRoute`](https://developer.here.com/documentation/places/dev_guide/topics/location-contexts.html#location-contexts__here-polyline-encoding) requests parameter.
 
 Note that the HERE Places (Search) API is in maintenance. This Python package can be used to test applications being migrated to 
 the newer [HERE Geocoding & Search API](https://developer.here.com/documentation/geocoding-search-api/dev_guide/index.html).
 
 
-## Install
+### Install
 
 ```shell
 $ pip install python-flexpolyline-pbapi
 ```
 
 ## Usage
 
@@ -65,15 +65,15 @@
 
 ```
 >>> encode_pbapi(iterable)
 ```
 
 Note that `width` is expected to be one of `DW`, `HW`, `CW`.
 
-#### Examples
+##### Examples
 
 ```python
 >>> import flexpolyline_pbapi as fp
 >>> here_polyline = "oz5xJ67i1B1B7PzIhaxL7Y"
 >>> flexible_polyline = fp.reencode_pbapi_to_flex(here_polyline)
 >>> flexible_polyline
 'BFoz5xJ67i1B1B7PzIhaxL7Y'
@@ -93,14 +93,12 @@
 git tag v0.2.0
 git remote add origin git@github.com:decitre/python-flexpolyline-pbapi.git`
 git push -u origin master v0.2.0
 python sdist bdist_wheel
 twine upload --skip-existing dist/*
 -->
 
-## License
+### License
 
 Copyright (C) 2019 HERE Europe B.V.
 
 See the [LICENSE](./LICENSE) file in the root of this project for license details.
-
-
```

### Comparing `python-flexpolyline-pbapi-0.2.0/README.md` & `python-flexpolyline-pbapi-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 ![workflow](https://github.com/decitre/python-flexpolyline-pbapi/actions/workflows/test.yml/badge.svg)
 
-# FlexPolyline and HERE Polyline
+# This project is deprecated. Please check [here-polyline-converter](https://github.com/heremaps/here-polyline-converter)
+
+## FlexPolyline and HERE Polyline
 
 This is Python extension of the [Flexible Polyline](https://github.com/heremaps/flexible-polyline) 
 codec library to support the HERE polyline format used by 
 [HERE Places (Search) API](https://developer.here.com/documentation/places/dev_guide/topics/guide.html)
 for the [`compressedRoute`](https://developer.here.com/documentation/places/dev_guide/topics/location-contexts.html#location-contexts__here-polyline-encoding) requests parameter.
 
 Note that the HERE Places (Search) API is in maintenance. This Python package can be used to test applications being migrated to 
 the newer [HERE Geocoding & Search API](https://developer.here.com/documentation/geocoding-search-api/dev_guide/index.html).
 
 
-## Install
+### Install
 
 ```shell
 $ pip install python-flexpolyline-pbapi
 ```
 
 ## Usage
 
@@ -44,15 +46,15 @@
 
 ```
 >>> encode_pbapi(iterable)
 ```
 
 Note that `width` is expected to be one of `DW`, `HW`, `CW`.
 
-#### Examples
+##### Examples
 
 ```python
 >>> import flexpolyline_pbapi as fp
 >>> here_polyline = "oz5xJ67i1B1B7PzIhaxL7Y"
 >>> flexible_polyline = fp.reencode_pbapi_to_flex(here_polyline)
 >>> flexible_polyline
 'BFoz5xJ67i1B1B7PzIhaxL7Y'
@@ -72,12 +74,12 @@
 git tag v0.2.0
 git remote add origin git@github.com:decitre/python-flexpolyline-pbapi.git`
 git push -u origin master v0.2.0
 python sdist bdist_wheel
 twine upload --skip-existing dist/*
 -->
 
-## License
+### License
 
 Copyright (C) 2019 HERE Europe B.V.
 
 See the [LICENSE](./LICENSE) file in the root of this project for license details.
```

### Comparing `python-flexpolyline-pbapi-0.2.0/flexpolyline_pbapi/__init__.py` & `python-flexpolyline-pbapi-0.2.1/flexpolyline_pbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `python-flexpolyline-pbapi-0.2.0/flexpolyline_pbapi/decoding.py` & `python-flexpolyline-pbapi-0.2.1/flexpolyline_pbapi/decoding.py`

 * *Files identical despite different names*

### Comparing `python-flexpolyline-pbapi-0.2.0/flexpolyline_pbapi/encoding.py` & `python-flexpolyline-pbapi-0.2.1/flexpolyline_pbapi/encoding.py`

 * *Files identical despite different names*

### Comparing `python-flexpolyline-pbapi-0.2.0/python_flexpolyline_pbapi.egg-info/PKG-INFO` & `python-flexpolyline-pbapi-0.2.1/python_flexpolyline_pbapi.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: python-flexpolyline-pbapi
-Version: 0.2.0
+Version: 0.2.1
 Summary: Flexible Polyline encoding (PBAPI extension)
-Home-page: UNKNOWN
 Author: decitre
 License: MIT
 Project-URL: Source, https://github.com/decitre/python-flexpolyline-pbapi.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![workflow](https://github.com/decitre/python-flexpolyline-pbapi/actions/workflows/test.yml/badge.svg)
 
-# FlexPolyline and HERE Polyline
+# This project is deprecated. Please check [here-polyline-converter](https://github.com/heremaps/here-polyline-converter)
+
+## FlexPolyline and HERE Polyline
 
 This is Python extension of the [Flexible Polyline](https://github.com/heremaps/flexible-polyline) 
 codec library to support the HERE polyline format used by 
 [HERE Places (Search) API](https://developer.here.com/documentation/places/dev_guide/topics/guide.html)
 for the [`compressedRoute`](https://developer.here.com/documentation/places/dev_guide/topics/location-contexts.html#location-contexts__here-polyline-encoding) requests parameter.
 
 Note that the HERE Places (Search) API is in maintenance. This Python package can be used to test applications being migrated to 
 the newer [HERE Geocoding & Search API](https://developer.here.com/documentation/geocoding-search-api/dev_guide/index.html).
 
 
-## Install
+### Install
 
 ```shell
 $ pip install python-flexpolyline-pbapi
 ```
 
 ## Usage
 
@@ -65,15 +65,15 @@
 
 ```
 >>> encode_pbapi(iterable)
 ```
 
 Note that `width` is expected to be one of `DW`, `HW`, `CW`.
 
-#### Examples
+##### Examples
 
 ```python
 >>> import flexpolyline_pbapi as fp
 >>> here_polyline = "oz5xJ67i1B1B7PzIhaxL7Y"
 >>> flexible_polyline = fp.reencode_pbapi_to_flex(here_polyline)
 >>> flexible_polyline
 'BFoz5xJ67i1B1B7PzIhaxL7Y'
@@ -93,14 +93,12 @@
 git tag v0.2.0
 git remote add origin git@github.com:decitre/python-flexpolyline-pbapi.git`
 git push -u origin master v0.2.0
 python sdist bdist_wheel
 twine upload --skip-existing dist/*
 -->
 
-## License
+### License
 
 Copyright (C) 2019 HERE Europe B.V.
 
 See the [LICENSE](./LICENSE) file in the root of this project for license details.
-
-
```

### Comparing `python-flexpolyline-pbapi-0.2.0/setup.py` & `python-flexpolyline-pbapi-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 setup(
     name="python-flexpolyline-pbapi",
     description="Flexible Polyline encoding (PBAPI extension)",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.2.0",
+    version="0.2.1",
     author="decitre",
     packages=["flexpolyline_pbapi"],
     # SPDX-License-Identifier: MIT
     license="MIT",
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3 :: Only",
```

