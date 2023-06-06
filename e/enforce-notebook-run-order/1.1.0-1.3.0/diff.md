# Comparing `tmp/enforce_notebook_run_order-1.1.0.tar.gz` & `tmp/enforce_notebook_run_order-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enforce_notebook_run_order-1.1.0.tar", max compression
+gzip compressed data, was "enforce_notebook_run_order-1.3.0.tar", max compression
```

## Comparing `enforce_notebook_run_order-1.1.0.tar` & `enforce_notebook_run_order-1.3.0.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0     3160 2023-06-05 19:36:42.036154 enforce_notebook_run_order-1.1.0/README.md
--rw-r--r--   0        0        0      865 2023-06-05 19:36:42.036154 enforce_notebook_run_order-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     5578 2023-06-05 19:36:42.036154 enforce_notebook_run_order-1.1.0/src/enforce_notebook_run_order.py
--rw-r--r--   0        0        0     3445 2023-06-05 19:36:42.036154 enforce_notebook_run_order-1.1.0/src/temp_notebook.py
--rw-r--r--   0        0        0     3878 1970-01-01 00:00:00.000000 enforce_notebook_run_order-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4156 2023-06-06 16:17:40.819149 enforce_notebook_run_order-1.3.0/README.md
+-rw-r--r--   0        0        0      898 2023-06-06 16:17:40.819149 enforce_notebook_run_order-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      131 2023-06-06 16:17:40.819149 enforce_notebook_run_order-1.3.0/src/enforce_notebook_run_order/__init__.py
+-rw-r--r--   0        0        0     1562 2023-06-06 16:17:40.819149 enforce_notebook_run_order-1.3.0/src/enforce_notebook_run_order/cli.py
+-rw-r--r--   0        0        0     4666 2023-06-06 16:17:40.819149 enforce_notebook_run_order-1.3.0/src/enforce_notebook_run_order/enforce_notebook_run_order.py
+-rw-r--r--   0        0        0     4028 2023-06-06 16:17:40.819149 enforce_notebook_run_order-1.3.0/src/enforce_notebook_run_order/temp_notebook.py
+-rw-r--r--   0        0        0     2045 2023-06-06 16:17:40.823150 enforce_notebook_run_order-1.3.0/src/enforce_notebook_run_order/utils.py
+-rw-r--r--   0        0        0     4874 1970-01-01 00:00:00.000000 enforce_notebook_run_order-1.3.0/PKG-INFO
```

### Comparing `enforce_notebook_run_order-1.1.0/README.md` & `enforce_notebook_run_order-1.3.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -59,25 +59,58 @@
 
 Or point it to a directory to check all notebooks in that directory:
 
 ``` {.sourceCode .bash}
 nbcheck my_notebooks/
 ```
 
+If no paths are specified, `nbcheck` will check all notebooks in the
+current directory.
+
 You can also use the full `enforce-notebook-run-order` command, but the
 `nbcheck` command is provided as a convenience.
 
