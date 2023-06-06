# Comparing `tmp/deez_py-0.1.3.tar.gz` & `tmp/deez_py-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deez_py-0.1.3.tar", max compression
+gzip compressed data, was "deez_py-0.1.4.tar", max compression
```

## Comparing `deez_py-0.1.3.tar` & `deez_py-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     3139 2023-05-28 18:59:02.114372 deez_py-0.1.3/README.rst
--rw-r--r--   0        0        0      213 2023-05-28 18:41:58.282468 deez_py-0.1.3/deez_py/__init__.py
--rw-r--r--   0        0        0      154 2023-05-28 18:29:18.278283 deez_py-0.1.3/deez_py/__main__.py
--rw-r--r--   0        0        0     8141 2023-05-28 18:18:15.690579 deez_py-0.1.3/deez_py/lexer.py
--rw-r--r--   0        0        0      674 2023-05-28 17:56:42.794879 deez_py-0.1.3/deez_py/tokens.py
--rw-r--r--   0        0        0     1327 2023-05-28 18:41:41.202409 deez_py-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4013 1970-01-01 00:00:00.000000 deez_py-0.1.3/setup.py
--rw-r--r--   0        0        0     4173 1970-01-01 00:00:00.000000 deez_py-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3151 2023-06-06 11:46:24.355163 deez_py-0.1.4/README.rst
+-rw-r--r--   0        0        0      225 2023-06-06 11:26:08.254149 deez_py-0.1.4/deez_py/__init__.py
+-rw-r--r--   0        0        0      163 2023-06-06 11:13:48.158670 deez_py-0.1.4/deez_py/__main__.py
+-rw-r--r--   0        0        0     2444 2023-06-06 11:25:46.594323 deez_py-0.1.4/deez_py/deez_ast.py
+-rw-r--r--   0        0        0     9315 2023-06-06 11:35:43.905146 deez_py-0.1.4/deez_py/lexer.py
+-rw-r--r--   0        0        0    11558 2023-06-06 11:42:34.685333 deez_py-0.1.4/deez_py/parser.py
+-rw-r--r--   0        0        0      469 2023-06-06 10:15:33.712716 deez_py-0.1.4/deez_py/token_types.py
+-rw-r--r--   0        0        0     1650 2023-06-06 11:04:32.801328 deez_py-0.1.4/deez_py/tokens.py
+-rw-r--r--   0        0        0     1398 2023-06-06 11:16:43.429971 deez_py-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4065 1970-01-01 00:00:00.000000 deez_py-0.1.4/PKG-INFO
```

### Comparing `deez_py-0.1.3/README.rst` & `deez_py-0.1.4/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -11,17 +11,17 @@
    :alt: pypi version
 
 **deez_py** is a Python implementation of a lexical analyzer that provides comprehensive scanning, and lookahead capabilities.
 
 🛠️ Requirements
 ---------------
 
-**deez_py** requires Python 3.9 or above.
+**deez_py** requires Python 3.10 or above.
 
-To install Python 3.9, I recommend using `pyenv`_.
+To install Python 3.10.1, we recommend using `pyenv`_.
 
 .. code-block:: bash
 
    # install pyenv
    git clone https://github.com/pyenv/pyenv ~/.pyenv
 
    # setup pyenv (you should also put these three lines in .bashrc or similar)
@@ -37,49 +37,49 @@
    cat << EOF >> ~/.bashrc
    # pyenv config
    export PATH="${HOME}/.pyenv/bin:${PATH}"
    export PYENV_ROOT="${HOME}/.pyenv"
    eval "$(pyenv init -)"
    EOF
    # Close and open a new shell session
-   # install Python 3.9.10
-   pyenv install 3.9.10
+   # install Python 3.10.1
+   pyenv install 3.10.1
 
    # make it available globally
-   pyenv global system 3.9.10
+   pyenv global system 3.10.1
 
 
-To manage the Python 3.9 virtualenv, I recommend using `poetry`_.
+To manage the Python 3.10.1 virtualenv, we recommend using `poetry`_.
 
 .. code-block:: bash
 
    # install poetry
    curl -sSL https://install.python-poetry.org | python3 -
    poetry --version
-   Poetry version 1.1.13
+   Poetry (version 1.5.1)
 
    # Having the python executable in your PATH, you can use it:
