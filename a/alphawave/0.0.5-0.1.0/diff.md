# Comparing `tmp/alphawave-0.0.5.tar.gz` & `tmp/alphawave-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphawave-0.0.5.tar", last modified: Mon Jun  5 22:07:17 2023, max compression
+gzip compressed data, was "alphawave-0.1.0.tar", last modified: Mon Jun  5 23:40:50 2023, max compression
```

## Comparing `alphawave-0.0.5.tar` & `alphawave-0.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-05 22:07:17.334973 alphawave-0.0.5/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.0.5/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      670 2023-06-05 22:07:17.334973 alphawave-0.0.5/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       57 2023-06-05 21:20:34.000000 alphawave-0.0.5/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      837 2023-06-05 21:17:25.000000 alphawave-0.0.5/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-05 22:07:17.334973 alphawave-0.0.5/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-05 22:07:17.330973 alphawave-0.0.5/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-05 22:07:17.330973 alphawave-0.0.5/src/alphawave/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    10089 2023-06-05 02:02:06.000000 alphawave-0.0.5/src/alphawave/AlphaWave.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1207 2023-06-04 00:33:26.000000 alphawave-0.0.5/src/alphawave/Colorize.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      701 2023-06-04 23:38:31.000000 alphawave-0.0.5/src/alphawave/DefaultResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1890 2023-06-03 23:06:34.000000 alphawave-0.0.5/src/alphawave/JSONResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1963 2023-06-03 23:22:26.000000 alphawave-0.0.5/src/alphawave/MemoryForkTest.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6799 2023-06-04 16:26:58.000000 alphawave-0.0.5/src/alphawave/OSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7514 2023-06-05 18:36:51.000000 alphawave-0.0.5/src/alphawave/OpenAIClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2301 2023-06-03 23:24:45.000000 alphawave-0.0.5/src/alphawave/Response.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14731 2023-06-04 03:49:37.000000 alphawave-0.0.5/src/alphawave/TestAlphaWave.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      850 2023-06-04 03:32:15.000000 alphawave-0.0.5/src/alphawave/TestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1485 2023-06-03 23:57:30.000000 alphawave-0.0.5/src/alphawave/TestClientTest.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1914 2023-06-05 18:40:59.000000 alphawave-0.0.5/src/alphawave/alphaChat.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1311 2023-06-04 00:58:56.000000 alphawave-0.0.5/src/alphawave/alphawaveTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.0.5/src/alphawave/internalTypes.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-05 22:07:17.330973 alphawave-0.0.5/src/alphawave.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      670 2023-06-05 22:07:17.000000 alphawave-0.0.5/src/alphawave.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      671 2023-06-05 22:07:17.000000 alphawave-0.0.5/src/alphawave.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-05 22:07:17.000000 alphawave-0.0.5/src/alphawave.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       81 2023-06-05 22:07:17.000000 alphawave-0.0.5/src/alphawave.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       10 2023-06-05 22:07:17.000000 alphawave-0.0.5/src/alphawave.egg-info/top_level.txt
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-05 22:07:17.330973 alphawave-0.0.5/tests/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14712 2023-06-05 18:15:14.000000 alphawave-0.0.5/tests/testOpenAiClient.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-05 23:40:50.613758 alphawave-0.1.0/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.1.0/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      670 2023-06-05 23:40:50.613758 alphawave-0.1.0/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       57 2023-06-05 21:20:34.000000 alphawave-0.1.0/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      837 2023-06-05 23:40:25.000000 alphawave-0.1.0/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-05 23:40:50.613758 alphawave-0.1.0/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-05 23:40:50.613758 alphawave-0.1.0/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-05 23:40:50.613758 alphawave-0.1.0/src/alphawave/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    10089 2023-06-05 02:02:06.000000 alphawave-0.1.0/src/alphawave/AlphaWave.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1207 2023-06-04 00:33:26.000000 alphawave-0.1.0/src/alphawave/Colorize.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      701 2023-06-04 23:38:31.000000 alphawave-0.1.0/src/alphawave/DefaultResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1890 2023-06-03 23:06:34.000000 alphawave-0.1.0/src/alphawave/JSONResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1963 2023-06-03 23:22:26.000000 alphawave-0.1.0/src/alphawave/MemoryForkTest.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6799 2023-06-04 16:26:58.000000 alphawave-0.1.0/src/alphawave/OSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7514 2023-06-05 18:36:51.000000 alphawave-0.1.0/src/alphawave/OpenAIClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2301 2023-06-03 23:24:45.000000 alphawave-0.1.0/src/alphawave/Response.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14731 2023-06-04 03:49:37.000000 alphawave-0.1.0/src/alphawave/TestAlphaWave.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      850 2023-06-04 03:32:15.000000 alphawave-0.1.0/src/alphawave/TestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1485 2023-06-03 23:57:30.000000 alphawave-0.1.0/src/alphawave/TestClientTest.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1914 2023-06-05 18:40:59.000000 alphawave-0.1.0/src/alphawave/alphaChat.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1311 2023-06-04 00:58:56.000000 alphawave-0.1.0/src/alphawave/alphawaveTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.1.0/src/alphawave/internalTypes.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-05 23:40:50.613758 alphawave-0.1.0/src/alphawave.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      670 2023-06-05 23:40:50.000000 alphawave-0.1.0/src/alphawave.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      671 2023-06-05 23:40:50.000000 alphawave-0.1.0/src/alphawave.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-05 23:40:50.000000 alphawave-0.1.0/src/alphawave.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       81 2023-06-05 23:40:50.000000 alphawave-0.1.0/src/alphawave.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       10 2023-06-05 23:40:50.000000 alphawave-0.1.0/src/alphawave.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-05 23:40:50.613758 alphawave-0.1.0/tests/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14712 2023-06-05 18:15:14.000000 alphawave-0.1.0/tests/testOpenAiClient.py
```

### Comparing `alphawave-0.0.5/LICENSE` & `alphawave-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alphawave-0.0.5/PKG-INFO` & `alphawave-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.0.5
+Version: 0.1.0
 Summary: AlphaWave - a very opinionated client for interfacing with Large Language Models (LLM)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
