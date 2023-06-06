# Comparing `tmp/motion_python-0.1.56.tar.gz` & `tmp/motion_python-0.1.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.56.tar", max compression
+gzip compressed data, was "motion_python-0.1.57.tar", max compression
```

## Comparing `motion_python-0.1.56.tar` & `motion_python-0.1.57.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3344 2023-06-05 18:15:48.822358 motion_python-0.1.56/README.md
--rw-r--r--   0        0        0      221 2023-06-05 18:15:48.826358 motion_python-0.1.56/motion/__init__.py
--rw-r--r--   0        0        0     2883 2023-06-05 18:15:48.826358 motion_python-0.1.56/motion/cli.py
--rw-r--r--   0        0        0    23617 2023-06-05 18:15:48.826358 motion_python-0.1.56/motion/component.py
--rw-r--r--   0        0        0    14675 2023-06-05 18:15:48.826358 motion_python-0.1.56/motion/execute.py
--rw-r--r--   0        0        0     5209 2023-06-05 18:15:48.826358 motion_python-0.1.56/motion/fit_task.py
--rw-r--r--   0        0        0    10317 2023-06-05 18:15:48.826358 motion_python-0.1.56/motion/instance.py
--rw-r--r--   0        0        0    13660 2023-06-05 18:15:48.826358 motion_python-0.1.56/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0      595 2023-06-05 18:15:48.826358 motion_python-0.1.56/motion/route.py
--rw-r--r--   0        0        0     7616 2023-06-05 18:15:48.826358 motion_python-0.1.56/motion/utils.py
--rw-r--r--   0        0        0     1572 2023-06-05 18:16:09.062633 motion_python-0.1.56/pyproject.toml
--rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.56/PKG-INFO
+-rw-r--r--   0        0        0     3344 2023-06-06 04:57:08.743146 motion_python-0.1.57/README.md
+-rw-r--r--   0        0        0      221 2023-06-06 04:57:08.747146 motion_python-0.1.57/motion/__init__.py
+-rw-r--r--   0        0        0     2883 2023-06-06 04:57:08.747146 motion_python-0.1.57/motion/cli.py
+-rw-r--r--   0        0        0    23617 2023-06-06 04:57:08.747146 motion_python-0.1.57/motion/component.py
+-rw-r--r--   0        0        0    17368 2023-06-06 04:57:08.747146 motion_python-0.1.57/motion/execute.py
+-rw-r--r--   0        0        0     5406 2023-06-06 04:57:08.747146 motion_python-0.1.57/motion/fit_task.py
+-rw-r--r--   0        0        0    12513 2023-06-06 04:57:08.747146 motion_python-0.1.57/motion/instance.py
+-rw-r--r--   0        0        0    13660 2023-06-06 04:57:08.747146 motion_python-0.1.57/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0      619 2023-06-06 04:57:08.747146 motion_python-0.1.57/motion/route.py
+-rw-r--r--   0        0        0     7616 2023-06-06 04:57:08.747146 motion_python-0.1.57/motion/utils.py
+-rw-r--r--   0        0        0     1736 2023-06-06 04:57:34.799300 motion_python-0.1.57/pyproject.toml
+-rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.57/PKG-INFO
```

### Comparing `motion_python-0.1.56/README.md` & `motion_python-0.1.57/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.56/motion/cli.py` & `motion_python-0.1.57/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.56/motion/component.py` & `motion_python-0.1.57/motion/component.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.56/motion/execute.py` & `motion_python-0.1.57/motion/execute.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import asyncio
 import multiprocessing
 import threading
-from typing import Any, Callable, Dict, List, Optional
+from typing import Any, Callable, Dict, List, Optional, Tuple
 from uuid import uuid4
 
 import cloudpickle
 import psutil
 import redis
 from redis.lock import Lock
 
@@ -252,75 +253,22 @@
     def empty_batch(self) -> Dict[str, List[Any]]:
         return {
             "fit_events": [],
             "values": [],
             "infer_results": [],
         }
 
