# Comparing `tmp/pylena-0.1.1.tar.gz` & `tmp/pylena-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylena-0.1.1.tar", last modified: Mon Jul  4 17:29:32 2022, max compression
+gzip compressed data, was "pylena-0.1.2.tar", last modified: Tue Jun  6 09:29:44 2023, max compression
```

## Comparing `pylena-0.1.1.tar` & `pylena-0.1.2.tar`

### file list

```diff
@@ -1,48 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-04 17:29:32.861307 pylena-0.1.1/
--rw-rw-rw-   0 root         (0) root         (0)      637 2022-06-24 09:05:01.000000 pylena-0.1.1/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)    16725 2022-06-23 09:41:09.000000 pylena-0.1.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      209 2022-06-23 09:41:09.000000 pylena-0.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    22729 2022-07-04 17:29:32.861307 pylena-0.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1921 2022-06-23 09:41:09.000000 pylena-0.1.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1906 2022-06-23 11:34:18.000000 pylena-0.1.1/conanfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-04 17:29:32.821307 pylena-0.1.1/pylena/
--rw-rw-rw-   0 root         (0) root         (0)      123 2022-06-23 09:41:09.000000 pylena-0.1.1/pylena/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)      172 2022-07-01 11:22:59.000000 pylena-0.1.1/pylena/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-07-04 14:58:33.000000 pylena-0.1.1/pylena/_version.py
--rw-rw-rw-   0 root         (0) root         (0)      239 2022-06-23 09:41:09.000000 pylena-0.1.1/pylena/module.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-04 17:29:32.857307 pylena-0.1.1/pylena/morpho/
--rw-rw-rw-   0 root         (0) root         (0)       94 2022-06-29 12:40:29.000000 pylena-0.1.1/pylena/morpho/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)      384 2022-07-01 11:22:59.000000 pylena-0.1.1/pylena/morpho/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8607 2022-07-04 12:19:01.000000 pylena-0.1.1/pylena/morpho/component_tree.py
--rw-rw-rw-   0 root         (0) root         (0)     2728 2022-06-24 14:20:35.000000 pylena-0.1.1/pylena/morpho/maxtree.cpp
--rw-rw-rw-   0 root         (0) root         (0)      137 2022-06-24 14:20:35.000000 pylena-0.1.1/pylena/morpho/maxtree.hpp
--rw-rw-rw-   0 root         (0) root         (0)      391 2022-06-29 12:40:29.000000 pylena-0.1.1/pylena/morpho/morpho.cpp
--rw-rw-rw-   0 root         (0) root         (0)      112 2022-06-23 09:41:09.000000 pylena-0.1.1/pylena/morpho/morpho.hpp
--rw-rw-rw-   0 root         (0) root         (0)     3958 2022-06-23 09:41:09.000000 pylena-0.1.1/pylena/morpho/se.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2626 2022-06-24 14:20:35.000000 pylena-0.1.1/pylena/morpho/se.hpp
--rw-rw-rw-   0 root         (0) root         (0)     3003 2022-07-01 11:22:59.000000 pylena-0.1.1/pylena/morpho/se.py
--rw-rw-rw-   0 root         (0) root         (0)     3251 2022-06-29 12:40:29.000000 pylena-0.1.1/pylena/morpho/soperations.cpp
--rw-rw-rw-   0 root         (0) root         (0)      162 2022-06-29 12:40:29.000000 pylena-0.1.1/pylena/morpho/soperations.hpp
--rw-rw-rw-   0 root         (0) root         (0)     6567 2022-07-01 14:15:02.000000 pylena-0.1.1/pylena/morpho/soperations.py
--rw-rw-rw-   0 root         (0) root         (0)     1827 2022-06-29 12:40:29.000000 pylena-0.1.1/pylena/morpho/watershed.cpp
--rw-rw-rw-   0 root         (0) root         (0)      114 2022-06-29 12:40:29.000000 pylena-0.1.1/pylena/morpho/watershed.hpp
--rw-rw-rw-   0 root         (0) root         (0)     1965 2022-07-01 14:15:02.000000 pylena-0.1.1/pylena/morpho/watershed.py
--rw-rw-rw-   0 root         (0) root         (0)     3905 2022-07-01 13:20:59.000000 pylena-0.1.1/pylena/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-04 17:29:32.821307 pylena-0.1.1/pylena.egg-info/
--rw-r--r--   0 root         (0) root         (0)    22729 2022-07-04 17:29:32.000000 pylena-0.1.1/pylena.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      915 2022-07-04 17:29:32.000000 pylena-0.1.1/pylena.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-04 17:29:32.000000 pylena-0.1.1/pylena.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      174 2022-07-04 17:29:32.000000 pylena-0.1.1/pylena.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2022-07-04 17:29:32.000000 pylena-0.1.1/pylena.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-04 17:29:32.857307 pylena-0.1.1/pylene-numpy/
--rw-rw-rw-   0 root         (0) root         (0)      728 2022-06-24 09:05:01.000000 pylena-0.1.1/pylene-numpy/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-04 17:29:32.817307 pylena-0.1.1/pylene-numpy/include/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-04 17:29:32.857307 pylena-0.1.1/pylene-numpy/include/pln/
--rw-rw-rw-   0 root         (0) root         (0)     1479 2022-06-23 09:41:09.000000 pylena-0.1.1/pylene-numpy/include/pln/image_cast.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-04 17:29:32.861307 pylena-0.1.1/pylene-numpy/src/
--rw-rw-rw-   0 root         (0) root         (0)     3818 2022-06-23 09:41:09.000000 pylena-0.1.1/pylene-numpy/src/image_cast.cpp
--rw-rw-rw-   0 root         (0) root         (0)     3196 2022-06-23 09:41:09.000000 pylena-0.1.1/pylene-numpy/src/numpy_format.cpp
--rw-rw-rw-   0 root         (0) root         (0)      609 2022-06-23 09:41:09.000000 pylena-0.1.1/pylene-numpy/src/numpy_format.hpp
--rw-rw-rw-   0 root         (0) root         (0)     1555 2022-07-01 14:15:02.000000 pylena-0.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-04 17:29:32.861307 pylena-0.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     5724 2022-06-24 11:53:01.000000 pylena-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:44.769305 pylena-0.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)      637 2023-06-06 09:28:15.000000 pylena-0.1.2/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)    16725 2023-06-06 09:28:15.000000 pylena-0.1.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-06-06 09:28:15.000000 pylena-0.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    22683 2023-06-06 09:29:44.769305 pylena-0.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2023-06-06 09:28:15.000000 pylena-0.1.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1952 2023-06-06 09:28:15.000000 pylena-0.1.2/conanfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:44.749305 pylena-0.1.2/pylena/
+-rw-rw-rw-   0 root         (0) root         (0)      223 2023-06-06 09:28:15.000000 pylena-0.1.2/pylena/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)      213 2023-06-06 09:28:15.000000 pylena-0.1.2/pylena/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-06 09:28:15.000000 pylena-0.1.2/pylena/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-06-06 09:28:15.000000 pylena-0.1.2/pylena/module.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:44.761305 pylena-0.1.2/pylena/morpho/
+-rw-rw-rw-   0 root         (0) root         (0)       94 2023-06-06 09:28:15.000000 pylena-0.1.2/pylena/morpho/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)      384 2023-06-06 09:28:15.000000 pylena-0.1.2/pylena/morpho/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8607 2023-06-06 09:28:15.000000 pylena-0.1.2/pylena/morpho/component_tree.py
+-rw-rw-rw-   0 root         (0) root         (0)     2723 2023-06-06 09:28:15.000000 pylena-0.1.2/pylena/morpho/maxtree.cpp
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-06-06 09:28:15.000000 pylena-0.1.2/pylena/morpho/maxtree.hpp
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-06-06 09:28:15.000000 pylena-0.1.2/pylena/morpho/morpho.cpp
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-06 09:28:15.000000 pylena-0.1.2/pylena/morpho/morpho.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     3958 2023-06-06 09:28:15.000000 pylena-0.1.2/pylena/morpho/se.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     2626 2023-06-06 09:28:15.000000 pylena-0.1.2/pylena/morpho/se.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     3003 2023-06-06 09:28:15.000000 pylena-0.1.2/pylena/morpho/se.py
+-rw-rw-rw-   0 root         (0) root         (0)     3246 2023-06-06 09:28:15.000000 pylena-0.1.2/pylena/morpho/soperations.cpp
+-rw-rw-rw-   0 root         (0) root         (0)      162 2023-06-06 09:28:15.000000 pylena-0.1.2/pylena/morpho/soperations.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     6567 2023-06-06 09:28:15.000000 pylena-0.1.2/pylena/morpho/soperations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2023-06-06 09:28:15.000000 pylena-0.1.2/pylena/morpho/watershed.cpp
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-06-06 09:28:15.000000 pylena-0.1.2/pylena/morpho/watershed.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     1965 2023-06-06 09:28:15.000000 pylena-0.1.2/pylena/morpho/watershed.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:44.765305 pylena-0.1.2/pylena/scribo/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-06 09:28:15.000000 pylena-0.1.2/pylena/scribo/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)      515 2023-06-06 09:28:15.000000 pylena-0.1.2/pylena/scribo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15018 2023-06-06 09:28:15.000000 pylena-0.1.2/pylena/scribo/line_detector.cpp
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-06-06 09:28:15.000000 pylena-0.1.2/pylena/scribo/line_detector.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     9055 2023-06-06 09:28:15.000000 pylena-0.1.2/pylena/scribo/line_detector.py
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-06-06 09:28:15.000000 pylena-0.1.2/pylena/scribo/scribo.cpp
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-06 09:28:15.000000 pylena-0.1.2/pylena/scribo/scribo.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     3905 2023-06-06 09:28:15.000000 pylena-0.1.2/pylena/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:44.753305 pylena-0.1.2/pylena.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    22683 2023-06-06 09:29:44.000000 pylena-0.1.2/pylena.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1157 2023-06-06 09:29:44.000000 pylena-0.1.2/pylena.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 09:29:44.000000 pylena-0.1.2/pylena.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      183 2023-06-06 09:29:44.000000 pylena-0.1.2/pylena.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-06 09:29:44.000000 pylena-0.1.2/pylena.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:44.765305 pylena-0.1.2/pylene-numpy/
+-rw-rw-rw-   0 root         (0) root         (0)      727 2023-06-06 09:28:15.000000 pylena-0.1.2/pylene-numpy/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:44.745305 pylena-0.1.2/pylene-numpy/include/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:44.765305 pylena-0.1.2/pylene-numpy/include/pln/
+-rw-rw-rw-   0 root         (0) root         (0)     1479 2023-06-06 09:28:15.000000 pylena-0.1.2/pylene-numpy/include/pln/image_cast.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:44.769305 pylena-0.1.2/pylene-numpy/src/
+-rw-rw-rw-   0 root         (0) root         (0)     3813 2023-06-06 09:28:15.000000 pylena-0.1.2/pylene-numpy/src/image_cast.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     3196 2023-06-06 09:28:15.000000 pylena-0.1.2/pylene-numpy/src/numpy_format.cpp
+-rw-rw-rw-   0 root         (0) root         (0)      609 2023-06-06 09:28:15.000000 pylena-0.1.2/pylene-numpy/src/numpy_format.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     1539 2023-06-06 09:28:15.000000 pylena-0.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 09:29:44.769305 pylena-0.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     6326 2023-06-06 09:28:15.000000 pylena-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:44.769305 pylena-0.1.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1543 2023-06-06 09:28:15.000000 pylena-0.1.2/tests/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-06-06 09:28:15.000000 pylena-0.1.2/tests/test_version.py
```

### Comparing `pylena-0.1.1/CMakeLists.txt` & `pylena-0.1.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pylena-0.1.1/LICENSE` & `pylena-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pylena-0.1.1/PKG-INFO` & `pylena-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pylena
-Version: 0.1.1
+Version: 0.1.2
 Summary: Image processing library
