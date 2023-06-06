# Comparing `tmp/bpc-poseur-0.4.3.tar.gz` & `tmp/bpc-poseur-0.4.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bpc-poseur-0.4.3.tar", last modified: Mon Jun  5 09:57:34 2023, max compression
+gzip compressed data, was "bpc-poseur-0.4.3.post1.tar", last modified: Tue Jun  6 15:18:10 2023, max compression
```

## Comparing `bpc-poseur-0.4.3.tar` & `bpc-poseur-0.4.3.post1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-06-05 09:57:34.000000 bpc-poseur-0.4.3/
--rw-r--r--   0 jarryshaw   (501) staff       (20)     1099 2021-04-05 09:07:13.000000 bpc-poseur-0.4.3/LICENSE
--rw-r--r--   0 jarryshaw   (501) staff       (20)       32 2021-04-02 15:12:58.000000 bpc-poseur-0.4.3/MANIFEST.in
--rw-r--r--   0 jarryshaw   (501) staff       (20)     3254 2023-06-05 09:57:34.000000 bpc-poseur-0.4.3/PKG-INFO
--rw-r--r--   0 jarryshaw   (501) staff       (20)     2097 2021-04-05 09:07:13.000000 bpc-poseur-0.4.3/README.md
-drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-06-05 09:57:34.000000 bpc-poseur-0.4.3/bpc_poseur.egg-info/
--rw-r--r--   0 jarryshaw   (501) staff       (20)     3254 2023-06-05 09:57:34.000000 bpc-poseur-0.4.3/bpc_poseur.egg-info/PKG-INFO
--rw-r--r--   0 jarryshaw   (501) staff       (20)      337 2023-06-05 09:57:34.000000 bpc-poseur-0.4.3/bpc_poseur.egg-info/SOURCES.txt
--rw-r--r--   0 jarryshaw   (501) staff       (20)        1 2023-06-05 09:57:34.000000 bpc-poseur-0.4.3/bpc_poseur.egg-info/dependency_links.txt
--rw-r--r--   0 jarryshaw   (501) staff       (20)       39 2023-06-05 09:57:34.000000 bpc-poseur-0.4.3/bpc_poseur.egg-info/entry_points.txt
--rw-r--r--   0 jarryshaw   (501) staff       (20)      306 2023-06-05 09:57:34.000000 bpc-poseur-0.4.3/bpc_poseur.egg-info/requires.txt
--rw-r--r--   0 jarryshaw   (501) staff       (20)        7 2023-06-05 09:57:34.000000 bpc-poseur-0.4.3/bpc_poseur.egg-info/top_level.txt
-drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-06-05 09:57:34.000000 bpc-poseur-0.4.3/docs/
-drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-06-05 09:57:34.000000 bpc-poseur-0.4.3/docs/source/
--rw-r--r--   0 jarryshaw   (501) staff       (20)     3549 2021-04-05 09:07:13.000000 bpc-poseur-0.4.3/docs/source/conf.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)    54216 2021-03-26 16:19:44.000000 bpc-poseur-0.4.3/poseur.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)      233 2020-11-22 15:07:42.000000 bpc-poseur-0.4.3/pyproject.toml
-drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-06-05 09:57:34.000000 bpc-poseur-0.4.3/scripts/
--rw-r--r--   0 jarryshaw   (501) staff       (20)      497 2021-04-02 16:27:07.000000 bpc-poseur-0.4.3/scripts/find_version.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)      102 2023-06-05 09:57:34.000000 bpc-poseur-0.4.3/setup.cfg
--rw-r--r--   0 jarryshaw   (501) staff       (20)     2571 2023-06-05 09:56:56.000000 bpc-poseur-0.4.3/setup.py
-drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-06-05 09:57:34.000000 bpc-poseur-0.4.3/tests/
--rw-r--r--   0 jarryshaw   (501) staff       (20)     7706 2020-11-22 15:07:42.000000 bpc-poseur-0.4.3/tests/test.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-06-06 15:18:10.805270 bpc-poseur-0.4.3.post1/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1099 2021-04-05 09:07:13.000000 bpc-poseur-0.4.3.post1/LICENSE
+-rw-r--r--   0 jarryshaw   (501) staff       (20)       32 2021-04-02 15:12:58.000000 bpc-poseur-0.4.3.post1/MANIFEST.in
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3260 2023-06-06 15:18:10.805393 bpc-poseur-0.4.3.post1/PKG-INFO
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2097 2021-04-05 09:07:13.000000 bpc-poseur-0.4.3.post1/README.md
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-06-06 15:18:10.804044 bpc-poseur-0.4.3.post1/bpc_poseur.egg-info/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3260 2023-06-06 15:18:10.000000 bpc-poseur-0.4.3.post1/bpc_poseur.egg-info/PKG-INFO
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      337 2023-06-06 15:18:10.000000 bpc-poseur-0.4.3.post1/bpc_poseur.egg-info/SOURCES.txt
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        1 2023-06-06 15:18:10.000000 bpc-poseur-0.4.3.post1/bpc_poseur.egg-info/dependency_links.txt
+-rw-r--r--   0 jarryshaw   (501) staff       (20)       39 2023-06-06 15:18:10.000000 bpc-poseur-0.4.3.post1/bpc_poseur.egg-info/entry_points.txt
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      306 2023-06-06 15:18:10.000000 bpc-poseur-0.4.3.post1/bpc_poseur.egg-info/requires.txt
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        7 2023-06-06 15:18:10.000000 bpc-poseur-0.4.3.post1/bpc_poseur.egg-info/top_level.txt
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-06-06 15:18:10.801031 bpc-poseur-0.4.3.post1/docs/
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-06-06 15:18:10.804231 bpc-poseur-0.4.3.post1/docs/source/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3549 2021-04-05 09:07:13.000000 bpc-poseur-0.4.3.post1/docs/source/conf.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    54222 2023-06-06 15:16:25.000000 bpc-poseur-0.4.3.post1/poseur.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      233 2020-11-22 15:07:42.000000 bpc-poseur-0.4.3.post1/pyproject.toml
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-06-06 15:18:10.804648 bpc-poseur-0.4.3.post1/scripts/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      497 2021-04-02 16:27:07.000000 bpc-poseur-0.4.3.post1/scripts/find_version.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      102 2023-06-06 15:18:10.805963 bpc-poseur-0.4.3.post1/setup.cfg
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2571 2023-06-06 15:13:41.000000 bpc-poseur-0.4.3.post1/setup.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-06-06 15:18:10.804876 bpc-poseur-0.4.3.post1/tests/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     7706 2020-11-22 15:07:42.000000 bpc-poseur-0.4.3.post1/tests/test.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bpc-poseur-0.4.3/LICENSE` & `bpc-poseur-0.4.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `bpc-poseur-0.4.3/PKG-INFO` & `bpc-poseur-0.4.3.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpc-poseur
-Version: 0.4.3
+Version: 0.4.3.post1
 Summary: Back-port compiler for Python 3.8 positional-only parameter syntax.
 Home-page: https://github.com/pybpc/poseur
 Author: Jarry Shaw
 Author-email: jarryshaw@icloud.com
 License: MIT
 Keywords: positional-only parameters,back-port compiler
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bpc-poseur-0.4.3/README.md` & `bpc-poseur-0.4.3.post1/README.md`

 * *Files identical despite different names*

