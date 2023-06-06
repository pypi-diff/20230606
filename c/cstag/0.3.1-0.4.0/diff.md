# Comparing `tmp/cstag-0.3.1.zip` & `tmp/cstag-0.4.0.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 12063 bytes, number of entries: 19
-drwxr-xr-x  2.0 unx        0 b- stor 22-Sep-16 20:24 cstag-0.3.1/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Sep-16 20:24 cstag-0.3.1/src/
--rw-r--r--  2.0 unx      847 b- defN 22-Sep-16 20:24 cstag-0.3.1/setup.py
--rw-r--r--  2.0 unx       38 b- defN 22-Sep-16 20:24 cstag-0.3.1/setup.cfg
--rw-r--r--  2.0 unx     1069 b- defN 22-Sep-16 20:24 cstag-0.3.1/LICENSE
--rw-r--r--  2.0 unx     2912 b- defN 22-Sep-16 20:24 cstag-0.3.1/README.md
--rw-r--r--  2.0 unx     3507 b- defN 22-Sep-16 20:24 cstag-0.3.1/PKG-INFO
-drwxr-xr-x  2.0 unx        0 b- stor 22-Sep-16 20:24 cstag-0.3.1/src/cstag.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Sep-16 20:24 cstag-0.3.1/src/cstag/
--rw-r--r--  2.0 unx      285 b- defN 22-Sep-16 20:24 cstag-0.3.1/src/cstag.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        6 b- defN 22-Sep-16 20:24 cstag-0.3.1/src/cstag.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 22-Sep-16 20:24 cstag-0.3.1/src/cstag.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     3507 b- defN 22-Sep-16 20:24 cstag-0.3.1/src/cstag.egg-info/PKG-INFO
--rw-r--r--  2.0 unx      687 b- defN 22-Sep-16 20:24 cstag-0.3.1/src/cstag/shorten.py
--rw-r--r--  2.0 unx     1306 b- defN 22-Sep-16 20:24 cstag-0.3.1/src/cstag/lengthen.py
--rw-r--r--  2.0 unx     1902 b- defN 22-Sep-16 20:24 cstag-0.3.1/src/cstag/mask.py
--rw-r--r--  2.0 unx     2547 b- defN 22-Sep-16 20:24 cstag-0.3.1/src/cstag/consensus.py
--rw-r--r--  2.0 unx     3791 b- defN 22-Sep-16 20:24 cstag-0.3.1/src/cstag/to_html.py
--rw-r--r--  2.0 unx      185 b- defN 22-Sep-16 20:24 cstag-0.3.1/src/cstag/__init__.py
-19 files, 22590 bytes uncompressed, 9495 bytes compressed:  58.0%
+Zip file size: 12102 bytes, number of entries: 19
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 04:48 cstag-0.4.0/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 04:48 cstag-0.4.0/src/
+-rw-r--r--  2.0 unx       38 b- defN 23-Jun-06 04:48 cstag-0.4.0/setup.cfg
+-rw-r--r--  2.0 unx     1069 b- defN 23-Jun-06 04:48 cstag-0.4.0/LICENSE
+-rw-r--r--  2.0 unx     3524 b- defN 23-Jun-06 04:48 cstag-0.4.0/PKG-INFO
+-rw-r--r--  2.0 unx      847 b- defN 23-Jun-06 04:48 cstag-0.4.0/setup.py
+-rw-r--r--  2.0 unx     2929 b- defN 23-Jun-06 04:48 cstag-0.4.0/README.md
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 04:48 cstag-0.4.0/src/cstag.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 04:48 cstag-0.4.0/src/cstag/
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-06 04:48 cstag-0.4.0/src/cstag.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx      285 b- defN 23-Jun-06 04:48 cstag-0.4.0/src/cstag.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx     3524 b- defN 23-Jun-06 04:48 cstag-0.4.0/src/cstag.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-06 04:48 cstag-0.4.0/src/cstag.egg-info/top_level.txt
+-rw-r--r--  2.0 unx      185 b- defN 23-Jun-06 04:48 cstag-0.4.0/src/cstag/__init__.py
+-rw-r--r--  2.0 unx     1306 b- defN 23-Jun-06 04:48 cstag-0.4.0/src/cstag/lengthen.py
+-rw-r--r--  2.0 unx     3840 b- defN 23-Jun-06 04:48 cstag-0.4.0/src/cstag/to_html.py
+-rw-r--r--  2.0 unx      687 b- defN 23-Jun-06 04:48 cstag-0.4.0/src/cstag/shorten.py
+-rw-r--r--  2.0 unx     1902 b- defN 23-Jun-06 04:48 cstag-0.4.0/src/cstag/mask.py
+-rw-r--r--  2.0 unx     2547 b- defN 23-Jun-06 04:48 cstag-0.4.0/src/cstag/consensus.py
+19 files, 22690 bytes uncompressed, 9534 bytes compressed:  58.0%
```

## zipnote {}

```diff
@@ -1,58 +1,58 @@
-Filename: cstag-0.3.1/
+Filename: cstag-0.4.0/
 Comment: 
 
