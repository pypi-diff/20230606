# Comparing `tmp/inputty-1.0.2.tar.gz` & `tmp/inputty-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inputty-1.0.2.tar", last modified: Tue Jun  6 16:49:35 2023, max compression
+gzip compressed data, was "inputty-1.0.3.tar", last modified: Tue Jun  6 16:52:30 2023, max compression
```

## Comparing `inputty-1.0.2.tar` & `inputty-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-06 16:49:35.572835 inputty-1.0.2/
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 inputty-1.0.2/LICENSE.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1108 2023-06-06 16:49:35.572835 inputty-1.0.2/PKG-INFO
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)       96 2023-05-09 13:23:03.000000 inputty-1.0.2/README.md
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-06 16:49:35.566168 inputty-1.0.2/inputty/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      124 2023-05-09 13:45:56.000000 inputty-1.0.2/inputty/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-06-06 16:46:52.000000 inputty-1.0.2/inputty/_version.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-06 16:49:35.569501 inputty-1.0.2/inputty/src/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:37:49.000000 inputty-1.0.2/inputty/src/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     7787 2023-06-06 10:20:18.000000 inputty-1.0.2/inputty/src/input.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-06 16:49:35.569501 inputty-1.0.2/inputty/tests/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-29 12:23:03.000000 inputty-1.0.2/inputty/tests/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3230 2023-05-30 11:09:18.000000 inputty-1.0.2/inputty/tests/test_input.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      339 2023-05-31 08:29:56.000000 inputty-1.0.2/inputty/xxx.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-06 16:49:35.566168 inputty-1.0.2/inputty.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1108 2023-06-06 16:49:35.000000 inputty-1.0.2/inputty.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)      318 2023-06-06 16:49:35.000000 inputty-1.0.2/inputty.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-06-06 16:49:35.000000 inputty-1.0.2/inputty.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        8 2023-06-06 16:49:35.000000 inputty-1.0.2/inputty.egg-info/top_level.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-06-06 16:49:35.572835 inputty-1.0.2/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1157 2023-05-09 13:25:02.000000 inputty-1.0.2/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-06 16:52:30.119789 inputty-1.0.3/
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 inputty-1.0.3/LICENSE.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1161 2023-06-06 16:52:30.119789 inputty-1.0.3/PKG-INFO
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)       96 2023-05-09 13:23:03.000000 inputty-1.0.3/README.md
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-06 16:52:30.119789 inputty-1.0.3/inputty/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      124 2023-05-09 13:45:56.000000 inputty-1.0.3/inputty/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-06-06 16:52:09.000000 inputty-1.0.3/inputty/_version.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-06 16:52:30.119789 inputty-1.0.3/inputty/src/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:37:49.000000 inputty-1.0.3/inputty/src/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     8058 2023-06-06 16:52:25.000000 inputty-1.0.3/inputty/src/input.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-06 16:52:30.119789 inputty-1.0.3/inputty/tests/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-29 12:23:03.000000 inputty-1.0.3/inputty/tests/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3230 2023-05-30 11:09:18.000000 inputty-1.0.3/inputty/tests/test_input.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      339 2023-05-31 08:29:56.000000 inputty-1.0.3/inputty/xxx.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-06 16:52:30.119789 inputty-1.0.3/inputty.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1161 2023-06-06 16:52:29.000000 inputty-1.0.3/inputty.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      318 2023-06-06 16:52:30.000000 inputty-1.0.3/inputty.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-06-06 16:52:29.000000 inputty-1.0.3/inputty.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        8 2023-06-06 16:52:29.000000 inputty-1.0.3/inputty.egg-info/top_level.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-06-06 16:52:30.123123 inputty-1.0.3/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1157 2023-05-09 13:25:02.000000 inputty-1.0.3/setup.py
```

### Comparing `inputty-1.0.2/LICENSE.txt` & `inputty-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `inputty-1.0.2/PKG-INFO` & `inputty-1.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inputty
-Version: 1.0.2
+Version: 1.0.3
 Summary: """A collection of modules that supports cCLI inputs."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: cli,input
@@ -20,14 +20,18 @@
 ```bash
 pip install inputty
 ```
 
 
 # Version History
 
+Version 1.0.3 6 June 2023
+
+1. Actually make changes
+
 Version 1.0.2 6 June 2023
 
 1. Allow the capture of a string
 2. Add extra args with INTEGERS
 3. Add space to end of prompt
 
 ------
```