-   poetry env use 3.9.10
+   poetry env use 3.10.1
 
    # However, you are most likely to get the following issue:
-   Creating virtualenv deez_py-dxc671ba-py3.9 in ~/.cache/pypoetry/virtualenvs
+   Creating virtualenv deez_py-dxc671ba-py3.10 in ~/.cache/pypoetry/virtualenvs
 
    ModuleNotFoundError
 
    No module named 'virtualenv.seed.via_app_data'
 
    at <frozen importlib._bootstrap>:973 in _find_and_load_unlocked
 
    # To resolve it, you need to reinstall virtualenv through pip
    sudo apt remove --purge python3-virtualenv virtualenv
    python3 -m pip install -U virtualenv
 
    # Now, you can just use the minor Python version in this case:
-   poetry env use 3.9.10
-   Using virtualenv: ~/.cache/pypoetry/virtualenvs/deez_py-dxc671ba-py3.9
+   poetry env use 3.10.1
+   Using virtualenv: ~/.cache/pypoetry/virtualenvs/deez_py-dxc671ba-py3.10
 
 
 🚨 Installation
 ---------------
 
 With :code:`pip`:
```

### Comparing `deez_py-0.1.3/deez_py/lexer.py` & `deez_py-0.1.4/deez_py/lexer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-from dataclasses import dataclass
-from typing import Dict
-
-from .tokens import Token, TokenType, char_to_token_type
-
-keywords: Dict[str, Token] = {
-    "fn": Token(TokenType.Function, "fn"),
-    "let": Token(TokenType.Let, "let"),
-}
+from dataclasses import (
+    dataclass,
+)
+
+import deez_py.token_types as TokenType
+
+from .tokens import (
+    FIXED_TOKENS,
+    RESERVED_KEYWORDS,
+    Token,
+)
 
 
 @dataclass
 class Lexer:
     """
     Lexer tokenizes an input string into a sequence of tokens.
 
@@ -27,24 +29,24 @@
         read_position (int): Current position for reading the next character.
         ch (str): The current character being processed.
 
     Examples:
         >>> lex = Lexer('=+(){},;')
         >>> for _ in range(9):
         >>>     print(lex.get_next_token())
-        ... 
-        Token(type=<TokenType.Equal: '='>, literal='=')
-        Token(type=<TokenType.Plus: '+'>, literal='+')
-        Token(type=<TokenType.LParen: '('>, literal='(')
-        Token(type=<TokenType.RParen: ')'>, literal=')')
-        Token(type=<TokenType.LSquirly: '{'>, literal='{')
-        Token(type=<TokenType.RSquirly: '}'>, literal='}')
-        Token(type=<TokenType.Comma: ','>, literal=',')
-        Token(type=<TokenType.Semicolon: ';'>, literal=';')
-        Token(type=<TokenType.Eof: 'EOF'>, literal='EOF')
+        ...
+        Token(type='=', literal='=')
+        Token(type='+', literal='+')
+        Token(type='(', literal='(')
+        Token(type=')', literal=')')
+        Token(type='{', literal='{')
+        Token(type='}', literal='}')
+        Token(type=',', literal=',')
+        Token(type=';', literal=';')
+        Token(type='EOF', literal='EOF')
     """
 
     input: str
     position: int = 0
     read_position: int = 0
     ch: str = ""
 
@@ -72,22 +74,47 @@
             >>> lex.read_char()
             >>> lex.ch
             'b'
             >>> lex.read_char()
             >>> lex.ch
             'c'
         """
-        if self.read_position >= self.input_length:
-            self.ch = "\0"
-        else:
-            self.ch = self.input[self.read_position]
-
+        self.ch = self.peek_char()
         self.position = self.read_position
         self.read_position += 1
 
+    def peek_char(self) -> str:
+        """
+        Returns the next character in the input string without advancing the lexer's position.
+
+        If the lexer's read position (`self.read_position`) is greater than or equal to the length
+        of the input string, the null character ("\0") is returned. Otherwise, the character at the
+        current read position is returned.
+
+        Returns:
+            str: The next character in the input string.
+
+        Examples:
+            >>> lex = Lexer("abc")
+            >>> lex.peek_char()
+            'a'
+            >>> lex.read_position = 1
+            >>> lex.peek_char()
+            'b'
+            >>> lex.read_position = 2
+            >>> lex.peek_char()
+            'c'
+            >>> lex.read_position = 3
+            >>> lex.peek_char()
+            '\\0'
+        """
+        if self.read_position >= self.input_length:
+            return "\0"
+        return self.input[self.read_position]
+
     def reset(self) -> None:
         """Resets the lexer's position to the beginning.
 
         This method resets the lexer's position to the beginning of the input string by setting both the
         current position (`self.position`) and the position for the next character (`self.read_position`) to 0.
         After resetting the position, the current character (`self.ch`) is updated to the first character in
         the input string.
