# Comparing `tmp/etdd-0.0.8.tar.gz` & `tmp/etdd-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etdd-0.0.8.tar", last modified: Tue Jun  6 12:15:32 2023, max compression
+gzip compressed data, was "etdd-0.0.9.tar", last modified: Tue Jun  6 12:29:23 2023, max compression
```

## Comparing `etdd-0.0.8.tar` & `etdd-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-06 12:15:32.105376 etdd-0.0.8/
--rw-rw-r--   0 user      (1000) user      (1000)     1516 2023-06-05 11:53:50.000000 etdd-0.0.8/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)     1636 2023-06-06 12:15:32.105376 etdd-0.0.8/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      987 2023-06-06 12:15:13.000000 etdd-0.0.8/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-06 12:15:32.101376 etdd-0.0.8/etdd/
--rwxrwxr-x   0 user      (1000) user      (1000)       38 2023-06-06 11:48:09.000000 etdd-0.0.8/etdd/__init__.py
--rwxrwxr-x   0 user      (1000) user      (1000)    16709 2023-06-06 11:47:58.000000 etdd-0.0.8/etdd/core.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-06 12:15:32.101376 etdd-0.0.8/etdd.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     1636 2023-06-06 12:15:32.000000 etdd-0.0.8/etdd.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      195 2023-06-06 12:15:32.000000 etdd-0.0.8/etdd.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-06 12:15:32.000000 etdd-0.0.8/etdd.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       53 2023-06-06 12:15:32.000000 etdd-0.0.8/etdd.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        5 2023-06-06 12:15:32.000000 etdd-0.0.8/etdd.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-06 12:15:32.105376 etdd-0.0.8/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1131 2023-06-06 12:15:29.000000 etdd-0.0.8/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-06 12:29:23.886839 etdd-0.0.9/
+-rw-rw-r--   0 user      (1000) user      (1000)     1516 2023-06-05 11:53:50.000000 etdd-0.0.9/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)     2849 2023-06-06 12:29:23.882839 etdd-0.0.9/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2200 2023-06-06 12:28:46.000000 etdd-0.0.9/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-06 12:29:23.882839 etdd-0.0.9/etdd/
+-rwxrwxr-x   0 user      (1000) user      (1000)       38 2023-06-06 11:48:09.000000 etdd-0.0.9/etdd/__init__.py
+-rwxrwxr-x   0 user      (1000) user      (1000)    16709 2023-06-06 11:47:58.000000 etdd-0.0.9/etdd/core.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-06 12:29:23.882839 etdd-0.0.9/etdd.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     2849 2023-06-06 12:29:23.000000 etdd-0.0.9/etdd.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      195 2023-06-06 12:29:23.000000 etdd-0.0.9/etdd.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-06 12:29:23.000000 etdd-0.0.9/etdd.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       53 2023-06-06 12:29:23.000000 etdd-0.0.9/etdd.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        5 2023-06-06 12:29:23.000000 etdd-0.0.9/etdd.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-06 12:29:23.886839 etdd-0.0.9/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1131 2023-06-06 12:29:20.000000 etdd-0.0.9/setup.py
```

### Comparing `etdd-0.0.8/LICENSE` & `etdd-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `etdd-0.0.8/PKG-INFO` & `etdd-0.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etdd
-Version: 0.0.8
+Version: 0.0.9
 Summary: eTDD framework
 Home-page: https://github.com/neubertm/TDD_framework
 Author: Milan Neubert, Felipe Bombardelli
 Author-email: felipebombardelli@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,43 +17,99 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # eTDD
 
 Framework for Test-driven development (TDD) to support to isolate the unit code in C/C++.
 
-# Example 1
+# Installing
 
-You can create the file tdd.py and execute it with the follow code:
+## Windows
+
+Before to execute the test, you need to execute the option "Install CppUTest on ./tmp" in the tdd.menu(). It will download and compile the cpputest code.
+
+You need to install also:
+ - cmake : https://cmake.org/download/
+ - cppcheck : http://cppcheck.net/
+ - git : https://github.com/git-for-windows/git/releases/tag/v2.41.0.windows.1
+ - mingw-gcc : https://github.com/niXman/mingw-builds-binaries/releases
+ - doxygen : https://www.doxygen.nl/download.html
+
+
+## Linux
 
 ```
