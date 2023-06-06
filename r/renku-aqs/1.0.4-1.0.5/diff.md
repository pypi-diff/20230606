# Comparing `tmp/renku-aqs-1.0.4.tar.gz` & `tmp/renku-aqs-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renku-aqs-1.0.4.tar", last modified: Wed Mar 29 07:14:31 2023, max compression
+gzip compressed data, was "renku-aqs-1.0.5.tar", last modified: Mon Jun  5 21:24:13 2023, max compression
```

## Comparing `renku-aqs-1.0.4.tar` & `renku-aqs-1.0.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2023-03-29 07:14:31.128398 renku-aqs-1.0.4/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       57 2023-02-15 12:13:10.000000 renku-aqs-1.0.4/.gitignore
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    11358 2021-11-03 09:51:02.000000 renku-aqs-1.0.4/LICENSE
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      114 2021-11-03 09:51:02.000000 renku-aqs-1.0.4/MANIFEST.in
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      966 2023-03-29 07:14:31.128398 renku-aqs-1.0.4/PKG-INFO
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     6340 2023-02-22 13:20:01.000000 renku-aqs-1.0.4/README.md
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        6 2023-03-29 07:14:28.000000 renku-aqs-1.0.4/VERSION
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      345 2021-11-03 09:51:02.000000 renku-aqs-1.0.4/concepts.md
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1659 2021-11-03 09:51:02.000000 renku-aqs-1.0.4/example.md
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2023-03-29 07:14:31.124398 renku-aqs-1.0.4/readme_imgs/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)  1891362 2023-02-15 12:13:10.000000 renku-aqs-1.0.4/readme_imgs/animation_expansion_retraction.gif
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    22497 2023-02-15 12:13:10.000000 renku-aqs-1.0.4/readme_imgs/enable_disable_configuration-graph.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)   302729 2023-02-15 12:13:10.000000 renku-aqs-1.0.4/readme_imgs/example_display_graph_complete.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)   150316 2023-02-15 12:13:10.000000 renku-aqs-1.0.4/readme_imgs/example_display_graph_final-an.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    36993 2023-02-15 12:13:10.000000 renku-aqs-1.0.4/readme_imgs/example_display_graph_final-an_no-oda-info.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)   146690 2023-02-15 12:13:10.000000 renku-aqs-1.0.4/readme_imgs/example_show-graph.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    61174 2023-02-15 12:13:10.000000 renku-aqs-1.0.4/readme_imgs/expanded_plan.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    71535 2023-02-15 12:13:10.000000 renku-aqs-1.0.4/readme_imgs/hierarchical_view.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    52046 2023-02-15 12:13:10.000000 renku-aqs-1.0.4/readme_imgs/reduced_plan.png
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    52899 2023-02-15 12:13:10.000000 renku-aqs-1.0.4/readme_imgs/subgraph.png
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2023-03-29 07:14:31.128398 renku-aqs-1.0.4/renku_aqs.egg-info/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      966 2023-03-29 07:14:30.000000 renku-aqs-1.0.4/renku_aqs.egg-info/PKG-INFO
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1070 2023-03-29 07:14:31.000000 renku-aqs-1.0.4/renku_aqs.egg-info/SOURCES.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        1 2023-03-29 07:14:30.000000 renku-aqs-1.0.4/renku_aqs.egg-info/dependency_links.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      172 2023-03-29 07:14:30.000000 renku-aqs-1.0.4/renku_aqs.egg-info/entry_points.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        1 2022-09-19 09:18:07.000000 renku-aqs-1.0.4/renku_aqs.egg-info/not-zip-safe
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      100 2023-03-29 07:14:30.000000 renku-aqs-1.0.4/renku_aqs.egg-info/requires.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        9 2023-03-29 07:14:30.000000 renku-aqs-1.0.4/renku_aqs.egg-info/top_level.txt
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2023-03-29 07:14:31.128398 renku-aqs-1.0.4/renkuaqs/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     5761 2023-02-22 13:20:01.000000 renku-aqs-1.0.4/renkuaqs/__init__.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      627 2022-09-13 14:05:06.000000 renku-aqs-1.0.4/renkuaqs/config.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     2092 2023-02-15 12:13:10.000000 renku-aqs-1.0.4/renkuaqs/graph_config.yaml
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     5206 2023-03-07 17:13:35.000000 renku-aqs-1.0.4/renkuaqs/graph_graphical_config.json
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     6705 2023-03-07 17:13:35.000000 renku-aqs-1.0.4/renkuaqs/graph_nodes_subset_config.json
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      421 2023-02-15 12:13:10.000000 renku-aqs-1.0.4/renkuaqs/graph_reduction_config.json
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    44128 2023-02-22 13:20:01.000000 renku-aqs-1.0.4/renkuaqs/graph_utils.py
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2023-03-29 07:14:31.128398 renku-aqs-1.0.4/renkuaqs/icons/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     3416 2023-02-15 12:13:10.000000 renku-aqs-1.0.4/renkuaqs/icons/graph_icon.svg
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    11874 2023-03-29 07:08:20.000000 renku-aqs-1.0.4/renkuaqs/javascript_graph_utils.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    12562 2023-02-15 12:13:10.000000 renku-aqs-1.0.4/renkuaqs/oda_ontology.ttl
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    16091 2023-02-22 13:20:01.000000 renku-aqs-1.0.4/renkuaqs/plugin.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        0 2023-02-15 12:13:10.000000 renku-aqs-1.0.4/requirements.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       38 2023-03-29 07:14:31.128398 renku-aqs-1.0.4/setup.cfg
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     2558 2023-03-29 07:14:06.000000 renku-aqs-1.0.4/setup.py
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2023-03-29 07:14:31.128398 renku-aqs-1.0.4/tests/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     3093 2023-02-15 12:13:10.000000 renku-aqs-1.0.4/tests/test_example.py
+drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-06-05 21:24:13.847607 renku-aqs-1.0.5/
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      187 2023-06-05 17:42:34.000000 renku-aqs-1.0.5/.gitignore
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    11358 2021-06-14 15:54:58.000000 renku-aqs-1.0.5/LICENSE
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      114 2021-06-14 15:54:58.000000 renku-aqs-1.0.5/MANIFEST.in
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      937 2023-06-05 21:24:13.847607 renku-aqs-1.0.5/PKG-INFO
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     6340 2023-02-22 13:05:10.000000 renku-aqs-1.0.5/README.md
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)        5 2023-06-05 17:42:57.000000 renku-aqs-1.0.5/VERSION
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      345 2021-06-14 15:54:58.000000 renku-aqs-1.0.5/concepts.md
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     1659 2021-06-28 10:31:11.000000 renku-aqs-1.0.5/example.md
+drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-06-05 21:24:13.843607 renku-aqs-1.0.5/readme_imgs/
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)  1891362 2023-01-23 09:07:17.000000 renku-aqs-1.0.5/readme_imgs/animation_expansion_retraction.gif
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    22497 2023-01-23 09:07:17.000000 renku-aqs-1.0.5/readme_imgs/enable_disable_configuration-graph.png
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)   302729 2023-01-23 09:07:17.000000 renku-aqs-1.0.5/readme_imgs/example_display_graph_complete.png
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)   150316 2023-01-23 09:07:17.000000 renku-aqs-1.0.5/readme_imgs/example_display_graph_final-an.png
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    36993 2023-01-23 09:07:17.000000 renku-aqs-1.0.5/readme_imgs/example_display_graph_final-an_no-oda-info.png
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)   146690 2023-01-23 09:07:17.000000 renku-aqs-1.0.5/readme_imgs/example_show-graph.png
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    61174 2023-01-23 09:07:17.000000 renku-aqs-1.0.5/readme_imgs/expanded_plan.png
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    71535 2023-01-23 09:07:17.000000 renku-aqs-1.0.5/readme_imgs/hierarchical_view.png
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    52046 2023-01-23 09:07:17.000000 renku-aqs-1.0.5/readme_imgs/reduced_plan.png
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    52899 2023-01-23 09:07:17.000000 renku-aqs-1.0.5/readme_imgs/subgraph.png
+drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-06-05 21:24:13.843607 renku-aqs-1.0.5/renku_aqs.egg-info/
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      937 2023-06-05 21:24:13.000000 renku-aqs-1.0.5/renku_aqs.egg-info/PKG-INFO
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     1066 2023-06-05 21:24:13.000000 renku-aqs-1.0.5/renku_aqs.egg-info/SOURCES.txt
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)        1 2023-06-05 21:24:13.000000 renku-aqs-1.0.5/renku_aqs.egg-info/dependency_links.txt
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      171 2023-06-05 21:24:13.000000 renku-aqs-1.0.5/renku_aqs.egg-info/entry_points.txt
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)        1 2021-12-08 07:18:18.000000 renku-aqs-1.0.5/renku_aqs.egg-info/not-zip-safe
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      120 2023-06-05 21:24:13.000000 renku-aqs-1.0.5/renku_aqs.egg-info/requires.txt
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)        9 2023-06-05 21:24:13.000000 renku-aqs-1.0.5/renku_aqs.egg-info/top_level.txt
+drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-06-05 21:24:13.847607 renku-aqs-1.0.5/renkuaqs/
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     5975 2023-06-05 17:42:34.000000 renku-aqs-1.0.5/renkuaqs/__init__.py
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      606 2023-06-05 17:42:34.000000 renku-aqs-1.0.5/renkuaqs/config.py
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     2092 2023-01-23 09:07:17.000000 renku-aqs-1.0.5/renkuaqs/graph_config.yaml
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     7384 2023-06-05 17:42:34.000000 renku-aqs-1.0.5/renkuaqs/graph_graphical_config.json
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     8836 2023-06-05 17:42:34.000000 renku-aqs-1.0.5/renkuaqs/graph_nodes_subset_config.json
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      421 2023-02-10 17:08:04.000000 renku-aqs-1.0.5/renkuaqs/graph_reduction_config.json
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    50791 2023-06-05 17:42:34.000000 renku-aqs-1.0.5/renkuaqs/graph_utils.py
+drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-06-05 21:24:13.847607 renku-aqs-1.0.5/renkuaqs/icons/
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     3416 2023-01-23 09:07:17.000000 renku-aqs-1.0.5/renkuaqs/icons/graph_icon.svg
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    11874 2023-03-14 09:55:25.000000 renku-aqs-1.0.5/renkuaqs/javascript_graph_utils.py
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    42892 2023-05-26 14:38:27.000000 renku-aqs-1.0.5/renkuaqs/ontology.ttl
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    18708 2023-06-05 17:42:34.000000 renku-aqs-1.0.5/renkuaqs/plugin.py
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)        0 2023-01-23 09:07:17.000000 renku-aqs-1.0.5/requirements.txt
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)       38 2023-06-05 21:24:13.847607 renku-aqs-1.0.5/setup.cfg
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     2399 2023-06-05 21:24:05.000000 renku-aqs-1.0.5/setup.py
+drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-06-05 21:24:13.847607 renku-aqs-1.0.5/tests/
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     3093 2023-02-08 14:37:58.000000 renku-aqs-1.0.5/tests/test_example.py
```

### Comparing `renku-aqs-1.0.4/LICENSE` & `renku-aqs-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.4/PKG-INFO` & `renku-aqs-1.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: renku-aqs
-Version: 1.0.4
+Version: 1.0.5
 Summary: Renku AQS plugin