-    def run(
+    def _enqueue_and_trigger_fit(
         self,
         key: str,
         value: Any,
-        cache_ttl: int,
-        force_refresh: bool,
+        infer_result: Any,
         flush_fit: bool,
-    ) -> Any:
-        route_hit = False
-        infer_result = None
-
-        # Run the infer route
-        if key in self._infer_routes.keys():
-            route_hit = True
-            route_run = False
-
-            if force_refresh:
-                self._state = self._loadState()
-                v = self._redis_con.get(f"MOTION_VERSION:{self._instance_name}")
-                if not v:
-                    raise ValueError(
-                        f"Error loading state for {self._instance_name}."
-                        + " No version found."
-                    )
-                self.version = int(v)
-
-            # Try hashing the value
-            try:
-                value_hash = hash_object(value)
-            except TypeError:
-                value_hash = None
-
-            # Check if key is in cache if value can be hashed and
-            # user doesn't want to force refresh state
-            if value_hash and not force_refresh:
-                cache_result_key = (
-                    f"MOTION_RESULT:{self._instance_name}/{key}/{value_hash}"
-                )
-                if self._redis_con.exists(cache_result_key):
-                    infer_result = cloudpickle.loads(
-                        self._redis_con.get(cache_result_key)
-                    )
-                    route_run = True
-
-            # If not in cache or value can't be hashed or
-            # user wants to force refresh state, run route
-            if not route_run:
-                infer_result = self._infer_routes[key].run(
-                    state=self._state, value=value
-                )
-                # Cache result
-                if value_hash:
-                    cache_result_key = (
-                        f"MOTION_RESULT:{self._instance_name}/{key}/{value_hash}"
-                    )
-                    self._redis_con.set(
-                        cache_result_key,
-                        cloudpickle.dumps(infer_result),
-                        ex=cache_ttl,
-                    )
-
+        route_hit: bool,
+    ) -> bool:
         # Run the fit routes
         # Enqueue results into fit queues
         if key in self._fit_routes.keys():
             route_hit = True
 
             fit_events = FitEventGroup(key)
             for fit_udf_name in self._fit_routes[key].keys():
@@ -362,14 +310,154 @@
                 if not v:
                     raise ValueError(
                         f"Error loading state for {self._instance_name}."
                         + " No version found."
                     )
                 self.version = int(v)
 
