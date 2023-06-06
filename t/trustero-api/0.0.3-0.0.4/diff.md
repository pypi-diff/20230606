# Comparing `tmp/trustero_api-0.0.3.tar.gz` & `tmp/trustero_api-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trustero_api-0.0.3.tar", max compression
+gzip compressed data, was "trustero_api-0.0.4.tar", max compression
```

## Comparing `trustero_api-0.0.3.tar` & `trustero_api-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1009 2023-06-05 16:16:18.874956 trustero_api-0.0.3/PyPI.md
--rw-r--r--   0        0        0      230 2023-06-06 09:30:42.948598 trustero_api-0.0.3/build.py
--rw-r--r--   0        0        0       22 2023-06-05 16:16:18.902325 trustero_api-0.0.3/docs/.gitignore
--rw-r--r--   0        0        0      142 2023-06-05 16:16:18.891900 trustero_api-0.0.3/docs/.sphinxignore
--rw-r--r--   0        0        0     6814 2023-06-05 16:16:18.896784 trustero_api-0.0.3/docs/Makefile
--rw-r--r--   0        0        0      120 2023-06-05 16:16:18.899963 trustero_api-0.0.3/docs/README.md
--rw-r--r--   0        0        0      130 2023-06-05 16:16:18.906979 trustero_api-0.0.3/docs/_static/custom.css
--rw-r--r--   0        0        0     1861 2023-06-05 16:16:18.903666 trustero_api-0.0.3/docs/_themes/LICENSE
--rw-r--r--   0        0        0     3905 2023-06-05 16:16:18.905413 trustero_api-0.0.3/docs/_themes/flask_theme_support.py
--rw-r--r--   0        0        0    13038 2023-06-05 17:49:16.949950 trustero_api-0.0.3/docs/conf.py
--rw-r--r--   0        0        0     1274 2023-06-05 16:16:18.894796 trustero_api-0.0.3/docs/index.rst
--rw-r--r--   0        0        0     6467 2023-06-05 16:16:18.901601 trustero_api-0.0.3/docs/make.bat
--rwxr-xr-x   0        0        0      612 2023-06-05 16:49:16.699356 trustero_api-0.0.3/proto-gen
--rw-r--r--   0        0        0     1975 2023-06-06 09:53:31.377104 trustero_api-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       29 2023-06-05 16:16:18.948110 trustero_api-0.0.3/src/api/__init__.py
--rw-r--r--   0        0        0       60 2023-06-05 16:16:18.948765 trustero_api-0.0.3/src/api/py.typed
--rw-r--r--   0        0        0        0 2023-06-05 17:46:12.197230 trustero_api-0.0.3/src/api/receptor_v1/__init__.py
--rw-r--r--   0        0        0     6561 2023-06-06 09:34:12.380508 trustero_api-0.0.3/src/api/receptor_v1/receptor_pb2.py
--rw-r--r--   0        0        0       29 2023-06-05 16:16:18.889897 trustero_api-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0      201 2023-06-05 19:06:51.410474 trustero_api-0.0.3/tests/test_import.py
--rw-r--r--   0        0        0     2060 1970-01-01 00:00:00.000000 trustero_api-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1009 2023-06-05 16:16:18.874956 trustero_api-0.0.4/PyPI.md
+-rw-r--r--   0        0        0      230 2023-06-06 09:30:42.948598 trustero_api-0.0.4/build.py
+-rw-r--r--   0        0        0       22 2023-06-05 16:16:18.902325 trustero_api-0.0.4/docs/.gitignore
+-rw-r--r--   0        0        0      142 2023-06-05 16:16:18.891900 trustero_api-0.0.4/docs/.sphinxignore
+-rw-r--r--   0        0        0     6814 2023-06-05 16:16:18.896784 trustero_api-0.0.4/docs/Makefile
+-rw-r--r--   0        0        0      120 2023-06-05 16:16:18.899963 trustero_api-0.0.4/docs/README.md
+-rw-r--r--   0        0        0      130 2023-06-05 16:16:18.906979 trustero_api-0.0.4/docs/_static/custom.css
+-rw-r--r--   0        0        0     1861 2023-06-05 16:16:18.903666 trustero_api-0.0.4/docs/_themes/LICENSE
+-rw-r--r--   0        0        0     3905 2023-06-05 16:16:18.905413 trustero_api-0.0.4/docs/_themes/flask_theme_support.py
+-rw-r--r--   0        0        0    13038 2023-06-05 17:49:16.949950 trustero_api-0.0.4/docs/conf.py
+-rw-r--r--   0        0        0     1274 2023-06-05 16:16:18.894796 trustero_api-0.0.4/docs/index.rst
+-rw-r--r--   0        0        0     6467 2023-06-05 16:16:18.901601 trustero_api-0.0.4/docs/make.bat
+-rwxr-xr-x   0        0        0      621 2023-06-06 10:12:03.992060 trustero_api-0.0.4/proto-gen
+-rw-r--r--   0        0        0     2002 2023-06-06 10:14:04.364965 trustero_api-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-06-05 16:16:18.948110 trustero_api-0.0.4/src/trustero_api/__init__.py
+-rw-r--r--   0        0        0       60 2023-06-05 16:16:18.948765 trustero_api-0.0.4/src/trustero_api/py.typed
+-rw-r--r--   0        0        0        0 2023-06-05 17:46:12.197230 trustero_api-0.0.4/src/trustero_api/receptor_v1/__init__.py
+-rw-r--r--   0        0        0     6561 2023-06-06 10:13:12.421401 trustero_api-0.0.4/src/trustero_api/receptor_v1/receptor_pb2.py
+-rw-r--r--   0        0        0       29 2023-06-05 16:16:18.889897 trustero_api-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      201 2023-06-05 19:06:51.410474 trustero_api-0.0.4/tests/test_import.py
+-rw-r--r--   0        0        0     2060 1970-01-01 00:00:00.000000 trustero_api-0.0.4/PKG-INFO
```

### Comparing `trustero_api-0.0.3/PyPI.md` & `trustero_api-0.0.4/PyPI.md`

 * *Files identical despite different names*

### Comparing `trustero_api-0.0.3/docs/Makefile` & `trustero_api-0.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `trustero_api-0.0.3/docs/_themes/LICENSE` & `trustero_api-0.0.4/docs/_themes/LICENSE`

 * *Files identical despite different names*