### Comparing `bpc-poseur-0.4.3/bpc_poseur.egg-info/PKG-INFO` & `bpc-poseur-0.4.3.post1/bpc_poseur.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpc-poseur
-Version: 0.4.3
+Version: 0.4.3.post1
 Summary: Back-port compiler for Python 3.8 positional-only parameter syntax.
 Home-page: https://github.com/pybpc/poseur
 Author: Jarry Shaw
 Author-email: jarryshaw@icloud.com
 License: MIT
 Keywords: positional-only parameters,back-port compiler
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bpc-poseur-0.4.3/docs/source/conf.py` & `bpc-poseur-0.4.3.post1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `bpc-poseur-0.4.3/poseur.py` & `bpc-poseur-0.4.3.post1/poseur.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                        recover_files)
 from bpc_utils.typing import Linesep
 from typing_extensions import Literal, final
 
 __all__ = ['main', 'poseur', 'convert', 'decorator']  # pylint: disable=undefined-all-variable
 
 # version string
-__version__ = '0.4.3'
+__version__ = '0.4.3.post1'
 
 ###############################################################################
 # Typings
 
 
 class PoseurConfig(Config):
     indentation = ''  # type: str
```

### Comparing `bpc-poseur-0.4.3/setup.py` & `bpc-poseur-0.4.3.post1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         'Topic :: Utilities',
         'Typing :: Typed',
     ],
     keywords=['positional-only parameters', 'back-port compiler'],
     py_modules=[module_name],
     python_requires='>=3.4',
     install_requires=[
-        'parso>=0.6.0',         # universal AST support
+        'parso~=0.6.0',         # universal AST support
         'tbtrim>=0.2.1',        # traceback trim support
         'bpc-f2format',         # bpc-f2format
         'bpc-utils~=0.10.0',    # utility library
         'typing;python_version<"3.5"',
         'typing_extensions',
     ],
     extras_require={
```

### Comparing `bpc-poseur-0.4.3/tests/test.py` & `bpc-poseur-0.4.3.post1/tests/test.py`

 * *Files identical despite different names*

