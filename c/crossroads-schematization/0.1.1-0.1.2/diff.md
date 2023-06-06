# Comparing `tmp/crossroads-schematization-0.1.1.tar.gz` & `tmp/crossroads-schematization-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossroads-schematization-0.1.1.tar", last modified: Tue Jun  6 15:33:59 2023, max compression
+gzip compressed data, was "crossroads-schematization-0.1.2.tar", last modified: Tue Jun  6 15:48:46 2023, max compression
```

## Comparing `crossroads-schematization-0.1.1.tar` & `crossroads-schematization-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-06 15:33:59.892695 crossroads-schematization-0.1.1/
--rw-r--r--   0 jm        (1000) jm        (1000)      107 2022-11-30 16:15:16.000000 crossroads-schematization-0.1.1/MANIFEST.in
--rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-06-06 15:33:59.892695 crossroads-schematization-0.1.1/PKG-INFO
--rw-r--r--   0 jm        (1000) jm        (1000)     2897 2022-11-30 16:53:52.000000 crossroads-schematization-0.1.1/README.md
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-06 15:33:59.888695 crossroads-schematization-0.1.1/crossroads_schematization.egg-info/
--rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-06-06 15:33:59.000000 crossroads-schematization-0.1.1/crossroads_schematization.egg-info/PKG-INFO
--rw-r--r--   0 jm        (1000) jm        (1000)      794 2023-06-06 15:33:59.000000 crossroads-schematization-0.1.1/crossroads_schematization.egg-info/SOURCES.txt
--rw-r--r--   0 jm        (1000) jm        (1000)        1 2023-06-06 15:33:59.000000 crossroads-schematization-0.1.1/crossroads_schematization.egg-info/dependency_links.txt
--rw-r--r--   0 jm        (1000) jm        (1000)       98 2023-06-06 15:33:59.000000 crossroads-schematization-0.1.1/crossroads_schematization.egg-info/entry_points.txt
--rw-r--r--   0 jm        (1000) jm        (1000)        8 2023-06-06 15:33:59.000000 crossroads-schematization-0.1.1/crossroads_schematization.egg-info/top_level.txt
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-06 15:33:59.892695 crossroads-schematization-0.1.1/crschem/
--rw-r--r--   0 jm        (1000) jm        (1000)       22 2023-06-06 15:33:21.000000 crossroads-schematization-0.1.1/crschem/__init__.py
--rw-r--r--   0 jm        (1000) jm        (1000)     6727 2023-06-06 12:30:02.000000 crossroads-schematization-0.1.1/crschem/cmd.py
--rw-r--r--   0 jm        (1000) jm        (1000)    51224 2023-06-06 12:40:32.000000 crossroads-schematization-0.1.1/crschem/crossroad.py
--rw-r--r--   0 jm        (1000) jm        (1000)    23404 2023-06-06 15:32:38.000000 crossroads-schematization-0.1.1/crschem/crossroad_schematization.py
--rw-r--r--   0 jm        (1000) jm        (1000)     5393 2023-05-12 08:32:50.000000 crossroads-schematization-0.1.1/crschem/processing.py
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-06 15:33:59.892695 crossroads-schematization-0.1.1/crschem/resources/
--rw-r--r--   0 jm        (1000) jm        (1000)     2425 2022-10-28 13:53:49.000000 crossroads-schematization-0.1.1/crschem/resources/crossing.svg
--rw-r--r--   0 jm        (1000) jm        (1000)    23130 2023-02-06 15:35:04.000000 crossroads-schematization-0.1.1/crschem/resources/rendering-areas.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    29214 2023-05-19 13:30:46.000000 crossroads-schematization-0.1.1/crschem/resources/rendering-nodes-crossings.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    22244 2023-05-19 13:29:18.000000 crossroads-schematization-0.1.1/crschem/resources/rendering-nodes-islands.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    22753 2023-05-19 13:31:32.000000 crossroads-schematization-0.1.1/crschem/resources/rendering-nodes-space.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    35238 2023-05-19 13:31:15.000000 crossroads-schematization-0.1.1/crschem/resources/rendering-nodes.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    28654 2023-02-06 15:35:25.000000 crossroads-schematization-0.1.1/crschem/resources/rendering-polylines-space.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    28635 2023-01-16 09:29:31.000000 crossroads-schematization-0.1.1/crschem/resources/rendering-polylines.qml
--rw-r--r--   0 jm        (1000) jm        (1000)     7371 2022-11-10 14:22:27.000000 crossroads-schematization-0.1.1/crschem/resources/tactile-a5.qpt
--rw-r--r--   0 jm        (1000) jm        (1000)     7843 2023-06-05 15:25:19.000000 crossroads-schematization-0.1.1/crschem/utils.py
--rw-r--r--   0 jm        (1000) jm        (1000)       36 2023-05-15 13:14:07.000000 crossroads-schematization-0.1.1/requirements.txt
--rw-r--r--   0 jm        (1000) jm        (1000)       38 2023-06-06 15:33:59.892695 crossroads-schematization-0.1.1/setup.cfg
--rw-r--r--   0 jm        (1000) jm        (1000)     1207 2022-11-30 16:14:11.000000 crossroads-schematization-0.1.1/setup.py
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-06 15:48:46.574860 crossroads-schematization-0.1.2/
+-rw-r--r--   0 jm        (1000) jm        (1000)      107 2022-11-30 16:15:16.000000 crossroads-schematization-0.1.2/MANIFEST.in
+-rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-06-06 15:48:46.574860 crossroads-schematization-0.1.2/PKG-INFO
+-rw-r--r--   0 jm        (1000) jm        (1000)     2897 2022-11-30 16:53:52.000000 crossroads-schematization-0.1.2/README.md
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-06 15:48:46.570860 crossroads-schematization-0.1.2/crossroads_schematization.egg-info/
+-rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-06-06 15:48:46.000000 crossroads-schematization-0.1.2/crossroads_schematization.egg-info/PKG-INFO
+-rw-r--r--   0 jm        (1000) jm        (1000)      794 2023-06-06 15:48:46.000000 crossroads-schematization-0.1.2/crossroads_schematization.egg-info/SOURCES.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)        1 2023-06-06 15:48:46.000000 crossroads-schematization-0.1.2/crossroads_schematization.egg-info/dependency_links.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)       98 2023-06-06 15:48:46.000000 crossroads-schematization-0.1.2/crossroads_schematization.egg-info/entry_points.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)        8 2023-06-06 15:48:46.000000 crossroads-schematization-0.1.2/crossroads_schematization.egg-info/top_level.txt
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-06 15:48:46.570860 crossroads-schematization-0.1.2/crschem/
+-rw-r--r--   0 jm        (1000) jm        (1000)       22 2023-06-06 15:48:27.000000 crossroads-schematization-0.1.2/crschem/__init__.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     6727 2023-06-06 12:30:02.000000 crossroads-schematization-0.1.2/crschem/cmd.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    51224 2023-06-06 12:40:32.000000 crossroads-schematization-0.1.2/crschem/crossroad.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    23428 2023-06-06 15:46:50.000000 crossroads-schematization-0.1.2/crschem/crossroad_schematization.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     5393 2023-05-12 08:32:50.000000 crossroads-schematization-0.1.2/crschem/processing.py
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-06 15:48:46.570860 crossroads-schematization-0.1.2/crschem/resources/
+-rw-r--r--   0 jm        (1000) jm        (1000)     2425 2022-10-28 13:53:49.000000 crossroads-schematization-0.1.2/crschem/resources/crossing.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)    23130 2023-02-06 15:35:04.000000 crossroads-schematization-0.1.2/crschem/resources/rendering-areas.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    29214 2023-05-19 13:30:46.000000 crossroads-schematization-0.1.2/crschem/resources/rendering-nodes-crossings.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    22244 2023-05-19 13:29:18.000000 crossroads-schematization-0.1.2/crschem/resources/rendering-nodes-islands.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    22753 2023-05-19 13:31:32.000000 crossroads-schematization-0.1.2/crschem/resources/rendering-nodes-space.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    35238 2023-05-19 13:31:15.000000 crossroads-schematization-0.1.2/crschem/resources/rendering-nodes.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    28654 2023-02-06 15:35:25.000000 crossroads-schematization-0.1.2/crschem/resources/rendering-polylines-space.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    28635 2023-01-16 09:29:31.000000 crossroads-schematization-0.1.2/crschem/resources/rendering-polylines.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)     7371 2022-11-10 14:22:27.000000 crossroads-schematization-0.1.2/crschem/resources/tactile-a5.qpt
+-rw-r--r--   0 jm        (1000) jm        (1000)     7843 2023-06-05 15:25:19.000000 crossroads-schematization-0.1.2/crschem/utils.py
+-rw-r--r--   0 jm        (1000) jm        (1000)       36 2023-05-15 13:14:07.000000 crossroads-schematization-0.1.2/requirements.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)       38 2023-06-06 15:48:46.574860 crossroads-schematization-0.1.2/setup.cfg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1207 2022-11-30 16:14:11.000000 crossroads-schematization-0.1.2/setup.py
```

### Comparing `crossroads-schematization-0.1.1/PKG-INFO` & `crossroads-schematization-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossroads-schematization
-Version: 0.1.1
+Version: 0.1.2
 Summary: Crossroads schematization is a python tool that produces automatic schematization of intersections from OpenStreetMap.
 Home-page: https://github.com/jmtrivial/crossroads-schematization/
 Author: Jean-Marie Favreau
 Author-email: j-marie.favreau@uca.fr
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crossroads-schematization-0.1.1/README.md` & `crossroads-schematization-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.1.1/crossroads_schematization.egg-info/PKG-INFO` & `crossroads-schematization-0.1.2/crossroads_schematization.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossroads-schematization
-Version: 0.1.1
+Version: 0.1.2
 Summary: Crossroads schematization is a python tool that produces automatic schematization of intersections from OpenStreetMap.
 Home-page: https://github.com/jmtrivial/crossroads-schematization/
 Author: Jean-Marie Favreau
 Author-email: j-marie.favreau@uca.fr
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crossroads-schematization-0.1.1/crossroads_schematization.egg-info/SOURCES.txt` & `crossroads-schematization-0.1.2/crossroads_schematization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.1.1/crschem/cmd.py` & `crossroads-schematization-0.1.2/crschem/cmd.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.1.1/crschem/crossroad.py` & `crossroads-schematization-0.1.2/crschem/crossroad.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.1.1/crschem/crossroad_schematization.py` & `crossroads-schematization-0.1.2/crschem/crossroad_schematization.py`

 * *Files 1% similar despite different names*

```diff
@@ -445,14 +445,15 @@
             exporter.exportToPdf(filename, settings)
         else:
             settings = QgsLayoutExporter.ImageExportSettings()
             if dpi > 0:
                 settings.dpi = dpi
             exporter.exportToImage(filename, settings)
         
