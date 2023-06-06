# Comparing `tmp/alphawave-0.1.0.tar.gz` & `tmp/alphawave-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphawave-0.1.0.tar", last modified: Mon Jun  5 23:40:50 2023, max compression
+gzip compressed data, was "alphawave-0.1.1.tar", last modified: Tue Jun  6 01:34:18 2023, max compression
```

## Comparing `alphawave-0.1.0.tar` & `alphawave-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-05 23:40:50.613758 alphawave-0.1.0/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.1.0/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      670 2023-06-05 23:40:50.613758 alphawave-0.1.0/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       57 2023-06-05 21:20:34.000000 alphawave-0.1.0/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      837 2023-06-05 23:40:25.000000 alphawave-0.1.0/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-05 23:40:50.613758 alphawave-0.1.0/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-05 23:40:50.613758 alphawave-0.1.0/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-05 23:40:50.613758 alphawave-0.1.0/src/alphawave/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    10089 2023-06-05 02:02:06.000000 alphawave-0.1.0/src/alphawave/AlphaWave.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1207 2023-06-04 00:33:26.000000 alphawave-0.1.0/src/alphawave/Colorize.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      701 2023-06-04 23:38:31.000000 alphawave-0.1.0/src/alphawave/DefaultResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1890 2023-06-03 23:06:34.000000 alphawave-0.1.0/src/alphawave/JSONResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1963 2023-06-03 23:22:26.000000 alphawave-0.1.0/src/alphawave/MemoryForkTest.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6799 2023-06-04 16:26:58.000000 alphawave-0.1.0/src/alphawave/OSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7514 2023-06-05 18:36:51.000000 alphawave-0.1.0/src/alphawave/OpenAIClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2301 2023-06-03 23:24:45.000000 alphawave-0.1.0/src/alphawave/Response.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14731 2023-06-04 03:49:37.000000 alphawave-0.1.0/src/alphawave/TestAlphaWave.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      850 2023-06-04 03:32:15.000000 alphawave-0.1.0/src/alphawave/TestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1485 2023-06-03 23:57:30.000000 alphawave-0.1.0/src/alphawave/TestClientTest.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1914 2023-06-05 18:40:59.000000 alphawave-0.1.0/src/alphawave/alphaChat.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1311 2023-06-04 00:58:56.000000 alphawave-0.1.0/src/alphawave/alphawaveTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.1.0/src/alphawave/internalTypes.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-05 23:40:50.613758 alphawave-0.1.0/src/alphawave.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      670 2023-06-05 23:40:50.000000 alphawave-0.1.0/src/alphawave.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      671 2023-06-05 23:40:50.000000 alphawave-0.1.0/src/alphawave.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-05 23:40:50.000000 alphawave-0.1.0/src/alphawave.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       81 2023-06-05 23:40:50.000000 alphawave-0.1.0/src/alphawave.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       10 2023-06-05 23:40:50.000000 alphawave-0.1.0/src/alphawave.egg-info/top_level.txt
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-05 23:40:50.613758 alphawave-0.1.0/tests/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14712 2023-06-05 18:15:14.000000 alphawave-0.1.0/tests/testOpenAiClient.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-06 01:34:18.981710 alphawave-0.1.1/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.1.1/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      670 2023-06-06 01:34:18.981710 alphawave-0.1.1/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       57 2023-06-05 21:20:34.000000 alphawave-0.1.1/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      837 2023-06-06 01:33:47.000000 alphawave-0.1.1/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-06 01:34:18.981710 alphawave-0.1.1/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-06 01:34:18.981710 alphawave-0.1.1/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-06 01:34:18.981710 alphawave-0.1.1/src/alphawave/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    10171 2023-06-06 01:27:21.000000 alphawave-0.1.1/src/alphawave/AlphaWave.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1207 2023-06-04 00:33:26.000000 alphawave-0.1.1/src/alphawave/Colorize.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      711 2023-06-06 01:24:12.000000 alphawave-0.1.1/src/alphawave/DefaultResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1900 2023-06-06 01:24:39.000000 alphawave-0.1.1/src/alphawave/JSONResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      545 2023-06-03 22:27:04.000000 alphawave-0.1.1/src/alphawave/MemoryFork.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6799 2023-06-04 16:26:58.000000 alphawave-0.1.1/src/alphawave/OSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7556 2023-06-06 01:29:30.000000 alphawave-0.1.1/src/alphawave/OpenAIClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2301 2023-06-03 23:24:45.000000 alphawave-0.1.1/src/alphawave/Response.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14771 2023-06-06 01:26:17.000000 alphawave-0.1.1/src/alphawave/TestAlphaWave.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      860 2023-06-06 01:26:32.000000 alphawave-0.1.1/src/alphawave/TestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1505 2023-06-06 01:26:50.000000 alphawave-0.1.1/src/alphawave/TestClientTest.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1914 2023-06-05 18:40:59.000000 alphawave-0.1.1/src/alphawave/alphaChat.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1311 2023-06-04 00:58:56.000000 alphawave-0.1.1/src/alphawave/alphawaveTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.1.1/src/alphawave/internalTypes.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-06 01:34:18.981710 alphawave-0.1.1/src/alphawave.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      670 2023-06-06 01:34:18.000000 alphawave-0.1.1/src/alphawave.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      667 2023-06-06 01:34:18.000000 alphawave-0.1.1/src/alphawave.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-06 01:34:18.000000 alphawave-0.1.1/src/alphawave.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       81 2023-06-06 01:34:18.000000 alphawave-0.1.1/src/alphawave.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       10 2023-06-06 01:34:18.000000 alphawave-0.1.1/src/alphawave.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-06 01:34:18.981710 alphawave-0.1.1/tests/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14712 2023-06-05 18:15:14.000000 alphawave-0.1.1/tests/testOpenAiClient.py
```

### Comparing `alphawave-0.1.0/LICENSE` & `alphawave-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.0/PKG-INFO` & `alphawave-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.1.0
+Version: 0.1.1
 Summary: AlphaWave - a very opinionated client for interfacing with Large Language Models (LLM)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://github.com/Stevenic/alphawave-py
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alphawave-0.1.0/pyproject.toml` & `alphawave-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alphawave"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Steven Ickman", email="author@example.com" },
   { name="Bruce DAmbrosio", email="bruce.dambrosio@gmail.com" },
 ]
 
 description = "AlphaWave - a very opinionated client for interfacing with Large Language Models (LLM)"
