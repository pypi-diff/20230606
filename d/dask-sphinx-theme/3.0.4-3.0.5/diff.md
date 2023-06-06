# Comparing `tmp/dask_sphinx_theme-3.0.4.tar.gz` & `tmp/dask_sphinx_theme-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dask_sphinx_theme-3.0.4.tar", last modified: Tue May  2 18:43:36 2023, max compression
+gzip compressed data, was "dist/dask_sphinx_theme-3.0.5.tar", last modified: Tue Jun  6 14:41:24 2023, max compression
```

## Comparing `dask_sphinx_theme-3.0.4.tar` & `dask_sphinx_theme-3.0.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/_pygments/
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/_pygments/style.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/ext/
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/ext/dask_config_sphinx_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/images/background-grid.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/images/dask-horizontal-white.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/images/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/images/icon-download.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/images/icon-expand.svg
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/images/icon-menu.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/js/custom.js
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/theme.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 18:43:23.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:41:24.000000 dask_sphinx_theme-3.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-06 14:41:04.000000 dask_sphinx_theme-3.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-06 14:41:04.000000 dask_sphinx_theme-3.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-06 14:41:24.000000 dask_sphinx_theme-3.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-06 14:41:04.000000 dask_sphinx_theme-3.0.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:41:24.000000 dask_sphinx_theme-3.0.5/dask_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-06 14:41:04.000000 dask_sphinx_theme-3.0.5/dask_sphinx_theme/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:41:24.000000 dask_sphinx_theme-3.0.5/dask_sphinx_theme/_pygments/
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-06-06 14:41:04.000000 dask_sphinx_theme-3.0.5/dask_sphinx_theme/_pygments/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-06 14:41:24.000000 dask_sphinx_theme-3.0.5/dask_sphinx_theme/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:41:24.000000 dask_sphinx_theme-3.0.5/dask_sphinx_theme/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-06 14:41:04.000000 dask_sphinx_theme-3.0.5/dask_sphinx_theme/ext/dask_config_sphinx_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-06 14:41:04.000000 dask_sphinx_theme-3.0.5/dask_sphinx_theme/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:41:24.000000 dask_sphinx_theme-3.0.5/dask_sphinx_theme/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:41:24.000000 dask_sphinx_theme-3.0.5/dask_sphinx_theme/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-06-06 14:41:04.000000 dask_sphinx_theme-3.0.5/dask_sphinx_theme/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:41:24.000000 dask_sphinx_theme-3.0.5/dask_sphinx_theme/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-06 14:41:04.000000 dask_sphinx_theme-3.0.5/dask_sphinx_theme/static/images/background-grid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-06-06 14:41:04.000000 dask_sphinx_theme-3.0.5/dask_sphinx_theme/static/images/dask-horizontal-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-06 14:41:04.000000 dask_sphinx_theme-3.0.5/dask_sphinx_theme/static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-06 14:41:04.000000 dask_sphinx_theme-3.0.5/dask_sphinx_theme/static/images/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-06 14:41:04.000000 dask_sphinx_theme-3.0.5/dask_sphinx_theme/static/images/icon-download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-06 14:41:04.000000 dask_sphinx_theme-3.0.5/dask_sphinx_theme/static/images/icon-expand.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-06 14:41:04.000000 dask_sphinx_theme-3.0.5/dask_sphinx_theme/static/images/icon-menu.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:41:24.000000 dask_sphinx_theme-3.0.5/dask_sphinx_theme/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-06 14:41:04.000000 dask_sphinx_theme-3.0.5/dask_sphinx_theme/static/js/custom.js
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-06 14:41:04.000000 dask_sphinx_theme-3.0.5/dask_sphinx_theme/theme.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:41:24.000000 dask_sphinx_theme-3.0.5/dask_sphinx_theme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-06 14:41:24.000000 dask_sphinx_theme-3.0.5/dask_sphinx_theme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-06 14:41:24.000000 dask_sphinx_theme-3.0.5/dask_sphinx_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:41:24.000000 dask_sphinx_theme-3.0.5/dask_sphinx_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-06 14:41:24.000000 dask_sphinx_theme-3.0.5/dask_sphinx_theme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:41:09.000000 dask_sphinx_theme-3.0.5/dask_sphinx_theme.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-06 14:41:24.000000 dask_sphinx_theme-3.0.5/dask_sphinx_theme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 14:41:24.000000 dask_sphinx_theme-3.0.5/dask_sphinx_theme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-06 14:41:04.000000 dask_sphinx_theme-3.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-06 14:41:24.000000 dask_sphinx_theme-3.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-06 14:41:04.000000 dask_sphinx_theme-3.0.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-06-06 14:41:04.000000 dask_sphinx_theme-3.0.5/versioneer.py
```

### Comparing `dask_sphinx_theme-3.0.4/LICENSE.txt` & `dask_sphinx_theme-3.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dask_sphinx_theme-3.0.4/PKG-INFO` & `dask_sphinx_theme-3.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: dask_sphinx_theme
-Version: 3.0.4
+Version: 3.0.5
 Summary: Dask theme for Sphinx
 Home-page: https://github.com/dask/dask-sphinx-theme/
 Author: Dask Developers
 Author-email: UNKNOWN
 License: BSD
 Description: Dask Sphinx Theme
         =================
