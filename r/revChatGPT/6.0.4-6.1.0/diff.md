# Comparing `tmp/revChatGPT-6.0.4.tar.gz` & `tmp/revChatGPT-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-6.0.4.tar", last modified: Tue Jun  6 06:43:26 2023, max compression
+gzip compressed data, was "revChatGPT-6.1.0.tar", last modified: Tue Jun  6 16:24:18 2023, max compression
```

## Comparing `revChatGPT-6.0.4.tar` & `revChatGPT-6.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:43:26.070523 revChatGPT-6.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-06 06:42:56.000000 revChatGPT-6.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-06-06 06:43:26.070523 revChatGPT-6.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-06 06:43:25.000000 revChatGPT-6.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-06 06:43:26.070523 revChatGPT-6.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-06 06:42:56.000000 revChatGPT-6.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:43:26.070523 revChatGPT-6.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:43:26.070523 revChatGPT-6.0.4/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    49765 2023-06-06 06:42:56.000000 revChatGPT-6.0.4/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-06-06 06:42:56.000000 revChatGPT-6.0.4/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-06 06:42:56.000000 revChatGPT-6.0.4/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-06 06:42:56.000000 revChatGPT-6.0.4/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:43:26.070523 revChatGPT-6.0.4/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-06 06:42:56.000000 revChatGPT-6.0.4/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-06 06:42:56.000000 revChatGPT-6.0.4/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-06 06:42:56.000000 revChatGPT-6.0.4/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:43:26.070523 revChatGPT-6.0.4/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-06-06 06:43:26.000000 revChatGPT-6.0.4/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-06 06:43:26.000000 revChatGPT-6.0.4/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 06:43:26.000000 revChatGPT-6.0.4/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-06 06:43:26.000000 revChatGPT-6.0.4/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-06 06:43:26.000000 revChatGPT-6.0.4/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:43:26.070523 revChatGPT-6.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-06 06:42:56.000000 revChatGPT-6.0.4/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:24:18.597769 revChatGPT-6.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-06 16:23:42.000000 revChatGPT-6.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-06-06 16:24:18.597769 revChatGPT-6.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-06 16:24:18.000000 revChatGPT-6.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-06 16:24:18.597769 revChatGPT-6.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-06 16:23:42.000000 revChatGPT-6.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:24:18.593769 revChatGPT-6.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:24:18.597769 revChatGPT-6.1.0/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    51072 2023-06-06 16:23:42.000000 revChatGPT-6.1.0/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-06-06 16:23:42.000000 revChatGPT-6.1.0/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-06 16:23:42.000000 revChatGPT-6.1.0/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-06 16:23:42.000000 revChatGPT-6.1.0/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:24:18.597769 revChatGPT-6.1.0/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-06 16:23:42.000000 revChatGPT-6.1.0/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-06 16:23:42.000000 revChatGPT-6.1.0/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-06 16:23:42.000000 revChatGPT-6.1.0/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:24:18.597769 revChatGPT-6.1.0/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-06-06 16:24:18.000000 revChatGPT-6.1.0/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-06 16:24:18.000000 revChatGPT-6.1.0/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 16:24:18.000000 revChatGPT-6.1.0/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-06 16:24:18.000000 revChatGPT-6.1.0/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-06 16:24:18.000000 revChatGPT-6.1.0/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:24:18.597769 revChatGPT-6.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-06 16:23:42.000000 revChatGPT-6.1.0/tests/test_recipient.py
```

### Comparing `revChatGPT-6.0.4/LICENSE` & `revChatGPT-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.0.4/PKG-INFO` & `revChatGPT-6.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.0.4
+Version: 6.1.0
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.0.4/README.md` & `revChatGPT-6.1.0/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.0.4/setup.py` & `revChatGPT-6.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="6.0.4",
+    version="6.1.0",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-6.0.4/src/revChatGPT/V1.py` & `revChatGPT-6.1.0/src/revChatGPT/V1.py`

 * *Files 2% similar despite different names*

```diff
@@ -485,15 +485,15 @@
                         print("Conversation unavailable")
                 else:
                     self.__map_conversations()
             if conversation_id in self.conversation_mapping:
                 parent_id = self.conversation_mapping[conversation_id]
             else:
                 print(
-                    "Warning: Invalid conversation_id provided, treat as a new conversation"
+                    "Warning: Invalid conversation_id provided, treat as a new conversation",
                 )
                 conversation_id = None
                 parent_id = str(uuid.uuid4())
 
         data = {
             "action": "next",
             "messages": messages,
@@ -801,57 +801,71 @@
 class AsyncChatbot(Chatbot):
     """Async Chatbot class for ChatGPT"""
 
     def __init__(
         self,
         config: dict,
         conversation_id: str | None = None,
-        parent_id: str = "",
-        base_url: str = "",
+        parent_id: str | None = None,
+        base_url: str | None = None,
+        lazy_loading: bool = True,
     ) -> None:
         """
         Same as Chatbot class, but with async methods.
         """
         super().__init__(
             config=config,
             conversation_id=conversation_id,
             parent_id=parent_id,
             base_url=base_url,
+            lazy_loading=lazy_loading,
         )
 
         # overwrite inherited normal session with async
         self.session = AsyncClient(headers=self.session.headers)
 
     async def __send_request(
         self,
         data: dict,
         auto_continue: bool = False,
         timeout: float = 360,
+        **kwargs,
     ) -> AsyncGenerator[dict, None]:
+        log.debug("Sending the payload")
+
         cid, pid = data["conversation_id"], data["parent_message_id"]
+        model, message = None, ""
 
         self.conversation_id_prev_queue.append(cid)
         self.parent_id_prev_queue.append(pid)
-        message = ""
-
-        finish_details = None
-        response = None
-        async with self.session.stream(
-            method="POST",
+        async with self.session.post(
             url=f"{self.base_url}conversation",
             data=json.dumps(data),
             timeout=timeout,
+            stream=True,
         ) as response:
             await self.__check_response(response)
+
+            finish_details = None
             async for line in response.aiter_lines():
+                # remove b' and ' at the beginning and end and ignore case
+                line = str(line)[2:-1]
+                if line.lower() == "internal server error":
+                    log.error(f"Internal Server Error: {line}")
+                    error = t.Error(
+                        source="ask",
+                        message="Internal Server Error",
+                        code=t.ErrorType.SERVER_ERROR,
+                    )
+                    raise error
                 if not line or line is None:
                     continue
                 if "data: " in line:
                     line = line[6:]
-                if "[DONE]" in line:
+                if line == "[DONE]":
                     break
 
                 # DO NOT REMOVE THIS
                 line = line.replace('\\"', '"')
                 line = line.replace("\\'", "'")
                 line = line.replace("\\\\", "\\")
 
@@ -860,23 +874,23 @@
                 except json.decoder.JSONDecodeError:
                     continue
                 if not self.__check_fields(line):
                     raise ValueError(f"Field missing. Details: {str(line)}")
                 if line.get("message").get("author").get("role") != "assistant":
                     continue
 
-                message: str = line["message"]["content"]["parts"][0]
                 cid = line["conversation_id"]
                 pid = line["message"]["id"]
                 metadata = line["message"].get("metadata", {})
                 message_exists = False
                 author = {}
                 if line.get("message"):
                     author = metadata.get("author", {}) or line["message"].get(
-                        "author", {}
+                        "author",
+                        {},
                     )
                     if line["message"].get("content"):
                         if line["message"]["content"].get("parts"):
                             if len(line["message"]["content"]["parts"]) > 0:
                                 message_exists = True
                 message: str = (
                     line["message"]["content"]["parts"][0] if message_exists else ""
@@ -892,106 +906,119 @@
                     "finish_details": finish_details,
                     "end_turn": line["message"].get("end_turn", True),
                     "recipient": line["message"].get("recipient", "all"),
                     "citations": metadata.get("citations", []),
                 }
 
             self.conversation_mapping[cid] = pid
-            if pid:
+            if pid is not None:
                 self.parent_id = pid
-            if cid:
+            if cid is not None:
                 self.conversation_id = cid
 
-        if not (auto_continue and finish_details == "max_tokens"):
-            return
-        async for msg in self.continue_write(
-            conversation_id=cid,
-            auto_continue=False,
-            timeout=timeout,
-        ):
-            msg["message"] = message + msg["message"]
-            yield msg
+            if not (auto_continue and finish_details == "max_tokens"):
+                return
+            message = message.strip("\n")
+            async for i in self.continue_write(
+                conversation_id=cid,
+                timeout=timeout,
+                auto_continue=False,
+            ):
+                i["message"] = message + i["message"]
+                yield i
 
     async def post_messages(
         self,
         messages: list[dict],
         conversation_id: str | None = None,
-        parent_id: str = "",
+        parent_id: str | None = None,
         plugin_ids: list = [],
-        model: str = "",
+        model: str | None = None,
         auto_continue: bool = False,
-        timeout: int = 360,
+        timeout: float = 360,
+        **kwargs,
     ) -> AsyncGenerator[dict, None]:
         """Post messages to the chatbot
 
         Args:
             messages (list[dict]): the messages to post
             conversation_id (str | None, optional): UUID for the conversation to continue on. Defaults to None.
-            parent_id (str, optional): UUID for the message to continue on. Defaults to "".
-            model (str, optional): The model to use. Defaults to "".
+            parent_id (str | None, optional): UUID for the message to continue on. Defaults to None.
+            model (str | None, optional): The model to use. Defaults to None.
             auto_continue (bool, optional): Whether to continue the conversation automatically. Defaults to False.
             timeout (float, optional): Timeout for getting the full response, unit is second. Defaults to 360.
 
         Yields:
             AsyncGenerator[dict, None]: The response from the chatbot
             {
                 "message": str,
                 "conversation_id": str,
                 "parent_id": str,
                 "model": str,
                 "finish_details": str,
                 "end_turn": bool,
                 "recipient": str,
+                "citations": list[dict],
             }
         """
         if parent_id and not conversation_id:
-            error = t.Error(
+            raise t.Error(
                 source="User",
                 message="conversation_id must be set once parent_id is set",
-                code=t.ErrorType.SERVER_ERROR,
+                code=t.ErrorType.USER_ERROR,
             )
-            raise error
+
         if conversation_id and conversation_id != self.conversation_id:
             self.parent_id = None
         conversation_id = conversation_id or self.conversation_id
-
         parent_id = parent_id or self.parent_id or ""
         if not conversation_id and not parent_id:
             parent_id = str(uuid.uuid4())
+
         if conversation_id and not parent_id:
             if conversation_id not in self.conversation_mapping:
-                await self.__map_conversations()
+                if self.lazy_loading:
+                    log.debug(
+                        "Conversation ID %s not found in conversation mapping, try to get conversation history for the given ID",
+                        conversation_id,
+                    )
+                    try:
+                        history = await self.get_msg_history(conversation_id)
+                        self.conversation_mapping[conversation_id] = history[
+                            "current_node"
+                        ]
+                    except requests.exceptions.HTTPError:
+                        print("Conversation unavailable")
+                else:
+                    await self.__map_conversations()
             if conversation_id in self.conversation_mapping:
                 parent_id = self.conversation_mapping[conversation_id]
-            else:  # invalid conversation_id provided, treat as a new conversation
+            else:
+                print(
+                    "Warning: Invalid conversation_id provided, treat as a new conversation"
+                )
                 conversation_id = None
                 parent_id = str(uuid.uuid4())
 
         data = {
             "action": "next",
             "messages": messages,
             "conversation_id": conversation_id,
             "parent_message_id": parent_id,
-            "model": model
-            or self.config.get("model")
-            or (
-                "text-davinci-002-render-paid"
-                if self.config.get("paid")
-                else "text-davinci-002-render-sha"
-            ),
+            "model": model or self.config.get("model") or "text-davinci-002-render-sha",
             "history_and_training_disabled": self.disable_history,
         }
         plugin_ids = self.config.get("plugin_ids", []) or plugin_ids
         if len(plugin_ids) > 0 and not conversation_id:
             data["plugin_ids"] = plugin_ids
 
         async for msg in self.__send_request(
-            data=data,
-            auto_continue=auto_continue,
+            data,
             timeout=timeout,
+            auto_continue=auto_continue,
         ):
             yield msg
 
     async def ask(
         self,
         prompt: str,
         conversation_id: str | None = None,
```

### Comparing `revChatGPT-6.0.4/src/revChatGPT/V3.py` & `revChatGPT-6.1.0/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.0.4/src/revChatGPT/__init__.py` & `revChatGPT-6.1.0/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.0.4/src/revChatGPT/__main__.py` & `revChatGPT-6.1.0/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.0.4/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.1.0/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.0.4/src/revChatGPT/typings.py` & `revChatGPT-6.1.0/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.0.4/src/revChatGPT/utils.py` & `revChatGPT-6.1.0/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.0.4/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.1.0/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.0.4
+Version: 6.1.0
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.0.4/tests/test_recipient.py` & `revChatGPT-6.1.0/tests/test_recipient.py`

 * *Files identical despite different names*

