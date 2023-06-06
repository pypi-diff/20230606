# Comparing `tmp/logfire-python-0.0.2.tar.gz` & `tmp/logfire-python-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logfire-python-0.0.2.tar", last modified: Fri Apr 21 05:17:54 2023, max compression
+gzip compressed data, was "logfire-python-0.0.3.tar", last modified: Tue Jun  6 06:55:00 2023, max compression
```

## Comparing `logfire-python-0.0.2.tar` & `logfire-python-0.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 05:17:54.588896 logfire-python-0.0.2/
--rw-rw-rw-   0        0        0      741 2023-04-12 02:48:20.000000 logfire-python-0.0.2/LICENSE.md
--rw-rw-rw-   0        0        0      106 2023-04-12 06:15:33.000000 logfire-python-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3757 2023-04-21 05:17:54.588896 logfire-python-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2672 2023-04-12 03:58:47.000000 logfire-python-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 05:17:54.571896 logfire-python-0.0.2/logfire/
--rw-rw-rw-   0        0        0      260 2023-04-12 03:28:58.000000 logfire-python-0.0.2/logfire/__init__.py
--rw-rw-rw-   0        0        0      141 2023-04-12 03:31:13.000000 logfire-python-0.0.2/logfire/compat.py
--rw-rw-rw-   0        0        0     2998 2023-04-12 03:31:03.000000 logfire-python-0.0.2/logfire/flusher.py
--rw-rw-rw-   0        0        0      968 2023-04-12 03:30:53.000000 logfire-python-0.0.2/logfire/formatter.py
--rw-rw-rw-   0        0        0     2441 2023-04-12 03:30:43.000000 logfire-python-0.0.2/logfire/frame.py
--rw-rw-rw-   0        0        0     2692 2023-04-21 05:16:34.000000 logfire-python-0.0.2/logfire/handler.py
--rw-rw-rw-   0        0        0     1156 2023-04-12 03:30:18.000000 logfire-python-0.0.2/logfire/helpers.py
--rw-rw-rw-   0        0        0      588 2023-04-12 03:30:07.000000 logfire-python-0.0.2/logfire/uploader.py
-drwxrwxrwx   0        0        0        0 2023-04-21 05:17:54.580897 logfire-python-0.0.2/logfire_python.egg-info/
--rw-rw-rw-   0        0        0     3757 2023-04-21 05:17:54.000000 logfire-python-0.0.2/logfire_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-04-21 05:17:54.000000 logfire-python-0.0.2/logfire_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 05:17:54.000000 logfire-python-0.0.2/logfire_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-04-21 05:17:54.000000 logfire-python-0.0.2/logfire_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-21 05:17:54.000000 logfire-python-0.0.2/logfire_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1263 2023-04-21 05:17:16.000000 logfire-python-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      222 2023-04-12 07:58:34.000000 logfire-python-0.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 05:17:54.589896 logfire-python-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0       54 2023-04-12 05:19:07.000000 logfire-python-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 05:17:54.588896 logfire-python-0.0.2/tests/
--rw-rw-rw-   0        0        0        0 2023-04-11 14:45:50.000000 logfire-python-0.0.2/tests/__init__.py
--rw-rw-rw-   0        0        0     5218 2023-04-21 05:17:37.000000 logfire-python-0.0.2/tests/test_flusher.py
--rw-rw-rw-   0        0        0     5264 2023-04-11 15:02:08.000000 logfire-python-0.0.2/tests/test_formatter.py
--rw-rw-rw-   0        0        0     1955 2023-04-11 15:02:30.000000 logfire-python-0.0.2/tests/test_frame.py
--rw-rw-rw-   0        0        0     4337 2023-04-11 15:02:51.000000 logfire-python-0.0.2/tests/test_handler.py
--rw-rw-rw-   0        0        0     1846 2023-04-11 15:03:14.000000 logfire-python-0.0.2/tests/test_helpers.py
--rw-rw-rw-   0        0        0     1059 2023-04-11 15:03:40.000000 logfire-python-0.0.2/tests/test_uploader.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:55:00.001047 logfire-python-0.0.3/
+-rw-rw-rw-   0        0        0      741 2023-04-12 02:48:20.000000 logfire-python-0.0.3/LICENSE.md
+-rw-rw-rw-   0        0        0      106 2023-04-12 06:15:33.000000 logfire-python-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3861 2023-06-06 06:55:00.000046 logfire-python-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2672 2023-04-12 03:58:47.000000 logfire-python-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 06:54:59.981473 logfire-python-0.0.3/logfire/
+-rw-rw-rw-   0        0        0      260 2023-04-12 03:28:58.000000 logfire-python-0.0.3/logfire/__init__.py
+-rw-rw-rw-   0        0        0      141 2023-04-12 03:31:13.000000 logfire-python-0.0.3/logfire/compat.py
+-rw-rw-rw-   0        0        0     2998 2023-04-12 03:31:03.000000 logfire-python-0.0.3/logfire/flusher.py
+-rw-rw-rw-   0        0        0      968 2023-04-12 03:30:53.000000 logfire-python-0.0.3/logfire/formatter.py
+-rw-rw-rw-   0        0        0     2441 2023-04-12 03:30:43.000000 logfire-python-0.0.3/logfire/frame.py
+-rw-rw-rw-   0        0        0     2680 2023-06-06 06:50:37.000000 logfire-python-0.0.3/logfire/handler.py
+-rw-rw-rw-   0        0        0     1156 2023-04-12 03:30:18.000000 logfire-python-0.0.3/logfire/helpers.py
+-rw-rw-rw-   0        0        0      588 2023-04-12 03:30:07.000000 logfire-python-0.0.3/logfire/uploader.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:54:59.991983 logfire-python-0.0.3/logfire_python.egg-info/
+-rw-rw-rw-   0        0        0     3861 2023-06-06 06:54:59.000000 logfire-python-0.0.3/logfire_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-06-06 06:54:59.000000 logfire-python-0.0.3/logfire_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 06:54:59.000000 logfire-python-0.0.3/logfire_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-06-06 06:54:59.000000 logfire-python-0.0.3/logfire_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-06 06:54:59.000000 logfire-python-0.0.3/logfire_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1357 2023-06-06 06:53:53.000000 logfire-python-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      222 2023-04-12 07:58:34.000000 logfire-python-0.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 06:55:00.001047 logfire-python-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0       54 2023-04-12 05:19:07.000000 logfire-python-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:54:59.999046 logfire-python-0.0.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-11 14:45:50.000000 logfire-python-0.0.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     5206 2023-06-06 06:50:49.000000 logfire-python-0.0.3/tests/test_flusher.py
+-rw-rw-rw-   0        0        0     5264 2023-04-11 15:02:08.000000 logfire-python-0.0.3/tests/test_formatter.py
+-rw-rw-rw-   0        0        0     1955 2023-04-11 15:02:30.000000 logfire-python-0.0.3/tests/test_frame.py
+-rw-rw-rw-   0        0        0     4337 2023-04-11 15:02:51.000000 logfire-python-0.0.3/tests/test_handler.py
+-rw-rw-rw-   0        0        0     1846 2023-04-11 15:03:14.000000 logfire-python-0.0.3/tests/test_helpers.py
+-rw-rw-rw-   0        0        0     1059 2023-04-11 15:03:40.000000 logfire-python-0.0.3/tests/test_uploader.py
```

### Comparing `logfire-python-0.0.2/LICENSE.md` & `logfire-python-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.2/PKG-INFO` & `logfire-python-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logfire-python
-Version: 0.0.2
+Version: 0.0.3
 Summary: Logfire.sh client library
 Author-email: Logfire <support@logfire.sh>
 Project-URL: Homepage, https://github.com/logfire-sh/logfire-python
 Keywords: api,logfire,logging,client
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,16 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.md
 
 # Logfire - Python Logging Made Easy
