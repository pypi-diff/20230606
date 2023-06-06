# Comparing `tmp/languagemodels-0.1.2.tar.gz` & `tmp/languagemodels-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "languagemodels-0.1.2.tar", last modified: Mon Jun  5 17:01:32 2023, max compression
+gzip compressed data, was "languagemodels-0.2.1.tar", last modified: Tue Jun  6 02:17:19 2023, max compression
```

## Comparing `languagemodels-0.1.2.tar` & `languagemodels-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-05 17:01:32.532605 languagemodels-0.1.2/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     6060 2023-06-05 17:01:32.532605 languagemodels-0.1.2/PKG-INFO
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-05 17:01:32.528605 languagemodels-0.1.2/languagemodels/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     8050 2023-06-05 16:58:20.000000 languagemodels-0.1.2/languagemodels/__init__.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     1384 2023-06-05 16:58:20.000000 languagemodels-0.1.2/languagemodels/embeddings.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     6128 2023-06-05 16:58:20.000000 languagemodels-0.1.2/languagemodels/inference.py
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-05 17:01:32.532605 languagemodels-0.1.2/languagemodels.egg-info/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     6060 2023-06-05 17:01:32.000000 languagemodels-0.1.2/languagemodels.egg-info/PKG-INFO
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      281 2023-06-05 17:01:32.000000 languagemodels-0.1.2/languagemodels.egg-info/SOURCES.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-06-05 17:01:32.000000 languagemodels-0.1.2/languagemodels.egg-info/dependency_links.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       49 2023-06-05 17:01:32.000000 languagemodels-0.1.2/languagemodels.egg-info/requires.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       15 2023-06-05 17:01:32.000000 languagemodels-0.1.2/languagemodels.egg-info/top_level.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-06-05 17:01:32.532605 languagemodels-0.1.2/setup.cfg
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      788 2023-06-05 17:01:21.000000 languagemodels-0.1.2/setup.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-06 02:17:19.375507 languagemodels-0.2.1/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     6216 2023-06-06 02:17:19.375507 languagemodels-0.2.1/PKG-INFO
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-06 02:17:19.371507 languagemodels-0.2.1/languagemodels/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     8559 2023-06-06 02:10:02.000000 languagemodels-0.2.1/languagemodels/__init__.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     1384 2023-06-05 16:58:20.000000 languagemodels-0.2.1/languagemodels/embeddings.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     7011 2023-06-06 02:09:50.000000 languagemodels-0.2.1/languagemodels/inference.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-06 02:17:19.375507 languagemodels-0.2.1/languagemodels.egg-info/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     6216 2023-06-06 02:17:19.000000 languagemodels-0.2.1/languagemodels.egg-info/PKG-INFO
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      281 2023-06-06 02:17:19.000000 languagemodels-0.2.1/languagemodels.egg-info/SOURCES.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-06-06 02:17:19.000000 languagemodels-0.2.1/languagemodels.egg-info/dependency_links.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       49 2023-06-06 02:17:19.000000 languagemodels-0.2.1/languagemodels.egg-info/requires.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       15 2023-06-06 02:17:19.000000 languagemodels-0.2.1/languagemodels.egg-info/top_level.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-06-06 02:17:19.375507 languagemodels-0.2.1/setup.cfg
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      788 2023-06-06 02:17:06.000000 languagemodels-0.2.1/setup.py
```

### Comparing `languagemodels-0.1.2/PKG-INFO` & `languagemodels-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: languagemodels
-Version: 0.1.2
+Version: 0.2.1
 Summary: Simple inference for large language models
 Home-page: https://github.com/jncraton/languagemodels
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: Language Models
         ===============
         
         [![PyPI version](https://badge.fury.io/py/languagemodels.svg)](https://badge.fury.io/py/languagemodels)
         [![docs](https://img.shields.io/badge/docs-online-brightgreen)](https://languagemodels.netlify.app/)
         [![Build](https://github.com/jncraton/languagemodels/actions/workflows/build.yml/badge.svg)](https://github.com/jncraton/languagemodels/actions/workflows/build.yml)
         [![Netlify Status](https://api.netlify.com/api/v1/badges/722e625a-c6bc-4373-bd88-c017adc58c00/deploy-status)](https://app.netlify.com/sites/languagemodels/deploys)
         [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jncraton/languagemodels/blob/master/examples/translate.ipynb)
+        [![Try with Replit Badge](https://replit.com/badge?caption=Try%20with%20Replit&variant=small)](https://replit.com/@jncraton/langaugemodels#main.py)
         
         A Python package providing simple building blocks for exploring natural language processing.
         
         ![Translation hello world example](media/hello.gif)
         
         Target Audience
         ---------------
```

### Comparing `languagemodels-0.1.2/languagemodels/__init__.py` & `languagemodels-0.2.1/languagemodels/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import datetime
 import json
 
-from languagemodels.inference import generate_instruct, convert_chat, list_tokens
+from languagemodels.inference import generate_instruct, parse_chat, list_tokens
 from languagemodels.embeddings import RetrievalContext
 
 docs = RetrievalContext()
 
 
 def print_tokens(prompt: str) -> None:
     """Prints a list of tokens in a prompt
@@ -81,45 +81,79 @@
 def chat(prompt: str) -> str:
     """Get new message from chat-optimized language model
 
     The `prompt` for this model is provided as a series of messages as a single
     plain-text string. Several special tokens are used to delineate chat
     messages.
 
-    - `<|system|>` - Indicates the start of a system message providing
+    - `system:` - Indicates the start of a system message providing
     instructions about how the assistant should behave.
-    - `<|prompter|>` - Indicates the start of a prompter (typically user)
+    - `user:` - Indicates the start of a prompter (typically user)
     message.
-    - `<|assistant|>` - Indicates the start of an assistant message.
-    - `<|endoftext|>` - Used to terminal all message types.
+    - `assistant:` - Indicates the start of an assistant message.
 
     A complete prompt may look something like this:
 
     ```
-    <|system|>Assistant is helpful and harmless<|endoftext|>
-    <|prompter|>What is the capital of Germany?<|endoftext|>
-    <|assistant|>The capital of Germany is Berlin.<|endoftext|>
-    <|prompter|>How many people live there?<|endoftext|>
-    <|assistant|>
+    Assistant is helpful and harmless
+
+    User: What is the capital of Germany?
+
+    Assistant: The capital of Germany is Berlin.
+
+    User: How many people live there?
+
+    Assistant:
     ```
 
     The completion from the language model is returned.
 
     :param message: Prompt using formatting described above
     :return: Completion returned from the language model
 
-    >>> chat("<|system|>It is 5:15pm. Assistant is helpful<|endoftext|>" \\
-    ...      "<|prompter|>What time is it?<|endoftext|>" \\
-    ...      "<|assistant|>")
-    '5:15pm.'
-    """
-
-    prompt = convert_chat(prompt)
+    >>> chat('''
+    ...      System: It is 5:15pm. Assistant is helpful.
+    ...
+    ...      User: What time is it?
+    ...
+    ...      Assistant:
+    ...      ''')
+    '...5:15pm...'
+    """
+
+    messages = parse_chat(prompt)
+
+    # Suppress starts of all assistant messages to avoid repeat generation
+    suppress = [
+        "Assistant: " + m["content"].split(" ")[0]
+        for m in messages
+        if m["role"] == "assistant"
+    ]
+
+    messages = [f"{m['role'].title()}: {m['content']}" for m in messages]
+
+    prompt = "\n\n".join(messages)
+
+    if prompt.startswith("System:"):
+        prompt = prompt[7:].strip()
+
+    response = generate_instruct(
+        prompt,
+        max_tokens=200,
+        repetition_penalty=1.3,
+        temperature=0.7,
+        prefix="Assistant: ",
+        suppress=suppress,
+    )
+
+    # Remove duplicate assistant being generated
+    if response.startswith("Assistant:"):
+        response = response[10:]
 
-    return generate_instruct(prompt, max_tokens=200)
+    return response.strip()
 
 
 def extract_answer(question: str, context: str) -> str:
     """Extract an answer to a `question` from a provided `context`
 
     The returned answer will always be a substring extracted from `context`.
     It may not always be a correct or meaningful answer, but it will never be
@@ -193,19 +227,19 @@
 
     This function ignores the complexity of disambiguation pages and simply
     returns the first result that is not a disambiguation page
 
     :param topic: Topic to search for on Wikipedia
     :return: Text content of the lead section of the most popular matching article
 
-    >>> fetch_wiki('Python') # doctest: +ELLIPSIS
-    'Python is a high-level...
+    >>> fetch_wiki('Python')
+    'Python is a high-level...'
 
-    >>> fetch_wiki('Chemistry') # doctest: +ELLIPSIS
-    'Chemistry is the scientific study...
+    >>> fetch_wiki('Chemistry')
+    'Chemistry is the scientific study...'
     """
 
     url = "https://api.wikimedia.org/core/v1/wikipedia/en/search/title"
     response = requests.get(url, params={"q": topic, "limit": 5})
     response = json.loads(response.text)
 
     for page in response["pages"]:
```

### Comparing `languagemodels-0.1.2/languagemodels/embeddings.py` & `languagemodels-0.2.1/languagemodels/embeddings.py`

 * *Files identical despite different names*

### Comparing `languagemodels-0.1.2/languagemodels.egg-info/PKG-INFO` & `languagemodels-0.2.1/languagemodels.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: languagemodels
-Version: 0.1.2
+Version: 0.2.1
 Summary: Simple inference for large language models
 Home-page: https://github.com/jncraton/languagemodels
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: Language Models
         ===============
         
         [![PyPI version](https://badge.fury.io/py/languagemodels.svg)](https://badge.fury.io/py/languagemodels)
         [![docs](https://img.shields.io/badge/docs-online-brightgreen)](https://languagemodels.netlify.app/)
         [![Build](https://github.com/jncraton/languagemodels/actions/workflows/build.yml/badge.svg)](https://github.com/jncraton/languagemodels/actions/workflows/build.yml)
         [![Netlify Status](https://api.netlify.com/api/v1/badges/722e625a-c6bc-4373-bd88-c017adc58c00/deploy-status)](https://app.netlify.com/sites/languagemodels/deploys)
         [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jncraton/languagemodels/blob/master/examples/translate.ipynb)
+        [![Try with Replit Badge](https://replit.com/badge?caption=Try%20with%20Replit&variant=small)](https://replit.com/@jncraton/langaugemodels#main.py)
         
         A Python package providing simple building blocks for exploring natural language processing.
         
         ![Translation hello world example](media/hello.gif)
         
         Target Audience
         ---------------
```

### Comparing `languagemodels-0.1.2/setup.py` & `languagemodels-0.2.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="languagemodels",
-    version="0.1.2",
+    version="0.2.1",
     author="Jon Craton",
     author_email="jon@joncraton.com",
     description="Simple inference for large language models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jncraton/languagemodels",
     packages=setuptools.find_packages(),
```

