# Comparing `tmp/trustero_api-0.0.0.tar.gz` & `tmp/trustero_api-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trustero_api-0.0.0.tar", max compression
+gzip compressed data, was "trustero_api-0.0.1.tar", max compression
```

## Comparing `trustero_api-0.0.0.tar` & `trustero_api-0.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1009 2023-06-05 16:16:18.874956 trustero_api-0.0.0/PyPI.md
--rw-r--r--   0        0        0      233 2023-06-05 17:22:26.503817 trustero_api-0.0.0/build.py
--rw-r--r--   0        0        0       22 2023-06-05 16:16:18.902325 trustero_api-0.0.0/docs/.gitignore
--rw-r--r--   0        0        0      142 2023-06-05 16:16:18.891900 trustero_api-0.0.0/docs/.sphinxignore
--rw-r--r--   0        0        0     6814 2023-06-05 16:16:18.896784 trustero_api-0.0.0/docs/Makefile
--rw-r--r--   0        0        0      120 2023-06-05 16:16:18.899963 trustero_api-0.0.0/docs/README.md
--rw-r--r--   0        0        0      130 2023-06-05 16:16:18.906979 trustero_api-0.0.0/docs/_static/custom.css
--rw-r--r--   0        0        0     1861 2023-06-05 16:16:18.903666 trustero_api-0.0.0/docs/_themes/LICENSE
--rw-r--r--   0        0        0     3905 2023-06-05 16:16:18.905413 trustero_api-0.0.0/docs/_themes/flask_theme_support.py
--rw-r--r--   0        0        0    13038 2023-06-05 17:49:16.949950 trustero_api-0.0.0/docs/conf.py
--rw-r--r--   0        0        0     1274 2023-06-05 16:16:18.894796 trustero_api-0.0.0/docs/index.rst
--rw-r--r--   0        0        0     6467 2023-06-05 16:16:18.901601 trustero_api-0.0.0/docs/make.bat
--rw-r--r--   0        0        0     2483 2023-06-05 19:04:08.194750 trustero_api-0.0.0/pyproject.toml
--rw-r--r--   0        0        0       29 2023-06-05 16:16:18.948110 trustero_api-0.0.0/src/api/__init__.py
--rw-r--r--   0        0        0       60 2023-06-05 16:16:18.948765 trustero_api-0.0.0/src/api/py.typed
--rw-r--r--   0        0        0        0 2023-06-05 17:46:12.197230 trustero_api-0.0.0/src/api/receptor_v1/__init__.py
--rw-r--r--   0        0        0     6561 2023-06-05 19:11:05.984660 trustero_api-0.0.0/src/api/receptor_v1/receptor_pb2.py
--rw-r--r--   0        0        0       29 2023-06-05 16:16:18.889897 trustero_api-0.0.0/tests/__init__.py
--rw-r--r--   0        0        0      201 2023-06-05 19:06:51.410474 trustero_api-0.0.0/tests/test_import.py
--rw-r--r--   0        0        0     1910 1970-01-01 00:00:00.000000 trustero_api-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1009 2023-06-05 16:16:18.874956 trustero_api-0.0.1/PyPI.md
+-rw-r--r--   0        0        0      233 2023-06-05 17:22:26.503817 trustero_api-0.0.1/build.py
+-rw-r--r--   0        0        0       22 2023-06-05 16:16:18.902325 trustero_api-0.0.1/docs/.gitignore
+-rw-r--r--   0        0        0      142 2023-06-05 16:16:18.891900 trustero_api-0.0.1/docs/.sphinxignore
+-rw-r--r--   0        0        0     6814 2023-06-05 16:16:18.896784 trustero_api-0.0.1/docs/Makefile
+-rw-r--r--   0        0        0      120 2023-06-05 16:16:18.899963 trustero_api-0.0.1/docs/README.md
+-rw-r--r--   0        0        0      130 2023-06-05 16:16:18.906979 trustero_api-0.0.1/docs/_static/custom.css
+-rw-r--r--   0        0        0     1861 2023-06-05 16:16:18.903666 trustero_api-0.0.1/docs/_themes/LICENSE
+-rw-r--r--   0        0        0     3905 2023-06-05 16:16:18.905413 trustero_api-0.0.1/docs/_themes/flask_theme_support.py
+-rw-r--r--   0        0        0    13038 2023-06-05 17:49:16.949950 trustero_api-0.0.1/docs/conf.py
+-rw-r--r--   0        0        0     1274 2023-06-05 16:16:18.894796 trustero_api-0.0.1/docs/index.rst
+-rw-r--r--   0        0        0     6467 2023-06-05 16:16:18.901601 trustero_api-0.0.1/docs/make.bat
+-rw-r--r--   0        0        0     2482 2023-06-06 08:57:14.128357 trustero_api-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-06-05 16:16:18.948110 trustero_api-0.0.1/src/api/__init__.py
+-rw-r--r--   0        0        0       60 2023-06-05 16:16:18.948765 trustero_api-0.0.1/src/api/py.typed
+-rw-r--r--   0        0        0        0 2023-06-05 17:46:12.197230 trustero_api-0.0.1/src/api/receptor_v1/__init__.py
+-rw-r--r--   0        0        0     6561 2023-06-06 08:51:32.864505 trustero_api-0.0.1/src/api/receptor_v1/receptor_pb2.py
+-rw-r--r--   0        0        0       29 2023-06-05 16:16:18.889897 trustero_api-0.0.1/tests/__init__.py
+-rw-r--r--   0        0        0      201 2023-06-05 19:06:51.410474 trustero_api-0.0.1/tests/test_import.py
+-rw-r--r--   0        0        0     2060 1970-01-01 00:00:00.000000 trustero_api-0.0.1/PKG-INFO
```

### Comparing `trustero_api-0.0.0/PyPI.md` & `trustero_api-0.0.1/PyPI.md`

 * *Files identical despite different names*

### Comparing `trustero_api-0.0.0/docs/Makefile` & `trustero_api-0.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `trustero_api-0.0.0/docs/_themes/LICENSE` & `trustero_api-0.0.1/docs/_themes/LICENSE`

 * *Files identical despite different names*

