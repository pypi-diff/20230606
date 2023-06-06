# Comparing `tmp/hatch_rest_api-1.8.0.tar.gz` & `tmp/hatch_rest_api-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hatch_rest_api-1.8.0.tar", last modified: Tue Mar 29 00:24:20 2022, max compression
+gzip compressed data, was "hatch_rest_api-1.9.0.tar", last modified: Tue Mar 29 00:56:26 2022, max compression
```

## Comparing `hatch_rest_api-1.8.0.tar` & `hatch_rest_api-1.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 00:24:20.291143 hatch_rest_api-1.8.0/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1066 2022-03-29 00:23:42.000000 hatch_rest_api-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-03-29 00:24:20.291143 hatch_rest_api-1.8.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (121)      330 2022-03-29 00:23:42.000000 hatch_rest_api-1.8.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (121)      104 2022-03-29 00:23:42.000000 hatch_rest_api-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-29 00:24:20.291143 hatch_rest_api-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1318 2022-03-29 00:24:06.000000 hatch_rest_api-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 00:24:20.287142 hatch_rest_api-1.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 00:24:20.291143 hatch_rest_api-1.8.0/src/hatch_rest_api/
--rwxr-xr-x   0 runner    (1001) docker     (121)      244 2022-03-29 00:23:42.000000 hatch_rest_api-1.8.0/src/hatch_rest_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-03-29 00:23:42.000000 hatch_rest_api-1.8.0/src/hatch_rest_api/aws_http.py
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-03-29 00:23:42.000000 hatch_rest_api-1.8.0/src/hatch_rest_api/callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      611 2022-03-29 00:23:42.000000 hatch_rest_api-1.8.0/src/hatch_rest_api/const.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      151 2022-03-29 00:23:42.000000 hatch_rest_api-1.8.0/src/hatch_rest_api/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     3523 2022-03-29 00:23:42.000000 hatch_rest_api-1.8.0/src/hatch_rest_api/hatch.py
--rw-r--r--   0 runner    (1001) docker     (121)     6040 2022-03-29 00:23:42.000000 hatch_rest_api-1.8.0/src/hatch_rest_api/rest_mini.py
--rw-r--r--   0 runner    (1001) docker     (121)     1743 2022-03-29 00:23:42.000000 hatch_rest_api-1.8.0/src/hatch_rest_api/stub.py
--rw-r--r--   0 runner    (1001) docker     (121)     1651 2022-03-29 00:23:42.000000 hatch_rest_api-1.8.0/src/hatch_rest_api/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     2527 2022-03-29 00:23:42.000000 hatch_rest_api-1.8.0/src/hatch_rest_api/util_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (121)     1249 2022-03-29 00:23:42.000000 hatch_rest_api-1.8.0/src/hatch_rest_api/util_http.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 00:24:20.291143 hatch_rest_api-1.8.0/src/hatch_rest_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-03-29 00:24:19.000000 hatch_rest_api-1.8.0/src/hatch_rest_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-03-29 00:24:20.000000 hatch_rest_api-1.8.0/src/hatch_rest_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-29 00:24:19.000000 hatch_rest_api-1.8.0/src/hatch_rest_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-03-29 00:24:20.000000 hatch_rest_api-1.8.0/src/hatch_rest_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-03-29 00:24:20.000000 hatch_rest_api-1.8.0/src/hatch_rest_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 00:56:26.436071 hatch_rest_api-1.9.0/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1066 2022-03-29 00:55:49.000000 hatch_rest_api-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-03-29 00:56:26.436071 hatch_rest_api-1.9.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (121)      330 2022-03-29 00:55:49.000000 hatch_rest_api-1.9.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (121)      104 2022-03-29 00:55:49.000000 hatch_rest_api-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-29 00:56:26.436071 hatch_rest_api-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1318 2022-03-29 00:56:14.000000 hatch_rest_api-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 00:56:26.436071 hatch_rest_api-1.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 00:56:26.436071 hatch_rest_api-1.9.0/src/hatch_rest_api/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      244 2022-03-29 00:55:49.000000 hatch_rest_api-1.9.0/src/hatch_rest_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-03-29 00:55:49.000000 hatch_rest_api-1.9.0/src/hatch_rest_api/aws_http.py
+-rw-r--r--   0 runner    (1001) docker     (121)      732 2022-03-29 00:55:49.000000 hatch_rest_api-1.9.0/src/hatch_rest_api/callbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      611 2022-03-29 00:55:49.000000 hatch_rest_api-1.9.0/src/hatch_rest_api/const.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      151 2022-03-29 00:55:49.000000 hatch_rest_api-1.9.0/src/hatch_rest_api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3523 2022-03-29 00:55:49.000000 hatch_rest_api-1.9.0/src/hatch_rest_api/hatch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6040 2022-03-29 00:55:49.000000 hatch_rest_api-1.9.0/src/hatch_rest_api/rest_mini.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1743 2022-03-29 00:55:49.000000 hatch_rest_api-1.9.0/src/hatch_rest_api/stub.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1651 2022-03-29 00:55:49.000000 hatch_rest_api-1.9.0/src/hatch_rest_api/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2527 2022-03-29 00:55:49.000000 hatch_rest_api-1.9.0/src/hatch_rest_api/util_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1249 2022-03-29 00:55:49.000000 hatch_rest_api-1.9.0/src/hatch_rest_api/util_http.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 00:56:26.436071 hatch_rest_api-1.9.0/src/hatch_rest_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-03-29 00:56:25.000000 hatch_rest_api-1.9.0/src/hatch_rest_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      584 2022-03-29 00:56:26.000000 hatch_rest_api-1.9.0/src/hatch_rest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-29 00:56:25.000000 hatch_rest_api-1.9.0/src/hatch_rest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-03-29 00:56:26.000000 hatch_rest_api-1.9.0/src/hatch_rest_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-03-29 00:56:26.000000 hatch_rest_api-1.9.0/src/hatch_rest_api.egg-info/top_level.txt
```

### Comparing `hatch_rest_api-1.8.0/LICENSE` & `hatch_rest_api-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hatch_rest_api-1.8.0/PKG-INFO` & `hatch_rest_api-1.9.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch_rest_api
-Version: 1.8.0
+Version: 1.9.0
 Summary: Hatch Rest mini Api Wrapper
 Home-page: https://github.com/dahlb/hatch_rest_api
 Author: Brendan Dahl
 Author-email: dahl.brendan@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/dahlb/hatch_rest_api/issues
 Project-URL: Source, https://github.com/dahlb/hatch_rest_api
