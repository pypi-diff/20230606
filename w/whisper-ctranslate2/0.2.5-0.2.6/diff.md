# Comparing `tmp/whisper-ctranslate2-0.2.5.tar.gz` & `tmp/whisper-ctranslate2-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper-ctranslate2-0.2.5.tar", last modified: Sat May 27 11:31:40 2023, max compression
+gzip compressed data, was "whisper-ctranslate2-0.2.6.tar", last modified: Tue Jun  6 05:27:30 2023, max compression
```

## Comparing `whisper-ctranslate2-0.2.5.tar` & `whisper-ctranslate2-0.2.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-27 11:31:40.077345 whisper-ctranslate2-0.2.5/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.2.5/LICENSE
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5623 2023-05-27 11:31:40.077345 whisper-ctranslate2-0.2.5/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4990 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.2.5/README.md
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2023-05-27 11:31:40.077345 whisper-ctranslate2-0.2.5/setup.cfg
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1501 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.2.5/setup.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-27 11:31:40.073345 whisper-ctranslate2-0.2.5/src/
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-27 11:31:40.073345 whisper-ctranslate2-0.2.5/src/whisper_ctranslate2/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2846 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.2.5/src/whisper_ctranslate2/languages.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5154 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.2.5/src/whisper_ctranslate2/live.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6275 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.2.5/src/whisper_ctranslate2/transcribe.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.2.5/src/whisper_ctranslate2/version.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    17511 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.2.5/src/whisper_ctranslate2/whisper_ctranslate2.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    10359 2023-05-27 10:54:49.000000 whisper-ctranslate2-0.2.5/src/whisper_ctranslate2/writers.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-27 11:31:40.077345 whisper-ctranslate2-0.2.5/whisper_ctranslate2.egg-info/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5623 2023-05-27 11:31:39.000000 whisper-ctranslate2-0.2.5/whisper_ctranslate2.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      520 2023-05-27 11:31:40.000000 whisper-ctranslate2-0.2.5/whisper_ctranslate2.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-05-27 11:31:39.000000 whisper-ctranslate2-0.2.5/whisper_ctranslate2.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       89 2023-05-27 11:31:39.000000 whisper-ctranslate2-0.2.5/whisper_ctranslate2.egg-info/entry_points.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      100 2023-05-27 11:31:39.000000 whisper-ctranslate2-0.2.5/whisper_ctranslate2.egg-info/requires.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       24 2023-05-27 11:31:39.000000 whisper-ctranslate2-0.2.5/whisper_ctranslate2.egg-info/top_level.txt
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-06 05:27:30.020632 whisper-ctranslate2-0.2.6/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.2.6/LICENSE
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5623 2023-06-06 05:27:30.020632 whisper-ctranslate2-0.2.6/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4990 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.2.6/README.md
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2023-06-06 05:27:30.020632 whisper-ctranslate2-0.2.6/setup.cfg
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1501 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.2.6/setup.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-06 05:27:30.020632 whisper-ctranslate2-0.2.6/src/
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-06 05:27:30.020632 whisper-ctranslate2-0.2.6/src/whisper_ctranslate2/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2846 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.2.6/src/whisper_ctranslate2/languages.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5232 2023-06-06 05:24:38.000000 whisper-ctranslate2-0.2.6/src/whisper_ctranslate2/live.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6324 2023-06-06 05:24:38.000000 whisper-ctranslate2-0.2.6/src/whisper_ctranslate2/transcribe.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2023-05-27 11:37:32.000000 whisper-ctranslate2-0.2.6/src/whisper_ctranslate2/version.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    17517 2023-06-06 05:24:38.000000 whisper-ctranslate2-0.2.6/src/whisper_ctranslate2/whisper_ctranslate2.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    10359 2023-05-27 10:54:49.000000 whisper-ctranslate2-0.2.6/src/whisper_ctranslate2/writers.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-06 05:27:30.020632 whisper-ctranslate2-0.2.6/whisper_ctranslate2.egg-info/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5623 2023-06-06 05:27:29.000000 whisper-ctranslate2-0.2.6/whisper_ctranslate2.egg-info/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      520 2023-06-06 05:27:29.000000 whisper-ctranslate2-0.2.6/whisper_ctranslate2.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-06-06 05:27:29.000000 whisper-ctranslate2-0.2.6/whisper_ctranslate2.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       89 2023-06-06 05:27:29.000000 whisper-ctranslate2-0.2.6/whisper_ctranslate2.egg-info/entry_points.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      100 2023-06-06 05:27:29.000000 whisper-ctranslate2-0.2.6/whisper_ctranslate2.egg-info/requires.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       24 2023-06-06 05:27:29.000000 whisper-ctranslate2-0.2.6/whisper_ctranslate2.egg-info/top_level.txt
```

### Comparing `whisper-ctranslate2-0.2.5/LICENSE` & `whisper-ctranslate2-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.5/PKG-INFO` & `whisper-ctranslate2-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-ctranslate2
-Version: 0.2.5
+Version: 0.2.6
 Summary: Whisper command line client that uses CTranslate2
 Home-page: https://github.com/Softcatala/whisper-ctranslate2
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `whisper-ctranslate2-0.2.5/README.md` & `whisper-ctranslate2-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.5/setup.py` & `whisper-ctranslate2-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.5/src/whisper_ctranslate2/languages.py` & `whisper-ctranslate2-0.2.6/src/whisper_ctranslate2/languages.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.5/src/whisper_ctranslate2/live.py` & `whisper-ctranslate2-0.2.6/src/whisper_ctranslate2/live.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 
         self.running = True
         self.waiting = 0
         self.prevblock = self.buffer = np.zeros((0, 1))
         self.speaking = False
         self.blocks_speaking = 0
         self.buffers_to_process = []
+        self.transcribe = None
 
     @staticmethod
     def is_available():
         return sounddevice_available
 
     @staticmethod
     def force_not_available_exception():
@@ -115,25 +116,29 @@
 
     def process(self):
         if len(self.buffers_to_process) > 0:
             _buffer = self.buffers_to_process.pop()
             if self.verbose:
                 print("\n\033[90mTranscribing..\033[0m")
 
-            result = Transcribe().inference(
+            if not self.transcribe:
+                self.transcribe = Transcribe(
+                    self.model_path,
+                    self.device,
+                    self.device_index,
+                    self.compute_type,
+                    self.threads,
+                    self.cache_directory,
+                    self.local_files_only,
+                )
+
+            result = self.transcribe.inference(
                 audio=_buffer.flatten(),
-                model_path=self.model_path,
-                cache_directory=self.cache_directory,
-                local_files_only=self.local_files_only,
                 task=self.task,
                 language=self.language,
-                threads=self.threads,
-                device=self.device,
-                device_index=self.device_index,
-                compute_type=self.compute_type,
                 verbose=self.verbose,
                 live=True,
                 options=self.options,
             )
             print(f"\033[1A\033[2K\033[0G{result['text']}")
             if not self.verbose:
                 print("")
```

