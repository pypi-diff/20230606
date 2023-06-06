# Comparing `tmp/timering-1.0.1.tar.gz` & `tmp/timering-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timering-1.0.1.tar", last modified: Mon Jun  5 22:37:21 2023, max compression
+gzip compressed data, was "timering-1.0.2.tar", last modified: Tue Jun  6 18:33:21 2023, max compression
```

## Comparing `timering-1.0.1.tar` & `timering-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-x---   0 jonas     (1000) jonas     (1000)        0 2023-06-05 22:37:21.741737 timering-1.0.1/
--rw-r-----   0 jonas     (1000) jonas     (1000)     1498 2023-06-04 09:27:36.000000 timering-1.0.1/LICENSE
--rw-r-----   0 jonas     (1000) jonas     (1000)     5695 2023-06-05 22:37:21.741737 timering-1.0.1/PKG-INFO
--rw-r-----   0 jonas     (1000) jonas     (1000)     3269 2023-06-05 21:04:03.000000 timering-1.0.1/README.md
--rw-r-----   0 jonas     (1000) jonas     (1000)        6 2023-06-05 22:37:12.000000 timering-1.0.1/VERSION
--rw-r-----   0 jonas     (1000) jonas     (1000)       38 2023-06-05 22:37:21.741737 timering-1.0.1/setup.cfg
--rw-r-----   0 jonas     (1000) jonas     (1000)     1412 2023-06-05 22:35:19.000000 timering-1.0.1/setup.py
-drwxr-x---   0 jonas     (1000) jonas     (1000)        0 2023-06-05 22:37:21.741737 timering-1.0.1/src/
-drwxr-x---   0 jonas     (1000) jonas     (1000)        0 2023-06-05 22:37:21.741737 timering-1.0.1/src/timering.egg-info/
--rw-r-----   0 jonas     (1000) jonas     (1000)     5695 2023-06-05 22:37:21.000000 timering-1.0.1/src/timering.egg-info/PKG-INFO
--rw-r-----   0 jonas     (1000) jonas     (1000)      303 2023-06-05 22:37:21.000000 timering-1.0.1/src/timering.egg-info/SOURCES.txt
--rw-r-----   0 jonas     (1000) jonas     (1000)        1 2023-06-05 22:37:21.000000 timering-1.0.1/src/timering.egg-info/dependency_links.txt
--rw-r-----   0 jonas     (1000) jonas     (1000)       30 2023-06-05 22:37:21.000000 timering-1.0.1/src/timering.egg-info/requires.txt
--rw-r-----   0 jonas     (1000) jonas     (1000)        7 2023-06-05 22:37:21.000000 timering-1.0.1/src/timering.egg-info/top_level.txt
-drwxr-x---   0 jonas     (1000) jonas     (1000)        0 2023-06-05 22:37:21.741737 timering-1.0.1/src/timing/
--rw-r-----   0 jonas     (1000) jonas     (1000)      361 2023-06-05 22:28:21.000000 timering-1.0.1/src/timing/__init__.py
--rw-r-----   0 jonas     (1000) jonas     (1000)     9938 2023-06-05 20:44:41.000000 timering-1.0.1/src/timing/timing.py
-drwxr-x---   0 jonas     (1000) jonas     (1000)        0 2023-06-05 22:37:21.741737 timering-1.0.1/tests/
--rw-r-----   0 jonas     (1000) jonas     (1000)     1197 2023-06-04 18:13:12.000000 timering-1.0.1/tests/test_functions.py
--rw-r-----   0 jonas     (1000) jonas     (1000)     2252 2023-06-04 18:53:19.000000 timering-1.0.1/tests/test_methods.py
+drwxr-x---   0 jonas     (1000) jonas     (1000)        0 2023-06-06 18:33:21.682999 timering-1.0.2/
+-rw-r-----   0 jonas     (1000) jonas     (1000)     1498 2023-06-04 09:27:36.000000 timering-1.0.2/LICENSE
+-rw-r-----   0 jonas     (1000) jonas     (1000)     5922 2023-06-06 18:33:21.682999 timering-1.0.2/PKG-INFO
+-rw-r-----   0 jonas     (1000) jonas     (1000)     3359 2023-06-06 17:42:48.000000 timering-1.0.2/README.md
+-rw-r-----   0 jonas     (1000) jonas     (1000)        6 2023-06-06 17:02:40.000000 timering-1.0.2/VERSION
+-rw-r-----   0 jonas     (1000) jonas     (1000)     1233 2023-06-06 18:33:02.000000 timering-1.0.2/pyproject.toml
+-rw-r-----   0 jonas     (1000) jonas     (1000)       38 2023-06-06 18:33:21.682999 timering-1.0.2/setup.cfg
+drwxr-x---   0 jonas     (1000) jonas     (1000)        0 2023-06-06 18:33:21.678999 timering-1.0.2/src/
+drwxr-x---   0 jonas     (1000) jonas     (1000)        0 2023-06-06 18:33:21.678999 timering-1.0.2/src/timering.egg-info/
+-rw-r-----   0 jonas     (1000) jonas     (1000)     5922 2023-06-06 18:33:21.000000 timering-1.0.2/src/timering.egg-info/PKG-INFO
+-rw-r-----   0 jonas     (1000) jonas     (1000)      309 2023-06-06 18:33:21.000000 timering-1.0.2/src/timering.egg-info/SOURCES.txt
+-rw-r-----   0 jonas     (1000) jonas     (1000)        1 2023-06-06 18:33:21.000000 timering-1.0.2/src/timering.egg-info/dependency_links.txt
+-rw-r-----   0 jonas     (1000) jonas     (1000)       68 2023-06-06 18:33:21.000000 timering-1.0.2/src/timering.egg-info/requires.txt
+-rw-r-----   0 jonas     (1000) jonas     (1000)        7 2023-06-06 18:33:21.000000 timering-1.0.2/src/timering.egg-info/top_level.txt
+drwxr-x---   0 jonas     (1000) jonas     (1000)        0 2023-06-06 18:33:21.678999 timering-1.0.2/src/timing/
+-rw-r-----   0 jonas     (1000) jonas     (1000)     2068 2023-06-06 17:12:46.000000 timering-1.0.2/src/timing/__init__.py
+-rw-r-----   0 jonas     (1000) jonas     (1000)     8301 2023-06-06 17:22:49.000000 timering-1.0.2/src/timing/timing.py
+drwxr-x---   0 jonas     (1000) jonas     (1000)        0 2023-06-06 18:33:21.682999 timering-1.0.2/tests/
+-rw-r-----   0 jonas     (1000) jonas     (1000)     1197 2023-06-04 18:13:12.000000 timering-1.0.2/tests/test_functions.py
+-rw-r-----   0 jonas     (1000) jonas     (1000)     2252 2023-06-04 18:53:19.000000 timering-1.0.2/tests/test_methods.py
```

### Comparing `timering-1.0.1/LICENSE` & `timering-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `timering-1.0.1/PKG-INFO` & `timering-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: timering
-Version: 1.0.1
+Version: 1.0.2
 Summary: The only timing library you'll ever need.
-Home-page: https://github.com/ruzickbelle/python-timing
 Author: ruzickbelle
 License: BSD 3-Clause License
         
         Copyright (c) 2023, ruzickbelle
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -28,26 +27,30 @@
         DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+Project-URL: Repository, https://github.com/ruzickbelle/python-timing
+Project-URL: Changelog, https://github.com/ruzickbelle/python-timing/blob/main/CHANGELOG.md
 Keywords: timer,timing
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: build
 License-File: LICENSE
 
 # timing
 **timing** is a Python timing library providing timer functionality.
 
 This library is one of many providing timers, but aims to:
 * incorporate all patterns for timing execution times
@@ -88,14 +91,17 @@
 ```bash
 $ python -m pip install timering
 ```
 
 Note that on some systems, the Python 3 executable is called `python3` instead.
 
 
+## [Release Notes](https://github.com/ruzickbelle/python-timing/blob/main/CHANGELOG.md)
+
+
 ## Supported Patterns
 
 ### Start and Stop
 
 Create a timer, start and stop it:
 
 ```python
