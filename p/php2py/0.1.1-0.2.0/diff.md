# Comparing `tmp/php2py-0.1.1.tar.gz` & `tmp/php2py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "php2py-0.1.1.tar", max compression
+gzip compressed data, was "php2py-0.2.0.tar", max compression
```

## Comparing `php2py-0.1.1.tar` & `php2py-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,41 @@
--rw-r--r--   0        0        0     1559 2023-05-23 06:32:18.069556 php2py-0.1.1/LICENSE
--rw-r--r--   0        0        0     1898 2023-05-23 07:14:27.931239 php2py-0.1.1/README.md
--rw-r--r--   0        0        0     1256 2023-05-23 07:14:50.964995 php2py-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-03-05 11:27:00.834601 php2py-0.1.1/src/php2py/__init__.py
--rw-r--r--   0        0        0      216 2022-03-04 18:54:00.719295 php2py-0.1.1/src/php2py/etc/composer.json
--rw-r--r--   0        0        0     2448 2023-05-23 06:32:18.070273 php2py-0.1.1/src/php2py/etc/composer.lock
--rw-r--r--   0        0        0     1064 2023-05-23 07:09:01.029475 php2py-0.1.1/src/php2py/main.py
--rw-r--r--   0        0        0     1990 2023-05-23 06:56:16.686004 php2py-0.1.1/src/php2py/parser.py
--rw-r--r--   0        0        0    14892 2022-03-08 17:39:04.665953 php2py-0.1.1/src/php2py/php_ast.py
--rw-r--r--   0        0        0    34971 2022-03-08 17:43:12.031753 php2py-0.1.1/src/php2py/translator.py
--rw-r--r--   0        0        0        0 2023-05-23 06:32:18.074916 php2py-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0       40 2022-03-08 09:11:16.167491 php2py-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0      930 2023-05-23 06:32:18.076808 php2py-0.1.1/tests/test_assignments.py
--rw-r--r--   0        0        0      968 2023-05-23 06:32:18.078753 php2py-0.1.1/tests/test_classes.py
--rw-r--r--   0        0        0     2011 2023-05-23 06:35:52.574763 php2py-0.1.1/tests/test_control_flow.py
--rw-r--r--   0        0        0     1412 2023-05-23 06:32:18.080739 php2py-0.1.1/tests/test_functions.py
--rw-r--r--   0        0        0     3095 2023-05-23 06:32:18.081938 php2py-0.1.1/tests/test_translator.py
--rw-r--r--   0        0        0      246 2023-05-23 06:32:18.082305 php2py-0.1.1/tests/test_whole_programs.py
--rw-r--r--   0        0        0     2209 2023-05-23 07:01:27.241961 php2py-0.1.1/tests/util.py
--rw-r--r--   0        0        0     2759 1970-01-01 00:00:00.000000 php2py-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1559 2023-05-23 06:32:18.069556 php2py-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1814 2023-06-05 14:23:45.698510 php2py-0.2.0/README.md
+-rw-r--r--   0        0        0     1393 2023-06-06 20:56:17.692472 php2py-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-03-05 11:27:00.834601 php2py-0.2.0/src/php2py/__init__.py
+-rw-r--r--   0        0        0      548 2023-06-05 16:56:34.801404 php2py-0.2.0/src/php2py/ast_utils.py
+-rw-r--r--   0        0        0      986 2023-06-05 19:50:11.170994 php2py-0.2.0/src/php2py/cli.py
+-rw-r--r--   0        0        0       20 2023-06-05 14:46:20.943782 php2py-0.2.0/src/php2py/constants.py
+-rw-r--r--   0        0        0      216 2022-03-04 18:54:00.719295 php2py-0.2.0/src/php2py/etc/composer.json
+-rw-r--r--   0        0        0     2448 2023-05-23 06:32:18.070273 php2py-0.2.0/src/php2py/etc/composer.lock
+-rw-r--r--   0        0        0      921 2023-06-05 19:50:55.889189 php2py-0.2.0/src/php2py/main.py
+-rw-r--r--   0        0        0     2976 2023-06-06 07:00:22.797890 php2py-0.2.0/src/php2py/parser.py
+-rw-r--r--   0        0        0    15146 2023-06-06 14:21:40.748925 php2py-0.2.0/src/php2py/php_ast.py
+-rw-r--r--   0        0        0      134 2023-06-06 06:41:11.970178 php2py-0.2.0/src/php2py/py_ast.py
+-rw-r--r--   0        0        0       61 2023-06-06 09:24:10.540290 php2py-0.2.0/src/php2py/translator/__init__.py
+-rw-r--r--   0        0        0       92 2023-06-06 09:17:44.073166 php2py-0.2.0/src/php2py/translator/base.py
+-rw-r--r--   0        0        0    18513 2023-06-06 14:20:08.531749 php2py-0.2.0/src/php2py/translator/exprs.py
+-rw-r--r--   0        0        0     1361 2023-06-06 09:21:18.488252 php2py-0.2.0/src/php2py/translator/scalars.py
+-rw-r--r--   0        0        0    19953 2023-06-06 14:55:28.396695 php2py-0.2.0/src/php2py/translator/stmts.py
+-rw-r--r--   0        0        0     1623 2023-06-06 10:38:08.438816 php2py-0.2.0/src/php2py/translator/translator.py
+-rw-r--r--   0        0        0     1098 2023-06-06 07:44:17.501541 php2py-0.2.0/src/php2py/translator/utils.py
+-rw-r--r--   0        0        0        0 2023-05-23 06:32:18.074916 php2py-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0       40 2022-03-08 09:11:16.167491 php2py-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0    10518 2023-06-06 06:47:42.115074 php2py-0.2.0/tests/programs/RepositorySchema.php
+-rw-r--r--   0        0        0    14477 2023-06-01 12:42:34.000000 php2py-0.2.0/tests/programs/TransportInterface.php
+-rw-r--r--   0        0        0     6008 2023-06-06 06:59:49.795122 php2py-0.2.0/tests/programs/_XmlToPropsParser.php
+-rw-r--r--   0        0        0      180 2023-05-24 14:06:19.749813 php2py-0.2.0/tests/programs/class.php
+-rw-r--r--   0        0        0      301 2023-05-24 14:07:23.988724 php2py-0.2.0/tests/programs/if.php
+-rw-r--r--   0        0        0      209 2023-05-24 14:05:42.894895 php2py-0.2.0/tests/programs/variables.php
+-rw-r--r--   0        0        0        0 2023-06-06 09:18:02.369955 php2py-0.2.0/tests/snippets/__init__.py
+-rw-r--r--   0        0        0      453 2023-06-06 09:18:21.853566 php2py-0.2.0/tests/snippets/class.py
+-rw-r--r--   0        0        0      313 2023-06-06 06:45:52.324808 php2py-0.2.0/tests/snippets/switch.py
+-rw-r--r--   0        0        0      170 2023-06-06 06:45:11.382027 php2py-0.2.0/tests/snippets/use.py
+-rw-r--r--   0        0        0      890 2023-06-06 14:07:12.282645 php2py-0.2.0/tests/test_assignments.py
+-rw-r--r--   0        0        0      968 2023-05-23 06:32:18.078753 php2py-0.2.0/tests/test_classes.py
+-rw-r--r--   0        0        0     2332 2023-06-06 14:52:10.424973 php2py-0.2.0/tests/test_control_flow.py
+-rw-r--r--   0        0        0     1414 2023-06-06 07:17:07.912896 php2py-0.2.0/tests/test_functions.py
+-rw-r--r--   0        0        0      624 2023-06-06 14:05:41.597663 php2py-0.2.0/tests/test_snippets.py
+-rw-r--r--   0        0        0     3096 2023-06-06 07:17:16.115088 php2py-0.2.0/tests/test_translator.py
+-rw-r--r--   0        0        0      447 2023-06-06 09:18:49.588686 php2py-0.2.0/tests/test_whole_programs.py
+-rw-r--r--   0        0        0     3444 2023-06-06 14:50:36.700779 php2py-0.2.0/tests/util.py
+-rw-r--r--   0        0        0     2761 1970-01-01 00:00:00.000000 php2py-0.2.0/PKG-INFO
```

### Comparing `php2py-0.1.1/LICENSE` & `php2py-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `php2py-0.1.1/README.md` & `php2py-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 # php2py
 
 [![image](https://img.shields.io/pypi/v/php2py.svg)](https://pypi.python.org/pypi/php2py)
 
-[![image](https://img.shields.io/travis/sfermigier/php2py.svg)](https://travis-ci.com/sfermigier/php2py)
-
-[![Documentation Status](https://readthedocs.org/projects/php2py/badge/?version=latest)](https://php2py.readthedocs.io/en/latest/?version=latest)
-
 PHP to Python transpiler.
 
 -   Free software: GNU General Public License v3
--   Documentation: <https://php2py.readthedocs.io> (nope!).
 
 ## Use cases
 
 - Helping port PHP code to Python (provides a first pass, which can then be
   manually edited).
 
 ## Features
@@ -52,20 +47,26 @@
 
 ## TODO
 
 - Add test cases (real programs) and make sure they pass.
 - Make a runtime / stdlib of common PHP functions in Python.
 - Cleanup.
 
+## Prior art
+
+- <https://github.com/nicolasrod/php2python>
+
 ## Contributing
 
 I don't have time to work on this project ATM, but I'm happy to review pull requests.
 
 If you are a student (or a group of students) in a computer science or engineering program, and you want to work on this, please contact me (<mailto:sf@abilian.com>).
 
+If you think this project can be useful for your company, you can support the development effort through a sponsorship via my company, Abilian: <https://abilian.com/>.
+
 ## Credits
 
 This package was created with [Cruft](https://cruft.github.io/cruft/) and the
 [abilian/cookiecutter-abilian-python](https://github.com/abilian/cookiecutter-abilian-python)
 project template.
 
 This project uses the `nikic/php-parser` PHP parser (in PHP).
```

