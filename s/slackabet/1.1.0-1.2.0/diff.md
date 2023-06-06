# Comparing `tmp/slackabet-1.1.0.tar.gz` & `tmp/slackabet-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, last modified: Tue Jun  6 16:06:00 2023, max compression
```

## Comparing `slackabet-1.1.0.tar` & `slackabet-1.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 slackabet-1.1.0/.coveragerc
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 slackabet-1.1.0/.editorconfig
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 slackabet-1.1.0/.flake8
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 slackabet-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 slackabet-1.1.0/RELEASING.md
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 slackabet-1.1.0/codecov.yml
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 slackabet-1.1.0/tox.ini
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 slackabet-1.1.0/.github/labels.yml
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 slackabet-1.1.0/.github/release-drafter.yml
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 slackabet-1.1.0/.github/workflows/deploy.yml
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 slackabet-1.1.0/.github/workflows/labels.yml
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 slackabet-1.1.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 slackabet-1.1.0/.github/workflows/release-drafter.yml
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 slackabet-1.1.0/.github/workflows/require-pr-label.yml
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 slackabet-1.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 slackabet-1.1.0/src/slackabet/__init__.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 slackabet-1.1.0/src/slackabet/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 slackabet-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 slackabet-1.1.0/tests/test_slackabet.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 slackabet-1.1.0/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 slackabet-1.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 slackabet-1.1.0/README.md
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 slackabet-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 slackabet-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      303 2023-06-06 16:06:00.000000 slackabet-1.2.0/.coveragerc
+-rw-r--r--   0        0        0      313 2023-06-06 16:06:00.000000 slackabet-1.2.0/.editorconfig
+-rw-r--r--   0        0        0       30 2023-06-06 16:06:00.000000 slackabet-1.2.0/.flake8
+-rw-r--r--   0        0        0     1883 2023-06-06 16:06:00.000000 slackabet-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      829 2023-06-06 16:06:00.000000 slackabet-1.2.0/RELEASING.md
+-rw-r--r--   0        0        0       35 2023-06-06 16:06:00.000000 slackabet-1.2.0/codecov.yml
+-rw-r--r--   0        0        0      500 2023-06-06 16:06:00.000000 slackabet-1.2.0/tox.ini
+-rw-r--r--   0        0        0     1785 2023-06-06 16:06:00.000000 slackabet-1.2.0/.github/labels.yml
+-rw-r--r--   0        0        0      900 2023-06-06 16:06:00.000000 slackabet-1.2.0/.github/release-drafter.yml
+-rw-r--r--   0        0        0     1755 2023-06-06 16:06:00.000000 slackabet-1.2.0/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      352 2023-06-06 16:06:00.000000 slackabet-1.2.0/.github/workflows/labels.yml
+-rw-r--r--   0        0        0      298 2023-06-06 16:06:00.000000 slackabet-1.2.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1084 2023-06-06 16:06:00.000000 slackabet-1.2.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0        0        0      490 2023-06-06 16:06:00.000000 slackabet-1.2.0/.github/workflows/require-pr-label.yml
+-rw-r--r--   0        0        0     1187 2023-06-06 16:06:00.000000 slackabet-1.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1060 2023-06-06 16:06:00.000000 slackabet-1.2.0/src/slackabet/__init__.py
+-rw-r--r--   0        0        0     1408 2023-06-06 16:06:00.000000 slackabet-1.2.0/src/slackabet/cli.py
+-rw-r--r--   0        0        0        0 2023-06-06 16:06:00.000000 slackabet-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1320 2023-06-06 16:06:00.000000 slackabet-1.2.0/tests/test_slackabet.py
+-rw-r--r--   0        0        0      799 2023-06-06 16:06:00.000000 slackabet-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1079 2023-06-06 16:06:00.000000 slackabet-1.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     1865 2023-06-06 16:06:00.000000 slackabet-1.2.0/README.md
+-rw-r--r--   0        0        0     1600 2023-06-06 16:06:00.000000 slackabet-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3249 2023-06-06 16:06:00.000000 slackabet-1.2.0/PKG-INFO
```

### Comparing `slackabet-1.1.0/.pre-commit-config.yaml` & `slackabet-1.2.0/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,79 +1,78 @@
 repos:
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.2.2
+    rev: v3.4.0
     hooks:
       - id: pyupgrade
-        args: [--py37-plus]
+        args: [--py38-plus]
 
   - repo: https://github.com/psf/black
-    rev: 22.10.0
+    rev: 23.3.0
     hooks:
       - id: black
-        args: [--target-version=py37]
 
   - repo: https://github.com/asottile/blacken-docs
