# Comparing `tmp/configzen-0.2.4.tar.gz` & `tmp/configzen-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.2.4.tar", max compression
+gzip compressed data, was "configzen-0.2.5.tar", max compression
```

## Comparing `configzen-0.2.4.tar` & `configzen-0.2.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.2.4/configzen/__init__.py
--rw-r--r--   0        0        0      939 2023-05-30 00:29:12.190684 configzen-0.2.4/configzen/__main__.py
--rw-r--r--   0        0        0    68063 2023-06-05 07:06:03.591411 configzen-0.2.4/configzen/config.py
--rw-r--r--   0        0        0     2460 2023-06-05 06:53:12.902541 configzen-0.2.4/configzen/errors.py
--rw-r--r--   0        0        0    30567 2023-06-05 06:53:19.290433 configzen-0.2.4/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.2.4/configzen/py.typed
--rw-r--r--   0        0        0     1047 2023-06-05 06:53:17.656362 configzen-0.2.4/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.2.4/LICENSE
--rw-r--r--   0        0        0     1154 2023-06-05 07:06:36.501662 configzen-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     7155 2023-05-30 19:13:13.036046 configzen-0.2.4/README.md
--rw-r--r--   0        0        0     7891 1970-01-01 00:00:00.000000 configzen-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.2.5/configzen/__init__.py
+-rw-r--r--   0        0        0      939 2023-05-30 00:29:12.190684 configzen-0.2.5/configzen/__main__.py
+-rw-r--r--   0        0        0    67942 2023-06-06 17:33:04.155792 configzen-0.2.5/configzen/config.py
+-rw-r--r--   0        0        0     2460 2023-06-05 06:53:12.902541 configzen-0.2.5/configzen/errors.py
+-rw-r--r--   0        0        0    30567 2023-06-05 06:53:19.290433 configzen-0.2.5/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.2.5/configzen/py.typed
+-rw-r--r--   0        0        0     1047 2023-06-05 06:53:17.656362 configzen-0.2.5/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.2.5/LICENSE
+-rw-r--r--   0        0        0     1154 2023-06-06 17:34:53.185776 configzen-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     7155 2023-05-30 19:13:13.036046 configzen-0.2.5/README.md
+-rw-r--r--   0        0        0     7891 1970-01-01 00:00:00.000000 configzen-0.2.5/PKG-INFO
```

### Comparing `configzen-0.2.4/configzen/__main__.py` & `configzen-0.2.5/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.2.4/configzen/config.py` & `configzen-0.2.5/configzen/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1983,20 +1983,18 @@
         create_if_missing: bool | None = None,
     ) -> ConfigManager[ConfigModelT]:
         if resource is None:
             resource = getattr(cls.__config__, "resource", None)
         if resource is None:
             raise ValueError("No resource specified")
         manager: ConfigManager[ConfigModelT]
-        if isinstance(resource, str):
-            manager = ConfigManager(resource)
-        elif isinstance(resource, ConfigManager):
+        if isinstance(resource, ConfigManager):
             manager = resource
         else:
-            raise TypeError(f"Invalid resource type: {type(resource).__name__}")
+            manager = ConfigManager(resource)
         if create_if_missing is not None:
             manager.create_if_missing = create_if_missing
         return manager
 
     @property
     def initial_state(self) -> dict[str, Any]:
         """
```

### Comparing `configzen-0.2.4/configzen/errors.py` & `configzen-0.2.5/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.2.4/configzen/processor.py` & `configzen-0.2.5/configzen/processor.py`

 * *Files identical despite different names*

### Comparing `configzen-0.2.4/configzen/typedefs.py` & `configzen-0.2.5/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.2.4/LICENSE` & `configzen-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.2.4/pyproject.toml` & `configzen-0.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.2.4"
+version = "0.2.5"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bswck/configzen"
 
 [tool.poetry.dependencies]
```

### Comparing `configzen-0.2.4/README.md` & `configzen-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.2.4/PKG-INFO` & `configzen-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.2.4
+Version: 0.2.5
 Summary: The easiest way to manage configuration files in Python
 Home-page: https://github.com/bswck/configzen
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

