# Comparing `tmp/trustero_api-0.0.2.tar.gz` & `tmp/trustero_api-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trustero_api-0.0.2.tar", max compression
+gzip compressed data, was "trustero_api-0.0.3.tar", max compression
```

## Comparing `trustero_api-0.0.2.tar` & `trustero_api-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1009 2023-06-05 16:16:18.874956 trustero_api-0.0.2/PyPI.md
--rw-r--r--   0        0        0      233 2023-06-05 17:22:26.503817 trustero_api-0.0.2/build.py
--rw-r--r--   0        0        0       22 2023-06-05 16:16:18.902325 trustero_api-0.0.2/docs/.gitignore
--rw-r--r--   0        0        0      142 2023-06-05 16:16:18.891900 trustero_api-0.0.2/docs/.sphinxignore
--rw-r--r--   0        0        0     6814 2023-06-05 16:16:18.896784 trustero_api-0.0.2/docs/Makefile
--rw-r--r--   0        0        0      120 2023-06-05 16:16:18.899963 trustero_api-0.0.2/docs/README.md
--rw-r--r--   0        0        0      130 2023-06-05 16:16:18.906979 trustero_api-0.0.2/docs/_static/custom.css
--rw-r--r--   0        0        0     1861 2023-06-05 16:16:18.903666 trustero_api-0.0.2/docs/_themes/LICENSE
--rw-r--r--   0        0        0     3905 2023-06-05 16:16:18.905413 trustero_api-0.0.2/docs/_themes/flask_theme_support.py
--rw-r--r--   0        0        0    13038 2023-06-05 17:49:16.949950 trustero_api-0.0.2/docs/conf.py
--rw-r--r--   0        0        0     1274 2023-06-05 16:16:18.894796 trustero_api-0.0.2/docs/index.rst
--rw-r--r--   0        0        0     6467 2023-06-05 16:16:18.901601 trustero_api-0.0.2/docs/make.bat
--rw-r--r--   0        0        0     1931 2023-06-06 09:08:40.038183 trustero_api-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       29 2023-06-05 16:16:18.948110 trustero_api-0.0.2/src/api/__init__.py
--rw-r--r--   0        0        0       60 2023-06-05 16:16:18.948765 trustero_api-0.0.2/src/api/py.typed
--rw-r--r--   0        0        0        0 2023-06-05 17:46:12.197230 trustero_api-0.0.2/src/api/receptor_v1/__init__.py
--rw-r--r--   0        0        0     6561 2023-06-06 08:58:40.493471 trustero_api-0.0.2/src/api/receptor_v1/receptor_pb2.py
--rw-r--r--   0        0        0       29 2023-06-05 16:16:18.889897 trustero_api-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      201 2023-06-05 19:06:51.410474 trustero_api-0.0.2/tests/test_import.py
--rw-r--r--   0        0        0     2060 1970-01-01 00:00:00.000000 trustero_api-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1009 2023-06-05 16:16:18.874956 trustero_api-0.0.3/PyPI.md
+-rw-r--r--   0        0        0      230 2023-06-06 09:30:42.948598 trustero_api-0.0.3/build.py
+-rw-r--r--   0        0        0       22 2023-06-05 16:16:18.902325 trustero_api-0.0.3/docs/.gitignore
+-rw-r--r--   0        0        0      142 2023-06-05 16:16:18.891900 trustero_api-0.0.3/docs/.sphinxignore
+-rw-r--r--   0        0        0     6814 2023-06-05 16:16:18.896784 trustero_api-0.0.3/docs/Makefile
+-rw-r--r--   0        0        0      120 2023-06-05 16:16:18.899963 trustero_api-0.0.3/docs/README.md
+-rw-r--r--   0        0        0      130 2023-06-05 16:16:18.906979 trustero_api-0.0.3/docs/_static/custom.css
+-rw-r--r--   0        0        0     1861 2023-06-05 16:16:18.903666 trustero_api-0.0.3/docs/_themes/LICENSE
+-rw-r--r--   0        0        0     3905 2023-06-05 16:16:18.905413 trustero_api-0.0.3/docs/_themes/flask_theme_support.py
+-rw-r--r--   0        0        0    13038 2023-06-05 17:49:16.949950 trustero_api-0.0.3/docs/conf.py
+-rw-r--r--   0        0        0     1274 2023-06-05 16:16:18.894796 trustero_api-0.0.3/docs/index.rst
+-rw-r--r--   0        0        0     6467 2023-06-05 16:16:18.901601 trustero_api-0.0.3/docs/make.bat
+-rwxr-xr-x   0        0        0      612 2023-06-05 16:49:16.699356 trustero_api-0.0.3/proto-gen
+-rw-r--r--   0        0        0     1975 2023-06-06 09:53:31.377104 trustero_api-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-06-05 16:16:18.948110 trustero_api-0.0.3/src/api/__init__.py
+-rw-r--r--   0        0        0       60 2023-06-05 16:16:18.948765 trustero_api-0.0.3/src/api/py.typed
+-rw-r--r--   0        0        0        0 2023-06-05 17:46:12.197230 trustero_api-0.0.3/src/api/receptor_v1/__init__.py
+-rw-r--r--   0        0        0     6561 2023-06-06 09:34:12.380508 trustero_api-0.0.3/src/api/receptor_v1/receptor_pb2.py
+-rw-r--r--   0        0        0       29 2023-06-05 16:16:18.889897 trustero_api-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      201 2023-06-05 19:06:51.410474 trustero_api-0.0.3/tests/test_import.py
+-rw-r--r--   0        0        0     2060 1970-01-01 00:00:00.000000 trustero_api-0.0.3/PKG-INFO
```

### Comparing `trustero_api-0.0.2/PyPI.md` & `trustero_api-0.0.3/PyPI.md`

 * *Files identical despite different names*

### Comparing `trustero_api-0.0.2/docs/Makefile` & `trustero_api-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `trustero_api-0.0.2/docs/_themes/LICENSE` & `trustero_api-0.0.3/docs/_themes/LICENSE`

 * *Files identical despite different names*