-Filename: cstag-0.3.1/src/
+Filename: cstag-0.4.0/src/
 Comment: 
 
-Filename: cstag-0.3.1/setup.py
+Filename: cstag-0.4.0/setup.cfg
 Comment: 
 
-Filename: cstag-0.3.1/setup.cfg
+Filename: cstag-0.4.0/LICENSE
 Comment: 
 
-Filename: cstag-0.3.1/LICENSE
+Filename: cstag-0.4.0/PKG-INFO
 Comment: 
 
-Filename: cstag-0.3.1/README.md
+Filename: cstag-0.4.0/setup.py
 Comment: 
 
-Filename: cstag-0.3.1/PKG-INFO
+Filename: cstag-0.4.0/README.md
 Comment: 
 
-Filename: cstag-0.3.1/src/cstag.egg-info/
+Filename: cstag-0.4.0/src/cstag.egg-info/
 Comment: 
 
-Filename: cstag-0.3.1/src/cstag/
+Filename: cstag-0.4.0/src/cstag/
 Comment: 
 
-Filename: cstag-0.3.1/src/cstag.egg-info/SOURCES.txt
+Filename: cstag-0.4.0/src/cstag.egg-info/dependency_links.txt
 Comment: 
 
-Filename: cstag-0.3.1/src/cstag.egg-info/top_level.txt
+Filename: cstag-0.4.0/src/cstag.egg-info/SOURCES.txt
 Comment: 
 
-Filename: cstag-0.3.1/src/cstag.egg-info/dependency_links.txt
+Filename: cstag-0.4.0/src/cstag.egg-info/PKG-INFO
 Comment: 
 
-Filename: cstag-0.3.1/src/cstag.egg-info/PKG-INFO
+Filename: cstag-0.4.0/src/cstag.egg-info/top_level.txt
 Comment: 
 
-Filename: cstag-0.3.1/src/cstag/shorten.py
+Filename: cstag-0.4.0/src/cstag/__init__.py
 Comment: 
 
-Filename: cstag-0.3.1/src/cstag/lengthen.py
+Filename: cstag-0.4.0/src/cstag/lengthen.py
 Comment: 
 
-Filename: cstag-0.3.1/src/cstag/mask.py
+Filename: cstag-0.4.0/src/cstag/to_html.py
 Comment: 
 
-Filename: cstag-0.3.1/src/cstag/consensus.py
+Filename: cstag-0.4.0/src/cstag/shorten.py
 Comment: 
 
-Filename: cstag-0.3.1/src/cstag/to_html.py
+Filename: cstag-0.4.0/src/cstag/mask.py
 Comment: 
 
-Filename: cstag-0.3.1/src/cstag/__init__.py
+Filename: cstag-0.4.0/src/cstag/consensus.py
 Comment: 
 
 Zip file comment:
```

## Comparing `cstag-0.3.1/setup.py` & `cstag-0.4.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="cstag",
-    version="0.3.1",
+    version="0.4.0",
     author="Akihiro Kuno",
     author_email="akuno@md.tsukuba.ac.jp",
     description="Python module to manipulate the minimap2's CS tag",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/akikuno/cstag",
     packages=setuptools.find_packages(where="src",),
