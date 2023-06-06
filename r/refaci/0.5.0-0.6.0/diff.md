# Comparing `tmp/refaci-0.5.0.tar.gz` & `tmp/refaci-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refaci-0.5.0.tar", max compression
+gzip compressed data, was "refaci-0.6.0.tar", max compression
```

## Comparing `refaci-0.5.0.tar` & `refaci-0.6.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2023-05-27 11:26:39.245469 refaci-0.5.0/LICENSE
--rw-r--r--   0        0        0      961 2023-05-28 23:14:34.768094 refaci-0.5.0/README.md
--rw-r--r--   0        0        0     3854 2023-06-06 05:54:10.611111 refaci-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       78 2023-05-28 23:14:34.914760 refaci-0.5.0/refaci/__init__.py
--rw-r--r--   0        0        0      434 2023-05-28 22:39:51.012862 refaci-0.5.0/refaci/__main__.py
--rw-r--r--   0        0        0     2850 2023-06-06 05:52:02.528480 refaci-0.5.0/refaci/gather.py
--rw-r--r--   0        0        0     4958 2023-06-06 05:49:09.949427 refaci-0.5.0/refaci/refactor.py
--rw-r--r--   0        0        0     1726 1970-01-01 00:00:00.000000 refaci-0.5.0/setup.py
--rw-r--r--   0        0        0     1534 1970-01-01 00:00:00.000000 refaci-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-27 11:26:39.245469 refaci-0.6.0/LICENSE
+-rw-r--r--   0        0        0      961 2023-05-28 23:14:34.768094 refaci-0.6.0/README.md
+-rw-r--r--   0        0        0     3854 2023-06-06 05:55:11.364110 refaci-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-05-28 23:14:34.914760 refaci-0.6.0/refaci/__init__.py
+-rw-r--r--   0        0        0      434 2023-05-28 22:39:51.012862 refaci-0.6.0/refaci/__main__.py
+-rw-r--r--   0        0        0     2901 2023-06-06 05:54:59.307510 refaci-0.6.0/refaci/gather.py
+-rw-r--r--   0        0        0     4958 2023-06-06 05:49:09.949427 refaci-0.6.0/refaci/refactor.py
+-rw-r--r--   0        0        0     1726 1970-01-01 00:00:00.000000 refaci-0.6.0/setup.py
+-rw-r--r--   0        0        0     1534 1970-01-01 00:00:00.000000 refaci-0.6.0/PKG-INFO
```

### Comparing `refaci-0.5.0/LICENSE` & `refaci-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `refaci-0.5.0/README.md` & `refaci-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `refaci-0.5.0/pyproject.toml` & `refaci-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "refaci"
-version = "0.5.0"
+version = "0.6.0"
 description = ""
 authors = ["Stanislav Zmiev <szmiev2000@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ovsyanka83/refaci"
 
 [tool.poetry.dependencies]
```

### Comparing `refaci-0.5.0/refaci/gather.py` & `refaci-0.6.0/refaci/gather.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import ast
 import json
 import os
+from collections import defaultdict
 from collections.abc import Collection
 from dataclasses import dataclass
 from pathlib import Path
 
 {
     "old.path": {
         "Alias": {"path": "new.path", "alias": "NewAlias"},
@@ -60,15 +61,15 @@
     return result
 
 
 def main(original_packages: Collection[Path], new_packages: Collection[Path]) -> None:
     main_package_result = {p.name: p.path for path in original_packages for p in gather_names(path)}
     subpackage_results = {p.name: p.path for path in new_packages for p in gather_names(path)}
 
-    moved_symbols = {}
+    moved_symbols = defaultdict(dict)
     removed_symbols = {}
     new_symbols = {}
 
     for p, ppath in main_package_result.items():
         if p in subpackage_results:
             moved_symbols[ppath.rsplit(".", 1)[0]][p] = {"path": subpackage_results[p].rsplit(".", 1)[0], "alias": p}
         else:
```

### Comparing `refaci-0.5.0/refaci/refactor.py` & `refaci-0.6.0/refaci/refactor.py`

 * *Files identical despite different names*

### Comparing `refaci-0.5.0/setup.py` & `refaci-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['typer[all]', 'typing-extensions']
 
 entry_points = \
 {'console_scripts': ['refaci = refaci.__main__:app']}
 
 setup_kwargs = {
     'name': 'refaci',
-    'version': '0.5.0',
+    'version': '0.6.0',
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
-app']} setup_kwargs = { 'name': 'refaci', 'version': '0.5.0', 'description':
+app']} setup_kwargs = { 'name': 'refaci', 'version': '0.6.0', 'description':
 '', 'long_description': '# refaci\n\nA toolbox for changing imports in enormous
 codebases after a large refactoring.\n\n---\n\n
 \n\n_[Test]\n\n\n_[Coverage]\n\n\n_[PyPI]\n\n\n_[Supported_Python_versions]\n\n
 \n\n## Installation\n\n```bash\npip install refaci\n```\n', 'author':
 'Stanislav Zmiev', 'author_email': 'szmiev2000@gmail.com', 'maintainer':
 'None', 'maintainer_email': 'None', 'url': 'https://github.com/ovsyanka83/
 refaci', 'packages': packages, 'package_data': package_data,
```

### Comparing `refaci-0.5.0/PKG-INFO` & `refaci-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refaci
-Version: 0.5.0
+Version: 0.6.0
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
-Metadata-Version: 2.1 Name: refaci Version: 0.5.0 Summary: Home-page: https://
+Metadata-Version: 2.1 Name: refaci Version: 0.6.0 Summary: Home-page: https://
 github.com/ovsyanka83/refaci License: MIT Author: Stanislav Zmiev Author-email:
 szmiev2000@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: typer[all] Requires-Dist: typing-
 extensions Project-URL: Repository, https://github.com/ovsyanka83/refaci
 Description-Content-Type: text/markdown # refaci A toolbox for changing imports
```

