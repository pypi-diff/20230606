# Comparing `tmp/notebook_copilot-0.1.1.tar.gz` & `tmp/notebook_copilot-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notebook_copilot-0.1.1.tar", last modified: Sun Jun  4 23:46:51 2023, max compression
+gzip compressed data, was "notebook_copilot-0.1.4.tar", last modified: Tue Jun  6 21:22:02 2023, max compression
```

## Comparing `notebook_copilot-0.1.1.tar` & `notebook_copilot-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 tp         (501) staff       (20)        0 2023-06-04 23:46:51.959344 notebook_copilot-0.1.1/
--rw-r--r--   0 tp         (501) staff       (20)     2827 2023-06-04 23:46:51.959217 notebook_copilot-0.1.1/PKG-INFO
--rw-r--r--   0 tp         (501) staff       (20)     2536 2023-06-04 23:34:52.000000 notebook_copilot-0.1.1/README.md
-drwxr-xr-x   0 tp         (501) staff       (20)        0 2023-06-04 23:46:51.958197 notebook_copilot-0.1.1/notebook_copilot/
--rw-r--r--   0 tp         (501) staff       (20)       52 2023-05-26 01:34:01.000000 notebook_copilot-0.1.1/notebook_copilot/__init__.py
--rw-r--r--   0 tp         (501) staff       (20)     1678 2023-06-03 00:21:02.000000 notebook_copilot-0.1.1/notebook_copilot/agents.py
--rw-r--r--   0 tp         (501) staff       (20)     1300 2023-06-03 23:50:52.000000 notebook_copilot-0.1.1/notebook_copilot/chains.py
--rw-r--r--   0 tp         (501) staff       (20)     1944 2023-06-03 01:01:52.000000 notebook_copilot-0.1.1/notebook_copilot/context.py
--rw-r--r--   0 tp         (501) staff       (20)     4554 2023-06-03 23:28:59.000000 notebook_copilot-0.1.1/notebook_copilot/notebook_copilot.py
--rw-r--r--   0 tp         (501) staff       (20)     2469 2023-06-03 23:53:58.000000 notebook_copilot-0.1.1/notebook_copilot/output.py
--rw-r--r--   0 tp         (501) staff       (20)     2775 2023-06-03 23:49:21.000000 notebook_copilot-0.1.1/notebook_copilot/prompts.py
--rw-r--r--   0 tp         (501) staff       (20)     2430 2023-06-03 23:30:56.000000 notebook_copilot-0.1.1/notebook_copilot/tools.py
--rw-r--r--   0 tp         (501) staff       (20)      316 2023-06-01 20:58:10.000000 notebook_copilot-0.1.1/notebook_copilot/utils.py
-drwxr-xr-x   0 tp         (501) staff       (20)        0 2023-06-04 23:46:51.959019 notebook_copilot-0.1.1/notebook_copilot.egg-info/
--rw-r--r--   0 tp         (501) staff       (20)     2827 2023-06-04 23:46:51.000000 notebook_copilot-0.1.1/notebook_copilot.egg-info/PKG-INFO
--rw-r--r--   0 tp         (501) staff       (20)      472 2023-06-04 23:46:51.000000 notebook_copilot-0.1.1/notebook_copilot.egg-info/SOURCES.txt
--rw-r--r--   0 tp         (501) staff       (20)        1 2023-06-04 23:46:51.000000 notebook_copilot-0.1.1/notebook_copilot.egg-info/dependency_links.txt
--rw-r--r--   0 tp         (501) staff       (20)      118 2023-06-04 23:46:51.000000 notebook_copilot-0.1.1/notebook_copilot.egg-info/requires.txt
--rw-r--r--   0 tp         (501) staff       (20)       17 2023-06-04 23:46:51.000000 notebook_copilot-0.1.1/notebook_copilot.egg-info/top_level.txt
--rw-r--r--   0 tp         (501) staff       (20)       38 2023-06-04 23:46:51.959386 notebook_copilot-0.1.1/setup.cfg
--rw-r--r--   0 tp         (501) staff       (20)      673 2023-06-04 23:46:49.000000 notebook_copilot-0.1.1/setup.py
+drwxr-xr-x   0 tp         (501) staff       (20)        0 2023-06-06 21:22:02.907738 notebook_copilot-0.1.4/
+-rw-r--r--   0 tp         (501) staff       (20)     1059 2023-06-05 01:38:02.000000 notebook_copilot-0.1.4/LICENSE
+-rw-r--r--   0 tp         (501) staff       (20)     4068 2023-06-06 21:22:02.907618 notebook_copilot-0.1.4/PKG-INFO
+-rw-r--r--   0 tp         (501) staff       (20)     3529 2023-06-05 02:20:23.000000 notebook_copilot-0.1.4/README.md
+drwxr-xr-x   0 tp         (501) staff       (20)        0 2023-06-06 21:22:02.906180 notebook_copilot-0.1.4/notebook_copilot/
+-rw-r--r--   0 tp         (501) staff       (20)       52 2023-05-26 01:34:01.000000 notebook_copilot-0.1.4/notebook_copilot/__init__.py
+-rw-r--r--   0 tp         (501) staff       (20)     1678 2023-06-03 00:21:02.000000 notebook_copilot-0.1.4/notebook_copilot/agents.py
+-rw-r--r--   0 tp         (501) staff       (20)     1296 2023-06-05 01:04:00.000000 notebook_copilot-0.1.4/notebook_copilot/chains.py
+-rw-r--r--   0 tp         (501) staff       (20)     1944 2023-06-03 01:01:52.000000 notebook_copilot-0.1.4/notebook_copilot/context.py
+-rw-r--r--   0 tp         (501) staff       (20)     4554 2023-06-03 23:28:59.000000 notebook_copilot-0.1.4/notebook_copilot/notebook_copilot.py
+-rw-r--r--   0 tp         (501) staff       (20)     2469 2023-06-03 23:53:58.000000 notebook_copilot-0.1.4/notebook_copilot/output.py
+-rw-r--r--   0 tp         (501) staff       (20)     2775 2023-06-03 23:49:21.000000 notebook_copilot-0.1.4/notebook_copilot/prompts.py
+-rw-r--r--   0 tp         (501) staff       (20)     2328 2023-06-05 01:34:26.000000 notebook_copilot-0.1.4/notebook_copilot/tools.py
+-rw-r--r--   0 tp         (501) staff       (20)      316 2023-06-01 20:58:10.000000 notebook_copilot-0.1.4/notebook_copilot/utils.py
+drwxr-xr-x   0 tp         (501) staff       (20)        0 2023-06-06 21:22:02.907111 notebook_copilot-0.1.4/notebook_copilot.egg-info/
+-rw-r--r--   0 tp         (501) staff       (20)     4068 2023-06-06 21:22:02.000000 notebook_copilot-0.1.4/notebook_copilot.egg-info/PKG-INFO
+-rw-r--r--   0 tp         (501) staff       (20)      520 2023-06-06 21:22:02.000000 notebook_copilot-0.1.4/notebook_copilot.egg-info/SOURCES.txt
+-rw-r--r--   0 tp         (501) staff       (20)        1 2023-06-06 21:22:02.000000 notebook_copilot-0.1.4/notebook_copilot.egg-info/dependency_links.txt
+-rw-r--r--   0 tp         (501) staff       (20)      118 2023-06-06 21:22:02.000000 notebook_copilot-0.1.4/notebook_copilot.egg-info/requires.txt
+-rw-r--r--   0 tp         (501) staff       (20)       23 2023-06-06 21:22:02.000000 notebook_copilot-0.1.4/notebook_copilot.egg-info/top_level.txt
+-rw-r--r--   0 tp         (501) staff       (20)       38 2023-06-06 21:22:02.907776 notebook_copilot-0.1.4/setup.cfg
+-rw-r--r--   0 tp         (501) staff       (20)      927 2023-06-06 21:21:59.000000 notebook_copilot-0.1.4/setup.py
+drwxr-xr-x   0 tp         (501) staff       (20)        0 2023-06-06 21:22:02.907396 notebook_copilot-0.1.4/tests/
+-rw-r--r--   0 tp         (501) staff       (20)        0 2023-06-05 00:27:43.000000 notebook_copilot-0.1.4/tests/__init__.py
+-rw-r--r--   0 tp         (501) staff       (20)     2129 2023-06-05 01:15:45.000000 notebook_copilot-0.1.4/tests/test_copilot.py
```

### Comparing `notebook_copilot-0.1.1/PKG-INFO` & `notebook_copilot-0.1.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,78 +1,86 @@
-Metadata-Version: 2.1
-Name: notebook_copilot
-Version: 0.1.1
-Summary: The Bridge from Thoughts to Well-Crafted Jupyter Notebook
-Home-page: https://github.com/talperetz/notebook_copilot
-Author: Tal Peretz
-Author-email: tp@aihumanlabs.com
-License: MIT
-Description-Content-Type: text/markdown
-
-# 🚀 Notebook Copilot: From Thoughts to Well-Crafted Code at Record-Speed.
+# 🚀 Notebook Copilot: From Thoughts to Well-Crafted Notebook at Record-Speed. 
 
 Welcome to Notebook Copilot, your next-generation tool for Jupyter Notebooks. Inspired by GitHub Copilot, Notebook
 Copilot is designed to help engineers and data scientists in developing professional, high-quality notebooks. It's like
 having your personal AI-powered assistant that helps you navigate through the Jupyter universe, seamlessly
 generating code and markdown cells based on your inputs.
 
 Imagine not having to start with a blank notebook every time. Sounds dreamy, right?
 