-    rev: v1.12.1
+    rev: 1.13.0
     hooks:
       - id: blacken-docs
-        args: [--target-version=py37]
-        additional_dependencies: [black==22.10.0]
+        additional_dependencies: [black==23.3.0]
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
         args: [--add-import=from __future__ import annotations]
 
   - repo: https://github.com/PyCQA/flake8
-    rev: 5.0.4
+    rev: 6.0.0
     hooks:
       - id: flake8
-        additional_dependencies: [flake8-2020, flake8-implicit-str-concat]
+        additional_dependencies:
+          [flake8-2020, flake8-errmsg, flake8-implicit-str-concat]
 
   - repo: https://github.com/pre-commit/pygrep-hooks
-    rev: v1.9.0
+    rev: v1.10.0
     hooks:
       - id: python-check-blanket-noqa
       - id: python-no-log-warn
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
-      - id: check-json
+      - id: check-case-conflict
       - id: check-merge-conflict
+      - id: check-json
       - id: check-toml
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.991
+    rev: v1.3.0
     hooks:
       - id: mypy
-        additional_dependencies: [pytest==7.2.0]
+        additional_dependencies: [pytest==7.3.1]
         args: [--strict, --pretty, --show-error-codes]
 
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: 0.3.5
+    rev: 0.10.0
     hooks:
       - id: pyproject-fmt
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.10.1
+    rev: v0.13
     hooks:
       - id: validate-pyproject
 
-  # Skip whilst it strips comments
-  #  - repo: https://github.com/tox-dev/tox-ini-fmt
-  #    rev: 0.5.0
-  #    hooks:
-  #      - id: tox-ini-fmt
+  - repo: https://github.com/tox-dev/tox-ini-fmt
+    rev: 1.3.0
+    hooks:
+      - id: tox-ini-fmt
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.0-alpha.4
+    rev: v3.0.0-alpha.9-for-vscode
     hooks:
       - id: prettier
         args: [--prose-wrap=always, --print-width=88]
 
 ci:
   autoupdate_schedule: quarterly
```

### Comparing `slackabet-1.1.0/RELEASING.md` & `slackabet-1.2.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `slackabet-1.1.0/.github/labels.yml` & `slackabet-1.2.0/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `slackabet-1.1.0/.github/release-drafter.yml` & `slackabet-1.2.0/.github/release-drafter.yml`

 * *Files 20% similar despite different names*

```diff
@@ -18,14 +18,19 @@
       - "bug"
   - title: "Security"
     label: "changelog: Security"
 
 exclude-labels:
   - "changelog: skip"
 
+autolabeler:
+  - label: "changelog: skip"
+    branch:
+      - "/pre-commit-ci-update-config/"
+
 template: |
   $CHANGES
 
 version-resolver:
   major:
     labels:
       - "changelog: Removed"
```

### Comparing `slackabet-1.1.0/.github/workflows/test.yml` & `slackabet-1.2.0/.github/workflows/test.yml`

 * *Files 8% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["pypy3.8", "3.7", "3.8", "3.9", "3.10", "3.11", "3.12-dev"]
+        python-version: ["pypy3.9", "3.8", "3.9", "3.10", "3.11", "3.12"]
         os: [windows-latest, macos-latest, ubuntu-latest]
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
+          allow-prereleases: true
           cache: pip
           cache-dependency-path: pyproject.toml
 
       - name: Install dependencies
         run: |
           python -m pip install -U pip
           python -m pip install -U wheel
```

### Comparing `slackabet-1.1.0/src/slackabet/__init__.py` & `slackabet-1.2.0/src/slackabet/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,33 @@
 from __future__ import annotations
 
+import importlib.metadata
 import random
 
-try:
-    # Python 3.8+
-    import importlib.metadata as importlib_metadata
-except ImportError:
-    # Python 3.7 and lower
-    import importlib_metadata  # type: ignore
-
-__version__: str = importlib_metadata.version(__name__)
+__version__: str = importlib.metadata.version(__name__)
 
 
 COLOURS = ["white", "yellow"]
 
 
 def slackabet(text: str, colour: str = "white") -> str:
     """Convert your text into alphabet emoji"""
 
     if colour == "words":
         words = text.split()
         converted = []
         for i, word in enumerate(words):
-            if i % 2 == 0:
-                colour = "white"
-            else:
-                colour = "yellow"
             colour = "white" if i % 2 == 0 else "yellow"
 
             converted.append(slackabet(word, colour))
         return " ".join(converted)
 
     new = ""
     prefix = f"alphabet-{colour}"
     for c in text:
