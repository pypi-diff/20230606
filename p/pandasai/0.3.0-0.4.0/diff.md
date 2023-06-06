# Comparing `tmp/pandasai-0.3.0.tar.gz` & `tmp/pandasai-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.3.0.tar", max compression
+gzip compressed data, was "pandasai-0.4.0.tar", max compression
```

## Comparing `pandasai-0.3.0.tar` & `pandasai-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     1055 2023-04-24 05:55:05.323190 pandasai-0.3.0/LICENSE
--rw-r--r--   0        0        0     8330 2023-05-29 12:51:07.868554 pandasai-0.3.0/README.md
--rw-r--r--   0        0        0    16080 2023-05-29 12:51:07.872906 pandasai-0.3.0/pandasai/__init__.py
--rw-r--r--   0        0        0     1122 2023-05-29 12:51:07.873140 pandasai-0.3.0/pandasai/constants.py
--rw-r--r--   0        0        0      950 2023-05-29 12:51:07.873695 pandasai-0.3.0/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-03 14:53:42.378883 pandasai-0.3.0/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     5347 2023-05-29 12:51:07.874366 pandasai-0.3.0/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0      568 2023-05-29 12:51:07.875099 pandasai-0.3.0/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1487 2023-05-29 12:51:07.875283 pandasai-0.3.0/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     2643 2023-05-29 12:51:07.875419 pandasai-0.3.0/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0        0 2023-04-30 09:49:31.456755 pandasai-0.3.0/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     1493 2023-05-07 12:19:23.603585 pandasai-0.3.0/pandasai/llm/alpaca.py
--rw-r--r--   0        0        0     4325 2023-05-29 12:51:07.876227 pandasai-0.3.0/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    10840 2023-05-29 12:51:07.876513 pandasai-0.3.0/pandasai/llm/base.py
--rw-r--r--   0        0        0      542 2023-05-27 07:25:53.172948 pandasai-0.3.0/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1838 2023-05-29 12:51:07.877290 pandasai-0.3.0/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0     1481 2023-05-29 12:51:07.878110 pandasai-0.3.0/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     2869 2023-05-29 12:51:07.878277 pandasai-0.3.0/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1220 2023-05-29 12:51:07.878427 pandasai-0.3.0/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-05-29 12:51:07.878463 pandasai-0.3.0/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      734 2023-05-29 12:51:07.878751 pandasai-0.3.0/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1786 2023-05-29 12:51:07.878903 pandasai-0.3.0/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1333 2023-05-29 12:51:07.879011 pandasai-0.3.0/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1603 2023-05-29 12:51:07.879149 pandasai-0.3.0/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      505 2023-05-29 12:51:07.879285 pandasai-0.3.0/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1414 2023-05-29 12:51:07.879389 pandasai-0.3.0/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1162 2023-05-29 12:51:26.381317 pandasai-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     9237 1970-01-01 00:00:00.000000 pandasai-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-06-06 00:41:09.700228 pandasai-0.4.0/LICENSE
+-rw-r--r--   0        0        0     8904 2023-06-06 00:41:09.700228 pandasai-0.4.0/README.md
+-rw-r--r--   0        0        0    17831 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/__init__.py
+-rw-r--r--   0        0        0     1678 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/constants.py
+-rw-r--r--   0        0        0     1494 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3774 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5347 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1466 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      566 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1487 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3103 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0        0 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4325 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    10698 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/llm/base.py
+-rw-r--r--   0        0        0      542 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1838 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0     1481 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     2869 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1220 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      734 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1786 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1333 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1603 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      505 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1414 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1457 2023-06-06 00:41:09.708228 pandasai-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     9811 1970-01-01 00:00:00.000000 pandasai-0.4.0/PKG-INFO
```

### Comparing `pandasai-0.3.0/LICENSE` & `pandasai-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.3.0/README.md` & `pandasai-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 pip install pandasai
 ```
 
 ## Usage
 
 > Disclaimer: GDP data was collected from [this source](https://ourworldindata.org/grapher/gross-domestic-product?tab=table), published by World Development Indicators - World Bank (2022.05.26) and collected at National accounts data - World Bank / OECD. It relates to the year of 2020. Happiness indexes were extracted from [the World Happiness Report](https://ftnnews.com/images/stories/documents/2020/WHR20.pdf). Another useful [link](https://data.world/makeovermonday/2020w19-world-happiness-report-2020).
 
-PandasAI is designed to be used in conjunction with [pandas](https://github.com/pandas-dev/pandas). It makes Pandas conversational, allowing you to ask questions about your data and get answers back, in the form of pandas DataFrames. 
+PandasAI is designed to be used in conjunction with [pandas](https://github.com/pandas-dev/pandas). It makes Pandas conversational, allowing you to ask questions about your data and get answers back, in the form of pandas DataFrames.
 
 ### Queries
 
 For example, you can ask PandasAI to find all the rows in a DataFrame where the value of a column is greater than 5, and it will return a DataFrame containing only those rows:
 
 ```python
 import pandas as pd
