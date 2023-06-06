# Comparing `tmp/clipol-3.tar.gz` & `tmp/clipol-4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipol-3.tar", last modified: Tue Jun  6 16:04:50 2023, max compression
+gzip compressed data, was "clipol-4.tar", last modified: Tue Jun  6 16:41:41 2023, max compression
```

## Comparing `clipol-3.tar` & `clipol-4.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-06 16:04:50.361706 clipol-3/
--rw-rw-r--   0 coco      (1000) coco      (1000)       56 2023-06-06 16:04:33.000000 clipol-3/MANIFEST.in
--rw-rw-r--   0 coco      (1000) coco      (1000)      518 2023-06-06 16:04:50.361706 clipol-3/PKG-INFO
--rw-rw-r--   0 coco      (1000) coco      (1000)     3608 2020-12-08 21:30:42.000000 clipol-3/README
-drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-06 16:04:50.361706 clipol-3/clipol.egg-info/
--rw-rw-r--   0 coco      (1000) coco      (1000)      518 2023-06-06 16:04:50.000000 clipol-3/clipol.egg-info/PKG-INFO
--rw-rw-r--   0 coco      (1000) coco      (1000)      408 2023-06-06 16:04:50.000000 clipol-3/clipol.egg-info/SOURCES.txt
--rw-rw-r--   0 coco      (1000) coco      (1000)        1 2023-06-06 16:04:50.000000 clipol-3/clipol.egg-info/dependency_links.txt
--rw-rw-r--   0 coco      (1000) coco      (1000)        5 2023-06-06 16:04:50.000000 clipol-3/clipol.egg-info/top_level.txt
-drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-06 16:04:50.361706 clipol-3/idl/
--rw-rw-r--   0 coco      (1000) coco      (1000)      358 2023-06-06 11:16:00.000000 clipol-3/idl/ace.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      623 2023-06-06 11:16:00.000000 clipol-3/idl/bm3d.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      545 2023-06-06 13:51:32.000000 clipol-3/idl/dctdenoise.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      758 2023-06-06 15:32:45.000000 clipol-3/idl/ffdnet.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      280 2020-12-08 23:32:50.000000 clipol-3/idl/lsd.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      996 2023-06-06 13:02:24.000000 clipol-3/idl/msdctd.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      597 2023-06-06 14:02:48.000000 clipol-3/idl/nlbayes.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      380 2023-06-06 11:16:00.000000 clipol-3/idl/nlm.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      209 2023-06-06 11:16:00.000000 clipol-3/idl/phs.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      441 2020-12-08 18:01:47.000000 clipol-3/idl/scb.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      379 2023-06-06 11:16:00.000000 clipol-3/idl/tvdenoise.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      303 2020-12-08 23:21:23.000000 clipol-3/idl/tvl1.Dockerfile
--rwxrwxr-x   0 coco      (1000) coco      (1000)    18151 2023-06-06 16:01:32.000000 clipol-3/ipol.py
--rw-rw-r--   0 coco      (1000) coco      (1000)       38 2023-06-06 16:04:50.361706 clipol-3/setup.cfg
--rw-rw-r--   0 coco      (1000) coco      (1000)      535 2023-06-06 16:01:37.000000 clipol-3/setup.py
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-06 16:41:41.796714 clipol-4/
+-rw-rw-r--   0 coco      (1000) coco      (1000)      518 2023-06-06 16:41:41.796714 clipol-4/PKG-INFO
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3608 2020-12-08 21:30:42.000000 clipol-4/README
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-06 16:41:41.792714 clipol-4/clipol.egg-info/
+-rw-rw-r--   0 coco      (1000) coco      (1000)      518 2023-06-06 16:41:41.000000 clipol-4/clipol.egg-info/PKG-INFO
+-rw-rw-r--   0 coco      (1000) coco      (1000)      396 2023-06-06 16:41:41.000000 clipol-4/clipol.egg-info/SOURCES.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)        1 2023-06-06 16:41:41.000000 clipol-4/clipol.egg-info/dependency_links.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)        5 2023-06-06 16:41:41.000000 clipol-4/clipol.egg-info/top_level.txt
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-06 16:41:41.796714 clipol-4/idl/
+-rw-rw-r--   0 coco      (1000) coco      (1000)      358 2023-06-06 11:16:00.000000 clipol-4/idl/ace.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      623 2023-06-06 11:16:00.000000 clipol-4/idl/bm3d.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      545 2023-06-06 13:51:32.000000 clipol-4/idl/dctdenoise.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      758 2023-06-06 15:32:45.000000 clipol-4/idl/ffdnet.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      280 2020-12-08 23:32:50.000000 clipol-4/idl/lsd.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      996 2023-06-06 13:02:24.000000 clipol-4/idl/msdctd.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      597 2023-06-06 14:02:48.000000 clipol-4/idl/nlbayes.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      380 2023-06-06 11:16:00.000000 clipol-4/idl/nlm.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      209 2023-06-06 11:16:00.000000 clipol-4/idl/phs.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      441 2020-12-08 18:01:47.000000 clipol-4/idl/scb.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      379 2023-06-06 11:16:00.000000 clipol-4/idl/tvdenoise.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      303 2020-12-08 23:21:23.000000 clipol-4/idl/tvl1.Dockerfile
+-rwxrwxr-x   0 coco      (1000) coco      (1000)    18288 2023-06-06 16:37:46.000000 clipol-4/ipol.py
+-rw-rw-r--   0 coco      (1000) coco      (1000)       38 2023-06-06 16:41:41.796714 clipol-4/setup.cfg
+-rw-rw-r--   0 coco      (1000) coco      (1000)      643 2023-06-06 16:41:33.000000 clipol-4/setup.py
```

### Comparing `clipol-3/PKG-INFO` & `clipol-4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipol
-Version: 3
+Version: 4
 Summary: python interface to some IPOL journal algorithms
 Home-page: https://git.sr.ht/~coco/clipol
 Author: Enric Meinhardt-Llopis
 Author-email: enric.meinhardt@ens-paris-saclay.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `clipol-3/README` & `clipol-4/README`

 * *Files identical despite different names*

