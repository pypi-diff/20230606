# Comparing `tmp/readthedocs-sphinx-ext-2.2.0.tar.gz` & `tmp/readthedocs-sphinx-ext-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readthedocs-sphinx-ext-2.2.0.tar", last modified: Tue Oct 25 15:59:36 2022, max compression
+gzip compressed data, was "readthedocs-sphinx-ext-2.2.1.tar", last modified: Tue Jun  6 20:54:02 2023, max compression
```

## Comparing `readthedocs-sphinx-ext-2.2.0.tar` & `readthedocs-sphinx-ext-2.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-10-25 15:59:36.479214 readthedocs-sphinx-ext-2.2.0/
--rw-r--r--   0 eric       (501) staff       (20)     1083 2022-10-25 15:53:21.000000 readthedocs-sphinx-ext-2.2.0/LICENSE
--rw-r--r--   0 eric       (501) staff       (20)      250 2022-10-25 15:53:21.000000 readthedocs-sphinx-ext-2.2.0/MANIFEST.in
--rw-r--r--   0 eric       (501) staff       (20)     1443 2022-10-25 15:59:36.479261 readthedocs-sphinx-ext-2.2.0/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     1162 2022-10-25 15:53:21.000000 readthedocs-sphinx-ext-2.2.0/README.rst
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-10-25 15:59:36.476878 readthedocs-sphinx-ext-2.2.0/readthedocs_ext/
--rw-r--r--   0 eric       (501) staff       (20)        0 2022-10-25 15:53:21.000000 readthedocs-sphinx-ext-2.2.0/readthedocs_ext/__init__.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-10-25 15:59:36.477030 readthedocs-sphinx-ext-2.2.0/readthedocs_ext/_templates/
--rw-r--r--   0 eric       (501) staff       (20)     1166 2022-10-25 15:53:21.000000 readthedocs-sphinx-ext-2.2.0/readthedocs_ext/_templates/readthedocs-insert.html.tmpl
--rw-r--r--   0 eric       (501) staff       (20)     2400 2022-10-25 15:53:21.000000 readthedocs-sphinx-ext-2.2.0/readthedocs_ext/embed.py
--rw-r--r--   0 eric       (501) staff       (20)     2140 2022-10-25 15:53:21.000000 readthedocs-sphinx-ext-2.2.0/readthedocs_ext/external_version_warning.py
--rw-r--r--   0 eric       (501) staff       (20)    15172 2022-10-25 15:53:21.000000 readthedocs-sphinx-ext-2.2.0/readthedocs_ext/readthedocs.py
--rw-r--r--   0 eric       (501) staff       (20)      576 2022-10-25 15:53:21.000000 readthedocs-sphinx-ext-2.2.0/readthedocs_ext/template-meta.py
--rw-r--r--   0 eric       (501) staff       (20)     2215 2022-10-25 15:53:21.000000 readthedocs-sphinx-ext-2.2.0/readthedocs_ext/versionwarning.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-10-25 15:59:36.477672 readthedocs-sphinx-ext-2.2.0/readthedocs_sphinx_ext.egg-info/
--rw-r--r--   0 eric       (501) staff       (20)     1443 2022-10-25 15:59:36.000000 readthedocs-sphinx-ext-2.2.0/readthedocs_sphinx_ext.egg-info/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)      855 2022-10-25 15:59:36.000000 readthedocs-sphinx-ext-2.2.0/readthedocs_sphinx_ext.egg-info/SOURCES.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2022-10-25 15:59:36.000000 readthedocs-sphinx-ext-2.2.0/readthedocs_sphinx_ext.egg-info/dependency_links.txt
--rw-r--r--   0 eric       (501) staff       (20)       31 2022-10-25 15:59:36.000000 readthedocs-sphinx-ext-2.2.0/readthedocs_sphinx_ext.egg-info/requires.txt
--rw-r--r--   0 eric       (501) staff       (20)       16 2022-10-25 15:59:36.000000 readthedocs-sphinx-ext-2.2.0/readthedocs_sphinx_ext.egg-info/top_level.txt
--rw-r--r--   0 eric       (501) staff       (20)       67 2022-10-25 15:59:36.479447 readthedocs-sphinx-ext-2.2.0/setup.cfg
--rwxr-xr-x   0 eric       (501) staff       (20)      728 2022-10-25 15:58:44.000000 readthedocs-sphinx-ext-2.2.0/setup.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-10-25 15:59:36.478105 readthedocs-sphinx-ext-2.2.0/tests/
--rw-r--r--   0 eric       (501) staff       (20)        0 2022-10-25 15:53:21.000000 readthedocs-sphinx-ext-2.2.0/tests/__init__.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-10-25 15:59:36.478430 readthedocs-sphinx-ext-2.2.0/tests/pr-example/
--rw-r--r--   0 eric       (501) staff       (20)      760 2022-10-25 15:53:21.000000 readthedocs-sphinx-ext-2.2.0/tests/pr-example/conf.py
--rw-r--r--   0 eric       (501) staff       (20)      315 2022-10-25 15:53:21.000000 readthedocs-sphinx-ext-2.2.0/tests/pr-example/index.rst
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-10-25 15:59:36.478814 readthedocs-sphinx-ext-2.2.0/tests/pyexample/
--rw-r--r--   0 eric       (501) staff       (20)      762 2022-10-25 15:53:21.000000 readthedocs-sphinx-ext-2.2.0/tests/pyexample/conf.py
--rw-r--r--   0 eric       (501) staff       (20)       95 2022-10-25 15:53:21.000000 readthedocs-sphinx-ext-2.2.0/tests/pyexample/escape' this js.rst
--rw-r--r--   0 eric       (501) staff       (20)      315 2022-10-25 15:53:21.000000 readthedocs-sphinx-ext-2.2.0/tests/pyexample/index.rst
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-10-25 15:59:36.479084 readthedocs-sphinx-ext-2.2.0/tests/pyexample-json/
--rw-r--r--   0 eric       (501) staff       (20)      582 2022-10-25 15:53:21.000000 readthedocs-sphinx-ext-2.2.0/tests/pyexample-json/conf.py
--rw-r--r--   0 eric       (501) staff       (20)      315 2022-10-25 15:53:21.000000 readthedocs-sphinx-ext-2.2.0/tests/pyexample-json/index.rst
--rw-r--r--   0 eric       (501) staff       (20)     4521 2022-10-25 15:53:21.000000 readthedocs-sphinx-ext-2.2.0/tests/test_integration.py
--rw-r--r--   0 eric       (501) staff       (20)      768 2022-10-25 15:53:21.000000 readthedocs-sphinx-ext-2.2.0/tests/util.py
+drwxr-xr-x   0 stsewd    (1000) stsewd    (1000)        0 2023-06-06 20:54:02.745692 readthedocs-sphinx-ext-2.2.1/
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)     1083 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/LICENSE
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)      250 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/MANIFEST.in
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)     1443 2023-06-06 20:54:02.745692 readthedocs-sphinx-ext-2.2.1/PKG-INFO
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)     1162 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/README.rst
+drwxr-xr-x   0 stsewd    (1000) stsewd    (1000)        0 2023-06-06 20:54:02.734692 readthedocs-sphinx-ext-2.2.1/readthedocs_ext/
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)        0 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/readthedocs_ext/__init__.py
+drwxr-xr-x   0 stsewd    (1000) stsewd    (1000)        0 2023-06-06 20:54:02.735692 readthedocs-sphinx-ext-2.2.1/readthedocs_ext/_templates/
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)     1166 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/readthedocs_ext/_templates/readthedocs-insert.html.tmpl
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)     2400 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/readthedocs_ext/embed.py
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)     2140 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/readthedocs_ext/external_version_warning.py
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)    14982 2023-06-06 20:44:42.000000 readthedocs-sphinx-ext-2.2.1/readthedocs_ext/readthedocs.py
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)      576 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/readthedocs_ext/template-meta.py
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)     2215 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/readthedocs_ext/versionwarning.py
+drwxr-xr-x   0 stsewd    (1000) stsewd    (1000)        0 2023-06-06 20:54:02.738692 readthedocs-sphinx-ext-2.2.1/readthedocs_sphinx_ext.egg-info/
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)     1443 2023-06-06 20:54:02.000000 readthedocs-sphinx-ext-2.2.1/readthedocs_sphinx_ext.egg-info/PKG-INFO
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)      855 2023-06-06 20:54:02.000000 readthedocs-sphinx-ext-2.2.1/readthedocs_sphinx_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)        1 2023-06-06 20:54:02.000000 readthedocs-sphinx-ext-2.2.1/readthedocs_sphinx_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)       31 2023-06-06 20:54:02.000000 readthedocs-sphinx-ext-2.2.1/readthedocs_sphinx_ext.egg-info/requires.txt
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)       16 2023-06-06 20:54:02.000000 readthedocs-sphinx-ext-2.2.1/readthedocs_sphinx_ext.egg-info/top_level.txt
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)       67 2023-06-06 20:54:02.747692 readthedocs-sphinx-ext-2.2.1/setup.cfg
+-rwxr-xr-x   0 stsewd    (1000) stsewd    (1000)      728 2023-06-06 20:49:35.000000 readthedocs-sphinx-ext-2.2.1/setup.py
+drwxr-xr-x   0 stsewd    (1000) stsewd    (1000)        0 2023-06-06 20:54:02.740692 readthedocs-sphinx-ext-2.2.1/tests/
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)        0 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/tests/__init__.py
+drwxr-xr-x   0 stsewd    (1000) stsewd    (1000)        0 2023-06-06 20:54:02.741692 readthedocs-sphinx-ext-2.2.1/tests/pr-example/
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)      760 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/tests/pr-example/conf.py
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)      315 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/tests/pr-example/index.rst
+drwxr-xr-x   0 stsewd    (1000) stsewd    (1000)        0 2023-06-06 20:54:02.743692 readthedocs-sphinx-ext-2.2.1/tests/pyexample/
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)      762 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/tests/pyexample/conf.py
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)       95 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/tests/pyexample/escape' this js.rst
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)      315 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/tests/pyexample/index.rst
+drwxr-xr-x   0 stsewd    (1000) stsewd    (1000)        0 2023-06-06 20:54:02.745692 readthedocs-sphinx-ext-2.2.1/tests/pyexample-json/
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)      582 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/tests/pyexample-json/conf.py
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)      315 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/tests/pyexample-json/index.rst
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)     4521 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/tests/test_integration.py
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)      768 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/tests/util.py
```

### Comparing `readthedocs-sphinx-ext-2.2.0/LICENSE` & `readthedocs-sphinx-ext-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `readthedocs-sphinx-ext-2.2.0/PKG-INFO` & `readthedocs-sphinx-ext-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readthedocs-sphinx-ext
-Version: 2.2.0
+Version: 2.2.1
 Summary: Sphinx extension for Read the Docs overrides
 Home-page: http://github.com/readthedocs/readthedocs-sphinx-ext
 Author: Read the Docs, Inc
 Author-email: dev@readthedocs.com
 License: MIT
 License-File: LICENSE
```