```

### Comparing `dask_sphinx_theme-3.0.4/README.rst` & `dask_sphinx_theme-3.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `dask_sphinx_theme-3.0.4/dask_sphinx_theme/__init__.py` & `dask_sphinx_theme-3.0.5/dask_sphinx_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_sphinx_theme-3.0.4/dask_sphinx_theme/_pygments/style.py` & `dask_sphinx_theme-3.0.5/dask_sphinx_theme/_pygments/style.py`

 * *Files identical despite different names*

### Comparing `dask_sphinx_theme-3.0.4/dask_sphinx_theme/ext/dask_config_sphinx_ext.py` & `dask_sphinx_theme-3.0.5/dask_sphinx_theme/ext/dask_config_sphinx_ext.py`

 * *Files identical despite different names*

### Comparing `dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/css/style.css` & `dask_sphinx_theme-3.0.5/dask_sphinx_theme/static/css/style.css`

 * *Files identical despite different names*

### Comparing `dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/images/background-grid.svg` & `dask_sphinx_theme-3.0.5/dask_sphinx_theme/static/images/background-grid.svg`

 * *Files identical despite different names*

### Comparing `dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/images/dask-horizontal-white.svg` & `dask_sphinx_theme-3.0.5/dask_sphinx_theme/static/images/dask-horizontal-white.svg`

 * *Files identical despite different names*

### Comparing `dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/images/favicon.ico` & `dask_sphinx_theme-3.0.5/dask_sphinx_theme/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/images/favicon.svg` & `dask_sphinx_theme-3.0.5/dask_sphinx_theme/static/images/favicon.svg`

 * *Files identical despite different names*

### Comparing `dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/images/icon-download.svg` & `dask_sphinx_theme-3.0.5/dask_sphinx_theme/static/images/icon-download.svg`

 * *Files identical despite different names*

### Comparing `dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/images/icon-expand.svg` & `dask_sphinx_theme-3.0.5/dask_sphinx_theme/static/images/icon-expand.svg`

 * *Files identical despite different names*

### Comparing `dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/images/icon-menu.svg` & `dask_sphinx_theme-3.0.5/dask_sphinx_theme/static/images/icon-menu.svg`

 * *Files identical despite different names*

### Comparing `dask_sphinx_theme-3.0.4/dask_sphinx_theme.egg-info/PKG-INFO` & `dask_sphinx_theme-3.0.5/dask_sphinx_theme.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: dask-sphinx-theme
-Version: 3.0.4
+Version: 3.0.5
 Summary: Dask theme for Sphinx
 Home-page: https://github.com/dask/dask-sphinx-theme/
 Author: Dask Developers
 Author-email: UNKNOWN
 License: BSD
 Description: Dask Sphinx Theme
         =================
```

### Comparing `dask_sphinx_theme-3.0.4/dask_sphinx_theme.egg-info/SOURCES.txt` & `dask_sphinx_theme-3.0.5/dask_sphinx_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dask_sphinx_theme-3.0.4/setup.py` & `dask_sphinx_theme-3.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `dask_sphinx_theme-3.0.4/versioneer.py` & `dask_sphinx_theme-3.0.5/versioneer.py`

 * *Files identical despite different names*

