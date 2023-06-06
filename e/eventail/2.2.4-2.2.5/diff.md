# Comparing `tmp/eventail-2.2.4.tar.gz` & `tmp/eventail-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventail-2.2.4.tar", last modified: Tue Apr 25 14:19:04 2023, max compression
+gzip compressed data, was "eventail-2.2.5.tar", last modified: Tue Jun  6 08:20:01 2023, max compression
```

## Comparing `eventail-2.2.4.tar` & `eventail-2.2.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-25 14:19:04.365403 eventail-2.2.4/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1079 2023-04-25 14:19:03.000000 eventail-2.2.4/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-04-25 14:19:03.000000 eventail-2.2.4/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8234 2023-04-25 14:19:04.365403 eventail-2.2.4/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6154 2023-04-25 14:19:03.000000 eventail-2.2.4/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-25 14:19:04.361403 eventail-2.2.4/scripts/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4202 2023-04-25 14:19:03.000000 eventail-2.2.4/scripts/inspect_queue.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3742 2023-04-25 14:19:03.000000 eventail-2.2.4/scripts/logger.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5358 2023-04-25 14:19:03.000000 eventail-2.2.4/scripts/monitor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2108 2023-04-25 14:19:03.000000 eventail-2.2.4/scripts/publish_configuration.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3098 2023-04-25 14:19:03.000000 eventail-2.2.4/scripts/publish_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5297 2023-04-25 14:19:03.000000 eventail-2.2.4/scripts/resurrect.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3447 2023-04-25 14:19:03.000000 eventail-2.2.4/scripts/send_command.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-04-25 14:19:04.365403 eventail-2.2.4/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1351 2023-04-25 14:19:03.000000 eventail-2.2.4/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-25 14:19:04.361403 eventail-2.2.4/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-25 14:19:04.365403 eventail-2.2.4/src/eventail/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1121 2023-04-25 14:19:03.000000 eventail-2.2.4/src/eventail/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-25 14:19:04.365403 eventail-2.2.4/src/eventail/async_service/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1121 2023-04-25 14:19:03.000000 eventail-2.2.4/src/eventail/async_service/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-25 14:19:04.365403 eventail-2.2.4/src/eventail/async_service/aio/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1181 2023-04-25 14:19:03.000000 eventail-2.2.4/src/eventail/async_service/aio/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23412 2023-04-25 14:19:03.000000 eventail-2.2.4/src/eventail/async_service/aio/base.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-25 14:19:04.365403 eventail-2.2.4/src/eventail/async_service/pika/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1242 2023-04-25 14:19:03.000000 eventail-2.2.4/src/eventail/async_service/pika/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    44831 2023-04-25 14:19:03.000000 eventail-2.2.4/src/eventail/async_service/pika/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2811 2023-04-25 14:19:03.000000 eventail-2.2.4/src/eventail/async_service/pika/supervisor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3576 2023-04-25 14:19:03.000000 eventail-2.2.4/src/eventail/batch_processor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1534 2023-04-25 14:19:03.000000 eventail-2.2.4/src/eventail/gelf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1380 2023-04-25 14:19:03.000000 eventail-2.2.4/src/eventail/log_criticity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-25 14:19:03.000000 eventail-2.2.4/src/eventail/py.typed
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7806 2023-04-25 14:19:03.000000 eventail-2.2.4/src/eventail/sync_publisher.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7622 2023-04-25 14:19:03.000000 eventail-2.2.4/src/eventail/tmp_store.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-25 14:19:04.365403 eventail-2.2.4/src/eventail.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8234 2023-04-25 14:19:04.000000 eventail-2.2.4/src/eventail.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      820 2023-04-25 14:19:04.000000 eventail-2.2.4/src/eventail.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-25 14:19:04.000000 eventail-2.2.4/src/eventail.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2023-04-25 14:19:04.000000 eventail-2.2.4/src/eventail.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        9 2023-04-25 14:19:04.000000 eventail-2.2.4/src/eventail.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-06 08:20:01.039548 eventail-2.2.5/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1079 2023-06-06 08:20:00.000000 eventail-2.2.5/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-06-06 08:20:00.000000 eventail-2.2.5/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8234 2023-06-06 08:20:01.039548 eventail-2.2.5/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6154 2023-06-06 08:20:00.000000 eventail-2.2.5/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-06 08:20:01.039548 eventail-2.2.5/scripts/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4202 2023-06-06 08:20:00.000000 eventail-2.2.5/scripts/inspect_queue.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3742 2023-06-06 08:20:00.000000 eventail-2.2.5/scripts/logger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5358 2023-06-06 08:20:00.000000 eventail-2.2.5/scripts/monitor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2108 2023-06-06 08:20:00.000000 eventail-2.2.5/scripts/publish_configuration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3098 2023-06-06 08:20:00.000000 eventail-2.2.5/scripts/publish_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5297 2023-06-06 08:20:00.000000 eventail-2.2.5/scripts/resurrect.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3447 2023-06-06 08:20:00.000000 eventail-2.2.5/scripts/send_command.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-06-06 08:20:01.039548 eventail-2.2.5/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1351 2023-06-06 08:20:00.000000 eventail-2.2.5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-06 08:20:01.035548 eventail-2.2.5/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-06 08:20:01.039548 eventail-2.2.5/src/eventail/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1121 2023-06-06 08:20:00.000000 eventail-2.2.5/src/eventail/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-06 08:20:01.039548 eventail-2.2.5/src/eventail/async_service/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1121 2023-06-06 08:20:00.000000 eventail-2.2.5/src/eventail/async_service/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-06 08:20:01.039548 eventail-2.2.5/src/eventail/async_service/aio/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1181 2023-06-06 08:20:00.000000 eventail-2.2.5/src/eventail/async_service/aio/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23412 2023-06-06 08:20:00.000000 eventail-2.2.5/src/eventail/async_service/aio/base.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-06 08:20:01.039548 eventail-2.2.5/src/eventail/async_service/pika/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1242 2023-06-06 08:20:00.000000 eventail-2.2.5/src/eventail/async_service/pika/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    44888 2023-06-06 08:20:00.000000 eventail-2.2.5/src/eventail/async_service/pika/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2811 2023-06-06 08:20:00.000000 eventail-2.2.5/src/eventail/async_service/pika/supervisor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3576 2023-06-06 08:20:00.000000 eventail-2.2.5/src/eventail/batch_processor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1534 2023-06-06 08:20:00.000000 eventail-2.2.5/src/eventail/gelf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1380 2023-06-06 08:20:00.000000 eventail-2.2.5/src/eventail/log_criticity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-06 08:20:00.000000 eventail-2.2.5/src/eventail/py.typed
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7806 2023-06-06 08:20:00.000000 eventail-2.2.5/src/eventail/sync_publisher.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7622 2023-06-06 08:20:00.000000 eventail-2.2.5/src/eventail/tmp_store.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-06 08:20:01.039548 eventail-2.2.5/src/eventail.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8234 2023-06-06 08:20:01.000000 eventail-2.2.5/src/eventail.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      820 2023-06-06 08:20:01.000000 eventail-2.2.5/src/eventail.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-06 08:20:01.000000 eventail-2.2.5/src/eventail.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2023-06-06 08:20:01.000000 eventail-2.2.5/src/eventail.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        9 2023-06-06 08:20:01.000000 eventail-2.2.5/src/eventail.egg-info/top_level.txt
```

### Comparing `eventail-2.2.4/LICENSE` & `eventail-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `eventail-2.2.4/PKG-INFO` & `eventail-2.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventail
-Version: 2.2.4
+Version: 2.2.5
 Summary: A base class and utilities for AM service architecture
 Home-page: https://github.com/allo-media/eventail
 Author: Allo-Media
 Author-email: dev@allo-media.fr
 License: MIT
 Description: ![CircleCI](https://img.shields.io/circleci/build/github/allo-media/eventail)
         ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/eventail)
```