### Comparing `trustero_api-0.0.2/docs/_themes/flask_theme_support.py` & `trustero_api-0.0.3/docs/_themes/flask_theme_support.py`

 * *Files identical despite different names*

### Comparing `trustero_api-0.0.2/docs/conf.py` & `trustero_api-0.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `trustero_api-0.0.2/docs/index.rst` & `trustero_api-0.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `trustero_api-0.0.2/docs/make.bat` & `trustero_api-0.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `trustero_api-0.0.2/pyproject.toml` & `trustero_api-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "trustero_api"
-version = "0.0.2" 
+version = "0.0.3"
 description = "Trustero Receptor API Python Proto File Bindings"
 authors = ["Alex Gonopolskiy <alex@trustero.com>"]
 license = "Apache-2.0"
 readme = "PyPI.md"
 homepage = "https://pypi.org/project/python/"
 repository = "https://github.com/trustalex/https://github.com/trustero/api"
 include = [
    { path = 'Changelog', format = 'sdist' },
    { path = 'NOTICE', format = 'sdist' },
    { path = 'LICENSE', format = 'sdist' },
    { path = 'README.md', format = 'sdist' },
    { path = 'docs', format = 'sdist' },
    { path = 'tests', format = 'sdist' },
+   { path = 'proto-gen', format = 'sdist' },
 ]
 packages = [ 
    { include = "api", from = "src" },
 ]
 classifiers=[
    "Programming Language :: Python :: 3",
    "License :: OSI Approved :: Apache Software License",
```

### Comparing `trustero_api-0.0.2/src/api/receptor_v1/receptor_pb2.py` & `trustero_api-0.0.3/src/api/receptor_v1/receptor_pb2.py`

 * *Files identical despite different names*

### Comparing `trustero_api-0.0.2/PKG-INFO` & `trustero_api-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustero-api
-Version: 0.0.2
+Version: 0.0.3
 Summary: Trustero Receptor API Python Proto File Bindings
 Home-page: https://pypi.org/project/python/
 License: Apache-2.0
 Author: Alex Gonopolskiy
 Author-email: alex@trustero.com
 Requires-Python: >=3.8,<4
 Classifier: Development Status :: 4 - Beta
```

