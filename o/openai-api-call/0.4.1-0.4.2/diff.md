# Comparing `tmp/openai_api_call-0.4.1.tar.gz` & `tmp/openai_api_call-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_api_call-0.4.1.tar", last modified: Sun May 28 02:54:32 2023, max compression
+gzip compressed data, was "openai_api_call-0.4.2.tar", last modified: Tue Jun  6 15:13:35 2023, max compression
```

## Comparing `openai_api_call-0.4.1.tar` & `openai_api_call-0.4.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 02:54:32.063508 openai_api_call-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-28 02:54:21.000000 openai_api_call-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-05-28 02:54:32.063508 openai_api_call-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-28 02:54:21.000000 openai_api_call-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 02:54:32.063508 openai_api_call-0.4.1/openai_api_call/
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-28 02:54:21.000000 openai_api_call-0.4.1/openai_api_call/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-05-28 02:54:21.000000 openai_api_call-0.4.1/openai_api_call/chattool.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-28 02:54:21.000000 openai_api_call-0.4.1/openai_api_call/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-28 02:54:21.000000 openai_api_call-0.4.1/openai_api_call/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-28 02:54:21.000000 openai_api_call-0.4.1/openai_api_call/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-28 02:54:21.000000 openai_api_call-0.4.1/openai_api_call/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 02:54:32.063508 openai_api_call-0.4.1/openai_api_call.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-05-28 02:54:31.000000 openai_api_call-0.4.1/openai_api_call.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-28 02:54:32.000000 openai_api_call-0.4.1/openai_api_call.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 02:54:31.000000 openai_api_call-0.4.1/openai_api_call.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-28 02:54:31.000000 openai_api_call-0.4.1/openai_api_call.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 02:54:31.000000 openai_api_call-0.4.1/openai_api_call.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-28 02:54:31.000000 openai_api_call-0.4.1/openai_api_call.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-28 02:54:31.000000 openai_api_call-0.4.1/openai_api_call.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 02:54:32.063508 openai_api_call-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-28 02:54:21.000000 openai_api_call-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:13:35.454256 openai_api_call-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-06 15:13:24.000000 openai_api_call-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-06-06 15:13:35.454256 openai_api_call-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-06 15:13:24.000000 openai_api_call-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:13:35.450256 openai_api_call-0.4.2/openai_api_call/
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-06-06 15:13:24.000000 openai_api_call-0.4.2/openai_api_call/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-06-06 15:13:24.000000 openai_api_call-0.4.2/openai_api_call/chattool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-06 15:13:24.000000 openai_api_call-0.4.2/openai_api_call/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-06 15:13:24.000000 openai_api_call-0.4.2/openai_api_call/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-06 15:13:24.000000 openai_api_call-0.4.2/openai_api_call/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-06 15:13:24.000000 openai_api_call-0.4.2/openai_api_call/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:13:35.454256 openai_api_call-0.4.2/openai_api_call.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-06-06 15:13:35.000000 openai_api_call-0.4.2/openai_api_call.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-06 15:13:35.000000 openai_api_call-0.4.2/openai_api_call.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 15:13:35.000000 openai_api_call-0.4.2/openai_api_call.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-06 15:13:35.000000 openai_api_call-0.4.2/openai_api_call.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 15:13:35.000000 openai_api_call-0.4.2/openai_api_call.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-06 15:13:35.000000 openai_api_call-0.4.2/openai_api_call.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-06 15:13:35.000000 openai_api_call-0.4.2/openai_api_call.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 15:13:35.454256 openai_api_call-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-06 15:13:24.000000 openai_api_call-0.4.2/setup.py
```

### Comparing `openai_api_call-0.4.1/LICENSE` & `openai_api_call-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.4.1/PKG-INFO` & `openai_api_call-0.4.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_api_call
-Version: 0.4.1
+Version: 0.4.2
 Summary: A short wrapper of the OpenAI api call.
 Home-page: https://github.com/cubenlp/openai_api_call
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: > **中文文档移步[这里](README_zh_CN.md)。**
         
@@ -152,14 +152,47 @@
         chat.show_usage_status()
         
         # show usage status of the specified API key
         chat.api_key = "sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
         chat.show_usage_status()
         ```
         
+        ### Advance usage
+        
+        Save the chat history to a file:
+        
+        ```python
+        checkpoint = "tmp.log"
+        # chat 1
+        chat = Chat()
+        chat.save(checkpoint, mode="w") # default to "a"
+        # chat 2
+        chat = Chat("hello!")
+        chat.save(checkpoint)
+        # chat 3
+        chat.assistant("你好, how can I assist you today?")
+        chat.save(checkpoint)
+        ```
+        
+        Load the chat history from a file:
+        
+        ```python
+        # load chats(default)
+        chats = load_chats(checkpoint)
+        assert chats == [Chat(log) for log in chat_logs]
+        # load chat log only
+        chat_logs = load_chats(checkpoint, chat_log_only=True)
+        assert chat_logs == [[], [{'role': 'user', 'content': 'hello!'}],
+                              [{'role': 'user', 'content': 'hello!'}, 
+                               {'role': 'assistant', 'content': '你好, how can I assist you today?'}]]
+        # load the last message only
+        chat_msgs = load_chats(checkpoint, last_message_only=True)
+        assert chat_msgs == ["", "hello!", "你好, how can I assist you today?"]
+        ```
+        
         ## License
         
         This package is licensed under the MIT license. See the LICENSE file for more details.
         
         ## update log
         
         - Since version `0.2.0`, `Chat` type is used to handle data
```