### Comparing `eventail-2.2.4/README.md` & `eventail-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `eventail-2.2.4/scripts/inspect_queue.py` & `eventail-2.2.5/scripts/inspect_queue.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.4/scripts/logger.py` & `eventail-2.2.5/scripts/logger.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.4/scripts/monitor.py` & `eventail-2.2.5/scripts/monitor.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.4/scripts/publish_configuration.py` & `eventail-2.2.5/scripts/publish_configuration.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.4/scripts/publish_event.py` & `eventail-2.2.5/scripts/publish_event.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.4/scripts/resurrect.py` & `eventail-2.2.5/scripts/resurrect.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.4/scripts/send_command.py` & `eventail-2.2.5/scripts/send_command.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.4/setup.py` & `eventail-2.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="eventail",
-    version="2.2.4",
+    version="2.2.5",
     url="https://github.com/allo-media/eventail",
     author="Allo-Media",
     author_email="dev@allo-media.fr",
     description="A base class and utilities for AM service architecture",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
```

### Comparing `eventail-2.2.4/src/eventail/__init__.py` & `eventail-2.2.5/src/eventail/__init__.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.4/src/eventail/async_service/__init__.py` & `eventail-2.2.5/src/eventail/async_service/__init__.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.4/src/eventail/async_service/aio/__init__.py` & `eventail-2.2.5/src/eventail/async_service/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.4/src/eventail/async_service/aio/base.py` & `eventail-2.2.5/src/eventail/async_service/aio/base.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.4/src/eventail/async_service/pika/__init__.py` & `eventail-2.2.5/src/eventail/async_service/pika/__init__.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.4/src/eventail/async_service/pika/base.py` & `eventail-2.2.5/src/eventail/async_service/pika/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,14 +132,15 @@
         self._bind_count = (
             (len(self._event_routing_keys) or 1)
             + (len(self._command_routing_keys) or 1)
             + (len(self._config_routing_keys) or 1)
         )
         self.should_reconnect = False
         self.was_consuming = False
+        self._configured = not self._config_routing_keys
 
         self._closing = False
         self._event_consumer_tag: Optional[str] = None
         self._command_consumer_tag: Optional[str] = None
         self._config_consumer_tag: Optional[str] = None
         self._consuming = False
```

### Comparing `eventail-2.2.4/src/eventail/async_service/pika/supervisor.py` & `eventail-2.2.5/src/eventail/async_service/pika/supervisor.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.4/src/eventail/batch_processor.py` & `eventail-2.2.5/src/eventail/batch_processor.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.4/src/eventail/gelf.py` & `eventail-2.2.5/src/eventail/gelf.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.4/src/eventail/log_criticity.py` & `eventail-2.2.5/src/eventail/log_criticity.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.4/src/eventail/sync_publisher.py` & `eventail-2.2.5/src/eventail/sync_publisher.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.4/src/eventail/tmp_store.py` & `eventail-2.2.5/src/eventail/tmp_store.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.4/src/eventail.egg-info/PKG-INFO` & `eventail-2.2.5/src/eventail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventail
-Version: 2.2.4
+Version: 2.2.5
 Summary: A base class and utilities for AM service architecture
 Home-page: https://github.com/allo-media/eventail
 Author: Allo-Media
 Author-email: dev@allo-media.fr
 License: MIT
 Description: ![CircleCI](https://img.shields.io/circleci/build/github/allo-media/eventail)
         ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/eventail)
```

### Comparing `eventail-2.2.4/src/eventail.egg-info/SOURCES.txt` & `eventail-2.2.5/src/eventail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