+        project.clear()
         # trick [END]: go back to the initial directory
         os.chdir(cwd)
         
         # delete temporary file if not required
         if log_files:
             print("geojson:", tmp.name)
         else:
```

### Comparing `crossroads-schematization-0.1.1/crschem/processing.py` & `crossroads-schematization-0.1.2/crschem/processing.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.1.1/crschem/resources/crossing.svg` & `crossroads-schematization-0.1.2/crschem/resources/crossing.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.1.1/crschem/resources/rendering-areas.qml` & `crossroads-schematization-0.1.2/crschem/resources/rendering-areas.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.1.1/crschem/resources/rendering-nodes-crossings.qml` & `crossroads-schematization-0.1.2/crschem/resources/rendering-nodes-crossings.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.1.1/crschem/resources/rendering-nodes-islands.qml` & `crossroads-schematization-0.1.2/crschem/resources/rendering-nodes-islands.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.1.1/crschem/resources/rendering-nodes-space.qml` & `crossroads-schematization-0.1.2/crschem/resources/rendering-nodes-space.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.1.1/crschem/resources/rendering-nodes.qml` & `crossroads-schematization-0.1.2/crschem/resources/rendering-nodes.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.1.1/crschem/resources/rendering-polylines-space.qml` & `crossroads-schematization-0.1.2/crschem/resources/rendering-polylines-space.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.1.1/crschem/resources/rendering-polylines.qml` & `crossroads-schematization-0.1.2/crschem/resources/rendering-polylines.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.1.1/crschem/resources/tactile-a5.qpt` & `crossroads-schematization-0.1.2/crschem/resources/tactile-a5.qpt`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.1.1/crschem/utils.py` & `crossroads-schematization-0.1.2/crschem/utils.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.1.1/setup.py` & `crossroads-schematization-0.1.2/setup.py`

 * *Files identical despite different names*