### Comparing `readthedocs-sphinx-ext-2.2.0/README.rst` & `readthedocs-sphinx-ext-2.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `readthedocs-sphinx-ext-2.2.0/readthedocs_ext/_templates/readthedocs-insert.html.tmpl` & `readthedocs-sphinx-ext-2.2.1/readthedocs_ext/_templates/readthedocs-insert.html.tmpl`

 * *Files identical despite different names*

### Comparing `readthedocs-sphinx-ext-2.2.0/readthedocs_ext/embed.py` & `readthedocs-sphinx-ext-2.2.1/readthedocs_ext/embed.py`

 * *Files identical despite different names*

### Comparing `readthedocs-sphinx-ext-2.2.0/readthedocs_ext/external_version_warning.py` & `readthedocs-sphinx-ext-2.2.1/readthedocs_ext/external_version_warning.py`

 * *Files identical despite different names*

### Comparing `readthedocs-sphinx-ext-2.2.0/readthedocs_ext/readthedocs.py` & `readthedocs-sphinx-ext-2.2.1/readthedocs_ext/readthedocs.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,17 @@
 from __future__ import absolute_import
 
 import codecs
 import json
 import os
 import re
 import types
-from datetime import datetime
 from packaging.version import Version
 
 import sphinx
-from sphinx import package_dir
 from sphinx.util.console import bold
 
 
 from .embed import EmbedDirective
 
 try:
     # Available from Sphinx 1.6
