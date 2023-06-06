# Comparing `tmp/enforce_notebook_run_order-1.3.0.tar.gz` & `tmp/enforce_notebook_run_order-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enforce_notebook_run_order-1.3.0.tar", max compression
+gzip compressed data, was "enforce_notebook_run_order-1.3.1.tar", max compression
```

## Comparing `enforce_notebook_run_order-1.3.0.tar` & `enforce_notebook_run_order-1.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     4156 2023-06-06 16:17:40.819149 enforce_notebook_run_order-1.3.0/README.md
--rw-r--r--   0        0        0      898 2023-06-06 16:17:40.819149 enforce_notebook_run_order-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      131 2023-06-06 16:17:40.819149 enforce_notebook_run_order-1.3.0/src/enforce_notebook_run_order/__init__.py
--rw-r--r--   0        0        0     1562 2023-06-06 16:17:40.819149 enforce_notebook_run_order-1.3.0/src/enforce_notebook_run_order/cli.py
--rw-r--r--   0        0        0     4666 2023-06-06 16:17:40.819149 enforce_notebook_run_order-1.3.0/src/enforce_notebook_run_order/enforce_notebook_run_order.py
--rw-r--r--   0        0        0     4028 2023-06-06 16:17:40.819149 enforce_notebook_run_order-1.3.0/src/enforce_notebook_run_order/temp_notebook.py
--rw-r--r--   0        0        0     2045 2023-06-06 16:17:40.823150 enforce_notebook_run_order-1.3.0/src/enforce_notebook_run_order/utils.py
--rw-r--r--   0        0        0     4874 1970-01-01 00:00:00.000000 enforce_notebook_run_order-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     4156 2023-06-06 16:21:56.675274 enforce_notebook_run_order-1.3.1/README.md
+-rw-r--r--   0        0        0      898 2023-06-06 16:21:56.675274 enforce_notebook_run_order-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      131 2023-06-06 16:21:56.675274 enforce_notebook_run_order-1.3.1/src/enforce_notebook_run_order/__init__.py
+-rw-r--r--   0        0        0     1562 2023-06-06 16:21:56.675274 enforce_notebook_run_order-1.3.1/src/enforce_notebook_run_order/cli.py
+-rw-r--r--   0        0        0     4666 2023-06-06 16:21:56.675274 enforce_notebook_run_order-1.3.1/src/enforce_notebook_run_order/enforce_notebook_run_order.py
+-rw-r--r--   0        0        0     4028 2023-06-06 16:21:56.675274 enforce_notebook_run_order-1.3.1/src/enforce_notebook_run_order/temp_notebook.py
+-rw-r--r--   0        0        0     2045 2023-06-06 16:21:56.675274 enforce_notebook_run_order-1.3.1/src/enforce_notebook_run_order/utils.py
+-rw-r--r--   0        0        0     4874 1970-01-01 00:00:00.000000 enforce_notebook_run_order-1.3.1/PKG-INFO
```

### Comparing `enforce_notebook_run_order-1.3.0/README.md` & `enforce_notebook_run_order-1.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
 To use `enforce_notebook_run_order` as a pre-commit hook, add the
 following to your `.pre-commit-config.yaml`:
 
 ``` {.sourceCode .yaml}
 repos:
 -   repo: https://github.com/christopher-hacker/enforce_notebook_run_order
-    rev: 1.0.0
+    rev: 1.3.1
     hooks:
     -   id: enforce-notebook-run-order
 ```
 
 ### disabling output checks
 
 By default, `enforce-notebook-run-order` will check that the output of
```

#### html2text {}

```diff
@@ -19,15 +19,15 @@
 check all notebooks in that directory: ``` {.sourceCode .bash} nbcheck
 my_notebooks/ ``` If no paths are specified, `nbcheck` will check all notebooks
 in the current directory. You can also use the full `enforce-notebook-run-
 order` command, but the `nbcheck` command is provided as a convenience. ###
 pre-commit hook To use `enforce_notebook_run_order` as a pre-commit hook, add
 the following to your `.pre-commit-config.yaml`: ``` {.sourceCode .yaml} repos:
 - repo: https://github.com/christopher-hacker/enforce_notebook_run_order rev:
-1.0.0 hooks: - id: enforce-notebook-run-order ``` ### disabling output checks
+1.3.1 hooks: - id: enforce-notebook-run-order ``` ### disabling output checks
 By default, `enforce-notebook-run-order` will check that the output of each
 cell matches the output of the previous run. This will catch cases where a cell
 is run out of order, but the execution count is still sequential. However, this
 can be problematic if the output of a cell changes between runs, such as when
 using random numbers. It can also be problematic if the notebook runs for a
 long time. There are three ways to disable output checks: 1. Disabling running
 all notebooks using the `--no-run` flag: ``` {.sourceCode .bash} nbcheck --no-
