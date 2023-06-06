# Comparing `tmp/gkligo-0.1.6.tar.gz` & `tmp/gkligo-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gkligo-0.1.6.tar", last modified: Mon May 29 23:27:01 2023, max compression
+gzip compressed data, was "gkligo-0.1.8.tar", last modified: Tue Jun  6 12:23:22 2023, max compression
```

## Comparing `gkligo-0.1.6.tar` & `gkligo-0.1.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-29 23:27:01.157066 gkligo-0.1.6/
--rw-r--r--   0 kws        (502) staff       (20)       74 2023-03-08 21:39:07.000000 gkligo-0.1.6/MANIFEST.in
--rw-r--r--   0 kws        (502) staff       (20)     1794 2023-05-29 23:27:01.156579 gkligo-0.1.6/PKG-INFO
--rw-r--r--   0 kws        (502) staff       (20)     1089 2023-05-24 11:09:44.000000 gkligo-0.1.6/README.md
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-29 23:27:01.143845 gkligo-0.1.6/gkligo/
--rw-r--r--   0 kws        (502) staff       (20)       22 2023-04-28 14:27:19.000000 gkligo-0.1.6/gkligo/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)       22 2023-05-29 23:26:40.000000 gkligo-0.1.6/gkligo/__version__.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-29 23:27:01.146783 gkligo-0.1.6/gkligo/scripts/
--rw-r--r--   0 kws        (502) staff       (20)       21 2023-03-08 21:34:47.000000 gkligo-0.1.6/gkligo/scripts/__init__.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-29 23:27:01.155458 gkligo-0.1.6/gkligo/scripts/python/
--rw-r--r--   0 kws        (502) staff       (20)        0 2023-05-28 12:23:50.000000 gkligo-0.1.6/gkligo/scripts/python/=
--rw-r--r--   0 kws        (502) staff       (20)       31 2023-04-28 14:27:05.000000 gkligo-0.1.6/gkligo/scripts/python/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)       89 2023-04-20 16:53:23.000000 gkligo-0.1.6/gkligo/scripts/python/config_download_example.yaml
--rw-r--r--   0 kws        (502) staff       (20)      426 2023-04-24 12:50:06.000000 gkligo-0.1.6/gkligo/scripts/python/config_reports.yaml
--rw-r--r--   0 kws        (502) staff       (20)      498 2023-04-24 13:37:26.000000 gkligo-0.1.6/gkligo/scripts/python/config_reports_example.yaml
--rwxr-xr-x   0 kws        (502) staff       (20)    13101 2023-05-29 23:26:40.000000 gkligo-0.1.6/gkligo/scripts/python/downloadGWAlerts.py
--rwxr-xr-x   0 kws        (502) staff       (20)     5793 2023-05-26 22:32:11.000000 gkligo-0.1.6/gkligo/scripts/python/generateGWReports.py
--rw-r--r--   0 kws        (502) staff       (20)      267 2023-05-29 14:39:19.000000 gkligo-0.1.6/gkligo/scripts/python/test.py
--rw-r--r--   0 kws        (502) staff       (20)     1266 2023-05-23 20:34:59.000000 gkligo-0.1.6/gkligo/scripts/python/test.yaml
--rwxr-xr-x   0 kws        (502) staff       (20)     2792 2023-04-27 21:33:22.000000 gkligo-0.1.6/gkligo/scripts/python/testDaemon.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-29 23:27:01.146362 gkligo-0.1.6/gkligo.egg-info/
--rw-r--r--   0 kws        (502) staff       (20)     1794 2023-05-29 23:27:01.000000 gkligo-0.1.6/gkligo.egg-info/PKG-INFO
--rw-r--r--   0 kws        (502) staff       (20)      664 2023-05-29 23:27:01.000000 gkligo-0.1.6/gkligo.egg-info/SOURCES.txt
--rw-r--r--   0 kws        (502) staff       (20)        1 2023-05-29 23:27:01.000000 gkligo-0.1.6/gkligo.egg-info/dependency_links.txt
--rw-r--r--   0 kws        (502) staff       (20)      147 2023-05-29 23:27:01.000000 gkligo-0.1.6/gkligo.egg-info/entry_points.txt
--rw-r--r--   0 kws        (502) staff       (20)       85 2023-05-29 23:27:01.000000 gkligo-0.1.6/gkligo.egg-info/requires.txt
--rw-r--r--   0 kws        (502) staff       (20)        7 2023-05-29 23:27:01.000000 gkligo-0.1.6/gkligo.egg-info/top_level.txt
--rw-r--r--   0 kws        (502) staff       (20)       38 2023-05-29 23:27:01.157322 gkligo-0.1.6/setup.cfg
--rwxr-xr-x   0 kws        (502) staff       (20)     1308 2023-04-24 13:23:15.000000 gkligo-0.1.6/setup.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-06-06 12:23:22.822497 gkligo-0.1.8/
+-rw-r--r--   0 kws        (502) staff       (20)       74 2023-03-08 21:39:07.000000 gkligo-0.1.8/MANIFEST.in
+-rw-r--r--   0 kws        (502) staff       (20)     1794 2023-06-06 12:23:22.822049 gkligo-0.1.8/PKG-INFO
+-rw-r--r--   0 kws        (502) staff       (20)     1089 2023-05-24 11:09:44.000000 gkligo-0.1.8/README.md
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-06-06 12:23:22.809628 gkligo-0.1.8/gkligo/
+-rw-r--r--   0 kws        (502) staff       (20)       22 2023-04-28 14:27:19.000000 gkligo-0.1.8/gkligo/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)       22 2023-06-06 12:22:01.000000 gkligo-0.1.8/gkligo/__version__.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-06-06 12:23:22.812624 gkligo-0.1.8/gkligo/scripts/
+-rw-r--r--   0 kws        (502) staff       (20)       21 2023-03-08 21:34:47.000000 gkligo-0.1.8/gkligo/scripts/__init__.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-06-06 12:23:22.820797 gkligo-0.1.8/gkligo/scripts/python/
+-rw-r--r--   0 kws        (502) staff       (20)        0 2023-05-28 12:23:50.000000 gkligo-0.1.8/gkligo/scripts/python/=
+-rw-r--r--   0 kws        (502) staff       (20)       31 2023-04-28 14:27:05.000000 gkligo-0.1.8/gkligo/scripts/python/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)       89 2023-04-20 16:53:23.000000 gkligo-0.1.8/gkligo/scripts/python/config_download_example.yaml
+-rw-r--r--   0 kws        (502) staff       (20)      426 2023-04-24 12:50:06.000000 gkligo-0.1.8/gkligo/scripts/python/config_reports.yaml
+-rw-r--r--   0 kws        (502) staff       (20)      498 2023-04-24 13:37:26.000000 gkligo-0.1.8/gkligo/scripts/python/config_reports_example.yaml
+-rwxr-xr-x   0 kws        (502) staff       (20)    13101 2023-05-29 23:26:40.000000 gkligo-0.1.8/gkligo/scripts/python/downloadGWAlerts.py
+-rwxr-xr-x   0 kws        (502) staff       (20)    15258 2023-06-06 12:21:12.000000 gkligo-0.1.8/gkligo/scripts/python/generateGWReports.py
+-rw-r--r--   0 kws        (502) staff       (20)      267 2023-05-29 14:39:19.000000 gkligo-0.1.8/gkligo/scripts/python/test.py
+-rw-r--r--   0 kws        (502) staff       (20)     1266 2023-05-23 20:34:59.000000 gkligo-0.1.8/gkligo/scripts/python/test.yaml
+-rwxr-xr-x   0 kws        (502) staff       (20)     2792 2023-04-27 21:33:22.000000 gkligo-0.1.8/gkligo/scripts/python/testDaemon.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-06-06 12:23:22.811997 gkligo-0.1.8/gkligo.egg-info/
+-rw-r--r--   0 kws        (502) staff       (20)     1794 2023-06-06 12:23:22.000000 gkligo-0.1.8/gkligo.egg-info/PKG-INFO
+-rw-r--r--   0 kws        (502) staff       (20)      664 2023-06-06 12:23:22.000000 gkligo-0.1.8/gkligo.egg-info/SOURCES.txt
+-rw-r--r--   0 kws        (502) staff       (20)        1 2023-06-06 12:23:22.000000 gkligo-0.1.8/gkligo.egg-info/dependency_links.txt
+-rw-r--r--   0 kws        (502) staff       (20)      147 2023-06-06 12:23:22.000000 gkligo-0.1.8/gkligo.egg-info/entry_points.txt
+-rw-r--r--   0 kws        (502) staff       (20)       85 2023-06-06 12:23:22.000000 gkligo-0.1.8/gkligo.egg-info/requires.txt
+-rw-r--r--   0 kws        (502) staff       (20)        7 2023-06-06 12:23:22.000000 gkligo-0.1.8/gkligo.egg-info/top_level.txt
+-rw-r--r--   0 kws        (502) staff       (20)       38 2023-06-06 12:23:22.822703 gkligo-0.1.8/setup.cfg
+-rwxr-xr-x   0 kws        (502) staff       (20)     1308 2023-04-24 13:23:15.000000 gkligo-0.1.8/setup.py
```

### Comparing `gkligo-0.1.6/PKG-INFO` & `gkligo-0.1.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gkligo
-Version: 0.1.6
+Version: 0.1.8
 Summary: GW (LIGO) utilities
 Home-page: https://github.com/genghisken/gkligo
 Author: genghisken
 Author-email: ken.w.smith@gmail.com
 License: MIT
 Description: # gkligo
         Code to download GW Alert skymaps from Kafka, and optionally write them
