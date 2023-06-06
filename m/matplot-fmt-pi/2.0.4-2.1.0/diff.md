# Comparing `tmp/matplot-fmt-pi-2.0.4.tar.gz` & `tmp/matplot-fmt-pi-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/matplot-fmt-pi-2.0.4.tar", last modified: Tue Jan  5 19:58:31 2021, max compression
+gzip compressed data, was "matplot-fmt-pi-2.1.0.tar", last modified: Tue Jun  6 00:23:36 2023, max compression
```

## Comparing `matplot-fmt-pi-2.0.4.tar` & `matplot-fmt-pi-2.1.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 19:58:31.533322 matplot-fmt-pi-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (116)     6214 2021-01-05 19:58:31.533322 matplot-fmt-pi-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4927 2021-01-05 19:58:19.000000 matplot-fmt-pi-2.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 19:58:31.529322 matplot-fmt-pi-2.0.4/matplot_fmt_pi/
--rw-r--r--   0 runner    (1001) docker     (116)      773 2021-01-05 19:58:19.000000 matplot-fmt-pi-2.0.4/matplot_fmt_pi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       13 2021-01-05 19:58:19.000000 matplot-fmt-pi-2.0.4/matplot_fmt_pi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-05 19:58:19.000000 matplot-fmt-pi-2.0.4/matplot_fmt_pi/py.typed
--rw-r--r--   0 runner    (1001) docker     (116)     6213 2021-01-05 19:58:19.000000 matplot-fmt-pi-2.0.4/matplot_fmt_pi/ticker.py
--rw-r--r--   0 runner    (1001) docker     (116)      377 2021-01-05 19:58:19.000000 matplot-fmt-pi-2.0.4/matplot_fmt_pi/ticker.pyi
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 19:58:31.533322 matplot-fmt-pi-2.0.4/matplot_fmt_pi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     6214 2021-01-05 19:58:31.000000 matplot-fmt-pi-2.0.4/matplot_fmt_pi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      374 2021-01-05 19:58:31.000000 matplot-fmt-pi-2.0.4/matplot_fmt_pi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-05 19:58:31.000000 matplot-fmt-pi-2.0.4/matplot_fmt_pi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-05 19:58:31.000000 matplot-fmt-pi-2.0.4/matplot_fmt_pi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       17 2021-01-05 19:58:31.000000 matplot-fmt-pi-2.0.4/matplot_fmt_pi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       15 2021-01-05 19:58:31.000000 matplot-fmt-pi-2.0.4/matplot_fmt_pi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-01-05 19:58:31.533322 matplot-fmt-pi-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1274 2021-01-05 19:58:19.000000 matplot-fmt-pi-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:23:36.116344 matplot-fmt-pi-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-06 00:23:22.000000 matplot-fmt-pi-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-06-06 00:23:36.116344 matplot-fmt-pi-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-06-06 00:23:22.000000 matplot-fmt-pi-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:23:36.112344 matplot-fmt-pi-2.1.0/matplot_fmt_pi/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-06 00:23:22.000000 matplot-fmt-pi-2.1.0/matplot_fmt_pi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-06 00:23:22.000000 matplot-fmt-pi-2.1.0/matplot_fmt_pi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 00:23:22.000000 matplot-fmt-pi-2.1.0/matplot_fmt_pi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-06-06 00:23:22.000000 matplot-fmt-pi-2.1.0/matplot_fmt_pi/ticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-06 00:23:22.000000 matplot-fmt-pi-2.1.0/matplot_fmt_pi/ticker.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:23:36.116344 matplot-fmt-pi-2.1.0/matplot_fmt_pi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-06-06 00:23:35.000000 matplot-fmt-pi-2.1.0/matplot_fmt_pi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-06 00:23:36.000000 matplot-fmt-pi-2.1.0/matplot_fmt_pi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 00:23:35.000000 matplot-fmt-pi-2.1.0/matplot_fmt_pi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 00:23:35.000000 matplot-fmt-pi-2.1.0/matplot_fmt_pi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-06 00:23:35.000000 matplot-fmt-pi-2.1.0/matplot_fmt_pi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-06 00:23:35.000000 matplot-fmt-pi-2.1.0/matplot_fmt_pi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 00:23:36.116344 matplot-fmt-pi-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-06 00:23:22.000000 matplot-fmt-pi-2.1.0/setup.py
```

### Comparing `matplot-fmt-pi-2.0.4/PKG-INFO` & `matplot-fmt-pi-2.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matplot-fmt-pi
-Version: 2.0.4
+Version: 2.1.0
 Summary: Format numbers as multiples of Pi
 Home-page: https://github.com/k-donn/format-pi
 Author: k-donn
 Author-email: k-donn@github.com
 License: MIT
 Description: # Matplotlib Format Pi
         
@@ -12,21 +12,21 @@
         
         ## Branches
         
         ### Master
         
         | Version                                                                                                               | Upload Status                                                                                                                                                                                                                                              | Downloads                                                                                                                      |
         | :-------------------------------------------------------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------- |
