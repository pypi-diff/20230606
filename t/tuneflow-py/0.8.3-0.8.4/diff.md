# Comparing `tmp/tuneflow-py-0.8.3.tar.gz` & `tmp/tuneflow-py-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuneflow-py-0.8.3.tar", last modified: Fri Jun  2 01:00:55 2023, max compression
+gzip compressed data, was "tuneflow-py-0.8.4.tar", last modified: Tue Jun  6 20:46:19 2023, max compression
```

## Comparing `tuneflow-py-0.8.3.tar` & `tuneflow-py-0.8.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-02 01:00:55.703975 tuneflow-py-0.8.3/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1065 2023-01-10 14:03:44.000000 tuneflow-py-0.8.3/LICENSE
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-06-02 01:00:55.703975 tuneflow-py-0.8.3/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)     3809 2023-03-06 23:39:23.000000 tuneflow-py-0.8.3/README.md
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1288 2023-06-02 00:56:25.000000 tuneflow-py-0.8.3/pyproject.toml
--rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-06-02 01:00:55.703975 tuneflow-py-0.8.3/setup.cfg
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-02 01:00:55.693975 tuneflow-py-0.8.3/src/
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-02 01:00:55.703975 tuneflow-py-0.8.3/src/tuneflow_py/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1221 2023-04-29 04:10:56.000000 tuneflow-py-0.8.3/src/tuneflow_py/__init__.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1987 2023-02-28 00:04:43.000000 tuneflow-py-0.8.3/src/tuneflow_py/base_plugin.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-02 01:00:55.703975 tuneflow-py-0.8.3/src/tuneflow_py/descriptors/
--rw-r--r--   0 panacea   (1000) panacea   (1000)      922 2023-03-30 21:40:36.000000 tuneflow-py-0.8.3/src/tuneflow_py/descriptors/audio_plugin_descriptor.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1857 2023-04-16 06:53:45.000000 tuneflow-py-0.8.3/src/tuneflow_py/descriptors/clip_descriptor.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)      839 2023-05-08 17:27:14.000000 tuneflow-py-0.8.3/src/tuneflow_py/descriptors/common.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4283 2023-05-07 06:46:25.000000 tuneflow-py-0.8.3/src/tuneflow_py/descriptors/param.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     5088 2023-05-08 17:24:18.000000 tuneflow-py-0.8.3/src/tuneflow_py/descriptors/plugin.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)       71 2023-06-02 00:53:05.000000 tuneflow-py-0.8.3/src/tuneflow_py/descriptors/text.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     5805 2023-06-02 00:54:12.000000 tuneflow-py-0.8.3/src/tuneflow_py/descriptors/widget.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-02 01:00:55.703975 tuneflow-py-0.8.3/src/tuneflow_py/models/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     3128 2023-03-01 03:02:02.000000 tuneflow-py-0.8.3/src/tuneflow_py/models/audio_plugin.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    17158 2023-03-31 07:33:41.000000 tuneflow-py-0.8.3/src/tuneflow_py/models/automation.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    34271 2023-05-10 04:28:18.000000 tuneflow-py-0.8.3/src/tuneflow_py/models/clip.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    17149 2023-04-29 04:10:56.000000 tuneflow-py-0.8.3/src/tuneflow_py/models/lyric.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1305 2023-04-10 18:15:27.000000 tuneflow-py-0.8.3/src/tuneflow_py/models/marker.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     5275 2023-02-22 00:50:28.000000 tuneflow-py-0.8.3/src/tuneflow_py/models/note.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-02 01:00:55.703975 tuneflow-py-0.8.3/src/tuneflow_py/models/protos/
--rw-r--r--   0 panacea   (1000) panacea   (1000)    76828 2023-04-29 04:10:56.000000 tuneflow-py-0.8.3/src/tuneflow_py/models/protos/song_pb2.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    25653 2023-04-29 04:10:56.000000 tuneflow-py-0.8.3/src/tuneflow_py/models/song.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)      873 2023-03-01 22:09:14.000000 tuneflow-py-0.8.3/src/tuneflow_py/models/tempo.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1093 2023-02-22 00:28:50.000000 tuneflow-py-0.8.3/src/tuneflow_py/models/time_signature.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    16703 2023-04-29 04:10:56.000000 tuneflow-py-0.8.3/src/tuneflow_py/models/track.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     6210 2023-03-29 01:48:05.000000 tuneflow-py-0.8.3/src/tuneflow_py/utils.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-02 01:00:55.703975 tuneflow-py-0.8.3/src/tuneflow_py.egg-info/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-06-02 01:00:55.000000 tuneflow-py-0.8.3/src/tuneflow_py.egg-info/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1164 2023-06-02 01:00:55.000000 tuneflow-py-0.8.3/src/tuneflow_py.egg-info/SOURCES.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-06-02 01:00:55.000000 tuneflow-py-0.8.3/src/tuneflow_py.egg-info/dependency_links.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)       96 2023-06-02 01:00:55.000000 tuneflow-py-0.8.3/src/tuneflow_py.egg-info/requires.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)       12 2023-06-02 01:00:55.000000 tuneflow-py-0.8.3/src/tuneflow_py.egg-info/top_level.txt
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-02 01:00:55.703975 tuneflow-py-0.8.3/test/
--rw-r--r--   0 panacea   (1000) panacea   (1000)    30358 2023-05-10 04:29:39.000000 tuneflow-py-0.8.3/test/test_audio_clip.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    24170 2023-03-31 07:02:16.000000 tuneflow-py-0.8.3/test/test_automation.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    16632 2023-04-29 04:10:56.000000 tuneflow-py-0.8.3/test/test_lyric.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     8001 2023-04-10 18:37:18.000000 tuneflow-py-0.8.3/test/test_marker.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    33568 2023-03-09 18:17:16.000000 tuneflow-py-0.8.3/test/test_midi_clip.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    24300 2023-02-22 00:33:25.000000 tuneflow-py-0.8.3/test/test_note.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    14091 2023-03-31 16:54:59.000000 tuneflow-py-0.8.3/test/test_song.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     5693 2023-04-29 04:10:56.000000 tuneflow-py-0.8.3/test/test_track.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     2071 2023-02-16 23:10:13.000000 tuneflow-py-0.8.3/test/test_utils.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-06 20:46:19.291051 tuneflow-py-0.8.4/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1065 2023-01-10 14:03:44.000000 tuneflow-py-0.8.4/LICENSE
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-06-06 20:46:19.291051 tuneflow-py-0.8.4/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     3809 2023-03-06 23:39:23.000000 tuneflow-py-0.8.4/README.md
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1288 2023-06-06 20:45:44.000000 tuneflow-py-0.8.4/pyproject.toml
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-06-06 20:46:19.291051 tuneflow-py-0.8.4/setup.cfg
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-06 20:46:19.281051 tuneflow-py-0.8.4/src/
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-06 20:46:19.281051 tuneflow-py-0.8.4/src/tuneflow_py/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1221 2023-04-29 04:10:56.000000 tuneflow-py-0.8.4/src/tuneflow_py/__init__.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1987 2023-02-28 00:04:43.000000 tuneflow-py-0.8.4/src/tuneflow_py/base_plugin.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-06 20:46:19.281051 tuneflow-py-0.8.4/src/tuneflow_py/descriptors/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      922 2023-03-30 21:40:36.000000 tuneflow-py-0.8.4/src/tuneflow_py/descriptors/audio_plugin_descriptor.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1857 2023-04-16 06:53:45.000000 tuneflow-py-0.8.4/src/tuneflow_py/descriptors/clip_descriptor.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      839 2023-05-08 17:27:14.000000 tuneflow-py-0.8.4/src/tuneflow_py/descriptors/common.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4305 2023-06-06 20:40:08.000000 tuneflow-py-0.8.4/src/tuneflow_py/descriptors/param.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     5088 2023-05-08 17:24:18.000000 tuneflow-py-0.8.4/src/tuneflow_py/descriptors/plugin.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       71 2023-06-02 00:53:05.000000 tuneflow-py-0.8.4/src/tuneflow_py/descriptors/text.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     5805 2023-06-02 00:54:12.000000 tuneflow-py-0.8.4/src/tuneflow_py/descriptors/widget.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-06 20:46:19.281051 tuneflow-py-0.8.4/src/tuneflow_py/models/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     3128 2023-03-01 03:02:02.000000 tuneflow-py-0.8.4/src/tuneflow_py/models/audio_plugin.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    17158 2023-03-31 07:33:41.000000 tuneflow-py-0.8.4/src/tuneflow_py/models/automation.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    34271 2023-05-10 04:28:18.000000 tuneflow-py-0.8.4/src/tuneflow_py/models/clip.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    17149 2023-04-29 04:10:56.000000 tuneflow-py-0.8.4/src/tuneflow_py/models/lyric.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1305 2023-04-10 18:15:27.000000 tuneflow-py-0.8.4/src/tuneflow_py/models/marker.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     5275 2023-02-22 00:50:28.000000 tuneflow-py-0.8.4/src/tuneflow_py/models/note.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-06 20:46:19.281051 tuneflow-py-0.8.4/src/tuneflow_py/models/protos/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    76828 2023-04-29 04:10:56.000000 tuneflow-py-0.8.4/src/tuneflow_py/models/protos/song_pb2.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    25653 2023-04-29 04:10:56.000000 tuneflow-py-0.8.4/src/tuneflow_py/models/song.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      873 2023-03-01 22:09:14.000000 tuneflow-py-0.8.4/src/tuneflow_py/models/tempo.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1093 2023-02-22 00:28:50.000000 tuneflow-py-0.8.4/src/tuneflow_py/models/time_signature.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    16703 2023-04-29 04:10:56.000000 tuneflow-py-0.8.4/src/tuneflow_py/models/track.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     6210 2023-03-29 01:48:05.000000 tuneflow-py-0.8.4/src/tuneflow_py/utils.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-06 20:46:19.281051 tuneflow-py-0.8.4/src/tuneflow_py.egg-info/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-06-06 20:46:19.000000 tuneflow-py-0.8.4/src/tuneflow_py.egg-info/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1164 2023-06-06 20:46:19.000000 tuneflow-py-0.8.4/src/tuneflow_py.egg-info/SOURCES.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-06-06 20:46:19.000000 tuneflow-py-0.8.4/src/tuneflow_py.egg-info/dependency_links.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       96 2023-06-06 20:46:19.000000 tuneflow-py-0.8.4/src/tuneflow_py.egg-info/requires.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       12 2023-06-06 20:46:19.000000 tuneflow-py-0.8.4/src/tuneflow_py.egg-info/top_level.txt
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-06 20:46:19.291051 tuneflow-py-0.8.4/test/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    30358 2023-05-10 04:29:39.000000 tuneflow-py-0.8.4/test/test_audio_clip.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    24170 2023-03-31 07:02:16.000000 tuneflow-py-0.8.4/test/test_automation.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    16632 2023-04-29 04:10:56.000000 tuneflow-py-0.8.4/test/test_lyric.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     8001 2023-04-10 18:37:18.000000 tuneflow-py-0.8.4/test/test_marker.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    33568 2023-03-09 18:17:16.000000 tuneflow-py-0.8.4/test/test_midi_clip.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    24300 2023-02-22 00:33:25.000000 tuneflow-py-0.8.4/test/test_note.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    14091 2023-03-31 16:54:59.000000 tuneflow-py-0.8.4/test/test_song.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     5693 2023-04-29 04:10:56.000000 tuneflow-py-0.8.4/test/test_track.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     2071 2023-02-16 23:10:13.000000 tuneflow-py-0.8.4/test/test_utils.py
```

### Comparing `tuneflow-py-0.8.3/LICENSE` & `tuneflow-py-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.3/PKG-INFO` & `tuneflow-py-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneflow-py
-Version: 0.8.3
+Version: 0.8.4
 Summary: Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era
 Author-email: TuneFlow <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/tuneflow/tuneflow-py
 Project-URL: Bug Tracker, https://github.com/tuneflow/tuneflow-py/issues
 Keywords: AI,music,DAW,TuneFlow,composition,songwriting,music production,music generation,music transcription,mixing,music theory,music information retrieval,MIR,music analysis,song analysis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuneflow-py-0.8.3/README.md` & `tuneflow-py-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.3/pyproject.toml` & `tuneflow-py-0.8.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "tuneflow-py"