-Project-URL: Homepage, https://github.com/Stevenic/promptrix-py
-Project-URL: Bug Tracker, https://github.com/Stevenic/promptrix-py/issues
+Project-URL: Homepage, https://github.com/Stevenic/alphawave-py
+Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `alphawave-0.0.5/pyproject.toml` & `alphawave-0.1.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alphawave"
-version = "0.0.5"
+version = "0.1.0"
 authors = [
   { name="Steven Ickman", email="author@example.com" },
   { name="Bruce DAmbrosio", email="bruce.dambrosio@gmail.com" },
 ]
 
 description = "AlphaWave - a very opinionated client for interfacing with Large Language Models (LLM)"
 
@@ -28,9 +28,9 @@
     "tiktoken",
     "pyyaml",
     'importlib-metadata; python_version<"3.9"',
 ]
 
 
 [project.urls]
-"Homepage" = "https://github.com/Stevenic/promptrix-py"
-"Bug Tracker" = "https://github.com/Stevenic/promptrix-py/issues"
+"Homepage" = "https://github.com/Stevenic/alphawave-py"
+"Bug Tracker" = "https://github.com/Stevenic/alphawave-py/issues"
```

### Comparing `alphawave-0.0.5/src/alphawave/AlphaWave.py` & `alphawave-0.1.0/src/alphawave/AlphaWave.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.0.5/src/alphawave/Colorize.py` & `alphawave-0.1.0/src/alphawave/Colorize.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.0.5/src/alphawave/DefaultResponseValidator.py` & `alphawave-0.1.0/src/alphawave/DefaultResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.0.5/src/alphawave/JSONResponseValidator.py` & `alphawave-0.1.0/src/alphawave/JSONResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.0.5/src/alphawave/MemoryForkTest.py` & `alphawave-0.1.0/src/alphawave/MemoryForkTest.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.0.5/src/alphawave/OSClient.py` & `alphawave-0.1.0/src/alphawave/OSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.0.5/src/alphawave/OpenAIClient.py` & `alphawave-0.1.0/src/alphawave/OpenAIClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.0.5/src/alphawave/Response.py` & `alphawave-0.1.0/src/alphawave/Response.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.0.5/src/alphawave/TestAlphaWave.py` & `alphawave-0.1.0/src/alphawave/TestAlphaWave.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.0.5/src/alphawave/TestClient.py` & `alphawave-0.1.0/src/alphawave/TestClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.0.5/src/alphawave/TestClientTest.py` & `alphawave-0.1.0/src/alphawave/TestClientTest.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.0.5/src/alphawave/alphaChat.py` & `alphawave-0.1.0/src/alphawave/alphaChat.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.0.5/src/alphawave/alphawaveTypes.py` & `alphawave-0.1.0/src/alphawave/alphawaveTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.0.5/src/alphawave/internalTypes.py` & `alphawave-0.1.0/src/alphawave/internalTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.0.5/src/alphawave.egg-info/PKG-INFO` & `alphawave-0.1.0/src/alphawave.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.0.5
+Version: 0.1.0
 Summary: AlphaWave - a very opinionated client for interfacing with Large Language Models (LLM)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
-Project-URL: Homepage, https://github.com/Stevenic/promptrix-py
-Project-URL: Bug Tracker, https://github.com/Stevenic/promptrix-py/issues
+Project-URL: Homepage, https://github.com/Stevenic/alphawave-py
+Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `alphawave-0.0.5/src/alphawave.egg-info/SOURCES.txt` & `alphawave-0.1.0/src/alphawave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphawave-0.0.5/tests/testOpenAiClient.py` & `alphawave-0.1.0/tests/testOpenAiClient.py`

 * *Files identical despite different names*

