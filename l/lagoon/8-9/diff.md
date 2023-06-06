# Comparing `tmp/lagoon-8.tar.gz` & `tmp/lagoon-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lagoon-8.tar", last modified: Tue Mar 10 23:59:18 2020, max compression
+gzip compressed data, was "dist/lagoon-9.tar", last modified: Tue Mar 17 20:03:58 2020, max compression
```

## Comparing `lagoon-8.tar` & `lagoon-9.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-03-10 23:59:18.000000 lagoon-8/
-drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-03-10 23:59:18.000000 lagoon-8/lagoon.egg-info/
--rw-rw-r--   0 arc       (1000) arc       (1000)        1 2020-03-10 23:59:18.000000 lagoon-8/lagoon.egg-info/dependency_links.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)       20 2020-03-10 23:59:18.000000 lagoon-8/lagoon.egg-info/entry_points.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)      267 2020-03-10 23:59:18.000000 lagoon-8/lagoon.egg-info/SOURCES.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)       14 2020-03-10 23:59:18.000000 lagoon-8/lagoon.egg-info/top_level.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)      403 2020-03-10 23:59:18.000000 lagoon-8/lagoon.egg-info/PKG-INFO
--rw-rw-r--   0 arc       (1000) arc       (1000)      691 2020-03-10 23:59:17.000000 lagoon-8/setup.py
--rw-rw-r--   0 arc       (1000) arc       (1000)       67 2020-03-10 23:59:18.000000 lagoon-8/setup.cfg
-drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-03-10 23:59:18.000000 lagoon-8/lagoon/
--rw-rw-r--   0 arc       (1000) arc       (1000)     4624 2020-03-10 20:13:56.000000 lagoon-8/lagoon/program.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      691 2020-02-29 19:51:18.000000 lagoon-8/lagoon/binary.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     7053 2020-03-10 20:02:47.000000 lagoon-8/lagoon/test_lagoon.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      744 2020-03-07 21:54:54.000000 lagoon-8/lagoon/__init__.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     2451 2020-03-07 12:25:47.000000 lagoon-8/screen.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      129 2019-11-03 21:55:02.000000 lagoon-8/README.md
--rw-rw-r--   0 arc       (1000) arc       (1000)      403 2020-03-10 23:59:18.000000 lagoon-8/PKG-INFO
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-03-17 20:03:58.000000 lagoon-9/
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-03-17 20:03:58.000000 lagoon-9/lagoon.egg-info/
+-rw-rw-r--   0 arc       (1000) arc       (1000)        1 2020-03-17 20:03:58.000000 lagoon-9/lagoon.egg-info/dependency_links.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)        7 2020-03-17 20:03:58.000000 lagoon-9/lagoon.egg-info/requires.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)       20 2020-03-17 20:03:58.000000 lagoon-9/lagoon.egg-info/entry_points.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)      331 2020-03-17 20:03:58.000000 lagoon-9/lagoon.egg-info/SOURCES.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)       14 2020-03-17 20:03:58.000000 lagoon-9/lagoon.egg-info/top_level.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)      403 2020-03-17 20:03:58.000000 lagoon-9/lagoon.egg-info/PKG-INFO
+-rw-rw-r--   0 arc       (1000) arc       (1000)      699 2020-03-17 20:03:57.000000 lagoon-9/setup.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)       67 2020-03-17 20:03:58.000000 lagoon-9/setup.cfg
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-03-17 20:03:58.000000 lagoon-9/lagoon/
+-rw-rw-r--   0 arc       (1000) arc       (1000)      846 2020-03-17 20:00:07.000000 lagoon-9/lagoon/util.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     4559 2020-03-17 20:00:07.000000 lagoon-9/lagoon/program.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2314 2020-03-17 20:00:07.000000 lagoon-9/lagoon/test_util.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      697 2020-03-17 20:00:07.000000 lagoon-9/lagoon/binary.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     7211 2020-03-17 20:00:07.000000 lagoon-9/lagoon/test_lagoon.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      750 2020-03-17 20:00:07.000000 lagoon-9/lagoon/__init__.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2457 2020-03-17 20:00:07.000000 lagoon-9/screen.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      129 2019-11-03 21:55:02.000000 lagoon-9/README.md
+-rw-rw-r--   0 arc       (1000) arc       (1000)      403 2020-03-17 20:03:58.000000 lagoon-9/PKG-INFO
```

### Comparing `lagoon-8/setup.py` & `lagoon-9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 def long_description():
     with open('README.md') as f:
         return f.read()
 
 setuptools.setup(
         name = 'lagoon',
-        version = '8',
+        version = '9',
         description = 'Experimental layer on top of subprocess',
         long_description = long_description(),
         long_description_content_type = 'text/markdown',
         url = 'https://github.com/combatopera/lagoon',
         author = 'Andrzej Cichocki',
         packages = setuptools.find_packages(),
         py_modules = ['screen'],
-        install_requires = [],
+        install_requires = ['diapyr'],
         package_data = {'': ['*.pxd', '*.pyx', '*.pyxbld', '*.arid', '*.aridt']},
         scripts = [],
         entry_points = {'console_scripts': []})
