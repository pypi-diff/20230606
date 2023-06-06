# Comparing `tmp/consoleprint-1.2.2.tar.gz` & `tmp/consoleprint-1.2.4.tar.gz`

## Comparing `consoleprint-1.2.2.tar` & `consoleprint-1.2.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 consoleprint-1.2.2/src/ConsolePrint/__init__.py
--rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 consoleprint-1.2.2/src/ConsolePrint/animate.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 consoleprint-1.2.2/src/ConsolePrint/console2file.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 consoleprint-1.2.2/src/ConsolePrint/loading.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 consoleprint-1.2.2/tests/tests.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 consoleprint-1.2.2/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 consoleprint-1.2.2/LICENSE
--rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 consoleprint-1.2.2/README.md
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 consoleprint-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 consoleprint-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 consoleprint-1.2.4/src/ConsolePrint/__init__.py
+-rw-r--r--   0        0        0     9439 2020-02-02 00:00:00.000000 consoleprint-1.2.4/src/ConsolePrint/animate.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 consoleprint-1.2.4/src/ConsolePrint/console2file.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 consoleprint-1.2.4/src/ConsolePrint/loading.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 consoleprint-1.2.4/tests/tests.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 consoleprint-1.2.4/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 consoleprint-1.2.4/LICENSE
+-rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 consoleprint-1.2.4/README.md
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 consoleprint-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 consoleprint-1.2.4/PKG-INFO
```

### Comparing `consoleprint-1.2.2/src/ConsolePrint/animate.py` & `consoleprint-1.2.4/src/ConsolePrint/animate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,52 @@
 import time
 import os
 
-# Font Colors
-reset = '\033[0m'
-grey = '\033[30m'
-red = '\033[31m'
-green = '\033[32m'
-yellow = '\033[33m'
-blue = '\033[34m'
-magenta = '\033[35m'
-cyan = '\033[36m'
-white = '\033[37m'
-
-
-# Text Formats
-bold = '\033[1m'
-italics = '\033[3m'
-underscore = '\033[4m'
-strike = '\033[9m'
-double_under = '\033[21m'
-red_bg = '\033[41m'
-green_bg = '\033[42m'
-yellow_bg = '\033[43m'
-blue_bg = '\033[44m'
-magenta_bg = '\033[45m'
-cyan_bg = '\033[46m'
-white_bg = '\033[47m'
+def ansify_color(color):  
+    match color:
+        #colours
+        case 'default': color = '\033[0m'
+        case 'grey': color = '\033[30m'
+        case 'red': color = '\033[31m'
+        case 'green': color = '\033[32m'
+        case 'yellow': color = '\033[33m'
+        case 'blue': color = '\033[34m'
+        case 'magenta': color = '\033[35m'
+        case 'cyan': color = '\033[36m'
+        case 'white': color = '\033[37m'
+        # Text Formats
+        case 'bold': color = '\033[1m'
+        case 'italics': color = '\033[3m'
+        case 'underscore': color = '\033[4m'
+        case 'strike': color = '\033[9m'
+        case 'double_under': color = '\033[21m'
+        case 'red_bg': color = '\033[41m'
+        case 'green_bg': color = '\033[42m'
+        case 'yellow_bg': color = '\033[43m'
+        case 'blue_bg': color = '\033[44m'
+        case 'magenta_bg': color = '\033[45m'
+        case 'cyan_bg': color = '\033[46m'
+        case 'white_bg': color = '\033[47m'
+    if '[' not in color or color[-1] != 'm' or not color[2:3].isdigit():
+        raise Exception("Invalid ANSI escape sequence for argument format")
+    return color
 
-terminal_width = os.get_terminal_size().columns
 
+if __name__ == "__main__":
+    os.system('cls')
+    print('\033[0m', end="\r")
+    print((terminal_size:=os.get_terminal_size()))
+    print(f'{terminal_size.columns = }, {terminal_size.lines = }')
+    print()
+
+terminal_width = os.get_terminal_size().columns
 
-def printing(text: str, delay=0.05, style='letter', stay=True, rev=False, format=reset):
+def printing(text: str, delay=0.05, style='letter', stay=True, rev=False, format: str='default'):
     """Prints text to console letter by letter or word by word"""
+    format = ansify_color(format)
     print(format, end='\r')
     text = text.strip()
     match rev:
         case False:
             if style.lower() == 'letter':
                 for _ in range(len(text)):
                     print(text[:_ + 1], end='\r')
@@ -53,31 +64,33 @@
             elif style.lower() == 'word':
                 text = text.split(' ')
                 for _ in range(len(text)):
                     print(' '.join(text[-1 - _:]), end='\r')
                     time.sleep(delay)
     if stay:
         print()
