# Comparing `tmp/pysmali-0.1.3.tar.gz` & `tmp/pysmali-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysmali-0.1.3.tar", last modified: Sat Jun  3 19:31:15 2023, max compression
+gzip compressed data, was "pysmali-0.2.0.tar", last modified: Tue Jun  6 06:03:03 2023, max compression
```

## Comparing `pysmali-0.1.3.tar` & `pysmali-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 19:31:15.903026 pysmali-0.1.3/
--rw-rw-rw-   0        0        0    35803 2023-06-03 19:18:10.000000 pysmali-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     6068 2023-06-03 19:31:15.905026 pysmali-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     5393 2023-06-03 19:28:49.000000 pysmali-0.1.3/README.md
--rw-rw-rw-   0        0        0      856 2023-06-03 19:22:30.000000 pysmali-0.1.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-03 19:31:15.198167 pysmali-0.1.3/pysmali.egg-info/
--rw-rw-rw-   0        0        0     6068 2023-06-03 19:31:14.000000 pysmali-0.1.3/pysmali.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      534 2023-06-03 19:31:14.000000 pysmali-0.1.3/pysmali.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 19:31:14.000000 pysmali-0.1.3/pysmali.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-03 19:31:14.000000 pysmali-0.1.3/pysmali.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-06-03 19:31:14.000000 pysmali-0.1.3/pysmali.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 19:31:15.916027 pysmali-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-03 19:31:15.465331 pysmali-0.1.3/smali/
--rw-rw-rw-   0        0        0     1012 2023-06-03 19:18:11.000000 pysmali-0.1.3/smali/__init__.py
--rw-rw-rw-   0        0        0    21638 2023-06-03 19:22:30.000000 pysmali-0.1.3/smali/base.py
-drwxrwxrwx   0        0        0        0 2023-06-03 19:31:15.724027 pysmali-0.1.3/smali/bridge/
--rw-rw-rw-   0        0        0      909 2023-06-03 19:18:11.000000 pysmali-0.1.3/smali/bridge/__init__.py
--rw-rw-rw-   0        0        0     1972 2023-06-03 19:18:11.000000 pysmali-0.1.3/smali/bridge/errors.py
--rw-rw-rw-   0        0        0    24233 2023-06-03 19:22:30.000000 pysmali-0.1.3/smali/bridge/executor.py
--rw-rw-rw-   0        0        0     3733 2023-06-03 19:22:30.000000 pysmali-0.1.3/smali/bridge/frame.py
--rw-rw-rw-   0        0        0    28077 2023-06-03 19:18:11.000000 pysmali-0.1.3/smali/bridge/lang.py
--rw-rw-rw-   0        0        0     1133 2023-06-03 19:18:11.000000 pysmali-0.1.3/smali/bridge/objects.py
--rw-rw-rw-   0        0        0    18607 2023-06-03 19:22:30.000000 pysmali-0.1.3/smali/bridge/vm.py
--rw-rw-rw-   0        0        0     8936 2023-06-03 19:18:11.000000 pysmali-0.1.3/smali/opcode.py
--rw-rw-rw-   0        0        0    34778 2023-06-03 19:18:11.000000 pysmali-0.1.3/smali/reader.py
-drwxrwxrwx   0        0        0        0 2023-06-03 19:31:15.869033 pysmali-0.1.3/smali/shell/
--rw-rw-rw-   0        0        0     1356 2023-06-03 19:18:11.000000 pysmali-0.1.3/smali/shell/__init__.py
--rw-rw-rw-   0        0        0      854 2023-06-03 19:18:11.000000 pysmali-0.1.3/smali/shell/__main__.py
--rw-rw-rw-   0        0        0     2274 2023-06-03 19:18:11.000000 pysmali-0.1.3/smali/shell/cli.py
--rw-rw-rw-   0        0        0    10014 2023-06-03 19:18:11.000000 pysmali-0.1.3/smali/shell/model.py
--rw-rw-rw-   0        0        0    16049 2023-06-03 19:18:11.000000 pysmali-0.1.3/smali/visitor.py
--rw-rw-rw-   0        0        0    22486 2023-06-03 19:18:11.000000 pysmali-0.1.3/smali/writer.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:03:03.608658 pysmali-0.2.0/
+-rw-rw-rw-   0        0        0    35803 2023-06-03 19:18:10.000000 pysmali-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     6235 2023-06-06 06:03:03.610660 pysmali-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5560 2023-06-06 05:57:56.000000 pysmali-0.2.0/README.md
+-rw-rw-rw-   0        0        0      856 2023-06-05 19:54:53.000000 pysmali-0.2.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-06 06:03:02.856660 pysmali-0.2.0/pysmali.egg-info/
+-rw-rw-rw-   0        0        0     6235 2023-06-06 06:03:02.000000 pysmali-0.2.0/pysmali.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      534 2023-06-06 06:03:02.000000 pysmali-0.2.0/pysmali.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 06:03:02.000000 pysmali-0.2.0/pysmali.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-06 06:03:02.000000 pysmali-0.2.0/pysmali.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-06-06 06:03:02.000000 pysmali-0.2.0/pysmali.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 06:03:03.617658 pysmali-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-06 06:03:03.104447 pysmali-0.2.0/smali/
+-rw-rw-rw-   0        0        0     1012 2023-06-03 19:18:11.000000 pysmali-0.2.0/smali/__init__.py
+-rw-rw-rw-   0        0        0    22560 2023-06-06 05:56:23.000000 pysmali-0.2.0/smali/base.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:03:03.406658 pysmali-0.2.0/smali/bridge/
+-rw-rw-rw-   0        0        0      909 2023-06-03 19:18:11.000000 pysmali-0.2.0/smali/bridge/__init__.py
+-rw-rw-rw-   0        0        0     1972 2023-06-03 19:18:11.000000 pysmali-0.2.0/smali/bridge/errors.py
+-rw-rw-rw-   0        0        0    24322 2023-06-05 20:08:04.000000 pysmali-0.2.0/smali/bridge/executor.py
+-rw-rw-rw-   0        0        0     3733 2023-06-03 19:22:30.000000 pysmali-0.2.0/smali/bridge/frame.py
+-rw-rw-rw-   0        0        0    29231 2023-06-06 05:39:18.000000 pysmali-0.2.0/smali/bridge/lang.py
+-rw-rw-rw-   0        0        0     1133 2023-06-03 19:18:11.000000 pysmali-0.2.0/smali/bridge/objects.py
+-rw-rw-rw-   0        0        0    18853 2023-06-06 05:12:57.000000 pysmali-0.2.0/smali/bridge/vm.py
+-rw-rw-rw-   0        0        0     8936 2023-06-03 19:18:11.000000 pysmali-0.2.0/smali/opcode.py
+-rw-rw-rw-   0        0        0    34838 2023-06-06 05:38:46.000000 pysmali-0.2.0/smali/reader.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:03:03.567657 pysmali-0.2.0/smali/shell/
+-rw-rw-rw-   0        0        0     1356 2023-06-03 19:18:11.000000 pysmali-0.2.0/smali/shell/__init__.py
+-rw-rw-rw-   0        0        0      854 2023-06-03 19:18:11.000000 pysmali-0.2.0/smali/shell/__main__.py
+-rw-rw-rw-   0        0        0     2274 2023-06-03 19:18:11.000000 pysmali-0.2.0/smali/shell/cli.py
+-rw-rw-rw-   0        0        0    10082 2023-06-05 20:11:32.000000 pysmali-0.2.0/smali/shell/model.py
+-rw-rw-rw-   0        0        0    16049 2023-06-03 19:18:11.000000 pysmali-0.2.0/smali/visitor.py
+-rw-rw-rw-   0        0        0    22486 2023-06-03 19:18:11.000000 pysmali-0.2.0/smali/writer.py
```

### Comparing `pysmali-0.1.3/LICENSE` & `pysmali-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.3/PKG-INFO` & `pysmali-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysmali
-Version: 0.1.3
+Version: 0.2.0
 Summary: Smali Visitor-API and Smali emulator
 Author-email: MatrixEditor <not@supported.com>
 Project-URL: Homepage, https://github.com/MatrixEditor/pysmali
 Project-URL: API-Docs, https://pysmali.readthedocs.io/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -17,15 +17,15 @@
 # PySmali
 
 [![python](https://img.shields.io/badge/python-3.8+-blue.svg?logo=python&labelColor=lightgrey)](https://www.python.org/downloads/)
 ![LastEdit](https://img.shields.io:/static/v1?label=LastEdit&message=06/03/2023&color=9cf)
 ![Status](https://img.shields.io:/static/v1?label=Status&message=Pre-Release&color=teal)
 ![Platform](https://img.shields.io:/static/v1?label=Platforms&message=Linux|Windows&color=lightgrey)
 [![Build and Deploy Sphinx Documentation](https://github.com/MatrixEditor/pysmali/actions/workflows/sphinx.yml/badge.svg)](https://github.com/MatrixEditor/pysmali/actions/workflows/sphinx.yml)
-![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=0.1.3&color=lightblue)
+![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=0.2.0&color=lightblue)
 
 
 The main functionalities of this repository cover creating and parsing Smali files with Python3 as well as interpret Smali source code files. There is also an interactive interpreter provided that acts as a Python-CLI.
 
 ## Installation
 
 By now, the only way to install the python module in this repository is by cloning it and running the following command:
@@ -36,17 +36,19 @@
 $ pip install pysmali
 ```
 
 ## Usage
 
 For a more detailed explanation of the Smali Visitor-API use the [Github-Pages Docs](https://matrixeditor.github.io/pysmali/).
 
+> **Info**: Make sure you are using ``pysmali>=0.2.0`` as it introduces a user-friendly type system to mitigate possible issues from parsing type descriptors.
+
 ### ISmali (Interactive Smali Interpreter)
 
-As of version `0.1.3` the interactive interpreter can be used to execute Smali code directly:
+As of version `0.1.2` the interactive interpreter can be used to execute Smali code directly:
 
 ```bash
 $ ismali example.ssf
 # or start interactive mode
 $ ismali
 >>> vars
 {'p0': <SmaliObject@195f5c0da90>}
@@ -84,22 +86,22 @@
 * `snippet`: To parse simple code snippets without a .class definition, use the 'snippet' variable (or within the constructor). Use this property only if you don't have a '.class' definition at the start of the source code
 * `validate`: Validates the parsed code
 * `errors`: With values `"strict"` or `"ignore"` this attribute will cause the reader to raise or ignore exceptions
 
 Actually, the code above does nothing as the `ClassVisitor` class does not handle any notification by the reader. For instance, to print out the class name of a parsed code, the following implementation could be used:
 
 ```python
-from smali import SmaliReader, ClassVisitor, Type
+from smali import SmaliReader, ClassVisitor, SVMType
 
 class NamePrinterVisitor(ClassVisitor):
     def visit_class(self, name: str, access_flags: int) -> None:
         # The provided name is the type descriptor, so we have to
         # convert it:
-        cls_type = Type(name)
-        print('ClassName:', cls_type.class_name)
+        cls_type = SVMType(name)
+        print('Class:', cls_type.pretty_name) # prints: com.example.Hello
 
 reader = SmaliReader()
 reader.visit(".class public final Lcom/example/Hello;", NamePrinterVisitor())
 ```
 
 ### Writing Smali-Files
 
@@ -132,25 +134,23 @@
 # create the finished source code, BUT don't forget visit_end()
 writer.visit_end()
 text = writer.code
 ```
 
 ### Importing classes and execute methods
 
-As of version `0.1.3` you can import Smali files and execute defined methods:
+As of version `0.1.2` you can import Smali files and execute defined methods:
 
 ```python
 from smali.bridge import SmaliVM, SmaliObject
 
-with open('example.smali', 'r', encoding='utf-8') as fp:
-    source = fp.read()
-
 vm = SmaliVM()
 # Import class definition
-smali_class = vm.classloader.load_class(source, init=False)
+with open('example.smali', 'r', encoding='utf-8') as fp:
+    smali_class = vm.classloader.load_class(fp, init=False)
 # Call <clinit> method
 smali_class.clinit()
 
 # Create a new instance of the imported class
 instance = SmaliObject(smali_class)
 # Call the object's constructor
 instance.init()
```

### Comparing `pysmali-0.1.3/README.md` & `pysmali-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # PySmali
 
 [![python](https://img.shields.io/badge/python-3.8+-blue.svg?logo=python&labelColor=lightgrey)](https://www.python.org/downloads/)
 ![LastEdit](https://img.shields.io:/static/v1?label=LastEdit&message=06/03/2023&color=9cf)
 ![Status](https://img.shields.io:/static/v1?label=Status&message=Pre-Release&color=teal)
 ![Platform](https://img.shields.io:/static/v1?label=Platforms&message=Linux|Windows&color=lightgrey)
 [![Build and Deploy Sphinx Documentation](https://github.com/MatrixEditor/pysmali/actions/workflows/sphinx.yml/badge.svg)](https://github.com/MatrixEditor/pysmali/actions/workflows/sphinx.yml)
-![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=0.1.3&color=lightblue)
+![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=0.2.0&color=lightblue)
 
 
 The main functionalities of this repository cover creating and parsing Smali files with Python3 as well as interpret Smali source code files. There is also an interactive interpreter provided that acts as a Python-CLI.
 
 ## Installation
 
 By now, the only way to install the python module in this repository is by cloning it and running the following command:
@@ -20,17 +20,19 @@
 $ pip install pysmali
 ```
 
 ## Usage
 
 For a more detailed explanation of the Smali Visitor-API use the [Github-Pages Docs](https://matrixeditor.github.io/pysmali/).
 
+> **Info**: Make sure you are using ``pysmali>=0.2.0`` as it introduces a user-friendly type system to mitigate possible issues from parsing type descriptors.
+
 ### ISmali (Interactive Smali Interpreter)
 
-As of version `0.1.3` the interactive interpreter can be used to execute Smali code directly:
+As of version `0.1.2` the interactive interpreter can be used to execute Smali code directly:
 
 ```bash
 $ ismali example.ssf
 # or start interactive mode
 $ ismali
 >>> vars
 {'p0': <SmaliObject@195f5c0da90>}
@@ -68,22 +70,22 @@
 * `snippet`: To parse simple code snippets without a .class definition, use the 'snippet' variable (or within the constructor). Use this property only if you don't have a '.class' definition at the start of the source code
 * `validate`: Validates the parsed code
 * `errors`: With values `"strict"` or `"ignore"` this attribute will cause the reader to raise or ignore exceptions
 
 Actually, the code above does nothing as the `ClassVisitor` class does not handle any notification by the reader. For instance, to print out the class name of a parsed code, the following implementation could be used:
 
 ```python
-from smali import SmaliReader, ClassVisitor, Type
+from smali import SmaliReader, ClassVisitor, SVMType
 
 class NamePrinterVisitor(ClassVisitor):
     def visit_class(self, name: str, access_flags: int) -> None:
         # The provided name is the type descriptor, so we have to
         # convert it:
-        cls_type = Type(name)
-        print('ClassName:', cls_type.class_name)
+        cls_type = SVMType(name)
+        print('Class:', cls_type.pretty_name) # prints: com.example.Hello
 
 reader = SmaliReader()
 reader.visit(".class public final Lcom/example/Hello;", NamePrinterVisitor())
 ```
 
 ### Writing Smali-Files
 
@@ -116,25 +118,23 @@
 # create the finished source code, BUT don't forget visit_end()
 writer.visit_end()
 text = writer.code
 ```
 
 ### Importing classes and execute methods
 
-As of version `0.1.3` you can import Smali files and execute defined methods:
+As of version `0.1.2` you can import Smali files and execute defined methods:
 
 ```python
 from smali.bridge import SmaliVM, SmaliObject
 
-with open('example.smali', 'r', encoding='utf-8') as fp:
-    source = fp.read()
-
 vm = SmaliVM()
 # Import class definition
-smali_class = vm.classloader.load_class(source, init=False)
+with open('example.smali', 'r', encoding='utf-8') as fp:
+    smali_class = vm.classloader.load_class(fp, init=False)
 # Call <clinit> method
 smali_class.clinit()
 
 # Create a new instance of the imported class
 instance = SmaliObject(smali_class)
 # Call the object's constructor
 instance.init()
```

### Comparing `pysmali-0.1.3/pyproject.toml` & `pysmali-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pysmali"
-version = "0.1.3"
+version = "0.2.0"
 description="Smali Visitor-API and Smali emulator"
 authors = [
   { name="MatrixEditor", email="not@supported.com" },
 ]
 readme = "README.md"
 classifiers = [
     'Development Status :: 5 - Production/Stable',
```

### Comparing `pysmali-0.1.3/pysmali.egg-info/PKG-INFO` & `pysmali-0.2.0/pysmali.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysmali
-Version: 0.1.3
+Version: 0.2.0
 Summary: Smali Visitor-API and Smali emulator
 Author-email: MatrixEditor <not@supported.com>
 Project-URL: Homepage, https://github.com/MatrixEditor/pysmali
 Project-URL: API-Docs, https://pysmali.readthedocs.io/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -17,15 +17,15 @@
 # PySmali
 
 [![python](https://img.shields.io/badge/python-3.8+-blue.svg?logo=python&labelColor=lightgrey)](https://www.python.org/downloads/)
 ![LastEdit](https://img.shields.io:/static/v1?label=LastEdit&message=06/03/2023&color=9cf)
 ![Status](https://img.shields.io:/static/v1?label=Status&message=Pre-Release&color=teal)
 ![Platform](https://img.shields.io:/static/v1?label=Platforms&message=Linux|Windows&color=lightgrey)
 [![Build and Deploy Sphinx Documentation](https://github.com/MatrixEditor/pysmali/actions/workflows/sphinx.yml/badge.svg)](https://github.com/MatrixEditor/pysmali/actions/workflows/sphinx.yml)
-![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=0.1.3&color=lightblue)
+![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=0.2.0&color=lightblue)
 
 
 The main functionalities of this repository cover creating and parsing Smali files with Python3 as well as interpret Smali source code files. There is also an interactive interpreter provided that acts as a Python-CLI.
 
 ## Installation
 
 By now, the only way to install the python module in this repository is by cloning it and running the following command:
@@ -36,17 +36,19 @@
 $ pip install pysmali
 ```
 
 ## Usage
 
 For a more detailed explanation of the Smali Visitor-API use the [Github-Pages Docs](https://matrixeditor.github.io/pysmali/).
 
+> **Info**: Make sure you are using ``pysmali>=0.2.0`` as it introduces a user-friendly type system to mitigate possible issues from parsing type descriptors.
+
 ### ISmali (Interactive Smali Interpreter)
 
-As of version `0.1.3` the interactive interpreter can be used to execute Smali code directly:
+As of version `0.1.2` the interactive interpreter can be used to execute Smali code directly:
 
 ```bash
 $ ismali example.ssf
 # or start interactive mode
 $ ismali
 >>> vars
 {'p0': <SmaliObject@195f5c0da90>}
@@ -84,22 +86,22 @@
 * `snippet`: To parse simple code snippets without a .class definition, use the 'snippet' variable (or within the constructor). Use this property only if you don't have a '.class' definition at the start of the source code
 * `validate`: Validates the parsed code
 * `errors`: With values `"strict"` or `"ignore"` this attribute will cause the reader to raise or ignore exceptions
 
 Actually, the code above does nothing as the `ClassVisitor` class does not handle any notification by the reader. For instance, to print out the class name of a parsed code, the following implementation could be used:
 
 ```python
-from smali import SmaliReader, ClassVisitor, Type
+from smali import SmaliReader, ClassVisitor, SVMType
 
 class NamePrinterVisitor(ClassVisitor):
     def visit_class(self, name: str, access_flags: int) -> None:
         # The provided name is the type descriptor, so we have to
         # convert it:
-        cls_type = Type(name)
-        print('ClassName:', cls_type.class_name)
+        cls_type = SVMType(name)
+        print('Class:', cls_type.pretty_name) # prints: com.example.Hello
 
 reader = SmaliReader()
 reader.visit(".class public final Lcom/example/Hello;", NamePrinterVisitor())
 ```
 
 ### Writing Smali-Files
 
@@ -132,25 +134,23 @@
 # create the finished source code, BUT don't forget visit_end()
 writer.visit_end()
 text = writer.code
 ```
 
 ### Importing classes and execute methods
 
-As of version `0.1.3` you can import Smali files and execute defined methods:
+As of version `0.1.2` you can import Smali files and execute defined methods:
 
 ```python
 from smali.bridge import SmaliVM, SmaliObject
 
-with open('example.smali', 'r', encoding='utf-8') as fp:
-    source = fp.read()
-
 vm = SmaliVM()
 # Import class definition
-smali_class = vm.classloader.load_class(source, init=False)
+with open('example.smali', 'r', encoding='utf-8') as fp:
+    smali_class = vm.classloader.load_class(fp, init=False)
 # Call <clinit> method
 smali_class.clinit()
 
 # Create a new instance of the imported class
 instance = SmaliObject(smali_class)
 # Call the object's constructor
 instance.init()
```

### Comparing `pysmali-0.1.3/pysmali.egg-info/SOURCES.txt` & `pysmali-0.2.0/pysmali.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.3/smali/__init__.py` & `pysmali-0.2.0/smali/__init__.py`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.3/smali/base.py` & `pysmali-0.2.0/smali/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,23 +9,33 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
+from __future__ import annotations
+
 __doc__ = """
 Basic component classes when working with the Smali language.
 """
 
 import re
 
 from enum import Enum, IntFlag
 
-__all__ = ["AccessType", "Token", "Line", "Type", "smali_value", "SmaliValueProxy"]
+__all__ = [
+    "AccessType",
+    "Token",
+    "Line",
+    "smali_value",
+    "is_type_descriptor",
+    "Signature",
+    "SVMType",
+]
 
 
 class AccessType(IntFlag):
     """Contains all access modifiers for classes, fields, methods and annotations.
 
     There is also a possibility to use values of this class with an ``in``
     statement:
@@ -324,112 +334,107 @@
                 start = end + 1
 
             end = cleaned.find(sep, end + 1)
         elements.append(cleaned[start:])
         return elements
 
 
-class Type:
-    """Basic type definition that can handle both class and method types."""
+class Signature:
+    """Internal class to encapsulate method signatures."""
 
     CLINIT = "<clinit>"
     """Static block initializer"""
 
     INIT = "<init>"
     """Constructor method"""
 
-    def __init__(self, signature: str) -> None:
-        self.__signature = signature.strip()
-        if isinstance(signature, type):
-            self.__signature = f"{signature.__module__}.{signature.__name__}"
-
-    @property
-    def descriptor(self) -> str:
-        """Returns the type descriptor of this type.
-
-        :return: the type descriptor used in the DVM (e.g. "Lcom/example/ABC;")
-        :rtype: str
-        """
-        name = self.__signature
-        if SmaliValueProxy.RE_TYPE_VALUE.match(name):
-            return name
-
-        if name.startswith("["):
-            idx = name.rfind("[")
-            prefix = name[:idx]
-            if not name.endswith(";") and name not in "ZCBSIFVJD":
-                return prefix + f"L{name[idx+1:].replace('.', '/')};"
-
-            return prefix + f"{name[idx+1:].replace('.', '/')}"
-
-        name = f"{name.replace('.', '/')}"
-        if name[-1] != ";" and name not in "ZCBSIFVJD":
-            name = f"L{name};"
-        return name
+    def __init__(self, __signature: str | SVMType) -> None:
+        self.__signature = str(__signature)
+        self.__params = None
+        self.__return_type = None
+        self.__name = None
 
     @property
-    def dim(self) -> int:
-        """Returns the amount of array dimensions.
-
-        :return: the amount of array dimensions.
-        :rtype: int
-        """
-        return self.__signature.count("[")
+    def sig(self) -> str:
+        """Returns the fully qualified signature string.
 
-    @property
-    def type_name(self) -> str:
-        """Returns the type name without 'L' and ';'
+        >>> s = Signature("<init>(II)V")
+        >>> s.sig
+        '<init>(II)V'
 
-        :return: the type name
+        :return: the input string
         :rtype: str
         """
-        if not SmaliValueProxy.RE_TYPE_VALUE.match(self.__signature):
-            return self.__signature
-        name = self.__signature.lstrip("[").replace(".", "/")
-        return name.lstrip("L").rstrip(";")
+        return self.__signature
 
     @property
-    def class_name(self) -> str:
-        """Returns the Smali class name equivalent to Smali class names.
-
-        :return: the class name (e.g. "com.example.ABC")
-        :rtype: str
-        """
-        return self.type_name.replace("/", ".").replace("[", "")
-
-    def get_method_name(self) -> str:
+    def name(self) -> str:
         """Returns the method name
 
+        >>> s = Signature("Lcom/example/Class;->getLength(Ljava/lang/String;)I")
+        >>> s.name
+        'getLength'
+
         :return: the absolute method name
         :rtype: str
         """
+        if self.__name:
+            return self.__name
+
         idx = self.__signature.find("(")
         if idx == -1:
             raise TypeError(
                 f"Invalid method signature: could not find name ({self.__signature})"
             )
 
-
         name = self.__signature[:idx]
         if "->" in name:
-            name = name[name.find("->") + 2:]
+            name = name[name.find("->") + 2 :]
         # Handle bracket names if not <clinit> or <init>
-        if name in (Type.INIT, Type.CLINIT):
+        if name in (Signature.INIT, Signature.CLINIT):
             return name
 
         return name.rstrip(">").lstrip("<")
 
-    def get_method_params(self) -> list:
-        """Returns the method parameter internal names.
+    @property
+    def declaring_class(self) -> SVMType | None:
+        """Returns the :class:`SVMType` of the method's declaring class.
+
+        >>> s1 = Signature("Lcom/example/Class;-><init>(II)V")
+        >>> str(s1.declaring_class)
+        'Lcom/example/Class;'
+        >>> s2 = Signature("<init>(II)V")
+        >>> str(s2.declaring_class)
+        'None'
+
+        :return: the method's declaring class
+        :rtype: SVMType | None
+        """
+        if "->" not in self.sig:
+            return None  # no class defined
+
+        return SVMType(self.sig.split("->")[0])
+
+    @property
+    def parameter_types(self) -> list[SVMType]:
+        """Returns the method parameter types.
+
+        >>> s = Signature("<init>(II)V")
+        >>> params: list[SVMType] = s.parameter_types
+        >>> [str(x) for x in params]
+        ["I", "I"]
 
         :return: the method parameters
         :rtype: list
         """
+        if self.__params:
+            return self.__params
+
         start = self.__signature.find("(")
-        end = self.__signature.find(")") + 1
+        end = self.__signature.find(")")  # we don't want the closing brace
         if start == -1 or end == -1:
             raise TypeError("Invalid method signature")
 
         params = self.__signature[start + 1 : end]
         if not params:
             return []
 
@@ -439,244 +444,312 @@
         for char in params:
             current_param = f"{current_param}{char}"
 
             if char == "L":
                 is_type_def = True
                 continue
 
-            if char == "[" or is_type_def:
-                continue
-
             if char == ";":
+                # This check has to be made before validating whether
+                # the current param is a custom type, otherwise the
+                # whole string would be returned. See issue #3
                 is_type_def = False
 
-            param_list.append(current_param)
+            if char == "[" or is_type_def:
+                continue
+
+            param_list.append(SVMType(current_param))
             current_param = ""
 
         if current_param:
-            param_list.append(current_param)
-        return param_list
+            param_list.append(SVMType(current_param))
 
-    def get_method_return_type(self) -> str:
+        self.__params = param_list
+        return self.__params
+
+    @property  # lazy
+    def return_type(self) -> SVMType:
         """Retrieves the method's return type
 
+        >>> s = Signature("<init>(II)V")
+        >>> str(s.return_type) # returns a SVMType instance
+        'V'
+
         :raises TypeError: if there is no valid return type
         :return: the return type's descriptor
         :rtype: str
         """
-        end = self.__signature.find(")")
-        if end == -1:
-            raise TypeError("Invalid method signature")
-        return self.__signature[end + 1 :]
+        if not self.__return_type:
+            end = self.__signature.find(")")
+            if end == -1:
+                raise TypeError("Invalid method signature")
+            self.__return_type = SVMType(self.__signature[end + 1 :])
+
+        return self.__return_type
+
+    @property
+    def descriptor(self) -> str:
+        """Returns the method descriptor of this signature
+
+        >>> s = Signature("<init>(II)V")
+        >>> s.descriptor
+        '(II)V'
+
+        :raises ValueError: if there is no descriptor
+        :return: the method's descriptor string
+        :rtype: str
+        """
+        idx = self.sig.find("(")
+        if idx == -1:
+            raise ValueError("Invalid method signature - expected '('")
+
+        return self.sig[idx:]
 
     def __str__(self) -> str:
-        return self.__signature
+        return self.sig
+
+    def __repr__(self) -> str:
+        return f"Signature(\"{self.__signature}\")"
+
+
+class SVMType:
+    class TYPES(Enum):
+        """Represents the classification of a type descriptor."""
+        ARRAY = 1
+        PRIMITIVE = 2
+        CLASS = 3
+        METHOD = 4
+        UNKNOWN = 5
+
+    def __init__(self, __type: str) -> None:
+        self.__class = SVMType.TYPES.UNKNOWN
+        self.__dim = __type.count("[")
+        self.__type = self._clean(str(__type))
+        self.__array_type = None
+        if self.dim > 0 and not self.is_signature():
+            self.__class = SVMType.TYPES.ARRAY
+            self.__array_type = SVMType(self.__type.replace("[", ""))
+
+    def _clean(self, __type: str) -> str:
+        # 1. check if we have a primitive type:
+        if re.match(r"\[*[ZCBSIFVJD]$", __type):
+            self.__class = SVMType.TYPES.PRIMITIVE
+            return __type
+
+        # 2. perform normalization
+        value = __type.replace(".", "/")
+        if "(" in value:
+            # TODO: how to handle malformed method signatures
+            self.__class = SVMType.TYPES.METHOD
+            return value
+
+        # 3. Perform class normalization
+        idx = value.rfind("[") + 1
+        if value[idx] != "L":
+            if self.dim > 0:
+                value = f"{value[:idx]}L{value[idx]}"
+            else:
+                value = f"L{value}"
+
+        if not value.endswith(";"):
+            value = f"{value};"
+
+        self.__class = SVMType.TYPES.CLASS
+        return value
+
+    def __str__(self) -> str:
+        return self.__type
 
     def __repr__(self) -> str:
-        return f"<Type sig='{self.__signature}'>"
+        return f"SVMType(\"{self.__type}\")"
 
-def smali_value(value: str) -> "SmaliValueProxy":
+    def is_signature(self) -> bool:
+        """Returns whether this type instance is a method signature.
+
+        >>> t = SVMType("<init>(II)V")
+        >>> t.is_signature()
+        True
+
+        :return: True, if this instance represents a method signature
+        :rtype: bool
+        """
+        return self.__class == SVMType.TYPES.METHOD
+
+    @property
+    def signature(self) -> Signature | None:
+        """Creates a :class:`Signature` object from this type instance.
+
+        :return: the signature object or nothing if this type does not represent a
+                 method signature.
+        :rtype: Signature | None
+        """
+        return None if self.svm_type != SVMType.TYPES.METHOD else Signature(self.__type)
+
+    @property
+    def dim(self) -> int:
+        """Returns the amount of array dimensions.
+
+        :return: the amount of array dimensions.
+        :rtype: int
+        """
+        return self.__dim
+
+    @property
+    def svm_type(self) -> SVMType.TYPES:
+        """Returns the descriptor classification (ARRAY, PRIMITIVE, METHOD or CLASS)
+
+        :return: the classification of this type instance
+        :rtype: SVMType.TYPES
+        """
+        return self.__class
+
+    @property
+    def array_type(self) -> SVMType:
+        """Returns the underlying array type (if any)
+
+        >>> array = SVMType("[[B")
+
+        :return: the underlying array type instance
+        :rtype: SVMType
+        """
+        return self.__array_type
+
+    @property
+    def pretty_name(self) -> str:
+        """Returns a prettified version of the class name.
+
+        >>> array = SVMType("[[Lcom/example/Class;")
+        >>> array.pretty_name
+        '[[com.example.Class'
+
+        :return: full name without ``L`` and ``;``; ``/`` is replaced by a dot.
+        :rtype: str
+        """
+        value = str(self)
+        return re.sub(r"\/|(->)", ".", value.replace("L", "").replace(";", ""))
+
+    @property
+    def dvm_name(self) -> str:
+        """Returns the DVM representation of this type descriptor.
+
+        >>> cls = SVMType("Lcom/example/Class;")
+        >>> cls.dvm_name
+        'com/example/Class'
+
+        :return: the full name without ``L`` and ``;``.
+        :rtype: str
+        """
+        value = str(self)
+        return re.sub(r"[L;]", "", value)
+
+    @property
+    def full_name(self) -> str:
+        """Returns the full name of this type descriptor (input value)
+
+        >>> cls = SVMType("com.example.Class")
+        >>> cls.full_name
+        'Lcom/example/Class;'
+
+        :return: the full name
+        :rtype: str
+        """
+        return str(self)
+
+    @property
+    def simple_name(self) -> str:
+        """Returns only the class name (not applicable to method signatures)
+
+        :return: the class' name
+        :rtype: str
+        """
+        return self.pretty_name.split(".")[-1]
+
+
+def smali_value(value: str) -> int | float | str | SVMType | bool:
     """Parses the given string and returns its Smali value representation.
 
     :param value: the value as a string
     :type value: str
     :raises ValueError: if it has no valid Smali type
     :return: the Smali value representation
-    :rtype: SmaliValueProxy
+    :rtype: int | float | str | SVMType | bool
     """
-    sm_value = SmaliValueProxy()
-    sm_value.value = value
-    sm_value.actual_value = None
-    for i, entry in enumerate(SmaliValueProxy.TYPE_MAP):
+    actual_value = None
+    for i, entry in enumerate(TYPE_MAP):
         matcher, wrapper = entry
-        if matcher.match(sm_value.value):
+        if matcher.match(value):
             if i <= 3:  # hex value possible
-                hex_val = SmaliValueProxy.RE_HEX_VALUE.match(value) is not None
+                hex_val = RE_HEX_VALUE.match(value) is not None
                 if not hex_val:
-                    sm_value.actual_value = wrapper(value)
+                    actual_value = wrapper(value)
                 else:
-                    sm_value.actual_value = wrapper(value, base=16)
+                    actual_value = wrapper(value, base=16)
             else:
-                sm_value.actual_value = wrapper(value)
+                actual_value = wrapper(value)
             break
 
     # Handling of null values is not implemented yet
-    if sm_value.actual_value is None:
+    if actual_value is None:
         raise ValueError(f"Could not find any matching primitive type for {value}")
 
-    sm_locals = {}
-    for key in __smali_builtins__:
-        if hasattr(sm_value.actual_value, key):
-            sm_locals[key] = getattr(sm_value.actual_value, key)
-
-    vars(sm_value).update(sm_locals)
-    return sm_value
-
-
-class SmaliValueProxy:
-    """Wrapper class for primitives in Smali.
-
-    Use this class to retrieve the actual primitiva value for a parsed
-    source code snippet. As this class overrides most of the internal
-    special functions, objects of this class can be used as regualar
-    strings or numeric values:
-
-    >>> value = SmaliValue("1234")
-    1234
-    >>> value += 1
-    1235
-
-    The same behaviour applies to parsed strings (note that you need
-    quotation marks):
-
-    >>> string = SmaliValue('"Hello World"')
-    'Hello World'
-    >>> len(string)
-    11
-    """
+    return actual_value
 
-    RE_INT_VALUE = re.compile(r"[\-\+]?(0x)?[\dabcdefABCDEF]+$")
-    """Pattern for ``int`` values."""
+RE_INT_VALUE = re.compile(r"[\-\+]?(0x)?[\dabcdefABCDEF]+$")
+"""Pattern for ``int`` values."""
 
-    RE_BYTE_VALUE = re.compile(r"[\-\+]?(0x)?[\dabcdefABCDEF]+t$")
-    """Pattern for ``byte`` values."""
+RE_BYTE_VALUE = re.compile(r"[\-\+]?(0x)?[\dabcdefABCDEF]+t$")
+"""Pattern for ``byte`` values."""
 
-    RE_SHORT_VALUE = re.compile(r"[\-\+]?(0x)?[\dabcdefABCDEF]+s$")
-    """Pattern for ``short`` values."""
+RE_SHORT_VALUE = re.compile(r"[\-\+]?(0x)?[\dabcdefABCDEF]+s$")
+"""Pattern for ``short`` values."""
 
-    RE_FLOAT_VALUE = re.compile(r"[\-\+]?\d+\.\d+f$")
-    """Pattern for ``float`` values."""
-
-    RE_DOUBLE_VALUE = re.compile(r"[\-\+]?\d+\.\d+")
-    """Pattern for ``double`` values."""
-
-    RE_LONG_VALUE = re.compile(r"[\-\+]?(0x)?[\dabcdefABCDEF]+l$")
-    """Pattern for ``long`` values."""
-
-    RE_CHAR_VALUE = re.compile(r"^'.*'$")
-    """Pattern for ``char`` values."""
-
-    RE_STRING_VALUE = re.compile(r'^".*"$')
-    """Pattern for ``String`` values."""
-
-    RE_TYPE_VALUE = re.compile(r"\[*((L\S*;$)|([ZCBSIFVJD])$)")  # NOQA
-    """Pattern for type descriptors."""
-
-    RE_BOOL_VALUE = re.compile(r"true|false")
-    """Pattern for ``boolean`` values."""
-
-    RE_HEX_VALUE = re.compile(r"0x[\dabcdefABCDEF]+")
-    """Pattern for integer values."""
-
-    TYPE_MAP: list = [
-        (RE_SHORT_VALUE, lambda x, **kw: int(x[:-1], **kw)),
-        (RE_LONG_VALUE, lambda x, **kw: int(x[:-1], **kw)),
-        (RE_BYTE_VALUE, lambda x, **kw: int(x[:-1], **kw)),
-        (RE_INT_VALUE, int),
-        (RE_BOOL_VALUE, lambda x: str(x).lower() == "true"),
-        (RE_FLOAT_VALUE, lambda x: float(x[:-1])),
-        (RE_DOUBLE_VALUE, lambda x: float(x[:-1])),
-        (RE_CHAR_VALUE, lambda x: str(x[1:-1])),
-        (RE_STRING_VALUE, lambda x: str(x[1:-1])),
-        (RE_TYPE_VALUE, Type),
-    ]
-    """Defines custom handlers for actual value defintions
+RE_FLOAT_VALUE = re.compile(r"[\-\+]?\d+\.\d+f$")
+"""Pattern for ``float`` values."""
 
-    :meta private:
-    """
+RE_DOUBLE_VALUE = re.compile(r"[\-\+]?\d+\.\d+")
+"""Pattern for ``double`` values."""
 
-    value: str
-    """The initial source code value (string)"""
+RE_LONG_VALUE = re.compile(r"[\-\+]?(0x)?[\dabcdefABCDEF]+l$")
+"""Pattern for ``long`` values."""
 
-    actual_value = None
-    """The actual value of any type"""
+RE_CHAR_VALUE = re.compile(r"^'.*'$")
+"""Pattern for ``char`` values."""
 
-    @staticmethod
-    def is_type_descriptor(value: str) -> bool:
-        """Returns whether the given value is a valid type descriptor.
+RE_STRING_VALUE = re.compile(r'^".*"$')
+"""Pattern for ``String`` values."""
 
-        :param value: the value to check
-        :type value: str
-        :return: True, if the value is a valid type descriptor
-        :rtype: bool
-        """
-        return SmaliValueProxy.RE_TYPE_VALUE.match(value) is not None
+RE_TYPE_VALUE = re.compile(r"\[*((L\S*;$)|([ZCBSIFVJD])$)")  # NOQA
+"""Pattern for type descriptors."""
 
+RE_BOOL_VALUE = re.compile(r"true|false")
+"""Pattern for ``boolean`` values."""
 
-####################################################################################
-# INTERNAL
-####################################################################################
-
-__smali_builtins__ = [
-    "__contains__", "__eq__", "__ne__", "__len__", "__str__", "__next__", "__bool__",
-    "__repr__", "__str__", "__bytes__", "__format__", "__lt__", "__le__", "__eq__",
-    "__ne__", "__gt__", "__ge__", "__hash__", "__bool__", "__len__", "__length_hint__",
-    "__getitem__", "__setitem__", "__delitem__", "__missing__", "__iter__", "__reversed__",
-    "__contains__", "__add__", "__sub__", "__mul__", "__truediv__", "__floordiv__",
-    "__mod__", "__divmod__", "__lshift__", "__rshift__", "__and__", "__xor__", "__or__",
-    "__radd__", "__rsub__", "__rmul__", "__rtruediv__", "__rfloordiv__", "__rmod__",
-    "__rdivmod__", "__rlshift__", "__rrshift__", "__rand__", "__rxor__", "__ror__",
-    "__neg__", "__pos__", "__abs__", "__invert__", "__complex__", "__int__", "__float__",
-    "__index__", "__trunc__", "__floor__", "__ceil__",
-]
+RE_HEX_VALUE = re.compile(r"0x[\dabcdefABCDEF]+")
+"""Pattern for integer values."""
 
-__smali_specials__ = [
-    ("__iadd__", lambda x, y: x.actual_value + y.actual_value),
-    ("__isub__", lambda x, y: x.actual_value - y.actual_value),
-    ("__imul__", lambda x, y: x.actual_value * y.actual_value),
-    ("__itruediv__", lambda x, y: x.actual_value / y.actual_value),
-    ("__ifloordiv__", lambda x, y: x.actual_value // y.actual_value),
-    ("__imod__", lambda x, y: x.actual_value % y.actual_value),
-    ("__ilshift__", lambda x, y: x.actual_value << y.actual_value),
-    ("__irshift__", lambda x, y: x.actual_value >> y.actual_value),
-    ("__iand__", lambda x, y: x.actual_value & y.actual_value),
-    ("__ixor__", lambda x, y: x.actual_value ^ y.actual_value),
-    ("__ior__", lambda x, y: x.actual_value | y.actual_value),
+TYPE_MAP: list = [
+    (RE_SHORT_VALUE, lambda x, **kw: int(x[:-1], **kw)),
+    (RE_LONG_VALUE, lambda x, **kw: int(x[:-1], **kw)),
+    (RE_BYTE_VALUE, lambda x, **kw: int(x[:-1], **kw)),
+    (RE_INT_VALUE, int),
+    (RE_BOOL_VALUE, lambda x: str(x).lower() == "true"),
+    (RE_FLOAT_VALUE, lambda x: float(x[:-1])),
+    (RE_DOUBLE_VALUE, lambda x: float(x[:-1])),
+    (RE_CHAR_VALUE, lambda x: str(x[1:-1])),
+    (RE_STRING_VALUE, lambda x: str(x[1:-1])),
+    (RE_TYPE_VALUE, SVMType),
 ]
+"""Defines custom handlers for actual value defintions
 
+:meta private:
+"""
 
-def __wrap_args__(self, target: str, *args):
-    """Tries to wrap ``SmalivalueProxy`` objects before calling the special method.
+def is_type_descriptor(value: str) -> bool:
+    """Returns whether the given value is a valid type descriptor.
 
-    :param target: the method to call
-    :type target: str
+    :param value: the value to check
+    :type value: str
+    :return: True, if the value is a valid type descriptor
+    :rtype: bool
     """
-    if len(args) == 0:
-        return self.__dict__[target](*args)
-
-    new_args = []
-    for val in args:
-        # Built-in types will throw errors when using executing
-        # SmaliValueProxy * SmaliValueProxy, so we have to convert
-        # the proxy argument by using the actual value
-        if isinstance(val, SmaliValueProxy):
-            new_args.append(val.actual_value)
-        else:
-            new_args.append(val)
-
-    return self.__dict__[target](*new_args)
-
-
-for method in __smali_builtins__:
-    setattr(
-        SmaliValueProxy,
-        method,
-        lambda self, *args, method=method: __wrap_args__(self, method, *args),
-    )
-
-
-def __wrap_special__(instance, actual_val, val, funct):
-    funct(actual_val, val)
-    return instance
-
-
-for method, func in __smali_specials__:
-    setattr(
-        SmaliValueProxy,
-        method,
-        lambda self, val, func=func: __wrap_special__(
-            self, self.actual_value, val, func
-        ),
-    )
+    return RE_TYPE_VALUE.match(value) is not None
 
-del method
-del func
```

### Comparing `pysmali-0.1.3/smali/bridge/__init__.py` & `pysmali-0.2.0/smali/bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.3/smali/bridge/errors.py` & `pysmali-0.2.0/smali/bridge/errors.py`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.3/smali/bridge/executor.py` & `pysmali-0.2.0/smali/bridge/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 import struct
 
-from smali import SmaliValue, Type
+from smali import SmaliValue, SVMType
 from smali.opcode import *  # noqa
 from smali.bridge.frame import Frame
 from smali.bridge.errors import ExecutionError
 from smali.bridge.lang import SmaliObject
 from smali.bridge.objects import Object, Class
 
 cache = {}
@@ -369,21 +369,22 @@
         instance.init()
 
         self.frame[register] = instance
 
 
 @opcode_executor()
 def new_array(self: Executor, dest: str, count_register: str, descriptor: str):
-    cls_name = Type(descriptor).class_name
+    cls_type = SVMType(descriptor)
     values = [None] * self.frame[count_register]
-    if cls_name in "BSIJ":  # number
-        values = [0] * self.frame[count_register]
+    if cls_type.svm_type == SVMType.TYPES.PRIMITIVE:
+        if cls_type.simple_name in "BSIJ":  # number
+            values = [0] * self.frame[count_register]
 
-    elif cls_name in "FD":  # floating point
-        values = [0.0] * self.frame[count_register]
+        elif cls_type.simple_name in "FD":  # floating point
+            values = [0.0] * self.frame[count_register]
 
     self.frame[dest] = values
 
 
 @opcode_executor(map_to=[INSTANCE_OF])
 def check_cast(self: Executor, dest: str, descriptor: str):
     src_class = self.frame[dest]
```

### Comparing `pysmali-0.1.3/smali/bridge/frame.py` & `pysmali-0.2.0/smali/bridge/frame.py`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.3/smali/bridge/lang.py` & `pysmali-0.2.0/smali/bridge/lang.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
+from __future__ import annotations
+
 __doc__ = """
 The module ``lang`` of the provided Smali bridge defines classes that
 can be used to mimic Java's reflection at runtime of the :class:`SmaliVM`.
 
 All members of a Smali class inherit functionalities of ``__eq__``,
 ``__ne__``, as well as hash value calculation and string representation
 of objects.
@@ -29,15 +31,15 @@
 
 """
 
 import re
 
 from io import UnsupportedOperation
 
-from smali.base import AccessType, SmaliValueProxy, Type
+from smali.base import AccessType, SVMType, Signature
 from smali.bridge.errors import NoSuchMethodError, NoSuchFieldError, NoSuchClassError
 
 __all__ = [
     "SmaliMember",
     "SmaliAnnotation",
     "SmaliField",
     "SmaliMethod",
@@ -55,33 +57,37 @@
 
     __parent: "SmaliMember"
     """The parent of this member."""
 
     __signature: str
     """The qualified signature of this member"""
 
+    __type: SVMType
+
     __modifiers: int
     """The member's visibility modifiers."""
 
     __annotations: dict
     """All annotations of this member. The will be stored in
     a type-2-object mapping.
 
     >>> member.annotations
     { 'Ljava/lang/Deprecated;': [<SmaliAnnotation at 0x...>, ...] }
     """
 
     def __init__(
         self,
+        type_: str,
         parent: "SmaliMember",
         signature: str,
         modifiers: int,
         base_class: type,
         annotations: list = None,
     ) -> None:
+        self.__type = SVMType(str(type_))
         self.__signature = signature
         self.__modifiers = modifiers
         self.__annotations = annotations or []
         if self.__class__ != base_class:
             raise TypeError(f"{base_class.__name__} cannot be sub-classed!")
 
         self.__parent = parent
@@ -92,29 +98,29 @@
         """Returns whether the given annotation is present.
 
         :param a_type: the annotation's type descriptor
         :type a_type: str
         :return: True, if present; False otherwise
         :rtype: bool
         """
-        if isinstance(a_type, Type):
-            a_type = a_type.descriptor
+        if isinstance(a_type, SVMType):
+            a_type = str(a_type)
 
         return isinstance(a_type, str) and a_type in self.__annotations
 
     def get_annotations(self, a_type: str) -> list:
         """Returns all declared annnotations of the given type.
 
         :param a_type: the annotation's type descriptor
-        :type a_type: str | Type
+        :type a_type: str | SVMType
         :return: a list of declared annotations
         :rtype: list
         """
-        if isinstance(a_type, Type):
-            a_type = a_type.descriptor
+        if isinstance(a_type, SVMType):
+            a_type = str(a_type)
 
         if not isinstance(a_type, str):
             # to prevent errors, the output is non-null
             return []
 
         return self.__annotations.get(a_type, [])
 
@@ -150,27 +156,36 @@
         """The declared annotations of this member
 
         :return: all declared annotations
         :rtype: list
         """
         return self.__annotations
 
+    @property
+    def type(self) -> SVMType:
+        """Returns the type of this member
+
+        :return: the type instance
+        :rtype: :class:`SVMType`
+        """
+        return self.__type
+
     def __eq__(self, __o: object) -> bool:
         if isinstance(__o, self.__class__):
             return __o.signature == self.__signature
         return super().__eq__(__o)
 
     def __ne__(self, __o: object) -> bool:
         return not self.__eq__(__o)
 
     def __hash__(self) -> int:
-        return self.__signature.__hash__()
+        return hash(str(self.type))
 
     def __repr__(self) -> str:
-        return f"<{self.__class__.__name__} '{self.signature}' at {id(self):#x}"
+        return f"<{self.__class__.__name__} '{self.signature}' at {id(self):#x}>"
 
     def __str__(self) -> str:
         return f"<{self.__class__.__name__} {self.signature}>"
 
 
 class SmaliAnnotation(SmaliMember):
     """Class that represents Smali annotations (and subannotations).
@@ -196,21 +211,23 @@
     """
 
     attr: dict
     """The attributes of this annotation (key-value map)."""
 
     def __init__(
         self,
-        parent,
+        parent: SmaliMember,
         signature: str,
         modifiers: int,
         annotations: list = None,
-        attr: dict = None,
+        attr=None,
     ) -> None:
-        super().__init__(parent, signature, modifiers, SmaliAnnotation, annotations)
+        super().__init__(
+            signature, parent, signature, modifiers, SmaliAnnotation, annotations
+        )
         self.attr = attr or {}
 
     def __getitem__(self, key: str) -> object:
         return self.attr.get(key, None)
 
     def __setitem__(self, key: str, value):
         self.attr[key] = value
@@ -225,70 +242,57 @@
     :param signature: the field's signature (``name:type``)
     :type signature: str
     :param modifiers: the field's access modifiers
     :type modifiers: int
     :param annotations: the field's annotations, defaults to None
     :type annotations: list, optional
     :param value: the field's value, defaults to None
-    :type value: :class:`SmaliValueProxy`, optional
+    :type value: int | float | str | SVMType | bool, optional
     """
 
     __name: str
     """The field's name"""
 
-    __smali_type: Type
-    """The field's type (Smali type descriptor)"""
-
-    __value: SmaliValueProxy
+    __value: int | float | str | SVMType | bool
     """Stores the actual value of this field"""
 
     def __init__(
         self,
+        _type: str,
         parent,
         signature: str,
         modifiers: int,
         name: str,
-        smali_type: Type,
         annotations: list = None,
-        value: SmaliValueProxy = None,
+        value=None,
     ) -> None:
-        super().__init__(parent, signature, modifiers, SmaliField, annotations)
+        super().__init__(_type, parent, signature, modifiers, SmaliField, annotations)
         self.__value = value
-        self.__smali_type = smali_type
         self.__name = name
 
     @property
-    def value(self) -> SmaliValueProxy:
+    def value(self) -> int | float | str | SVMType | bool:
         """Returns the value of this field.
 
         :return: the value as a :class:`SmaliValue`
-        :rtype: :class:`SmaliValueProxy`
+        :rtype: int | float | str | SVMType | bool
         """
         return self.__value
 
     @value.setter
-    def value(self, new_value: SmaliValueProxy):
+    def value(self, new_value: int | float | str | SVMType | bool):
         """Setter for ``self.value``.
 
         :param new_value: the new value to apply
-        :type new_value: :class:`SmaliValueProxy`
+        :type new_value: int | float | str | SVMType | bool
         :raises UnsupportedOperation: if this field can not be modified
         """
         self.__value = new_value
 
     @property
-    def smali_type(self) -> Type:
-        """Returns the type of this field
-
-        :return: the type object
-        :rtype: Type
-        """
-        return self.__smali_type
-
-    @property
     def name(self) -> str:
         """Returns the name of this field
 
         :return: the name
         :rtype: str
         """
         return self.__name
@@ -311,17 +315,17 @@
 
     The instance of the object that defines the method is always
     needed except for static method. They can bbe called with
     ``None`` as the instance parameter.
     """
 
     __smali_params: list = []
-    """The smali parameter types (type descriptor strings)"""
+    """The smali parameter types (:class:`SVMType`)"""
 
-    __smali_return: Type
+    __smali_return: SVMType
     """The return type"""
 
     __name: str
     """The method's name"""
 
     __vm = None
     """The VM that delegates the execution of this method."""
@@ -333,20 +337,29 @@
         self,
         vm,
         parent: "SmaliMember",
         signature: str,
         modifiers: int,
         annotations: list = None,
     ) -> None:
-        super().__init__(parent, signature, modifiers, SmaliMethod, annotations)
+        super().__init__(
+            f"{parent.type}->{signature}",
+            parent,
+            signature,
+            modifiers,
+            SmaliMethod,
+            annotations,
+        )
         self.__vm = vm
-        sig_type = Type(signature)
-        self.name = sig_type.get_method_name()
-        self.smali_params = sig_type.get_method_params()
-        self.smali_return = sig_type.get_method_return_type()
+        sig_type = self.type.signature
+        if not sig_type:
+            raise ValueError(f"Expected a method signature - got {self.type}")
+        self.name = sig_type.name
+        self.smali_params = sig_type.parameter_types
+        self.smali_return = sig_type.return_type
 
     def __call__(self, instance, *args, **kwds) -> object:
         if not self.__vm:
             raise UnsupportedOperation("VM not activated!")
 
         if self.modifiers in AccessType.ABSTRACT:
             raise UnsupportedOperation("Abstract methods cannot e executed!")
@@ -364,28 +377,28 @@
         return self.__name
 
     @name.setter
     def name(self, value: str):
         self.__name = value
 
     @property
-    def parameters(self) -> list:
+    def parameters(self) -> list[SVMType]:
         """Returns the parameters of this method as type descriptor strings
 
         :return: the parameters of this method
         :rtype: list
         """
         return self.__smali_params
 
     @property
-    def return_type(self) -> Type:
+    def return_type(self) -> SVMType:
         """Returns the method's return type
 
         :return: the return type
-        :rtype: Type
+        :rtype: SVMType
         """
         return self.__smali_return
 
     @property
     def locals(self) -> int:
         """Returns the amount of local variables."""
         return self.__locals
@@ -418,23 +431,24 @@
     There is a pre-defined alias for this class named :class:`SmaliMethodBroker` in the .
     same module.
     """
 
     __name: str
     """The method's name"""
 
-    __methods: list
+    __methods: list[SmaliMethod]
     """The methods that can be called."""
 
     def __init__(self, name: str, methods: list) -> None:
         self.__methods = methods or []
         self.__name = name
 
     def __iadd__(self, method: SmaliMethod) -> "_MethodBroker":
         self.__methods.append(method)
+        return self
 
     def __call__(self, instance, *args, **kwds) -> object:
         if len(self.__methods) == 1:
             method = self.__methods[0]
             return method(instance, *args, **kwds)
 
         returns = kwds.get("returns", None)
@@ -458,19 +472,19 @@
                 if returns is None:
                     raise NoSuchMethodError(
                         f"Attempted to call {self.__name}() with invalid arguments"
                     )
                 # Filter by return type
                 if not returns:
                     targets = list(
-                        filter(lambda x: (x.return_type.descriptor != "V"), targets)
+                        filter(lambda x: (str(x.return_type) != "V"), targets)
                     )
                 else:
                     targets = list(
-                        filter(lambda x: (x.return_type.descriptor == "V"), targets)
+                        filter(lambda x: (str(x.return_type) == "V"), targets)
                     )
 
                 # We found one method, call it!
                 if len(targets) == 1:
                     method = targets[0]
                     return method(instance, *args, **kwds)
 
@@ -494,14 +508,17 @@
 
     def __repr__(self) -> str:
         return f"<MethodBroker of '{self.__name}' at {id(self):#x}"
 
     def __iter__(self):
         return iter(self.__methods)
 
+    def __getitem__(self, idx):
+        return self.__methods[idx]
+
 
 SmaliMethodBroker = _MethodBroker
 """Public alias for method broker objects"""
 
 
 class SmaliClass(SmaliMember):
     """Internal class for storing imported class data.
@@ -588,107 +605,125 @@
 
     __simple_name: str
     """The simple name of this class"""
 
     __name: str
     """The full name of this class with dots (``.``)"""
 
-    __methods: dict
+    __methods: dict[str, _MethodBroker]
     """All methods that can be executed are stored in a separate dict.
 
     The values are instances of ``_Methodbroker``.
     """
 
-    __fields: dict
+    __fields: dict[str, SmaliField]
     """All fields if this class"""
 
-    __classes: dict
+    __classes: dict[str, SmaliClass]
     """All inner classes of this class"""
 
-    __super: str
+    __super: SVMType
     """The class descriptor of the super class"""
 
-    __implements: list
+    __implements: list[SVMType]
     """The list of implemented interfaces."""
 
     def __init__(
         self,
         parent: "SmaliMember",
         signature: str,
         modifiers: int,
         annotations: list = None,
     ) -> None:
-        super().__init__(parent, signature, modifiers, SmaliClass, annotations)
-        sig_type = Type(signature)
-        self.__name = sig_type.class_name
-        self.__simple_name = self.__name.split(".")[-1]
+        super().__init__(
+            signature, parent, signature, modifiers, SmaliClass, annotations
+        )
+        self.__name = self.type.pretty_name
+        self.__simple_name = self.type.simple_name
         self.__fields = {}
         self.__methods = {}
         self.__super = None
         self.__implements = []
+        self.__classes = {}
 
     @property
     def simple_name(self) -> str:
         """Returns the name of this class.
 
         :return: the class name
         :rtype: str
         """
         return self.__simple_name
 
     @property
     def name(self) -> str:
-        """Returns the name of this class with the package"""
+        """Returns the name of this class with the package (with dots)"""
         return self.__name
 
     @name.setter
     def name(self, value: str):
         """Setter for the name property.
 
         :param value: the name of this class
         :type value: str
         """
         self.__name = value
 
     @property
-    def inner_classes(self) -> dict:
+    def inner_classes(self) -> dict[str, SmaliClass]:
         """Returns all inner classes
 
-        :return: _description_
+        :return: all defined inner classes
         :rtype: dict
         """
         return self.__classes
 
     @property
-    def super_cls(self) -> str:
+    def super_cls(self) -> SVMType:
         """Returns the super class of this class
 
         :return: the super class name
-        :rtype: str
+        :rtype: SVMType | SmaliClass
         """
         return self.__super
 
     @super_cls.setter
     def super_cls(self, value):
         """Setter for the super-class name
 
         :param value: the new name
         :type value: str
         """
         self.__super = value
 
     @property
-    def interfaces(self) -> list:
+    def interfaces(self) -> list[SVMType]:
         """Returns all implemented interfaces (type descriptors)
 
         :return: all implemented interfacea in a list
         :rtype: list
         """
         return self.__implements
 
+    def get_declared_methods(self, access_type: AccessType = None) -> list[SmaliMethod]:
+        """Returns all declared methods in this class,
+
+        :param access_type: an extra filter, defaults to None
+        :type access_type: AccessType, optional
+        :return: the list of defined smali methods
+        :rtype: list[SmaliMethod]
+        """
+        result = []
+        for name in self.__methods:
+            for method in self.__methods[name]:
+                if access_type is None or method.modifiers in access_type:
+                    result.append(method)
+
+        return result
+
     def method(self, signature: str) -> SmaliMethod:
         """Searches for the given method signature or name.
 
         :param signature: the name or signature of the method
         :type signature: str
         :raises NoSuchMethodError: if no method with a name or wignature
                                    equal to the given could be found
@@ -697,16 +732,15 @@
         :rtype: SmaliMethod | SmaliMethodBroker
         """
         for name, broker in self.__methods.items():
             if name == signature:
                 return broker
 
             for method in broker:
-                # See __eq__() in SmaliMember
-                if method == signature:
+                if method.signature == signature:
                     return method
 
         raise NoSuchMethodError(f'Method with signature "{signature}" not found')
 
     def field(self, name: str) -> SmaliField:
         """Returns the field with the given name.
```

### Comparing `pysmali-0.1.3/smali/bridge/objects.py` & `pysmali-0.2.0/smali/bridge/objects.py`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.3/smali/bridge/vm.py` & `pysmali-0.2.0/smali/bridge/vm.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,31 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
+from __future__ import annotations
+
 __doc__ = """
 Implementation of a simple Smali emulator named *SmaliVM*. It supports
 execution of small code snippets as well as the execution of whole
 class files.
 
 Debugging can be done by providing a :class:`DebugHandler` and enabling the
 debug-option wihtin the VM object. It is also possible to use a custom
 ``ClassLoader`` to load or define new classes.
 """
 
+from io import IOBase
 from abc import ABCMeta, abstractmethod
 
 from smali import SmaliValue, opcode
-from smali.base import Type, AccessType
+from smali.base import AccessType, SVMType
 from smali.reader import SmaliReader
 from smali.visitor import ClassVisitor, MethodVisitor, FieldVisitor, AnnotationVisitor
 from smali.bridge.lang import (
     SmaliClass,
     SmaliMethod,
     SmaliField,
     SmaliAnnotation,
@@ -57,29 +60,29 @@
 ]
 
 
 class ClassLoader(metaclass=ABCMeta):
     """Abstract base class for SmaliClassLoader"""
 
     @abstractmethod
-    def define_class(self, source: bytes) -> SmaliClass:
+    def define_class(self, source: bytes | str | IOBase) -> SmaliClass:
         """Defines a new SmaliClass by parsing the given source file.
 
         :param source: the source code
         :type source: bytes | str
         :return: the parsed class definition
         :rtype: SmaliClass
         """
 
     @abstractmethod
-    def load_class(self, source: str, init=True, lookup_missing=False) -> SmaliClass:
+    def load_class(self, source: str | bytes | IOBase, init=True, lookup_missing=False) -> SmaliClass:
         """Parses the given source code and initializes the given class if enabled.
 
         :param source: the source code
-        :type source: str | bytes
+        :type source: str | bytes | IOBase
         :param init: whether ``<clinit>`` should be executed, defaults to True
         :type init: bool, optional
         :param lookup_missing: whether missing classes should be searched before parsing
                                can continue, defaults to False
         :type lookup_missing: bool, optional
         :raises NoSuchClassError: if the given class is not defined and ``lookup_missing`` is true
         :raises InvalidOpcodeError: if the parsed opcode is invalid
@@ -107,27 +110,27 @@
 
     classloader: ClassLoader
     """The class loader used to define classes."""
 
     debug_handler: DebugHandler
     """The debug handler to use."""
 
-    executors: dict
+    executors: dict[str, executor.Executor]
     """External executors used to operate on a single opcode."""
 
     use_strict: bool = False
     """Tells the VM to throw exceptions on unkown opcodes."""
 
-    __classes: dict = {}
+    __classes: dict[str, SmaliClass] = {}
     """All classes are stored in a dict
 
     :meta public:
     """
 
-    __frames: dict = {}
+    __frames: dict[int, Frame] = {}
     """Stores all execution frames mapped to their method object
 
     :meta public:
     """
 
     # This map is used to determine which parameters are applied to the right
     # values.
@@ -146,60 +149,62 @@
         str: ("Ljava/lang/String;", "C", "Ljava/lang/Character;"),
         bool: ("Z", "Ljava/lang/Boolean;"),
     }
 
     def __init__(
         self,
         class_loader: ClassLoader = None,
-        executors: dict = executor.cache,
+        executors: dict = None,
         use_strict: bool = False,
     ) -> None:
         self.classloader = _SmaliClassLoader(self) or class_loader
-        self.executors = executors or {}
+        self.executors = executors or executor.cache
         self.use_strict = use_strict
+        self.debug_handler = None
 
-    def new_class(self, cls: SmaliClass):
+    def new_class(self, __class: SmaliClass):
         """Defines a new class that can be accessed globally.
 
         :param cls: the class to be defined
         :type cls: SmaliClass
         """
-        if not cls:
+        if not __class:
             raise ValueError("SmaliClass object is null!")
 
-        self.__classes[cls.signature] = cls
+        self.__classes[__class.signature] = __class
 
     def new_frame(self, method: SmaliMethod, frame: Frame):
         """Creates a new method frame that will be mapped to the method's signature-
 
         :param method: the target method
         :type method: SmaliMethod
         :param frame: the execution frame
         :type frame: Frame
         """
         mhash = hash(method)
         if mhash not in self.__frames:
             self.__frames[mhash] = frame
             frame.vm = self
 
-    def get_class(self, name) -> SmaliClass:
+
+    def get_class(self, name: str) -> SmaliClass:
         """Searches for a class with the given name.
 
         :param name: the class name
         :type name: str
         :raises NoSuchClassError: if no class with the given name is defined
         :return: the defined Smali class
         :rtype: SmaliClass
         """
         if name not in self.__classes:
             raise NoSuchClassError(f'Class "{name}" not defined!')
 
         return self.__classes[name]
 
-    def call(self, method, instance, *args, **kwargs) -> object:
+    def call(self, method: SmaliMethod, instance, *args, **kwargs) -> object:
         """Executes the given method in the given object instance.
 
         Before the method will be executed, there is an input parameter
         check to validate all passed arguments. The required registers
         will be filled automatically.
 
         Debugging is done via the :class:`DebugHandler` that must be set globally
@@ -255,15 +260,15 @@
 
             raise ExecutionError(frame.error)
 
         value = frame.return_value
         frame.reset()
         return value
 
-    def _validate_call(self, method, frame: Frame, args: tuple, kwargs: dict):
+    def _validate_call(self, method: SmaliMethod, frame: Frame, args: tuple, kwargs: dict):
         parameters = method.parameters
 
         registers = {}
         for key, value in kwargs.items():
             if RE_REGISTER.match(key):
                 registers[key] = value
 
@@ -274,26 +279,26 @@
         if len(parameters) != len(registers):
             raise ValueError(
                 "Invalid argument count! - expected %s, got %d"
                 % (len(parameters), len(registers))
             )
 
         for param, register in zip(parameters, registers):
-            param_type = Type(param)
+            param_type: SVMType = param
             # Lookup primitive types
             for primitive, ptypes in self.__type_map.items():
-                if param_type.class_name in ptypes:
+                if param_type.full_name in ptypes:
                     if not isinstance(registers[register], primitive):
                         raise TypeError(
                             "Invalid type for parameter, expected %s - got %s"
                             % (param, type(registers[register]))
                         )
 
-            if param_type.descriptor not in self.__classes:
-                raise NoSuchClassError(f'Class "{param_type.descriptor}" not defined!')
+            if param_type.full_name not in self.__classes:
+                raise NoSuchClassError(f'Class "{param_type}" not defined!')
 
         frame.registers.update(registers)
 
 
 ####################################################################################################
 # INTERNAL
 ####################################################################################################
@@ -446,19 +451,19 @@
         self.smali_class[name] = inner
         return SmaliVMClassReader(self.vm, inner)
 
     def visit_field(
         self, name: str, access_flags: int, field_type: str, value=None
     ) -> FieldVisitor:
         field = SmaliField(
+            field_type,
             self.smali_class,
             f"{name}:{field_type}",
             access_flags,
             name,
-            Type(field_type),
             value=SmaliValue(value) if value else None,
         )
         self.smali_class[name] = field
         return SmaliVMFieldReader(field)
 
     def visit_method(
         self, name: str, access_flags: int, parameters: list, return_type: str
@@ -467,18 +472,18 @@
         method = SmaliMethod(self.vm, self.smali_class, signature, access_flags)
         visitor = SmaliVMMethodReader(method)
         self.vm.new_frame(method, visitor.frame)
         self.smali_class[name] = method
         return visitor
 
     def visit_implements(self, interface: str) -> None:
-        self.smali_class.interfaces.append(interface)
+        self.smali_class.interfaces.append(SVMType(interface))
 
     def visit_super(self, super_class: str) -> None:
-        self.smali_class.super_cls = super_class
+        self.smali_class.super_cls = SVMType(super_class)
 
 
 class _SmaliClassLoader(ClassLoader):
     vm: SmaliVM
     """The vm storing all defined classes."""
 
     def __init__(self, vm: SmaliVM) -> None:
```

### Comparing `pysmali-0.1.3/smali/opcode.py` & `pysmali-0.2.0/smali/opcode.py`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.3/smali/reader.py` & `pysmali-0.2.0/smali/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,22 @@
 from smali.visitor import (
     VisitorBase,
     ClassVisitor,
     FieldVisitor,
     AnnotationVisitor,
     MethodVisitor,
 )
-from smali.base import AccessType, Line, Token, Type, SmaliValueProxy
+from smali.base import (
+    AccessType,
+    Line,
+    Token,
+    SVMType,
+    smali_value,
+    is_type_descriptor
+)
 from smali.opcode import RETURN, GOTO
 
 
 class SupportsCopy:
     """Interface for classes that can react as a copy handler for a SmaliReader.
 
     Note that the context is used to distinguish the current visitor.
@@ -230,15 +237,15 @@
         :type name: str
         :raises SyntaxError: if the provided string is not a valid descriptor
         :meta public:
         """
         if not self.validate:
             return
 
-        if not SmaliValueProxy.is_type_descriptor(name):
+        if not is_type_descriptor(name):
             raise SyntaxError(f"Expected type descriptor - got '{name}'")
 
     def _publish_comment(self) -> None:
         """Publishes the EOL comment and notifies the given visitor
 
         :param visitor: the visitor to notify
         :type visitor: ClassVisitor | MethodVisitor | FieldVisitor | AnnotationVisitor
@@ -434,15 +441,15 @@
     def _handle_super(self) -> None:
         try:
             # If validation is enabled, the '.super' token is verified
             token = next(self.line)
             self._validate_token(token, Token.SUPER)
 
             super_class = self.line.peek()
-            if not SmaliValueProxy.is_type_descriptor(super_class):
+            if not is_type_descriptor(super_class):
                 raise SyntaxError(
                     f"Expected super-class type descriptor - got '{super_class}'"
                 )
 
             if self._visitor:
                 # Visit the class afterwards
                 self._visitor.visit_super(super_class)
@@ -530,23 +537,26 @@
             token = next(self.line)
             self._validate_token(token, Token.METHOD)
 
             flags = self._read_access_flags()
             access_flags = AccessType.get_flags(flags)
 
             # We don't need to verify the signature as this is done
-            # in the Type class
-            signature = Type(self.line.peek())
+            # in the SVMType class
+            signature = SVMType(self.line.peek()).signature
+            if not signature:
+                raise SyntaxError(f"Expected a method signature - got {signature}")
+
             m_visitor = EMPTY_METHV
             if self._visitor:
                 m_visitor = self._visitor.visit_method(
-                    signature.get_method_name(),
+                    signature.name,
                     access_flags,
-                    signature.get_method_params(),
-                    signature.get_method_return_type(),
+                    [str(x) for x in signature.parameter_types],
+                    str(signature.return_type),
                 )
 
             # Add the visitor first before publishing the comment
             self.stack.append(m_visitor if m_visitor else EMPTY_METHV)
             self._publish_comment()
             # The line will be copied if no visitor has been set
             if not m_visitor or m_visitor == EMPTY_METHV:
@@ -564,16 +574,14 @@
         try:
             token = next(self.line)
             self._validate_token(token, Token.ANNOTATION)
 
             flags = self._read_access_flags()
             access_flags = AccessType.get_flags(flags)
 
-            # We don't need to verify the signature as this is done
-            # in the Type class
             descriptor = self.line.peek()
             self._validate_descriptor(descriptor)
 
             a_visitor = EMPTY_ANNOV
             if self._visitor:
                 a_visitor = self._visitor.visit_annotation(access_flags, descriptor)
 
@@ -885,15 +893,15 @@
             self._next_line()
             value = self.line.peek()
             self._publish_comment()
             if do_copy:
                 self._copy_line()
             if value[0] == "." and value[1:] == Token.END.value:
                 break
-            values.append(value)
+            values.append(smali_value(value))
 
         if self._visitor and self._visitor != EMPTY_METHV:
             self._visitor.visit_array_data(length, values)
 
     def _handle_local(self) -> None:
         """Handle debug information."""
         if not self._visitor or self._visitor == EMPTY_METHV:
```

### Comparing `pysmali-0.1.3/smali/shell/__init__.py` & `pysmali-0.2.0/smali/shell/__init__.py`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.3/smali/shell/__main__.py` & `pysmali-0.2.0/smali/shell/__main__.py`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.3/smali/shell/cli.py` & `pysmali-0.2.0/smali/shell/cli.py`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.3/smali/shell/model.py` & `pysmali-0.2.0/smali/shell/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,69 +19,68 @@
 import pprint
 
 from cmd import Cmd
 
 from smali import (
     AccessType,
     opcode,
-    Type,
     SmaliValue,
     MethodVisitor,
     ClassVisitor,
     FieldVisitor,
-    SmaliReader
+    SmaliReader,
 )
 from smali.bridge import (
     Frame,
     executor,
     SmaliObject,
     SmaliClass,
     SmaliField,
-    SmaliMethod
+    SmaliMethod,
 )
 from smali.bridge.vm import (
     SmaliVMClassReader,
     SmaliVMMethodReader,
     SmaliVMFieldReader,
-    SmaliVM
+    SmaliVM,
 )
 
-SMALI_SCRIPT_SUFFIX = 'ssf'
+SMALI_SCRIPT_SUFFIX = "ssf"
 """File suffix for Smali-Script files"""
 
 
 class DefaultVisitor(MethodVisitor, ClassVisitor):
     """Visitor implementation that handles both class and method definitions"""
 
     frame: Frame
     """The root method context"""
 
     cls: SmaliVMClassReader
     """The root class"""
 
-    shell: 'ISmaliShell'
+    shell: "ISmaliShell"
     """The shell reference"""
 
     last_label: str
     """Stores the last label that has been typed"""
 
     importing: bool = False
 
-    def __init__(self, shell: 'ISmaliShell') -> None:
+    def __init__(self, shell: "ISmaliShell") -> None:
         super().__init__(None)
         self.shell = shell
         self.frame = Frame()
         self.last_label = None
         self.pos = 0
 
         self.frame.vm = shell.emulator
-        self.reset_var('p0', shell.root)
+        self.reset_var("p0", shell.root)
 
     def visit_restart(self, register: str) -> None:
-        if register != 'p0':
+        if register != "p0":
             self.reset_var(register)
         else:
             self.reset_var(register, self.shell.root)
 
     def reset_var(self, register: str, val=None):
         """Applies a new value to the given register name"""
         self.frame.registers[register] = val
@@ -110,87 +109,97 @@
         for _, value in opcode.__dict__.items():
             if value == ins_name:
                 exc = executor.get_executor(ins_name)
                 exc.args = args
                 exc(self.frame)
                 self.pos += 1
 
-                if 'return' in value:
+                if "return" in value:
                     print(self.frame.return_value)
                 return
 
         if self.importing:
             self.shell.onecmd(f"{ins_name} {' '.join(args)}")
         else:
-            raise SyntaxError(f'Invalid OpCode: {ins_name}')
+            raise SyntaxError(f"Invalid OpCode: {ins_name}")
 
-    def visit_field(self, name: str, access_flags: int, field_type: str,
-                    value=None) -> FieldVisitor:
-        field = SmaliField(self.shell.root.smali_class, f"{name}:{field_type}", access_flags,
-                           name, Type(field_type), value=SmaliValue(value) if value else None)
+    def visit_field(
+        self, name: str, access_flags: int, field_type: str, value=None
+    ) -> FieldVisitor:
+        field = SmaliField(
+            field_type,
+            self.shell.root.smali_class,
+            f"{name}:{field_type}",
+            access_flags,
+            name,
+            value=SmaliValue(value) if value else None,
+        )
         self.shell.root.smali_class[name] = field
         if access_flags not in AccessType.STATIC and value is not None:
             self.shell.root[name] = value
 
         return SmaliVMFieldReader(field)
 
     def visit_return(self, ret_type: str, args: list) -> None:
         if ret_type:
             self.visit_instruction(f"return-{ret_type}", args)
         else:
             self.visit_instruction("return", args)
 
     def visit_invoke(self, inv_type: str, args: list, owner: str, method: str) -> None:
         if inv_type:
-            self.visit_instruction(f"invoke-{inv_type}", [inv_type, args, owner, method])
+            self.visit_instruction(
+                f"invoke-{inv_type}", [inv_type, args, owner, method]
+            )
         else:
             self.visit_instruction("invoke", [inv_type, args, owner, method])
 
-    def visit_method(self, name: str, access_flags: int, parameters: list,
-                     return_type: str) -> MethodVisitor:
+    def visit_method(
+        self, name: str, access_flags: int, parameters: list, return_type: str
+    ) -> MethodVisitor:
         signature = f"{name}({''.join(parameters)}){return_type}"
         smali_class = self.shell.root.smali_class
 
         method = SmaliMethod(self.shell.emulator, smali_class, signature, access_flags)
         visitor = SmaliVMMethodReader(method)
         self.shell.emulator.new_frame(method, visitor.frame)
         smali_class[name] = method
         return visitor
 
-    def visit_inner_class(self, name: str, access_flags: int) -> 'ClassVisitor':
+    def visit_inner_class(self, name: str, access_flags: int) -> "ClassVisitor":
         if self.importing:
             smali_class = self.shell.root.smali_class
             inner = SmaliClass(smali_class, name, access_flags)
 
             smali_class[name] = inner
             return SmaliVMClassReader(self.shell.emulator, inner)
 
 
 class ISmaliShell(Cmd):
     """Implementation of an interactive Smali-Interpreter."""
 
-    DEFAULT_PROMPT = '>>> '
+    DEFAULT_PROMPT = ">>> "
     """The default prompt"""
 
-    INLINE_PROMPT = '... '
+    INLINE_PROMPT = "... "
     """Prompt used for field and method definitions"""
 
     visitor: DefaultVisitor
     """The default visitor instance"""
 
     reader: SmaliReader
     """The reader used to parse code snippets."""
 
     emulator: SmaliVM
     """The actual VM reference that will execute each method"""
 
     root: SmaliObject
     """The base context used to define fields and methods."""
 
-    prompt: str = '>>> '
+    prompt: str = ">>> "
     """The prompt used by ``cmd.Cmd``"""
 
     check_import: bool = True
     """Used to indicate whether this shell should verify each import"""
 
     __imported_files: list = []
     """Internal file list"""
@@ -216,33 +225,32 @@
         if not os.path.exists(path):
             print(f'! Could not find file at "{path}"')
             return
 
         if path in self.__imported_files and self.check_import:
             return
 
-        if not path.endswith(('.smali', f".{SMALI_SCRIPT_SUFFIX}")):
+        if not path.endswith((".smali", f".{SMALI_SCRIPT_SUFFIX}")):
             print(f"! Unknown file format (unknown suffix) at '{path}'")
             return
 
         cls = None
-        with open(path, 'r', encoding='utf-8') as source:
+        with open(path, "r", encoding="utf-8") as source:
             self.__imported_files.append(path)
             if path.endswith(f".{SMALI_SCRIPT_SUFFIX}"):
                 self.visitor.importing = True
                 self.reader.visit(source, self.visitor)
                 self.visitor.importing = False
             else:
                 cls = self.emulator.classloader.load_class(source, init=False)
 
-
         try:
             if cls is not None:
                 cls.clinit()
-        except Exception: # :noqa
+        except Exception:  # :noqa
             print(traceback.format_exc())
 
     def do_vars(self, _):
         """usage: vars
 
         Prints all variables with the help of ``pprint``.
         """
@@ -264,36 +272,36 @@
 
     def do_del(self, register):
         """usage: del <register>
 
         Deletes the variable at the specified register. The root
         context at 'p0' can't be deleted.
         """
-        if register == 'p0':
-            print('! Attempted to delete root-context - skipping...\n')
+        if register == "p0":
+            print("! Attempted to delete root-context - skipping...\n")
             return
 
         if register in self.visitor.frame.registers:
             val = self.visitor.frame.registers.pop(register)
             del val
 
     def precmd(self, line: str):
         if len(line) == 0:
             self.change_prompt(ISmaliShell.DEFAULT_PROMPT)
-            return 'EOF'
+            return "EOF"
 
         return line
 
     def default(self, line: str) -> None:
         """Handles the instruction or register name
 
         :param line: the input line
         :type line: str
         """
-        if line == 'EOF':
+        if line == "EOF":
             return
 
         if isinstance(self.visitor, DefaultVisitor):
             if line in self.visitor.frame.registers:
                 print(self.visitor.frame.registers[line])
                 return
 
@@ -304,12 +312,12 @@
 
     def do_exit(self, _):
         """Exits the interpreter"""
         sys.exit(0)
 
     def do_copyright(self, _):
         """Prints copyright information"""
-        print('Copyright (C) 2023 MatrixEditor')
+        print("Copyright (C) 2023 MatrixEditor")
 
     def change_prompt(self, new_prompt: str):
         """Changes the prompt (for later usage)"""
         self.prompt = new_prompt
```

### Comparing `pysmali-0.1.3/smali/visitor.py` & `pysmali-0.2.0/smali/visitor.py`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.3/smali/writer.py` & `pysmali-0.2.0/smali/writer.py`

 * *Files identical despite different names*