-For information on the command line interface, please refer to the [CLI
-documentation](module_enforce_notebook_run_order.html#command-line-interface).
-
 ### pre-commit hook
 
 To use `enforce_notebook_run_order` as a pre-commit hook, add the
 following to your `.pre-commit-config.yaml`:
 
 ``` {.sourceCode .yaml}
 repos:
 -   repo: https://github.com/christopher-hacker/enforce_notebook_run_order
     rev: 1.0.0
     hooks:
     -   id: enforce-notebook-run-order
 ```
+
+### disabling output checks
+
+By default, `enforce-notebook-run-order` will check that the output of
+each cell matches the output of the previous run. This will catch cases
+where a cell is run out of order, but the execution count is still
+sequential. However, this can be problematic if the output of a cell
+changes between runs, such as when using random numbers. It can also be
+problematic if the notebook runs for a long time.
+
+There are three ways to disable output checks:
+
+1.  Disabling running all notebooks using the `--no-run` flag:
+
+    ``` {.sourceCode .bash}
+    nbcheck --no-run my_notebook.ipynb
+    ```
+
+2.  Disabling running a single notebook using the `no-run` marker **in
+    the first cell of the notebook**:
+
+    > ``` {.sourceCode .python}
+    > # no-run
+    > print("This notebook will not be run")
+    > ```
+
+3.  Disabling output checks for a single cell using the
+    `no-check-output` marker:
+
+    > ``` {.sourceCode .python}
+    > # no-check-output
+    > print("This cell will be run, but its output will not be checked")
+    > ```
```

#### html2text {}

```diff
@@ -13,15 +13,27 @@
 pre-commit.com/). See the [pre-commit hook](#pre-commit-hook) section for more
 details. Usage ----- `enforce-notebook-run-order` can be used as a standalone
 script, or as a [pre-commit hook](https://pre-commit.com/). ### Standalone To
 use `enforce-notebook-run-order` as a standalone script, simply run it with the
 path to the notebook(s) you want to check: ``` {.sourceCode .bash} nbcheck
 my_notebook.ipynb my_other_notebook.ipynb ``` Or point it to a directory to
 check all notebooks in that directory: ``` {.sourceCode .bash} nbcheck
-my_notebooks/ ``` You can also use the full `enforce-notebook-run-order`
-command, but the `nbcheck` command is provided as a convenience. For
-information on the command line interface, please refer to the [CLI
-documentation](module_enforce_notebook_run_order.html#command-line-interface).
-### pre-commit hook To use `enforce_notebook_run_order` as a pre-commit hook,
-add the following to your `.pre-commit-config.yaml`: ``` {.sourceCode .yaml}
-repos: - repo: https://github.com/christopher-hacker/enforce_notebook_run_order
-rev: 1.0.0 hooks: - id: enforce-notebook-run-order ```
+my_notebooks/ ``` If no paths are specified, `nbcheck` will check all notebooks
+in the current directory. You can also use the full `enforce-notebook-run-
+order` command, but the `nbcheck` command is provided as a convenience. ###
+pre-commit hook To use `enforce_notebook_run_order` as a pre-commit hook, add
+the following to your `.pre-commit-config.yaml`: ``` {.sourceCode .yaml} repos:
+- repo: https://github.com/christopher-hacker/enforce_notebook_run_order rev:
+1.0.0 hooks: - id: enforce-notebook-run-order ``` ### disabling output checks
+By default, `enforce-notebook-run-order` will check that the output of each
+cell matches the output of the previous run. This will catch cases where a cell
+is run out of order, but the execution count is still sequential. However, this
+can be problematic if the output of a cell changes between runs, such as when
+using random numbers. It can also be problematic if the notebook runs for a
+long time. There are three ways to disable output checks: 1. Disabling running
+all notebooks using the `--no-run` flag: ``` {.sourceCode .bash} nbcheck --no-
+run my_notebook.ipynb ``` 2. Disabling running a single notebook using the `no-
+run` marker **in the first cell of the notebook**: > ``` {.sourceCode .python}
+> # no-run > print("This notebook will not be run") > ``` 3. Disabling output
+checks for a single cell using the `no-check-output` marker: > ``` {.sourceCode
+.python} > # no-check-output > print("This cell will be run, but its output
+will not be checked") > ```
```

### Comparing `enforce_notebook_run_order-1.1.0/pyproject.toml` & `enforce_notebook_run_order-1.3.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "enforce-notebook-run-order"
-version = "1.1.0"
+version = "1.3.0"
 description = ""
 authors = ["Chris Hacker <49451910+christopher-hacker@users.noreply.github.com>"]
 license = "MIT"
 urls = { homepage = "https://github.com/christopher-hacker/enforce-notebook-run-order" }
 readme = "README.md"
 packages = [
-    { include = "*", from = "src" },
+    { include = "enforce_notebook_run_order", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 jupyter = "^1.0.0"
 click = "^8.1.3"
 
@@ -27,9 +27,9 @@
 pre-commit = "^3.3.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-enforce-notebook-run-order = "enforce_notebook_run_order:cli"
-nbcheck = "enforce_notebook_run_order:cli"
+enforce-notebook-run-order = "enforce_notebook_run_order.cli:cli"
+nbcheck = "enforce_notebook_run_order.cli:cli"
```

### Comparing `enforce_notebook_run_order-1.1.0/src/enforce_notebook_run_order.py` & `enforce_notebook_run_order-1.3.0/src/enforce_notebook_run_order/enforce_notebook_run_order.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,25 @@
-"""forces notebooks to run cells sequentially and fails if cells were run out of order"""
+"""Forces notebooks to run cells sequentially and fails if cells were run out of order"""
 
-import json
 import os
 import pathlib
-from typing import List
-import warnings
-import click
-import temp_notebook
+from . import temp_notebook
+from . import utils
 
 
 class NotebookCodeCellNotRunError(Exception):
-    """raised when a notebook code cell was not run"""
+    """Raised when a notebook code cell was not run"""
 
 
 class NotebookRunOrderError(Exception):
-    """raised when a notebook is run out of order"""
+    """Raised when a notebook is run out of order"""
 
 
 class InvalidNotebookRunError(Exception):
-    """raised when any problems were identified with a notebook's run order"""
+    """Raised when any problems were identified with a notebook's run order"""
 
 
 def notebook_is_in_virtualenv(notebook_path: pathlib.Path) -> bool:
     """
     Checks whether a notebook is in the current repo or is in the virtual environment's
     site-packages directory.
 
@@ -48,37 +45,44 @@
         notebook_data (dict): Notebook data in dictionary format.
 
     Raises:
         NotebookCodeCellNotRunError: If a code cell in the notebook was not run.
         NotebookRunOrderError: If the cells in the notebook were not run sequentially.
     """
     previous_cell_number = 0
-    for cell in notebook_data["cells"]:
-        if cell["cell_type"] == "code":
-            current_cell_number = cell["execution_count"]
-            if current_cell_number is None:
-                raise NotebookCodeCellNotRunError(
-                    f"Code cell was not run. The previous cell was #{previous_cell_number}. \n\n"
-                    f"Cell contents: \n\n> {cell}"
-                )
-            if current_cell_number != previous_cell_number + 1:
-                raise NotebookRunOrderError(
-                    "Cells were not run sequentially. "
-                    f"The cell that caused this error is #{current_cell_number} "
-                    f"and the previous cell was #{previous_cell_number}. \n\n"
-                    f"Cell contents: \n\n> {cell}"
-                )
-            previous_cell_number = current_cell_number
+    code_cells = utils.get_code_cells(notebook_data)
+    for cell in code_cells:
+        current_cell_number = cell["execution_count"]
+        if current_cell_number is None:
+            raise NotebookCodeCellNotRunError(
+                f"Code cell was not run. The previous cell was #{previous_cell_number}. \n\n"
+                f"Cell contents: \n\n> {cell}"
+            )
+        if current_cell_number != previous_cell_number + 1:
+            raise NotebookRunOrderError(
+                "Cells were not run sequentially. "
+                f"The cell that caused this error is #{current_cell_number} "
+                f"and the previous cell was #{previous_cell_number}. \n\n"
+                f"Cell contents: \n\n> {cell}"
+            )
+        previous_cell_number = current_cell_number
 
 
 def check_single_notebook(notebook_path: str, no_run: bool = False):
-    """Check a single notebook."""
+    """Check a single notebook
+
+    Args:
+        notebook_path (str): Path to the notebook file.
+        no_run (bool, optional): If True, do not run the notebook. Defaults to False.
+
+    Raises:
+        InvalidNotebookRunError: If any problems were identified with the notebook's run order.
+    """
     notebook_path = pathlib.Path(notebook_path)
-    with open(notebook_path, "r", encoding="UTF-8") as notebook_file:
-        notebook_data = json.load(notebook_file)
+    notebook_data = utils.load_notebook_data(notebook_path)
     try:
         check_notebook_run_order(notebook_data)
         if not no_run:
             with temp_notebook.TempNotebook(notebook_data) as temp_nb:
                 temp_nb.check_notebook()
     except (
         NotebookCodeCellNotRunError,
@@ -89,15 +93,25 @@
         raise InvalidNotebookRunError(
             f"Notebook {notebook_path} was not run in order.\n\n{error}\n\n"
         ) from error
     print(f"Notebook {notebook_path} was run correctly.")
 
 
 def process_path(path: str, no_run: bool = False):
-    """Processes a single path. Raises an exception if the path is invalid."""
+    """
+    Processes a single path. Raises an exception if the path is invalid
+
+    Args:
+        path (str): Path to the notebook file or directory.
+        no_run (bool, optional): If True, do not run the notebook. Defaults to False.
+
+    Raises:
+        ValueError: If the path is invalid.
+    """
+
     if os.path.isdir(path):
         # Get all .ipynb files in the directory and its subdirectories
         for dirpath, _, filenames in os.walk(path):
             for filename in filenames:
                 notebok_path = pathlib.Path(dirpath) / filename
                 if filename.endswith(".ipynb") and not notebook_is_in_virtualenv(
                     notebok_path
@@ -109,42 +123,7 @@
     elif path.endswith(".ipynb"):
         check_single_notebook(path)
     else:
         raise ValueError(
             f"Cannot check file {path}. "
             "Must be a path to a notebook file with the .ipynb extension, or a directory."
         )
-
-
-@click.command()
-@click.argument("paths", nargs=-1, type=click.Path(exists=True), required=False)
-@click.option(
-    "--no-run",
-    is_flag=True,
-    help="Do not run the notebooks, only check the run order. "
-    "This may miss some errors, but is useful for extremely long running notebooks. "
-    "If you use this option, you should consider moving the long-running code to a "
-    "separate task that runs separately from the notebook.",
-)
-def cli(paths: List[str] = None, no_run: bool = False):
-    """
-    Checks the run order of notebooks in the specified paths,
-    or the entire repo if no paths are specified
-    """
-    if no_run:
-        warnings.warn(
-            "The --no-run option will not catch all problems with notebooks. "
-            "It is possible that the checks will pass, but the notebook was still run "
-            "out of order. It is highly recommended to move any long-running code to a separate "
-            "task that runs separately from the notebook."
-        )
-
-    if paths:
-        for path in paths:
-            process_path(path, no_run)
-    else:
-        # If no paths are provided, check the current directory
-        process_path(".", no_run)
-
-
-if __name__ == "__main__":  # pragma: no cover
-    cli()
```

### Comparing `enforce_notebook_run_order-1.1.0/src/temp_notebook.py` & `enforce_notebook_run_order-1.3.0/src/enforce_notebook_run_order/temp_notebook.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-"""creates and runs a temporary notebook to verify outputs"""
+"""Creates and runs a temporary notebook to verify outputs"""
 
 import json
 from pathlib import Path
 import shutil
 import subprocess
 import tempfile
+from . import utils
 
 
 class InvalidNotebookJsonError(Exception):
     """
     raised when a notebook fails to run because the provided json is not a valid notebook
     """
 
@@ -16,34 +17,39 @@
 class CellOutputMismatchError(Exception):
     """
     raised when the output of a code cell does not match the expected output
     """
 
 
 class TempNotebook:
-    """creates and runs a temporary notebook to verify outputs"""
+    """Creates and runs a temporary notebook to verify outputs"""
 
     def __init__(self, notebook_data: dict):
         """
         Args:
             notebook_path (Union[str, pathlib.Path]): Path to the notebook file.
         """
         self.notebook_data = notebook_data
         self.temp_dir = Path(tempfile.mkdtemp())
         self.notebook_path = self.temp_dir / "temp_notebook.ipynb"
         self.create_temp_file()
 
     def create_temp_file(self):
-        """creates a temporary notebook file with the given notebook data"""
+        """Creates a temporary notebook file with the given notebook data"""
 
         with open(self.notebook_path, "w", encoding="UTF-8") as notebook_file:
             json.dump(self.notebook_data, notebook_file)
 
     def run(self):
-        """runs the temporary notebook"""
+        """Runs the temporary notebook
+
+        Raises:
+            InvalidNotebookJsonError: if the notebook fails to run because
+                the provided json is not a valid notebook
+        """
         try:
             subprocess.run(
                 [
                     "jupyter",
                     "nbconvert",
                     "--to",
                     "notebook",
@@ -57,46 +63,59 @@
                 f"Notebook {self.notebook_path} failed to run.\n\n"
                 f"Error message: {error}\n\n"
             ) from error
 
         # get the json data from the saved notebook
         # file will be at filename.nbconvert.ipynb
         output_file_path = self.notebook_path.with_suffix(".nbconvert.ipynb")
-        with open(output_file_path, "r", encoding="UTF-8") as output_file:
-            output_data = json.load(output_file)
+        output_data = utils.load_notebook_data(output_file_path)
         return output_data
 
     def compare_outputs(self, output_data: dict):
         """
         compares the outputs of cells of the temporary notebook to the cells
         of the output notebook
+
+        Args:
+            output_data (dict): the output notebook data
+
+        Raises:
+            CellOutputMismatchError: if the output of a cell does not match the expected output
         """
-        for cell_index, cell in enumerate(output_data["cells"]):
-            if cell["cell_type"] == "code":
-                # check that the output cell matches the input cell
-                if (
-                    cell["outputs"]
-                    != self.notebook_data["cells"][cell_index]["outputs"]
-                ):
-                    raise CellOutputMismatchError(
-                        f"Cell #{cell_index} output does not match the expected output.\n\n"
-                        f"Cell contents: \n\n> {cell}"
-                        "Expected output: \n\n> "
-                        f"{self.notebook_data['cells'][cell_index]['outputs']}"
-                    )
+        code_cells = utils.get_code_cells(output_data)
+        # if the first cell has the no-run comment, exit early
+        if utils.cell_has_no_run_comment(code_cells[0]):
+            return
+
+        for cell_index, cell_data in enumerate(code_cells):
+            # if the cell has a no-check-output comment, skip checking it
+            if utils.cell_has_no_check_output_comment(cell_data):
+                continue
+
+            # check that the output cell matches the input cell
+            if (
+                cell_data["outputs"]
+                != self.notebook_data["cells"][cell_index]["outputs"]
+            ):
+                raise CellOutputMismatchError(
+                    f"Cell #{cell_index} output does not match the expected output.\n\n"
+                    f"Cell contents: \n\n> {cell_data}"
+                    "Expected output: \n\n> "
+                    f"{self.notebook_data['cells'][cell_index]['outputs']}"
+                )
 
     def check_notebook(self):
-        """runs the temporary notebook and compares the outputs"""
+        """Runs the temporary notebook and compares the outputs"""
         output_data = self.run()
         self.compare_outputs(output_data)
 
     def __del__(self):
-        """deletes the temporary directory"""
+        """Deletes the temporary directory"""
         shutil.rmtree(self.temp_dir)
 
     def __enter__(self):
-        """returns the path to the temporary notebook"""
+        """Returns the path to the temporary notebook"""
         return self
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
-        """deletes the temporary directory"""
+        """Deletes the temporary directory"""
         del self
```

### Comparing `enforce_notebook_run_order-1.1.0/PKG-INFO` & `enforce_notebook_run_order-1.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enforce-notebook-run-order
-Version: 1.1.0
+Version: 1.3.0
 Summary: 
 License: MIT
 Author: Chris Hacker
 Author-email: 49451910+christopher-hacker@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -78,26 +78,59 @@
 
 Or point it to a directory to check all notebooks in that directory:
 
 ``` {.sourceCode .bash}
 nbcheck my_notebooks/
 ```
 
+If no paths are specified, `nbcheck` will check all notebooks in the
+current directory.
+
 You can also use the full `enforce-notebook-run-order` command, but the
 `nbcheck` command is provided as a convenience.
 
-For information on the command line interface, please refer to the [CLI
-documentation](module_enforce_notebook_run_order.html#command-line-interface).
-
 ### pre-commit hook
 
 To use `enforce_notebook_run_order` as a pre-commit hook, add the
 following to your `.pre-commit-config.yaml`:
 
 ``` {.sourceCode .yaml}
 repos:
 -   repo: https://github.com/christopher-hacker/enforce_notebook_run_order
     rev: 1.0.0
     hooks:
     -   id: enforce-notebook-run-order
 ```
 
+### disabling output checks
+
+By default, `enforce-notebook-run-order` will check that the output of
+each cell matches the output of the previous run. This will catch cases
+where a cell is run out of order, but the execution count is still
+sequential. However, this can be problematic if the output of a cell
+changes between runs, such as when using random numbers. It can also be
+problematic if the notebook runs for a long time.
+
+There are three ways to disable output checks:
+
+1.  Disabling running all notebooks using the `--no-run` flag:
+
+    ``` {.sourceCode .bash}
+    nbcheck --no-run my_notebook.ipynb
+    ```
+
+2.  Disabling running a single notebook using the `no-run` marker **in
+    the first cell of the notebook**:
+
+    > ``` {.sourceCode .python}
+    > # no-run
+    > print("This notebook will not be run")
+    > ```
+
+3.  Disabling output checks for a single cell using the
+    `no-check-output` marker:
+
+    > ``` {.sourceCode .python}
+    > # no-check-output
+    > print("This cell will be run, but its output will not be checked")
+    > ```
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: enforce-notebook-run-order Version: 1.1.0 Summary:
+Metadata-Version: 2.1 Name: enforce-notebook-run-order Version: 1.3.0 Summary:
 License: MIT Author: Chris Hacker Author-email: 49451910+christopher-
 hacker@users.noreply.github.com Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: click
 (>=8.1.3,<9.0.0) Requires-Dist: jupyter (>=1.0.0,<2.0.0) Project-URL: homepage,
@@ -23,15 +23,27 @@
 pre-commit.com/). See the [pre-commit hook](#pre-commit-hook) section for more
 details. Usage ----- `enforce-notebook-run-order` can be used as a standalone
 script, or as a [pre-commit hook](https://pre-commit.com/). ### Standalone To
 use `enforce-notebook-run-order` as a standalone script, simply run it with the
 path to the notebook(s) you want to check: ``` {.sourceCode .bash} nbcheck
 my_notebook.ipynb my_other_notebook.ipynb ``` Or point it to a directory to
 check all notebooks in that directory: ``` {.sourceCode .bash} nbcheck
-my_notebooks/ ``` You can also use the full `enforce-notebook-run-order`
-command, but the `nbcheck` command is provided as a convenience. For
-information on the command line interface, please refer to the [CLI
-documentation](module_enforce_notebook_run_order.html#command-line-interface).
-### pre-commit hook To use `enforce_notebook_run_order` as a pre-commit hook,
-add the following to your `.pre-commit-config.yaml`: ``` {.sourceCode .yaml}
-repos: - repo: https://github.com/christopher-hacker/enforce_notebook_run_order
-rev: 1.0.0 hooks: - id: enforce-notebook-run-order ```
+my_notebooks/ ``` If no paths are specified, `nbcheck` will check all notebooks
+in the current directory. You can also use the full `enforce-notebook-run-
+order` command, but the `nbcheck` command is provided as a convenience. ###
+pre-commit hook To use `enforce_notebook_run_order` as a pre-commit hook, add
+the following to your `.pre-commit-config.yaml`: ``` {.sourceCode .yaml} repos:
+- repo: https://github.com/christopher-hacker/enforce_notebook_run_order rev:
+1.0.0 hooks: - id: enforce-notebook-run-order ``` ### disabling output checks
+By default, `enforce-notebook-run-order` will check that the output of each
+cell matches the output of the previous run. This will catch cases where a cell
+is run out of order, but the execution count is still sequential. However, this
+can be problematic if the output of a cell changes between runs, such as when
+using random numbers. It can also be problematic if the notebook runs for a
+long time. There are three ways to disable output checks: 1. Disabling running
+all notebooks using the `--no-run` flag: ``` {.sourceCode .bash} nbcheck --no-
+run my_notebook.ipynb ``` 2. Disabling running a single notebook using the `no-
+run` marker **in the first cell of the notebook**: > ``` {.sourceCode .python}
+> # no-run > print("This notebook will not be run") > ``` 3. Disabling output
+checks for a single cell using the `no-check-output` marker: > ``` {.sourceCode
+.python} > # no-check-output > print("This cell will be run, but its output
+will not be checked") > ```
```

