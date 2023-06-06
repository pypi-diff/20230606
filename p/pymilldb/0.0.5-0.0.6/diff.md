# Comparing `tmp/pymilldb-0.0.5.tar.gz` & `tmp/pymilldb-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymilldb-0.0.5.tar", last modified: Thu Jun  1 18:42:50 2023, max compression
+gzip compressed data, was "pymilldb-0.0.6.tar", last modified: Tue Jun  6 21:15:59 2023, max compression
```

## Comparing `pymilldb-0.0.5.tar` & `pymilldb-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-01 18:42:50.531944 pymilldb-0.0.5/
--rw-rw-r--   0 zeus      (1000) zeus      (1000)     1095 2023-06-01 18:38:01.000000 pymilldb-0.0.5/LICENSE
--rw-rw-r--   0 zeus      (1000) zeus      (1000)     1031 2023-06-01 18:42:50.531944 pymilldb-0.0.5/PKG-INFO
--rw-rw-r--   0 zeus      (1000) zeus      (1000)      523 2023-06-01 18:38:01.000000 pymilldb-0.0.5/README.md
--rw-rw-r--   0 zeus      (1000) zeus      (1000)       89 2023-06-01 18:38:01.000000 pymilldb-0.0.5/pyproject.toml
--rw-rw-r--   0 zeus      (1000) zeus      (1000)      633 2023-06-01 18:42:50.531944 pymilldb-0.0.5/setup.cfg
-drwxrwxr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-01 18:42:50.527944 pymilldb-0.0.5/src/
-drwxrwxr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-01 18:42:50.531944 pymilldb-0.0.5/src/pymilldb/
--rw-rw-r--   0 zeus      (1000) zeus      (1000)      167 2023-06-01 18:38:01.000000 pymilldb-0.0.5/src/pymilldb/__init__.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)     2669 2023-06-01 18:38:01.000000 pymilldb-0.0.5/src/pymilldb/mdb_client.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)     1554 2023-06-01 18:38:01.000000 pymilldb-0.0.5/src/pymilldb/protocol.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)     1602 2023-06-01 18:38:01.000000 pymilldb-0.0.5/src/pymilldb/sampler.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)     9875 2023-06-01 18:39:28.000000 pymilldb-0.0.5/src/pymilldb/tensor_store.py
-drwxrwxr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-01 18:42:50.531944 pymilldb-0.0.5/src/pymilldb/utils/
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-06-01 18:38:01.000000 pymilldb-0.0.5/src/pymilldb/utils/__init__.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)      353 2023-06-01 18:38:01.000000 pymilldb-0.0.5/src/pymilldb/utils/decorators.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)      630 2023-06-01 18:38:01.000000 pymilldb-0.0.5/src/pymilldb/utils/graph.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)     1911 2023-06-01 18:38:01.000000 pymilldb-0.0.5/src/pymilldb/utils/packer.py
-drwxrwxr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-01 18:42:50.531944 pymilldb-0.0.5/src/pymilldb.egg-info/
--rw-rw-r--   0 zeus      (1000) zeus      (1000)     1031 2023-06-01 18:42:50.000000 pymilldb-0.0.5/src/pymilldb.egg-info/PKG-INFO
--rw-rw-r--   0 zeus      (1000) zeus      (1000)      437 2023-06-01 18:42:50.000000 pymilldb-0.0.5/src/pymilldb.egg-info/SOURCES.txt
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        1 2023-06-01 18:42:50.000000 pymilldb-0.0.5/src/pymilldb.egg-info/dependency_links.txt
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        9 2023-06-01 18:42:50.000000 pymilldb-0.0.5/src/pymilldb.egg-info/top_level.txt
+drwxr-xr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-06 21:15:59.185585 pymilldb-0.0.6/
+-rw-r--r--   0 zeus      (1000) zeus      (1000)     1095 2023-05-30 21:05:16.000000 pymilldb-0.0.6/LICENSE
+-rw-r--r--   0 zeus      (1000) zeus      (1000)     1031 2023-06-06 21:15:59.185585 pymilldb-0.0.6/PKG-INFO
+-rw-r--r--   0 zeus      (1000) zeus      (1000)      523 2023-05-30 21:18:35.000000 pymilldb-0.0.6/README.md
+-rw-r--r--   0 zeus      (1000) zeus      (1000)       89 2023-05-30 21:05:16.000000 pymilldb-0.0.6/pyproject.toml
+-rw-r--r--   0 zeus      (1000) zeus      (1000)      633 2023-06-06 21:15:59.185585 pymilldb-0.0.6/setup.cfg
+drwxr-xr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-06 21:15:59.185585 pymilldb-0.0.6/src/
+drwxr-xr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-06 21:15:59.185585 pymilldb-0.0.6/src/pymilldb/
+-rw-r--r--   0 zeus      (1000) zeus      (1000)      167 2023-05-30 21:05:16.000000 pymilldb-0.0.6/src/pymilldb/__init__.py
+-rw-r--r--   0 zeus      (1000) zeus      (1000)     2802 2023-06-06 21:04:43.000000 pymilldb-0.0.6/src/pymilldb/mdb_client.py
+-rw-r--r--   0 zeus      (1000) zeus      (1000)     1518 2023-06-06 21:04:43.000000 pymilldb-0.0.6/src/pymilldb/protocol.py
+-rw-r--r--   0 zeus      (1000) zeus      (1000)     1430 2023-06-06 21:04:43.000000 pymilldb-0.0.6/src/pymilldb/sampler.py
+-rw-r--r--   0 zeus      (1000) zeus      (1000)    10804 2023-06-06 21:04:43.000000 pymilldb-0.0.6/src/pymilldb/tensor_store.py
+drwxr-xr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-06 21:15:59.185585 pymilldb-0.0.6/src/pymilldb/utils/
+-rw-r--r--   0 zeus      (1000) zeus      (1000)        0 2023-05-30 21:05:16.000000 pymilldb-0.0.6/src/pymilldb/utils/__init__.py
+-rw-r--r--   0 zeus      (1000) zeus      (1000)      353 2023-05-30 21:05:16.000000 pymilldb-0.0.6/src/pymilldb/utils/decorators.py
+-rw-r--r--   0 zeus      (1000) zeus      (1000)      630 2023-05-30 21:05:16.000000 pymilldb-0.0.6/src/pymilldb/utils/graph.py
+-rw-r--r--   0 zeus      (1000) zeus      (1000)     2173 2023-06-06 21:04:43.000000 pymilldb-0.0.6/src/pymilldb/utils/packer.py
+drwxr-xr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-06 21:15:59.185585 pymilldb-0.0.6/src/pymilldb.egg-info/
+-rw-r--r--   0 zeus      (1000) zeus      (1000)     1031 2023-06-06 21:15:59.000000 pymilldb-0.0.6/src/pymilldb.egg-info/PKG-INFO
+-rw-r--r--   0 zeus      (1000) zeus      (1000)      437 2023-06-06 21:15:59.000000 pymilldb-0.0.6/src/pymilldb.egg-info/SOURCES.txt
+-rw-r--r--   0 zeus      (1000) zeus      (1000)        1 2023-06-06 21:15:59.000000 pymilldb-0.0.6/src/pymilldb.egg-info/dependency_links.txt
+-rw-r--r--   0 zeus      (1000) zeus      (1000)        9 2023-06-06 21:15:59.000000 pymilldb-0.0.6/src/pymilldb.egg-info/top_level.txt
```

### Comparing `pymilldb-0.0.5/LICENSE` & `pymilldb-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pymilldb-0.0.5/PKG-INFO` & `pymilldb-0.0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymilldb
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python library for MillenniumDB
 Home-page: https://github.com/MillenniumDB/PyMillDB
 Author: Vicente Calisto
 Author-email: vecalisto@uc.cl
 Project-URL: Bug Tracker, https://github.com/MillenniumDB/PyMillDB/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymilldb-0.0.5/README.md` & `pymilldb-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pymilldb-0.0.5/setup.cfg` & `pymilldb-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pymilldb