### Comparing `php2py-0.1.1/pyproject.toml` & `php2py-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "php2py"
-version = "0.1.1"
+version = "0.2.0"
 homepage = "https://github.com/sfermigier/php2py"
 description = "PHP to Python transpiler."
 authors = ["Abilian SAS <sf@abilian.com>"]
 readme = "README.md"
 classifiers = [
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
@@ -20,29 +20,35 @@
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
 astor = "^0.8.1"
 attrs = "^23.1.0"
 
 # For debugging. Remove later.
-icecream = "^2.1.2"
-rich = "^11.2.0"
-devtools = "^0.8.0"
-astpretty = "^2.1.0"
+icecream = "^2.1.3"
+rich = "^13.4.1"
+devtools = "^0.11.0"
+astpretty = "^3.0.0"
 click = "^8.1.3"
+platformdirs = "^3.5.1"
+cleez = "^0.1.11"
 
 [tool.poetry.dev-dependencies]
-abilian-devtools = "*"
+abilian-devtools = "^0.5.2"
 
-restructuredtext_lint = "*"
+restructuredtext_lint = "^1.4.0"
 
 [tool.poetry.scripts]
-php2py = "php2py.main:main"
+php2py = "php2py.cli:cli"
 
 
+[tool.poetry.group.dev.dependencies]
+abilian-devtools = "^0.5.2"
+coverage = "^7.2.7"
+
 [tool.ruff]
 extend-ignore = [
     "S101", # Use of 'assert'
     "E501", # Line too long
     # TODO: fix these
     "F841", # Local variable `key` is assigned to but never used
 ]
```

### Comparing `php2py-0.1.1/src/php2py/etc/composer.lock` & `php2py-0.2.0/src/php2py/etc/composer.lock`

 * *Files identical despite different names*

### Comparing `php2py-0.1.1/src/php2py/parser.py` & `php2py-0.2.0/src/php2py/parser.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,68 @@
 import json
 import shlex
+import shutil
 import subprocess
 import tempfile
 from pathlib import Path
 
+from devtools import debug
+from platformdirs import user_cache_dir
+
 from . import php_ast
+from .constants import APP_NAME
+
+PHP_PARSE = "vendor/nikic/php-parser/bin/php-parse"
+
+
+def install_parser(force: bool = False, ignore_errors: bool = False):
+    cache_dir = Path(user_cache_dir(APP_NAME))
+    php_parse = cache_dir / PHP_PARSE
+
+    if not force and php_parse.exists():
+        return
+
+    Path(cache_dir).mkdir(exist_ok=True)
+
+    etc_dir = Path(__file__).parent / "etc"
+    print(etc_dir)
+    for file in etc_dir.glob("*"):
+        dest = cache_dir / file.name
+        print(dest)
+        if dest.exists():
+            continue
+        dest.write_text(file.read_text())
+
+    subprocess.run("composer install", shell=True, cwd=cache_dir)
 
 
-def parse(source_code: str, php_parse: str | Path = ""):
-    if not php_parse:
-        php_parse = "vendor/nikic/php-parser/bin/php-parse"
-    php_parse = Path(php_parse)
+def parse(source_code):
+    cache_dir = Path(user_cache_dir(APP_NAME))
+    php_parse = cache_dir / PHP_PARSE
     assert php_parse.exists()
 
     with tempfile.NamedTemporaryFile("w", suffix=".php", delete=False) as source_file:
         source_file.write(source_code)
         source_file.flush()
 
         cmd_line = f"{php_parse} -j {source_file.name}"
         args = shlex.split(cmd_line)
+        which = shutil.which(args[0])
+        assert which is not None
         with subprocess.Popen(
-            args, stdout=subprocess.PIPE, stderr=subprocess.DEVNULL
+            args,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
         ) as p:
-            json_ast = json.load(p.stdout)
+            data = p.stdout.read()
+            try:
+                json_ast = json.loads(data)
+            except json.JSONDecodeError:
+                debug(args, which, data, stderr=p.stderr.read())
+                raise ValueError("Could not parse PHP file")
             result = make_ast(json_ast)
 
     return result
 
 
 def make_ast(
     json_node: list | dict | str | int | None,
```

### Comparing `php2py-0.1.1/src/php2py/php_ast.py` & `php2py-0.2.0/src/php2py/php_ast.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from typing import Any
 
 from attr import dataclass
+from devtools import debug
 
 frozen = dataclass
 
 
 @frozen
 class Node:
     def __getitem__(self, item):
@@ -19,14 +20,24 @@
         return self._json["attributes"]["startLine"]
 
     @property
     def _col_offset(self):
         return 0
         # return self._attributes["col_offset"]
 
+    def get_parts(self):
+        if "parts" in self._json:
+            return self._json["parts"]
+
+        if "name" in self._json:
+            return [self._json["name"]]
+
+        debug(self._json)
+        raise ValueError()
+
 
 @frozen
 class Expr(Node):
     pass
 
 
 @frozen
@@ -537,16 +548,16 @@
 class Expr_StaticPropertyFetch(Expr):
     class_: Expr | Name | Scalar_String
     name: Expr | VarLikeIdentifier
 
 
 @frozen
 class Expr_Ternary(Expr):
-    if_: Expr | None | Scalar_Encapsed | Scalar_LNumber | Scalar_String
     cond: Expr
+    if_: Expr | None | Scalar_Encapsed | Scalar_LNumber | Scalar_String
     else_: Expr | Scalar_DNumber | Scalar_Encapsed | Scalar_LNumber | Scalar_String
 
 
 @frozen
 class Expr_Throw(Expr):
     expr: Expr
 
@@ -685,21 +696,21 @@
     var: Expr
     types: list[Node]
     stmts: list[Stmt]
 
 
 @frozen
 class Stmt_Class(Stmt):
+    name: Identifier | None
+    implements: list[Node] | list[Stmt]
+    extends: Name | Name_FullyQualified | None
+    stmts: list[Stmt]
     attrGroups: list[Stmt]
     flags: int
-    extends: Name | Name_FullyQualified | None
-    implements: list[Node] | list[Stmt]
     namespacedName: None
-    stmts: list[Stmt]
-    name: Identifier | None
 
 
 @frozen
 class Stmt_ClassConst(Stmt):
     flags: int
     attrGroups: list[Stmt]
     consts: list[Node]
@@ -736,16 +747,16 @@
 class Stmt_DeclareDeclare(Stmt):
     key: Identifier
     value: Scalar_LNumber
 
 
 @frozen
 class Stmt_Do(Stmt):
-    stmts: list[Stmt]
     cond: Expr | Scalar_LNumber
+    stmts: list[Stmt]
 
 
 @frozen
 class Stmt_Echo(Stmt):
     exprs: list[Expr] | list[Node] | list[Scalar]
```

### Comparing `php2py-0.1.1/tests/test_assignments.py` & `php2py-0.2.0/tests/test_assignments.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+from textwrap import dedent
+
+import pytest
+
 from .util import check_compiles
 
 
 def test_assign():
     input = r"""<?php
         $a = 1;
         $b = +2;
@@ -23,26 +27,25 @@
 def test_assignment_ops():
     input = r"""<?php
         $a += 5;
         $b -= 6;
         $c .= $d;
         $e ^= $f;
     ?>"""
-    expected = (
-        "a += 5\n"
-        "\n"
-        "b += 6\n"
-        "\n"
-        "c += d\n"
-        "\n"
-        "e += f"
-        #
+    expected = dedent(
+        """\
+        a += 5
+        b -= 6
+        c += d
+        e ^= f
+    """
     )
     check_compiles(input, expected)
 
 
-# def test_list_assignment():
-#     input = r"""<?php
-#         list($a, $b, $c) = $d;
-#     ?>"""
-#     expected = "xxx += 5\n" "\n" "xxx -= 6\n" "\n" "xxx += d\n" "\n" "xxx ^= f"
-#     check_compiles(input, expected)
+@pytest.mark.skip("TODO")
+def test_list_assignment():
+    input = r"""<?php
+        list($a, $b, $c) = $d;
+    ?>"""
+    expected = ""
+    check_compiles(input, expected)
```

### Comparing `php2py-0.1.1/tests/test_classes.py` & `php2py-0.2.0/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `php2py-0.1.1/tests/test_functions.py` & `php2py-0.2.0/tests/test_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 def test_function():
     input = """<?php
         function foo() {
             echo "bar";
         }
         foo();
     """
-    expected = "def foo():\n" "    echo('bar')\n" "foo()"
+    expected = "def foo():\n" "    print('bar')\n" "foo()"
     check_compiles(input, expected)
 
 
 def test_function_with_args():
     input = """<?php
         function foo($bar) {
             echo $bar;
         }
         foo();
     """
-    expected = "def foo(bar):\n" "    echo(bar)\n" "foo()"
+    expected = "def foo(bar):\n" "    print(bar)\n" "foo()"
     check_compiles(input, expected)
 
 
 def test_more_function_calls():
     input = r"""<?php
         # doit($arg1, &$arg2, 3 + 4);
         name\spaced();
```

### Comparing `php2py-0.1.1/tests/test_translator.py` & `php2py-0.2.0/tests/test_translator.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         "e = None"
     )
     check_compiles(input, expected)
 
 
 def test_echo():
     input = '<?php echo "hello, world!"; ?>'
-    expected = "echo('hello, world!')"
+    expected = "print('hello, world!')"
     check_compiles(input, expected)
 
 
 def test_string_unescape():
     # TODO: check this is correct
     input = r"""<?php "\r\n\t" ?>"""
     expected = '"""\\r\n\t"""'
```

### Comparing `php2py-0.1.1/tests/util.py` & `php2py-0.2.0/tests/util.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import ast
+import re
 import shlex
 import subprocess
+import sys
 import tempfile
 from ast import unparse
 
+import astpretty
 import rich
+from cleez.colors import red
 from devtools import debug
 
 from php2py.parser import parse
 from php2py.translator import Translator
 
 
 def translate(source):
@@ -51,15 +55,15 @@
         ) as p:
             p.wait()
 
         fd.seek(0)
         return print(fd.read())
 
 