+        return route_hit
+
+    def _try_cached_infer(
+        self,
+        key: str,
+        value: Any,
+        force_refresh: bool,
+    ) -> Tuple[bool, Optional[Any], Optional[str]]:
+        route_run = False
+        infer_result = None
+
+        if force_refresh:
+            self._state = self._loadState()
+            v = self._redis_con.get(f"MOTION_VERSION:{self._instance_name}")
+            if not v:
+                raise ValueError(
+                    f"Error loading state for {self._instance_name}."
+                    + " No version found."
+                )
+            self.version = int(v)
+
+        # Try hashing the value
+        try:
+            value_hash = hash_object(value)
+        except TypeError:
+            value_hash = None
+
+        # Check if key is in cache if value can be hashed and
+        # user doesn't want to force refresh state
+        if value_hash and not force_refresh:
+            cache_result_key = f"MOTION_RESULT:{self._instance_name}/{key}/{value_hash}"
+            if self._redis_con.exists(cache_result_key):
+                infer_result = cloudpickle.loads(self._redis_con.get(cache_result_key))
+                route_run = True
+
+        return route_run, infer_result, value_hash
+
+    def run(
+        self,
+        key: str,
+        value: Any,
+        cache_ttl: int,
+        force_refresh: bool,
+        flush_fit: bool,
+    ) -> Any:
+        route_hit = False
+        infer_result = None
+
+        # Run the infer route
+        if key in self._infer_routes.keys():
+            route_hit = True
+            route_run, infer_result, value_hash = self._try_cached_infer(
+                key, value, force_refresh
+            )
+
+            # If not in cache or value can't be hashed or
+            # user wants to force refresh state, run route
+            if not route_run:
+                infer_result = self._infer_routes[key].run(
+                    state=self._state, value=value
+                )
+
+                # Check that infer_result is not an awaitable
+                if asyncio.iscoroutine(infer_result):
+                    raise TypeError(
+                        f"Route {key} returned an awaitable. "
+                        + "Call `await instance.arun(...)` instead."
+                    )
+
+                # Cache result
+                if value_hash:
+                    cache_result_key = (
+                        f"MOTION_RESULT:{self._instance_name}/{key}/{value_hash}"
+                    )
+                    self._redis_con.set(
+                        cache_result_key,
+                        cloudpickle.dumps(infer_result),
+                        ex=cache_ttl,
+                    )
+
+        # Run the fit routes
+        # Enqueue results into fit queues
+        route_hit = self._enqueue_and_trigger_fit(
+            key, value, infer_result, flush_fit, route_hit
+        )
+
+        if not route_hit:
+            raise KeyError(f"Key {key} not in routes.")
+
+        return infer_result
+
+    async def arun(
+        self,
+        key: str,
+        value: Any,
+        cache_ttl: int,
+        force_refresh: bool,
+        flush_fit: bool,
+    ) -> Any:
+        route_hit = False
+        infer_result = None
+
+        # Run the infer route
+        if key in self._infer_routes.keys():
+            route_hit = True
+            route_run, infer_result, value_hash = self._try_cached_infer(
+                key, value, force_refresh
+            )
+
+            # If not in cache or value can't be hashed or
+            # user wants to force refresh state, run route
+            if not route_run:
+                infer_result_awaitable = self._infer_routes[key].run(
+                    state=self._state, value=value
+                )
+                if not asyncio.iscoroutine(infer_result_awaitable):
+                    raise TypeError(
+                        f"Route {key} returned a non-awaitable. "
+                        + "Call `instance.run(...)` instead."
+                    )
+
+                infer_result = await infer_result_awaitable
+
+                # Cache result
+                if value_hash:
+                    cache_result_key = (
+                        f"MOTION_RESULT:{self._instance_name}/{key}/{value_hash}"
+                    )
+                    self._redis_con.set(
+                        cache_result_key,
+                        cloudpickle.dumps(infer_result),
+                        ex=cache_ttl,
+                    )
+
+        # Run the fit routes
+        # Enqueue results into fit queues
+        route_hit = self._enqueue_and_trigger_fit(
+            key, value, infer_result, flush_fit, route_hit
+        )
+
         if not route_hit:
             raise KeyError(f"Key {key} not in routes.")
 
         return infer_result
 
     def flush_fit(self, dataflow_key: str) -> None:
         # Check if key has fit ops
```

### Comparing `motion_python-0.1.56/motion/fit_task.py` & `motion_python-0.1.57/motion/fit_task.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import multiprocessing
 from typing import Any, Callable, List, Optional
 
 import cloudpickle
 import redis
 from redis.lock import Lock
 
@@ -108,14 +109,17 @@
                         redis_con, self.instance_name, self.load_state_func
                     )
                     state_update = self.route.run(
                         state=old_state,
                         values=values,
                         infer_results=infer_results,
                     )
+                    # Await if state_update is a coroutine
+                    if asyncio.iscoroutine(state_update):
+                        state_update = asyncio.run(state_update)
 
                     if not isinstance(state_update, dict):
                         logger.error(
                             "fit methods should return a dict of state updates."
                         )
                     else:
                         old_state.update(state_update)
```

### Comparing `motion_python-0.1.56/motion/instance.py` & `motion_python-0.1.57/motion/instance.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import atexit
 import logging
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+from typing import Any, Awaitable, Callable, Dict, List, Optional
 
 from motion.execute import Executor
 from motion.route import Route