-
         if colour == "random":
             prefix = f"alphabet-{random.choice(COLOURS)}"
 
         if c.isalpha():
             new += f":{prefix}-{c}:"
         elif c == "@":
             new += f":{prefix}-at:"
```

### Comparing `slackabet-1.1.0/src/slackabet/cli.py` & `slackabet-1.2.0/src/slackabet/cli.py`

 * *Files identical despite different names*

### Comparing `slackabet-1.1.0/tests/test_slackabet.py` & `slackabet-1.2.0/tests/test_slackabet.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import pytest
-from hypothesis_auto import auto_pytest_magic  # type: ignore[import]
 
 import slackabet
 
 
 def test_slackabet_default() -> None:
     # Act
     text = slackabet.slackabet("123ABCabc@!#?")
@@ -52,10 +51,7 @@
 
     # Assert
     words = text.split()
     assert "alphabet-white-" in words[0]
     assert "alphabet-yellow-" in words[1]
     assert "alphabet-yellow-" not in words[0]
     assert "alphabet-white-" not in words[1]
-
-
-auto_pytest_magic(slackabet.slackabet)
```

### Comparing `slackabet-1.1.0/.gitignore` & `slackabet-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `slackabet-1.1.0/LICENSE.txt` & `slackabet-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `slackabet-1.1.0/README.md` & `slackabet-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `slackabet-1.1.0/pyproject.toml` & `slackabet-1.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -16,59 +16,51 @@
   "converter",
   "emoji",
   "Slack",
   "text",
 ]
 license = {text = "MIT"}
 authors = [{name = "Hugo van Kemenade"}]
-requires-python = ">=3.7"
-dependencies = [
-  'importlib-metadata; python_version < "3.8"',
-  'pyperclip; platform_system != "Linux"',
+requires-python = ">=3.8"
+classifiers = [
+  "Development Status :: 4 - Beta",
+  "Intended Audience :: Developers",
+  "License :: OSI Approved :: MIT License",
+  "Natural Language :: English",
+  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
+  "Programming Language :: Python :: Implementation :: CPython",
+  "Programming Language :: Python :: Implementation :: PyPy",
+  "Topic :: Artistic Software",
+  "Topic :: Text Processing",
 ]
 dynamic = [
   "version",
 ]
-classifiers = [
-    "Development Status :: 4 - Beta",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Natural Language :: English",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: Implementation :: CPython",
-    "Programming Language :: Python :: Implementation :: PyPy",
-    "Topic :: Artistic Software",
-    "Topic :: Text Processing",
+dependencies = [
+  'pyperclip; platform_system != "Linux"',
 ]
 [project.optional-dependencies]
 tests = [
-  "hypothesis-auto",
   "pytest",
   "pytest-cov",
 ]
-
 [project.urls]
 Changelog = "https://github.com/hugovk/slackabet/releases"
 Homepage = "https://github.com/hugovk/slackabet"
 Source = "https://github.com/hugovk/slackabet"
-
 [project.scripts]
 sb = "slackabet.cli:main"
 slackabet = "slackabet.cli:main"
 
-
-[tool.black]
-target_version = ["py37"]
-
 [tool.hatch]
 version.source = "vcs"
 
 [tool.hatch.version.raw-options]
 local_scheme = "no-local-version"
 
 [tool.isort]
```

### Comparing `slackabet-1.1.0/PKG-INFO` & `slackabet-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 Metadata-Version: 2.1
 Name: slackabet
-Version: 1.1.0
+Version: 1.2.0
 Summary: Convert text into Slack alphabet emoji
 Project-URL: Changelog, https://github.com/hugovk/slackabet/releases
 Project-URL: Homepage, https://github.com/hugovk/slackabet
 Project-URL: Source, https://github.com/hugovk/slackabet
 Author: Hugo van Kemenade
 License: MIT
 License-File: LICENSE.txt
 Keywords: CLI,Slack,alphabet,convert,converter,emoji,text
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Artistic Software
 Classifier: Topic :: Text Processing
-Requires-Python: >=3.7
-Requires-Dist: importlib-metadata; python_version < '3.8'
+Requires-Python: >=3.8
 Requires-Dist: pyperclip; platform_system != 'Linux'
 Provides-Extra: tests
-Requires-Dist: hypothesis-auto; extra == 'tests'
 Requires-Dist: pytest; extra == 'tests'
 Requires-Dist: pytest-cov; extra == 'tests'
 Description-Content-Type: text/markdown
 
 # slackabet
 
 [![PyPI version](https://img.shields.io/pypi/v/slackabet.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/slackabet)
```

