# Comparing `tmp/eidolon-0.1.0.tar.gz` & `tmp/eidolon-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eidolon-0.1.0.tar", max compression
+gzip compressed data, was "eidolon-0.1.1.tar", max compression
```

## Comparing `eidolon-0.1.0.tar` & `eidolon-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      116 2023-06-06 19:51:32.894643 eidolon-0.1.0/README.md
--rw-r--r--   0        0        0     4861 2023-06-06 19:30:56.508608 eidolon-0.1.0/eidolon/__init__.py
--rw-r--r--   0        0        0     3197 2023-06-06 19:30:56.508608 eidolon-0.1.0/eidolon/api_request.py
--rw-r--r--   0        0        0      549 2023-06-06 17:58:02.453446 eidolon-0.1.0/eidolon/tracker.py
--rw-r--r--   0        0        0      495 2023-06-06 19:28:43.173013 eidolon-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      814 1970-01-01 00:00:00.000000 eidolon-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      116 2023-06-06 19:51:32.894643 eidolon-0.1.1/README.md
+-rw-r--r--   0        0        0     4861 2023-06-06 19:30:56.508608 eidolon-0.1.1/eidolon/__init__.py
+-rw-r--r--   0        0        0     3174 2023-06-06 20:01:33.035631 eidolon-0.1.1/eidolon/api_request.py
+-rw-r--r--   0        0        0      549 2023-06-06 17:58:02.453446 eidolon-0.1.1/eidolon/tracker.py
+-rw-r--r--   0        0        0      495 2023-06-06 20:05:10.338654 eidolon-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      814 1970-01-01 00:00:00.000000 eidolon-0.1.1/PKG-INFO
```

### Comparing `eidolon-0.1.0/eidolon/__init__.py` & `eidolon-0.1.1/eidolon/__init__.py`

 * *Files identical despite different names*

### Comparing `eidolon-0.1.0/eidolon/api_request.py` & `eidolon-0.1.1/eidolon/api_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 import asyncio
 from dataclasses import dataclass, field
 import inspect
 import logging
 import time
-from typing import Callable, Dict, Literal
+from typing import Awaitable, Callable, Dict, Literal, Optional, Union
 import aiohttp
 from yarl import URL
 
 from eidolon.tracker import StatusTracker
 
 
 @dataclass
 class APIRequest:
     """Stores an API request's inputs, outputs, and other metadata. Contains a method to make an API call."""
 
     task_id: int
     attempts_left: int
-    result: list = field(default_factory=list)
-    callback: Callable[[dict, dict], None] = None
+    callback: Callable[[dict, dict], Awaitable[None]] = None
     request_method: Literal[
         "GET", "POST", "HEAD", "PUT", "DELETE", "CONNECT", "OPTIONS", "TRACE", "PATCH"
-    ] = None
-    request_headers: Dict[str, str] | None = None
-    request_json: dict | None = None
-    request_params: dict | None = None
-    request_form_data: aiohttp.FormData | dict | bytes | None = None
-    request_url: str | URL = None
+    ] = "GET"
+    request_headers: Optional[Dict[str, str]] = None
+    request_json: Optional[dict] = None
+    request_params: Optional[dict] = None
+    request_form_data: Optional[Union[aiohttp.FormData, dict, bytes]]  = None
+    request_url: Optional[Union[str, URL]] = None
 
     async def call_api(
         self,
         retry_queue: asyncio.Queue,
         status_tracker: StatusTracker,
     ):
         """Calls the API and saves results."""
@@ -46,15 +45,14 @@
                             f"Request {self.task_id} failed with status 429"
                         )
                         status_tracker.num_rate_limit_errors += 1
                         status_tracker.time_of_last_rate_limit_error = time.time()
                         error = True
                     
                     if error:
-                        self.result.append(error)
                         if self.attempts_left:
                             retry_queue.put_nowait(self)
                         else:
                             logging.error(f"Request {self.request_json} failed after all attempts.")
 
                             status_tracker.num_tasks_in_progress -= 1
                             status_tracker.num_tasks_failed += 1
```

### Comparing `eidolon-0.1.0/eidolon/tracker.py` & `eidolon-0.1.1/eidolon/tracker.py`

 * *Files identical despite different names*

### Comparing `eidolon-0.1.0/PKG-INFO` & `eidolon-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eidolon
-Version: 0.1.0
+Version: 0.1.1
 Summary: A utility to concurrently make HTTP requests, with an optional rate limit. Powered by asyncio and aiohttp
 License: MIT
 Author: Sphericalkat
 Author-email: amolele@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

