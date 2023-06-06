# Comparing `tmp/EdgeGPT-0.9.0.tar.gz` & `tmp/EdgeGPT-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.9.0.tar", last modified: Mon Jun  5 14:09:57 2023, max compression
+gzip compressed data, was "EdgeGPT-0.9.1.tar", last modified: Mon Jun  5 14:25:11 2023, max compression
```

## Comparing `EdgeGPT-0.9.0.tar` & `EdgeGPT-0.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:09:57.142855 EdgeGPT-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-05 14:09:16.000000 EdgeGPT-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-06-05 14:09:57.142855 EdgeGPT-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10802 2023-06-05 14:09:56.000000 EdgeGPT-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-05 14:09:57.142855 EdgeGPT-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-05 14:09:16.000000 EdgeGPT-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:09:57.138855 EdgeGPT-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:09:57.138855 EdgeGPT-0.9.0/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-06-05 14:09:57.000000 EdgeGPT-0.9.0/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-05 14:09:57.000000 EdgeGPT-0.9.0/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:09:57.000000 EdgeGPT-0.9.0/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-05 14:09:57.000000 EdgeGPT-0.9.0/src/EdgeGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-05 14:09:57.000000 EdgeGPT-0.9.0/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-05 14:09:57.000000 EdgeGPT-0.9.0/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-06-05 14:09:16.000000 EdgeGPT-0.9.0/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-06-05 14:09:16.000000 EdgeGPT-0.9.0/src/EdgeUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-05 14:09:16.000000 EdgeGPT-0.9.0/src/ImageGen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:09:57.142855 EdgeGPT-0.9.0/src/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:09:16.000000 EdgeGPT-0.9.0/src/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-05 14:09:16.000000 EdgeGPT-0.9.0/src/helpers/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-06-05 14:09:16.000000 EdgeGPT-0.9.0/src/helpers/conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-05 14:09:16.000000 EdgeGPT-0.9.0/src/helpers/conversation_style.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-05 14:09:16.000000 EdgeGPT-0.9.0/src/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-05 14:09:16.000000 EdgeGPT-0.9.0/src/helpers/locale.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-05 14:09:16.000000 EdgeGPT-0.9.0/src/helpers/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:25:11.448655 EdgeGPT-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-05 14:24:43.000000 EdgeGPT-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-06-05 14:25:11.448655 EdgeGPT-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10802 2023-06-05 14:25:11.000000 EdgeGPT-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-05 14:25:11.448655 EdgeGPT-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-05 14:24:43.000000 EdgeGPT-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:25:11.448655 EdgeGPT-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:25:11.448655 EdgeGPT-0.9.1/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-06-05 14:25:11.000000 EdgeGPT-0.9.1/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-05 14:25:11.000000 EdgeGPT-0.9.1/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:25:11.000000 EdgeGPT-0.9.1/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-05 14:25:11.000000 EdgeGPT-0.9.1/src/EdgeGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-05 14:25:11.000000 EdgeGPT-0.9.1/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-05 14:25:11.000000 EdgeGPT-0.9.1/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11971 2023-06-05 14:24:43.000000 EdgeGPT-0.9.1/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-06-05 14:24:43.000000 EdgeGPT-0.9.1/src/EdgeUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-05 14:24:43.000000 EdgeGPT-0.9.1/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:25:11.448655 EdgeGPT-0.9.1/src/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:24:43.000000 EdgeGPT-0.9.1/src/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-05 14:24:43.000000 EdgeGPT-0.9.1/src/helpers/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-06-05 14:24:43.000000 EdgeGPT-0.9.1/src/helpers/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-05 14:24:43.000000 EdgeGPT-0.9.1/src/helpers/conversation_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-05 14:24:43.000000 EdgeGPT-0.9.1/src/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-05 14:24:43.000000 EdgeGPT-0.9.1/src/helpers/locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-05 14:24:43.000000 EdgeGPT-0.9.1/src/helpers/utilities.py
```

### Comparing `EdgeGPT-0.9.0/LICENSE` & `EdgeGPT-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.9.0/PKG-INFO` & `EdgeGPT-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.9.0
+Version: 0.9.1
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.9.0 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.9.1 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.9.0/README.md` & `EdgeGPT-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.9.0/setup.py` & `EdgeGPT-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with Path.open(DOCS_PATH, encoding="utf-8") as f1:
         with Path.open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT",