```

### Comparing `logfire-python-0.0.2/README.md` & `logfire-python-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.2/logfire/flusher.py` & `logfire-python-0.0.3/logfire/flusher.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.2/logfire/formatter.py` & `logfire-python-0.0.3/logfire/formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.2/logfire/frame.py` & `logfire-python-0.0.3/logfire/frame.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.2/logfire/handler.py` & `logfire-python-0.0.3/logfire/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from .compat import queue
 from .helpers import DEFAULT_CONTEXT
 from .flusher import FlushWorker
 from .uploader import Uploader
 from .frame import create_frame
 
-DEFAULT_HOST = 'https://api.logfire.sh/logfire.sh'
+DEFAULT_HOST = 'https://in.logfire.sh'
 DEFAULT_BUFFER_CAPACITY = 1000
 DEFAULT_FLUSH_INTERVAL = 1
 DEFAULT_RAISE_EXCEPTIONS = False
 DEFAULT_DROP_EXTRA_EVENTS = True
 DEFAULT_INCLUDE_EXTRA_ATTRIBUTES = True
```

### Comparing `logfire-python-0.0.2/logfire/helpers.py` & `logfire-python-0.0.3/logfire/helpers.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.2/logfire/uploader.py` & `logfire-python-0.0.3/logfire/uploader.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.2/logfire_python.egg-info/PKG-INFO` & `logfire-python-0.0.3/logfire_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logfire-python
-Version: 0.0.2
+Version: 0.0.3
 Summary: Logfire.sh client library
 Author-email: Logfire <support@logfire.sh>
 Project-URL: Homepage, https://github.com/logfire-sh/logfire-python
 Keywords: api,logfire,logging,client
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,16 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.md
 
 # Logfire - Python Logging Made Easy
```

### Comparing `logfire-python-0.0.2/logfire_python.egg-info/SOURCES.txt` & `logfire-python-0.0.3/logfire_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.2/pyproject.toml` & `logfire-python-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "logfire-python"
-version = "0.0.2"
+version = "0.0.3"
 description = "Logfire.sh client library"
 readme = "README.md"
 authors = [{ name = "Logfire", email = "support@logfire.sh" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: ISC License (ISCL)",
@@ -18,14 +18,16 @@
     "Programming Language :: Python :: 2.7",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.5",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 keywords = ["api", "logfire", "logging", "client"]
 dependencies = [
     "requests",
     "msgpack",
 ]
```

### Comparing `logfire-python-0.0.2/tests/test_flusher.py` & `logfire-python-0.0.3/tests/test_flusher.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from logfire.compat import queue
 from logfire.flusher import RETRY_SCHEDULE
 from logfire.flusher import FlushWorker
 from logfire.uploader import Uploader
 
 
 class TestFlushWorker(unittest2.TestCase):
-    host = 'https://api.logfire.sh/logfire.sh'
+    host = 'https://in.logfire.sh'
     source_token = 'dummy_source_token'
     buffer_capacity = 5
     flush_interval = 2
 
     def _setup_worker(self, uploader=None):
         pipe = queue.Queue(maxsize=self.buffer_capacity)
         uploader = uploader or Uploader(self.source_token, self.host)
```

### Comparing `logfire-python-0.0.2/tests/test_formatter.py` & `logfire-python-0.0.3/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.2/tests/test_frame.py` & `logfire-python-0.0.3/tests/test_frame.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.2/tests/test_handler.py` & `logfire-python-0.0.3/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.2/tests/test_helpers.py` & `logfire-python-0.0.3/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.2/tests/test_uploader.py` & `logfire-python-0.0.3/tests/test_uploader.py`

 * *Files identical despite different names*