-        | [![PyPI](https://img.shields.io/pypi/v/matplot-fmt-pi?label=PyPi%20package)](https://badge.fury.io/py/matplot-fmt-pi) | [![Upload Python Package](https://img.shields.io/github/workflow/status/k-donn/format-pi/Upload%20Python%20Package?label=Upload%20Python%20Package&logo=github)](https://github.com/k-donn/format-pi/actions?query=workflow%3A%22Upload+Python+Package%22) | [![PyPI - Downloads](https://img.shields.io/pypi/dm/matplot-fmt-pi?logo=pypi)](https://pepy.tech/project/matplot-fmt-pi/month) |
+        | [![PyPI](https://img.shields.io/pypi/v/matplot-fmt-pi?label=PyPi%20package)](https://badge.fury.io/py/matplot-fmt-pi) | ![Upload Python Package](https://github.com/k-donn/format-pi/actions/workflows/pythonpublish.yml/badge.svg) | [![PyPI - Downloads](https://img.shields.io/pypi/dm/matplot-fmt-pi?logo=pypi)](https://pepy.tech/project/matplot-fmt-pi/month) |
         
         ### Release
         
         | Version                                                                                                                                                | Upload Status                                                                                                                                                                                                                                                                 | Size                                                                                             |
         | :----------------------------------------------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------- |
-        | [![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/k-donn/format-pi?label=Release)](https://github.com/k-donn/format-pi/tree/release) | [![Upload Python Package](https://img.shields.io/github/workflow/status/k-donn/format-pi/Test%20Upload%20Python%20Package?label=Test%20Upload%20Python%20Package&logo=github)](https://github.com/k-donn/format-pi/actions?query=workflow%3A%22Test+Upload+Python+Package%22) | ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/k-donn/format-pi) |
+        | [![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/k-donn/format-pi?label=Release)](https://github.com/k-donn/format-pi/tree/release) | ![Test Upload Python Package](https://github.com/k-donn/format-pi/actions/workflows/testpythonpublish.yml/badge.svg) | ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/k-donn/format-pi) |
         
         Format multiples of pi as strings on Matplotlib axes.
         
         The `MultiplePi` class creates a [Locator](https://matplotlib.org/api/ticker_api.html?highlight=locator#matplotlib.ticker.MultipleLocator) to place ticks at desired multiples and a [Formatter](https://matplotlib.org/api/ticker_api.html?highlight=locator#matplotlib.ticker.FuncFormatter) to format all tick labels.
         
         The base (π or τ) can be divided by any Natural Number.
```

### Comparing `matplot-fmt-pi-2.0.4/README.md` & `matplot-fmt-pi-2.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 
 ## Branches
 
 ### Master
 
 | Version                                                                                                               | Upload Status                                                                                                                                                                                                                                              | Downloads                                                                                                                      |
 | :-------------------------------------------------------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------- |
-| [![PyPI](https://img.shields.io/pypi/v/matplot-fmt-pi?label=PyPi%20package)](https://badge.fury.io/py/matplot-fmt-pi) | [![Upload Python Package](https://img.shields.io/github/workflow/status/k-donn/format-pi/Upload%20Python%20Package?label=Upload%20Python%20Package&logo=github)](https://github.com/k-donn/format-pi/actions?query=workflow%3A%22Upload+Python+Package%22) | [![PyPI - Downloads](https://img.shields.io/pypi/dm/matplot-fmt-pi?logo=pypi)](https://pepy.tech/project/matplot-fmt-pi/month) |
+| [![PyPI](https://img.shields.io/pypi/v/matplot-fmt-pi?label=PyPi%20package)](https://badge.fury.io/py/matplot-fmt-pi) | ![Upload Python Package](https://github.com/k-donn/format-pi/actions/workflows/pythonpublish.yml/badge.svg) | [![PyPI - Downloads](https://img.shields.io/pypi/dm/matplot-fmt-pi?logo=pypi)](https://pepy.tech/project/matplot-fmt-pi/month) |
 
 ### Release
 
 | Version                                                                                                                                                | Upload Status                                                                                                                                                                                                                                                                 | Size                                                                                             |
 | :----------------------------------------------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------- |
-| [![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/k-donn/format-pi?label=Release)](https://github.com/k-donn/format-pi/tree/release) | [![Upload Python Package](https://img.shields.io/github/workflow/status/k-donn/format-pi/Test%20Upload%20Python%20Package?label=Test%20Upload%20Python%20Package&logo=github)](https://github.com/k-donn/format-pi/actions?query=workflow%3A%22Test+Upload+Python+Package%22) | ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/k-donn/format-pi) |
+| [![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/k-donn/format-pi?label=Release)](https://github.com/k-donn/format-pi/tree/release) | ![Test Upload Python Package](https://github.com/k-donn/format-pi/actions/workflows/testpythonpublish.yml/badge.svg) | ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/k-donn/format-pi) |
 
 Format multiples of pi as strings on Matplotlib axes.
 
 The `MultiplePi` class creates a [Locator](https://matplotlib.org/api/ticker_api.html?highlight=locator#matplotlib.ticker.MultipleLocator) to place ticks at desired multiples and a [Formatter](https://matplotlib.org/api/ticker_api.html?highlight=locator#matplotlib.ticker.FuncFormatter) to format all tick labels.
 
 The base (π or τ) can be divided by any Natural Number.
```

### Comparing `matplot-fmt-pi-2.0.4/matplot_fmt_pi/__init__.py` & `matplot-fmt-pi-2.1.0/matplot_fmt_pi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,10 +18,10 @@
 ----
 Matplotlib has a basic_units.py module that can do this, however,
 it can only do format multiples of pi/2.
 In addition, it forces use of its own cos, sin, etc.
 while this is far more extensible.
 """
 
-__version__ = "2.0.4"
+__version__ = "2.1.0"
 __name__ = "matplot_fmt_pi"
 __pie__ = "Tastes good"
```

### Comparing `matplot-fmt-pi-2.0.4/matplot_fmt_pi/ticker.py` & `matplot-fmt-pi-2.1.0/matplot_fmt_pi/ticker.py`

 * *Files identical despite different names*

### Comparing `matplot-fmt-pi-2.0.4/matplot_fmt_pi.egg-info/PKG-INFO` & `matplot-fmt-pi-2.1.0/matplot_fmt_pi.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matplot-fmt-pi
-Version: 2.0.4
+Version: 2.1.0
 Summary: Format numbers as multiples of Pi
 Home-page: https://github.com/k-donn/format-pi
 Author: k-donn
 Author-email: k-donn@github.com
 License: MIT
 Description: # Matplotlib Format Pi
         
@@ -12,21 +12,21 @@
         
         ## Branches
         
         ### Master
         
         | Version                                                                                                               | Upload Status                                                                                                                                                                                                                                              | Downloads                                                                                                                      |
         | :-------------------------------------------------------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------- |
-        | [![PyPI](https://img.shields.io/pypi/v/matplot-fmt-pi?label=PyPi%20package)](https://badge.fury.io/py/matplot-fmt-pi) | [![Upload Python Package](https://img.shields.io/github/workflow/status/k-donn/format-pi/Upload%20Python%20Package?label=Upload%20Python%20Package&logo=github)](https://github.com/k-donn/format-pi/actions?query=workflow%3A%22Upload+Python+Package%22) | [![PyPI - Downloads](https://img.shields.io/pypi/dm/matplot-fmt-pi?logo=pypi)](https://pepy.tech/project/matplot-fmt-pi/month) |
+        | [![PyPI](https://img.shields.io/pypi/v/matplot-fmt-pi?label=PyPi%20package)](https://badge.fury.io/py/matplot-fmt-pi) | ![Upload Python Package](https://github.com/k-donn/format-pi/actions/workflows/pythonpublish.yml/badge.svg) | [![PyPI - Downloads](https://img.shields.io/pypi/dm/matplot-fmt-pi?logo=pypi)](https://pepy.tech/project/matplot-fmt-pi/month) |
         
         ### Release
         
         | Version                                                                                                                                                | Upload Status                                                                                                                                                                                                                                                                 | Size                                                                                             |
         | :----------------------------------------------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------- |
-        | [![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/k-donn/format-pi?label=Release)](https://github.com/k-donn/format-pi/tree/release) | [![Upload Python Package](https://img.shields.io/github/workflow/status/k-donn/format-pi/Test%20Upload%20Python%20Package?label=Test%20Upload%20Python%20Package&logo=github)](https://github.com/k-donn/format-pi/actions?query=workflow%3A%22Test+Upload+Python+Package%22) | ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/k-donn/format-pi) |
+        | [![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/k-donn/format-pi?label=Release)](https://github.com/k-donn/format-pi/tree/release) | ![Test Upload Python Package](https://github.com/k-donn/format-pi/actions/workflows/testpythonpublish.yml/badge.svg) | ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/k-donn/format-pi) |
         
         Format multiples of pi as strings on Matplotlib axes.
         
         The `MultiplePi` class creates a [Locator](https://matplotlib.org/api/ticker_api.html?highlight=locator#matplotlib.ticker.MultipleLocator) to place ticks at desired multiples and a [Formatter](https://matplotlib.org/api/ticker_api.html?highlight=locator#matplotlib.ticker.FuncFormatter) to format all tick labels.
         
         The base (π or τ) can be divided by any Natural Number.
```

### Comparing `matplot-fmt-pi-2.0.4/setup.py` & `matplot-fmt-pi-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # The dir containing this file
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name="matplot-fmt-pi",
-    version="2.0.4",
+    version="2.1.0",
     description="Format numbers as multiples of Pi",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/k-donn/format-pi",
     author="k-donn",
     author_email="k-donn@github.com",
     license="MIT",
```

