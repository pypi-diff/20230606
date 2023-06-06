# Comparing `tmp/clipol-1.tar.gz` & `tmp/clipol-2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipol-1.tar", last modified: Tue Jun  6 11:27:40 2023, max compression
+gzip compressed data, was "clipol-2.tar", last modified: Tue Jun  6 15:34:30 2023, max compression
```

## Comparing `clipol-1.tar` & `clipol-2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-06 11:27:40.209272 clipol-1/
--rw-rw-r--   0 coco      (1000) coco      (1000)      518 2023-06-06 11:27:40.209272 clipol-1/PKG-INFO
--rw-rw-r--   0 coco      (1000) coco      (1000)     3608 2020-12-08 21:30:42.000000 clipol-1/README
-drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-06 11:27:40.209272 clipol-1/clipol.egg-info/
--rw-rw-r--   0 coco      (1000) coco      (1000)      518 2023-06-06 11:27:40.000000 clipol-1/clipol.egg-info/PKG-INFO
--rw-rw-r--   0 coco      (1000) coco      (1000)      143 2023-06-06 11:27:40.000000 clipol-1/clipol.egg-info/SOURCES.txt
--rw-rw-r--   0 coco      (1000) coco      (1000)        1 2023-06-06 11:27:40.000000 clipol-1/clipol.egg-info/dependency_links.txt
--rw-rw-r--   0 coco      (1000) coco      (1000)        5 2023-06-06 11:27:40.000000 clipol-1/clipol.egg-info/top_level.txt
--rwxrwxr-x   0 coco      (1000) coco      (1000)    17299 2023-06-06 11:16:00.000000 clipol-1/ipol.py
--rw-rw-r--   0 coco      (1000) coco      (1000)       38 2023-06-06 11:27:40.209272 clipol-1/setup.cfg
--rw-rw-r--   0 coco      (1000) coco      (1000)      535 2023-06-06 11:27:21.000000 clipol-1/setup.py
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-06 15:34:30.519775 clipol-2/
+-rw-rw-r--   0 coco      (1000) coco      (1000)      518 2023-06-06 15:34:30.519775 clipol-2/PKG-INFO
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3608 2020-12-08 21:30:42.000000 clipol-2/README
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-06 15:34:30.515775 clipol-2/clipol.egg-info/
+-rw-rw-r--   0 coco      (1000) coco      (1000)      518 2023-06-06 15:34:30.000000 clipol-2/clipol.egg-info/PKG-INFO
+-rw-rw-r--   0 coco      (1000) coco      (1000)      143 2023-06-06 15:34:30.000000 clipol-2/clipol.egg-info/SOURCES.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)        1 2023-06-06 15:34:30.000000 clipol-2/clipol.egg-info/dependency_links.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)        5 2023-06-06 15:34:30.000000 clipol-2/clipol.egg-info/top_level.txt
+-rwxrwxr-x   0 coco      (1000) coco      (1000)    17666 2023-06-06 15:34:25.000000 clipol-2/ipol.py
+-rw-rw-r--   0 coco      (1000) coco      (1000)       38 2023-06-06 15:34:30.519775 clipol-2/setup.cfg
+-rw-rw-r--   0 coco      (1000) coco      (1000)      535 2023-06-06 15:34:18.000000 clipol-2/setup.py
```

### Comparing `clipol-1/PKG-INFO` & `clipol-2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipol
-Version: 1
+Version: 2
 Summary: python interface to some IPOL journal algorithms
 Home-page: https://git.sr.ht/~coco/clipol
 Author: Enric Meinhardt-Llopis
 Author-email: enric.meinhardt@ens-paris-saclay.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `clipol-1/README` & `clipol-2/README`

 * *Files identical despite different names*

