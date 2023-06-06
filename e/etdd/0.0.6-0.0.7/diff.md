# Comparing `tmp/etdd-0.0.6.tar.gz` & `tmp/etdd-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etdd-0.0.6.tar", last modified: Fri May 12 20:28:36 2023, max compression
+gzip compressed data, was "etdd-0.0.7.tar", last modified: Tue Jun  6 11:53:49 2023, max compression
```

## Comparing `etdd-0.0.6.tar` & `etdd-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-12 20:28:36.889212 etdd-0.0.6/
--rw-r--r--   0 user      (1000) user      (1000)      613 2023-05-12 20:28:36.889212 etdd-0.0.6/PKG-INFO
--rwxr-xr-x   0 user      (1000) user      (1000)        3 2023-05-12 20:15:11.000000 etdd-0.0.6/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-12 20:28:36.889212 etdd-0.0.6/etdd/
--rwxr-xr-x   0 user      (1000) user      (1000)       27 2023-05-12 20:15:11.000000 etdd-0.0.6/etdd/__init__.py
--rwxr-xr-x   0 user      (1000) user      (1000)    15624 2023-05-12 20:18:20.000000 etdd-0.0.6/etdd/core.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-12 20:28:36.889212 etdd-0.0.6/etdd.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      613 2023-05-12 20:28:36.000000 etdd-0.0.6/etdd.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      187 2023-05-12 20:28:36.000000 etdd-0.0.6/etdd.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-12 20:28:36.000000 etdd-0.0.6/etdd.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       62 2023-05-12 20:28:36.000000 etdd-0.0.6/etdd.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        5 2023-05-12 20:28:36.000000 etdd-0.0.6/etdd.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-05-12 20:28:36.889212 etdd-0.0.6/setup.cfg
--rwxr-xr-x   0 user      (1000) user      (1000)      979 2023-05-12 20:28:17.000000 etdd-0.0.6/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-06 11:53:49.681840 etdd-0.0.7/
+-rw-rw-r--   0 user      (1000) user      (1000)     1516 2023-06-05 11:53:50.000000 etdd-0.0.7/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)     1080 2023-06-06 11:53:49.681840 etdd-0.0.7/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      431 2023-06-06 11:49:15.000000 etdd-0.0.7/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-06 11:53:49.681840 etdd-0.0.7/etdd/
+-rwxrwxr-x   0 user      (1000) user      (1000)       38 2023-06-06 11:48:09.000000 etdd-0.0.7/etdd/__init__.py
+-rwxrwxr-x   0 user      (1000) user      (1000)    16709 2023-06-06 11:47:58.000000 etdd-0.0.7/etdd/core.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-06 11:53:49.681840 etdd-0.0.7/etdd.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     1080 2023-06-06 11:53:49.000000 etdd-0.0.7/etdd.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      195 2023-06-06 11:53:49.000000 etdd-0.0.7/etdd.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-06 11:53:49.000000 etdd-0.0.7/etdd.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       46 2023-06-06 11:53:49.000000 etdd-0.0.7/etdd.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        5 2023-06-06 11:53:49.000000 etdd-0.0.7/etdd.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-06 11:53:49.681840 etdd-0.0.7/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1111 2023-06-06 11:53:48.000000 etdd-0.0.7/setup.py
```

### Comparing `etdd-0.0.6/etdd/core.py` & `etdd-0.0.7/etdd/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import jinja2
 import shutil
 import re
 import time
 import glob
 import readchar
 import threading
+
+from configparser import ConfigParser
 from pathlib import Path
 from consolemenu import ConsoleMenu
 from consolemenu.items import ExitItem
 from consolemenu.items import FunctionItem
 from colorama import Fore, Style
 
 # =======================================================================================
@@ -22,14 +24,18 @@
 
 std_cmake_template = """project({{name}})
 cmake_minimum_required(VERSION 3.00)
 
 SET(PROJECT_DIR {{project_dir}})
 SET(CPPCHECK_LIB "${PROJECT_DIR}/tmp/cpputest_mingw")
 
+SET(CMAKE_C_FLAGS  ${CMAKE_C_FLAGS} -include MemLeakDetectionMallocMacros.h )
+SET(CMAKE_CXX_FLAGS  ${CMAKE_CXX_FLAGS} -include MemLeakDetectionNewMacros.h )
+SET(CMAKE_CXX_FLAGS  ${CMAKE_CXX_FLAGS} -include MemLeakDetectionMallocMacros.h )
+
 {% for var_name,var_value in cmake.items() -%}
 SET({{var_name}} "{{var_value}}")
 {% endfor %}
 
 add_executable(TestApp
     {% for file in compile -%}
     {{file}}        
@@ -64,15 +70,15 @@
 
 int main(int ac, char** av)
 {
     return CommandLineTestRunner::RunAllTests(ac, av);
 }
 """
 