```

### Comparing `lagoon-8/lagoon/program.py` & `lagoon-9/lagoon/program.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018, 2019 Andrzej Cichocki
+# Copyright 2018, 2019, 2020 Andrzej Cichocki
 
 # This file is part of lagoon.
 #
 # lagoon is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -12,14 +12,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with lagoon.  If not, see <http://www.gnu.org/licenses/>.
 
 from . import binary
+from .util import unmangle
 from contextlib import contextmanager
 from pathlib import Path
 import os, subprocess, sys
 
 class Program:
 
     @staticmethod
@@ -33,36 +34,35 @@
             if os.path.isdir(parent):
                 for name in os.listdir(parent):
                     if name not in programs:
                         programs[name] = os.path.join(parent, name)
         module = sys.modules[modulename]
         delattr(module, cls.__name__)
         for name, path in programs.items():
-            setattr(module, name, cls(path, True, None, (), (), {}))
-            setattr(binary, name, cls(path, None, None, (), (), {}))
+            setattr(module, name, cls(path, True, None, (), {}))
+            setattr(binary, name, cls(path, None, None, (), {}))
 
-    def __init__(self, path, textmode, cwd, subcommand, args, kwargs):
+    def __init__(self, path, textmode, cwd, args, kwargs):
         self.path = path
         self.textmode = textmode
         self.cwd = cwd
-        self.subcommand = subcommand
         self.args = args
         self.kwargs = kwargs
 
     def _resolve(self, path):
         return Path(path) if self.cwd is None else self.cwd / path
 
     def cd(self, cwd):
-        return type(self)(self.path, self.textmode, self._resolve(cwd), self.subcommand, self.args, self.kwargs)
+        return type(self)(self.path, self.textmode, self._resolve(cwd), self.args, self.kwargs)
 
     def __getattr__(self, name):
-        return type(self)(self.path, self.textmode, self.cwd, self.subcommand + (name,), self.args, self.kwargs)
+        return type(self)(self.path, self.textmode, self.cwd, self.args + (unmangle(name).replace('_', '-'),), self.kwargs)
 
     def partial(self, *args, **kwargs):
-        return type(self)(self.path, self.textmode, self.cwd, self.subcommand, self.args + args, {**self.kwargs, **kwargs})
+        return type(self)(self.path, self.textmode, self.cwd, self.args + args, {**self.kwargs, **kwargs})
 
     def _transform(self, args, kwargs, checkxform):
         # TODO: Merge env with current instead of replacing by default.
         args = self.args + args
         kwargs = {**self.kwargs, **kwargs}
         kwargs.setdefault('check', True)
         kwargs.setdefault('stdout', subprocess.PIPE)
@@ -91,15 +91,15 @@
             try:
                 next(xforms)
                 xform = lambda res: res
             except StopIteration:
                 pass
         except StopIteration:
             xform = lambda res: None
-        return [self.path, *self.subcommand, *transformargs()], kwargs, xform
+        return [self.path, *transformargs()], kwargs, xform
 
     def __call__(self, *args, **kwargs):
         cmd, kwargs, xform = self._transform(args, kwargs, lambda res: res.returncode)
         return xform(subprocess.run(cmd, **kwargs))
 
     @contextmanager
     def bg(self, *args, **kwargs):
```

### Comparing `lagoon-8/lagoon/binary.py` & `lagoon-9/lagoon/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018, 2019 Andrzej Cichocki
+# Copyright 2018, 2019, 2020 Andrzej Cichocki
 
 # This file is part of lagoon.
 #
 # lagoon is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,7 +11,10 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with lagoon.  If not, see <http://www.gnu.org/licenses/>.
 
+from .program import Program
+
+Program.scan(__name__)
```

### Comparing `lagoon-8/lagoon/test_lagoon.py` & `lagoon-9/lagoon/test_lagoon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018, 2019 Andrzej Cichocki
+# Copyright 2018, 2019, 2020 Andrzej Cichocki
 
 # This file is part of lagoon.
 #
 # lagoon is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -158,7 +158,12 @@
         self.assertEqual('0\n', cp.stdout)
         self.assertEqual(1, cp.returncode)
         self.assertEqual(0, test100('=', 100, stdout = subprocess.DEVNULL))
         with self.assertRaises(subprocess.CalledProcessError):
             test100('=', 101, check = True)
         with test100.bg('=', 100) as process:
             self.assertEqual('1\n', process.stdout.read())
+
+    def test_partial2(self):
+        from . import bash
+        git = bash._c.partial('git "$@"', 'git')
+        self.assertEqual('', git.rev_parse())
```

### Comparing `lagoon-8/lagoon/__init__.py` & `lagoon-9/lagoon/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018, 2019 Andrzej Cichocki
+# Copyright 2018, 2019, 2020 Andrzej Cichocki
 
 # This file is part of lagoon.
 #
 # lagoon is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,10 +11,14 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with lagoon.  If not, see <http://www.gnu.org/licenses/>.
 
-from .program import Program
+import re
 
-Program.scan(__name__)
+mangled = re.compile('_.*(__.*[^_]_?)')
+
+def unmangle(name):
+    m = mangled.fullmatch(name)
+    return name if m is None else m.group(1)
```

### Comparing `lagoon-8/screen.py` & `lagoon-9/screen.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018, 2019 Andrzej Cichocki
+# Copyright 2018, 2019, 2020 Andrzej Cichocki
 
 # This file is part of lagoon.
 #
 # lagoon is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