@@ -51,15 +51,15 @@
     "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
 })
 
 # Instantiate a LLM
 from pandasai.llm.openai import OpenAI
 llm = OpenAI(api_token="YOUR_API_TOKEN")
 
-pandas_ai = PandasAI(llm, conversational=False)
+pandas_ai = PandasAI(llm)
 pandas_ai(df, prompt='Which are the 5 happiest countries?')
 ```
 
 The above code will return the following:
 
 ```
 6            Canada
@@ -131,15 +131,33 @@
 Oh, Olivia gets paid the most.
 ```
 
 You can find more examples in the [examples](examples) directory.
 
 ## Command-Line Tool
 
-Pai is the command line tool designed to provide a convenient way to interact with PandasAI through a command line interface (CLI).
+Pai is the command line tool designed to provide a convenient way to interact with PandasAI through a command line interface (CLI). In order to access the CLI tool, make sure to create a virtualenv for testing purpose and to install project dependencies in your local virtual environment using `pip` by running the following command:
+
+```
+pip install -e .
+```
+
+Alternatively, you can use `poetry` to create and activate the virtual environment by running the following command:
+
+```
+poetry shell
+```
+
+Inside the activated virtual environment, install the project dependencies by running the following command:
+
+```
+poetry install
+```
+
+By following these steps, you will now have the necessary environment to access the CLI tool.
 
 ```
 pai [OPTIONS]
 ```
 
 Options:
```

### Comparing `pandasai-0.3.0/pandasai/__init__.py` & `pandasai-0.4.0/pandasai/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
-""" PandasAI is a wrapper around a LLM to make dataframes conversational
+"""
+PandasAI is a wrapper around a LLM to make dataframes conversational
 
 This module includes the implementation of basis  PandasAI class with methods to run the LLMs
 models on Pandas dataframes. Following LLMs are implemented so far.
 
 Example:
 
     This module is the Entry point of the `pandasai` package. Following is an example of how to
@@ -22,131 +23,143 @@
         "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
     })
 
     # Instantiate a LLM
     from pandasai.llm.openai import OpenAI
     llm = OpenAI(api_token="YOUR_API_TOKEN")
 
