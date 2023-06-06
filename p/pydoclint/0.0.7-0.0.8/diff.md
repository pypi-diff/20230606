# Comparing `tmp/pydoclint-0.0.7.tar.gz` & `tmp/pydoclint-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydoclint-0.0.7.tar", last modified: Thu Jun  1 10:42:17 2023, max compression
+gzip compressed data, was "pydoclint-0.0.8.tar", last modified: Tue Jun  6 08:37:39 2023, max compression
```

## Comparing `pydoclint-0.0.7.tar` & `pydoclint-0.0.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:42:17.178283 pydoclint-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-01 10:42:07.000000 pydoclint-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-06-01 10:42:17.178283 pydoclint-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-06-01 10:42:07.000000 pydoclint-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:42:17.178283 pydoclint-0.0.7/pydoclint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/flake8_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/parse_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:42:17.178283 pydoclint-0.0.7/pydoclint/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/utils/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/utils/arg.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/utils/astTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/utils/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/utils/internal_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/utils/method_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/utils/return_yield_raise.py
--rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/utils/unparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/utils/violation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/utils/walk.py
--rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pydoclint/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:42:17.178283 pydoclint-0.0.7/pydoclint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-06-01 10:42:17.000000 pydoclint-0.0.7/pydoclint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-01 10:42:17.000000 pydoclint-0.0.7/pydoclint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 10:42:17.000000 pydoclint-0.0.7/pydoclint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 10:42:17.000000 pydoclint-0.0.7/pydoclint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-01 10:42:17.000000 pydoclint-0.0.7/pydoclint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 10:42:17.000000 pydoclint-0.0.7/pydoclint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-01 10:42:07.000000 pydoclint-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-01 10:42:17.178283 pydoclint-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-01 10:42:07.000000 pydoclint-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:42:17.178283 pydoclint-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    25632 2023-06-01 10:42:07.000000 pydoclint-0.0.7/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-01 10:42:07.000000 pydoclint-0.0.7/tests/test_parse_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:37:39.372371 pydoclint-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-06 08:37:23.000000 pydoclint-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-06-06 08:37:39.376371 pydoclint-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12340 2023-06-06 08:37:23.000000 pydoclint-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:37:39.368371 pydoclint-0.0.8/pydoclint/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/flake8_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/parse_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:37:39.372371 pydoclint-0.0.8/pydoclint/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/utils/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/utils/arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/utils/astTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/utils/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/utils/internal_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/utils/method_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/utils/return_yield_raise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/utils/unparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/utils/violation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/utils/walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17710 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:37:39.372371 pydoclint-0.0.8/pydoclint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-06-06 08:37:39.000000 pydoclint-0.0.8/pydoclint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-06 08:37:39.000000 pydoclint-0.0.8/pydoclint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 08:37:39.000000 pydoclint-0.0.8/pydoclint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-06 08:37:39.000000 pydoclint-0.0.8/pydoclint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-06 08:37:39.000000 pydoclint-0.0.8/pydoclint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-06 08:37:39.000000 pydoclint-0.0.8/pydoclint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-06 08:37:39.376371 pydoclint-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-06 08:37:23.000000 pydoclint-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:37:39.372371 pydoclint-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    26966 2023-06-06 08:37:23.000000 pydoclint-0.0.8/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-06 08:37:23.000000 pydoclint-0.0.8/tests/test_parse_config.py
```

### Comparing `pydoclint-0.0.7/LICENSE` & `pydoclint-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.7/PKG-INFO` & `pydoclint-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoclint
-Version: 0.0.7
+Version: 0.0.8
 Summary: A linter to check arguments in Python docstrings
 Home-page: https://github.com/jsh9/pydoclint
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
@@ -67,46 +67,62 @@
 ```
 flake8 --select=DOC <FILE_OR_FOLDER>
 ```
 
 If you don't include `--select=DOC` in your command, _flake8_ will also run
 other built-in _flake8_ linters on your code.
 
-### 2.3. Native vs _flake8_
+### 2.3. As a pre-commit hook
+
+`pydoclint` is configured for [pre-commit](https://pre-commit.com/) and can be
+set up as a hook with the following `.pre-commit-config.yaml` configuration:
+
+```yaml
+- repo: https://github.com/jsh9/pydoclint
+  rev: <latest_tag>
+  hooks:
+    - id: pydoclint
+      args:
+        - "--config=pyproject.toml"
+```
+
+You will need to install `pre-commit` and run `pre-commit install`.
+
+### 2.4. Native vs _flake8_
 
 Should I use _pydoclint_ as a native command line tool or a _flake8_ plugin?
 Here's comparison:
 
 |                 | Pros                                     | Cons                                                          |
 | --------------- | ---------------------------------------- | ------------------------------------------------------------- |
 | Native tool     | Slightly faster                          | No inline or project-wide omission support right now [*]      |
 | _flake8_ plugin | Supports inline or project-wide omission | Slightly slower because other flake8 plugins are run together |
 
 \*) This feature may be added in the near future
 
