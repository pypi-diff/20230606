# Comparing `tmp/seavoice-sdk-0.2.8.post1.tar.gz` & `tmp/seavoice-sdk-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seavoice-sdk-0.2.8.post1.tar", last modified: Fri Feb 10 21:06:42 2023, max compression
+gzip compressed data, was "seavoice-sdk-0.2.9.tar", last modified: Fri Mar 17 04:04:18 2023, max compression
```

## Comparing `seavoice-sdk-0.2.8.post1.tar` & `seavoice-sdk-0.2.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 cody       (501) staff       (20)        0 2023-02-10 21:06:42.083054 seavoice-sdk-0.2.8.post1/
--rw-r--r--   0 cody       (501) staff       (20)     1074 2022-07-12 18:30:05.000000 seavoice-sdk-0.2.8.post1/LICENSE
--rw-r--r--   0 cody       (501) staff       (20)    11544 2023-02-10 21:06:42.082897 seavoice-sdk-0.2.8.post1/PKG-INFO
--rw-r--r--   0 cody       (501) staff       (20)    11062 2022-12-09 05:07:10.000000 seavoice-sdk-0.2.8.post1/README.md
-drwxr-xr-x   0 cody       (501) staff       (20)        0 2023-02-10 21:06:42.082075 seavoice-sdk-0.2.8.post1/seavoice_sdk/
--rw-r--r--   0 cody       (501) staff       (20)        0 2022-12-09 05:07:06.000000 seavoice-sdk-0.2.8.post1/seavoice_sdk/__init__.py
--rw-r--r--   0 cody       (501) staff       (20)     6567 2023-01-07 01:56:57.000000 seavoice-sdk-0.2.8.post1/seavoice_sdk/audio.py
--rw-r--r--   0 cody       (501) staff       (20)     2987 2022-12-09 05:07:06.000000 seavoice-sdk-0.2.8.post1/seavoice_sdk/logger.py
--rw-r--r--   0 cody       (501) staff       (20)    43092 2023-02-10 20:46:27.000000 seavoice-sdk-0.2.8.post1/seavoice_sdk/speech.py
--rw-r--r--   0 cody       (501) staff       (20)     4146 2022-12-09 05:07:06.000000 seavoice-sdk-0.2.8.post1/seavoice_sdk/utils.py
-drwxr-xr-x   0 cody       (501) staff       (20)        0 2023-02-10 21:06:42.082745 seavoice-sdk-0.2.8.post1/seavoice_sdk.egg-info/
--rw-r--r--   0 cody       (501) staff       (20)    11544 2023-02-10 21:06:42.000000 seavoice-sdk-0.2.8.post1/seavoice_sdk.egg-info/PKG-INFO
--rw-r--r--   0 cody       (501) staff       (20)      320 2023-02-10 21:06:42.000000 seavoice-sdk-0.2.8.post1/seavoice_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 cody       (501) staff       (20)        1 2023-02-10 21:06:42.000000 seavoice-sdk-0.2.8.post1/seavoice_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 cody       (501) staff       (20)       54 2023-02-10 21:06:42.000000 seavoice-sdk-0.2.8.post1/seavoice_sdk.egg-info/requires.txt
--rw-r--r--   0 cody       (501) staff       (20)       13 2023-02-10 21:06:42.000000 seavoice-sdk-0.2.8.post1/seavoice_sdk.egg-info/top_level.txt
--rw-r--r--   0 cody       (501) staff       (20)       38 2023-02-10 21:06:42.083094 seavoice-sdk-0.2.8.post1/setup.cfg
--rw-r--r--   0 cody       (501) staff       (20)      754 2023-02-10 21:04:02.000000 seavoice-sdk-0.2.8.post1/setup.py
+drwxr-xr-x   0 cody       (501) staff       (20)        0 2023-03-17 04:04:18.617096 seavoice-sdk-0.2.9/
+-rw-r--r--   0 cody       (501) staff       (20)     1074 2022-07-12 18:30:05.000000 seavoice-sdk-0.2.9/LICENSE
+-rw-r--r--   0 cody       (501) staff       (20)    11538 2023-03-17 04:04:18.616908 seavoice-sdk-0.2.9/PKG-INFO
+-rw-r--r--   0 cody       (501) staff       (20)    11062 2022-12-09 05:07:10.000000 seavoice-sdk-0.2.9/README.md
+drwxr-xr-x   0 cody       (501) staff       (20)        0 2023-03-17 04:04:18.616065 seavoice-sdk-0.2.9/seavoice_sdk/
+-rw-r--r--   0 cody       (501) staff       (20)        0 2022-12-09 05:07:06.000000 seavoice-sdk-0.2.9/seavoice_sdk/__init__.py
+-rw-r--r--   0 cody       (501) staff       (20)     6860 2023-03-17 03:33:50.000000 seavoice-sdk-0.2.9/seavoice_sdk/audio.py
+-rw-r--r--   0 cody       (501) staff       (20)     2987 2022-12-09 05:07:06.000000 seavoice-sdk-0.2.9/seavoice_sdk/logger.py
+-rw-r--r--   0 cody       (501) staff       (20)    43382 2023-03-17 03:38:30.000000 seavoice-sdk-0.2.9/seavoice_sdk/speech.py
+-rw-r--r--   0 cody       (501) staff       (20)     4146 2022-12-09 05:07:06.000000 seavoice-sdk-0.2.9/seavoice_sdk/utils.py
+drwxr-xr-x   0 cody       (501) staff       (20)        0 2023-03-17 04:04:18.616685 seavoice-sdk-0.2.9/seavoice_sdk.egg-info/
+-rw-r--r--   0 cody       (501) staff       (20)    11538 2023-03-17 04:04:18.000000 seavoice-sdk-0.2.9/seavoice_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 cody       (501) staff       (20)      320 2023-03-17 04:04:18.000000 seavoice-sdk-0.2.9/seavoice_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 cody       (501) staff       (20)        1 2023-03-17 04:04:18.000000 seavoice-sdk-0.2.9/seavoice_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 cody       (501) staff       (20)       54 2023-03-17 04:04:18.000000 seavoice-sdk-0.2.9/seavoice_sdk.egg-info/requires.txt
+-rw-r--r--   0 cody       (501) staff       (20)       13 2023-03-17 04:04:18.000000 seavoice-sdk-0.2.9/seavoice_sdk.egg-info/top_level.txt
+-rw-r--r--   0 cody       (501) staff       (20)       38 2023-03-17 04:04:18.617142 seavoice-sdk-0.2.9/setup.cfg
+-rw-r--r--   0 cody       (501) staff       (20)      752 2023-03-17 04:01:22.000000 seavoice-sdk-0.2.9/setup.py
```

### Comparing `seavoice-sdk-0.2.8.post1/LICENSE` & `seavoice-sdk-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `seavoice-sdk-0.2.8.post1/PKG-INFO` & `seavoice-sdk-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seavoice-sdk
-Version: 0.2.8.post1
+Version: 0.2.9
 Summary: SeaVoice SDK: Client for Seasalt speech recognition and speech synthesis.
 Home-page: UNKNOWN
 Author: Seasalt.ai
 Author-email: info@seasalt.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `seavoice-sdk-0.2.8.post1/README.md` & `seavoice-sdk-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `seavoice-sdk-0.2.8.post1/seavoice_sdk/audio.py` & `seavoice-sdk-0.2.9/seavoice_sdk/audio.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 from typing import (
     Optional,
     Text
 )
 import queue
 
+from seavoice_sdk import logger
+svc_logger = logger.get_SVCLogger(__name__)
 
 class AudioStreamFormat():
     """audio configuration"""
 
     def __init__(
         self,
         samples_per_second: int = 16000,
@@ -56,25 +58,29 @@
         self.__buffer_space = None
 
     def write(self, buffer: bytes):
         """Write buffer to __buffer_space"""
         if self.is_closed is False:
             self.__buffer_space.put(buffer)
         else:
-            raise RuntimeError("Stream has been closed")
+            self.__buffer_space = queue.Queue(maxsize=1000)
+            self.__buffer_space.put(buffer)
+            svc_logger.warn("Write failed: Stream has been closed")
+            self.is_closed = False
 
     def read(self):
         """Read bytes from __buffer_space, nowait"""
         if self.is_closed is False:
             if self.__buffer_space.empty() is False:
                 return self.__buffer_space.get_nowait()
             else:
                 return None
         else:
-            raise RuntimeError("Stream has been closed")
+            self.__buffer_space = queue.Queue(maxsize=1000)
+            svc_logger.warn("Read Failed: Stream has been closed")
 
     def read_wait(self):
         """Read bytes from __buffer_space, wait until get"""
         if self.is_closed is False:
             return self.__buffer_space.get()
         else:
             raise RuntimeError("Stream has been closed")
@@ -108,15 +114,15 @@
         self.__output_stream = None
 
     def write(self, buffer: bytes):
         """Write buffer to output_stream"""
         if self.is_closed is False:
             self.__output_stream.put(buffer)
         else:
-            raise RuntimeError("Stream has been closed")
+            svc_logger.warn("Stream has been closed")
 
     def read(self):
         """Read bytes from __output_stream, nowait"""
         if self.is_closed is False:
             return self.__output_stream.get_nowait()
         else:
             raise RuntimeError("Stream has been closed")
```

