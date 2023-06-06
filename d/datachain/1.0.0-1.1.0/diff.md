# Comparing `tmp/datachain-1.0.0.tar.gz` & `tmp/datachain-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datachain-1.0.0.tar", max compression
+gzip compressed data, was "datachain-1.1.0.tar", max compression
```

## Comparing `datachain-1.0.0.tar` & `datachain-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,39 @@
--rw-r--r--   0        0        0    35060 2023-03-26 22:49:34.715348 datachain-1.0.0/LICENSE
--rw-r--r--   0        0        0        0 2023-03-26 22:49:34.715403 datachain-1.0.0/README.md
--rw-r--r--   0        0        0      187 2023-03-27 10:55:56.699305 datachain-1.0.0/datachain/__init__.py
--rw-r--r--   0        0        0      120 2023-06-01 01:19:09.359858 datachain-1.0.0/datachain/config/__init__.py
--rw-r--r--   0        0        0     2629 2023-03-31 02:43:07.470280 datachain-1.0.0/datachain/config/logging.py
--rw-r--r--   0        0        0      748 2023-06-01 01:19:09.359983 datachain-1.0.0/datachain/config/params.py
--rw-r--r--   0        0        0       32 2023-03-26 22:49:34.715707 datachain-1.0.0/datachain/core/__init__.py
--rw-r--r--   0        0        0    17603 2023-06-01 01:19:09.360230 datachain-1.0.0/datachain/core/common.py
--rw-r--r--   0        0        0     3044 2023-03-27 10:29:58.237300 datachain-1.0.0/datachain/core/lazy.py
--rw-r--r--   0        0        0     2243 2023-03-31 01:27:20.943629 datachain-1.0.0/datachain/core/sync.py
--rw-r--r--   0        0        0       32 2023-03-26 22:49:34.716372 datachain-1.0.0/datachain/sources/__init__.py
--rw-r--r--   0        0        0      617 2023-03-28 17:59:32.602567 datachain-1.0.0/datachain/utils/func.py
--rw-r--r--   0        0        0      577 2023-06-01 01:19:59.948926 datachain-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      584 1970-01-01 00:00:00.000000 datachain-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35060 2023-05-23 08:21:28.841649 datachain-1.1.0/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-23 08:21:28.841716 datachain-1.1.0/README.md
+-rw-r--r--   0        0        0      187 2023-06-01 08:01:10.099643 datachain-1.1.0/datachain/__init__.py
+-rw-r--r--   0        0        0      120 2023-06-01 00:25:14.448453 datachain-1.1.0/datachain/config/__init__.py
+-rw-r--r--   0        0        0     2749 2023-06-06 13:28:01.504285 datachain-1.1.0/datachain/config/logging.py
+-rw-r--r--   0        0        0      752 2023-06-01 03:30:25.805131 datachain-1.1.0/datachain/config/params.py
+-rw-r--r--   0        0        0       32 2023-05-23 08:21:28.842314 datachain-1.1.0/datachain/core/__init__.py
+-rw-r--r--   0        0        0    18812 2023-06-06 10:07:49.632053 datachain-1.1.0/datachain/core/common.py
+-rw-r--r--   0        0        0     3044 2023-05-23 08:21:28.842591 datachain-1.1.0/datachain/core/lazy.py
+-rw-r--r--   0        0        0     2243 2023-05-23 08:21:28.842704 datachain-1.1.0/datachain/core/sync.py
+-rw-r--r--   0        0        0       32 2023-05-31 11:13:21.000000 datachain-1.1.0/datachain/sources/__init__.py
+-rw-r--r--   0        0        0     3919 2023-06-06 10:09:48.818894 datachain-1.1.0/datachain/sources/_utils.py
+-rw-r--r--   0        0        0       32 2023-05-31 14:27:33.000000 datachain-1.1.0/datachain/sources/bytes/__init__.py
+-rw-r--r--   0        0        0     1338 2023-06-06 08:42:46.052456 datachain-1.1.0/datachain/sources/bytes/_pandas.py
+-rw-r--r--   0        0        0      816 2023-06-06 08:22:54.813123 datachain-1.1.0/datachain/sources/file.py
+-rw-r--r--   0        0        0       32 2023-06-01 00:28:56.000000 datachain-1.1.0/datachain/sources/files/__init__.py
+-rw-r--r--   0        0        0     1038 2023-06-06 10:10:23.465279 datachain-1.1.0/datachain/sources/files/_file.py
+-rw-r--r--   0        0        0     1135 2023-06-06 10:15:30.554275 datachain-1.1.0/datachain/sources/files/_ftp.py
+-rw-r--r--   0        0        0      859 2023-06-06 08:39:33.394438 datachain-1.1.0/datachain/sources/files/_http.py
+-rw-r--r--   0        0        0      624 2023-06-06 08:22:54.828168 datachain-1.1.0/datachain/sources/files/_jsonfile.py
+-rw-r--r--   0        0        0      442 2023-03-31 02:13:33.000000 datachain-1.1.0/datachain/sources/files/_local.py
+-rw-r--r--   0        0        0     2825 2023-06-06 09:42:09.908877 datachain-1.1.0/datachain/sources/files/_pandas.py
+-rw-r--r--   0        0        0     1281 2023-06-06 08:45:42.480612 datachain-1.1.0/datachain/sources/files/_sftp.py
+-rw-r--r--   0        0        0     1232 2023-06-06 08:22:54.812738 datachain-1.1.0/datachain/sources/ftp.py
+-rw-r--r--   0        0        0     1847 2023-06-06 10:10:48.078320 datachain-1.1.0/datachain/sources/http.py
+-rw-r--r--   0        0        0       32 2023-05-31 12:23:56.000000 datachain-1.1.0/datachain/sources/query/__init__.py
+-rw-r--r--   0        0        0     3038 2023-06-06 08:44:39.844032 datachain-1.1.0/datachain/sources/query/_pandas.py
+-rw-r--r--   0        0        0     1348 2023-06-06 08:44:01.909822 datachain-1.1.0/datachain/sources/sftp.py
+-rw-r--r--   0        0        0     1969 2023-06-06 08:22:54.813000 datachain-1.1.0/datachain/sources/sharepoint.py
+-rw-r--r--   0        0        0     2473 2023-06-06 08:22:54.813016 datachain-1.1.0/datachain/sources/sql.py
+-rw-r--r--   0        0        0      353 2023-06-06 08:09:47.500631 datachain-1.1.0/datachain/sources/utils/__init__.py
+-rw-r--r--   0        0        0     2241 2023-06-06 08:12:04.292242 datachain-1.1.0/datachain/sources/utils/_column.py
+-rw-r--r--   0        0        0     4577 2023-06-06 08:12:39.732515 datachain-1.1.0/datachain/sources/utils/_dataframe.py
+-rw-r--r--   0        0        0      410 2023-02-06 12:21:00.337713 datachain-1.1.0/datachain/sources/utils/_func.py
+-rw-r--r--   0        0        0      567 2023-06-06 08:23:42.203847 datachain-1.1.0/datachain/sources/utils/utils.py
+-rw-r--r--   0        0        0      617 2023-05-23 08:21:28.842996 datachain-1.1.0/datachain/utils/func.py
+-rw-r--r--   0        0        0     2000 2023-06-06 13:42:59.895962 datachain-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 datachain-1.1.0/setup.py
+-rw-r--r--   0        0        0      817 1970-01-01 00:00:00.000000 datachain-1.1.0/PKG-INFO
```

### Comparing `datachain-1.0.0/LICENSE` & `datachain-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datachain-1.0.0/datachain/config/logging.py` & `datachain-1.1.0/datachain/config/logging.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 import functools
 
 from typing import Any
 
 
 class Logger:
     """Logger class."""