@@ -152,15 +179,17 @@
             >>> lexer.position
             7
             >>> lexer.read_position
             8
             >>> lexer.ch
             '4'
         """
-        while self.ch != "\x00" and self.get_next_token().type not in token_names:
+        while (
+            self.ch != "\x00" and self.get_next_token().type not in token_names
+        ):
             ...
 
     def get_next_token(self) -> Token:
         """
         Get the next token from the input string.
 
         Returns:
@@ -169,28 +198,41 @@
         Examples:
             >>> lex = Lexer('=+(){},;')
             >>> lex.get_next_token()
             Token(type=<TokenType.Equal: '='>, literal='=')
         """
         self.skip_whitespace()
 
-        tok_type = char_to_token_type.get(self.ch, None)
-        if tok_type is not None:
-            tok = Token(tok_type, tok_type.value)
-            self.read_char()
-            return tok
-
-        if self.is_letter(self.ch):
-            indent = self.read_ident()
-            return keywords.get(indent, Token(TokenType.Ident, indent))
-
-        if self.ch.isdigit():
-            return Token(TokenType.Int, self.read_int())
+        # I dont wanna write if else for each character
+        tok = None
+        if self.ch in FIXED_TOKENS:
+            tok = FIXED_TOKENS[self.ch]
+        match tok:
+            case Token(TokenType.ASSING):
+                # PEEK
+                if self.peek_char() == "=":
+                    self.read_char()
+                    tok = FIXED_TOKENS["=="]
+            case Token(TokenType.BANG):
+                # PEEK
+                if self.peek_char() == "=":
+                    self.read_char()
+                    tok = FIXED_TOKENS["!="]
+            case None:
+                if self.is_letter(self.ch):
+                    ident = self.read_ident()
+                    if ident in RESERVED_KEYWORDS:
+                        return RESERVED_KEYWORDS[ident]
+                    return Token(TokenType.IDENT, ident)
+                elif self.ch.isdigit():
+                    return Token(TokenType.INT, self.read_int())
+                tok = Token(TokenType.ILLEGAL, TokenType.ILLEGAL)
 
-        return Token(TokenType.Illegal, self.ch)
+        self.read_char()
+        return tok
 
     def read_int(self) -> str:
         """
         Read an integer from the input string.
 
         Returns:
             str: The integer as a string.