-version = 0.0.5
+version = 0.0.6
 author = Vicente Calisto
 author_email = vecalisto@uc.cl
 description = A python library for MillenniumDB
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MillenniumDB/PyMillDB
 project_urls =
```

### Comparing `pymilldb-0.0.5/src/pymilldb/mdb_client.py` & `pymilldb-0.0.6/src/pymilldb/mdb_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import socket
 from typing import Tuple
 
 from . import protocol
-from .utils import decorators
+from .utils import decorators, packer
 
 
 ## Interface for stablishing a connection with the server for
 # sending and receiving data.
 #
 # Almost every class and function in this library needs a `MDBClient` instance
 # as an argument to communicate with the server.
@@ -45,16 +45,17 @@
             self._closed = False
         except ConnectionRefusedError as e:
             raise ConnectionError(
                 f"Couldn't connect to MillenniumDB server at {self.address}"
             ) from e
 
     @decorators.check_closed
-    def _send(self, data: bytes) -> None:
-        self._sock.sendall(data)
+    def _send(self, request_type: protocol.RequestType, data: bytes) -> None:
+        header = packer.pack_byte(request_type) + packer.pack_uint64(len(data))
+        self._sock.sendall(header + data)
 
     @decorators.check_closed
     def _recv(self) -> Tuple[bytes, protocol.StatusCode]:
         # Helper function to receive exactly `length` bytes
         def recvall(length: int) -> bytes:
             data = b""
             while len(data) < length:
