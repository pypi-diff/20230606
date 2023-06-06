# Comparing `tmp/byu_pytest_utils-0.6.1.tar.gz` & `tmp/byu_pytest_utils-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byu_pytest_utils-0.6.1.tar", max compression
+gzip compressed data, was "byu_pytest_utils-0.6.3.tar", max compression
```

## Comparing `byu_pytest_utils-0.6.1.tar` & `byu_pytest_utils-0.6.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1062 2023-04-21 21:42:09.303677 byu_pytest_utils-0.6.1/byu_pytest_utils/__init__.py
--rw-r--r--   0        0        0      714 2022-03-14 21:00:52.263812 byu_pytest_utils-0.6.1/byu_pytest_utils/decorators.py
--rw-r--r--   0        0        0     9913 2023-05-09 20:05:05.372932 byu_pytest_utils-0.6.1/byu_pytest_utils/dialog.py
--rw-r--r--   0        0        0     3088 2023-03-04 23:37:17.852701 byu_pytest_utils-0.6.1/byu_pytest_utils/edit_dist.py
--rw-r--r--   0        0        0     3595 2023-03-06 23:42:26.126776 byu_pytest_utils-0.6.1/byu_pytest_utils/pytest_plugin.py
--rw-r--r--   0        0        0     3474 2023-04-21 21:39:00.608118 byu_pytest_utils-0.6.1/byu_pytest_utils/utils.py
--rw-r--r--   0        0        0      562 2023-05-09 20:05:17.878302 byu_pytest_utils-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 byu_pytest_utils-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-06 21:35:25.303938 byu_pytest_utils-0.6.3/byu_pytest_utils/__init__.py
+-rw-r--r--   0        0        0      714 2023-06-06 21:35:25.305612 byu_pytest_utils-0.6.3/byu_pytest_utils/decorators.py
+-rw-r--r--   0        0        0    10070 2023-06-06 21:36:21.100032 byu_pytest_utils-0.6.3/byu_pytest_utils/dialog.py
+-rw-r--r--   0        0        0     3088 2023-03-04 23:37:17.852701 byu_pytest_utils-0.6.3/byu_pytest_utils/edit_dist.py
+-rw-r--r--   0        0        0     3595 2023-03-06 23:42:26.126776 byu_pytest_utils-0.6.3/byu_pytest_utils/pytest_plugin.py
+-rw-r--r--   0        0        0     3474 2023-04-21 21:39:00.608118 byu_pytest_utils-0.6.3/byu_pytest_utils/utils.py
+-rw-r--r--   0        0        0      562 2023-06-06 21:36:21.064538 byu_pytest_utils-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 byu_pytest_utils-0.6.3/PKG-INFO
```

### Comparing `byu_pytest_utils-0.6.1/byu_pytest_utils/__init__.py` & `byu_pytest_utils-0.6.3/byu_pytest_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.6.1/byu_pytest_utils/decorators.py` & `byu_pytest_utils-0.6.3/byu_pytest_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.6.1/byu_pytest_utils/dialog.py` & `byu_pytest_utils-0.6.3/byu_pytest_utils/dialog.py`

 * *Files 3% similar despite different names*

```diff
@@ -217,25 +217,27 @@
             'sys': sys
         }
 
         # Run script as __main__
         try:
             runpy.run_path(script_name, _globals, module)
 
+            if output_file is not None:
+                if os.path.exists(output_file):
+                    with open(output_file) as output:
+                        group_stats = self._score_output(output.read())
+                else:
+                    group_stats = self._score_output(f"File not found: {output_file}. Did you write it?")
+            else:
+                group_stats = self._score_output(self.observed_output)
+
         except Exception as ex:
             # get stack trace as string
-            self._consume_output(f'\nException: {ex}\n')
-            self._consume_output(traceback.format_exc())
-
-        # Final assertion of observed and expected output
-        if output_file is not None:
-            with open(output_file) as output:
-                group_stats = self._score_output(output.read())
-        else:
-            group_stats = self._score_output(self.observed_output)
+            exception = f"Exception: {ex}\n{traceback.format_exc()}"
+            group_stats = self._score_output(exception)
 
         return group_stats
 
 
 def record_script(dialog_file, script_name, *script_args):
     # Intercept input, print, and sys.argv
     sys.argv = [script_name, *(str(a) for a in script_args)]
```

### Comparing `byu_pytest_utils-0.6.1/byu_pytest_utils/edit_dist.py` & `byu_pytest_utils-0.6.3/byu_pytest_utils/edit_dist.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.6.1/byu_pytest_utils/pytest_plugin.py` & `byu_pytest_utils-0.6.3/byu_pytest_utils/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.6.1/byu_pytest_utils/utils.py` & `byu_pytest_utils-0.6.3/byu_pytest_utils/utils.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.6.1/pyproject.toml` & `byu_pytest_utils-0.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "byu_pytest_utils"
-version = "0.6.1"
+version = "0.6.3"
 description = "A few utilities for pytest to help with integration into gradescope"
 authors = ["Gordon Bean <gbean@cs.byu.edu>", "Daniel Zappala <daniel.zappala@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Framework :: Pytest"
 ]
```

### Comparing `byu_pytest_utils-0.6.1/PKG-INFO` & `byu_pytest_utils-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byu-pytest-utils
-Version: 0.6.1
+Version: 0.6.3
 Summary: A few utilities for pytest to help with integration into gradescope
 License: MIT
 Author: Gordon Bean
 Author-email: gbean@cs.byu.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: MIT License
```