### Comparing `clipol-1/clipol.egg-info/PKG-INFO` & `clipol-2/clipol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipol
-Version: 1
+Version: 2
 Summary: python interface to some IPOL journal algorithms
 Home-page: https://git.sr.ht/~coco/clipol
 Author: Enric Meinhardt-Llopis
 Author-email: enric.meinhardt@ens-paris-saclay.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `clipol-1/ipol.py` & `clipol-2/ipol.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,42 @@
 				p[c].append(k)
 			else:
 				key = k.partition("=")[0].strip()
 				val = k.partition("=")[2].strip()
 				p[c][key] = val
 	return p
 
+
+# check whether an article is already unzipped and built
+def ipol_is_built(p):
+	import os
+	name = p['NAME']
+	mycache = "%s/%s" % (IPOL_CACHE, name)
+	if not os.path.exists(mycache):
+		return False
+	bindir = "%s/bin" % mycache
+	if not os.path.exists(bindir):
+		return False
+	if len(os.listdir(bindir)) < 1:
+		return False
+	return True
+
+
+# auxiliary function to get the SRCDIR of an article (with some heuristics)
+def get_srcdir(p):
+	import os
+	name = p['NAME']
+	mysrc = "%s/%s/src" % (IPOL_CACHE, name)
+	l = os.listdir(mysrc)
+	if len(l) == 1:
+		return f"{mysrc}/{l[0]}"
+	else:
+		return mysrc
+
+
 # download, build and cache an ipol code
 def ipol_build_interface(p):
 	import os
 	import shutil
 	import subprocess
 	dprint(f"IPOL: ipol_build_interface")
 	dprint("building interface \"%s\"" % p)
@@ -152,41 +180,28 @@
 	os.makedirs("%s/bin" % mycache)
 	os.makedirs("%s/tmp" % mycache)
 
 	os.system("wget -P %s/dl %s" % (mycache, srcurl))
 	mysrc = os.listdir("%s/dl" % mycache)[0]
 	shutil.unpack_archive("%s/dl/%s" % (mycache,mysrc), "%s/src" % mycache)
 
-	l = os.listdir("%s/src" % mycache)
-	if len(l) != 1:
-		fail("more than one file! %s" % l)
-	srcdir = "%s/src/%s" % (mycache, l[0])
+	srcdir = get_srcdir(p)
 	bindir = "%s/bin" % mycache
+	dprint(f"srcdir = {srcdir}")
+	dprint(f"bindir = {bindir}")
+
 	popd = os.getcwd()
 	os.chdir(srcdir)
 	buildscript = "%s/%s" % (srcdir, BUILD_SCRIPT_NAME)
 	with open(buildscript, "w") as f:
 		f.write("export BIN=%s\n" % bindir)
 		f.writelines(["%s\n" % i  for i in p['BUILD']])
 	subprocess.call(". %s" % buildscript, shell=True)
 	os.chdir(popd)
 
-def ipol_is_built(p):
-	import os
-	name = p['NAME']
-	mycache = "%s/%s" % (IPOL_CACHE, name)
-	if not os.path.exists(mycache):
-		return False
-	bindir = "%s/bin" % mycache
-	if not os.path.exists(bindir):
-		return False
-	if len(os.listdir(bindir)) < 1:
-		return False
-	return True
-
 def ipol_signature(p):
 	nb_in = 0
 	nb_out = 0
 	for k,v in p['INPUT'].items():
 		#a,_,b = tuple(x.strip() for x in v.partition(":"))
 		#print("\tinpupa k(%s) a(%s) b(%s)" % (k,v[0],v[1]))
 		if len(v[1]) == 0:
@@ -294,14 +309,15 @@
 
 
 	# 3. write the call script into the sanitized run environement
 	callscript = "%s/%s" % (tmpdir, CALL_SCRIPT_NAME)
 	with open(callscript, "w") as f:
 		from string import Template
 		f.write("export PATH=%s:$PATH\n" % bindir)
+		f.write("export SRCDIR=%s\n" % get_srcdir(p))
 		f.writelines(["%s\n" % Template(i).safe_substitute(m)
 		              for i in p['RUN']])
 
 	# 4. run the call script
 	import subprocess
 	#subprocess.call("pwd;cat %s" % callscript, shell=True, cwd=tmpdir)
 	subprocess.call(". %s" % callscript, shell=True, cwd=tmpdir)
@@ -436,14 +452,15 @@
 		iio.write(fname, args[idx])
 
 	# 3. write the call script into the sanitized run environement
 	callscript = "%s/%s" % (tmpdir, CALL_SCRIPT_NAME)
 	with open(callscript, "w") as f:
 		from string import Template
 		f.write("export PATH=%s:$PATH\n" % bindir)
+		f.write("export SRCDIR=%s\n" % get_srcdir(p))
 		f.writelines(["%s\n" % Template(i).safe_substitute(m)
 		              for i in p['RUN']])
 
 	# 4. run the call script
 	import subprocess
 	#subprocess.call("pwd;cat %s" % callscript, shell=True, cwd=tmpdir)
 	subprocess.call(". %s" % callscript, shell=True, cwd=tmpdir)
@@ -592,10 +609,10 @@
 	idls = os.listdir(f"{IPOL_CONFIG}/idl")
 	idls = [ x[:-11] if x.endswith(".Dockerfile") else x for x in idls ]
 	for i in idls:
 		export_article_interface(i)
 
 
 # API
-version = 1
+version = 2
 
 # vim: sw=8 ts=8 sts=0 noexpandtab:
```

### Comparing `clipol-1/setup.py` & `clipol-2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
 	name = "clipol",
-	version = "1",
+	version = "2",
 	author = "Enric Meinhardt-Llopis",
 	author_email = "enric.meinhardt@ens-paris-saclay.fr",
 	description = "python interface to some IPOL journal algorithms",
 	url = "https://git.sr.ht/~coco/clipol",
 	classifiers = [
 		"Operating System :: OS Independent",
 		"License :: OSI Approved :: GNU Affero General Public License v3",
```

