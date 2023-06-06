# Comparing `tmp/consoleprint-1.0.3.tar.gz` & `tmp/consoleprint-1.2.1.tar.gz`

## Comparing `consoleprint-1.0.3.tar` & `consoleprint-1.2.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 consoleprint-1.0.3/src/ConsolePrint/__init__.py
--rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 consoleprint-1.0.3/src/ConsolePrint/animate.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 consoleprint-1.0.3/src/ConsolePrint/console2file.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 consoleprint-1.0.3/src/ConsolePrint/loading.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 consoleprint-1.0.3/tests/tests.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 consoleprint-1.0.3/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 consoleprint-1.0.3/LICENSE
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 consoleprint-1.0.3/README.md
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 consoleprint-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 consoleprint-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 consoleprint-1.2.1/src/ConsolePrint/__init__.py
+-rw-r--r--   0        0        0     7621 2020-02-02 00:00:00.000000 consoleprint-1.2.1/src/ConsolePrint/animate.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 consoleprint-1.2.1/src/ConsolePrint/console2file.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 consoleprint-1.2.1/src/ConsolePrint/formats.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 consoleprint-1.2.1/src/ConsolePrint/loading.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 consoleprint-1.2.1/tests/tests.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 consoleprint-1.2.1/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 consoleprint-1.2.1/LICENSE
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 consoleprint-1.2.1/README.md
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 consoleprint-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 consoleprint-1.2.1/PKG-INFO
```

### Comparing `consoleprint-1.0.3/src/ConsolePrint/console2file.py` & `consoleprint-1.2.1/src/ConsolePrint/console2file.py`

 * *Files identical despite different names*

### Comparing `consoleprint-1.0.3/src/ConsolePrint/loading.py` & `consoleprint-1.2.1/src/ConsolePrint/loading.py`

 * *Files identical despite different names*

### Comparing `consoleprint-1.0.3/tests/tests.py` & `consoleprint-1.2.1/tests/tests.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Test codes.  Ensure you have installed the module first using: pip install ConsolePrint
 
 # animate.py
 import ConsolePrint.animate as prt
 
-prt.printing("hello this should print letter by letter", delay=0.05, style="letter", stay=True, rev=False)
-prt.printing("hello this should print word by word but in reverse", delay=0.05, style="word", stay=True, rev=True)
-prt.flashprint("The entire text should flash", blinks=5, delay=0.2, stay=True)
-prt.flashtext("The text in  will flash", "UPPER CASE", blinks=5, index=12, delay=0.2)
-prt.animate1("This text is animated with #", symbol="#")
-prt.animate2("Prints letter by letter but masked with # first", symbol="#", delay=0.05)
-prt.text_box("C O D E  B R E A K E R", symbol="#", padding=True, wall=True, align="right")
-prt.star_square(8, symbol="@")
+prt.printing("hello this should print letter by letter", delay=0.05, style="letter", stay=True, rev=False, format=strike)
+prt.printing("hello this should print word by word but in reverse", delay=0.3, style="word", stay=True, rev=True, format=red_bg)
+prt.flashprint("The entire text should flash", blinks=5, delay=0.2, stay=True, format=green)
+prt.flashtext("The text in  will flash", "UPPER CASE", blinks=5, index=12, delay=0.2, format=yellow)
+prt.animate1("This text is animated with #", symbol="#", format=white)
+prt.animate2("Prints letter by letter but masked with # first  ", symbol="#", delay=0.05, format="\033[48;5;150m")
+prt.text_box("B O X E D  I N", symbol="#", padding=True, wall=True, align='right', format='\033[48;5;4m')
+prt.star_square(10, symbol="@", align=15, flush="True", format="\033[104m")
+prt.asteriskify('This has been asteriskified', align='center', underscore=True, format=cyan)
 
 # console2file.pt
 import ConsolePrint.console2file as file
 import calendar
 
 file.startConsoleSave()