-    pandas_ai = PandasAI(llm, conversational=False)
+    pandas_ai = PandasAI(llm)
     pandas_ai(df, prompt='Which are the 5 happiest countries?')
 
     ```
 """
 import ast
 import io
 import re
+import sys
 from contextlib import redirect_stdout
-from typing import Optional
+from typing import Optional, Union
 
 import astor
 import matplotlib.pyplot as plt
 import pandas as pd
 
-from .constants import WHITELISTED_BUILTINS, WHITELISTED_LIBRARIES
-from .exceptions import LLMNotFoundError
+from .constants import (
+    ENVIRONMENT_DEFAULTS,
+    WHITELISTED_BUILTINS,
+    WHITELISTED_LIBRARIES,
+    WHITELISTED_OPTIONAL_LIBRARIES,
+)
+from .exceptions import BadImportError, LLMNotFoundError
+from .helpers._optional import import_optional_dependency
 from .helpers.anonymizer import anonymize_dataframe_head
+from .helpers.cache import Cache
 from .helpers.notebook import Notebook
 from .helpers.save_chart import add_save_chart
 from .llm.base import LLM
 from .prompts.correct_error_prompt import CorrectErrorPrompt
+from .prompts.correct_multiples_prompt import CorrectMultipleDataframesErrorPrompt
 from .prompts.generate_python_code import GeneratePythonCodePrompt
 from .prompts.generate_response import GenerateResponsePrompt
 from .prompts.multiple_dataframes import MultipleDataframesPrompt
-from .prompts.correct_multiples_prompt import CorrectMultipleDataframesErrorPrompt
+
 
 # pylint: disable=too-many-instance-attributes disable=too-many-arguments
 class PandasAI:
-    """PandasAI is a wrapper around a LLM to make dataframes conversational.
+    """
+    PandasAI is a wrapper around a LLM to make dataframes conversational.
 
 
-    This is a an entry point of `pandasai` object. This class consists of methods to interface the
-    LLMs with Pandas     dataframes. A pandas dataframe metadata i.e df.head() and prompt is
+    This is an entry point of `pandasai` object. This class consists of methods to interface the
+    LLMs with Pandas     dataframes. A pandas dataframe metadata i.e. df.head() and prompt is
     passed on to chosen LLMs API end point to     generate a Python code to answer the questions
     asked. The resultant python code is run on actual data and answer is converted into a
     conversational form.
 
     Note:
         Do not include the `self` parameter in the ``Args`` section.
     Args:
         _llm (obj): LLMs option to be used for API access
-        _verbose (bool, optional): To show the intermediate outputs e.g python code
+        _verbose (bool, optional): To show the intermediate outputs e.g. python code
         generated and execution step on the prompt. Default to False
         _is_conversational_answer (bool, optional): Whether to return answer in conversational
         form. Default to False
         _enforce_privacy (bool, optional): Do not display the data on prompt in case of
         Sensitive data. Default to False
         _max_retries (int, optional): max no. of tries to generate code on failure. Default to 3
         _is_notebook (bool, optional): Whether to run code in notebook. Default to False
         _original_instructions (dict, optional): The dict of instruction to run. Default to None
         last_code_generated (str, optional): Pass last Code if generated. Default to None
         last_run_code (str, optional): Pass the last execution / run. Default to None
         code_output (str, optional): The code output if any. Default to None
         last_error (str, optional): Error of running code last time. Default to None
 
 
-    Returns:
-        response (str): Returns the Response to a Question related to Data
+    Returns (str): Response to a Question related to Data
 
     """
 
     _llm: LLM
     _verbose: bool = False
-    _is_conversational_answer: bool = True
+    _is_conversational_answer: bool = False
     _enforce_privacy: bool = False
     _max_retries: int = 3
     _is_notebook: bool = False
     _original_instructions: dict = {
         "question": None,
         "df_head": None,
         "num_rows": None,
         "num_columns": None,
         "rows_to_display": None,
     }
+    _cache: Cache = Cache()
+    _enable_cache: bool = True
     last_code_generated: Optional[str] = None
     last_run_code: Optional[str] = None
     code_output: Optional[str] = None
     last_error: Optional[str] = None
 
-
-
     def __init__(
         self,
         llm=None,
-        conversational=True,
+        conversational=False,
         verbose=False,
         enforce_privacy=False,
         save_charts=False,
+        enable_cache=True,
     ):
         """
 
         __init__ method of the Class PandasAI
 
         Args:
             llm (object): LLMs option to be used for API access. Default is None
-            conversational (bool): Whether to return answer in conversational form. Default to True
-            verbose (bool): To show the intermediate outputs e.g python code generated and
+            conversational (bool): Whether to return answer in conversational form. Default to False
+            verbose (bool): To show the intermediate outputs e.g. python code generated and
              execution step on the prompt.  Default to False
             enforce_privacy (bool): Execute the codes with Privacy Mode ON.  Default to False
+            save_charts (bool): Save the charts generated in the notebook. Default to False
         """
         if llm is None:
             raise LLMNotFoundError(
                 "An LLM should be provided to instantiate a PandasAI instance"
             )
         self._llm = llm
         self._is_conversational_answer = conversational
         self._verbose = verbose
         self._enforce_privacy = enforce_privacy
         self._save_charts = save_charts
+        self._enable_cache = enable_cache
 
         self.notebook = Notebook()
         self._in_notebook = self.notebook.in_notebook()
 
     def conversational_answer(self, question: str, answer: str) -> str:
-
-        """Returns the answer in conversational form about the resultant data.
+        """
+        Returns the answer in conversational form about the resultant data.
 
         Args:
             question (str): A question in Conversational form
             answer (str): A summary / resultant Data
 
         Returns (str): Response
 
@@ -164,92 +177,99 @@
         self,
         data_frame: pd.DataFrame,
         prompt: str,
         is_conversational_answer: bool = None,
         show_code: bool = False,
         anonymize_df: bool = True,
         use_error_correction_framework: bool = True,
-    ) -> str:
+    ) -> Union[str, pd.DataFrame]:
         """
         Run the PandasAI to make Dataframes Conversational.
 
         Args:
             data_frame (pd.Dataframe): A pandas Dataframe
             prompt (str): A prompt to query about the Dataframe
             is_conversational_answer (bool): Whether to return answer in conversational form.
             Default to False
             show_code (bool): To show the intermediate python code generated on the prompt.
             Default to False
             anonymize_df (bool): Running the code with Sensitive Data. Default to True
             use_error_correction_framework (bool): Turn on Error Correction mechanism.
             Default to True
 
-        Returns: Answer to the Input Questions about the DataFrame
+        Returns (str): Answer to the Input Questions about the DataFrame
 
         """
 
         self.log(f"Running PandasAI with {self._llm.type} LLM...")
 
         try:
-            rows_to_display = 0 if self._enforce_privacy else 5
-
-            multiple: bool = isinstance(data_frame, list)
+            if self._enable_cache and self._cache.get(prompt):
+                self.log("Using cached response")
+                code = self._cache.get(prompt)
+            else:
+                rows_to_display = 0 if self._enforce_privacy else 5
 
-            if multiple:
+                multiple: bool = isinstance(data_frame, list)
 
-                heads = [anonymize_dataframe_head(dataframe)
+                if multiple:
+                    heads = [
+                        anonymize_dataframe_head(dataframe)
                         if anonymize_df
                         else dataframe.head(rows_to_display)
-                        for dataframe in data_frame]
+                        for dataframe in data_frame
+                    ]
 
-                code = self._llm.generate_code(
-                    MultipleDataframesPrompt(dataframes=heads),
-                    prompt,
-                )
-
-                self._original_instructions = {
-                    "question": prompt,
-                    "df_head": heads,
-                    "rows_to_display": rows_to_display,
-                }
+                    code = self._llm.generate_code(
+                        MultipleDataframesPrompt(dataframes=heads),
+                        prompt,
+                    )
 
-            else:
+                    self._original_instructions = {
+                        "question": prompt,
+                        "df_head": heads,
+                        "rows_to_display": rows_to_display,
+                    }
+
+                else:
+                    df_head = data_frame.head(rows_to_display)
+                    if anonymize_df:
+                        df_head = anonymize_dataframe_head(df_head)
+
+                    code = self._llm.generate_code(
+                        GeneratePythonCodePrompt(
+                            prompt=prompt,
+                            df_head=df_head,
+                            num_rows=data_frame.shape[0],
+                            num_columns=data_frame.shape[1],
+                            rows_to_display=rows_to_display,
+                        ),
+                        prompt,
+                    )
 
-                df_head = data_frame.head(rows_to_display)
-                if anonymize_df:
-                    df_head = anonymize_dataframe_head(df_head)
-
-                code = self._llm.generate_code(
-                    GeneratePythonCodePrompt(
-                        prompt=prompt,
-                        df_head=df_head,
-                        num_rows=data_frame.shape[0],
-                        num_columns=data_frame.shape[1],
-                        rows_to_display=rows_to_display,
-                    ),
-                    prompt,
+                    self._original_instructions = {
+                        "question": prompt,
+                        "df_head": df_head,
+                        "num_rows": data_frame.shape[0],
+                        "num_columns": data_frame.shape[1],
+                        "rows_to_display": rows_to_display,
+                    }
+
+                self.last_code_generated = code
+                self.log(
+                    f"""
+                        Code generated:
+                        ```
+                        {code}
+                        ```
+                    """
                 )
 
-                self._original_instructions = {
-                    "question": prompt,
-                    "df_head": df_head,
-                    "num_rows": data_frame.shape[0],
-                    "num_columns": data_frame.shape[1],
-                    "rows_to_display": rows_to_display,
-                }
-
-            self.last_code_generated = code
-            self.log(
-                f"""
-                    Code generated:
-                    ```
-                    {code}
-                    ```
-                """
-            )
+                self._cache.set(prompt, code)
+
             if show_code and self._in_notebook:
                 self.notebook.create_new_cell(code)
 
             answer = self.run_code(
                 code,
                 data_frame,
                 use_error_correction_framework=use_error_correction_framework,
@@ -267,153 +287,171 @@
             self.last_error = str(exception)
             return (
                 "Unfortunately, I was not able to answer your question, "
                 "because of the following error:\n"
                 f"\n{exception}\n"
             )
 
+    def clear_cache(self):
+        """
+        Clears the cache of the PandasAI instance.
+        """
+        self._cache.clear()
+
     def __call__(
         self,
         data_frame: pd.DataFrame,
         prompt: str,
         is_conversational_answer: bool = None,
         show_code: bool = False,
         anonymize_df: bool = True,
         use_error_correction_framework: bool = True,
-    ) -> str:
+    ) -> Union[str, pd.DataFrame]:
         """
-        __call__ method of PandasAI class. It call `run` method
+        __call__ method of PandasAI class. It calls the `run` method.
+
         Args:
             data_frame:
             prompt:
             is_conversational_answer:
             show_code:
             anonymize_df:
             use_error_correction_framework:
 
-        Returns:
+        Returns (str): Answer to the Input Questions about the DataFrame.
 
         """
 
         return self.run(
             data_frame,
             prompt,
             is_conversational_answer,
             show_code,
             anonymize_df,
             use_error_correction_framework,
         )
 
-    def is_unsafe_import(self, node: ast.stmt) -> bool:
-
-        """Remove non-whitelisted imports from the code to prevent malicious code execution
+    def _is_unsafe_import(self, node: ast.stmt) -> bool:
+        """
+        Remove non-whitelisted imports from the code to prevent malicious code execution
 
         Args:
             node (object): ast.stmt
 
         Returns (bool): A flag if unsafe_imports found.
 
         """
 
-        return isinstance(node, (ast.Import, ast.ImportFrom)) and any(
-            alias.name not in WHITELISTED_LIBRARIES for alias in node.names
-        )
+        if isinstance(node, (ast.Import, ast.ImportFrom)):
+            for alias in node.names:
+                if (
+                    alias.name in WHITELISTED_BUILTINS
+                    or alias.name in ENVIRONMENT_DEFAULTS
+                ):
+                    return True
+                if alias.name in WHITELISTED_OPTIONAL_LIBRARIES:
+                    import_optional_dependency(alias.name)
+                    continue
+                if alias.name.split(".")[0] not in WHITELISTED_LIBRARIES:
+                    raise BadImportError(alias.name)
 
-    def is_df_overwrite(self, node: ast.stmt) -> str:
+        return False
 
+    def _is_df_overwrite(self, node: ast.stmt) -> bool:
         """
         Remove df declarations from the code to prevent malicious code execution. A helper method.
+
         Args:
             node (object): ast.stmt
 
-        Returns (str):
+        Returns (bool):
 
         """
 
         return (
             isinstance(node, ast.Assign)
             and isinstance(node.targets[0], ast.Name)
             and re.match(r"df\d{0,2}$", node.targets[0].id)
         )
 
-    def clean_code(self, code: str) -> str:
-
+    def _clean_code(self, code: str) -> str:
         """
         A method to clean the code to prevent malicious code execution
+
         Args:
             code(str): A python code
 
         Returns (str): Returns a Clean Code String
 
         """
 
         tree = ast.parse(code)
 
         new_body = [
             node
             for node in tree.body
-            if not (self.is_unsafe_import(node) or self.is_df_overwrite(node))
+            if not (self._is_unsafe_import(node) or self._is_df_overwrite(node))
         ]
 
         new_tree = ast.Module(body=new_body)
         return astor.to_source(new_tree).strip()
 
     def run_code(
         self,
         code: str,
         data_frame: pd.DataFrame,
         use_error_correction_framework: bool = True,
     ) -> str:
         """
         A method to execute the python code generated by LLMs to answer the question about the
         input dataframe. Run the code in the current context and return the result.
+
         Args:
             code (str): A python code to execute
             data_frame (pd.DataFrame): A full Pandas DataFrame
             use_error_correction_framework (bool): Turn on Error Correction mechanism.
             Default to True
 
-        Returns:
+        Returns (str): String representation of the result of the code execution.
 
         """
 
         # pylint: disable=W0122 disable=W0123 disable=W0702:bare-except
 
         multiple: bool = isinstance(data_frame, list)
 
         # Add save chart code
         if self._save_charts:
             code = add_save_chart(code)
 
         # Get the code to run removing unsafe imports and df overwrites
-        code_to_run = self.clean_code(code)
+        code_to_run = self._clean_code(code)
         self.last_run_code = code_to_run
         self.log(
             f"""
 Code running:
 ```
 {code_to_run}
 ```"""
         )
 
         environment: dict = {
-            "pd": pd,
-            "plt": plt,
+            **{
+                alias: sys.modules[library]
+                for library, alias in ENVIRONMENT_DEFAULTS.items()
+            },
             "__builtins__": {
-                **{
-                    builtin: __builtins__[builtin]
-                    for builtin in WHITELISTED_BUILTINS
-                },
+                **{builtin: __builtins__[builtin] for builtin in WHITELISTED_BUILTINS},
             },
         }
 
         if multiple:
-            environment.update({
-                f"df{i}": dataframe for i, dataframe in enumerate(data_frame, start = 1)
-            })
+            environment.update(
+                {f"df{i}": dataframe for i, dataframe in enumerate(data_frame, start=1)}
+            )
 
         else:
             environment["df"] = data_frame
 
         # Redirect standard output to a StringIO buffer
         with redirect_stdout(io.StringIO()) as output:
             count = 0
@@ -426,30 +464,34 @@
                 except Exception as e:  # pylint: disable=W0718 disable=C0103
                     if not use_error_correction_framework:
                         raise e
 
                     count += 1
 
                     if multiple:
-                        error_correcting_instruction = CorrectMultipleDataframesErrorPrompt(
-                            code=code,
-                            error_returned=e,
-                            question=self._original_instructions["question"],
-                            df_head=self._original_instructions["df_head"],
+                        error_correcting_instruction = (
+                            CorrectMultipleDataframesErrorPrompt(
+                                code=code,
+                                error_returned=e,
+                                question=self._original_instructions["question"],
+                                df_head=self._original_instructions["df_head"],
+                            )
                         )
 
                     else:
                         error_correcting_instruction = CorrectErrorPrompt(
                             code=code,
                             error_returned=e,
                             question=self._original_instructions["question"],
                             df_head=self._original_instructions["df_head"],
                             num_rows=self._original_instructions["num_rows"],
                             num_columns=self._original_instructions["num_columns"],
-                            rows_to_display=self._original_instructions["rows_to_display"],
+                            rows_to_display=self._original_instructions[
+                                "rows_to_display"
+                            ],
                         )
 
                     code_to_run = self._llm.generate_code(
                         error_correcting_instruction, ""
                     )
 
         captured_output = output.getvalue()
```