```

### Comparing `alphawave-0.1.0/src/alphawave/AlphaWave.py` & `alphawave-0.1.1/src/alphawave/AlphaWave.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import Callable, Dict, Optional, Any
-from DefaultResponseValidator import DefaultResponseValidator
+from alphawave.DefaultResponseValidator import DefaultResponseValidator
 from promptrix.promptrixTypes import Message, PromptFunctions, PromptSection, PromptMemory, Tokenizer
 from promptrix.FunctionRegistry import  FunctionRegistry
 from promptrix.GPT3Tokenizer import GPT3Tokenizer
 from promptrix.VolatileMemory import VolatileMemory
 from promptrix.Utilities import Utilities
-from alphawaveTypes import  PromptCompletionClient, PromptCompletionOptions, PromptResponse,Validation, PromptResponseValidator 
-from DefaultResponseValidator import DefaultResponseValidator
-from MemoryFork import  MemoryFork
-from alphawaveTypes import PromptCompletionClient, PromptCompletionOptions, PromptResponse, Validation, PromptResponseValidator
-from MemoryFork import MemoryFork
-import Colorize
+from alphawave.alphawaveTypes import  PromptCompletionClient, PromptCompletionOptions, PromptResponse,Validation, PromptResponseValidator 
+from alphawave.DefaultResponseValidator import DefaultResponseValidator
+from alphawave.MemoryFork import  MemoryFork
+from alphawave.alphawaveTypes import PromptCompletionClient, PromptCompletionOptions, PromptResponse, Validation, PromptResponseValidator
+from alphawave.MemoryFork import MemoryFork
+import alphawave.Colorize as Colorize
 from pyee import AsyncIOEventEmitter
 import traceback
 
 class AlphaWaveOptions:
     def __init__(self, client: PromptCompletionClient, prompt: PromptSection, prompt_options: PromptCompletionOptions, functions: Optional[PromptFunctions] = None, history_variable: Optional[str] = None, input_variable: Optional[str] = None, max_history_messages: Optional[int] = None, max_repair_attempts: Optional[int] = None, memory: Optional[PromptMemory] = None, tokenizer: Optional[Tokenizer] = None, validator: Optional[PromptResponseValidator] = None, logRepairs: Optional[bool] = None):
         self.client = client
         self.prompt = prompt
