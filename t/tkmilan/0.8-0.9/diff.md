# Comparing `tmp/tkmilan-0.8.tar.gz` & `tmp/tkmilan-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkmilan-0.8.tar", last modified: Thu Mar 17 19:13:27 2022, max compression
+gzip compressed data, was "tkmilan-0.9.tar", last modified: Fri May  6 18:25:13 2022, max compression
```

## Comparing `tkmilan-0.8.tar` & `tkmilan-0.9.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 safonso   (1000) safonso   (1000)        0 2022-03-17 19:13:27.730695 tkmilan-0.8/
--rw-r--r--   0 safonso   (1000) safonso   (1000)      141 2021-10-25 16:38:36.000000 tkmilan-0.8/.gitignore
--rw-r--r--   0 safonso   (1000) safonso   (1000)     7652 2021-05-11 10:18:43.000000 tkmilan-0.8/LICENSE
--rw-r--r--   0 safonso   (1000) safonso   (1000)      236 2022-03-16 18:47:21.000000 tkmilan-0.8/MANIFEST.in
--rw-r--r--   0 safonso   (1000) safonso   (1000)      622 2022-03-17 19:13:27.734029 tkmilan-0.8/PKG-INFO
--rw-r--r--   0 safonso   (1000) safonso   (1000)       33 2022-03-16 17:37:01.000000 tkmilan-0.8/README.md
-drwxr-xr-x   0 safonso   (1000) safonso   (1000)        0 2022-03-17 19:13:27.720695 tkmilan-0.8/docs/
-drwxr-xr-x   0 safonso   (1000) safonso   (1000)        0 2022-03-17 19:13:27.724028 tkmilan-0.8/docs/api/
--rw-r--r--   0 safonso   (1000) safonso   (1000)      313 2022-03-17 19:13:25.000000 tkmilan-0.8/docs/api/tkmilan.exception.rst
--rw-r--r--   0 safonso   (1000) safonso   (1000)      380 2022-03-17 19:13:25.000000 tkmilan-0.8/docs/api/tkmilan.fn.rst
--rw-r--r--   0 safonso   (1000) safonso   (1000)      330 2022-03-17 19:13:25.000000 tkmilan-0.8/docs/api/tkmilan.mixin.rst
--rw-r--r--   0 safonso   (1000) safonso   (1000)      746 2022-03-17 19:13:25.000000 tkmilan-0.8/docs/api/tkmilan.model.rst
--rw-r--r--   0 safonso   (1000) safonso   (1000)      273 2022-03-17 19:13:25.000000 tkmilan-0.8/docs/api/tkmilan.parser.rst
--rw-r--r--   0 safonso   (1000) safonso   (1000)      796 2022-03-17 19:13:25.000000 tkmilan-0.8/docs/api/tkmilan.rst
--rw-r--r--   0 safonso   (1000) safonso   (1000)      398 2022-03-17 19:13:25.000000 tkmilan-0.8/docs/api/tkmilan.spec.rst
--rw-r--r--   0 safonso   (1000) safonso   (1000)      201 2022-03-17 19:13:25.000000 tkmilan-0.8/docs/api/tkmilan.util.rst
--rw-r--r--   0 safonso   (1000) safonso   (1000)      292 2022-03-17 19:13:25.000000 tkmilan-0.8/docs/api/tkmilan.var.rst
--rw-r--r--   0 safonso   (1000) safonso   (1000)      230 2021-08-06 18:41:16.000000 tkmilan-0.8/docs/api.rst
--rw-r--r--   0 safonso   (1000) safonso   (1000)     6649 2021-08-26 17:56:37.000000 tkmilan-0.8/docs/conf.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)      492 2021-08-11 10:55:58.000000 tkmilan-0.8/docs/development.rst
--rw-r--r--   0 safonso   (1000) safonso   (1000)      693 2021-08-26 17:58:29.000000 tkmilan-0.8/docs/index.rst
--rw-r--r--   0 safonso   (1000) safonso   (1000)      567 2021-08-10 15:42:51.000000 tkmilan-0.8/docs/summary.rst
--rw-r--r--   0 safonso   (1000) safonso   (1000)      161 2021-08-03 16:16:44.000000 tkmilan-0.8/pyproject.toml
--rw-r--r--   0 safonso   (1000) safonso   (1000)      244 2021-10-25 17:24:57.000000 tkmilan-0.8/requirements-dev.txt
--rw-r--r--   0 safonso   (1000) safonso   (1000)        0 2021-06-01 15:43:08.000000 tkmilan-0.8/requirements.txt
--rw-r--r--   0 safonso   (1000) safonso   (1000)      975 2022-03-17 19:13:27.734029 tkmilan-0.8/setup.cfg
--rw-r--r--   0 safonso   (1000) safonso   (1000)       65 2021-08-03 16:16:44.000000 tkmilan-0.8/setup.py
-drwxr-xr-x   0 safonso   (1000) safonso   (1000)        0 2022-03-17 19:13:27.717362 tkmilan-0.8/src/
-drwxr-xr-x   0 safonso   (1000) safonso   (1000)        0 2022-03-17 19:13:27.727362 tkmilan-0.8/src/tkmilan/
--rw-r--r--   0 safonso   (1000) safonso   (1000)    83876 2022-03-17 17:34:17.000000 tkmilan-0.8/src/tkmilan/__init__.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)    23020 2022-03-16 20:05:00.000000 tkmilan-0.8/src/tkmilan/__main__.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)      451 2022-03-16 12:52:05.000000 tkmilan-0.8/src/tkmilan/exception.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)    17816 2022-03-04 18:52:17.000000 tkmilan-0.8/src/tkmilan/fn.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)    33073 2022-03-16 19:30:23.000000 tkmilan-0.8/src/tkmilan/mixin.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)    40585 2022-03-16 18:56:29.000000 tkmilan-0.8/src/tkmilan/model.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)     8255 2022-03-03 19:17:16.000000 tkmilan-0.8/src/tkmilan/parser.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)        0 2021-10-27 18:27:38.000000 tkmilan-0.8/src/tkmilan/py.typed
-drwxr-xr-x   0 safonso   (1000) safonso   (1000)        0 2022-03-17 19:13:27.730695 tkmilan-0.8/src/tkmilan/showcase-images/
--rw-r--r--   0 safonso   (1000) safonso   (1000)      152 2022-03-16 18:49:29.000000 tkmilan-0.8/src/tkmilan/showcase-images/README.md
--rw-r--r--   0 safonso   (1000) safonso   (1000)      728 2022-03-15 15:12:08.000000 tkmilan-0.8/src/tkmilan/showcase-images/error-s16.png
--rw-r--r--   0 safonso   (1000) safonso   (1000)      200 2022-03-16 19:59:26.000000 tkmilan-0.8/src/tkmilan/showcase-images/info-msgbox-s16.png
--rw-r--r--   0 safonso   (1000) safonso   (1000)      114 2022-03-16 19:47:04.000000 tkmilan-0.8/src/tkmilan/showcase-images/info-s16.png
--rw-r--r--   0 safonso   (1000) safonso   (1000)      520 2022-03-15 15:12:08.000000 tkmilan-0.8/src/tkmilan/showcase-images/warning-s16.png
--rw-r--r--   0 safonso   (1000) safonso   (1000)     6721 2022-02-18 12:24:20.000000 tkmilan-0.8/src/tkmilan/spec.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)      425 2021-08-06 18:41:16.000000 tkmilan-0.8/src/tkmilan/util.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)     2942 2021-11-15 19:44:19.000000 tkmilan-0.8/src/tkmilan/var.py
-drwxr-xr-x   0 safonso   (1000) safonso   (1000)        0 2022-03-17 19:13:27.730695 tkmilan-0.8/src/tkmilan.egg-info/
--rw-r--r--   0 safonso   (1000) safonso   (1000)      622 2022-03-17 19:13:27.000000 tkmilan-0.8/src/tkmilan.egg-info/PKG-INFO
--rw-r--r--   0 safonso   (1000) safonso   (1000)     1105 2022-03-17 19:13:27.000000 tkmilan-0.8/src/tkmilan.egg-info/SOURCES.txt
--rw-r--r--   0 safonso   (1000) safonso   (1000)        1 2022-03-17 19:13:27.000000 tkmilan-0.8/src/tkmilan.egg-info/dependency_links.txt
--rw-r--r--   0 safonso   (1000) safonso   (1000)       65 2022-03-17 19:13:27.000000 tkmilan-0.8/src/tkmilan.egg-info/entry_points.txt
--rw-r--r--   0 safonso   (1000) safonso   (1000)        8 2022-03-17 19:13:27.000000 tkmilan-0.8/src/tkmilan.egg-info/top_level.txt
-drwxr-xr-x   0 safonso   (1000) safonso   (1000)        0 2022-03-17 19:13:27.730695 tkmilan-0.8/tests/
--rw-r--r--   0 safonso   (1000) safonso   (1000)     6135 2021-09-03 16:46:53.000000 tkmilan-0.8/tests/test_model.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)     2468 2022-03-03 18:47:10.000000 tkmilan-0.8/tests/test_parser_ltml.py
+drwxr-xr-x   0 safonso   (1000) safonso   (1000)        0 2022-05-06 18:25:13.338069 tkmilan-0.9/
+-rw-r--r--   0 safonso   (1000) safonso   (1000)      155 2022-05-04 15:47:58.000000 tkmilan-0.9/.gitignore
+-rw-r--r--   0 safonso   (1000) safonso   (1000)     7652 2021-05-11 10:18:43.000000 tkmilan-0.9/LICENSE
+-rw-r--r--   0 safonso   (1000) safonso   (1000)      236 2022-03-16 18:47:21.000000 tkmilan-0.9/MANIFEST.in
+-rw-r--r--   0 safonso   (1000) safonso   (1000)      622 2022-05-06 18:25:13.338069 tkmilan-0.9/PKG-INFO
+-rw-r--r--   0 safonso   (1000) safonso   (1000)       33 2022-03-16 17:37:01.000000 tkmilan-0.9/README.md
+drwxr-xr-x   0 safonso   (1000) safonso   (1000)        0 2022-05-06 18:25:13.331402 tkmilan-0.9/docs/
+drwxr-xr-x   0 safonso   (1000) safonso   (1000)        0 2022-05-06 18:25:13.331402 tkmilan-0.9/docs/api/
+-rw-r--r--   0 safonso   (1000) safonso   (1000)      313 2022-05-06 18:23:00.000000 tkmilan-0.9/docs/api/tkmilan.exception.rst
+-rw-r--r--   0 safonso   (1000) safonso   (1000)      396 2022-05-06 18:23:00.000000 tkmilan-0.9/docs/api/tkmilan.fn.rst
+-rw-r--r--   0 safonso   (1000) safonso   (1000)      330 2022-05-06 18:23:00.000000 tkmilan-0.9/docs/api/tkmilan.mixin.rst
+-rw-r--r--   0 safonso   (1000) safonso   (1000)      746 2022-05-06 18:23:00.000000 tkmilan-0.9/docs/api/tkmilan.model.rst
+-rw-r--r--   0 safonso   (1000) safonso   (1000)      273 2022-05-06 18:23:00.000000 tkmilan-0.9/docs/api/tkmilan.parser.rst
+-rw-r--r--   0 safonso   (1000) safonso   (1000)      817 2022-05-06 18:23:00.000000 tkmilan-0.9/docs/api/tkmilan.rst
+-rw-r--r--   0 safonso   (1000) safonso   (1000)      398 2022-05-06 18:23:00.000000 tkmilan-0.9/docs/api/tkmilan.spec.rst
+-rw-r--r--   0 safonso   (1000) safonso   (1000)      280 2022-05-06 18:23:00.000000 tkmilan-0.9/docs/api/tkmilan.util.rst
+-rw-r--r--   0 safonso   (1000) safonso   (1000)      292 2022-05-06 18:23:00.000000 tkmilan-0.9/docs/api/tkmilan.var.rst
+-rw-r--r--   0 safonso   (1000) safonso   (1000)      230 2021-08-06 18:41:16.000000 tkmilan-0.9/docs/api.rst
+-rw-r--r--   0 safonso   (1000) safonso   (1000)     6668 2022-05-04 15:18:11.000000 tkmilan-0.9/docs/conf.py
+-rw-r--r--   0 safonso   (1000) safonso   (1000)      492 2021-08-11 10:55:58.000000 tkmilan-0.9/docs/development.rst
+-rw-r--r--   0 safonso   (1000) safonso   (1000)      693 2021-08-26 17:58:29.000000 tkmilan-0.9/docs/index.rst
+-rw-r--r--   0 safonso   (1000) safonso   (1000)      567 2021-08-10 15:42:51.000000 tkmilan-0.9/docs/summary.rst
+-rw-r--r--   0 safonso   (1000) safonso   (1000)      225 2022-05-04 15:51:13.000000 tkmilan-0.9/pyproject.toml
+-rw-r--r--   0 safonso   (1000) safonso   (1000)      249 2022-05-06 18:24:35.000000 tkmilan-0.9/requirements-dev.txt
+-rw-r--r--   0 safonso   (1000) safonso   (1000)        0 2021-06-01 15:43:08.000000 tkmilan-0.9/requirements.txt
+-rw-r--r--   0 safonso   (1000) safonso   (1000)      975 2022-05-06 18:25:13.338069 tkmilan-0.9/setup.cfg
+-rw-r--r--   0 safonso   (1000) safonso   (1000)       65 2021-08-03 16:16:44.000000 tkmilan-0.9/setup.py
+drwxr-xr-x   0 safonso   (1000) safonso   (1000)        0 2022-05-06 18:25:13.328068 tkmilan-0.9/src/
+drwxr-xr-x   0 safonso   (1000) safonso   (1000)        0 2022-05-06 18:25:13.334735 tkmilan-0.9/src/tkmilan/
+-rw-r--r--   0 safonso   (1000) safonso   (1000)    96031 2022-05-06 18:23:30.000000 tkmilan-0.9/src/tkmilan/__init__.py
+-rw-r--r--   0 safonso   (1000) safonso   (1000)    24098 2022-05-06 18:14:18.000000 tkmilan-0.9/src/tkmilan/__main__.py
+-rw-r--r--   0 safonso   (1000) safonso   (1000)      451 2022-03-16 12:52:05.000000 tkmilan-0.9/src/tkmilan/exception.py
+-rw-r--r--   0 safonso   (1000) safonso   (1000)    19083 2022-05-05 16:43:52.000000 tkmilan-0.9/src/tkmilan/fn.py
+-rw-r--r--   0 safonso   (1000) safonso   (1000)    35878 2022-05-05 12:05:23.000000 tkmilan-0.9/src/tkmilan/mixin.py
+-rw-r--r--   0 safonso   (1000) safonso   (1000)    40789 2022-05-03 16:57:37.000000 tkmilan-0.9/src/tkmilan/model.py
+-rw-r--r--   0 safonso   (1000) safonso   (1000)     8255 2022-03-03 19:17:16.000000 tkmilan-0.9/src/tkmilan/parser.py
+-rw-r--r--   0 safonso   (1000) safonso   (1000)        0 2021-10-27 18:27:38.000000 tkmilan-0.9/src/tkmilan/py.typed
+drwxr-xr-x   0 safonso   (1000) safonso   (1000)        0 2022-05-06 18:25:13.334735 tkmilan-0.9/src/tkmilan/showcase-images/
+-rw-r--r--   0 safonso   (1000) safonso   (1000)      152 2022-03-16 18:49:29.000000 tkmilan-0.9/src/tkmilan/showcase-images/README.md
+-rw-r--r--   0 safonso   (1000) safonso   (1000)      728 2022-03-15 15:12:08.000000 tkmilan-0.9/src/tkmilan/showcase-images/error-s16.png
+-rw-r--r--   0 safonso   (1000) safonso   (1000)      200 2022-03-16 19:59:26.000000 tkmilan-0.9/src/tkmilan/showcase-images/info-msgbox-s16.png
+-rw-r--r--   0 safonso   (1000) safonso   (1000)      114 2022-03-16 19:47:04.000000 tkmilan-0.9/src/tkmilan/showcase-images/info-s16.png
+-rw-r--r--   0 safonso   (1000) safonso   (1000)      520 2022-03-15 15:12:08.000000 tkmilan-0.9/src/tkmilan/showcase-images/warning-s16.png
+-rw-r--r--   0 safonso   (1000) safonso   (1000)     6721 2022-02-18 12:24:20.000000 tkmilan-0.9/src/tkmilan/spec.py
+-rw-r--r--   0 safonso   (1000) safonso   (1000)      767 2022-05-04 12:08:15.000000 tkmilan-0.9/src/tkmilan/util.py
+-rw-r--r--   0 safonso   (1000) safonso   (1000)     2942 2021-11-15 19:44:19.000000 tkmilan-0.9/src/tkmilan/var.py
+drwxr-xr-x   0 safonso   (1000) safonso   (1000)        0 2022-05-06 18:25:13.334735 tkmilan-0.9/src/tkmilan.egg-info/
+-rw-r--r--   0 safonso   (1000) safonso   (1000)      622 2022-05-06 18:25:12.000000 tkmilan-0.9/src/tkmilan.egg-info/PKG-INFO
+-rw-r--r--   0 safonso   (1000) safonso   (1000)     1134 2022-05-06 18:25:13.000000 tkmilan-0.9/src/tkmilan.egg-info/SOURCES.txt
+-rw-r--r--   0 safonso   (1000) safonso   (1000)        1 2022-05-06 18:25:12.000000 tkmilan-0.9/src/tkmilan.egg-info/dependency_links.txt
+-rw-r--r--   0 safonso   (1000) safonso   (1000)       65 2022-05-06 18:25:12.000000 tkmilan-0.9/src/tkmilan.egg-info/entry_points.txt
+-rw-r--r--   0 safonso   (1000) safonso   (1000)        8 2022-05-06 18:25:13.000000 tkmilan-0.9/src/tkmilan.egg-info/top_level.txt
+drwxr-xr-x   0 safonso   (1000) safonso   (1000)        0 2022-05-06 18:25:13.334735 tkmilan-0.9/tests/
+-rw-r--r--   0 safonso   (1000) safonso   (1000)     6135 2021-09-03 16:46:53.000000 tkmilan-0.9/tests/test_model.py
+-rw-r--r--   0 safonso   (1000) safonso   (1000)     2468 2022-03-03 18:47:10.000000 tkmilan-0.9/tests/test_parser_ltml.py
+-rw-r--r--   0 safonso   (1000) safonso   (1000)      407 2022-05-06 17:16:24.000000 tkmilan-0.9/tests/test_widget_listbox.py
```

### Comparing `tkmilan-0.8/LICENSE` & `tkmilan-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tkmilan-0.8/PKG-INFO` & `tkmilan-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkmilan
-Version: 0.8
+Version: 0.9
 Summary: tkinter's evil twin
 Home-page: https://support.powertools-tech.com/PowertoolsTech/tkmilan
 Author: Powertools Technologies
 Author-email: simao.afonso@powertools-tech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tkmilan-0.8/docs/api/tkmilan.model.rst` & `tkmilan-0.9/docs/api/tkmilan.model.rst`

 * *Files identical despite different names*

### Comparing `tkmilan-0.8/docs/api/tkmilan.rst` & `tkmilan-0.9/docs/api/tkmilan.rst`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
       FrameLabelled
       FramePaned
       FrameStateful
       FrameUnlabelled
       Label
       LabelStateful
       Listbox
+      ListboxControl
       Notebook
       NotebookUniform
       RootWindow
       ScrolledWidget
       Tree
       varTree
```

### Comparing `tkmilan-0.8/docs/conf.py` & `tkmilan-0.9/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,16 @@
 
 # Auto API Documentation
 # - A souped-up version of AutoSummary and AutoDoc
 extensions.append('sphinx_automodapi.automodapi')
 extensions.append('sphinx_automodapi.smart_resolver')
 
 # Expose slow files
-extensions.append('sphinx.ext.duration')
+if PRODUCTION:
+    extensions.append('sphinx.ext.duration')
 
 # Include GitHub Detritus
 extensions.append('sphinx.ext.githubpages')
 
 # Support ToDo
 extensions.append('sphinx.ext.todo')
 todo_emit_warnings = PRODUCTION is False
```

### Comparing `tkmilan-0.8/docs/index.rst` & `tkmilan-0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tkmilan-0.8/docs/summary.rst` & `tkmilan-0.9/docs/summary.rst`

 * *Files identical despite different names*

### Comparing `tkmilan-0.8/setup.cfg` & `tkmilan-0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `tkmilan-0.8/src/tkmilan/__init__.py` & `tkmilan-0.9/src/tkmilan/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -83,5161 +83,5920 @@
 00000520: 2727 270a 5645 5254 4943 414c 203d 206d  '''.VERTICAL = m
 00000530: 6978 696e 2e56 4552 5449 4341 4c0a 2727  ixin.VERTICAL.''
 00000540: 2756 6572 7469 6361 6c20 2831 2063 6f6c  'Vertical (1 col
 00000550: 756d 6e29 204c 6179 6f75 742e 0a27 2727  umn) Layout..'''
 00000560: 0a0a 6c6f 6767 6572 203d 206c 6f67 6769  ..logger = loggi
 00000570: 6e67 2e67 6574 4c6f 6767 6572 285f 5f6e  ng.getLogger(__n
 00000580: 616d 655f 5f29 0a0a 0a23 2055 7361 626c  ame__)...# Usabl
-00000590: 6520 5769 6467 6574 730a 0a0a 636c 6173  e Widgets...clas
-000005a0: 7320 526f 6f74 5769 6e64 6f77 2874 6b2e  s RootWindow(tk.
-000005b0: 546b 2c20 6d69 7869 6e2e 436f 6e74 6169  Tk, mixin.Contai
-000005c0: 6e65 7257 6964 6765 7429 3a0a 2020 2020  nerWidget):.    
-000005d0: 2727 2741 2072 6f6f 7420 7769 6e64 6f77  '''A root window
-000005e0: 2c20 7468 6520 746f 706c 6576 656c 2077  , the toplevel w
-000005f0: 6964 6765 7420 666f 7220 7468 6520 656e  idget for the en
-00000600: 7469 7265 2061 7070 6c69 6361 7469 6f6e  tire application
-00000610: 2e0a 0a20 2020 2055 7375 616c 6c79 2074  ...    Usually t
-00000620: 6865 7265 2773 206f 6e6c 7920 6f6e 6520  here's only one 
-00000630: 6f66 2074 6869 7320 696e 2061 2073 696e  of this in a sin
-00000640: 676c 6520 6170 706c 6963 6174 696f 6e2e  gle application.
-00000650: 204d 756c 7469 706c 6520 726f 6f74 0a20   Multiple root. 
-00000660: 2020 2077 696e 646f 7773 2061 7265 2075     windows are u
-00000670: 6e73 7570 706f 7274 6564 2e0a 0a20 2020  nsupported...   
-00000680: 2054 6865 2060 7365 7475 705f 696d 6167   The `setup_imag
-00000690: 6573 6020 6675 6e63 7469 6f6e 2063 616e  es` function can
-000006a0: 2062 6520 6f76 6572 7269 6465 6e20 746f   be overriden to
-000006b0: 206c 6f61 6420 616e 7920 6e75 6d62 6572   load any number
-000006c0: 206f 6620 696d 6167 6573 0a20 2020 2069   of images.    i
-000006d0: 6e20 616e 7920 7761 792e 2054 6865 2063  n any way. The c
-000006e0: 6f6d 6d6f 6e20 7573 6167 6520 6f66 206c  ommon usage of l
-000006f0: 6f61 6469 6e67 2061 6c6c 2069 6d61 6765  oading all image
-00000700: 7320 696e 2061 2066 6f6c 6465 7220 6973  s in a folder is
-00000710: 2073 7570 706f 7274 6564 0a20 2020 2064   supported.    d
-00000720: 6972 6563 746c 7920 7769 7468 2060 6069  irectly with ``i
-00000730: 6d67 666f 6c64 6572 6060 2e0a 0a20 2020  mgfolder``...   
-00000740: 2053 6565 2060 746b 696e 7465 722e 546b   See `tkinter.Tk
-00000750: 602e 0a0a 2020 2020 4172 6773 3a0a 2020  `...    Args:.  
-00000760: 2020 2020 2020 7468 656d 653a 2054 6865        theme: The
-00000770: 6d65 2074 6f20 7573 652e 2044 6566 6175  me to use. Defau
-00000780: 6c74 2074 6f20 6368 6f6f 7369 6e67 2061  lt to choosing a
-00000790: 2074 6173 7465 6675 6c20 6368 6f69 6365   tasteful choice
-000007a0: 2064 6570 656e 6469 6e67 206f 6e0a 2020   depending on.  
-000007b0: 2020 2020 2020 2020 2020 7468 6520 4f53            the OS
-000007c0: 2e0a 2020 2020 2020 2020 696d 6766 6f6c  ..        imgfol
-000007d0: 6465 723a 2046 6f6c 6465 7220 7769 7468  der: Folder with
-000007e0: 2069 6d61 6765 7320 746f 2062 6520 6c6f   images to be lo
-000007f0: 6164 6564 2028 7365 6520 6073 6574 7570  aded (see `setup
-00000800: 5f69 6d61 6765 735f 666f 6c64 6572 6029  _images_folder`)
-00000810: 2e20 4f70 7469 6f6e 616c 2e0a 0a20 2020  . Optional...   
-00000820: 204e 6f74 653a 0a20 2020 2020 2020 2054   Note:.        T
-00000830: 6563 686e 6963 616c 6c79 2c20 6974 2073  echnically, it s
-00000840: 686f 756c 6420 6265 204f 4b20 746f 2075  hould be OK to u
-00000850: 7365 206d 756c 7469 706c 6520 726f 6f74  se multiple root
-00000860: 2077 696e 646f 7773 2070 6572 2d70 726f   windows per-pro
-00000870: 6365 7373 2c0a 2020 2020 2020 2020 6275  cess,.        bu
-00000880: 7420 7468 6973 2068 6173 6e27 7420 6265  t this hasn't be
-00000890: 656e 2074 6573 7465 642c 2074 6865 7265  en tested, there
-000008a0: 2061 7265 206e 6f20 7465 7374 2063 6173   are no test cas
-000008b0: 6573 2077 6865 7265 2074 6869 7320 6d61  es where this ma
-000008c0: 6b65 730a 2020 2020 2020 2020 7365 6e73  kes.        sens
-000008d0: 652e 0a20 2020 2027 2727 0a20 2020 2069  e..    '''.    i
-000008e0: 734e 6f6e 6561 626c 653a 2062 6f6f 6c20  sNoneable: bool 
-000008f0: 3d20 4661 6c73 6520 2023 2041 6c77 6179  = False  # Alway
-00000900: 7320 7072 6573 656e 742c 206e 6f20 6d61  s present, no ma
-00000910: 7474 6572 2077 6861 740a 0a20 2020 2064  tter what..    d
-00000920: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00000930: 2c20 2a61 7267 732c 2074 6865 6d65 3a20  , *args, theme: 
-00000940: 7374 7220 3d20 4e6f 6e65 2c20 696d 6766  str = None, imgf
-00000950: 6f6c 6465 723a 2074 7970 696e 672e 4f70  older: typing.Op
-00000960: 7469 6f6e 616c 5b50 6174 685d 203d 204e  tional[Path] = N
-00000970: 6f6e 652c 202a 2a6b 7761 7267 7329 3a0a  one, **kwargs):.
-00000980: 2020 2020 2020 2020 7365 6c66 2e5f 6269          self._bi
-00000990: 6e64 696e 6773 5f67 6c6f 6261 6c3a 2074  ndings_global: t
-000009a0: 7970 696e 672e 4d75 7461 626c 654d 6170  yping.MutableMap
-000009b0: 7069 6e67 5b73 7472 2c20 6d6f 6465 6c2e  ping[str, model.
-000009c0: 4269 6e64 696e 6747 6c6f 6261 6c5d 203d  BindingGlobal] =
-000009d0: 207b 7d0a 2020 2020 2020 2020 7365 6c66   {}.        self
-000009e0: 2e69 6d61 6765 735f 6361 6368 653a 2074  .images_cache: t
-000009f0: 7970 696e 672e 4d75 7461 626c 654d 6170  yping.MutableMap
-00000a00: 7069 6e67 5b73 7472 2c20 6d6f 6465 6c2e  ping[str, model.
-00000a10: 496d 6167 6543 6163 6865 5d20 3d20 7b7d  ImageCache] = {}
-00000a20: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
-00000a30: 2e5f 5f69 6e69 745f 5f28 2920 2023 2074  .__init__()  # t
-00000a40: 6b2e 546b 0a20 2020 2020 2020 206b 7761  k.Tk.        kwa
-00000a50: 7267 735b 2765 7870 616e 6427 5d20 3d20  rgs['expand'] = 
-00000a60: 4661 6c73 6520 2023 2060 546f 706c 6576  False  # `Toplev
-00000a70: 656c 6020 6861 7320 6e6f 2070 6172 656e  el` has no paren
-00000a80: 7420 6772 6964 2074 6f20 6578 7061 6e64  t grid to expand
-00000a90: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-00000aa0: 7475 705f 696d 6167 6573 2869 6d67 666f  tup_images(imgfo
-00000ab0: 6c64 6572 2920 2023 2052 6567 6973 7465  lder)  # Registe
-00000ac0: 7220 616c 6c20 696d 6167 6573 2062 6566  r all images bef
-00000ad0: 6f72 6520 7468 6520 6368 696c 6420 7769  ore the child wi
-00000ae0: 6467 6574 7320 6172 6520 7365 7475 700a  dgets are setup.
-00000af0: 2020 2020 2020 2020 7365 6c66 2e69 6e69          self.ini
-00000b00: 745f 636f 6e74 6169 6e65 7228 2a61 7267  t_container(*arg
-00000b10: 732c 202a 2a6b 7761 7267 7329 0a20 2020  s, **kwargs).   
-00000b20: 2020 2020 2073 656c 662e 7374 796c 6520       self.style 
-00000b30: 3d20 7365 6c66 2e73 6574 7570 5f73 7479  = self.setup_sty
-00000b40: 6c65 2874 6865 6d65 290a 0a20 2020 2064  le(theme)..    d
-00000b50: 6566 2073 6574 7570 5f73 7479 6c65 2873  ef setup_style(s
-00000b60: 656c 662c 2074 6865 6d65 3a20 7479 7069  elf, theme: typi
-00000b70: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
-00000b80: 2920 2d3e 2074 746b 2e53 7479 6c65 3a0a  ) -> ttk.Style:.
-00000b90: 2020 2020 2020 2020 7374 796c 6520 3d20          style = 
-00000ba0: 7474 6b2e 5374 796c 6528 7365 6c66 290a  ttk.Style(self).
-00000bb0: 2020 2020 2020 2020 6966 2074 6865 6d65          if theme
-00000bc0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00000bd0: 2020 2020 2020 2320 476f 6f64 2066 6f72        # Good for
-00000be0: 204c 696e 7578 0a20 2020 2020 2020 2020   Linux.         
-00000bf0: 2020 2023 204f 6e20 5769 6e64 6f77 732c     # On Windows,
-00000c00: 2063 6865 636b 3a20 2777 696e 6e61 7469   check: 'winnati
-00000c10: 7665 272c 2027 7669 7374 6127 0a20 2020  ve', 'vista'.   
-00000c20: 2020 2020 2020 2020 2074 6865 6d65 203d           theme =
-00000c30: 2027 616c 7427 0a20 2020 2020 2020 2073   'alt'.        s
-00000c40: 7479 6c65 2e74 6865 6d65 5f75 7365 2874  tyle.theme_use(t
-00000c50: 6865 6d65 290a 2020 2020 2020 2020 7265  heme).        re
-00000c60: 7475 726e 2073 7479 6c65 0a0a 2020 2020  turn style..    
-00000c70: 6465 6620 7365 7475 705f 696d 6167 6573  def setup_images
-00000c80: 2873 656c 662c 2069 6d67 666f 6c64 6572  (self, imgfolder
-00000c90: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00000ca0: 6c5b 5061 7468 5d29 3a0a 2020 2020 2020  l[Path]):.      
-00000cb0: 2020 2727 2752 6567 6973 7465 7220 616c    '''Register al
-00000cc0: 6c20 696d 6167 6573 2068 6572 652e 0a0a  l images here...
-00000cd0: 2020 2020 2020 2020 5468 6973 2069 7320          This is 
-00000ce0: 6361 6c6c 6564 2062 6566 6f72 6520 7468  called before th
-00000cf0: 6520 6368 696c 6420 7769 6467 6574 7320  e child widgets 
-00000d00: 6172 6520 6465 6669 6e65 642e 0a0a 2020  are defined...  
-00000d10: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00000d20: 2020 2020 2020 2020 696d 6766 6f6c 6465          imgfolde
-00000d30: 723a 2046 6f6c 6465 7220 7769 7468 2069  r: Folder with i
-00000d40: 6d61 6765 7320 746f 2062 6520 6c6f 6164  mages to be load
-00000d50: 6564 2028 7573 696e 6720 6073 6574 7570  ed (using `setup
-00000d60: 5f69 6d61 6765 735f 666f 6c64 6572 6029  _images_folder`)
-00000d70: 2e20 4f70 7469 6f6e 616c 2e0a 2020 2020  . Optional..    
-00000d80: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-00000d90: 6966 2069 6d67 666f 6c64 6572 3a0a 2020  if imgfolder:.  
-00000da0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00000db0: 6574 7570 5f69 6d61 6765 735f 666f 6c64  etup_images_fold
-00000dc0: 6572 2869 6d67 666f 6c64 6572 290a 0a20  er(imgfolder).. 
-00000dd0: 2020 2040 6c72 755f 6361 6368 650a 2020     @lru_cache.  
-00000de0: 2020 6465 6620 7769 6d61 6765 2873 656c    def wimage(sel
-00000df0: 662c 206b 6579 3a20 7374 7229 202d 3e20  f, key: str) -> 
-00000e00: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00000e10: 746b 2e49 6d61 6765 5d3a 0a20 2020 2020  tk.Image]:.     
-00000e20: 2020 2027 2727 4765 7420 696d 6167 6520     '''Get image 
-00000e30: 6461 7461 2062 7920 6b65 792e 0a0a 2020  data by key...  
-00000e40: 2020 2020 2020 5468 6973 2066 756e 6374        This funct
-00000e50: 696f 6e20 7769 6c6c 2063 6163 6865 2074  ion will cache t
-00000e60: 6865 2069 6d61 6765 206f 626a 6563 742c  he image object,
-00000e70: 2073 6f20 6e6f 2065 7874 7261 2050 7974   so no extra Pyt
-00000e80: 686f 6e0a 2020 2020 2020 2020 7265 6665  hon.        refe
-00000e90: 7265 6e63 6573 2061 7265 206e 6565 6465  rences are neede
-00000ea0: 642e 2054 6865 2063 6163 6865 2077 696c  d. The cache wil
-00000eb0: 6c20 7374 6f72 6520 616c 6c20 7573 6564  l store all used
-00000ec0: 2069 6d61 6765 2c20 6176 6f69 640a 2020   image, avoid.  
-00000ed0: 2020 2020 2020 7275 6e61 7761 7920 6d65        runaway me
-00000ee0: 6d6f 7279 2063 6f6e 7375 6d70 7469 6f6e  mory consumption
-00000ef0: 2062 7920 7573 696e 6720 656e 6f72 6d6f   by using enormo
-00000f00: 7573 2061 6d6f 756e 7473 206f 6620 696d  us amounts of im
-00000f10: 6167 6573 2e0a 0a20 2020 2020 2020 2053  ages...        S
-00000f20: 6565 2050 7974 686f 6e20 646f 6375 6d65  ee Python docume
-00000f30: 6e74 6174 696f 6e20 666f 7220 6069 6d61  ntation for `ima
-00000f40: 6765 7320 3c68 7474 7073 3a2f 2f64 6f63  ges <https://doc
-00000f50: 732e 7079 7468 6f6e 2e6f 7267 2f33 2f6c  s.python.org/3/l
-00000f60: 6962 7261 7279 2f74 6b69 6e74 6572 2e68  ibrary/tkinter.h
-00000f70: 746d 6c23 696d 6167 6573 3e60 5f2e 0a0a  tml#images>`_...
-00000f80: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00000f90: 2020 2020 2020 2020 2020 6b65 793a 2054            key: T
-00000fa0: 6865 206b 6579 2074 6f20 6669 6e64 2074  he key to find t
-00000fb0: 6865 2069 6d61 6765 2064 6174 612e 0a0a  he image data...
-00000fc0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00000fd0: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
-00000fe0: 7468 6520 6b65 7920 6578 6973 7473 2c20  the key exists, 
-00000ff0: 7265 7475 726e 2074 6865 2060 746b 696e  return the `tkin
-00001000: 7465 722e 496d 6167 6560 206f 626a 6563  ter.Image` objec
-00001010: 742c 206f 7468 6572 7769 7365 0a20 2020  t, otherwise.   
-00001020: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00001030: 604e 6f6e 6560 2e0a 2020 2020 2020 2020  `None`..        
-00001040: 2727 270a 2020 2020 2020 2020 696f 626a  '''.        iobj
-00001050: 203d 2073 656c 662e 696d 6167 6573 5f63   = self.images_c
-00001060: 6163 6865 2e67 6574 286b 6579 290a 2020  ache.get(key).  
-00001070: 2020 2020 2020 6966 2069 6f62 6a20 6973        if iobj is
-00001080: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00001090: 2020 2069 6620 5f5f 6465 6275 675f 5f3a     if __debug__:
-000010a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000010b0: 2077 6172 6e69 6e67 732e 7761 726e 2866   warnings.warn(f
-000010c0: 274d 6973 7369 6e67 2069 6d61 6765 3a20  'Missing image: 
-000010d0: 7b6b 6579 7d27 2c20 7374 6163 6b6c 6576  {key}', stacklev
-000010e0: 656c 3d32 290a 2020 2020 2020 2020 2020  el=2).          
-000010f0: 2020 7265 7475 726e 204e 6f6e 650a 2020    return None.  
-00001100: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00001110: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
-00001120: 6f62 6a2e 6361 6368 6564 3a0a 2020 2020  obj.cached:.    
-00001130: 2020 2020 2020 2020 2020 2020 696d 675f              img_
-00001140: 6675 6e63 7469 6f6e 203d 2074 6b2e 5068  function = tk.Ph
-00001150: 6f74 6f49 6d61 6765 2020 2320 4465 6661  otoImage  # Defa
-00001160: 756c 7420 4675 6e63 7469 6f6e 0a20 2020  ult Function.   
-00001170: 2020 2020 2020 2020 2020 2020 2069 6d67               img
-00001180: 5f6b 7761 7267 733a 2074 7970 696e 672e  _kwargs: typing.
-00001190: 4469 6374 5b73 7472 2c20 7479 7069 6e67  Dict[str, typing
-000011a0: 2e41 6e79 5d20 3d20 7b7d 0a20 2020 2020  .Any] = {}.     
-000011b0: 2020 2020 2020 2020 2020 2069 6620 696f             if io
-000011c0: 626a 2e64 7479 7065 2061 6e64 2069 6f62  bj.dtype and iob
-000011d0: 6a2e 6474 7970 6520 696e 206d 6f64 656c  j.dtype in model
-000011e0: 2e49 4d41 4745 5f54 5950 4553 3a0a 2020  .IMAGE_TYPES:.  
-000011f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001200: 2020 696d 675f 6675 6e63 7469 6f6e 203d    img_function =
-00001210: 206d 6f64 656c 2e49 4d41 4745 5f54 5950   model.IMAGE_TYP
-00001220: 4553 5b69 6f62 6a2e 6474 7970 655d 0a20  ES[iobj.dtype]. 
-00001230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001240: 2020 2069 6d67 5f6b 7761 7267 735b 2766     img_kwargs['f
-00001250: 6f72 6d61 7427 5d20 3d20 696f 626a 2e64  ormat'] = iobj.d
-00001260: 7479 7065 0a20 2020 2020 2020 2020 2020  type.           
-00001270: 2020 2020 2023 204c 6f61 6420 7468 6520       # Load the 
-00001280: 696d 6167 650a 2020 2020 2020 2020 2020  image.          
-00001290: 2020 2020 2020 6966 2069 6f62 6a2e 666e        if iobj.fn
-000012a0: 616d 653a 0a20 2020 2020 2020 2020 2020  ame:.           
-000012b0: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-000012c0: 6465 6275 6728 6627 4c6f 6164 2049 6d61  debug(f'Load Ima
-000012d0: 6765 2022 7b6b 6579 7d22 2066 726f 6d20  ge "{key}" from 
-000012e0: 6669 6c65 2022 7b69 6f62 6a2e 666e 616d  file "{iobj.fnam
-000012f0: 657d 2227 290a 2020 2020 2020 2020 2020  e}"').          
-00001300: 2020 2020 2020 2020 2020 696f 626a 2e6f            iobj.o
-00001310: 626a 203d 2069 6d67 5f66 756e 6374 696f  bj = img_functio
-00001320: 6e28 6669 6c65 3d69 6f62 6a2e 666e 616d  n(file=iobj.fnam
-00001330: 652c 202a 2a69 6d67 5f6b 7761 7267 7329  e, **img_kwargs)
-00001340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001350: 2065 6c69 6620 696f 626a 2e64 6174 613a   elif iobj.data:
-00001360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001370: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-00001380: 6728 6627 4c6f 6164 2049 6d61 6765 2022  g(f'Load Image "
-00001390: 7b6b 6579 7d22 2066 726f 6d20 6461 7461  {key}" from data
-000013a0: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
-000013b0: 2020 2020 2020 2069 6f62 6a2e 6f62 6a20         iobj.obj 
-000013c0: 3d20 696d 675f 6675 6e63 7469 6f6e 2864  = img_function(d
-000013d0: 6174 613d 696f 626a 2e64 6174 612c 202a  ata=iobj.data, *
-000013e0: 2a69 6d67 5f6b 7761 7267 7329 0a20 2020  *img_kwargs).   
+00000590: 6520 5769 6467 6574 730a 0a23 2023 2043  e Widgets..# # C
+000005a0: 6f6e 7461 696e 6572 730a 0a0a 636c 6173  ontainers...clas
+000005b0: 7320 526f 6f74 5769 6e64 6f77 2874 6b2e  s RootWindow(tk.
+000005c0: 546b 2c20 6d69 7869 6e2e 436f 6e74 6169  Tk, mixin.Contai
+000005d0: 6e65 7257 6964 6765 7429 3a0a 2020 2020  nerWidget):.    
+000005e0: 2727 2741 2072 6f6f 7420 7769 6e64 6f77  '''A root window
+000005f0: 2c20 7468 6520 746f 706c 6576 656c 2077  , the toplevel w
+00000600: 6964 6765 7420 666f 7220 7468 6520 656e  idget for the en
+00000610: 7469 7265 2061 7070 6c69 6361 7469 6f6e  tire application
+00000620: 2e0a 0a20 2020 2055 7375 616c 6c79 2074  ...    Usually t
+00000630: 6865 7265 2773 206f 6e6c 7920 6f6e 6520  here's only one 
+00000640: 6f66 2074 6869 7320 696e 2061 2073 696e  of this in a sin
+00000650: 676c 6520 6170 706c 6963 6174 696f 6e2e  gle application.
+00000660: 204d 756c 7469 706c 6520 726f 6f74 0a20   Multiple root. 
+00000670: 2020 2077 696e 646f 7773 2061 7265 2075     windows are u
+00000680: 6e73 7570 706f 7274 6564 2e0a 0a20 2020  nsupported...   
+00000690: 2054 6865 2060 7365 7475 705f 696d 6167   The `setup_imag
+000006a0: 6573 6020 6675 6e63 7469 6f6e 2063 616e  es` function can
+000006b0: 2062 6520 6f76 6572 7269 6465 6e20 746f   be overriden to
+000006c0: 206c 6f61 6420 616e 7920 6e75 6d62 6572   load any number
+000006d0: 206f 6620 696d 6167 6573 0a20 2020 2069   of images.    i
+000006e0: 6e20 616e 7920 7761 792e 2054 6865 2063  n any way. The c
+000006f0: 6f6d 6d6f 6e20 7573 6167 6520 6f66 206c  ommon usage of l
+00000700: 6f61 6469 6e67 2061 6c6c 2069 6d61 6765  oading all image
+00000710: 7320 696e 2061 2066 6f6c 6465 7220 6973  s in a folder is
+00000720: 2073 7570 706f 7274 6564 0a20 2020 2064   supported.    d
+00000730: 6972 6563 746c 7920 7769 7468 2060 6069  irectly with ``i
+00000740: 6d67 666f 6c64 6572 6060 2e0a 0a20 2020  mgfolder``...   
+00000750: 204f 6e20 6465 6275 6720 6d6f 6465 2c20   On debug mode, 
+00000760: 7468 6973 2077 696c 6c20 7361 6e69 7479  this will sanity
+00000770: 2063 6865 636b 2074 6865 2065 6e74 6972   check the entir
+00000780: 6520 4755 492c 2062 7920 7265 6164 696e  e GUI, by readin
+00000790: 6720 6974 7320 7374 6174 652e 0a20 2020  g its state..   
+000007a0: 2054 6869 7320 646f 6573 6e27 7420 6861   This doesn't ha
+000007b0: 7070 656e 2069 6e20 7072 6f64 7563 7469  ppen in producti
+000007c0: 6f6e 2e0a 0a20 2020 2053 6565 2060 746b  on...    See `tk
+000007d0: 696e 7465 722e 546b 602e 0a0a 2020 2020  inter.Tk`...    
+000007e0: 4172 6773 3a0a 2020 2020 2020 2020 7468  Args:.        th
+000007f0: 656d 653a 2054 6865 6d65 2074 6f20 7573  eme: Theme to us
+00000800: 652e 2044 6566 6175 6c74 2074 6f20 6368  e. Default to ch
+00000810: 6f6f 7369 6e67 2061 2074 6173 7465 6675  oosing a tastefu
+00000820: 6c20 6368 6f69 6365 2064 6570 656e 6469  l choice dependi
+00000830: 6e67 206f 6e0a 2020 2020 2020 2020 2020  ng on.          
+00000840: 2020 7468 6520 4f53 2e0a 2020 2020 2020    the OS..      
+00000850: 2020 696d 6766 6f6c 6465 723a 2046 6f6c    imgfolder: Fol
+00000860: 6465 7220 7769 7468 2069 6d61 6765 7320  der with images 
+00000870: 746f 2062 6520 6c6f 6164 6564 2028 7365  to be loaded (se
+00000880: 6520 6073 6574 7570 5f69 6d61 6765 735f  e `setup_images_
+00000890: 666f 6c64 6572 6029 2e20 4f70 7469 6f6e  folder`). Option
+000008a0: 616c 2e0a 0a20 2020 204e 6f74 653a 0a20  al...    Note:. 
+000008b0: 2020 2020 2020 2054 6563 686e 6963 616c         Technical
+000008c0: 6c79 2c20 6974 2073 686f 756c 6420 6265  ly, it should be
+000008d0: 204f 4b20 746f 2075 7365 206d 756c 7469   OK to use multi
+000008e0: 706c 6520 726f 6f74 2077 696e 646f 7773  ple root windows
+000008f0: 2070 6572 2d70 726f 6365 7373 2c0a 2020   per-process,.  
+00000900: 2020 2020 2020 6275 7420 7468 6973 2068        but this h
+00000910: 6173 6e27 7420 6265 656e 2074 6573 7465  asn't been teste
+00000920: 642c 2074 6865 7265 2061 7265 206e 6f20  d, there are no 
+00000930: 7465 7374 2063 6173 6573 2077 6865 7265  test cases where
+00000940: 2074 6869 7320 6d61 6b65 730a 2020 2020   this makes.    
+00000950: 2020 2020 7365 6e73 652e 0a20 2020 2027      sense..    '
+00000960: 2727 0a20 2020 2069 734e 6f6e 6561 626c  ''.    isNoneabl
+00000970: 653a 2062 6f6f 6c20 3d20 4661 6c73 6520  e: bool = False 
+00000980: 2023 2041 6c77 6179 7320 7072 6573 656e   # Always presen
+00000990: 742c 206e 6f20 6d61 7474 6572 2077 6861  t, no matter wha
+000009a0: 740a 0a20 2020 2064 6566 205f 5f69 6e69  t..    def __ini
+000009b0: 745f 5f28 7365 6c66 2c20 2a61 7267 732c  t__(self, *args,
+000009c0: 2074 6865 6d65 3a20 7374 7220 3d20 4e6f   theme: str = No
+000009d0: 6e65 2c20 696d 6766 6f6c 6465 723a 2074  ne, imgfolder: t
+000009e0: 7970 696e 672e 4f70 7469 6f6e 616c 5b50  yping.Optional[P
+000009f0: 6174 685d 203d 204e 6f6e 652c 202a 2a6b  ath] = None, **k
+00000a00: 7761 7267 7329 3a0a 2020 2020 2020 2020  wargs):.        
+00000a10: 7365 6c66 2e5f 6269 6e64 696e 6773 5f67  self._bindings_g
+00000a20: 6c6f 6261 6c3a 2074 7970 696e 672e 4d75  lobal: typing.Mu
+00000a30: 7461 626c 654d 6170 7069 6e67 5b73 7472  tableMapping[str
+00000a40: 2c20 6d6f 6465 6c2e 4269 6e64 696e 6747  , model.BindingG
+00000a50: 6c6f 6261 6c5d 203d 207b 7d0a 2020 2020  lobal] = {}.    
+00000a60: 2020 2020 7365 6c66 2e69 6d61 6765 735f      self.images_
+00000a70: 6361 6368 653a 2074 7970 696e 672e 4d75  cache: typing.Mu
+00000a80: 7461 626c 654d 6170 7069 6e67 5b73 7472  tableMapping[str
+00000a90: 2c20 6d6f 6465 6c2e 496d 6167 6543 6163  , model.ImageCac
+00000aa0: 6865 5d20 3d20 7b7d 0a20 2020 2020 2020  he] = {}.       
+00000ab0: 2073 7570 6572 2829 2e5f 5f69 6e69 745f   super().__init_
+00000ac0: 5f28 2920 2023 2074 6b2e 546b 0a20 2020  _()  # tk.Tk.   
+00000ad0: 2020 2020 206b 7761 7267 735b 2765 7870       kwargs['exp
+00000ae0: 616e 6427 5d20 3d20 4661 6c73 6520 2023  and'] = False  #
+00000af0: 2060 546f 706c 6576 656c 6020 6861 7320   `Toplevel` has 
+00000b00: 6e6f 2070 6172 656e 7420 6772 6964 2074  no parent grid t
+00000b10: 6f20 6578 7061 6e64 0a20 2020 2020 2020  o expand.       
+00000b20: 2073 656c 662e 7365 7475 705f 696d 6167   self.setup_imag
+00000b30: 6573 2869 6d67 666f 6c64 6572 2920 2023  es(imgfolder)  #
+00000b40: 2052 6567 6973 7465 7220 616c 6c20 696d   Register all im
+00000b50: 6167 6573 2062 6566 6f72 6520 7468 6520  ages before the 
+00000b60: 6368 696c 6420 7769 6467 6574 7320 6172  child widgets ar
+00000b70: 6520 7365 7475 700a 2020 2020 2020 2020  e setup.        
+00000b80: 7365 6c66 2e69 6e69 745f 636f 6e74 6169  self.init_contai
+00000b90: 6e65 7228 2a61 7267 732c 202a 2a6b 7761  ner(*args, **kwa
+00000ba0: 7267 7329 0a20 2020 2020 2020 2073 656c  rgs).        sel
+00000bb0: 662e 7374 796c 6520 3d20 7365 6c66 2e73  f.style = self.s
+00000bc0: 6574 7570 5f73 7479 6c65 2874 6865 6d65  etup_style(theme
+00000bd0: 290a 2020 2020 2020 2020 6966 205f 5f64  ).        if __d
+00000be0: 6562 7567 5f5f 3a0a 2020 2020 2020 2020  ebug__:.        
+00000bf0: 2020 2020 696d 706f 7274 2074 7261 6365      import trace
+00000c00: 6261 636b 0a20 2020 2020 2020 2020 2020  back.           
+00000c10: 2069 6d70 6f72 7420 7379 730a 0a20 2020   import sys..   
+00000c20: 2020 2020 2020 2020 2064 6566 2073 616e           def san
+00000c30: 6974 795f 6368 6563 6b28 293a 0a20 2020  ity_check():.   
+00000c40: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+00000c50: 6765 722e 6465 6275 6728 273d 3e20 5361  ger.debug('=> Sa
+00000c60: 6e69 7479 2043 6865 636b 2047 5549 2053  nity Check GUI S
+00000c70: 7461 7465 2729 0a20 2020 2020 2020 2020  tate').         
+00000c80: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00000c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ca0: 7365 6c66 2e77 7374 6174 655f 6765 7428  self.wstate_get(
+00000cb0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00000cc0: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
+00000cd0: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
+00000ce0: 2020 2020 2020 2020 7472 6163 6562 6163          tracebac
+00000cf0: 6b2e 7072 696e 745f 6578 6328 290a 2020  k.print_exc().  
+00000d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d10: 2020 7379 732e 6578 6974 2831 3030 290a    sys.exit(100).
+00000d20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00000d30: 2e61 6674 6572 5f69 646c 6528 7361 6e69  .after_idle(sani
+00000d40: 7479 5f63 6865 636b 290a 0a20 2020 2064  ty_check)..    d
+00000d50: 6566 2073 6574 7570 5f73 7479 6c65 2873  ef setup_style(s
+00000d60: 656c 662c 2074 6865 6d65 3a20 7479 7069  elf, theme: typi
+00000d70: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
+00000d80: 2920 2d3e 2074 746b 2e53 7479 6c65 3a0a  ) -> ttk.Style:.
+00000d90: 2020 2020 2020 2020 7374 796c 6520 3d20          style = 
+00000da0: 7474 6b2e 5374 796c 6528 7365 6c66 290a  ttk.Style(self).
+00000db0: 2020 2020 2020 2020 6966 2074 6865 6d65          if theme
+00000dc0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00000dd0: 2020 2020 2020 2320 476f 6f64 2066 6f72        # Good for
+00000de0: 204c 696e 7578 0a20 2020 2020 2020 2020   Linux.         
+00000df0: 2020 2023 204f 6e20 5769 6e64 6f77 732c     # On Windows,
+00000e00: 2063 6865 636b 3a20 2777 696e 6e61 7469   check: 'winnati
+00000e10: 7665 272c 2027 7669 7374 6127 0a20 2020  ve', 'vista'.   
+00000e20: 2020 2020 2020 2020 2074 6865 6d65 203d           theme =
+00000e30: 2027 616c 7427 0a20 2020 2020 2020 2073   'alt'.        s
+00000e40: 7479 6c65 2e74 6865 6d65 5f75 7365 2874  tyle.theme_use(t
+00000e50: 6865 6d65 290a 2020 2020 2020 2020 7265  heme).        re
+00000e60: 7475 726e 2073 7479 6c65 0a0a 2020 2020  turn style..    
+00000e70: 6465 6620 7365 7475 705f 696d 6167 6573  def setup_images
+00000e80: 2873 656c 662c 2069 6d67 666f 6c64 6572  (self, imgfolder
+00000e90: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+00000ea0: 6c5b 5061 7468 5d29 3a0a 2020 2020 2020  l[Path]):.      
+00000eb0: 2020 2727 2752 6567 6973 7465 7220 616c    '''Register al
+00000ec0: 6c20 696d 6167 6573 2068 6572 652e 0a0a  l images here...
+00000ed0: 2020 2020 2020 2020 5468 6973 2069 7320          This is 
+00000ee0: 6361 6c6c 6564 2062 6566 6f72 6520 7468  called before th
+00000ef0: 6520 6368 696c 6420 7769 6467 6574 7320  e child widgets 
+00000f00: 6172 6520 6465 6669 6e65 642e 0a0a 2020  are defined...  
+00000f10: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+00000f20: 2020 2020 2020 2020 696d 6766 6f6c 6465          imgfolde
+00000f30: 723a 2046 6f6c 6465 7220 7769 7468 2069  r: Folder with i
+00000f40: 6d61 6765 7320 746f 2062 6520 6c6f 6164  mages to be load
+00000f50: 6564 2028 7573 696e 6720 6073 6574 7570  ed (using `setup
+00000f60: 5f69 6d61 6765 735f 666f 6c64 6572 6029  _images_folder`)
+00000f70: 2e20 4f70 7469 6f6e 616c 2e0a 2020 2020  . Optional..    
+00000f80: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+00000f90: 6966 2069 6d67 666f 6c64 6572 3a0a 2020  if imgfolder:.  
+00000fa0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00000fb0: 6574 7570 5f69 6d61 6765 735f 666f 6c64  etup_images_fold
+00000fc0: 6572 2869 6d67 666f 6c64 6572 290a 0a20  er(imgfolder).. 
+00000fd0: 2020 2040 6c72 755f 6361 6368 650a 2020     @lru_cache.  
+00000fe0: 2020 6465 6620 7769 6d61 6765 2873 656c    def wimage(sel
+00000ff0: 662c 206b 6579 3a20 7374 7229 202d 3e20  f, key: str) -> 
+00001000: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+00001010: 746b 2e49 6d61 6765 5d3a 0a20 2020 2020  tk.Image]:.     
+00001020: 2020 2027 2727 4765 7420 696d 6167 6520     '''Get image 
+00001030: 6461 7461 2062 7920 6b65 792e 0a0a 2020  data by key...  
+00001040: 2020 2020 2020 5468 6973 2066 756e 6374        This funct
+00001050: 696f 6e20 7769 6c6c 2063 6163 6865 2074  ion will cache t
+00001060: 6865 2069 6d61 6765 206f 626a 6563 742c  he image object,
+00001070: 2073 6f20 6e6f 2065 7874 7261 2050 7974   so no extra Pyt
+00001080: 686f 6e0a 2020 2020 2020 2020 7265 6665  hon.        refe
+00001090: 7265 6e63 6573 2061 7265 206e 6565 6465  rences are neede
+000010a0: 642e 2054 6865 2063 6163 6865 2077 696c  d. The cache wil
+000010b0: 6c20 7374 6f72 6520 616c 6c20 7573 6564  l store all used
+000010c0: 2069 6d61 6765 2c20 6176 6f69 640a 2020   image, avoid.  
+000010d0: 2020 2020 2020 7275 6e61 7761 7920 6d65        runaway me
+000010e0: 6d6f 7279 2063 6f6e 7375 6d70 7469 6f6e  mory consumption
+000010f0: 2062 7920 7573 696e 6720 656e 6f72 6d6f   by using enormo
+00001100: 7573 2061 6d6f 756e 7473 206f 6620 696d  us amounts of im
+00001110: 6167 6573 2e0a 0a20 2020 2020 2020 2053  ages...        S
+00001120: 6565 2050 7974 686f 6e20 646f 6375 6d65  ee Python docume
+00001130: 6e74 6174 696f 6e20 666f 7220 6069 6d61  ntation for `ima
+00001140: 6765 7320 3c68 7474 7073 3a2f 2f64 6f63  ges <https://doc
+00001150: 732e 7079 7468 6f6e 2e6f 7267 2f33 2f6c  s.python.org/3/l
+00001160: 6962 7261 7279 2f74 6b69 6e74 6572 2e68  ibrary/tkinter.h
+00001170: 746d 6c23 696d 6167 6573 3e60 5f2e 0a0a  tml#images>`_...
+00001180: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00001190: 2020 2020 2020 2020 2020 6b65 793a 2054            key: T
+000011a0: 6865 206b 6579 2074 6f20 6669 6e64 2074  he key to find t
+000011b0: 6865 2069 6d61 6765 2064 6174 612e 0a0a  he image data...
+000011c0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+000011d0: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
+000011e0: 7468 6520 6b65 7920 6578 6973 7473 2c20  the key exists, 
+000011f0: 7265 7475 726e 2074 6865 2060 6074 6b69  return the ``tki
+00001200: 6e74 6572 2e49 6d61 6765 6060 206f 626a  nter.Image`` obj
+00001210: 6563 742c 206f 7468 6572 7769 7365 0a20  ect, otherwise. 
+00001220: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00001230: 6e20 604e 6f6e 6560 2e0a 2020 2020 2020  n `None`..      
+00001240: 2020 2727 270a 2020 2020 2020 2020 696f    '''.        io
+00001250: 626a 203d 2073 656c 662e 696d 6167 6573  bj = self.images
+00001260: 5f63 6163 6865 2e67 6574 286b 6579 290a  _cache.get(key).
+00001270: 2020 2020 2020 2020 6966 2069 6f62 6a20          if iobj 
+00001280: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00001290: 2020 2020 2069 6620 5f5f 6465 6275 675f       if __debug_
+000012a0: 5f3a 0a20 2020 2020 2020 2020 2020 2020  _:.             
+000012b0: 2020 2077 6172 6e69 6e67 732e 7761 726e     warnings.warn
+000012c0: 2866 274d 6973 7369 6e67 2069 6d61 6765  (f'Missing image
+000012d0: 3a20 7b6b 6579 7d27 2c20 7374 6163 6b6c  : {key}', stackl
+000012e0: 6576 656c 3d32 290a 2020 2020 2020 2020  evel=2).        
+000012f0: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
+00001300: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00001310: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+00001320: 2069 6f62 6a2e 6361 6368 6564 3a0a 2020   iobj.cached:.  
+00001330: 2020 2020 2020 2020 2020 2020 2020 696d                im
+00001340: 675f 6675 6e63 7469 6f6e 203d 2074 6b2e  g_function = tk.
+00001350: 5068 6f74 6f49 6d61 6765 2020 2320 4465  PhotoImage  # De
+00001360: 6661 756c 7420 4675 6e63 7469 6f6e 0a20  fault Function. 
+00001370: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00001380: 6d67 5f6b 7761 7267 733a 2074 7970 696e  mg_kwargs: typin
+00001390: 672e 4469 6374 5b73 7472 2c20 7479 7069  g.Dict[str, typi
+000013a0: 6e67 2e41 6e79 5d20 3d20 7b7d 0a20 2020  ng.Any] = {}.   
+000013b0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000013c0: 696f 626a 2e64 7479 7065 2061 6e64 2069  iobj.dtype and i
+000013d0: 6f62 6a2e 6474 7970 6520 696e 206d 6f64  obj.dtype in mod
+000013e0: 656c 2e49 4d41 4745 5f54 5950 4553 3a0a  el.IMAGE_TYPES:.
 000013f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001400: 2023 2054 4f44 4f3a 2052 656d 6f76 6520   # TODO: Remove 
-00001410: 7468 6520 6461 7461 2063 6f70 793a 2060  the data copy: `
-00001420: 696f 626a 2e64 6174 6120 3d20 4e6f 6e65  iobj.data = None
-00001430: 600a 2020 2020 2020 2020 2020 2020 2020  `.              
-00001440: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00001450: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00001460: 6520 5661 6c75 6545 7272 6f72 2866 2749  e ValueError(f'I
-00001470: 6e76 616c 6964 2043 6163 6865 204d 6574  nvalid Cache Met
-00001480: 6164 6174 6120 666f 7220 496d 6167 6520  adata for Image 
-00001490: 7b6b 6579 7d27 290a 2020 2020 2020 2020  {key}').        
-000014a0: 2020 2020 7265 7475 726e 2069 6f62 6a2e      return iobj.
-000014b0: 6f62 6a0a 0a20 2020 2064 6566 2069 6e73  obj..    def ins
-000014c0: 7461 7465 2873 656c 662c 2073 7461 7465  tate(self, state
-000014d0: 7370 6563 3a20 7479 7069 6e67 2e53 6571  spec: typing.Seq
-000014e0: 7565 6e63 655b 7374 725d 2c20 6361 6c6c  uence[str], call
-000014f0: 6261 636b 3a20 7479 7069 6e67 2e4f 7074  back: typing.Opt
-00001500: 696f 6e61 6c5b 7479 7069 6e67 2e43 616c  ional[typing.Cal
-00001510: 6c61 626c 655d 203d 204e 6f6e 6529 202d  lable] = None) -
-00001520: 3e20 7479 7069 6e67 2e4f 7074 696f 6e61  > typing.Optiona
-00001530: 6c5b 626f 6f6c 5d3a 0a20 2020 2020 2020  l[bool]:.       
-00001540: 2027 2727 2727 2720 2023 2044 6f20 6e6f   ''''''  # Do no
-00001550: 7420 646f 6375 6d65 6e74 0a20 2020 2020  t document.     
-00001560: 2020 2023 204e 6f74 2061 7070 6c69 6361     # Not applica
-00001570: 626c 6520 746f 2074 6865 2072 6f6f 7420  ble to the root 
-00001580: 7769 6e64 6f77 0a20 2020 2020 2020 2072  window.        r
-00001590: 6574 7572 6e20 4e6f 6e65 0a0a 2020 2020  eturn None..    
-000015a0: 6465 6620 7374 6174 6528 7365 6c66 2c20  def state(self, 
-000015b0: 7374 6174 6573 7065 6329 3a0a 2020 2020  statespec):.    
-000015c0: 2020 2020 2727 2727 2727 2020 2320 446f      ''''''  # Do
-000015d0: 206e 6f74 2064 6f63 756d 656e 740a 2020   not document.  
-000015e0: 2020 2020 2020 2320 4e6f 7420 6170 706c        # Not appl
-000015f0: 6963 6162 6c65 2074 6f20 726f 6f74 2077  icable to root w
-00001600: 696e 646f 770a 2020 2020 2020 2020 7261  indow.        ra
-00001610: 6973 6520 4e6f 7449 6d70 6c65 6d65 6e74  ise NotImplement
-00001620: 6564 4572 726f 720a 0a20 2020 2064 6566  edError..    def
-00001630: 2067 6269 6e64 696e 6728 7365 6c66 2c20   gbinding(self, 
-00001640: 2a61 7267 732c 2069 6d6d 6564 6961 7465  *args, immediate
-00001650: 3a20 626f 6f6c 203d 2054 7275 652c 202a  : bool = True, *
-00001660: 2a6b 7761 7267 7329 202d 3e20 6d6f 6465  *kwargs) -> mode
-00001670: 6c2e 4269 6e64 696e 6747 6c6f 6261 6c3a  l.BindingGlobal:
-00001680: 0a20 2020 2020 2020 2027 2727 4372 6561  .        '''Crea
-00001690: 7465 2061 2060 6d6f 6465 6c2e 4269 6e64  te a `model.Bind
-000016a0: 696e 6747 6c6f 6261 6c60 2066 6f72 2074  ingGlobal` for t
-000016b0: 6869 7320 6170 706c 6963 6174 696f 6e2e  his application.
-000016c0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-000016d0: 2020 2020 2020 2020 2020 2020 696d 6d65              imme
-000016e0: 6469 6174 653a 2050 6173 7365 6420 746f  diate: Passed to
-000016f0: 2074 6865 2075 7073 7472 6561 6d20 6f62   the upstream ob
-00001700: 6a65 6374 2c20 6465 6661 756c 7420 746f  ject, default to
-00001710: 2065 6e61 626c 696e 6720 7468 650a 2020   enabling the.  
-00001720: 2020 2020 2020 2020 2020 2020 2020 6269                bi
-00001730: 6e64 696e 6720 6f6e 2063 7265 6174 696f  nding on creatio
-00001740: 6e2e 2054 6869 7320 6973 2074 6865 206f  n. This is the o
-00001750: 7070 6f73 6974 6520 6672 6f6d 2075 7073  pposite from ups
-00001760: 7472 6561 6d2e 0a0a 2020 2020 2020 2020  tream...        
-00001770: 416c 6c20 6172 6775 6d65 6e74 7320 6172  All arguments ar
-00001780: 6520 7061 7373 6564 2074 6f20 7468 6520  e passed to the 
-00001790: 606d 6f64 656c 2e42 696e 6469 6e67 476c  `model.BindingGl
-000017a0: 6f62 616c 6020 6f62 6a65 6374 2e0a 2020  obal` object..  
-000017b0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-000017c0: 2020 7265 7475 726e 206d 6f64 656c 2e42    return model.B
-000017d0: 696e 6469 6e67 476c 6f62 616c 2873 656c  indingGlobal(sel
-000017e0: 662c 202a 6172 6773 2c20 696d 6d65 6469  f, *args, immedi
-000017f0: 6174 653d 696d 6d65 6469 6174 652c 202a  ate=immediate, *
-00001800: 2a6b 7761 7267 7329 0a0a 2020 2020 6465  *kwargs)..    de
-00001810: 6620 7365 7475 705f 696d 6167 655f 6461  f setup_image_da
-00001820: 7461 2873 656c 662c 206b 6579 3a20 7374  ta(self, key: st
-00001830: 722c 2064 6174 613a 2062 7974 6573 2c20  r, data: bytes, 
-00001840: 6474 7970 653a 2073 7472 2c20 2a2c 2063  dtype: str, *, c
-00001850: 6163 6865 5f63 6c65 6172 3a20 626f 6f6c  ache_clear: bool
-00001860: 203d 2054 7275 6529 202d 3e20 4e6f 6e65   = True) -> None
-00001870: 3a0a 2020 2020 2020 2020 2727 2752 6567  :.        '''Reg
-00001880: 6973 7465 7220 6120 7369 6e67 6c65 2069  ister a single i
-00001890: 6d61 6765 2c20 6672 6f6d 2061 7262 6974  mage, from arbit
-000018a0: 7261 7279 2064 6174 612e 0a0a 2020 2020  rary data...    
-000018b0: 2020 2020 5468 6973 2069 7320 7573 6566      This is usef
-000018c0: 756c 2074 6f20 6176 6f69 6420 6578 7465  ul to avoid exte
-000018d0: 726e 616c 2069 6d61 6765 2066 696c 6573  rnal image files
-000018e0: 2061 6e64 2068 6172 6463 6f64 6520 616c   and hardcode al
-000018f0: 6c20 696d 6167 650a 2020 2020 2020 2020  l image.        
-00001900: 6461 7461 206f 6e20 7468 6520 6269 6e61  data on the bina
-00001910: 7279 2069 7473 656c 662e 0a0a 2020 2020  ry itself...    
-00001920: 2020 2020 5468 6520 6461 7461 2063 616e      The data can
-00001930: 2062 6520 6769 7665 6e20 6173 2061 2062   be given as a b
-00001940: 6173 6536 3420 6279 7465 2073 7472 696e  ase64 byte strin
-00001950: 672e 2054 6869 7320 6361 6e20 6265 2063  g. This can be c
-00001960: 6f6d 7075 7465 640a 2020 2020 2020 2020  omputed.        
-00001970: 6672 6f6d 2061 2066 696c 6520 6060 2449  from a file ``$I
-00001980: 4d41 4745 6060 2075 7369 6e67 2074 6865  MAGE`` using the
-00001990: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
-000019a0: 6e64 0a0a 2020 2020 2020 2020 2e2e 2063  nd..        .. c
-000019b0: 6f64 653a 3a20 7368 656c 6c0a 0a20 2020  ode:: shell..   
-000019c0: 2020 2020 2020 2020 2062 6173 6536 3420           base64 
-000019d0: 2d2d 7772 6170 3d30 203c 2224 494d 4147  --wrap=0 <"$IMAG
-000019e0: 4522 0a0a 2020 2020 2020 2020 4172 6773  E"..        Args
-000019f0: 3a0a 2020 2020 2020 2020 2020 2020 6b65  :.            ke
-00001a00: 793a 2054 6865 206b 6579 2074 6f20 7374  y: The key to st
-00001a10: 6f72 6520 7468 6520 696d 6167 6520 756e  ore the image un
-00001a20: 6465 720a 2020 2020 2020 2020 2020 2020  der.            
-00001a30: 6461 7461 3a20 5468 6520 696d 6167 6520  data: The image 
-00001a40: 6461 7461 2c20 6173 2062 7974 6573 2e0a  data, as bytes..
-00001a50: 2020 2020 2020 2020 2020 2020 6474 7970              dtyp
-00001a60: 653a 2054 6865 2069 6d61 6765 2066 6f72  e: The image for
-00001a70: 6d61 742e 204f 6e6c 7920 6074 6b69 6e74  mat. Only `tkint
-00001a80: 6572 6020 7375 7070 6f72 7465 6420 696d  er` supported im
-00001a90: 6167 6573 2e0a 0a20 2020 2020 2020 2020  ages...         
-00001aa0: 2020 2063 6163 6865 5f63 6c65 6172 3a20     cache_clear: 
-00001ab0: 436c 6561 7220 7468 6520 696d 6167 6520  Clear the image 
-00001ac0: 6361 6368 6520 6166 7465 7220 7265 6769  cache after regi
-00001ad0: 7374 6572 2074 6865 7365 206e 6577 2069  ster these new i
-00001ae0: 6d61 6765 2e0a 2020 2020 2020 2020 2020  mage..          
-00001af0: 2020 2020 2020 4465 6661 756c 7420 746f        Default to
-00001b00: 2060 5472 7565 602e 0a0a 2020 2020 2020   `True`...      
-00001b10: 2020 5365 6520 416c 736f 3a0a 2020 2020    See Also:.    
-00001b20: 2020 2020 2020 2020 2d20 6073 6574 7570          - `setup
-00001b30: 5f69 6d61 6765 735f 666f 6c64 6572 603a  _images_folder`:
-00001b40: 2052 6567 6973 7465 7220 7365 7665 7261   Register severa
-00001b50: 6c20 696d 6167 6573 2066 726f 6d20 6120  l images from a 
-00001b60: 666f 6c64 6572 2e0a 2020 2020 2020 2020  folder..        
-00001b70: 2020 2020 2d20 6077 696d 6167 6560 3a20      - `wimage`: 
-00001b80: 4765 7420 7468 6520 6c6f 6164 6564 2069  Get the loaded i
-00001b90: 6d61 6765 2064 6174 612e 0a20 2020 2020  mage data..     
-00001ba0: 2020 2027 2727 0a20 2020 2020 2020 2069     '''.        i
-00001bb0: 6620 6b65 7920 696e 2073 656c 662e 696d  f key in self.im
-00001bc0: 6167 6573 5f63 6163 6865 3a0a 2020 2020  ages_cache:.    
-00001bd0: 2020 2020 2020 2020 7261 6973 6520 6578          raise ex
-00001be0: 6365 7074 696f 6e2e 496e 7661 6c69 6449  ception.InvalidI
-00001bf0: 6d61 6765 4b65 7928 6b65 7929 0a20 2020  mageKey(key).   
-00001c00: 2020 2020 2069 6620 6474 7970 6520 6e6f       if dtype no
-00001c10: 7420 696e 206d 6f64 656c 2e49 4d41 4745  t in model.IMAGE
-00001c20: 5f54 5950 4553 3a0a 2020 2020 2020 2020  _TYPES:.        
-00001c30: 2020 2020 7261 6973 6520 6578 6365 7074      raise except
-00001c40: 696f 6e2e 496e 7661 6c69 6449 6d61 6765  ion.InvalidImage
-00001c50: 5479 7065 2864 7479 7065 290a 2020 2020  Type(dtype).    
-00001c60: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-00001c70: 2866 2752 6567 6973 7465 7220 7b64 7479  (f'Register {dty
-00001c80: 7065 2e75 7070 6572 2829 7d20 496d 6167  pe.upper()} Imag
-00001c90: 6520 227b 6b65 797d 2227 290a 2020 2020  e "{key}"').    
-00001ca0: 2020 2020 7365 6c66 2e69 6d61 6765 735f      self.images_
-00001cb0: 6361 6368 655b 6b65 795d 203d 206d 6f64  cache[key] = mod
-00001cc0: 656c 2e49 6d61 6765 4361 6368 6528 6461  el.ImageCache(da
-00001cd0: 7461 3d64 6174 612c 2064 7479 7065 3d64  ta=data, dtype=d
-00001ce0: 7479 7065 290a 2020 2020 2020 2020 6966  type).        if
-00001cf0: 2063 6163 6865 5f63 6c65 6172 3a0a 2020   cache_clear:.  
-00001d00: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
-00001d10: 696d 6167 652e 6361 6368 655f 636c 6561  image.cache_clea
-00001d20: 7228 290a 0a20 2020 2023 2054 4f44 4f3a  r()..    # TODO:
-00001d30: 2053 7570 706f 7274 206c 6f61 6469 6e67   Support loading
-00001d40: 2061 6c6c 2069 6d61 6765 7320 7269 6768   all images righ
-00001d50: 7420 6865 7265 2c20 6e6f 206c 617a 7920  t here, no lazy 
-00001d60: 6c6f 6164 696e 673f 0a20 2020 2064 6566  loading?.    def
-00001d70: 2073 6574 7570 5f69 6d61 6765 735f 666f   setup_images_fo
-00001d80: 6c64 6572 2873 656c 662c 2066 6f6c 6465  lder(self, folde
-00001d90: 723a 2050 6174 682c 202a 2c20 6361 6368  r: Path, *, cach
-00001da0: 655f 636c 6561 723a 2062 6f6f 6c20 3d20  e_clear: bool = 
-00001db0: 5472 7565 2920 2d3e 204e 6f6e 653a 0a20  True) -> None:. 
-00001dc0: 2020 2020 2020 2027 2727 5265 6769 7374         '''Regist
-00001dd0: 6572 2061 6c6c 2073 7570 706f 7274 6564  er all supported
-00001de0: 2069 6d61 6765 7320 6672 6f6d 2061 2066   images from a f
-00001df0: 6f6c 6465 722e 0a0a 2020 2020 2020 2020  older...        
-00001e00: 5265 6769 7374 6572 7320 616c 6c20 7375  Registers all su
-00001e10: 7070 6f72 7465 6420 696d 6167 6573 206f  pported images o
-00001e20: 6e20 7468 6520 6769 7665 6e20 666f 6c64  n the given fold
-00001e30: 6572 2c20 646f 6573 206e 6f74 2072 6563  er, does not rec
-00001e40: 7572 7365 0a20 2020 2020 2020 2069 6e74  urse.        int
-00001e50: 6f20 7375 6266 6f6c 6465 7273 2e20 556e  o subfolders. Un
-00001e60: 7375 7070 6f72 7465 6420 6669 6c65 2065  supported file e
-00001e70: 7874 656e 7369 6f6e 7320 6172 6520 736b  xtensions are sk
-00001e80: 6970 7065 642e 0a0a 2020 2020 2020 2020  ipped...        
-00001e90: 5468 6520 6b65 7920 666f 7220 6669 6e64  The key for find
-00001ea0: 696e 6720 7468 6520 696d 6167 6573 2069  ing the images i
-00001eb0: 7320 7468 6520 6669 6c65 206e 616d 652c  s the file name,
-00001ec0: 2077 6974 686f 7574 2074 6865 206c 6173   without the las
-00001ed0: 740a 2020 2020 2020 2020 6578 7465 6e73  t.        extens
-00001ee0: 696f 6e2e 204d 756c 7469 706c 6520 696d  ion. Multiple im
-00001ef0: 6167 6573 2077 6974 6820 7468 6520 7361  ages with the sa
-00001f00: 6d65 206b 6579 2061 6e64 2064 6966 6665  me key and diffe
-00001f10: 7265 6e74 2065 7874 656e 7369 6f6e 730a  rent extensions.
-00001f20: 2020 2020 2020 2020 6172 6520 756e 7375          are unsu
-00001f30: 7070 6f72 7465 642e 0a0a 2020 2020 2020  pported...      
-00001f40: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00001f50: 2020 2020 666f 6c64 6572 3a20 5468 6520      folder: The 
-00001f60: 736f 7572 6365 2066 6f6c 6465 722e 204f  source folder. O
-00001f70: 7074 696f 6e61 6c2e 0a20 2020 2020 2020  ptional..       
-00001f80: 2020 2020 2063 6163 6865 5f63 6c65 6172       cache_clear
-00001f90: 3a20 436c 6561 7220 7468 6520 696d 6167  : Clear the imag
-00001fa0: 6520 6361 6368 6520 6166 7465 7220 7265  e cache after re
-00001fb0: 6769 7374 6572 2074 6865 7365 206e 6577  gister these new
-00001fc0: 2069 6d61 6765 732e 0a20 2020 2020 2020   images..       
-00001fd0: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
-00001fe0: 2074 6f20 6054 7275 6560 2e0a 0a20 2020   to `True`...   
-00001ff0: 2020 2020 2053 6565 2041 6c73 6f3a 0a20       See Also:. 
-00002000: 2020 2020 2020 2020 2020 202d 2060 7365             - `se
-00002010: 7475 705f 696d 6167 655f 6461 7461 603a  tup_image_data`:
-00002020: 2052 6567 6973 7465 7220 6120 7369 6e67   Register a sing
-00002030: 6c65 2069 6d61 6765 2066 726f 6d20 7261  le image from ra
-00002040: 7720 6461 7461 2e0a 2020 2020 2020 2020  w data..        
-00002050: 2020 2020 2d20 6077 696d 6167 6560 3a20      - `wimage`: 
-00002060: 4765 7420 7468 6520 6c6f 6164 6564 2069  Get the loaded i
-00002070: 6d61 6765 2064 6174 612e 0a20 2020 2020  mage data..     
-00002080: 2020 2027 2727 0a20 2020 2020 2020 2069     '''.        i
-00002090: 6620 6e6f 7420 666f 6c64 6572 2e69 735f  f not folder.is_
-000020a0: 6469 7228 293a 0a20 2020 2020 2020 2020  dir():.         
-000020b0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-000020c0: 726f 7228 6627 496e 7661 6c69 6420 466f  ror(f'Invalid Fo
-000020d0: 6c64 6572 3a20 7b66 6f6c 6465 727d 2729  lder: {folder}')
-000020e0: 0a20 2020 2020 2020 2066 6f72 2069 6d67  .        for img
-000020f0: 6669 6c65 2069 6e20 666f 6c64 6572 2e69  file in folder.i
-00002100: 7465 7264 6972 2829 3a0a 2020 2020 2020  terdir():.      
-00002110: 2020 2020 2020 696d 6765 7874 203d 2069        imgext = i
-00002120: 6d67 6669 6c65 2e73 7566 6669 780a 2020  mgfile.suffix.  
-00002130: 2020 2020 2020 2020 2020 6474 7970 6520            dtype 
-00002140: 3d20 4e6f 6e65 2069 6620 696d 6765 7874  = None if imgext
-00002150: 203d 3d20 2727 2065 6c73 6520 696d 6765   == '' else imge
-00002160: 7874 5b31 3a5d 2e6c 6f77 6572 2829 0a20  xt[1:].lower(). 
-00002170: 2020 2020 2020 2020 2020 2069 6620 696d             if im
-00002180: 6766 696c 652e 6973 5f66 696c 6528 2920  gfile.is_file() 
-00002190: 616e 6420 6474 7970 6520 696e 206d 6f64  and dtype in mod
-000021a0: 656c 2e49 4d41 4745 5f54 5950 4553 3a0a  el.IMAGE_TYPES:.
-000021b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021c0: 696d 676b 6579 203d 2069 6d67 6669 6c65  imgkey = imgfile
-000021d0: 2e73 7465 6d0a 2020 2020 2020 2020 2020  .stem.          
-000021e0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-000021f0: 7567 2866 2752 6567 6973 7465 7220 7b64  ug(f'Register {d
-00002200: 7479 7065 2e75 7070 6572 2829 7d20 496d  type.upper()} Im
-00002210: 6167 6520 227b 696d 676b 6579 7d22 3a20  age "{imgkey}": 
-00002220: 227b 696d 6766 696c 657d 2227 290a 2020  "{imgfile}"').  
-00002230: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00002240: 2069 6d67 6b65 7920 696e 2073 656c 662e   imgkey in self.
-00002250: 696d 6167 6573 5f63 6163 6865 3a0a 2020  images_cache:.  
-00002260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002270: 2020 7261 6973 6520 6578 6365 7074 696f    raise exceptio
-00002280: 6e2e 496e 7661 6c69 6449 6d61 6765 4b65  n.InvalidImageKe
-00002290: 7928 696d 676b 6579 290a 2020 2020 2020  y(imgkey).      
-000022a0: 2020 2020 2020 2020 2020 6966 2064 7479            if dty
-000022b0: 7065 206e 6f74 2069 6e20 6d6f 6465 6c2e  pe not in model.
-000022c0: 494d 4147 455f 5459 5045 533a 0a20 2020  IMAGE_TYPES:.   
-000022d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022e0: 2072 6169 7365 2065 7863 6570 7469 6f6e   raise exception
-000022f0: 2e49 6e76 616c 6964 496d 6167 6554 7970  .InvalidImageTyp
-00002300: 6528 6474 7970 6529 0a20 2020 2020 2020  e(dtype).       
-00002310: 2020 2020 2020 2020 2073 656c 662e 696d           self.im
-00002320: 6167 6573 5f63 6163 6865 5b69 6d67 6b65  ages_cache[imgke
-00002330: 795d 203d 206d 6f64 656c 2e49 6d61 6765  y] = model.Image
-00002340: 4361 6368 6528 666e 616d 653d 696d 6766  Cache(fname=imgf
-00002350: 696c 652c 2064 7479 7065 3d64 7479 7065  ile, dtype=dtype
-00002360: 290a 2020 2020 2020 2020 6966 2063 6163  ).        if cac
-00002370: 6865 5f63 6c65 6172 3a0a 2020 2020 2020  he_clear:.      
-00002380: 2020 2020 2020 7365 6c66 2e77 696d 6167        self.wimag
-00002390: 652e 6361 6368 655f 636c 6561 7228 290a  e.cache_clear().
-000023a0: 0a0a 636c 6173 7320 4672 616d 6555 6e6c  ..class FrameUnl
-000023b0: 6162 656c 6c65 6428 7474 6b2e 4672 616d  abelled(ttk.Fram
-000023c0: 652c 206d 6978 696e 2e43 6f6e 7461 696e  e, mixin.Contain
-000023d0: 6572 5769 6467 6574 293a 0a20 2020 2027  erWidget):.    '
-000023e0: 2727 4120 7369 6d70 6c65 2066 7261 6d65  ''A simple frame
-000023f0: 2074 6f20 686f 6c64 206f 7468 6572 2077   to hold other w
-00002400: 6964 6765 7473 2c20 7669 7375 616c 6c79  idgets, visually
-00002410: 2069 6e76 6973 6962 6c65 2e0a 0a20 2020   invisible...   
-00002420: 2054 6869 7320 6973 2074 6865 2073 696d   This is the sim
-00002430: 706c 6573 7420 666f 726d 206f 6620 606d  plest form of `m
-00002440: 6978 696e 2e43 6f6e 7461 696e 6572 5769  ixin.ContainerWi
-00002450: 6467 6574 602c 206a 7573 7420 6120 6275  dget`, just a bu
-00002460: 6e63 6820 6f66 0a20 2020 2077 6964 6765  nch of.    widge
-00002470: 7473 2e20 5468 6572 6527 7320 6e6f 2073  ts. There's no s
-00002480: 6570 6172 6174 696f 6e20 6265 7477 6565  eparation betwee
-00002490: 6e20 7468 6520 6f75 7473 6964 6520 616e  n the outside an
-000024a0: 6420 7468 6520 696e 7369 6465 206f 6620  d the inside of 
-000024b0: 7468 650a 2020 2020 6672 616d 652e 0a0a  the.    frame...
-000024c0: 2020 2020 5468 6572 6520 6973 206e 6f20      There is no 
-000024d0: 5079 7468 6f6e 2064 6f63 756d 656e 7461  Python documenta
-000024e0: 7469 6f6e 2c20 7365 6520 6060 546b 6060  tion, see ``Tk``
-000024f0: 2060 7474 6b2e 4672 616d 6520 3c68 7474   `ttk.Frame <htt
-00002500: 7073 3a2f 2f77 7777 2e74 636c 2e74 6b2f  ps://www.tcl.tk/
-00002510: 6d61 6e2f 7463 6c2f 546b 436d 642f 7474  man/tcl/TkCmd/tt
-00002520: 6b5f 6672 616d 652e 6874 6d6c 3e60 5f20  k_frame.html>`_ 
-00002530: 646f 6375 6d65 6e74 6174 696f 6e2e 0a0a  documentation...
-00002540: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00002550: 2020 7061 7265 6e74 3a20 5468 6520 7061    parent: The pa
-00002560: 7265 6e74 2077 6964 6765 742e 2043 616e  rent widget. Can
-00002570: 2062 6520 6120 6052 6f6f 7457 696e 646f   be a `RootWindo
-00002580: 7760 206f 7220 616e 6f74 6865 7220 606d  w` or another `m
-00002590: 6978 696e 2e43 6f6e 7461 696e 6572 5769  ixin.ContainerWi
-000025a0: 6467 6574 602e 0a0a 2020 2020 5365 6520  dget`...    See 
-000025b0: 416c 736f 3a0a 2020 2020 2020 2020 6046  Also:.        `F
-000025c0: 7261 6d65 4c61 6265 6c6c 6564 603a 2056  rameLabelled`: V
-000025d0: 6973 6962 6c65 2076 6572 7369 6f6e 2c20  isible version, 
-000025e0: 7769 7468 2061 206c 6162 656c 2e0a 2020  with a label..  
-000025f0: 2020 2727 270a 2020 2020 6465 6620 5f5f    '''.    def __
-00002600: 696e 6974 5f5f 2873 656c 662c 2070 6172  init__(self, par
-00002610: 656e 742c 202a 6172 6773 2c20 2a2a 6b77  ent, *args, **kw
-00002620: 6172 6773 293a 0a20 2020 2020 2020 2073  args):.        s
-00002630: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
-00002640: 7061 7265 6e74 2920 2023 2074 746b 2e46  parent)  # ttk.F
-00002650: 7261 6d65 0a20 2020 2020 2020 2073 656c  rame.        sel
-00002660: 662e 696e 6974 5f63 6f6e 7461 696e 6572  f.init_container
-00002670: 282a 6172 6773 2c20 2a2a 6b77 6172 6773  (*args, **kwargs
-00002680: 290a 0a0a 636c 6173 7320 4672 616d 654c  )...class FrameL
-00002690: 6162 656c 6c65 6428 7474 6b2e 4c61 6265  abelled(ttk.Labe
-000026a0: 6c46 7261 6d65 2c20 6d69 7869 6e2e 436f  lFrame, mixin.Co
-000026b0: 6e74 6169 6e65 7257 6964 6765 7429 3a0a  ntainerWidget):.
-000026c0: 2020 2020 2727 2741 2066 7261 6d65 2074      '''A frame t
-000026d0: 6f20 686f 6c64 206f 7468 6572 2077 6964  o hold other wid
-000026e0: 6765 7473 2073 7572 726f 756e 6465 6420  gets surrounded 
-000026f0: 6279 2061 206c 696e 652c 2069 6e63 6c75  by a line, inclu
-00002700: 6469 6e67 2061 206c 6162 656c 2e0a 0a20  ding a label... 
-00002710: 2020 2054 6869 7320 6973 2061 2066 7261     This is a fra
-00002720: 6d65 2077 6974 6820 6120 6c61 6265 6c2e  me with a label.
-00002730: 2049 7420 6973 2076 6973 7561 6c6c 7920   It is visually 
-00002740: 7365 7061 7261 7465 6420 6672 6f6d 2074  separated from t
-00002750: 6865 206f 7468 6572 0a20 2020 2077 6964  he other.    wid
-00002760: 6765 7473 2e20 596f 7520 6361 6e20 636f  gets. You can co
-00002770: 6e74 726f 6c20 7468 6520 6c61 6265 6c20  ntrol the label 
-00002780: 706f 7369 7469 6f6e 2e0a 0a20 2020 2054  position...    T
-00002790: 6865 7265 2069 7320 6e6f 2050 7974 686f  here is no Pytho
-000027a0: 6e20 646f 6375 6d65 6e74 6174 696f 6e2c  n documentation,
-000027b0: 2073 6565 2060 6054 6b60 6020 6074 746b   see ``Tk`` `ttk
-000027c0: 2e4c 6162 656c 4672 616d 6520 3c68 7474  .LabelFrame <htt
-000027d0: 7073 3a2f 2f77 7777 2e74 636c 2e74 6b2f  ps://www.tcl.tk/
-000027e0: 6d61 6e2f 7463 6c2f 546b 436d 642f 7474  man/tcl/TkCmd/tt
-000027f0: 6b5f 6c61 6265 6c66 7261 6d65 2e68 746d  k_labelframe.htm
-00002800: 6c3e 605f 2064 6f63 756d 656e 7461 7469  l>`_ documentati
-00002810: 6f6e 2e0a 0a20 2020 2041 7267 733a 0a20  on...    Args:. 
-00002820: 2020 2020 2020 206c 6162 656c 3a20 5468         label: Th
-00002830: 6520 6c61 6265 6c20 746f 2069 6e63 6c75  e label to inclu
-00002840: 6465 206f 6e20 7468 6520 6672 616d 6520  de on the frame 
-00002850: 7365 7061 7261 746f 722e 2043 616e 2062  separator. Can b
-00002860: 6520 6769 7665 6e20 6173 2061 2063 6c61  e given as a cla
-00002870: 7373 2076 6172 6961 626c 652e 0a20 2020  ss variable..   
-00002880: 2020 2020 206c 6162 656c 416e 6368 6f72       labelAnchor
-00002890: 3a20 5468 6520 706f 7369 7469 6f6e 206f  : The position o
-000028a0: 6620 7468 6520 6c61 6265 6c20 6f6e 2074  f the label on t
-000028b0: 6865 2066 7261 6d65 2073 6570 6172 6174  he frame separat
-000028c0: 6f72 2e0a 2020 2020 2020 2020 2020 2020  or..            
-000028d0: 4769 7665 6e20 6173 206f 6e65 206f 6620  Given as one of 
-000028e0: 7468 6520 6361 7264 696e 616c 2070 6f69  the cardinal poi
-000028f0: 6e74 732e 0a20 2020 2020 2020 2020 2020  nts..           
-00002900: 2044 6566 6175 6c74 7320 746f 2061 204f   Defaults to a O
-00002910: 532d 7370 6563 6966 6963 206c 6f63 6174  S-specific locat
-00002920: 696f 6e20 2860 6d6f 6465 6c2e 4350 2e64  ion (`model.CP.d
-00002930: 6566 6175 6c74 6029 2e0a 0a20 2020 2020  efault`)...     
-00002940: 2020 2070 6172 656e 743a 2054 6865 2070     parent: The p
-00002950: 6172 656e 7420 7769 6467 6574 2e20 4361  arent widget. Ca
-00002960: 6e20 6265 2061 2060 526f 6f74 5769 6e64  n be a `RootWind
-00002970: 6f77 6020 6f72 2061 6e6f 7468 6572 2060  ow` or another `
-00002980: 6d69 7869 6e2e 436f 6e74 6169 6e65 7257  mixin.ContainerW
-00002990: 6964 6765 7460 2e0a 0a20 2020 2053 6565  idget`...    See
-000029a0: 2041 6c73 6f3a 0a20 2020 2020 2020 2060   Also:.        `
-000029b0: 4672 616d 6555 6e6c 6162 656c 6c65 6460  FrameUnlabelled`
-000029c0: 3a20 496e 7669 7369 626c 6520 7665 7273  : Invisible vers
-000029d0: 696f 6e2c 2077 6974 686f 7574 2061 206c  ion, without a l
-000029e0: 6162 656c 2e0a 0a20 2020 2020 2020 2060  abel...        `
-000029f0: 4672 616d 6553 7461 7465 6675 6c60 3a20  FrameStateful`: 
-00002a00: 5375 7070 6f72 7420 666f 7220 616e 2065  Support for an e
-00002a10: 6d62 6564 6465 6420 6043 6865 636b 626f  mbedded `Checkbo
-00002a20: 7860 2061 7320 6c61 6265 6c2e 0a20 2020  x` as label..   
-00002a30: 2027 2727 0a20 2020 206c 6162 656c 3a20   '''.    label: 
-00002a40: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00002a50: 7374 725d 203d 204e 6f6e 650a 0a20 2020  str] = None..   
-00002a60: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00002a70: 6c66 2c20 7061 7265 6e74 2c20 2a61 7267  lf, parent, *arg
-00002a80: 732c 206c 6162 656c 3a20 7479 7069 6e67  s, label: typing
-00002a90: 2e4f 7074 696f 6e61 6c5b 7374 725d 203d  .Optional[str] =
-00002aa0: 204e 6f6e 652c 206c 6162 656c 416e 6368   None, labelAnch
-00002ab0: 6f72 3a20 6d6f 6465 6c2e 4350 203d 206d  or: model.CP = m
-00002ac0: 6f64 656c 2e43 502e 6465 6661 756c 742c  odel.CP.default,
-00002ad0: 202a 2a6b 7761 7267 7329 3a0a 2020 2020   **kwargs):.    
-00002ae0: 2020 2020 6368 6f73 656e 5f6c 6162 656c      chosen_label
-00002af0: 203d 2073 656c 662e 6c61 6265 6c20 6f72   = self.label or
-00002b00: 206c 6162 656c 0a20 2020 2020 2020 2069   label.        i
-00002b10: 6620 6368 6f73 656e 5f6c 6162 656c 2069  f chosen_label i
-00002b20: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00002b30: 2020 2020 7261 6973 6520 6578 6365 7074      raise except
-00002b40: 696f 6e2e 496e 7661 6c69 6457 6964 6765  ion.InvalidWidge
-00002b50: 7444 6566 696e 6974 696f 6e28 277b 7365  tDefinition('{se
-00002b60: 6c66 2172 7d3a 204d 6973 7369 6e67 2072  lf!r}: Missing r
-00002b70: 6571 7569 7265 6420 6c61 6265 6c27 290a  equired label').
-00002b80: 2020 2020 2020 2020 2320 544f 444f 3a20          # TODO: 
-00002b90: 496d 7072 6f76 6520 6c61 6265 6c41 6e63  Improve labelAnc
-00002ba0: 686f 7220 6f62 6a65 6374 0a20 2020 2020  hor object.     
-00002bb0: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
-00002bc0: 745f 5f28 7061 7265 6e74 2c20 7465 7874  t__(parent, text
-00002bd0: 3d63 686f 7365 6e5f 6c61 6265 6c2c 206c  =chosen_label, l
-00002be0: 6162 656c 616e 6368 6f72 3d6c 6162 656c  abelanchor=label
-00002bf0: 416e 6368 6f72 2e76 616c 7565 2920 2023  Anchor.value)  #
-00002c00: 2074 746b 2e4c 6162 656c 4672 616d 650a   ttk.LabelFrame.
-00002c10: 2020 2020 2020 2020 6966 205f 5f64 6562          if __deb
-00002c20: 7567 5f5f 3a0a 2020 2020 2020 2020 2020  ug__:.          
-00002c30: 2020 6966 2027 6c61 6265 6c77 6964 6765    if 'labelwidge
-00002c40: 7427 2069 6e20 6b77 6172 6773 3a0a 2020  t' in kwargs:.  
-00002c50: 2020 2020 2020 2020 2020 2020 2020 7761                wa
-00002c60: 726e 696e 6773 2e77 6172 6e28 6627 7b73  rnings.warn(f'{s
-00002c70: 656c 667d 3a20 556e 7375 7070 6f72 7465  elf}: Unsupporte
-00002c80: 6420 226c 6162 656c 7769 6467 6574 2227  d "labelwidget"'
-00002c90: 2c20 7374 6163 6b6c 6576 656c 3d32 290a  , stacklevel=2).
-00002ca0: 2020 2020 2020 2020 6b77 6172 6773 2e70          kwargs.p
-00002cb0: 6f70 2827 6c61 6265 6c77 6964 6765 7427  op('labelwidget'
-00002cc0: 2c20 4e6f 6e65 2920 2023 2055 6e73 7570  , None)  # Unsup
-00002cd0: 706f 7274 6564 0a20 2020 2020 2020 2073  ported.        s
-00002ce0: 656c 662e 696e 6974 5f63 6f6e 7461 696e  elf.init_contain
-00002cf0: 6572 282a 6172 6773 2c20 2a2a 6b77 6172  er(*args, **kwar
-00002d00: 6773 290a 0a0a 636c 6173 7320 4c61 6265  gs)...class Labe
-00002d10: 6c28 7474 6b2e 4c61 6265 6c2c 206d 6978  l(ttk.Label, mix
-00002d20: 696e 2e53 696e 676c 6557 6964 6765 7429  in.SingleWidget)
-00002d30: 3a0a 2020 2020 2727 2741 206c 6162 656c  :.    '''A label
-00002d40: 2c20 6361 6e20 6265 2074 6578 742c 2069  , can be text, i
-00002d50: 6d61 6765 2c20 6f72 2062 6f74 682e 0a0a  mage, or both...
-00002d60: 2020 2020 5468 6973 2069 7320 6120 6c61      This is a la
-00002d70: 6265 6c2c 2061 2073 7461 7469 632d 6973  bel, a static-is
-00002d80: 6820 7769 6467 6574 2077 6974 686f 7574  h widget without
-00002d90: 2069 6e74 6572 6163 7469 6f6e 2e0a 0a20   interaction... 
-00002da0: 2020 2054 6869 7320 6d75 7374 2069 6e63     This must inc
-00002db0: 6c75 6465 2061 7420 6c65 6173 7420 736f  lude at least so
-00002dc0: 6d65 2074 6578 7420 6f72 2061 6e20 696d  me text or an im
-00002dd0: 6167 652c 2065 7665 6e20 7468 6f75 6768  age, even though
-00002de0: 2062 6f74 6820 6172 6520 6f70 7469 6f6e   both are option
-00002df0: 616c 2e0a 0a20 2020 204e 6f20 7374 6174  al...    No stat
-00002e00: 6520 6973 2069 6e63 6c75 6465 642e 0a0a  e is included...
-00002e10: 2020 2020 5468 6572 6520 6973 206e 6f20      There is no 
-00002e20: 5079 7468 6f6e 2064 6f63 756d 656e 7461  Python documenta
-00002e30: 7469 6f6e 2c20 7365 6520 6060 546b 6060  tion, see ``Tk``
-00002e40: 2060 7474 6b2e 4c61 6265 6c20 3c68 7474   `ttk.Label <htt
-00002e50: 7073 3a2f 2f77 7777 2e74 636c 2e74 6b2f  ps://www.tcl.tk/
-00002e60: 6d61 6e2f 7463 6c2f 546b 436d 642f 7474  man/tcl/TkCmd/tt
-00002e70: 6b5f 6c61 6265 6c2e 6874 6d6c 3e60 5f20  k_label.html>`_ 
-00002e80: 646f 6375 6d65 6e74 6174 696f 6e2e 0a0a  documentation...
-00002e90: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00002ea0: 2020 6c61 6265 6c3a 2054 6865 2074 6578    label: The tex
-00002eb0: 7420 746f 2073 686f 772e 204f 7074 696f  t to show. Optio
-00002ec0: 6e61 6c2e 2043 616e 2062 6520 6769 7665  nal. Can be give
-00002ed0: 6e20 6173 2061 2063 6c61 7373 2076 6172  n as a class var
-00002ee0: 6961 626c 652e 0a20 2020 2020 2020 2069  iable..        i
-00002ef0: 6d61 6765 3a20 5468 6520 696d 6167 6520  mage: The image 
-00002f00: 746f 2073 686f 772e 204f 7074 696f 6e61  to show. Optiona
-00002f10: 6c2e 0a20 2020 2020 2020 2020 2020 2053  l..            S
-00002f20: 6565 2060 6054 6b60 6020 6074 6b2e 496d  ee ``Tk`` `tk.Im
-00002f30: 6167 6520 3c68 7474 7073 3a2f 2f77 7777  age <https://www
-00002f40: 2e74 636c 2e74 6b2f 6d61 6e2f 7463 6c2f  .tcl.tk/man/tcl/
-00002f50: 546b 436d 642f 696d 6167 652e 6874 6d6c  TkCmd/image.html
-00002f60: 3e60 5f20 646f 6375 6d65 6e74 6174 696f  >`_ documentatio
-00002f70: 6e2e 0a0a 2020 2020 2020 2020 7061 7265  n...        pare
-00002f80: 6e74 3a20 5468 6520 7061 7265 6e74 2077  nt: The parent w
-00002f90: 6964 6765 742e 2043 616e 2062 6520 6120  idget. Can be a 
-00002fa0: 6052 6f6f 7457 696e 646f 7760 206f 7220  `RootWindow` or 
-00002fb0: 616e 6f74 6865 7220 606d 6978 696e 2e43  another `mixin.C
-00002fc0: 6f6e 7461 696e 6572 5769 6467 6574 602e  ontainerWidget`.
-00002fd0: 0a20 2020 2027 2727 0a20 2020 206c 6162  .    '''.    lab
-00002fe0: 656c 3a20 7479 7069 6e67 2e4f 7074 696f  el: typing.Optio
-00002ff0: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
-00003000: 2020 2020 7374 6174 655f 7479 7065 203d      state_type =
-00003010: 2076 6172 2e6e 6f74 6869 6e67 0a20 2020   var.nothing.   
-00003020: 2077 696d 673a 2074 7970 696e 672e 4f70   wimg: typing.Op
-00003030: 7469 6f6e 616c 5b74 6b2e 496d 6167 655d  tional[tk.Image]
-00003040: 0a20 2020 2027 2727 5468 6520 696d 6167  .    '''The imag
-00003050: 6520 6f62 6a65 6374 2c20 6966 2064 6566  e object, if def
-00003060: 696e 6564 2e0a 0a20 2020 2054 6869 7320  ined...    This 
-00003070: 6176 6f69 6473 2074 6865 2069 7373 7565  avoids the issue
-00003080: 2077 6974 6820 696d 6167 6520 6f62 6a65   with image obje
-00003090: 6374 7320 6265 696e 6720 6761 7262 6167  cts being garbag
-000030a0: 6520 636f 6c6c 6563 7465 642c 2077 6869  e collected, whi
-000030b0: 6c65 206b 6565 7069 6e67 2061 2072 6566  le keeping a ref
-000030c0: 6572 656e 6365 2066 6f72 2070 6f73 7369  erence for possi
-000030d0: 626c 6520 6d61 6e69 7075 6c61 7469 6f6e  ble manipulation
-000030e0: 2e0a 0a20 2020 204e 6f74 653a 0a20 2020  ...    Note:.   
-000030f0: 2020 2020 2054 6869 7320 6973 2061 2072       This is a r
-00003100: 6561 642d 6f6e 6c79 2072 6566 6572 656e  ead-only referen
-00003110: 6365 2c20 6974 206d 7573 7420 6265 206d  ce, it must be m
-00003120: 616e 6970 756c 6174 6564 2075 7369 6e67  anipulated using
-00003130: 2060 7365 745f 696d 6167 6560 2e0a 2020   `set_image`..  
-00003140: 2020 2727 270a 0a20 2020 2064 6566 205f    '''..    def _
-00003150: 5f69 6e69 745f 5f28 7365 6c66 2c20 7061  _init__(self, pa
-00003160: 7265 6e74 2c20 2a2c 206c 6162 656c 3a20  rent, *, label: 
-00003170: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00003180: 7374 725d 203d 204e 6f6e 652c 2069 6d61  str] = None, ima
-00003190: 6765 3a20 7479 7069 6e67 2e4f 7074 696f  ge: typing.Optio
-000031a0: 6e61 6c5b 746b 2e49 6d61 6765 5d20 3d20  nal[tk.Image] = 
-000031b0: 4e6f 6e65 2c20 2a2a 6b77 6172 6773 293a  None, **kwargs):
-000031c0: 0a20 2020 2020 2020 2023 2054 4f44 4f3a  .        # TODO:
-000031d0: 2053 7570 706f 7274 2060 616e 6368 6f72   Support `anchor
-000031e0: 602c 2077 6974 6820 606d 6f64 656c 2e43  `, with `model.C
-000031f0: 5060 0a20 2020 2020 2020 2063 686f 7365  P`.        chose
-00003200: 6e5f 6c61 6265 6c20 3d20 7365 6c66 2e6c  n_label = self.l
-00003210: 6162 656c 206f 7220 6c61 6265 6c0a 2020  abel or label.  
-00003220: 2020 2020 2020 6966 2063 686f 7365 6e5f        if chosen_
-00003230: 6c61 6265 6c20 6973 204e 6f6e 6520 616e  label is None an
-00003240: 6420 696d 6167 6520 6973 204e 6f6e 653a  d image is None:
-00003250: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00003260: 7365 2065 7863 6570 7469 6f6e 2e49 6e76  se exception.Inv
-00003270: 616c 6964 5769 6467 6574 4465 6669 6e69  alidWidgetDefini
-00003280: 7469 6f6e 2827 7b73 656c 6621 727d 3a20  tion('{self!r}: 
-00003290: 4e65 6564 7320 616e 2069 6d61 6765 206f  Needs an image o
-000032a0: 7220 6120 6c61 6265 6c27 290a 2020 2020  r a label').    
-000032b0: 2020 2020 7365 6c66 2e69 6e69 745f 7369      self.init_si
-000032c0: 6e67 6c65 2876 6172 6961 626c 653d 4e6f  ngle(variable=No
-000032d0: 6e65 2920 2023 204e 6f20 7374 6174 6520  ne)  # No state 
-000032e0: 6865 7265 0a20 2020 2020 2020 2073 7570  here.        sup
-000032f0: 6572 2829 2e5f 5f69 6e69 745f 5f28 7061  er().__init__(pa
-00003300: 7265 6e74 2c20 2a2a 6b77 6172 6773 2920  rent, **kwargs) 
-00003310: 2023 2074 746b 2e4c 6162 656c 0a20 2020   # ttk.Label.   
-00003320: 2020 2020 2061 7373 6572 7420 6973 696e       assert isin
-00003330: 7374 616e 6365 2863 686f 7365 6e5f 6c61  stance(chosen_la
-00003340: 6265 6c2c 2073 7472 290a 2020 2020 2020  bel, str).      
-00003350: 2020 6966 2063 686f 7365 6e5f 6c61 6265    if chosen_labe
-00003360: 6c3a 0a20 2020 2020 2020 2020 2020 2073  l:.            s
-00003370: 656c 662e 7365 745f 6c61 6265 6c28 6368  elf.set_label(ch
-00003380: 6f73 656e 5f6c 6162 656c 290a 2020 2020  osen_label).    
-00003390: 2020 2020 6966 2069 6d61 6765 3a0a 2020      if image:.  
-000033a0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-000033b0: 6574 5f69 6d61 6765 2869 6d61 6765 290a  et_image(image).
-000033c0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000033d0: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
-000033e0: 696d 6720 3d20 4e6f 6e65 0a20 2020 2020  img = None.     
-000033f0: 2020 2073 656c 662e 6269 6e64 696e 6728     self.binding(
-00003400: 273c 4275 7474 6f6e 2d31 3e27 2c20 7365  '<Button-1>', se
-00003410: 6c66 2e69 6e76 6f6b 655f 6f6e 436c 6963  lf.invoke_onClic
-00003420: 6b29 0a20 2020 2020 2020 2069 6620 5f5f  k).        if __
-00003430: 6465 6275 675f 5f3a 0a20 2020 2020 2020  debug__:.       
-00003440: 2020 2020 2069 6620 2774 6578 7476 6172       if 'textvar
-00003450: 6961 626c 6527 2069 6e20 6b77 6172 6773  iable' in kwargs
-00003460: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00003470: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
-00003480: 6627 7b73 656c 667d 3a20 546f 2075 7365  f'{self}: To use
-00003490: 2061 2076 6172 6961 626c 6520 6173 206c   a variable as l
-000034a0: 6162 656c 2c20 7365 6520 4c61 6265 6c53  abel, see LabelS
-000034b0: 7461 7465 6675 6c27 2c20 7374 6163 6b6c  tateful', stackl
-000034c0: 6576 656c 3d32 290a 0a20 2020 2064 6566  evel=2)..    def
-000034d0: 2069 6e76 6f6b 655f 6f6e 436c 6963 6b28   invoke_onClick(
-000034e0: 7365 6c66 2c20 6576 656e 743d 4e6f 6e65  self, event=None
-000034f0: 293a 0a20 2020 2020 2020 2027 2727 2727  ):.        '''''
-00003500: 2720 2023 2049 6e74 6572 6e61 6c2c 2064  '  # Internal, d
-00003510: 6f20 6e6f 7420 646f 6375 6d65 6e74 0a20  o not document. 
-00003520: 2020 2020 2020 2073 656c 662e 6f6e 436c         self.onCl
-00003530: 6963 6b28 290a 0a20 2020 2064 6566 2073  ick()..    def s
-00003540: 6574 5f69 6d61 6765 2873 656c 662c 2069  et_image(self, i
-00003550: 6d61 6765 3a20 7479 7069 6e67 2e4f 7074  mage: typing.Opt
-00003560: 696f 6e61 6c5b 746b 2e49 6d61 6765 5d29  ional[tk.Image])
-00003570: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00003580: 2020 2727 2743 6861 6e67 6520 7468 6520    '''Change the 
-00003590: 6c61 6265 6c20 696d 6167 652e 0a0a 2020  label image...  
-000035a0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-000035b0: 2020 2020 2020 2020 696d 6167 653a 2054          image: T
-000035c0: 6865 2069 6d61 6765 206f 626a 6563 7420  he image object 
-000035d0: 746f 2073 6574 2c20 6f72 2060 4e6f 6e65  to set, or `None
-000035e0: 6020 746f 2072 656d 6f76 6520 6974 2e0a  ` to remove it..
-000035f0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-00003600: 2020 2020 7365 6c66 2e77 696d 6720 3d20      self.wimg = 
-00003610: 696d 6167 6520 2023 2053 6176 6520 6120  image  # Save a 
-00003620: 7265 6665 7265 6e63 6520 746f 2061 766f  reference to avo
-00003630: 6964 2067 6172 6261 6765 2063 6f6c 6c65  id garbage colle
-00003640: 6374 696f 6e0a 2020 2020 2020 2020 7365  ction.        se
-00003650: 6c66 5b27 696d 6167 6527 5d20 3d20 7365  lf['image'] = se
-00003660: 6c66 2e77 696d 670a 0a20 2020 2064 6566  lf.wimg..    def
-00003670: 2073 6574 5f6c 6162 656c 2873 656c 662c   set_label(self,
-00003680: 206c 6162 656c 3a20 7374 7229 202d 3e20   label: str) -> 
-00003690: 4e6f 6e65 3a0a 2020 2020 2020 2020 2727  None:.        ''
-000036a0: 2743 6861 6e67 6520 7468 6520 6c61 6265  'Change the labe
-000036b0: 6c20 7465 7874 2e27 2727 0a20 2020 2020  l text.'''.     
-000036c0: 2020 2073 656c 665b 2774 6578 7427 5d20     self['text'] 
-000036d0: 3d20 6c61 6265 6c0a 0a20 2020 2023 2054  = label..    # T
-000036e0: 4f44 4f3a 2050 6173 7320 7468 6520 6576  ODO: Pass the ev
-000036f0: 656e 7420 6f62 6a65 6374 3f0a 2020 2020  ent object?.    
-00003700: 2320 544f 444f 3a20 4e6f 7420 6e65 6564  # TODO: Not need
-00003710: 6564 206f 6e20 6c61 6265 6c73 0a20 2020  ed on labels.   
-00003720: 2064 6566 206f 6e43 6c69 636b 2873 656c   def onClick(sel
-00003730: 6629 3a0a 2020 2020 2020 2020 2222 2243  f):.        """C
-00003740: 616c 6c62 6163 6b20 746f 2062 6520 6578  allback to be ex
-00003750: 6563 7574 6564 2077 6865 6e20 636c 6963  ecuted when clic
-00003760: 6b69 6e67 2074 6869 7320 7769 6467 6574  king this widget
-00003770: 2e0a 0a20 2020 2020 2020 2044 6566 6175  ...        Defau
-00003780: 6c74 7320 746f 2064 6f69 6e67 206e 6f74  lts to doing not
-00003790: 6869 6e67 2e0a 0a20 2020 2020 2020 2041  hing...        A
-000037a0: 7661 696c 6162 6c65 2066 6f72 2073 7562  vailable for sub
-000037b0: 636c 6173 7320 7265 6465 6669 6e69 7469  class redefiniti
-000037c0: 6f6e 2e0a 2020 2020 2020 2020 2222 220a  on..        """.
-000037d0: 2020 2020 2020 2020 7061 7373 0a0a 0a63          pass...c
-000037e0: 6c61 7373 204c 6162 656c 5374 6174 6566  lass LabelStatef
-000037f0: 756c 2874 746b 2e4c 6162 656c 2c20 6d69  ul(ttk.Label, mi
-00003800: 7869 6e2e 5369 6e67 6c65 5769 6467 6574  xin.SingleWidget
-00003810: 293a 0a20 2020 2027 2727 4120 7374 6174  ):.    '''A stat
-00003820: 6566 756c 2060 4c61 6265 6c60 2c20 7768  eful `Label`, wh
-00003830: 6572 6520 7468 6520 7465 7874 2069 7320  ere the text is 
-00003840: 636f 6e74 726f 6c6c 6564 2062 7920 6120  controlled by a 
-00003850: 7661 7269 6162 6c65 2e0a 0a20 2020 2054  variable...    T
-00003860: 6869 7320 6973 2061 6e20 616c 7465 726e  his is an altern
-00003870: 6174 6976 6520 604c 6162 656c 602c 2077  ative `Label`, w
-00003880: 6865 7265 2074 6865 2074 6578 7420 6973  here the text is
-00003890: 2063 6f6e 7472 6f6c 6c65 6420 6279 2061   controlled by a
-000038a0: 2076 6172 6961 626c 652e 0a20 2020 2049   variable..    I
-000038b0: 7427 7320 616e 2061 6c74 6572 6e61 7469  t's an alternati
-000038c0: 7665 2074 6f20 6d61 6e75 616c 6c79 2063  ve to manually c
-000038d0: 616c 6c69 6e67 2060 4c61 6265 6c2e 7365  alling `Label.se
-000038e0: 745f 6c61 6265 6c60 2c20 6f72 2061 2072  t_label`, or a r
-000038f0: 6561 642d 6f6e 6c79 0a20 2020 2060 456e  ead-only.    `En
-00003900: 7472 7960 2e0a 0a20 2020 2054 6865 2069  try`...    The i
-00003910: 6d61 6765 2069 7320 6f70 7469 6f6e 616c  mage is optional
-00003920: 2e0a 0a20 2020 2054 6865 7265 2069 7320  ...    There is 
-00003930: 6e6f 2050 7974 686f 6e20 646f 6375 6d65  no Python docume
-00003940: 6e74 6174 696f 6e2c 2073 6565 2060 6054  ntation, see ``T
-00003950: 6b60 6020 6074 746b 2e4c 6162 656c 203c  k`` `ttk.Label <
-00003960: 6874 7470 733a 2f2f 7777 772e 7463 6c2e  https://www.tcl.
-00003970: 746b 2f6d 616e 2f74 636c 2f54 6b43 6d64  tk/man/tcl/TkCmd
-00003980: 2f74 746b 5f6c 6162 656c 2e68 746d 6c3e  /ttk_label.html>
-00003990: 605f 2064 6f63 756d 656e 7461 7469 6f6e  `_ documentation
-000039a0: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
-000039b0: 2020 2020 2076 6172 6961 626c 653a 2055       variable: U
-000039c0: 7365 2061 6e20 6578 7465 726e 616c 6c79  se an externally
-000039d0: 2064 6566 696e 6564 2076 6172 6961 626c   defined variabl
-000039e0: 652c 2069 6e73 7465 6164 206f 6620 6372  e, instead of cr
-000039f0: 6561 7469 6e67 2061 206e 6577 206f 6e65  eating a new one
-00003a00: 2073 7065 6369 6669 6320 666f 7220 7468   specific for th
-00003a10: 6973 2077 6964 6765 742e 0a20 2020 2020  is widget..     
-00003a20: 2020 2070 6172 656e 743a 2054 6865 2070     parent: The p
-00003a30: 6172 656e 7420 7769 6467 6574 2e20 4361  arent widget. Ca
-00003a40: 6e20 6265 2061 2060 526f 6f74 5769 6e64  n be a `RootWind
-00003a50: 6f77 6020 6f72 2061 6e6f 7468 6572 2060  ow` or another `
-00003a60: 6d69 7869 6e2e 436f 6e74 6169 6e65 7257  mixin.ContainerW
-00003a70: 6964 6765 7460 2e0a 2020 2020 2727 270a  idget`..    '''.
-00003a80: 2020 2020 7374 6174 655f 7479 7065 203d      state_type =
-00003a90: 2076 6172 2e53 7472 696e 670a 2020 2020   var.String.    
-00003aa0: 7769 6d67 3a20 7479 7069 6e67 2e4f 7074  wimg: typing.Opt
-00003ab0: 696f 6e61 6c5b 746b 2e49 6d61 6765 5d0a  ional[tk.Image].
-00003ac0: 2020 2020 2727 2754 6865 2069 6d61 6765      '''The image
-00003ad0: 206f 626a 6563 742c 2069 6620 6465 6669   object, if defi
-00003ae0: 6e65 642e 0a0a 2020 2020 5468 6973 2061  ned...    This a
-00003af0: 766f 6964 7320 7468 6520 6973 7375 6520  voids the issue 
-00003b00: 7769 7468 2069 6d61 6765 206f 626a 6563  with image objec
-00003b10: 7473 2062 6569 6e67 2067 6172 6261 6765  ts being garbage
-00003b20: 2063 6f6c 6c65 6374 6564 2c20 7768 696c   collected, whil
-00003b30: 6520 6b65 6570 696e 6720 6120 7265 6665  e keeping a refe
-00003b40: 7265 6e63 6520 666f 7220 706f 7373 6962  rence for possib
-00003b50: 6c65 206d 616e 6970 756c 6174 696f 6e2e  le manipulation.
-00003b60: 0a0a 2020 2020 4e6f 7465 3a0a 2020 2020  ..    Note:.    
-00003b70: 2020 2020 5468 6973 2069 7320 6120 7265      This is a re
-00003b80: 6164 2d6f 6e6c 7920 7265 6665 7265 6e63  ad-only referenc
-00003b90: 652c 2069 7420 6d75 7374 2062 6520 6d61  e, it must be ma
-00003ba0: 6e69 7075 6c61 7465 6420 7573 696e 6720  nipulated using 
-00003bb0: 6073 6574 5f69 6d61 6765 602e 0a20 2020  `set_image`..   
-00003bc0: 2027 2727 0a0a 2020 2020 6465 6620 5f5f   '''..    def __
-00003bd0: 696e 6974 5f5f 2873 656c 662c 2070 6172  init__(self, par
-00003be0: 656e 742c 202a 2c20 7661 7269 6162 6c65  ent, *, variable
-00003bf0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00003c00: 6c5b 7661 722e 5374 7269 6e67 5d20 3d20  l[var.String] = 
-00003c10: 4e6f 6e65 2c20 696d 6167 653a 2074 7970  None, image: typ
-00003c20: 696e 672e 4f70 7469 6f6e 616c 5b74 6b2e  ing.Optional[tk.
-00003c30: 496d 6167 655d 203d 204e 6f6e 652c 202a  Image] = None, *
-00003c40: 2a6b 7761 7267 7329 3a0a 2020 2020 2020  *kwargs):.      
-00003c50: 2020 7365 6c66 2e69 6e69 745f 7369 6e67    self.init_sing
-00003c60: 6c65 2876 6172 6961 626c 653d 7661 7269  le(variable=vari
-00003c70: 6162 6c65 290a 2020 2020 2020 2020 6b77  able).        kw
-00003c80: 6172 6773 2e75 7064 6174 6528 7b0a 2020  args.update({.  
-00003c90: 2020 2020 2020 2020 2020 2774 6578 7476            'textv
-00003ca0: 6172 6961 626c 6527 3a20 7365 6c66 2e76  ariable': self.v
-00003cb0: 6172 6961 626c 652c 0a20 2020 2020 2020  ariable,.       
-00003cc0: 207d 290a 2020 2020 2020 2020 6b77 6172   }).        kwar
-00003cd0: 6773 2e70 6f70 2827 7465 7874 272c 204e  gs.pop('text', N
-00003ce0: 6f6e 6529 2020 2320 4967 6e6f 7265 2074  one)  # Ignore t
-00003cf0: 6865 2067 6976 656e 2074 6578 740a 2020  he given text.  
-00003d00: 2020 2020 2020 7375 7065 7228 292e 5f5f        super().__
-00003d10: 696e 6974 5f5f 2870 6172 656e 742c 202a  init__(parent, *
-00003d20: 2a6b 7761 7267 7329 2020 2320 7474 6b2e  *kwargs)  # ttk.
-00003d30: 4c61 6265 6c0a 2020 2020 2020 2020 6966  Label.        if
-00003d40: 2069 6d61 6765 3a0a 2020 2020 2020 2020   image:.        
-00003d50: 2020 2020 7365 6c66 2e73 6574 5f69 6d61      self.set_ima
-00003d60: 6765 2869 6d61 6765 290a 2020 2020 2020  ge(image).      
-00003d70: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00003d80: 2020 2020 7365 6c66 2e77 696d 6720 3d20      self.wimg = 
-00003d90: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
-00003da0: 662e 6269 6e64 696e 6728 273c 4275 7474  f.binding('<Butt
-00003db0: 6f6e 2d31 3e27 2c20 7365 6c66 2e69 6e76  on-1>', self.inv
-00003dc0: 6f6b 655f 6f6e 436c 6963 6b29 0a0a 2020  oke_onClick)..  
-00003dd0: 2020 6465 6620 696e 766f 6b65 5f6f 6e43    def invoke_onC
-00003de0: 6c69 636b 2873 656c 662c 2065 7665 6e74  lick(self, event
-00003df0: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-00003e00: 2727 2727 2727 2020 2320 496e 7465 726e  ''''''  # Intern
-00003e10: 616c 2c20 646f 206e 6f74 2064 6f63 756d  al, do not docum
-00003e20: 656e 740a 2020 2020 2020 2020 7365 6c66  ent.        self
-00003e30: 2e6f 6e43 6c69 636b 2829 0a0a 2020 2020  .onClick()..    
-00003e40: 6465 6620 7365 745f 696d 6167 6528 7365  def set_image(se
-00003e50: 6c66 2c20 696d 6167 653a 2074 7970 696e  lf, image: typin
-00003e60: 672e 4f70 7469 6f6e 616c 5b74 6b2e 496d  g.Optional[tk.Im
-00003e70: 6167 655d 2920 2d3e 204e 6f6e 653a 0a20  age]) -> None:. 
-00003e80: 2020 2020 2020 2027 2727 4368 616e 6765         '''Change
-00003e90: 2074 6865 206c 6162 656c 2069 6d61 6765   the label image
-00003ea0: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-00003eb0: 0a20 2020 2020 2020 2020 2020 2069 6d61  .            ima
-00003ec0: 6765 3a20 5468 6520 696d 6167 6520 6f62  ge: The image ob
-00003ed0: 6a65 6374 2074 6f20 7365 742c 206f 7220  ject to set, or 
-00003ee0: 604e 6f6e 6560 2074 6f20 7265 6d6f 7665  `None` to remove
-00003ef0: 2069 742e 0a20 2020 2020 2020 2027 2727   it..        '''
-00003f00: 0a20 2020 2020 2020 2073 656c 662e 7769  .        self.wi
-00003f10: 6d67 203d 2069 6d61 6765 2020 2320 5361  mg = image  # Sa
-00003f20: 7665 2061 2072 6566 6572 656e 6365 2074  ve a reference t
-00003f30: 6f20 6176 6f69 6420 6761 7262 6167 6520  o avoid garbage 
-00003f40: 636f 6c6c 6563 7469 6f6e 0a20 2020 2020  collection.     
-00003f50: 2020 2073 656c 665b 2769 6d61 6765 275d     self['image']
-00003f60: 203d 2073 656c 662e 7769 6d67 0a0a 2020   = self.wimg..  
-00003f70: 2020 2320 544f 444f 3a20 5061 7373 2074    # TODO: Pass t
-00003f80: 6865 2065 7665 6e74 206f 626a 6563 743f  he event object?
-00003f90: 0a20 2020 2023 2054 4f44 4f3a 204e 6f74  .    # TODO: Not
-00003fa0: 206e 6565 6465 6420 6f6e 206c 6162 656c   needed on label
-00003fb0: 730a 2020 2020 6465 6620 6f6e 436c 6963  s.    def onClic
-00003fc0: 6b28 7365 6c66 293a 0a20 2020 2020 2020  k(self):.       
-00003fd0: 2022 2222 4361 6c6c 6261 636b 2074 6f20   """Callback to 
-00003fe0: 6265 2065 7865 6375 7465 6420 7768 656e  be executed when
-00003ff0: 2063 6c69 636b 696e 6720 7468 6973 2077   clicking this w
-00004000: 6964 6765 742e 0a0a 2020 2020 2020 2020  idget...        
-00004010: 4465 6661 756c 7473 2074 6f20 646f 696e  Defaults to doin
-00004020: 6720 6e6f 7468 696e 672e 0a0a 2020 2020  g nothing...    
-00004030: 2020 2020 4176 6169 6c61 626c 6520 666f      Available fo
-00004040: 7220 7375 6263 6c61 7373 2072 6564 6566  r subclass redef
-00004050: 696e 6974 696f 6e2e 0a20 2020 2020 2020  inition..       
-00004060: 2022 2222 0a20 2020 2020 2020 2070 6173   """.        pas
-00004070: 730a 0a0a 636c 6173 7320 4275 7474 6f6e  s...class Button
-00004080: 2874 746b 2e42 7574 746f 6e2c 206d 6978  (ttk.Button, mix
-00004090: 696e 2e53 696e 676c 6557 6964 6765 7429  in.SingleWidget)
-000040a0: 3a0a 2020 2020 2727 2741 2062 7574 746f  :.    '''A butto
-000040b0: 6e20 7769 7468 2061 206c 6162 656c 2e0a  n with a label..
-000040c0: 0a20 2020 2054 6869 7320 6973 2061 2062  .    This is a b
-000040d0: 7574 746f 6e2c 2077 6974 6820 6120 6c61  utton, with a la
-000040e0: 6265 6c2e 2054 6865 206d 6169 6e20 696e  bel. The main in
-000040f0: 7465 7261 6374 696f 6e20 6973 2062 6569  teraction is bei
-00004100: 6e67 2063 6c69 636b 6564 206f 6e2e 0a0a  ng clicked on...
-00004110: 2020 2020 4e6f 2073 7461 7465 2069 7320      No state is 
-00004120: 696e 636c 7564 6564 2e0a 0a20 2020 2054  included...    T
-00004130: 6865 7265 2069 7320 6e6f 2050 7974 686f  here is no Pytho
-00004140: 6e20 646f 6375 6d65 6e74 6174 696f 6e2c  n documentation,
-00004150: 2073 6565 2060 6054 6b60 6020 6074 746b   see ``Tk`` `ttk
-00004160: 2e42 7574 746f 6e20 3c68 7474 7073 3a2f  .Button <https:/
-00004170: 2f77 7777 2e74 636c 2e74 6b2f 6d61 6e2f  /www.tcl.tk/man/
-00004180: 7463 6c2f 546b 436d 642f 7474 6b5f 6275  tcl/TkCmd/ttk_bu
-00004190: 7474 6f6e 2e68 746d 6c3e 605f 2064 6f63  tton.html>`_ doc
-000041a0: 756d 656e 7461 7469 6f6e 2e0a 0a20 2020  umentation...   
-000041b0: 2041 7267 733a 0a20 2020 2020 2020 206c   Args:.        l
-000041c0: 6162 656c 3a20 5468 6520 6c61 6265 6c20  abel: The label 
-000041d0: 746f 2069 6e63 6c75 6465 2069 6e73 6964  to include insid
-000041e0: 6520 7468 6520 6275 7474 6f6e 2e20 4f70  e the button. Op
-000041f0: 7469 6f6e 616c 2e20 4361 6e20 6265 2067  tional. Can be g
-00004200: 6976 656e 2061 7320 6120 636c 6173 7320  iven as a class 
-00004210: 7661 7269 6162 6c65 2e0a 2020 2020 2020  variable..      
-00004220: 2020 7769 6474 683a 2054 6865 2062 7574    width: The but
-00004230: 746f 6e20 7769 6474 682c 2069 6e20 7069  ton width, in pi
-00004240: 7865 6c73 2e0a 2020 2020 2020 2020 2020  xels..          
-00004250: 2020 4465 6661 756c 7473 2074 6f20 616e    Defaults to an
-00004260: 2061 642d 686f 6320 6361 6c63 756c 6174   ad-hoc calculat
-00004270: 696f 6e20 6261 7365 6420 6f6e 2074 6865  ion based on the
-00004280: 206c 656e 6774 6820 6f66 2074 6865 206c   length of the l
-00004290: 6162 656c 2e0a 0a20 2020 2020 2020 2070  abel...        p
-000042a0: 6172 656e 743a 2054 6865 2070 6172 656e  arent: The paren
-000042b0: 7420 7769 6467 6574 2e20 4361 6e20 6265  t widget. Can be
-000042c0: 2061 2060 526f 6f74 5769 6e64 6f77 6020   a `RootWindow` 
-000042d0: 6f72 2061 6e6f 7468 6572 2060 6d69 7869  or another `mixi
-000042e0: 6e2e 436f 6e74 6169 6e65 7257 6964 6765  n.ContainerWidge
-000042f0: 7460 2e0a 2020 2020 2727 270a 2020 2020  t`..    '''.    
-00004300: 6c61 6265 6c3a 2074 7970 696e 672e 4f70  label: typing.Op
-00004310: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00004320: 6e65 0a20 2020 2073 7461 7465 5f74 7970  ne.    state_typ
-00004330: 6520 3d20 7661 722e 6e6f 7468 696e 670a  e = var.nothing.
-00004340: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00004350: 5f28 7365 6c66 2c20 7061 7265 6e74 2c20  _(self, parent, 
-00004360: 2a2c 206c 6162 656c 3a20 7479 7069 6e67  *, label: typing
-00004370: 2e4f 7074 696f 6e61 6c5b 7374 725d 203d  .Optional[str] =
-00004380: 204e 6f6e 652c 2077 6964 7468 3a20 7479   None, width: ty
-00004390: 7069 6e67 2e4f 7074 696f 6e61 6c5b 696e  ping.Optional[in
-000043a0: 745d 203d 204e 6f6e 652c 202a 2a6b 7761  t] = None, **kwa
-000043b0: 7267 7329 3a0a 2020 2020 2020 2020 6368  rgs):.        ch
-000043c0: 6f73 656e 5f6c 6162 656c 203d 2073 656c  osen_label = sel
-000043d0: 662e 6c61 6265 6c20 6f72 206c 6162 656c  f.label or label
-000043e0: 0a20 2020 2020 2020 2069 6620 6368 6f73  .        if chos
-000043f0: 656e 5f6c 6162 656c 2069 7320 4e6f 6e65  en_label is None
-00004400: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00004410: 6973 6520 6578 6365 7074 696f 6e2e 496e  ise exception.In
-00004420: 7661 6c69 6457 6964 6765 7444 6566 696e  validWidgetDefin
-00004430: 6974 696f 6e28 277b 7365 6c66 2172 7d3a  ition('{self!r}:
-00004440: 204d 6973 7369 6e67 2072 6571 7569 7265   Missing require
-00004450: 6420 6c61 6265 6c27 290a 2020 2020 2020  d label').      
-00004460: 2020 7365 6c66 2e69 6e69 745f 7369 6e67    self.init_sing
-00004470: 6c65 2876 6172 6961 626c 653d 4e6f 6e65  le(variable=None
-00004480: 2920 2023 204e 6f20 7374 6174 6520 6865  )  # No state he
-00004490: 7265 0a20 2020 2020 2020 2061 7373 6572  re.        asser
-000044a0: 7420 6973 696e 7374 616e 6365 2863 686f  t isinstance(cho
-000044b0: 7365 6e5f 6c61 6265 6c2c 2073 7472 290a  sen_label, str).
-000044c0: 2020 2020 2020 2020 6b77 6172 6773 2e75          kwargs.u
-000044d0: 7064 6174 6528 7b0a 2020 2020 2020 2020  pdate({.        
-000044e0: 2020 2020 2774 6578 7427 3a20 6368 6f73      'text': chos
-000044f0: 656e 5f6c 6162 656c 2c0a 2020 2020 2020  en_label,.      
-00004500: 2020 2020 2020 2777 6964 7468 273a 2077        'width': w
-00004510: 6964 7468 206f 7220 666e 2e6c 6162 656c  idth or fn.label
-00004520: 5f73 697a 6528 6c65 6e28 6c61 6265 6c20  _size(len(label 
-00004530: 6f72 2027 4d27 2929 2c0a 2020 2020 2020  or 'M')),.      
-00004540: 2020 2020 2020 2763 6f6d 6d61 6e64 273a        'command':
-00004550: 2073 656c 662e 696e 766f 6b65 5f6f 6e43   self.invoke_onC
-00004560: 6c69 636b 2c0a 2020 2020 2020 2020 7d29  lick,.        })
-00004570: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
-00004580: 2e5f 5f69 6e69 745f 5f28 7061 7265 6e74  .__init__(parent
-00004590: 2c20 2a2a 6b77 6172 6773 2920 2023 2074  , **kwargs)  # t
-000045a0: 746b 2e42 7574 746f 6e0a 0a20 2020 2064  tk.Button..    d
-000045b0: 6566 2069 6e76 6f6b 655f 6f6e 436c 6963  ef invoke_onClic
-000045c0: 6b28 7365 6c66 293a 0a20 2020 2020 2020  k(self):.       
-000045d0: 2027 2727 2727 2720 2023 2049 6e74 6572   ''''''  # Inter
-000045e0: 6e61 6c2c 2064 6f20 6e6f 7420 646f 6375  nal, do not docu
-000045f0: 6d65 6e74 0a20 2020 2020 2020 2073 656c  ment.        sel
-00004600: 662e 6f6e 436c 6963 6b28 290a 0a20 2020  f.onClick()..   
-00004610: 2064 6566 206f 6e43 6c69 636b 2873 656c   def onClick(sel
-00004620: 6629 3a0a 2020 2020 2020 2020 2222 2243  f):.        """C
-00004630: 616c 6c62 6163 6b20 746f 2062 6520 6361  allback to be ca
-00004640: 6c6c 6564 2077 6865 6e20 636c 6963 6b69  lled when clicki
-00004650: 6e67 2074 6869 7320 7769 6467 6574 2e0a  ng this widget..
-00004660: 0a20 2020 2020 2020 2044 6566 6175 6c74  .        Default
-00004670: 7320 746f 2064 6f69 6e67 206e 6f74 6869  s to doing nothi
-00004680: 6e67 2e0a 0a20 2020 2020 2020 2041 7661  ng...        Ava
-00004690: 696c 6162 6c65 2066 6f72 2073 7562 636c  ilable for subcl
-000046a0: 6173 7320 7265 6465 6669 6e69 7469 6f6e  ass redefinition
-000046b0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-000046c0: 2020 2020 2020 7061 7373 0a0a 0a63 6c61        pass...cla
-000046d0: 7373 2043 6865 636b 626f 7828 7474 6b2e  ss Checkbox(ttk.
-000046e0: 4368 6563 6b62 7574 746f 6e2c 206d 6978  Checkbutton, mix
-000046f0: 696e 2e53 696e 676c 6557 6964 6765 7429  in.SingleWidget)
-00004700: 3a0a 2020 2020 2727 2741 2063 6865 636b  :.    '''A check
-00004710: 626f 782c 2073 696d 706c 6520 626f 6f6c  box, simple bool
-00004720: 6561 6e20 6368 6f69 6365 2e0a 0a20 2020  ean choice...   
-00004730: 2054 6869 7320 6973 2061 2063 6865 636b   This is a check
-00004740: 626f 7820 7769 7468 2061 206c 6162 656c  box with a label
-00004750: 2e20 5468 6520 6d61 696e 2069 6e74 6572  . The main inter
-00004760: 6163 7469 6f6e 2069 7320 6265 696e 6720  action is being 
-00004770: 636c 6963 6b65 6420 6f6e 2c0a 2020 2020  clicked on,.    
-00004780: 7768 6963 6820 746f 6767 6c65 7320 6974  which toggles it
-00004790: 7320 7661 6c75 652e 0a0a 2020 2020 5468  s value...    Th
-000047a0: 6520 7374 6174 6520 6973 2061 2073 696e  e state is a sin
-000047b0: 676c 6520 6062 6f6f 6c60 2076 616c 7565  gle `bool` value
-000047c0: 2e0a 0a20 2020 2054 6865 7265 2069 7320  ...    There is 
-000047d0: 6e6f 2050 7974 686f 6e20 646f 6375 6d65  no Python docume
-000047e0: 6e74 6174 696f 6e2c 2073 6565 2060 6054  ntation, see ``T
-000047f0: 6b60 6020 6074 746b 2e43 6865 636b 6275  k`` `ttk.Checkbu
-00004800: 7474 6f6e 203c 6874 7470 733a 2f2f 7777  tton <https://ww
-00004810: 772e 7463 6c2e 746b 2f6d 616e 2f74 636c  w.tcl.tk/man/tcl
-00004820: 2f54 6b43 6d64 2f74 746b 5f63 6865 636b  /TkCmd/ttk_check
-00004830: 6275 7474 6f6e 2e68 746d 3e60 5f20 646f  button.htm>`_ do
-00004840: 6375 6d65 6e74 6174 696f 6e2e 0a0a 2020  cumentation...  
-00004850: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00004860: 6c61 6265 6c3a 2054 6865 206c 6162 656c  label: The label
-00004870: 2074 6f20 696e 636c 7564 6520 6265 7369   to include besi
-00004880: 6465 7320 7468 6520 6368 6563 6b62 6f78  des the checkbox
-00004890: 2e20 4361 6e20 6265 2067 6976 656e 2061  . Can be given a
-000048a0: 7320 6120 636c 6173 7320 7661 7269 6162  s a class variab
-000048b0: 6c65 2e0a 2020 2020 2020 2020 2020 2020  le..            
-000048c0: 4974 2069 7320 696e 636c 7564 6564 206f  It is included o
-000048d0: 6e20 7468 6520 7269 6768 7420 7369 6465  n the right side
-000048e0: 206f 6620 7468 6520 6368 6563 6b62 6f78   of the checkbox
-000048f0: 2e0a 2020 2020 2020 2020 7265 6164 6f6e  ..        readon
-00004900: 6c79 3a20 5368 6f75 6c64 2074 6865 2077  ly: Should the w
-00004910: 6964 6765 7420 616c 6c6f 7720 696e 7465  idget allow inte
-00004920: 7261 6374 696f 6e20 746f 2074 6f67 676c  raction to toggl
-00004930: 6520 6974 7320 7661 6c75 652e 2044 6566  e its value. Def
-00004940: 6175 6c74 2074 6f20 2a61 6c6c 6f77 696e  ault to *allowin
-00004950: 672a 2069 6e74 6572 6163 7469 6f6e 2e0a  g* interaction..
-00004960: 0a20 2020 2020 2020 2070 6172 656e 743a  .        parent:
-00004970: 2054 6865 2070 6172 656e 7420 7769 6467   The parent widg
-00004980: 6574 2e20 4361 6e20 6265 2061 2060 526f  et. Can be a `Ro
-00004990: 6f74 5769 6e64 6f77 6020 6f72 2061 6e6f  otWindow` or ano
-000049a0: 7468 6572 2060 6d69 7869 6e2e 436f 6e74  ther `mixin.Cont
-000049b0: 6169 6e65 7257 6964 6765 7460 2e0a 2020  ainerWidget`..  
-000049c0: 2020 2020 2020 7661 7269 6162 6c65 3a20        variable: 
-000049d0: 5573 6520 616e 2065 7874 6572 6e61 6c6c  Use an externall
-000049e0: 7920 6465 6669 6e65 6420 7661 7269 6162  y defined variab
-000049f0: 6c65 2c20 696e 7374 6561 6420 6f66 2063  le, instead of c
-00004a00: 7265 6174 696e 6720 6120 6e65 7720 6f6e  reating a new on
-00004a10: 6520 7370 6563 6966 6963 2066 6f72 2074  e specific for t
-00004a20: 6869 7320 7769 6467 6574 2e0a 2020 2020  his widget..    
-00004a30: 2727 270a 2020 2020 6c61 6265 6c3a 2074  '''.    label: t
-00004a40: 7970 696e 672e 4f70 7469 6f6e 616c 5b73  yping.Optional[s
-00004a50: 7472 5d20 3d20 4e6f 6e65 0a20 2020 2073  tr] = None.    s
-00004a60: 7461 7465 5f74 7970 6520 3d20 7661 722e  tate_type = var.
-00004a70: 426f 6f6c 6561 6e0a 0a20 2020 2064 6566  Boolean..    def
-00004a80: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-00004a90: 7061 7265 6e74 2c20 2a2c 206c 6162 656c  parent, *, label
-00004aa0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00004ab0: 6c5b 7374 725d 203d 204e 6f6e 652c 2072  l[str] = None, r
-00004ac0: 6561 646f 6e6c 793a 2062 6f6f 6c20 3d20  eadonly: bool = 
-00004ad0: 4661 6c73 652c 2076 6172 6961 626c 653a  False, variable:
-00004ae0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-00004af0: 5b76 6172 2e42 6f6f 6c65 616e 5d20 3d20  [var.Boolean] = 
-00004b00: 4e6f 6e65 2c20 2a2a 6b77 6172 6773 293a  None, **kwargs):
-00004b10: 0a20 2020 2020 2020 2063 686f 7365 6e5f  .        chosen_
-00004b20: 6c61 6265 6c20 3d20 7365 6c66 2e6c 6162  label = self.lab
-00004b30: 656c 206f 7220 6c61 6265 6c0a 2020 2020  el or label.    
-00004b40: 2020 2020 6966 2063 686f 7365 6e5f 6c61      if chosen_la
-00004b50: 6265 6c20 6973 204e 6f6e 653a 0a20 2020  bel is None:.   
-00004b60: 2020 2020 2020 2020 2072 6169 7365 2065           raise e
-00004b70: 7863 6570 7469 6f6e 2e49 6e76 616c 6964  xception.Invalid
-00004b80: 5769 6467 6574 4465 6669 6e69 7469 6f6e  WidgetDefinition
-00004b90: 2827 7b73 656c 6621 727d 3a20 4d69 7373  ('{self!r}: Miss
-00004ba0: 696e 6720 7265 7175 6972 6564 206c 6162  ing required lab
-00004bb0: 656c 2729 0a20 2020 2020 2020 2073 656c  el').        sel
-00004bc0: 662e 696e 6974 5f73 696e 676c 6528 7661  f.init_single(va
-00004bd0: 7269 6162 6c65 2c20 676b 6579 733d 5b27  riable, gkeys=['
-00004be0: 7265 6164 6f6e 6c79 275d 290a 2020 2020  readonly']).    
-00004bf0: 2020 2020 6173 7365 7274 2069 7369 6e73      assert isins
-00004c00: 7461 6e63 6528 6368 6f73 656e 5f6c 6162  tance(chosen_lab
-00004c10: 656c 2c20 7374 7229 0a20 2020 2020 2020  el, str).       
-00004c20: 206b 7761 7267 732e 7570 6461 7465 287b   kwargs.update({
-00004c30: 0a20 2020 2020 2020 2020 2020 2027 7465  .            'te
-00004c40: 7874 273a 2063 686f 7365 6e5f 6c61 6265  xt': chosen_labe
-00004c50: 6c2c 0a20 2020 2020 2020 2020 2020 2027  l,.            '
-00004c60: 6f6e 7661 6c75 6527 3a20 5472 7565 2c0a  onvalue': True,.
-00004c70: 2020 2020 2020 2020 2020 2020 276f 6666              'off
-00004c80: 7661 6c75 6527 3a20 4661 6c73 652c 0a20  value': False,. 
-00004c90: 2020 2020 2020 2020 2020 2027 7661 7269             'vari
-00004ca0: 6162 6c65 273a 2073 656c 662e 7661 7269  able': self.vari
-00004cb0: 6162 6c65 2c0a 2020 2020 2020 2020 7d29  able,.        })
-00004cc0: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
-00004cd0: 2e5f 5f69 6e69 745f 5f28 7061 7265 6e74  .__init__(parent
-00004ce0: 2c20 2a2a 6b77 6172 6773 2920 2023 2074  , **kwargs)  # t
-00004cf0: 746b 2e43 6865 636b 6275 7474 6f6e 0a20  tk.Checkbutton. 
-00004d00: 2020 2020 2020 2069 6620 7265 6164 6f6e         if readon
-00004d10: 6c79 3a0a 2020 2020 2020 2020 2020 2020  ly:.            
-00004d20: 2320 5265 6164 2d6f 6e6c 7920 6368 6563  # Read-only chec
-00004d30: 6b62 6f78 656e 2061 7265 2065 6469 7461  kboxen are edita
-00004d40: 626c 652c 2066 6f72 2073 6f6d 6520 7265  ble, for some re
-00004d50: 6173 6f6e 0a20 2020 2020 2020 2020 2020  ason.           
-00004d60: 2073 656c 662e 6773 7461 7465 203d 206d   self.gstate = m
-00004d70: 6f64 656c 2e47 7569 5374 6174 6528 656e  odel.GuiState(en
-00004d80: 6162 6c65 643d 4661 6c73 652c 2072 6561  abled=False, rea
-00004d90: 646f 6e6c 793d 5472 7565 290a 0a20 2020  donly=True)..   
-00004da0: 2064 6566 2074 6f67 676c 6528 7365 6c66   def toggle(self
-00004db0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00004dc0: 2020 2027 2727 5377 6974 6368 2074 6865     '''Switch the
-00004dd0: 2076 6172 6961 626c 6520 7374 6174 6520   variable state 
-00004de0: 746f 2069 7473 206f 7070 6f73 6974 6520  to its opposite 
-00004df0: 2860 6e6f 7420 3c6e 6f74 3e60 292e 2727  (`not <not>`).''
-00004e00: 270a 2020 2020 2020 2020 7365 6c66 2e77  '.        self.w
-00004e10: 7374 6174 6520 3d20 6e6f 7420 7365 6c66  state = not self
-00004e20: 2e77 7374 6174 650a 0a0a 636c 6173 7320  .wstate...class 
-00004e30: 456e 7472 7928 7474 6b2e 456e 7472 792c  Entry(ttk.Entry,
-00004e40: 206d 6978 696e 2e53 696e 676c 6557 6964   mixin.SingleWid
-00004e50: 6765 7429 3a0a 2020 2020 2727 2741 6e20  get):.    '''An 
-00004e60: 656e 7472 7920 7769 6467 6574 2c20 7369  entry widget, si
-00004e70: 6e67 6c65 2d6c 696e 6520 7465 7874 2065  ngle-line text e
-00004e80: 6469 746f 722e 0a0a 2020 2020 5468 6973  ditor...    This
-00004e90: 2069 7320 616e 2065 6e74 7279 2062 6f78   is an entry box
-00004ea0: 2c20 6120 7369 6e67 6c65 2d6c 696e 6520  , a single-line 
-00004eb0: 6564 6974 6f72 2066 6f72 2073 7472 696e  editor for strin
-00004ec0: 6773 2e20 5468 6520 6d61 696e 0a20 2020  gs. The main.   
-00004ed0: 2069 6e74 6572 6163 7469 6f6e 2069 7320   interaction is 
-00004ee0: 6564 6974 696e 6720 7468 6520 7465 7874  editing the text
-00004ef0: 2063 6f6e 7461 696e 6564 2077 6974 6869   contained withi
-00004f00: 6e2e 0a0a 2020 2020 5468 6520 7374 6174  n...    The stat
-00004f10: 6520 6973 2061 2073 696e 676c 6520 6073  e is a single `s
-00004f20: 7472 6020 7661 6c75 652e 0a0a 2020 2020  tr` value...    
-00004f30: 5468 6572 6520 6973 206e 6f20 5079 7468  There is no Pyth
-00004f40: 6f6e 2064 6f63 756d 656e 7461 7469 6f6e  on documentation
-00004f50: 2c20 7365 6520 6060 546b 6060 2060 7474  , see ``Tk`` `tt
-00004f60: 6b2e 456e 7472 7920 3c68 7474 7073 3a2f  k.Entry <https:/
-00004f70: 2f77 7777 2e74 636c 2e74 6b2f 6d61 6e2f  /www.tcl.tk/man/
-00004f80: 7463 6c2f 546b 436d 642f 7474 6b5f 656e  tcl/TkCmd/ttk_en
-00004f90: 7472 792e 6874 6d3e 605f 2064 6f63 756d  try.htm>`_ docum
-00004fa0: 656e 7461 7469 6f6e 2e0a 0a20 2020 2041  entation...    A
-00004fb0: 7267 733a 0a20 2020 2020 2020 2076 6172  rgs:.        var
-00004fc0: 6961 626c 653a 2055 7365 2061 6e20 6578  iable: Use an ex
-00004fd0: 7465 726e 616c 6c79 2064 6566 696e 6564  ternally defined
-00004fe0: 2076 6172 6961 626c 652c 2069 6e73 7465   variable, inste
-00004ff0: 6164 206f 6620 6372 6561 7469 6e67 2061  ad of creating a
-00005000: 206e 6577 206f 6e65 2073 7065 6369 6669   new one specifi
-00005010: 6320 666f 7220 7468 6973 2077 6964 6765  c for this widge
-00005020: 742e 0a0a 2020 2020 2020 2020 6c61 6265  t...        labe
-00005030: 6c3a 2054 6865 206c 6162 656c 2074 6f20  l: The label to 
-00005040: 696e 636c 7564 6520 6265 7369 6465 7320  include besides 
-00005050: 7468 6520 656e 7472 792e 202a 2a4e 6f74  the entry. **Not
-00005060: 2069 6d70 6c65 6d65 6e74 6564 2079 6574   implemented yet
-00005070: 2a2a 2e0a 2020 2020 2020 2020 7061 7265  **..        pare
-00005080: 6e74 3a20 5468 6520 7061 7265 6e74 2077  nt: The parent w
-00005090: 6964 6765 742e 2043 616e 2062 6520 6120  idget. Can be a 
-000050a0: 6052 6f6f 7457 696e 646f 7760 206f 7220  `RootWindow` or 
-000050b0: 616e 6f74 6865 7220 606d 6978 696e 2e43  another `mixin.C
-000050c0: 6f6e 7461 696e 6572 5769 6467 6574 602e  ontainerWidget`.
-000050d0: 0a20 2020 2027 2727 0a20 2020 2073 7461  .    '''.    sta
-000050e0: 7465 5f74 7970 6520 3d20 7661 722e 5374  te_type = var.St
-000050f0: 7269 6e67 0a0a 2020 2020 6465 6620 5f5f  ring..    def __
-00005100: 696e 6974 5f5f 2873 656c 662c 2070 6172  init__(self, par
-00005110: 656e 742c 202a 2c20 7661 7269 6162 6c65  ent, *, variable
-00005120: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00005130: 6c5b 7661 722e 5374 7269 6e67 5d20 3d20  l[var.String] = 
-00005140: 4e6f 6e65 2c20 6c61 6265 6c3a 2074 7970  None, label: typ
-00005150: 696e 672e 4f70 7469 6f6e 616c 5b73 7472  ing.Optional[str
-00005160: 5d20 3d20 4e6f 6e65 2c20 2a2a 6b77 6172  ] = None, **kwar
-00005170: 6773 293a 0a20 2020 2020 2020 2073 656c  gs):.        sel
-00005180: 662e 696e 6974 5f73 696e 676c 6528 7661  f.init_single(va
-00005190: 7269 6162 6c65 290a 2020 2020 2020 2020  riable).        
-000051a0: 7365 6c66 2e6c 6162 656c 203d 206c 6162  self.label = lab
-000051b0: 656c 206f 7220 2727 2020 2320 544f 444f  el or ''  # TODO
-000051c0: 3a20 5368 6f77 206c 6162 656c 2073 6f6d  : Show label som
-000051d0: 6568 6f77 3f0a 2020 2020 2020 2020 6b77  ehow?.        kw
-000051e0: 6172 6773 2e75 7064 6174 6528 7b0a 2020  args.update({.  
-000051f0: 2020 2020 2020 2020 2020 2774 6578 7476            'textv
-00005200: 6172 6961 626c 6527 3a20 7365 6c66 2e76  ariable': self.v
-00005210: 6172 6961 626c 652c 0a20 2020 2020 2020  ariable,.       
-00005220: 207d 290a 2020 2020 2020 2020 7375 7065   }).        supe
-00005230: 7228 292e 5f5f 696e 6974 5f5f 2870 6172  r().__init__(par
-00005240: 656e 742c 202a 2a6b 7761 7267 7329 2020  ent, **kwargs)  
-00005250: 2320 7474 6b2e 456e 7472 790a 2020 2020  # ttk.Entry.    
-00005260: 2020 2020 6966 205f 5f64 6562 7567 5f5f      if __debug__
-00005270: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00005280: 206c 6162 656c 2069 7320 6e6f 7420 4e6f   label is not No
-00005290: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000052a0: 2020 2020 7761 726e 696e 6773 2e77 6172      warnings.war
-000052b0: 6e28 6627 7b73 656c 667d 3a20 4c61 6265  n(f'{self}: Labe
-000052c0: 6c73 206f 6e20 456e 7472 7920 6172 6520  ls on Entry are 
-000052d0: 7374 696c 6c20 756e 7375 7070 6f72 7465  still unsupporte
-000052e0: 642e 2049 6e63 6c75 6465 2061 204c 6162  d. Include a Lab
-000052f0: 656c 206d 616e 7561 6c6c 792e 272c 2073  el manually.', s
-00005300: 7461 636b 6c65 7665 6c3d 3229 0a0a 0a63  tacklevel=2)...c
-00005310: 6c61 7373 2043 6f6d 626f 626f 7828 7474  lass Combobox(tt
-00005320: 6b2e 436f 6d62 6f62 6f78 2c20 6d69 7869  k.Combobox, mixi
-00005330: 6e2e 5369 6e67 6c65 5769 6467 6574 293a  n.SingleWidget):
-00005340: 0a20 2020 2027 2727 4120 636f 6d62 6f62  .    '''A combob
-00005350: 6f78 2077 6964 6765 742c 2063 6f6d 6269  ox widget, combi
-00005360: 6e69 6e67 2061 6e20 6045 6e74 7279 6020  ning an `Entry` 
-00005370: 7769 7468 2061 2060 4c69 7374 626f 7860  with a `Listbox`
-00005380: 2e0a 0a20 2020 2054 6869 7320 6973 2061  ...    This is a
-00005390: 2063 6f6d 626f 626f 782c 2061 6e20 6045   combobox, an `E
-000053a0: 6e74 7279 6020 7769 7468 2061 2062 7574  ntry` with a but
-000053b0: 746f 6e20 7468 6174 2073 686f 7773 2061  ton that shows a
-000053c0: 2070 6f70 2d75 7020 604c 6973 7462 6f78   pop-up `Listbox
-000053d0: 600a 2020 2020 7769 7468 2073 6f6d 6520  `.    with some 
-000053e0: 7072 6564 6566 696e 6564 2060 6076 616c  predefined ``val
-000053f0: 7565 7360 602e 0a0a 2020 2020 5468 6520  ues``...    The 
-00005400: 656e 7472 7920 6361 6e20 6265 2060 6072  entry can be ``r
-00005410: 6561 646f 6e6c 7960 602c 2069 6e20 7768  eadonly``, in wh
-00005420: 6963 6820 6361 7365 2074 6865 206f 6e6c  ich case the onl
-00005430: 7920 706f 7373 6962 6c65 2076 616c 7565  y possible value
-00005440: 7320 6172 650a 2020 2020 7468 6520 6f6e  s are.    the on
-00005450: 6573 2073 686f 776e 206f 6e20 7468 6520  es shown on the 
-00005460: 7661 6c75 6520 6c69 7374 2c20 6f74 6865  value list, othe
-00005470: 7277 6973 6520 7468 6520 656e 7472 7920  rwise the entry 
-00005480: 6973 2065 6469 7461 626c 6520 7769 7468  is editable with
-00005490: 0a20 2020 2061 7262 6974 7261 7279 2076  .    arbitrary v
-000054a0: 616c 7565 732c 206a 7573 7420 6c69 6b65  alues, just like
-000054b0: 2061 6e79 2060 456e 7472 7960 2e0a 0a20   any `Entry`... 
-000054c0: 2020 2054 6865 2060 6069 6d6d 6564 6961     The ``immedia
-000054d0: 7465 6060 2070 6172 616d 6574 6572 2063  te`` parameter c
-000054e0: 616e 2062 6520 7573 6564 2074 6f20 636f  an be used to co
-000054f0: 6e74 726f 6c20 7768 656e 2069 7320 7468  ntrol when is th
-00005500: 6520 6465 6661 756c 740a 2020 2020 7661  e default.    va
-00005510: 6c75 6520 7365 7475 702e 2044 6566 6175  lue setup. Defau
-00005520: 6c74 7320 746f 2062 6569 6e67 2073 6574  lts to being set
-00005530: 206f 6e6c 7920 7768 656e 2074 6865 2047   only when the G
-00005540: 5549 2073 7461 6269 6c69 7a65 732c 2062  UI stabilizes, b
-00005550: 7574 2069 7420 6361 6e0a 2020 2020 6265  ut it can.    be
-00005560: 2073 6574 2061 7320 736f 6f6e 2061 7320   set as soon as 
-00005570: 706f 7373 6962 6c65 2e0a 0a20 2020 2054  possible...    T
-00005580: 6865 7265 2069 7320 6e6f 2050 7974 686f  here is no Pytho
-00005590: 6e20 646f 6375 6d65 6e74 6174 696f 6e2c  n documentation,
-000055a0: 2073 6565 2060 6054 6b60 6020 6074 746b   see ``Tk`` `ttk
-000055b0: 2e43 6f6d 626f 626f 7820 3c68 7474 7073  .Combobox <https
-000055c0: 3a2f 2f77 7777 2e74 636c 2e74 6b2f 6d61  ://www.tcl.tk/ma
-000055d0: 6e2f 7463 6c2f 546b 436d 642f 7474 6b5f  n/tcl/TkCmd/ttk_
-000055e0: 636f 6d62 6f62 6f78 2e68 746d 6c3e 605f  combobox.html>`_
-000055f0: 2064 6f63 756d 656e 7461 7469 6f6e 2e0a   documentation..
-00005600: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-00005610: 2020 2076 616c 7565 733a 2041 2063 6f75     values: A cou
-00005620: 6e74 6162 6c65 2073 7065 6369 6669 6361  ntable specifica
-00005630: 7469 6f6e 206f 6620 7661 6c75 6573 2074  tion of values t
-00005640: 6f20 7368 6f77 206f 6e20 7468 6520 706f  o show on the po
-00005650: 702d 7570 206c 6973 7462 6f78 2e0a 2020  p-up listbox..  
-00005660: 2020 2020 2020 7265 6164 6f6e 6c79 3a20        readonly: 
-00005670: 5368 6f75 6c64 2074 6865 2077 6964 6765  Should the widge
-00005680: 7420 616c 6c6f 7720 696e 7465 7261 6374  t allow interact
-00005690: 696f 6e20 746f 2063 6861 6e67 6520 6974  ion to change it
-000056a0: 7320 7661 6c75 652e 0a20 2020 2020 2020  s value..       
-000056b0: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
-000056c0: 202a 6469 7361 6c6c 6f77 696e 672a 2069   *disallowing* i
-000056d0: 6e74 6572 6163 7469 6f6e 2e0a 2020 2020  nteraction..    
-000056e0: 2020 2020 696d 6d65 6469 6174 653a 2053      immediate: S
-000056f0: 6574 2074 6865 2064 6566 6175 6c74 2076  et the default v
-00005700: 616c 7565 2041 5341 5020 2860 5472 7565  alue ASAP (`True
-00005710: 6029 2c20 6f72 2064 656c 6179 2069 7420  `), or delay it 
-00005720: 6166 7465 7220 7468 650a 2020 2020 2020  after the.      
-00005730: 2020 2020 2020 4755 4920 6973 2073 7461        GUI is sta
-00005740: 626c 6520 2860 4661 6c73 6560 292e 2044  ble (`False`). D
-00005750: 6566 6175 6c74 7320 746f 2060 4661 6c73  efaults to `Fals
-00005760: 6560 2e0a 2020 2020 2020 2020 7661 7269  e`..        vari
-00005770: 6162 6c65 3a20 5573 6520 616e 2065 7874  able: Use an ext
-00005780: 6572 6e61 6c6c 7920 6465 6669 6e65 6420  ernally defined 
-00005790: 7661 7269 6162 6c65 2c20 696e 7374 6561  variable, instea
-000057a0: 6420 6f66 2063 7265 6174 696e 6720 6120  d of creating a 
-000057b0: 6e65 770a 2020 2020 2020 2020 2020 2020  new.            
-000057c0: 6f6e 6520 7370 6563 6966 6963 2066 6f72  one specific for
-000057d0: 2074 6869 7320 7769 6467 6574 2e0a 0a20   this widget... 
-000057e0: 2020 2020 2020 206c 6162 656c 3a20 5468         label: Th
-000057f0: 6520 6c61 6265 6c20 746f 2069 6e63 6c75  e label to inclu
-00005800: 6465 2062 6573 6964 6573 2074 6865 2063  de besides the c
-00005810: 6f6d 626f 626f 782e 202a 2a4e 6f74 2069  ombobox. **Not i
-00005820: 6d70 6c65 6d65 6e74 6564 2079 6574 2a2a  mplemented yet**
-00005830: 2e0a 2020 2020 2020 2020 7061 7265 6e74  ..        parent
-00005840: 3a20 5468 6520 7061 7265 6e74 2077 6964  : The parent wid
-00005850: 6765 742e 2043 616e 2062 6520 6120 6052  get. Can be a `R
-00005860: 6f6f 7457 696e 646f 7760 206f 7220 616e  ootWindow` or an
-00005870: 6f74 6865 7220 606d 6978 696e 2e43 6f6e  other `mixin.Con
-00005880: 7461 696e 6572 5769 6467 6574 602e 0a20  tainerWidget`.. 
-00005890: 2020 2027 2727 0a20 2020 2073 7461 7465     '''.    state
-000058a0: 5f74 7970 6520 3d20 7661 722e 5374 7269  _type = var.Stri
-000058b0: 6e67 0a0a 2020 2020 6465 6620 5f5f 696e  ng..    def __in
-000058c0: 6974 5f5f 2873 656c 662c 2070 6172 656e  it__(self, paren
-000058d0: 742c 2076 616c 7565 733a 2073 7065 632e  t, values: spec.
-000058e0: 5370 6563 436f 756e 7461 626c 652c 202a  SpecCountable, *
-000058f0: 2c20 7265 6164 6f6e 6c79 3a20 626f 6f6c  , readonly: bool
-00005900: 203d 2054 7275 652c 2069 6d6d 6564 6961   = True, immedia
-00005910: 7465 3a20 626f 6f6c 203d 2046 616c 7365  te: bool = False
-00005920: 2c20 7661 7269 6162 6c65 3a20 7479 7069  , variable: typi
-00005930: 6e67 2e4f 7074 696f 6e61 6c5b 7661 722e  ng.Optional[var.
-00005940: 5374 7269 6e67 5d20 3d20 4e6f 6e65 2c20  String] = None, 
-00005950: 6c61 6265 6c3a 2074 7970 696e 672e 4f70  label: typing.Op
-00005960: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00005970: 6e65 2c20 2a2a 6b77 6172 6773 293a 0a20  ne, **kwargs):. 
-00005980: 2020 2020 2020 2073 656c 662e 696e 6974         self.init
-00005990: 5f73 696e 676c 6528 7661 7269 6162 6c65  _single(variable
-000059a0: 2c20 676b 6579 733d 5b27 7265 6164 6f6e  , gkeys=['readon
-000059b0: 6c79 275d 290a 2020 2020 2020 2020 7365  ly']).        se
-000059c0: 6c66 2e6c 6162 656c 203d 206c 6162 656c  lf.label = label
-000059d0: 206f 7220 2727 2020 2320 544f 444f 3a20   or ''  # TODO: 
-000059e0: 5368 6f77 206c 6162 656c 2073 6f6d 6568  Show label someh
-000059f0: 6f77 0a20 2020 2020 2020 2073 656c 662e  ow.        self.
-00005a00: 7370 6563 5661 6c75 6573 203d 2076 616c  specValues = val
-00005a10: 7565 730a 2020 2020 2020 2020 6b77 6172  ues.        kwar
-00005a20: 6773 2e75 7064 6174 6528 7b0a 2020 2020  gs.update({.    
-00005a30: 2020 2020 2020 2020 2774 6578 7476 6172          'textvar
-00005a40: 6961 626c 6527 3a20 7365 6c66 2e76 6172  iable': self.var
-00005a50: 6961 626c 652c 0a20 2020 2020 2020 2020  iable,.         
-00005a60: 2020 2027 7661 6c75 6573 273a 206c 6973     'values': lis
-00005a70: 7428 7365 6c66 2e73 7065 6356 616c 7565  t(self.specValue
-00005a80: 732e 616c 6c28 2929 2c0a 2020 2020 2020  s.all()),.      
-00005a90: 2020 7d29 0a20 2020 2020 2020 2073 7570    }).        sup
-00005aa0: 6572 2829 2e5f 5f69 6e69 745f 5f28 7061  er().__init__(pa
-00005ab0: 7265 6e74 2c20 2a2a 6b77 6172 6773 2920  rent, **kwargs) 
-00005ac0: 2023 2074 746b 2e43 6f6d 626f 626f 780a   # ttk.Combobox.
-00005ad0: 2020 2020 2020 2020 6966 2069 6d6d 6564          if immed
-00005ae0: 6961 7465 3a0a 2020 2020 2020 2020 2020  iate:.          
-00005af0: 2020 7365 6c66 2e73 6574 4465 6661 756c    self.setDefaul
-00005b00: 7428 290a 2020 2020 2020 2020 656c 7365  t().        else
-00005b10: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00005b20: 6c66 2e61 6674 6572 5f69 646c 6528 7365  lf.after_idle(se
-00005b30: 6c66 2e73 6574 4465 6661 756c 7429 2020  lf.setDefault)  
-00005b40: 2320 4e6f 206e 6565 6420 666f 7220 6120  # No need for a 
-00005b50: 6054 696d 656f 7574 4964 6c65 6020 6865  `TimeoutIdle` he
-00005b60: 7265 0a20 2020 2020 2020 2069 6620 7265  re.        if re
-00005b70: 6164 6f6e 6c79 3a0a 2020 2020 2020 2020  adonly:.        
-00005b80: 2020 2020 7365 6c66 2e67 7374 6174 6520      self.gstate 
-00005b90: 3d20 6d6f 6465 6c2e 4775 6953 7461 7465  = model.GuiState
-00005ba0: 2872 6561 646f 6e6c 793d 5472 7565 290a  (readonly=True).
-00005bb0: 2020 2020 2020 2020 6966 205f 5f64 6562          if __deb
-00005bc0: 7567 5f5f 3a0a 2020 2020 2020 2020 2020  ug__:.          
-00005bd0: 2020 2320 4465 6669 6e65 2061 6c6c 2074    # Define all t
-00005be0: 6865 206c 6f63 616c 2073 7562 636c 6173  he local subclas
-00005bf0: 7365 7320 2874 6861 7420 6f76 6572 7269  ses (that overri
-00005c00: 6465 205f 5f69 6e69 745f 5f29 2074 6f20  de __init__) to 
-00005c10: 696d 7072 6f76 6520 6c6f 6767 696e 670a  improve logging.
-00005c20: 2020 2020 2020 2020 2020 2020 5f64 656c              _del
-00005c30: 7461 6c65 7665 6c20 3d20 3120 6966 2069  talevel = 1 if i
-00005c40: 7369 6e73 7461 6e63 6528 7365 6c66 2c20  sinstance(self, 
-00005c50: 2843 6f6d 626f 626f 784d 6170 2c29 2920  (ComboboxMap,)) 
-00005c60: 656c 7365 2030 0a20 2020 2020 2020 2020  else 0.         
-00005c70: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
-00005c80: 616e 6365 2873 656c 662c 2043 6f6d 626f  ance(self, Combo
-00005c90: 626f 784d 6170 2920 616e 6420 6973 696e  boxMap) and isin
-00005ca0: 7374 616e 6365 2873 656c 662e 7370 6563  stance(self.spec
-00005cb0: 5661 6c75 6573 2c20 7370 6563 2e53 7461  Values, spec.Sta
-00005cc0: 7469 634d 6170 293a 0a20 2020 2020 2020  ticMap):.       
-00005cd0: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
-00005ce0: 732e 7761 726e 2866 277b 7365 6c66 7d3a  s.warn(f'{self}:
-00005cf0: 2053 6565 2060 436f 6d62 6f62 6f78 4d61   See `ComboboxMa
-00005d00: 7060 2066 6f72 2075 7369 6e67 2074 6865  p` for using the
-00005d10: 2076 616c 7565 7320 636f 7272 6563 746c   values correctl
-00005d20: 7927 2c20 7374 6163 6b6c 6576 656c 3d32  y', stacklevel=2
-00005d30: 202b 205f 6465 6c74 616c 6576 656c 290a   + _deltalevel).
-00005d40: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-00005d50: 6162 656c 2069 7320 6e6f 7420 4e6f 6e65  abel is not None
-00005d60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00005d70: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
-00005d80: 6627 7b73 656c 667d 3a20 4c61 6265 6c73  f'{self}: Labels
-00005d90: 206f 6e20 436f 6d62 6f62 6f78 2061 7265   on Combobox are
-00005da0: 2073 7469 6c6c 2075 6e73 7570 706f 7274   still unsupport
-00005db0: 6564 2e20 496e 636c 7564 6520 6120 4c61  ed. Include a La
-00005dc0: 6265 6c20 6d61 6e75 616c 6c79 2e27 2c20  bel manually.', 
-00005dd0: 7374 6163 6b6c 6576 656c 3d32 202b 205f  stacklevel=2 + _
-00005de0: 6465 6c74 616c 6576 656c 290a 0a20 2020  deltalevel)..   
-00005df0: 2023 2054 4f44 4f3a 2054 6869 7320 636f   # TODO: This co
-00005e00: 756c 6420 6265 2061 2063 6f6d 6d6f 6e20  uld be a common 
-00005e10: 606d 6978 696e 2e53 696e 676c 6557 6964  `mixin.SingleWid
-00005e20: 6765 7460 206d 6574 686f 643f 0a20 2020  get` method?.   
-00005e30: 2064 6566 2073 6574 4465 6661 756c 7428   def setDefault(
-00005e40: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-00005e50: 2020 2020 2020 2027 2727 5365 7420 7468         '''Set th
-00005e60: 6520 6375 7272 656e 7420 7374 6174 6520  e current state 
-00005e70: 746f 2074 6865 2064 6566 6175 6c74 206c  to the default l
-00005e80: 6162 656c 2e27 2727 0a20 2020 2020 2020  abel.'''.       
-00005e90: 2073 656c 662e 7773 7461 7465 203d 2073   self.wstate = s
-00005ea0: 656c 662e 7370 6563 5661 6c75 6573 2e64  elf.specValues.d
-00005eb0: 6566 6175 6c74 0a0a 2020 2020 2320 544f  efault..    # TO
-00005ec0: 444f 3a20 5468 6973 2063 6f75 6c64 2062  DO: This could b
-00005ed0: 6520 6120 636f 6d6d 6f6e 2060 6d69 7869  e a common `mixi
-00005ee0: 6e2e 5369 6e67 6c65 5769 6467 6574 6020  n.SingleWidget` 
-00005ef0: 6d65 7468 6f64 3f0a 2020 2020 6465 6620  method?.    def 
-00005f00: 6553 6574 2873 656c 662c 206c 6162 656c  eSet(self, label
-00005f10: 3a20 7374 7229 202d 3e20 7479 7069 6e67  : str) -> typing
-00005f20: 2e43 616c 6c61 626c 655b 2e2e 2e2c 204e  .Callable[..., N
-00005f30: 6f6e 655d 3a0a 2020 2020 2020 2020 2727  one]:.        ''
-00005f40: 2752 6574 7572 6e20 616e 2065 7665 6e74  'Return an event
-00005f50: 2066 756e 6374 696f 6e20 746f 2073 6574   function to set
-00005f60: 2074 6865 2073 7461 7465 2061 2063 6572   the state a cer
-00005f70: 7461 696e 206c 6162 656c 2e27 2727 0a20  tain label.'''. 
-00005f80: 2020 2020 2020 2069 6620 6c61 6265 6c20         if label 
-00005f90: 6e6f 7420 696e 2073 656c 662e 7370 6563  not in self.spec
-00005fa0: 5661 6c75 6573 3a0a 2020 2020 2020 2020  Values:.        
-00005fb0: 2020 2020 7261 6973 6520 6578 6365 7074      raise except
-00005fc0: 696f 6e2e 496e 7661 6c69 6443 616c 6c62  ion.InvalidCallb
-00005fd0: 6163 6b44 6566 696e 6974 696f 6e28 6627  ackDefinition(f'
-00005fe0: 5365 7474 696e 6720 616e 2069 6e76 616c  Setting an inval
-00005ff0: 6964 206c 6162 656c 3a20 7b6c 6162 656c  id label: {label
-00006000: 7d27 290a 0a20 2020 2020 2020 2064 6566  }')..        def
-00006010: 2065 5365 7428 293a 0a20 2020 2020 2020   eSet():.       
-00006020: 2020 2020 2073 656c 662e 7773 7461 7465       self.wstate
-00006030: 203d 206c 6162 656c 0a20 2020 2020 2020   = label.       
-00006040: 2072 6574 7572 6e20 6553 6574 0a0a 0a63   return eSet...c
-00006050: 6c61 7373 2043 6f6d 626f 626f 784d 6170  lass ComboboxMap
-00006060: 2843 6f6d 626f 626f 7829 3a0a 2020 2020  (Combobox):.    
-00006070: 2727 2741 2063 6f6d 626f 626f 7820 7769  '''A combobox wi
-00006080: 6467 6574 2c20 7072 6570 6172 6564 2074  dget, prepared t
-00006090: 6f20 7573 6520 6073 7065 632e 5374 6174  o use `spec.Stat
-000060a0: 6963 4d61 7060 2e0a 0a20 2020 2054 6869  icMap`...    Thi
-000060b0: 7320 6973 206a 7573 7420 6120 6e6f 726d  s is just a norm
-000060c0: 616c 2060 436f 6d62 6f62 6f78 602c 2062  al `Combobox`, b
-000060d0: 7574 2074 6865 2060 6076 616c 7565 7360  ut the ``values`
-000060e0: 6020 6f62 6a65 6374 206d 7573 7420 6265  ` object must be
-000060f0: 2061 0a20 2020 2060 7370 6563 2e53 7461   a.    `spec.Sta
-00006100: 7469 634d 6170 602c 2061 6e64 2074 6865  ticMap`, and the
-00006110: 2077 6964 6765 7420 7661 6c75 6520 7769   widget value wi
-00006120: 6c6c 2062 6520 7265 7475 726e 6564 2061  ll be returned a
-00006130: 7320 6974 7320 7661 6c75 652c 206e 6f74  s its value, not
-00006140: 0a20 2020 2074 6865 206c 6162 656c 2e0a  .    the label..
-00006150: 0a20 2020 204e 6f74 653a 0a20 2020 2020  .    Note:.     
-00006160: 2020 2054 6869 7320 6973 2073 7469 6c6c     This is still
-00006170: 2057 4950 2c20 7365 656d 7320 6c69 6b65   WIP, seems like
-00006180: 2061 2076 6572 7920 6269 6720 6861 636b   a very big hack
-00006190: 2066 6f72 206e 6f77 2e0a 2020 2020 2727   for now..    ''
-000061a0: 270a 2020 2020 6465 6620 5f5f 696e 6974  '.    def __init
-000061b0: 5f5f 2873 656c 662c 202a 6172 6773 2c20  __(self, *args, 
-000061c0: 2a2a 6b77 6172 6773 293a 0a20 2020 2020  **kwargs):.     
-000061d0: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
-000061e0: 745f 5f28 2a61 7267 732c 202a 2a6b 7761  t__(*args, **kwa
-000061f0: 7267 7329 0a20 2020 2020 2020 2061 7373  rgs).        ass
-00006200: 6572 7420 6973 696e 7374 616e 6365 2873  ert isinstance(s
-00006210: 656c 662e 7370 6563 5661 6c75 6573 2c20  elf.specValues, 
-00006220: 7370 6563 2e53 7461 7469 634d 6170 292c  spec.StaticMap),
-00006230: 2066 277b 7365 6c66 7d3a 2076 616c 7565   f'{self}: value
-00006240: 7320 6d75 7374 2062 6520 6120 6073 7065  s must be a `spe
-00006250: 632e 5374 6174 6963 4d61 7060 270a 0a20  c.StaticMap`'.. 
-00006260: 2020 2064 6566 2073 7461 7465 5f67 6574     def state_get
-00006270: 2873 656c 662c 202a 6172 6773 2c20 2a2a  (self, *args, **
-00006280: 6b77 6172 6773 293a 0a20 2020 2020 2020  kwargs):.       
-00006290: 2027 2727 2727 2720 2023 2044 6f20 6e6f   ''''''  # Do no
-000062a0: 7420 646f 6375 6d65 6e74 0a20 2020 2020  t document.     
-000062b0: 2020 206c 6162 656c 203d 2073 7570 6572     label = super
-000062c0: 2829 2e73 7461 7465 5f67 6574 282a 6172  ().state_get(*ar
-000062d0: 6773 2c20 2a2a 6b77 6172 6773 290a 2020  gs, **kwargs).  
-000062e0: 2020 2020 2020 7661 6c75 6520 3d20 7365        value = se
-000062f0: 6c66 2e73 7065 6356 616c 7565 732e 7661  lf.specValues.va
-00006300: 6c75 6528 6c61 6265 6c29 0a20 2020 2020  lue(label).     
-00006310: 2020 2023 2069 6620 5f5f 6465 6275 675f     # if __debug_
-00006320: 5f3a 0a20 2020 2020 2020 2023 2020 2020  _:.        #    
-00006330: 206c 6f67 6765 722e 6465 6275 6728 274c   logger.debug('L
-00006340: 5b25 735d 203d 3e20 2572 272c 206c 6162  [%s] => %r', lab
-00006350: 656c 2c20 7661 6c75 6529 0a20 2020 2020  el, value).     
-00006360: 2020 2072 6574 7572 6e20 6d6f 6465 6c2e     return model.
-00006370: 5653 7461 7465 2876 616c 7565 2c20 6c61  VState(value, la
-00006380: 6265 6c3d 6c61 6265 6c29 0a0a 2020 2020  bel=label)..    
-00006390: 6465 6620 7374 6174 655f 7365 7428 7365  def state_set(se
-000063a0: 6c66 2c20 7374 6174 652c 202a 6172 6773  lf, state, *args
-000063b0: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
-000063c0: 2020 2020 2027 2727 2727 2720 2023 2044       ''''''  # D
-000063d0: 6f20 6e6f 7420 646f 6375 6d65 6e74 0a20  o not document. 
-000063e0: 2020 2020 2020 2023 2053 7570 706f 7274         # Support
-000063f0: 2073 6574 7469 6e67 206c 6162 656c 7320   setting labels 
-00006400: 616e 6420 5653 7461 7465 0a20 2020 2020  and VState.     
-00006410: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00006420: 2873 7461 7465 2c20 6d6f 6465 6c2e 5653  (state, model.VS
-00006430: 7461 7465 293a 0a20 2020 2020 2020 2020  tate):.         
-00006440: 2020 206c 6162 656c 203d 2073 656c 662e     label = self.
-00006450: 7370 6563 5661 6c75 6573 2e6c 6162 656c  specValues.label
-00006460: 2873 7461 7465 2e76 616c 7565 290a 2020  (state.value).  
-00006470: 2020 2020 2020 2020 2020 6966 205f 5f64            if __d
-00006480: 6562 7567 5f5f 3a0a 2020 2020 2020 2020  ebug__:.        
-00006490: 2020 2020 2020 2020 6966 2073 7461 7465          if state
-000064a0: 2e6c 6162 656c 3a0a 2020 2020 2020 2020  .label:.        
-000064b0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-000064c0: 7274 2073 7461 7465 2e6c 6162 656c 203d  rt state.label =
-000064d0: 3d20 6c61 6265 6c0a 2020 2020 2020 2020  = label.        
-000064e0: 2020 2020 2020 2020 2320 6c6f 6767 6572          # logger
-000064f0: 2e64 6562 7567 2827 2572 203d 3e20 2573  .debug('%r => %s
-00006500: 272c 2073 7461 7465 2c20 6c61 6265 6c29  ', state, label)
-00006510: 0a20 2020 2020 2020 2065 6c73 653a 2020  .        else:  
-00006520: 2320 5365 7474 696e 6720 6120 7369 6d70  # Setting a simp
-00006530: 6c65 206c 6162 656c 0a20 2020 2020 2020  le label.       
-00006540: 2020 2020 206c 6162 656c 203d 2073 7461       label = sta
-00006550: 7465 0a20 2020 2020 2020 2020 2020 2069  te.            i
-00006560: 6620 5f5f 6465 6275 675f 5f3a 0a20 2020  f __debug__:.   
-00006570: 2020 2020 2020 2020 2020 2020 2070 6173               pas
-00006580: 7320 2023 206c 6f67 6765 722e 6465 6275  s  # logger.debu
-00006590: 6728 274c 5b25 735d 272c 206c 6162 656c  g('L[%s]', label
-000065a0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-000065b0: 2073 7570 6572 2829 2e73 7461 7465 5f73   super().state_s
-000065c0: 6574 286c 6162 656c 2c20 2a61 7267 732c  et(label, *args,
-000065d0: 202a 2a6b 7761 7267 7329 0a0a 2020 2020   **kwargs)..    
-000065e0: 6465 6620 6553 6574 5661 6c75 6528 7365  def eSetValue(se
-000065f0: 6c66 2c20 7661 6c75 6529 3a0a 2020 2020  lf, value):.    
-00006600: 2020 2020 2727 2757 7261 7065 7220 666f      '''Wraper fo
-00006610: 7220 6043 6f6d 626f 626f 782e 6553 6574  r `Combobox.eSet
-00006620: 602c 2070 7265 7061 7265 6420 746f 2075  `, prepared to u
-00006630: 7365 2060 7370 6563 2e53 7461 7469 634d  se `spec.StaticM
-00006640: 6170 602e 2727 270a 2020 2020 2020 2020  ap`.'''.        
-00006650: 6173 7365 7274 2069 7369 6e73 7461 6e63  assert isinstanc
-00006660: 6528 7365 6c66 2e73 7065 6356 616c 7565  e(self.specValue
-00006670: 732c 2073 7065 632e 5374 6174 6963 4d61  s, spec.StaticMa
-00006680: 7029 0a20 2020 2020 2020 2072 6574 7572  p).        retur
-00006690: 6e20 7365 6c66 2e65 5365 7428 7365 6c66  n self.eSet(self
-000066a0: 2e73 7065 6356 616c 7565 732e 6c61 6265  .specValues.labe
-000066b0: 6c28 7661 6c75 6529 290a 0a20 2020 2069  l(value))..    i
-000066c0: 6620 5f5f 6465 6275 675f 5f3a 0a20 2020  f __debug__:.   
-000066d0: 2020 2020 2023 2057 6172 6e20 6162 6f75       # Warn abou
-000066e0: 7420 7472 6163 6520 7573 6167 650a 2020  t trace usage.  
-000066f0: 2020 2020 2020 6465 6620 7472 6163 6528        def trace(
-00006700: 7365 6c66 2c20 2a61 7267 732c 202a 2a6b  self, *args, **k
-00006710: 7761 7267 7329 3a0a 2020 2020 2020 2020  wargs):.        
-00006720: 2020 2020 6966 2073 656c 662e 7370 6563      if self.spec
-00006730: 5661 6c75 6573 206e 6f74 2069 6e20 6b77  Values not in kw
-00006740: 6172 6773 2e76 616c 7565 7328 293a 0a20  args.values():. 
-00006750: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00006760: 6172 6e69 6e67 732e 7761 726e 2827 4d61  arnings.warn('Ma
-00006770: 6b65 2073 7572 6520 746f 2073 656e 6420  ke sure to send 
-00006780: 6073 656c 662e 7370 6563 5661 6c75 6573  `self.specValues
-00006790: 6020 746f 2067 6574 2074 6865 2022 7265  ` to get the "re
-000067a0: 616c 2220 7661 6c75 6573 272c 2073 7461  al" values', sta
-000067b0: 636b 6c65 7665 6c3d 3229 0a20 2020 2020  cklevel=2).     
-000067c0: 2020 2020 2020 2072 6574 7572 6e20 7375         return su
-000067d0: 7065 7228 292e 7472 6163 6528 2a61 7267  per().trace(*arg
-000067e0: 732c 202a 2a6b 7761 7267 7329 0a0a 0a63  s, **kwargs)...c
-000067f0: 6c61 7373 2046 7261 6d65 5374 6174 6566  lass FrameStatef
-00006800: 756c 2874 746b 2e4c 6162 656c 4672 616d  ul(ttk.LabelFram
-00006810: 652c 206d 6978 696e 2e43 6f6e 7461 696e  e, mixin.Contain
-00006820: 6572 5769 6467 6574 293a 0a20 2020 2027  erWidget):.    '
-00006830: 2727 4120 6672 616d 6520 746f 2068 6f6c  ''A frame to hol
-00006840: 6420 6f74 6865 7220 7769 6467 6574 732c  d other widgets,
-00006850: 2077 6974 6820 6120 6368 6563 6b62 6f78   with a checkbox
-00006860: 2e0a 0a20 2020 2054 6869 7320 6973 2061  ...    This is a
-00006870: 2066 7261 6d65 2077 6974 6820 616e 2065   frame with an e
-00006880: 6d62 6564 6465 6420 6368 6563 6b62 6f78  mbedded checkbox
-00006890: 2060 6373 7461 7465 5f77 6964 6765 7460   `cstate_widget`
-000068a0: 2061 7320 226c 6162 656c 222e 2054 6869   as "label". Thi
-000068b0: 730a 2020 2020 6c61 6265 6c20 636f 6e74  s.    label cont
-000068c0: 726f 6c73 2074 6865 2065 6e61 626c 6564  rols the enabled
-000068d0: 2073 7461 7465 206f 6620 7468 6520 6368   state of the ch
-000068e0: 696c 6420 7769 6467 6574 732e 2059 6f75  ild widgets. You
-000068f0: 2063 616e 2063 6f6e 7472 6f6c 2074 6865   can control the
-00006900: 0a20 2020 2063 6865 636b 626f 7820 706f  .    checkbox po
-00006910: 7369 7469 6f6e 2e0a 0a20 2020 2054 6865  sition...    The
-00006920: 7265 2069 7320 6e6f 2050 7974 686f 6e20  re is no Python 
-00006930: 646f 6375 6d65 6e74 6174 696f 6e2c 2073  documentation, s
-00006940: 6565 2060 6054 6b60 6020 6074 746b 2e4c  ee ``Tk`` `ttk.L
-00006950: 6162 656c 4672 616d 6520 3c68 7474 7073  abelFrame <https
-00006960: 3a2f 2f77 7777 2e74 636c 2e74 6b2f 6d61  ://www.tcl.tk/ma
-00006970: 6e2f 7463 6c2f 546b 436d 642f 7474 6b5f  n/tcl/TkCmd/ttk_
-00006980: 6c61 6265 6c66 7261 6d65 2e68 746d 6c3e  labelframe.html>
-00006990: 605f 2064 6f63 756d 656e 7461 7469 6f6e  `_ documentation
-000069a0: 2e0a 2020 2020 4e6f 7465 2074 6865 2060  ..    Note the `
-000069b0: 606c 6162 656c 7769 6467 6574 6060 206f  `labelwidget`` o
-000069c0: 7074 696f 6e2e 0a0a 2020 2020 4172 6773  ption...    Args
-000069d0: 3a0a 2020 2020 2020 2020 6c61 6265 6c3a  :.        label:
-000069e0: 2054 6865 206c 6162 656c 2074 6f20 696e   The label to in
-000069f0: 636c 7564 6520 6f6e 2074 6865 2066 7261  clude on the fra
-00006a00: 6d65 2073 6570 6172 6174 6f72 2e20 4361  me separator. Ca
-00006a10: 6e20 6265 2067 6976 656e 2061 7320 6120  n be given as a 
-00006a20: 636c 6173 7320 7661 7269 6162 6c65 2e0a  class variable..
-00006a30: 2020 2020 2020 2020 6c61 6265 6c41 6e63          labelAnc
-00006a40: 686f 723a 2054 6865 2070 6f73 6974 696f  hor: The positio
-00006a50: 6e20 6f66 2074 6865 206c 6162 656c 206f  n of the label o
-00006a60: 6e20 7468 6520 6672 616d 6520 7365 7061  n the frame sepa
-00006a70: 7261 746f 722e 0a20 2020 2020 2020 2020  rator..         
-00006a80: 2020 2047 6976 656e 2061 7320 6f6e 6520     Given as one 
-00006a90: 6f66 2074 6865 2063 6172 6469 6e61 6c20  of the cardinal 
-00006aa0: 706f 696e 7473 2e0a 2020 2020 2020 2020  points..        
-00006ab0: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
-00006ac0: 6120 4f53 2d73 7065 6369 6669 6320 6c6f  a OS-specific lo
-00006ad0: 6361 7469 6f6e 2028 606d 6f64 656c 2e43  cation (`model.C
-00006ae0: 502e 6465 6661 756c 7460 292e 0a20 2020  P.default`)..   
-00006af0: 2020 2020 2063 7661 7269 6162 6c65 3a20       cvariable: 
-00006b00: 5573 6520 616e 2065 7874 6572 6e61 6c6c  Use an externall
-00006b10: 7920 6465 6669 6e65 6420 6063 7374 6174  y defined `cstat
-00006b20: 6560 2076 6172 6961 626c 652c 2069 6e73  e` variable, ins
-00006b30: 7465 6164 206f 660a 2020 2020 2020 2020  tead of.        
-00006b40: 2020 2020 6372 6561 7469 6e67 2061 206e      creating a n
-00006b50: 6577 206f 6e65 2073 7065 6369 6669 6320  ew one specific 
-00006b60: 666f 7220 7468 6520 6063 7374 6174 6560  for the `cstate`
-00006b70: 2077 6964 6765 742e 0a20 2020 2020 2020   widget..       
-00006b80: 2063 7661 7269 6162 6c65 4465 6661 756c   cvariableDefaul
-00006b90: 743a 2054 6865 2064 6566 6175 6c74 2076  t: The default v
-00006ba0: 616c 7565 2066 6f72 2060 6373 7461 7465  alue for `cstate
-00006bb0: 602e 0a20 2020 2020 2020 2020 2020 2057  `..            W
-00006bc0: 6865 6e20 604e 6f6e 6560 2c20 7468 6520  hen `None`, the 
-00006bd0: 7661 6c75 6520 6973 206e 6f74 2063 6861  value is not cha
-00006be0: 6e67 6564 2061 7420 7374 6172 742e 0a20  nged at start.. 
-00006bf0: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
-00006c00: 6c74 7320 746f 2073 7461 7274 696e 6720  lts to starting 
-00006c10: 656e 6162 6c65 642c 2075 6e6c 6573 7320  enabled, unless 
-00006c20: 6060 6376 6172 6961 626c 6560 6020 6973  ``cvariable`` is
-00006c30: 2067 6976 656e 2c20 666f 720a 2020 2020   given, for.    
-00006c40: 2020 2020 2020 2020 7768 6963 6820 7468          which th
-00006c50: 6520 7661 6c75 6520 6973 206e 6f74 2063  e value is not c
-00006c60: 6861 6e67 6564 2e0a 2020 2020 2020 2020  hanged..        
-00006c70: 6373 7461 7465 4172 6773 3a20 4578 7472  cstateArgs: Extr
-00006c80: 6120 6172 6775 6d65 6e74 7320 666f 7220  a arguments for 
-00006c90: 7468 6520 6063 7374 6174 6560 2077 6964  the `cstate` wid
-00006ca0: 6765 742c 2060 6373 7461 7465 5f77 6964  get, `cstate_wid
-00006cb0: 6765 7460 2e0a 0a20 2020 2020 2020 2070  get`...        p
-00006cc0: 6172 656e 743a 2054 6865 2070 6172 656e  arent: The paren
-00006cd0: 7420 7769 6467 6574 2e20 4361 6e20 6265  t widget. Can be
-00006ce0: 2061 2060 526f 6f74 5769 6e64 6f77 6020   a `RootWindow` 
-00006cf0: 6f72 2061 6e6f 7468 6572 2060 6d69 7869  or another `mixi
-00006d00: 6e2e 436f 6e74 6169 6e65 7257 6964 6765  n.ContainerWidge
-00006d10: 7460 2e0a 0a20 2020 2053 6565 2041 6c73  t`...    See Als
-00006d20: 6f3a 0a20 2020 2020 2020 2060 4672 616d  o:.        `Fram
-00006d30: 654c 6162 656c 6c65 6460 3a20 4120 7369  eLabelled`: A si
-00006d40: 6d70 6c65 7220 7665 7273 696f 6e20 6f66  mpler version of
-00006d50: 2074 6869 732c 2077 6974 686f 7574 2074   this, without t
-00006d60: 6865 2065 6d62 6564 6465 6420 6368 6563  he embedded chec
-00006d70: 6b62 6f78 2e0a 2020 2020 2727 270a 2020  kbox..    '''.  
-00006d80: 2020 6c61 6265 6c3a 2074 7970 696e 672e    label: typing.
-00006d90: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-00006da0: 4e6f 6e65 0a0a 2020 2020 636c 6173 7320  None..    class 
-00006db0: 5f5f 775f 6373 7461 7465 2843 6865 636b  __w_cstate(Check
-00006dc0: 626f 7829 3a0a 2020 2020 2020 2020 6973  box):.        is
-00006dd0: 4865 6c70 6572 203d 2054 7275 650a 0a20  Helper = True.. 
-00006de0: 2020 2063 7374 6174 655f 7769 6467 6574     cstate_widget
-00006df0: 3a20 5f5f 775f 6373 7461 7465 0a20 2020  : __w_cstate.   
-00006e00: 2027 2727 5468 6520 7769 6467 6574 2066   '''The widget f
-00006e10: 6f72 2074 6865 2065 6d62 6564 6465 6420  or the embedded 
-00006e20: 6043 6865 636b 626f 7860 2e0a 0a20 2020  `Checkbox`...   
-00006e30: 2055 7365 7320 7468 6520 6063 7374 6174   Uses the `cstat
-00006e40: 6560 2076 6172 6961 626c 652e 0a0a 2020  e` variable...  
-00006e50: 2020 4e6f 7465 3a0a 2020 2020 2020 2020    Note:.        
-00006e60: 5468 6520 7769 6467 6574 2074 7970 6520  The widget type 
-00006e70: 6973 2061 206c 6f63 616c 2060 4368 6563  is a local `Chec
-00006e80: 6b62 6f78 6020 7375 6263 6c61 7373 2c20  kbox` subclass, 
-00006e90: 7370 6563 6966 6963 2066 6f72 2074 6869  specific for thi
-00006ea0: 7320 7769 6467 6574 2e0a 2020 2020 2727  s widget..    ''
-00006eb0: 270a 2020 2020 6373 7461 7465 3a20 7661  '.    cstate: va
-00006ec0: 722e 426f 6f6c 6561 6e0a 2020 2020 2727  r.Boolean.    ''
-00006ed0: 2754 6865 2076 6172 6961 626c 6520 686f  'The variable ho
-00006ee0: 6c64 696e 6720 7468 6520 656d 6265 6464  lding the embedd
-00006ef0: 6564 2060 4368 6563 6b62 6f78 6020 7374  ed `Checkbox` st
-00006f00: 6174 652e 0a0a 2020 2020 5573 6564 206f  ate...    Used o
-00006f10: 6e20 7468 6520 6063 7374 6174 655f 7769  n the `cstate_wi
-00006f20: 6467 6574 602e 0a0a 2020 2020 5365 6520  dget`...    See 
-00006f30: 416c 736f 3a0a 2020 2020 2020 2020 6060  Also:.        ``
-00006f40: 6376 6172 6961 626c 6560 603a 2054 6869  cvariable``: Thi
-00006f50: 7320 6361 6e20 6265 2063 6f6e 6669 6775  s can be configu
-00006f60: 7265 6420 6173 2061 6e20 6578 7465 726e  red as an extern
-00006f70: 616c 2076 6172 6961 626c 652e 0a20 2020  al variable..   
-00006f80: 2027 2727 0a0a 2020 2020 6465 6620 5f5f   '''..    def __
-00006f90: 696e 6974 5f5f 2873 656c 662c 2070 6172  init__(self, par
-00006fa0: 656e 742c 202a 6172 6773 2c20 6c61 6265  ent, *args, labe
-00006fb0: 6c3a 2074 7970 696e 672e 4f70 7469 6f6e  l: typing.Option
-00006fc0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c20  al[str] = None, 
-00006fd0: 6c61 6265 6c41 6e63 686f 723a 206d 6f64  labelAnchor: mod
-00006fe0: 656c 2e43 5020 3d20 6d6f 6465 6c2e 4350  el.CP = model.CP
-00006ff0: 2e64 6566 6175 6c74 2c0a 2020 2020 2020  .default,.      
-00007000: 2020 2020 2020 2020 2020 2063 7661 7269             cvari
-00007010: 6162 6c65 3a20 7479 7069 6e67 2e4f 7074  able: typing.Opt
-00007020: 696f 6e61 6c5b 7661 722e 426f 6f6c 6561  ional[var.Boolea
-00007030: 6e5d 203d 204e 6f6e 652c 2063 7661 7269  n] = None, cvari
-00007040: 6162 6c65 4465 6661 756c 743a 2074 7970  ableDefault: typ
-00007050: 696e 672e 4f70 7469 6f6e 616c 5b62 6f6f  ing.Optional[boo
-00007060: 6c5d 203d 204e 6f6e 652c 0a20 2020 2020  l] = None,.     
-00007070: 2020 2020 2020 2020 2020 2020 6373 7461              csta
-00007080: 7465 4172 6773 3a20 7479 7069 6e67 2e4f  teArgs: typing.O
-00007090: 7074 696f 6e61 6c5b 7479 7069 6e67 2e4d  ptional[typing.M
-000070a0: 6170 7069 6e67 5b73 7472 2c20 7479 7069  apping[str, typi
-000070b0: 6e67 2e41 6e79 5d5d 203d 204e 6f6e 652c  ng.Any]] = None,
-000070c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000070d0: 2020 2a2a 6b77 6172 6773 293a 0a20 2020    **kwargs):.   
-000070e0: 2020 2020 2023 2043 7265 6174 6520 7468       # Create th
-000070f0: 6520 6368 6563 6b62 6f78 2077 6964 6765  e checkbox widge
-00007100: 740a 2020 2020 2020 2020 6368 6f73 656e  t.        chosen
-00007110: 5f6c 6162 656c 203d 2073 656c 662e 6c61  _label = self.la
-00007120: 6265 6c20 6f72 206c 6162 656c 0a20 2020  bel or label.   
-00007130: 2020 2020 2069 6620 6368 6f73 656e 5f6c       if chosen_l
-00007140: 6162 656c 2069 7320 4e6f 6e65 3a0a 2020  abel is None:.  
-00007150: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00007160: 5661 6c75 6545 7272 6f72 2827 7b73 656c  ValueError('{sel
-00007170: 6621 727d 3a20 4d69 7373 696e 6720 7265  f!r}: Missing re
-00007180: 7175 6972 6564 206c 6162 656c 2729 0a20  quired label'). 
-00007190: 2020 2020 2020 2063 7374 6174 6541 7267         cstateArg
-000071a0: 7320 3d20 6469 6374 2863 7374 6174 6541  s = dict(cstateA
-000071b0: 7267 7320 6f72 207b 7d29 0a20 2020 2020  rgs or {}).     
-000071c0: 2020 2063 7374 6174 6541 7267 732e 7570     cstateArgs.up
-000071d0: 6461 7465 287b 2020 2320 4f76 6572 7269  date({  # Overri
-000071e0: 6465 2063 7374 6174 6520 6172 6775 6d65  de cstate argume
-000071f0: 6e74 730a 2020 2020 2020 2020 2020 2020  nts.            
-00007200: 2776 6172 6961 626c 6527 3a20 6376 6172  'variable': cvar
-00007210: 6961 626c 652c 0a20 2020 2020 2020 2020  iable,.         
-00007220: 2020 2027 6c61 6265 6c27 3a20 6368 6f73     'label': chos
-00007230: 656e 5f6c 6162 656c 2c0a 2020 2020 2020  en_label,.      
-00007240: 2020 2020 2020 2772 6561 646f 6e6c 7927        'readonly'
-00007250: 3a20 4661 6c73 652c 0a20 2020 2020 2020  : False,.       
-00007260: 207d 290a 2020 2020 2020 2020 6373 7461   }).        csta
-00007270: 7465 5f77 6964 6765 7420 3d20 7365 6c66  te_widget = self
-00007280: 2e5f 5f63 6c61 7373 5f5f 2e5f 5f77 5f63  .__class__.__w_c
-00007290: 7374 6174 6528 7061 7265 6e74 2c20 2a2a  state(parent, **
-000072a0: 6373 7461 7465 4172 6773 290a 2020 2020  cstateArgs).    
-000072b0: 2020 2020 6173 7365 7274 2069 7369 6e73      assert isins
-000072c0: 7461 6e63 6528 6373 7461 7465 5f77 6964  tance(cstate_wid
-000072d0: 6765 742e 7661 7269 6162 6c65 2c20 7661  get.variable, va
-000072e0: 722e 426f 6f6c 6561 6e29 2c20 6627 7b73  r.Boolean), f'{s
-000072f0: 656c 6621 727d 2063 6865 636b 626f 7820  elf!r} checkbox 
-00007300: 7769 6467 6574 2069 7320 6e6f 7420 6120  widget is not a 
-00007310: 7369 6d70 6c65 2062 6f6f 6c65 616e 270a  simple boolean'.
-00007320: 2020 2020 2020 2020 7365 6c66 2e63 7374          self.cst
-00007330: 6174 6520 3d20 6373 7461 7465 5f77 6964  ate = cstate_wid
-00007340: 6765 742e 7661 7269 6162 6c65 0a20 2020  get.variable.   
-00007350: 2020 2020 2023 2055 7375 616c 2049 6e69       # Usual Ini
-00007360: 7469 616c 697a 6174 696f 6e0a 2020 2020  tialization.    
-00007370: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
-00007380: 6974 5f5f 2870 6172 656e 742c 206c 6162  it__(parent, lab
-00007390: 656c 7769 6467 6574 3d63 7374 6174 655f  elwidget=cstate_
-000073a0: 7769 6467 6574 2c20 6c61 6265 6c61 6e63  widget, labelanc
-000073b0: 686f 723d 6c61 6265 6c41 6e63 686f 722e  hor=labelAnchor.
-000073c0: 7661 6c75 6529 0a20 2020 2020 2020 2073  value).        s
-000073d0: 656c 662e 696e 6974 5f63 6f6e 7461 696e  elf.init_contain
-000073e0: 6572 282a 6172 6773 2c20 2a2a 6b77 6172  er(*args, **kwar
-000073f0: 6773 290a 2020 2020 2020 2020 2320 436f  gs).        # Co
-00007400: 6e66 6967 7572 6520 7468 6520 6368 6563  nfigure the chec
-00007410: 6b62 6f78 2077 6964 6765 740a 2020 2020  kbox widget.    
-00007420: 2020 2020 7365 6c66 2e63 7374 6174 655f      self.cstate_
-00007430: 7769 6467 6574 203d 2063 7374 6174 655f  widget = cstate_
-00007440: 7769 6467 6574 0a20 2020 2020 2020 2073  widget.        s
-00007450: 656c 662e 6373 7461 7465 5f77 6964 6765  elf.cstate_widge
-00007460: 742e 7472 6163 6528 7365 6c66 2e6f 6e43  t.trace(self.onC
-00007470: 6861 6e67 6564 5f63 7374 6174 6529 0a20  hanged_cstate). 
-00007480: 2020 2020 2020 2023 2023 2053 6574 7570         # # Setup
-00007490: 2074 6865 2064 6566 6175 6c74 2076 616c   the default val
-000074a0: 7565 2066 6f72 2074 6861 7420 7769 6467  ue for that widg
-000074b0: 6574 0a20 2020 2020 2020 2069 6620 5f5f  et.        if __
-000074c0: 6465 6275 675f 5f3a 0a20 2020 2020 2020  debug__:.       
-000074d0: 2020 2020 2069 6620 6376 6172 6961 626c       if cvariabl
-000074e0: 6520 6973 206e 6f74 204e 6f6e 6520 616e  e is not None an
-000074f0: 6420 6376 6172 6961 626c 6544 6566 6175  d cvariableDefau
-00007500: 6c74 2069 7320 6e6f 7420 4e6f 6e65 3a0a  lt is not None:.
-00007510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007520: 7761 726e 696e 6773 2e77 6172 6e28 6627  warnings.warn(f'
-00007530: 7b73 656c 667d 3a20 6376 6172 6961 626c  {self}: cvariabl
-00007540: 653a 2053 6574 7469 6e67 2061 2064 6566  e: Setting a def
-00007550: 6175 6c74 2077 6974 6820 616e 2065 7874  ault with an ext
-00007560: 6572 6e61 6c20 7661 7269 6162 6c65 2729  ernal variable')
-00007570: 0a20 2020 2020 2020 2069 6620 6376 6172  .        if cvar
-00007580: 6961 626c 6520 6973 204e 6f6e 6520 616e  iable is None an
-00007590: 6420 6376 6172 6961 626c 6544 6566 6175  d cvariableDefau
-000075a0: 6c74 2069 7320 4e6f 6e65 3a0a 2020 2020  lt is None:.    
-000075b0: 2020 2020 2020 2020 6376 6172 6961 626c          cvariabl
-000075c0: 6544 6566 6175 6c74 203d 2054 7275 650a  eDefault = True.
-000075d0: 2020 2020 2020 2020 6966 2063 7661 7269          if cvari
-000075e0: 6162 6c65 4465 6661 756c 7420 6973 206e  ableDefault is n
-000075f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00007600: 2020 2020 2073 656c 662e 6373 7461 7465       self.cstate
-00007610: 2e73 6574 2863 7661 7269 6162 6c65 4465  .set(cvariableDe
-00007620: 6661 756c 7429 0a0a 2020 2020 6465 6620  fault)..    def 
-00007630: 7374 6174 655f 6765 7428 7365 6c66 2c20  state_get(self, 
-00007640: 2a61 7267 732c 2076 6964 5f75 7073 7472  *args, vid_upstr
-00007650: 6561 6d3a 2074 7970 696e 672e 4f70 7469  eam: typing.Opti
-00007660: 6f6e 616c 5b74 7970 696e 672e 5365 745b  onal[typing.Set[
-00007670: 7374 725d 5d20 3d20 4e6f 6e65 2c20 2a2a  str]] = None, **
-00007680: 6b77 6172 6773 2920 2d3e 206d 6f64 656c  kwargs) -> model
-00007690: 2e57 5374 6174 655b 626f 6f6c 2c20 7479  .WState[bool, ty
-000076a0: 7069 6e67 2e41 6e79 5d3a 0a20 2020 2020  ping.Any]:.     
-000076b0: 2020 2027 2727 2727 2720 2023 2044 6f20     ''''''  # Do 
-000076c0: 6e6f 7420 646f 6375 6d65 6e74 0a20 2020  not document.   
-000076d0: 2020 2020 2063 6964 203d 2066 6e2e 766e       cid = fn.vn
-000076e0: 616d 6528 7365 6c66 2e63 7374 6174 6529  ame(self.cstate)
-000076f0: 0a20 2020 2020 2020 2069 6620 7669 645f  .        if vid_
-00007700: 7570 7374 7265 616d 2061 6e64 2063 6964  upstream and cid
-00007710: 2069 6e20 7669 645f 7570 7374 7265 616d   in vid_upstream
-00007720: 3a0a 2020 2020 2020 2020 2020 2020 6373  :.            cs
-00007730: 7461 7465 203d 204e 6f6e 650a 2020 2020  tate = None.    
-00007740: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00007750: 2020 2020 2020 6373 7461 7465 203d 2073        cstate = s
-00007760: 656c 662e 6373 7461 7465 2e67 6574 2829  elf.cstate.get()
-00007770: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00007780: 6d6f 6465 6c2e 5753 7461 7465 280a 2020  model.WState(.  
-00007790: 2020 2020 2020 2020 2020 6373 7461 7465            cstate
-000077a0: 2c0a 2020 2020 2020 2020 2020 2020 7375  ,.            su
-000077b0: 7065 7228 292e 7374 6174 655f 6765 7428  per().state_get(
-000077c0: 2a61 7267 732c 2076 6964 5f75 7073 7472  *args, vid_upstr
-000077d0: 6561 6d3d 7669 645f 7570 7374 7265 616d  eam=vid_upstream
-000077e0: 2c20 2a2a 6b77 6172 6773 292c 0a20 2020  , **kwargs),.   
-000077f0: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
-00007800: 7374 6174 655f 7365 7428 7365 6c66 2c20  state_set(self, 
-00007810: 7374 6174 653a 206d 6f64 656c 2e57 5374  state: model.WSt
-00007820: 6174 655b 626f 6f6c 2c20 7479 7069 6e67  ate[bool, typing
-00007830: 2e41 6e79 5d2c 202a 6172 6773 2c20 2a2a  .Any], *args, **
-00007840: 6b77 6172 6773 293a 0a20 2020 2020 2020  kwargs):.       
-00007850: 2027 2727 2727 2720 2023 2044 6f20 6e6f   ''''''  # Do no
-00007860: 7420 646f 6375 6d65 6e74 0a20 2020 2020  t document.     
-00007870: 2020 2069 6620 7374 6174 652e 7374 6174     if state.stat
-00007880: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-00007890: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-000078a0: 7420 6973 696e 7374 616e 6365 2873 7461  t isinstance(sta
-000078b0: 7465 2e73 7461 7465 2c20 626f 6f6c 292c  te.state, bool),
-000078c0: 2066 2749 6e76 616c 6964 2057 5374 6174   f'Invalid WStat
-000078d0: 653a 207b 7374 6174 6521 727d 270a 2020  e: {state!r}'.  
-000078e0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-000078f0: 7374 6174 652e 7365 7428 7374 6174 652e  state.set(state.
-00007900: 7374 6174 6529 0a20 2020 2020 2020 2073  state).        s
-00007910: 7570 6572 2829 2e73 7461 7465 5f73 6574  uper().state_set
-00007920: 2873 7461 7465 2e73 7562 7374 6174 652c  (state.substate,
-00007930: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
-00007940: 290a 0a20 2020 2064 6566 2073 6574 5f67  )..    def set_g
-00007950: 7569 5f73 7461 7465 2873 656c 662c 2073  ui_state(self, s
-00007960: 7461 7465 3a20 7479 7069 6e67 2e4f 7074  tate: typing.Opt
-00007970: 696f 6e61 6c5b 6d6f 6465 6c2e 4775 6953  ional[model.GuiS
-00007980: 7461 7465 5d20 3d20 4e6f 6e65 2c20 2a2a  tate] = None, **
-00007990: 6b77 6172 6773 2920 2d3e 204e 6f6e 653a  kwargs) -> None:
-000079a0: 0a20 2020 2020 2020 2023 2022 5472 6163  .        # "Trac
-000079b0: 6522 2074 6865 2066 7261 6d65 2065 6e61  e" the frame ena
-000079c0: 626c 6564 2073 7461 7475 730a 2020 2020  bled status.    
-000079d0: 2020 2020 6672 616d 655f 656e 6162 6c65      frame_enable
-000079e0: 6420 3d20 6b77 6172 6773 2e67 6574 2827  d = kwargs.get('
-000079f0: 656e 6162 6c65 6427 2c20 4e6f 6e65 2920  enabled', None) 
-00007a00: 6966 2073 7461 7465 2069 7320 4e6f 6e65  if state is None
-00007a10: 2065 6c73 6520 7374 6174 652e 656e 6162   else state.enab
-00007a20: 6c65 640a 2020 2020 2020 2020 7375 7065  led.        supe
-00007a30: 7228 292e 7365 745f 6775 695f 7374 6174  r().set_gui_stat
-00007a40: 6528 7374 6174 652c 202a 2a6b 7761 7267  e(state, **kwarg
-00007a50: 7329 0a20 2020 2020 2020 2069 6620 6973  s).        if is
-00007a60: 696e 7374 616e 6365 2866 7261 6d65 5f65  instance(frame_e
-00007a70: 6e61 626c 6564 2c20 626f 6f6c 293a 0a20  nabled, bool):. 
-00007a80: 2020 2020 2020 2020 2020 2073 7461 7465             state
-00007a90: 5f65 6e61 626c 6564 203d 2073 656c 662e  _enabled = self.
-00007aa0: 6373 7461 7465 2e67 6574 2829 0a20 2020  cstate.get().   
-00007ab0: 2020 2020 2020 2020 2023 2069 6620 5f5f           # if __
-00007ac0: 6465 6275 675f 5f3a 0a20 2020 2020 2020  debug__:.       
-00007ad0: 2020 2020 2023 2020 2020 206c 6f67 6765       #     logge
-00007ae0: 722e 6465 6275 6728 6627 537c 207b 7365  r.debug(f'S| {se
-00007af0: 6c66 7d3a 2046 3d7b 6672 616d 655f 656e  lf}: F={frame_en
-00007b00: 6162 6c65 647d 2053 3d7b 7374 6174 655f  abled} S={state_
-00007b10: 656e 6162 6c65 647d 2729 0a20 2020 2020  enabled}').     
-00007b20: 2020 2020 2020 2073 656c 662e 6373 7461         self.csta
-00007b30: 7465 5f77 6964 6765 742e 6773 7461 7465  te_widget.gstate
-00007b40: 203d 206d 6f64 656c 2e47 7569 5374 6174   = model.GuiStat
-00007b50: 6528 656e 6162 6c65 643d 6672 616d 655f  e(enabled=frame_
-00007b60: 656e 6162 6c65 6429 0a20 2020 2020 2020  enabled).       
-00007b70: 2020 2020 2073 656c 662e 7365 745f 6775       self.set_gu
-00007b80: 695f 7375 6273 7461 7465 2865 6e61 626c  i_substate(enabl
-00007b90: 6564 3d66 7261 6d65 5f65 6e61 626c 6564  ed=frame_enabled
-00007ba0: 2061 6e64 2073 7461 7465 5f65 6e61 626c   and state_enabl
-00007bb0: 6564 290a 2020 2020 2020 2020 2020 2020  ed).            
-00007bc0: 2320 544f 444f 3a20 756e 7365 744f 6e44  # TODO: unsetOnD
-00007bd0: 6973 6162 6c65 0a20 2020 2020 2020 2020  isable.         
-00007be0: 2020 2023 2054 4f44 4f3a 2073 6574 4f6e     # TODO: setOn
-00007bf0: 456e 6162 6c65 0a0a 2020 2020 6465 6620  Enable..    def 
-00007c00: 6f6e 4368 616e 6765 645f 6373 7461 7465  onChanged_cstate
-00007c10: 2873 656c 662c 2063 7374 6174 652c 2065  (self, cstate, e
-00007c20: 7479 7065 293a 0a20 2020 2020 2020 2061  type):.        a
-00007c30: 7373 6572 7420 6574 7970 6520 3d3d 2027  ssert etype == '
-00007c40: 7772 6974 6527 0a20 2020 2020 2020 2073  write'.        s
-00007c50: 7461 7475 7320 3d20 6373 7461 7465 2e67  tatus = cstate.g
-00007c60: 6574 2829 0a20 2020 2020 2020 2066 7261  et().        fra
-00007c70: 6d65 5f65 6e61 626c 6564 203d 2073 656c  me_enabled = sel
-00007c80: 662e 6773 7461 7465 2e65 6e61 626c 6564  f.gstate.enabled
-00007c90: 0a20 2020 2020 2020 2023 2069 6620 5f5f  .        # if __
-00007ca0: 6465 6275 675f 5f3a 0a20 2020 2020 2020  debug__:.       
-00007cb0: 2023 2020 2020 206c 6f67 6765 722e 6465   #     logger.de
-00007cc0: 6275 6728 6627 7b73 656c 667d 3a20 533d  bug(f'{self}: S=
-00007cd0: 7b73 7461 7475 737d 2046 653d 7b66 7261  {status} Fe={fra
-00007ce0: 6d65 5f65 6e61 626c 6564 7d27 290a 2020  me_enabled}').  
-00007cf0: 2020 2020 2020 7365 6c66 2e73 6574 5f67        self.set_g
-00007d00: 7569 5f73 7562 7374 6174 6528 6d6f 6465  ui_substate(mode
-00007d10: 6c2e 4775 6953 7461 7465 2865 6e61 626c  l.GuiState(enabl
-00007d20: 6564 3d66 7261 6d65 5f65 6e61 626c 6564  ed=frame_enabled
-00007d30: 2061 6e64 2073 7461 7475 7329 290a 0a0a   and status))...
-00007d40: 2320 544f 444f 3a20 5573 6520 6074 6b2e  # TODO: Use `tk.
-00007d50: 7363 726f 6c6c 6564 7465 7874 2e53 6372  scrolledtext.Scr
-00007d60: 6f6c 6c65 6454 6578 7460 3f20 446f 2074  olledText`? Do t
-00007d70: 6865 2073 616d 6520 7468 696e 6720 666f  he same thing fo
-00007d80: 7220 6d75 6c74 6970 6c65 2077 6964 6765  r multiple widge
-00007d90: 7473 3f0a 636c 6173 7320 456e 7472 794d  ts?.class EntryM
-00007da0: 756c 7469 6c69 6e65 2874 6b2e 5465 7874  ultiline(tk.Text
-00007db0: 2c20 6d69 7869 6e2e 5369 6e67 6c65 5769  , mixin.SingleWi
-00007dc0: 6467 6574 293a 0a20 2020 2027 2727 4120  dget):.    '''A 
-00007dd0: 6d75 6c74 696c 696e 6520 7465 7874 2077  multiline text w
-00007de0: 6964 6765 742c 2073 7570 706f 7274 696e  idget, supportin
-00007df0: 6720 604c 544d 4c60 2063 6f6e 7465 6e74  g `LTML` content
-00007e00: 732e 0a0a 2020 2020 5468 6973 2069 7320  s...    This is 
-00007e10: 6120 6d75 6c74 696c 696e 6520 7665 7273  a multiline vers
-00007e20: 696f 6e20 6f66 2074 6865 2060 456e 7472  ion of the `Entr
-00007e30: 7960 2077 6964 6765 742c 2077 6974 6820  y` widget, with 
-00007e40: 7269 6368 2074 6578 740a 2020 2020 6361  rich text.    ca
-00007e50: 7061 6269 6c69 7469 6573 2e0a 2020 2020  pabilities..    
-00007e60: 5375 7070 6f72 7473 206f 6e6c 7920 7468  Supports only th
-00007e70: 6520 7265 6164 6f6e 6c79 2073 7461 7465  e readonly state
-00007e80: 2c20 7468 6174 2069 732c 2074 6865 2077  , that is, the w
-00007e90: 6964 6765 7420 636f 6e74 656e 7473 2063  idget contents c
-00007ea0: 616e 206f 6e6c 7920 6265 0a20 2020 2065  an only be.    e
-00007eb0: 6469 7465 6420 7072 6f67 7261 6d61 7469  dited programati
-00007ec0: 6361 6c6c 792e 0a0a 2020 2020 5468 6520  cally...    The 
-00007ed0: 7374 6174 6520 6973 2061 2073 696e 676c  state is a singl
-00007ee0: 6520 6073 7472 6020 7661 6c75 652c 2069  e `str` value, i
-00007ef0: 6e74 6572 6e61 6c6c 7920 7061 7273 6564  nternally parsed
-00007f00: 2074 6f20 6070 6172 7365 722e 4c54 4d4c   to `parser.LTML
-00007f10: 0a20 2020 203c 4c54 4d4c 3e60 2e0a 0a20  .    <LTML>`... 
-00007f20: 2020 2054 6865 7265 2069 7320 6e6f 2050     There is no P
-00007f30: 7974 686f 6e20 646f 6375 6d65 6e74 6174  ython documentat
-00007f40: 696f 6e2c 2073 6565 2060 6054 6b60 6020  ion, see ``Tk`` 
-00007f50: 6074 6b2e 5465 7874 203c 6874 7470 733a  `tk.Text <https:
-00007f60: 2f2f 7777 772e 7463 6c2e 746b 2f6d 616e  //www.tcl.tk/man
-00007f70: 2f74 636c 2f54 6b43 6d64 2f74 6578 742e  /tcl/TkCmd/text.
-00007f80: 6874 6d3e 605f 2064 6f63 756d 656e 7461  htm>`_ documenta
-00007f90: 7469 6f6e 2e0a 0a20 2020 2041 7267 733a  tion...    Args:
-00007fa0: 0a20 2020 2020 2020 2076 6172 6961 626c  .        variabl
-00007fb0: 653a 2055 7365 2061 6e20 6578 7465 726e  e: Use an extern
-00007fc0: 616c 6c79 2064 6566 696e 6564 2076 6172  ally defined var
-00007fd0: 6961 626c 652c 2069 6e73 7465 6164 206f  iable, instead o
-00007fe0: 6620 6372 6561 7469 6e67 2061 206e 6577  f creating a new
-00007ff0: 0a20 2020 2020 2020 2020 2020 206f 6e65  .            one
-00008000: 2073 7065 6369 6669 6320 666f 7220 7468   specific for th
-00008010: 6973 2077 6964 6765 742e 0a20 2020 2020  is widget..     
-00008020: 2020 2073 7479 6c65 3a20 436f 6e66 6967     style: Config
-00008030: 7572 6520 7468 6520 7769 6467 6574 2073  ure the widget s
-00008040: 7479 6c65 2e0a 0a20 2020 2020 2020 2070  tyle...        p
-00008050: 6172 656e 743a 2054 6865 2070 6172 656e  arent: The paren
-00008060: 7420 7769 6467 6574 2e20 4361 6e20 6265  t widget. Can be
-00008070: 2061 2060 526f 6f74 5769 6e64 6f77 6020   a `RootWindow` 
-00008080: 6f72 2061 6e6f 7468 6572 2060 6d69 7869  or another `mixi
-00008090: 6e2e 436f 6e74 6169 6e65 7257 6964 6765  n.ContainerWidge
-000080a0: 7460 2e0a 0a20 2020 204e 6f74 653a 0a0a  t`...    Note:..
-000080b0: 2020 2020 2020 2020 5468 6520 756e 6465          The unde
-000080c0: 726c 7969 6e67 2077 6964 6765 7420 6973  rlying widget is
-000080d0: 206e 6f74 2070 6172 7420 6f66 2060 7474   not part of `tt
-000080e0: 6b20 3c74 6b69 6e74 6572 2e74 746b 3e60  k <tkinter.ttk>`
-000080f0: 206c 696b 6520 6d6f 7374 206f 7468 6572   like most other
-00008100: 732e 2041 6c6c 0a20 2020 2020 2020 2065  s. All.        e
-00008110: 6666 6f72 7473 2061 7265 2065 7870 656e  fforts are expen
-00008120: 6465 6420 746f 206d 616b 6520 7468 6973  ded to make this
-00008130: 2061 6e20 696d 706c 656d 656e 7461 7469   an implementati
-00008140: 6f6e 2064 6574 6169 6c2c 2077 6974 686f  on detail, witho
-00008150: 7574 0a20 2020 2020 2020 2070 7261 6374  ut.        pract
-00008160: 6963 616c 2065 6666 6563 7473 2e0a 2020  ical effects..  
-00008170: 2020 2727 270a 2020 2020 7374 6174 655f    '''.    state_
-00008180: 7479 7065 203d 2076 6172 2e53 7472 696e  type = var.Strin
-00008190: 670a 2020 2020 5f62 696e 6469 6e67 735f  g.    _bindings_
-000081a0: 7461 673a 2074 7970 696e 672e 4d75 7461  tag: typing.Muta
-000081b0: 626c 654d 6170 7069 6e67 5b74 7970 696e  bleMapping[typin
-000081c0: 672e 5475 706c 655b 7374 722c 2073 7472  g.Tuple[str, str
-000081d0: 5d2c 206d 6f64 656c 2e42 696e 6469 6e67  ], model.Binding
-000081e0: 5461 675d 0a20 2020 2027 2727 5374 6f72  Tag].    '''Stor
-000081f0: 6520 616c 6c20 7769 6467 6574 2060 4269  e all widget `Bi
-00008200: 6e64 696e 6754 6167 6020 6f62 6a65 6374  ndingTag` object
-00008210: 732c 206b 6579 6564 2062 7920 6060 2874  s, keyed by ``(t
-00008220: 6167 2c20 6e61 6d65 2960 6020 2873 6565  ag, name)`` (see
-00008230: 2060 6269 6e64 696e 675f 7461 6760 292e   `binding_tag`).
-00008240: 2727 270a 0a20 2020 2040 6461 7461 636c  '''..    @datacl
-00008250: 6173 730a 2020 2020 636c 6173 7320 5374  ass.    class St
-00008260: 796c 6528 6d6f 6465 6c2e 5753 7479 6c65  yle(model.WStyle
-00008270: 293a 0a20 2020 2020 2020 2027 2727 6045  ):.        '''`E
-00008280: 6e74 7279 4d75 6c74 696c 696e 6560 2073  ntryMultiline` s
-00008290: 7479 6c65 206f 626a 6563 742e 0a0a 2020  tyle object...  
-000082a0: 2020 2020 2020 5468 6573 6520 6172 6520        These are 
-000082b0: 7468 6520 7365 7474 696e 6773 3a0a 0a20  the settings:.. 
-000082c0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-000082d0: 2020 2020 2020 2020 2066 6f6e 745f 6261           font_ba
-000082e0: 7365 3a20 4261 7365 2046 6f6e 7420 6e61  se: Base Font na
-000082f0: 6d65 2c20 666f 7220 616c 6c20 7468 6520  me, for all the 
-00008300: 7769 6467 6574 2e0a 2020 2020 2020 2020  widget..        
-00008310: 2020 2020 636f 6c6f 7572 5f62 675f 6f6e      colour_bg_on
-00008320: 3a20 5769 6467 6574 2062 6163 6b67 726f  : Widget backgro
-00008330: 756e 642c 2077 6865 6e20 656e 6162 6c65  und, when enable
-00008340: 642e 0a20 2020 2020 2020 2020 2020 2063  d..            c
-00008350: 6f6c 6f75 725f 6267 5f6f 6666 3a20 5769  olour_bg_off: Wi
-00008360: 6467 6574 2062 6163 6b67 726f 756e 642c  dget background,
-00008370: 2077 6865 6e20 6469 7361 626c 6564 2e0a   when disabled..
-00008380: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
-00008390: 7572 5f6c 696e 6b5f 6e6f 726d 616c 3a20  ur_link_normal: 
-000083a0: 4879 7065 726c 696e 6b20 666f 7265 6772  Hyperlink foregr
-000083b0: 6f75 6e64 2063 6f6c 6f75 722c 206e 6f72  ound colour, nor
-000083c0: 6d61 6c20 6c69 6e6b 732e 0a20 2020 2020  mal links..     
-000083d0: 2020 2020 2020 2063 6f6c 6f75 725f 6c69         colour_li
-000083e0: 6e6b 5f76 6973 6974 6564 3a20 4879 7065  nk_visited: Hype
-000083f0: 726c 696e 6b20 666f 7265 6772 6f75 6e64  rlink foreground
-00008400: 2063 6f6c 6f75 722c 2076 6973 6974 6564   colour, visited
-00008410: 206c 696e 6b73 2e0a 2020 2020 2020 2020   links..        
-00008420: 2727 270a 2020 2020 2020 2020 666f 6e74  '''.        font
-00008430: 5f62 6173 653a 2073 7472 203d 2027 546b  _base: str = 'Tk
-00008440: 5465 7874 466f 6e74 2720 2023 2054 6869  TextFont'  # Thi
-00008450: 7320 666f 6e74 2073 686f 756c 6420 6265  s font should be
-00008460: 2075 7365 6420 666f 7220 7573 6572 2074   used for user t
-00008470: 6578 7420 696e 2065 6e74 7279 2077 6964  ext in entry wid
-00008480: 6765 7473 2c20 6c69 7374 626f 7865 7320  gets, listboxes 
-00008490: 6574 632e 0a20 2020 2020 2020 2063 6f6c  etc..        col
-000084a0: 6f75 725f 6267 5f6f 6e3a 2073 7472 203d  our_bg_on: str =
-000084b0: 2027 7768 6974 6527 0a20 2020 2020 2020   'white'.       
-000084c0: 2063 6f6c 6f75 725f 6267 5f6f 6666 3a20   colour_bg_off: 
-000084d0: 7374 7220 3d20 276c 6967 6874 6772 6579  str = 'lightgrey
-000084e0: 270a 2020 2020 2020 2020 636f 6c6f 7572  '.        colour
-000084f0: 5f6c 696e 6b5f 6e6f 726d 616c 3a20 7374  _link_normal: st
-00008500: 7220 3d20 2762 6c75 6527 0a20 2020 2020  r = 'blue'.     
-00008510: 2020 2063 6f6c 6f75 725f 6c69 6e6b 5f76     colour_link_v
-00008520: 6973 6974 6564 3a20 7374 7220 3d20 2770  isited: str = 'p
-00008530: 7572 706c 6527 0a0a 2020 2020 6465 6620  urple'..    def 
-00008540: 5f5f 696e 6974 5f5f 2873 656c 662c 2070  __init__(self, p
-00008550: 6172 656e 742c 202a 2c20 7661 7269 6162  arent, *, variab
-00008560: 6c65 3a20 7661 722e 5374 7269 6e67 203d  le: var.String =
-00008570: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-00008580: 2020 2020 2020 2020 7374 796c 653a 2053          style: S
-00008590: 7479 6c65 203d 2053 7479 6c65 285f 6465  tyle = Style(_de
-000085a0: 6661 756c 743d 5472 7565 292c 0a20 2020  fault=True),.   
-000085b0: 2020 2020 2020 2020 2020 2020 2020 2a2a                **
-000085c0: 6b77 6172 6773 293a 0a20 2020 2020 2020  kwargs):.       
-000085d0: 2073 656c 662e 7773 7479 6c65 203d 2073   self.wstyle = s
-000085e0: 7479 6c65 0a20 2020 2020 2020 2073 656c  tyle.        sel
-000085f0: 662e 696e 6974 5f73 696e 676c 6528 7661  f.init_single(va
-00008600: 7269 6162 6c65 290a 2020 2020 2020 2020  riable).        
-00008610: 6b77 6172 6773 2e70 6f70 2827 7374 6174  kwargs.pop('stat
-00008620: 6527 2c20 4e6f 6e65 2920 2023 2053 7570  e', None)  # Sup
-00008630: 706f 7274 206f 6e6c 7920 7265 6164 6f6e  port only readon
-00008640: 6c79 2073 7461 7465 0a20 2020 2020 2020  ly state.       
-00008650: 206b 7761 7267 735b 2766 6f6e 7427 5d20   kwargs['font'] 
-00008660: 3d20 7374 796c 652e 666f 6e74 5f62 6173  = style.font_bas
-00008670: 6520 2023 204f 7665 7272 6964 6520 7468  e  # Override th
-00008680: 6520 6261 7365 2066 6f6e 740a 2020 2020  e base font.    
-00008690: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
-000086a0: 6974 5f5f 2870 6172 656e 742c 202a 2a6b  it__(parent, **k
-000086b0: 7761 7267 7329 2020 2320 746b 2e45 6e74  wargs)  # tk.Ent
-000086c0: 7279 0a20 2020 2020 2020 2072 6561 646f  ry.        reado
-000086d0: 6e6c 7920 3d20 5472 7565 2020 2320 5375  nly = True  # Su
-000086e0: 7070 6f72 7420 6f6e 6c79 2072 6561 646f  pport only reado
-000086f0: 6e6c 7920 7374 6174 652c 2066 6f72 206e  nly state, for n
-00008700: 6f77 2e2e 2e0a 2020 2020 2020 2020 2320  ow....        # 
-00008710: 4755 4920 5374 6174 6520 5472 6163 6b65  GUI State Tracke
-00008720: 720a 2020 2020 2020 2020 2320 2d20 5369  r.        # - Si
-00008730: 6e63 6520 7468 6973 2069 7320 6e6f 7420  nce this is not 
-00008740: 6120 6074 746b 2e57 6964 6765 7460 2c20  a `ttk.Widget`, 
-00008750: 7468 6973 206e 6565 6420 746f 2062 6520  this need to be 
-00008760: 656d 756c 6174 6564 0a20 2020 2020 2020  emulated.       
-00008770: 2073 656c 662e 5f5f 6773 7461 7465 3a20   self.__gstate: 
-00008780: 6d6f 6465 6c2e 4775 6953 7461 7465 203d  model.GuiState =
-00008790: 206d 6f64 656c 2e47 7569 5374 6174 6528   model.GuiState(
-000087a0: 656e 6162 6c65 643d 5472 7565 2c20 7265  enabled=True, re
-000087b0: 6164 6f6e 6c79 3d72 6561 646f 6e6c 7929  adonly=readonly)
-000087c0: 0a20 2020 2020 2020 2023 202d 2053 6574  .        # - Set
-000087d0: 2074 6865 2069 6e74 6572 6e61 6c20 7265   the internal re
-000087e0: 6164 6f6e 6c79 2073 7461 7465 206f 7574  adonly state out
-000087f0: 2d6f 662d 7468 652d 626f 780a 2020 2020  -of-the-box.    
-00008800: 2020 2020 7365 6c66 2e73 6574 5f67 7569      self.set_gui
-00008810: 5f73 7461 7465 2872 6561 646f 6e6c 793d  _state(readonly=
-00008820: 7265 6164 6f6e 6c79 2c20 5f69 6e74 6572  readonly, _inter
-00008830: 6e61 6c3d 5472 7565 290a 2020 2020 2020  nal=True).      
-00008840: 2020 6173 7365 7274 2073 656c 662e 7661    assert self.va
-00008850: 7269 6162 6c65 2069 7320 6e6f 7420 4e6f  riable is not No
-00008860: 6e65 2c20 6627 7b73 656c 6621 727d 3a20  ne, f'{self!r}: 
-00008870: 4d69 7373 696e 6720 7661 7269 6162 6c65  Missing variable
-00008880: 270a 2020 2020 2020 2020 7365 6c66 2e77  '.        self.w
-00008890: 7374 6174 6520 3d20 6765 7461 7474 7228  state = getattr(
-000088a0: 7365 6c66 2e76 6172 6961 626c 652c 2027  self.variable, '
-000088b0: 5f64 6566 6175 6c74 272c 2027 2729 2020  _default', '')  
-000088c0: 2320 5365 7420 7468 6520 6465 6661 756c  # Set the defaul
-000088d0: 7420 2862 6566 6f72 6520 7468 6520 7472  t (before the tr
-000088e0: 6163 6529 0a20 2020 2020 2020 2023 2053  ace).        # S
-000088f0: 7461 7465 2054 7261 636b 6572 0a20 2020  tate Tracker.   
-00008900: 2020 2020 2073 656c 662e 7472 6163 6528       self.trace(
-00008910: 7365 6c66 2e5f 7661 7243 6861 6e67 6564  self._varChanged
-00008920: 2c20 7472 6163 655f 6e61 6d65 3d66 275f  , trace_name=f'_
-00008930: 5f3a 7b5f 5f6e 616d 655f 5f7d 2729 0a0a  _:{__name__}')..
-00008940: 2020 2020 2020 2020 2320 4269 6e64 696e          # Bindin
-00008950: 6773 0a20 2020 2020 2020 2073 656c 662e  gs.        self.
-00008960: 5f62 696e 6469 6e67 735f 7461 6720 3d20  _bindings_tag = 
-00008970: 7b7d 0a20 2020 2020 2020 2023 2054 4f44  {}.        # TOD
-00008980: 4f3a 2049 6e76 6573 7469 6761 7465 2063  O: Investigate c
-00008990: 6861 6e67 696e 6720 7468 6520 6375 7273  hanging the curs
-000089a0: 6f72 206f 6e20 6d6f 7573 656f 7665 720a  or on mouseover.
-000089b0: 2020 2020 2020 2020 7365 6c66 2e62 696e          self.bin
-000089c0: 6469 6e67 5f74 6167 2827 6127 2c20 273c  ding_tag('a', '<
-000089d0: 4275 7474 6f6e 2d31 3e27 2c20 7365 6c66  Button-1>', self
-000089e0: 2e5f 6f6e 436c 6963 6b54 6167 290a 2020  ._onClickTag).  
-000089f0: 2020 2020 2020 6966 2072 6561 646f 6e6c        if readonl
-00008a00: 793a 0a20 2020 2020 2020 2020 2020 2023  y:.            #
-00008a10: 2044 6973 6162 6c65 2044 6f75 626c 652d   Disable Double-
-00008a20: 436c 6963 6b20 6576 656e 742c 2077 6865  Click event, whe
-00008a30: 6e20 7265 6164 6f6e 6c79 0a20 2020 2020  n readonly.     
-00008a40: 2020 2020 2020 2073 656c 662e 6269 6e64         self.bind
-00008a50: 696e 6728 273c 446f 7562 6c65 2d42 7574  ing('<Double-But
-00008a60: 746f 6e2d 313e 272c 2066 6e2e 6269 6e64  ton-1>', fn.bind
-00008a70: 696e 675f 6469 7361 626c 6529 0a0a 2020  ing_disable)..  
-00008a80: 2020 6465 6620 5f76 6172 4368 616e 6765    def _varChange
-00008a90: 6428 7365 6c66 2c20 7661 722c 2065 7479  d(self, var, ety
-00008aa0: 7065 293a 0a20 2020 2020 2020 2061 7373  pe):.        ass
-00008ab0: 6572 7420 6574 7970 6520 3d3d 2027 7772  ert etype == 'wr
-00008ac0: 6974 6527 0a20 2020 2020 2020 2023 2054  ite'.        # T
-00008ad0: 6869 7320 6675 6e63 7469 6f6e 2069 7320  his function is 
-00008ae0: 6361 6c6c 6564 2077 6865 6e20 7468 6520  called when the 
-00008af0: 7661 6c75 6520 6368 616e 6765 730a 2020  value changes.  
-00008b00: 2020 2020 2020 2320 4974 2773 2074 6865        # It's the
-00008b10: 2069 6d70 6c65 6d65 6e74 6174 696f 6e20   implementation 
-00008b20: 7468 6174 2062 696e 6473 2074 6865 2076  that binds the v
-00008b30: 6172 6961 626c 6520 616e 6420 7468 6520  ariable and the 
-00008b40: 7769 6467 6574 2c0a 2020 2020 2020 2020  widget,.        
-00008b50: 2320 2073 6f20 7468 6973 2073 686f 756c  #  so this shoul
-00008b60: 6420 6265 2069 6465 6d70 6f74 656e 740a  d be idempotent.
-00008b70: 2020 2020 2020 2020 7673 203d 2076 6172          vs = var
-00008b80: 2e67 6574 2829 0a20 2020 2020 2020 2077  .get().        w
-00008b90: 6974 6820 7365 6c66 2e61 735f 6564 6974  ith self.as_edit
-00008ba0: 6162 6c65 2829 3a0a 2020 2020 2020 2020  able():.        
-00008bb0: 2020 2020 2320 4465 6c65 7465 2074 6865      # Delete the
-00008bc0: 2065 6e74 6972 6520 7374 6174 650a 2020   entire state.  
-00008bd0: 2020 2020 2020 2020 2020 2320 4672 6f6d            # From
-00008be0: 3a20 4669 7273 7420 6c69 6e65 2c20 6669  : First line, fi
-00008bf0: 7273 7420 6368 6172 6163 7465 720a 2020  rst character.  
-00008c00: 2020 2020 2020 2020 2020 2320 2020 546f            #   To
-00008c10: 3a20 456e 640a 2020 2020 2020 2020 2020  : End.          
-00008c20: 2020 7365 6c66 2e64 656c 6574 6528 2731    self.delete('1
-00008c30: 2e30 272c 2027 656e 6427 290a 2020 2020  .0', 'end').    
-00008c40: 2020 2020 2020 2020 2320 5265 7365 7420          # Reset 
-00008c50: 7374 796c 6573 0a20 2020 2020 2020 2020  styles.         
-00008c60: 2020 2073 656c 662e 7374 796c 655f 7265     self.style_re
-00008c70: 7365 7428 290a 2020 2020 2020 2020 2020  set().          
-00008c80: 2020 2320 4164 6420 7468 6520 6375 7272    # Add the curr
-00008c90: 656e 7420 7374 6174 650a 2020 2020 2020  ent state.      
-00008ca0: 2020 2020 2020 2320 544f 444f 3a20 5361        # TODO: Sa
-00008cb0: 7665 2074 6865 2070 6172 7365 6420 4c54  ve the parsed LT
-00008cc0: 4d4c 2073 7461 7465 2073 6f6d 6577 6865  ML state somewhe
-00008cd0: 7265 2069 6e20 7468 6973 206f 626a 6563  re in this objec
-00008ce0: 742c 2077 6974 6820 6064 6174 6160 3f0a  t, with `data`?.
-00008cf0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00008d00: 7465 2069 6e20 7061 7273 6572 2e70 6172  te in parser.par
-00008d10: 7365 5f4c 544d 4c28 7673 293a 0a20 2020  se_LTML(vs):.   
-00008d20: 2020 2020 2020 2020 2020 2020 2061 7373               ass
-00008d30: 6572 7420 6973 696e 7374 616e 6365 2874  ert isinstance(t
-00008d40: 652c 206d 6f64 656c 2e54 6578 7445 6c65  e, model.TextEle
-00008d50: 6d65 6e74 290a 2020 2020 2020 2020 2020  ment).          
-00008d60: 2020 2020 2020 7365 6c66 2e69 6e73 6572        self.inser
-00008d70: 7428 746b 2e45 4e44 2c20 7465 2e74 6578  t(tk.END, te.tex
-00008d80: 742c 2074 652e 6174 6167 7329 0a0a 2020  t, te.atags)..  
-00008d90: 2020 6465 6620 6765 745f 6775 695f 7374    def get_gui_st
-00008da0: 6174 6528 7365 6c66 2920 2d3e 206d 6f64  ate(self) -> mod
-00008db0: 656c 2e47 7569 5374 6174 653a 0a20 2020  el.GuiState:.   
-00008dc0: 2020 2020 2027 2727 2727 2720 2023 2044       ''''''  # D
-00008dd0: 6f20 6e6f 7420 646f 6375 6d65 6e74 0a20  o not document. 
-00008de0: 2020 2020 2020 2069 6620 5f5f 6465 6275         if __debu
-00008df0: 675f 5f3a 0a20 2020 2020 2020 2020 2020  g__:.           
-00008e00: 206c 6f67 6765 722e 6465 6275 6728 2753   logger.debug('S
-00008e10: 7461 7465 203e 2025 7227 2c20 7365 6c66  tate > %r', self
-00008e20: 2e5f 5f67 7374 6174 6529 0a20 2020 2020  .__gstate).     
-00008e30: 2020 2023 2072 6574 7572 6e20 6120 636f     # return a co
-00008e40: 7079 206f 6620 7468 6520 6f62 6a65 6374  py of the object
-00008e50: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00008e60: 6d6f 6465 6c2e 4775 6953 7461 7465 282a  model.GuiState(*
-00008e70: 2a64 6963 7428 7365 6c66 2e5f 5f67 7374  *dict(self.__gst
-00008e80: 6174 652e 6974 656d 7328 2929 290a 0a20  ate.items())).. 
-00008e90: 2020 2064 6566 2073 6574 5f67 7569 5f73     def set_gui_s
-00008ea0: 7461 7465 2873 656c 662c 2073 7461 7465  tate(self, state
-00008eb0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00008ec0: 6c5b 6d6f 6465 6c2e 4775 6953 7461 7465  l[model.GuiState
-00008ed0: 5d20 3d20 4e6f 6e65 2c20 2a2c 205f 696e  ] = None, *, _in
-00008ee0: 7465 726e 616c 3a20 626f 6f6c 203d 2046  ternal: bool = F
-00008ef0: 616c 7365 2c20 2a2a 6b77 6172 6773 2920  alse, **kwargs) 
-00008f00: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00008f10: 2027 2727 2727 2720 2023 2044 6f20 6e6f   ''''''  # Do no
-00008f20: 7420 646f 6375 6d65 6e74 0a20 2020 2020  t document.     
-00008f30: 2020 2069 6620 7374 6174 6520 6973 204e     if state is N
-00008f40: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00008f50: 2073 7461 7465 203d 206d 6f64 656c 2e47   state = model.G
-00008f60: 7569 5374 6174 6528 2a2a 6b77 6172 6773  uiState(**kwargs
-00008f70: 290a 2020 2020 2020 2020 6966 205f 5f64  ).        if __d
-00008f80: 6562 7567 5f5f 3a0a 2020 2020 2020 2020  ebug__:.        
-00008f90: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-00008fa0: 2827 5374 6174 6520 3c20 2572 272c 2073  ('State < %r', s
-00008fb0: 7461 7465 290a 2020 2020 2020 2020 2320  tate).        # 
-00008fc0: 4164 6a75 7374 2063 7572 7265 6e74 2073  Adjust current s
-00008fd0: 7461 7465 0a20 2020 2020 2020 2066 6f72  tate.        for
-00008fe0: 2073 6e61 6d65 2c20 7376 616c 7565 2069   sname, svalue i
-00008ff0: 6e20 7374 6174 652e 6974 656d 7328 293a  n state.items():
-00009000: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-00009010: 6572 7420 736e 616d 6520 213d 2027 5f69  ert sname != '_i
-00009020: 6e74 6572 6e61 6c27 2020 2320 5368 6f75  nternal'  # Shou
-00009030: 6c64 2062 6520 696d 706f 7373 6962 6c65  ld be impossible
-00009040: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
-00009050: 6966 2073 7661 6c75 6520 6973 206e 6f74  if svalue is not
-00009060: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00009070: 2020 2020 2020 2069 6620 736e 616d 6520         if sname 
-00009080: 3d3d 2027 7265 6164 6f6e 6c79 2720 616e  == 'readonly' an
-00009090: 6420 5f69 6e74 6572 6e61 6c20 6973 2046  d _internal is F
-000090a0: 616c 7365 3a0a 2020 2020 2020 2020 2020  alse:.          
-000090b0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000090c0: 5661 6c75 6545 7272 6f72 2866 277b 7365  ValueError(f'{se
-000090d0: 6c66 7d3a 204e 6f20 7375 7070 6f72 7420  lf}: No support 
-000090e0: 666f 7220 6578 7465 726e 616c 2072 6561  for external rea
-000090f0: 646f 6e6c 7920 7374 6174 6520 6d61 6e69  donly state mani
-00009100: 7075 6c61 7469 6f6e 2729 0a20 2020 2020  pulation').     
-00009110: 2020 2020 2020 2020 2020 2073 6574 6174             setat
-00009120: 7472 2873 656c 662e 5f5f 6773 7461 7465  tr(self.__gstate
-00009130: 2c20 736e 616d 652c 2073 7661 6c75 6529  , sname, svalue)
-00009140: 0a20 2020 2020 2020 2023 2041 646a 7573  .        # Adjus
-00009150: 7420 7769 6467 6574 2073 7461 7465 0a20  t widget state. 
-00009160: 2020 2020 2020 2063 6667 203d 207b 7d0a         cfg = {}.
-00009170: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00009180: 5f5f 6773 7461 7465 2e65 6e61 626c 6564  __gstate.enabled
-00009190: 2069 7320 5472 7565 3a0a 2020 2020 2020   is True:.      
-000091a0: 2020 2020 2020 6966 2073 656c 662e 5f5f        if self.__
-000091b0: 6773 7461 7465 2e72 6561 646f 6e6c 7920  gstate.readonly 
-000091c0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000091d0: 2020 2020 2020 2020 2020 2020 2063 6667               cfg
-000091e0: 5b27 7374 6174 6527 5d20 3d20 746b 2e4e  ['state'] = tk.N
-000091f0: 4f52 4d41 4c20 6966 206e 6f74 2073 656c  ORMAL if not sel
-00009200: 662e 5f5f 6773 7461 7465 2e72 6561 646f  f.__gstate.reado
-00009210: 6e6c 7920 656c 7365 2074 6b2e 4449 5341  nly else tk.DISA
-00009220: 424c 4544 0a20 2020 2020 2020 2020 2020  BLED.           
-00009230: 2063 6667 5b27 6261 636b 6772 6f75 6e64   cfg['background
-00009240: 275d 203d 2073 656c 662e 7773 7479 6c65  '] = self.wstyle
-00009250: 2e63 6f6c 6f75 725f 6267 5f6f 6e0a 2020  .colour_bg_on.  
-00009260: 2020 2020 2020 656c 6966 2073 656c 662e        elif self.
-00009270: 5f5f 6773 7461 7465 2e65 6e61 626c 6564  __gstate.enabled
-00009280: 2069 7320 4661 6c73 653a 0a20 2020 2020   is False:.     
-00009290: 2020 2020 2020 2063 6667 5b27 7374 6174         cfg['stat
-000092a0: 6527 5d20 3d20 746b 2e44 4953 4142 4c45  e'] = tk.DISABLE
-000092b0: 440a 2020 2020 2020 2020 2020 2020 6366  D.            cf
-000092c0: 675b 2762 6163 6b67 726f 756e 6427 5d20  g['background'] 
-000092d0: 3d20 7365 6c66 2e77 7374 796c 652e 636f  = self.wstyle.co
-000092e0: 6c6f 7572 5f62 675f 6f66 660a 2020 2020  lour_bg_off.    
-000092f0: 2020 2020 2020 2020 7365 6c66 2e73 7479          self.sty
-00009300: 6c65 5f72 6573 6574 2829 0a20 2020 2020  le_reset().     
-00009310: 2020 2023 2069 6620 5f5f 6465 6275 675f     # if __debug_
-00009320: 5f3a 0a20 2020 2020 2020 2023 2020 2020  _:.        #    
-00009330: 206c 6f67 6765 722e 6465 6275 6728 2743   logger.debug('C
-00009340: 2025 7327 2c20 7365 6c66 2e5f 5f67 7374   %s', self.__gst
-00009350: 6174 6529 0a20 2020 2020 2020 2023 2020  ate).        #  
-00009360: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-00009370: 277c 2025 7327 2c20 6366 6729 0a20 2020  '| %s', cfg).   
-00009380: 2020 2020 2073 656c 662e 636f 6e66 6967       self.config
-00009390: 7572 6528 2a2a 6366 6729 0a20 2020 2020  ure(**cfg).     
-000093a0: 2020 2023 2056 616c 6964 3a20 5442 440a     # Valid: TBD.
-000093b0: 0a20 2020 2040 636f 6e74 6578 746d 616e  .    @contextman
-000093c0: 6167 6572 0a20 2020 2064 6566 2061 735f  ager.    def as_
-000093d0: 6564 6974 6162 6c65 2873 656c 6629 3a0a  editable(self):.
-000093e0: 2020 2020 2020 2020 2727 2754 656d 706f          '''Tempo
-000093f0: 7261 7269 6c79 206d 6172 6b20 7468 6520  rarily mark the 
-00009400: 7769 6467 6574 2061 7320 6564 6974 6162  widget as editab
-00009410: 6c65 2e0a 0a20 2020 2020 2020 2041 2063  le...        A c
-00009420: 6f6e 7465 7874 206d 616e 6167 6572 2c20  ontext manager, 
-00009430: 7573 6564 2074 6f20 6368 616e 6765 2074  used to change t
-00009440: 6865 2063 6f6e 7465 6e74 7320 6f66 2074  he contents of t
-00009450: 6865 2077 6964 6765 7420 7768 696c 6520  he widget while 
-00009460: 6b65 6570 0a20 2020 2020 2020 2069 7420  keep.        it 
-00009470: 2272 6561 646f 6e6c 7922 2e0a 2020 2020  "readonly"..    
-00009480: 2020 2020 5465 6368 6e69 6361 6c6c 792c      Technically,
-00009490: 2074 6869 7320 7368 6f75 6c64 206f 6e6c   this should onl
-000094a0: 7920 6265 2075 7365 6420 696e 7465 726e  y be used intern
-000094b0: 616c 6c79 2c20 7573 696e 6720 7468 6520  ally, using the 
-000094c0: 7374 6174 650a 2020 2020 2020 2020 7472  state.        tr
-000094d0: 6163 6b65 7220 6675 6e63 7469 6f6e 732c  acker functions,
-000094e0: 2062 7574 2069 7420 6d69 6768 7420 6265   but it might be
-000094f0: 2075 7365 6675 6c20 6578 7465 726e 616c   useful external
-00009500: 6c79 2e0a 0a20 2020 2020 2020 2054 6869  ly...        Thi
-00009510: 7320 6973 2074 6f20 6265 2075 7365 6420  s is to be used 
-00009520: 6c69 6b65 2074 6869 733a 0a0a 2020 2020  like this:..    
-00009530: 2020 2020 2e2e 2063 6f64 653a 3a20 7079      .. code:: py
-00009540: 7468 6f6e 0a0a 2020 2020 2020 2020 2020  thon..          
-00009550: 2020 2320 6077 6964 6765 7460 2069 7320    # `widget` is 
-00009560: 7265 6164 6f6e 6c79 0a20 2020 2020 2020  readonly.       
-00009570: 2020 2020 2077 6974 6820 7769 6467 6574       with widget
-00009580: 2e61 735f 6564 6974 6162 6c65 2829 3a0a  .as_editable():.
-00009590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095a0: 7061 7373 2020 2320 6077 6964 6765 7460  pass  # `widget`
-000095b0: 2069 7320 6564 6974 6162 6c65 0a20 2020   is editable.   
-000095c0: 2020 2020 2020 2020 2023 2060 7769 6467           # `widg
-000095d0: 6574 6020 6973 2072 6561 646f 6e6c 790a  et` is readonly.
-000095e0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-000095f0: 2020 2020 6173 7365 7274 2073 656c 662e      assert self.
-00009600: 5f5f 6773 7461 7465 2e72 6561 646f 6e6c  __gstate.readonl
-00009610: 7920 6973 2054 7275 650a 2020 2020 2020  y is True.      
-00009620: 2020 7365 6c66 2e73 6574 5f67 7569 5f73    self.set_gui_s
-00009630: 7461 7465 2872 6561 646f 6e6c 793d 4661  tate(readonly=Fa
-00009640: 6c73 652c 205f 696e 7465 726e 616c 3d54  lse, _internal=T
-00009650: 7275 6529 0a20 2020 2020 2020 2074 7279  rue).        try
-00009660: 3a0a 2020 2020 2020 2020 2020 2020 7969  :.            yi
-00009670: 656c 640a 2020 2020 2020 2020 6669 6e61  eld.        fina
-00009680: 6c6c 793a 0a20 2020 2020 2020 2020 2020  lly:.           
-00009690: 2073 656c 662e 7365 745f 6775 695f 7374   self.set_gui_st
-000096a0: 6174 6528 7265 6164 6f6e 6c79 3d54 7275  ate(readonly=Tru
-000096b0: 652c 205f 696e 7465 726e 616c 3d54 7275  e, _internal=Tru
-000096c0: 6529 0a0a 2020 2020 6465 6620 6269 6e64  e)..    def bind
-000096d0: 696e 675f 7461 6728 7365 6c66 2c20 7461  ing_tag(self, ta
-000096e0: 673a 2073 7472 2c20 7365 7175 656e 6365  g: str, sequence
-000096f0: 3a20 7374 722c 202a 6172 6773 2c20 6b65  : str, *args, ke
-00009700: 793a 2073 7472 203d 204e 6f6e 652c 2069  y: str = None, i
-00009710: 6d6d 6564 6961 7465 3a20 626f 6f6c 203d  mmediate: bool =
-00009720: 2054 7275 652c 202a 2a6b 7761 7267 7329   True, **kwargs)
-00009730: 202d 3e20 6d6f 6465 6c2e 4269 6e64 696e   -> model.Bindin
-00009740: 6754 6167 3a0a 2020 2020 2020 2020 2727  gTag:.        ''
-00009750: 2742 696e 6473 2061 2073 6571 7565 6e63  'Binds a sequenc
-00009760: 6520 746f 2061 2074 6167 2e0a 0a20 2020  e to a tag...   
-00009770: 2020 2020 2053 746f 7265 7320 616c 6c20       Stores all 
-00009780: 7769 6467 6574 2074 6167 2062 696e 6469  widget tag bindi
-00009790: 6e67 7320 6f6e 2061 2070 6572 2d69 6e73  ngs on a per-ins
-000097a0: 7461 6e63 6520 6469 6374 696f 6e61 7279  tance dictionary
-000097b0: 2c20 666f 7220 6c61 7465 720a 2020 2020  , for later.    
-000097c0: 2020 2020 7573 6167 652e 204e 6f74 6520      usage. Note 
-000097d0: 7468 6174 2061 6c6c 2064 6963 7469 6f6e  that all diction
-000097e0: 6172 7920 6b65 7973 206d 7573 7420 6265  ary keys must be
-000097f0: 2064 6966 6665 7265 6e74 2e20 466f 7220   different. For 
-00009800: 7468 6520 7361 6d65 0a20 2020 2020 2020  the same.       
-00009810: 2062 696e 6469 6e67 7320 6f6e 2061 2073   bindings on a s
-00009820: 696e 676c 6520 7769 6467 6574 2074 6167  ingle widget tag
-00009830: 2c20 7468 6973 2072 6571 7569 7265 7320  , this requires 
-00009840: 7061 7373 696e 6720 7468 6520 6060 6b65  passing the ``ke
-00009850: 7960 600a 2020 2020 2020 2020 6172 6775  y``.        argu
-00009860: 6d65 6e74 2e0a 0a20 2020 2020 2020 2053  ment...        S
-00009870: 6565 2074 6865 2060 6054 6b60 6020 6074  ee the ``Tk`` `t
-00009880: 6167 2062 696e 6420 3c68 7474 7073 3a2f  ag bind <https:/
-00009890: 2f77 7777 2e74 636c 2e74 6b2f 6d61 6e2f  /www.tcl.tk/man/
-000098a0: 7463 6c2f 546b 436d 642f 7465 7874 2e68  tcl/TkCmd/text.h
-000098b0: 746d 6c23 4d31 3636 3e60 5f20 646f 6375  tml#M166>`_ docu
-000098c0: 6d65 6e74 6174 696f 6e2e 0a0a 2020 2020  mentation...    
-000098d0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-000098e0: 2020 2020 2020 6b65 793a 204f 7074 696f        key: Optio
-000098f0: 6e61 6c2e 2044 6566 6175 6c74 7320 746f  nal. Defaults to
-00009900: 2074 6865 2060 6073 6571 7565 6e63 6560   the ``sequence`
-00009910: 6020 6974 7365 6c66 2e20 5573 6566 756c  ` itself. Useful
-00009920: 2074 6f0a 2020 2020 2020 2020 2020 2020   to.            
-00009930: 2020 2020 7375 7070 6f72 7420 6d75 6c74      support mult
-00009940: 6970 6c65 2062 696e 6469 6e67 7320 6f6e  iple bindings on
-00009950: 2074 6865 2073 616d 6520 7365 7175 656e   the same sequen
-00009960: 6365 2c20 666f 7220 7468 6520 7361 6d65  ce, for the same
-00009970: 2074 6167 2e0a 0a20 2020 2020 2020 2041   tag...        A
-00009980: 6c6c 206f 7468 6572 2061 7267 756d 656e  ll other argumen
-00009990: 7473 2061 7265 2070 6173 7365 6420 746f  ts are passed to
-000099a0: 2060 6d6f 6465 6c2e 4269 6e64 696e 6754   `model.BindingT
-000099b0: 6167 6020 6f62 6a65 6374 2e0a 2020 2020  ag` object..    
-000099c0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-000099d0: 6e61 6d65 203d 2028 7461 672c 206b 6579  name = (tag, key
-000099e0: 206f 7220 7365 7175 656e 6365 290a 2020   or sequence).  
-000099f0: 2020 2020 2020 6966 206e 616d 6520 696e        if name in
-00009a00: 2073 656c 662e 5f62 696e 6469 6e67 735f   self._bindings_
-00009a10: 7461 673a 0a20 2020 2020 2020 2020 2020  tag:.           
-00009a20: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00009a30: 7228 6627 5265 7065 6174 6564 2062 696e  r(f'Repeated bin
-00009a40: 6469 6e67 2066 6f72 2022 7b73 6571 7565  ding for "{seque
-00009a50: 6e63 657d 2220 696e 207b 7365 6c66 2172  nce}" in {self!r
-00009a60: 7d28 7461 6720 227b 7461 677d 2229 2e20  }(tag "{tag}"). 
-00009a70: 4368 616e 6765 2074 6865 2022 6b65 7922  Change the "key"
-00009a80: 2070 6172 616d 6574 6572 2e27 290a 2020   parameter.').  
-00009a90: 2020 2020 2020 6966 205f 5f64 6562 7567        if __debug
-00009aa0: 5f5f 3a0a 2020 2020 2020 2020 2020 2020  __:.            
-00009ab0: 6966 206c 656e 2874 6167 2920 3d3d 2030  if len(tag) == 0
-00009ac0: 206f 7220 7461 675b 305d 203d 3d20 273c   or tag[0] == '<
-00009ad0: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
-00009ae0: 2020 2077 6172 6e69 6e67 732e 7761 726e     warnings.warn
-00009af0: 2866 277b 7365 6c66 7d3a 2062 696e 6469  (f'{self}: bindi
-00009b00: 6e67 5f74 6167 2072 6571 7569 7265 7320  ng_tag requires 
-00009b10: 7461 675b 7b74 6167 7d5d 2061 6e64 2073  tag[{tag}] and s
-00009b20: 6571 7565 6e63 655b 7b73 6571 7565 6e63  equence[{sequenc
-00009b30: 657d 5d2c 2062 7920 7468 6973 206f 7264  e}], by this ord
-00009b40: 6572 272c 2073 7461 636b 6c65 7665 6c3d  er', stacklevel=
-00009b50: 3229 0a20 2020 2020 2020 2073 656c 662e  2).        self.
-00009b60: 5f62 696e 6469 6e67 735f 7461 675b 6e61  _bindings_tag[na
-00009b70: 6d65 5d20 3d20 6d6f 6465 6c2e 4269 6e64  me] = model.Bind
-00009b80: 696e 6754 6167 2873 656c 662c 2074 6167  ingTag(self, tag
-00009b90: 2c20 7365 7175 656e 6365 2c20 2a61 7267  , sequence, *arg
-00009ba0: 732c 2069 6d6d 6564 6961 7465 3d69 6d6d  s, immediate=imm
-00009bb0: 6564 6961 7465 2c20 2a2a 6b77 6172 6773  ediate, **kwargs
-00009bc0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00009bd0: 2073 656c 662e 5f62 696e 6469 6e67 735f   self._bindings_
-00009be0: 7461 675b 6e61 6d65 5d0a 0a20 2020 2023  tag[name]..    #
-00009bf0: 2054 4f44 4f3a 2075 7365 2061 6e20 606c   TODO: use an `l
-00009c00: 7275 5f63 6163 6865 603f 0a20 2020 2064  ru_cache`?.    d
-00009c10: 6566 205f 666f 6e74 2873 656c 662c 2066  ef _font(self, f
-00009c20: 6f6e 7462 6173 653a 2074 7970 696e 672e  ontbase: typing.
-00009c30: 4f70 7469 6f6e 616c 5b74 6b2e 666f 6e74  Optional[tk.font
-00009c40: 2e46 6f6e 745d 203d 204e 6f6e 652c 0a20  .Font] = None,. 
-00009c50: 2020 2020 2020 2020 2020 2020 202a 2c0a               *,.
-00009c60: 2020 2020 2020 2020 2020 2020 2020 7369                si
-00009c70: 7a65 3a20 7479 7069 6e67 2e4f 7074 696f  ze: typing.Optio
-00009c80: 6e61 6c5b 696e 745d 203d 204e 6f6e 652c  nal[int] = None,
-00009c90: 0a20 2020 2020 2020 2020 2020 2020 2062  .              b
-00009ca0: 6f6c 643a 2074 7970 696e 672e 4f70 7469  old: typing.Opti
-00009cb0: 6f6e 616c 5b62 6f6f 6c5d 203d 204e 6f6e  onal[bool] = Non
-00009cc0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00009cd0: 2069 7461 6c69 633a 2074 7970 696e 672e   italic: typing.
-00009ce0: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
-00009cf0: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-00009d00: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
-00009d10: 666f 6e74 6261 7365 203d 2066 6f6e 7462  fontbase = fontb
-00009d20: 6173 6520 6f72 2074 6b2e 666f 6e74 2e6e  ase or tk.font.n
-00009d30: 616d 6574 6f66 6f6e 7428 7365 6c66 2e77  ametofont(self.w
-00009d40: 7374 796c 652e 666f 6e74 5f62 6173 6529  style.font_base)
-00009d50: 0a20 2020 2020 2020 2023 2053 7461 7274  .        # Start
-00009d60: 2066 726f 6d20 7468 6520 6261 7365 2066   from the base f
-00009d70: 6f6e 7420 6f70 7469 6f6e 730a 2020 2020  ont options.    
-00009d80: 2020 2020 6f70 7469 6f6e 7320 3d20 666f      options = fo
-00009d90: 6e74 6261 7365 2e61 6374 7561 6c28 290a  ntbase.actual().
-00009da0: 2020 2020 2020 2020 6966 2073 697a 653a          if size:
-00009db0: 0a20 2020 2020 2020 2020 2020 206f 7074  .            opt
-00009dc0: 696f 6e73 5b27 7369 7a65 275d 203d 2073  ions['size'] = s
-00009dd0: 697a 650a 2020 2020 2020 2020 6966 2062  ize.        if b
-00009de0: 6f6c 6420 6973 2054 7275 653a 0a20 2020  old is True:.   
-00009df0: 2020 2020 2020 2020 206f 7074 696f 6e73           options
-00009e00: 5b27 7765 6967 6874 275d 203d 2074 6b2e  ['weight'] = tk.
-00009e10: 666f 6e74 2e42 4f4c 440a 2020 2020 2020  font.BOLD.      
-00009e20: 2020 6966 2069 7461 6c69 6320 6973 2054    if italic is T
-00009e30: 7275 653a 0a20 2020 2020 2020 2020 2020  rue:.           
-00009e40: 206f 7074 696f 6e73 5b27 736c 616e 7427   options['slant'
-00009e50: 5d20 3d20 746b 2e66 6f6e 742e 4954 414c  ] = tk.font.ITAL
-00009e60: 4943 0a20 2020 2020 2020 2072 6574 7572  IC.        retur
-00009e70: 6e20 746b 2e66 6f6e 742e 466f 6e74 282a  n tk.font.Font(*
-00009e80: 2a6f 7074 696f 6e73 290a 0a20 2020 2064  *options)..    d
-00009e90: 6566 205f 7374 796c 655f 6128 7365 6c66  ef _style_a(self
-00009ea0: 2c20 7461 673a 2073 7472 203d 2027 6127  , tag: str = 'a'
-00009eb0: 2c20 2a2c 2076 6973 6974 6564 3a20 626f  , *, visited: bo
-00009ec0: 6f6c 2920 2d3e 204e 6f6e 653a 0a20 2020  ol) -> None:.   
-00009ed0: 2020 2020 2066 6720 3d20 7365 6c66 2e77       fg = self.w
-00009ee0: 7374 796c 652e 636f 6c6f 7572 5f6c 696e  style.colour_lin
-00009ef0: 6b5f 7669 7369 7465 6420 6966 2076 6973  k_visited if vis
-00009f00: 6974 6564 2065 6c73 6520 7365 6c66 2e77  ited else self.w
-00009f10: 7374 796c 652e 636f 6c6f 7572 5f6c 696e  style.colour_lin
-00009f20: 6b5f 6e6f 726d 616c 0a20 2020 2020 2020  k_normal.       
-00009f30: 2073 656c 662e 7461 675f 636f 6e66 6967   self.tag_config
-00009f40: 7572 6528 7461 672c 2066 6f72 6567 726f  ure(tag, foregro
-00009f50: 756e 643d 6667 2c20 756e 6465 726c 696e  und=fg, underlin
-00009f60: 653d 5472 7565 290a 0a20 2020 2064 6566  e=True)..    def
-00009f70: 2073 7479 6c65 5f72 6573 6574 2873 656c   style_reset(sel
-00009f80: 662c 2065 7665 6e74 3d4e 6f6e 652c 202a  f, event=None, *
-00009f90: 2c20 613a 2062 6f6f 6c20 3d20 5472 7565  , a: bool = True
-00009fa0: 2c20 623a 2062 6f6f 6c20 3d20 5472 7565  , b: bool = True
-00009fb0: 2c20 693a 2062 6f6f 6c20 3d20 5472 7565  , i: bool = True
-00009fc0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00009fd0: 2020 2027 2727 5265 7365 7420 7468 6520     '''Reset the 
-00009fe0: 7374 796c 6520 746f 2074 6865 206f 7269  style to the ori
-00009ff0: 6769 6e61 6c2e 0a0a 2020 2020 2020 2020  ginal...        
-0000a000: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-0000a010: 2020 613a 2052 6573 6574 2060 6061 6060    a: Reset ``a``
-0000a020: 2061 6e63 686f 7273 2e0a 2020 2020 2020   anchors..      
-0000a030: 2020 2020 2020 623a 2052 6573 6574 2060        b: Reset `
-0000a040: 6062 6060 2062 6f6c 6420 696e 6c69 6e65  `b`` bold inline
-0000a050: 2073 7061 6e73 2e0a 2020 2020 2020 2020   spans..        
-0000a060: 2020 2020 693a 2052 6573 6574 2060 6069      i: Reset ``i
-0000a070: 6060 2069 7461 6c69 6320 696e 6c69 6e65  `` italic inline
-0000a080: 2073 7061 6e73 2e0a 0a20 2020 2020 2020   spans...       
-0000a090: 2020 2020 2065 7665 6e74 3a20 4f70 7469       event: Opti
-0000a0a0: 6f6e 616c 2c20 756e 7573 6564 2e20 5468  onal, unused. Th
-0000a0b0: 6973 2065 7869 7374 7320 666f 7220 4150  is exists for AP
-0000a0c0: 4920 636f 6d70 6174 6962 696c 6974 7920  I compatibility 
-0000a0d0: 7769 7468 2074 6865 0a20 2020 2020 2020  with the.       
-0000a0e0: 2020 2020 2020 2020 2060 606f 6e43 6c69           ``onCli
-0000a0f0: 636b 6060 2066 756e 6374 696f 6e73 2e0a  ck`` functions..
-0000a100: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-0000a110: 2020 2020 2320 544f 444f 3a20 5768 7920      # TODO: Why 
-0000a120: 6e6f 7420 7265 7365 7420 6576 6572 7974  not reset everyt
-0000a130: 6869 6e67 2061 6c77 6179 733f 2059 4147  hing always? YAG
-0000a140: 4e49 2e0a 2020 2020 2020 2020 6966 2062  NI..        if b
-0000a150: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000a160: 6c66 2e74 6167 5f63 6f6e 6669 6775 7265  lf.tag_configure
-0000a170: 2827 6227 2c20 666f 6e74 3d73 656c 662e  ('b', font=self.
-0000a180: 5f66 6f6e 7428 626f 6c64 3d54 7275 6529  _font(bold=True)
-0000a190: 290a 2020 2020 2020 2020 6966 2069 3a0a  ).        if i:.
-0000a1a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000a1b0: 2e74 6167 5f63 6f6e 6669 6775 7265 2827  .tag_configure('
-0000a1c0: 6927 2c20 666f 6e74 3d73 656c 662e 5f66  i', font=self._f
-0000a1d0: 6f6e 7428 6974 616c 6963 3d54 7275 6529  ont(italic=True)
-0000a1e0: 290a 2020 2020 2020 2020 666f 7220 7461  ).        for ta
-0000a1f0: 6720 696e 2073 656c 662e 7461 675f 6e61  g in self.tag_na
-0000a200: 6d65 7328 293a 0a20 2020 2020 2020 2020  mes():.         
-0000a210: 2020 2023 2061 0a20 2020 2020 2020 2020     # a.         
-0000a220: 2020 2069 6620 6120 616e 6420 7461 6720     if a and tag 
-0000a230: 3d3d 2027 6127 206f 7220 7461 672e 7374  == 'a' or tag.st
-0000a240: 6172 7473 7769 7468 2827 613a 3a27 293a  artswith('a::'):
-0000a250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a260: 2073 656c 662e 5f73 7479 6c65 5f61 2874   self._style_a(t
-0000a270: 6167 3d74 6167 2c20 7669 7369 7465 643d  ag=tag, visited=
-0000a280: 4661 6c73 6529 0a0a 2020 2020 6465 6620  False)..    def 
-0000a290: 5f6f 6e43 6c69 636b 5461 6728 7365 6c66  _onClickTag(self
-0000a2a0: 2c20 6576 656e 742c 202a 2c20 7461 675f  , event, *, tag_
-0000a2b0: 6e61 6d65 3a20 7374 7220 3d20 2761 2729  name: str = 'a')
-0000a2c0: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
-0000a2d0: 2073 656c 662e 5f5f 6773 7461 7465 2e65   self.__gstate.e
-0000a2e0: 6e61 626c 6564 3a0a 2020 2020 2020 2020  nabled:.        
-0000a2f0: 2020 2020 7265 7475 726e 2020 2320 446f      return  # Do
-0000a300: 206e 6f74 6869 6e67 2077 6865 6e20 6469   nothing when di
-0000a310: 7361 626c 6564 0a20 2020 2020 2020 2064  sabled.        d
-0000a320: 6f62 6a20 3d20 7365 6c66 2e64 756d 7028  obj = self.dump(
-0000a330: 6627 407b 6576 656e 742e 787d 2c7b 6576  f'@{event.x},{ev
-0000a340: 656e 742e 797d 272c 2074 6578 743d 5472  ent.y}', text=Tr
-0000a350: 7565 2c20 7461 673d 5472 7565 290a 2020  ue, tag=True).  
-0000a360: 2020 2020 2020 6966 205f 5f64 6562 7567        if __debug
-0000a370: 5f5f 3a0a 2020 2020 2020 2020 2020 2020  __:.            
-0000a380: 6c6f 6767 6572 2e64 6562 7567 2827 443a  logger.debug('D:
-0000a390: 2025 7227 2c20 646f 626a 290a 2020 2020   %r', dobj).    
-0000a3a0: 2020 2020 6477 6861 7420 3d20 5b64 696e      dwhat = [din
-0000a3b0: 6e65 725b 305d 2066 6f72 2064 696e 6e65  ner[0] for dinne
-0000a3c0: 7220 696e 2064 6f62 6a5d 0a20 2020 2020  r in dobj].     
-0000a3d0: 2020 2074 6167 735f 636c 203d 205b 5d20     tags_cl = [] 
-0000a3e0: 2023 2049 676e 6f72 6520 7468 6520 2273   # Ignore the "s
-0000a3f0: 656c 2220 7461 670a 2020 2020 2020 2020  el" tag.        
-0000a400: 6966 2027 7461 676f 6e27 2069 6e20 6477  if 'tagon' in dw
-0000a410: 6861 743a 0a20 2020 2020 2020 2020 2020  hat:.           
-0000a420: 2023 2043 6c69 636b 2069 6e20 7468 6520   # Click in the 
-0000a430: 7374 6172 7420 6f66 2074 6865 2074 6167  start of the tag
-0000a440: 0a20 2020 2020 2020 2020 2020 2074 6167  .            tag
-0000a450: 735f 636c 203d 205b 6c73 745b 315d 2066  s_cl = [lst[1] f
-0000a460: 6f72 206c 7374 2069 6e20 646f 626a 2069  or lst in dobj i
-0000a470: 6620 6c73 745b 305d 203d 3d20 2774 6167  f lst[0] == 'tag
-0000a480: 6f6e 2720 616e 6420 6c73 745b 315d 2021  on' and lst[1] !
-0000a490: 3d20 746b 2e53 454c 5d0a 2020 2020 2020  = tk.SEL].      
-0000a4a0: 2020 2020 2020 2320 466f 7220 6e65 7374        # For nest
-0000a4b0: 6564 2074 6167 732c 2074 6869 7320 6d69  ed tags, this mi
-0000a4c0: 6768 7420 6e6f 7420 6265 2074 6865 2073  ght not be the s
-0000a4d0: 616d 6520 6173 2074 6865 2074 6578 7420  ame as the text 
-0000a4e0: 6d65 7468 6f64 0a20 2020 2020 2020 2069  method.        i
-0000a4f0: 6620 6c65 6e28 7461 6773 5f63 6c29 203d  f len(tags_cl) =
-0000a500: 3d20 3020 616e 6420 2774 6578 7427 2069  = 0 and 'text' i
-0000a510: 6e20 6477 6861 743a 0a20 2020 2020 2020  n dwhat:.       
-0000a520: 2020 2020 2023 2043 6c69 636b 2069 6e20       # Click in 
-0000a530: 7468 6520 6d69 6464 6c65 206f 6620 7468  the middle of th
-0000a540: 6520 7461 670a 2020 2020 2020 2020 2020  e tag.          
-0000a550: 2020 636c 6963 6b5f 6c6f 6361 7469 6f6e    click_location
-0000a560: 203d 205b 6c73 745b 325d 2066 6f72 206c   = [lst[2] for l
-0000a570: 7374 2069 6e20 646f 626a 2069 6620 6c73  st in dobj if ls
-0000a580: 745b 305d 203d 3d20 2774 6578 7427 5d5b  t[0] == 'text'][
-0000a590: 305d 0a20 2020 2020 2020 2020 2020 2074  0].            t
-0000a5a0: 7020 3d20 7365 6c66 2e74 6167 5f70 7265  p = self.tag_pre
-0000a5b0: 7672 616e 6765 2874 6167 5f6e 616d 652c  vrange(tag_name,
-0000a5c0: 2063 6c69 636b 5f6c 6f63 6174 696f 6e29   click_location)
-0000a5d0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000a5e0: 5f5f 6465 6275 675f 5f3a 0a20 2020 2020  __debug__:.     
-0000a5f0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-0000a600: 722e 6465 6275 6728 2720 7c20 5465 7874  r.debug(' | Text
-0000a610: 2040 203c 2573 272c 2074 7029 0a20 2020   @ <%s', tp).   
-0000a620: 2020 2020 2020 2020 2074 6167 735f 636c           tags_cl
-0000a630: 203d 205b 6c73 745b 315d 2066 6f72 206c   = [lst[1] for l
-0000a640: 7374 2069 6e20 7365 6c66 2e64 756d 7028  st in self.dump(
-0000a650: 2a74 702c 2074 6167 3d54 7275 6529 2069  *tp, tag=True) i
-0000a660: 6620 6c73 745b 315d 2021 3d20 746b 2e53  f lst[1] != tk.S
-0000a670: 454c 5d0a 2020 2020 2020 2020 6966 206c  EL].        if l
-0000a680: 656e 2874 6167 735f 636c 2920 3d3d 2030  en(tags_cl) == 0
-0000a690: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-0000a6a0: 6973 6520 4e6f 7449 6d70 6c65 6d65 6e74  ise NotImplement
-0000a6b0: 6564 4572 726f 720a 2020 2020 2020 2020  edError.        
-0000a6c0: 6966 205f 5f64 6562 7567 5f5f 3a0a 2020  if __debug__:.  
-0000a6d0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-0000a6e0: 2e64 6562 7567 2827 207c 2054 6167 7320  .debug(' | Tags 
-0000a6f0: 2573 272c 2074 6167 735f 636c 290a 2020  %s', tags_cl).  
-0000a700: 2020 2020 2020 6173 7365 7274 206c 656e        assert len
-0000a710: 2874 6167 735f 636c 2920 3e3d 2032 2c20  (tags_cl) >= 2, 
-0000a720: 6627 4d69 7373 696e 6720 7461 6773 3a20  f'Missing tags: 
-0000a730: 7b74 6167 735f 636c 7d27 0a20 2020 2020  {tags_cl}'.     
-0000a740: 2020 2074 6167 735f 7072 6f63 203d 205b     tags_proc = [
-0000a750: 7420 666f 7220 7420 696e 2074 6167 735f  t for t in tags_
-0000a760: 636c 2069 6620 273a 3a27 2069 6e20 745d  cl if '::' in t]
-0000a770: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-0000a780: 6c65 6e28 7461 6773 5f70 726f 6329 203d  len(tags_proc) =
-0000a790: 3d20 310a 2020 2020 2020 2020 7461 6769  = 1.        tagi
-0000a7a0: 203d 2074 6167 735f 7072 6f63 5b30 5d0a   = tags_proc[0].
-0000a7b0: 2020 2020 2020 2020 7461 6720 3d20 7461          tag = ta
-0000a7c0: 6769 2e73 706c 6974 2827 3a3a 2729 5b30  gi.split('::')[0
-0000a7d0: 5d0a 2020 2020 2020 2020 6173 7365 7274  ].        assert
-0000a7e0: 2074 6167 5f6e 616d 6520 3d3d 2074 6167   tag_name == tag
-0000a7f0: 2c20 6627 5772 6f6e 6720 6f6e 436c 6963  , f'Wrong onClic
-0000a800: 6b54 6167 3a20 5265 7175 6573 7465 645b  kTag: Requested[
-0000a810: 7b74 6167 5f6e 616d 657d 5d20 213d 2046  {tag_name}] != F
-0000a820: 6f75 6e64 5b7b 7461 677d 5d27 0a20 2020  ound[{tag}]'.   
-0000a830: 2020 2020 2061 7373 6572 7420 7461 6720       assert tag 
-0000a840: 696e 2074 6167 735f 636c 2c20 6627 5772  in tags_cl, f'Wr
-0000a850: 6f6e 6720 7461 675f 696e 6465 783a 207b  ong tag_index: {
-0000a860: 7461 677d 5b7b 7461 6769 7d5d 270a 2020  tag}[{tagi}]'.  
-0000a870: 2020 2020 2020 7461 6773 5f6f 7468 6572        tags_other
-0000a880: 203d 205b 7420 666f 7220 7420 696e 2074   = [t for t in t
-0000a890: 6167 735f 636c 2069 6620 7420 6e6f 7420  ags_cl if t not 
-0000a8a0: 696e 2028 7461 672c 2074 6167 6929 5d0a  in (tag, tagi)].
-0000a8b0: 2020 2020 2020 2020 6966 205f 5f64 6562          if __deb
-0000a8c0: 7567 5f5f 3a0a 2020 2020 2020 2020 2020  ug__:.          
-0000a8d0: 2020 6c6f 6767 6572 2e64 6562 7567 2866    logger.debug(f
-0000a8e0: 2720 3d20 7b74 6167 7d5b 7b74 6167 697d  ' = {tag}[{tagi}
-0000a8f0: 5d27 290a 2020 2020 2020 2020 7365 6c66  ]').        self
-0000a900: 2e5f 7374 796c 655f 6128 7461 673d 7461  ._style_a(tag=ta
-0000a910: 6769 2c20 7669 7369 7465 643d 5472 7565  gi, visited=True
-0000a920: 290a 2020 2020 2020 2020 7365 6c66 2e6f  ).        self.o
-0000a930: 6e43 6c69 636b 5461 6728 7461 672c 2074  nClickTag(tag, t
-0000a940: 6167 692c 2074 6167 735f 6f74 6865 7229  agi, tags_other)
-0000a950: 0a0a 2020 2020 6465 6620 6f6e 436c 6963  ..    def onClic
-0000a960: 6b54 6167 2873 656c 662c 2074 6167 3a20  kTag(self, tag: 
-0000a970: 7374 722c 2074 6167 5f69 6e64 6578 3a20  str, tag_index: 
-0000a980: 7374 722c 2074 6167 735f 6f74 6865 723a  str, tags_other:
-0000a990: 2074 7970 696e 672e 5365 7175 656e 6365   typing.Sequence
-0000a9a0: 5b73 7472 5d29 202d 3e20 4e6f 6e65 3a0a  [str]) -> None:.
-0000a9b0: 2020 2020 2020 2020 2727 2743 616c 6c62          '''Callb
-0000a9c0: 6163 6b20 746f 2062 6520 6361 6c6c 6564  ack to be called
-0000a9d0: 2077 6865 6e20 636c 6963 6b69 6e67 2060   when clicking `
-0000a9e0: 6061 6060 2074 6167 7320 696e 2074 6869  `a`` tags in thi
-0000a9f0: 7320 7769 6467 6574 2e0a 0a20 2020 2020  s widget...     
-0000aa00: 2020 2044 6566 6175 6c74 7320 746f 2064     Defaults to d
-0000aa10: 6f69 6e67 206e 6f74 6869 6e67 2e0a 0a20  oing nothing... 
-0000aa20: 2020 2020 2020 2041 7661 696c 6162 6c65         Available
-0000aa30: 2066 6f72 2073 7562 636c 6173 7320 7265   for subclass re
-0000aa40: 6465 6669 6e69 7469 6f6e 2e0a 0a20 2020  definition...   
-0000aa50: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-0000aa60: 2020 2020 2020 2074 6167 3a20 5468 6520         tag: The 
-0000aa70: 6d61 696e 2074 6167 2074 7970 652e 2049  main tag type. I
-0000aa80: 6e20 7468 6973 2063 6173 652c 2069 7427  n this case, it'
-0000aa90: 7320 616c 7761 7973 2060 6061 6060 2e0a  s always ``a``..
-0000aaa0: 2020 2020 2020 2020 2020 2020 7461 675f              tag_
-0000aab0: 696e 6465 783a 2054 6865 2074 6167 2069  index: The tag i
-0000aac0: 6e64 6578 2e20 5365 6520 604c 544d 4c20  ndex. See `LTML 
-0000aad0: 3c70 6172 7365 722e 4c54 4d4c 3e60 2041  <parser.LTML>` A
-0000aae0: 7574 6f6d 6174 6963 2043 6f75 6e74 6572  utomatic Counter
-0000aaf0: 2074 6167 732e 0a20 2020 2020 2020 2020   tags..         
-0000ab00: 2020 2074 6167 735f 6f74 6865 723a 204c     tags_other: L
-0000ab10: 6973 7420 6f66 2065 7874 7261 2074 6167  ist of extra tag
-0000ab20: 7320 6174 7461 6368 6564 2074 6f20 7468  s attached to th
-0000ab30: 6520 616e 6368 6f72 2e20 4d69 6768 7420  e anchor. Might 
-0000ab40: 6265 2065 6d70 7479 2e0a 2020 2020 2020  be empty..      
-0000ab50: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
-0000ab60: 7373 0a0a 2020 2020 6465 6620 7773 7461  ss..    def wsta
-0000ab70: 7465 4c54 4d4c 2873 656c 6629 202d 3e20  teLTML(self) -> 
-0000ab80: 7479 7069 6e67 2e47 656e 6572 6174 6f72  typing.Generator
-0000ab90: 5b6d 6f64 656c 2e54 6578 7445 6c65 6d65  [model.TextEleme
-0000aba0: 6e74 2c20 4e6f 6e65 2c20 4e6f 6e65 5d3a  nt, None, None]:
-0000abb0: 0a20 2020 2020 2020 2027 2727 5265 7475  .        '''Retu
-0000abc0: 726e 2074 6865 2070 6172 7365 6420 4c54  rn the parsed LT
-0000abd0: 4d4c 2073 7461 7465 2c20 6173 2061 2067  ML state, as a g
-0000abe0: 656e 6572 6174 6f72 206f 6620 606d 6f64  enerator of `mod
-0000abf0: 656c 2e54 6578 7445 6c65 6d65 6e74 602e  el.TextElement`.
-0000ac00: 0a0a 2020 2020 2020 2020 5365 6520 416c  ..        See Al
-0000ac10: 736f 3a0a 2020 2020 2020 2020 2020 2020  so:.            
-0000ac20: 2d20 6077 7374 6174 6560 3a20 5265 7475  - `wstate`: Retu
-0000ac30: 726e 2074 6865 204c 544d 4c20 7374 7269  rn the LTML stri
-0000ac40: 6e67 2e0a 2020 2020 2020 2020 2020 2020  ng..            
-0000ac50: 2d20 6077 7374 6174 6554 6578 7460 3a20  - `wstateText`: 
-0000ac60: 5265 7475 726e 2074 6865 2075 6e64 6572  Return the under
-0000ac70: 6c79 696e 6720 7465 7874 2c20 7769 7468  lying text, with
-0000ac80: 6f75 7420 616e 7920 7461 6773 2e0a 2020  out any tags..  
-0000ac90: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-0000aca0: 2020 2320 544f 444f 3a20 5361 7665 2074    # TODO: Save t
-0000acb0: 6865 2070 6172 7365 6420 4c54 4d4c 2073  he parsed LTML s
-0000acc0: 7461 7465 2073 6f6d 6577 6865 7265 2069  tate somewhere i
-0000acd0: 6e20 7468 6973 206f 626a 6563 742c 2077  n this object, w
-0000ace0: 6974 6820 6064 6174 6160 3f0a 2020 2020  ith `data`?.    
-0000acf0: 2020 2020 7969 656c 6420 6672 6f6d 2070      yield from p
-0000ad00: 6172 7365 722e 7061 7273 655f 4c54 4d4c  arser.parse_LTML
-0000ad10: 2873 656c 662e 7773 7461 7465 290a 0a20  (self.wstate).. 
-0000ad20: 2020 2064 6566 2077 7374 6174 6554 6578     def wstateTex
-0000ad30: 7428 7365 6c66 2920 2d3e 2073 7472 3a0a  t(self) -> str:.
-0000ad40: 2020 2020 2020 2020 2727 2753 7472 6970          '''Strip
-0000ad50: 2061 6c6c 204c 544d 4c20 7461 6773 2061   all LTML tags a
-0000ad60: 6e64 2072 6574 7572 6e20 7468 6520 756e  nd return the un
-0000ad70: 6465 726c 7969 6e67 2074 6578 742e 0a0a  derlying text...
-0000ad80: 2020 2020 2020 2020 5365 6520 416c 736f          See Also
-0000ad90: 3a0a 2020 2020 2020 2020 2020 2020 2d20  :.            - 
-0000ada0: 6077 7374 6174 6560 3a20 5265 7475 726e  `wstate`: Return
-0000adb0: 2074 6865 204c 544d 4c20 7374 7269 6e67   the LTML string
-0000adc0: 2e0a 2020 2020 2020 2020 2020 2020 2d20  ..            - 
-0000add0: 6077 7374 6174 654c 544d 4c60 3a20 4765  `wstateLTML`: Ge
-0000ade0: 6e65 7261 7465 2061 206c 6973 7420 6f66  nerate a list of
-0000adf0: 204c 544d 4c20 7061 7273 6564 206f 626a   LTML parsed obj
-0000ae00: 6563 7473 2e0a 2020 2020 2020 2020 2727  ects..        ''
-0000ae10: 270a 2020 2020 2020 2020 2320 544f 444f  '.        # TODO
-0000ae20: 3a20 5361 7665 2074 6865 2070 6172 7365  : Save the parse
-0000ae30: 6420 4c54 4d4c 2073 7461 7465 2073 6f6d  d LTML state som
-0000ae40: 6577 6865 7265 2069 6e20 7468 6973 206f  ewhere in this o
-0000ae50: 626a 6563 742c 2077 6974 6820 6064 6174  bject, with `dat
-0000ae60: 6160 3f0a 2020 2020 2020 2020 7265 7475  a`?.        retu
-0000ae70: 726e 2027 272e 6a6f 696e 280a 2020 2020  rn ''.join(.    
-0000ae80: 2020 2020 2020 2020 7465 2e74 6578 740a          te.text.
-0000ae90: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000aea0: 7465 2069 6e20 7061 7273 6572 2e70 6172  te in parser.par
-0000aeb0: 7365 5f4c 544d 4c28 7365 6c66 2e77 7374  se_LTML(self.wst
-0000aec0: 6174 6529 0a20 2020 2020 2020 2029 0a0a  ate).        )..
-0000aed0: 0a63 6c61 7373 204e 6f74 6562 6f6f 6b28  .class Notebook(
-0000aee0: 7474 6b2e 4e6f 7465 626f 6f6b 2c20 6d69  ttk.Notebook, mi
-0000aef0: 7869 6e2e 436f 6e74 6169 6e65 7257 6964  xin.ContainerWid
-0000af00: 6765 7429 3a0a 2020 2020 2727 2741 2074  get):.    '''A t
-0000af10: 6162 6265 6420 696e 7465 7266 6163 6520  abbed interface 
-0000af20: 746f 2068 6f6c 6420 6f74 6865 7220 636f  to hold other co
-0000af30: 6e74 6169 6e65 7273 2e0a 0a20 2020 2054  ntainers...    T
-0000af40: 6869 7320 6973 2061 2074 6162 6265 6420  his is a tabbed 
-0000af50: 696e 7465 7266 6163 6520 746f 2073 686f  interface to sho
-0000af60: 7720 7365 7665 7261 6c20 636f 6e74 6169  w several contai
-0000af70: 6e65 7273 2069 6e20 7468 6520 7361 6d65  ners in the same
-0000af80: 2073 7061 6365 2e0a 0a20 2020 2054 6865   space...    The
-0000af90: 2069 6e64 6976 6964 7561 6c20 7461 6273   individual tabs
-0000afa0: 206d 7573 7420 616c 6c20 6265 2063 6f6e   must all be con
-0000afb0: 7461 696e 6572 732c 2074 6865 7265 2773  tainers, there's
-0000afc0: 206e 6f20 7375 7070 6f72 7420 666f 7220   no support for 
-0000afd0: 7369 6e67 6c65 0a20 2020 2077 6964 6765  single.    widge
-0000afe0: 7473 2e20 5573 6520 6120 686f 6c64 6572  ts. Use a holder
-0000aff0: 2060 4672 616d 6555 6e6c 6162 656c 6c65   `FrameUnlabelle
-0000b000: 6460 2074 6f20 7368 6f77 2061 2073 696e  d` to show a sin
-0000b010: 676c 6520 7769 6467 6574 2066 6f72 2065  gle widget for e
-0000b020: 6163 680a 2020 2020 7461 622e 0a0a 2020  ach.    tab...  
-0000b030: 2020 5468 6572 6520 6973 206e 6f20 5079    There is no Py
-0000b040: 7468 6f6e 2064 6f63 756d 656e 7461 7469  thon documentati
-0000b050: 6f6e 2c20 7365 6520 6060 546b 6060 2060  on, see ``Tk`` `
-0000b060: 7474 6b2e 4e6f 7465 626f 6f6b 203c 6874  ttk.Notebook <ht
-0000b070: 7470 733a 2f2f 7777 772e 7463 6c2e 746b  tps://www.tcl.tk
-0000b080: 2f6d 616e 2f74 636c 2f54 6b43 6d64 2f74  /man/tcl/TkCmd/t
-0000b090: 746b 5f6e 6f74 6562 6f6f 6b2e 6874 6d6c  tk_notebook.html
-0000b0a0: 3e60 5f20 646f 6375 6d65 6e74 6174 696f  >`_ documentatio
-0000b0b0: 6e2e 0a0a 2020 2020 4172 6773 3a0a 2020  n...    Args:.  
-0000b0c0: 2020 2020 2020 7472 6176 6572 7361 6c3a        traversal:
-0000b0d0: 2053 6574 7570 2074 6162 2074 7261 7665   Setup tab trave
-0000b0e0: 7273 616c 2077 6974 6820 7370 6563 6961  rsal with specia
-0000b0f0: 6c20 6b65 7962 6f61 7264 2073 686f 7274  l keyboard short
-0000b100: 6375 7473 2c20 616e 640a 2020 2020 2020  cuts, and.      
-0000b110: 2020 2020 2020 616c 736f 2077 6974 6820        also with 
-0000b120: 6d6f 7573 6520 7768 6565 6c20 7363 726f  mouse wheel scro
-0000b130: 6c6c 696e 672e 2053 6565 2074 6865 2054  lling. See the T
-0000b140: 6b20 646f 6375 6d65 6e74 6174 696f 6e20  k documentation 
-0000b150: 666f 7220 7468 650a 2020 2020 2020 2020  for the.        
-0000b160: 2020 2020 6b65 7962 6f61 7264 2070 6172      keyboard par
-0000b170: 742e 2045 6e61 626c 6564 2062 7920 6465  t. Enabled by de
-0000b180: 6661 756c 742e 0a20 2020 2020 2020 2074  fault..        t
-0000b190: 7261 7665 7273 616c 5772 6170 6172 6f75  raversalWraparou
-0000b1a0: 6e64 3a20 5768 656e 2060 6074 7261 7665  nd: When ``trave
-0000b1b0: 7273 616c 6060 2069 7320 7365 7475 702c  rsal`` is setup,
-0000b1c0: 2063 6f6e 6669 6775 7265 2077 7261 7061   configure wrapa
-0000b1d0: 726f 756e 642e 0a20 2020 2020 2020 2020  round..         
-0000b1e0: 2020 2054 6861 7420 6973 2c20 7363 726f     That is, scro
-0000b1f0: 6c6c 696e 6720 746f 2074 6865 206e 6578  lling to the nex
-0000b200: 7420 7461 6220 6672 6f6d 2074 6865 206c  t tab from the l
-0000b210: 6173 7420 6f6e 6520 7368 6f75 6c64 2022  ast one should "
-0000b220: 7363 726f 6c6c 220a 2020 2020 2020 2020  scroll".        
-0000b230: 2020 2020 696e 746f 2074 6865 2066 6972      into the fir
-0000b240: 7374 2074 6162 2c20 616e 6420 7669 6365  st tab, and vice
-0000b250: 2d76 6572 7361 2066 6f72 2074 6865 2066  -versa for the f
-0000b260: 6972 7374 2074 6162 2e20 5468 6973 206f  irst tab. This o
-0000b270: 6e6c 7920 6d61 7474 6572 730a 2020 2020  nly matters.    
-0000b280: 2020 2020 2020 2020 666f 7220 7468 6520          for the 
-0000b290: 6d6f 7573 6520 7768 6565 6c20 7472 6176  mouse wheel trav
-0000b2a0: 6572 7361 6c2c 2074 6865 206b 6579 626f  ersal, the keybo
-0000b2b0: 6172 6420 7368 6f72 7463 7574 7320 616c  ard shortcuts al
-0000b2c0: 7761 7973 2065 6e61 626c 650a 2020 2020  ways enable.    
-0000b2d0: 2020 2020 2020 2020 7468 6973 2074 7261          this tra
-0000b2e0: 7665 7273 616c 2e0a 2020 2020 2020 2020  versal..        
-0000b2f0: 2020 2020 4469 7361 626c 6564 2062 7920      Disabled by 
-0000b300: 6465 6661 756c 742e 0a0a 2020 2020 2020  default...      
-0000b310: 2020 6c61 796f 7574 3a20 4967 6e6f 7265    layout: Ignore
-0000b320: 642c 2069 7420 6973 2068 6172 6463 6f64  d, it is hardcod
-0000b330: 6564 2074 6f20 604e 6f6e 6560 2061 6c77  ed to `None` alw
-0000b340: 6179 732e 0a20 2020 2020 2020 2070 6172  ays..        par
-0000b350: 656e 743a 2054 6865 2070 6172 656e 7420  ent: The parent 
-0000b360: 7769 6467 6574 2e20 4361 6e20 6265 2061  widget. Can be a
-0000b370: 2060 526f 6f74 5769 6e64 6f77 6020 6f72   `RootWindow` or
-0000b380: 2061 6e6f 7468 6572 2060 6d69 7869 6e2e   another `mixin.
-0000b390: 436f 6e74 6169 6e65 7257 6964 6765 7460  ContainerWidget`
-0000b3a0: 2e0a 0a20 2020 2053 6565 2041 6c73 6f3a  ...    See Also:
-0000b3b0: 0a20 2020 2020 2020 2060 4e6f 7465 626f  .        `Notebo
-0000b3c0: 6f6b 556e 6966 6f72 6d60 3a20 4120 7369  okUniform`: A si
-0000b3d0: 6d70 6c65 7220 7665 7273 696f 6e20 6f66  mpler version of
-0000b3e0: 2074 6869 732c 2077 6865 6e20 6561 6368   this, when each
-0000b3f0: 2069 6e64 6976 6964 7561 6c20 7461 6220   individual tab 
-0000b400: 6973 2074 6865 2073 616d 6520 7479 7065  is the same type
-0000b410: 0a20 2020 2027 2727 0a20 2020 2054 6162  .    '''.    Tab
-0000b420: 203d 206d 6f64 656c 2e4e 6f74 6562 6f6f   = model.Noteboo
-0000b430: 6b54 6162 2020 2320 416c 6961 7320 7468  kTab  # Alias th
-0000b440: 6520 6e6f 7465 626f 6f6b 2074 6162 2069  e notebook tab i
-0000b450: 6e66 6f72 6d61 7469 6f6e 2020 2320 544f  nformation  # TO
-0000b460: 444f 3a20 4d6f 7665 204e 6f74 6562 6f6f  DO: Move Noteboo
-0000b470: 6b54 6162 2063 6c61 7373 2068 6572 653f  kTab class here?
-0000b480: 0a20 2020 2027 2727 416c 6961 7320 666f  .    '''Alias fo
-0000b490: 7220 606d 6f64 656c 2e4e 6f74 6562 6f6f  r `model.Noteboo
-0000b4a0: 6b54 6162 6020 636c 6173 732e 2727 270a  kTab` class.'''.
-0000b4b0: 2020 2020 7774 6162 733a 2074 7970 696e      wtabs: typin
-0000b4c0: 672e 4d61 7070 696e 675b 7374 722c 206d  g.Mapping[str, m
-0000b4d0: 6f64 656c 2e4e 6f74 6562 6f6f 6b54 6162  odel.NotebookTab
-0000b4e0: 5d0a 2020 2020 2727 274d 6170 7069 6e67  ].    '''Mapping
-0000b4f0: 206f 6620 7461 6220 6964 656e 7469 6669   of tab identifi
-0000b500: 6572 732c 2061 6e64 2060 6d6f 6465 6c2e  ers, and `model.
-0000b510: 4e6f 7465 626f 6f6b 5461 6260 206f 626a  NotebookTab` obj
-0000b520: 6563 7473 2e27 2727 0a0a 2020 2020 6465  ects.'''..    de
-0000b530: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-0000b540: 2070 6172 656e 742c 202a 6172 6773 2c20   parent, *args, 
-0000b550: 6c61 796f 7574 3a20 4e6f 6e65 203d 204e  layout: None = N
-0000b560: 6f6e 652c 2074 7261 7665 7273 616c 3a20  one, traversal: 
-0000b570: 626f 6f6c 203d 2054 7275 652c 2074 7261  bool = True, tra
-0000b580: 7665 7273 616c 5772 6170 6172 6f75 6e64  versalWraparound
-0000b590: 3a20 626f 6f6c 203d 2046 616c 7365 2c20  : bool = False, 
-0000b5a0: 2a2a 6b77 6172 6773 293a 0a20 2020 2020  **kwargs):.     
-0000b5b0: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
-0000b5c0: 745f 5f28 7061 7265 6e74 290a 2020 2020  t__(parent).    
-0000b5d0: 2020 2020 2320 4e6f 2060 6c61 796f 7574      # No `layout
-0000b5e0: 6020 6973 2075 7365 642c 2066 6f72 6365  ` is used, force
-0000b5f0: 2069 7420 746f 2060 4e6f 6e65 600a 2020   it to `None`.  
-0000b600: 2020 2020 2020 7365 6c66 2e69 6e69 745f        self.init_
-0000b610: 636f 6e74 6169 6e65 7228 2a61 7267 732c  container(*args,
-0000b620: 206c 6179 6f75 743d 4e6f 6e65 2c20 2a2a   layout=None, **
-0000b630: 6b77 6172 6773 290a 2020 2020 2020 2020  kwargs).        
-0000b640: 2320 5461 6220 5472 6176 6572 7361 6c0a  # Tab Traversal.
-0000b650: 2020 2020 2020 2020 7365 6c66 2e74 5772          self.tWr
-0000b660: 6170 6172 6f75 6e64 203d 2074 7261 7665  aparound = trave
-0000b670: 7273 616c 5772 6170 6172 6f75 6e64 0a20  rsalWraparound. 
-0000b680: 2020 2020 2020 2069 6620 7472 6176 6572         if traver
-0000b690: 7361 6c3a 0a20 2020 2020 2020 2020 2020  sal:.           
-0000b6a0: 2023 2054 4f44 4f3a 2052 652d 496d 706c   # TODO: Re-Impl
-0000b6b0: 656d 656e 7420 6c6f 6361 6c6c 792c 2074  ement locally, t
-0000b6c0: 616b 6520 6074 7261 7665 7273 616c 5772  ake `traversalWr
-0000b6d0: 6170 6172 6f75 6e64 6020 696e 746f 2061  aparound` into a
-0000b6e0: 6363 6f75 6e74 2e0a 2020 2020 2020 2020  ccount..        
-0000b6f0: 2020 2020 2320 2020 2020 2020 4d61 703a      #       Map:
-0000b700: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
-0000b710: 2020 2020 202d 2060 4374 726c 2d54 6162       - `Ctrl-Tab
-0000b720: 603a 205f 7461 6253 6372 6f6c 6c55 700a  `: _tabScrollUp.
-0000b730: 2020 2020 2020 2020 2020 2020 2320 2020              #   
-0000b740: 2020 2020 2d20 6043 7472 6c2d 5368 6966      - `Ctrl-Shif
-0000b750: 742d 5461 6260 3a20 5f74 6162 5363 726f  t-Tab`: _tabScro
-0000b760: 6c6c 446f 776e 0a20 2020 2020 2020 2020  llDown.         
-0000b770: 2020 2073 656c 662e 656e 6162 6c65 5f74     self.enable_t
-0000b780: 7261 7665 7273 616c 2829 0a20 2020 2020  raversal().     
-0000b790: 2020 2020 2020 2023 2042 696e 6420 6d6f         # Bind mo
-0000b7a0: 7573 6520 7768 6565 6c3a 2044 6967 6974  use wheel: Digit
-0000b7b0: 616c 2053 6372 6f6c 6c69 6e67 0a20 2020  al Scrolling.   
-0000b7c0: 2020 2020 2020 2020 2073 656c 662e 5f74           self._t
-0000b7d0: 7261 7665 7273 616c 203d 2066 6e2e 6269  raversal = fn.bi
-0000b7e0: 6e64 5f6d 6f75 7365 7768 6565 6c28 7365  nd_mousewheel(se
-0000b7f0: 6c66 2c20 7570 3d73 656c 662e 5f74 6162  lf, up=self._tab
-0000b800: 5363 726f 6c6c 5570 2c20 646f 776e 3d73  ScrollUp, down=s
-0000b810: 656c 662e 5f74 6162 5363 726f 6c6c 446f  elf._tabScrollDo
-0000b820: 776e 2c20 696d 6d65 6469 6174 653d 5472  wn, immediate=Tr
-0000b830: 7565 290a 0a20 2020 2064 6566 2073 6574  ue)..    def set
-0000b840: 7570 5f77 6964 6765 7473 2873 656c 662c  up_widgets(self,
-0000b850: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
-0000b860: 293a 0a20 2020 2020 2020 2027 2727 4465  ):.        '''De
-0000b870: 6669 6e65 2074 6865 2073 7562 2077 6964  fine the sub wid
-0000b880: 6765 7473 2062 6173 6564 206f 6e20 7468  gets based on th
-0000b890: 6520 7461 6273 2e0a 0a20 2020 2020 2020  e tabs...       
-0000b8a0: 2044 6f20 6e6f 7420 6f76 6572 7772 6974   Do not overwrit
-0000b8b0: 6520 7468 6973 2075 6e6c 6573 7320 796f  e this unless yo
-0000b8c0: 7520 6b6e 6f77 2077 6861 7420 796f 7520  u know what you 
-0000b8d0: 6172 6520 646f 696e 672e 0a0a 2020 2020  are doing...    
-0000b8e0: 2020 2020 546f 2065 6469 7420 7468 6520      To edit the 
-0000b8f0: 7461 6273 2c20 7365 6520 6073 6574 7570  tabs, see `setup
-0000b900: 5f74 6162 7360 2e0a 2020 2020 2020 2020  _tabs`..        
-0000b910: 2727 270a 2020 2020 2020 2020 7365 6c66  '''.        self
-0000b920: 2e77 7461 6273 203d 2073 656c 662e 7365  .wtabs = self.se
-0000b930: 7475 705f 7461 6273 282a 6172 6773 2c20  tup_tabs(*args, 
-0000b940: 2a2a 6b77 6172 6773 290a 2020 2020 2020  **kwargs).      
-0000b950: 2020 2320 6966 205f 5f64 6562 7567 5f5f    # if __debug__
-0000b960: 3a0a 2020 2020 2020 2020 2320 2020 2020  :.        #     
-0000b970: 6c6f 6767 6572 2e64 6562 7567 2866 277b  logger.debug(f'{
-0000b980: 7365 6c66 7d3a 207b 6c65 6e28 7365 6c66  self}: {len(self
-0000b990: 2e77 7461 6273 297d 2054 6162 7327 290a  .wtabs)} Tabs').
-0000b9a0: 2020 2020 2020 2020 7769 6467 6574 7320          widgets 
-0000b9b0: 3d20 7b7d 0a20 2020 2020 2020 2066 6f72  = {}.        for
-0000b9c0: 2069 6465 6e74 6966 6965 722c 2074 6920   identifier, ti 
-0000b9d0: 696e 2073 656c 662e 7774 6162 732e 6974  in self.wtabs.it
-0000b9e0: 656d 7328 293a 0a20 2020 2020 2020 2020  ems():.         
-0000b9f0: 2020 2023 2069 6620 5f5f 6465 6275 675f     # if __debug_
-0000ba00: 5f3a 0a20 2020 2020 2020 2020 2020 2023  _:.            #
-0000ba10: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-0000ba20: 6728 273e 2025 733a 2025 7227 2c20 7469  g('> %s: %r', ti
-0000ba30: 2e6e 616d 652c 2074 692e 7769 6467 6574  .name, ti.widget
-0000ba40: 290a 2020 2020 2020 2020 2020 2020 6173  ).            as
-0000ba50: 7365 7274 2069 7369 6e73 7461 6e63 6528  sert isinstance(
-0000ba60: 7469 2e77 6964 6765 742c 206d 6978 696e  ti.widget, mixin
-0000ba70: 2e43 6f6e 7461 696e 6572 5769 6467 6574  .ContainerWidget
-0000ba80: 292c 2066 277b 7365 6c66 2172 7d3a 2054  ), f'{self!r}: T
-0000ba90: 6162 2057 6964 6765 7420 5b7b 7469 2e69  ab Widget [{ti.i
-0000baa0: 6465 6e74 6966 6965 7220 6f72 2069 6465  dentifier or ide
-0000bab0: 6e74 6966 6965 727d 5d22 7b74 692e 6e61  ntifier}]"{ti.na
-0000bac0: 6d65 7d22 206d 7573 7420 6265 2061 2063  me}" must be a c
-0000bad0: 6f6e 7461 696e 6572 270a 2020 2020 2020  ontainer'.      
-0000bae0: 2020 2020 2020 6578 7472 6120 3d20 7b0a        extra = {.
-0000baf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb00: 2a2a 7469 2e65 7874 7261 2c0a 2020 2020  **ti.extra,.    
-0000bb10: 2020 2020 2020 2020 2020 2020 2774 6578              'tex
-0000bb20: 7427 3a20 7469 2e6e 616d 652c 0a20 2020  t': ti.name,.   
-0000bb30: 2020 2020 2020 2020 2020 2020 2027 696d               'im
-0000bb40: 6167 6527 3a20 7469 2e69 6d61 6765 206f  age': ti.image o
-0000bb50: 7220 2727 2c0a 2020 2020 2020 2020 2020  r '',.          
-0000bb60: 2020 2020 2020 2763 6f6d 706f 756e 6427        'compound'
-0000bb70: 3a20 7469 2e69 6d61 6765 436f 6d70 6f75  : ti.imageCompou
-0000bb80: 6e64 2c0a 2020 2020 2020 2020 2020 2020  nd,.            
-0000bb90: 7d0a 2020 2020 2020 2020 2020 2020 7365  }.            se
-0000bba0: 6c66 2e61 6464 2874 692e 7769 6467 6574  lf.add(ti.widget
-0000bbb0: 2c20 2a2a 6578 7472 6129 0a20 2020 2020  , **extra).     
-0000bbc0: 2020 2020 2020 2074 692e 6964 656e 7469         ti.identi
-0000bbd0: 6669 6572 203d 2069 6465 6e74 6966 6965  fier = identifie
-0000bbe0: 720a 2020 2020 2020 2020 2020 2020 7769  r.            wi
-0000bbf0: 6467 6574 735b 6964 656e 7469 6669 6572  dgets[identifier
-0000bc00: 5d20 3d20 7469 2e77 6964 6765 740a 2020  ] = ti.widget.  
-0000bc10: 2020 2020 2020 7265 7475 726e 2077 6964        return wid
-0000bc20: 6765 7473 0a0a 2020 2020 6465 6620 7365  gets..    def se
-0000bc30: 7475 705f 7461 6273 2873 656c 662c 202a  tup_tabs(self, *
-0000bc40: 6172 6773 2c20 2a2a 6b77 6172 6773 2920  args, **kwargs) 
-0000bc50: 2d3e 2074 7970 696e 672e 4d61 7070 696e  -> typing.Mappin
-0000bc60: 675b 7374 722c 206d 6f64 656c 2e4e 6f74  g[str, model.Not
-0000bc70: 6562 6f6f 6b54 6162 5d3a 0a20 2020 2020  ebookTab]:.     
-0000bc80: 2020 2027 2727 4465 6669 6e65 2074 6865     '''Define the
-0000bc90: 2074 6162 7320 6865 7265 2e0a 0a20 2020   tabs here...   
-0000bca0: 2020 2020 2053 696d 696c 6172 2074 6f20       Similar to 
-0000bcb0: 6073 6574 7570 5f77 6964 6765 7473 203c  `setup_widgets <
-0000bcc0: 6d69 7869 6e2e 436f 6e74 6169 6e65 7257  mixin.ContainerW
-0000bcd0: 6964 6765 742e 7365 7475 705f 7769 6467  idget.setup_widg
-0000bce0: 6574 733e 602c 2062 7574 0a20 2020 2020  ets>`, but.     
-0000bcf0: 2020 2064 6566 696e 6573 2060 6d6f 6465     defines `mode
-0000bd00: 6c2e 4e6f 7465 626f 6f6b 5461 6260 2c20  l.NotebookTab`, 
-0000bd10: 6578 7472 6120 696e 666f 726d 6174 696f  extra informatio
-0000bd20: 6e20 6162 6f75 7420 6561 6368 2077 6964  n about each wid
-0000bd30: 6765 742e 0a20 2020 2020 2020 2027 2727  get..        '''
-0000bd40: 0a20 2020 2020 2020 2072 6169 7365 204e  .        raise N
-0000bd50: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
-0000bd60: 6f72 0a0a 2020 2020 6465 6620 7774 6162  or..    def wtab
-0000bd70: 2873 656c 662c 2069 6478 3a20 7374 7229  (self, idx: str)
-0000bd80: 202d 3e20 6d69 7869 6e2e 436f 6e74 6169   -> mixin.Contai
-0000bd90: 6e65 7257 6964 6765 743a 0a20 2020 2020  nerWidget:.     
-0000bda0: 2020 2027 2727 4765 7420 7468 6520 7461     '''Get the ta
-0000bdb0: 6220 7769 6467 6574 2062 7920 6964 656e  b widget by iden
-0000bdc0: 7469 6669 6572 2e0a 0a20 2020 2020 2020  tifier...       
-0000bdd0: 2054 6869 7320 6973 206a 7573 7420 616e   This is just an
-0000bde0: 2068 656c 7065 7220 6675 6e63 7469 6f6e   helper function
-0000bdf0: 2074 6f20 6765 7420 7468 6520 636f 7272   to get the corr
-0000be00: 6563 7420 7769 6467 6574 2076 616c 7565  ect widget value
-0000be10: 206f 7574 206f 660a 2020 2020 2020 2020   out of.        
-0000be20: 6077 7461 6273 602e 0a0a 2020 2020 2020  `wtabs`...      
-0000be30: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-0000be40: 2020 2020 6964 783a 2054 6865 2074 6162      idx: The tab
-0000be50: 2069 6465 6e74 6966 6965 722e 0a0a 2020   identifier...  
-0000be60: 2020 2020 2020 4e6f 7465 3a0a 2020 2020        Note:.    
-0000be70: 2020 2020 2020 2020 496e 2064 6562 7567          In debug
-0000be80: 206d 6f64 652c 2074 6869 7320 7769 6c6c   mode, this will
-0000be90: 2066 6169 6c20 6966 2063 616c 6c65 6420   fail if called 
-0000bea0: 7769 7468 2074 6865 2077 726f 6e67 2069  with the wrong i
-0000beb0: 6465 6e74 6966 6965 722e 0a20 2020 2020  dentifier..     
-0000bec0: 2020 2020 2020 2054 6869 7320 6368 6563         This chec
-0000bed0: 6b20 6973 2073 6b69 7070 6564 2066 6f72  k is skipped for
-0000bee0: 2070 6572 666f 726d 616e 6365 206f 6e20   performance on 
-0000bef0: 6f70 7469 6d69 7a65 6420 6d6f 6465 2e0a  optimized mode..
-0000bf00: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-0000bf10: 2020 2020 7774 6162 203d 2073 656c 662e      wtab = self.
-0000bf20: 7774 6162 732e 6765 7428 6964 782c 204e  wtabs.get(idx, N
-0000bf30: 6f6e 6529 0a20 2020 2020 2020 2061 7373  one).        ass
-0000bf40: 6572 7420 7774 6162 2069 7320 6e6f 7420  ert wtab is not 
-0000bf50: 4e6f 6e65 2c20 6627 496e 7661 6c69 6420  None, f'Invalid 
-0000bf60: 5365 6c65 6374 696f 6e3a 207b 6964 787d  Selection: {idx}
-0000bf70: 270a 2020 2020 2020 2020 7265 7475 726e  '.        return
-0000bf80: 2077 7461 622e 7769 6467 6574 0a0a 2020   wtab.widget..  
-0000bf90: 2020 6465 6620 7773 656c 6563 7469 6f6e    def wselection
-0000bfa0: 2873 656c 6629 202d 3e20 7374 723a 0a20  (self) -> str:. 
-0000bfb0: 2020 2020 2020 2027 2727 5365 6172 6368         '''Search
-0000bfc0: 2066 6f72 2074 6865 2063 7572 7265 6e74   for the current
-0000bfd0: 2073 656c 6563 7465 6420 7461 622e 0a0a   selected tab...
-0000bfe0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-0000bff0: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
-0000c000: 7320 6675 6e63 7469 6f6e 7320 7365 6172  s functions sear
-0000c010: 6368 6573 2066 6f72 2074 6865 2063 7572  ches for the cur
-0000c020: 7265 6e74 6c79 2073 656c 6563 7465 6420  rently selected 
-0000c030: 7461 622c 2061 6e64 2072 6574 7572 6e73  tab, and returns
-0000c040: 2069 7473 0a20 2020 2020 2020 2020 2020   its.           
-0000c050: 2069 6465 6e74 6966 6965 7220 2874 6865   identifier (the
-0000c060: 206b 6579 206f 6e20 7468 6520 6077 7461   key on the `wta
-0000c070: 6273 6020 6469 6374 696f 6e61 7279 292e  bs` dictionary).
-0000c080: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-0000c090: 2020 2020 2023 2054 4f44 4f3a 204f 7074       # TODO: Opt
-0000c0a0: 696d 6973 6520 7468 6973 3f20 5361 7665  imise this? Save
-0000c0b0: 2061 2064 6963 7420 6f66 2069 6e64 6578   a dict of index
-0000c0c0: 6573 206f 7220 736f 6d65 7468 696e 673f  es or something?
-0000c0d0: 0a20 2020 2020 2020 2073 656c 6563 7465  .        selecte
-0000c0e0: 645f 6964 203d 2073 656c 662e 7365 6c65  d_id = self.sele
-0000c0f0: 6374 2829 0a20 2020 2020 2020 2023 2069  ct().        # i
-0000c100: 6620 5f5f 6465 6275 675f 5f3a 0a20 2020  f __debug__:.   
-0000c110: 2020 2020 2023 2020 2020 206c 6f67 6765       #     logge
-0000c120: 722e 6465 6275 6728 2753 3a20 2572 272c  r.debug('S: %r',
-0000c130: 2073 656c 6563 7465 645f 6964 290a 2020   selected_id).  
-0000c140: 2020 2020 2020 2320 2020 2020 7461 6273        #     tabs
-0000c150: 5f69 6420 3d20 5b73 7472 2877 2920 666f  _id = [str(w) fo
-0000c160: 7220 7720 696e 2073 656c 662e 7461 6273  r w in self.tabs
-0000c170: 2829 5d0a 2020 2020 2020 2020 2320 2020  ()].        #   
-0000c180: 2020 6c6f 6767 6572 2e64 6562 7567 2827    logger.debug('
-0000c190: 207c 2025 7327 2c20 2720 272e 6a6f 696e   | %s', ' '.join
-0000c1a0: 2874 6162 735f 6964 2929 0a20 2020 2020  (tabs_id)).     
-0000c1b0: 2020 2066 6f72 2069 6478 2c20 7774 6162     for idx, wtab
-0000c1c0: 2069 6e20 7365 6c66 2e77 7461 6273 2e69   in self.wtabs.i
-0000c1d0: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
-0000c1e0: 2020 2020 6966 2073 7472 2877 7461 622e      if str(wtab.
-0000c1f0: 7769 6467 6574 2920 3d3d 2073 656c 6563  widget) == selec
-0000c200: 7465 645f 6964 3a0a 2020 2020 2020 2020  ted_id:.        
-0000c210: 2020 2020 2020 2020 7265 7475 726e 2069          return i
-0000c220: 6478 0a20 2020 2020 2020 2072 6169 7365  dx.        raise
-0000c230: 2056 616c 7565 4572 726f 7228 277b 7365   ValueError('{se
-0000c240: 6c66 2172 7d3a 2049 6e76 616c 6964 2063  lf!r}: Invalid c
-0000c250: 7572 7265 6e74 2073 656c 6563 7469 6f6e  urrent selection
-0000c260: 3a20 7b73 656c 6563 7465 645f 6964 2172  : {selected_id!r
-0000c270: 7d27 290a 0a20 2020 2064 6566 2077 7365  }')..    def wse
-0000c280: 6c65 6374 2873 656c 662c 2069 6478 3a20  lect(self, idx: 
-0000c290: 7374 7229 202d 3e20 4e6f 6e65 3a0a 2020  str) -> None:.  
-0000c2a0: 2020 2020 2020 2727 2753 656c 6563 7420        '''Select 
-0000c2b0: 6120 7461 6220 6279 2069 6465 6e74 6966  a tab by identif
-0000c2c0: 6965 722e 0a0a 2020 2020 2020 2020 4172  ier...        Ar
-0000c2d0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-0000c2e0: 6964 783a 2054 6865 2074 6162 2069 6465  idx: The tab ide
-0000c2f0: 6e74 6966 6965 722e 0a0a 2020 2020 2020  ntifier...      
-0000c300: 2020 4e6f 7465 3a0a 2020 2020 2020 2020    Note:.        
-0000c310: 2020 2020 496e 2064 6562 7567 206d 6f64      In debug mod
-0000c320: 652c 2074 6869 7320 7769 6c6c 2066 6169  e, this will fai
-0000c330: 6c20 6966 2063 616c 6c65 6420 7769 7468  l if called with
-0000c340: 2074 6865 2077 726f 6e67 2069 6465 6e74   the wrong ident
-0000c350: 6966 6965 722e 0a20 2020 2020 2020 2020  ifier..         
-0000c360: 2020 2054 6869 7320 6368 6563 6b20 6973     This check is
-0000c370: 2073 6b69 7070 6564 2066 6f72 2070 6572   skipped for per
-0000c380: 666f 726d 616e 6365 206f 6e20 6f70 7469  formance on opti
-0000c390: 6d69 7a65 6420 6d6f 6465 2e0a 2020 2020  mized mode..    
-0000c3a0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-0000c3b0: 7774 6162 203d 2073 656c 662e 7774 6162  wtab = self.wtab
-0000c3c0: 732e 6765 7428 6964 782c 204e 6f6e 6529  s.get(idx, None)
-0000c3d0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-0000c3e0: 7774 6162 2069 7320 6e6f 7420 4e6f 6e65  wtab is not None
-0000c3f0: 2c20 6627 496e 7661 6c69 6420 5365 6c65  , f'Invalid Sele
-0000c400: 6374 696f 6e3a 207b 6964 787d 270a 2020  ction: {idx}'.  
-0000c410: 2020 2020 2020 7365 6c66 2e73 656c 6563        self.selec
-0000c420: 7428 7461 625f 6964 3d73 7472 2877 7461  t(tab_id=str(wta
-0000c430: 622e 7769 6467 6574 2929 0a0a 2020 2020  b.widget))..    
-0000c440: 6465 6620 5f74 6162 5363 726f 6c6c 5570  def _tabScrollUp
-0000c450: 2873 656c 662c 2065 7665 6e74 3d4e 6f6e  (self, event=Non
-0000c460: 6529 3a0a 2020 2020 2020 2020 6b65 7973  e):.        keys
-0000c470: 203d 206c 6973 7428 7365 6c66 2e77 7461   = list(self.wta
-0000c480: 6273 2e6b 6579 7328 2929 0a20 2020 2020  bs.keys()).     
-0000c490: 2020 2073 656c 6563 7465 6420 3d20 7365     selected = se
-0000c4a0: 6c66 2e77 7365 6c65 6374 696f 6e28 290a  lf.wselection().
-0000c4b0: 2020 2020 2020 2020 6966 2073 656c 6563          if selec
-0000c4c0: 7465 6420 3d3d 206b 6579 735b 305d 3a0a  ted == keys[0]:.
-0000c4d0: 2020 2020 2020 2020 2020 2020 2320 4669              # Fi
-0000c4e0: 7273 7420 5461 620a 2020 2020 2020 2020  rst Tab.        
-0000c4f0: 2020 2020 6966 2073 656c 662e 7457 7261      if self.tWra
-0000c500: 7061 726f 756e 643a 0a20 2020 2020 2020  paround:.       
-0000c510: 2020 2020 2020 2020 206e 6577 5f73 656c           new_sel
-0000c520: 6563 7465 6420 3d20 6b65 7973 5b2d 315d  ected = keys[-1]
-0000c530: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0000c540: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000c550: 2020 206e 6577 5f73 656c 6563 7465 6420     new_selected 
-0000c560: 3d20 4e6f 6e65 0a20 2020 2020 2020 2065  = None.        e
-0000c570: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000c580: 2023 2054 4f44 4f3a 204f 7074 696d 6973   # TODO: Optimis
-0000c590: 6520 7468 6973 3f20 5365 6520 6077 7365  e this? See `wse
-0000c5a0: 6c65 6374 696f 6e60 0a20 2020 2020 2020  lection`.       
-0000c5b0: 2020 2020 2073 656c 6563 7465 645f 6964       selected_id
-0000c5c0: 7820 3d20 6b65 7973 2e69 6e64 6578 2873  x = keys.index(s
-0000c5d0: 656c 6563 7465 6429 0a20 2020 2020 2020  elected).       
-0000c5e0: 2020 2020 206e 6577 5f73 656c 6563 7465       new_selecte
-0000c5f0: 6420 3d20 6b65 7973 5b73 656c 6563 7465  d = keys[selecte
-0000c600: 645f 6964 7820 2d20 315d 0a20 2020 2020  d_idx - 1].     
-0000c610: 2020 2069 6620 6e65 775f 7365 6c65 6374     if new_select
-0000c620: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
-0000c630: 7365 6c66 2e77 7365 6c65 6374 286e 6577  self.wselect(new
-0000c640: 5f73 656c 6563 7465 6429 0a0a 2020 2020  _selected)..    
-0000c650: 6465 6620 5f74 6162 5363 726f 6c6c 446f  def _tabScrollDo
-0000c660: 776e 2873 656c 662c 2065 7665 6e74 3d4e  wn(self, event=N
-0000c670: 6f6e 6529 3a0a 2020 2020 2020 2020 6b65  one):.        ke
-0000c680: 7973 203d 206c 6973 7428 7365 6c66 2e77  ys = list(self.w
-0000c690: 7461 6273 2e6b 6579 7328 2929 0a20 2020  tabs.keys()).   
-0000c6a0: 2020 2020 2073 656c 6563 7465 6420 3d20       selected = 
-0000c6b0: 7365 6c66 2e77 7365 6c65 6374 696f 6e28  self.wselection(
-0000c6c0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0000c6d0: 6563 7465 6420 3d3d 206b 6579 735b 2d31  ected == keys[-1
-0000c6e0: 5d3a 0a20 2020 2020 2020 2020 2020 2023  ]:.            #
-0000c6f0: 204c 6173 7420 5461 620a 2020 2020 2020   Last Tab.      
-0000c700: 2020 2020 2020 6966 2073 656c 662e 7457        if self.tW
-0000c710: 7261 7061 726f 756e 643a 0a20 2020 2020  raparound:.     
-0000c720: 2020 2020 2020 2020 2020 206e 6577 5f73             new_s
-0000c730: 656c 6563 7465 6420 3d20 6b65 7973 5b30  elected = keys[0
-0000c740: 5d0a 2020 2020 2020 2020 2020 2020 656c  ].            el
-0000c750: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000c760: 2020 2020 6e65 775f 7365 6c65 6374 6564      new_selected
-0000c770: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-0000c780: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000c790: 2020 2320 544f 444f 3a20 4f70 7469 6d69    # TODO: Optimi
-0000c7a0: 7365 2074 6869 733f 2053 6565 2060 7773  se this? See `ws
-0000c7b0: 656c 6563 7469 6f6e 600a 2020 2020 2020  election`.      
-0000c7c0: 2020 2020 2020 7365 6c65 6374 6564 5f69        selected_i
-0000c7d0: 6478 203d 206b 6579 732e 696e 6465 7828  dx = keys.index(
-0000c7e0: 7365 6c65 6374 6564 290a 2020 2020 2020  selected).      
-0000c7f0: 2020 2020 2020 6e65 775f 7365 6c65 6374        new_select
-0000c800: 6564 203d 206b 6579 735b 7365 6c65 6374  ed = keys[select
-0000c810: 6564 5f69 6478 202b 2031 5d0a 2020 2020  ed_idx + 1].    
-0000c820: 2020 2020 6966 206e 6577 5f73 656c 6563      if new_selec
-0000c830: 7465 643a 0a20 2020 2020 2020 2020 2020  ted:.           
-0000c840: 2073 656c 662e 7773 656c 6563 7428 6e65   self.wselect(ne
-0000c850: 775f 7365 6c65 6374 6564 290a 0a0a 636c  w_selected)...cl
-0000c860: 6173 7320 4e6f 7465 626f 6f6b 556e 6966  ass NotebookUnif
-0000c870: 6f72 6d28 4e6f 7465 626f 6f6b 293a 0a20  orm(Notebook):. 
-0000c880: 2020 2027 2727 4120 7461 6262 6564 2069     '''A tabbed i
-0000c890: 6e74 6572 6661 6365 2074 6f20 686f 6c64  nterface to hold
-0000c8a0: 2061 2073 6572 6965 7320 6f66 2075 6e69   a series of uni
-0000c8b0: 666f 726d 2063 6f6e 7461 696e 6572 732e  form containers.
-0000c8c0: 0a0a 2020 2020 5468 6973 2069 7320 6120  ..    This is a 
-0000c8d0: 7661 7269 616e 7420 6f66 2074 6865 2072  variant of the r
-0000c8e0: 6567 756c 6172 2060 4e6f 7465 626f 6f6b  egular `Notebook
-0000c8f0: 6020 7370 6563 6961 6c6c 7920 6372 6561  ` specially crea
-0000c900: 7465 6420 746f 2073 696d 706c 6966 790a  ted to simplify.
-0000c910: 2020 2020 7468 6520 7573 7561 6c20 6361      the usual ca
-0000c920: 7365 2077 6865 7265 2061 6c6c 2074 6865  se where all the
-0000c930: 2074 6162 7320 6172 6520 7665 7279 2073   tabs are very s
-0000c940: 696d 696c 6172 2028 7573 7561 6c6c 792c  imilar (usually,
-0000c950: 2074 6865 7920 6172 6520 7468 650a 2020   they are the.  
-0000c960: 2020 7361 6d65 2075 6e64 6572 6c79 696e    same underlyin
-0000c970: 6720 636c 6173 7329 2e0a 0a20 2020 2041  g class)...    A
-0000c980: 7267 733a 0a20 2020 2020 2020 2074 6162  rgs:.        tab
-0000c990: 6964 733a 2041 206d 6170 7069 6e67 206f  ids: A mapping o
-0000c9a0: 6620 7461 6220 6964 656e 7469 6669 6572  f tab identifier
-0000c9b0: 7320 616e 6420 7461 6220 7469 746c 6573  s and tab titles
-0000c9c0: 2e0a 0a20 2020 2053 6565 2041 6c73 6f3a  ...    See Also:
-0000c9d0: 0a20 2020 2020 2020 2060 4e6f 7465 626f  .        `Notebo
-0000c9e0: 6f6b 603a 2041 2066 756c 6c79 2067 656e  ok`: A fully gen
-0000c9f0: 6572 6963 2076 6572 7369 6f6e 206f 6620  eric version of 
-0000ca00: 7468 6973 2e20 446f 6e27 7420 7472 7920  this. Don't try 
-0000ca10: 746f 206d 616b 6520 7468 650a 2020 2020  to make the.    
-0000ca20: 2020 2020 6073 6574 7570 5f74 6162 6020      `setup_tab` 
-0000ca30: 6675 6e63 7469 6f6e 2074 6f6f 2063 6f6d  function too com
-0000ca40: 706c 6578 2c20 6d6f 7665 2074 6f20 7468  plex, move to th
-0000ca50: 6973 2077 6964 6765 7420 696e 7374 6561  is widget instea
-0000ca60: 642e 0a20 2020 2027 2727 0a20 2020 2074  d..    '''.    t
-0000ca70: 6162 6964 733a 2074 7970 696e 672e 4f70  abids: typing.Op
-0000ca80: 7469 6f6e 616c 5b74 7970 696e 672e 4d61  tional[typing.Ma
-0000ca90: 7070 696e 675b 7374 722c 2073 7472 5d5d  pping[str, str]]
-0000caa0: 203d 204e 6f6e 650a 0a20 2020 2064 6566   = None..    def
-0000cab0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-0000cac0: 2a61 7267 732c 2074 6162 6964 733a 2074  *args, tabids: t
-0000cad0: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
-0000cae0: 7970 696e 672e 4d61 7070 696e 675b 7374  yping.Mapping[st
-0000caf0: 722c 2073 7472 5d5d 203d 204e 6f6e 652c  r, str]] = None,
-0000cb00: 202a 2a6b 7761 7267 7329 3a0a 2020 2020   **kwargs):.    
-0000cb10: 2020 2020 7365 6c66 2e74 6162 6964 7320      self.tabids 
-0000cb20: 3d20 7365 6c66 2e74 6162 6964 7320 6f72  = self.tabids or
-0000cb30: 2074 6162 6964 730a 2020 2020 2020 2020   tabids.        
-0000cb40: 6966 2073 656c 662e 7461 6269 6473 2069  if self.tabids i
-0000cb50: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-0000cb60: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-0000cb70: 7272 6f72 2827 7b73 656c 6621 727d 3a20  rror('{self!r}: 
-0000cb80: 4d69 7373 696e 6720 7265 7175 6972 6564  Missing required
-0000cb90: 2074 6162 6964 7327 290a 2020 2020 2020   tabids').      
-0000cba0: 2020 7375 7065 7228 292e 5f5f 696e 6974    super().__init
-0000cbb0: 5f5f 282a 6172 6773 2c20 2a2a 6b77 6172  __(*args, **kwar
-0000cbc0: 6773 290a 0a20 2020 2064 6566 2073 6574  gs)..    def set
-0000cbd0: 7570 5f74 6162 7328 7365 6c66 2c20 2a61  up_tabs(self, *a
-0000cbe0: 7267 732c 202a 2a6b 7761 7267 7329 202d  rgs, **kwargs) -
-0000cbf0: 3e20 7479 7069 6e67 2e4d 6170 7069 6e67  > typing.Mapping
-0000cc00: 5b73 7472 2c20 6d6f 6465 6c2e 4e6f 7465  [str, model.Note
-0000cc10: 626f 6f6b 5461 625d 3a0a 2020 2020 2020  bookTab]:.      
-0000cc20: 2020 2727 2744 6566 696e 6520 7468 6520    '''Define the 
-0000cc30: 7375 6220 7461 6273 2c20 6261 7365 6420  sub tabs, based 
-0000cc40: 6f6e 2074 6865 2063 6f6d 6d6f 6e20 7461  on the common ta
-0000cc50: 622e 0a0a 2020 2020 2020 2020 446f 206e  b...        Do n
-0000cc60: 6f74 206f 7665 7277 7269 7465 2074 6869  ot overwrite thi
-0000cc70: 7320 756e 6c65 7373 2079 6f75 206b 6e6f  s unless you kno
-0000cc80: 7720 7768 6174 2079 6f75 2061 7265 2064  w what you are d
-0000cc90: 6f69 6e67 2e0a 0a20 2020 2020 2020 2054  oing...        T
-0000cca0: 6f20 6564 6974 2074 6865 2063 6f6d 6d6f  o edit the commo
-0000ccb0: 6e20 7461 622c 2073 6565 2060 7365 7475  n tab, see `setu
-0000ccc0: 705f 7461 6260 2e0a 2020 2020 2020 2020  p_tab`..        
-0000ccd0: 2727 270a 2020 2020 2020 2020 6173 7365  '''.        asse
-0000cce0: 7274 2073 656c 662e 7461 6269 6473 2069  rt self.tabids i
-0000ccf0: 7320 6e6f 7420 4e6f 6e65 0a20 2020 2020  s not None.     
-0000cd00: 2020 2074 6162 7320 3d20 7b7d 0a20 2020     tabs = {}.   
-0000cd10: 2020 2020 2066 6f72 2074 6964 2c20 746e       for tid, tn
-0000cd20: 616d 6520 696e 2073 656c 662e 7461 6269  ame in self.tabi
-0000cd30: 6473 2e69 7465 6d73 2829 3a0a 2020 2020  ds.items():.    
-0000cd40: 2020 2020 2020 2020 7461 6273 5b74 6964          tabs[tid
-0000cd50: 5d20 3d20 4e6f 7465 626f 6f6b 2e54 6162  ] = Notebook.Tab
-0000cd60: 2874 6e61 6d65 2c0a 2020 2020 2020 2020  (tname,.        
-0000cd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000cd90: 662e 7365 7475 705f 7461 6228 7469 642c  f.setup_tab(tid,
-0000cda0: 2074 6e61 6d65 292c 0a20 2020 2020 2020   tname),.       
-0000cdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cdc0: 2020 2020 2020 2020 2020 2020 2020 2a61                *a
-0000cdd0: 7267 732c 202a 2a6b 7761 7267 7329 0a20  rgs, **kwargs). 
-0000cde0: 2020 2020 2020 2072 6574 7572 6e20 7461         return ta
-0000cdf0: 6273 0a0a 2020 2020 6465 6620 7365 7475  bs..    def setu
-0000ce00: 705f 7461 6228 7365 6c66 2c20 6964 656e  p_tab(self, iden
-0000ce10: 7469 6669 6572 3a20 7374 722c 206e 616d  tifier: str, nam
-0000ce20: 653a 2073 7472 2920 2d3e 206d 6978 696e  e: str) -> mixin
-0000ce30: 2e43 6f6e 7461 696e 6572 5769 6467 6574  .ContainerWidget
-0000ce40: 3a0a 2020 2020 2020 2020 2727 2744 6566  :.        '''Def
-0000ce50: 696e 6520 7468 6520 636f 6d6d 6f6e 2074  ine the common t
-0000ce60: 6162 2060 436f 6e74 6169 6e65 7257 6964  ab `ContainerWid
-0000ce70: 6765 7460 2068 6572 652e 0a0a 2020 2020  get` here...    
-0000ce80: 2020 2020 5369 6d69 6c61 7220 746f 2060      Similar to `
-0000ce90: 7365 7475 705f 7461 6273 203c 4e6f 7465  setup_tabs <Note
-0000cea0: 626f 6f6b 2e73 6574 7570 5f74 6162 733e  book.setup_tabs>
-0000ceb0: 602c 2062 7574 2066 6f72 2061 2073 696e  `, but for a sin
-0000cec0: 676c 6520 7461 6220 7769 6467 6574 2e0a  gle tab widget..
-0000ced0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-0000cee0: 2020 2020 7261 6973 6520 4e6f 7449 6d70      raise NotImp
-0000cef0: 6c65 6d65 6e74 6564 4572 726f 720a 0a0a  lementedError...
-0000cf00: 636c 6173 7320 5472 6565 2874 746b 2e54  class Tree(ttk.T
-0000cf10: 7265 6576 6965 772c 206d 6978 696e 2e53  reeview, mixin.S
-0000cf20: 696e 676c 6557 6964 6765 7429 3a0a 2020  ingleWidget):.  
-0000cf30: 2020 2727 2741 2068 6965 7261 7263 6869    '''A hierarchi
-0000cf40: 6361 6c20 6d75 6c74 6963 6f6c 756d 6e20  cal multicolumn 
-0000cf50: 6461 7461 2064 6973 706c 6179 2077 6964  data display wid
-0000cf60: 6765 742e 0a0a 2020 2020 5468 6973 2077  get...    This w
-0000cf70: 6964 6765 7420 6973 2063 6170 6162 6c65  idget is capable
-0000cf80: 206f 6620 7368 6f77 696e 6720 6120 6869   of showing a hi
-0000cf90: 6572 6172 6368 7920 6f66 2064 6174 6120  erarchy of data 
-0000cfa0: 7265 636f 7264 7320 286f 6e65 2070 6572  records (one per
-0000cfb0: 0a20 2020 2072 6f77 292e 2045 6163 6820  .    row). Each 
-0000cfc0: 7265 636f 7264 2063 616e 2068 6176 6520  record can have 
-0000cfd0: 6d75 6c74 6970 6c65 2063 6f6c 756d 6e73  multiple columns
-0000cfe0: 206f 6620 6461 7461 2e0a 2020 2020 4561   of data..    Ea
-0000cff0: 6368 2072 6563 6f72 6420 6361 6e20 7374  ch record can st
-0000d000: 6f72 6520 6172 6269 7472 6172 7920 6461  ore arbitrary da
-0000d010: 7461 206f 6e20 6974 7320 6045 6c65 6d65  ta on its `Eleme
-0000d020: 6e74 203c 6d6f 6465 6c2e 5472 6565 456c  nt <model.TreeEl
-0000d030: 656d 656e 743e 602c 0a20 2020 2065 7870  ement>`,.    exp
-0000d040: 6f73 6564 206f 6e20 7468 6520 606f 6e53  osed on the `onS
-0000d050: 656c 6563 7460 2066 756e 6374 696f 6e2e  elect` function.
-0000d060: 0a0a 2020 2020 5365 6520 6050 7974 686f  ..    See `Pytho
-0000d070: 6e20 7474 6b2e 5472 6565 7669 6577 203c  n ttk.Treeview <
-0000d080: 746b 696e 7465 722e 7474 6b2e 5472 6565  tkinter.ttk.Tree
-0000d090: 7669 6577 3e60 2061 6e64 2060 6054 6b60  view>` and ``Tk`
-0000d0a0: 600a 2020 2020 6074 746b 2e54 7265 6576  `.    `ttk.Treev
-0000d0b0: 6965 7720 3c68 7474 7073 3a2f 2f74 636c  iew <https://tcl
-0000d0c0: 2e74 6b2f 6d61 6e2f 7463 6c38 2e36 2f54  .tk/man/tcl8.6/T
-0000d0d0: 6b43 6d64 2f74 746b 5f74 7265 6576 6965  kCmd/ttk_treevie
-0000d0e0: 772e 6874 6d3e 605f 0a20 2020 2064 6f63  w.htm>`_.    doc
-0000d0f0: 756d 656e 7461 7469 6f6e 2e0a 0a20 2020  umentation...   
-0000d100: 2041 7267 733a 0a20 2020 2020 2020 2076   Args:.        v
-0000d110: 6172 6961 626c 653a 2055 7365 2061 6e20  ariable: Use an 
-0000d120: 6578 7465 726e 616c 6c79 2064 6566 696e  externally defin
-0000d130: 6564 2076 6172 6961 626c 652c 2069 6e73  ed variable, ins
-0000d140: 7465 6164 206f 6620 6372 6561 7469 6e67  tead of creating
-0000d150: 2061 206e 6577 0a20 2020 2020 2020 2020   a new.         
-0000d160: 2020 206f 6e65 2073 7065 6369 6669 6320     one specific 
-0000d170: 666f 7220 7468 6973 2077 6964 6765 742e  for this widget.
-0000d180: 0a20 2020 2020 2020 206c 6162 656c 3a20  .        label: 
-0000d190: 5468 6520 6865 6164 696e 6720 7465 7874  The heading text
-0000d1a0: 2066 6f72 2074 6865 2066 6972 7374 2063   for the first c
-0000d1b0: 6f6c 756d 6e2c 2077 6869 6368 2069 6e63  olumn, which inc
-0000d1c0: 6c75 6465 7320 7468 6520 6c61 6265 6c73  ludes the labels
-0000d1d0: 2e0a 2020 2020 2020 2020 636f 6c75 6d6e  ..        column
-0000d1e0: 733a 204d 6170 7069 6e67 2062 6574 7765  s: Mapping betwe
-0000d1f0: 656e 2063 6f6c 756d 6e20 6964 656e 7469  en column identi
-0000d200: 6669 6572 7320 616e 6420 6974 7320 7469  fiers and its ti
-0000d210: 746c 6573 2e20 5375 7070 6f72 7473 0a20  tles. Supports. 
-0000d220: 2020 2020 2020 2020 2020 2061 6c73 6f20             also 
-0000d230: 6120 6469 7265 6374 206d 6170 2062 6574  a direct map bet
-0000d240: 7765 656e 2069 6465 6e74 6966 6965 7220  ween identifier 
-0000d250: 616e 6420 606d 6f64 656c 2e54 7265 6543  and `model.TreeC
-0000d260: 6f6c 756d 6e60 2e0a 2020 2020 2020 2020  olumn`..        
-0000d270: 7365 6c65 6374 6162 6c65 3a20 5368 6f75  selectable: Shou
-0000d280: 6c64 2074 6865 2075 7365 7220 6265 2061  ld the user be a
-0000d290: 626c 6520 746f 2073 656c 6563 7420 6f6e  ble to select on
-0000d2a0: 6520 6f66 2074 6865 2076 616c 7565 733f  e of the values?
-0000d2b0: 0a20 2020 2020 2020 2020 2020 2044 6566  .            Def
-0000d2c0: 6175 6c74 7320 746f 2060 4661 6c73 6560  aults to `False`
-0000d2d0: 2e0a 2020 2020 2020 2020 6f70 656e 6c65  ..        openle
-0000d2e0: 7665 6c3a 2054 6865 2068 6965 7261 7263  vel: The hierarc
-0000d2f0: 6879 206c 6576 656c 2074 6f20 6f70 656e  hy level to open
-0000d300: 2074 6865 2065 6c65 6d65 6e74 732e 2044   the elements. D
-0000d310: 6566 6175 6c74 7320 746f 2060 6031 6060  efaults to ``1``
-0000d320: 2c0a 2020 2020 2020 2020 2020 2020 6f6e  ,.            on
-0000d330: 6c79 2074 6865 2074 6f70 6c65 7665 6c20  ly the toplevel 
-0000d340: 656c 656d 656e 7473 2061 7265 206f 7065  elements are ope
-0000d350: 6e65 642e 0a20 2020 2020 2020 2020 2020  ned..           
-0000d360: 2053 6574 2074 6f20 6060 3060 6020 746f   Set to ``0`` to
-0000d370: 2063 6c6f 7365 2061 6c6c 2c20 616e 6420   close all, and 
-0000d380: 746f 2061 2072 6561 6c6c 7920 6269 6720  to a really big 
-0000d390: 6e75 6d62 6572 2074 6f20 6f70 656e 2061  number to open a
-0000d3a0: 6c6c 2e0a 2020 2020 2020 2020 6578 7061  ll..        expa
-0000d3b0: 6e64 3a20 4772 6f77 2074 6865 2077 6964  nd: Grow the wid
-0000d3c0: 6765 7420 746f 206d 6174 6368 2074 6865  get to match the
-0000d3d0: 2063 6f6e 7461 696e 6572 2067 7269 6420   container grid 
-0000d3e0: 7369 7a65 2e20 5468 6973 2069 730a 2020  size. This is.  
-0000d3f0: 2020 2020 2020 2020 2020 7573 7561 6c6c            usuall
-0000d400: 7920 7375 7070 6f72 7465 6420 666f 7220  y supported for 
-0000d410: 636f 6e74 6169 6e65 7273 2c20 6275 7420  containers, but 
-0000d420: 6974 2069 7320 696e 636c 7564 6564 2068  it is included h
-0000d430: 6572 652e 0a20 2020 2020 2020 2073 7479  ere..        sty
-0000d440: 6c65 3a20 436f 6e66 6967 7572 6520 7468  le: Configure th
-0000d450: 6520 7769 6467 6574 2073 7479 6c65 2e0a  e widget style..
-0000d460: 0a20 2020 2020 2020 2070 6172 656e 743a  .        parent:
-0000d470: 2054 6865 2070 6172 656e 7420 7769 6467   The parent widg
-0000d480: 6574 2e20 4361 6e20 6265 2061 2060 526f  et. Can be a `Ro
-0000d490: 6f74 5769 6e64 6f77 6020 6f72 2061 6e6f  otWindow` or ano
-0000d4a0: 7468 6572 2060 6d69 7869 6e2e 436f 6e74  ther `mixin.Cont
-0000d4b0: 6169 6e65 7257 6964 6765 7460 2e0a 0a20  ainerWidget`... 
-0000d4c0: 2020 2053 6565 2041 6c73 6f3a 0a20 2020     See Also:.   
-0000d4d0: 2020 2020 2060 4c69 7374 626f 7860 3a20       `Listbox`: 
-0000d4e0: 5369 6d70 6c69 6669 6564 2076 6572 7369  Simplified versi
-0000d4f0: 6f6e 206f 6620 7468 6973 0a20 2020 2027  on of this.    '
-0000d500: 2727 0a20 2020 2045 6c65 6d65 6e74 203d  ''.    Element =
-0000d510: 206d 6f64 656c 2e54 7265 6545 6c65 6d65   model.TreeEleme
-0000d520: 6e74 2020 2320 416c 6961 7320 7468 6520  nt  # Alias the 
-0000d530: 7472 6565 2065 6c65 6d65 6e74 2069 6e66  tree element inf
-0000d540: 6f72 6d61 7469 6f6e 2020 2320 544f 444f  ormation  # TODO
-0000d550: 3a20 4d6f 7665 2054 7265 6545 6c65 6d65  : Move TreeEleme
-0000d560: 6e74 2063 6c61 7373 2068 6572 653f 0a0a  nt class here?..
-0000d570: 2020 2020 4064 6174 6163 6c61 7373 0a20      @dataclass. 
-0000d580: 2020 2063 6c61 7373 2053 7479 6c65 286d     class Style(m
-0000d590: 6f64 656c 2e57 5374 796c 6529 3a0a 2020  odel.WStyle):.  
-0000d5a0: 2020 2020 2020 2727 2760 5472 6565 6020        '''`Tree` 
-0000d5b0: 7374 796c 6520 6f62 6a65 6374 2e0a 0a20  style object... 
-0000d5c0: 2020 2020 2020 2054 6865 7365 2061 7265         These are
-0000d5d0: 2074 6865 2073 7479 6c65 2063 6f6e 6669   the style confi
-0000d5e0: 6775 7261 7469 6f6e 733a 0a0a 2020 2020  gurations:..    
-0000d5f0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0000d600: 2020 2020 2020 7368 6f77 5f68 6561 6469        show_headi
-0000d610: 6e67 733a 2053 686f 7720 636f 6c75 6d6e  ngs: Show column
-0000d620: 2074 6974 6c65 2068 6561 6469 6e67 732e   title headings.
-0000d630: 0a20 2020 2020 2020 2020 2020 2073 686f  .            sho
-0000d640: 775f 6c61 6265 6c73 3a20 5368 6f77 2074  w_labels: Show t
-0000d650: 6865 2066 6972 7374 2063 6f6c 756d 6e2c  he first column,
-0000d660: 2077 6869 6368 2069 6e63 6c75 6465 7320   which includes 
-0000d670: 7468 6520 6c61 6265 6c73 2e0a 2020 2020  the labels..    
-0000d680: 2020 2020 2020 2020 616c 7462 673a 2053          altbg: S
-0000d690: 686f 7720 616c 7465 726e 6174 6520 6261  how alternate ba
-0000d6a0: 636b 6772 6f75 6e64 7320 666f 7220 6561  ckgrounds for ea
-0000d6b0: 6368 2072 6563 6f72 642e 0a20 2020 2020  ch record..     
-0000d6c0: 2020 2020 2020 2061 6c74 6267 5f73 696e         altbg_sin
-0000d6d0: 6465 783a 2060 6061 6c74 6267 6060 2069  dex: ``altbg`` i
-0000d6e0: 6e69 7469 616c 2061 6c74 6572 6e61 7465  nitial alternate
-0000d6f0: 2063 6f6c 6f75 7220 696e 6465 782e 0a0a   colour index...
-0000d700: 2020 2020 2020 2020 5468 6573 6520 6172          These ar
-0000d710: 6520 7468 6520 636f 6c6f 7572 733a 0a0a  e the colours:..
-0000d720: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-0000d730: 2020 2020 2020 2020 2020 636f 6c6f 7572            colour
-0000d740: 5f61 6c74 6267 3a20 6060 616c 7462 6760  _altbg: ``altbg`
-0000d750: 6020 616c 7465 726e 6174 6520 6c69 6e65  ` alternate line
-0000d760: 2063 6f6c 6f75 722e 0a20 2020 2020 2020   colour..       
-0000d770: 2020 2020 2020 2020 2055 7365 6420 6173           Used as
-0000d780: 2074 6865 2062 6163 6b67 726f 756e 6420   the background 
-0000d790: 636f 6c6f 7572 2e0a 2020 2020 2020 2020  colour..        
-0000d7a0: 2727 270a 2020 2020 2020 2020 7368 6f77  '''.        show
-0000d7b0: 5f68 6561 6469 6e67 733a 2062 6f6f 6c20  _headings: bool 
-0000d7c0: 3d20 5472 7565 0a20 2020 2020 2020 2073  = True.        s
-0000d7d0: 686f 775f 6c61 6265 6c73 3a20 626f 6f6c  how_labels: bool
-0000d7e0: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
-0000d7f0: 616c 7462 673a 2062 6f6f 6c20 3d20 5472  altbg: bool = Tr
-0000d800: 7565 0a20 2020 2020 2020 2061 6c74 6267  ue.        altbg
-0000d810: 5f73 696e 6465 783a 2074 7970 696e 672e  _sindex: typing.
-0000d820: 4c69 7465 7261 6c5b 302c 2031 5d20 3d20  Literal[0, 1] = 
-0000d830: 310a 2020 2020 2020 2020 2320 436f 6c6f  1.        # Colo
-0000d840: 7572 730a 2020 2020 2020 2020 636f 6c6f  urs.        colo
-0000d850: 7572 5f61 6c74 6267 3a20 7374 7220 3d20  ur_altbg: str = 
-0000d860: 276c 6967 6874 6772 6579 270a 0a20 2020  'lightgrey'..   
-0000d870: 2073 7461 7465 5f74 7970 6520 3d20 7661   state_type = va
-0000d880: 7254 7265 650a 2020 2020 5f5f 6c69 6e65  rTree.    __line
-0000d890: 735f 616c 743a 2073 7472 203d 2027 5f5f  s_alt: str = '__
-0000d8a0: 3a6c 696e 6573 2d61 6c74 270a 0a20 2020  :lines-alt'..   
-0000d8b0: 2077 636f 6c75 6d6e 733a 2074 7970 696e   wcolumns: typin
-0000d8c0: 672e 4d61 7070 696e 675b 7374 722c 206d  g.Mapping[str, m
-0000d8d0: 6f64 656c 2e54 7265 6543 6f6c 756d 6e5d  odel.TreeColumn]
-0000d8e0: 0a20 2020 2077 6461 7461 3a20 7479 7069  .    wdata: typi
-0000d8f0: 6e67 2e4d 7574 6162 6c65 4d61 7070 696e  ng.MutableMappin
-0000d900: 675b 7374 722c 2074 7970 696e 672e 416e  g[str, typing.An
-0000d910: 795d 0a0a 2020 2020 6465 6620 5f5f 696e  y]..    def __in
-0000d920: 6974 5f5f 2873 656c 662c 2070 6172 656e  it__(self, paren
-0000d930: 742c 202a 2c20 7661 7269 6162 6c65 3a20  t, *, variable: 
-0000d940: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-0000d950: 7661 7254 7265 655d 203d 204e 6f6e 652c  varTree] = None,
-0000d960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d970: 2020 6c61 6265 6c3a 2074 7970 696e 672e    label: typing.
-0000d980: 4f70 7469 6f6e 616c 5b73 7472 5d2c 0a20  Optional[str],. 
-0000d990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9a0: 636f 6c75 6d6e 733a 2074 7970 696e 672e  columns: typing.
-0000d9b0: 4d61 7070 696e 675b 7374 722c 2074 7970  Mapping[str, typ
-0000d9c0: 696e 672e 556e 696f 6e5b 6d6f 6465 6c2e  ing.Union[model.
-0000d9d0: 5472 6565 436f 6c75 6d6e 2c20 7374 725d  TreeColumn, str]
-0000d9e0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-0000d9f0: 2020 2020 7365 6c65 6374 6162 6c65 3a20      selectable: 
-0000da00: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
-0000da10: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-0000da20: 7065 6e6c 6576 656c 3a20 696e 7420 3d20  penlevel: int = 
-0000da30: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
-0000da40: 2020 2020 6578 7061 6e64 3a20 626f 6f6c      expand: bool
-0000da50: 203d 2054 7275 652c 0a20 2020 2020 2020   = True,.       
-0000da60: 2020 2020 2020 2020 2020 7374 796c 653a            style:
-0000da70: 2053 7479 6c65 203d 2053 7479 6c65 285f   Style = Style(_
-0000da80: 6465 6661 756c 743d 5472 7565 292c 0a20  default=True),. 
-0000da90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000daa0: 2a2a 6b77 6172 6773 293a 0a20 2020 2020  **kwargs):.     
-0000dab0: 2020 2073 656c 662e 7773 7479 6c65 203d     self.wstyle =
-0000dac0: 2073 7479 6c65 0a20 2020 2020 2020 2023   style.        #
-0000dad0: 2054 4f44 4f3a 2053 7570 706f 7274 3a0a   TODO: Support:.
-0000dae0: 2020 2020 2020 2020 2320 2d20 5365 7475          # - Setu
-0000daf0: 7020 7769 6467 6574 2063 6f6c 756d 6e20  p widget column 
-0000db00: 7365 7474 696e 6773 3f20 5365 6520 4c69  settings? See Li
-0000db10: 7374 626f 780a 2020 2020 2020 2020 7763  stbox.        wc
-0000db20: 6f6c 756d 6e73 203d 207b 7d0a 2020 2020  olumns = {}.    
-0000db30: 2020 2020 666f 7220 6369 642c 2063 6f62      for cid, cob
-0000db40: 6a20 696e 2063 6f6c 756d 6e73 2e69 7465  j in columns.ite
-0000db50: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
-0000db60: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-0000db70: 636f 626a 2c20 6d6f 6465 6c2e 5472 6565  cobj, model.Tree
-0000db80: 436f 6c75 6d6e 293a 0a20 2020 2020 2020  Column):.       
-0000db90: 2020 2020 2020 2020 2063 636f 6c20 3d20           ccol = 
-0000dba0: 636f 626a 0a20 2020 2020 2020 2020 2020  cobj.           
-0000dbb0: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
-0000dbc0: 2863 6f62 6a2c 2073 7472 293a 0a20 2020  (cobj, str):.   
-0000dbd0: 2020 2020 2020 2020 2020 2020 2063 636f               cco
-0000dbe0: 6c20 3d20 6d6f 6465 6c2e 5472 6565 436f  l = model.TreeCo
-0000dbf0: 6c75 6d6e 2863 6964 2c20 6e61 6d65 3d63  lumn(cid, name=c
-0000dc00: 6f62 6a29 0a20 2020 2020 2020 2020 2020  obj).           
-0000dc10: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000dc20: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-0000dc30: 7565 4572 726f 7228 6627 7b73 656c 6621  ueError(f'{self!
-0000dc40: 727d 3a20 496e 7661 6c69 6420 636f 6c75  r}: Invalid colu
-0000dc50: 6d6e 2022 7b63 6964 7d22 3a20 7b63 6f62  mn "{cid}": {cob
-0000dc60: 6a21 727d 2729 0a20 2020 2020 2020 2020  j!r}').         
-0000dc70: 2020 2077 636f 6c75 6d6e 735b 6369 645d     wcolumns[cid]
-0000dc80: 203d 2063 636f 6c0a 2020 2020 2020 2020   = ccol.        
-0000dc90: 7365 6c66 2e77 636f 6c75 6d6e 7320 3d20  self.wcolumns = 
-0000dca0: 7763 6f6c 756d 6e73 0a20 2020 2020 2020  wcolumns.       
-0000dcb0: 2077 7368 6f77 203d 205b 5d0a 2020 2020   wshow = [].    
-0000dcc0: 2020 2020 6966 2073 656c 662e 7773 7479      if self.wsty
-0000dcd0: 6c65 2e73 686f 775f 6865 6164 696e 6773  le.show_headings
-0000dce0: 3a0a 2020 2020 2020 2020 2020 2020 7773  :.            ws
-0000dcf0: 686f 772e 6170 7065 6e64 2827 6865 6164  how.append('head
-0000dd00: 696e 6773 2729 0a20 2020 2020 2020 2069  ings').        i
-0000dd10: 6620 7365 6c66 2e77 7374 796c 652e 7368  f self.wstyle.sh
-0000dd20: 6f77 5f6c 6162 656c 733a 0a20 2020 2020  ow_labels:.     
-0000dd30: 2020 2020 2020 2077 7368 6f77 2e61 7070         wshow.app
-0000dd40: 656e 6428 2774 7265 6527 290a 2020 2020  end('tree').    
-0000dd50: 2020 2020 2320 496e 6974 6961 6c69 7365      # Initialise
-0000dd60: 2056 6172 6961 626c 6520 616e 6420 4461   Variable and Da
-0000dd70: 7461 0a20 2020 2020 2020 2073 656c 662e  ta.        self.
-0000dd80: 696e 6974 5f73 696e 676c 6528 7661 7269  init_single(vari
-0000dd90: 6162 6c65 290a 2020 2020 2020 2020 6b77  able).        kw
-0000dda0: 6172 6773 2e75 7064 6174 6528 7b0a 2020  args.update({.  
-0000ddb0: 2020 2020 2020 2020 2020 2773 686f 7727            'show'
-0000ddc0: 3a20 7773 686f 772c 2020 2320 4f76 6572  : wshow,  # Over
-0000ddd0: 7269 6465 2074 6865 2067 6976 656e 2060  ride the given `
-0000dde0: 7368 6f77 6020 6172 6775 6d65 6e74 0a20  show` argument. 
-0000ddf0: 2020 2020 2020 2020 2020 2027 7365 6c65             'sele
-0000de00: 6374 6d6f 6465 273a 2074 6b2e 4252 4f57  ctmode': tk.BROW
-0000de10: 5345 2069 6620 7365 6c65 6374 6162 6c65  SE if selectable
-0000de20: 2065 6c73 6520 746b 2e4e 4f4e 452c 0a20   else tk.NONE,. 
-0000de30: 2020 2020 2020 2020 2020 2027 636f 6c75             'colu
-0000de40: 6d6e 7327 3a20 6c69 7374 2873 656c 662e  mns': list(self.
-0000de50: 7763 6f6c 756d 6e73 2e6b 6579 7328 2929  wcolumns.keys())
-0000de60: 2c0a 2020 2020 2020 2020 7d29 0a20 2020  ,.        }).   
-0000de70: 2020 2020 2073 7570 6572 2829 2e5f 5f69       super().__i
-0000de80: 6e69 745f 5f28 7061 7265 6e74 2c20 2a2a  nit__(parent, **
-0000de90: 6b77 6172 6773 290a 2020 2020 2020 2020  kwargs).        
-0000dea0: 7365 6c66 2e77 6461 7461 203d 207b 7d0a  self.wdata = {}.
-0000deb0: 2020 2020 2020 2020 2320 5365 6c65 6374          # Select
-0000dec0: 696f 6e0a 2020 2020 2020 2020 6966 2073  ion.        if s
-0000ded0: 656c 6563 7461 626c 653a 0a20 2020 2020  electable:.     
-0000dee0: 2020 2020 2020 2073 656c 662e 6269 6e64         self.bind
-0000def0: 696e 6728 273c 3c54 7265 6576 6965 7753  ing('<<TreeviewS
-0000df00: 656c 6563 743e 3e27 2c20 7365 6c66 2e5f  elect>>', self._
-0000df10: 6f6e 5365 6c65 6374 290a 2020 2020 2020  onSelect).      
-0000df20: 2020 2020 2020 2320 4469 7361 626c 6520        # Disable 
-0000df30: 446f 7562 6c65 2d43 6c69 636b 2065 7665  Double-Click eve
-0000df40: 6e74 2c20 7768 656e 2073 656c 6563 7461  nt, when selecta
-0000df50: 626c 650a 2020 2020 2020 2020 2020 2020  ble.            
-0000df60: 7365 6c66 2e62 696e 6469 6e67 2827 3c44  self.binding('<D
-0000df70: 6f75 626c 652d 4275 7474 6f6e 2d31 3e27  ouble-Button-1>'
-0000df80: 2c20 666e 2e62 696e 6469 6e67 5f64 6973  , fn.binding_dis
-0000df90: 6162 6c65 290a 2020 2020 2020 2020 2320  able).        # 
-0000dfa0: 4170 7065 6172 616e 6365 0a20 2020 2020  Appearance.     
-0000dfb0: 2020 2069 6620 6578 7061 6e64 3a0a 2020     if expand:.  
-0000dfc0: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
-0000dfd0: 7269 6428 7374 6963 6b79 3d74 6b2e 4e53  rid(sticky=tk.NS
-0000dfe0: 4557 290a 2020 2020 2020 2020 7365 6c66  EW).        self
-0000dff0: 2e6f 7065 6e6c 6576 656c 3a20 696e 7420  .openlevel: int 
-0000e000: 3d20 6f70 656e 6c65 7665 6c20 2023 2054  = openlevel  # T
-0000e010: 4f44 4f3a 2053 7570 706f 7274 206f 7065  ODO: Support ope
-0000e020: 6e69 6e67 2061 6c6c 206c 6576 656c 732c  ning all levels,
-0000e030: 2065 7870 6c69 6369 743f 0a20 2020 2020   explicit?.     
-0000e040: 2020 2023 2023 2048 6561 6465 7273 0a20     # # Headers. 
-0000e050: 2020 2020 2020 2069 6620 6c61 6265 6c20         if label 
-0000e060: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000e070: 2020 2020 2020 2020 2073 656c 662e 6865           self.he
-0000e080: 6164 696e 6728 2723 3027 2c20 7465 7874  ading('#0', text
-0000e090: 3d6c 6162 656c 290a 2020 2020 2020 2020  =label).        
-0000e0a0: 666f 7220 7763 6f6c 2069 6e20 7365 6c66  for wcol in self
-0000e0b0: 2e77 636f 6c75 6d6e 732e 7661 6c75 6573  .wcolumns.values
-0000e0c0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000e0d0: 7365 6c66 2e68 6561 6469 6e67 2877 636f  self.heading(wco
-0000e0e0: 6c2e 6964 656e 7469 6669 6572 2c20 7465  l.identifier, te
-0000e0f0: 7874 3d77 636f 6c2e 6e61 6d65 290a 2020  xt=wcol.name).  
-0000e100: 2020 2020 2020 2320 2320 416c 7465 726e        # # Altern
-0000e110: 6174 6520 4261 636b 6772 6f75 6e64 730a  ate Backgrounds.
-0000e120: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000e130: 7773 7479 6c65 2e61 6c74 6267 3a0a 2020  wstyle.altbg:.  
-0000e140: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-0000e150: 6167 5f63 6f6e 6669 6775 7265 2854 7265  ag_configure(Tre
-0000e160: 652e 5f5f 6c69 6e65 735f 616c 742c 2062  e.__lines_alt, b
-0000e170: 6163 6b67 726f 756e 643d 7365 6c66 2e77  ackground=self.w
-0000e180: 7374 796c 652e 636f 6c6f 7572 5f61 6c74  style.colour_alt
-0000e190: 6267 290a 2020 2020 2020 2020 2020 2020  bg).            
-0000e1a0: 2320 4d69 6e6f 7220 6973 7375 653a 2054  # Minor issue: T
-0000e1b0: 6865 7265 2069 7320 6120 6e65 6172 6c79  here is a nearly
-0000e1c0: 2069 6d70 6572 6365 7469 626c 6520 666c   impercetible fl
-0000e1d0: 6173 6820 6f66 2062 6164 6e65 7373 2077  ash of badness w
-0000e1e0: 6974 680a 2020 2020 2020 2020 2020 2020  ith.            
-0000e1f0: 2320 6054 696d 656f 7574 4964 6c65 6020  # `TimeoutIdle` 
-0000e200: 7468 6174 2064 6f65 736e 2774 2068 6170  that doesn't hap
-0000e210: 7065 6e20 7768 656e 2063 616c 6c69 6e67  pen when calling
-0000e220: 2074 6865 2066 756e 6374 696f 6e0a 2020   the function.  
-0000e230: 2020 2020 2020 2020 2020 2320 6469 7265            # dire
-0000e240: 6374 6c79 2e0a 2020 2020 2020 2020 2020  ctly..          
-0000e250: 2020 2320 506f 7373 6962 6c65 2066 6978    # Possible fix
-0000e260: 3a20 696e 2060 5f5f 7472 6565 5f6c 7376  : in `__tree_lsv
-0000e270: 6973 6962 6c65 602c 2070 6173 7320 616e  isible`, pass an
-0000e280: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-0000e290: 2020 2020 2020 2320 6073 656c 662e 666f        # `self.fo
-0000e2a0: 6375 7328 2960 2049 4420 2877 6865 6e20  cus()` ID (when 
-0000e2b0: 213d 2027 2729 2061 6e64 206f 7065 6e2f  != '') and open/
-0000e2c0: 636c 6f73 6520 7374 6174 652c 2074 6861  close state, tha
-0000e2d0: 740a 2020 2020 2020 2020 2020 2020 2320  t.            # 
-0000e2e0: 7265 706c 6163 6573 2060 776f 7065 6e60  replaces `wopen`
-0000e2f0: 2e0a 2020 2020 2020 2020 2020 2020 616c  ..            al
-0000e300: 7462 6720 3d20 7365 6c66 2e74 6964 6c65  tbg = self.tidle
-0000e310: 2873 656c 662e 5f5f 7472 6565 5f61 6c74  (self.__tree_alt
-0000e320: 6267 2c20 6b65 793d 2761 6c74 6267 2729  bg, key='altbg')
-0000e330: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000e340: 662e 6269 6e64 696e 6728 273c 3c54 7265  f.binding('<<Tre
-0000e350: 6576 6965 774f 7065 6e3e 3e27 2c20 616c  eviewOpen>>', al
-0000e360: 7462 672e 7265 7363 6865 6475 6c65 290a  tbg.reschedule).
-0000e370: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e380: 2e62 696e 6469 6e67 2827 3c3c 5472 6565  .binding('<<Tree
-0000e390: 7669 6577 436c 6f73 653e 3e27 2c20 616c  viewClose>>', al
-0000e3a0: 7462 672e 7265 7363 6865 6475 6c65 290a  tbg.reschedule).
-0000e3b0: 2020 2020 2020 2020 2320 5472 6163 6520          # Trace 
-0000e3c0: 7661 7269 6162 6c65 2073 7461 7465 0a20  variable state. 
-0000e3d0: 2020 2020 2020 2073 656c 662e 7472 6163         self.trac
-0000e3e0: 6528 7365 6c66 2e5f 5f74 7265 655f 7365  e(self.__tree_se
-0000e3f0: 742c 2074 7261 6365 5f6e 616d 653d 6627  t, trace_name=f'
-0000e400: 5f5f 3a7b 5f5f 6e61 6d65 5f5f 7d27 290a  __:{__name__}').
-0000e410: 0a20 2020 2064 6566 205f 7472 6565 5f67  .    def _tree_g
-0000e420: 6574 2873 656c 662c 2076 6172 6961 626c  et(self, variabl
-0000e430: 653a 2076 6172 2e56 6172 6961 626c 6529  e: var.Variable)
-0000e440: 202d 3e20 7479 7069 6e67 2e53 6571 7565   -> typing.Seque
-0000e450: 6e63 655b 6d6f 6465 6c2e 5472 6565 456c  nce[model.TreeEl
-0000e460: 656d 656e 745d 3a0a 2020 2020 2020 2020  ement]:.        
-0000e470: 2727 2747 656e 6572 6174 6520 6120 6076  '''Generate a `v
-0000e480: 6172 5472 6565 6020 6f62 6a65 6374 2c20  arTree` object, 
-0000e490: 6261 7365 6420 6f6e 2074 6865 2076 6172  based on the var
-0000e4a0: 6961 626c 652e 0a0a 2020 2020 2020 2020  iable...        
-0000e4b0: 5368 6f75 6c64 2062 6520 7265 696d 706c  Should be reimpl
-0000e4c0: 656d 656e 7465 6420 6279 2073 7562 636c  emented by subcl
-0000e4d0: 6173 7365 7320 7468 6174 2063 6861 6e67  asses that chang
-0000e4e0: 6520 7468 6520 7661 7269 6162 6c65 2074  e the variable t
-0000e4f0: 7970 652e 0a20 2020 2020 2020 2027 2727  ype..        '''
-0000e500: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-0000e510: 6973 696e 7374 616e 6365 2876 6172 6961  isinstance(varia
-0000e520: 626c 652c 2076 6172 5472 6565 290a 2020  ble, varTree).  
-0000e530: 2020 2020 2020 7265 7475 726e 2076 6172        return var
-0000e540: 6961 626c 652e 6765 7428 290a 0a20 2020  iable.get()..   
-0000e550: 2064 6566 205f 5f74 7265 655f 6c73 2873   def __tree_ls(s
-0000e560: 656c 662c 2070 6172 656e 743a 2074 7970  elf, parent: typ
-0000e570: 696e 672e 4f70 7469 6f6e 616c 5b73 7472  ing.Optional[str
-0000e580: 5d20 3d20 4e6f 6e65 2920 2d3e 2074 7970  ] = None) -> typ
-0000e590: 696e 672e 4974 6572 6162 6c65 5b73 7472  ing.Iterable[str
-0000e5a0: 5d3a 0a20 2020 2020 2020 2027 2727 4765  ]:.        '''Ge
-0000e5b0: 6e65 7261 7465 2061 206c 6973 7420 616c  nerate a list al
-0000e5c0: 6c20 7769 6467 6574 2069 6473 2c20 696e  l widget ids, in
-0000e5d0: 206c 696e 6561 7220 6f72 6465 722e 2727   linear order.''
-0000e5e0: 270a 2020 2020 2020 2020 666f 7220 7774  '.        for wt
-0000e5f0: 6f70 2069 6e20 7365 6c66 2e67 6574 5f63  op in self.get_c
-0000e600: 6869 6c64 7265 6e28 6974 656d 3d70 6172  hildren(item=par
-0000e610: 656e 7429 3a0a 2020 2020 2020 2020 2020  ent):.          
-0000e620: 2020 7969 656c 6420 7774 6f70 0a20 2020    yield wtop.   
-0000e630: 2020 2020 2020 2020 2079 6965 6c64 2066           yield f
-0000e640: 726f 6d20 7365 6c66 2e5f 5f74 7265 655f  rom self.__tree_
-0000e650: 6c73 2870 6172 656e 743d 7774 6f70 290a  ls(parent=wtop).
-0000e660: 0a20 2020 2064 6566 205f 5f74 7265 655f  .    def __tree_
-0000e670: 6c73 7669 7369 626c 6528 7365 6c66 2c20  lsvisible(self, 
-0000e680: 7061 7265 6e74 3a20 7479 7069 6e67 2e4f  parent: typing.O
-0000e690: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-0000e6a0: 6f6e 652c 205f 6b69 6473 3d4e 6f6e 6529  one, _kids=None)
-0000e6b0: 202d 3e20 7479 7069 6e67 2e49 7465 7261   -> typing.Itera
-0000e6c0: 626c 655b 7374 725d 3a0a 2020 2020 2020  ble[str]:.      
-0000e6d0: 2020 2727 2747 656e 6572 6174 6520 6120    '''Generate a 
-0000e6e0: 6c69 7374 206f 6620 616c 6c20 7669 7369  list of all visi
-0000e6f0: 626c 6520 7769 6467 6574 2069 6473 2c20  ble widget ids, 
-0000e700: 696e 2047 5549 206f 7264 6572 2e0a 0a20  in GUI order... 
-0000e710: 2020 2020 2020 2054 6869 7320 6775 6172         This guar
-0000e720: 616e 7465 6573 2074 6865 2079 6965 6c64  antees the yield
-0000e730: 6564 2076 616c 7565 7320 6172 6520 7669  ed values are vi
-0000e740: 7369 626c 6520 746f 2074 6865 2075 7365  sible to the use
-0000e750: 722c 2061 7320 6c6f 6e67 2061 730a 2020  r, as long as.  
-0000e760: 2020 2020 2020 7468 6520 7472 6565 2069        the tree i
-0000e770: 7320 7374 6162 6c65 2e0a 0a20 2020 2020  s stable...     
-0000e780: 2020 2053 6565 2041 6c73 6f3a 0a20 2020     See Also:.   
-0000e790: 2020 2020 2020 2020 2060 5f5f 7472 6565           `__tree
-0000e7a0: 5f6c 7360 3a20 5368 6f77 2061 6c6c 2077  _ls`: Show all w
-0000e7b0: 6964 6765 7473 2c20 6576 656e 2074 6865  idgets, even the
-0000e7c0: 206e 6f74 2063 7572 7265 6e74 6c79 2073   not currently s
-0000e7d0: 686f 776e 2e0a 0a20 2020 2020 2020 204e  hown...        N
-0000e7e0: 6f74 653a 0a20 2020 2020 2020 2020 2020  ote:.           
-0000e7f0: 2057 6865 6e20 6361 6c6c 6564 2064 6972   When called dir
-0000e800: 6563 746c 7920 6672 6f6d 2074 6865 2060  ectly from the `
-0000e810: 603c 3c54 7265 6576 6965 774f 7065 6e3e  `<<TreeviewOpen>
-0000e820: 3e60 6020 6f72 0a20 2020 2020 2020 2020  >`` or.         
-0000e830: 2020 2060 603c 3c54 7265 6576 6965 7743     ``<<TreeviewC
-0000e840: 6c6f 7365 3e3e 6060 2065 7665 6e74 2c20  lose>>`` event, 
-0000e850: 7468 6973 2077 696c 6c20 2266 6169 6c22  this will "fail"
-0000e860: 2c20 7468 6174 2065 7665 6e74 2072 756e  , that event run
-0000e870: 7320 746f 6f0a 2020 2020 2020 2020 2020  s too.          
-0000e880: 2020 6561 726c 792e 2055 7365 2061 2060    early. Use a `
-0000e890: 6d6f 6465 6c2e 5469 6d65 6f75 7449 646c  model.TimeoutIdl
-0000e8a0: 6560 2069 6e20 7468 6572 6520 746f 2067  e` in there to g
-0000e8b0: 6574 2074 6865 2063 6f72 7265 6374 0a20  et the correct. 
-0000e8c0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0000e8d0: 7473 2e0a 2020 2020 2020 2020 2727 270a  ts..        '''.
-0000e8e0: 2020 2020 2020 2020 666f 7220 7774 6f70          for wtop
-0000e8f0: 2069 6e20 5f6b 6964 7320 6f72 2073 656c   in _kids or sel
-0000e900: 662e 6765 745f 6368 696c 6472 656e 2869  f.get_children(i
-0000e910: 7465 6d3d 7061 7265 6e74 293a 0a20 2020  tem=parent):.   
-0000e920: 2020 2020 2020 2020 2079 6965 6c64 2077           yield w
-0000e930: 746f 700a 2020 2020 2020 2020 2020 2020  top.            
-0000e940: 776f 7065 6e20 3d20 7365 6c66 2e69 7465  wopen = self.ite
-0000e950: 6d28 7774 6f70 2c20 6f70 7469 6f6e 3d27  m(wtop, option='
-0000e960: 6f70 656e 2729 203d 3d20 310a 2020 2020  open') == 1.    
-0000e970: 2020 2020 2020 2020 776b 6964 7320 3d20          wkids = 
-0000e980: 7365 6c66 2e67 6574 5f63 6869 6c64 7265  self.get_childre
-0000e990: 6e28 6974 656d 3d77 746f 7029 0a20 2020  n(item=wtop).   
-0000e9a0: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
-0000e9b0: 776b 6964 7329 203e 2030 2061 6e64 2077  wkids) > 0 and w
-0000e9c0: 6f70 656e 3a0a 2020 2020 2020 2020 2020  open:.          
-0000e9d0: 2020 2020 2020 7969 656c 6420 6672 6f6d        yield from
-0000e9e0: 2073 656c 662e 5f5f 7472 6565 5f6c 7376   self.__tree_lsv
-0000e9f0: 6973 6962 6c65 2870 6172 656e 743d 7774  isible(parent=wt
-0000ea00: 6f70 2c20 5f6b 6964 733d 776b 6964 7329  op, _kids=wkids)
-0000ea10: 0a0a 2020 2020 6465 6620 5f5f 7472 6565  ..    def __tree
-0000ea20: 5f63 6c65 616e 2873 656c 662c 2070 6172  _clean(self, par
-0000ea30: 656e 743d 4e6f 6e65 2920 2d3e 204e 6f6e  ent=None) -> Non
-0000ea40: 653a 0a20 2020 2020 2020 2073 656c 662e  e:.        self.
-0000ea50: 6465 6c65 7465 282a 7365 6c66 2e5f 5f74  delete(*self.__t
-0000ea60: 7265 655f 6c73 2870 6172 656e 743d 7061  ree_ls(parent=pa
-0000ea70: 7265 6e74 2929 0a20 2020 2020 2020 2073  rent)).        s
-0000ea80: 656c 662e 7764 6174 612e 636c 6561 7228  elf.wdata.clear(
-0000ea90: 290a 0a20 2020 2064 6566 205f 5f74 7265  )..    def __tre
-0000eaa0: 655f 7075 7428 7365 6c66 2c20 656c 656d  e_put(self, elem
-0000eab0: 656e 7473 3a20 7479 7069 6e67 2e53 6571  ents: typing.Seq
-0000eac0: 7565 6e63 655b 6d6f 6465 6c2e 5472 6565  uence[model.Tree
-0000ead0: 456c 656d 656e 745d 2c20 2a2c 0a20 2020  Element], *,.   
-0000eae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eaf0: 7061 7265 6e74 3a20 7479 7069 6e67 2e4f  parent: typing.O
-0000eb00: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-0000eb10: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-0000eb20: 2020 2020 2020 2020 6f70 656e 6c65 7665          openleve
-0000eb30: 6c3a 2074 7970 696e 672e 4f70 7469 6f6e  l: typing.Option
-0000eb40: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 2c20  al[int] = None, 
-0000eb50: 5f6c 6576 656c 3a20 696e 7420 3d20 3029  _level: int = 0)
-0000eb60: 3a0a 2020 2020 2020 2020 7061 7265 6e74  :.        parent
-0000eb70: 5f6c 6f63 3a20 7479 7069 6e67 2e4f 7074  _loc: typing.Opt
-0000eb80: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-0000eb90: 6520 6966 2070 6172 656e 7420 6973 204e  e if parent is N
-0000eba0: 6f6e 6520 656c 7365 2073 656c 662e 696e  one else self.in
-0000ebb0: 6465 7828 7061 7265 6e74 290a 2020 2020  dex(parent).    
-0000ebc0: 2020 2020 6f70 656e 6c65 7665 6c20 3d20      openlevel = 
-0000ebd0: 6f70 656e 6c65 7665 6c20 6f72 2073 656c  openlevel or sel
-0000ebe0: 662e 6f70 656e 6c65 7665 6c0a 2020 2020  f.openlevel.    
-0000ebf0: 2020 2020 666f 7220 6569 642c 2065 6c65      for eid, ele
-0000ec00: 6d65 6e74 2069 6e20 656e 756d 6572 6174  ment in enumerat
-0000ec10: 6528 656c 656d 656e 7473 293a 0a20 2020  e(elements):.   
-0000ec20: 2020 2020 2020 2020 2023 2069 6620 5f5f           # if __
-0000ec30: 6465 6275 675f 5f3a 0a20 2020 2020 2020  debug__:.       
-0000ec40: 2020 2020 2023 2020 2020 2074 706c 5f74       #     tpl_t
-0000ec50: 6578 7420 3d20 6627 7b70 6172 656e 7420  ext = f'{parent 
-0000ec60: 6f72 2022 5f5f 746f 705f 5f22 7d3a 3a23  or "__top__"}::#
-0000ec70: 7b65 6964 7d27 0a20 2020 2020 2020 2020  {eid}'.         
-0000ec80: 2020 2023 2020 2020 206c 6f67 6765 722e     #     logger.
-0000ec90: 6465 6275 6728 6627 7b22 3e22 202a 2028  debug(f'{">" * (
-0000eca0: 5f6c 6576 656c 202b 2031 297d 207b 7470  _level + 1)} {tp
-0000ecb0: 6c5f 7465 7874 7d3a 204c 3a22 7b65 6c65  l_text}: L:"{ele
-0000ecc0: 6d65 6e74 2e6c 6162 656c 7d22 2043 3a7c  ment.label}" C:|
-0000ecd0: 7b22 2022 2e6a 6f69 6e28 656c 656d 656e  {" ".join(elemen
-0000ece0: 742e 636f 6c75 6d6e 7329 7d7c 2729 0a20  t.columns)}|'). 
-0000ecf0: 2020 2020 2020 2020 2020 2069 6620 656c             if el
-0000ed00: 656d 656e 742e 636f 6c75 6d6e 7320 6973  ement.columns is
-0000ed10: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000ed20: 2020 2020 2020 2020 2020 2023 2054 4f44             # TOD
-0000ed30: 4f3a 2053 7570 706f 7274 2061 2064 6963  O: Support a dic
-0000ed40: 7420 7769 7468 206b 6579 7320 636f 7272  t with keys corr
-0000ed50: 6573 706f 6e64 696e 6720 746f 2074 6865  esponding to the
-0000ed60: 2060 7365 6c66 2e77 636f 6c75 6d6e 7360   `self.wcolumns`
-0000ed70: 2c20 706f 7373 6962 6c65 2073 7562 7365  , possible subse
-0000ed80: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
-0000ed90: 2020 6173 7365 7274 206c 656e 2865 6c65    assert len(ele
-0000eda0: 6d65 6e74 2e63 6f6c 756d 6e73 2920 3d3d  ment.columns) ==
-0000edb0: 206c 656e 2873 656c 662e 7763 6f6c 756d   len(self.wcolum
-0000edc0: 6e73 292c 2066 2749 6e76 616c 6964 2043  ns), f'Invalid C
-0000edd0: 6f6c 756d 6e20 237b 6569 647d 3a20 5369  olumn #{eid}: Si
-0000ede0: 7a65 3a20 457b 6c65 6e28 656c 656d 656e  ze: E{len(elemen
-0000edf0: 742e 636f 6c75 6d6e 7329 7d20 577b 6c65  t.columns)} W{le
-0000ee00: 6e28 7365 6c66 2e77 636f 6c75 6d6e 7329  n(self.wcolumns)
-0000ee10: 7d27 0a20 2020 2020 2020 2020 2020 2063  }'.            c
-0000ee20: 6869 6c64 5f6c 6f63 3a20 7479 7069 6e67  hild_loc: typing
-0000ee30: 2e55 6e69 6f6e 5b69 6e74 2c20 7479 7069  .Union[int, typi
-0000ee40: 6e67 2e4c 6974 6572 616c 5b27 656e 6427  ng.Literal['end'
-0000ee50: 5d5d 0a20 2020 2020 2020 2020 2020 2069  ]].            i
-0000ee60: 6620 7061 7265 6e74 5f6c 6f63 2069 7320  f parent_loc is 
-0000ee70: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000ee80: 2020 2020 2020 6368 696c 645f 6c6f 6320        child_loc 
-0000ee90: 3d20 746b 2e45 4e44 0a20 2020 2020 2020  = tk.END.       
-0000eea0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000eeb0: 2020 2020 2020 2020 2020 2063 6869 6c64             child
-0000eec0: 5f6c 6f63 203d 2070 6172 656e 745f 6c6f  _loc = parent_lo
-0000eed0: 6320 2b20 6569 640a 2020 2020 2020 2020  c + eid.        
-0000eee0: 2020 2020 6369 6420 3d20 7365 6c66 2e69      cid = self.i
-0000eef0: 6e73 6572 7428 7061 7265 6e74 206f 7220  nsert(parent or 
-0000ef00: 2727 2c20 6368 696c 645f 6c6f 632c 0a20  '', child_loc,. 
-0000ef10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef20: 2020 2020 2020 2020 2020 2020 2074 6578               tex
-0000ef30: 743d 656c 656d 656e 742e 6c61 6265 6c2c  t=element.label,
-0000ef40: 2076 616c 7565 733d 7475 706c 6528 656c   values=tuple(el
-0000ef50: 656d 656e 742e 636f 6c75 6d6e 7320 6f72  ement.columns or
-0000ef60: 205b 5d29 2c0a 2020 2020 2020 2020 2020   []),.          
-0000ef70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef80: 2020 2020 6f70 656e 3d5f 6c65 7665 6c20      open=_level 
-0000ef90: 3c20 6f70 656e 6c65 7665 6c2c 0a20 2020  < openlevel,.   
-0000efa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000efb0: 2020 2020 2020 2020 2020 2069 6d61 6765             image
-0000efc0: 3d65 6c65 6d65 6e74 2e69 6d61 6765 206f  =element.image o
-0000efd0: 7220 2727 2c0a 2020 2020 2020 2020 2020  r '',.          
-0000efe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eff0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0000f000: 2020 7365 6c66 2e77 6461 7461 5b63 6964    self.wdata[cid
-0000f010: 5d20 3d20 656c 656d 656e 742e 6461 7461  ] = element.data
-0000f020: 0a20 2020 2020 2020 2020 2020 2023 2069  .            # i
-0000f030: 6620 5f5f 6465 6275 675f 5f3a 0a20 2020  f __debug__:.   
-0000f040: 2020 2020 2020 2020 2023 2020 2020 206c           #     l
-0000f050: 6f67 6765 722e 6465 6275 6728 6627 7b22  ogger.debug(f'{"
-0000f060: 7c22 202a 2028 5f6c 6576 656c 202b 2031  |" * (_level + 1
-0000f070: 297d 2049 443a 207b 6369 647d 2729 0a20  )} ID: {cid}'). 
-0000f080: 2020 2020 2020 2020 2020 2069 6620 656c             if el
-0000f090: 656d 656e 742e 6368 696c 6472 656e 3a0a  ement.children:.
-0000f0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f0b0: 2320 6966 205f 5f64 6562 7567 5f5f 3a0a  # if __debug__:.
-0000f0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f0d0: 2320 2020 2020 6c6f 6767 6572 2e64 6562  #     logger.deb
-0000f0e0: 7567 2866 277b 227c 2220 2a20 285f 6c65  ug(f'{"|" * (_le
-0000f0f0: 7665 6c20 2b20 3129 7d20 4368 696c 6472  vel + 1)} Childr
-0000f100: 656e 3a20 7b6c 656e 2865 6c65 6d65 6e74  en: {len(element
-0000f110: 2e63 6869 6c64 7265 6e29 7d27 290a 2020  .children)}').  
-0000f120: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000f130: 6c66 2e5f 5f74 7265 655f 7075 7428 656c  lf.__tree_put(el
-0000f140: 656d 656e 742e 6368 696c 6472 656e 2c0a  ement.children,.
-0000f150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f170: 7061 7265 6e74 3d63 6964 2c0a 2020 2020  parent=cid,.    
-0000f180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f190: 2020 2020 2020 2020 2020 2020 6f70 656e              open
-0000f1a0: 6c65 7665 6c3d 6f70 656e 6c65 7665 6c2c  level=openlevel,
-0000f1b0: 205f 6c65 7665 6c3d 5f6c 6576 656c 202b   _level=_level +
-0000f1c0: 2031 290a 0a20 2020 2064 6566 205f 5f74   1)..    def __t
-0000f1d0: 7265 655f 7365 7428 7365 6c66 2c20 2a61  ree_set(self, *a
-0000f1e0: 7267 732c 202a 2a6b 7761 7267 7329 202d  rgs, **kwargs) -
-0000f1f0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-0000f200: 6173 7365 7274 2073 656c 662e 7661 7269  assert self.vari
-0000f210: 6162 6c65 2069 7320 6e6f 7420 4e6f 6e65  able is not None
-0000f220: 2c20 6627 7b73 656c 6621 727d 3a20 4d69  , f'{self!r}: Mi
-0000f230: 7373 696e 6720 7661 7269 6162 6c65 270a  ssing variable'.
-0000f240: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
-0000f250: 7365 6c66 2e5f 7472 6565 5f67 6574 2873  self._tree_get(s
-0000f260: 656c 662e 7661 7269 6162 6c65 290a 2020  elf.variable).  
-0000f270: 2020 2020 2020 7365 6c66 2e5f 5f74 7265        self.__tre
-0000f280: 655f 636c 6561 6e28 290a 2020 2020 2020  e_clean().      
-0000f290: 2020 7365 6c66 2e5f 5f74 7265 655f 7075    self.__tree_pu
-0000f2a0: 7428 7661 6c75 6529 0a20 2020 2020 2020  t(value).       
-0000f2b0: 2069 6620 7365 6c66 2e77 7374 796c 652e   if self.wstyle.
-0000f2c0: 616c 7462 673a 0a20 2020 2020 2020 2020  altbg:.         
-0000f2d0: 2020 2073 656c 662e 5f74 6964 6c65 735b     self._tidles[
-0000f2e0: 2761 6c74 6267 275d 2e73 6368 6564 756c  'altbg'].schedul
-0000f2f0: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
-0000f300: 2e5f 7472 6565 5f6f 6e73 6574 2876 616c  ._tree_onset(val
-0000f310: 7565 290a 0a20 2020 2064 6566 205f 5f74  ue)..    def __t
-0000f320: 7265 655f 616c 7462 6728 7365 6c66 2c20  ree_altbg(self, 
-0000f330: 2a2c 2072 656d 6f76 653a 2062 6f6f 6c20  *, remove: bool 
-0000f340: 3d20 4661 6c73 6529 202d 3e20 4e6f 6e65  = False) -> None
-0000f350: 3a0a 2020 2020 2020 2020 2727 2753 6574  :.        '''Set
-0000f360: 7570 2074 6865 2061 6c74 6572 6e61 7465  up the alternate
-0000f370: 2062 6163 6b67 726f 756e 642c 2062 6173   background, bas
-0000f380: 6564 206f 6e20 7461 6773 2e0a 0a20 2020  ed on tags...   
-0000f390: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-0000f3a0: 2020 2020 2020 2072 656d 6f76 653a 2046         remove: F
-0000f3b0: 6f72 6365 2072 656d 6f76 696e 6720 616c  orce removing al
-0000f3c0: 6c20 7468 6520 6261 636b 6772 6f75 6e64  l the background
-0000f3d0: 730a 2020 2020 2020 2020 2727 270a 2020  s.        '''.  
-0000f3e0: 2020 2020 2020 746e 616d 6520 3d20 5472        tname = Tr
-0000f3f0: 6565 2e5f 5f6c 696e 6573 5f61 6c74 0a20  ee.__lines_alt. 
-0000f400: 2020 2020 2020 2069 6e64 6578 3a20 696e         index: in
-0000f410: 7420 3d20 7365 6c66 2e77 7374 796c 652e  t = self.wstyle.
-0000f420: 616c 7462 675f 7369 6e64 6578 0a20 2020  altbg_sindex.   
-0000f430: 2020 2020 2066 6f72 2072 6964 2069 6e20       for rid in 
-0000f440: 7365 6c66 2e5f 5f74 7265 655f 6c73 7669  self.__tree_lsvi
-0000f450: 7369 626c 6528 293a 0a20 2020 2020 2020  sible():.       
-0000f460: 2020 2020 2074 6167 7320 3d20 7365 7428       tags = set(
-0000f470: 7365 6c66 2e69 7465 6d28 7269 642c 206f  self.item(rid, o
-0000f480: 7074 696f 6e3d 2774 6167 7327 2929 0a20  ption='tags')). 
-0000f490: 2020 2020 2020 2020 2020 2064 6f74 6167             dotag
-0000f4a0: 7320 3d20 4661 6c73 650a 2020 2020 2020  s = False.      
-0000f4b0: 2020 2020 2020 6966 206e 6f74 2072 656d        if not rem
-0000f4c0: 6f76 6520 616e 6420 696e 6465 7820 2520  ove and index % 
-0000f4d0: 3220 3d3d 2030 3a0a 2020 2020 2020 2020  2 == 0:.        
-0000f4e0: 2020 2020 2020 2020 6966 2074 6e61 6d65          if tname
-0000f4f0: 206e 6f74 2069 6e20 7461 6773 3a0a 2020   not in tags:.  
-0000f500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f510: 2020 7461 6773 2e61 6464 2874 6e61 6d65    tags.add(tname
-0000f520: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000f530: 2020 2020 2020 646f 7461 6773 203d 2054        dotags = T
-0000f540: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
-0000f550: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000f560: 2020 2020 2020 6966 2074 6e61 6d65 2069        if tname i
-0000f570: 6e20 7461 6773 3a0a 2020 2020 2020 2020  n tags:.        
-0000f580: 2020 2020 2020 2020 2020 2020 7461 6773              tags
-0000f590: 2e72 656d 6f76 6528 746e 616d 6529 0a20  .remove(tname). 
-0000f5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f5b0: 2020 2064 6f74 6167 7320 3d20 5472 7565     dotags = True
-0000f5c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000f5d0: 646f 7461 6773 3a0a 2020 2020 2020 2020  dotags:.        
-0000f5e0: 2020 2020 2020 2020 7365 6c66 2e69 7465          self.ite
-0000f5f0: 6d28 7269 642c 2074 6167 733d 6c69 7374  m(rid, tags=list
-0000f600: 2874 6167 7329 290a 2020 2020 2020 2020  (tags)).        
-0000f610: 2020 2020 696e 6465 7820 2b3d 2031 0a20      index += 1. 
-0000f620: 2020 2020 2020 2023 2069 6620 5f5f 6465         # if __de
-0000f630: 6275 675f 5f3a 0a20 2020 2020 2020 2023  bug__:.        #
-0000f640: 2020 2020 2023 2054 6869 7320 7368 6f75       # This shou
-0000f650: 6c64 2072 756e 206f 6e6c 7920 6f6e 6365  ld run only once
-0000f660: 2c20 6576 656e 2077 6974 6820 6d75 6c74  , even with mult
-0000f670: 6970 6c65 2063 6861 6e67 6573 0a20 2020  iple changes.   
-0000f680: 2020 2020 2023 2020 2020 2069 6620 696e       #     if in
-0000f690: 6465 7820 3e20 7365 6c66 2e77 7374 796c  dex > self.wstyl
-0000f6a0: 652e 616c 7462 675f 7369 6e64 6578 3a0a  e.altbg_sindex:.
-0000f6b0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0000f6c0: 2020 6c6f 6767 6572 2e64 6562 7567 2866    logger.debug(f
-0000f6d0: 277b 7365 6c66 7d3a 2043 616c 6375 6c61  '{self}: Calcula
-0000f6e0: 7465 6420 416c 7442 4727 290a 0a20 2020  ted AltBG')..   
-0000f6f0: 2064 6566 2077 7369 6428 7365 6c66 2920   def wsid(self) 
-0000f700: 2d3e 2074 7970 696e 672e 4f70 7469 6f6e  -> typing.Option
-0000f710: 616c 5b73 7472 5d3a 0a20 2020 2020 2020  al[str]:.       
-0000f720: 2027 2727 4765 7420 7468 6520 7365 6c65   '''Get the sele
-0000f730: 6374 6564 2065 6c65 6d65 6e74 2069 6465  cted element ide
-0000f740: 6e74 6966 6965 722e 0a0a 2020 2020 2020  ntifier...      
-0000f750: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-0000f760: 2020 2020 2020 2060 456c 656d 656e 7420         `Element 
-0000f770: 3c6d 6f64 656c 2e54 7265 6545 6c65 6d65  <model.TreeEleme
-0000f780: 6e74 3e60 2069 642c 206f 7220 604e 6f6e  nt>` id, or `Non
-0000f790: 6560 2077 6865 6e20 6e6f 7468 696e 6720  e` when nothing 
-0000f7a0: 6973 2073 656c 6563 7465 642e 0a0a 2020  is selected...  
-0000f7b0: 2020 2020 2020 2020 2020 4966 2074 6865            If the
-0000f7c0: 2077 6964 6765 7420 7761 7320 6372 6561   widget was crea
-0000f7d0: 7465 6420 7769 7468 6f75 7420 7468 6520  ted without the 
-0000f7e0: 6060 7365 6c65 6374 6162 6c65 6060 2066  ``selectable`` f
-0000f7f0: 6c61 672c 2074 6869 7320 616c 7761 7973  lag, this always
-0000f800: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000f810: 7572 6e73 2060 4e6f 6e65 602e 0a20 2020  urns `None`..   
-0000f820: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-0000f830: 2073 656c 6563 7469 6f6e 203d 2073 656c   selection = sel
-0000f840: 662e 7365 6c65 6374 696f 6e28 290a 2020  f.selection().  
-0000f850: 2020 2020 2020 6966 205f 5f64 6562 7567        if __debug
-0000f860: 5f5f 3a0a 2020 2020 2020 2020 2020 2020  __:.            
-0000f870: 7365 6c65 6374 6d6f 6465 203d 2073 7472  selectmode = str
-0000f880: 2873 656c 665b 2773 656c 6563 746d 6f64  (self['selectmod
-0000f890: 6527 5d29 0a20 2020 2020 2020 2020 2020  e']).           
-0000f8a0: 2061 7373 6572 7420 7365 6c65 6374 6d6f   assert selectmo
-0000f8b0: 6465 2069 6e20 5b74 6b2e 4252 4f57 5345  de in [tk.BROWSE
-0000f8c0: 2c20 746b 2e4e 4f4e 455d 2c20 6627 7b73  , tk.NONE], f'{s
-0000f8d0: 656c 6621 727d 3a20 496e 7661 6c69 6420  elf!r}: Invalid 
-0000f8e0: 5365 6c65 6374 696f 6e20 4d6f 6465 3a20  Selection Mode: 
-0000f8f0: 7b73 656c 6563 746d 6f64 657d 270a 2020  {selectmode}'.  
-0000f900: 2020 2020 2020 2020 2020 2320 6c6f 6767            # logg
-0000f910: 6572 2e64 6562 7567 2827 5365 6c65 6374  er.debug('Select
-0000f920: 696f 6e3a 2025 7227 2c20 7365 6c65 6374  ion: %r', select
-0000f930: 696f 6e29 0a20 2020 2020 2020 2069 6620  ion).        if 
-0000f940: 6c65 6e28 7365 6c65 6374 696f 6e29 203d  len(selection) =
-0000f950: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-0000f960: 2023 2053 6b69 7020 756e 2d73 656c 6563   # Skip un-selec
-0000f970: 7469 6f6e 730a 2020 2020 2020 2020 2020  tions.          
-0000f980: 2020 2320 5573 7561 6c6c 7920 7468 6520    # Usually the 
-0000f990: 5472 6565 2063 6f6e 7465 6e74 7320 6368  Tree contents ch
-0000f9a0: 616e 6765 642e 2e2e 0a20 2020 2020 2020  anged....       
-0000f9b0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
-0000f9c0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-0000f9d0: 2020 2020 2020 2020 2020 2023 2052 6567             # Reg
-0000f9e0: 756c 6172 2053 656c 6563 7469 6f6e 0a20  ular Selection. 
-0000f9f0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-0000fa00: 7420 6c65 6e28 7365 6c65 6374 696f 6e29  t len(selection)
-0000fa10: 203d 3d20 312c 2066 277b 7365 6c66 2172   == 1, f'{self!r
-0000fa20: 7d3a 2049 6e76 616c 6964 2073 656c 6563  }: Invalid selec
-0000fa30: 7469 6f6e 206d 6f64 6527 0a20 2020 2020  tion mode'.     
-0000fa40: 2020 2020 2020 2074 7265 6569 6420 3d20         treeid = 
-0000fa50: 7365 6c65 6374 696f 6e5b 305d 0a20 2020  selection[0].   
-0000fa60: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000fa70: 7472 6565 6964 0a0a 2020 2020 6465 6620  treeid..    def 
-0000fa80: 7773 656c 6563 7469 6f6e 2873 656c 6629  wselection(self)
-0000fa90: 202d 3e20 7479 7069 6e67 2e4f 7074 696f   -> typing.Optio
-0000faa0: 6e61 6c5b 7479 7069 6e67 2e41 6e79 5d3a  nal[typing.Any]:
-0000fab0: 0a20 2020 2020 2020 2027 2727 4765 7420  .        '''Get 
-0000fac0: 7468 6520 7365 6c65 6374 6564 2064 6174  the selected dat
-0000fad0: 612e 0a0a 2020 2020 2020 2020 5265 7475  a...        Retu
-0000fae0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-0000faf0: 2053 696e 6365 2074 6869 7320 7375 7070   Since this supp
-0000fb00: 6f72 7473 206f 6e6c 7920 6120 7369 6e67  orts only a sing
-0000fb10: 6c65 2073 656c 6563 7469 6f6e 2c20 7265  le selection, re
-0000fb20: 7475 726e 2074 6865 2073 656c 6563 7465  turn the selecte
-0000fb30: 640a 2020 2020 2020 2020 2020 2020 7661  d.            va
-0000fb40: 6c75 652c 206f 7220 6060 4e6f 6e65 6060  lue, or ``None``
-0000fb50: 2077 6865 6e20 6e6f 7468 696e 6720 6973   when nothing is
-0000fb60: 2073 656c 6563 7465 642e 0a0a 2020 2020   selected...    
-0000fb70: 2020 2020 2020 2020 4966 2074 6865 2077          If the w
-0000fb80: 6964 6765 7420 7761 7320 6372 6561 7465  idget was create
-0000fb90: 6420 7769 7468 6f75 7420 7468 6520 6060  d without the ``
-0000fba0: 7365 6c65 6374 6162 6c65 6060 2066 6c61  selectable`` fla
-0000fbb0: 672c 2074 6869 7320 616c 7761 7973 0a20  g, this always. 
-0000fbc0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000fbd0: 6e73 2060 4e6f 6e65 602e 0a20 2020 2020  ns `None`..     
-0000fbe0: 2020 2027 2727 0a20 2020 2020 2020 2077     '''.        w
-0000fbf0: 7369 6420 3d20 7365 6c66 2e77 7369 6428  sid = self.wsid(
-0000fc00: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0000fc10: 2073 656c 662e 7764 6174 615b 7773 6964   self.wdata[wsid
-0000fc20: 5d20 6966 2077 7369 6420 656c 7365 204e  ] if wsid else N
-0000fc30: 6f6e 650a 0a20 2020 2064 6566 205f 6f6e  one..    def _on
-0000fc40: 5365 6c65 6374 2873 656c 662c 2065 7665  Select(self, eve
-0000fc50: 6e74 3d4e 6f6e 6529 3a0a 2020 2020 2020  nt=None):.      
-0000fc60: 2020 2727 2727 2727 2020 2320 496e 7465    ''''''  # Inte
-0000fc70: 726e 616c 2c20 646f 206e 6f74 2064 6f63  rnal, do not doc
-0000fc80: 756d 656e 740a 2020 2020 2020 2020 7365  ument.        se
-0000fc90: 6c65 6374 696f 6e3a 2074 7570 6c65 203d  lection: tuple =
-0000fca0: 2073 656c 662e 7365 6c65 6374 696f 6e28   self.selection(
-0000fcb0: 290a 2020 2020 2020 2020 6966 205f 5f64  ).        if __d
-0000fcc0: 6562 7567 5f5f 3a0a 2020 2020 2020 2020  ebug__:.        
-0000fcd0: 2020 2020 7365 6c65 6374 6d6f 6465 203d      selectmode =
-0000fce0: 2073 7472 2873 656c 665b 2773 656c 6563   str(self['selec
-0000fcf0: 746d 6f64 6527 5d29 0a20 2020 2020 2020  tmode']).       
-0000fd00: 2020 2020 2061 7373 6572 7420 7365 6c65       assert sele
-0000fd10: 6374 6d6f 6465 2069 6e20 5b74 6b2e 4252  ctmode in [tk.BR
-0000fd20: 4f57 5345 2c20 746b 2e4e 4f4e 455d 2c20  OWSE, tk.NONE], 
-0000fd30: 6627 7b73 656c 6621 727d 3a20 496e 7661  f'{self!r}: Inva
-0000fd40: 6c69 6420 5365 6c65 6374 696f 6e20 4d6f  lid Selection Mo
-0000fd50: 6465 3a20 7b73 656c 6563 746d 6f64 657d  de: {selectmode}
-0000fd60: 270a 2020 2020 2020 2020 2020 2020 2320  '.            # 
-0000fd70: 6c6f 6767 6572 2e64 6562 7567 2827 5365  logger.debug('Se
-0000fd80: 6c65 6374 696f 6e3a 2025 7227 2c20 7365  lection: %r', se
-0000fd90: 6c66 2e73 656c 6563 7469 6f6e 2829 290a  lf.selection()).
-0000fda0: 2020 2020 2020 2020 6966 206c 656e 2873          if len(s
-0000fdb0: 656c 6563 7469 6f6e 2920 3d3d 2030 3a0a  election) == 0:.
-0000fdc0: 2020 2020 2020 2020 2020 2020 2320 536b              # Sk
-0000fdd0: 6970 0a20 2020 2020 2020 2020 2020 2023  ip.            #
-0000fde0: 202d 204e 4f4e 4520 7365 6c65 6374 6d6f   - NONE selectmo
-0000fdf0: 6465 0a20 2020 2020 2020 2020 2020 2023  de.            #
-0000fe00: 202d 2075 6e2d 7365 6c65 6374 696f 6e73   - un-selections
-0000fe10: 2028 7573 7561 6c6c 7920 7468 6520 5472   (usually the Tr
-0000fe20: 6565 2063 6f6e 7465 6e74 7320 6368 616e  ee contents chan
-0000fe30: 6765 6429 0a20 2020 2020 2020 2020 2020  ged).           
-0000fe40: 2070 6173 730a 2020 2020 2020 2020 656c   pass.        el
-0000fe50: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000fe60: 2320 5265 6775 6c61 7220 5365 6c65 6374  # Regular Select
-0000fe70: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-0000fe80: 6173 7365 7274 206c 656e 2873 656c 6563  assert len(selec
-0000fe90: 7469 6f6e 2920 3d3d 2031 2c20 6627 7b73  tion) == 1, f'{s
-0000fea0: 656c 6621 727d 3a20 496e 7661 6c69 6420  elf!r}: Invalid 
-0000feb0: 7365 6c65 6374 696f 6e20 6d6f 6465 270a  selection mode'.
-0000fec0: 2020 2020 2020 2020 2020 2020 7472 6565              tree
-0000fed0: 6964 203d 2073 656c 6563 7469 6f6e 5b30  id = selection[0
-0000fee0: 5d0a 2020 2020 2020 2020 2020 2020 6461  ].            da
-0000fef0: 7461 203d 2073 656c 662e 7764 6174 615b  ta = self.wdata[
-0000ff00: 7472 6565 6964 5d0a 2020 2020 2020 2020  treeid].        
-0000ff10: 2020 2020 7365 6c66 2e6f 6e53 656c 6563      self.onSelec
-0000ff20: 7428 7472 6565 6964 2c20 6461 7461 290a  t(treeid, data).
-0000ff30: 0a20 2020 2064 6566 205f 7472 6565 5f6f  .    def _tree_o
-0000ff40: 6e73 6574 2873 656c 662c 2076 616c 7565  nset(self, value
-0000ff50: 3a20 7479 7069 6e67 2e53 6571 7565 6e63  : typing.Sequenc
-0000ff60: 655b 6d6f 6465 6c2e 5472 6565 456c 656d  e[model.TreeElem
-0000ff70: 656e 745d 2920 2d3e 204e 6f6e 653a 0a20  ent]) -> None:. 
-0000ff80: 2020 2020 2020 2027 2727 4361 6c6c 6261         '''Callba
-0000ff90: 636b 2074 6f20 6265 2065 7865 6375 7465  ck to be execute
-0000ffa0: 6420 7768 656e 2073 6574 7469 6e67 2061  d when setting a
-0000ffb0: 2064 6966 6665 7265 6e74 2076 616c 7565   different value
-0000ffc0: 2e0a 0a20 2020 2020 2020 2041 7661 696c  ...        Avail
-0000ffd0: 6162 6c65 2066 6f72 2073 7562 636c 6173  able for subclas
-0000ffe0: 7320 7265 6465 6669 6e69 7469 6f6e 2e0a  s redefinition..
-0000fff0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-00010000: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
-00010010: 6620 6f6e 5365 6c65 6374 2873 656c 662c  f onSelect(self,
-00010020: 2074 7265 6569 643a 2073 7472 2c20 6461   treeid: str, da
-00010030: 7461 3a20 7479 7069 6e67 2e41 6e79 203d  ta: typing.Any =
-00010040: 204e 6f6e 6529 202d 3e20 4e6f 6e65 3a0a   None) -> None:.
-00010050: 2020 2020 2020 2020 2727 2743 616c 6c62          '''Callb
-00010060: 6163 6b20 746f 2062 6520 6578 6563 7574  ack to be execut
-00010070: 6564 2077 6865 6e20 636c 6963 6b69 6e67  ed when clicking
-00010080: 2074 6869 7320 7769 6467 6574 2e0a 0a20   this widget... 
-00010090: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
-000100a0: 746f 2064 6f69 6e67 206e 6f74 6869 6e67  to doing nothing
-000100b0: 2e0a 0a20 2020 2020 2020 2041 7661 696c  ...        Avail
-000100c0: 6162 6c65 2066 6f72 2073 7562 636c 6173  able for subclas
-000100d0: 7320 7265 6465 6669 6e69 7469 6f6e 2e0a  s redefinition..
-000100e0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-000100f0: 2020 2020 2020 2020 2020 2074 7265 6569             treei
-00010100: 643a 2054 6865 2073 656c 6563 7465 6420  d: The selected 
-00010110: 7472 6565 2069 640a 2020 2020 2020 2020  tree id.        
-00010120: 2020 2020 6461 7461 3a20 5468 6520 6172      data: The ar
-00010130: 6269 7472 6172 7920 6461 7461 2061 7373  bitrary data ass
-00010140: 6f63 6961 7465 6420 7769 7468 2074 6865  ociated with the
-00010150: 2065 6c65 6d65 6e74 2e20 4465 6661 756c   element. Defaul
-00010160: 7473 2074 6f20 604e 6f6e 6560 2e0a 2020  ts to `None`..  
-00010170: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-00010180: 2020 7061 7373 0a0a 0a63 6c61 7373 204c    pass...class L
-00010190: 6973 7462 6f78 2854 7265 6529 3a0a 2020  istbox(Tree):.  
-000101a0: 2020 2727 2741 206c 6973 7462 6f78 2077    '''A listbox w
-000101b0: 6964 6765 742c 2061 206c 6973 7420 6f66  idget, a list of
-000101c0: 2073 7472 696e 6773 2e0a 0a20 2020 2054   strings...    T
-000101d0: 6869 7320 6973 2061 206d 6f64 6572 6e20  his is a modern 
-000101e0: 7661 7269 6174 696f 6e20 6f66 2074 6865  variation of the
-000101f0: 206c 6973 7462 6f78 2c20 6120 7761 7920   listbox, a way 
-00010200: 746f 2064 6973 706c 6179 2073 6576 6572  to display sever
-00010210: 616c 2072 6f77 7320 6f66 0a20 2020 2063  al rows of.    c
-00010220: 6f6e 7465 6e74 2028 7369 6d70 6c65 2073  ontent (simple s
-00010230: 7472 696e 6773 2c20 696e 2074 6869 7320  trings, in this 
-00010240: 6361 7365 292c 2061 6e64 2062 6520 6162  case), and be ab
-00010250: 6c65 2074 6f20 7365 6c65 6374 206f 6e65  le to select one
-00010260: 2061 7420 610a 2020 2020 7469 6d65 2e0a   at a.    time..
-00010270: 0a20 2020 2054 6865 2060 6068 6569 6768  .    The ``heigh
-00010280: 7460 6020 6361 6e20 6265 2068 6172 6463  t`` can be hardc
-00010290: 6f64 6564 2074 6f20 6120 7661 6c75 652c  oded to a value,
-000102a0: 206f 7220 6974 2063 616e 2076 6172 7920   or it can vary 
-000102b0: 7769 7468 2074 6865 0a20 2020 2063 6f6e  with the.    con
-000102c0: 7465 6e74 732e 204e 6f74 6520 7468 6174  tents. Note that
-000102d0: 2074 6865 2060 606d 6178 4865 6967 6874   the ``maxHeight
-000102e0: 6060 2069 7320 736d 616c 6c65 7220 7468  `` is smaller th
-000102f0: 616e 2074 6865 2061 6d6f 756e 7420 6f66  an the amount of
-00010300: 2072 6f77 7320 746f 0a20 2020 2064 6973   rows to.    dis
-00010310: 706c 6179 2c20 6e6f 2073 6372 6f6c 6c62  play, no scrollb
-00010320: 6172 2069 7320 7368 6f77 6e2c 2062 7574  ar is shown, but
-00010330: 2074 6865 206c 6973 7420 6361 6e20 6265   the list can be
-00010340: 0a20 2020 2073 6372 6f6c 6c65 6420 7769  .    scrolled wi
-00010350: 7468 2074 6865 206d 6f75 7365 2077 6865  th the mouse whe
-00010360: 656c 2e0a 2020 2020 5468 6520 6175 746f  el..    The auto
-00010370: 6d61 7469 6320 7661 7269 6174 696f 6e20  matic variation 
-00010380: 6f6e 2074 6865 2068 6569 6768 7420 7369  on the height si
-00010390: 7a65 2028 414b 4120 6175 746f 2d68 6569  ze (AKA auto-hei
-000103a0: 6768 7429 2063 616e 2062 650a 2020 2020  ght) can be.    
-000103b0: 636f 6d70 6c65 7465 6c79 2064 6973 6162  completely disab
-000103c0: 6c65 6420 6279 2073 6574 7469 6e67 2061  led by setting a
-000103d0: 6c6c 2068 6569 6768 742d 7265 6c61 7465  ll height-relate
-000103e0: 6420 6172 6775 6d65 6e74 7320 746f 2060  d arguments to `
-000103f0: 4e6f 6e65 602e 2054 6869 730a 2020 2020  None`. This.    
-00010400: 6973 2074 6865 2064 6566 6175 6c74 2e20  is the default. 
-00010410: 5468 6520 6060 6578 7061 6e64 6060 2061  The ``expand`` a
-00010420: 7267 756d 656e 7420 6973 2073 6574 2074  rgument is set t
-00010430: 6f20 6046 616c 7365 6020 7768 656e 2074  o `False` when t
-00010440: 6865 0a20 2020 2061 7574 6f2d 6865 6967  he.    auto-heig
-00010450: 6874 2069 7320 6469 7361 626c 6564 2e0a  ht is disabled..
-00010460: 0a20 2020 2045 6163 6820 7374 7269 6e67  .    Each string
-00010470: 2069 7320 6365 6e74 6572 6564 206f 6e20   is centered on 
-00010480: 7468 6520 6c69 7374 2e20 5468 6973 2063  the list. This c
-00010490: 616e 2062 6520 7477 6561 6b65 6420 7573  an be tweaked us
-000104a0: 696e 6720 7468 650a 2020 2020 6060 636f  ing the.    ``co
-000104b0: 6c75 6d6e 436f 6e66 6967 6060 2061 7267  lumnConfig`` arg
-000104c0: 756d 656e 742e 0a0a 2020 2020 5468 6520  ument...    The 
-000104d0: 7374 6174 6520 6973 2061 2060 6c69 7374  state is a `list
-000104e0: 6020 6f66 2060 7374 7260 2076 616c 7565  ` of `str` value
-000104f0: 732c 2060 7661 722e 5374 7269 6e67 4c69  s, `var.StringLi
-00010500: 7374 602e 0a0a 2020 2020 5468 6973 2069  st`...    This i
-00010510: 7320 6120 7661 7269 6174 696f 6e20 6f6e  s a variation on
-00010520: 2074 6865 2060 5472 6565 6020 7769 6467   the `Tree` widg
-00010530: 6574 2c20 7769 7468 2061 2073 696e 676c  et, with a singl
-00010540: 6520 636f 6c75 6d6e 2c20 6120 6469 6666  e column, a diff
-00010550: 6572 656e 740a 2020 2020 7661 7269 6162  erent.    variab
-00010560: 6c65 2074 7970 6520 616e 6420 736f 6d65  le type and some
-00010570: 206f 7665 7272 6964 656e 2064 6566 6175   overriden defau
-00010580: 6c74 2076 616c 7565 732e 0a20 2020 2053  lt values..    S
-00010590: 6565 2061 6c73 6f20 6050 7974 686f 6e20  ee also `Python 
-000105a0: 7474 6b2e 5472 6565 7669 6577 203c 746b  ttk.Treeview <tk
-000105b0: 696e 7465 722e 7474 6b2e 5472 6565 7669  inter.ttk.Treevi
-000105c0: 6577 3e60 2061 6e64 2060 6054 6b60 600a  ew>` and ``Tk``.
-000105d0: 2020 2020 6074 746b 2e54 7265 6576 6965      `ttk.Treevie
-000105e0: 7720 3c68 7474 7073 3a2f 2f74 636c 2e74  w <https://tcl.t
-000105f0: 6b2f 6d61 6e2f 7463 6c38 2e36 2f54 6b43  k/man/tcl8.6/TkC
-00010600: 6d64 2f74 746b 5f74 7265 6576 6965 772e  md/ttk_treeview.
-00010610: 6874 6d3e 605f 0a20 2020 2064 6f63 756d  htm>`_.    docum
-00010620: 656e 7461 7469 6f6e 2e0a 0a20 2020 2041  entation...    A
-00010630: 7267 733a 0a20 2020 2020 2020 2076 6172  rgs:.        var
-00010640: 6961 626c 653a 2055 7365 2061 6e20 6578  iable: Use an ex
-00010650: 7465 726e 616c 6c79 2064 6566 696e 6564  ternally defined
-00010660: 2076 6172 6961 626c 652c 2069 6e73 7465   variable, inste
-00010670: 6164 206f 6620 6372 6561 7469 6e67 2061  ad of creating a
-00010680: 206e 6577 0a20 2020 2020 2020 2020 2020   new.           
-00010690: 206f 6e65 2073 7065 6369 6669 6320 666f   one specific fo
-000106a0: 7220 7468 6973 2077 6964 6765 742e 0a20  r this widget.. 
-000106b0: 2020 2020 2020 206c 6162 656c 3a20 5468         label: Th
-000106c0: 6520 6c61 6265 6c20 746f 2069 6e63 6c75  e label to inclu
-000106d0: 6465 2062 6573 6964 6573 2074 6865 206c  de besides the l
-000106e0: 6973 7462 6f78 2e20 4361 6e20 6265 2067  istbox. Can be g
-000106f0: 6976 656e 2061 7320 610a 2020 2020 2020  iven as a.      
-00010700: 2020 2020 2020 636c 6173 7320 7661 7269        class vari
-00010710: 6162 6c65 2e0a 2020 2020 2020 2020 2020  able..          
-00010720: 2020 4f70 7469 6f6e 616c 2c20 7768 656e    Optional, when
-00010730: 2067 6976 656e 2069 7320 7368 6f77 2061   given is show a
-00010740: 7320 7468 6520 7369 6e67 6c65 2063 6f6c  s the single col
-00010750: 756d 6e20 6865 6164 696e 672e 0a20 2020  umn heading..   
-00010760: 2020 2020 2063 6f6c 756d 6e43 6f6e 6669       columnConfi
-00010770: 673a 204f 7665 7272 6964 6520 636f 6e66  g: Override conf
-00010780: 6967 7572 6174 696f 6e20 666f 7220 7468  iguration for th
-00010790: 6520 7369 6e67 6c65 2063 6f6c 756d 6e2e  e single column.
-000107a0: 2041 6476 616e 6365 640a 2020 2020 2020   Advanced.      
-000107b0: 2020 2020 2020 7573 6167 6520 6f6e 6c79        usage only
-000107c0: 2e0a 2020 2020 2020 2020 6865 6967 6874  ..        height
-000107d0: 3a20 4966 2067 6976 656e 2c20 616c 7761  : If given, alwa
-000107e0: 7973 2073 686f 7720 7468 6973 2071 7561  ys show this qua
-000107f0: 6e74 6974 7920 6f66 2072 6f77 732e 0a20  ntity of rows.. 
-00010800: 2020 2020 2020 2020 2020 2049 6620 6974             If it
-00010810: 2069 7320 604e 6f6e 6560 2c20 7468 6520   is `None`, the 
-00010820: 6e75 6d62 6572 206f 6620 7065 726d 616e  number of perman
-00010830: 656e 746c 7920 7368 6f77 6e20 726f 7773  ently shown rows
-00010840: 2077 696c 6c20 7661 7279 2062 6574 7765   will vary betwe
-00010850: 656e 0a20 2020 2020 2020 2020 2020 2060  en.            `
-00010860: 606d 696e 4865 6967 6874 6060 2061 6e64  `minHeight`` and
-00010870: 2060 606d 6178 4865 6967 6874 6060 2e0a   ``maxHeight``..
-00010880: 2020 2020 2020 2020 6d69 6e48 6569 6768          minHeigh
-00010890: 743a 2049 6620 6060 6865 6967 6874 6060  t: If ``height``
-000108a0: 2069 7320 604e 6f6e 6560 2c20 6d61 6b65   is `None`, make
-000108b0: 2073 7572 6520 7468 6973 206e 756d 6265   sure this numbe
-000108c0: 7220 6f66 2072 6f77 7320 6973 0a20 2020  r of rows is.   
-000108d0: 2020 2020 2020 2020 2061 6c77 6179 7320           always 
-000108e0: 7669 7369 626c 652e 0a20 2020 2020 2020  visible..       
-000108f0: 2020 2020 204f 7074 696f 6e61 6c2c 2077       Optional, w
-00010900: 6865 6e20 604e 6f6e 6560 2c20 7468 6572  hen `None`, ther
-00010910: 6527 7320 6e6f 206c 6f77 6572 206c 696d  e's no lower lim
-00010920: 6974 206f 6e20 7468 6520 7669 7369 626c  it on the visibl
-00010930: 6520 6e75 6d62 6572 0a20 2020 2020 2020  e number.       
-00010940: 2020 2020 206f 6620 726f 7773 2e0a 2020       of rows..  
-00010950: 2020 2020 2020 6d61 7848 6569 6768 743a        maxHeight:
-00010960: 2049 6620 6060 6865 6967 6874 6060 2069   If ``height`` i
-00010970: 7320 604e 6f6e 6560 2c20 6d61 6b65 2073  s `None`, make s
-00010980: 7572 6520 7468 6572 6520 6172 6520 6e6f  ure there are no
-00010990: 206d 6f72 650a 2020 2020 2020 2020 2020   more.          
-000109a0: 2020 7669 7369 626c 6520 726f 7773 2074    visible rows t
-000109b0: 6861 6e20 7468 6973 206e 756d 6265 722e  han this number.
-000109c0: 0a20 2020 2020 2020 2020 2020 204f 7074  .            Opt
-000109d0: 696f 6e61 6c2c 2077 6865 6e20 604e 6f6e  ional, when `Non
-000109e0: 6560 2c20 7468 6572 6527 7320 6e6f 2075  e`, there's no u
-000109f0: 7070 6572 206c 696d 6974 206f 6e20 7468  pper limit on th
-00010a00: 6520 7669 7369 626c 650a 2020 2020 2020  e visible.      
-00010a10: 2020 2020 2020 6e75 6d62 6572 206f 6620        number of 
-00010a20: 726f 7773 2e0a 2020 2020 2020 2020 7365  rows..        se
-00010a30: 6c65 6374 6162 6c65 3a20 5365 6520 6054  lectable: See `T
-00010a40: 7265 6560 2066 6f72 2069 7473 206d 6561  ree` for its mea
-00010a50: 6e69 6e67 2e0a 2020 2020 2020 2020 2020  ning..          
-00010a60: 2020 4465 6661 756c 7473 2074 6f20 6054    Defaults to `T
-00010a70: 7275 6560 2e0a 2020 2020 2020 2020 7374  rue`..        st
-00010a80: 796c 655f 616c 7462 673a 2053 6565 2060  yle_altbg: See `
-00010a90: 5472 6565 6020 666f 7220 6974 7320 6d65  Tree` for its me
-00010aa0: 616e 696e 672e 0a20 2020 2020 2020 2020  aning..         
-00010ab0: 2020 2044 6566 6175 6c74 7320 746f 2060     Defaults to `
-00010ac0: 4661 6c73 6560 2e0a 2020 2020 2020 2020  False`..        
-00010ad0: 6578 7061 6e64 3a20 5365 6520 6054 7265  expand: See `Tre
-00010ae0: 6560 2066 6f72 2069 7473 206d 6561 6e69  e` for its meani
-00010af0: 6e67 2e0a 2020 2020 2020 2020 2020 2020  ng..            
-00010b00: 4465 6661 756c 7473 2074 6f20 6046 616c  Defaults to `Fal
-00010b10: 7365 602c 2062 7574 2069 6e74 6572 6163  se`, but interac
-00010b20: 7473 2077 6974 6820 7468 6520 6175 746f  ts with the auto
-00010b30: 2d68 6569 6768 7420 7365 7474 696e 6773  -height settings
-00010b40: 2e0a 2020 2020 2020 2020 7374 796c 653a  ..        style:
-00010b50: 2043 6f6e 6669 6775 7265 2074 6865 2077   Configure the w
-00010b60: 6964 6765 7420 7374 796c 652e 0a0a 2020  idget style...  
-00010b70: 2020 2020 2020 7061 7265 6e74 3a20 5468        parent: Th
-00010b80: 6520 7061 7265 6e74 2077 6964 6765 742e  e parent widget.
-00010b90: 2043 616e 2062 6520 6120 6052 6f6f 7457   Can be a `RootW
-00010ba0: 696e 646f 7760 206f 7220 616e 6f74 6865  indow` or anothe
-00010bb0: 7220 606d 6978 696e 2e43 6f6e 7461 696e  r `mixin.Contain
-00010bc0: 6572 5769 6467 6574 602e 0a20 2020 2027  erWidget`..    '
-00010bd0: 2727 0a20 2020 206c 6162 656c 3a20 7479  ''.    label: ty
-00010be0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7374  ping.Optional[st
-00010bf0: 725d 203d 204e 6f6e 650a 0a20 2020 2040  r] = None..    @
-00010c00: 6461 7461 636c 6173 730a 2020 2020 636c  dataclass.    cl
-00010c10: 6173 7320 5374 796c 6528 5472 6565 2e53  ass Style(Tree.S
-00010c20: 7479 6c65 293a 0a20 2020 2020 2020 2027  tyle):.        '
-00010c30: 2727 604c 6973 7462 6f78 6020 7374 796c  ''`Listbox` styl
-00010c40: 6520 6f62 6a65 6374 2e0a 0a20 2020 2020  e object...     
-00010c50: 2020 2053 6565 2060 5472 6565 2e53 7479     See `Tree.Sty
-00010c60: 6c65 6020 666f 7220 7570 7374 7265 616d  le` for upstream
-00010c70: 2076 616c 7565 732c 2074 6865 7365 2061   values, these a
-00010c80: 7265 2074 6865 2064 6966 6665 7265 6e63  re the differenc
-00010c90: 6573 3a0a 0a20 2020 2020 2020 2041 7267  es:..        Arg
-00010ca0: 733a 0a20 2020 2020 2020 2020 2020 2061  s:.            a
-00010cb0: 6c74 6267 3a20 4469 7361 626c 6564 2062  ltbg: Disabled b
-00010cc0: 7920 6465 6661 756c 742e 0a20 2020 2020  y default..     
-00010cd0: 2020 2020 2020 2073 686f 775f 6c61 6265         show_labe
-00010ce0: 6c73 3a20 556e 7375 7070 6f72 7465 642e  ls: Unsupported.
-00010cf0: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-00010d00: 2020 2020 2061 6c74 6267 3a20 626f 6f6c       altbg: bool
-00010d10: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
-00010d20: 2073 686f 775f 6c61 6265 6c73 3a20 626f   show_labels: bo
-00010d30: 6f6c 203d 2046 616c 7365 0a0a 2020 2020  ol = False..    
-00010d40: 2020 2020 6966 205f 5f64 6562 7567 5f5f      if __debug__
-00010d50: 3a0a 2020 2020 2020 2020 2020 2020 6465  :.            de
-00010d60: 6620 5f5f 706f 7374 5f69 6e69 745f 5f28  f __post_init__(
-00010d70: 7365 6c66 293a 0a20 2020 2020 2020 2020  self):.         
-00010d80: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-00010d90: 686f 775f 6c61 6265 6c73 3a0a 2020 2020  how_labels:.    
-00010da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010db0: 7761 726e 696e 6773 2e77 6172 6e28 6627  warnings.warn(f'
-00010dc0: 7b73 656c 667d 3a20 556e 7375 7070 6f72  {self}: Unsuppor
-00010dd0: 7465 6420 2273 686f 775f 6c61 6265 6c73  ted "show_labels
-00010de0: 2227 2c20 7374 6163 6b6c 6576 656c 3d33  "', stacklevel=3
-00010df0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00010e00: 2020 7365 6c66 2e73 686f 775f 6c61 6265    self.show_labe
-00010e10: 6c73 203d 2046 616c 7365 0a0a 2020 2020  ls = False..    
-00010e20: 7374 6174 655f 7479 7065 203d 2076 6172  state_type = var
-00010e30: 2e53 7472 696e 674c 6973 7420 2023 2074  .StringList  # t
-00010e40: 7970 653a 2069 676e 6f72 6520 2023 2043  ype: ignore  # C
-00010e50: 6861 6e67 6520 7468 6520 7661 7269 6162  hange the variab
-00010e60: 6c65 2074 7970 650a 0a20 2020 2064 6566  le type..    def
-00010e70: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-00010e80: 2a61 7267 732c 2076 6172 6961 626c 653a  *args, variable:
-00010e90: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-00010ea0: 5b76 6172 2e53 7472 696e 674c 6973 745d  [var.StringList]
-00010eb0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00010ec0: 2020 2020 2020 2020 2020 6c61 6265 6c3a            label:
-00010ed0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-00010ee0: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
-00010ef0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00010f00: 6f6c 756d 6e43 6f6e 6669 673a 2074 7970  olumnConfig: typ
-00010f10: 696e 672e 4d61 7070 696e 675b 7374 722c  ing.Mapping[str,
-00010f20: 2074 7970 696e 672e 416e 795d 203d 204e   typing.Any] = N
-00010f30: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00010f40: 2020 2020 2020 6865 6967 6874 3a20 7479        height: ty
-00010f50: 7069 6e67 2e4f 7074 696f 6e61 6c5b 696e  ping.Optional[in
-00010f60: 745d 203d 204e 6f6e 652c 206d 696e 4865  t] = None, minHe
-00010f70: 6967 6874 3a20 7479 7069 6e67 2e4f 7074  ight: typing.Opt
-00010f80: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-00010f90: 652c 206d 6178 4865 6967 6874 3a20 7479  e, maxHeight: ty
-00010fa0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 696e  ping.Optional[in
-00010fb0: 745d 203d 204e 6f6e 652c 0a20 2020 2020  t] = None,.     
-00010fc0: 2020 2020 2020 2020 2020 2020 7365 6c65              sele
-00010fd0: 6374 6162 6c65 3a20 626f 6f6c 203d 2054  ctable: bool = T
-00010fe0: 7275 652c 2065 7870 616e 643a 2074 7970  rue, expand: typ
-00010ff0: 696e 672e 4f70 7469 6f6e 616c 5b62 6f6f  ing.Optional[boo
-00011000: 6c5d 203d 204e 6f6e 652c 2020 2320 4f76  l] = None,  # Ov
-00011010: 6572 7269 6465 0a20 2020 2020 2020 2020  erride.         
-00011020: 2020 2020 2020 2020 7374 796c 653a 2053          style: S
-00011030: 7479 6c65 203d 2053 7479 6c65 285f 6465  tyle = Style(_de
-00011040: 6661 756c 743d 5472 7565 292c 0a20 2020  fault=True),.   
-00011050: 2020 2020 2020 2020 2020 2020 2020 2a2a                **
-00011060: 6b77 6172 6773 293a 0a20 2020 2020 2020  kwargs):.       
-00011070: 2063 686f 7365 6e5f 6c61 6265 6c20 3d20   chosen_label = 
-00011080: 7365 6c66 2e6c 6162 656c 206f 7220 6c61  self.label or la
-00011090: 6265 6c0a 2020 2020 2020 2020 6966 2073  bel.        if s
-000110a0: 7479 6c65 2e5f 6465 6661 756c 743a 0a20  tyle._default:. 
-000110b0: 2020 2020 2020 2020 2020 2073 7479 6c65             style
-000110c0: 2e73 686f 775f 6865 6164 696e 6773 203d  .show_headings =
-000110d0: 2063 686f 7365 6e5f 6c61 6265 6c20 6973   chosen_label is
-000110e0: 206e 6f74 204e 6f6e 650a 2020 2020 2020   not None.      
-000110f0: 2020 6b77 6172 6773 2e75 7064 6174 6528    kwargs.update(
-00011100: 7b0a 2020 2020 2020 2020 2020 2020 276c  {.            'l
-00011110: 6162 656c 273a 2063 686f 7365 6e5f 6c61  abel': chosen_la
-00011120: 6265 6c2c 0a20 2020 2020 2020 2020 2020  bel,.           
-00011130: 2027 7661 7269 6162 6c65 273a 2076 6172   'variable': var
-00011140: 6961 626c 652c 0a20 2020 2020 2020 2020  iable,.         
-00011150: 2020 2027 7365 6c65 6374 6162 6c65 273a     'selectable':
-00011160: 2073 656c 6563 7461 626c 652c 2020 2320   selectable,  # 
-00011170: 4f76 6572 7269 6465 0a20 2020 2020 2020  Override.       
-00011180: 2020 2020 2027 636f 6c75 6d6e 7327 3a20       'columns': 
-00011190: 7b27 6c61 6265 6c27 3a20 6368 6f73 656e  {'label': chosen
-000111a0: 5f6c 6162 656c 206f 7220 274c 6162 656c  _label or 'Label
-000111b0: 277d 2c20 2023 2053 696e 676c 6520 436f  '},  # Single Co
-000111c0: 6c75 6d6e 2022 6c61 6265 6c22 0a20 2020  lumn "label".   
-000111d0: 2020 2020 2020 2020 2027 7374 796c 6527           'style'
-000111e0: 3a20 7374 796c 652c 0a20 2020 2020 2020  : style,.       
-000111f0: 207d 290a 2020 2020 2020 2020 2320 436f   }).        # Co
-00011200: 6e66 6967 7572 6520 6865 6967 6874 0a20  nfigure height. 
-00011210: 2020 2020 2020 2073 656c 662e 6865 6967         self.heig
-00011220: 6874 5261 6e67 653a 2074 7970 696e 672e  htRange: typing.
-00011230: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
-00011240: 5475 706c 655b 7479 7069 6e67 2e4f 7074  Tuple[typing.Opt
-00011250: 696f 6e61 6c5b 696e 745d 2c20 7479 7069  ional[int], typi
-00011260: 6e67 2e4f 7074 696f 6e61 6c5b 696e 745d  ng.Optional[int]
-00011270: 5d5d 0a20 2020 2020 2020 2069 6620 6865  ]].        if he
-00011280: 6967 6874 2069 7320 4e6f 6e65 3a0a 2020  ight is None:.  
-00011290: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
-000112a0: 6569 6768 7452 616e 6765 203d 206d 696e  eightRange = min
-000112b0: 4865 6967 6874 2c20 6d61 7848 6569 6768  Height, maxHeigh
-000112c0: 740a 2020 2020 2020 2020 656c 7365 3a0a  t.        else:.
-000112d0: 2020 2020 2020 2020 2020 2020 6b77 6172              kwar
-000112e0: 6773 5b27 6865 6967 6874 275d 203d 2068  gs['height'] = h
-000112f0: 6569 6768 7420 2023 2048 6172 6463 6f64  eight  # Hardcod
-00011300: 6520 7468 6520 6865 6967 6874 2076 616c  e the height val
-00011310: 7565 0a20 2020 2020 2020 2020 2020 2073  ue.            s
-00011320: 656c 662e 6865 6967 6874 5261 6e67 6520  elf.heightRange 
-00011330: 3d20 4e6f 6e65 0a20 2020 2020 2020 2069  = None.        i
-00011340: 6620 6865 6967 6874 206f 7220 6d69 6e48  f height or minH
-00011350: 6569 6768 7420 6f72 206d 6178 4865 6967  eight or maxHeig
-00011360: 6874 2061 6e64 2065 7870 616e 6420 6973  ht and expand is
-00011370: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00011380: 2020 2023 2044 6f6e 2774 2065 7870 616e     # Don't expan
-00011390: 6420 7768 656e 2074 6865 2066 6978 6564  d when the fixed
-000113a0: 206f 7220 7661 7279 696e 6720 6865 6967   or varying heig
-000113b0: 6874 2069 7320 7365 740a 2020 2020 2020  ht is set.      
-000113c0: 2020 2020 2020 6578 7061 6e64 203d 2046        expand = F
-000113d0: 616c 7365 0a20 2020 2020 2020 2023 2043  alse.        # C
-000113e0: 6f6e 6669 6775 7265 2028 7369 6e67 6c65  onfigure (single
-000113f0: 2920 636f 6c75 6d6e 0a20 2020 2020 2020  ) column.       
-00011400: 2023 202d 2044 6f6e 2774 2075 7365 2060   # - Don't use `
-00011410: 2330 6020 7369 6e63 6520 7468 6174 2069  #0` since that i
-00011420: 7320 6e6f 7420 7072 6f70 6572 6c79 2063  s not properly c
-00011430: 656e 7465 7265 642c 2069 7420 6861 7320  entered, it has 
-00011440: 7468 6520 7472 6565 0a20 2020 2020 2020  the tree.       
-00011450: 2023 2020 2065 6c65 6d65 6e74 7320 696e   #   elements in
-00011460: 2074 6865 7265 2c20 6576 656e 2068 6964   there, even hid
-00011470: 6465 6e2e 0a20 2020 2020 2020 2063 436f  den..        cCo
-00011480: 6e66 6967 203d 207b 0a20 2020 2020 2020  nfig = {.       
-00011490: 2020 2020 2027 616e 6368 6f72 273a 2074       'anchor': t
-000114a0: 6b2e 4345 4e54 4552 2c0a 2020 2020 2020  k.CENTER,.      
-000114b0: 2020 2020 2020 2773 7472 6574 6368 273a        'stretch':
-000114c0: 2054 7275 652c 0a20 2020 2020 2020 207d   True,.        }
-000114d0: 0a20 2020 2020 2020 2069 6620 6578 7061  .        if expa
-000114e0: 6e64 2069 7320 6e6f 7420 4e6f 6e65 3a0a  nd is not None:.
-000114f0: 2020 2020 2020 2020 2020 2020 6b77 6172              kwar
-00011500: 6773 5b27 6578 7061 6e64 275d 203d 2065  gs['expand'] = e
-00011510: 7870 616e 640a 2020 2020 2020 2020 6966  xpand.        if
-00011520: 2063 6f6c 756d 6e43 6f6e 6669 673a 0a20   columnConfig:. 
-00011530: 2020 2020 2020 2020 2020 2063 436f 6e66             cConf
-00011540: 6967 2e75 7064 6174 6528 636f 6c75 6d6e  ig.update(column
-00011550: 436f 6e66 6967 290a 2020 2020 2020 2020  Config).        
-00011560: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
-00011570: 282a 6172 6773 2c20 2a2a 6b77 6172 6773  (*args, **kwargs
-00011580: 290a 2020 2020 2020 2020 2320 4d61 6b65  ).        # Make
-00011590: 2073 7572 6520 6343 6f6e 6669 6720 6b65   sure cConfig ke
-000115a0: 7973 206d 6174 6368 206f 7074 696f 6e73  ys match options
-000115b0: 2066 6f72 2060 746b 696e 7465 722e 7474   for `tkinter.tt
-000115c0: 6b2e 5472 6565 7669 6577 2e63 6f6c 756d  k.Treeview.colum
-000115d0: 6e60 0a20 2020 2020 2020 2073 656c 662e  n`.        self.
-000115e0: 636f 6c75 6d6e 2827 6c61 6265 6c27 2c20  column('label', 
-000115f0: 2a2a 6343 6f6e 6669 6729 2020 2320 7479  **cConfig)  # ty
-00011600: 7065 3a20 6967 6e6f 7265 0a0a 2020 2020  pe: ignore..    
-00011610: 6465 6620 5f74 7265 655f 6765 7428 7365  def _tree_get(se
-00011620: 6c66 2c20 7661 7269 6162 6c65 3a20 7661  lf, variable: va
-00011630: 722e 5661 7269 6162 6c65 2920 2d3e 2074  r.Variable) -> t
-00011640: 7970 696e 672e 5365 7175 656e 6365 5b6d  yping.Sequence[m
-00011650: 6f64 656c 2e54 7265 6545 6c65 6d65 6e74  odel.TreeElement
-00011660: 5d3a 0a20 2020 2020 2020 2072 6574 7572  ]:.        retur
-00011670: 6e20 5b6d 6f64 656c 2e54 7265 6545 6c65  n [model.TreeEle
-00011680: 6d65 6e74 286c 6162 656c 3d65 2c20 636f  ment(label=e, co
-00011690: 6c75 6d6e 733d 5b65 5d2c 2064 6174 613d  lumns=[e], data=
-000116a0: 6529 2066 6f72 2065 2069 6e20 7661 7269  e) for e in vari
-000116b0: 6162 6c65 2e67 6574 2829 5d0a 0a20 2020  able.get()]..   
-000116c0: 2064 6566 205f 7472 6565 5f6f 6e73 6574   def _tree_onset
-000116d0: 2873 656c 662c 2076 616c 7565 3a20 7479  (self, value: ty
-000116e0: 7069 6e67 2e53 6571 7565 6e63 655b 6d6f  ping.Sequence[mo
-000116f0: 6465 6c2e 5472 6565 456c 656d 656e 745d  del.TreeElement]
-00011700: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00011710: 2020 2069 6620 7365 6c66 2e68 6569 6768     if self.heigh
-00011720: 7452 616e 6765 2069 7320 6e6f 7420 4e6f  tRange is not No
-00011730: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00011740: 6d69 6e48 6569 6768 742c 206d 6178 4865  minHeight, maxHe
-00011750: 6967 6874 203d 2073 656c 662e 6865 6967  ight = self.heig
-00011760: 6874 5261 6e67 650a 2020 2020 2020 2020  htRange.        
-00011770: 2020 2020 7773 697a 6520 3d20 4e6f 6e65      wsize = None
-00011780: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00011790: 6d69 6e48 6569 6768 743a 0a20 2020 2020  minHeight:.     
-000117a0: 2020 2020 2020 2020 2020 2077 7369 7a65             wsize
-000117b0: 203d 206d 6178 286d 696e 4865 6967 6874   = max(minHeight
-000117c0: 2c20 6c65 6e28 7661 6c75 6529 290a 2020  , len(value)).  
-000117d0: 2020 2020 2020 2020 2020 6966 206d 6178            if max
-000117e0: 4865 6967 6874 3a0a 2020 2020 2020 2020  Height:.        
-000117f0: 2020 2020 2020 2020 7773 697a 6520 3d20          wsize = 
-00011800: 6d69 6e28 6d61 7848 6569 6768 742c 2077  min(maxHeight, w
-00011810: 7369 7a65 206f 7220 6c65 6e28 7661 6c75  size or len(valu
-00011820: 6529 290a 2020 2020 2020 2020 2020 2020  e)).            
-00011830: 6966 2077 7369 7a65 3a0a 2020 2020 2020  if wsize:.      
-00011840: 2020 2020 2020 2020 2020 6966 205f 5f64            if __d
-00011850: 6562 7567 5f5f 3a0a 2020 2020 2020 2020  ebug__:.        
-00011860: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-00011870: 6572 2e64 6562 7567 2866 277b 7365 6c66  er.debug(f'{self
-00011880: 7d3a 2041 7574 6f20 4865 6967 6874 3a20  }: Auto Height: 
-00011890: 7b77 7369 7a65 7d27 290a 2020 2020 2020  {wsize}').      
-000118a0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-000118b0: 6f6e 6669 6775 7265 2868 6569 6768 743d  onfigure(height=
-000118c0: 7773 697a 6529 0a0a 0a63 6c61 7373 2046  wsize)...class F
-000118d0: 7261 6d65 5061 6e65 6428 7474 6b2e 5061  ramePaned(ttk.Pa
-000118e0: 6e65 6457 696e 646f 772c 206d 6978 696e  nedWindow, mixin
-000118f0: 2e43 6f6e 7461 696e 6572 5769 6467 6574  .ContainerWidget
-00011900: 293a 0a20 2020 2027 2727 4120 6672 616d  ):.    '''A fram
-00011910: 6520 746f 2068 6f6c 6420 6f74 6865 7220  e to hold other 
-00011920: 7769 6467 6574 732c 2077 6974 6820 7573  widgets, with us
-00011930: 6572 2d63 6f6e 7472 6f6c 6c61 626c 6520  er-controllable 
-00011940: 7265 6c61 7469 7665 2073 697a 6573 2e0a  relative sizes..
-00011950: 0a20 2020 2054 6869 7320 6973 2073 696d  .    This is sim
-00011960: 696c 6172 2074 6f20 6120 6046 7261 6d65  ilar to a `Frame
-00011970: 556e 6c61 6265 6c6c 6564 602c 2072 6573  Unlabelled`, res
-00011980: 7472 6963 7465 6420 746f 2068 6f72 697a  tricted to horiz
-00011990: 6f6e 7461 6c20 6f72 0a20 2020 2076 6572  ontal or.    ver
-000119a0: 7469 6361 6c20 6c61 796f 7574 732c 2062  tical layouts, b
-000119b0: 7574 2077 6865 7265 2074 6865 2069 6e74  ut where the int
-000119c0: 6572 6661 6365 7320 6265 7477 6565 6e20  erfaces between 
-000119d0: 7468 6520 6368 696c 6472 656e 2063 616e  the children can
-000119e0: 2062 650a 2020 2020 6164 6a75 7374 6564   be.    adjusted
-000119f0: 2062 7920 7468 6520 7573 6572 2c20 746f   by the user, to
-00011a00: 2072 6573 697a 6520 7468 656d 2061 7420   resize them at 
-00011a10: 7769 6c6c 2e0a 0a20 2020 2054 6869 7320  will...    This 
-00011a20: 616c 6c6f 7773 2073 6f6d 6520 6368 696c  allows some chil
-00011a30: 6420 7769 6467 6574 7320 746f 2062 6520  d widgets to be 
-00011a40: 6869 6464 656e 2c20 6279 2072 6573 697a  hidden, by resiz
-00011a50: 696e 6720 7468 6520 6f74 6865 7220 7061  ing the other pa
-00011a60: 6e65 7320 746f 0a20 2020 2066 756c 6c79  nes to.    fully
-00011a70: 206f 6363 7570 7920 7468 6520 7769 6467   occupy the widg
-00011a80: 6574 2061 7265 612e 0a0a 2020 2020 4e6f  et area...    No
-00011a90: 7465 2074 6861 7420 7573 696e 6720 7468  te that using th
-00011aa0: 6973 2077 6974 6820 6d6f 7265 2074 6861  is with more tha
-00011ab0: 6e20 7477 6f20 6368 696c 6472 656e 2063  n two children c
-00011ac0: 616e 2062 6520 636f 6e66 7573 696e 6720  an be confusing 
-00011ad0: 666f 7220 7468 650a 2020 2020 7573 6572  for the.    user
-00011ae0: 732c 2070 6172 7469 6375 6c61 726c 7920  s, particularly 
-00011af0: 7768 656e 2072 6573 697a 696e 6720 7461  when resizing ta
-00011b00: 6b65 7320 706c 6163 652e 0a0a 2020 2020  kes place...    
-00011b10: 5468 6572 6520 6973 206e 6f20 5079 7468  There is no Pyth
-00011b20: 6f6e 2064 6f63 756d 656e 7461 7469 6f6e  on documentation
-00011b30: 2c20 7365 6520 6060 546b 6060 2060 7474  , see ``Tk`` `tt
-00011b40: 6b2e 5061 6e65 6457 696e 646f 7720 3c68  k.PanedWindow <h
-00011b50: 7474 7073 3a2f 2f77 7777 2e74 636c 2e74  ttps://www.tcl.t
-00011b60: 6b2f 6d61 6e2f 7463 6c2f 546b 436d 642f  k/man/tcl/TkCmd/
-00011b70: 7474 6b5f 7061 6e65 6477 696e 646f 772e  ttk_panedwindow.
-00011b80: 6874 6d6c 3e60 5f20 646f 6375 6d65 6e74  html>`_ document
-00011b90: 6174 696f 6e2e 0a0a 2020 2020 4172 6773  ation...    Args
-00011ba0: 3a0a 2020 2020 2020 2020 6c61 796f 7574  :.        layout
-00011bb0: 3a20 5468 6520 6f72 6965 6e74 6174 696f  : The orientatio
-00011bc0: 6e20 6f66 2074 6865 2063 6869 6c64 2077  n of the child w
-00011bd0: 6964 6765 7473 2e0a 2020 2020 2020 2020  idgets..        
-00011be0: 2020 2020 5265 7374 7269 6374 6564 2074      Restricted t
-00011bf0: 6f20 6060 746b 2e56 4552 5449 4341 4c60  o ``tk.VERTICAL`
-00011c00: 6020 6f72 2060 6074 6b2e 484f 5249 5a4f  ` or ``tk.HORIZO
-00011c10: 4e54 414c 6060 2e0a 2020 2020 2020 2020  NTAL``..        
-00011c20: 6f72 6965 6e74 3a20 416c 6961 7320 666f  orient: Alias fo
-00011c30: 7220 226c 6179 6f75 7422 2e0a 2020 2020  r "layout"..    
-00011c40: 2020 2020 7765 6967 6874 3a20 5468 6520      weight: The 
-00011c50: 7765 6967 6874 2066 6f72 2065 6163 6820  weight for each 
-00011c60: 6368 696c 6472 656e 2077 6964 6765 742e  children widget.
-00011c70: 204f 7074 696f 6e61 6c2c 2064 6566 6175   Optional, defau
-00011c80: 6c74 7320 746f 2031 2e0a 2020 2020 2020  lts to 1..      
-00011c90: 2020 7765 6967 6874 733a 2050 6572 2d63    weights: Per-c
-00011ca0: 6869 6c64 2077 6964 6765 742e 204f 7074  hild widget. Opt
-00011cb0: 696f 6e61 6c2c 2064 6566 6175 6c74 7320  ional, defaults 
-00011cc0: 746f 2074 6865 2063 6f6d 6d6f 6e20 2277  to the common "w
-00011cd0: 6569 6768 7422 2e0a 0a20 2020 204e 6f74  eight"...    Not
-00011ce0: 653a 0a20 2020 2020 2020 2054 6865 2060  e:.        The `
-00011cf0: 606c 6179 6f75 7460 602f 6060 6f72 6965  `layout``/``orie
-00011d00: 6e74 6060 2061 7267 756d 656e 7420 6861  nt`` argument ha
-00011d10: 7320 7369 6d69 6c61 7220 7365 6d61 6e74  s similar semant
-00011d20: 6963 7320 746f 2060 606c 6179 6f75 7460  ics to ``layout`
-00011d30: 600a 2020 2020 2020 2020 6172 6775 6d65  `.        argume
-00011d40: 6e74 206f 6e20 6f74 6865 7220 6672 616d  nt on other fram
-00011d50: 6520 7479 7065 732e 0a0a 2020 2020 5365  e types...    Se
-00011d60: 6520 416c 736f 3a0a 2020 2020 2020 2020  e Also:.        
-00011d70: 2d20 6046 7261 6d65 556e 6c61 6265 6c6c  - `FrameUnlabell
-00011d80: 6564 602c 2060 4672 616d 654c 6162 656c  ed`, `FrameLabel
-00011d90: 6c65 6460 3a20 5369 6d69 6c61 7220 7665  led`: Similar ve
-00011da0: 7273 696f 6e73 2c20 7769 7468 6f75 7420  rsions, without 
-00011db0: 7573 6572 0a20 2020 2020 2020 2020 2063  user.          c
-00011dc0: 6f6e 7472 6f6c 206f 7665 7220 7369 7a69  ontrol over sizi
-00011dd0: 6e67 2e0a 2020 2020 2727 270a 2020 2020  ng..    '''.    
-00011de0: 6c61 796f 7574 3a20 7479 7069 6e67 2e4f  layout: typing.O
-00011df0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-00011e00: 6f6e 650a 0a20 2020 2064 6566 205f 5f69  one..    def __i
-00011e10: 6e69 745f 5f28 7365 6c66 2c20 7061 7265  nit__(self, pare
-00011e20: 6e74 2c0a 2020 2020 2020 2020 2020 2020  nt,.            
-00011e30: 2020 2020 202a 6172 6773 2c0a 2020 2020       *args,.    
-00011e40: 2020 2020 2020 2020 2020 2020 206f 7269               ori
-00011e50: 656e 743a 2074 7970 696e 672e 4f70 7469  ent: typing.Opti
-00011e60: 6f6e 616c 5b74 7970 696e 672e 556e 696f  onal[typing.Unio
-00011e70: 6e5b 7479 7069 6e67 2e4c 6974 6572 616c  n[typing.Literal
-00011e80: 5b27 7665 7274 6963 616c 275d 2c20 7479  ['vertical'], ty
-00011e90: 7069 6e67 2e4c 6974 6572 616c 5b27 686f  ping.Literal['ho
-00011ea0: 7269 7a6f 6e74 616c 275d 5d5d 203d 204e  rizontal']]] = N
-00011eb0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00011ec0: 2020 2020 2020 7765 6967 6874 3a20 7479        weight: ty
-00011ed0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 696e  ping.Optional[in
-00011ee0: 745d 203d 204e 6f6e 652c 0a20 2020 2020  t] = None,.     
-00011ef0: 2020 2020 2020 2020 2020 2020 7765 6967              weig
-00011f00: 6874 733a 2074 7970 696e 672e 4f70 7469  hts: typing.Opti
-00011f10: 6f6e 616c 5b74 7970 696e 672e 4d61 7070  onal[typing.Mapp
-00011f20: 696e 675b 7374 722c 2069 6e74 5d5d 203d  ing[str, int]] =
-00011f30: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-00011f40: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
-00011f50: 293a 0a20 2020 2020 2020 2023 204f 7269  ):.        # Ori
-00011f60: 656e 7461 7469 6f6e 2063 616e 2062 6520  entation can be 
-00011f70: 6769 7665 6e20 6173 2074 6865 206c 6179  given as the lay
-00011f80: 6f75 740a 2020 2020 2020 2020 2320 4275  out.        # Bu
-00011f90: 7420 7468 6520 436f 6e74 6169 6e65 7257  t the ContainerW
-00011fa0: 6964 6765 7420 6c61 796f 7574 2069 7320  idget layout is 
-00011fb0: 616c 7761 7973 204e 6f6e 650a 2020 2020  always None.    
-00011fc0: 2020 2020 2320 4e6f 2044 6566 6175 6c74      # No Default
-00011fd0: 204f 7269 656e 7461 7469 6f6e 2c20 6d75   Orientation, mu
-00011fe0: 7374 2062 6520 6769 7665 6e20 736f 6d65  st be given some
-00011ff0: 7768 6572 650a 2020 2020 2020 2020 6f72  where.        or
-00012000: 6965 6e74 6174 696f 6e20 3d20 6b77 6172  ientation = kwar
-00012010: 6773 2e70 6f70 2827 6c61 796f 7574 272c  gs.pop('layout',
-00012020: 204e 6f6e 6529 206f 7220 6f72 6965 6e74   None) or orient
-00012030: 206f 7220 7365 6c66 2e6c 6179 6f75 740a   or self.layout.
-00012040: 2020 2020 2020 2020 6173 7365 7274 206f          assert o
-00012050: 7269 656e 7461 7469 6f6e 2069 6e20 5b74  rientation in [t
-00012060: 6b2e 5645 5254 4943 414c 2c20 746b 2e48  k.VERTICAL, tk.H
-00012070: 4f52 495a 4f4e 5441 4c5d 2c20 6627 496e  ORIZONTAL], f'In
-00012080: 7661 6c69 6420 4f72 6965 6e74 6174 696f  valid Orientatio
-00012090: 6e3a 207b 6f72 6965 6e74 6174 696f 6e7d  n: {orientation}
-000120a0: 270a 2020 2020 2020 2020 6966 2074 7970  '.        if typ
-000120b0: 696e 672e 5459 5045 5f43 4845 434b 494e  ing.TYPE_CHECKIN
-000120c0: 473a 0a20 2020 2020 2020 2020 2020 206f  G:.            o
-000120d0: 7269 656e 7461 7469 6f6e 203d 2074 7970  rientation = typ
-000120e0: 696e 672e 6361 7374 2874 7970 696e 672e  ing.cast(typing.
-000120f0: 556e 696f 6e5b 7479 7069 6e67 2e4c 6974  Union[typing.Lit
-00012100: 6572 616c 5b27 7665 7274 6963 616c 275d  eral['vertical']
-00012110: 2c20 7479 7069 6e67 2e4c 6974 6572 616c  , typing.Literal
-00012120: 5b27 686f 7269 7a6f 6e74 616c 275d 5d2c  ['horizontal']],
-00012130: 206f 7269 656e 7461 7469 6f6e 290a 2020   orientation).  
-00012140: 2020 2020 2020 7375 7065 7228 292e 5f5f        super().__
-00012150: 696e 6974 5f5f 2870 6172 656e 742c 206f  init__(parent, o
-00012160: 7269 656e 743d 6f72 6965 6e74 6174 696f  rient=orientatio
-00012170: 6e29 2020 2320 7474 6b2e 5061 6e65 6457  n)  # ttk.PanedW
-00012180: 696e 646f 770a 2020 2020 2020 2020 7365  indow.        se
-00012190: 6c66 2e69 6e69 745f 636f 6e74 6169 6e65  lf.init_containe
-000121a0: 7228 2a61 7267 732c 206c 6179 6f75 743d  r(*args, layout=
-000121b0: 4e6f 6e65 2c20 2a2a 6b77 6172 6773 290a  None, **kwargs).
-000121c0: 2020 2020 2020 2020 666f 7220 776e 616d          for wnam
-000121d0: 652c 2077 6964 6765 7420 696e 2073 656c  e, widget in sel
-000121e0: 662e 7769 6467 6574 732e 6974 656d 7328  f.widgets.items(
-000121f0: 293a 0a20 2020 2020 2020 2020 2020 2023  ):.            #
-00012200: 2057 6964 6765 7420 5765 6967 6874 3a20   Widget Weight: 
-00012210: 4465 6661 756c 7420 746f 2031 0a20 2020  Default to 1.   
-00012220: 2020 2020 2020 2020 2077 7765 6967 6874           wweight
-00012230: 203d 2077 6569 6768 7420 6f72 2031 0a20   = weight or 1. 
-00012240: 2020 2020 2020 2020 2020 2069 6620 7765             if we
-00012250: 6967 6874 733a 0a20 2020 2020 2020 2020  ights:.         
-00012260: 2020 2020 2020 2023 2050 6572 2d57 6964         # Per-Wid
-00012270: 6765 7420 4f76 6572 7269 6465 0a20 2020  get Override.   
-00012280: 2020 2020 2020 2020 2020 2020 2077 7765               wwe
-00012290: 6967 6874 203d 2077 6569 6768 7473 2e67  ight = weights.g
-000122a0: 6574 2877 6e61 6d65 2c20 7777 6569 6768  et(wname, wweigh
-000122b0: 7429 0a20 2020 2020 2020 2020 2020 2061  t).            a
-000122c0: 7373 6572 7420 6973 696e 7374 616e 6365  ssert isinstance
-000122d0: 2877 6964 6765 742c 2074 6b2e 5769 6467  (widget, tk.Widg
-000122e0: 6574 290a 2020 2020 2020 2020 2020 2020  et).            
-000122f0: 7365 6c66 2e61 6464 2877 6964 6765 742c  self.add(widget,
-00012300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012310: 2020 2020 2020 7765 6967 6874 3d77 7765        weight=wwe
-00012320: 6967 6874 290a 2020 2020 2020 2020 6173  ight).        as
-00012330: 7365 7274 206c 656e 2873 656c 662e 7061  sert len(self.pa
-00012340: 6e65 7328 2929 203d 3d20 6c65 6e28 7365  nes()) == len(se
-00012350: 6c66 2e77 6964 6765 7473 290a 0a0a 2320  lf.widgets)...# 
-00012360: 544f 444f 3a20 5375 7070 6f72 7420 6175  TODO: Support au
-00012370: 746f 2073 6372 6f6c 6c20 2868 6964 6520  to scroll (hide 
-00012380: 7363 726f 6c6c 6261 7273 2077 6865 6e20  scrollbars when 
-00012390: 7363 726f 6c6c 636f 6d6d 616e 6420 6973  scrollcommand is
-000123a0: 2063 616c 6c65 6420 6173 2060 7365 7428   called as `set(
-000123b0: 2730 2e30 272c 2027 312e 3027 2960 290a  '0.0', '1.0')`).
-000123c0: 636c 6173 7320 5363 726f 6c6c 6564 5769  class ScrolledWi
-000123d0: 6467 6574 2874 746b 2e46 7261 6d65 2c20  dget(ttk.Frame, 
-000123e0: 6d69 7869 6e2e 5369 6e67 6c65 5769 6467  mixin.SingleWidg
-000123f0: 6574 293a 0a20 2020 2027 2727 4120 7369  et):.    '''A si
-00012400: 6e67 6c65 2077 6964 6765 7420 6672 616d  ngle widget fram
-00012410: 6520 7772 6170 7065 722c 2074 6f20 696e  e wrapper, to in
-00012420: 636c 7564 6520 6675 6e63 7469 6f6e 616c  clude functional
-00012430: 2073 6372 6f6c 6c62 6172 732e 0a0a 2020   scrollbars...  
-00012440: 2020 5468 6973 2069 7320 6120 7772 6170    This is a wrap
-00012450: 7065 7220 6672 616d 652c 2077 6974 6820  per frame, with 
-00012460: 6120 7369 6e67 6c65 2063 6869 6c64 2077  a single child w
-00012470: 6964 6765 742c 2077 6869 6368 2069 6e63  idget, which inc
-00012480: 6c75 6465 730a 2020 2020 6675 6e63 7469  ludes.    functi
-00012490: 6f6e 616c 2073 6372 6f6c 6c62 6172 732e  onal scrollbars.
-000124a0: 2042 6f74 6820 686f 7269 7a6f 6e74 616c   Both horizontal
-000124b0: 2061 6e64 2076 6572 7469 6361 6c20 7363   and vertical sc
-000124c0: 726f 6c6c 6261 7273 2061 7265 0a20 2020  rollbars are.   
-000124d0: 2073 7570 706f 7274 6564 2028 6465 7065   supported (depe
-000124e0: 6e64 696e 6720 6f6e 2074 6865 2063 6869  nding on the chi
-000124f0: 6c64 2077 6964 6765 7429 2e0a 0a20 2020  ld widget)...   
-00012500: 2041 2063 6f72 6e65 7220 7769 6467 6574   A corner widget
-00012510: 2074 6f20 6869 6465 2074 6865 2022 626c   to hide the "bl
-00012520: 616e 6b22 2073 7061 6365 2062 6574 7765  ank" space betwe
-00012530: 656e 2073 6372 6f6c 6c62 6172 7320 6973  en scrollbars is
-00012540: 0a20 2020 2061 7574 6f6d 6174 6963 616c  .    automatical
-00012550: 6c79 2069 6e63 6c75 6465 6420 6966 206e  ly included if n
-00012560: 6565 6465 642c 2074 6869 7320 6973 2069  eeded, this is i
-00012570: 6d70 6c65 6d65 6e74 6564 2061 7320 6120  mplemented as a 
-00012580: 736f 2d63 616c 6c65 640a 2020 2020 2273  so-called.    "s
-00012590: 697a 6567 7269 7022 2e0a 0a20 2020 2054  izegrip"...    T
-000125a0: 6865 7265 2069 7320 6e6f 2050 7974 686f  here is no Pytho
-000125b0: 6e20 646f 6375 6d65 6e74 6174 696f 6e2c  n documentation,
-000125c0: 2073 6565 2060 6054 6b60 600a 2020 2020   see ``Tk``.    
-000125d0: 6074 746b 2e53 6372 6f6c 6c62 6172 203c  `ttk.Scrollbar <
-000125e0: 6874 7470 733a 2f2f 7777 772e 7463 6c2e  https://www.tcl.
-000125f0: 746b 2f6d 616e 2f74 636c 2f54 6b43 6d64  tk/man/tcl/TkCmd
-00012600: 2f74 746b 5f73 6372 6f6c 6c62 6172 2e68  /ttk_scrollbar.h
-00012610: 746d 6c3e 605f 2061 6e64 0a20 2020 2060  tml>`_ and.    `
-00012620: 7474 6b2e 5369 7a65 6772 6970 203c 6874  ttk.Sizegrip <ht
-00012630: 7470 733a 2f2f 7777 772e 7463 6c2e 746b  tps://www.tcl.tk
-00012640: 2f6d 616e 2f74 636c 2f54 6b43 6d64 2f74  /man/tcl/TkCmd/t
-00012650: 746b 5f73 697a 6567 7269 702e 6874 6d6c  tk_sizegrip.html
-00012660: 3e60 5f20 646f 6375 6d65 6e74 6174 696f  >`_ documentatio
-00012670: 6e2e 0a0a 2020 2020 5468 6520 7363 726f  n...    The scro
-00012680: 6c6c 6261 7273 2063 616e 2062 6520 666f  llbars can be fo
-00012690: 7263 6564 2074 6f20 6265 2073 686f 776e  rced to be shown
-000126a0: 2c20 6f72 2074 6865 7920 6361 6e20 6265  , or they can be
-000126b0: 2063 6f6e 6669 6775 7265 6420 696e 0a20   configured in. 
-000126c0: 2020 2061 7574 6f6d 6174 6963 206d 6f64     automatic mod
-000126d0: 652e 2054 6869 7320 7769 6c6c 2073 686f  e. This will sho
-000126e0: 7720 6f72 2068 6964 6520 7468 6520 7363  w or hide the sc
-000126f0: 726f 6c6c 6261 7273 2061 7320 6e65 6564  rollbars as need
-00012700: 6564 2e0a 2020 2020 5468 6973 2061 6d6f  ed..    This amo
-00012710: 756e 7473 2074 6f20 6869 6465 2074 6865  unts to hide the
-00012720: 6d20 7768 656e 2074 6865 2063 6869 6c64  m when the child
-00012730: 2077 6964 6765 7420 6e65 6564 7320 6e6f   widget needs no
-00012740: 2073 6372 6f6c 6c62 6172 732e 0a20 2020   scrollbars..   
-00012750: 2054 6865 2064 6566 6175 6c74 2062 6568   The default beh
-00012760: 6176 696f 7572 2069 7320 7468 6973 2061  aviour is this a
-00012770: 7574 6f6d 6174 6963 2073 686f 7769 6e67  utomatic showing
-00012780: 2f68 6964 696e 6720 666f 7220 626f 7468  /hiding for both
-00012790: 2073 6372 6f6c 6c62 6172 732e 0a0a 2020   scrollbars...  
-000127a0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-000127b0: 6368 696c 6443 6c61 7373 3a20 5468 6520  childClass: The 
-000127c0: 6368 696c 6472 656e 2063 6c61 7373 2028  children class (
-000127d0: 6361 6c6c 6564 2074 6f20 6372 6561 7465  called to create
-000127e0: 2074 6865 2063 6869 6c64 2077 6964 6765   the child widge
-000127f0: 7429 2e0a 2020 2020 2020 2020 2020 2020  t)..            
-00012800: 4d75 7374 2062 6520 6120 6053 696e 676c  Must be a `Singl
-00012810: 6557 6964 6765 7460 2e0a 2020 2020 2020  eWidget`..      
-00012820: 2020 7363 726f 6c6c 5665 7274 6963 616c    scrollVertical
-00012830: 3a20 5368 6f77 2074 6865 2076 6572 7469  : Show the verti
-00012840: 6361 6c20 7363 726f 6c6c 6261 722e 0a20  cal scrollbar.. 
-00012850: 2020 2020 2020 2020 2020 2055 7365 2061             Use a
-00012860: 2060 626f 6f6c 6020 746f 2066 6f72 6365   `bool` to force
-00012870: 2061 2073 7461 7465 2c20 6f72 2060 4e6f   a state, or `No
-00012880: 6e65 6020 746f 2061 7574 6f6d 6174 6963  ne` to automatic
-00012890: 616c 6c79 2073 686f 7720 6f72 2068 6964  ally show or hid
-000128a0: 6520 7468 6520 7363 726f 6c6c 6261 722e  e the scrollbar.
-000128b0: 0a20 2020 2020 2020 2020 2020 2044 6566  .            Def
-000128c0: 6175 6c74 7320 746f 2060 4e6f 6e65 602e  aults to `None`.
-000128d0: 0a20 2020 2020 2020 2073 6372 6f6c 6c48  .        scrollH
-000128e0: 6f72 697a 6f6e 7461 6c3a 2049 6e63 6c75  orizontal: Inclu
-000128f0: 6465 2061 2068 6f72 697a 6f6e 7461 6c20  de a horizontal 
-00012900: 7363 726f 6c6c 6261 722e 0a20 2020 2020  scrollbar..     
-00012910: 2020 2020 2020 2055 7365 2061 2060 626f         Use a `bo
-00012920: 6f6c 6020 746f 2066 6f72 6365 2061 2073  ol` to force a s
-00012930: 7461 7465 2c20 6f72 2060 4e6f 6e65 6020  tate, or `None` 
-00012940: 746f 2061 7574 6f6d 6174 6963 616c 6c79  to automatically
-00012950: 2073 686f 7720 6f72 2068 6964 6520 7468   show or hide th
-00012960: 6520 7363 726f 6c6c 6261 722e 0a20 2020  e scrollbar..   
-00012970: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
-00012980: 7320 746f 2060 4e6f 6e65 602e 0a20 2020  s to `None`..   
-00012990: 2020 2020 2073 6372 6f6c 6c45 7870 616e       scrollExpan
-000129a0: 643a 2045 7870 616e 6420 7468 6520 7061  d: Expand the pa
-000129b0: 7265 6e74 2077 6964 6765 742e 0a20 2020  rent widget..   
-000129c0: 2020 2020 2020 2020 2054 6869 7320 6973           This is
-000129d0: 2061 6e61 6c6f 676f 7573 2074 6f20 7468   analogous to th
-000129e0: 6520 6060 6578 7061 6e64 6060 2061 7267  e ``expand`` arg
-000129f0: 756d 656e 7420 6f6e 0a20 2020 2020 2020  ument on.       
-00012a00: 2020 2020 2060 6d69 7869 6e2e 436f 6e74       `mixin.Cont
-00012a10: 6169 6e65 7257 6964 6765 742e 696e 6974  ainerWidget.init
-00012a20: 5f63 6f6e 7461 696e 6572 602e 0a0a 2020  _container`...  
-00012a30: 2020 2020 2020 7061 7265 6e74 3a20 5468        parent: Th
-00012a40: 6520 7061 7265 6e74 2077 6964 6765 742e  e parent widget.
-00012a50: 2043 616e 2062 6520 6120 6052 6f6f 7457   Can be a `RootW
-00012a60: 696e 646f 7760 206f 7220 616e 6f74 6865  indow` or anothe
-00012a70: 7220 606d 6978 696e 2e43 6f6e 7461 696e  r `mixin.Contain
-00012a80: 6572 5769 6467 6574 602e 0a0a 2020 2020  erWidget`...    
-00012a90: 416c 6c20 6f74 6865 7220 6172 6775 6d65  All other argume
-00012aa0: 6e74 7320 6172 6520 7061 7373 6564 2074  nts are passed t
-00012ab0: 6f20 7468 6520 6368 696c 6472 656e 2060  o the children `
-00012ac0: 6063 6869 6c64 436c 6173 7360 6020 696e  `childClass`` in
-00012ad0: 766f 6361 7469 6f6e 2e0a 0a20 2020 204e  vocation...    N
-00012ae0: 6f74 653a 0a20 2020 2020 2020 2054 6865  ote:.        The
-00012af0: 2063 6869 6c64 2077 6964 6765 7420 7769   child widget wi
-00012b00: 6c6c 2068 6176 6520 6120 7265 6665 7265  ll have a refere
-00012b10: 6e63 6520 746f 2074 6869 7320 6672 616d  nce to this fram
-00012b20: 652c 2073 6565 2060 6d69 7869 6e2e 5369  e, see `mixin.Si
-00012b30: 6e67 6c65 5769 6467 6574 2e73 6372 6f6c  ngleWidget.scrol
-00012b40: 6c46 7261 6d65 602e 0a0a 2020 2020 5365  lFrame`...    Se
-00012b50: 6520 416c 736f 3a0a 2020 2020 2020 2020  e Also:.        
-00012b60: 5468 6572 6520 6973 2073 6f6d 6520 616e  There is some an
-00012b70: 6369 6c69 6172 7920 5079 7468 6f6e 2064  ciliary Python d
-00012b80: 6f63 756d 656e 7461 7469 6f6e 2069 6e20  ocumentation in 
-00012b90: 6073 6372 6f6c 6c61 626c 6520 7769 6467  `scrollable widg
-00012ba0: 6574 0a20 2020 2020 2020 206f 7074 696f  et.        optio
-00012bb0: 6e73 0a20 2020 2020 2020 203c 6874 7470  ns.        <http
-00012bc0: 733a 2f2f 646f 6373 2e70 7974 686f 6e2e  s://docs.python.
-00012bd0: 6f72 672f 332f 6c69 6272 6172 792f 746b  org/3/library/tk
-00012be0: 696e 7465 722e 7474 6b2e 6874 6d6c 2373  inter.ttk.html#s
-00012bf0: 6372 6f6c 6c61 626c 652d 7769 6467 6574  crollable-widget
-00012c00: 2d6f 7074 696f 6e73 3e60 5f2e 0a0a 2020  -options>`_...  
-00012c10: 2020 2e2e 0a20 2020 2020 2020 2050 7974    ...        Pyt
-00012c20: 686f 6e20 332e 3820 6973 206d 6973 7369  hon 3.8 is missi
-00012c30: 6e67 2074 6869 7320 7265 6665 7265 6e63  ng this referenc
-00012c40: 652c 2069 6e63 6c75 6465 6420 696e 2050  e, included in P
-00012c50: 7974 686f 6e20 332e 393a 0a0a 2020 2020  ython 3.9:..    
-00012c60: 2020 2020 3a72 6566 3a60 7363 726f 6c6c      :ref:`scroll
-00012c70: 6162 6c65 2077 6964 6765 7420 6f70 7469  able widget opti
-00012c80: 6f6e 7320 3c70 7974 686f 6e3a 5363 726f  ons <python:Scro
-00012c90: 6c6c 6162 6c65 2d57 6964 6765 742d 4f70  llable-Widget-Op
-00012ca0: 7469 6f6e 733e 600a 2020 2020 2727 270a  tions>`.    '''.
-00012cb0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00012cc0: 2873 656c 662c 2070 6172 656e 742c 2063  (self, parent, c
-00012cd0: 6869 6c64 436c 6173 733a 2074 7970 696e  hildClass: typin
-00012ce0: 672e 5479 7065 5b6d 6978 696e 2e53 696e  g.Type[mixin.Sin
-00012cf0: 676c 6557 6964 6765 745d 2c0a 2020 2020  gleWidget],.    
-00012d00: 2020 2020 2020 2020 2020 2020 202a 6172               *ar
-00012d10: 6773 2c0a 2020 2020 2020 2020 2020 2020  gs,.            
-00012d20: 2020 2020 2073 6372 6f6c 6c56 6572 7469       scrollVerti
-00012d30: 6361 6c3a 2074 7970 696e 672e 4f70 7469  cal: typing.Opti
-00012d40: 6f6e 616c 5b62 6f6f 6c5d 203d 204e 6f6e  onal[bool] = Non
-00012d50: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00012d60: 2020 2020 7363 726f 6c6c 486f 7269 7a6f      scrollHorizo
-00012d70: 6e74 616c 3a20 7479 7069 6e67 2e4f 7074  ntal: typing.Opt
-00012d80: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f  ional[bool] = No
-00012d90: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00012da0: 2020 2020 2073 6372 6f6c 6c45 7870 616e       scrollExpan
-00012db0: 643a 2062 6f6f 6c20 3d20 5472 7565 2c0a  d: bool = True,.
-00012dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012dd0: 202a 2a63 6b77 6172 6773 293a 0a20 2020   **ckwargs):.   
-00012de0: 2020 2020 2023 2054 6869 7320 6973 2061       # This is a
-00012df0: 2070 726f 7879 206f 626a 6563 742c 2064   proxy object, d
-00012e00: 6f6e 2774 2073 6574 2061 6e79 2075 6e65  on't set any une
-00012e10: 6365 7373 6172 7920 6073 656c 6660 2061  cessary `self` a
-00012e20: 7474 7269 6275 7465 732c 206f 7220 7468  ttributes, or th
-00012e30: 6579 2077 696c 6c20 6f76 6572 7269 6465  ey will override
-00012e40: 2060 6368 696c 6443 6c61 7373 6020 6174   `childClass` at
-00012e50: 7472 6962 7574 6573 0a0a 2020 2020 2020  tributes..      
-00012e60: 2020 2320 4375 7272 656e 7420 4672 616d    # Current Fram
-00012e70: 650a 2020 2020 2020 2020 7375 7065 7228  e.        super(
-00012e80: 292e 5f5f 696e 6974 5f5f 2870 6172 656e  ).__init__(paren
-00012e90: 7429 2020 2320 7474 6b2e 4672 616d 650a  t)  # ttk.Frame.
-00012ea0: 2020 2020 2020 2020 7277 6569 6768 7420          rweight 
-00012eb0: 3d20 5b31 5d0a 2020 2020 2020 2020 6377  = [1].        cw
-00012ec0: 6569 6768 7420 3d20 5b31 5d0a 0a20 2020  eight = [1]..   
-00012ed0: 2020 2020 2023 2057 6964 6765 7420 4865       # Widget He
-00012ee0: 6c70 6572 730a 2020 2020 2020 2020 6465  lpers.        de
-00012ef0: 6620 7363 726f 6c6c 4765 6e43 6f6d 6d61  f scrollGenComma
-00012f00: 6e64 2866 6e3a 2074 7970 696e 672e 4361  nd(fn: typing.Ca
-00012f10: 6c6c 6162 6c65 5b5b 7374 722c 2073 7472  llable[[str, str
-00012f20: 5d2c 204e 6f6e 655d 2c20 7768 793a 2074  ], None], why: t
-00012f30: 7970 696e 672e 4f70 7469 6f6e 616c 5b62  yping.Optional[b
-00012f40: 6f6f 6c5d 2c20 7768 6174 3a20 7374 7229  ool], what: str)
-00012f50: 202d 3e20 7479 7069 6e67 2e43 616c 6c61   -> typing.Calla
-00012f60: 626c 655b 5b73 7472 2c20 7374 725d 2c20  ble[[str, str], 
-00012f70: 4e6f 6e65 5d3a 0a20 2020 2020 2020 2020  None]:.         
-00012f80: 2020 2069 6620 7768 793a 0a20 2020 2020     if why:.     
-00012f90: 2020 2020 2020 2020 2020 2023 2046 6f72             # For
-00012fa0: 6365 2045 6e61 626c 652c 2064 6f6e 2774  ce Enable, don't
-00012fb0: 2063 6861 6e67 6520 7468 6520 7374 6174   change the stat
-00012fc0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00012fd0: 2020 7265 7475 726e 2066 6e0a 2020 2020    return fn.    
-00012fe0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00012ff0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00013000: 4175 746f 6d61 7469 632c 2063 6861 6e67  Automatic, chang
-00013010: 6520 7468 6520 7374 6174 6520 6173 206e  e the state as n
-00013020: 6565 6465 640a 2020 2020 2020 2020 2020  eeded.          
-00013030: 2020 2020 2020 4077 7261 7073 2866 6e29        @wraps(fn)
-00013040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013050: 2064 6566 2073 6372 6f6c 6c47 656e 436f   def scrollGenCo
-00013060: 6d6d 616e 6428 7370 6f73 733a 2073 7472  mmand(sposs: str
-00013070: 2c20 6570 6f73 733a 2073 7472 2920 2d3e  , eposs: str) ->
-00013080: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00013090: 2020 2020 2020 2020 2020 2073 706f 733a             spos:
-000130a0: 2066 6c6f 6174 203d 2066 6c6f 6174 2873   float = float(s
-000130b0: 706f 7373 290a 2020 2020 2020 2020 2020  poss).          
-000130c0: 2020 2020 2020 2020 2020 6570 6f73 3a20            epos: 
-000130d0: 666c 6f61 7420 3d20 666c 6f61 7428 6570  float = float(ep
-000130e0: 6f73 7329 0a20 2020 2020 2020 2020 2020  oss).           
-000130f0: 2020 2020 2020 2020 2061 6c6c 7669 7369           allvisi
-00013100: 626c 653a 2062 6f6f 6c20 3d20 7370 6f73  ble: bool = spos
-00013110: 203d 3d20 302e 3020 616e 6420 6570 6f73   == 0.0 and epos
-00013120: 203d 3d20 312e 300a 2020 2020 2020 2020   == 1.0.        
-00013130: 2020 2020 2020 2020 2020 2020 2320 6966              # if
-00013140: 205f 5f64 6562 7567 5f5f 3a0a 2020 2020   __debug__:.    
-00013150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013160: 2320 2020 2020 6c6f 6767 6572 2e64 6562  #     logger.deb
-00013170: 7567 2827 5363 726f 6c6c 436f 6d6d 616e  ug('ScrollComman
-00013180: 645b 2573 5d3a 205b 2566 202c 2025 665d  d[%s]: [%f , %f]
-00013190: 203d 2025 7327 2c20 7768 6174 2c20 7370   = %s', what, sp
-000131a0: 6f73 2c20 6570 6f73 2c20 616c 6c76 6973  os, epos, allvis
-000131b0: 6962 6c65 290a 2020 2020 2020 2020 2020  ible).          
-000131c0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-000131d0: 6574 5f73 6372 6f6c 6c5f 7374 6174 6528  et_scroll_state(
-000131e0: 2a2a 7b77 6861 743a 206e 6f74 2061 6c6c  **{what: not all
-000131f0: 7669 7369 626c 657d 290a 2020 2020 2020  visible}).      
-00013200: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00013210: 7475 726e 2066 6e28 7370 6f73 732c 2065  turn fn(sposs, e
-00013220: 706f 7373 290a 2020 2020 2020 2020 2020  poss).          
-00013230: 2020 2020 2020 7265 7475 726e 2073 6372        return scr
-00013240: 6f6c 6c47 656e 436f 6d6d 616e 640a 0a20  ollGenCommand.. 
-00013250: 2020 2020 2020 2023 2057 6964 6765 7473         # Widgets
-00013260: 0a20 2020 2020 2020 2073 656c 662e 5f5f  .        self.__
-00013270: 7662 6172 3a20 7479 7069 6e67 2e4f 7074  vbar: typing.Opt
-00013280: 696f 6e61 6c5b 7474 6b2e 5363 726f 6c6c  ional[ttk.Scroll
-00013290: 6261 725d 203d 204e 6f6e 650a 2020 2020  bar] = None.    
-000132a0: 2020 2020 7365 6c66 2e5f 5f68 6261 723a      self.__hbar:
-000132b0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-000132c0: 5b74 746b 2e53 6372 6f6c 6c62 6172 5d20  [ttk.Scrollbar] 
-000132d0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
-000132e0: 656c 662e 5f5f 636f 726e 6572 3a20 7479  elf.__corner: ty
-000132f0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7474  ping.Optional[tt
-00013300: 6b2e 5369 7a65 6772 6970 5d20 3d20 4e6f  k.Sizegrip] = No
-00013310: 6e65 0a20 2020 2020 2020 2069 6620 7363  ne.        if sc
-00013320: 726f 6c6c 486f 7269 7a6f 6e74 616c 2069  rollHorizontal i
-00013330: 6e20 284e 6f6e 652c 2054 7275 6529 3a0a  n (None, True):.
-00013340: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00013350: 2e5f 5f68 6261 7220 3d20 7474 6b2e 5363  .__hbar = ttk.Sc
-00013360: 726f 6c6c 6261 7228 7365 6c66 2c20 6f72  rollbar(self, or
-00013370: 6965 6e74 3d74 6b2e 484f 5249 5a4f 4e54  ient=tk.HORIZONT
-00013380: 414c 290a 2020 2020 2020 2020 2020 2020  AL).            
-00013390: 636b 7761 7267 735b 2778 7363 726f 6c6c  ckwargs['xscroll
-000133a0: 636f 6d6d 616e 6427 5d20 3d20 7363 726f  command'] = scro
-000133b0: 6c6c 4765 6e43 6f6d 6d61 6e64 2873 656c  llGenCommand(sel
-000133c0: 662e 5f5f 6862 6172 2e73 6574 2c20 7363  f.__hbar.set, sc
-000133d0: 726f 6c6c 486f 7269 7a6f 6e74 616c 2c20  rollHorizontal, 
-000133e0: 2768 7374 6174 6527 290a 2020 2020 2020  'hstate').      
-000133f0: 2020 2020 2020 6377 6569 6768 742e 6170        cweight.ap
-00013400: 7065 6e64 2830 290a 2020 2020 2020 2020  pend(0).        
-00013410: 6966 2073 6372 6f6c 6c56 6572 7469 6361  if scrollVertica
-00013420: 6c20 696e 2028 4e6f 6e65 2c20 5472 7565  l in (None, True
-00013430: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-00013440: 656c 662e 5f5f 7662 6172 203d 2074 746b  elf.__vbar = ttk
-00013450: 2e53 6372 6f6c 6c62 6172 2873 656c 662c  .Scrollbar(self,
-00013460: 206f 7269 656e 743d 746b 2e56 4552 5449   orient=tk.VERTI
-00013470: 4341 4c29 0a20 2020 2020 2020 2020 2020  CAL).           
-00013480: 2063 6b77 6172 6773 5b27 7973 6372 6f6c   ckwargs['yscrol
-00013490: 6c63 6f6d 6d61 6e64 275d 203d 2073 6372  lcommand'] = scr
-000134a0: 6f6c 6c47 656e 436f 6d6d 616e 6428 7365  ollGenCommand(se
-000134b0: 6c66 2e5f 5f76 6261 722e 7365 742c 2073  lf.__vbar.set, s
-000134c0: 6372 6f6c 6c56 6572 7469 6361 6c2c 2027  crollVertical, '
-000134d0: 7673 7461 7465 2729 0a20 2020 2020 2020  vstate').       
-000134e0: 2020 2020 2072 7765 6967 6874 2e61 7070       rweight.app
-000134f0: 656e 6428 3029 0a20 2020 2020 2020 2069  end(0).        i
-00013500: 6620 7363 726f 6c6c 5665 7274 6963 616c  f scrollVertical
-00013510: 2069 6e20 284e 6f6e 652c 2054 7275 6529   in (None, True)
-00013520: 2061 6e64 2073 6372 6f6c 6c56 6572 7469   and scrollVerti
-00013530: 6361 6c20 696e 2028 4e6f 6e65 2c20 5472  cal in (None, Tr
-00013540: 7565 293a 0a20 2020 2020 2020 2020 2020  ue):.           
-00013550: 2023 2054 6869 7320 6973 206e 6f74 2073   # This is not s
-00013560: 7472 6963 6c79 206e 6563 6573 7361 7279  tricly necessary
-00013570: 2c20 6275 7420 6e69 6365 2074 6f20 6861  , but nice to ha
-00013580: 7665 2e0a 2020 2020 2020 2020 2020 2020  ve..            
-00013590: 7365 6c66 2e5f 5f63 6f72 6e65 7220 3d20  self.__corner = 
-000135a0: 7474 6b2e 5369 7a65 6772 6970 2873 656c  ttk.Sizegrip(sel
-000135b0: 662c 2063 7572 736f 723d 2727 2c20 7461  f, cursor='', ta
-000135c0: 6b65 666f 6375 733d 4661 6c73 6529 0a20  kefocus=False). 
-000135d0: 2020 2020 2020 2020 2020 2023 2044 6973             # Dis
-000135e0: 6162 6c65 2073 697a 6567 7269 7020 6576  able sizegrip ev
-000135f0: 656e 7473 0a20 2020 2020 2020 2020 2020  ents.           
-00013600: 2073 656c 662e 5f5f 636f 726e 6572 2e62   self.__corner.b
-00013610: 696e 6428 273c 4275 7474 6f6e 2d31 3e27  ind('<Button-1>'
-00013620: 2c20 666e 2e62 696e 6469 6e67 5f64 6973  , fn.binding_dis
-00013630: 6162 6c65 290a 2020 2020 2020 2020 6377  able).        cw
-00013640: 6964 6765 7420 3d20 6368 696c 6443 6c61  idget = childCla
-00013650: 7373 2873 656c 662c 202a 6172 6773 2c20  ss(self, *args, 
-00013660: 2a2a 636b 7761 7267 7329 2020 2320 7479  **ckwargs)  # ty
-00013670: 7065 3a20 6967 6e6f 7265 0a0a 2020 2020  pe: ignore..    
-00013680: 2020 2020 2320 5374 6174 650a 2020 2020      # State.    
-00013690: 2020 2020 7365 6c66 2e73 7461 7465 5f74      self.state_t
-000136a0: 7970 6520 3d20 6377 6964 6765 742e 7374  ype = cwidget.st
-000136b0: 6174 655f 7479 7065 0a20 2020 2020 2020  ate_type.       
-000136c0: 2073 656c 662e 696e 6974 5f73 696e 676c   self.init_singl
-000136d0: 6528 7661 7269 6162 6c65 3d63 7769 6467  e(variable=cwidg
-000136e0: 6574 2e76 6172 6961 626c 6529 0a20 2020  et.variable).   
-000136f0: 2020 2020 2023 2053 7065 6369 616c 2057       # Special W
-00013700: 6964 6765 7420 7374 6174 650a 2020 2020  idget state.    
-00013710: 2020 2020 7365 6c66 2e77 7061 7265 6e74      self.wparent
-00013720: 203d 2070 6172 656e 740a 0a20 2020 2020   = parent..     
-00013730: 2020 2023 2047 6c75 6520 7363 726f 6c6c     # Glue scroll
-00013740: 6261 7273 2077 6974 6820 6368 696c 6420  bars with child 
-00013750: 7769 6467 6574 0a20 2020 2020 2020 2069  widget.        i
-00013760: 6620 7365 6c66 2e5f 5f68 6261 723a 0a20  f self.__hbar:. 
-00013770: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-00013780: 7420 6973 696e 7374 616e 6365 2863 7769  t isinstance(cwi
-00013790: 6467 6574 2c20 746b 2e58 5669 6577 292c  dget, tk.XView),
-000137a0: 2066 2749 6e76 616c 6964 2043 6869 6c64   f'Invalid Child
-000137b0: 2057 6964 6765 743a 207b 6377 6964 6765   Widget: {cwidge
-000137c0: 7421 727d 270a 2020 2020 2020 2020 2020  t!r}'.          
-000137d0: 2020 7365 6c66 2e5f 5f68 6261 725b 2763    self.__hbar['c
-000137e0: 6f6d 6d61 6e64 275d 203d 2063 7769 6467  ommand'] = cwidg
-000137f0: 6574 2e78 7669 6577 0a20 2020 2020 2020  et.xview.       
-00013800: 2069 6620 7365 6c66 2e5f 5f76 6261 723a   if self.__vbar:
-00013810: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-00013820: 6572 7420 6973 696e 7374 616e 6365 2863  ert isinstance(c
-00013830: 7769 6467 6574 2c20 746b 2e59 5669 6577  widget, tk.YView
-00013840: 292c 2066 2749 6e76 616c 6964 2043 6869  ), f'Invalid Chi
-00013850: 6c64 2057 6964 6765 743a 207b 6377 6964  ld Widget: {cwid
-00013860: 6765 7421 727d 270a 2020 2020 2020 2020  get!r}'.        
-00013870: 2020 2020 7365 6c66 2e5f 5f76 6261 725b      self.__vbar[
-00013880: 2763 6f6d 6d61 6e64 275d 203d 2063 7769  'command'] = cwi
-00013890: 6467 6574 2e79 7669 6577 0a0a 2020 2020  dget.yview..    
-000138a0: 2020 2020 2320 4c61 796f 7574 0a20 2020      # Layout.   
-000138b0: 2020 2020 2069 6620 7363 726f 6c6c 4578       if scrollEx
-000138c0: 7061 6e64 3a0a 2020 2020 2020 2020 2020  pand:.          
-000138d0: 2020 7365 6c66 2e67 7269 6428 7374 6963    self.grid(stic
-000138e0: 6b79 3d74 6b2e 4e53 4557 290a 2020 2020  ky=tk.NSEW).    
-000138f0: 2020 2020 6173 7365 7274 2069 7369 6e73      assert isins
-00013900: 7461 6e63 6528 6377 6964 6765 742c 2074  tance(cwidget, t
-00013910: 6b2e 4772 6964 292c 2066 2749 6e76 616c  k.Grid), f'Inval
-00013920: 6964 2043 6869 6c64 2057 6964 6765 743a  id Child Widget:
-00013930: 207b 6377 6964 6765 7421 727d 270a 2020   {cwidget!r}'.  
-00013940: 2020 2020 2020 6377 6964 6765 742e 6772        cwidget.gr
-00013950: 6964 2872 6f77 3d30 2c20 636f 6c75 6d6e  id(row=0, column
-00013960: 3d30 2c20 7374 6963 6b79 3d74 6b2e 4e53  =0, sticky=tk.NS
-00013970: 4557 290a 2020 2020 2020 2020 7365 6c66  EW).        self
-00013980: 2e73 6574 5f73 6372 6f6c 6c5f 7374 6174  .set_scroll_stat
-00013990: 6528 7363 726f 6c6c 486f 7269 7a6f 6e74  e(scrollHorizont
-000139a0: 616c 206f 7220 4e6f 6e65 2c20 7363 726f  al or None, scro
-000139b0: 6c6c 5665 7274 6963 616c 206f 7220 4e6f  llVertical or No
-000139c0: 6e65 290a 2020 2020 2020 2020 2320 456d  ne).        # Em
-000139d0: 756c 6174 6520 6066 6e2e 636f 6e66 6967  ulate `fn.config
-000139e0: 7572 655f 6772 6964 2873 656c 662c 2072  ure_grid(self, r
-000139f0: 7765 6967 6874 2c20 6377 6569 6768 7429  weight, cweight)
-00013a00: 600a 2020 2020 2020 2020 666f 7220 7269  `.        for ri
-00013a10: 6478 2c20 7765 6967 6874 2069 6e20 656e  dx, weight in en
-00013a20: 756d 6572 6174 6528 7277 6569 6768 7429  umerate(rweight)
-00013a30: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00013a40: 6c66 2e72 6f77 636f 6e66 6967 7572 6528  lf.rowconfigure(
-00013a50: 7269 6478 2c20 7765 6967 6874 3d77 6569  ridx, weight=wei
-00013a60: 6768 7429 0a20 2020 2020 2020 2066 6f72  ght).        for
-00013a70: 2063 6964 782c 2077 6569 6768 7420 696e   cidx, weight in
-00013a80: 2065 6e75 6d65 7261 7465 2863 7765 6967   enumerate(cweig
-00013a90: 6874 293a 0a20 2020 2020 2020 2020 2020  ht):.           
-00013aa0: 2073 656c 662e 636f 6c75 6d6e 636f 6e66   self.columnconf
-00013ab0: 6967 7572 6528 6369 6478 2c20 7765 6967  igure(cidx, weig
-00013ac0: 6874 3d77 6569 6768 7429 0a0a 2020 2020  ht=weight)..    
-00013ad0: 2020 2020 2320 5072 6f78 7920 616c 6c20      # Proxy all 
-00013ae0: 6163 6365 7373 2074 6f20 6063 7769 6467  access to `cwidg
-00013af0: 6574 600a 2020 2020 2020 2020 6377 6964  et`.        cwid
-00013b00: 6765 742e 7363 726f 6c6c 4672 616d 6520  get.scrollFrame 
-00013b10: 3d20 7365 6c66 0a20 2020 2020 2020 2073  = self.        s
-00013b20: 656c 662e 7072 6f78 6565 203d 2063 7769  elf.proxee = cwi
-00013b30: 6467 6574 0a0a 2020 2020 6465 6620 6765  dget..    def ge
-00013b40: 745f 7363 726f 6c6c 5f73 7461 7465 2873  t_scroll_state(s
-00013b50: 656c 6629 202d 3e20 7479 7069 6e67 2e54  elf) -> typing.T
-00013b60: 7570 6c65 5b62 6f6f 6c2c 2062 6f6f 6c5d  uple[bool, bool]
-00013b70: 3a0a 2020 2020 2020 2020 2727 2747 6574  :.        '''Get
-00013b80: 2074 6865 2063 7572 7265 6e74 2073 6372   the current scr
-00013b90: 6f6c 6c62 6172 2076 6973 6962 696c 6974  ollbar visibilit
-00013ba0: 7920 7374 6174 652e 0a0a 2020 2020 2020  y state...      
-00013bb0: 2020 4966 2074 6865 2073 6372 6f6c 6c62    If the scrollb
-00013bc0: 6172 2069 7320 636f 6d70 6c65 7465 6c79  ar is completely
-00013bd0: 2064 6973 6162 6c65 642c 2060 4661 6c73   disabled, `Fals
-00013be0: 6560 2069 7320 7265 7475 726e 6564 2e0a  e` is returned..
-00013bf0: 0a20 2020 2020 2020 2054 6869 7320 6973  .        This is
-00013c00: 2061 2074 7570 6c65 2077 6974 6820 7468   a tuple with th
-00013c10: 6520 7374 6174 6520 666f 7220 626f 7468  e state for both
-00013c20: 2073 6372 6f6c 6c62 6172 732c 2068 6f72   scrollbars, hor
-00013c30: 697a 6f6e 7461 6c20 616e 640a 2020 2020  izontal and.    
-00013c40: 2020 2020 7665 7274 6963 616c 2e0a 0a20      vertical... 
-00013c50: 2020 2020 2020 2053 6565 2041 6c73 6f3a         See Also:
-00013c60: 0a20 2020 2020 2020 2020 2020 202d 2060  .            - `
-00013c70: 7365 745f 7363 726f 6c6c 5f73 7461 7465  set_scroll_state
-00013c80: 603a 2043 6861 6e67 6520 7468 6520 6375  `: Change the cu
-00013c90: 7272 656e 7420 7374 6174 650a 2020 2020  rrent state.    
-00013ca0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-00013cb0: 7265 7475 726e 2028 0a20 2020 2020 2020  return (.       
-00013cc0: 2020 2020 2073 656c 662e 5f5f 6862 6172       self.__hbar
-00013cd0: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
-00013ce0: 2062 6f6f 6c28 7365 6c66 2e5f 5f68 6261   bool(self.__hba
-00013cf0: 722e 6772 6964 5f69 6e66 6f28 2929 2c0a  r.grid_info()),.
-00013d00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00013d10: 2e5f 5f76 6261 7220 6973 206e 6f74 204e  .__vbar is not N
-00013d20: 6f6e 6520 616e 6420 626f 6f6c 2873 656c  one and bool(sel
-00013d30: 662e 5f5f 7662 6172 2e67 7269 645f 696e  f.__vbar.grid_in
-00013d40: 666f 2829 292c 0a20 2020 2020 2020 2029  fo()),.        )
-00013d50: 0a0a 2020 2020 6465 6620 7365 745f 7363  ..    def set_sc
-00013d60: 726f 6c6c 5f73 7461 7465 2873 656c 662c  roll_state(self,
-00013d70: 2068 7374 6174 653a 2074 7970 696e 672e   hstate: typing.
-00013d80: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
-00013d90: 204e 6f6e 652c 2076 7374 6174 653a 2074   None, vstate: t
-00013da0: 7970 696e 672e 4f70 7469 6f6e 616c 5b62  yping.Optional[b
-00013db0: 6f6f 6c5d 203d 204e 6f6e 6529 202d 3e20  ool] = None) -> 
-00013dc0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2727  None:.        ''
-00013dd0: 2743 6861 6e67 6520 7468 6520 6375 7272  'Change the curr
-00013de0: 656e 7420 7363 726f 6c6c 6261 7220 7669  ent scrollbar vi
-00013df0: 7369 6269 6c69 7479 2073 7461 7465 2e0a  sibility state..
-00013e00: 0a20 2020 2020 2020 2054 6869 7320 6361  .        This ca
-00013e10: 6e20 6368 616e 6765 2062 6f74 6820 686f  n change both ho
-00013e20: 7269 7a6f 6e74 616c 2061 6e64 2076 6572  rizontal and ver
-00013e30: 7469 6361 6c20 7374 6174 6520 696e 6465  tical state inde
-00013e40: 7065 6e64 656e 746c 792e 2054 6865 0a20  pendently. The. 
-00013e50: 2020 2020 2020 2063 6f72 6e65 7220 7769         corner wi
-00013e60: 6467 6574 2069 7320 6d61 6e61 6765 6420  dget is managed 
-00013e70: 6175 746f 6d61 7469 6361 6c6c 792e 0a0a  automatically...
-00013e80: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00013e90: 2020 2020 2020 2020 2020 6873 7461 7465            hstate
-00013ea0: 3a20 4966 206e 6f74 2060 4e6f 6e65 602c  : If not `None`,
-00013eb0: 2073 6574 2074 6865 2068 6f72 697a 6f6e   set the horizon
-00013ec0: 7461 6c20 7363 726f 6c6c 6261 7220 7669  tal scrollbar vi
-00013ed0: 7369 6269 6c69 7479 2e0a 2020 2020 2020  sibility..      
-00013ee0: 2020 2020 2020 7673 7461 7465 3a20 4966        vstate: If
-00013ef0: 206e 6f74 2060 4e6f 6e65 602c 2073 6574   not `None`, set
-00013f00: 2074 6865 2076 6572 7469 6361 6c20 7363   the vertical sc
-00013f10: 726f 6c6c 6261 7220 7669 7369 6269 6c69  rollbar visibili
-00013f20: 7479 2e0a 0a20 2020 2020 2020 2053 6565  ty...        See
-00013f30: 2041 6c73 6f3a 0a20 2020 2020 2020 2020   Also:.         
-00013f40: 2020 202d 2060 6765 745f 7363 726f 6c6c     - `get_scroll
-00013f50: 5f73 7461 7465 603a 2047 6574 2074 6865  _state`: Get the
-00013f60: 2063 7572 7265 6e74 2073 7461 7465 0a20   current state. 
-00013f70: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-00013f80: 2020 2069 6620 6873 7461 7465 2069 7320     if hstate is 
-00013f90: 6e6f 7420 4e6f 6e65 2061 6e64 2073 656c  not None and sel
-00013fa0: 662e 5f5f 6862 6172 2069 7320 6e6f 7420  f.__hbar is not 
-00013fb0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00013fc0: 2020 6966 2068 7374 6174 653a 0a20 2020    if hstate:.   
-00013fd0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00013fe0: 6e6f 7420 7365 6c66 2e5f 5f68 6261 722e  not self.__hbar.
-00013ff0: 6772 6964 5f69 6e66 6f28 293a 0a20 2020  grid_info():.   
-00014000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014010: 2073 656c 662e 5f5f 6862 6172 2e67 7269   self.__hbar.gri
-00014020: 6428 726f 773d 312c 2063 6f6c 756d 6e3d  d(row=1, column=
-00014030: 302c 2073 7469 636b 793d 746b 2e45 5729  0, sticky=tk.EW)
-00014040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014050: 2020 2020 2069 6620 5f5f 6465 6275 675f       if __debug_
-00014060: 5f3a 0a20 2020 2020 2020 2020 2020 2020  _:.             
-00014070: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-00014080: 722e 6465 6275 6728 2725 733a 2053 686f  r.debug('%s: Sho
-00014090: 7720 6862 6172 272c 2073 656c 6629 0a20  w hbar', self). 
-000140a0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000140b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000140c0: 2069 6620 7365 6c66 2e5f 5f68 6261 722e   if self.__hbar.
-000140d0: 6772 6964 5f69 6e66 6f28 293a 0a20 2020  grid_info():.   
-000140e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000140f0: 2069 6620 5f5f 6465 6275 675f 5f3a 0a20   if __debug__:. 
-00014100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014110: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-00014120: 6275 6728 2725 733a 2048 6964 6520 6862  bug('%s: Hide hb
-00014130: 6172 272c 2073 656c 6629 0a20 2020 2020  ar', self).     
-00014140: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00014150: 656c 662e 5f5f 6862 6172 2e67 7269 645f  elf.__hbar.grid_
-00014160: 7265 6d6f 7665 2829 0a20 2020 2020 2020  remove().       
-00014170: 2069 6620 7673 7461 7465 2069 7320 6e6f   if vstate is no
-00014180: 7420 4e6f 6e65 2061 6e64 2073 656c 662e  t None and self.
-00014190: 5f5f 7662 6172 2069 7320 6e6f 7420 4e6f  __vbar is not No
-000141a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000141b0: 6966 2076 7374 6174 653a 0a20 2020 2020  if vstate:.     
-000141c0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-000141d0: 7420 7365 6c66 2e5f 5f76 6261 722e 6772  t self.__vbar.gr
-000141e0: 6964 5f69 6e66 6f28 293a 0a20 2020 2020  id_info():.     
-000141f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00014200: 656c 662e 5f5f 7662 6172 2e67 7269 6428  elf.__vbar.grid(
-00014210: 726f 773d 302c 2063 6f6c 756d 6e3d 312c  row=0, column=1,
-00014220: 2073 7469 636b 793d 746b 2e4e 5329 0a20   sticky=tk.NS). 
-00014230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014240: 2020 2069 6620 5f5f 6465 6275 675f 5f3a     if __debug__:
-00014250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014260: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-00014270: 6465 6275 6728 2725 733a 2053 686f 7720  debug('%s: Show 
-00014280: 7662 6172 272c 2073 656c 6629 0a20 2020  vbar', self).   
-00014290: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-000142a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000142b0: 6620 7365 6c66 2e5f 5f76 6261 722e 6772  f self.__vbar.gr
-000142c0: 6964 5f69 6e66 6f28 293a 0a20 2020 2020  id_info():.     
-000142d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000142e0: 6620 5f5f 6465 6275 675f 5f3a 0a20 2020  f __debug__:.   
-000142f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014300: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-00014310: 6728 2725 733a 2048 6964 6520 7662 6172  g('%s: Hide vbar
-00014320: 272c 2073 656c 6629 0a20 2020 2020 2020  ', self).       
-00014330: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00014340: 662e 5f5f 7662 6172 2e67 7269 645f 7265  f.__vbar.grid_re
-00014350: 6d6f 7665 2829 0a20 2020 2020 2020 2069  move().        i
-00014360: 6620 7365 6c66 2e5f 5f63 6f72 6e65 7220  f self.__corner 
-00014370: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00014380: 2020 2020 2020 2020 2069 7348 6f72 697a           isHoriz
-00014390: 6f6e 7461 6c20 3d20 7365 6c66 2e5f 5f68  ontal = self.__h
-000143a0: 6261 7220 6973 206e 6f74 204e 6f6e 6520  bar is not None 
-000143b0: 616e 6420 7365 6c66 2e5f 5f68 6261 722e  and self.__hbar.
-000143c0: 6772 6964 5f69 6e66 6f28 290a 2020 2020  grid_info().    
-000143d0: 2020 2020 2020 2020 6973 5665 7274 6963          isVertic
-000143e0: 616c 203d 2073 656c 662e 5f5f 7662 6172  al = self.__vbar
-000143f0: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
-00014400: 2073 656c 662e 5f5f 7662 6172 2e67 7269   self.__vbar.gri
-00014410: 645f 696e 666f 2829 0a20 2020 2020 2020  d_info().       
-00014420: 2020 2020 2069 6620 6973 486f 7269 7a6f       if isHorizo
-00014430: 6e74 616c 2061 6e64 2069 7356 6572 7469  ntal and isVerti
-00014440: 6361 6c3a 0a20 2020 2020 2020 2020 2020  cal:.           
-00014450: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-00014460: 2e5f 5f63 6f72 6e65 722e 6772 6964 5f69  .__corner.grid_i
-00014470: 6e66 6f28 293a 0a20 2020 2020 2020 2020  nfo():.         
-00014480: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00014490: 5f5f 636f 726e 6572 2e67 7269 6428 726f  __corner.grid(ro
-000144a0: 773d 312c 2063 6f6c 756d 6e3d 3129 0a20  w=1, column=1). 
-000144b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000144c0: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-000144d0: 2725 733a 2053 686f 7720 636f 726e 6572  '%s: Show corner
-000144e0: 272c 2073 656c 6629 0a20 2020 2020 2020  ', self).       
-000144f0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00014500: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00014510: 6c66 2e5f 5f63 6f72 6e65 722e 6772 6964  lf.__corner.grid
-00014520: 5f69 6e66 6f28 293a 0a20 2020 2020 2020  _info():.       
-00014530: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-00014540: 6765 722e 6465 6275 6728 2725 733a 2048  ger.debug('%s: H
-00014550: 6964 6520 636f 726e 6572 272c 2073 656c  ide corner', sel
-00014560: 6629 0a20 2020 2020 2020 2020 2020 2020  f).             
-00014570: 2020 2020 2020 2073 656c 662e 5f5f 636f         self.__co
-00014580: 726e 6572 2e67 7269 645f 7265 6d6f 7665  rner.grid_remove
-00014590: 2829 0a0a 2020 2020 6465 6620 5f5f 6765  ()..    def __ge
-000145a0: 7461 7474 725f 5f28 7365 6c66 2c20 6e61  tattr__(self, na
-000145b0: 6d65 293a 0a20 2020 2020 2020 2069 6620  me):.        if 
-000145c0: 7072 6f78 6565 203a 3d20 7365 6c66 2e5f  proxee := self._
-000145d0: 5f64 6963 745f 5f2e 6765 7428 2770 726f  _dict__.get('pro
-000145e0: 7865 6527 2c20 4e6f 6e65 293a 0a20 2020  xee', None):.   
-000145f0: 2020 2020 2020 2020 2023 2050 6f73 742d           # Post-
-00014600: 496e 6974 6961 6c69 7a61 7469 6f6e 0a20  Initialization. 
-00014610: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00014620: 6e20 6765 7461 7474 7228 7072 6f78 6565  n getattr(proxee
-00014630: 2c20 6e61 6d65 290a 2020 2020 2020 2020  , name).        
-00014640: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00014650: 2020 2320 4475 7269 6e67 2060 5f5f 696e    # During `__in
-00014660: 6974 5f5f 600a 2020 2020 2020 2020 2020  it__`.          
-00014670: 2020 7265 7475 726e 206f 626a 6563 742e    return object.
-00014680: 5f5f 6765 7461 7474 725f 5f28 7365 6c66  __getattr__(self
-00014690: 2c20 6e61 6d65 290a 0a20 2020 2064 6566  , name)..    def
-000146a0: 205f 5f73 6574 6174 7472 5f5f 2873 656c   __setattr__(sel
-000146b0: 662c 206e 616d 652c 2076 616c 7565 293a  f, name, value):
-000146c0: 0a20 2020 2020 2020 2069 6620 7072 6f78  .        if prox
-000146d0: 6565 203a 3d20 7365 6c66 2e5f 5f64 6963  ee := self.__dic
-000146e0: 745f 5f2e 6765 7428 2770 726f 7865 6527  t__.get('proxee'
-000146f0: 2c20 4e6f 6e65 293a 0a20 2020 2020 2020  , None):.       
-00014700: 2020 2020 2023 2050 6f73 742d 496e 6974       # Post-Init
-00014710: 6961 6c69 7a61 7469 6f6e 0a20 2020 2020  ialization.     
-00014720: 2020 2020 2020 2073 6574 6174 7472 2870         setattr(p
-00014730: 726f 7865 652c 206e 616d 652c 2076 616c  roxee, name, val
-00014740: 7565 290a 2020 2020 2020 2020 656c 7365  ue).        else
-00014750: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-00014760: 4475 7269 6e67 2060 5f5f 696e 6974 5f5f  During `__init__
-00014770: 600a 2020 2020 2020 2020 2020 2020 6f62  `.            ob
-00014780: 6a65 6374 2e5f 5f73 6574 6174 7472 5f5f  ject.__setattr__
-00014790: 2873 656c 662c 206e 616d 652c 2076 616c  (self, name, val
-000147a0: 7565 290a                                ue).
+00001400: 2020 2020 696d 675f 6675 6e63 7469 6f6e      img_function
+00001410: 203d 206d 6f64 656c 2e49 4d41 4745 5f54   = model.IMAGE_T
+00001420: 5950 4553 5b69 6f62 6a2e 6474 7970 655d  YPES[iobj.dtype]
+00001430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001440: 2020 2020 2069 6d67 5f6b 7761 7267 735b       img_kwargs[
+00001450: 2766 6f72 6d61 7427 5d20 3d20 696f 626a  'format'] = iobj
+00001460: 2e64 7479 7065 0a20 2020 2020 2020 2020  .dtype.         
+00001470: 2020 2020 2020 2023 204c 6f61 6420 7468         # Load th
+00001480: 6520 696d 6167 650a 2020 2020 2020 2020  e image.        
+00001490: 2020 2020 2020 2020 6966 2069 6f62 6a2e          if iobj.
+000014a0: 666e 616d 653a 0a20 2020 2020 2020 2020  fname:.         
+000014b0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+000014c0: 722e 6465 6275 6728 6627 4c6f 6164 2049  r.debug(f'Load I
+000014d0: 6d61 6765 2022 7b6b 6579 7d22 2066 726f  mage "{key}" fro
+000014e0: 6d20 6669 6c65 2022 7b69 6f62 6a2e 666e  m file "{iobj.fn
+000014f0: 616d 657d 2227 290a 2020 2020 2020 2020  ame}"').        
+00001500: 2020 2020 2020 2020 2020 2020 696f 626a              iobj
+00001510: 2e6f 626a 203d 2069 6d67 5f66 756e 6374  .obj = img_funct
+00001520: 696f 6e28 6669 6c65 3d69 6f62 6a2e 666e  ion(file=iobj.fn
+00001530: 616d 652c 202a 2a69 6d67 5f6b 7761 7267  ame, **img_kwarg
+00001540: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
+00001550: 2020 2065 6c69 6620 696f 626a 2e64 6174     elif iobj.dat
+00001560: 613a 0a20 2020 2020 2020 2020 2020 2020  a:.             
+00001570: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+00001580: 6275 6728 6627 4c6f 6164 2049 6d61 6765  bug(f'Load Image
+00001590: 2022 7b6b 6579 7d22 2066 726f 6d20 6461   "{key}" from da
+000015a0: 7461 2729 0a20 2020 2020 2020 2020 2020  ta').           
+000015b0: 2020 2020 2020 2020 2069 6f62 6a2e 6f62           iobj.ob
+000015c0: 6a20 3d20 696d 675f 6675 6e63 7469 6f6e  j = img_function
+000015d0: 2864 6174 613d 696f 626a 2e64 6174 612c  (data=iobj.data,
+000015e0: 202a 2a69 6d67 5f6b 7761 7267 7329 0a20   **img_kwargs). 
+000015f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001600: 2020 2023 2054 4f44 4f3a 2052 656d 6f76     # TODO: Remov
+00001610: 6520 7468 6520 6461 7461 2063 6f70 793a  e the data copy:
+00001620: 2060 696f 626a 2e64 6174 6120 3d20 4e6f   `iobj.data = No
+00001630: 6e65 600a 2020 2020 2020 2020 2020 2020  ne`.            
+00001640: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00001650: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00001660: 6973 6520 5661 6c75 6545 7272 6f72 2866  ise ValueError(f
+00001670: 2749 6e76 616c 6964 2043 6163 6865 204d  'Invalid Cache M
+00001680: 6574 6164 6174 6120 666f 7220 496d 6167  etadata for Imag
+00001690: 6520 7b6b 6579 7d27 290a 2020 2020 2020  e {key}').      
+000016a0: 2020 2020 2020 7265 7475 726e 2069 6f62        return iob
+000016b0: 6a2e 6f62 6a0a 0a20 2020 2064 6566 2069  j.obj..    def i
+000016c0: 6e73 7461 7465 2873 656c 662c 2073 7461  nstate(self, sta
+000016d0: 7465 7370 6563 3a20 7479 7069 6e67 2e53  tespec: typing.S
+000016e0: 6571 7565 6e63 655b 7374 725d 2c20 6361  equence[str], ca
+000016f0: 6c6c 6261 636b 3a20 7479 7069 6e67 2e4f  llback: typing.O
+00001700: 7074 696f 6e61 6c5b 7479 7069 6e67 2e43  ptional[typing.C
+00001710: 616c 6c61 626c 655d 203d 204e 6f6e 6529  allable] = None)
+00001720: 202d 3e20 7479 7069 6e67 2e4f 7074 696f   -> typing.Optio
+00001730: 6e61 6c5b 626f 6f6c 5d3a 0a20 2020 2020  nal[bool]:.     
+00001740: 2020 2027 2727 2727 2720 2023 2044 6f20     ''''''  # Do 
+00001750: 6e6f 7420 646f 6375 6d65 6e74 0a20 2020  not document.   
+00001760: 2020 2020 2023 204e 6f74 2061 7070 6c69       # Not appli
+00001770: 6361 626c 6520 746f 2074 6865 2072 6f6f  cable to the roo
+00001780: 7420 7769 6e64 6f77 0a20 2020 2020 2020  t window.       
+00001790: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
+000017a0: 2020 6465 6620 7374 6174 6528 7365 6c66    def state(self
+000017b0: 2c20 7374 6174 6573 7065 6329 3a0a 2020  , statespec):.  
+000017c0: 2020 2020 2020 2727 2727 2727 2020 2320        ''''''  # 
+000017d0: 446f 206e 6f74 2064 6f63 756d 656e 740a  Do not document.
+000017e0: 2020 2020 2020 2020 2320 4e6f 7420 6170          # Not ap
+000017f0: 706c 6963 6162 6c65 2074 6f20 726f 6f74  plicable to root
+00001800: 2077 696e 646f 770a 2020 2020 2020 2020   window.        
+00001810: 7261 6973 6520 4e6f 7449 6d70 6c65 6d65  raise NotImpleme
+00001820: 6e74 6564 4572 726f 720a 0a20 2020 2064  ntedError..    d
+00001830: 6566 2067 6269 6e64 696e 6728 7365 6c66  ef gbinding(self
+00001840: 2c20 2a61 7267 732c 2069 6d6d 6564 6961  , *args, immedia
+00001850: 7465 3a20 626f 6f6c 203d 2054 7275 652c  te: bool = True,
+00001860: 202a 2a6b 7761 7267 7329 202d 3e20 6d6f   **kwargs) -> mo
+00001870: 6465 6c2e 4269 6e64 696e 6747 6c6f 6261  del.BindingGloba
+00001880: 6c3a 0a20 2020 2020 2020 2027 2727 4372  l:.        '''Cr
+00001890: 6561 7465 2061 2060 6d6f 6465 6c2e 4269  eate a `model.Bi
+000018a0: 6e64 696e 6747 6c6f 6261 6c60 2066 6f72  ndingGlobal` for
+000018b0: 2074 6869 7320 6170 706c 6963 6174 696f   this applicatio
+000018c0: 6e2e 0a0a 2020 2020 2020 2020 4172 6773  n...        Args
+000018d0: 3a0a 2020 2020 2020 2020 2020 2020 696d  :.            im
+000018e0: 6d65 6469 6174 653a 2050 6173 7365 6420  mediate: Passed 
+000018f0: 746f 2074 6865 2075 7073 7472 6561 6d20  to the upstream 
+00001900: 6f62 6a65 6374 2c20 6465 6661 756c 7420  object, default 
+00001910: 746f 2065 6e61 626c 696e 6720 7468 650a  to enabling the.
+00001920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001930: 6269 6e64 696e 6720 6f6e 2063 7265 6174  binding on creat
+00001940: 696f 6e2e 2054 6869 7320 6973 2074 6865  ion. This is the
+00001950: 206f 7070 6f73 6974 6520 6672 6f6d 2075   opposite from u
+00001960: 7073 7472 6561 6d2e 0a0a 2020 2020 2020  pstream...      
+00001970: 2020 416c 6c20 6172 6775 6d65 6e74 7320    All arguments 
+00001980: 6172 6520 7061 7373 6564 2074 6f20 7468  are passed to th
+00001990: 6520 606d 6f64 656c 2e42 696e 6469 6e67  e `model.Binding
+000019a0: 476c 6f62 616c 6020 6f62 6a65 6374 2e0a  Global` object..
+000019b0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+000019c0: 2020 2020 7265 7475 726e 206d 6f64 656c      return model
+000019d0: 2e42 696e 6469 6e67 476c 6f62 616c 2873  .BindingGlobal(s
+000019e0: 656c 662c 202a 6172 6773 2c20 696d 6d65  elf, *args, imme
+000019f0: 6469 6174 653d 696d 6d65 6469 6174 652c  diate=immediate,
+00001a00: 202a 2a6b 7761 7267 7329 0a0a 2020 2020   **kwargs)..    
+00001a10: 6465 6620 7365 7475 705f 696d 6167 655f  def setup_image_
+00001a20: 6461 7461 2873 656c 662c 206b 6579 3a20  data(self, key: 
+00001a30: 7374 722c 2064 6174 613a 2062 7974 6573  str, data: bytes
+00001a40: 2c20 6474 7970 653a 2073 7472 2c20 2a2c  , dtype: str, *,
+00001a50: 2063 6163 6865 5f63 6c65 6172 3a20 626f   cache_clear: bo
+00001a60: 6f6c 203d 2054 7275 6529 202d 3e20 4e6f  ol = True) -> No
+00001a70: 6e65 3a0a 2020 2020 2020 2020 2727 2752  ne:.        '''R
+00001a80: 6567 6973 7465 7220 6120 7369 6e67 6c65  egister a single
+00001a90: 2069 6d61 6765 2c20 6672 6f6d 2061 7262   image, from arb
+00001aa0: 6974 7261 7279 2064 6174 612e 0a0a 2020  itrary data...  
+00001ab0: 2020 2020 2020 5468 6973 2069 7320 7573        This is us
+00001ac0: 6566 756c 2074 6f20 6176 6f69 6420 6578  eful to avoid ex
+00001ad0: 7465 726e 616c 2069 6d61 6765 2066 696c  ternal image fil
+00001ae0: 6573 2061 6e64 2068 6172 6463 6f64 6520  es and hardcode 
+00001af0: 616c 6c20 696d 6167 650a 2020 2020 2020  all image.      
+00001b00: 2020 6461 7461 206f 6e20 7468 6520 6269    data on the bi
+00001b10: 6e61 7279 2069 7473 656c 662e 0a0a 2020  nary itself...  
+00001b20: 2020 2020 2020 5468 6520 6461 7461 2063        The data c
+00001b30: 616e 2062 6520 6769 7665 6e20 6173 2061  an be given as a
+00001b40: 2062 6173 6536 3420 6279 7465 2073 7472   base64 byte str
+00001b50: 696e 672e 2054 6869 7320 6361 6e20 6265  ing. This can be
+00001b60: 2063 6f6d 7075 7465 640a 2020 2020 2020   computed.      
+00001b70: 2020 6672 6f6d 2061 2066 696c 6520 6060    from a file ``
+00001b80: 2449 4d41 4745 6060 2075 7369 6e67 2074  $IMAGE`` using t
+00001b90: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
+00001ba0: 6d61 6e64 0a0a 2020 2020 2020 2020 2e2e  mand..        ..
+00001bb0: 2063 6f64 653a 3a20 7368 656c 6c0a 0a20   code:: shell.. 
+00001bc0: 2020 2020 2020 2020 2020 2062 6173 6536             base6
+00001bd0: 3420 2d2d 7772 6170 3d30 203c 2224 494d  4 --wrap=0 <"$IM
+00001be0: 4147 4522 0a0a 2020 2020 2020 2020 4172  AGE"..        Ar
+00001bf0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00001c00: 6b65 793a 2054 6865 206b 6579 2074 6f20  key: The key to 
+00001c10: 7374 6f72 6520 7468 6520 696d 6167 6520  store the image 
+00001c20: 756e 6465 720a 2020 2020 2020 2020 2020  under.          
+00001c30: 2020 6461 7461 3a20 5468 6520 696d 6167    data: The imag
+00001c40: 6520 6461 7461 2c20 6173 2062 7974 6573  e data, as bytes
+00001c50: 2e0a 2020 2020 2020 2020 2020 2020 6474  ..            dt
+00001c60: 7970 653a 2054 6865 2069 6d61 6765 2066  ype: The image f
+00001c70: 6f72 6d61 742e 204f 6e6c 7920 6074 6b69  ormat. Only `tki
+00001c80: 6e74 6572 6020 7375 7070 6f72 7465 6420  nter` supported 
+00001c90: 696d 6167 6573 2e0a 0a20 2020 2020 2020  images...       
+00001ca0: 2020 2020 2063 6163 6865 5f63 6c65 6172       cache_clear
+00001cb0: 3a20 436c 6561 7220 7468 6520 696d 6167  : Clear the imag
+00001cc0: 6520 6361 6368 6520 6166 7465 7220 7265  e cache after re
+00001cd0: 6769 7374 6572 2074 6865 7365 206e 6577  gister these new
+00001ce0: 2069 6d61 6765 2e0a 2020 2020 2020 2020   image..        
+00001cf0: 2020 2020 2020 2020 4465 6661 756c 7420          Default 
+00001d00: 746f 2060 5472 7565 602e 0a0a 2020 2020  to `True`...    
+00001d10: 2020 2020 5365 6520 416c 736f 3a0a 2020      See Also:.  
+00001d20: 2020 2020 2020 2020 2020 2d20 6073 6574            - `set
+00001d30: 7570 5f69 6d61 6765 735f 666f 6c64 6572  up_images_folder
+00001d40: 603a 2052 6567 6973 7465 7220 7365 7665  `: Register seve
+00001d50: 7261 6c20 696d 6167 6573 2066 726f 6d20  ral images from 
+00001d60: 6120 666f 6c64 6572 2e0a 2020 2020 2020  a folder..      
+00001d70: 2020 2020 2020 2d20 6077 696d 6167 6560        - `wimage`
+00001d80: 3a20 4765 7420 7468 6520 6c6f 6164 6564  : Get the loaded
+00001d90: 2069 6d61 6765 2064 6174 612e 0a20 2020   image data..   
+00001da0: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00001db0: 2069 6620 6b65 7920 696e 2073 656c 662e   if key in self.
+00001dc0: 696d 6167 6573 5f63 6163 6865 3a0a 2020  images_cache:.  
+00001dd0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00001de0: 6578 6365 7074 696f 6e2e 496e 7661 6c69  exception.Invali
+00001df0: 6449 6d61 6765 4b65 7928 6b65 7929 0a20  dImageKey(key). 
+00001e00: 2020 2020 2020 2069 6620 6474 7970 6520         if dtype 
+00001e10: 6e6f 7420 696e 206d 6f64 656c 2e49 4d41  not in model.IMA
+00001e20: 4745 5f54 5950 4553 3a0a 2020 2020 2020  GE_TYPES:.      
+00001e30: 2020 2020 2020 7261 6973 6520 6578 6365        raise exce
+00001e40: 7074 696f 6e2e 496e 7661 6c69 6449 6d61  ption.InvalidIma
+00001e50: 6765 5479 7065 2864 7479 7065 290a 2020  geType(dtype).  
+00001e60: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+00001e70: 7567 2866 2752 6567 6973 7465 7220 7b64  ug(f'Register {d
+00001e80: 7479 7065 2e75 7070 6572 2829 7d20 496d  type.upper()} Im
+00001e90: 6167 6520 227b 6b65 797d 2227 290a 2020  age "{key}"').  
+00001ea0: 2020 2020 2020 7365 6c66 2e69 6d61 6765        self.image
+00001eb0: 735f 6361 6368 655b 6b65 795d 203d 206d  s_cache[key] = m
+00001ec0: 6f64 656c 2e49 6d61 6765 4361 6368 6528  odel.ImageCache(
+00001ed0: 6461 7461 3d64 6174 612c 2064 7479 7065  data=data, dtype
+00001ee0: 3d64 7479 7065 290a 2020 2020 2020 2020  =dtype).        
+00001ef0: 6966 2063 6163 6865 5f63 6c65 6172 3a0a  if cache_clear:.
+00001f00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00001f10: 2e77 696d 6167 652e 6361 6368 655f 636c  .wimage.cache_cl
+00001f20: 6561 7228 290a 0a20 2020 2023 2054 4f44  ear()..    # TOD
+00001f30: 4f3a 2053 7570 706f 7274 206c 6f61 6469  O: Support loadi
+00001f40: 6e67 2061 6c6c 2069 6d61 6765 7320 7269  ng all images ri
+00001f50: 6768 7420 6865 7265 2c20 6e6f 206c 617a  ght here, no laz
+00001f60: 7920 6c6f 6164 696e 673f 0a20 2020 2023  y loading?.    #
+00001f70: 2054 4f44 4f3a 2041 6363 6570 7420 6d75   TODO: Accept mu
+00001f80: 6c74 6970 6c65 2066 6f72 6d61 7473 2028  ltiple formats (
+00001f90: 606d 6f64 656c 2e49 4d41 4745 5f54 5950  `model.IMAGE_TYP
+00001fa0: 4553 6029 2c20 6279 2074 6861 7420 6f72  ES`), by that or
+00001fb0: 6465 7220 2866 6972 7374 2077 696e 7329  der (first wins)
+00001fc0: 0a20 2020 2064 6566 2073 6574 7570 5f69  .    def setup_i
+00001fd0: 6d61 6765 735f 666f 6c64 6572 2873 656c  mages_folder(sel
+00001fe0: 662c 2066 6f6c 6465 723a 2050 6174 682c  f, folder: Path,
+00001ff0: 202a 2c20 6361 6368 655f 636c 6561 723a   *, cache_clear:
+00002000: 2062 6f6f 6c20 3d20 5472 7565 2920 2d3e   bool = True) ->
+00002010: 204e 6f6e 653a 0a20 2020 2020 2020 2027   None:.        '
+00002020: 2727 5265 6769 7374 6572 2061 6c6c 2073  ''Register all s
+00002030: 7570 706f 7274 6564 2069 6d61 6765 7320  upported images 
+00002040: 6672 6f6d 2061 2066 6f6c 6465 722e 0a0a  from a folder...
+00002050: 2020 2020 2020 2020 5265 6769 7374 6572          Register
+00002060: 7320 616c 6c20 7375 7070 6f72 7465 6420  s all supported 
+00002070: 696d 6167 6573 206f 6e20 7468 6520 6769  images on the gi
+00002080: 7665 6e20 666f 6c64 6572 2c20 646f 6573  ven folder, does
+00002090: 206e 6f74 2072 6563 7572 7365 0a20 2020   not recurse.   
+000020a0: 2020 2020 2069 6e74 6f20 7375 6266 6f6c       into subfol
+000020b0: 6465 7273 2e20 556e 7375 7070 6f72 7465  ders. Unsupporte
+000020c0: 6420 6669 6c65 2065 7874 656e 7369 6f6e  d file extension
+000020d0: 7320 6172 6520 736b 6970 7065 642e 0a0a  s are skipped...
+000020e0: 2020 2020 2020 2020 5468 6520 6b65 7920          The key 
+000020f0: 666f 7220 6669 6e64 696e 6720 7468 6520  for finding the 
+00002100: 696d 6167 6573 2069 7320 7468 6520 6669  images is the fi
+00002110: 6c65 206e 616d 652c 2077 6974 686f 7574  le name, without
+00002120: 2074 6865 206c 6173 740a 2020 2020 2020   the last.      
+00002130: 2020 6578 7465 6e73 696f 6e2e 204d 756c    extension. Mul
+00002140: 7469 706c 6520 696d 6167 6573 2077 6974  tiple images wit
+00002150: 6820 7468 6520 7361 6d65 206b 6579 2061  h the same key a
+00002160: 6e64 2064 6966 6665 7265 6e74 2065 7874  nd different ext
+00002170: 656e 7369 6f6e 730a 2020 2020 2020 2020  ensions.        
+00002180: 6172 6520 756e 7375 7070 6f72 7465 642e  are unsupported.
+00002190: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+000021a0: 2020 2020 2020 2020 2020 2020 666f 6c64              fold
+000021b0: 6572 3a20 5468 6520 736f 7572 6365 2066  er: The source f
+000021c0: 6f6c 6465 722e 204f 7074 696f 6e61 6c2e  older. Optional.
+000021d0: 0a20 2020 2020 2020 2020 2020 2063 6163  .            cac
+000021e0: 6865 5f63 6c65 6172 3a20 436c 6561 7220  he_clear: Clear 
+000021f0: 7468 6520 696d 6167 6520 6361 6368 6520  the image cache 
+00002200: 6166 7465 7220 7265 6769 7374 6572 2074  after register t
+00002210: 6865 7365 206e 6577 2069 6d61 6765 732e  hese new images.
+00002220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002230: 2044 6566 6175 6c74 2074 6f20 6054 7275   Default to `Tru
+00002240: 6560 2e0a 0a20 2020 2020 2020 2053 6565  e`...        See
+00002250: 2041 6c73 6f3a 0a20 2020 2020 2020 2020   Also:.         
+00002260: 2020 202d 2060 7365 7475 705f 696d 6167     - `setup_imag
+00002270: 655f 6461 7461 603a 2052 6567 6973 7465  e_data`: Registe
+00002280: 7220 6120 7369 6e67 6c65 2069 6d61 6765  r a single image
+00002290: 2066 726f 6d20 7261 7720 6461 7461 2e0a   from raw data..
+000022a0: 2020 2020 2020 2020 2020 2020 2d20 6077              - `w
+000022b0: 696d 6167 6560 3a20 4765 7420 7468 6520  image`: Get the 
+000022c0: 6c6f 6164 6564 2069 6d61 6765 2064 6174  loaded image dat
+000022d0: 612e 0a20 2020 2020 2020 2027 2727 0a20  a..        '''. 
+000022e0: 2020 2020 2020 2069 6620 6e6f 7420 666f         if not fo
+000022f0: 6c64 6572 2e69 735f 6469 7228 293a 0a20  lder.is_dir():. 
+00002300: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00002310: 2056 616c 7565 4572 726f 7228 6627 496e   ValueError(f'In
+00002320: 7661 6c69 6420 466f 6c64 6572 3a20 7b66  valid Folder: {f
+00002330: 6f6c 6465 727d 2729 0a20 2020 2020 2020  older}').       
+00002340: 2066 6f72 2069 6d67 6669 6c65 2069 6e20   for imgfile in 
+00002350: 666f 6c64 6572 2e69 7465 7264 6972 2829  folder.iterdir()
+00002360: 3a0a 2020 2020 2020 2020 2020 2020 696d  :.            im
+00002370: 6765 7874 203d 2069 6d67 6669 6c65 2e73  gext = imgfile.s
+00002380: 7566 6669 780a 2020 2020 2020 2020 2020  uffix.          
+00002390: 2020 6474 7970 6520 3d20 4e6f 6e65 2069    dtype = None i
+000023a0: 6620 696d 6765 7874 203d 3d20 2727 2065  f imgext == '' e
+000023b0: 6c73 6520 696d 6765 7874 5b31 3a5d 2e6c  lse imgext[1:].l
+000023c0: 6f77 6572 2829 0a20 2020 2020 2020 2020  ower().         
+000023d0: 2020 2069 6620 696d 6766 696c 652e 6973     if imgfile.is
+000023e0: 5f66 696c 6528 2920 616e 6420 6474 7970  _file() and dtyp
+000023f0: 6520 696e 206d 6f64 656c 2e49 4d41 4745  e in model.IMAGE
+00002400: 5f54 5950 4553 3a0a 2020 2020 2020 2020  _TYPES:.        
+00002410: 2020 2020 2020 2020 696d 676b 6579 203d          imgkey =
+00002420: 2069 6d67 6669 6c65 2e73 7465 6d0a 2020   imgfile.stem.  
+00002430: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00002440: 6767 6572 2e64 6562 7567 2866 2752 6567  gger.debug(f'Reg
+00002450: 6973 7465 7220 7b64 7479 7065 2e75 7070  ister {dtype.upp
+00002460: 6572 2829 7d20 496d 6167 6520 227b 696d  er()} Image "{im
+00002470: 676b 6579 7d22 3a20 227b 696d 6766 696c  gkey}": "{imgfil
+00002480: 657d 2227 290a 2020 2020 2020 2020 2020  e}"').          
+00002490: 2020 2020 2020 6966 2069 6d67 6b65 7920        if imgkey 
+000024a0: 696e 2073 656c 662e 696d 6167 6573 5f63  in self.images_c
+000024b0: 6163 6865 3a0a 2020 2020 2020 2020 2020  ache:.          
+000024c0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000024d0: 6578 6365 7074 696f 6e2e 496e 7661 6c69  exception.Invali
+000024e0: 6449 6d61 6765 4b65 7928 696d 676b 6579  dImageKey(imgkey
+000024f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00002500: 2020 6966 2064 7479 7065 206e 6f74 2069    if dtype not i
+00002510: 6e20 6d6f 6465 6c2e 494d 4147 455f 5459  n model.IMAGE_TY
+00002520: 5045 533a 0a20 2020 2020 2020 2020 2020  PES:.           
+00002530: 2020 2020 2020 2020 2072 6169 7365 2065           raise e
+00002540: 7863 6570 7469 6f6e 2e49 6e76 616c 6964  xception.Invalid
+00002550: 496d 6167 6554 7970 6528 6474 7970 6529  ImageType(dtype)
+00002560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002570: 2073 656c 662e 696d 6167 6573 5f63 6163   self.images_cac
+00002580: 6865 5b69 6d67 6b65 795d 203d 206d 6f64  he[imgkey] = mod
+00002590: 656c 2e49 6d61 6765 4361 6368 6528 666e  el.ImageCache(fn
+000025a0: 616d 653d 696d 6766 696c 652c 2064 7479  ame=imgfile, dty
+000025b0: 7065 3d64 7479 7065 290a 2020 2020 2020  pe=dtype).      
+000025c0: 2020 6966 2063 6163 6865 5f63 6c65 6172    if cache_clear
+000025d0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000025e0: 6c66 2e77 696d 6167 652e 6361 6368 655f  lf.wimage.cache_
+000025f0: 636c 6561 7228 290a 0a0a 636c 6173 7320  clear()...class 
+00002600: 4672 616d 6555 6e6c 6162 656c 6c65 6428  FrameUnlabelled(
+00002610: 7474 6b2e 4672 616d 652c 206d 6978 696e  ttk.Frame, mixin
+00002620: 2e43 6f6e 7461 696e 6572 5769 6467 6574  .ContainerWidget
+00002630: 293a 0a20 2020 2027 2727 4120 7369 6d70  ):.    '''A simp
+00002640: 6c65 2066 7261 6d65 2074 6f20 686f 6c64  le frame to hold
+00002650: 206f 7468 6572 2077 6964 6765 7473 2c20   other widgets, 
+00002660: 7669 7375 616c 6c79 2069 6e76 6973 6962  visually invisib
+00002670: 6c65 2e0a 0a20 2020 2054 6869 7320 6973  le...    This is
+00002680: 2074 6865 2073 696d 706c 6573 7420 666f   the simplest fo
+00002690: 726d 206f 6620 606d 6978 696e 2e43 6f6e  rm of `mixin.Con
+000026a0: 7461 696e 6572 5769 6467 6574 602c 206a  tainerWidget`, j
+000026b0: 7573 7420 6120 6275 6e63 6820 6f66 0a20  ust a bunch of. 
+000026c0: 2020 2077 6964 6765 7473 2e20 5468 6572     widgets. Ther
+000026d0: 6527 7320 6e6f 2073 6570 6172 6174 696f  e's no separatio
+000026e0: 6e20 6265 7477 6565 6e20 7468 6520 6f75  n between the ou
+000026f0: 7473 6964 6520 616e 6420 7468 6520 696e  tside and the in
+00002700: 7369 6465 206f 6620 7468 650a 2020 2020  side of the.    
+00002710: 6672 616d 652e 0a0a 2020 2020 5468 6572  frame...    Ther
+00002720: 6520 6973 206e 6f20 5079 7468 6f6e 2064  e is no Python d
+00002730: 6f63 756d 656e 7461 7469 6f6e 2c20 7365  ocumentation, se
+00002740: 6520 6060 546b 6060 2060 7474 6b2e 4672  e ``Tk`` `ttk.Fr
+00002750: 616d 6520 3c68 7474 7073 3a2f 2f77 7777  ame <https://www
+00002760: 2e74 636c 2e74 6b2f 6d61 6e2f 7463 6c2f  .tcl.tk/man/tcl/
+00002770: 546b 436d 642f 7474 6b5f 6672 616d 652e  TkCmd/ttk_frame.
+00002780: 6874 6d6c 3e60 5f20 646f 6375 6d65 6e74  html>`_ document
+00002790: 6174 696f 6e2e 0a0a 2020 2020 4172 6773  ation...    Args
+000027a0: 3a0a 2020 2020 2020 2020 7061 7265 6e74  :.        parent
+000027b0: 3a20 5468 6520 7061 7265 6e74 2077 6964  : The parent wid
+000027c0: 6765 742e 2043 616e 2062 6520 6120 6052  get. Can be a `R
+000027d0: 6f6f 7457 696e 646f 7760 206f 7220 616e  ootWindow` or an
+000027e0: 6f74 6865 7220 606d 6978 696e 2e43 6f6e  other `mixin.Con
+000027f0: 7461 696e 6572 5769 6467 6574 602e 0a0a  tainerWidget`...
+00002800: 2020 2020 5365 6520 416c 736f 3a0a 2020      See Also:.  
+00002810: 2020 2020 2020 6046 7261 6d65 4c61 6265        `FrameLabe
+00002820: 6c6c 6564 603a 2056 6973 6962 6c65 2076  lled`: Visible v
+00002830: 6572 7369 6f6e 2c20 7769 7468 2061 206c  ersion, with a l
+00002840: 6162 656c 2e0a 2020 2020 2727 270a 2020  abel..    '''.  
+00002850: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+00002860: 656c 662c 2070 6172 656e 742c 202a 6172  elf, parent, *ar
+00002870: 6773 2c20 2a2a 6b77 6172 6773 293a 0a20  gs, **kwargs):. 
+00002880: 2020 2020 2020 2073 7570 6572 2829 2e5f         super()._
+00002890: 5f69 6e69 745f 5f28 7061 7265 6e74 2920  _init__(parent) 
+000028a0: 2023 2074 746b 2e46 7261 6d65 0a20 2020   # ttk.Frame.   
+000028b0: 2020 2020 2073 656c 662e 696e 6974 5f63       self.init_c
+000028c0: 6f6e 7461 696e 6572 282a 6172 6773 2c20  ontainer(*args, 
+000028d0: 2a2a 6b77 6172 6773 290a 0a0a 636c 6173  **kwargs)...clas
+000028e0: 7320 4672 616d 654c 6162 656c 6c65 6428  s FrameLabelled(
+000028f0: 7474 6b2e 4c61 6265 6c46 7261 6d65 2c20  ttk.LabelFrame, 
+00002900: 6d69 7869 6e2e 436f 6e74 6169 6e65 7257  mixin.ContainerW
+00002910: 6964 6765 7429 3a0a 2020 2020 2727 2741  idget):.    '''A
+00002920: 2066 7261 6d65 2074 6f20 686f 6c64 206f   frame to hold o
+00002930: 7468 6572 2077 6964 6765 7473 2073 7572  ther widgets sur
+00002940: 726f 756e 6465 6420 6279 2061 206c 696e  rounded by a lin
+00002950: 652c 2069 6e63 6c75 6469 6e67 2061 206c  e, including a l
+00002960: 6162 656c 2e0a 0a20 2020 2054 6869 7320  abel...    This 
+00002970: 6973 2061 2066 7261 6d65 2077 6974 6820  is a frame with 
+00002980: 6120 6c61 6265 6c2e 2049 7420 6973 2076  a label. It is v
+00002990: 6973 7561 6c6c 7920 7365 7061 7261 7465  isually separate
+000029a0: 6420 6672 6f6d 2074 6865 206f 7468 6572  d from the other
+000029b0: 0a20 2020 2077 6964 6765 7473 2e20 596f  .    widgets. Yo
+000029c0: 7520 6361 6e20 636f 6e74 726f 6c20 7468  u can control th
+000029d0: 6520 6c61 6265 6c20 706f 7369 7469 6f6e  e label position
+000029e0: 2e0a 0a20 2020 2054 6865 7265 2069 7320  ...    There is 
+000029f0: 6e6f 2050 7974 686f 6e20 646f 6375 6d65  no Python docume
+00002a00: 6e74 6174 696f 6e2c 2073 6565 2060 6054  ntation, see ``T
+00002a10: 6b60 6020 6074 746b 2e4c 6162 656c 4672  k`` `ttk.LabelFr
+00002a20: 616d 6520 3c68 7474 7073 3a2f 2f77 7777  ame <https://www
+00002a30: 2e74 636c 2e74 6b2f 6d61 6e2f 7463 6c2f  .tcl.tk/man/tcl/
+00002a40: 546b 436d 642f 7474 6b5f 6c61 6265 6c66  TkCmd/ttk_labelf
+00002a50: 7261 6d65 2e68 746d 6c3e 605f 2064 6f63  rame.html>`_ doc
+00002a60: 756d 656e 7461 7469 6f6e 2e0a 0a20 2020  umentation...   
+00002a70: 2041 7267 733a 0a20 2020 2020 2020 206c   Args:.        l
+00002a80: 6162 656c 3a20 5468 6520 6c61 6265 6c20  abel: The label 
+00002a90: 746f 2069 6e63 6c75 6465 206f 6e20 7468  to include on th
+00002aa0: 6520 6672 616d 6520 7365 7061 7261 746f  e frame separato
+00002ab0: 722e 2043 616e 2062 6520 6769 7665 6e20  r. Can be given 
+00002ac0: 6173 2061 2063 6c61 7373 2076 6172 6961  as a class varia
+00002ad0: 626c 652e 0a20 2020 2020 2020 206c 6162  ble..        lab
+00002ae0: 656c 416e 6368 6f72 3a20 5468 6520 706f  elAnchor: The po
+00002af0: 7369 7469 6f6e 206f 6620 7468 6520 6c61  sition of the la
+00002b00: 6265 6c20 6f6e 2074 6865 2066 7261 6d65  bel on the frame
+00002b10: 2073 6570 6172 6174 6f72 2e0a 2020 2020   separator..    
+00002b20: 2020 2020 2020 2020 4769 7665 6e20 6173          Given as
+00002b30: 206f 6e65 206f 6620 7468 6520 6361 7264   one of the card
+00002b40: 696e 616c 2070 6f69 6e74 732e 0a20 2020  inal points..   
+00002b50: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
+00002b60: 7320 746f 2061 204f 532d 7370 6563 6966  s to a OS-specif
+00002b70: 6963 206c 6f63 6174 696f 6e20 2860 6d6f  ic location (`mo
+00002b80: 6465 6c2e 4350 2e64 6566 6175 6c74 6029  del.CP.default`)
+00002b90: 2e0a 0a20 2020 2020 2020 2070 6172 656e  ...        paren
+00002ba0: 743a 2054 6865 2070 6172 656e 7420 7769  t: The parent wi
+00002bb0: 6467 6574 2e20 4361 6e20 6265 2061 2060  dget. Can be a `
+00002bc0: 526f 6f74 5769 6e64 6f77 6020 6f72 2061  RootWindow` or a
+00002bd0: 6e6f 7468 6572 2060 6d69 7869 6e2e 436f  nother `mixin.Co
+00002be0: 6e74 6169 6e65 7257 6964 6765 7460 2e0a  ntainerWidget`..
+00002bf0: 0a20 2020 2053 6565 2041 6c73 6f3a 0a20  .    See Also:. 
+00002c00: 2020 2020 2020 2060 4672 616d 6555 6e6c         `FrameUnl
+00002c10: 6162 656c 6c65 6460 3a20 496e 7669 7369  abelled`: Invisi
+00002c20: 626c 6520 7665 7273 696f 6e2c 2077 6974  ble version, wit
+00002c30: 686f 7574 2061 206c 6162 656c 2e0a 0a20  hout a label... 
+00002c40: 2020 2020 2020 2060 4672 616d 6553 7461         `FrameSta
+00002c50: 7465 6675 6c60 3a20 5375 7070 6f72 7420  teful`: Support 
+00002c60: 666f 7220 616e 2065 6d62 6564 6465 6420  for an embedded 
+00002c70: 6043 6865 636b 626f 7860 2061 7320 6c61  `Checkbox` as la
+00002c80: 6265 6c2e 0a20 2020 2027 2727 0a20 2020  bel..    '''.   
+00002c90: 206c 6162 656c 3a20 7479 7069 6e67 2e4f   label: typing.O
+00002ca0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00002cb0: 6f6e 650a 0a20 2020 2064 6566 205f 5f69  one..    def __i
+00002cc0: 6e69 745f 5f28 7365 6c66 2c20 7061 7265  nit__(self, pare
+00002cd0: 6e74 2c20 2a61 7267 732c 206c 6162 656c  nt, *args, label
+00002ce0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+00002cf0: 6c5b 7374 725d 203d 204e 6f6e 652c 206c  l[str] = None, l
+00002d00: 6162 656c 416e 6368 6f72 3a20 6d6f 6465  abelAnchor: mode
+00002d10: 6c2e 4350 203d 206d 6f64 656c 2e43 502e  l.CP = model.CP.
+00002d20: 6465 6661 756c 742c 202a 2a6b 7761 7267  default, **kwarg
+00002d30: 7329 3a0a 2020 2020 2020 2020 6368 6f73  s):.        chos
+00002d40: 656e 5f6c 6162 656c 203d 2073 656c 662e  en_label = self.
+00002d50: 6c61 6265 6c20 6f72 206c 6162 656c 0a20  label or label. 
+00002d60: 2020 2020 2020 2069 6620 6368 6f73 656e         if chosen
+00002d70: 5f6c 6162 656c 2069 7320 4e6f 6e65 3a0a  _label is None:.
+00002d80: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00002d90: 6520 6578 6365 7074 696f 6e2e 496e 7661  e exception.Inva
+00002da0: 6c69 6457 6964 6765 7444 6566 696e 6974  lidWidgetDefinit
+00002db0: 696f 6e28 277b 7365 6c66 2172 7d3a 204d  ion('{self!r}: M
+00002dc0: 6973 7369 6e67 2072 6571 7569 7265 6420  issing required 
+00002dd0: 6c61 6265 6c27 290a 2020 2020 2020 2020  label').        
+00002de0: 2320 544f 444f 3a20 496d 7072 6f76 6520  # TODO: Improve 
+00002df0: 6c61 6265 6c41 6e63 686f 7220 6f62 6a65  labelAnchor obje
+00002e00: 6374 0a20 2020 2020 2020 2073 7570 6572  ct.        super
+00002e10: 2829 2e5f 5f69 6e69 745f 5f28 7061 7265  ().__init__(pare
+00002e20: 6e74 2c20 7465 7874 3d63 686f 7365 6e5f  nt, text=chosen_
+00002e30: 6c61 6265 6c2c 206c 6162 656c 616e 6368  label, labelanch
+00002e40: 6f72 3d6c 6162 656c 416e 6368 6f72 2e76  or=labelAnchor.v
+00002e50: 616c 7565 2920 2023 2074 746b 2e4c 6162  alue)  # ttk.Lab
+00002e60: 656c 4672 616d 650a 2020 2020 2020 2020  elFrame.        
+00002e70: 6966 205f 5f64 6562 7567 5f5f 3a0a 2020  if __debug__:.  
+00002e80: 2020 2020 2020 2020 2020 6966 2027 6c61            if 'la
+00002e90: 6265 6c77 6964 6765 7427 2069 6e20 6b77  belwidget' in kw
+00002ea0: 6172 6773 3a0a 2020 2020 2020 2020 2020  args:.          
+00002eb0: 2020 2020 2020 7761 726e 696e 6773 2e77        warnings.w
+00002ec0: 6172 6e28 6627 7b73 656c 667d 3a20 556e  arn(f'{self}: Un
+00002ed0: 7375 7070 6f72 7465 6420 226c 6162 656c  supported "label
+00002ee0: 7769 6467 6574 2227 2c20 7374 6163 6b6c  widget"', stackl
+00002ef0: 6576 656c 3d32 290a 2020 2020 2020 2020  evel=2).        
+00002f00: 6b77 6172 6773 2e70 6f70 2827 6c61 6265  kwargs.pop('labe
+00002f10: 6c77 6964 6765 7427 2c20 4e6f 6e65 2920  lwidget', None) 
+00002f20: 2023 2055 6e73 7570 706f 7274 6564 0a20   # Unsupported. 
+00002f30: 2020 2020 2020 2073 656c 662e 696e 6974         self.init
+00002f40: 5f63 6f6e 7461 696e 6572 282a 6172 6773  _container(*args
+00002f50: 2c20 2a2a 6b77 6172 6773 290a 0a0a 2320  , **kwargs)...# 
+00002f60: 2320 5369 6d70 6c65 2057 6964 6765 7473  # Simple Widgets
+00002f70: 0a0a 0a63 6c61 7373 204c 6162 656c 2874  ...class Label(t
+00002f80: 746b 2e4c 6162 656c 2c20 6d69 7869 6e2e  tk.Label, mixin.
+00002f90: 5369 6e67 6c65 5769 6467 6574 293a 0a20  SingleWidget):. 
+00002fa0: 2020 2027 2727 4120 6c61 6265 6c2c 2063     '''A label, c
+00002fb0: 616e 2062 6520 7465 7874 2c20 696d 6167  an be text, imag
+00002fc0: 652c 206f 7220 626f 7468 2e0a 0a20 2020  e, or both...   
+00002fd0: 2054 6869 7320 6973 2061 206c 6162 656c   This is a label
+00002fe0: 2c20 6120 7374 6174 6963 2d69 7368 2077  , a static-ish w
+00002ff0: 6964 6765 7420 7769 7468 6f75 7420 696e  idget without in
+00003000: 7465 7261 6374 696f 6e2e 0a0a 2020 2020  teraction...    
+00003010: 5468 6973 206d 7573 7420 696e 636c 7564  This must includ
+00003020: 6520 6174 206c 6561 7374 2073 6f6d 6520  e at least some 
+00003030: 7465 7874 206f 7220 616e 2069 6d61 6765  text or an image
+00003040: 2c20 6576 656e 2074 686f 7567 6820 626f  , even though bo
+00003050: 7468 2061 7265 206f 7074 696f 6e61 6c2e  th are optional.
+00003060: 0a0a 2020 2020 4e6f 2073 7461 7465 2069  ..    No state i
+00003070: 7320 696e 636c 7564 6564 2e0a 0a20 2020  s included...   
+00003080: 2054 6865 7265 2069 7320 6e6f 2050 7974   There is no Pyt
+00003090: 686f 6e20 646f 6375 6d65 6e74 6174 696f  hon documentatio
+000030a0: 6e2c 2073 6565 2060 6054 6b60 6020 6074  n, see ``Tk`` `t
+000030b0: 746b 2e4c 6162 656c 203c 6874 7470 733a  tk.Label <https:
+000030c0: 2f2f 7777 772e 7463 6c2e 746b 2f6d 616e  //www.tcl.tk/man
+000030d0: 2f74 636c 2f54 6b43 6d64 2f74 746b 5f6c  /tcl/TkCmd/ttk_l
+000030e0: 6162 656c 2e68 746d 6c3e 605f 2064 6f63  abel.html>`_ doc
+000030f0: 756d 656e 7461 7469 6f6e 2e0a 0a20 2020  umentation...   
+00003100: 2041 7267 733a 0a20 2020 2020 2020 206c   Args:.        l
+00003110: 6162 656c 3a20 5468 6520 7465 7874 2074  abel: The text t
+00003120: 6f20 7368 6f77 2e20 4f70 7469 6f6e 616c  o show. Optional
+00003130: 2e20 4361 6e20 6265 2067 6976 656e 2061  . Can be given a
+00003140: 7320 6120 636c 6173 7320 7661 7269 6162  s a class variab
+00003150: 6c65 2e0a 2020 2020 2020 2020 696d 6167  le..        imag
+00003160: 653a 2054 6865 2069 6d61 6765 2074 6f20  e: The image to 
+00003170: 7368 6f77 2e20 4f70 7469 6f6e 616c 2e0a  show. Optional..
+00003180: 2020 2020 2020 2020 2020 2020 5365 6520              See 
+00003190: 6060 546b 6060 2060 746b 2e49 6d61 6765  ``Tk`` `tk.Image
+000031a0: 203c 6874 7470 733a 2f2f 7777 772e 7463   <https://www.tc
+000031b0: 6c2e 746b 2f6d 616e 2f74 636c 2f54 6b43  l.tk/man/tcl/TkC
+000031c0: 6d64 2f69 6d61 6765 2e68 746d 6c3e 605f  md/image.html>`_
+000031d0: 2064 6f63 756d 656e 7461 7469 6f6e 2e0a   documentation..
+000031e0: 0a20 2020 2020 2020 2070 6172 656e 743a  .        parent:
+000031f0: 2054 6865 2070 6172 656e 7420 7769 6467   The parent widg
+00003200: 6574 2e20 4361 6e20 6265 2061 2060 526f  et. Can be a `Ro
+00003210: 6f74 5769 6e64 6f77 6020 6f72 2061 6e6f  otWindow` or ano
+00003220: 7468 6572 2060 6d69 7869 6e2e 436f 6e74  ther `mixin.Cont
+00003230: 6169 6e65 7257 6964 6765 7460 2e0a 2020  ainerWidget`..  
+00003240: 2020 2727 270a 2020 2020 6c61 6265 6c3a    '''.    label:
+00003250: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00003260: 5b73 7472 5d20 3d20 4e6f 6e65 0a20 2020  [str] = None.   
+00003270: 2073 7461 7465 5f74 7970 6520 3d20 7661   state_type = va
+00003280: 722e 6e6f 7468 696e 670a 2020 2020 7769  r.nothing.    wi
+00003290: 6d67 3a20 7479 7069 6e67 2e4f 7074 696f  mg: typing.Optio
+000032a0: 6e61 6c5b 746b 2e49 6d61 6765 5d0a 2020  nal[tk.Image].  
+000032b0: 2020 2727 2754 6865 2069 6d61 6765 206f    '''The image o
+000032c0: 626a 6563 742c 2069 6620 6465 6669 6e65  bject, if define
+000032d0: 642e 0a0a 2020 2020 5468 6973 2061 766f  d...    This avo
+000032e0: 6964 7320 7468 6520 6973 7375 6520 7769  ids the issue wi
+000032f0: 7468 2069 6d61 6765 206f 626a 6563 7473  th image objects
+00003300: 2062 6569 6e67 2067 6172 6261 6765 2063   being garbage c
+00003310: 6f6c 6c65 6374 6564 2c20 7768 696c 6520  ollected, while 
+00003320: 6b65 6570 696e 6720 6120 7265 6665 7265  keeping a refere
+00003330: 6e63 6520 666f 7220 706f 7373 6962 6c65  nce for possible
+00003340: 206d 616e 6970 756c 6174 696f 6e2e 0a0a   manipulation...
+00003350: 2020 2020 4e6f 7465 3a0a 2020 2020 2020      Note:.      
+00003360: 2020 5468 6973 2069 7320 6120 7265 6164    This is a read
+00003370: 2d6f 6e6c 7920 7265 6665 7265 6e63 652c  -only reference,
+00003380: 2069 7420 6d75 7374 2062 6520 6d61 6e69   it must be mani
+00003390: 7075 6c61 7465 6420 7573 696e 6720 6073  pulated using `s
+000033a0: 6574 5f69 6d61 6765 602e 0a20 2020 2027  et_image`..    '
+000033b0: 2727 0a0a 2020 2020 6465 6620 5f5f 696e  ''..    def __in
+000033c0: 6974 5f5f 2873 656c 662c 2070 6172 656e  it__(self, paren
+000033d0: 742c 202a 2c20 6c61 6265 6c3a 2074 7970  t, *, label: typ
+000033e0: 696e 672e 4f70 7469 6f6e 616c 5b73 7472  ing.Optional[str
+000033f0: 5d20 3d20 4e6f 6e65 2c20 696d 6167 653a  ] = None, image:
+00003400: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00003410: 5b74 6b2e 496d 6167 655d 203d 204e 6f6e  [tk.Image] = Non
+00003420: 652c 202a 2a6b 7761 7267 7329 3a0a 2020  e, **kwargs):.  
+00003430: 2020 2020 2020 2320 544f 444f 3a20 5375        # TODO: Su
+00003440: 7070 6f72 7420 6061 6e63 686f 7260 2c20  pport `anchor`, 
+00003450: 7769 7468 2060 6d6f 6465 6c2e 4350 600a  with `model.CP`.
+00003460: 2020 2020 2020 2020 6368 6f73 656e 5f6c          chosen_l
+00003470: 6162 656c 203d 2073 656c 662e 6c61 6265  abel = self.labe
+00003480: 6c20 6f72 206c 6162 656c 0a20 2020 2020  l or label.     
+00003490: 2020 2069 6620 6368 6f73 656e 5f6c 6162     if chosen_lab
+000034a0: 656c 2069 7320 4e6f 6e65 2061 6e64 2069  el is None and i
+000034b0: 6d61 6765 2069 7320 4e6f 6e65 3a0a 2020  mage is None:.  
+000034c0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000034d0: 6578 6365 7074 696f 6e2e 496e 7661 6c69  exception.Invali
+000034e0: 6457 6964 6765 7444 6566 696e 6974 696f  dWidgetDefinitio
+000034f0: 6e28 277b 7365 6c66 2172 7d3a 204e 6565  n('{self!r}: Nee
+00003500: 6473 2061 6e20 696d 6167 6520 6f72 2061  ds an image or a
+00003510: 206c 6162 656c 2729 0a20 2020 2020 2020   label').       
+00003520: 2073 656c 662e 696e 6974 5f73 696e 676c   self.init_singl
+00003530: 6528 7661 7269 6162 6c65 3d4e 6f6e 6529  e(variable=None)
+00003540: 2020 2320 4e6f 2073 7461 7465 2068 6572    # No state her
+00003550: 650a 2020 2020 2020 2020 7375 7065 7228  e.        super(
+00003560: 292e 5f5f 696e 6974 5f5f 2870 6172 656e  ).__init__(paren
+00003570: 742c 202a 2a6b 7761 7267 7329 2020 2320  t, **kwargs)  # 
+00003580: 7474 6b2e 4c61 6265 6c0a 2020 2020 2020  ttk.Label.      
+00003590: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
+000035a0: 6e63 6528 6368 6f73 656e 5f6c 6162 656c  nce(chosen_label
+000035b0: 2c20 7374 7229 0a20 2020 2020 2020 2069  , str).        i
+000035c0: 6620 6368 6f73 656e 5f6c 6162 656c 3a0a  f chosen_label:.
+000035d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000035e0: 2e73 6574 5f6c 6162 656c 2863 686f 7365  .set_label(chose
+000035f0: 6e5f 6c61 6265 6c29 0a20 2020 2020 2020  n_label).       
+00003600: 2069 6620 696d 6167 653a 0a20 2020 2020   if image:.     
+00003610: 2020 2020 2020 2073 656c 662e 7365 745f         self.set_
+00003620: 696d 6167 6528 696d 6167 6529 0a20 2020  image(image).   
+00003630: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00003640: 2020 2020 2020 2073 656c 662e 7769 6d67         self.wimg
+00003650: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+00003660: 7365 6c66 2e62 696e 6469 6e67 2827 3c42  self.binding('<B
+00003670: 7574 746f 6e2d 313e 272c 2073 656c 662e  utton-1>', self.
+00003680: 696e 766f 6b65 5f6f 6e43 6c69 636b 290a  invoke_onClick).
+00003690: 2020 2020 2020 2020 6966 205f 5f64 6562          if __deb
+000036a0: 7567 5f5f 3a0a 2020 2020 2020 2020 2020  ug__:.          
+000036b0: 2020 6966 2027 7465 7874 7661 7269 6162    if 'textvariab
+000036c0: 6c65 2720 696e 206b 7761 7267 733a 0a20  le' in kwargs:. 
+000036d0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+000036e0: 6172 6e69 6e67 732e 7761 726e 2866 277b  arnings.warn(f'{
+000036f0: 7365 6c66 7d3a 2054 6f20 7573 6520 6120  self}: To use a 
+00003700: 7661 7269 6162 6c65 2061 7320 6c61 6265  variable as labe
+00003710: 6c2c 2073 6565 204c 6162 656c 5374 6174  l, see LabelStat
+00003720: 6566 756c 272c 2073 7461 636b 6c65 7665  eful', stackleve
+00003730: 6c3d 3229 0a0a 2020 2020 6465 6620 696e  l=2)..    def in
+00003740: 766f 6b65 5f6f 6e43 6c69 636b 2873 656c  voke_onClick(sel
+00003750: 662c 2065 7665 6e74 3d4e 6f6e 6529 3a0a  f, event=None):.
+00003760: 2020 2020 2020 2020 2727 2727 2727 2020          ''''''  
+00003770: 2320 496e 7465 726e 616c 2c20 646f 206e  # Internal, do n
+00003780: 6f74 2064 6f63 756d 656e 740a 2020 2020  ot document.    
+00003790: 2020 2020 7365 6c66 2e6f 6e43 6c69 636b      self.onClick
+000037a0: 2829 0a0a 2020 2020 6465 6620 7365 745f  ()..    def set_
+000037b0: 696d 6167 6528 7365 6c66 2c20 696d 6167  image(self, imag
+000037c0: 653a 2074 7970 696e 672e 4f70 7469 6f6e  e: typing.Option
+000037d0: 616c 5b74 6b2e 496d 6167 655d 2920 2d3e  al[tk.Image]) ->
+000037e0: 204e 6f6e 653a 0a20 2020 2020 2020 2027   None:.        '
+000037f0: 2727 4368 616e 6765 2074 6865 206c 6162  ''Change the lab
+00003800: 656c 2069 6d61 6765 2e0a 0a20 2020 2020  el image...     
+00003810: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00003820: 2020 2020 2069 6d61 6765 3a20 5468 6520       image: The 
+00003830: 696d 6167 6520 6f62 6a65 6374 2074 6f20  image object to 
+00003840: 7365 742c 206f 7220 604e 6f6e 6560 2074  set, or `None` t
+00003850: 6f20 7265 6d6f 7665 2069 742e 0a20 2020  o remove it..   
+00003860: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00003870: 2073 656c 662e 7769 6d67 203d 2069 6d61   self.wimg = ima
+00003880: 6765 2020 2320 5361 7665 2061 2072 6566  ge  # Save a ref
+00003890: 6572 656e 6365 2074 6f20 6176 6f69 6420  erence to avoid 
+000038a0: 6761 7262 6167 6520 636f 6c6c 6563 7469  garbage collecti
+000038b0: 6f6e 0a20 2020 2020 2020 2073 656c 665b  on.        self[
+000038c0: 2769 6d61 6765 275d 203d 2073 656c 662e  'image'] = self.
+000038d0: 7769 6d67 0a0a 2020 2020 6465 6620 7365  wimg..    def se
+000038e0: 745f 6c61 6265 6c28 7365 6c66 2c20 6c61  t_label(self, la
+000038f0: 6265 6c3a 2073 7472 2920 2d3e 204e 6f6e  bel: str) -> Non
+00003900: 653a 0a20 2020 2020 2020 2027 2727 4368  e:.        '''Ch
+00003910: 616e 6765 2074 6865 206c 6162 656c 2074  ange the label t
+00003920: 6578 742e 2727 270a 2020 2020 2020 2020  ext.'''.        
+00003930: 7365 6c66 5b27 7465 7874 275d 203d 206c  self['text'] = l
+00003940: 6162 656c 0a0a 2020 2020 2320 544f 444f  abel..    # TODO
+00003950: 3a20 5061 7373 2074 6865 2065 7665 6e74  : Pass the event
+00003960: 206f 626a 6563 743f 0a20 2020 2023 2054   object?.    # T
+00003970: 4f44 4f3a 204e 6f74 206e 6565 6465 6420  ODO: Not needed 
+00003980: 6f6e 206c 6162 656c 730a 2020 2020 6465  on labels.    de
+00003990: 6620 6f6e 436c 6963 6b28 7365 6c66 293a  f onClick(self):
+000039a0: 0a20 2020 2020 2020 2022 2222 4361 6c6c  .        """Call
+000039b0: 6261 636b 2074 6f20 6265 2065 7865 6375  back to be execu
+000039c0: 7465 6420 7768 656e 2063 6c69 636b 696e  ted when clickin
+000039d0: 6720 7468 6973 2077 6964 6765 742e 0a0a  g this widget...
+000039e0: 2020 2020 2020 2020 4465 6661 756c 7473          Defaults
+000039f0: 2074 6f20 646f 696e 6720 6e6f 7468 696e   to doing nothin
+00003a00: 672e 0a0a 2020 2020 2020 2020 4176 6169  g...        Avai
+00003a10: 6c61 626c 6520 666f 7220 7375 6263 6c61  lable for subcla
+00003a20: 7373 2072 6564 6566 696e 6974 696f 6e2e  ss redefinition.
+00003a30: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00003a40: 2020 2020 2070 6173 730a 0a0a 636c 6173       pass...clas
+00003a50: 7320 4c61 6265 6c53 7461 7465 6675 6c28  s LabelStateful(
+00003a60: 7474 6b2e 4c61 6265 6c2c 206d 6978 696e  ttk.Label, mixin
+00003a70: 2e53 696e 676c 6557 6964 6765 7429 3a0a  .SingleWidget):.
+00003a80: 2020 2020 2727 2741 2073 7461 7465 6675      '''A statefu
+00003a90: 6c20 604c 6162 656c 602c 2077 6865 7265  l `Label`, where
+00003aa0: 2074 6865 2074 6578 7420 6973 2063 6f6e   the text is con
+00003ab0: 7472 6f6c 6c65 6420 6279 2061 2076 6172  trolled by a var
+00003ac0: 6961 626c 652e 0a0a 2020 2020 5468 6973  iable...    This
+00003ad0: 2069 7320 616e 2061 6c74 6572 6e61 7469   is an alternati
+00003ae0: 7665 2060 4c61 6265 6c60 2c20 7768 6572  ve `Label`, wher
+00003af0: 6520 7468 6520 7465 7874 2069 7320 636f  e the text is co
+00003b00: 6e74 726f 6c6c 6564 2062 7920 6120 7661  ntrolled by a va
+00003b10: 7269 6162 6c65 2e0a 2020 2020 4974 2773  riable..    It's
+00003b20: 2061 6e20 616c 7465 726e 6174 6976 6520   an alternative 
+00003b30: 746f 206d 616e 7561 6c6c 7920 6361 6c6c  to manually call
+00003b40: 696e 6720 604c 6162 656c 2e73 6574 5f6c  ing `Label.set_l
+00003b50: 6162 656c 602c 206f 7220 6120 7265 6164  abel`, or a read
+00003b60: 2d6f 6e6c 790a 2020 2020 6045 6e74 7279  -only.    `Entry
+00003b70: 602e 0a0a 2020 2020 5468 6520 696d 6167  `...    The imag
+00003b80: 6520 6973 206f 7074 696f 6e61 6c2e 0a0a  e is optional...
+00003b90: 2020 2020 5468 6572 6520 6973 206e 6f20      There is no 
+00003ba0: 5079 7468 6f6e 2064 6f63 756d 656e 7461  Python documenta
+00003bb0: 7469 6f6e 2c20 7365 6520 6060 546b 6060  tion, see ``Tk``
+00003bc0: 2060 7474 6b2e 4c61 6265 6c20 3c68 7474   `ttk.Label <htt
+00003bd0: 7073 3a2f 2f77 7777 2e74 636c 2e74 6b2f  ps://www.tcl.tk/
+00003be0: 6d61 6e2f 7463 6c2f 546b 436d 642f 7474  man/tcl/TkCmd/tt
+00003bf0: 6b5f 6c61 6265 6c2e 6874 6d6c 3e60 5f20  k_label.html>`_ 
+00003c00: 646f 6375 6d65 6e74 6174 696f 6e2e 0a0a  documentation...
+00003c10: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00003c20: 2020 7661 7269 6162 6c65 3a20 5573 6520    variable: Use 
+00003c30: 616e 2065 7874 6572 6e61 6c6c 7920 6465  an externally de
+00003c40: 6669 6e65 6420 7661 7269 6162 6c65 2c20  fined variable, 
+00003c50: 696e 7374 6561 6420 6f66 2063 7265 6174  instead of creat
+00003c60: 696e 6720 6120 6e65 7720 6f6e 6520 7370  ing a new one sp
+00003c70: 6563 6966 6963 2066 6f72 2074 6869 7320  ecific for this 
+00003c80: 7769 6467 6574 2e0a 2020 2020 2020 2020  widget..        
+00003c90: 7061 7265 6e74 3a20 5468 6520 7061 7265  parent: The pare
+00003ca0: 6e74 2077 6964 6765 742e 2043 616e 2062  nt widget. Can b
+00003cb0: 6520 6120 6052 6f6f 7457 696e 646f 7760  e a `RootWindow`
+00003cc0: 206f 7220 616e 6f74 6865 7220 606d 6978   or another `mix
+00003cd0: 696e 2e43 6f6e 7461 696e 6572 5769 6467  in.ContainerWidg
+00003ce0: 6574 602e 0a20 2020 2027 2727 0a20 2020  et`..    '''.   
+00003cf0: 2073 7461 7465 5f74 7970 6520 3d20 7661   state_type = va
+00003d00: 722e 5374 7269 6e67 0a20 2020 2077 696d  r.String.    wim
+00003d10: 673a 2074 7970 696e 672e 4f70 7469 6f6e  g: typing.Option
+00003d20: 616c 5b74 6b2e 496d 6167 655d 0a20 2020  al[tk.Image].   
+00003d30: 2027 2727 5468 6520 696d 6167 6520 6f62   '''The image ob
+00003d40: 6a65 6374 2c20 6966 2064 6566 696e 6564  ject, if defined
+00003d50: 2e0a 0a20 2020 2054 6869 7320 6176 6f69  ...    This avoi
+00003d60: 6473 2074 6865 2069 7373 7565 2077 6974  ds the issue wit
+00003d70: 6820 696d 6167 6520 6f62 6a65 6374 7320  h image objects 
+00003d80: 6265 696e 6720 6761 7262 6167 6520 636f  being garbage co
+00003d90: 6c6c 6563 7465 642c 2077 6869 6c65 206b  llected, while k
+00003da0: 6565 7069 6e67 2061 2072 6566 6572 656e  eeping a referen
+00003db0: 6365 2066 6f72 2070 6f73 7369 626c 6520  ce for possible 
+00003dc0: 6d61 6e69 7075 6c61 7469 6f6e 2e0a 0a20  manipulation... 
+00003dd0: 2020 204e 6f74 653a 0a20 2020 2020 2020     Note:.       
+00003de0: 2054 6869 7320 6973 2061 2072 6561 642d   This is a read-
+00003df0: 6f6e 6c79 2072 6566 6572 656e 6365 2c20  only reference, 
+00003e00: 6974 206d 7573 7420 6265 206d 616e 6970  it must be manip
+00003e10: 756c 6174 6564 2075 7369 6e67 2060 7365  ulated using `se
+00003e20: 745f 696d 6167 6560 2e0a 2020 2020 2727  t_image`..    ''
+00003e30: 270a 0a20 2020 2064 6566 205f 5f69 6e69  '..    def __ini
+00003e40: 745f 5f28 7365 6c66 2c20 7061 7265 6e74  t__(self, parent
+00003e50: 2c20 2a2c 2076 6172 6961 626c 653a 2074  , *, variable: t
+00003e60: 7970 696e 672e 4f70 7469 6f6e 616c 5b76  yping.Optional[v
+00003e70: 6172 2e53 7472 696e 675d 203d 204e 6f6e  ar.String] = Non
+00003e80: 652c 2069 6d61 6765 3a20 7479 7069 6e67  e, image: typing
+00003e90: 2e4f 7074 696f 6e61 6c5b 746b 2e49 6d61  .Optional[tk.Ima
+00003ea0: 6765 5d20 3d20 4e6f 6e65 2c20 2a2a 6b77  ge] = None, **kw
+00003eb0: 6172 6773 293a 0a20 2020 2020 2020 2073  args):.        s
+00003ec0: 656c 662e 696e 6974 5f73 696e 676c 6528  elf.init_single(
+00003ed0: 7661 7269 6162 6c65 3d76 6172 6961 626c  variable=variabl
+00003ee0: 6529 0a20 2020 2020 2020 206b 7761 7267  e).        kwarg
+00003ef0: 732e 7570 6461 7465 287b 0a20 2020 2020  s.update({.     
+00003f00: 2020 2020 2020 2027 7465 7874 7661 7269         'textvari
+00003f10: 6162 6c65 273a 2073 656c 662e 7661 7269  able': self.vari
+00003f20: 6162 6c65 2c0a 2020 2020 2020 2020 7d29  able,.        })
+00003f30: 0a20 2020 2020 2020 206b 7761 7267 732e  .        kwargs.
+00003f40: 706f 7028 2774 6578 7427 2c20 4e6f 6e65  pop('text', None
+00003f50: 2920 2023 2049 676e 6f72 6520 7468 6520  )  # Ignore the 
+00003f60: 6769 7665 6e20 7465 7874 0a20 2020 2020  given text.     
+00003f70: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
+00003f80: 745f 5f28 7061 7265 6e74 2c20 2a2a 6b77  t__(parent, **kw
+00003f90: 6172 6773 2920 2023 2074 746b 2e4c 6162  args)  # ttk.Lab
+00003fa0: 656c 0a20 2020 2020 2020 2069 6620 696d  el.        if im
+00003fb0: 6167 653a 0a20 2020 2020 2020 2020 2020  age:.           
+00003fc0: 2073 656c 662e 7365 745f 696d 6167 6528   self.set_image(
+00003fd0: 696d 6167 6529 0a20 2020 2020 2020 2065  image).        e
+00003fe0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00003ff0: 2073 656c 662e 7769 6d67 203d 204e 6f6e   self.wimg = Non
+00004000: 650a 2020 2020 2020 2020 7365 6c66 2e62  e.        self.b
+00004010: 696e 6469 6e67 2827 3c42 7574 746f 6e2d  inding('<Button-
+00004020: 313e 272c 2073 656c 662e 696e 766f 6b65  1>', self.invoke
+00004030: 5f6f 6e43 6c69 636b 290a 0a20 2020 2064  _onClick)..    d
+00004040: 6566 2069 6e76 6f6b 655f 6f6e 436c 6963  ef invoke_onClic
+00004050: 6b28 7365 6c66 2c20 6576 656e 743d 4e6f  k(self, event=No
+00004060: 6e65 293a 0a20 2020 2020 2020 2027 2727  ne):.        '''
+00004070: 2727 2720 2023 2049 6e74 6572 6e61 6c2c  '''  # Internal,
+00004080: 2064 6f20 6e6f 7420 646f 6375 6d65 6e74   do not document
+00004090: 0a20 2020 2020 2020 2073 656c 662e 6f6e  .        self.on
+000040a0: 436c 6963 6b28 290a 0a20 2020 2064 6566  Click()..    def
+000040b0: 2073 6574 5f69 6d61 6765 2873 656c 662c   set_image(self,
+000040c0: 2069 6d61 6765 3a20 7479 7069 6e67 2e4f   image: typing.O
+000040d0: 7074 696f 6e61 6c5b 746b 2e49 6d61 6765  ptional[tk.Image
+000040e0: 5d29 202d 3e20 4e6f 6e65 3a0a 2020 2020  ]) -> None:.    
+000040f0: 2020 2020 2727 2743 6861 6e67 6520 7468      '''Change th
+00004100: 6520 6c61 6265 6c20 696d 6167 652e 0a0a  e label image...
+00004110: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00004120: 2020 2020 2020 2020 2020 696d 6167 653a            image:
+00004130: 2054 6865 2069 6d61 6765 206f 626a 6563   The image objec
+00004140: 7420 746f 2073 6574 2c20 6f72 2060 4e6f  t to set, or `No
+00004150: 6e65 6020 746f 2072 656d 6f76 6520 6974  ne` to remove it
+00004160: 2e0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
+00004170: 2020 2020 2020 7365 6c66 2e77 696d 6720        self.wimg 
+00004180: 3d20 696d 6167 6520 2023 2053 6176 6520  = image  # Save 
+00004190: 6120 7265 6665 7265 6e63 6520 746f 2061  a reference to a
+000041a0: 766f 6964 2067 6172 6261 6765 2063 6f6c  void garbage col
+000041b0: 6c65 6374 696f 6e0a 2020 2020 2020 2020  lection.        
+000041c0: 7365 6c66 5b27 696d 6167 6527 5d20 3d20  self['image'] = 
+000041d0: 7365 6c66 2e77 696d 670a 0a20 2020 2023  self.wimg..    #
+000041e0: 2054 4f44 4f3a 2050 6173 7320 7468 6520   TODO: Pass the 
+000041f0: 6576 656e 7420 6f62 6a65 6374 3f0a 2020  event object?.  
+00004200: 2020 2320 544f 444f 3a20 4e6f 7420 6e65    # TODO: Not ne
+00004210: 6564 6564 206f 6e20 6c61 6265 6c73 0a20  eded on labels. 
+00004220: 2020 2064 6566 206f 6e43 6c69 636b 2873     def onClick(s
+00004230: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00004240: 2243 616c 6c62 6163 6b20 746f 2062 6520  "Callback to be 
+00004250: 6578 6563 7574 6564 2077 6865 6e20 636c  executed when cl
+00004260: 6963 6b69 6e67 2074 6869 7320 7769 6467  icking this widg
+00004270: 6574 2e0a 0a20 2020 2020 2020 2044 6566  et...        Def
+00004280: 6175 6c74 7320 746f 2064 6f69 6e67 206e  aults to doing n
+00004290: 6f74 6869 6e67 2e0a 0a20 2020 2020 2020  othing...       
+000042a0: 2041 7661 696c 6162 6c65 2066 6f72 2073   Available for s
+000042b0: 7562 636c 6173 7320 7265 6465 6669 6e69  ubclass redefini
+000042c0: 7469 6f6e 2e0a 2020 2020 2020 2020 2222  tion..        ""
+000042d0: 220a 2020 2020 2020 2020 7061 7373 0a0a  ".        pass..
+000042e0: 0a63 6c61 7373 2042 7574 746f 6e28 7474  .class Button(tt
+000042f0: 6b2e 4275 7474 6f6e 2c20 6d69 7869 6e2e  k.Button, mixin.
+00004300: 5369 6e67 6c65 5769 6467 6574 293a 0a20  SingleWidget):. 
+00004310: 2020 2027 2727 4120 6275 7474 6f6e 2077     '''A button w
+00004320: 6974 6820 6120 6c61 6265 6c2e 0a0a 2020  ith a label...  
+00004330: 2020 5468 6973 2069 7320 6120 6275 7474    This is a butt
+00004340: 6f6e 2c20 7769 7468 2061 206c 6162 656c  on, with a label
+00004350: 2e20 5468 6520 6d61 696e 2069 6e74 6572  . The main inter
+00004360: 6163 7469 6f6e 2069 7320 6265 696e 6720  action is being 
+00004370: 636c 6963 6b65 6420 6f6e 2e0a 0a20 2020  clicked on...   
+00004380: 204e 6f20 7374 6174 6520 6973 2069 6e63   No state is inc
+00004390: 6c75 6465 642e 0a0a 2020 2020 5468 6572  luded...    Ther
+000043a0: 6520 6973 206e 6f20 5079 7468 6f6e 2064  e is no Python d
+000043b0: 6f63 756d 656e 7461 7469 6f6e 2c20 7365  ocumentation, se
+000043c0: 6520 6060 546b 6060 2060 7474 6b2e 4275  e ``Tk`` `ttk.Bu
+000043d0: 7474 6f6e 203c 6874 7470 733a 2f2f 7777  tton <https://ww
+000043e0: 772e 7463 6c2e 746b 2f6d 616e 2f74 636c  w.tcl.tk/man/tcl
+000043f0: 2f54 6b43 6d64 2f74 746b 5f62 7574 746f  /TkCmd/ttk_butto
+00004400: 6e2e 6874 6d6c 3e60 5f20 646f 6375 6d65  n.html>`_ docume
+00004410: 6e74 6174 696f 6e2e 0a0a 2020 2020 4172  ntation...    Ar
+00004420: 6773 3a0a 2020 2020 2020 2020 6c61 6265  gs:.        labe
+00004430: 6c3a 2054 6865 206c 6162 656c 2074 6f20  l: The label to 
+00004440: 696e 636c 7564 6520 696e 7369 6465 2074  include inside t
+00004450: 6865 2062 7574 746f 6e2e 204f 7074 696f  he button. Optio
+00004460: 6e61 6c2e 2043 616e 2062 6520 6769 7665  nal. Can be give
+00004470: 6e20 6173 2061 2063 6c61 7373 2076 6172  n as a class var
+00004480: 6961 626c 652e 0a20 2020 2020 2020 2077  iable..        w
+00004490: 6964 7468 3a20 5468 6520 6275 7474 6f6e  idth: The button
+000044a0: 2077 6964 7468 2c20 696e 2070 6978 656c   width, in pixel
+000044b0: 732e 0a20 2020 2020 2020 2020 2020 2044  s..            D
+000044c0: 6566 6175 6c74 7320 746f 2061 6e20 6164  efaults to an ad
+000044d0: 2d68 6f63 2063 616c 6375 6c61 7469 6f6e  -hoc calculation
+000044e0: 2062 6173 6564 206f 6e20 7468 6520 6c65   based on the le
+000044f0: 6e67 7468 206f 6620 7468 6520 6c61 6265  ngth of the labe
+00004500: 6c2e 0a0a 2020 2020 2020 2020 7061 7265  l...        pare
+00004510: 6e74 3a20 5468 6520 7061 7265 6e74 2077  nt: The parent w
+00004520: 6964 6765 742e 2043 616e 2062 6520 6120  idget. Can be a 
+00004530: 6052 6f6f 7457 696e 646f 7760 206f 7220  `RootWindow` or 
+00004540: 616e 6f74 6865 7220 606d 6978 696e 2e43  another `mixin.C
+00004550: 6f6e 7461 696e 6572 5769 6467 6574 602e  ontainerWidget`.
+00004560: 0a20 2020 2027 2727 0a20 2020 206c 6162  .    '''.    lab
+00004570: 656c 3a20 7479 7069 6e67 2e4f 7074 696f  el: typing.Optio
+00004580: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
+00004590: 2020 2020 7374 6174 655f 7479 7065 203d      state_type =
+000045a0: 2076 6172 2e6e 6f74 6869 6e67 0a0a 2020   var.nothing..  
+000045b0: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+000045c0: 656c 662c 2070 6172 656e 742c 202a 2c20  elf, parent, *, 
+000045d0: 6c61 6265 6c3a 2074 7970 696e 672e 4f70  label: typing.Op
+000045e0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+000045f0: 6e65 2c20 7769 6474 683a 2074 7970 696e  ne, width: typin
+00004600: 672e 4f70 7469 6f6e 616c 5b69 6e74 5d20  g.Optional[int] 
+00004610: 3d20 4e6f 6e65 2c20 2a2a 6b77 6172 6773  = None, **kwargs
+00004620: 293a 0a20 2020 2020 2020 2063 686f 7365  ):.        chose
+00004630: 6e5f 6c61 6265 6c20 3d20 7365 6c66 2e6c  n_label = self.l
+00004640: 6162 656c 206f 7220 6c61 6265 6c0a 2020  abel or label.  
+00004650: 2020 2020 2020 6966 2063 686f 7365 6e5f        if chosen_
+00004660: 6c61 6265 6c20 6973 204e 6f6e 653a 0a20  label is None:. 
+00004670: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00004680: 2065 7863 6570 7469 6f6e 2e49 6e76 616c   exception.Inval
+00004690: 6964 5769 6467 6574 4465 6669 6e69 7469  idWidgetDefiniti
+000046a0: 6f6e 2827 7b73 656c 6621 727d 3a20 4d69  on('{self!r}: Mi
+000046b0: 7373 696e 6720 7265 7175 6972 6564 206c  ssing required l
+000046c0: 6162 656c 2729 0a20 2020 2020 2020 2073  abel').        s
+000046d0: 656c 662e 696e 6974 5f73 696e 676c 6528  elf.init_single(
+000046e0: 7661 7269 6162 6c65 3d4e 6f6e 6529 2020  variable=None)  
+000046f0: 2320 4e6f 2073 7461 7465 2068 6572 650a  # No state here.
+00004700: 2020 2020 2020 2020 6173 7365 7274 2069          assert i
+00004710: 7369 6e73 7461 6e63 6528 6368 6f73 656e  sinstance(chosen
+00004720: 5f6c 6162 656c 2c20 7374 7229 0a20 2020  _label, str).   
+00004730: 2020 2020 206b 7761 7267 732e 7570 6461       kwargs.upda
+00004740: 7465 287b 0a20 2020 2020 2020 2020 2020  te({.           
+00004750: 2027 7465 7874 273a 2063 686f 7365 6e5f   'text': chosen_
+00004760: 6c61 6265 6c2c 0a20 2020 2020 2020 2020  label,.         
+00004770: 2020 2027 7769 6474 6827 3a20 7769 6474     'width': widt
+00004780: 6820 6f72 2066 6e2e 6c61 6265 6c5f 7369  h or fn.label_si
+00004790: 7a65 286c 656e 286c 6162 656c 206f 7220  ze(len(label or 
+000047a0: 274d 2729 292c 0a20 2020 2020 2020 2020  'M')),.         
+000047b0: 2020 2027 636f 6d6d 616e 6427 3a20 7365     'command': se
+000047c0: 6c66 2e69 6e76 6f6b 655f 6f6e 436c 6963  lf.invoke_onClic
+000047d0: 6b2c 0a20 2020 2020 2020 207d 290a 2020  k,.        }).  
+000047e0: 2020 2020 2020 7375 7065 7228 292e 5f5f        super().__
+000047f0: 696e 6974 5f5f 2870 6172 656e 742c 202a  init__(parent, *
+00004800: 2a6b 7761 7267 7329 2020 2320 7474 6b2e  *kwargs)  # ttk.
+00004810: 4275 7474 6f6e 0a0a 2020 2020 6465 6620  Button..    def 
+00004820: 696e 766f 6b65 5f6f 6e43 6c69 636b 2873  invoke_onClick(s
+00004830: 656c 6629 3a0a 2020 2020 2020 2020 2727  elf):.        ''
+00004840: 2727 2727 2020 2320 496e 7465 726e 616c  ''''  # Internal
+00004850: 2c20 646f 206e 6f74 2064 6f63 756d 656e  , do not documen
+00004860: 740a 2020 2020 2020 2020 7365 6c66 2e6f  t.        self.o
+00004870: 6e43 6c69 636b 2829 0a0a 2020 2020 6465  nClick()..    de
+00004880: 6620 6f6e 436c 6963 6b28 7365 6c66 293a  f onClick(self):
+00004890: 0a20 2020 2020 2020 2022 2222 4361 6c6c  .        """Call
+000048a0: 6261 636b 2074 6f20 6265 2063 616c 6c65  back to be calle
+000048b0: 6420 7768 656e 2063 6c69 636b 696e 6720  d when clicking 
+000048c0: 7468 6973 2077 6964 6765 742e 0a0a 2020  this widget...  
+000048d0: 2020 2020 2020 4465 6661 756c 7473 2074        Defaults t
+000048e0: 6f20 646f 696e 6720 6e6f 7468 696e 672e  o doing nothing.
+000048f0: 0a0a 2020 2020 2020 2020 4176 6169 6c61  ..        Availa
+00004900: 626c 6520 666f 7220 7375 6263 6c61 7373  ble for subclass
+00004910: 2072 6564 6566 696e 6974 696f 6e2e 0a20   redefinition.. 
+00004920: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00004930: 2020 2070 6173 730a 0a0a 636c 6173 7320     pass...class 
+00004940: 4368 6563 6b62 6f78 2874 746b 2e43 6865  Checkbox(ttk.Che
+00004950: 636b 6275 7474 6f6e 2c20 6d69 7869 6e2e  ckbutton, mixin.
+00004960: 5369 6e67 6c65 5769 6467 6574 293a 0a20  SingleWidget):. 
+00004970: 2020 2027 2727 4120 6368 6563 6b62 6f78     '''A checkbox
+00004980: 2c20 7369 6d70 6c65 2062 6f6f 6c65 616e  , simple boolean
+00004990: 2063 686f 6963 652e 0a0a 2020 2020 5468   choice...    Th
+000049a0: 6973 2069 7320 6120 6368 6563 6b62 6f78  is is a checkbox
+000049b0: 2077 6974 6820 6120 6c61 6265 6c2e 2054   with a label. T
+000049c0: 6865 206d 6169 6e20 696e 7465 7261 6374  he main interact
+000049d0: 696f 6e20 6973 2062 6569 6e67 2063 6c69  ion is being cli
+000049e0: 636b 6564 206f 6e2c 0a20 2020 2077 6869  cked on,.    whi
+000049f0: 6368 2074 6f67 676c 6573 2069 7473 2076  ch toggles its v
+00004a00: 616c 7565 2e0a 0a20 2020 2054 6865 2073  alue...    The s
+00004a10: 7461 7465 2069 7320 6120 7369 6e67 6c65  tate is a single
+00004a20: 2060 626f 6f6c 6020 7661 6c75 652e 0a0a   `bool` value...
+00004a30: 2020 2020 5468 6572 6520 6973 206e 6f20      There is no 
+00004a40: 5079 7468 6f6e 2064 6f63 756d 656e 7461  Python documenta
+00004a50: 7469 6f6e 2c20 7365 6520 6060 546b 6060  tion, see ``Tk``
+00004a60: 2060 7474 6b2e 4368 6563 6b62 7574 746f   `ttk.Checkbutto
+00004a70: 6e20 3c68 7474 7073 3a2f 2f77 7777 2e74  n <https://www.t
+00004a80: 636c 2e74 6b2f 6d61 6e2f 7463 6c2f 546b  cl.tk/man/tcl/Tk
+00004a90: 436d 642f 7474 6b5f 6368 6563 6b62 7574  Cmd/ttk_checkbut
+00004aa0: 746f 6e2e 6874 6d6c 3e60 5f20 646f 6375  ton.html>`_ docu
+00004ab0: 6d65 6e74 6174 696f 6e2e 0a0a 2020 2020  mentation...    
+00004ac0: 4172 6773 3a0a 2020 2020 2020 2020 6c61  Args:.        la
+00004ad0: 6265 6c3a 2054 6865 206c 6162 656c 2074  bel: The label t
+00004ae0: 6f20 696e 636c 7564 6520 6265 7369 6465  o include beside
+00004af0: 7320 7468 6520 6368 6563 6b62 6f78 2e20  s the checkbox. 
+00004b00: 4361 6e20 6265 2067 6976 656e 2061 7320  Can be given as 
+00004b10: 6120 636c 6173 7320 7661 7269 6162 6c65  a class variable
+00004b20: 2e0a 2020 2020 2020 2020 2020 2020 4974  ..            It
+00004b30: 2069 7320 696e 636c 7564 6564 206f 6e20   is included on 
+00004b40: 7468 6520 7269 6768 7420 7369 6465 206f  the right side o
+00004b50: 6620 7468 6520 6368 6563 6b62 6f78 2e0a  f the checkbox..
+00004b60: 2020 2020 2020 2020 7265 6164 6f6e 6c79          readonly
+00004b70: 3a20 5368 6f75 6c64 2074 6865 2077 6964  : Should the wid
+00004b80: 6765 7420 616c 6c6f 7720 696e 7465 7261  get allow intera
+00004b90: 6374 696f 6e20 746f 2074 6f67 676c 6520  ction to toggle 
+00004ba0: 6974 7320 7661 6c75 652e 2044 6566 6175  its value. Defau
+00004bb0: 6c74 2074 6f20 2a61 6c6c 6f77 696e 672a  lt to *allowing*
+00004bc0: 2069 6e74 6572 6163 7469 6f6e 2e0a 0a20   interaction... 
+00004bd0: 2020 2020 2020 2070 6172 656e 743a 2054         parent: T
+00004be0: 6865 2070 6172 656e 7420 7769 6467 6574  he parent widget
+00004bf0: 2e20 4361 6e20 6265 2061 2060 526f 6f74  . Can be a `Root
+00004c00: 5769 6e64 6f77 6020 6f72 2061 6e6f 7468  Window` or anoth
+00004c10: 6572 2060 6d69 7869 6e2e 436f 6e74 6169  er `mixin.Contai
+00004c20: 6e65 7257 6964 6765 7460 2e0a 2020 2020  nerWidget`..    
+00004c30: 2020 2020 7661 7269 6162 6c65 3a20 5573      variable: Us
+00004c40: 6520 616e 2065 7874 6572 6e61 6c6c 7920  e an externally 
+00004c50: 6465 6669 6e65 6420 7661 7269 6162 6c65  defined variable
+00004c60: 2c20 696e 7374 6561 6420 6f66 2063 7265  , instead of cre
+00004c70: 6174 696e 6720 6120 6e65 7720 6f6e 6520  ating a new one 
+00004c80: 7370 6563 6966 6963 2066 6f72 2074 6869  specific for thi
+00004c90: 7320 7769 6467 6574 2e0a 2020 2020 2727  s widget..    ''
+00004ca0: 270a 2020 2020 6c61 6265 6c3a 2074 7970  '.    label: typ
+00004cb0: 696e 672e 4f70 7469 6f6e 616c 5b73 7472  ing.Optional[str
+00004cc0: 5d20 3d20 4e6f 6e65 0a20 2020 2073 7461  ] = None.    sta
+00004cd0: 7465 5f74 7970 6520 3d20 7661 722e 426f  te_type = var.Bo
+00004ce0: 6f6c 6561 6e0a 0a20 2020 2064 6566 205f  olean..    def _
+00004cf0: 5f69 6e69 745f 5f28 7365 6c66 2c20 7061  _init__(self, pa
+00004d00: 7265 6e74 2c20 2a2c 206c 6162 656c 3a20  rent, *, label: 
+00004d10: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+00004d20: 7374 725d 203d 204e 6f6e 652c 2072 6561  str] = None, rea
+00004d30: 646f 6e6c 793a 2062 6f6f 6c20 3d20 4661  donly: bool = Fa
+00004d40: 6c73 652c 2076 6172 6961 626c 653a 2074  lse, variable: t
+00004d50: 7970 696e 672e 4f70 7469 6f6e 616c 5b76  yping.Optional[v
+00004d60: 6172 2e42 6f6f 6c65 616e 5d20 3d20 4e6f  ar.Boolean] = No
+00004d70: 6e65 2c20 2a2a 6b77 6172 6773 293a 0a20  ne, **kwargs):. 
+00004d80: 2020 2020 2020 2063 686f 7365 6e5f 6c61         chosen_la
+00004d90: 6265 6c20 3d20 7365 6c66 2e6c 6162 656c  bel = self.label
+00004da0: 206f 7220 6c61 6265 6c0a 2020 2020 2020   or label.      
+00004db0: 2020 6966 2063 686f 7365 6e5f 6c61 6265    if chosen_labe
+00004dc0: 6c20 6973 204e 6f6e 653a 0a20 2020 2020  l is None:.     
+00004dd0: 2020 2020 2020 2072 6169 7365 2065 7863         raise exc
+00004de0: 6570 7469 6f6e 2e49 6e76 616c 6964 5769  eption.InvalidWi
+00004df0: 6467 6574 4465 6669 6e69 7469 6f6e 2827  dgetDefinition('
+00004e00: 7b73 656c 6621 727d 3a20 4d69 7373 696e  {self!r}: Missin
+00004e10: 6720 7265 7175 6972 6564 206c 6162 656c  g required label
+00004e20: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
+00004e30: 696e 6974 5f73 696e 676c 6528 7661 7269  init_single(vari
+00004e40: 6162 6c65 2c20 676b 6579 733d 5b27 7265  able, gkeys=['re
+00004e50: 6164 6f6e 6c79 275d 290a 2020 2020 2020  adonly']).      
+00004e60: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
+00004e70: 6e63 6528 6368 6f73 656e 5f6c 6162 656c  nce(chosen_label
+00004e80: 2c20 7374 7229 0a20 2020 2020 2020 206b  , str).        k
+00004e90: 7761 7267 732e 7570 6461 7465 287b 0a20  wargs.update({. 
+00004ea0: 2020 2020 2020 2020 2020 2027 7465 7874             'text
+00004eb0: 273a 2063 686f 7365 6e5f 6c61 6265 6c2c  ': chosen_label,
+00004ec0: 0a20 2020 2020 2020 2020 2020 2027 6f6e  .            'on
+00004ed0: 7661 6c75 6527 3a20 5472 7565 2c0a 2020  value': True,.  
+00004ee0: 2020 2020 2020 2020 2020 276f 6666 7661            'offva
+00004ef0: 6c75 6527 3a20 4661 6c73 652c 0a20 2020  lue': False,.   
+00004f00: 2020 2020 2020 2020 2027 7661 7269 6162           'variab
+00004f10: 6c65 273a 2073 656c 662e 7661 7269 6162  le': self.variab
+00004f20: 6c65 2c0a 2020 2020 2020 2020 7d29 0a20  le,.        }). 
+00004f30: 2020 2020 2020 2073 7570 6572 2829 2e5f         super()._
+00004f40: 5f69 6e69 745f 5f28 7061 7265 6e74 2c20  _init__(parent, 
+00004f50: 2a2a 6b77 6172 6773 2920 2023 2074 746b  **kwargs)  # ttk
+00004f60: 2e43 6865 636b 6275 7474 6f6e 0a20 2020  .Checkbutton.   
+00004f70: 2020 2020 2069 6620 7265 6164 6f6e 6c79       if readonly
+00004f80: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00004f90: 5265 6164 2d6f 6e6c 7920 6368 6563 6b62  Read-only checkb
+00004fa0: 6f78 656e 2061 7265 2065 6469 7461 626c  oxen are editabl
+00004fb0: 652c 2066 6f72 2073 6f6d 6520 7265 6173  e, for some reas
+00004fc0: 6f6e 0a20 2020 2020 2020 2020 2020 2073  on.            s
+00004fd0: 656c 662e 6773 7461 7465 203d 206d 6f64  elf.gstate = mod
+00004fe0: 656c 2e47 7569 5374 6174 6528 656e 6162  el.GuiState(enab
+00004ff0: 6c65 643d 4661 6c73 652c 2072 6561 646f  led=False, reado
+00005000: 6e6c 793d 5472 7565 290a 0a20 2020 2064  nly=True)..    d
+00005010: 6566 2074 6f67 676c 6528 7365 6c66 2920  ef toggle(self) 
+00005020: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00005030: 2027 2727 5377 6974 6368 2074 6865 2076   '''Switch the v
+00005040: 6172 6961 626c 6520 7374 6174 6520 746f  ariable state to
+00005050: 2069 7473 206f 7070 6f73 6974 6520 2860   its opposite (`
+00005060: 6e6f 7420 3c6e 6f74 3e60 292e 2727 270a  not <not>`).'''.
+00005070: 2020 2020 2020 2020 7365 6c66 2e77 7374          self.wst
+00005080: 6174 6520 3d20 6e6f 7420 7365 6c66 2e77  ate = not self.w
+00005090: 7374 6174 650a 0a0a 636c 6173 7320 456e  state...class En
+000050a0: 7472 7928 7474 6b2e 456e 7472 792c 206d  try(ttk.Entry, m
+000050b0: 6978 696e 2e53 696e 676c 6557 6964 6765  ixin.SingleWidge
+000050c0: 7429 3a0a 2020 2020 2727 2741 6e20 656e  t):.    '''An en
+000050d0: 7472 7920 7769 6467 6574 2c20 7369 6e67  try widget, sing
+000050e0: 6c65 2d6c 696e 6520 7465 7874 2065 6469  le-line text edi
+000050f0: 746f 722e 0a0a 2020 2020 5468 6973 2069  tor...    This i
+00005100: 7320 616e 2065 6e74 7279 2062 6f78 2c20  s an entry box, 
+00005110: 6120 7369 6e67 6c65 2d6c 696e 6520 6564  a single-line ed
+00005120: 6974 6f72 2066 6f72 2073 7472 696e 6773  itor for strings
+00005130: 2e20 5468 6520 6d61 696e 0a20 2020 2069  . The main.    i
+00005140: 6e74 6572 6163 7469 6f6e 2069 7320 6564  nteraction is ed
+00005150: 6974 696e 6720 7468 6520 7465 7874 2063  iting the text c
+00005160: 6f6e 7461 696e 6564 2077 6974 6869 6e2e  ontained within.
+00005170: 0a0a 2020 2020 5468 6520 7374 6174 6520  ..    The state 
+00005180: 6973 2061 2073 696e 676c 6520 6073 7472  is a single `str
+00005190: 6020 7661 6c75 652e 0a0a 2020 2020 5468  ` value...    Th
+000051a0: 6572 6520 6973 206e 6f20 5079 7468 6f6e  ere is no Python
+000051b0: 2064 6f63 756d 656e 7461 7469 6f6e 2c20   documentation, 
+000051c0: 7365 6520 6060 546b 6060 2060 7474 6b2e  see ``Tk`` `ttk.
+000051d0: 456e 7472 7920 3c68 7474 7073 3a2f 2f77  Entry <https://w
+000051e0: 7777 2e74 636c 2e74 6b2f 6d61 6e2f 7463  ww.tcl.tk/man/tc
+000051f0: 6c2f 546b 436d 642f 7474 6b5f 656e 7472  l/TkCmd/ttk_entr
+00005200: 792e 6874 6d6c 3e60 5f20 646f 6375 6d65  y.html>`_ docume
+00005210: 6e74 6174 696f 6e2e 0a0a 2020 2020 4172  ntation...    Ar
+00005220: 6773 3a0a 2020 2020 2020 2020 7661 7269  gs:.        vari
+00005230: 6162 6c65 3a20 5573 6520 616e 2065 7874  able: Use an ext
+00005240: 6572 6e61 6c6c 7920 6465 6669 6e65 6420  ernally defined 
+00005250: 7661 7269 6162 6c65 2c20 696e 7374 6561  variable, instea
+00005260: 6420 6f66 2063 7265 6174 696e 6720 6120  d of creating a 
+00005270: 6e65 7720 6f6e 6520 7370 6563 6966 6963  new one specific
+00005280: 2066 6f72 2074 6869 7320 7769 6467 6574   for this widget
+00005290: 2e0a 0a20 2020 2020 2020 206c 6162 656c  ...        label
+000052a0: 3a20 5468 6520 6c61 6265 6c20 746f 2069  : The label to i
+000052b0: 6e63 6c75 6465 2062 6573 6964 6573 2074  nclude besides t
+000052c0: 6865 2065 6e74 7279 2e20 2a2a 4e6f 7420  he entry. **Not 
+000052d0: 696d 706c 656d 656e 7465 6420 7965 742a  implemented yet*
+000052e0: 2a2e 0a20 2020 2020 2020 2070 6172 656e  *..        paren
+000052f0: 743a 2054 6865 2070 6172 656e 7420 7769  t: The parent wi
+00005300: 6467 6574 2e20 4361 6e20 6265 2061 2060  dget. Can be a `
+00005310: 526f 6f74 5769 6e64 6f77 6020 6f72 2061  RootWindow` or a
+00005320: 6e6f 7468 6572 2060 6d69 7869 6e2e 436f  nother `mixin.Co
+00005330: 6e74 6169 6e65 7257 6964 6765 7460 2e0a  ntainerWidget`..
+00005340: 2020 2020 2727 270a 2020 2020 7374 6174      '''.    stat
+00005350: 655f 7479 7065 203d 2076 6172 2e53 7472  e_type = var.Str
+00005360: 696e 670a 0a20 2020 2064 6566 205f 5f69  ing..    def __i
+00005370: 6e69 745f 5f28 7365 6c66 2c20 7061 7265  nit__(self, pare
+00005380: 6e74 2c20 2a2c 2076 6172 6961 626c 653a  nt, *, variable:
+00005390: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+000053a0: 5b76 6172 2e53 7472 696e 675d 203d 204e  [var.String] = N
+000053b0: 6f6e 652c 206c 6162 656c 3a20 7479 7069  one, label: typi
+000053c0: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
+000053d0: 203d 204e 6f6e 652c 202a 2a6b 7761 7267   = None, **kwarg
+000053e0: 7329 3a0a 2020 2020 2020 2020 7365 6c66  s):.        self
+000053f0: 2e69 6e69 745f 7369 6e67 6c65 2876 6172  .init_single(var
+00005400: 6961 626c 6529 0a20 2020 2020 2020 2073  iable).        s
+00005410: 656c 662e 6c61 6265 6c20 3d20 6c61 6265  elf.label = labe
+00005420: 6c20 6f72 2027 2720 2023 2054 4f44 4f3a  l or ''  # TODO:
+00005430: 2053 686f 7720 6c61 6265 6c20 736f 6d65   Show label some
+00005440: 686f 773f 0a20 2020 2020 2020 206b 7761  how?.        kwa
+00005450: 7267 732e 7570 6461 7465 287b 0a20 2020  rgs.update({.   
+00005460: 2020 2020 2020 2020 2027 7465 7874 7661           'textva
+00005470: 7269 6162 6c65 273a 2073 656c 662e 7661  riable': self.va
+00005480: 7269 6162 6c65 2c0a 2020 2020 2020 2020  riable,.        
+00005490: 7d29 0a20 2020 2020 2020 2073 7570 6572  }).        super
+000054a0: 2829 2e5f 5f69 6e69 745f 5f28 7061 7265  ().__init__(pare
+000054b0: 6e74 2c20 2a2a 6b77 6172 6773 2920 2023  nt, **kwargs)  #
+000054c0: 2074 746b 2e45 6e74 7279 0a20 2020 2020   ttk.Entry.     
+000054d0: 2020 2069 6620 5f5f 6465 6275 675f 5f3a     if __debug__:
+000054e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000054f0: 6c61 6265 6c20 6973 206e 6f74 204e 6f6e  label is not Non
+00005500: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00005510: 2020 2077 6172 6e69 6e67 732e 7761 726e     warnings.warn
+00005520: 2866 277b 7365 6c66 7d3a 204c 6162 656c  (f'{self}: Label
+00005530: 7320 6f6e 2045 6e74 7279 2061 7265 2073  s on Entry are s
+00005540: 7469 6c6c 2075 6e73 7570 706f 7274 6564  till unsupported
+00005550: 2e20 496e 636c 7564 6520 6120 4c61 6265  . Include a Labe
+00005560: 6c20 6d61 6e75 616c 6c79 2e27 2c20 7374  l manually.', st
+00005570: 6163 6b6c 6576 656c 3d32 290a 0a0a 636c  acklevel=2)...cl
+00005580: 6173 7320 436f 6d62 6f62 6f78 2874 746b  ass Combobox(ttk
+00005590: 2e43 6f6d 626f 626f 782c 206d 6978 696e  .Combobox, mixin
+000055a0: 2e53 696e 676c 6557 6964 6765 7429 3a0a  .SingleWidget):.
+000055b0: 2020 2020 2727 2741 2063 6f6d 626f 626f      '''A combobo
+000055c0: 7820 7769 6467 6574 2c20 636f 6d62 696e  x widget, combin
+000055d0: 696e 6720 616e 2060 456e 7472 7960 2077  ing an `Entry` w
+000055e0: 6974 6820 6120 604c 6973 7462 6f78 602e  ith a `Listbox`.
+000055f0: 0a0a 2020 2020 5468 6973 2069 7320 6120  ..    This is a 
+00005600: 636f 6d62 6f62 6f78 2c20 616e 2060 456e  combobox, an `En
+00005610: 7472 7960 2077 6974 6820 6120 6275 7474  try` with a butt
+00005620: 6f6e 2074 6861 7420 7368 6f77 7320 6120  on that shows a 
+00005630: 706f 702d 7570 2060 4c69 7374 626f 7860  pop-up `Listbox`
+00005640: 0a20 2020 2077 6974 6820 736f 6d65 2070  .    with some p
+00005650: 7265 6465 6669 6e65 6420 6060 7661 6c75  redefined ``valu
+00005660: 6573 6060 2e0a 0a20 2020 2054 6865 2065  es``...    The e
+00005670: 6e74 7279 2063 616e 2062 6520 6060 7265  ntry can be ``re
+00005680: 6164 6f6e 6c79 6060 2c20 696e 2077 6869  adonly``, in whi
+00005690: 6368 2063 6173 6520 7468 6520 6f6e 6c79  ch case the only
+000056a0: 2070 6f73 7369 626c 6520 7661 6c75 6573   possible values
+000056b0: 2061 7265 0a20 2020 2074 6865 206f 6e65   are.    the one
+000056c0: 7320 7368 6f77 6e20 6f6e 2074 6865 2076  s shown on the v
+000056d0: 616c 7565 206c 6973 742c 206f 7468 6572  alue list, other
+000056e0: 7769 7365 2074 6865 2065 6e74 7279 2069  wise the entry i
+000056f0: 7320 6564 6974 6162 6c65 2077 6974 680a  s editable with.
+00005700: 2020 2020 6172 6269 7472 6172 7920 7661      arbitrary va
+00005710: 6c75 6573 2c20 6a75 7374 206c 696b 6520  lues, just like 
+00005720: 616e 7920 6045 6e74 7279 602e 0a0a 2020  any `Entry`...  
+00005730: 2020 5468 6520 6060 696d 6d65 6469 6174    The ``immediat
+00005740: 6560 6020 7061 7261 6d65 7465 7220 6361  e`` parameter ca
+00005750: 6e20 6265 2075 7365 6420 746f 2063 6f6e  n be used to con
+00005760: 7472 6f6c 2077 6865 6e20 6973 2074 6865  trol when is the
+00005770: 2064 6566 6175 6c74 0a20 2020 2076 616c   default.    val
+00005780: 7565 2073 6574 7570 2e20 4465 6661 756c  ue setup. Defaul
+00005790: 7473 2074 6f20 6265 696e 6720 7365 7420  ts to being set 
+000057a0: 6f6e 6c79 2077 6865 6e20 7468 6520 4755  only when the GU
+000057b0: 4920 7374 6162 696c 697a 6573 2c20 6275  I stabilizes, bu
+000057c0: 7420 6974 2063 616e 0a20 2020 2062 6520  t it can.    be 
+000057d0: 7365 7420 6173 2073 6f6f 6e20 6173 2070  set as soon as p
+000057e0: 6f73 7369 626c 652e 0a0a 2020 2020 5468  ossible...    Th
+000057f0: 6572 6520 6973 206e 6f20 5079 7468 6f6e  ere is no Python
+00005800: 2064 6f63 756d 656e 7461 7469 6f6e 2c20   documentation, 
+00005810: 7365 6520 6060 546b 6060 2060 7474 6b2e  see ``Tk`` `ttk.
+00005820: 436f 6d62 6f62 6f78 203c 6874 7470 733a  Combobox <https:
+00005830: 2f2f 7777 772e 7463 6c2e 746b 2f6d 616e  //www.tcl.tk/man
+00005840: 2f74 636c 2f54 6b43 6d64 2f74 746b 5f63  /tcl/TkCmd/ttk_c
+00005850: 6f6d 626f 626f 782e 6874 6d6c 3e60 5f20  ombobox.html>`_ 
+00005860: 646f 6375 6d65 6e74 6174 696f 6e2e 0a0a  documentation...
+00005870: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00005880: 2020 7661 6c75 6573 3a20 4120 636f 756e    values: A coun
+00005890: 7461 626c 6520 7370 6563 6966 6963 6174  table specificat
+000058a0: 696f 6e20 6f66 2076 616c 7565 7320 746f  ion of values to
+000058b0: 2073 686f 7720 6f6e 2074 6865 2070 6f70   show on the pop
+000058c0: 2d75 7020 6c69 7374 626f 782e 0a20 2020  -up listbox..   
+000058d0: 2020 2020 2072 6561 646f 6e6c 793a 2053       readonly: S
+000058e0: 686f 756c 6420 7468 6520 7769 6467 6574  hould the widget
+000058f0: 2061 6c6c 6f77 2069 6e74 6572 6163 7469   allow interacti
+00005900: 6f6e 2074 6f20 6368 616e 6765 2069 7473  on to change its
+00005910: 2076 616c 7565 2e0a 2020 2020 2020 2020   value..        
+00005920: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
+00005930: 2a64 6973 616c 6c6f 7769 6e67 2a20 696e  *disallowing* in
+00005940: 7465 7261 6374 696f 6e2e 0a20 2020 2020  teraction..     
+00005950: 2020 2069 6d6d 6564 6961 7465 3a20 5365     immediate: Se
+00005960: 7420 7468 6520 6465 6661 756c 7420 7661  t the default va
+00005970: 6c75 6520 4153 4150 2028 6054 7275 6560  lue ASAP (`True`
+00005980: 292c 206f 7220 6465 6c61 7920 6974 2061  ), or delay it a
+00005990: 6674 6572 2074 6865 0a20 2020 2020 2020  fter the.       
+000059a0: 2020 2020 2047 5549 2069 7320 7374 6162       GUI is stab
+000059b0: 6c65 2028 6046 616c 7365 6029 2e20 4465  le (`False`). De
+000059c0: 6661 756c 7473 2074 6f20 6046 616c 7365  faults to `False
+000059d0: 602e 0a20 2020 2020 2020 2076 6172 6961  `..        varia
+000059e0: 626c 653a 2055 7365 2061 6e20 6578 7465  ble: Use an exte
+000059f0: 726e 616c 6c79 2064 6566 696e 6564 2076  rnally defined v
+00005a00: 6172 6961 626c 652c 2069 6e73 7465 6164  ariable, instead
+00005a10: 206f 6620 6372 6561 7469 6e67 2061 206e   of creating a n
+00005a20: 6577 0a20 2020 2020 2020 2020 2020 206f  ew.            o
+00005a30: 6e65 2073 7065 6369 6669 6320 666f 7220  ne specific for 
+00005a40: 7468 6973 2077 6964 6765 742e 0a0a 2020  this widget...  
+00005a50: 2020 2020 2020 6c61 6265 6c3a 2054 6865        label: The
+00005a60: 206c 6162 656c 2074 6f20 696e 636c 7564   label to includ
+00005a70: 6520 6265 7369 6465 7320 7468 6520 636f  e besides the co
+00005a80: 6d62 6f62 6f78 2e20 2a2a 4e6f 7420 696d  mbobox. **Not im
+00005a90: 706c 656d 656e 7465 6420 7965 742a 2a2e  plemented yet**.
+00005aa0: 0a20 2020 2020 2020 2070 6172 656e 743a  .        parent:
+00005ab0: 2054 6865 2070 6172 656e 7420 7769 6467   The parent widg
+00005ac0: 6574 2e20 4361 6e20 6265 2061 2060 526f  et. Can be a `Ro
+00005ad0: 6f74 5769 6e64 6f77 6020 6f72 2061 6e6f  otWindow` or ano
+00005ae0: 7468 6572 2060 6d69 7869 6e2e 436f 6e74  ther `mixin.Cont
+00005af0: 6169 6e65 7257 6964 6765 7460 2e0a 0a20  ainerWidget`... 
+00005b00: 2020 202e 2e20 6175 746f 6174 7472 6962     .. autoattrib
+00005b10: 7574 653a 3a20 7370 6563 5661 6c75 6573  ute:: specValues
+00005b20: 0a20 2020 2027 2727 0a20 2020 2073 7461  .    '''.    sta
+00005b30: 7465 5f74 7970 6520 3d20 7661 722e 5374  te_type = var.St
+00005b40: 7269 6e67 0a0a 2020 2020 6465 6620 5f5f  ring..    def __
+00005b50: 696e 6974 5f5f 2873 656c 662c 2070 6172  init__(self, par
+00005b60: 656e 742c 2076 616c 7565 733a 2073 7065  ent, values: spe
+00005b70: 632e 5370 6563 436f 756e 7461 626c 652c  c.SpecCountable,
+00005b80: 202a 2c20 7265 6164 6f6e 6c79 3a20 626f   *, readonly: bo
+00005b90: 6f6c 203d 2054 7275 652c 2069 6d6d 6564  ol = True, immed
+00005ba0: 6961 7465 3a20 626f 6f6c 203d 2046 616c  iate: bool = Fal
+00005bb0: 7365 2c20 7661 7269 6162 6c65 3a20 7479  se, variable: ty
+00005bc0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7661  ping.Optional[va
+00005bd0: 722e 5374 7269 6e67 5d20 3d20 4e6f 6e65  r.String] = None
+00005be0: 2c20 6c61 6265 6c3a 2074 7970 696e 672e  , label: typing.
+00005bf0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00005c00: 4e6f 6e65 2c20 2a2a 6b77 6172 6773 293a  None, **kwargs):
+00005c10: 0a20 2020 2020 2020 2073 656c 662e 696e  .        self.in
+00005c20: 6974 5f73 696e 676c 6528 7661 7269 6162  it_single(variab
+00005c30: 6c65 2c20 676b 6579 733d 5b27 7265 6164  le, gkeys=['read
+00005c40: 6f6e 6c79 275d 290a 2020 2020 2020 2020  only']).        
+00005c50: 7365 6c66 2e6c 6162 656c 203d 206c 6162  self.label = lab
+00005c60: 656c 206f 7220 2727 2020 2320 544f 444f  el or ''  # TODO
+00005c70: 3a20 5368 6f77 206c 6162 656c 2073 6f6d  : Show label som
+00005c80: 6568 6f77 0a20 2020 2020 2020 2073 656c  ehow.        sel
+00005c90: 662e 7370 6563 5661 6c75 6573 203d 2076  f.specValues = v
+00005ca0: 616c 7565 730a 2020 2020 2020 2020 6b77  alues.        kw
+00005cb0: 6172 6773 2e75 7064 6174 6528 7b0a 2020  args.update({.  
+00005cc0: 2020 2020 2020 2020 2020 2774 6578 7476            'textv
+00005cd0: 6172 6961 626c 6527 3a20 7365 6c66 2e76  ariable': self.v
+00005ce0: 6172 6961 626c 652c 0a20 2020 2020 2020  ariable,.       
+00005cf0: 2020 2020 2027 7661 6c75 6573 273a 206c       'values': l
+00005d00: 6973 7428 7365 6c66 2e73 7065 6356 616c  ist(self.specVal
+00005d10: 7565 732e 616c 6c28 2929 2c0a 2020 2020  ues.all()),.    
+00005d20: 2020 2020 7d29 0a20 2020 2020 2020 2073      }).        s
+00005d30: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
+00005d40: 7061 7265 6e74 2c20 2a2a 6b77 6172 6773  parent, **kwargs
+00005d50: 2920 2023 2074 746b 2e43 6f6d 626f 626f  )  # ttk.Combobo
+00005d60: 780a 2020 2020 2020 2020 6966 2069 6d6d  x.        if imm
+00005d70: 6564 6961 7465 3a0a 2020 2020 2020 2020  ediate:.        
+00005d80: 2020 2020 7365 6c66 2e73 6574 4465 6661      self.setDefa
+00005d90: 756c 7428 290a 2020 2020 2020 2020 656c  ult().        el
+00005da0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00005db0: 7365 6c66 2e61 6674 6572 5f69 646c 6528  self.after_idle(
+00005dc0: 7365 6c66 2e73 6574 4465 6661 756c 7429  self.setDefault)
+00005dd0: 2020 2320 4e6f 206e 6565 6420 666f 7220    # No need for 
+00005de0: 6120 6054 696d 656f 7574 4964 6c65 6020  a `TimeoutIdle` 
+00005df0: 6865 7265 0a20 2020 2020 2020 2069 6620  here.        if 
+00005e00: 7265 6164 6f6e 6c79 3a0a 2020 2020 2020  readonly:.      
+00005e10: 2020 2020 2020 7365 6c66 2e67 7374 6174        self.gstat
+00005e20: 6520 3d20 6d6f 6465 6c2e 4775 6953 7461  e = model.GuiSta
+00005e30: 7465 2872 6561 646f 6e6c 793d 5472 7565  te(readonly=True
+00005e40: 290a 2020 2020 2020 2020 6966 205f 5f64  ).        if __d
+00005e50: 6562 7567 5f5f 3a0a 2020 2020 2020 2020  ebug__:.        
+00005e60: 2020 2020 2320 4465 6669 6e65 2061 6c6c      # Define all
+00005e70: 2074 6865 206c 6f63 616c 2073 7562 636c   the local subcl
+00005e80: 6173 7365 7320 2874 6861 7420 6f76 6572  asses (that over
+00005e90: 7269 6465 205f 5f69 6e69 745f 5f29 2074  ride __init__) t
+00005ea0: 6f20 696d 7072 6f76 6520 6c6f 6767 696e  o improve loggin
+00005eb0: 670a 2020 2020 2020 2020 2020 2020 5f64  g.            _d
+00005ec0: 656c 7461 6c65 7665 6c20 3d20 3120 6966  eltalevel = 1 if
+00005ed0: 2069 7369 6e73 7461 6e63 6528 7365 6c66   isinstance(self
+00005ee0: 2c20 2843 6f6d 626f 626f 784d 6170 2c29  , (ComboboxMap,)
+00005ef0: 2920 656c 7365 2030 0a20 2020 2020 2020  ) else 0.       
+00005f00: 2020 2020 2069 6620 6e6f 7420 6973 696e       if not isin
+00005f10: 7374 616e 6365 2873 656c 662c 2043 6f6d  stance(self, Com
+00005f20: 626f 626f 784d 6170 2920 616e 6420 6973  boboxMap) and is
+00005f30: 696e 7374 616e 6365 2873 656c 662e 7370  instance(self.sp
+00005f40: 6563 5661 6c75 6573 2c20 7370 6563 2e53  ecValues, spec.S
+00005f50: 7461 7469 634d 6170 293a 0a20 2020 2020  taticMap):.     
+00005f60: 2020 2020 2020 2020 2020 2077 6172 6e69             warni
+00005f70: 6e67 732e 7761 726e 2866 277b 7365 6c66  ngs.warn(f'{self
+00005f80: 7d3a 2053 6565 2060 436f 6d62 6f62 6f78  }: See `Combobox
+00005f90: 4d61 7060 2066 6f72 2075 7369 6e67 2074  Map` for using t
+00005fa0: 6865 2076 616c 7565 7320 636f 7272 6563  he values correc
+00005fb0: 746c 7927 2c20 7374 6163 6b6c 6576 656c  tly', stacklevel
+00005fc0: 3d32 202b 205f 6465 6c74 616c 6576 656c  =2 + _deltalevel
+00005fd0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00005fe0: 206c 6162 656c 2069 7320 6e6f 7420 4e6f   label is not No
+00005ff0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00006000: 2020 2020 7761 726e 696e 6773 2e77 6172      warnings.war
+00006010: 6e28 6627 7b73 656c 667d 3a20 4c61 6265  n(f'{self}: Labe
+00006020: 6c73 206f 6e20 436f 6d62 6f62 6f78 2061  ls on Combobox a
+00006030: 7265 2073 7469 6c6c 2075 6e73 7570 706f  re still unsuppo
+00006040: 7274 6564 2e20 496e 636c 7564 6520 6120  rted. Include a 
+00006050: 4c61 6265 6c20 6d61 6e75 616c 6c79 2e27  Label manually.'
+00006060: 2c20 7374 6163 6b6c 6576 656c 3d32 202b  , stacklevel=2 +
+00006070: 205f 6465 6c74 616c 6576 656c 290a 0a20   _deltalevel).. 
+00006080: 2020 2023 2054 4f44 4f3a 2054 6869 7320     # TODO: This 
+00006090: 636f 756c 6420 6265 2061 2063 6f6d 6d6f  could be a commo
+000060a0: 6e20 606d 6978 696e 2e53 696e 676c 6557  n `mixin.SingleW
+000060b0: 6964 6765 7460 206d 6574 686f 643f 0a20  idget` method?. 
+000060c0: 2020 2064 6566 2073 6574 4465 6661 756c     def setDefaul
+000060d0: 7428 7365 6c66 2920 2d3e 204e 6f6e 653a  t(self) -> None:
+000060e0: 0a20 2020 2020 2020 2027 2727 5365 7420  .        '''Set 
+000060f0: 7468 6520 6375 7272 656e 7420 7374 6174  the current stat
+00006100: 6520 746f 2074 6865 2064 6566 6175 6c74  e to the default
+00006110: 206c 6162 656c 2e27 2727 0a20 2020 2020   label.'''.     
+00006120: 2020 2073 656c 662e 7773 7461 7465 203d     self.wstate =
+00006130: 2073 656c 662e 7370 6563 5661 6c75 6573   self.specValues
+00006140: 2e64 6566 6175 6c74 0a0a 2020 2020 2320  .default..    # 
+00006150: 544f 444f 3a20 5468 6973 2063 6f75 6c64  TODO: This could
+00006160: 2062 6520 6120 636f 6d6d 6f6e 2060 6d69   be a common `mi
+00006170: 7869 6e2e 5369 6e67 6c65 5769 6467 6574  xin.SingleWidget
+00006180: 6020 6d65 7468 6f64 3f0a 2020 2020 6465  ` method?.    de
+00006190: 6620 6553 6574 2873 656c 662c 206c 6162  f eSet(self, lab
+000061a0: 656c 3a20 7374 7229 202d 3e20 7479 7069  el: str) -> typi
+000061b0: 6e67 2e43 616c 6c61 626c 655b 2e2e 2e2c  ng.Callable[...,
+000061c0: 204e 6f6e 655d 3a0a 2020 2020 2020 2020   None]:.        
+000061d0: 2727 2752 6574 7572 6e20 616e 2065 7665  '''Return an eve
+000061e0: 6e74 2066 756e 6374 696f 6e20 746f 2073  nt function to s
+000061f0: 6574 2074 6865 2073 7461 7465 2061 2063  et the state a c
+00006200: 6572 7461 696e 206c 6162 656c 2e27 2727  ertain label.'''
+00006210: 0a20 2020 2020 2020 2069 6620 6c61 6265  .        if labe
+00006220: 6c20 6e6f 7420 696e 2073 656c 662e 7370  l not in self.sp
+00006230: 6563 5661 6c75 6573 3a0a 2020 2020 2020  ecValues:.      
+00006240: 2020 2020 2020 7261 6973 6520 6578 6365        raise exce
+00006250: 7074 696f 6e2e 496e 7661 6c69 6443 616c  ption.InvalidCal
+00006260: 6c62 6163 6b44 6566 696e 6974 696f 6e28  lbackDefinition(
+00006270: 6627 5365 7474 696e 6720 616e 2069 6e76  f'Setting an inv
+00006280: 616c 6964 206c 6162 656c 3a20 7b6c 6162  alid label: {lab
+00006290: 656c 7d27 290a 0a20 2020 2020 2020 2064  el}')..        d
+000062a0: 6566 2065 5365 7428 293a 0a20 2020 2020  ef eSet():.     
+000062b0: 2020 2020 2020 2073 656c 662e 7773 7461         self.wsta
+000062c0: 7465 203d 206c 6162 656c 0a20 2020 2020  te = label.     
+000062d0: 2020 2072 6574 7572 6e20 6553 6574 0a0a     return eSet..
+000062e0: 0a63 6c61 7373 2043 6f6d 626f 626f 784d  .class ComboboxM
+000062f0: 6170 2843 6f6d 626f 626f 7829 3a0a 2020  ap(Combobox):.  
+00006300: 2020 2727 2741 2063 6f6d 626f 626f 7820    '''A combobox 
+00006310: 7769 6467 6574 2c20 7072 6570 6172 6564  widget, prepared
+00006320: 2074 6f20 7573 6520 6073 7065 632e 5374   to use `spec.St
+00006330: 6174 6963 4d61 7060 2e0a 0a20 2020 2054  aticMap`...    T
+00006340: 6869 7320 6973 206a 7573 7420 6120 6e6f  his is just a no
+00006350: 726d 616c 2060 436f 6d62 6f62 6f78 602c  rmal `Combobox`,
+00006360: 2062 7574 2074 6865 2060 6076 616c 7565   but the ``value
+00006370: 7360 6020 6f62 6a65 6374 206d 7573 7420  s`` object must 
+00006380: 6265 2061 0a20 2020 2060 7370 6563 2e53  be a.    `spec.S
+00006390: 7461 7469 634d 6170 602c 2061 6e64 2074  taticMap`, and t
+000063a0: 6865 2077 6964 6765 7420 7661 6c75 6520  he widget value 
+000063b0: 7769 6c6c 2062 6520 7265 7475 726e 6564  will be returned
+000063c0: 2061 7320 6974 7320 7661 6c75 652c 206e   as its value, n
+000063d0: 6f74 0a20 2020 2074 6865 206c 6162 656c  ot.    the label
+000063e0: 2e0a 0a20 2020 204e 6f74 653a 0a20 2020  ...    Note:.   
+000063f0: 2020 2020 2054 6869 7320 6973 2073 7469       This is sti
+00006400: 6c6c 2057 4950 2c20 7365 656d 7320 6c69  ll WIP, seems li
+00006410: 6b65 2061 2076 6572 7920 6269 6720 6861  ke a very big ha
+00006420: 636b 2066 6f72 206e 6f77 2e0a 2020 2020  ck for now..    
+00006430: 2727 270a 2020 2020 6465 6620 5f5f 696e  '''.    def __in
+00006440: 6974 5f5f 2873 656c 662c 202a 6172 6773  it__(self, *args
+00006450: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
+00006460: 2020 2020 2073 7570 6572 2829 2e5f 5f69       super().__i
+00006470: 6e69 745f 5f28 2a61 7267 732c 202a 2a6b  nit__(*args, **k
+00006480: 7761 7267 7329 0a20 2020 2020 2020 2061  wargs).        a
+00006490: 7373 6572 7420 6973 696e 7374 616e 6365  ssert isinstance
+000064a0: 2873 656c 662e 7370 6563 5661 6c75 6573  (self.specValues
+000064b0: 2c20 7370 6563 2e53 7461 7469 634d 6170  , spec.StaticMap
+000064c0: 292c 2066 277b 7365 6c66 7d3a 2076 616c  ), f'{self}: val
+000064d0: 7565 7320 6d75 7374 2062 6520 6120 6073  ues must be a `s
+000064e0: 7065 632e 5374 6174 6963 4d61 7060 270a  pec.StaticMap`'.
+000064f0: 0a20 2020 2064 6566 2073 7461 7465 5f67  .    def state_g
+00006500: 6574 2873 656c 662c 202a 6172 6773 2c20  et(self, *args, 
+00006510: 2a2a 6b77 6172 6773 293a 0a20 2020 2020  **kwargs):.     
+00006520: 2020 2027 2727 2727 2720 2023 2044 6f20     ''''''  # Do 
+00006530: 6e6f 7420 646f 6375 6d65 6e74 0a20 2020  not document.   
+00006540: 2020 2020 206c 6162 656c 203d 2073 7570       label = sup
+00006550: 6572 2829 2e73 7461 7465 5f67 6574 282a  er().state_get(*
+00006560: 6172 6773 2c20 2a2a 6b77 6172 6773 290a  args, **kwargs).
+00006570: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
+00006580: 7365 6c66 2e73 7065 6356 616c 7565 732e  self.specValues.
+00006590: 7661 6c75 6528 6c61 6265 6c29 0a20 2020  value(label).   
+000065a0: 2020 2020 2023 2069 6620 5f5f 6465 6275       # if __debu
+000065b0: 675f 5f3a 0a20 2020 2020 2020 2023 2020  g__:.        #  
+000065c0: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+000065d0: 274c 5b25 735d 203d 3e20 2572 272c 206c  'L[%s] => %r', l
+000065e0: 6162 656c 2c20 7661 6c75 6529 0a20 2020  abel, value).   
+000065f0: 2020 2020 2072 6574 7572 6e20 6d6f 6465       return mode
+00006600: 6c2e 5653 7461 7465 2876 616c 7565 2c20  l.VState(value, 
+00006610: 6c61 6265 6c3d 6c61 6265 6c29 0a0a 2020  label=label)..  
+00006620: 2020 6465 6620 7374 6174 655f 7365 7428    def state_set(
+00006630: 7365 6c66 2c20 7374 6174 652c 202a 6172  self, state, *ar
+00006640: 6773 2c20 2a2a 6b77 6172 6773 293a 0a20  gs, **kwargs):. 
+00006650: 2020 2020 2020 2027 2727 2727 2720 2023         ''''''  #
+00006660: 2044 6f20 6e6f 7420 646f 6375 6d65 6e74   Do not document
+00006670: 0a20 2020 2020 2020 2023 2053 7570 706f  .        # Suppo
+00006680: 7274 2073 6574 7469 6e67 206c 6162 656c  rt setting label
+00006690: 7320 616e 6420 5653 7461 7465 0a20 2020  s and VState.   
+000066a0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+000066b0: 6365 2873 7461 7465 2c20 6d6f 6465 6c2e  ce(state, model.
+000066c0: 5653 7461 7465 293a 0a20 2020 2020 2020  VState):.       
+000066d0: 2020 2020 206c 6162 656c 203d 2073 656c       label = sel
+000066e0: 662e 7370 6563 5661 6c75 6573 2e6c 6162  f.specValues.lab
+000066f0: 656c 2873 7461 7465 2e76 616c 7565 290a  el(state.value).
+00006700: 2020 2020 2020 2020 2020 2020 6966 205f              if _
+00006710: 5f64 6562 7567 5f5f 3a0a 2020 2020 2020  _debug__:.      
+00006720: 2020 2020 2020 2020 2020 6966 2073 7461            if sta
+00006730: 7465 2e6c 6162 656c 3a0a 2020 2020 2020  te.label:.      
+00006740: 2020 2020 2020 2020 2020 2020 2020 6173                as
+00006750: 7365 7274 2073 7461 7465 2e6c 6162 656c  sert state.label
+00006760: 203d 3d20 6c61 6265 6c0a 2020 2020 2020   == label.      
+00006770: 2020 2020 2020 2020 2020 2320 6c6f 6767            # logg
+00006780: 6572 2e64 6562 7567 2827 2572 203d 3e20  er.debug('%r => 
+00006790: 2573 272c 2073 7461 7465 2c20 6c61 6265  %s', state, labe
+000067a0: 6c29 0a20 2020 2020 2020 2065 6c73 653a  l).        else:
+000067b0: 2020 2320 5365 7474 696e 6720 6120 7369    # Setting a si
+000067c0: 6d70 6c65 206c 6162 656c 0a20 2020 2020  mple label.     
+000067d0: 2020 2020 2020 206c 6162 656c 203d 2073         label = s
+000067e0: 7461 7465 0a20 2020 2020 2020 2020 2020  tate.           
+000067f0: 2069 6620 5f5f 6465 6275 675f 5f3a 0a20   if __debug__:. 
+00006800: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00006810: 6173 7320 2023 206c 6f67 6765 722e 6465  ass  # logger.de
+00006820: 6275 6728 274c 5b25 735d 272c 206c 6162  bug('L[%s]', lab
+00006830: 656c 290a 2020 2020 2020 2020 7265 7475  el).        retu
+00006840: 726e 2073 7570 6572 2829 2e73 7461 7465  rn super().state
+00006850: 5f73 6574 286c 6162 656c 2c20 2a61 7267  _set(label, *arg
+00006860: 732c 202a 2a6b 7761 7267 7329 0a0a 2020  s, **kwargs)..  
+00006870: 2020 6465 6620 6553 6574 5661 6c75 6528    def eSetValue(
+00006880: 7365 6c66 2c20 7661 6c75 6529 3a0a 2020  self, value):.  
+00006890: 2020 2020 2020 2727 2757 7261 7065 7220        '''Wraper 
+000068a0: 666f 7220 6043 6f6d 626f 626f 782e 6553  for `Combobox.eS
+000068b0: 6574 602c 2070 7265 7061 7265 6420 746f  et`, prepared to
+000068c0: 2075 7365 2060 7370 6563 2e53 7461 7469   use `spec.Stati
+000068d0: 634d 6170 602e 2727 270a 2020 2020 2020  cMap`.'''.      
+000068e0: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
+000068f0: 6e63 6528 7365 6c66 2e73 7065 6356 616c  nce(self.specVal
+00006900: 7565 732c 2073 7065 632e 5374 6174 6963  ues, spec.Static
+00006910: 4d61 7029 0a20 2020 2020 2020 2072 6574  Map).        ret
+00006920: 7572 6e20 7365 6c66 2e65 5365 7428 7365  urn self.eSet(se
+00006930: 6c66 2e73 7065 6356 616c 7565 732e 6c61  lf.specValues.la
+00006940: 6265 6c28 7661 6c75 6529 290a 0a20 2020  bel(value))..   
+00006950: 2069 6620 5f5f 6465 6275 675f 5f3a 0a20   if __debug__:. 
+00006960: 2020 2020 2020 2023 2057 6172 6e20 6162         # Warn ab
+00006970: 6f75 7420 7472 6163 6520 7573 6167 650a  out trace usage.
+00006980: 2020 2020 2020 2020 6465 6620 7472 6163          def trac
+00006990: 6528 7365 6c66 2c20 2a61 7267 732c 202a  e(self, *args, *
+000069a0: 2a6b 7761 7267 7329 3a0a 2020 2020 2020  *kwargs):.      
+000069b0: 2020 2020 2020 6966 2073 656c 662e 7370        if self.sp
+000069c0: 6563 5661 6c75 6573 206e 6f74 2069 6e20  ecValues not in 
+000069d0: 6b77 6172 6773 2e76 616c 7565 7328 293a  kwargs.values():
+000069e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000069f0: 2077 6172 6e69 6e67 732e 7761 726e 2827   warnings.warn('
+00006a00: 4d61 6b65 2073 7572 6520 746f 2073 656e  Make sure to sen
+00006a10: 6420 6073 656c 662e 7370 6563 5661 6c75  d `self.specValu
+00006a20: 6573 6020 746f 2067 6574 2074 6865 2022  es` to get the "
+00006a30: 7265 616c 2220 7661 6c75 6573 272c 2073  real" values', s
+00006a40: 7461 636b 6c65 7665 6c3d 3229 0a20 2020  tacklevel=2).   
+00006a50: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00006a60: 7375 7065 7228 292e 7472 6163 6528 2a61  super().trace(*a
+00006a70: 7267 732c 202a 2a6b 7761 7267 7329 0a0a  rgs, **kwargs)..
+00006a80: 0a63 6c61 7373 2046 7261 6d65 5374 6174  .class FrameStat
+00006a90: 6566 756c 2874 746b 2e4c 6162 656c 4672  eful(ttk.LabelFr
+00006aa0: 616d 652c 206d 6978 696e 2e43 6f6e 7461  ame, mixin.Conta
+00006ab0: 696e 6572 5769 6467 6574 293a 0a20 2020  inerWidget):.   
+00006ac0: 2027 2727 4120 6672 616d 6520 746f 2068   '''A frame to h
+00006ad0: 6f6c 6420 6f74 6865 7220 7769 6467 6574  old other widget
+00006ae0: 732c 2077 6974 6820 6120 6368 6563 6b62  s, with a checkb
+00006af0: 6f78 2e0a 0a20 2020 2054 6869 7320 6973  ox...    This is
+00006b00: 2061 2066 7261 6d65 2077 6974 6820 616e   a frame with an
+00006b10: 2065 6d62 6564 6465 6420 6368 6563 6b62   embedded checkb
+00006b20: 6f78 2060 6373 7461 7465 5f77 6964 6765  ox `cstate_widge
+00006b30: 7460 2061 7320 226c 6162 656c 222e 2054  t` as "label". T
+00006b40: 6869 730a 2020 2020 6c61 6265 6c20 636f  his.    label co
+00006b50: 6e74 726f 6c73 2074 6865 2065 6e61 626c  ntrols the enabl
+00006b60: 6564 2073 7461 7465 206f 6620 7468 6520  ed state of the 
+00006b70: 6368 696c 6420 7769 6467 6574 732e 2059  child widgets. Y
+00006b80: 6f75 2063 616e 2063 6f6e 7472 6f6c 2074  ou can control t
+00006b90: 6865 0a20 2020 2063 6865 636b 626f 7820  he.    checkbox 
+00006ba0: 706f 7369 7469 6f6e 2e0a 0a20 2020 2054  position...    T
+00006bb0: 6865 7265 2069 7320 6e6f 2050 7974 686f  here is no Pytho
+00006bc0: 6e20 646f 6375 6d65 6e74 6174 696f 6e2c  n documentation,
+00006bd0: 2073 6565 2060 6054 6b60 6020 6074 746b   see ``Tk`` `ttk
+00006be0: 2e4c 6162 656c 4672 616d 6520 3c68 7474  .LabelFrame <htt
+00006bf0: 7073 3a2f 2f77 7777 2e74 636c 2e74 6b2f  ps://www.tcl.tk/
+00006c00: 6d61 6e2f 7463 6c2f 546b 436d 642f 7474  man/tcl/TkCmd/tt
+00006c10: 6b5f 6c61 6265 6c66 7261 6d65 2e68 746d  k_labelframe.htm
+00006c20: 6c3e 605f 2064 6f63 756d 656e 7461 7469  l>`_ documentati
+00006c30: 6f6e 2e0a 2020 2020 4e6f 7465 2074 6865  on..    Note the
+00006c40: 2060 606c 6162 656c 7769 6467 6574 6060   ``labelwidget``
+00006c50: 206f 7074 696f 6e2e 0a0a 2020 2020 4172   option...    Ar
+00006c60: 6773 3a0a 2020 2020 2020 2020 6c61 6265  gs:.        labe
+00006c70: 6c3a 2054 6865 206c 6162 656c 2074 6f20  l: The label to 
+00006c80: 696e 636c 7564 6520 6f6e 2074 6865 2066  include on the f
+00006c90: 7261 6d65 2073 6570 6172 6174 6f72 2e20  rame separator. 
+00006ca0: 4361 6e20 6265 2067 6976 656e 2061 7320  Can be given as 
+00006cb0: 6120 636c 6173 7320 7661 7269 6162 6c65  a class variable
+00006cc0: 2e0a 2020 2020 2020 2020 6c61 6265 6c41  ..        labelA
+00006cd0: 6e63 686f 723a 2054 6865 2070 6f73 6974  nchor: The posit
+00006ce0: 696f 6e20 6f66 2074 6865 206c 6162 656c  ion of the label
+00006cf0: 206f 6e20 7468 6520 6672 616d 6520 7365   on the frame se
+00006d00: 7061 7261 746f 722e 0a20 2020 2020 2020  parator..       
+00006d10: 2020 2020 2047 6976 656e 2061 7320 6f6e       Given as on
+00006d20: 6520 6f66 2074 6865 2063 6172 6469 6e61  e of the cardina
+00006d30: 6c20 706f 696e 7473 2e0a 2020 2020 2020  l points..      
+00006d40: 2020 2020 2020 4465 6661 756c 7473 2074        Defaults t
+00006d50: 6f20 6120 4f53 2d73 7065 6369 6669 6320  o a OS-specific 
+00006d60: 6c6f 6361 7469 6f6e 2028 606d 6f64 656c  location (`model
+00006d70: 2e43 502e 6465 6661 756c 7460 292e 0a20  .CP.default`).. 
+00006d80: 2020 2020 2020 2063 7661 7269 6162 6c65         cvariable
+00006d90: 3a20 5573 6520 616e 2065 7874 6572 6e61  : Use an externa
+00006da0: 6c6c 7920 6465 6669 6e65 6420 6063 7374  lly defined `cst
+00006db0: 6174 6560 2076 6172 6961 626c 652c 2069  ate` variable, i
+00006dc0: 6e73 7465 6164 206f 660a 2020 2020 2020  nstead of.      
+00006dd0: 2020 2020 2020 6372 6561 7469 6e67 2061        creating a
+00006de0: 206e 6577 206f 6e65 2073 7065 6369 6669   new one specifi
+00006df0: 6320 666f 7220 7468 6520 6063 7374 6174  c for the `cstat
+00006e00: 6560 2077 6964 6765 742e 0a20 2020 2020  e` widget..     
+00006e10: 2020 2063 7661 7269 6162 6c65 4465 6661     cvariableDefa
+00006e20: 756c 743a 2054 6865 2064 6566 6175 6c74  ult: The default
+00006e30: 2076 616c 7565 2066 6f72 2060 6373 7461   value for `csta
+00006e40: 7465 602e 0a20 2020 2020 2020 2020 2020  te`..           
+00006e50: 2057 6865 6e20 604e 6f6e 6560 2c20 7468   When `None`, th
+00006e60: 6520 7661 6c75 6520 6973 206e 6f74 2063  e value is not c
+00006e70: 6861 6e67 6564 2061 7420 7374 6172 742e  hanged at start.
+00006e80: 0a20 2020 2020 2020 2020 2020 2044 6566  .            Def
+00006e90: 6175 6c74 7320 746f 2073 7461 7274 696e  aults to startin
+00006ea0: 6720 656e 6162 6c65 642c 2075 6e6c 6573  g enabled, unles
+00006eb0: 7320 6060 6376 6172 6961 626c 6560 6020  s ``cvariable`` 
+00006ec0: 6973 2067 6976 656e 2c20 666f 720a 2020  is given, for.  
+00006ed0: 2020 2020 2020 2020 2020 7768 6963 6820            which 
+00006ee0: 7468 6520 7661 6c75 6520 6973 206e 6f74  the value is not
+00006ef0: 2063 6861 6e67 6564 2e0a 2020 2020 2020   changed..      
+00006f00: 2020 6373 7461 7465 4172 6773 3a20 4578    cstateArgs: Ex
+00006f10: 7472 6120 6172 6775 6d65 6e74 7320 666f  tra arguments fo
+00006f20: 7220 7468 6520 6063 7374 6174 6560 2077  r the `cstate` w
+00006f30: 6964 6765 742c 2060 6373 7461 7465 5f77  idget, `cstate_w
+00006f40: 6964 6765 7460 2e0a 0a20 2020 2020 2020  idget`...       
+00006f50: 2070 6172 656e 743a 2054 6865 2070 6172   parent: The par
+00006f60: 656e 7420 7769 6467 6574 2e20 4361 6e20  ent widget. Can 
+00006f70: 6265 2061 2060 526f 6f74 5769 6e64 6f77  be a `RootWindow
+00006f80: 6020 6f72 2061 6e6f 7468 6572 2060 6d69  ` or another `mi
+00006f90: 7869 6e2e 436f 6e74 6169 6e65 7257 6964  xin.ContainerWid
+00006fa0: 6765 7460 2e0a 0a20 2020 2053 6565 2041  get`...    See A
+00006fb0: 6c73 6f3a 0a20 2020 2020 2020 2060 4672  lso:.        `Fr
+00006fc0: 616d 654c 6162 656c 6c65 6460 3a20 4120  ameLabelled`: A 
+00006fd0: 7369 6d70 6c65 7220 7665 7273 696f 6e20  simpler version 
+00006fe0: 6f66 2074 6869 732c 2077 6974 686f 7574  of this, without
+00006ff0: 2074 6865 2065 6d62 6564 6465 6420 6368   the embedded ch
+00007000: 6563 6b62 6f78 2e0a 2020 2020 2727 270a  eckbox..    '''.
+00007010: 2020 2020 6c61 6265 6c3a 2074 7970 696e      label: typin
+00007020: 672e 4f70 7469 6f6e 616c 5b73 7472 5d20  g.Optional[str] 
+00007030: 3d20 4e6f 6e65 0a0a 2020 2020 636c 6173  = None..    clas
+00007040: 7320 5f5f 775f 6373 7461 7465 2843 6865  s __w_cstate(Che
+00007050: 636b 626f 7829 3a0a 2020 2020 2020 2020  ckbox):.        
+00007060: 6973 4865 6c70 6572 203d 2054 7275 650a  isHelper = True.
+00007070: 0a20 2020 2063 7374 6174 655f 7769 6467  .    cstate_widg
+00007080: 6574 3a20 5f5f 775f 6373 7461 7465 0a20  et: __w_cstate. 
+00007090: 2020 2027 2727 5468 6520 7769 6467 6574     '''The widget
+000070a0: 2066 6f72 2074 6865 2065 6d62 6564 6465   for the embedde
+000070b0: 6420 6043 6865 636b 626f 7860 2e0a 0a20  d `Checkbox`... 
+000070c0: 2020 2055 7365 7320 7468 6520 6063 7374     Uses the `cst
+000070d0: 6174 6560 2076 6172 6961 626c 652e 0a0a  ate` variable...
+000070e0: 2020 2020 4e6f 7465 3a0a 2020 2020 2020      Note:.      
+000070f0: 2020 5468 6520 7769 6467 6574 2074 7970    The widget typ
+00007100: 6520 6973 2061 206c 6f63 616c 2060 4368  e is a local `Ch
+00007110: 6563 6b62 6f78 6020 7375 6263 6c61 7373  eckbox` subclass
+00007120: 2c20 7370 6563 6966 6963 2066 6f72 2074  , specific for t
+00007130: 6869 7320 7769 6467 6574 2e0a 2020 2020  his widget..    
+00007140: 2727 270a 2020 2020 6373 7461 7465 3a20  '''.    cstate: 
+00007150: 7661 722e 426f 6f6c 6561 6e0a 2020 2020  var.Boolean.    
+00007160: 2727 2754 6865 2076 6172 6961 626c 6520  '''The variable 
+00007170: 686f 6c64 696e 6720 7468 6520 656d 6265  holding the embe
+00007180: 6464 6564 2060 4368 6563 6b62 6f78 6020  dded `Checkbox` 
+00007190: 7374 6174 652e 0a0a 2020 2020 5573 6564  state...    Used
+000071a0: 206f 6e20 7468 6520 6063 7374 6174 655f   on the `cstate_
+000071b0: 7769 6467 6574 602e 0a0a 2020 2020 5365  widget`...    Se
+000071c0: 6520 416c 736f 3a0a 2020 2020 2020 2020  e Also:.        
+000071d0: 6060 6376 6172 6961 626c 6560 603a 2054  ``cvariable``: T
+000071e0: 6869 7320 6361 6e20 6265 2063 6f6e 6669  his can be confi
+000071f0: 6775 7265 6420 6173 2061 6e20 6578 7465  gured as an exte
+00007200: 726e 616c 2076 6172 6961 626c 652e 0a20  rnal variable.. 
+00007210: 2020 2027 2727 0a0a 2020 2020 6465 6620     '''..    def 
+00007220: 5f5f 696e 6974 5f5f 2873 656c 662c 2070  __init__(self, p
+00007230: 6172 656e 742c 202a 6172 6773 2c20 6c61  arent, *args, la
+00007240: 6265 6c3a 2074 7970 696e 672e 4f70 7469  bel: typing.Opti
+00007250: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00007260: 2c20 6c61 6265 6c41 6e63 686f 723a 206d  , labelAnchor: m
+00007270: 6f64 656c 2e43 5020 3d20 6d6f 6465 6c2e  odel.CP = model.
+00007280: 4350 2e64 6566 6175 6c74 2c0a 2020 2020  CP.default,.    
+00007290: 2020 2020 2020 2020 2020 2020 2063 7661               cva
+000072a0: 7269 6162 6c65 3a20 7479 7069 6e67 2e4f  riable: typing.O
+000072b0: 7074 696f 6e61 6c5b 7661 722e 426f 6f6c  ptional[var.Bool
+000072c0: 6561 6e5d 203d 204e 6f6e 652c 2063 7661  ean] = None, cva
+000072d0: 7269 6162 6c65 4465 6661 756c 743a 2074  riableDefault: t
+000072e0: 7970 696e 672e 4f70 7469 6f6e 616c 5b62  yping.Optional[b
+000072f0: 6f6f 6c5d 203d 204e 6f6e 652c 0a20 2020  ool] = None,.   
+00007300: 2020 2020 2020 2020 2020 2020 2020 6373                cs
+00007310: 7461 7465 4172 6773 3a20 7479 7069 6e67  tateArgs: typing
+00007320: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
+00007330: 2e4d 6170 7069 6e67 5b73 7472 2c20 7479  .Mapping[str, ty
+00007340: 7069 6e67 2e41 6e79 5d5d 203d 204e 6f6e  ping.Any]] = Non
+00007350: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00007360: 2020 2020 2a2a 6b77 6172 6773 293a 0a20      **kwargs):. 
+00007370: 2020 2020 2020 2023 2043 7265 6174 6520         # Create 
+00007380: 7468 6520 6368 6563 6b62 6f78 2077 6964  the checkbox wid
+00007390: 6765 740a 2020 2020 2020 2020 6368 6f73  get.        chos
+000073a0: 656e 5f6c 6162 656c 203d 2073 656c 662e  en_label = self.
+000073b0: 6c61 6265 6c20 6f72 206c 6162 656c 0a20  label or label. 
+000073c0: 2020 2020 2020 2069 6620 6368 6f73 656e         if chosen
+000073d0: 5f6c 6162 656c 2069 7320 4e6f 6e65 3a0a  _label is None:.
+000073e0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+000073f0: 6520 5661 6c75 6545 7272 6f72 2827 7b73  e ValueError('{s
+00007400: 656c 6621 727d 3a20 4d69 7373 696e 6720  elf!r}: Missing 
+00007410: 7265 7175 6972 6564 206c 6162 656c 2729  required label')
+00007420: 0a20 2020 2020 2020 2063 7374 6174 6541  .        cstateA
+00007430: 7267 7320 3d20 6469 6374 2863 7374 6174  rgs = dict(cstat
+00007440: 6541 7267 7320 6f72 207b 7d29 0a20 2020  eArgs or {}).   
+00007450: 2020 2020 2063 7374 6174 6541 7267 732e       cstateArgs.
+00007460: 7570 6461 7465 287b 2020 2320 4f76 6572  update({  # Over
+00007470: 7269 6465 2063 7374 6174 6520 6172 6775  ride cstate argu
+00007480: 6d65 6e74 730a 2020 2020 2020 2020 2020  ments.          
+00007490: 2020 2776 6172 6961 626c 6527 3a20 6376    'variable': cv
+000074a0: 6172 6961 626c 652c 0a20 2020 2020 2020  ariable,.       
+000074b0: 2020 2020 2027 6c61 6265 6c27 3a20 6368       'label': ch
+000074c0: 6f73 656e 5f6c 6162 656c 2c0a 2020 2020  osen_label,.    
+000074d0: 2020 2020 2020 2020 2772 6561 646f 6e6c          'readonl
+000074e0: 7927 3a20 4661 6c73 652c 0a20 2020 2020  y': False,.     
+000074f0: 2020 207d 290a 2020 2020 2020 2020 6373     }).        cs
+00007500: 7461 7465 5f77 6964 6765 7420 3d20 7365  tate_widget = se
+00007510: 6c66 2e5f 5f63 6c61 7373 5f5f 2e5f 5f77  lf.__class__.__w
+00007520: 5f63 7374 6174 6528 7061 7265 6e74 2c20  _cstate(parent, 
+00007530: 2a2a 6373 7461 7465 4172 6773 290a 2020  **cstateArgs).  
+00007540: 2020 2020 2020 6173 7365 7274 2069 7369        assert isi
+00007550: 6e73 7461 6e63 6528 6373 7461 7465 5f77  nstance(cstate_w
+00007560: 6964 6765 742e 7661 7269 6162 6c65 2c20  idget.variable, 
+00007570: 7661 722e 426f 6f6c 6561 6e29 2c20 6627  var.Boolean), f'
+00007580: 7b73 656c 6621 727d 2063 6865 636b 626f  {self!r} checkbo
+00007590: 7820 7769 6467 6574 2069 7320 6e6f 7420  x widget is not 
+000075a0: 6120 7369 6d70 6c65 2062 6f6f 6c65 616e  a simple boolean
+000075b0: 270a 2020 2020 2020 2020 7365 6c66 2e63  '.        self.c
+000075c0: 7374 6174 6520 3d20 6373 7461 7465 5f77  state = cstate_w
+000075d0: 6964 6765 742e 7661 7269 6162 6c65 0a20  idget.variable. 
+000075e0: 2020 2020 2020 2023 2055 7375 616c 2049         # Usual I
+000075f0: 6e69 7469 616c 697a 6174 696f 6e0a 2020  nitialization.  
+00007600: 2020 2020 2020 7375 7065 7228 292e 5f5f        super().__
+00007610: 696e 6974 5f5f 2870 6172 656e 742c 206c  init__(parent, l
+00007620: 6162 656c 7769 6467 6574 3d63 7374 6174  abelwidget=cstat
+00007630: 655f 7769 6467 6574 2c20 6c61 6265 6c61  e_widget, labela
+00007640: 6e63 686f 723d 6c61 6265 6c41 6e63 686f  nchor=labelAncho
+00007650: 722e 7661 6c75 6529 0a20 2020 2020 2020  r.value).       
+00007660: 2073 656c 662e 696e 6974 5f63 6f6e 7461   self.init_conta
+00007670: 696e 6572 282a 6172 6773 2c20 2a2a 6b77  iner(*args, **kw
+00007680: 6172 6773 290a 2020 2020 2020 2020 2320  args).        # 
+00007690: 436f 6e66 6967 7572 6520 7468 6520 6368  Configure the ch
+000076a0: 6563 6b62 6f78 2077 6964 6765 740a 2020  eckbox widget.  
+000076b0: 2020 2020 2020 7365 6c66 2e63 7374 6174        self.cstat
+000076c0: 655f 7769 6467 6574 203d 2063 7374 6174  e_widget = cstat
+000076d0: 655f 7769 6467 6574 0a20 2020 2020 2020  e_widget.       
+000076e0: 2073 656c 662e 6373 7461 7465 5f77 6964   self.cstate_wid
+000076f0: 6765 742e 7472 6163 6528 7365 6c66 2e6f  get.trace(self.o
+00007700: 6e43 6861 6e67 6564 5f63 7374 6174 6529  nChanged_cstate)
+00007710: 0a20 2020 2020 2020 2023 2023 2053 6574  .        # # Set
+00007720: 7570 2074 6865 2064 6566 6175 6c74 2076  up the default v
+00007730: 616c 7565 2066 6f72 2074 6861 7420 7769  alue for that wi
+00007740: 6467 6574 0a20 2020 2020 2020 2069 6620  dget.        if 
+00007750: 5f5f 6465 6275 675f 5f3a 0a20 2020 2020  __debug__:.     
+00007760: 2020 2020 2020 2069 6620 6376 6172 6961         if cvaria
+00007770: 626c 6520 6973 206e 6f74 204e 6f6e 6520  ble is not None 
+00007780: 616e 6420 6376 6172 6961 626c 6544 6566  and cvariableDef
+00007790: 6175 6c74 2069 7320 6e6f 7420 4e6f 6e65  ault is not None
+000077a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000077b0: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
+000077c0: 6627 7b73 656c 667d 3a20 6376 6172 6961  f'{self}: cvaria
+000077d0: 626c 653a 2053 6574 7469 6e67 2061 2064  ble: Setting a d
+000077e0: 6566 6175 6c74 2077 6974 6820 616e 2065  efault with an e
+000077f0: 7874 6572 6e61 6c20 7661 7269 6162 6c65  xternal variable
+00007800: 2729 0a20 2020 2020 2020 2069 6620 6376  ').        if cv
+00007810: 6172 6961 626c 6520 6973 204e 6f6e 6520  ariable is None 
+00007820: 616e 6420 6376 6172 6961 626c 6544 6566  and cvariableDef
+00007830: 6175 6c74 2069 7320 4e6f 6e65 3a0a 2020  ault is None:.  
+00007840: 2020 2020 2020 2020 2020 6376 6172 6961            cvaria
+00007850: 626c 6544 6566 6175 6c74 203d 2054 7275  bleDefault = Tru
+00007860: 650a 2020 2020 2020 2020 6966 2063 7661  e.        if cva
+00007870: 7269 6162 6c65 4465 6661 756c 7420 6973  riableDefault is
+00007880: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00007890: 2020 2020 2020 2073 656c 662e 6373 7461         self.csta
+000078a0: 7465 2e73 6574 2863 7661 7269 6162 6c65  te.set(cvariable
+000078b0: 4465 6661 756c 7429 0a0a 2020 2020 6465  Default)..    de
+000078c0: 6620 7374 6174 655f 6765 7428 7365 6c66  f state_get(self
+000078d0: 2c20 2a61 7267 732c 2076 6964 5f75 7073  , *args, vid_ups
+000078e0: 7472 6561 6d3a 2074 7970 696e 672e 4f70  tream: typing.Op
+000078f0: 7469 6f6e 616c 5b74 7970 696e 672e 5365  tional[typing.Se
+00007900: 745b 7374 725d 5d20 3d20 4e6f 6e65 2c20  t[str]] = None, 
+00007910: 2a2a 6b77 6172 6773 2920 2d3e 206d 6f64  **kwargs) -> mod
+00007920: 656c 2e57 5374 6174 655b 626f 6f6c 2c20  el.WState[bool, 
+00007930: 7479 7069 6e67 2e41 6e79 5d3a 0a20 2020  typing.Any]:.   
+00007940: 2020 2020 2027 2727 2727 2720 2023 2044       ''''''  # D
+00007950: 6f20 6e6f 7420 646f 6375 6d65 6e74 0a20  o not document. 
+00007960: 2020 2020 2020 2063 6964 203d 2066 6e2e         cid = fn.
+00007970: 766e 616d 6528 7365 6c66 2e63 7374 6174  vname(self.cstat
+00007980: 6529 0a20 2020 2020 2020 2069 6620 7669  e).        if vi
+00007990: 645f 7570 7374 7265 616d 2061 6e64 2063  d_upstream and c
+000079a0: 6964 2069 6e20 7669 645f 7570 7374 7265  id in vid_upstre
+000079b0: 616d 3a0a 2020 2020 2020 2020 2020 2020  am:.            
+000079c0: 6373 7461 7465 203d 204e 6f6e 650a 2020  cstate = None.  
+000079d0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000079e0: 2020 2020 2020 2020 6373 7461 7465 203d          cstate =
+000079f0: 2073 656c 662e 6373 7461 7465 2e67 6574   self.cstate.get
+00007a00: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
+00007a10: 6e20 6d6f 6465 6c2e 5753 7461 7465 280a  n model.WState(.
+00007a20: 2020 2020 2020 2020 2020 2020 6373 7461              csta
+00007a30: 7465 2c0a 2020 2020 2020 2020 2020 2020  te,.            
+00007a40: 7375 7065 7228 292e 7374 6174 655f 6765  super().state_ge
+00007a50: 7428 2a61 7267 732c 2076 6964 5f75 7073  t(*args, vid_ups
+00007a60: 7472 6561 6d3d 7669 645f 7570 7374 7265  tream=vid_upstre
+00007a70: 616d 2c20 2a2a 6b77 6172 6773 292c 0a20  am, **kwargs),. 
+00007a80: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
+00007a90: 6620 7374 6174 655f 7365 7428 7365 6c66  f state_set(self
+00007aa0: 2c20 7374 6174 653a 206d 6f64 656c 2e57  , state: model.W
+00007ab0: 5374 6174 655b 626f 6f6c 2c20 7479 7069  State[bool, typi
+00007ac0: 6e67 2e41 6e79 5d2c 202a 6172 6773 2c20  ng.Any], *args, 
+00007ad0: 2a2a 6b77 6172 6773 293a 0a20 2020 2020  **kwargs):.     
+00007ae0: 2020 2027 2727 2727 2720 2023 2044 6f20     ''''''  # Do 
+00007af0: 6e6f 7420 646f 6375 6d65 6e74 0a20 2020  not document.   
+00007b00: 2020 2020 2069 6620 7374 6174 652e 7374       if state.st
+00007b10: 6174 6520 6973 206e 6f74 204e 6f6e 653a  ate is not None:
+00007b20: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
+00007b30: 6572 7420 6973 696e 7374 616e 6365 2873  ert isinstance(s
+00007b40: 7461 7465 2e73 7461 7465 2c20 626f 6f6c  tate.state, bool
+00007b50: 292c 2066 2749 6e76 616c 6964 2057 5374  ), f'Invalid WSt
+00007b60: 6174 653a 207b 7374 6174 6521 727d 270a  ate: {state!r}'.
+00007b70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007b80: 2e63 7374 6174 652e 7365 7428 7374 6174  .cstate.set(stat
+00007b90: 652e 7374 6174 6529 0a20 2020 2020 2020  e.state).       
+00007ba0: 2073 7570 6572 2829 2e73 7461 7465 5f73   super().state_s
+00007bb0: 6574 2873 7461 7465 2e73 7562 7374 6174  et(state.substat
+00007bc0: 652c 202a 6172 6773 2c20 2a2a 6b77 6172  e, *args, **kwar
+00007bd0: 6773 290a 0a20 2020 2064 6566 2073 6574  gs)..    def set
+00007be0: 5f67 7569 5f73 7461 7465 2873 656c 662c  _gui_state(self,
+00007bf0: 2073 7461 7465 3a20 7479 7069 6e67 2e4f   state: typing.O
+00007c00: 7074 696f 6e61 6c5b 6d6f 6465 6c2e 4775  ptional[model.Gu
+00007c10: 6953 7461 7465 5d20 3d20 4e6f 6e65 2c20  iState] = None, 
+00007c20: 2a2a 6b77 6172 6773 2920 2d3e 204e 6f6e  **kwargs) -> Non
+00007c30: 653a 0a20 2020 2020 2020 2023 2022 5472  e:.        # "Tr
+00007c40: 6163 6522 2074 6865 2066 7261 6d65 2065  ace" the frame e
+00007c50: 6e61 626c 6564 2073 7461 7475 730a 2020  nabled status.  
+00007c60: 2020 2020 2020 6672 616d 655f 656e 6162        frame_enab
+00007c70: 6c65 6420 3d20 6b77 6172 6773 2e67 6574  led = kwargs.get
+00007c80: 2827 656e 6162 6c65 6427 2c20 4e6f 6e65  ('enabled', None
+00007c90: 2920 6966 2073 7461 7465 2069 7320 4e6f  ) if state is No
+00007ca0: 6e65 2065 6c73 6520 7374 6174 652e 656e  ne else state.en
+00007cb0: 6162 6c65 640a 2020 2020 2020 2020 7375  abled.        su
+00007cc0: 7065 7228 292e 7365 745f 6775 695f 7374  per().set_gui_st
+00007cd0: 6174 6528 7374 6174 652c 202a 2a6b 7761  ate(state, **kwa
+00007ce0: 7267 7329 0a20 2020 2020 2020 2069 6620  rgs).        if 
+00007cf0: 6973 696e 7374 616e 6365 2866 7261 6d65  isinstance(frame
+00007d00: 5f65 6e61 626c 6564 2c20 626f 6f6c 293a  _enabled, bool):
+00007d10: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
+00007d20: 7465 5f65 6e61 626c 6564 203d 2073 656c  te_enabled = sel
+00007d30: 662e 6373 7461 7465 2e67 6574 2829 0a20  f.cstate.get(). 
+00007d40: 2020 2020 2020 2020 2020 2023 2069 6620             # if 
+00007d50: 5f5f 6465 6275 675f 5f3a 0a20 2020 2020  __debug__:.     
+00007d60: 2020 2020 2020 2023 2020 2020 206c 6f67         #     log
+00007d70: 6765 722e 6465 6275 6728 6627 537c 207b  ger.debug(f'S| {
+00007d80: 7365 6c66 7d3a 2046 3d7b 6672 616d 655f  self}: F={frame_
+00007d90: 656e 6162 6c65 647d 2053 3d7b 7374 6174  enabled} S={stat
+00007da0: 655f 656e 6162 6c65 647d 2729 0a20 2020  e_enabled}').   
+00007db0: 2020 2020 2020 2020 2073 656c 662e 6373           self.cs
+00007dc0: 7461 7465 5f77 6964 6765 742e 6773 7461  tate_widget.gsta
+00007dd0: 7465 203d 206d 6f64 656c 2e47 7569 5374  te = model.GuiSt
+00007de0: 6174 6528 656e 6162 6c65 643d 6672 616d  ate(enabled=fram
+00007df0: 655f 656e 6162 6c65 6429 0a20 2020 2020  e_enabled).     
+00007e00: 2020 2020 2020 2073 656c 662e 7365 745f         self.set_
+00007e10: 6775 695f 7375 6273 7461 7465 2865 6e61  gui_substate(ena
+00007e20: 626c 6564 3d66 7261 6d65 5f65 6e61 626c  bled=frame_enabl
+00007e30: 6564 2061 6e64 2073 7461 7465 5f65 6e61  ed and state_ena
+00007e40: 626c 6564 290a 2020 2020 2020 2020 2020  bled).          
+00007e50: 2020 2320 544f 444f 3a20 756e 7365 744f    # TODO: unsetO
+00007e60: 6e44 6973 6162 6c65 0a20 2020 2020 2020  nDisable.       
+00007e70: 2020 2020 2023 2054 4f44 4f3a 2073 6574       # TODO: set
+00007e80: 4f6e 456e 6162 6c65 0a0a 2020 2020 6465  OnEnable..    de
+00007e90: 6620 6f6e 4368 616e 6765 645f 6373 7461  f onChanged_csta
+00007ea0: 7465 2873 656c 662c 2063 7374 6174 652c  te(self, cstate,
+00007eb0: 2065 7479 7065 293a 0a20 2020 2020 2020   etype):.       
+00007ec0: 2061 7373 6572 7420 6574 7970 6520 3d3d   assert etype ==
+00007ed0: 2027 7772 6974 6527 0a20 2020 2020 2020   'write'.       
+00007ee0: 2073 7461 7475 7320 3d20 6373 7461 7465   status = cstate
+00007ef0: 2e67 6574 2829 0a20 2020 2020 2020 2066  .get().        f
+00007f00: 7261 6d65 5f65 6e61 626c 6564 203d 2073  rame_enabled = s
+00007f10: 656c 662e 6773 7461 7465 2e65 6e61 626c  elf.gstate.enabl
+00007f20: 6564 0a20 2020 2020 2020 2023 2069 6620  ed.        # if 
+00007f30: 5f5f 6465 6275 675f 5f3a 0a20 2020 2020  __debug__:.     
+00007f40: 2020 2023 2020 2020 206c 6f67 6765 722e     #     logger.
+00007f50: 6465 6275 6728 6627 7b73 656c 667d 3a20  debug(f'{self}: 
+00007f60: 533d 7b73 7461 7475 737d 2046 653d 7b66  S={status} Fe={f
+00007f70: 7261 6d65 5f65 6e61 626c 6564 7d27 290a  rame_enabled}').
+00007f80: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+00007f90: 5f67 7569 5f73 7562 7374 6174 6528 6d6f  _gui_substate(mo
+00007fa0: 6465 6c2e 4775 6953 7461 7465 2865 6e61  del.GuiState(ena
+00007fb0: 626c 6564 3d66 7261 6d65 5f65 6e61 626c  bled=frame_enabl
+00007fc0: 6564 2061 6e64 2073 7461 7475 7329 290a  ed and status)).
+00007fd0: 0a0a 2320 544f 444f 3a20 5573 6520 6074  ..# TODO: Use `t
+00007fe0: 6b2e 7363 726f 6c6c 6564 7465 7874 2e53  k.scrolledtext.S
+00007ff0: 6372 6f6c 6c65 6454 6578 7460 3f20 446f  crolledText`? Do
+00008000: 2074 6865 2073 616d 6520 7468 696e 6720   the same thing 
+00008010: 666f 7220 6d75 6c74 6970 6c65 2077 6964  for multiple wid
+00008020: 6765 7473 3f0a 636c 6173 7320 456e 7472  gets?.class Entr
+00008030: 794d 756c 7469 6c69 6e65 2874 6b2e 5465  yMultiline(tk.Te
+00008040: 7874 2c20 6d69 7869 6e2e 5369 6e67 6c65  xt, mixin.Single
+00008050: 5769 6467 6574 293a 0a20 2020 2027 2727  Widget):.    '''
+00008060: 4120 6d75 6c74 696c 696e 6520 7465 7874  A multiline text
+00008070: 2077 6964 6765 742c 2073 7570 706f 7274   widget, support
+00008080: 696e 6720 604c 544d 4c60 2063 6f6e 7465  ing `LTML` conte
+00008090: 6e74 732e 0a0a 2020 2020 5468 6973 2069  nts...    This i
+000080a0: 7320 6120 6d75 6c74 696c 696e 6520 7665  s a multiline ve
+000080b0: 7273 696f 6e20 6f66 2074 6865 2060 456e  rsion of the `En
+000080c0: 7472 7960 2077 6964 6765 742c 2077 6974  try` widget, wit
+000080d0: 6820 7269 6368 2074 6578 740a 2020 2020  h rich text.    
+000080e0: 6361 7061 6269 6c69 7469 6573 2e0a 2020  capabilities..  
+000080f0: 2020 5375 7070 6f72 7473 206f 6e6c 7920    Supports only 
+00008100: 7468 6520 7265 6164 6f6e 6c79 2073 7461  the readonly sta
+00008110: 7465 2c20 7468 6174 2069 732c 2074 6865  te, that is, the
+00008120: 2077 6964 6765 7420 636f 6e74 656e 7473   widget contents
+00008130: 2063 616e 206f 6e6c 7920 6265 0a20 2020   can only be.   
+00008140: 2065 6469 7465 6420 7072 6f67 7261 6d61   edited programa
+00008150: 7469 6361 6c6c 792e 0a0a 2020 2020 5468  tically...    Th
+00008160: 6520 7374 6174 6520 6973 2061 2073 696e  e state is a sin
+00008170: 676c 6520 6073 7472 6020 7661 6c75 652c  gle `str` value,
+00008180: 2069 6e74 6572 6e61 6c6c 7920 7061 7273   internally pars
+00008190: 6564 2074 6f20 6070 6172 7365 722e 4c54  ed to `parser.LT
+000081a0: 4d4c 0a20 2020 203c 4c54 4d4c 3e60 2e0a  ML.    <LTML>`..
+000081b0: 0a20 2020 2054 6865 7265 2069 7320 6e6f  .    There is no
+000081c0: 2050 7974 686f 6e20 646f 6375 6d65 6e74   Python document
+000081d0: 6174 696f 6e2c 2073 6565 2060 6054 6b60  ation, see ``Tk`
+000081e0: 6020 6074 6b2e 5465 7874 203c 6874 7470  ` `tk.Text <http
+000081f0: 733a 2f2f 7777 772e 7463 6c2e 746b 2f6d  s://www.tcl.tk/m
+00008200: 616e 2f74 636c 2f54 6b43 6d64 2f74 6578  an/tcl/TkCmd/tex
+00008210: 742e 6874 6d6c 3e60 5f20 646f 6375 6d65  t.html>`_ docume
+00008220: 6e74 6174 696f 6e2e 0a0a 2020 2020 4172  ntation...    Ar
+00008230: 6773 3a0a 2020 2020 2020 2020 7661 7269  gs:.        vari
+00008240: 6162 6c65 3a20 5573 6520 616e 2065 7874  able: Use an ext
+00008250: 6572 6e61 6c6c 7920 6465 6669 6e65 6420  ernally defined 
+00008260: 7661 7269 6162 6c65 2c20 696e 7374 6561  variable, instea
+00008270: 6420 6f66 2063 7265 6174 696e 6720 6120  d of creating a 
+00008280: 6e65 770a 2020 2020 2020 2020 2020 2020  new.            
+00008290: 6f6e 6520 7370 6563 6966 6963 2066 6f72  one specific for
+000082a0: 2074 6869 7320 7769 6467 6574 2e0a 2020   this widget..  
+000082b0: 2020 2020 2020 7374 796c 653a 2043 6f6e        style: Con
+000082c0: 6669 6775 7265 2074 6865 2077 6964 6765  figure the widge
+000082d0: 7420 7374 796c 652e 0a0a 2020 2020 2020  t style...      
+000082e0: 2020 7061 7265 6e74 3a20 5468 6520 7061    parent: The pa
+000082f0: 7265 6e74 2077 6964 6765 742e 2043 616e  rent widget. Can
+00008300: 2062 6520 6120 6052 6f6f 7457 696e 646f   be a `RootWindo
+00008310: 7760 206f 7220 616e 6f74 6865 7220 606d  w` or another `m
+00008320: 6978 696e 2e43 6f6e 7461 696e 6572 5769  ixin.ContainerWi
+00008330: 6467 6574 602e 0a0a 2020 2020 4e6f 7465  dget`...    Note
+00008340: 3a0a 0a20 2020 2020 2020 2054 6865 2075  :..        The u
+00008350: 6e64 6572 6c79 696e 6720 7769 6467 6574  nderlying widget
+00008360: 2069 7320 6e6f 7420 7061 7274 206f 6620   is not part of 
+00008370: 6074 746b 203c 746b 696e 7465 722e 7474  `ttk <tkinter.tt
+00008380: 6b3e 6020 6c69 6b65 206d 6f73 7420 6f74  k>` like most ot
+00008390: 6865 7273 2e20 416c 6c0a 2020 2020 2020  hers. All.      
+000083a0: 2020 6566 666f 7274 7320 6172 6520 6578    efforts are ex
+000083b0: 7065 6e64 6564 2074 6f20 6d61 6b65 2074  pended to make t
+000083c0: 6869 7320 616e 2069 6d70 6c65 6d65 6e74  his an implement
+000083d0: 6174 696f 6e20 6465 7461 696c 2c20 7769  ation detail, wi
+000083e0: 7468 6f75 740a 2020 2020 2020 2020 7072  thout.        pr
+000083f0: 6163 7469 6361 6c20 6566 6665 6374 732e  actical effects.
+00008400: 0a20 2020 2027 2727 0a20 2020 2073 7461  .    '''.    sta
+00008410: 7465 5f74 7970 6520 3d20 7661 722e 5374  te_type = var.St
+00008420: 7269 6e67 0a20 2020 205f 6269 6e64 696e  ring.    _bindin
+00008430: 6773 5f74 6167 3a20 7479 7069 6e67 2e4d  gs_tag: typing.M
+00008440: 7574 6162 6c65 4d61 7070 696e 675b 7479  utableMapping[ty
+00008450: 7069 6e67 2e54 7570 6c65 5b73 7472 2c20  ping.Tuple[str, 
+00008460: 7374 725d 2c20 6d6f 6465 6c2e 4269 6e64  str], model.Bind
+00008470: 696e 6754 6167 5d0a 2020 2020 2727 2753  ingTag].    '''S
+00008480: 746f 7265 2061 6c6c 2077 6964 6765 7420  tore all widget 
+00008490: 6042 696e 6469 6e67 5461 6760 206f 626a  `BindingTag` obj
+000084a0: 6563 7473 2c20 6b65 7965 6420 6279 2060  ects, keyed by `
+000084b0: 6028 7461 672c 206e 616d 6529 6060 2028  `(tag, name)`` (
+000084c0: 7365 6520 6062 696e 6469 6e67 5f74 6167  see `binding_tag
+000084d0: 6029 2e27 2727 0a0a 2020 2020 4064 6174  `).'''..    @dat
+000084e0: 6163 6c61 7373 0a20 2020 2063 6c61 7373  aclass.    class
+000084f0: 2053 7479 6c65 286d 6f64 656c 2e57 5374   Style(model.WSt
+00008500: 796c 6529 3a0a 2020 2020 2020 2020 2727  yle):.        ''
+00008510: 2760 456e 7472 794d 756c 7469 6c69 6e65  '`EntryMultiline
+00008520: 6020 7374 796c 6520 6f62 6a65 6374 2e0a  ` style object..
+00008530: 0a20 2020 2020 2020 2054 6865 7365 2061  .        These a
+00008540: 7265 2074 6865 2073 6574 7469 6e67 733a  re the settings:
+00008550: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+00008560: 2020 2020 2020 2020 2020 2020 666f 6e74              font
+00008570: 5f62 6173 653a 2042 6173 6520 466f 6e74  _base: Base Font
+00008580: 206e 616d 652c 2066 6f72 2061 6c6c 2074   name, for all t
+00008590: 6865 2077 6964 6765 742e 0a20 2020 2020  he widget..     
+000085a0: 2020 2020 2020 2063 6f6c 6f75 725f 6267         colour_bg
+000085b0: 5f6f 6e3a 2057 6964 6765 7420 6261 636b  _on: Widget back
+000085c0: 6772 6f75 6e64 2c20 7768 656e 2065 6e61  ground, when ena
+000085d0: 626c 6564 2e0a 2020 2020 2020 2020 2020  bled..          
+000085e0: 2020 636f 6c6f 7572 5f62 675f 6f66 663a    colour_bg_off:
+000085f0: 2057 6964 6765 7420 6261 636b 6772 6f75   Widget backgrou
+00008600: 6e64 2c20 7768 656e 2064 6973 6162 6c65  nd, when disable
+00008610: 642e 0a20 2020 2020 2020 2020 2020 2063  d..            c
+00008620: 6f6c 6f75 725f 6c69 6e6b 5f6e 6f72 6d61  olour_link_norma
+00008630: 6c3a 2048 7970 6572 6c69 6e6b 2066 6f72  l: Hyperlink for
+00008640: 6567 726f 756e 6420 636f 6c6f 7572 2c20  eground colour, 
+00008650: 6e6f 726d 616c 206c 696e 6b73 2e0a 2020  normal links..  
+00008660: 2020 2020 2020 2020 2020 636f 6c6f 7572            colour
+00008670: 5f6c 696e 6b5f 7669 7369 7465 643a 2048  _link_visited: H
+00008680: 7970 6572 6c69 6e6b 2066 6f72 6567 726f  yperlink foregro
+00008690: 756e 6420 636f 6c6f 7572 2c20 7669 7369  und colour, visi
+000086a0: 7465 6420 6c69 6e6b 732e 0a20 2020 2020  ted links..     
+000086b0: 2020 2027 2727 0a20 2020 2020 2020 2066     '''.        f
+000086c0: 6f6e 745f 6261 7365 3a20 7374 7220 3d20  ont_base: str = 
+000086d0: 2754 6b54 6578 7446 6f6e 7427 2020 2320  'TkTextFont'  # 
+000086e0: 5468 6973 2066 6f6e 7420 7368 6f75 6c64  This font should
+000086f0: 2062 6520 7573 6564 2066 6f72 2075 7365   be used for use
+00008700: 7220 7465 7874 2069 6e20 656e 7472 7920  r text in entry 
+00008710: 7769 6467 6574 732c 206c 6973 7462 6f78  widgets, listbox
+00008720: 6573 2065 7463 2e0a 2020 2020 2020 2020  es etc..        
+00008730: 636f 6c6f 7572 5f62 675f 6f6e 3a20 7374  colour_bg_on: st
+00008740: 7220 3d20 2777 6869 7465 270a 2020 2020  r = 'white'.    
+00008750: 2020 2020 636f 6c6f 7572 5f62 675f 6f66      colour_bg_of
+00008760: 663a 2073 7472 203d 2027 6c69 6768 7467  f: str = 'lightg
+00008770: 7265 7927 0a20 2020 2020 2020 2063 6f6c  rey'.        col
+00008780: 6f75 725f 6c69 6e6b 5f6e 6f72 6d61 6c3a  our_link_normal:
+00008790: 2073 7472 203d 2027 626c 7565 270a 2020   str = 'blue'.  
+000087a0: 2020 2020 2020 636f 6c6f 7572 5f6c 696e        colour_lin
+000087b0: 6b5f 7669 7369 7465 643a 2073 7472 203d  k_visited: str =
+000087c0: 2027 7075 7270 6c65 270a 0a20 2020 2064   'purple'..    d
+000087d0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+000087e0: 2c20 7061 7265 6e74 2c20 2a2c 2076 6172  , parent, *, var
+000087f0: 6961 626c 653a 2076 6172 2e53 7472 696e  iable: var.Strin
+00008800: 6720 3d20 4e6f 6e65 2c0a 2020 2020 2020  g = None,.      
+00008810: 2020 2020 2020 2020 2020 2073 7479 6c65             style
+00008820: 3a20 5374 796c 6520 3d20 5374 796c 6528  : Style = Style(
+00008830: 5f64 6566 6175 6c74 3d54 7275 6529 2c0a  _default=True),.
+00008840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008850: 202a 2a6b 7761 7267 7329 3a0a 2020 2020   **kwargs):.    
+00008860: 2020 2020 7365 6c66 2e77 7374 796c 6520      self.wstyle 
+00008870: 3d20 7374 796c 650a 2020 2020 2020 2020  = style.        
+00008880: 7365 6c66 2e69 6e69 745f 7369 6e67 6c65  self.init_single
+00008890: 2876 6172 6961 626c 6529 0a20 2020 2020  (variable).     
+000088a0: 2020 206b 7761 7267 732e 706f 7028 2773     kwargs.pop('s
+000088b0: 7461 7465 272c 204e 6f6e 6529 2020 2320  tate', None)  # 
+000088c0: 5375 7070 6f72 7420 6f6e 6c79 2072 6561  Support only rea
+000088d0: 646f 6e6c 7920 7374 6174 650a 2020 2020  donly state.    
+000088e0: 2020 2020 6b77 6172 6773 5b27 666f 6e74      kwargs['font
+000088f0: 275d 203d 2073 7479 6c65 2e66 6f6e 745f  '] = style.font_
+00008900: 6261 7365 2020 2320 4f76 6572 7269 6465  base  # Override
+00008910: 2074 6865 2062 6173 6520 666f 6e74 0a20   the base font. 
+00008920: 2020 2020 2020 2073 7570 6572 2829 2e5f         super()._
+00008930: 5f69 6e69 745f 5f28 7061 7265 6e74 2c20  _init__(parent, 
+00008940: 2a2a 6b77 6172 6773 2920 2023 2074 6b2e  **kwargs)  # tk.
+00008950: 456e 7472 790a 2020 2020 2020 2020 7265  Entry.        re
+00008960: 6164 6f6e 6c79 203d 2054 7275 6520 2023  adonly = True  #
+00008970: 2053 7570 706f 7274 206f 6e6c 7920 7265   Support only re
+00008980: 6164 6f6e 6c79 2073 7461 7465 2c20 666f  adonly state, fo
+00008990: 7220 6e6f 772e 2e2e 0a20 2020 2020 2020  r now....       
+000089a0: 2023 2047 5549 2053 7461 7465 2054 7261   # GUI State Tra
+000089b0: 636b 6572 0a20 2020 2020 2020 2023 202d  cker.        # -
+000089c0: 2053 696e 6365 2074 6869 7320 6973 206e   Since this is n
+000089d0: 6f74 2061 2060 7474 6b2e 5769 6467 6574  ot a `ttk.Widget
+000089e0: 602c 2074 6869 7320 6e65 6564 2074 6f20  `, this need to 
+000089f0: 6265 2065 6d75 6c61 7465 640a 2020 2020  be emulated.    
+00008a00: 2020 2020 7365 6c66 2e5f 5f67 7374 6174      self.__gstat
+00008a10: 653a 206d 6f64 656c 2e47 7569 5374 6174  e: model.GuiStat
+00008a20: 6520 3d20 6d6f 6465 6c2e 4775 6953 7461  e = model.GuiSta
+00008a30: 7465 2865 6e61 626c 6564 3d54 7275 652c  te(enabled=True,
+00008a40: 2072 6561 646f 6e6c 793d 7265 6164 6f6e   readonly=readon
+00008a50: 6c79 290a 2020 2020 2020 2020 2320 2d20  ly).        # - 
+00008a60: 5365 7420 7468 6520 696e 7465 726e 616c  Set the internal
+00008a70: 2072 6561 646f 6e6c 7920 7374 6174 6520   readonly state 
+00008a80: 6f75 742d 6f66 2d74 6865 2d62 6f78 0a20  out-of-the-box. 
+00008a90: 2020 2020 2020 2073 656c 662e 7365 745f         self.set_
+00008aa0: 6775 695f 7374 6174 6528 7265 6164 6f6e  gui_state(readon
+00008ab0: 6c79 3d72 6561 646f 6e6c 792c 205f 696e  ly=readonly, _in
+00008ac0: 7465 726e 616c 3d54 7275 6529 0a20 2020  ternal=True).   
+00008ad0: 2020 2020 2061 7373 6572 7420 7365 6c66       assert self
+00008ae0: 2e76 6172 6961 626c 6520 6973 206e 6f74  .variable is not
+00008af0: 204e 6f6e 652c 2066 277b 7365 6c66 2172   None, f'{self!r
+00008b00: 7d3a 204d 6973 7369 6e67 2076 6172 6961  }: Missing varia
+00008b10: 626c 6527 0a20 2020 2020 2020 2073 656c  ble'.        sel
+00008b20: 662e 7773 7461 7465 203d 2067 6574 6174  f.wstate = getat
+00008b30: 7472 2873 656c 662e 7661 7269 6162 6c65  tr(self.variable
+00008b40: 2c20 275f 6465 6661 756c 7427 2c20 2727  , '_default', ''
+00008b50: 2920 2023 2053 6574 2074 6865 2064 6566  )  # Set the def
+00008b60: 6175 6c74 2028 6265 666f 7265 2074 6865  ault (before the
+00008b70: 2074 7261 6365 290a 2020 2020 2020 2020   trace).        
+00008b80: 2320 5374 6174 6520 5472 6163 6b65 720a  # State Tracker.
+00008b90: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
+00008ba0: 6365 2873 656c 662e 5f76 6172 4368 616e  ce(self._varChan
+00008bb0: 6765 642c 2074 7261 6365 5f6e 616d 653d  ged, trace_name=
+00008bc0: 6627 5f5f 3a7b 5f5f 6e61 6d65 5f5f 7d27  f'__:{__name__}'
+00008bd0: 290a 0a20 2020 2020 2020 2023 2042 696e  )..        # Bin
+00008be0: 6469 6e67 730a 2020 2020 2020 2020 7365  dings.        se
+00008bf0: 6c66 2e5f 6269 6e64 696e 6773 5f74 6167  lf._bindings_tag
+00008c00: 203d 207b 7d0a 2020 2020 2020 2020 2320   = {}.        # 
+00008c10: 544f 444f 3a20 496e 7665 7374 6967 6174  TODO: Investigat
+00008c20: 6520 6368 616e 6769 6e67 2074 6865 2063  e changing the c
+00008c30: 7572 736f 7220 6f6e 206d 6f75 7365 6f76  ursor on mouseov
+00008c40: 6572 0a20 2020 2020 2020 2073 656c 662e  er.        self.
+00008c50: 6269 6e64 696e 675f 7461 6728 2761 272c  binding_tag('a',
+00008c60: 2027 3c42 7574 746f 6e2d 313e 272c 2073   '<Button-1>', s
+00008c70: 656c 662e 5f6f 6e43 6c69 636b 5461 6729  elf._onClickTag)
+00008c80: 0a20 2020 2020 2020 2069 6620 7265 6164  .        if read
+00008c90: 6f6e 6c79 3a0a 2020 2020 2020 2020 2020  only:.          
+00008ca0: 2020 2320 4469 7361 626c 6520 446f 7562    # Disable Doub
+00008cb0: 6c65 2d43 6c69 636b 2065 7665 6e74 2c20  le-Click event, 
+00008cc0: 7768 656e 2072 6561 646f 6e6c 790a 2020  when readonly.  
+00008cd0: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+00008ce0: 696e 6469 6e67 2827 3c44 6f75 626c 652d  inding('<Double-
+00008cf0: 4275 7474 6f6e 2d31 3e27 2c20 666e 2e62  Button-1>', fn.b
+00008d00: 696e 6469 6e67 5f64 6973 6162 6c65 290a  inding_disable).
+00008d10: 0a20 2020 2064 6566 205f 7661 7243 6861  .    def _varCha
+00008d20: 6e67 6564 2873 656c 662c 2076 6172 2c20  nged(self, var, 
+00008d30: 6574 7970 6529 3a0a 2020 2020 2020 2020  etype):.        
+00008d40: 6173 7365 7274 2065 7479 7065 203d 3d20  assert etype == 
+00008d50: 2777 7269 7465 270a 2020 2020 2020 2020  'write'.        
+00008d60: 2320 5468 6973 2066 756e 6374 696f 6e20  # This function 
+00008d70: 6973 2063 616c 6c65 6420 7768 656e 2074  is called when t
+00008d80: 6865 2076 616c 7565 2063 6861 6e67 6573  he value changes
+00008d90: 0a20 2020 2020 2020 2023 2049 7427 7320  .        # It's 
+00008da0: 7468 6520 696d 706c 656d 656e 7461 7469  the implementati
+00008db0: 6f6e 2074 6861 7420 6269 6e64 7320 7468  on that binds th
+00008dc0: 6520 7661 7269 6162 6c65 2061 6e64 2074  e variable and t
+00008dd0: 6865 2077 6964 6765 742c 0a20 2020 2020  he widget,.     
+00008de0: 2020 2023 2020 736f 2074 6869 7320 7368     #  so this sh
+00008df0: 6f75 6c64 2062 6520 6964 656d 706f 7465  ould be idempote
+00008e00: 6e74 0a20 2020 2020 2020 2076 7320 3d20  nt.        vs = 
+00008e10: 7661 722e 6765 7428 290a 2020 2020 2020  var.get().      
+00008e20: 2020 7769 7468 2073 656c 662e 6173 5f65    with self.as_e
+00008e30: 6469 7461 626c 6528 293a 0a20 2020 2020  ditable():.     
+00008e40: 2020 2020 2020 2023 2044 656c 6574 6520         # Delete 
+00008e50: 7468 6520 656e 7469 7265 2073 7461 7465  the entire state
+00008e60: 0a20 2020 2020 2020 2020 2020 2023 2046  .            # F
+00008e70: 726f 6d3a 2046 6972 7374 206c 696e 652c  rom: First line,
+00008e80: 2066 6972 7374 2063 6861 7261 6374 6572   first character
+00008e90: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
+00008ea0: 2054 6f3a 2045 6e64 0a20 2020 2020 2020   To: End.       
+00008eb0: 2020 2020 2073 656c 662e 6465 6c65 7465       self.delete
+00008ec0: 2827 312e 3027 2c20 2765 6e64 2729 0a20  ('1.0', 'end'). 
+00008ed0: 2020 2020 2020 2020 2020 2023 2052 6573             # Res
+00008ee0: 6574 2073 7479 6c65 730a 2020 2020 2020  et styles.      
+00008ef0: 2020 2020 2020 7365 6c66 2e73 7479 6c65        self.style
+00008f00: 5f72 6573 6574 2829 0a20 2020 2020 2020  _reset().       
+00008f10: 2020 2020 2023 2041 6464 2074 6865 2063       # Add the c
+00008f20: 7572 7265 6e74 2073 7461 7465 0a20 2020  urrent state.   
+00008f30: 2020 2020 2020 2020 2023 2054 4f44 4f3a           # TODO:
+00008f40: 2053 6176 6520 7468 6520 7061 7273 6564   Save the parsed
+00008f50: 204c 544d 4c20 7374 6174 6520 736f 6d65   LTML state some
+00008f60: 7768 6572 6520 696e 2074 6869 7320 6f62  where in this ob
+00008f70: 6a65 6374 2c20 7769 7468 2060 6461 7461  ject, with `data
+00008f80: 603f 0a20 2020 2020 2020 2020 2020 2066  `?.            f
+00008f90: 6f72 2074 6520 696e 2070 6172 7365 722e  or te in parser.
+00008fa0: 7061 7273 655f 4c54 4d4c 2876 7329 3a0a  parse_LTML(vs):.
+00008fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008fc0: 6173 7365 7274 2069 7369 6e73 7461 6e63  assert isinstanc
+00008fd0: 6528 7465 2c20 6d6f 6465 6c2e 5465 7874  e(te, model.Text
+00008fe0: 456c 656d 656e 7429 0a20 2020 2020 2020  Element).       
+00008ff0: 2020 2020 2020 2020 2073 656c 662e 696e           self.in
+00009000: 7365 7274 2874 6b2e 454e 442c 2074 652e  sert(tk.END, te.
+00009010: 7465 7874 2c20 7465 2e61 7461 6773 290a  text, te.atags).
+00009020: 0a20 2020 2064 6566 2067 6574 5f67 7569  .    def get_gui
+00009030: 5f73 7461 7465 2873 656c 6629 202d 3e20  _state(self) -> 
+00009040: 6d6f 6465 6c2e 4775 6953 7461 7465 3a0a  model.GuiState:.
+00009050: 2020 2020 2020 2020 2727 2727 2727 2020          ''''''  
+00009060: 2320 446f 206e 6f74 2064 6f63 756d 656e  # Do not documen
+00009070: 740a 2020 2020 2020 2020 6966 205f 5f64  t.        if __d
+00009080: 6562 7567 5f5f 3a0a 2020 2020 2020 2020  ebug__:.        
+00009090: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+000090a0: 2827 5374 6174 6520 3e20 2572 272c 2073  ('State > %r', s
+000090b0: 656c 662e 5f5f 6773 7461 7465 290a 2020  elf.__gstate).  
+000090c0: 2020 2020 2020 2320 7265 7475 726e 2061        # return a
+000090d0: 2063 6f70 7920 6f66 2074 6865 206f 626a   copy of the obj
+000090e0: 6563 740a 2020 2020 2020 2020 7265 7475  ect.        retu
+000090f0: 726e 206d 6f64 656c 2e47 7569 5374 6174  rn model.GuiStat
+00009100: 6528 2a2a 6469 6374 2873 656c 662e 5f5f  e(**dict(self.__
+00009110: 6773 7461 7465 2e69 7465 6d73 2829 2929  gstate.items()))
+00009120: 0a0a 2020 2020 6465 6620 7365 745f 6775  ..    def set_gu
+00009130: 695f 7374 6174 6528 7365 6c66 2c20 7374  i_state(self, st
+00009140: 6174 653a 2074 7970 696e 672e 4f70 7469  ate: typing.Opti
+00009150: 6f6e 616c 5b6d 6f64 656c 2e47 7569 5374  onal[model.GuiSt
+00009160: 6174 655d 203d 204e 6f6e 652c 202a 2c20  ate] = None, *, 
+00009170: 5f69 6e74 6572 6e61 6c3a 2062 6f6f 6c20  _internal: bool 
+00009180: 3d20 4661 6c73 652c 202a 2a6b 7761 7267  = False, **kwarg
+00009190: 7329 202d 3e20 4e6f 6e65 3a0a 2020 2020  s) -> None:.    
+000091a0: 2020 2020 2727 2727 2727 2020 2320 446f      ''''''  # Do
+000091b0: 206e 6f74 2064 6f63 756d 656e 740a 2020   not document.  
+000091c0: 2020 2020 2020 6966 2073 7461 7465 2069        if state i
+000091d0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+000091e0: 2020 2020 7374 6174 6520 3d20 6d6f 6465      state = mode
+000091f0: 6c2e 4775 6953 7461 7465 282a 2a6b 7761  l.GuiState(**kwa
+00009200: 7267 7329 0a20 2020 2020 2020 2069 6620  rgs).        if 
+00009210: 5f5f 6465 6275 675f 5f3a 0a20 2020 2020  __debug__:.     
+00009220: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+00009230: 6275 6728 2753 7461 7465 203c 2025 7227  bug('State < %r'
+00009240: 2c20 7374 6174 6529 0a20 2020 2020 2020  , state).       
+00009250: 2023 2041 646a 7573 7420 6375 7272 656e   # Adjust curren
+00009260: 7420 7374 6174 650a 2020 2020 2020 2020  t state.        
+00009270: 666f 7220 736e 616d 652c 2073 7661 6c75  for sname, svalu
+00009280: 6520 696e 2073 7461 7465 2e69 7465 6d73  e in state.items
+00009290: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+000092a0: 6173 7365 7274 2073 6e61 6d65 2021 3d20  assert sname != 
+000092b0: 275f 696e 7465 726e 616c 2720 2023 2053  '_internal'  # S
+000092c0: 686f 756c 6420 6265 2069 6d70 6f73 7369  hould be impossi
+000092d0: 626c 652e 2e2e 0a20 2020 2020 2020 2020  ble....         
+000092e0: 2020 2069 6620 7376 616c 7565 2069 7320     if svalue is 
+000092f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00009300: 2020 2020 2020 2020 2020 6966 2073 6e61            if sna
+00009310: 6d65 203d 3d20 2772 6561 646f 6e6c 7927  me == 'readonly'
+00009320: 2061 6e64 205f 696e 7465 726e 616c 2069   and _internal i
+00009330: 7320 4661 6c73 653a 0a20 2020 2020 2020  s False:.       
+00009340: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+00009350: 7365 2056 616c 7565 4572 726f 7228 6627  se ValueError(f'
+00009360: 7b73 656c 667d 3a20 4e6f 2073 7570 706f  {self}: No suppo
+00009370: 7274 2066 6f72 2065 7874 6572 6e61 6c20  rt for external 
+00009380: 7265 6164 6f6e 6c79 2073 7461 7465 206d  readonly state m
+00009390: 616e 6970 756c 6174 696f 6e27 290a 2020  anipulation').  
+000093a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000093b0: 7461 7474 7228 7365 6c66 2e5f 5f67 7374  tattr(self.__gst
+000093c0: 6174 652c 2073 6e61 6d65 2c20 7376 616c  ate, sname, sval
+000093d0: 7565 290a 2020 2020 2020 2020 2320 4164  ue).        # Ad
+000093e0: 6a75 7374 2077 6964 6765 7420 7374 6174  just widget stat
+000093f0: 650a 2020 2020 2020 2020 6366 6720 3d20  e.        cfg = 
+00009400: 7b7d 0a20 2020 2020 2020 2069 6620 7365  {}.        if se
+00009410: 6c66 2e5f 5f67 7374 6174 652e 656e 6162  lf.__gstate.enab
+00009420: 6c65 6420 6973 2054 7275 653a 0a20 2020  led is True:.   
+00009430: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00009440: 2e5f 5f67 7374 6174 652e 7265 6164 6f6e  .__gstate.readon
+00009450: 6c79 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ly is not None:.
+00009460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009470: 6366 675b 2773 7461 7465 275d 203d 2074  cfg['state'] = t
+00009480: 6b2e 4e4f 524d 414c 2069 6620 6e6f 7420  k.NORMAL if not 
+00009490: 7365 6c66 2e5f 5f67 7374 6174 652e 7265  self.__gstate.re
+000094a0: 6164 6f6e 6c79 2065 6c73 6520 746b 2e44  adonly else tk.D
+000094b0: 4953 4142 4c45 440a 2020 2020 2020 2020  ISABLED.        
+000094c0: 2020 2020 6366 675b 2762 6163 6b67 726f      cfg['backgro
+000094d0: 756e 6427 5d20 3d20 7365 6c66 2e77 7374  und'] = self.wst
+000094e0: 796c 652e 636f 6c6f 7572 5f62 675f 6f6e  yle.colour_bg_on
+000094f0: 0a20 2020 2020 2020 2065 6c69 6620 7365  .        elif se
+00009500: 6c66 2e5f 5f67 7374 6174 652e 656e 6162  lf.__gstate.enab
+00009510: 6c65 6420 6973 2046 616c 7365 3a0a 2020  led is False:.  
+00009520: 2020 2020 2020 2020 2020 6366 675b 2773            cfg['s
+00009530: 7461 7465 275d 203d 2074 6b2e 4449 5341  tate'] = tk.DISA
+00009540: 424c 4544 0a20 2020 2020 2020 2020 2020  BLED.           
+00009550: 2063 6667 5b27 6261 636b 6772 6f75 6e64   cfg['background
+00009560: 275d 203d 2073 656c 662e 7773 7479 6c65  '] = self.wstyle
+00009570: 2e63 6f6c 6f75 725f 6267 5f6f 6666 0a20  .colour_bg_off. 
+00009580: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00009590: 7374 796c 655f 7265 7365 7428 290a 2020  style_reset().  
+000095a0: 2020 2020 2020 2320 6966 205f 5f64 6562        # if __deb
+000095b0: 7567 5f5f 3a0a 2020 2020 2020 2020 2320  ug__:.        # 
+000095c0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+000095d0: 2827 4320 2573 272c 2073 656c 662e 5f5f  ('C %s', self.__
+000095e0: 6773 7461 7465 290a 2020 2020 2020 2020  gstate).        
+000095f0: 2320 2020 2020 6c6f 6767 6572 2e64 6562  #     logger.deb
+00009600: 7567 2827 7c20 2573 272c 2063 6667 290a  ug('| %s', cfg).
+00009610: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00009620: 6669 6775 7265 282a 2a63 6667 290a 2020  figure(**cfg).  
+00009630: 2020 2020 2020 2320 5661 6c69 643a 2054        # Valid: T
+00009640: 4244 0a0a 2020 2020 4063 6f6e 7465 7874  BD..    @context
+00009650: 6d61 6e61 6765 720a 2020 2020 6465 6620  manager.    def 
+00009660: 6173 5f65 6469 7461 626c 6528 7365 6c66  as_editable(self
+00009670: 293a 0a20 2020 2020 2020 2027 2727 5465  ):.        '''Te
+00009680: 6d70 6f72 6172 696c 7920 6d61 726b 2074  mporarily mark t
+00009690: 6865 2077 6964 6765 7420 6173 2065 6469  he widget as edi
+000096a0: 7461 626c 652e 0a0a 2020 2020 2020 2020  table...        
+000096b0: 4120 636f 6e74 6578 7420 6d61 6e61 6765  A context manage
+000096c0: 722c 2075 7365 6420 746f 2063 6861 6e67  r, used to chang
+000096d0: 6520 7468 6520 636f 6e74 656e 7473 206f  e the contents o
+000096e0: 6620 7468 6520 7769 6467 6574 2077 6869  f the widget whi
+000096f0: 6c65 206b 6565 700a 2020 2020 2020 2020  le keep.        
+00009700: 6974 2022 7265 6164 6f6e 6c79 222e 0a20  it "readonly".. 
+00009710: 2020 2020 2020 2054 6563 686e 6963 616c         Technical
+00009720: 6c79 2c20 7468 6973 2073 686f 756c 6420  ly, this should 
+00009730: 6f6e 6c79 2062 6520 7573 6564 2069 6e74  only be used int
+00009740: 6572 6e61 6c6c 792c 2075 7369 6e67 2074  ernally, using t
+00009750: 6865 2073 7461 7465 0a20 2020 2020 2020  he state.       
+00009760: 2074 7261 636b 6572 2066 756e 6374 696f   tracker functio
+00009770: 6e73 2c20 6275 7420 6974 206d 6967 6874  ns, but it might
+00009780: 2062 6520 7573 6566 756c 2065 7874 6572   be useful exter
+00009790: 6e61 6c6c 792e 0a0a 2020 2020 2020 2020  nally...        
+000097a0: 5468 6973 2069 7320 746f 2062 6520 7573  This is to be us
+000097b0: 6564 206c 696b 6520 7468 6973 3a0a 0a20  ed like this:.. 
+000097c0: 2020 2020 2020 202e 2e20 636f 6465 3a3a         .. code::
+000097d0: 2070 7974 686f 6e0a 0a20 2020 2020 2020   python..       
+000097e0: 2020 2020 2023 2060 7769 6467 6574 6020       # `widget` 
+000097f0: 6973 2072 6561 646f 6e6c 790a 2020 2020  is readonly.    
+00009800: 2020 2020 2020 2020 7769 7468 2077 6964          with wid
+00009810: 6765 742e 6173 5f65 6469 7461 626c 6528  get.as_editable(
+00009820: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00009830: 2020 2070 6173 7320 2023 2060 7769 6467     pass  # `widg
+00009840: 6574 6020 6973 2065 6469 7461 626c 650a  et` is editable.
+00009850: 2020 2020 2020 2020 2020 2020 2320 6077              # `w
+00009860: 6964 6765 7460 2069 7320 7265 6164 6f6e  idget` is readon
+00009870: 6c79 0a20 2020 2020 2020 2027 2727 0a20  ly.        '''. 
+00009880: 2020 2020 2020 2061 7373 6572 7420 7365         assert se
+00009890: 6c66 2e5f 5f67 7374 6174 652e 7265 6164  lf.__gstate.read
+000098a0: 6f6e 6c79 2069 7320 5472 7565 0a20 2020  only is True.   
+000098b0: 2020 2020 2073 656c 662e 7365 745f 6775       self.set_gu
+000098c0: 695f 7374 6174 6528 7265 6164 6f6e 6c79  i_state(readonly
+000098d0: 3d46 616c 7365 2c20 5f69 6e74 6572 6e61  =False, _interna
+000098e0: 6c3d 5472 7565 290a 2020 2020 2020 2020  l=True).        
+000098f0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00009900: 2079 6965 6c64 0a20 2020 2020 2020 2066   yield.        f
+00009910: 696e 616c 6c79 3a0a 2020 2020 2020 2020  inally:.        
+00009920: 2020 2020 7365 6c66 2e73 6574 5f67 7569      self.set_gui
+00009930: 5f73 7461 7465 2872 6561 646f 6e6c 793d  _state(readonly=
+00009940: 5472 7565 2c20 5f69 6e74 6572 6e61 6c3d  True, _internal=
+00009950: 5472 7565 290a 0a20 2020 2064 6566 2062  True)..    def b
+00009960: 696e 6469 6e67 5f74 6167 2873 656c 662c  inding_tag(self,
+00009970: 2074 6167 3a20 7374 722c 2073 6571 7565   tag: str, seque
+00009980: 6e63 653a 2073 7472 2c20 2a61 7267 732c  nce: str, *args,
+00009990: 206b 6579 3a20 7374 7220 3d20 4e6f 6e65   key: str = None
+000099a0: 2c20 696d 6d65 6469 6174 653a 2062 6f6f  , immediate: boo
+000099b0: 6c20 3d20 5472 7565 2c20 2a2a 6b77 6172  l = True, **kwar
+000099c0: 6773 2920 2d3e 206d 6f64 656c 2e42 696e  gs) -> model.Bin
+000099d0: 6469 6e67 5461 673a 0a20 2020 2020 2020  dingTag:.       
+000099e0: 2027 2727 4269 6e64 7320 6120 7365 7175   '''Binds a sequ
+000099f0: 656e 6365 2074 6f20 6120 7461 672e 0a0a  ence to a tag...
+00009a00: 2020 2020 2020 2020 5374 6f72 6573 2061          Stores a
+00009a10: 6c6c 2077 6964 6765 7420 7461 6720 6269  ll widget tag bi
+00009a20: 6e64 696e 6773 206f 6e20 6120 7065 722d  ndings on a per-
+00009a30: 696e 7374 616e 6365 2064 6963 7469 6f6e  instance diction
+00009a40: 6172 792c 2066 6f72 206c 6174 6572 0a20  ary, for later. 
+00009a50: 2020 2020 2020 2075 7361 6765 2e20 4e6f         usage. No
+00009a60: 7465 2074 6861 7420 616c 6c20 6469 6374  te that all dict
+00009a70: 696f 6e61 7279 206b 6579 7320 6d75 7374  ionary keys must
+00009a80: 2062 6520 6469 6666 6572 656e 742e 2046   be different. F
+00009a90: 6f72 2074 6865 2073 616d 650a 2020 2020  or the same.    
+00009aa0: 2020 2020 6269 6e64 696e 6773 206f 6e20      bindings on 
+00009ab0: 6120 7369 6e67 6c65 2077 6964 6765 7420  a single widget 
+00009ac0: 7461 672c 2074 6869 7320 7265 7175 6972  tag, this requir
+00009ad0: 6573 2070 6173 7369 6e67 2074 6865 2060  es passing the `
+00009ae0: 606b 6579 6060 0a20 2020 2020 2020 2061  `key``.        a
+00009af0: 7267 756d 656e 742e 0a0a 2020 2020 2020  rgument...      
+00009b00: 2020 5365 6520 7468 6520 6060 546b 6060    See the ``Tk``
+00009b10: 2060 7461 6720 6269 6e64 203c 6874 7470   `tag bind <http
+00009b20: 733a 2f2f 7777 772e 7463 6c2e 746b 2f6d  s://www.tcl.tk/m
+00009b30: 616e 2f74 636c 2f54 6b43 6d64 2f74 6578  an/tcl/TkCmd/tex
+00009b40: 742e 6874 6d6c 234d 3136 363e 605f 2064  t.html#M166>`_ d
+00009b50: 6f63 756d 656e 7461 7469 6f6e 2e0a 0a20  ocumentation... 
+00009b60: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+00009b70: 2020 2020 2020 2020 206b 6579 3a20 4f70           key: Op
+00009b80: 7469 6f6e 616c 2e20 4465 6661 756c 7473  tional. Defaults
+00009b90: 2074 6f20 7468 6520 6060 7365 7175 656e   to the ``sequen
+00009ba0: 6365 6060 2069 7473 656c 662e 2055 7365  ce`` itself. Use
+00009bb0: 6675 6c20 746f 0a20 2020 2020 2020 2020  ful to.         
+00009bc0: 2020 2020 2020 2073 7570 706f 7274 206d         support m
+00009bd0: 756c 7469 706c 6520 6269 6e64 696e 6773  ultiple bindings
+00009be0: 206f 6e20 7468 6520 7361 6d65 2073 6571   on the same seq
+00009bf0: 7565 6e63 652c 2066 6f72 2074 6865 2073  uence, for the s
+00009c00: 616d 6520 7461 672e 0a0a 2020 2020 2020  ame tag...      
+00009c10: 2020 416c 6c20 6f74 6865 7220 6172 6775    All other argu
+00009c20: 6d65 6e74 7320 6172 6520 7061 7373 6564  ments are passed
+00009c30: 2074 6f20 606d 6f64 656c 2e42 696e 6469   to `model.Bindi
+00009c40: 6e67 5461 6760 206f 626a 6563 742e 0a20  ngTag` object.. 
+00009c50: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00009c60: 2020 206e 616d 6520 3d20 2874 6167 2c20     name = (tag, 
+00009c70: 6b65 7920 6f72 2073 6571 7565 6e63 6529  key or sequence)
+00009c80: 0a20 2020 2020 2020 2069 6620 6e61 6d65  .        if name
+00009c90: 2069 6e20 7365 6c66 2e5f 6269 6e64 696e   in self._bindin
+00009ca0: 6773 5f74 6167 3a0a 2020 2020 2020 2020  gs_tag:.        
+00009cb0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00009cc0: 7272 6f72 2866 2752 6570 6561 7465 6420  rror(f'Repeated 
+00009cd0: 6269 6e64 696e 6720 666f 7220 227b 7365  binding for "{se
+00009ce0: 7175 656e 6365 7d22 2069 6e20 7b73 656c  quence}" in {sel
+00009cf0: 6621 727d 2874 6167 2022 7b74 6167 7d22  f!r}(tag "{tag}"
+00009d00: 292e 2043 6861 6e67 6520 7468 6520 226b  ). Change the "k
+00009d10: 6579 2220 7061 7261 6d65 7465 722e 2729  ey" parameter.')
+00009d20: 0a20 2020 2020 2020 2069 6620 5f5f 6465  .        if __de
+00009d30: 6275 675f 5f3a 0a20 2020 2020 2020 2020  bug__:.         
+00009d40: 2020 2069 6620 6c65 6e28 7461 6729 203d     if len(tag) =
+00009d50: 3d20 3020 6f72 2074 6167 5b30 5d20 3d3d  = 0 or tag[0] ==
+00009d60: 2027 3c27 3a0a 2020 2020 2020 2020 2020   '<':.          
+00009d70: 2020 2020 2020 7761 726e 696e 6773 2e77        warnings.w
+00009d80: 6172 6e28 6627 7b73 656c 667d 3a20 6269  arn(f'{self}: bi
+00009d90: 6e64 696e 675f 7461 6720 7265 7175 6972  nding_tag requir
+00009da0: 6573 2074 6167 5b7b 7461 677d 5d20 616e  es tag[{tag}] an
+00009db0: 6420 7365 7175 656e 6365 5b7b 7365 7175  d sequence[{sequ
+00009dc0: 656e 6365 7d5d 2c20 6279 2074 6869 7320  ence}], by this 
+00009dd0: 6f72 6465 7227 2c20 7374 6163 6b6c 6576  order', stacklev
+00009de0: 656c 3d32 290a 2020 2020 2020 2020 7365  el=2).        se
+00009df0: 6c66 2e5f 6269 6e64 696e 6773 5f74 6167  lf._bindings_tag
+00009e00: 5b6e 616d 655d 203d 206d 6f64 656c 2e42  [name] = model.B
+00009e10: 696e 6469 6e67 5461 6728 7365 6c66 2c20  indingTag(self, 
+00009e20: 7461 672c 2073 6571 7565 6e63 652c 202a  tag, sequence, *
+00009e30: 6172 6773 2c20 696d 6d65 6469 6174 653d  args, immediate=
+00009e40: 696d 6d65 6469 6174 652c 202a 2a6b 7761  immediate, **kwa
+00009e50: 7267 7329 0a20 2020 2020 2020 2072 6574  rgs).        ret
+00009e60: 7572 6e20 7365 6c66 2e5f 6269 6e64 696e  urn self._bindin
+00009e70: 6773 5f74 6167 5b6e 616d 655d 0a0a 2020  gs_tag[name]..  
+00009e80: 2020 2320 544f 444f 3a20 7573 6520 616e    # TODO: use an
+00009e90: 2060 6c72 755f 6361 6368 6560 3f0a 2020   `lru_cache`?.  
+00009ea0: 2020 6465 6620 5f66 6f6e 7428 7365 6c66    def _font(self
+00009eb0: 2c20 666f 6e74 6261 7365 3a20 7479 7069  , fontbase: typi
+00009ec0: 6e67 2e4f 7074 696f 6e61 6c5b 746b 2e66  ng.Optional[tk.f
+00009ed0: 6f6e 742e 466f 6e74 5d20 3d20 4e6f 6e65  ont.Font] = None
+00009ee0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00009ef0: 2a2c 0a20 2020 2020 2020 2020 2020 2020  *,.             
+00009f00: 2073 697a 653a 2074 7970 696e 672e 4f70   size: typing.Op
+00009f10: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+00009f20: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00009f30: 2020 626f 6c64 3a20 7479 7069 6e67 2e4f    bold: typing.O
+00009f40: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
+00009f50: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+00009f60: 2020 2020 6974 616c 6963 3a20 7479 7069      italic: typi
+00009f70: 6e67 2e4f 7074 696f 6e61 6c5b 626f 6f6c  ng.Optional[bool
+00009f80: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00009f90: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
+00009fa0: 2020 2066 6f6e 7462 6173 6520 3d20 666f     fontbase = fo
+00009fb0: 6e74 6261 7365 206f 7220 746b 2e66 6f6e  ntbase or tk.fon
+00009fc0: 742e 6e61 6d65 746f 666f 6e74 2873 656c  t.nametofont(sel
+00009fd0: 662e 7773 7479 6c65 2e66 6f6e 745f 6261  f.wstyle.font_ba
+00009fe0: 7365 290a 2020 2020 2020 2020 2320 5374  se).        # St
+00009ff0: 6172 7420 6672 6f6d 2074 6865 2062 6173  art from the bas
+0000a000: 6520 666f 6e74 206f 7074 696f 6e73 0a20  e font options. 
+0000a010: 2020 2020 2020 206f 7074 696f 6e73 203d         options =
+0000a020: 2066 6f6e 7462 6173 652e 6163 7475 616c   fontbase.actual
+0000a030: 2829 0a20 2020 2020 2020 2069 6620 7369  ().        if si
+0000a040: 7a65 3a0a 2020 2020 2020 2020 2020 2020  ze:.            
+0000a050: 6f70 7469 6f6e 735b 2773 697a 6527 5d20  options['size'] 
+0000a060: 3d20 7369 7a65 0a20 2020 2020 2020 2069  = size.        i
+0000a070: 6620 626f 6c64 2069 7320 5472 7565 3a0a  f bold is True:.
+0000a080: 2020 2020 2020 2020 2020 2020 6f70 7469              opti
+0000a090: 6f6e 735b 2777 6569 6768 7427 5d20 3d20  ons['weight'] = 
+0000a0a0: 746b 2e66 6f6e 742e 424f 4c44 0a20 2020  tk.font.BOLD.   
+0000a0b0: 2020 2020 2069 6620 6974 616c 6963 2069       if italic i
+0000a0c0: 7320 5472 7565 3a0a 2020 2020 2020 2020  s True:.        
+0000a0d0: 2020 2020 6f70 7469 6f6e 735b 2773 6c61      options['sla
+0000a0e0: 6e74 275d 203d 2074 6b2e 666f 6e74 2e49  nt'] = tk.font.I
+0000a0f0: 5441 4c49 430a 2020 2020 2020 2020 7265  TALIC.        re
+0000a100: 7475 726e 2074 6b2e 666f 6e74 2e46 6f6e  turn tk.font.Fon
+0000a110: 7428 2a2a 6f70 7469 6f6e 7329 0a0a 2020  t(**options)..  
+0000a120: 2020 6465 6620 5f73 7479 6c65 5f61 2873    def _style_a(s
+0000a130: 656c 662c 2074 6167 3a20 7374 7220 3d20  elf, tag: str = 
+0000a140: 2761 272c 202a 2c20 7669 7369 7465 643a  'a', *, visited:
+0000a150: 2062 6f6f 6c29 202d 3e20 4e6f 6e65 3a0a   bool) -> None:.
+0000a160: 2020 2020 2020 2020 6667 203d 2073 656c          fg = sel
+0000a170: 662e 7773 7479 6c65 2e63 6f6c 6f75 725f  f.wstyle.colour_
+0000a180: 6c69 6e6b 5f76 6973 6974 6564 2069 6620  link_visited if 
+0000a190: 7669 7369 7465 6420 656c 7365 2073 656c  visited else sel
+0000a1a0: 662e 7773 7479 6c65 2e63 6f6c 6f75 725f  f.wstyle.colour_
+0000a1b0: 6c69 6e6b 5f6e 6f72 6d61 6c0a 2020 2020  link_normal.    
+0000a1c0: 2020 2020 7365 6c66 2e74 6167 5f63 6f6e      self.tag_con
+0000a1d0: 6669 6775 7265 2874 6167 2c20 666f 7265  figure(tag, fore
+0000a1e0: 6772 6f75 6e64 3d66 672c 2075 6e64 6572  ground=fg, under
+0000a1f0: 6c69 6e65 3d54 7275 6529 0a0a 2020 2020  line=True)..    
+0000a200: 6465 6620 7374 796c 655f 7265 7365 7428  def style_reset(
+0000a210: 7365 6c66 2c20 6576 656e 743d 4e6f 6e65  self, event=None
+0000a220: 2c20 2a2c 2061 3a20 626f 6f6c 203d 2054  , *, a: bool = T
+0000a230: 7275 652c 2062 3a20 626f 6f6c 203d 2054  rue, b: bool = T
+0000a240: 7275 652c 2069 3a20 626f 6f6c 203d 2054  rue, i: bool = T
+0000a250: 7275 6529 202d 3e20 4e6f 6e65 3a0a 2020  rue) -> None:.  
+0000a260: 2020 2020 2020 2727 2752 6573 6574 2074        '''Reset t
+0000a270: 6865 2073 7479 6c65 2074 6f20 7468 6520  he style to the 
+0000a280: 6f72 6967 696e 616c 2e0a 0a20 2020 2020  original...     
+0000a290: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+0000a2a0: 2020 2020 2061 3a20 5265 7365 7420 6060       a: Reset ``
+0000a2b0: 6160 6020 616e 6368 6f72 732e 0a20 2020  a`` anchors..   
+0000a2c0: 2020 2020 2020 2020 2062 3a20 5265 7365           b: Rese
+0000a2d0: 7420 6060 6260 6020 626f 6c64 2069 6e6c  t ``b`` bold inl
+0000a2e0: 696e 6520 7370 616e 732e 0a20 2020 2020  ine spans..     
+0000a2f0: 2020 2020 2020 2069 3a20 5265 7365 7420         i: Reset 
+0000a300: 6060 6960 6020 6974 616c 6963 2069 6e6c  ``i`` italic inl
+0000a310: 696e 6520 7370 616e 732e 0a0a 2020 2020  ine spans...    
+0000a320: 2020 2020 2020 2020 6576 656e 743a 204f          event: O
+0000a330: 7074 696f 6e61 6c2c 2075 6e75 7365 642e  ptional, unused.
+0000a340: 2054 6869 7320 6578 6973 7473 2066 6f72   This exists for
+0000a350: 2041 5049 2063 6f6d 7061 7469 6269 6c69   API compatibili
+0000a360: 7479 2077 6974 6820 7468 650a 2020 2020  ty with the.    
+0000a370: 2020 2020 2020 2020 2020 2020 6060 6f6e              ``on
+0000a380: 436c 6963 6b60 6020 6675 6e63 7469 6f6e  Click`` function
+0000a390: 732e 0a20 2020 2020 2020 2027 2727 0a20  s..        '''. 
+0000a3a0: 2020 2020 2020 2023 2054 4f44 4f3a 2057         # TODO: W
+0000a3b0: 6879 206e 6f74 2072 6573 6574 2065 7665  hy not reset eve
+0000a3c0: 7279 7468 696e 6720 616c 7761 7973 3f20  rything always? 
+0000a3d0: 5941 474e 492e 0a20 2020 2020 2020 2069  YAGNI..        i
+0000a3e0: 6620 623a 0a20 2020 2020 2020 2020 2020  f b:.           
+0000a3f0: 2073 656c 662e 7461 675f 636f 6e66 6967   self.tag_config
+0000a400: 7572 6528 2762 272c 2066 6f6e 743d 7365  ure('b', font=se
+0000a410: 6c66 2e5f 666f 6e74 2862 6f6c 643d 5472  lf._font(bold=Tr
+0000a420: 7565 2929 0a20 2020 2020 2020 2069 6620  ue)).        if 
+0000a430: 693a 0a20 2020 2020 2020 2020 2020 2073  i:.            s
+0000a440: 656c 662e 7461 675f 636f 6e66 6967 7572  elf.tag_configur
+0000a450: 6528 2769 272c 2066 6f6e 743d 7365 6c66  e('i', font=self
+0000a460: 2e5f 666f 6e74 2869 7461 6c69 633d 5472  ._font(italic=Tr
+0000a470: 7565 2929 0a20 2020 2020 2020 2066 6f72  ue)).        for
+0000a480: 2074 6167 2069 6e20 7365 6c66 2e74 6167   tag in self.tag
+0000a490: 5f6e 616d 6573 2829 3a0a 2020 2020 2020  _names():.      
+0000a4a0: 2020 2020 2020 2320 610a 2020 2020 2020        # a.      
+0000a4b0: 2020 2020 2020 6966 2061 2061 6e64 2074        if a and t
+0000a4c0: 6167 203d 3d20 2761 2720 6f72 2074 6167  ag == 'a' or tag
+0000a4d0: 2e73 7461 7274 7377 6974 6828 2761 3a3a  .startswith('a::
+0000a4e0: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
+0000a4f0: 2020 2020 7365 6c66 2e5f 7374 796c 655f      self._style_
+0000a500: 6128 7461 673d 7461 672c 2076 6973 6974  a(tag=tag, visit
+0000a510: 6564 3d46 616c 7365 290a 0a20 2020 2064  ed=False)..    d
+0000a520: 6566 205f 6f6e 436c 6963 6b54 6167 2873  ef _onClickTag(s
+0000a530: 656c 662c 2065 7665 6e74 2c20 2a2c 2074  elf, event, *, t
+0000a540: 6167 5f6e 616d 653a 2073 7472 203d 2027  ag_name: str = '
+0000a550: 6127 293a 0a20 2020 2020 2020 2069 6620  a'):.        if 
+0000a560: 6e6f 7420 7365 6c66 2e5f 5f67 7374 6174  not self.__gstat
+0000a570: 652e 656e 6162 6c65 643a 0a20 2020 2020  e.enabled:.     
+0000a580: 2020 2020 2020 2072 6574 7572 6e20 2023         return  #
+0000a590: 2044 6f20 6e6f 7468 696e 6720 7768 656e   Do nothing when
+0000a5a0: 2064 6973 6162 6c65 640a 2020 2020 2020   disabled.      
+0000a5b0: 2020 646f 626a 203d 2073 656c 662e 6475    dobj = self.du
+0000a5c0: 6d70 2866 2740 7b65 7665 6e74 2e78 7d2c  mp(f'@{event.x},
+0000a5d0: 7b65 7665 6e74 2e79 7d27 2c20 7465 7874  {event.y}', text
+0000a5e0: 3d54 7275 652c 2074 6167 3d54 7275 6529  =True, tag=True)
+0000a5f0: 0a20 2020 2020 2020 2069 6620 5f5f 6465  .        if __de
+0000a600: 6275 675f 5f3a 0a20 2020 2020 2020 2020  bug__:.         
+0000a610: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+0000a620: 2744 3a20 2572 272c 2064 6f62 6a29 0a20  'D: %r', dobj). 
+0000a630: 2020 2020 2020 2064 7768 6174 203d 205b         dwhat = [
+0000a640: 6469 6e6e 6572 5b30 5d20 666f 7220 6469  dinner[0] for di
+0000a650: 6e6e 6572 2069 6e20 646f 626a 5d0a 2020  nner in dobj].  
+0000a660: 2020 2020 2020 7461 6773 5f63 6c20 3d20        tags_cl = 
+0000a670: 5b5d 2020 2320 4967 6e6f 7265 2074 6865  []  # Ignore the
+0000a680: 2022 7365 6c22 2074 6167 0a20 2020 2020   "sel" tag.     
+0000a690: 2020 2069 6620 2774 6167 6f6e 2720 696e     if 'tagon' in
+0000a6a0: 2064 7768 6174 3a0a 2020 2020 2020 2020   dwhat:.        
+0000a6b0: 2020 2020 2320 436c 6963 6b20 696e 2074      # Click in t
+0000a6c0: 6865 2073 7461 7274 206f 6620 7468 6520  he start of the 
+0000a6d0: 7461 670a 2020 2020 2020 2020 2020 2020  tag.            
+0000a6e0: 7461 6773 5f63 6c20 3d20 5b6c 7374 5b31  tags_cl = [lst[1
+0000a6f0: 5d20 666f 7220 6c73 7420 696e 2064 6f62  ] for lst in dob
+0000a700: 6a20 6966 206c 7374 5b30 5d20 3d3d 2027  j if lst[0] == '
+0000a710: 7461 676f 6e27 2061 6e64 206c 7374 5b31  tagon' and lst[1
+0000a720: 5d20 213d 2074 6b2e 5345 4c5d 0a20 2020  ] != tk.SEL].   
+0000a730: 2020 2020 2020 2020 2023 2046 6f72 206e           # For n
+0000a740: 6573 7465 6420 7461 6773 2c20 7468 6973  ested tags, this
+0000a750: 206d 6967 6874 206e 6f74 2062 6520 7468   might not be th
+0000a760: 6520 7361 6d65 2061 7320 7468 6520 7465  e same as the te
+0000a770: 7874 206d 6574 686f 640a 2020 2020 2020  xt method.      
+0000a780: 2020 6966 206c 656e 2874 6167 735f 636c    if len(tags_cl
+0000a790: 2920 3d3d 2030 2061 6e64 2027 7465 7874  ) == 0 and 'text
+0000a7a0: 2720 696e 2064 7768 6174 3a0a 2020 2020  ' in dwhat:.    
+0000a7b0: 2020 2020 2020 2020 2320 436c 6963 6b20          # Click 
+0000a7c0: 696e 2074 6865 206d 6964 646c 6520 6f66  in the middle of
+0000a7d0: 2074 6865 2074 6167 0a20 2020 2020 2020   the tag.       
+0000a7e0: 2020 2020 2063 6c69 636b 5f6c 6f63 6174       click_locat
+0000a7f0: 696f 6e20 3d20 5b6c 7374 5b32 5d20 666f  ion = [lst[2] fo
+0000a800: 7220 6c73 7420 696e 2064 6f62 6a20 6966  r lst in dobj if
+0000a810: 206c 7374 5b30 5d20 3d3d 2027 7465 7874   lst[0] == 'text
+0000a820: 275d 5b30 5d0a 2020 2020 2020 2020 2020  '][0].          
+0000a830: 2020 7470 203d 2073 656c 662e 7461 675f    tp = self.tag_
+0000a840: 7072 6576 7261 6e67 6528 7461 675f 6e61  prevrange(tag_na
+0000a850: 6d65 2c20 636c 6963 6b5f 6c6f 6361 7469  me, click_locati
+0000a860: 6f6e 290a 2020 2020 2020 2020 2020 2020  on).            
+0000a870: 6966 205f 5f64 6562 7567 5f5f 3a0a 2020  if __debug__:.  
+0000a880: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+0000a890: 6767 6572 2e64 6562 7567 2827 207c 2054  gger.debug(' | T
+0000a8a0: 6578 7420 4020 3c25 7327 2c20 7470 290a  ext @ <%s', tp).
+0000a8b0: 2020 2020 2020 2020 2020 2020 7461 6773              tags
+0000a8c0: 5f63 6c20 3d20 5b6c 7374 5b31 5d20 666f  _cl = [lst[1] fo
+0000a8d0: 7220 6c73 7420 696e 2073 656c 662e 6475  r lst in self.du
+0000a8e0: 6d70 282a 7470 2c20 7461 673d 5472 7565  mp(*tp, tag=True
+0000a8f0: 2920 6966 206c 7374 5b31 5d20 213d 2074  ) if lst[1] != t
+0000a900: 6b2e 5345 4c5d 0a20 2020 2020 2020 2069  k.SEL].        i
+0000a910: 6620 6c65 6e28 7461 6773 5f63 6c29 203d  f len(tags_cl) =
+0000a920: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+0000a930: 2072 6169 7365 204e 6f74 496d 706c 656d   raise NotImplem
+0000a940: 656e 7465 6445 7272 6f72 0a20 2020 2020  entedError.     
+0000a950: 2020 2069 6620 5f5f 6465 6275 675f 5f3a     if __debug__:
+0000a960: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+0000a970: 6765 722e 6465 6275 6728 2720 7c20 5461  ger.debug(' | Ta
+0000a980: 6773 2025 7327 2c20 7461 6773 5f63 6c29  gs %s', tags_cl)
+0000a990: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+0000a9a0: 6c65 6e28 7461 6773 5f63 6c29 203e 3d20  len(tags_cl) >= 
+0000a9b0: 322c 2066 274d 6973 7369 6e67 2074 6167  2, f'Missing tag
+0000a9c0: 733a 207b 7461 6773 5f63 6c7d 270a 2020  s: {tags_cl}'.  
+0000a9d0: 2020 2020 2020 7461 6773 5f70 726f 6320        tags_proc 
+0000a9e0: 3d20 5b74 2066 6f72 2074 2069 6e20 7461  = [t for t in ta
+0000a9f0: 6773 5f63 6c20 6966 2027 3a3a 2720 696e  gs_cl if '::' in
+0000aa00: 2074 5d0a 2020 2020 2020 2020 6173 7365   t].        asse
+0000aa10: 7274 206c 656e 2874 6167 735f 7072 6f63  rt len(tags_proc
+0000aa20: 2920 3d3d 2031 0a20 2020 2020 2020 2074  ) == 1.        t
+0000aa30: 6167 6920 3d20 7461 6773 5f70 726f 635b  agi = tags_proc[
+0000aa40: 305d 0a20 2020 2020 2020 2074 6167 203d  0].        tag =
+0000aa50: 2074 6167 692e 7370 6c69 7428 273a 3a27   tagi.split('::'
+0000aa60: 295b 305d 0a20 2020 2020 2020 2061 7373  )[0].        ass
+0000aa70: 6572 7420 7461 675f 6e61 6d65 203d 3d20  ert tag_name == 
+0000aa80: 7461 672c 2066 2757 726f 6e67 206f 6e43  tag, f'Wrong onC
+0000aa90: 6c69 636b 5461 673a 2052 6571 7565 7374  lickTag: Request
+0000aaa0: 6564 5b7b 7461 675f 6e61 6d65 7d5d 2021  ed[{tag_name}] !
+0000aab0: 3d20 466f 756e 645b 7b74 6167 7d5d 270a  = Found[{tag}]'.
+0000aac0: 2020 2020 2020 2020 6173 7365 7274 2074          assert t
+0000aad0: 6167 2069 6e20 7461 6773 5f63 6c2c 2066  ag in tags_cl, f
+0000aae0: 2757 726f 6e67 2074 6167 5f69 6e64 6578  'Wrong tag_index
+0000aaf0: 3a20 7b74 6167 7d5b 7b74 6167 697d 5d27  : {tag}[{tagi}]'
+0000ab00: 0a20 2020 2020 2020 2074 6167 735f 6f74  .        tags_ot
+0000ab10: 6865 7220 3d20 5b74 2066 6f72 2074 2069  her = [t for t i
+0000ab20: 6e20 7461 6773 5f63 6c20 6966 2074 206e  n tags_cl if t n
+0000ab30: 6f74 2069 6e20 2874 6167 2c20 7461 6769  ot in (tag, tagi
+0000ab40: 295d 0a20 2020 2020 2020 2069 6620 5f5f  )].        if __
+0000ab50: 6465 6275 675f 5f3a 0a20 2020 2020 2020  debug__:.       
+0000ab60: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+0000ab70: 6728 6627 203d 207b 7461 677d 5b7b 7461  g(f' = {tag}[{ta
+0000ab80: 6769 7d5d 2729 0a20 2020 2020 2020 2073  gi}]').        s
+0000ab90: 656c 662e 5f73 7479 6c65 5f61 2874 6167  elf._style_a(tag
+0000aba0: 3d74 6167 692c 2076 6973 6974 6564 3d54  =tagi, visited=T
+0000abb0: 7275 6529 0a20 2020 2020 2020 2073 656c  rue).        sel
+0000abc0: 662e 6f6e 436c 6963 6b54 6167 2874 6167  f.onClickTag(tag
+0000abd0: 2c20 7461 6769 2c20 7461 6773 5f6f 7468  , tagi, tags_oth
+0000abe0: 6572 290a 0a20 2020 2064 6566 206f 6e43  er)..    def onC
+0000abf0: 6c69 636b 5461 6728 7365 6c66 2c20 7461  lickTag(self, ta
+0000ac00: 673a 2073 7472 2c20 7461 675f 696e 6465  g: str, tag_inde
+0000ac10: 783a 2073 7472 2c20 7461 6773 5f6f 7468  x: str, tags_oth
+0000ac20: 6572 3a20 7479 7069 6e67 2e53 6571 7565  er: typing.Seque
+0000ac30: 6e63 655b 7374 725d 2920 2d3e 204e 6f6e  nce[str]) -> Non
+0000ac40: 653a 0a20 2020 2020 2020 2027 2727 4361  e:.        '''Ca
+0000ac50: 6c6c 6261 636b 2074 6f20 6265 2063 616c  llback to be cal
+0000ac60: 6c65 6420 7768 656e 2063 6c69 636b 696e  led when clickin
+0000ac70: 6720 6060 6160 6020 7461 6773 2069 6e20  g ``a`` tags in 
+0000ac80: 7468 6973 2077 6964 6765 742e 0a0a 2020  this widget...  
+0000ac90: 2020 2020 2020 4465 6661 756c 7473 2074        Defaults t
+0000aca0: 6f20 646f 696e 6720 6e6f 7468 696e 672e  o doing nothing.
+0000acb0: 0a0a 2020 2020 2020 2020 4176 6169 6c61  ..        Availa
+0000acc0: 626c 6520 666f 7220 7375 6263 6c61 7373  ble for subclass
+0000acd0: 2072 6564 6566 696e 6974 696f 6e2e 0a0a   redefinition...
+0000ace0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+0000acf0: 2020 2020 2020 2020 2020 7461 673a 2054            tag: T
+0000ad00: 6865 206d 6169 6e20 7461 6720 7479 7065  he main tag type
+0000ad10: 2e20 496e 2074 6869 7320 6361 7365 2c20  . In this case, 
+0000ad20: 6974 2773 2061 6c77 6179 7320 6060 6160  it's always ``a`
+0000ad30: 602e 0a20 2020 2020 2020 2020 2020 2074  `..            t
+0000ad40: 6167 5f69 6e64 6578 3a20 5468 6520 7461  ag_index: The ta
+0000ad50: 6720 696e 6465 782e 2053 6565 2060 4c54  g index. See `LT
+0000ad60: 4d4c 203c 7061 7273 6572 2e4c 544d 4c3e  ML <parser.LTML>
+0000ad70: 6020 4175 746f 6d61 7469 6320 436f 756e  ` Automatic Coun
+0000ad80: 7465 7220 7461 6773 2e0a 2020 2020 2020  ter tags..      
+0000ad90: 2020 2020 2020 7461 6773 5f6f 7468 6572        tags_other
+0000ada0: 3a20 4c69 7374 206f 6620 6578 7472 6120  : List of extra 
+0000adb0: 7461 6773 2061 7474 6163 6865 6420 746f  tags attached to
+0000adc0: 2074 6865 2061 6e63 686f 722e 204d 6967   the anchor. Mig
+0000add0: 6874 2062 6520 656d 7074 792e 0a20 2020  ht be empty..   
+0000ade0: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+0000adf0: 2070 6173 730a 0a20 2020 2064 6566 2077   pass..    def w
+0000ae00: 7374 6174 654c 544d 4c28 7365 6c66 2920  stateLTML(self) 
+0000ae10: 2d3e 2074 7970 696e 672e 4765 6e65 7261  -> typing.Genera
+0000ae20: 746f 725b 6d6f 6465 6c2e 5465 7874 456c  tor[model.TextEl
+0000ae30: 656d 656e 742c 204e 6f6e 652c 204e 6f6e  ement, None, Non
+0000ae40: 655d 3a0a 2020 2020 2020 2020 2727 2752  e]:.        '''R
+0000ae50: 6574 7572 6e20 7468 6520 7061 7273 6564  eturn the parsed
+0000ae60: 204c 544d 4c20 7374 6174 652c 2061 7320   LTML state, as 
+0000ae70: 6120 6765 6e65 7261 746f 7220 6f66 2060  a generator of `
+0000ae80: 6d6f 6465 6c2e 5465 7874 456c 656d 656e  model.TextElemen
+0000ae90: 7460 2e0a 0a20 2020 2020 2020 2053 6565  t`...        See
+0000aea0: 2041 6c73 6f3a 0a20 2020 2020 2020 2020   Also:.         
+0000aeb0: 2020 202d 2060 7773 7461 7465 603a 2052     - `wstate`: R
+0000aec0: 6574 7572 6e20 7468 6520 4c54 4d4c 2073  eturn the LTML s
+0000aed0: 7472 696e 672e 0a20 2020 2020 2020 2020  tring..         
+0000aee0: 2020 202d 2060 7773 7461 7465 5465 7874     - `wstateText
+0000aef0: 603a 2052 6574 7572 6e20 7468 6520 756e  `: Return the un
+0000af00: 6465 726c 7969 6e67 2074 6578 742c 2077  derlying text, w
+0000af10: 6974 686f 7574 2061 6e79 2074 6167 732e  ithout any tags.
+0000af20: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+0000af30: 2020 2020 2023 2054 4f44 4f3a 2053 6176       # TODO: Sav
+0000af40: 6520 7468 6520 7061 7273 6564 204c 544d  e the parsed LTM
+0000af50: 4c20 7374 6174 6520 736f 6d65 7768 6572  L state somewher
+0000af60: 6520 696e 2074 6869 7320 6f62 6a65 6374  e in this object
+0000af70: 2c20 7769 7468 2060 6461 7461 603f 0a20  , with `data`?. 
+0000af80: 2020 2020 2020 2079 6965 6c64 2066 726f         yield fro
+0000af90: 6d20 7061 7273 6572 2e70 6172 7365 5f4c  m parser.parse_L
+0000afa0: 544d 4c28 7365 6c66 2e77 7374 6174 6529  TML(self.wstate)
+0000afb0: 0a0a 2020 2020 6465 6620 7773 7461 7465  ..    def wstate
+0000afc0: 5465 7874 2873 656c 6629 202d 3e20 7374  Text(self) -> st
+0000afd0: 723a 0a20 2020 2020 2020 2027 2727 5374  r:.        '''St
+0000afe0: 7269 7020 616c 6c20 4c54 4d4c 2074 6167  rip all LTML tag
+0000aff0: 7320 616e 6420 7265 7475 726e 2074 6865  s and return the
+0000b000: 2075 6e64 6572 6c79 696e 6720 7465 7874   underlying text
+0000b010: 2e0a 0a20 2020 2020 2020 2053 6565 2041  ...        See A
+0000b020: 6c73 6f3a 0a20 2020 2020 2020 2020 2020  lso:.           
+0000b030: 202d 2060 7773 7461 7465 603a 2052 6574   - `wstate`: Ret
+0000b040: 7572 6e20 7468 6520 4c54 4d4c 2073 7472  urn the LTML str
+0000b050: 696e 672e 0a20 2020 2020 2020 2020 2020  ing..           
+0000b060: 202d 2060 7773 7461 7465 4c54 4d4c 603a   - `wstateLTML`:
+0000b070: 2047 656e 6572 6174 6520 6120 6c69 7374   Generate a list
+0000b080: 206f 6620 4c54 4d4c 2070 6172 7365 6420   of LTML parsed 
+0000b090: 6f62 6a65 6374 732e 0a20 2020 2020 2020  objects..       
+0000b0a0: 2027 2727 0a20 2020 2020 2020 2023 2054   '''.        # T
+0000b0b0: 4f44 4f3a 2053 6176 6520 7468 6520 7061  ODO: Save the pa
+0000b0c0: 7273 6564 204c 544d 4c20 7374 6174 6520  rsed LTML state 
+0000b0d0: 736f 6d65 7768 6572 6520 696e 2074 6869  somewhere in thi
+0000b0e0: 7320 6f62 6a65 6374 2c20 7769 7468 2060  s object, with `
+0000b0f0: 6461 7461 603f 0a20 2020 2020 2020 2072  data`?.        r
+0000b100: 6574 7572 6e20 2727 2e6a 6f69 6e28 0a20  eturn ''.join(. 
+0000b110: 2020 2020 2020 2020 2020 2074 652e 7465             te.te
+0000b120: 7874 0a20 2020 2020 2020 2020 2020 2066  xt.            f
+0000b130: 6f72 2074 6520 696e 2070 6172 7365 722e  or te in parser.
+0000b140: 7061 7273 655f 4c54 4d4c 2873 656c 662e  parse_LTML(self.
+0000b150: 7773 7461 7465 290a 2020 2020 2020 2020  wstate).        
+0000b160: 290a 0a0a 636c 6173 7320 4e6f 7465 626f  )...class Notebo
+0000b170: 6f6b 2874 746b 2e4e 6f74 6562 6f6f 6b2c  ok(ttk.Notebook,
+0000b180: 206d 6978 696e 2e43 6f6e 7461 696e 6572   mixin.Container
+0000b190: 5769 6467 6574 293a 0a20 2020 2027 2727  Widget):.    '''
+0000b1a0: 4120 7461 6262 6564 2069 6e74 6572 6661  A tabbed interfa
+0000b1b0: 6365 2074 6f20 686f 6c64 206f 7468 6572  ce to hold other
+0000b1c0: 2063 6f6e 7461 696e 6572 732e 0a0a 2020   containers...  
+0000b1d0: 2020 5468 6973 2069 7320 6120 7461 6262    This is a tabb
+0000b1e0: 6564 2069 6e74 6572 6661 6365 2074 6f20  ed interface to 
+0000b1f0: 7368 6f77 2073 6576 6572 616c 2063 6f6e  show several con
+0000b200: 7461 696e 6572 7320 696e 2074 6865 2073  tainers in the s
+0000b210: 616d 6520 7370 6163 652e 0a0a 2020 2020  ame space...    
+0000b220: 5468 6520 696e 6469 7669 6475 616c 2074  The individual t
+0000b230: 6162 7320 6d75 7374 2061 6c6c 2062 6520  abs must all be 
+0000b240: 636f 6e74 6169 6e65 7273 2c20 7468 6572  containers, ther
+0000b250: 6527 7320 6e6f 2073 7570 706f 7274 2066  e's no support f
+0000b260: 6f72 2073 696e 676c 650a 2020 2020 7769  or single.    wi
+0000b270: 6467 6574 732e 2055 7365 2061 2068 6f6c  dgets. Use a hol
+0000b280: 6465 7220 6046 7261 6d65 556e 6c61 6265  der `FrameUnlabe
+0000b290: 6c6c 6564 6020 746f 2073 686f 7720 6120  lled` to show a 
+0000b2a0: 7369 6e67 6c65 2077 6964 6765 7420 666f  single widget fo
+0000b2b0: 7220 6561 6368 0a20 2020 2074 6162 2e0a  r each.    tab..
+0000b2c0: 0a20 2020 2054 6865 7265 2069 7320 6e6f  .    There is no
+0000b2d0: 2050 7974 686f 6e20 646f 6375 6d65 6e74   Python document
+0000b2e0: 6174 696f 6e2c 2073 6565 2060 6054 6b60  ation, see ``Tk`
+0000b2f0: 6020 6074 746b 2e4e 6f74 6562 6f6f 6b20  ` `ttk.Notebook 
+0000b300: 3c68 7474 7073 3a2f 2f77 7777 2e74 636c  <https://www.tcl
+0000b310: 2e74 6b2f 6d61 6e2f 7463 6c2f 546b 436d  .tk/man/tcl/TkCm
+0000b320: 642f 7474 6b5f 6e6f 7465 626f 6f6b 2e68  d/ttk_notebook.h
+0000b330: 746d 6c3e 605f 2064 6f63 756d 656e 7461  tml>`_ documenta
+0000b340: 7469 6f6e 2e0a 0a20 2020 2041 7267 733a  tion...    Args:
+0000b350: 0a20 2020 2020 2020 2074 7261 7665 7273  .        travers
+0000b360: 616c 3a20 5365 7475 7020 7461 6220 7472  al: Setup tab tr
+0000b370: 6176 6572 7361 6c20 7769 7468 2073 7065  aversal with spe
+0000b380: 6369 616c 206b 6579 626f 6172 6420 7368  cial keyboard sh
+0000b390: 6f72 7463 7574 732c 2061 6e64 0a20 2020  ortcuts, and.   
+0000b3a0: 2020 2020 2020 2020 2061 6c73 6f20 7769           also wi
+0000b3b0: 7468 206d 6f75 7365 2077 6865 656c 2073  th mouse wheel s
+0000b3c0: 6372 6f6c 6c69 6e67 2e20 5365 6520 7468  crolling. See th
+0000b3d0: 6520 546b 2064 6f63 756d 656e 7461 7469  e Tk documentati
+0000b3e0: 6f6e 2066 6f72 2074 6865 0a20 2020 2020  on for the.     
+0000b3f0: 2020 2020 2020 206b 6579 626f 6172 6420         keyboard 
+0000b400: 7061 7274 2e20 456e 6162 6c65 6420 6279  part. Enabled by
+0000b410: 2064 6566 6175 6c74 2e0a 2020 2020 2020   default..      
+0000b420: 2020 7472 6176 6572 7361 6c57 7261 7061    traversalWrapa
+0000b430: 726f 756e 643a 2057 6865 6e20 6060 7472  round: When ``tr
+0000b440: 6176 6572 7361 6c60 6020 6973 2073 6574  aversal`` is set
+0000b450: 7570 2c20 636f 6e66 6967 7572 6520 7772  up, configure wr
+0000b460: 6170 6172 6f75 6e64 2e0a 2020 2020 2020  aparound..      
+0000b470: 2020 2020 2020 5468 6174 2069 732c 2073        That is, s
+0000b480: 6372 6f6c 6c69 6e67 2074 6f20 7468 6520  crolling to the 
+0000b490: 6e65 7874 2074 6162 2066 726f 6d20 7468  next tab from th
+0000b4a0: 6520 6c61 7374 206f 6e65 2073 686f 756c  e last one shoul
+0000b4b0: 6420 2273 6372 6f6c 6c22 0a20 2020 2020  d "scroll".     
+0000b4c0: 2020 2020 2020 2069 6e74 6f20 7468 6520         into the 
+0000b4d0: 6669 7273 7420 7461 622c 2061 6e64 2076  first tab, and v
+0000b4e0: 6963 652d 7665 7273 6120 666f 7220 7468  ice-versa for th
+0000b4f0: 6520 6669 7273 7420 7461 622e 2054 6869  e first tab. Thi
+0000b500: 7320 6f6e 6c79 206d 6174 7465 7273 0a20  s only matters. 
+0000b510: 2020 2020 2020 2020 2020 2066 6f72 2074             for t
+0000b520: 6865 206d 6f75 7365 2077 6865 656c 2074  he mouse wheel t
+0000b530: 7261 7665 7273 616c 2c20 7468 6520 6b65  raversal, the ke
+0000b540: 7962 6f61 7264 2073 686f 7274 6375 7473  yboard shortcuts
+0000b550: 2061 6c77 6179 7320 656e 6162 6c65 0a20   always enable. 
+0000b560: 2020 2020 2020 2020 2020 2074 6869 7320             this 
+0000b570: 7472 6176 6572 7361 6c2e 0a20 2020 2020  traversal..     
+0000b580: 2020 2020 2020 2044 6973 6162 6c65 6420         Disabled 
+0000b590: 6279 2064 6566 6175 6c74 2e0a 0a20 2020  by default...   
+0000b5a0: 2020 2020 206c 6179 6f75 743a 2049 676e       layout: Ign
+0000b5b0: 6f72 6564 2c20 6974 2069 7320 6861 7264  ored, it is hard
+0000b5c0: 636f 6465 6420 746f 2060 4e6f 6e65 6020  coded to `None` 
+0000b5d0: 616c 7761 7973 2e0a 2020 2020 2020 2020  always..        
+0000b5e0: 7061 7265 6e74 3a20 5468 6520 7061 7265  parent: The pare
+0000b5f0: 6e74 2077 6964 6765 742e 2043 616e 2062  nt widget. Can b
+0000b600: 6520 6120 6052 6f6f 7457 696e 646f 7760  e a `RootWindow`
+0000b610: 206f 7220 616e 6f74 6865 7220 606d 6978   or another `mix
+0000b620: 696e 2e43 6f6e 7461 696e 6572 5769 6467  in.ContainerWidg
+0000b630: 6574 602e 0a0a 2020 2020 5365 6520 416c  et`...    See Al
+0000b640: 736f 3a0a 2020 2020 2020 2020 604e 6f74  so:.        `Not
+0000b650: 6562 6f6f 6b55 6e69 666f 726d 603a 2041  ebookUniform`: A
+0000b660: 2073 696d 706c 6572 2076 6572 7369 6f6e   simpler version
+0000b670: 206f 6620 7468 6973 2c20 7768 656e 2065   of this, when e
+0000b680: 6163 6820 696e 6469 7669 6475 616c 2074  ach individual t
+0000b690: 6162 2069 7320 7468 6520 7361 6d65 2074  ab is the same t
+0000b6a0: 7970 650a 2020 2020 2727 270a 2020 2020  ype.    '''.    
+0000b6b0: 5461 6220 3d20 6d6f 6465 6c2e 4e6f 7465  Tab = model.Note
+0000b6c0: 626f 6f6b 5461 6220 2023 2041 6c69 6173  bookTab  # Alias
+0000b6d0: 2074 6865 206e 6f74 6562 6f6f 6b20 7461   the notebook ta
+0000b6e0: 6220 696e 666f 726d 6174 696f 6e20 2023  b information  #
+0000b6f0: 2054 4f44 4f3a 204d 6f76 6520 4e6f 7465   TODO: Move Note
+0000b700: 626f 6f6b 5461 6220 636c 6173 7320 6865  bookTab class he
+0000b710: 7265 3f0a 2020 2020 2727 2741 6c69 6173  re?.    '''Alias
+0000b720: 2066 6f72 2060 6d6f 6465 6c2e 4e6f 7465   for `model.Note
+0000b730: 626f 6f6b 5461 6260 2063 6c61 7373 2e27  bookTab` class.'
+0000b740: 2727 0a20 2020 2077 7461 6273 3a20 7479  ''.    wtabs: ty
+0000b750: 7069 6e67 2e4d 6170 7069 6e67 5b73 7472  ping.Mapping[str
+0000b760: 2c20 6d6f 6465 6c2e 4e6f 7465 626f 6f6b  , model.Notebook
+0000b770: 5461 625d 0a20 2020 2027 2727 4d61 7070  Tab].    '''Mapp
+0000b780: 696e 6720 6f66 2074 6162 2069 6465 6e74  ing of tab ident
+0000b790: 6966 6965 7273 2c20 616e 6420 606d 6f64  ifiers, and `mod
+0000b7a0: 656c 2e4e 6f74 6562 6f6f 6b54 6162 6020  el.NotebookTab` 
+0000b7b0: 6f62 6a65 6374 732e 2727 270a 0a20 2020  objects.'''..   
+0000b7c0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+0000b7d0: 6c66 2c20 7061 7265 6e74 2c20 2a61 7267  lf, parent, *arg
+0000b7e0: 732c 206c 6179 6f75 743a 204e 6f6e 6520  s, layout: None 
+0000b7f0: 3d20 4e6f 6e65 2c20 7472 6176 6572 7361  = None, traversa
+0000b800: 6c3a 2062 6f6f 6c20 3d20 5472 7565 2c20  l: bool = True, 
+0000b810: 7472 6176 6572 7361 6c57 7261 7061 726f  traversalWraparo
+0000b820: 756e 643a 2062 6f6f 6c20 3d20 4661 6c73  und: bool = Fals
+0000b830: 652c 202a 2a6b 7761 7267 7329 3a0a 2020  e, **kwargs):.  
+0000b840: 2020 2020 2020 7375 7065 7228 292e 5f5f        super().__
+0000b850: 696e 6974 5f5f 2870 6172 656e 7429 0a20  init__(parent). 
+0000b860: 2020 2020 2020 2023 204e 6f20 606c 6179         # No `lay
+0000b870: 6f75 7460 2069 7320 7573 6564 2c20 666f  out` is used, fo
+0000b880: 7263 6520 6974 2074 6f20 604e 6f6e 6560  rce it to `None`
+0000b890: 0a20 2020 2020 2020 2073 656c 662e 696e  .        self.in
+0000b8a0: 6974 5f63 6f6e 7461 696e 6572 282a 6172  it_container(*ar
+0000b8b0: 6773 2c20 6c61 796f 7574 3d4e 6f6e 652c  gs, layout=None,
+0000b8c0: 202a 2a6b 7761 7267 7329 0a20 2020 2020   **kwargs).     
+0000b8d0: 2020 2023 2054 6162 2054 7261 7665 7273     # Tab Travers
+0000b8e0: 616c 0a20 2020 2020 2020 2073 656c 662e  al.        self.
+0000b8f0: 7457 7261 7061 726f 756e 6420 3d20 7472  tWraparound = tr
+0000b900: 6176 6572 7361 6c57 7261 7061 726f 756e  aversalWraparoun
+0000b910: 640a 2020 2020 2020 2020 6966 2074 7261  d.        if tra
+0000b920: 7665 7273 616c 3a0a 2020 2020 2020 2020  versal:.        
+0000b930: 2020 2020 2320 544f 444f 3a20 5265 2d49      # TODO: Re-I
+0000b940: 6d70 6c65 6d65 6e74 206c 6f63 616c 6c79  mplement locally
+0000b950: 2c20 7461 6b65 2060 7472 6176 6572 7361  , take `traversa
+0000b960: 6c57 7261 7061 726f 756e 6460 2069 6e74  lWraparound` int
+0000b970: 6f20 6163 636f 756e 742e 0a20 2020 2020  o account..     
+0000b980: 2020 2020 2020 2023 2020 2020 2020 204d         #       M
+0000b990: 6170 3a0a 2020 2020 2020 2020 2020 2020  ap:.            
+0000b9a0: 2320 2020 2020 2020 2d20 6043 7472 6c2d  #       - `Ctrl-
+0000b9b0: 5461 6260 3a20 5f74 6162 5363 726f 6c6c  Tab`: _tabScroll
+0000b9c0: 5570 0a20 2020 2020 2020 2020 2020 2023  Up.            #
+0000b9d0: 2020 2020 2020 202d 2060 4374 726c 2d53         - `Ctrl-S
+0000b9e0: 6869 6674 2d54 6162 603a 205f 7461 6253  hift-Tab`: _tabS
+0000b9f0: 6372 6f6c 6c44 6f77 6e0a 2020 2020 2020  crollDown.      
+0000ba00: 2020 2020 2020 7365 6c66 2e65 6e61 626c        self.enabl
+0000ba10: 655f 7472 6176 6572 7361 6c28 290a 2020  e_traversal().  
+0000ba20: 2020 2020 2020 2020 2020 2320 4269 6e64            # Bind
+0000ba30: 206d 6f75 7365 2077 6865 656c 3a20 4469   mouse wheel: Di
+0000ba40: 6769 7461 6c20 5363 726f 6c6c 696e 670a  gital Scrolling.
+0000ba50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ba60: 2e5f 7472 6176 6572 7361 6c20 3d20 666e  ._traversal = fn
+0000ba70: 2e62 696e 645f 6d6f 7573 6577 6865 656c  .bind_mousewheel
+0000ba80: 2873 656c 662c 2075 703d 7365 6c66 2e5f  (self, up=self._
+0000ba90: 7461 6253 6372 6f6c 6c55 702c 2064 6f77  tabScrollUp, dow
+0000baa0: 6e3d 7365 6c66 2e5f 7461 6253 6372 6f6c  n=self._tabScrol
+0000bab0: 6c44 6f77 6e2c 2069 6d6d 6564 6961 7465  lDown, immediate
+0000bac0: 3d54 7275 6529 0a0a 2020 2020 6465 6620  =True)..    def 
+0000bad0: 7365 7475 705f 7769 6467 6574 7328 7365  setup_widgets(se
+0000bae0: 6c66 2c20 2a61 7267 732c 202a 2a6b 7761  lf, *args, **kwa
+0000baf0: 7267 7329 3a0a 2020 2020 2020 2020 2727  rgs):.        ''
+0000bb00: 2744 6566 696e 6520 7468 6520 7375 6220  'Define the sub 
+0000bb10: 7769 6467 6574 7320 6261 7365 6420 6f6e  widgets based on
+0000bb20: 2074 6865 2074 6162 732e 0a0a 2020 2020   the tabs...    
+0000bb30: 2020 2020 446f 206e 6f74 206f 7665 7277      Do not overw
+0000bb40: 7269 7465 2074 6869 7320 756e 6c65 7373  rite this unless
+0000bb50: 2079 6f75 206b 6e6f 7720 7768 6174 2079   you know what y
+0000bb60: 6f75 2061 7265 2064 6f69 6e67 2e0a 0a20  ou are doing... 
+0000bb70: 2020 2020 2020 2054 6f20 6564 6974 2074         To edit t
+0000bb80: 6865 2074 6162 732c 2073 6565 2060 7365  he tabs, see `se
+0000bb90: 7475 705f 7461 6273 602e 0a20 2020 2020  tup_tabs`..     
+0000bba0: 2020 2027 2727 0a20 2020 2020 2020 2073     '''.        s
+0000bbb0: 656c 662e 7774 6162 7320 3d20 7365 6c66  elf.wtabs = self
+0000bbc0: 2e73 6574 7570 5f74 6162 7328 2a61 7267  .setup_tabs(*arg
+0000bbd0: 732c 202a 2a6b 7761 7267 7329 0a20 2020  s, **kwargs).   
+0000bbe0: 2020 2020 2023 2069 6620 5f5f 6465 6275       # if __debu
+0000bbf0: 675f 5f3a 0a20 2020 2020 2020 2023 2020  g__:.        #  
+0000bc00: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+0000bc10: 6627 7b73 656c 667d 3a20 7b6c 656e 2873  f'{self}: {len(s
+0000bc20: 656c 662e 7774 6162 7329 7d20 5461 6273  elf.wtabs)} Tabs
+0000bc30: 2729 0a20 2020 2020 2020 2077 6964 6765  ').        widge
+0000bc40: 7473 203d 207b 7d0a 2020 2020 2020 2020  ts = {}.        
+0000bc50: 666f 7220 6964 656e 7469 6669 6572 2c20  for identifier, 
+0000bc60: 7469 2069 6e20 7365 6c66 2e77 7461 6273  ti in self.wtabs
+0000bc70: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
+0000bc80: 2020 2020 2020 2320 6966 205f 5f64 6562        # if __deb
+0000bc90: 7567 5f5f 3a0a 2020 2020 2020 2020 2020  ug__:.          
+0000bca0: 2020 2320 2020 2020 6c6f 6767 6572 2e64    #     logger.d
+0000bcb0: 6562 7567 2827 3e20 2573 3a20 2572 272c  ebug('> %s: %r',
+0000bcc0: 2074 692e 6e61 6d65 2c20 7469 2e77 6964   ti.name, ti.wid
+0000bcd0: 6765 7429 0a20 2020 2020 2020 2020 2020  get).           
+0000bce0: 2061 7373 6572 7420 6973 696e 7374 616e   assert isinstan
+0000bcf0: 6365 2874 692e 7769 6467 6574 2c20 6d69  ce(ti.widget, mi
+0000bd00: 7869 6e2e 436f 6e74 6169 6e65 7257 6964  xin.ContainerWid
+0000bd10: 6765 7429 2c20 6627 7b73 656c 6621 727d  get), f'{self!r}
+0000bd20: 3a20 5461 6220 5769 6467 6574 205b 7b74  : Tab Widget [{t
+0000bd30: 692e 6964 656e 7469 6669 6572 206f 7220  i.identifier or 
+0000bd40: 6964 656e 7469 6669 6572 7d5d 227b 7469  identifier}]"{ti
+0000bd50: 2e6e 616d 657d 2220 6d75 7374 2062 6520  .name}" must be 
+0000bd60: 6120 636f 6e74 6169 6e65 7227 0a20 2020  a container'.   
+0000bd70: 2020 2020 2020 2020 2065 7874 7261 203d           extra =
+0000bd80: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+0000bd90: 2020 202a 2a74 692e 6578 7472 612c 0a20     **ti.extra,. 
+0000bda0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0000bdb0: 7465 7874 273a 2074 692e 6e61 6d65 2c0a  text': ti.name,.
+0000bdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bdd0: 2769 6d61 6765 273a 2074 692e 696d 6167  'image': ti.imag
+0000bde0: 6520 6f72 2027 272c 0a20 2020 2020 2020  e or '',.       
+0000bdf0: 2020 2020 2020 2020 2027 636f 6d70 6f75           'compou
+0000be00: 6e64 273a 2074 692e 696d 6167 6543 6f6d  nd': ti.imageCom
+0000be10: 706f 756e 642c 0a20 2020 2020 2020 2020  pound,.         
+0000be20: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
+0000be30: 2073 656c 662e 6164 6428 7469 2e77 6964   self.add(ti.wid
+0000be40: 6765 742c 202a 2a65 7874 7261 290a 2020  get, **extra).  
+0000be50: 2020 2020 2020 2020 2020 7469 2e69 6465            ti.ide
+0000be60: 6e74 6966 6965 7220 3d20 6964 656e 7469  ntifier = identi
+0000be70: 6669 6572 0a20 2020 2020 2020 2020 2020  fier.           
+0000be80: 2077 6964 6765 7473 5b69 6465 6e74 6966   widgets[identif
+0000be90: 6965 725d 203d 2074 692e 7769 6467 6574  ier] = ti.widget
+0000bea0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000beb0: 7769 6467 6574 730a 0a20 2020 2064 6566  widgets..    def
+0000bec0: 2073 6574 7570 5f74 6162 7328 7365 6c66   setup_tabs(self
+0000bed0: 2c20 2a61 7267 732c 202a 2a6b 7761 7267  , *args, **kwarg
+0000bee0: 7329 202d 3e20 7479 7069 6e67 2e4d 6170  s) -> typing.Map
+0000bef0: 7069 6e67 5b73 7472 2c20 6d6f 6465 6c2e  ping[str, model.
+0000bf00: 4e6f 7465 626f 6f6b 5461 625d 3a0a 2020  NotebookTab]:.  
+0000bf10: 2020 2020 2020 2727 2744 6566 696e 6520        '''Define 
+0000bf20: 7468 6520 7461 6273 2068 6572 652e 0a0a  the tabs here...
+0000bf30: 2020 2020 2020 2020 5369 6d69 6c61 7220          Similar 
+0000bf40: 746f 2060 7365 7475 705f 7769 6467 6574  to `setup_widget
+0000bf50: 7320 3c6d 6978 696e 2e43 6f6e 7461 696e  s <mixin.Contain
+0000bf60: 6572 5769 6467 6574 2e73 6574 7570 5f77  erWidget.setup_w
+0000bf70: 6964 6765 7473 3e60 2c20 6275 740a 2020  idgets>`, but.  
+0000bf80: 2020 2020 2020 6465 6669 6e65 7320 606d        defines `m
+0000bf90: 6f64 656c 2e4e 6f74 6562 6f6f 6b54 6162  odel.NotebookTab
+0000bfa0: 602c 2065 7874 7261 2069 6e66 6f72 6d61  `, extra informa
+0000bfb0: 7469 6f6e 2061 626f 7574 2065 6163 6820  tion about each 
+0000bfc0: 7769 6467 6574 2e0a 2020 2020 2020 2020  widget..        
+0000bfd0: 2727 270a 2020 2020 2020 2020 7261 6973  '''.        rais
+0000bfe0: 6520 4e6f 7449 6d70 6c65 6d65 6e74 6564  e NotImplemented
+0000bff0: 4572 726f 720a 0a20 2020 2064 6566 2077  Error..    def w
+0000c000: 7461 6228 7365 6c66 2c20 6964 783a 2073  tab(self, idx: s
+0000c010: 7472 2920 2d3e 206d 6978 696e 2e43 6f6e  tr) -> mixin.Con
+0000c020: 7461 696e 6572 5769 6467 6574 3a0a 2020  tainerWidget:.  
+0000c030: 2020 2020 2020 2727 2747 6574 2074 6865        '''Get the
+0000c040: 2074 6162 2077 6964 6765 7420 6279 2069   tab widget by i
+0000c050: 6465 6e74 6966 6965 722e 0a0a 2020 2020  dentifier...    
+0000c060: 2020 2020 5468 6973 2069 7320 6a75 7374      This is just
+0000c070: 2061 6e20 6865 6c70 6572 2066 756e 6374   an helper funct
+0000c080: 696f 6e20 746f 2067 6574 2074 6865 2063  ion to get the c
+0000c090: 6f72 7265 6374 2077 6964 6765 7420 7661  orrect widget va
+0000c0a0: 6c75 6520 6f75 7420 6f66 0a20 2020 2020  lue out of.     
+0000c0b0: 2020 2060 7774 6162 7360 2e0a 0a20 2020     `wtabs`...   
+0000c0c0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+0000c0d0: 2020 2020 2020 2069 6478 3a20 5468 6520         idx: The 
+0000c0e0: 7461 6220 6964 656e 7469 6669 6572 2e0a  tab identifier..
+0000c0f0: 0a20 2020 2020 2020 204e 6f74 653a 0a20  .        Note:. 
+0000c100: 2020 2020 2020 2020 2020 2049 6e20 6465             In de
+0000c110: 6275 6720 6d6f 6465 2c20 7468 6973 2077  bug mode, this w
+0000c120: 696c 6c20 6661 696c 2069 6620 6361 6c6c  ill fail if call
+0000c130: 6564 2077 6974 6820 7468 6520 7772 6f6e  ed with the wron
+0000c140: 6720 6964 656e 7469 6669 6572 2e0a 2020  g identifier..  
+0000c150: 2020 2020 2020 2020 2020 5468 6973 2063            This c
+0000c160: 6865 636b 2069 7320 736b 6970 7065 6420  heck is skipped 
+0000c170: 666f 7220 7065 7266 6f72 6d61 6e63 6520  for performance 
+0000c180: 6f6e 206f 7074 696d 697a 6564 206d 6f64  on optimized mod
+0000c190: 652e 0a20 2020 2020 2020 2027 2727 0a20  e..        '''. 
+0000c1a0: 2020 2020 2020 2077 7461 6220 3d20 7365         wtab = se
+0000c1b0: 6c66 2e77 7461 6273 2e67 6574 2869 6478  lf.wtabs.get(idx
+0000c1c0: 2c20 4e6f 6e65 290a 2020 2020 2020 2020  , None).        
+0000c1d0: 6173 7365 7274 2077 7461 6220 6973 206e  assert wtab is n
+0000c1e0: 6f74 204e 6f6e 652c 2066 2749 6e76 616c  ot None, f'Inval
+0000c1f0: 6964 2053 656c 6563 7469 6f6e 3a20 7b69  id Selection: {i
+0000c200: 6478 7d27 0a20 2020 2020 2020 2072 6574  dx}'.        ret
+0000c210: 7572 6e20 7774 6162 2e77 6964 6765 740a  urn wtab.widget.
+0000c220: 0a20 2020 2064 6566 2077 7365 6c65 6374  .    def wselect
+0000c230: 696f 6e28 7365 6c66 2920 2d3e 2073 7472  ion(self) -> str
+0000c240: 3a0a 2020 2020 2020 2020 2727 2753 6561  :.        '''Sea
+0000c250: 7263 6820 666f 7220 7468 6520 6375 7272  rch for the curr
+0000c260: 656e 7420 7365 6c65 6374 6564 2074 6162  ent selected tab
+0000c270: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+0000c280: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+0000c290: 5468 6973 2066 756e 6374 696f 6e73 2073  This functions s
+0000c2a0: 6561 7263 6865 7320 666f 7220 7468 6520  earches for the 
+0000c2b0: 6375 7272 656e 746c 7920 7365 6c65 6374  currently select
+0000c2c0: 6564 2074 6162 2c20 616e 6420 7265 7475  ed tab, and retu
+0000c2d0: 726e 7320 6974 730a 2020 2020 2020 2020  rns its.        
+0000c2e0: 2020 2020 6964 656e 7469 6669 6572 2028      identifier (
+0000c2f0: 7468 6520 6b65 7920 6f6e 2074 6865 2060  the key on the `
+0000c300: 7774 6162 7360 2064 6963 7469 6f6e 6172  wtabs` dictionar
+0000c310: 7929 2e0a 2020 2020 2020 2020 2727 270a  y)..        '''.
+0000c320: 2020 2020 2020 2020 2320 544f 444f 3a20          # TODO: 
+0000c330: 4f70 7469 6d69 7365 2074 6869 733f 2053  Optimise this? S
+0000c340: 6176 6520 6120 6469 6374 206f 6620 696e  ave a dict of in
+0000c350: 6465 7865 7320 6f72 2073 6f6d 6574 6869  dexes or somethi
+0000c360: 6e67 3f0a 2020 2020 2020 2020 7365 6c65  ng?.        sele
+0000c370: 6374 6564 5f69 6420 3d20 7365 6c66 2e73  cted_id = self.s
+0000c380: 656c 6563 7428 290a 2020 2020 2020 2020  elect().        
+0000c390: 2320 6966 205f 5f64 6562 7567 5f5f 3a0a  # if __debug__:.
+0000c3a0: 2020 2020 2020 2020 2320 2020 2020 6c6f          #     lo
+0000c3b0: 6767 6572 2e64 6562 7567 2827 533a 2025  gger.debug('S: %
+0000c3c0: 7227 2c20 7365 6c65 6374 6564 5f69 6429  r', selected_id)
+0000c3d0: 0a20 2020 2020 2020 2023 2020 2020 2074  .        #     t
+0000c3e0: 6162 735f 6964 203d 205b 7374 7228 7729  abs_id = [str(w)
+0000c3f0: 2066 6f72 2077 2069 6e20 7365 6c66 2e74   for w in self.t
+0000c400: 6162 7328 295d 0a20 2020 2020 2020 2023  abs()].        #
+0000c410: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+0000c420: 6728 2720 7c20 2573 272c 2027 2027 2e6a  g(' | %s', ' '.j
+0000c430: 6f69 6e28 7461 6273 5f69 6429 290a 2020  oin(tabs_id)).  
+0000c440: 2020 2020 2020 666f 7220 6964 782c 2077        for idx, w
+0000c450: 7461 6220 696e 2073 656c 662e 7774 6162  tab in self.wtab
+0000c460: 732e 6974 656d 7328 293a 0a20 2020 2020  s.items():.     
+0000c470: 2020 2020 2020 2069 6620 7374 7228 7774         if str(wt
+0000c480: 6162 2e77 6964 6765 7429 203d 3d20 7365  ab.widget) == se
+0000c490: 6c65 6374 6564 5f69 643a 0a20 2020 2020  lected_id:.     
+0000c4a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000c4b0: 6e20 6964 780a 2020 2020 2020 2020 7261  n idx.        ra
+0000c4c0: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
+0000c4d0: 7b73 656c 6621 727d 3a20 496e 7661 6c69  {self!r}: Invali
+0000c4e0: 6420 6375 7272 656e 7420 7365 6c65 6374  d current select
+0000c4f0: 696f 6e3a 207b 7365 6c65 6374 6564 5f69  ion: {selected_i
+0000c500: 6421 727d 2729 0a0a 2020 2020 6465 6620  d!r}')..    def 
+0000c510: 7773 656c 6563 7428 7365 6c66 2c20 6964  wselect(self, id
+0000c520: 783a 2073 7472 2920 2d3e 204e 6f6e 653a  x: str) -> None:
+0000c530: 0a20 2020 2020 2020 2027 2727 5365 6c65  .        '''Sele
+0000c540: 6374 2061 2074 6162 2062 7920 6964 656e  ct a tab by iden
+0000c550: 7469 6669 6572 2e0a 0a20 2020 2020 2020  tifier...       
+0000c560: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+0000c570: 2020 2069 6478 3a20 5468 6520 7461 6220     idx: The tab 
+0000c580: 6964 656e 7469 6669 6572 2e0a 0a20 2020  identifier...   
+0000c590: 2020 2020 204e 6f74 653a 0a20 2020 2020       Note:.     
+0000c5a0: 2020 2020 2020 2049 6e20 6465 6275 6720         In debug 
+0000c5b0: 6d6f 6465 2c20 7468 6973 2077 696c 6c20  mode, this will 
+0000c5c0: 6661 696c 2069 6620 6361 6c6c 6564 2077  fail if called w
+0000c5d0: 6974 6820 7468 6520 7772 6f6e 6720 6964  ith the wrong id
+0000c5e0: 656e 7469 6669 6572 2e0a 2020 2020 2020  entifier..      
+0000c5f0: 2020 2020 2020 5468 6973 2063 6865 636b        This check
+0000c600: 2069 7320 736b 6970 7065 6420 666f 7220   is skipped for 
+0000c610: 7065 7266 6f72 6d61 6e63 6520 6f6e 206f  performance on o
+0000c620: 7074 696d 697a 6564 206d 6f64 652e 0a20  ptimized mode.. 
+0000c630: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+0000c640: 2020 2077 7461 6220 3d20 7365 6c66 2e77     wtab = self.w
+0000c650: 7461 6273 2e67 6574 2869 6478 2c20 4e6f  tabs.get(idx, No
+0000c660: 6e65 290a 2020 2020 2020 2020 6173 7365  ne).        asse
+0000c670: 7274 2077 7461 6220 6973 206e 6f74 204e  rt wtab is not N
+0000c680: 6f6e 652c 2066 2749 6e76 616c 6964 2053  one, f'Invalid S
+0000c690: 656c 6563 7469 6f6e 3a20 7b69 6478 7d27  election: {idx}'
+0000c6a0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+0000c6b0: 6c65 6374 2874 6162 5f69 643d 7374 7228  lect(tab_id=str(
+0000c6c0: 7774 6162 2e77 6964 6765 7429 290a 0a20  wtab.widget)).. 
+0000c6d0: 2020 2064 6566 205f 7461 6253 6372 6f6c     def _tabScrol
+0000c6e0: 6c55 7028 7365 6c66 2c20 6576 656e 743d  lUp(self, event=
+0000c6f0: 4e6f 6e65 293a 0a20 2020 2020 2020 206b  None):.        k
+0000c700: 6579 7320 3d20 6c69 7374 2873 656c 662e  eys = list(self.
+0000c710: 7774 6162 732e 6b65 7973 2829 290a 2020  wtabs.keys()).  
+0000c720: 2020 2020 2020 7365 6c65 6374 6564 203d        selected =
+0000c730: 2073 656c 662e 7773 656c 6563 7469 6f6e   self.wselection
+0000c740: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+0000c750: 6c65 6374 6564 203d 3d20 6b65 7973 5b30  lected == keys[0
+0000c760: 5d3a 0a20 2020 2020 2020 2020 2020 2023  ]:.            #
+0000c770: 2046 6972 7374 2054 6162 0a20 2020 2020   First Tab.     
+0000c780: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
+0000c790: 5772 6170 6172 6f75 6e64 3a0a 2020 2020  Wraparound:.    
+0000c7a0: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+0000c7b0: 7365 6c65 6374 6564 203d 206b 6579 735b  selected = keys[
+0000c7c0: 2d31 5d0a 2020 2020 2020 2020 2020 2020  -1].            
+0000c7d0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000c7e0: 2020 2020 2020 6e65 775f 7365 6c65 6374        new_select
+0000c7f0: 6564 203d 204e 6f6e 650a 2020 2020 2020  ed = None.      
+0000c800: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000c810: 2020 2020 2320 544f 444f 3a20 4f70 7469      # TODO: Opti
+0000c820: 6d69 7365 2074 6869 733f 2053 6565 2060  mise this? See `
+0000c830: 7773 656c 6563 7469 6f6e 600a 2020 2020  wselection`.    
+0000c840: 2020 2020 2020 2020 7365 6c65 6374 6564          selected
+0000c850: 5f69 6478 203d 206b 6579 732e 696e 6465  _idx = keys.inde
+0000c860: 7828 7365 6c65 6374 6564 290a 2020 2020  x(selected).    
+0000c870: 2020 2020 2020 2020 6e65 775f 7365 6c65          new_sele
+0000c880: 6374 6564 203d 206b 6579 735b 7365 6c65  cted = keys[sele
+0000c890: 6374 6564 5f69 6478 202d 2031 5d0a 2020  cted_idx - 1].  
+0000c8a0: 2020 2020 2020 6966 206e 6577 5f73 656c        if new_sel
+0000c8b0: 6563 7465 643a 0a20 2020 2020 2020 2020  ected:.         
+0000c8c0: 2020 2073 656c 662e 7773 656c 6563 7428     self.wselect(
+0000c8d0: 6e65 775f 7365 6c65 6374 6564 290a 0a20  new_selected).. 
+0000c8e0: 2020 2064 6566 205f 7461 6253 6372 6f6c     def _tabScrol
+0000c8f0: 6c44 6f77 6e28 7365 6c66 2c20 6576 656e  lDown(self, even
+0000c900: 743d 4e6f 6e65 293a 0a20 2020 2020 2020  t=None):.       
+0000c910: 206b 6579 7320 3d20 6c69 7374 2873 656c   keys = list(sel
+0000c920: 662e 7774 6162 732e 6b65 7973 2829 290a  f.wtabs.keys()).
+0000c930: 2020 2020 2020 2020 7365 6c65 6374 6564          selected
+0000c940: 203d 2073 656c 662e 7773 656c 6563 7469   = self.wselecti
+0000c950: 6f6e 2829 0a20 2020 2020 2020 2069 6620  on().        if 
+0000c960: 7365 6c65 6374 6564 203d 3d20 6b65 7973  selected == keys
+0000c970: 5b2d 315d 3a0a 2020 2020 2020 2020 2020  [-1]:.          
+0000c980: 2020 2320 4c61 7374 2054 6162 0a20 2020    # Last Tab.   
+0000c990: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0000c9a0: 2e74 5772 6170 6172 6f75 6e64 3a0a 2020  .tWraparound:.  
+0000c9b0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+0000c9c0: 775f 7365 6c65 6374 6564 203d 206b 6579  w_selected = key
+0000c9d0: 735b 305d 0a20 2020 2020 2020 2020 2020  s[0].           
+0000c9e0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000c9f0: 2020 2020 2020 206e 6577 5f73 656c 6563         new_selec
+0000ca00: 7465 6420 3d20 4e6f 6e65 0a20 2020 2020  ted = None.     
+0000ca10: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000ca20: 2020 2020 2023 2054 4f44 4f3a 204f 7074       # TODO: Opt
+0000ca30: 696d 6973 6520 7468 6973 3f20 5365 6520  imise this? See 
+0000ca40: 6077 7365 6c65 6374 696f 6e60 0a20 2020  `wselection`.   
+0000ca50: 2020 2020 2020 2020 2073 656c 6563 7465           selecte
+0000ca60: 645f 6964 7820 3d20 6b65 7973 2e69 6e64  d_idx = keys.ind
+0000ca70: 6578 2873 656c 6563 7465 6429 0a20 2020  ex(selected).   
+0000ca80: 2020 2020 2020 2020 206e 6577 5f73 656c           new_sel
+0000ca90: 6563 7465 6420 3d20 6b65 7973 5b73 656c  ected = keys[sel
+0000caa0: 6563 7465 645f 6964 7820 2b20 315d 0a20  ected_idx + 1]. 
+0000cab0: 2020 2020 2020 2069 6620 6e65 775f 7365         if new_se
+0000cac0: 6c65 6374 6564 3a0a 2020 2020 2020 2020  lected:.        
+0000cad0: 2020 2020 7365 6c66 2e77 7365 6c65 6374      self.wselect
+0000cae0: 286e 6577 5f73 656c 6563 7465 6429 0a0a  (new_selected)..
+0000caf0: 0a63 6c61 7373 204e 6f74 6562 6f6f 6b55  .class NotebookU
+0000cb00: 6e69 666f 726d 284e 6f74 6562 6f6f 6b29  niform(Notebook)
+0000cb10: 3a0a 2020 2020 2727 2741 2074 6162 6265  :.    '''A tabbe
+0000cb20: 6420 696e 7465 7266 6163 6520 746f 2068  d interface to h
+0000cb30: 6f6c 6420 6120 7365 7269 6573 206f 6620  old a series of 
+0000cb40: 756e 6966 6f72 6d20 636f 6e74 6169 6e65  uniform containe
+0000cb50: 7273 2e0a 0a20 2020 2054 6869 7320 6973  rs...    This is
+0000cb60: 2061 2076 6172 6961 6e74 206f 6620 7468   a variant of th
+0000cb70: 6520 7265 6775 6c61 7220 604e 6f74 6562  e regular `Noteb
+0000cb80: 6f6f 6b60 2073 7065 6369 616c 6c79 2063  ook` specially c
+0000cb90: 7265 6174 6564 2074 6f20 7369 6d70 6c69  reated to simpli
+0000cba0: 6679 0a20 2020 2074 6865 2075 7375 616c  fy.    the usual
+0000cbb0: 2063 6173 6520 7768 6572 6520 616c 6c20   case where all 
+0000cbc0: 7468 6520 7461 6273 2061 7265 2076 6572  the tabs are ver
+0000cbd0: 7920 7369 6d69 6c61 7220 2875 7375 616c  y similar (usual
+0000cbe0: 6c79 2c20 7468 6579 2061 7265 2074 6865  ly, they are the
+0000cbf0: 0a20 2020 2073 616d 6520 756e 6465 726c  .    same underl
+0000cc00: 7969 6e67 2063 6c61 7373 292e 0a0a 2020  ying class)...  
+0000cc10: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+0000cc20: 7461 6269 6473 3a20 4120 6d61 7070 696e  tabids: A mappin
+0000cc30: 6720 6f66 2074 6162 2069 6465 6e74 6966  g of tab identif
+0000cc40: 6965 7273 2061 6e64 2074 6162 2074 6974  iers and tab tit
+0000cc50: 6c65 732e 0a0a 2020 2020 5365 6520 416c  les...    See Al
+0000cc60: 736f 3a0a 2020 2020 2020 2020 604e 6f74  so:.        `Not
+0000cc70: 6562 6f6f 6b60 3a20 4120 6675 6c6c 7920  ebook`: A fully 
+0000cc80: 6765 6e65 7269 6320 7665 7273 696f 6e20  generic version 
+0000cc90: 6f66 2074 6869 732e 2044 6f6e 2774 2074  of this. Don't t
+0000cca0: 7279 2074 6f20 6d61 6b65 2074 6865 0a20  ry to make the. 
+0000ccb0: 2020 2020 2020 2060 7365 7475 705f 7461         `setup_ta
+0000ccc0: 6260 2066 756e 6374 696f 6e20 746f 6f20  b` function too 
+0000ccd0: 636f 6d70 6c65 782c 206d 6f76 6520 746f  complex, move to
+0000cce0: 2074 6869 7320 7769 6467 6574 2069 6e73   this widget ins
+0000ccf0: 7465 6164 2e0a 2020 2020 2727 270a 2020  tead..    '''.  
+0000cd00: 2020 7461 6269 6473 3a20 7479 7069 6e67    tabids: typing
+0000cd10: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
+0000cd20: 2e4d 6170 7069 6e67 5b73 7472 2c20 7374  .Mapping[str, st
+0000cd30: 725d 5d20 3d20 4e6f 6e65 0a0a 2020 2020  r]] = None..    
+0000cd40: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+0000cd50: 662c 202a 6172 6773 2c20 7461 6269 6473  f, *args, tabids
+0000cd60: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+0000cd70: 6c5b 7479 7069 6e67 2e4d 6170 7069 6e67  l[typing.Mapping
+0000cd80: 5b73 7472 2c20 7374 725d 5d20 3d20 4e6f  [str, str]] = No
+0000cd90: 6e65 2c20 2a2a 6b77 6172 6773 293a 0a20  ne, **kwargs):. 
+0000cda0: 2020 2020 2020 2073 656c 662e 7461 6269         self.tabi
+0000cdb0: 6473 203d 2073 656c 662e 7461 6269 6473  ds = self.tabids
+0000cdc0: 206f 7220 7461 6269 6473 0a20 2020 2020   or tabids.     
+0000cdd0: 2020 2069 6620 7365 6c66 2e74 6162 6964     if self.tabid
+0000cde0: 7320 6973 204e 6f6e 653a 0a20 2020 2020  s is None:.     
+0000cdf0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+0000ce00: 7565 4572 726f 7228 277b 7365 6c66 2172  ueError('{self!r
+0000ce10: 7d3a 204d 6973 7369 6e67 2072 6571 7569  }: Missing requi
+0000ce20: 7265 6420 7461 6269 6473 2729 0a20 2020  red tabids').   
+0000ce30: 2020 2020 2073 7570 6572 2829 2e5f 5f69       super().__i
+0000ce40: 6e69 745f 5f28 2a61 7267 732c 202a 2a6b  nit__(*args, **k
+0000ce50: 7761 7267 7329 0a0a 2020 2020 6465 6620  wargs)..    def 
+0000ce60: 7365 7475 705f 7461 6273 2873 656c 662c  setup_tabs(self,
+0000ce70: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
+0000ce80: 2920 2d3e 2074 7970 696e 672e 4d61 7070  ) -> typing.Mapp
+0000ce90: 696e 675b 7374 722c 206d 6f64 656c 2e4e  ing[str, model.N
+0000cea0: 6f74 6562 6f6f 6b54 6162 5d3a 0a20 2020  otebookTab]:.   
+0000ceb0: 2020 2020 2027 2727 4465 6669 6e65 2074       '''Define t
+0000cec0: 6865 2073 7562 2074 6162 732c 2062 6173  he sub tabs, bas
+0000ced0: 6564 206f 6e20 7468 6520 636f 6d6d 6f6e  ed on the common
+0000cee0: 2074 6162 2e0a 0a20 2020 2020 2020 2044   tab...        D
+0000cef0: 6f20 6e6f 7420 6f76 6572 7772 6974 6520  o not overwrite 
+0000cf00: 7468 6973 2075 6e6c 6573 7320 796f 7520  this unless you 
+0000cf10: 6b6e 6f77 2077 6861 7420 796f 7520 6172  know what you ar
+0000cf20: 6520 646f 696e 672e 0a0a 2020 2020 2020  e doing...      
+0000cf30: 2020 546f 2065 6469 7420 7468 6520 636f    To edit the co
+0000cf40: 6d6d 6f6e 2074 6162 2c20 7365 6520 6073  mmon tab, see `s
+0000cf50: 6574 7570 5f74 6162 602e 0a20 2020 2020  etup_tab`..     
+0000cf60: 2020 2027 2727 0a20 2020 2020 2020 2061     '''.        a
+0000cf70: 7373 6572 7420 7365 6c66 2e74 6162 6964  ssert self.tabid
+0000cf80: 7320 6973 206e 6f74 204e 6f6e 650a 2020  s is not None.  
+0000cf90: 2020 2020 2020 7461 6273 203d 207b 7d0a        tabs = {}.
+0000cfa0: 2020 2020 2020 2020 666f 7220 7469 642c          for tid,
+0000cfb0: 2074 6e61 6d65 2069 6e20 7365 6c66 2e74   tname in self.t
+0000cfc0: 6162 6964 732e 6974 656d 7328 293a 0a20  abids.items():. 
+0000cfd0: 2020 2020 2020 2020 2020 2074 6162 735b             tabs[
+0000cfe0: 7469 645d 203d 204e 6f74 6562 6f6f 6b2e  tid] = Notebook.
+0000cff0: 5461 6228 746e 616d 652c 0a20 2020 2020  Tab(tname,.     
+0000d000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d020: 7365 6c66 2e73 6574 7570 5f74 6162 2874  self.setup_tab(t
+0000d030: 6964 2c20 746e 616d 6529 2c0a 2020 2020  id, tname),.    
+0000d040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d060: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
+0000d070: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0000d080: 2074 6162 730a 0a20 2020 2064 6566 2073   tabs..    def s
+0000d090: 6574 7570 5f74 6162 2873 656c 662c 2069  etup_tab(self, i
+0000d0a0: 6465 6e74 6966 6965 723a 2073 7472 2c20  dentifier: str, 
+0000d0b0: 6e61 6d65 3a20 7374 7229 202d 3e20 6d69  name: str) -> mi
+0000d0c0: 7869 6e2e 436f 6e74 6169 6e65 7257 6964  xin.ContainerWid
+0000d0d0: 6765 743a 0a20 2020 2020 2020 2027 2727  get:.        '''
+0000d0e0: 4465 6669 6e65 2074 6865 2063 6f6d 6d6f  Define the commo
+0000d0f0: 6e20 7461 6220 6043 6f6e 7461 696e 6572  n tab `Container
+0000d100: 5769 6467 6574 6020 6865 7265 2e0a 0a20  Widget` here... 
+0000d110: 2020 2020 2020 2053 696d 696c 6172 2074         Similar t
+0000d120: 6f20 6073 6574 7570 5f74 6162 7320 3c4e  o `setup_tabs <N
+0000d130: 6f74 6562 6f6f 6b2e 7365 7475 705f 7461  otebook.setup_ta
+0000d140: 6273 3e60 2c20 6275 7420 666f 7220 6120  bs>`, but for a 
+0000d150: 7369 6e67 6c65 2074 6162 2077 6964 6765  single tab widge
+0000d160: 742e 0a20 2020 2020 2020 2027 2727 0a20  t..        '''. 
+0000d170: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
+0000d180: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
+0000d190: 0a0a 0a63 6c61 7373 2054 7265 6528 7474  ...class Tree(tt
+0000d1a0: 6b2e 5472 6565 7669 6577 2c20 6d69 7869  k.Treeview, mixi
+0000d1b0: 6e2e 5369 6e67 6c65 5769 6467 6574 293a  n.SingleWidget):
+0000d1c0: 0a20 2020 2027 2727 4120 6869 6572 6172  .    '''A hierar
+0000d1d0: 6368 6963 616c 206d 756c 7469 636f 6c75  chical multicolu
+0000d1e0: 6d6e 2064 6174 6120 6469 7370 6c61 7920  mn data display 
+0000d1f0: 7769 6467 6574 2e0a 0a20 2020 2054 6869  widget...    Thi
+0000d200: 7320 7769 6467 6574 2069 7320 6361 7061  s widget is capa
+0000d210: 626c 6520 6f66 2073 686f 7769 6e67 2061  ble of showing a
+0000d220: 2068 6965 7261 7263 6879 206f 6620 6461   hierarchy of da
+0000d230: 7461 2072 6563 6f72 6473 2028 6f6e 6520  ta records (one 
+0000d240: 7065 720a 2020 2020 726f 7729 2e20 4561  per.    row). Ea
+0000d250: 6368 2072 6563 6f72 6420 6361 6e20 6861  ch record can ha
+0000d260: 7665 206d 756c 7469 706c 6520 636f 6c75  ve multiple colu
+0000d270: 6d6e 7320 6f66 2064 6174 612e 0a20 2020  mns of data..   
+0000d280: 2045 6163 6820 7265 636f 7264 2063 616e   Each record can
+0000d290: 2073 746f 7265 2061 7262 6974 7261 7279   store arbitrary
+0000d2a0: 2064 6174 6120 6f6e 2069 7473 2060 456c   data on its `El
+0000d2b0: 656d 656e 7420 3c6d 6f64 656c 2e54 7265  ement <model.Tre
+0000d2c0: 6545 6c65 6d65 6e74 3e60 2c0a 2020 2020  eElement>`,.    
+0000d2d0: 6578 706f 7365 6420 6f6e 2074 6865 2060  exposed on the `
+0000d2e0: 6f6e 5365 6c65 6374 6020 6675 6e63 7469  onSelect` functi
+0000d2f0: 6f6e 2e0a 0a20 2020 2053 6565 2060 5079  on...    See `Py
+0000d300: 7468 6f6e 2074 746b 2e54 7265 6576 6965  thon ttk.Treevie
+0000d310: 7720 3c74 6b69 6e74 6572 2e74 746b 2e54  w <tkinter.ttk.T
+0000d320: 7265 6576 6965 773e 6020 616e 6420 6060  reeview>` and ``
+0000d330: 546b 6060 0a20 2020 2060 7474 6b2e 5472  Tk``.    `ttk.Tr
+0000d340: 6565 7669 6577 203c 6874 7470 733a 2f2f  eeview <https://
+0000d350: 7463 6c2e 746b 2f6d 616e 2f74 636c 382e  tcl.tk/man/tcl8.
+0000d360: 362f 546b 436d 642f 7474 6b5f 7472 6565  6/TkCmd/ttk_tree
+0000d370: 7669 6577 2e68 746d 6c3e 605f 0a20 2020  view.html>`_.   
+0000d380: 2064 6f63 756d 656e 7461 7469 6f6e 2e0a   documentation..
+0000d390: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
+0000d3a0: 2020 2076 6172 6961 626c 653a 2055 7365     variable: Use
+0000d3b0: 2061 6e20 6578 7465 726e 616c 6c79 2064   an externally d
+0000d3c0: 6566 696e 6564 2076 6172 6961 626c 652c  efined variable,
+0000d3d0: 2069 6e73 7465 6164 206f 6620 6372 6561   instead of crea
+0000d3e0: 7469 6e67 2061 206e 6577 0a20 2020 2020  ting a new.     
+0000d3f0: 2020 2020 2020 206f 6e65 2073 7065 6369         one speci
+0000d400: 6669 6320 666f 7220 7468 6973 2077 6964  fic for this wid
+0000d410: 6765 742e 0a20 2020 2020 2020 206c 6162  get..        lab
+0000d420: 656c 3a20 5468 6520 6865 6164 696e 6720  el: The heading 
+0000d430: 7465 7874 2066 6f72 2074 6865 2066 6972  text for the fir
+0000d440: 7374 2063 6f6c 756d 6e2c 2077 6869 6368  st column, which
+0000d450: 2069 6e63 6c75 6465 7320 7468 6520 6c61   includes the la
+0000d460: 6265 6c73 2e0a 2020 2020 2020 2020 636f  bels..        co
+0000d470: 6c75 6d6e 733a 204d 6170 7069 6e67 2062  lumns: Mapping b
+0000d480: 6574 7765 656e 2063 6f6c 756d 6e20 6964  etween column id
+0000d490: 656e 7469 6669 6572 7320 616e 6420 6974  entifiers and it
+0000d4a0: 7320 7469 746c 6573 2e20 5375 7070 6f72  s titles. Suppor
+0000d4b0: 7473 0a20 2020 2020 2020 2020 2020 2061  ts.            a
+0000d4c0: 6c73 6f20 6120 6469 7265 6374 206d 6170  lso a direct map
+0000d4d0: 2062 6574 7765 656e 2069 6465 6e74 6966   between identif
+0000d4e0: 6965 7220 616e 6420 606d 6f64 656c 2e54  ier and `model.T
+0000d4f0: 7265 6543 6f6c 756d 6e60 2e0a 2020 2020  reeColumn`..    
+0000d500: 2020 2020 7365 6c65 6374 6162 6c65 3a20      selectable: 
+0000d510: 5368 6f75 6c64 2074 6865 2075 7365 7220  Should the user 
+0000d520: 6265 2061 626c 6520 746f 2073 656c 6563  be able to selec
+0000d530: 7420 6f6e 6520 6f66 2074 6865 2076 616c  t one of the val
+0000d540: 7565 733f 0a20 2020 2020 2020 2020 2020  ues?.           
+0000d550: 2044 6566 6175 6c74 7320 746f 2060 4661   Defaults to `Fa
+0000d560: 6c73 6560 2e0a 2020 2020 2020 2020 6f70  lse`..        op
+0000d570: 656e 6c65 7665 6c3a 2054 6865 2068 6965  enlevel: The hie
+0000d580: 7261 7263 6879 206c 6576 656c 2074 6f20  rarchy level to 
+0000d590: 6f70 656e 2074 6865 2065 6c65 6d65 6e74  open the element
+0000d5a0: 732e 2044 6566 6175 6c74 7320 746f 2060  s. Defaults to `
+0000d5b0: 6031 6060 2c0a 2020 2020 2020 2020 2020  `1``,.          
+0000d5c0: 2020 6f6e 6c79 2074 6865 2074 6f70 6c65    only the tople
+0000d5d0: 7665 6c20 656c 656d 656e 7473 2061 7265  vel elements are
+0000d5e0: 206f 7065 6e65 642e 0a20 2020 2020 2020   opened..       
+0000d5f0: 2020 2020 2053 6574 2074 6f20 6060 3060       Set to ``0`
+0000d600: 6020 746f 2063 6c6f 7365 2061 6c6c 2c20  ` to close all, 
+0000d610: 616e 6420 746f 2061 2072 6561 6c6c 7920  and to a really 
+0000d620: 6269 6720 6e75 6d62 6572 2074 6f20 6f70  big number to op
+0000d630: 656e 2061 6c6c 2e0a 2020 2020 2020 2020  en all..        
+0000d640: 6578 7061 6e64 3a20 4772 6f77 2074 6865  expand: Grow the
+0000d650: 2077 6964 6765 7420 746f 206d 6174 6368   widget to match
+0000d660: 2074 6865 2063 6f6e 7461 696e 6572 2067   the container g
+0000d670: 7269 6420 7369 7a65 2e20 5468 6973 2069  rid size. This i
+0000d680: 730a 2020 2020 2020 2020 2020 2020 7573  s.            us
+0000d690: 7561 6c6c 7920 7375 7070 6f72 7465 6420  ually supported 
+0000d6a0: 666f 7220 636f 6e74 6169 6e65 7273 2c20  for containers, 
+0000d6b0: 6275 7420 6974 2069 7320 696e 636c 7564  but it is includ
+0000d6c0: 6564 2068 6572 652e 0a20 2020 2020 2020  ed here..       
+0000d6d0: 2073 7479 6c65 3a20 436f 6e66 6967 7572   style: Configur
+0000d6e0: 6520 7468 6520 7769 6467 6574 2073 7479  e the widget sty
+0000d6f0: 6c65 2e0a 0a20 2020 2020 2020 2070 6172  le...        par
+0000d700: 656e 743a 2054 6865 2070 6172 656e 7420  ent: The parent 
+0000d710: 7769 6467 6574 2e20 4361 6e20 6265 2061  widget. Can be a
+0000d720: 2060 526f 6f74 5769 6e64 6f77 6020 6f72   `RootWindow` or
+0000d730: 2061 6e6f 7468 6572 2060 6d69 7869 6e2e   another `mixin.
+0000d740: 436f 6e74 6169 6e65 7257 6964 6765 7460  ContainerWidget`
+0000d750: 2e0a 0a20 2020 2053 6565 2041 6c73 6f3a  ...    See Also:
+0000d760: 0a20 2020 2020 2020 2060 4c69 7374 626f  .        `Listbo
+0000d770: 7860 3a20 5369 6d70 6c69 6669 6564 2076  x`: Simplified v
+0000d780: 6572 7369 6f6e 206f 6620 7468 6973 0a20  ersion of this. 
+0000d790: 2020 2027 2727 0a20 2020 2045 6c65 6d65     '''.    Eleme
+0000d7a0: 6e74 203d 206d 6f64 656c 2e54 7265 6545  nt = model.TreeE
+0000d7b0: 6c65 6d65 6e74 2020 2320 416c 6961 7320  lement  # Alias 
+0000d7c0: 7468 6520 7472 6565 2065 6c65 6d65 6e74  the tree element
+0000d7d0: 2069 6e66 6f72 6d61 7469 6f6e 2020 2320   information  # 
+0000d7e0: 544f 444f 3a20 4d6f 7665 2054 7265 6545  TODO: Move TreeE
+0000d7f0: 6c65 6d65 6e74 2063 6c61 7373 2068 6572  lement class her
+0000d800: 653f 0a0a 2020 2020 4064 6174 6163 6c61  e?..    @datacla
+0000d810: 7373 0a20 2020 2063 6c61 7373 2053 7479  ss.    class Sty
+0000d820: 6c65 286d 6f64 656c 2e57 5374 796c 6529  le(model.WStyle)
+0000d830: 3a0a 2020 2020 2020 2020 2727 2760 5472  :.        '''`Tr
+0000d840: 6565 6020 7374 796c 6520 6f62 6a65 6374  ee` style object
+0000d850: 2e0a 0a20 2020 2020 2020 2054 6865 7365  ...        These
+0000d860: 2061 7265 2074 6865 2073 7479 6c65 2063   are the style c
+0000d870: 6f6e 6669 6775 7261 7469 6f6e 733a 0a0a  onfigurations:..
+0000d880: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+0000d890: 2020 2020 2020 2020 2020 7368 6f77 5f68            show_h
+0000d8a0: 6561 6469 6e67 733a 2053 686f 7720 636f  eadings: Show co
+0000d8b0: 6c75 6d6e 2074 6974 6c65 2068 6561 6469  lumn title headi
+0000d8c0: 6e67 732e 0a20 2020 2020 2020 2020 2020  ngs..           
+0000d8d0: 2073 686f 775f 6c61 6265 6c73 3a20 5368   show_labels: Sh
+0000d8e0: 6f77 2074 6865 2066 6972 7374 2063 6f6c  ow the first col
+0000d8f0: 756d 6e2c 2077 6869 6368 2069 6e63 6c75  umn, which inclu
+0000d900: 6465 7320 7468 6520 6c61 6265 6c73 2e0a  des the labels..
+0000d910: 2020 2020 2020 2020 2020 2020 616c 7462              altb
+0000d920: 673a 2053 686f 7720 616c 7465 726e 6174  g: Show alternat
+0000d930: 6520 6261 636b 6772 6f75 6e64 7320 666f  e backgrounds fo
+0000d940: 7220 6561 6368 2072 6563 6f72 642e 0a20  r each record.. 
+0000d950: 2020 2020 2020 2020 2020 2061 6c74 6267             altbg
+0000d960: 5f73 696e 6465 783a 2060 6061 6c74 6267  _sindex: ``altbg
+0000d970: 6060 2069 6e69 7469 616c 2061 6c74 6572  `` initial alter
+0000d980: 6e61 7465 2063 6f6c 6f75 7220 696e 6465  nate colour inde
+0000d990: 782e 0a0a 2020 2020 2020 2020 5468 6573  x...        Thes
+0000d9a0: 6520 6172 6520 7468 6520 636f 6c6f 7572  e are the colour
+0000d9b0: 733a 0a0a 2020 2020 2020 2020 4172 6773  s:..        Args
+0000d9c0: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
+0000d9d0: 6c6f 7572 5f61 6c74 6267 3a20 6060 616c  lour_altbg: ``al
+0000d9e0: 7462 6760 6020 616c 7465 726e 6174 6520  tbg`` alternate 
+0000d9f0: 6c69 6e65 2063 6f6c 6f75 722e 0a20 2020  line colour..   
+0000da00: 2020 2020 2020 2020 2020 2020 2055 7365               Use
+0000da10: 6420 6173 2074 6865 2062 6163 6b67 726f  d as the backgro
+0000da20: 756e 6420 636f 6c6f 7572 2e0a 2020 2020  und colour..    
+0000da30: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+0000da40: 7368 6f77 5f68 6561 6469 6e67 733a 2062  show_headings: b
+0000da50: 6f6f 6c20 3d20 5472 7565 0a20 2020 2020  ool = True.     
+0000da60: 2020 2073 686f 775f 6c61 6265 6c73 3a20     show_labels: 
+0000da70: 626f 6f6c 203d 2054 7275 650a 2020 2020  bool = True.    
+0000da80: 2020 2020 616c 7462 673a 2062 6f6f 6c20      altbg: bool 
+0000da90: 3d20 5472 7565 0a20 2020 2020 2020 2061  = True.        a
+0000daa0: 6c74 6267 5f73 696e 6465 783a 2074 7970  ltbg_sindex: typ
+0000dab0: 696e 672e 4c69 7465 7261 6c5b 302c 2031  ing.Literal[0, 1
+0000dac0: 5d20 3d20 310a 2020 2020 2020 2020 2320  ] = 1.        # 
+0000dad0: 436f 6c6f 7572 730a 2020 2020 2020 2020  Colours.        
+0000dae0: 636f 6c6f 7572 5f61 6c74 6267 3a20 7374  colour_altbg: st
+0000daf0: 7220 3d20 276c 6967 6874 6772 6579 270a  r = 'lightgrey'.
+0000db00: 0a20 2020 2073 7461 7465 5f74 7970 6520  .    state_type 
+0000db10: 3d20 7661 7254 7265 650a 2020 2020 5f5f  = varTree.    __
+0000db20: 6c69 6e65 735f 616c 743a 2073 7472 203d  lines_alt: str =
+0000db30: 2027 5f5f 3a6c 696e 6573 2d61 6c74 270a   '__:lines-alt'.
+0000db40: 0a20 2020 2077 636f 6c75 6d6e 733a 2074  .    wcolumns: t
+0000db50: 7970 696e 672e 4d61 7070 696e 675b 7374  yping.Mapping[st
+0000db60: 722c 206d 6f64 656c 2e54 7265 6543 6f6c  r, model.TreeCol
+0000db70: 756d 6e5d 0a20 2020 2077 6461 7461 3a20  umn].    wdata: 
+0000db80: 7479 7069 6e67 2e4d 7574 6162 6c65 4d61  typing.MutableMa
+0000db90: 7070 696e 675b 7374 722c 2074 7970 696e  pping[str, typin
+0000dba0: 672e 416e 795d 0a0a 2020 2020 6465 6620  g.Any]..    def 
+0000dbb0: 5f5f 696e 6974 5f5f 2873 656c 662c 2070  __init__(self, p
+0000dbc0: 6172 656e 742c 202a 2c20 7661 7269 6162  arent, *, variab
+0000dbd0: 6c65 3a20 7479 7069 6e67 2e4f 7074 696f  le: typing.Optio
+0000dbe0: 6e61 6c5b 7661 7254 7265 655d 203d 204e  nal[varTree] = N
+0000dbf0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+0000dc00: 2020 2020 2020 6c61 6265 6c3a 2074 7970        label: typ
+0000dc10: 696e 672e 4f70 7469 6f6e 616c 5b73 7472  ing.Optional[str
+0000dc20: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+0000dc30: 2020 2020 636f 6c75 6d6e 733a 2074 7970      columns: typ
+0000dc40: 696e 672e 4d61 7070 696e 675b 7374 722c  ing.Mapping[str,
+0000dc50: 2074 7970 696e 672e 556e 696f 6e5b 6d6f   typing.Union[mo
+0000dc60: 6465 6c2e 5472 6565 436f 6c75 6d6e 2c20  del.TreeColumn, 
+0000dc70: 7374 725d 5d2c 0a20 2020 2020 2020 2020  str]],.         
+0000dc80: 2020 2020 2020 2020 7365 6c65 6374 6162          selectab
+0000dc90: 6c65 3a20 626f 6f6c 203d 2046 616c 7365  le: bool = False
+0000dca0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000dcb0: 2020 206f 7065 6e6c 6576 656c 3a20 696e     openlevel: in
+0000dcc0: 7420 3d20 312c 0a20 2020 2020 2020 2020  t = 1,.         
+0000dcd0: 2020 2020 2020 2020 6578 7061 6e64 3a20          expand: 
+0000dce0: 626f 6f6c 203d 2054 7275 652c 0a20 2020  bool = True,.   
+0000dcf0: 2020 2020 2020 2020 2020 2020 2020 7374                st
+0000dd00: 796c 653a 2053 7479 6c65 203d 2053 7479  yle: Style = Sty
+0000dd10: 6c65 285f 6465 6661 756c 743d 5472 7565  le(_default=True
+0000dd20: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0000dd30: 2020 2020 2a2a 6b77 6172 6773 293a 0a20      **kwargs):. 
+0000dd40: 2020 2020 2020 2073 656c 662e 7773 7479         self.wsty
+0000dd50: 6c65 203d 2073 7479 6c65 0a20 2020 2020  le = style.     
+0000dd60: 2020 2023 2054 4f44 4f3a 2053 7570 706f     # TODO: Suppo
+0000dd70: 7274 3a0a 2020 2020 2020 2020 2320 2d20  rt:.        # - 
+0000dd80: 5365 7475 7020 7769 6467 6574 2063 6f6c  Setup widget col
+0000dd90: 756d 6e20 7365 7474 696e 6773 3f20 5365  umn settings? Se
+0000dda0: 6520 4c69 7374 626f 780a 2020 2020 2020  e Listbox.      
+0000ddb0: 2020 7763 6f6c 756d 6e73 203d 207b 7d0a    wcolumns = {}.
+0000ddc0: 2020 2020 2020 2020 666f 7220 6369 642c          for cid,
+0000ddd0: 2063 6f62 6a20 696e 2063 6f6c 756d 6e73   cobj in columns
+0000dde0: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
+0000ddf0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+0000de00: 6e63 6528 636f 626a 2c20 6d6f 6465 6c2e  nce(cobj, model.
+0000de10: 5472 6565 436f 6c75 6d6e 293a 0a20 2020  TreeColumn):.   
+0000de20: 2020 2020 2020 2020 2020 2020 2063 636f               cco
+0000de30: 6c20 3d20 636f 626a 0a20 2020 2020 2020  l = cobj.       
+0000de40: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
+0000de50: 616e 6365 2863 6f62 6a2c 2073 7472 293a  ance(cobj, str):
+0000de60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000de70: 2063 636f 6c20 3d20 6d6f 6465 6c2e 5472   ccol = model.Tr
+0000de80: 6565 436f 6c75 6d6e 2863 6964 2c20 6e61  eeColumn(cid, na
+0000de90: 6d65 3d63 6f62 6a29 0a20 2020 2020 2020  me=cobj).       
+0000dea0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000deb0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0000dec0: 2056 616c 7565 4572 726f 7228 6627 7b73   ValueError(f'{s
+0000ded0: 656c 6621 727d 3a20 496e 7661 6c69 6420  elf!r}: Invalid 
+0000dee0: 636f 6c75 6d6e 2022 7b63 6964 7d22 3a20  column "{cid}": 
+0000def0: 7b63 6f62 6a21 727d 2729 0a20 2020 2020  {cobj!r}').     
+0000df00: 2020 2020 2020 2077 636f 6c75 6d6e 735b         wcolumns[
+0000df10: 6369 645d 203d 2063 636f 6c0a 2020 2020  cid] = ccol.    
+0000df20: 2020 2020 7365 6c66 2e77 636f 6c75 6d6e      self.wcolumn
+0000df30: 7320 3d20 7763 6f6c 756d 6e73 0a20 2020  s = wcolumns.   
+0000df40: 2020 2020 2077 7368 6f77 203d 205b 5d0a       wshow = [].
+0000df50: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000df60: 7773 7479 6c65 2e73 686f 775f 6865 6164  wstyle.show_head
+0000df70: 696e 6773 3a0a 2020 2020 2020 2020 2020  ings:.          
+0000df80: 2020 7773 686f 772e 6170 7065 6e64 2827    wshow.append('
+0000df90: 6865 6164 696e 6773 2729 0a20 2020 2020  headings').     
+0000dfa0: 2020 2069 6620 7365 6c66 2e77 7374 796c     if self.wstyl
+0000dfb0: 652e 7368 6f77 5f6c 6162 656c 733a 0a20  e.show_labels:. 
+0000dfc0: 2020 2020 2020 2020 2020 2077 7368 6f77             wshow
+0000dfd0: 2e61 7070 656e 6428 2774 7265 6527 290a  .append('tree').
+0000dfe0: 2020 2020 2020 2020 2320 496e 6974 6961          # Initia
+0000dff0: 6c69 7365 2056 6172 6961 626c 6520 616e  lise Variable an
+0000e000: 6420 4461 7461 0a20 2020 2020 2020 2073  d Data.        s
+0000e010: 656c 662e 696e 6974 5f73 696e 676c 6528  elf.init_single(
+0000e020: 7661 7269 6162 6c65 290a 2020 2020 2020  variable).      
+0000e030: 2020 6b77 6172 6773 2e75 7064 6174 6528    kwargs.update(
+0000e040: 7b0a 2020 2020 2020 2020 2020 2020 2773  {.            's
+0000e050: 686f 7727 3a20 7773 686f 772c 2020 2320  how': wshow,  # 
+0000e060: 4f76 6572 7269 6465 2074 6865 2067 6976  Override the giv
+0000e070: 656e 2060 7368 6f77 6020 6172 6775 6d65  en `show` argume
+0000e080: 6e74 0a20 2020 2020 2020 2020 2020 2027  nt.            '
+0000e090: 7365 6c65 6374 6d6f 6465 273a 2074 6b2e  selectmode': tk.
+0000e0a0: 4252 4f57 5345 2069 6620 7365 6c65 6374  BROWSE if select
+0000e0b0: 6162 6c65 2065 6c73 6520 746b 2e4e 4f4e  able else tk.NON
+0000e0c0: 452c 0a20 2020 2020 2020 2020 2020 2027  E,.            '
+0000e0d0: 636f 6c75 6d6e 7327 3a20 6c69 7374 2873  columns': list(s
+0000e0e0: 656c 662e 7763 6f6c 756d 6e73 2e6b 6579  elf.wcolumns.key
+0000e0f0: 7328 2929 2c0a 2020 2020 2020 2020 7d29  s()),.        })
+0000e100: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
+0000e110: 2e5f 5f69 6e69 745f 5f28 7061 7265 6e74  .__init__(parent
+0000e120: 2c20 2a2a 6b77 6172 6773 290a 2020 2020  , **kwargs).    
+0000e130: 2020 2020 7365 6c66 2e77 6461 7461 203d      self.wdata =
+0000e140: 207b 7d0a 2020 2020 2020 2020 2320 5365   {}.        # Se
+0000e150: 6c65 6374 696f 6e0a 2020 2020 2020 2020  lection.        
+0000e160: 6966 2073 656c 6563 7461 626c 653a 0a20  if selectable:. 
+0000e170: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000e180: 6269 6e64 696e 6728 273c 3c54 7265 6576  binding('<<Treev
+0000e190: 6965 7753 656c 6563 743e 3e27 2c20 7365  iewSelect>>', se
+0000e1a0: 6c66 2e5f 6f6e 5365 6c65 6374 290a 2020  lf._onSelect).  
+0000e1b0: 2020 2020 2020 2020 2020 2320 4469 7361            # Disa
+0000e1c0: 626c 6520 446f 7562 6c65 2d43 6c69 636b  ble Double-Click
+0000e1d0: 2065 7665 6e74 2c20 7768 656e 2073 656c   event, when sel
+0000e1e0: 6563 7461 626c 650a 2020 2020 2020 2020  ectable.        
+0000e1f0: 2020 2020 7365 6c66 2e62 696e 6469 6e67      self.binding
+0000e200: 2827 3c44 6f75 626c 652d 4275 7474 6f6e  ('<Double-Button
+0000e210: 2d31 3e27 2c20 666e 2e62 696e 6469 6e67  -1>', fn.binding
+0000e220: 5f64 6973 6162 6c65 290a 2020 2020 2020  _disable).      
+0000e230: 2020 2320 4170 7065 6172 616e 6365 0a20    # Appearance. 
+0000e240: 2020 2020 2020 2069 6620 6578 7061 6e64         if expand
+0000e250: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000e260: 6c66 2e67 7269 6428 7374 6963 6b79 3d74  lf.grid(sticky=t
+0000e270: 6b2e 4e53 4557 290a 2020 2020 2020 2020  k.NSEW).        
+0000e280: 7365 6c66 2e6f 7065 6e6c 6576 656c 3a20  self.openlevel: 
+0000e290: 696e 7420 3d20 6f70 656e 6c65 7665 6c20  int = openlevel 
+0000e2a0: 2023 2054 4f44 4f3a 2053 7570 706f 7274   # TODO: Support
+0000e2b0: 206f 7065 6e69 6e67 2061 6c6c 206c 6576   opening all lev
+0000e2c0: 656c 732c 2065 7870 6c69 6369 743f 0a20  els, explicit?. 
+0000e2d0: 2020 2020 2020 2023 2023 2048 6561 6465         # # Heade
+0000e2e0: 7273 0a20 2020 2020 2020 2069 6620 6c61  rs.        if la
+0000e2f0: 6265 6c20 6973 206e 6f74 204e 6f6e 653a  bel is not None:
+0000e300: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000e310: 662e 6865 6164 696e 6728 2723 3027 2c20  f.heading('#0', 
+0000e320: 7465 7874 3d6c 6162 656c 290a 2020 2020  text=label).    
+0000e330: 2020 2020 666f 7220 7763 6f6c 2069 6e20      for wcol in 
+0000e340: 7365 6c66 2e77 636f 6c75 6d6e 732e 7661  self.wcolumns.va
+0000e350: 6c75 6573 2829 3a0a 2020 2020 2020 2020  lues():.        
+0000e360: 2020 2020 7365 6c66 2e68 6561 6469 6e67      self.heading
+0000e370: 2877 636f 6c2e 6964 656e 7469 6669 6572  (wcol.identifier
+0000e380: 2c20 7465 7874 3d77 636f 6c2e 6e61 6d65  , text=wcol.name
+0000e390: 290a 2020 2020 2020 2020 2320 2320 416c  ).        # # Al
+0000e3a0: 7465 726e 6174 6520 4261 636b 6772 6f75  ternate Backgrou
+0000e3b0: 6e64 730a 2020 2020 2020 2020 6966 2073  nds.        if s
+0000e3c0: 656c 662e 7773 7479 6c65 2e61 6c74 6267  elf.wstyle.altbg
+0000e3d0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000e3e0: 6c66 2e74 6167 5f63 6f6e 6669 6775 7265  lf.tag_configure
+0000e3f0: 2854 7265 652e 5f5f 6c69 6e65 735f 616c  (Tree.__lines_al
+0000e400: 742c 2062 6163 6b67 726f 756e 643d 7365  t, background=se
+0000e410: 6c66 2e77 7374 796c 652e 636f 6c6f 7572  lf.wstyle.colour
+0000e420: 5f61 6c74 6267 290a 2020 2020 2020 2020  _altbg).        
+0000e430: 2020 2020 2320 4d69 6e6f 7220 6973 7375      # Minor issu
+0000e440: 653a 2054 6865 7265 2069 7320 6120 6e65  e: There is a ne
+0000e450: 6172 6c79 2069 6d70 6572 6365 7469 626c  arly impercetibl
+0000e460: 6520 666c 6173 6820 6f66 2062 6164 6e65  e flash of badne
+0000e470: 7373 2077 6974 680a 2020 2020 2020 2020  ss with.        
+0000e480: 2020 2020 2320 6054 696d 656f 7574 4964      # `TimeoutId
+0000e490: 6c65 6020 7468 6174 2064 6f65 736e 2774  le` that doesn't
+0000e4a0: 2068 6170 7065 6e20 7768 656e 2063 616c   happen when cal
+0000e4b0: 6c69 6e67 2074 6865 2066 756e 6374 696f  ling the functio
+0000e4c0: 6e0a 2020 2020 2020 2020 2020 2020 2320  n.            # 
+0000e4d0: 6469 7265 6374 6c79 2e0a 2020 2020 2020  directly..      
+0000e4e0: 2020 2020 2020 2320 506f 7373 6962 6c65        # Possible
+0000e4f0: 2066 6978 3a20 696e 2060 5f5f 7472 6565   fix: in `__tree
+0000e500: 5f6c 7376 6973 6962 6c65 602c 2070 6173  _lsvisible`, pas
+0000e510: 7320 616e 206f 7074 696f 6e61 6c0a 2020  s an optional.  
+0000e520: 2020 2020 2020 2020 2020 2320 6073 656c            # `sel
+0000e530: 662e 666f 6375 7328 2960 2049 4420 2877  f.focus()` ID (w
+0000e540: 6865 6e20 213d 2027 2729 2061 6e64 206f  hen != '') and o
+0000e550: 7065 6e2f 636c 6f73 6520 7374 6174 652c  pen/close state,
+0000e560: 2074 6861 740a 2020 2020 2020 2020 2020   that.          
+0000e570: 2020 2320 7265 706c 6163 6573 2060 776f    # replaces `wo
+0000e580: 7065 6e60 2e0a 2020 2020 2020 2020 2020  pen`..          
+0000e590: 2020 616c 7462 6720 3d20 7365 6c66 2e74    altbg = self.t
+0000e5a0: 6964 6c65 2873 656c 662e 5f5f 7472 6565  idle(self.__tree
+0000e5b0: 5f61 6c74 6267 2c20 6b65 793d 2761 6c74  _altbg, key='alt
+0000e5c0: 6267 2729 0a20 2020 2020 2020 2020 2020  bg').           
+0000e5d0: 2073 656c 662e 6269 6e64 696e 6728 273c   self.binding('<
+0000e5e0: 3c54 7265 6576 6965 774f 7065 6e3e 3e27  <TreeviewOpen>>'
+0000e5f0: 2c20 616c 7462 672e 7265 7363 6865 6475  , altbg.reschedu
+0000e600: 6c65 290a 2020 2020 2020 2020 2020 2020  le).            
+0000e610: 7365 6c66 2e62 696e 6469 6e67 2827 3c3c  self.binding('<<
+0000e620: 5472 6565 7669 6577 436c 6f73 653e 3e27  TreeviewClose>>'
+0000e630: 2c20 616c 7462 672e 7265 7363 6865 6475  , altbg.reschedu
+0000e640: 6c65 290a 2020 2020 2020 2020 2320 5472  le).        # Tr
+0000e650: 6163 6520 7661 7269 6162 6c65 2073 7461  ace variable sta
+0000e660: 7465 0a20 2020 2020 2020 2073 656c 662e  te.        self.
+0000e670: 5f5f 6775 695f 6368 616e 6765 643a 2062  __gui_changed: b
+0000e680: 6f6f 6c20 3d20 4661 6c73 6520 2023 204d  ool = False  # M
+0000e690: 6172 6b20 7468 6520 4755 4920 6173 2063  ark the GUI as c
+0000e6a0: 6861 6e67 6564 2061 6c72 6561 6479 0a20  hanged already. 
+0000e6b0: 2020 2020 2020 2073 656c 662e 7472 6163         self.trac
+0000e6c0: 6528 7365 6c66 2e5f 5f74 7265 655f 7365  e(self.__tree_se
+0000e6d0: 742c 2074 7261 6365 5f6e 616d 653d 6627  t, trace_name=f'
+0000e6e0: 5f5f 3a7b 5f5f 6e61 6d65 5f5f 7d27 290a  __:{__name__}').
+0000e6f0: 0a20 2020 2064 6566 205f 7472 6565 5f67  .    def _tree_g
+0000e700: 6574 2873 656c 662c 2076 6172 6961 626c  et(self, variabl
+0000e710: 653a 2076 6172 2e56 6172 6961 626c 6529  e: var.Variable)
+0000e720: 202d 3e20 7479 7069 6e67 2e53 6571 7565   -> typing.Seque
+0000e730: 6e63 655b 6d6f 6465 6c2e 5472 6565 456c  nce[model.TreeEl
+0000e740: 656d 656e 745d 3a0a 2020 2020 2020 2020  ement]:.        
+0000e750: 2727 2747 656e 6572 6174 6520 6120 6076  '''Generate a `v
+0000e760: 6172 5472 6565 6020 6f62 6a65 6374 2c20  arTree` object, 
+0000e770: 6261 7365 6420 6f6e 2074 6865 2076 6172  based on the var
+0000e780: 6961 626c 652e 0a0a 2020 2020 2020 2020  iable...        
+0000e790: 5368 6f75 6c64 2062 6520 7265 696d 706c  Should be reimpl
+0000e7a0: 656d 656e 7465 6420 6279 2073 7562 636c  emented by subcl
+0000e7b0: 6173 7365 7320 7468 6174 2063 6861 6e67  asses that chang
+0000e7c0: 6520 7468 6520 7661 7269 6162 6c65 2074  e the variable t
+0000e7d0: 7970 652e 0a20 2020 2020 2020 2027 2727  ype..        '''
+0000e7e0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+0000e7f0: 6973 696e 7374 616e 6365 2876 6172 6961  isinstance(varia
+0000e800: 626c 652c 2076 6172 5472 6565 290a 2020  ble, varTree).  
+0000e810: 2020 2020 2020 7265 7475 726e 2076 6172        return var
+0000e820: 6961 626c 652e 6765 7428 290a 0a20 2020  iable.get()..   
+0000e830: 2064 6566 205f 5f74 7265 655f 6c73 2873   def __tree_ls(s
+0000e840: 656c 662c 2070 6172 656e 743a 2074 7970  elf, parent: typ
+0000e850: 696e 672e 4f70 7469 6f6e 616c 5b73 7472  ing.Optional[str
+0000e860: 5d20 3d20 4e6f 6e65 2920 2d3e 2074 7970  ] = None) -> typ
+0000e870: 696e 672e 4974 6572 6162 6c65 5b73 7472  ing.Iterable[str
+0000e880: 5d3a 0a20 2020 2020 2020 2027 2727 4765  ]:.        '''Ge
+0000e890: 6e65 7261 7465 2061 206c 6973 7420 616c  nerate a list al
+0000e8a0: 6c20 7769 6467 6574 2069 6473 2c20 696e  l widget ids, in
+0000e8b0: 206c 696e 6561 7220 6f72 6465 722e 2727   linear order.''
+0000e8c0: 270a 2020 2020 2020 2020 666f 7220 7774  '.        for wt
+0000e8d0: 6f70 2069 6e20 7365 6c66 2e67 6574 5f63  op in self.get_c
+0000e8e0: 6869 6c64 7265 6e28 6974 656d 3d70 6172  hildren(item=par
+0000e8f0: 656e 7429 3a0a 2020 2020 2020 2020 2020  ent):.          
+0000e900: 2020 7969 656c 6420 7774 6f70 0a20 2020    yield wtop.   
+0000e910: 2020 2020 2020 2020 2079 6965 6c64 2066           yield f
+0000e920: 726f 6d20 7365 6c66 2e5f 5f74 7265 655f  rom self.__tree_
+0000e930: 6c73 2870 6172 656e 743d 7774 6f70 290a  ls(parent=wtop).
+0000e940: 0a20 2020 2064 6566 205f 5f74 7265 655f  .    def __tree_
+0000e950: 6c73 7669 7369 626c 6528 7365 6c66 2c20  lsvisible(self, 
+0000e960: 7061 7265 6e74 3a20 7479 7069 6e67 2e4f  parent: typing.O
+0000e970: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+0000e980: 6f6e 652c 205f 6b69 6473 3d4e 6f6e 6529  one, _kids=None)
+0000e990: 202d 3e20 7479 7069 6e67 2e49 7465 7261   -> typing.Itera
+0000e9a0: 626c 655b 7374 725d 3a0a 2020 2020 2020  ble[str]:.      
+0000e9b0: 2020 2727 2747 656e 6572 6174 6520 6120    '''Generate a 
+0000e9c0: 6c69 7374 206f 6620 616c 6c20 7669 7369  list of all visi
+0000e9d0: 626c 6520 7769 6467 6574 2069 6473 2c20  ble widget ids, 
+0000e9e0: 696e 2047 5549 206f 7264 6572 2e0a 0a20  in GUI order... 
+0000e9f0: 2020 2020 2020 2054 6869 7320 6775 6172         This guar
+0000ea00: 616e 7465 6573 2074 6865 2079 6965 6c64  antees the yield
+0000ea10: 6564 2076 616c 7565 7320 6172 6520 7669  ed values are vi
+0000ea20: 7369 626c 6520 746f 2074 6865 2075 7365  sible to the use
+0000ea30: 722c 2061 7320 6c6f 6e67 2061 730a 2020  r, as long as.  
+0000ea40: 2020 2020 2020 7468 6520 7472 6565 2069        the tree i
+0000ea50: 7320 7374 6162 6c65 2e0a 0a20 2020 2020  s stable...     
+0000ea60: 2020 2053 6565 2041 6c73 6f3a 0a20 2020     See Also:.   
+0000ea70: 2020 2020 2020 2020 2060 5f5f 7472 6565           `__tree
+0000ea80: 5f6c 7360 3a20 5368 6f77 2061 6c6c 2077  _ls`: Show all w
+0000ea90: 6964 6765 7473 2c20 6576 656e 2074 6865  idgets, even the
+0000eaa0: 206e 6f74 2063 7572 7265 6e74 6c79 2073   not currently s
+0000eab0: 686f 776e 2e0a 0a20 2020 2020 2020 204e  hown...        N
+0000eac0: 6f74 653a 0a20 2020 2020 2020 2020 2020  ote:.           
+0000ead0: 2057 6865 6e20 6361 6c6c 6564 2064 6972   When called dir
+0000eae0: 6563 746c 7920 6672 6f6d 2074 6865 2060  ectly from the `
+0000eaf0: 603c 3c54 7265 6576 6965 774f 7065 6e3e  `<<TreeviewOpen>
+0000eb00: 3e60 6020 6f72 0a20 2020 2020 2020 2020  >`` or.         
+0000eb10: 2020 2060 603c 3c54 7265 6576 6965 7743     ``<<TreeviewC
+0000eb20: 6c6f 7365 3e3e 6060 2065 7665 6e74 2c20  lose>>`` event, 
+0000eb30: 7468 6973 2077 696c 6c20 2266 6169 6c22  this will "fail"
+0000eb40: 2c20 7468 6174 2065 7665 6e74 2072 756e  , that event run
+0000eb50: 7320 746f 6f0a 2020 2020 2020 2020 2020  s too.          
+0000eb60: 2020 6561 726c 792e 2055 7365 2061 2060    early. Use a `
+0000eb70: 6d6f 6465 6c2e 5469 6d65 6f75 7449 646c  model.TimeoutIdl
+0000eb80: 6560 2069 6e20 7468 6572 6520 746f 2067  e` in there to g
+0000eb90: 6574 2074 6865 2063 6f72 7265 6374 0a20  et the correct. 
+0000eba0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0000ebb0: 7473 2e0a 2020 2020 2020 2020 2727 270a  ts..        '''.
+0000ebc0: 2020 2020 2020 2020 666f 7220 7774 6f70          for wtop
+0000ebd0: 2069 6e20 5f6b 6964 7320 6f72 2073 656c   in _kids or sel
+0000ebe0: 662e 6765 745f 6368 696c 6472 656e 2869  f.get_children(i
+0000ebf0: 7465 6d3d 7061 7265 6e74 293a 0a20 2020  tem=parent):.   
+0000ec00: 2020 2020 2020 2020 2079 6965 6c64 2077           yield w
+0000ec10: 746f 700a 2020 2020 2020 2020 2020 2020  top.            
+0000ec20: 776f 7065 6e20 3d20 7365 6c66 2e69 7465  wopen = self.ite
+0000ec30: 6d28 7774 6f70 2c20 6f70 7469 6f6e 3d27  m(wtop, option='
+0000ec40: 6f70 656e 2729 203d 3d20 310a 2020 2020  open') == 1.    
+0000ec50: 2020 2020 2020 2020 776b 6964 7320 3d20          wkids = 
+0000ec60: 7365 6c66 2e67 6574 5f63 6869 6c64 7265  self.get_childre
+0000ec70: 6e28 6974 656d 3d77 746f 7029 0a20 2020  n(item=wtop).   
+0000ec80: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
+0000ec90: 776b 6964 7329 203e 2030 2061 6e64 2077  wkids) > 0 and w
+0000eca0: 6f70 656e 3a0a 2020 2020 2020 2020 2020  open:.          
+0000ecb0: 2020 2020 2020 7969 656c 6420 6672 6f6d        yield from
+0000ecc0: 2073 656c 662e 5f5f 7472 6565 5f6c 7376   self.__tree_lsv
+0000ecd0: 6973 6962 6c65 2870 6172 656e 743d 7774  isible(parent=wt
+0000ece0: 6f70 2c20 5f6b 6964 733d 776b 6964 7329  op, _kids=wkids)
+0000ecf0: 0a0a 2020 2020 6465 6620 5f5f 7472 6565  ..    def __tree
+0000ed00: 5f63 6c65 616e 2873 656c 662c 2070 6172  _clean(self, par
+0000ed10: 656e 743d 4e6f 6e65 2920 2d3e 204e 6f6e  ent=None) -> Non
+0000ed20: 653a 0a20 2020 2020 2020 2073 656c 662e  e:.        self.
+0000ed30: 6465 6c65 7465 282a 7365 6c66 2e5f 5f74  delete(*self.__t
+0000ed40: 7265 655f 6c73 2870 6172 656e 743d 7061  ree_ls(parent=pa
+0000ed50: 7265 6e74 2929 0a20 2020 2020 2020 2073  rent)).        s
+0000ed60: 656c 662e 7764 6174 612e 636c 6561 7228  elf.wdata.clear(
+0000ed70: 290a 0a20 2020 2064 6566 205f 5f74 7265  )..    def __tre
+0000ed80: 655f 7075 7428 7365 6c66 2c20 656c 656d  e_put(self, elem
+0000ed90: 656e 7473 3a20 7479 7069 6e67 2e53 6571  ents: typing.Seq
+0000eda0: 7565 6e63 655b 6d6f 6465 6c2e 5472 6565  uence[model.Tree
+0000edb0: 456c 656d 656e 745d 2c20 2a2c 0a20 2020  Element], *,.   
+0000edc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000edd0: 7061 7265 6e74 3a20 7479 7069 6e67 2e4f  parent: typing.O
+0000ede0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+0000edf0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+0000ee00: 2020 2020 2020 2020 6f70 656e 6c65 7665          openleve
+0000ee10: 6c3a 2074 7970 696e 672e 4f70 7469 6f6e  l: typing.Option
+0000ee20: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 2c20  al[int] = None, 
+0000ee30: 5f6c 6576 656c 3a20 696e 7420 3d20 3029  _level: int = 0)
+0000ee40: 3a0a 2020 2020 2020 2020 7061 7265 6e74  :.        parent
+0000ee50: 5f6c 6f63 3a20 7479 7069 6e67 2e4f 7074  _loc: typing.Opt
+0000ee60: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+0000ee70: 6520 6966 2070 6172 656e 7420 6973 204e  e if parent is N
+0000ee80: 6f6e 6520 656c 7365 2073 656c 662e 696e  one else self.in
+0000ee90: 6465 7828 7061 7265 6e74 290a 2020 2020  dex(parent).    
+0000eea0: 2020 2020 6f70 656e 6c65 7665 6c20 3d20      openlevel = 
+0000eeb0: 6f70 656e 6c65 7665 6c20 6f72 2073 656c  openlevel or sel
+0000eec0: 662e 6f70 656e 6c65 7665 6c0a 2020 2020  f.openlevel.    
+0000eed0: 2020 2020 666f 7220 6569 642c 2065 6c65      for eid, ele
+0000eee0: 6d65 6e74 2069 6e20 656e 756d 6572 6174  ment in enumerat
+0000eef0: 6528 656c 656d 656e 7473 293a 0a20 2020  e(elements):.   
+0000ef00: 2020 2020 2020 2020 2023 2069 6620 5f5f           # if __
+0000ef10: 6465 6275 675f 5f3a 0a20 2020 2020 2020  debug__:.       
+0000ef20: 2020 2020 2023 2020 2020 2074 706c 5f74       #     tpl_t
+0000ef30: 6578 7420 3d20 6627 7b70 6172 656e 7420  ext = f'{parent 
+0000ef40: 6f72 2022 5f5f 746f 705f 5f22 7d3a 3a23  or "__top__"}::#
+0000ef50: 7b65 6964 7d27 0a20 2020 2020 2020 2020  {eid}'.         
+0000ef60: 2020 2023 2020 2020 206c 6f67 6765 722e     #     logger.
+0000ef70: 6465 6275 6728 6627 7b22 3e22 202a 2028  debug(f'{">" * (
+0000ef80: 5f6c 6576 656c 202b 2031 297d 207b 7470  _level + 1)} {tp
+0000ef90: 6c5f 7465 7874 7d3a 204c 3a22 7b65 6c65  l_text}: L:"{ele
+0000efa0: 6d65 6e74 2e6c 6162 656c 7d22 2043 3a7c  ment.label}" C:|
+0000efb0: 7b22 2022 2e6a 6f69 6e28 656c 656d 656e  {" ".join(elemen
+0000efc0: 742e 636f 6c75 6d6e 7329 7d7c 2729 0a20  t.columns)}|'). 
+0000efd0: 2020 2020 2020 2020 2020 2069 6620 656c             if el
+0000efe0: 656d 656e 742e 636f 6c75 6d6e 7320 6973  ement.columns is
+0000eff0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000f000: 2020 2020 2020 2020 2020 2023 2054 4f44             # TOD
+0000f010: 4f3a 2053 7570 706f 7274 2061 2064 6963  O: Support a dic
+0000f020: 7420 7769 7468 206b 6579 7320 636f 7272  t with keys corr
+0000f030: 6573 706f 6e64 696e 6720 746f 2074 6865  esponding to the
+0000f040: 2060 7365 6c66 2e77 636f 6c75 6d6e 7360   `self.wcolumns`
+0000f050: 2c20 706f 7373 6962 6c65 2073 7562 7365  , possible subse
+0000f060: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+0000f070: 2020 6173 7365 7274 206c 656e 2865 6c65    assert len(ele
+0000f080: 6d65 6e74 2e63 6f6c 756d 6e73 2920 3d3d  ment.columns) ==
+0000f090: 206c 656e 2873 656c 662e 7763 6f6c 756d   len(self.wcolum
+0000f0a0: 6e73 292c 2066 2749 6e76 616c 6964 2043  ns), f'Invalid C
+0000f0b0: 6f6c 756d 6e20 237b 6569 647d 3a20 5369  olumn #{eid}: Si
+0000f0c0: 7a65 3a20 457b 6c65 6e28 656c 656d 656e  ze: E{len(elemen
+0000f0d0: 742e 636f 6c75 6d6e 7329 7d20 577b 6c65  t.columns)} W{le
+0000f0e0: 6e28 7365 6c66 2e77 636f 6c75 6d6e 7329  n(self.wcolumns)
+0000f0f0: 7d27 0a20 2020 2020 2020 2020 2020 2063  }'.            c
+0000f100: 6869 6c64 5f6c 6f63 3a20 7479 7069 6e67  hild_loc: typing
+0000f110: 2e55 6e69 6f6e 5b69 6e74 2c20 7479 7069  .Union[int, typi
+0000f120: 6e67 2e4c 6974 6572 616c 5b27 656e 6427  ng.Literal['end'
+0000f130: 5d5d 0a20 2020 2020 2020 2020 2020 2069  ]].            i
+0000f140: 6620 7061 7265 6e74 5f6c 6f63 2069 7320  f parent_loc is 
+0000f150: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000f160: 2020 2020 2020 6368 696c 645f 6c6f 6320        child_loc 
+0000f170: 3d20 746b 2e45 4e44 0a20 2020 2020 2020  = tk.END.       
+0000f180: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000f190: 2020 2020 2020 2020 2020 2063 6869 6c64             child
+0000f1a0: 5f6c 6f63 203d 2070 6172 656e 745f 6c6f  _loc = parent_lo
+0000f1b0: 6320 2b20 6569 640a 2020 2020 2020 2020  c + eid.        
+0000f1c0: 2020 2020 6369 6420 3d20 7365 6c66 2e69      cid = self.i
+0000f1d0: 6e73 6572 7428 7061 7265 6e74 206f 7220  nsert(parent or 
+0000f1e0: 2727 2c20 6368 696c 645f 6c6f 632c 0a20  '', child_loc,. 
+0000f1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f200: 2020 2020 2020 2020 2020 2020 2074 6578               tex
+0000f210: 743d 656c 656d 656e 742e 6c61 6265 6c2c  t=element.label,
+0000f220: 2076 616c 7565 733d 7475 706c 6528 656c   values=tuple(el
+0000f230: 656d 656e 742e 636f 6c75 6d6e 7320 6f72  ement.columns or
+0000f240: 205b 5d29 2c0a 2020 2020 2020 2020 2020   []),.          
+0000f250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f260: 2020 2020 6f70 656e 3d5f 6c65 7665 6c20      open=_level 
+0000f270: 3c20 6f70 656e 6c65 7665 6c2c 0a20 2020  < openlevel,.   
+0000f280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f290: 2020 2020 2020 2020 2020 2069 6d61 6765             image
+0000f2a0: 3d65 6c65 6d65 6e74 2e69 6d61 6765 206f  =element.image o
+0000f2b0: 7220 2727 2c0a 2020 2020 2020 2020 2020  r '',.          
+0000f2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f2d0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000f2e0: 2020 7365 6c66 2e77 6461 7461 5b63 6964    self.wdata[cid
+0000f2f0: 5d20 3d20 656c 656d 656e 742e 6461 7461  ] = element.data
+0000f300: 0a20 2020 2020 2020 2020 2020 2023 2069  .            # i
+0000f310: 6620 5f5f 6465 6275 675f 5f3a 0a20 2020  f __debug__:.   
+0000f320: 2020 2020 2020 2020 2023 2020 2020 206c           #     l
+0000f330: 6f67 6765 722e 6465 6275 6728 6627 7b22  ogger.debug(f'{"
+0000f340: 7c22 202a 2028 5f6c 6576 656c 202b 2031  |" * (_level + 1
+0000f350: 297d 2049 443a 207b 6369 647d 2729 0a20  )} ID: {cid}'). 
+0000f360: 2020 2020 2020 2020 2020 2069 6620 656c             if el
+0000f370: 656d 656e 742e 6368 696c 6472 656e 3a0a  ement.children:.
+0000f380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f390: 2320 6966 205f 5f64 6562 7567 5f5f 3a0a  # if __debug__:.
+0000f3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f3b0: 2320 2020 2020 6c6f 6767 6572 2e64 6562  #     logger.deb
+0000f3c0: 7567 2866 277b 227c 2220 2a20 285f 6c65  ug(f'{"|" * (_le
+0000f3d0: 7665 6c20 2b20 3129 7d20 4368 696c 6472  vel + 1)} Childr
+0000f3e0: 656e 3a20 7b6c 656e 2865 6c65 6d65 6e74  en: {len(element
+0000f3f0: 2e63 6869 6c64 7265 6e29 7d27 290a 2020  .children)}').  
+0000f400: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000f410: 6c66 2e5f 5f74 7265 655f 7075 7428 656c  lf.__tree_put(el
+0000f420: 656d 656e 742e 6368 696c 6472 656e 2c0a  ement.children,.
+0000f430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f450: 7061 7265 6e74 3d63 6964 2c0a 2020 2020  parent=cid,.    
+0000f460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f470: 2020 2020 2020 2020 2020 2020 6f70 656e              open
+0000f480: 6c65 7665 6c3d 6f70 656e 6c65 7665 6c2c  level=openlevel,
+0000f490: 205f 6c65 7665 6c3d 5f6c 6576 656c 202b   _level=_level +
+0000f4a0: 2031 290a 0a20 2020 2064 6566 205f 5f74   1)..    def __t
+0000f4b0: 7265 655f 7365 7428 7365 6c66 2c20 2a61  ree_set(self, *a
+0000f4c0: 7267 732c 202a 2a6b 7761 7267 7329 202d  rgs, **kwargs) -
+0000f4d0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+0000f4e0: 6173 7365 7274 2073 656c 662e 7661 7269  assert self.vari
+0000f4f0: 6162 6c65 2069 7320 6e6f 7420 4e6f 6e65  able is not None
+0000f500: 2c20 6627 7b73 656c 6621 727d 3a20 4d69  , f'{self!r}: Mi
+0000f510: 7373 696e 6720 7661 7269 6162 6c65 270a  ssing variable'.
+0000f520: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
+0000f530: 7365 6c66 2e5f 7472 6565 5f67 6574 2873  self._tree_get(s
+0000f540: 656c 662e 7661 7269 6162 6c65 290a 2020  elf.variable).  
+0000f550: 2020 2020 2020 6966 2073 656c 662e 5f5f        if self.__
+0000f560: 6775 695f 6368 616e 6765 643a 0a20 2020  gui_changed:.   
+0000f570: 2020 2020 2020 2020 2023 2069 6620 5f5f           # if __
+0000f580: 6465 6275 675f 5f3a 0a20 2020 2020 2020  debug__:.       
+0000f590: 2020 2020 2023 2020 2020 206c 6f67 6765       #     logge
+0000f5a0: 722e 6465 6275 6728 6627 7b73 656c 667d  r.debug(f'{self}
+0000f5b0: 3a20 2020 4b65 6570 2047 5549 2073 7461  :   Keep GUI sta
+0000f5c0: 7465 2729 0a20 2020 2020 2020 2020 2020  te').           
+0000f5d0: 2073 656c 662e 5f5f 6775 695f 6368 616e   self.__gui_chan
+0000f5e0: 6765 6420 3d20 4661 6c73 650a 2020 2020  ged = False.    
+0000f5f0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000f600: 2020 2020 2020 2320 6966 205f 5f64 6562        # if __deb
+0000f610: 7567 5f5f 3a0a 2020 2020 2020 2020 2020  ug__:.          
+0000f620: 2020 2320 2020 2020 6c6f 6767 6572 2e64    #     logger.d
+0000f630: 6562 7567 2866 277b 7365 6c66 7d3a 2043  ebug(f'{self}: C
+0000f640: 6861 6e67 6520 4755 4920 7374 6174 6527  hange GUI state'
+0000f650: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+0000f660: 6c66 2e5f 5f74 7265 655f 636c 6561 6e28  lf.__tree_clean(
+0000f670: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+0000f680: 6c66 2e5f 5f74 7265 655f 7075 7428 7661  lf.__tree_put(va
+0000f690: 6c75 6529 0a20 2020 2020 2020 2069 6620  lue).        if 
+0000f6a0: 7365 6c66 2e77 7374 796c 652e 616c 7462  self.wstyle.altb
+0000f6b0: 673a 0a20 2020 2020 2020 2020 2020 2073  g:.            s
+0000f6c0: 656c 662e 5f74 6964 6c65 735b 2761 6c74  elf._tidles['alt
+0000f6d0: 6267 275d 2e73 6368 6564 756c 6528 290a  bg'].schedule().
+0000f6e0: 2020 2020 2020 2020 7365 6c66 2e5f 7472          self._tr
+0000f6f0: 6565 5f6f 6e73 6574 2876 616c 7565 290a  ee_onset(value).
+0000f700: 0a20 2020 2064 6566 2065 6c65 6d65 6e74  .    def element
+0000f710: 5f6d 6f76 6528 7365 6c66 2c20 7769 643a  _move(self, wid:
+0000f720: 2073 7472 2c20 6e65 7769 6e64 6578 3a20   str, newindex: 
+0000f730: 696e 7429 202d 3e20 626f 6f6c 3a0a 2020  int) -> bool:.  
+0000f740: 2020 2020 2020 2727 274d 6f76 6520 656c        '''Move el
+0000f750: 656d 656e 7420 6f6e 2074 6865 2060 5472  ement on the `Tr
+0000f760: 6565 6020 7769 7468 6f75 7420 7265 6372  ee` without recr
+0000f770: 6561 7469 6e67 2074 6865 2073 7461 7465  eating the state
+0000f780: 2e0a 0a20 2020 2020 2020 2054 6869 7320  ...        This 
+0000f790: 6973 2061 2060 7773 7461 7465 6020 616c  is a `wstate` al
+0000f7a0: 7465 726e 6174 6976 652c 2066 6f72 206d  ternative, for m
+0000f7b0: 6f76 696e 6720 616e 2065 7869 7374 696e  oving an existin
+0000f7c0: 6720 656c 656d 656e 7420 7769 7468 6f75  g element withou
+0000f7d0: 740a 2020 2020 2020 2020 6861 7669 6e67  t.        having
+0000f7e0: 2074 6f20 7265 6765 6e65 7261 7465 2074   to regenerate t
+0000f7f0: 6865 2065 6e74 6972 6520 7374 6174 652e  he entire state.
+0000f800: 2054 6869 7320 6861 7320 6d75 6368 2062   This has much b
+0000f810: 6574 7465 7220 7065 7266 6f72 6d61 6e63  etter performanc
+0000f820: 650a 2020 2020 2020 2020 6368 6172 6163  e.        charac
+0000f830: 7465 7269 7374 6963 732c 2070 6172 7469  teristics, parti
+0000f840: 6375 6c61 726c 7920 666f 7220 6269 6720  cularly for big 
+0000f850: 7472 6565 732e 0a0a 2020 2020 2020 2020  trees...        
+0000f860: 466f 7220 6e6f 7720 7468 6973 2064 6f65  For now this doe
+0000f870: 7320 6e6f 7420 7375 7070 6f72 7420 616e  s not support an
+0000f880: 7920 6368 696c 6472 656e 2065 6c65 6d65  y children eleme
+0000f890: 6e74 7320 616e 7977 6865 7265 2e0a 2020  nts anywhere..  
+0000f8a0: 2020 2020 2020 4576 6572 7974 6869 6e67        Everything
+0000f8b0: 206d 7573 7420 7265 6d61 696e 206f 6e20   must remain on 
+0000f8c0: 7468 6520 746f 706c 6576 656c 206c 6576  the toplevel lev
+0000f8d0: 656c 2e0a 0a20 2020 2020 2020 2052 6574  el...        Ret
+0000f8e0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+0000f8f0: 2020 6054 7275 6560 2077 6865 6e20 7468    `True` when th
+0000f900: 6520 7374 6174 6520 6973 2065 6666 6563  e state is effec
+0000f910: 7469 7665 6c79 2063 6861 6e67 6564 2c20  tively changed, 
+0000f920: 6046 616c 7365 6020 6f74 6865 7277 6973  `False` otherwis
+0000f930: 652e 0a20 2020 2020 2020 2020 2020 2054  e..            T
+0000f940: 6865 2072 6561 736f 6e73 2066 6f72 206e  he reasons for n
+0000f950: 6f74 2063 6861 6e67 696e 6720 7468 6520  ot changing the 
+0000f960: 7374 6174 6520 6d69 6768 7420 6265 2061  state might be a
+0000f970: 206e 6f2d 6f70 2028 7468 650a 2020 2020   no-op (the.    
+0000f980: 2020 2020 2020 2020 6375 7272 656e 7420          current 
+0000f990: 616e 6420 7468 6520 6e65 7720 696e 6465  and the new inde
+0000f9a0: 7865 7320 6172 6520 7468 6520 7361 6d65  xes are the same
+0000f9b0: 292c 206f 7220 616e 2069 6e76 616c 6964  ), or an invalid
+0000f9c0: 206f 7065 7261 7469 6f6e 0a20 2020 2020   operation.     
+0000f9d0: 2020 2020 2020 2028 6d6f 7669 6e67 2061         (moving a
+0000f9e0: 6e20 656c 656d 656e 7420 6f75 7473 6964  n element outsid
+0000f9f0: 6520 7468 6520 7261 6e67 6529 2e0a 0a20  e the range)... 
+0000fa00: 2020 2020 2020 2053 6565 2041 6c73 6f3a         See Also:
+0000fa10: 0a20 2020 2020 2020 2020 2020 2059 6f75  .            You
+0000fa20: 2063 616e 2067 6574 2074 6865 2073 656c   can get the sel
+0000fa30: 6563 7465 6420 656c 656d 656e 7420 7573  ected element us
+0000fa40: 696e 6720 6077 7369 6460 2e0a 2020 2020  ing `wsid`..    
+0000fa50: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+0000fa60: 7069 6420 3d20 2727 2020 2320 4f6e 6c79  pid = ''  # Only
+0000fa70: 2066 6f72 2074 6865 2074 6f70 6c65 7665   for the topleve
+0000fa80: 6c20 656c 656d 656e 7473 0a20 2020 2020  l elements.     
+0000fa90: 2020 206f 6c64 696e 6465 7820 3d20 7365     oldindex = se
+0000faa0: 6c66 2e69 6e64 6578 2877 6964 290a 2020  lf.index(wid).  
+0000fab0: 2020 2020 2020 6173 7365 7274 2077 6964        assert wid
+0000fac0: 2069 6e20 7365 6c66 2e77 6461 7461 2c20   in self.wdata, 
+0000fad0: 6627 7b73 656c 667d 3a20 4d69 7373 696e  f'{self}: Missin
+0000fae0: 6720 656c 656d 656e 7420 227b 7769 647d  g element "{wid}
+0000faf0: 2227 0a20 2020 2020 2020 2069 6620 5f5f  "'.        if __
+0000fb00: 6465 6275 675f 5f3a 0a20 2020 2020 2020  debug__:.       
+0000fb10: 2020 2020 206f 6c64 5f70 6964 203d 2073       old_pid = s
+0000fb20: 656c 662e 7061 7265 6e74 2877 6964 290a  elf.parent(wid).
+0000fb30: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+0000fb40: 7274 206f 6c64 5f70 6964 203d 3d20 7069  rt old_pid == pi
+0000fb50: 642c 2066 277b 7365 6c66 7d3a 2045 6c65  d, f'{self}: Ele
+0000fb60: 6d65 6e74 2022 7b77 6964 7d22 2063 6869  ment "{wid}" chi
+0000fb70: 6c64 206f 6620 227b 6f6c 645f 7069 647d  ld of "{old_pid}
+0000fb80: 2227 0a20 2020 2020 2020 2020 2020 2061  "'.            a
+0000fb90: 7373 6572 7420 6c65 6e28 7365 6c66 2e67  ssert len(self.g
+0000fba0: 6574 5f63 6869 6c64 7265 6e28 6974 656d  et_children(item
+0000fbb0: 3d77 6964 2929 203d 3d20 302c 2066 277b  =wid)) == 0, f'{
+0000fbc0: 7365 6c66 7d3a 2045 6c65 6d65 6e74 2022  self}: Element "
+0000fbd0: 7b77 6964 7d22 2068 6173 2063 6869 6c64  {wid}" has child
+0000fbe0: 7265 6e27 0a20 2020 2020 2020 2069 6620  ren'.        if 
+0000fbf0: 6f6c 6469 6e64 6578 203d 3d20 6e65 7769  oldindex == newi
+0000fc00: 6e64 6578 3a0a 2020 2020 2020 2020 2020  ndex:.          
+0000fc10: 2020 7265 7475 726e 2046 616c 7365 2020    return False  
+0000fc20: 2320 4e6f 2d4f 700a 2020 2020 2020 2020  # No-Op.        
+0000fc30: 6966 206e 6577 696e 6465 7820 3c20 3020  if newindex < 0 
+0000fc40: 6f72 206e 6577 696e 6465 7820 3e3d 206c  or newindex >= l
+0000fc50: 656e 2873 656c 662e 7764 6174 6129 3a0a  en(self.wdata):.
+0000fc60: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000fc70: 726e 2046 616c 7365 2020 2320 4f75 7473  rn False  # Outs
+0000fc80: 6964 6520 7468 6520 7261 6e67 650a 2020  ide the range.  
+0000fc90: 2020 2020 2020 6966 205f 5f64 6562 7567        if __debug
+0000fca0: 5f5f 3a0a 2020 2020 2020 2020 2020 2020  __:.            
+0000fcb0: 6e65 775f 6964 203d 2073 656c 662e 6765  new_id = self.ge
+0000fcc0: 745f 6368 696c 6472 656e 2869 7465 6d3d  t_children(item=
+0000fcd0: 7069 6429 5b6e 6577 696e 6465 785d 0a20  pid)[newindex]. 
+0000fce0: 2020 2020 2020 2020 2020 206e 6577 5f70             new_p
+0000fcf0: 6964 203d 2073 656c 662e 7061 7265 6e74  id = self.parent
+0000fd00: 286e 6577 5f69 6429 0a20 2020 2020 2020  (new_id).       
+0000fd10: 2020 2020 2061 7373 6572 7420 6e65 775f       assert new_
+0000fd20: 7069 6420 3d3d 2070 6964 2c20 6627 7b73  pid == pid, f'{s
+0000fd30: 656c 667d 3a20 4d6f 7669 6e67 2022 7b77  elf}: Moving "{w
+0000fd40: 6964 7d22 2069 6e74 6f20 7468 6520 6d69  id}" into the mi
+0000fd50: 6464 6c65 206f 6620 6368 696c 6472 656e  ddle of children
+0000fd60: 2028 227b 6e65 7769 6e64 6578 7d22 2927   ("{newindex}")'
+0000fd70: 0a20 2020 2020 2020 2023 2043 616c 6375  .        # Calcu
+0000fd80: 6c61 7465 2056 6172 6961 626c 6520 5374  late Variable St
+0000fd90: 6174 650a 2020 2020 2020 2020 7374 6174  ate.        stat
+0000fda0: 6520 3d20 7365 6c66 2e77 7374 6174 650a  e = self.wstate.
+0000fdb0: 2020 2020 2020 2020 7374 6174 655b 6f6c          state[ol
+0000fdc0: 6469 6e64 6578 5d2c 2073 7461 7465 5b6e  dindex], state[n
+0000fdd0: 6577 696e 6465 785d 203d 2073 7461 7465  ewindex] = state
+0000fde0: 5b6e 6577 696e 6465 785d 2c20 7374 6174  [newindex], stat
+0000fdf0: 655b 6f6c 6469 6e64 6578 5d0a 2020 2020  e[oldindex].    
+0000fe00: 2020 2020 2320 4368 616e 6765 2074 6865      # Change the
+0000fe10: 2047 5549 2053 7461 7465 0a20 2020 2020   GUI State.     
+0000fe20: 2020 2073 656c 662e 6d6f 7665 2877 6964     self.move(wid
+0000fe30: 2c20 7069 642c 206e 6577 696e 6465 7829  , pid, newindex)
+0000fe40: 0a20 2020 2020 2020 2023 2043 6861 6e67  .        # Chang
+0000fe50: 6520 7468 6520 5661 7269 6162 6c65 2053  e the Variable S
+0000fe60: 7461 7465 2028 6e6f 2047 5549 2063 6861  tate (no GUI cha
+0000fe70: 6e67 6573 290a 2020 2020 2020 2020 7365  nges).        se
+0000fe80: 6c66 2e5f 5f67 7569 5f63 6861 6e67 6564  lf.__gui_changed
+0000fe90: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
+0000fea0: 7365 6c66 2e77 7374 6174 6520 3d20 7374  self.wstate = st
+0000feb0: 6174 650a 2020 2020 2020 2020 7265 7475  ate.        retu
+0000fec0: 726e 2054 7275 650a 0a20 2020 2064 6566  rn True..    def
+0000fed0: 205f 5f74 7265 655f 616c 7462 6728 7365   __tree_altbg(se
+0000fee0: 6c66 2c20 2a2c 2072 656d 6f76 653a 2062  lf, *, remove: b
+0000fef0: 6f6f 6c20 3d20 4661 6c73 6529 202d 3e20  ool = False) -> 
+0000ff00: 4e6f 6e65 3a0a 2020 2020 2020 2020 2727  None:.        ''
+0000ff10: 2753 6574 7570 2074 6865 2061 6c74 6572  'Setup the alter
+0000ff20: 6e61 7465 2062 6163 6b67 726f 756e 642c  nate background,
+0000ff30: 2062 6173 6564 206f 6e20 7461 6773 2e0a   based on tags..
+0000ff40: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+0000ff50: 2020 2020 2020 2020 2020 2072 656d 6f76             remov
+0000ff60: 653a 2046 6f72 6365 2072 656d 6f76 696e  e: Force removin
+0000ff70: 6720 616c 6c20 7468 6520 6261 636b 6772  g all the backgr
+0000ff80: 6f75 6e64 730a 2020 2020 2020 2020 2727  ounds.        ''
+0000ff90: 270a 2020 2020 2020 2020 746e 616d 6520  '.        tname 
+0000ffa0: 3d20 5472 6565 2e5f 5f6c 696e 6573 5f61  = Tree.__lines_a
+0000ffb0: 6c74 0a20 2020 2020 2020 2069 6e64 6578  lt.        index
+0000ffc0: 3a20 696e 7420 3d20 7365 6c66 2e77 7374  : int = self.wst
+0000ffd0: 796c 652e 616c 7462 675f 7369 6e64 6578  yle.altbg_sindex
+0000ffe0: 0a20 2020 2020 2020 2066 6f72 2072 6964  .        for rid
+0000fff0: 2069 6e20 7365 6c66 2e5f 5f74 7265 655f   in self.__tree_
+00010000: 6c73 7669 7369 626c 6528 293a 0a20 2020  lsvisible():.   
+00010010: 2020 2020 2020 2020 2074 6167 7320 3d20           tags = 
+00010020: 7365 7428 7365 6c66 2e69 7465 6d28 7269  set(self.item(ri
+00010030: 642c 206f 7074 696f 6e3d 2774 6167 7327  d, option='tags'
+00010040: 2929 0a20 2020 2020 2020 2020 2020 2064  )).            d
+00010050: 6f74 6167 7320 3d20 4661 6c73 650a 2020  otags = False.  
+00010060: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+00010070: 2072 656d 6f76 6520 616e 6420 696e 6465   remove and inde
+00010080: 7820 2520 3220 3d3d 2030 3a0a 2020 2020  x % 2 == 0:.    
+00010090: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+000100a0: 6e61 6d65 206e 6f74 2069 6e20 7461 6773  name not in tags
+000100b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000100c0: 2020 2020 2020 7461 6773 2e61 6464 2874        tags.add(t
+000100d0: 6e61 6d65 290a 2020 2020 2020 2020 2020  name).          
+000100e0: 2020 2020 2020 2020 2020 646f 7461 6773            dotags
+000100f0: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
+00010100: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00010110: 2020 2020 2020 2020 2020 6966 2074 6e61            if tna
+00010120: 6d65 2069 6e20 7461 6773 3a0a 2020 2020  me in tags:.    
+00010130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010140: 7461 6773 2e72 656d 6f76 6528 746e 616d  tags.remove(tnam
+00010150: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+00010160: 2020 2020 2020 2064 6f74 6167 7320 3d20         dotags = 
+00010170: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
+00010180: 2069 6620 646f 7461 6773 3a0a 2020 2020   if dotags:.    
+00010190: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000101a0: 2e69 7465 6d28 7269 642c 2074 6167 733d  .item(rid, tags=
+000101b0: 6c69 7374 2874 6167 7329 290a 2020 2020  list(tags)).    
+000101c0: 2020 2020 2020 2020 696e 6465 7820 2b3d          index +=
+000101d0: 2031 0a20 2020 2020 2020 2023 2069 6620   1.        # if 
+000101e0: 5f5f 6465 6275 675f 5f3a 0a20 2020 2020  __debug__:.     
+000101f0: 2020 2023 2020 2020 2023 2054 6869 7320     #     # This 
+00010200: 7368 6f75 6c64 2072 756e 206f 6e6c 7920  should run only 
+00010210: 6f6e 6365 2c20 6576 656e 2077 6974 6820  once, even with 
+00010220: 6d75 6c74 6970 6c65 2063 6861 6e67 6573  multiple changes
+00010230: 0a20 2020 2020 2020 2023 2020 2020 2069  .        #     i
+00010240: 6620 696e 6465 7820 3e20 7365 6c66 2e77  f index > self.w
+00010250: 7374 796c 652e 616c 7462 675f 7369 6e64  style.altbg_sind
+00010260: 6578 3a0a 2020 2020 2020 2020 2320 2020  ex:.        #   
+00010270: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+00010280: 7567 2866 277b 7365 6c66 7d3a 2043 616c  ug(f'{self}: Cal
+00010290: 6375 6c61 7465 6420 416c 7442 4727 290a  culated AltBG').
+000102a0: 0a20 2020 2064 6566 2077 7369 6428 7365  .    def wsid(se
+000102b0: 6c66 2920 2d3e 2074 7970 696e 672e 4f70  lf) -> typing.Op
+000102c0: 7469 6f6e 616c 5b73 7472 5d3a 0a20 2020  tional[str]:.   
+000102d0: 2020 2020 2027 2727 4765 7420 7468 6520       '''Get the 
+000102e0: 7365 6c65 6374 6564 2065 6c65 6d65 6e74  selected element
+000102f0: 2069 6465 6e74 6966 6965 722e 0a0a 2020   identifier...  
+00010300: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+00010310: 2020 2020 2020 2020 2020 2060 456c 656d             `Elem
+00010320: 656e 7420 3c6d 6f64 656c 2e54 7265 6545  ent <model.TreeE
+00010330: 6c65 6d65 6e74 3e60 2069 642c 206f 7220  lement>` id, or 
+00010340: 604e 6f6e 6560 2077 6865 6e20 6e6f 7468  `None` when noth
+00010350: 696e 6720 6973 2073 656c 6563 7465 642e  ing is selected.
+00010360: 0a0a 2020 2020 2020 2020 2020 2020 4966  ..            If
+00010370: 2074 6865 2077 6964 6765 7420 7761 7320   the widget was 
+00010380: 6372 6561 7465 6420 7769 7468 6f75 7420  created without 
+00010390: 7468 6520 6060 7365 6c65 6374 6162 6c65  the ``selectable
+000103a0: 6060 2066 6c61 672c 2074 6869 7320 616c  `` flag, this al
+000103b0: 7761 7973 0a20 2020 2020 2020 2020 2020  ways.           
+000103c0: 2072 6574 7572 6e73 2060 4e6f 6e65 602e   returns `None`.
+000103d0: 0a0a 2020 2020 2020 2020 5365 6520 416c  ..        See Al
+000103e0: 736f 3a0a 2020 2020 2020 2020 2020 2020  so:.            
+000103f0: 5573 6520 6077 7365 6c60 2074 6f20 7365  Use `wsel` to se
+00010400: 7420 7468 6520 6375 7272 656e 746c 7920  t the currently 
+00010410: 7365 6c65 6374 6564 2065 6c65 6d65 6e74  selected element
+00010420: 2069 6465 6e74 6966 6965 722e 0a20 2020   identifier..   
+00010430: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00010440: 2073 656c 6563 7469 6f6e 203d 2073 656c   selection = sel
+00010450: 662e 7365 6c65 6374 696f 6e28 290a 2020  f.selection().  
+00010460: 2020 2020 2020 6966 205f 5f64 6562 7567        if __debug
+00010470: 5f5f 3a0a 2020 2020 2020 2020 2020 2020  __:.            
+00010480: 7365 6c65 6374 6d6f 6465 203d 2073 7472  selectmode = str
+00010490: 2873 656c 665b 2773 656c 6563 746d 6f64  (self['selectmod
+000104a0: 6527 5d29 0a20 2020 2020 2020 2020 2020  e']).           
+000104b0: 2061 7373 6572 7420 7365 6c65 6374 6d6f   assert selectmo
+000104c0: 6465 2069 6e20 5b74 6b2e 4252 4f57 5345  de in [tk.BROWSE
+000104d0: 2c20 746b 2e4e 4f4e 455d 2c20 6627 7b73  , tk.NONE], f'{s
+000104e0: 656c 6621 727d 3a20 496e 7661 6c69 6420  elf!r}: Invalid 
+000104f0: 5365 6c65 6374 696f 6e20 4d6f 6465 3a20  Selection Mode: 
+00010500: 7b73 656c 6563 746d 6f64 657d 270a 2020  {selectmode}'.  
+00010510: 2020 2020 2020 2020 2020 2320 6c6f 6767            # logg
+00010520: 6572 2e64 6562 7567 2827 5365 6c65 6374  er.debug('Select
+00010530: 696f 6e3a 2025 7227 2c20 7365 6c65 6374  ion: %r', select
+00010540: 696f 6e29 0a20 2020 2020 2020 2069 6620  ion).        if 
+00010550: 6c65 6e28 7365 6c65 6374 696f 6e29 203d  len(selection) =
+00010560: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+00010570: 2023 2053 6b69 7020 756e 2d73 656c 6563   # Skip un-selec
+00010580: 7469 6f6e 730a 2020 2020 2020 2020 2020  tions.          
+00010590: 2020 2320 5573 7561 6c6c 7920 7468 6520    # Usually the 
+000105a0: 5472 6565 2063 6f6e 7465 6e74 7320 6368  Tree contents ch
+000105b0: 616e 6765 642e 2e2e 0a20 2020 2020 2020  anged....       
+000105c0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+000105d0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+000105e0: 2020 2020 2020 2020 2020 2023 2052 6567             # Reg
+000105f0: 756c 6172 2053 656c 6563 7469 6f6e 0a20  ular Selection. 
+00010600: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+00010610: 7420 6c65 6e28 7365 6c65 6374 696f 6e29  t len(selection)
+00010620: 203d 3d20 312c 2066 277b 7365 6c66 2172   == 1, f'{self!r
+00010630: 7d3a 2049 6e76 616c 6964 2073 656c 6563  }: Invalid selec
+00010640: 7469 6f6e 206d 6f64 6527 0a20 2020 2020  tion mode'.     
+00010650: 2020 2020 2020 2074 7265 6569 6420 3d20         treeid = 
+00010660: 7365 6c65 6374 696f 6e5b 305d 0a20 2020  selection[0].   
+00010670: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00010680: 7472 6565 6964 0a0a 2020 2020 6465 6620  treeid..    def 
+00010690: 7773 656c 2873 656c 662c 2077 6964 3a20  wsel(self, wid: 
+000106a0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+000106b0: 7374 725d 2c20 2a2c 2073 6565 3a20 626f  str], *, see: bo
+000106c0: 6f6c 203d 2054 7275 6529 202d 3e20 7479  ol = True) -> ty
+000106d0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7374  ping.Optional[st
+000106e0: 725d 3a0a 2020 2020 2020 2020 2727 2753  r]:.        '''S
+000106f0: 6574 2074 6865 2063 7572 7265 6e74 6c79  et the currently
+00010700: 2073 656c 6563 7465 6420 656c 656d 656e   selected elemen
+00010710: 7420 6964 656e 7469 6669 6572 2e0a 0a20  t identifier... 
+00010720: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
+00010730: 746f 2065 6e73 7572 696e 6720 7468 6520  to ensuring the 
+00010740: 7365 6c65 6374 6564 2065 6c65 6d65 6e74  selected element
+00010750: 2c20 6279 2073 6372 6f6c 6c69 6e67 2074  , by scrolling t
+00010760: 6865 2076 6965 772e 2054 6869 730a 2020  he view. This.  
+00010770: 2020 2020 2020 6973 2063 6f6e 7472 6f6c        is control
+00010780: 6c65 6420 6279 2074 6865 2060 6073 6565  led by the ``see
+00010790: 6060 2061 7267 756d 656e 742e 0a0a 2020  `` argument...  
+000107a0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+000107b0: 2020 2020 2020 2020 7769 643a 2054 6865          wid: The
+000107c0: 2065 6c65 6d65 6e74 2069 6465 6e74 6966   element identif
+000107d0: 6965 7220 746f 2073 656c 6563 742e 2060  ier to select. `
+000107e0: 4e6f 6e65 6020 746f 2063 6c65 6172 2074  None` to clear t
+000107f0: 6865 0a20 2020 2020 2020 2020 2020 2020  he.             
+00010800: 2020 2073 656c 6563 7469 6f6e 2e0a 2020     selection..  
+00010810: 2020 2020 2020 2020 2020 7365 653a 2045            see: E
+00010820: 6e73 7572 6520 7468 6520 656c 656d 656e  nsure the elemen
+00010830: 7420 6973 2076 6973 6962 6c65 2e0a 0a20  t is visible... 
+00010840: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00010850: 2020 2020 2020 2020 2020 2020 5265 7475              Retu
+00010860: 726e 2074 6865 2073 6f75 7263 6520 6060  rn the source ``
+00010870: 7769 6460 6020 6172 6775 6d65 6e74 2e0a  wid`` argument..
+00010880: 0a20 2020 2020 2020 2053 6565 2041 6c73  .        See Als
+00010890: 6f3a 0a20 2020 2020 2020 2020 2020 2055  o:.            U
+000108a0: 7365 2060 7773 6964 6020 746f 2067 6574  se `wsid` to get
+000108b0: 2074 6865 2063 7572 7265 6e74 6c79 2073   the currently s
+000108c0: 656c 6563 7465 6420 6461 7461 2e0a 2020  elected data..  
+000108d0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+000108e0: 2020 6966 2077 6964 2069 7320 4e6f 6e65    if wid is None
+000108f0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00010900: 436c 6561 7220 7365 6c65 6374 696f 6e0a  Clear selection.
+00010910: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010920: 2e73 656c 6563 7469 6f6e 5f72 656d 6f76  .selection_remov
+00010930: 6528 2a73 656c 662e 7764 6174 612e 6b65  e(*self.wdata.ke
+00010940: 7973 2829 290a 2020 2020 2020 2020 656c  ys()).        el
+00010950: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00010960: 6173 7365 7274 2077 6964 2069 6e20 7365  assert wid in se
+00010970: 6c66 2e77 6461 7461 2c20 6627 7b73 656c  lf.wdata, f'{sel
+00010980: 667d 3a20 4d69 7373 696e 6720 656c 656d  f}: Missing elem
+00010990: 656e 7420 227b 7769 647d 2227 0a20 2020  ent "{wid}"'.   
+000109a0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+000109b0: 6c65 6374 696f 6e5f 7365 7428 7769 6429  lection_set(wid)
+000109c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000109d0: 7365 653a 0a20 2020 2020 2020 2020 2020  see:.           
+000109e0: 2020 2020 2073 656c 662e 7365 6528 7769       self.see(wi
+000109f0: 6429 0a20 2020 2020 2020 2072 6574 7572  d).        retur
+00010a00: 6e20 7769 640a 0a20 2020 2064 6566 2077  n wid..    def w
+00010a10: 7365 6c65 6374 696f 6e28 7365 6c66 2920  selection(self) 
+00010a20: 2d3e 2074 7970 696e 672e 4f70 7469 6f6e  -> typing.Option
+00010a30: 616c 5b74 7970 696e 672e 416e 795d 3a0a  al[typing.Any]:.
+00010a40: 2020 2020 2020 2020 2727 2747 6574 2074          '''Get t
+00010a50: 6865 2073 656c 6563 7465 6420 6461 7461  he selected data
+00010a60: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00010a70: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+00010a80: 5369 6e63 6520 7468 6973 2073 7570 706f  Since this suppo
+00010a90: 7274 7320 6f6e 6c79 2061 2073 696e 676c  rts only a singl
+00010aa0: 6520 7365 6c65 6374 696f 6e2c 2072 6574  e selection, ret
+00010ab0: 7572 6e20 7468 6520 7365 6c65 6374 6564  urn the selected
+00010ac0: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+00010ad0: 7565 2c20 6f72 2060 604e 6f6e 6560 6020  ue, or ``None`` 
+00010ae0: 7768 656e 206e 6f74 6869 6e67 2069 7320  when nothing is 
+00010af0: 7365 6c65 6374 6564 2e0a 0a20 2020 2020  selected...     
+00010b00: 2020 2020 2020 2049 6620 7468 6520 7769         If the wi
+00010b10: 6467 6574 2077 6173 2063 7265 6174 6564  dget was created
+00010b20: 2077 6974 686f 7574 2074 6865 2060 6073   without the ``s
+00010b30: 656c 6563 7461 626c 6560 6020 666c 6167  electable`` flag
+00010b40: 2c20 7468 6973 2061 6c77 6179 730a 2020  , this always.  
+00010b50: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00010b60: 7320 604e 6f6e 6560 2e0a 0a20 2020 2020  s `None`...     
+00010b70: 2020 2053 6565 2041 6c73 6f3a 0a20 2020     See Also:.   
+00010b80: 2020 2020 2020 2020 2055 7365 2060 7773           Use `ws
+00010b90: 656c 6563 7460 2074 6f20 7365 7420 7468  elect` to set th
+00010ba0: 6520 6375 7272 656e 746c 7920 7365 6c65  e currently sele
+00010bb0: 6374 6564 2064 6174 612e 0a20 2020 2020  cted data..     
+00010bc0: 2020 2027 2727 0a20 2020 2020 2020 2077     '''.        w
+00010bd0: 7369 6420 3d20 7365 6c66 2e77 7369 6428  sid = self.wsid(
+00010be0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00010bf0: 2073 656c 662e 7764 6174 615b 7773 6964   self.wdata[wsid
+00010c00: 5d20 6966 2077 7369 6420 656c 7365 204e  ] if wsid else N
+00010c10: 6f6e 650a 0a20 2020 2064 6566 2077 7365  one..    def wse
+00010c20: 6c65 6374 2873 656c 662c 2073 656c 6563  lect(self, selec
+00010c30: 7469 6f6e 3a20 7479 7069 6e67 2e4f 7074  tion: typing.Opt
+00010c40: 696f 6e61 6c5b 7479 7069 6e67 2e41 6e79  ional[typing.Any
+00010c50: 5d2c 202a 2c20 7365 653a 2062 6f6f 6c20  ], *, see: bool 
+00010c60: 3d20 5472 7565 2920 2d3e 2074 7970 696e  = True) -> typin
+00010c70: 672e 4f70 7469 6f6e 616c 5b73 7472 5d3a  g.Optional[str]:
+00010c80: 0a20 2020 2020 2020 2027 2727 5365 7420  .        '''Set 
+00010c90: 7468 6520 6375 7272 656e 7420 7365 6c65  the current sele
+00010ca0: 6374 696f 6e20 6461 7461 2e0a 0a20 2020  ction data...   
+00010cb0: 2020 2020 2054 6869 7320 7769 6c6c 2073       This will s
+00010cc0: 656c 6563 7420 7468 6520 656c 656d 656e  elect the elemen
+00010cd0: 7420 7769 7468 2074 6865 2067 6976 656e  t with the given
+00010ce0: 2064 6174 612e 2054 6869 7320 7769 6c6c   data. This will
+00010cf0: 206e 6565 6420 746f 0a20 2020 2020 2020   need to.       
+00010d00: 2072 6561 6420 7468 6520 7768 6f6c 6520   read the whole 
+00010d10: 6461 7461 2c20 616e 6420 646f 6573 206e  data, and does n
+00010d20: 6f74 2073 7570 706f 7274 206d 756c 7469  ot support multi
+00010d30: 706c 6520 656c 656d 656e 7473 2077 6974  ple elements wit
+00010d40: 6820 7468 650a 2020 2020 2020 2020 7361  h the.        sa
+00010d50: 6d65 2064 6174 612e 2041 766f 6964 2075  me data. Avoid u
+00010d60: 7369 6e67 2074 6869 7320 756e 6c65 7373  sing this unless
+00010d70: 2061 6273 6f6c 7574 656c 7920 6e65 6564   absolutely need
+00010d80: 6564 2c20 7573 6520 6077 7365 6c60 0a20  ed, use `wsel`. 
+00010d90: 2020 2020 2020 2064 6972 6563 746c 792e         directly.
+00010da0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+00010db0: 2020 2020 2020 2020 2020 2020 7365 6c65              sele
+00010dc0: 6374 696f 6e3a 2054 6865 2065 6c65 6d65  ction: The eleme
+00010dd0: 6e74 2064 6174 6120 746f 2073 656c 6563  nt data to selec
+00010de0: 742e 2060 4e6f 6e65 6020 636c 6561 7273  t. `None` clears
+00010df0: 2074 6865 2073 656c 6563 7469 6f6e 2e0a   the selection..
+00010e00: 2020 2020 2020 2020 2020 2020 7365 653a              see:
+00010e10: 2045 6e73 7572 6520 7468 6520 656c 656d   Ensure the elem
+00010e20: 656e 7420 6973 2076 6973 6962 6c65 2e0a  ent is visible..
+00010e30: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00010e40: 3a0a 2020 2020 2020 2020 2020 2020 5265  :.            Re
+00010e50: 7475 726e 2074 6865 2073 656c 6563 7465  turn the selecte
+00010e60: 6420 656c 656d 656e 7420 6964 656e 7469  d element identi
+00010e70: 6669 6572 2e0a 0a20 2020 2020 2020 2053  fier...        S
+00010e80: 6565 2041 6c73 6f3a 0a20 2020 2020 2020  ee Also:.       
+00010e90: 2020 2020 2055 7365 2060 7773 656c 6020       Use `wsel` 
+00010ea0: 746f 2073 656c 6563 7420 6120 7370 6563  to select a spec
+00010eb0: 6966 6963 2069 6465 6e74 6966 6965 722e  ific identifier.
+00010ec0: 0a20 2020 2020 2020 2020 2020 2055 7365  .            Use
+00010ed0: 2060 7773 656c 6563 7469 6f6e 6020 746f   `wselection` to
+00010ee0: 2067 6574 2074 6865 2063 7572 7265 6e74   get the current
+00010ef0: 6c79 2073 656c 6563 7465 6420 6461 7461  ly selected data
+00010f00: 2e0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
+00010f10: 2020 2020 2020 6966 2073 656c 6563 7469        if selecti
+00010f20: 6f6e 2069 7320 4e6f 6e65 3a0a 2020 2020  on is None:.    
+00010f30: 2020 2020 2020 2020 7773 6964 203d 204e          wsid = N
+00010f40: 6f6e 650a 2020 2020 2020 2020 656c 7365  one.        else
+00010f50: 3a0a 2020 2020 2020 2020 2020 2020 7773  :.            ws
+00010f60: 6964 7320 3d20 5b77 7369 6420 666f 7220  ids = [wsid for 
+00010f70: 7773 6964 2069 6e20 7365 6c66 2e5f 5f74  wsid in self.__t
+00010f80: 7265 655f 6c73 2829 2069 6620 7365 6c66  ree_ls() if self
+00010f90: 2e77 6461 7461 5b77 7369 645d 203d 3d20  .wdata[wsid] == 
+00010fa0: 7365 6c65 6374 696f 6e5d 0a20 2020 2020  selection].     
+00010fb0: 2020 2020 2020 2061 7373 6572 7420 6c65         assert le
+00010fc0: 6e28 7773 6964 7329 203e 2030 2c20 6627  n(wsids) > 0, f'
+00010fd0: 7b73 656c 667d 3a20 4d69 7373 696e 6720  {self}: Missing 
+00010fe0: 7365 6c65 6374 696f 6e20 227b 7365 6c65  selection "{sele
+00010ff0: 6374 696f 6e7d 270a 2020 2020 2020 2020  ction}'.        
+00011000: 2020 2020 6173 7365 7274 206c 656e 2877      assert len(w
+00011010: 7369 6473 2920 3d3d 2031 2c20 6627 7b73  sids) == 1, f'{s
+00011020: 656c 667d 3a20 4d75 6c74 6970 6c65 2073  elf}: Multiple s
+00011030: 656c 6563 7469 6f6e 7320 227b 7365 6c65  elections "{sele
+00011040: 6374 696f 6e7d 2220 3e20 7b77 7369 6473  ction}" > {wsids
+00011050: 7d27 0a20 2020 2020 2020 2020 2020 2077  }'.            w
+00011060: 7369 6420 3d20 7773 6964 735b 305d 0a20  sid = wsids[0]. 
+00011070: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00011080: 6c66 2e77 7365 6c28 7773 6964 2c20 7365  lf.wsel(wsid, se
+00011090: 653d 7365 6529 0a0a 2020 2020 6465 6620  e=see)..    def 
+000110a0: 5f6f 6e53 656c 6563 7428 7365 6c66 2c20  _onSelect(self, 
+000110b0: 6576 656e 743d 4e6f 6e65 293a 0a20 2020  event=None):.   
+000110c0: 2020 2020 2027 2727 2727 2720 2023 2049       ''''''  # I
+000110d0: 6e74 6572 6e61 6c2c 2064 6f20 6e6f 7420  nternal, do not 
+000110e0: 646f 6375 6d65 6e74 0a20 2020 2020 2020  document.       
+000110f0: 2073 656c 6563 7469 6f6e 3a20 7475 706c   selection: tupl
+00011100: 6520 3d20 7365 6c66 2e73 656c 6563 7469  e = self.selecti
+00011110: 6f6e 2829 0a20 2020 2020 2020 2069 6620  on().        if 
+00011120: 5f5f 6465 6275 675f 5f3a 0a20 2020 2020  __debug__:.     
+00011130: 2020 2020 2020 2073 656c 6563 746d 6f64         selectmod
+00011140: 6520 3d20 7374 7228 7365 6c66 5b27 7365  e = str(self['se
+00011150: 6c65 6374 6d6f 6465 275d 290a 2020 2020  lectmode']).    
+00011160: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
+00011170: 656c 6563 746d 6f64 6520 696e 205b 746b  electmode in [tk
+00011180: 2e42 524f 5753 452c 2074 6b2e 4e4f 4e45  .BROWSE, tk.NONE
+00011190: 5d2c 2066 277b 7365 6c66 2172 7d3a 2049  ], f'{self!r}: I
+000111a0: 6e76 616c 6964 2053 656c 6563 7469 6f6e  nvalid Selection
+000111b0: 204d 6f64 653a 207b 7365 6c65 6374 6d6f   Mode: {selectmo
+000111c0: 6465 7d27 0a20 2020 2020 2020 2020 2020  de}'.           
+000111d0: 2023 206c 6f67 6765 722e 6465 6275 6728   # logger.debug(
+000111e0: 2753 656c 6563 7469 6f6e 3a20 2572 272c  'Selection: %r',
+000111f0: 2073 656c 662e 7365 6c65 6374 696f 6e28   self.selection(
+00011200: 2929 0a20 2020 2020 2020 2069 6620 6c65  )).        if le
+00011210: 6e28 7365 6c65 6374 696f 6e29 203d 3d20  n(selection) == 
+00011220: 303a 0a20 2020 2020 2020 2020 2020 2023  0:.            #
+00011230: 2053 6b69 700a 2020 2020 2020 2020 2020   Skip.          
+00011240: 2020 2320 2d20 4e4f 4e45 2073 656c 6563    # - NONE selec
+00011250: 746d 6f64 650a 2020 2020 2020 2020 2020  tmode.          
+00011260: 2020 2320 2d20 756e 2d73 656c 6563 7469    # - un-selecti
+00011270: 6f6e 7320 2875 7375 616c 6c79 2074 6865  ons (usually the
+00011280: 2054 7265 6520 636f 6e74 656e 7473 2063   Tree contents c
+00011290: 6861 6e67 6564 290a 2020 2020 2020 2020  hanged).        
+000112a0: 2020 2020 7061 7373 0a20 2020 2020 2020      pass.       
+000112b0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000112c0: 2020 2023 2052 6567 756c 6172 2053 656c     # Regular Sel
+000112d0: 6563 7469 6f6e 0a20 2020 2020 2020 2020  ection.         
+000112e0: 2020 2061 7373 6572 7420 6c65 6e28 7365     assert len(se
+000112f0: 6c65 6374 696f 6e29 203d 3d20 312c 2066  lection) == 1, f
+00011300: 277b 7365 6c66 2172 7d3a 2049 6e76 616c  '{self!r}: Inval
+00011310: 6964 2073 656c 6563 7469 6f6e 206d 6f64  id selection mod
+00011320: 6527 0a20 2020 2020 2020 2020 2020 2074  e'.            t
+00011330: 7265 6569 6420 3d20 7365 6c65 6374 696f  reeid = selectio
+00011340: 6e5b 305d 0a20 2020 2020 2020 2020 2020  n[0].           
+00011350: 2064 6174 6120 3d20 7365 6c66 2e77 6461   data = self.wda
+00011360: 7461 5b74 7265 6569 645d 0a20 2020 2020  ta[treeid].     
+00011370: 2020 2020 2020 2073 656c 662e 6f6e 5365         self.onSe
+00011380: 6c65 6374 2874 7265 6569 642c 2064 6174  lect(treeid, dat
+00011390: 6129 0a0a 2020 2020 6465 6620 5f74 7265  a)..    def _tre
+000113a0: 655f 6f6e 7365 7428 7365 6c66 2c20 7661  e_onset(self, va
+000113b0: 6c75 653a 2074 7970 696e 672e 5365 7175  lue: typing.Sequ
+000113c0: 656e 6365 5b6d 6f64 656c 2e54 7265 6545  ence[model.TreeE
+000113d0: 6c65 6d65 6e74 5d29 202d 3e20 4e6f 6e65  lement]) -> None
+000113e0: 3a0a 2020 2020 2020 2020 2727 2743 616c  :.        '''Cal
+000113f0: 6c62 6163 6b20 746f 2062 6520 6578 6563  lback to be exec
+00011400: 7574 6564 2077 6865 6e20 7365 7474 696e  uted when settin
+00011410: 6720 6120 6469 6666 6572 656e 7420 7661  g a different va
+00011420: 6c75 652e 0a0a 2020 2020 2020 2020 4176  lue...        Av
+00011430: 6169 6c61 626c 6520 666f 7220 7375 6263  ailable for subc
+00011440: 6c61 7373 2072 6564 6566 696e 6974 696f  lass redefinitio
+00011450: 6e2e 0a20 2020 2020 2020 2027 2727 0a20  n..        '''. 
+00011460: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+00011470: 2064 6566 206f 6e53 656c 6563 7428 7365   def onSelect(se
+00011480: 6c66 2c20 7472 6565 6964 3a20 7374 722c  lf, treeid: str,
+00011490: 2064 6174 613a 2074 7970 696e 672e 416e   data: typing.An
+000114a0: 7920 3d20 4e6f 6e65 2920 2d3e 204e 6f6e  y = None) -> Non
+000114b0: 653a 0a20 2020 2020 2020 2027 2727 4361  e:.        '''Ca
+000114c0: 6c6c 6261 636b 2074 6f20 6265 2065 7865  llback to be exe
+000114d0: 6375 7465 6420 7768 656e 2063 6c69 636b  cuted when click
+000114e0: 696e 6720 7468 6973 2077 6964 6765 742e  ing this widget.
+000114f0: 0a0a 2020 2020 2020 2020 4465 6661 756c  ..        Defaul
+00011500: 7473 2074 6f20 646f 696e 6720 6e6f 7468  ts to doing noth
+00011510: 696e 672e 0a0a 2020 2020 2020 2020 4176  ing...        Av
+00011520: 6169 6c61 626c 6520 666f 7220 7375 6263  ailable for subc
+00011530: 6c61 7373 2072 6564 6566 696e 6974 696f  lass redefinitio
+00011540: 6e2e 0a0a 2020 2020 2020 2020 4172 6773  n...        Args
+00011550: 3a0a 2020 2020 2020 2020 2020 2020 7472  :.            tr
+00011560: 6565 6964 3a20 5468 6520 7365 6c65 6374  eeid: The select
+00011570: 6564 2074 7265 6520 6964 0a20 2020 2020  ed tree id.     
+00011580: 2020 2020 2020 2064 6174 613a 2054 6865         data: The
+00011590: 2061 7262 6974 7261 7279 2064 6174 6120   arbitrary data 
+000115a0: 6173 736f 6369 6174 6564 2077 6974 6820  associated with 
+000115b0: 7468 6520 656c 656d 656e 742e 2044 6566  the element. Def
+000115c0: 6175 6c74 7320 746f 2060 4e6f 6e65 602e  aults to `None`.
+000115d0: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+000115e0: 2020 2020 2070 6173 730a 0a0a 636c 6173       pass...clas
+000115f0: 7320 4c69 7374 626f 7828 5472 6565 293a  s Listbox(Tree):
+00011600: 0a20 2020 2027 2727 4120 6c69 7374 626f  .    '''A listbo
+00011610: 7820 7769 6467 6574 2c20 6120 6c69 7374  x widget, a list
+00011620: 206f 6620 7374 7269 6e67 732e 0a0a 2020   of strings...  
+00011630: 2020 5468 6973 2069 7320 6120 6d6f 6465    This is a mode
+00011640: 726e 2076 6172 6961 7469 6f6e 206f 6620  rn variation of 
+00011650: 7468 6520 6c69 7374 626f 782c 2061 2077  the listbox, a w
+00011660: 6179 2074 6f20 6469 7370 6c61 7920 7365  ay to display se
+00011670: 7665 7261 6c20 726f 7773 206f 660a 2020  veral rows of.  
+00011680: 2020 636f 6e74 656e 7420 2873 696d 706c    content (simpl
+00011690: 6520 7374 7269 6e67 732c 2069 6e20 7468  e strings, in th
+000116a0: 6973 2063 6173 6529 2c20 616e 6420 6265  is case), and be
+000116b0: 2061 626c 6520 746f 2073 656c 6563 7420   able to select 
+000116c0: 6f6e 6520 6174 2061 0a20 2020 2074 696d  one at a.    tim
+000116d0: 652e 0a0a 2020 2020 5468 6520 6060 6865  e...    The ``he
+000116e0: 6967 6874 6060 2063 616e 2062 6520 6861  ight`` can be ha
+000116f0: 7264 636f 6465 6420 746f 2061 2076 616c  rdcoded to a val
+00011700: 7565 2c20 6f72 2069 7420 6361 6e20 7661  ue, or it can va
+00011710: 7279 2077 6974 6820 7468 650a 2020 2020  ry with the.    
+00011720: 636f 6e74 656e 7473 2e20 4e6f 7465 2074  contents. Note t
+00011730: 6861 7420 7468 6520 6060 6d61 7848 6569  hat the ``maxHei
+00011740: 6768 7460 6020 6973 2073 6d61 6c6c 6572  ght`` is smaller
+00011750: 2074 6861 6e20 7468 6520 616d 6f75 6e74   than the amount
+00011760: 206f 6620 726f 7773 2074 6f0a 2020 2020   of rows to.    
+00011770: 6469 7370 6c61 792c 206e 6f20 7363 726f  display, no scro
+00011780: 6c6c 6261 7220 6973 2073 686f 776e 2c20  llbar is shown, 
+00011790: 6275 7420 7468 6520 6c69 7374 2063 616e  but the list can
+000117a0: 2062 650a 2020 2020 7363 726f 6c6c 6564   be.    scrolled
+000117b0: 2077 6974 6820 7468 6520 6d6f 7573 6520   with the mouse 
+000117c0: 7768 6565 6c2e 0a20 2020 2054 6865 2061  wheel..    The a
+000117d0: 7574 6f6d 6174 6963 2076 6172 6961 7469  utomatic variati
+000117e0: 6f6e 206f 6e20 7468 6520 6865 6967 6874  on on the height
+000117f0: 2073 697a 6520 2841 4b41 2061 7574 6f2d   size (AKA auto-
+00011800: 6865 6967 6874 2920 6361 6e20 6265 0a20  height) can be. 
+00011810: 2020 2063 6f6d 706c 6574 656c 7920 6469     completely di
+00011820: 7361 626c 6564 2062 7920 7365 7474 696e  sabled by settin
+00011830: 6720 616c 6c20 6865 6967 6874 2d72 656c  g all height-rel
+00011840: 6174 6564 2061 7267 756d 656e 7473 2074  ated arguments t
+00011850: 6f20 604e 6f6e 6560 2e20 5468 6973 0a20  o `None`. This. 
+00011860: 2020 2069 7320 7468 6520 6465 6661 756c     is the defaul
+00011870: 742e 2054 6865 2060 6065 7870 616e 6460  t. The ``expand`
+00011880: 6020 6172 6775 6d65 6e74 2069 7320 7365  ` argument is se
+00011890: 7420 746f 2060 4661 6c73 6560 2077 6865  t to `False` whe
+000118a0: 6e20 7468 650a 2020 2020 6175 746f 2d68  n the.    auto-h
+000118b0: 6569 6768 7420 6973 2064 6973 6162 6c65  eight is disable
+000118c0: 642e 0a0a 2020 2020 4561 6368 2073 7472  d...    Each str
+000118d0: 696e 6720 6973 2063 656e 7465 7265 6420  ing is centered 
+000118e0: 6f6e 2074 6865 206c 6973 742e 2054 6869  on the list. Thi
+000118f0: 7320 6361 6e20 6265 2074 7765 616b 6564  s can be tweaked
+00011900: 2075 7369 6e67 2074 6865 0a20 2020 2060   using the.    `
+00011910: 6063 6f6c 756d 6e43 6f6e 6669 6760 6020  `columnConfig`` 
+00011920: 6172 6775 6d65 6e74 2e0a 0a20 2020 2054  argument...    T
+00011930: 6865 2073 7461 7465 2069 7320 6120 606c  he state is a `l
+00011940: 6973 7460 206f 6620 6073 7472 6020 7661  ist` of `str` va
+00011950: 6c75 6573 2c20 6076 6172 2e53 7472 696e  lues, `var.Strin
+00011960: 674c 6973 7460 2e0a 0a20 2020 2054 6869  gList`...    Thi
+00011970: 7320 6973 2061 2076 6172 6961 7469 6f6e  s is a variation
+00011980: 206f 6e20 7468 6520 6054 7265 6560 2077   on the `Tree` w
+00011990: 6964 6765 742c 2077 6974 6820 6120 7369  idget, with a si
+000119a0: 6e67 6c65 2063 6f6c 756d 6e2c 2061 2064  ngle column, a d
+000119b0: 6966 6665 7265 6e74 0a20 2020 2076 6172  ifferent.    var
+000119c0: 6961 626c 6520 7479 7065 2061 6e64 2073  iable type and s
+000119d0: 6f6d 6520 6f76 6572 7269 6465 6e20 6465  ome overriden de
+000119e0: 6661 756c 7420 7661 6c75 6573 2e0a 2020  fault values..  
+000119f0: 2020 5365 6520 616c 736f 2060 5079 7468    See also `Pyth
+00011a00: 6f6e 2074 746b 2e54 7265 6576 6965 7720  on ttk.Treeview 
+00011a10: 3c74 6b69 6e74 6572 2e74 746b 2e54 7265  <tkinter.ttk.Tre
+00011a20: 6576 6965 773e 6020 616e 6420 6060 546b  eview>` and ``Tk
+00011a30: 6060 0a20 2020 2060 7474 6b2e 5472 6565  ``.    `ttk.Tree
+00011a40: 7669 6577 203c 6874 7470 733a 2f2f 7463  view <https://tc
+00011a50: 6c2e 746b 2f6d 616e 2f74 636c 382e 362f  l.tk/man/tcl8.6/
+00011a60: 546b 436d 642f 7474 6b5f 7472 6565 7669  TkCmd/ttk_treevi
+00011a70: 6577 2e68 746d 6c3e 605f 0a20 2020 2064  ew.html>`_.    d
+00011a80: 6f63 756d 656e 7461 7469 6f6e 2e0a 0a20  ocumentation... 
+00011a90: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00011aa0: 2076 6172 6961 626c 653a 2055 7365 2061   variable: Use a
+00011ab0: 6e20 6578 7465 726e 616c 6c79 2064 6566  n externally def
+00011ac0: 696e 6564 2076 6172 6961 626c 652c 2069  ined variable, i
+00011ad0: 6e73 7465 6164 206f 6620 6372 6561 7469  nstead of creati
+00011ae0: 6e67 2061 206e 6577 0a20 2020 2020 2020  ng a new.       
+00011af0: 2020 2020 206f 6e65 2073 7065 6369 6669       one specifi
+00011b00: 6320 666f 7220 7468 6973 2077 6964 6765  c for this widge
+00011b10: 742e 0a20 2020 2020 2020 206c 6162 656c  t..        label
+00011b20: 3a20 5468 6520 6c61 6265 6c20 746f 2069  : The label to i
+00011b30: 6e63 6c75 6465 2062 6573 6964 6573 2074  nclude besides t
+00011b40: 6865 206c 6973 7462 6f78 2e20 4361 6e20  he listbox. Can 
+00011b50: 6265 2067 6976 656e 2061 7320 610a 2020  be given as a.  
+00011b60: 2020 2020 2020 2020 2020 636c 6173 7320            class 
+00011b70: 7661 7269 6162 6c65 2e0a 2020 2020 2020  variable..      
+00011b80: 2020 2020 2020 4f70 7469 6f6e 616c 2c20        Optional, 
+00011b90: 7768 656e 2067 6976 656e 2069 7320 7368  when given is sh
+00011ba0: 6f77 2061 7320 7468 6520 7369 6e67 6c65  ow as the single
+00011bb0: 2063 6f6c 756d 6e20 6865 6164 696e 672e   column heading.
+00011bc0: 0a20 2020 2020 2020 2063 6f6c 756d 6e43  .        columnC
+00011bd0: 6f6e 6669 673a 204f 7665 7272 6964 6520  onfig: Override 
+00011be0: 636f 6e66 6967 7572 6174 696f 6e20 666f  configuration fo
+00011bf0: 7220 7468 6520 7369 6e67 6c65 2063 6f6c  r the single col
+00011c00: 756d 6e2e 2041 6476 616e 6365 640a 2020  umn. Advanced.  
+00011c10: 2020 2020 2020 2020 2020 7573 6167 6520            usage 
+00011c20: 6f6e 6c79 2e0a 2020 2020 2020 2020 6865  only..        he
+00011c30: 6967 6874 3a20 4966 2067 6976 656e 2c20  ight: If given, 
+00011c40: 616c 7761 7973 2073 686f 7720 7468 6973  always show this
+00011c50: 2071 7561 6e74 6974 7920 6f66 2072 6f77   quantity of row
+00011c60: 732e 0a20 2020 2020 2020 2020 2020 2049  s..            I
+00011c70: 6620 6974 2069 7320 604e 6f6e 6560 2c20  f it is `None`, 
+00011c80: 7468 6520 6e75 6d62 6572 206f 6620 7065  the number of pe
+00011c90: 726d 616e 656e 746c 7920 7368 6f77 6e20  rmanently shown 
+00011ca0: 726f 7773 2077 696c 6c20 7661 7279 2062  rows will vary b
+00011cb0: 6574 7765 656e 0a20 2020 2020 2020 2020  etween.         
+00011cc0: 2020 2060 606d 696e 4865 6967 6874 6060     ``minHeight``
+00011cd0: 2061 6e64 2060 606d 6178 4865 6967 6874   and ``maxHeight
+00011ce0: 6060 2e0a 2020 2020 2020 2020 6d69 6e48  ``..        minH
+00011cf0: 6569 6768 743a 2049 6620 6060 6865 6967  eight: If ``heig
+00011d00: 6874 6060 2069 7320 604e 6f6e 6560 2c20  ht`` is `None`, 
+00011d10: 6d61 6b65 2073 7572 6520 7468 6973 206e  make sure this n
+00011d20: 756d 6265 7220 6f66 2072 6f77 7320 6973  umber of rows is
+00011d30: 0a20 2020 2020 2020 2020 2020 2061 6c77  .            alw
+00011d40: 6179 7320 7669 7369 626c 652e 0a20 2020  ays visible..   
+00011d50: 2020 2020 2020 2020 204f 7074 696f 6e61           Optiona
+00011d60: 6c2c 2077 6865 6e20 604e 6f6e 6560 2c20  l, when `None`, 
+00011d70: 7468 6572 6527 7320 6e6f 206c 6f77 6572  there's no lower
+00011d80: 206c 696d 6974 206f 6e20 7468 6520 7669   limit on the vi
+00011d90: 7369 626c 6520 6e75 6d62 6572 0a20 2020  sible number.   
+00011da0: 2020 2020 2020 2020 206f 6620 726f 7773           of rows
+00011db0: 2e0a 2020 2020 2020 2020 6d61 7848 6569  ..        maxHei
+00011dc0: 6768 743a 2049 6620 6060 6865 6967 6874  ght: If ``height
+00011dd0: 6060 2069 7320 604e 6f6e 6560 2c20 6d61  `` is `None`, ma
+00011de0: 6b65 2073 7572 6520 7468 6572 6520 6172  ke sure there ar
+00011df0: 6520 6e6f 206d 6f72 650a 2020 2020 2020  e no more.      
+00011e00: 2020 2020 2020 7669 7369 626c 6520 726f        visible ro
+00011e10: 7773 2074 6861 6e20 7468 6973 206e 756d  ws than this num
+00011e20: 6265 722e 0a20 2020 2020 2020 2020 2020  ber..           
+00011e30: 204f 7074 696f 6e61 6c2c 2077 6865 6e20   Optional, when 
+00011e40: 604e 6f6e 6560 2c20 7468 6572 6527 7320  `None`, there's 
+00011e50: 6e6f 2075 7070 6572 206c 696d 6974 206f  no upper limit o
+00011e60: 6e20 7468 6520 7669 7369 626c 650a 2020  n the visible.  
+00011e70: 2020 2020 2020 2020 2020 6e75 6d62 6572            number
+00011e80: 206f 6620 726f 7773 2e0a 2020 2020 2020   of rows..      
+00011e90: 2020 7365 6c65 6374 6162 6c65 3a20 5365    selectable: Se
+00011ea0: 6520 6054 7265 6560 2066 6f72 2069 7473  e `Tree` for its
+00011eb0: 206d 6561 6e69 6e67 2e0a 2020 2020 2020   meaning..      
+00011ec0: 2020 2020 2020 4465 6661 756c 7473 2074        Defaults t
+00011ed0: 6f20 6054 7275 6560 2e0a 2020 2020 2020  o `True`..      
+00011ee0: 2020 7374 796c 655f 616c 7462 673a 2053    style_altbg: S
+00011ef0: 6565 2060 5472 6565 6020 666f 7220 6974  ee `Tree` for it
+00011f00: 7320 6d65 616e 696e 672e 0a20 2020 2020  s meaning..     
+00011f10: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
+00011f20: 746f 2060 4661 6c73 6560 2e0a 2020 2020  to `False`..    
+00011f30: 2020 2020 6578 7061 6e64 3a20 5365 6520      expand: See 
+00011f40: 6054 7265 6560 2066 6f72 2069 7473 206d  `Tree` for its m
+00011f50: 6561 6e69 6e67 2e0a 2020 2020 2020 2020  eaning..        
+00011f60: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
+00011f70: 6046 616c 7365 602c 2062 7574 2069 6e74  `False`, but int
+00011f80: 6572 6163 7473 2077 6974 6820 7468 6520  eracts with the 
+00011f90: 6175 746f 2d68 6569 6768 7420 7365 7474  auto-height sett
+00011fa0: 696e 6773 2e0a 2020 2020 2020 2020 7374  ings..        st
+00011fb0: 796c 653a 2043 6f6e 6669 6775 7265 2074  yle: Configure t
+00011fc0: 6865 2077 6964 6765 7420 7374 796c 652e  he widget style.
+00011fd0: 0a0a 2020 2020 2020 2020 7061 7265 6e74  ..        parent
+00011fe0: 3a20 5468 6520 7061 7265 6e74 2077 6964  : The parent wid
+00011ff0: 6765 742e 2043 616e 2062 6520 6120 6052  get. Can be a `R
+00012000: 6f6f 7457 696e 646f 7760 206f 7220 616e  ootWindow` or an
+00012010: 6f74 6865 7220 606d 6978 696e 2e43 6f6e  other `mixin.Con
+00012020: 7461 696e 6572 5769 6467 6574 602e 0a20  tainerWidget`.. 
+00012030: 2020 2027 2727 0a20 2020 206c 6162 656c     '''.    label
+00012040: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+00012050: 6c5b 7374 725d 203d 204e 6f6e 650a 0a20  l[str] = None.. 
+00012060: 2020 2040 6461 7461 636c 6173 730a 2020     @dataclass.  
+00012070: 2020 636c 6173 7320 5374 796c 6528 5472    class Style(Tr
+00012080: 6565 2e53 7479 6c65 293a 0a20 2020 2020  ee.Style):.     
+00012090: 2020 2027 2727 604c 6973 7462 6f78 6020     '''`Listbox` 
+000120a0: 7374 796c 6520 6f62 6a65 6374 2e0a 0a20  style object... 
+000120b0: 2020 2020 2020 2053 6565 2060 5472 6565         See `Tree
+000120c0: 2e53 7479 6c65 6020 666f 7220 7570 7374  .Style` for upst
+000120d0: 7265 616d 2076 616c 7565 732c 2074 6865  ream values, the
+000120e0: 7365 2061 7265 2074 6865 2064 6966 6665  se are the diffe
+000120f0: 7265 6e63 6573 3a0a 0a20 2020 2020 2020  rences:..       
+00012100: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00012110: 2020 2061 6c74 6267 3a20 4469 7361 626c     altbg: Disabl
+00012120: 6564 2062 7920 6465 6661 756c 742e 0a20  ed by default.. 
+00012130: 2020 2020 2020 2020 2020 2073 686f 775f             show_
+00012140: 6c61 6265 6c73 3a20 556e 7375 7070 6f72  labels: Unsuppor
+00012150: 7465 642e 0a20 2020 2020 2020 2027 2727  ted..        '''
+00012160: 0a20 2020 2020 2020 2061 6c74 6267 3a20  .        altbg: 
+00012170: 626f 6f6c 203d 2046 616c 7365 0a20 2020  bool = False.   
+00012180: 2020 2020 2073 686f 775f 6c61 6265 6c73       show_labels
+00012190: 3a20 626f 6f6c 203d 2046 616c 7365 0a0a  : bool = False..
+000121a0: 2020 2020 2020 2020 6966 205f 5f64 6562          if __deb
+000121b0: 7567 5f5f 3a0a 2020 2020 2020 2020 2020  ug__:.          
+000121c0: 2020 6465 6620 5f5f 706f 7374 5f69 6e69    def __post_ini
+000121d0: 745f 5f28 7365 6c66 293a 0a20 2020 2020  t__(self):.     
+000121e0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+000121f0: 6c66 2e73 686f 775f 6c61 6265 6c73 3a0a  lf.show_labels:.
+00012200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012210: 2020 2020 7761 726e 696e 6773 2e77 6172      warnings.war
+00012220: 6e28 6627 7b73 656c 667d 3a20 556e 7375  n(f'{self}: Unsu
+00012230: 7070 6f72 7465 6420 2273 686f 775f 6c61  pported "show_la
+00012240: 6265 6c73 2227 2c20 7374 6163 6b6c 6576  bels"', stacklev
+00012250: 656c 3d33 290a 2020 2020 2020 2020 2020  el=3).          
+00012260: 2020 2020 2020 7365 6c66 2e73 686f 775f        self.show_
+00012270: 6c61 6265 6c73 203d 2046 616c 7365 0a0a  labels = False..
+00012280: 2020 2020 7374 6174 655f 7479 7065 203d      state_type =
+00012290: 2076 6172 2e53 7472 696e 674c 6973 7420   var.StringList 
+000122a0: 2023 2074 7970 653a 2069 676e 6f72 6520   # type: ignore 
+000122b0: 2023 2043 6861 6e67 6520 7468 6520 7661   # Change the va
+000122c0: 7269 6162 6c65 2074 7970 650a 0a20 2020  riable type..   
+000122d0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+000122e0: 6c66 2c20 2a61 7267 732c 2076 6172 6961  lf, *args, varia
+000122f0: 626c 653a 2074 7970 696e 672e 4f70 7469  ble: typing.Opti
+00012300: 6f6e 616c 5b76 6172 2e53 7472 696e 674c  onal[var.StringL
+00012310: 6973 745d 203d 204e 6f6e 652c 0a20 2020  ist] = None,.   
+00012320: 2020 2020 2020 2020 2020 2020 2020 6c61                la
+00012330: 6265 6c3a 2074 7970 696e 672e 4f70 7469  bel: typing.Opti
+00012340: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00012350: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00012360: 2020 2063 6f6c 756d 6e43 6f6e 6669 673a     columnConfig:
+00012370: 2074 7970 696e 672e 4d61 7070 696e 675b   typing.Mapping[
+00012380: 7374 722c 2074 7970 696e 672e 416e 795d  str, typing.Any]
+00012390: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+000123a0: 2020 2020 2020 2020 2020 6865 6967 6874            height
+000123b0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+000123c0: 6c5b 696e 745d 203d 204e 6f6e 652c 206d  l[int] = None, m
+000123d0: 696e 4865 6967 6874 3a20 7479 7069 6e67  inHeight: typing
+000123e0: 2e4f 7074 696f 6e61 6c5b 696e 745d 203d  .Optional[int] =
+000123f0: 204e 6f6e 652c 206d 6178 4865 6967 6874   None, maxHeight
+00012400: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+00012410: 6c5b 696e 745d 203d 204e 6f6e 652c 0a20  l[int] = None,. 
+00012420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012430: 7365 6c65 6374 6162 6c65 3a20 626f 6f6c  selectable: bool
+00012440: 203d 2054 7275 652c 2065 7870 616e 643a   = True, expand:
+00012450: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00012460: 5b62 6f6f 6c5d 203d 204e 6f6e 652c 2020  [bool] = None,  
+00012470: 2320 4f76 6572 7269 6465 0a20 2020 2020  # Override.     
+00012480: 2020 2020 2020 2020 2020 2020 7374 796c              styl
+00012490: 653a 2053 7479 6c65 203d 2053 7479 6c65  e: Style = Style
+000124a0: 285f 6465 6661 756c 743d 5472 7565 292c  (_default=True),
+000124b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000124c0: 2020 2a2a 6b77 6172 6773 293a 0a20 2020    **kwargs):.   
+000124d0: 2020 2020 2063 686f 7365 6e5f 6c61 6265       chosen_labe
+000124e0: 6c20 3d20 7365 6c66 2e6c 6162 656c 206f  l = self.label o
+000124f0: 7220 6c61 6265 6c0a 2020 2020 2020 2020  r label.        
+00012500: 6966 2073 7479 6c65 2e5f 6465 6661 756c  if style._defaul
+00012510: 743a 0a20 2020 2020 2020 2020 2020 2073  t:.            s
+00012520: 7479 6c65 2e73 686f 775f 6865 6164 696e  tyle.show_headin
+00012530: 6773 203d 2063 686f 7365 6e5f 6c61 6265  gs = chosen_labe
+00012540: 6c20 6973 206e 6f74 204e 6f6e 650a 2020  l is not None.  
+00012550: 2020 2020 2020 6b77 6172 6773 2e75 7064        kwargs.upd
+00012560: 6174 6528 7b0a 2020 2020 2020 2020 2020  ate({.          
+00012570: 2020 276c 6162 656c 273a 2063 686f 7365    'label': chose
+00012580: 6e5f 6c61 6265 6c2c 0a20 2020 2020 2020  n_label,.       
+00012590: 2020 2020 2027 7661 7269 6162 6c65 273a       'variable':
+000125a0: 2076 6172 6961 626c 652c 0a20 2020 2020   variable,.     
+000125b0: 2020 2020 2020 2027 7365 6c65 6374 6162         'selectab
+000125c0: 6c65 273a 2073 656c 6563 7461 626c 652c  le': selectable,
+000125d0: 2020 2320 4f76 6572 7269 6465 0a20 2020    # Override.   
+000125e0: 2020 2020 2020 2020 2027 636f 6c75 6d6e           'column
+000125f0: 7327 3a20 7b27 6c61 6265 6c27 3a20 6368  s': {'label': ch
+00012600: 6f73 656e 5f6c 6162 656c 206f 7220 274c  osen_label or 'L
+00012610: 6162 656c 277d 2c20 2023 2053 696e 676c  abel'},  # Singl
+00012620: 6520 436f 6c75 6d6e 2022 6c61 6265 6c22  e Column "label"
+00012630: 0a20 2020 2020 2020 2020 2020 2027 7374  .            'st
+00012640: 796c 6527 3a20 7374 796c 652c 0a20 2020  yle': style,.   
+00012650: 2020 2020 207d 290a 2020 2020 2020 2020       }).        
+00012660: 2320 436f 6e66 6967 7572 6520 6865 6967  # Configure heig
+00012670: 6874 0a20 2020 2020 2020 2073 656c 662e  ht.        self.
+00012680: 6865 6967 6874 5261 6e67 653a 2074 7970  heightRange: typ
+00012690: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
+000126a0: 696e 672e 5475 706c 655b 7479 7069 6e67  ing.Tuple[typing
+000126b0: 2e4f 7074 696f 6e61 6c5b 696e 745d 2c20  .Optional[int], 
+000126c0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+000126d0: 696e 745d 5d5d 0a20 2020 2020 2020 2069  int]]].        i
+000126e0: 6620 6865 6967 6874 2069 7320 4e6f 6e65  f height is None
+000126f0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00012700: 6c66 2e68 6569 6768 7452 616e 6765 203d  lf.heightRange =
+00012710: 206d 696e 4865 6967 6874 2c20 6d61 7848   minHeight, maxH
+00012720: 6569 6768 740a 2020 2020 2020 2020 656c  eight.        el
+00012730: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00012740: 6b77 6172 6773 5b27 6865 6967 6874 275d  kwargs['height']
+00012750: 203d 2068 6569 6768 7420 2023 2048 6172   = height  # Har
+00012760: 6463 6f64 6520 7468 6520 6865 6967 6874  dcode the height
+00012770: 2076 616c 7565 0a20 2020 2020 2020 2020   value.         
+00012780: 2020 2073 656c 662e 6865 6967 6874 5261     self.heightRa
+00012790: 6e67 6520 3d20 4e6f 6e65 0a20 2020 2020  nge = None.     
+000127a0: 2020 2069 6620 6865 6967 6874 206f 7220     if height or 
+000127b0: 6d69 6e48 6569 6768 7420 6f72 206d 6178  minHeight or max
+000127c0: 4865 6967 6874 2061 6e64 2065 7870 616e  Height and expan
+000127d0: 6420 6973 204e 6f6e 653a 0a20 2020 2020  d is None:.     
+000127e0: 2020 2020 2020 2023 2044 6f6e 2774 2065         # Don't e
+000127f0: 7870 616e 6420 7768 656e 2074 6865 2066  xpand when the f
+00012800: 6978 6564 206f 7220 7661 7279 696e 6720  ixed or varying 
+00012810: 6865 6967 6874 2069 7320 7365 740a 2020  height is set.  
+00012820: 2020 2020 2020 2020 2020 6578 7061 6e64            expand
+00012830: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
+00012840: 2023 2043 6f6e 6669 6775 7265 2028 7369   # Configure (si
+00012850: 6e67 6c65 2920 636f 6c75 6d6e 0a20 2020  ngle) column.   
+00012860: 2020 2020 2023 202d 2044 6f6e 2774 2075       # - Don't u
+00012870: 7365 2060 2330 6020 7369 6e63 6520 7468  se `#0` since th
+00012880: 6174 2069 7320 6e6f 7420 7072 6f70 6572  at is not proper
+00012890: 6c79 2063 656e 7465 7265 642c 2069 7420  ly centered, it 
+000128a0: 6861 7320 7468 6520 7472 6565 0a20 2020  has the tree.   
+000128b0: 2020 2020 2023 2020 2065 6c65 6d65 6e74       #   element
+000128c0: 7320 696e 2074 6865 7265 2c20 6576 656e  s in there, even
+000128d0: 2068 6964 6465 6e2e 0a20 2020 2020 2020   hidden..       
+000128e0: 2063 436f 6e66 6967 203d 207b 0a20 2020   cConfig = {.   
+000128f0: 2020 2020 2020 2020 2027 616e 6368 6f72           'anchor
+00012900: 273a 2074 6b2e 4345 4e54 4552 2c0a 2020  ': tk.CENTER,.  
+00012910: 2020 2020 2020 2020 2020 2773 7472 6574            'stret
+00012920: 6368 273a 2054 7275 652c 0a20 2020 2020  ch': True,.     
+00012930: 2020 207d 0a20 2020 2020 2020 2069 6620     }.        if 
+00012940: 6578 7061 6e64 2069 7320 6e6f 7420 4e6f  expand is not No
+00012950: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00012960: 6b77 6172 6773 5b27 6578 7061 6e64 275d  kwargs['expand']
+00012970: 203d 2065 7870 616e 640a 2020 2020 2020   = expand.      
+00012980: 2020 6966 2063 6f6c 756d 6e43 6f6e 6669    if columnConfi
+00012990: 673a 0a20 2020 2020 2020 2020 2020 2063  g:.            c
+000129a0: 436f 6e66 6967 2e75 7064 6174 6528 636f  Config.update(co
+000129b0: 6c75 6d6e 436f 6e66 6967 290a 2020 2020  lumnConfig).    
+000129c0: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
+000129d0: 6974 5f5f 282a 6172 6773 2c20 2a2a 6b77  it__(*args, **kw
+000129e0: 6172 6773 290a 2020 2020 2020 2020 2320  args).        # 
+000129f0: 4d61 6b65 2073 7572 6520 6343 6f6e 6669  Make sure cConfi
+00012a00: 6720 6b65 7973 206d 6174 6368 206f 7074  g keys match opt
+00012a10: 696f 6e73 2066 6f72 2060 746b 696e 7465  ions for `tkinte
+00012a20: 722e 7474 6b2e 5472 6565 7669 6577 2e63  r.ttk.Treeview.c
+00012a30: 6f6c 756d 6e60 0a20 2020 2020 2020 2073  olumn`.        s
+00012a40: 656c 662e 636f 6c75 6d6e 2827 6c61 6265  elf.column('labe
+00012a50: 6c27 2c20 2a2a 6343 6f6e 6669 6729 2020  l', **cConfig)  
+00012a60: 2320 7479 7065 3a20 6967 6e6f 7265 0a0a  # type: ignore..
+00012a70: 2020 2020 6465 6620 5f74 7265 655f 6765      def _tree_ge
+00012a80: 7428 7365 6c66 2c20 7661 7269 6162 6c65  t(self, variable
+00012a90: 3a20 7661 722e 5661 7269 6162 6c65 2920  : var.Variable) 
+00012aa0: 2d3e 2074 7970 696e 672e 5365 7175 656e  -> typing.Sequen
+00012ab0: 6365 5b6d 6f64 656c 2e54 7265 6545 6c65  ce[model.TreeEle
+00012ac0: 6d65 6e74 5d3a 0a20 2020 2020 2020 2072  ment]:.        r
+00012ad0: 6574 7572 6e20 5b6d 6f64 656c 2e54 7265  eturn [model.Tre
+00012ae0: 6545 6c65 6d65 6e74 286c 6162 656c 3d65  eElement(label=e
+00012af0: 2c20 636f 6c75 6d6e 733d 5b65 5d2c 2064  , columns=[e], d
+00012b00: 6174 613d 6529 2066 6f72 2065 2069 6e20  ata=e) for e in 
+00012b10: 7661 7269 6162 6c65 2e67 6574 2829 5d0a  variable.get()].
+00012b20: 0a20 2020 2064 6566 205f 7472 6565 5f6f  .    def _tree_o
+00012b30: 6e73 6574 2873 656c 662c 2076 616c 7565  nset(self, value
+00012b40: 3a20 7479 7069 6e67 2e53 6571 7565 6e63  : typing.Sequenc
+00012b50: 655b 6d6f 6465 6c2e 5472 6565 456c 656d  e[model.TreeElem
+00012b60: 656e 745d 2920 2d3e 204e 6f6e 653a 0a20  ent]) -> None:. 
+00012b70: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
+00012b80: 6569 6768 7452 616e 6765 2069 7320 6e6f  eightRange is no
+00012b90: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00012ba0: 2020 2020 6d69 6e48 6569 6768 742c 206d      minHeight, m
+00012bb0: 6178 4865 6967 6874 203d 2073 656c 662e  axHeight = self.
+00012bc0: 6865 6967 6874 5261 6e67 650a 2020 2020  heightRange.    
+00012bd0: 2020 2020 2020 2020 7773 697a 6520 3d20          wsize = 
+00012be0: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+00012bf0: 2069 6620 6d69 6e48 6569 6768 743a 0a20   if minHeight:. 
+00012c00: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00012c10: 7369 7a65 203d 206d 6178 286d 696e 4865  size = max(minHe
+00012c20: 6967 6874 2c20 6c65 6e28 7661 6c75 6529  ight, len(value)
+00012c30: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00012c40: 206d 6178 4865 6967 6874 3a0a 2020 2020   maxHeight:.    
+00012c50: 2020 2020 2020 2020 2020 2020 7773 697a              wsiz
+00012c60: 6520 3d20 6d69 6e28 6d61 7848 6569 6768  e = min(maxHeigh
+00012c70: 742c 2077 7369 7a65 206f 7220 6c65 6e28  t, wsize or len(
+00012c80: 7661 6c75 6529 290a 2020 2020 2020 2020  value)).        
+00012c90: 2020 2020 6966 2077 7369 7a65 3a0a 2020      if wsize:.  
+00012ca0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00012cb0: 205f 5f64 6562 7567 5f5f 3a0a 2020 2020   __debug__:.    
+00012cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012cd0: 6c6f 6767 6572 2e64 6562 7567 2866 277b  logger.debug(f'{
+00012ce0: 7365 6c66 7d3a 2041 7574 6f20 4865 6967  self}: Auto Heig
+00012cf0: 6874 3a20 7b77 7369 7a65 7d27 290a 2020  ht: {wsize}').  
+00012d00: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00012d10: 6c66 2e63 6f6e 6669 6775 7265 2868 6569  lf.configure(hei
+00012d20: 6768 743d 7773 697a 6529 0a0a 0a63 6c61  ght=wsize)...cla
+00012d30: 7373 2046 7261 6d65 5061 6e65 6428 7474  ss FramePaned(tt
+00012d40: 6b2e 5061 6e65 6457 696e 646f 772c 206d  k.PanedWindow, m
+00012d50: 6978 696e 2e43 6f6e 7461 696e 6572 5769  ixin.ContainerWi
+00012d60: 6467 6574 293a 0a20 2020 2027 2727 4120  dget):.    '''A 
+00012d70: 6672 616d 6520 746f 2068 6f6c 6420 6f74  frame to hold ot
+00012d80: 6865 7220 7769 6467 6574 732c 2077 6974  her widgets, wit
+00012d90: 6820 7573 6572 2d63 6f6e 7472 6f6c 6c61  h user-controlla
+00012da0: 626c 6520 7265 6c61 7469 7665 2073 697a  ble relative siz
+00012db0: 6573 2e0a 0a20 2020 2054 6869 7320 6973  es...    This is
+00012dc0: 2073 696d 696c 6172 2074 6f20 6120 6046   similar to a `F
+00012dd0: 7261 6d65 556e 6c61 6265 6c6c 6564 602c  rameUnlabelled`,
+00012de0: 2072 6573 7472 6963 7465 6420 746f 2068   restricted to h
+00012df0: 6f72 697a 6f6e 7461 6c20 6f72 0a20 2020  orizontal or.   
+00012e00: 2076 6572 7469 6361 6c20 6c61 796f 7574   vertical layout
+00012e10: 732c 2062 7574 2077 6865 7265 2074 6865  s, but where the
+00012e20: 2069 6e74 6572 6661 6365 7320 6265 7477   interfaces betw
+00012e30: 6565 6e20 7468 6520 6368 696c 6472 656e  een the children
+00012e40: 2063 616e 2062 650a 2020 2020 6164 6a75   can be.    adju
+00012e50: 7374 6564 2062 7920 7468 6520 7573 6572  sted by the user
+00012e60: 2c20 746f 2072 6573 697a 6520 7468 656d  , to resize them
+00012e70: 2061 7420 7769 6c6c 2e0a 0a20 2020 2054   at will...    T
+00012e80: 6869 7320 616c 6c6f 7773 2073 6f6d 6520  his allows some 
+00012e90: 6368 696c 6420 7769 6467 6574 7320 746f  child widgets to
+00012ea0: 2062 6520 6869 6464 656e 2c20 6279 2072   be hidden, by r
+00012eb0: 6573 697a 696e 6720 7468 6520 6f74 6865  esizing the othe
+00012ec0: 7220 7061 6e65 7320 746f 0a20 2020 2066  r panes to.    f
+00012ed0: 756c 6c79 206f 6363 7570 7920 7468 6520  ully occupy the 
+00012ee0: 7769 6467 6574 2061 7265 612e 0a0a 2020  widget area...  
+00012ef0: 2020 4e6f 7465 2074 6861 7420 7573 696e    Note that usin
+00012f00: 6720 7468 6973 2077 6974 6820 6d6f 7265  g this with more
+00012f10: 2074 6861 6e20 7477 6f20 6368 696c 6472   than two childr
+00012f20: 656e 2063 616e 2062 6520 636f 6e66 7573  en can be confus
+00012f30: 696e 6720 666f 7220 7468 650a 2020 2020  ing for the.    
+00012f40: 7573 6572 732c 2070 6172 7469 6375 6c61  users, particula
+00012f50: 726c 7920 7768 656e 2072 6573 697a 696e  rly when resizin
+00012f60: 6720 7461 6b65 7320 706c 6163 652e 0a0a  g takes place...
+00012f70: 2020 2020 5468 6572 6520 6973 206e 6f20      There is no 
+00012f80: 5079 7468 6f6e 2064 6f63 756d 656e 7461  Python documenta
+00012f90: 7469 6f6e 2c20 7365 6520 6060 546b 6060  tion, see ``Tk``
+00012fa0: 2060 7474 6b2e 5061 6e65 6457 696e 646f   `ttk.PanedWindo
+00012fb0: 7720 3c68 7474 7073 3a2f 2f77 7777 2e74  w <https://www.t
+00012fc0: 636c 2e74 6b2f 6d61 6e2f 7463 6c2f 546b  cl.tk/man/tcl/Tk
+00012fd0: 436d 642f 7474 6b5f 7061 6e65 6477 696e  Cmd/ttk_panedwin
+00012fe0: 646f 772e 6874 6d6c 3e60 5f20 646f 6375  dow.html>`_ docu
+00012ff0: 6d65 6e74 6174 696f 6e2e 0a0a 2020 2020  mentation...    
+00013000: 4172 6773 3a0a 2020 2020 2020 2020 6c61  Args:.        la
+00013010: 796f 7574 3a20 5468 6520 6f72 6965 6e74  yout: The orient
+00013020: 6174 696f 6e20 6f66 2074 6865 2063 6869  ation of the chi
+00013030: 6c64 2077 6964 6765 7473 2e0a 2020 2020  ld widgets..    
+00013040: 2020 2020 2020 2020 5265 7374 7269 6374          Restrict
+00013050: 6564 2074 6f20 6060 746b 2e56 4552 5449  ed to ``tk.VERTI
+00013060: 4341 4c60 6020 6f72 2060 6074 6b2e 484f  CAL`` or ``tk.HO
+00013070: 5249 5a4f 4e54 414c 6060 2e0a 2020 2020  RIZONTAL``..    
+00013080: 2020 2020 6f72 6965 6e74 3a20 416c 6961      orient: Alia
+00013090: 7320 666f 7220 226c 6179 6f75 7422 2e0a  s for "layout"..
+000130a0: 2020 2020 2020 2020 7765 6967 6874 3a20          weight: 
+000130b0: 5468 6520 7765 6967 6874 2066 6f72 2065  The weight for e
+000130c0: 6163 6820 6368 696c 6472 656e 2077 6964  ach children wid
+000130d0: 6765 742e 204f 7074 696f 6e61 6c2c 2064  get. Optional, d
+000130e0: 6566 6175 6c74 7320 746f 2031 2e0a 2020  efaults to 1..  
+000130f0: 2020 2020 2020 7765 6967 6874 733a 2050        weights: P
+00013100: 6572 2d63 6869 6c64 2077 6964 6765 742e  er-child widget.
+00013110: 204f 7074 696f 6e61 6c2c 2064 6566 6175   Optional, defau
+00013120: 6c74 7320 746f 2074 6865 2063 6f6d 6d6f  lts to the commo
+00013130: 6e20 2277 6569 6768 7422 2e0a 0a20 2020  n "weight"...   
+00013140: 204e 6f74 653a 0a20 2020 2020 2020 2054   Note:.        T
+00013150: 6865 2060 606c 6179 6f75 7460 602f 6060  he ``layout``/``
+00013160: 6f72 6965 6e74 6060 2061 7267 756d 656e  orient`` argumen
+00013170: 7420 6861 7320 7369 6d69 6c61 7220 7365  t has similar se
+00013180: 6d61 6e74 6963 7320 746f 2060 606c 6179  mantics to ``lay
+00013190: 6f75 7460 600a 2020 2020 2020 2020 6172  out``.        ar
+000131a0: 6775 6d65 6e74 206f 6e20 6f74 6865 7220  gument on other 
+000131b0: 6672 616d 6520 7479 7065 732e 0a0a 2020  frame types...  
+000131c0: 2020 5365 6520 416c 736f 3a0a 2020 2020    See Also:.    
+000131d0: 2020 2020 2d20 6046 7261 6d65 556e 6c61      - `FrameUnla
+000131e0: 6265 6c6c 6564 602c 2060 4672 616d 654c  belled`, `FrameL
+000131f0: 6162 656c 6c65 6460 3a20 5369 6d69 6c61  abelled`: Simila
+00013200: 7220 7665 7273 696f 6e73 2c20 7769 7468  r versions, with
+00013210: 6f75 7420 7573 6572 0a20 2020 2020 2020  out user.       
+00013220: 2020 2063 6f6e 7472 6f6c 206f 7665 7220     control over 
+00013230: 7369 7a69 6e67 2e0a 2020 2020 2727 270a  sizing..    '''.
+00013240: 2020 2020 6c61 796f 7574 3a20 7479 7069      layout: typi
+00013250: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
+00013260: 203d 204e 6f6e 650a 0a20 2020 2064 6566   = None..    def
+00013270: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+00013280: 7061 7265 6e74 2c0a 2020 2020 2020 2020  parent,.        
+00013290: 2020 2020 2020 2020 202a 6172 6773 2c0a           *args,.
+000132a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000132b0: 206f 7269 656e 743a 2074 7970 696e 672e   orient: typing.
+000132c0: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
+000132d0: 556e 696f 6e5b 7479 7069 6e67 2e4c 6974  Union[typing.Lit
+000132e0: 6572 616c 5b27 7665 7274 6963 616c 275d  eral['vertical']
+000132f0: 2c20 7479 7069 6e67 2e4c 6974 6572 616c  , typing.Literal
+00013300: 5b27 686f 7269 7a6f 6e74 616c 275d 5d5d  ['horizontal']]]
+00013310: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00013320: 2020 2020 2020 2020 2020 7765 6967 6874            weight
+00013330: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+00013340: 6c5b 696e 745d 203d 204e 6f6e 652c 0a20  l[int] = None,. 
+00013350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013360: 7765 6967 6874 733a 2074 7970 696e 672e  weights: typing.
+00013370: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
+00013380: 4d61 7070 696e 675b 7374 722c 2069 6e74  Mapping[str, int
+00013390: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
+000133a0: 2020 2020 2020 2020 2020 2020 2a2a 6b77              **kw
+000133b0: 6172 6773 293a 0a20 2020 2020 2020 2023  args):.        #
+000133c0: 204f 7269 656e 7461 7469 6f6e 2063 616e   Orientation can
+000133d0: 2062 6520 6769 7665 6e20 6173 2074 6865   be given as the
+000133e0: 206c 6179 6f75 740a 2020 2020 2020 2020   layout.        
+000133f0: 2320 4275 7420 7468 6520 436f 6e74 6169  # But the Contai
+00013400: 6e65 7257 6964 6765 7420 6c61 796f 7574  nerWidget layout
+00013410: 2069 7320 616c 7761 7973 204e 6f6e 650a   is always None.
+00013420: 2020 2020 2020 2020 2320 4e6f 2044 6566          # No Def
+00013430: 6175 6c74 204f 7269 656e 7461 7469 6f6e  ault Orientation
+00013440: 2c20 6d75 7374 2062 6520 6769 7665 6e20  , must be given 
+00013450: 736f 6d65 7768 6572 650a 2020 2020 2020  somewhere.      
+00013460: 2020 6f72 6965 6e74 6174 696f 6e20 3d20    orientation = 
+00013470: 6b77 6172 6773 2e70 6f70 2827 6c61 796f  kwargs.pop('layo
+00013480: 7574 272c 204e 6f6e 6529 206f 7220 6f72  ut', None) or or
+00013490: 6965 6e74 206f 7220 7365 6c66 2e6c 6179  ient or self.lay
+000134a0: 6f75 740a 2020 2020 2020 2020 6173 7365  out.        asse
+000134b0: 7274 206f 7269 656e 7461 7469 6f6e 2069  rt orientation i
+000134c0: 6e20 5b74 6b2e 5645 5254 4943 414c 2c20  n [tk.VERTICAL, 
+000134d0: 746b 2e48 4f52 495a 4f4e 5441 4c5d 2c20  tk.HORIZONTAL], 
+000134e0: 6627 496e 7661 6c69 6420 4f72 6965 6e74  f'Invalid Orient
+000134f0: 6174 696f 6e3a 207b 6f72 6965 6e74 6174  ation: {orientat
+00013500: 696f 6e7d 270a 2020 2020 2020 2020 6966  ion}'.        if
+00013510: 2074 7970 696e 672e 5459 5045 5f43 4845   typing.TYPE_CHE
+00013520: 434b 494e 473a 0a20 2020 2020 2020 2020  CKING:.         
+00013530: 2020 206f 7269 656e 7461 7469 6f6e 203d     orientation =
+00013540: 2074 7970 696e 672e 6361 7374 2874 7970   typing.cast(typ
+00013550: 696e 672e 556e 696f 6e5b 7479 7069 6e67  ing.Union[typing
+00013560: 2e4c 6974 6572 616c 5b27 7665 7274 6963  .Literal['vertic
+00013570: 616c 275d 2c20 7479 7069 6e67 2e4c 6974  al'], typing.Lit
+00013580: 6572 616c 5b27 686f 7269 7a6f 6e74 616c  eral['horizontal
+00013590: 275d 5d2c 206f 7269 656e 7461 7469 6f6e  ']], orientation
+000135a0: 290a 2020 2020 2020 2020 7375 7065 7228  ).        super(
+000135b0: 292e 5f5f 696e 6974 5f5f 2870 6172 656e  ).__init__(paren
+000135c0: 742c 206f 7269 656e 743d 6f72 6965 6e74  t, orient=orient
+000135d0: 6174 696f 6e29 2020 2320 7474 6b2e 5061  ation)  # ttk.Pa
+000135e0: 6e65 6457 696e 646f 770a 2020 2020 2020  nedWindow.      
+000135f0: 2020 7365 6c66 2e69 6e69 745f 636f 6e74    self.init_cont
+00013600: 6169 6e65 7228 2a61 7267 732c 206c 6179  ainer(*args, lay
+00013610: 6f75 743d 4e6f 6e65 2c20 2a2a 6b77 6172  out=None, **kwar
+00013620: 6773 290a 2020 2020 2020 2020 666f 7220  gs).        for 
+00013630: 776e 616d 652c 2077 6964 6765 7420 696e  wname, widget in
+00013640: 2073 656c 662e 7769 6467 6574 732e 6974   self.widgets.it
+00013650: 656d 7328 293a 0a20 2020 2020 2020 2020  ems():.         
+00013660: 2020 2023 2057 6964 6765 7420 5765 6967     # Widget Weig
+00013670: 6874 3a20 4465 6661 756c 7420 746f 2031  ht: Default to 1
+00013680: 0a20 2020 2020 2020 2020 2020 2077 7765  .            wwe
+00013690: 6967 6874 203d 2077 6569 6768 7420 6f72  ight = weight or
+000136a0: 2031 0a20 2020 2020 2020 2020 2020 2069   1.            i
+000136b0: 6620 7765 6967 6874 733a 0a20 2020 2020  f weights:.     
+000136c0: 2020 2020 2020 2020 2020 2023 2050 6572             # Per
+000136d0: 2d57 6964 6765 7420 4f76 6572 7269 6465  -Widget Override
+000136e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000136f0: 2077 7765 6967 6874 203d 2077 6569 6768   wweight = weigh
+00013700: 7473 2e67 6574 2877 6e61 6d65 2c20 7777  ts.get(wname, ww
+00013710: 6569 6768 7429 0a20 2020 2020 2020 2020  eight).         
+00013720: 2020 2061 7373 6572 7420 6973 696e 7374     assert isinst
+00013730: 616e 6365 2877 6964 6765 742c 2074 6b2e  ance(widget, tk.
+00013740: 5769 6467 6574 290a 2020 2020 2020 2020  Widget).        
+00013750: 2020 2020 7365 6c66 2e61 6464 2877 6964      self.add(wid
+00013760: 6765 742c 0a20 2020 2020 2020 2020 2020  get,.           
+00013770: 2020 2020 2020 2020 2020 7765 6967 6874            weight
+00013780: 3d77 7765 6967 6874 290a 2020 2020 2020  =wweight).      
+00013790: 2020 6173 7365 7274 206c 656e 2873 656c    assert len(sel
+000137a0: 662e 7061 6e65 7328 2929 203d 3d20 6c65  f.panes()) == le
+000137b0: 6e28 7365 6c66 2e77 6964 6765 7473 290a  n(self.widgets).
+000137c0: 0a0a 2320 544f 444f 3a20 5375 7070 6f72  ..# TODO: Suppor
+000137d0: 7420 6175 746f 2073 6372 6f6c 6c20 2868  t auto scroll (h
+000137e0: 6964 6520 7363 726f 6c6c 6261 7273 2077  ide scrollbars w
+000137f0: 6865 6e20 7363 726f 6c6c 636f 6d6d 616e  hen scrollcomman
+00013800: 6420 6973 2063 616c 6c65 6420 6173 2060  d is called as `
+00013810: 7365 7428 2730 2e30 272c 2027 312e 3027  set('0.0', '1.0'
+00013820: 2960 290a 636c 6173 7320 5363 726f 6c6c  )`).class Scroll
+00013830: 6564 5769 6467 6574 2874 746b 2e46 7261  edWidget(ttk.Fra
+00013840: 6d65 2c20 6d69 7869 6e2e 5369 6e67 6c65  me, mixin.Single
+00013850: 5769 6467 6574 293a 0a20 2020 2027 2727  Widget):.    '''
+00013860: 4120 7369 6e67 6c65 2077 6964 6765 7420  A single widget 
+00013870: 6672 616d 6520 7772 6170 7065 722c 2074  frame wrapper, t
+00013880: 6f20 696e 636c 7564 6520 6675 6e63 7469  o include functi
+00013890: 6f6e 616c 2073 6372 6f6c 6c62 6172 732e  onal scrollbars.
+000138a0: 0a0a 2020 2020 5468 6973 2069 7320 6120  ..    This is a 
+000138b0: 7772 6170 7065 7220 6672 616d 652c 2077  wrapper frame, w
+000138c0: 6974 6820 6120 7369 6e67 6c65 2063 6869  ith a single chi
+000138d0: 6c64 2077 6964 6765 742c 2077 6869 6368  ld widget, which
+000138e0: 2069 6e63 6c75 6465 730a 2020 2020 6675   includes.    fu
+000138f0: 6e63 7469 6f6e 616c 2073 6372 6f6c 6c62  nctional scrollb
+00013900: 6172 732e 2042 6f74 6820 686f 7269 7a6f  ars. Both horizo
+00013910: 6e74 616c 2061 6e64 2076 6572 7469 6361  ntal and vertica
+00013920: 6c20 7363 726f 6c6c 6261 7273 2061 7265  l scrollbars are
+00013930: 0a20 2020 2073 7570 706f 7274 6564 2028  .    supported (
+00013940: 6465 7065 6e64 696e 6720 6f6e 2074 6865  depending on the
+00013950: 2063 6869 6c64 2077 6964 6765 7429 2e0a   child widget)..
+00013960: 0a20 2020 2041 2063 6f72 6e65 7220 7769  .    A corner wi
+00013970: 6467 6574 2074 6f20 6869 6465 2074 6865  dget to hide the
+00013980: 2022 626c 616e 6b22 2073 7061 6365 2062   "blank" space b
+00013990: 6574 7765 656e 2073 6372 6f6c 6c62 6172  etween scrollbar
+000139a0: 7320 6973 0a20 2020 2061 7574 6f6d 6174  s is.    automat
+000139b0: 6963 616c 6c79 2069 6e63 6c75 6465 6420  ically included 
+000139c0: 6966 206e 6565 6465 642c 2074 6869 7320  if needed, this 
+000139d0: 6973 2069 6d70 6c65 6d65 6e74 6564 2061  is implemented a
+000139e0: 7320 6120 736f 2d63 616c 6c65 640a 2020  s a so-called.  
+000139f0: 2020 2273 697a 6567 7269 7022 2e0a 0a20    "sizegrip"... 
+00013a00: 2020 2054 6865 7265 2069 7320 6e6f 2050     There is no P
+00013a10: 7974 686f 6e20 646f 6375 6d65 6e74 6174  ython documentat
+00013a20: 696f 6e2c 2073 6565 2060 6054 6b60 600a  ion, see ``Tk``.
+00013a30: 2020 2020 6074 746b 2e53 6372 6f6c 6c62      `ttk.Scrollb
+00013a40: 6172 203c 6874 7470 733a 2f2f 7777 772e  ar <https://www.
+00013a50: 7463 6c2e 746b 2f6d 616e 2f74 636c 2f54  tcl.tk/man/tcl/T
+00013a60: 6b43 6d64 2f74 746b 5f73 6372 6f6c 6c62  kCmd/ttk_scrollb
+00013a70: 6172 2e68 746d 6c3e 605f 2061 6e64 0a20  ar.html>`_ and. 
+00013a80: 2020 2060 7474 6b2e 5369 7a65 6772 6970     `ttk.Sizegrip
+00013a90: 203c 6874 7470 733a 2f2f 7777 772e 7463   <https://www.tc
+00013aa0: 6c2e 746b 2f6d 616e 2f74 636c 2f54 6b43  l.tk/man/tcl/TkC
+00013ab0: 6d64 2f74 746b 5f73 697a 6567 7269 702e  md/ttk_sizegrip.
+00013ac0: 6874 6d6c 3e60 5f20 646f 6375 6d65 6e74  html>`_ document
+00013ad0: 6174 696f 6e2e 0a0a 2020 2020 5468 6520  ation...    The 
+00013ae0: 7363 726f 6c6c 6261 7273 2063 616e 2062  scrollbars can b
+00013af0: 6520 666f 7263 6564 2074 6f20 6265 2073  e forced to be s
+00013b00: 686f 776e 2c20 6f72 2074 6865 7920 6361  hown, or they ca
+00013b10: 6e20 6265 2063 6f6e 6669 6775 7265 6420  n be configured 
+00013b20: 696e 0a20 2020 2061 7574 6f6d 6174 6963  in.    automatic
+00013b30: 206d 6f64 652e 2054 6869 7320 7769 6c6c   mode. This will
+00013b40: 2073 686f 7720 6f72 2068 6964 6520 7468   show or hide th
+00013b50: 6520 7363 726f 6c6c 6261 7273 2061 7320  e scrollbars as 
+00013b60: 6e65 6564 6564 2e0a 2020 2020 5468 6973  needed..    This
+00013b70: 2061 6d6f 756e 7473 2074 6f20 6869 6465   amounts to hide
+00013b80: 2074 6865 6d20 7768 656e 2074 6865 2063   them when the c
+00013b90: 6869 6c64 2077 6964 6765 7420 6e65 6564  hild widget need
+00013ba0: 7320 6e6f 2073 6372 6f6c 6c62 6172 732e  s no scrollbars.
+00013bb0: 0a20 2020 2054 6865 2064 6566 6175 6c74  .    The default
+00013bc0: 2062 6568 6176 696f 7572 2069 7320 7468   behaviour is th
+00013bd0: 6973 2061 7574 6f6d 6174 6963 2073 686f  is automatic sho
+00013be0: 7769 6e67 2f68 6964 696e 6720 666f 7220  wing/hiding for 
+00013bf0: 626f 7468 2073 6372 6f6c 6c62 6172 732e  both scrollbars.
+00013c00: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+00013c10: 2020 2020 6368 696c 6443 6c61 7373 3a20      childClass: 
+00013c20: 5468 6520 6368 696c 6472 656e 2063 6c61  The children cla
+00013c30: 7373 2028 6361 6c6c 6564 2074 6f20 6372  ss (called to cr
+00013c40: 6561 7465 2074 6865 2063 6869 6c64 2077  eate the child w
+00013c50: 6964 6765 7429 2e0a 2020 2020 2020 2020  idget)..        
+00013c60: 2020 2020 4d75 7374 2062 6520 6120 6053      Must be a `S
+00013c70: 696e 676c 6557 6964 6765 7460 2e0a 2020  ingleWidget`..  
+00013c80: 2020 2020 2020 7363 726f 6c6c 5665 7274        scrollVert
+00013c90: 6963 616c 3a20 5368 6f77 2074 6865 2076  ical: Show the v
+00013ca0: 6572 7469 6361 6c20 7363 726f 6c6c 6261  ertical scrollba
+00013cb0: 722e 0a20 2020 2020 2020 2020 2020 2055  r..            U
+00013cc0: 7365 2061 2060 626f 6f6c 6020 746f 2066  se a `bool` to f
+00013cd0: 6f72 6365 2061 2073 7461 7465 2c20 6f72  orce a state, or
+00013ce0: 2060 4e6f 6e65 6020 746f 2061 7574 6f6d   `None` to autom
+00013cf0: 6174 6963 616c 6c79 2073 686f 7720 6f72  atically show or
+00013d00: 2068 6964 6520 7468 6520 7363 726f 6c6c   hide the scroll
+00013d10: 6261 722e 0a20 2020 2020 2020 2020 2020  bar..           
+00013d20: 2044 6566 6175 6c74 7320 746f 2060 4e6f   Defaults to `No
+00013d30: 6e65 602e 0a20 2020 2020 2020 2073 6372  ne`..        scr
+00013d40: 6f6c 6c48 6f72 697a 6f6e 7461 6c3a 2049  ollHorizontal: I
+00013d50: 6e63 6c75 6465 2061 2068 6f72 697a 6f6e  nclude a horizon
+00013d60: 7461 6c20 7363 726f 6c6c 6261 722e 0a20  tal scrollbar.. 
+00013d70: 2020 2020 2020 2020 2020 2055 7365 2061             Use a
+00013d80: 2060 626f 6f6c 6020 746f 2066 6f72 6365   `bool` to force
+00013d90: 2061 2073 7461 7465 2c20 6f72 2060 4e6f   a state, or `No
+00013da0: 6e65 6020 746f 2061 7574 6f6d 6174 6963  ne` to automatic
+00013db0: 616c 6c79 2073 686f 7720 6f72 2068 6964  ally show or hid
+00013dc0: 6520 7468 6520 7363 726f 6c6c 6261 722e  e the scrollbar.
+00013dd0: 0a20 2020 2020 2020 2020 2020 2044 6566  .            Def
+00013de0: 6175 6c74 7320 746f 2060 4e6f 6e65 602e  aults to `None`.
+00013df0: 0a20 2020 2020 2020 2073 6372 6f6c 6c45  .        scrollE
+00013e00: 7870 616e 643a 2045 7870 616e 6420 7468  xpand: Expand th
+00013e10: 6520 7061 7265 6e74 2077 6964 6765 742e  e parent widget.
+00013e20: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
+00013e30: 7320 6973 2061 6e61 6c6f 676f 7573 2074  s is analogous t
+00013e40: 6f20 7468 6520 6060 6578 7061 6e64 6060  o the ``expand``
+00013e50: 2061 7267 756d 656e 7420 6f6e 0a20 2020   argument on.   
+00013e60: 2020 2020 2020 2020 2060 6d69 7869 6e2e           `mixin.
+00013e70: 436f 6e74 6169 6e65 7257 6964 6765 742e  ContainerWidget.
+00013e80: 696e 6974 5f63 6f6e 7461 696e 6572 602e  init_container`.
+00013e90: 0a0a 2020 2020 2020 2020 7061 7265 6e74  ..        parent
+00013ea0: 3a20 5468 6520 7061 7265 6e74 2077 6964  : The parent wid
+00013eb0: 6765 742e 2043 616e 2062 6520 6120 6052  get. Can be a `R
+00013ec0: 6f6f 7457 696e 646f 7760 206f 7220 616e  ootWindow` or an
+00013ed0: 6f74 6865 7220 606d 6978 696e 2e43 6f6e  other `mixin.Con
+00013ee0: 7461 696e 6572 5769 6467 6574 602e 0a0a  tainerWidget`...
+00013ef0: 2020 2020 416c 6c20 6f74 6865 7220 6172      All other ar
+00013f00: 6775 6d65 6e74 7320 6172 6520 7061 7373  guments are pass
+00013f10: 6564 2074 6f20 7468 6520 6368 696c 6472  ed to the childr
+00013f20: 656e 2060 6063 6869 6c64 436c 6173 7360  en ``childClass`
+00013f30: 6020 696e 766f 6361 7469 6f6e 2e0a 0a20  ` invocation... 
+00013f40: 2020 204e 6f74 653a 0a20 2020 2020 2020     Note:.       
+00013f50: 2054 6865 2063 6869 6c64 2077 6964 6765   The child widge
+00013f60: 7420 7769 6c6c 2068 6176 6520 6120 7265  t will have a re
+00013f70: 6665 7265 6e63 6520 746f 2074 6869 7320  ference to this 
+00013f80: 6672 616d 652c 2073 6565 2060 6d69 7869  frame, see `mixi
+00013f90: 6e2e 5369 6e67 6c65 5769 6467 6574 2e73  n.SingleWidget.s
+00013fa0: 6372 6f6c 6c46 7261 6d65 602e 0a0a 2020  crollFrame`...  
+00013fb0: 2020 5365 6520 416c 736f 3a0a 2020 2020    See Also:.    
+00013fc0: 2020 2020 5468 6572 6520 6973 2073 6f6d      There is som
+00013fd0: 6520 616e 6369 6c69 6172 7920 5079 7468  e anciliary Pyth
+00013fe0: 6f6e 2064 6f63 756d 656e 7461 7469 6f6e  on documentation
+00013ff0: 2069 6e20 6073 6372 6f6c 6c61 626c 6520   in `scrollable 
+00014000: 7769 6467 6574 0a20 2020 2020 2020 206f  widget.        o
+00014010: 7074 696f 6e73 0a20 2020 2020 2020 203c  ptions.        <
+00014020: 6874 7470 733a 2f2f 646f 6373 2e70 7974  https://docs.pyt
+00014030: 686f 6e2e 6f72 672f 332f 6c69 6272 6172  hon.org/3/librar
+00014040: 792f 746b 696e 7465 722e 7474 6b2e 6874  y/tkinter.ttk.ht
+00014050: 6d6c 2373 6372 6f6c 6c61 626c 652d 7769  ml#scrollable-wi
+00014060: 6467 6574 2d6f 7074 696f 6e73 3e60 5f2e  dget-options>`_.
+00014070: 0a0a 2020 2020 2e2e 0a20 2020 2020 2020  ..    ...       
+00014080: 2050 7974 686f 6e20 332e 3820 6973 206d   Python 3.8 is m
+00014090: 6973 7369 6e67 2074 6869 7320 7265 6665  issing this refe
+000140a0: 7265 6e63 652c 2069 6e63 6c75 6465 6420  rence, included 
+000140b0: 696e 2050 7974 686f 6e20 332e 393a 0a0a  in Python 3.9:..
+000140c0: 2020 2020 2020 2020 3a72 6566 3a60 7363          :ref:`sc
+000140d0: 726f 6c6c 6162 6c65 2077 6964 6765 7420  rollable widget 
+000140e0: 6f70 7469 6f6e 7320 3c70 7974 686f 6e3a  options <python:
+000140f0: 5363 726f 6c6c 6162 6c65 2d57 6964 6765  Scrollable-Widge
+00014100: 742d 4f70 7469 6f6e 733e 600a 2020 2020  t-Options>`.    
+00014110: 2727 270a 2020 2020 6465 6620 5f5f 696e  '''.    def __in
+00014120: 6974 5f5f 2873 656c 662c 2070 6172 656e  it__(self, paren
+00014130: 742c 2063 6869 6c64 436c 6173 733a 2074  t, childClass: t
+00014140: 7970 696e 672e 5479 7065 5b6d 6978 696e  yping.Type[mixin
+00014150: 2e53 696e 676c 6557 6964 6765 745d 2c0a  .SingleWidget],.
+00014160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014170: 202a 6172 6773 2c0a 2020 2020 2020 2020   *args,.        
+00014180: 2020 2020 2020 2020 2073 6372 6f6c 6c56           scrollV
+00014190: 6572 7469 6361 6c3a 2074 7970 696e 672e  ertical: typing.
+000141a0: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
+000141b0: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+000141c0: 2020 2020 2020 2020 7363 726f 6c6c 486f          scrollHo
+000141d0: 7269 7a6f 6e74 616c 3a20 7479 7069 6e67  rizontal: typing
+000141e0: 2e4f 7074 696f 6e61 6c5b 626f 6f6c 5d20  .Optional[bool] 
+000141f0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00014200: 2020 2020 2020 2020 2073 6372 6f6c 6c45           scrollE
+00014210: 7870 616e 643a 2062 6f6f 6c20 3d20 5472  xpand: bool = Tr
+00014220: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+00014230: 2020 2020 202a 2a63 6b77 6172 6773 293a       **ckwargs):
+00014240: 0a20 2020 2020 2020 2023 2054 6869 7320  .        # This 
+00014250: 6973 2061 2070 726f 7879 206f 626a 6563  is a proxy objec
+00014260: 742c 2064 6f6e 2774 2073 6574 2061 6e79  t, don't set any
+00014270: 2075 6e65 6365 7373 6172 7920 6073 656c   unecessary `sel
+00014280: 6660 2061 7474 7269 6275 7465 732c 206f  f` attributes, o
+00014290: 7220 7468 6579 2077 696c 6c20 6f76 6572  r they will over
+000142a0: 7269 6465 2060 6368 696c 6443 6c61 7373  ride `childClass
+000142b0: 6020 6174 7472 6962 7574 6573 0a0a 2020  ` attributes..  
+000142c0: 2020 2020 2020 2320 4375 7272 656e 7420        # Current 
+000142d0: 4672 616d 650a 2020 2020 2020 2020 7375  Frame.        su
+000142e0: 7065 7228 292e 5f5f 696e 6974 5f5f 2870  per().__init__(p
+000142f0: 6172 656e 7429 2020 2320 7474 6b2e 4672  arent)  # ttk.Fr
+00014300: 616d 650a 2020 2020 2020 2020 7277 6569  ame.        rwei
+00014310: 6768 7420 3d20 5b31 5d0a 2020 2020 2020  ght = [1].      
+00014320: 2020 6377 6569 6768 7420 3d20 5b31 5d0a    cweight = [1].
+00014330: 0a20 2020 2020 2020 2074 7970 655f 7363  .        type_sc
+00014340: 726f 6c6c 4765 6e43 6f6d 6d61 6e64 203d  rollGenCommand =
+00014350: 2074 7970 696e 672e 4361 6c6c 6162 6c65   typing.Callable
+00014360: 5b5b 666c 6f61 742c 2066 6c6f 6174 5d2c  [[float, float],
+00014370: 204e 6f6e 655d 0a0a 2020 2020 2020 2020   None]..        
+00014380: 2320 5769 6467 6574 2048 656c 7065 7273  # Widget Helpers
+00014390: 0a20 2020 2020 2020 2064 6566 2073 6372  .        def scr
+000143a0: 6f6c 6c47 656e 436f 6d6d 616e 6428 666e  ollGenCommand(fn
+000143b0: 3a20 7479 7065 5f73 6372 6f6c 6c47 656e  : type_scrollGen
+000143c0: 436f 6d6d 616e 642c 2077 6879 3a20 7479  Command, why: ty
+000143d0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 626f  ping.Optional[bo
+000143e0: 6f6c 5d2c 2077 6861 743a 2073 7472 2920  ol], what: str) 
+000143f0: 2d3e 2074 7970 655f 7363 726f 6c6c 4765  -> type_scrollGe
+00014400: 6e43 6f6d 6d61 6e64 3a0a 2020 2020 2020  nCommand:.      
+00014410: 2020 2020 2020 6966 2077 6879 3a0a 2020        if why:.  
+00014420: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00014430: 466f 7263 6520 456e 6162 6c65 2c20 646f  Force Enable, do
+00014440: 6e27 7420 6368 616e 6765 2074 6865 2073  n't change the s
+00014450: 7461 7465 0a20 2020 2020 2020 2020 2020  tate.           
+00014460: 2020 2020 2072 6574 7572 6e20 666e 0a20       return fn. 
+00014470: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00014480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014490: 2023 2041 7574 6f6d 6174 6963 2c20 6368   # Automatic, ch
+000144a0: 616e 6765 2074 6865 2073 7461 7465 2061  ange the state a
+000144b0: 7320 6e65 6564 6564 0a20 2020 2020 2020  s needed.       
+000144c0: 2020 2020 2020 2020 2040 7772 6170 7328           @wraps(
+000144d0: 666e 290a 2020 2020 2020 2020 2020 2020  fn).            
+000144e0: 2020 2020 6465 6620 7363 726f 6c6c 4765      def scrollGe
+000144f0: 6e43 6f6d 6d61 6e64 2873 706f 7373 3a20  nCommand(sposs: 
+00014500: 666c 6f61 742c 2065 706f 7373 3a20 666c  float, eposs: fl
+00014510: 6f61 7429 202d 3e20 4e6f 6e65 3a0a 2020  oat) -> None:.  
+00014520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014530: 2020 2320 4465 6665 6e73 6976 6520 5072    # Defensive Pr
+00014540: 6f67 7261 6d6d 696e 672c 2066 6f72 206f  ogramming, for o
+00014550: 6c64 6572 2076 6572 7369 6f6e 7320 286d  lder versions (m
+00014560: 616b 6520 5245 414c 4c59 2073 7572 6520  ake REALLY sure 
+00014570: 7468 6f73 6520 6172 6520 666c 6f61 7473  those are floats
+00014580: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00014590: 2020 2020 2020 7370 6f73 3a20 666c 6f61        spos: floa
+000145a0: 7420 3d20 666c 6f61 7428 7370 6f73 7329  t = float(sposs)
+000145b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000145c0: 2020 2020 2065 706f 733a 2066 6c6f 6174       epos: float
+000145d0: 203d 2066 6c6f 6174 2865 706f 7373 290a   = float(eposs).
+000145e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000145f0: 2020 2020 616c 6c76 6973 6962 6c65 3a20      allvisible: 
+00014600: 626f 6f6c 203d 2073 706f 7320 3d3d 2030  bool = spos == 0
+00014610: 2e30 2061 6e64 2065 706f 7320 3d3d 2031  .0 and epos == 1
+00014620: 2e30 0a20 2020 2020 2020 2020 2020 2020  .0.             
+00014630: 2020 2020 2020 2023 2069 6620 5f5f 6465         # if __de
+00014640: 6275 675f 5f3a 0a20 2020 2020 2020 2020  bug__:.         
+00014650: 2020 2020 2020 2020 2020 2023 2020 2020             #    
+00014660: 206c 6f67 6765 722e 6465 6275 6728 2753   logger.debug('S
+00014670: 6372 6f6c 6c43 6f6d 6d61 6e64 5b25 735d  crollCommand[%s]
+00014680: 3a20 5b25 6620 2c20 2566 5d20 3d20 2573  : [%f , %f] = %s
+00014690: 272c 2077 6861 742c 2073 706f 732c 2065  ', what, spos, e
+000146a0: 706f 732c 2061 6c6c 7669 7369 626c 6529  pos, allvisible)
+000146b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000146c0: 2020 2020 2073 656c 662e 7365 745f 7363       self.set_sc
+000146d0: 726f 6c6c 5f73 7461 7465 282a 2a7b 7768  roll_state(**{wh
+000146e0: 6174 3a20 6e6f 7420 616c 6c76 6973 6962  at: not allvisib
+000146f0: 6c65 7d29 0a20 2020 2020 2020 2020 2020  le}).           
+00014700: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00014710: 666e 2873 706f 732c 2065 706f 7329 0a20  fn(spos, epos). 
+00014720: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00014730: 6574 7572 6e20 7363 726f 6c6c 4765 6e43  eturn scrollGenC
+00014740: 6f6d 6d61 6e64 0a0a 2020 2020 2020 2020  ommand..        
+00014750: 2320 5769 6467 6574 730a 2020 2020 2020  # Widgets.      
+00014760: 2020 7365 6c66 2e5f 5f76 6261 723a 2074    self.__vbar: t
+00014770: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
+00014780: 746b 2e53 6372 6f6c 6c62 6172 5d20 3d20  tk.Scrollbar] = 
+00014790: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
+000147a0: 662e 5f5f 6862 6172 3a20 7479 7069 6e67  f.__hbar: typing
+000147b0: 2e4f 7074 696f 6e61 6c5b 7474 6b2e 5363  .Optional[ttk.Sc
+000147c0: 726f 6c6c 6261 725d 203d 204e 6f6e 650a  rollbar] = None.
+000147d0: 2020 2020 2020 2020 7365 6c66 2e5f 5f63          self.__c
+000147e0: 6f72 6e65 723a 2074 7970 696e 672e 4f70  orner: typing.Op
+000147f0: 7469 6f6e 616c 5b74 746b 2e53 697a 6567  tional[ttk.Sizeg
+00014800: 7269 705d 203d 204e 6f6e 650a 2020 2020  rip] = None.    
+00014810: 2020 2020 6966 2073 6372 6f6c 6c48 6f72      if scrollHor
+00014820: 697a 6f6e 7461 6c20 696e 2028 4e6f 6e65  izontal in (None
+00014830: 2c20 5472 7565 293a 0a20 2020 2020 2020  , True):.       
+00014840: 2020 2020 2073 656c 662e 5f5f 6862 6172       self.__hbar
+00014850: 203d 2074 746b 2e53 6372 6f6c 6c62 6172   = ttk.Scrollbar
+00014860: 2873 656c 662c 206f 7269 656e 743d 746b  (self, orient=tk
+00014870: 2e48 4f52 495a 4f4e 5441 4c29 0a20 2020  .HORIZONTAL).   
+00014880: 2020 2020 2020 2020 2063 6b77 6172 6773           ckwargs
+00014890: 5b27 7873 6372 6f6c 6c63 6f6d 6d61 6e64  ['xscrollcommand
+000148a0: 275d 203d 2073 6372 6f6c 6c47 656e 436f  '] = scrollGenCo
+000148b0: 6d6d 616e 6428 7365 6c66 2e5f 5f68 6261  mmand(self.__hba
+000148c0: 722e 7365 742c 2073 6372 6f6c 6c48 6f72  r.set, scrollHor
+000148d0: 697a 6f6e 7461 6c2c 2027 6873 7461 7465  izontal, 'hstate
+000148e0: 2729 0a20 2020 2020 2020 2020 2020 2063  ').            c
+000148f0: 7765 6967 6874 2e61 7070 656e 6428 3029  weight.append(0)
+00014900: 0a20 2020 2020 2020 2069 6620 7363 726f  .        if scro
+00014910: 6c6c 5665 7274 6963 616c 2069 6e20 284e  llVertical in (N
+00014920: 6f6e 652c 2054 7275 6529 3a0a 2020 2020  one, True):.    
+00014930: 2020 2020 2020 2020 7365 6c66 2e5f 5f76          self.__v
+00014940: 6261 7220 3d20 7474 6b2e 5363 726f 6c6c  bar = ttk.Scroll
+00014950: 6261 7228 7365 6c66 2c20 6f72 6965 6e74  bar(self, orient
+00014960: 3d74 6b2e 5645 5254 4943 414c 290a 2020  =tk.VERTICAL).  
+00014970: 2020 2020 2020 2020 2020 636b 7761 7267            ckwarg
+00014980: 735b 2779 7363 726f 6c6c 636f 6d6d 616e  s['yscrollcomman
+00014990: 6427 5d20 3d20 7363 726f 6c6c 4765 6e43  d'] = scrollGenC
+000149a0: 6f6d 6d61 6e64 2873 656c 662e 5f5f 7662  ommand(self.__vb
+000149b0: 6172 2e73 6574 2c20 7363 726f 6c6c 5665  ar.set, scrollVe
+000149c0: 7274 6963 616c 2c20 2776 7374 6174 6527  rtical, 'vstate'
+000149d0: 290a 2020 2020 2020 2020 2020 2020 7277  ).            rw
+000149e0: 6569 6768 742e 6170 7065 6e64 2830 290a  eight.append(0).
+000149f0: 2020 2020 2020 2020 6966 2073 6372 6f6c          if scrol
+00014a00: 6c56 6572 7469 6361 6c20 696e 2028 4e6f  lVertical in (No
+00014a10: 6e65 2c20 5472 7565 2920 616e 6420 7363  ne, True) and sc
+00014a20: 726f 6c6c 5665 7274 6963 616c 2069 6e20  rollVertical in 
+00014a30: 284e 6f6e 652c 2054 7275 6529 3a0a 2020  (None, True):.  
+00014a40: 2020 2020 2020 2020 2020 2320 5468 6973            # This
+00014a50: 2069 7320 6e6f 7420 7374 7269 636c 7920   is not stricly 
+00014a60: 6e65 6365 7373 6172 792c 2062 7574 206e  necessary, but n
+00014a70: 6963 6520 746f 2068 6176 652e 0a20 2020  ice to have..   
+00014a80: 2020 2020 2020 2020 2073 656c 662e 5f5f           self.__
+00014a90: 636f 726e 6572 203d 2074 746b 2e53 697a  corner = ttk.Siz
+00014aa0: 6567 7269 7028 7365 6c66 2c20 6375 7273  egrip(self, curs
+00014ab0: 6f72 3d27 272c 2074 616b 6566 6f63 7573  or='', takefocus
+00014ac0: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
+00014ad0: 2020 2020 2320 4469 7361 626c 6520 7369      # Disable si
+00014ae0: 7a65 6772 6970 2065 7665 6e74 730a 2020  zegrip events.  
+00014af0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00014b00: 5f63 6f72 6e65 722e 6269 6e64 2827 3c42  _corner.bind('<B
+00014b10: 7574 746f 6e2d 313e 272c 2066 6e2e 6269  utton-1>', fn.bi
+00014b20: 6e64 696e 675f 6469 7361 626c 6529 0a20  nding_disable). 
+00014b30: 2020 2020 2020 2063 7769 6467 6574 203d         cwidget =
+00014b40: 2063 6869 6c64 436c 6173 7328 7365 6c66   childClass(self
+00014b50: 2c20 2a61 7267 732c 202a 2a63 6b77 6172  , *args, **ckwar
+00014b60: 6773 2920 2023 2074 7970 653a 2069 676e  gs)  # type: ign
+00014b70: 6f72 650a 0a20 2020 2020 2020 2023 2053  ore..        # S
+00014b80: 7461 7465 0a20 2020 2020 2020 2073 656c  tate.        sel
+00014b90: 662e 7374 6174 655f 7479 7065 203d 2063  f.state_type = c
+00014ba0: 7769 6467 6574 2e73 7461 7465 5f74 7970  widget.state_typ
+00014bb0: 650a 2020 2020 2020 2020 7365 6c66 2e69  e.        self.i
+00014bc0: 6e69 745f 7369 6e67 6c65 2876 6172 6961  nit_single(varia
+00014bd0: 626c 653d 6377 6964 6765 742e 7661 7269  ble=cwidget.vari
+00014be0: 6162 6c65 290a 2020 2020 2020 2020 2320  able).        # 
+00014bf0: 5370 6563 6961 6c20 5769 6467 6574 2073  Special Widget s
+00014c00: 7461 7465 0a20 2020 2020 2020 2073 656c  tate.        sel
+00014c10: 662e 7770 6172 656e 7420 3d20 7061 7265  f.wparent = pare
+00014c20: 6e74 0a0a 2020 2020 2020 2020 2320 476c  nt..        # Gl
+00014c30: 7565 2073 6372 6f6c 6c62 6172 7320 7769  ue scrollbars wi
+00014c40: 7468 2063 6869 6c64 2077 6964 6765 740a  th child widget.
+00014c50: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00014c60: 5f5f 6862 6172 3a0a 2020 2020 2020 2020  __hbar:.        
+00014c70: 2020 2020 6173 7365 7274 2069 7369 6e73      assert isins
+00014c80: 7461 6e63 6528 6377 6964 6765 742c 2074  tance(cwidget, t
+00014c90: 6b2e 5856 6965 7729 2c20 6627 496e 7661  k.XView), f'Inva
+00014ca0: 6c69 6420 4368 696c 6420 5769 6467 6574  lid Child Widget
+00014cb0: 3a20 7b63 7769 6467 6574 2172 7d27 0a20  : {cwidget!r}'. 
+00014cc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014cd0: 5f5f 6862 6172 5b27 636f 6d6d 616e 6427  __hbar['command'
+00014ce0: 5d20 3d20 6377 6964 6765 742e 7876 6965  ] = cwidget.xvie
+00014cf0: 770a 2020 2020 2020 2020 6966 2073 656c  w.        if sel
+00014d00: 662e 5f5f 7662 6172 3a0a 2020 2020 2020  f.__vbar:.      
+00014d10: 2020 2020 2020 6173 7365 7274 2069 7369        assert isi
+00014d20: 6e73 7461 6e63 6528 6377 6964 6765 742c  nstance(cwidget,
+00014d30: 2074 6b2e 5956 6965 7729 2c20 6627 496e   tk.YView), f'In
+00014d40: 7661 6c69 6420 4368 696c 6420 5769 6467  valid Child Widg
+00014d50: 6574 3a20 7b63 7769 6467 6574 2172 7d27  et: {cwidget!r}'
+00014d60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00014d70: 662e 5f5f 7662 6172 5b27 636f 6d6d 616e  f.__vbar['comman
+00014d80: 6427 5d20 3d20 6377 6964 6765 742e 7976  d'] = cwidget.yv
+00014d90: 6965 770a 0a20 2020 2020 2020 2023 204c  iew..        # L
+00014da0: 6179 6f75 740a 2020 2020 2020 2020 6966  ayout.        if
+00014db0: 2073 6372 6f6c 6c45 7870 616e 643a 0a20   scrollExpand:. 
+00014dc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014dd0: 6772 6964 2873 7469 636b 793d 746b 2e4e  grid(sticky=tk.N
+00014de0: 5345 5729 0a20 2020 2020 2020 2061 7373  SEW).        ass
+00014df0: 6572 7420 6973 696e 7374 616e 6365 2863  ert isinstance(c
+00014e00: 7769 6467 6574 2c20 746b 2e47 7269 6429  widget, tk.Grid)
+00014e10: 2c20 6627 496e 7661 6c69 6420 4368 696c  , f'Invalid Chil
+00014e20: 6420 5769 6467 6574 3a20 7b63 7769 6467  d Widget: {cwidg
+00014e30: 6574 2172 7d27 0a20 2020 2020 2020 2063  et!r}'.        c
+00014e40: 7769 6467 6574 2e67 7269 6428 726f 773d  widget.grid(row=
+00014e50: 302c 2063 6f6c 756d 6e3d 302c 2073 7469  0, column=0, sti
+00014e60: 636b 793d 746b 2e4e 5345 5729 0a20 2020  cky=tk.NSEW).   
+00014e70: 2020 2020 2073 656c 662e 7365 745f 7363       self.set_sc
+00014e80: 726f 6c6c 5f73 7461 7465 2873 6372 6f6c  roll_state(scrol
+00014e90: 6c48 6f72 697a 6f6e 7461 6c20 6f72 204e  lHorizontal or N
+00014ea0: 6f6e 652c 2073 6372 6f6c 6c56 6572 7469  one, scrollVerti
+00014eb0: 6361 6c20 6f72 204e 6f6e 6529 0a20 2020  cal or None).   
+00014ec0: 2020 2020 2023 2045 6d75 6c61 7465 2060       # Emulate `
+00014ed0: 666e 2e63 6f6e 6669 6775 7265 5f67 7269  fn.configure_gri
+00014ee0: 6428 7365 6c66 2c20 7277 6569 6768 742c  d(self, rweight,
+00014ef0: 2063 7765 6967 6874 2960 0a20 2020 2020   cweight)`.     
+00014f00: 2020 2066 6f72 2072 6964 782c 2077 6569     for ridx, wei
+00014f10: 6768 7420 696e 2065 6e75 6d65 7261 7465  ght in enumerate
+00014f20: 2872 7765 6967 6874 293a 0a20 2020 2020  (rweight):.     
+00014f30: 2020 2020 2020 2073 656c 662e 726f 7763         self.rowc
+00014f40: 6f6e 6669 6775 7265 2872 6964 782c 2077  onfigure(ridx, w
+00014f50: 6569 6768 743d 7765 6967 6874 290a 2020  eight=weight).  
+00014f60: 2020 2020 2020 666f 7220 6369 6478 2c20        for cidx, 
+00014f70: 7765 6967 6874 2069 6e20 656e 756d 6572  weight in enumer
+00014f80: 6174 6528 6377 6569 6768 7429 3a0a 2020  ate(cweight):.  
+00014f90: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00014fa0: 6f6c 756d 6e63 6f6e 6669 6775 7265 2863  olumnconfigure(c
+00014fb0: 6964 782c 2077 6569 6768 743d 7765 6967  idx, weight=weig
+00014fc0: 6874 290a 0a20 2020 2020 2020 2023 2050  ht)..        # P
+00014fd0: 726f 7879 2061 6c6c 2061 6363 6573 7320  roxy all access 
+00014fe0: 746f 2060 6377 6964 6765 7460 0a20 2020  to `cwidget`.   
+00014ff0: 2020 2020 2063 7769 6467 6574 2e73 6372       cwidget.scr
+00015000: 6f6c 6c46 7261 6d65 203d 2073 656c 660a  ollFrame = self.
+00015010: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
+00015020: 7865 6520 3d20 6377 6964 6765 740a 0a20  xee = cwidget.. 
+00015030: 2020 2064 6566 2067 6574 5f73 6372 6f6c     def get_scrol
+00015040: 6c5f 7374 6174 6528 7365 6c66 2920 2d3e  l_state(self) ->
+00015050: 2074 7970 696e 672e 5475 706c 655b 626f   typing.Tuple[bo
+00015060: 6f6c 2c20 626f 6f6c 5d3a 0a20 2020 2020  ol, bool]:.     
+00015070: 2020 2027 2727 4765 7420 7468 6520 6375     '''Get the cu
+00015080: 7272 656e 7420 7363 726f 6c6c 6261 7220  rrent scrollbar 
+00015090: 7669 7369 6269 6c69 7479 2073 7461 7465  visibility state
+000150a0: 2e0a 0a20 2020 2020 2020 2049 6620 7468  ...        If th
+000150b0: 6520 7363 726f 6c6c 6261 7220 6973 2063  e scrollbar is c
+000150c0: 6f6d 706c 6574 656c 7920 6469 7361 626c  ompletely disabl
+000150d0: 6564 2c20 6046 616c 7365 6020 6973 2072  ed, `False` is r
+000150e0: 6574 7572 6e65 642e 0a0a 2020 2020 2020  eturned...      
+000150f0: 2020 5468 6973 2069 7320 6120 7475 706c    This is a tupl
+00015100: 6520 7769 7468 2074 6865 2073 7461 7465  e with the state
+00015110: 2066 6f72 2062 6f74 6820 7363 726f 6c6c   for both scroll
+00015120: 6261 7273 2c20 686f 7269 7a6f 6e74 616c  bars, horizontal
+00015130: 2061 6e64 0a20 2020 2020 2020 2076 6572   and.        ver
+00015140: 7469 6361 6c2e 0a0a 2020 2020 2020 2020  tical...        
+00015150: 5365 6520 416c 736f 3a0a 2020 2020 2020  See Also:.      
+00015160: 2020 2020 2020 2d20 6073 6574 5f73 6372        - `set_scr
+00015170: 6f6c 6c5f 7374 6174 6560 3a20 4368 616e  oll_state`: Chan
+00015180: 6765 2074 6865 2063 7572 7265 6e74 2073  ge the current s
+00015190: 7461 7465 0a20 2020 2020 2020 2027 2727  tate.        '''
+000151a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000151b0: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
+000151c0: 6c66 2e5f 5f68 6261 7220 6973 206e 6f74  lf.__hbar is not
+000151d0: 204e 6f6e 6520 616e 6420 626f 6f6c 2873   None and bool(s
+000151e0: 656c 662e 5f5f 6862 6172 2e67 7269 645f  elf.__hbar.grid_
+000151f0: 696e 666f 2829 292c 0a20 2020 2020 2020  info()),.       
+00015200: 2020 2020 2073 656c 662e 5f5f 7662 6172       self.__vbar
+00015210: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+00015220: 2062 6f6f 6c28 7365 6c66 2e5f 5f76 6261   bool(self.__vba
+00015230: 722e 6772 6964 5f69 6e66 6f28 2929 2c0a  r.grid_info()),.
+00015240: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+00015250: 6566 2073 6574 5f73 6372 6f6c 6c5f 7374  ef set_scroll_st
+00015260: 6174 6528 7365 6c66 2c20 6873 7461 7465  ate(self, hstate
+00015270: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+00015280: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 2c20  l[bool] = None, 
+00015290: 7673 7461 7465 3a20 7479 7069 6e67 2e4f  vstate: typing.O
+000152a0: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
+000152b0: 4e6f 6e65 2920 2d3e 204e 6f6e 653a 0a20  None) -> None:. 
+000152c0: 2020 2020 2020 2027 2727 4368 616e 6765         '''Change
+000152d0: 2074 6865 2063 7572 7265 6e74 2073 6372   the current scr
+000152e0: 6f6c 6c62 6172 2076 6973 6962 696c 6974  ollbar visibilit
+000152f0: 7920 7374 6174 652e 0a0a 2020 2020 2020  y state...      
+00015300: 2020 5468 6973 2063 616e 2063 6861 6e67    This can chang
+00015310: 6520 626f 7468 2068 6f72 697a 6f6e 7461  e both horizonta
+00015320: 6c20 616e 6420 7665 7274 6963 616c 2073  l and vertical s
+00015330: 7461 7465 2069 6e64 6570 656e 6465 6e74  tate independent
+00015340: 6c79 2e20 5468 650a 2020 2020 2020 2020  ly. The.        
+00015350: 636f 726e 6572 2077 6964 6765 7420 6973  corner widget is
+00015360: 206d 616e 6167 6564 2061 7574 6f6d 6174   managed automat
+00015370: 6963 616c 6c79 2e0a 0a20 2020 2020 2020  ically...       
+00015380: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00015390: 2020 2068 7374 6174 653a 2049 6620 6e6f     hstate: If no
+000153a0: 7420 604e 6f6e 6560 2c20 7365 7420 7468  t `None`, set th
+000153b0: 6520 686f 7269 7a6f 6e74 616c 2073 6372  e horizontal scr
+000153c0: 6f6c 6c62 6172 2076 6973 6962 696c 6974  ollbar visibilit
+000153d0: 792e 0a20 2020 2020 2020 2020 2020 2076  y..            v
+000153e0: 7374 6174 653a 2049 6620 6e6f 7420 604e  state: If not `N
+000153f0: 6f6e 6560 2c20 7365 7420 7468 6520 7665  one`, set the ve
+00015400: 7274 6963 616c 2073 6372 6f6c 6c62 6172  rtical scrollbar
+00015410: 2076 6973 6962 696c 6974 792e 0a0a 2020   visibility...  
+00015420: 2020 2020 2020 5365 6520 416c 736f 3a0a        See Also:.
+00015430: 2020 2020 2020 2020 2020 2020 2d20 6067              - `g
+00015440: 6574 5f73 6372 6f6c 6c5f 7374 6174 6560  et_scroll_state`
+00015450: 3a20 4765 7420 7468 6520 6375 7272 656e  : Get the curren
+00015460: 7420 7374 6174 650a 2020 2020 2020 2020  t state.        
+00015470: 2727 270a 2020 2020 2020 2020 6966 2068  '''.        if h
+00015480: 7374 6174 6520 6973 206e 6f74 204e 6f6e  state is not Non
+00015490: 6520 616e 6420 7365 6c66 2e5f 5f68 6261  e and self.__hba
+000154a0: 7220 6973 206e 6f74 204e 6f6e 653a 0a20  r is not None:. 
+000154b0: 2020 2020 2020 2020 2020 2068 5f77 6772             h_wgr
+000154c0: 6964 203d 2073 656c 662e 5f5f 6862 6172  id = self.__hbar
+000154d0: 2e67 7269 645f 696e 666f 2829 0a20 2020  .grid_info().   
+000154e0: 2020 2020 2020 2020 2069 6620 6873 7461           if hsta
+000154f0: 7465 3a0a 2020 2020 2020 2020 2020 2020  te:.            
+00015500: 2020 2020 6966 206e 6f74 2068 5f77 6772      if not h_wgr
+00015510: 6964 3a0a 2020 2020 2020 2020 2020 2020  id:.            
+00015520: 2020 2020 2020 2020 7365 6c66 2e5f 5f68          self.__h
+00015530: 6261 722e 6772 6964 2872 6f77 3d31 2c20  bar.grid(row=1, 
+00015540: 636f 6c75 6d6e 3d30 2c20 7374 6963 6b79  column=0, sticky
+00015550: 3d74 6b2e 4557 290a 2020 2020 2020 2020  =tk.EW).        
+00015560: 2020 2020 2020 2020 2020 2020 6966 205f              if _
+00015570: 5f64 6562 7567 5f5f 3a0a 2020 2020 2020  _debug__:.      
+00015580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015590: 2020 6c6f 6767 6572 2e64 6562 7567 2827    logger.debug('
+000155a0: 2573 3a20 5368 6f77 2068 6261 7227 2c20  %s: Show hbar', 
+000155b0: 7365 6c66 290a 2020 2020 2020 2020 2020  self).          
+000155c0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000155d0: 2020 2020 2020 2020 6966 2068 5f77 6772          if h_wgr
+000155e0: 6964 3a0a 2020 2020 2020 2020 2020 2020  id:.            
+000155f0: 2020 2020 2020 2020 6966 205f 5f64 6562          if __deb
+00015600: 7567 5f5f 3a0a 2020 2020 2020 2020 2020  ug__:.          
+00015610: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00015620: 6767 6572 2e64 6562 7567 2827 2573 3a20  gger.debug('%s: 
+00015630: 4869 6465 2068 6261 7227 2c20 7365 6c66  Hide hbar', self
+00015640: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00015650: 2020 2020 2020 7365 6c66 2e5f 5f68 6261        self.__hba
+00015660: 722e 6772 6964 5f72 656d 6f76 6528 290a  r.grid_remove().
+00015670: 2020 2020 2020 2020 6966 2076 7374 6174          if vstat
+00015680: 6520 6973 206e 6f74 204e 6f6e 6520 616e  e is not None an
+00015690: 6420 7365 6c66 2e5f 5f76 6261 7220 6973  d self.__vbar is
+000156a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000156b0: 2020 2020 2020 2076 5f77 6772 6964 203d         v_wgrid =
+000156c0: 2073 656c 662e 5f5f 7662 6172 2e67 7269   self.__vbar.gri
+000156d0: 645f 696e 666f 2829 0a20 2020 2020 2020  d_info().       
+000156e0: 2020 2020 2069 6620 7673 7461 7465 3a0a       if vstate:.
+000156f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015700: 6966 206e 6f74 2076 5f77 6772 6964 3a0a  if not v_wgrid:.
+00015710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015720: 2020 2020 7365 6c66 2e5f 5f76 6261 722e      self.__vbar.
+00015730: 6772 6964 2872 6f77 3d30 2c20 636f 6c75  grid(row=0, colu
+00015740: 6d6e 3d31 2c20 7374 6963 6b79 3d74 6b2e  mn=1, sticky=tk.
+00015750: 4e53 290a 2020 2020 2020 2020 2020 2020  NS).            
+00015760: 2020 2020 2020 2020 6966 205f 5f64 6562          if __deb
+00015770: 7567 5f5f 3a0a 2020 2020 2020 2020 2020  ug__:.          
+00015780: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00015790: 6767 6572 2e64 6562 7567 2827 2573 3a20  gger.debug('%s: 
+000157a0: 5368 6f77 2076 6261 7227 2c20 7365 6c66  Show vbar', self
+000157b0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+000157c0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000157d0: 2020 2020 6966 2076 5f77 6772 6964 3a0a      if v_wgrid:.
+000157e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000157f0: 2020 2020 6966 205f 5f64 6562 7567 5f5f      if __debug__
+00015800: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00015810: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+00015820: 2e64 6562 7567 2827 2573 3a20 4869 6465  .debug('%s: Hide
+00015830: 2076 6261 7227 2c20 7365 6c66 290a 2020   vbar', self).  
+00015840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015850: 2020 7365 6c66 2e5f 5f76 6261 722e 6772    self.__vbar.gr
+00015860: 6964 5f72 656d 6f76 6528 290a 2020 2020  id_remove().    
+00015870: 2020 2020 6966 2073 656c 662e 5f5f 636f      if self.__co
+00015880: 726e 6572 2069 7320 6e6f 7420 4e6f 6e65  rner is not None
+00015890: 3a0a 2020 2020 2020 2020 2020 2020 6973  :.            is
+000158a0: 486f 7269 7a6f 6e74 616c 203d 2073 656c  Horizontal = sel
+000158b0: 662e 5f5f 6862 6172 2069 7320 6e6f 7420  f.__hbar is not 
+000158c0: 4e6f 6e65 2061 6e64 2073 656c 662e 5f5f  None and self.__
+000158d0: 6862 6172 2e67 7269 645f 696e 666f 2829  hbar.grid_info()
+000158e0: 0a20 2020 2020 2020 2020 2020 2069 7356  .            isV
+000158f0: 6572 7469 6361 6c20 3d20 7365 6c66 2e5f  ertical = self._
+00015900: 5f76 6261 7220 6973 206e 6f74 204e 6f6e  _vbar is not Non
+00015910: 6520 616e 6420 7365 6c66 2e5f 5f76 6261  e and self.__vba
+00015920: 722e 6772 6964 5f69 6e66 6f28 290a 2020  r.grid_info().  
+00015930: 2020 2020 2020 2020 2020 635f 7767 7269            c_wgri
+00015940: 6420 3d20 7365 6c66 2e5f 5f63 6f72 6e65  d = self.__corne
+00015950: 722e 6772 6964 5f69 6e66 6f28 290a 2020  r.grid_info().  
+00015960: 2020 2020 2020 2020 2020 6966 2069 7348            if isH
+00015970: 6f72 697a 6f6e 7461 6c20 616e 6420 6973  orizontal and is
+00015980: 5665 7274 6963 616c 3a0a 2020 2020 2020  Vertical:.      
+00015990: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+000159a0: 2063 5f77 6772 6964 3a0a 2020 2020 2020   c_wgrid:.      
+000159b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000159c0: 6c66 2e5f 5f63 6f72 6e65 722e 6772 6964  lf.__corner.grid
+000159d0: 2872 6f77 3d31 2c20 636f 6c75 6d6e 3d31  (row=1, column=1
+000159e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000159f0: 2020 2020 2020 6966 205f 5f64 6562 7567        if __debug
+00015a00: 5f5f 3a0a 2020 2020 2020 2020 2020 2020  __:.            
+00015a10: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+00015a20: 6572 2e64 6562 7567 2827 2573 3a20 5368  er.debug('%s: Sh
+00015a30: 6f77 2063 6f72 6e65 7227 2c20 7365 6c66  ow corner', self
+00015a40: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+00015a50: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00015a60: 2020 2020 6966 2063 5f77 6772 6964 3a0a      if c_wgrid:.
+00015a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015a80: 2020 2020 6966 205f 5f64 6562 7567 5f5f      if __debug__
+00015a90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00015aa0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+00015ab0: 2e64 6562 7567 2827 2573 3a20 4869 6465  .debug('%s: Hide
+00015ac0: 2063 6f72 6e65 7227 2c20 7365 6c66 290a   corner', self).
+00015ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ae0: 2020 2020 7365 6c66 2e5f 5f63 6f72 6e65      self.__corne
+00015af0: 722e 6772 6964 5f72 656d 6f76 6528 290a  r.grid_remove().
+00015b00: 0a20 2020 2064 6566 205f 5f67 6574 6174  .    def __getat
+00015b10: 7472 5f5f 2873 656c 662c 206e 616d 6529  tr__(self, name)
+00015b20: 3a0a 2020 2020 2020 2020 6966 2070 726f  :.        if pro
+00015b30: 7865 6520 3a3d 2073 656c 662e 5f5f 6469  xee := self.__di
+00015b40: 6374 5f5f 2e67 6574 2827 7072 6f78 6565  ct__.get('proxee
+00015b50: 272c 204e 6f6e 6529 3a0a 2020 2020 2020  ', None):.      
+00015b60: 2020 2020 2020 2320 506f 7374 2d49 6e69        # Post-Ini
+00015b70: 7469 616c 697a 6174 696f 6e0a 2020 2020  tialization.    
+00015b80: 2020 2020 2020 2020 7265 7475 726e 2067          return g
+00015b90: 6574 6174 7472 2870 726f 7865 652c 206e  etattr(proxee, n
+00015ba0: 616d 6529 0a20 2020 2020 2020 2065 6c73  ame).        els
+00015bb0: 653a 0a20 2020 2020 2020 2020 2020 2023  e:.            #
+00015bc0: 2044 7572 696e 6720 605f 5f69 6e69 745f   During `__init_
+00015bd0: 5f60 0a20 2020 2020 2020 2020 2020 2072  _`.            r
+00015be0: 6574 7572 6e20 6f62 6a65 6374 2e5f 5f67  eturn object.__g
+00015bf0: 6574 6174 7472 5f5f 2873 656c 662c 206e  etattr__(self, n
+00015c00: 616d 6529 0a0a 2020 2020 6465 6620 5f5f  ame)..    def __
+00015c10: 7365 7461 7474 725f 5f28 7365 6c66 2c20  setattr__(self, 
+00015c20: 6e61 6d65 2c20 7661 6c75 6529 3a0a 2020  name, value):.  
+00015c30: 2020 2020 2020 6966 2070 726f 7865 6520        if proxee 
+00015c40: 3a3d 2073 656c 662e 5f5f 6469 6374 5f5f  := self.__dict__
+00015c50: 2e67 6574 2827 7072 6f78 6565 272c 204e  .get('proxee', N
+00015c60: 6f6e 6529 3a0a 2020 2020 2020 2020 2020  one):.          
+00015c70: 2020 2320 506f 7374 2d49 6e69 7469 616c    # Post-Initial
+00015c80: 697a 6174 696f 6e0a 2020 2020 2020 2020  ization.        
+00015c90: 2020 2020 7365 7461 7474 7228 7072 6f78      setattr(prox
+00015ca0: 6565 2c20 6e61 6d65 2c20 7661 6c75 6529  ee, name, value)
+00015cb0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00015cc0: 2020 2020 2020 2020 2020 2023 2044 7572             # Dur
+00015cd0: 696e 6720 605f 5f69 6e69 745f 5f60 0a20  ing `__init__`. 
+00015ce0: 2020 2020 2020 2020 2020 206f 626a 6563             objec
+00015cf0: 742e 5f5f 7365 7461 7474 725f 5f28 7365  t.__setattr__(se
+00015d00: 6c66 2c20 6e61 6d65 2c20 7661 6c75 6529  lf, name, value)
+00015d10: 0a0a 0a23 2023 2043 6f6d 706c 6578 2057  ...# # Complex W
+00015d20: 6964 6765 7473 0a0a 0a63 6c61 7373 204c  idgets...class L
+00015d30: 6973 7462 6f78 436f 6e74 726f 6c28 4672  istboxControl(Fr
+00015d40: 616d 6555 6e6c 6162 656c 6c65 6429 3a0a  ameUnlabelled):.
+00015d50: 2020 2020 2727 2741 206c 6973 7462 6f78      '''A listbox
+00015d60: 2077 6964 6765 742c 2077 6974 6820 6578   widget, with ex
+00015d70: 7472 6120 636f 6e74 726f 6c73 2066 6f72  tra controls for
+00015d80: 2061 2073 6574 206f 6620 7374 7269 6e67   a set of string
+00015d90: 732e 0a0a 2020 2020 5468 6973 2069 7320  s...    This is 
+00015da0: 636f 6d70 6c65 7820 7661 7269 6174 696f  complex variatio
+00015db0: 6e20 6f6e 2060 4c69 7374 626f 7860 2c20  n on `Listbox`, 
+00015dc0: 7769 7468 2065 7874 7261 2077 6964 6765  with extra widge
+00015dd0: 7473 2066 6f72 206d 616e 6970 756c 6174  ts for manipulat
+00015de0: 696e 670a 2020 2020 7468 6520 7374 7269  ing.    the stri
+00015df0: 6e67 206c 6973 742e 2054 6869 7320 6973  ng list. This is
+00015e00: 2075 7365 6675 6c20 746f 206d 616e 6970   useful to manip
+00015e10: 756c 6174 6520 7374 7269 6e67 206c 6973  ulate string lis
+00015e20: 7473 2e0a 0a20 2020 2054 6865 2065 7874  ts...    The ext
+00015e30: 7261 2077 6964 6765 7420 636f 6e74 726f  ra widget contro
+00015e40: 6c73 2063 616e 2062 6520 6772 6f75 7065  ls can be groupe
+00015e50: 6420 6173 2066 6f6c 6c6f 7773 3a0a 0a20  d as follows:.. 
+00015e60: 2020 202d 2054 6865 7265 2069 7320 6120     - There is a 
+00015e70: 6043 6f6d 626f 626f 7860 2074 6f20 7365  `Combobox` to se
+00015e80: 6c65 6374 2074 6865 2065 6c65 6d65 6e74  lect the element
+00015e90: 2074 6f20 6164 642c 206f 7220 616e 6f74   to add, or anot
+00015ea0: 6865 7220 6275 7474 6f6e 2074 6f0a 2020  her button to.  
+00015eb0: 2020 2020 6164 6420 616c 6c20 7375 7070      add all supp
+00015ec0: 6f72 7465 6420 656c 656d 656e 7473 2e0a  orted elements..
+00015ed0: 2020 2020 2d20 5468 6572 6520 6172 6520      - There are 
+00015ee0: 6275 7474 6f6e 7320 746f 2072 656d 6f76  buttons to remov
+00015ef0: 6520 7468 6520 6375 7272 656e 746c 7920  e the currently 
+00015f00: 7365 6c65 6374 6564 2065 6c65 6d65 6e74  selected element
+00015f10: 2c20 6f72 2063 6c65 6172 2061 6c6c 0a20  , or clear all. 
+00015f20: 2020 2020 2065 6c65 6d65 6e74 732e 0a20       elements.. 
+00015f30: 2020 202d 2054 6865 7265 2061 7265 2062     - There are b
+00015f40: 7574 746f 6e73 2074 6f20 6d61 6e69 7075  uttons to manipu
+00015f50: 6c61 7465 2074 6865 206f 7264 6572 206f  late the order o
+00015f60: 6620 7468 6520 6375 7272 656e 746c 7920  f the currently 
+00015f70: 7365 6c65 6374 6564 0a20 2020 2020 2065  selected.      e
+00015f80: 6c65 6d65 6e74 2c20 7570 7761 7264 7320  lement, upwards 
+00015f90: 6f72 2064 6f77 6e77 6172 6473 2e20 436c  or downwards. Cl
+00015fa0: 6963 6b69 6e67 206f 6e20 7468 6573 6520  icking on these 
+00015fb0: 6275 7474 6f6e 7320 7769 7468 2074 6865  buttons with the
+00015fc0: 206d 6964 646c 650a 2020 2020 2020 6d6f   middle.      mo
+00015fd0: 7573 6520 6275 7474 6f6e 206d 6f76 6573  use button moves
+00015fe0: 2074 6865 2063 7572 7265 6e74 6c79 2073   the currently s
+00015ff0: 656c 6563 7465 6420 656c 656d 656e 7420  elected element 
+00016000: 746f 2074 6865 2074 6f70 206f 7220 626f  to the top or bo
+00016010: 7474 6f6d 206f 660a 2020 2020 2020 7468  ttom of.      th
+00016020: 6520 6c69 7374 2e0a 0a20 2020 2041 6c6c  e list...    All
+00016030: 2074 6865 7365 2067 726f 7570 7320 6172   these groups ar
+00016040: 6520 636f 6e66 6967 7572 6162 6c65 2c20  e configurable, 
+00016050: 7365 6520 7468 6520 6060 6275 7474 6f6e  see the ``button
+00016060: 2a60 6020 6172 6775 6d65 6e74 732e 0a0a  *`` arguments...
+00016070: 2020 2020 2e2e 206e 6f74 653a 3a0a 2020      .. note::.  
+00016080: 2020 2020 2020 5768 656e 2060 6062 7574        When ``but
+00016090: 746f 6e4f 6e65 6060 2069 7320 7365 7420  tonOne`` is set 
+000160a0: 746f 2060 4661 6c73 6560 2c20 6974 206d  to `False`, it m
+000160b0: 6967 6874 2062 6520 696e 7465 7265 7374  ight be interest
+000160c0: 696e 6720 746f 206d 6f76 650a 2020 2020  ing to move.    
+000160d0: 2020 2020 7468 6520 6275 7474 6f6e 2077      the button w
+000160e0: 6964 6765 7473 2074 6f20 7468 6520 7269  idgets to the ri
+000160f0: 6768 7420 7369 6465 2e0a 2020 2020 2020  ght side..      
+00016100: 2020 5365 7420 7468 6520 6046 7261 6d65    Set the `Frame
+00016110: 556e 6c61 6265 6c6c 6564 2e6c 6179 6f75  Unlabelled.layou
+00016120: 7460 2061 7320 6060 6c61 796f 7574 3d27  t` as ``layout='
+00016130: 6331 2c78 2760 6020 746f 2061 6368 6965  c1,x'`` to achie
+00016140: 7665 2074 6869 7320 636f 6e66 6967 7572  ve this configur
+00016150: 6174 696f 6e2e 0a0a 2020 2020 4172 6773  ation...    Args
+00016160: 3a0a 2020 2020 2020 2020 7365 6c41 6c6c  :.        selAll
+00016170: 3a20 5370 6563 6966 6963 6174 696f 6e20  : Specification 
+00016180: 666f 7220 616c 6c20 7375 7070 6f72 7465  for all supporte
+00016190: 6420 656c 656d 656e 7473 2e0a 2020 2020  d elements..    
+000161a0: 2020 2020 7365 6c4c 6973 743a 2049 6e69      selList: Ini
+000161b0: 7469 616c 2073 656c 6563 7465 6420 7374  tial selected st
+000161c0: 7269 6e67 206c 6973 742e 0a20 2020 2020  ring list..     
+000161d0: 2020 2076 6172 6961 626c 653a 2055 7365     variable: Use
+000161e0: 2061 6e20 6578 7465 726e 616c 6c79 2064   an externally d
+000161f0: 6566 696e 6564 2076 6172 6961 626c 652c  efined variable,
+00016200: 2069 6e73 7465 6164 206f 6620 6372 6561   instead of crea
+00016210: 7469 6e67 2061 206e 6577 0a20 2020 2020  ting a new.     
+00016220: 2020 2020 2020 206f 6e65 2073 7065 6369         one speci
+00016230: 6669 6320 666f 7220 7468 6973 2077 6964  fic for this wid
+00016240: 6765 742e 2050 6173 7365 6420 746f 2074  get. Passed to t
+00016250: 6865 2060 4c69 7374 626f 7860 2e0a 2020  he `Listbox`..  
+00016260: 2020 2020 2020 6c61 6265 6c3a 2054 6865        label: The
+00016270: 2068 6561 6469 6e67 2074 6578 7420 666f   heading text fo
+00016280: 7220 7468 6520 6669 7273 7420 636f 6c75  r the first colu
+00016290: 6d6e 2e20 4f70 7469 6f6e 616c 2c20 7061  mn. Optional, pa
+000162a0: 7373 6564 2074 6f20 7468 6520 604c 6973  ssed to the `Lis
+000162b0: 7462 6f78 602e 0a20 2020 2020 2020 2062  tbox`..        b
+000162c0: 7574 746f 6e4f 6e65 3a20 496e 636c 7564  uttonOne: Includ
+000162d0: 6520 6275 7474 6f6e 7320 666f 7220 6164  e buttons for ad
+000162e0: 6469 6e67 2061 2073 696e 676c 6520 656c  ding a single el
+000162f0: 656d 656e 742c 2061 6e64 2072 656d 6f76  ement, and remov
+00016300: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
+00016310: 7468 6520 7365 6c65 6374 6564 2065 6c65  the selected ele
+00016320: 6d65 6e74 2e20 5468 6973 2063 6f6e 7472  ment. This contr
+00016330: 6f6c 7320 7468 6520 6043 6f6d 626f 626f  ols the `Combobo
+00016340: 7860 2070 6c61 6365 6d65 6e74 2074 6f6f  x` placement too
+00016350: 2e0a 2020 2020 2020 2020 6275 7474 6f6e  ..        button
+00016360: 416c 6c3a 2049 6e63 6c75 6465 2062 7574  All: Include but
+00016370: 746f 6e73 2066 6f72 2061 6464 696e 6720  tons for adding 
+00016380: 616c 6c20 7375 7070 6f72 7465 6420 656c  all supported el
+00016390: 656d 656e 7473 2061 6e64 2063 6c65 616e  ements and clean
+000163a0: 0a20 2020 2020 2020 2020 2020 2061 6c6c  .            all
+000163b0: 2065 6c65 6d65 6e74 732e 2044 6566 6175   elements. Defau
+000163c0: 6c74 7320 746f 2069 6e63 6c75 6465 2e0a  lts to include..
+000163d0: 2020 2020 2020 2020 6275 7474 6f6e 4f72          buttonOr
+000163e0: 6465 723a 2049 6e63 6c75 6465 2062 7574  der: Include but
+000163f0: 746f 6e73 2074 6f20 6d61 6e69 7075 6c61  tons to manipula
+00016400: 7465 2074 6865 206f 7264 6572 206f 6620  te the order of 
+00016410: 7365 6c65 6374 6564 0a20 2020 2020 2020  selected.       
+00016420: 2020 2020 2065 6c65 6d65 6e74 2e20 4465       element. De
+00016430: 6661 756c 7473 2074 6f20 6e6f 7420 696e  faults to not in
+00016440: 636c 7564 652e 0a0a 2020 2020 5365 6520  clude...    See 
+00016450: 416c 736f 3a0a 2020 2020 2020 2020 5468  Also:.        Th
+00016460: 6520 636f 6e74 6169 6e65 7220 7769 6467  e container widg
+00016470: 6574 2069 7320 6046 7261 6d65 556e 6c61  et is `FrameUnla
+00016480: 6265 6c6c 6564 602c 2061 6e64 2074 6865  belled`, and the
+00016490: 2069 6e6e 6572 2077 6964 6765 7473 2061   inner widgets a
+000164a0: 7265 0a20 2020 2020 2020 2060 4c69 7374  re.        `List
+000164b0: 626f 7860 2028 7769 7468 2060 5363 726f  box` (with `Scro
+000164c0: 6c6c 6564 5769 6467 6574 6020 6861 6e64  lledWidget` hand
+000164d0: 6c69 6e67 292c 2060 436f 6d62 6f62 6f78  ling), `Combobox
+000164e0: 6020 616e 6420 6042 7574 746f 6e60 2e0a  ` and `Button`..
+000164f0: 2020 2020 2727 270a 2020 2020 6c61 796f      '''.    layo
+00016500: 7574 203d 2027 5231 2c78 270a 2020 2020  ut = 'R1,x'.    
+00016510: 7773 7461 7465 5f73 696e 676c 6520 3d20  wstate_single = 
+00016520: 2773 656c 6563 7465 6427 0a0a 2020 2020  'selected'..    
+00016530: 2320 4967 6e6f 7265 2074 7970 6573 2c20  # Ignore types, 
+00016540: 696e 636f 6d70 6174 6962 6c65 2077 6974  incompatible wit
+00016550: 6820 6046 7261 6d65 4c61 6265 6c6c 6564  h `FrameLabelled
+00016560: 2e73 6574 7570 5f77 6964 6765 7473 600a  .setup_widgets`.
+00016570: 2020 2020 6465 6620 7365 7475 705f 7769      def setup_wi
+00016580: 6467 6574 7328 7365 6c66 2c20 2023 2074  dgets(self,  # t
+00016590: 7970 653a 2069 676e 6f72 650a 2020 2020  ype: ignore.    
+000165a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000165b0: 2020 7365 6c41 6c6c 3a20 7370 6563 2e53    selAll: spec.S
+000165c0: 7065 6343 6f75 6e74 6162 6c65 2c20 7365  pecCountable, se
+000165d0: 6c4c 6973 743a 2074 7970 696e 672e 4f70  lList: typing.Op
+000165e0: 7469 6f6e 616c 5b74 7970 696e 672e 4974  tional[typing.It
+000165f0: 6572 6162 6c65 5b73 7472 5d5d 203d 204e  erable[str]] = N
+00016600: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+00016610: 2020 2020 2020 2020 2020 2076 6172 6961             varia
+00016620: 626c 653a 2074 7970 696e 672e 4f70 7469  ble: typing.Opti
+00016630: 6f6e 616c 5b76 6172 2e53 7472 696e 674c  onal[var.StringL
+00016640: 6973 745d 203d 204e 6f6e 652c 0a20 2020  ist] = None,.   
+00016650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016660: 2020 206c 6162 656c 3a20 7479 7069 6e67     label: typing
+00016670: 2e4f 7074 696f 6e61 6c5b 7374 725d 203d  .Optional[str] =
+00016680: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+00016690: 2020 2020 2020 2020 2020 2020 2062 7574               but
+000166a0: 746f 6e4f 6e65 3a20 626f 6f6c 203d 2054  tonOne: bool = T
+000166b0: 7275 652c 2062 7574 746f 6e41 6c6c 3a20  rue, buttonAll: 
+000166c0: 626f 6f6c 203d 2054 7275 652c 2062 7574  bool = True, but
+000166d0: 746f 6e4f 7264 6572 3a20 626f 6f6c 203d  tonOrder: bool =
+000166e0: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
+000166f0: 2020 2020 2020 2020 2020 2020 2020 2920                ) 
+00016700: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00016710: 2027 2727 2727 2720 2023 2044 6f20 6e6f   ''''''  # Do no
+00016720: 7420 646f 6375 6d65 6e74 0a20 2020 2020  t document.     
+00016730: 2020 2061 7373 6572 7420 616e 7928 2862     assert any((b
+00016740: 7574 746f 6e4f 6e65 2c20 6275 7474 6f6e  uttonOne, button
+00016750: 416c 6c2c 2062 7574 746f 6e4f 7264 6572  All, buttonOrder
+00016760: 2929 2c20 6627 7b73 656c 667d 3a20 5468  )), f'{self}: Th
+00016770: 6973 2069 7320 6a75 7374 2061 204c 6973  is is just a Lis
+00016780: 7462 6f78 270a 2020 2020 2020 2020 7365  tbox'.        se
+00016790: 6c66 2e73 656c 6563 7465 6420 3d20 5363  lf.selected = Sc
+000167a0: 726f 6c6c 6564 5769 6467 6574 2873 656c  rolledWidget(sel
+000167b0: 662c 204c 6973 7462 6f78 2c0a 2020 2020  f, Listbox,.    
+000167c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000167d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000167e0: 2020 2076 6172 6961 626c 653d 7661 7269     variable=vari
+000167f0: 6162 6c65 2c20 7365 6c65 6374 6162 6c65  able, selectable
+00016800: 3d54 7275 652c 206c 6162 656c 3d6c 6162  =True, label=lab
+00016810: 656c 2c0a 2020 2020 2020 2020 2020 2020  el,.            
+00016820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016830: 2020 2020 2020 2020 2020 2073 6372 6f6c             scrol
+00016840: 6c48 6f72 697a 6f6e 7461 6c3d 4661 6c73  lHorizontal=Fals
+00016850: 652c 2073 6372 6f6c 6c56 6572 7469 6361  e, scrollVertica
+00016860: 6c3d 4e6f 6e65 290a 2020 2020 2020 2020  l=None).        
+00016870: 7365 6c66 2e72 6d20 3d20 4275 7474 6f6e  self.rm = Button
+00016880: 2873 656c 662c 206c 6162 656c 3d27 2d27  (self, label='-'
+00016890: 2920 6966 2062 7574 746f 6e4f 6e65 2065  ) if buttonOne e
+000168a0: 6c73 6520 4e6f 6e65 0a20 2020 2020 2020  lse None.       
+000168b0: 2073 656c 662e 726d 416c 6c20 3d20 4275   self.rmAll = Bu
+000168c0: 7474 6f6e 2873 656c 662c 206c 6162 656c  tton(self, label
+000168d0: 3d27 2d2d 2d27 2920 6966 2062 7574 746f  ='---') if butto
+000168e0: 6e41 6c6c 2065 6c73 6520 4e6f 6e65 0a20  nAll else None. 
+000168f0: 2020 2020 2020 2073 656c 662e 6d6f 7665         self.move
+00016900: 446f 776e 203d 2042 7574 746f 6e28 7365  Down = Button(se
+00016910: 6c66 2c20 6c61 6265 6c3d 27e2 8693 2729  lf, label='...')
+00016920: 2069 6620 6275 7474 6f6e 4f72 6465 7220   if buttonOrder 
+00016930: 656c 7365 204e 6f6e 650a 2020 2020 2020  else None.      
+00016940: 2020 7365 6c66 2e61 6c6c 203d 2043 6f6d    self.all = Com
+00016950: 626f 626f 7828 7365 6c66 2c20 7661 6c75  bobox(self, valu
+00016960: 6573 3d73 656c 416c 6c29 2069 6620 6275  es=selAll) if bu
+00016970: 7474 6f6e 4f6e 6520 656c 7365 204e 6f6e  ttonOne else Non
+00016980: 650a 2020 2020 2020 2020 7365 6c66 2e6d  e.        self.m
+00016990: 6f76 6555 7020 3d20 4275 7474 6f6e 2873  oveUp = Button(s
+000169a0: 656c 662c 206c 6162 656c 3d27 e286 9127  elf, label='...'
+000169b0: 2920 6966 2062 7574 746f 6e4f 7264 6572  ) if buttonOrder
+000169c0: 2065 6c73 6520 4e6f 6e65 0a20 2020 2020   else None.     
+000169d0: 2020 2073 656c 662e 6164 6441 6c6c 203d     self.addAll =
+000169e0: 2042 7574 746f 6e28 7365 6c66 2c20 6c61   Button(self, la
+000169f0: 6265 6c3d 272b 2b2b 2729 2069 6620 6275  bel='+++') if bu
+00016a00: 7474 6f6e 416c 6c20 656c 7365 204e 6f6e  ttonAll else Non
+00016a10: 650a 2020 2020 2020 2020 7365 6c66 2e61  e.        self.a
+00016a20: 6464 203d 2042 7574 746f 6e28 7365 6c66  dd = Button(self
+00016a30: 2c20 6c61 6265 6c3d 272b 2729 2069 6620  , label='+') if 
+00016a40: 6275 7474 6f6e 4f6e 6520 656c 7365 204e  buttonOne else N
+00016a50: 6f6e 650a 0a20 2020 2020 2020 2023 2045  one..        # E
+00016a60: 7665 6e74 730a 2020 2020 2020 2020 6966  vents.        if
+00016a70: 2073 656c 662e 726d 3a0a 2020 2020 2020   self.rm:.      
+00016a80: 2020 2020 2020 7365 6c66 2e72 6d2e 6f6e        self.rm.on
+00016a90: 436c 6963 6b20 3d20 7365 6c66 2e6f 6e52  Click = self.onR
+00016aa0: 656d 6f76 6520 2023 2074 7970 653a 2069  emove  # type: i
+00016ab0: 676e 6f72 650a 2020 2020 2020 2020 6966  gnore.        if
+00016ac0: 2073 656c 662e 726d 416c 6c3a 0a20 2020   self.rmAll:.   
+00016ad0: 2020 2020 2020 2020 2073 656c 662e 726d           self.rm
+00016ae0: 416c 6c2e 6f6e 436c 6963 6b20 3d20 7365  All.onClick = se
+00016af0: 6c66 2e6f 6e52 656d 6f76 6541 6c6c 2020  lf.onRemoveAll  
+00016b00: 2320 7479 7065 3a20 6967 6e6f 7265 0a20  # type: ignore. 
+00016b10: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
+00016b20: 6f76 6544 6f77 6e3a 0a20 2020 2020 2020  oveDown:.       
+00016b30: 2020 2020 2073 656c 662e 6d6f 7665 446f       self.moveDo
+00016b40: 776e 2e6f 6e43 6c69 636b 203d 2073 656c  wn.onClick = sel
+00016b50: 662e 6f6e 4d6f 7665 446f 776e 2020 2320  f.onMoveDown  # 
+00016b60: 7479 7065 3a20 6967 6e6f 7265 0a20 2020  type: ignore.   
+00016b70: 2020 2020 2020 2020 2073 656c 662e 6d6f           self.mo
+00016b80: 7665 446f 776e 2e62 696e 6428 273c 4275  veDown.bind('<Bu
+00016b90: 7474 6f6e 5072 6573 732d 323e 272c 2073  ttonPress-2>', s
+00016ba0: 656c 662e 6f6e 4d6f 7665 426f 7474 6f6d  elf.onMoveBottom
+00016bb0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+00016bc0: 662e 6164 643a 0a20 2020 2020 2020 2020  f.add:.         
+00016bd0: 2020 2073 656c 662e 6164 642e 6f6e 436c     self.add.onCl
+00016be0: 6963 6b20 3d20 7365 6c66 2e6f 6e41 6464  ick = self.onAdd
+00016bf0: 2020 2320 7479 7065 3a20 6967 6e6f 7265    # type: ignore
+00016c00: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00016c10: 2e6d 6f76 6555 703a 0a20 2020 2020 2020  .moveUp:.       
+00016c20: 2020 2020 2073 656c 662e 6d6f 7665 5570       self.moveUp
+00016c30: 2e6f 6e43 6c69 636b 203d 2073 656c 662e  .onClick = self.
+00016c40: 6f6e 4d6f 7665 5570 2020 2320 7479 7065  onMoveUp  # type
+00016c50: 3a20 6967 6e6f 7265 0a20 2020 2020 2020  : ignore.       
+00016c60: 2020 2020 2073 656c 662e 6d6f 7665 5570       self.moveUp
+00016c70: 2e62 696e 6428 273c 4275 7474 6f6e 5072  .bind('<ButtonPr
+00016c80: 6573 732d 323e 272c 2073 656c 662e 6f6e  ess-2>', self.on
+00016c90: 4d6f 7665 546f 7029 0a20 2020 2020 2020  MoveTop).       
+00016ca0: 2069 6620 7365 6c66 2e61 6464 416c 6c3a   if self.addAll:
+00016cb0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00016cc0: 662e 6164 6441 6c6c 2e6f 6e43 6c69 636b  f.addAll.onClick
+00016cd0: 203d 2073 656c 662e 6f6e 4164 6441 6c6c   = self.onAddAll
+00016ce0: 2020 2320 7479 7065 3a20 6967 6e6f 7265    # type: ignore
+00016cf0: 0a0a 2020 2020 2020 2020 2320 5374 6174  ..        # Stat
+00016d00: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
+00016d10: 616c 6c20 3d20 7365 6c41 6c6c 0a20 2020  all = selAll.   
+00016d20: 2020 2020 2069 6620 7365 6c66 2e61 6c6c       if self.all
+00016d30: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00016d40: 6c66 2e61 6c6c 2e69 676e 6f72 6543 6f6e  lf.all.ignoreCon
+00016d50: 7461 696e 6572 5374 6174 6520 3d20 5472  tainerState = Tr
+00016d60: 7565 0a20 2020 2020 2020 2069 6620 7365  ue.        if se
+00016d70: 6c4c 6973 743a 0a20 2020 2020 2020 2020  lList:.         
+00016d80: 2020 2073 656c 6563 7469 6f6e 203d 206c     selection = l
+00016d90: 6973 7428 7365 6c4c 6973 7429 0a20 2020  ist(selList).   
+00016da0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+00016db0: 616c 6c28 6520 696e 2073 656c 416c 6c20  all(e in selAll 
+00016dc0: 666f 7220 6520 696e 2073 656c 6563 7469  for e in selecti
+00016dd0: 6f6e 292c 2066 2749 6e76 616c 6964 2073  on), f'Invalid s
+00016de0: 656c 4c69 7374 3a20 7b73 656c 4c69 7374  elList: {selList
+00016df0: 7d27 0a20 2020 2020 2020 2020 2020 2073  }'.            s
+00016e00: 656c 662e 7365 6c65 6374 6564 2e77 7374  elf.selected.wst
+00016e10: 6174 6520 3d20 7365 6c65 6374 696f 6e0a  ate = selection.
+00016e20: 0a20 2020 2064 6566 2073 6574 7570 5f64  .    def setup_d
+00016e30: 6566 6175 6c74 7328 7365 6c66 293a 0a20  efaults(self):. 
+00016e40: 2020 2020 2020 2023 2044 6f6e 2774 2067         # Don't g
+00016e50: 726f 7720 616e 7920 6275 7474 6f6e 730a  row any buttons.
+00016e60: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00016e70: 726d 2061 6e64 2073 656c 662e 6164 643a  rm and self.add:
+00016e80: 0a20 2020 2020 2020 2020 2020 2066 6e2e  .            fn.
+00016e90: 636f 6e66 6967 7572 6528 7365 6c66 2c0a  configure(self,.
+00016ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016eb0: 2020 2020 2020 2020 2073 656c 662e 726d           self.rm
+00016ec0: 2c20 7365 6c66 2e61 6464 2c0a 2020 2020  , self.add,.    
+00016ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ee0: 2020 2020 2063 5f72 6f77 733d 5472 7565       c_rows=True
+00016ef0: 2c20 635f 636f 6c73 3d54 7275 652c 0a20  , c_cols=True,. 
+00016f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f10: 2020 2020 2020 2020 7765 6967 6874 3d30          weight=0
+00016f20: 2c20 756e 6966 6f72 6d3d 2762 7574 746f  , uniform='butto
+00016f30: 6e5f 736d 616c 6c27 290a 2020 2020 2020  n_small').      
+00016f40: 2020 6966 2073 656c 662e 726d 416c 6c20    if self.rmAll 
+00016f50: 616e 6420 7365 6c66 2e61 6464 416c 6c3a  and self.addAll:
+00016f60: 0a20 2020 2020 2020 2020 2020 2066 6e2e  .            fn.
+00016f70: 636f 6e66 6967 7572 6528 7365 6c66 2c0a  configure(self,.
+00016f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f90: 2020 2020 2020 2020 2073 656c 662e 726d           self.rm
+00016fa0: 416c 6c2c 2073 656c 662e 6164 6441 6c6c  All, self.addAll
+00016fb0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00016fc0: 2020 2020 2020 2020 2020 2063 5f72 6f77             c_row
+00016fd0: 733d 5472 7565 2c20 635f 636f 6c73 3d54  s=True, c_cols=T
+00016fe0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+00016ff0: 2020 2020 2020 2020 2020 2020 2020 7765                we
+00017000: 6967 6874 3d30 2c20 756e 6966 6f72 6d3d  ight=0, uniform=
+00017010: 2762 7574 746f 6e5f 6269 6727 290a 0a20  'button_big').. 
+00017020: 2020 2064 6566 206f 6e41 6464 2873 656c     def onAdd(sel
+00017030: 662c 2065 7665 6e74 3a20 7479 7069 6e67  f, event: typing
+00017040: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
+00017050: 4e6f 6e65 3a0a 2020 2020 2020 2020 6173  None:.        as
+00017060: 7365 7274 2073 656c 662e 616c 6c2c 2066  sert self.all, f
+00017070: 277b 7365 6c66 7d3a 2043 616c 6c69 6e67  '{self}: Calling
+00017080: 2060 6f6e 4164 6460 2077 6974 686f 7574   `onAdd` without
+00017090: 2022 6275 7474 6f6e 4f6e 6522 2061 7267   "buttonOne" arg
+000170a0: 756d 656e 7427 0a20 2020 2020 2020 2073  ument'.        s
+000170b0: 656c 6563 7469 6f6e 203d 2073 656c 662e  election = self.
+000170c0: 616c 6c2e 7773 7461 7465 0a20 2020 2020  all.wstate.     
+000170d0: 2020 2061 6c6c 656c 656d 656e 7473 203d     allelements =
+000170e0: 2073 656c 662e 7365 6c65 6374 6564 2e77   self.selected.w
+000170f0: 7374 6174 650a 2020 2020 2020 2020 6966  state.        if
+00017100: 2073 656c 6563 7469 6f6e 206e 6f74 2069   selection not i
+00017110: 6e20 616c 6c65 6c65 6d65 6e74 733a 0a20  n allelements:. 
+00017120: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00017130: 7365 6c65 6374 6564 2e77 7374 6174 6520  selected.wstate 
+00017140: 3d20 282a 616c 6c65 6c65 6d65 6e74 732c  = (*allelements,
+00017150: 2073 656c 6563 7469 6f6e 290a 0a20 2020   selection)..   
+00017160: 2064 6566 206f 6e41 6464 416c 6c28 7365   def onAddAll(se
+00017170: 6c66 2c20 6576 656e 743a 2074 7970 696e  lf, event: typin
+00017180: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
+00017190: 204e 6f6e 653a 0a20 2020 2020 2020 2073   None:.        s
+000171a0: 656c 662e 7365 6c65 6374 6564 2e77 7374  elf.selected.wst
+000171b0: 6174 6520 3d20 7365 6c66 2e5f 616c 6c2e  ate = self._all.
+000171c0: 616c 6c28 290a 0a20 2020 2064 6566 206f  all()..    def o
+000171d0: 6e52 656d 6f76 6528 7365 6c66 2c20 6576  nRemove(self, ev
+000171e0: 656e 743a 2074 7970 696e 672e 416e 7920  ent: typing.Any 
+000171f0: 3d20 4e6f 6e65 2920 2d3e 204e 6f6e 653a  = None) -> None:
+00017200: 0a20 2020 2020 2020 2073 656c 6563 7469  .        selecti
+00017210: 6f6e 203d 2073 656c 662e 7365 6c65 6374  on = self.select
+00017220: 6564 2e77 7365 6c65 6374 696f 6e28 290a  ed.wselection().
+00017230: 2020 2020 2020 2020 6966 2073 656c 6563          if selec
+00017240: 7469 6f6e 3a0a 2020 2020 2020 2020 2020  tion:.          
+00017250: 2020 616c 6c65 6c65 6d65 6e74 7320 3d20    allelements = 
+00017260: 7365 6c66 2e73 656c 6563 7465 642e 7773  self.selected.ws
+00017270: 7461 7465 0a20 2020 2020 2020 2020 2020  tate.           
+00017280: 2069 6620 7365 6c65 6374 696f 6e20 696e   if selection in
+00017290: 2061 6c6c 656c 656d 656e 7473 3a0a 2020   allelements:.  
+000172a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000172b0: 6c66 2e73 656c 6563 7465 642e 7773 7461  lf.selected.wsta
+000172c0: 7465 203d 2028 7320 666f 7220 7320 696e  te = (s for s in
+000172d0: 2061 6c6c 656c 656d 656e 7473 2069 6620   allelements if 
+000172e0: 7320 213d 2073 656c 6563 7469 6f6e 290a  s != selection).
+000172f0: 0a20 2020 2064 6566 206f 6e52 656d 6f76  .    def onRemov
+00017300: 6541 6c6c 2873 656c 662c 2065 7665 6e74  eAll(self, event
+00017310: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
+00017320: 6f6e 6529 202d 3e20 4e6f 6e65 3a0a 2020  one) -> None:.  
+00017330: 2020 2020 2020 7365 6c66 2e73 656c 6563        self.selec
+00017340: 7465 642e 7773 7461 7465 203d 205b 5d0a  ted.wstate = [].
+00017350: 0a20 2020 2064 6566 206f 6e4d 6f76 6528  .    def onMove(
+00017360: 7365 6c66 2c20 6465 6c74 613a 2074 7970  self, delta: typ
+00017370: 696e 672e 556e 696f 6e5b 696e 742c 2074  ing.Union[int, t
+00017380: 7970 696e 672e 4c69 7465 7261 6c5b 2774  yping.Literal['t
+00017390: 6f70 275d 2c20 7479 7069 6e67 2e4c 6974  op'], typing.Lit
+000173a0: 6572 616c 5b27 626f 7474 6f6d 275d 5d29  eral['bottom']])
+000173b0: 3a0a 2020 2020 2020 2020 6173 7365 7274  :.        assert
+000173c0: 2064 656c 7461 2021 3d20 300a 2020 2020   delta != 0.    
+000173d0: 2020 2020 7377 6964 6765 7420 3d20 7365      swidget = se
+000173e0: 6c66 2e73 656c 6563 7465 640a 2020 2020  lf.selected.    
+000173f0: 2020 2020 7365 6c65 6374 696f 6e20 3d20      selection = 
+00017400: 7377 6964 6765 742e 7773 656c 6563 7469  swidget.wselecti
+00017410: 6f6e 2829 0a20 2020 2020 2020 2023 2054  on().        # T
+00017420: 4f44 4f3a 2054 6573 7420 7468 6973 2c20  ODO: Test this, 
+00017430: 6074 6573 7473 2f74 6573 745f 7769 6467  `tests/test_widg
+00017440: 6574 5f6c 6973 7462 6f78 2e70 7960 0a20  et_listbox.py`. 
+00017450: 2020 2020 2020 2069 6620 7365 6c65 6374         if select
+00017460: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
+00017470: 2077 7369 6420 3d20 7377 6964 6765 742e   wsid = swidget.
+00017480: 7773 6964 2829 0a20 2020 2020 2020 2020  wsid().         
+00017490: 2020 2069 6620 6465 6c74 6120 3d3d 2027     if delta == '
+000174a0: 746f 7027 3a0a 2020 2020 2020 2020 2020  top':.          
+000174b0: 2020 2020 2020 6e65 7769 6478 203d 2030        newidx = 0
+000174c0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+000174d0: 6620 6465 6c74 6120 3d3d 2027 626f 7474  f delta == 'bott
+000174e0: 6f6d 273a 0a20 2020 2020 2020 2020 2020  om':.           
+000174f0: 2020 2020 206e 6577 6964 7820 3d20 6c65       newidx = le
+00017500: 6e28 7377 6964 6765 742e 7773 7461 7465  n(swidget.wstate
+00017510: 2920 2d20 310a 2020 2020 2020 2020 2020  ) - 1.          
+00017520: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00017530: 2020 2020 2020 2020 6f6c 6469 6478 203d          oldidx =
+00017540: 2073 7769 6467 6574 2e69 6e64 6578 2877   swidget.index(w
+00017550: 7369 6429 0a20 2020 2020 2020 2020 2020  sid).           
+00017560: 2020 2020 206e 6577 6964 7820 3d20 6f6c       newidx = ol
+00017570: 6469 6478 202b 2064 656c 7461 0a20 2020  didx + delta.   
+00017580: 2020 2020 2020 2020 2069 6620 7377 6964           if swid
+00017590: 6765 742e 656c 656d 656e 745f 6d6f 7665  get.element_move
+000175a0: 2877 7369 642c 206e 6577 6964 7829 3a0a  (wsid, newidx):.
+000175b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000175c0: 2320 5265 2d53 656c 6563 7420 7468 6520  # Re-Select the 
+000175d0: 6f6c 6420 656c 656d 656e 740a 2020 2020  old element.    
+000175e0: 2020 2020 2020 2020 2020 2020 7377 6964              swid
+000175f0: 6765 742e 7773 656c 2877 7369 6429 0a0a  get.wsel(wsid)..
+00017600: 2020 2020 6465 6620 6f6e 4d6f 7665 5570      def onMoveUp
+00017610: 2873 656c 662c 2065 7665 6e74 3d4e 6f6e  (self, event=Non
+00017620: 6529 3a0a 2020 2020 2020 2020 7265 7475  e):.        retu
+00017630: 726e 2073 656c 662e 6f6e 4d6f 7665 282d  rn self.onMove(-
+00017640: 3129 0a0a 2020 2020 6465 6620 6f6e 4d6f  1)..    def onMo
+00017650: 7665 546f 7028 7365 6c66 2c20 6576 656e  veTop(self, even
+00017660: 743d 4e6f 6e65 293a 0a20 2020 2020 2020  t=None):.       
+00017670: 2072 6574 7572 6e20 7365 6c66 2e6f 6e4d   return self.onM
+00017680: 6f76 6528 2774 6f70 2729 0a0a 2020 2020  ove('top')..    
+00017690: 6465 6620 6f6e 4d6f 7665 446f 776e 2873  def onMoveDown(s
+000176a0: 656c 662c 2065 7665 6e74 3d4e 6f6e 6529  elf, event=None)
+000176b0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+000176c0: 2073 656c 662e 6f6e 4d6f 7665 282b 3129   self.onMove(+1)
+000176d0: 0a0a 2020 2020 6465 6620 6f6e 4d6f 7665  ..    def onMove
+000176e0: 426f 7474 6f6d 2873 656c 662c 2065 7665  Bottom(self, eve
+000176f0: 6e74 3d4e 6f6e 6529 3a0a 2020 2020 2020  nt=None):.      
+00017700: 2020 7265 7475 726e 2073 656c 662e 6f6e    return self.on
+00017710: 4d6f 7665 2827 626f 7474 6f6d 2729 0a    Move('bottom').
```

### Comparing `tkmilan-0.8/src/tkmilan/__main__.py` & `tkmilan-0.9/src/tkmilan/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from functools import wraps
 from datetime import datetime
 import random
 
 import tkinter as tk
 from . import MODULES_VERBOSE
 from . import RootWindow, FrameUnlabelled, FrameLabelled, FrameStateful, FramePaned, Notebook, NotebookUniform, ScrolledWidget
-from . import Button, Checkbox, Entry, Label, LabelStateful, Listbox, Combobox, ComboboxMap, EntryMultiline, Tree
+from . import Button, Checkbox, Entry, Label, LabelStateful, Listbox, Combobox, ComboboxMap, EntryMultiline, Tree, ListboxControl
 from . import var, spec, fn
 from .model import CP, BindingGlobal, Timeout, TimeoutIdle, FileType, FileTypes
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -31,14 +31,16 @@
     def onClick_lb(self, vobj, etype, *, idx):
         pass
         # logger.debug('Clicked on "%s" @ %s:%s', idx, vobj, etype)
         # logger.debug('- State: %r', vobj.get())
 
 
 class ListFrame_Inner(FrameStateful):
+    wstate_single = 'e'
+
     def __init__(self, *args, label, **kwargs):
         super().__init__(*args, label=label, labelInner=label, **kwargs)
 
     def setup_widgets(self, labelInner):
         self.lbl = Label(self, label=f'Label: {labelInner}')
         self.e = Entry(self)  # label=f'Entry: {labelInner}'
 
@@ -88,15 +90,15 @@
         self.bChoice = Button(self, label='CB=2')
         self.i_choice = ComboboxMap(self, values=i_choices)  # label='CB(int)'
 
         self.rstateful = ListFrame_Outer(self, labelAnchor=CP.N,
                                          cbox1=cbox1)
 
     def setup_layout(self, layout):
-        self.rowconfigure(self.cLst.grid_info().get('row'), weight=0)
+        fn.configure(self, self.cLst, rows=True, weight=0)
 
     def setup_defaults(self):
         self.fill_lst()
         # Events
         self.bFill.onClick = self.fill_lst
         self.bCheck.onClick = self.check_lst
         self.bChoice.onClick = self.i_choice.eSetValue(2)
@@ -137,14 +139,15 @@
         self.bNoOp = Button(self, label='noop')
         self.u_bool = Checkbox(self, variable=what_bool, label='Upstream "bool"')
         self.bNoOp_Big = Button(self, label='No Operation')
 
 
 class NB_Child_Simple(FrameUnlabelled):
     layout = 'Rx,1'
+    wstate_single = 'e'
 
     def setup_widgets(self, label):
         w = {}
         for n in range(5):
             w[f'n{n}'] = Label(self, label=f'{n}: {label}')
         w['e'] = LabelStateful(self)  # label=f'LS #{n}'
         return w
@@ -326,14 +329,15 @@
         self.timeout_d = NB_Child_Timeout_Delay(self)
         self.timeout_idle_d = NB_Child_TimeoutIdle_Delay(self)
         self.timeout_idle_c = NB_Child_TimeoutIdle_Chain(self)
 
 
 class NB_Child_Dialog(FrameUnlabelled):
     layout = 'Rx,1'
+    wstate_single = 'txt'
 
     def setup_widgets(self):
         self.ds = Button(self, label='D S')
         self.dl = Button(self, label='D L')
         self.fs = Button(self, label='F S')
         self.fl = Button(self, label='F L')
         self.flc = Button(self, label='F L(py)')
@@ -368,14 +372,15 @@
                             'Python': FileType('py'),
                             'TOML': FileType('toml'),
                         }))
 
 
 class NB_Child_Scrollbars(FrameUnlabelled):
     layout = 'R2,x'
+    wstate_single = 'slst'
 
     def setup_widgets(self):
         self.randomize = Button(self, label='Randomize List Size')
         self.setscrolls = Button(self, label='Toggle Scrollbars')
 
         vSlist = self.var(var.StringList, name='slst')
         self.sbL = ScrolledWidget(self, Listbox,
@@ -403,37 +408,57 @@
         self.sbL.set_scroll_state(True, True)
         # sbC: Manual, Set True (no-op)
         self.sbC.set_scroll_state(True, True)
         # sbR: Manual, Set Reversed
         self.sbR.set_scroll_state(*(not b for b in self.sbR.get_scroll_state()))
 
 
+class NB_Child_ListboxSet(FrameUnlabelled):
+    layout = tk.HORIZONTAL
+
+    def setup_widgets(self):
+        ls_all = spec.StaticList((f'String {idx:02}' for idx in range(1, 20 + 1)), defaultIndex=0)
+
+        ls_selected = random.sample(list(ls_all.all()), k=5)
+        self.left = ListboxControl(self,
+                                   selAll=ls_all)
+        self.right = ListboxControl(self, layout='c1,x', label='Full Control',
+                                    selAll=ls_all, selList=ls_selected,
+                                    buttonOne=False, buttonAll=True, buttonOrder=True)
+
+    def setup_defaults(self):
+        self.left.onAddAll()
+
+
 class NB(Notebook):
     def setup_tabs(self):
         logger.debug('» %r', self)
         # TODO: Test images, etc.
+
         return {
             'sb': Notebook.Tab('Scrollbars', NB_Child_Scrollbars(self)),
             'tt': Notebook.Tab('Timeouts', NB_Child_Timeouts(self),
                                image=self.wimage('info-s16'), labelPosition=CP.E),  # Default labelPosition
             'td': Notebook.Tab('Dialogues', NB_Child_Dialog(self),
                                image=self.wimage('info-msgbox-s16'), labelPosition=True),  # Only image
             'tc': Notebook.Tab('Tab Complex', NB_Child_Complex(self),
                                image=self.wimage('info-s16'), labelPosition=CP.W),  # "Reverse" labelPosition
             't1': Notebook.Tab('Tab 1', NB_Child_Simple(self, label='Tab 1')),
             't2': Notebook.Tab('Tab 2', NB_Child_Simple(self, label='Tab 2')),
+            'c:lc': Notebook.Tab('Complex ListboxControl', NB_Child_ListboxSet(self)),
         }
 
     def setup_adefaults(self):
-        self.wselect('sb')
+        self.wselect('c:lc')
 
 
 class TextEditor(FrameStateful):
     label = 'LTML'
     layout = 'Rx,1'
+    wstate_single = 'txt'
 
     def setup_widgets(self):
         self.bTxtClean = Button(self, label='Clean TXT')
         self.bTxtReset = Button(self, label='Reset TXT')
         self.bTxtSet = Button(self, label='Set TXT')
         self.txt = ScrolledWidget(self, EntryMultiline,
                                   setgrid=False)
@@ -544,22 +569,25 @@
         string = tk.simpledialog.askstring('Set Contents', f'Set the "{self.e1.label}" contents')
         if string is not None:
             self.e1.wstate = string
 
     def debug(self):
         from pprint import pformat
         logging.info('=> State @ %s[%r]', self, self)
-        for line in pformat(self.wstate).splitlines():
+        for line in pformat(self.wstate_get()).splitlines():  # No `.wstate` for better tracebacks
             logging.info('%s', line)
         # logging.info('=> State @ ubox')
         # for line in pformat(self.ubox.wstate).splitlines():
         #     logging.info('%s', line)
         # logging.info('=> State @ lf.cLst')
         # for line in pformat(self.lf.cLst.wstate).splitlines():
         #     logging.info('%s', line)
+        # logging.info('=> State @ nb[c:lc]')
+        # for line in pformat(self.nb.wtab('c:lc').wstate).splitlines():
+        #     logging.info('%s', line)
         logging.info('=> State Set')
         new = self.wstate
         for b in ('0', '12'):
             new['lbs'][f'lb:{b}'] = not new['lbs'][f'lb:{b}']
         self.wstate = new
         logging.info('=> GUI States')
         logging.info('   GUI State @ %s[%r]', self, self)
```

### Comparing `tkmilan-0.8/src/tkmilan/fn.py` & `tkmilan-0.9/src/tkmilan/fn.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,61 +43,91 @@
 
     This should be used by a frame to calculate its grid size,
     by checking the values for all its children widgets.
 
     Args:
         widgets: Widgets in the same grid. There should be at least one.
     """
-    def maxs(w):
-        assert isinstance(w, tk.Widget), f'Invalid Widget: {w!r}'
-        info = w.grid_info()
+    def maxs(w: 'mixin.MixinWidget') -> typing.Tuple[int, int]:
+        info = w.wgrid
         # logger.debug(f'=> Grid Info: {info}')
-        # If the grid information doesn't exist, default to a single frame
-        # Force elements to integer, on tcl v8.5 they are returned as strings
-        r = int(info.get('row', 0)) + int(info.get('rowspan', 1)) - 1
-        c = int(info.get('column', 0)) + int(info.get('columnspan', 1)) - 1
-        return (r, c)
+        if info is None:
+            return (-1, -1)  # Not included on a grid yet
+        else:
+            return (info.row + info.rowspan - 1, info.column + info.columnspan - 1)
     if __debug__:
         parents = set()
         for w in widgets:
             if w.wparent:
                 parents.add(w.wparent)
-        assert len(parents) == 1, f'Grid Size only for sibling widgets. Parents {parents}'
+        assert len(parents) == 1, f'Grid Size only for sibling widgets. Parents: {parents}'
     m = [maxs(w) for w in widgets]
     num_columns = max([w[1] for w in m]) + 1
     num_rows = max([w[0] for w in m]) + 1
     return model.GridSize(rows=num_rows, columns=num_columns)
 
 
-def configure_grid(master: 'mixin.ContainerWidget', column_weights: typing.Sequence[int], row_weights: typing.Sequence[int], **kwargs) -> None:
+def configure_grid(master: 'mixin.ContainerWidget',
+                   column_weights: typing.Sequence[int], row_weights: typing.Sequence[int],
+                   **kwargs: typing.Mapping[str, typing.Any]) -> None:
     """Configure the grid.
 
     Weights can be:
 
         - ``0`` : Fit the widgets, never resize
         - ``>0``: Resize with this number as weight
 
-    Make sure to include all columns and rows. When in doubt, use 0
+    Make sure to include all columns and rows. When in doubt, use 0.
 
     Args:
         column_weights: List of column weights
         row_weights: List of row weights
-        kwargs: Extra arguments to `columnconfigure
-            <https://www.tcl.tk/man/tcl/TkCmd/grid.html#M8>`_/`rowconfigure
-            <https://www.tcl.tk/man/tcl/TkCmd/grid.html#M24>`_ function.
+        kwargs: Extra arguments to the configuration functions
+            `columnconfigure <https://www.tcl.tk/man/tcl/TkCmd/grid.html#M8>`_
+            /
+            `rowconfigure <https://www.tcl.tk/man/tcl/TkCmd/grid.html#M24>`_.
     """
     if __debug__:
         gw = master.gsize
         gr = model.GridSize(rows=len(row_weights), columns=len(column_weights))
         assert gw == gr, f'{master!r}: Invalid grid size: W::{gw} R::{gr}'
     assert isinstance(master, (tk.Widget, tk.Tk)), f'{master} is not a valid tkinter.Widget'
     for col, w in enumerate(column_weights):
-        master.columnconfigure(col, weight=w, **kwargs)
+        master.columnconfigure(col, weight=w, **kwargs)  # type: ignore  # Invalid Types
     for row, h in enumerate(row_weights):
-        master.rowconfigure(row, weight=h, **kwargs)
+        master.rowconfigure(row, weight=h, **kwargs)  # type: ignore  # Invalid Types
+
+
+def configure(master: 'mixin.ContainerWidget',
+              *widgets: 'mixin.MixinWidget',
+              c_rows: bool = False, c_cols: bool = False,
+              **kwargs: typing.Mapping[str, typing.Any]) -> None:
+    '''Configure the rows and columns for the given widgets.
+
+    For widgets that span more than one row or column, the settings are changed
+    for all rows or columns.
+
+    Args:
+        widgets: Widgets to consider.
+        c_rows: Configure the rows
+        c_cols: Configure the columns
+        kwargs: Arguments passed to the configuration functions:
+            `columnconfigure <https://www.tcl.tk/man/tcl/TkCmd/grid.html#M8>`_
+            /
+            `rowconfigure <https://www.tcl.tk/man/tcl/TkCmd/grid.html#M24>`_.
+    '''
+    assert isinstance(master, (tk.Widget, tk.Tk)), f'{master} is not a valid tkinter.Widget'
+    for w in widgets:
+        wgrid = w.wgrid
+        if wgrid and c_rows:
+            for r in range(wgrid.row, wgrid.row + wgrid.rowspan):
+                master.rowconfigure(r, **kwargs)  # type: ignore  # Invalid Types
+        if wgrid and c_cols:
+            for c in range(wgrid.column, wgrid.column + wgrid.columnspan):
+                master.columnconfigure(c, **kwargs)  # type: ignore  # Invalid Types
 
 
 def generate_trace(variable: tk.Variable, function: typing.Callable, **kwargs):
     '''Generate an internal trace callback.
 
     The function generated here should be attached to the ``Tk`` event.
     '''
```

### Comparing `tkmilan-0.8/src/tkmilan/mixin.py` & `tkmilan-0.9/src/tkmilan/mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -166,51 +166,75 @@
     '''Mixin class for container widgets.
 
     Note:
         When subclassing this, define `MixinState.setup_state` to return a
         dictionary mapping subwidget identifier to `WidgetDynamicState`.
     '''
     wstate_static: bool = False
+    wstate_single: typing.Optional[str] = None
+    '''
+    Mark the container state as "single", including only the state for this child.
+
+    Should only be enabled where there is a single child element, this is
+    verified when getting the value. Use `MixinWidget.ignoreContainerState` to
+    ignore other widgets.
+
+    This creates no performance improvements, it is only useful to simplify the
+    state.
+    '''
 
     def state_get(self, **kwargs):
         state = {}
         for identifier, wds in self.stateSetup(**kwargs).items():
             result = wds.getter()
             if wds.noneable and result is None:
                 pass  # Skip
             else:
                 state[identifier] = result
-        if len(state) == 0:
-            return None
+        if self.wstate_single is not None:
+            assert len(state) == 1, f'{self}: Invalid "wstate_single" marking, {len(state)} elements'
+            return state[self.wstate_single]
         else:
-            return state
+            if len(state) == 0:
+                return None
+            else:
+                if __debug__:
+                    if len(state) == 1:
+                        logger.warning('%s: This widget can be marked "wstate_single": `%s`', self, list(state)[0])
+                return state
 
     def state_set(self, state, substate, **kwargs) -> None:
         # # Debug container state flow
         # self_names = None
         # if __debug__:
         #     self_names = str(self).split('.')[1:]
-        #     logger.debug('%s: %s', '>' * len(self_names), self)
+        #     logger.debug('%s: %s%s',
+        #                  '>' * len(self_names),
+        #                  self,
+        #                  '' if self.wstate_single is None else f' [{self.wstate_single}]',
+        #                  )
         for identifier, wds in self.stateSetup(**kwargs).items():
-            if (wds.noneable and state is None) or ((substate or wds.noneable) and identifier not in state):
+            skip = (wds.noneable and state is None) or \
+                ((substate or wds.noneable) and identifier not in state) or \
+                (self.wstate_single is not None and self.wstate_single != identifier)
+            if skip:
                 # if __debug__:
                 #     logger.debug('%s|> Skip "%s"', ' ' * len(self_names), identifier)
                 pass
             else:
+                # if __debug__:
+                #     logger.debug('%s|>  Set "%s"', ' ' * len(self_names), identifier)
+                if self.wstate_single:
+                    widget_state = state
+                else:
+                    widget_state = state[identifier]
                 if wds.container:
-                    wds.setter(state[identifier], substate, **kwargs)
+                    wds.setter(widget_state, substate, **kwargs)
                 else:
-                    wds.setter(state[identifier])
-
-    def IgnoreWidgets(self, *ignored):
-        '''
-        Wrap `MixinState.setup_state`, ignoring some widgets.
-        '''
-        state = super().setup_state()
-        return {i: w for i, w in state if w not in ignored}
+                    wds.setter(widget_state)
 
 
 class MixinWidget:
     '''Parent class of all widgets.
 
     Args:
         gkeys: Append widget-specific `GuiState` keys to common list
@@ -222,14 +246,16 @@
 
     wparent: 'typing.Optional[MixinWidget]' = None
     '''A reference to the parent widget.'''
     gkeys: typing.FrozenSet[str]
     '''The supported `GuiState` keys.'''
     isHelper: bool
     '''Marker that indicates the widgets is not part of the automatic state.'''
+    ignoreContainerState: bool = False
+    '''Ignore this widget's state when included on a container.'''
     _bindings: typing.MutableMapping[str, model.Binding]
     '''Store all widget `Binding` objects, keyed by name (see `binding`).'''
     _tidles: typing.MutableMapping[str, model.TimeoutIdle]
     '''Store some widget `TimeoutIdle` objects, keyed by name (see `tidle`).'''
 
     def __init__(self, *, gkeys: typing.Iterable[str] = None):
         self.isHelper: bool = getattr(self, 'isHelper', False)
@@ -344,21 +370,57 @@
 
         ``fmt`` can be given as a `model.GridCoordinates`, or as a single
         `str`, to be parsed by `model.GridCoordinates.parse`.
 
         Args:
             fmt: The grid configuration format. Specified above.
             kwargs: Passed upstream
+
+        See Also:
+            `wgrid`: Get the current widget grid coordinates.
         '''
         assert isinstance(self, (tk.Widget, tk.Tk)), f'{self} is not a valid tkinter.Widget'
         if isinstance(fmt, str):
             fmt = model.GridCoordinates.parse(fmt)
         kwargs.update(fmt.dict())
         self.grid(**kwargs)
 
+    @property
+    def wgrid(self) -> typing.Optional[model.GridCoordinates]:
+        '''Get the widget grid coordinates, if the widget is visible.
+
+        Returns:
+            Return a `model.GridCoordinates` object with the widget information. If
+            the wiget was hidden, return `None`.
+
+            This is also available for the root widget (`wroot`) for
+            completeness, but that doesn't really correspond to any grid,
+            return `None`.
+
+        See Also:
+            `setup_grid`: Change the widget grid coordinates.
+        '''
+        if self == self.wroot:
+            assert isinstance(self, tk.Tk)
+            return None
+        else:
+            assert isinstance(self, tk.Widget), f'{self} is not a valid tkinter.Widget'
+            # If the grid information doesn't exist, default to a single frame
+            # Force elements to integer, on tcl v8.5 they are returned as strings
+            ginfo = self.grid_info()
+            if ginfo:
+                return model.GridCoordinates(
+                    row=int(ginfo.get('row', 0)),
+                    rowspan=int(ginfo.get('rowspan', 1)),
+                    column=int(ginfo.get('column', 0)),
+                    columnspan=int(ginfo.get('columnspan', 1)),
+                )
+            else:
+                return None
+
     def get_gui_state(self) -> model.GuiState:
         if __debug__:
             from . import RootWindow  # For typechecking
         assert isinstance(self, (tk.ttk.Widget, RootWindow)), f'{self} is not a valid tkinter.ttk.Widget'
         state: typing.MutableMapping[str, typing.Optional[bool]] = {}
         for estr in self.gkeys:
             itk = model.GUI_STATES[estr]
@@ -702,14 +764,17 @@
         wvariables = {}
         vid_upstream = set(vid_upstream or ())
         vid_variables = set(fn.vname(v) for v in self._variables.values())
         vwidgets = collections.defaultdict(lambda: [])
         # logger.debug('%r START | %r', self, vid_upstream)
         for name, widget in self.widgets.items():
             # logger.debug('%s: %r', name, widget)
+            if widget.ignoreContainerState:
+                # logger.debug('| Skipping Widget')
+                continue
             if isinstance(widget, SingleWidget):
                 assert widget.variable is not None
                 vid = fn.vname(widget.variable)
                 # logger.debug('| Variable: %s[%r]', vid, widget.variable)
                 if vid in vid_upstream:
                     # logger.debug('  @Upstream, skipping')
                     continue
```

### Comparing `tkmilan-0.8/src/tkmilan/model.py` & `tkmilan-0.9/src/tkmilan/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,20 +28,27 @@
 TraceModeT = typing.Literal['read', 'write', 'unset']
 '''The supported operations to watch for a trace.
 
 There is no Python documentation, see ``Tk`` `trace variable <https://www.tcl.tk/man/tcl/TclCmd/trace.html#M14>`_ documentation.
 '''
 
 
-# Support more image types with Pillow:
-# https://pillow.readthedocs.io/en/stable/reference/ImageTk.html
-IMAGE_TYPES = {
-    'gif': tk.PhotoImage,
-    'png': tk.PhotoImage,
+# Image Types
+__image_types = {
 }
+# TODO: Support more image types with Pillow:
+# - See https://pillow.readthedocs.io/en/stable/reference/ImageTk.html
+# PNG is only supported on "tk8.6"
+# - Gated by Tk version
+if util.TK_VERSION >= (8, 6):
+    __image_types['png'] = tk.PhotoImage
+# GIF is supported everywhere
+__image_types['gif'] = tk.PhotoImage
+
+IMAGE_TYPES = __image_types
 '''Supported image types, and corresponding loaders.
 
 See `ImageCache`.
 '''
 
 
 logger = logging.getLogger(__name__)
@@ -1085,15 +1092,15 @@
 class TreeElement:
     '''Information for each `tkmilan.Tree` record.
 
     Technically, this is not enough to reconstruct the entire tree, but it
     should.
 
     The ``image`` argument is optional, but when created, no resizing is performed.
-    By default, the ideal image size is `16x16` pixels.
+    By default, the ideal image size is ``16x16`` pixels.
 
     Args:
         label: The leftmost string shown on the first column. This identifies the entire record.
         columns: A list of strings corresponding to the column data.
             Optional, defaults to `None`.
         children: A list of `TreeElement`, to be shown as children of this
             `TreeElement`. This can recurse without limit.
```

### Comparing `tkmilan-0.8/src/tkmilan/parser.py` & `tkmilan-0.9/src/tkmilan/parser.py`

 * *Files identical despite different names*

### Comparing `tkmilan-0.8/src/tkmilan/showcase-images/error-s16.png` & `tkmilan-0.9/src/tkmilan/showcase-images/error-s16.png`

 * *Files identical despite different names*

### Comparing `tkmilan-0.8/src/tkmilan/showcase-images/warning-s16.png` & `tkmilan-0.9/src/tkmilan/showcase-images/warning-s16.png`

 * *Files identical despite different names*

### Comparing `tkmilan-0.8/src/tkmilan/spec.py` & `tkmilan-0.9/src/tkmilan/spec.py`

 * *Files identical despite different names*

### Comparing `tkmilan-0.8/src/tkmilan/var.py` & `tkmilan-0.9/src/tkmilan/var.py`

 * *Files identical despite different names*

### Comparing `tkmilan-0.8/src/tkmilan.egg-info/PKG-INFO` & `tkmilan-0.9/src/tkmilan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkmilan
-Version: 0.8
+Version: 0.9
 Summary: tkinter's evil twin
 Home-page: https://support.powertools-tech.com/PowertoolsTech/tkmilan
 Author: Powertools Technologies
 Author-email: simao.afonso@powertools-tech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tkmilan-0.8/src/tkmilan.egg-info/SOURCES.txt` & `tkmilan-0.9/src/tkmilan.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -40,8 +40,9 @@
 src/tkmilan.egg-info/top_level.txt
 src/tkmilan/showcase-images/README.md
 src/tkmilan/showcase-images/error-s16.png
 src/tkmilan/showcase-images/info-msgbox-s16.png
 src/tkmilan/showcase-images/info-s16.png
 src/tkmilan/showcase-images/warning-s16.png
 tests/test_model.py
-tests/test_parser_ltml.py
+tests/test_parser_ltml.py
+tests/test_widget_listbox.py
```

### Comparing `tkmilan-0.8/tests/test_model.py` & `tkmilan-0.9/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `tkmilan-0.8/tests/test_parser_ltml.py` & `tkmilan-0.9/tests/test_parser_ltml.py`

 * *Files identical despite different names*

