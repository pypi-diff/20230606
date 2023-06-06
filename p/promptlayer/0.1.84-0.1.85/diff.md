# Comparing `tmp/promptlayer-0.1.84.tar.gz` & `tmp/promptlayer-0.1.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/promptlayer-0.1.84.tar", last modified: Tue May 30 03:06:09 2023, max compression
+gzip compressed data, was "dist/promptlayer-0.1.85.tar", last modified: Tue Jun  6 13:58:25 2023, max compression
```

## Comparing `promptlayer-0.1.84.tar` & `promptlayer-0.1.85.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-30 03:06:09.097950 promptlayer-0.1.84/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    11357 2023-01-26 22:51:29.000000 promptlayer-0.1.84/LICENSE
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5046 2023-05-30 03:06:09.097504 promptlayer-0.1.84/PKG-INFO
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3891 2023-01-26 22:51:29.000000 promptlayer-0.1.84/README.md
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-30 03:06:09.084355 promptlayer-0.1.84/promptlayer/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      888 2023-05-30 02:39:06.000000 promptlayer-0.1.84/promptlayer/__init__.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-30 03:06:09.093012 promptlayer-0.1.84/promptlayer/langchain/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        0 2023-02-01 20:15:14.000000 promptlayer-0.1.84/promptlayer/langchain/__init__.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-30 03:06:09.094205 promptlayer-0.1.84/promptlayer/langchain/llms/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       26 2023-02-01 20:08:36.000000 promptlayer-0.1.84/promptlayer/langchain/llms/__init__.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     2012 2023-02-15 16:07:17.000000 promptlayer-0.1.84/promptlayer/langchain/llms/openai.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3141 2023-05-30 02:39:06.000000 promptlayer-0.1.84/promptlayer/promptlayer.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-30 03:06:09.095447 promptlayer-0.1.84/promptlayer/prompts/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      124 2023-02-16 22:50:19.000000 promptlayer-0.1.84/promptlayer/prompts/__init__.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1285 2023-03-31 18:02:42.000000 promptlayer-0.1.84/promptlayer/prompts/prompts.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-30 03:06:09.096711 promptlayer-0.1.84/promptlayer/track/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       59 2023-03-13 20:43:03.000000 promptlayer-0.1.84/promptlayer/track/__init__.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1239 2023-05-12 18:10:56.000000 promptlayer-0.1.84/promptlayer/track/track.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    13445 2023-05-24 19:31:54.000000 promptlayer-0.1.84/promptlayer/utils.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-30 03:06:09.091879 promptlayer-0.1.84/promptlayer.egg-info/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5046 2023-05-30 03:06:09.000000 promptlayer-0.1.84/promptlayer.egg-info/PKG-INFO
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      502 2023-05-30 03:06:09.000000 promptlayer-0.1.84/promptlayer.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        1 2023-05-30 03:06:09.000000 promptlayer-0.1.84/promptlayer.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       19 2023-05-30 03:06:09.000000 promptlayer-0.1.84/promptlayer.egg-info/requires.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       12 2023-05-30 03:06:09.000000 promptlayer-0.1.84/promptlayer.egg-info/top_level.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       38 2023-05-30 03:06:09.098099 promptlayer-0.1.84/setup.cfg
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      837 2023-05-30 03:05:33.000000 promptlayer-0.1.84/setup.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-06 13:58:25.103383 promptlayer-0.1.85/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    11357 2023-01-26 22:51:29.000000 promptlayer-0.1.85/LICENSE
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5046 2023-06-06 13:58:25.103041 promptlayer-0.1.85/PKG-INFO
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3891 2023-01-26 22:51:29.000000 promptlayer-0.1.85/README.md
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-06 13:58:25.096910 promptlayer-0.1.85/promptlayer/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      888 2023-05-30 02:39:06.000000 promptlayer-0.1.85/promptlayer/__init__.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-06 13:58:25.100072 promptlayer-0.1.85/promptlayer/langchain/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        0 2023-02-01 20:15:14.000000 promptlayer-0.1.85/promptlayer/langchain/__init__.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-06 13:58:25.100997 promptlayer-0.1.85/promptlayer/langchain/llms/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       26 2023-02-01 20:08:36.000000 promptlayer-0.1.85/promptlayer/langchain/llms/__init__.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     2012 2023-02-15 16:07:17.000000 promptlayer-0.1.85/promptlayer/langchain/llms/openai.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3141 2023-05-30 02:39:06.000000 promptlayer-0.1.85/promptlayer/promptlayer.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-06 13:58:25.101926 promptlayer-0.1.85/promptlayer/prompts/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      124 2023-02-16 22:50:19.000000 promptlayer-0.1.85/promptlayer/prompts/__init__.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1740 2023-06-06 13:57:37.000000 promptlayer-0.1.85/promptlayer/prompts/chat.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1700 2023-06-06 13:57:37.000000 promptlayer-0.1.85/promptlayer/prompts/prompts.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-06 13:58:25.102554 promptlayer-0.1.85/promptlayer/track/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       59 2023-03-13 20:43:03.000000 promptlayer-0.1.85/promptlayer/track/__init__.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1239 2023-05-12 18:10:56.000000 promptlayer-0.1.85/promptlayer/track/track.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    13445 2023-05-24 19:31:54.000000 promptlayer-0.1.85/promptlayer/utils.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-06 13:58:25.099607 promptlayer-0.1.85/promptlayer.egg-info/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5046 2023-06-06 13:58:25.000000 promptlayer-0.1.85/promptlayer.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      530 2023-06-06 13:58:25.000000 promptlayer-0.1.85/promptlayer.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        1 2023-06-06 13:58:25.000000 promptlayer-0.1.85/promptlayer.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       19 2023-06-06 13:58:25.000000 promptlayer-0.1.85/promptlayer.egg-info/requires.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       12 2023-06-06 13:58:25.000000 promptlayer-0.1.85/promptlayer.egg-info/top_level.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       38 2023-06-06 13:58:25.103496 promptlayer-0.1.85/setup.cfg
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      837 2023-06-06 13:57:40.000000 promptlayer-0.1.85/setup.py
```

### Comparing `promptlayer-0.1.84/LICENSE` & `promptlayer-0.1.85/LICENSE`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.84/PKG-INFO` & `promptlayer-0.1.85/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptlayer
-Version: 0.1.84
+Version: 0.1.85
 Summary: PromptLayer is a package to keep track of your GPT models training
 Home-page: https://www.promptlayer.com
 Author: Magniv
 Author-email: hello@magniv.io
 License: UNKNOWN
 Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: promptlayer Version: 0.1.84 Summary: PromptLayer is
+Metadata-Version: 2.1 Name: promptlayer Version: 0.1.85 Summary: PromptLayer is
 a package to keep track of your GPT models training Home-page: https://
 www.promptlayer.com Author: Magniv Author-email: hello@magniv.io License:
 UNKNOWN Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-
 Docs-db0e6f50cacf4564a6d09824ba17a629 Description:
 # ð° PromptLayer **The first platform built for prompt engineers** [Python]
                           [Docs] [Demo_with_Loom] ---
 [PromptLayer](https://promptlayer.com/) is the first platform that allows you
```

