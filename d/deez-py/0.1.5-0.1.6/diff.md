# Comparing `tmp/deez_py-0.1.5.tar.gz` & `tmp/deez_py-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deez_py-0.1.5.tar", max compression
+gzip compressed data, was "deez_py-0.1.6.tar", max compression
```

## Comparing `deez_py-0.1.5.tar` & `deez_py-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3219 2023-06-06 12:01:30.162499 deez_py-0.1.5/README.rst
--rw-r--r--   0        0        0      225 2023-06-06 12:01:40.898396 deez_py-0.1.5/deez_py/__init__.py
--rw-r--r--   0        0        0      163 2023-06-06 11:13:48.158670 deez_py-0.1.5/deez_py/__main__.py
--rw-r--r--   0        0        0     2444 2023-06-06 11:25:46.594323 deez_py-0.1.5/deez_py/deez_ast.py
--rw-r--r--   0        0        0     9315 2023-06-06 11:35:43.905146 deez_py-0.1.5/deez_py/lexer.py
--rw-r--r--   0        0        0    11558 2023-06-06 11:56:51.589174 deez_py-0.1.5/deez_py/parser.py
--rw-r--r--   0        0        0      469 2023-06-06 10:15:33.712716 deez_py-0.1.5/deez_py/token_types.py
--rw-r--r--   0        0        0     1650 2023-06-06 11:04:32.801328 deez_py-0.1.5/deez_py/tokens.py
--rw-r--r--   0        0        0     1389 2023-06-06 12:01:55.880757 deez_py-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     4124 1970-01-01 00:00:00.000000 deez_py-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     3854 2023-06-06 17:24:26.039813 deez_py-0.1.6/README.rst
+-rw-r--r--   0        0        0      225 2023-06-06 17:41:32.093740 deez_py-0.1.6/deez_py/__init__.py
+-rw-r--r--   0        0        0      163 2023-06-06 11:13:48.158670 deez_py-0.1.6/deez_py/__main__.py
+-rw-r--r--   0        0        0     2444 2023-06-06 11:25:46.594323 deez_py-0.1.6/deez_py/deez_ast.py
+-rw-r--r--   0        0        0     9315 2023-06-06 11:35:43.905146 deez_py-0.1.6/deez_py/lexer.py
+-rw-r--r--   0        0        0    11558 2023-06-06 11:56:51.589173 deez_py-0.1.6/deez_py/parser.py
+-rw-r--r--   0        0        0      469 2023-06-06 10:15:33.712716 deez_py-0.1.6/deez_py/token_types.py
+-rw-r--r--   0        0        0     1650 2023-06-06 11:04:32.801328 deez_py-0.1.6/deez_py/tokens.py
+-rw-r--r--   0        0        0     1389 2023-06-06 17:41:53.157832 deez_py-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     4759 1970-01-01 00:00:00.000000 deez_py-0.1.6/PKG-INFO
```

### Comparing `deez_py-0.1.5/README.rst` & `deez_py-0.1.6/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -6,15 +6,15 @@
    :target: https://github.com/ThePrimeagen/ts-rust-zig-deez_py/tree/master/python/LICENSE
    :alt: License
 
 .. image:: https://img.shields.io/pypi/v/deez_py.svg
    :target: https://pypi.org/project/deez_py/
    :alt: pypi version
 
-**deez_py** is python implementation of a lexical analyzer that provides comprehensive scanning, and lookahead capabilities. It also implements a parser that comes with awesome functionalities.
+**deez_py** is a python implementation of a lexical analyzer that provides comprehensive scanning, and lookahead capabilities. It also implements a parser that comes with awesome functionalities.
 
 🛠️ Requirements
 ---------------
 
 **deez_py** requires Python 3.10 or above.
 
 To install Python 3.10.1, we recommend using `pyenv`_.
@@ -36,15 +36,14 @@
    # or if you using the default bash shell, do this instead:
    cat << EOF >> ~/.bashrc
    # pyenv config
    export PATH="${HOME}/.pyenv/bin:${PATH}"
    export PYENV_ROOT="${HOME}/.pyenv"
    eval "$(pyenv init -)"
    EOF