-from etdd import TDD, full_main
+sudo apt install cmake libcpputest-dev cppcheck
+sudo apt install doxygen graphviz
+```
 
-tdd = TDD(main=full_main, envpath="envpath.ini")
+
+# Example 1 - simplest example
+
+```
+from etdd import TDD
+
+tdd = TDD()
 tdd.download_from_git("https://github.com/neubertm/TDD_framework.git")
 
+# Set the flags in the CMakelists
+tdd.cmake["CMAKE_C_FLAGS"] = "-g -O0 -coverage -lgcov "
+tdd.cmake["CMAKE_CXX_FLAGS"] = "-g -O0 -coverage -lgcov "
+
+# Test 1 - BitInverter
 test = tdd.test("TDD_framework/TESTs/BitInverter_Tpkg/src/test.cpp", "BitInverter")
 test.files = ["TDD_framework/project/BitInverter/BitInverter.*", "TDD_framework/TESTs/BitInverter_Tpkg/src/MemLeakDetection*.h"]
 test.compile = ["BitInverter.c"]
 
+# Open the menu in the console
 tdd.menu()
 ```
 
-# Windows
 
-Before to execute the test, you need to execute the option "Install CppUTest on ./tmp" in the tdd.menu(). It will download and compile the cpputest code.
+# Example 2 - with environment file
 
-You need to install also:
- - cmake
- - cppcheck
- - git
- - mingw-gcc
- - doxygen and dot (optional)
+You can create the file tdd.py and execute it with the follow code:
+
+```
+from etdd import TDD, full_main
 
+tdd = TDD(main=full_main, envpath="envpath.ini")
+tdd.download_from_git("https://github.com/neubertm/TDD_framework.git")
+
+# Test 1 - BitInverter
+test = tdd.test("TDD_framework/TESTs/BitInverter_Tpkg/src/test.cpp", "BitInverter")
+test.files = ["TDD_framework/project/BitInverter/BitInverter.*", "TDD_framework/TESTs/BitInverter_Tpkg/src/MemLeakDetection*.h"]
+test.compile = ["BitInverter.c"]
 
-# Linux
+# Open the menu in the console
+tdd.menu()
+```
 
-You must to install the library libcpputest-dev
+## envpath.ini
 ```
-sudo apt install cmake libcpputest-dev doxygen cppcheck
+[CMAKE]
+check=true
+ENV_CONFIG_SCRIPT = /usr/bin/
+
+[MINGW]
+check=False
+ENV_CONFIG_SCRIPT = /usr/bin/
+
+[MSVC]
+check=False
+ENV_CONFIG_SCRIPT = /usr/bin/
+
+[CLANG]
+check=False
+ENV_CONFIG_SCRIPT = /usr/bin/
+
+[CPPCHECK]
+check=False
+ENV_CONFIG_SCRIPT = /usr/bin/
+
+[CPPUMOCKGEN]
+ENV_CONFIG_SCRIPT = /usr/bin/
 ```
 
+
+
+
```

### Comparing `etdd-0.0.8/etdd/core.py` & `etdd-0.0.9/etdd/core.py`

 * *Files identical despite different names*

### Comparing `etdd-0.0.8/etdd.egg-info/PKG-INFO` & `etdd-0.0.9/etdd.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etdd
-Version: 0.0.8
+Version: 0.0.9
 Summary: eTDD framework
 Home-page: https://github.com/neubertm/TDD_framework
 Author: Milan Neubert, Felipe Bombardelli
 Author-email: felipebombardelli@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,43 +17,99 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # eTDD
 
 Framework for Test-driven development (TDD) to support to isolate the unit code in C/C++.
 
