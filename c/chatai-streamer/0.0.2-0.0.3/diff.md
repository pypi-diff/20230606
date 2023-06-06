# Comparing `tmp/chatai-streamer-0.0.2.tar.gz` & `tmp/chatai-streamer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatai-streamer-0.0.2.tar", last modified: Mon Jun  5 16:17:57 2023, max compression
+gzip compressed data, was "chatai-streamer-0.0.3.tar", last modified: Tue Jun  6 14:04:01 2023, max compression
```

## Comparing `chatai-streamer-0.0.2.tar` & `chatai-streamer-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-05 16:17:57.803234 chatai-streamer-0.0.2/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-28 12:23:33.000000 chatai-streamer-0.0.2/LICENSE
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      604 2023-06-05 16:17:57.803234 chatai-streamer-0.0.2/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)    12612 2023-06-04 13:03:07.000000 chatai-streamer-0.0.2/README.md
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-06-05 16:17:57.803234 chatai-streamer-0.0.2/setup.cfg
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1172 2023-06-05 16:15:43.000000 chatai-streamer-0.0.2/setup.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-05 16:17:57.803234 chatai-streamer-0.0.2/src/
--rwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      929 2023-06-04 12:04:18.000000 chatai-streamer-0.0.2/src/ChatAIStreamer.py
--rwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     4560 2023-06-05 04:09:57.000000 chatai-streamer-0.0.2/src/GttsAIStreamer.py
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       83 2023-06-05 16:15:43.000000 chatai-streamer-0.0.2/src/__init__.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-05 16:17:57.803234 chatai-streamer-0.0.2/src/chatai_streamer.egg-info/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      604 2023-06-05 16:17:57.000000 chatai-streamer-0.0.2/src/chatai_streamer.egg-info/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      342 2023-06-05 16:17:57.000000 chatai-streamer-0.0.2/src/chatai_streamer.egg-info/SOURCES.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-05 16:17:57.000000 chatai-streamer-0.0.2/src/chatai_streamer.egg-info/dependency_links.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-05 16:15:43.000000 chatai-streamer-0.0.2/src/chatai_streamer.egg-info/not-zip-safe
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      104 2023-06-05 16:17:57.000000 chatai-streamer-0.0.2/src/chatai_streamer.egg-info/requires.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       39 2023-06-05 16:17:57.000000 chatai-streamer-0.0.2/src/chatai_streamer.egg-info/top_level.txt
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-06 14:04:01.573235 chatai-streamer-0.0.3/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-28 12:23:33.000000 chatai-streamer-0.0.3/LICENSE
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      604 2023-06-06 14:04:01.573235 chatai-streamer-0.0.3/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)    12831 2023-06-06 13:54:02.000000 chatai-streamer-0.0.3/README.md
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-06-06 14:04:01.573235 chatai-streamer-0.0.3/setup.cfg
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1172 2023-06-06 13:54:02.000000 chatai-streamer-0.0.3/setup.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-06 14:04:01.573235 chatai-streamer-0.0.3/src/
+-rwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      929 2023-06-04 12:04:18.000000 chatai-streamer-0.0.3/src/ChatAIStreamer.py
+-rwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     4663 2023-06-06 13:54:02.000000 chatai-streamer-0.0.3/src/GttsAIStreamer.py
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       83 2023-06-06 13:54:02.000000 chatai-streamer-0.0.3/src/__init__.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-06 14:04:01.573235 chatai-streamer-0.0.3/src/chatai_streamer.egg-info/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      604 2023-06-06 14:04:01.000000 chatai-streamer-0.0.3/src/chatai_streamer.egg-info/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      342 2023-06-06 14:04:01.000000 chatai-streamer-0.0.3/src/chatai_streamer.egg-info/SOURCES.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-06 14:04:01.000000 chatai-streamer-0.0.3/src/chatai_streamer.egg-info/dependency_links.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-06 13:54:02.000000 chatai-streamer-0.0.3/src/chatai_streamer.egg-info/not-zip-safe
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      104 2023-06-06 14:04:01.000000 chatai-streamer-0.0.3/src/chatai_streamer.egg-info/requires.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       39 2023-06-06 14:04:01.000000 chatai-streamer-0.0.3/src/chatai_streamer.egg-info/top_level.txt
```

### Comparing `chatai-streamer-0.0.2/LICENSE` & `chatai-streamer-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chatai-streamer-0.0.2/PKG-INFO` & `chatai-streamer-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatai-streamer
-Version: 0.0.2
+Version: 0.0.3
 Summary: ChatGPT answer aloud YouTube chat messages.
 Home-page: https://github.com/GeneralYadoc/ChatAIStreamer
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `chatai-streamer-0.0.2/README.md` & `chatai-streamer-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -297,14 +297,15 @@
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
```