```

### Comparing `enforce_notebook_run_order-1.3.0/pyproject.toml` & `enforce_notebook_run_order-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "enforce-notebook-run-order"
-version = "1.3.0"
+version = "1.3.1"
 description = ""
 authors = ["Chris Hacker <49451910+christopher-hacker@users.noreply.github.com>"]
 license = "MIT"
 urls = { homepage = "https://github.com/christopher-hacker/enforce-notebook-run-order" }
 readme = "README.md"
 packages = [
     { include = "enforce_notebook_run_order", from = "src" },
```

### Comparing `enforce_notebook_run_order-1.3.0/src/enforce_notebook_run_order/cli.py` & `enforce_notebook_run_order-1.3.1/src/enforce_notebook_run_order/cli.py`

 * *Files identical despite different names*

### Comparing `enforce_notebook_run_order-1.3.0/src/enforce_notebook_run_order/enforce_notebook_run_order.py` & `enforce_notebook_run_order-1.3.1/src/enforce_notebook_run_order/enforce_notebook_run_order.py`

 * *Files identical despite different names*

### Comparing `enforce_notebook_run_order-1.3.0/src/enforce_notebook_run_order/temp_notebook.py` & `enforce_notebook_run_order-1.3.1/src/enforce_notebook_run_order/temp_notebook.py`

 * *Files identical despite different names*

### Comparing `enforce_notebook_run_order-1.3.0/src/enforce_notebook_run_order/utils.py` & `enforce_notebook_run_order-1.3.1/src/enforce_notebook_run_order/utils.py`

 * *Files identical despite different names*

### Comparing `enforce_notebook_run_order-1.3.0/PKG-INFO` & `enforce_notebook_run_order-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enforce-notebook-run-order
-Version: 1.3.0
+Version: 1.3.1
 Summary: 
 License: MIT
 Author: Chris Hacker
 Author-email: 49451910+christopher-hacker@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -92,15 +92,15 @@
 
 To use `enforce_notebook_run_order` as a pre-commit hook, add the
 following to your `.pre-commit-config.yaml`:
 
 ``` {.sourceCode .yaml}
 repos:
 -   repo: https://github.com/christopher-hacker/enforce_notebook_run_order
-    rev: 1.0.0
+    rev: 1.3.1
     hooks:
     -   id: enforce-notebook-run-order
 ```
 
 ### disabling output checks
 
 By default, `enforce-notebook-run-order` will check that the output of
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: enforce-notebook-run-order Version: 1.3.0 Summary:
+Metadata-Version: 2.1 Name: enforce-notebook-run-order Version: 1.3.1 Summary:
 License: MIT Author: Chris Hacker Author-email: 49451910+christopher-
 hacker@users.noreply.github.com Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: click
 (>=8.1.3,<9.0.0) Requires-Dist: jupyter (>=1.0.0,<2.0.0) Project-URL: homepage,
@@ -29,15 +29,15 @@
 check all notebooks in that directory: ``` {.sourceCode .bash} nbcheck
 my_notebooks/ ``` If no paths are specified, `nbcheck` will check all notebooks
 in the current directory. You can also use the full `enforce-notebook-run-
 order` command, but the `nbcheck` command is provided as a convenience. ###
 pre-commit hook To use `enforce_notebook_run_order` as a pre-commit hook, add
 the following to your `.pre-commit-config.yaml`: ``` {.sourceCode .yaml} repos:
 - repo: https://github.com/christopher-hacker/enforce_notebook_run_order rev:
-1.0.0 hooks: - id: enforce-notebook-run-order ``` ### disabling output checks
+1.3.1 hooks: - id: enforce-notebook-run-order ``` ### disabling output checks
 By default, `enforce-notebook-run-order` will check that the output of each
 cell matches the output of the previous run. This will catch cases where a cell
 is run out of order, but the execution count is still sequential. However, this
 can be problematic if the output of a cell changes between runs, such as when
 using random numbers. It can also be problematic if the notebook runs for a
 long time. There are three ways to disable output checks: 1. Disabling running
 all notebooks using the `--no-run` flag: ``` {.sourceCode .bash} nbcheck --no-
```