```

### Comparing `hatch_rest_api-1.8.0/setup.py` & `hatch_rest_api-1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 LONG_DESCRIPTION = (here / "README.md").read_text(encoding="utf-8")
 
-VERSION = "1.8.0"
+VERSION = "1.9.0"
 
 # Setting up
 setup(
     name="hatch_rest_api",
     version=VERSION,
     author="Brendan Dahl",
     author_email="dahl.brendan@gmail.com",
     description="Hatch Rest mini Api Wrapper",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
-    install_requires=["aiohttp>=3.8.1", "awsiotsdk==1.9.2"],
+    install_requires=["aiohttp>=3.8.1", "awsiotsdk==1.9.3"],
     keywords=["hatch", "rest-mini", "api"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Framework :: AsyncIO",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Intended Audience :: Developers",
```

### Comparing `hatch_rest_api-1.8.0/src/hatch_rest_api/aws_http.py` & `hatch_rest_api-1.9.0/src/hatch_rest_api/aws_http.py`

 * *Files identical despite different names*

### Comparing `hatch_rest_api-1.8.0/src/hatch_rest_api/callbacks.py` & `hatch_rest_api-1.9.0/src/hatch_rest_api/callbacks.py`

 * *Files identical despite different names*

### Comparing `hatch_rest_api-1.8.0/src/hatch_rest_api/const.py` & `hatch_rest_api-1.9.0/src/hatch_rest_api/const.py`

 * *Files identical despite different names*

### Comparing `hatch_rest_api-1.8.0/src/hatch_rest_api/hatch.py` & `hatch_rest_api-1.9.0/src/hatch_rest_api/hatch.py`

 * *Files identical despite different names*

### Comparing `hatch_rest_api-1.8.0/src/hatch_rest_api/rest_mini.py` & `hatch_rest_api-1.9.0/src/hatch_rest_api/rest_mini.py`

 * *Files identical despite different names*

### Comparing `hatch_rest_api-1.8.0/src/hatch_rest_api/stub.py` & `hatch_rest_api-1.9.0/src/hatch_rest_api/stub.py`

 * *Files identical despite different names*

### Comparing `hatch_rest_api-1.8.0/src/hatch_rest_api/util.py` & `hatch_rest_api-1.9.0/src/hatch_rest_api/util.py`

 * *Files identical despite different names*

### Comparing `hatch_rest_api-1.8.0/src/hatch_rest_api/util_bootstrap.py` & `hatch_rest_api-1.9.0/src/hatch_rest_api/util_bootstrap.py`

 * *Files identical despite different names*

### Comparing `hatch_rest_api-1.8.0/src/hatch_rest_api/util_http.py` & `hatch_rest_api-1.9.0/src/hatch_rest_api/util_http.py`

 * *Files identical despite different names*

### Comparing `hatch_rest_api-1.8.0/src/hatch_rest_api.egg-info/PKG-INFO` & `hatch_rest_api-1.9.0/src/hatch_rest_api.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch-rest-api
-Version: 1.8.0
+Version: 1.9.0
 Summary: Hatch Rest mini Api Wrapper
 Home-page: https://github.com/dahlb/hatch_rest_api
 Author: Brendan Dahl
 Author-email: dahl.brendan@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/dahlb/hatch_rest_api/issues
 Project-URL: Source, https://github.com/dahlb/hatch_rest_api
```

### Comparing `hatch_rest_api-1.8.0/src/hatch_rest_api.egg-info/SOURCES.txt` & `hatch_rest_api-1.9.0/src/hatch_rest_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

