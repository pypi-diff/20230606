# Comparing `tmp/refaci-0.2.0.tar.gz` & `tmp/refaci-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refaci-0.2.0.tar", max compression
+gzip compressed data, was "refaci-0.3.0.tar", max compression
```

## Comparing `refaci-0.2.0.tar` & `refaci-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2023-05-27 11:26:39.245469 refaci-0.2.0/LICENSE
--rw-r--r--   0        0        0      961 2023-05-28 23:14:34.768094 refaci-0.2.0/README.md
--rw-r--r--   0        0        0     3854 2023-05-29 09:54:59.616531 refaci-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       78 2023-05-28 23:14:34.914760 refaci-0.2.0/refaci/__init__.py
--rw-r--r--   0        0        0      434 2023-05-28 22:39:51.012862 refaci-0.2.0/refaci/__main__.py
--rw-r--r--   0        0        0     2741 2023-05-29 09:30:21.732347 refaci-0.2.0/refaci/gather.py
--rw-r--r--   0        0        0     3751 2023-05-28 23:12:37.072073 refaci-0.2.0/refaci/refactor.py
--rw-r--r--   0        0        0     1726 1970-01-01 00:00:00.000000 refaci-0.2.0/setup.py
--rw-r--r--   0        0        0     1534 1970-01-01 00:00:00.000000 refaci-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-27 11:26:39.245469 refaci-0.3.0/LICENSE
+-rw-r--r--   0        0        0      961 2023-05-28 23:14:34.768094 refaci-0.3.0/README.md
+-rw-r--r--   0        0        0     3854 2023-06-06 04:57:44.176360 refaci-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-05-28 23:14:34.914760 refaci-0.3.0/refaci/__init__.py
+-rw-r--r--   0        0        0      434 2023-05-28 22:39:51.012862 refaci-0.3.0/refaci/__main__.py
+-rw-r--r--   0        0        0     2741 2023-05-29 10:03:43.766988 refaci-0.3.0/refaci/gather.py
+-rw-r--r--   0        0        0     5105 2023-06-06 04:57:21.123153 refaci-0.3.0/refaci/refactor.py
+-rw-r--r--   0        0        0     1726 1970-01-01 00:00:00.000000 refaci-0.3.0/setup.py
+-rw-r--r--   0        0        0     1534 1970-01-01 00:00:00.000000 refaci-0.3.0/PKG-INFO
```

### Comparing `refaci-0.2.0/LICENSE` & `refaci-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `refaci-0.2.0/README.md` & `refaci-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `refaci-0.2.0/pyproject.toml` & `refaci-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "refaci"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = ["Stanislav Zmiev <szmiev2000@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ovsyanka83/refaci"
 
 [tool.poetry.dependencies]
```

### Comparing `refaci-0.2.0/refaci/gather.py` & `refaci-0.3.0/refaci/gather.py`

 * *Files identical despite different names*

### Comparing `refaci-0.2.0/refaci/refactor.py` & `refaci-0.3.0/refaci/refactor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,77 @@
 import ast
 import itertools
 import json
+import os
 import re
 from collections import defaultdict
 from collections.abc import Sequence
 from pathlib import Path
-from typing import Collection
+from typing import Callable, Collection, TypeVar, cast
+
+T = TypeVar("T", Path, str)
 
 
 def refactor(
-    dir_or_path: Path,
+    root_dir: Path,
     imports_to_change: dict[str, tuple[str, str]] = {},
     missing_imports_to_add: dict[str, str] = {},
     replacements: dict["PathRegex | ContentsRegex", Sequence[tuple[str, str]]] = {},
 ):
-    if dir_or_path.is_file():
-        files = [dir_or_path]
-    else:
-        files = dir_or_path.glob("**/*.py")
-
-    path_replacements = {
+    dir_path_replacements = {
+        regex: replacements for regex, replacements in replacements.items() if isinstance(regex, DirRegex)
+    }
+    file_path_replacements = {
         regex: replacements for regex, replacements in replacements.items() if isinstance(regex, PathRegex)
     }
     contents_re = {
         regex: replacements for regex, replacements in replacements.items() if isinstance(regex, ContentsRegex)
     }
 
-    for file in files:
-        print(str(file))
-        try:
-            contents = file.read_text()
-            file_replacements = []
-            file_replacements.extend(
-                [replacements for regex, replacements in path_replacements.items() if regex.pattern.search(str(file))],
-            )
-            file_replacements.extend(
-                [replacements for regex, replacements in contents_re.items() if regex.pattern.search(contents)],
-            )
-            file_replacements = itertools.chain.from_iterable(file_replacements)
-            contents = refactor_imports(contents, imports_to_change, missing_imports_to_add)
-            contents = globally_replace(contents, file_replacements)
-            file.write_text(contents)
-        except Exception as e:
-            print(repr(e))
+    for root, dirs, files in os.walk(root_dir):
+        root = Path(root)
+        dirs = [root / dir for dir in dirs]
+        files = [root / file for file in files]
+
+        for file in files:
+            print(str(file))
+            try:
+                contents = file.read_text()
+                file_replacements = []
+                file_replacements.extend(
+                    [
+                        replacements
+                        for regex, replacements in file_path_replacements.items()
+                        if regex.pattern.search(str(file))
+                    ],
+                )
+                file_replacements.extend(
+                    [replacements for regex, replacements in contents_re.items() if regex.pattern.search(contents)],
+                )
+                file_replacements = tuple(itertools.chain.from_iterable(file_replacements))
+                contents = refactor_imports(contents, imports_to_change, missing_imports_to_add)
+                contents = globally_replace(contents, file_replacements)
+                file.write_text(contents)
+            except Exception as e:
+                print(repr(e))
+        for dir in dirs:
+            for regex, replacement in dir_path_replacements.items():
+                if regex.pattern.search(str(dir.resolve().absolute())):
+                    assert callable(replacement), "DirRegex must be a callable that accepts a dir path"
+                    run_replacement(dir, replacement)
 
 
 def refactor_imports(
     contents: str,
     imports_to_change: dict[str, tuple[str, str]] = {},
     missing_imports_to_add: dict[str, str] = {},
 ):
     modules = to_modules(imports_to_change)
     tree = ast.parse(contents)
-    lines: list[str | list[str]] = contents.splitlines()
+    lines = cast(list[str | list[str]], contents.splitlines())
 
     for node in ast.walk(tree):
         # TODO
         if isinstance(node, ast.Import):
             for alias in node.names:
                 ...
         elif isinstance(node, ast.ImportFrom) and node.module in modules:
@@ -79,20 +94,34 @@
         if isinstance(line, list):
             new_lines.extend(line)
         else:
             new_lines.append(line)
     return "\n".join(new_lines)
 
 
-def globally_replace(contents: str, replacements: Collection[tuple[str, str]] = ()):
-    for old, new in replacements:
-        contents = contents.replace(old, new)
+def globally_replace(contents: str, replacements: Collection[tuple[str, str] | Callable[[Path | str], str]] = ()):
+    for replacement in replacements:
+        contents = run_replacement(contents, replacement)
     return contents
 
 
+def run_replacement(contents_or_dir_path: T, replacement: tuple[str, str] | Callable[[T], str]) -> str:
+    if isinstance(contents_or_dir_path, Path):
+        assert callable(replacement)
+
+        return replacement(contents_or_dir_path)
+    elif isinstance(contents_or_dir_path, str):
+        if callable(replacement):
+            return replacement(contents_or_dir_path)
+        else:
+            return contents_or_dir_path.replace(*replacement)
+    else:
+        raise TypeError(f"Expected Path or str, got {type(contents_or_dir_path)}")
+
+
 def to_modules(imports_to_change: dict[str, tuple[str, str]]) -> dict[str, dict[str, str]]:
     modules = defaultdict(dict)
     for alias, (old, new) in imports_to_change.items():
         modules[old][alias] = new
     return modules
```

### Comparing `refaci-0.2.0/setup.py` & `refaci-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['typer[all]', 'typing-extensions']
 
 entry_points = \
 {'console_scripts': ['refaci = refaci.__main__:app']}
 
 setup_kwargs = {
     'name': 'refaci',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': '',
     'long_description': '# refaci\n\nA toolbox for changing imports in enormous codebases after a large refactoring.\n\n---\n\n<p align="center">\n<a href="https://github.com/ovsyanka83/refaci/actions?query=workflow%3ATests+event%3Apush+branch%3Amain" target="_blank">\n    <img src="https://github.com/Ovsyanka83/refaci/actions/workflows/test.yaml/badge.svg?branch=main&event=push" alt="Test">\n</a>\n<a href="https://codecov.io/gh/ovsyanka83/refaci" target="_blank">\n    <img src="https://img.shields.io/codecov/c/github/ovsyanka83/refaci?color=%2334D058" alt="Coverage">\n</a>\n<a href="https://pypi.org/project/refaci/" target="_blank">\n    <img alt="PyPI" src="https://img.shields.io/pypi/v/refaci?color=%2334D058&label=pypi%20package" alt="Package version">\n</a>\n<a href="https://pypi.org/project/refaci/" target="_blank">\n    <img src="https://img.shields.io/pypi/pyversions/refaci?color=%2334D058" alt="Supported Python versions">\n</a>\n</p>\n\n## Installation\n\n```bash\npip install refaci\n```\n',
     'author': 'Stanislav Zmiev',
     'author_email': 'szmiev2000@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ovsyanka83/refaci',
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['refaci']
 package_data = \ {'': ['*']} install_requires = \ ['typer[all]', 'typing-
 extensions'] entry_points = \ {'console_scripts': ['refaci = refaci.__main__:
-app']} setup_kwargs = { 'name': 'refaci', 'version': '0.2.0', 'description':
+app']} setup_kwargs = { 'name': 'refaci', 'version': '0.3.0', 'description':
 '', 'long_description': '# refaci\n\nA toolbox for changing imports in enormous
 codebases after a large refactoring.\n\n---\n\n
 \n\n_[Test]\n\n\n_[Coverage]\n\n\n_[PyPI]\n\n\n_[Supported_Python_versions]\n\n
 \n\n## Installation\n\n```bash\npip install refaci\n```\n', 'author':
 'Stanislav Zmiev', 'author_email': 'szmiev2000@gmail.com', 'maintainer':
 'None', 'maintainer_email': 'None', 'url': 'https://github.com/ovsyanka83/
 refaci', 'packages': packages, 'package_data': package_data,
```

### Comparing `refaci-0.2.0/PKG-INFO` & `refaci-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refaci
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Home-page: https://github.com/ovsyanka83/refaci
 License: MIT
 Author: Stanislav Zmiev
 Author-email: szmiev2000@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: refaci Version: 0.2.0 Summary: Home-page: https://
+Metadata-Version: 2.1 Name: refaci Version: 0.3.0 Summary: Home-page: https://
 github.com/ovsyanka83/refaci License: MIT Author: Stanislav Zmiev Author-email:
 szmiev2000@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: typer[all] Requires-Dist: typing-
 extensions Project-URL: Repository, https://github.com/ovsyanka83/refaci
 Description-Content-Type: text/markdown # refaci A toolbox for changing imports
```