-    version="0.9.0",
+    version="0.9.1",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
```

### Comparing `EdgeGPT-0.9.0/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.9.1/src/EdgeGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.9.0
+Version: 0.9.1
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.9.0 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.9.1 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.9.0/src/EdgeGPT.py` & `EdgeGPT-0.9.1/src/EdgeGPT.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,16 +17,17 @@
 from prompt_toolkit.completion import WordCompleter
 from prompt_toolkit.history import InMemoryHistory
 from prompt_toolkit.key_binding import KeyBindings
 from rich.live import Live
 from rich.markdown import Markdown
 
 from src.helpers.chathub.chathub import ChatHub
+from src.helpers.chathub.request import ChatHubRequest
 from src.helpers.conversation import Conversation
-from src.helpers.utilities import guess_locale
+from src.helpers.utilities import guess_locale, get_ran_hex
 from src.helpers.conversation_style import CONVERSATION_STYLE_TYPE
 
 
 class Chatbot:
     """
     Combines everything to make it seamless
     """
@@ -58,22 +59,45 @@
         return self
 
     async def save_conversation(self, filename: str) -> None:
         """
         Save the conversation to a file
         """
         with open(filename, "w") as f:
-            f.write(json.dumps(self.chat_hub.request.struct))
+            conversation_id = self.chat_hub.request.conversation_id
+            conversation_signature = self.chat_hub.request.conversation_signature
+            client_id = self.chat_hub.request.client_id
+            invocation_id = self.chat_hub.request.invocation_id
+            f.write(
+                {
+                    "conversation_id": conversation_id,
+                    "conversation_signature": conversation_signature,
+                    "client_id": client_id,
+                    "invocation_id": invocation_id,
+                }
+            )
 
     async def load_conversation(self, filename: str) -> None:
         """
         Load the conversation from a file
         """
         with open(filename, "r") as f:
-            self.chat_hub.request.struct = json.loads(f.read())
+            conversation = json.load(f)
+            self.chat_hub.request = ChatHubRequest(
+                conversation_signature=conversation["conversation_signature"],
+                client_id=conversation["client_id"],
+                conversation_id=conversation["conversation_id"],
+                invocation_id=conversation["invocation_id"],
+            )
+
+    async def get_conversation(self) -> dict:
+        """
+        Gets the conversation history from conversation_id (requires load_conversation)
+        """
+        return await self.chat_hub.get_conversation()
 
     async def ask(
         self,
         prompt: str,
         wss_link: str = "wss://sydney.bing.com/sydney/ChatHub",
         conversation_style: CONVERSATION_STYLE_TYPE = None,
         webpage_context: str | None = None,
```

### Comparing `EdgeGPT-0.9.0/src/EdgeUtils.py` & `EdgeGPT-0.9.1/src/EdgeUtils.py`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.9.0/src/helpers/constants.py` & `EdgeGPT-0.9.1/src/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.9.0/src/helpers/conversation.py` & `EdgeGPT-0.9.1/src/helpers/conversation.py`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.9.0/src/helpers/conversation_style.py` & `EdgeGPT-0.9.1/src/helpers/conversation_style.py`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.9.0/src/helpers/locale.py` & `EdgeGPT-0.9.1/src/helpers/locale.py`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.9.0/src/helpers/utilities.py` & `EdgeGPT-0.9.1/src/helpers/utilities.py`

 * *Files identical despite different names*