### Comparing `openai_api_call-0.4.1/openai_api_call/__init__.py` & `openai_api_call-0.4.2/openai_api_call/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Top-level package for Openai API call."""
 
 __author__ = """Rex Wang"""
 __email__ = '1073853456@qq.com'
-__version__ = '0.4.1'
+__version__ = '0.4.2'
 
 import os
-from .chattool import Chat, Resp, chat_completion, usage_status
+from .chattool import Chat, Resp, chat_completion, usage_status, load_chats
 from .proxy import proxy_on, proxy_off, proxy_status
 import requests
 from . import request
 
 
 # read API key from the environment variable
 if os.environ.get('OPENAI_API_KEY') is not None:
@@ -39,16 +39,28 @@
 
 def show_base_url():
     """Show the base url of the API call"""
     print(f"Base url:\t{request.base_url}")
 
 def debug_log( net_url:str="https://www.baidu.com"
              , timeout:int=5
+             , message:str="hello world! 你好！"
              , test_usage:bool=True
              , test_response:bool=True):
+    """Debug the API call
+
+    Args:
+        net_url (str, optional): The url to test the network. Defaults to "https://www.baidu.com".
+        timeout (int, optional): The timeout for the network test. Defaults to 5.
+        test_usage (bool, optional): Whether to test the usage status. Defaults to True.
+        test_response (bool, optional): Whether to test the hello world. Defaults to True.
+    
+    Returns:
+        bool: True if the debug is finished.
+    """
     # 1. Test whether the network is available
     try:
         requests.get(net_url, timeout=timeout)
     except:
         print("Warning: Network is not available.")
         return False
     
@@ -72,14 +84,14 @@
     # 5. Get usage status
     if test_usage:
         print("\nThe usage status of your API key:")
         Chat().show_usage_status(recent=3)
 
     # 6. Test hello world
     if test_response:
-        print("\nTest hello world:")
-        chat = Chat("hello world")
+        print("\nTest message:", message)
+        chat = Chat(message)
         chat.getresponse(max_requests=3)
         chat.print_log()
 
     print("\nDebug is finished.")
     return True
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openai_api_call-0.4.1/openai_api_call/chattool.py` & `openai_api_call-0.4.2/openai_api_call/chattool.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import List, Dict, Union
 import openai_api_call
 from .response import Resp
 from .request import chat_completion, usage_status
 import signal, time, random
 import datetime
 import json
