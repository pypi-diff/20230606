# Comparing `tmp/openedx_webhooks-0.2.0.tar.gz` & `tmp/openedx_webhooks-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/andres/Workspace/site-local-dev/env/build/openedx/requirements/openedx-webhooks/dist/.tmp-yo0yikbd/openedx_webhooks-0.2.", last modified: Tue Jun  6 15:32:35 2023, max compression
+gzip compressed data, was "/Users/andres/Workspace/site-local-dev/env/build/openedx/requirements/openedx-webhooks/dist/.tmp-h88e0w5s/openedx_webhooks-0.2.", last modified: Tue Jun  6 16:33:55 2023, max compression
```

## Comparing `openedx_webhooks-0.2.0.tar` & `openedx_webhooks-0.2.1.tar`

### file list

```diff
@@ -1,32 +1,37 @@
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-06-06 15:32:35.171014 openedx_webhooks-0.2.0/
--rw-r--r--   0 andres     (501) staff       (20)      361 2023-06-06 15:31:37.000000 openedx_webhooks-0.2.0/CHANGELOG.rst
--rw-r--r--   0 andres     (501) staff       (20)    35139 2023-05-31 15:48:08.000000 openedx_webhooks-0.2.0/LICENSE.txt
--rw-r--r--   0 andres     (501) staff       (20)      211 2023-06-06 15:00:55.000000 openedx_webhooks-0.2.0/MANIFEST.in
--rw-r--r--   0 andres     (501) staff       (20)     7125 2023-06-06 15:32:35.171233 openedx_webhooks-0.2.0/PKG-INFO
--rw-r--r--   0 andres     (501) staff       (20)     6096 2023-06-06 15:00:55.000000 openedx_webhooks-0.2.0/README.rst
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-06-06 15:32:35.166289 openedx_webhooks-0.2.0/openedx_webhooks/
--rw-r--r--   0 andres     (501) staff       (20)      147 2023-06-06 15:31:37.000000 openedx_webhooks-0.2.0/openedx_webhooks/__init__.py
--rw-r--r--   0 andres     (501) staff       (20)      524 2023-06-06 15:00:55.000000 openedx_webhooks-0.2.0/openedx_webhooks/admin.py
--rw-r--r--   0 andres     (501) staff       (20)     1391 2023-06-06 15:00:55.000000 openedx_webhooks-0.2.0/openedx_webhooks/apps.py
--rw-r--r--   0 andres     (501) staff       (20)     1673 2023-06-06 15:00:55.000000 openedx_webhooks-0.2.0/openedx_webhooks/models.py
--rw-r--r--   0 andres     (501) staff       (20)     5512 2023-06-06 15:00:55.000000 openedx_webhooks-0.2.0/openedx_webhooks/receivers.py
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-06-06 15:32:35.158543 openedx_webhooks-0.2.0/openedx_webhooks/templates/
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-06-06 15:32:35.169436 openedx_webhooks-0.2.0/openedx_webhooks/templates/webhooks/
--rw-r--r--   0 andres     (501) staff       (20)      662 2023-06-06 15:00:55.000000 openedx_webhooks-0.2.0/openedx_webhooks/templates/webhooks/base.html
--rw-r--r--   0 andres     (501) staff       (20)      325 2023-06-06 15:00:55.000000 openedx_webhooks-0.2.0/openedx_webhooks/urls.py
--rw-r--r--   0 andres     (501) staff       (20)      947 2023-06-06 15:00:55.000000 openedx_webhooks-0.2.0/openedx_webhooks/utils.py
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-06-06 15:32:35.169133 openedx_webhooks-0.2.0/openedx_webhooks.egg-info/
--rw-r--r--   0 andres     (501) staff       (20)     7125 2023-06-06 15:32:35.000000 openedx_webhooks-0.2.0/openedx_webhooks.egg-info/PKG-INFO
--rw-r--r--   0 andres     (501) staff       (20)      653 2023-06-06 15:32:35.000000 openedx_webhooks-0.2.0/openedx_webhooks.egg-info/SOURCES.txt
--rw-r--r--   0 andres     (501) staff       (20)        1 2023-06-06 15:32:35.000000 openedx_webhooks-0.2.0/openedx_webhooks.egg-info/dependency_links.txt
--rw-r--r--   0 andres     (501) staff       (20)       64 2023-06-06 15:32:35.000000 openedx_webhooks-0.2.0/openedx_webhooks.egg-info/entry_points.txt
--rw-r--r--   0 andres     (501) staff       (20)        1 2023-06-06 14:48:45.000000 openedx_webhooks-0.2.0/openedx_webhooks.egg-info/not-zip-safe
--rw-r--r--   0 andres     (501) staff       (20)       74 2023-06-06 15:32:35.000000 openedx_webhooks-0.2.0/openedx_webhooks.egg-info/requires.txt
--rw-r--r--   0 andres     (501) staff       (20)       17 2023-06-06 15:32:35.000000 openedx_webhooks-0.2.0/openedx_webhooks.egg-info/top_level.txt
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-06-06 15:32:35.170241 openedx_webhooks-0.2.0/requirements/
--rw-r--r--   0 andres     (501) staff       (20)      373 2023-06-02 18:52:16.000000 openedx_webhooks-0.2.0/requirements/base.in
--rw-r--r--   0 andres     (501) staff       (20)      561 2023-05-31 15:48:07.000000 openedx_webhooks-0.2.0/requirements/constraints.txt
--rw-r--r--   0 andres     (501) staff       (20)      176 2023-06-06 15:32:35.171860 openedx_webhooks-0.2.0/setup.cfg
--rwxr-xr-x   0 andres     (501) staff       (20)     5170 2023-06-06 15:00:55.000000 openedx_webhooks-0.2.0/setup.py
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-06-06 15:32:35.170573 openedx_webhooks-0.2.0/tests/
--rw-r--r--   0 andres     (501) staff       (20)      221 2023-06-06 15:00:55.000000 openedx_webhooks-0.2.0/tests/test_models.py
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-06-06 16:33:55.039716 openedx_webhooks-0.2.1/
+-rw-r--r--   0 andres     (501) staff       (20)      361 2023-06-06 16:33:30.000000 openedx_webhooks-0.2.1/CHANGELOG.rst
+-rw-r--r--   0 andres     (501) staff       (20)    35139 2023-05-31 15:48:08.000000 openedx_webhooks-0.2.1/LICENSE.txt
+-rw-r--r--   0 andres     (501) staff       (20)      211 2023-06-06 15:00:55.000000 openedx_webhooks-0.2.1/MANIFEST.in
+-rw-r--r--   0 andres     (501) staff       (20)     7125 2023-06-06 16:33:55.039873 openedx_webhooks-0.2.1/PKG-INFO
+-rw-r--r--   0 andres     (501) staff       (20)     6096 2023-06-06 15:00:55.000000 openedx_webhooks-0.2.1/README.rst
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-06-06 16:33:55.033131 openedx_webhooks-0.2.1/openedx_webhooks/
+-rw-r--r--   0 andres     (501) staff       (20)      147 2023-06-06 16:33:30.000000 openedx_webhooks-0.2.1/openedx_webhooks/__init__.py
+-rw-r--r--   0 andres     (501) staff       (20)      524 2023-06-06 15:00:55.000000 openedx_webhooks-0.2.1/openedx_webhooks/admin.py
+-rw-r--r--   0 andres     (501) staff       (20)     1391 2023-06-06 16:33:19.000000 openedx_webhooks-0.2.1/openedx_webhooks/apps.py
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-06-06 16:33:55.036986 openedx_webhooks-0.2.1/openedx_webhooks/migrations/
+-rw-r--r--   0 andres     (501) staff       (20)     1737 2023-06-06 15:00:55.000000 openedx_webhooks-0.2.1/openedx_webhooks/migrations/0001_initial.py
+-rw-r--r--   0 andres     (501) staff       (20)        0 2023-06-06 15:00:55.000000 openedx_webhooks-0.2.1/openedx_webhooks/migrations/__init__.py
+-rw-r--r--   0 andres     (501) staff       (20)     1673 2023-06-06 15:00:55.000000 openedx_webhooks-0.2.1/openedx_webhooks/models.py
+-rw-r--r--   0 andres     (501) staff       (20)     5512 2023-06-06 15:00:55.000000 openedx_webhooks-0.2.1/openedx_webhooks/receivers.py
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-06-06 16:33:55.023825 openedx_webhooks-0.2.1/openedx_webhooks/templates/
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-06-06 16:33:55.037266 openedx_webhooks-0.2.1/openedx_webhooks/templates/webhooks/
+-rw-r--r--   0 andres     (501) staff       (20)      662 2023-06-06 15:00:55.000000 openedx_webhooks-0.2.1/openedx_webhooks/templates/webhooks/base.html
+-rw-r--r--   0 andres     (501) staff       (20)      325 2023-06-06 15:00:55.000000 openedx_webhooks-0.2.1/openedx_webhooks/urls.py
+-rw-r--r--   0 andres     (501) staff       (20)      947 2023-06-06 15:00:55.000000 openedx_webhooks-0.2.1/openedx_webhooks/utils.py
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-06-06 16:33:55.036159 openedx_webhooks-0.2.1/openedx_webhooks.egg-info/
+-rw-r--r--   0 andres     (501) staff       (20)     7125 2023-06-06 16:33:55.000000 openedx_webhooks-0.2.1/openedx_webhooks.egg-info/PKG-INFO
+-rw-r--r--   0 andres     (501) staff       (20)      760 2023-06-06 16:33:55.000000 openedx_webhooks-0.2.1/openedx_webhooks.egg-info/SOURCES.txt
+-rw-r--r--   0 andres     (501) staff       (20)        1 2023-06-06 16:33:55.000000 openedx_webhooks-0.2.1/openedx_webhooks.egg-info/dependency_links.txt
+-rw-r--r--   0 andres     (501) staff       (20)       64 2023-06-06 16:33:55.000000 openedx_webhooks-0.2.1/openedx_webhooks.egg-info/entry_points.txt
+-rw-r--r--   0 andres     (501) staff       (20)        1 2023-06-06 16:28:42.000000 openedx_webhooks-0.2.1/openedx_webhooks.egg-info/not-zip-safe
+-rw-r--r--   0 andres     (501) staff       (20)       74 2023-06-06 16:33:55.000000 openedx_webhooks-0.2.1/openedx_webhooks.egg-info/requires.txt
+-rw-r--r--   0 andres     (501) staff       (20)       28 2023-06-06 16:33:55.000000 openedx_webhooks-0.2.1/openedx_webhooks.egg-info/top_level.txt
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-06-06 16:33:55.038130 openedx_webhooks-0.2.1/requirements/
+-rw-r--r--   0 andres     (501) staff       (20)      373 2023-06-02 18:52:16.000000 openedx_webhooks-0.2.1/requirements/base.in
+-rw-r--r--   0 andres     (501) staff       (20)      561 2023-05-31 15:48:07.000000 openedx_webhooks-0.2.1/requirements/constraints.txt
+-rw-r--r--   0 andres     (501) staff       (20)      176 2023-06-06 16:33:55.040431 openedx_webhooks-0.2.1/setup.cfg
+-rwxr-xr-x   0 andres     (501) staff       (20)     5132 2023-06-06 16:29:43.000000 openedx_webhooks-0.2.1/setup.py
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-06-06 16:33:55.038459 openedx_webhooks-0.2.1/test_utils/
+-rw-r--r--   0 andres     (501) staff       (20)      341 2023-05-31 15:48:08.000000 openedx_webhooks-0.2.1/test_utils/__init__.py
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-06-06 16:33:55.039172 openedx_webhooks-0.2.1/tests/
+-rw-r--r--   0 andres     (501) staff       (20)      221 2023-06-06 15:00:55.000000 openedx_webhooks-0.2.1/tests/test_models.py
```

### Comparing `openedx_webhooks-0.2.0/LICENSE.txt` & `openedx_webhooks-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openedx_webhooks-0.2.0/PKG-INFO` & `openedx_webhooks-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx_webhooks
-Version: 0.2.0
+Version: 0.2.1
 Summary: Webhooks for Open edX
 Home-page: https://github.com/openedx/openedx-webhooks
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -219,15 +219,15 @@
 .. .. |status-badge| image:: https://img.shields.io/badge/Status-Deprecated-orange
 .. .. |status-badge| image:: https://img.shields.io/badge/Status-Unsupported-red
 
 
 Change Log
 ##########
 