+    logger = None
+    console = False
+    paths = [] # type: list
 
     @classmethod
     def init_logger(cls) -> None:
         """Initializes a logger with the name 'datachain', removes any existing
         handlers, and sets the logging level to INFO.
         """
         cls.logger = logging.getLogger("datachain")
@@ -45,24 +48,26 @@
         formatter = logging.Formatter(
             fmt="%(asctime)s - %(name)s - %(levelname)s - %(message)s",
             datefmt="%a, %d %b %Y %H:%M:%S",
         )
         os.makedirs(path, exist_ok=True)
         file_handler = logging.FileHandler(os.path.join(path, "datachain.log"))
         file_handler.setFormatter(formatter)
-        cls.logger.addHandler(file_handler)
+        if cls.logger:
+            cls.logger.addHandler(file_handler)
         cls.paths.append(path)
 
     @classmethod
     def add_console(cls) -> None:
         """Initializes a console handler and adds it to the 'datachain' logger."""
         if cls.console:
             return
         console_handler = logging.StreamHandler()
-        cls.logger.addHandler(console_handler)
+        if cls.logger:
+            cls.logger.addHandler(console_handler)
         cls.console = True
 
     @staticmethod
     def log_func(func: Any) -> Any:
         """
         A decorator function that logs the execution time of a function.
         """
