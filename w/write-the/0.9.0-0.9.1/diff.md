# Comparing `tmp/write_the-0.9.0.tar.gz` & `tmp/write_the-0.9.1.tar.gz`

## Comparing `write_the-0.9.0.tar` & `write_the-0.9.1.tar`

### file list

```diff
@@ -1,70 +1,71 @@
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 write_the-0.9.0/mkdocs.yml
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 write_the-0.9.0/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 write_the-0.9.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 write_the-0.9.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.9.0/docs/CNAME
--rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 write_the-0.9.0/docs/index.md
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.9.0/docs/reference/cli.md
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 write_the-0.9.0/docs/reference/commands.md
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 write_the-0.9.0/docs/reference/cst.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 write_the-0.9.0/docs/reference/llm.md
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.9.0/docs/reference/utils.md
--rw-r--r--   0        0        0   121662 2020-02-02 00:00:00.000000 write_the-0.9.0/images/convert-help.png
--rw-r--r--   0        0        0   118788 2020-02-02 00:00:00.000000 write_the-0.9.0/images/docs-help.png
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 write_the-0.9.0/images/logo-black.svg
--rw-r--r--   0        0        0   821015 2020-02-02 00:00:00.000000 write_the-0.9.0/images/logo.png
--rw-r--r--   0        0        0    84667 2020-02-02 00:00:00.000000 write_the-0.9.0/images/mkdocs-help.png
--rw-r--r--   0        0        0  1092197 2020-02-02 00:00:00.000000 write_the-0.9.0/images/multiply-docs-tests.png
--rw-r--r--   0        0        0   139626 2020-02-02 00:00:00.000000 write_the-0.9.0/images/tests-help.png
--rw-r--r--   0        0        0  3588464 2020-02-02 00:00:00.000000 write_the-0.9.0/images/untitled.blend
--rw-r--r--   0        0        0  3580784 2020-02-02 00:00:00.000000 write_the-0.9.0/images/untitled.blend1
--rw-r--r--   0        0        0   464261 2020-02-02 00:00:00.000000 write_the-0.9.0/images/write-the-docs.gif
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 write_the-0.9.0/images/write-the-icon.svg
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 write_the-0.9.0/images/write-the.svg
--rw-r--r--   0        0        0     3413 2020-02-02 00:00:00.000000 write_the-0.9.0/tests/test_cli_main.py
--rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 write_the-0.9.0/tests/test_cst_docstring_adder.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 write_the-0.9.0/tests/test_cst_docstring_remover.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 write_the-0.9.0/tests/test_cst_function_and_class_collector.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 write_the-0.9.0/tests/test_cst_node_extractor.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 write_the-0.9.0/tests/test_cst_node_remover.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 write_the-0.9.0/tests/test_cst_utils.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 write_the-0.9.0/tests/test_utils.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 write_the-0.9.0/tests/data/calculate.py
--rw-r--r--   0        0        0    98897 2020-02-02 00:00:00.000000 write_the-0.9.0/tests/data/expected.dat
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 write_the-0.9.0/tests/data/multiply.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 write_the-0.9.0/tests/data/multiply_docstring.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/__about__.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/__main__.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/llm.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/utils.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/cli/__init__.py
--rw-r--r--   0        0        0    10009 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/cli/main.py
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/cli/tasks.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/commands/__init__.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/commands/converters/__init__.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/commands/converters/converters.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/commands/converters/prompts.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/commands/docs/__init__.py
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/commands/docs/docs.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/commands/docs/prompts.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/commands/docs/utils.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/commands/mkdocs/__init__.py
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/commands/mkdocs/mkdocs.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/commands/mkdocs/templates.py
--rwxr-xr-x   0        0        0       35 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/commands/tests/__init__.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/commands/tests/prompts.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/commands/tests/tests.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/cst/__init__.py
--rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/cst/docstring_adder.py
--rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/cst/docstring_remover.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/cst/function_and_class_collector.py
--rw-r--r--   0        0        0     8011 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/cst/node_batcher.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/cst/node_extractor.py
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/cst/node_remover.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/cst/utils.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 write_the-0.9.0/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 write_the-0.9.0/LICENSE.txt
--rw-r--r--   0        0        0     4566 2020-02-02 00:00:00.000000 write_the-0.9.0/README.md
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 write_the-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 write_the-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 write_the-0.9.1/mkdocs.yml
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 write_the-0.9.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 write_the-0.9.1/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 write_the-0.9.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 write_the-0.9.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.9.1/docs/CNAME
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 write_the-0.9.1/docs/index.md
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.9.1/docs/reference/cli.md
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 write_the-0.9.1/docs/reference/commands.md
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 write_the-0.9.1/docs/reference/cst.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 write_the-0.9.1/docs/reference/llm.md
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.9.1/docs/reference/utils.md
+-rw-r--r--   0        0        0   121662 2020-02-02 00:00:00.000000 write_the-0.9.1/images/convert-help.png
+-rw-r--r--   0        0        0   118788 2020-02-02 00:00:00.000000 write_the-0.9.1/images/docs-help.png
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 write_the-0.9.1/images/logo-black.svg
+-rw-r--r--   0        0        0   821015 2020-02-02 00:00:00.000000 write_the-0.9.1/images/logo.png
+-rw-r--r--   0        0        0    84667 2020-02-02 00:00:00.000000 write_the-0.9.1/images/mkdocs-help.png
+-rw-r--r--   0        0        0  1092197 2020-02-02 00:00:00.000000 write_the-0.9.1/images/multiply-docs-tests.png
+-rw-r--r--   0        0        0   139626 2020-02-02 00:00:00.000000 write_the-0.9.1/images/tests-help.png
+-rw-r--r--   0        0        0  3588464 2020-02-02 00:00:00.000000 write_the-0.9.1/images/untitled.blend
+-rw-r--r--   0        0        0  3580784 2020-02-02 00:00:00.000000 write_the-0.9.1/images/untitled.blend1
+-rw-r--r--   0        0        0   464261 2020-02-02 00:00:00.000000 write_the-0.9.1/images/write-the-docs.gif
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 write_the-0.9.1/images/write-the-icon.svg
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 write_the-0.9.1/images/write-the.svg
+-rw-r--r--   0        0        0     3413 2020-02-02 00:00:00.000000 write_the-0.9.1/tests/test_cli_main.py
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 write_the-0.9.1/tests/test_cst_docstring_adder.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 write_the-0.9.1/tests/test_cst_docstring_remover.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 write_the-0.9.1/tests/test_cst_function_and_class_collector.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 write_the-0.9.1/tests/test_cst_node_extractor.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 write_the-0.9.1/tests/test_cst_node_remover.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 write_the-0.9.1/tests/test_cst_utils.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 write_the-0.9.1/tests/test_utils.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 write_the-0.9.1/tests/data/calculate.py
+-rw-r--r--   0        0        0    98897 2020-02-02 00:00:00.000000 write_the-0.9.1/tests/data/expected.dat
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 write_the-0.9.1/tests/data/multiply.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 write_the-0.9.1/tests/data/multiply_docstring.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 write_the-0.9.1/write_the/__about__.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 write_the-0.9.1/write_the/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.9.1/write_the/__main__.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 write_the-0.9.1/write_the/llm.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 write_the-0.9.1/write_the/utils.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 write_the-0.9.1/write_the/cli/__init__.py
+-rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 write_the-0.9.1/write_the/cli/main.py
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 write_the-0.9.1/write_the/cli/tasks.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 write_the-0.9.1/write_the/commands/__init__.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 write_the-0.9.1/write_the/commands/converters/__init__.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 write_the-0.9.1/write_the/commands/converters/converters.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 write_the-0.9.1/write_the/commands/converters/prompts.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 write_the-0.9.1/write_the/commands/docs/__init__.py
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 write_the-0.9.1/write_the/commands/docs/docs.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 write_the-0.9.1/write_the/commands/docs/prompts.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 write_the-0.9.1/write_the/commands/docs/utils.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 write_the-0.9.1/write_the/commands/mkdocs/__init__.py
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 write_the-0.9.1/write_the/commands/mkdocs/mkdocs.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 write_the-0.9.1/write_the/commands/mkdocs/templates.py
+-rwxr-xr-x   0        0        0       35 2020-02-02 00:00:00.000000 write_the-0.9.1/write_the/commands/tests/__init__.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 write_the-0.9.1/write_the/commands/tests/prompts.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 write_the-0.9.1/write_the/commands/tests/tests.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 write_the-0.9.1/write_the/cst/__init__.py
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 write_the-0.9.1/write_the/cst/docstring_adder.py
+-rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 write_the-0.9.1/write_the/cst/docstring_remover.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 write_the-0.9.1/write_the/cst/function_and_class_collector.py
+-rw-r--r--   0        0        0     8011 2020-02-02 00:00:00.000000 write_the-0.9.1/write_the/cst/node_batcher.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 write_the-0.9.1/write_the/cst/node_extractor.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 write_the-0.9.1/write_the/cst/node_remover.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 write_the-0.9.1/write_the/cst/utils.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 write_the-0.9.1/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 write_the-0.9.1/LICENSE.txt
+-rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 write_the-0.9.1/README.md
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 write_the-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 write_the-0.9.1/PKG-INFO
```

