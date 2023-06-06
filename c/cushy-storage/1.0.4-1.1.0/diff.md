# Comparing `tmp/cushy-storage-1.0.4.tar.gz` & `tmp/cushy-storage-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/cushy-storage/cushy-storage/dist/.tmp-pwlr5tu9/cushy-storage-1.0.4.tar", last modified: Sun Jun  4 15:18:19 2023, max compression
+gzip compressed data, was "/home/runner/work/cushy-storage/cushy-storage/dist/.tmp-5170kyh4/cushy-storage-1.1.0.tar", last modified: Tue Jun  6 08:52:38 2023, max compression
```

## Comparing `cushy-storage-1.0.4.tar` & `cushy-storage-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:18:19.000000 cushy-storage-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-04 15:18:08.000000 cushy-storage-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-06-04 15:18:19.000000 cushy-storage-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-06-04 15:18:08.000000 cushy-storage-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:18:19.000000 cushy-storage-1.0.4/cushy_storage/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-04 15:18:08.000000 cushy-storage-1.0.4/cushy_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-06-04 15:18:08.000000 cushy-storage-1.0.4/cushy_storage/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-04 15:18:08.000000 cushy-storage-1.0.4/cushy_storage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:18:19.000000 cushy-storage-1.0.4/cushy_storage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-06-04 15:18:19.000000 cushy-storage-1.0.4/cushy_storage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-04 15:18:19.000000 cushy-storage-1.0.4/cushy_storage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 15:18:19.000000 cushy-storage-1.0.4/cushy_storage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-04 15:18:19.000000 cushy-storage-1.0.4/cushy_storage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 15:18:19.000000 cushy-storage-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-04 15:18:08.000000 cushy-storage-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:18:19.000000 cushy-storage-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-04 15:18:08.000000 cushy-storage-1.0.4/tests/test_base_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-04 15:18:08.000000 cushy-storage-1.0.4/tests/test_cushy_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-04 15:18:08.000000 cushy-storage-1.0.4/tests/test_dict_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:52:38.000000 cushy-storage-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 08:52:20.000000 cushy-storage-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-06-06 08:52:38.000000 cushy-storage-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10175 2023-06-06 08:52:20.000000 cushy-storage-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:52:38.000000 cushy-storage-1.1.0/cushy_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-06 08:52:20.000000 cushy-storage-1.1.0/cushy_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-06-06 08:52:20.000000 cushy-storage-1.1.0/cushy_storage/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-06 08:52:20.000000 cushy-storage-1.1.0/cushy_storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-06 08:52:20.000000 cushy-storage-1.1.0/cushy_storage/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-06-06 08:52:20.000000 cushy-storage-1.1.0/cushy_storage/orm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-06 08:52:20.000000 cushy-storage-1.1.0/cushy_storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:52:38.000000 cushy-storage-1.1.0/cushy_storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-06-06 08:52:38.000000 cushy-storage-1.1.0/cushy_storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-06 08:52:38.000000 cushy-storage-1.1.0/cushy_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 08:52:38.000000 cushy-storage-1.1.0/cushy_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-06 08:52:38.000000 cushy-storage-1.1.0/cushy_storage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 08:52:38.000000 cushy-storage-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-06 08:52:20.000000 cushy-storage-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:52:38.000000 cushy-storage-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-06 08:52:20.000000 cushy-storage-1.1.0/tests/test_base_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-06 08:52:20.000000 cushy-storage-1.1.0/tests/test_cushy_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-06 08:52:20.000000 cushy-storage-1.1.0/tests/test_dict_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-06-06 08:52:20.000000 cushy-storage-1.1.0/tests/test_orm.py
```

### Comparing `cushy-storage-1.0.4/LICENSE` & `cushy-storage-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.0.4/cushy_storage/_core.py` & `cushy-storage-1.1.0/cushy_storage/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 import json
 import pickle
 import hashlib
 import threading
 from pathlib import Path
 from typing import MutableMapping, Callable, Tuple, Union, Any, List
 