```

### Comparing `pymilldb-0.0.5/src/pymilldb/protocol.py` & `pymilldb-0.0.6/src/pymilldb/protocol.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
     # TENSOR STORE
     # STATIC METHODS
     TENSOR_STORE_EXISTS = 0b0000_0111
     TENSOR_STORE_IS_OPEN = 0b0000_1000
     TENSOR_STORE_CREATE = 0b0000_1001
     TENSOR_STORE_REMOVE = 0b0000_1010
-    TENSOR_STORE_LIST = 0b0000_1011
     TENSOR_STORE_OPEN = 0b0000_1100
     # INSTANCE METHODS
     TENSOR_STORE_CLOSE = 0b0000_1101
     TENSOR_STORE_CONTAINS = 0b0000_1110
     TENSOR_STORE_INSERT = 0b0000_1111
     TENSOR_STORE_MULTI_INSERT = 0b0001_0000
     TENSOR_STORE_GET = 0b0001_0001
```

### Comparing `pymilldb-0.0.5/src/pymilldb/sampler.py` & `pymilldb-0.0.6/src/pymilldb/sampler.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,32 +17,28 @@
         ## Client instance.
         self.client = client
 
     ## Returns a random subgraph
     def subgraph(self, num_seeds: int, num_neighbors: List[int]) -> Graph:
         # Send request
         msg = b""
-        msg += packer.pack_byte(RequestType.SAMPLER_SUBGRAPH)
         msg += packer.pack_uint64(num_seeds)
-        msg += packer.pack_uint64(len(num_neighbors))
         msg += packer.pack_uint64_vector(num_neighbors)
-        self.client._send(msg)
+        self.client._send(RequestType.SAMPLER_SUBGRAPH, msg)
 
         # Handle response
         data, _ = self.client._recv()
         return packer.unpack_graph(data)
 
     ## Returns a random subgraph for edge existance prediction
     def subgraph_edge_existance(
         self, num_preseeds: int, num_neighbors: List[int]
     ) -> Graph:
         # Send request
         msg = b""
-        msg += packer.pack_byte(RequestType.SAMPLER_SUBGRAPH_EDGE_EXISTANCE)
         msg += packer.pack_uint64(num_preseeds)
-        msg += packer.pack_uint64(len(num_neighbors))
         msg += packer.pack_uint64_vector(num_neighbors)
-        self.client._send(msg)
+        self.client._send(RequestType.SAMPLER_SUBGRAPH_EDGE_EXISTANCE, msg)
 
         # Handle response
         data, _ = self.client._recv()
         return packer.unpack_graph(data)
```

### Comparing `pymilldb-0.0.5/src/pymilldb/tensor_store.py` & `pymilldb-0.0.6/src/pymilldb/tensor_store.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from collections.abc import Iterable
 from typing import TYPE_CHECKING, List, Union
 
 import torch
 
 from .protocol import RequestType
 from .utils import decorators, packer
 
@@ -16,86 +17,58 @@
 # created. For consistency and our own use cases the tensors cannot be removed.
 class TensorStore:
     ## Returns `True` if the store exists.
     @staticmethod
     def exists(client: "MDBClient", name: str) -> bool:
         # Send request
         msg = b""