-### 2.4. Configuration
+### 2.5. Configuration
 
 Here is how to configure _pydoclint_. For detailed explanations of all options,
 see [Section 4](#4-configuration-options) below.
 
-#### 2.4.1. Setting options inline
+#### 2.5.1. Setting options inline
 
 - Native:
 
   ```bash
   pydoclint --check-arg-order=False <FILE_OR_FOLDER_PATH>
   ```
 
 - Flake8:
 
   ```bash
   flake8 --check-arg-order=False <FILE_OR_FOLDER_PATH>
   ```
 
-#### 2.4.2. Setting options in a configuration file
+#### 2.5.2. Setting options in a configuration file
 
 - Native:
 
   - In a `.toml` file somewhere in your project folder, add a section like this
     (put in the config that you need):
 
     ```toml
@@ -135,21 +151,21 @@
 
 | Code     | Explanation                              |
 | -------- | ---------------------------------------- |
 | `DOC001` | Potential formatting errors in docstring |
 
 ### 3.1. `DOC1xx`: Violations about input arguments
 
-| Code     | Explanation                                                                                                                                          |
-| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `DOC101` | Docstring contains fewer arguments than in function signature                                                                                        |
-| `DOC102` | Docstring contains more arguments than in function signature                                                                                         |
+| Code     | Explanation                                                                                                                                         |
+| -------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `DOC101` | Docstring contains fewer arguments than in function signature                                                                                       |
+| `DOC102` | Docstring contains more arguments than in function signature                                                                                        |
 | `DOC103` | Docstring arguments are different from function arguments. (Or could be other formatting issues: https://github.com/jsh9/pydoclint#notes-on-doc103) |
-| `DOC104` | Arguments are the same in the docstring and the function signature, but are in a different order.                                                    |
-| `DOC105` | Argument names match, but type hints do not match                                                                                                    |
+| `DOC104` | Arguments are the same in the docstring and the function signature, but are in a different order.                                                   |
+| `DOC105` | Argument names match, but type hints do not match                                                                                                   |
 
 #### Notes on `DOC103`:
 
 Other potential causes to `DOC103` include:
 
 - Numpy docstring style requires this style: `arg1 : int` (a space between
   `arg1` and `:`) but people sometimes write `arg1: int`. This will trigger
```

### Comparing `pydoclint-0.0.7/README.md` & `pydoclint-0.0.8/pydoclint.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: pydoclint
+Version: 0.0.8
+Summary: A linter to check arguments in Python docstrings
+Home-page: https://github.com/jsh9/pydoclint
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # pydoclint
 
 A Python docstring linter to check whether a docstring's sections (arguments,
 returns, raises, ...) match the function signature or function implementation.
 
 It runs really fast. In fact, it is at least ~1,475 times faster than
 [darglint](https://github.com/terrencepreilly/darglint) (another linter of the
@@ -54,46 +67,62 @@
 ```
 flake8 --select=DOC <FILE_OR_FOLDER>
 ```
 
 If you don't include `--select=DOC` in your command, _flake8_ will also run
 other built-in _flake8_ linters on your code.
 
-### 2.3. Native vs _flake8_
+### 2.3. As a pre-commit hook
+
+`pydoclint` is configured for [pre-commit](https://pre-commit.com/) and can be
+set up as a hook with the following `.pre-commit-config.yaml` configuration:
+
+```yaml
+- repo: https://github.com/jsh9/pydoclint
+  rev: <latest_tag>
+  hooks:
+    - id: pydoclint
+      args:
+        - "--config=pyproject.toml"
+```
+
+You will need to install `pre-commit` and run `pre-commit install`.
+
+### 2.4. Native vs _flake8_
 
 Should I use _pydoclint_ as a native command line tool or a _flake8_ plugin?
 Here's comparison:
 
 |                 | Pros                                     | Cons                                                          |
 | --------------- | ---------------------------------------- | ------------------------------------------------------------- |
 | Native tool     | Slightly faster                          | No inline or project-wide omission support right now [*]      |
 | _flake8_ plugin | Supports inline or project-wide omission | Slightly slower because other flake8 plugins are run together |
 
 \*) This feature may be added in the near future
 
-### 2.4. Configuration
+### 2.5. Configuration
 
 Here is how to configure _pydoclint_. For detailed explanations of all options,
 see [Section 4](#4-configuration-options) below.
 
-#### 2.4.1. Setting options inline
+#### 2.5.1. Setting options inline
 
 - Native:
 
   ```bash
   pydoclint --check-arg-order=False <FILE_OR_FOLDER_PATH>
   ```
 
 - Flake8:
 
   ```bash
   flake8 --check-arg-order=False <FILE_OR_FOLDER_PATH>
   ```
 
-#### 2.4.2. Setting options in a configuration file
+#### 2.5.2. Setting options in a configuration file
 
 - Native:
 
   - In a `.toml` file somewhere in your project folder, add a section like this
     (put in the config that you need):
 
     ```toml
@@ -122,21 +151,21 @@
 
 | Code     | Explanation                              |
 | -------- | ---------------------------------------- |
 | `DOC001` | Potential formatting errors in docstring |
 
 ### 3.1. `DOC1xx`: Violations about input arguments
 
-| Code     | Explanation                                                                                                                                          |
-| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `DOC101` | Docstring contains fewer arguments than in function signature                                                                                        |
-| `DOC102` | Docstring contains more arguments than in function signature                                                                                         |
+| Code     | Explanation                                                                                                                                         |
+| -------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `DOC101` | Docstring contains fewer arguments than in function signature                                                                                       |
+| `DOC102` | Docstring contains more arguments than in function signature                                                                                        |
 | `DOC103` | Docstring arguments are different from function arguments. (Or could be other formatting issues: https://github.com/jsh9/pydoclint#notes-on-doc103) |
-| `DOC104` | Arguments are the same in the docstring and the function signature, but are in a different order.                                                    |
-| `DOC105` | Argument names match, but type hints do not match                                                                                                    |
+| `DOC104` | Arguments are the same in the docstring and the function signature, but are in a different order.                                                   |
+| `DOC105` | Argument names match, but type hints do not match                                                                                                   |
 
 #### Notes on `DOC103`:
 
 Other potential causes to `DOC103` include:
 
 - Numpy docstring style requires this style: `arg1 : int` (a space between
   `arg1` and `:`) but people sometimes write `arg1: int`. This will trigger
```

### Comparing `pydoclint-0.0.7/pydoclint/flake8_entry.py` & `pydoclint-0.0.8/pydoclint/flake8_entry.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.7/pydoclint/main.py` & `pydoclint-0.0.8/pydoclint/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 import ast
 import re
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple
 
 import click
 
+from pydoclint import __version__
 from pydoclint.parse_config import (
     injectDefaultOptionsFromUserSpecifiedTomlFilePath,
 )
 from pydoclint.utils.violation import Violation
 from pydoclint.visitor import Visitor
 
+# Due to a potential bug in Windows + pre-commit, non-ASCII
+# characters cannot be rendered correctly as stdout in the terminal.
+# Therefore, we set all CLI output as stderr.
+# (More details in https://github.com/jsh9/pydoclint/issues/20)
+echoAsError = True
+
 
 def validateStyleValue(
         context: click.Context,
         param: click.Parameter,
         value: Optional[str],
 ) -> Optional[str]:
     """Validate the value of the 'style' option"""
@@ -138,14 +145,15 @@
     callback=injectDefaultOptionsFromUserSpecifiedTomlFilePath,
     help=(
         'The full path of the .toml config file that contains the config'
         ' options; note that the command line options take precedence'
         ' over the .toml file'
     ),
 )
+@click.version_option(__version__)
 @click.pass_context
 def main(  # noqa: C901
         ctx: click.Context,
         quiet: bool,
         exclude: str,
         style: str,
         src: Optional[str],
@@ -160,21 +168,23 @@
 ) -> None:
     """Command-line entry point of pydoclint"""
     ctx.ensure_object(dict)
 
     if paths and src is not None:
         click.echo(
             main.get_usage(ctx)
-            + "\n\n'paths' and 'src' cannot be passed simultaneously."
+            + "\n\n'paths' and 'src' cannot be passed simultaneously.",
+            err=echoAsError,
         )
         ctx.exit(1)
 
     if not paths and src is None:
         click.echo(
-            main.get_usage(ctx) + "\n\nOne of 'paths' or 'src' is required."
+            main.get_usage(ctx) + "\n\nOne of 'paths' or 'src' is required.",
+            err=echoAsError,
         )
         ctx.exit(1)
 
     violationsInAllFiles: Dict[str, List[Violation]] = _checkPaths(
         quiet=quiet,
         exclude=exclude,
         style=style,
@@ -192,35 +202,44 @@
         counter = 0
         for filename, violationsInThisFile in violationsInAllFiles.items():
             counter += 1
             if len(violationsInThisFile) > 0:
                 if counter > 1:
                     print('')
 
-                click.echo(click.style(filename, fg='yellow', bold=True))
+                click.echo(
+                    click.style(filename, fg='yellow', bold=True),
+                    err=echoAsError,
+                )
                 for violation in violationsInThisFile:
                     violationCounter += 1
                     fourSpaces = '    '
-                    click.echo(fourSpaces, nl=False)
-                    click.echo(f'{violation.line}: ', nl=False)
+                    click.echo(fourSpaces, nl=False, err=echoAsError)
+                    click.echo(
+                        f'{violation.line}: ', nl=False, err=echoAsError
+                    )
                     click.echo(
                         click.style(
                             f'{violation.fullErrorCode}',
                             fg='red',
                             bold=True,
                         ),
                         nl=False,
+                        err=echoAsError,
                     )
-                    click.echo(f': {violation.msg}')
+                    click.echo(f': {violation.msg}', err=echoAsError)
 
     if violationCounter > 0:
         ctx.exit(1)
     else:
         if not quiet:
-            click.echo(click.style('🎉 No violations 🎉', fg='green', bold=True))
+            click.echo(
+                click.style('🎉 No violations 🎉', fg='green', bold=True),
+                err=echoAsError,
+            )
 
         ctx.exit(0)
 
 
 def _checkPaths(
         paths: Tuple[str, ...],
         style: str = 'numpy',
@@ -233,15 +252,17 @@
         quiet: bool = False,
         exclude: str = '',
 ) -> Dict[str, List[Violation]]:
     filenames: List[Path] = []
 
     if not quiet:
         skipMsg = f'Skipping files that match this pattern: {exclude}'
-        click.echo(click.style(skipMsg, fg='yellow', bold=True))
+        click.echo(
+            click.style(skipMsg, fg='yellow', bold=True), err=echoAsError
+        )
 
     excludePattern = re.compile(exclude)
 
     for path_ in paths:
         path = Path(path_)
         if path.is_file():
             filenames.append(path)
@@ -251,15 +272,17 @@
     allViolations: Dict[str, List[Violation]] = {}
 
     for filename in filenames:
         if excludePattern.search(filename.as_posix()):
             continue
 
         if not quiet:
-            click.echo(click.style(filename, fg='cyan', bold=True))
+            click.echo(
+                click.style(filename, fg='cyan', bold=True), err=echoAsError
+            )
 
         violationsInThisFile: List[Violation] = _checkFile(
             filename,
             style=style,
             checkTypeHint=checkTypeHint,
             checkArgOrder=checkArgOrder,
             skipCheckingShortDocstrings=skipCheckingShortDocstrings,
@@ -278,15 +301,15 @@
         checkTypeHint: bool = True,
         checkArgOrder: bool = True,
         skipCheckingShortDocstrings: bool = True,
         skipCheckingRaises: bool = False,
         allowInitDocstring: bool = False,
         requireReturnSectionWhenReturningNone: bool = False,
 ) -> List[Violation]:
-    with open(filename) as fp:
+    with open(filename, encoding='utf8') as fp:
         src: str = ''.join(fp.readlines())
 
     tree: ast.Module = ast.parse(src)
     visitor = Visitor(
         style=style,
         checkTypeHint=checkTypeHint,
         checkArgOrder=checkArgOrder,
```

### Comparing `pydoclint-0.0.7/pydoclint/parse_config.py` & `pydoclint-0.0.8/pydoclint/parse_config.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.7/pydoclint/utils/annotation.py` & `pydoclint-0.0.8/pydoclint/utils/annotation.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.7/pydoclint/utils/arg.py` & `pydoclint-0.0.8/pydoclint/utils/arg.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.7/pydoclint/utils/astTypes.py` & `pydoclint-0.0.8/pydoclint/utils/astTypes.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.7/pydoclint/utils/doc.py` & `pydoclint-0.0.8/pydoclint/utils/doc.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.7/pydoclint/utils/generic.py` & `pydoclint-0.0.8/pydoclint/utils/generic.py`

 * *Files 9% similar despite different names*

```diff
@@ -129,7 +129,16 @@
     return (
         isinstance(node.decorator_list, list)
         and len(node.decorator_list) > 0
         and isinstance(node.decorator_list[-1], ast.Name)
         and hasattr(node.decorator_list[-1], 'id')
         and node.decorator_list[-1].id == 'property'
     )
+
+
+def stringStartsWith(string: str, substrings: Tuple[str, ...]) -> bool:
+    """Check whether the string starts with any of the substrings"""
+    for substring in substrings:
+        if string.startswith(substring):
+            return True
+
+    return False
```

### Comparing `pydoclint-0.0.7/pydoclint/utils/return_yield_raise.py` & `pydoclint-0.0.8/pydoclint/utils/return_yield_raise.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import ast
 from typing import Tuple, Type, Union
 
 from pydoclint.utils import walk
 from pydoclint.utils.annotation import unparseAnnotation
 from pydoclint.utils.astTypes import BlockType, FuncOrAsyncFuncDef
-from pydoclint.utils.generic import getFunctionId
+from pydoclint.utils.generic import getFunctionId, stringStartsWith
 
 ReturnType = Type[ast.Return]
 ExprType = Type[ast.Expr]
 YieldAndYieldFromTypes = Tuple[Type[ast.Yield], Type[ast.YieldFrom]]
 FuncOrAsyncFuncTypes = Tuple[Type[ast.FunctionDef], Type[ast.AsyncFunctionDef]]
 
 
@@ -24,15 +24,27 @@
 
 def hasGeneratorAsReturnAnnotation(node: FuncOrAsyncFuncDef) -> bool:
     """Check whether the function node has a 'Generator' return annotation"""
     if node.returns is None:
         return False
 
     returnAnnotation: str = unparseAnnotation(node.returns)
-    return returnAnnotation.startswith('Generator')
+    return stringStartsWith(returnAnnotation, ('Generator', 'AsyncGenerator'))
+
+
+def hasIteratorOrIterableAsReturnAnnotation(node: FuncOrAsyncFuncDef) -> bool:
+    """Check whether `node` has a 'Iterator' or 'Iterable' return annotation"""
+    if node.returns is None:
+        return False
+
+    returnAnnotation: str = unparseAnnotation(node.returns)
+    return stringStartsWith(
+        returnAnnotation,
+        ('Iterator', 'Iterable', 'AsyncIterator', 'AsyncIterable'),
+    )
 
 
 def hasYieldStatements(node: FuncOrAsyncFuncDef) -> bool:
     """Check whether the function node has any yield statements"""
     thisId = getFunctionId(node)
     for child, parent in walk.walk(node):
         if isinstance(child, ast.Expr) and isinstance(
```

### Comparing `pydoclint-0.0.7/pydoclint/utils/unparser.py` & `pydoclint-0.0.8/pydoclint/utils/unparser.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.7/pydoclint/utils/violation.py` & `pydoclint-0.0.8/pydoclint/utils/violation.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 VIOLATION_CODES = types.MappingProxyType({
     1: 'Potential formatting errors in docstring. Error message:',
 
     101: 'Docstring contains fewer arguments than in function signature.',
     102: 'Docstring contains more arguments than in function signature.',
     103: (  # noqa: PAR001
         'Docstring arguments are different from function arguments.'
-        ' (Or could be other formatting issues: https://github.com/jsh9/pydoclint#notes-on-doc103).'
+        ' (Or could be other formatting issues: https://github.com/jsh9/pydoclint#notes-on-doc103 ).'
     ),
     104: 'Arguments are the same in the docstring and the function signature, but are in a different order.',
     105: 'Argument names match, but type hints do not match',
 
     201: 'does not have a return section in docstring',
     202: 'has a return section in docstring, but there are no return statements or annotations',
 
@@ -68,8 +68,9 @@
             return self.__str__()
 
         return f'{self.line}: {self.__str__()}'
 
     def getInfoForFlake8(self) -> Tuple[int, int, str]:
         """Get the violation info for flake8"""
         colOffset: int = 0  # we don't need column offset to locate the issue
-        return self.line, colOffset, self.__str__()
+        msg = f'{self.fullErrorCode} {self.msg}'  # no colon b/c that would cause 'yesqa' issues
+        return self.line, colOffset, msg
```

### Comparing `pydoclint-0.0.7/pydoclint/utils/walk.py` & `pydoclint-0.0.8/pydoclint/utils/walk.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.7/pydoclint/visitor.py` & `pydoclint-0.0.8/pydoclint/visitor.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     getDocstring,
     isPropertyMethod,
 )
 from pydoclint.utils.internal_error import InternalError
 from pydoclint.utils.method_type import MethodType
 from pydoclint.utils.return_yield_raise import (
     hasGeneratorAsReturnAnnotation,
+    hasIteratorOrIterableAsReturnAnnotation,
     hasRaiseStatements,
     hasReturnAnnotation,
     hasReturnStatements,
     hasYieldStatements,
     isReturnAnnotationNone,
 )
 from pydoclint.utils.violation import Violation
@@ -392,20 +393,28 @@
 
         v201 = Violation(code=201, line=lineNum, msgPrefix=msgPrefix)
         v202 = Violation(code=202, line=lineNum, msgPrefix=msgPrefix)
 
         hasReturnStmt: bool = hasReturnStatements(node)
         hasReturnAnno: bool = hasReturnAnnotation(node)
         hasGenAsRetAnno: bool = hasGeneratorAsReturnAnnotation(node)
+        onlyHasYieldStmt: bool = hasYieldStatements(node) and not hasReturnStmt
+        hasIterAsRetAnno: bool = hasIteratorOrIterableAsReturnAnnotation(node)
 
         docstringHasReturnSection: bool = doc.hasReturnsSection
 
         violations: List[Violation] = []
         if not docstringHasReturnSection and not isPropertyMethod(node):
-            if hasReturnStmt or (hasReturnAnno and not hasGenAsRetAnno):
+            if (
+                # fmt: off
+                not (onlyHasYieldStmt and hasIterAsRetAnno)
+                and (hasReturnStmt or (hasReturnAnno and not hasGenAsRetAnno))
+
+                # fmt: on
+            ):
                 # If "Generator[...]" is put in the return type annotation,
                 # we don't need a "Returns" section in the docstring. Instead,
                 # we need a "Yields" section.
                 if self.requireReturnSectionWhenReturningNone:
                     violations.append(v201)
                 elif not isReturnAnnotationNone(node):
                     violations.append(v201)
```

### Comparing `pydoclint-0.0.7/pydoclint.egg-info/PKG-INFO` & `pydoclint-0.0.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: pydoclint
-Version: 0.0.7
-Summary: A linter to check arguments in Python docstrings
-Home-page: https://github.com/jsh9/pydoclint
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pydoclint
 
 A Python docstring linter to check whether a docstring's sections (arguments,
 returns, raises, ...) match the function signature or function implementation.
 
 It runs really fast. In fact, it is at least ~1,475 times faster than
 [darglint](https://github.com/terrencepreilly/darglint) (another linter of the
@@ -67,46 +54,62 @@
 ```
 flake8 --select=DOC <FILE_OR_FOLDER>
 ```
 
 If you don't include `--select=DOC` in your command, _flake8_ will also run
 other built-in _flake8_ linters on your code.
 
-### 2.3. Native vs _flake8_
+### 2.3. As a pre-commit hook
+
+`pydoclint` is configured for [pre-commit](https://pre-commit.com/) and can be
+set up as a hook with the following `.pre-commit-config.yaml` configuration:
+
+```yaml
+- repo: https://github.com/jsh9/pydoclint
+  rev: <latest_tag>
+  hooks:
+    - id: pydoclint
+      args:
+        - "--config=pyproject.toml"
+```
+
+You will need to install `pre-commit` and run `pre-commit install`.
+
+### 2.4. Native vs _flake8_
 
 Should I use _pydoclint_ as a native command line tool or a _flake8_ plugin?
 Here's comparison:
 
 |                 | Pros                                     | Cons                                                          |
 | --------------- | ---------------------------------------- | ------------------------------------------------------------- |
 | Native tool     | Slightly faster                          | No inline or project-wide omission support right now [*]      |
 | _flake8_ plugin | Supports inline or project-wide omission | Slightly slower because other flake8 plugins are run together |
 
 \*) This feature may be added in the near future
 
-### 2.4. Configuration
+### 2.5. Configuration
 
 Here is how to configure _pydoclint_. For detailed explanations of all options,
 see [Section 4](#4-configuration-options) below.
 
-#### 2.4.1. Setting options inline
+#### 2.5.1. Setting options inline
 
 - Native:
 
   ```bash
   pydoclint --check-arg-order=False <FILE_OR_FOLDER_PATH>
   ```
 
 - Flake8:
 
   ```bash
   flake8 --check-arg-order=False <FILE_OR_FOLDER_PATH>
   ```
 
-#### 2.4.2. Setting options in a configuration file
+#### 2.5.2. Setting options in a configuration file
 
 - Native:
 
   - In a `.toml` file somewhere in your project folder, add a section like this
     (put in the config that you need):
 
     ```toml
@@ -135,21 +138,21 @@
 
 | Code     | Explanation                              |
 | -------- | ---------------------------------------- |
 | `DOC001` | Potential formatting errors in docstring |
 
 ### 3.1. `DOC1xx`: Violations about input arguments
 
-| Code     | Explanation                                                                                                                                          |
-| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `DOC101` | Docstring contains fewer arguments than in function signature                                                                                        |
-| `DOC102` | Docstring contains more arguments than in function signature                                                                                         |
+| Code     | Explanation                                                                                                                                         |
+| -------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `DOC101` | Docstring contains fewer arguments than in function signature                                                                                       |
+| `DOC102` | Docstring contains more arguments than in function signature                                                                                        |
 | `DOC103` | Docstring arguments are different from function arguments. (Or could be other formatting issues: https://github.com/jsh9/pydoclint#notes-on-doc103) |
-| `DOC104` | Arguments are the same in the docstring and the function signature, but are in a different order.                                                    |
-| `DOC105` | Argument names match, but type hints do not match                                                                                                    |
+| `DOC104` | Arguments are the same in the docstring and the function signature, but are in a different order.                                                   |
+| `DOC105` | Argument names match, but type hints do not match                                                                                                   |
 
 #### Notes on `DOC103`:
 
 Other potential causes to `DOC103` include:
 
 - Numpy docstring style requires this style: `arg1 : int` (a space between
   `arg1` and `:`) but people sometimes write `arg1: int`. This will trigger
```

### Comparing `pydoclint-0.0.7/pydoclint.egg-info/SOURCES.txt` & `pydoclint-0.0.8/pydoclint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.7/setup.cfg` & `pydoclint-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pydoclint
-version = 0.0.7
+version = 0.0.8
 description = A linter to check arguments in Python docstrings
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jsh9/pydoclint
 license = MIT
 license_file = LICENSE
 classifiers =
```

### Comparing `pydoclint-0.0.7/tests/test_main.py` & `pydoclint-0.0.8/tests/test_main.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,154 +12,154 @@
 
 
 expectedViolations_True_True = [
     'DOC101: Method `MyClass.func1_3`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func1_3`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in '
     'the docstring: [arg1: str, arg2: list[int]].',
     'DOC102: Method `MyClass.func1_6`: Docstring contains more arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func1_6`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the docstring but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the docstring but not in the '
     'function signature: [arg1: int].',
     'DOC101: Method `MyClass.func2`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func2`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in '
     'the docstring: [arg2: float | int | None].',
     'DOC102: Method `MyClass.func3`: Docstring contains more arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func3`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the docstring but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the docstring but not in the '
     'function signature: [arg3: Optional[Union[float, int, str]]].',
     'DOC104: Method `MyClass.func4`: Arguments are the same in the docstring and '
     'the function signature, but are in a different order. ',
     'DOC105: Method `MyClass.func5`: Argument names match, but type hints do not '
     'match ',
     'DOC104: Method `MyClass.func6`: Arguments are the same in the docstring and '
     'the function signature, but are in a different order. ',
     'DOC105: Method `MyClass.func6`: Argument names match, but type hints do not '
     'match ',
     'DOC101: Function `func72`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Function `func72`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in the '
     'docstring: [arg3: list, arg4: tuple, arg5: dict].',
 ]
 
 expectedViolations_False_True = [
     'DOC101: Method `MyClass.func1_3`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func1_3`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in '
     'the docstring: [arg1: str, arg2: list[int]].',
     'DOC102: Method `MyClass.func1_6`: Docstring contains more arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func1_6`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the docstring but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the docstring but not in the '
     'function signature: [arg1: int].',
     'DOC101: Method `MyClass.func2`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func2`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in '
     'the docstring: [arg2: float | int | None].',
     'DOC102: Method `MyClass.func3`: Docstring contains more arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func3`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the docstring but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the docstring but not in the '
     'function signature: [arg3: Optional[Union[float, int, str]]].',
     'DOC104: Method `MyClass.func4`: Arguments are the same in the docstring and '
     'the function signature, but are in a different order. ',
     'DOC104: Method `MyClass.func6`: Arguments are the same in the docstring and '
     'the function signature, but are in a different order. ',
     'DOC101: Function `func72`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Function `func72`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in the '
     'docstring: [arg3: list, arg4: tuple, arg5: dict].',
 ]
 
 expectedViolations_True_False = [
     'DOC101: Method `MyClass.func1_3`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func1_3`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in '
     'the docstring: [arg1: str, arg2: list[int]].',
     'DOC102: Method `MyClass.func1_6`: Docstring contains more arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func1_6`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the docstring but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the docstring but not in the '
     'function signature: [arg1: int].',
     'DOC101: Method `MyClass.func2`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func2`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in '
     'the docstring: [arg2: float | int | None].',
     'DOC102: Method `MyClass.func3`: Docstring contains more arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func3`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the docstring but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the docstring but not in the '
     'function signature: [arg3: Optional[Union[float, int, str]]].',
     'DOC105: Method `MyClass.func5`: Argument names match, but type hints do not '
     'match ',
     'DOC105: Method `MyClass.func6`: Argument names match, but type hints do not '
     'match ',
     'DOC101: Function `func72`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Function `func72`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in the '
     'docstring: [arg3: list, arg4: tuple, arg5: dict].',
 ]
 
 expectedViolations_False_False = [
     'DOC101: Method `MyClass.func1_3`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func1_3`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in '
     'the docstring: [arg1: str, arg2: list[int]].',
     'DOC102: Method `MyClass.func1_6`: Docstring contains more arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func1_6`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the docstring but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the docstring but not in the '
     'function signature: [arg1: int].',
     'DOC101: Method `MyClass.func2`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func2`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in '
     'the docstring: [arg2: float | int | None].',
     'DOC102: Method `MyClass.func3`: Docstring contains more arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func3`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the docstring but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the docstring but not in the '
     'function signature: [arg3: Optional[Union[float, int, str]]].',
     'DOC101: Function `func72`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Function `func72`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in the '
     'docstring: [arg3: list, arg4: tuple, arg5: dict].',
 ]
 
 expectedViolationsLookup: Dict[str, List[str]] = {
     'true_true': expectedViolations_True_True,
     'true_false': expectedViolations_True_False,
     'false_true': expectedViolations_False_True,
@@ -236,15 +236,15 @@
         'docstring ',
         'DOC201: Method `MyClass.func1_6` does not have a return section in '
         'docstring ',
         'DOC101: Method `MyClass.func2`: Docstring contains fewer arguments than in '
         'function signature. ',
         'DOC103: Method `MyClass.func2`: Docstring arguments are different from '
         'function arguments. (Or could be other formatting issues: '
-        'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in '
+        'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in '
         'the docstring: [arg2: float, arg3: str]. Arguments in the docstring but not '
         'in the function signature: [arg1: int].',
         'DOC201: Function `func52` does not have a return section in docstring ',
         'DOC202: Method `MyClass.func6` has a return section in docstring, but there '
         'are no return statements or annotations ',
     ]
 
@@ -263,40 +263,40 @@
 
 
 expected_True = [
     'DOC101: Function `func3`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Function `func3`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in the '
     'docstring: [arg1: , arg2: , arg3: ]. Arguments in the docstring but not in '
     'the function signature: [var1: int, var2: str].',
     'DOC201: Function `func3` does not have a return section in docstring ',
 ]
 
 expected_False = [
     'DOC101: Function `func1`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Function `func1`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in the '
     'docstring: [arg1: , arg2: , arg3: ].',
     'DOC201: Function `func1` does not have a return section in docstring ',
     'DOC101: Function `func2`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Function `func2`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in the '
     'docstring: [arg1: , arg2: , arg3: ].',
     'DOC201: Function `func2` does not have a return section in docstring ',
     'DOC101: Function `func3`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Function `func3`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in the '
+    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in the '
     'docstring: [arg1: , arg2: , arg3: ]. Arguments in the docstring but not in '
     'the function signature: [var1: int, var2: str].',
     'DOC201: Function `func3` does not have a return section in docstring ',
 ]
 
 
 @pytest.mark.parametrize(
@@ -337,15 +337,15 @@
         'because __init__() cannot return anything ',
         'DOC105: Method `C.__init__`: Argument names match, but type hints do not '
         'match ',
         'DOC302: Class `C`: The class docstring does not need a "Returns" section, '
         'because __init__() cannot return anything ',
         'DOC103: Method `D.__init__`: Docstring arguments are different from function '
         'arguments. (Or could be other formatting issues: '
-        'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in the '
+        'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in the '
         'docstring: [arg1: int, arg2: float]. Arguments in the docstring but not in '
         'the function signature: [var1: list, var2: dict].',
         'DOC302: Class `D`: The class docstring does not need a "Returns" section, '
         'because __init__() cannot return anything ',
     ]
     assert list(map(str, violations)) == expected
 
@@ -396,14 +396,29 @@
         'have a "Yields" section ',
         'DOC402: Method `A.method1` has "yield" statements, but the docstring does '
         'not have a "Yields" section ',
         'DOC402: Method `A.method2` has "yield" statements, but the docstring does '
         'not have a "Yields" section ',
         'DOC403: Method `A.method3` has a "Yields" section in the docstring, but '
         'there are no "yield" statements or a Generator return annotation ',
+        'DOC401: Method `A.method6` returns a Generator, but the docstring does not '
+        'have a "Yields" section ',
+        'DOC402: Method `A.method6` has "yield" statements, but the docstring does '
+        'not have a "Yields" section ',
+        'DOC402: Method `A.method8a` has "yield" statements, but the docstring does '
+        'not have a "Yields" section ',
+        'DOC402: Method `A.method8b` has "yield" statements, but the docstring does '
+        'not have a "Yields" section ',
+        'DOC402: Method `A.method8c` has "yield" statements, but the docstring does '
+        'not have a "Yields" section ',
+        'DOC402: Method `A.method8d` has "yield" statements, but the docstring does '
+        'not have a "Yields" section ',
+        'DOC201: Method `A.zipLists2` does not have a return section in docstring ',
+        'DOC403: Method `A.zipLists2` has a "Yields" section in the docstring, but '
+        'there are no "yield" statements or a Generator return annotation ',
     ]
     assert list(map(str, violations)) == expected
 
 
 @pytest.mark.parametrize(
     'style, skipRaisesCheck',
     itertools.product(
@@ -435,33 +450,33 @@
     violations = _checkFile(
         filename=DATA_DIR / f'{style}/star_args/cases.py',
         style=style,
     )
     expected = [
         'DOC103: Function `func2`: Docstring arguments are different from function '
         'arguments. (Or could be other formatting issues: '
-        'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in the '
+        'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in the '
         'docstring: [**kwargs: ]. Arguments in the docstring but not in the function '
         'signature: [kwargs: ].',
         'DOC103: Function `func4`: Docstring arguments are different from function '
         'arguments. (Or could be other formatting issues: '
-        'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in the '
+        'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in the '
         'docstring: [*args: ]. Arguments in the docstring but not in the function '
         'signature: [args: ].',
         'DOC101: Function `func6`: Docstring contains fewer arguments than in '
         'function signature. ',
         'DOC103: Function `func6`: Docstring arguments are different from function '
         'arguments. (Or could be other formatting issues: '
-        'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in the '
+        'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in the '
         'docstring: [**kwargs: , *args: ].',
         'DOC101: Function `func7`: Docstring contains fewer arguments than in '
         'function signature. ',
         'DOC103: Function `func7`: Docstring arguments are different from function '
         'arguments. (Or could be other formatting issues: '
-        'https://github.com/jsh9/pydoclint#notes-on-doc103). Arguments in the function signature but not in the '
+        'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in the '
         'docstring: [**kwargs: , *args: , arg1: float, arg2: str]. Arguments in the '
         'docstring but not in the function signature: [arg1: int, arg2: dict].',
     ]
     assert list(map(str, violations)) == expected
 
 
 def testParsingErrors_google() -> None:
@@ -547,7 +562,18 @@
     """
     violations = _checkFile(
         filename=DATA_DIR / 'playground.py',
         style='google',
     )
     expected = []
     assert list(map(str, violations)) == expected
+
+
+def testNonAscii() -> None:
+    """Don't crash on non ASCII arguments."""
+    violations = _checkFile(
+        filename=DATA_DIR / 'common/non_ascii/non_ascii.py',
+        style='numpy',
+        skipCheckingShortDocstrings=False,
+    )
+    expected = []
+    assert list(map(str, violations)) == expected
```

### Comparing `pydoclint-0.0.7/tests/test_parse_config.py` & `pydoclint-0.0.8/tests/test_parse_config.py`

 * *Files identical despite different names*