-def check_compiles(input, expected):
+def check_compiles(input, expected=""):
     php_ast = parse(input)
     try:
         py_ast = translate(input)
     except:
         rich.print("[red]Error while translating[/red]")
         print("php_ast:")
         dump_php_ast(php_ast)
@@ -67,21 +71,74 @@
 
     try:
         output = unparse(py_ast)
     except:
         rich.print("[red]Error while translating[/red]")
         print("php_ast:")
         dump_php_ast(php_ast)
-        print("py_ast=", ast.dump(py_ast, indent=2))
+        print("py_ast:", ast.dump(py_ast, indent=2))
         # print("py_ast=", astpretty.pprint(py_ast, indent="  "))
         raise
 
     output = output.strip()
 
-    if expected != output:
-        print("php_ast:")
+    # Check Python code is syntactically valid
+    output_ast = ast.parse(output)
+
+    if not expected:
+        return
+
+    expected = blacken(expected).strip()
+    blacked_output = blacken(output).strip()
+
+    if not compare(blacked_output, expected):
+        print(red("php_ast:"))
+        print(78 * "-")
         dump_php_ast(php_ast)
-        print("py_ast=", ast.dump(py_ast, indent=2))
-        # print("py_ast=", astpretty.pprint(py_ast, indent="  "))
-        debug(output)
+        print(78 * "-")
+
+        print(red("py_ast:"))
+        print(78 * "-")
+        astpretty.pprint(output_ast)
+        print(78 * "-")
+
+        print(red("expected:"))
+        print(78 * "-")
+        print(expected)
+        print(78 * "-")
+
+        print(red("output:"))
+        print(78 * "-")
+        print(output)
+        print(78 * "-")
+
+        print(red("output formatted:"))
+        print(78 * "-")
+        print(blacked_output)
+        print(78 * "-")
+
+        sys.stdout.flush()
+
+    assert compare(blacked_output, expected)
+
 