-Author-email: "EPITA Research and Development Laboratory (LRDE)" <baptiste.esteban@lrde.epita.fr>
+Author-email: "EPITA Research Laboratory (LRE)" <baptiste.esteban@epita.fr>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
         
         1.1. "Contributor"
@@ -373,19 +373,19 @@
         
         Exhibit B - "Incompatible With Secondary Licenses" Notice
         ---------------------------------------------------------
         
           This Source Code Form is "Incompatible With Secondary Licenses", as
           defined by the Mozilla Public License, v. 2.0.
         
-Project-URL: homepage, http://olena.pages.lrde.epita.fr/pylena/
-Project-URL: documentation, http://olena.pages.lrde.epita.fr/pylena/
-Project-URL: repository, https://gitlab.lrde.epita.fr/olena/pylena
-Project-URL: Bug Tracker, https://gitlab.lrde.epita.fr/olena/pylena/-/issues
-Project-URL: changelog, http://olena.pages.lrde.epita.fr/pylena/changelog.html
+Project-URL: homepage, http://olena.pages.lre.epita.fr/pylena/
+Project-URL: documentation, http://olena.pages.lre.epita.fr/pylena/
+Project-URL: repository, https://gitlab.lre.epita.fr/olena/pylena
+Project-URL: Bug Tracker, https://gitlab.lre.epita.fr/olena/pylena/-/issues
+Project-URL: changelog, http://olena.pages.lre.epita.fr/pylena/changelog.html
 Platform: linux
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -394,20 +394,20 @@
 Provides-Extra: packaging
 Provides-Extra: doc
 Provides-Extra: tests
 License-File: LICENSE
 
 # Pylena image processing library
 