```

### Comparing `gkligo-0.1.6/README.md` & `gkligo-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `gkligo-0.1.6/gkligo/scripts/python/downloadGWAlerts.py` & `gkligo-0.1.8/gkligo/scripts/python/downloadGWAlerts.py`

 * *Files identical despite different names*

### Comparing `gkligo-0.1.6/gkligo/scripts/python/test.yaml` & `gkligo-0.1.8/gkligo/scripts/python/test.yaml`

 * *Files identical despite different names*

### Comparing `gkligo-0.1.6/gkligo/scripts/python/testDaemon.py` & `gkligo-0.1.8/gkligo/scripts/python/testDaemon.py`

 * *Files identical despite different names*

### Comparing `gkligo-0.1.6/gkligo.egg-info/PKG-INFO` & `gkligo-0.1.8/gkligo.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gkligo
-Version: 0.1.6
+Version: 0.1.8
 Summary: GW (LIGO) utilities
 Home-page: https://github.com/genghisken/gkligo
 Author: genghisken
 Author-email: ken.w.smith@gmail.com
 License: MIT
 Description: # gkligo
         Code to download GW Alert skymaps from Kafka, and optionally write them
```

### Comparing `gkligo-0.1.6/gkligo.egg-info/SOURCES.txt` & `gkligo-0.1.8/gkligo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gkligo-0.1.6/setup.py` & `gkligo-0.1.8/setup.py`

 * *Files identical despite different names*

