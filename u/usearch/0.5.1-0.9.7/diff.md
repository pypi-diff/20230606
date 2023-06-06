# Comparing `tmp/usearch-0.5.1-cp39-cp39-win_amd64.whl.zip` & `tmp/usearch-0.9.7-cp39-cp39-manylinux_2_28_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,16 @@
-Zip file size: 136394 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat        0 b- defN 23-May-19 00:53 usearch/__init__.py
--rw-rw-rw-  2.0 fat     1462 b- defN 23-May-19 00:53 usearch/client.py
--rw-rw-rw-  2.0 fat   284160 b- defN 23-May-19 01:01 usearch/index.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2298 b- defN 23-May-19 00:53 usearch/io.py
--rw-rw-rw-  2.0 fat     2748 b- defN 23-May-19 00:53 usearch/server.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-May-19 01:01 usearch-0.5.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    19489 b- defN 23-May-19 01:01 usearch-0.5.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-19 01:01 usearch-0.5.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-19 01:01 usearch-0.5.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      770 b- defN 23-May-19 01:01 usearch-0.5.1.dist-info/RECORD
-10 files, 322593 bytes uncompressed, 135098 bytes compressed:  58.1%
+Zip file size: 280689 bytes, number of entries: 14
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-26 22:22 usearch/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-26 22:22 usearch-0.9.7.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-26 22:22 usearch./
+-rwxr-xr-x  2.0 unx   450521 b- defN 23-May-26 22:22 usearch/index.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx     4207 b- defN 23-May-26 22:22 usearch/client.py
+-rw-r--r--  2.0 unx     4075 b- defN 23-May-26 22:22 usearch/server.py
+-rw-r--r--  2.0 unx     2231 b- defN 23-May-26 22:22 usearch/io.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-26 22:22 usearch/__init__.py
+-rw-r--r--  2.0 unx        8 b- defN 23-May-26 22:22 usearch-0.9.7.dist-info/top_level.txt
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-26 22:22 usearch-0.9.7.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      886 b- defN 23-May-26 22:22 usearch-0.9.7.dist-info/RECORD
+-rw-r--r--  2.0 unx    19393 b- defN 23-May-26 22:22 usearch-0.9.7.dist-info/METADATA
+-rw-r--r--  2.0 unx      112 b- defN 23-May-26 22:22 usearch-0.9.7.dist-info/WHEEL
+-rwxr-xr-x  2.0 unx   253289 b- defN 23-May-26 22:22 usearch./libgomp-2c51bfab.so.1.0.0
+14 files, 746079 bytes uncompressed, 278915 bytes compressed:  62.6%
```

## zipnote {}

```diff
@@ -1,31 +1,43 @@
-Filename: usearch/__init__.py
+Filename: usearch/
+Comment: 
+
+Filename: usearch-0.9.7.dist-info/
+Comment: 
+
+Filename: usearch./
+Comment: 
+
+Filename: usearch/index.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
 Filename: usearch/client.py
 Comment: 
 
-Filename: usearch/index.cp39-win_amd64.pyd
+Filename: usearch/server.py
 Comment: 
 
 Filename: usearch/io.py
 Comment: 
 
-Filename: usearch/server.py
+Filename: usearch/__init__.py
+Comment: 
+
+Filename: usearch-0.9.7.dist-info/top_level.txt
 Comment: 
 
-Filename: usearch-0.5.1.dist-info/LICENSE
+Filename: usearch-0.9.7.dist-info/LICENSE
 Comment: 
 
-Filename: usearch-0.5.1.dist-info/METADATA
+Filename: usearch-0.9.7.dist-info/RECORD
 Comment: 
 
-Filename: usearch-0.5.1.dist-info/WHEEL
+Filename: usearch-0.9.7.dist-info/METADATA
 Comment: 
 
-Filename: usearch-0.5.1.dist-info/top_level.txt
+Filename: usearch-0.9.7.dist-info/WHEEL
 Comment: 
 
-Filename: usearch-0.5.1.dist-info/RECORD
+Filename: usearch./libgomp-2c51bfab.so.1.0.0
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## usearch/client.py

```diff
@@ -1,50 +1,127 @@
-import numpy as np
-from ucall.client import Client
-
-
-class IndexClient:
-
-    def __init__(self, uri: str = '127.0.0.1', port: int = 8545, use_http: bool = True) -> None:
-        self.client = Client(uri=uri, port=port, use_http=use_http)
-
-    def add(self, labels: np.array, vectors: np.array):
-        if isinstance(labels, int):
-            self.client.add_one(label=labels, vectors=vectors)
-        else:
-            self.client.add_many(labels=labels, vectors=vectors)
-
-    def search(self, vectors: np.array, count: int) -> tuple[np.array, np.array, np.array]:
-        matches = []
-        distances = []
-        counts = []
-        # return self.client.search_one(vectors=vectors, count=count)
-        return matches, distances, counts
-
-    def __len__(self):
-        return self.client.size()
-
-    @property
-    def ndim(self):
-        return self.client.ndim()
-
-    def capacity(self):
-        return self.client.capacity()
-
-    def connectivity(self):
-        return self.client.connectivity()
-
-    def load(self, path: str):
-        raise NotImplementedError()
-
-    def view(self, path: str):
-        raise NotImplementedError()
-
-    def save(self, path: str):
-        raise NotImplementedError()
-
-
-if __name__ == '__main__':
-    index = IndexClient()
-    index.add(42, np.array([0.4] * 256, dtype=np.float32))
-    results = index.search(np.array([0.4] * 256, dtype=np.float32), 10)
-    print(results)
+from typing import Union, Optional
+
+import numpy as np
+from ucall.client import Client
+
+
+def _vector_to_ascii(vector: np.ndarray) -> Optional[str]:
+    if vector.dtype != np.int8 and vector.dtype != np.uint8 and vector.dtype != np.byte:
+        return None
+    if not np.all((vector >= 0) | (vector <= 100)):
+        return None
+
+    # Let's map [0, 100] to the range from [23, 123],
+    # poking 60 and replacing with the 124.
+    vector += 23
+    vector[vector == 60] = 124
+    ascii = str(vector)
+    return ascii
+
+
+Triplet = tuple[np.ndarray, np.ndarray, np.ndarray]
+
+
+class IndexClient:
+
+    def __init__(
+            self,
+            uri: str = '127.0.0.1',
+            port: int = 8545,
+            use_http: bool = True) -> None:
+        self.client = Client(uri=uri, port=port, use_http=use_http)
+
+    def add_one(self, label: int, vector: np.ndarray):
+        assert isinstance(label, int)
+        assert isinstance(vector, np.ndarray)
+        vector = vector.flatten()
+        ascii = _vector_to_ascii(vector)
+        if ascii:
+            self.client.add_ascii(label=label, string=ascii)
+        else:
+            self.client.add_one(label=label, vectors=vector)
+
+    def add_many(self, labels: np.ndarray, vectors: np.ndarray):
+        assert isinstance(labels, int)
+        assert isinstance(vectors, np.ndarray)
+        assert labels.ndim == 1 and vectors.ndim == 2
+        assert labels.shape[0] == vectors.shape[0]
+        self.client.add_many(labels=labels, vectors=vectors)
+
+    def add(self, labels: Union[np.ndarray, int], vectors: np.ndarray):
+        if isinstance(labels, int) or len(labels) == 1:
+            return self.add_one(labels, vectors)
+        else:
+            return self.add_many(labels, vectors)
+
+    def search_one(self, vector: np.ndarray, count: int) -> Triplet:
+        matches: list[dict] = []
+        vector = vector.flatten()
+        ascii = _vector_to_ascii(vector)
+        if ascii:
+            matches = self.client.search_ascii(string=ascii, count=count)
+        else:
+            matches = self.client.search_one(vector=vector, count=count)
+
+        print(matches.data)
+        matches = matches.json
+
+        labels = np.array((1, count), dtype=np.uint32)
+        distances = np.array((1, count), dtype=np.float32)
+        counts = np.array((1), dtype=np.uint32)
+        for col, result in enumerate(matches):
+            labels[0, col] = result['label']
+            distances[0, col] = result['distance']
+        counts[0] = len(matches)
+
+        return labels, distances, counts
+
+    def search_many(self, vectors: np.ndarray, count: int) -> Triplet:
+        batch_size: int = vectors.shape[0]
+        list_of_matches: list[list[dict]] = self.client.search_many(
+            vectors=vectors, count=count)
+
+        labels = np.array((batch_size, count), dtype=np.uint32)
+        distances = np.array((batch_size, count), dtype=np.float32)
+        counts = np.array((batch_size), dtype=np.uint32)
+        for row, matches in enumerate(list_of_matches):
+            for col, result in enumerate(matches):
+                labels[row, col] = result['label']
+                distances[row, col] = result['distance']
+            counts[row] = len(results)
+
+        return labels, distances, counts
+
+    def search(self, vectors: np.ndarray, count: int) -> Triplet:
+        if vectors.ndim == 1 or (vectors.ndim == 2 and vectors.shape[0] == 1):
+            return self.search_one(vectors, count)
+        else:
+            return self.search_many(vectors, count)
+
+    def __len__(self):
+        return self.client.size().json()
+
+    @property
+    def ndim(self):
+        return self.client.ndim().json()
+
+    def capacity(self):
+        return self.client.capacity().json()
+
+    def connectivity(self):
+        return self.client.connectivity().json()
+
+    def load(self, path: str):
+        raise NotImplementedError()
+
+    def view(self, path: str):
+        raise NotImplementedError()
+
+    def save(self, path: str):
+        raise NotImplementedError()
+
+
+if __name__ == '__main__':
+    index = IndexClient()
+    index.add(42, np.array([0.4] * 256, dtype=np.float32))
+    results = index.search(np.array([0.4] * 256, dtype=np.float32), 10)
+    print(results)
```