-Home-page: UNKNOWN
 Author: Gabriele Barni, Volodymyr Savchenko
 Author-email: 
 License: Apache License 2.0
 Keywords: Renku AQS
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -19,10 +18,7 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 4 - Beta
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `renku-aqs-1.0.4/README.md` & `renku-aqs-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.4/example.md` & `renku-aqs-1.0.5/example.md`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.4/readme_imgs/animation_expansion_retraction.gif` & `renku-aqs-1.0.5/readme_imgs/animation_expansion_retraction.gif`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.4/readme_imgs/enable_disable_configuration-graph.png` & `renku-aqs-1.0.5/readme_imgs/enable_disable_configuration-graph.png`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.4/readme_imgs/example_display_graph_complete.png` & `renku-aqs-1.0.5/readme_imgs/example_display_graph_complete.png`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.4/readme_imgs/example_display_graph_final-an.png` & `renku-aqs-1.0.5/readme_imgs/example_display_graph_final-an.png`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.4/readme_imgs/example_display_graph_final-an_no-oda-info.png` & `renku-aqs-1.0.5/readme_imgs/example_display_graph_final-an_no-oda-info.png`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.4/readme_imgs/example_show-graph.png` & `renku-aqs-1.0.5/readme_imgs/example_show-graph.png`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.4/readme_imgs/expanded_plan.png` & `renku-aqs-1.0.5/readme_imgs/expanded_plan.png`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.4/readme_imgs/hierarchical_view.png` & `renku-aqs-1.0.5/readme_imgs/hierarchical_view.png`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.4/readme_imgs/reduced_plan.png` & `renku-aqs-1.0.5/readme_imgs/reduced_plan.png`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.4/readme_imgs/subgraph.png` & `renku-aqs-1.0.5/readme_imgs/subgraph.png`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.4/renku_aqs.egg-info/PKG-INFO` & `renku-aqs-1.0.5/renku_aqs.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: renku-aqs
-Version: 1.0.4
+Version: 1.0.5
 Summary: Renku AQS plugin