### Comparing `promptlayer-0.1.84/README.md` & `promptlayer-0.1.85/README.md`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.84/promptlayer/__init__.py` & `promptlayer-0.1.85/promptlayer/__init__.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.84/promptlayer/langchain/llms/openai.py` & `promptlayer-0.1.85/promptlayer/langchain/llms/openai.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.84/promptlayer/promptlayer.py` & `promptlayer-0.1.85/promptlayer/promptlayer.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.84/promptlayer/prompts/prompts.py` & `promptlayer-0.1.85/promptlayer/prompts/prompts.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,41 @@
-from langchain import PromptTemplate
+from langchain import PromptTemplate, prompts
 from langchain.prompts.loading import load_prompt_from_config
 
-from promptlayer.utils import (get_api_key, promptlayer_get_prompt,
-                               promptlayer_publish_prompt)
+from promptlayer.prompts.chat import CHAT_PROMPTLAYER_LANGCHAIN, to_dict, to_prompt
+from promptlayer.utils import (
+    get_api_key,
+    promptlayer_get_prompt,
+    promptlayer_publish_prompt,
+)
 
 
 def get_prompt(prompt_name, langchain=False, version=None):
     """
     Get a prompt template from PromptLayer.
     version: The version of the prompt to get. If not specified, the latest version will be returned.
     """
     api_key = get_api_key()
     prompt = promptlayer_get_prompt(prompt_name, api_key, version)
     if langchain:
         if "_type" not in prompt["prompt_template"]:
             prompt["prompt_template"]["_type"] = "prompt"