-Version 0.2.0 (2023-06-06)
+Version 0.2.1 (2023-06-06)
 **********************************************
 
 * Renamed package to openedx_webhooks. Upload to PyPI.
 
 Version 0.1.1 (2023-06-05)
 **********************************************
```

### Comparing `openedx_webhooks-0.2.0/README.rst` & `openedx_webhooks-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `openedx_webhooks-0.2.0/openedx_webhooks/admin.py` & `openedx_webhooks-0.2.1/openedx_webhooks/admin.py`

 * *Files identical despite different names*

### Comparing `openedx_webhooks-0.2.0/openedx_webhooks/apps.py` & `openedx_webhooks-0.2.1/openedx_webhooks/apps.py`

 * *Files identical despite different names*

### Comparing `openedx_webhooks-0.2.0/openedx_webhooks/models.py` & `openedx_webhooks-0.2.1/openedx_webhooks/models.py`

 * *Files identical despite different names*

### Comparing `openedx_webhooks-0.2.0/openedx_webhooks/receivers.py` & `openedx_webhooks-0.2.1/openedx_webhooks/receivers.py`

 * *Files identical despite different names*

### Comparing `openedx_webhooks-0.2.0/openedx_webhooks/templates/webhooks/base.html` & `openedx_webhooks-0.2.1/openedx_webhooks/templates/webhooks/base.html`

 * *Files identical despite different names*

