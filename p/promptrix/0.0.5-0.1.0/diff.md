# Comparing `tmp/promptrix-0.0.5.tar.gz` & `tmp/promptrix-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptrix-0.0.5.tar", last modified: Mon Jun  5 18:17:59 2023, max compression
+gzip compressed data, was "promptrix-0.1.0.tar", last modified: Mon Jun  5 23:20:20 2023, max compression
```

## Comparing `promptrix-0.0.5.tar` & `promptrix-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-05 18:17:59.399273 promptrix-0.0.5/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-01 23:37:06.000000 promptrix-0.0.5/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      648 2023-06-05 18:17:59.399273 promptrix-0.0.5/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       78 2023-06-01 23:37:06.000000 promptrix-0.0.5/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      777 2023-06-05 18:17:48.000000 promptrix-0.0.5/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-05 18:17:59.399273 promptrix-0.0.5/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-05 18:17:59.395273 promptrix-0.0.5/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-05 18:17:59.399273 promptrix-0.0.5/src/promptrix/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      746 2023-06-03 03:50:31.000000 promptrix-0.0.5/src/promptrix/AssistantMessage.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2517 2023-06-05 18:17:18.000000 promptrix-0.0.5/src/promptrix/ConversationHistory.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1184 2023-06-02 18:46:08.000000 promptrix-0.0.5/src/promptrix/FunctionRegistry.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      551 2023-06-02 18:46:08.000000 promptrix-0.0.5/src/promptrix/GPT3Tokenizer.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1092 2023-06-02 18:46:08.000000 promptrix-0.0.5/src/promptrix/GroupSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     5158 2023-06-02 18:46:08.000000 promptrix-0.0.5/src/promptrix/LayoutEngine.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      421 2023-06-02 18:46:08.000000 promptrix-0.0.5/src/promptrix/Prompt.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2190 2023-06-02 18:46:08.000000 promptrix-0.0.5/src/promptrix/PromptSectionBase.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      475 2023-06-02 18:46:08.000000 promptrix-0.0.5/src/promptrix/SystemMessage.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     5352 2023-06-03 03:50:22.000000 promptrix-0.0.5/src/promptrix/TemplateSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      821 2023-06-02 18:46:08.000000 promptrix-0.0.5/src/promptrix/TextSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      621 2023-06-02 18:46:08.000000 promptrix-0.0.5/src/promptrix/UserMessage.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      985 2023-06-02 18:46:08.000000 promptrix-0.0.5/src/promptrix/Utilities.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      936 2023-06-02 18:46:08.000000 promptrix-0.0.5/src/promptrix/VolatileMemory.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1255 2023-06-02 18:46:08.000000 promptrix-0.0.5/src/promptrix/example.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1494 2023-06-02 18:46:08.000000 promptrix-0.0.5/src/promptrix/promptrixTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1733 2023-06-02 18:46:08.000000 promptrix-0.0.5/src/promptrix/types.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-05 18:17:59.399273 promptrix-0.0.5/src/promptrix.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      648 2023-06-05 18:17:59.000000 promptrix-0.0.5/src/promptrix.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      732 2023-06-05 18:17:59.000000 promptrix-0.0.5/src/promptrix.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-05 18:17:59.000000 promptrix-0.0.5/src/promptrix.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       71 2023-06-05 18:17:59.000000 promptrix-0.0.5/src/promptrix.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       10 2023-06-05 18:17:59.000000 promptrix-0.0.5/src/promptrix.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-05 23:20:20.844457 promptrix-0.1.0/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-01 23:37:06.000000 promptrix-0.1.0/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      648 2023-06-05 23:20:20.844457 promptrix-0.1.0/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       78 2023-06-01 23:37:06.000000 promptrix-0.1.0/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      777 2023-06-05 23:20:10.000000 promptrix-0.1.0/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-05 23:20:20.844457 promptrix-0.1.0/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-05 23:20:20.844457 promptrix-0.1.0/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-05 23:20:20.844457 promptrix-0.1.0/src/promptrix/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      746 2023-06-03 03:50:31.000000 promptrix-0.1.0/src/promptrix/AssistantMessage.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2542 2023-06-05 23:16:40.000000 promptrix-0.1.0/src/promptrix/ConversationHistory.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1164 2023-06-05 23:10:10.000000 promptrix-0.1.0/src/promptrix/FunctionRegistry.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      551 2023-06-02 18:46:08.000000 promptrix-0.1.0/src/promptrix/GPT3Tokenizer.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1092 2023-06-02 18:46:08.000000 promptrix-0.1.0/src/promptrix/GroupSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     5158 2023-06-02 18:46:08.000000 promptrix-0.1.0/src/promptrix/LayoutEngine.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      421 2023-06-02 18:46:08.000000 promptrix-0.1.0/src/promptrix/Prompt.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2193 2023-06-05 23:06:31.000000 promptrix-0.1.0/src/promptrix/PromptSectionBase.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      475 2023-06-02 18:46:08.000000 promptrix-0.1.0/src/promptrix/SystemMessage.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     5352 2023-06-03 03:50:22.000000 promptrix-0.1.0/src/promptrix/TemplateSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      821 2023-06-02 18:46:08.000000 promptrix-0.1.0/src/promptrix/TextSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      621 2023-06-02 18:46:08.000000 promptrix-0.1.0/src/promptrix/UserMessage.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      985 2023-06-02 18:46:08.000000 promptrix-0.1.0/src/promptrix/Utilities.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      936 2023-06-02 18:46:08.000000 promptrix-0.1.0/src/promptrix/VolatileMemory.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1494 2023-06-02 18:46:08.000000 promptrix-0.1.0/src/promptrix/promptrixTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1733 2023-06-02 18:46:08.000000 promptrix-0.1.0/src/promptrix/types.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-05 23:20:20.844457 promptrix-0.1.0/src/promptrix.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      648 2023-06-05 23:20:20.000000 promptrix-0.1.0/src/promptrix.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      707 2023-06-05 23:20:20.000000 promptrix-0.1.0/src/promptrix.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-05 23:20:20.000000 promptrix-0.1.0/src/promptrix.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       71 2023-06-05 23:20:20.000000 promptrix-0.1.0/src/promptrix.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       10 2023-06-05 23:20:20.000000 promptrix-0.1.0/src/promptrix.egg-info/top_level.txt
```

### Comparing `promptrix-0.0.5/LICENSE` & `promptrix-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `promptrix-0.0.5/PKG-INFO` & `promptrix-0.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptrix
-Version: 0.0.5
+Version: 0.1.0
 Summary: Promptrix. A prompt layout manager for LLMs
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://github.com/Stevenic/promptrix-py
 Project-URL: Bug Tracker, https://github.com/Stevenic/promptrix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `promptrix-0.0.5/pyproject.toml` & `promptrix-0.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "promptrix"