### Comparing `chatai-streamer-0.0.2/setup.py` & `chatai-streamer-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def _requires_from_file(filename):
     return open(filename).read().splitlines()
 
 
 setup(
     name="chatai-streamer",
-    version="0.0.2",
+    version="0.0.3",
     license="MIT",
     description="ChatGPT answer aloud YouTube chat messages.",
     author="General Yadoc",
     author_email="133023047+GeneralYadoc@users.noreply.github.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         'Programming Language :: Python',
```

### Comparing `chatai-streamer-0.0.2/src/ChatAIStreamer.py` & `chatai-streamer-0.0.3/src/ChatAIStreamer.py`

 * *Files identical despite different names*

### Comparing `chatai-streamer-0.0.2/src/GttsAIStreamer.py` & `chatai-streamer-0.0.3/src/GttsAIStreamer.py`

 * *Files 9% similar despite different names*

```diff
@@ -64,42 +64,43 @@
 # voice_generator is defaultly intialized with English voiceGenerator.
 @dataclass
 class params(casr.params):
   voice_generator : casr.voiceGenerator = GttsGenerator()
 
 # VoicePlayer class which plays the voice generated by GttsGenerator.
 class VoicePlayer(threading.Thread):
-  def __init__(self, voice, volume=100):
-    self.voice = voice
-    self.volume = volume
+  def __init__(self, voice, volume=100, python_command="python3"):
+    self.__voice = voice
+    self.__volume = volume
+    self.__python_command = python_command
     super(VoicePlayer, self).__init__()
 
   def run(self):
     # Create path of temporary file.
     with tempfile.NamedTemporaryFile() as file:
       file_path = file.name + TMPFILE_POSTFIX
     # Create wave writer.
     writer = wave.open(file_path, mode='wb')
 
     # Write voice to Temporary wav file in order to receive it on subprocess.
-    writer.setsampwidth(self.voice.sample_width)
-    writer.setframerate(self.voice.frame_rate)
-    writer.setnchannels(self.voice.channels)
-    writer.writeframesraw(self.voice.content)
+    writer.setsampwidth(self.__voice.sample_width)
+    writer.setframerate(self.__voice.frame_rate)
+    writer.setnchannels(self.__voice.channels)
+    writer.writeframesraw(self.__voice.content)
 
     # Play voice on subprocess in order to suppress pydub log.
     subprocess.run(
-      [ 'python3',
+      [ self.__python_command,
          __file__,
         file_path,
-        str(self.voice.sample_width),
-        str(self.voice.frame_rate),
-        str(self.voice.channels),
-        str(self.voice.duration_seconds),
-        str(self.volume) ],
+        str(self.__voice.sample_width),
+        str(self.__voice.frame_rate),
+        str(self.__voice.channels),
+        str(self.__voice.duration_seconds),
+        str(self.__volume) ],
         stdout=subprocess.PIPE, stderr=subprocess.PIPE )
 
 # GttsAIStreamer as inheritence from ChatAIStreamer
 class GttsAIStreamer(casr.ChatAIStreamer):
   def __init__(self, params):
     # Remove garbage of temporary files.
     with tempfile.NamedTemporaryFile() as file:
```

### Comparing `chatai-streamer-0.0.2/src/chatai_streamer.egg-info/PKG-INFO` & `chatai-streamer-0.0.3/src/chatai_streamer.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatai-streamer
-Version: 0.0.2
+Version: 0.0.3
 Summary: ChatGPT answer aloud YouTube chat messages.
 Home-page: https://github.com/GeneralYadoc/ChatAIStreamer
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