@@ -258,10 +300,9 @@
             >>> Lexer.is_letter('7')
             False
             >>> Lexer.is_letter('_')
             True
         """
         return ch.isalpha() or ch == "_"
 
-__all__ = [
-    "Lexer"
-]
+
+__all__ = ["Lexer"]
```

### Comparing `deez_py-0.1.3/pyproject.toml` & `deez_py-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "deez_py"
-version = "0.1.3"
-description = "A Python implementation of a lexical analyzer that provides comprehensive scanning, and lookahead capabilities."
+version = "0.1.4"
+description = "A Python implementation of a lexical analyzer that provides comprehensive scanning, and lookahead capabilities. It also implements a parser that comes with a lot of awesome functionalities."
 authors = [
     "Mahmoud Harmouch <business@wiseai.dev>",
     "BatikanHyt <batikanhyt@gmail.com>",
     "ThePrimeagen <the.primeagen@gmail.com>"
 ]
 license = "GNU General Public License v3.0"
 readme = "README.rst"
@@ -13,38 +13,40 @@
 homepage = "https://github.com/ThePrimeagen/ts-rust-zig-deez"
 documentation = ""
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 keywords = ["python", "deez_py", "lexer"]
 packages = [
     { include = "deez_py", from = "." },
 ]
 include = [
     "LICENSE",
     "README.rst",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 
-[tool.poetry.dev-dependencies]
-pytest = "^5.2"
-flake8 = "^4.0.1"
-coverage = "^6.3.2"
-rstcheck = "^3.3.1"
-mypy = "^0.941"
-pytest-cov = "^3.0.0"
-tox = "^3.24.5"
-isort = "^5.10.1"
-black = "^22.1.0"
-pre-commit = "^2.17.0"
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.3.1"
+flake8 = "^6.0.0"
+coverage = "^7.2.7"
+rstcheck = "^6.1.2"
+mypy = "^1.3.0"
+pytest-cov = "^4.1.0"
+tox = "^4.6.0"
+isort = "^5.12.0"
+black = "^23.3.0"
+pre-commit = "^3.3.2"
 bump2version = "^1.0.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.black]
+line-length = 79
```

### Comparing `deez_py-0.1.3/PKG-INFO` & `deez_py-0.1.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 Metadata-Version: 2.1
 Name: deez-py
-Version: 0.1.3
-Summary: A Python implementation of a lexical analyzer that provides comprehensive scanning, and lookahead capabilities.
+Version: 0.1.4
+Summary: A Python implementation of a lexical analyzer that provides comprehensive scanning, and lookahead capabilities. It also implements a parser that comes with a lot of awesome functionalities.
 Home-page: https://github.com/ThePrimeagen/ts-rust-zig-deez
 License: GNU General Public License v3.0
 Keywords: python,deez_py,lexer
 Author: Mahmoud Harmouch
 Author-email: business@wiseai.dev
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
 Project-URL: Repository, https://github.com/ThePrimeagen/ts-rust-zig-deez
 Description-Content-Type: text/x-rst
 
 =========
 deez_py
 =========
 
@@ -35,17 +31,17 @@
    :alt: pypi version
 
 **deez_py** is a Python implementation of a lexical analyzer that provides comprehensive scanning, and lookahead capabilities.
 
 🛠️ Requirements
 ---------------
 
-**deez_py** requires Python 3.9 or above.
+**deez_py** requires Python 3.10 or above.
 
-To install Python 3.9, I recommend using `pyenv`_.
+To install Python 3.10.1, we recommend using `pyenv`_.
 
 .. code-block:: bash
 
    # install pyenv
    git clone https://github.com/pyenv/pyenv ~/.pyenv
 
    # setup pyenv (you should also put these three lines in .bashrc or similar)
@@ -61,49 +57,49 @@
    cat << EOF >> ~/.bashrc
    # pyenv config
    export PATH="${HOME}/.pyenv/bin:${PATH}"
    export PYENV_ROOT="${HOME}/.pyenv"
    eval "$(pyenv init -)"
    EOF
    # Close and open a new shell session
-   # install Python 3.9.10
-   pyenv install 3.9.10
+   # install Python 3.10.1
+   pyenv install 3.10.1
 
    # make it available globally
-   pyenv global system 3.9.10
+   pyenv global system 3.10.1
 
 
-To manage the Python 3.9 virtualenv, I recommend using `poetry`_.
+To manage the Python 3.10.1 virtualenv, we recommend using `poetry`_.
 
 .. code-block:: bash
 
    # install poetry
    curl -sSL https://install.python-poetry.org | python3 -
    poetry --version
-   Poetry version 1.1.13
+   Poetry (version 1.5.1)
 
    # Having the python executable in your PATH, you can use it:
-   poetry env use 3.9.10
+   poetry env use 3.10.1
 
    # However, you are most likely to get the following issue:
-   Creating virtualenv deez_py-dxc671ba-py3.9 in ~/.cache/pypoetry/virtualenvs
+   Creating virtualenv deez_py-dxc671ba-py3.10 in ~/.cache/pypoetry/virtualenvs
 
    ModuleNotFoundError
 
    No module named 'virtualenv.seed.via_app_data'
 
    at <frozen importlib._bootstrap>:973 in _find_and_load_unlocked
 
    # To resolve it, you need to reinstall virtualenv through pip
    sudo apt remove --purge python3-virtualenv virtualenv
    python3 -m pip install -U virtualenv
 
    # Now, you can just use the minor Python version in this case:
-   poetry env use 3.9.10
-   Using virtualenv: ~/.cache/pypoetry/virtualenvs/deez_py-dxc671ba-py3.9
+   poetry env use 3.10.1
+   Using virtualenv: ~/.cache/pypoetry/virtualenvs/deez_py-dxc671ba-py3.10
 
 
 🚨 Installation
 ---------------
 
 With :code:`pip`:
```