-Home-page: UNKNOWN
 Author: Gabriele Barni, Volodymyr Savchenko
 Author-email: 
 License: Apache License 2.0
 Keywords: Renku AQS
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -19,10 +18,7 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 4 - Beta
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `renku-aqs-1.0.4/renku_aqs.egg-info/SOURCES.txt` & `renku-aqs-1.0.5/renku_aqs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -28,11 +28,11 @@
 renkuaqs/config.py
 renkuaqs/graph_config.yaml
 renkuaqs/graph_graphical_config.json
 renkuaqs/graph_nodes_subset_config.json
 renkuaqs/graph_reduction_config.json
 renkuaqs/graph_utils.py
 renkuaqs/javascript_graph_utils.py
-renkuaqs/oda_ontology.ttl
+renkuaqs/ontology.ttl
 renkuaqs/plugin.py
 renkuaqs/icons/graph_icon.svg
 tests/test_example.py
```

### Comparing `renku-aqs-1.0.4/renkuaqs/__init__.py` & `renku-aqs-1.0.5/renkuaqs/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,18 +56,20 @@
         self.logger = logging.getLogger(self.__class__.__name__)
 
 
     def do_GET(self) -> None:
         mount_path_env = os.environ.get('MOUNT_PATH', None)
         logging.info(f'self.path = {self.path}, os.cwd = {os.getcwd()}, mount_path = {mount_path_env}')
         if self.path == '/':
+
             try:
                 self.send_response(200)
                 self.send_header("Content-type", "text/html")
                 self.end_headers()
