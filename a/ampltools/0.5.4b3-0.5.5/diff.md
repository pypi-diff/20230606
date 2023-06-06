# Comparing `tmp/ampltools-0.5.4b3.tar.gz` & `tmp/ampltools-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ampltools-0.5.4b3.tar", last modified: Tue May 30 13:33:44 2023, max compression
+gzip compressed data, was "ampltools-0.5.5.tar", last modified: Tue Jun  6 10:57:45 2023, max compression
```

## Comparing `ampltools-0.5.4b3.tar` & `ampltools-0.5.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-30 13:33:44.477687 ampltools-0.5.4b3/
--rw-r--r--   0 fdabrandao   (501) staff       (20)     2822 2023-05-03 11:08:48.000000 ampltools-0.5.4b3/CHANGELOG.md
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1522 2023-03-08 15:44:27.000000 ampltools-0.5.4b3/LICENSE
--rw-r--r--   0 fdabrandao   (501) staff       (20)       57 2023-03-08 15:44:27.000000 ampltools-0.5.4b3/MANIFEST.in
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1219 2023-05-30 13:33:44.477383 ampltools-0.5.4b3/PKG-INFO
--rw-r--r--   0 fdabrandao   (501) staff       (20)      446 2023-03-08 15:44:27.000000 ampltools-0.5.4b3/README.md
-drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-30 13:33:44.472104 ampltools-0.5.4b3/ampltools/
--rw-r--r--   0 fdabrandao   (501) staff       (20)      409 2023-05-30 13:33:41.000000 ampltools-0.5.4b3/ampltools/__init__.py
-drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-30 13:33:44.474796 ampltools-0.5.4b3/ampltools/modules/
--rw-r--r--   0 fdabrandao   (501) staff       (20)      443 2023-05-30 13:33:41.000000 ampltools-0.5.4b3/ampltools/modules/__init__.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)       93 2023-03-08 15:44:27.000000 ampltools-0.5.4b3/ampltools/modules/__main__.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)    12683 2023-05-03 11:08:48.000000 ampltools-0.5.4b3/ampltools/modules/amplpypi.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     3723 2023-03-09 15:01:44.000000 ampltools-0.5.4b3/ampltools/modules/commands.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     5838 2023-05-30 13:33:35.000000 ampltools-0.5.4b3/ampltools/notebooks.py
-drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-30 13:33:44.476912 ampltools-0.5.4b3/ampltools/tests/
--rw-r--r--   0 fdabrandao   (501) staff       (20)      433 2023-03-08 15:44:27.000000 ampltools-0.5.4b3/ampltools/tests/TestBase.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)       24 2023-03-08 15:44:27.000000 ampltools-0.5.4b3/ampltools/tests/__init__.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)      286 2023-03-08 15:44:27.000000 ampltools-0.5.4b3/ampltools/tests/__main__.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     3566 2023-03-08 15:44:27.000000 ampltools-0.5.4b3/ampltools/tests/test_install.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1951 2023-03-08 15:44:27.000000 ampltools-0.5.4b3/ampltools/tests/test_load.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     2411 2023-03-13 18:25:11.000000 ampltools-0.5.4b3/ampltools/tests/test_preload.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1751 2023-03-08 15:44:27.000000 ampltools-0.5.4b3/ampltools/tests/test_run.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     3228 2023-03-09 15:37:57.000000 ampltools-0.5.4b3/ampltools/utils.py
-drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-30 13:33:44.473664 ampltools-0.5.4b3/ampltools.egg-info/
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1219 2023-05-30 13:33:44.000000 ampltools-0.5.4b3/ampltools.egg-info/PKG-INFO
--rw-r--r--   0 fdabrandao   (501) staff       (20)      621 2023-05-30 13:33:44.000000 ampltools-0.5.4b3/ampltools.egg-info/SOURCES.txt
--rw-r--r--   0 fdabrandao   (501) staff       (20)        1 2023-05-30 13:33:44.000000 ampltools-0.5.4b3/ampltools.egg-info/dependency_links.txt
--rw-r--r--   0 fdabrandao   (501) staff       (20)        9 2023-05-30 13:33:44.000000 ampltools-0.5.4b3/ampltools.egg-info/requires.txt
--rw-r--r--   0 fdabrandao   (501) staff       (20)       10 2023-05-30 13:33:44.000000 ampltools-0.5.4b3/ampltools.egg-info/top_level.txt
--rw-r--r--   0 fdabrandao   (501) staff       (20)        8 2023-03-08 15:44:27.000000 ampltools-0.5.4b3/requirements.txt
--rw-r--r--   0 fdabrandao   (501) staff       (20)       38 2023-05-30 13:33:44.477766 ampltools-0.5.4b3/setup.cfg
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1717 2023-05-30 13:33:41.000000 ampltools-0.5.4b3/setup.py
+drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-06-06 10:57:45.256783 ampltools-0.5.5/
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     2987 2023-06-06 10:15:43.000000 ampltools-0.5.5/CHANGELOG.md
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     1522 2023-03-08 15:44:27.000000 ampltools-0.5.5/LICENSE
+-rw-r--r--   0 fdabrandao   (501) staff       (20)       57 2023-03-08 15:44:27.000000 ampltools-0.5.5/MANIFEST.in
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     1280 2023-06-06 10:57:45.256493 ampltools-0.5.5/PKG-INFO
+-rw-r--r--   0 fdabrandao   (501) staff       (20)      446 2023-03-08 15:44:27.000000 ampltools-0.5.5/README.md
+drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-06-06 10:57:45.245542 ampltools-0.5.5/ampltools/
+-rw-r--r--   0 fdabrandao   (501) staff       (20)      407 2023-06-06 10:18:36.000000 ampltools-0.5.5/ampltools/__init__.py
+drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-06-06 10:57:45.251606 ampltools-0.5.5/ampltools/modules/
+-rw-r--r--   0 fdabrandao   (501) staff       (20)      451 2023-06-06 10:19:22.000000 ampltools-0.5.5/ampltools/modules/__init__.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)       93 2023-03-08 15:44:27.000000 ampltools-0.5.5/ampltools/modules/__main__.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)    13054 2023-06-06 10:38:28.000000 ampltools-0.5.5/ampltools/modules/amplpypi.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     4027 2023-06-06 10:46:36.000000 ampltools-0.5.5/ampltools/modules/commands.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     5838 2023-06-06 10:17:59.000000 ampltools-0.5.5/ampltools/notebooks.py
+drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-06-06 10:57:45.255835 ampltools-0.5.5/ampltools/tests/
+-rw-r--r--   0 fdabrandao   (501) staff       (20)      433 2023-03-08 15:44:27.000000 ampltools-0.5.5/ampltools/tests/TestBase.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)       24 2023-03-08 15:44:27.000000 ampltools-0.5.5/ampltools/tests/__init__.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)      286 2023-03-08 15:44:27.000000 ampltools-0.5.5/ampltools/tests/__main__.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     3566 2023-03-08 15:44:27.000000 ampltools-0.5.5/ampltools/tests/test_install.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     2084 2023-06-06 10:42:43.000000 ampltools-0.5.5/ampltools/tests/test_load.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     2411 2023-03-13 18:25:11.000000 ampltools-0.5.5/ampltools/tests/test_preload.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     1751 2023-03-08 15:44:27.000000 ampltools-0.5.5/ampltools/tests/test_run.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     3228 2023-03-09 15:37:57.000000 ampltools-0.5.5/ampltools/utils.py
+drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-06-06 10:57:45.248782 ampltools-0.5.5/ampltools.egg-info/
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     1280 2023-06-06 10:57:45.000000 ampltools-0.5.5/ampltools.egg-info/PKG-INFO
+-rw-r--r--   0 fdabrandao   (501) staff       (20)      621 2023-06-06 10:57:45.000000 ampltools-0.5.5/ampltools.egg-info/SOURCES.txt
+-rw-r--r--   0 fdabrandao   (501) staff       (20)        1 2023-06-06 10:57:45.000000 ampltools-0.5.5/ampltools.egg-info/dependency_links.txt
+-rw-r--r--   0 fdabrandao   (501) staff       (20)        9 2023-06-06 10:57:45.000000 ampltools-0.5.5/ampltools.egg-info/requires.txt
+-rw-r--r--   0 fdabrandao   (501) staff       (20)       10 2023-06-06 10:57:45.000000 ampltools-0.5.5/ampltools.egg-info/top_level.txt
+-rw-r--r--   0 fdabrandao   (501) staff       (20)        8 2023-03-08 15:44:27.000000 ampltools-0.5.5/requirements.txt
+-rw-r--r--   0 fdabrandao   (501) staff       (20)       38 2023-06-06 10:57:45.256881 ampltools-0.5.5/setup.cfg
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     1715 2023-06-06 10:18:36.000000 ampltools-0.5.5/setup.py
```

### Comparing `ampltools-0.5.4b3/CHANGELOG.md` & `ampltools-0.5.5/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Change Log
 All notable changes to this project will be documented in this file.
 This project adheres to [Semantic Versioning](http://semver.org/).
 
+## 0.5.5 - 2023-06-06
+- Add modules.find.
+
+## 0.5.4 - 2023-05-30
+- ampl_notebook: Drop g/globals_ argument.
+- ampl_notebook: Remove button to use existing license.
+
 ## 0.5.3 - 2023-05-03
 - Set ampl_libpath when loading modules.
 
 ## 0.5.2 - 2023-04-05
 - Add message to append to AMPLException messages.
 
 ## 0.5.1 - 2023-03-14
```

### Comparing `ampltools-0.5.4b3/LICENSE` & `ampltools-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.4b3/PKG-INFO` & `ampltools-0.5.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 Metadata-Version: 2.1
 Name: ampltools
-Version: 0.5.4b3
+Version: 0.5.5
 Summary: AMPL Python Tools
 Home-page: http://ampl.com/
-Download-URL: https://github.com/ampl/amplpy/tree/master/ampltools
 Author: Filipe Brandão
 Author-email: fdabrandao@ampl.com
 License: BSD-3
+Download-URL: https://github.com/ampl/amplpy/tree/master/ampltools
+Description: 
+        # AMPL Python Tools
+        
+        This package includes tools to use with [AMPL](https://ampl.com) and [amplpy](https://amplpy.readthedocs.io).
+        
+        ## Links
+        
+        * GitHub Repository: https://github.com/ampl/amplpy/
+        * PyPI Repository: https://pypi.python.org/pypi/ampltools
+        
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -19,18 +29,7 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# AMPL Python Tools
-
-This package includes tools to use with [AMPL](https://ampl.com) and [amplpy](https://amplpy.readthedocs.io).
-
-## Links
-
-* GitHub Repository: https://github.com/ampl/amplpy/
-* PyPI Repository: https://pypi.python.org/pypi/ampltools
```

### Comparing `ampltools-0.5.4b3/ampltools/modules/amplpypi.py` & `ampltools-0.5.5/ampltools/modules/amplpypi.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 def installed_modules():
     from pkgutil import iter_modules
 
     prefix = "ampl_module_"
     installed = []
-    for (_, name, _) in iter_modules():
+    for _, name, _ in iter_modules():
         norm = name.replace("-", "_")
         if norm.startswith(prefix):
             installed.append(norm.replace(prefix, ""))
     return installed
 
 
 def available_modules():
@@ -382,14 +382,27 @@
     Args:
         modules: list of modules to be included.
     """
     modules = _sort_modules_for_loading(modules)
     return os.pathsep.join(_locate_modules(modules, verbose=False))
 
 
+def find(module):
+    """
+    Return PATH for an AMPL module.
+    Args:
+        module: name of the module to locate.
+    """
+    modules = _sort_modules_for_loading(module, add_base=False)
+    paths = _locate_modules(modules[:1], verbose=False)
+    if paths == []:
+        raise ModuleNotFoundError("Could not find AMPL module '{}'.".format(module))
+    return paths[0]
+
+
 def activate_license(uuid, verbose=False):
     """
     Activate an AMPL license using the UUID.
     Args:
         uuid: license uuid.
         verbose: show verbose output if True.
     """
```

### Comparing `ampltools-0.5.4b3/ampltools/modules/commands.py` & `ampltools-0.5.5/ampltools/modules/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
     install_modules,
     uninstall_modules,
     installed_modules,
     available_modules,
     generate_requirements,
     load_modules,
     path,
+    find,
     activate_license,
 )
 import subprocess
 import sys
 
 ERROR = """
 Invalid command.
@@ -37,14 +38,19 @@
     $ python -m $PACKAGE.modules available
 
 - Value to append to the environment variable PATH to access modules
     $ python -m $PACKAGE.modules path
     Example:
         $ export PATH=$PATH:`python -m amplpy.modules path`
 
+- Find the path to a specific module
+    $ python -m $PACKAGE.modules find <name>
+    Example:
+        $ python -m amplpy.modules find gurobi
+
 - Generate requirements.txt for the modules currently installed
     $ python -m $PACKAGE.modules requirements
 
 - Run command in the same environment as the modules:
     $ python -m $PACKAGE.modules run <command>
     Example:
         $ python -m $PACKAGE.modules run ampl -v
@@ -91,14 +97,19 @@
             raise Exception("Could not find any modules for download.")
         print("You can install any of the following modules:")
         for name in sorted(set(names)):
             print("\t" + name)
     elif command == "path":
         modules = [m for m in args if not m.startswith("-")]
         print(path(modules))
+    elif command == "find":
+        if len(args) != 1:
+            raise Exception(ERROR + usage)
+        module = args[0]
+        print(find(module))
     elif command == "run":
         if len(args) == 0:
             raise Exception(ERROR + usage)
         load_modules()
         p = subprocess.run(" ".join(args), shell=True)
         if p.returncode != 0:
             raise Exception("Exit code {}".format(p.returncode))
```

### Comparing `ampltools-0.5.4b3/ampltools/notebooks.py` & `ampltools-0.5.5/ampltools/notebooks.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.4b3/ampltools/tests/test_install.py` & `ampltools-0.5.5/ampltools/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.4b3/ampltools/tests/test_load.py` & `ampltools-0.5.5/ampltools/tests/test_load.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,20 +23,22 @@
 
         self.assertEqual(modules.installed(), [])
         modules.preload(verbose=verbose)
         self.assertEqual(initial_path, self.get_env_path_list())
 
         modules.install("highs", verbose=verbose)
         self.assertEqual(initial_path, self.get_env_path_list())
+        self.assertTrue(os.path.isdir(modules.find("highs")))
 
         modules.load("highs", verbose=verbose)
         self.assertNotEqual(initial_path, self.get_env_path_list())
         expected = modules.path().split(os.pathsep) + initial_path
         self.assertEqual(expected, self.get_env_path_list())
         self.assertEqual(len(initial_path) + 2, len(self.get_env_path_list()))
+        self.assertIn(modules.find("highs"), self.get_env_path_list())
 
         modules.install(["cbc"], verbose=verbose)
         modules.unload(["base", "highs"])
         modules.load(["cbc", "highs"], verbose=verbose)
         expected = modules.path().split(os.pathsep) + initial_path
         self.assertEqual(expected, self.get_env_path_list())
         self.assertEqual(len(initial_path) + 3, len(self.get_env_path_list()))
```

### Comparing `ampltools-0.5.4b3/ampltools/tests/test_preload.py` & `ampltools-0.5.5/ampltools/tests/test_preload.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.4b3/ampltools/tests/test_run.py` & `ampltools-0.5.5/ampltools/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.4b3/ampltools/utils.py` & `ampltools-0.5.5/ampltools/utils.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.4b3/ampltools.egg-info/PKG-INFO` & `ampltools-0.5.5/ampltools.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 Metadata-Version: 2.1
 Name: ampltools
-Version: 0.5.4b3
+Version: 0.5.5
 Summary: AMPL Python Tools
 Home-page: http://ampl.com/
-Download-URL: https://github.com/ampl/amplpy/tree/master/ampltools
 Author: Filipe Brandão
 Author-email: fdabrandao@ampl.com
 License: BSD-3
+Download-URL: https://github.com/ampl/amplpy/tree/master/ampltools
+Description: 
+        # AMPL Python Tools
+        
+        This package includes tools to use with [AMPL](https://ampl.com) and [amplpy](https://amplpy.readthedocs.io).
+        
+        ## Links
+        
+        * GitHub Repository: https://github.com/ampl/amplpy/
+        * PyPI Repository: https://pypi.python.org/pypi/ampltools
+        
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -19,18 +29,7 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# AMPL Python Tools
-
-This package includes tools to use with [AMPL](https://ampl.com) and [amplpy](https://amplpy.readthedocs.io).
-
-## Links
-
-* GitHub Repository: https://github.com/ampl/amplpy/
-* PyPI Repository: https://pypi.python.org/pypi/ampltools
```

### Comparing `ampltools-0.5.4b3/ampltools.egg-info/SOURCES.txt` & `ampltools-0.5.5/ampltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.4b3/setup.py` & `ampltools-0.5.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         for (dirpath, dirnames, files) in os.walk(base_dir)
         for f in files
     ]
 
 
 setup(
     name="ampltools",
-    version="0.5.4b3",
+    version="0.5.5",
     description="AMPL Python Tools",
     long_description=__doc__,
     long_description_content_type="text/markdown",
     license="BSD-3",
     platforms="any",
     author="Filipe Brandão",
     author_email="fdabrandao@ampl.com",
```

