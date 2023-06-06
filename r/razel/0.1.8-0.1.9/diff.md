# Comparing `tmp/razel-0.1.8.tar.gz` & `tmp/razel-0.1.9.tar.gz`

## Comparing `razel-0.1.8.tar` & `razel-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 razel-0.1.8/version.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 razel-0.1.8/src/razel/__init__.py
--rw-r--r--   0        0        0    15328 2020-02-02 00:00:00.000000 razel-0.1.8/src/razel/razel.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 razel-0.1.8/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 razel-0.1.8/LICENSE.md
--rw-r--r--   0        0        0     6351 2020-02-02 00:00:00.000000 razel-0.1.8/README.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 razel-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 razel-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 razel-0.1.9/version.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 razel-0.1.9/src/razel/__init__.py
+-rw-r--r--   0        0        0    15766 2020-02-02 00:00:00.000000 razel-0.1.9/src/razel/razel.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 razel-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 razel-0.1.9/LICENSE.md
+-rw-r--r--   0        0        0     6351 2020-02-02 00:00:00.000000 razel-0.1.9/README.md
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 razel-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 razel-0.1.9/PKG-INFO
```

### Comparing `razel-0.1.8/src/razel/razel.py` & `razel-0.1.9/src/razel/razel.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import sys
 from enum import Enum
 from typing import ClassVar, Optional, Any, Tuple, TypeVar
 from collections.abc import Mapping, Sequence
 
 
 class Razel:
-    version: ClassVar[str] = "0.1.8"
+    version: ClassVar[str] = "0.1.9"
     _instance: ClassVar[Optional[Razel]] = None
 
     class Tag(str, Enum):
         QUIET = 'razel:quiet'
         VERBOSE = 'razel:verbose'
 
     def __init__(self, workspace_dir: str) -> None:
@@ -54,27 +54,27 @@
         name = Razel._sanitize_name(name)
         command = Task(name, task, _map_args_to_output_files(args))
         return self._add(command)
 
     def ensure_equal(self, arg1: File | Command, arg2: File | Command) -> None:
         """Add a task to compare two files. In case of two commands, all output files will be compared."""
         if isinstance(arg1, Command) and isinstance(arg2, Command):
-            assert len(arg1.outputs) == len(arg2.outputs)
+            assert len(arg1.outputs) == len(arg2.outputs), "Commands to compare have different number of output files!"
             for i in range(len(arg1.outputs)):
                 self.ensure_equal(arg1.outputs[i], arg2.outputs[i])
         else:
             file1 = _map_arg_to_output_file(arg1)
             file2 = _map_arg_to_output_file(arg2)
             name = f"{file1.basename}##shouldEqual##{file2.basename}"
             self._add(Task(name, "ensure-equal", [file1, file2]))
 
     def ensure_not_equal(self, arg1: File | Command, arg2: File | Command) -> None:
         """Add a task to compare two files. In case of two commands, all output files will be compared."""
         if isinstance(arg1, Command) and isinstance(arg2, Command):
-            assert len(arg1.outputs) == len(arg2.outputs)
+            assert len(arg1.outputs) == len(arg2.outputs), "Commands to compare have different number of output files!"
             for i in range(len(arg1.outputs)):
                 self.ensure_equal(arg1.outputs[i], arg2.outputs[i])
         else:
             file1 = _map_arg_to_output_file(arg1)
             file2 = _map_arg_to_output_file(arg2)
             name = f"{file1.basename}##shouldNotEqual##{file2.basename}"
             self._add(Task(name, "ensure-not-equal", [file1, file2]))
@@ -264,21 +264,29 @@
         """Add an output file which is not part of the command line."""
         file = arg if isinstance(arg, File) else Razel.instance().add_output_file(arg)
         file._created_by = self
         self._outputs.append(file)
         return self
 
     def write_stdout_to_file(self, path: Optional[str] = None) -> CustomCommand:
-        self._stdout = Razel.instance().add_output_file(path if path else self._name)
+        new_file = Razel.instance().add_output_file(path if path else self._name + ".stdout.txt")
+        if self._stdout:
+            assert new_file.file_name == self._stdout.file_name
+            return self
+        self._stdout = new_file
         self._stdout._created_by = self
         self._outputs.append(self._stdout)
         return self
 
     def write_stderr_to_file(self, path: Optional[str] = None) -> CustomCommand:
-        self._stderr = Razel.instance().add_output_file(path if path else self._name)
+        new_file = Razel.instance().add_output_file(path if path else self._name + ".stderr.txt")
+        if self._stderr:
+            assert new_file.file_name == self._stderr.file_name
+            return self
+        self._stderr = new_file
         self._stderr._created_by = self
         self._outputs.append(self._stderr)
         return self
 
     def json(self) -> Mapping[str, Any]:
         j: Any = {
             "name": self.name,
```

### Comparing `razel-0.1.8/LICENSE.md` & `razel-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `razel-0.1.8/README.md` & `razel-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `razel-0.1.8/pyproject.toml` & `razel-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `razel-0.1.8/PKG-INFO` & `razel-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: razel
-Version: 0.1.8
+Version: 0.1.9
 Summary: a command executor with caching for data processing pipelines
 Project-URL: Homepage, https://github.com/reu-dev/razel
 Project-URL: Bug Tracker, https://github.com/reu-dev/razel/issues
 Author-email: Stefan Reuschl <stefan@reu-dev.de>, Kacper Sagnowski <ksagnowski@gmail.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