-## Demo
-<div><iframe src="https://www.loom.com/embed/d347052d3403412083cf4ea75b2e2cd4" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe></div>
+<h2 align="center"> v1 Demo </h2>
 
-## Key Features
 
-- **`%copilot` magic function**: Continues the notebook for you, generating professional code and markdown cells, making
-  blank notebooks a thing of the past.
-- **`%generate` magic function**: Utilizes AI to generate the next cell from your comments. Just give it a hint, and
-  it'll do the heavy lifting for you.
-- **`%explain` magic function**: Produces a markdown cell that elaborates the functionality of the current cell. Don't
-  just write code, understand it thoroughly!
+https://github.com/talperetz/notebook-copilot/assets/11588598/02e2b030-adb3-42f2-bd6d-4a8451e3831f
+
+
+## Features
+
+- 🚀 GPT Based Generation: Notebook Copilot employs advanced GPT instances for precise and efficient code generation.
+- 💻 Integrated with Any Notebook Environments: Seamless access within Jupyter Notebook and other popular platforms, boosting your productivity.
+- 🧩 Automatic Context Retrieval: Understands the full context of your notebook, ensuring consistent and relevant code generation.
+- 🔑 Bring Your Own OpenAI Key: Flexibility to use your own OpenAI key for personalized code generation and optimal results.
+- 🆓 Free and Open Source: Everyone can benefit from Notebook Copilot. It's our contribution to the coding community, aiming to make coding accessible, efficient, and fun.
 