```

## Comparing `cstag-0.3.1/LICENSE` & `cstag-0.4.0/LICENSE`

 * *Files identical despite different names*

## Comparing `cstag-0.3.1/README.md` & `cstag-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [![Licence](https://img.shields.io/badge/License-MIT-9cf.svg?style=flat-square)](https://choosealicense.com/licenses/mit/)
-[![Test](https://img.shields.io/github/workflow/status/akikuno/cstag/Pytest?json&label=Test&color=brightgreen&style=flat-square)](https://github.com/akikuno/cstag/actions)
+[![Test](https://img.shields.io/github/actions/workflow/status/akikuno/cstag/test.yml?branch=main&label=Test&color=brightgreen&style=flat-square)](https://github.com/akikuno/cstag/actions)
 [![Python](https://img.shields.io/pypi/pyversions/cstag.svg?label=Python&color=blue&style=flat-square)](https://pypi.org/project/cstag/)
 [![PyPI](https://img.shields.io/pypi/v/cstag.svg?label=PyPI&color=orange&style=flat-square)](https://pypi.org/project/cstag/)
 [![Bioconda](https://img.shields.io/conda/v/bioconda/cstag?label=Bioconda&color=orange&style=flat-square)](https://anaconda.org/bioconda/cstag)
 
 # cstag
 
 `cstag` is a Python module to manipulate [minimap2's CS tag](https://github.com/lh3/minimap2#cs).
```

## Comparing `cstag-0.3.1/PKG-INFO` & `cstag-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cstag
-Version: 0.3.1
+Version: 0.4.0
 Summary: Python module to manipulate the minimap2's CS tag
 Home-page: https://github.com/akikuno/cstag
 Author: Akihiro Kuno
 Author-email: akuno@md.tsukuba.ac.jp
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Licence](https://img.shields.io/badge/License-MIT-9cf.svg?style=flat-square)](https://choosealicense.com/licenses/mit/)
-[![Test](https://img.shields.io/github/workflow/status/akikuno/cstag/Pytest?json&label=Test&color=brightgreen&style=flat-square)](https://github.com/akikuno/cstag/actions)
+[![Test](https://img.shields.io/github/actions/workflow/status/akikuno/cstag/test.yml?branch=main&label=Test&color=brightgreen&style=flat-square)](https://github.com/akikuno/cstag/actions)
 [![Python](https://img.shields.io/pypi/pyversions/cstag.svg?label=Python&color=blue&style=flat-square)](https://pypi.org/project/cstag/)
 [![PyPI](https://img.shields.io/pypi/v/cstag.svg?label=PyPI&color=orange&style=flat-square)](https://pypi.org/project/cstag/)
 [![Bioconda](https://img.shields.io/conda/v/bioconda/cstag?label=Bioconda&color=orange&style=flat-square)](https://anaconda.org/bioconda/cstag)
 
 # cstag
 
 `cstag` is a Python module to manipulate [minimap2's CS tag](https://github.com/lh3/minimap2#cs).
```

## Comparing `cstag-0.3.1/src/cstag.egg-info/PKG-INFO` & `cstag-0.4.0/src/cstag.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cstag
-Version: 0.3.1
+Version: 0.4.0
 Summary: Python module to manipulate the minimap2's CS tag
 Home-page: https://github.com/akikuno/cstag
 Author: Akihiro Kuno
 Author-email: akuno@md.tsukuba.ac.jp
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Licence](https://img.shields.io/badge/License-MIT-9cf.svg?style=flat-square)](https://choosealicense.com/licenses/mit/)
-[![Test](https://img.shields.io/github/workflow/status/akikuno/cstag/Pytest?json&label=Test&color=brightgreen&style=flat-square)](https://github.com/akikuno/cstag/actions)
+[![Test](https://img.shields.io/github/actions/workflow/status/akikuno/cstag/test.yml?branch=main&label=Test&color=brightgreen&style=flat-square)](https://github.com/akikuno/cstag/actions)
 [![Python](https://img.shields.io/pypi/pyversions/cstag.svg?label=Python&color=blue&style=flat-square)](https://pypi.org/project/cstag/)
 [![PyPI](https://img.shields.io/pypi/v/cstag.svg?label=PyPI&color=orange&style=flat-square)](https://pypi.org/project/cstag/)
 [![Bioconda](https://img.shields.io/conda/v/bioconda/cstag?label=Bioconda&color=orange&style=flat-square)](https://anaconda.org/bioconda/cstag)
 
 # cstag
 
 `cstag` is a Python module to manipulate [minimap2's CS tag](https://github.com/lh3/minimap2#cs).
```

## Comparing `cstag-0.3.1/src/cstag/shorten.py` & `cstag-0.4.0/src/cstag/shorten.py`

 * *Files identical despite different names*

## Comparing `cstag-0.3.1/src/cstag/lengthen.py` & `cstag-0.4.0/src/cstag/lengthen.py`

 * *Files identical despite different names*

## Comparing `cstag-0.3.1/src/cstag/mask.py` & `cstag-0.4.0/src/cstag/mask.py`

 * *Files identical despite different names*

## Comparing `cstag-0.3.1/src/cstag/consensus.py` & `cstag-0.4.0/src/cstag/consensus.py`

 * *Files identical despite different names*

## Comparing `cstag-0.3.1/src/cstag/to_html.py` & `cstag-0.4.0/src/cstag/to_html.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,14 +99,16 @@
     """
 
     description = DESCRIPTION
     if description:
         description = f"<h1>{description}</h1>"
 
     cs = CSTAG.replace("cs:Z:", "")
+    if cs.startswith("N"):
+        cs = "=" + cs
     list_cs = re.split(r"([-+*~=])", cs)[1:]
     list_cs = [i + j for i, j in zip(list_cs[0::2], list_cs[1::2])]
 
     html_cs = []
     idx = 0
     while idx < len(list_cs):
         cs = list_cs[idx]
```