### Comparing `write_the-0.9.0/mkdocs.yml` & `write_the-0.9.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/.github/workflows/publish.yml` & `write_the-0.9.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/.github/workflows/tests.yml` & `write_the-0.9.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/docs/index.md` & `write_the-0.9.1/docs/index.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 Write-the is an AI-powered documentation and test generation tool that leverages GPTs to automatically write tests, generate documentation, and refactor code. It is designed to streamline the development process, improve code quality, and increase productivity.
 
 ![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/write-the-docs.gif)
 
 ## Real-world examples
 
-- [`write-the docs` to write the docs for the `write-the docs` command 🤖](https://github.com/Wytamma/write-the/blob/master/write_the/docs/write.py#L14)
+- [`write-the docs` to write the docs for the `write-the docs` command 🤖](https://github.com/Wytamma/write-the/blob/5d7a5a22d082be6ee870c694ef2d24e6d1610758/write_the/commands/docs/docs.py#L26f)
 - [`write-the mkdocs` to build the documentation site for `write-the` 🤖](https://write-the.wytamma.com/)
 - [`write-the tests` to write tests for `write-the docs` 🤖](https://github.com/Wytamma/write-the/commit/6b6c8a08d7991e07e4972281c471f7842c04dda0)
 - [`write-the docs` and `write-the mkdocs` to build documenation for `autoresearcher` 🤖](https://github.com/eimenhmdt/autoresearcher/pull/17)
 - [`write-the docs` and `write-the mkdocs` to build documenation for `hyperspec` 🤖](https://github.com/smutch/hyperspec/pull/1)
 - [`write-the docs` and `write-the mkdocs` to build documenation for `CUPCAKEAGI` 🤖](https://github.com/AkshitIreddy/CUPCAKEAGI/pull/4)
 
 ## Installation
```

### Comparing `write_the-0.9.0/images/convert-help.png` & `write_the-0.9.1/images/convert-help.png`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/images/docs-help.png` & `write_the-0.9.1/images/docs-help.png`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/images/logo-black.svg` & `write_the-0.9.1/images/logo-black.svg`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/images/logo.png` & `write_the-0.9.1/images/logo.png`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/images/mkdocs-help.png` & `write_the-0.9.1/images/mkdocs-help.png`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/images/multiply-docs-tests.png` & `write_the-0.9.1/images/multiply-docs-tests.png`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/images/tests-help.png` & `write_the-0.9.1/images/tests-help.png`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/images/untitled.blend` & `write_the-0.9.1/images/untitled.blend`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/images/untitled.blend1` & `write_the-0.9.1/images/untitled.blend1`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/images/write-the-docs.gif` & `write_the-0.9.1/images/write-the-docs.gif`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/images/write-the-icon.svg` & `write_the-0.9.1/images/write-the-icon.svg`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/images/write-the.svg` & `write_the-0.9.1/images/write-the.svg`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/tests/test_cli_main.py` & `write_the-0.9.1/tests/test_cli_main.py`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/tests/test_cst_docstring_adder.py` & `write_the-0.9.1/tests/test_cst_docstring_adder.py`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/tests/test_cst_docstring_remover.py` & `write_the-0.9.1/tests/test_cst_docstring_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/tests/test_cst_function_and_class_collector.py` & `write_the-0.9.1/tests/test_cst_function_and_class_collector.py`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/tests/test_cst_node_extractor.py` & `write_the-0.9.1/tests/test_cst_node_extractor.py`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/tests/test_cst_node_remover.py` & `write_the-0.9.1/tests/test_cst_node_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/tests/test_cst_utils.py` & `write_the-0.9.1/tests/test_cst_utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/tests/test_utils.py` & `write_the-0.9.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/tests/data/expected.dat` & `write_the-0.9.1/tests/data/expected.dat`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/write_the/llm.py` & `write_the-0.9.1/write_the/llm.py`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/write_the/utils.py` & `write_the-0.9.1/write_the/utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/write_the/cli/main.py` & `write_the-0.9.1/write_the/cli/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     """
     AI-powered Code Generation and Refactoring Tool
     """
 
 
 @app.async_command()
 async def docs(
-    file: Path = typer.Argument(..., help="Path to the code file/folder."),
+    file: List[Path] = typer.Argument(..., help="Path to the code file/folder."),
     nodes: List[str] = typer.Option(
         None,
         "--node",
         "-n",
         help="Generate docs for specific nodes (functions and classes).",
     ),
     save: bool = typer.Option(
@@ -93,19 +93,21 @@
     batch: bool = typer.Option(
         False, "--batch/--no-batch", "-b", help="Send each node as a separate request."
     ),
 ):
     """
     Document your code with AI.
     """
-    if file.is_dir():
-        files = list_python_files(file)
-    else:
-        assert file.suffix == ".py"
-        files = [file]
+    files = []
+    for f in file:
+        if f.is_dir():
+            files.extend(list_python_files(f))
+        else:
+            assert f.suffix == ".py"
+            files.append(f)
     with Progress(
         SpinnerColumn(),
         TextColumn("{task.description}"),
         transient=True,
         auto_refresh=True,
     ) as progress:
         tasks = []
```

### Comparing `write_the-0.9.0/write_the/cli/tasks.py` & `write_the-0.9.1/write_the/cli/tasks.py`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/write_the/commands/converters/converters.py` & `write_the-0.9.1/write_the/commands/converters/converters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from pathlib import Path
-from black import format_str, FileMode
 from .prompts import write_converters_for_file_prompt
 from write_the.llm import LLM
 
 
 async def write_the_converters(filename: Path, input_format: str, output_format: str, gpt_4: bool = False) -> str:
     """
     Formats and runs the tests for a given file.
```

### Comparing `write_the-0.9.0/write_the/commands/docs/docs.py` & `write_the-0.9.1/write_the/commands/docs/docs.py`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/write_the/commands/docs/prompts.py` & `write_the-0.9.1/write_the/commands/docs/prompts.py`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/write_the/commands/docs/utils.py` & `write_the-0.9.1/write_the/commands/docs/utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/write_the/commands/mkdocs/mkdocs.py` & `write_the-0.9.1/write_the/commands/mkdocs/mkdocs.py`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/write_the/commands/mkdocs/templates.py` & `write_the-0.9.1/write_the/commands/mkdocs/templates.py`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/write_the/commands/tests/tests.py` & `write_the-0.9.1/write_the/commands/tests/tests.py`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/write_the/cst/docstring_adder.py` & `write_the-0.9.1/write_the/cst/docstring_adder.py`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/write_the/cst/docstring_remover.py` & `write_the-0.9.1/write_the/cst/docstring_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/write_the/cst/function_and_class_collector.py` & `write_the-0.9.1/write_the/cst/function_and_class_collector.py`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/write_the/cst/node_batcher.py` & `write_the-0.9.1/write_the/cst/node_batcher.py`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/write_the/cst/node_extractor.py` & `write_the-0.9.1/write_the/cst/node_extractor.py`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/write_the/cst/node_remover.py` & `write_the-0.9.1/write_the/cst/node_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/write_the/cst/utils.py` & `write_the-0.9.1/write_the/cst/utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/LICENSE.txt` & `write_the-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/README.md` & `write_the-0.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 AI-powered Documentation and Test Generation Tool
 
 [![PyPI - Version](https://img.shields.io/pypi/v/write-the.svg)](https://pypi.org/project/write-the)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/write-the.svg)](https://pypi.org/project/write-the)
 [![write-the - docs](https://badgen.net/badge/write-the/docs/blue?icon=https://raw.githubusercontent.com/Wytamma/write-the/master/images/write-the-icon.svg)](https://write-the.wytamma.com/)
 [![write-the - test](https://badgen.net/badge/write-the/tests/green?icon=https://raw.githubusercontent.com/Wytamma/write-the/master/images/write-the-icon.svg)](https://github.com/Wytamma/write-the/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/Wytamma/write-the/branch/master/graph/badge.svg?token=yEDn56L76k)](https://app.codecov.io/gh/Wytamma/write-the/tree/master)
-
+[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FWytamma%2Fwrite-the&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://github.com/Wytamma/write-the)
 
 Write-the is an AI-powered documentation and test generation tool that leverages GPTs to automatically write tests, generate documentation, and refactor code. It is designed to streamline the development process, improve code quality, and increase productivity.
 
 ![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/write-the-docs.gif)
 
 ## Real-world examples
 
-- [`write-the docs` to write the docs for the `write-the docs` command 🤖](https://github.com/Wytamma/write-the/blob/master/write_the/docs/write.py#L14)
+- [`write-the docs` to write the docs for the `write-the docs` command 🤖](https://github.com/Wytamma/write-the/blob/5d7a5a22d082be6ee870c694ef2d24e6d1610758/write_the/commands/docs/docs.py#L26)
 - [`write-the mkdocs` to build the documentation site for `write-the` 🤖](https://write-the.wytamma.com/)
 - [`write-the tests` to write tests for `write-the docs` 🤖](https://github.com/Wytamma/write-the/commit/6b6c8a08d7991e07e4972281c471f7842c04dda0)
 - [`write-the docs` and `write-the mkdocs` to build documenation for `autoresearcher` 🤖](https://github.com/eimenhmdt/autoresearcher/pull/17)
 - [`write-the docs` and `write-the mkdocs` to build documenation for `hyperspec` 🤖](https://github.com/smutch/hyperspec/pull/1)
 - [`write-the docs` and `write-the mkdocs` to build documenation for `CUPCAKEAGI` 🤖](https://github.com/AkshitIreddy/CUPCAKEAGI/pull/4)
 
 ## Installation
```

### Comparing `write_the-0.9.0/pyproject.toml` & `write_the-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `write_the-0.9.0/PKG-INFO` & `write_the-0.9.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: write-the
-Version: 0.9.0
+Version: 0.9.1
 Summary: AI-powered Code Generation and Refactoring Tool
 Project-URL: Documentation, https://github.com/wytamma/write-the#readme
 Project-URL: Issues, https://github.com/wytamma/write-the/issues
 Project-URL: Source, https://github.com/wytamma/write-the
 Author-email: wytamma <wytamma.wirth@me.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -32,23 +32,23 @@
 AI-powered Documentation and Test Generation Tool
 
 [![PyPI - Version](https://img.shields.io/pypi/v/write-the.svg)](https://pypi.org/project/write-the)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/write-the.svg)](https://pypi.org/project/write-the)
 [![write-the - docs](https://badgen.net/badge/write-the/docs/blue?icon=https://raw.githubusercontent.com/Wytamma/write-the/master/images/write-the-icon.svg)](https://write-the.wytamma.com/)
 [![write-the - test](https://badgen.net/badge/write-the/tests/green?icon=https://raw.githubusercontent.com/Wytamma/write-the/master/images/write-the-icon.svg)](https://github.com/Wytamma/write-the/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/Wytamma/write-the/branch/master/graph/badge.svg?token=yEDn56L76k)](https://app.codecov.io/gh/Wytamma/write-the/tree/master)
-
+[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FWytamma%2Fwrite-the&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://github.com/Wytamma/write-the)
 
 Write-the is an AI-powered documentation and test generation tool that leverages GPTs to automatically write tests, generate documentation, and refactor code. It is designed to streamline the development process, improve code quality, and increase productivity.
 
 ![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/write-the-docs.gif)
 
 ## Real-world examples
 
-- [`write-the docs` to write the docs for the `write-the docs` command 🤖](https://github.com/Wytamma/write-the/blob/master/write_the/docs/write.py#L14)
+- [`write-the docs` to write the docs for the `write-the docs` command 🤖](https://github.com/Wytamma/write-the/blob/5d7a5a22d082be6ee870c694ef2d24e6d1610758/write_the/commands/docs/docs.py#L26)
 - [`write-the mkdocs` to build the documentation site for `write-the` 🤖](https://write-the.wytamma.com/)
 - [`write-the tests` to write tests for `write-the docs` 🤖](https://github.com/Wytamma/write-the/commit/6b6c8a08d7991e07e4972281c471f7842c04dda0)
 - [`write-the docs` and `write-the mkdocs` to build documenation for `autoresearcher` 🤖](https://github.com/eimenhmdt/autoresearcher/pull/17)
 - [`write-the docs` and `write-the mkdocs` to build documenation for `hyperspec` 🤖](https://github.com/smutch/hyperspec/pull/1)
 - [`write-the docs` and `write-the mkdocs` to build documenation for `CUPCAKEAGI` 🤖](https://github.com/AkshitIreddy/CUPCAKEAGI/pull/4)
 
 ## Installation
```