### Comparing `pandasai-0.3.0/pandasai/helpers/anonymizer.py` & `pandasai-0.4.0/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.3.0/pandasai/helpers/from_excel.py` & `pandasai-0.4.0/pandasai/helpers/from_excel.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-
-""" Helper Module to Handle Data
+"""
+Helper Module to Handle Data
 This module collects the helper function on handling various Data Sources.
 
-
 """
 from __future__ import annotations
 
 import pandas as pd
 
 
 def from_excel(file, sheet: str | int | None = 0) -> pd.DataFrame:
-
     """
     Return a pandas DataFrame from an Excel file.
     Wrapper for pandas.read_excel().
+
     Args:
         file (str):  A file path to be read
         sheet (str | int): Name of the sheet or Sheet No. Default is 0
 
     Returns (pd.DataFrame): A Pandas Dataframe
 
     """
```

### Comparing `pandasai-0.3.0/pandasai/helpers/notebook.py` & `pandasai-0.4.0/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.3.0/pandasai/helpers/save_chart.py` & `pandasai-0.4.0/pandasai/helpers/save_chart.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,16 +10,28 @@
 
 
 def compare_ast(
     node1: Union[ast.expr, list[ast.expr], ast.stmt, ast.AST],
     node2: Union[ast.expr, list[ast.expr], ast.stmt, ast.AST],
     ignore_args=False,
 ) -> bool:
-    """Compare two AST nodes for equality.
-    Source: https://stackoverflow.com/a/66733795/11080806"""
+    """
+    Compare two AST nodes for equality.
+    Source: https://stackoverflow.com/a/66733795/11080806
+
+    Args:
+        node1 (ast.AST): First AST node to compare.
+        node2 (ast.AST): Second AST node to compare.
+        ignore_args (bool, optional): Whether to ignore the arguments of the nodes.
+            Defaults to False.
+
+    Returns:
+        bool: True if the nodes are equal, False otherwise.
+
+    """
     if type(node1) is not type(node2):
         return False
 
     if isinstance(node1, ast.AST):
         for k, node in vars(node1).items():
             if k in {"lineno", "end_lineno", "col_offset", "end_col_offset", "ctx"}:
                 continue
