# Comparing `tmp/languagemodels-0.2.1.tar.gz` & `tmp/languagemodels-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "languagemodels-0.2.1.tar", last modified: Tue Jun  6 02:17:19 2023, max compression
+gzip compressed data, was "languagemodels-0.2.2.tar", last modified: Tue Jun  6 12:48:41 2023, max compression
```

## Comparing `languagemodels-0.2.1.tar` & `languagemodels-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-06 02:17:19.375507 languagemodels-0.2.1/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     6216 2023-06-06 02:17:19.375507 languagemodels-0.2.1/PKG-INFO
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-06 02:17:19.371507 languagemodels-0.2.1/languagemodels/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     8559 2023-06-06 02:10:02.000000 languagemodels-0.2.1/languagemodels/__init__.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     1384 2023-06-05 16:58:20.000000 languagemodels-0.2.1/languagemodels/embeddings.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     7011 2023-06-06 02:09:50.000000 languagemodels-0.2.1/languagemodels/inference.py
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-06 02:17:19.375507 languagemodels-0.2.1/languagemodels.egg-info/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     6216 2023-06-06 02:17:19.000000 languagemodels-0.2.1/languagemodels.egg-info/PKG-INFO
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      281 2023-06-06 02:17:19.000000 languagemodels-0.2.1/languagemodels.egg-info/SOURCES.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-06-06 02:17:19.000000 languagemodels-0.2.1/languagemodels.egg-info/dependency_links.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       49 2023-06-06 02:17:19.000000 languagemodels-0.2.1/languagemodels.egg-info/requires.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       15 2023-06-06 02:17:19.000000 languagemodels-0.2.1/languagemodels.egg-info/top_level.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-06-06 02:17:19.375507 languagemodels-0.2.1/setup.cfg
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      788 2023-06-06 02:17:06.000000 languagemodels-0.2.1/setup.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-06 12:48:41.980648 languagemodels-0.2.2/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     6295 2023-06-06 12:48:41.980648 languagemodels-0.2.2/PKG-INFO
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-06 12:48:41.976648 languagemodels-0.2.2/languagemodels/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     8559 2023-06-06 02:10:02.000000 languagemodels-0.2.2/languagemodels/__init__.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     1384 2023-06-05 16:58:20.000000 languagemodels-0.2.2/languagemodels/embeddings.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     7183 2023-06-06 12:46:45.000000 languagemodels-0.2.2/languagemodels/inference.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-06 12:48:41.980648 languagemodels-0.2.2/languagemodels.egg-info/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     6295 2023-06-06 12:48:41.000000 languagemodels-0.2.2/languagemodels.egg-info/PKG-INFO
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      281 2023-06-06 12:48:41.000000 languagemodels-0.2.2/languagemodels.egg-info/SOURCES.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-06-06 12:48:41.000000 languagemodels-0.2.2/languagemodels.egg-info/dependency_links.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       49 2023-06-06 12:48:41.000000 languagemodels-0.2.2/languagemodels.egg-info/requires.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       15 2023-06-06 12:48:41.000000 languagemodels-0.2.2/languagemodels.egg-info/top_level.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-06-06 12:48:41.980648 languagemodels-0.2.2/setup.cfg
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      788 2023-06-06 12:48:10.000000 languagemodels-0.2.2/setup.py
```

### Comparing `languagemodels-0.2.1/PKG-INFO` & `languagemodels-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: languagemodels
-Version: 0.2.1
+Version: 0.2.2
 Summary: Simple inference for large language models
 Home-page: https://github.com/jncraton/languagemodels
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: Language Models
         ===============
@@ -129,15 +129,15 @@
         This package will use approximately 5GB of network data to download models initially.
         
         Projects Ideas
         --------------
         
         This package can be used to do the heavy lifting for a number of learning projects:
         