## usearch/io.py

 * *Ordering differences only*

```diff
@@ -1,67 +1,67 @@
-import struct
-import numpy as np
-
-
-def load_matrix(filename: str, start_row: int = 0, count_rows: int = None, view: bool = False):
-    """
-    Read *.ibin, *.hbin, *.fbin, *.dbin files with matrixes.
-    Args:
-        :param filename (str): path to the matrix file
-        :param start_row (int): start reading vectors from this index
-        :param count_rows (int): number of vectors to read. If None, read all vectors
-    Returns:
-        Parsed matrix (numpy.ndarray)
-    """
-    dtype = np.float32
-    scalar_size = 4
-    if filename.endswith('.fbin'):
-        dtype = np.float32
-        scalar_size = 4
-    elif filename.endswith('.dbin'):
-        dtype = np.float64
-        scalar_size = 8
-    elif filename.endswith('.hbin'):
-        dtype = np.float16
-        scalar_size = 2
-    elif filename.endswith('.ibin'):
-        dtype = np.int32
-        scalar_size = 4
-    else:
-        raise Exception('Unknown file type')
-
-    with open(filename, 'rb') as f:
-        rows, cols = np.fromfile(f, count=2, dtype=np.int32)
-        rows = (rows - start_row) if count_rows is None else count_rows
-        row_offset = start_row * scalar_size * cols
-
-        if view:
-            return np.memmap(f, dtype=dtype, mode='r', offset=8+row_offset, shape=(rows, cols))
-        else:
-            return np.fromfile(f, count=rows * cols, dtype=dtype, offset=row_offset).reshape(rows, cols)
-
-
-def save_matrix(vecs: np.array, filename: str):
-    """
-    Write *.ibin, *.hbin, *.fbin, *.dbin files with matrixes.
-    Args:
-        :param vecs (numpy.array): the matrix to serialize
-        :param filename (str): path to the matrix file
-    """
-    dtype = np.float32
-    if filename.endswith('.fbin'):
-        dtype = np.float32
-    elif filename.endswith('.dbin'):
-        dtype = np.float64
-    elif filename.endswith('.hbin'):
-        dtype = np.float16
-    elif filename.endswith('.ibin'):
-        dtype = np.int32
-    else:
-        raise Exception('Unknown file type')
-
-    assert len(vecs.shape) == 2, 'Input array must have 2 dimensions'
-    with open(filename, 'wb') as f:
-        nvecs, dim = vecs.shape
-        f.write(struct.pack('<i', nvecs))
-        f.write(struct.pack('<i', dim))
-        vecs.astype(dtype).flatten().tofile(f)
+import struct
+import numpy as np
+
+
+def load_matrix(filename: str, start_row: int = 0, count_rows: int = None, view: bool = False):
+    """
+    Read *.ibin, *.hbin, *.fbin, *.dbin files with matrixes.
+    Args:
+        :param filename (str): path to the matrix file
+        :param start_row (int): start reading vectors from this index
+        :param count_rows (int): number of vectors to read. If None, read all vectors
+    Returns:
+        Parsed matrix (numpy.ndarray)
+    """
+    dtype = np.float32
+    scalar_size = 4
+    if filename.endswith('.fbin'):
+        dtype = np.float32
+        scalar_size = 4
+    elif filename.endswith('.dbin'):
+        dtype = np.float64
+        scalar_size = 8
+    elif filename.endswith('.hbin'):
+        dtype = np.float16
+        scalar_size = 2
+    elif filename.endswith('.ibin'):
+        dtype = np.int32
+        scalar_size = 4
+    else:
+        raise Exception('Unknown file type')
+
+    with open(filename, 'rb') as f:
+        rows, cols = np.fromfile(f, count=2, dtype=np.int32)
+        rows = (rows - start_row) if count_rows is None else count_rows
+        row_offset = start_row * scalar_size * cols
+
+        if view:
+            return np.memmap(f, dtype=dtype, mode='r', offset=8+row_offset, shape=(rows, cols))
+        else:
+            return np.fromfile(f, count=rows * cols, dtype=dtype, offset=row_offset).reshape(rows, cols)
+
+
+def save_matrix(vecs: np.array, filename: str):
+    """
+    Write *.ibin, *.hbin, *.fbin, *.dbin files with matrixes.
+    Args:
+        :param vecs (numpy.array): the matrix to serialize
+        :param filename (str): path to the matrix file
+    """
+    dtype = np.float32
+    if filename.endswith('.fbin'):
+        dtype = np.float32
+    elif filename.endswith('.dbin'):
+        dtype = np.float64
+    elif filename.endswith('.hbin'):
+        dtype = np.float16
+    elif filename.endswith('.ibin'):
+        dtype = np.int32
+    else:
+        raise Exception('Unknown file type')
+
+    assert len(vecs.shape) == 2, 'Input array must have 2 dimensions'
+    with open(filename, 'wb') as f:
+        nvecs, dim = vecs.shape
+        f.write(struct.pack('<i', nvecs))
+        f.write(struct.pack('<i', dim))
+        vecs.astype(dtype).flatten().tofile(f)
```

## usearch/server.py

