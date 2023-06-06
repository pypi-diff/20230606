# Comparing `tmp/clipol-2.tar.gz` & `tmp/clipol-3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipol-2.tar", last modified: Tue Jun  6 15:34:30 2023, max compression
+gzip compressed data, was "clipol-3.tar", last modified: Tue Jun  6 16:04:50 2023, max compression
```

## Comparing `clipol-2.tar` & `clipol-3.tar`

### file list

```diff
@@ -1,11 +1,25 @@
-drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-06 15:34:30.519775 clipol-2/
--rw-rw-r--   0 coco      (1000) coco      (1000)      518 2023-06-06 15:34:30.519775 clipol-2/PKG-INFO
--rw-rw-r--   0 coco      (1000) coco      (1000)     3608 2020-12-08 21:30:42.000000 clipol-2/README
-drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-06 15:34:30.515775 clipol-2/clipol.egg-info/
--rw-rw-r--   0 coco      (1000) coco      (1000)      518 2023-06-06 15:34:30.000000 clipol-2/clipol.egg-info/PKG-INFO
--rw-rw-r--   0 coco      (1000) coco      (1000)      143 2023-06-06 15:34:30.000000 clipol-2/clipol.egg-info/SOURCES.txt
--rw-rw-r--   0 coco      (1000) coco      (1000)        1 2023-06-06 15:34:30.000000 clipol-2/clipol.egg-info/dependency_links.txt
--rw-rw-r--   0 coco      (1000) coco      (1000)        5 2023-06-06 15:34:30.000000 clipol-2/clipol.egg-info/top_level.txt
--rwxrwxr-x   0 coco      (1000) coco      (1000)    17666 2023-06-06 15:34:25.000000 clipol-2/ipol.py
--rw-rw-r--   0 coco      (1000) coco      (1000)       38 2023-06-06 15:34:30.519775 clipol-2/setup.cfg
--rw-rw-r--   0 coco      (1000) coco      (1000)      535 2023-06-06 15:34:18.000000 clipol-2/setup.py
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-06 16:04:50.361706 clipol-3/
+-rw-rw-r--   0 coco      (1000) coco      (1000)       56 2023-06-06 16:04:33.000000 clipol-3/MANIFEST.in
+-rw-rw-r--   0 coco      (1000) coco      (1000)      518 2023-06-06 16:04:50.361706 clipol-3/PKG-INFO
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3608 2020-12-08 21:30:42.000000 clipol-3/README
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-06 16:04:50.361706 clipol-3/clipol.egg-info/
+-rw-rw-r--   0 coco      (1000) coco      (1000)      518 2023-06-06 16:04:50.000000 clipol-3/clipol.egg-info/PKG-INFO
+-rw-rw-r--   0 coco      (1000) coco      (1000)      408 2023-06-06 16:04:50.000000 clipol-3/clipol.egg-info/SOURCES.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)        1 2023-06-06 16:04:50.000000 clipol-3/clipol.egg-info/dependency_links.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)        5 2023-06-06 16:04:50.000000 clipol-3/clipol.egg-info/top_level.txt
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-06 16:04:50.361706 clipol-3/idl/
+-rw-rw-r--   0 coco      (1000) coco      (1000)      358 2023-06-06 11:16:00.000000 clipol-3/idl/ace.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      623 2023-06-06 11:16:00.000000 clipol-3/idl/bm3d.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      545 2023-06-06 13:51:32.000000 clipol-3/idl/dctdenoise.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      758 2023-06-06 15:32:45.000000 clipol-3/idl/ffdnet.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      280 2020-12-08 23:32:50.000000 clipol-3/idl/lsd.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      996 2023-06-06 13:02:24.000000 clipol-3/idl/msdctd.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      597 2023-06-06 14:02:48.000000 clipol-3/idl/nlbayes.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      380 2023-06-06 11:16:00.000000 clipol-3/idl/nlm.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      209 2023-06-06 11:16:00.000000 clipol-3/idl/phs.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      441 2020-12-08 18:01:47.000000 clipol-3/idl/scb.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      379 2023-06-06 11:16:00.000000 clipol-3/idl/tvdenoise.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      303 2020-12-08 23:21:23.000000 clipol-3/idl/tvl1.Dockerfile
+-rwxrwxr-x   0 coco      (1000) coco      (1000)    18151 2023-06-06 16:01:32.000000 clipol-3/ipol.py
+-rw-rw-r--   0 coco      (1000) coco      (1000)       38 2023-06-06 16:04:50.361706 clipol-3/setup.cfg
+-rw-rw-r--   0 coco      (1000) coco      (1000)      535 2023-06-06 16:01:37.000000 clipol-3/setup.py
```

### Comparing `clipol-2/PKG-INFO` & `clipol-3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipol
-Version: 2
+Version: 3
 Summary: python interface to some IPOL journal algorithms
 Home-page: https://git.sr.ht/~coco/clipol
 Author: Enric Meinhardt-Llopis
 Author-email: enric.meinhardt@ens-paris-saclay.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `clipol-2/README` & `clipol-3/README`

 * *Files identical despite different names*