```

### Comparing `consoleprint-1.0.3/LICENSE` & `consoleprint-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `consoleprint-1.0.3/README.md` & `consoleprint-1.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,24 @@
+Metadata-Version: 2.1
+Name: ConsolePrint
+Version: 1.2.1
+Summary: A package to animate and beautify print output to console
+Project-URL: Homepage, https://github.com/iloabachie/ConsolePrint
+Project-URL: Bug Tracker, https://github.com/iloabachie/ConsolePrint/issues
+Author-email: Udemezue Iloabachie <udemezue@gmail.com>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 # ConsolePrint
 This module making printing to the terminal more exciting by animating the text output.
+It also makes output richer my modifying the color
 You can also save routine console output to a file using the console2file module.
 Created using python 3.11
 
 # Installation
 You may install it form PyPI.org using the pip command.
 
 pip install ConsolePrint
@@ -14,39 +29,47 @@
 import ConsolePrint.animate as prt    
 
 import ConsolePrint.console2file as file  
 
 import ConsolePrint.loading as load        
 
 # Test Cases
-You may change the arguments as desired
+1.  Here uou may change the arguments as desired
 
 file.startConsoleSave()
 
 'Saves all output between the start and end functions to file.'
 
 from calendar import calendar
 
 print(calendar(2023))
 
 file.endConsoleSave()
 
-prt.printing("hello this should print letter by letter", delay=0.05, style="letter", new_line=True, rev=False)
+2. Here you may use ANSI escape sequences for the format argument and change others as desired.
+
+prt.printing("hello this should print letter by letter      ", delay=0.05, style="letter", stay=True, rev=False, format=strike)
+
+prt.printing("hello this should print word by word but in reverse", delay=0.3, style="word", stay=True, rev=True, format=red_bg)
+
+prt.flashprint("The entire text should flash", blinks=5, delay=0.2, stay=True, format=green)
+
+prt.flashtext("The text in  will flash", "UPPER CASE", blinks=5, index=12, delay=0.2, format=yellow)
 
-prt.printing("hello this should print word by word but in reverse", delay=0.05, style="word", new_line=True, rev=True)
+prt.animate1("This text is animated with #", symbol="#", format=white)
 
-prt.flashprint("The entire text should flash", flashes=5, delay=0.2, stay=True)
+prt.animate2("Prints letter by letter but masked with # first  ", symbol="#", delay=0.05, format="\033[48;5;150m")
 
-prt.flashtext("The text in  will flash", "UPPER CASE", blinks=5, index=12, delay=0.2)
+prt.text_box("B O X E D  I N", symbol="#", padding=True, wall=True, align='right', format='\033[48;5;4m')
 
-prt.animate1("This text is animated with #", symbol="#")
+prt.star_square(10, symbol="@", align=15, flush="True", format="\033[104m")
 
-prt.animate2("Prints letter by letter but masked with # first", symbol="#", delay=0.05)
+prt.format('This has been asteriskified', align='center', underscore=True, format=cyan)
 
-prt.text_box("M O N E Y  M A K E R", symbol="$", padding=True, wall=True)
+3.  Here, the load time is specified in seconds
 
 load.countdown(5)
 
 load.loading1(10)
 
 print()
```

### Comparing `consoleprint-1.0.3/pyproject.toml` & `consoleprint-1.2.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ConsolePrint"
-version = "1.0.3"
+version = "1.2.1"
 authors = [
   { name="Udemezue Iloabachie", email="udemezue@gmail.com" },
 ]
-description = "A package to animate print output to console"
+description = "A package to animate and beautify print output to console"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `consoleprint-1.0.3/PKG-INFO` & `consoleprint-1.2.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,10 @@
-Metadata-Version: 2.1
-Name: ConsolePrint
-Version: 1.0.3
-Summary: A package to animate print output to console
-Project-URL: Homepage, https://github.com/iloabachie/ConsolePrint
-Project-URL: Bug Tracker, https://github.com/iloabachie/ConsolePrint/issues
-Author-email: Udemezue Iloabachie <udemezue@gmail.com>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 # ConsolePrint
 This module making printing to the terminal more exciting by animating the text output.
+It also makes output richer my modifying the color
 You can also save routine console output to a file using the console2file module.
 Created using python 3.11
 
 # Installation
 You may install it form PyPI.org using the pip command.
 
 pip install ConsolePrint
@@ -28,39 +15,47 @@
 import ConsolePrint.animate as prt    
 
 import ConsolePrint.console2file as file  
 
 import ConsolePrint.loading as load        
 
 # Test Cases
-You may change the arguments as desired
+1.  Here uou may change the arguments as desired
 
 file.startConsoleSave()
 
 'Saves all output between the start and end functions to file.'
 
 from calendar import calendar
 
 print(calendar(2023))
 
 file.endConsoleSave()
 
-prt.printing("hello this should print letter by letter", delay=0.05, style="letter", new_line=True, rev=False)
+2. Here you may use ANSI escape sequences for the format argument and change others as desired.
+
+prt.printing("hello this should print letter by letter      ", delay=0.05, style="letter", stay=True, rev=False, format=strike)
+
+prt.printing("hello this should print word by word but in reverse", delay=0.3, style="word", stay=True, rev=True, format=red_bg)
+
+prt.flashprint("The entire text should flash", blinks=5, delay=0.2, stay=True, format=green)
+
+prt.flashtext("The text in  will flash", "UPPER CASE", blinks=5, index=12, delay=0.2, format=yellow)
 
-prt.printing("hello this should print word by word but in reverse", delay=0.05, style="word", new_line=True, rev=True)
+prt.animate1("This text is animated with #", symbol="#", format=white)
 
-prt.flashprint("The entire text should flash", flashes=5, delay=0.2, stay=True)
+prt.animate2("Prints letter by letter but masked with # first  ", symbol="#", delay=0.05, format="\033[48;5;150m")
 
-prt.flashtext("The text in  will flash", "UPPER CASE", blinks=5, index=12, delay=0.2)
+prt.text_box("B O X E D  I N", symbol="#", padding=True, wall=True, align='right', format='\033[48;5;4m')
 
-prt.animate1("This text is animated with #", symbol="#")
+prt.star_square(10, symbol="@", align=15, flush="True", format="\033[104m")
 
-prt.animate2("Prints letter by letter but masked with # first", symbol="#", delay=0.05)
+prt.format('This has been asteriskified', align='center', underscore=True, format=cyan)
 
-prt.text_box("M O N E Y  M A K E R", symbol="$", padding=True, wall=True)
+3.  Here, the load time is specified in seconds
 
 load.countdown(5)
 
 load.loading1(10)
 
 print()
```