```

### Comparing `datachain-1.0.0/datachain/config/params.py` & `datachain-1.1.0/datachain/config/params.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import json
 
 
 class Params:
     """Params class."""
 
     config = {}  # type: dict
-    env_path = ""
+    env_path = ".env"
 
     @classmethod
     def reset_config(cls):
         """Reset the shared config dictionnary."""
         cls.config = {}
 
     @classmethod
```

### Comparing `datachain-1.0.0/datachain/core/common.py` & `datachain-1.1.0/datachain/core/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,14 +97,16 @@
 
 
 class DataSource:
     """Data Source class."""
 
     def __init__(self, func: Any = None, **kwds) -> None:
         self.func = func
+        self._cache = {}  # type: dict
+        self.to_cache = None #type: Optional[str]
         self.params = kwds
 
     def preload(self, **kwds) -> Any:
         """Preload parameters for a given source.
 
         Args:
             **kwds: Arbitrary keyword arguments to feed parameters.
@@ -123,19 +125,42 @@
 
         Returns:
             Any: Returns the data source object.
         """
         self.func = func
         return self
 
+    def cache(self, name: Optional[str]) -> DataSource:
+        """Cache data or access cached data.
+
+        Args:
+            name (str): Name of the data in cache or to cache.
+
+        Returns:
+            DataSource: Returns self to use during extraction.
+        """
+        self.to_cache = name
+        return self
+
+    def clear_cache(self):
+        """Clear the cache of the DataSource"""
+        self._cache = {}
+
     def __call__(self, *args: Any, **kwds: Any) -> Any:
         params = self.params.copy()
         params.update(kwds)
         if self.func:
-            return self.func(*args, **params)
+            if self.to_cache in self._cache:
+                self.to_cache = None
+                return self._cache[self.to_cache]
+            data = self.func(*args, **params)
+            if self.to_cache:
+                self._cache[self.to_cache] = data
+                self.to_cache = None
+            return data
         return None
 
 
 def _transform(obj: Any, func: Any, args: Tuple, kwds: Dict) -> Any:
     """Apply a given function to transform data using the given arguments.
 
     Args:
@@ -196,27 +221,34 @@
 
 class Data(Lazy):
     """Data class."""
 
     def __init__(
         self,
         extractor: Optional[Callable] = None,
-        args: Optional[Tuple] = None,
+        args: Optional[List] = None,
         kwds: Optional[Dict] = None,
         cached: bool = True,
     ) -> None:
         """Initializes a new Data instance.
 
         Args:
             extractor (Optional[Callable]): The data extraction function to use.
             params (Optional[Dict]): Parameters to pass to the extraction function.
             cached (bool): Whether the data should be cached or loaded on demand.
         """
         self.extractor = extractor
-        self.params = inspect.signature(extractor).bind(*args, **kwds)
+        if args is None:
+            args = []
+        if kwds is None:
+            kwds = {}
+        if extractor is None:
+            self.params = inspect.signature(lambda: 1).bind()
+        else:
+            self.params = inspect.signature(extractor).bind(*args, **kwds)
         self.cached = cached
 
     @Lazy.property
     def data(self) -> Any:
         """Returns the value of the `_data` attribute, loading it lazily if necessary.
 
         Raises:
@@ -304,15 +336,15 @@
             *args (Any): Additional positional arguments to pass to the function.
             **kwds (Any): Additional keyword arguments to pass to the function.
 
         Returns:
             Any: A new Data instance with the transformed data.
         """
         sign = inspect.signature(_transform).bind(self, func, args, kwds)
-        return Data(_transform, sign.args, sign.kwargs, self.cached)
+        return Data(_transform, list(sign.args), sign.kwargs, self.cached)
 
     def chain(self, *pipes: Pipe) -> Union[Any, Tuple[Any, List[Any]]]:
         """Chains multiple transformation functions together and applies them
         sequentially to the data stored in the current instance of Data.
 
         Args:
             *pipes (Pipe): One or more Pipe objects representing transformation