### Comparing `clipol-2/clipol.egg-info/PKG-INFO` & `clipol-3/clipol.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipol
-Version: 2
+Version: 3
 Summary: python interface to some IPOL journal algorithms
 Home-page: https://git.sr.ht/~coco/clipol
 Author: Enric Meinhardt-Llopis
 Author-email: enric.meinhardt@ens-paris-saclay.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `clipol-2/ipol.py` & `clipol-3/ipol.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 #!/usr/bin/env python3
 
 # global configuration options
 DEBUG_LEVEL = 1
-IPOL_CACHE = "/tmp/cache/ipol"
+IPOL_CACHE = "/tmp/ipol/cache"
+IPOL_CONFIG = "/tmp/ipol/config"
 #IPOL_CACHE = "%s/.cache/ipol" % os.path.expanduser("~")
 #IPOL_CONFIG = "%s/.config/ipol" % os.path.expanduser("~")
-IPOL_CONFIG = "/home/coco/src/clipol"
+#IPOL_CONFIG = "/home/coco/src/clipol"
 def setup_global_variables():
 	import os
 	global IPOL_CACHE
 	global IPOL_CONFIG
+
+	# cache is easy
 	IPOL_CACHE = "%s/.cache/ipol" % os.path.expanduser("~")
-	IPOL_CONFIG = "/home/coco/src/clipol"
+
+	# config is harder...
+	# if ~/.config/ipol/idl/lsd.Dockerfile exists, use that folder
+	# otherwise it's the idl folder besides this ipol.py
+	IPOL_CONFIG = os.path.dirname(os.path.realpath(__file__))
+	t = "%s/.config/ipol" % os.path.expanduser("~")
+	if os.path.exists(f"{t}/idl/lsd.Dockerfile"):
+		IPOL_CONFIG = t
+
 setup_global_variables()
 
 
 # arbitrary names for temporary files
 BUILD_SCRIPT_NAME = "_ipol_build_script.sh"
 CALL_SCRIPT_NAME = "_ipol_call_script.sh"
 
@@ -593,26 +604,30 @@
 	if len(sys.argv) == 2:
 		return main_info(sys.argv[1])
 	return main_article(sys.argv[1:])
 
 # ipol.sh: the shell interface
 if __name__ == "__main__":
 	dprint(f"IPOL: entering shell interface")
+	dprint(f"IPOL_CONFIG = {IPOL_CONFIG}")
+	dprint(f"IPOL_CACHE = {IPOL_CACHE}")
 	import sys
 	sys.dont_write_bytecode = True
 	sys.exit(main())
 
 # ipol.py: the import-able interface
 if __name__ == "ipol":
 	dprint(f"IPOL: entering importable interface")
+	dprint(f"IPOL_CONFIG = {IPOL_CONFIG}")
+	dprint(f"IPOL_CACHE = {IPOL_CACHE}")
 	#available_idls = ("scb", "lsd")  # TODO: traverse the idl folder
 	import os
 	idls = os.listdir(f"{IPOL_CONFIG}/idl")
 	idls = [ x[:-11] if x.endswith(".Dockerfile") else x for x in idls ]
 	for i in idls:
 		export_article_interface(i)
 
 
 # API
-version = 2
+version = 3
 
 # vim: sw=8 ts=8 sts=0 noexpandtab:
```

### Comparing `clipol-2/setup.py` & `clipol-3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
 	name = "clipol",
-	version = "2",
+	version = "3",
 	author = "Enric Meinhardt-Llopis",
 	author_email = "enric.meinhardt@ens-paris-saclay.fr",
 	description = "python interface to some IPOL journal algorithms",
 	url = "https://git.sr.ht/~coco/clipol",
 	classifiers = [
 		"Operating System :: OS Independent",
 		"License :: OSI Approved :: GNU Affero General Public License v3",
```

