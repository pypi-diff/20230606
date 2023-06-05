# Comparing `tmp/mdformat_mkdocs-1.0.0.tar.gz` & `tmp/mdformat_mkdocs-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdformat_mkdocs-1.0.0.tar", last modified: Thu Jan 12 01:24:25 2023, max compression
+gzip compressed data, was "mdformat_mkdocs-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mdformat_mkdocs-1.0.0.tar` & `mdformat_mkdocs-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1819 2023-01-12 01:24:21.630849 mdformat_mkdocs-1.0.0/.gitignore
--rw-r--r--   0        0        0     1974 2023-01-12 01:24:21.634849 mdformat_mkdocs-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      296 2023-01-12 01:24:21.634849 mdformat_mkdocs-1.0.0/.pre-commit-test.yaml
--rw-r--r--   0        0        0       33 2023-01-12 01:24:21.634849 mdformat_mkdocs-1.0.0/.tool-versions
--rw-r--r--   0        0        0      921 2023-01-12 01:24:21.634849 mdformat_mkdocs-1.0.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1073 2023-01-12 01:24:21.634849 mdformat_mkdocs-1.0.0/LICENSE
--rw-r--r--   0        0        0     2596 2023-01-12 01:24:21.634849 mdformat_mkdocs-1.0.0/README.md
--rw-r--r--   0        0        0      134 2023-01-12 01:24:21.634849 mdformat_mkdocs-1.0.0/mdformat_mkdocs/__init__.py
--rw-r--r--   0        0        0     2818 2023-01-12 01:24:21.634849 mdformat_mkdocs-1.0.0/mdformat_mkdocs/plugin.py
--rw-r--r--   0        0        0     1639 2023-01-12 01:24:21.634849 mdformat_mkdocs-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      789 2023-01-12 01:24:21.634849 mdformat_mkdocs-1.0.0/tox.ini
--rw-r--r--   0        0        0     4025 1970-01-01 00:00:00.000000 mdformat_mkdocs-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1819 2023-06-05 22:05:28.405867 mdformat_mkdocs-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1729 2023-06-05 22:05:28.405867 mdformat_mkdocs-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      296 2023-06-05 22:05:28.405867 mdformat_mkdocs-1.0.1/.pre-commit-test.yaml
+-rw-r--r--   0        0        0       33 2023-06-05 22:05:28.405867 mdformat_mkdocs-1.0.1/.tool-versions
+-rw-r--r--   0        0        0      921 2023-06-05 22:05:28.405867 mdformat_mkdocs-1.0.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1073 2023-06-05 22:05:28.405867 mdformat_mkdocs-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2589 2023-06-05 22:05:28.405867 mdformat_mkdocs-1.0.1/README.md
+-rw-r--r--   0        0        0      134 2023-06-05 22:05:28.405867 mdformat_mkdocs-1.0.1/mdformat_mkdocs/__init__.py
+-rw-r--r--   0        0        0     2764 2023-06-05 22:05:28.405867 mdformat_mkdocs-1.0.1/mdformat_mkdocs/plugin.py
+-rw-r--r--   0        0        0     1639 2023-06-05 22:05:28.405867 mdformat_mkdocs-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      789 2023-06-05 22:05:28.405867 mdformat_mkdocs-1.0.1/tox.ini
+-rw-r--r--   0        0        0     4018 1970-01-01 00:00:00.000000 mdformat_mkdocs-1.0.1/PKG-INFO
```

### Comparing `mdformat_mkdocs-1.0.0/.gitignore` & `mdformat_mkdocs-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.0/.pre-commit-config.yaml` & `mdformat_mkdocs-1.0.1/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -23,23 +23,23 @@
       - id: mixed-line-ending
         args: [--fix=auto]
       - id: pretty-format-json
         args: [--autofix, --indent=4]
       - id: trailing-whitespace
         exclude: tests/fixtures.*\.md
   - repo: https://github.com/pre-commit/pygrep-hooks
-    rev: v1.9.0
+    rev: v1.10.0
     hooks:
       - id: python-check-blanket-noqa
   - repo: https://github.com/timothycrosley/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/psf/black
-    rev: 22.10.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/pycqa/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
         additional_dependencies:
@@ -47,26 +47,16 @@
           - flake8-builtins>=1.5.3
           - flake8-comprehensions>=3.4.0
         args: [--ignore=E501]
   - repo: https://github.com/executablebooks/mdformat
     rev: 0.7.16
     hooks:
       - id: mdformat
-        additional_dependencies:
-          - mdformat-admon
-          - mdformat-beautysh
-          - mdformat-black
-          - mdformat-config
-          - mdformat-footnote
-          - mdformat-frontmatter
-          - mdformat-gfm
-          - mdformat-tables
-          - mdformat-toc
-          - mdformat-web
+        additional_dependencies: ['mdformat-mkdocs[recommended]']
         exclude: tests/.+\.md
         args: [--wrap=no]
   - repo: https://github.com/lyz-code/yamlfix/
-    rev: 1.1.1
+    rev: 1.9.0
     hooks:
       - id: yamlfix
         types_or: []
         types: [file, yaml]
