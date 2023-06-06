# Comparing `tmp/miniofs-0.0.4b0-py3-none-any.whl.zip` & `tmp/miniofs-0.0.4b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5334 bytes, number of entries: 8
--rw-rw-r--  2.0 unx      209 b- defN 23-Jan-04 12:55 miniofs/__init__.py
--rw-rw-r--  2.0 unx       79 b- defN 23-Jan-04 12:22 miniofs/config.yml
--rw-rw-r--  2.0 unx     3458 b- defN 23-Jan-04 12:30 miniofs/functional.py
--rw-r--r--  2.0 unx     1079 b- defN 23-Jan-04 12:55 miniofs-0.0.4b0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     4902 b- defN 23-Jan-04 12:55 miniofs-0.0.4b0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jan-04 12:55 miniofs-0.0.4b0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 23-Jan-04 12:55 miniofs-0.0.4b0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      621 b- defN 23-Jan-04 12:55 miniofs-0.0.4b0.dist-info/RECORD
-8 files, 10448 bytes uncompressed, 4250 bytes compressed:  59.3%
+Zip file size: 5685 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx      210 b- defN 23-Jan-04 14:13 miniofs/__init__.py
+-rw-rw-r--  2.0 unx       78 b- defN 23-Jan-04 13:03 miniofs/config.yml
+-rw-rw-r--  2.0 unx     4819 b- defN 23-Jan-04 14:06 miniofs/functional.py
+-rw-r--r--  2.0 unx     1079 b- defN 23-Jan-04 14:13 miniofs-0.0.4b1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     4902 b- defN 23-Jan-04 14:13 miniofs-0.0.4b1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jan-04 14:13 miniofs-0.0.4b1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 23-Jan-04 14:13 miniofs-0.0.4b1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      621 b- defN 23-Jan-04 14:13 miniofs-0.0.4b1.dist-info/RECORD
+8 files, 11809 bytes uncompressed, 4601 bytes compressed:  61.0%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: miniofs/config.yml
 Comment: 
 
 Filename: miniofs/functional.py
 Comment: 
 
-Filename: miniofs-0.0.4b0.dist-info/LICENSE
+Filename: miniofs-0.0.4b1.dist-info/LICENSE
 Comment: 
 
-Filename: miniofs-0.0.4b0.dist-info/METADATA
+Filename: miniofs-0.0.4b1.dist-info/METADATA
 Comment: 
 
-Filename: miniofs-0.0.4b0.dist-info/WHEEL
+Filename: miniofs-0.0.4b1.dist-info/WHEEL
 Comment: 
 
-Filename: miniofs-0.0.4b0.dist-info/top_level.txt
+Filename: miniofs-0.0.4b1.dist-info/top_level.txt
 Comment: 
 
-Filename: miniofs-0.0.4b0.dist-info/RECORD
+Filename: miniofs-0.0.4b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## miniofs/__init__.py

```diff
@@ -1,11 +1,11 @@
 from miniofs.functional import *
 from minio import Minio
 
-__version__ = "0.0.4b"
+__version__ = "0.0.4b1"
 cfg = load_config()
 client = Minio(
     cfg.host,
     secure=False,
     access_key=cfg.username,
     secret_key=cfg.password,
 )
```

## miniofs/config.yml

```diff
@@ -1,4 +1,4 @@
 project: miniofs
-host: 10.1.0.13:9000
+host: 10.1.0.7:9000
 username: minioadmin
 password: minioadmin
```

## miniofs/functional.py

```diff
@@ -1,11 +1,60 @@
 from gnutools.fs import load_config as _load_config, parent
 import os
 from tqdm import tqdm
 import re
+from gnutools.utils import id_generator
+
+
+class Object:
+    def __init__(
+        self,
+        filepath,
+        host=None,
+        username=None,
+        password=None,
+        read_binary=False,
+        secure=False,
+        version_id=0,
+    ):
+        if host is not None:
+            from minio import Minio
+
+            self._client = Minio(
+                host,
+                secure=secure,
+                access_key=username,
+                secret_key=password,
+            )
+        else:
+            from miniofs import client
+
+            self._client = client
+        self._filepath = filepath
+        self._version_id = version_id
+        if read_binary:
+            self._cdata = self.collect()
+        else:
+            self._cdata = None
+
+    def collect(self):
+        if self._filepath.startswith("/zfs/"):
+            filepath = "zfs://" + self._filepath[5:]
+        else:
+            assert self._filepath.startswith("zfs://")
+            filepath = self._filepath
+        output_file = f"/tmp/.miniofs_{id_generator(128)}"
+        bucket, object_name = split_bucket_name(filepath)
+        self._client.fget_object(
+            bucket, object_name, output_file, version_id=self._version_id
+        )
+        binary = open(output_file, "rb").read()
+        os.remove(output_file)
+        self._cdata = binary
+        return self._cdata
 
 
 def load_config():
     filename = f"{parent(__file__)}/config.yml"
     cfg = _load_config(filename)
     return cfg
```

## Comparing `miniofs-0.0.4b0.dist-info/LICENSE` & `miniofs-0.0.4b1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `miniofs-0.0.4b0.dist-info/METADATA` & `miniofs-0.0.4b1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniofs
-Version: 0.0.4b0
+Version: 0.0.4b1
 Summary: Minio Tools for python
 Home-page: https://github.com/JeanMaximilienCadic/miniofs
 Author: Jean Maximilien Cadic
 Author-email: git@cadic.jp
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
```

### html2text {}

```diff
@@ -1,6 +1,6 @@
-Metadata-Version: 2.1 Name: miniofs Version: 0.0.4b0 Summary: Minio Tools for
+Metadata-Version: 2.1 Name: miniofs Version: 0.0.4b1 Summary: Minio Tools for
 python Home-page: https://github.com/JeanMaximilienCadic/miniofs Author: Jean
 Maximilien Cadic Author-email: git@cadic.jp License: MIT Classifier:
 Programming Language :: Python :: 3.6 Classifier: License :: OSI Approved ::
 MIT License Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: minio Requires-Dist: gnutools-python
```