```

### Comparing `timering-1.0.1/README.md` & `timering-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,17 @@
 ```bash
 $ python -m pip install timering
 ```
 
 Note that on some systems, the Python 3 executable is called `python3` instead.
 
 
+## [Release Notes](https://github.com/ruzickbelle/python-timing/blob/main/CHANGELOG.md)
+
+
 ## Supported Patterns
 
 ### Start and Stop
 
 Create a timer, start and stop it:
 
 ```python
```

### Comparing `timering-1.0.1/src/timering.egg-info/PKG-INFO` & `timering-1.0.2/src/timering.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: timering
-Version: 1.0.1
+Version: 1.0.2
 Summary: The only timing library you'll ever need.
-Home-page: https://github.com/ruzickbelle/python-timing
 Author: ruzickbelle
 License: BSD 3-Clause License
         
         Copyright (c) 2023, ruzickbelle
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -28,26 +27,30 @@
         DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+Project-URL: Repository, https://github.com/ruzickbelle/python-timing
+Project-URL: Changelog, https://github.com/ruzickbelle/python-timing/blob/main/CHANGELOG.md
 Keywords: timer,timing
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: build
 License-File: LICENSE
 
 # timing
 **timing** is a Python timing library providing timer functionality.
 
 This library is one of many providing timers, but aims to:
 * incorporate all patterns for timing execution times
@@ -88,14 +91,17 @@
 ```bash
 $ python -m pip install timering
 ```
 
 Note that on some systems, the Python 3 executable is called `python3` instead.
 
 
+## [Release Notes](https://github.com/ruzickbelle/python-timing/blob/main/CHANGELOG.md)
+
+
 ## Supported Patterns
 
 ### Start and Stop
 
 Create a timer, start and stop it:
 
 ```python
```