```diff
@@ -1,95 +1,136 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-import os
-import argparse
-import numpy as np
-
-from ucall.rich_posix import Server
-from usearch.index import Index
-
-
-def serve(
-        ndim: int, metric: str = 'ip',
-        port: int = 8545, threads: int = 1,
-        path: str = 'index.usearch', immutable: bool = False):
-
-    server = Server(port=port)
-    index = Index(ndim=ndim, metric=metric)
-
-    if os.path.exists(path):
-        if immutable:
-            index.view(path)
-        else:
-            index.load(path)
-
-    @server
-    def add_one(label: int, vector: np.array):
-        labels = np.array([label], dtype=np.longlong)
-        vectors = vector.reshape(vector.shape[0], 1)
-        index.add(labels, vectors, copy=True)
-
-    @server
-    def add_many(labels: np.array, vectors: np.array):
-        labels = labels.astype(np.longlong)
-        index.add(labels, vectors, threads=threads, copy=True)
-
-    @server
-    def search_one(vector: np.array, count: int) -> np.ndarray:
-        vectors = vector.reshape(vector.shape[0], 1)
-        results = index.search(vectors, 3)
-        return results[0][:results[2][0]]
-
-    @server
-    def size() -> int:
-        return len(index)
-
-    @server
-    def ndim() -> int:
-        return index.ndim
-
-    @server
-    def capacity() -> int:
-        return index.capacity()
-
-    @server
-    def connectivity() -> int:
-        return index.connectivity()
-
-    try:
-        server.run()
-    except KeyboardInterrupt:
-        if not immutable:
-            index.save(path)
-
-
-if __name__ == '__main__':
-
-    parser = argparse.ArgumentParser()
-    parser.add_argument('-v', '--verbose', help='log server activity')
-    parser.add_argument(
-        '--ndim', type=int,
-        help='dimensionality of the vectors')
-    parser.add_argument(
-        '--immutable', type=bool, default=False,
-        help='the index can not be updated')
-
-    parser.add_argument(
-        '--metric', type=str, default='ip', choices=['ip', 'cos', 'l2', 'haversine'],
-        help='distance function to compare vectors')
-    parser.add_argument(
-        '-p', '--port', type=int, default=8545,
-        help='port to open for client connections')
-    parser.add_argument(
-        '-j', '--threads', type=int, default=1,
-        help='number of CPU threads to use')
-    parser.add_argument(
-        '--path', type=str, default='index.usearch',
-        help='where to store the index')
-
-    args = parser.parse_args()
-    assert args.ndim is not None, 'Define the number of dimensions!'
-    serve(
-        ndim=args.ndim, metric=args.metric,
-        threads=args.threads, port=args.port,
-        path=args.path, immutable=args.immutable)
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+import os
+import argparse
+import numpy as np
+
+from ucall.rich_posix import Server
+from usearch.index import Index
+
+Triplet = tuple[np.ndarray, np.ndarray, np.ndarray]
+
+
+def _results_to_json(results: Triplet, row: int) -> list[dict]:
+
+    count = results[2][row]
+    labels = results[0][row, :count]
+    distances = results[1][row, :count]
+    return [{'label': int(label), 'distance': float(distance)}
+            for label, distance in zip(labels, distances)]
+
+
+def _ascii_to_vector(string: str) -> np.ndarray:
+    """
+    WARNING: A dirty performance hack!
+    Assuming the `f8` vectors in our implementations are just integers,
+    and generally contain scalars in the [0, 100] range, we can transmit
+    them as JSON-embedded strings. The only symbols we must avoid are
+    the double-quote '"' (code 22) and backslash '\' (code 60).
+    Printable ASCII characters are in [20, 126].
+    """
+    vector = np.array(string, dtype=np.int8)
+    vector[vector == 124] = 60
+    vector -= 23
+    return vector
+
+
+def serve(
+        ndim_: int, metric: str = 'ip',
+        port: int = 8545, threads: int = 1,
+        path: str = 'index.usearch', immutable: bool = False):
+
+    server = Server(port=port)
+    index = Index(ndim=ndim_, metric=metric)
+
+    if os.path.exists(path):
+        if immutable:
+            index.view(path)
+        else:
+            index.load(path)
+
+    @server
+    def size() -> int:
+        return len(index)
+
+    @server
+    def ndim() -> int:
+        return index.ndim
+
+    @server
+    def capacity() -> int:
+        return index.capacity()
+
+    @server
+    def connectivity() -> int:
+        return index.connectivity()
+
+    @server
+    def add_one(label: int, vector: np.ndarray):
+        print('adding', label, vector)
+        labels = np.array([label], dtype=np.longlong)
+        vectors = vector.flatten().reshape(vector.shape[0], 1)
+        index.add(labels, vectors)
+
+    @server
+    def add_many(labels: np.ndarray, vectors: np.ndarray):
+        labels = labels.astype(np.longlong)
+        index.add(labels, vectors, threads=threads)
+
+    @server
+    def search_one(vector: np.ndarray, count: int) -> list[dict]:
+        print('search', vector, count)
+        vectors = vector.reshape(vector.shape[0], 1)
+        results = index.search(vectors, count)
+        return _results_to_json(results, 0)
+
+    @server
+    def search_many(vectors: np.ndarray, count: int) -> list[list[dict]]:
+        results = index.search(vectors, count)
+        return [_results_to_json(results, i) for i in range(vectors.shape[0])]
+
+    @server
+    def add_ascii(label: int, string: str):
+        return add_one(label, _ascii_to_vector(string))
+
+    @server
+    def search_ascii(string: str, count: int):
+        return search_one(_ascii_to_vector(string), count)
+
+    try:
+        server.run()
+    except KeyboardInterrupt:
+        if not immutable:
+            index.save(path)
+
+
+if __name__ == '__main__':
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument('-v', '--verbose', help='log server activity')
+    parser.add_argument(
+        '--ndim', type=int,
+        help='dimensionality of the vectors')
+    parser.add_argument(
+        '--immutable', type=bool, default=False,
+        help='the index can not be updated')
+
+    parser.add_argument(
+        '--metric', type=str, default='ip', choices=['ip', 'cos', 'l2sq', 'haversine'],
+        help='distance function to compare vectors')
+    parser.add_argument(
+        '-p', '--port', type=int, default=8545,
+        help='port to open for client connections')
+    parser.add_argument(
+        '-j', '--threads', type=int, default=1,
+        help='number of CPU threads to use')
+    parser.add_argument(
+        '--path', type=str, default='index.usearch',
+        help='where to store the index')
+
+    args = parser.parse_args()
+    assert args.ndim is not None, 'Define the number of dimensions!'
+    serve(
+        ndim_=args.ndim, metric=args.metric,
+        threads=args.threads, port=args.port,
+        path=args.path, immutable=args.immutable)
```

## Comparing `usearch-0.5.1.dist-info/LICENSE` & `usearch-0.9.7.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