-# Example 1
+# Installing
 
-You can create the file tdd.py and execute it with the follow code:
+## Windows
+
+Before to execute the test, you need to execute the option "Install CppUTest on ./tmp" in the tdd.menu(). It will download and compile the cpputest code.
+
+You need to install also:
+ - cmake : https://cmake.org/download/
+ - cppcheck : http://cppcheck.net/
+ - git : https://github.com/git-for-windows/git/releases/tag/v2.41.0.windows.1
+ - mingw-gcc : https://github.com/niXman/mingw-builds-binaries/releases
+ - doxygen : https://www.doxygen.nl/download.html
+
+
+## Linux
 
 ```
-from etdd import TDD, full_main
+sudo apt install cmake libcpputest-dev cppcheck
+sudo apt install doxygen graphviz
+```
 
-tdd = TDD(main=full_main, envpath="envpath.ini")
+
+# Example 1 - simplest example
+
+```
+from etdd import TDD
+
+tdd = TDD()
 tdd.download_from_git("https://github.com/neubertm/TDD_framework.git")
 
+# Set the flags in the CMakelists
+tdd.cmake["CMAKE_C_FLAGS"] = "-g -O0 -coverage -lgcov "
+tdd.cmake["CMAKE_CXX_FLAGS"] = "-g -O0 -coverage -lgcov "
+
+# Test 1 - BitInverter
 test = tdd.test("TDD_framework/TESTs/BitInverter_Tpkg/src/test.cpp", "BitInverter")
 test.files = ["TDD_framework/project/BitInverter/BitInverter.*", "TDD_framework/TESTs/BitInverter_Tpkg/src/MemLeakDetection*.h"]
 test.compile = ["BitInverter.c"]
 
+# Open the menu in the console
 tdd.menu()
 ```
 
-# Windows
 
-Before to execute the test, you need to execute the option "Install CppUTest on ./tmp" in the tdd.menu(). It will download and compile the cpputest code.
+# Example 2 - with environment file
 
-You need to install also:
- - cmake
- - cppcheck
- - git
- - mingw-gcc
- - doxygen and dot (optional)
+You can create the file tdd.py and execute it with the follow code:
+
+```
+from etdd import TDD, full_main
 
+tdd = TDD(main=full_main, envpath="envpath.ini")
+tdd.download_from_git("https://github.com/neubertm/TDD_framework.git")
+
+# Test 1 - BitInverter
+test = tdd.test("TDD_framework/TESTs/BitInverter_Tpkg/src/test.cpp", "BitInverter")
+test.files = ["TDD_framework/project/BitInverter/BitInverter.*", "TDD_framework/TESTs/BitInverter_Tpkg/src/MemLeakDetection*.h"]
+test.compile = ["BitInverter.c"]
 
-# Linux
+# Open the menu in the console
+tdd.menu()
+```
 
-You must to install the library libcpputest-dev
+## envpath.ini
 ```
-sudo apt install cmake libcpputest-dev doxygen cppcheck
+[CMAKE]
+check=true
+ENV_CONFIG_SCRIPT = /usr/bin/
+
+[MINGW]
+check=False
+ENV_CONFIG_SCRIPT = /usr/bin/
+
+[MSVC]
+check=False
+ENV_CONFIG_SCRIPT = /usr/bin/
+
+[CLANG]
+check=False
+ENV_CONFIG_SCRIPT = /usr/bin/
+
+[CPPCHECK]
+check=False
+ENV_CONFIG_SCRIPT = /usr/bin/
+
+[CPPUMOCKGEN]
+ENV_CONFIG_SCRIPT = /usr/bin/
 ```
 
+
+
+
```

### Comparing `etdd-0.0.8/setup.py` & `etdd-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='etdd',
-    version='0.0.8',
+    version='0.0.9',
     description='eTDD framework',
     packages=['etdd'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Topic :: Software Development :: Libraries :: Python Modules",
```