### Comparing `trustero_api-0.0.3/docs/_themes/flask_theme_support.py` & `trustero_api-0.0.4/docs/_themes/flask_theme_support.py`

 * *Files identical despite different names*

### Comparing `trustero_api-0.0.3/docs/conf.py` & `trustero_api-0.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `trustero_api-0.0.3/docs/index.rst` & `trustero_api-0.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `trustero_api-0.0.3/docs/make.bat` & `trustero_api-0.0.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `trustero_api-0.0.3/proto-gen` & `trustero_api-0.0.4/proto-gen`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 PROTOC_FLAGS="--experimental_allow_proto3_optional"
 PROTO_MODULES="receptor_v1"
 PROTOS_SRC_DIR="../proto/"
 
 export GO111MODULE=on
 export PATH=$PATH:$GO_PATH_BIN
 
-outDir="src/api"
+outDir="src/trustero_api"
 
 for module in $PROTO_MODULES; do
   proto_files=$(find ../proto/"${module}" -name "*.proto")
 
   for proto in $proto_files; do
     protoc $PROTOC_FLAGS \
           --python_out=$outDir \
```

### Comparing `trustero_api-0.0.3/pyproject.toml` & `trustero_api-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trustero_api"
-version = "0.0.3"
+version = "0.0.4"
 description = "Trustero Receptor API Python Proto File Bindings"
 authors = ["Alex Gonopolskiy <alex@trustero.com>"]
 license = "Apache-2.0"
 readme = "PyPI.md"
 homepage = "https://pypi.org/project/python/"
 repository = "https://github.com/trustalex/https://github.com/trustero/api"
 include = [
@@ -13,15 +13,15 @@
    { path = 'LICENSE', format = 'sdist' },
    { path = 'README.md', format = 'sdist' },
    { path = 'docs', format = 'sdist' },
    { path = 'tests', format = 'sdist' },
    { path = 'proto-gen', format = 'sdist' },
 ]
 packages = [ 
-   { include = "api", from = "src" },
+   { include = "trustero_api", from = "src" },
 ]
 classifiers=[
    "Programming Language :: Python :: 3",
    "License :: OSI Approved :: Apache Software License",
    "Development Status :: 4 - Beta",
 ]
 
@@ -60,22 +60,22 @@
   | \.tox
   | \.venv
   | \.poetry
   | build
   | dist
   | docs
   | notes
-  | src/api/receptor_v1
+  | src/trustero_api/receptor_v1
 )/
 '''
 
 [tool.isort]
 profile = "black"
 line_length = 132
-skip_glob = [ "docs", "notes", "src/api/receptor_v1"]
+skip_glob = [ "docs", "notes", "src/trustero_api/receptor_v1"]
 
 [build-system]
 requires = ["poetry>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry.build]
 generate-setup-file = false
```

### Comparing `trustero_api-0.0.3/src/api/receptor_v1/receptor_pb2.py` & `trustero_api-0.0.4/src/trustero_api/receptor_v1/receptor_pb2.py`

 * *Files identical despite different names*

### Comparing `trustero_api-0.0.3/PKG-INFO` & `trustero_api-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustero-api
-Version: 0.0.3
+Version: 0.0.4
 Summary: Trustero Receptor API Python Proto File Bindings
 Home-page: https://pypi.org/project/python/
 License: Apache-2.0
 Author: Alex Gonopolskiy
 Author-email: alex@trustero.com
 Requires-Python: >=3.8,<4
 Classifier: Development Status :: 4 - Beta
```