@@ -34,47 +46,55 @@
             compare_ast(n1, n2, ignore_args) for n1, n2 in zip_longest(node1, node2)
         )
 
     return node1 == node2
 
 
 def add_save_chart(code: str) -> str:
-    """Add line to code that save charts to a file, if plt.show() is called."""
-    date = datetime.now().strftime("%Y-%m-%d")
-    timestamp = datetime.now().strftime("%Y-%m-%d-%H-%M-%S")
+    """
+    Add line to code that save charts to a file, if plt.show() is called.
 
-    # define chart save directory
-    project_root = dirname(dirname(dirname(__file__)))
-    chart_save_dir = os.path.join(project_root, f"exports\\charts\\{date}")
-    if not os.path.exists(chart_save_dir):
-        os.makedirs(chart_save_dir)
+    Args:
+        code (str): Code to add line to.
+
+    Returns:
+        str: Code with line added.
 
+    """
+    date = datetime.now().strftime("%Y-%m-%d")
+    timestamp = datetime.now().strftime("%Y-%m-%d-%H-%M-%S")
     tree = ast.parse(code)
 
     # count number of plt.show() calls
     show_count = sum(
         compare_ast(node, ast.parse("plt.show()").body[0], ignore_args=True)
         for node in ast.walk(tree)
     )
 
     # if there are no plt.show() calls, return the original code
     if show_count == 0:
         return code
 