@@ -376,19 +408,20 @@
             except KeyError as _:
                 params = {}
         else:
             params = {}
         params.update(kwds)
         extractor_func = getattr(extractor, "func", extractor)
         sign = inspect.signature(extractor_func).bind(*args, **params)
-        Logger.logger.info(
-            "Extract data from extractor '%s' using these arguments: %s",
-            extractor_func.__name__,
-            str(sign.arguments),
-        )
+        if Logger.logger:
+            Logger.logger.info(
+                "Extract data from extractor '%s' using these arguments: %s",
+                extractor_func.__name__,
+                str(sign.arguments),
+            )
         return sign
 
     @staticmethod
     def extract(
         extractor: Callable, *args: Any, key: Optional[str] = None, **kwds: Any
     ) -> Any:
         """Extract data from a data source using the config and an appropriate
@@ -427,15 +460,16 @@
             try:
                 params = Params.config[key]
             except KeyError as _:
                 params = {}
         else:
             params = {}
         params.update(kwds)
-        sign = inspect.signature(_transform).bind(self, loader, args, params)
+        loader_func = getattr(loader, "func", loader)
+        sign = inspect.signature(_transform).bind(self, loader_func, args, params)
         _transform(*sign.args, **sign.kwargs)
         return self
 
 
 class DataManager:
     """
     Data Manager class.
@@ -475,19 +509,20 @@
         Returns:
             Any: The arguments to pass to the extractor function.
         """
         self.__params.update(kwds)
         extractor_func = getattr(extractor, "func", extractor)
         sign = inspect.signature(extractor_func).bind(*args, **self.__params)
         self.__params = {}
-        Logger.logger.info(
-            "Extract data from extractor '%s' using these arguments: %s",
-            extractor_func.__name__,
-            str(sign.arguments),
-        )
+        if Logger.logger:
+            Logger.logger.info(
+                "Extract data from extractor '%s' using these arguments: %s",
+                extractor_func.__name__,
+                str(sign.arguments),
+            )
         return sign
 
     def extract(self, extractor: Callable, *args: Any, **kwds: Any) -> Any:
         """Extract data from a data source using the config and an appropriate
         extractor.
 
         Args:
@@ -498,15 +533,16 @@
         Returns:
             Any: The extracted data.
         """
         params = self.__setup_extract(extractor, args, kwds)
         data = Data(extractor, params.args, params.kwargs, True)
         cache_key = str(uuid.uuid5(session_uuid, data.serialize()))
         if cache_key in self.__cache.keys():
-            Logger.logger.info("Load data from cache")
+            if Logger.logger:
+                Logger.logger.info("Load data from cache")
             data.force_data(self.__cache[cache_key])
         else:
             self.load_cache(data, data.serialize())
         return data
 
     def uncached_extract(self, extractor: Callable, *args: Any, **kwds: Any) -> Data:
         """Extract data from a data source using the config and an appropriate
@@ -531,13 +567,14 @@
             data (Any): The data to be cached.
             key (str): A string key used to retrieve cached data from the DataManager.
 
         Raises:
             NotImplementedError: If the data is an awaitable object, as these cannot be
             cached.
         """
-        Logger.logger.info("Load data to cache")
+        if Logger.logger:
+            Logger.logger.info("Load data to cache")
         if not inspect.isawaitable(data.data):
             key = str(uuid.uuid5(session_uuid, key))
             self.__cache[key] = data.data
         else:
             raise NotImplementedError("Awaitable extraction is not cacheable")
```

### Comparing `datachain-1.0.0/datachain/core/lazy.py` & `datachain-1.1.0/datachain/core/lazy.py`

 * *Files identical despite different names*

### Comparing `datachain-1.0.0/datachain/core/sync.py` & `datachain-1.1.0/datachain/core/sync.py`

 * *Files identical despite different names*

### Comparing `datachain-1.0.0/datachain/utils/func.py` & `datachain-1.1.0/datachain/utils/func.py`

 * *Files identical despite different names*