+                graph_utils.inspect_oda_graph_inputs(None, paths=os.getcwd())
                 graph_html_content, ttl_content = graph_utils.build_graph_html(None, paths=os.getcwd(),
                                                                                template_location="remote",
                                                                                include_ttl_content_within_html=False)
                 self.wfile.write(graph_html_content.encode())
             except Exception as e:
                 output_html = f'''
                 <html><head></head><body><h1>Error while generating the output graph:</h1>
@@ -145,15 +147,16 @@
     if 'MOUNT_PATH' in os.environ:
         mount_dir = os.path.join(mount_dir, os.environ['MOUNT_PATH'][1:])
 
     return {
         'command': [
             'bash',
             '-c',
-            f'python -c \'import renkuaqs; renkuaqs._start_graph_http_server("{mount_dir}", "{{port}}")\''
+            f'python -c \'import renkuaqs; import os; from renku.domain_model.project_context import project_context; '
+                f'project_context.push_path(os.getcwd()); renkuaqs._start_graph_http_server("{mount_dir}", "{{port}}")\''
         ],
         'new_browser_tab': False,
         'launcher_entry': {
                 'enabled': True,
                 'icon_path': os.path.join(os.path.dirname(os.path.abspath(__file__)), "icons", "graph_icon.svg"),
                 'title': 'Graph'
             }
```

### Comparing `renku-aqs-1.0.4/renkuaqs/config.py` & `renku-aqs-1.0.5/renkuaqs/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-AQS_DIR = 'aqs'
-AQS_METADATA_FILE = 'metadata.jsonld'
+ENTITY_METADATA_AQS_DIR = '.aqs'
```

### Comparing `renku-aqs-1.0.4/renkuaqs/graph_config.yaml` & `renku-aqs-1.0.5/renkuaqs/graph_config.yaml`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.4/renkuaqs/graph_graphical_config.json` & `renku-aqs-1.0.5/renkuaqs/graph_graphical_config.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.933752204585538%*

 * *Differences: {"'Nodes'": "{'Activity': {delete: ['displayed_literals_format']}, 'AstrophysicalObject': "*

 * *            "{'color': '#d0d0e8', 'displayed_literals_format': "*

 * *            "'AstroObject:no,arg_name:yes,parameter_name:no,value:yes'}, 'StartTime,EndTime': "*

 * *            "OrderedDict([('shape', 'box'), ('color', '#bcddc9'), ('style', 'filled'), ('value', "*

 * *            "35), ('level', 1), ('displayed_information', 'literals'), "*

 * *            "('displayed_literals_format', 'parameter_name:no,value:yes')]), "*

 * *         […]*

```diff
@@ -9,15 +9,14 @@
             "level": 4,
             "shape": "box",
             "style": "filled",
             "value": 35
         },
         "Activity": {
             "color": "#00FC10",
-            "displayed_literals_format": "command:no",
             "level": 0,
             "shape": "box",
             "style": "filled",
             "value": 35
         },
         "Angle": {
             "color": "#1B81FB",
@@ -33,17 +32,17 @@
             "displayed_information": "title",
             "level": 1,
             "shape": "box",
             "style": "filled",
             "value": 35
         },
         "AstrophysicalObject": {
-            "color": "#6262be",
+            "color": "#d0d0e8",
             "displayed_information": "literals",
-            "displayed_literals_format": "AstroObject:no",
+            "displayed_literals_format": "AstroObject:no,arg_name:yes,parameter_name:no,value:yes",
             "level": 1,
             "shape": "box",
             "style": "filled",
             "value": 35
         },
         "AstrophysicalRegion": {
             "color": "#6262bf",
@@ -59,14 +58,32 @@
             "displayed_information": "literals",
             "displayed_literals_format": "AQModule:no",
             "level": 0,
             "shape": "box",
             "style": "filled",
             "value": 35
         },
+        "Class": {
+            "color": "#ffffff",
+            "displayed_information": "literals",
+            "displayed_literals_format": "label:no",
+            "displayed_type_name": "<i>OntologyClass</i>",
+            "font": {
+                "boldital": {
+                    "size": 21
+                },
+                "face": "courier",
+                "multi": "html",
+                "size": 38
+            },
+            "level": 0,
+            "shape": "box",
+            "style": "filled",
+            "value": 35
+        },
         "CommandInput": {
             "color": "#DBA3BC",
             "displayed_information": "literals",
             "displayed_literals_format": "defaultValue:no",
             "displayed_type_name": "Input",
             "level": 3,
             "shape": "box",
@@ -140,23 +157,50 @@
             "displayed_literals_format": "atLocation:no",
             "displayed_type_name": "Input",
             "level": 3,
             "shape": "box",
             "style": "filled",
             "value": 20
         },
+        "LightCurve": {
+            "color": "#91acca",
+            "displayed_information": "literals",
+            "displayed_literals_format": "output_name:no,parameter_name:no,value:yes",
+            "level": 1,
+            "shape": "box",
+            "style": "filled",
+            "value": 35
+        },
+        "ODAPictureProduct": {
+            "color": "#91acca",
+            "displayed_information": "literals",
+            "displayed_literals_format": "output_name:no,parameter_name:no,value:yes",
+            "level": 1,
+            "shape": "box",
+            "style": "filled",
+            "value": 35
+        },
         "Pixels": {
             "color": "#1B81FB",
             "displayed_information": "both",
             "displayed_literals_format": "title:no",
             "level": 2,
             "shape": "box",
             "style": "filled",
             "value": 35
         },
+        "PointOfInterestRA,PointOfInterestDEC": {
+            "color": "#91acc1",
+            "displayed_information": "literals",
+            "displayed_literals_format": "parameter_name:no,value:yes",
+            "level": 1,
+            "shape": "box",
+            "style": "filled",
+            "value": 35
+        },
         "Position": {
             "color": "#1B81FB",
             "displayed_information": "both",
             "displayed_literals_format": "title:no",
             "level": 2,
             "shape": "box",
             "style": "filled",
@@ -181,10 +225,37 @@
             "color": "#1B81FB",
             "displayed_information": "both",
             "displayed_literals_format": "title:no",
             "level": 2,
             "shape": "box",
             "style": "filled",
             "value": 35
+        },
+        "StartTime,EndTime": {
+            "color": "#bcddc9",
+            "displayed_information": "literals",
+            "displayed_literals_format": "parameter_name:no,value:yes",
+            "level": 1,
+            "shape": "box",
+            "style": "filled",
+            "value": 35
+        },
+        "int,integer,Integer": {
+            "color": "#91acbf",
+            "displayed_information": "literals",
+            "displayed_literals_format": "parameter_name:no,value:yes",
+            "level": 1,
+            "shape": "box",
+            "style": "filled",
+            "value": 35
+        },
+        "str,String,string": {
+            "color": "#91acdf",
+            "displayed_information": "literals",
+            "displayed_literals_format": "parameter_name:no,value:yes",
+            "level": 1,
+            "shape": "box",
+            "style": "filled",
+            "value": 35
         }
     }
 }
```

### Comparing `renku-aqs-1.0.4/renkuaqs/graph_utils.py` & `renku-aqs-1.0.5/renkuaqs/graph_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,79 @@
 import os
 import io
 import typing
 import pydotplus
 import rdflib
 import yaml
 import json
+import hashlib
+import glob
+import urllib.request
 
+from prettytable import PrettyTable
 from rdflib.tools.rdf2dot import LABEL_PROPERTIES
 from rdflib.tools import rdf2dot
 from lxml import etree
 from dateutil import parser
 from astropy.coordinates import SkyCoord, Angle
 from IPython.display import display
 from pyvis.network import Network
 from importlib import resources
+from nb2workflow import ontology
+from pathlib import Path
 
 from renku.domain_model.project_context import project_context
 from renku.command.graph import export_graph_command
 from renku.core.errors import RenkuException
+from renku.core.util.git import get_entity_from_revision
 
 import renkuaqs.javascript_graph_utils as javascript_graph_utils
 
+from renkuaqs.config import ENTITY_METADATA_AQS_DIR
+from renkuaqs.plugin import AQS
+
 # TODO improve this
 __this_dir__ = os.path.join(os.path.abspath(os.path.dirname(__file__)))
+
+
 graph_configuration = yaml.load(open(os.path.join(__this_dir__, "graph_config.yaml")), Loader=yaml.SafeLoader)
 
 
-def _graph(revision=None, paths=None):
+def _aqs_graph(revision=None, paths=None):
+    G = rdflib.Graph()
+    if os.path.exists(ENTITY_METADATA_AQS_DIR):
+        annotation_list = []
+        entity_folder_list = glob.glob(f"{ENTITY_METADATA_AQS_DIR}/*")
+        for entity_folder in entity_folder_list:
+            print("Scanning entity folder: ", entity_folder)
+            revision_entity_folder_list = glob.glob(f"{entity_folder}/*")
+            for revision_entity_folder in revision_entity_folder_list:
+                print("Scanning entity folder checksum: ", revision_entity_folder)
+                annotation_object_list = glob.glob(f"{revision_entity_folder}/*.jsonld")
+                for annotation_object_file in annotation_object_list:
+                    with open(annotation_object_file) as annotation_object_file_fn:
+                        annotation_object = json.load(annotation_object_file_fn)
+                    annotation_list.append(annotation_object)
+                    G.parse(data=json.dumps(annotation_object), format="json-ld")
+
+    return G
+
+
+def _renku_graph(revision=None, paths=None):
     # FIXME: use (revision) filter
 
     cmd_result = export_graph_command().working_directory(paths).build().execute()
 
     if cmd_result.status == cmd_result.FAILURE:
         raise RenkuException("fail to export the renku graph")
     graph = cmd_result.output.as_rdflib_graph()
 
-    graph.bind("aqs", "http://www.w3.org/ns/aqs#")
-    graph.bind("oa", "http://www.w3.org/ns/oa#")
-    graph.bind("xsd", "http://www.w3.org/2001/XAQSchema#")
-    graph.bind("oda", "http://odahub.io/ontology#")
-    graph.bind("odas", "https://odahub.io/ontology#")
-    graph.bind("local-renku", f"file://{paths}/")
-
     return graph
 
+
 def write_graph_files(graph_html_content, ttl_content):
     html_fn = 'graph.html'
     ttl_fn = 'full_graph.ttl'
 
     with open(ttl_fn, 'w') as gfn:
         gfn.write(ttl_content)
 
@@ -59,37 +85,68 @@
     return html_fn, ttl_fn
 
 
 def extract_graph(revision, paths):
     if paths is None:
         paths = project_context.path
 
-    graph = _graph(revision, paths)
+    renku_graph = _renku_graph(revision, paths)
+
+    aqs_graph = _aqs_graph(revision, paths)
 
-    graph_str = graph.serialize(format="n3")
+    ontologies_graph = _nodes_subset_ontologies_graph()
+
+    # not the recommended approach but works in our case https://rdflib.readthedocs.io/en/stable/merging.html
+    overall_graph = aqs_graph + renku_graph + ontologies_graph
+
+    overall_graph.bind("aqs", "http://www.w3.org/ns/aqs#")
+    overall_graph.bind("oa", "http://www.w3.org/ns/oa#")
+    overall_graph.bind("xsd", "http://www.w3.org/2001/XAQSchema#")
+    overall_graph.bind("oda", "http://odahub.io/ontology#")
+    overall_graph.bind("odas", "https://odahub.io/ontology#")
+    overall_graph.bind("local-renku", f"file://{paths}/")
+
+    graph_str = overall_graph.serialize(format="n3")
 
     return graph_str
 
+
+def _nodes_subset_ontologies_graph():
+    G = rdflib.Graph()
+    graph_nodes_subset_config_fn = 'graph_nodes_subset_config.json'
+    with resources.open_text("renkuaqs", graph_nodes_subset_config_fn) as graph_nodes_subset_config_fn_f:
+        graph_nodes_subset_config_obj = json.load(graph_nodes_subset_config_fn_f)
+
+    for subset_obj_name, subset_obj_dict in graph_nodes_subset_config_obj.items():
+        if 'ontology_url' in subset_obj_dict:
+            data = urllib.request.urlopen(subset_obj_dict['ontology_url'])
+            G.parse(data)
+        elif 'ontology_path' in subset_obj_dict:
+            if os.path.exists(subset_obj_dict['ontology_path']):
+                with open(subset_obj_dict['ontology_path']) as oo_fn:
+                    G.parse(oo_fn)
+            else:
+                print(f"\033[31m{subset_obj_dict['ontology_path']} not found\033[0m")
+
+    return G
+
+
 def build_graph_html(revision, paths,
                      include_title=True,
                      template_location="local",
                      include_ttl_content_within_html=True):
 
     default_graph_graphical_config_fn = 'graph_graphical_config.json'
     graph_nodes_subset_config_fn = 'graph_nodes_subset_config.json'
     graph_reduction_config_fn = 'graph_reduction_config.json'
 
     graph_str = extract_graph(revision, paths)
 
     full_graph_ttl_str = graph_str.replace("\\\"", '\\\\"')
 
-    # # TODO to be tested
-    # with resources.path("renkuaqs", 'oda_ontology.ttl') as ttl_ontology_fn:
-    #     graph = graph.parse(source=ttl_ontology_fn)
-
     nodes_graph_config_obj = {}
     edges_graph_config_obj = {}
 
     graph_config_names_list = []
     with resources.open_text("renkuaqs", default_graph_graphical_config_fn) as graph_config_fn_f:
         graph_config_loaded = json.load(graph_config_fn_f)
         nodes_graph_config_obj_loaded = graph_config_loaded.get('Nodes', {})
@@ -101,28 +158,33 @@
         nodes_graph_config_obj.update(nodes_graph_config_obj_loaded)
     if edges_graph_config_obj_loaded:
         for config_type in edges_graph_config_obj_loaded:
             edges_graph_config_obj_loaded[config_type]['config_file'] = default_graph_graphical_config_fn
         edges_graph_config_obj.update(edges_graph_config_obj_loaded)
     graph_config_names_list.append(default_graph_graphical_config_fn)
     # for compatibility with Javascript
-    nodes_graph_config_obj_str = json.dumps(nodes_graph_config_obj)
-    edges_graph_config_obj_str = json.dumps(edges_graph_config_obj)
+    nodes_graph_config_obj_str = json.dumps(nodes_graph_config_obj).replace("\\\"", '\\\\"')
+    edges_graph_config_obj_str = json.dumps(edges_graph_config_obj).replace("\\\"", '\\\\"')
 
     with resources.open_text("renkuaqs", graph_reduction_config_fn) as graph_reduction_config_fn_f:
         graph_reduction_config_obj = json.load(graph_reduction_config_fn_f)
 
     # for compatibility with Javascript
     graph_reductions_obj_str = json.dumps(graph_reduction_config_obj)
 
     with resources.open_text("renkuaqs", graph_nodes_subset_config_fn) as graph_nodes_subset_config_fn_f:
         graph_nodes_subset_config_obj = json.load(graph_nodes_subset_config_fn_f)
 
     # for compatibility with Javascript
-    graph_nodes_subset_config_obj_str = json.dumps(graph_nodes_subset_config_obj).replace("\\\"", '\\\\"').replace("\\n", '\\\\n')
+    # FIXME there must be a better way
+    graph_nodes_subset_config_obj_str = json.dumps(graph_nodes_subset_config_obj)\
+        .replace("\\\"", '\\\\"') \
+        .replace("\\\\s", '\\\\\\\\\\\\s') \
+        .replace("\\n", '\\\\n') \
+        .replace("\\t", '\\\\t')
 
     net = Network(
         height='750px', width='100%',
         cdn_resources=template_location
     )
     net.generate_html()
 
@@ -144,21 +206,111 @@
                                             graph_nodes_subset_config_obj_dict=graph_nodes_subset_config_obj,
                                             include_title=include_title)
 
     # return net, html_fn
     return net.html, graph_str
 
 
+def inspect_oda_graph_inputs(revision, paths, input_notebook: str = None):
+    if paths is None:
+        paths = project_context.path
+
+    graph = _renku_graph(revision, paths)
+
+    query_select = "SELECT DISTINCT ?entityInput ?entityInputLocation ?entityInputChecksum"
+
+    query_where = """WHERE {
+                    ?entityInput a <http://www.w3.org/ns/prov#Entity> ;
+                        <http://www.w3.org/ns/prov#atLocation> ?entityInputLocation ;
+                        <https://swissdatasciencecenter.github.io/renku-ontology#checksum> ?entityInputChecksum .
+            """
+
+    if input_notebook is not None:
+        query_where += f"""
+        
+                FILTER ( ?entityInputLocation = '{input_notebook}' ) .
+        """
+
+    query_where += """
+            ?activity a ?activityType ;
+                <http://www.w3.org/ns/prov#qualifiedUsage>/<http://www.w3.org/ns/prov#entity> ?entityInput .        
+    }
+    """
+
+    query = f"""{query_select}
+               {query_where}
+            """
+
+    r = graph.query(query)
+
+    G = rdflib.Graph()
+
+    output = PrettyTable()
+    output.field_names = ["Entity ID", "Entity checksum", "Entity input location"]
+    output.align["Entity ID"] = "l"
+    output.align["Entity checksum"] = "l"
+    output.align["Entity input location"] = "l"
+    for row in r:
+        entity_path = row.entityInputLocation
+        entity_checksum = row.entityInputChecksum
+        entity_id = row.entityInput
+        output.add_row([
+            entity_id,
+            entity_checksum,
+            entity_path
+        ])
+        entity_file_name, entity_file_extension = os.path.splitext(entity_path)
+        if entity_file_extension == '.ipynb':
+            print(f"\033[31mExtracting metadata from the input notebook: {entity_path}, id: {entity_id}\033[0m")
+            # get checksum from the path
+            repository = project_context.repository
+            revision = repository.head.commit.hexsha
+            entity_obj = get_entity_from_revision(repository=repository, path=entity_path, revision=revision, bypass_cache=True)
+            print(f"\033[31mEntity object extracted from entity_path: {entity_obj.path}, checksum: {entity_obj.checksum}\033[0m")
+            print(f"\033[31mEntity checksum from the graph: {entity_checksum}\033[0m")
+            if str(entity_obj.checksum) == str(entity_checksum):
+                # file present on disk based on the checksum equality
+                rdf_nb = ontology.nb2rdf(entity_path)
+                aqs_obj = AQS(entity_path)
+                G.parse(data=rdf_nb)
+                rdf_jsonld_str = G.serialize(format="json-ld")
+                rdf_jsonld = json.loads(rdf_jsonld_str)
+
+                print(f"\033[32mlog_aqs_annotation\033[0m")
+
+                annotation_folder_path = Path(
+                    os.path.join(aqs_obj.aqs_annotation_path, entity_file_name, entity_checksum))
+                if annotation_folder_path.exists():
+                    # directory gets cleaned-up in order to avoid to generate duplicate jsonld files
+                    # that can occur in case of new commits where input notebook is not affected
+                    jsonld_files = glob.glob(str(annotation_folder_path.joinpath("*.jsonld")))
+                    for j_f in jsonld_files:
+                        os.remove(j_f)
+                else:
+                    annotation_folder_path.mkdir(parents=True)
+
+                for nb2annotation in rdf_jsonld:
+                    nb2annotation["http://odahub.io/ontology#entity_checksum"] = entity_checksum
+                    print(f"found jsonLD annotation:\n", json.dumps(nb2annotation, sort_keys=True, indent=4))
+                    nb2annotation_id_hash = hashlib.sha256(nb2annotation["@id"].encode()).hexdigest()[:8]
+
+                    jsonld_path = os.path.join(annotation_folder_path, nb2annotation_id_hash + ".jsonld")
+                    with open(jsonld_path, mode="w") as f:
+                        print("writing", jsonld_path)
+                        f.write(json.dumps(nb2annotation, sort_keys=True, indent=4))
+
+    print(output, "\n")
+
+
 def build_graph_image(revision, paths, filename, no_oda_info, input_notebook):
-    """Simple graph visualization """
 
     if paths is None:
         paths = project_context.path
 
-    graph = _graph(revision, paths)
+    graph = _renku_graph(revision, paths)
     renku_path = paths
 
     query_where = build_query_where(input_notebook=input_notebook, no_oda_info=no_oda_info)
     query_construct = build_query_construct(no_oda_info=no_oda_info)
 
     query = f"""{query_construct}
                {query_where}
```

### Comparing `renku-aqs-1.0.4/renkuaqs/icons/graph_icon.svg` & `renku-aqs-1.0.5/renkuaqs/icons/graph_icon.svg`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.4/renkuaqs/javascript_graph_utils.py` & `renku-aqs-1.0.5/renkuaqs/javascript_graph_utils.py`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.4/renkuaqs/plugin.py` & `renku-aqs-1.0.5/renkuaqs/plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,59 +29,104 @@
 from pathlib import Path
 from renku.domain_model.provenance.annotation import Annotation
 from renku.domain_model.project_context import project_context
 from renku.core.plugin import hookimpl
 from IPython.display import Image, HTML
 from prettytable import PrettyTable
 from aqsconverters.io import AQS_DIR, COMMON_DIR
+from renkuaqs.config import ENTITY_METADATA_AQS_DIR
+from nb2workflow import ontology
 
 import renkuaqs.graph_utils as graph_utils
 
 
 class AQS(object):
     def __init__(self, run):
         self.run = run
 
     @property
     def renku_aqs_path(self):
         """Return a ``Path`` instance of Renku AQS metadata folder."""
         return Path(project_context.metadata_path).joinpath(AQS_DIR).joinpath(COMMON_DIR)
 
+    @property
+    def aqs_annotation_path(self):
+        """Return a ``Path`` instance of Renku AQS specific annotation."""
+        return Path(ENTITY_METADATA_AQS_DIR)
+
     def load_model(self, path):
         """Load AQS reference file."""
         if path and path.exists():
             return json.load(path.open())
         return {}
 
 
 @hookimpl
+def plan_annotations(plan):
+    print(f"plan_annotations, plan \033[31m{plan.name}\033[0m")
+
+    annotations = []
+
+    return annotations
+
+
+@hookimpl
 def activity_annotations(activity):
     """``process_run_annotations`` hook implementation."""
     aqs = AQS(activity)
 
     sitecustomize_path = pathlib.Path(os.path.join(project_context.metadata_path, AQS_DIR, "sitecustomize.py"))
     if sitecustomize_path.exists():
         sitecustomize_path.unlink()
 
     annotations = []
 
     print("process_run_annotations")
     print(aqs.renku_aqs_path)
+    # apply nb2rdf also to input nb and also add the name of the notebook
+    # should be related to the input/output notebook
+    # add the annotations to the plan
+
+    if activity.generations is not None and len(activity.generations) >= 1:
+        for generation in activity.generations:
+            entity = generation.entity
+            if isinstance(entity, list):
+                entity = generation.entity[0]
+            entity_file_name, entity_file_extension = os.path.splitext(entity.path)
+            if entity_file_extension == '.ipynb':
+                print(f"\033[31mExtracting metadata from the output notebook: {entity.path}, id: {entity.id}\033[0m")
+                rdf_nb = ontology.nb2rdf(entity.path)
+                print(f"\033[32m{rdf_nb}\033[0m")
+                G = rdflib.Graph()
+                G.parse(data=rdf_nb)
+                rdf_jsonld_str = G.serialize(format="json-ld")
+                rdf_jsonld = json.loads(rdf_jsonld_str)
+                for nb2annotation in rdf_jsonld:
+                    # to comply with the terminology
+                    nb2annotation["http://odahub.io/ontology#entity_checksum"] = entity.checksum
+                    print(f"found jsonLD annotation:\n", json.dumps(nb2annotation, sort_keys=True, indent=4))
+                    model_id = nb2annotation["@id"]
+                    annotation_id = "{activity}/annotations/aqs/{id}".format(
+                        activity=activity.id, id=model_id
+                    )
+                    annotations.append(
+                        Annotation(id=annotation_id, source="AQS plugin", body=nb2annotation)
+                    )
 
     if os.path.exists(aqs.renku_aqs_path):
         for p in aqs.renku_aqs_path.iterdir():
             if p.match("*json"):
                 print(f"found json annotation: {p}")
                 print(open(p).read())
 
             elif p.match("*jsonld"):
-                print(f"found jsonLD annotation: {p}\n", json.dumps(json.load(p.open()), sort_keys=True, indent=4))
+                aqs_annotation = aqs.load_model(p)
+                print(f"found jsonLD annotation: {p}\n", json.dumps(aqs_annotation, sort_keys=True, indent=4))
 
                 # this will make annotations according to https://odahub.io/ontology/
-                aqs_annotation = aqs.load_model(p)
                 model_id = aqs_annotation["@id"]
                 annotation_id = "{activity}/annotations/aqs/{id}".format(
                     activity=activity.id, id=model_id
                 )
                 p.unlink()
                 annotations.append(
                     Annotation(id=annotation_id, source="AQS plugin", body=aqs_annotation)
@@ -389,21 +434,41 @@
 
 @aqs.command()
 @click.option(
     "--revision",
     default="HEAD",
     help="The git revision to generate the log for, default: HEAD",
 )
+@click.option("--input-notebook", default=None, help="Input notebook to process")
+@click.argument("paths", type=click.Path(exists=False), nargs=-1)
+def inspect(revision, paths, input_notebook):
+    """Inspect the input entities within the graph"""
+
+    path = paths
+    if paths is not None and isinstance(paths, click.Path):
+        path = str(path)
+
+    graph_utils.inspect_oda_graph_inputs(revision, path, input_notebook)
+
+    return ""
+
+
+@aqs.command()
+@click.option(
+    "--revision",
+    default="HEAD",
+    help="The git revision to generate the log for, default: HEAD",
+)
 @click.option("--filename", default="graph.png", help="The filename of the output file image")
 @click.option("--input-notebook", default=None, help="Input notebook to process")
 @click.option("--no-oda-info", is_flag=True, help="Exclude oda related information in the output graph")
 @click.argument("paths", type=click.Path(exists=False), nargs=-1)
 def display(revision, paths, filename, no_oda_info, input_notebook):
     path = paths
-    if paths is not  None and isinstance(paths, click.Path):
+    if paths is not None and isinstance(paths, click.Path):
         path = str(path)
     output_filename = graph_utils.build_graph_image(revision, path, filename, no_oda_info, input_notebook)
     return output_filename
 
 
 @aqs.command()
 def start_session():
```

### Comparing `renku-aqs-1.0.4/setup.py` & `renku-aqs-1.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,18 +20,17 @@
 
 install_requires = [
     'deepdiff',
     'pydotplus',
     'rdflib',
     'bs4',
     'renku==2.2.0',
-    #'astroquery @ git+https://github.com/oda-hub/astroquery#egg=astroquery',
     'astroquery',
     'aqsconverters',
-    #'aqsconverters @ git+https://github.com/oda-hub/aqsmodel-converters@simple-autolog#egg=aqsconverters',
+    'nb2workflow>=1.3.41',
     'pyvis==0.3.0',
     'pydotplus',
     'lockfile'
 ]
 
 packages = find_packages()
 version_file = open('VERSION')
```

### Comparing `renku-aqs-1.0.4/tests/test_example.py` & `renku-aqs-1.0.5/tests/test_example.py`

 * *Files identical despite different names*

