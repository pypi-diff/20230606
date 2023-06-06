# Comparing `tmp/pnwkit-py-2.6.8.tar.gz` & `tmp/pnwkit-py-2.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pnwkit-py-2.6.8.tar", last modified: Thu Jan 12 23:21:36 2023, max compression
+gzip compressed data, was "pnwkit-py-2.6.9.tar", last modified: Thu Jan 12 23:53:12 2023, max compression
```

## Comparing `pnwkit-py-2.6.8.tar` & `pnwkit-py-2.6.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:21:36.025232 pnwkit-py-2.6.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-01-12 23:21:25.000000 pnwkit-py-2.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-01-12 23:21:36.025232 pnwkit-py-2.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-01-12 23:21:25.000000 pnwkit-py-2.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:21:36.021232 pnwkit-py-2.6.8/pnwkit/
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-01-12 23:21:25.000000 pnwkit-py-2.6.8/pnwkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20764 2023-01-12 23:21:25.000000 pnwkit-py-2.6.8/pnwkit/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21779 2023-01-12 23:21:25.000000 pnwkit-py-2.6.8/pnwkit/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-01-12 23:21:25.000000 pnwkit-py-2.6.8/pnwkit/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:21:36.017232 pnwkit-py-2.6.8/pnwkit/ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:21:36.021232 pnwkit-py-2.6.8/pnwkit/ext/dumps/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-01-12 23:21:25.000000 pnwkit-py-2.6.8/pnwkit/ext/dumps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-01-12 23:21:25.000000 pnwkit-py-2.6.8/pnwkit/ext/dumps/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-01-12 23:21:25.000000 pnwkit-py-2.6.8/pnwkit/ext/dumps/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-01-12 23:21:25.000000 pnwkit-py-2.6.8/pnwkit/ext/dumps/async_.py
--rw-r--r--   0 runner    (1001) docker     (123)    24963 2023-01-12 23:21:25.000000 pnwkit-py-2.6.8/pnwkit/ext/dumps/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-01-12 23:21:25.000000 pnwkit-py-2.6.8/pnwkit/ext/dumps/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:21:36.021232 pnwkit-py-2.6.8/pnwkit/ext/scrape/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-12 23:21:25.000000 pnwkit-py-2.6.8/pnwkit/ext/scrape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-01-12 23:21:25.000000 pnwkit-py-2.6.8/pnwkit/ext/scrape/async_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-01-12 23:21:25.000000 pnwkit-py-2.6.8/pnwkit/ext/scrape/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:21:36.025232 pnwkit-py-2.6.8/pnwkit/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)    20812 2023-01-12 23:21:25.000000 pnwkit-py-2.6.8/pnwkit/legacy/async_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33144 2023-01-12 23:21:25.000000 pnwkit-py-2.6.8/pnwkit/legacy/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-01-12 23:21:25.000000 pnwkit-py-2.6.8/pnwkit/legacy/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    51408 2023-01-12 23:21:25.000000 pnwkit-py-2.6.8/pnwkit/legacy/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-01-12 23:21:25.000000 pnwkit-py-2.6.8/pnwkit/legacy/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-01-12 23:21:25.000000 pnwkit-py-2.6.8/pnwkit/legacy/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19857 2023-01-12 23:21:25.000000 pnwkit-py-2.6.8/pnwkit/legacy/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    59892 2023-01-12 23:21:25.000000 pnwkit-py-2.6.8/pnwkit/new.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 23:21:25.000000 pnwkit-py-2.6.8/pnwkit/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-01-12 23:21:25.000000 pnwkit-py-2.6.8/pnwkit/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-01-12 23:21:25.000000 pnwkit-py-2.6.8/pnwkit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:21:36.025232 pnwkit-py-2.6.8/pnwkit_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-01-12 23:21:36.000000 pnwkit-py-2.6.8/pnwkit_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-01-12 23:21:36.000000 pnwkit-py-2.6.8/pnwkit_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 23:21:36.000000 pnwkit-py-2.6.8/pnwkit_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-01-12 23:21:36.000000 pnwkit-py-2.6.8/pnwkit_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-12 23:21:36.000000 pnwkit-py-2.6.8/pnwkit_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-01-12 23:21:25.000000 pnwkit-py-2.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 23:21:36.025232 pnwkit-py-2.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-01-12 23:21:25.000000 pnwkit-py-2.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:53:12.858015 pnwkit-py-2.6.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-01-12 23:52:57.000000 pnwkit-py-2.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-01-12 23:53:12.854014 pnwkit-py-2.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-01-12 23:52:57.000000 pnwkit-py-2.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:53:12.854014 pnwkit-py-2.6.9/pnwkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-01-12 23:52:57.000000 pnwkit-py-2.6.9/pnwkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20764 2023-01-12 23:52:57.000000 pnwkit-py-2.6.9/pnwkit/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21836 2023-01-12 23:52:57.000000 pnwkit-py-2.6.9/pnwkit/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-01-12 23:52:57.000000 pnwkit-py-2.6.9/pnwkit/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:53:12.850015 pnwkit-py-2.6.9/pnwkit/ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:53:12.854014 pnwkit-py-2.6.9/pnwkit/ext/dumps/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-01-12 23:52:57.000000 pnwkit-py-2.6.9/pnwkit/ext/dumps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-01-12 23:52:57.000000 pnwkit-py-2.6.9/pnwkit/ext/dumps/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-01-12 23:52:57.000000 pnwkit-py-2.6.9/pnwkit/ext/dumps/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-01-12 23:52:57.000000 pnwkit-py-2.6.9/pnwkit/ext/dumps/async_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24963 2023-01-12 23:52:57.000000 pnwkit-py-2.6.9/pnwkit/ext/dumps/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-01-12 23:52:57.000000 pnwkit-py-2.6.9/pnwkit/ext/dumps/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:53:12.854014 pnwkit-py-2.6.9/pnwkit/ext/scrape/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-12 23:52:57.000000 pnwkit-py-2.6.9/pnwkit/ext/scrape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-01-12 23:52:57.000000 pnwkit-py-2.6.9/pnwkit/ext/scrape/async_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-01-12 23:52:57.000000 pnwkit-py-2.6.9/pnwkit/ext/scrape/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:53:12.854014 pnwkit-py-2.6.9/pnwkit/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)    20812 2023-01-12 23:52:57.000000 pnwkit-py-2.6.9/pnwkit/legacy/async_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33144 2023-01-12 23:52:57.000000 pnwkit-py-2.6.9/pnwkit/legacy/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-01-12 23:52:57.000000 pnwkit-py-2.6.9/pnwkit/legacy/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51408 2023-01-12 23:52:57.000000 pnwkit-py-2.6.9/pnwkit/legacy/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-01-12 23:52:57.000000 pnwkit-py-2.6.9/pnwkit/legacy/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-01-12 23:52:57.000000 pnwkit-py-2.6.9/pnwkit/legacy/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19857 2023-01-12 23:52:57.000000 pnwkit-py-2.6.9/pnwkit/legacy/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60106 2023-01-12 23:52:57.000000 pnwkit-py-2.6.9/pnwkit/new.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 23:52:57.000000 pnwkit-py-2.6.9/pnwkit/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-01-12 23:52:57.000000 pnwkit-py-2.6.9/pnwkit/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-01-12 23:52:57.000000 pnwkit-py-2.6.9/pnwkit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:53:12.854014 pnwkit-py-2.6.9/pnwkit_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-01-12 23:53:12.000000 pnwkit-py-2.6.9/pnwkit_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-01-12 23:53:12.000000 pnwkit-py-2.6.9/pnwkit_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 23:53:12.000000 pnwkit-py-2.6.9/pnwkit_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-01-12 23:53:12.000000 pnwkit-py-2.6.9/pnwkit_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-12 23:53:12.000000 pnwkit-py-2.6.9/pnwkit_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-01-12 23:52:57.000000 pnwkit-py-2.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 23:53:12.858015 pnwkit-py-2.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-01-12 23:52:57.000000 pnwkit-py-2.6.9/setup.py
```

### Comparing `pnwkit-py-2.6.8/LICENSE` & `pnwkit-py-2.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pnwkit-py-2.6.8/PKG-INFO` & `pnwkit-py-2.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnwkit-py
-Version: 2.6.8
+Version: 2.6.9
 Summary: A Python wrapper for the Politics and War API.
 Home-page: https://github.com/Village05/pnwkit-py
 Author: Village
 License: MIT
 Project-URL: Documentation, https://pnwkit-py.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/Village05/pnwkit-py/issues
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pnwkit-py Version: 2.6.8 Summary: A Python wrapper
+Metadata-Version: 2.1 Name: pnwkit-py Version: 2.6.9 Summary: A Python wrapper
 for the Politics and War API. Home-page: https://github.com/Village05/pnwkit-py
 Author: Village License: MIT Project-URL: Documentation, https://pnwkit-
 py.readthedocs.io/en/latest/ Project-URL: Issue tracker, https://github.com/
 Village05/pnwkit-py/issues Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: OSI Approved :: MIT License Classifier: Intended
 Audience :: Developers Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