-    print(reset, end='\r')
+    print('\033[0m', end='\r')
 
 
-def flashprint(text: str, blinks=5, delay=0.2, stay=True, format=reset):
+def flashprint(text: str, blinks=5, delay=0.2, stay=True, format: str='default'):
     """Gets printed output to blink"""
+    format = ansify_color(format)
     print(format, end='\r')
     text = text.strip()
     for _ in range(blinks):
         print(text, end='\r'), time.sleep(delay)
         print(' ' * len(text), end='\r'), time.sleep(delay)
     if stay:
         print(text)
-    print(reset, end='\r')
+    print('\033[0m', end='\r')
 
 
-def flashtext(phrase: str, text: str, index='end', blinks=5, delay=0.2, format=reset):
+def flashtext(phrase: str, text: str, index='end', blinks=5, delay=0.2, format: str='default'):
     """Hilights key word by flashing it"""
+    format = ansify_color(format)
     print(format, end='\r')
     text = text.strip()
     phrase = phrase.strip()
     textb = ' ' * len(text)
     if index == 'end':
         phrase1 = phrase
         phrase2 = ''
@@ -87,41 +100,44 @@
 
     for _ in range(blinks):
         print(phrase1 + text + phrase2, end='\r')
         time.sleep(delay)
         print(phrase1 + textb + phrase2, end='\r')
         time.sleep(delay)
     print(phrase1 + text + phrase2)
-    print(reset, end='\r')
+    print('\033[0m', end='\r')
 
 
-def animate1(text: str, symbol="#", format=reset):
+def animate1(text: str, symbol="#", format: str='default'):
     """Flashing masked text to transition to flasing text"""
+    format = ansify_color(format)
     print(format, end='\r')
     text = text.strip()
     symbol = len(text) * symbol
     flashprint(symbol, blinks=3, stay=False)
     flashprint(text, blinks=2, stay=True)
-    print(reset, end='\r')
+    print('\033[0m', end='\r')
 
 
-def animate2(text: str, symbol="#", delay=0.05, format=reset):
+def animate2(text: str, symbol="#", delay=0.05, format: str='default'):
     """Reveals all characters text by text but first masked then flashes"""
+    format = ansify_color(format)
     print(format, end='\r')
     text = text.strip()
     symbol = len(text) * symbol
     for _ in symbol + "\r" + text + "\r":
         print(_, end="", flush=True)
         time.sleep(delay)
     flashprint(text, blinks=2, stay=True, format=format)
-    print(reset, end='\r')
+    print('\033[0m', end='\r')
 
-def text_box(text: str, symbol="#", padding: bool=False, wall: bool=True, align="center", format=reset):
+def text_box(text: str, symbol="#", padding: bool=False, wall: bool=True, align="center", format: str='default'):
     """Prints text in a box of symbols.
 If the align parameter is a number then the box is indented by the number count"""
+    format = ansify_color(format)
     print(format, end='\r')
     text = text.strip()
     end = 5 if padding else 3
     text_row = 3 if padding else 2
     length = len(text) + 8
     left_border = text_row - 1  if padding else text_row
     right_border = text_row + 1 if padding else text_row
@@ -131,15 +147,15 @@
     elif align == "center": indent = terminal_width//2 - length//2
     elif isinstance(align, int) and align <= (terminal_width - length): indent = align
     else: raise Exception(f"Error in the align argument: {align=}")  
     
     for row in range(1, end + 1):
         for col in range(1, length + 1):
             if col == 1:
-                print(reset + (" " * indent) + format, end="")
+                print('\033[0m' + (" " * indent) + format, end="")
             if row == 1 or row == end or col == 1 or col == length:
                 if wall:
                     print(symbol, end="")
                 else:
                     if left_border <= row <= right_border:
                         print(" ", end="") 
                     else:
@@ -147,29 +163,30 @@
             elif row == text_row:
                 if col == 3:
                     print("{:^{}}".format(text, length-2), end="")
             else:
                 print(" ", end="")  
             if col == length:
                 print()
-    print(reset, end='\r')
+    print('\033[0m', end='\r')
                 
                 
-def star_square(num: int, symbol: str="#", align: str='center', flush: bool=True, format=reset):
+def star_square(num: int, symbol: str="#", align: str='center', flush: bool=True, format: str='default'):
+    format = ansify_color(format)
     print(format, end='\r')
     if num < 5 or num > terminal_width or not isinstance(num, int):
         raise Exception(f"Invalid square size. Number must be an integer greater than 4 and less than the terminal width: {terminal_width}")
     elif align == 'center':