```

### Comparing `alphawave-0.1.0/src/alphawave/Colorize.py` & `alphawave-0.1.1/src/alphawave/Colorize.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.0/src/alphawave/DefaultResponseValidator.py` & `alphawave-0.1.1/src/alphawave/DefaultResponseValidator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from promptrix.promptrixTypes import PromptFunctions, PromptMemory, Tokenizer
-from alphawaveTypes import PromptResponse, Validation, PromptResponseValidator
+from alphawave.alphawaveTypes import PromptResponse, Validation, PromptResponseValidator
 
 class DefaultResponseValidator(PromptResponseValidator):
     def validate_response(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, response: PromptResponse, remaining_attempts) -> Validation:
         self.feedback = response['message']['content'] if isinstance(response['message'], dict) else response.message
         return {
             'type': 'Validation',
             'valid': True,
```

### Comparing `alphawave-0.1.0/src/alphawave/JSONResponseValidator.py` & `alphawave-0.1.1/src/alphawave/JSONResponseValidator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from jsonschema import validate, ValidationError
 from promptrix import Message, PromptFunctions, PromptMemory, Tokenizer
 from types import PromptResponse, Validation
-from Response import Response
+from alphawave.Response import Response
 
 class JSONResponseValidator:
     def __init__(self, schema=None):
         self.schema = schema
 
     def validate_response(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, response: PromptResponse, remaining_attempts: int):
         message = response.message
```

### Comparing `alphawave-0.1.0/src/alphawave/OSClient.py` & `alphawave-0.1.1/src/alphawave/OSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.0/src/alphawave/OpenAIClient.py` & `alphawave-0.1.1/src/alphawave/OpenAIClient.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from typing import Optional, Dict, Any, Union
 import dataclasses
 from promptrix.promptrixTypes import PromptFunctions, PromptMemory, PromptSection, Tokenizer
 from promptrix.SystemMessage import SystemMessage
 from promptrix.ConversationHistory import ConversationHistory
 from promptrix.AssistantMessage import AssistantMessage
 
-from alphawaveTypes import PromptCompletionClient, PromptCompletionOptions, PromptResponse
-from internalTypes import ChatCompletionRequestMessage, CreateChatCompletionRequest, CreateChatCompletionResponse, CreateCompletionRequest, CreateCompletionResponse
-import Colorize
+from alphawave.alphawaveTypes import PromptCompletionClient, PromptCompletionOptions, PromptResponse
+from alphawave.internalTypes import ChatCompletionRequestMessage, CreateChatCompletionRequest, CreateChatCompletionResponse, CreateCompletionRequest, CreateCompletionResponse
+import alphawave.Colorize as Colorize
 
 class OpenAIClientOptions:
     def __init__(self, apiKey=None, organization = None, endpoint = None, logRequests = False):
         self.apiKey = apiKey
         self.organization = organization
         self.endpoint = endpoint
         self.logRequests = logRequests
```

### Comparing `alphawave-0.1.0/src/alphawave/Response.py` & `alphawave-0.1.1/src/alphawave/Response.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.0/src/alphawave/TestAlphaWave.py` & `alphawave-0.1.1/src/alphawave/TestAlphaWave.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import aiounittest, unittest
 from assertpy import assert_that
 from promptrix.promptrixTypes import Message, PromptFunctions, PromptMemory, Tokenizer
 from promptrix.FunctionRegistry import FunctionRegistry 
 from promptrix.Prompt import Prompt
 from promptrix.GPT3Tokenizer import GPT3Tokenizer
 from promptrix.VolatileMemory import VolatileMemory
-from alphawaveTypes import PromptCompletionOptions, PromptResponse, PromptResponseValidator, Validation
-from DefaultResponseValidator import DefaultResponseValidator
-from TestClient import TestClient
-from AlphaWave import AlphaWave
+from alphawave.alphawaveTypes import PromptCompletionOptions, PromptResponse, PromptResponseValidator, Validation
+from alphawave.DefaultResponseValidator import DefaultResponseValidator
+from alphawave.TestClient import TestClient
+from alphawave.AlphaWave import AlphaWave
 
 class TestValidator(PromptResponseValidator):
     def __init__(self, client):
         self.feedback = 'Something is wrong'
         self.repairAttempts = 0
         self.exception = None
         self.clientErrorDuringRepair = False
```

### Comparing `alphawave-0.1.0/src/alphawave/TestClient.py` & `alphawave-0.1.1/src/alphawave/TestClient.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Union
 from promptrix.promptrixTypes import PromptFunctions, PromptMemory, PromptSection, Tokenizer
 from  promptrix.promptrixTypes import Message
-from alphawaveTypes import PromptCompletionClient, PromptCompletionOptions, PromptResponse, PromptResponseStatus
+from alphawave.alphawaveTypes import PromptCompletionClient, PromptCompletionOptions, PromptResponse, PromptResponseStatus
 
 class TestClient(PromptCompletionClient):
     def __init__(self, status: PromptResponseStatus = 'success', response: Union[str, Message] = {'role': 'assistant', 'content': "Hello World"}):
         self.status = status
         self.response = response
 
     async def complete_prompt(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, prompt: PromptSection, options: PromptCompletionOptions) -> PromptResponse:
```

### Comparing `alphawave-0.1.0/src/alphawave/TestClientTest.py` & `alphawave-0.1.1/src/alphawave/TestClientTest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import unittest
 import yaml
 from promptrix.VolatileMemory import VolatileMemory
 from promptrix.FunctionRegistry import FunctionRegistry
 from promptrix.GPT3Tokenizer import  GPT3Tokenizer
 from promptrix.Prompt import Prompt
 
-from alphawaveTypes import PromptCompletionOptions
-from TestClient import TestClient
+from alphawave.alphawaveTypes import PromptCompletionOptions
+from alphawave.TestClient import TestClient
 import asyncio
 
 class TestClientTest(unittest.TestCase):
     def setUp(self):
         self.memory = VolatileMemory()
         self.functions = FunctionRegistry()
         self.tokenizer = GPT3Tokenizer()
```

### Comparing `alphawave-0.1.0/src/alphawave/alphaChat.py` & `alphawave-0.1.1/src/alphawave/alphaChat.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.0/src/alphawave/alphawaveTypes.py` & `alphawave-0.1.1/src/alphawave/alphawaveTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.0/src/alphawave/internalTypes.py` & `alphawave-0.1.1/src/alphawave/internalTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.0/src/alphawave.egg-info/PKG-INFO` & `alphawave-0.1.1/src/alphawave.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.1.0
+Version: 0.1.1
 Summary: AlphaWave - a very opinionated client for interfacing with Large Language Models (LLM)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://github.com/Stevenic/alphawave-py
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alphawave-0.1.0/src/alphawave.egg-info/SOURCES.txt` & `alphawave-0.1.1/src/alphawave.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 src/alphawave/AlphaWave.py
 src/alphawave/Colorize.py
 src/alphawave/DefaultResponseValidator.py
 src/alphawave/JSONResponseValidator.py
-src/alphawave/MemoryForkTest.py
+src/alphawave/MemoryFork.py
 src/alphawave/OSClient.py
 src/alphawave/OpenAIClient.py
 src/alphawave/Response.py
 src/alphawave/TestAlphaWave.py
 src/alphawave/TestClient.py
 src/alphawave/TestClientTest.py
 src/alphawave/alphaChat.py
```

### Comparing `alphawave-0.1.0/tests/testOpenAiClient.py` & `alphawave-0.1.1/tests/testOpenAiClient.py`

 * *Files identical despite different names*