-version = "0.0.5"
+version = "0.1.0"
 authors = [
   { name="Steven Ickman", email="author@example.com" },
   { name="Bruce DAmbrosio", email="bruce.dambrosio@gmail.com" },
 ]
 
 description = "Promptrix. A prompt layout manager for LLMs"
```

### Comparing `promptrix-0.0.5/src/promptrix/AssistantMessage.py` & `promptrix-0.1.0/src/promptrix/AssistantMessage.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.0.5/src/promptrix/ConversationHistory.py` & `promptrix-0.1.0/src/promptrix/ConversationHistory.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,12 +40,13 @@
         for i in range(len(history)-1, -1, -1):
             msg = history[i]
             message = Message(role=msg['role'], content=Utilities.to_string(tokenizer, msg['content']))
             length = len(tokenizer.encode(message.content))
             if len(messages) == 0 and self.required:
                 tokens += length
                 messages.insert(0, message)
+                continue
             if tokens + length > budget:
                 break
             tokens += length
             messages.insert(0, msg)
         return RenderedPromptSection(output=messages, length=tokens, tooLong=tokens > maxTokens)
```

### Comparing `promptrix-0.0.5/src/promptrix/FunctionRegistry.py` & `promptrix-0.1.0/src/promptrix/FunctionRegistry.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
             for key, value in functions.items():
                 self._functions[key] = value
 
     def has(self, name: str) -> bool:
         return name in self._functions
 
     def get(self, name: str) -> Callable:
