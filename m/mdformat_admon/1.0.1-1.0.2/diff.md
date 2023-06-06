# Comparing `tmp/mdformat_admon-1.0.1.tar.gz` & `tmp/mdformat_admon-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdformat_admon-1.0.1.tar", last modified: Tue Feb  7 00:26:53 2023, max compression
+gzip compressed data, was "mdformat_admon-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mdformat_admon-1.0.1.tar` & `mdformat_admon-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1819 2023-02-07 00:26:49.238128 mdformat_admon-1.0.1/.gitignore
--rw-r--r--   0        0        0     1729 2023-02-07 00:26:49.238128 mdformat_admon-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      296 2023-02-07 00:26:49.238128 mdformat_admon-1.0.1/.pre-commit-test.yaml
--rw-r--r--   0        0        0       21 2023-02-07 00:26:49.238128 mdformat_admon-1.0.1/.tool-versions
--rw-r--r--   0        0        0      923 2023-02-07 00:26:49.238128 mdformat_admon-1.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1073 2023-02-07 00:26:49.238128 mdformat_admon-1.0.1/LICENSE
--rw-r--r--   0        0        0     2789 2023-02-07 00:26:49.238128 mdformat_admon-1.0.1/README.md
--rw-r--r--   0        0        0      123 2023-02-07 00:26:49.238128 mdformat_admon-1.0.1/mdformat_admon/__init__.py
--rw-r--r--   0        0        0     5122 2023-02-07 00:26:49.238128 mdformat_admon-1.0.1/mdformat_admon/index_pr58.py
--rw-r--r--   0        0        0     2193 2023-02-07 00:26:49.238128 mdformat_admon-1.0.1/mdformat_admon/plugin.py
--rw-r--r--   0        0        0     1314 2023-02-07 00:26:49.238128 mdformat_admon-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      678 2023-02-07 00:26:49.238128 mdformat_admon-1.0.1/tox.ini
--rw-r--r--   0        0        0     3579 1970-01-01 00:00:00.000000 mdformat_admon-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1819 2023-06-06 00:20:26.849021 mdformat_admon-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1729 2023-06-06 00:20:26.849021 mdformat_admon-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      296 2023-06-06 00:20:26.849021 mdformat_admon-1.0.2/.pre-commit-test.yaml
+-rw-r--r--   0        0        0       21 2023-06-06 00:20:26.849021 mdformat_admon-1.0.2/.tool-versions
+-rw-r--r--   0        0        0      923 2023-06-06 00:20:26.849021 mdformat_admon-1.0.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1073 2023-06-06 00:20:26.849021 mdformat_admon-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2789 2023-06-06 00:20:26.849021 mdformat_admon-1.0.2/README.md
+-rw-r--r--   0        0        0      123 2023-06-06 00:20:26.849021 mdformat_admon-1.0.2/mdformat_admon/__init__.py
+-rw-r--r--   0        0        0     2076 2023-06-06 00:20:26.849021 mdformat_admon-1.0.2/mdformat_admon/plugin.py
+-rw-r--r--   0        0        0     1314 2023-06-06 00:20:26.849021 mdformat_admon-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      678 2023-06-06 00:20:26.849021 mdformat_admon-1.0.2/tox.ini
+-rw-r--r--   0        0        0     3579 1970-01-01 00:00:00.000000 mdformat_admon-1.0.2/PKG-INFO
```

### Comparing `mdformat_admon-1.0.1/.gitignore` & `mdformat_admon-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mdformat_admon-1.0.1/.pre-commit-config.yaml` & `mdformat_admon-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mdformat_admon-1.0.1/CONTRIBUTING.md` & `mdformat_admon-1.0.2/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,36 +13,36 @@
 ```bash
 tox
 ```
 
 and with test coverage:
 
 ```bash
-tox -e py37-cov
+tox -e py38-cov
 ```
 
 The easiest way to write tests, is to edit `tests/fixtures.md`
 
 To run the code formatting and style checks:
 
 ```bash
-tox -e py37-pre-commit
+tox -e py38-pre-commit
 ```
 
 or directly
 
 ```bash
 pip install pre-commit
 pre-commit run --all
 ```
 
 To run the pre-commit hook test:
 
 ```bash
-tox -e py37-hook
+tox -e py38-hook
 ```
 
 ## Publish to PyPi
 
 Either use flit directly:
 
 ```bash
```

### Comparing `mdformat_admon-1.0.1/LICENSE` & `mdformat_admon-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mdformat_admon-1.0.1/README.md` & `mdformat_admon-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mdformat_admon-1.0.1/mdformat_admon/plugin.py` & `mdformat_admon-1.0.2/mdformat_admon/plugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 import textwrap
 from typing import Mapping
 
 from markdown_it import MarkdownIt
 from mdformat.renderer import RenderContext, RenderTreeNode
 from mdformat.renderer.typing import Render
-
-from .index_pr58 import admon_plugin
-
-# FIXME: Use latest mdit_py_pluign once my PR is merged
-#   https://github.com/executablebooks/mdit-py-plugins/pull/58/files
+from mdit_py_plugins.admon import admon_plugin
 
 
 def update_mdit(mdit: MarkdownIt) -> None:
     """Update the parser."""
     mdit.use(admon_plugin)
```

### Comparing `mdformat_admon-1.0.1/pyproject.toml` & `mdformat_admon-1.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 keywords = ["mdformat", "markdown", "markdown-it"]
-requires-python = ">=3.7.2"
+requires-python = ">=3.8.0"
 dependencies = [
     "mdformat >= 0.7.16",
-    "mdit-py-plugins >= 0.3.2",
+    "mdit-py-plugins >= 0.4.0",
 ]
 dynamic = ["version", "description"]
 
 [project.optional-dependencies]
 test = [
     "pytest >= 7.0",
     "pytest-cov",
```

### Comparing `mdformat_admon-1.0.1/tox.ini` & `mdformat_admon-1.0.2/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tox]
 envlist =
-    py{37,310}-cov
+    py{38,310}-cov
     py{310}-pre-commit
-    py{37,310}-hook
+    py{38,310}-hook
 isolated_build = True
 skip_missing_interpreters = False
 
-[testenv:py{37,310}]
+[testenv:py{38,310}]
 extras = test
 commands = pytest {posargs} --ff -vv
 
 [testenv:py{310}-cov]
 extras = test
 commands = pytest --cov={envsitepackagesdir}/mdformat_admon {posargs}
 
 [testenv:py{310}-pre-commit]
 extras = dev
 commands = pre-commit run {posargs:--all-files}
 
-[testenv:py{37,310}-hook]
+[testenv:py{38,310}-hook]
 extras = dev
 commands = pre-commit run --config .pre-commit-test.yaml {posargs:--all-files --verbose --show-diff-on-failure}
 
 [flake8]
 max-line-length = 88
 max-complexity = 10
 # These checks violate PEP8 so let's ignore them
```

### Comparing `mdformat_admon-1.0.1/PKG-INFO` & `mdformat_admon-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: mdformat_admon
-Version: 1.0.1
+Version: 1.0.2
 Summary: An mdformat plugin for admonitions.
 Keywords: mdformat,markdown,markdown-it
 Author-email: Kyle King <dev.act.kyle@gmail.com>
-Requires-Python: >=3.7.2
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: mdformat >= 0.7.16
-Requires-Dist: mdit-py-plugins >= 0.3.2
+Requires-Dist: mdit-py-plugins >= 0.4.0
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: pytest >= 7.0 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Project-URL: Homepage, https://github.com/KyleKing/mdformat-admon
 Provides-Extra: dev
 Provides-Extra: test
```