-    assert expected == output
+def compare(s1, s2) -> bool:
+    s1 = re.sub("\n+", "\n", s1)
+    s2 = re.sub("\n+", "\n", s2)
+    return s1 == s2
+
+
+def blacken(code):
+    with tempfile.NamedTemporaryFile("w+", suffix=".py") as fd:
+        fd.write(code)
+        fd.flush()
+
+        cmd_line = f"black {fd.name}"
+        args = shlex.split(cmd_line)
+        with subprocess.Popen(
+            args, stdout=subprocess.PIPE, stderr=subprocess.PIPE
+        ) as p:
+            stdout, stderr = p.communicate()
+            p.wait()
+
+        fd.seek(0)
+        return fd.read()
```

### Comparing `php2py-0.1.1/PKG-INFO` & `php2py-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 Metadata-Version: 2.1
 Name: php2py
-Version: 0.1.1
+Version: 0.2.0
 Summary: PHP to Python transpiler.
 Home-page: https://github.com/sfermigier/php2py
 Author: Abilian SAS
 Author-email: sf@abilian.com
 Requires-Python: >=3.9,<4
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: astor (>=0.8.1,<0.9.0)
-Requires-Dist: astpretty (>=2.1.0,<3.0.0)
+Requires-Dist: astpretty (>=3.0.0,<4.0.0)
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
+Requires-Dist: cleez (>=0.1.11,<0.2.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: devtools (>=0.8.0,<0.9.0)
-Requires-Dist: icecream (>=2.1.2,<3.0.0)
-Requires-Dist: rich (>=11.2.0,<12.0.0)
+Requires-Dist: devtools (>=0.11.0,<0.12.0)
+Requires-Dist: icecream (>=2.1.3,<3.0.0)
+Requires-Dist: platformdirs (>=3.5.1,<4.0.0)
+Requires-Dist: rich (>=13.4.1,<14.0.0)
 Description-Content-Type: text/markdown
 
 # php2py
 
 [![image](https://img.shields.io/pypi/v/php2py.svg)](https://pypi.python.org/pypi/php2py)
 
-[![image](https://img.shields.io/travis/sfermigier/php2py.svg)](https://travis-ci.com/sfermigier/php2py)
-
-[![Documentation Status](https://readthedocs.org/projects/php2py/badge/?version=latest)](https://php2py.readthedocs.io/en/latest/?version=latest)
-
 PHP to Python transpiler.
 
 -   Free software: GNU General Public License v3
--   Documentation: <https://php2py.readthedocs.io> (nope!).
 
 ## Use cases
 
 - Helping port PHP code to Python (provides a first pass, which can then be
   manually edited).
 
 ## Features
@@ -76,20 +73,26 @@
 
 ## TODO
 
 - Add test cases (real programs) and make sure they pass.
 - Make a runtime / stdlib of common PHP functions in Python.
 - Cleanup.
 
+## Prior art
+
+- <https://github.com/nicolasrod/php2python>
+
 ## Contributing
 
 I don't have time to work on this project ATM, but I'm happy to review pull requests.
 
 If you are a student (or a group of students) in a computer science or engineering program, and you want to work on this, please contact me (<mailto:sf@abilian.com>).
 
+If you think this project can be useful for your company, you can support the development effort through a sponsorship via my company, Abilian: <https://abilian.com/>.
+
 ## Credits
 
 This package was created with [Cruft](https://cruft.github.io/cruft/) and the
 [abilian/cookiecutter-abilian-python](https://github.com/abilian/cookiecutter-abilian-python)
 project template.
 
 This project uses the `nikic/php-parser` PHP parser (in PHP).
```