+        elif prompt["prompt_template"]["_type"] == CHAT_PROMPTLAYER_LANGCHAIN:
+            return to_prompt(prompt["prompt_template"])
         return load_prompt_from_config(prompt["prompt_template"])
     else:
         return prompt["prompt_template"]
 
 
 def publish_prompt(prompt_name, tags=[], prompt_template=None):
     api_key = get_api_key()
     if type(prompt_template) == dict:
         promptlayer_publish_prompt(prompt_name, prompt_template, tags, api_key)
+    elif isinstance(prompt_template, prompts.ChatPromptTemplate):
+        prompt_template_dict = to_dict(prompt_template)
+        promptlayer_publish_prompt(prompt_name, prompt_template_dict, tags, api_key)
     elif isinstance(prompt_template, PromptTemplate):
-        promptlayer_publish_prompt(
-            prompt_name, prompt_template.dict(), tags, api_key)
+        promptlayer_publish_prompt(prompt_name, prompt_template.dict(), tags, api_key)
     else:
         raise Exception(
-            "Please provide either a JSON prompt template or a langchain prompt template.")
+            "Please provide either a JSON prompt template or a langchain prompt template."
+        )
```

### Comparing `promptlayer-0.1.84/promptlayer/track/track.py` & `promptlayer-0.1.85/promptlayer/track/track.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.84/promptlayer/utils.py` & `promptlayer-0.1.85/promptlayer/utils.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.84/promptlayer.egg-info/PKG-INFO` & `promptlayer-0.1.85/promptlayer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptlayer
-Version: 0.1.84
+Version: 0.1.85
 Summary: PromptLayer is a package to keep track of your GPT models training
 Home-page: https://www.promptlayer.com
 Author: Magniv
 Author-email: hello@magniv.io
 License: UNKNOWN
 Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: promptlayer Version: 0.1.84 Summary: PromptLayer is
+Metadata-Version: 2.1 Name: promptlayer Version: 0.1.85 Summary: PromptLayer is
 a package to keep track of your GPT models training Home-page: https://
 www.promptlayer.com Author: Magniv Author-email: hello@magniv.io License:
 UNKNOWN Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-
 Docs-db0e6f50cacf4564a6d09824ba17a629 Description:
 # ð° PromptLayer **The first platform built for prompt engineers** [Python]
                           [Docs] [Demo_with_Loom] ---
 [PromptLayer](https://promptlayer.com/) is the first platform that allows you
```

### Comparing `promptlayer-0.1.84/setup.py` & `promptlayer-0.1.85/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,12 +16,12 @@
     long_description_content_type="text/markdown",
     author="Magniv",
     author_email="hello@magniv.io",
     url="https://www.promptlayer.com",
     project_urls={
         "Documentation": "https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629",
     },
-    version="0.1.84",
+    version="0.1.85",
     py_modules=["promptlayer"],
     packages=find_packages(),
     install_requires=["requests", "langchain"],
 )
```