-        print(name)
         fn = self._functions.get(name)
         if not fn:
             raise Exception(f"Function {name} not found.")
         return fn
 
     def addFunction(self, name: str, value: Callable) -> None:
         if self.has(name):
```

### Comparing `promptrix-0.0.5/src/promptrix/GPT3Tokenizer.py` & `promptrix-0.1.0/src/promptrix/GPT3Tokenizer.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.0.5/src/promptrix/GroupSection.py` & `promptrix-0.1.0/src/promptrix/GroupSection.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.0.5/src/promptrix/LayoutEngine.py` & `promptrix-0.1.0/src/promptrix/LayoutEngine.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.0.5/src/promptrix/PromptSectionBase.py` & `promptrix-0.1.0/src/promptrix/PromptSectionBase.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             length = self.tokens
         return RenderedPromptSection(output=text, length=length, tooLong=length > max_tokens)
 
     def return_messages(self, output, length, tokenizer, max_tokens):
         if self.tokens > 1.0:
             while length > self.tokens:
                 msg = output.pop()
-                encoded = tokenizer.encode(msg.content)
+                encoded = tokenizer.encode(msg['content'])
                 length -= len(encoded)
                 if length < self.tokens:
                     delta = self.tokens - length
                     truncated = tokenizer.decode(encoded[:delta])
                     output.append(Message(role=msg.role, content=truncated))
                     length += delta
         return RenderedPromptSection(output=output, length=length, tooLong=length > max_tokens)
```

### Comparing `promptrix-0.0.5/src/promptrix/TemplateSection.py` & `promptrix-0.1.0/src/promptrix/TemplateSection.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.0.5/src/promptrix/TextSection.py` & `promptrix-0.1.0/src/promptrix/TextSection.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.0.5/src/promptrix/UserMessage.py` & `promptrix-0.1.0/src/promptrix/UserMessage.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.0.5/src/promptrix/Utilities.py` & `promptrix-0.1.0/src/promptrix/Utilities.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.0.5/src/promptrix/VolatileMemory.py` & `promptrix-0.1.0/src/promptrix/VolatileMemory.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.0.5/src/promptrix/promptrixTypes.py` & `promptrix-0.1.0/src/promptrix/promptrixTypes.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.0.5/src/promptrix/types.py` & `promptrix-0.1.0/src/promptrix/types.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.0.5/src/promptrix.egg-info/PKG-INFO` & `promptrix-0.1.0/src/promptrix.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptrix
-Version: 0.0.5
+Version: 0.1.0
 Summary: Promptrix. A prompt layout manager for LLMs
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://github.com/Stevenic/promptrix-py
 Project-URL: Bug Tracker, https://github.com/Stevenic/promptrix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `promptrix-0.0.5/src/promptrix.egg-info/SOURCES.txt` & `promptrix-0.1.0/src/promptrix.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 src/promptrix/PromptSectionBase.py
 src/promptrix/SystemMessage.py
 src/promptrix/TemplateSection.py
 src/promptrix/TextSection.py
 src/promptrix/UserMessage.py
 src/promptrix/Utilities.py
 src/promptrix/VolatileMemory.py
-src/promptrix/example.py
 src/promptrix/promptrixTypes.py
 src/promptrix/types.py
 src/promptrix.egg-info/PKG-INFO
 src/promptrix.egg-info/SOURCES.txt
 src/promptrix.egg-info/dependency_links.txt
 src/promptrix.egg-info/requires.txt
 src/promptrix.egg-info/top_level.txt
```