-main_template22 = """
+full_main = """
 #include "CppUTest/CommandLineTestRunner.h"
 #include "CppUTest/TestPlugin.h"
 #include "CppUTest/TestRegistry.h"
 #include "CppUTestExt/IEEE754ExceptionsPlugin.h"
 #include "CppUTestExt/MockSupportPlugin.h"
 
 class MyDummyComparator : public MockNamedValueComparator
@@ -123,14 +129,20 @@
     print(f"\n{Fore.YELLOW}# {cmd}{Style.RESET_ALL}")
     error = os.system(cmd)
     if error != 0:
         os.chdir(saved_path)
         raise(Exception("Error in {}".format(cmd)))
     os.chdir(saved_path)
 
+def where(exec_name):
+    if os.name == 'nt':
+        bash_exec(".", "where "+exec_name)
+    else:
+        bash_exec(".", "whereis "+exec_name)
+
 def pause():
     if os.name == 'nt':
         os.system("pause")
     else:
         input('Press <ENTER> to continue')
 
 # =======================================================================================
@@ -158,100 +170,119 @@
         return(self.b_keyPressed)
 
 # =======================================================================================
 #  TDD
 # =======================================================================================
 
 class TDD:
-    def __init__(self, cmakelists=std_cmake_template, main=std_main_template):
+    def __init__(self, cmakelists=std_cmake_template, main=std_main_template, envpath=""):
         std_gcc_flags = "-g -O0 -coverage -lgcov " # keep one space after the flags
 
         self.project = Path(".")
         self.tests = []
         self.includes = []
         self.cmake = {"CMAKE_C_FLAGS": std_gcc_flags, "CMAKE_CXX_FLAGS": std_gcc_flags}
         self.templates = {"cmakelists": cmakelists, "main": main}
         self.run_test_func = None
         if os.name == 'nt':
+            self.make_cmd = "mingw32-make"
             self.makefile = "MinGW Makefiles"
         else:
+            self.make_cmd = "make"
             self.makefile = "Unix Makefiles"
-    
+
+        if envpath != "":
+            self.config_path(envpath)
+
+    def config_path(self, filename):
+        parser = ConfigParser()
+        parser.optionxform = str
+        parser.read(filename)      
+        for key, item in parser._sections.items():
+            if "check" in item and item["check"].lower() == "true":
+                # print(item)
+                os.environ["PATH"] = item["ENV_CONFIG_SCRIPT"] + os.pathsep + os.environ["PATH"]
+
     def test(self, test_file, name="", cmakelists="", main=""):
         test_name = name
         if test_name == "":
             test_name = Path(test_file).stem
         
         test = Test(test_file, self, test_name)
         self.tests.append(test)
         if cmakelists != "":
             test.templates["cmakelists"] = cmakelists
         if main != "":
             test.templates["main"] = main
         return test
 
     def info(self):
-        bash_exec(self.project, "where cmake")
-        bash_exec(self.project, "where gcc")
-        bash_exec(self.project, "where g++")
-        bash_exec(self.project, "where mingw32-make")
-        bash_exec(self.project, "where git")
-        bash_exec(self.project, "where doxygen")
-        bash_exec(self.project, "where lizard")
-        bash_exec(self.project, "where gcovr")
-        bash_exec(self.project, "where dot")
+        where("cmake")
+        where("gcc")
+        where("g++")
+        where(self.make_cmd)
+        where("git")
+        where("doxygen")
+        where("lizard")
+        where("gcovr")
+        where("dot")
         pause()
 
     def doxygen(self):
         print("opa")
         doxygen_file = self.project / "Doxyfile"
         if not doxygen_file.exists():
             bash_exec(self.project, "doxygen -g")    
         bash_exec(self.project, "doxygen")
         pause()
 
-    def installCPPUTest(self, version="v4.0"):
+    def install_CPPUTest(self, version="v4.0"):
         tmp_path = self.project / "tmp";
         os.makedirs(tmp_path, exist_ok=True)
         cpputest_path = tmp_path / "cpputest"
         if not cpputest_path.exists():
             print("Downloading and compiling the CPPUTest in {}".format(tmp_path))
             bash_exec_check(tmp_path, "git clone --depth 1 https://github.com/cpputest/cpputest".format(version))
 
         build_path = cpputest_path / "build-mingw" 
         install_path_abs = Path(tmp_path/"cpputest_mingw").resolve()
         os.makedirs(build_path, exist_ok=True)
