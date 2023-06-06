# Comparing `tmp/deez_py-0.1.4.tar.gz` & `tmp/deez_py-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deez_py-0.1.4.tar", max compression
+gzip compressed data, was "deez_py-0.1.5.tar", max compression
```

## Comparing `deez_py-0.1.4.tar` & `deez_py-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3151 2023-06-06 11:46:24.355163 deez_py-0.1.4/README.rst
--rw-r--r--   0        0        0      225 2023-06-06 11:26:08.254149 deez_py-0.1.4/deez_py/__init__.py
--rw-r--r--   0        0        0      163 2023-06-06 11:13:48.158670 deez_py-0.1.4/deez_py/__main__.py
--rw-r--r--   0        0        0     2444 2023-06-06 11:25:46.594323 deez_py-0.1.4/deez_py/deez_ast.py
--rw-r--r--   0        0        0     9315 2023-06-06 11:35:43.905146 deez_py-0.1.4/deez_py/lexer.py
--rw-r--r--   0        0        0    11558 2023-06-06 11:42:34.685333 deez_py-0.1.4/deez_py/parser.py
--rw-r--r--   0        0        0      469 2023-06-06 10:15:33.712716 deez_py-0.1.4/deez_py/token_types.py
--rw-r--r--   0        0        0     1650 2023-06-06 11:04:32.801328 deez_py-0.1.4/deez_py/tokens.py
--rw-r--r--   0        0        0     1398 2023-06-06 11:16:43.429971 deez_py-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4065 1970-01-01 00:00:00.000000 deez_py-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3219 2023-06-06 12:01:30.162499 deez_py-0.1.5/README.rst
+-rw-r--r--   0        0        0      225 2023-06-06 12:01:40.898396 deez_py-0.1.5/deez_py/__init__.py
+-rw-r--r--   0        0        0      163 2023-06-06 11:13:48.158670 deez_py-0.1.5/deez_py/__main__.py
+-rw-r--r--   0        0        0     2444 2023-06-06 11:25:46.594323 deez_py-0.1.5/deez_py/deez_ast.py
+-rw-r--r--   0        0        0     9315 2023-06-06 11:35:43.905146 deez_py-0.1.5/deez_py/lexer.py
+-rw-r--r--   0        0        0    11558 2023-06-06 11:56:51.589174 deez_py-0.1.5/deez_py/parser.py
+-rw-r--r--   0        0        0      469 2023-06-06 10:15:33.712716 deez_py-0.1.5/deez_py/token_types.py
+-rw-r--r--   0        0        0     1650 2023-06-06 11:04:32.801328 deez_py-0.1.5/deez_py/tokens.py
+-rw-r--r--   0        0        0     1389 2023-06-06 12:01:55.880757 deez_py-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4124 1970-01-01 00:00:00.000000 deez_py-0.1.5/PKG-INFO
```

### Comparing `deez_py-0.1.4/README.rst` & `deez_py-0.1.5/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
    :target: https://github.com/ThePrimeagen/ts-rust-zig-deez_py/tree/master/python/LICENSE
    :alt: License
 
 .. image:: https://img.shields.io/pypi/v/deez_py.svg
    :target: https://pypi.org/project/deez_py/
    :alt: pypi version
 
-**deez_py** is a Python implementation of a lexical analyzer that provides comprehensive scanning, and lookahead capabilities.
+**deez_py** is python implementation of a lexical analyzer that provides comprehensive scanning, and lookahead capabilities. It also implements a parser that comes with awesome functionalities.
 
 🛠️ Requirements
 ---------------
 
 **deez_py** requires Python 3.10 or above.
 
 To install Python 3.10.1, we recommend using `pyenv`_.
@@ -36,14 +36,15 @@
    # or if you using the default bash shell, do this instead:
    cat << EOF >> ~/.bashrc
    # pyenv config
    export PATH="${HOME}/.pyenv/bin:${PATH}"
    export PYENV_ROOT="${HOME}/.pyenv"
    eval "$(pyenv init -)"
    EOF
+
    # Close and open a new shell session
    # install Python 3.10.1
    pyenv install 3.10.1
 
    # make it available globally
    pyenv global system 3.10.1
```

### Comparing `deez_py-0.1.4/deez_py/deez_ast.py` & `deez_py-0.1.5/deez_py/deez_ast.py`

 * *Files identical despite different names*

### Comparing `deez_py-0.1.4/deez_py/lexer.py` & `deez_py-0.1.5/deez_py/lexer.py`

 * *Files identical despite different names*

### Comparing `deez_py-0.1.4/deez_py/parser.py` & `deez_py-0.1.5/deez_py/parser.py`

 * *Files identical despite different names*

### Comparing `deez_py-0.1.4/deez_py/tokens.py` & `deez_py-0.1.5/deez_py/tokens.py`

 * *Files identical despite different names*

### Comparing `deez_py-0.1.4/pyproject.toml` & `deez_py-0.1.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "deez_py"
-version = "0.1.4"
-description = "A Python implementation of a lexical analyzer that provides comprehensive scanning, and lookahead capabilities. It also implements a parser that comes with a lot of awesome functionalities."
+version = "0.1.5"
+description = "A Python implementation of a lexical analyzer that provides comprehensive scanning, and lookahead capabilities. It also implements a parser that comes with awesome functionalities."
 authors = [
     "Mahmoud Harmouch <business@wiseai.dev>",
     "BatikanHyt <batikanhyt@gmail.com>",
     "ThePrimeagen <the.primeagen@gmail.com>"
 ]
 license = "GNU General Public License v3.0"
 readme = "README.rst"
```

### Comparing `deez_py-0.1.4/PKG-INFO` & `deez_py-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: deez-py
-Version: 0.1.4
-Summary: A Python implementation of a lexical analyzer that provides comprehensive scanning, and lookahead capabilities. It also implements a parser that comes with a lot of awesome functionalities.
+Version: 0.1.5
+Summary: A Python implementation of a lexical analyzer that provides comprehensive scanning, and lookahead capabilities. It also implements a parser that comes with awesome functionalities.
 Home-page: https://github.com/ThePrimeagen/ts-rust-zig-deez
 License: GNU General Public License v3.0
 Keywords: python,deez_py,lexer
 Author: Mahmoud Harmouch
 Author-email: business@wiseai.dev
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -26,15 +26,15 @@
    :target: https://github.com/ThePrimeagen/ts-rust-zig-deez_py/tree/master/python/LICENSE
    :alt: License
 
 .. image:: https://img.shields.io/pypi/v/deez_py.svg
    :target: https://pypi.org/project/deez_py/
    :alt: pypi version
 
-**deez_py** is a Python implementation of a lexical analyzer that provides comprehensive scanning, and lookahead capabilities.
+**deez_py** is python implementation of a lexical analyzer that provides comprehensive scanning, and lookahead capabilities. It also implements a parser that comes with awesome functionalities.
 
 🛠️ Requirements
 ---------------
 
 **deez_py** requires Python 3.10 or above.
 
 To install Python 3.10.1, we recommend using `pyenv`_.
@@ -56,14 +56,15 @@
    # or if you using the default bash shell, do this instead:
    cat << EOF >> ~/.bashrc
    # pyenv config
    export PATH="${HOME}/.pyenv/bin:${PATH}"
    export PYENV_ROOT="${HOME}/.pyenv"
    eval "$(pyenv init -)"
    EOF
+
    # Close and open a new shell session
    # install Python 3.10.1
    pyenv install 3.10.1
 
    # make it available globally
    pyenv global system 3.10.1
```