### Comparing `openedx_webhooks-0.2.0/openedx_webhooks/utils.py` & `openedx_webhooks-0.2.1/openedx_webhooks/utils.py`

 * *Files identical despite different names*

### Comparing `openedx_webhooks-0.2.0/openedx_webhooks.egg-info/PKG-INFO` & `openedx_webhooks-0.2.1/openedx_webhooks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-webhooks
-Version: 0.2.0
+Version: 0.2.1
 Summary: Webhooks for Open edX
 Home-page: https://github.com/openedx/openedx-webhooks
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -219,15 +219,15 @@
 .. .. |status-badge| image:: https://img.shields.io/badge/Status-Deprecated-orange
 .. .. |status-badge| image:: https://img.shields.io/badge/Status-Unsupported-red
 
 
 Change Log
 ##########
 
-Version 0.2.0 (2023-06-06)
+Version 0.2.1 (2023-06-06)
 **********************************************
 
 * Renamed package to openedx_webhooks. Upload to PyPI.
 
 Version 0.1.1 (2023-06-05)
 **********************************************
```

### Comparing `openedx_webhooks-0.2.0/openedx_webhooks.egg-info/SOURCES.txt` & `openedx_webhooks-0.2.1/openedx_webhooks.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -14,11 +14,14 @@
 openedx_webhooks.egg-info/PKG-INFO
 openedx_webhooks.egg-info/SOURCES.txt
 openedx_webhooks.egg-info/dependency_links.txt
 openedx_webhooks.egg-info/entry_points.txt
 openedx_webhooks.egg-info/not-zip-safe
 openedx_webhooks.egg-info/requires.txt
 openedx_webhooks.egg-info/top_level.txt
+openedx_webhooks/migrations/0001_initial.py
+openedx_webhooks/migrations/__init__.py
 openedx_webhooks/templates/webhooks/base.html
 requirements/base.in
 requirements/constraints.txt
+test_utils/__init__.py
 tests/test_models.py
```

### Comparing `openedx_webhooks-0.2.0/requirements/constraints.txt` & `openedx_webhooks-0.2.1/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `openedx_webhooks-0.2.0/setup.py` & `openedx_webhooks-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,14 @@
     version=VERSION,
     description="""Webhooks for Open edX""",
     long_description=README + '\n\n' + CHANGELOG,
     author='edX',
     author_email='oscm@edx.org',
     url='https://github.com/openedx/openedx-webhooks',
     packages=find_packages(
-        include=['openedx_webhooks'],
         exclude=["*tests"],
     ),
 
     include_package_data=True,
     install_requires=load_requirements('requirements/base.in'),
     python_requires=">=3.8",
     license="AGPL 3.0",
```