-[![image alt pipeline](https://gitlab.lrde.epita.fr/olena/pylena/badges/master/pipeline.svg)](https://gitlab.lrde.epita.fr/olena/pylena/-/commits/master)
-[![image alt python coverage](https://gitlab.lrde.epita.fr/olena/pylena/badges/master/coverage.svg?job=python_coverage&key_text=Python+Coverage&key_width=100)](https://gitlab.lrde.epita.fr/olena/pylena/-/commits/master)
-[![image alt cpp coverage](https://gitlab.lrde.epita.fr/olena/pylena/badges/master/coverage.svg?job=cpp_coverage&key_text=C%2B%2B+Coverage&key_width=100)](https://gitlab.lrde.epita.fr/olena/pylena/-/commits/master)
+[![image alt pipeline](https://gitlab.lre.epita.fr/olena/pylena/badges/master/pipeline.svg)](https://gitlab.lre.epita.fr/olena/pylena/-/commits/master)
+[![image alt python coverage](https://gitlab.lre.epita.fr/olena/pylena/badges/master/coverage.svg?job=python_coverage&key_text=Python+Coverage&key_width=100)](https://gitlab.lre.epita.fr/olena/pylena/-/commits/master)
+[![image alt cpp coverage](https://gitlab.lre.epita.fr/olena/pylena/badges/master/coverage.svg?job=cpp_coverage&key_text=C%2B%2B+Coverage&key_width=100)](https://gitlab.lre.epita.fr/olena/pylena/-/commits/master)
 
 Pylena is the Python interface to the modern C++ image processing library
-[Pylene](https://gitlab.lrde.epita.fr/olena/pylene). Its aim is to fill the three following requirements:
+[Pylene](https://gitlab.lre.epita.fr/olena/pylene). Its aim is to fill the three following requirements:
 * Interactivity
 * Genericity
 * Efficiency
 
 Many image processing libraries succeed to fill these requirements but they are
 still limited by the static nature of the C++ language, where the genericity,
 based on *templates*, is resolved at compile time. Thus, the goal of this library is to tackle this problem.
@@ -428,18 +428,18 @@
 
 ```
 $ pip install pylena
 ```
 
 ## Documentation
 
-The documentation is available [here](http://olena.pages.lrde.epita.fr/pylena/).
+The documentation is available [here](http://olena.pages.lre.epita.fr/pylena/).
 
 ## Contributing
 
 If you find any bug or have any suggestions, feel free to create a new issue
-[here](https://gitlab.lrde.epita.fr/olena/pylena/-/issues) or send an email to
-[baptiste.esteban@lrde.epita.fr](mailto:baptiste.esteban@lrde.epita.fr).
+[here](https://gitlab.lre.epita.fr/olena/pylena/-/issues) or send an email to
+[baptiste.esteban@epita.fr](mailto:baptiste.esteban@epita.fr).
 
 ## Licence
 
 [Mozilla Public License Version 2.0](https://www.mozilla.org/en-US/MPL/2.0/)
```

### Comparing `pylena-0.1.1/README.md` & `pylena-0.1.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Pylena image processing library
 
-[![image alt pipeline](https://gitlab.lrde.epita.fr/olena/pylena/badges/master/pipeline.svg)](https://gitlab.lrde.epita.fr/olena/pylena/-/commits/master)
-[![image alt python coverage](https://gitlab.lrde.epita.fr/olena/pylena/badges/master/coverage.svg?job=python_coverage&key_text=Python+Coverage&key_width=100)](https://gitlab.lrde.epita.fr/olena/pylena/-/commits/master)
-[![image alt cpp coverage](https://gitlab.lrde.epita.fr/olena/pylena/badges/master/coverage.svg?job=cpp_coverage&key_text=C%2B%2B+Coverage&key_width=100)](https://gitlab.lrde.epita.fr/olena/pylena/-/commits/master)
+[![image alt pipeline](https://gitlab.lre.epita.fr/olena/pylena/badges/master/pipeline.svg)](https://gitlab.lre.epita.fr/olena/pylena/-/commits/master)
+[![image alt python coverage](https://gitlab.lre.epita.fr/olena/pylena/badges/master/coverage.svg?job=python_coverage&key_text=Python+Coverage&key_width=100)](https://gitlab.lre.epita.fr/olena/pylena/-/commits/master)
+[![image alt cpp coverage](https://gitlab.lre.epita.fr/olena/pylena/badges/master/coverage.svg?job=cpp_coverage&key_text=C%2B%2B+Coverage&key_width=100)](https://gitlab.lre.epita.fr/olena/pylena/-/commits/master)
 
 Pylena is the Python interface to the modern C++ image processing library
-[Pylene](https://gitlab.lrde.epita.fr/olena/pylene). Its aim is to fill the three following requirements:
+[Pylene](https://gitlab.lre.epita.fr/olena/pylene). Its aim is to fill the three following requirements:
 * Interactivity
 * Genericity
 * Efficiency
 
 Many image processing libraries succeed to fill these requirements but they are
 still limited by the static nature of the C++ language, where the genericity,
 based on *templates*, is resolved at compile time. Thus, the goal of this library is to tackle this problem.
@@ -30,18 +30,18 @@
 
 ```
 $ pip install pylena
 ```
 
 ## Documentation
 
-The documentation is available [here](http://olena.pages.lrde.epita.fr/pylena/).
+The documentation is available [here](http://olena.pages.lre.epita.fr/pylena/).
 
 ## Contributing
 
 If you find any bug or have any suggestions, feel free to create a new issue
-[here](https://gitlab.lrde.epita.fr/olena/pylena/-/issues) or send an email to
-[baptiste.esteban@lrde.epita.fr](mailto:baptiste.esteban@lrde.epita.fr).
+[here](https://gitlab.lre.epita.fr/olena/pylena/-/issues) or send an email to
+[baptiste.esteban@epita.fr](mailto:baptiste.esteban@epita.fr).
 
 ## Licence
 
 [Mozilla Public License Version 2.0](https://www.mozilla.org/en-US/MPL/2.0/)
```

### Comparing `pylena-0.1.1/pylena/morpho/component_tree.py` & `pylena-0.1.2/pylena/morpho/component_tree.py`

 * *Files identical despite different names*

### Comparing `pylena-0.1.1/pylena/morpho/maxtree.cpp` & `pylena-0.1.2/pylena/morpho/maxtree.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #include <mln/morpho/maxtree.hpp>
 #include <mln/morpho/tos.hpp>
 #include <mln/core/image/ndimage.hpp>
 #include <mln/core/neighborhood/c4.hpp>
 #include <mln/core/neighborhood/c8.hpp>
 
-#include <pln/core/image_cast.hpp>
+#include <pln/image_cast.hpp>
 #include <pybind11/pybind11.h>
 #include <pybind11/numpy.h>
 #include <iostream>
 
 namespace py = pybind11;
 
 namespace pln::morpho
```

### Comparing `pylena-0.1.1/pylena/morpho/se.cpp` & `pylena-0.1.2/pylena/morpho/se.cpp`

 * *Files identical despite different names*

### Comparing `pylena-0.1.1/pylena/morpho/se.hpp` & `pylena-0.1.2/pylena/morpho/se.hpp`

 * *Files identical despite different names*

### Comparing `pylena-0.1.1/pylena/morpho/se.py` & `pylena-0.1.2/pylena/morpho/se.py`

 * *Files identical despite different names*

### Comparing `pylena-0.1.1/pylena/morpho/soperations.cpp` & `pylena-0.1.2/pylena/morpho/soperations.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <pln/core/image_cast.hpp>
+#include <pln/image_cast.hpp>
 
 #include <mln/core/image/ndimage.hpp>
 #include <mln/morpho/closing.hpp>
 #include <mln/morpho/dilation.hpp>
 #include <mln/morpho/gradient.hpp>
 #include <mln/morpho/opening.hpp>
 #include <mln/core/extension/border_management.hpp>
```

### Comparing `pylena-0.1.1/pylena/morpho/soperations.py` & `pylena-0.1.2/pylena/morpho/soperations.py`

 * *Files identical despite different names*

### Comparing `pylena-0.1.1/pylena/morpho/watershed.cpp` & `pylena-0.1.2/pylena/morpho/watershed.cpp`

 * *Files identical despite different names*

### Comparing `pylena-0.1.1/pylena/morpho/watershed.py` & `pylena-0.1.2/pylena/morpho/watershed.py`

 * *Files identical despite different names*

### Comparing `pylena-0.1.1/pylena/utils.py` & `pylena-0.1.2/pylena/utils.py`

 * *Files identical despite different names*

### Comparing `pylena-0.1.1/pylena.egg-info/PKG-INFO` & `pylena-0.1.2/pylena.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pylena
-Version: 0.1.1
+Version: 0.1.2
 Summary: Image processing library
-Author-email: "EPITA Research and Development Laboratory (LRDE)" <baptiste.esteban@lrde.epita.fr>
+Author-email: "EPITA Research Laboratory (LRE)" <baptiste.esteban@epita.fr>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
         
         1.1. "Contributor"
@@ -373,19 +373,19 @@
         
         Exhibit B - "Incompatible With Secondary Licenses" Notice
         ---------------------------------------------------------
         
           This Source Code Form is "Incompatible With Secondary Licenses", as
           defined by the Mozilla Public License, v. 2.0.
         
-Project-URL: homepage, http://olena.pages.lrde.epita.fr/pylena/
-Project-URL: documentation, http://olena.pages.lrde.epita.fr/pylena/
-Project-URL: repository, https://gitlab.lrde.epita.fr/olena/pylena
-Project-URL: Bug Tracker, https://gitlab.lrde.epita.fr/olena/pylena/-/issues
-Project-URL: changelog, http://olena.pages.lrde.epita.fr/pylena/changelog.html
+Project-URL: homepage, http://olena.pages.lre.epita.fr/pylena/
+Project-URL: documentation, http://olena.pages.lre.epita.fr/pylena/
+Project-URL: repository, https://gitlab.lre.epita.fr/olena/pylena
+Project-URL: Bug Tracker, https://gitlab.lre.epita.fr/olena/pylena/-/issues
+Project-URL: changelog, http://olena.pages.lre.epita.fr/pylena/changelog.html
 Platform: linux
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -394,20 +394,20 @@
 Provides-Extra: packaging
 Provides-Extra: doc
 Provides-Extra: tests
 License-File: LICENSE
 
 # Pylena image processing library
 
-[![image alt pipeline](https://gitlab.lrde.epita.fr/olena/pylena/badges/master/pipeline.svg)](https://gitlab.lrde.epita.fr/olena/pylena/-/commits/master)
-[![image alt python coverage](https://gitlab.lrde.epita.fr/olena/pylena/badges/master/coverage.svg?job=python_coverage&key_text=Python+Coverage&key_width=100)](https://gitlab.lrde.epita.fr/olena/pylena/-/commits/master)
-[![image alt cpp coverage](https://gitlab.lrde.epita.fr/olena/pylena/badges/master/coverage.svg?job=cpp_coverage&key_text=C%2B%2B+Coverage&key_width=100)](https://gitlab.lrde.epita.fr/olena/pylena/-/commits/master)
+[![image alt pipeline](https://gitlab.lre.epita.fr/olena/pylena/badges/master/pipeline.svg)](https://gitlab.lre.epita.fr/olena/pylena/-/commits/master)
+[![image alt python coverage](https://gitlab.lre.epita.fr/olena/pylena/badges/master/coverage.svg?job=python_coverage&key_text=Python+Coverage&key_width=100)](https://gitlab.lre.epita.fr/olena/pylena/-/commits/master)
+[![image alt cpp coverage](https://gitlab.lre.epita.fr/olena/pylena/badges/master/coverage.svg?job=cpp_coverage&key_text=C%2B%2B+Coverage&key_width=100)](https://gitlab.lre.epita.fr/olena/pylena/-/commits/master)
 
 Pylena is the Python interface to the modern C++ image processing library
-[Pylene](https://gitlab.lrde.epita.fr/olena/pylene). Its aim is to fill the three following requirements:
+[Pylene](https://gitlab.lre.epita.fr/olena/pylene). Its aim is to fill the three following requirements:
 * Interactivity
 * Genericity
 * Efficiency
 
 Many image processing libraries succeed to fill these requirements but they are
 still limited by the static nature of the C++ language, where the genericity,
 based on *templates*, is resolved at compile time. Thus, the goal of this library is to tackle this problem.
@@ -428,18 +428,18 @@
 
 ```
 $ pip install pylena
 ```
 
 ## Documentation
 
-The documentation is available [here](http://olena.pages.lrde.epita.fr/pylena/).
+The documentation is available [here](http://olena.pages.lre.epita.fr/pylena/).
 
 ## Contributing
 
 If you find any bug or have any suggestions, feel free to create a new issue
-[here](https://gitlab.lrde.epita.fr/olena/pylena/-/issues) or send an email to
-[baptiste.esteban@lrde.epita.fr](mailto:baptiste.esteban@lrde.epita.fr).
+[here](https://gitlab.lre.epita.fr/olena/pylena/-/issues) or send an email to
+[baptiste.esteban@epita.fr](mailto:baptiste.esteban@epita.fr).
 
 ## Licence
 
 [Mozilla Public License Version 2.0](https://www.mozilla.org/en-US/MPL/2.0/)
```

### Comparing `pylena-0.1.1/pylene-numpy/CMakeLists.txt` & `pylena-0.1.2/pylene-numpy/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,11 +4,11 @@
                          $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>
                          $<INSTALL_INTERFACE:include>)
 target_sources(pylene-numpy PRIVATE ${CMAKE_CURRENT_SOURCE_DIR}/src/image_cast.cpp
                                     ${CMAKE_CURRENT_SOURCE_DIR}/src/numpy_format.cpp
 )
 target_link_libraries(pylene-numpy PUBLIC pylene::core pybind11::pybind11)
 
-# Waiting issue Pylene#101 is solved (https://gitlab.lrde.epita.fr/olena/pylene/-/issues/101)
+# Waiting issue Pylene#101 is solved (https://gitlab.lre.epita.fr/olena/pylene/-/issues/101)
 if (MSVC)
     target_compile_options(pylene-numpy PUBLIC "/Zc:preprocessor" "/permissive-")
 endif (MSVC)
```

### Comparing `pylena-0.1.1/pylene-numpy/include/pln/image_cast.hpp` & `pylena-0.1.2/pylene-numpy/include/pln/image_cast.hpp`

 * *Files identical despite different names*

### Comparing `pylena-0.1.1/pylene-numpy/src/image_cast.cpp` & `pylena-0.1.2/pylene-numpy/src/image_cast.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #include <mln/core/image/private/ndbuffer_image_data.hpp>
-#include <pln/core/image_cast.hpp>
+#include <pln/image_cast.hpp>
 #include "numpy_format.hpp"
 
 #include <pybind11/cast.h>
 
 #include <fmt/format.h>
 
 #include <cassert>
```

### Comparing `pylena-0.1.1/pylene-numpy/src/numpy_format.cpp` & `pylena-0.1.2/pylene-numpy/src/numpy_format.cpp`

 * *Files identical despite different names*

### Comparing `pylena-0.1.1/pylene-numpy/src/numpy_format.hpp` & `pylena-0.1.2/pylene-numpy/src/numpy_format.hpp`

 * *Files identical despite different names*

### Comparing `pylena-0.1.1/pyproject.toml` & `pylena-0.1.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "pylena"
 description = "Image processing library"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
-    {name = "EPITA Research and Development Laboratory (LRDE)", email = "baptiste.esteban@lrde.epita.fr"}
+    {name = "EPITA Research Laboratory (LRE)", email = "baptiste.esteban@epita.fr"}
 ]
 classifiers = [
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: C++",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
@@ -18,30 +18,30 @@
 dependencies = [
     "numpy",
     "numba"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
-packaging = ["auditwheel"]
+packaging = ["auditwheel", "patchelf"]
 doc = ["sphinx", "sphinx_rtd_theme", "sphinx_gallery", "scikit-image", "matplotlib", "imagecodecs>=2021.11.20", "pandas", "sphinxcontrib-bibtex"]
 tests = ["pytest"]
 
 [project.urls]
-homepage = "http://olena.pages.lrde.epita.fr/pylena/"
-documentation = "http://olena.pages.lrde.epita.fr/pylena/"
-repository = "https://gitlab.lrde.epita.fr/olena/pylena"
-"Bug Tracker" = "https://gitlab.lrde.epita.fr/olena/pylena/-/issues"
-changelog = "http://olena.pages.lrde.epita.fr/pylena/changelog.html"
+homepage = "http://olena.pages.lre.epita.fr/pylena/"
+documentation = "http://olena.pages.lre.epita.fr/pylena/"
+repository = "https://gitlab.lre.epita.fr/olena/pylena"
+"Bug Tracker" = "https://gitlab.lre.epita.fr/olena/pylena/-/issues"
+changelog = "http://olena.pages.lre.epita.fr/pylena/changelog.html"
 
 [tool.setuptools.dynamic]
 version = {attr = "pylena._version.__version__"}
 
 [build-system]
-requires = ["setuptools>=61.0.0", "wheel", "conan>=1.49.0", "cmake>=3.15.0", "pybind11==2.9.2"]
+requires = ["setuptools>=61.0.0", "wheel", "conan==2.0.4", "cmake>=3.15.0", "pybind11==2.9.2"]
 build-backend = "setuptools.build_meta"
 
 # Development tools
 
 [tool.coverage.report]
 exclude_lines = [
     "# coverage: disable"
```

