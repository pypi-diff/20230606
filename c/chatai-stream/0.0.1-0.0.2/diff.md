# Comparing `tmp/chatai-stream-0.0.1.tar.gz` & `tmp/chatai-stream-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatai-stream-0.0.1.tar", last modified: Sun May 28 11:26:44 2023, max compression
+gzip compressed data, was "chatai-stream-0.0.2.tar", last modified: Tue Jun  6 12:57:24 2023, max compression
```

## Comparing `chatai-stream-0.0.1.tar` & `chatai-stream-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-05-28 11:26:44.327405 chatai-stream-0.0.1/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-28 11:25:30.000000 chatai-stream-0.0.1/LICENSE
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      594 2023-05-28 11:26:44.327405 chatai-stream-0.0.1/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     7988 2023-05-28 11:25:30.000000 chatai-stream-0.0.1/README.md
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-05-28 11:26:44.327405 chatai-stream-0.0.1/setup.cfg
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1161 2023-05-28 11:25:31.000000 chatai-stream-0.0.1/setup.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-05-28 11:26:44.327405 chatai-stream-0.0.1/src/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1751 2023-05-28 11:25:31.000000 chatai-stream-0.0.1/src/ChatAIStream.py
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       50 2023-05-28 11:25:31.000000 chatai-stream-0.0.1/src/__init__.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-05-28 11:26:44.327405 chatai-stream-0.0.1/src/chatai_stream.egg-info/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      594 2023-05-28 11:26:44.000000 chatai-stream-0.0.1/src/chatai_stream.egg-info/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      306 2023-05-28 11:26:44.000000 chatai-stream-0.0.1/src/chatai_stream.egg-info/SOURCES.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-05-28 11:26:44.000000 chatai-stream-0.0.1/src/chatai_stream.egg-info/dependency_links.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-05-28 11:26:44.000000 chatai-stream-0.0.1/src/chatai_stream.egg-info/not-zip-safe
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       44 2023-05-28 11:26:44.000000 chatai-stream-0.0.1/src/chatai_stream.egg-info/requires.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       22 2023-05-28 11:26:44.000000 chatai-stream-0.0.1/src/chatai_stream.egg-info/top_level.txt
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-06 12:57:24.373233 chatai-stream-0.0.2/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-28 11:25:30.000000 chatai-stream-0.0.2/LICENSE
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      594 2023-06-06 12:57:24.373233 chatai-stream-0.0.2/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     8103 2023-06-06 12:52:21.000000 chatai-stream-0.0.2/README.md
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-06-06 12:57:24.373233 chatai-stream-0.0.2/setup.cfg
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1162 2023-06-06 12:52:21.000000 chatai-stream-0.0.2/setup.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-06 12:57:24.373233 chatai-stream-0.0.2/src/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1582 2023-06-06 12:52:21.000000 chatai-stream-0.0.2/src/ChatAIStream.py
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       51 2023-06-06 12:52:21.000000 chatai-stream-0.0.2/src/__init__.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-06 12:57:24.373233 chatai-stream-0.0.2/src/chatai_stream.egg-info/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      594 2023-06-06 12:57:24.000000 chatai-stream-0.0.2/src/chatai_stream.egg-info/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      306 2023-06-06 12:57:24.000000 chatai-stream-0.0.2/src/chatai_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-06 12:57:24.000000 chatai-stream-0.0.2/src/chatai_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-06 12:52:21.000000 chatai-stream-0.0.2/src/chatai_stream.egg-info/not-zip-safe
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       44 2023-06-06 12:57:24.000000 chatai-stream-0.0.2/src/chatai_stream.egg-info/requires.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       22 2023-06-06 12:57:24.000000 chatai-stream-0.0.2/src/chatai_stream.egg-info/top_level.txt
```

### Comparing `chatai-stream-0.0.1/LICENSE` & `chatai-stream-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chatai-stream-0.0.1/PKG-INFO` & `chatai-stream-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatai-stream
-Version: 0.0.1
+Version: 0.0.2
 Summary: ChatGPT reacts YouTube chat messages.
 Home-page: https://github.com/GeneralYadoc/ChatAIStream
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `chatai-stream-0.0.1/README.md` & `chatai-stream-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # ChatAIStream
 Message broker between YouTube chat stream and ChatGPT.
 
 ## The user of this library can
 - pick up massegase from YouTube Chat and generate answer by ChatGPT.
 - easily give role to ChatGPT.
 
-## Hou to install
+## How to install
 
 ### Install from PyPI
 - Install package to your environment.<br>
     ```install
     $ pip install chatai-stream
     ```
 
@@ -27,23 +27,21 @@
   $ pip install .
   ```
 ## How to use
 - [OpenAI API Key](https://www.howtogeek.com/885918/how-to-get-an-openai-api-key/) is necessary to execute following sample.
 
 - Sample codes exist [here](samples/sample.py).
   ``` sample.py
-  # To execute this sample, please install streamchat-agent from PyPI as follows.
-  # $ pip install streamchat-agent
   import sys
   import time
   import math
   import datetime
   import ChatAIStream as cas
 
-  # print sentencce by a character incrementally.
+  # print sentence by a character incrementally.
   def print_incremental(st, interval_sec):
     for i in range(len(st)):
       if not running:
         break
       print(f"{st[i]}", end='')
       sys.stdout.flush()
       interruptible_sleep(interval_sec)
@@ -94,15 +92,15 @@
 
   # Wake up internal thread to get chat messages from stream and ChatGPT answers.
   ai_stream.start()
 
   # Wait any key inputted from keyboad.
   input()
 
-  # Turn off runnging flag in order to finish printing fung of dhit sample.
+  # Turn off runnging flag in order to finish printing messages and answers by the sample.
   running=False
 
   # Finish getting ChatGPT answers.
   # Internal thread will stop soon.
   ai_stream.disconnect()
 
   # terminating internal thread.
@@ -110,15 +108,15 @@
 
   del ai_stream
 
   ```
 
 - Usage of the sample
   ```usage
-  $ python3 ./sample2.py VIDEO-ID OpenAI-API-KEY
+  $ python3 ./sample.py VIDEO-ID OpenAI-API-KEY
   ```
 - Output of the sample<br>
   The outputs of the right window are provided by this sample.<br>
   Left outputs are also available by ChatAIStream.
   ![](ReadMeParts/ChatAIAgent.gif)
 
 ## Arguments of Constructor
@@ -135,25 +133,25 @@
     | interval_sec | Polling interval of picking up items from YouTube | 0.01 \[sec\] | 
   ### aiParams
 
 
     | name | description | default |
     |------|------------|---------|
     | api_key | API Key string of OpenAI | - |
-    | system_role | API Key string of OpenAI | "You are a helpful assistant." |
+    | system_role | ChatGPT role in convesation | "You are a helpful assistant." |
     | ask_cb | user message given to ChatGPT is thrown to this callback | None |
     | max_messages_in_context | Max messages in context given to ChatGPT | 20 |
     | answer_cb | ChatGPT answer is thrown to this callback | None |
     | max_queue_size | Max slots of internal queue (0 is no limit) | 10 |
     | model | Model of AI to be used. | None |
     | max_tokens_per_request | Max number of tokens which can be contained in a request. | 256 |
     | interval_sec | Interval of ChatGPT API call | 20.0 \[sec\] | 
 ### Notice
 - Please refer [pytchat README](https://github.com/taizan-hokuto/pytchat) to know the type of YouTube Chat item used by get_item_cb, pre_filter_cb and post filter_cb.
-- Stamps in a message and messages consisted by stamps only are removed defaultly even if user doesn't set pre_filter_cb.
+- Emoticons in a message and messages consisted by emoticons only are removed defaultly even if user doesn't set pre_filter_cb.
 - Default value of interval_sec is 20.0, since free user of OpenAI API can get only 3 completions per minitue.
 - The system role given by user remains ever as the oldest sentence of current context even if the number of messages is reached to the maximum, so ChatGPT doesn't forgot the role while current cunversation.
 
 ## Methods
 ### start()
 - Start YouTube Chat polling and ChatGPT conversation, then start calling user callbacks asyncronously.
 - No arguments required, nothing returns.
@@ -180,14 +178,15 @@
 - You can implement several processes in it.
 - YouTube chat item is thrown as an argument.
 - It's not be assumed that any values are returned.
 ### pre_filter_cb
 - pre putting queue filter.
 - YouTube chat item is thrown as an argument.
 - You can edit YouTube chat items before putting internal queue.
+- <b>If you want to get Complete items from YouTube, please implement this callback, since emoticons in a message and messages consisted by emoticons only are already removed from the items gotten in get_item_cb.</b> 
 - It's required that edited chat item is returned.
 - You can avoid putting internal queue by returning None.
 ### post_filter_cb
 - post getting queue filter
 - You can edit YouTube chat items after popping internal queue.
 - It's required that edited chat item is returned.
 - You can avoid sending item to get_item_cb by returning None.
@@ -197,13 +196,13 @@
 - It's not be assumed that any values are returned.
 ### answer_cb
 - Callback for getting question and answer of ChatGPT
 - The type of completion is mentioned [here](https://platform.openai.com/docs/guides/chat).
 - It's not be assumed that any values are returned.
 
 ## Links
-StreamingChaatAgent uses following libraries internally.
+ChatAIStream uses following libraries internally.
 
 - [streamchat-agent](https://github.com/GeneralYadoc/StreamChatAgent)<br>
  YouTube chat poller which can get massages very smothly by using internal queue.
 - [chatai-agent](https://github.com/GeneralYadoc/ChatAIAgent)<br>
  Message broker between user and ChatGPT.
```

### Comparing `chatai-stream-0.0.1/setup.py` & `chatai-stream-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def _requires_from_file(filename):
     return open(filename).read().splitlines()
 
 
 setup(
     name="chatai-stream",
-    version="0.0.1",
+    version="0.0.2",
     license="MIT",
     description="ChatGPT reacts YouTube chat messages.",
     author="General Yadoc",
     author_email="133023047+GeneralYadoc@users.noreply.github.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         'Programming Language :: Python',
@@ -30,8 +30,8 @@
     package_dir={"": "src"},
     py_modules=[splitext(basename(path))[0] for path in glob('src/*.py')],
     include_package_data=True,
     zip_safe=False,
     install_requires=_requires_from_file('requirements.txt'),
     setup_requires=["pytest-runner"],
     tests_require=["pytest", "pytest-cov"]
-)
+)
```

### Comparing `chatai-stream-0.0.1/src/ChatAIStream.py` & `chatai-stream-0.0.2/src/ChatAIStream.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,31 +13,26 @@
 class params():
   stream_params: streamParams
   ai_params: aiParams
 
 class ChatAIStream(threading.Thread):
   def my_pre_filter_cb(self, c):
     prefiltered_c = c
-    prefiltered_c.message = re.sub(r':[^:]+:', ".", prefiltered_c.message)
-    prefiltered_c.message = re.sub(r'^[\.]+', "", prefiltered_c.message)
     if prefiltered_c and self.pre_filter_cb:
       prefiltered_c = self.pre_filter_cb(prefiltered_c)
+    prefiltered_c.message = re.sub(r':[^:]+:', ".", prefiltered_c.message)
+    prefiltered_c.message = re.sub(r'^[\.]+', "", prefiltered_c.message)
     return None if prefiltered_c.message == "" else prefiltered_c
 
   def ask_stream_message_to_ai(self, c):
     if self.get_stream_message_cb:
       self.get_stream_message_cb(c)
     if self.ai_agent:
       self.ai_agent.put_message(ca.userMessage(message=c.message, extern=c))
   
-  def default_answer_cb(self, user_message, completion):
-    print("testtest")
-    answer = completion.choices[0]["message"]["content"]
-    print(f"[Answer] {answer}")
-
   def __init__( self, params):
     self.get_stream_message_cb=params.stream_params.get_item_cb
     params.stream_params.get_item_cb=self.ask_stream_message_to_ai
     self.pre_filter_cb=params.stream_params.pre_filter_cb
     params.stream_params.pre_filter_cb=self.my_pre_filter_cb
 
     self.ai_agent = ca.ChatAIAgent( params.ai_params )
```

### Comparing `chatai-stream-0.0.1/src/chatai_stream.egg-info/PKG-INFO` & `chatai-stream-0.0.2/src/chatai_stream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatai-stream
-Version: 0.0.1
+Version: 0.0.2
 Summary: ChatGPT reacts YouTube chat messages.
 Home-page: https://github.com/GeneralYadoc/ChatAIStream
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

