# Comparing `tmp/revChatGPT-6.0.3.tar.gz` & `tmp/revChatGPT-6.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-6.0.3.tar", last modified: Tue Jun  6 03:03:22 2023, max compression
+gzip compressed data, was "revChatGPT-6.0.4.tar", last modified: Tue Jun  6 06:43:26 2023, max compression
```

## Comparing `revChatGPT-6.0.3.tar` & `revChatGPT-6.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 03:03:22.193700 revChatGPT-6.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-06 03:02:54.000000 revChatGPT-6.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-06-06 03:03:22.193700 revChatGPT-6.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-06 03:03:22.000000 revChatGPT-6.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-06 03:03:22.197700 revChatGPT-6.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-06 03:02:54.000000 revChatGPT-6.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 03:03:22.193700 revChatGPT-6.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 03:03:22.193700 revChatGPT-6.0.3/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    49622 2023-06-06 03:02:54.000000 revChatGPT-6.0.3/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-06-06 03:02:54.000000 revChatGPT-6.0.3/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-06 03:02:54.000000 revChatGPT-6.0.3/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-06 03:02:54.000000 revChatGPT-6.0.3/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 03:03:22.193700 revChatGPT-6.0.3/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-06 03:02:54.000000 revChatGPT-6.0.3/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-06 03:02:54.000000 revChatGPT-6.0.3/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-06 03:02:54.000000 revChatGPT-6.0.3/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 03:03:22.193700 revChatGPT-6.0.3/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-06-06 03:03:22.000000 revChatGPT-6.0.3/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-06 03:03:22.000000 revChatGPT-6.0.3/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 03:03:22.000000 revChatGPT-6.0.3/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-06 03:03:22.000000 revChatGPT-6.0.3/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-06 03:03:22.000000 revChatGPT-6.0.3/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 03:03:22.193700 revChatGPT-6.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-06 03:02:54.000000 revChatGPT-6.0.3/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:43:26.070523 revChatGPT-6.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-06 06:42:56.000000 revChatGPT-6.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-06-06 06:43:26.070523 revChatGPT-6.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-06 06:43:25.000000 revChatGPT-6.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-06 06:43:26.070523 revChatGPT-6.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-06 06:42:56.000000 revChatGPT-6.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:43:26.070523 revChatGPT-6.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:43:26.070523 revChatGPT-6.0.4/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    49765 2023-06-06 06:42:56.000000 revChatGPT-6.0.4/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-06-06 06:42:56.000000 revChatGPT-6.0.4/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-06 06:42:56.000000 revChatGPT-6.0.4/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-06 06:42:56.000000 revChatGPT-6.0.4/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:43:26.070523 revChatGPT-6.0.4/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-06 06:42:56.000000 revChatGPT-6.0.4/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-06 06:42:56.000000 revChatGPT-6.0.4/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-06 06:42:56.000000 revChatGPT-6.0.4/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:43:26.070523 revChatGPT-6.0.4/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-06-06 06:43:26.000000 revChatGPT-6.0.4/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-06 06:43:26.000000 revChatGPT-6.0.4/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 06:43:26.000000 revChatGPT-6.0.4/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-06 06:43:26.000000 revChatGPT-6.0.4/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-06 06:43:26.000000 revChatGPT-6.0.4/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:43:26.070523 revChatGPT-6.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-06 06:42:56.000000 revChatGPT-6.0.4/tests/test_recipient.py
```

### Comparing `revChatGPT-6.0.3/LICENSE` & `revChatGPT-6.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.0.3/PKG-INFO` & `revChatGPT-6.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.0.3
+Version: 6.0.4
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.0.3/README.md` & `revChatGPT-6.0.4/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.0.3/setup.py` & `revChatGPT-6.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="6.0.3",
+    version="6.0.4",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-6.0.3/src/revChatGPT/V1.py` & `revChatGPT-6.0.4/src/revChatGPT/V1.py`

 * *Files 1% similar despite different names*

```diff
@@ -472,24 +472,29 @@
         if conversation_id and not parent_id:
             if conversation_id not in self.conversation_mapping:
                 if self.lazy_loading:
                     log.debug(
                         "Conversation ID %s not found in conversation mapping, try to get conversation history for the given ID",
                         conversation_id,
                     )
-                    with contextlib.suppress(Exception):
+                    try:
                         history = self.get_msg_history(conversation_id)
                         self.conversation_mapping[conversation_id] = history[
                             "current_node"
                         ]
+                    except requests.exceptions.HTTPError:
+                        print("Conversation unavailable")
                 else:
                     self.__map_conversations()
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
@@ -699,15 +704,15 @@
         :param encoding: String
         """
         url = f"{self.base_url}conversation/{convo_id}"
         response = self.session.get(url)
         self.__check_response(response)
         if encoding is not None:
             response.encoding = encoding
-        return json.loads(response.text)
+        return response.json()
 
     @logger(is_timed=True)
     def gen_title(self, convo_id: str, message_id: str) -> str:
         """
         Generate title for conversation
         """
         response = self.session.post(
```

### Comparing `revChatGPT-6.0.3/src/revChatGPT/V3.py` & `revChatGPT-6.0.4/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.0.3/src/revChatGPT/__init__.py` & `revChatGPT-6.0.4/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.0.3/src/revChatGPT/__main__.py` & `revChatGPT-6.0.4/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.0.3/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.0.4/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.0.3/src/revChatGPT/typings.py` & `revChatGPT-6.0.4/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.0.3/src/revChatGPT/utils.py` & `revChatGPT-6.0.4/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.0.3/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.0.4/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.0.3
+Version: 6.0.4
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.0.3/tests/test_recipient.py` & `revChatGPT-6.0.4/tests/test_recipient.py`

 * *Files identical despite different names*