+    # define chart save directory
+    project_root = dirname(dirname(dirname(__file__)))
+    chart_save_dir = os.path.join(project_root, "exports", "charts", date)
+    if not os.path.exists(chart_save_dir):
+        os.makedirs(chart_save_dir)
+
     # iterate through the AST and add plt.savefig() calls before plt.show() calls
     counter = ord("a")
     new_body = []
     for node in tree.body:
         if compare_ast(node, ast.parse("plt.show()").body[0], ignore_args=True):
             filename = f"chart_{timestamp}"
             if show_count > 1:
                 filename += f"_{chr(counter)}"
                 counter += 1
-            new_body.append(
-                ast.parse(f"plt.savefig(r'{chart_save_dir}\\{filename}.png')")
-            )
+
+            chart_save_path = os.path.join(chart_save_dir, f"{filename}.png")
+            new_body.append(ast.parse(f"plt.savefig(r'{chart_save_path}')"))
         new_body.append(node)
 
     new_body.append(ast.parse(f"print(r'Charts saved to: {chart_save_dir}')"))
 
     new_tree = ast.Module(body=new_body)
     return astor.to_source(new_tree).strip()
```

### Comparing `pandasai-0.3.0/pandasai/llm/azure_openai.py` & `pandasai-0.4.0/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.3.0/pandasai/llm/base.py` & `pandasai-0.4.0/pandasai/llm/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 from ..constants import END_CODE_TAG, START_CODE_TAG
 from ..exceptions import (
     APIKeyNotFoundError,
     MethodNotImplementedError,
     NoCodeFoundError,
 )