@@ -153,17 +151,15 @@
                 'canonical_url': ctx.get('canonical_url', ''),
                 'theme': ctx.get('html_theme', ''),
                 'builder': 'sphinx',
                 'docroot': ctx.get('conf_py_path', ''),
                 'source_suffix': ctx.get('source_suffix', ''),
                 'page': ctx.get('pagename', ''),
                 'api_host': ctx.get('api_host', ''),
-                'commit': ctx.get('commit', ''),
                 'ad_free': ctx.get('ad_free', ''),
-                'build_date': datetime.utcnow().strftime('%Y-%m-%dT%H:%M:%SZ'),
                 'global_analytics_code': ctx.get('global_analytics_code'),
                 'user_analytics_code': ctx.get('user_analytics_code'),
                 'subprojects': dict(ctx.get('subprojects', [])),
                 'features': {
                     'docsearch_disabled': ctx.get('docsearch_disabled', False),
                 },
             }
```

### Comparing `readthedocs-sphinx-ext-2.2.0/readthedocs_ext/template-meta.py` & `readthedocs-sphinx-ext-2.2.1/readthedocs_ext/template-meta.py`

 * *Files identical despite different names*

### Comparing `readthedocs-sphinx-ext-2.2.0/readthedocs_ext/versionwarning.py` & `readthedocs-sphinx-ext-2.2.1/readthedocs_ext/versionwarning.py`

 * *Files identical despite different names*

### Comparing `readthedocs-sphinx-ext-2.2.0/readthedocs_sphinx_ext.egg-info/PKG-INFO` & `readthedocs-sphinx-ext-2.2.1/readthedocs_sphinx_ext.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readthedocs-sphinx-ext
-Version: 2.2.0
+Version: 2.2.1
 Summary: Sphinx extension for Read the Docs overrides
 Home-page: http://github.com/readthedocs/readthedocs-sphinx-ext
 Author: Read the Docs, Inc
 Author-email: dev@readthedocs.com
 License: MIT
 License-File: LICENSE