### Comparing `whisper-ctranslate2-0.2.5/src/whisper_ctranslate2/transcribe.py` & `whisper-ctranslate2-0.2.6/src/whisper_ctranslate2/transcribe.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,43 +90,46 @@
         if options.vad_min_silence_duration_ms:
             vad_parameters[
                 "min_silence_duration_ms"
             ] = options.vad_min_silence_duration_ms
 
         return vad_parameters
 
-    def inference(
+    def __init__(
         self,
-        audio: Union[str, BinaryIO, np.ndarray],
         model_path: str,
-        cache_directory: str,
-        local_files_only: bool,
-        task: str,
-        language: str,
-        threads: int,
         device: str,
         device_index: Union[int, List[int]],
         compute_type: str,
-        verbose: bool,
-        live: bool,
-        options: TranscriptionOptions,
+        threads: int,
+        cache_directory: str,
+        local_files_only: bool,
     ):
-        model = WhisperModel(
+        self.model = WhisperModel(
             model_path,
             device=device,
             device_index=device_index,
             compute_type=compute_type,
             cpu_threads=threads,
             download_root=cache_directory,
             local_files_only=local_files_only,
         )
 
+    def inference(
+        self,
+        audio: Union[str, BinaryIO, np.ndarray],
+        task: str,
+        language: str,
+        verbose: bool,
+        live: bool,
+        options: TranscriptionOptions,
+    ):
         vad_parameters = self._get_vad_parameters_dictionary(options)
 
-        segments, info = model.transcribe(
+        segments, info = self.model.transcribe(
             audio=audio,
             language=language,
             task=task,
             beam_size=options.beam_size,
             best_of=options.best_of,
             patience=options.patience,
             length_penalty=options.length_penalty,
```

### Comparing `whisper-ctranslate2-0.2.5/src/whisper_ctranslate2/whisper_ctranslate2.py` & `whisper-ctranslate2-0.2.6/src/whisper_ctranslate2/whisper_ctranslate2.py`

 * *Files 0% similar despite different names*

```diff
@@ -509,26 +509,29 @@
             live_volume_threshold,
             live_input_device,
             options,
         ).inference()
 
         return
 
+    transcribe = Transcribe(
+        model_dir,
+        device,
+        device_index,
+        compute_type,
+        threads,
+        cache_directory,
+        local_files_only,
+    )
+
     for audio_path in audio:
-        result = Transcribe().inference(
+        result = transcribe.inference(
             audio_path,
-            model_dir,
-            cache_directory,
-            local_files_only,
             task,
             language,
-            threads,
-            device,
-            device_index,
-            compute_type,
             verbose,
             False,
             options,
         )
         writer = get_writer(output_format, output_dir)
         writer(result, audio_path, writer_args)
```

### Comparing `whisper-ctranslate2-0.2.5/src/whisper_ctranslate2/writers.py` & `whisper-ctranslate2-0.2.6/src/whisper_ctranslate2/writers.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.5/whisper_ctranslate2.egg-info/PKG-INFO` & `whisper-ctranslate2-0.2.6/whisper_ctranslate2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-ctranslate2
-Version: 0.2.5
+Version: 0.2.6
 Summary: Whisper command line client that uses CTranslate2
 Home-page: https://github.com/Softcatala/whisper-ctranslate2
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `whisper-ctranslate2-0.2.5/whisper_ctranslate2.egg-info/SOURCES.txt` & `whisper-ctranslate2-0.2.6/whisper_ctranslate2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