+from ..helpers._optional import import_optional_dependency
 from ..prompts.base import Prompt
 
 
 class LLM:
     """Base class to implement a new LLM."""
 
     last_prompt: Optional[str] = None
@@ -148,15 +149,14 @@
     max_tokens: int = 512
     top_p: float = 1
     frequency_penalty: float = 0
     presence_penalty: float = 0.6
     stop: Optional[str] = None
 
     def _set_params(self, **kwargs):
-
         """
         Set Parameters
         Args:
             **kwargs: ["model", "engine", "deployment_id", "temperature","max_tokens",
             "top_p", "frequency_penalty", "presence_penalty", "stop", ]
 
         Returns: None
@@ -176,15 +176,14 @@
         ]
         for key, value in kwargs.items():
             if key in valid_params:
                 setattr(self, key, value)
 
     @property
     def _default_params(self) -> Dict[str, Any]:
-
         """
         Get the default parameters for calling OpenAI API
 
         Returns (Dict): A dict of OpenAi API parameters
 
         """
 
@@ -274,15 +273,14 @@
         response = requests.post(
             self._api_url, headers=headers, json=payload, timeout=60
         )
 
         return response.json()[0]["generated_text"]
 
     def call(self, instruction: Prompt, value: str, suffix: str = "") -> str:
-
         """
         A call method of HuggingFaceLLM class.
         Args:
             instruction (object): A prompt object
             value (str):
             suffix (str):
 
@@ -305,15 +303,15 @@
         output = response.replace(prompt + value + suffix, "")
         return output
 
 
 class BaseGoogle(LLM):
     """Base class to implement a new Google LLM
 
-     LLM base class is extended to be used with Google Palm API.
+    LLM base class is extended to be used with Google Palm API.
     """
 
     genai: Any
     temperature: Optional[float] = 0
     top_p: Optional[float] = None
     top_k: Optional[float] = None
     max_output_tokens: Optional[int] = None
@@ -326,24 +324,19 @@
 
         Returns:
 
         """
 
         if not api_key:
             raise APIKeyNotFoundError("Google Palm API key is required")
-        try:
-            # pylint: disable=import-outside-toplevel
-            import google.generativeai as genai
 
-            genai.configure(api_key=api_key)
-        except ImportError as ex:
-            raise ImportError(
-                "Could not import google-generativeai python package. "
-                "Please install it with `pip install google-generativeai`."
-            ) from ex
+        err_msg = "Install google-generativeai >= 0.1 for Google Palm API"
+        genai = import_optional_dependency("google.generativeai", extra=err_msg)
+
+        genai.configure(api_key=api_key)
         self.genai = genai
 
     def _valid_params(self):
         return ["temperature", "top_p", "top_k", "max_output_tokens"]
 
     def _set_params(self, **kwargs):
         """
