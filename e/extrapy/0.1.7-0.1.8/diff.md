# Comparing `tmp/extrapy-0.1.7.tar.gz` & `tmp/extrapy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extrapy-0.1.7.tar", max compression
+gzip compressed data, was "extrapy-0.1.8.tar", max compression
```

## Comparing `extrapy-0.1.7.tar` & `extrapy-0.1.8.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      835 2023-06-06 14:47:36.111069 extrapy-0.1.7/extrapy/__init__.py
--rw-r--r--   0        0        0      388 2023-06-06 14:47:39.843085 extrapy-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      588 2023-06-06 14:49:26.696143 extrapy-0.1.7/setup.py
--rw-r--r--   0        0        0      320 2023-06-06 14:49:26.696403 extrapy-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      573 2023-06-06 14:54:52.344968 extrapy-0.1.8/extrapy/__init__.py
+-rw-r--r--   0        0        0      388 2023-06-06 14:54:55.020979 extrapy-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      588 2023-06-06 14:55:08.886524 extrapy-0.1.8/setup.py
+-rw-r--r--   0        0        0      320 2023-06-06 14:55:08.888021 extrapy-0.1.8/PKG-INFO
```

### Comparing `extrapy-0.1.7/setup.py` & `extrapy-0.1.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['extrapy']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'extrapy',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': 'Adding in simple things that are tedious to add in on your own, with one simple line you can unlock easiness.',
     'long_description': None,
     'author': 'SalladShooter',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