-        bash_exec_check(build_path, 'cmake -G "MinGW Makefiles" -DCMAKE_INSTALL_PREFIX={} ..'.format(install_path_abs))
-        bash_exec_check(build_path, "mingw32-make")
-        bash_exec_check(build_path, "mingw32-make install")
+        bash_exec_check(build_path, f'cmake -G "{self.makefile}" -DCMAKE_INSTALL_PREFIX={install_path_abs} ..')
+        bash_exec_check(build_path, f'{self.make_cmd}')
+        bash_exec_check(build_path, f'{self.make_cmd} install')
         pause()
 
     def menu(self):
         menu = ConsoleMenu("eTDD is C++ unit test framework. (%s)" % ("opa"),
                             "Choose test packag/es variant.", show_exit_option=False)
         menu.append_item( ExitItem("Auf wiedersehen!!", menu=None, menu_char='q') )
-        menu.append_item( FunctionItem("Install CppUTest on ./tmp", self.installCPPUTest, [], menu_char='c') )
-        menu.append_item( FunctionItem("Documentation", self.doxygen, [], menu_char='d') )
-        menu.append_item( FunctionItem("Information", self.info, [], menu_char='i') )
+        menu.append_item( FunctionItem("Install CppUTest on ./tmp", self.install_CPPUTest, [], menu_char='c') )
+        menu.append_item( FunctionItem("Generate the Documentation", self.doxygen, [], menu_char='d') )
+        menu.append_item( FunctionItem("Information on path of executables", self.info, [], menu_char='i') )
+        # menu.append_item( FunctionItem("Execute all Tests", self.run_all_tests, [], menu_char='a') )
 
         count = 1
         for test in self.tests:
             menu.append_item( FunctionItem(test.name, test.run_in_loop, [], menu_char=str(count))  )
             count += 1
         menu.show()
 
     def download_from_git(self, repo):
         name = Path(repo).stem
         project_path = Path(".") / name
         if not project_path.exists():
             bash_exec_check(self.project, "git clone {}".format(repo))
 
     def run_test(self, func):
+        """ Decoder to replace the test function """
         self.run_test_func = func
 
+    def run_all_tests(self):
+        pause()
+
 # =======================================================================================
 #  Test
 # =======================================================================================
 
 class Test:
     def __init__(self, test_file: str, tdd: TDD, name: str):
         self.name = name
@@ -384,30 +415,30 @@
 
     def configure(self):
         os.makedirs(self.build, exist_ok=True)
         bash_exec_check(self.build, 'cmake -G "{}" ..'.format(self.tdd.makefile))
 
     def make(self, debug=False):
         if debug:
-            bash_exec_check(self.build, 'mingw32-make VERBOSE=1')
+            bash_exec_check(self.build, f'{self.tdd.make_cmd} VERBOSE=1')
         else:
-            bash_exec_check(self.build, 'mingw32-make')
+            bash_exec_check(self.build, self.tdd.make_cmd)
 
     def exec(self):
         if os.name == 'nt':
             bash_exec_check(self.build, 'TestApp')
         else:
             bash_exec_check(self.build, './TestApp')
 
     def cppcheck(self):
         # cppcheck
         pass
 
     def clean(self):
-        bash_exec(self.build, "make clean")
+        bash_exec(self.build, f"{self.tdd.make_cmd} clean")
 
     def coverage(self):
         """
             # gcovr --object-directory CMakeFiles\TestApp.dir\mingw_tmp_single -r ..\mingw_tmp_single\ -f "\.\./mingw_tmp_single/Calculator.cpp" -b --txt cov_vypis.txt --html cov\cov_html.html --html-details cov\coverage_details.html
         """
         bash_exec(self.home, 'gcovr')
 
@@ -431,15 +462,18 @@
             self.coverage()
             self.clean()
 
     def run_in_loop(self):
         keyboard = KeyboardThread()
         while(True):
             # Run the Test
-            self.run()
+            try:
+                self.run()
+            except Exception as e:
+                print(e)
 
             # Check changes on files or keyboard event
             while(True):
                 if self.is_changed_files():
                     os.system('cls')
                     break;
                 if keyboard.isAnyKeyPressed():
```

### Comparing `etdd-0.0.6/setup.py` & `etdd-0.0.7/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='etdd',
-    version='0.0.6',
-    description='extend TDD framework',
+    version='0.0.7',
+    description='eTDD framework',
     packages=['etdd'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"
     ],
+    url = "https://github.com/neubertm/TDD_framework",
     python_requires='>=3',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Milan Neubert, Felipe Bombardelli",
     author_email="felipebombardelli@gmail.com",
-    
+    # url="https://github.com/bombark/iotproj",
+    # entry_points={'console_scripts': [
+    #     'iotproj = iotproj:app',
+    # ]},
     install_requires=[
         'pathlib'
         , 'jinja2'
         , 'colorama'
         , 'tabulate'
-        , 'lizard'
-        , 'console-menu' # 0.8.0
-        , 'readchar'
+        , 'console-menu'
     ]
 )
```