-from motion.utils import DEFAULT_KEY_TTL, FitEventGroup, configureLogging, logger
+from motion.utils import DEFAULT_KEY_TTL, configureLogging, logger
 
 
 def is_logger_open(logger: logging.Logger) -> bool:
     for handler in logger.handlers:
         if (
             hasattr(handler, "stream")
             and handler.stream is not None
@@ -239,15 +239,15 @@
     def run(
         self,
         *,
         cache_ttl: int = DEFAULT_KEY_TTL,
         force_refresh: bool = False,
         flush_fit: bool = False,
         **kwargs: Any,
-    ) -> Union[Any, Tuple[Any, FitEventGroup]]:
+    ) -> Any:
         """Runs the dataflow (infer and fit ops) for the keyword argument
         passed in. If the key is not found to have any ops, an error
         is raised. Only one keyword argument should be passed in.
         Fit ops are only executed when the batch size is reached.
 
         Example Usage:
         ```python
@@ -323,7 +323,75 @@
             value=value,
             cache_ttl=cache_ttl,
             force_refresh=force_refresh,
             flush_fit=flush_fit,
         )
 
         return infer_result
+
+    async def arun(
+        self,
+        *,
+        cache_ttl: int = DEFAULT_KEY_TTL,
+        force_refresh: bool = False,
+        flush_fit: bool = False,
+        **kwargs: Any,
+    ) -> Awaitable[Any]:
+        """Async version of run. Runs the dataflow (infer and fit ops) for the .
+        keyword argument.
+
+        Example Usage:
+        ```python
+        from motion import Component
+        import asyncio
+
+        C = Component("MyComponent")
+
+        @C.infer("sleep")
+        async def sleep(state, value):
+            await asyncio.sleep(value)
+            return "Slept!"
+
+        async def main():
+            c = C()
+            await c.arun(sleep=1)
+
+        if __name__ == "__main__":
+            asyncio.run(main())
+        ```
+
+        Args:
+            cache_ttl (int, optional):
+                How long the inference result should live in a cache (in
+                seconds). Defaults to 1 day (60 * 60 * 24).
+            force_refresh (bool, optional): Read the latest value of the
+                state before running an inference call, otherwise a stale
+                version of the state or a cached result may be used.
+                If you do not want to read from the cache, set force_refresh
+                = True. Defaults to False.
+            flush_fit (bool, optional):
+                If True, waits for the fit op to finish executing before
+                returning. If the fit queue hasn't reached batch_size
+                yet, the fit op runs anyways. Force refreshes the
+                state after the fit op completes. Defaults to False.
+            **kwargs:
+                Keyword arguments for the infer and fit ops. You can only
+                pass in one pair.
+
+        Returns:
+            Awaitable[Any]: Awaitable Result of the inference call.
+        """
+
+        if len(kwargs) != 1:
+            raise ValueError("Only one key-value pair is allowed in kwargs.")
+
+        key, value = next(iter(kwargs.items()))
+
+        infer_result = await self._executor.arun(
+            key=key,
+            value=value,
+            cache_ttl=cache_ttl,
+            force_refresh=force_refresh,
+            flush_fit=flush_fit,
+        )  # type: ignore
+
+        return infer_result  # type: ignore
```

### Comparing `motion_python-0.1.56/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.57/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.56/motion/route.py` & `motion_python-0.1.57/motion/route.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,8 +10,9 @@
         ...,
         description="The udf to call for the op. The udf should have 2 args:"
         + " `state` and `value` for `infer` and 3 arguments: `state`, "
         + "`values`, and `infer_results` for `fit`.",
     )
 
     def run(self, **kwargs: Any) -> Any:
-        return self.udf(**kwargs)
+        result = self.udf(**kwargs)
+        return result
```

### Comparing `motion_python-0.1.56/motion/utils.py` & `motion_python-0.1.57/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.56/pyproject.toml` & `motion_python-0.1.57/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.56"
+version = "0.1.57"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -33,21 +33,28 @@
 ruff = "^0.0.261"
 maturin = "^0.14.17"
 mike = "^1.1.2"
 scikit-learn = "^1.2.2"
 types-redis = "^4.5.5.2"
 fastapi = "^0.95.2"
 httpx = "^0.24.1"
+pytest-asyncio = "^0.21.0"
+pytest-timeout = "^2.1.0"
 
 [tool.poetry.scripts]
 motion = "motion.cli:motioncli"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 addopts = "--basetemp=/tmp/pytest"
+filterwarnings = [
+    "ignore::DeprecationWarning",
+    "ignore::UserWarning",
+    "ignore::RuntimeWarning"
+]
 
 [tool.mypy]
 files = "motion"
 mypy_path = "motion"
 warn_return_any = true
 warn_unused_configs = true
 disallow_untyped_defs = true
```

### Comparing `motion_python-0.1.56/PKG-INFO` & `motion_python-0.1.57/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.56
+Version: 0.1.57
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