### Comparing `clipol-3/clipol.egg-info/PKG-INFO` & `clipol-4/clipol.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipol
-Version: 3
+Version: 4
 Summary: python interface to some IPOL journal algorithms
 Home-page: https://git.sr.ht/~coco/clipol
 Author: Enric Meinhardt-Llopis
 Author-email: enric.meinhardt@ens-paris-saclay.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `clipol-3/idl/bm3d.Dockerfile` & `clipol-4/idl/bm3d.Dockerfile`

 * *Files identical despite different names*

### Comparing `clipol-3/idl/dctdenoise.Dockerfile` & `clipol-4/idl/dctdenoise.Dockerfile`

 * *Files identical despite different names*

### Comparing `clipol-3/idl/ffdnet.Dockerfile` & `clipol-4/idl/ffdnet.Dockerfile`

 * *Files identical despite different names*

### Comparing `clipol-3/idl/msdctd.Dockerfile` & `clipol-4/idl/msdctd.Dockerfile`

 * *Files identical despite different names*

### Comparing `clipol-3/idl/nlbayes.Dockerfile` & `clipol-4/idl/nlbayes.Dockerfile`

 * *Files identical despite different names*

### Comparing `clipol-3/ipol.py` & `clipol-4/ipol.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 DEBUG_LEVEL = 1
 IPOL_CACHE = "/tmp/ipol/cache"
 IPOL_CONFIG = "/tmp/ipol/config"
 #IPOL_CACHE = "%s/.cache/ipol" % os.path.expanduser("~")
 #IPOL_CONFIG = "%s/.config/ipol" % os.path.expanduser("~")
 #IPOL_CONFIG = "/home/coco/src/clipol"
 def setup_global_variables():
-	import os
 	global IPOL_CACHE
 	global IPOL_CONFIG
 
 	# cache is easy
+	import os
 	IPOL_CACHE = "%s/.cache/ipol" % os.path.expanduser("~")
 
 	# config is harder...
 	# if ~/.config/ipol/idl/lsd.Dockerfile exists, use that folder
-	# otherwise it's the idl folder besides this ipol.py
-	IPOL_CONFIG = os.path.dirname(os.path.realpath(__file__))
-	t = "%s/.config/ipol" % os.path.expanduser("~")
-	if os.path.exists(f"{t}/idl/lsd.Dockerfile"):
-		IPOL_CONFIG = t
+	# if there's an idl folder besides this ipol.py, use that
+	# otherwise, use site.USER_BASE
+
+	import site
+	IPOL_CONFIG = site.USER_BASE
+	x = os.path.dirname(os.path.realpath(__file__))
+	if os.path.exists(f"{x}/idl/lsd.Dockerfile"):
+		IPOL_CONFIG = x
+	x = "%s/.config/ipol" % os.path.expanduser("~")
+	if os.path.exists(f"{x}/idl/lsd.Dockerfile"):
+		IPOL_CONFIG = x
 
 setup_global_variables()
 
 
 # arbitrary names for temporary files
 BUILD_SCRIPT_NAME = "_ipol_build_script.sh"
 CALL_SCRIPT_NAME = "_ipol_call_script.sh"
@@ -624,10 +630,10 @@
 	idls = os.listdir(f"{IPOL_CONFIG}/idl")
 	idls = [ x[:-11] if x.endswith(".Dockerfile") else x for x in idls ]
 	for i in idls:
 		export_article_interface(i)
 
 
 # API
-version = 3
+version = 4
 
 # vim: sw=8 ts=8 sts=0 noexpandtab:
```

### Comparing `clipol-3/setup.py` & `clipol-4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import setuptools
 
+def data_files():
+	import glob
+	return glob.glob("idl/*.Dockerfile")
+
 setuptools.setup(
 	name = "clipol",
-	version = "3",
+	version = "4",
 	author = "Enric Meinhardt-Llopis",
 	author_email = "enric.meinhardt@ens-paris-saclay.fr",
 	description = "python interface to some IPOL journal algorithms",
 	url = "https://git.sr.ht/~coco/clipol",
 	classifiers = [
 		"Operating System :: OS Independent",
 		"License :: OSI Approved :: GNU Affero General Public License v3",
 		"Topic :: Scientific/Engineering :: Image Processing",
 		"Topic :: Scientific/Engineering :: Mathematics"
 		],
-	py_modules = ["ipol"]
+	py_modules = ["ipol"],
+	data_files = [("idl", data_files())]
 )
-
```