-version = "0.8.3"
+version = "0.8.4"
 authors = [{ name = "TuneFlow", email = "contact@info.tuneflow.com" }]
 description = "Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = [
   "AI",
   "music",
```

### Comparing `tuneflow-py-0.8.3/src/tuneflow_py/__init__.py` & `tuneflow-py-0.8.4/src/tuneflow_py/__init__.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.3/src/tuneflow_py/base_plugin.py` & `tuneflow-py-0.8.4/src/tuneflow_py/base_plugin.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.3/src/tuneflow_py/descriptors/audio_plugin_descriptor.py` & `tuneflow-py-0.8.4/src/tuneflow_py/descriptors/audio_plugin_descriptor.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.3/src/tuneflow_py/descriptors/clip_descriptor.py` & `tuneflow-py-0.8.4/src/tuneflow_py/descriptors/clip_descriptor.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.3/src/tuneflow_py/descriptors/common.py` & `tuneflow-py-0.8.4/src/tuneflow_py/descriptors/common.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.3/src/tuneflow_py/descriptors/param.py` & `tuneflow-py-0.8.4/src/tuneflow_py/descriptors/param.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     '''
 
 
 class ClipAudioDataInjectOptions(AudioDataInjectOptions):
     '''
     Inject config for when injection source is `InjectSource.ClipAudioData`.
     '''
-    clips: Required[Literal['selectedAudioClips',] | List[ClipInfo]]
+    clips: Required[Literal['selectedAudioClips', 'triggeredAudioClips'] | List[ClipInfo]]
 
 
 class SelectedClipInfosInjectOptions(TypedDict):
     '''
     Inject config for when injection source is `InjectSource.SelectedClipInfos`.
     '''
```

### Comparing `tuneflow-py-0.8.3/src/tuneflow_py/descriptors/plugin.py` & `tuneflow-py-0.8.4/src/tuneflow_py/descriptors/plugin.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.3/src/tuneflow_py/descriptors/widget.py` & `tuneflow-py-0.8.4/src/tuneflow_py/descriptors/widget.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.3/src/tuneflow_py/models/audio_plugin.py` & `tuneflow-py-0.8.4/src/tuneflow_py/models/audio_plugin.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.3/src/tuneflow_py/models/automation.py` & `tuneflow-py-0.8.4/src/tuneflow_py/models/automation.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.3/src/tuneflow_py/models/clip.py` & `tuneflow-py-0.8.4/src/tuneflow_py/models/clip.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.3/src/tuneflow_py/models/lyric.py` & `tuneflow-py-0.8.4/src/tuneflow_py/models/lyric.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.3/src/tuneflow_py/models/marker.py` & `tuneflow-py-0.8.4/src/tuneflow_py/models/marker.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.3/src/tuneflow_py/models/note.py` & `tuneflow-py-0.8.4/src/tuneflow_py/models/note.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.3/src/tuneflow_py/models/protos/song_pb2.py` & `tuneflow-py-0.8.4/src/tuneflow_py/models/protos/song_pb2.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.3/src/tuneflow_py/models/song.py` & `tuneflow-py-0.8.4/src/tuneflow_py/models/song.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.3/src/tuneflow_py/models/tempo.py` & `tuneflow-py-0.8.4/src/tuneflow_py/models/tempo.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.3/src/tuneflow_py/models/time_signature.py` & `tuneflow-py-0.8.4/src/tuneflow_py/models/time_signature.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.3/src/tuneflow_py/models/track.py` & `tuneflow-py-0.8.4/src/tuneflow_py/models/track.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.3/src/tuneflow_py/utils.py` & `tuneflow-py-0.8.4/src/tuneflow_py/utils.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.3/src/tuneflow_py.egg-info/PKG-INFO` & `tuneflow-py-0.8.4/src/tuneflow_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneflow-py
-Version: 0.8.3
+Version: 0.8.4
 Summary: Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era
 Author-email: TuneFlow <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/tuneflow/tuneflow-py
 Project-URL: Bug Tracker, https://github.com/tuneflow/tuneflow-py/issues
 Keywords: AI,music,DAW,TuneFlow,composition,songwriting,music production,music generation,music transcription,mixing,music theory,music information retrieval,MIR,music analysis,song analysis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuneflow-py-0.8.3/src/tuneflow_py.egg-info/SOURCES.txt` & `tuneflow-py-0.8.4/src/tuneflow_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.3/test/test_audio_clip.py` & `tuneflow-py-0.8.4/test/test_audio_clip.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.3/test/test_automation.py` & `tuneflow-py-0.8.4/test/test_automation.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.3/test/test_lyric.py` & `tuneflow-py-0.8.4/test/test_lyric.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.3/test/test_marker.py` & `tuneflow-py-0.8.4/test/test_marker.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.3/test/test_midi_clip.py` & `tuneflow-py-0.8.4/test/test_midi_clip.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.3/test/test_note.py` & `tuneflow-py-0.8.4/test/test_note.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.3/test/test_song.py` & `tuneflow-py-0.8.4/test/test_song.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.3/test/test_track.py` & `tuneflow-py-0.8.4/test/test_track.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.3/test/test_utils.py` & `tuneflow-py-0.8.4/test/test_utils.py`

 * *Files identical despite different names*