-from cushy_storage.base import _List, BASE_TYPE
-from cushy_storage.utils import get_default_storage_path
+from cushy_storage.base import EnhancedList, BASE_TYPE
+from cushy_storage.utils import get_default_cache_path
 
 __all__ = ['BaseDict', 'CushyDict', 'disk_cache']
 
 # Compression algorithms and their corresponding functions
 _COMPRESS = {
     'zlib': (
         zlib.compress,
@@ -148,32 +148,32 @@
 class CushyDict(BaseDict):
     """
     A subclass of BaseDict that can serialize and deserialize values using different algorithms
     """
 
     def __init__(
             self,
-            path: str = get_default_storage_path(),
+            path: str = get_default_cache_path(),
             compress: Union[str, Tuple[Callable, Callable], None] = None,
             serialize: Union[str, Tuple[Callable, Callable], None] = 'json'
     ):
         """
         Args:
             path: the path to save
             compress: zlib or lzma
             serialize: json or pickle
         """
         super().__init__(path, compress)
         self.serialize, self.deserialize = _method_convert_helper(serialize, _SERIALIZATION)
 
-    def __getitem__(self, k: str):
+    def __getitem__(self, k: str) -> Any:
         ret = self.deserialize(super().__getitem__(k))
 
         if isinstance(ret, list):
-            ret: List = _List(ret)
+            ret: List = EnhancedList(ret)
         return ret
 
     def __setitem__(self, k: str, v: Any):
         if isinstance(v, list) and self.deserialize is json.loads and len(v) > 0 and type(v[0]) not in BASE_TYPE:
             raise ValueError((
                 f"Can not use 'json' to serialize your '{type(v[0])}' data in '{k}'. If you want to store "
                 "complex data or custom data, please use 'pickle' to serialize."
```

### Comparing `cushy-storage-1.0.4/cushy_storage/utils.py` & `cushy-storage-1.1.0/cushy_storage/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,16 +31,24 @@
         project_path = os.path.split(project_path)[0]
         count += 1
         if count > max_depth:
             return os.getcwd()
     return project_path
 
 
-def get_default_storage_path() -> str:
+def get_default_storage_path(file_name) -> str:
     if platform.system() == 'Windows':
-        return f"./cache"
+        return f"./{file_name}"
     elif platform.system() == 'Linux':
         dir_path = os.environ.get('TMPDIR')
         if not dir_path:
             dir_path = tempfile.gettempdir()
         dir_path = os.path.join(dir_path, "prompt_me")
-        return f"{dir_path}/cache"
+        return f"{dir_path}/{file_name}"
+
+
+def get_default_cache_path() -> str:
+    return get_default_storage_path("cache")
+
+
+def get_default_log_path() -> str:
+    return get_default_storage_path("log")
```

### Comparing `cushy-storage-1.0.4/setup.py` & `cushy-storage-1.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="cushy-storage",
-    version="1.0.4",
+    version="1.1.0",
     author="Zeeland",
     author_email="zeeland@foxmail.com",
     description="A data local persistence framework library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Undertone0809/cushy-storage",
     packages=setuptools.find_packages(),
```

### Comparing `cushy-storage-1.0.4/tests/test_base_dict.py` & `cushy-storage-1.1.0/tests/test_base_dict.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,42 +14,33 @@
 #
 # Copyright Owner: Zeeland
 # GitHub Link: https://github.com/Undertone0809/
 # Project Link: https://github.com/Undertone0809/cushy-storage
 # Contact Email: zeeland@foxmail.com
 
 import unittest
-from cushy_storage import CushyDict
+from cushy_storage import BaseDict
 
 
 class TestBaseDict(unittest.TestCase):
     def test_basic_operations(self):
-        cache = CushyDict('./test-cache')
+        cache = BaseDict('./cache/test-base-dict')
 
         # Test adding items to the cache
         cache['foo'] = b'bar'
         self.assertEqual(cache['foo'], b'bar')
 
         # Test deleting items from the cache
         del cache['foo']
         with self.assertRaises(KeyError):
             cache['foo']
 
         # Test checking if an item is in the cache
         self.assertFalse('foo' in cache)
 
-    def test_serialization(self):
-        cache = CushyDict('./test-cache', serialize='pickle')
-
-        # Test storing and retrieving a dictionary in the cache using pickle serialization
-        cache['data'] = {'foo': 'bar', 'baz': [1, 2, 3]}
-        self.assertEqual(cache['data'], {'foo': 'bar', 'baz': [1, 2, 3]})
-
     def test_compression(self):
-        cache = CushyDict('./test-cache', compress='lzma')
+        cache = BaseDict('./cache/test-base-dict', compress='lzma')
 
         # Test storing and retrieving a large string in the cache using LZMA compression
         data = 'a' * (1024 * 1024)
         cache['big_data'] = data.encode()
         self.assertEqual(cache['big_data'].decode(), data)
-
-
```

### Comparing `cushy-storage-1.0.4/tests/test_cushy_dict.py` & `cushy-storage-1.1.0/tests/test_cushy_dict.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,19 +15,20 @@
 # Copyright Owner: Zeeland
 # GitHub Link: https://github.com/Undertone0809/
 # Project Link: https://github.com/Undertone0809/cushy-storage
 # Contact Email: zeeland@foxmail.com
 
 import unittest
 from cushy_storage import CushyDict
+from cushy_storage.base import EnhancedList
 
 
 class TestCushyDict(unittest.TestCase):
     def test_read_and_write_data(self):
-        cache = CushyDict("./test-cache")
+        cache = CushyDict("./cache/test-cushy-dict")
         cache['a'] = 10
         self.assertEqual(cache['a'], 10)
 
         cache['b'] = "test"
         self.assertEqual(cache['b'], "test")
 
         cache['c'] = [1, 2, 3, 4]
@@ -37,14 +38,14 @@
         self.assertEqual(cache['d'], {"key": "value"})
 
         cache['e'] = ("hello", 1)
         print(type(cache['e']))
         self.assertEqual(cache['e'], ["hello", 1])
 
     def test_data_type(self):
-        cache = CushyDict("./test-cache")
+        cache = CushyDict("./cache/test-cushy-dict")
         self.assertEqual(type(cache['a']), int)
         self.assertEqual(type(cache['b']), str)
-        self.assertEqual(type(cache['c']), list)
+        self.assertEqual(type(cache['c']), EnhancedList)
         self.assertEqual(type(cache['d']), dict)
         # todo https://github.com/Undertone0809/cushy-stroage/issues/1
-        self.assertEqual(type(cache['e']), list)
+        self.assertEqual(type(cache['e']), EnhancedList)
```

### Comparing `cushy-storage-1.0.4/tests/test_dict_cache.py` & `cushy-storage-1.1.0/tests/test_dict_cache.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,37 +20,37 @@
 import time
 import unittest
 from cushy_storage import CushyDict, disk_cache
 
 
 class TestDiskCache(unittest.TestCase):
     def test_basic_usage(self):
-        @disk_cache('./test-disk-cache')
+        @disk_cache('./cache/test-disk-cache')
         def slow_function(x):
             time.sleep(0.1)
             return x + 1
 
         # Test calling the function with different arguments and caching the output
         self.assertEqual(slow_function(5), 6)
         self.assertEqual(slow_function(5), 6)  # Should use cache this time
         self.assertEqual(slow_function(10), 11)
 
     def test_serialization(self):
-        @disk_cache('./test-disk-cache-serialize', serialize='pickle')
+        @disk_cache('./cache/test-disk-cache-serialize', serialize='pickle')
         def slow_function(x):
             time.sleep(0.1)
             return {'result': x}
 
         # Test caching the output of a function that returns a dictionary using pickle serialization
         self.assertEqual(slow_function(5), {'result': 5})
         self.assertEqual(slow_function(5), {'result': 5})  # Should use cache this time
         self.assertEqual(slow_function(10), {'result': 10})
 
     def test_compression(self):
-        @disk_cache('./test-disk-cache-compress', compress='lzma')
+        @disk_cache('./cache/test-disk-cache-compress', compress='lzma')
         def slow_function(x):
             time.sleep(0.1)
             return 'a' * (1024 * 1024)
 
         # Test caching the output of a function that returns a large string using LZMA compression
         self.assertEqual(slow_function(5), 'a' * (1024 * 1024))
         self.assertEqual(slow_function(5), 'a' * (1024 * 1024))  # Should use cache this time
```