+import warnings
 
 # timeout handler
 def handler(signum, frame):
     raise Exception("API call timed out!")
 
 class Chat():
     def __init__( self
@@ -176,28 +177,31 @@
         """Clear the chat log"""
         self._chat_log = []
     
     def copy(self):
         """Copy the chat log"""
         return Chat(self._chat_log)
 
-    def save(self, path:str, mode:str='a', end:str='\n'):
+    def save(self, path:str, mode:str='a', end:str='\n', chatid:int=-1):
         """
         Save the chat log to a file
 
         Args:
             path (str): path to the file
             mode (str, optional): mode to open the file. Defaults to 'a'.
             end (str, optional): end of each line. Defaults to '\n'.
+            chatid (int, optional): chat id. Defaults to -1.
         """
         assert mode in ['a', 'w'], "mode should be 'a' or 'w'"
         data = self.chat_log
+        if chatid >= 0:
+            data = {'chatid': chatid, 'chatlog': data}
         with open(path, mode, encoding='utf-8') as f:
             f.write(json.dumps(data, ensure_ascii=False) + end)
-        return True
+        return
         
     def print_log(self, sep: Union[str, None]=None):
         """Print the chat log"""
         if sep is None:
             sep = '\n' + '-'*15 + '\n'
         for d in self._chat_log:
             print(sep, d['role'], sep, d['content'])
@@ -216,11 +220,68 @@
         return len(self._chat_log)
     
     def __repr__(self) -> str:
         return f"<Chat with {len(self)} messages>"
     
     def __str__(self) -> str:
         return self.__repr__()
+    
+    def __eq__(self, chat: object) -> bool:
+        if isinstance(chat, Chat):
+            return self._chat_log == chat._chat_log
+        return False
 
     def __getitem__(self, index):
         """Get the message at index"""
-        return self._chat_log[index]['content']
+        return self._chat_log[index]['content']
+
+def load_chats( checkpoint:str
+              , sep='\n'
+              , last_message_only:bool=False
+              , chat_log_only:bool=False
+              , chat_size:int=0):
+    """Load chats from a checkpoint file
+    
+    Args:
+        checkpoint (str): path to the checkpoint file
+        sep (str, optional): separator of chats. Defaults to '\n'.
+        last_message_only (bool, optional): whether to return the last message of each chat. Defaults to False.
+        chat_log_only (bool, optional): whether to return the chat log only. Defaults to False.
+        chat_size (int, optional): number of chats. Defaults to 0.
+
+    Returns:
+        list: chats
+    """
+    # load chats from the checkpoint file
+    with open(checkpoint, 'r', encoding='utf-8') as f:
+        txts = f.read().strip().split(sep)
+    chats = [json.loads(txt) for txt in txts]
+    # no chats
+    if not len(chats): return []
+    # number of chats
+    if chat_size == 0:
+        chat_size = len(chats)
+    # chats with chatid
+    if 'chatid' in chats[0]:
+        chatlogs = [None] * chat_size
+        for chat in chats:
+            idx = chat['chatid']
+            if idx >= chat_size:
+                warnings.warn(f"chatid {idx} is out of the default chat size {chat_size}")
+                chatlogs.extend([None] * (idx - chat_size + 1))
+                chat_size = idx + 1
+            chatlogs[idx] = chat['chatlog']
+    else:
+        # chats without chatid
+        chatlogs = chats
+    # last message of chats only
+    if last_message_only:
+        msgs = [None] * len(chatlogs)
+        for i, chat in enumerate(chatlogs):
+            if chat is None: continue
+            msgs[i] = chat[-1]['content'] if len(chat) else ""
+        return msgs
+    # chat log only
+    if chat_log_only:
+        return chatlogs
+    # return Chat class
+    return [Chat(chatlog) if chatlog is not None else None for chatlog in chatlogs]
```

### Comparing `openai_api_call-0.4.1/openai_api_call/proxy.py` & `openai_api_call-0.4.2/openai_api_call/proxy.py`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.4.1/openai_api_call/request.py` & `openai_api_call-0.4.2/openai_api_call/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         warnings.warn("The `url` parameter is deprecated. Please use `base_url` instead.", DeprecationWarning)
         chat_url = url
     else:
         chat_url = os.path.join(base_url, "v1/chat/completions")
     
     chat_url = normalize_url(chat_url)
     # get response
-    response = requests.post(chat_url, headers=headers, data=json.dumps(payload, ensure_ascii=False))
+    response = requests.post(chat_url, headers=headers, data=json.dumps(payload))
     if response.status_code != 200:
         raise Exception(response.text)
     return response.json()
 
 def usage_status(api_key:str, duration:int=99):
     """Get usage status
```

### Comparing `openai_api_call-0.4.1/openai_api_call/response.py` & `openai_api_call-0.4.2/openai_api_call/response.py`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.4.1/openai_api_call.egg-info/PKG-INFO` & `openai_api_call-0.4.2/openai_api_call.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-api-call
-Version: 0.4.1
+Version: 0.4.2
 Summary: A short wrapper of the OpenAI api call.
 Home-page: https://github.com/cubenlp/openai_api_call
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: > **中文文档移步[这里](README_zh_CN.md)。**
         
@@ -152,14 +152,47 @@
         chat.show_usage_status()
         
         # show usage status of the specified API key
         chat.api_key = "sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
         chat.show_usage_status()
         ```
         
+        ### Advance usage
+        
+        Save the chat history to a file:
+        
+        ```python
+        checkpoint = "tmp.log"
+        # chat 1
+        chat = Chat()
+        chat.save(checkpoint, mode="w") # default to "a"
+        # chat 2
+        chat = Chat("hello!")
+        chat.save(checkpoint)
+        # chat 3
+        chat.assistant("你好, how can I assist you today?")
+        chat.save(checkpoint)
+        ```
+        
+        Load the chat history from a file:
+        
+        ```python
+        # load chats(default)
+        chats = load_chats(checkpoint)
+        assert chats == [Chat(log) for log in chat_logs]
+        # load chat log only
+        chat_logs = load_chats(checkpoint, chat_log_only=True)
+        assert chat_logs == [[], [{'role': 'user', 'content': 'hello!'}],
+                              [{'role': 'user', 'content': 'hello!'}, 
+                               {'role': 'assistant', 'content': '你好, how can I assist you today?'}]]
+        # load the last message only
+        chat_msgs = load_chats(checkpoint, last_message_only=True)
+        assert chat_msgs == ["", "hello!", "你好, how can I assist you today?"]
+        ```
+        
         ## License
         
         This package is licensed under the MIT license. See the LICENSE file for more details.
         
         ## update log
         
         - Since version `0.2.0`, `Chat` type is used to handle data
```

### Comparing `openai_api_call-0.4.1/setup.py` & `openai_api_call-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
-VERSION = '0.4.1'
+VERSION = '0.4.2'
 
 requirements = ['Click>=7.0', 'requests>=2.20']
 
 test_requirements = ['pytest>=3', 'unittest']
 
 setup(
     author="Rex Wang",
```

