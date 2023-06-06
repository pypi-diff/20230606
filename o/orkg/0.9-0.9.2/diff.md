# Comparing `tmp/orkg-0.9.tar.gz` & `tmp/orkg-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/orkg-0.9.tar", last modified: Fri Feb  5 11:24:45 2021, max compression
+gzip compressed data, was "dist/orkg-0.9.2.tar", last modified: Thu Feb 25 12:12:40 2021, max compression
```

## Comparing `orkg-0.9.tar` & `orkg-0.9.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 jaradeh   (1000) jaradeh   (1000)        0 2021-02-05 11:24:45.000000 orkg-0.9/
--rwxr-xr-x   0 jaradeh   (1000) jaradeh   (1000)     1310 2021-02-05 11:19:02.000000 orkg-0.9/setup.py
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)      524 2020-07-21 09:00:14.000000 orkg-0.9/README.md
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     1624 2021-02-05 11:24:45.000000 orkg-0.9/PKG-INFO
-drwxr-xr-x   0 jaradeh   (1000) jaradeh   (1000)        0 2021-02-05 11:24:45.000000 orkg-0.9/orkg.egg-info/
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     1624 2021-02-05 11:24:45.000000 orkg-0.9/orkg.egg-info/PKG-INFO
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)      753 2021-02-05 11:24:45.000000 orkg-0.9/orkg.egg-info/SOURCES.txt
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)        1 2021-02-05 11:24:45.000000 orkg-0.9/orkg.egg-info/dependency_links.txt
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)       15 2021-02-05 11:24:45.000000 orkg-0.9/orkg.egg-info/requires.txt
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)       11 2021-02-05 11:24:45.000000 orkg-0.9/orkg.egg-info/top_level.txt
-drwxr-xr-x   0 jaradeh   (1000) jaradeh   (1000)        0 2021-02-05 11:24:45.000000 orkg-0.9/orkg/
-drwxr-xr-x   0 jaradeh   (1000) jaradeh   (1000)        0 2021-02-05 11:24:45.000000 orkg-0.9/orkg/client/
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     3050 2020-07-21 08:22:45.000000 orkg-0.9/orkg/client/classes.py
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)      271 2020-02-21 15:15:29.000000 orkg-0.9/orkg/client/stats.py
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)       25 2020-02-21 15:15:29.000000 orkg-0.9/orkg/client/__init__.py
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     9184 2020-07-28 10:48:05.000000 orkg-0.9/orkg/client/resources.py
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     2603 2020-07-21 08:22:45.000000 orkg-0.9/orkg/client/predicates.py
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     3440 2020-09-30 08:30:02.000000 orkg-0.9/orkg/client/contributions.py
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     3561 2020-07-28 10:48:05.000000 orkg-0.9/orkg/client/statements.py
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     1595 2020-07-21 08:22:45.000000 orkg-0.9/orkg/client/literals.py
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)    10293 2020-07-21 08:57:37.000000 orkg-0.9/orkg/client/papers.py
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)      663 2021-02-05 11:05:13.000000 orkg-0.9/orkg/client/objects.py
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     1810 2020-07-21 08:22:45.000000 orkg-0.9/orkg/client/comparisons.py
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     2452 2021-02-05 11:09:53.000000 orkg-0.9/orkg/client/backend.py
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)      296 2020-02-21 15:15:29.000000 orkg-0.9/orkg/__init__.py
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     2730 2020-07-21 08:22:45.000000 orkg-0.9/orkg/utils.py
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)      993 2020-07-21 08:22:45.000000 orkg-0.9/orkg/out.py
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)       79 2021-02-05 11:24:45.000000 orkg-0.9/setup.cfg
-drwxr-xr-x   0 jaradeh   (1000) jaradeh   (1000)        0 2021-02-05 11:24:45.000000 orkg-0.9/tests/
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     1200 2020-02-21 15:15:29.000000 orkg-0.9/tests/test_literals.py
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     1966 2020-07-21 08:22:45.000000 orkg-0.9/tests/test_predicates.py
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)        0 2020-02-21 15:15:29.000000 orkg-0.9/tests/__init__.py
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)      305 2020-02-21 15:15:29.000000 orkg-0.9/tests/test_stats.py
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     2236 2020-07-21 08:22:45.000000 orkg-0.9/tests/test_classes.py
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     2262 2020-07-28 10:48:05.000000 orkg-0.9/tests/test_statements.py
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)      354 2020-07-21 08:22:45.000000 orkg-0.9/tests/test_backend.py
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     3026 2020-07-28 10:48:05.000000 orkg-0.9/tests/test_resources.py
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     4047 2020-07-21 08:22:45.000000 orkg-0.9/tests/test_papers.py
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     1037 2021-02-05 11:08:09.000000 orkg-0.9/tests/test_objects.py
--rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)      963 2020-09-30 08:13:25.000000 orkg-0.9/tests/test_contributions.py
+drwxr-xr-x   0 jaradeh   (1000) jaradeh   (1000)        0 2021-02-25 12:12:40.000000 orkg-0.9.2/
+-rwxr-xr-x   0 jaradeh   (1000) jaradeh   (1000)     1315 2021-02-25 12:11:24.000000 orkg-0.9.2/setup.py
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)      524 2020-07-21 09:00:14.000000 orkg-0.9.2/README.md
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     1629 2021-02-25 12:12:40.000000 orkg-0.9.2/PKG-INFO
+drwxr-xr-x   0 jaradeh   (1000) jaradeh   (1000)        0 2021-02-25 12:12:40.000000 orkg-0.9.2/orkg.egg-info/
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     1629 2021-02-25 12:12:40.000000 orkg-0.9.2/orkg.egg-info/PKG-INFO
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)      753 2021-02-25 12:12:40.000000 orkg-0.9.2/orkg.egg-info/SOURCES.txt
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)        1 2021-02-25 12:12:40.000000 orkg-0.9.2/orkg.egg-info/dependency_links.txt
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)       15 2021-02-25 12:12:40.000000 orkg-0.9.2/orkg.egg-info/requires.txt
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)       11 2021-02-25 12:12:40.000000 orkg-0.9.2/orkg.egg-info/top_level.txt
+drwxr-xr-x   0 jaradeh   (1000) jaradeh   (1000)        0 2021-02-25 12:12:40.000000 orkg-0.9.2/orkg/
+drwxr-xr-x   0 jaradeh   (1000) jaradeh   (1000)        0 2021-02-25 12:12:40.000000 orkg-0.9.2/orkg/client/
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     3050 2020-07-21 08:22:45.000000 orkg-0.9.2/orkg/client/classes.py
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)      271 2020-02-21 15:15:29.000000 orkg-0.9.2/orkg/client/stats.py
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)       25 2020-02-21 15:15:29.000000 orkg-0.9.2/orkg/client/__init__.py
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     9184 2020-07-28 10:48:05.000000 orkg-0.9.2/orkg/client/resources.py
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     2603 2020-07-21 08:22:45.000000 orkg-0.9.2/orkg/client/predicates.py
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     3440 2020-09-30 08:30:02.000000 orkg-0.9.2/orkg/client/contributions.py
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     3561 2020-07-28 10:48:05.000000 orkg-0.9.2/orkg/client/statements.py
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     1595 2020-07-21 08:22:45.000000 orkg-0.9.2/orkg/client/literals.py
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)    10460 2021-02-25 12:01:31.000000 orkg-0.9.2/orkg/client/papers.py
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)      663 2021-02-05 11:05:13.000000 orkg-0.9.2/orkg/client/objects.py
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     1810 2020-07-21 08:22:45.000000 orkg-0.9.2/orkg/client/comparisons.py
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     2452 2021-02-05 11:09:53.000000 orkg-0.9.2/orkg/client/backend.py
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)      296 2020-02-21 15:15:29.000000 orkg-0.9.2/orkg/__init__.py
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     2730 2020-07-21 08:22:45.000000 orkg-0.9.2/orkg/utils.py
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)      993 2020-07-21 08:22:45.000000 orkg-0.9.2/orkg/out.py
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)       79 2021-02-25 12:12:40.000000 orkg-0.9.2/setup.cfg
+drwxr-xr-x   0 jaradeh   (1000) jaradeh   (1000)        0 2021-02-25 12:12:40.000000 orkg-0.9.2/tests/
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     1200 2020-02-21 15:15:29.000000 orkg-0.9.2/tests/test_literals.py
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     1966 2020-07-21 08:22:45.000000 orkg-0.9.2/tests/test_predicates.py
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)        0 2020-02-21 15:15:29.000000 orkg-0.9.2/tests/__init__.py
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)      305 2020-02-21 15:15:29.000000 orkg-0.9.2/tests/test_stats.py
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     2236 2020-07-21 08:22:45.000000 orkg-0.9.2/tests/test_classes.py
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     2262 2020-07-28 10:48:05.000000 orkg-0.9.2/tests/test_statements.py
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)      354 2020-07-21 08:22:45.000000 orkg-0.9.2/tests/test_backend.py
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     3026 2020-07-28 10:48:05.000000 orkg-0.9.2/tests/test_resources.py
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     4047 2020-07-21 08:22:45.000000 orkg-0.9.2/tests/test_papers.py
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)     1037 2021-02-05 11:08:09.000000 orkg-0.9.2/tests/test_objects.py
+-rw-r--r--   0 jaradeh   (1000) jaradeh   (1000)      963 2020-09-30 08:13:25.000000 orkg-0.9.2/tests/test_contributions.py
```

### Comparing `orkg-0.9/setup.py` & `orkg-0.9.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 from distutils.core import setup
 
 long_description = open('README.md').read()
 
 setup(
   name='orkg',
   packages=find_packages(),
-  version='0.9',
+  version='0.9.2',
   license='MIT',
   description='Python wrapper for the Open Research Knowledge Graph (ORKG) API',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author='Mohamad Yaser Jaradeh',
   author_email='jaradeh@l3s.de',
   url='http://orkg.org/about',
-  download_url='https://gitlab.com/TIBHannover/orkg/orkg-pypi/-/archive/0.9/orkg-pypi-0.9.tar.gz',
+  download_url='https://gitlab.com/TIBHannover/orkg/orkg-pypi/-/archive/0.9.2/orkg-pypi-0.9.2.tar.gz',
   keywords=['ORKG', 'Scholarly communication', 'API wrapper'],
   install_requires=[
           'hammock',
           'pandas'
       ],
   classifiers=[
-    'Development Status :: 3 - Alpha',
+    'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.2",
     "Programming Language :: Python :: 3.3",
     "Programming Language :: Python :: 3.4",
```

### Comparing `orkg-0.9/README.md` & `orkg-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `orkg-0.9/PKG-INFO` & `orkg-0.9.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: orkg
-Version: 0.9
+Version: 0.9.2
 Summary: Python wrapper for the Open Research Knowledge Graph (ORKG) API
 Home-page: http://orkg.org/about
 Author: Mohamad Yaser Jaradeh
 Author-email: jaradeh@l3s.de
 License: MIT
-Download-URL: https://gitlab.com/TIBHannover/orkg/orkg-pypi/-/archive/0.9/orkg-pypi-0.9.tar.gz
+Download-URL: https://gitlab.com/TIBHannover/orkg/orkg-pypi/-/archive/0.9.2/orkg-pypi-0.9.2.tar.gz
 Description: # orkg-pypi
         [![Documentation Status](https://readthedocs.org/projects/orkg/badge/?version=latest)](https://orkg.readthedocs.io/en/latest/?badge=latest)
         [![PyPI version](https://badge.fury.io/py/orkg.svg)](https://badge.fury.io/py/orkg)
         
         Python package wrapping the ORKG API
         
         The package is a straightforward implementation of the API described in the [documentation](http://tibhannover.gitlab.io/orkg/orkg-backend/api-doc/)
         
         Special thanks to **Allard Oelen** and **Kheir Eddine Farfar** for their contributions to the code.
 Keywords: ORKG,Scholarly communication,API wrapper
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
```

### Comparing `orkg-0.9/orkg.egg-info/PKG-INFO` & `orkg-0.9.2/orkg.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: orkg
-Version: 0.9
+Version: 0.9.2
 Summary: Python wrapper for the Open Research Knowledge Graph (ORKG) API
 Home-page: http://orkg.org/about
 Author: Mohamad Yaser Jaradeh
 Author-email: jaradeh@l3s.de
 License: MIT
-Download-URL: https://gitlab.com/TIBHannover/orkg/orkg-pypi/-/archive/0.9/orkg-pypi-0.9.tar.gz
+Download-URL: https://gitlab.com/TIBHannover/orkg/orkg-pypi/-/archive/0.9.2/orkg-pypi-0.9.2.tar.gz
 Description: # orkg-pypi
         [![Documentation Status](https://readthedocs.org/projects/orkg/badge/?version=latest)](https://orkg.readthedocs.io/en/latest/?badge=latest)
         [![PyPI version](https://badge.fury.io/py/orkg.svg)](https://badge.fury.io/py/orkg)
         
         Python package wrapping the ORKG API
         
         The package is a straightforward implementation of the API described in the [documentation](http://tibhannover.gitlab.io/orkg/orkg-backend/api-doc/)
         
         Special thanks to **Allard Oelen** and **Kheir Eddine Farfar** for their contributions to the code.
 Keywords: ORKG,Scholarly communication,API wrapper
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
```

### Comparing `orkg-0.9/orkg.egg-info/SOURCES.txt` & `orkg-0.9.2/orkg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `orkg-0.9/orkg/client/classes.py` & `orkg-0.9.2/orkg/client/classes.py`

 * *Files identical despite different names*

### Comparing `orkg-0.9/orkg/client/resources.py` & `orkg-0.9.2/orkg/client/resources.py`

 * *Files identical despite different names*

### Comparing `orkg-0.9/orkg/client/predicates.py` & `orkg-0.9.2/orkg/client/predicates.py`

 * *Files identical despite different names*

### Comparing `orkg-0.9/orkg/client/contributions.py` & `orkg-0.9.2/orkg/client/contributions.py`

 * *Files identical despite different names*

### Comparing `orkg-0.9/orkg/client/statements.py` & `orkg-0.9.2/orkg/client/statements.py`

 * *Files identical despite different names*

### Comparing `orkg-0.9/orkg/client/literals.py` & `orkg-0.9.2/orkg/client/literals.py`

 * *Files identical despite different names*

### Comparing `orkg-0.9/orkg/client/papers.py` & `orkg-0.9.2/orkg/client/papers.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 import re
 from ast import literal_eval
 import os
 
 
 class PapersClient(NamespacedClient):
 
-    def add(self, params=None):
+    def add(self, params=None, merge_if_exists=False):
         """
         Create a new paper in the ORKG instance
         :param params: paper Object
+        :param merge_if_exists: merge the papers if they exist in the graph and append contributions
         :return: an OrkgResponse object containing the newly created paper resource
         """
         self.client.backend._append_slash = True
-        response = self.client.backend.papers.POST(json=params, headers=self.auth)
+        response = self.client.backend.papers.POST(json=params, params={'mergeIfExists': merge_if_exists}, headers=self.auth)
         return OrkgResponse(response)
 
     @query_params("file", "standard_statements")
     def add_csv(self, params=None):
         """
         Create a new paper in the ORKG instance
         :param file: csv file containing the papers, with at least a column with title: "paper:title"
```

### Comparing `orkg-0.9/orkg/client/objects.py` & `orkg-0.9.2/orkg/client/objects.py`

 * *Files identical despite different names*

### Comparing `orkg-0.9/orkg/client/comparisons.py` & `orkg-0.9.2/orkg/client/comparisons.py`

 * *Files identical despite different names*

### Comparing `orkg-0.9/orkg/client/backend.py` & `orkg-0.9.2/orkg/client/backend.py`

 * *Files identical despite different names*

### Comparing `orkg-0.9/orkg/utils.py` & `orkg-0.9.2/orkg/utils.py`

 * *Files identical despite different names*

### Comparing `orkg-0.9/orkg/out.py` & `orkg-0.9.2/orkg/out.py`

 * *Files identical despite different names*

### Comparing `orkg-0.9/tests/test_literals.py` & `orkg-0.9.2/tests/test_literals.py`

 * *Files identical despite different names*

### Comparing `orkg-0.9/tests/test_predicates.py` & `orkg-0.9.2/tests/test_predicates.py`

 * *Files identical despite different names*

### Comparing `orkg-0.9/tests/test_classes.py` & `orkg-0.9.2/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `orkg-0.9/tests/test_statements.py` & `orkg-0.9.2/tests/test_statements.py`

 * *Files identical despite different names*

### Comparing `orkg-0.9/tests/test_resources.py` & `orkg-0.9.2/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `orkg-0.9/tests/test_papers.py` & `orkg-0.9.2/tests/test_papers.py`

 * *Files identical despite different names*

### Comparing `orkg-0.9/tests/test_objects.py` & `orkg-0.9.2/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `orkg-0.9/tests/test_contributions.py` & `orkg-0.9.2/tests/test_contributions.py`

 * *Files identical despite different names*