### Comparing `pnwkit-py-2.6.8/README.md` & `pnwkit-py-2.6.9/README.md`

 * *Files identical despite different names*

### Comparing `pnwkit-py-2.6.8/pnwkit/__init__.py` & `pnwkit-py-2.6.9/pnwkit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from typing import TextIO
 
 from .data import *
 from .legacy.core import Kit, async_pnwkit, pnwkit  # type: ignore
 from .legacy.keys import set_bot_key, set_key  # type: ignore
 from .new import *
 
-__version__ = "2.6.8"
+__version__ = "2.6.9"
 
 # Set default logging handler to avoid "No handler found" warnings.
 logging.getLogger(__name__).addHandler(NullHandler())
 
 
 def add_stderr_logger(level: int = logging.DEBUG) -> logging.StreamHandler[TextIO]:
     """
```

### Comparing `pnwkit-py-2.6.8/pnwkit/__init__.pyi` & `pnwkit-py-2.6.9/pnwkit/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pnwkit-py-2.6.8/pnwkit/data.py` & `pnwkit-py-2.6.9/pnwkit/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,23 +60,25 @@
     "Trade",
     "TreasureTrade",
     "Embargo",
     "PaginatorInfo",
 )
 
 if TYPE_CHECKING:
-    from typing import Any, Callable, ClassVar, Dict, List, Optional
+    from typing import Any, Callable, ClassVar, Dict, List, Optional, Type, TypeVar
+
+    T = TypeVar("T", bound="Data")
 
 
 class Data:
     _CONVERTERS: ClassVar[Dict[str, Callable[[Any], Any]]] = {}
     __slots__ = ("__dict__",)
 
     @classmethod
-    def from_data(cls, data: Dict[str, Any]) -> Data:
+    def from_data(cls: Type[T], data: Dict[str, Any]) -> T:
         self = cls()
         for key, value in data.items():
             if key == "global":
                 key = "global_"
             if isinstance(value, dict):
                 # value is Unknown
                 value = utils.convert_data_dict(value)  # type: ignore
```

### Comparing `pnwkit-py-2.6.8/pnwkit/errors.py` & `pnwkit-py-2.6.9/pnwkit/errors.py`

 * *Files identical despite different names*

### Comparing `pnwkit-py-2.6.8/pnwkit/ext/dumps/__init__.py` & `pnwkit-py-2.6.9/pnwkit/ext/dumps/__init__.py`

 * *Files identical despite different names*

### Comparing `pnwkit-py-2.6.8/pnwkit/ext/dumps/__init__.pyi` & `pnwkit-py-2.6.9/pnwkit/ext/dumps/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pnwkit-py-2.6.8/pnwkit/ext/dumps/abc.py` & `pnwkit-py-2.6.9/pnwkit/ext/dumps/abc.py`

 * *Files identical despite different names*

### Comparing `pnwkit-py-2.6.8/pnwkit/ext/dumps/async_.py` & `pnwkit-py-2.6.9/pnwkit/ext/dumps/async_.py`

 * *Files identical despite different names*

### Comparing `pnwkit-py-2.6.8/pnwkit/ext/dumps/data.py` & `pnwkit-py-2.6.9/pnwkit/ext/dumps/data.py`

 * *Files identical despite different names*

### Comparing `pnwkit-py-2.6.8/pnwkit/ext/dumps/sync.py` & `pnwkit-py-2.6.9/pnwkit/ext/dumps/sync.py`

 * *Files identical despite different names*

### Comparing `pnwkit-py-2.6.8/pnwkit/ext/scrape/async_.py` & `pnwkit-py-2.6.9/pnwkit/ext/scrape/async_.py`

 * *Files identical despite different names*

### Comparing `pnwkit-py-2.6.8/pnwkit/ext/scrape/sync.py` & `pnwkit-py-2.6.9/pnwkit/ext/scrape/sync.py`

 * *Files identical despite different names*

### Comparing `pnwkit-py-2.6.8/pnwkit/legacy/async_.py` & `pnwkit-py-2.6.9/pnwkit/legacy/async_.py`

 * *Files identical despite different names*

### Comparing `pnwkit-py-2.6.8/pnwkit/legacy/base.py` & `pnwkit-py-2.6.9/pnwkit/legacy/base.py`

 * *Files identical despite different names*

### Comparing `pnwkit-py-2.6.8/pnwkit/legacy/core.py` & `pnwkit-py-2.6.9/pnwkit/legacy/core.py`

 * *Files identical despite different names*

### Comparing `pnwkit-py-2.6.8/pnwkit/legacy/data.py` & `pnwkit-py-2.6.9/pnwkit/legacy/data.py`

 * *Files identical despite different names*

### Comparing `pnwkit-py-2.6.8/pnwkit/legacy/keys.py` & `pnwkit-py-2.6.9/pnwkit/legacy/keys.py`

 * *Files identical despite different names*

### Comparing `pnwkit-py-2.6.8/pnwkit/legacy/paginator.py` & `pnwkit-py-2.6.9/pnwkit/legacy/paginator.py`

 * *Files identical despite different names*

### Comparing `pnwkit-py-2.6.8/pnwkit/legacy/sync.py` & `pnwkit-py-2.6.9/pnwkit/legacy/sync.py`

 * *Files identical despite different names*

### Comparing `pnwkit-py-2.6.8/pnwkit/new.py` & `pnwkit-py-2.6.9/pnwkit/new.py`

 * *Files 0% similar despite different names*

```diff
@@ -1574,15 +1574,15 @@
                 # sleeps until next ping
                 await asyncio.sleep(
                     self.last_message + self.activity_timeout - time.perf_counter()
                 )
                 # if received a message within activity timeout, continue to next iteration since we do not need to ping
                 if self.last_message + self.activity_timeout > time.perf_counter():
                     continue
-                if self.last_ping > self.last_pong:
+                if self.last_ping + self.activity_timeout > self.last_pong:
                     # if pinged, not received pong, passed timeout, close and reconnect
                     if self.last_ping + self.activity_timeout > time.perf_counter():
                         logger.debug("ping_pong - Pong timeout")
                         # has pinged, has not received pong, and has not received any other messages in activity_timeout
                         # therefore, connection is dead and should be closed and reconnected
                         await self.close_and_reconnect()
                         await asyncio.sleep(self.activity_timeout)
@@ -1603,24 +1603,28 @@
 
     def run(self) -> None:
         self.task = asyncio.create_task(self.actual_run())
         self.ping_pong_task = asyncio.create_task(self.ping_pong())
 
     async def authorize_subscription(self, subscription: Subscription[Any]) -> str:
         if not self.established.is_set():
-            logger.debug("authorize_subscription - Waiting for connection to be spcket")
+            logger.debug(
+                "authorize_subscription - Waiting for connection to be established"
+            )
         await self.established.wait()
+        logger.debug("authorized_subscription - connection is established")
         if self.kit.aiohttp_session is None:
             logger.debug("authorize_subscription - Creating aiohttp session")
             self.kit.aiohttp_session = aiohttp.ClientSession()
         async with self.kit.aiohttp_session.request(
             "POST",
             self.kit.subscription_auth_url,
             data={"socket_id": self.socket_id, "channel_name": subscription.channel},
         ) as response:
+            logger.debug("authorize_subscription - Got response %s", response)
             if response.status != 200:
                 raise errors.Unauthorized()
             data = await response.json()
             self.kit.check_response_for_errors(data)
             return data["auth"]
         raise errors.SubscribeError(
             f"Failed to authorize subscription to {subscription.channel}"
```

### Comparing `pnwkit-py-2.6.8/pnwkit/ratelimit.py` & `pnwkit-py-2.6.9/pnwkit/ratelimit.py`

 * *Files identical despite different names*

### Comparing `pnwkit-py-2.6.8/pnwkit/utils.py` & `pnwkit-py-2.6.9/pnwkit/utils.py`

 * *Files identical despite different names*

### Comparing `pnwkit-py-2.6.8/pnwkit_py.egg-info/PKG-INFO` & `pnwkit-py-2.6.9/pnwkit_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnwkit-py
-Version: 2.6.8
+Version: 2.6.9
 Summary: A Python wrapper for the Politics and War API.
 Home-page: https://github.com/Village05/pnwkit-py
 Author: Village
 License: MIT
 Project-URL: Documentation, https://pnwkit-py.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/Village05/pnwkit-py/issues
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pnwkit-py Version: 2.6.8 Summary: A Python wrapper
+Metadata-Version: 2.1 Name: pnwkit-py Version: 2.6.9 Summary: A Python wrapper
 for the Politics and War API. Home-page: https://github.com/Village05/pnwkit-py
 Author: Village License: MIT Project-URL: Documentation, https://pnwkit-
 py.readthedocs.io/en/latest/ Project-URL: Issue tracker, https://github.com/
 Village05/pnwkit-py/issues Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: OSI Approved :: MIT License Classifier: Intended
 Audience :: Developers Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

### Comparing `pnwkit-py-2.6.8/pnwkit_py.egg-info/SOURCES.txt` & `pnwkit-py-2.6.9/pnwkit_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pnwkit-py-2.6.8/setup.py` & `pnwkit-py-2.6.9/setup.py`

 * *Files identical despite different names*