-        msg += packer.pack_byte(RequestType.TENSOR_STORE_EXISTS)
-        msg += packer.pack_uint64(len(name))
         msg += packer.pack_string(name)
-        client._send(msg)
+        client._send(RequestType.TENSOR_STORE_EXISTS, msg)
 
         # Handle response
         data, _ = client._recv()
         return packer.unpack_bool(data[0:8])
 
     ## Returns `True` if the store is open.
     @staticmethod
     def is_open(client: "MDBClient", name: str) -> bool:
         # Send request
         msg = b""
-        msg += packer.pack_byte(RequestType.TENSOR_STORE_IS_OPEN)
-        msg += packer.pack_uint64(len(name))
         msg += packer.pack_string(name)
-        client._send(msg)
+        client._send(RequestType.TENSOR_STORE_IS_OPEN, msg)
 
         # Handle response
         data, _ = client._recv()
         return packer.unpack_bool(data[0:8])
 
     ## Creates a new store on disk.
     @staticmethod
     def create(client: "MDBClient", name: str, tensor_size: int) -> None:
         if tensor_size <= 0:
             raise ValueError(f"tensor_size must be positive integer, got {tensor_size}")
         # Send request
         msg = b""
-        msg += packer.pack_byte(RequestType.TENSOR_STORE_CREATE)
         msg += packer.pack_uint64(tensor_size)
-        msg += packer.pack_uint64(len(name))
         msg += packer.pack_string(name)
-        client._send(msg)
+        client._send(RequestType.TENSOR_STORE_CREATE, msg)
 
         # Handle response
         client._recv()
 
     ## Removes a store from disk.
     @staticmethod
     def remove(client: "MDBClient", name: str) -> None:
         # Send request
         msg = b""
-        msg += packer.pack_byte(RequestType.TENSOR_STORE_REMOVE)
-        msg += packer.pack_uint64(len(name))
         msg += packer.pack_string(name)
-        client._send(msg)
+        client._send(RequestType.TENSOR_STORE_REMOVE, msg)
 
         # Handle response
         client._recv()
 
-    ## Returns a list of all store names.
-    @staticmethod
-    def list(client: "MDBClient") -> List[str]:
-        # Send request
-        msg = b""
-        msg += packer.pack_byte(RequestType.TENSOR_STORE_LIST)
-        client._send(msg)
-
-        # Handle response
-        data, _ = client._recv()
-        names = list()
-        lo, hi = 0, 8
-        num_stores = packer.unpack_uint64(data[lo:hi])
-        lo, hi = hi, hi + 8 * num_stores
-        name_sizes = packer.unpack_uint64_vector(data[lo:hi])
-        for name_size in name_sizes:
-            lo, hi = hi, hi + name_size
-            names.append(packer.unpack_string(data[lo:hi]))
-        return names
-
     ## Constructor for opening an existing store.
     def __init__(self, client: "MDBClient", name: str) -> None:
         ## Client instance.
         self.client = client
         ## Name of the store.
         self.name = name
         ## Fixed size for the tensors.
@@ -123,166 +96,212 @@
         return self
 
     ## Exit context manager.
     def __exit__(self, *_):
         self.close()
 
     ## Get tensors from the store with the pythonic syntax `store[key]`.
-    def __getitem__(self, key: Union[int, List[int]]) -> torch.Tensor:
-        if isinstance(key, int):
-            return self.get(key)
-        else:
+    def __getitem__(self, key: Union[int, str, List[int], List[str]]) -> torch.Tensor:
+        if not isinstance(key, str) and isinstance(key, Iterable):
             return self.multi_get(key)
+        else:
+            return self.get(key)
 
     ## Insert tensors into the store with the pythonic syntax `store[key] = value`.
-    def __setitem__(self, key: Union[int, List[int]], value: torch.Tensor) -> None:
-        if isinstance(key, int):
-            self.insert(key, value)
-        else:
+    def __setitem__(
+        self, key: Union[int, str, List[int], List[str]], value: torch.Tensor
+    ) -> None:
+        if not isinstance(key, str) and isinstance(key, Iterable):
             self.multi_insert(key, value)
+        else:
+            self.insert(key, value)
 
     ## Returns `True` if the store contains the given key with the pythonic syntax `key in store`.
