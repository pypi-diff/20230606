# Comparing `tmp/asynciomultiplexer-1.0.1.tar.gz` & `tmp/asynciomultiplexer-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asynciomultiplexer-1.0.1.tar", last modified: Mon May 29 23:40:40 2023, max compression
+gzip compressed data, was "asynciomultiplexer-1.1.0.tar", last modified: Tue Jun  6 04:05:40 2023, max compression
```

## Comparing `asynciomultiplexer-1.0.1.tar` & `asynciomultiplexer-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-05-29 23:40:40.125461 asynciomultiplexer-1.0.1/
--rw-rw-r--   0 pi        (1000) pi        (1000)     1490 2023-05-29 22:44:19.000000 asynciomultiplexer-1.0.1/LICENSE
--rw-rw-r--   0 pi        (1000) pi        (1000)      138 2023-05-29 23:40:40.125461 asynciomultiplexer-1.0.1/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      106 2023-05-29 22:44:19.000000 asynciomultiplexer-1.0.1/README.md
--rw-rw-r--   0 pi        (1000) pi        (1000)       38 2023-05-29 23:40:40.125461 asynciomultiplexer-1.0.1/setup.cfg
--rw-rw-r--   0 pi        (1000) pi        (1000)      345 2023-05-29 23:40:23.000000 asynciomultiplexer-1.0.1/setup.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-05-29 23:40:40.125461 asynciomultiplexer-1.0.1/src/
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-05-29 23:40:40.125461 asynciomultiplexer-1.0.1/src/asynciomultiplexer/
--rw-rw-r--   0 pi        (1000) pi        (1000)     4669 2023-05-29 23:40:23.000000 asynciomultiplexer-1.0.1/src/asynciomultiplexer/asynciomultiplexer.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-05-29 23:40:40.125461 asynciomultiplexer-1.0.1/src/asynciomultiplexer.egg-info/
--rw-rw-r--   0 pi        (1000) pi        (1000)      138 2023-05-29 23:40:40.000000 asynciomultiplexer-1.0.1/src/asynciomultiplexer.egg-info/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      281 2023-05-29 23:40:40.000000 asynciomultiplexer-1.0.1/src/asynciomultiplexer.egg-info/SOURCES.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-05-29 23:40:40.000000 asynciomultiplexer-1.0.1/src/asynciomultiplexer.egg-info/dependency_links.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       19 2023-05-29 23:40:40.000000 asynciomultiplexer-1.0.1/src/asynciomultiplexer.egg-info/top_level.txt
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-05-29 23:40:40.125461 asynciomultiplexer-1.0.1/test/
--rw-rw-r--   0 pi        (1000) pi        (1000)      524 2023-05-29 23:04:29.000000 asynciomultiplexer-1.0.1/test/test_multiplexing.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-06 04:05:40.499729 asynciomultiplexer-1.1.0/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1490 2023-05-29 22:44:19.000000 asynciomultiplexer-1.1.0/LICENSE
+-rw-rw-r--   0 pi        (1000) pi        (1000)      138 2023-06-06 04:05:40.499729 asynciomultiplexer-1.1.0/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      106 2023-05-29 22:44:19.000000 asynciomultiplexer-1.1.0/README.md
+-rw-rw-r--   0 pi        (1000) pi        (1000)       38 2023-06-06 04:05:40.499729 asynciomultiplexer-1.1.0/setup.cfg
+-rw-rw-r--   0 pi        (1000) pi        (1000)      345 2023-06-06 04:05:06.000000 asynciomultiplexer-1.1.0/setup.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-06 04:05:40.495728 asynciomultiplexer-1.1.0/src/
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-06 04:05:40.499729 asynciomultiplexer-1.1.0/src/asynciomultiplexer/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     5868 2023-06-06 04:00:41.000000 asynciomultiplexer-1.1.0/src/asynciomultiplexer/asynciomultiplexer.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-06 04:05:40.499729 asynciomultiplexer-1.1.0/src/asynciomultiplexer.egg-info/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      138 2023-06-06 04:05:40.000000 asynciomultiplexer-1.1.0/src/asynciomultiplexer.egg-info/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      281 2023-06-06 04:05:40.000000 asynciomultiplexer-1.1.0/src/asynciomultiplexer.egg-info/SOURCES.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-06-06 04:05:40.000000 asynciomultiplexer-1.1.0/src/asynciomultiplexer.egg-info/dependency_links.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       19 2023-06-06 04:05:40.000000 asynciomultiplexer-1.1.0/src/asynciomultiplexer.egg-info/top_level.txt
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-06 04:05:40.499729 asynciomultiplexer-1.1.0/test/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1324 2023-06-06 04:03:49.000000 asynciomultiplexer-1.1.0/test/test_multiplexing.py
```

### Comparing `asynciomultiplexer-1.0.1/LICENSE` & `asynciomultiplexer-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asynciomultiplexer-1.0.1/src/asynciomultiplexer/asynciomultiplexer.py` & `asynciomultiplexer-1.1.0/src/asynciomultiplexer/asynciomultiplexer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,81 +1,107 @@
 """
 multiplexing utils for parallel (async) tasks
 """
 
 import asyncio
 import queue