-
    # Close and open a new shell session
    # install Python 3.10.1
    pyenv install 3.10.1
 
    # make it available globally
    pyenv global system 3.10.1
 
@@ -52,15 +51,15 @@
 To manage the Python 3.10.1 virtualenv, we recommend using `poetry`_.
 
 .. code-block:: bash
 
    # install poetry
    curl -sSL https://install.python-poetry.org | python3 -
    poetry --version
-   Poetry (version 1.5.1)
+   Poetry \(version 1.5.1\)
 
    # Having the python executable in your PATH, you can use it:
    poetry env use 3.10.1
 
    # However, you are most likely to get the following issue:
    Creating virtualenv deez_py-dxc671ba-py3.10 in ~/.cache/pypoetry/virtualenvs
 
@@ -94,26 +93,72 @@
 
 .. code-block:: python3
 
    >>> from deez_py import Lexer
    >>> lex = Lexer('=+(){},;')
    >>> for _ in range(9):
    >>>     print(lex.get_next_token())
-   ... 
+   ...
    Token(type=<TokenType.Equal: '='>, literal='=')
    Token(type=<TokenType.Plus: '+'>, literal='+')
    Token(type=<TokenType.LParen: '('>, literal='(')
    Token(type=<TokenType.RParen: ')'>, literal=')')
    Token(type=<TokenType.LSquirly: '{'>, literal='{')
    Token(type=<TokenType.RSquirly: '}'>, literal='}')
    Token(type=<TokenType.Comma: ','>, literal=',')
    Token(type=<TokenType.Semicolon: ';'>, literal=';')
    Token(type=<TokenType.Eof: 'EOF'>, literal='EOF')
 
 
+👨‍💻 Development
+------------------
+
+For local development, you can install all dependencies by running:
+
+.. code-block:: bash
+
+   make install
+
+
+🧪 Testing
+------------------
+
+.. code-block:: bash
+
+   make test
+   # or
+   pytest -vv tests
+
+
+💡 Tips
+------------------
+
+To run a subset of tests:
+
+.. code-block:: bash
+
+   make test
+   make lint
+   make coverage
+
+
+🚀 Deploying
+------------------
+
+A reminder for maintainers on how to deploy. Run the following commands in order:
+
+.. code-block:: bash
+
+   bump2version patch # possible: major / minor / patch
+   git push
+   git push --tags
+   make dist
+   make release
+
+
 📝 License
 ----------
 
 Todo.
 
 .. _pyenv: https://github.com/pyenv/pyenv
 .. _poetry: https://github.com/python-poetry/poetry
```

### Comparing `deez_py-0.1.5/deez_py/deez_ast.py` & `deez_py-0.1.6/deez_py/deez_ast.py`

 * *Files identical despite different names*

### Comparing `deez_py-0.1.5/deez_py/lexer.py` & `deez_py-0.1.6/deez_py/lexer.py`

 * *Files identical despite different names*

### Comparing `deez_py-0.1.5/deez_py/parser.py` & `deez_py-0.1.6/deez_py/parser.py`

 * *Files identical despite different names*

### Comparing `deez_py-0.1.5/deez_py/tokens.py` & `deez_py-0.1.6/deez_py/tokens.py`

 * *Files identical despite different names*

### Comparing `deez_py-0.1.5/pyproject.toml` & `deez_py-0.1.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deez_py"
-version = "0.1.5"
+version = "0.1.6"
 description = "A Python implementation of a lexical analyzer that provides comprehensive scanning, and lookahead capabilities. It also implements a parser that comes with awesome functionalities."
 authors = [
     "Mahmoud Harmouch <business@wiseai.dev>",
     "BatikanHyt <batikanhyt@gmail.com>",
     "ThePrimeagen <the.primeagen@gmail.com>"
 ]
 license = "GNU General Public License v3.0"