-    def __contains__(self, key: int) -> bool:
+    def __contains__(self, key: Union[int, str]) -> bool:
         return self.contains(key)
 
     ## Returns `True` if the store contains the given key.
     @decorators.check_closed
-    def contains(self, object_id: int) -> bool:
+    def contains(self, key: Union[int, str]) -> bool:
+        packed_key = b""
+        if isinstance(key, int):
+            packed_key += packer.pack_bool(True)
+            packed_key += packer.pack_uint64(key)
+        elif isinstance(key, str):
+            packed_key += packer.pack_bool(False)
+            packed_key += packer.pack_string(key)
+        else:
+            raise TypeError(f"Key must be int or str, got {type(key)}")
+
         # Send request
         msg = b""
-        msg += packer.pack_byte(RequestType.TENSOR_STORE_CONTAINS)
         msg += packer.pack_uint64(self._tensor_store_id)
-        msg += packer.pack_uint64(object_id)
-        self.client._send(msg)
+        msg += packed_key
+        self.client._send(RequestType.TENSOR_STORE_CONTAINS, msg)
 
         # Handle response
         data, _ = self.client._recv()
         return packer.unpack_bool(data[0:8])
 
     ## Inserts a tensor into the store.
     @decorators.check_closed
-    def insert(self, object_id: int, tensor: torch.Tensor) -> None:
+    def insert(self, key: Union[int, str], tensor: torch.Tensor) -> None:
+        packed_key = b""
+        if isinstance(key, int):
+            packed_key += packer.pack_bool(True)
+            packed_key += packer.pack_uint64(key)
+        elif isinstance(key, str):
+            packed_key += packer.pack_bool(False)
+            packed_key += packer.pack_string(key)
+        else:
+            raise TypeError(f"Key must be int or str, got {type(key)}")
+
         if tensor.dtype != torch.float32:
-            raise ValueError(f"Tensor dtype must be torch.float32, got {tensor.dtype}")
+            raise ValueError(f"Tensor dtype must be torch.float32, got {type(tensor)}")
         if tensor.numel() != self.tensor_size:
             raise ValueError(
                 f"Tensor size ({tensor.numel()}) does not match tensor_size of the store ({self.tensor_size})"
             )
 
         # Send request
         msg = b""
-        msg += packer.pack_byte(RequestType.TENSOR_STORE_INSERT)
         msg += packer.pack_uint64(self._tensor_store_id)
-        msg += packer.pack_uint64(object_id)
+        msg += packed_key
         msg += packer.pack_float_vector(tensor.flatten())
-        self.client._send(msg)
+        self.client._send(RequestType.TENSOR_STORE_INSERT, msg)
 
         # Handle response
         self.client._recv()
 
     ## Inserts multiple tensors into the store.
     @decorators.check_closed
-    def multi_insert(self, object_ids: List[int], tensors: torch.Tensor) -> None:
+    def multi_insert(
+        self, keys: Union[List[int], List[str]], tensors: torch.Tensor
+    ) -> None:
+        packed_key = b""
+        if all(isinstance(key, int) for key in keys):
+            packed_key += packer.pack_bool(True)
+            packed_key += packer.pack_uint64(len(keys))
+            packed_key += packer.pack_uint64_vector(keys)
+        elif all(isinstance(key, str) for key in keys):
+            packed_key += packer.pack_bool(False)
+            packed_key += packer.pack_string_vector(keys)
+        else:
+            raise TypeError(f"Key must be List[int] or List[str], got {type(keys)}")
+
         if tensors.dtype != torch.float32:
-            raise ValueError(f"Tensor dtype must be torch.float32, got {tensors.dtype}")
+            raise ValueError(f"Tensor dtype must be torch.float32, got {type(tensors)}")
         if len(tensors.size()) != 2:
             raise ValueError(
-                f"tensors must be 2-dimensional, but got {len(tensors.size())}-dimensional tensor"
+                f"Tensors must be 2-dimensional, but got {len(tensors.size())}-dimensional tensor"
             )