### Comparing `trustero_api-0.0.0/docs/_themes/flask_theme_support.py` & `trustero_api-0.0.1/docs/_themes/flask_theme_support.py`

 * *Files identical despite different names*

### Comparing `trustero_api-0.0.0/docs/conf.py` & `trustero_api-0.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `trustero_api-0.0.0/docs/index.rst` & `trustero_api-0.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `trustero_api-0.0.0/docs/make.bat` & `trustero_api-0.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `trustero_api-0.0.0/pyproject.toml` & `trustero_api-0.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trustero_api"
-version = "0.0.0" # published version is managed using Git tags (see below)
+version = "0.0.1" # published version is managed using Git tags (see below)
 description = "Trustero Receptor API Python Proto File Bindings"
 authors = ["Alex Gonopolskiy <alex@trustero.com>"]
 license = "Apache-2.0"
 readme = "PyPI.md"
 homepage = "https://pypi.org/project/python/"
 repository = "https://github.com/trustalex/https://github.com/trustero/api"
 include = [
@@ -29,15 +29,15 @@
 # If the plugin is not installed, then the version is always "0.0.0", taken from above
 [tool.poetry-dynamic-versioning]
 enable = true
 pattern = '^[vV](?P<base>\d+\.\d+\.\d+)'  # this extracts the version from our vX.Y.Z tag format
 format-jinja = "{% if distance == 0 and not dirty %}{{ base }}{% else %}{{ base }}+{{ distance }}.{{ commit }}{% endif %}"
 
 [tool.poetry.dependencies]
-python = ">=3.11,<4"
+python = ">=3.8,<4"
 importlib-metadata = { version="^6.0.0", optional=true }
 sphinx = { version="^6.1.3", optional=true }
 sphinx-autoapi = { version="^2.0.1", optional=true }
 protobuf = "^4.23.2"
 types-protobuf = "^4.23.0.1"
 
 [tool.poetry.extras]
```

### Comparing `trustero_api-0.0.0/src/api/receptor_v1/receptor_pb2.py` & `trustero_api-0.0.1/src/api/receptor_v1/receptor_pb2.py`

 * *Files identical despite different names*

### Comparing `trustero_api-0.0.0/PKG-INFO` & `trustero_api-0.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: trustero-api
-Version: 0.0.0
+Version: 0.0.1
 Summary: Trustero Receptor API Python Proto File Bindings
 Home-page: https://pypi.org/project/python/
 License: Apache-2.0
 Author: Alex Gonopolskiy
 Author-email: alex@trustero.com
-Requires-Python: >=3.11,<4
+Requires-Python: >=3.8,<4
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Requires-Dist: importlib-metadata (>=6.0.0,<7.0.0) ; extra == "docs"
 Requires-Dist: protobuf (>=4.23.2,<5.0.0)
 Requires-Dist: sphinx (>=6.1.3,<7.0.0) ; extra == "docs"
 Requires-Dist: sphinx-autoapi (>=2.0.1,<3.0.0) ; extra == "docs"
 Requires-Dist: types-protobuf (>=4.23.0.1,<5.0.0.0)
```