-        indent = reset + (' ' * (terminal_width//2 - num//2)) + format
+        indent = '\033[0m' + (' ' * (terminal_width//2 - num//2)) + format
     elif align == 'right':
-        indent = reset + (' ' * (terminal_width - num)) + format
+        indent = '\033[0m' + (' ' * (terminal_width - num)) + format
     elif align == 'left':
         indent = ''  
     elif isinstance(align, int) and terminal_width - align > num:
-        indent = reset + (" " * align) + format
+        indent = '\033[0m' + (" " * align) + format
     else:
         raise Exception("Align parameter is invalid")    
           
     for row in range(1, num + 1):
         # time.sleep(0.04)
         print(indent, end="")
         for col in range(1, num + 1):
@@ -180,40 +197,41 @@
                 print(symbol, end="", flush=flush)
             elif row + col == num + 1:
                 print(symbol, end="", flush=flush)  
             else:
                 print(" ", end="", flush=flush)              
             if col == num:
                 print()
-    print(reset, end='\r')
+    print('\033[0m', end='\r')
     
 
-def asteriskify(text: str, align: str="left", underscore: bool=False, format=reset):
+def asteriskify(text: str, align: str="left", underscore: bool=False, format: str='default'):
+    format = ansify_color(format)
     print(format, end='\r')
     text = text.strip()
     length = len(text)
     
     if align == 'center':
-        indent = ' ' * (terminal_width//2 - length//2)
+        indent = '\033[0m' + ' ' * (terminal_width//2 - length//2) + format
     elif align == 'right':
-        indent = ' ' * (terminal_width - length)
+        indent = '\033[0m' + ' ' * (terminal_width - length) + format
     elif align == 'left':
         indent = ''
     else:
         raise Exception("Align argument error") 
     print(indent + text)
     if underscore:
         print(indent + '*' * length)
-    print(reset, end='\r')
+    print('\033[0m', end='\r')
     
 
 # Code test
 if __name__ == "__main__":
-    printing("hello this should print letter by letter      ", delay=0.05, style="letter", stay=True, rev=False, format=magenta)
-    printing("hello this should print word by word but in reverse", delay=0.3, style="word", stay=True, rev=True, format=red)
-    flashprint("The entire text should flash", blinks=5, delay=0.2, stay=True, format=green)
-    flashtext("The text in  will flash", "UPPER CASE", blinks=5, index=12, delay=0.2, format=yellow)
-    animate1("This text is animated with #", symbol="#", format=white)
+    printing("hello this should print letter by letter      ", delay=0.05, style="letter", stay=True, rev=False, format='magenta')
+    printing("hello this should print word by word but in reverse", delay=0.3, style="word", stay=True, rev=True, format='red')
+    flashprint("The entire text should flash", blinks=5, delay=0.2, stay=True, format='green')
+    flashtext("The text in  will flash", "UPPER CASE", blinks=5, index=12, delay=0.2, format='yellow')
+    animate1("This text is animated with #", symbol="#", format='white')
     animate2("Prints letter by letter but masked with # first  ", symbol="#", delay=0.05, format="\033[48;5;150m")
     text_box("B O X E D  I N", symbol="#", padding=True, wall=True, align='center', format='\033[48;5;4m')
     star_square(10, symbol="@", align=15, flush="True", format="\033[104m")
-    asteriskify('This has been asteriskified', align='center', underscore=True, format=cyan)
+    asteriskify('This has been asteriskified', align='center', underscore=True, format='cyan')
```

### Comparing `consoleprint-1.2.2/src/ConsolePrint/console2file.py` & `consoleprint-1.2.4/src/ConsolePrint/console2file.py`

 * *Files identical despite different names*

### Comparing `consoleprint-1.2.2/src/ConsolePrint/loading.py` & `consoleprint-1.2.4/src/ConsolePrint/loading.py`

 * *Files identical despite different names*

### Comparing `consoleprint-1.2.2/tests/tests.py` & `consoleprint-1.2.4/tests/tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Test codes.  Ensure you have installed the module first using: pip install ConsolePrint
 
 # animate.py
 import ConsolePrint.animate as prt
 
-prt.printing("hello this should print letter by letter", delay=0.05, style="letter", stay=True, rev=False, format=strike)
-prt.printing("hello this should print word by word but in reverse", delay=0.3, style="word", stay=True, rev=True, format=red_bg)
-prt.flashprint("The entire text should flash", blinks=5, delay=0.2, stay=True, format=green)
-prt.flashtext("The text in  will flash", "UPPER CASE", blinks=5, index=12, delay=0.2, format=yellow)
-prt.animate1("This text is animated with #", symbol="#", format=white)
+prt.printing("hello this should print letter by letter", delay=0.05, style="letter", stay=True, rev=False, format='strike')
+prt.printing("hello this should print word by word but in reverse", delay=0.3, style="word", stay=True, rev=True, format='red_bg')
+prt.flashprint("The entire text should flash", blinks=5, delay=0.2, stay=True, format='green')
+prt.flashtext("The text in  will flash", "UPPER CASE", blinks=5, index=12, delay=0.2, format='yellow')
+prt.animate1("This text is animated with #", symbol="#", format='white')
 prt.animate2("Prints letter by letter but masked with # first  ", symbol="#", delay=0.05, format="\033[48;5;150m")
-prt.text_box("B O X E D  I N", symbol="#", padding=True, wall=True, align='right', format='\033[48;5;4m')
+prt.text_box("B O X E D  I N", symbol="#", padding=True, wall=True, align='center', format='\033[48;5;4m')
 prt.star_square(10, symbol="@", align=15, flush="True", format="\033[104m")
-prt.asteriskify('This has been asteriskified', align='center', underscore=True, format=cyan)
+prt.asteriskify('This has been asteriskified', align='center', underscore=True, format='cyan')
 
 # console2file.pt
 import ConsolePrint.console2file as file
 import calendar
 
 file.startConsoleSave()
```

### Comparing `consoleprint-1.2.2/LICENSE` & `consoleprint-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `consoleprint-1.2.2/README.md` & `consoleprint-1.2.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: ConsolePrint
+Version: 1.2.4
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
 It also makes output richer my modifying the color
 You can also save routine console output to a file using the console2file module.
 Created using python 3.11
 
 # Installation
@@ -28,32 +42,54 @@
 from calendar import calendar
 
 print(calendar(2023))
 
 file.endConsoleSave()
 
 2. Here you may use ANSI escape sequences for the format argument and change others as desired.
+Preset arguments for format:
+//colours
+'default':          '\033[0m'
+'grey':             '\033[30m'
+'red':              '\033[31m'
+'green':            '\033[32m'
+'yellow':           '\033[33m'
+'blue':             '\033[34m'
+'magenta':          '\033[35m'
+'cyan':             '\033[36m'
+'white':            '\033[37m'
+//Text Formats
+'bold':             '\033[1m'
+'italics':          '\033[3m'
+'underscore':       '\033[4m'
+'strike':           '\033[9m'
+'double_under':     '\033[21m'
+'red_bg':           '\033[41m'
+'green_bg':         '\033[42m'
+'yellow_bg':        '\033[43m'
+'blue_bg':          '\033[44m'
+'magenta_bg':       '\033[45m'
+'cyan_bg':          '\033[46m'
+'white_bg':         '\033[47m'
+
+prt.printing("hello this should print letter by letter", delay=0.05, style="letter", stay=True, rev=False, format='strike')
 
-prt.printing("hello this should print letter by letter      ", delay=0.05, style="letter", stay=True, rev=False, format=strike)
-
-prt.printing("hello this should print word by word but in reverse", delay=0.3, style="word", stay=True, rev=True, format=red_bg)
+prt.printing("hello this should print word by word but in reverse", delay=0.3, style="word", stay=True, rev=True, format='red_bg')
 
-prt.flashprint("The entire text should flash", blinks=5, delay=0.2, stay=True, format=green)
+prt.flashprint("The entire text should flash", blinks=5, delay=0.2, stay=True, format='green')
 
-prt.flashtext("The text in  will flash", "UPPER CASE", blinks=5, index=12, delay=0.2, format=yellow)
+prt.flashtext("The text in  will flash", "UPPER CASE", blinks=5, index=12, delay=0.2, format='yellow')
 
-prt.animate1("This text is animated with #", symbol="#", format=white)
+prt.animate1("This text is animated with #", symbol="#", format='white')
 
 prt.animate2("Prints letter by letter but masked with # first  ", symbol="#", delay=0.05, format="\033[48;5;150m")
 
-prt.text_box("B O X E D  I N", symbol="#", padding=True, wall=True, align='right', format='\033[48;5;4m')
-
-prt.star_square(10, symbol="@", align=15, flush="True", format="\033[104m")
+prt.text_box("B O X E D  I N", symbol="#", padding=True, wall=True, align='center', format='\033[48;5;4m')
 
-prt.format('This has been asteriskified', align='center', underscore=True, format=cyan)
+prt.asteriskify('This has been asteriskified', align='center', underscore=True, format='cyan')
 
 3.  Here, the load time is specified in seconds
 
 load.countdown(5)
 
 load.loading1(10)
```

### Comparing `consoleprint-1.2.2/pyproject.toml` & `consoleprint-1.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ConsolePrint"
-version = "1.2.2"
+version = "1.2.4"
 authors = [
   { name="Udemezue Iloabachie", email="udemezue@gmail.com" },
 ]
 description = "A package to animate and beautify print output to console"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

