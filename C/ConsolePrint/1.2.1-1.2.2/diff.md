# Comparing `tmp/consoleprint-1.2.1.tar.gz` & `tmp/consoleprint-1.2.2.tar.gz`

## Comparing `consoleprint-1.2.1.tar` & `consoleprint-1.2.2.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 consoleprint-1.2.1/src/ConsolePrint/__init__.py
--rw-r--r--   0        0        0     7621 2020-02-02 00:00:00.000000 consoleprint-1.2.1/src/ConsolePrint/animate.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 consoleprint-1.2.1/src/ConsolePrint/console2file.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 consoleprint-1.2.1/src/ConsolePrint/formats.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 consoleprint-1.2.1/src/ConsolePrint/loading.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 consoleprint-1.2.1/tests/tests.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 consoleprint-1.2.1/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 consoleprint-1.2.1/LICENSE
--rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 consoleprint-1.2.1/README.md
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 consoleprint-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 consoleprint-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 consoleprint-1.2.2/src/ConsolePrint/__init__.py
+-rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 consoleprint-1.2.2/src/ConsolePrint/animate.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 consoleprint-1.2.2/src/ConsolePrint/console2file.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 consoleprint-1.2.2/src/ConsolePrint/loading.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 consoleprint-1.2.2/tests/tests.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 consoleprint-1.2.2/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 consoleprint-1.2.2/LICENSE
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 consoleprint-1.2.2/README.md
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 consoleprint-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 consoleprint-1.2.2/PKG-INFO
```

### Comparing `consoleprint-1.2.1/src/ConsolePrint/animate.py` & `consoleprint-1.2.2/src/ConsolePrint/animate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,35 @@
 import time
 import os
-from formats import *
+
+# Font Colors
+reset = '\033[0m'
+grey = '\033[30m'
+red = '\033[31m'
+green = '\033[32m'
+yellow = '\033[33m'
+blue = '\033[34m'
+magenta = '\033[35m'
+cyan = '\033[36m'
+white = '\033[37m'
+
+
+# Text Formats
+bold = '\033[1m'
+italics = '\033[3m'
+underscore = '\033[4m'
+strike = '\033[9m'
+double_under = '\033[21m'
+red_bg = '\033[41m'
+green_bg = '\033[42m'
+yellow_bg = '\033[43m'
+blue_bg = '\033[44m'
+magenta_bg = '\033[45m'
+cyan_bg = '\033[46m'
+white_bg = '\033[47m'
 
 terminal_width = os.get_terminal_size().columns
 
 
 def printing(text: str, delay=0.05, style='letter', stay=True, rev=False, format=reset):
     """Prints text to console letter by letter or word by word"""
     print(format, end='\r')
```

### Comparing `consoleprint-1.2.1/src/ConsolePrint/console2file.py` & `consoleprint-1.2.2/src/ConsolePrint/console2file.py`

 * *Files identical despite different names*

### Comparing `consoleprint-1.2.1/src/ConsolePrint/loading.py` & `consoleprint-1.2.2/src/ConsolePrint/loading.py`

 * *Files identical despite different names*

### Comparing `consoleprint-1.2.1/tests/tests.py` & `consoleprint-1.2.2/tests/tests.py`

 * *Files identical despite different names*

### Comparing `consoleprint-1.2.1/LICENSE` & `consoleprint-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `consoleprint-1.2.1/README.md` & `consoleprint-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `consoleprint-1.2.1/pyproject.toml` & `consoleprint-1.2.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ConsolePrint"
-version = "1.2.1"
+version = "1.2.2"
 authors = [
   { name="Udemezue Iloabachie", email="udemezue@gmail.com" },
 ]
 description = "A package to animate and beautify print output to console"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `consoleprint-1.2.1/PKG-INFO` & `consoleprint-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConsolePrint
-Version: 1.2.1
+Version: 1.2.2
 Summary: A package to animate and beautify print output to console
 Project-URL: Homepage, https://github.com/iloabachie/ConsolePrint
 Project-URL: Bug Tracker, https://github.com/iloabachie/ConsolePrint/issues
 Author-email: Udemezue Iloabachie <udemezue@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