## Comparing `usearch-0.5.1.dist-info/METADATA` & `usearch-0.9.7.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,522 +1,528 @@
-Metadata-Version: 2.1
-Name: usearch
-Version: 0.5.1
-Summary: Smaller & Faster Single-File Vector Search Engine from Unum
-License: Apache-2.0
-Classifier: Development Status :: 4 - Beta
-Classifier: Natural Language :: English
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: C++
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Unix
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Topic :: System :: Clustering
-Classifier: Topic :: Database :: Database Engines/Servers
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<h1 align="center">USearch</h1>
-<h3 align="center">
-Smaller & Faster Single-File<br/>
-Vector Search Engine<br/>
-</h3>
-<br/>
-
-<p align="center">
-<a href="https://discord.gg/A6wxt6dS9j"><img height="25" src="https://github.com/unum-cloud/.github/raw/main/assets/discord.svg" alt="Discord"></a>
-&nbsp;&nbsp;&nbsp;
-<a href="https://www.linkedin.com/company/unum-cloud/"><img height="25" src="https://github.com/unum-cloud/.github/raw/main/assets/linkedin.svg" alt="LinkedIn"></a>
-&nbsp;&nbsp;&nbsp;
-<a href="https://twitter.com/unum_cloud"><img height="25" src="https://github.com/unum-cloud/.github/raw/main/assets/twitter.svg" alt="Twitter"></a>
-&nbsp;&nbsp;&nbsp;
-<a href="https://unum.cloud/post"><img height="25" src="https://github.com/unum-cloud/.github/raw/main/assets/blog.svg" alt="Blog"></a>
-&nbsp;&nbsp;&nbsp;
-<a href="https://github.com/unum-cloud/usearch"><img height="25" src="https://github.com/unum-cloud/.github/raw/main/assets/github.svg" alt="GitHub"></a>
-</p>
-
-<p align="center">
-Euclidean • Angular • Jaccard • Hamming • Haversine • User-Defined Metrics
-<br/>
-<a href="#c++">C++11</a> •
-<a href="#python">Python</a> •
-<a href="#javascript">JavaScript</a> •
-<a href="#java">Java</a> •
-<a href="#rust">Rust</a> •
-<a href="#objective-c">Objective-C</a> •
-<a href="#swift">Swift</a> •
-<a href="#golang">GoLang</a> •
-<a href="#wolfram">Wolfram</a>
-<br/>
-Linux • MacOS • Windows
-</p>
-
----
-
-- [x] Industry-leading [performance](#performance).
-- [x] Easily-extendible [single C++11 header][usearch-header] implementation.
-- [x] [User-defined](#define-custom-metrics) and pre-packaged SIMD-accelerated metrics.
-- [x] [Half-precision `f16` and Quarter-precision `f8`](#quantize-on-the-fly) support on any hardware.
-- [x] [View from disk](#view-larger-indexes-from-disk), without loading into RAM.
-- [x] [4B+](#go-beyond-4b-entries) sized space efficient point-clouds with `uint40_t`.
-- [x] Variable dimensionality vectors - for [obscure use-cases][obscure-use-cases].
-- [x] [Bring your threads](#bring-your-threads), like OpenMP.
-- [x] Multiple vectors per label.
-- [ ] Thread-safe `reserve`.
-- [x] AI + Vector Search = [Semantic Search](#ai--vector-search--semantic-search).
-
-[usearch-header]: https://github.com/unum-cloud/usearch/blob/main/include/usearch/usearch.hpp
-[obscure-use-cases]: https://ashvardanian.com/posts/abusing-vector-search
-
----
-
-|                    | FAISS                         | USearch                            |
-| :----------------- | :---------------------------- | :--------------------------------- |
-| Implementation     | 84 K [SLOC][sloc] in `faiss/` | 1 K [SLOC][sloc] in `usearch/`     |
-| Supported metrics  | 9 fixed metrics               | Any User-Defined metrics           |
-| Supported ID types | `uint32_t`, `uint64_t`        | `uint32_t`, `uint40_t`, `uint64_t` |
-| Dependencies       | BLAS, OpenMP                  | None                               |
-| Bindings           | SWIG                          | Native                             |
-| Acceleration       | Learned Quantization          | Downcasting                        |
-
-FAISS is the industry standard for a high-performance batteries-included vector search engine.
-Both USearch and FAISS implement the same HNSW algorithm.
-But they differ in a lot of design decisions.
-USearch is designed to be compact and broadly compatible without sacrificing performance.
-
-|            | FAISS, `f32` | USearch, `f32` | USearch, `f16` | USearch, `f8` |
-| :--------- | -----------: | -------------: | -------------: | ------------: |
-| Insertions |       76 K/s |         89 K/s |         73 K/s |   **137 K/s** |
-| Queries    |      118 K/s |        167 K/s |        140 K/s |   **281 K/s** |
-| Recall @1  |          99% |          99.2% |            98% |     **99.2%** |
-
-> Dataset: 1M vectors sample of the Deep1B dataset.
-> Hardware: `c7g.metal` AWS instance with 64 cores and DDR5 memory.
-> HNSW was configured with identical hyper-parameters:
-> connectivity `M=16`,
-> expansion @ construction `efConstruction=128`,
-> and expansion @ search `ef=64`.
-> Both libraries were compiled for the target architecture.
-> Jump to the [Performance Tuning][benchmarking] section to read about the effects of those hyper-parameters.
-
-[sloc]: https://en.wikipedia.org/wiki/Source_lines_of_code
-[benchmarking]: https://github.com/unum-cloud/usearch/blob/main/docs/benchmarks.md
-
-## User-Defined Functions
-
-Most vector-search packages focus on just 2 metrics - "Inner Product distance" and "Euclidean distance".
-That only partially exhausts the list of possible metrics.
-A good example would be the rare [Haversine][haversine] distance, used to compute the distance between geo-spatial coordinates, extending Vector Search into the GIS domain.
-Another example would be designing a custom metric for **composite embeddings** concatenated from multiple AI models in real-world applications. 
-USearch supports that: [Python](#user-defined-functions-in-python) and [C++](#user-defined-functions-in-c) examples.
-
-![USearch: Vector Search Approaches](https://github.com/unum-cloud/usearch/blob/main/assets/usearch-approaches-white.png?raw=true)
-
-Unlike older approaches indexing high-dimensional spaces, like KD-Trees and Locality Sensitive Hashing, HNSW doesn't require vectors to be identical in length.
-They only have to be comparable.
-So you can apply it in [obscure][obscure] applications, like searching for similar sets or fuzzy text matching.
-
-[haversine]: https://ashvardanian.com/posts/abusing-vector-search#geo-spatial-indexing
-[obscure]: https://ashvardanian.com/posts/abusing-vector-search
-
-## Memory Efficiency, Downcasting, and Quantization
-
-Training a quantization model and dimension-reduction is a common approach to accelerate vector search.
-Those, however, are only sometimes reliable, can significantly affect the statistical properties of your data, and require regular adjustments if your distribution shifts.
-
-![USearch uint40_t support](https://github.com/unum-cloud/usearch/blob/main/assets/usearch-neighbor-types.png?raw=true)
-
-Instead, we have focused on high-precision arithmetic over low-precision downcasted vectors.
-The same index, and `add` and `search` operations will automatically down-cast or up-cast between `f32_t`, `f16_t`, `f64_t`, and `f8_t` representations, even if the hardware doesn't natively support it.
-Continuing the topic of memory-efficiency, we provide a `uint40_t` to allow collection with over 4B+ vectors without allocating 8 bytes for every neighbor reference in the proximity graph.
-
-## View Larger Indexes from Disk
-
-Modern search systems often suggest using different servers to maximize indexing speed and minimize serving costs.
-Memory-optimized for the first task, and storage-optimized for the second, if the index can be served from external memory, which USearch can.
-
-|          |    To Build     |        To Serve        |
-| :------- | :-------------: | :--------------------: |
-| Instance |  u-24tb1.metal  |     is4gen.8xlarge     |
-| Price    |    ~ $200/h     |        ~$4.5/h         |
-| Memory   | 24 TB RAM + EBS | 192 GB RAM + 30 TB SSD |
-
-There is a 50x difference between the cost of such instances for identical capacity.
-Of course, the latency of external memory access will be higher, but it is in part compensated with an excellent prefetching mechanism.
-
-## Usage
-
-There are two usage patters:
-
-1. Bare-bones with `usearch/usearch.hpp`, only available in C++.
-2. Full-fat version with it's own threads, mutexes, type-punning, quantization, that is available both in C++ and is wrapped for higher-level bindings.
-
-### C++
-
-#### Installation
-
-To use in a C++ project simply copy the `include/usearch/usearch.hpp` header into your project.
-Alternatively fetch it with CMake:
-
-```cmake
-FetchContent_Declare(usearch GIT_REPOSITORY https://github.com/unum-cloud/usearch.git)
-FetchContent_MakeAvailable(usearch)
-```
-
-#### Quickstart
-
-Once included, the low-level C++11 interface is as simple as it gets: `reserve()`, `add()`, `search()`, `size()`, `capacity()`, `save()`, `load()`, `view()`.
-This covers 90% of use-cases.
-
-```c++
-using namespace unum::usearch;
-
-index_gt<cos_gt<float>> index;
-float vec[3] = {0.1, 0.3, 0.2};
-
-index.reserve(10);
-index.add(/* label: */ 42, /* vector: */ {&vec, 3});
-index.search(
-  /* query: */ {&vec, 3}, /* top */ 5 /* results */,
-  /* with callback: */ [](std::size_t label, float distance) { });
-```
-
-The `add` is thread-safe for concurrent index construction.
-
-#### Serialization
-
-```c++
-index.save("index.usearch");
-index.load("index.usearch"); // Copying from disk
-index.view("index.usearch"); // Memory-mapping from disk
-```
-
-#### User-Defined Metrics in C++
-
-For advanced users, more compile-time abstractions are available.
-
-```cpp
-template <typename metric_at = ip_gt<float>,            //
-          typename label_at = std::size_t,              // `uint32_t`, `uuid_t`...
-          typename id_at = std::uint32_t,               // `uint40_t`, `uint64_t`...
-          typename scalar_at = float,                   // `double`, `half`, `char`...
-          typename allocator_at = std::allocator<char>> //
-class index_gt;
-```
-
-You may want to use a custom memory allocator or a rare scalar type, but most often, you would start by defining a custom similarity measure.
-The function object should have the following signature to support different-length vectors.
-
-```cpp
-struct custom_metric_t {
-    T operator()(T const* a, T const* b, std::size_t a_length, std::size_t b_length) const;
-};
-```
-
-The following distances are pre-packaged:
-
-- `cos_gt<scalar_t>` for "Cosine" or "Angular" distance.
-- `ip_gt<scalar_t>` for "Inner Product" or "Dot Product" distance.
-- `l2sq_gt<scalar_t>` for the squared "L2" or "Euclidean" distance.
-- `jaccard_gt<scalar_t>` for "Jaccard" distance between two ordered sets of unique elements.
-- `bit_hamming_gt<scalar_t>` for "Hamming" distance, as the number of shared bits in hashes.
-- `pearson_correlation_gt<scalar_t>` for "Pearson" correlation between probability distributions.
-- `haversine_gt<scalar_t>` for "Haversine" or "Great Circle" distance between coordinates.
-
-#### Multi-Threading
-
-Most AI, HPC, or Big Data packages use some form of a thread pool.
-Instead of spawning additional threads within USearch, we focus on the thread safety of `add()` function, simplifying resource management.
-
-```cpp
-#pragma omp parallel for
-    for (std::size_t i = 0; i < n; ++i)
-        native.add(label, span_t{vector, dims}, add_config_t { .thread = omp_get_thread_num() });
-```
-
-During initialization, we allocate enough temporary memory for all the cores on the machine.
-On the call, the user can supply the identifier of the current thread, making this library easy to integrate with OpenMP and similar tools.
-
-### Python
-
-#### Installation
-
-```sh
-pip install usearch
-```
-
-#### Quickstart
-
-```python
-import numpy as np
-from usearch.index import Index
-
-index = Index(
-    ndim=3, # Define the number of dimensions in input vectors
-    metric='cos', # Choose 'l2', 'haversine' or other metric, default = 'ip'
-    dtype='f32', # Quantize to 'f16' or 'f8' if needed, default = 'f32'
-    connectivity=16, # How frequent should the connections in the graph be, optional
-    expansion_add=128, # Control the recall of indexing, optional
-    expansion_search=64, # Control the quality of search, optional
-)
-
-vector = np.array([0.2, 0.6, 0.4], dtype=np.float32)
-index.add(42, vector)
-matches, distances, count = index.search(vector, 10)
-
-assert len(index) == 1
-assert count == 1
-assert matches[0] == 42
-assert distances[0] <= 0.001
-```
-
-Python bindings are implemented with [`pybind/pybind11`](https://github.com/pybind/pybind11).
-Assuming the presence of Global Interpreter Lock in Python, we spawn threads in the C++ layer on large insertions.
-
-#### Serialization
-
-```py
-index.save('index.usearch')
-index.load('index.usearch') # Copy the whole index into memory
-index.view('index.usearch') # View from disk without loading in memory
-```
-
-#### Batch Operations
-
-Adding or querying a batch of entries is identical to adding a single vector.
-The difference would be in the shape of the tensors.
-
-```py
-n = 100
-labels = np.array(range(n), dtype=np.longlong)
-vectors = np.random.uniform(0, 0.3, (n, index.ndim)).astype(np.float32)
-
-index.add(labels, vectors, threads=..., copy=...)
-matches, distances, counts = index.search(vectors, 10, threads=...)
-
-assert matches.shape[0] == vectors.shape[0]
-assert counts[0] <= 10
-```
-
-You can also override the default `threads` and `copy` arguments in bulk workloads.
-The first controls the number of threads spawned for the task.
-The second controls whether the vector itself will be persisted inside the index.
-If you can preserve the lifetime of the vector somewhere else, you can avoid the copy.
-
-#### User-Defined Metrics in Python
-
-Assuming the language boundary exists between Python user code and C++ implementation, there are more efficient solutions than passing a Python callable to the engine.
-Luckily, with the help of [Numba][numba], we can JIT compile a function with a matching signature and pass it down to the engine.
-
-```py
-from numba import cfunc, types, carray
-
-signature = types.float32(
-    types.CPointer(types.float32),
-    types.CPointer(types.float32),
-    types.size_t, types.size_t)
-
-@cfunc(signature)
-def python_dot(a, b, n, m):
-    a_array = carray(a, n)
-    b_array = carray(b, n)
-    c = 0.0
-    for i in range(n):
-        c += a_array[i] * b_array[i]
-    return c
-
-index = Index(ndim=ndim, metric_pointer=python_dot.address)
-```
-
-[numba]: https://numba.readthedocs.io/en/stable/reference/jit-compilation.html#c-callbacks
-
-#### Tooling
-
-```py
-from usearch.index import Index
-from usearch.io import load_matrix, save_matrix
-
-vectors = load_matrix('deep1B.fbin')
-index = Index(ndim=vectors.shape[1])
-index.add(labels, vectors)
-```
-
-### JavaScript
-
-#### Installation
-
-```sh
-npm install usearch
-```
-
-#### Quickstart
-
-```js
-var index = new usearch.Index({ metric: 'cos', connectivity: 16, dimensions: 3 })
-index.add(42, new Float32Array([0.2, 0.6, 0.4]))
-var results = index.search(new Float32Array([0.2, 0.6, 0.4]), 10)
-
-assert.equal(index.size(), 1)
-assert.deepEqual(results.labels, new Uint32Array([42]))
-assert.deepEqual(results.distances, new Float32Array([0]))
-```
-
-#### Serialization
-
-```js
-index.save('index.usearch')
-index.load('index.usearch')
-index.view('index.usearch')
-```
-
-### Rust
-
-#### Installation
-
-```sh
-cargo add usearch
-```
-
-#### Quickstart
-
-```rust
-let quant: &str = "f16";
-let index = new_ip(3, &quant, 0, 0, 0).unwrap();
-
-assert!(index.reserve(10).is_ok());
-assert!(index.capacity() >= 10);
-assert!(index.connectivity() != 0);
-assert_eq!(index.dimensions(), 3);
-assert_eq!(index.size(), 0);
-
-let first: [f32; 3] = [0.2, 0.1, 0.2];
-let second: [f32; 3] = [0.2, 0.1, 0.2];
-
-assert!(index.add(42, &first).is_ok());
-assert!(index.add(43, &second).is_ok());
-assert_eq!(index.size(), 2);
-
-// Read back the tags
-let results = index.search(&first, 10).unwrap();
-assert_eq!(results.count, 2);
-```
-
-#### Multi-Threading
-
-```rust
-assert!(index.add_in_thread(42, &first, 0).is_ok());
-assert!(index.add_in_thread(43, &second, 0).is_ok());
-let results = index.search_in_thread(&first, 10, 0).unwrap();
-```
-
-Being a systems-programming language, Rust has better control over memory management and concurrency but lacks function overloading.
-Aside from the `add` and `search`, USearch Rust binding also provides `add_in_thread` and `search_in_thread`, which let users identify the calling thread to use underlying temporary memory more efficiently.
-
-#### Serialization
-
-```rust
-assert!(index.save("index.usearch").is_ok());
-assert!(index.load("index.usearch").is_ok());
-assert!(index.view("index.usearch").is_ok());
-```
-
-#### Metrics
-
-```rust
-assert!(new_l2(3, &quant, 0, 0, 0).is_ok());
-assert!(new_cos(3, &quant, 0, 0, 0).is_ok());
-assert!(new_haversine(&quant, 0, 0, 0).is_ok());
-```
-
-### Java
-
-#### Installation
-
-```xml
-<dependency>
-  <groupId>cloud.unum.usearch</groupId>
-  <artifactId>usearch</artifactId>
-  <version>0.2.3</version>
-</dependency>
-```
-
-Add that snippet to your `pom.xml` and hit `mvn install`.
-
-#### Quickstart
-
-```java
-Index index = new Index.Config().metric("cos").dimensions(2).build();
-float vec[] = {10, 20};
-index.add(42, vec);
-int[] labels = index.search(vec, 5);
-```
-
-### Swift
-
-#### Installation
-
-```txt
-https://github.com/unum-cloud/usearch
-```
-
-#### Quickstart
-
-```swift
-let index = Index.l2(dimensions: 3, connectivity: 8)
-let vectorA: [Float32] = [0.3, 0.5, 1.2]
-let vectorB: [Float32] = [0.4, 0.2, 1.2]
-index.add(label: 42, vector: vectorA[...])
-index.add(label: 43, vector: vectorB[...])
-
-let results = index.search(vector: vectorA[...], count: 10)
-assert(results.0[0] == 42)
-```
-
-### GoLang
-
-### Wolfram
-
-## TODO
-
-- JavaScript: Allow calling from "worker threads".
-- Rust: Allow passing a custom thread ID.
-- C# .NET bindings.
-
-## AI + Vector Search = Semantic Search
-
-AI has a growing number of applications, but one of the coolest classic ideas is to use it for Semantic Search.
-One can take an encoder model, like the multi-modal UForm, and a web-programming framework, like UCall, and build an image search platform in just 20 lines of Python.
-
-```python
-import ucall.rich_posix as ucall
-import uform
-from usearch.index import Index
-
-import numpy as np
-from PIL import Image
-
-server = ucall.Server()
-model = uform.get_model('unum-cloud/uform-vl-multilingual')
-index = Index(ndim=256)
-
-@server
-def add(label: int, photo: Image.Image):
-    image = model.preprocess_image(photo)
-    vector = model.encode_image(image).detach().numpy()
-    index.add(label, vector.flatten(), copy=True)
-
-@server
-def search(query: str) -> np.ndarray:
-    tokens = model.preprocess_text(query)
-    vector = model.encode_text(tokens).detach().numpy()
-    neighbors, _, _ = index.search(vector.flatten(), 3)
-    return neighbors
-
-server.run()
-```
-
-Check [that](https://github.com/ashvardanian/image-search) and [other](https://github.com/unum-cloud/examples) examples on our corporate GitHub 🤗
+Metadata-Version: 2.1
+Name: usearch
+Version: 0.9.7
+Summary: Smaller & Faster Single-File Vector Search Engine from Unum
+License: Apache-2.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Natural Language :: English
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: C++
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Java
+Classifier: Programming Language :: JavaScript
+Classifier: Programming Language :: Objective C
+Classifier: Programming Language :: Rust
+Classifier: Programming Language :: Other
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Unix
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Topic :: System :: Clustering
+Classifier: Topic :: Database :: Database Engines/Servers
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h1 align="center">USearch</h1>
+<h3 align="center">
+Smaller & Faster Single-File<br/>
+Vector Search Engine<br/>
+</h3>
+<br/>
+
+<p align="center">
+<a href="https://discord.gg/A6wxt6dS9j"><img height="25" src="https://github.com/unum-cloud/.github/raw/main/assets/discord.svg" alt="Discord"></a>
+&nbsp;&nbsp;&nbsp;
+<a href="https://www.linkedin.com/company/unum-cloud/"><img height="25" src="https://github.com/unum-cloud/.github/raw/main/assets/linkedin.svg" alt="LinkedIn"></a>
+&nbsp;&nbsp;&nbsp;
+<a href="https://twitter.com/unum_cloud"><img height="25" src="https://github.com/unum-cloud/.github/raw/main/assets/twitter.svg" alt="Twitter"></a>
+&nbsp;&nbsp;&nbsp;
+<a href="https://unum.cloud/post"><img height="25" src="https://github.com/unum-cloud/.github/raw/main/assets/blog.svg" alt="Blog"></a>
+&nbsp;&nbsp;&nbsp;
+<a href="https://github.com/unum-cloud/usearch"><img height="25" src="https://github.com/unum-cloud/.github/raw/main/assets/github.svg" alt="GitHub"></a>
+</p>
+
+<p align="center">
+Euclidean • Angular • Jaccard • Hamming • Haversine • User-Defined Metrics
+<br/>
+<a href="#c++">C++11</a> •
+<a href="#python">Python</a> •
+<a href="#javascript">JavaScript</a> •
+<a href="#java">Java</a> •
+<a href="#rust">Rust</a> •
+<a href="#objective-c">Objective-C</a> •
+<a href="#swift">Swift</a> •
+<a href="#golang">GoLang</a> •
+<a href="#wolfram">Wolfram</a>
+<br/>
+Linux • MacOS • Windows
+</p>
+
+---
+
+- [x] Industry-leading [performance](#performance).
+- [x] Easily-extendible [single C++11 header][usearch-header] implementation.
+- [x] [User-defined](#define-custom-metrics) and pre-packaged SIMD-accelerated metrics.
+- [x] [Half-precision `f16` and Quarter-precision `f8`](#quantize-on-the-fly) support on any hardware.
+- [x] [View from disk](#view-larger-indexes-from-disk), without loading into RAM.
+- [x] [4B+](#go-beyond-4b-entries) sized space efficient point-clouds with `uint40_t`.
+- [x] Variable dimensionality vectors - for [obscure use-cases][obscure-use-cases].
+- [x] [Bring your threads](#bring-your-threads), like OpenMP.
+- [x] Multiple vectors per label.
+- [ ] Thread-safe `reserve`.
+- [x] AI + Vector Search = [Semantic Search](#ai--vector-search--semantic-search).
+
+[usearch-header]: https://github.com/unum-cloud/usearch/blob/main/include/usearch/usearch.hpp
+[obscure-use-cases]: https://ashvardanian.com/posts/abusing-vector-search
+
+---
+
+|                    | FAISS                         | USearch                            |
+| :----------------- | :---------------------------- | :--------------------------------- |
+| Implementation     | 84 K [SLOC][sloc] in `faiss/` | 1 K [SLOC][sloc] in `usearch/`     |
+| Supported metrics  | 9 fixed metrics               | Any User-Defined metrics           |
+| Supported ID types | `uint32_t`, `uint64_t`        | `uint32_t`, `uint40_t`, `uint64_t` |
+| Dependencies       | BLAS, OpenMP                  | None                               |
+| Bindings           | SWIG                          | Native                             |
+| Acceleration       | Learned Quantization          | Downcasting                        |
+
+FAISS is the industry standard for a high-performance batteries-included vector search engine.
+Both USearch and FAISS implement the same HNSW algorithm.
+But they differ in a lot of design decisions.
+USearch is designed to be compact and broadly compatible without sacrificing performance.
+
+|            | FAISS, `f32` | USearch, `f32` | USearch, `f16` | USearch, `f8` | USearch + Numba, `f32` |
+| :--------- | -----------: | -------------: | -------------: | ------------: | ---------------------: |
+| Insertions |       76 K/s |         89 K/s |         73 K/s |   **137 K/s** |                 99 K/s |
+| Queries    |      118 K/s |        167 K/s |        140 K/s |   **281 K/s** |                165 K/s |
+| Recall @1  |          99% |          99.2% |            98% |     **99.2%** |                  99.2% |
+
+> Dataset: 1M vectors sample of the Deep1B dataset.
+> Hardware: `c7g.metal` AWS instance with 64 cores and DDR5 memory.
+> HNSW was configured with identical hyper-parameters:
+> connectivity `M=16`,
+> expansion @ construction `efConstruction=128`,
+> and expansion @ search `ef=64`.
+> Both libraries were compiled for the target architecture.
+> Jump to the [Performance Tuning][benchmarking] section to read about the effects of those hyper-parameters.
+
+[sloc]: https://en.wikipedia.org/wiki/Source_lines_of_code
+[benchmarking]: https://github.com/unum-cloud/usearch/blob/main/docs/benchmarks.md
+
+## User-Defined Functions
+
+Most vector-search packages focus on just 2 metrics - "Inner Product distance" and "Euclidean distance".
+That only partially exhausts the list of possible metrics.
+A good example would be the rare [Haversine][haversine] distance, used to compute the distance between geo-spatial coordinates, extending Vector Search into the GIS domain.
+Another example would be designing a custom metric for **composite embeddings** concatenated from multiple AI models in real-world applications. 
+USearch supports that: [Python](#user-defined-functions-in-python) and [C++](#user-defined-functions-in-c) examples.
+
+![USearch: Vector Search Approaches](https://github.com/unum-cloud/usearch/blob/main/assets/usearch-approaches-white.png?raw=true)
+
+Unlike older approaches indexing high-dimensional spaces, like KD-Trees and Locality Sensitive Hashing, HNSW doesn't require vectors to be identical in length.
+They only have to be comparable.
+So you can apply it in [obscure][obscure] applications, like searching for similar sets or fuzzy text matching.
+
+[haversine]: https://ashvardanian.com/posts/abusing-vector-search#geo-spatial-indexing
+[obscure]: https://ashvardanian.com/posts/abusing-vector-search
+
+## Memory Efficiency, Downcasting, and Quantization
+
+Training a quantization model and dimension-reduction is a common approach to accelerate vector search.
+Those, however, are only sometimes reliable, can significantly affect the statistical properties of your data, and require regular adjustments if your distribution shifts.
+
+![USearch uint40_t support](https://github.com/unum-cloud/usearch/blob/main/assets/usearch-neighbor-types.png?raw=true)
+
+Instead, we have focused on high-precision arithmetic over low-precision downcasted vectors.
+The same index, and `add` and `search` operations will automatically down-cast or up-cast between `f32_t`, `f16_t`, `f64_t`, and `f8_t` representations, even if the hardware doesn't natively support it.
+Continuing the topic of memory-efficiency, we provide a `uint40_t` to allow collection with over 4B+ vectors without allocating 8 bytes for every neighbor reference in the proximity graph.
+
+## View Larger Indexes from Disk
+
+Modern search systems often suggest using different servers to maximize indexing speed and minimize serving costs.
+Memory-optimized for the first task, and storage-optimized for the second, if the index can be served from external memory, which USearch can.
+
+|          |    To Build     |        To Serve        |
+| :------- | :-------------: | :--------------------: |
+| Instance |  u-24tb1.metal  |     is4gen.8xlarge     |
+| Price    |    ~ $200/h     |        ~$4.5/h         |
+| Memory   | 24 TB RAM + EBS | 192 GB RAM + 30 TB SSD |
+
+There is a 50x difference between the cost of such instances for identical capacity.
+Of course, the latency of external memory access will be higher, but it is in part compensated with an excellent prefetching mechanism.
+
+## Usage
+
+There are two usage patters:
+
+1. Bare-bones with `usearch/usearch.hpp`, only available in C++.
+2. Full-fat version with it's own threads, mutexes, type-punning, quantization, that is available both in C++ and is wrapped for higher-level bindings.
+
+### C++
+
+#### Installation
+
+To use in a C++ project simply copy the `include/usearch/usearch.hpp` header into your project.
+Alternatively fetch it with CMake:
+
+```cmake
+FetchContent_Declare(usearch GIT_REPOSITORY https://github.com/unum-cloud/usearch.git)
+FetchContent_MakeAvailable(usearch)
+```
+
+#### Quickstart
+
+Once included, the low-level C++11 interface is as simple as it gets: `reserve()`, `add()`, `search()`, `size()`, `capacity()`, `save()`, `load()`, `view()`.
+This covers 90% of use-cases.
+
+```c++
+using namespace unum::usearch;
+
+index_gt<cos_gt<float>> index;
+float vec[3] = {0.1, 0.3, 0.2};
+
+index.reserve(10);
+index.add(/* label: */ 42, /* vector: */ {&vec[0], 3});
+auto results = index.search(/* query: */ {&vec[0], 3}, 5 /* neighbors */);
+
+for (std::size_t i = 0; i != results.size(); ++i)
+    results[i].member.label, results[i].member.vector, results[i].distance;
+```
+
+The `add` is thread-safe for concurrent index construction.
+
+#### Serialization
+
+```c++
+index.save("index.usearch");
+index.load("index.usearch"); // Copying from disk
+index.view("index.usearch"); // Memory-mapping from disk
+```
+
+#### User-Defined Metrics in C++
+
+For advanced users, more compile-time abstractions are available.
+
+```cpp
+template <typename metric_at = ip_gt<float>,            //
+          typename label_at = std::size_t,              // `uint32_t`, `uuid_t`...
+          typename id_at = std::uint32_t,               // `uint40_t`, `uint64_t`...
+          typename scalar_at = float,                   // `double`, `half`, `char`...
+          typename allocator_at = std::allocator<char>> //
+class index_gt;
+```
+
+You may want to use a custom memory allocator or a rare scalar type, but most often, you would start by defining a custom similarity measure.
+The function object should have the following signature to support different-length vectors.
+
+```cpp
+struct custom_metric_t {
+    T operator()(T const* a, T const* b, std::size_t a_length, std::size_t b_length) const;
+};
+```
+
+The following distances are pre-packaged:
+
+- `cos_gt<scalar_t>` for "Cosine" or "Angular" distance.
+- `ip_gt<scalar_t>` for "Inner Product" or "Dot Product" distance.
+- `l2sq_gt<scalar_t>` for the squared "L2" or "Euclidean" distance.
+- `jaccard_gt<scalar_t>` for "Jaccard" distance between two ordered sets of unique elements.
+- `bit_hamming_gt<scalar_t>` for "Hamming" distance, as the number of shared bits in hashes.
+- `pearson_correlation_gt<scalar_t>` for "Pearson" correlation between probability distributions.
+- `haversine_gt<scalar_t>` for "Haversine" or "Great Circle" distance between coordinates.
+
+#### Multi-Threading
+
+Most AI, HPC, or Big Data packages use some form of a thread pool.
+Instead of spawning additional threads within USearch, we focus on the thread safety of `add()` function, simplifying resource management.
+
+```cpp
+#pragma omp parallel for
+    for (std::size_t i = 0; i < n; ++i)
+        native.add(label, span_t{vector, dims}, add_config_t { .thread = omp_get_thread_num() });
+```
+
+During initialization, we allocate enough temporary memory for all the cores on the machine.
+On the call, the user can supply the identifier of the current thread, making this library easy to integrate with OpenMP and similar tools.
+
+### Python
+
+#### Installation
+
+```sh
+pip install usearch
+```
+
+#### Quickstart
+
+```python
+import numpy as np
+from usearch.index import Index
+
+index = Index(
+    ndim=3, # Define the number of dimensions in input vectors
+    metric='cos', # Choose 'l2sq', 'haversine' or other metric, default = 'ip'
+    dtype='f32', # Quantize to 'f16' or 'f8' if needed, default = 'f32'
+    connectivity=16, # How frequent should the connections in the graph be, optional
+    expansion_add=128, # Control the recall of indexing, optional
+    expansion_search=64, # Control the quality of search, optional
+)
+
+vector = np.array([0.2, 0.6, 0.4], dtype=np.float32)
+index.add(42, vector)
+matches, distances, count = index.search(vector, 10)
+
+assert len(index) == 1
+assert count == 1
+assert matches[0] == 42
+assert distances[0] <= 0.001
+```
+
+Python bindings are implemented with [`pybind/pybind11`](https://github.com/pybind/pybind11).
+Assuming the presence of Global Interpreter Lock in Python, we spawn threads in the C++ layer on large insertions.
+
+#### Serialization
+
+```py
+index.save('index.usearch')
+index.load('index.usearch') # Copy the whole index into memory
+index.view('index.usearch') # View from disk without loading in memory
+```
+
+#### Batch Operations
+
+Adding or querying a batch of entries is identical to adding a single vector.
+The difference would be in the shape of the tensors.
+
+```py
+n = 100
+labels = np.array(range(n), dtype=np.longlong)
+vectors = np.random.uniform(0, 0.3, (n, index.ndim)).astype(np.float32)
+
+index.add(labels, vectors, threads=..., copy=...)
+matches, distances, counts = index.search(vectors, 10, threads=...)
+
+assert matches.shape[0] == vectors.shape[0]
+assert counts[0] <= 10
+```
+
+You can also override the default `threads` and `copy` arguments in bulk workloads.
+The first controls the number of threads spawned for the task.
+The second controls whether the vector itself will be persisted inside the index.
+If you can preserve the lifetime of the vector somewhere else, you can avoid the copy.
+
+#### User-Defined Metrics in Python
+
+Assuming the language boundary exists between Python user code and C++ implementation, there are more efficient solutions than passing a Python callable to the engine.
+Luckily, with the help of [Numba][numba], we can JIT compile a function with a matching signature and pass it down to the engine.
+
+```py
+from numba import cfunc, types, carray
+
+signature = types.float32(
+    types.CPointer(types.float32),
+    types.CPointer(types.float32),
+    types.size_t, types.size_t)
+
+@cfunc(signature)
+def python_dot(a, b, n, m):
+    a_array = carray(a, n)
+    b_array = carray(b, n)
+    c = 0.0
+    for i in range(n):
+        c += a_array[i] * b_array[i]
+    return c
+
+index = Index(ndim=ndim, metric_pointer=python_dot.address)
+```
+
+[numba]: https://numba.readthedocs.io/en/stable/reference/jit-compilation.html#c-callbacks
+
+#### Tooling
+
+```py
+from usearch.index import Index
+from usearch.io import load_matrix, save_matrix
+
+vectors = load_matrix('deep1B.fbin')
+index = Index(ndim=vectors.shape[1])
+index.add(labels, vectors)
+```
+
+### JavaScript
+
+#### Installation
+
+```sh
+npm install usearch
+```
+
+#### Quickstart
+
+```js
+var index = new usearch.Index({ metric: 'cos', connectivity: 16, dimensions: 3 })
+index.add(42, new Float32Array([0.2, 0.6, 0.4]))
+var results = index.search(new Float32Array([0.2, 0.6, 0.4]), 10)
+
+assert.equal(index.size(), 1)
+assert.deepEqual(results.labels, new Uint32Array([42]))
+assert.deepEqual(results.distances, new Float32Array([0]))
+```
+
+#### Serialization
+
+```js
+index.save('index.usearch')
+index.load('index.usearch')
+index.view('index.usearch')
+```
+
+### Rust
+
+#### Installation
+
+```sh
+cargo add usearch
+```
+
+#### Quickstart
+
+```rust
+let quant: &str = "f16";
+let index = new_ip(3, &quant, 0, 0, 0).unwrap();
+
+assert!(index.reserve(10).is_ok());
+assert!(index.capacity() >= 10);
+assert!(index.connectivity() != 0);
+assert_eq!(index.dimensions(), 3);
+assert_eq!(index.size(), 0);
+
+let first: [f32; 3] = [0.2, 0.1, 0.2];
+let second: [f32; 3] = [0.2, 0.1, 0.2];
+
+assert!(index.add(42, &first).is_ok());
+assert!(index.add(43, &second).is_ok());
+assert_eq!(index.size(), 2);
+
+// Read back the tags
+let results = index.search(&first, 10).unwrap();
+assert_eq!(results.count, 2);
+```
+
+#### Multi-Threading
+
+```rust
+assert!(index.add_in_thread(42, &first, 0).is_ok());
+assert!(index.add_in_thread(43, &second, 0).is_ok());
+let results = index.search_in_thread(&first, 10, 0).unwrap();
+```
+
+Being a systems-programming language, Rust has better control over memory management and concurrency but lacks function overloading.
+Aside from the `add` and `search`, USearch Rust binding also provides `add_in_thread` and `search_in_thread`, which let users identify the calling thread to use underlying temporary memory more efficiently.
+
+#### Serialization
+
+```rust
+assert!(index.save("index.usearch").is_ok());
+assert!(index.load("index.usearch").is_ok());
+assert!(index.view("index.usearch").is_ok());
+```
+
+#### Metrics
+
+```rust
+assert!(new_l2sq(3, &quant, 0, 0, 0).is_ok());
+assert!(new_cos(3, &quant, 0, 0, 0).is_ok());
+assert!(new_haversine(&quant, 0, 0, 0).is_ok());
+```
+
+### Java
+
+#### Installation
+
+```xml
+<dependency>
+  <groupId>cloud.unum</groupId>
+  <artifactId>usearch</artifactId>
+  <version>0.2.3</version>
+</dependency>
+```
+
+Add that snippet to your `pom.xml` and hit `mvn install`.
+
+#### Quickstart
+
+```java
+Index index = new Index.Config().metric("cos").dimensions(2).build();
+float vec[] = {10, 20};
+index.add(42, vec);
+int[] labels = index.search(vec, 5);
+```
+
+### Swift
+
+#### Installation
+
+```txt
+https://github.com/unum-cloud/usearch
+```
+
+#### Quickstart
+
+```swift
+let index = Index.l2sq(dimensions: 3, connectivity: 8)
+let vectorA: [Float32] = [0.3, 0.5, 1.2]
+let vectorB: [Float32] = [0.4, 0.2, 1.2]
+index.add(label: 42, vector: vectorA[...])
+index.add(label: 43, vector: vectorB[...])
+
+let results = index.search(vector: vectorA[...], count: 10)
+assert(results.0[0] == 42)
+```
+
+### GoLang
+
+### Wolfram
+
+## TODO
+
+- JavaScript: Allow calling from "worker threads".
+- Rust: Allow passing a custom thread ID.
+- C# .NET bindings.
+
+## AI + Vector Search = Semantic Search
+
+AI has a growing number of applications, but one of the coolest classic ideas is to use it for Semantic Search.
+One can take an encoder model, like the multi-modal UForm, and a web-programming framework, like UCall, and build an image search platform in just 20 lines of Python.
+
+```python
+import ucall.rich_posix as ucall
+import uform
+from usearch.index import Index
+
+import numpy as np
+from PIL import Image
+
+server = ucall.Server()
+model = uform.get_model('unum-cloud/uform-vl-multilingual')
+index = Index(ndim=256)
+
+@server
+def add(label: int, photo: Image.Image):
+    image = model.preprocess_image(photo)
+    vector = model.encode_image(image).detach().numpy()
+    index.add(label, vector.flatten(), copy=True)
+
+@server
+def search(query: str) -> np.ndarray:
+    tokens = model.preprocess_text(query)
+    vector = model.encode_text(tokens).detach().numpy()
+    neighbors, _, _ = index.search(vector.flatten(), 3)
+    return neighbors
+
+server.run()
+```
+
+Check [that](https://github.com/ashvardanian/image-search) and [other](https://github.com/unum-cloud/examples) examples on our corporate GitHub 🤗
```

### html2text {}

```diff
@@ -1,20 +1,22 @@
-Metadata-Version: 2.1 Name: usearch Version: 0.5.1 Summary: Smaller & Faster
+Metadata-Version: 2.1 Name: usearch Version: 0.9.7 Summary: Smaller & Faster
 Single-File Vector Search Engine from Unum License: Apache-2.0 Classifier:
-Development Status :: 4 - Beta Classifier: Natural Language :: English
-Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
-Information Technology Classifier: License :: OSI Approved :: Apache Software
-License Classifier: Programming Language :: Python :: 3 :: Only Classifier:
-Programming Language :: Python :: Implementation :: CPython Classifier:
-Programming Language :: C++ Classifier: Operating System :: MacOS Classifier:
-Operating System :: Unix Classifier: Operating System :: Microsoft :: Windows
-Classifier: Topic :: System :: Clustering Classifier: Topic :: Database ::
-Database Engines/Servers Classifier: Topic :: Scientific/Engineering ::
-Artificial Intelligence Description-Content-Type: text/markdown License-File:
-LICENSE
+Development Status :: 5 - Production/Stable Classifier: Natural Language ::
+English Classifier: Intended Audience :: Developers Classifier: Intended
+Audience :: Information Technology Classifier: License :: OSI Approved ::
+Apache Software License Classifier: Programming Language :: C++ Classifier:
+Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
+Python :: Implementation :: CPython Classifier: Programming Language :: Java
+Classifier: Programming Language :: JavaScript Classifier: Programming Language
+:: Objective C Classifier: Programming Language :: Rust Classifier: Programming
+Language :: Other Classifier: Operating System :: MacOS Classifier: Operating
+System :: Unix Classifier: Operating System :: Microsoft :: Windows Classifier:
+Topic :: System :: Clustering Classifier: Topic :: Database :: Database
+Engines/Servers Classifier: Topic :: Scientific/Engineering :: Artificial
+Intelligence Description-Content-Type: text/markdown License-File: LICENSE
                              ****** USearch ******
                        **** Smaller & Faster Single-File
                              Vector Search Engine
                                       ****
 
         [Discord]     [LinkedIn]     [Twitter]     [Blog]     [GitHub]
  Euclidean â¢ Angular â¢ Jaccard â¢ Hamming â¢ Haversine â¢ User-Defined
@@ -41,18 +43,19 @@
 Supported ID types | `uint32_t`, `uint64_t` | `uint32_t`, `uint40_t`,
 `uint64_t` | | Dependencies | BLAS, OpenMP | None | | Bindings | SWIG | Native
 | | Acceleration | Learned Quantization | Downcasting | FAISS is the industry
 standard for a high-performance batteries-included vector search engine. Both
 USearch and FAISS implement the same HNSW algorithm. But they differ in a lot
 of design decisions. USearch is designed to be compact and broadly compatible
 without sacrificing performance. | | FAISS, `f32` | USearch, `f32` | USearch,
-`f16` | USearch, `f8` | | :--------- | -----------: | -------------: | --------
------: | ------------: | | Insertions | 76 K/s | 89 K/s | 73 K/s | **137 K/s**
-| | Queries | 118 K/s | 167 K/s | 140 K/s | **281 K/s** | | Recall @1 | 99% |
-99.2% | 98% | **99.2%** | > Dataset: 1M vectors sample of the Deep1B dataset. >
+`f16` | USearch, `f8` | USearch + Numba, `f32` | | :--------- | -----------: |
+-------------: | -------------: | ------------: | ---------------------: | |
+Insertions | 76 K/s | 89 K/s | 73 K/s | **137 K/s** | 99 K/s | | Queries | 118
+K/s | 167 K/s | 140 K/s | **281 K/s** | 165 K/s | | Recall @1 | 99% | 99.2% |
+98% | **99.2%** | 99.2% | > Dataset: 1M vectors sample of the Deep1B dataset. >
 Hardware: `c7g.metal` AWS instance with 64 cores and DDR5 memory. > HNSW was
 configured with identical hyper-parameters: > connectivity `M=16`, > expansion
 @ construction `efConstruction=128`, > and expansion @ search `ef=64`. > Both
 libraries were compiled for the target architecture. > Jump to the [Performance
 Tuning][benchmarking] section to read about the effects of those hyper-
 parameters. [sloc]: https://en.wikipedia.org/wiki/Source_lines_of_code
 [benchmarking]: https://github.com/unum-cloud/usearch/blob/main/docs/
@@ -102,17 +105,18 @@
 with CMake: ```cmake FetchContent_Declare(usearch GIT_REPOSITORY https://
 github.com/unum-cloud/usearch.git) FetchContent_MakeAvailable(usearch) ``` ####
 Quickstart Once included, the low-level C++11 interface is as simple as it
 gets: `reserve()`, `add()`, `search()`, `size()`, `capacity()`, `save()`, `load
 ()`, `view()`. This covers 90% of use-cases. ```c++ using namespace unum::
 usearch; index_gt
 float>> index; float vec[3] = {0.1, 0.3, 0.2}; index.reserve(10); index.add(/
-* label: */ 42, /* vector: */ {&vec, 3}); index.search( /* query: */ {&vec, 3},
-/* top */ 5 /* results */, /* with callback: */ [](std::size_t label, float
-distance) { }); ``` The `add` is thread-safe for concurrent index construction.
+* label: */ 42, /* vector: */ {&vec[0], 3}); auto results = index.search(/
+* query: */ {&vec[0], 3}, 5 /* neighbors */); for (std::size_t i = 0; i !=
+results.size(); ++i) results[i].member.label, results[i].member.vector, results
+[i].distance; ``` The `add` is thread-safe for concurrent index construction.
 #### Serialization ```c++ index.save("index.usearch"); index.load
 ("index.usearch"); // Copying from disk index.view("index.usearch"); // Memory-
 mapping from disk ``` #### User-Defined Metrics in C++ For advanced users, more
 compile-time abstractions are available. ```cpp template , // typename label_at
 = std::size_t, // `uint32_t`, `uuid_t`... typename id_at = std::uint32_t, /
 / `uint40_t`, `uint64_t`... typename scalar_at = float, // `double`, `half`,
 `char`... typename allocator_at = std::allocator> // class index_gt; ``` You
@@ -134,15 +138,15 @@
 (std::size_t i = 0; i < n; ++i) native.add(label, span_t{vector, dims},
 add_config_t { .thread = omp_get_thread_num() }); ``` During initialization, we
 allocate enough temporary memory for all the cores on the machine. On the call,
 the user can supply the identifier of the current thread, making this library
 easy to integrate with OpenMP and similar tools. ### Python #### Installation
 ```sh pip install usearch ``` #### Quickstart ```python import numpy as np from
 usearch.index import Index index = Index( ndim=3, # Define the number of
-dimensions in input vectors metric='cos', # Choose 'l2', 'haversine' or other
+dimensions in input vectors metric='cos', # Choose 'l2sq', 'haversine' or other
 metric, default = 'ip' dtype='f32', # Quantize to 'f16' or 'f8' if needed,
 default = 'f32' connectivity=16, # How frequent should the connections in the
 graph be, optional expansion_add=128, # Control the recall of indexing,
 optional expansion_search=64, # Control the quality of search, optional )
 vector = np.array([0.2, 0.6, 0.4], dtype=np.float32) index.add(42, vector)
 matches, distances, count = index.search(vector, 10) assert len(index) == 1
 assert count == 1 assert matches[0] == 42 assert distances[0] <= 0.001 ```
@@ -197,22 +201,22 @@
 language, Rust has better control over memory management and concurrency but
 lacks function overloading. Aside from the `add` and `search`, USearch Rust
 binding also provides `add_in_thread` and `search_in_thread`, which let users
 identify the calling thread to use underlying temporary memory more
 efficiently. #### Serialization ```rust assert!(index.save
 ("index.usearch").is_ok()); assert!(index.load("index.usearch").is_ok());
 assert!(index.view("index.usearch").is_ok()); ``` #### Metrics ```rust assert!
-(new_l2(3, &quant, 0, 0, 0).is_ok()); assert!(new_cos(3, &quant, 0, 0, 0).is_ok
-()); assert!(new_haversine(&quant, 0, 0, 0).is_ok()); ``` ### Java ####
-Installation ```xml  cloud.unum.usearch usearch 0.2.3  ``` Add that snippet to
-your `pom.xml` and hit `mvn install`. #### Quickstart ```java Index index = new
+(new_l2sq(3, &quant, 0, 0, 0).is_ok()); assert!(new_cos(3, &quant, 0, 0,
+0).is_ok()); assert!(new_haversine(&quant, 0, 0, 0).is_ok()); ``` ### Java ####
+Installation ```xml  cloud.unum usearch 0.2.3  ``` Add that snippet to your
+`pom.xml` and hit `mvn install`. #### Quickstart ```java Index index = new
 Index.Config().metric("cos").dimensions(2).build(); float vec[] = {10, 20};
 index.add(42, vec); int[] labels = index.search(vec, 5); ``` ### Swift ####
 Installation ```txt https://github.com/unum-cloud/usearch ``` #### Quickstart
-```swift let index = Index.l2(dimensions: 3, connectivity: 8) let vectorA:
+```swift let index = Index.l2sq(dimensions: 3, connectivity: 8) let vectorA:
 [Float32] = [0.3, 0.5, 1.2] let vectorB: [Float32] = [0.4, 0.2, 1.2] index.add
 (label: 42, vector: vectorA[...]) index.add(label: 43, vector: vectorB[...])
 let results = index.search(vector: vectorA[...], count: 10) assert(results.0[0]
 == 42) ``` ### GoLang ### Wolfram ## TODO - JavaScript: Allow calling from
 "worker threads". - Rust: Allow passing a custom thread ID. - C# .NET bindings.
 ## AI + Vector Search = Semantic Search AI has a growing number of
 applications, but one of the coolest classic ideas is to use it for Semantic
```

