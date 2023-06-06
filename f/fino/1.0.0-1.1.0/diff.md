# Comparing `tmp/fino-1.0.0.tar.gz` & `tmp/fino-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, last modified: Tue Jun  6 15:43:47 2023, max compression
```

## Comparing `fino-1.0.0.tar` & `fino-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 fino-1.0.0/.coveragerc
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 fino-1.0.0/.editorconfig
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 fino-1.0.0/.flake8
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 fino-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 fino-1.0.0/RELEASING.md
--rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 fino-1.0.0/fino.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 fino-1.0.0/fino_guess.py
--rw-r--r--   0        0        0     8093 2020-02-02 00:00:00.000000 fino-1.0.0/test_fino.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 fino-1.0.0/tox.ini
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 fino-1.0.0/.github/labels.yml
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 fino-1.0.0/.github/release-drafter.yml
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 fino-1.0.0/.github/workflows/deploy.yml
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fino-1.0.0/.github/workflows/labels.yml
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 fino-1.0.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 fino-1.0.0/.github/workflows/release-drafter.yml
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 fino-1.0.0/.github/workflows/require-pr-label.yml
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 fino-1.0.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 fino-1.0.0/.gitignore
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 fino-1.0.0/README.md
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 fino-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 fino-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      346 2023-06-06 15:43:47.000000 fino-1.1.0/.coveragerc
+-rw-r--r--   0        0        0      313 2023-06-06 15:43:47.000000 fino-1.1.0/.editorconfig
+-rw-r--r--   0        0        0       44 2023-06-06 15:43:47.000000 fino-1.1.0/.flake8
+-rw-r--r--   0        0        0     1730 2023-06-06 15:43:47.000000 fino-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      818 2023-06-06 15:43:47.000000 fino-1.1.0/RELEASING.md
+-rw-r--r--   0        0        0     3692 2023-06-06 15:43:47.000000 fino-1.1.0/fino.py
+-rw-r--r--   0        0        0     1021 2023-06-06 15:43:47.000000 fino-1.1.0/fino_guess.py
+-rw-r--r--   0        0        0     3251 2023-06-06 15:43:47.000000 fino-1.1.0/test_fino.py
+-rw-r--r--   0        0        0      233 2023-06-06 15:43:47.000000 fino-1.1.0/tox.ini
+-rw-r--r--   0        0        0     1785 2023-06-06 15:43:47.000000 fino-1.1.0/.github/labels.yml
+-rw-r--r--   0        0        0      900 2023-06-06 15:43:47.000000 fino-1.1.0/.github/release-drafter.yml
+-rw-r--r--   0        0        0     1755 2023-06-06 15:43:47.000000 fino-1.1.0/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      352 2023-06-06 15:43:47.000000 fino-1.1.0/.github/workflows/labels.yml
+-rw-r--r--   0        0        0      298 2023-06-06 15:43:47.000000 fino-1.1.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1084 2023-06-06 15:43:47.000000 fino-1.1.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0        0        0      490 2023-06-06 15:43:47.000000 fino-1.1.0/.github/workflows/require-pr-label.yml
+-rw-r--r--   0        0        0     1187 2023-06-06 15:43:47.000000 fino-1.1.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      743 2023-06-06 15:43:47.000000 fino-1.1.0/.gitignore
+-rw-r--r--   0        0        0     2312 2023-06-06 15:43:47.000000 fino-1.1.0/README.md
+-rw-r--r--   0        0        0     1493 2023-06-06 15:43:47.000000 fino-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3690 2023-06-06 15:43:47.000000 fino-1.1.0/PKG-INFO
```

### Comparing `fino-1.0.0/.pre-commit-config.yaml` & `fino-1.1.0/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,69 +1,72 @@
 repos:
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.4.0
     hooks:
       - id: pyupgrade
-        args: [--py37-plus]
+        args: [--py38-plus]
 
   - repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black
-        args: [--target-version=py37]
 
   - repo: https://github.com/PyCQA/isort
-    rev: v5.11.3
+    rev: 5.12.0
     hooks:
       - id: isort
         args: [--add-import=from __future__ import annotations]
 
   - repo: https://github.com/PyCQA/flake8
     rev: 6.0.0
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
     rev: v4.4.0
     hooks:
+      - id: check-case-conflict
       - id: check-merge-conflict
+      - id: check-json
       - id: check-toml
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
-  #- repo: https://github.com/pre-commit/mirrors-mypy
-  #  rev: v0.991
-  #  hooks:
-  #    - id: mypy
-  #      args: [--strict, --pretty, --show-error-codes]
+  - repo: https://github.com/pre-commit/mirrors-mypy
+    rev: v1.3.0
+    hooks:
+      - id: mypy
+        additional_dependencies: [pytest==7.3.1]
+        args: [--strict, --pretty, --show-error-codes]
 
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: 0.4.1
+    rev: 0.10.0
     hooks:
       - id: pyproject-fmt
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.10.1
+    rev: v0.13
     hooks:
       - id: validate-pyproject
 
   - repo: https://github.com/tox-dev/tox-ini-fmt