```

### Comparing `pandasai-0.3.0/pandasai/llm/fake.py` & `pandasai-0.4.0/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.3.0/pandasai/llm/google_palm.py` & `pandasai-0.4.0/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.3.0/pandasai/llm/open_assistant.py` & `pandasai-0.4.0/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.3.0/pandasai/llm/openai.py` & `pandasai-0.4.0/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.3.0/pandasai/llm/starcoder.py` & `pandasai-0.4.0/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.3.0/pandasai/prompts/base.py` & `pandasai-0.4.0/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.3.0/pandasai/prompts/correct_error_prompt.py` & `pandasai-0.4.0/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.3.0/pandasai/prompts/correct_multiples_prompt.py` & `pandasai-0.4.0/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.3.0/pandasai/prompts/generate_python_code.py` & `pandasai-0.4.0/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.3.0/pandasai/prompts/multiple_dataframes.py` & `pandasai-0.4.0/pandasai/prompts/multiple_dataframes.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.3.0/pyproject.toml` & `pandasai-0.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.3.0"
+version = "0.4.0"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
@@ -27,14 +27,21 @@
 pytest-mock = "^3.10.0"
 pytest-env = "^0.8.1"
 click = "^8.1.3"
 
 [tool.poetry.extras]
 google = ["google-generativeai"]
 
+[tool.poetry.group.whitelist.dependencies]
+statsmodels = {version = "^0.14.0", optional = true}
+scikit-learn = {version = "^1.2.2", optional = true}
+seaborn = {version = "^0.12.2", optional = true}
+plotly = {version = "^5.14.1", optional = true}
+ggplot = {version = "^0.11.5", optional = true}
+
 [tool.poetry.group.docs.dependencies]
 mkdocs = "1.4.0"
 mkdocstrings-python = "0.7.1"
 markdown-include = "^0.6.0"
 
 [tool.poetry.scripts]
 pai = "pai.__main__:main"
```

### Comparing `pandasai-0.3.0/PKG-INFO` & `pandasai-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.3.0
+Version: 0.4.0
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -52,15 +52,15 @@
 pip install pandasai
 ```
 
 ## Usage
 
 > Disclaimer: GDP data was collected from [this source](https://ourworldindata.org/grapher/gross-domestic-product?tab=table), published by World Development Indicators - World Bank (2022.05.26) and collected at National accounts data - World Bank / OECD. It relates to the year of 2020. Happiness indexes were extracted from [the World Happiness Report](https://ftnnews.com/images/stories/documents/2020/WHR20.pdf). Another useful [link](https://data.world/makeovermonday/2020w19-world-happiness-report-2020).
 
-PandasAI is designed to be used in conjunction with [pandas](https://github.com/pandas-dev/pandas). It makes Pandas conversational, allowing you to ask questions about your data and get answers back, in the form of pandas DataFrames. 
+PandasAI is designed to be used in conjunction with [pandas](https://github.com/pandas-dev/pandas). It makes Pandas conversational, allowing you to ask questions about your data and get answers back, in the form of pandas DataFrames.
 
 ### Queries
 
 For example, you can ask PandasAI to find all the rows in a DataFrame where the value of a column is greater than 5, and it will return a DataFrame containing only those rows:
 
 ```python
 import pandas as pd
@@ -73,15 +73,15 @@
     "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
 })
 
 # Instantiate a LLM
 from pandasai.llm.openai import OpenAI
 llm = OpenAI(api_token="YOUR_API_TOKEN")
 
-pandas_ai = PandasAI(llm, conversational=False)
+pandas_ai = PandasAI(llm)
 pandas_ai(df, prompt='Which are the 5 happiest countries?')
 ```
 
 The above code will return the following:
 
 ```
 6            Canada
@@ -153,15 +153,33 @@
 Oh, Olivia gets paid the most.
 ```
 
 You can find more examples in the [examples](examples) directory.
 
 ## Command-Line Tool
 
-Pai is the command line tool designed to provide a convenient way to interact with PandasAI through a command line interface (CLI).
+Pai is the command line tool designed to provide a convenient way to interact with PandasAI through a command line interface (CLI). In order to access the CLI tool, make sure to create a virtualenv for testing purpose and to install project dependencies in your local virtual environment using `pip` by running the following command:
+
+```
+pip install -e .
+```
+
+Alternatively, you can use `poetry` to create and activate the virtual environment by running the following command:
+
+```
+poetry shell
+```
+
+Inside the activated virtual environment, install the project dependencies by running the following command:
+
+```
+poetry install
+```
+
+By following these steps, you will now have the necessary environment to access the CLI tool.
 
 ```
 pai [OPTIONS]
 ```
 
 Options:
```

