# Comparing `tmp/jupyverse_api-0.1.8.tar.gz` & `tmp/jupyverse_api-0.1.9.tar.gz`

## Comparing `jupyverse_api-0.1.8.tar` & `jupyverse_api-0.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 jupyverse_api-0.1.8/jupyverse_api/__init__.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 jupyverse_api-0.1.8/jupyverse_api/cli.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyverse_api-0.1.8/jupyverse_api/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse_api-0.1.8/jupyverse_api/py.typed
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 jupyverse_api-0.1.8/jupyverse_api/app/__init__.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse_api-0.1.8/jupyverse_api/auth/__init__.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyverse_api-0.1.8/jupyverse_api/auth/models.py
--rw-r--r--   0        0        0     5019 2020-02-02 00:00:00.000000 jupyverse_api-0.1.8/jupyverse_api/contents/__init__.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 jupyverse_api-0.1.8/jupyverse_api/contents/models.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse_api-0.1.8/jupyverse_api/frontend/__init__.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 jupyverse_api-0.1.8/jupyverse_api/jupyterlab/__init__.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 jupyverse_api-0.1.8/jupyverse_api/kernels/__init__.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse_api-0.1.8/jupyverse_api/kernels/models.py
--rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 jupyverse_api-0.1.8/jupyverse_api/lab/__init__.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyverse_api-0.1.8/jupyverse_api/login/__init__.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 jupyverse_api-0.1.8/jupyverse_api/main/__init__.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 jupyverse_api-0.1.8/jupyverse_api/nbconvert/__init__.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyverse_api-0.1.8/jupyverse_api/resource_usage/__init__.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 jupyverse_api-0.1.8/jupyverse_api/retrolab/__init__.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyverse_api-0.1.8/jupyverse_api/terminals/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse_api-0.1.8/jupyverse_api/terminals/models.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 jupyverse_api-0.1.8/jupyverse_api/yjs/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse_api-0.1.8/jupyverse_api/yjs/models.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 jupyverse_api-0.1.8/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse_api-0.1.8/COPYING.md
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse_api-0.1.8/README.md
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 jupyverse_api-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 jupyverse_api-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/__init__.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/cli.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/py.typed
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/app/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/auth/__init__.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/auth/models.py
+-rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/contents/__init__.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/contents/models.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/frontend/__init__.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/jupyterlab/__init__.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/kernels/__init__.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/kernels/models.py
+-rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/lab/__init__.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/login/__init__.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/main/__init__.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/nbconvert/__init__.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/resource_usage/__init__.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/retrolab/__init__.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/terminals/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/terminals/models.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/yjs/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/yjs/models.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/COPYING.md
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/README.md
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/PKG-INFO
```

### Comparing `jupyverse_api-0.1.8/jupyverse_api/__init__.py` & `jupyverse_api-0.1.9/jupyverse_api/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict
 
 from pydantic import BaseModel, Extra
 
 from .app import App
 
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 
 
 class Singleton(type):
     _instances: Dict = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
```

### Comparing `jupyverse_api-0.1.8/jupyverse_api/cli.py` & `jupyverse_api-0.1.9/jupyverse_api/cli.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.8/jupyverse_api/app/__init__.py` & `jupyverse_api-0.1.9/jupyverse_api/app/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.8/jupyverse_api/auth/__init__.py` & `jupyverse_api-0.1.9/jupyverse_api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.8/jupyverse_api/contents/__init__.py` & `jupyverse_api-0.1.9/jupyverse_api/contents/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     @property
     @abstractmethod
     def file_id_manager(self) -> FileIdManager:
         ...
 
     @abstractmethod
     async def read_content(
-        self, path: Union[str, Path], get_content: bool, as_json: bool = False
+        self, path: Union[str, Path], get_content: bool, file_format: Optional[str] = None
     ) -> Content:
         ...
 
     @abstractmethod
     async def write_content(self, content: Union[SaveContent, Dict]) -> None:
         ...
```

### Comparing `jupyverse_api-0.1.8/jupyverse_api/contents/models.py` & `jupyverse_api-0.1.9/jupyverse_api/contents/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.8/jupyverse_api/jupyterlab/__init__.py` & `jupyverse_api-0.1.9/jupyverse_api/jupyterlab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.8/jupyverse_api/kernels/__init__.py` & `jupyverse_api-0.1.9/jupyverse_api/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.8/jupyverse_api/kernels/models.py` & `jupyverse_api-0.1.9/jupyverse_api/kernels/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.8/jupyverse_api/lab/__init__.py` & `jupyverse_api-0.1.9/jupyverse_api/lab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.8/jupyverse_api/main/__init__.py` & `jupyverse_api-0.1.9/jupyverse_api/main/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.8/jupyverse_api/nbconvert/__init__.py` & `jupyverse_api-0.1.9/jupyverse_api/nbconvert/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.8/jupyverse_api/resource_usage/__init__.py` & `jupyverse_api-0.1.9/jupyverse_api/resource_usage/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.8/jupyverse_api/retrolab/__init__.py` & `jupyverse_api-0.1.9/jupyverse_api/retrolab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.8/jupyverse_api/terminals/__init__.py` & `jupyverse_api-0.1.9/jupyverse_api/terminals/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.8/jupyverse_api/yjs/__init__.py` & `jupyverse_api-0.1.9/jupyverse_api/yjs/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.8/.gitignore` & `jupyverse_api-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.8/COPYING.md` & `jupyverse_api-0.1.9/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.8/pyproject.toml` & `jupyverse_api-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.8/PKG-INFO` & `jupyverse_api-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyverse_api
-Version: 0.1.8
+Version: 0.1.9
 Summary: The public API for Jupyverse
 Project-URL: Source, https://github.com/jupyter-server/jupyverse/jupyverse_api
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: api,jupyverse
 Classifier: Development Status :: 4 - Beta
```