-        - Basic chatbot
+        - [Basic chatbot](https://jncraton-languagemodels-examplesstreamlitchat-g68aa2.streamlit.app/)
         - Chatbot with information retrieval
         - Chatbot with access to real-time information
         - Tool use
         - Text classification
         - Extractive question answering
         - Semantic search
         - Document question answering
```

### Comparing `languagemodels-0.2.1/languagemodels/__init__.py` & `languagemodels-0.2.2/languagemodels/__init__.py`

 * *Files identical despite different names*

### Comparing `languagemodels-0.2.1/languagemodels/embeddings.py` & `languagemodels-0.2.2/languagemodels/embeddings.py`

 * *Files identical despite different names*

### Comparing `languagemodels-0.2.1/languagemodels/inference.py` & `languagemodels-0.2.2/languagemodels/inference.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,34 +10,37 @@
     pass
 
 
 modelcache = {}
 
 
 def list_tokens(prompt):
-    tokenizer_path = hf_hub_download("t5-small", "spiece.model")
-    tokenizer = sentencepiece.SentencePieceProcessor()
-    tokenizer.Load(tokenizer_path)
+    """Generates a list of tokens for a supplied prompt
+
+    >>> list_tokens("Hello, world!")
+    [('▁Hello', 8774), (',', 6), ('▁world', 296), ('!', 55)]
+    """
+    tokenizer, _ = get_model("jncraton/LaMini-Flan-T5-248M-ct2-int8")
 
     tokens = tokenizer.EncodeAsPieces(prompt)
     ids = tokenizer.EncodeAsIds(prompt)
 
     return list(zip(tokens, ids))
 
 
 def generate_ts(engine, prompt, max_tokens=200):
     """Generates a single text response for a prompt from a textsynth server
 
     The server and API key are provided as environment variables:
 
-    ts_server is the server such as http://localhost:8080
-    ts_key is the API key
+    LANGUAGEMODELS_TS_SERVER is the server such as http://localhost:8080
+    LANGUAGEMODELS_TS_KEY is the API key
     """
-    apikey = os.environ.get("ts_key") or ""
-    server = os.environ.get("ts_server") or "https://api.textsynth.com"
+    apikey = os.environ.get("LANGUAGEMODELS_TS_KEY") or ""
+    server = os.environ.get("LANGUAGEMODELS_TS_SERVER") or "https://api.textsynth.com"
 
     response = requests.post(
         f"{server}/v1/engines/{engine}/completions",
         headers={"Authorization": f"Bearer {apikey}"},
         json={"prompt": prompt, "max_tokens": max_tokens},
     )
     resp = response.json()
@@ -48,17 +51,17 @@
 
 
 def generate_oa(engine, prompt, max_tokens=200, temperature=0):
     """Generates a single text response for a prompt using OpenAI
 
     The server and API key are provided as environment variables:
 
-    oa_key is the API key
+    LANGUAGEMODELS_OA_KEY is the API key
     """
-    apikey = os.environ.get("oa_key")
+    apikey = os.environ.get("LANGUAGEMODELS_OA_KEY")
 
     response = requests.post(
         "https://api.openai.com/v1/completions",
         headers={
             "Authorization": f"Bearer {apikey}",
             "Content-Type": "application/json",
         },
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `languagemodels-0.2.1/languagemodels.egg-info/PKG-INFO` & `languagemodels-0.2.2/languagemodels.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: languagemodels
-Version: 0.2.1
+Version: 0.2.2
 Summary: Simple inference for large language models
 Home-page: https://github.com/jncraton/languagemodels
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: Language Models
         ===============
@@ -129,15 +129,15 @@
         This package will use approximately 5GB of network data to download models initially.
         
         Projects Ideas
         --------------
         
         This package can be used to do the heavy lifting for a number of learning projects:
         
-        - Basic chatbot
+        - [Basic chatbot](https://jncraton-languagemodels-examplesstreamlitchat-g68aa2.streamlit.app/)
         - Chatbot with information retrieval
         - Chatbot with access to real-time information
         - Tool use
         - Text classification
         - Extractive question answering
         - Semantic search
         - Document question answering
```