```

### Comparing `readthedocs-sphinx-ext-2.2.0/readthedocs_sphinx_ext.egg-info/SOURCES.txt` & `readthedocs-sphinx-ext-2.2.1/readthedocs_sphinx_ext.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `readthedocs-sphinx-ext-2.2.0/setup.py` & `readthedocs-sphinx-ext-2.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import codecs
 
 from setuptools import setup, find_packages
 
 setup(
     name='readthedocs-sphinx-ext',
-    version='2.2.0',
+    version='2.2.1',
     author='Read the Docs, Inc',
     author_email='dev@readthedocs.com',
     url='http://github.com/readthedocs/readthedocs-sphinx-ext',
     license='MIT',
     description='Sphinx extension for Read the Docs overrides',
     install_requires=['requests', 'Jinja2>=2.9', 'packaging'],
     package_dir={'': '.'},
```

### Comparing `readthedocs-sphinx-ext-2.2.0/tests/pr-example/conf.py` & `readthedocs-sphinx-ext-2.2.1/tests/pr-example/conf.py`

 * *Files identical despite different names*

### Comparing `readthedocs-sphinx-ext-2.2.0/tests/pyexample/conf.py` & `readthedocs-sphinx-ext-2.2.1/tests/pyexample/conf.py`

 * *Files identical despite different names*

### Comparing `readthedocs-sphinx-ext-2.2.0/tests/pyexample-json/conf.py` & `readthedocs-sphinx-ext-2.2.1/tests/pyexample-json/conf.py`

 * *Files identical despite different names*

### Comparing `readthedocs-sphinx-ext-2.2.0/tests/test_integration.py` & `readthedocs-sphinx-ext-2.2.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `readthedocs-sphinx-ext-2.2.0/tests/util.py` & `readthedocs-sphinx-ext-2.2.1/tests/util.py`

 * *Files identical despite different names*