### Comparing `seavoice-sdk-0.2.8.post1/seavoice_sdk/logger.py` & `seavoice-sdk-0.2.9/seavoice_sdk/logger.py`

 * *Files identical despite different names*

### Comparing `seavoice-sdk-0.2.8.post1/seavoice_sdk/speech.py` & `seavoice-sdk-0.2.9/seavoice_sdk/speech.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 SUPPORTED_AUDIO_FORMAT = {
     "riff-8khz-16bit-mono-pcm": {"sample_rate": 8000, "sample_width": 2, "channels": 1},
     "riff-16khz-16bit-mono-pcm": {"sample_rate": 16000, "sample_width": 2, "channels": 1},
     "riff-22khz-16bit-mono-pcm": {"sample_rate": 22050, "sample_width": 2, "channels": 1},
 }
 ERROR_IN_SEND_THREAD = 11000
 
-
 class SpeechConfig:
     """Setup speech arguments"""
 
     def __init__(
         self,
         host: Optional[Text] = "",
         account_id: Text = "",
@@ -329,33 +328,36 @@
         self.__session_started_event = EventSignal()
         self.__session_stopped_event = EventSignal()
         self.__recognizing_event = EventSignal()
         self.__recognized_event = EventSignal()
         self.__canceled_event = EventSignal()
         self.session_id = None
 
-        #TODO: Turn off monitoring
-        # stats for monitoring session
-        self.reconnecting = False
-        self.monitor_session = False
+        # stats for monitoring session (deprecated)
+        self.monitor_session = False # Deprecated in v0.2.6
         self.connection_id = str(uuid.uuid4())
         self.seconds_received = 0
+        if monitor_session == True:
+            svc_logger.warn("Session monitoring was deprecated in v0.2.6")
+
+        self.reconnecting = False
 
         # Speech Recognition itn options
         self.itn = itn
         self.punctuation = punctuation
         
         if self.__input_stream:
             sample_rate = self.__input_stream.stream_format.samples_per_second
         else:
             sample_rate = 48000
         svc_logger.info(f"Sample Rate: {sample_rate}, ITN: {self.itn}, Punctuation: {self.punctuation}")
 
         # init websocket client
-        self.ws = self.RecognizerWebSocket(self.__ws_uri, [("sample_rate",sample_rate), ("itn",self.itn), ("punctuation",self.punctuation)], self)
+        self.sample_rate = sample_rate
+        self.ws = self.RecognizerWebSocket(self.__ws_uri, [("sample_rate",self.sample_rate), ("itn",self.itn), ("punctuation",self.punctuation)], self)
 
     def get_server_url_token(self) -> bool:
         """get stt server url and speech token by login token"""
         headers = {"Content-Type": "text/plain", "token": self.__login_token}
         response = requests.post(
             API_SERVER_STT_SERVICE_URL_TOKEN, headers=headers, json={"language": self.__speech_recognition_language}
         )
@@ -399,15 +401,15 @@
             self.ws.send("EOS")
 
     def start_continuous_recognition_async(self):
         """Start continuous speech recognition in asynchronized way"""
         self.is_running = True
         if self.reconnecting:
             self.reconnecting = False
-            self.ws = self.RecognizerWebSocket(self.__ws_uri, self)
+            self.ws = self.RecognizerWebSocket(self.__ws_uri, [("sample_rate",self.sample_rate), ("itn",self.itn), ("punctuation",self.punctuation)], self)
            
         if self.ws:
             self.ws.connect()
             recognition_thread = threading.Thread(
                 target=self.send_thread,
             )
             recognition_thread.daemon = True
@@ -475,14 +477,15 @@
                 evt = {"session_id": self.session_id}
                 evt_res = EventResults(evt)
                 self.__session_stopped_event.callback(evt_res)
         except Exception as e:
             svc_logger.error(f"Exception in continuous_recognition_async: {e}")
 
     def send_thread(self):
+        global i
         """Send data to websocket"""
         error_flag = False
 
         if self.monitor_session:
             data = {
                 "event": "start",
                 "connection_id": self.connection_id,
@@ -501,16 +504,16 @@
 
                     self.update_seconds_received(len(buf))
                     
                     if not self.ws.stream:
                         svc_logger.warning("The ws has been disconnected, trying to reconnect..")
                         self.reconnecting = True
                         self.start_continuous_recognition()
-
-                    self.ws.send(buf, binary=True)
+                    else:
+                        self.ws.send(buf, binary=True)
 
             except KeyboardInterrupt:
                 error_flag = True
                 self.stop_continuous_recognition_async()
             except Exception as e:
                 svc_logger.error(f"Exception in send_thread: {e}")
                 error_flag = True
```

### Comparing `seavoice-sdk-0.2.8.post1/seavoice_sdk/utils.py` & `seavoice-sdk-0.2.9/seavoice_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `seavoice-sdk-0.2.8.post1/seavoice_sdk.egg-info/PKG-INFO` & `seavoice-sdk-0.2.9/seavoice_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seavoice-sdk
-Version: 0.2.8.post1
+Version: 0.2.9
 Summary: SeaVoice SDK: Client for Seasalt speech recognition and speech synthesis.
 Home-page: UNKNOWN
 Author: Seasalt.ai
 Author-email: info@seasalt.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `seavoice-sdk-0.2.8.post1/setup.py` & `seavoice-sdk-0.2.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="seavoice-sdk",
-    version="0.2.8-1",
+    version="0.2.9",
     author="Seasalt.ai",
     author_email="info@seasalt.ai",
     description="SeaVoice SDK: Client for Seasalt speech recognition and speech synthesis.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=[
```

