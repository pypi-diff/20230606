# Comparing `tmp/ampltools-0.5.5.tar.gz` & `tmp/ampltools-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ampltools-0.5.5.tar", last modified: Tue Jun  6 10:57:45 2023, max compression
+gzip compressed data, was "ampltools-0.5.6.tar", last modified: Tue Jun  6 11:38:49 2023, max compression
```

## Comparing `ampltools-0.5.5.tar` & `ampltools-0.5.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-06-06 10:57:45.256783 ampltools-0.5.5/
--rw-r--r--   0 fdabrandao   (501) staff       (20)     2987 2023-06-06 10:15:43.000000 ampltools-0.5.5/CHANGELOG.md
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1522 2023-03-08 15:44:27.000000 ampltools-0.5.5/LICENSE
--rw-r--r--   0 fdabrandao   (501) staff       (20)       57 2023-03-08 15:44:27.000000 ampltools-0.5.5/MANIFEST.in
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1280 2023-06-06 10:57:45.256493 ampltools-0.5.5/PKG-INFO
--rw-r--r--   0 fdabrandao   (501) staff       (20)      446 2023-03-08 15:44:27.000000 ampltools-0.5.5/README.md
-drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-06-06 10:57:45.245542 ampltools-0.5.5/ampltools/
--rw-r--r--   0 fdabrandao   (501) staff       (20)      407 2023-06-06 10:18:36.000000 ampltools-0.5.5/ampltools/__init__.py
-drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-06-06 10:57:45.251606 ampltools-0.5.5/ampltools/modules/
--rw-r--r--   0 fdabrandao   (501) staff       (20)      451 2023-06-06 10:19:22.000000 ampltools-0.5.5/ampltools/modules/__init__.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)       93 2023-03-08 15:44:27.000000 ampltools-0.5.5/ampltools/modules/__main__.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)    13054 2023-06-06 10:38:28.000000 ampltools-0.5.5/ampltools/modules/amplpypi.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     4027 2023-06-06 10:46:36.000000 ampltools-0.5.5/ampltools/modules/commands.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     5838 2023-06-06 10:17:59.000000 ampltools-0.5.5/ampltools/notebooks.py
-drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-06-06 10:57:45.255835 ampltools-0.5.5/ampltools/tests/
--rw-r--r--   0 fdabrandao   (501) staff       (20)      433 2023-03-08 15:44:27.000000 ampltools-0.5.5/ampltools/tests/TestBase.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)       24 2023-03-08 15:44:27.000000 ampltools-0.5.5/ampltools/tests/__init__.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)      286 2023-03-08 15:44:27.000000 ampltools-0.5.5/ampltools/tests/__main__.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     3566 2023-03-08 15:44:27.000000 ampltools-0.5.5/ampltools/tests/test_install.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     2084 2023-06-06 10:42:43.000000 ampltools-0.5.5/ampltools/tests/test_load.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     2411 2023-03-13 18:25:11.000000 ampltools-0.5.5/ampltools/tests/test_preload.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1751 2023-03-08 15:44:27.000000 ampltools-0.5.5/ampltools/tests/test_run.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     3228 2023-03-09 15:37:57.000000 ampltools-0.5.5/ampltools/utils.py
-drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-06-06 10:57:45.248782 ampltools-0.5.5/ampltools.egg-info/
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1280 2023-06-06 10:57:45.000000 ampltools-0.5.5/ampltools.egg-info/PKG-INFO
--rw-r--r--   0 fdabrandao   (501) staff       (20)      621 2023-06-06 10:57:45.000000 ampltools-0.5.5/ampltools.egg-info/SOURCES.txt
--rw-r--r--   0 fdabrandao   (501) staff       (20)        1 2023-06-06 10:57:45.000000 ampltools-0.5.5/ampltools.egg-info/dependency_links.txt
--rw-r--r--   0 fdabrandao   (501) staff       (20)        9 2023-06-06 10:57:45.000000 ampltools-0.5.5/ampltools.egg-info/requires.txt
--rw-r--r--   0 fdabrandao   (501) staff       (20)       10 2023-06-06 10:57:45.000000 ampltools-0.5.5/ampltools.egg-info/top_level.txt
--rw-r--r--   0 fdabrandao   (501) staff       (20)        8 2023-03-08 15:44:27.000000 ampltools-0.5.5/requirements.txt
--rw-r--r--   0 fdabrandao   (501) staff       (20)       38 2023-06-06 10:57:45.256881 ampltools-0.5.5/setup.cfg
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1715 2023-06-06 10:18:36.000000 ampltools-0.5.5/setup.py
+drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-06-06 11:38:49.719372 ampltools-0.5.6/
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     3060 2023-06-06 11:33:03.000000 ampltools-0.5.6/CHANGELOG.md
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     1522 2023-03-08 15:44:27.000000 ampltools-0.5.6/LICENSE
+-rw-r--r--   0 fdabrandao   (501) staff       (20)       57 2023-03-08 15:44:27.000000 ampltools-0.5.6/MANIFEST.in
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     1280 2023-06-06 11:38:49.719115 ampltools-0.5.6/PKG-INFO
+-rw-r--r--   0 fdabrandao   (501) staff       (20)      446 2023-03-08 15:44:27.000000 ampltools-0.5.6/README.md
+drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-06-06 11:38:49.712758 ampltools-0.5.6/ampltools/
+-rw-r--r--   0 fdabrandao   (501) staff       (20)      407 2023-06-06 11:33:30.000000 ampltools-0.5.6/ampltools/__init__.py
+drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-06-06 11:38:49.715842 ampltools-0.5.6/ampltools/modules/
+-rw-r--r--   0 fdabrandao   (501) staff       (20)      451 2023-06-06 11:33:30.000000 ampltools-0.5.6/ampltools/modules/__init__.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)       93 2023-03-08 15:44:27.000000 ampltools-0.5.6/ampltools/modules/__main__.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)    13220 2023-06-06 11:34:00.000000 ampltools-0.5.6/ampltools/modules/amplpypi.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     4039 2023-06-06 11:34:32.000000 ampltools-0.5.6/ampltools/modules/commands.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     5838 2023-06-06 10:17:59.000000 ampltools-0.5.6/ampltools/notebooks.py
+drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-06-06 11:38:49.718719 ampltools-0.5.6/ampltools/tests/
+-rw-r--r--   0 fdabrandao   (501) staff       (20)      433 2023-03-08 15:44:27.000000 ampltools-0.5.6/ampltools/tests/TestBase.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)       24 2023-03-08 15:44:27.000000 ampltools-0.5.6/ampltools/tests/__init__.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)      286 2023-03-08 15:44:27.000000 ampltools-0.5.6/ampltools/tests/__main__.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     3566 2023-03-08 15:44:27.000000 ampltools-0.5.6/ampltools/tests/test_install.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     2101 2023-06-06 11:30:15.000000 ampltools-0.5.6/ampltools/tests/test_load.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     2411 2023-03-13 18:25:11.000000 ampltools-0.5.6/ampltools/tests/test_preload.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     1751 2023-03-08 15:44:27.000000 ampltools-0.5.6/ampltools/tests/test_run.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     3228 2023-03-09 15:37:57.000000 ampltools-0.5.6/ampltools/utils.py
+drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-06-06 11:38:49.714187 ampltools-0.5.6/ampltools.egg-info/
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     1280 2023-06-06 11:38:49.000000 ampltools-0.5.6/ampltools.egg-info/PKG-INFO
+-rw-r--r--   0 fdabrandao   (501) staff       (20)      621 2023-06-06 11:38:49.000000 ampltools-0.5.6/ampltools.egg-info/SOURCES.txt
+-rw-r--r--   0 fdabrandao   (501) staff       (20)        1 2023-06-06 11:38:49.000000 ampltools-0.5.6/ampltools.egg-info/dependency_links.txt
+-rw-r--r--   0 fdabrandao   (501) staff       (20)        9 2023-06-06 11:38:49.000000 ampltools-0.5.6/ampltools.egg-info/requires.txt
+-rw-r--r--   0 fdabrandao   (501) staff       (20)       10 2023-06-06 11:38:49.000000 ampltools-0.5.6/ampltools.egg-info/top_level.txt
+-rw-r--r--   0 fdabrandao   (501) staff       (20)        8 2023-03-08 15:44:27.000000 ampltools-0.5.6/requirements.txt
+-rw-r--r--   0 fdabrandao   (501) staff       (20)       38 2023-06-06 11:38:49.719457 ampltools-0.5.6/setup.cfg
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     1715 2023-06-06 11:33:30.000000 ampltools-0.5.6/setup.py
```

### Comparing `ampltools-0.5.5/CHANGELOG.md` & `ampltools-0.5.6/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Change Log
 All notable changes to this project will be documented in this file.
 This project adheres to [Semantic Versioning](http://semver.org/).
 
+## 0.5.6 - 2023-06-06
+- Adjust modules.find to find files, not modules.
+
 ## 0.5.5 - 2023-06-06
 - Add modules.find.
 
 ## 0.5.4 - 2023-05-30
 - ampl_notebook: Drop g/globals_ argument.
 - ampl_notebook: Remove button to use existing license.
```

### Comparing `ampltools-0.5.5/LICENSE` & `ampltools-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.5/PKG-INFO` & `ampltools-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ampltools
-Version: 0.5.5
+Version: 0.5.6
 Summary: AMPL Python Tools
 Home-page: http://ampl.com/
 Author: Filipe Brandão
 Author-email: fdabrandao@ampl.com
 License: BSD-3
 Download-URL: https://github.com/ampl/amplpy/tree/master/ampltools
 Description:
```

### Comparing `ampltools-0.5.5/ampltools/modules/amplpypi.py` & `ampltools-0.5.6/ampltools/modules/amplpypi.py`

 * *Files 2% similar despite different names*

```diff
@@ -372,35 +372,39 @@
         return True
     except:
         if not silently:
             raise
         return False
 
 
-def path(modules=[]):
+def path(modules=[], add_base=True):
     """
     Return PATH for AMPL modules.
     Args:
         modules: list of modules to be included.
     """
-    modules = _sort_modules_for_loading(modules)
+    modules = _sort_modules_for_loading(modules, add_base=add_base)
     return os.pathsep.join(_locate_modules(modules, verbose=False))
 
 
-def find(module):
+def find(filename):
     """
-    Return PATH for an AMPL module.
+    Find a file in AMPL modules.
     Args:
-        module: name of the module to locate.
+        filename: name of the file to locate.
     """
-    modules = _sort_modules_for_loading(module, add_base=False)
-    paths = _locate_modules(modules[:1], verbose=False)
-    if paths == []:
-        raise ModuleNotFoundError("Could not find AMPL module '{}'.".format(module))
-    return paths[0]
+    paths = path().split(os.pathsep)
+    for p in paths:
+        full_path = os.path.join(p, filename)
+        if os.path.isfile(full_path):
+            return full_path
+        full_path = os.path.join(p, filename + ".exe")
+        if os.path.isfile(full_path):
+            return full_path
+    raise FileNotFoundError("Could not find {} in any AMPL module.".format(filename))
 
 
 def activate_license(uuid, verbose=False):
     """
     Activate an AMPL license using the UUID.
     Args:
         uuid: license uuid.
```

### Comparing `ampltools-0.5.5/ampltools/modules/commands.py` & `ampltools-0.5.6/ampltools/modules/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,16 @@
     $ python -m $PACKAGE.modules available
 
 - Value to append to the environment variable PATH to access modules
     $ python -m $PACKAGE.modules path
     Example:
         $ export PATH=$PATH:`python -m amplpy.modules path`
 
-- Find the path to a specific module
-    $ python -m $PACKAGE.modules find <name>
+- Find the path to a file in any module
+    $ python -m $PACKAGE.modules find <file name>
     Example:
         $ python -m amplpy.modules find gurobi
 
 - Generate requirements.txt for the modules currently installed
     $ python -m $PACKAGE.modules requirements
 
 - Run command in the same environment as the modules:
@@ -100,16 +100,16 @@
             print("\t" + name)
     elif command == "path":
         modules = [m for m in args if not m.startswith("-")]
         print(path(modules))
     elif command == "find":
         if len(args) != 1:
             raise Exception(ERROR + usage)
-        module = args[0]
-        print(find(module))
+        filename = args[0]
+        print(find(filename))
     elif command == "run":
         if len(args) == 0:
             raise Exception(ERROR + usage)
         load_modules()
         p = subprocess.run(" ".join(args), shell=True)
         if p.returncode != 0:
             raise Exception("Exit code {}".format(p.returncode))
```

### Comparing `ampltools-0.5.5/ampltools/notebooks.py` & `ampltools-0.5.6/ampltools/notebooks.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.5/ampltools/tests/test_install.py` & `ampltools-0.5.6/ampltools/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.5/ampltools/tests/test_load.py` & `ampltools-0.5.6/ampltools/tests/test_load.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,22 +23,22 @@
 
         self.assertEqual(modules.installed(), [])
         modules.preload(verbose=verbose)
         self.assertEqual(initial_path, self.get_env_path_list())
 
         modules.install("highs", verbose=verbose)
         self.assertEqual(initial_path, self.get_env_path_list())
-        self.assertTrue(os.path.isdir(modules.find("highs")))
+        self.assertTrue(os.path.isfile(modules.find("highs")))
 
         modules.load("highs", verbose=verbose)
         self.assertNotEqual(initial_path, self.get_env_path_list())
         expected = modules.path().split(os.pathsep) + initial_path
         self.assertEqual(expected, self.get_env_path_list())
         self.assertEqual(len(initial_path) + 2, len(self.get_env_path_list()))
-        self.assertIn(modules.find("highs"), self.get_env_path_list())
+        self.assertIn(modules.path("highs", add_base=False), self.get_env_path_list())
 
         modules.install(["cbc"], verbose=verbose)
         modules.unload(["base", "highs"])
         modules.load(["cbc", "highs"], verbose=verbose)
         expected = modules.path().split(os.pathsep) + initial_path
         self.assertEqual(expected, self.get_env_path_list())
         self.assertEqual(len(initial_path) + 3, len(self.get_env_path_list()))
```

### Comparing `ampltools-0.5.5/ampltools/tests/test_preload.py` & `ampltools-0.5.6/ampltools/tests/test_preload.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.5/ampltools/tests/test_run.py` & `ampltools-0.5.6/ampltools/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.5/ampltools/utils.py` & `ampltools-0.5.6/ampltools/utils.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.5/ampltools.egg-info/PKG-INFO` & `ampltools-0.5.6/ampltools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ampltools
-Version: 0.5.5
+Version: 0.5.6
 Summary: AMPL Python Tools
 Home-page: http://ampl.com/
 Author: Filipe Brandão
 Author-email: fdabrandao@ampl.com
 License: BSD-3
 Download-URL: https://github.com/ampl/amplpy/tree/master/ampltools
 Description:
```

### Comparing `ampltools-0.5.5/ampltools.egg-info/SOURCES.txt` & `ampltools-0.5.6/ampltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.5/setup.py` & `ampltools-0.5.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         for (dirpath, dirnames, files) in os.walk(base_dir)
         for f in files
     ]
 
 
 setup(
     name="ampltools",
-    version="0.5.5",
+    version="0.5.6",
     description="AMPL Python Tools",
     long_description=__doc__,
     long_description_content_type="text/markdown",
     license="BSD-3",
     platforms="any",
     author="Filipe Brandão",
     author_email="fdabrandao@ampl.com",
```

