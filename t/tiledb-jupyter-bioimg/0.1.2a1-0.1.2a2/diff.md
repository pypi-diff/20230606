# Comparing `tmp/tiledb_jupyter_bioimg-0.1.2a1.tar.gz` & `tmp/tiledb_jupyter_bioimg-0.1.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiledb_jupyter_bioimg-0.1.2a1.tar", last modified: Fri Jun  2 13:54:32 2023, max compression
+gzip compressed data, was "tiledb_jupyter_bioimg-0.1.2a2.tar", last modified: Tue Jun  6 08:08:47 2023, max compression
```

## Comparing `tiledb_jupyter_bioimg-0.1.2a1.tar` & `tiledb_jupyter_bioimg-0.1.2a2.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:54:32.013759 tiledb_jupyter_bioimg-0.1.2a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-02 13:50:47.000000 tiledb_jupyter_bioimg-0.1.2a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-02 13:50:47.000000 tiledb_jupyter_bioimg-0.1.2a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-02 13:54:32.013759 tiledb_jupyter_bioimg-0.1.2a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-02 13:50:47.000000 tiledb_jupyter_bioimg-0.1.2a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-02 13:50:47.000000 tiledb_jupyter_bioimg-0.1.2a1/install.json
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-02 13:52:35.000000 tiledb_jupyter_bioimg-0.1.2a1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-02 13:50:47.000000 tiledb_jupyter_bioimg-0.1.2a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 13:54:32.013759 tiledb_jupyter_bioimg-0.1.2a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-06-02 13:50:47.000000 tiledb_jupyter_bioimg-0.1.2a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:54:32.009759 tiledb_jupyter_bioimg-0.1.2a1/src/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-02 13:50:47.000000 tiledb_jupyter_bioimg-0.1.2a1/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-02 13:50:47.000000 tiledb_jupyter_bioimg-0.1.2a1/src/version.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-02 13:50:47.000000 tiledb_jupyter_bioimg-0.1.2a1/src/widget.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:54:32.009759 tiledb_jupyter_bioimg-0.1.2a1/style/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 13:50:47.000000 tiledb_jupyter_bioimg-0.1.2a1/style/base.css
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-02 13:50:47.000000 tiledb_jupyter_bioimg-0.1.2a1/style/index.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-02 13:50:47.000000 tiledb_jupyter_bioimg-0.1.2a1/style/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:54:32.009759 tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-02 13:50:47.000000 tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-02 13:50:47.000000 tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-02 13:50:47.000000 tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:54:32.013759 tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-06-02 13:54:31.000000 tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:54:32.013759 tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)   189298 2023-06-02 13:54:31.000000 tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6875 2023-06-02 13:54:31.000000 tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/labextension/static/408.635d4bfc76ee689544e0.js
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-02 13:54:31.000000 tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
--rw-r--r--   0 runner    (1001) docker     (123)   516688 2023-06-02 13:54:31.000000 tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/labextension/static/635.b2bedc962bcd82714540.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-02 13:54:31.000000 tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/labextension/static/635.b2bedc962bcd82714540.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-06-02 13:54:31.000000 tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/labextension/static/744.23211eab87ca12d5bb82.js
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-02 13:54:31.000000 tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js
--rw-r--r--   0 runner    (1001) docker     (123)   754522 2023-06-02 13:54:31.000000 tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/labextension/static/774.a940595120cb008c0c58.js
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-02 13:54:31.000000 tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/labextension/static/774.a940595120cb008c0c58.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-06-02 13:54:31.000000 tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/labextension/static/remoteEntry.555c16a49a97a15a2937.js
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-02 13:54:09.000000 tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)    85217 2023-06-02 13:54:31.000000 tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-02 13:50:47.000000 tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:54:32.013759 tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-02 13:54:31.000000 tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-02 13:54:32.000000 tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 13:54:31.000000 tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 13:53:31.000000 tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-02 13:54:31.000000 tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 13:54:31.000000 tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-02 13:50:47.000000 tiledb_jupyter_bioimg-0.1.2a1/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:08:47.356563 tiledb_jupyter_bioimg-0.1.2a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-06 08:03:32.000000 tiledb_jupyter_bioimg-0.1.2a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-06 08:03:32.000000 tiledb_jupyter_bioimg-0.1.2a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-06 08:08:47.356563 tiledb_jupyter_bioimg-0.1.2a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-06 08:03:32.000000 tiledb_jupyter_bioimg-0.1.2a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-06 08:03:32.000000 tiledb_jupyter_bioimg-0.1.2a2/install.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-06 08:06:03.000000 tiledb_jupyter_bioimg-0.1.2a2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-06 08:03:32.000000 tiledb_jupyter_bioimg-0.1.2a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 08:08:47.356563 tiledb_jupyter_bioimg-0.1.2a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-06 08:03:32.000000 tiledb_jupyter_bioimg-0.1.2a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:08:47.344562 tiledb_jupyter_bioimg-0.1.2a2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-06 08:03:32.000000 tiledb_jupyter_bioimg-0.1.2a2/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-06 08:03:32.000000 tiledb_jupyter_bioimg-0.1.2a2/src/version.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-06 08:03:32.000000 tiledb_jupyter_bioimg-0.1.2a2/src/widget.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:08:47.344562 tiledb_jupyter_bioimg-0.1.2a2/style/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 08:03:32.000000 tiledb_jupyter_bioimg-0.1.2a2/style/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-06 08:03:32.000000 tiledb_jupyter_bioimg-0.1.2a2/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-06 08:03:32.000000 tiledb_jupyter_bioimg-0.1.2a2/style/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:08:47.348562 tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-06 08:03:32.000000 tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-06 08:03:32.000000 tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-06 08:03:32.000000 tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:08:47.348562 tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-06 08:08:45.000000 tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:08:47.356563 tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   189298 2023-06-06 08:08:45.000000 tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14610 2023-06-06 08:08:45.000000 tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/labextension/static/172.6267f3dd3063477e34ed.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6875 2023-06-06 08:08:45.000000 tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/labextension/static/408.bdb74ff9f40e9eef1c08.js
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-06 08:08:45.000000 tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
+-rw-r--r--   0 runner    (1001) docker     (123)   516688 2023-06-06 08:08:45.000000 tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/labextension/static/635.f8f404497739316e801c.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-06 08:08:45.000000 tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/labextension/static/635.f8f404497739316e801c.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   172313 2023-06-06 08:08:45.000000 tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-06 08:08:45.000000 tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-06-06 08:08:45.000000 tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/labextension/static/744.6ac09e98bdf01bd3b6d1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-06 08:08:45.000000 tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js
+-rw-r--r--   0 runner    (1001) docker     (123)   740256 2023-06-06 08:08:45.000000 tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/labextension/static/774.309d750794b6276f460a.js
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-06 08:08:45.000000 tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/labextension/static/774.309d750794b6276f460a.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-06-06 08:08:45.000000 tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/labextension/static/remoteEntry.b197e4666f084e8dece0.js
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-06 08:08:13.000000 tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)    90779 2023-06-06 08:08:45.000000 tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-06 08:03:32.000000 tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:08:47.348562 tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-06 08:08:47.000000 tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-06 08:08:47.000000 tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 08:08:47.000000 tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 08:07:20.000000 tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-06 08:08:47.000000 tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-06 08:08:47.000000 tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-06 08:03:32.000000 tiledb_jupyter_bioimg-0.1.2a2/tsconfig.json
```

### Comparing `tiledb_jupyter_bioimg-0.1.2a1/LICENSE` & `tiledb_jupyter_bioimg-0.1.2a2/LICENSE`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.2a1/PKG-INFO` & `tiledb_jupyter_bioimg-0.1.2a2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledb_jupyter_bioimg
-Version: 0.1.2a1
+Version: 0.1.2a2
 Summary: A jupyterlab extension to visualize bioimages in TileDB format
 Home-page: https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer
 Author: TileDB
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
@@ -85,14 +85,10 @@
 
 ### Usage
 
 ```python
 
 from tiledb_jupyter_bioimg import Render
 
-Render("<<NAMESPACE>>", "<<GROUP_ID>>")
+Render("<<NAMESPACE>>", "<<GROUP_ID>>", {"token": "<<TILEDB_API_TOKEN>>>"})
 
 ```
-
-### Common issues
-
-If you get error `Uncaught (in promise) Error: No provider for: jupyter.extensions.jupyterWidgetRegistry.` please make sure you are using correct version of `ipywidgets` (v8).
```

### Comparing `tiledb_jupyter_bioimg-0.1.2a1/README.md` & `tiledb_jupyter_bioimg-0.1.2a2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -63,14 +63,10 @@
 
 ### Usage
 
 ```python
 
 from tiledb_jupyter_bioimg import Render
 
-Render("<<NAMESPACE>>", "<<GROUP_ID>>")
+Render("<<NAMESPACE>>", "<<GROUP_ID>>", {"token": "<<TILEDB_API_TOKEN>>>"})
 
 ```
-
-### Common issues
-
-If you get error `Uncaught (in promise) Error: No provider for: jupyter.extensions.jupyterWidgetRegistry.` please make sure you are using correct version of `ipywidgets` (v8).
```

### Comparing `tiledb_jupyter_bioimg-0.1.2a1/package.json` & `tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/labextension/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9566666666666668%*

 * *Differences: {"'dependencies'": "{'@jupyter-widgets/base': '^1.1.10 || ^2 || ^3 || ^4', "*

 * *                   "'@tiledb-inc/bioimage-viewer': '^0.1.1-beta.0'}",*

 * * "'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.b197e4666f084e8dece0.js'), "*

 * *                 "('extension', './extension'), ('style', './style')]), delete: "*

 * *                 "['sharedPackages']}",*

 * * "'version'": "'0.1.2-alpha.2'"}*

```diff
@@ -1,16 +1,16 @@
 {
     "author": "TileDB",
     "bugs": {
         "url": "https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"
     },
     "dependencies": {
-        "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^5 || ^6",
+        "@jupyter-widgets/base": "^1.1.10 || ^2 || ^3 || ^4",
         "@jupyterlab/application": "^3.4.5",
-        "@tiledb-inc/bioimage-viewer": "^0.1.0-alpha.7"
+        "@tiledb-inc/bioimage-viewer": "^0.1.1-beta.0"
     },
     "description": "A jupyterlab extension to visualize bioimages in TileDB format",
     "devDependencies": {
         "@jupyterlab/builder": "^3.1.0",
         "@typescript-eslint/eslint-plugin": "^2.27.0",
         "@typescript-eslint/parser": "^2.27.0",
         "eslint": "^7.5.0",
@@ -25,22 +25,21 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.b197e4666f084e8dece0.js",
+            "style": "./style"
+        },
         "extension": "lib/index",
         "outputDir": "tiledb_jupyter_bioimg/labextension",
-        "sharedPackages": {
-            "@jupyter-widgets/base": {
-                "bundled": false,
-                "singleton": true
-            }
-        },
         "webpackConfig": "./webpack.config.js"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
@@ -93,9 +92,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.2-alpha.1"
+    "version": "0.1.2-alpha.2"
 }
```

### Comparing `tiledb_jupyter_bioimg-0.1.2a1/setup.py` & `tiledb_jupyter_bioimg-0.1.2a2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     author="TileDB",
     description="A jupyterlab extension to visualize bioimages in TileDB format",
     long_description= long_description,
     long_description_content_type="text/markdown",
     cmdclass= cmdclass,
     packages=setuptools.find_packages(),
     install_requires=[
-        "ipywidgets>=7,<9",
+        "ipywidgets>=7.0.0",
         "jupyterlab>=3.0.0rc13,==3.*",
     ],
     zip_safe=False,
     include_package_data=True,
     python_requires=">=3.6",
     license="BSD-3-Clause",
     platforms="Linux, Mac OS X, Windows",
```

### Comparing `tiledb_jupyter_bioimg-0.1.2a1/src/index.ts` & `tiledb_jupyter_bioimg-0.1.2a2/src/index.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.2a1/src/version.ts` & `tiledb_jupyter_bioimg-0.1.2a2/src/version.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.2a1/src/widget.ts` & `tiledb_jupyter_bioimg-0.1.2a2/src/widget.ts`

 * *Files 9% similar despite different names*

```diff
@@ -31,22 +31,32 @@
     };
   }
 
   static model_name = 'BioImageViewerModel';
   static view_name = 'BioImageViewerView';
 }
 
+interface IValues {
+  basePath?: string;
+  baseGroup?: string;
+  token: string;
+  groupID: string;
+  namespace: string;
+}
+
 export class BioImageViewerView extends DOMWidgetView {
-  values = this.model.get('value');
+  values: IValues = this.model.get('value');
 
   render(): void {
     const wrapper = document.createElement('div');
     this.el.appendChild(wrapper);
 
     createViewer({
       rootElement: wrapper,
       apiKey: this.values.token,
       groupID: this.values.groupID,
+      basePath: this.values.basePath,
+      baseGroup: this.values.baseGroup,
       namespace: this.values.namespace
     });
   }
 }
```

### Comparing `tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/_version.py` & `tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/_version.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/labextension/package.json` & `tiledb_jupyter_bioimg-0.1.2a2/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9566666666666668%*

 * *Differences: {"'dependencies'": "{'@jupyter-widgets/base': '^1.1.10 || ^2 || ^3 || ^4', "*

 * *                   "'@tiledb-inc/bioimage-viewer': '^0.1.1-beta.0'}",*

 * * "'jupyterlab'": "{delete: ['sharedPackages', '_build']}",*

 * * "'version'": "'0.1.2-alpha.2'"}*

```diff
@@ -1,16 +1,16 @@
 {
     "author": "TileDB",
     "bugs": {
         "url": "https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"
     },
     "dependencies": {
-        "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^5 || ^6",
+        "@jupyter-widgets/base": "^1.1.10 || ^2 || ^3 || ^4",
         "@jupyterlab/application": "^3.4.5",
-        "@tiledb-inc/bioimage-viewer": "^0.1.0-alpha.7"
+        "@tiledb-inc/bioimage-viewer": "^0.1.1-beta.0"
     },
     "description": "A jupyterlab extension to visualize bioimages in TileDB format",
     "devDependencies": {
         "@jupyterlab/builder": "^3.1.0",
         "@typescript-eslint/eslint-plugin": "^2.27.0",
         "@typescript-eslint/parser": "^2.27.0",
         "eslint": "^7.5.0",
@@ -25,27 +25,16 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.555c16a49a97a15a2937.js",
-            "style": "./style"
-        },
         "extension": "lib/index",
         "outputDir": "tiledb_jupyter_bioimg/labextension",
-        "sharedPackages": {
-            "@jupyter-widgets/base": {
-                "bundled": false,
-                "singleton": true
-            }
-        },
         "webpackConfig": "./webpack.config.js"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
@@ -98,9 +87,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.2-alpha.1"
+    "version": "0.1.2-alpha.2"
 }
```

### Comparing `tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg` & `tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/labextension/static/408.635d4bfc76ee689544e0.js` & `tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/labextension/static/408.bdb74ff9f40e9eef1c08.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -81,19 +81,19 @@
                         n = e.data.levelRecord.dimensions[e.data.levelRecord.axes.indexOf("X")],
                         s = e.data.levelRecord.dimensions[e.data.levelRecord.axes.indexOf("Y")],
                         h = e.data.levelRecord.downsample,
                         g = e.data.index.x,
                         p = e.data.index.y,
                         d = e.data.tileSize,
                         x = e.data.attribute.type.toLowerCase(),
-                        y = e.data.levelRecord.axesMapping,
-                        b = new i(e.data.levelRecord.arrayAxes.map((t => e.data.levelRecord.axesMapping.get(t))).flat(), ["C", "Y", "X"]),
-                        v = new Array(b.baseAxes.length);
-                    for (let e = 0; e < b.baseAxes.length; ++e) {
-                        const t = b.baseAxes[e];
+                        b = e.data.levelRecord.axesMapping,
+                        y = new i(e.data.levelRecord.arrayAxes.map((t => e.data.levelRecord.axesMapping.get(t))).flat(), ["C", "Y", "X"]),
+                        v = new Array(y.baseAxes.length);
+                    for (let e = 0; e < y.baseAxes.length; ++e) {
+                        const t = y.baseAxes[e];
                         v[e] = "X" === t || "Y" === t ? h : 1
                     }
                     const m = new Map;
                     m.set("C", e.data.channelRanges), m.set("Y", [p * d * h, Math.min((p + 1) * d * h, s) - 1]), m.set("X", [g * d * h, Math.min((g + 1) * d * h, n) - 1]);
                     const A = ~~((m.get("X")[1] - m.get("X")[0] + 1) / h),
                         w = ~~((m.get("Y")[1] - m.get("Y")[0] + 1) / h);
                     let E = 0;
@@ -117,44 +117,44 @@
                                         n = a.get(e);
                                     for (let e = 0; e < n.length; e += 2) t.push(n[e + 1] - n[e] + 1), r.push(n[e]);
                                     h.push(t), g.push(r)
                                 }
                                 const p = f(...h),
                                     d = f(...g),
                                     x = [],
-                                    y = [];
+                                    b = [];
                                 for (const e of d) {
                                     let t = 0;
                                     for (let r = 0; r < e.length; ++r) t += e[r] * c[r];
                                     x.push(t)
                                 }
                                 for (const e of p) {
                                     const t = new Array(i.length + 1).fill(Number.MAX_SAFE_INTEGER, 0, 1).fill(1, 1);
                                     for (let r = 0; r < e.length; ++r)
                                         for (let n = r + 1; n < e.length; ++n) t[r + 1] *= e[n];
-                                    y.push(t)
+                                    b.push(t)
                                 }
-                                let b = 0;
+                                let y = 0;
                                 const v = new Array(i.length),
                                     m = [],
                                     A = o[r.indexOf(l)];
                                 for (let e = 0; e < p.length; ++e) {
                                     const t = p[e].reduce(((e, t) => e * t), 1);
                                     for (let r = 0; r < t; ++r) {
-                                        b = x[e];
-                                        for (let t = 0; t < y[e].length - 1; ++t) v[t] = ~~(r % y[e][t] / y[e][t + 1]), b += v[t] * c[t];
-                                        if (b >= A) return console.error("OOB"), [];
-                                        m.push(b)
+                                        y = x[e];
+                                        for (let t = 0; t < b[e].length - 1; ++t) v[t] = ~~(r % b[e][t] / b[e][t + 1]), y += v[t] * c[t];
+                                        if (y >= A) return console.error("OOB"), [];
+                                        m.push(y)
                                     }
                                 }
                                 m.sort(((e, t) => e - t)), s.push(u(m))
                             }
                         }
                         return s
-                    }(e.data.levelRecord.dimensions, e.data.levelRecord.axes, e.data.levelRecord.arrayAxes, y, m, e.data.levelRecord.arrayExtends);
+                    }(e.data.levelRecord.dimensions, e.data.levelRecord.axes, e.data.levelRecord.arrayAxes, b, m, e.data.levelRecord.arrayExtends);
                     if (0 === R.length) return;
                     const S = {
                             layout: o.Layout.RowMajor,
                             ranges: R,
                             bufferSize: 7e7,
                             attributes: [e.data.attribute.name],
                             returnRawBuffers: !0
@@ -187,15 +187,15 @@
                             h = new Array(t.baseAxes.length);
                         for (let r = 0; r < e.length; ++r) {
                             f = 0;
                             for (let e = 0; e < i.length - 1; ++e) h[e] = ~~(r % i[e] / i[e + 1]), f += ~~(h[e] / o[t.permutationMatrix[e]]) * c[t.permutationMatrix[e]];
                             l[f] += e[r] / u
                         }
                         return l
-                    }(O, b, M, v);
+                    }(O, y, M, v);
                     self.postMessage({
                         data: T,
                         width: A,
                         height: w,
                         channels: E
                     }, [T.buffer])
                 }
@@ -238,15 +238,15 @@
             a: t
         }), t
     }, a.d = (e, t) => {
         for (var r in t) a.o(t, r) && !a.o(e, r) && Object.defineProperty(e, r, {
             enumerable: !0,
             get: t[r]
         })
-    }, a.f = {}, a.e = e => Promise.all(Object.keys(a.f).reduce(((t, r) => (a.f[r](e, t), t)), [])), a.u = e => e + ".b2bedc962bcd82714540.js?v=b2bedc962bcd82714540", a.g = function() {
+    }, a.f = {}, a.e = e => Promise.all(Object.keys(a.f).reduce(((t, r) => (a.f[r](e, t), t)), [])), a.u = e => e + ".f8f404497739316e801c.js?v=f8f404497739316e801c", a.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), a.o = (e, t) => Object.prototype.hasOwnProperty.call(e, t), a.r = e => {
```

### Comparing `tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/labextension/static/635.b2bedc962bcd82714540.js` & `tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/labextension/static/635.f8f404497739316e801c.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 635.b2bedc962bcd82714540.js.LICENSE.txt */
+/*! For license information please see 635.f8f404497739316e801c.js.LICENSE.txt */
 (self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer = self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer || []).push([
     [635], {
         9757: (t, e, r) => {
             "use strict";
             r.d(e, {
                 Z: () => i
             });
@@ -5125,15 +5125,15 @@
                     default: t
                 }
             };
             Object.defineProperty(e, "__esModule", {
                 value: !0
             });
             const s = r(4551),
-                n = i(r(2705)),
+                n = i(r(8117)),
                 a = i(r(3542)),
                 o = i(r(8005)),
                 c = i(r(9211)),
                 u = i(r(7820)),
                 p = t => {
                     const e = c.default(t),
                         r = u.default(t),
@@ -5207,15 +5207,15 @@
                     default: t
                 }
             };
             Object.defineProperty(e, "__esModule", {
                 value: !0
             });
             const s = r(4551),
-                n = i(r(2705)),
+                n = i(r(8117)),
                 a = i(r(8286));
             e.default = (t, e, r) => {
                 const i = Object.entries(r).map((([t, e]) => {
                         const r = e.offsetsBuffer.byteLength;
                         return {
                             name: t,
                             fixedLenBufferSizeInBytes: e.offsetsBuffer.byteLength || e.valuesBuffer.byteLength,
@@ -5812,15 +5812,15 @@
             const s = r(4551),
                 n = i(r(1440));
             e.default = t => {
                 const e = n.default(t);
                 return e ? e.BYTES_PER_ELEMENT : t === s.Datatype.StringAscii || t === s.Datatype.Char || t === s.Datatype.StringUtf8 ? 1 : t === s.Datatype.StringUcs2 || t === s.Datatype.StringUtf16 ? 2 : t === s.Datatype.StringUtf32 || t === s.Datatype.StringUcs4 ? 4 : void 0
             }
         },
-        2705: function(t, e, r) {
+        8117: function(t, e, r) {
             "use strict";
             var i = this && this.__importDefault || function(t) {
                 return t && t.__esModule ? t : {
                     default: t
                 }
             };
             Object.defineProperty(e, "__esModule", {
```

### Comparing `tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/labextension/static/635.b2bedc962bcd82714540.js.LICENSE.txt` & `tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/labextension/static/635.f8f404497739316e801c.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/labextension/static/744.23211eab87ca12d5bb82.js` & `tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/labextension/static/744.6ac09e98bdf01bd3b6d1.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -8,19 +8,19 @@
                 default: () => c
             });
             var t = {};
             l.r(t), l.d(t, {
                 BioImageViewerModel: () => d,
                 BioImageViewerView: () => p
             });
-            var s = l(1395);
+            var s = l(8233);
             const n = l(4147),
                 a = n.version,
                 r = n.name;
-            var o = l(2832),
+            var o = l(1057),
                 u = l.n(o);
             class d extends s.DOMWidgetModel {
                 defaults() {
                     return Object.assign(Object.assign({}, super.defaults()), {
                         _model_name: d.model_name,
                         _model_module: d.model_module,
                         _model_module_version: d.model_module_version,
@@ -37,14 +37,16 @@
                 }
                 render() {
                     const e = document.createElement("div");
                     this.el.appendChild(e), u()({
                         rootElement: e,
                         apiKey: this.values.token,
                         groupID: this.values.groupID,
+                        basePath: this.values.basePath,
+                        baseGroup: this.values.baseGroup,
                         namespace: this.values.namespace
                     })
                 }
             }
             const c = {
                 id: "@tiledb-inc/jupyter-bioimage-viewer",
                 autoStart: !0,
@@ -55,11 +57,11 @@
                         version: a,
                         exports: t
                     })
                 }
             }
         },
         4147: e => {
-            e.exports = JSON.parse('{"name":"@tiledb-inc/jupyter-bioimage-viewer","version":"0.1.2-alpha.1","description":"A jupyterlab extension to visualize bioimages in TileDB format","keywords":["jupyter","jupyterlab","jupyterlab-extension"],"homepage":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer","bugs":{"url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"},"license":"BSD-3-Clause","author":"TileDB","files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","style/*.css","style/index.js"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer.git"},"scripts":{"test":"echo No tests yet","build":"jlpm run build:lib && jlpm run build:labextension:dev","build:prod":"jlpm run build:lib && jlpm run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","clean":"jlpm run clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:labextension":"rimraf tiledb_jupyter_bioimg/labextension","clean:all":"jlpm run clean:lib && jlpm run clean:labextension","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"jupyter labextension develop --overwrite .","prepare":"jlpm run clean && jlpm run build:prod","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^5 || ^6","@jupyterlab/application":"^3.4.5","@tiledb-inc/bioimage-viewer":"^0.1.0-alpha.7"},"devDependencies":{"@jupyterlab/builder":"^3.1.0","@typescript-eslint/eslint-plugin":"^2.27.0","@typescript-eslint/parser":"^2.27.0","eslint":"^7.5.0","eslint-config-prettier":"^6.10.1","eslint-plugin-prettier":"^3.1.2","npm-run-all":"^4.1.5","prettier":"^1.19.0","rimraf":"^3.0.2","typescript":"~4.1.3"},"resolutions":{"@luma.gl/constants":"8.5.16","@luma.gl/core":"8.5.16","@luma.gl/engine":"8.5.16","@luma.gl/experimental":"8.5.16","@luma.gl/gltools":"8.5.16","@luma.gl/shadertools":"8.5.16","@luma.gl/webgl":"8.5.16","@deck.gl/aggregation-layers":"8.8.12","@deck.gl/core":"8.8.12","@deck.gl/carto":"8.8.12","@deck.gl/extensions":"8.8.12","@deck.gl/geo-layers":"8.8.12","@deck.gl/google-maps":"8.8.12","@deck.gl/mapbox":"8.8.12","@deck.gl/json":"8.8.12","@deck.gl/layers":"8.8.12","@deck.gl/mesh-layers":"8.8.12","@deck.gl/react":"8.8.12"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","jupyterlab":{"extension":"lib/index","outputDir":"tiledb_jupyter_bioimg/labextension","webpackConfig":"./webpack.config.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"@tiledb-inc/jupyter-bioimage-viewer","version":"0.1.2-alpha.2","description":"A jupyterlab extension to visualize bioimages in TileDB format","keywords":["jupyter","jupyterlab","jupyterlab-extension"],"homepage":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer","bugs":{"url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"},"license":"BSD-3-Clause","author":"TileDB","files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","style/*.css","style/index.js"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer.git"},"scripts":{"test":"echo No tests yet","build":"jlpm run build:lib && jlpm run build:labextension:dev","build:prod":"jlpm run build:lib && jlpm run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","clean":"jlpm run clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:labextension":"rimraf tiledb_jupyter_bioimg/labextension","clean:all":"jlpm run clean:lib && jlpm run clean:labextension","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"jupyter labextension develop --overwrite .","prepare":"jlpm run clean && jlpm run build:prod","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4","@jupyterlab/application":"^3.4.5","@tiledb-inc/bioimage-viewer":"^0.1.1-beta.0"},"devDependencies":{"@jupyterlab/builder":"^3.1.0","@typescript-eslint/eslint-plugin":"^2.27.0","@typescript-eslint/parser":"^2.27.0","eslint":"^7.5.0","eslint-config-prettier":"^6.10.1","eslint-plugin-prettier":"^3.1.2","npm-run-all":"^4.1.5","prettier":"^1.19.0","rimraf":"^3.0.2","typescript":"~4.1.3"},"resolutions":{"@luma.gl/constants":"8.5.16","@luma.gl/core":"8.5.16","@luma.gl/engine":"8.5.16","@luma.gl/experimental":"8.5.16","@luma.gl/gltools":"8.5.16","@luma.gl/shadertools":"8.5.16","@luma.gl/webgl":"8.5.16","@deck.gl/aggregation-layers":"8.8.12","@deck.gl/core":"8.8.12","@deck.gl/carto":"8.8.12","@deck.gl/extensions":"8.8.12","@deck.gl/geo-layers":"8.8.12","@deck.gl/google-maps":"8.8.12","@deck.gl/mapbox":"8.8.12","@deck.gl/json":"8.8.12","@deck.gl/layers":"8.8.12","@deck.gl/mesh-layers":"8.8.12","@deck.gl/react":"8.8.12"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","jupyterlab":{"extension":"lib/index","outputDir":"tiledb_jupyter_bioimg/labextension","webpackConfig":"./webpack.config.js"}}')
         }
     }
 ]);
```

### Comparing `tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js` & `tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/labextension/static/774.a940595120cb008c0c58.js` & `tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/labextension/static/774.309d750794b6276f460a.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 774.a940595120cb008c0c58.js.LICENSE.txt */
+/*! For license information please see 774.309d750794b6276f460a.js.LICENSE.txt */
 (self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer = self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer || []).push([
     [774], {
         597: (t, e, n) => {
             "use strict";
             var i, r = Object.assign || function(t) {
                     for (var e = 1; e < arguments.length; e++) {
                         var n = arguments[e];
@@ -670,54 +670,54 @@
                             style: i.pointer
                         }, this.props.pointer ? h().createElement(this.props.pointer, this.props) : h().createElement("div", {
                             style: i.slider
                         }))))
                     }
                 }]), e
             }(c.PureComponent || c.Component);
-            var O = n(5697),
-                L = n.n(O);
+            var L = n(5697),
+                O = n.n(L);
             const k = function(t, e) {
                     return t === e || t != t && e != e
                 },
-                I = function(t, e) {
+                R = function(t, e) {
                     for (var n = t.length; n--;)
                         if (k(t[n][0], e)) return n;
                     return -1
                 };
-            var R = Array.prototype.splice;
+            var I = Array.prototype.splice;
 
             function j(t) {
                 var e = -1,
                     n = null == t ? 0 : t.length;
                 for (this.clear(); ++e < n;) {
                     var i = t[e];
                     this.set(i[0], i[1])
                 }
             }
             j.prototype.clear = function() {
                 this.__data__ = [], this.size = 0
             }, j.prototype.delete = function(t) {
                 var e = this.__data__,
-                    n = I(e, t);
-                return !(n < 0 || (n == e.length - 1 ? e.pop() : R.call(e, n, 1), --this.size, 0))
+                    n = R(e, t);
+                return !(n < 0 || (n == e.length - 1 ? e.pop() : I.call(e, n, 1), --this.size, 0))
             }, j.prototype.get = function(t) {
                 var e = this.__data__,
-                    n = I(e, t);
+                    n = R(e, t);
                 return n < 0 ? void 0 : e[n][1]
             }, j.prototype.has = function(t) {
-                return I(this.__data__, t) > -1
+                return R(this.__data__, t) > -1
             }, j.prototype.set = function(t, e) {
                 var n = this.__data__,
-                    i = I(n, t);
+                    i = R(n, t);
                 return i < 0 ? (++this.size, n.push([t, e])) : n[i][1] = e, this
             };
-            const z = j;
-            var F = n(6169);
-            const B = F.Z.Symbol;
+            const F = j;
+            var z = n(6169);
+            const B = z.Z.Symbol;
             var D = Object.prototype,
                 N = D.hasOwnProperty,
                 V = D.toString,
                 U = B ? B.toStringTag : void 0;
             var G = Object.prototype.toString;
             var W = B ? B.toStringTag : void 0;
             const H = function(t) {
@@ -739,48 +739,48 @@
                     return null != t && ("object" == e || "function" == e)
                 },
                 q = function(t) {
                     if (!Z(t)) return !1;
                     var e = H(t);
                     return "[object Function]" == e || "[object GeneratorFunction]" == e || "[object AsyncFunction]" == e || "[object Proxy]" == e
                 },
-                X = F.Z["__core-js_shared__"];
+                X = z.Z["__core-js_shared__"];
             var Y = function() {
                 var t = /[^.]+$/.exec(X && X.keys && X.keys.IE_PROTO || "");
                 return t ? "Symbol(src)_1." + t : ""
             }();
             var K = Function.prototype.toString;
-            const $ = function(t) {
+            const J = function(t) {
                 if (null != t) {
                     try {
                         return K.call(t)
                     } catch (t) {}
                     try {
                         return t + ""
                     } catch (t) {}
                 }
                 return ""
             };
-            var J = /^\[object .+?Constructor\]$/,
-                Q = Function.prototype,
+            var Q = /^\[object .+?Constructor\]$/,
+                $ = Function.prototype,
                 tt = Object.prototype,
-                et = Q.toString,
+                et = $.toString,
                 nt = tt.hasOwnProperty,
                 it = RegExp("^" + et.call(nt).replace(/[\\^$.*+?()[\]{}|]/g, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$");
             const rt = function(t) {
-                    return !(!Z(t) || (e = t, Y && Y in e)) && (q(t) ? it : J).test($(t));
+                    return !(!Z(t) || (e = t, Y && Y in e)) && (q(t) ? it : Q).test(J(t));
                     var e
                 },
                 st = function(t, e) {
                     var n = function(t, e) {
                         return null == t ? void 0 : t[e]
                     }(t, e);
                     return rt(n) ? n : void 0
                 },
-                ot = st(F.Z, "Map"),
+                ot = st(z.Z, "Map"),
                 at = st(Object, "create");
             var lt = Object.prototype.hasOwnProperty;
             var ct = Object.prototype.hasOwnProperty;
 
             function ht(t) {
                 var e = -1,
                     n = null == t ? 0 : t.length;
@@ -821,15 +821,15 @@
                     var i = t[e];
                     this.set(i[0], i[1])
                 }
             }
             pt.prototype.clear = function() {
                 this.size = 0, this.__data__ = {
                     hash: new ut,
-                    map: new(ot || z),
+                    map: new(ot || F),
                     string: new ut
                 }
             }, pt.prototype.delete = function(t) {
                 var e = dt(this, t).delete(t);
                 return this.size -= e ? 1 : 0, e
             }, pt.prototype.get = function(t) {
                 return dt(this, t).get(t)
@@ -839,30 +839,30 @@
                 var n = dt(this, t),
                     i = n.size;
                 return n.set(t, e), this.size += n.size == i ? 0 : 1, this
             };
             const ft = pt;
 
             function gt(t) {
-                var e = this.__data__ = new z(t);
+                var e = this.__data__ = new F(t);
                 this.size = e.size
             }
             gt.prototype.clear = function() {
-                this.__data__ = new z, this.size = 0
+                this.__data__ = new F, this.size = 0
             }, gt.prototype.delete = function(t) {
                 var e = this.__data__,
                     n = e.delete(t);
                 return this.size = e.size, n
             }, gt.prototype.get = function(t) {
                 return this.__data__.get(t)
             }, gt.prototype.has = function(t) {
                 return this.__data__.has(t)
             }, gt.prototype.set = function(t, e) {
                 var n = this.__data__;
-                if (n instanceof z) {
+                if (n instanceof F) {
                     var i = n.__data__;
                     if (!ot || i.length < 199) return i.push([t, e]), this.size = ++n.size, this;
                     n = this.__data__ = new ft(i)
                 }
                 return n.set(t, e), this.size = n.size, this
             };
             const mt = gt,
@@ -887,15 +887,15 @@
                     for (var i = -1, r = Object(t), s = n(t), o = s.length; o--;) {
                         var a = s[++i];
                         if (!1 === e(r[a], a, r)) break
                     }
                     return t
                 };
             var xt = n(2896);
-            const wt = F.Z.Uint8Array,
+            const wt = z.Z.Uint8Array,
                 Et = function(t, e) {
                     var n = e ? function(t) {
                         var e = new t.constructor(t.byteLength);
                         return new wt(e).set(new wt(t)), e
                     }(t.buffer) : t.buffer;
                     return new t.constructor(n, t.byteOffset, t.length)
                 };
@@ -917,67 +917,67 @@
                 },
                 Tt = Ct(Object.getPrototypeOf, Object);
             var At = Object.prototype;
             const Mt = function(t) {
                     var e = t && t.constructor;
                     return t === ("function" == typeof e && e.prototype || At)
                 },
-                Ot = function(t) {
+                Lt = function(t) {
                     return null != t && "object" == typeof t
                 },
-                Lt = function(t) {
-                    return Ot(t) && "[object Arguments]" == H(t)
+                Ot = function(t) {
+                    return Lt(t) && "[object Arguments]" == H(t)
                 };
             var kt = Object.prototype,
-                It = kt.hasOwnProperty,
-                Rt = kt.propertyIsEnumerable;
-            const jt = Lt(function() {
+                Rt = kt.hasOwnProperty,
+                It = kt.propertyIsEnumerable;
+            const jt = Ot(function() {
                     return arguments
-                }()) ? Lt : function(t) {
-                    return Ot(t) && It.call(t, "callee") && !Rt.call(t, "callee")
+                }()) ? Ot : function(t) {
+                    return Lt(t) && Rt.call(t, "callee") && !It.call(t, "callee")
                 },
-                zt = Array.isArray,
-                Ft = function(t) {
+                Ft = Array.isArray,
+                zt = function(t) {
                     return "number" == typeof t && t > -1 && t % 1 == 0 && t <= 9007199254740991
                 },
                 Bt = function(t) {
-                    return null != t && Ft(t.length) && !q(t)
+                    return null != t && zt(t.length) && !q(t)
                 };
             var Dt = n(4002),
                 Nt = Function.prototype,
                 Vt = Object.prototype,
                 Ut = Nt.toString,
                 Gt = Vt.hasOwnProperty,
                 Wt = Ut.call(Object);
             var Ht = {};
             Ht["[object Float32Array]"] = Ht["[object Float64Array]"] = Ht["[object Int8Array]"] = Ht["[object Int16Array]"] = Ht["[object Int32Array]"] = Ht["[object Uint8Array]"] = Ht["[object Uint8ClampedArray]"] = Ht["[object Uint16Array]"] = Ht["[object Uint32Array]"] = !0, Ht["[object Arguments]"] = Ht["[object Array]"] = Ht["[object ArrayBuffer]"] = Ht["[object Boolean]"] = Ht["[object DataView]"] = Ht["[object Date]"] = Ht["[object Error]"] = Ht["[object Function]"] = Ht["[object Map]"] = Ht["[object Number]"] = Ht["[object Object]"] = Ht["[object RegExp]"] = Ht["[object Set]"] = Ht["[object String]"] = Ht["[object WeakMap]"] = !1;
             var Zt = n(9730),
                 qt = Zt.Z && Zt.Z.isTypedArray;
             const Xt = qt ? (Yt = qt, function(t) {
                 return Yt(t)
             }) : function(t) {
-                return Ot(t) && Ft(t.length) && !!Ht[H(t)]
+                return Lt(t) && zt(t.length) && !!Ht[H(t)]
             };
             var Yt;
             const Kt = function(t, e) {
                 if (("constructor" !== e || "function" != typeof t[e]) && "__proto__" != e) return t[e]
             };
-            var $t = Object.prototype.hasOwnProperty;
-            const Jt = function(t, e, n) {
+            var Jt = Object.prototype.hasOwnProperty;
+            const Qt = function(t, e, n) {
                 var i = t[e];
-                $t.call(t, e) && k(i, n) && (void 0 !== n || e in t) || bt(t, e, n)
+                Jt.call(t, e) && k(i, n) && (void 0 !== n || e in t) || bt(t, e, n)
             };
-            var Qt = /^(?:0|[1-9]\d*)$/;
+            var $t = /^(?:0|[1-9]\d*)$/;
             const te = function(t, e) {
                 var n = typeof t;
-                return !!(e = null == e ? 9007199254740991 : e) && ("number" == n || "symbol" != n && Qt.test(t)) && t > -1 && t % 1 == 0 && t < e
+                return !!(e = null == e ? 9007199254740991 : e) && ("number" == n || "symbol" != n && $t.test(t)) && t > -1 && t % 1 == 0 && t < e
             };
             var ee = Object.prototype.hasOwnProperty;
             const ne = function(t, e) {
-                var n = zt(t),
+                var n = Ft(t),
                     i = !n && jt(t),
                     r = !n && !i && (0, Dt.Z)(t),
                     s = !n && !i && !r && Xt(t),
                     o = n || i || r || s,
                     a = o ? function(t, e) {
                         for (var n = -1, i = Array(t); ++n < t;) i[n] = e(n);
                         return i
@@ -1005,38 +1005,38 @@
                 oe = function(t) {
                     return function(t, e, n, i) {
                         var r = !n;
                         n || (n = {});
                         for (var s = -1, o = e.length; ++s < o;) {
                             var a = e[s],
                                 l = i ? i(n[a], t[a], a, n, t) : void 0;
-                            void 0 === l && (l = t[a]), r ? bt(n, a, l) : Jt(n, a, l)
+                            void 0 === l && (l = t[a]), r ? bt(n, a, l) : Qt(n, a, l)
                         }
                         return n
                     }(t, se(t))
                 },
                 ae = function(t, e, n, i, r, s, o) {
                     var a, l = Kt(t, n),
                         c = Kt(e, n),
                         h = o.get(c);
                     if (h) yt(t, n, h);
                     else {
                         var u = s ? s(l, c, n + "", t, e, o) : void 0,
                             d = void 0 === u;
                         if (d) {
-                            var p = zt(c),
+                            var p = Ft(c),
                                 f = !p && (0, Dt.Z)(c),
                                 g = !p && !f && Xt(c);
-                            u = c, p || f || g ? zt(l) ? u = l : Ot(a = l) && Bt(a) ? u = function(t, e) {
+                            u = c, p || f || g ? Ft(l) ? u = l : Lt(a = l) && Bt(a) ? u = function(t, e) {
                                 var n = -1,
                                     i = t.length;
                                 for (e || (e = Array(i)); ++n < i;) e[n] = t[n];
                                 return e
                             }(l) : f ? (d = !1, u = (0, xt.Z)(c, !0)) : g ? (d = !1, u = Et(c, !0)) : u = [] : function(t) {
-                                if (!Ot(t) || "[object Object]" != H(t)) return !1;
+                                if (!Lt(t) || "[object Object]" != H(t)) return !1;
                                 var e = Tt(t);
                                 if (null === e) return !0;
                                 var n = Gt.call(e, "constructor") && e.constructor;
                                 return "function" == typeof n && n instanceof n && Ut.call(n) == Wt
                             }(c) || jt(c) ? (u = l, jt(l) ? u = oe(l) : Z(l) && !q(l) || (u = function(t) {
                                 return "function" != typeof t.constructor || Mt(t) ? {} : St(Tt(t))
                             }(c))) : d = !1
@@ -1193,38 +1193,38 @@
                 }, h().createElement("div", {
                     style: a.bg
                 }), h().createElement("div", {
                     style: a.content
                 }, r))
             };
             ve.propTypes = {
-                background: L().string,
-                zDepth: L().oneOf([0, 1, 2, 3, 4, 5]),
-                radius: L().number,
-                styles: L().object
+                background: O().string,
+                zDepth: O().oneOf([0, 1, 2, 3, 4, 5]),
+                radius: O().number,
+                styles: O().object
             }, ve.defaultProps = {
                 background: "#fff",
                 zDepth: 1,
                 radius: 2,
                 styles: {}
             };
             const be = ve,
                 ye = function() {
-                    return F.Z.Date.now()
+                    return z.Z.Date.now()
                 };
             var _e = /\s/;
             var xe = /^\s+/;
             const we = function(t) {
                     return t ? t.slice(0, function(t) {
                         for (var e = t.length; e-- && _e.test(t.charAt(e)););
                         return e
                     }(t) + 1).replace(xe, "") : t
                 },
                 Ee = function(t) {
-                    return "symbol" == typeof t || Ot(t) && "[object Symbol]" == H(t)
+                    return "symbol" == typeof t || Lt(t) && "[object Symbol]" == H(t)
                 };
             var Pe = /^[-+]0x[0-9a-f]+$/i,
                 Se = /^0b[01]+$/i,
                 Ce = /^0o[0-7]+$/i,
                 Te = parseInt;
             const Ae = function(t) {
                 if ("number" == typeof t) return t;
@@ -1235,16 +1235,16 @@
                 }
                 if ("string" != typeof t) return 0 === t ? t : +t;
                 t = we(t);
                 var n = Se.test(t);
                 return n || Ce.test(t) ? Te(t.slice(2), n ? 2 : 8) : Pe.test(t) ? NaN : +t
             };
             var Me = Math.max,
-                Oe = Math.min;
-            const Le = function(t, e, n) {
+                Le = Math.min;
+            const Oe = function(t, e, n) {
                 var i, r, s, o, a, l, c = 0,
                     h = !1,
                     u = !1,
                     d = !0;
                 if ("function" != typeof t) throw new TypeError("Expected a function");
 
                 function p(e) {
@@ -1259,15 +1259,15 @@
                 }
 
                 function g() {
                     var t = ye();
                     if (f(t)) return m(t);
                     a = setTimeout(g, function(t) {
                         var n = e - (t - l);
-                        return u ? Oe(n, s - (t - c)) : n
+                        return u ? Le(n, s - (t - c)) : n
                     }(t))
                 }
 
                 function m(t) {
                     return a = void 0, d && i ? p(t) : (i = r = void 0, o)
                 }
 
@@ -1295,15 +1295,15 @@
                             i.enumerable = i.enumerable || !1, i.configurable = !0, "value" in i && (i.writable = !0), Object.defineProperty(t, i.key, i)
                         }
                     }
                     return function(e, n, i) {
                         return n && t(e.prototype, n), i && t(e, i), e
                     }
                 }(),
-                Ie = function(t) {
+                Re = function(t) {
                     function e(t) {
                         ! function(t, e) {
                             if (!(t instanceof e)) throw new TypeError("Cannot call a class as a function")
                         }(this, e);
                         var n = function(t, e) {
                             if (!t) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
                             return !e || "object" != typeof e && "function" != typeof e ? t : e
@@ -1334,15 +1334,15 @@
                             e.addEventListener("mousemove", n.handleChange), e.addEventListener("mouseup", n.handleMouseUp)
                         }, n.handleMouseUp = function() {
                             n.unbindEventListeners()
                         }, n.throttle = function(t, e, n) {
                             var i = !0,
                                 r = !0;
                             if ("function" != typeof t) throw new TypeError("Expected a function");
-                            return Z(n) && (i = "leading" in n ? !!n.leading : i, r = "trailing" in n ? !!n.trailing : r), Le(t, e, {
+                            return Z(n) && (i = "leading" in n ? !!n.leading : i, r = "trailing" in n ? !!n.trailing : r), Oe(t, e, {
                                 leading: i,
                                 maxWait: e,
                                 trailing: r
                             })
                         }((function(t, e, n) {
                             t(e, n)
                         }), 50), n
@@ -1443,39 +1443,39 @@
                                 style: a.pointer
                             }, this.props.pointer ? h().createElement(this.props.pointer, this.props) : h().createElement("div", {
                                 style: a.circle
                             }))))
                         }
                     }]), e
                 }(c.PureComponent || c.Component);
-            const Re = Ie,
+            const Ie = Re,
                 je = function(t, e) {
                     for (var n = -1, i = null == t ? 0 : t.length; ++n < i && !1 !== e(t[n], n, t););
                     return t
                 },
-                ze = Ct(Object.keys, Object);
-            var Fe = Object.prototype.hasOwnProperty;
+                Fe = Ct(Object.keys, Object);
+            var ze = Object.prototype.hasOwnProperty;
             const Be = function(t) {
                     return Bt(t) ? ne(t) : function(t) {
-                        if (!Mt(t)) return ze(t);
+                        if (!Mt(t)) return Fe(t);
                         var e = [];
-                        for (var n in Object(t)) Fe.call(t, n) && "constructor" != n && e.push(n);
+                        for (var n in Object(t)) ze.call(t, n) && "constructor" != n && e.push(n);
                         return e
                     }(t)
                 },
                 De = function(t, e) {
                     if (null == t) return t;
                     if (!Bt(t)) return function(t, e) {
                         return t && _t(t, e, Be)
                     }(t, e);
                     for (var n = t.length, i = -1, r = Object(t); ++i < n && !1 !== e(r[i], i, r););
                     return t
                 },
                 Ne = function(t, e) {
-                    return (zt(t) ? je : De)(t, "function" == typeof(n = e) ? n : ce);
+                    return (Ft(t) ? je : De)(t, "function" == typeof(n = e) ? n : ce);
                     var n
                 };
 
             function Ve(t) {
                 return Ve = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
                     return typeof t
                 } : function(t) {
@@ -1678,25 +1678,25 @@
 
             function Ke(t, e) {
                 e = 0 === e ? 0 : e || 10;
                 var n = We(t).toHsl();
                 return n.s += e / 100, n.s = dn(n.s), We(n)
             }
 
-            function $e(t) {
+            function Je(t) {
                 return We(t).desaturate(100)
             }
 
-            function Je(t, e) {
+            function Qe(t, e) {
                 e = 0 === e ? 0 : e || 10;
                 var n = We(t).toHsl();
                 return n.l += e / 100, n.l = dn(n.l), We(n)
             }
 
-            function Qe(t, e) {
+            function $e(t, e) {
                 e = 0 === e ? 0 : e || 10;
                 var n = We(t).toRgb();
                 return n.r = Math.max(0, Math.min(255, n.r - Math.round(-e / 100 * 255))), n.g = Math.max(0, Math.min(255, n.g - Math.round(-e / 100 * 255))), n.b = Math.max(0, Math.min(255, n.b - Math.round(-e / 100 * 255))), We(n)
             }
 
             function tn(t, e) {
                 e = 0 === e ? 0 : e || 10;
@@ -1880,30 +1880,30 @@
                     return We(this.toString())
                 },
                 _applyModification: function(t, e) {
                     var n = t.apply(null, [this].concat([].slice.call(e)));
                     return this._r = n._r, this._g = n._g, this._b = n._b, this.setAlpha(n._a), this
                 },
                 lighten: function() {
-                    return this._applyModification(Je, arguments)
+                    return this._applyModification(Qe, arguments)
                 },
                 brighten: function() {
-                    return this._applyModification(Qe, arguments)
+                    return this._applyModification($e, arguments)
                 },
                 darken: function() {
                     return this._applyModification(tn, arguments)
                 },
                 desaturate: function() {
                     return this._applyModification(Ye, arguments)
                 },
                 saturate: function() {
                     return this._applyModification(Ke, arguments)
                 },
                 greyscale: function() {
-                    return this._applyModification($e, arguments)
+                    return this._applyModification(Je, arguments)
                 },
                 spin: function() {
                     return this._applyModification(en, arguments)
                 },
                 _applyCombination: function(t, e) {
                     return t.apply(null, [this].concat([].slice.call(e)))
                 },
@@ -2245,15 +2245,15 @@
                             i.enumerable = i.enumerable || !1, i.configurable = !0, "value" in i && (i.writable = !0), Object.defineProperty(t, i.key, i)
                         }
                     }
                     return function(e, n, i) {
                         return n && t(e.prototype, n), i && t(e, i), e
                     }
                 }();
-            const On = function(t) {
+            const Ln = function(t) {
                 var e = function(e) {
                     function n(t) {
                         ! function(t, e) {
                             if (!(t instanceof e)) throw new TypeError("Cannot call a class as a function")
                         }(this, n);
                         var e = function(t, e) {
                             if (!t) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
@@ -2265,15 +2265,15 @@
                                 e.setState(i), e.props.onChangeComplete && e.debounce(e.props.onChangeComplete, i, n), e.props.onChange && e.props.onChange(i, n)
                             }
                         }, e.handleSwatchHover = function(t, n) {
                             if (En(t)) {
                                 var i = Pn(t, t.h || e.state.oldHue);
                                 e.props.onSwatchHover && e.props.onSwatchHover(i, n)
                             }
-                        }, e.state = An({}, Pn(t.color, 0)), e.debounce = Le((function(t, e, n) {
+                        }, e.state = An({}, Pn(t.color, 0)), e.debounce = Oe((function(t, e, n) {
                             t(e, n)
                         }), 100), e
                     }
                     return function(t, e) {
                         if ("function" != typeof e && null !== e) throw new TypeError("Super expression must either be null or a function, not " + typeof e);
                         t.prototype = Object.create(e && e.prototype, {
                             constructor: {
@@ -2303,15 +2303,15 @@
                         h: 250,
                         s: .5,
                         l: .2,
                         a: 1
                     }
                 }), e
             };
-            var Ln = Object.assign || function(t) {
+            var On = Object.assign || function(t) {
                     for (var e = 1; e < arguments.length; e++) {
                         var n = arguments[e];
                         for (var i in n) Object.prototype.hasOwnProperty.call(n, i) && (t[i] = n[i])
                     }
                     return t
                 },
                 kn = function() {
@@ -2322,19 +2322,19 @@
                         }
                     }
                     return function(e, n, i) {
                         return n && t(e.prototype, n), i && t(e, i), e
                     }
                 }();
 
-            function In(t, e) {
+            function Rn(t, e) {
                 if (!t) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
                 return !e || "object" != typeof e && "function" != typeof e ? t : e
             }
-            var Rn = Object.assign || function(t) {
+            var In = Object.assign || function(t) {
                 for (var e = 1; e < arguments.length; e++) {
                     var n = arguments[e];
                     for (var i in n) Object.prototype.hasOwnProperty.call(n, i) && (t[i] = n[i])
                 }
                 return t
             };
             const jn = function(t) {
@@ -2342,25 +2342,25 @@
                 return function(n) {
                     function i() {
                         var t, e, n;
                         ! function(t, e) {
                             if (!(t instanceof e)) throw new TypeError("Cannot call a class as a function")
                         }(this, i);
                         for (var r = arguments.length, s = Array(r), o = 0; o < r; o++) s[o] = arguments[o];
-                        return e = n = In(this, (t = i.__proto__ || Object.getPrototypeOf(i)).call.apply(t, [this].concat(s))), n.state = {
+                        return e = n = Rn(this, (t = i.__proto__ || Object.getPrototypeOf(i)).call.apply(t, [this].concat(s))), n.state = {
                             focus: !1
                         }, n.handleFocus = function() {
                             return n.setState({
                                 focus: !0
                             })
                         }, n.handleBlur = function() {
                             return n.setState({
                                 focus: !1
                             })
-                        }, In(n, e)
+                        }, Rn(n, e)
                     }
                     return function(t, e) {
                         if ("function" != typeof e && null !== e) throw new TypeError("Super expression must either be null or a function, not " + typeof e);
                         t.prototype = Object.create(e && e.prototype, {
                             constructor: {
                                 value: t,
                                 enumerable: !1,
@@ -2370,15 +2370,15 @@
                         }), e && (Object.setPrototypeOf ? Object.setPrototypeOf(t, e) : t.__proto__ = e)
                     }(i, n), kn(i, [{
                         key: "render",
                         value: function() {
                             return h().createElement(e, {
                                 onFocus: this.handleFocus,
                                 onBlur: this.handleBlur
-                            }, h().createElement(t, Ln({}, this.props, this.state)))
+                            }, h().createElement(t, On({}, this.props, this.state)))
                         }
                     }]), i
                 }(h().Component)
             }((function(t) {
                 var e = t.color,
                     n = t.style,
                     i = t.onClick,
@@ -2389,50 +2389,50 @@
                     l = t.children,
                     c = t.focus,
                     u = t.focusStyle,
                     d = void 0 === u ? {} : u,
                     f = "transparent" === e,
                     g = (0, p.ZP)({
                         default: {
-                            swatch: Rn({
+                            swatch: In({
                                 background: e,
                                 height: "100%",
                                 width: "100%",
                                 cursor: "pointer",
                                 position: "relative",
                                 outline: "none"
                             }, n, c ? d : {})
                         }
                     }),
                     m = {};
                 return s && (m.onMouseOver = function(t) {
                     return s(e, t)
-                }), h().createElement("div", Rn({
+                }), h().createElement("div", In({
                     style: g.swatch,
                     onClick: function(t) {
                         return r(e, t)
                     },
                     title: a,
                     tabIndex: 0,
                     onKeyDown: function(t) {
                         return 13 === t.keyCode && r(e, t)
                     }
                 }, m), l, f && h().createElement(b, {
                     borderRadius: g.swatch.borderRadius,
                     boxShadow: "inset 0 0 0 1px rgba(0,0,0,0.1)"
                 }))
             }));
-            var zn = Object.assign || function(t) {
+            var Fn = Object.assign || function(t) {
                     for (var e = 1; e < arguments.length; e++) {
                         var n = arguments[e];
                         for (var i in n) Object.prototype.hasOwnProperty.call(n, i) && (t[i] = n[i])
                     }
                     return t
                 },
-                Fn = function(t) {
+                zn = function(t) {
                     var e = t.rgb,
                         n = t.hsl,
                         i = t.width,
                         r = t.height,
                         s = t.onChange,
                         o = t.direction,
                         a = t.style,
@@ -2452,24 +2452,24 @@
                                     style: a
                                 }
                             }
                         });
                     return h().createElement("div", {
                         style: f.picker,
                         className: "alpha-picker " + d
-                    }, h().createElement(w, zn({}, f.alpha, {
+                    }, h().createElement(w, Fn({}, f.alpha, {
                         rgb: e,
                         hsl: n,
                         pointer: c,
                         renderers: l,
                         onChange: s,
                         direction: o
                     })))
                 };
-            Fn.defaultProps = {
+            zn.defaultProps = {
                 width: "316px",
                 height: "16px",
                 direction: "horizontal",
                 pointer: function(t) {
                     var e = t.direction,
                         n = (0, p.ZP)({
                             default: {
@@ -2490,15 +2490,15 @@
                         }, {
                             vertical: "vertical" === e
                         });
                     return h().createElement("div", {
                         style: n.picker
                     })
                 }
-            }, On(Fn);
+            }, Ln(zn);
             const Bn = function(t, e) {
                 for (var n = -1, i = null == t ? 0 : t.length, r = Array(i); ++n < i;) r[n] = e(t[n], n, t);
                 return r
             };
 
             function Dn(t) {
                 var e = -1,
@@ -2580,43 +2580,43 @@
                         return s
                     }(Yn(t), (function(e) {
                         return Xn.call(t, e)
                     })))
                 } : function() {
                     return []
                 },
-                $n = function(t) {
+                Jn = function(t) {
                     return function(t, e, n) {
                         var i = e(t);
-                        return zt(t) ? i : function(t, e) {
+                        return Ft(t) ? i : function(t, e) {
                             for (var n = -1, i = e.length, r = t.length; ++n < i;) t[r + n] = e[n];
                             return t
                         }(i, n(t))
                     }(t, Be, Kn)
                 };
-            var Jn = Object.prototype.hasOwnProperty;
-            const Qn = st(F.Z, "DataView"),
-                ti = st(F.Z, "Promise"),
-                ei = st(F.Z, "Set"),
-                ni = st(F.Z, "WeakMap");
+            var Qn = Object.prototype.hasOwnProperty;
+            const $n = st(z.Z, "DataView"),
+                ti = st(z.Z, "Promise"),
+                ei = st(z.Z, "Set"),
+                ni = st(z.Z, "WeakMap");
             var ii = "[object Map]",
                 ri = "[object Promise]",
                 si = "[object Set]",
                 oi = "[object WeakMap]",
                 ai = "[object DataView]",
-                li = $(Qn),
-                ci = $(ot),
-                hi = $(ti),
-                ui = $(ei),
-                di = $(ni),
+                li = J($n),
+                ci = J(ot),
+                hi = J(ti),
+                ui = J(ei),
+                di = J(ni),
                 pi = H;
-            (Qn && pi(new Qn(new ArrayBuffer(1))) != ai || ot && pi(new ot) != ii || ti && pi(ti.resolve()) != ri || ei && pi(new ei) != si || ni && pi(new ni) != oi) && (pi = function(t) {
+            ($n && pi(new $n(new ArrayBuffer(1))) != ai || ot && pi(new ot) != ii || ti && pi(ti.resolve()) != ri || ei && pi(new ei) != si || ni && pi(new ni) != oi) && (pi = function(t) {
                 var e = H(t),
                     n = "[object Object]" == e ? t.constructor : void 0,
-                    i = n ? $(n) : "";
+                    i = n ? J(n) : "";
                 if (i) switch (i) {
                     case li:
                         return ai;
                     case ci:
                         return ii;
                     case hi:
                         return ri;
@@ -2629,16 +2629,16 @@
             });
             const fi = pi;
             var gi = "[object Arguments]",
                 mi = "[object Array]",
                 vi = "[object Object]",
                 bi = Object.prototype.hasOwnProperty;
             const yi = function(t, e, n, i, r, s) {
-                    var o = zt(t),
-                        a = zt(e),
+                    var o = Ft(t),
+                        a = Ft(e),
                         l = o ? mi : fi(t),
                         c = a ? mi : fi(e),
                         h = (l = l == gi ? vi : l) == vi,
                         u = (c = c == gi ? vi : c) == vi,
                         d = l == c;
                     if (d && (0, Dt.Z)(t)) {
                         if (!(0, Dt.Z)(e)) return !1;
@@ -2682,20 +2682,20 @@
                             var g = p ? t.value() : t,
                                 m = f ? e.value() : e;
                             return s || (s = new mt), r(g, m, n, i, s)
                         }
                     }
                     return !!d && (s || (s = new mt), function(t, e, n, i, r, s) {
                         var o = 1 & n,
-                            a = $n(t),
+                            a = Jn(t),
                             l = a.length;
-                        if (l != $n(e).length && !o) return !1;
+                        if (l != Jn(e).length && !o) return !1;
                         for (var c = l; c--;) {
                             var h = a[c];
-                            if (!(o ? h in e : Jn.call(e, h))) return !1
+                            if (!(o ? h in e : Qn.call(e, h))) return !1
                         }
                         var u = s.get(t),
                             d = s.get(e);
                         if (u && d) return u == e && d == t;
                         var p = !0;
                         s.set(t, e), s.set(e, t);
                         for (var f = o; ++c < l;) {
@@ -2713,15 +2713,15 @@
                                 y = e.constructor;
                             b == y || !("constructor" in t) || !("constructor" in e) || "function" == typeof b && b instanceof b && "function" == typeof y && y instanceof y || (p = !1)
                         }
                         return s.delete(t), s.delete(e), p
                     }(t, e, n, i, r, s))
                 },
                 _i = function t(e, n, i, r, s) {
-                    return e === n || (null == e || null == n || !Ot(e) && !Ot(n) ? e != e && n != n : yi(e, n, i, r, t, s))
+                    return e === n || (null == e || null == n || !Lt(e) && !Lt(n) ? e != e && n != n : yi(e, n, i, r, t, s))
                 },
                 xi = function(t) {
                     return t == t && !Z(t)
                 },
                 wi = function(t, e) {
                     return function(n) {
                         return null != n && n[t] === e && (void 0 !== e || t in Object(n))
@@ -2761,15 +2761,15 @@
                             return !0
                         }(n, t, e)
                     }
                 };
             var Pi = /\.|\[(?:[^[\]]*|(["'])(?:(?!\1)[^\\]|\\.)*?\1)\]/,
                 Si = /^\w*$/;
             const Ci = function(t, e) {
-                if (zt(t)) return !1;
+                if (Ft(t)) return !1;
                 var n = typeof t;
                 return !("number" != n && "symbol" != n && "boolean" != n && null != t && !Ee(t)) || Si.test(t) || !Pi.test(t) || null != e && t in Object(e)
             };
 
             function Ti(t, e) {
                 if ("function" != typeof t || null != e && "function" != typeof e) throw new TypeError("Expected a function");
                 var n = function() {
@@ -2781,75 +2781,75 @@
                     return n.cache = s.set(r, o) || s, o
                 };
                 return n.cache = new(Ti.Cache || ft), n
             }
             Ti.Cache = ft;
             const Ai = Ti;
             var Mi = /[^.[\]]+|\[(?:(-?\d+(?:\.\d+)?)|(["'])((?:(?!\2)[^\\]|\\.)*?)\2)\]|(?=(?:\.|\[\])(?:\.|\[\]|$))/g,
-                Oi = /\\(\\)?/g;
-            const Li = function(t) {
+                Li = /\\(\\)?/g;
+            const Oi = function(t) {
                 var e = Ai(t, (function(t) {
                         return 500 === n.size && n.clear(), t
                     })),
                     n = e.cache;
                 return e
             }((function(t) {
                 var e = [];
                 return 46 === t.charCodeAt(0) && e.push(""), t.replace(Mi, (function(t, n, i, r) {
-                    e.push(i ? r.replace(Oi, "$1") : n || t)
+                    e.push(i ? r.replace(Li, "$1") : n || t)
                 })), e
             }));
             var ki = B ? B.prototype : void 0,
-                Ii = ki ? ki.toString : void 0;
-            const Ri = function t(e) {
+                Ri = ki ? ki.toString : void 0;
+            const Ii = function t(e) {
                     if ("string" == typeof e) return e;
-                    if (zt(e)) return Bn(e, t) + "";
-                    if (Ee(e)) return Ii ? Ii.call(e) : "";
+                    if (Ft(e)) return Bn(e, t) + "";
+                    if (Ee(e)) return Ri ? Ri.call(e) : "";
                     var n = e + "";
                     return "0" == n && 1 / e == -1 / 0 ? "-0" : n
                 },
                 ji = function(t) {
-                    return null == t ? "" : Ri(t)
+                    return null == t ? "" : Ii(t)
                 },
-                zi = function(t, e) {
-                    return zt(t) ? t : Ci(t, e) ? [t] : Li(ji(t))
+                Fi = function(t, e) {
+                    return Ft(t) ? t : Ci(t, e) ? [t] : Oi(ji(t))
                 },
-                Fi = function(t) {
+                zi = function(t) {
                     if ("string" == typeof t || Ee(t)) return t;
                     var e = t + "";
                     return "0" == e && 1 / t == -1 / 0 ? "-0" : e
                 },
                 Bi = function(t, e) {
-                    for (var n = 0, i = (e = zi(e, t)).length; null != t && n < i;) t = t[Fi(e[n++])];
+                    for (var n = 0, i = (e = Fi(e, t)).length; null != t && n < i;) t = t[zi(e[n++])];
                     return n && n == i ? t : void 0
                 },
                 Di = function(t, e) {
                     return null != t && e in Object(t)
                 },
                 Ni = function(t, e) {
                     return null != t && function(t, e, n) {
-                        for (var i = -1, r = (e = zi(e, t)).length, s = !1; ++i < r;) {
-                            var o = Fi(e[i]);
+                        for (var i = -1, r = (e = Fi(e, t)).length, s = !1; ++i < r;) {
+                            var o = zi(e[i]);
                             if (!(s = null != t && n(t, o))) break;
                             t = t[o]
                         }
-                        return s || ++i != r ? s : !!(r = null == t ? 0 : t.length) && Ft(r) && te(o, r) && (zt(t) || jt(t))
+                        return s || ++i != r ? s : !!(r = null == t ? 0 : t.length) && zt(r) && te(o, r) && (Ft(t) || jt(t))
                     }(t, e, Di)
                 },
                 Vi = function(t, e) {
-                    return Ci(t) && xi(e) ? wi(Fi(t), e) : function(n) {
+                    return Ci(t) && xi(e) ? wi(zi(t), e) : function(n) {
                         var i = function(t, e, n) {
                             var i = null == t ? void 0 : Bi(t, e);
                             return void 0 === i ? n : i
                         }(n, t);
                         return void 0 === i && i === e ? Ni(n, t) : _i(e, i, 3)
                     }
                 },
                 Ui = function(t) {
-                    return Ci(t) ? (e = Fi(t), function(t) {
+                    return Ci(t) ? (e = zi(t), function(t) {
                         return null == t ? void 0 : t[e]
                     }) : function(t) {
                         return function(e) {
                             return Bi(e, t)
                         }
                     }(t);
                     var e
@@ -2858,15 +2858,15 @@
                     var n = -1,
                         i = Bt(t) ? Array(t.length) : [];
                     return De(t, (function(t, r, s) {
                         i[++n] = e(t, r, s)
                     })), i
                 },
                 Wi = function(t, e) {
-                    return (zt(t) ? Bn : Gi)(t, "function" == typeof(n = e) ? n : null == n ? ce : "object" == typeof n ? zt(n) ? Vi(n[0], n[1]) : Ei(n) : Ui(n));
+                    return (Ft(t) ? Bn : Gi)(t, "function" == typeof(n = e) ? n : null == n ? ce : "object" == typeof n ? Ft(n) ? Vi(n[0], n[1]) : Ei(n) : Ui(n));
                     var n
                 },
                 Hi = function(t) {
                     var e = t.colors,
                         n = t.onClick,
                         i = t.onSwatchHover,
                         r = (0, p.ZP)({
@@ -3002,31 +3002,31 @@
                         input: g.input
                     },
                     value: i,
                     onChange: f
                 })))
             };
             Zi.propTypes = {
-                width: L().oneOfType([L().string, L().number]),
-                colors: L().arrayOf(L().string),
-                triangle: L().oneOf(["top", "hide"]),
-                styles: L().object
+                width: O().oneOfType([O().string, O().number]),
+                colors: O().arrayOf(O().string),
+                triangle: O().oneOf(["top", "hide"]),
+                styles: O().object
             }, Zi.defaultProps = {
                 width: 170,
                 colors: ["#D9E3F0", "#F47373", "#697689", "#37D67A", "#2CCCE4", "#555555", "#dce775", "#ff8a65", "#ba68c8"],
                 triangle: "top",
                 styles: {}
-            }, On(Zi);
+            }, Ln(Zi);
             var qi = "#ffcdd2",
                 Xi = "#e57373",
                 Yi = "#f44336",
                 Ki = "#d32f2f",
-                $i = "#b71c1c",
-                Ji = "#f8bbd0",
-                Qi = "#f06292",
+                Ji = "#b71c1c",
+                Qi = "#f8bbd0",
+                $i = "#f06292",
                 tr = "#e91e63",
                 er = "#c2185b",
                 nr = "#880e4f",
                 ir = "#e1bee7",
                 rr = "#ba68c8",
                 sr = "#9c27b0",
                 or = "#7b1fa2",
@@ -3049,38 +3049,38 @@
                 Er = "#b3e5fc",
                 Pr = "#4fc3f7",
                 Sr = "#03a9f4",
                 Cr = "#0288d1",
                 Tr = "#01579b",
                 Ar = "#b2ebf2",
                 Mr = "#4dd0e1",
-                Or = "#00bcd4",
-                Lr = "#0097a7",
+                Lr = "#00bcd4",
+                Or = "#0097a7",
                 kr = "#006064",
-                Ir = "#b2dfdb",
-                Rr = "#4db6ac",
+                Rr = "#b2dfdb",
+                Ir = "#4db6ac",
                 jr = "#009688",
-                zr = "#00796b",
-                Fr = "#004d40",
+                Fr = "#00796b",
+                zr = "#004d40",
                 Br = "#c8e6c9",
                 Dr = "#81c784",
                 Nr = "#4caf50",
                 Vr = "#388e3c",
                 Ur = "#dcedc8",
                 Gr = "#aed581",
                 Wr = "#8bc34a",
                 Hr = "#689f38",
                 Zr = "#33691e",
                 qr = "#f0f4c3",
                 Xr = "#dce775",
                 Yr = "#cddc39",
                 Kr = "#afb42b",
-                $r = "#827717",
-                Jr = "#fff9c4",
-                Qr = "#fff176",
+                Jr = "#827717",
+                Qr = "#fff9c4",
+                $r = "#fff176",
                 ts = "#ffeb3b",
                 es = "#fbc02d",
                 ns = "#f57f17",
                 is = "#ffecb3",
                 rs = "#ffd54f",
                 ss = "#ffc107",
                 os = "#ffa000",
@@ -3157,15 +3157,15 @@
                     }))
                 };
             As.defaultProps = {
                 circleSize: 28,
                 circleSpacing: 14
             };
             const Ms = (0, p.tz)(As);
-            var Os = function(t) {
+            var Ls = function(t) {
                 var e = t.width,
                     n = t.onChange,
                     i = t.onSwatchHover,
                     r = t.colors,
                     s = t.hex,
                     o = t.circleSize,
                     a = t.styles,
@@ -3201,42 +3201,42 @@
                         onSwatchHover: i,
                         active: s === t.toLowerCase(),
                         circleSize: o,
                         circleSpacing: c
                     })
                 })))
             };
-            Os.propTypes = {
-                width: L().oneOfType([L().string, L().number]),
-                circleSize: L().number,
-                circleSpacing: L().number,
-                styles: L().object
-            }, Os.defaultProps = {
+            Ls.propTypes = {
+                width: O().oneOfType([O().string, O().number]),
+                circleSize: O().number,
+                circleSpacing: O().number,
+                styles: O().object
+            }, Ls.defaultProps = {
                 width: 252,
                 circleSize: 28,
                 circleSpacing: 14,
-                colors: [Yi, tr, sr, hr, gr, _r, Sr, Or, jr, Nr, Wr, Yr, ts, ss, hs, gs, _s, Ss],
+                colors: [Yi, tr, sr, hr, gr, _r, Sr, Lr, jr, Nr, Wr, Yr, ts, ss, hs, gs, _s, Ss],
                 styles: {}
-            }, On(Os);
-            const Ls = function(t) {
+            }, Ln(Ls);
+            const Os = function(t) {
                 return void 0 === t
             };
             var ks = n(1995),
-                Is = function() {
+                Rs = function() {
                     function t(t, e) {
                         for (var n = 0; n < e.length; n++) {
                             var i = e[n];
                             i.enumerable = i.enumerable || !1, i.configurable = !0, "value" in i && (i.writable = !0), Object.defineProperty(t, i.key, i)
                         }
                     }
                     return function(e, n, i) {
                         return n && t(e.prototype, n), i && t(e, i), e
                     }
                 }(),
-                Rs = function(t) {
+                Is = function(t) {
                     function e(t) {
                         ! function(t, e) {
                             if (!(t instanceof e)) throw new TypeError("Cannot call a class as a function")
                         }(this, e);
                         var n = function(t, e) {
                             if (!t) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
                             return !e || "object" != typeof e && "function" != typeof e ? t : e
@@ -3264,16 +3264,16 @@
                                 h: n.props.hsl.h,
                                 s: n.props.hsl.s,
                                 l: n.props.hsl.l,
                                 a: Math.round(100 * t.a) / 100,
                                 source: "rgb"
                             }, e)) : (t.h || t.s || t.l) && ("string" == typeof t.s && t.s.includes("%") && (t.s = t.s.replace("%", "")), "string" == typeof t.l && t.l.includes("%") && (t.l = t.l.replace("%", "")), 1 == t.s ? t.s = .01 : 1 == t.l && (t.l = .01), n.props.onChange({
                                 h: t.h || n.props.hsl.h,
-                                s: Number(Ls(t.s) ? n.props.hsl.s : t.s),
-                                l: Number(Ls(t.l) ? n.props.hsl.l : t.l),
+                                s: Number(Os(t.s) ? n.props.hsl.s : t.s),
+                                l: Number(Os(t.l) ? n.props.hsl.l : t.l),
                                 source: "hsl"
                             }, e))
                         }, n.showHighlight = function(t) {
                             t.currentTarget.style.background = "#eee"
                         }, n.hideHighlight = function(t) {
                             t.currentTarget.style.background = "transparent"
                         }, 1 !== t.hsl.a && "hex" === t.view ? n.state = {
@@ -3288,15 +3288,15 @@
                             constructor: {
                                 value: t,
                                 enumerable: !1,
                                 writable: !0,
                                 configurable: !0
                             }
                         }), e && (Object.setPrototypeOf ? Object.setPrototypeOf(t, e) : t.__proto__ = e)
-                    }(e, t), Is(e, [{
+                    }(e, t), Rs(e, [{
                         key: "render",
                         value: function() {
                             var t = this,
                                 e = (0, p.ZP)({
                                     default: {
                                         wrap: {
                                             paddingTop: "16px",
@@ -3494,19 +3494,19 @@
                         value: function(t, e) {
                             return 1 !== t.hsl.a && "hex" === e.view ? {
                                 view: "rgb"
                             } : null
                         }
                     }]), e
                 }(h().Component);
-            Rs.defaultProps = {
+            Is.defaultProps = {
                 view: "hex"
             };
-            const js = Rs,
-                zs = function() {
+            const js = Is,
+                Fs = function() {
                     var t = (0, p.ZP)({
                         default: {
                             picker: {
                                 width: "12px",
                                 height: "12px",
                                 borderRadius: "6px",
                                 transform: "translate(-6px, -1px)",
@@ -3515,15 +3515,15 @@
                             }
                         }
                     });
                     return h().createElement("div", {
                         style: t.picker
                     })
                 },
-                Fs = function() {
+                zs = function() {
                     var t = (0, p.ZP)({
                         default: {
                             picker: {
                                 width: "12px",
                                 height: "12px",
                                 borderRadius: "6px",
                                 boxShadow: "inset 0 0 0 1px #fff",
@@ -3632,19 +3632,19 @@
                         disableAlpha: i
                     });
                 return h().createElement("div", {
                     style: m.picker,
                     className: "chrome-picker " + f
                 }, h().createElement("div", {
                     style: m.saturation
-                }, h().createElement(Re, {
+                }, h().createElement(Ie, {
                     style: m.Saturation,
                     hsl: s,
                     hsv: o,
-                    pointer: Fs,
+                    pointer: zs,
                     onChange: n
                 })), h().createElement("div", {
                     style: m.body
                 }, h().createElement("div", {
                     style: m.controls,
                     className: "flexbox-fix"
                 }, h().createElement("div", {
@@ -3658,44 +3658,44 @@
                 }))), h().createElement("div", {
                     style: m.toggles
                 }, h().createElement("div", {
                     style: m.hue
                 }, h().createElement(M, {
                     style: m.Hue,
                     hsl: s,
-                    pointer: zs,
+                    pointer: Fs,
                     onChange: n
                 })), h().createElement("div", {
                     style: m.alpha
                 }, h().createElement(w, {
                     style: m.Alpha,
                     rgb: r,
                     hsl: s,
-                    pointer: zs,
+                    pointer: Fs,
                     renderers: l,
                     onChange: n
                 })))), h().createElement(js, {
                     rgb: r,
                     hsl: s,
                     hex: a,
                     view: g,
                     onChange: n,
                     disableAlpha: i
                 })))
             };
             Bs.propTypes = {
-                width: L().oneOfType([L().string, L().number]),
-                disableAlpha: L().bool,
-                styles: L().object,
-                defaultView: L().oneOf(["hex", "rgb", "hsl"])
+                width: O().oneOfType([O().string, O().number]),
+                disableAlpha: O().bool,
+                styles: O().object,
+                defaultView: O().oneOf(["hex", "rgb", "hsl"])
             }, Bs.defaultProps = {
                 width: 225,
                 disableAlpha: !1,
                 styles: {}
-            }, On(Bs);
+            }, Ln(Bs);
             const Ds = function(t) {
                     var e = t.color,
                         n = t.onClick,
                         i = void 0 === n ? function() {} : n,
                         r = t.onSwatchHover,
                         s = t.active,
                         o = (0, p.ZP)({
@@ -3922,20 +3922,20 @@
                 })), h().createElement(Ns, {
                     hex: r,
                     rgb: s,
                     onChange: d
                 })))
             };
             Vs.propTypes = {
-                colors: L().arrayOf(L().string),
-                styles: L().object
+                colors: O().arrayOf(O().string),
+                styles: O().object
             }, Vs.defaultProps = {
                 colors: ["#4D4D4D", "#999999", "#FFFFFF", "#F44E3B", "#FE9200", "#FCDC00", "#DBDF00", "#A4DD00", "#68CCCA", "#73D8FF", "#AEA1FF", "#FDA1FF", "#333333", "#808080", "#cccccc", "#D33115", "#E27300", "#FCC400", "#B0BC00", "#68BC00", "#16A5A5", "#009CE0", "#7B64FF", "#FA28FF", "#000000", "#666666", "#B3B3B3", "#9F0500", "#C45100", "#FB9E00", "#808900", "#194D33", "#0C797D", "#0062B1", "#653294", "#AB149E"],
                 styles: {}
-            }, On(Vs);
+            }, Ln(Vs);
             const Us = (0, p.tz)((function(t) {
                 var e = t.hover,
                     n = t.color,
                     i = t.onClick,
                     r = t.onSwatchHover,
                     s = {
                         position: "relative",
@@ -4078,24 +4078,24 @@
                         key: t,
                         onClick: d,
                         onSwatchHover: r
                     })
                 })))
             };
             Gs.propTypes = {
-                width: L().oneOfType([L().string, L().number]),
-                colors: L().arrayOf(L().string),
-                triangle: L().oneOf(["hide", "top-left", "top-right", "bottom-left", "bottom-right"]),
-                styles: L().object
+                width: O().oneOfType([O().string, O().number]),
+                colors: O().arrayOf(O().string),
+                triangle: O().oneOf(["hide", "top-left", "top-right", "bottom-left", "bottom-right"]),
+                styles: O().object
             }, Gs.defaultProps = {
                 width: 200,
                 colors: ["#B80000", "#DB3E00", "#FCCB00", "#008B02", "#006B76", "#1273DE", "#004DCF", "#5300EB", "#EB9694", "#FAD0C3", "#FEF3BD", "#C1E1C5", "#BEDADC", "#C4DEF6", "#BED3F3", "#D4C4FB"],
                 triangle: "top-left",
                 styles: {}
-            }, On(Gs);
+            }, Ln(Gs);
             var Ws = Object.assign || function(t) {
                     for (var e = 1; e < arguments.length; e++) {
                         var n = arguments[e];
                         for (var i in n) Object.prototype.hasOwnProperty.call(n, i) && (t[i] = n[i])
                     }
                     return t
                 },
@@ -4136,15 +4136,15 @@
                                 s: 1
                             })
                         },
                         direction: s
                     })))
                 };
             Hs.propTypes = {
-                styles: L().object
+                styles: O().object
             }, Hs.defaultProps = {
                 width: "316px",
                 height: "16px",
                 direction: "horizontal",
                 pointer: function(t) {
                     var e = t.direction,
                         n = (0, p.ZP)({
@@ -4167,15 +4167,15 @@
                             vertical: "vertical" === e
                         });
                     return h().createElement("div", {
                         style: n.picker
                     })
                 },
                 styles: {}
-            }, On(Hs), On((function(t) {
+            }, Ln(Hs), Ln((function(t) {
                 var e = t.onChange,
                     n = t.hex,
                     i = t.rgb,
                     r = t.styles,
                     s = void 0 === r ? {} : r,
                     o = t.className,
                     a = void 0 === o ? "" : o,
@@ -4623,26 +4623,26 @@
                         style: i.new
                     }), h().createElement("div", {
                         style: i.current
                     })), h().createElement("div", {
                         style: i.label
                     }, "current"))
                 };
-            var $s = function() {
+            var Js = function() {
                     function t(t, e) {
                         for (var n = 0; n < e.length; n++) {
                             var i = e[n];
                             i.enumerable = i.enumerable || !1, i.configurable = !0, "value" in i && (i.writable = !0), Object.defineProperty(t, i.key, i)
                         }
                     }
                     return function(e, n, i) {
                         return n && t(e.prototype, n), i && t(e, i), e
                     }
                 }(),
-                Js = function(t) {
+                Qs = function(t) {
                     function e(t) {
                         ! function(t, e) {
                             if (!(t instanceof e)) throw new TypeError("Cannot call a class as a function")
                         }(this, e);
                         var n = function(t, e) {
                             if (!t) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
                             return !e || "object" != typeof e && "function" != typeof e ? t : e
@@ -4657,15 +4657,15 @@
                             constructor: {
                                 value: t,
                                 enumerable: !1,
                                 writable: !0,
                                 configurable: !0
                             }
                         }), e && (Object.setPrototypeOf ? Object.setPrototypeOf(t, e) : t.__proto__ = e)
-                    }(e, t), $s(e, [{
+                    }(e, t), Js(e, [{
                         key: "render",
                         value: function() {
                             var t = this.props,
                                 e = t.styles,
                                 n = void 0 === e ? {} : e,
                                 i = t.className,
                                 r = void 0 === i ? "" : i,
@@ -4731,15 +4731,15 @@
                             }, h().createElement("div", {
                                 style: s.head
                             }, this.props.header), h().createElement("div", {
                                 style: s.body,
                                 className: "flexbox-fix"
                             }, h().createElement("div", {
                                 style: s.saturation
-                            }, h().createElement(Re, {
+                            }, h().createElement(Ie, {
                                 hsl: this.props.hsl,
                                 hsv: this.props.hsv,
                                 pointer: qs,
                                 onChange: this.props.onChange
                             })), h().createElement("div", {
                                 style: s.hue
                             }, h().createElement(M, {
@@ -4771,22 +4771,22 @@
                                 rgb: this.props.rgb,
                                 hsv: this.props.hsv,
                                 hex: this.props.hex
                             }))))))
                         }
                     }]), e
                 }(h().Component);
-            Js.propTypes = {
-                header: L().string,
-                styles: L().object
-            }, Js.defaultProps = {
+            Qs.propTypes = {
+                header: O().string,
+                styles: O().object
+            }, Qs.defaultProps = {
                 header: "Color Picker",
                 styles: {}
-            }, On(Js);
-            const Qs = function(t) {
+            }, Ln(Qs);
+            const $s = function(t) {
                 var e = t.onChange,
                     n = t.rgb,
                     i = t.hsl,
                     r = t.hex,
                     s = t.disableAlpha,
                     o = (0, p.ZP)({
                         default: {
@@ -4975,17 +4975,17 @@
                             focusStyle: {
                                 boxShadow: "inset 0 0 0 1px rgba(0,0,0,.15), 0 0 4px " + e.color
                             }
                         })))
                     })))
                 };
             eo.propTypes = {
-                colors: L().arrayOf(L().oneOfType([L().string, L().shape({
-                    color: L().string,
-                    title: L().string
+                colors: O().arrayOf(O().oneOfType([O().string, O().shape({
+                    color: O().string,
+                    title: O().string
                 })])).isRequired
             };
             const no = eo;
             var io = Object.assign || function(t) {
                     for (var e = 1; e < arguments.length; e++) {
                         var n = arguments[e];
                         for (var i in n) Object.prototype.hasOwnProperty.call(n, i) && (t[i] = n[i])
@@ -5083,15 +5083,15 @@
                             disableAlpha: l
                         });
                     return h().createElement("div", {
                         style: v.picker,
                         className: "sketch-picker " + m
                     }, h().createElement("div", {
                         style: v.saturation
-                    }, h().createElement(Re, {
+                    }, h().createElement(Ie, {
                         style: v.Saturation,
                         hsl: s,
                         hsv: r,
                         onChange: o
                     })), h().createElement("div", {
                         style: v.controls,
                         className: "flexbox-fix"
@@ -5111,37 +5111,37 @@
                         hsl: s,
                         renderers: u,
                         onChange: o
                     }))), h().createElement("div", {
                         style: v.color
                     }, h().createElement(b, null), h().createElement("div", {
                         style: v.activeColor
-                    }))), h().createElement(Qs, {
+                    }))), h().createElement($s, {
                         rgb: n,
                         hsl: s,
                         hex: i,
                         onChange: o,
                         disableAlpha: l
                     }), h().createElement(no, {
                         colors: c,
                         onClick: o,
                         onSwatchHover: a
                     }))
                 };
             ro.propTypes = {
-                disableAlpha: L().bool,
-                width: L().oneOfType([L().string, L().number]),
-                styles: L().object
+                disableAlpha: O().bool,
+                width: O().oneOfType([O().string, O().number]),
+                styles: O().object
             }, ro.defaultProps = {
                 disableAlpha: !1,
                 width: 200,
                 styles: {},
                 presetColors: ["#D0021B", "#F5A623", "#F8E71C", "#8B572A", "#7ED321", "#417505", "#BD10E0", "#9013FE", "#4A90E2", "#50E3C2", "#B8E986", "#000000", "#4A4A4A", "#9B9B9B", "#FFFFFF"]
             };
-            const so = On(ro),
+            const so = Ln(ro),
                 oo = function(t) {
                     var e = t.hsl,
                         n = t.offset,
                         i = t.onClick,
                         r = void 0 === i ? function() {} : i,
                         s = t.active,
                         o = t.first,
@@ -5283,15 +5283,15 @@
                     style: l.swatches
                 }, h().createElement(ao, {
                     hsl: e,
                     onClick: n
                 })))
             };
             lo.propTypes = {
-                styles: L().object
+                styles: O().object
             }, lo.defaultProps = {
                 pointer: function() {
                     var t = (0, p.ZP)({
                         default: {
                             picker: {
                                 width: "14px",
                                 height: "14px",
@@ -5303,15 +5303,15 @@
                         }
                     });
                     return h().createElement("div", {
                         style: t.picker
                     })
                 },
                 styles: {}
-            }, On(lo);
+            }, Ln(lo);
             var co = n(597);
             const ho = function(t) {
                     var e = t.color,
                         n = t.onClick,
                         i = void 0 === n ? function() {} : n,
                         r = t.onSwatchHover,
                         s = t.first,
@@ -5461,44 +5461,44 @@
                         onSwatchHover: r
                     })
                 })), h().createElement("div", {
                     style: d.clear
                 })))))
             };
             po.propTypes = {
-                width: L().oneOfType([L().string, L().number]),
-                height: L().oneOfType([L().string, L().number]),
-                colors: L().arrayOf(L().arrayOf(L().string)),
-                styles: L().object
+                width: O().oneOfType([O().string, O().number]),
+                height: O().oneOfType([O().string, O().number]),
+                colors: O().arrayOf(O().arrayOf(O().string)),
+                styles: O().object
             }, po.defaultProps = {
                 width: 320,
                 height: 240,
                 colors: [
-                    [$i, Ki, Yi, Xi, qi],
-                    [nr, er, tr, Qi, Ji],
+                    [Ji, Ki, Yi, Xi, qi],
+                    [nr, er, tr, $i, Qi],
                     [ar, or, sr, rr, ir],
                     [dr, ur, hr, cr, lr],
                     [vr, mr, gr, fr, pr],
                     [wr, xr, _r, yr, br],
                     [Tr, Cr, Sr, Pr, Er],
-                    [kr, Lr, Or, Mr, Ar],
-                    [Fr, zr, jr, Rr, Ir],
+                    [kr, Or, Lr, Mr, Ar],
+                    [zr, Fr, jr, Ir, Rr],
                     ["#194D33", Vr, Nr, Dr, Br],
                     [Zr, Hr, Wr, Gr, Ur],
-                    [$r, Kr, Yr, Xr, qr],
-                    [ns, es, ts, Qr, Jr],
+                    [Jr, Kr, Yr, Xr, qr],
+                    [ns, es, ts, $r, Qr],
                     [as, os, ss, rs, is],
                     [ds, us, hs, cs, ls],
                     [vs, ms, gs, fs, ps],
                     [ws, xs, _s, ys, bs],
                     [Ts, Cs, Ss, Ps, Es],
                     ["#000000", "#525252", "#969696", "#D9D9D9", "#FFFFFF"]
                 ],
                 styles: {}
-            }, On(po);
+            }, Ln(po);
             var fo = function(t) {
                 var e = t.onChange,
                     n = t.onSwatchHover,
                     i = t.hex,
                     r = t.colors,
                     s = t.width,
                     o = t.triangle,
@@ -5644,24 +5644,24 @@
                     value: i.replace("#", ""),
                     onChange: f
                 }), h().createElement("div", {
                     style: d.clear
                 })))
             };
             fo.propTypes = {
-                width: L().oneOfType([L().string, L().number]),
-                triangle: L().oneOf(["hide", "top-left", "top-right"]),
-                colors: L().arrayOf(L().string),
-                styles: L().object
+                width: O().oneOfType([O().string, O().number]),
+                triangle: O().oneOf(["hide", "top-left", "top-right"]),
+                colors: O().arrayOf(O().string),
+                styles: O().object
             }, fo.defaultProps = {
                 width: 276,
                 colors: ["#FF6900", "#FCB900", "#7BDCB5", "#00D084", "#8ED1FC", "#0693E3", "#ABB8C3", "#EB144C", "#F78DA7", "#9900EF"],
                 triangle: "top-left",
                 styles: {}
-            }, On(fo);
+            }, Ln(fo);
             var go = function(t) {
                 var e = (0, p.ZP)({
                     default: {
                         picker: {
                             width: "20px",
                             height: "20px",
                             borderRadius: "22px",
@@ -5672,19 +5672,19 @@
                     }
                 });
                 return h().createElement("div", {
                     style: e.picker
                 })
             };
             go.propTypes = {
-                hsl: L().shape({
-                    h: L().number,
-                    s: L().number,
-                    l: L().number,
-                    a: L().number
+                hsl: O().shape({
+                    h: O().number,
+                    s: O().number,
+                    l: O().number,
+                    a: O().number
                 })
             }, go.defaultProps = {
                 hsl: {
                     a: 1,
                     h: 249.94,
                     l: .2,
                     s: .5
@@ -5705,19 +5705,19 @@
                     }
                 });
                 return h().createElement("div", {
                     style: e.picker
                 })
             };
             vo.propTypes = {
-                hsl: L().shape({
-                    h: L().number,
-                    s: L().number,
-                    l: L().number,
-                    a: L().number
+                hsl: O().shape({
+                    h: O().number,
+                    s: O().number,
+                    l: O().number,
+                    a: O().number
                 })
             }, vo.defaultProps = {
                 hsl: {
                     a: 1,
                     h: 249.94,
                     l: .2,
                     s: .5
@@ -5967,15 +5967,15 @@
                     className: "google-picker " + d
                 }, h().createElement("div", {
                     style: f.head
                 }, a), h().createElement("div", {
                     style: f.swatch
                 }), h().createElement("div", {
                     style: f.saturation
-                }, h().createElement(Re, {
+                }, h().createElement(Ie, {
                     hsl: r,
                     hsv: s,
                     pointer: mo,
                     onChange: n
                 })), h().createElement("div", {
                     style: f.body
                 }, h().createElement("div", {
@@ -6023,22 +6023,22 @@
                     value: n,
                     enumerable: !0,
                     configurable: !0,
                     writable: !0
                 }) : t[e] = n, t
             }
             _o.propTypes = {
-                width: L().oneOfType([L().string, L().number]),
-                styles: L().object,
-                header: L().string
+                width: O().oneOfType([O().string, O().number]),
+                styles: O().object,
+                header: O().string
             }, _o.defaultProps = {
                 width: 652,
                 styles: {},
                 header: "Color picker"
-            }, On(_o);
+            }, Ln(_o);
             let Eo = 1,
                 Po = 1;
             class So {
                 constructor() {
                     this.time = 0, this.channels = new Map, this.animations = new Map, this.playing = !1, this.lastEngineTime = -1
                 }
                 addChannel(t) {
@@ -6109,30 +6109,30 @@
                     n >= t.duration * t.repeat ? t.time = t.duration * t.rate : (t.time = Math.max(0, n) % t.duration, t.time *= t.rate)
                 }
             }
             const Co = Symbol.for("component"),
                 To = Symbol.for("asyncPropDefaults"),
                 Ao = Symbol.for("asyncPropOriginal"),
                 Mo = Symbol.for("asyncPropResolved");
-            var Oo = n(4155);
+            var Lo = n(4155);
 
-            function Lo(t) {
+            function Oo(t) {
                 if ("undefined" != typeof window && "object" == typeof window.process && "renderer" === window.process.type) return !0;
-                if (void 0 !== Oo && "object" == typeof Oo.versions && Boolean(Oo.versions.electron)) return !0;
+                if (void 0 !== Lo && "object" == typeof Lo.versions && Boolean(Lo.versions.electron)) return !0;
                 const e = "object" == typeof navigator && "string" == typeof navigator.userAgent && navigator.userAgent,
                     n = t || e;
                 return !!(n && n.indexOf("Electron") >= 0)
             }
             var ko = n(4155);
 
-            function Io() {
-                return !("object" == typeof ko && "[object process]" === String(ko) && !ko.browser) || Lo()
+            function Ro() {
+                return !("object" == typeof ko && "[object process]" === String(ko) && !ko.browser) || Oo()
             }
-            const Ro = "undefined" != typeof __VERSION__ ? __VERSION__ : "untranspiled source";
-            Io();
+            const Io = "undefined" != typeof __VERSION__ ? __VERSION__ : "untranspiled source";
+            Ro();
             class jo {
                 constructor(t, e) {
                     let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : "sessionStorage";
                     wo(this, "storage", void 0), wo(this, "id", void 0), wo(this, "config", void 0), this.storage = function(t) {
                         try {
                             const e = window[t],
                                 n = "__storage_test__";
@@ -6157,58 +6157,59 @@
                         const e = this.storage.getItem(this.id);
                         t = e ? JSON.parse(e) : {}
                     }
                     return Object.assign(this.config, t), this
                 }
             }
 
-            function zo(t, e, n) {
+            function Fo(t, e, n) {
                 let i = arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : 600;
                 const r = t.src.replace(/\(/g, "%28").replace(/\)/g, "%29");
                 t.width > i && (n = Math.min(n, i / t.width));
                 const s = t.width * n,
                     o = t.height * n,
                     a = ["font-size:1px;", "padding:".concat(Math.floor(o / 2), "px ").concat(Math.floor(s / 2), "px;"), "line-height:".concat(o, "px;"), "background:url(".concat(r, ");"), "background-size:".concat(s, "px ").concat(o, "px;"), "color:transparent;"].join("");
                 return ["".concat(e, " %c+"), a]
             }
-            let Fo;
+            let zo;
 
             function Bo(t) {
-                return "string" == typeof t ? Fo[t.toUpperCase()] || Fo.WHITE : t
+                return "string" == typeof t ? zo[t.toUpperCase()] || zo.WHITE : t
             }
 
             function Do(t, e) {
                 if (!t) throw new Error(e || "Assertion failed")
             }! function(t) {
                 t[t.BLACK = 30] = "BLACK", t[t.RED = 31] = "RED", t[t.GREEN = 32] = "GREEN", t[t.YELLOW = 33] = "YELLOW", t[t.BLUE = 34] = "BLUE", t[t.MAGENTA = 35] = "MAGENTA", t[t.CYAN = 36] = "CYAN", t[t.WHITE = 37] = "WHITE", t[t.BRIGHT_BLACK = 90] = "BRIGHT_BLACK", t[t.BRIGHT_RED = 91] = "BRIGHT_RED", t[t.BRIGHT_GREEN = 92] = "BRIGHT_GREEN", t[t.BRIGHT_YELLOW = 93] = "BRIGHT_YELLOW", t[t.BRIGHT_BLUE = 94] = "BRIGHT_BLUE", t[t.BRIGHT_MAGENTA = 95] = "BRIGHT_MAGENTA", t[t.BRIGHT_CYAN = 96] = "BRIGHT_CYAN", t[t.BRIGHT_WHITE = 97] = "BRIGHT_WHITE"
-            }(Fo || (Fo = {}));
+            }(zo || (zo = {}));
             var No = n(4155);
             const Vo = {
                     self: "undefined" != typeof self && self,
                     window: "undefined" != typeof window && window,
                     global: void 0 !== n.g && n.g,
                     document: "undefined" != typeof document && document,
                     process: "object" == typeof No && No
                 },
-                Uo = Vo.window || Vo.self || Vo.global,
+                Uo = (globalThis, Vo.window || Vo.self || Vo.global),
                 Go = Vo.process || {};
 
             function Wo() {
                 let t;
                 var e, n;
-                if (Io && "performance" in Uo) t = null == Uo || null === (e = Uo.performance) || void 0 === e || null === (n = e.now) || void 0 === n ? void 0 : n.call(e);
+                if (Ro && "performance" in Uo) t = null == Uo || null === (e = Uo.performance) || void 0 === e || null === (n = e.now) || void 0 === n ? void 0 : n.call(e);
                 else if ("hrtime" in Go) {
                     var i;
                     const e = null == Go || null === (i = Go.hrtime) || void 0 === i ? void 0 : i.call(Go);
                     t = 1e3 * e[0] + e[1] / 1e6
                 } else t = Date.now();
                 return t
             }
+            console;
             const Ho = {
-                    debug: Io && console.debug || console.log,
+                    debug: Ro && console.debug || console.log,
                     log: console.log,
                     info: console.info,
                     warn: console.warn,
                     error: console.error
                 },
                 Zo = {
                     enabled: !0,
@@ -6223,15 +6224,15 @@
             class Ko {
                 constructor() {
                     let {
                         id: t
                     } = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {
                         id: ""
                     };
-                    wo(this, "id", void 0), wo(this, "VERSION", Ro), wo(this, "_startTs", Wo()), wo(this, "_deltaTs", Wo()), wo(this, "_storage", void 0), wo(this, "userData", {}), wo(this, "LOG_THROTTLE_TIMEOUT", 0), this.id = t, this.userData = {}, this._storage = new jo("__probe-".concat(this.id, "__"), Zo), this.timeStamp("".concat(this.id, " started")),
+                    wo(this, "id", void 0), wo(this, "VERSION", Io), wo(this, "_startTs", Wo()), wo(this, "_deltaTs", Wo()), wo(this, "_storage", void 0), wo(this, "userData", {}), wo(this, "LOG_THROTTLE_TIMEOUT", 0), this.id = t, this.userData = {}, this._storage = new jo("__probe-".concat(this.id, "__"), Zo), this.timeStamp("".concat(this.id, " started")),
                         function(t) {
                             let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : ["constructor"];
                             const n = Object.getPrototypeOf(t),
                                 i = Object.getOwnPropertyNames(n);
                             for (const n of i) "function" == typeof t[n] && (e.find((t => n === t)) || (t[n] = t[n].bind(t)))
                         }(this), Object.seal(this)
                 }
@@ -6313,43 +6314,43 @@
                 }
                 once(t, e) {
                     for (var n = arguments.length, i = new Array(n > 2 ? n - 2 : 0), r = 2; r < n; r++) i[r - 2] = arguments[r];
                     return this._getLogFunction(t, e, Ho.debug || Ho.info, arguments, Yo)
                 }
                 table(t, e, n) {
                     return e ? this._getLogFunction(t, e, console.table || qo, n && [n], {
-                        tag: Qo(e)
+                        tag: $o(e)
                     }) : qo
                 }
                 image(t) {
                     let {
                         logLevel: e,
                         priority: n,
                         image: i,
                         message: r = "",
                         scale: s = 1
                     } = t;
-                    return this._shouldLog(e || n) ? Io ? function(t) {
+                    return this._shouldLog(e || n) ? Ro ? function(t) {
                         let {
                             image: e,
                             message: n = "",
                             scale: i = 1
                         } = t;
                         if ("string" == typeof e) {
                             const t = new Image;
                             return t.onload = () => {
-                                const e = zo(t, n, i);
+                                const e = Fo(t, n, i);
                                 console.log(...e)
                             }, t.src = e, qo
                         }
                         const r = e.nodeName || "";
-                        if ("img" === r.toLowerCase()) return console.log(...zo(e, n, i)), qo;
+                        if ("img" === r.toLowerCase()) return console.log(...Fo(e, n, i)), qo;
                         if ("canvas" === r.toLowerCase()) {
                             const t = new Image;
-                            return t.onload = () => console.log(...zo(t, n, i)), t.src = e.toDataURL(), qo
+                            return t.onload = () => console.log(...Fo(t, n, i)), t.src = e.toDataURL(), qo
                         }
                         return qo
                     }({
                         image: i,
                         message: r,
                         scale: s
                     }) : function(t) {
@@ -6374,15 +6375,15 @@
                 timeStamp(t, e) {
                     return this._getLogFunction(t, e, console.timeStamp || qo)
                 }
                 group(t, e) {
                     let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : {
                         collapsed: !1
                     };
-                    const i = Jo({
+                    const i = Qo({
                             logLevel: t,
                             message: e,
                             opts: n
                         }),
                         {
                             collapsed: r
                         } = n;
@@ -6405,19 +6406,19 @@
                         this.groupEnd(t)()
                     }
                 }
                 trace() {
                     console.trace && console.trace()
                 }
                 _shouldLog(t) {
-                    return this.isEnabled() && this.getLevel() >= $o(t)
+                    return this.isEnabled() && this.getLevel() >= Jo(t)
                 }
                 _getLogFunction(t, e, n, i, r) {
                     if (this._shouldLog(t)) {
-                        r = Jo({
+                        r = Qo({
                             logLevel: t,
                             message: e,
                             args: i,
                             opts: r
                         }), Do(n = n || r.method), r.total = this.getTotal(), r.delta = this.getDelta(), this._deltaTs = Wo();
                         const s = r.tag || r.message;
                         if (r.once) {
@@ -6430,25 +6431,25 @@
                                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 8;
                                     const n = Math.max(e - t.length, 0);
                                     return "".concat(" ".repeat(n)).concat(t)
                                 }(function(t) {
                                     let e;
                                     return e = t < 10 ? "".concat(t.toFixed(2), "ms") : t < 100 ? "".concat(t.toFixed(1), "ms") : t < 1e3 ? "".concat(t.toFixed(0), "ms") : "".concat((t / 1e3).toFixed(2), "s"), e
                                 }(n.total)) : "";
-                                i = e = n.time ? "".concat(t, ": ").concat(o, "  ").concat(e) : "".concat(t, ": ").concat(e), r = n.color, s = n.background, Io || "string" != typeof i || (r && (r = Bo(r), i = "[".concat(r, "m").concat(i, "[39m")), s && (r = Bo(s), i = "[".concat(s + 10, "m").concat(i, "[49m"))), e = i
+                                i = e = n.time ? "".concat(t, ": ").concat(o, "  ").concat(e) : "".concat(t, ": ").concat(e), r = n.color, s = n.background, Ro || "string" != typeof i || (r && (r = Bo(r), i = "[".concat(r, "m").concat(i, "[39m")), s && (r = Bo(s), i = "[".concat(s + 10, "m").concat(i, "[49m"))), e = i
                             }
                             var i, r, s;
                             return e
                         }(this.id, r.message, r), n.bind(console, e, ...r.args)
                     }
                     return qo
                 }
             }
 
-            function $o(t) {
+            function Jo(t) {
                 if (!t) return 0;
                 let e;
                 switch (typeof t) {
                     case "number":
                         e = t;
                         break;
                     case "object":
@@ -6456,20 +6457,20 @@
                         break;
                     default:
                         return 0
                 }
                 return Do(Number.isFinite(e) && e >= 0), e
             }
 
-            function Jo(t) {
+            function Qo(t) {
                 const {
                     logLevel: e,
                     message: n
                 } = t;
-                t.logLevel = $o(e);
+                t.logLevel = Jo(e);
                 const i = t.args ? Array.from(t.args) : [];
                 for (; i.length && i.shift() !== n;);
                 switch (typeof e) {
                     case "string":
                     case "function":
                         void 0 !== n && i.unshift(n), t.message = e;
                         break;
@@ -6479,20 +6480,20 @@
                 "function" == typeof t.message && (t.message = t.message());
                 const r = typeof t.message;
                 return Do("string" === r || "object" === r), Object.assign(t, {
                     args: i
                 }, t.opts)
             }
 
-            function Qo(t) {
+            function $o(t) {
                 for (const e in t)
                     for (const n in t[e]) return n || "untitled";
                 return "empty"
             }
-            wo(Ko, "VERSION", Ro);
+            wo(Ko, "VERSION", Io);
             const ta = new Ko({
                 id: "deck"
             });
             let ea = {};
 
             function na(t, e, n, i) {
                 ta.level > 0 && ea[t] && ea[t].call(null, e, n, i)
@@ -6677,35 +6678,35 @@
                 return t.replace(Ta, "")
             }
 
             function Ma(t) {
                 return ga(t) ? t.url : ma(t) ? t.name || "" : "string" == typeof t ? t : ""
             }
 
-            function Oa(t) {
+            function La(t) {
                 if (ga(t)) {
                     const e = t,
                         n = e.headers.get("content-type") || "",
                         i = Aa(e.url);
                     return function(t) {
                         const e = Sa.exec(t);
                         return e ? e[1] : t
                     }(n) || Ca(i)
                 }
                 return ma(t) ? t.type || "" : "string" == typeof t ? Ca(t) : ""
             }
-            async function La(t) {
+            async function Oa(t) {
                 if (ga(t)) return t;
                 const e = {},
                     n = function(t) {
                         return ga(t) ? t.headers["content-length"] || -1 : ma(t) ? t.size : "string" == typeof t ? t.length : t instanceof ArrayBuffer || ArrayBuffer.isView(t) ? t.byteLength : -1
                     }(t);
                 n >= 0 && (e["content-length"] = String(n));
                 const i = Ma(t),
-                    r = Oa(t);
+                    r = La(t);
                 r && (e["content-type"] = r);
                 const s = await async function(t) {
                     if ("string" == typeof t) return "data:,".concat(t.slice(0, 5));
                     if (t instanceof Blob) {
                         const e = t.slice(0, 5);
                         return await new Promise((t => {
                             const n = new FileReader;
@@ -6742,33 +6743,33 @@
                                 const n = Ea[e];
                                 t = t.replace(e, n)
                             } return t.startsWith("http://") || t.startsWith("https://") || (t = "".concat(wa).concat(t)), t
                     }(t);
                     let n = e;
                     return null != e && e.fetch && "function" != typeof(null == e ? void 0 : e.fetch) && (n = e.fetch), await fetch(t, n)
                 }
-                return await La(t)
+                return await Oa(t)
             }
-            var Ia = n(4155),
-                Ra = n(4155);
+            var Ra = n(4155),
+                Ia = n(4155);
 
             function ja() {
-                return !("object" == typeof Ra && "[object process]" === String(Ra) && !Ra.browser) || function(t) {
+                return !("object" == typeof Ia && "[object process]" === String(Ia) && !Ia.browser) || function(t) {
                     if ("undefined" != typeof window && "object" == typeof window.process && "renderer" === window.process.type) return !0;
-                    if (void 0 !== Ia && "object" == typeof Ia.versions && Boolean(Ia.versions.electron)) return !0;
+                    if (void 0 !== Ra && "object" == typeof Ra.versions && Boolean(Ra.versions.electron)) return !0;
                     const e = "object" == typeof navigator && "string" == typeof navigator.userAgent && navigator.userAgent;
                     return !!(e && e.indexOf("Electron") >= 0)
                 }()
             }
-            const za = "undefined" != typeof __VERSION__ ? __VERSION__ : "untranspiled source";
+            const Fa = "undefined" != typeof __VERSION__ ? __VERSION__ : "untranspiled source";
             ja();
-            class Fa {
+            class za {
                 constructor(t, e) {
                     let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : "sessionStorage";
-                    this.storage = void 0, this.id = void 0, this.config = void 0, this.storage = function(t) {
+                    wo(this, "storage", void 0), wo(this, "id", void 0), wo(this, "config", void 0), this.storage = function(t) {
                         try {
                             const e = window[t],
                                 n = "__storage_test__";
                             return e.setItem(n, n), e.removeItem(n), e
                         } catch (t) {
                             return null
                         }
@@ -6810,15 +6811,15 @@
             function Na(t) {
                 return "string" != typeof t ? t : (t = t.toUpperCase(), Da[t] || Da.WHITE)
             }
 
             function Va(t, e) {
                 if (!t) throw new Error(e || "Assertion failed")
             }
-            globalThis.self || globalThis.window || globalThis.global;
+            globalThis, globalThis.self || globalThis.window || globalThis.global;
             const Ua = globalThis.window || globalThis.self || globalThis.global,
                 Ga = (globalThis.document, globalThis.process || {});
 
             function Wa() {
                 let t;
                 var e, n;
                 if (ja() && Ua.performance) t = null == Ua || null === (e = Ua.performance) || void 0 === e || null === (n = e.now) || void 0 === n ? void 0 : n.call(e);
@@ -6850,15 +6851,15 @@
             class Ka {
                 constructor() {
                     let {
                         id: t
                     } = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {
                         id: ""
                     };
-                    this.id = void 0, this.VERSION = za, this._startTs = Wa(), this._deltaTs = Wa(), this._storage = void 0, this.userData = {}, this.LOG_THROTTLE_TIMEOUT = 0, this.id = t, this.userData = {}, this._storage = new Fa("__probe-".concat(this.id, "__"), Za), this.timeStamp("".concat(this.id, " started")),
+                    wo(this, "id", void 0), wo(this, "VERSION", Fa), wo(this, "_startTs", Wa()), wo(this, "_deltaTs", Wa()), wo(this, "_storage", void 0), wo(this, "userData", {}), wo(this, "LOG_THROTTLE_TIMEOUT", 0), this.id = t, this.userData = {}, this._storage = new za("__probe-".concat(this.id, "__"), Za), this.timeStamp("".concat(this.id, " started")),
                         function(t) {
                             let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : ["constructor"];
                             const n = Object.getPrototypeOf(t),
                                 i = Object.getOwnPropertyNames(n),
                                 r = t;
                             for (const n of i) {
                                 const i = r[n];
@@ -6943,15 +6944,15 @@
                     return this._getLogFunction(t, e, console.info, arguments)
                 }
                 once(t, e) {
                     return this._getLogFunction(t, e, Ha.debug || Ha.info, arguments, Ya)
                 }
                 table(t, e, n) {
                     return e ? this._getLogFunction(t, e, console.table || qa, n && [n], {
-                        tag: Qa(e)
+                        tag: $a(e)
                     }) : qa
                 }
                 image(t) {
                     let {
                         logLevel: e,
                         priority: n,
                         image: i,
@@ -7004,15 +7005,15 @@
                 timeStamp(t, e) {
                     return this._getLogFunction(t, e, console.timeStamp || qa)
                 }
                 group(t, e) {
                     let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : {
                         collapsed: !1
                     };
-                    const i = Ja({
+                    const i = Qa({
                             logLevel: t,
                             message: e,
                             opts: n
                         }),
                         {
                             collapsed: r
                         } = n;
@@ -7035,19 +7036,19 @@
                         this.groupEnd(t)()
                     }
                 }
                 trace() {
                     console.trace && console.trace()
                 }
                 _shouldLog(t) {
-                    return this.isEnabled() && this.getLevel() >= $a(t)
+                    return this.isEnabled() && this.getLevel() >= Ja(t)
                 }
                 _getLogFunction(t, e, n, i, r) {
                     if (this._shouldLog(t)) {
-                        r = Ja({
+                        r = Qa({
                             logLevel: t,
                             message: e,
                             args: i,
                             opts: r
                         }), Va(n = n || r.method), r.total = this.getTotal(), r.delta = this.getDelta(), this._deltaTs = Wa();
                         const s = r.tag || r.message;
                         if (r.once && s) {
@@ -7081,15 +7082,15 @@
                             return e
                         }(this.id, r.message, r), n.bind(console, e, ...r.args)
                     }
                     return qa
                 }
             }
 
-            function $a(t) {
+            function Ja(t) {
                 if (!t) return 0;
                 let e;
                 switch (typeof t) {
                     case "number":
                         e = t;
                         break;
                     case "object":
@@ -7097,20 +7098,20 @@
                         break;
                     default:
                         return 0
                 }
                 return Va(Number.isFinite(e) && e >= 0), e
             }
 
-            function Ja(t) {
+            function Qa(t) {
                 const {
                     logLevel: e,
                     message: n
                 } = t;
-                t.logLevel = $a(e);
+                t.logLevel = Ja(e);
                 const i = t.args ? Array.from(t.args) : [];
                 for (; i.length && i.shift() !== n;);
                 switch (typeof e) {
                     case "string":
                     case "function":
                         void 0 !== n && i.unshift(n), t.message = e;
                         break;
@@ -7120,20 +7121,20 @@
                 "function" == typeof t.message && (t.message = t.message());
                 const r = typeof t.message;
                 return Va("string" === r || "object" === r), Object.assign(t, {
                     args: i
                 }, t.opts)
             }
 
-            function Qa(t) {
+            function $a(t) {
                 for (const e in t)
                     for (const n in t[e]) return n || "untitled";
                 return "empty"
             }
-            Ka.VERSION = za;
+            wo(Ka, "VERSION", Fa);
             const tl = new Ka({
                 id: "loaders.gl"
             });
             class el {
                 log() {
                     return () => {}
                 }
@@ -7526,25 +7527,25 @@
                         maxMobileConcurrency: this.props.maxMobileConcurrency,
                         reuseWorkers: this.props.reuseWorkers,
                         onDebug: this.props.onDebug
                     }
                 }
             }
             wo(Ml, "_workerFarm", void 0);
-            const Ol = "latest";
-            async function Ll(t, e, n, i, r) {
+            const Ll = "latest";
+            async function Ol(t, e, n, i, r) {
                 const s = t.id,
                     o = function(t) {
                         let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                         const n = e[t.id] || {},
                             i = "".concat(t.id, "-worker.js");
                         let r = n.workerUrl;
                         if (r || "compression" !== t.id || (r = e.workerUrl), "test" === e._workerType && (r = "modules/".concat(t.module, "/dist/").concat(i)), !r) {
                             let e = t.version;
-                            "latest" === e && (e = Ol);
+                            "latest" === e && (e = Ll);
                             const n = e ? "@".concat(e) : "";
                             r = "https://unpkg.com/@loaders.gl/".concat(t.module).concat(n, "/dist/").concat(i)
                         }
                         return fl(r), r
                     }(t, n),
                     a = Ml.getWorkerFarm(n).getWorkerPool({
                         name: s,
@@ -7586,51 +7587,51 @@
                             })
                         }
                         break;
                     default:
                         console.warn("parse-with-worker unknown message ".concat(n))
                 }
             }
-            const Il = 262144,
-                Rl = 262144,
+            const Rl = 262144,
+                Il = 262144,
                 jl = 1048576;
 
-            function zl(t) {
+            function Fl(t) {
                 if ((e = t) && "object" == typeof e && e.isBuffer) return t;
                 var e;
                 if (t instanceof ArrayBuffer) return t;
                 if (ArrayBuffer.isView(t)) return 0 === t.byteOffset && t.byteLength === t.buffer.byteLength ? t.buffer : t.buffer.slice(t.byteOffset, t.byteOffset + t.byteLength);
                 if ("string" == typeof t) {
                     const e = t;
                     return (new TextEncoder).encode(e).buffer
                 }
                 if (t && "object" == typeof t && t._toArrayBuffer) return t._toArrayBuffer();
                 throw new Error("toArrayBuffer")
             }
 
-            function Fl(t, e) {
+            function zl(t, e) {
                 return il ? async function*(t, e) {
                     const n = t.getReader();
                     let i;
                     try {
                         for (;;) {
                             const t = i || n.read();
                             null != e && e._streamReadAhead && (i = n.read());
                             const {
                                 done: r,
                                 value: s
                             } = await t;
                             if (r) return;
-                            yield zl(s)
+                            yield Fl(s)
                         }
                     } catch (t) {
                         n.releaseLock()
                     }
                 }(t, e): async function*(t, e) {
-                    for await (const e of t) yield zl(e)
+                    for await (const e of t) yield Fl(e)
                 }(t)
             }
             const Bl = "Cannot convert supplied data type";
             async function Dl(t, e, n) {
                 const i = t instanceof ArrayBuffer || ArrayBuffer.isView(t);
                 if ("string" == typeof t || i) return function(t, e, n) {
                     if (e.text && "string" == typeof t) return t;
@@ -7642,15 +7643,15 @@
                         if (e.text && !e.binary) return new TextDecoder("utf8").decode(t);
                         let n = t.buffer;
                         const i = t.byteLength || t.length;
                         return 0 === t.byteOffset && i === n.byteLength || (n = n.slice(t.byteOffset, t.byteOffset + i)), n
                     }
                     throw new Error(Bl)
                 }(t, e);
-                if (ma(t) && (t = await La(t)), ga(t)) {
+                if (ma(t) && (t = await Oa(t)), ga(t)) {
                     const n = t;
                     return await async function(t) {
                         if (!t.ok) {
                             const e = await async function(t) {
                                 let e = "Failed to fetch resource ".concat(t.url, " (").concat(t.status, "): ");
                                 try {
                                     const n = t.headers.get("Content-Type");
@@ -7661,28 +7662,28 @@
                             }(t);
                             throw new Error(e)
                         }
                     }(n), e.binary ? await n.arrayBuffer() : await n.text()
                 }
                 if (ba(t) && (t = function(t, e) {
                         if ("string" == typeof t) return function*(t, e) {
-                            const n = (null == e ? void 0 : e.chunkSize) || Il;
+                            const n = (null == e ? void 0 : e.chunkSize) || Rl;
                             let i = 0;
                             const r = new TextEncoder;
                             for (; i < t.length;) {
                                 const e = Math.min(t.length - i, n),
                                     s = t.slice(i, i + e);
                                 i += e, yield r.encode(s)
                             }
                         }(t, e);
                         if (t instanceof ArrayBuffer) return function(t) {
                             let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                             return function*() {
                                 const {
-                                    chunkSize: n = Rl
+                                    chunkSize: n = Il
                                 } = e;
                                 let i = 0;
                                 for (; i < t.byteLength;) {
                                     const e = Math.min(t.byteLength - i, n),
                                         r = new ArrayBuffer(e),
                                         s = new Uint8Array(t, i, e);
                                     new Uint8Array(r).set(s), i += e, yield r
@@ -7694,16 +7695,16 @@
                             let i = 0;
                             for (; i < t.size;) {
                                 const e = i + n,
                                     r = await t.slice(i, e).arrayBuffer();
                                 i = e, yield r
                             }
                         }(t, e);
-                        if (ba(t)) return Fl(t, e);
-                        if (ga(t)) return Fl(t.body, e);
+                        if (ba(t)) return zl(t, e);
+                        if (ga(t)) return zl(t.body, e);
                         throw new Error("makeIterator")
                     }(t, n)), pa(t) || fa(t)) return async function(t) {
                     const e = [];
                     for await (const n of t) e.push(n);
                     return function() {
                         for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
                         const i = e.map((t => t instanceof ArrayBuffer ? new Uint8Array(t) : t)),
@@ -7739,15 +7740,15 @@
                 let r = [];
                 e && (r = r.concat(e)), null != n && n.ignoreRegisteredLoaders || r.push(...Ul()),
                     function(t) {
                         for (const e of t) xa(e)
                     }(r);
                 const s = function(t, e, n, i) {
                     const r = Ma(t),
-                        s = Oa(t),
+                        s = La(t),
                         o = Aa(r) || (null == i ? void 0 : i.url);
                     let a = null,
                         l = "";
                     var c;
                     return null != n && n.mimeType && (a = ql(e, null == n ? void 0 : n.mimeType), l = "match forced by supplied MIME type ".concat(null == n ? void 0 : n.mimeType)), a = a || function(t, e) {
                         const n = e && Gl.exec(e),
                             i = n && n[1];
@@ -7775,15 +7776,15 @@
 
             function Hl(t) {
                 return !(t instanceof Response && 204 === t.status)
             }
 
             function Zl(t) {
                 const e = Ma(t),
-                    n = Oa(t);
+                    n = La(t);
                 let i = "No valid loader found (";
                 i += e ? "".concat(Nl(e), ", ") : "no url provided, ", i += "MIME type: ".concat(n ? '"'.concat(n, '"') : "not provided", ", ");
                 const r = t ? Kl(t) : "";
                 return i += r ? ' first bytes: "'.concat(r, '"') : "first bytes: not available", i += ")", i
             }
 
             function ql(t, e) {
@@ -7808,34 +7809,34 @@
                             if (i[t] !== r[t]) return !1;
                         return !0
                     }(i, t, i.byteLength);
                     switch (typeof i) {
                         case "function":
                             return i(t, n);
                         case "string":
-                            return i === $l(t, e, i.length);
+                            return i === Jl(t, e, i.length);
                         default:
                             return !1
                     }
                 }(t, e, n, i)))
             }
 
             function Kl(t) {
                 let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 5;
-                return "string" == typeof t ? t.slice(0, e) : ArrayBuffer.isView(t) ? $l(t.buffer, t.byteOffset, e) : t instanceof ArrayBuffer ? $l(t, 0, e) : ""
+                return "string" == typeof t ? t.slice(0, e) : ArrayBuffer.isView(t) ? Jl(t.buffer, t.byteOffset, e) : t instanceof ArrayBuffer ? Jl(t, 0, e) : ""
             }
 
-            function $l(t, e, n) {
+            function Jl(t, e, n) {
                 if (t.byteLength < e + n) return "";
                 const i = new DataView(t);
                 let r = "";
                 for (let t = 0; t < n; t++) r += String.fromCharCode(i.getUint8(e + t));
                 return r
             }
-            async function Jl(t, e, n, i) {
+            async function Ql(t, e, n, i) {
                 fl(!i || "object" == typeof i), !e || Array.isArray(e) || _a(e) || (i = void 0, n = e, e = void 0), n = n || {};
                 const r = Ma(t = await t),
                     s = function(t, e) {
                         if (!e && t && !Array.isArray(t)) return t;
                         let n;
                         if (t && (n = Array.isArray(t) ? t : [t]), e && e.loaders) {
                             const t = Array.isArray(e.loaders) ? e.loaders : [e.loaders];
@@ -7871,15 +7872,15 @@
                             const e = t ? t.lastIndexOf("/") : -1;
                             return e >= 0 ? t.substr(0, e) : ""
                         }(t)
                     }
                     return Array.isArray(i.loaders) || (i.loaders = null), i
                 }({
                     url: r,
-                    parse: Jl,
+                    parse: Ql,
                     loaders: s
                 }, n = cl(n, o, s, r), i || null), await async function(t, e, n, i) {
                     if (function(t) {
                             fl(t, "no worker provided");
                             t.version
                         }(t), ga(e)) {
                         const t = e,
@@ -7901,25 +7902,25 @@
                             type: a,
                             url: l
                         }
                     }
                     if (e = await Dl(e, t, n), t.parseTextSync && "string" == typeof e) return n.dataType = "text", t.parseTextSync(e, n, i, t);
                     if (function(t, e) {
                             return !!Ml.isSupported() && !!(ml || null != e && e._nodeWorkers) && t.worker && (null == e ? void 0 : e.worker)
-                        }(t, n)) return await Ll(t, e, n, i, Jl);
+                        }(t, n)) return await Ol(t, e, n, i, Ql);
                     if (t.parseText && "string" == typeof e) return await t.parseText(e, n, i, t);
                     if (t.parse) return await t.parse(e, n, i, t);
                     throw fl(!t.parseSync), new Error("".concat(t.id, " loader - no parser found and worker is disabled"))
                 }(o, t, n, i)) : null
             }
-            async function Ql(t, e, n, i) {
+            async function $l(t, e, n, i) {
                 Array.isArray(e) || _a(e) || (n = e, e = void 0);
                 const r = pl(n);
                 let s = t;
-                return "string" == typeof t && (s = await r(t)), ma(t) && (s = await r(t)), await Jl(s, e, n)
+                return "string" == typeof t && (s = await r(t)), ma(t) && (s = await r(t)), await Ql(s, e, n)
             }
             class tc {
                 constructor(t, e, n) {
                     wo(this, "id", void 0), wo(this, "context", void 0), wo(this, "isLoaded", void 0), wo(this, "persistent", void 0), wo(this, "_loadCount", 0), wo(this, "_subscribers", new Set), wo(this, "_data", void 0), wo(this, "_loader", void 0), wo(this, "_error", void 0), wo(this, "_content", void 0), this.id = t, this.context = n, this.setData(e)
                 }
                 subscribe(t) {
                     this._subscribers.add(t)
@@ -7935,15 +7936,15 @@
                     return this.isLoaded ? this._error ? Promise.reject(this._error) : this._content : this._loader.then((() => this.getData()))
                 }
                 setData(t, e) {
                     if (t === this._data && !e) return;
                     this._data = t;
                     const n = ++this._loadCount;
                     let i = t;
-                    "string" == typeof t && (i = Ql(t)), i instanceof Promise ? (this.isLoaded = !1, this._loader = i.then((t => {
+                    "string" == typeof t && (i = $l(t)), i instanceof Promise ? (this.isLoaded = !1, this._loader = i.then((t => {
                         this._loadCount === n && (this.isLoaded = !0, this._error = void 0, this._content = t)
                     })).catch((t => {
                         this._loadCount === n && (this.isLoaded = !0, this._error = t || !0)
                     }))) : (this.isLoaded = !0, this._error = void 0, this._content = t);
                     for (const t of this._subscribers) t.onChange(this.getData())
                 }
             }
@@ -8475,17 +8476,17 @@
                     r = e[1],
                     s = e[2];
                 return t[0] = n[0] * i + n[3] * r + n[6] * s, t[1] = n[1] * i + n[4] * r + n[7] * s, t[2] = n[2] * i + n[5] * r + n[8] * s, t[3] = e[3], t
             }
             mc();
             const Ac = [0, 0, 0];
             let Mc;
-            class Oc extends pc {
+            class Lc extends pc {
                 static get ZERO() {
-                    return Mc || (Mc = new Oc(0, 0, 0), Object.freeze(Mc)), Mc
+                    return Mc || (Mc = new Lc(0, 0, 0), Object.freeze(Mc)), Mc
                 }
                 constructor(t = 0, e = 0, n = 0) {
                     super(-0, -0, -0), 1 === arguments.length && sc(t) ? this.copy(t) : (ic.debug && (hc(t), hc(e), hc(n)), this[0] = t, this[1] = e, this[2] = n)
                 }
                 set(t, e, n) {
                     return this[0] = t, this[1] = e, this[2] = n, this.check()
                 }
@@ -8554,46 +8555,46 @@
                         t[0] = n[0] * i + n[2] * r, t[1] = n[1] * i + n[3] * r, t[2] = e[2]
                     }(this, this, t), this.check()
                 }
                 transformByQuaternion(t) {
                     return wc(this, this, t), this.check()
                 }
             }
-            const Lc = new Oc;
+            const Oc = new Lc;
 
             function kc(t, e, n, i) {
-                Lc.set(t, e, n);
-                const r = Lc.len();
+                Oc.set(t, e, n);
+                const r = Oc.len();
                 return {
                     distance: i / r,
-                    normal: new Oc(-t / r, -e / r, -n / r)
+                    normal: new Lc(-t / r, -e / r, -n / r)
                 }
             }
-            let Ic;
+            let Rc;
 
-            function Rc(t, e) {
+            function Ic(t, e) {
                 const {
                     size: n = 1,
                     startIndex: i = 0
                 } = e, r = void 0 !== e.endIndex ? e.endIndex : t.length, s = (r - i) / n;
-                Ic = nc.allocate(Ic, s, {
+                Rc = nc.allocate(Rc, s, {
                     type: Float32Array,
                     size: 2 * n
                 });
                 let o = i,
                     a = 0;
                 for (; o < r;) {
                     for (let e = 0; e < n; e++) {
                         const i = t[o++];
-                        Ic[a + e] = i, Ic[a + e + n] = (l = i) - Math.fround(l)
+                        Rc[a + e] = i, Rc[a + e + n] = (l = i) - Math.fround(l)
                     }
                     a += 2 * n
                 }
                 var l;
-                return Ic.subarray(0, s * n * 2)
+                return Rc.subarray(0, s * n * 2)
             }
             class jc extends cc {
                 toString() {
                     let t = "[";
                     if (ic.printRowMajor) {
                         t += "row-major:";
                         for (let e = 0; e < this.RANK; ++e)
@@ -8621,15 +8622,15 @@
                 setColumn(t, e) {
                     const n = t * this.RANK;
                     for (let t = 0; t < this.RANK; ++t) this[n + t] = e[t];
                     return this
                 }
             }
 
-            function zc(t, e) {
+            function Fc(t, e) {
                 var n = e[0],
                     i = e[1],
                     r = e[2],
                     s = e[3],
                     o = e[4],
                     a = e[5],
                     l = e[6],
@@ -8650,19 +8651,19 @@
                     E = r * c - s * l,
                     P = h * g - u * f,
                     S = h * m - d * f,
                     C = h * v - p * f,
                     T = u * m - d * g,
                     A = u * v - p * g,
                     M = d * v - p * m,
-                    O = b * M - y * A + _ * T + x * C - w * S + E * P;
-                return O ? (O = 1 / O, t[0] = (a * M - l * A + c * T) * O, t[1] = (r * A - i * M - s * T) * O, t[2] = (g * E - m * w + v * x) * O, t[3] = (d * w - u * E - p * x) * O, t[4] = (l * C - o * M - c * S) * O, t[5] = (n * M - r * C + s * S) * O, t[6] = (m * _ - f * E - v * y) * O, t[7] = (h * E - d * _ + p * y) * O, t[8] = (o * A - a * C + c * P) * O, t[9] = (i * C - n * A - s * P) * O, t[10] = (f * w - g * _ + v * b) * O, t[11] = (u * _ - h * w - p * b) * O, t[12] = (a * S - o * T - l * P) * O, t[13] = (n * T - i * S + r * P) * O, t[14] = (g * y - f * x - m * b) * O, t[15] = (h * x - u * y + d * b) * O, t) : null
+                    L = b * M - y * A + _ * T + x * C - w * S + E * P;
+                return L ? (L = 1 / L, t[0] = (a * M - l * A + c * T) * L, t[1] = (r * A - i * M - s * T) * L, t[2] = (g * E - m * w + v * x) * L, t[3] = (d * w - u * E - p * x) * L, t[4] = (l * C - o * M - c * S) * L, t[5] = (n * M - r * C + s * S) * L, t[6] = (m * _ - f * E - v * y) * L, t[7] = (h * E - d * _ + p * y) * L, t[8] = (o * A - a * C + c * P) * L, t[9] = (i * C - n * A - s * P) * L, t[10] = (f * w - g * _ + v * b) * L, t[11] = (u * _ - h * w - p * b) * L, t[12] = (a * S - o * T - l * P) * L, t[13] = (n * T - i * S + r * P) * L, t[14] = (g * y - f * x - m * b) * L, t[15] = (h * x - u * y + d * b) * L, t) : null
             }
 
-            function Fc(t, e, n) {
+            function zc(t, e, n) {
                 var i = e[0],
                     r = e[1],
                     s = e[2],
                     o = e[3],
                     a = e[4],
                     l = e[5],
                     c = e[6],
@@ -8759,22 +8760,22 @@
             }(),
             function(t) {
                 t[t.COL0ROW0 = 0] = "COL0ROW0", t[t.COL0ROW1 = 1] = "COL0ROW1", t[t.COL0ROW2 = 2] = "COL0ROW2", t[t.COL0ROW3 = 3] = "COL0ROW3", t[t.COL1ROW0 = 4] = "COL1ROW0", t[t.COL1ROW1 = 5] = "COL1ROW1", t[t.COL1ROW2 = 6] = "COL1ROW2", t[t.COL1ROW3 = 7] = "COL1ROW3", t[t.COL2ROW0 = 8] = "COL2ROW0", t[t.COL2ROW1 = 9] = "COL2ROW1", t[t.COL2ROW2 = 10] = "COL2ROW2", t[t.COL2ROW3 = 11] = "COL2ROW3", t[t.COL3ROW0 = 12] = "COL3ROW0", t[t.COL3ROW1 = 13] = "COL3ROW1", t[t.COL3ROW2 = 14] = "COL3ROW2", t[t.COL3ROW3 = 15] = "COL3ROW3"
             }(Uc || (Uc = {}));
             const Xc = 45 * Math.PI / 180,
                 Yc = 1,
                 Kc = .1,
-                $c = 500,
-                Jc = Object.freeze([1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1]);
-            class Qc extends jc {
+                Jc = 500,
+                Qc = Object.freeze([1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1]);
+            class $c extends jc {
                 static get IDENTITY() {
-                    return eh || (eh = new Qc, Object.freeze(eh)), eh
+                    return eh || (eh = new $c, Object.freeze(eh)), eh
                 }
                 static get ZERO() {
-                    return th || (th = new Qc([0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]), Object.freeze(th)), th
+                    return th || (th = new $c([0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]), Object.freeze(th)), th
                 }
                 get ELEMENTS() {
                     return 16
                 }
                 get RANK() {
                     return 4
                 }
@@ -8793,15 +8794,15 @@
                 setRowMajor(t, e, n, i, r, s, o, a, l, c, h, u, d, p, f, g) {
                     return this[0] = t, this[1] = r, this[2] = l, this[3] = d, this[4] = e, this[5] = s, this[6] = c, this[7] = p, this[8] = n, this[9] = o, this[10] = h, this[11] = f, this[12] = i, this[13] = a, this[14] = u, this[15] = g, this.check()
                 }
                 toRowMajor(t) {
                     return t[0] = this[0], t[1] = this[4], t[2] = this[8], t[3] = this[12], t[4] = this[1], t[5] = this[5], t[6] = this[9], t[7] = this[13], t[8] = this[2], t[9] = this[6], t[10] = this[10], t[11] = this[14], t[12] = this[3], t[13] = this[7], t[14] = this[11], t[15] = this[15], t
                 }
                 identity() {
-                    return this.copy(Jc)
+                    return this.copy(Qc)
                 }
                 fromObject(t) {
                     return this.check()
                 }
                 fromQuaternion(t) {
                     var e, n, i, r, s, o, a, l, c, h, u, d, p, f, g, m, v, b;
                     return e = this, h = (i = (n = t)[0]) * (a = i + i), u = (r = n[1]) * a, d = r * (l = r + r), p = (s = n[2]) * a, f = s * l, g = s * (c = s + s), m = (o = n[3]) * a, v = o * l, b = o * c, e[0] = 1 - d - g, e[1] = u + b, e[2] = p - v, e[3] = 0, e[4] = u - b, e[5] = 1 - h - g, e[6] = f + m, e[7] = 0, e[8] = p + v, e[9] = f - m, e[10] = 1 - h - d, e[11] = 0, e[12] = 0, e[13] = 0, e[14] = 0, e[15] = 1, this.check()
@@ -8809,15 +8810,15 @@
                 frustum(t) {
                     const {
                         left: e,
                         right: n,
                         bottom: i,
                         top: r,
                         near: s = Kc,
-                        far: o = $c
+                        far: o = Jc
                     } = t;
                     return o === 1 / 0 ? function(t, e, n, i, r, s) {
                         const o = 2 * s / (n - e),
                             a = 2 * s / (r - i),
                             l = (n + e) / (n - e),
                             c = (r + i) / (r - i),
                             h = -2 * s;
@@ -8853,30 +8854,30 @@
                 ortho(t) {
                     const {
                         left: e,
                         right: n,
                         bottom: i,
                         top: r,
                         near: s = Kc,
-                        far: o = $c
+                        far: o = Jc
                     } = t;
                     return function(t, e, n, i, r, s, o) {
                         var a = 1 / (e - n),
                             l = 1 / (i - r),
                             c = 1 / (s - o);
                         t[0] = -2 * a, t[1] = 0, t[2] = 0, t[3] = 0, t[4] = 0, t[5] = -2 * l, t[6] = 0, t[7] = 0, t[8] = 0, t[9] = 0, t[10] = 2 * c, t[11] = 0, t[12] = (e + n) * a, t[13] = (r + i) * l, t[14] = (o + s) * c, t[15] = 1
                     }(this, e, n, i, r, s, o), this.check()
                 }
                 orthographic(t) {
                     const {
                         fovy: e = Xc,
                         aspect: n = Yc,
                         focalDistance: i = 1,
                         near: r = Kc,
-                        far: s = $c
+                        far: s = Jc
                     } = t;
                     nh(e);
                     const o = e / 2,
                         a = i * Math.tan(o),
                         l = a * n;
                     return this.ortho({
                         left: -l,
@@ -8936,21 +8937,21 @@
                                 o = e[7],
                                 a = e[11];
                             t[1] = e[4], t[2] = e[8], t[3] = e[12], t[4] = n, t[6] = e[9], t[7] = e[13], t[8] = i, t[9] = s, t[11] = e[14], t[12] = r, t[13] = o, t[14] = a
                         } else t[0] = e[0], t[1] = e[4], t[2] = e[8], t[3] = e[12], t[4] = e[1], t[5] = e[5], t[6] = e[9], t[7] = e[13], t[8] = e[2], t[9] = e[6], t[10] = e[10], t[11] = e[14], t[12] = e[3], t[13] = e[7], t[14] = e[11], t[15] = e[15]
                     }(this, this), this.check()
                 }
                 invert() {
-                    return zc(this, this), this.check()
+                    return Fc(this, this), this.check()
                 }
                 multiplyLeft(t) {
-                    return Fc(this, t, this), this.check()
+                    return zc(this, t, this), this.check()
                 }
                 multiplyRight(t) {
-                    return Fc(this, this, t), this.check()
+                    return zc(this, this, t), this.check()
                 }
                 rotateX(t) {
                     return Nc(this, this, t), this.check()
                 }
                 rotateY(t) {
                     var e, n, i, r, s, o, a, l, c, h, u, d, p;
                     return e = this, n = this, i = t, r = Math.sin(i), s = Math.cos(i), o = n[0], a = n[1], l = n[2], c = n[3], h = n[8], u = n[9], d = n[10], p = n[11], n !== e && (e[4] = n[4], e[5] = n[5], e[6] = n[6], e[7] = n[7], e[12] = n[12], e[13] = n[13], e[14] = n[14], e[15] = n[15]), e[0] = o * s - h * r, e[1] = a * s - u * r, e[2] = l * s - d * r, e[3] = c * s - p * r, e[8] = o * r + h * s, e[9] = a * r + u * s, e[10] = l * r + d * s, e[11] = c * r + p * s, this.check()
@@ -8961,17 +8962,17 @@
                 rotateXYZ(t) {
                     return this.rotateX(t[0]).rotateY(t[1]).rotateZ(t[2])
                 }
                 rotateAxis(t, e) {
                     return function(t, e, n, i) {
                         var r, s, o, a, l, c, h, u, d, p, f, g, m, v, b, y, _, x, w, E, P, S, C, T, A = i[0],
                             M = i[1],
-                            O = i[2],
-                            L = Math.hypot(A, M, O);
-                        L < fc || (A *= L = 1 / L, M *= L, O *= L, r = Math.sin(n), o = 1 - (s = Math.cos(n)), a = e[0], l = e[1], c = e[2], h = e[3], u = e[4], d = e[5], p = e[6], f = e[7], g = e[8], m = e[9], v = e[10], b = e[11], y = A * A * o + s, _ = M * A * o + O * r, x = O * A * o - M * r, w = A * M * o - O * r, E = M * M * o + s, P = O * M * o + A * r, S = A * O * o + M * r, C = M * O * o - A * r, T = O * O * o + s, t[0] = a * y + u * _ + g * x, t[1] = l * y + d * _ + m * x, t[2] = c * y + p * _ + v * x, t[3] = h * y + f * _ + b * x, t[4] = a * w + u * E + g * P, t[5] = l * w + d * E + m * P, t[6] = c * w + p * E + v * P, t[7] = h * w + f * E + b * P, t[8] = a * S + u * C + g * T, t[9] = l * S + d * C + m * T, t[10] = c * S + p * C + v * T, t[11] = h * S + f * C + b * T, e !== t && (t[12] = e[12], t[13] = e[13], t[14] = e[14], t[15] = e[15]))
+                            L = i[2],
+                            O = Math.hypot(A, M, L);
+                        O < fc || (A *= O = 1 / O, M *= O, L *= O, r = Math.sin(n), o = 1 - (s = Math.cos(n)), a = e[0], l = e[1], c = e[2], h = e[3], u = e[4], d = e[5], p = e[6], f = e[7], g = e[8], m = e[9], v = e[10], b = e[11], y = A * A * o + s, _ = M * A * o + L * r, x = L * A * o - M * r, w = A * M * o - L * r, E = M * M * o + s, P = L * M * o + A * r, S = A * L * o + M * r, C = M * L * o - A * r, T = L * L * o + s, t[0] = a * y + u * _ + g * x, t[1] = l * y + d * _ + m * x, t[2] = c * y + p * _ + v * x, t[3] = h * y + f * _ + b * x, t[4] = a * w + u * E + g * P, t[5] = l * w + d * E + m * P, t[6] = c * w + p * E + v * P, t[7] = h * w + f * E + b * P, t[8] = a * S + u * C + g * T, t[9] = l * S + d * C + m * T, t[10] = c * S + p * C + v * T, t[11] = h * S + f * C + b * T, e !== t && (t[12] = e[12], t[13] = e[13], t[14] = e[14], t[15] = e[15]))
                     }(this, this, t, e), this.check()
                 }
                 scale(t) {
                     return Dc(this, this, Array.isArray(t) ? t : [t, t, t]), this.check()
                 }
                 translate(t) {
                     return Bc(this, this, t), this.check()
@@ -9205,54 +9206,54 @@
                     IDENTITY: 0
                 },
                 Mh = {
                     common: 0,
                     meters: 1,
                     pixels: 2
                 },
-                Oh = {
+                Lh = {
                     click: {
                         handler: "onClick"
                     },
                     panstart: {
                         handler: "onDragStart"
                     },
                     panmove: {
                         handler: "onDrag"
                     },
                     panend: {
                         handler: "onDragEnd"
                     }
                 },
-                Lh = "draw",
+                Oh = "draw",
                 kh = "mask",
-                Ih = Math.PI / 180,
-                Rh = [1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1],
+                Rh = Math.PI / 180,
+                Ih = [1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1],
                 jh = [0, 0, 0],
-                zh = {
+                Fh = {
                     unitsPerMeter: [1, 1, 1],
                     metersPerUnit: [1, 1, 1]
                 };
-            class Fh {
+            class zh {
                 constructor(t = {}) {
-                    wo(this, "id", void 0), wo(this, "x", void 0), wo(this, "y", void 0), wo(this, "width", void 0), wo(this, "height", void 0), wo(this, "isGeospatial", void 0), wo(this, "zoom", void 0), wo(this, "focalDistance", void 0), wo(this, "position", void 0), wo(this, "modelMatrix", void 0), wo(this, "distanceScales", void 0), wo(this, "scale", void 0), wo(this, "center", void 0), wo(this, "cameraPosition", void 0), wo(this, "projectionMatrix", void 0), wo(this, "viewMatrix", void 0), wo(this, "viewMatrixUncentered", void 0), wo(this, "viewMatrixInverse", void 0), wo(this, "viewProjectionMatrix", void 0), wo(this, "pixelProjectionMatrix", void 0), wo(this, "pixelUnprojectionMatrix", void 0), wo(this, "resolution", void 0), wo(this, "_frustumPlanes", {}), this.id = t.id || this.constructor.displayName || "viewport", this.x = t.x || 0, this.y = t.y || 0, this.width = t.width || 1, this.height = t.height || 1, this.zoom = t.zoom || 0, this.distanceScales = t.distanceScales || zh, this.focalDistance = t.focalDistance || 1, this.position = t.position || jh, this.modelMatrix = t.modelMatrix || null;
+                    wo(this, "id", void 0), wo(this, "x", void 0), wo(this, "y", void 0), wo(this, "width", void 0), wo(this, "height", void 0), wo(this, "isGeospatial", void 0), wo(this, "zoom", void 0), wo(this, "focalDistance", void 0), wo(this, "position", void 0), wo(this, "modelMatrix", void 0), wo(this, "distanceScales", void 0), wo(this, "scale", void 0), wo(this, "center", void 0), wo(this, "cameraPosition", void 0), wo(this, "projectionMatrix", void 0), wo(this, "viewMatrix", void 0), wo(this, "viewMatrixUncentered", void 0), wo(this, "viewMatrixInverse", void 0), wo(this, "viewProjectionMatrix", void 0), wo(this, "pixelProjectionMatrix", void 0), wo(this, "pixelUnprojectionMatrix", void 0), wo(this, "resolution", void 0), wo(this, "_frustumPlanes", {}), this.id = t.id || this.constructor.displayName || "viewport", this.x = t.x || 0, this.y = t.y || 0, this.width = t.width || 1, this.height = t.height || 1, this.zoom = t.zoom || 0, this.distanceScales = t.distanceScales || Fh, this.focalDistance = t.focalDistance || 1, this.position = t.position || jh, this.modelMatrix = t.modelMatrix || null;
                     const {
                         longitude: e,
                         latitude: n
                     } = t;
                     this.isGeospatial = Number.isFinite(n) && Number.isFinite(e), this._initProps(t), this._initMatrices(t), this.equals = this.equals.bind(this), this.project = this.project.bind(this), this.unproject = this.unproject.bind(this), this.projectPosition = this.projectPosition.bind(this), this.unprojectPosition = this.unprojectPosition.bind(this), this.projectFlat = this.projectFlat.bind(this), this.unprojectFlat = this.unprojectFlat.bind(this)
                 }
                 get metersPerPixel() {
                     return this.distanceScales.metersPerUnit[2] / this.scale
                 }
                 get projectionMode() {
                     return this.isGeospatial ? this.zoom < 12 ? Ah.WEB_MERCATOR : Ah.WEB_MERCATOR_AUTO_OFFSET : Ah.IDENTITY
                 }
                 equals(t) {
-                    return t instanceof Fh && (this === t || t.width === this.width && t.height === this.height && t.scale === this.scale && lc(t.projectionMatrix, this.projectionMatrix) && lc(t.viewMatrix, this.viewMatrix))
+                    return t instanceof zh && (this === t || t.width === this.width && t.height === this.height && t.scale === this.scale && lc(t.projectionMatrix, this.projectionMatrix) && lc(t.viewMatrix, this.viewMatrix))
                 }
                 project(t, {
                     topLeft: e = !0
                 } = {}) {
                     const n = wh(this.projectPosition(t), this.pixelProjectionMatrix),
                         [i, r] = n,
                         s = e ? r : this.height - r;
@@ -9341,49 +9342,49 @@
                     const i = Math.pow(2, this.zoom);
                     this.scale = i;
                     const {
                         position: r,
                         modelMatrix: s
                     } = t;
                     let o = jh;
-                    if (r && (o = s ? new Qc(s).transformAsVector(r, []) : r), this.isGeospatial) {
+                    if (r && (o = s ? new $c(s).transformAsVector(r, []) : r), this.isGeospatial) {
                         const t = this.projectPosition([e, n, 0]);
-                        this.center = new Oc(o).scale(this.distanceScales.unitsPerMeter).add(t)
+                        this.center = new Lc(o).scale(this.distanceScales.unitsPerMeter).add(t)
                     } else this.center = this.projectPosition(o)
                 }
                 _initMatrices(t) {
                     const {
-                        viewMatrix: e = Rh,
+                        viewMatrix: e = Ih,
                         projectionMatrix: n = null,
                         orthographic: i = !1,
                         fovyRadians: r,
                         fovy: s = 75,
                         near: o = .1,
                         far: a = 1e3,
                         padding: l = null,
                         focalDistance: c = 1
                     } = t;
-                    this.viewMatrixUncentered = e, this.viewMatrix = (new Qc).multiplyRight(e).translate(new Oc(this.center).negate()), this.projectionMatrix = n || function({
+                    this.viewMatrixUncentered = e, this.viewMatrix = (new $c).multiplyRight(e).translate(new Lc(this.center).negate()), this.projectionMatrix = n || function({
                         width: t,
                         height: e,
                         orthographic: n,
                         fovyRadians: i,
                         focalDistance: r,
                         padding: s,
                         near: o,
                         far: a
                     }) {
                         const l = t / e,
-                            c = n ? (new Qc).orthographic({
+                            c = n ? (new $c).orthographic({
                                 fovy: i,
                                 aspect: l,
                                 focalDistance: r,
                                 near: o,
                                 far: a
-                            }) : (new Qc).perspective({
+                            }) : (new $c).perspective({
                                 fovy: i,
                                 aspect: l,
                                 near: o,
                                 far: a
                             });
                         if (s) {
                             const {
@@ -9395,29 +9396,29 @@
                             c[8] -= 2 * a / t, c[9] += 2 * l / e
                         }
                         return c
                     }({
                         width: this.width,
                         height: this.height,
                         orthographic: i,
-                        fovyRadians: r || s * Ih,
+                        fovyRadians: r || s * Rh,
                         focalDistance: c,
                         padding: l,
                         near: o,
                         far: a
                     });
                     const h = [1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1];
                     var u;
-                    Fc(h, h, this.projectionMatrix), Fc(h, h, this.viewMatrix), this.viewProjectionMatrix = h, this.viewMatrixInverse = zc([], this.viewMatrix) || this.viewMatrix, this.cameraPosition = [(u = this.viewMatrixInverse)[12], u[13], u[14]];
+                    zc(h, h, this.projectionMatrix), zc(h, h, this.viewMatrix), this.viewProjectionMatrix = h, this.viewMatrixInverse = Fc([], this.viewMatrix) || this.viewMatrix, this.cameraPosition = [(u = this.viewMatrixInverse)[12], u[13], u[14]];
                     const d = [1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1],
                         p = [1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1];
-                    Dc(d, d, [this.width / 2, -this.height / 2, 1]), Bc(d, d, [1, -1, 0]), Fc(p, d, this.viewProjectionMatrix), this.pixelProjectionMatrix = p, this.pixelUnprojectionMatrix = zc([1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1], this.pixelProjectionMatrix), this.pixelUnprojectionMatrix || ta.warn("Pixel project matrix not invertible")()
+                    Dc(d, d, [this.width / 2, -this.height / 2, 1]), Bc(d, d, [1, -1, 0]), zc(p, d, this.viewProjectionMatrix), this.pixelProjectionMatrix = p, this.pixelUnprojectionMatrix = Fc([1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1], this.pixelProjectionMatrix), this.pixelUnprojectionMatrix || ta.warn("Pixel project matrix not invertible")()
                 }
             }
-            wo(Fh, "displayName", "Viewport");
+            wo(zh, "displayName", "Viewport");
             const Bh = "vs",
                 Dh = "fs";
 
             function Nh(t, e) {
                 if (!t) throw new Error(e || "shadertools: assertion failed.")
             }
             const Vh = {
@@ -9559,30 +9560,30 @@
 
             function qh(t, e) {
                 return t.map((t => (t instanceof Wh || (Nh("string" != typeof t, "Shader module use by name is deprecated. Import shader module '".concat(t, "' and use it directly.")), Nh(t.name, "shader module has no name"), (t = new Wh(t)).dependencies = qh(t.dependencies)), t)))
             }
             const Xh = 7936,
                 Yh = 7937,
                 Kh = 7938,
-                $h = 35724,
-                Jh = {
+                Jh = 35724,
+                Qh = {
                     GLSL_FRAG_DATA: ["WEBGL_draw_buffers", !0],
                     GLSL_FRAG_DEPTH: ["EXT_frag_depth", !0],
                     GLSL_DERIVATIVES: ["OES_standard_derivatives", !0],
                     GLSL_TEXTURE_LOD: ["EXT_shader_texture_lod", !0]
                 },
-                Qh = {};
-            Object.keys(Jh).forEach((t => {
-                Qh[t] = t
+                $h = {};
+            Object.keys(Qh).forEach((t => {
+                $h[t] = t
             }));
             const tu = {};
 
             function eu(t, e) {
                 let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : {};
-                const i = Jh[e];
+                const i = Qh[e];
                 if (Nh(i, e), ! function() {
                         let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                         const e = "undefined" != typeof window && window.navigator || {},
                             n = t.userAgent || e.userAgent || "",
                             i = -1 !== n.indexOf("MSIE "),
                             r = -1 !== n.indexOf("Trident/");
                         return i || r
@@ -9595,15 +9596,15 @@
                 t.shaderSource(a, o), t.compileShader(a);
                 const l = t.getShaderParameter(a, 35713);
                 return t.deleteShader(a), tu[e] = l, l
             }
 
             function nu(t, e) {
                 return (e = Array.isArray(e) ? e : [e]).every((e => function(t, e) {
-                    const n = Jh[e];
+                    const n = Qh[e];
                     Nh(n, e);
                     const i = function(t) {
                             return "undefined" != typeof WebGL2RenderingContext && t instanceof WebGL2RenderingContext || Boolean(t && 2 === t._version)
                         }(t) && n[1] || n[0],
                         r = "string" == typeof i ? Boolean(t.getExtension(i)) : i;
                     return Nh(!1 === r || !0 === r), r
                 }(t, e)))
@@ -9744,32 +9745,32 @@
                         return {
                             gpuVendor: function(t, e) {
                                 return t.match(/NVIDIA/i) || e.match(/NVIDIA/i) ? "NVIDIA" : t.match(/INTEL/i) || e.match(/INTEL/i) ? "INTEL" : t.match(/AMD/i) || e.match(/AMD/i) || t.match(/ATI/i) || e.match(/ATI/i) ? "AMD" : "UNKNOWN GPU"
                             }(n, i),
                             vendor: n,
                             renderer: i,
                             version: t.getParameter(Kh),
-                            shadingLanguageVersion: t.getParameter($h)
+                            shadingLanguageVersion: t.getParameter(Jh)
                         }
                     }(t);
                     switch (e.gpuVendor.toLowerCase()) {
                         case "nvidia":
                             return "#define NVIDIA_GPU\n// Nvidia optimizes away the calculation necessary for emulated fp64\n#define LUMA_FP64_CODE_ELIMINATION_WORKAROUND 1\n";
                         case "intel":
                             return "#define INTEL_GPU\n// Intel optimizes away the calculation necessary for emulated fp64\n#define LUMA_FP64_CODE_ELIMINATION_WORKAROUND 1\n// Intel's built-in 'tan' function doesn't have acceptable precision\n#define LUMA_FP32_TAN_PRECISION_WORKAROUND 1\n// Intel GPU doesn't have full 32 bits precision in same cases, causes overflow\n#define LUMA_FP64_HIGH_BITS_OVERFLOW_WORKAROUND 1\n";
                         case "amd":
                             return "#define AMD_GPU\n";
                         default:
                             return "#define DEFAULT_GPU\n// Prevent driver from optimizing away the calculation necessary for emulated fp64\n#define LUMA_FP64_CODE_ELIMINATION_WORKAROUND 1\n// Intel's built-in 'tan' function doesn't have acceptable precision\n#define LUMA_FP32_TAN_PRECISION_WORKAROUND 1\n// Intel GPU doesn't have full 32 bits precision in same cases, causes overflow\n#define LUMA_FP64_HIGH_BITS_OVERFLOW_WORKAROUND 1\n"
                     }
                 }(t), "\n").concat(function(t, e, n) {
                     let i = "#if (__VERSION__ > 120)\n\n# define FEATURE_GLSL_DERIVATIVES\n# define FEATURE_GLSL_DRAW_BUFFERS\n# define FEATURE_GLSL_FRAG_DEPTH\n# define FEATURE_GLSL_TEXTURE_LOD\n\n// DEPRECATED FLAGS, remove in v9\n# define FRAG_DEPTH\n# define DERIVATIVES\n# define DRAW_BUFFERS\n# define TEXTURE_LOD\n\n#endif // __VERSION\n";
-                    return nu(t, Qh.GLSL_FRAG_DEPTH) && (i += "\n// FRAG_DEPTH => gl_FragDepth is available\n#ifdef GL_EXT_frag_depth\n#extension GL_EXT_frag_depth : enable\n# define FEATURE_GLSL_FRAG_DEPTH\n# define FRAG_DEPTH\n# define gl_FragDepth gl_FragDepthEXT\n#endif\n"), nu(t, Qh.GLSL_DERIVATIVES) && eu(t, Qh.GLSL_DERIVATIVES) && (i += "\n// DERIVATIVES => dxdF, dxdY and fwidth are available\n#ifdef GL_OES_standard_derivatives\n#extension GL_OES_standard_derivatives : enable\n# define FEATURE_GLSL_DERIVATIVES\n# define DERIVATIVES\n#endif\n"), nu(t, Qh.GLSL_FRAG_DATA) && eu(t, Qh.GLSL_FRAG_DATA, {
+                    return nu(t, $h.GLSL_FRAG_DEPTH) && (i += "\n// FRAG_DEPTH => gl_FragDepth is available\n#ifdef GL_EXT_frag_depth\n#extension GL_EXT_frag_depth : enable\n# define FEATURE_GLSL_FRAG_DEPTH\n# define FRAG_DEPTH\n# define gl_FragDepth gl_FragDepthEXT\n#endif\n"), nu(t, $h.GLSL_DERIVATIVES) && eu(t, $h.GLSL_DERIVATIVES) && (i += "\n// DERIVATIVES => dxdF, dxdY and fwidth are available\n#ifdef GL_OES_standard_derivatives\n#extension GL_OES_standard_derivatives : enable\n# define FEATURE_GLSL_DERIVATIVES\n# define DERIVATIVES\n#endif\n"), nu(t, $h.GLSL_FRAG_DATA) && eu(t, $h.GLSL_FRAG_DATA, {
                         behavior: "require"
-                    }) && (i += "\n// DRAW_BUFFERS => gl_FragData[] is available\n#ifdef GL_EXT_draw_buffers\n#extension GL_EXT_draw_buffers : require\n#define FEATURE_GLSL_DRAW_BUFFERS\n#define DRAW_BUFFERS\n#endif\n"), nu(t, Qh.GLSL_TEXTURE_LOD) && (i += "// TEXTURE_LOD => texture2DLod etc are available\n#ifdef GL_EXT_shader_texture_lod\n#extension GL_EXT_shader_texture_lod : enable\n\n# define FEATURE_GLSL_TEXTURE_LOD\n# define TEXTURE_LOD\n\n#endif\n"), i
+                    }) && (i += "\n// DRAW_BUFFERS => gl_FragData[] is available\n#ifdef GL_EXT_draw_buffers\n#extension GL_EXT_draw_buffers : require\n#define FEATURE_GLSL_DRAW_BUFFERS\n#define DRAW_BUFFERS\n#endif\n"), nu(t, $h.GLSL_TEXTURE_LOD) && (i += "// TEXTURE_LOD => texture2DLod etc are available\n#ifdef GL_EXT_shader_texture_lod\n#extension GL_EXT_shader_texture_lod : enable\n\n# define FEATURE_GLSL_TEXTURE_LOD\n# define TEXTURE_LOD\n\n#endif\n"), i
                 }(t), "\n").concat(function() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {},
                         e = 0,
                         n = "";
                     for (const i in t) {
                         0 === e && (n += "\n// APPLICATION DEFINES\n"), e++;
                         const r = t[i];
@@ -9881,37 +9882,37 @@
                 return "undefined" != typeof WebGLRenderingContext && t instanceof WebGLRenderingContext || "undefined" != typeof WebGL2RenderingContext && t instanceof WebGL2RenderingContext || Boolean(t && Number.isFinite(t._version))
             }
 
             function Mu(t) {
                 return "undefined" != typeof WebGL2RenderingContext && t instanceof WebGL2RenderingContext || Boolean(t && 2 === t._version)
             }
 
-            function Ou(t) {
+            function Lu(t) {
                 return Cu(Au(t), "Invalid WebGLRenderingContext"), t
             }
 
-            function Lu(t) {
+            function Ou(t) {
                 return Cu(Mu(t), Tu), t
             }
             const ku = {};
-            const Iu = function t(e) {
+            const Ru = function t(e) {
                 const n = e.gl;
                 this.ext = e, this.isAlive = !0, this.hasBeenBound = !1, this.elementArrayBuffer = null, this.attribs = new Array(e.maxVertexAttribs);
                 for (let e = 0; e < this.attribs.length; e++) {
                     const i = new t.VertexAttrib(n);
                     this.attribs[e] = i
                 }
                 this.maxAttrib = 0
             };
-            (Iu.VertexAttrib = function(t) {
+            (Ru.VertexAttrib = function(t) {
                 this.enabled = !1, this.buffer = null, this.size = 4, this.type = 5126, this.normalized = !1, this.stride = 16, this.offset = 0, this.cached = "", this.recache()
             }).prototype.recache = function() {
                 this.cached = [this.size, this.type, this.normalized, this.stride, this.offset].join(":")
             };
-            const Ru = function(t) {
+            const Iu = function(t) {
                 const e = this;
                 this.gl = t,
                     function(t) {
                         const e = t.getError;
                         t.getError = function() {
                             let n;
                             do {
@@ -9970,27 +9971,27 @@
                     l.maxAttrib = Math.max(l.maxAttrib, t);
                     const c = l.attribs[t];
                     return c.buffer = e.currentArrayBuffer, c.size = i, c.type = r, c.normalized = s, c.stride = o, c.offset = a, c.recache(), n.vertexAttribPointer.apply(this, arguments)
                 }, t.instrumentExtension && t.instrumentExtension(this, "OES_vertex_array_object"), t.canvas && t.canvas.addEventListener("webglcontextrestored", (() => {
                     globalThis.console && globalThis.console.log && globalThis.console.log("OESVertexArrayObject emulation library context restored"), e.reset_()
                 }), !0), this.reset_()
             };
-            Ru.prototype.VERTEX_ARRAY_BINDING_OES = 34229, Ru.prototype.reset_ = function() {
+            Iu.prototype.VERTEX_ARRAY_BINDING_OES = 34229, Iu.prototype.reset_ = function() {
                 if (void 0 !== this.vertexArrayObjects)
                     for (let t = 0; t < this.vertexArrayObjects.length; ++t) this.vertexArrayObjects.isAlive = !1;
                 const t = this.gl;
-                this.maxVertexAttribs = t.getParameter(34921), this.defaultVertexArrayObject = new Iu(this), this.currentVertexArrayObject = null, this.currentArrayBuffer = null, this.vertexArrayObjects = [this.defaultVertexArrayObject], this.bindVertexArrayOES(null)
-            }, Ru.prototype.createVertexArrayOES = function() {
-                const t = new Iu(this);
+                this.maxVertexAttribs = t.getParameter(34921), this.defaultVertexArrayObject = new Ru(this), this.currentVertexArrayObject = null, this.currentArrayBuffer = null, this.vertexArrayObjects = [this.defaultVertexArrayObject], this.bindVertexArrayOES(null)
+            }, Iu.prototype.createVertexArrayOES = function() {
+                const t = new Ru(this);
                 return this.vertexArrayObjects.push(t), t
-            }, Ru.prototype.deleteVertexArrayOES = function(t) {
+            }, Iu.prototype.deleteVertexArrayOES = function(t) {
                 t.isAlive = !1, this.vertexArrayObjects.splice(this.vertexArrayObjects.indexOf(t), 1), this.currentVertexArrayObject === t && this.bindVertexArrayOES(null)
-            }, Ru.prototype.isVertexArrayOES = function(t) {
-                return !!(t && t instanceof Iu && t.hasBeenBound && t.ext === this)
-            }, Ru.prototype.bindVertexArrayOES = function(t) {
+            }, Iu.prototype.isVertexArrayOES = function(t) {
+                return !!(t && t instanceof Ru && t.hasBeenBound && t.ext === this)
+            }, Iu.prototype.bindVertexArrayOES = function(t) {
                 const e = this.gl;
                 if (t && !t.isAlive) return n = "bindVertexArrayOES: attempt to bind deleted arrayObject", ku[1282] = !0, void(void 0 !== n && (i = n, globalThis.console && globalThis.console.error && globalThis.console.error(i)));
                 var n, i;
                 const r = this.original,
                     s = this.currentVertexArrayObject;
                 this.currentVertexArrayObject = t || this.defaultVertexArrayObject, this.currentVertexArrayObject.hasBeenBound = !0;
                 const o = this.currentVertexArrayObject;
@@ -10005,53 +10006,53 @@
                         let o = !1;
                         s && n.buffer === i.buffer || (a !== n.buffer && (r.bindBuffer.call(e, 34962, n.buffer), a = n.buffer), o = !0), (o || n.cached !== i.cached) && r.vertexAttribPointer.call(e, t, n.size, n.type, n.normalized, n.stride, n.offset)
                     }
                 }
                 this.currentArrayBuffer !== a && r.bindBuffer.call(e, 34962, this.currentArrayBuffer)
             };
             const ju = "OES_element_index",
-                zu = "WEBGL_draw_buffers",
-                Fu = "WEBGL_debug_renderer_info",
+                Fu = "WEBGL_draw_buffers",
+                zu = "WEBGL_debug_renderer_info",
                 Bu = t => Mu(t) ? void 0 : 0,
                 Du = {
                     3074: t => Mu(t) ? void 0 : 36064,
                     35723: t => Mu(t) ? void 0 : 4352,
                     35977: Bu,
                     32937: Bu,
                     36795: (t, e) => {
                         const n = Mu(t) ? t.getExtension("EXT_disjoint_timer_query_webgl2") : t.getExtension("EXT_disjoint_timer_query");
                         return n && n.GPU_DISJOINT_EXT ? e(n.GPU_DISJOINT_EXT) : 0
                     },
                     37445: (t, e) => {
-                        const n = t.getExtension(Fu);
+                        const n = t.getExtension(zu);
                         return e(n && n.UNMASKED_VENDOR_WEBGL || 7936)
                     },
                     37446: (t, e) => {
-                        const n = t.getExtension(Fu);
+                        const n = t.getExtension(zu);
                         return e(n && n.UNMASKED_RENDERER_WEBGL || 7937)
                     },
                     34047: (t, e) => {
                         const n = t.luma.extensions.EXT_texture_filter_anisotropic;
                         return n ? e(n.MAX_TEXTURE_MAX_ANISOTROPY_EXT) : 1
                     },
                     32883: Bu,
                     35071: Bu,
                     37447: Bu,
                     36063: (t, e) => {
                         if (!Mu(t)) {
-                            const n = t.getExtension(zu);
+                            const n = t.getExtension(Fu);
                             return n ? e(n.MAX_COLOR_ATTACHMENTS_WEBGL) : 0
                         }
                     },
                     35379: Bu,
                     35374: Bu,
                     35377: Bu,
                     34852: t => {
                         if (!Mu(t)) {
-                            const e = t.getExtension(zu);
+                            const e = t.getExtension(Fu);
                             return e ? e.MAX_DRAW_BUFFERS_WEBGL : 0
                         }
                     },
                     36203: t => t.getExtension(ju) ? 2147483647 : 65535,
                     33001: t => t.getExtension(ju) ? 16777216 : 65535,
                     33e3: t => 16777216,
                     37157: Bu,
@@ -10210,15 +10211,15 @@
                     const e = t.getSupportedExtensions;
                     t.getSupportedExtensions = function() {
                         const t = e.call(this) || [];
                         return t.indexOf("OES_vertex_array_object") < 0 && t.push("OES_vertex_array_object"), t
                     };
                     const n = t.getExtension;
                     t.getExtension = function(e) {
-                        return n.call(this, e) || ("OES_vertex_array_object" !== e ? null : (t.__OESVertexArrayObject || (this.__OESVertexArrayObject = new Ru(this)), this.__OESVertexArrayObject))
+                        return n.call(this, e) || ("OES_vertex_array_object" !== e ? null : (t.__OESVertexArrayObject || (this.__OESVertexArrayObject = new Iu(this)), this.__OESVertexArrayObject))
                     }
                 }(t), function(t) {
                     t.luma.extensions = {};
                     const e = t.getSupportedExtensions() || [];
                     for (const n of e) t.luma[n] = t.getExtension(n)
                 }(t), function(t, e) {
                     for (const n of Object.getOwnPropertyNames(e)) "overrides" !== n && Gu(t, {
@@ -10432,25 +10433,25 @@
                 },
                 viewport: (t, e) => t.viewport(...e)
             };
 
             function Ku(t, e, n) {
                 return void 0 !== e[t] ? e[t] : n[t]
             }
-            const $u = {
+            const Ju = {
                     blendEquation: (t, e, n) => t.blendEquationSeparate(Ku(32777, e, n), Ku(34877, e, n)),
                     blendFunc: (t, e, n) => t.blendFuncSeparate(Ku(32969, e, n), Ku(32968, e, n), Ku(32971, e, n), Ku(32970, e, n)),
                     polygonOffset: (t, e, n) => t.polygonOffset(Ku(32824, e, n), Ku(10752, e, n)),
                     sampleCoverage: (t, e, n) => t.sampleCoverage(Ku(32938, e, n), Ku(32939, e, n)),
                     stencilFuncFront: (t, e, n) => t.stencilFuncSeparate(1028, Ku(2962, e, n), Ku(2967, e, n), Ku(2963, e, n)),
                     stencilFuncBack: (t, e, n) => t.stencilFuncSeparate(1029, Ku(34816, e, n), Ku(36003, e, n), Ku(36004, e, n)),
                     stencilOpFront: (t, e, n) => t.stencilOpSeparate(1028, Ku(2964, e, n), Ku(2965, e, n), Ku(2966, e, n)),
                     stencilOpBack: (t, e, n) => t.stencilOpSeparate(1029, Ku(34817, e, n), Ku(34818, e, n), Ku(34819, e, n))
                 },
-                Ju = {
+                Qu = {
                     enable: (t, e) => t({
                         [e]: !0
                     }),
                     disable: (t, e) => t({
                         [e]: !1
                     }),
                     pixelStorei: (t, e, n) => t({
@@ -10575,26 +10576,26 @@
                         [1028 === e ? 2965 : 34818]: i,
                         [1028 === e ? 2966 : 34819]: r
                     }),
                     viewport: (t, e, n, i, r) => t({
                         2978: [e, n, i, r]
                     })
                 },
-                Qu = (t, e) => t.isEnabled(e),
+                $u = (t, e) => t.isEnabled(e),
                 td = {
-                    3042: Qu,
-                    2884: Qu,
-                    2929: Qu,
-                    3024: Qu,
-                    32823: Qu,
-                    32926: Qu,
-                    32928: Qu,
-                    3089: Qu,
-                    2960: Qu,
-                    35977: Qu
+                    3042: $u,
+                    2884: $u,
+                    2929: $u,
+                    3024: $u,
+                    32823: $u,
+                    32926: $u,
+                    32928: $u,
+                    3089: $u,
+                    2960: $u,
+                    35977: $u
                 };
 
             function ed(t) {
                 for (const e in t) return !1;
                 return !0
             }
 
@@ -10695,15 +10696,15 @@
                         }),
                         function(t) {
                             const e = t.useProgram.bind(t);
                             t.useProgram = function(n) {
                                 t.state.program !== n && (e(n), t.state.program = n)
                             }
                         }(t);
-                    for (const e in Ju) rd(t, e, Ju[e]);
+                    for (const e in Qu) rd(t, e, Qu[e]);
                     id(t, "getParameter"), id(t, "isEnabled")
                 }
                 return t.state.enable = n, t
             }
 
             function ad(t) {
                 Cu(t.state), t.state.pop()
@@ -10715,15 +10716,15 @@
                 for (const i in e) {
                     const r = Number(i),
                         s = Yu[i];
                     s && ("string" == typeof s ? n[s] = !0 : s(t, e[i], r))
                 }
                 const i = t.state && t.state.cache;
                 if (i)
-                    for (const r in n)(0, $u[r])(t, e, i)
+                    for (const r in n)(0, Ju[r])(t, e, i)
             }
 
             function cd(t, e, n) {
                 if (ed(e)) return n(t);
                 const {
                     nocatch: i = !0
                 } = e;
@@ -10774,15 +10775,15 @@
             function dd(t, e, n) {
                 return Math.min(Math.round(t * e), n - 1)
             }
 
             function pd(t, e, n, i) {
                 return i ? Math.max(0, n - 1 - Math.round(t * e)) : Math.min(Math.round(t * e), n - 1)
             }
-            const fd = Io(),
+            const fd = Ro(),
                 gd = fd && "undefined" != typeof document,
                 md = {
                     webgl2: !0,
                     webgl1: !0,
                     throwOnError: !0,
                     manageState: !0,
                     canvas: null,
@@ -10901,15 +10902,15 @@
 
             function Pd(t, e) {
                 e = Number(e);
                 for (const n in t)
                     if (t[n] === e) return "GL.".concat(n);
                 return String(e)
             }
-            globalThis.luma || (Io() && Su.log(1, "luma.gl ".concat(yd, " - ").concat("set luma.log.level=1 (or higher) to trace rendering"))(), globalThis.luma = globalThis.luma || {
+            globalThis.luma || (Ro() && Su.log(1, "luma.gl ".concat(yd, " - ").concat("set luma.log.level=1 (or higher) to trace rendering"))(), globalThis.luma = globalThis.luma || {
                 VERSION: yd,
                 version: yd,
                 log: Su,
                 stats: xd,
                 globals: {
                     modules: {},
                     nodeIO: {}
@@ -10942,22 +10943,22 @@
                     s = Object.getPrototypeOf(t);
                 i.forEach((t => {
                     s.methodName || (s[t] = () => {
                         throw Su.removed("Calling removed method ".concat(e, ".").concat(t, ": "), r)(), new Error(t)
                     })
                 }))
             }
-            const Od = "Resource subclass must define virtual methods";
-            class Ld {
+            const Ld = "Resource subclass must define virtual methods";
+            class Od {
                 get[Symbol.toStringTag]() {
                     return "Resource"
                 }
                 constructor(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
-                    Ou(t);
+                    Lu(t);
                     const {
                         id: n,
                         userData: i = {}
                     } = e;
                     this.gl = t, this.gl2 = t, this.id = n || Cd(this[Symbol.toStringTag]), this.userData = i, this._bound = !1, this._handle = e.handle, void 0 === this._handle && (this._handle = this._createHandle()), this.byteLength = 0, this._initStats(), this._addStats()
                 }
                 toString() {
@@ -11024,30 +11025,30 @@
                     return this
                 }
                 stubRemovedMethods(t, e, n) {
                     return Md(this, t, e, n)
                 }
                 initialize(t) {}
                 _createHandle() {
-                    throw new Error(Od)
+                    throw new Error(Ld)
                 }
                 _deleteHandle() {
-                    throw new Error(Od)
+                    throw new Error(Ld)
                 }
                 _bindHandle(t) {
-                    throw new Error(Od)
+                    throw new Error(Ld)
                 }
                 _getOptsFromHandle() {
-                    throw new Error(Od)
+                    throw new Error(Ld)
                 }
                 _getParameter(t, e) {
-                    throw new Error(Od)
+                    throw new Error(Ld)
                 }
                 _setParameter(t, e) {
-                    throw new Error(Od)
+                    throw new Error(Ld)
                 }
                 _context() {
                     return this.gl.luma = this.gl.luma || {}, this.gl.luma
                 }
                 _initStats() {
                     this.gl.stats = this.gl.stats || new _d
                 }
@@ -11077,15 +11078,15 @@
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : this[Symbol.toStringTag],
                         e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : xd.get("Memory Usage");
                     e.get("GPU Memory").subtractCount(this.byteLength), e.get("".concat(t, " Memory")).subtractCount(this.byteLength), this.byteLength = 0
                 }
             }
             const kd = "Failed to deduce GL constant from typed array";
 
-            function Id(t) {
+            function Rd(t) {
                 switch (ArrayBuffer.isView(t) ? t.constructor : t) {
                     case Float32Array:
                         return 5126;
                     case Uint16Array:
                         return 5123;
                     case Uint32Array:
                         return 5125;
@@ -11099,15 +11100,15 @@
                     case Int32Array:
                         return 5124;
                     default:
                         throw new Error(kd)
                 }
             }
 
-            function Rd(t) {
+            function Id(t) {
                 let {
                     clamped: e = !0
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                 switch (t) {
                     case 5126:
                         return Float32Array;
                     case 5123:
@@ -11145,15 +11146,15 @@
                 return {
                     data: o,
                     width: r,
                     height: s
                 }
             }
 
-            function zd(t, e, n) {
+            function Fd(t, e, n) {
                 const {
                     removedProps: i = {},
                     deprecatedProps: r = {},
                     replacedProps: s = {}
                 } = n;
                 for (const n in i)
                     if (n in e) {
@@ -11166,15 +11167,15 @@
                     } let o = null;
                 for (const n in s)
                     if (n in e) {
                         const i = s[n];
                         Su.deprecated("".concat(t, ".").concat(n), "".concat(t, ".").concat(i))(), o = o || Object.assign({}, e), o[i] = e[n], delete o[n]
                     } return o || e
             }
-            const Fd = {
+            const zd = {
                     offset: 0,
                     stride: 0,
                     type: 5126,
                     size: 1,
                     divisor: 0,
                     normalized: !1,
                     integer: !1
@@ -11183,22 +11184,22 @@
                     deprecatedProps: {
                         instanced: "divisor",
                         isInstanced: "divisor"
                     }
                 };
             class Dd {
                 static getBytesPerElement(t) {
-                    return Rd(t.type || 5126).BYTES_PER_ELEMENT
+                    return Id(t.type || 5126).BYTES_PER_ELEMENT
                 }
                 static getBytesPerVertex(t) {
-                    return wd(t.size), Rd(t.type || 5126).BYTES_PER_ELEMENT * t.size
+                    return wd(t.size), Id(t.type || 5126).BYTES_PER_ELEMENT * t.size
                 }
                 static resolve() {
                     for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
-                    return new Dd(...[Fd, ...e])
+                    return new Dd(...[zd, ...e])
                 }
                 constructor() {
                     for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
                     e.forEach((t => this._assign(t))), Object.freeze(this)
                 }
                 toString() {
                     return JSON.stringify(this)
@@ -11207,15 +11208,15 @@
                     return Dd.getBytesPerElement(this)
                 }
                 get BYTES_PER_VERTEX() {
                     return Dd.getBytesPerVertex(this)
                 }
                 _assign() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
-                    return t = zd("Accessor", t, Bd), void 0 !== t.type && (this.type = t.type, 5124 !== t.type && 5125 !== t.type || (this.integer = !0)), void 0 !== t.size && (this.size = t.size), void 0 !== t.offset && (this.offset = t.offset), void 0 !== t.stride && (this.stride = t.stride), void 0 !== t.normalized && (this.normalized = t.normalized), void 0 !== t.integer && (this.integer = t.integer), void 0 !== t.divisor && (this.divisor = t.divisor), void 0 !== t.buffer && (this.buffer = t.buffer), void 0 !== t.index && ("boolean" == typeof t.index ? this.index = t.index ? 1 : 0 : this.index = t.index), void 0 !== t.instanced && (this.divisor = t.instanced ? 1 : 0), void 0 !== t.isInstanced && (this.divisor = t.isInstanced ? 1 : 0), this
+                    return t = Fd("Accessor", t, Bd), void 0 !== t.type && (this.type = t.type, 5124 !== t.type && 5125 !== t.type || (this.integer = !0)), void 0 !== t.size && (this.size = t.size), void 0 !== t.offset && (this.offset = t.offset), void 0 !== t.stride && (this.stride = t.stride), void 0 !== t.normalized && (this.normalized = t.normalized), void 0 !== t.integer && (this.integer = t.integer), void 0 !== t.divisor && (this.divisor = t.divisor), void 0 !== t.buffer && (this.buffer = t.buffer), void 0 !== t.index && ("boolean" == typeof t.index ? this.index = t.index ? 1 : 0 : this.index = t.index), void 0 !== t.instanced && (this.divisor = t.instanced ? 1 : 0), void 0 !== t.isInstanced && (this.divisor = t.isInstanced ? 1 : 0), this
                 }
             }
             const Nd = {
                     offset: "accessor.offset",
                     stride: "accessor.stride",
                     type: "accessor.type",
                     size: "accessor.size",
@@ -11231,15 +11232,15 @@
                         bytes: "byteLength"
                     },
                     deprecatedProps: Nd
                 },
                 Ud = {
                     removedProps: Nd
                 };
-            class Gd extends Ld {
+            class Gd extends Od {
                 get[Symbol.toStringTag]() {
                     return "Buffer"
                 }
                 constructor(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                     super(t, e), this.stubRemovedMethods("Buffer", "v6.0", ["layout", "setLayout", "getIndexedParameter"]), this.target = e.target || (this.gl.webgl2 ? 36662 : 34962), this.initialize(e), Object.seal(this)
                 }
@@ -11253,18 +11254,18 @@
                 }
                 initialize() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     return ArrayBuffer.isView(t) && (t = {
                         data: t
                     }), Number.isFinite(t) && (t = {
                         byteLength: t
-                    }), t = zd("Buffer", t, Vd), this.usage = t.usage || 35044, this.debugData = null, this.setAccessor(Object.assign({}, t, t.accessor)), t.data ? this._setData(t.data, t.offset, t.byteLength) : this._setByteLength(t.byteLength || 0), this
+                    }), t = Fd("Buffer", t, Vd), this.usage = t.usage || 35044, this.debugData = null, this.setAccessor(Object.assign({}, t, t.accessor)), t.data ? this._setData(t.data, t.offset, t.byteLength) : this._setByteLength(t.byteLength || 0), this
                 }
                 setProps(t) {
-                    return "accessor" in (t = zd("Buffer", t, Ud)) && this.setAccessor(t.accessor), this
+                    return "accessor" in (t = Fd("Buffer", t, Ud)) && this.setAccessor(t.accessor), this
                 }
                 setAccessor(t) {
                     return delete(t = Object.assign({}, t)).buffer, this.accessor = new Dd(t), this
                 }
                 reallocate(t) {
                     return t > this.byteLength ? (this._setByteLength(t), !0) : (this.bytesUsed = t, !1)
                 }
@@ -11278,37 +11279,37 @@
                     const {
                         data: e,
                         offset: n = 0,
                         srcOffset: i = 0
                     } = t, r = t.byteLength || t.length;
                     wd(e);
                     const s = this.gl.webgl2 ? 36663 : this.target;
-                    return this.gl.bindBuffer(s, this.handle), 0 !== i || void 0 !== r ? (Lu(this.gl), this.gl.bufferSubData(this.target, n, e, i, r)) : this.gl.bufferSubData(s, n, e), this.gl.bindBuffer(s, null), this.debugData = null, this._inferType(e), this
+                    return this.gl.bindBuffer(s, this.handle), 0 !== i || void 0 !== r ? (Ou(this.gl), this.gl.bufferSubData(this.target, n, e, i, r)) : this.gl.bufferSubData(s, n, e), this.gl.bindBuffer(s, null), this.debugData = null, this._inferType(e), this
                 }
                 copyData(t) {
                     let {
                         sourceBuffer: e,
                         readOffset: n = 0,
                         writeOffset: i = 0,
                         size: r
                     } = t;
                     const {
                         gl: s
                     } = this;
-                    return Lu(s), s.bindBuffer(36662, e.handle), s.bindBuffer(36663, this.handle), s.copyBufferSubData(36662, 36663, n, i, r), s.bindBuffer(36662, null), s.bindBuffer(36663, null), this.debugData = null, this
+                    return Ou(s), s.bindBuffer(36662, e.handle), s.bindBuffer(36663, this.handle), s.copyBufferSubData(36662, 36663, n, i, r), s.bindBuffer(36662, null), s.bindBuffer(36663, null), this.debugData = null, this
                 }
                 getData() {
                     let {
                         dstData: t = null,
                         srcByteOffset: e = 0,
                         dstOffset: n = 0,
                         length: i = 0
                     } = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
-                    Lu(this.gl);
-                    const r = Rd(this.accessor.type || 5126, {
+                    Ou(this.gl);
+                    const r = Id(this.accessor.type || 5126, {
                             clamped: !1
                         }),
                         s = this._getAvailableElementCount(e),
                         o = n;
                     let a, l;
                     t ? (l = t.length, a = l - o) : (a = Math.min(s, i || s), l = o + a);
                     const c = Math.min(s, a);
@@ -11346,15 +11347,15 @@
                 }
                 _setData(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 0,
                         n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : t.byteLength + e;
                     wd(ArrayBuffer.isView(t)), this._trackDeallocatedMemory();
                     const i = this._getTarget();
                     this.gl.bindBuffer(i, this.handle), this.gl.bufferData(i, n, this.usage), this.gl.bufferSubData(i, e, t), this.gl.bindBuffer(i, null), this.debugData = t.slice(0, 10), this.bytesUsed = n, this._trackAllocatedMemory(n);
-                    const r = Id(t);
+                    const r = Rd(t);
                     return wd(r), this.setAccessor(new Dd(this.accessor, {
                         type: r
                     })), this
                 }
                 _setByteLength(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.usage;
                     wd(t >= 0), this._trackDeallocatedMemory();
@@ -11363,22 +11364,22 @@
                     const i = this._getTarget();
                     return this.gl.bindBuffer(i, this.handle), this.gl.bufferData(i, n, e), this.gl.bindBuffer(i, null), this.usage = e, this.debugData = null, this.bytesUsed = t, this._trackAllocatedMemory(t), this
                 }
                 _getTarget() {
                     return this.gl.webgl2 ? 36663 : this.target
                 }
                 _getAvailableElementCount(t) {
-                    const e = t / Rd(this.accessor.type || 5126, {
+                    const e = t / Id(this.accessor.type || 5126, {
                         clamped: !1
                     }).BYTES_PER_ELEMENT;
                     return this.getElementCount() - e
                 }
                 _inferType(t) {
                     this.accessor.type || this.setAccessor(new Dd(this.accessor, {
-                        type: Id(t)
+                        type: Rd(t)
                     }))
                 }
                 _createHandle() {
                     return this.gl.createBuffer()
                 }
                 _deleteHandle() {
                     this.gl.deleteBuffer(this.handle), this._trackDeallocatedMemory()
@@ -11466,15 +11467,15 @@
                     5122: 2,
                     5131: 2,
                     5120: 1,
                     5121: 1
                 },
                 qd = [9729, 9728],
                 Xd = globalThis.WebGLBuffer || function() {};
-            class Yd extends Ld {
+            class Yd extends Od {
                 get[Symbol.toStringTag]() {
                     return "Texture"
                 }
                 static isSupported(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                     const {
                         format: n,
@@ -11663,15 +11664,15 @@
                                 case "null":
                                     f.texImage2D(e, i, r, h, u, s, d, c, l);
                                     break;
                                 case "typed-array":
                                     f.texImage2D(e, i, r, h, u, s, d, c, l, o);
                                     break;
                                 case "buffer":
-                                    g = Lu(f), g.bindBuffer(35052, l.handle || l), g.texImage2D(e, i, r, h, u, s, d, c, o), g.bindBuffer(35052, null);
+                                    g = Ou(f), g.bindBuffer(35052, l.handle || l), g.texImage2D(e, i, r, h, u, s, d, c, o), g.bindBuffer(35052, null);
                                     break;
                                 case "browser-object":
                                     Mu(f) ? f.texImage2D(e, i, r, h, u, s, d, c, l) : f.texImage2D(e, i, r, d, c, l);
                                     break;
                                 case "compressed":
                                     for (const [t, n] of l.entries()) f.compressedTexImage2D(e, t, n.format, n.width, n.height, s, n.data), v += n.levelSize;
                                     break;
@@ -11724,17 +11725,17 @@
                         i = t.data, o = t.shape[0], a = t.shape[1]
                     }
                     i instanceof Gd && (i = i.handle), this.gl.bindTexture(this.target, this.handle), cd(this.gl, g, (() => {
                         if (d) this.gl.compressedTexSubImage2D(e, l, r, s, o, a, c, i);
                         else if (null === i) this.gl.texSubImage2D(e, l, r, s, o, a, u, h, null);
                         else if (ArrayBuffer.isView(i)) this.gl.texSubImage2D(e, l, r, s, o, a, u, h, i, p);
                         else if (i instanceof Xd) {
-                            const t = Lu(this.gl);
+                            const t = Ou(this.gl);
                             t.bindBuffer(35052, i), t.texSubImage2D(e, l, r, s, o, a, u, h, p), t.bindBuffer(35052, null)
-                        } else Mu(this.gl) ? Lu(this.gl).texSubImage2D(e, l, r, s, o, a, u, h, i) : this.gl.texSubImage2D(e, l, r, s, u, h, i)
+                        } else Mu(this.gl) ? Ou(this.gl).texSubImage2D(e, l, r, s, o, a, u, h, i) : this.gl.texSubImage2D(e, l, r, s, u, h, i)
                     })), this.gl.bindTexture(this.target, null)
                 }
                 copyFramebuffer() {
                     return Su.error("Texture.copyFramebuffer({...}) is no logner supported, use copyToTexture(source, target, opts})")(), null
                 }
                 getActiveUnit() {
                     return this.gl.getParameter(34016) - 33984
@@ -11883,15 +11884,15 @@
                 }
                 static isSupported(t, e) {
                     return Yd.isSupported(t, e)
                 }
                 constructor(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                     var n;
-                    Ou(t), (e instanceof Promise || "string" == typeof e) && (e = {
+                    Lu(t), (e instanceof Promise || "string" == typeof e) && (e = {
                         data: e
                     }), "string" == typeof e.data && (e = Object.assign({}, e, {
                         data: (n = e.data, wd("string" == typeof n), n = "" + n, new Promise(((t, e) => {
                             try {
                                 const i = new Image;
                                 i.onload = () => t(i), i.onerror = () => e(new Error("Could not load image ".concat(n, "."))), i.crossOrigin = "anonymous", i.src = n
                             } catch (t) {
@@ -11899,16 +11900,16 @@
                             }
                         })))
                     })), super(t, Object.assign({}, e, {
                         target: 3553
                     })), this.initialize(e), Object.seal(this)
                 }
             }
-            const $d = "EXT_color_buffer_float",
-                Jd = {
+            const Jd = "EXT_color_buffer_float",
+                Qd = {
                     33189: {
                         bpp: 2
                     },
                     33190: {
                         gl2: !0,
                         bpp: 3
                     },
@@ -12032,58 +12033,58 @@
                         bpp: 16
                     },
                     36208: {
                         gl2: !0,
                         bpp: 16
                     },
                     33325: {
-                        gl2: $d,
+                        gl2: Jd,
                         bpp: 2
                     },
                     33327: {
-                        gl2: $d,
+                        gl2: Jd,
                         bpp: 4
                     },
                     34842: {
-                        gl2: $d,
+                        gl2: Jd,
                         bpp: 8
                     },
                     33326: {
-                        gl2: $d,
+                        gl2: Jd,
                         bpp: 4
                     },
                     33328: {
-                        gl2: $d,
+                        gl2: Jd,
                         bpp: 8
                     },
                     34836: {
-                        gl2: $d,
+                        gl2: Jd,
                         bpp: 16
                     },
                     35898: {
-                        gl2: $d,
+                        gl2: Jd,
                         bpp: 4
                     }
                 };
-            class Qd extends Ld {
+            class $d extends Od {
                 get[Symbol.toStringTag]() {
                     return "Renderbuffer"
                 }
                 static isSupported(t) {
                     let {
                         format: e
                     } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {
                         format: null
                     };
                     return !e || function(t, e, n) {
                         const i = n[e];
                         if (!i) return !1;
                         const r = Mu(t) && i.gl2 || i.gl1;
                         return "string" == typeof r ? t.getExtension(r) : r
-                    }(t, e, Jd)
+                    }(t, e, Qd)
                 }
                 static getSamplesForFormat(t, e) {
                     let {
                         format: n
                     } = e;
                     return t.getInternalformatParameter(36161, n, 32937)
                 }
@@ -12094,15 +12095,15 @@
                 initialize(t) {
                     let {
                         format: e,
                         width: n = 1,
                         height: i = 1,
                         samples: r = 0
                     } = t;
-                    return wd(e, "Needs format"), this._trackDeallocatedMemory(), this.gl.bindRenderbuffer(36161, this.handle), 0 !== r && Mu(this.gl) ? this.gl.renderbufferStorageMultisample(36161, r, e, n, i) : this.gl.renderbufferStorage(36161, e, n, i), this.format = e, this.width = n, this.height = i, this.samples = r, this._trackAllocatedMemory(this.width * this.height * (this.samples || 1) * Jd[this.format].bpp), this
+                    return wd(e, "Needs format"), this._trackDeallocatedMemory(), this.gl.bindRenderbuffer(36161, this.handle), 0 !== r && Mu(this.gl) ? this.gl.renderbufferStorageMultisample(36161, r, e, n, i) : this.gl.renderbufferStorage(36161, e, n, i), this.format = e, this.width = n, this.height = i, this.samples = r, this._trackAllocatedMemory(this.width * this.height * (this.samples || 1) * Qd[this.format].bpp), this
                 }
                 resize(t) {
                     let {
                         width: e,
                         height: n
                     } = t;
                     return e !== this.width || n !== this.height ? this.initialize({
@@ -12148,15 +12149,15 @@
             const ip = [34069, 34070, 34071, 34072, 34073, 34074];
             class rp extends Yd {
                 get[Symbol.toStringTag]() {
                     return "TextureCube"
                 }
                 constructor(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
-                    Ou(t), super(t, Object.assign({}, e, {
+                    Lu(t), super(t, Object.assign({}, e, {
                         target: 34067
                     })), this.initialize(e), Object.seal(this)
                 }
                 initialize() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     const {
                         mipmaps: e = !0,
@@ -12230,15 +12231,15 @@
                     return "Texture3D"
                 }
                 static isSupported(t) {
                     return Mu(t)
                 }
                 constructor(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
-                    Lu(t), e = Object.assign({
+                    Ou(t), e = Object.assign({
                         depth: 1
                     }, e, {
                         target: 32879,
                         unpackFlipY: !1
                     }), super(t, e), this.initialize(e), Object.seal(this)
                 }
                 setImageData(t) {
@@ -12306,15 +12307,15 @@
                 const {
                     gl: d,
                     handle: p,
                     attachments: f
                 } = h;
                 a = a || h.width, l = l || h.height, 36064 === s && null === p && (s = 1028), wd(f[s]), c = c || f[s].type, o = function(t, e, n, i, r) {
                     if (t) return t;
-                    const s = Rd(e = e || 5121, {
+                    const s = Id(e = e || 5121, {
                             clamped: !1
                         }),
                         o = function(t) {
                             switch (t) {
                                 case 6406:
                                 case 33326:
                                 case 6403:
@@ -12329,15 +12330,15 @@
                                 case 34836:
                                     return 4;
                                 default:
                                     return wd(!1), 0
                             }
                         }(n);
                     return new s(i * r * o)
-                }(o, c, r, a, l), c = c || Id(o);
+                }(o, c, r, a, l), c = c || Rd(o);
                 const g = d.bindFramebuffer(36160, p);
                 return d.readPixels(n, i, a, l, r, c, o), d.bindFramebuffer(36160, g || null), u && h.delete(), o
             }
 
             function lp(t) {
                 let {
                     sourceAttachment: e = 36064,
@@ -12451,15 +12452,15 @@
                         i = !0;
                         for (const e of r) i = i && Boolean(t.getExtension(e))
                     } else "string" == typeof r ? i = Boolean(t.getExtension(r)) : "boolean" == typeof r ? i = r : wd(!1);
                     return i
                 }(t, e)), t.luma.caps[e] || Su.log(pp, "Feature: ".concat(e, " not supported"))(), t.luma.caps[e]
             }
             const mp = "Multiple render targets not supported";
-            class vp extends Ld {
+            class vp extends Od {
                 get[Symbol.toStringTag]() {
                     return "Framebuffer"
                 }
                 static isSupported(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                     const {
                         colorBufferFloat: n,
@@ -12472,19 +12473,19 @@
                     return t.luma = t.luma || {}, t.luma.defaultFramebuffer = t.luma.defaultFramebuffer || new vp(t, {
                         id: "default-framebuffer",
                         handle: null,
                         attachments: {}
                     }), t.luma.defaultFramebuffer
                 }
                 get MAX_COLOR_ATTACHMENTS() {
-                    const t = Lu(this.gl);
+                    const t = Ou(this.gl);
                     return t.getParameter(t.MAX_COLOR_ATTACHMENTS)
                 }
                 get MAX_DRAW_BUFFERS() {
-                    const t = Lu(this.gl);
+                    const t = Ou(this.gl);
                     return t.getParameter(t.MAX_DRAW_BUFFERS)
                 }
                 constructor(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                     super(t, e), this.width = null, this.height = null, this.attachments = {}, this.readBuffer = 36064, this.drawBuffers = [36064], this.ownResources = [], this.initialize(e), Object.seal(this)
                 }
                 get color() {
@@ -12573,15 +12574,15 @@
                     const r = this.gl.bindFramebuffer(36160, this.handle);
                     for (const t in i) {
                         wd(void 0 !== t, "Misspelled framebuffer binding point?");
                         const e = Number(t),
                             r = i[e];
                         let s = r;
                         if (s)
-                            if (s instanceof Qd) this._attachRenderbuffer({
+                            if (s instanceof $d) this._attachRenderbuffer({
                                 attachment: e,
                                 renderbuffer: s
                             });
                             else if (Array.isArray(r)) {
                             const [t, n = 0, i = 0] = r;
                             s = t, this._attachTexture({
                                 attachment: e,
@@ -12636,15 +12637,15 @@
                         ! function(t) {
                             let {
                                 framebuffer: e = null,
                                 buffer: n = tp,
                                 drawBuffer: i = 0,
                                 value: r = [0, 0, 0, 0]
                             } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
-                            Lu(t), cd(t, {
+                            Ou(t), cd(t, {
                                 framebuffer: e
                             }, (() => {
                                 switch (n) {
                                     case tp:
                                         switch (r.constructor) {
                                             case Int32Array:
                                                 t.clearBufferiv(n, i, r);
@@ -12699,15 +12700,15 @@
                     let {
                         attachments: e = [],
                         x: n = 0,
                         y: i = 0,
                         width: r,
                         height: s
                     } = t;
-                    const o = Lu(this.gl),
+                    const o = Ou(this.gl),
                         a = o.bindFramebuffer(36008, this.handle);
                     return 0 === n && 0 === i && void 0 === r && void 0 === s ? o.invalidateFramebuffer(36008, e) : o.invalidateFramebuffer(36008, e, n, i, r, s), o.bindFramebuffer(36008, a), this
                 }
                 getAttachmentParameter(t, e, n) {
                     let i = this._getAttachmentParameterFallback(e);
                     return null === i && (this.gl.bindFramebuffer(36160, this.handle), i = this.gl.getFramebufferAttachmentParameter(36160, t, e), this.gl.bindFramebuffer(36160, null)), n && i > 1e3 && (i = Pd(this.gl, i)), i
                 }
@@ -12770,29 +12771,29 @@
                         mipmaps: !1,
                         parameters: {
                             10241: 9729,
                             10240: 9729,
                             10242: 33071,
                             10243: 33071
                         }
-                    }), this.ownResources.push(s[36064])), e && n ? (s = s || {}, s[33306] = new Qd(this.gl, {
+                    }), this.ownResources.push(s[36064])), e && n ? (s = s || {}, s[33306] = new $d(this.gl, {
                         id: "".concat(this.id, "-depth-stencil"),
                         format: 35056,
                         width: i,
                         height: 111
-                    }), this.ownResources.push(s[33306])) : e ? (s = s || {}, s[36096] = new Qd(this.gl, {
+                    }), this.ownResources.push(s[33306])) : e ? (s = s || {}, s[36096] = new $d(this.gl, {
                         id: "".concat(this.id, "-depth"),
                         format: 33189,
                         width: i,
                         height: r
                     }), this.ownResources.push(s[36096])) : n && wd(!1), s
                 }
                 _unattach(t) {
                     const e = this.attachments[t];
-                    e && (e instanceof Qd ? this.gl.framebufferRenderbuffer(36160, t, 36161, null) : this.gl.framebufferTexture2D(36160, t, 3553, null, 0), delete this.attachments[t])
+                    e && (e instanceof $d ? this.gl.framebufferRenderbuffer(36160, t, 36161, null) : this.gl.framebufferTexture2D(36160, t, 3553, null, 0), delete this.attachments[t])
                 }
                 _attachRenderbuffer(t) {
                     let {
                         attachment: e = 36064,
                         renderbuffer: n
                     } = t;
                     const {
@@ -12809,15 +12810,15 @@
                     } = t;
                     const {
                         gl: s
                     } = this;
                     switch (s.bindTexture(n.target, n.handle), n.target) {
                         case 35866:
                         case 32879:
-                            Lu(s).framebufferTextureLayer(36160, e, n.target, r, i);
+                            Ou(s).framebufferTextureLayer(36160, e, n.target, r, i);
                             break;
                         case 34067:
                             const t = function(t) {
                                 return t < 34069 ? t + 34069 : t
                             }(i);
                             s.framebufferTexture2D(36160, e, t, n.handle, r);
                             break;
@@ -12833,15 +12834,15 @@
                     const e = Mu(n = this.gl) ? n : null;
                     var n;
                     e ? e.readBuffer(t) : wd(36064 === t || 1029 === t, mp), this.readBuffer = t
                 }
                 _setDrawBuffers(t) {
                     const {
                         gl: e
-                    } = this, n = Lu(e);
+                    } = this, n = Ou(e);
                     if (n) n.drawBuffers(t);
                     else {
                         const n = e.getExtension("WEBGL_draw_buffers");
                         n ? n.drawBuffersWEBGL(t) : wd(1 === t.length && (36064 === t[0] || 1029 === t[0]), mp)
                     }
                     this.drawBuffers = t
                 }
@@ -12877,56 +12878,56 @@
                 }
                 _bindHandle(t) {
                     return this.gl.bindFramebuffer(36160, t)
                 }
             }
             vp.ATTACHMENT_PARAMETERS = [36049, 36048, 33296, 33298, 33299, 33300, 33301, 33302, 33303];
             const bp = {
-                    5126: kp.bind(null, "uniform1fv", Pp, 1, Ip),
-                    35664: kp.bind(null, "uniform2fv", Pp, 2, Ip),
-                    35665: kp.bind(null, "uniform3fv", Pp, 3, Ip),
-                    35666: kp.bind(null, "uniform4fv", Pp, 4, Ip),
-                    5124: kp.bind(null, "uniform1iv", Sp, 1, Ip),
-                    35667: kp.bind(null, "uniform2iv", Sp, 2, Ip),
-                    35668: kp.bind(null, "uniform3iv", Sp, 3, Ip),
-                    35669: kp.bind(null, "uniform4iv", Sp, 4, Ip),
-                    35670: kp.bind(null, "uniform1iv", Sp, 1, Ip),
-                    35671: kp.bind(null, "uniform2iv", Sp, 2, Ip),
-                    35672: kp.bind(null, "uniform3iv", Sp, 3, Ip),
-                    35673: kp.bind(null, "uniform4iv", Sp, 4, Ip),
-                    35674: kp.bind(null, "uniformMatrix2fv", Pp, 4, Rp),
-                    35675: kp.bind(null, "uniformMatrix3fv", Pp, 9, Rp),
-                    35676: kp.bind(null, "uniformMatrix4fv", Pp, 16, Rp),
-                    35678: Lp,
-                    35680: Lp,
-                    5125: kp.bind(null, "uniform1uiv", Cp, 1, Ip),
-                    36294: kp.bind(null, "uniform2uiv", Cp, 2, Ip),
-                    36295: kp.bind(null, "uniform3uiv", Cp, 3, Ip),
-                    36296: kp.bind(null, "uniform4uiv", Cp, 4, Ip),
-                    35685: kp.bind(null, "uniformMatrix2x3fv", Pp, 6, Rp),
-                    35686: kp.bind(null, "uniformMatrix2x4fv", Pp, 8, Rp),
-                    35687: kp.bind(null, "uniformMatrix3x2fv", Pp, 6, Rp),
-                    35688: kp.bind(null, "uniformMatrix3x4fv", Pp, 12, Rp),
-                    35689: kp.bind(null, "uniformMatrix4x2fv", Pp, 8, Rp),
-                    35690: kp.bind(null, "uniformMatrix4x3fv", Pp, 12, Rp),
-                    35678: Lp,
-                    35680: Lp,
-                    35679: Lp,
-                    35682: Lp,
-                    36289: Lp,
-                    36292: Lp,
-                    36293: Lp,
-                    36298: Lp,
-                    36299: Lp,
-                    36300: Lp,
-                    36303: Lp,
-                    36306: Lp,
-                    36307: Lp,
-                    36308: Lp,
-                    36311: Lp
+                    5126: kp.bind(null, "uniform1fv", Pp, 1, Rp),
+                    35664: kp.bind(null, "uniform2fv", Pp, 2, Rp),
+                    35665: kp.bind(null, "uniform3fv", Pp, 3, Rp),
+                    35666: kp.bind(null, "uniform4fv", Pp, 4, Rp),
+                    5124: kp.bind(null, "uniform1iv", Sp, 1, Rp),
+                    35667: kp.bind(null, "uniform2iv", Sp, 2, Rp),
+                    35668: kp.bind(null, "uniform3iv", Sp, 3, Rp),
+                    35669: kp.bind(null, "uniform4iv", Sp, 4, Rp),
+                    35670: kp.bind(null, "uniform1iv", Sp, 1, Rp),
+                    35671: kp.bind(null, "uniform2iv", Sp, 2, Rp),
+                    35672: kp.bind(null, "uniform3iv", Sp, 3, Rp),
+                    35673: kp.bind(null, "uniform4iv", Sp, 4, Rp),
+                    35674: kp.bind(null, "uniformMatrix2fv", Pp, 4, Ip),
+                    35675: kp.bind(null, "uniformMatrix3fv", Pp, 9, Ip),
+                    35676: kp.bind(null, "uniformMatrix4fv", Pp, 16, Ip),
+                    35678: Op,
+                    35680: Op,
+                    5125: kp.bind(null, "uniform1uiv", Cp, 1, Rp),
+                    36294: kp.bind(null, "uniform2uiv", Cp, 2, Rp),
+                    36295: kp.bind(null, "uniform3uiv", Cp, 3, Rp),
+                    36296: kp.bind(null, "uniform4uiv", Cp, 4, Rp),
+                    35685: kp.bind(null, "uniformMatrix2x3fv", Pp, 6, Ip),
+                    35686: kp.bind(null, "uniformMatrix2x4fv", Pp, 8, Ip),
+                    35687: kp.bind(null, "uniformMatrix3x2fv", Pp, 6, Ip),
+                    35688: kp.bind(null, "uniformMatrix3x4fv", Pp, 12, Ip),
+                    35689: kp.bind(null, "uniformMatrix4x2fv", Pp, 8, Ip),
+                    35690: kp.bind(null, "uniformMatrix4x3fv", Pp, 12, Ip),
+                    35678: Op,
+                    35680: Op,
+                    35679: Op,
+                    35682: Op,
+                    36289: Op,
+                    36292: Op,
+                    36293: Op,
+                    36298: Op,
+                    36299: Op,
+                    36300: Op,
+                    36303: Op,
+                    36306: Op,
+                    36307: Op,
+                    36308: Op,
+                    36311: Op
                 },
                 yp = {},
                 _p = {},
                 xp = {},
                 wp = [0];
 
             function Ep(t, e, n, i) {
@@ -12975,27 +12976,27 @@
             function Mp(t) {
                 return Array.isArray(t) || ArrayBuffer.isView(t) ? function(t) {
                     if (0 === t.length) return !1;
                     const e = Math.min(t.length, 16);
                     for (let n = 0; n < e; ++n)
                         if (!Number.isFinite(t[n])) return !1;
                     return !0
-                }(t) : !!isFinite(t) || !0 === t || !1 === t || t instanceof Yd || t instanceof Qd || t instanceof vp && Boolean(t.texture)
+                }(t) : !!isFinite(t) || !0 === t || !1 === t || t instanceof Yd || t instanceof $d || t instanceof vp && Boolean(t.texture)
             }
 
-            function Op(t, e, n) {
+            function Lp(t, e, n) {
                 if (Array.isArray(n) || ArrayBuffer.isView(n))
                     if (t[e]) {
                         const i = t[e];
                         for (let t = 0, e = n.length; t < e; ++t) i[t] = n[t]
                     } else t[e] = n.slice();
                 else t[e] = n
             }
 
-            function Lp() {
+            function Op() {
                 let t = null;
                 return (e, n, i) => {
                     const r = t !== i;
                     return r && (e.uniform1i(n, i), t = i), r
                 }
             }
 
@@ -13015,65 +13016,65 @@
                                 break
                             }
                     }
                     return u && (i(o, t, a, c), r.set(c)), u
                 }
             }
 
-            function Ip(t, e, n, i) {
+            function Rp(t, e, n, i) {
                 t[e](n, i)
             }
 
-            function Rp(t, e, n, i) {
+            function Ip(t, e, n, i) {
                 t[e](n, !1, i)
             }
 
             function jp(t) {
                 let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "unnamed";
                 const n = t.match(/#define[\s*]SHADER_NAME[\s*]([A-Za-z0-9_-]+)[\s*]/);
                 return n ? n[1] : e
             }
 
-            function zp(t, e) {
+            function Fp(t, e) {
                 let n = "";
                 for (let i = 0; i < e.length; i++) {
                     const r = e[i];
                     if ((t[i + 3] || t[i + 2] || t[i + 1]) && (n += "".concat(r, "\n"), t[i + 1])) {
                         const e = t[i + 1],
                             r = e.split(":", 3),
                             s = r[0],
                             o = parseInt(r[1], 10) || 0,
                             a = e.substring(r.join(":").length + 1).trim();
-                        n += Fp("^^^ ".concat(s, ": ").concat(a, "\n\n"), o)
+                        n += zp("^^^ ".concat(s, ": ").concat(a, "\n\n"), o)
                     }
                 }
                 return n
             }
 
-            function Fp(t, e) {
+            function zp(t, e) {
                 let n = "";
                 for (let t = 0; t < e; ++t) n += " ";
                 return "".concat(n).concat(t)
             }
-            class Bp extends Ld {
+            class Bp extends Od {
                 get[Symbol.toStringTag]() {
                     return "Shader"
                 }
                 static getTypeName(t) {
                     switch (t) {
                         case 35633:
                             return "vertex-shader";
                         case 35632:
                             return "fragment-shader";
                         default:
                             return wd(!1), "unknown"
                     }
                 }
                 constructor(t, e) {
-                    Ou(t), wd("string" == typeof e.source, "Shader: GLSL source code must be a JavaScript string"), super(t, {
+                    Lu(t), wd("string" == typeof e.source, "Shader: GLSL source code must be a JavaScript string"), super(t, {
                         id: jp(e.source, null) || e.id || Cd("unnamed ".concat(Bp.getTypeName(e.shaderType)))
                     }), this.shaderType = e.shaderType, this.source = e.source, this.initialize(e)
                 }
                 initialize(t) {
                     let {
                         source: e
                     } = t;
@@ -13132,21 +13133,21 @@
                                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 1,
                                         n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : ": ";
                                     const i = t.split(/\r?\n/),
                                         r = String(i.length + e - 1).length;
                                     return i.map(((t, i) => {
                                         const s = String(i + e),
                                             o = s.length;
-                                        return Fp(s, r - o) + n + t
+                                        return zp(s, r - o) + n + t
                                     }))
                                 }(e);
                                 return {
                                     shaderName: l,
-                                    errors: zp(s, c),
-                                    warnings: zp(o, c)
+                                    errors: Fp(s, c),
+                                    warnings: Fp(o, c)
                                 }
                             }(t, this.source, this.shaderType, this.id);
                         throw Su.error("GLSL compilation errors in ".concat(e, "\n").concat(n))(), Su.warn("GLSL compilation warnings in ".concat(e, "\n").concat(i))(), new Error("GLSL compilation errors in ".concat(e))
                     }
                 }
                 _deleteHandle() {
                     this.gl.deleteShader(this.handle)
@@ -13246,15 +13247,15 @@
                     if (i === t && r === e) return {
                         glType: n,
                         name: s
                     }
                 }
                 return null
             }
-            class $p {
+            class Jp {
                 constructor(t) {
                     this.id = t.id, this.attributeInfos = [], this.attributeInfosByName = {}, this.attributeInfosByLocation = [], this.varyingInfos = [], this.varyingInfosByName = {}, Object.seal(this), this._readAttributesFromProgram(t), this._readVaryingsFromProgram(t)
                 }
                 getAttributeInfo(t) {
                     const e = Number(t);
                     return Number.isFinite(e) ? this.attributeInfosByLocation[e] : this.attributeInfosByName[t] || null
                 }
@@ -13338,40 +13339,40 @@
                             type: r,
                             size: i * s
                         })
                     };
                     this.varyingInfos.push(o), this.varyingInfosByName[o.name] = o
                 }
             }
-            const Jp = 35981,
-                Qp = ["setVertexArray", "setAttributes", "setBuffers", "unsetBuffers", "use", "getUniformCount", "getUniformInfo", "getUniformLocation", "getUniformValue", "getVarying", "getFragDataLocation", "getAttachedShaders", "getAttributeCount", "getAttributeLocation", "getAttributeInfo"];
-            class tf extends Ld {
+            const Qp = 35981,
+                $p = ["setVertexArray", "setAttributes", "setBuffers", "unsetBuffers", "use", "getUniformCount", "getUniformInfo", "getUniformLocation", "getUniformValue", "getVarying", "getFragDataLocation", "getAttachedShaders", "getAttributeCount", "getAttributeLocation", "getAttributeInfo"];
+            class tf extends Od {
                 get[Symbol.toStringTag]() {
                     return "Program"
                 }
                 constructor(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
-                    super(t, e), this.stubRemovedMethods("Program", "v6.0", Qp), this._isCached = !1, this.initialize(e), Object.seal(this), this._setId(e.id)
+                    super(t, e), this.stubRemovedMethods("Program", "v6.0", $p), this._isCached = !1, this.initialize(e), Object.seal(this), this._setId(e.id)
                 }
                 initialize() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     const {
                         hash: e,
                         vs: n,
                         fs: i,
                         varyings: r,
-                        bufferMode: s = Jp
+                        bufferMode: s = Qp
                     } = t;
                     return this.hash = e || "", this.vs = "string" == typeof n ? new Dp(this.gl, {
                         id: "".concat(t.id, "-vs"),
                         source: n
                     }) : n, this.fs = "string" == typeof i ? new Np(this.gl, {
                         id: "".concat(t.id, "-fs"),
                         source: i
-                    }) : i, wd(this.vs instanceof Dp), wd(this.fs instanceof Np), this.uniforms = {}, this._textureUniforms = {}, r && r.length > 0 && (Lu(this.gl), this.varyings = r, this.gl2.transformFeedbackVaryings(this.handle, r, s)), this._compileAndLink(), this._readUniformLocationsFromLinkedProgram(), this.configuration = new $p(this), this.setProps(t)
+                    }) : i, wd(this.vs instanceof Dp), wd(this.fs instanceof Np), this.uniforms = {}, this._textureUniforms = {}, r && r.length > 0 && (Ou(this.gl), this.varyings = r, this.gl2.transformFeedbackVaryings(this.handle, r, s)), this._compileAndLink(), this._readUniformLocationsFromLinkedProgram(), this.configuration = new Jp(this), this.setProps(t)
                 }
                 delete() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     return this._isCached ? this : super.delete(t)
                 }
                 setProps(t) {
                     return "uniforms" in t && this.setUniforms(t.uniforms), this
@@ -13447,15 +13448,15 @@
                                     const n = t,
                                         {
                                             textureIndex: r
                                         } = i;
                                     n.bind(r), t = r, this._textureUniforms[e] = n
                                 } else t = i.textureIndex;
                             else this._textureUniforms[e] && delete this._textureUniforms[e];
-                            (i(t) || r) && Op(this.uniforms, e, n)
+                            (i(t) || r) && Lp(this.uniforms, e, n)
                         }
                     }
                     return this
                 }
                 _areTexturesRenderable() {
                     let t = !0;
                     for (const e in this._textureUniforms) {
@@ -13704,15 +13705,15 @@
                             viewProjectionMatrix: o
                         } = t, a = uf, l = uf, c = t.cameraPosition;
                         const {
                             geospatialOrigin: h,
                             shaderCoordinateOrigin: u,
                             offsetMode: d
                         } = vf(t, e, n);
-                        return d && (l = t.projectPosition(h || u), c = [c[0] - l[0], c[1] - l[1], c[2] - l[2]], l[3] = 1, a = qc([], l, o), s = i || s, o = Fc([], r, s), o = Fc([], o, df)), {
+                        return d && (l = t.projectPosition(h || u), c = [c[0] - l[0], c[1] - l[1], c[2] - l[2]], l[3] = 1, a = qc([], l, o), s = i || s, o = zc([], r, s), o = zc([], o, df)), {
                             viewMatrix: s,
                             viewProjectionMatrix: o,
                             projectionCenter: a,
                             originCommon: l,
                             cameraPosCommon: c,
                             shaderCoordinateOrigin: u,
                             geospatialOrigin: h
@@ -13835,15 +13836,15 @@
                         layerManager: this,
                         gl: t,
                         deck: e,
                         programManager: t && wf(t),
                         stats: n || new ca({
                             id: "deck.gl"
                         }),
-                        viewport: i || new Fh({
+                        viewport: i || new zh({
                             id: "DEFAULT-INITIAL-VIEWPORT"
                         }),
                         timeline: r || new So,
                         resourceManager: this.resourceManager,
                         onError: void 0
                     }, Object.seal(this)
                 }
@@ -14137,27 +14138,27 @@
             function Af(t, e) {
                 return t.relative ? Math.round(t.position * e) : t.position
             }
 
             function Mf(t, e) {
                 if (!t) throw new Error(e || "deck.gl: assertion failed.")
             }
-            class Of {
+            class Lf {
                 constructor(t) {
                     wo(this, "id", void 0), wo(this, "viewportInstance", void 0), wo(this, "_x", void 0), wo(this, "_y", void 0), wo(this, "_width", void 0), wo(this, "_height", void 0), wo(this, "_padding", void 0), wo(this, "props", void 0);
                     const {
                         id: e,
                         x: n = 0,
                         y: i = 0,
                         width: r = "100%",
                         height: s = "100%",
                         padding: o = null,
                         viewportInstance: a
                     } = t || {};
-                    Mf(!a || a instanceof Fh), this.viewportInstance = a, this.id = e || this.constructor.displayName || "view", this.props = {
+                    Mf(!a || a instanceof zh), this.viewportInstance = a, this.id = e || this.constructor.displayName || "view", this.props = {
                         ...t,
                         id: this.id
                     }, this._x = Tf(n), this._y = Tf(i), this._width = Tf(r), this._height = Tf(s), this._padding = o && {
                         left: Tf(o.left || 0),
                         right: Tf(o.right || 0),
                         top: Tf(o.top || 0),
                         bottom: Tf(o.bottom || 0)
@@ -14225,20 +14226,20 @@
                         type: t
                     } : {
                         type: this.ControllerType,
                         ...t
                     } : null
                 }
             }
-            const Lf = Math.PI / 180;
+            const Of = Math.PI / 180;
 
             function kf(t) {
-                return 512 / 4003e4 / Math.cos(t * Lf)
+                return 512 / 4003e4 / Math.cos(t * Of)
             }
-            class If extends Fh {
+            class Rf extends zh {
                 constructor(t = {}) {
                     const {
                         latitude: e = 0,
                         longitude: n = 0,
                         zoom: i = 0,
                         pitch: r = 0,
                         bearing: s = 0,
@@ -14315,15 +14316,15 @@
                     }({
                         height: f,
                         pitch: r,
                         bearing: s,
                         scale: m,
                         altitude: g
                     });
-                    u && (y = (new Qc).translate([512 * u, 0, 0]).multiplyLeft(y)), super({
+                    u && (y = (new $c).translate([512 * u, 0, 0]).multiplyLeft(y)), super({
                         ...t,
                         width: p,
                         height: f,
                         viewMatrix: y,
                         longitude: n,
                         latitude: e,
                         zoom: i,
@@ -14334,15 +14335,15 @@
                 }
                 get subViewports() {
                     if (this._subViewports && !this._subViewports.length) {
                         const t = this.getBounds(),
                             e = Math.floor((t[0] + 180) / 360),
                             n = Math.ceil((t[2] - 180) / 360);
                         for (let t = e; t <= n; t++) {
-                            const e = t ? new If({
+                            const e = t ? new Rf({
                                 ...this,
                                 worldOffset: t
                             }) : this;
                             this._subViewports.push(e)
                         }
                     }
                     return this._subViewports
@@ -14394,25 +14395,25 @@
                         zoom: o
                     } = Ph({
                         width: n,
                         height: i,
                         bounds: t,
                         ...e
                     });
-                    return new If({
+                    return new Rf({
                         width: n,
                         height: i,
                         longitude: r,
                         latitude: s,
                         zoom: o
                     })
                 }
             }
-            wo(If, "displayName", "WebMercatorViewport");
-            class Rf {
+            wo(Rf, "displayName", "WebMercatorViewport");
+            class If {
                 constructor(t) {
                     wo(this, "_inProgress", void 0), wo(this, "_handle", void 0), wo(this, "_timeline", void 0), wo(this, "time", void 0), wo(this, "settings", void 0), this._inProgress = !1, this._handle = null, this._timeline = t, this.time = 0, this.settings = {
                         duration: 0
                     }
                 }
                 get inProgress() {
                     return this._inProgress
@@ -14443,16 +14444,16 @@
                         })
                     }
                     return this.time = this._timeline.getTime(this._handle), this._onUpdate(), null === (t = (e = this.settings).onUpdate) || void 0 === t || t.call(e, this), this._timeline.isFinished(this._handle) && this.end(), !0
                 }
                 _onUpdate() {}
             }
             const jf = () => {},
-                zf = t => t;
-            class Ff {
+                Ff = t => t;
+            class zf {
                 constructor(t) {
                     wo(this, "getControllerState", void 0), wo(this, "props", void 0), wo(this, "propsInTransition", void 0), wo(this, "transition", void 0), wo(this, "onViewStateChange", void 0), wo(this, "onStateChange", void 0), wo(this, "_onTransitionUpdate", (t => {
                         const {
                             time: e,
                             settings: {
                                 interpolator: n,
                                 startProps: i,
@@ -14464,15 +14465,15 @@
                         this.propsInTransition = this.getControllerState({
                             ...this.props,
                             ...l
                         }).getViewportProps(), this.onViewStateChange({
                             viewState: this.propsInTransition,
                             oldViewState: this.props
                         })
-                    })), this.getControllerState = t.getControllerState, this.propsInTransition = null, this.transition = new Rf(t.timeline), this.onViewStateChange = t.onViewStateChange || jf, this.onStateChange = t.onStateChange || jf
+                    })), this.getControllerState = t.getControllerState, this.propsInTransition = null, this.transition = new If(t.timeline), this.onViewStateChange = t.onViewStateChange || jf, this.onStateChange = t.onStateChange || jf
                 }
                 finalize() {
                     this.transition.cancel()
                 }
                 getViewportInTransition() {
                     return this.propsInTransition
                 }
@@ -14518,15 +14519,15 @@
                         r = e.transitionInterpolator,
                         s = r.getDuration ? r.getDuration(t, e) : e.transitionDuration;
                     if (0 === s) return;
                     const o = r.initializeProps(t, i);
                     this.propsInTransition = {};
                     const a = {
                         duration: s,
-                        easing: e.transitionEasing || zf,
+                        easing: e.transitionEasing || Ff,
                         interpolator: r,
                         interruption: e.transitionInterruption || 1,
                         startProps: o.start,
                         endProps: o.end,
                         onStart: e.onTransitionStart,
                         onUpdate: this._onTransitionUpdate,
                         onInterrupt: this._onTransitionEnd(e.onTransitionInterrupt),
@@ -14634,19 +14635,19 @@
                 Wf = ["wheel"],
                 Hf = ["panstart", "panmove", "panend"],
                 Zf = ["pinchstart", "pinchmove", "pinchend"],
                 qf = ["tripanstart", "tripanmove", "tripanend"],
                 Xf = ["doubletap"],
                 Yf = ["keydown"],
                 Kf = {};
-            class $f {
+            class Jf {
                 constructor(t) {
                     wo(this, "props", void 0), wo(this, "state", {}), wo(this, "transitionManager", void 0), wo(this, "eventManager", void 0), wo(this, "onViewStateChange", void 0), wo(this, "onStateChange", void 0), wo(this, "makeViewport", void 0), wo(this, "_controllerState", void 0), wo(this, "_events", {}), wo(this, "_interactionState", {
                         isDragging: !1
-                    }), wo(this, "_customEvents", []), wo(this, "_eventStartBlocked", null), wo(this, "_panMove", !1), wo(this, "invertPan", !1), wo(this, "dragMode", "rotate"), wo(this, "inertia", 0), wo(this, "scrollZoom", !0), wo(this, "dragPan", !0), wo(this, "dragRotate", !0), wo(this, "doubleClickZoom", !0), wo(this, "touchZoom", !0), wo(this, "touchRotate", !1), wo(this, "keyboard", !0), this.transitionManager = new Ff({
+                    }), wo(this, "_customEvents", []), wo(this, "_eventStartBlocked", null), wo(this, "_panMove", !1), wo(this, "invertPan", !1), wo(this, "dragMode", "rotate"), wo(this, "inertia", 0), wo(this, "scrollZoom", !0), wo(this, "dragPan", !0), wo(this, "dragRotate", !0), wo(this, "doubleClickZoom", !0), wo(this, "touchZoom", !0), wo(this, "touchRotate", !1), wo(this, "keyboard", !0), this.transitionManager = new zf({
                         ...t,
                         getControllerState: t => new this.ControllerState(t),
                         onViewStateChange: this._onTransition.bind(this),
                         onStateChange: this._setInteractionState.bind(this)
                     }), this.handleEvent = this.handleEvent.bind(this), this.eventManager = t.eventManager, this.onViewStateChange = t.onViewStateChange || (() => {}), this.onStateChange = t.onStateChange || (() => {}), this.makeViewport = t.makeViewport
                 }
                 set events(t) {
@@ -15095,26 +15096,26 @@
                             ...t,
                             ...e.transitionInterpolator.opts,
                             makeViewport: this.controllerState.makeViewport
                         })
                     } : e : Uf
                 }
             }
-            class Jf {
+            class Qf {
                 constructor(t, e) {
                     wo(this, "_viewportProps", void 0), wo(this, "_state", void 0), this._viewportProps = this.applyConstraints(t), this._state = e
                 }
                 getViewportProps() {
                     return this._viewportProps
                 }
                 getState() {
                     return this._state
                 }
             }
-            class Qf extends Jf {
+            class $f extends Qf {
                 constructor(t) {
                     const {
                         width: e,
                         height: n,
                         latitude: i,
                         longitude: r,
                         zoom: s,
@@ -15401,17 +15402,17 @@
                     let f = n;
                     return u > 0 ? f = n + u * (p - n) : u < 0 && (f = n - u * (d - n)), {
                         pitch: f,
                         bearing: i + 180 * h
                     }
                 }
             }
-            class tg extends $f {
+            class tg extends Jf {
                 constructor(...t) {
-                    super(...t), wo(this, "ControllerState", Qf), wo(this, "transition", {
+                    super(...t), wo(this, "ControllerState", $f), wo(this, "transition", {
                         transitionDuration: 300,
                         transitionInterpolator: new Vf({
                             transitionProps: {
                                 compare: ["longitude", "latitude", "zoom", "bearing", "pitch", "position"],
                                 required: ["longitude", "latitude", "zoom"]
                             }
                         })
@@ -15423,17 +15424,17 @@
                     super.setProps(t), (!e || e.height !== t.height) && this.updateViewport(new this.ControllerState({
                         makeViewport: this.makeViewport,
                         ...t,
                         ...this.state
                     }))
                 }
             }
-            class eg extends Of {
+            class eg extends Lf {
                 get ViewportType() {
-                    return If
+                    return Rf
                 }
                 get ControllerType() {
                     return tg
                 }
             }
             wo(eg, "displayName", "MapView");
             const ng = [255, 255, 255],
@@ -15462,15 +15463,15 @@
                     } = t, {
                         intensity: n = ag
                     } = t, {
                         direction: i = lg
                     } = t, {
                         _shadow: r = !1
                     } = t;
-                    this.id = t.id || "directional-".concat(cg++), this.color = e, this.intensity = n, this.type = "directional", this.direction = new Oc(i).normalize().toArray(), this.shadow = r
+                    this.id = t.id || "directional-".concat(cg++), this.color = e, this.intensity = n, this.type = "directional", this.direction = new Lc(i).normalize().toArray(), this.shadow = r
                 }
                 getProjectedLight(t) {
                     return this
                 }
             }
             class ug {
                 constructor(t, e = {
@@ -15695,15 +15696,15 @@
                         height: 1,
                         parameters: {
                             10241: 9729,
                             10240: 9729,
                             10242: 33071,
                             10243: 33071
                         }
-                    }), this.depthBuffer = new Qd(t, {
+                    }), this.depthBuffer = new $d(t, {
                         format: 33189,
                         width: 1,
                         height: 1
                     }), this.fbo = new vp(t, {
                         id: "shadowmap",
                         width: 1,
                         height: 1,
@@ -15747,15 +15748,15 @@
                     this.fbo && (this.fbo.delete(), this.fbo = null), this.shadowMap && (this.shadowMap.delete(), this.shadowMap = null), this.depthBuffer && (this.depthBuffer.delete(), this.depthBuffer = null)
                 }
             }
             const gg = hf((function({
                     viewport: t,
                     center: e
                 }) {
-                    return new Qc(t.viewProjectionMatrix).invert().transform(e)
+                    return new $c(t.viewProjectionMatrix).invert().transform(e)
                 })),
                 mg = hf((function({
                     viewport: t,
                     shadowMatrices: e
                 }) {
                     const n = [],
                         i = t.pixelUnprojectionMatrix,
@@ -15770,17 +15771,17 @@
                             [0, t.height, -1],
                             [t.width, t.height, -1]
                         ].map((t => function(t, e) {
                             const [n, i, r] = t, s = Eh([n, i, r], e);
                             return Number.isFinite(r) ? s : [s[0], s[1], 0]
                         }(t, i)));
                     for (const i of e) {
-                        const e = i.clone().translate(new Oc(t.center).negate()),
+                        const e = i.clone().translate(new Lc(t.center).negate()),
                             r = s.map((t => e.transform(t))),
-                            o = (new Qc).ortho({
+                            o = (new $c).ortho({
                                 left: Math.min(...r.map((t => t[0]))),
                                 right: Math.max(...r.map((t => t[0]))),
                                 bottom: Math.min(...r.map((t => t[1]))),
                                 top: Math.max(...r.map((t => t[1]))),
                                 near: Math.min(...r.map((t => -t[2]))),
                                 far: Math.max(...r.map((t => -t[2])))
                             });
@@ -15821,15 +15822,15 @@
                             s = [],
                             o = mg({
                                 shadowMatrices: t.shadowMatrices,
                                 viewport: t.viewport
                             }).slice();
                         for (let n = 0; n < t.shadowMatrices.length; n++) {
                             const i = o[n],
-                                a = i.clone().translate(new Oc(t.viewport.center).negate());
+                                a = i.clone().translate(new Lc(t.viewport.center).negate());
                             e.project_uCoordinateSystem === Th.LNGLAT && e.project_uProjectionMode === Ah.WEB_MERCATOR ? (o[n] = a, s[n] = r) : (o[n] = i.clone().multiplyRight(bg), s[n] = a.transform(r))
                         }
                         for (let e = 0; e < o.length; e++) i["shadow_uViewProjectionMatrices[".concat(e, "]")] = o[e], i["shadow_uProjectCenters[".concat(e, "]")] = s[e], t.shadowMaps && t.shadowMaps.length > 0 ? i["shadow_uShadowMap".concat(e)] = t.shadowMaps[e] : i["shadow_uShadowMap".concat(e)] = t.dummyShadowMap;
                         return i
                     }(t, e) : {}
                 },
                 _g = {
@@ -15910,16 +15911,16 @@
                 cleanup() {
                     for (const t of this.shadowPasses) t.delete();
                     this.shadowPasses.length = 0, this.shadowMaps.length = 0, this.dummyShadowMap && (this.dummyShadowMap.delete(), this.dummyShadowMap = null), this.shadow && this.programManager && (this.programManager.removeDefaultModule(yg), this.programManager = null)
                 }
                 _calculateMatrices() {
                     const t = [];
                     for (const e of this.directionalLights) {
-                        const n = (new Qc).lookAt({
-                            eye: new Oc(e.direction).negate()
+                        const n = (new $c).lookAt({
+                            eye: new Lc(e.direction).negate()
                         });
                         t.push(n)
                     }
                     return t
                 }
                 _createShadowPasses(t) {
                     for (let e = 0; e < this.directionalLights.length; e++) {
@@ -15979,15 +15980,15 @@
                 shouldDrawLayer(t) {
                     return t.props.operation === kh
                 }
                 delete() {
                     this.fbo.delete(), this.maskMap.delete()
                 }
             }
-            const Sg = (new Qc).lookAt({
+            const Sg = (new $c).lookAt({
                 eye: [0, 0, 1]
             });
 
             function Cg({
                 width: t,
                 height: e,
                 near: n,
@@ -16003,24 +16004,24 @@
                         left: n = 0,
                         right: i = 0,
                         top: c = 0,
                         bottom: h = 0
                     } = r, u = oc((n + t - i) / 2, 0, t) - t / 2, d = oc((c + e - h) / 2, 0, e) - e / 2;
                     s -= u, o -= u, a += d, l += d
                 }
-                return (new Qc).ortho({
+                return (new $c).ortho({
                     left: s,
                     right: o,
                     bottom: a,
                     top: l,
                     near: n,
                     far: i
                 })
             }
-            class Tg extends Fh {
+            class Tg extends zh {
                 constructor(t) {
                     const {
                         width: e,
                         height: n,
                         near: i = .1,
                         far: r = 1e3,
                         zoom: s = 0,
@@ -16070,15 +16071,15 @@
                         i = Gc([], this.projectFlat(t), Wc([], n)),
                         r = Gc([], this.center, i);
                     return {
                         target: this.unprojectFlat(r)
                     }
                 }
             }
-            class Ag extends Jf {
+            class Ag extends Qf {
                 constructor(t) {
                     const {
                         width: e,
                         height: n,
                         rotationX: i = 0,
                         rotationOrbit: r = 0,
                         target: s = [0, 0, 0],
@@ -16346,34 +16347,34 @@
                                 e < i && (r += i - e), e = Math.max(t + r, s + r), e > n && (r += n - e), t += r, s += r
                         }
                         return [t, s]
                     }
                     return oc(e + r, i, n)
                 }
             }
-            class Og extends $f {
+            class Lg extends Jf {
                 constructor(...t) {
                     super(...t), wo(this, "ControllerState", Mg), wo(this, "transition", {
                         transitionDuration: 300,
                         transitionInterpolator: new Vf(["target", "zoom"])
                     }), wo(this, "dragMode", "pan")
                 }
                 _onPanRotate() {
                     return !1
                 }
             }
-            class Lg extends Of {
+            class Og extends Lf {
                 get ViewportType() {
                     return Tg
                 }
                 get ControllerType() {
-                    return Og
+                    return Lg
                 }
             }
-            wo(Lg, "displayName", "OrthographicView");
+            wo(Og, "displayName", "OrthographicView");
             class kg {
                 constructor() {
                     wo(this, "id", "mask-effect"), wo(this, "props", null), wo(this, "useInPicking", !0), wo(this, "dummyMaskMap", void 0), wo(this, "channels", []), wo(this, "masks", null), wo(this, "maskPass", void 0), wo(this, "maskMap", void 0), wo(this, "lastViewport", void 0)
                 }
                 preRender(t, {
                     layers: e,
                     layerFilter: n,
@@ -16440,41 +16441,41 @@
                         } = this, a = function({
                             bounds: t,
                             viewport: e,
                             width: n,
                             height: i
                         }) {
                             if (t[2] <= t[0] || t[3] <= t[1]) return null;
-                            if (n -= 2, i -= 2, e instanceof If) {
+                            if (n -= 2, i -= 2, e instanceof Rf) {
                                 const {
                                     longitude: e,
                                     latitude: r,
                                     zoom: s
                                 } = Ph({
                                     width: n,
                                     height: i,
                                     bounds: [
                                         [t[0], t[1]],
                                         [t[2], t[3]]
                                     ],
                                     maxZoom: 20
                                 });
-                                return new If({
+                                return new Rf({
                                     longitude: e,
                                     latitude: r,
                                     zoom: s,
                                     x: 1,
                                     y: 1,
                                     width: n,
                                     height: i
                                 })
                             }
                             const r = [(t[0] + t[2]) / 2, (t[1] + t[3]) / 2, 0],
                                 s = Math.min(20, n / (t[2] - t[0]), i / (t[3] - t[1]));
-                            return new Lg({
+                            return new Og({
                                 x: 1,
                                 y: 1
                             }).makeViewport({
                                 width: n,
                                 height: i,
                                 viewState: {
                                     target: r,
@@ -16547,16 +16548,16 @@
                         maskChannels: this.masks
                     }
                 }
                 cleanup() {
                     this.dummyMaskMap && (this.dummyMaskMap.delete(), this.dummyMaskMap = void 0), this.maskPass && (this.maskPass.delete(), this.maskPass = void 0, this.maskMap = void 0), this.lastViewport = void 0, this.masks = null, this.channels.length = 0
                 }
             }
-            const Ig = new Eg;
-            class Rg {
+            const Rg = new Eg;
+            class Ig {
                 constructor() {
                     wo(this, "effects", void 0), wo(this, "_internalEffects", void 0), wo(this, "_needsRedraw", void 0), this.effects = [], this._internalEffects = [], this._needsRedraw = "Initial render", this.setEffects()
                 }
                 setProps(t) {
                     "effects" in t && (t.effects.length === this.effects.length && Pf(t.effects, this.effects) || (this.setEffects(t.effects), this._needsRedraw = "effects changed"))
                 }
                 needsRedraw(t = {
@@ -16568,32 +16569,32 @@
                 getEffects() {
                     return this._internalEffects
                 }
                 finalize() {
                     this.cleanup()
                 }
                 setEffects(t = []) {
-                    this.cleanup(), this.effects = t, this._internalEffects = t.slice(), this._internalEffects.push(new kg), t.some((t => t instanceof Eg)) || this._internalEffects.push(Ig)
+                    this.cleanup(), this.effects = t, this._internalEffects = t.slice(), this._internalEffects.push(new kg), t.some((t => t instanceof Eg)) || this._internalEffects.push(Rg)
                 }
                 cleanup() {
                     for (const t of this.effects) t.cleanup();
                     for (const t of this._internalEffects) t.cleanup();
                     this.effects.length = 0, this._internalEffects.length = 0
                 }
             }
             class jg extends dg {
                 shouldDrawLayer(t) {
-                    return t.props.operation === Lh
+                    return t.props.operation === Oh
                 }
             }
-            const zg = {
+            const Fg = {
                 blendFunc: [1, 0, 32771, 0],
                 blendEquation: 32774
             };
-            class Fg extends dg {
+            class zg extends dg {
                 constructor(...t) {
                     super(...t), wo(this, "pickZ", void 0), wo(this, "_colors", null)
                 }
                 render(t) {
                     return t.pickingFBO ? this._drawPickingBuffer(t) : super.render(t)
                 }
                 _drawPickingBuffer({
@@ -16625,15 +16626,15 @@
                         scissorTest: !0,
                         scissor: [o, a, l, c],
                         clearColor: [0, 0, 0, 0],
                         depthMask: !0,
                         depthTest: !0,
                         depthRange: [0, 1],
                         colorMask: [!0, !0, !0, !0],
-                        ...zg,
+                        ...Fg,
                         blend: !p
                     }, (() => super.render({
                         target: s,
                         layers: t,
                         layerFilter: e,
                         views: n,
                         viewports: i,
@@ -16644,28 +16645,28 @@
                     })));
                     return this._colors = null, {
                         decodePickingColor: g && Bg.bind(null, g),
                         stats: m
                     }
                 }
                 shouldDrawLayer(t) {
-                    return t.props.pickable && t.props.operation === Lh
+                    return t.props.pickable && t.props.operation === Oh
                 }
                 getModuleParameters() {
                     return {
                         pickingActive: 1,
                         pickingAttribute: this.pickZ,
                         lightSources: {}
                     }
                 }
                 getLayerParameters(t, e, n) {
                     const i = {
                         ...t.props.parameters
                     };
-                    return this._colors ? (Object.assign(i, zg), i.blend = !0, i.blendColor = function(t, e, n) {
+                    return this._colors ? (Object.assign(i, Fg), i.blend = !0, i.blendColor = function(t, e, n) {
                         const {
                             byLayer: i,
                             byAlpha: r
                         } = t;
                         let s, o = i.get(e);
                         return o ? (o.viewports.push(n), s = o.a) : (s = i.size + 1, s <= 255 ? (o = {
                             a: s,
@@ -16682,15 +16683,15 @@
                     pickedLayer: n.layer,
                     pickedViewports: n.viewports,
                     pickedObjectIndex: n.layer.decodePickingColor(e)
                 }
             }
             class Dg {
                 constructor(t) {
-                    this.gl = t, this.layerFilter = null, this.drawPickingColors = !1, this.drawLayersPass = new jg(t), this.pickLayersPass = new Fg(t), this.renderCount = 0, this._needsRedraw = "Initial render", this.renderBuffers = [], this.lastPostProcessEffect = null
+                    this.gl = t, this.layerFilter = null, this.drawPickingColors = !1, this.drawLayersPass = new jg(t), this.pickLayersPass = new zg(t), this.renderCount = 0, this._needsRedraw = "Initial render", this.renderBuffers = [], this.lastPostProcessEffect = null
                 }
                 setProps(t) {
                     "layerFilter" in t && this.layerFilter !== t.layerFilter && (this.layerFilter = t.layerFilter, this._needsRedraw = "layerFilter changed"), "drawPickingColors" in t && this.drawPickingColors !== t.drawPickingColors && (this.drawPickingColors = t.drawPickingColors, this._needsRedraw = "drawPickingColors changed")
                 }
                 renderLayers(t) {
                     const e = this.drawPickingColors ? this.pickLayersPass : this.drawLayersPass;
                     t.layerFilter = t.layerFilter || this.layerFilter, t.effects = t.effects || [], t.target = t.target || vp.getDefaultFramebuffer(this.gl), this._preRender(t.effects, t);
@@ -16888,15 +16889,15 @@
                         sourceLayer: i
                     }), t = t.parent
                 }
                 return e
             }
             class Hg {
                 constructor(t) {
-                    wo(this, "gl", void 0), wo(this, "pickingFBO", void 0), wo(this, "depthFBO", void 0), wo(this, "pickLayersPass", void 0), wo(this, "layerFilter", void 0), wo(this, "lastPickedInfo", void 0), wo(this, "_pickable", !0), this.gl = t, this.pickLayersPass = new Fg(t), this.lastPickedInfo = {
+                    wo(this, "gl", void 0), wo(this, "pickingFBO", void 0), wo(this, "depthFBO", void 0), wo(this, "pickLayersPass", void 0), wo(this, "layerFilter", void 0), wo(this, "lastPickedInfo", void 0), wo(this, "_pickable", !0), this.gl = t, this.pickLayersPass = new zg(t), this.lastPickedInfo = {
                         index: -1,
                         layerId: null,
                         info: null
                     }
                 }
                 setProps(t) {
                     "layerFilter" in t && (this.layerFilter = t.layerFilter), "_pickable" in t && (this._pickable = t._pickable)
@@ -17240,17 +17241,17 @@
                 }
                 remove() {
                     this.el && (this.el.remove(), this.el = null)
                 }
             }
             const {
                 _parseImageNode: Xg
-            } = globalThis, Yg = "undefined" != typeof Image, Kg = "undefined" != typeof ImageBitmap, $g = Boolean(Xg), Jg = !!il || $g;
+            } = globalThis, Yg = "undefined" != typeof Image, Kg = "undefined" != typeof ImageBitmap, Jg = Boolean(Xg), Qg = !!il || Jg;
 
-            function Qg(t) {
+            function $g(t) {
                 const e = function(t) {
                     return "undefined" != typeof ImageBitmap && t instanceof ImageBitmap ? "imagebitmap" : "undefined" != typeof Image && t instanceof Image ? "image" : t && "object" == typeof t && t.data && t.width && t.height ? "data" : null
                 }(t);
                 if (!e) throw new Error("Not an image");
                 return e
             }
             const tm = /^data:image\/svg\+xml/,
@@ -17400,28 +17401,28 @@
                         switch (function(t) {
                                 switch (t) {
                                     case "auto":
                                     case "data":
                                         return function() {
                                             if (Kg) return "imagebitmap";
                                             if (Yg) return "image";
-                                            if (Jg) return "data";
+                                            if (Qg) return "data";
                                             throw new Error("Install '@loaders.gl/polyfills' to parse images under Node.js")
                                         }();
                                     default:
                                         return function(t) {
                                             switch (t) {
                                                 case "auto":
-                                                    return Kg || Yg || Jg;
+                                                    return Kg || Yg || Qg;
                                                 case "imagebitmap":
                                                     return Kg;
                                                 case "image":
                                                     return Yg;
                                                 case "data":
-                                                    return Jg;
+                                                    return Qg;
                                                 default:
                                                     throw new Error("@loaders.gl/images: image ".concat(t, " not supported in this environment"))
                                             }
                                         }(t), t
                                 }
                             }(i)) {
                             case "imagebitmap":
@@ -17454,15 +17455,15 @@
                                     return ya(i), await i(t, n)
                                 }(t);
                                 break;
                             default:
                                 ya(!1)
                         }
                         return "data" === i && (s = function(t) {
-                            switch (Qg(t)) {
+                            switch ($g(t)) {
                                 case "data":
                                     return t;
                                 case "image":
                                 case "imagebitmap":
                                     const e = document.createElement("canvas"),
                                         n = e.getContext("2d");
                                     if (!n) throw new Error("getImageData");
@@ -17518,24 +17519,24 @@
                     premultiplyAlpha: "none"
                 }
             }]]));
             const gm = globalThis.deck,
                 mm = globalThis;
 
             function vm(t) {
-                if (!t && !Io()) return "Node";
-                if (Lo(t)) return "Electron";
+                if (!t && !Ro()) return "Node";
+                if (Oo(t)) return "Electron";
                 const e = "undefined" != typeof navigator ? navigator : {},
                     n = t || e.userAgent || "";
                 if (n.indexOf("Edge") > -1) return "Edge";
                 const i = -1 !== n.indexOf("MSIE "),
                     r = -1 !== n.indexOf("Trident/");
                 return i || r ? "IE" : mm.chrome ? "Chrome" : mm.safari ? "Safari" : mm.mozInnerScreenX ? "Firefox" : "Unknown"
             }
-            class bm extends Ld {
+            class bm extends Od {
                 get[Symbol.toStringTag]() {
                     return "Query"
                 }
                 static isSupported(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : [];
                     const n = Mu(t),
                         i = fp(t, hp);
@@ -17601,15 +17602,15 @@
                 _createHandle() {
                     return bm.isSupported(this.gl) ? this.gl2.createQuery() : null
                 }
                 _deleteHandle() {
                     this.gl2.deleteQuery(this.handle)
                 }
             }
-            const ym = Io() && "undefined" != typeof document;
+            const ym = Ro() && "undefined" != typeof document;
             let _m = 0;
             class xm {
                 constructor() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     const {
                         onCreateContext: e = (t => vd(t)),
                         onAddHTML: n = null,
@@ -17937,26 +17938,26 @@
                     pan: ["press", "doubletap", "anytap", "tap"],
                     doubletap: ["anytap"],
                     anytap: ["tap"]
                 },
                 Mm = {
                     doubletap: ["tap"]
                 },
-                Om = {
+                Lm = {
                     pointerdown: "pointerdown",
                     pointermove: "pointermove",
                     pointerup: "pointerup",
                     touchstart: "pointerdown",
                     touchmove: "pointermove",
                     touchend: "pointerup",
                     mousedown: "pointerdown",
                     mousemove: "pointermove",
                     mouseup: "pointerup"
                 },
-                Lm = {
+                Om = {
                     KEY_EVENTS: ["keydown", "keyup"],
                     MOUSE_EVENTS: ["mousedown", "mousemove", "mouseup", "mouseover", "mouseout", "mouseleave"],
                     WHEEL_EVENTS: ["wheel", "mousewheel"]
                 },
                 km = {
                     tap: "tap",
                     anytap: "anytap",
@@ -17994,75 +17995,75 @@
                     pancancel: "pan",
                     swipe: "swipe",
                     swipeleft: "swipe",
                     swiperight: "swipe",
                     swipeup: "swipe",
                     swipedown: "swipe"
                 },
-                Im = {
+                Rm = {
                     click: "tap",
                     anyclick: "anytap",
                     dblclick: "doubletap",
                     mousedown: "pointerdown",
                     mousemove: "pointermove",
                     mouseup: "pointerup",
                     mouseover: "pointerover",
                     mouseout: "pointerout",
                     mouseleave: "pointerleave"
                 },
-                Rm = "undefined" != typeof navigator && navigator.userAgent ? navigator.userAgent.toLowerCase() : "",
+                Im = "undefined" != typeof navigator && navigator.userAgent ? navigator.userAgent.toLowerCase() : "",
                 jm = "undefined" != typeof window ? window : n.g;
             void 0 !== n.g ? n.g : window, "undefined" != typeof document && document;
-            let zm = !1;
+            let Fm = !1;
             try {
                 const t = {
                     get passive() {
-                        return zm = !0, !0
+                        return Fm = !0, !0
                     }
                 };
                 jm.addEventListener("test", null, t), jm.removeEventListener("test", null)
             } catch (t) {
-                zm = !1
+                Fm = !1
             }
-            const Fm = -1 !== Rm.indexOf("firefox"),
+            const zm = -1 !== Im.indexOf("firefox"),
                 {
                     WHEEL_EVENTS: Bm
-                } = Lm,
+                } = Om,
                 Dm = "wheel",
                 Nm = 4.000244140625;
             class Vm extends Cm {
                 constructor(t, e, n) {
                     super(t, e, n), this.handleEvent = t => {
                         if (!this.options.enable) return;
                         let e = t.deltaY;
-                        jm.WheelEvent && (Fm && t.deltaMode === jm.WheelEvent.DOM_DELTA_PIXEL && (e /= jm.devicePixelRatio), t.deltaMode === jm.WheelEvent.DOM_DELTA_LINE && (e *= 40)), 0 !== e && e % Nm == 0 && (e = Math.floor(e / Nm)), t.shiftKey && e && (e *= .25), this.callback({
+                        jm.WheelEvent && (zm && t.deltaMode === jm.WheelEvent.DOM_DELTA_PIXEL && (e /= jm.devicePixelRatio), t.deltaMode === jm.WheelEvent.DOM_DELTA_LINE && (e *= 40)), 0 !== e && e % Nm == 0 && (e = Math.floor(e / Nm)), t.shiftKey && e && (e *= .25), this.callback({
                             type: Dm,
                             center: {
                                 x: t.clientX,
                                 y: t.clientY
                             },
                             delta: -e,
                             srcEvent: t,
                             pointerType: "mouse",
                             target: t.target
                         })
-                    }, this.events = (this.options.events || []).concat(Bm), this.events.forEach((e => t.addEventListener(e, this.handleEvent, !!zm && {
+                    }, this.events = (this.options.events || []).concat(Bm), this.events.forEach((e => t.addEventListener(e, this.handleEvent, !!Fm && {
                         passive: !1
                     })))
                 }
                 destroy() {
                     this.events.forEach((t => this.element.removeEventListener(t, this.handleEvent)))
                 }
                 enableEventType(t, e) {
                     t === Dm && (this.options.enable = e)
                 }
             }
             const {
                 MOUSE_EVENTS: Um
-            } = Lm, Gm = "pointermove", Wm = "pointerover", Hm = "pointerout", Zm = "pointerenter", qm = "pointerleave";
+            } = Om, Gm = "pointermove", Wm = "pointerover", Hm = "pointerout", Zm = "pointerenter", qm = "pointerleave";
             class Xm extends Cm {
                 constructor(t, e, n) {
                     super(t, e, n), this.handleEvent = t => {
                         this.handleOverEvent(t), this.handleOutEvent(t), this.handleEnterEvent(t), this.handleLeaveEvent(t), this.handleMoveEvent(t)
                     }, this.pressed = !1;
                     const {
                         enable: i
@@ -18110,60 +18111,60 @@
                         pointerType: "mouse",
                         target: e.target
                     })
                 }
             }
             const {
                 KEY_EVENTS: Ym
-            } = Lm, Km = "keydown", $m = "keyup";
-            class Jm extends Cm {
+            } = Om, Km = "keydown", Jm = "keyup";
+            class Qm extends Cm {
                 constructor(t, e, n) {
                     super(t, e, n), this.handleEvent = t => {
                         const e = t.target || t.srcElement;
                         "INPUT" === e.tagName && "text" === e.type || "TEXTAREA" === e.tagName || (this.enableDownEvent && "keydown" === t.type && this.callback({
                             type: Km,
                             srcEvent: t,
                             key: t.key,
                             target: t.target
                         }), this.enableUpEvent && "keyup" === t.type && this.callback({
-                            type: $m,
+                            type: Jm,
                             srcEvent: t,
                             key: t.key,
                             target: t.target
                         }))
                     }, this.enableDownEvent = this.options.enable, this.enableUpEvent = this.options.enable, this.events = (this.options.events || []).concat(Ym), t.tabIndex = this.options.tabIndex || 0, t.style.outline = "none", this.events.forEach((e => t.addEventListener(e, this.handleEvent)))
                 }
                 destroy() {
                     this.events.forEach((t => this.element.removeEventListener(t, this.handleEvent)))
                 }
                 enableEventType(t, e) {
-                    t === Km && (this.enableDownEvent = e), t === $m && (this.enableUpEvent = e)
+                    t === Km && (this.enableDownEvent = e), t === Jm && (this.enableUpEvent = e)
                 }
             }
-            const Qm = "contextmenu";
+            const $m = "contextmenu";
             class tv extends Cm {
                 constructor(t, e, n) {
                     super(t, e, n), this.handleEvent = t => {
                         this.options.enable && this.callback({
-                            type: Qm,
+                            type: $m,
                             center: {
                                 x: t.clientX,
                                 y: t.clientY
                             },
                             srcEvent: t,
                             pointerType: "mouse",
                             target: t.target
                         })
                     }, t.addEventListener("contextmenu", this.handleEvent)
                 }
                 destroy() {
                     this.element.removeEventListener("contextmenu", this.handleEvent)
                 }
                 enableEventType(t, e) {
-                    t === Qm && (this.options.enable = e)
+                    t === $m && (this.options.enable = e)
                 }
             }
             const ev = {
                 pointerdown: 1,
                 pointermove: 2,
                 pointerup: 4,
                 mousedown: 1,
@@ -18322,15 +18323,15 @@
                 tabIndex: 0
             };
             class av {
                 constructor(t = null, e) {
                     this._onBasicInput = t => {
                         const {
                             srcEvent: e
-                        } = t, n = Om[e.type];
+                        } = t, n = Lm[e.type];
                         n && this.manager.emit(n, t)
                     }, this._onOtherEvent = t => {
                         this.manager.emit(t.type, t)
                     }, this.options = {
                         ...ov,
                         ...e
                     }, this.events = new Map, this.setElement(t);
@@ -18363,15 +18364,15 @@
                             delete i.enable, n.set(i)
                         }
                     }
                     this.wheelInput = new Vm(t, this._onOtherEvent, {
                         enable: !1
                     }), this.moveInput = new Xm(t, this._onOtherEvent, {
                         enable: !1
-                    }), this.keyInput = new Jm(t, this._onOtherEvent, {
+                    }), this.keyInput = new Qm(t, this._onOtherEvent, {
                         enable: !1,
                         tabIndex: e.tabIndex
                     }), this.contextmenuInput = new tv(t, this._onOtherEvent, {
                         enable: !1
                     });
                     for (const [t, e] of this.events) e.isEmpty() || (this._toggleRecognizer(e.recognizerName, !0), this.manager.on(t, e.handleEvent))
                 }
@@ -18413,26 +18414,26 @@
                         n = e;
                         for (const e in t) this._addEventHandler(e, t[e], n, i, r);
                         return
                     }
                     const {
                         manager: s,
                         events: o
-                    } = this, a = Im[t] || t;
+                    } = this, a = Rm[t] || t;
                     let l = o.get(a);
                     l || (l = new sv(this), o.set(a, l), l.recognizerName = km[a] || a, s && s.on(a, l.handleEvent)), l.add(t, e, n, i, r), l.isEmpty() || this._toggleRecognizer(l.recognizerName, !0)
                 }
                 _removeEventHandler(t, e) {
                     if ("string" != typeof t) {
                         for (const e in t) this._removeEventHandler(e, t[e]);
                         return
                     }
                     const {
                         events: n
-                    } = this, i = Im[t] || t, r = n.get(i);
+                    } = this, i = Rm[t] || t, r = n.get(i);
                     if (r && (r.remove(t, e), r.isEmpty())) {
                         const {
                             recognizerName: t
                         } = r;
                         let e = !1;
                         for (const i of n.values())
                             if (i.recognizerName === t && !i.isEmpty()) {
@@ -18506,15 +18507,15 @@
                             }
                         }
                         this.layerManager && (this.layerManager.context.mousePosition = {
                             x: e.x,
                             y: e.y
                         }), e.event = t
                     })), wo(this, "_onEvent", (t => {
-                        const e = Oh[t.type],
+                        const e = Lh[t.type],
                             n = t.offsetCenter;
                         if (!e || !n || !this.layerManager) return;
                         const i = this.layerManager.getLayers(),
                             r = this.deckPicker.getLastPickedObject({
                                 x: n.x,
                                 y: n.y,
                                 layers: i,
@@ -18773,15 +18774,15 @@
                         recognizerOptions: this.props.eventRecognizerOptions,
                         events: {
                             pointerdown: this._onPointerDown,
                             pointermove: this._onPointerMove,
                             pointerleave: this._onPointerMove
                         }
                     });
-                    for (const t in Oh) this.eventManager.on(t, this._onEvent);
+                    for (const t in Lh) this.eventManager.on(t, this._onEvent);
                     this.viewManager = new Sf({
                         timeline: e,
                         eventManager: this.eventManager,
                         onViewStateChange: this._onViewStateChange.bind(this),
                         onInteractionStateChange: this._onInteractionStateChange.bind(this),
                         views: this._getViews(),
                         viewState: this._getViewState(),
@@ -18790,15 +18791,15 @@
                     });
                     const n = this.viewManager.getViewports()[0];
                     this.layerManager = new Ef(t, {
                         deck: this,
                         stats: this.stats,
                         viewport: n,
                         timeline: e
-                    }), this.effectManager = new Rg, this.deckRenderer = new Dg(t), this.deckPicker = new Hg(t), this.setProps(this.props), this._updateCanvasSize(), this.props.onLoad()
+                    }), this.effectManager = new Ig, this.deckRenderer = new Dg(t), this.deckPicker = new Hg(t), this.setProps(this.props), this._updateCanvasSize(), this.props.onLoad()
                 }
                 _drawLayers(t, e) {
                     const {
                         gl: n
                     } = this.layerManager.context;
                     ld(n, this.props.parameters), this.props.onBeforeRender({
                         gl: n
@@ -19078,15 +19079,15 @@
                         this._checkExternalBuffer(n);
                         let t = n.value;
                         e.externalBuffer = null, e.constant = !1, this.value = t, i.bytesPerElement = t.BYTES_PER_ELEMENT, i.stride = fv(i);
                         const {
                             buffer: r,
                             byteOffset: s
                         } = this;
-                        this.doublePrecision && t instanceof Float64Array && (t = Rc(t, i));
+                        this.doublePrecision && t instanceof Float64Array && (t = Ic(t, i));
                         const o = t.byteLength + s + 2 * i.stride;
                         r.byteLength < o && r.reallocate(o), r.setAccessor(null), r.subData({
                             data: t,
                             offset: s
                         }), i.type = n.type || r.accessor.type
                     }
                     return !0
@@ -19095,15 +19096,15 @@
                     this.state.bounds = null;
                     const e = this.value,
                         {
                             startOffset: n = 0,
                             endOffset: i
                         } = t;
                     this.buffer.subData({
-                        data: this.doublePrecision && e instanceof Float64Array ? Rc(e, {
+                        data: this.doublePrecision && e instanceof Float64Array ? Ic(e, {
                             size: this.size,
                             startIndex: n,
                             endIndex: i
                         }) : e.subarray(n, i),
                         offset: n * e.BYTES_PER_ELEMENT + this.byteOffset
                     })
                 }
@@ -19117,15 +19118,15 @@
                     });
                     this.value = r;
                     const {
                         buffer: s,
                         byteOffset: o
                     } = this;
                     return s.byteLength < r.byteLength + o && (s.reallocate(r.byteLength + o), e && i && s.subData({
-                        data: i instanceof Float64Array ? Rc(i, this) : i,
+                        data: i instanceof Float64Array ? Ic(i, this) : i,
                         offset: o
                     })), n.allocatedValue = r, n.constant = !1, n.externalBuffer = null, n.bufferAccessor = this.settings, !0
                 }
                 _checkExternalBuffer(t) {
                     const {
                         value: e
                     } = t;
@@ -19313,38 +19314,38 @@
                 }
             }
 
             function Mv(t) {
                 t.push(t.shift())
             }
 
-            function Ov(t, e) {
+            function Lv(t, e) {
                 const {
                     doublePrecision: n,
                     settings: i,
                     value: r,
                     size: s
                 } = t, o = n && r instanceof Float64Array ? 2 : 1;
                 return (i.noAlloc ? r.length : e * s) * o
             }
 
-            function Lv({
+            function Ov({
                 buffer: t,
                 numInstances: e,
                 attribute: n,
                 fromLength: i,
                 fromStartIndices: r,
                 getData: s = (t => t)
             }) {
                 const o = n.doublePrecision && n.value instanceof Float64Array ? 2 : 1,
                     a = n.size * o,
                     l = n.byteOffset,
                     c = n.startIndices,
                     h = r && c,
-                    u = Ov(n, e),
+                    u = Lv(n, e),
                     d = n.isConstant;
                 if (!h && i >= u) return;
                 const p = d ? n.value : n.getBuffer().getData({
                     srcByteOffset: l
                 });
                 if (n.settings.normalized && !d) {
                     const t = s;
@@ -19641,37 +19642,37 @@
                             default:
                                 n = !1
                         }
                         if (!n) throw new Error("Illegal attribute generated for ".concat(this.id))
                     }
                 }
             }
-            const Iv = "out vec4 transform_output;\nvoid main() {\n  transform_output = vec4(0);\n}",
-                Rv = "#version 300 es\n".concat(Iv);
+            const Rv = "out vec4 transform_output;\nvoid main() {\n  transform_output = vec4(0);\n}",
+                Iv = "#version 300 es\n".concat(Rv);
 
             function jv(t, e) {
                 e = Array.isArray(e) ? e : [e];
                 const n = t.replace(/^\s+/, "").split(/\s+/),
                     [i, r, s] = n;
                 return e.includes(i) && r && s ? {
                     qualifier: i,
                     type: r,
                     name: s.split(";")[0]
                 } : null
             }
 
-            function zv() {
+            function Fv() {
                 let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                 const {
                     version: e = 100,
                     input: n,
                     inputType: i,
                     output: r
                 } = t;
-                if (!n) return 300 === e ? Rv : e > 300 ? "#version ".concat(e, "\n").concat(Iv) : "void main() {gl_FragColor = vec4(0);}";
+                if (!n) return 300 === e ? Iv : e > 300 ? "#version ".concat(e, "\n").concat(Rv) : "void main() {gl_FragColor = vec4(0);}";
                 const s = function(t, e) {
                     switch (e) {
                         case "float":
                             return "vec4(".concat(t, ", 0.0, 0.0, 1.0)");
                         case "vec2":
                             return "vec4(".concat(t, ", 0.0, 1.0)");
                         case "vec3":
@@ -19680,24 +19681,24 @@
                             return t;
                         default:
                             return Nh(!1), null
                     }
                 }(n, i);
                 return e >= 300 ? "#version ".concat(e, " ").concat(300 === e ? "es" : "", "\nin ").concat(i, " ").concat(n, ";\nout vec4 ").concat(r, ";\nvoid main() {\n  ").concat(r, " = ").concat(s, ";\n}") : "varying ".concat(i, " ").concat(n, ";\nvoid main() {\n  gl_FragColor = ").concat(s, ";\n}")
             }
-            class Fv extends Ld {
+            class zv extends Od {
                 get[Symbol.toStringTag]() {
                     return "TransformFeedback"
                 }
                 static isSupported(t) {
                     return Mu(t)
                 }
                 constructor(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
-                    Lu(t), super(t, e), this.initialize(e), this.stubRemovedMethods("TransformFeedback", "v6.0", ["pause", "resume"]), Object.seal(this)
+                    Ou(t), super(t, e), this.initialize(e), this.stubRemovedMethods("TransformFeedback", "v6.0", ["pause", "resume"]), Object.seal(this)
                 }
                 initialize() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     return this.buffers = {}, this.unused = {}, this.configuration = null, this.bindOnUse = !0, Ad(this.buffers) || this.bind((() => this._unbindBuffers())), this.setProps(t), this
                 }
                 setProps(t) {
                     "program" in t && (this.configuration = t.program && t.program.configuration), "configuration" in t && (this.configuration = t.configuration), "bindOnUse" in t && (t = t.bindOnUse), "buffers" in t && this.setBuffers(t.buffers)
@@ -19870,15 +19871,15 @@
                 _setupTransformFeedback(t, e) {
                     let {
                         model: n
                     } = e;
                     const {
                         program: i
                     } = n;
-                    t.transformFeedback = new Fv(this.gl, {
+                    t.transformFeedback = new zv(this.gl, {
                         program: i,
                         buffers: t.feedbackBuffers
                     })
                 }
                 _updateBindings(t) {
                     if (this.bindings[this.currentIndex] = this._updateBinding(this.bindings[this.currentIndex], t), this.feedbackMap) {
                         const {
@@ -20308,28 +20309,28 @@
                         vs: t.vs,
                         sourceTextureMap: e,
                         targetTextureVarying: this.targetTextureVarying,
                         targetTexture: n
                     }), l = cu([t.inject || {}, o]);
                     return this.targetTextureType = s, this.samplerTextureMap = a, {
                         vs: i,
-                        fs: t._fs || zv({
+                        fs: t._fs || Fv({
                             version: Dv(i),
                             input: this.targetTextureVarying,
                             inputType: s,
                             output: "transform_output"
                         }),
                         modules: this.hasSourceTextures || this.targetTextureVarying ? [Nv].concat(t.modules || []) : t.modules,
                         uniforms: r,
                         inject: l
                     }
                 }
             }
             let Hv = null;
-            class Zv extends Ld {
+            class Zv extends Od {
                 get[Symbol.toStringTag]() {
                     return "VertexArrayObject"
                 }
                 static isSupported(t) {
                     return !(arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {}).constantAttributeZero || Mu(t) || "Chrome" === vm()
                 }
                 static getDefaultArray(t) {
@@ -20733,15 +20734,15 @@
                 if (Math.abs(t) < 1e-16) return n ? "0" : "0.";
                 if (n) return t.toFixed(0);
                 if (Math.abs(t) > 100 && Math.abs(t) < 1e4) return t.toFixed(0);
                 const i = t.toPrecision(2);
                 return i.indexOf(".0") === i.length - 2 ? i.slice(0, -1) : i
             }
 
-            function $v(t, e, n, i) {
+            function Jv(t, e, n, i) {
                 const {
                     gl: r
                 } = t;
                 if (!e) return {
                     [i]: "null",
                     "Format ": "N/A"
                 };
@@ -20773,23 +20774,23 @@
                         size: c,
                         isInteger: s
                     }), " (constant)"),
                     "Format ": "".concat(c, "x").concat(l, " (constant)")
                 }
             }
 
-            function Jv(t, e) {
+            function Qv(t, e) {
                 const {
                     type: n,
                     size: i
                 } = e, r = Kp(n, i);
                 return r ? "".concat(t, " (").concat(r.name, ")") : t
             }
 
-            function Qv(t) {
+            function $v(t) {
                 let {
                     header: e = "Uniforms",
                     program: n,
                     uniforms: i,
                     undefinedOnly: r = !1
                 } = t;
                 wd(n);
@@ -21175,15 +21176,15 @@
                 }
                 _setFeedbackBuffers() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     if (Ad(t)) return this;
                     const {
                         gl: e
                     } = this.program;
-                    return this.transformFeedback = this.transformFeedback || new Fv(e, {
+                    return this.transformFeedback = this.transformFeedback || new zv(e, {
                         program: this.program
                     }), this.transformFeedback.setBuffers(t), this
                 }
                 _logDrawCallStart(t) {
                     const e = t > 3 ? 0 : 1e4;
                     if (!(Date.now() - this.lastLogTime < e)) return this.lastLogTime = Date.now(), Su.group(2, ">>> DRAWING MODEL ".concat(this.id), {
                         collapsed: Su.level <= 2
@@ -21194,43 +21195,43 @@
                     const r = function(t) {
                             let {
                                 vertexArray: e,
                                 header: n = "Attributes"
                             } = t;
                             if (!e.configuration) return {};
                             const i = {};
-                            e.elements && (i.ELEMENT_ARRAY_BUFFER = $v(e, e.elements, null, n));
+                            e.elements && (i.ELEMENT_ARRAY_BUFFER = Jv(e, e.elements, null, n));
                             const r = e.values;
                             for (const t in r) {
                                 const s = e._getAttributeInfo(t);
                                 if (s) {
                                     let o = "".concat(t, ": ").concat(s.name);
                                     const a = e.accessors[s.location];
-                                    a && (o = "".concat(t, ": ").concat(Jv(s.name, a))), i[o] = $v(e, r[t], a, n)
+                                    a && (o = "".concat(t, ": ").concat(Qv(s.name, a))), i[o] = Jv(e, r[t], a, n)
                                 }
                             }
                             return i
                         }({
                             vertexArray: e,
                             header: "".concat(this.id, " attributes"),
                             attributes: this._attributes
                         }),
                         {
                             table: s,
                             unusedTable: o,
                             unusedCount: a
-                        } = Qv({
+                        } = $v({
                             header: "".concat(this.id, " uniforms"),
                             program: this.program,
                             uniforms: Object.assign({}, this.program.uniforms, n)
                         }),
                         {
                             table: l,
                             count: c
-                        } = Qv({
+                        } = $v({
                             header: "".concat(this.id, " uniforms"),
                             program: this.program,
                             uniforms: Object.assign({}, this.program.uniforms, n),
                             undefinedOnly: !0
                         });
                     c > 0 && Su.log("MISSING UNIFORMS", Object.keys(l))(), a > 0 && Su.log("UNUSED UNIFORMS", Object.keys(o))();
                     const h = function(t) {
@@ -21311,15 +21312,15 @@
                 }
                 _initialize() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     const {
                         gl: e
                     } = this;
                     this._buildResourceTransforms(e, t), t = this._updateModelProps(t), this.model = new ab(e, Object.assign({}, t, {
-                        fs: t.fs || zv({
+                        fs: t.fs || Fv({
                             version: Dv(t.vs)
                         }),
                         id: t.id || "transform-model",
                         drawMode: t.drawMode || 0,
                         vertexCount: t.elementCount
                     })), this.bufferTransform && this.bufferTransform.setupResources({
                         model: this.model
@@ -21349,15 +21350,15 @@
             const cb = {
                 interpolation: class {
                     constructor({
                         gl: t,
                         attribute: e,
                         timeline: n
                     }) {
-                        wo(this, "gl", void 0), wo(this, "type", "interpolation"), wo(this, "attributeInTransition", void 0), wo(this, "settings", void 0), wo(this, "attribute", void 0), wo(this, "transition", void 0), wo(this, "currentStartIndices", void 0), wo(this, "currentLength", void 0), wo(this, "transform", void 0), wo(this, "buffers", void 0), this.gl = t, this.transition = new Rf(n), this.attribute = e, this.attributeInTransition = new kv(t, e.settings), this.currentStartIndices = e.startIndices, this.currentLength = 0, this.transform = function(t, e) {
+                        wo(this, "gl", void 0), wo(this, "type", "interpolation"), wo(this, "attributeInTransition", void 0), wo(this, "settings", void 0), wo(this, "attribute", void 0), wo(this, "transition", void 0), wo(this, "currentStartIndices", void 0), wo(this, "currentLength", void 0), wo(this, "transform", void 0), wo(this, "buffers", void 0), this.gl = t, this.transition = new If(n), this.attribute = e, this.attributeInTransition = new kv(t, e.settings), this.currentStartIndices = e.startIndices, this.currentLength = 0, this.transform = function(t, e) {
                             const n = Av(e.size);
                             return new lb(t, {
                                 vs: "\n#define SHADER_NAME interpolation-transition-vertex-shader\n\nuniform float time;\nattribute ATTRIBUTE_TYPE aFrom;\nattribute ATTRIBUTE_TYPE aTo;\nvarying ATTRIBUTE_TYPE vCurrent;\n\nvoid main(void) {\n  vCurrent = mix(aFrom, aTo, time);\n  gl_Position = vec4(0.0);\n}\n",
                                 defines: {
                                     ATTRIBUTE_TYPE: n
                                 },
                                 varyings: ["vCurrent"]
@@ -21384,19 +21385,19 @@
                         const s = {
                             numInstances: e,
                             attribute: r,
                             fromLength: this.currentLength,
                             fromStartIndices: this.currentStartIndices,
                             getData: t.enter
                         };
-                        for (const t of i) Lv({
+                        for (const t of i) Ov({
                             buffer: t,
                             ...s
                         });
-                        this.currentStartIndices = r.startIndices, this.currentLength = Ov(r, e), this.attributeInTransition.setData({
+                        this.currentStartIndices = r.startIndices, this.currentLength = Lv(r, e), this.attributeInTransition.setData({
                             buffer: i[1],
                             value: r.value
                         }), this.transition.start(t), this.transform.update({
                             elementCount: Math.floor(this.currentLength / r.size),
                             sourceBuffers: {
                                 aFrom: i[0],
                                 aTo: Tv(0, r)
@@ -21432,15 +21433,15 @@
                 },
                 spring: class {
                     constructor({
                         gl: t,
                         attribute: e,
                         timeline: n
                     }) {
-                        wo(this, "gl", void 0), wo(this, "type", "spring"), wo(this, "attributeInTransition", void 0), wo(this, "settings", void 0), wo(this, "attribute", void 0), wo(this, "transition", void 0), wo(this, "currentStartIndices", void 0), wo(this, "currentLength", void 0), wo(this, "texture", void 0), wo(this, "framebuffer", void 0), wo(this, "transform", void 0), wo(this, "buffers", void 0), this.gl = t, this.type = "spring", this.transition = new Rf(n), this.attribute = e, this.attributeInTransition = new kv(t, {
+                        wo(this, "gl", void 0), wo(this, "type", "spring"), wo(this, "attributeInTransition", void 0), wo(this, "settings", void 0), wo(this, "attribute", void 0), wo(this, "transition", void 0), wo(this, "currentStartIndices", void 0), wo(this, "currentLength", void 0), wo(this, "texture", void 0), wo(this, "framebuffer", void 0), wo(this, "transform", void 0), wo(this, "buffers", void 0), this.gl = t, this.type = "spring", this.transition = new If(n), this.attribute = e, this.attributeInTransition = new kv(t, {
                             ...e.settings,
                             normalized: !1
                         }), this.currentStartIndices = e.startIndices, this.currentLength = 0, this.texture = function(t) {
                             return new Kd(t, {
                                 data: new Uint8Array(4),
                                 format: 6408,
                                 type: 5121,
@@ -21488,19 +21489,19 @@
                         } = this, s = {
                             numInstances: e,
                             attribute: r,
                             fromLength: this.currentLength,
                             fromStartIndices: this.currentStartIndices,
                             getData: t.enter
                         };
-                        for (const t of i) Lv({
+                        for (const t of i) Ov({
                             buffer: t,
                             ...s
                         });
-                        this.settings = t, this.currentStartIndices = r.startIndices, this.currentLength = Ov(r, e), this.attributeInTransition.setData({
+                        this.settings = t, this.currentStartIndices = r.startIndices, this.currentLength = Lv(r, e), this.attributeInTransition.setData({
                             buffer: i[1],
                             value: r.value
                         }), this.transition.start({
                             ...t,
                             duration: 1 / 0
                         }), this.transform.update({
                             elementCount: Math.floor(this.currentLength / r.size),
@@ -21773,15 +21774,15 @@
                         n += r * r
                     }
                     return Math.sqrt(n)
                 }
                 return Math.abs(t - e)
             }
             const mb = {
-                interpolation: class extends Rf {
+                interpolation: class extends If {
                     get value() {
                         return this._value
                     }
                     _onUpdate() {
                         const {
                             time: t,
                             settings: {
@@ -21790,15 +21791,15 @@
                                 duration: i,
                                 easing: r
                             }
                         } = this, s = r(t / i);
                         this._value = ac(e, n, s)
                     }
                 },
-                spring: class extends Rf {
+                spring: class extends If {
                     get value() {
                         return this._currValue
                     }
                     _onUpdate() {
                         const {
                             fromValue: t,
                             toValue: e,
@@ -21962,15 +21963,15 @@
                         n.inject = i
                     } else n.inject = e.inject;
                 return n
             }
 
             function Sb(t, e, n = !1) {
                 const i = e.projectPosition(t);
-                if (n && e instanceof If) {
+                if (n && e instanceof Rf) {
                     const [n, r, s = 0] = t, o = e.getDistanceScales([n, r]);
                     i[2] = s * o.unitsPerMeter[2]
                 }
                 return i
             }
 
             function Cb(t, {
@@ -22005,27 +22006,27 @@
                         validate: (t, e) => !0,
                         equal: (t, e, n) => Boolean(t) === Boolean(e)
                     },
                     number: {
                         validate: (t, e) => Number.isFinite(t) && (!("max" in e) || t <= e.max) && (!("min" in e) || t >= e.min)
                     },
                     color: {
-                        validate: (t, e) => e.optional && !t || Ib(t) && (3 === t.length || 4 === t.length),
-                        equal: (t, e, n) => Ob(t, e)
+                        validate: (t, e) => e.optional && !t || Rb(t) && (3 === t.length || 4 === t.length),
+                        equal: (t, e, n) => Lb(t, e)
                     },
                     accessor: {
                         validate(t, e) {
-                            const n = Rb(t);
-                            return "function" === n || n === Rb(e.value)
+                            const n = Ib(t);
+                            return "function" === n || n === Ib(e.value)
                         },
-                        equal: (t, e, n) => "function" == typeof e || Ob(t, e)
+                        equal: (t, e, n) => "function" == typeof e || Lb(t, e)
                     },
                     array: {
-                        validate: (t, e) => e.optional && !t || Ib(t),
-                        equal: (t, e, n) => n.compare ? Ob(t, e) : t === e
+                        validate: (t, e) => e.optional && !t || Rb(t),
+                        equal: (t, e, n) => n.compare ? Lb(t, e) : t === e
                     },
                     object: {
                         equal: (t, e, n) => n.compare ? Pf(t, e) : t === e
                     },
                     function: {
                         validate: (t, e) => e.optional && !t || "function" == typeof t,
                         equal: (t, e, n) => !n.compare || t === e
@@ -22063,26 +22064,26 @@
                         release: t => {
                             var e;
                             (e = t) && e instanceof Kd && Ab[e.id] && (e.delete(), delete Ab[e.id])
                         }
                     }
                 };
 
-            function Ob(t, e) {
+            function Lb(t, e) {
                 if (t === e) return !0;
-                if (!Ib(t) || !Ib(e)) return !1;
+                if (!Rb(t) || !Rb(e)) return !1;
                 const n = t.length;
                 if (n !== e.length) return !1;
                 for (let i = 0; i < n; i++)
                     if (t[i] !== e[i]) return !1;
                 return !0
             }
 
-            function Lb(t, e) {
-                switch (Rb(e)) {
+            function Ob(t, e) {
+                switch (Ib(e)) {
                     case "object":
                         return kb(t, e);
                     case "array":
                         return kb(t, {
                             type: "array",
                             value: e,
                             compare: !1
@@ -22113,29 +22114,29 @@
             function kb(t, e) {
                 return "type" in e ? {
                     name: t,
                     ...Mb[e.type],
                     ...e
                 } : "value" in e ? {
                     name: t,
-                    type: Rb(e.value),
+                    type: Ib(e.value),
                     ...e
                 } : {
                     name: t,
                     type: "object",
                     value: e
                 }
             }
 
-            function Ib(t) {
+            function Rb(t) {
                 return Array.isArray(t) || ArrayBuffer.isView(t)
             }
 
-            function Rb(t) {
-                return Ib(t) ? "array" : null === t ? "null" : typeof t
+            function Ib(t) {
+                return Rb(t) ? "array" : null === t ? "null" : typeof t
             }
 
             function jb(t) {
                 return Bb(t, "_mergedDefaultProps") || (function(t) {
                     if (!t.prototype) return;
                     const e = Object.getPrototypeOf(t),
                         n = jb(e),
@@ -22143,15 +22144,15 @@
                             const e = {},
                                 n = {},
                                 i = {};
                             for (const [r, s] of Object.entries(t)) {
                                 const t = null == s ? void 0 : s.deprecatedFor;
                                 if (t) i[r] = Array.isArray(t) ? t : [t];
                                 else {
-                                    const t = Lb(r, s);
+                                    const t = Ob(r, s);
                                     e[r] = t, n[r] = t.value
                                 }
                             }
                             return {
                                 propTypes: e,
                                 defaultProps: n,
                                 deprecatedProps: i
@@ -22180,36 +22181,36 @@
                             i = {};
                         for (const t in e) {
                             const r = e[t],
                                 {
                                     name: s,
                                     value: o
                                 } = r;
-                            r.async && (n[s] = o, i[s] = zb(s))
+                            r.async && (n[s] = o, i[s] = Fb(s))
                         }
                         t[To] = n, t[Ao] = {}, Object.defineProperties(t, i)
                     }(r, s);
                     const o = {
                         ...e._deprecatedProps,
                         ...i.deprecatedProps
                     };
                     (function(t, e) {
                         for (const n in e) Object.defineProperty(t, n, {
                             enumerable: !1,
                             set(t) {
                                 const i = "".concat(this.id, ": ").concat(n);
-                                for (const i of e[n]) Fb(this, i) || (this[i] = t);
+                                for (const i of e[n]) zb(this, i) || (this[i] = t);
                                 ta.deprecated(i, e[n].join("/"))()
                             }
                         })
                     })(r, o), t._mergedDefaultProps = r, t._propTypes = s, t._deprecatedProps = o
                 }(t), t._mergedDefaultProps)
             }
 
-            function zb(t) {
+            function Fb(t) {
                 return {
                     enumerable: !0,
                     set(e) {
                         "string" == typeof e || e instanceof Promise || _v(e) ? this[Ao][t] = e : this[Mo][t] = e
                     },
                     get() {
                         if (this[Mo]) {
@@ -22220,20 +22221,20 @@
                             }
                         }
                         return this[To][t]
                     }
                 }
             }
 
-            function Fb(t, e) {
+            function zb(t, e) {
                 return Object.prototype.hasOwnProperty.call(t, e)
             }
 
             function Bb(t, e) {
-                return Fb(t, e) && t[e]
+                return zb(t, e) && t[e]
             }
             let Db = 0;
             class Nb {
                 constructor(...t) {
                     wo(this, "id", void 0), wo(this, "props", void 0), wo(this, "count", void 0), this.props = function(t, e) {
                         const n = jb(t.constructor),
                             i = Object.create(n);
@@ -22481,38 +22482,38 @@
                                 ...null === (a = r) || void 0 === a ? void 0 : a.fetch,
                                 signal: s
                             }
                         });
                         let l = o.contains(t);
                         return l || r || (o.add({
                             resourceId: t,
-                            data: Ql(t, i),
+                            data: $l(t, i),
                             persistent: !1
                         }), l = !0), l ? o.subscribe({
                             resourceId: t,
                             onChange: t => {
                                 var i;
                                 return null === (i = n.internalState) || void 0 === i ? void 0 : i.reloadAsyncProp(e, t)
                             },
                             consumerId: n.id,
                             requestId: e
-                        }) : Ql(t, i, r)
+                        }) : $l(t, i, r)
                     },
                     compare: !1
                 },
                 updateTriggers: {},
                 visible: !0,
                 pickable: !1,
                 opacity: {
                     type: "number",
                     min: 0,
                     max: 1,
                     value: 1
                 },
-                operation: Lh,
+                operation: Oh,
                 onHover: {
                     type: "function",
                     value: null,
                     compare: !1,
                     optional: !0
                 },
                 onClick: {
@@ -23166,41 +23167,41 @@
             }
             wo(Yb, "defaultProps", Xb), wo(Yb, "layerName", "Layer");
             const Kb = {
                 position: "absolute",
                 zIndex: -1
             };
 
-            function $b(t, e) {
+            function Jb(t, e) {
                 if ("function" == typeof t) return t(e);
-                if (Array.isArray(t)) return t.map((t => $b(t, e)));
-                if (Jb(t)) {
+                if (Array.isArray(t)) return t.map((t => Jb(t, e)));
+                if (Qb(t)) {
                     if (function(t) {
                             const e = t.type,
                                 n = e && e.defaultProps;
                             return n && n.mapStyle
                         }(t)) return e.style = Kb, (0, c.cloneElement)(t, e);
                     if (function(t) {
                             const e = t.type;
                             return e && e.deckGLViewProps
                         }(t)) return (0, c.cloneElement)(t, e)
                 }
                 return t
             }
 
-            function Jb(t) {
+            function Qb(t) {
                 return t && "object" == typeof t && "type" in t || !1
             }
 
-            function Qb(t) {
-                if ("function" == typeof t) return (0, c.createElement)(Of, {}, t);
-                if (Array.isArray(t)) return t.map(Qb);
-                if (Jb(t)) {
-                    if (t.type === c.Fragment) return Qb(t.props.children);
-                    if (dv(t.type, Of)) return t
+            function $b(t) {
+                if ("function" == typeof t) return (0, c.createElement)(Lf, {}, t);
+                if (Array.isArray(t)) return t.map($b);
+                if (Qb(t)) {
+                    if (t.type === c.Fragment) return $b(t.props.children);
+                    if (dv(t.type, Lf)) return t
                 }
                 return t
             }
             const ty = {
                 mixBlendMode: null
             };
 
@@ -23216,27 +23217,27 @@
                     children: t,
                     layers: e = [],
                     views: n = null
                 }) {
                     const i = [],
                         r = [],
                         s = {};
-                    return c.Children.forEach(Qb(t), (t => {
-                        if (Jb(t)) {
+                    return c.Children.forEach($b(t), (t => {
+                        if (Qb(t)) {
                             const e = t.type;
                             if (dv(e, Yb)) {
                                 const n = function(t, e) {
                                     const n = {},
                                         i = t.defaultProps || {};
                                     for (const t in e) i[t] !== e[t] && (n[t] = e[t]);
                                     return new t(n)
                                 }(e, t.props);
                                 r.push(n)
                             } else i.push(t);
-                            if (dv(e, Of) && e !== Of && t.props.id) {
+                            if (dv(e, Lf) && e !== Lf && t.props.id) {
                                 const n = new e(t.props);
                                 s[n.id] = n
                             }
                         } else t && i.push(t)
                     })), Object.keys(s).length > 0 && (Array.isArray(n) ? n.forEach((t => {
                         s[t.id] = t
                     })) : n && (s[n.id] = n), n = Object.values(s)), {
@@ -23357,25 +23358,25 @@
                             } = e || {};
                             if (!i || !i.views.length) return [];
                             const r = {},
                                 s = i.views[0].id;
                             for (const e of t) {
                                 let t = s,
                                     n = e;
-                                Jb(e) && dv(e.type, Of) && (t = e.props.id || s, n = e.props.children);
+                                Qb(e) && dv(e.type, Lf) && (t = e.props.id || s, n = e.props.children);
                                 const o = i.getViewport(t),
                                     a = i.getViewState(t);
                                 if (o) {
                                     const {
                                         x: e,
                                         y: i,
                                         width: s,
                                         height: l
                                     } = o;
-                                    n = $b(n, {
+                                    n = Jb(n, {
                                         x: e,
                                         y: i,
                                         width: s,
                                         height: l,
                                         viewport: o,
                                         viewState: a
                                     }), r[t] || (r[t] = {
@@ -23902,15 +23903,15 @@
                 let h = [];
                 for (; l.length;) {
                     const {
                         pos: t,
                         types: e,
                         holes: n
                     } = l.shift();
-                    Oy(t, i, n[0] || t.length, c), h = Ay(c[0], r, s, h);
+                    Ly(t, i, n[0] || t.length, c), h = Ay(c[0], r, s, h);
                     const u = yy(c[1], h);
                     if (u) {
                         let r = Ty(t, e, i, 0, n[0] || t.length, h, u);
                         const s = {
                                 pos: r[0].pos,
                                 types: r[0].types,
                                 holes: []
@@ -23961,28 +23962,28 @@
                 return i[0] = r, i[1] = s, i[2] = r + e, i[3] = s + e, i
             }
 
             function My(t, e, n) {
                 8 & n ? (t[1] += e, t[3] += e) : 4 & n ? (t[1] -= e, t[3] -= e) : 2 & n ? (t[0] += e, t[2] += e) : 1 & n && (t[0] -= e, t[2] -= e)
             }
 
-            function Oy(t, e, n, i) {
+            function Ly(t, e, n, i) {
                 let r = 1 / 0,
                     s = -1 / 0,
                     o = 1 / 0,
                     a = -1 / 0;
                 for (let i = 0; i < n; i += e) {
                     const e = t[i],
                         n = t[i + 1];
                     r = e < r ? e : r, s = e > s ? e : s, o = n < o ? n : o, a = n > a ? n : a
                 }
                 return i[0][0] = r, i[0][1] = o, i[1][0] = s, i[1][1] = a, i
             }
 
-            function Ly(t, e, n, i) {
+            function Oy(t, e, n, i) {
                 let r = -1,
                     s = -1;
                 for (let o = n + 1; o < i; o += e) {
                     const e = Math.abs(t[o]);
                     e > r && (r = e, s = o - 1)
                 }
                 return s
@@ -23993,40 +23994,40 @@
                     o = t[i - e];
                 if (Math.abs(s - o) > 180) {
                     const i = wy(t, 0, e, n);
                     i[0] += 360 * Math.round((o - s) / 360), _y(t, i), i[1] = Math.sign(i[1]) * r, _y(t, i), i[0] = s, _y(t, i)
                 }
             }
 
-            function Iy(t, e, n, i) {
+            function Ry(t, e, n, i) {
                 let r, s = t[0];
                 for (let o = n; o < i; o += e) {
                     r = t[o];
                     const e = r - s;
                     (e > 180 || e < -180) && (r -= 360 * Math.round(e / 360)), t[o] = s = r
                 }
             }
 
-            function Ry(t, e) {
+            function Iy(t, e) {
                 let n;
                 const i = t.length / e;
                 for (let r = 0; r < i && (n = t[r * e], (n + 180) % 360 == 0); r++);
                 const r = 360 * -Math.round(n / 360);
                 if (0 !== r)
                     for (let n = 0; n < i; n++) t[n * e] += r
             }
             const jy = {
                 isClosed: !0
             };
 
-            function zy(t) {
+            function Fy(t) {
                 return "positions" in t ? t.positions : t
             }
 
-            function Fy(t) {
+            function zy(t) {
                 return "holeIndices" in t ? t.holeIndices : null
             }
 
             function By(t, e, n, i, r) {
                 let s = e;
                 const o = n.length;
                 for (let e = 0; e < o; e++)
@@ -24230,15 +24231,15 @@
                     const e = this.buffers.indices;
                     if (e) this.vertexCount = (e.value || e).length;
                     else if (this.data && !this.getGeometry) throw new Error("missing indices buffer")
                 }
                 normalizeGeometry(t) {
                     if (this.normalize) {
                         const e = Ny(t, this.positionSize);
-                        return this.opts.resolution ? Cy(zy(e), Fy(e), {
+                        return this.opts.resolution ? Cy(Fy(e), zy(e), {
                             size: this.positionSize,
                             gridResolution: this.opts.resolution,
                             edgeTypes: !0
                         }) : this.opts.wrapLongitude ? function(t, e = null, n) {
                             const {
                                 size: i = 2,
                                 normalize: r = !0,
@@ -24248,44 +24249,44 @@
                             const o = [],
                                 a = [];
                             let l = 0,
                                 c = 0;
                             for (let r = 0; r <= e.length; r++) {
                                 const s = e[r] || t.length,
                                     h = c,
-                                    u = Ly(t, i, l, s);
+                                    u = Oy(t, i, l, s);
                                 for (let e = u; e < s; e++) o[c++] = t[e];
                                 for (let e = l; e < u; e++) o[c++] = t[e];
-                                Iy(o, i, h, c), ky(o, i, h, c, null == n ? void 0 : n.maxLatitude), l = s, a[r] = c
+                                Ry(o, i, h, c), ky(o, i, h, c, null == n ? void 0 : n.maxLatitude), l = s, a[r] = c
                             }
                             a.pop();
                             const h = Cy(o, a, {
                                 size: i,
                                 gridResolution: 360,
                                 gridOffset: [-180, -180],
                                 edgeTypes: s
                             });
                             if (r)
-                                for (const t of h) Ry(t.positions, i);
+                                for (const t of h) Iy(t.positions, i);
                             return h
-                        }(zy(e), Fy(e), {
+                        }(Fy(e), zy(e), {
                             size: this.positionSize,
                             maxLatitude: 86,
                             edgeTypes: !0
                         }) : e
                     }
                     return t
                 }
                 getGeometrySize(t) {
                     if (Gy(t)) {
                         let e = 0;
                         for (const n of t) e += this.getGeometrySize(n);
                         return e
                     }
-                    return zy(t).length / this.positionSize
+                    return Fy(t).length / this.positionSize
                 }
                 getGeometryFromBuffer(t) {
                     return this.normalize || !this.buffers.indices ? super.getGeometryFromBuffer(t) : null
                 }
                 updateGeometryAttributes(t, e) {
                     if (t && Gy(t))
                         for (const n of t) {
@@ -24303,17 +24304,17 @@
                         indexStarts: s,
                         typedArrayManager: o
                     } = this;
                     let a = r.indices;
                     if (!a || !t) return;
                     let l = i;
                     const c = function(t, e, n) {
-                        let i = Fy(t);
+                        let i = zy(t);
                         i && (i = i.map((t => t / e)));
-                        let r = zy(t);
+                        let r = Fy(t);
                         if (n) {
                             const t = r.length;
                             r = r.slice();
                             const i = [];
                             for (let s = 0; s < t; s += e) {
                                 i[0] = r[s], i[1] = r[s + 1];
                                 const t = n(i);
@@ -24335,29 +24336,29 @@
                     const {
                         attributes: {
                             positions: i
                         },
                         positionSize: r
                     } = this;
                     if (!i || !t) return;
-                    const s = zy(t);
+                    const s = Fy(t);
                     for (let t = e, o = 0; o < n; t++, o++) {
                         const e = s[o * r],
                             n = s[o * r + 1],
                             a = r > 2 ? s[o * r + 2] : 0;
                         i[3 * t] = e, i[3 * t + 1] = n, i[3 * t + 2] = a
                     }
                 }
                 _updateVertexValid(t, {
                     vertexStart: e,
                     geometrySize: n
                 }) {
                     const {
                         positionSize: i
-                    } = this, r = this.attributes.vertexValid, s = t && Fy(t);
+                    } = this, r = this.attributes.vertexValid, s = t && zy(t);
                     if (t && t.edgeTypes ? r.set(t.edgeTypes, e) : r.fill(1, e, e + n), s)
                         for (let t = 0; t < s.length; t++) r[e + s[t] / i - 1] = 0;
                     r[e + n - 1] = 0
                 }
             }
 
             function Gy(t) {
@@ -24671,15 +24672,15 @@
                     t.startIndices = e.vertexStarts, t.value = e.get("positions")
                 }
                 calculateVertexValid(t) {
                     t.value = this.state.polygonTesselator.get("vertexValid")
                 }
             }
             wo(Ky, "defaultProps", Xy), wo(Ky, "layerName", "SolidPolygonLayer");
-            class $y extends Vy {
+            class Jy extends Vy {
                 constructor(t) {
                     super({
                         ...t,
                         attributes: {
                             positions: {
                                 size: 3,
                                 padding: 18,
@@ -24714,41 +24715,41 @@
                         }) : i ? function(t, e) {
                             const {
                                 size: n = 2,
                                 startIndex: i = 0,
                                 endIndex: r = t.length,
                                 normalize: s = !0
                             } = e || {}, o = t.slice(i, r);
-                            Iy(o, n, 0, r - i);
+                            Ry(o, n, 0, r - i);
                             const a = Ey(o, {
                                 size: n,
                                 broken: !0,
                                 gridResolution: 360,
                                 gridOffset: [-180, -180]
                             });
                             if (s)
-                                for (const t of a) Ry(t, n);
+                                for (const t of a) Iy(t, n);
                             return a
                         }(r, {
                             size: e
                         }) : r
                     }(t, this.positionSize, this.opts.resolution, this.opts.wrapLongitude) : t
                 }
                 getGeometrySize(t) {
-                    if (Jy(t)) {
+                    if (Qy(t)) {
                         let e = 0;
                         for (const n of t) e += this.getGeometrySize(n);
                         return e
                     }
                     const e = this.getPathLength(t);
                     return e < 2 ? 0 : this.isClosed(t) ? e < 3 ? 0 : e + 2 : e
                 }
                 updateGeometryAttributes(t, e) {
                     if (0 !== e.geometrySize)
-                        if (t && Jy(t))
+                        if (t && Qy(t))
                             for (const n of t) {
                                 const t = this.getGeometrySize(n);
                                 e.geometrySize = t, this.updateGeometryAttributes(n, e), e.vertexStart += t
                             } else this._updateSegmentTypes(t, e), this._updatePositions(t, e)
                 }
                 _updateSegmentTypes(t, e) {
                     const n = this.attributes.segmentTypes,
@@ -24786,18 +24787,18 @@
                     const {
                         positionSize: e
                     } = this, n = t.length - e;
                     return t[0] === t[n] && t[1] === t[n + 1] && (2 === e || t[2] === t[n + 2])
                 }
             }
 
-            function Jy(t) {
+            function Qy(t) {
                 return Array.isArray(t[0])
             }
-            const Qy = [0, 0, 0, 255],
+            const $y = [0, 0, 0, 255],
                 t_ = {
                     widthUnits: "meters",
                     widthScale: {
                         type: "number",
                         min: 0,
                         value: 1
                     },
@@ -24822,15 +24823,15 @@
                     _pathType: null,
                     getPath: {
                         type: "accessor",
                         value: t => t.path
                     },
                     getColor: {
                         type: "accessor",
-                        value: Qy
+                        value: $y
                     },
                     getWidth: {
                         type: "accessor",
                         value: 1
                     },
                     rounded: {
                         deprecatedFor: ["jointRounded", "capRounded"]
@@ -24893,26 +24894,26 @@
                         },
                         instanceColors: {
                             size: this.props.colorFormat.length,
                             type: 5121,
                             normalized: !0,
                             accessor: "getColor",
                             transition: e_,
-                            defaultValue: Qy
+                            defaultValue: $y
                         },
                         instancePickingColors: {
                             size: 3,
                             type: 5121,
                             accessor: (t, {
                                 index: e,
                                 target: n
                             }) => this.encodePickingColor(t && t.__source ? t.__source.index : e, n)
                         }
                     }), this.setState({
-                        pathTesselator: new $y({
+                        pathTesselator: new Jy({
                             fp64: this.use64bitPositions()
                         })
                     })
                 }
                 updateState(t) {
                     super.updateState(t);
                     const {
@@ -25177,15 +25178,15 @@
                         getElevation: w,
                         getPolygon: E,
                         updateTriggers: P,
                         material: S
                     } = this.props, {
                         paths: C,
                         pathsDiff: T
-                    } = this.state, A = this.getSubLayerClass("fill", Ky), M = this.getSubLayerClass("stroke", n_), O = this.shouldRenderSubLayer("fill", C) && new A({
+                    } = this.state, A = this.getSubLayerClass("fill", Ky), M = this.getSubLayerClass("stroke", n_), L = this.shouldRenderSubLayer("fill", C) && new A({
                         _dataDiff: e,
                         extruded: r,
                         elevationScale: l,
                         filled: i,
                         wireframe: s,
                         _normalize: o,
                         _windingOrder: a,
@@ -25204,15 +25205,15 @@
                             getLineColor: P.getLineColor
                         }
                     }), {
                         data: t,
                         positionFormat: h,
                         getPolygon: E
                     });
-                    return [!r && O, !r && n && this.shouldRenderSubLayer("stroke", C) && new M({
+                    return [!r && L, !r && n && this.shouldRenderSubLayer("stroke", C) && new M({
                         _dataDiff: T && (() => T),
                         widthUnits: u,
                         widthScale: d,
                         widthMinPixels: p,
                         widthMaxPixels: f,
                         jointRounded: g,
                         miterLimit: m,
@@ -25233,15 +25234,15 @@
                             getColor: P.getLineColor,
                             getDashArray: P.getLineDashArray
                         }
                     }), {
                         data: C,
                         positionFormat: h,
                         getPath: t => t.path
-                    }), r && O]
+                    }), r && L]
                 }
             }
             wo(o_, "layerName", "PolygonLayer"), wo(o_, "defaultProps", s_);
             const a_ = () => {},
                 l_ = {
                     10241: 9987,
                     10240: 9729,
@@ -25416,28 +25417,28 @@
                                 if (e instanceof Yd && (b = e, h = Number.isFinite(h) ? h : b.width, u = Number.isFinite(u) ? u : b.height, b.bind(0), e = b.target), m) switch (e) {
                                     case 3553:
                                     case 34067:
                                         f.copyTexSubImage2D(e, s, a, l, i, r, h, u);
                                         break;
                                     case 35866:
                                     case 32879:
-                                        Lu(f).copyTexSubImage3D(e, s, a, l, c, i, r, h, u)
+                                        Ou(f).copyTexSubImage3D(e, s, a, l, c, i, r, h, u)
                                 } else f.copyTexImage2D(e, s, o, i, r, h, u, 0);
                                 b && b.unbind(), f.bindFramebuffer(36160, v || null), p && d.delete()
                             }(t, o, {
                                 targetY: 0,
                                 width: r,
                                 height: s
                             }), t.delete(), o
                         }(this._texture, this._canvasWidth, this._canvasHeight, this._textureParameters || l_)), this.onUpdate(), this._canvas = this._canvas || document.createElement("canvas"), this._loadIcons(n)
                     }
                 }
                 _loadIcons(t) {
                     const e = this._canvas.getContext("2d");
-                    for (const n of t) this._pendingCount++, Ql(n.url, um, this._loadOptions).then((t => {
+                    for (const n of t) this._pendingCount++, $l(n.url, um, this._loadOptions).then((t => {
                         const i = h_(n),
                             {
                                 x: r,
                                 y: s,
                                 width: o,
                                 height: a
                             } = this._mapping[i],
@@ -26037,15 +26038,15 @@
                 return u[1] = p, {
                     x: a,
                     y: l,
                     rowWidth: c,
                     size: u
                 }
             }
-            class O_ {
+            class L_ {
                 constructor(t = 5) {
                     wo(this, "limit", void 0), wo(this, "_cache", {}), wo(this, "_order", []), this.limit = t
                 }
                 get(t) {
                     const e = this._cache[t];
                     return e && (this._deleteOrder(t), this._appendOrder(t)), e
                 }
@@ -26059,42 +26060,42 @@
                     const e = this._order.indexOf(t);
                     e >= 0 && this._order.splice(e, 1)
                 }
                 _appendOrder(t) {
                     this._order.push(t)
                 }
             }
-            const L_ = {
+            const O_ = {
                 fontFamily: "Monaco, monospace",
                 fontWeight: "normal",
                 characterSet: function() {
                     const t = [];
                     for (let e = 32; e < 128; e++) t.push(String.fromCharCode(e));
                     return t
                 }(),
                 fontSize: 64,
                 buffer: 4,
                 sdf: !1,
                 cutoff: .25,
                 radius: 12,
                 smoothing: .1
             };
-            let k_ = new O_(3);
+            let k_ = new L_(3);
 
-            function I_(t, e) {
+            function R_(t, e) {
                 for (let n = 0; n < t.length; n++) e.data[4 * n + 3] = t[n]
             }
 
-            function R_(t, e, n, i) {
+            function I_(t, e, n, i) {
                 t.font = "".concat(i, " ").concat(n, "px ").concat(e), t.fillStyle = "#000", t.textBaseline = "alphabetic", t.textAlign = "left"
             }
             class j_ {
                 constructor() {
                     wo(this, "props", {
-                        ...L_
+                        ...O_
                     }), wo(this, "_key", void 0), wo(this, "_atlas", void 0)
                 }
                 get texture() {
                     return this._atlas
                 }
                 get mapping() {
                     return this._atlas && this._atlas.mapping
@@ -26128,15 +26129,15 @@
                         sdf: a,
                         radius: l,
                         cutoff: c
                     } = this.props;
                     let h = n && n.data;
                     h || (h = document.createElement("canvas"), h.width = 1024);
                     const u = h.getContext("2d");
-                    R_(u, i, s, r);
+                    I_(u, i, s, r);
                     const {
                         mapping: d,
                         canvasHeight: p,
                         xOffset: f,
                         yOffset: g
                     } = function({
                         characterSet: t,
@@ -26179,18 +26180,18 @@
                             yOffset: n.yOffset
                         }
                     });
                     if (h.height !== p) {
                         const t = u.getImageData(0, 0, h.width, h.height);
                         h.height = p, u.putImageData(t, 0, 0)
                     }
-                    if (R_(u, i, s, r), a) {
+                    if (I_(u, i, s, r), a) {
                         const t = new(w_())(s, o, l, c, i, r),
                             n = u.getImageData(0, 0, t.size, t.size);
-                        for (const i of e) I_(t.draw(i), n), u.putImageData(n, d[i].x - o, d[i].y + o)
+                        for (const i of e) R_(t.draw(i), n), u.putImageData(n, d[i].x - o, d[i].y + o)
                     } else
                         for (const t of e) u.fillText(t, d[t].x, d[t].y + .9 * s);
                     return {
                         xOffset: f,
                         yOffset: g,
                         mapping: d,
                         data: h,
@@ -26207,15 +26208,15 @@
                         sdf: r,
                         radius: s,
                         cutoff: o
                     } = this.props;
                     return r ? "".concat(t, " ").concat(e, " ").concat(n, " ").concat(i, " ").concat(s, " ").concat(o) : "".concat(t, " ").concat(e, " ").concat(n, " ").concat(i)
                 }
             }
-            const z_ = {
+            const F_ = {
                 billboard: !0,
                 sizeScale: 1,
                 sizeUnits: "pixels",
                 sizeMinPixels: 0,
                 sizeMaxPixels: Number.MAX_SAFE_INTEGER,
                 padding: {
                     type: "array",
@@ -26250,15 +26251,15 @@
                     value: [0, 0, 0, 255]
                 },
                 getLineWidth: {
                     type: "accessor",
                     value: 1
                 }
             };
-            class F_ extends Yb {
+            class z_ extends Yb {
                 constructor(...t) {
                     super(...t), wo(this, "state", void 0)
                 }
                 getShaders() {
                     return super.getShaders({
                         vs: "#define SHADER_NAME text-background-layer-vertex-shader\n\nattribute vec2 positions;\n\nattribute vec3 instancePositions;\nattribute vec3 instancePositions64Low;\nattribute vec4 instanceRects;\nattribute float instanceSizes;\nattribute float instanceAngles;\nattribute vec2 instancePixelOffsets;\nattribute float instanceLineWidths;\nattribute vec4 instanceFillColors;\nattribute vec4 instanceLineColors;\nattribute vec3 instancePickingColors;\n\nuniform bool billboard;\nuniform float opacity;\nuniform float sizeScale;\nuniform float sizeMinPixels;\nuniform float sizeMaxPixels;\nuniform vec4 padding;\nuniform int sizeUnits;\n\nvarying vec4 vFillColor;\nvarying vec4 vLineColor;\nvarying float vLineWidth;\nvarying vec2 uv;\nvarying vec2 dimensions;\n\nvec2 rotate_by_angle(vec2 vertex, float angle) {\n  float angle_radian = radians(angle);\n  float cos_angle = cos(angle_radian);\n  float sin_angle = sin(angle_radian);\n  mat2 rotationMatrix = mat2(cos_angle, -sin_angle, sin_angle, cos_angle);\n  return rotationMatrix * vertex;\n}\n\nvoid main(void) {\n  geometry.worldPosition = instancePositions;\n  geometry.uv = positions;\n  geometry.pickingColor = instancePickingColors;\n  uv = positions;\n  vLineWidth = instanceLineWidths;\n\n  // convert size in meters to pixels, then scaled and clamp\n\n  // project meters to pixels and clamp to limits\n  float sizePixels = clamp(\n    project_size_to_pixel(instanceSizes * sizeScale, sizeUnits),\n    sizeMinPixels, sizeMaxPixels\n  );\n\n  dimensions = instanceRects.zw * sizePixels + padding.xy + padding.zw;\n\n  vec2 pixelOffset = (positions * instanceRects.zw + instanceRects.xy) * sizePixels + mix(-padding.xy, padding.zw, positions);\n  pixelOffset = rotate_by_angle(pixelOffset, instanceAngles);\n  pixelOffset += instancePixelOffsets;\n  pixelOffset.y *= -1.0;\n\n  if (billboard)  {\n    gl_Position = project_position_to_clipspace(instancePositions, instancePositions64Low, vec3(0.0), geometry.position);\n    vec3 offset = vec3(pixelOffset, 0.0);\n    DECKGL_FILTER_SIZE(offset, geometry);\n    gl_Position.xy += project_pixel_size_to_clipspace(offset.xy);\n  } else {\n    vec3 offset_common = vec3(project_pixel_size(pixelOffset), 0.0);\n    DECKGL_FILTER_SIZE(offset_common, geometry);\n    gl_Position = project_position_to_clipspace(instancePositions, instancePositions64Low, offset_common, geometry.position);\n  }\n  DECKGL_FILTER_GL_POSITION(gl_Position, geometry);\n\n  // Apply opacity to instance color, or return instance picking color\n  vFillColor = vec4(instanceFillColors.rgb, instanceFillColors.a * opacity);\n  DECKGL_FILTER_COLOR(vFillColor, geometry);\n  vLineColor = vec4(instanceLineColors.rgb, instanceLineColors.a * opacity);\n  DECKGL_FILTER_COLOR(vLineColor, geometry);\n}\n",
                         fs: "#define SHADER_NAME text-background-layer-fragment-shader\n\nprecision highp float;\n\nuniform bool stroked;\n\nvarying vec4 vFillColor;\nvarying vec4 vLineColor;\nvarying float vLineWidth;\nvarying vec2 uv;\nvarying vec2 dimensions;\n\nvoid main(void) {\n  geometry.uv = uv;\n\n  vec2 pixelPosition = uv * dimensions;\n  if (stroked) {\n    float distToEdge = min(\n      min(pixelPosition.x, dimensions.x - pixelPosition.x),\n      min(pixelPosition.y, dimensions.y - pixelPosition.y)\n    );\n    float isBorder = smoothedge(distToEdge, vLineWidth);\n    gl_FragColor = mix(vFillColor, vLineColor, isBorder);\n  } else {\n    gl_FragColor = vFillColor;\n  }\n\n  DECKGL_FILTER_COLOR(gl_FragColor, geometry);\n}\n",
@@ -26369,15 +26370,15 @@
                                 }
                             }
                         }),
                         isInstanced: !0
                     })
                 }
             }
-            wo(F_, "defaultProps", z_), wo(F_, "layerName", "TextBackgroundLayer");
+            wo(z_, "defaultProps", F_), wo(z_, "layerName", "TextBackgroundLayer");
             const B_ = {
                     start: 1,
                     middle: 0,
                     end: -1
                 },
                 D_ = {
                     top: 1,
@@ -26406,18 +26407,18 @@
                     },
                     backgroundPadding: {
                         type: "array",
                         value: [0, 0, 0, 0]
                     },
                     characterSet: {
                         type: "object",
-                        value: L_.characterSet
+                        value: O_.characterSet
                     },
-                    fontFamily: L_.fontFamily,
-                    fontWeight: L_.fontWeight,
+                    fontFamily: O_.fontFamily,
+                    fontWeight: O_.fontWeight,
                     lineHeight: 1,
                     outlineWidth: {
                         type: "number",
                         value: 0,
                         min: 0
                     },
                     outlineColor: {
@@ -26658,16 +26659,16 @@
                         outlineColor: w,
                         sizeScale: E,
                         sizeUnits: P,
                         sizeMinPixels: S,
                         sizeMaxPixels: C,
                         transitions: T,
                         updateTriggers: A
-                    } = this.props, M = this.getSubLayerClass("characters", __), O = this.getSubLayerClass("background", F_);
-                    return [b && new O({
+                    } = this.props, M = this.getSubLayerClass("characters", __), L = this.getSubLayerClass("background", z_);
+                    return [b && new L({
                         getFillColor: f,
                         getLineColor: g,
                         getLineWidth: m,
                         padding: v,
                         getPosition: c,
                         getSize: u,
                         getAngle: d,
@@ -26709,15 +26710,15 @@
                             attributes: a.attributes.background
                         } : a,
                         _dataDiff: l,
                         autoHighlight: !1,
                         getBoundingRect: this.getBoundingRect
                     }), new M({
                         sdf: _.sdf,
-                        smoothing: Number.isFinite(_.smoothing) ? _.smoothing : L_.smoothing,
+                        smoothing: Number.isFinite(_.smoothing) ? _.smoothing : O_.smoothing,
                         outlineWidth: x,
                         outlineColor: w,
                         iconAtlas: r,
                         iconMapping: s,
                         getPosition: c,
                         getColor: h,
                         getSize: u,
@@ -26758,15 +26759,15 @@
                         numInstances: e,
                         getIconOffsets: this.getIconOffsets,
                         getIcon: n
                     })]
                 }
                 static set fontAtlasCacheLimit(t) {
                     ! function(t) {
-                        ta.assert(Number.isFinite(t) && t >= 3, "Invalid cache limit"), k_ = new O_(t)
+                        ta.assert(Number.isFinite(t) && t >= 3, "Invalid cache limit"), k_ = new L_(t)
                     }(t)
                 }
             }
             wo(U_, "defaultProps", V_), wo(U_, "layerName", "TextLayer");
             const G_ = {
                     circle: {
                         type: b_,
@@ -27003,19 +27004,19 @@
                 MultiPoint: 2,
                 LineString: 2,
                 MultiLineString: 3,
                 Polygon: 3,
                 MultiPolygon: 4
             };
 
-            function $_(t) {
+            function J_(t) {
                 return t.geometry.coordinates
             }
-            const J_ = ["points", "linestrings", "polygons"],
-                Q_ = {
+            const Q_ = ["points", "linestrings", "polygons"],
+                $_ = {
                     ...Z_(G_.circle),
                     ...Z_(G_.icon),
                     ...Z_(G_.text),
                     ...Z_(W_),
                     ...Z_(H_),
                     stroked: !0,
                     filled: !0,
@@ -27200,29 +27201,29 @@
                             },
                             {
                                 pointFeatures: i,
                                 lineFeatures: r,
                                 polygonFeatures: s,
                                 polygonOutlineFeatures: o
                             } = t;
-                        return n.points.data = i, n.points._dataDiff = e.pointFeatures && (() => e.pointFeatures), n.points.getPosition = $_, n.lines.data = r, n.lines._dataDiff = e.lineFeatures && (() => e.lineFeatures), n.lines.getPath = $_, n.polygons.data = s, n.polygons._dataDiff = e.polygonFeatures && (() => e.polygonFeatures), n.polygons.getPolygon = $_, n.polygonsOutline.data = o, n.polygonsOutline._dataDiff = e.polygonOutlineFeatures && (() => e.polygonOutlineFeatures), n.polygonsOutline.getPath = $_, n
+                        return n.points.data = i, n.points._dataDiff = e.pointFeatures && (() => e.pointFeatures), n.points.getPosition = J_, n.lines.data = r, n.lines._dataDiff = e.lineFeatures && (() => e.lineFeatures), n.lines.getPath = J_, n.polygons.data = s, n.polygons._dataDiff = e.polygonFeatures && (() => e.polygonFeatures), n.polygons.getPolygon = J_, n.polygonsOutline.data = o, n.polygonsOutline._dataDiff = e.polygonOutlineFeatures && (() => e.polygonOutlineFeatures), n.polygonsOutline.getPath = J_, n
                     }(r, s);
                     this.setState({
                         features: r,
                         featuresDiff: s,
                         layerProps: o
                     })
                 }
                 getPickingInfo(t) {
                     const e = super.getPickingInfo(t),
                         {
                             index: n,
                             sourceLayer: i
                         } = e;
-                    return e.featureType = J_.find((t => i.id.startsWith("".concat(this.id, "-").concat(t, "-")))), n >= 0 && i.id.startsWith("".concat(this.id, "-points-text")) && this.state.binary && (e.index = this.props.data.points.globalFeatureIds.value[n]), e
+                    return e.featureType = Q_.find((t => i.id.startsWith("".concat(this.id, "-").concat(t, "-")))), n >= 0 && i.id.startsWith("".concat(this.id, "-points-text")) && this.state.binary && (e.index = this.props.data.points.globalFeatureIds.value[n]), e
                 }
                 _updateAutoHighlight(t) {
                     const e = "".concat(this.id, "-points-"),
                         n = "points" === t.featureType;
                     for (const i of this.getSubLayers()) i.id.startsWith(e) === n && i.updateAutoHighlight(t)
                 }
                 _renderPolygonLayer() {
@@ -27331,15 +27332,15 @@
                                 return i
                             }(t, i, n) : null
                         }(i, r);
                         return t(s, n)
                     } : super.getSubLayerAccessor(t)
                 }
             }
-            wo(tx, "layerName", "GeoJsonLayer"), wo(tx, "defaultProps", Q_);
+            wo(tx, "layerName", "GeoJsonLayer"), wo(tx, "defaultProps", $_);
             class ex {
                 constructor(t) {
                     wo(this, "index", void 0), wo(this, "isVisible", void 0), wo(this, "isSelected", void 0), wo(this, "parent", void 0), wo(this, "children", void 0), wo(this, "content", void 0), wo(this, "state", void 0), wo(this, "layers", void 0), wo(this, "id", void 0), wo(this, "bbox", void 0), wo(this, "zoom", void 0), wo(this, "userData", void 0), wo(this, "_abortController", void 0), wo(this, "_loader", void 0), wo(this, "_loaderId", void 0), wo(this, "_isLoaded", void 0), wo(this, "_isCancelled", void 0), wo(this, "_needsReload", void 0), this.index = t, this.isVisible = !1, this.isSelected = !1, this.parent = null, this.children = [], this.content = null, this._loader = void 0, this._abortController = null, this._loaderId = 0, this._isLoaded = !1, this._isCancelled = !1, this._needsReload = !1
                 }
                 get data() {
                     return this.isLoading && this._loader ? this._loader.then((() => this.data)) : this.content
                 }
@@ -27416,30 +27417,30 @@
                     unitsPerMeter2: [0, 0, 0],
                     metersPerUnit: [24886.609375, 24886.609375, 24886.609375],
                     unitsPerDegree: [e, e, t],
                     unitsPerDegree2: [0, 0, 0],
                     degreesPerUnit: [1 / e, 1 / e, 24886.609375]
                 }
             }
-            class ax extends Fh {
+            class ax extends zh {
                 constructor(t = {}) {
                     const {
                         latitude: e = 0,
                         longitude: n = 0,
                         zoom: i = 0,
                         nearZMultiplier: r = .1,
                         farZMultiplier: s = 2,
                         resolution: o = 10
                     } = t;
                     let {
                         height: a,
                         altitude: l = 1.5
                     } = t;
                     a = a || 1, l = Math.max(.75, l);
-                    const c = (new Qc).lookAt({
+                    const c = (new $c).lookAt({
                             eye: [0, -l, 0],
                             up: [0, 0, 1]
                         }),
                         h = Math.pow(2, i);
                     c.rotateX(e * nx), c.rotateZ(-n * nx), c.scale(h / a);
                     const u = Math.atan(.5 / l),
                         d = 512 * h / a;
@@ -27524,19 +27525,19 @@
             }
 
             function lx(t, e) {
                 const n = qc([], e, t);
                 return Zc(n, n, 1 / n[3]), n
             }
             const cx = -1,
-                hx = new Oc,
-                ux = new Oc;
+                hx = new Lc,
+                ux = new Lc;
             class dx {
                 constructor(t = [0, 0, 0], e = [0, 0, 0], n) {
-                    wo(this, "center", void 0), wo(this, "halfDiagonal", void 0), wo(this, "minimum", void 0), wo(this, "maximum", void 0), n = n || hx.copy(t).add(e).scale(.5), this.center = new Oc(n), this.halfDiagonal = new Oc(e).subtract(this.center), this.minimum = new Oc(t), this.maximum = new Oc(e)
+                    wo(this, "center", void 0), wo(this, "halfDiagonal", void 0), wo(this, "minimum", void 0), wo(this, "maximum", void 0), n = n || hx.copy(t).add(e).scale(.5), this.center = new Lc(n), this.halfDiagonal = new Lc(e).subtract(this.center), this.minimum = new Lc(t), this.maximum = new Lc(e)
                 }
                 clone() {
                     return new dx(this.minimum, this.maximum, this.center)
                 }
                 equals(t) {
                     return this === t || Boolean(t) && this.minimum.equals(t.minimum) && this.maximum.equals(t.maximum)
                 }
@@ -27557,25 +27558,25 @@
                         {
                             halfDiagonal: n
                         } = this;
                     let i, r = 0;
                     return i = Math.abs(e.x) - n.x, i > 0 && (r += i * i), i = Math.abs(e.y) - n.y, i > 0 && (r += i * i), i = Math.abs(e.z) - n.z, i > 0 && (r += i * i), r
                 }
             }
-            const px = new Oc,
-                fx = new Oc;
+            const px = new Lc,
+                fx = new Lc;
             class gx {
                 constructor(t = [0, 0, 0], e = 0) {
-                    wo(this, "center", void 0), wo(this, "radius", void 0), this.radius = -0, this.center = new Oc, this.fromCenterRadius(t, e)
+                    wo(this, "center", void 0), wo(this, "radius", void 0), this.radius = -0, this.center = new Lc, this.fromCenterRadius(t, e)
                 }
                 fromCenterRadius(t, e) {
                     return this.center.from(t), this.radius = e, this
                 }
                 fromCornerPoints(t, e) {
-                    return e = px.from(e), this.center = (new Oc).from(t).add(e).scale(.5), this.radius = this.center.distance(e), this
+                    return e = px.from(e), this.center = (new Lc).from(t).add(e).scale(.5), this.radius = this.center.distance(e), this
                 }
                 equals(t) {
                     return this === t || Boolean(t) && this.center.equals(t.center) && this.radius === t.radius
                 }
                 clone() {
                     return new gx(this.center, this.radius)
                 }
@@ -27854,49 +27855,49 @@
                     o = e[3],
                     a = n[0],
                     l = n[1],
                     c = n[2],
                     h = n[3];
                 return t[0] = i * h + o * a + r * c - s * l, t[1] = r * h + o * l + s * a - i * c, t[2] = s * h + o * c + i * l - r * a, t[3] = o * h - i * a - r * l - s * c, t
             }
-            var Ax, Mx, Ox, Lx, kx = Zc,
-                Ix = function(t) {
+            var Ax, Mx, Lx, Ox, kx = Zc,
+                Rx = function(t) {
                     var e = t[0],
                         n = t[1],
                         i = t[2],
                         r = t[3];
                     return Math.hypot(e, n, i, r)
                 },
-                Rx = function(t) {
+                Ix = function(t) {
                     var e = t[0],
                         n = t[1],
                         i = t[2],
                         r = t[3];
                     return e * e + n * n + i * i + r * r
                 },
-                jx = (Ax = mc(), Mx = vc(1, 0, 0), Ox = vc(0, 1, 0), function(t, e, n) {
+                jx = (Ax = mc(), Mx = vc(1, 0, 0), Lx = vc(0, 1, 0), function(t, e, n) {
                     var i = bc(e, n);
-                    return i < -.999999 ? (yc(Ax, Mx, e), Pc(Ax) < 1e-6 && yc(Ax, Ox, e), function(t, e) {
+                    return i < -.999999 ? (yc(Ax, Mx, e), Pc(Ax) < 1e-6 && yc(Ax, Lx, e), function(t, e) {
                         var n = e[0],
                             i = e[1],
                             r = e[2],
                             s = n * n + i * i + r * r;
                         s > 0 && (s = 1 / Math.sqrt(s)), t[0] = e[0] * s, t[1] = e[1] * s, t[2] = e[2] * s
                     }(Ax, Ax), Cx(t, Ax, Math.PI), t) : i > .999999 ? (t[0] = 0, t[1] = 0, t[2] = 0, t[3] = 1, t) : (yc(Ax, e, n), t[0] = Ax[0], t[1] = Ax[1], t[2] = Ax[2], t[3] = 1 + i, function(t, e) {
                         var n = e[0],
                             i = e[1],
                             r = e[2],
                             s = e[3],
                             o = n * n + i * i + r * r + s * s;
                         return o > 0 && (o = 1 / Math.sqrt(o)), t[0] = n * o, t[1] = i * o, t[2] = r * o, t[3] = s * o, t
                     }(t, t))
                 });
-            Sx(), Sx(), Lx = new gc(9), gc != Float32Array && (Lx[1] = 0, Lx[2] = 0, Lx[3] = 0, Lx[5] = 0, Lx[6] = 0, Lx[7] = 0), Lx[0] = 1, Lx[4] = 1, Lx[8] = 1;
-            const zx = [0, 0, 0, 1];
-            class Fx extends cc {
+            Sx(), Sx(), Ox = new gc(9), gc != Float32Array && (Ox[1] = 0, Ox[2] = 0, Ox[3] = 0, Ox[5] = 0, Ox[6] = 0, Ox[7] = 0), Ox[0] = 1, Ox[4] = 1, Ox[8] = 1;
+            const Fx = [0, 0, 0, 1];
+            class zx extends cc {
                 constructor(t = 0, e = 0, n = 0, i = 1) {
                     super(-0, -0, -0, -0), Array.isArray(t) && 1 === arguments.length ? this.copy(t) : this.set(t, e, n, i)
                 }
                 copy(t) {
                     return this[0] = t[0], this[1] = t[1], this[2] = t[2], this[3] = t[3], this.check()
                 }
                 set(t, e, n, i) {
@@ -27953,18 +27954,18 @@
                 get w() {
                     return this[3]
                 }
                 set w(t) {
                     this[3] = hc(t)
                 }
                 len() {
-                    return Ix(this)
+                    return Rx(this)
                 }
                 lengthSquared() {
-                    return Rx(this)
+                    return Ix(this)
                 }
                 dot(t) {
                     return function(t, e) {
                         return t[0] * e[0] + t[1] * e[1] + t[2] * e[2] + t[3] * e[3]
                     }(this, t)
                 }
                 rotationTo(t, e) {
@@ -28059,15 +28060,15 @@
                     return kx(this, this, t), this.check()
                 }
                 slerp(t, e, n) {
                     let i, r, s;
                     switch (arguments.length) {
                         case 1:
                             ({
-                                start: i = zx,
+                                start: i = Fx,
                                 target: r,
                                 ratio: s
                             } = t);
                             break;
                         case 2:
                             i = this, r = t, s = e;
                             break;
@@ -28111,44 +28112,44 @@
                 premultiply(t) {
                     return this.multiplyLeft(t)
                 }
                 multiply(t) {
                     return this.multiplyRight(t)
                 }
             }
-            const Bx = new Oc,
-                Dx = new Oc,
-                Nx = new Oc,
-                Vx = new Oc,
-                Ux = new Oc,
-                Gx = new Oc,
-                Wx = new Oc;
+            const Bx = new Lc,
+                Dx = new Lc,
+                Nx = new Lc,
+                Vx = new Lc,
+                Ux = new Lc,
+                Gx = new Lc,
+                Wx = new Lc;
             class Hx {
                 constructor(t = [0, 0, 0], e = [0, 0, 0, 0, 0, 0, 0, 0, 0]) {
-                    wo(this, "center", void 0), wo(this, "halfAxes", void 0), this.center = (new Oc).from(t), this.halfAxes = new _x(e)
+                    wo(this, "center", void 0), wo(this, "halfAxes", void 0), this.center = (new Lc).from(t), this.halfAxes = new _x(e)
                 }
                 get halfSize() {
                     const t = this.halfAxes.getColumn(0),
                         e = this.halfAxes.getColumn(1),
                         n = this.halfAxes.getColumn(2);
-                    return [new Oc(t).len(), new Oc(e).len(), new Oc(n).len()]
+                    return [new Lc(t).len(), new Lc(e).len(), new Lc(n).len()]
                 }
                 get quaternion() {
                     const t = this.halfAxes.getColumn(0),
                         e = this.halfAxes.getColumn(1),
                         n = this.halfAxes.getColumn(2),
-                        i = new Oc(t).normalize(),
-                        r = new Oc(e).normalize(),
-                        s = new Oc(n).normalize();
-                    return (new Fx).fromMatrix3(new _x([...i, ...r, ...s]))
+                        i = new Lc(t).normalize(),
+                        r = new Lc(e).normalize(),
+                        s = new Lc(n).normalize();
+                    return (new zx).fromMatrix3(new _x([...i, ...r, ...s]))
                 }
                 fromCenterHalfSizeQuaternion(t, e, n) {
-                    const i = new Fx(n),
+                    const i = new zx(n),
                         r = (new _x).fromQuaternion(i);
-                    return r[0] = r[0] * e[0], r[1] = r[1] * e[0], r[2] = r[2] * e[0], r[3] = r[3] * e[1], r[4] = r[4] * e[1], r[5] = r[5] * e[1], r[6] = r[6] * e[2], r[7] = r[7] * e[2], r[8] = r[8] * e[2], this.center = (new Oc).from(t), this.halfAxes = r, this
+                    return r[0] = r[0] * e[0], r[1] = r[1] * e[0], r[2] = r[2] * e[0], r[3] = r[3] * e[1], r[4] = r[4] * e[1], r[5] = r[5] * e[1], r[6] = r[6] * e[2], r[7] = r[7] * e[2], r[8] = r[8] * e[2], this.center = (new Lc).from(t), this.halfAxes = r, this
                 }
                 clone() {
                     return new Hx(this.center, this.halfAxes)
                 }
                 equals(t) {
                     return this === t || Boolean(t) && this.center.equals(t.center) && this.halfAxes.equals(t.halfAxes)
                 }
@@ -28209,19 +28210,19 @@
                     const i = this.halfAxes.getColumn(2, Ux);
                     return i.transformAsPoint(t), this.halfAxes = new _x([...e, ...n, ...i]), this
                 }
                 getTransform() {
                     throw new Error("not implemented")
                 }
             }
-            const Zx = new Oc,
-                qx = new Oc;
+            const Zx = new Lc,
+                qx = new Lc;
             class Xx {
                 constructor(t = [0, 0, 1], e = 0) {
-                    wo(this, "normal", void 0), wo(this, "distance", void 0), this.normal = new Oc, this.distance = -0, this.fromNormalDistance(t, e)
+                    wo(this, "normal", void 0), wo(this, "distance", void 0), this.normal = new Lc, this.distance = -0, this.fromNormalDistance(t, e)
                 }
                 fromNormalDistance(t, e) {
                     return dc(Number.isFinite(e)), this.normal.from(t).normalize(), this.distance = e, this
                 }
                 fromPointNormal(t, e) {
                     t = Zx.from(t), this.normal.from(e).normalize();
                     const n = -this.normal.dot(t);
@@ -28247,19 +28248,19 @@
                 projectPointOntoPlane(t, e = [0, 0, 0]) {
                     t = Zx.from(t);
                     const n = this.getPointDistance(t),
                         i = qx.copy(this.normal).scale(n);
                     return t.subtract(i).to(e)
                 }
             }
-            const Yx = [new Oc([1, 0, 0]), new Oc([0, 1, 0]), new Oc([0, 0, 1])],
-                Kx = new Oc,
-                $x = new Oc;
-            new Xx(new Oc(1, 0, 0), 0);
-            class Jx {
+            const Yx = [new Lc([1, 0, 0]), new Lc([0, 1, 0]), new Lc([0, 0, 1])],
+                Kx = new Lc,
+                Jx = new Lc;
+            new Xx(new Lc(1, 0, 0), 0);
+            class Qx {
                 constructor(t = []) {
                     wo(this, "planes", void 0), this.planes = t
                 }
                 fromBoundingSphere(t) {
                     this.planes.length = 2 * Yx.length;
                     const e = t.center,
                         n = t.radius;
@@ -28267,15 +28268,15 @@
                     for (const t of Yx) {
                         let r = this.planes[i],
                             s = this.planes[i + 1];
                         r || (r = this.planes[i] = new Xx), s || (s = this.planes[i + 1] = new Xx);
                         const o = Kx.copy(t).scale(-n).add(e);
                         t.dot(o), r.fromPointNormal(o, t);
                         const a = Kx.copy(t).scale(n).add(e),
-                            l = $x.copy(t).negate();
+                            l = Jx.copy(t).negate();
                         l.dot(a), s.fromPointNormal(a, l), i += 2
                     }
                     return this
                 }
                 computeVisibility(t) {
                     let e = 1;
                     for (const n of this.planes) switch (t.intersectPlane(n)) {
@@ -28283,30 +28284,30 @@
                             return cx;
                         case 0:
                             e = 0
                     }
                     return e
                 }
                 computeVisibilityWithPlaneMask(t, e) {
-                    if (dc(Number.isFinite(e), "parentPlaneMask is required."), e === Jx.MASK_OUTSIDE || e === Jx.MASK_INSIDE) return e;
-                    let n = Jx.MASK_INSIDE;
+                    if (dc(Number.isFinite(e), "parentPlaneMask is required."), e === Qx.MASK_OUTSIDE || e === Qx.MASK_INSIDE) return e;
+                    let n = Qx.MASK_INSIDE;
                     const i = this.planes;
                     for (let r = 0; r < this.planes.length; ++r) {
                         const s = r < 31 ? 1 << r : 0;
                         if (r < 31 && 0 == (e & s)) continue;
                         const o = i[r],
                             a = t.intersectPlane(o);
-                        if (a === cx) return Jx.MASK_OUTSIDE;
+                        if (a === cx) return Qx.MASK_OUTSIDE;
                         0 === a && (n |= s)
                     }
                     return n
                 }
             }
-            wo(Jx, "MASK_OUTSIDE", 4294967295), wo(Jx, "MASK_INSIDE", 0), wo(Jx, "MASK_INDETERMINATE", 2147483647), new Oc, new Oc, new Oc, new Oc, new Oc, new Oc, new Oc, new Oc, new Oc, new Oc, new Oc, new Oc, new Oc, new Oc, new Oc, new Oc, new Oc, Math.PI;
-            const Qx = {
+            wo(Qx, "MASK_OUTSIDE", 4294967295), wo(Qx, "MASK_INSIDE", 0), wo(Qx, "MASK_INDETERMINATE", 2147483647), new Lc, new Lc, new Lc, new Lc, new Lc, new Lc, new Lc, new Lc, new Lc, new Lc, new Lc, new Lc, new Lc, new Lc, new Lc, new Lc, new Lc, Math.PI;
+            const $x = {
                     EPSILON1: .1,
                     EPSILON2: .01,
                     EPSILON3: .001,
                     EPSILON4: 1e-4,
                     EPSILON5: 1e-5,
                     EPSILON6: 1e-6,
                     EPSILON7: 1e-7,
@@ -28342,15 +28343,15 @@
                     const i = t[tw.getElementIndex(ow[n], sw[n])];
                     e += 2 * i * i
                 }
                 return Math.sqrt(e)
             }
 
             function lw(t, e) {
-                const n = Qx.EPSILON15;
+                const n = $x.EPSILON15;
                 let i = 0,
                     r = 1;
                 for (let e = 0; e < 3; ++e) {
                     const n = Math.abs(t[tw.getElementIndex(ow[e], sw[e])]);
                     n > i && (r = e, i = n)
                 }
                 const s = sw[r],
@@ -28360,19 +28361,19 @@
                 if (Math.abs(t[tw.getElementIndex(o, s)]) > n) {
                     const e = (t[tw.getElementIndex(o, o)] - t[tw.getElementIndex(s, s)]) / 2 / t[tw.getElementIndex(o, s)];
                     let n;
                     n = e < 0 ? -1 / (-e + Math.sqrt(1 + e * e)) : 1 / (e + Math.sqrt(1 + e * e)), a = 1 / Math.sqrt(1 + n * n), l = n * a
                 }
                 return _x.IDENTITY.to(e), e[tw.getElementIndex(s, s)] = e[tw.getElementIndex(o, o)] = a, e[tw.getElementIndex(o, s)] = l, e[tw.getElementIndex(s, o)] = -l, e
             }
-            const cw = new Oc,
-                hw = new Oc,
-                uw = new Oc,
-                dw = new Oc,
-                pw = new Oc,
+            const cw = new Lc,
+                hw = new Lc,
+                uw = new Lc,
+                dw = new Lc,
+                pw = new Lc,
                 fw = new _x,
                 gw = {
                     diagonal: new _x,
                     unitary: new _x
                 },
                 mw = 512,
                 vw = [
@@ -28447,17 +28448,17 @@
                         const e = this.z < 1 ? yw : this.z < 2 ? bw : vw,
                             i = [];
                         for (const r of e) {
                             const e = Tw(this.x + r[0], this.y + r[1], this.z);
                             e[2] = t[0], i.push(n(e)), t[0] !== t[1] && (e[2] = t[1], i.push(n(e)))
                         }
                         return function(t, e = new Hx) {
-                            if (!t || 0 === t.length) return e.halfAxes = new _x([0, 0, 0, 0, 0, 0, 0, 0, 0]), e.center = new Oc, e;
+                            if (!t || 0 === t.length) return e.halfAxes = new _x([0, 0, 0, 0, 0, 0, 0, 0, 0]), e.center = new Lc, e;
                             const n = t.length,
-                                i = new Oc(0, 0, 0);
+                                i = new Lc(0, 0, 0);
                             for (const e of t) i.add(e);
                             const r = 1 / n;
                             i.multiplyByScalar(r);
                             let s = 0,
                                 o = 0,
                                 a = 0,
                                 l = 0,
@@ -28469,15 +28470,15 @@
                             }
                             s *= r, o *= r, a *= r, l *= r, c *= r, h *= r;
                             const u = fw;
                             u[0] = s, u[1] = o, u[2] = a, u[3] = o, u[4] = l, u[5] = c, u[6] = a, u[7] = c, u[8] = h;
                             const {
                                 unitary: d
                             } = function(t, e = {}) {
-                                const n = Qx.EPSILON20;
+                                const n = $x.EPSILON20;
                                 let i = 0,
                                     r = 0;
                                 const s = ew,
                                     o = nw;
                                 s.identity(), o.copy(t);
                                 const a = n * function(t) {
                                     let e = 0;
@@ -28600,15 +28601,15 @@
                     left: s,
                     top: o,
                     right: a,
                     bottom: l
                 }
             }
 
-            function Ow({
+            function Lw({
                 viewport: t,
                 maxZoom: e,
                 minZoom: n,
                 zRange: i,
                 extent: r,
                 tileSize: s = xw,
                 modelMatrix: o,
@@ -28624,19 +28625,19 @@
                 let h = r;
                 return o && a && r && !t.isGeospatial && (h = Pw(r, o)), t.isGeospatial ? function(t, e, n, i) {
                     const r = t instanceof ax && t.resolution ? t.projectPosition : null,
                         s = Object.values(t.getFrustumPlanes()).map((({
                             normal: t,
                             distance: e
                         }) => new Xx(t.clone().negate(), e))),
-                        o = new Jx(s),
+                        o = new Qx(s),
                         a = t.distanceScales.unitsPerMeter[2],
                         l = n && n[0] * a || 0,
                         c = n && n[1] * a || 0,
-                        h = t instanceof If && t.pitch <= 60 ? e : 0;
+                        h = t instanceof Rf && t.pitch <= 60 ? e : 0;
                     if (i) {
                         const [t, e, n, r] = i, s = mh([t, r]), o = mh([n, e]);
                         i = [s[0], mw - s[1], o[0], mw - o[1]]
                     }
                     const u = new _w(0, 0, 0),
                         d = {
                             viewport: t,
@@ -28644,15 +28645,15 @@
                             cullingVolume: o,
                             elevationBounds: [l, c],
                             minZ: h,
                             maxZ: e,
                             bounds: i,
                             offset: 0
                         };
-                    if (u.update(d), t instanceof If && t.subViewports && t.subViewports.length > 1) {
+                    if (u.update(d), t instanceof Rf && t.subViewports && t.subViewports.length > 1) {
                         for (d.offset = -1; u.update(d) && !(--d.offset < -3););
                         for (d.offset = 1; u.update(d) && !(++d.offset > 3););
                     }
                     return u.getSelected()
                 }(t, c, i, r) : function(t, e, n, i, r) {
                     const s = function(t, e, n) {
                             let i;
@@ -28668,28 +28669,28 @@
                             x: t,
                             y: n,
                             z: e
                         });
                     return u
                 }(t, c, s, h || ww, a)
             }
-            var Lw = n(4155);
+            var Ow = n(4155);
 
             function kw() {
                 let t;
                 if ("undefined" != typeof window && window.performance) t = window.performance.now();
-                else if (void 0 !== Lw && Lw.hrtime) {
-                    const e = Lw.hrtime();
+                else if (void 0 !== Ow && Ow.hrtime) {
+                    const e = Ow.hrtime();
                     t = 1e3 * e[0] + e[1] / 1e6
                 } else t = Date.now();
                 return t
             }
-            class Iw {
+            class Rw {
                 constructor(t, e) {
-                    this.name = void 0, this.type = void 0, this.sampleSize = 1, this.time = 0, this.count = 0, this.samples = 0, this.lastTiming = 0, this.lastSampleTime = 0, this.lastSampleCount = 0, this._count = 0, this._time = 0, this._samples = 0, this._startTime = 0, this._timerPending = !1, this.name = t, this.type = e, this.reset()
+                    wo(this, "name", void 0), wo(this, "type", void 0), wo(this, "sampleSize", 1), wo(this, "time", 0), wo(this, "count", 0), wo(this, "samples", 0), wo(this, "lastTiming", 0), wo(this, "lastSampleTime", 0), wo(this, "lastSampleCount", 0), wo(this, "_count", 0), wo(this, "_time", 0), wo(this, "_samples", 0), wo(this, "_startTime", 0), wo(this, "_timerPending", !1), this.name = t, this.type = e, this.reset()
                 }
                 reset() {
                     return this.time = 0, this.count = 0, this.samples = 0, this.lastTiming = 0, this.lastSampleTime = 0, this.lastSampleCount = 0, this._count = 0, this._time = 0, this._samples = 0, this._startTime = 0, this._timerPending = !1, this
                 }
                 setSampleSize(t) {
                     return this.sampleSize = t, this
                 }
@@ -28732,17 +28733,17 @@
                 getHz() {
                     return this.time > 0 ? this.samples / (this.time / 1e3) : 0
                 }
                 _checkSampling() {
                     this._samples === this.sampleSize && (this.lastSampleTime = this._time, this.lastSampleCount = this._count, this.count += this._count, this.time += this._time, this.samples += this._samples, this._time = 0, this._count = 0, this._samples = 0)
                 }
             }
-            class Rw {
+            class Iw {
                 constructor(t) {
-                    this.id = void 0, this.stats = {}, this.id = t.id, this.stats = {}, this._initializeStats(t.stats), Object.seal(this)
+                    wo(this, "id", void 0), wo(this, "stats", {}), this.id = t.id, this.stats = {}, this._initializeStats(t.stats), Object.seal(this)
                 }
                 get(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "count";
                     return this._getOrCreate({
                         name: t,
                         type: e
                     })
@@ -28773,29 +28774,29 @@
                 }
                 _getOrCreate(t) {
                     const {
                         name: e,
                         type: n
                     } = t;
                     let i = this.stats[e];
-                    return i || (i = t instanceof Iw ? t : new Iw(e, n), this.stats[e] = i), i
+                    return i || (i = t instanceof Rw ? t : new Rw(e, n), this.stats[e] = i), i
                 }
             }
             const jw = {
                 id: "request-scheduler",
                 throttleRequests: !0,
                 maxRequests: 6
             };
-            class zw {
+            class Fw {
                 constructor() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     wo(this, "props", void 0), wo(this, "stats", void 0), wo(this, "activeRequestCount", 0), wo(this, "requestQueue", []), wo(this, "requestMap", new Map), wo(this, "deferredUpdate", null), this.props = {
                         ...jw,
                         ...t
-                    }, this.stats = new Rw({
+                    }, this.stats = new Iw({
                         id: this.props.id
                     }), this.stats.get("Queued Requests"), this.stats.get("Active Requests"), this.stats.get("Cancelled Requests"), this.stats.get("Queued Requests Ever"), this.stats.get("Active Requests Ever")
                 }
                 scheduleRequest(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : () => 0;
                     if (!this.props.throttleRequests) return Promise.resolve({
                         done: () => {}
@@ -28846,17 +28847,17 @@
                     }
                     t.sort(((t, e) => t.priority - e.priority))
                 }
                 _updateRequest(t) {
                     return t.priority = t.getPriority(t.handle), !(t.priority < 0 && (t.resolve(null), 1))
                 }
             }
-            const Fw = "best-available",
+            const zw = "best-available",
                 Bw = {
-                    [Fw]: function(t) {
+                    [zw]: function(t) {
                         for (const e of t) e.state = 0;
                         for (const e of t) e.isSelected && !Dw(e) && Nw(e);
                         for (const e of t) e.isVisible = Boolean(2 & e.state)
                     },
                     "no-overlap": function(t) {
                         for (const e of t) e.state = 0;
                         for (const e of t) e.isSelected && Dw(e);
@@ -28882,18 +28883,18 @@
                 for (const e of t.children) e.isLoaded || e.content ? e.state |= 2 : Nw(e)
             }
             const Vw = {
                 TilesetClass: class {
                     constructor(t) {
                         wo(this, "opts", void 0), wo(this, "_requestScheduler", void 0), wo(this, "_cache", void 0), wo(this, "_dirty", void 0), wo(this, "_tiles", void 0), wo(this, "_cacheByteSize", void 0), wo(this, "_viewport", void 0), wo(this, "_zRange", void 0), wo(this, "_selectedTiles", void 0), wo(this, "_frameNumber", void 0), wo(this, "_modelMatrix", void 0), wo(this, "_modelMatrixInverse", void 0), wo(this, "_maxZoom", void 0), wo(this, "_minZoom", void 0), wo(this, "onTileLoad", void 0), wo(this, "_getCullBounds", hf(Sw)), this.opts = t, this.onTileLoad = t => {
                             this.opts.onTileLoad(t), this.opts.maxCacheByteSize && (this._cacheByteSize += t.byteLength, this._resizeCache())
-                        }, this._requestScheduler = new zw({
+                        }, this._requestScheduler = new Fw({
                             maxRequests: t.maxRequests,
                             throttleRequests: t.maxRequests > 0
-                        }), this._cache = new Map, this._tiles = [], this._dirty = !1, this._cacheByteSize = 0, this._viewport = null, this._selectedTiles = null, this._frameNumber = 0, this._modelMatrix = new Qc, this._modelMatrixInverse = new Qc, this.setOptions(t)
+                        }), this._cache = new Map, this._tiles = [], this._dirty = !1, this._cacheByteSize = 0, this._viewport = null, this._selectedTiles = null, this._frameNumber = 0, this._modelMatrix = new $c, this._modelMatrixInverse = new $c, this.setOptions(t)
                     }
                     get tiles() {
                         return this._tiles
                     }
                     get selectedTiles() {
                         return this._selectedTiles
                     }
@@ -28916,15 +28917,15 @@
                             this._selectedTiles && this._selectedTiles.includes(e) ? e.setNeedsReload() : this._cache.delete(t)
                         }
                     }
                     update(t, {
                         zRange: e,
                         modelMatrix: n
                     } = {}) {
-                        const i = new Qc(n),
+                        const i = new $c(n),
                             r = !i.equals(this._modelMatrix);
                         if (this._viewport && t.equals(this._viewport) && lc(this._zRange, e) && !r) this.needsReload && (this._selectedTiles = this._selectedTiles.map((t => this._getTile(t.index, !0))));
                         else {
                             r && (this._modelMatrixInverse = i.clone().invert(), this._modelMatrix = i), this._viewport = t, this._zRange = e;
                             const n = this.getTileIndices({
                                 viewport: t,
                                 maxZoom: this._maxZoom,
@@ -28964,15 +28965,15 @@
                         modelMatrixInverse: s
                     }) {
                         const {
                             tileSize: o,
                             extent: a,
                             zoomOffset: l
                         } = this.opts;
-                        return Ow({
+                        return Lw({
                             viewport: t,
                             maxZoom: e,
                             minZoom: n,
                             zRange: i,
                             tileSize: o,
                             extent: a,
                             modelMatrix: r,
@@ -28998,15 +28999,15 @@
                         return {
                             x: Math.floor(t.x / 2),
                             y: Math.floor(t.y / 2),
                             z: t.z - 1
                         }
                     }
                     updateTileStates() {
-                        const t = this.opts.refinementStrategy || Fw,
+                        const t = this.opts.refinementStrategy || zw,
                             e = new Array(this._cache.size);
                         let n = 0;
                         for (const t of this._cache.values()) e[n++] = t.isVisible, t.isSelected = !1, t.isVisible = !1;
                         for (const t of this._selectedTiles) t.isSelected = !0, t.isVisible = !0;
                         ("function" == typeof t ? t : Bw[t])(Array.from(this._cache.values())), n = 0;
                         for (const t of this._cache.values())
                             if (e[n++] !== t.isVisible) return !0;
@@ -29113,15 +29114,15 @@
                     compare: !0
                 },
                 tileSize: 512,
                 maxZoom: null,
                 minZoom: 0,
                 maxCacheSize: null,
                 maxCacheByteSize: null,
-                refinementStrategy: Fw,
+                refinementStrategy: zw,
                 zRange: null,
                 maxRequests: 6,
                 zoomOffset: 0
             };
             class Uw extends ry {
                 initializeState() {
                     this.state = {
@@ -29613,15 +29614,15 @@
                 height: 0,
                 format: "uint8",
                 channels: [],
                 channelMapping: [],
                 activeChannels: 0
             };
             var Kw = Yw;
-            class $w extends Uw {
+            class Jw extends Uw {
                 constructor(t) {
                     super(t)
                 }
                 shouldUpdateState({
                     props: t,
                     oldProps: e,
                     context: n,
@@ -29681,24 +29682,24 @@
                         channels: this.props.channels,
                         activeChannels: t.data.channels,
                         channelMapping: this.props.channelMapping,
                         bounds: [oc(e, 0, t.extent[2]), oc(n, 0, t.extent[3]), oc(i, 0, t.extent[2]), oc(r, 0, t.extent[3])]
                     })
                 }
             }
-            $w.defaultProps = {
+            Jw.defaultProps = {
                 api: "",
                 namespace: "",
                 metadata: [],
                 channels: [],
                 channelRanges: [],
                 channelMapping: []
             };
-            var Jw = $w,
-                Qw = t => {
+            var Qw = Jw,
+                $w = t => {
                     const {
                         tooltipText: e,
                         children: n
                     } = t;
                     return (0, o.jsxs)("div", {
                         className: "BIV-Tooltip",
                         children: [n, (0, o.jsx)("div", {
@@ -29719,15 +29720,15 @@
                     }), [e]), a = (0, c.useMemo)((() => (t => {
                         if (void 0 === t) return "-";
                         const e = 100 * Math.pow(2, t);
                         return `${Math.floor(e)}%`
                     })(n)), [n]);
                     return (0, o.jsxs)("div", {
                         className: "BIV-ZoomControls",
-                        children: [(0, o.jsx)(Qw, {
+                        children: [(0, o.jsx)($w, {
                             tooltipText: "Zoom in +",
                             children: (0, o.jsx)("button", {
                                 className: "BIV-ZoomControls__button",
                                 onClick: r,
                                 children: (0, o.jsx)("svg", {
                                     width: "20",
                                     height: "20",
@@ -29737,15 +29738,15 @@
                                     children: (0, o.jsx)("path", {
                                         d: "M10.0261 18.3333C10.2671 18.3333 10.4851 18.2732 10.6803 18.1529C10.8754 18.0325 11.034 17.8776 11.156 17.6881C11.2749 17.4986 11.3344 17.2941 11.3344 17.0745V11.2949H17.0524C17.2811 11.2949 17.493 11.2362 17.6882 11.1189C17.8834 11.0016 18.0404 10.8452 18.1593 10.6497C18.2752 10.4542 18.3332 10.2376 18.3332 9.99999C18.3332 9.76538 18.2737 9.55182 18.1548 9.35931C18.0358 9.1638 17.8773 9.00589 17.679 8.88557C17.4808 8.76526 17.2673 8.7051 17.0386 8.7051H11.3161V2.93448C11.3161 2.70588 11.2551 2.49683 11.1331 2.30734C11.0112 2.11483 10.851 1.95992 10.6528 1.84262C10.4546 1.72531 10.235 1.66666 9.99412 1.66666C9.76235 1.66666 9.54736 1.72381 9.34914 1.83811C9.14786 1.95241 8.98776 2.10581 8.86883 2.29831C8.7499 2.48781 8.69043 2.69535 8.69043 2.92095V8.68705H2.95876C2.73309 8.68705 2.52343 8.74571 2.32979 8.86301C2.13156 8.98032 1.97146 9.13673 1.84948 9.33224C1.7275 9.52475 1.6665 9.7368 1.6665 9.96841C1.6665 10.206 1.72597 10.4211 1.8449 10.6136C1.96384 10.8061 2.12241 10.961 2.32064 11.0783C2.51581 11.1926 2.72547 11.2498 2.94961 11.2498H8.67671V17.0249C8.67671 17.2445 8.73465 17.4475 8.85053 17.634C8.96641 17.8205 9.12499 17.9739 9.32626 18.0942C9.52449 18.2115 9.73796 18.2702 9.96667 18.2702L10.0261 18.3333Z",
                                         fill: "black",
                                         fillOpacity: "0.7"
                                     })
                                 })
                             })
-                        }), (0, o.jsx)(Qw, {
+                        }), (0, o.jsx)($w, {
                             tooltipText: "Zoom out -",
                             children: (0, o.jsx)("button", {
                                 className: "BIV-ZoomControls__button",
                                 onClick: s,
                                 children: (0, o.jsxs)("svg", {
                                     width: "20",
                                     height: "20",
@@ -29771,15 +29772,15 @@
                                         })
                                     })]
                                 })
                             })
                         }), (0, o.jsx)("p", {
                             className: "BIV-ZoomControls__label",
                             children: a
-                        }), (0, o.jsx)(Qw, {
+                        }), (0, o.jsx)($w, {
                             tooltipText: "Reset zoom level",
                             children: (0, o.jsx)("button", {
                                 className: "BIV-ZoomControls__button",
                                 onClick: i,
                                 children: (0, o.jsx)("svg", {
                                     width: "20",
                                     height: "20",
@@ -29936,25 +29937,25 @@
                     return {
                         imageWidth: n,
                         imageHeight: i,
                         minimapZoom: r,
                         minimapWidth: Math.pow(2, r) * n - 2,
                         minimapHeight: Math.pow(2, r) * i - 2
                     }
-                }), [a.metadata]), g = (0, c.useMemo)((() => new Lg({
+                }), [a.metadata]), g = (0, c.useMemo)((() => new Og({
                     id: "main",
                     controller: {
                         scrollZoom: {
                             speed: .01,
                             smooth: !0
                         },
                         inertia: !0,
                         doubleClickZoom: !1
                     }
-                })), [Lg]), m = (0, c.useMemo)((() => eE((t => {
+                })), [Og]), m = (0, c.useMemo)((() => eE((t => {
                     l((e => ({
                         ...e,
                         ...t.viewState
                     })))
                 }), 200)), [eE]);
                 (0, c.useEffect)((() => {
                     a.loaded && v(a.target, a.width, a.height, a.zoom)
@@ -29989,42 +29990,42 @@
                         setZoom: t => {
                             l((e => ({
                                 ...e,
                                 zoom: t
                             })))
                         }
                     }), a.loaded && (0, o.jsxs)(iy, {
-                        views: [g, new Lg({
+                        views: [g, new Og({
                             id: "mini-map",
                             x: "30px",
                             y: "30px",
                             height: `${f}px`,
                             width: `${p}px`,
                             controller: !1,
                             viewState: {
                                 target: [h / 2, u / 2, 0],
                                 zoom: d
                             }
                         })],
-                        layers: [new Jw({
+                        layers: [new Qw({
                             id: "tiles-for-main",
                             tileSize: 1024,
                             minZoom: a.metadata[0].zoomLevel,
                             maxZoom: a.metadata.at(-1)?.zoomLevel,
                             coordinateSystem: Th.CARTESIAN,
                             extent: [0, 0, h, u],
                             metadata: a.metadata,
                             namespace: t.groupNamespace,
                             attribute: t.attributes.filter((t => !0 === t.visible))[0],
                             channels: t.channels,
                             channelRanges: t.channelRanges,
                             channelMapping: t.channelMapping,
                             api: t.client.config.apiKey,
                             basePath: t.basePath
-                        }), new Jw({
+                        }), new Qw({
                             id: "tiles-for-mini-map",
                             tileSize: 4096,
                             minZoom: a.metadata[0].zoomLevel,
                             maxZoom: a.metadata[0].zoomLevel,
                             coordinateSystem: Th.CARTESIAN,
                             extent: [0, 0, h, u],
                             metadata: a.metadata,
@@ -30055,17 +30056,17 @@
                         onViewStateChange: m,
                         initialViewState: {
                             target: a.target,
                             zoom: a.zoom,
                             minZoom: -2,
                             maxZoom: a.metadata.at(-1)?.zoomLevel ?? 0
                         },
-                        children: [(0, o.jsx)(Lg, {
+                        children: [(0, o.jsx)(Og, {
                             id: "main"
-                        }), (0, o.jsx)(Lg, {
+                        }), (0, o.jsx)(Og, {
                             id: "mini-map",
                             children: (0, o.jsx)("div", {
                                 className: "BioImageViewer-Viewer__minimap"
                             })
                         })]
                     }), (0, o.jsx)("div", {
                         style: {
@@ -30293,14 +30294,15 @@
                 dE = t => {
                     let e;
                     e = "string" == typeof t.rootElement ? document.getElementById(t.rootElement) : t.rootElement, l().render((0, o.jsx)(uE, {
                         errorHandler: t.onError,
                         children: (0, o.jsx)(cE, {
                             apiKey: t.apiKey,
                             groupID: t.groupID,
+                            baseGroup: t.baseGroup,
                             namespace: t.namespace,
                             onError: t.onError,
                             basePath: t.basePath,
                             onLoad: t.onLoad
                         })
                     }), e)
                 }
@@ -30743,68 +30745,68 @@
                     return t.indexOf(e) > -1
                 }
 
                 function M(t) {
                     return t.trim().split(/\s+/g)
                 }
 
-                function O(t, e, n) {
+                function L(t, e, n) {
                     if (t.indexOf && !n) return t.indexOf(e);
                     for (var i = 0; i < t.length;) {
                         if (n && t[i][n] == e || !n && t[i] === e) return i;
                         i++
                     }
                     return -1
                 }
 
-                function L(t) {
+                function O(t) {
                     return Array.prototype.slice.call(t, 0)
                 }
 
                 function k(t, e, n) {
                     for (var i = [], r = [], s = 0; s < t.length;) {
                         var o = e ? t[s][e] : t[s];
-                        O(r, o) < 0 && i.push(t[s]), r[s] = o, s++
+                        L(r, o) < 0 && i.push(t[s]), r[s] = o, s++
                     }
                     return n && (i = e ? i.sort((function(t, n) {
                         return t[e] > n[e]
                     })) : i.sort()), i
                 }
 
-                function I(t, e) {
+                function R(t, e) {
                     for (var n, i, r = e[0].toUpperCase() + e.slice(1), s = 0; s < c.length;) {
                         if ((i = (n = c[s]) ? n + r : e) in t) return i;
                         s++
                     }
                     return a
                 }
-                var R = 1;
+                var I = 1;
 
                 function j(t) {
                     var e = t.ownerDocument || t;
                     return e.defaultView || e.parentWindow || r
                 }
-                var z = "ontouchstart" in r,
-                    F = I(r, "PointerEvent") !== a,
-                    B = z && /mobile|tablet|ip(ad|hone|od)|android/i.test(navigator.userAgent),
+                var F = "ontouchstart" in r,
+                    z = R(r, "PointerEvent") !== a,
+                    B = F && /mobile|tablet|ip(ad|hone|od)|android/i.test(navigator.userAgent),
                     D = "touch",
                     N = "mouse",
                     V = 25,
                     U = 1,
                     G = 4,
                     W = 8,
                     H = 1,
                     Z = 2,
                     q = 4,
                     X = 8,
                     Y = 16,
                     K = Z | q,
-                    $ = X | Y,
-                    J = K | $,
-                    Q = ["x", "y"],
+                    J = X | Y,
+                    Q = K | J,
+                    $ = ["x", "y"],
                     tt = ["clientX", "clientY"];
 
                 function et(t, e) {
                     var n = this;
                     this.manager = t, this.callback = e, this.element = t.element, this.target = t.options.inputTarget, this.domHandler = function(e) {
                         E(t.options.enable, [t]) && n.handler(e)
                     }, this.init()
@@ -30894,22 +30896,22 @@
                 }
 
                 function ot(t, e) {
                     return t === e ? H : p(t) >= p(e) ? t < 0 ? Z : q : e < 0 ? X : Y
                 }
 
                 function at(t, e, n) {
-                    n || (n = Q);
+                    n || (n = $);
                     var i = e[n[0]] - t[n[0]],
                         r = e[n[1]] - t[n[1]];
                     return Math.sqrt(i * i + r * r)
                 }
 
                 function lt(t, e, n) {
-                    n || (n = Q);
+                    n || (n = $);
                     var i = e[n[0]] - t[n[0]],
                         r = e[n[1]] - t[n[1]];
                     return 180 * Math.atan2(r, i) / Math.PI
                 }
                 et.prototype = {
                     handler: function() {},
                     init: function() {
@@ -30964,15 +30966,15 @@
                     handler: function(t) {
                         var e = this.store,
                             n = !1,
                             i = t.type.toLowerCase().replace("ms", ""),
                             r = pt[i],
                             s = ft[t.pointerType] || t.pointerType,
                             o = s == D,
-                            a = O(e, t.pointerId, "pointerId");
+                            a = L(e, t.pointerId, "pointerId");
                         r & U && (0 === t.button || o) ? a < 0 && (e.push(t), a = e.length - 1) : r & (G | W) && (n = !0), a < 0 || (e[a] = t, this.callback(this.manager, r, {
                             pointers: e,
                             changedPointers: [t],
                             pointerType: s,
                             srcEvent: t
                         }), n && e.splice(a, 1))
                     }
@@ -30985,16 +30987,16 @@
                 };
 
                 function yt() {
                     this.evTarget = "touchstart", this.evWin = "touchstart touchmove touchend touchcancel", this.started = !1, et.apply(this, arguments)
                 }
 
                 function _t(t, e) {
-                    var n = L(t.touches),
-                        i = L(t.changedTouches);
+                    var n = O(t.touches),
+                        i = O(t.changedTouches);
                     return e & (G | W) && (n = k(n.concat(i), "identifier", !0)), [n, i]
                 }
                 x(yt, et, {
                     handler: function(t) {
                         var e = bt[t.type];
                         if (e === U && (this.started = !0), this.started) {
                             var n = _t.call(this, t, e);
@@ -31016,18 +31018,18 @@
                     wt = "touchstart touchmove touchend touchcancel";
 
                 function Et() {
                     this.evTarget = wt, this.targetIds = {}, et.apply(this, arguments)
                 }
 
                 function Pt(t, e) {
-                    var n = L(t.touches),
+                    var n = O(t.touches),
                         i = this.targetIds;
                     if (e & (2 | U) && 1 === n.length) return i[n[0].identifier] = !0, [n, n];
-                    var r, s, o = L(t.changedTouches),
+                    var r, s, o = O(t.changedTouches),
                         a = [],
                         l = this.target;
                     if (s = n.filter((function(t) {
                             return T(t.target, l)
                         })), e === U)
                         for (r = 0; r < s.length;) i[s[r].identifier] = !0, r++;
                     for (r = 0; r < o.length;) i[o[r].identifier] && a.push(o[r]), e & (G | W) && delete i[o[r].identifier], r++;
@@ -31092,80 +31094,80 @@
                             this.callback(t, e, n)
                         }
                     },
                     destroy: function() {
                         this.touch.destroy(), this.mouse.destroy()
                     }
                 });
-                var Ot = I(h.style, "touchAction"),
-                    Lt = Ot !== a,
+                var Lt = R(h.style, "touchAction"),
+                    Ot = Lt !== a,
                     kt = "compute",
-                    It = "auto",
-                    Rt = "manipulation",
+                    Rt = "auto",
+                    It = "manipulation",
                     jt = "none",
-                    zt = "pan-x",
-                    Ft = "pan-y",
+                    Ft = "pan-x",
+                    zt = "pan-y",
                     Bt = function() {
-                        if (!Lt) return !1;
+                        if (!Ot) return !1;
                         var t = {},
                             e = r.CSS && r.CSS.supports;
                         return ["auto", "manipulation", "pan-y", "pan-x", "pan-x pan-y", "none"].forEach((function(n) {
                             t[n] = !e || r.CSS.supports("touch-action", n)
                         })), t
                     }();
 
                 function Dt(t, e) {
                     this.manager = t, this.set(e)
                 }
                 Dt.prototype = {
                     set: function(t) {
-                        t == kt && (t = this.compute()), Lt && this.manager.element.style && Bt[t] && (this.manager.element.style[Ot] = t), this.actions = t.toLowerCase().trim()
+                        t == kt && (t = this.compute()), Ot && this.manager.element.style && Bt[t] && (this.manager.element.style[Lt] = t), this.actions = t.toLowerCase().trim()
                     },
                     update: function() {
                         this.set(this.manager.options.touchAction)
                     },
                     compute: function() {
                         var t = [];
                         return v(this.manager.recognizers, (function(e) {
                                 E(e.options.enable, [e]) && (t = t.concat(e.getTouchAction()))
                             })),
                             function(t) {
                                 if (A(t, jt)) return jt;
-                                var e = A(t, zt),
-                                    n = A(t, Ft);
-                                return e && n ? jt : e || n ? e ? zt : Ft : A(t, Rt) ? Rt : It
+                                var e = A(t, Ft),
+                                    n = A(t, zt);
+                                return e && n ? jt : e || n ? e ? Ft : zt : A(t, It) ? It : Rt
                             }(t.join(" "))
                     },
                     preventDefaults: function(t) {
                         var e = t.srcEvent,
                             n = t.offsetDirection;
                         if (this.manager.session.prevented) e.preventDefault();
                         else {
                             var i = this.actions,
                                 r = A(i, jt) && !Bt[jt],
-                                s = A(i, Ft) && !Bt[Ft],
-                                o = A(i, zt) && !Bt[zt];
+                                s = A(i, zt) && !Bt[zt],
+                                o = A(i, Ft) && !Bt[Ft];
                             if (r) {
                                 var a = 1 === t.pointers.length,
                                     l = t.distance < 2,
                                     c = t.deltaTime < 250;
                                 if (a && l && c) return
                             }
-                            if (!o || !s) return r || s && n & K || o && n & $ ? this.preventSrc(e) : void 0
+                            if (!o || !s) return r || s && n & K || o && n & J ? this.preventSrc(e) : void 0
                         }
                     },
                     preventSrc: function(t) {
                         this.manager.session.prevented = !0, t.preventDefault()
                     }
                 };
                 var Nt = 1,
                     Vt = 32;
 
                 function Ut(t) {
-                    this.options = l({}, this.defaults, t || {}), this.id = R++, this.manager = null, this.options.enable = P(this.options.enable, !0), this.state = Nt, this.simultaneous = {}, this.requireFail = []
+                    this.options = l({}, this.defaults, t || {}), this.id = I++, this.manager = null, this.options.enable = P(this.options.enable, !0), this.state = Nt, this.simultaneous = {}, this.requireFail = []
                 }
 
                 function Gt(t) {
                     return 16 & t ? "cancel" : 8 & t ? "end" : 4 & t ? "move" : 2 & t ? "start" : ""
                 }
 
                 function Wt(t) {
@@ -31193,37 +31195,37 @@
                     Ut.apply(this, arguments), this._timer = null, this._input = null
                 }
 
                 function Kt() {
                     Zt.apply(this, arguments)
                 }
 
-                function $t() {
+                function Jt() {
                     Zt.apply(this, arguments)
                 }
 
-                function Jt() {
+                function Qt() {
                     Ut.apply(this, arguments), this.pTime = !1, this.pCenter = !1, this._timer = null, this._input = null, this.count = 0
                 }
 
-                function Qt(t, e) {
-                    return (e = e || {}).recognizers = P(e.recognizers, Qt.defaults.preset), new te(t, e)
+                function $t(t, e) {
+                    return (e = e || {}).recognizers = P(e.recognizers, $t.defaults.preset), new te(t, e)
                 }
 
                 function te(t, e) {
-                    this.options = l({}, Qt.defaults, e || {}), this.options.inputTarget = this.options.inputTarget || t, this.handlers = {}, this.session = {}, this.recognizers = [], this.oldCssProps = {}, this.element = t, this.input = new(this.options.inputClass || (F ? vt : B ? Et : z ? Ct : dt))(this, nt), this.touchAction = new Dt(this, this.options.touchAction), ee(this, !0), v(this.options.recognizers, (function(t) {
+                    this.options = l({}, $t.defaults, e || {}), this.options.inputTarget = this.options.inputTarget || t, this.handlers = {}, this.session = {}, this.recognizers = [], this.oldCssProps = {}, this.element = t, this.input = new(this.options.inputClass || (z ? vt : B ? Et : F ? Ct : dt))(this, nt), this.touchAction = new Dt(this, this.options.touchAction), ee(this, !0), v(this.options.recognizers, (function(t) {
                         var e = this.add(new t[0](t[1]));
                         t[2] && e.recognizeWith(t[2]), t[3] && e.requireFailure(t[3])
                     }), this)
                 }
 
                 function ee(t, e) {
                     var n, i = t.element;
                     i.style && (v(t.options.cssProps, (function(r, s) {
-                        n = I(i.style, s), e ? (t.oldCssProps[n] = i.style[n], i.style[n] = r) : i.style[n] = t.oldCssProps[n] || ""
+                        n = R(i.style, s), e ? (t.oldCssProps[n] = i.style[n], i.style[n] = r) : i.style[n] = t.oldCssProps[n] || ""
                     })), e || (t.oldCssProps = {}))
                 }
                 Ut.prototype = {
                     defaults: {},
                     set: function(t) {
                         return l(this.options, t), this.manager && this.manager.touchAction.update(), this
                     },
@@ -31234,20 +31236,20 @@
                     },
                     dropRecognizeWith: function(t) {
                         return m(t, "dropRecognizeWith", this) || (t = Ht(t, this), delete this.simultaneous[t.id]), this
                     },
                     requireFailure: function(t) {
                         if (m(t, "requireFailure", this)) return this;
                         var e = this.requireFail;
-                        return -1 === O(e, t = Ht(t, this)) && (e.push(t), t.requireFailure(this)), this
+                        return -1 === L(e, t = Ht(t, this)) && (e.push(t), t.requireFailure(this)), this
                     },
                     dropRequireFailure: function(t) {
                         if (m(t, "dropRequireFailure", this)) return this;
                         t = Ht(t, this);
-                        var e = O(this.requireFail, t);
+                        var e = L(this.requireFail, t);
                         return e > -1 && this.requireFail.splice(e, 1), this
                     },
                     hasRequireFailures: function() {
                         return this.requireFail.length > 0
                     },
                     canRecognizeWith: function(t) {
                         return !!this.simultaneous[t.id]
@@ -31296,20 +31298,20 @@
                         return i && (n & W || !r) ? 16 | e : i || r ? n & G ? 8 | e : 2 & e ? 4 | e : 2 : Vt
                     }
                 }), x(qt, Zt, {
                     defaults: {
                         event: "pan",
                         threshold: 10,
                         pointers: 1,
-                        direction: J
+                        direction: Q
                     },
                     getTouchAction: function() {
                         var t = this.options.direction,
                             e = [];
-                        return t & K && e.push(Ft), t & $ && e.push(zt), e
+                        return t & K && e.push(zt), t & J && e.push(Ft), e
                     },
                     directionTest: function(t) {
                         var e = this.options,
                             n = !0,
                             i = t.distance,
                             r = t.direction,
                             s = t.deltaX,
@@ -31347,15 +31349,15 @@
                     defaults: {
                         event: "press",
                         pointers: 1,
                         time: 251,
                         threshold: 9
                     },
                     getTouchAction: function() {
-                        return [It]
+                        return [Rt]
                     },
                     process: function(t) {
                         var e = this.options,
                             n = t.pointers.length === e.pointers,
                             i = t.distance < e.threshold,
                             r = t.deltaTime > e.time;
                         if (this._input = t, !i || !n || t.eventType & (G | W) && !r) this.reset();
@@ -31379,45 +31381,45 @@
                     },
                     getTouchAction: function() {
                         return [jt]
                     },
                     attrTest: function(t) {
                         return this._super.attrTest.call(this, t) && (Math.abs(t.rotation) > this.options.threshold || 2 & this.state)
                     }
-                }), x($t, Zt, {
+                }), x(Jt, Zt, {
                     defaults: {
                         event: "swipe",
                         threshold: 10,
                         velocity: .3,
-                        direction: K | $,
+                        direction: K | J,
                         pointers: 1
                     },
                     getTouchAction: function() {
                         return qt.prototype.getTouchAction.call(this)
                     },
                     attrTest: function(t) {
                         var e, n = this.options.direction;
-                        return n & (K | $) ? e = t.overallVelocity : n & K ? e = t.overallVelocityX : n & $ && (e = t.overallVelocityY), this._super.attrTest.call(this, t) && n & t.offsetDirection && t.distance > this.options.threshold && t.maxPointers == this.options.pointers && p(e) > this.options.velocity && t.eventType & G
+                        return n & (K | J) ? e = t.overallVelocity : n & K ? e = t.overallVelocityX : n & J && (e = t.overallVelocityY), this._super.attrTest.call(this, t) && n & t.offsetDirection && t.distance > this.options.threshold && t.maxPointers == this.options.pointers && p(e) > this.options.velocity && t.eventType & G
                     },
                     emit: function(t) {
                         var e = Wt(t.offsetDirection);
                         e && this.manager.emit(this.options.event + e, t), this.manager.emit(this.options.event, t)
                     }
-                }), x(Jt, Ut, {
+                }), x(Qt, Ut, {
                     defaults: {
                         event: "tap",
                         pointers: 1,
                         taps: 1,
                         interval: 300,
                         time: 250,
                         threshold: 9,
                         posThreshold: 10
                     },
                     getTouchAction: function() {
-                        return [Rt]
+                        return [It]
                     },
                     process: function(t) {
                         var e = this.options,
                             n = t.pointers.length === e.pointers,
                             i = t.distance < e.threshold,
                             r = t.deltaTime < e.time;
                         if (this.reset(), t.eventType & U && 0 === this.count) return this.failTimeout();
@@ -31438,39 +31440,39 @@
                     },
                     reset: function() {
                         clearTimeout(this._timer)
                     },
                     emit: function() {
                         8 == this.state && (this._input.tapCount = this.count, this.manager.emit(this.options.event, this._input))
                     }
-                }), Qt.VERSION = "2.0.7", Qt.defaults = {
+                }), $t.VERSION = "2.0.7", $t.defaults = {
                     domEvents: !1,
                     touchAction: kt,
                     enable: !0,
                     inputTarget: null,
                     inputClass: null,
                     preset: [
                         [Kt, {
                             enable: !1
                         }],
                         [Xt, {
                                 enable: !1
                             },
                             ["rotate"]
                         ],
-                        [$t, {
+                        [Jt, {
                             direction: K
                         }],
                         [qt, {
                                 direction: K
                             },
                             ["swipe"]
                         ],
-                        [Jt],
-                        [Jt, {
+                        [Qt],
+                        [Qt, {
                                 event: "doubletap",
                                 taps: 2
                             },
                             ["tap"]
                         ],
                         [Yt]
                     ],
@@ -31511,15 +31513,15 @@
                         var e = this.get(t.options.event);
                         return e && this.remove(e), this.recognizers.push(t), t.manager = this, this.touchAction.update(), t
                     },
                     remove: function(t) {
                         if (m(t, "remove", this)) return this;
                         if (t = this.get(t)) {
                             var e = this.recognizers,
-                                n = O(e, t); - 1 !== n && (e.splice(n, 1), this.touchAction.update())
+                                n = L(e, t); - 1 !== n && (e.splice(n, 1), this.touchAction.update())
                         }
                         return this
                     },
                     on: function(t, e) {
                         if (t !== a && e !== a) {
                             var n = this.handlers;
                             return v(M(t), (function(t) {
@@ -31527,15 +31529,15 @@
                             })), this
                         }
                     },
                     off: function(t, e) {
                         if (t !== a) {
                             var n = this.handlers;
                             return v(M(t), (function(t) {
-                                e ? n[t] && n[t].splice(O(n[t], e), 1) : delete n[t]
+                                e ? n[t] && n[t].splice(L(n[t], e), 1) : delete n[t]
                             })), this
                         }
                     },
                     emit: function(t, e) {
                         this.options.domEvents && function(t, e) {
                             var n = s.createEvent("Event");
                             n.initEvent(t, !0, !0), n.gesture = e, e.target.dispatchEvent(n)
@@ -31547,15 +31549,15 @@
                             };
                             for (var i = 0; i < n.length;) n[i](e), i++
                         }
                     },
                     destroy: function() {
                         this.element && ee(this, !1), this.handlers = {}, this.session = {}, this.input.destroy(), this.element = null
                     }
-                }, l(Qt, {
+                }, l($t, {
                     INPUT_START: U,
                     INPUT_MOVE: 2,
                     INPUT_END: G,
                     INPUT_CANCEL: W,
                     STATE_POSSIBLE: Nt,
                     STATE_BEGAN: 2,
                     STATE_CHANGED: 4,
@@ -31565,43 +31567,43 @@
                     STATE_FAILED: Vt,
                     DIRECTION_NONE: H,
                     DIRECTION_LEFT: Z,
                     DIRECTION_RIGHT: q,
                     DIRECTION_UP: X,
                     DIRECTION_DOWN: Y,
                     DIRECTION_HORIZONTAL: K,
-                    DIRECTION_VERTICAL: $,
-                    DIRECTION_ALL: J,
+                    DIRECTION_VERTICAL: J,
+                    DIRECTION_ALL: Q,
                     Manager: te,
                     Input: et,
                     TouchAction: Dt,
                     TouchInput: Et,
                     MouseInput: dt,
                     PointerEventInput: vt,
                     TouchMouseInput: Ct,
                     SingleTouchInput: yt,
                     Recognizer: Ut,
                     AttrRecognizer: Zt,
-                    Tap: Jt,
+                    Tap: Qt,
                     Pan: qt,
-                    Swipe: $t,
+                    Swipe: Jt,
                     Pinch: Xt,
                     Rotate: Kt,
                     Press: Yt,
                     on: S,
                     off: C,
                     each: v,
                     merge: _,
                     extend: y,
                     assign: l,
                     inherit: x,
                     bindFn: w,
-                    prefixed: I
-                }), (void 0 !== r ? r : "undefined" != typeof self ? self : {}).Hammer = Qt, (i = function() {
-                    return Qt
+                    prefixed: R
+                }), (void 0 !== r ? r : "undefined" != typeof self ? self : {}).Hammer = $t, (i = function() {
+                    return $t
                 }.call(e, n, e, t)) === a || (t.exports = i)
             }(window, document)
         },
         2896: (t, e, n) => {
             "use strict";
             n.d(e, {
                 Z: () => l
@@ -31661,190 +31663,35 @@
             var r = "object" == typeof exports && exports && !exports.nodeType && exports,
                 s = r && t && !t.nodeType && t,
                 o = s && s.exports === r ? i.Z.Buffer : void 0;
             const a = (o ? o.isBuffer : void 0) || function() {
                 return !1
             }
         },
-        8552: (t, e, n) => {
-            var i = n(852)(n(5639), "DataView");
-            t.exports = i
-        },
-        1989: (t, e, n) => {
-            var i = n(1789),
-                r = n(401),
-                s = n(7667),
-                o = n(1327),
-                a = n(1866);
-
-            function l(t) {
-                var e = -1,
-                    n = null == t ? 0 : t.length;
-                for (this.clear(); ++e < n;) {
-                    var i = t[e];
-                    this.set(i[0], i[1])
-                }
-            }
-            l.prototype.clear = i, l.prototype.delete = r, l.prototype.get = s, l.prototype.has = o, l.prototype.set = a, t.exports = l
-        },
-        8407: (t, e, n) => {
-            var i = n(7040),
-                r = n(4125),
-                s = n(2117),
-                o = n(7529),
-                a = n(4705);
-
-            function l(t) {
-                var e = -1,
-                    n = null == t ? 0 : t.length;
-                for (this.clear(); ++e < n;) {
-                    var i = t[e];
-                    this.set(i[0], i[1])
-                }
-            }
-            l.prototype.clear = i, l.prototype.delete = r, l.prototype.get = s, l.prototype.has = o, l.prototype.set = a, t.exports = l
-        },
-        7071: (t, e, n) => {
-            var i = n(852)(n(5639), "Map");
-            t.exports = i
-        },
-        3369: (t, e, n) => {
-            var i = n(4785),
-                r = n(1285),
-                s = n(6e3),
-                o = n(9916),
-                a = n(5265);
-
-            function l(t) {
-                var e = -1,
-                    n = null == t ? 0 : t.length;
-                for (this.clear(); ++e < n;) {
-                    var i = t[e];
-                    this.set(i[0], i[1])
-                }
-            }
-            l.prototype.clear = i, l.prototype.delete = r, l.prototype.get = s, l.prototype.has = o, l.prototype.set = a, t.exports = l
-        },
-        3818: (t, e, n) => {
-            var i = n(852)(n(5639), "Promise");
-            t.exports = i
-        },
-        8525: (t, e, n) => {
-            var i = n(852)(n(5639), "Set");
-            t.exports = i
-        },
-        8668: (t, e, n) => {
-            var i = n(3369),
-                r = n(619),
-                s = n(2385);
-
-            function o(t) {
-                var e = -1,
-                    n = null == t ? 0 : t.length;
-                for (this.__data__ = new i; ++e < n;) this.add(t[e])
-            }
-            o.prototype.add = o.prototype.push = r, o.prototype.has = s, t.exports = o
-        },
-        6384: (t, e, n) => {
-            var i = n(8407),
-                r = n(7465),
-                s = n(3779),
-                o = n(7599),
-                a = n(4758),
-                l = n(4309);
-
-            function c(t) {
-                var e = this.__data__ = new i(t);
-                this.size = e.size
-            }
-            c.prototype.clear = r, c.prototype.delete = s, c.prototype.get = o, c.prototype.has = a, c.prototype.set = l, t.exports = c
-        },
-        2139: (t, e, n) => {
-            var i = n(5639).Symbol;
-            t.exports = i
-        },
-        1149: (t, e, n) => {
-            var i = n(5639).Uint8Array;
-            t.exports = i
-        },
-        577: (t, e, n) => {
-            var i = n(852)(n(5639), "WeakMap");
-            t.exports = i
-        },
         7412: t => {
             t.exports = function(t, e) {
                 for (var n = -1, i = null == t ? 0 : t.length; ++n < i && !1 !== e(t[n], n, t););
                 return t
             }
         },
-        4963: t => {
-            t.exports = function(t, e) {
-                for (var n = -1, i = null == t ? 0 : t.length, r = 0, s = []; ++n < i;) {
-                    var o = t[n];
-                    e(o, n, t) && (s[r++] = o)
-                }
-                return s
-            }
-        },
-        4636: (t, e, n) => {
-            var i = n(2545),
-                r = n(5694),
-                s = n(1469),
-                o = n(4144),
-                a = n(5776),
-                l = n(6719),
-                c = Object.prototype.hasOwnProperty;
-            t.exports = function(t, e) {
-                var n = s(t),
-                    h = !n && r(t),
-                    u = !n && !h && o(t),
-                    d = !n && !h && !u && l(t),
-                    p = n || h || u || d,
-                    f = p ? i(t.length, String) : [],
-                    g = f.length;
-                for (var m in t) !e && !c.call(t, m) || p && ("length" == m || u && ("offset" == m || "parent" == m) || d && ("buffer" == m || "byteLength" == m || "byteOffset" == m) || a(m, g)) || f.push(m);
-                return f
-            }
-        },
         9932: t => {
             t.exports = function(t, e) {
                 for (var n = -1, i = null == t ? 0 : t.length, r = Array(i); ++n < i;) r[n] = e(t[n], n, t);
                 return r
             }
         },
-        2488: t => {
-            t.exports = function(t, e) {
-                for (var n = -1, i = e.length, r = t.length; ++n < i;) t[r + n] = e[n];
-                return t
-            }
-        },
-        2908: t => {
-            t.exports = function(t, e) {
-                for (var n = -1, i = null == t ? 0 : t.length; ++n < i;)
-                    if (e(t[n], n, t)) return !0;
-                return !1
-            }
-        },
         4865: (t, e, n) => {
             var i = n(9465),
                 r = n(7813),
                 s = Object.prototype.hasOwnProperty;
             t.exports = function(t, e, n) {
                 var o = t[e];
                 s.call(t, e) && r(o, n) && (void 0 !== n || e in t) || i(t, e, n)
             }
         },
-        8470: (t, e, n) => {
-            var i = n(7813);
-            t.exports = function(t, e) {
-                for (var n = t.length; n--;)
-                    if (i(t[n][0], e)) return n;
-                return -1
-            }
-        },
         4037: (t, e, n) => {
             var i = n(8363),
                 r = n(3674);
             t.exports = function(t, e) {
                 return t && i(e, r(e), t)
             }
         },
@@ -31889,46 +31736,46 @@
                 w = n(2928),
                 E = n(3674),
                 P = n(1704),
                 S = "[object Arguments]",
                 C = "[object Function]",
                 T = "[object Object]",
                 A = {};
-            A[S] = A["[object Array]"] = A["[object ArrayBuffer]"] = A["[object DataView]"] = A["[object Boolean]"] = A["[object Date]"] = A["[object Float32Array]"] = A["[object Float64Array]"] = A["[object Int8Array]"] = A["[object Int16Array]"] = A["[object Int32Array]"] = A["[object Map]"] = A["[object Number]"] = A[T] = A["[object RegExp]"] = A["[object Set]"] = A["[object String]"] = A["[object Symbol]"] = A["[object Uint8Array]"] = A["[object Uint8ClampedArray]"] = A["[object Uint16Array]"] = A["[object Uint32Array]"] = !0, A["[object Error]"] = A[C] = A["[object WeakMap]"] = !1, t.exports = function t(e, n, M, O, L, k) {
-                var I, R = 1 & n,
+            A[S] = A["[object Array]"] = A["[object ArrayBuffer]"] = A["[object DataView]"] = A["[object Boolean]"] = A["[object Date]"] = A["[object Float32Array]"] = A["[object Float64Array]"] = A["[object Int8Array]"] = A["[object Int16Array]"] = A["[object Int32Array]"] = A["[object Map]"] = A["[object Number]"] = A[T] = A["[object RegExp]"] = A["[object Set]"] = A["[object String]"] = A["[object Symbol]"] = A["[object Uint8Array]"] = A["[object Uint8ClampedArray]"] = A["[object Uint16Array]"] = A["[object Uint32Array]"] = !0, A["[object Error]"] = A[C] = A["[object WeakMap]"] = !1, t.exports = function t(e, n, M, L, O, k) {
+                var R, I = 1 & n,
                     j = 2 & n,
-                    z = 4 & n;
-                if (M && (I = L ? M(e, O, L, k) : M(e)), void 0 !== I) return I;
+                    F = 4 & n;
+                if (M && (R = O ? M(e, L, O, k) : M(e)), void 0 !== R) return R;
                 if (!x(e)) return e;
-                var F = b(e);
-                if (F) {
-                    if (I = g(e), !R) return c(e, I)
+                var z = b(e);
+                if (z) {
+                    if (R = g(e), !I) return c(e, R)
                 } else {
                     var B = f(e),
                         D = B == C || "[object GeneratorFunction]" == B;
-                    if (y(e)) return l(e, R);
-                    if (B == T || B == S || D && !L) {
-                        if (I = j || D ? {} : v(e), !R) return j ? u(e, a(I, e)) : h(e, o(I, e))
+                    if (y(e)) return l(e, I);
+                    if (B == T || B == S || D && !O) {
+                        if (R = j || D ? {} : v(e), !I) return j ? u(e, a(R, e)) : h(e, o(R, e))
                     } else {
-                        if (!A[B]) return L ? e : {};
-                        I = m(e, B, R)
+                        if (!A[B]) return O ? e : {};
+                        R = m(e, B, I)
                     }
                 }
                 k || (k = new i);
                 var N = k.get(e);
                 if (N) return N;
-                k.set(e, I), w(e) ? e.forEach((function(i) {
-                    I.add(t(i, n, M, i, e, k))
+                k.set(e, R), w(e) ? e.forEach((function(i) {
+                    R.add(t(i, n, M, i, e, k))
                 })) : _(e) && e.forEach((function(i, r) {
-                    I.set(r, t(i, n, M, r, e, k))
+                    R.set(r, t(i, n, M, r, e, k))
                 }));
-                var V = F ? void 0 : (z ? j ? p : d : j ? P : E)(e);
+                var V = z ? void 0 : (F ? j ? p : d : j ? P : E)(e);
                 return r(V || e, (function(i, r) {
-                    V && (i = e[r = i]), s(I, r, t(i, n, M, r, e, k))
-                })), I
+                    V && (i = e[r = i]), s(R, r, t(i, n, M, r, e, k))
+                })), R
             }
         },
         3118: (t, e, n) => {
             var i = n(3218),
                 r = Object.create,
                 s = function() {
                     function t() {}
@@ -31962,88 +31809,19 @@
             var i = n(1811),
                 r = n(327);
             t.exports = function(t, e) {
                 for (var n = 0, s = (e = i(e, t)).length; null != t && n < s;) t = t[r(e[n++])];
                 return n && n == s ? t : void 0
             }
         },
-        8866: (t, e, n) => {
-            var i = n(2488),
-                r = n(1469);
-            t.exports = function(t, e, n) {
-                var s = e(t);
-                return r(t) ? s : i(s, n(t))
-            }
-        },
-        4239: (t, e, n) => {
-            var i = n(2139),
-                r = n(9607),
-                s = n(2333),
-                o = i ? i.toStringTag : void 0;
-            t.exports = function(t) {
-                return null == t ? void 0 === t ? "[object Undefined]" : "[object Null]" : o && o in Object(t) ? r(t) : s(t)
-            }
-        },
         13: t => {
             t.exports = function(t, e) {
                 return null != t && e in Object(t)
             }
         },
-        9454: (t, e, n) => {
-            var i = n(4239),
-                r = n(7005);
-            t.exports = function(t) {
-                return r(t) && "[object Arguments]" == i(t)
-            }
-        },
-        939: (t, e, n) => {
-            var i = n(2492),
-                r = n(7005);
-            t.exports = function t(e, n, s, o, a) {
-                return e === n || (null == e || null == n || !r(e) && !r(n) ? e != e && n != n : i(e, n, s, o, t, a))
-            }
-        },
-        2492: (t, e, n) => {
-            var i = n(6384),
-                r = n(7114),
-                s = n(8351),
-                o = n(6096),
-                a = n(4160),
-                l = n(1469),
-                c = n(4144),
-                h = n(6719),
-                u = "[object Arguments]",
-                d = "[object Array]",
-                p = "[object Object]",
-                f = Object.prototype.hasOwnProperty;
-            t.exports = function(t, e, n, g, m, v) {
-                var b = l(t),
-                    y = l(e),
-                    _ = b ? d : a(t),
-                    x = y ? d : a(e),
-                    w = (_ = _ == u ? p : _) == p,
-                    E = (x = x == u ? p : x) == p,
-                    P = _ == x;
-                if (P && c(t)) {
-                    if (!c(e)) return !1;
-                    b = !0, w = !1
-                }
-                if (P && !w) return v || (v = new i), b || h(t) ? r(t, e, n, g, m, v) : s(t, e, _, n, g, m, v);
-                if (!(1 & n)) {
-                    var S = w && f.call(t, "__wrapped__"),
-                        C = E && f.call(e, "__wrapped__");
-                    if (S || C) {
-                        var T = S ? t.value() : t,
-                            A = C ? e.value() : e;
-                        return v || (v = new i), m(T, A, n, g, v)
-                    }
-                }
-                return !!P && (v || (v = new i), o(t, e, n, g, m, v))
-            }
-        },
         5588: (t, e, n) => {
             var i = n(4160),
                 r = n(7005);
             t.exports = function(t) {
                 return r(t) && "[object Map]" == i(t)
             }
         },
@@ -32070,66 +31848,31 @@
                         if (s) var f = s(u, d, h, t, e, p);
                         if (!(void 0 === f ? r(d, u, 3, s, p) : f)) return !1
                     }
                 }
                 return !0
             }
         },
-        8458: (t, e, n) => {
-            var i = n(3560),
-                r = n(5346),
-                s = n(3218),
-                o = n(346),
-                a = /^\[object .+?Constructor\]$/,
-                l = Function.prototype,
-                c = Object.prototype,
-                h = l.toString,
-                u = c.hasOwnProperty,
-                d = RegExp("^" + h.call(u).replace(/[\\^$.*+?()[\]{}|]/g, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$");
-            t.exports = function(t) {
-                return !(!s(t) || r(t)) && (i(t) ? d : a).test(o(t))
-            }
-        },
         9221: (t, e, n) => {
             var i = n(4160),
                 r = n(7005);
             t.exports = function(t) {
                 return r(t) && "[object Set]" == i(t)
             }
         },
-        8749: (t, e, n) => {
-            var i = n(4239),
-                r = n(1780),
-                s = n(7005),
-                o = {};
-            o["[object Float32Array]"] = o["[object Float64Array]"] = o["[object Int8Array]"] = o["[object Int16Array]"] = o["[object Int32Array]"] = o["[object Uint8Array]"] = o["[object Uint8ClampedArray]"] = o["[object Uint16Array]"] = o["[object Uint32Array]"] = !0, o["[object Arguments]"] = o["[object Array]"] = o["[object ArrayBuffer]"] = o["[object Boolean]"] = o["[object DataView]"] = o["[object Date]"] = o["[object Error]"] = o["[object Function]"] = o["[object Map]"] = o["[object Number]"] = o["[object Object]"] = o["[object RegExp]"] = o["[object Set]"] = o["[object String]"] = o["[object WeakMap]"] = !1, t.exports = function(t) {
-                return s(t) && r(t.length) && !!o[i(t)]
-            }
-        },
         7206: (t, e, n) => {
             var i = n(1573),
                 r = n(6432),
                 s = n(6557),
                 o = n(1469),
                 a = n(9601);
             t.exports = function(t) {
                 return "function" == typeof t ? t : null == t ? s : "object" == typeof t ? o(t) ? r(t[0], t[1]) : i(t) : a(t)
             }
         },
-        280: (t, e, n) => {
-            var i = n(5726),
-                r = n(6916),
-                s = Object.prototype.hasOwnProperty;
-            t.exports = function(t) {
-                if (!i(t)) return r(t);
-                var e = [];
-                for (var n in Object(t)) s.call(t, n) && "constructor" != n && e.push(n);
-                return e
-            }
-        },
         313: (t, e, n) => {
             var i = n(3218),
                 r = n(5726),
                 s = n(3498),
                 o = Object.prototype.hasOwnProperty;
             t.exports = function(t) {
                 if (!i(t)) return s(t);
@@ -32187,47 +31930,29 @@
             var i = n(7786);
             t.exports = function(t) {
                 return function(e) {
                     return i(e, t)
                 }
             }
         },
-        2545: t => {
-            t.exports = function(t, e) {
-                for (var n = -1, i = Array(t); ++n < t;) i[n] = e(n);
-                return i
-            }
-        },
         531: (t, e, n) => {
-            var i = n(2139),
+            var i = n(2705),
                 r = n(9932),
                 s = n(1469),
                 o = n(3448),
                 a = i ? i.prototype : void 0,
                 l = a ? a.toString : void 0;
             t.exports = function t(e) {
                 if ("string" == typeof e) return e;
                 if (s(e)) return r(e, t) + "";
                 if (o(e)) return l ? l.call(e) : "";
                 var n = e + "";
                 return "0" == n && 1 / e == -1 / 0 ? "-0" : n
             }
         },
-        7518: t => {
-            t.exports = function(t) {
-                return function(e) {
-                    return t(e)
-                }
-            }
-        },
-        4757: t => {
-            t.exports = function(t, e) {
-                return t.has(e)
-            }
-        },
         4290: (t, e, n) => {
             var i = n(6557);
             t.exports = function(t) {
                 return "function" == typeof t ? t : i
             }
         },
         1811: (t, e, n) => {
@@ -32271,15 +31996,15 @@
             var e = /\w*$/;
             t.exports = function(t) {
                 var n = new t.constructor(t.source, e.exec(t));
                 return n.lastIndex = t.lastIndex, n
             }
         },
         419: (t, e, n) => {
-            var i = n(2139),
+            var i = n(2705),
                 r = i ? i.prototype : void 0,
                 s = r ? r.valueOf : void 0;
             t.exports = function(t) {
                 return s ? Object(s.call(t)) : {}
             }
         },
         7133: (t, e, n) => {
@@ -32321,18 +32046,14 @@
         1911: (t, e, n) => {
             var i = n(8363),
                 r = n(1442);
             t.exports = function(t, e) {
                 return i(t, r(t), e)
             }
         },
-        4429: (t, e, n) => {
-            var i = n(5639)["__core-js_shared__"];
-            t.exports = i
-        },
         9291: (t, e, n) => {
             var i = n(8612);
             t.exports = function(t, e) {
                 return function(n, r) {
                     if (null == n) return n;
                     if (!i(n)) return t(n, r);
                     for (var s = n.length, o = e ? s : -1, a = Object(n);
@@ -32358,263 +32079,45 @@
                     try {
                         var t = i(Object, "defineProperty");
                         return t({}, "", {}), t
                     } catch (t) {}
                 }();
             t.exports = r
         },
-        7114: (t, e, n) => {
-            var i = n(8668),
-                r = n(2908),
-                s = n(4757);
-            t.exports = function(t, e, n, o, a, l) {
-                var c = 1 & n,
-                    h = t.length,
-                    u = e.length;
-                if (h != u && !(c && u > h)) return !1;
-                var d = l.get(t),
-                    p = l.get(e);
-                if (d && p) return d == e && p == t;
-                var f = -1,
-                    g = !0,
-                    m = 2 & n ? new i : void 0;
-                for (l.set(t, e), l.set(e, t); ++f < h;) {
-                    var v = t[f],
-                        b = e[f];
-                    if (o) var y = c ? o(b, v, f, e, t, l) : o(v, b, f, t, e, l);
-                    if (void 0 !== y) {
-                        if (y) continue;
-                        g = !1;
-                        break
-                    }
-                    if (m) {
-                        if (!r(e, (function(t, e) {
-                                if (!s(m, e) && (v === t || a(v, t, n, o, l))) return m.push(e)
-                            }))) {
-                            g = !1;
-                            break
-                        }
-                    } else if (v !== b && !a(v, b, n, o, l)) {
-                        g = !1;
-                        break
-                    }
-                }
-                return l.delete(t), l.delete(e), g
-            }
-        },
-        8351: (t, e, n) => {
-            var i = n(2139),
-                r = n(1149),
-                s = n(7813),
-                o = n(7114),
-                a = n(8776),
-                l = n(1814),
-                c = i ? i.prototype : void 0,
-                h = c ? c.valueOf : void 0;
-            t.exports = function(t, e, n, i, c, u, d) {
-                switch (n) {
-                    case "[object DataView]":
-                        if (t.byteLength != e.byteLength || t.byteOffset != e.byteOffset) return !1;
-                        t = t.buffer, e = e.buffer;
-                    case "[object ArrayBuffer]":
-                        return !(t.byteLength != e.byteLength || !u(new r(t), new r(e)));
-                    case "[object Boolean]":
-                    case "[object Date]":
-                    case "[object Number]":
-                        return s(+t, +e);
-                    case "[object Error]":
-                        return t.name == e.name && t.message == e.message;
-                    case "[object RegExp]":
-                    case "[object String]":
-                        return t == e + "";
-                    case "[object Map]":
-                        var p = a;
-                    case "[object Set]":
-                        var f = 1 & i;
-                        if (p || (p = l), t.size != e.size && !f) return !1;
-                        var g = d.get(t);
-                        if (g) return g == e;
-                        i |= 2, d.set(t, e);
-                        var m = o(p(t), p(e), i, c, u, d);
-                        return d.delete(t), m;
-                    case "[object Symbol]":
-                        if (h) return h.call(t) == h.call(e)
-                }
-                return !1
-            }
-        },
-        6096: (t, e, n) => {
-            var i = n(8234),
-                r = Object.prototype.hasOwnProperty;
-            t.exports = function(t, e, n, s, o, a) {
-                var l = 1 & n,
-                    c = i(t),
-                    h = c.length;
-                if (h != i(e).length && !l) return !1;
-                for (var u = h; u--;) {
-                    var d = c[u];
-                    if (!(l ? d in e : r.call(e, d))) return !1
-                }
-                var p = a.get(t),
-                    f = a.get(e);
-                if (p && f) return p == e && f == t;
-                var g = !0;
-                a.set(t, e), a.set(e, t);
-                for (var m = l; ++u < h;) {
-                    var v = t[d = c[u]],
-                        b = e[d];
-                    if (s) var y = l ? s(b, v, d, e, t, a) : s(v, b, d, t, e, a);
-                    if (!(void 0 === y ? v === b || o(v, b, n, s, a) : y)) {
-                        g = !1;
-                        break
-                    }
-                    m || (m = "constructor" == d)
-                }
-                if (g && !m) {
-                    var _ = t.constructor,
-                        x = e.constructor;
-                    _ == x || !("constructor" in t) || !("constructor" in e) || "function" == typeof _ && _ instanceof _ && "function" == typeof x && x instanceof x || (g = !1)
-                }
-                return a.delete(t), a.delete(e), g
-            }
-        },
-        1957: (t, e, n) => {
-            var i = "object" == typeof n.g && n.g && n.g.Object === Object && n.g;
-            t.exports = i
-        },
-        8234: (t, e, n) => {
-            var i = n(8866),
-                r = n(9551),
-                s = n(3674);
-            t.exports = function(t) {
-                return i(t, s, r)
-            }
-        },
         6904: (t, e, n) => {
             var i = n(8866),
                 r = n(1442),
                 s = n(1704);
             t.exports = function(t) {
                 return i(t, s, r)
             }
         },
-        5050: (t, e, n) => {
-            var i = n(7019);
-            t.exports = function(t, e) {
-                var n = t.__data__;
-                return i(e) ? n["string" == typeof e ? "string" : "hash"] : n.map
-            }
-        },
         1499: (t, e, n) => {
             var i = n(9162),
                 r = n(3674);
             t.exports = function(t) {
                 for (var e = r(t), n = e.length; n--;) {
                     var s = e[n],
                         o = t[s];
                     e[n] = [s, o, i(o)]
                 }
                 return e
             }
         },
-        852: (t, e, n) => {
-            var i = n(8458),
-                r = n(7801);
-            t.exports = function(t, e) {
-                var n = r(t, e);
-                return i(n) ? n : void 0
-            }
-        },
-        5924: (t, e, n) => {
-            var i = n(5569)(Object.getPrototypeOf, Object);
-            t.exports = i
-        },
-        9607: (t, e, n) => {
-            var i = n(2139),
-                r = Object.prototype,
-                s = r.hasOwnProperty,
-                o = r.toString,
-                a = i ? i.toStringTag : void 0;
-            t.exports = function(t) {
-                var e = s.call(t, a),
-                    n = t[a];
-                try {
-                    t[a] = void 0;
-                    var i = !0
-                } catch (t) {}
-                var r = o.call(t);
-                return i && (e ? t[a] = n : delete t[a]), r
-            }
-        },
-        9551: (t, e, n) => {
-            var i = n(4963),
-                r = n(479),
-                s = Object.prototype.propertyIsEnumerable,
-                o = Object.getOwnPropertySymbols,
-                a = o ? function(t) {
-                    return null == t ? [] : (t = Object(t), i(o(t), (function(e) {
-                        return s.call(t, e)
-                    })))
-                } : r;
-            t.exports = a
-        },
         1442: (t, e, n) => {
             var i = n(2488),
                 r = n(5924),
                 s = n(9551),
                 o = n(479),
                 a = Object.getOwnPropertySymbols ? function(t) {
                     for (var e = []; t;) i(e, s(t)), t = r(t);
                     return e
                 } : o;
             t.exports = a
         },
-        4160: (t, e, n) => {
-            var i = n(8552),
-                r = n(7071),
-                s = n(3818),
-                o = n(8525),
-                a = n(577),
-                l = n(4239),
-                c = n(346),
-                h = "[object Map]",
-                u = "[object Promise]",
-                d = "[object Set]",
-                p = "[object WeakMap]",
-                f = "[object DataView]",
-                g = c(i),
-                m = c(r),
-                v = c(s),
-                b = c(o),
-                y = c(a),
-                _ = l;
-            (i && _(new i(new ArrayBuffer(1))) != f || r && _(new r) != h || s && _(s.resolve()) != u || o && _(new o) != d || a && _(new a) != p) && (_ = function(t) {
-                var e = l(t),
-                    n = "[object Object]" == e ? t.constructor : void 0,
-                    i = n ? c(n) : "";
-                if (i) switch (i) {
-                    case g:
-                        return f;
-                    case m:
-                        return h;
-                    case v:
-                        return u;
-                    case b:
-                        return d;
-                    case y:
-                        return p
-                }
-                return e
-            }), t.exports = _
-        },
-        7801: t => {
-            t.exports = function(t, e) {
-                return null == t ? void 0 : t[e]
-            }
-        },
         222: (t, e, n) => {
             var i = n(1811),
                 r = n(5694),
                 s = n(1469),
                 o = n(5776),
                 a = n(1780),
                 l = n(327);
@@ -32623,53 +32126,14 @@
                     var d = l(e[c]);
                     if (!(u = null != t && n(t, d))) break;
                     t = t[d]
                 }
                 return u || ++c != h ? u : !!(h = null == t ? 0 : t.length) && a(h) && o(d, h) && (s(t) || r(t))
             }
         },
-        1789: (t, e, n) => {
-            var i = n(4536);
-            t.exports = function() {
-                this.__data__ = i ? i(null) : {}, this.size = 0
-            }
-        },
-        401: t => {
-            t.exports = function(t) {
-                var e = this.has(t) && delete this.__data__[t];
-                return this.size -= e ? 1 : 0, e
-            }
-        },
-        7667: (t, e, n) => {
-            var i = n(4536),
-                r = Object.prototype.hasOwnProperty;
-            t.exports = function(t) {
-                var e = this.__data__;
-                if (i) {
-                    var n = e[t];
-                    return "__lodash_hash_undefined__" === n ? void 0 : n
-                }
-                return r.call(e, t) ? e[t] : void 0
-            }
-        },
-        1327: (t, e, n) => {
-            var i = n(4536),
-                r = Object.prototype.hasOwnProperty;
-            t.exports = function(t) {
-                var e = this.__data__;
-                return i ? void 0 !== e[t] : r.call(e, t)
-            }
-        },
-        1866: (t, e, n) => {
-            var i = n(4536);
-            t.exports = function(t, e) {
-                var n = this.__data__;
-                return this.size += this.has(t) ? 0 : 1, n[t] = i && void 0 === e ? "__lodash_hash_undefined__" : e, this
-            }
-        },
         3824: t => {
             var e = Object.prototype.hasOwnProperty;
             t.exports = function(t) {
                 var n = t.length,
                     i = new t.constructor(n);
                 return n && "string" == typeof t[0] && e.call(t, "index") && (i.index = t.index, i.input = t.input), i
             }
@@ -32717,142 +32181,31 @@
             var i = n(3118),
                 r = n(5924),
                 s = n(5726);
             t.exports = function(t) {
                 return "function" != typeof t.constructor || s(t) ? {} : i(r(t))
             }
         },
-        5776: t => {
-            var e = /^(?:0|[1-9]\d*)$/;
-            t.exports = function(t, n) {
-                var i = typeof t;
-                return !!(n = null == n ? 9007199254740991 : n) && ("number" == i || "symbol" != i && e.test(t)) && t > -1 && t % 1 == 0 && t < n
-            }
-        },
         5403: (t, e, n) => {
             var i = n(1469),
                 r = n(3448),
                 s = /\.|\[(?:[^[\]]*|(["'])(?:(?!\1)[^\\]|\\.)*?\1)\]/,
                 o = /^\w*$/;
             t.exports = function(t, e) {
                 if (i(t)) return !1;
                 var n = typeof t;
                 return !("number" != n && "symbol" != n && "boolean" != n && null != t && !r(t)) || o.test(t) || !s.test(t) || null != e && t in Object(e)
             }
         },
-        7019: t => {
-            t.exports = function(t) {
-                var e = typeof t;
-                return "string" == e || "number" == e || "symbol" == e || "boolean" == e ? "__proto__" !== t : null === t
-            }
-        },
-        5346: (t, e, n) => {
-            var i, r = n(4429),
-                s = (i = /[^.]+$/.exec(r && r.keys && r.keys.IE_PROTO || "")) ? "Symbol(src)_1." + i : "";
-            t.exports = function(t) {
-                return !!s && s in t
-            }
-        },
-        5726: t => {
-            var e = Object.prototype;
-            t.exports = function(t) {
-                var n = t && t.constructor;
-                return t === ("function" == typeof n && n.prototype || e)
-            }
-        },
         9162: (t, e, n) => {
             var i = n(3218);
             t.exports = function(t) {
                 return t == t && !i(t)
             }
         },
-        7040: t => {
-            t.exports = function() {
-                this.__data__ = [], this.size = 0
-            }
-        },
-        4125: (t, e, n) => {
-            var i = n(8470),
-                r = Array.prototype.splice;
-            t.exports = function(t) {
-                var e = this.__data__,
-                    n = i(e, t);
-                return !(n < 0 || (n == e.length - 1 ? e.pop() : r.call(e, n, 1), --this.size, 0))
-            }
-        },
-        2117: (t, e, n) => {
-            var i = n(8470);
-            t.exports = function(t) {
-                var e = this.__data__,
-                    n = i(e, t);
-                return n < 0 ? void 0 : e[n][1]
-            }
-        },
-        7529: (t, e, n) => {
-            var i = n(8470);
-            t.exports = function(t) {
-                return i(this.__data__, t) > -1
-            }
-        },
-        4705: (t, e, n) => {
-            var i = n(8470);
-            t.exports = function(t, e) {
-                var n = this.__data__,
-                    r = i(n, t);
-                return r < 0 ? (++this.size, n.push([t, e])) : n[r][1] = e, this
-            }
-        },
-        4785: (t, e, n) => {
-            var i = n(1989),
-                r = n(8407),
-                s = n(7071);
-            t.exports = function() {
-                this.size = 0, this.__data__ = {
-                    hash: new i,
-                    map: new(s || r),
-                    string: new i
-                }
-            }
-        },
-        1285: (t, e, n) => {
-            var i = n(5050);
-            t.exports = function(t) {
-                var e = i(this, t).delete(t);
-                return this.size -= e ? 1 : 0, e
-            }
-        },
-        6e3: (t, e, n) => {
-            var i = n(5050);
-            t.exports = function(t) {
-                return i(this, t).get(t)
-            }
-        },
-        9916: (t, e, n) => {
-            var i = n(5050);
-            t.exports = function(t) {
-                return i(this, t).has(t)
-            }
-        },
-        5265: (t, e, n) => {
-            var i = n(5050);
-            t.exports = function(t, e) {
-                var n = i(this, t),
-                    r = n.size;
-                return n.set(t, e), this.size += n.size == r ? 0 : 1, this
-            }
-        },
-        8776: t => {
-            t.exports = function(t) {
-                var e = -1,
-                    n = Array(t.size);
-                return t.forEach((function(t, i) {
-                    n[++e] = [i, t]
-                })), n
-            }
-        },
         6366: t => {
             t.exports = function(t, e) {
                 return function(n) {
                     return null != n && n[t] === e && (void 0 !== e || t in Object(n))
                 }
             }
         },
@@ -32862,118 +32215,22 @@
                 var e = i(t, (function(t) {
                         return 500 === n.size && n.clear(), t
                     })),
                     n = e.cache;
                 return e
             }
         },
-        4536: (t, e, n) => {
-            var i = n(852)(Object, "create");
-            t.exports = i
-        },
-        6916: (t, e, n) => {
-            var i = n(5569)(Object.keys, Object);
-            t.exports = i
-        },
         3498: t => {
             t.exports = function(t) {
                 var e = [];
                 if (null != t)
                     for (var n in Object(t)) e.push(n);
                 return e
             }
         },
-        1167: (t, e, n) => {
-            t = n.nmd(t);
-            var i = n(1957),
-                r = e && !e.nodeType && e,
-                s = r && t && !t.nodeType && t,
-                o = s && s.exports === r && i.process,
-                a = function() {
-                    try {
-                        return s && s.require && s.require("util").types || o && o.binding && o.binding("util")
-                    } catch (t) {}
-                }();
-            t.exports = a
-        },
-        2333: t => {
-            var e = Object.prototype.toString;
-            t.exports = function(t) {
-                return e.call(t)
-            }
-        },
-        5569: t => {
-            t.exports = function(t, e) {
-                return function(n) {
-                    return t(e(n))
-                }
-            }
-        },
-        5639: (t, e, n) => {
-            var i = n(1957),
-                r = "object" == typeof self && self && self.Object === Object && self,
-                s = i || r || Function("return this")();
-            t.exports = s
-        },
-        619: t => {
-            t.exports = function(t) {
-                return this.__data__.set(t, "__lodash_hash_undefined__"), this
-            }
-        },
-        2385: t => {
-            t.exports = function(t) {
-                return this.__data__.has(t)
-            }
-        },
-        1814: t => {
-            t.exports = function(t) {
-                var e = -1,
-                    n = Array(t.size);
-                return t.forEach((function(t) {
-                    n[++e] = t
-                })), n
-            }
-        },
-        7465: (t, e, n) => {
-            var i = n(8407);
-            t.exports = function() {
-                this.__data__ = new i, this.size = 0
-            }
-        },
-        3779: t => {
-            t.exports = function(t) {
-                var e = this.__data__,
-                    n = e.delete(t);
-                return this.size = e.size, n
-            }
-        },
-        7599: t => {
-            t.exports = function(t) {
-                return this.__data__.get(t)
-            }
-        },
-        4758: t => {
-            t.exports = function(t) {
-                return this.__data__.has(t)
-            }
-        },
-        4309: (t, e, n) => {
-            var i = n(8407),
-                r = n(7071),
-                s = n(3369);
-            t.exports = function(t, e) {
-                var n = this.__data__;
-                if (n instanceof i) {
-                    var o = n.__data__;
-                    if (!r || o.length < 199) return o.push([t, e]), this.size = ++n.size, this;
-                    n = this.__data__ = new s(o)
-                }
-                return n.set(t, e), this.size = n.size, this
-            }
-        },
         5514: (t, e, n) => {
             var i = n(4523),
                 r = /[^.[\]]+|\[(?:(-?\d+(?:\.\d+)?)|(["'])((?:(?!\2)[^\\]|\\.)*?)\2)\]|(?=(?:\.|\[\])(?:\.|\[\]|$))/g,
                 s = /\\(\\)?/g,
                 o = i((function(t) {
                     var e = [];
                     return 46 === t.charCodeAt(0) && e.push(""), t.replace(r, (function(t, n, i, r) {
@@ -32986,39 +32243,20 @@
             var i = n(3448);
             t.exports = function(t) {
                 if ("string" == typeof t || i(t)) return t;
                 var e = t + "";
                 return "0" == e && 1 / t == -1 / 0 ? "-0" : e
             }
         },
-        346: t => {
-            var e = Function.prototype.toString;
-            t.exports = function(t) {
-                if (null != t) {
-                    try {
-                        return e.call(t)
-                    } catch (t) {}
-                    try {
-                        return t + ""
-                    } catch (t) {}
-                }
-                return ""
-            }
-        },
         361: (t, e, n) => {
             var i = n(5990);
             t.exports = function(t) {
                 return i(t, 5)
             }
         },
-        7813: t => {
-            t.exports = function(t, e) {
-                return t === e || t != t && e != e
-            }
-        },
         2525: (t, e, n) => {
             var i = n(7816),
                 r = n(4290);
             t.exports = function(t, e) {
                 return t && i(t, r(e))
             }
         },
@@ -33037,101 +32275,25 @@
             }
         },
         6557: t => {
             t.exports = function(t) {
                 return t
             }
         },
-        5694: (t, e, n) => {
-            var i = n(9454),
-                r = n(7005),
-                s = Object.prototype,
-                o = s.hasOwnProperty,
-                a = s.propertyIsEnumerable,
-                l = i(function() {
-                    return arguments
-                }()) ? i : function(t) {
-                    return r(t) && o.call(t, "callee") && !a.call(t, "callee")
-                };
-            t.exports = l
-        },
-        1469: t => {
-            var e = Array.isArray;
-            t.exports = e
-        },
-        8612: (t, e, n) => {
-            var i = n(3560),
-                r = n(1780);
-            t.exports = function(t) {
-                return null != t && r(t.length) && !i(t)
-            }
-        },
-        4144: (t, e, n) => {
-            t = n.nmd(t);
-            var i = n(5639),
-                r = n(5062),
-                s = e && !e.nodeType && e,
-                o = s && t && !t.nodeType && t,
-                a = o && o.exports === s ? i.Buffer : void 0,
-                l = (a ? a.isBuffer : void 0) || r;
-            t.exports = l
-        },
-        3560: (t, e, n) => {
-            var i = n(4239),
-                r = n(3218);
-            t.exports = function(t) {
-                if (!r(t)) return !1;
-                var e = i(t);
-                return "[object Function]" == e || "[object GeneratorFunction]" == e || "[object AsyncFunction]" == e || "[object Proxy]" == e
-            }
-        },
-        1780: t => {
-            t.exports = function(t) {
-                return "number" == typeof t && t > -1 && t % 1 == 0 && t <= 9007199254740991
-            }
-        },
         6688: (t, e, n) => {
             var i = n(5588),
-                r = n(7518),
+                r = n(1717),
                 s = n(1167),
                 o = s && s.isMap,
                 a = o ? r(o) : i;
             t.exports = a
         },
-        3218: t => {
-            t.exports = function(t) {
-                var e = typeof t;
-                return null != t && ("object" == e || "function" == e)
-            }
-        },
-        7005: t => {
-            t.exports = function(t) {
-                return null != t && "object" == typeof t
-            }
-        },
-        8630: (t, e, n) => {
-            var i = n(4239),
-                r = n(5924),
-                s = n(7005),
-                o = Function.prototype,
-                a = Object.prototype,
-                l = o.toString,
-                c = a.hasOwnProperty,
-                h = l.call(Object);
-            t.exports = function(t) {
-                if (!s(t) || "[object Object]" != i(t)) return !1;
-                var e = r(t);
-                if (null === e) return !0;
-                var n = c.call(e, "constructor") && e.constructor;
-                return "function" == typeof n && n instanceof n && l.call(n) == h
-            }
-        },
         2928: (t, e, n) => {
             var i = n(9221),
-                r = n(7518),
+                r = n(1717),
                 s = n(1167),
                 o = s && s.isSet,
                 a = o ? r(o) : i;
             t.exports = a
         },
         7037: (t, e, n) => {
             var i = n(4239),
@@ -33144,30 +32306,14 @@
         3448: (t, e, n) => {
             var i = n(4239),
                 r = n(7005);
             t.exports = function(t) {
                 return "symbol" == typeof t || r(t) && "[object Symbol]" == i(t)
             }
         },
-        6719: (t, e, n) => {
-            var i = n(8749),
-                r = n(7518),
-                s = n(1167),
-                o = s && s.isTypedArray,
-                a = o ? r(o) : i;
-            t.exports = a
-        },
-        3674: (t, e, n) => {
-            var i = n(4636),
-                r = n(280),
-                s = n(8612);
-            t.exports = function(t) {
-                return s(t) ? i(t) : r(t)
-            }
-        },
         1704: (t, e, n) => {
             var i = n(4636),
                 r = n(313),
                 s = n(8612);
             t.exports = function(t) {
                 return s(t) ? i(t, !0) : r(t)
             }
@@ -33203,24 +32349,14 @@
                 r = n(9152),
                 s = n(5403),
                 o = n(327);
             t.exports = function(t) {
                 return s(t) ? i(o(t)) : r(t)
             }
         },
-        479: t => {
-            t.exports = function() {
-                return []
-            }
-        },
-        5062: t => {
-            t.exports = function() {
-                return !1
-            }
-        },
         9833: (t, e, n) => {
             var i = n(531);
             t.exports = function(t) {
                 return null == t ? "" : i(t)
             }
         },
         7418: t => {
```

### Comparing `tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/labextension/static/remoteEntry.555c16a49a97a15a2937.js` & `tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/labextension/static/remoteEntry.b197e4666f084e8dece0.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,305 +1,314 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, i, o, a, d, l, u, c, f, s, p, h, v, b, m, g, y = {
+    var e, r, t, a, n, i, o, l, d, u, c, f, s, p, h, b, v, m, g, y = {
             5290: (e, r, t) => {
-                var n = {
+                var a = {
                         "./index": () => t.e(744).then((() => () => t(1744))),
                         "./extension": () => t.e(744).then((() => () => t(1744))),
                         "./style": () => t.e(747).then((() => () => t(9747)))
                     },
-                    i = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    o = (e, r) => {
+                    i = (e, r) => {
                         if (t.S) {
-                            var n = "default",
-                                i = t.S[n];
-                            if (i && i !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
-                            return t.S[n] = e, t.I(n, r)
+                            var a = "default",
+                                n = t.S[a];
+                            if (n && n !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                            return t.S[a] = e, t.I(a, r)
                         }
                     };
                 t.d(r, {
-                    get: () => i,
-                    init: () => o
+                    get: () => n,
+                    init: () => i
                 })
             }
         },
         w = {};
 
-    function S(e) {
+    function j(e) {
         var r = w[e];
         if (void 0 !== r) return r.exports;
         var t = w[e] = {
             id: e,
             loaded: !1,
             exports: {}
         };
-        return y[e].call(t.exports, t, t.exports, S), t.loaded = !0, t.exports
+        return y[e].call(t.exports, t, t.exports, j), t.loaded = !0, t.exports
     }
-    S.m = y, S.c = w, S.n = e => {
+    j.m = y, j.c = w, j.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return S.d(r, {
+        return j.d(r, {
             a: r
         }), r
-    }, S.d = (e, r) => {
-        for (var t in r) S.o(r, t) && !S.o(e, t) && Object.defineProperty(e, t, {
+    }, j.d = (e, r) => {
+        for (var t in r) j.o(r, t) && !j.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
-        408: "635d4bfc76ee689544e0",
+    }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
+        38: "06c00f555d53e8ae5aa5",
+        172: "6267f3dd3063477e34ed",
+        408: "bdb74ff9f40e9eef1c08",
         446: "3bf34f45c93ace9c0f28",
-        635: "b2bedc962bcd82714540",
-        744: "23211eab87ca12d5bb82",
+        635: "f8f404497739316e801c",
+        713: "44bebcfa12a45c30ff83",
+        744: "6ac09e98bdf01bd3b6d1",
         747: "433530952542f03ebc71",
-        774: "a940595120cb008c0c58"
+        774: "309d750794b6276f460a"
     } [e] + ".js?v=" + {
-        408: "635d4bfc76ee689544e0",
+        38: "06c00f555d53e8ae5aa5",
+        172: "6267f3dd3063477e34ed",
+        408: "bdb74ff9f40e9eef1c08",
         446: "3bf34f45c93ace9c0f28",
-        635: "b2bedc962bcd82714540",
-        744: "23211eab87ca12d5bb82",
+        635: "f8f404497739316e801c",
+        713: "44bebcfa12a45c30ff83",
+        744: "6ac09e98bdf01bd3b6d1",
         747: "433530952542f03ebc71",
-        774: "a940595120cb008c0c58"
-    } [e], S.g = function() {
+        774: "309d750794b6276f460a"
+    } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), S.hmd = e => ((e = Object.create(e)).children || (e.children = []), Object.defineProperty(e, "exports", {
+    }(), j.hmd = e => ((e = Object.create(e)).children || (e.children = []), Object.defineProperty(e, "exports", {
         enumerable: !0,
         set: () => {
             throw new Error("ES Modules may not assign module.exports or exports.*, Use ESM export syntax, instead: " + e.id)
         }
-    }), e), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@tiledb-inc/jupyter-bioimage-viewer:", S.l = (t, n, i, o) => {
-        if (e[t]) e[t].push(n);
+    }), e), j.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@tiledb-inc/jupyter-bioimage-viewer:", j.l = (t, a, n, i) => {
+        if (e[t]) e[t].push(a);
         else {
-            var a, d;
-            if (void 0 !== i)
-                for (var l = document.getElementsByTagName("script"), u = 0; u < l.length; u++) {
-                    var c = l[u];
-                    if (c.getAttribute("src") == t || c.getAttribute("data-webpack") == r + i) {
-                        a = c;
+            var o, l;
+            if (void 0 !== n)
+                for (var d = document.getElementsByTagName("script"), u = 0; u < d.length; u++) {
+                    var c = d[u];
+                    if (c.getAttribute("src") == t || c.getAttribute("data-webpack") == r + n) {
+                        o = c;
                         break
                     }
                 }
-            a || (d = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, S.nc && a.setAttribute("nonce", S.nc), a.setAttribute("data-webpack", r + i), a.src = t), e[t] = [n];
-            var f = (r, n) => {
-                    a.onerror = a.onload = null, clearTimeout(s);
-                    var i = e[t];
-                    if (delete e[t], a.parentNode && a.parentNode.removeChild(a), i && i.forEach((e => e(n))), r) return r(n)
+            o || (l = !0, (o = document.createElement("script")).charset = "utf-8", o.timeout = 120, j.nc && o.setAttribute("nonce", j.nc), o.setAttribute("data-webpack", r + n), o.src = t), e[t] = [a];
+            var f = (r, a) => {
+                    o.onerror = o.onload = null, clearTimeout(s);
+                    var n = e[t];
+                    if (delete e[t], o.parentNode && o.parentNode.removeChild(o), n && n.forEach((e => e(a))), r) return r(a)
                 },
                 s = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
-                    target: a
+                    target: o
                 }), 12e4);
-            a.onerror = f.bind(null, a.onerror), a.onload = f.bind(null, a.onload), d && document.head.appendChild(a)
+            o.onerror = f.bind(null, o.onerror), o.onload = f.bind(null, o.onload), l && document.head.appendChild(o)
         }
-    }, S.r = e => {
+    }, j.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
-    }, S.nmd = e => (e.paths = [], e.children || (e.children = []), e), (() => {
-        S.S = {};
+    }, j.nmd = e => (e.paths = [], e.children || (e.children = []), e), (() => {
+        j.S = {};
         var e = {},
             r = {};
-        S.I = (t, n) => {
-            n || (n = []);
-            var i = r[t];
-            if (i || (i = r[t] = {}), !(n.indexOf(i) >= 0)) {
-                if (n.push(i), e[t]) return e[t];
-                S.o(S.S, t) || (S.S[t] = {});
-                var o = S.S[t],
-                    a = "@tiledb-inc/jupyter-bioimage-viewer",
-                    d = (e, r, t, n) => {
-                        var i = o[e] = o[e] || {},
-                            d = i[r];
-                        (!d || !d.loaded && (!n != !d.eager ? n : a > d.from)) && (i[r] = {
+        j.I = (t, a) => {
+            a || (a = []);
+            var n = r[t];
+            if (n || (n = r[t] = {}), !(a.indexOf(n) >= 0)) {
+                if (a.push(n), e[t]) return e[t];
+                j.o(j.S, t) || (j.S[t] = {});
+                var i = j.S[t],
+                    o = "@tiledb-inc/jupyter-bioimage-viewer",
+                    l = (e, r, t, a) => {
+                        var n = i[e] = i[e] || {},
+                            l = n[r];
+                        (!l || !l.loaded && (!a != !l.eager ? a : o > l.from)) && (n[r] = {
                             get: t,
-                            from: a,
-                            eager: !!n
+                            from: o,
+                            eager: !!a
                         })
                     },
-                    l = [];
-                return "default" === t && (d("@tiledb-inc/bioimage-viewer", "0.1.0-alpha.8", (() => Promise.all([S.e(635), S.e(774), S.e(446)]).then((() => () => S(3774))))), d("@tiledb-inc/jupyter-bioimage-viewer", "0.1.2-alpha.1", (() => S.e(744).then((() => () => S(1744)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                    d = [];
+                return "default" === t && (l("@jupyter-widgets/base", "4.1.1", (() => Promise.all([j.e(172), j.e(713), j.e(38)]).then((() => () => j(2713))))), l("@tiledb-inc/bioimage-viewer", "0.1.1-beta.0", (() => Promise.all([j.e(635), j.e(172), j.e(774), j.e(446)]).then((() => () => j(3774))))), l("@tiledb-inc/jupyter-bioimage-viewer", "0.1.2-alpha.2", (() => j.e(744).then((() => () => j(1744)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        S.g.importScripts && (e = S.g.location + "");
-        var r = S.g.document;
+        j.g.importScripts && (e = j.g.location + "");
+        var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
             if (t.length)
-                for (var n = t.length - 1; n > -1 && !e;) e = t[n--].src
+                for (var a = t.length - 1; a > -1 && !e;) e = t[a--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), S.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), j.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
-            n = t[1] ? r(t[1]) : [];
-        return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
-    }, n = (e, r) => {
+            a = t[1] ? r(t[1]) : [];
+        return t[2] && (a.length++, a.push.apply(a, r(t[2]))), t[3] && (a.push([]), a.push.apply(a, r(t[3]))), a
+    }, a = (e, r) => {
         e = t(e), r = t(r);
-        for (var n = 0;;) {
-            if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
-            var i = e[n],
-                o = (typeof i)[0];
-            if (n >= r.length) return "u" == o;
-            var a = r[n],
-                d = (typeof a)[0];
-            if (o != d) return "o" == o && "n" == d || "s" == d || "u" == o;
-            if ("o" != o && "u" != o && i != a) return i < a;
-            n++
+        for (var a = 0;;) {
+            if (a >= e.length) return a < r.length && "u" != (typeof r[a])[0];
+            var n = e[a],
+                i = (typeof n)[0];
+            if (a >= r.length) return "u" == i;
+            var o = r[a],
+                l = (typeof o)[0];
+            if (i != l) return "o" == i && "n" == l || "s" == l || "u" == i;
+            if ("o" != i && "u" != i && n != o) return n < o;
+            a++
         }
-    }, i = e => {
+    }, n = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(d = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, d);
+            for (var a = 1, i = 1; i < e.length; i++) a--, t += "u" == (typeof(l = e[i]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, l);
             return t
         }
-        var a = [];
-        for (o = 1; o < e.length; o++) {
-            var d = e[o];
-            a.push(0 === d ? "not(" + l() + ")" : 1 === d ? "(" + l() + " || " + l() + ")" : 2 === d ? a.pop() + " " + a.pop() : i(d))
+        var o = [];
+        for (i = 1; i < e.length; i++) {
+            var l = e[i];
+            o.push(0 === l ? "not(" + d() + ")" : 1 === l ? "(" + d() + " || " + d() + ")" : 2 === l ? o.pop() + " " + o.pop() : n(l))
         }
-        return l();
+        return d();
 
-        function l() {
-            return a.pop().replace(/^\((.+)\)$/, "$1")
+        function d() {
+            return o.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, o = (e, r) => {
+    }, i = (e, r) => {
         if (0 in e) {
             r = t(r);
-            var n = e[0],
-                i = n < 0;
-            i && (n = -n - 1);
-            for (var a = 0, d = 1, l = !0;; d++, a++) {
-                var u, c, f = d < e.length ? (typeof e[d])[0] : "";
-                if (a >= r.length || "o" == (c = (typeof(u = r[a]))[0])) return !l || ("u" == f ? d > n && !i : "" == f != i);
+            var a = e[0],
+                n = a < 0;
+            n && (a = -a - 1);
+            for (var o = 0, l = 1, d = !0;; l++, o++) {
+                var u, c, f = l < e.length ? (typeof e[l])[0] : "";
+                if (o >= r.length || "o" == (c = (typeof(u = r[o]))[0])) return !d || ("u" == f ? l > a && !n : "" == f != n);
                 if ("u" == c) {
-                    if (!l || "u" != f) return !1
-                } else if (l)
+                    if (!d || "u" != f) return !1
+                } else if (d)
                     if (f == c)
-                        if (d <= n) {
-                            if (u != e[d]) return !1
+                        if (l <= a) {
+                            if (u != e[l]) return !1
                         } else {
-                            if (i ? u > e[d] : u < e[d]) return !1;
-                            u != e[d] && (l = !1)
+                            if (n ? u > e[l] : u < e[l]) return !1;
+                            u != e[l] && (d = !1)
                         }
                 else if ("s" != f && "n" != f) {
-                    if (i || d <= n) return !1;
-                    l = !1, d--
+                    if (n || l <= a) return !1;
+                    d = !1, l--
                 } else {
-                    if (d <= n || c < f != i) return !1;
-                    l = !1
-                } else "s" != f && "n" != f && (l = !1, d--)
+                    if (l <= a || c < f != n) return !1;
+                    d = !1
+                } else "s" != f && "n" != f && (d = !1, l--)
             }
         }
         var s = [],
             p = s.pop.bind(s);
-        for (a = 1; a < e.length; a++) {
-            var h = e[a];
-            s.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
+        for (o = 1; o < e.length; o++) {
+            var h = e[o];
+            s.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? i(h, r) : !p())
         }
         return !!p()
-    }, a = (e, r) => {
-        var t = S.S[e];
-        if (!t || !S.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+    }, o = (e, r) => {
+        var t = j.S[e];
+        if (!t || !j.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
-    }, d = (e, r) => {
+    }, l = (e, r) => {
         var t = e[r];
-        return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + i(n) + ")", u = (e, r, t, n) => {
-        var i = d(e, t);
-        return o(n, i) || f(l(e, t, i, n)), s(e[t][i])
+        return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
+    }, d = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", u = (e, r, t, a) => {
+        var n = l(e, t);
+        return i(a, n) || f(d(e, t, n, a)), s(e[t][n])
     }, c = (e, r, t) => {
-        var i = e[r];
-        return (r = Object.keys(i).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && i[r]
+        var n = e[r];
+        return (r = Object.keys(n).reduce(((e, r) => !i(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
     }, f = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, s = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, i) {
-        var o = S.I(r);
-        return o && o.then ? o.then(e.bind(e, r, S.S[r], t, n, i)) : e(r, S.S[r], t, n, i)
-    })(((e, r, t, n) => (a(e, t), u(r, 0, t, n)))), v = p(((e, r, t, n, i) => {
-        var o = r && S.o(r, t) && c(r, t, n);
-        return o ? s(o) : i()
-    })), b = {}, m = {
-        1395: () => h("default", "@jupyter-widgets/base", [, [1, 6],
-            [1, 5],
-            [1, 4],
+    }, s = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, a, n) {
+        var i = j.I(r);
+        return i && i.then ? i.then(e.bind(e, r, j.S[r], t, a, n)) : e(r, j.S[r], t, a, n)
+    })(((e, r, t, a) => (o(e, t), u(r, 0, t, a)))), b = p(((e, r, t, a, n) => {
+        var i = r && j.o(r, t) && c(r, t, a);
+        return i ? s(i) : n()
+    })), v = {}, m = {
+        1057: () => b("default", "@tiledb-inc/bioimage-viewer", [2, 0, 1, 1, , "beta", 0], (() => Promise.all([j.e(635), j.e(172), j.e(774), j.e(446)]).then((() => () => j(3774))))),
+        8233: () => b("default", "@jupyter-widgets/base", [, [1, 4],
             [1, 3],
-            [1, 2], 1, 1, 1, 1
-        ]),
-        2832: () => v("default", "@tiledb-inc/bioimage-viewer", [2, 0, 1, 0, , "alpha", 7], (() => Promise.all([S.e(635), S.e(774), S.e(446)]).then((() => () => S(3774))))),
+            [1, 2],
+            [1, 1, 1, 10], 1, 1, 1
+        ], (() => Promise.all([j.e(172), j.e(713), j.e(38)]).then((() => () => j(2713))))),
+        1526: () => h("default", "@lumino/coreutils", [1, 1, 11, 0]),
+        2720: () => h("default", "@lumino/messaging", [1, 1, 10, 0]),
+        8832: () => h("default", "@lumino/widgets", [1, 1, 37, 2]),
         4456: () => h("default", "react-dom", [1, 17, 0, 1]),
         6271: () => h("default", "react", [1, 17, 0, 1])
     }, g = {
+        38: [1526, 2720, 8832],
         446: [4456, 6271],
-        744: [1395, 2832]
-    }, S.f.consumes = (e, r) => {
-        S.o(g, e) && g[e].forEach((e => {
-            if (S.o(b, e)) return r.push(b[e]);
+        744: [1057, 8233]
+    }, j.f.consumes = (e, r) => {
+        j.o(g, e) && g[e].forEach((e => {
+            if (j.o(v, e)) return r.push(v[e]);
             var t = r => {
-                    b[e] = 0, S.m[e] = t => {
-                        delete S.c[e], t.exports = r()
+                    v[e] = 0, j.m[e] = t => {
+                        delete j.c[e], t.exports = r()
                     }
                 },
-                n = r => {
-                    delete b[e], S.m[e] = t => {
-                        throw delete S.c[e], r
+                a = r => {
+                    delete v[e], j.m[e] = t => {
+                        throw delete j.c[e], r
                     }
                 };
             try {
-                var i = m[e]();
-                i.then ? r.push(b[e] = i.then(t).catch(n)) : t(i)
+                var n = m[e]();
+                n.then ? r.push(v[e] = n.then(t).catch(a)) : t(n)
             } catch (e) {
-                n(e)
+                a(e)
             }
         }))
     }, (() => {
-        S.b = document.baseURI || self.location.href;
+        j.b = document.baseURI || self.location.href;
         var e = {
             448: 0
         };
-        S.f.j = (r, t) => {
-            var n = S.o(e, r) ? e[r] : void 0;
-            if (0 !== n)
-                if (n) t.push(n[2]);
-                else {
-                    var i = new Promise(((t, i) => n = e[r] = [t, i]));
-                    t.push(n[2] = i);
-                    var o = S.p + S.u(r),
-                        a = new Error;
-                    S.l(o, (t => {
-                        if (S.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                            var i = t && ("load" === t.type ? "missing" : t.type),
-                                o = t && t.target && t.target.src;
-                            a.message = "Loading chunk " + r + " failed.\n(" + i + ": " + o + ")", a.name = "ChunkLoadError", a.type = i, a.request = o, n[1](a)
-                        }
-                    }), "chunk-" + r, r)
-                }
+        j.f.j = (r, t) => {
+            var a = j.o(e, r) ? e[r] : void 0;
+            if (0 !== a)
+                if (a) t.push(a[2]);
+                else if (38 != r) {
+                var n = new Promise(((t, n) => a = e[r] = [t, n]));
+                t.push(a[2] = n);
+                var i = j.p + j.u(r),
+                    o = new Error;
+                j.l(i, (t => {
+                    if (j.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
+                        var n = t && ("load" === t.type ? "missing" : t.type),
+                            i = t && t.target && t.target.src;
+                        o.message = "Loading chunk " + r + " failed.\n(" + n + ": " + i + ")", o.name = "ChunkLoadError", o.type = n, o.request = i, a[1](o)
+                    }
+                }), "chunk-" + r, r)
+            } else e[r] = 0
         };
         var r = (r, t) => {
-                var n, i, [o, a, d] = t,
-                    l = 0;
-                if (o.some((r => 0 !== e[r]))) {
-                    for (n in a) S.o(a, n) && (S.m[n] = a[n]);
-                    d && d(S)
+                var a, n, [i, o, l] = t,
+                    d = 0;
+                if (i.some((r => 0 !== e[r]))) {
+                    for (a in o) j.o(o, a) && (j.m[a] = o[a]);
+                    l && l(j)
                 }
-                for (r && r(t); l < o.length; l++) i = o[l], S.o(e, i) && e[i] && e[i][0](), e[i] = 0
+                for (r && r(t); d < i.length; d++) n = i[d], j.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer = self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })(), S.nc = void 0;
-    var j = S(5290);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@tiledb-inc/jupyter-bioimage-viewer"] = j
+    })(), j.nc = void 0;
+    var S = j(5290);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@tiledb-inc/jupyter-bioimage-viewer"] = S
 })();
```

### Comparing `tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json` & `tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9576612903225806%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '7.21.5'}, 24: {'versionInfo': '0.1.1-beta.0'}, insert: [(6, "*

 * *               "OrderedDict([('name', '@jupyter-widgets/base'), ('versionInfo', '4.1.1'), "*

 * *               "('licenseId', 'BSD-3-Clause'), ('extractedText', 'Copyright (c) 2015 Project "*

 * *               'Jupyter Contributors\\nAll rights reserved.\\n\\nRedistribution and use in source '*

 * *               'and binary forms, with or without\\nmodification, are permitted provided that the '*

 * *               'following  […]*

```diff
@@ -1,14 +1,14 @@
 {
     "packages": [
         {
             "extractedText": "MIT License\n\nCopyright (c) 2014-present Sebastian McKenzie and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n\"Software\"), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND\nNONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE\nLIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION\nOF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION\nWITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "@babel/runtime",
-            "versionInfo": "7.22.3"
+            "versionInfo": "7.21.5"
         },
         {
             "extractedText": "Copyright (c) 2020 Urban Computing Foundation\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN\nTHE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "@deck.gl/core",
             "versionInfo": "8.8.12"
         },
@@ -33,14 +33,20 @@
         {
             "extractedText": "",
             "licenseId": "MIT",
             "name": "@icons/material",
             "versionInfo": "0.2.4"
         },
         {
+            "extractedText": "Copyright (c) 2015 Project Jupyter Contributors\nAll rights reserved.\n\nRedistribution and use in source and binary forms, with or without\nmodification, are permitted provided that the following conditions are met:\n\n1. Redistributions of source code must retain the above copyright notice, this\n   list of conditions and the following disclaimer.\n\n2. Redistributions in binary form must reproduce the above copyright notice,\n   this list of conditions and the following disclaimer in the documentation\n   and/or other materials provided with the distribution.\n\n3. Neither the name of the copyright holder nor the names of its\n   contributors may be used to endorse or promote products derived from\n   this software without specific prior written permission.\n\nTHIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS \"AS IS\"\nAND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE\nIMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE\nDISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE\nFOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL\nDAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR\nSERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER\nCAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,\nOR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE\nOF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.\n",
+            "licenseId": "BSD-3-Clause",
+            "name": "@jupyter-widgets/base",
+            "versionInfo": "4.1.1"
+        },
+        {
             "extractedText": "Copyright (c) 2015 Uber Technologies, Inc.\n\nThis software includes parts of PhiloGL (https://github.com/philogb/philogl)\nunder MIT license. PhiloGL parts Copyright \u00a9 2013 Sencha Labs.\n\nThis software includes adaptations of postprocessing code from THREE.js (https://github.com/mrdoob/three.js/) under MIT license. Additional attribution given in specific source files. THREE.js parts Copyright \u00a9 2010-2018 three.js authors.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN\nTHE SOFTWARE.\n\n\nloaders.gl includes certain files from Cesium (https://github.com/AnalyticalGraphicsInc/cesium) under the Apache 2 License:\n\nCopyright 2011-2018 CesiumJS Contributors\n\nLicensed under the Apache License, Version 2.0 (the \"License\");\nyou may not use this file except in compliance with the License.\nYou may obtain a copy of the License at\nhttp://www.apache.org/licenses/LICENSE-2.0\n\nUnless required by applicable law or agreed to in writing, software\ndistributed under the License is distributed on an \"AS IS\" BASIS,\nWITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\nSee the License for the specific language governing permissions and limitations under the License.\n\nCesium-derived code can be found in the submodule: modules/3d-tiles\n",
             "licenseId": "MIT",
             "name": "@loaders.gl/core",
             "versionInfo": "3.4.4"
         },
         {
             "extractedText": "Copyright (c) 2015 Uber Technologies, Inc.\n\nThis software includes parts of PhiloGL (https://github.com/philogb/philogl)\nunder MIT license. PhiloGL parts Copyright \u00a9 2013 Sencha Labs.\n\nThis software includes adaptations of postprocessing code from THREE.js (https://github.com/mrdoob/three.js/) under MIT license. Additional attribution given in specific source files. THREE.js parts Copyright \u00a9 2010-2018 three.js authors.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN\nTHE SOFTWARE.\n\n\nloaders.gl includes certain files from Cesium (https://github.com/AnalyticalGraphicsInc/cesium) under the Apache 2 License:\n\nCopyright 2011-2018 CesiumJS Contributors\n\nLicensed under the Apache License, Version 2.0 (the \"License\");\nyou may not use this file except in compliance with the License.\nYou may obtain a copy of the License at\nhttp://www.apache.org/licenses/LICENSE-2.0\n\nUnless required by applicable law or agreed to in writing, software\ndistributed under the License is distributed on an \"AS IS\" BASIS,\nWITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\nSee the License for the specific language governing permissions and limitations under the License.\n\nCesium-derived code can be found in the submodule: modules/3d-tiles\n",
@@ -138,15 +144,15 @@
             "name": "@probe.gl/stats",
             "versionInfo": "3.6.0"
         },
         {
             "extractedText": "",
             "licenseId": "MIT",
             "name": "@tiledb-inc/bioimage-viewer",
-            "versionInfo": "0.1.0-alpha.8"
+            "versionInfo": "0.1.1-beta.0"
         },
         {
             "extractedText": "MIT License\n\nCopyright (c) 2020 TileDB, Inc.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "@tiledb-inc/tiledb-cloud",
             "versionInfo": "1.0.13-alpha.0"
         },
@@ -159,14 +165,26 @@
         {
             "extractedText": "Copyright (c) 2014-present Matt Zabriskie\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN\nTHE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "axios",
             "versionInfo": "0.21.4"
         },
         {
+            "extractedText": "",
+            "licenseId": "MIT",
+            "name": "backbone",
+            "versionInfo": "1.2.3"
+        },
+        {
+            "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2014 Jameson Little\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN\nTHE SOFTWARE.\n",
+            "licenseId": "MIT",
+            "name": "base64-js",
+            "versionInfo": "1.5.1"
+        },
+        {
             "extractedText": "MIT License\n\nCopyright (c) 2017 Juli\u00e1n D\u00edaz (jdiaz5513)\n\nPermission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the \"Software\"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "capnp-ts",
             "versionInfo": "0.4.0"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
@@ -225,14 +243,20 @@
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) Sindre Sorhus <sindresorhus@gmail.com> (sindresorhus.com)\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN\nTHE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "is-blob",
             "versionInfo": "1.0.0"
         },
         {
+            "extractedText": "Copyright OpenJS Foundation and other contributors, https://openjsf.org/\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n\"Software\"), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND\nNONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE\nLIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION\nOF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION\nWITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
+            "licenseId": "MIT",
+            "name": "jquery",
+            "versionInfo": "3.7.0"
+        },
+        {
             "extractedText": "Copyright OpenJS Foundation and other contributors <https://openjsf.org/>\n\nBased on Underscore.js, copyright Jeremy Ashkenas,\nDocumentCloud and Investigative Reporters & Editors <http://underscorejs.org/>\n\nThis software consists of voluntary contributions made by many\nindividuals. For exact contribution history, see the revision history\navailable at https://github.com/lodash/lodash\n\nThe following license applies to all parts of this software except as\ndocumented below:\n\n====\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n\"Software\"), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND\nNONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE\nLIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION\nOF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION\nWITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n\n====\n\nCopyright and related rights for sample code are waived via CC0. Sample\ncode is defined as all source code displayed within the prose of the\ndocumentation.\n\nCC0: http://creativecommons.org/publicdomain/zero/1.0/\n\n====\n\nFiles located in the node_modules and vendor directories are externally\nmaintained libraries used by this software which have their own\nlicenses; we recommend you read them, as their terms may differ from the\nterms above.\n",
             "licenseId": "MIT",
             "name": "lodash",
             "versionInfo": "4.17.21"
         },
         {
             "extractedText": "Copyright OpenJS Foundation and other contributors <https://openjsf.org/>\n\nBased on Underscore.js, copyright Jeremy Ashkenas,\nDocumentCloud and Investigative Reporters & Editors <http://underscorejs.org/>\n\nThis software consists of voluntary contributions made by many\nindividuals. For exact contribution history, see the revision history\navailable at https://github.com/lodash/lodash\n\nThe following license applies to all parts of this software except as\ndocumented below:\n\n====\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n\"Software\"), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND\nNONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE\nLIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION\nOF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION\nWITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n\n====\n\nCopyright and related rights for sample code are waived via CC0. Sample\ncode is defined as all source code displayed within the prose of the\ndocumentation.\n\nCC0: http://creativecommons.org/publicdomain/zero/1.0/\n\n====\n\nFiles located in the node_modules and vendor directories are externally\nmaintained libraries used by this software which have their own\nlicenses; we recommend you read them, as their terms may differ from the\nterms above.\n",
@@ -337,10 +361,16 @@
             "versionInfo": "3.2.0"
         },
         {
             "extractedText": "Copyright (c) Microsoft Corporation.\n\nPermission to use, copy, modify, and/or distribute this software for any\npurpose with or without fee is hereby granted.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH\nREGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY\nAND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,\nINDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM\nLOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR\nOTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR\nPERFORMANCE OF THIS SOFTWARE.",
             "licenseId": "0BSD",
             "name": "tslib",
             "versionInfo": "1.14.1"
+        },
+        {
+            "extractedText": "Copyright (c) 2009-2022 Jeremy Ashkenas, Julian Gonggrijp, and DocumentCloud and Investigative Reporters & Editors\n\nPermission is hereby granted, free of charge, to any person\nobtaining a copy of this software and associated documentation\nfiles (the \"Software\"), to deal in the Software without\nrestriction, including without limitation the rights to use,\ncopy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the\nSoftware is furnished to do so, subject to the following\nconditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES\nOF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND\nNONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT\nHOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,\nWHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING\nFROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR\nOTHER DEALINGS IN THE SOFTWARE.\n",
+            "licenseId": "MIT",
+            "name": "underscore",
+            "versionInfo": "1.13.6"
         }
     ]
 }
```

### Comparing `tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg.egg-info/PKG-INFO` & `tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledb-jupyter-bioimg
-Version: 0.1.2a1
+Version: 0.1.2a2
 Summary: A jupyterlab extension to visualize bioimages in TileDB format
 Home-page: https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer
 Author: TileDB
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
@@ -85,14 +85,10 @@
 
 ### Usage
 
 ```python
 
 from tiledb_jupyter_bioimg import Render
 
-Render("<<NAMESPACE>>", "<<GROUP_ID>>")
+Render("<<NAMESPACE>>", "<<GROUP_ID>>", {"token": "<<TILEDB_API_TOKEN>>>"})
 
 ```
-
-### Common issues
-
-If you get error `Uncaught (in promise) Error: No provider for: jupyter.extensions.jupyterWidgetRegistry.` please make sure you are using correct version of `ipywidgets` (v8).
```

### Comparing `tiledb_jupyter_bioimg-0.1.2a1/tiledb_jupyter_bioimg.egg-info/SOURCES.txt` & `tiledb_jupyter_bioimg-0.1.2a2/tiledb_jupyter_bioimg.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -20,18 +20,21 @@
 tiledb_jupyter_bioimg.egg-info/SOURCES.txt
 tiledb_jupyter_bioimg.egg-info/dependency_links.txt
 tiledb_jupyter_bioimg.egg-info/not-zip-safe
 tiledb_jupyter_bioimg.egg-info/requires.txt
 tiledb_jupyter_bioimg.egg-info/top_level.txt
 tiledb_jupyter_bioimg/labextension/package.json
 tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg
-tiledb_jupyter_bioimg/labextension/static/408.635d4bfc76ee689544e0.js
+tiledb_jupyter_bioimg/labextension/static/172.6267f3dd3063477e34ed.js
+tiledb_jupyter_bioimg/labextension/static/408.bdb74ff9f40e9eef1c08.js
 tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
-tiledb_jupyter_bioimg/labextension/static/635.b2bedc962bcd82714540.js
-tiledb_jupyter_bioimg/labextension/static/635.b2bedc962bcd82714540.js.LICENSE.txt
-tiledb_jupyter_bioimg/labextension/static/744.23211eab87ca12d5bb82.js
+tiledb_jupyter_bioimg/labextension/static/635.f8f404497739316e801c.js
+tiledb_jupyter_bioimg/labextension/static/635.f8f404497739316e801c.js.LICENSE.txt
+tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js
+tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js.LICENSE.txt
+tiledb_jupyter_bioimg/labextension/static/744.6ac09e98bdf01bd3b6d1.js
 tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js
-tiledb_jupyter_bioimg/labextension/static/774.a940595120cb008c0c58.js
-tiledb_jupyter_bioimg/labextension/static/774.a940595120cb008c0c58.js.LICENSE.txt
-tiledb_jupyter_bioimg/labextension/static/remoteEntry.555c16a49a97a15a2937.js
+tiledb_jupyter_bioimg/labextension/static/774.309d750794b6276f460a.js
+tiledb_jupyter_bioimg/labextension/static/774.309d750794b6276f460a.js.LICENSE.txt
+tiledb_jupyter_bioimg/labextension/static/remoteEntry.b197e4666f084e8dece0.js
 tiledb_jupyter_bioimg/labextension/static/style.js
 tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
```

### Comparing `tiledb_jupyter_bioimg-0.1.2a1/tsconfig.json` & `tiledb_jupyter_bioimg-0.1.2a2/tsconfig.json`

 * *Files identical despite different names*

