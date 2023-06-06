# Comparing `tmp/Algebra_with_SymPy-0.9.4.tar.gz` & `tmp/Algebra_with_SymPy-0.9.4rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Algebra_with_SymPy-0.9.4.tar", last modified: Thu Aug 11 16:44:53 2022, max compression
+gzip compressed data, was "Algebra_with_SymPy-0.9.4rc0.tar", last modified: Thu Aug 11 16:47:01 2022, max compression
```

## Comparing `Algebra_with_SymPy-0.9.4.tar` & `Algebra_with_SymPy-0.9.4rc0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2022-08-11 16:44:53.485854 Algebra_with_SymPy-0.9.4/
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2022-08-11 16:44:53.481854 Algebra_with_SymPy-0.9.4/Algebra_with_SymPy.egg-info/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       92 2021-02-12 03:15:32.000000 Algebra_with_SymPy-0.9.4/Algebra_with_SymPy.egg-info/.~lock.In process discussion comment.odt#
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    13120 2021-02-12 03:15:32.000000 Algebra_with_SymPy-0.9.4/Algebra_with_SymPy.egg-info/In process discussion comment.odt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     7441 2022-08-11 16:44:53.000000 Algebra_with_SymPy-0.9.4/Algebra_with_SymPy.egg-info/PKG-INFO
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      532 2022-08-11 16:44:53.000000 Algebra_with_SymPy-0.9.4/Algebra_with_SymPy.egg-info/SOURCES.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)        1 2022-08-11 16:44:53.000000 Algebra_with_SymPy-0.9.4/Algebra_with_SymPy.egg-info/dependency_links.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       27 2022-08-11 16:44:53.000000 Algebra_with_SymPy-0.9.4/Algebra_with_SymPy.egg-info/requires.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       25 2022-08-11 16:44:53.000000 Algebra_with_SymPy-0.9.4/Algebra_with_SymPy.egg-info/top_level.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     7441 2022-08-11 16:44:53.485854 Algebra_with_SymPy-0.9.4/PKG-INFO
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2022-08-11 16:44:53.481854 Algebra_with_SymPy-0.9.4/algebra_with_sympy/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      306 2022-08-11 16:12:04.000000 Algebra_with_SymPy-0.9.4/algebra_with_sympy/__init__.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    28988 2022-08-11 15:53:47.000000 Algebra_with_SymPy-0.9.4/algebra_with_sympy/algebraic_equation.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     2473 2022-08-11 16:33:45.000000 Algebra_with_SymPy-0.9.4/algebra_with_sympy/preparser.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       38 2022-08-11 16:44:53.485854 Algebra_with_SymPy-0.9.4/setup.cfg
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1194 2022-08-11 16:12:04.000000 Algebra_with_SymPy-0.9.4/setup.py
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2022-08-11 16:44:53.481854 Algebra_with_SymPy-0.9.4/tests/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)        0 2022-04-03 01:35:16.000000 Algebra_with_SymPy-0.9.4/tests/__init__.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    28988 2022-08-11 15:53:47.000000 Algebra_with_SymPy-0.9.4/tests/algebraic_equation.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     7992 2022-04-03 01:35:16.000000 Algebra_with_SymPy-0.9.4/tests/test_algebraic_equation.py
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2022-08-11 16:47:01.650005 Algebra_with_SymPy-0.9.4rc0/
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2022-08-11 16:47:01.646005 Algebra_with_SymPy-0.9.4rc0/Algebra_with_SymPy.egg-info/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       92 2021-02-12 03:15:32.000000 Algebra_with_SymPy-0.9.4rc0/Algebra_with_SymPy.egg-info/.~lock.In process discussion comment.odt#
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    13120 2021-02-12 03:15:32.000000 Algebra_with_SymPy-0.9.4rc0/Algebra_with_SymPy.egg-info/In process discussion comment.odt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     7444 2022-08-11 16:47:01.000000 Algebra_with_SymPy-0.9.4rc0/Algebra_with_SymPy.egg-info/PKG-INFO
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      532 2022-08-11 16:47:01.000000 Algebra_with_SymPy-0.9.4rc0/Algebra_with_SymPy.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)        1 2022-08-11 16:47:01.000000 Algebra_with_SymPy-0.9.4rc0/Algebra_with_SymPy.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       27 2022-08-11 16:47:01.000000 Algebra_with_SymPy-0.9.4rc0/Algebra_with_SymPy.egg-info/requires.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       25 2022-08-11 16:47:01.000000 Algebra_with_SymPy-0.9.4rc0/Algebra_with_SymPy.egg-info/top_level.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     7444 2022-08-11 16:47:01.650005 Algebra_with_SymPy-0.9.4rc0/PKG-INFO
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2022-08-11 16:47:01.650005 Algebra_with_SymPy-0.9.4rc0/algebra_with_sympy/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      306 2022-08-11 16:12:04.000000 Algebra_with_SymPy-0.9.4rc0/algebra_with_sympy/__init__.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    28988 2022-08-11 15:53:47.000000 Algebra_with_SymPy-0.9.4rc0/algebra_with_sympy/algebraic_equation.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     2473 2022-08-11 16:33:45.000000 Algebra_with_SymPy-0.9.4rc0/algebra_with_sympy/preparser.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       38 2022-08-11 16:47:01.650005 Algebra_with_SymPy-0.9.4rc0/setup.cfg
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1197 2022-08-11 16:46:57.000000 Algebra_with_SymPy-0.9.4rc0/setup.py
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2022-08-11 16:47:01.650005 Algebra_with_SymPy-0.9.4rc0/tests/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)        0 2022-04-03 01:35:16.000000 Algebra_with_SymPy-0.9.4rc0/tests/__init__.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    28988 2022-08-11 15:53:47.000000 Algebra_with_SymPy-0.9.4rc0/tests/algebraic_equation.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     7992 2022-04-03 01:35:16.000000 Algebra_with_SymPy-0.9.4rc0/tests/test_algebraic_equation.py
```

### Comparing `Algebra_with_SymPy-0.9.4/Algebra_with_SymPy.egg-info/In process discussion comment.odt` & `Algebra_with_SymPy-0.9.4rc0/Algebra_with_SymPy.egg-info/In process discussion comment.odt`

 * *Files identical despite different names*

### Comparing `Algebra_with_SymPy-0.9.4/Algebra_with_SymPy.egg-info/PKG-INFO` & `Algebra_with_SymPy-0.9.4rc0/Algebra_with_SymPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Algebra-with-SymPy
-Version: 0.9.4
+Version: 0.9.4rc0
 Summary: Equations that can be algebraicly manipulated.
 Home-page: https://gutow.github.io/Algebra_with_Sympy/
 Author: Jonathan Gutow
 Author-email: gutow@uwosh.edu
 License: GPL-3.0+
 Keywords: symbolic algebra,computer algebra,CAS,calculations with units,sympy
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Algebra_with_SymPy-0.9.4/Algebra_with_SymPy.egg-info/SOURCES.txt` & `Algebra_with_SymPy-0.9.4rc0/Algebra_with_SymPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Algebra_with_SymPy-0.9.4/PKG-INFO` & `Algebra_with_SymPy-0.9.4rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Algebra_with_SymPy
-Version: 0.9.4
+Version: 0.9.4rc0
 Summary: Equations that can be algebraicly manipulated.
 Home-page: https://gutow.github.io/Algebra_with_Sympy/
 Author: Jonathan Gutow
 Author-email: gutow@uwosh.edu
 License: GPL-3.0+
 Keywords: symbolic algebra,computer algebra,CAS,calculations with units,sympy
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Algebra_with_SymPy-0.9.4/algebra_with_sympy/algebraic_equation.py` & `Algebra_with_SymPy-0.9.4rc0/algebra_with_sympy/algebraic_equation.py`

 * *Files identical despite different names*

### Comparing `Algebra_with_SymPy-0.9.4/algebra_with_sympy/preparser.py` & `Algebra_with_SymPy-0.9.4rc0/algebra_with_sympy/preparser.py`

 * *Files identical despite different names*

### Comparing `Algebra_with_SymPy-0.9.4/setup.py` & `Algebra_with_SymPy-0.9.4rc0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("ReadMe.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="Algebra_with_SymPy",
     url = "https://gutow.github.io/Algebra_with_Sympy/",
-    version="0.9.4",
+    version="0.9.4rc0",
     description="Equations that can be algebraicly manipulated.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Jonathan Gutow",
     author_email="gutow@uwosh.edu",
     keywords="symbolic algebra, computer algebra, CAS, calculations with "
              "units, sympy",
```

### Comparing `Algebra_with_SymPy-0.9.4/tests/algebraic_equation.py` & `Algebra_with_SymPy-0.9.4rc0/tests/algebraic_equation.py`

 * *Files identical despite different names*

### Comparing `Algebra_with_SymPy-0.9.4/tests/test_algebraic_equation.py` & `Algebra_with_SymPy-0.9.4rc0/tests/test_algebraic_equation.py`

 * *Files identical despite different names*