### Comparing `inputty-1.0.2/inputty/src/input.py` & `inputty-1.0.3/inputty/src/input.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 ERROR_COLOUR = 'red'
 INVALID_SPEC_MSG = 'Invalid specification for process:'
 INVALID_INPUT_MSG = 'Invalid input.'
 USE_ONE_OF_MSG = 'Use one of'
 INTEGER_RANGE_MSG = 'Integer outside valid range:'
 
 RETURN = '<RTN>'
+STRING = '<STRING>'
 INTEGER_SELECTION = '<INTEGERS>'
 INTEGER_BASE = 1
 
 __all__ = ['Input']
 
 
 class Input():
@@ -37,15 +38,15 @@
         The process object is the function to be called when the input is the key
         the list contains the parameters to be passed to the function.
         The second definition includes a two-ple for min_integer and max_integer
 
         An example process:
 
             processes = {
-                '<INTEGERS>': (function_one, [], (min_integer, max_integer)),
+                '<INTEGERS>': (function_one, [arg], (min_integer, max_integer)),
                 '<RTN>': (function_two, []),
                 'S': (function_three, [files_to_copy]),
                 'Q': (quit, []),
             }
         If the process key is <RTN> (RETURN) then a null input will invoke the associated process.
 
         If the process key is <INTEGERS> (INTEGER_SELECTION) then a valid input is created for
@@ -69,15 +70,15 @@
     or,
         my_input = Input(prompt, processes)
         my_input()
     """
     def __init__(self, prompt: str,
                  processes: dict[str, Tuple[object, List[object]]],
                  validation: dict[str, object] = {}):
-        self.prompt = prompt
+        self.prompt = prompt.strip() + ' '
         self.processes = self._generate_processes(processes)
         self.validation = validation
         self.message_list = self._get_message_list(processes)
         self .response = None
         self.error_colour = ERROR_COLOUR
         # Are valid inputs to be included in the error message?
         self.include_valid_in_error = True
@@ -111,18 +112,22 @@
             response = input(self.prompt)
 
             # Handle null input
             if not response:
                 if RETURN in self.processes:
                     return RETURN
                 continue
-
             if response in self.processes:
                 return response
-            elif self.validation:
+
+            # Capture string
+            if STRING in self.processes:
+                return response
+
+            if self.validation:
                 return self.validate_input(response)
             cprint(f"{self._input_error_message}", self.error_colour)
 
     def validate_input(self, response):
         # Return a valid input string having validated input.
         if 'integer' in self.validation:
             return self.validate_integer(response)
@@ -184,15 +189,18 @@
         integer_processes = {}
         for key in processes:
             if key == INTEGER_SELECTION:
                 Input._validate_integers(key, processes[key])
                 (min_, max_) = Input._get_integers_min_max(processes[key])
                 integer_range = range(min_, max_+1)
                 for index in integer_range:
-                    integer_processes[str(index)] = (processes[key][0], [index])
+                    args = [index]
+                    if processes[key][1]:
+                        args = [index] + processes[key][1]
+                    integer_processes[str(index)] = (processes[key][0], args)
         return integer_processes
 
     @staticmethod
     def _get_integers_min_max(process):
         if isinstance(process[2], int):
             return (INTEGER_BASE, process[2])
         else:
```

### Comparing `inputty-1.0.2/inputty/tests/test_input.py` & `inputty-1.0.3/inputty/tests/test_input.py`

 * *Files identical despite different names*

### Comparing `inputty-1.0.2/inputty.egg-info/PKG-INFO` & `inputty-1.0.3/inputty.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inputty
-Version: 1.0.2
+Version: 1.0.3
 Summary: """A collection of modules that supports cCLI inputs."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: cli,input
@@ -20,14 +20,18 @@
 ```bash
 pip install inputty
 ```
 
 
 # Version History
 
+Version 1.0.3 6 June 2023
+
+1. Actually make changes
+
 Version 1.0.2 6 June 2023
 
 1. Allow the capture of a string
 2. Add extra args with INTEGERS
 3. Add space to end of prompt
 
 ------
```

### Comparing `inputty-1.0.2/setup.py` & `inputty-1.0.3/setup.py`

 * *Files identical despite different names*