```

### Comparing `deez_py-0.1.5/PKG-INFO` & `deez_py-0.1.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deez-py
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python implementation of a lexical analyzer that provides comprehensive scanning, and lookahead capabilities. It also implements a parser that comes with awesome functionalities.
 Home-page: https://github.com/ThePrimeagen/ts-rust-zig-deez
 License: GNU General Public License v3.0
 Keywords: python,deez_py,lexer
 Author: Mahmoud Harmouch
 Author-email: business@wiseai.dev
 Requires-Python: >=3.10,<4.0
@@ -26,15 +26,15 @@
    :target: https://github.com/ThePrimeagen/ts-rust-zig-deez_py/tree/master/python/LICENSE
    :alt: License
 
 .. image:: https://img.shields.io/pypi/v/deez_py.svg
    :target: https://pypi.org/project/deez_py/
    :alt: pypi version
 
-**deez_py** is python implementation of a lexical analyzer that provides comprehensive scanning, and lookahead capabilities. It also implements a parser that comes with awesome functionalities.
+**deez_py** is a python implementation of a lexical analyzer that provides comprehensive scanning, and lookahead capabilities. It also implements a parser that comes with awesome functionalities.
 
 🛠️ Requirements
 ---------------
 
 **deez_py** requires Python 3.10 or above.
 
 To install Python 3.10.1, we recommend using `pyenv`_.
@@ -56,15 +56,14 @@
    # or if you using the default bash shell, do this instead:
    cat << EOF >> ~/.bashrc
    # pyenv config
    export PATH="${HOME}/.pyenv/bin:${PATH}"
    export PYENV_ROOT="${HOME}/.pyenv"
    eval "$(pyenv init -)"
    EOF
-
    # Close and open a new shell session
    # install Python 3.10.1
    pyenv install 3.10.1
 
    # make it available globally
    pyenv global system 3.10.1
 
@@ -72,15 +71,15 @@
 To manage the Python 3.10.1 virtualenv, we recommend using `poetry`_.
 
 .. code-block:: bash
 
    # install poetry
    curl -sSL https://install.python-poetry.org | python3 -
    poetry --version
-   Poetry (version 1.5.1)
+   Poetry \(version 1.5.1\)
 
    # Having the python executable in your PATH, you can use it:
    poetry env use 3.10.1
 
    # However, you are most likely to get the following issue:
    Creating virtualenv deez_py-dxc671ba-py3.10 in ~/.cache/pypoetry/virtualenvs
 
@@ -114,26 +113,72 @@
 
 .. code-block:: python3
 
    >>> from deez_py import Lexer
    >>> lex = Lexer('=+(){},;')
    >>> for _ in range(9):
    >>>     print(lex.get_next_token())
-   ... 
+   ...
    Token(type=<TokenType.Equal: '='>, literal='=')
    Token(type=<TokenType.Plus: '+'>, literal='+')
    Token(type=<TokenType.LParen: '('>, literal='(')
    Token(type=<TokenType.RParen: ')'>, literal=')')
    Token(type=<TokenType.LSquirly: '{'>, literal='{')
    Token(type=<TokenType.RSquirly: '}'>, literal='}')
    Token(type=<TokenType.Comma: ','>, literal=',')
    Token(type=<TokenType.Semicolon: ';'>, literal=';')
    Token(type=<TokenType.Eof: 'EOF'>, literal='EOF')
 
 
+👨‍💻 Development
+------------------
+
+For local development, you can install all dependencies by running:
+
+.. code-block:: bash
+
+   make install
+
+
+🧪 Testing
+------------------
+
+.. code-block:: bash
+
+   make test
+   # or
+   pytest -vv tests
+
+
+💡 Tips
+------------------
+
+To run a subset of tests:
+
+.. code-block:: bash
+
+   make test
+   make lint
+   make coverage
+
+
+🚀 Deploying
+------------------
+
+A reminder for maintainers on how to deploy. Run the following commands in order:
+
+.. code-block:: bash
+
+   bump2version patch # possible: major / minor / patch
+   git push
+   git push --tags
+   make dist
+   make release
+
+
 📝 License
 ----------
 
 Todo.
 
 .. _pyenv: https://github.com/pyenv/pyenv
 .. _poetry: https://github.com/python-poetry/poetry
```