-        if len(object_ids) != tensors.size(0):
+        if len(keys) != tensors.size(0):
             raise ValueError(
-                f"The number of object_ids ({len(object_ids)}) does not match the tensors rows ({tensors.size(0)})"
+                f"The number of keys ({len(keys)}) does not match the tensors rows ({tensors.size(0)})"
             )
         if tensors.size(1) != self.tensor_size:
             raise ValueError(
-                f"tensors columns ({tensors.size(1)}) does not match tensor_size of the store ({self.tensor_size})"
+                f"Tensors columns ({tensors.size(1)}) does not match tensor_size of the store ({self.tensor_size})"
             )
 
         # Send request
         msg = b""
-        msg += packer.pack_byte(RequestType.TENSOR_STORE_MULTI_INSERT)
         msg += packer.pack_uint64(self._tensor_store_id)
-        msg += packer.pack_uint64(len(object_ids))
-        msg += packer.pack_uint64_vector(object_ids)
+        msg += packed_key
+        # Written as a plain vector, the server knows the matrix shape
         msg += packer.pack_float_vector(tensors.flatten())
-        self.client._send(msg)
+        self.client._send(RequestType.TENSOR_STORE_MULTI_INSERT, msg)
 
         # Handle response
         self.client._recv()
 
     ## Gets a tensor from the store.
     @decorators.check_closed
-    def get(self, object_id: int) -> torch.Tensor:
+    def get(self, key: Union[int, str]) -> torch.Tensor:
+        packed_key = b""
+        if isinstance(key, int):
+            packed_key += packer.pack_bool(True)
+            packed_key += packer.pack_uint64(key)
+        elif isinstance(key, str):
+            packed_key += packer.pack_bool(False)
+            packed_key += packer.pack_string(key)
+        else:
+            raise TypeError(f"Key must be int or str, got {type(key)}")
+
         # Send request
         msg = b""
-        msg += packer.pack_byte(RequestType.TENSOR_STORE_GET)
         msg += packer.pack_uint64(self._tensor_store_id)
-        msg += packer.pack_uint64(object_id)
-        self.client._send(msg)
+        msg += packed_key
+        self.client._send(RequestType.TENSOR_STORE_GET, msg)
 
         # Handle response
         data, _ = self.client._recv()
-        lo, hi = 0, 4 * self.tensor_size
+        vector_size = packer.unpack_uint64(data[0:8])
         return torch.tensor(
-            data=packer.unpack_float_vector(data[lo:hi]), dtype=torch.float32
+            data=packer.unpack_float_vector(data[8 : 8 + 8 * vector_size]),
+            dtype=torch.float32,
         )
 
     ## Gets multiple tensors from the store.
     @decorators.check_closed
-    def multi_get(self, object_ids: List[int]) -> torch.Tensor:
+    def multi_get(self, keys: Union[List[int], List[str]]) -> torch.Tensor:
+        packed_key = b""
+        if all(isinstance(key, int) for key in keys):
+            packed_key += packer.pack_bool(True)
+            packed_key += packer.pack_uint64_vector(keys)
+        elif all(isinstance(key, str) for key in keys):
+            packed_key += packer.pack_bool(False)
+            packed_key += packer.pack_string_vector(keys)
+        else:
+            raise TypeError(f"Key must be List[int] or List[str], got {type(keys)}")
+
         # Send request
         msg = b""
-        msg += packer.pack_byte(RequestType.TENSOR_STORE_MULTI_GET)
         msg += packer.pack_uint64(self._tensor_store_id)
-        msg += packer.pack_uint64(len(object_ids))
-        msg += packer.pack_uint64_vector(object_ids)
-        self.client._send(msg)
+        msg += packed_key
+        self.client._send(RequestType.TENSOR_STORE_MULTI_GET, msg)
 
         # Handle response
         data, _ = self.client._recv()
-        lo, hi = 0, 4 * self.tensor_size * len(object_ids)
+        vector_size = packer.unpack_uint64(data[0:8])
         return torch.tensor(
-            data=packer.unpack_float_vector(data[lo:hi]),
+            data=packer.unpack_float_vector(data[8 : 8 + 8 * vector_size]),
             dtype=torch.float32,
-        ).reshape(len(object_ids), self.tensor_size)
+        ).reshape(len(keys), self.tensor_size)
 
     ## Returns the number of tensors in the store.
     @decorators.check_closed
     def size(self) -> int:
         # Send request
         msg = b""