-from typing import AsyncIterator, TypeVar, Generic
+from contextlib import suppress
+from typing import AsyncIterator, TypeVar, Generic, Optional, Callable, AsyncGenerator
 
 __all__ = ["AsyncMultiplexedIterator", "AsyncAdaptorQueue"]
 T = TypeVar('T')
 
 
 class AsyncMultiplexedIterator(Generic[T]):
     """
     Class for multiplexing multiple async iterators in parallel into a single async iterator
 
     >>> iterators: AsyncIterator[T] = ...
-    ... async for device_data in AsyncMultiplexedIterator(*iterators):
-    ...     yield device_data
+    ... with  AsyncMultiplexedIterator(*iterators) as multiplexre:
+    ...     async for device_data in AsyncMultiplexedIterator(*iterators):
+    ...         yield device_data
     """
 
     class Sentinel:
         """
         To mark the end of iteration in the multiplexing queue
         """
         def __init__(self, iterator: AsyncIterator[T]):
             self._iterator = iterator
 
         @property
         def iterator(self) -> AsyncIterator[T]:
             return self._iterator
 
-    def __init__(self, *iterators: AsyncIterator[T], timeout=0):
+    def __init__(self, *iterators: AsyncIterator[T], timeout=0,
+                 handle_orphan: Optional[Callable[[T], None]] = None):
         """
         :param iterators: which iterators to iterate over in parallel
         :param timeout: timeout in seconds to wait on next item, or default/zero to wait indefinitely
+        :param handle_orphan: optional callback to handle orphaned items.  An itme is orphaned when
+            the multiplexer exits early but the client inserts an item into the multiplexing queue
+            AFTER the multiplexer stops processing the queue but BEFORE it has properly shutdown
+            all the workers.  Any exceptions from this handler will be ignored and not propagated.
         """
         self._iterators = list(iterators)
         self._multiplexing_q: asyncio.Queue[T] = asyncio.Queue()
         self._timeout = timeout
+        self._handle_orphan = handle_orphan
+        self._active = False
+
+    async def __aenter__(self):
+        return self
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        self._active = False
+        for task in [t for t in self._tasks if not t.done()]:
+            await task
+        while self._handle_orphan is not None:  # always True or False
+            try:
+                item = self._multiplexing_q.get_nowait()
+                with suppress(Exception):
+                    self._handle_orphan(item)
+            except asyncio.queues.QueueEmpty:
+                break
 
     def __aiter__(self) -> "AsyncMultiplexedIterator[T]":
         async def worker(iterator: AsyncIterator[T]):
             try:
                 async for item in iterator:
+                    if not self._active:
+                        break
                     await self._multiplexing_q.put(item)
-            except BaseException as e:
+            except Exception as e:
                 await self._multiplexing_q.put(e)
+                raise
             finally:
-                await self._multiplexing_q.put(self.Sentinel(iterator))
+                if self._active:
+                    await self._multiplexing_q.put(self.Sentinel(iterator))
+
         self._tasks = [
             asyncio.create_task(worker(iterator)) for iterator in self._iterators
         ]
+        self._active = True
         return self
 
     async def __anext__(self) -> T:
-        try:
-            while self._iterators:
-                if self._timeout > 0:
-                    next_item = await asyncio.wait_for(self._multiplexing_q.get(), timeout=self._timeout)
-                else:
-                    next_item = await self._multiplexing_q.get()
-                if isinstance(next_item, BaseException):
-                    raise StopAsyncIteration() from next_item
-                elif isinstance(next_item, self.Sentinel):
-                    self._iterators.remove(next_item.iterator)
-                    if not self._iterators:
-                        raise StopAsyncIteration()
-                    continue
-                return next_item
-        except Exception:
-            for task in [t for t in self._tasks if not t.done()]:
-                task.cancel()
-            raise
+        while self._iterators:
+            if self._timeout > 0:
+                next_item = await asyncio.wait_for(self._multiplexing_q.get(), timeout=self._timeout)
+            else:
+                next_item = await self._multiplexing_q.get()
+            if isinstance(next_item, BaseException):
+                raise StopAsyncIteration() from next_item
+            elif isinstance(next_item, self.Sentinel):
+                self._iterators.remove(next_item.iterator)
+                if not self._iterators:
+                    self._active = False
+                    raise StopAsyncIteration()
+                continue
+            return next_item
 
 
 class AsyncAdaptorQueue(Generic[T]):
     """
     A sync-to-async bridge needed for communicating across async loops in multiple threads.
     Since async tasks cannot interact across threads directly, such a queue is needed that
     uses polling-with-sleep on the sync queue to convert to an async method
```

