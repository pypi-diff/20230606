# Comparing `tmp/chlore-0.8.1.tar.gz` & `tmp/chlore-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chlore-0.8.1.tar", max compression
+gzip compressed data, was "chlore-0.9.0.tar", max compression
```

## Comparing `chlore-0.8.1.tar` & `chlore-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1072 2022-07-18 13:56:31.466626 chlore-0.8.1/LICENSE
--rw-r--r--   0        0        0        0 2022-07-15 20:34:19.096976 chlore-0.8.1/chlore/__init__.py
--rw-r--r--   0        0        0      420 2022-07-18 20:21:30.791217 chlore-0.8.1/chlore/config.py
--rw-r--r--   0        0        0     2874 2022-07-29 12:23:11.794847 chlore-0.8.1/chlore/controller.py
--rw-r--r--   0        0        0     2244 2022-08-05 13:31:09.431483 chlore-0.8.1/chlore/form.py
--rw-r--r--   0        0        0     2325 2022-08-03 12:15:43.928468 chlore-0.8.1/chlore/jinja.py
--rw-r--r--   0        0        0     2724 2022-07-20 16:57:52.279702 chlore-0.8.1/chlore/logging.py
--rw-r--r--   0        0        0      608 2022-07-20 16:10:54.184993 chlore-0.8.1/chlore/request.py
--rw-r--r--   0        0        0        0 2022-08-03 15:58:47.766974 chlore-0.8.1/chlore/testing/__init__.py
--rw-r--r--   0        0        0      569 2022-08-03 16:08:00.344460 chlore-0.8.1/chlore/testing/dependencies.py
--rw-r--r--   0        0        0     2271 2022-08-03 17:08:34.919183 chlore-0.8.1/chlore/testing/web.py
--rw-r--r--   0        0        0      677 2022-08-05 13:42:33.521619 chlore-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      804 2022-08-05 13:49:02.389036 chlore-0.8.1/setup.py
--rw-r--r--   0        0        0      631 2022-08-05 13:49:02.389267 chlore-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2022-08-16 10:06:31.410760 chlore-0.9.0/LICENSE
+-rw-r--r--   0        0        0        0 2022-08-16 10:06:31.410760 chlore-0.9.0/chlore/__init__.py
+-rw-r--r--   0        0        0     1095 2022-08-16 10:06:31.410760 chlore-0.9.0/chlore/config.py
+-rw-r--r--   0        0        0     2874 2022-08-16 10:06:31.410760 chlore-0.9.0/chlore/controller.py
+-rw-r--r--   0        0        0     2244 2022-08-16 10:06:31.410760 chlore-0.9.0/chlore/form.py
+-rw-r--r--   0        0        0     2325 2022-08-16 10:06:31.410760 chlore-0.9.0/chlore/jinja.py
+-rw-r--r--   0        0        0     2724 2022-08-16 10:06:31.410760 chlore-0.9.0/chlore/logging.py
+-rw-r--r--   0        0        0      608 2022-08-16 10:06:31.410760 chlore-0.9.0/chlore/request.py
+-rw-r--r--   0        0        0        0 2022-08-16 10:06:31.410760 chlore-0.9.0/chlore/testing/__init__.py
+-rw-r--r--   0        0        0      569 2022-08-16 10:06:31.410760 chlore-0.9.0/chlore/testing/dependencies.py
+-rw-r--r--   0        0        0     2271 2022-08-16 10:06:31.410760 chlore-0.9.0/chlore/testing/web.py
+-rw-r--r--   0        0        0      677 2022-08-16 11:46:36.725463 chlore-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      804 2022-08-16 11:46:37.593397 chlore-0.9.0/setup.py
+-rw-r--r--   0        0        0      631 2022-08-16 11:46:37.593580 chlore-0.9.0/PKG-INFO
```

### Comparing `chlore-0.8.1/LICENSE` & `chlore-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chlore-0.8.1/chlore/controller.py` & `chlore-0.9.0/chlore/controller.py`

 * *Files identical despite different names*

### Comparing `chlore-0.8.1/chlore/form.py` & `chlore-0.9.0/chlore/form.py`

 * *Files identical despite different names*

### Comparing `chlore-0.8.1/chlore/jinja.py` & `chlore-0.9.0/chlore/jinja.py`

 * *Files identical despite different names*

### Comparing `chlore-0.8.1/chlore/logging.py` & `chlore-0.9.0/chlore/logging.py`

 * *Files identical despite different names*

### Comparing `chlore-0.8.1/chlore/request.py` & `chlore-0.9.0/chlore/request.py`

 * *Files identical despite different names*

### Comparing `chlore-0.8.1/chlore/testing/dependencies.py` & `chlore-0.9.0/chlore/testing/dependencies.py`

 * *Files identical despite different names*

### Comparing `chlore-0.8.1/chlore/testing/web.py` & `chlore-0.9.0/chlore/testing/web.py`

 * *Files identical despite different names*

### Comparing `chlore-0.8.1/pyproject.toml` & `chlore-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chlore"
-version = "0.8.1"
+version = "0.9.0"
 description = "Web utilities with a good smell"
 authors = [
     "Clément \"Doom\" Doumergue <clement.doumergue@etna.io>",
 ]
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `chlore-0.8.1/setup.py` & `chlore-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'fastapi>=0.79.0,<0.80.0',
  'pydantic>=1.9.1,<2.0.0',
  'requests>=2.28.1,<3.0.0',
  'structlog>=21.5.0,<22.0.0']
 
 setup_kwargs = {
     'name': 'chlore',
-    'version': '0.8.1',
+    'version': '0.9.0',
     'description': 'Web utilities with a good smell',
     'long_description': None,
     'author': 'Clément "Doom" Doumergue',
     'author_email': 'clement.doumergue@etna.io',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `chlore-0.8.1/PKG-INFO` & `chlore-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chlore
-Version: 0.8.1
+Version: 0.9.0
 Summary: Web utilities with a good smell
 License: MIT
 Author: Clément "Doom" Doumergue
 Author-email: clement.doumergue@etna.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