-        msg += packer.pack_byte(RequestType.TENSOR_STORE_SIZE)
         msg += packer.pack_uint64(self._tensor_store_id)
-        self.client._send(msg)
+        self.client._send(RequestType.TENSOR_STORE_SIZE, msg)
 
         # Handle response
         data, _ = self.client._recv()
         return packer.unpack_uint64(data[0:8])
 
     def _open(self) -> None:
         # Send request
         msg = b""
-        msg += packer.pack_byte(RequestType.TENSOR_STORE_OPEN)
-        msg += packer.pack_uint64(len(self.name))
         msg += packer.pack_string(self.name)
-        self.client._send(msg)
+        self.client._send(RequestType.TENSOR_STORE_OPEN, msg)
 
         # Handle response
         data, _ = self.client._recv()
         lo, hi = 0, 8
         self._tensor_store_id = packer.unpack_uint64(data[lo:hi])
         lo, hi = hi, hi + 8
         self.tensor_size = packer.unpack_uint64(data[lo:hi])
         self._closed = False
 
     def _close(self) -> None:
         # Send request
         msg = b""
-        msg += packer.pack_byte(RequestType.TENSOR_STORE_CLOSE)
         msg += packer.pack_uint64(self._tensor_store_id)
-        self.client._send(msg)
+        self.client._send(RequestType.TENSOR_STORE_CLOSE, msg)
 
         # Handle response
         self.client._recv()
         self.tensor_size = None
         self._tensor_store_id = None
         self._closed = True
```

### Comparing `pymilldb-0.0.5/src/pymilldb/utils/graph.py` & `pymilldb-0.0.6/src/pymilldb/utils/graph.py`

 * *Files identical despite different names*

### Comparing `pymilldb-0.0.5/src/pymilldb/utils/packer.py` & `pymilldb-0.0.6/src/pymilldb/utils/packer.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,31 +13,41 @@
 
 
 def pack_uint64(i: int) -> bytes:
     return struct.pack(">Q", i)
 
 
 def pack_string(string: str) -> bytes:
-    return string.encode("utf-8")
+    return pack_uint64(len(string)) + string.encode("utf-8")
 
 
 def pack_uint64_vector(vector: List[int]) -> bytes:
     data = b""
+    data += pack_uint64(len(vector))
     for value in vector:
         data += pack_uint64(value)
     return data
 
 
 def pack_float_vector(vector: List[float]) -> bytes:
     data = b""
+    data += pack_uint64(len(vector))
     for value in vector:
         data += struct.pack(">f", value)
     return data
 
 
+def pack_string_vector(vector: List[str]) -> bytes:
+    data = b""
+    data += pack_uint64(len(vector))
+    for value in vector:
+        data += pack_string(value)
+    return data
+
+
 def unpack_bool(data: bytes) -> bool:
     return struct.unpack(">?", data)[0]
 
 
 def unpack_uint64(data: bytes) -> int:
     return struct.unpack(">Q", data)[0]
 
@@ -69,12 +79,12 @@
     lo, hi = hi, hi + 8 * num_seeds
     seed_ids = unpack_uint64_vector(data[lo:hi])
     lo, hi = hi, hi + 8 * num_nodes
     node_ids = unpack_uint64_vector(data[lo:hi])
     lo, hi = hi, hi + 8 * num_edges
     edge_ids = unpack_uint64_vector(data[lo:hi])
 
-    edge_index = list()
-    for _ in range(num_edges):
-        lo, hi = hi, hi + 16
-        edge_index.append(unpack_uint64_vector(data[lo:hi]))
+    edge_index = [
+        unpack_uint64_vector(data[i : i + 16])
+        for i in range(hi, hi + 16 * num_edges, 16)
+    ]
     return Graph(seed_ids, node_ids, edge_ids, edge_index)
```

### Comparing `pymilldb-0.0.5/src/pymilldb.egg-info/PKG-INFO` & `pymilldb-0.0.6/src/pymilldb.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymilldb
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python library for MillenniumDB
 Home-page: https://github.com/MillenniumDB/PyMillDB
 Author: Vicente Calisto
 Author-email: vecalisto@uc.cl
 Project-URL: Bug Tracker, https://github.com/MillenniumDB/PyMillDB/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