-    rev: 0.5.2
+    rev: 1.3.0
     hooks:
       - id: tox-ini-fmt
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.0-alpha.4
+    rev: v3.0.0-alpha.9-for-vscode
     hooks:
       - id: prettier
         args: [--prose-wrap=always, --print-width=88]
 
 ci:
   autoupdate_schedule: quarterly
```

### Comparing `fino-1.0.0/RELEASING.md` & `fino-1.1.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `fino-1.0.0/fino.py` & `fino-1.1.0/fino.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,20 +51,20 @@
     10**600: "sentiljoona",
 }
 # Just the few which don't have a simple -a partitive suffix
 PLURAL_TENS = {10: "kymmentä", 1000: "tuhatta", 10**100: "googolia"}
 LIST_OF_TENS = sorted(SINGULAR_TENS.keys())
 
 
-def print_it(text):
+def print_it(text: str) -> None:
     """Windows cmd.exe cannot do Unicode so encode first"""
     print(text.encode("utf-8"))
 
 
-def wordify(number, tens):
+def wordify(number: int, tens: int) -> str:
     if number == tens:
         return SINGULAR_TENS[tens]
     d, m = divmod(number, tens)
     if d > 1:
         if tens in PLURAL_TENS:
             plural = PLURAL_TENS[tens]
         else:
@@ -73,28 +73,28 @@
     else:
         word = SINGULAR_TENS[tens]
     if m > 0:
         word += to_finnish(m)
     return word
 
 
-def find_tens_range(number):
+def find_tens_range(number: int) -> int:
     """
     Find where a number comes in the list of tens.
     Return the ten before (or equal to it), or None if out of range.
     """
     n = bisect.bisect_left(LIST_OF_TENS, number)
 
     if LIST_OF_TENS[n : n + 1] == [number]:
         return LIST_OF_TENS[n]
     else:
         return LIST_OF_TENS[n - 1]
 
 
-def to_finnish(number):
+def to_finnish(number: int) -> str:
     """
     Given an integer, return the Finnish word for that number.
     """
     if isinstance(number, float):
         return "en tiedä"
     if number < 0:
         return "miinus " + to_finnish(abs(number))
```

### Comparing `fino-1.0.0/fino_guess.py` & `fino-1.1.0/fino_guess.py`

 * *Files identical despite different names*

### Comparing `fino-1.0.0/.github/labels.yml` & `fino-1.1.0/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `fino-1.0.0/.github/release-drafter.yml` & `fino-1.1.0/.github/release-drafter.yml`

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

### Comparing `fino-1.0.0/.github/workflows/test.yml` & `fino-1.1.0/.github/workflows/test.yml`

 * *Files 8% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", "3.12-dev"]
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

### Comparing `fino-1.0.0/.gitignore` & `fino-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fino-1.0.0/README.md` & `fino-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `fino-1.0.0/pyproject.toml` & `fino-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -11,53 +11,48 @@
 readme = "README.md"
 keywords = [
   "Finnish",
   "integers",
   "numbers",
   "suomi",
 ]
-authors = [{name = "hugovk"}]
-requires-python = ">=3.7"
+authors = [{name = "Hugo van Kemenade"}]
+requires-python = ">=3.8"
+classifiers = [
+  "Development Status :: 6 - Mature",
+  "Intended Audience :: Developers",
+  "Intended Audience :: Education",
+  "Intended Audience :: Science/Research",
+  "Natural Language :: English",
+  "Natural Language :: Finnish",
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
+  "Topic :: Scientific/Engineering :: Artificial Intelligence",
+]
 dynamic = [
   "version",
 ]
-classifiers = [
-    "Development Status :: 6 - Mature",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: Implementation :: CPython",
-    "Programming Language :: Python :: Implementation :: PyPy",
-    "Intended Audience :: Developers",
-    "Intended Audience :: Education",
-    "Intended Audience :: Science/Research",
-    "Natural Language :: English",
-    "Natural Language :: Finnish",
-    "Topic :: Artistic Software",
-    "Topic :: Scientific/Engineering :: Artificial Intelligence",
-]
 [project.optional-dependencies]
 tests = [
   "pytest",
   "pytest-cov",
 ]
-
 [project.urls]
 Changelog = "https://github.com/hugovk/fino/releases"
 Homepage = "https://github.com/hugovk/fino"
 Source = "https://github.com/hugovk/fino"
 
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

### Comparing `fino-1.0.0/PKG-INFO` & `fino-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: fino
-Version: 1.0.0
+Version: 1.1.0
 Summary: Output the Finnish word for a given integer
 Project-URL: Changelog, https://github.com/hugovk/fino/releases
 Project-URL: Homepage, https://github.com/hugovk/fino
 Project-URL: Source, https://github.com/hugovk/fino
-Author: hugovk
+Author: Hugo van Kemenade
 Keywords: Finnish,integers,numbers,suomi
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Finnish
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
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: tests
 Requires-Dist: pytest; extra == 'tests'
 Requires-Dist: pytest-cov; extra == 'tests'
 Description-Content-Type: text/markdown
 
 # fino
```