```

### Comparing `mdformat_mkdocs-1.0.0/CONTRIBUTING.md` & `mdformat_mkdocs-1.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.0/LICENSE` & `mdformat_mkdocs-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.0/README.md` & `mdformat_mkdocs-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,11 +56,11 @@
 
 See the example test files, [./tests/pre-commit-test.md](https://raw.githubusercontent.com/KyleKing/mdformat-mkdocs/main/tests/pre-commit-test.md) and [./tests/fixtures.md](https://raw.githubusercontent.com/KyleKing/mdformat-mkdocs/main/tests/fixtures.md)
 
 ## Contributing
 
 See [CONTRIBUTING.md](https://github.com/KyleKing/mdformat-mkdocs/blob/main/CONTRIBUTING.md)
 
-[ci-badge]: https://github.com/executablebooks/mdformat-mkdocs/workflows/CI/badge.svg?branch=main
-[ci-link]: https://github.com/executablebooks/mdformat/actions?query=workflow%3ACI+branch%3Amain+event%3Apush
+[ci-badge]: https://github.com/kyleking/mdformat-mkdocs/workflows/CI/badge.svg?branch=main
+[ci-link]: https://github.com/kyleking/mdformat-mkdocs/actions?query=workflow%3ACI+branch%3Amain+event%3Apush
 [pypi-badge]: https://img.shields.io/pypi/v/mdformat-mkdocs.svg
 [pypi-link]: https://pypi.org/project/mdformat-mkdocs
```

### Comparing `mdformat_mkdocs-1.0.0/mdformat_mkdocs/plugin.py` & `mdformat_mkdocs-1.0.1/mdformat_mkdocs/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 
 
 def update_mdit(mdit: MarkdownIt) -> None:
     """No changes to markdown parsing are necessary."""
     ...
 
 
-_RE_INDENT = re.compile(r"(?P<indent>\s*)(?P<content>.*)")
+_RE_INDENT = re.compile(r"(?P<indent>\s*)(?P<content>[^\s]?.*)")
 """Match `indent` and `content` against line`."""
 
 _RE_LIST_ITEM = re.compile(r"(?P<bullet>[\-\*\d\.]+)\s+(?P<item>.+)")
 """Match `bullet` and `item` against `content`."""
 
 
 def _normalize_list(text: str, node: RenderTreeNode, context: RenderContext) -> str:
     """Post-processor to normalize lists."""
-    eol = "\n"  # PLANNED: Does this need to support carriage returns?
+    eol = "\n"
     indent = " " * _MKDOCS_INDENT_COUNT
 
     rendered = ""
     last_indent = ""
     indent_counter = 0
     indent_lookup: Dict[str, int] = {}
     for line in text.split(eol):
@@ -49,15 +49,15 @@
                 indent_lookup[this_indent] = indent_counter
             elif this_indent in indent_lookup:
                 indent_counter = indent_lookup[this_indent]
             else:
                 raise NotImplementedError(f"Error in indentation of: `{line}`")
         else:
             indent_counter = 0
-        last_indent = match["indent"]
+        last_indent = this_indent
         new_indent = indent * indent_counter
         rendered += f"{new_indent}{new_line.strip()}{eol}"
     return rendered.rstrip()
 
 
 # A mapping from `RenderTreeNode.type` to a `Render` function that can
 # render the given `RenderTreeNode` type. These override the default
```

### Comparing `mdformat_mkdocs-1.0.0/pyproject.toml` & `mdformat_mkdocs-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.0/tox.ini` & `mdformat_mkdocs-1.0.1/tox.ini`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.0/PKG-INFO` & `mdformat_mkdocs-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdformat_mkdocs
-Version: 1.0.0
+Version: 1.0.1
 Summary: An mdformat plugin for mkdocs.
 Keywords: mdformat,markdown,markdown-it
 Author-email: Kyle King <dev.act.kyle@gmail.com>
 Requires-Python: >=3.7.2
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -89,12 +89,12 @@
 
 See the example test files, [./tests/pre-commit-test.md](https://raw.githubusercontent.com/KyleKing/mdformat-mkdocs/main/tests/pre-commit-test.md) and [./tests/fixtures.md](https://raw.githubusercontent.com/KyleKing/mdformat-mkdocs/main/tests/fixtures.md)
 
 ## Contributing
 
 See [CONTRIBUTING.md](https://github.com/KyleKing/mdformat-mkdocs/blob/main/CONTRIBUTING.md)
 
-[ci-badge]: https://github.com/executablebooks/mdformat-mkdocs/workflows/CI/badge.svg?branch=main
-[ci-link]: https://github.com/executablebooks/mdformat/actions?query=workflow%3ACI+branch%3Amain+event%3Apush
+[ci-badge]: https://github.com/kyleking/mdformat-mkdocs/workflows/CI/badge.svg?branch=main
+[ci-link]: https://github.com/kyleking/mdformat-mkdocs/actions?query=workflow%3ACI+branch%3Amain+event%3Apush
 [pypi-badge]: https://img.shields.io/pypi/v/mdformat-mkdocs.svg
 [pypi-link]: https://pypi.org/project/mdformat-mkdocs
```