### Comparing `timering-1.0.1/src/timing/timing.py` & `timering-1.0.2/src/timing/timing.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 # -*- coding: utf-8 -*-
 
 """
-Yet another timing library. It aims to support every timing pattern:
-* Functions:    start() / stop() / measure(fn: Callable)
-* Decorators:   wrap(fn: Callable) / @wrap
-* Contexts:     with Timer() as timer: pass
-
-For repeated performance measurements (microbenchmarks), use the builtin `timeit` library.
+Classes and types for the timing library.
 """
 
 import typing
 import time
 
 TimerUnit = typing.Literal["seconds", "milliseconds", "microseconds", "nanoseconds"]
 TimerResult = typing.Union[int, float]
 TimerCallback = typing.Callable[[TimerResult], None]
 
-prevtimer = None
-
 
 class TimerStateError(Exception):
     """ Raised if the operation is not permitted in the current timer state. """
     __slots__ = ()
 
 
 class Timer:
@@ -149,35 +142,41 @@
         """ Calls `start()` and returns `self`. """
         self.start()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb) -> bool:
         """
         Calls `stop()`.
-        If an exception occurred in the context, the callback will not be called, but the timer will be stopped anyway.
+        If an exception was raised in the context, the callback will not be called, but the timer will be stopped anyway.
         """
-        callback = not bool(exc_type)  # don't call the callback if an exception occurred
+        callback = not bool(exc_type)  # don't call the callback if an exception was raised
         self.stop(callback=callback)
         return False  # don't suppress the exception
 
     def measure(self, fn: typing.Callable, unit: typing.Optional[TimerUnit] = None, callback: typing.Union[bool, TimerCallback] = True) -> typing.Any:
         """
         Times the Callable `fn` using this timer.
         * Returns the result of the Callable `fn`.
         * See `get()` for help of the `unit` argument.
         * Calls the given callback with the timer result:
             * If `callback is True`, `self.callback` will be used.
             * If `callback is False`, no callback will be called.
             * Otherwise the argument is called.
+            * If the Callable `fn` raises an exception, no callback will be stopped, but the timer will be stopped anyway.
         * Raises `TimerStateError` if the timer is already running.
         * Raises `ValueError` if the unit is not supported.
         """
         self.start()
-        ret = fn()
-        self.stop(unit=unit, callback=callback)
+        try:
+            ret = fn()
+        except:
+            self.stop(callback=False)
+            raise
+        else:
+            self.stop(unit=unit, callback=callback)
         return ret
 
     def wrap(self, fn: typing.Optional[typing.Callable] = None, **kwargs) -> typing.Callable:
         """
         Implements the decorator pattern for the `measure()` method:
         * Decorator:             wrap(fn: Callable, **kwargs) / @wrap
         * Decorator Generator:   wrap(**kwargs)(fn: Callable) / @wrap(**kwargs)
@@ -188,55 +187,7 @@
             return timed
         else:
             def decorator(fn: typing.Callable):
                 def timed():
                     return self.measure(fn, **kwargs)
                 return timed
             return decorator
-
-
-def start(*args, **kwargs) -> Timer:
-    """
-    Creates a new `Timer`, starts and returns it.
-    * All arguments are passed to the `Timer` constructor.
-    * The created `Timer` may also be found in the module attribute `prevtimer`.
-    """
-    global prevtimer
-    timer = Timer(*args, **kwargs)
-    prevtimer = timer
-    timer.start()
-    return timer
-
-
-def measure(fn: typing.Callable, **kwargs) -> typing.Any:
-    """
-    Creates a new `Timer`, times the Callable `fn` and returns the result.
-    * All keyword arguments are passed to the `Timer` constructor.
-    * The created `Timer` may also be found in the module attribute `prevtimer`.
-    """
-    global prevtimer
-    timer = Timer(**kwargs)
-    prevtimer = timer
-    return timer.measure(fn)
-
-
-def wrap(fn: typing.Optional[typing.Callable] = None, **kwargs) -> typing.Callable:
-    """
-    Creates a new `Timer`, wraps the Callable `fn` and returns the wrapped callable.
-    * Decorator:             wrap(fn: Callable, **kwargs) / @wrap
-    * Decorator Generator:   wrap(**kwargs)(fn: Callable) / @wrap(**kwargs)
-    * All keyword arguments are passed to the `Timer` constructor.
-    * The created `Timer` may also be found in the module attribute `prevtimer`, directly after wrapping.
-    """
-    global prevtimer
-    timer = Timer(**kwargs)
-    prevtimer = timer
-    if fn:
-        def timed():
-            return timer.measure(fn)
-        return timed
-    else:
-        def decorator(fn: typing.Callable):
-            def timed():
-                return timer.measure(fn)
-            return timed
-        return decorator
```

### Comparing `timering-1.0.1/tests/test_functions.py` & `timering-1.0.2/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `timering-1.0.1/tests/test_methods.py` & `timering-1.0.2/tests/test_methods.py`

 * *Files identical despite different names*