-## Installation
 
-You can install Notebook Copilot directly from PyPI:
+## Quickstart
+0. Get an OpenAI [API Key](https://platform.openai.com/account/api-keys)
+1. Install Notebook Copilot directly from PyPI:
 
 ```bash
 pip install notebook_copilot
 ```
 
-## Usage
-Load the Notebook Copilot extension in your Jupyter notebook:
+2. Load the Notebook Copilot extension in your Jupyter notebook:
 
 ```python
 %load_ext notebook_copilot
+
+# Optional: If you don't have OPENAI_API_KEY set in your environment, you can set it here
+from getpass import getpass
+import os
+os.environ["OPENAI_API_KEY"] = getpass("Enter your OpenAI Key: ")
+
+%copilot_init -n /Users/tp/dev/workspace/notebook_copilot/copilot_example_notebook.ipynb # improves copilot performance
 ```
 
-Now you're ready to use the magic functions:
+3. Start using Notebook Copilot Magic Functions in your notebook ↓
+
 
+## ✨ Magic Functions
+
+🪄 Enter Assistant Mode and let Copilot continuously generate professional code and markdown cells for you.
 ```python
-# Enter Assistant Mode, will continue the notebook for you
 %copilot
 ```
 
+✍️ Leverage AI to create the next cell from your comments. It's like having a conversation with your notebook.
+
 ```python
-# Generate the next cell code
-%%generate plot the confusion matrix using for the model
+%%generate 
+# Plot the confusion matrix using for the model
 ```
 
+📘 Automatically generate markdown cells to explain the code in the current cell. Your code is now not only functional but also well-documented.
 ```python
-# Explain the current cell
 %%explain
-# some code…
+# some code to explain…
 ```
 
 ## Roadmap
 
 - [x] **Copilot Magic Function**: Continues the notebook for you, generating professional code and markdown cells, making
   blank notebooks a thing of the past.
 - [x] **Generate Magic Function**: Turn Your Comments into Code
 - [x] **Explain Magic Function**: Generate Markdown Cells that Explain Your Code
-- [ ] Update underlying strategy to ToT
+- [ ] Support parallel cell generation
+- [ ] Update underlying strategy and prompts
+- [ ] Support more llm providers
+  - [ ] Starcoder
+  - [ ] Anthropic
 - [ ] AI-Powered Code completion inside cells
     
 
 ## Contributing
 We appreciate all contributions. If you're planning to contribute back bug-fixes, please do so without any further discussion. If you plan to contribute new features, utility functions, or extensions to the core, please first open an issue and discuss the feature with us.
 
 ## License
```

### Comparing `notebook_copilot-0.1.1/notebook_copilot/agents.py` & `notebook_copilot-0.1.4/notebook_copilot/agents.py`

 * *Files identical despite different names*

### Comparing `notebook_copilot-0.1.1/notebook_copilot/chains.py` & `notebook_copilot-0.1.4/notebook_copilot/chains.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,8 +27,8 @@
     output = chain.predict(run_history=run_history, cell=cell)
     return multiple_cells_completion_parser.parse(output)
 
 
 def explain_cell_completion(llm, run_history, cell=None) -> str:
     """Get a markdown explanation for current cell"""
     chain = LLMChain(llm=llm, prompt=markdown_explain_prompt_template)
-    return chain.run({'run_history': run_history, 'cell': cell})
+    return chain.predict(run_history=run_history, cell=cell)
```

### Comparing `notebook_copilot-0.1.1/notebook_copilot/context.py` & `notebook_copilot-0.1.4/notebook_copilot/context.py`

 * *Files identical despite different names*

### Comparing `notebook_copilot-0.1.1/notebook_copilot/notebook_copilot.py` & `notebook_copilot-0.1.4/notebook_copilot/notebook_copilot.py`

 * *Files identical despite different names*

### Comparing `notebook_copilot-0.1.1/notebook_copilot/output.py` & `notebook_copilot-0.1.4/notebook_copilot/output.py`

 * *Files identical despite different names*

### Comparing `notebook_copilot-0.1.1/notebook_copilot/prompts.py` & `notebook_copilot-0.1.4/notebook_copilot/prompts.py`

 * *Files identical despite different names*

### Comparing `notebook_copilot-0.1.1/notebook_copilot/tools.py` & `notebook_copilot-0.1.4/notebook_copilot/tools.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from notebook_copilot.context import get_ipython_run_history
 from notebook_copilot.output import generate_notebook_cell_below
 from notebook_copilot.prompts import CellType, CellCompletion
 
 
 class NewCodeCellTool(BaseTool):
-    # todo: change this to support multiple cells.
     name = "Notebook New Code Cell"
     description = (
         "use this tool when you want to create a new Code cell in the notebook. "
         "To use the tool you must provide the following parameter: 'content' (string)"
     )
 
     def _run(
@@ -23,15 +22,14 @@
         generate_notebook_cell_below(CellCompletion(type=CellType.CODE, content=content))
 
     def _arun(self, query: str):
         raise NotImplementedError("This tool does not support async")
 
 
 class NewMarkdownCellTool(BaseTool):
-    # todo: change this to support multiple cells.
     name = "Notebook New Markdown Cell"
     description = (
         "use this tool when you want to create a new Markdown cell in the notebook. "
         "To use the tool you must provide the following parameter: 'content' (string)."
     )
 
     def _run(
```

