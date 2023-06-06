# Comparing `tmp/aiodbm-0.3.0.tar.gz` & `tmp/aiodbm-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodbm-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiodbm-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiodbm-0.3.0.tar` & `aiodbm-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1080 2023-06-05 18:14:10.939963 aiodbm-0.3.0/LICENSE
--rw-r--r--   0        0        0     3725 2023-06-05 18:14:10.939963 aiodbm-0.3.0/README.rst
--rw-r--r--   0        0        0      795 2023-06-05 18:14:10.939963 aiodbm-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      142 2023-06-05 18:14:10.939963 aiodbm-0.3.0/src/aiodbm/__init__.py
--rw-r--r--   0        0        0     5819 2023-06-05 18:14:10.939963 aiodbm-0.3.0/src/aiodbm/core.py
--rw-r--r--   0        0        0     3103 2023-06-05 18:14:10.939963 aiodbm-0.3.0/src/aiodbm/threads.py
--rw-r--r--   0        0        0     4417 1970-01-01 00:00:00.000000 aiodbm-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-06-06 13:50:04.064326 aiodbm-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3725 2023-06-06 13:50:04.064326 aiodbm-0.4.0/README.rst
+-rw-r--r--   0        0        0      795 2023-06-06 13:50:04.064326 aiodbm-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      158 2023-06-06 13:50:04.064326 aiodbm-0.4.0/src/aiodbm/__init__.py
+-rw-r--r--   0        0        0     6796 2023-06-06 13:50:04.064326 aiodbm-0.4.0/src/aiodbm/core.py
+-rw-r--r--   0        0        0     3103 2023-06-06 13:50:04.064326 aiodbm-0.4.0/src/aiodbm/threads.py
+-rw-r--r--   0        0        0     4417 1970-01-01 00:00:00.000000 aiodbm-0.4.0/PKG-INFO
```

### Comparing `aiodbm-0.3.0/LICENSE` & `aiodbm-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodbm-0.3.0/README.rst` & `aiodbm-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `aiodbm-0.3.0/pyproject.toml` & `aiodbm-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiodbm-0.3.0/src/aiodbm/core.py` & `aiodbm-0.4.0/src/aiodbm/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 """Core logic for an async DBM proxy."""
 
 import asyncio
 import dbm
 import logging
+from dbm import error
 from functools import partial
 from pathlib import Path
-from typing import Any, Callable, Generator, List, Optional, Union
+from typing import Any, AsyncGenerator, Callable, Generator, List, Optional, Union
 
 from aiodbm.threads import ThreadRunner
 
 logger = logging.getLogger("aiodbm")
 
 
+__all__ = ["Database", "error", "open", "whichdb"]
+
+
 class Database:
-    """A proxy for a DBM database."""
+    """A DBM database.
+
+    Not that some methods are available on GDBM only.
+    You can check if your database is GDBM with :func:`is_gdbm`.
+    """
 
     def __init__(self, connector: Callable) -> None:
         super().__init__()
         self._db = None
         self._connector = connector
         self._runner = ThreadRunner()
 
@@ -139,14 +147,36 @@
     # GDBM only API
 
     async def firstkey(self) -> bytes:
         """Return the first key for looping over all keys. GDBM only."""
 
         return await self._execute(self._db_strict.firstkey)
 
+    async def keys_iterator(self) -> AsyncGenerator[bytes, None]:
+        """Return all keys as async generator. GDBM only.
+
+        In contrast to :func:`keys` this method will not load the full list of keys into
+        memory, but instead fetch keys one after the other.
+
+        Note that the order of keys is implementation specific
+        and can not be relied on.
+
+        Usage example:
+
+        .. code-block:: Python
+
+            async for key in db.keys_iterator():
+                print(key)
+
+        """
+        key = await self.firstkey()
+        while key is not None:
+            yield key
+            key = await self.nextkey(key)
+
     async def nextkey(self, key: Union[str, bytes]) -> Optional[bytes]:
         """Return the next key, when looping over all keys.
         Or return None, when the end of the loop has been reached.
         GDBM only.
         """
 
         return await self._execute(self._db_strict.nextkey, key)
@@ -162,28 +192,36 @@
         GDBM only.
         """
 
         await self._execute(self._db_strict.sync)
 
 
 def open(file: Union[str, Path], *args, **kwargs) -> Database:
-    """Create and return a proxy to the DBM database.
+    """Create and return a proxy to a DBM database.
 
-    Example:
+    Args:
+        file: filename for the DBM database
+
+    Returns:
+        DBM database proxy object
+
+    Usage A:
 
     .. code-block:: Python
 
         async with open("example.dbm", "c") as db:
             ...
 
-    Args:
-        file: filename for the DBM database
+    Usage B:
 
-    Returns:
-        DBM database proxy object
+    .. code-block:: Python
+
+        db = async open("example.dbm", "c"):
+        ...
+        await db.close()
     """
 
     def connector():
         filepath = str(file)
         return dbm.open(filepath, *args, **kwargs)
 
     return Database(connector)
```

### Comparing `aiodbm-0.3.0/src/aiodbm/threads.py` & `aiodbm-0.4.0/src/aiodbm/threads.py`

 * *Files identical despite different names*

### Comparing `aiodbm-0.3.0/PKG-INFO` & `aiodbm-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiodbm
-Version: 0.3.0
+Version: 0.4.0
 Summary: An AsyncIO bridge for DBM.
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
```

