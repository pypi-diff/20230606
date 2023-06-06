# Comparing `tmp/milvus-ingestion-0.3.0.tar.gz` & `tmp/milvus-ingestion-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "milvus-ingestion-0.3.0.tar", last modified: Thu May 18 06:19:07 2023, max compression
+gzip compressed data, was "milvus-ingestion-0.4.0.tar", last modified: Tue Jun  6 13:25:11 2023, max compression
```

## Comparing `milvus-ingestion-0.3.0.tar` & `milvus-ingestion-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxr-x   0 yhmo      (1000) yhmo      (1000)        0 2023-05-18 06:19:07.653404 milvus-ingestion-0.3.0/
--rw-rw-r--   0 yhmo      (1000) yhmo      (1000)    11357 2023-05-12 02:28:50.000000 milvus-ingestion-0.3.0/LICENSE
--rw-rw-r--   0 yhmo      (1000) yhmo      (1000)     1908 2023-05-18 06:19:07.653404 milvus-ingestion-0.3.0/PKG-INFO
--rw-rw-r--   0 yhmo      (1000) yhmo      (1000)     1337 2023-05-18 06:02:05.000000 milvus-ingestion-0.3.0/README.md
-drwxrwxr-x   0 yhmo      (1000) yhmo      (1000)        0 2023-05-18 06:19:07.649404 milvus-ingestion-0.3.0/milvus_ingestion/
--rw-rw-r--   0 yhmo      (1000) yhmo      (1000)      993 2023-05-18 05:52:29.000000 milvus-ingestion-0.3.0/milvus_ingestion/__init__.py
--rw-rw-r--   0 yhmo      (1000) yhmo      (1000)      712 2023-05-18 05:52:29.000000 milvus-ingestion-0.3.0/milvus_ingestion/constants.py
--rw-rw-r--   0 yhmo      (1000) yhmo      (1000)    13111 2023-05-18 05:52:29.000000 milvus-ingestion-0.3.0/milvus_ingestion/data_buffer.py
--rw-rw-r--   0 yhmo      (1000) yhmo      (1000)     3716 2023-05-18 05:52:29.000000 milvus-ingestion-0.3.0/milvus_ingestion/milvus_connector.py
--rw-rw-r--   0 yhmo      (1000) yhmo      (1000)     3159 2023-05-18 05:52:29.000000 milvus-ingestion-0.3.0/milvus_ingestion/uploader.py
--rw-rw-r--   0 yhmo      (1000) yhmo      (1000)     1292 2023-05-18 05:52:29.000000 milvus-ingestion-0.3.0/milvus_ingestion/util.py
-drwxrwxr-x   0 yhmo      (1000) yhmo      (1000)        0 2023-05-18 06:19:07.653404 milvus-ingestion-0.3.0/milvus_ingestion.egg-info/
--rw-rw-r--   0 yhmo      (1000) yhmo      (1000)     1908 2023-05-18 06:19:07.000000 milvus-ingestion-0.3.0/milvus_ingestion.egg-info/PKG-INFO
--rw-rw-r--   0 yhmo      (1000) yhmo      (1000)      407 2023-05-18 06:19:07.000000 milvus-ingestion-0.3.0/milvus_ingestion.egg-info/SOURCES.txt
--rw-rw-r--   0 yhmo      (1000) yhmo      (1000)        1 2023-05-18 06:19:07.000000 milvus-ingestion-0.3.0/milvus_ingestion.egg-info/dependency_links.txt
--rw-rw-r--   0 yhmo      (1000) yhmo      (1000)       44 2023-05-18 06:19:07.000000 milvus-ingestion-0.3.0/milvus_ingestion.egg-info/requires.txt
--rw-rw-r--   0 yhmo      (1000) yhmo      (1000)       17 2023-05-18 06:19:07.000000 milvus-ingestion-0.3.0/milvus_ingestion.egg-info/top_level.txt
--rw-rw-r--   0 yhmo      (1000) yhmo      (1000)       38 2023-05-18 06:19:07.653404 milvus-ingestion-0.3.0/setup.cfg
--rw-rw-r--   0 yhmo      (1000) yhmo      (1000)      946 2023-05-18 06:05:22.000000 milvus-ingestion-0.3.0/setup.py
+drwxr-xr-x   0 michaelmo   (501) staff       (20)        0 2023-06-06 13:25:11.877547 milvus-ingestion-0.4.0/
+-rw-r--r--   0 michaelmo   (501) staff       (20)    11357 2023-06-04 15:51:31.000000 milvus-ingestion-0.4.0/LICENSE
+-rw-r--r--   0 michaelmo   (501) staff       (20)     4235 2023-06-06 13:25:11.877101 milvus-ingestion-0.4.0/PKG-INFO
+-rw-r--r--   0 michaelmo   (501) staff       (20)     3663 2023-06-06 13:21:56.000000 milvus-ingestion-0.4.0/README.md
+drwxr-xr-x   0 michaelmo   (501) staff       (20)        0 2023-06-06 13:25:11.874669 milvus-ingestion-0.4.0/milvus_ingestion/
+-rw-r--r--   0 michaelmo   (501) staff       (20)      969 2023-06-06 13:21:56.000000 milvus-ingestion-0.4.0/milvus_ingestion/__init__.py
+-rw-r--r--   0 michaelmo   (501) staff       (20)    17876 2023-06-06 13:21:56.000000 milvus-ingestion-0.4.0/milvus_ingestion/buffer.py
+-rw-r--r--   0 michaelmo   (501) staff       (20)      973 2023-06-06 13:21:56.000000 milvus-ingestion-0.4.0/milvus_ingestion/constants.py
+-rw-r--r--   0 michaelmo   (501) staff       (20)    14361 2023-06-06 13:21:56.000000 milvus-ingestion-0.4.0/milvus_ingestion/data_buffer.py
+-rw-r--r--   0 michaelmo   (501) staff       (20)     2665 2023-06-06 13:21:56.000000 milvus-ingestion-0.4.0/milvus_ingestion/data_info.py
+-rw-r--r--   0 michaelmo   (501) staff       (20)     7631 2023-06-06 13:21:56.000000 milvus-ingestion-0.4.0/milvus_ingestion/milvus_connector.py
+-rw-r--r--   0 michaelmo   (501) staff       (20)     5355 2023-06-06 13:21:56.000000 milvus-ingestion-0.4.0/milvus_ingestion/uploader.py
+-rw-r--r--   0 michaelmo   (501) staff       (20)     1424 2023-06-06 13:21:56.000000 milvus-ingestion-0.4.0/milvus_ingestion/util.py
+drwxr-xr-x   0 michaelmo   (501) staff       (20)        0 2023-06-06 13:25:11.876588 milvus-ingestion-0.4.0/milvus_ingestion.egg-info/
+-rw-r--r--   0 michaelmo   (501) staff       (20)     4235 2023-06-06 13:25:11.000000 milvus-ingestion-0.4.0/milvus_ingestion.egg-info/PKG-INFO
+-rw-r--r--   0 michaelmo   (501) staff       (20)      464 2023-06-06 13:25:11.000000 milvus-ingestion-0.4.0/milvus_ingestion.egg-info/SOURCES.txt
+-rw-r--r--   0 michaelmo   (501) staff       (20)        1 2023-06-06 13:25:11.000000 milvus-ingestion-0.4.0/milvus_ingestion.egg-info/dependency_links.txt
+-rw-r--r--   0 michaelmo   (501) staff       (20)       63 2023-06-06 13:25:11.000000 milvus-ingestion-0.4.0/milvus_ingestion.egg-info/requires.txt
+-rw-r--r--   0 michaelmo   (501) staff       (20)       17 2023-06-06 13:25:11.000000 milvus-ingestion-0.4.0/milvus_ingestion.egg-info/top_level.txt
+-rw-r--r--   0 michaelmo   (501) staff       (20)       38 2023-06-06 13:25:11.877677 milvus-ingestion-0.4.0/setup.cfg
+-rw-r--r--   0 michaelmo   (501) staff       (20)      976 2023-06-06 13:21:56.000000 milvus-ingestion-0.4.0/setup.py
```

### Comparing `milvus-ingestion-0.3.0/LICENSE` & `milvus-ingestion-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `milvus-ingestion-0.3.0/milvus_ingestion/__init__.py` & `milvus-ingestion-0.4.0/milvus_ingestion/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,38 +6,36 @@
 # Unless required by applicable law or agreed to in writing, software distributed under the License
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
 
 from .constants import (
     IngestionType,
+    CleanDataOptions,
 )
 
 from .util import (
     Base,
     default_logger,
 )
 
 from .milvus_connector import (
     MilvusConnector,
     default_milvus,
 )
 
 from .uploader import (
-    Uploader,
+    MinioUploader,
     default_uploader,
 )
 
 from .data_buffer import (
     DataBuffer,
 )
 
 __all__ = [
     'IngestionType',
-    'Base',
-    'default_logger',
     'MilvusConnector',
-    'default_milvus',
-    'Uploader',
-    'default_uploader',
+    'MinioUploader',
     'DataBuffer',
+    'CleanDataOptions',
 ]
```

### Comparing `milvus-ingestion-0.3.0/milvus_ingestion/data_buffer.py` & `milvus-ingestion-0.4.0/milvus_ingestion/data_buffer.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,342 +4,373 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
 
-import json
-import time
 import os
-import numpy
+import shutil
+from typing import List
 
 from logging import Logger
+from threading import Lock
 
-from pymilvus import (
-    DataType,
-)
+from pymilvus import BulkInsertState
 
 from .util import (
     Base,
     default_logger,
 )
 
 from .constants import (
     IngestionType,
+    CleanDataOptions,
     OUTPUT_FOLDER,
+    DEFAULT_PARTITION_NAME,
     MB,
     GB,
 )
 
 from .milvus_connector import (
     MilvusConnector,
     default_milvus,
 )
 
 from .uploader import (
     Uploader,
     default_uploader,
 )
 
+from.buffer import (
+    MultiBuffer,
+)
+
+from .data_info import (
+    DATAINFO_FILE_NAME,
+    DataInfo,
+)
+
 
 class DataBuffer(Base):
     def __init__(
             self,
+            target_collection: str,
+            local_data_path: str = OUTPUT_FOLDER,
             milvus_connector: MilvusConnector = default_milvus,
             uploader: Uploader = default_uploader,
-            ingestion_type: IngestionType = IngestionType.ROW_BASED,
+            ingestion_type: IngestionType = IngestionType.COLUMN_BASED,
             logger: Logger = default_logger(),
         ):
+        self._args_check(target_collection, local_data_path, milvus_connector, uploader, ingestion_type)
         super().__init__(logger=logger)
+        self._local_data_path = local_data_path
         self._milvus_connector = milvus_connector
         self._uploader = uploader
         self._ingestion_type = ingestion_type
-        self._target_collection_schema = None
-        self._target_fields = {}
-        self._output_folder = OUTPUT_FOLDER
-        self._data_size_per_block = 1*GB
-        self._buffer_size = 0
-        self._buffer = {}
-        if self._ingestion_type == IngestionType.ROW_BASED:
-            self._buffer = []
-
-        self._default_values = {
-            DataType.BOOL.name: False,
-            DataType.INT8.name: 0,
-            DataType.INT16.name: 0,
-            DataType.INT32.name: 0,
-            DataType.INT64.name: 0,
-            DataType.FLOAT.name: 0.0,
-            DataType.DOUBLE.name: 0,
-            DataType.VARCHAR.name: "",
-        }
-
-        self._type_size = {
-            DataType.BOOL.name: 1,
-            DataType.INT8.name: 8,
-            DataType.INT16.name: 8,
-            DataType.INT32.name: 8,
-            DataType.INT64.name: 8,
-            DataType.FLOAT.name: 8,
-            DataType.DOUBLE.name: 8,
-        }
-
-        self._type_validator = {
-            DataType.BOOL.name: lambda x: isinstance(x, bool),
-            DataType.INT8.name: lambda x: isinstance(x, int) and -128 <= x <= 127,
-            DataType.INT16.name: lambda x: isinstance(x, int) and -32768 <= x <= 32767,
-            DataType.INT32.name: lambda x: isinstance(x, int) and -2147483648 <= x <= 2147483647,
-            DataType.INT64.name: lambda x: isinstance(x, int),
-            DataType.FLOAT.name: lambda x: isinstance(x, float),
-            DataType.DOUBLE.name: lambda x: isinstance(x, float),
-            DataType.VARCHAR.name: lambda x, l: isinstance(x, str) and len(x) <= l,
-            DataType.FLOAT_VECTOR.name: lambda x, dim: isinstance(x, list) and len(x) == dim,
-            DataType.BINARY_VECTOR.name: lambda x, dim: isinstance(x, bytes) and len(x)*8 == dim
-        }
-
-    def set_output_folder(self, folder: str):
-        self._output_folder = folder
-
-    def set_data_size_per_block(self, data_size: int):
-        if data_size <= 0:
-            data_size = 512*MB
-        self._data_size_per_block = data_size
-
-    def set_default_value(self, data_type: DataType, val)->bool:
-        if data_type == DataType.BINARY_VECTOR or data_type == DataType.FLOAT_VECTOR:
-            self._print_err("Cannot set default value for vector type")
-            return False
-        if val is None:
-            self._print_err("Not support None default value")
-            return False
-        self._default_values[data_type.name] = val
-        return True
+        self._buffer_max_size = 512*MB
+        self._buffer:MultiBuffer = None # RowBuffer or ColumnBuffer
+
+        self._collection_schema = None
+        self._set_target_collection(target_collection)
 
-    def clean_buffer(self):
-        self._buffer_size = 0
-        self._buffer = {}
-        if self._ingestion_type == IngestionType.ROW_BASED:
-            self._buffer = []
-
-    def clean_output(self):
-        def clean_files(path:str):
-            for root, dirs, files in os.walk(path):
-                for file in files:
-                    os.unlink(os.path.join(root, file))
-
-        for root, dirs, files in os.walk(self._output_folder):
-            for file in files:
-                os.unlink(os.path.join(root, file))
-            for dir in dirs:
-                clean_files(os.path.join(root, dir))
-                os.rmdir(os.path.join(root, dir))
-        self._print_info("Finished clean output folder {}".format(self._output_folder))
+        self._upload_lock = Lock()
 
-    def set_target_collection(self, collection_name: str)->bool:
+    def _args_check(self,
+                    target_collection: str,
+                    local_data_path: str,
+                    milvus_connector: MilvusConnector,
+                    uploader: Uploader,
+                    ingestion_type: IngestionType,
+                    ):
+        def _raise_err(msg: str):
+            self._print_err(msg)
+            raise Exception(msg)
+
+        if target_collection is None or len(target_collection) == 0:
+            _raise_err("Target collection name cannot be null or empty")
+        if local_data_path is None or len(local_data_path) == 0:
+            _raise_err("Local data path be null or empty")
+        if milvus_connector is None:
+            _raise_err("Milvus connector cannot be null")
+        if uploader is None:
+            _raise_err("Uploader cannot be null")
+        if not isinstance(ingestion_type, IngestionType):
+            _raise_err("illegal ingestion type: {}".format(ingestion_type))
+
+    def set_buffer_max_size(self, max_size: int):
+        if max_size <= 0:
+            max_size = 512*MB
+        self._buffer_max_size = max_size
+        if self._buffer is not None:
+            self._buffer.set_buffer_max_size(self._buffer_max_size)
+
+    def _set_target_collection(self, collection_name: str):
         if self._milvus_connector is None:
-            self._print_err("Milvus connector is None")
-            return False
+            msg = "Milvus connector is None"
+            self._print_err(msg)
+            raise Exception(msg)
+
+        collection_schema = self._milvus_connector.collection_schema(collection_name=collection_name)
+        if collection_schema is None:
+            msg = "Failed to get schema for collection '{}'".format(collection_name)
+            self._print_err()
+            raise Exception(msg)
+
+        self._collection_schema = collection_schema
+        self._buffer = MultiBuffer(collection_schema=self._collection_schema,
+                                   ingestion_type=self._ingestion_type,
+                                   buffer_max_size=self._buffer_max_size,
+                                   logger=self._logger)
+
+    def append_row(self, row: dict, partition_name: str = None)->bool:
+        if self._buffer is None:
+            msg = "Failed to append row, collection not specified"
+            self._print_err(msg)
+            raise Exception(msg)
 
-        self._target_fields = {}
-        self._target_collection_schema = self._milvus_connector.collection_schema(collection_name=collection_name)
-        if self._target_collection_schema is None:
-            self._print_err("Failed to get schema for collection '{}'".format(collection_name))
+        if not self._buffer.append_row(row=row, partition_name=partition_name):
             return False
 
-        for field in self._target_collection_schema['fields']:
-            self._target_fields[field['name']] = field
+        if self._buffer.has_large_buffer():
+            info_list = self._persist(force=False)
+            for info in info_list:
+                self._upload_import(info)
 
-        self.clean_buffer()
         return True
 
-    def current_row_count(self)->int:
-        if self._ingestion_type == IngestionType.ROW_BASED:
-            return len(self._buffer)
-        elif len(self._buffer) > 0:
-            return len(list(self._buffer.values())[0])
-        return 0
+    def current_row_count(self):
+        return self._buffer.buffer_row_count
 
+    def _persist(self, force: bool)->List[DataInfo]:
+        os.makedirs(name=self._local_data_path, exist_ok=True)
 
-    def append_row(self, row: dict)->bool:
-        if self._target_collection_schema is None:
-            self._print_err("Failed to append row, collection not specified")
-            return False
+        to_persist_buffer = self._buffer
+        self._buffer = MultiBuffer(collection_schema=self._collection_schema,
+                                   ingestion_type=self._ingestion_type,
+                                   logger=self._logger)
+
+        info_list = to_persist_buffer.persist(local_path=self._local_data_path, force=force)
+        if len(info_list) == 0:
+            self._print_info("Nothing to persist")
+            return []
 
-        if not self._verify_row(row=row):
-            return False
+        self._print_info("Successfully persist, buffer is reset")
+        return info_list
 
-        if self._buffer_size >= self._data_size_per_block:
-            self._print_info("Buffer size {} exceeds {}, force persist"
-                             .format(self._buffer_size, self._data_size_per_block))
-            self.persist()
-
-        if self._ingestion_type == IngestionType.ROW_BASED:
-            self._buffer.append(row)
-        else:
-            for k in self._target_fields:
-                if k not in self._buffer:
-                    self._buffer[k] = [row[k]]
-                else:
-                    self._buffer[k].append(row[k])
-        return True
+    def persist(self) -> List[str]:
+        info_list = self._persist(force=True)
+        return [info.local_folder for info in info_list]
 
-    def _verify_row(self, row: dict)->bool:
-        if len(self._target_fields) == 0:
-            self._print_err("Target collection schema is empty")
-            return False
+    def _update_info(self, info: DataInfo):
+        ok, msg = info.save()
+        if not ok:
+            self._print_err(msg)
 
-        row_size = 0
-        for k in self._target_fields:
-            if k not in row:
-                self._print_err("'{}' is missed in the row".format(k))
-                return False
-
-            field = self._target_fields[k]
-            if 'is_parimary' in field and field['auto_id']:
-                self._print_err("The primary key field '{}' is auto-id, no need to provide".format(k))
-                return False
-
-            dtype = DataType(field['type'])
-            validator = self._type_validator[dtype.name]
-            if dtype == DataType.BINARY_VECTOR or dtype == DataType.FLOAT_VECTOR:
-                dim = field['params']['dim']
-                if not validator(row[k], dim):
-                    self._print_err("Vector data doesn't match with {} schema".format(dtype.name))
-                    return False
-                row_size = row_size + len(row[k])
-            elif dtype == DataType.VARCHAR:
-                max_len = field['params']['max_length']
-                if not validator(row[k], max_len):
-                    self._print_err("Varchar value doesn't match with {} schema".format(dtype.name))
-                    return False
-                row_size = row_size + len(row[k])
-            else:
-                if not validator(row[k]):
-                    self._print_err("Scalar value doesn't match with {} schema".format(dtype.name))
-                    return False
-                row_size = row_size + self._type_size[dtype.name]
-        self._buffer_size = self._buffer_size + row_size
-        return True
+    def _upload_import(self, info: DataInfo)->int:
+        if len(info.local_files) == 0:
+            self._print_err("No local data files to upload")
+            return 0
 
-    def persist(self)->bool:
-        os.makedirs(name=self._output_folder, exist_ok=True)
-        if self._ingestion_type == IngestionType.ROW_BASED:
-            n = 1
-            while True:
-                target_path = os.path.join(self._output_folder, "rows_{}.json".format(n))
-                if not os.path.exists(target_path):
-                    break
-                n = n + 1
-
-            content = {
-                "rows": self._buffer,
-            }
-            try:
-                with open(target_path, 'w', encoding='utf-8') as f:
-                    json.dump(obj=content, fp=f, indent=2, ensure_ascii=False)
-            except Exception as e:
-                self._print_err("Failed to persist row-based file {}, error: {}".format(target_path, e))
-                return False
-
-            self._print_info("Successfully persist row-based file {}".format(target_path))
-        else:
-            n = 1
-            while True:
-                target_dir = os.path.join(self._output_folder, "columns_{}".format(n))
-                if not os.path.exists(target_dir):
-                    break
-                n = n + 1
-            os.makedirs(name=target_dir, exist_ok=True)
-            for k in self._buffer:
-                target_path = os.path.join(target_dir, k + ".npy")
-                try:
-                    numpy.save(target_path, self._buffer[k])
-                except Exception as e:
-                    self._print_err("Failed to persist column-based file {}, error: {}".format(target_path, e))
-                    return False
+        if self._uploader is None:
+            self._print_err("Uploader is None")
+            return 0
 
-                self._print_info("Successfully persist column-based file {}".format(target_path))
+        if self._milvus_connector is not None:
+            ok, msg = self._milvus_connector.verify_input(info.collection_name, info.partition_name)
+            if not ok:
+                msg = "Unable to import files {}, error: {}".format(info.local_files, msg)
+                self._print_err(msg)
+                info.bulkinsert_done = False
+                info.bulkinsert_err = msg
+                self._update_info(info)
+                return 0
 
-        self._print_info("Successfully persist, clean the buffer now")
-        self.clean_buffer()
-        return True
+        # upload files
+        ok, remote_files = self._uploader.upload(files=info.local_files, relative_path=self._local_data_path)
+        if not ok:
+            msg = "Failed to upload files {}".format(info.local_files)
+            self._print_err(msg)
+            info.bulkinsert_done = False
+            info.bulkinsert_err = msg
+            self._update_info(info)
+            return 0
 
-    def direct_insert(self, partition_name: str = None)->list:
         if self._milvus_connector is None:
             self._print_err("Milvus connector is None")
+            return 0
+
+        # call bulkinsert
+        partition_name = None if info.partition_name == DEFAULT_PARTITION_NAME else info.partition_name
+        task_id, msg = self._milvus_connector.bulk_insert(files=remote_files,
+                                                          collection_name=info.collection_name,
+                                                          partition_name=partition_name)
+        if task_id == 0:
+            self._print_err("Failed to import to collection '{}', partition '{}', error: {}"
+                            .format(info.collection_name, partition_name, msg))
+            info.bulkinsert_done = False
+            info.bulkinsert_err = msg
+            return 0
+        self._print_info("Start a bulkinsert task to import files {}, task id: {}".format(remote_files, task_id))
+
+        # write infomation into a json file
+        info.bulkinsert_id = task_id
+        info.remote_files = remote_files
+        ok, msg = info.save()
+        if not ok:
+            self._print_err(msg)
+
+        return task_id
+
+    def upload(self, data_folder: str=None)->List[int]:
+        if self._uploader is None:
+            self._print_err("Uploader is None")
             return []
 
-        if len(self._target_fields) == 0:
-            self._print_err("Target collection schema is empty")
+        if data_folder is None:
+            data_folder = self._local_data_path
+
+        task_list = []
+        info_list = self._list_bulkinsert_tasks(data_folder)
+        for info in info_list:
+            if info.bulkinsert_done:
+                continue
+
+            task_id = self._upload_import(info)
+            if task_id > 0:
+                task_list.append(task_id)
+
+        return task_list
+
+    def wait_upload_finish(self, task_list: List[int]=None)->bool:
+        if self._milvus_connector is None:
+            self._print_err("Milvus connector is None")
+            return False
+
+        wait_info_list = []
+        # find out the unfinished tasks
+        all_info_list = self._list_bulkinsert_tasks()
+        for info in all_info_list:
+            if info.bulkinsert_id is None or info.bulkinsert_done:
+                continue
+            if task_list is not None:
+                if info.bulkinsert_id in task_list:
+                    wait_info_list.append(info)
+            else:
+                wait_info_list.append(info)
+
+        # wait the unfinished tasks
+        collection_list = []
+        for info in wait_info_list:
+            if info.collection_name not in collection_list:
+                collection_list.append(info.collection_name)
+            state = self._milvus_connector.wait_bulkinsert_task(info.bulkinsert_id)
+            if state.state == BulkInsertState.ImportCompleted:
+                self._print_info("Bulklinsert task {} completed".format(info.bulkinsert_id))
+                info.bulkinsert_done = True
+                info.bulkinsert_pk_ranges = list(state.id_ranges)
+            elif state.state == BulkInsertState.ImportFailed or state.state == BulkInsertState.ImportFailedAndCleaned:
+                self._print_err("Bulklinsert task {} failed with reason: {}"
+                                .format(info.bulkinsert_id, info.bulkinsert_err))
+                info.bulkinsert_done = False
+                info.bulkinsert_err = state.failed_reason
+
+            # update the info
+            ok, msg = info.save()
+            if not ok:
+                self._print_err(msg)
+
+        # refresh load the collections
+        self._milvus_connector.refresh_load(collection_list)
+        return True
+
+    def _list_bulkinsert_tasks(self, data_folder: str=None)->List[DataInfo]:
+        if data_folder is None:
+            data_folder = self._local_data_path
+
+        info_list = []
+        for root, _, files in os.walk(data_folder):
+            if DATAINFO_FILE_NAME in files:
+                info = DataInfo()
+                ok, msg = info.load(root)
+                if not ok:
+                    self._print_err(msg)
+                    continue
+                info_list.append(info)
+        return info_list
+
+    def list_bulkinsert_tasks(self) -> List[dict]:
+        info_list = self._list_bulkinsert_tasks(self._local_data_path)
+        return [info.to_dict() for info in info_list]
+
+    def clear_data_folder(self, options: CleanDataOptions=CleanDataOptions.CLEAN_SUCCEED_IMPORT_DATA):
+        self._print_warn("Clear the data folder '{}', all the local data will be deleted".format(self._local_data_path))
+
+        def _remove_files(info: DataInfo):
+            if len(info.local_files) > 0:
+                for file in info.local_files:
+                    os.remove(file)
+            if len(info.remote_files) > 0:
+                if self._uploader != None:
+                    self._uploader.remove(info.remote_files)
+            shutil.rmtree(info.local_folder)
+
+        sub_paths = os.listdir(self._local_data_path)
+        for p in sub_paths:
+            full_path = os.path.join(self._local_data_path, p)
+            if os.path.isdir(full_path):
+                if options == CleanDataOptions.CLEAN_ALL_DATA:
+                    shutil.rmtree(full_path)
+                    continue
+
+                info_list = self._list_bulkinsert_tasks(full_path)
+                for info in info_list:
+                    if info.bulkinsert_done and (options & CleanDataOptions.CLEAN_SUCCEED_IMPORT_DATA):
+                        _remove_files(info)
+                    if (not info.bulkinsert_done) and (options & CleanDataOptions.CLEAN_FAILED_IMPORT_DATA):
+                        _remove_files(info)
+
+    def direct_insert(self)->list:
+        if self._milvus_connector is None:
+            self._print_err("Milvus connector is None")
             return []
 
-        row_count = self.current_row_count()
-        if row_count == 0:
+        row_count = self._buffer.buffer_row_count
+        if self._buffer is None or row_count == 0:
             self._print_err("Buffer is empty")
             return []
 
-        size_per_row = self._buffer_size/row_count
+        # reset the buffer
+        to_persist_buffer = self._buffer
+        self._buffer = MultiBuffer(collection_schema=self._collection_schema,
+                                   ingestion_type=self._ingestion_type,
+                                   logger=self._logger)
+
+        size_per_row = to_persist_buffer.buffer_size/row_count
         batch = int(8*MB/size_per_row)
         if batch > row_count:
             batch = row_count
 
         self._print_info("{} rows in buffer, prepare to insert batch by batch, {} rows per batch"
                          .format(row_count, batch))
 
+        collection_name = to_persist_buffer.collection_name
         primary_ids = []
-        if self._ingestion_type == IngestionType.ROW_BASED:
-            while len(self._buffer) > 0:
-                batch_data = {}
-                for k in self._target_fields:
-                    batch_data[k] = []
-                rows = self._buffer[:batch]
-                self._buffer = self._buffer[batch:]
-                for row in rows:
-                    for k in batch_data:
-                        batch_data[k].append(row[k])
-
-                data = []
-                for k in batch_data:
-                    data.append(batch_data[k])
-                ids = self._milvus_connector.insert(data = data,
-                                                    collection_name=self._target_collection_schema['collection_name'],
-                                                    partition_name=partition_name)
-                primary_ids.extend(ids)
-
-        else:
-            while len(list(self._buffer.values())[0]) > 0:
-                batch_data = {}
-                for k in self._target_fields:
-                    batch_data[k] = self._buffer[k][:batch]
-                    self._buffer[k] = self._buffer[k][batch:]
-                data = []
-                for k in batch_data:
-                    data.append(batch_data[k])
-                ids = self._milvus_connector.insert(data=data,
-                                                    collection_name=self._target_collection_schema['collection_name'],
-                                                    partition_name=partition_name)
-                primary_ids.extend(ids)
-
-        self._print_info("Finish insert {} rows into Milvus, clean the buffer now".format(row_count))
-        self.clean_buffer()
+        while True:
+            partition_name, rows = to_persist_buffer.pop(batch)
+            if len(rows) == 0:
+                break
+
+            if (partition_name == DEFAULT_PARTITION_NAME) or (len(partition_name) == 0):
+                partition_name = None
+            ids = self._milvus_connector.insert(data=rows,
+                                                collection_name=collection_name,
+                                                partition_name=partition_name)
+            primary_ids.extend(ids)
+            self._print_info("Finish insert {} rows into collection '{}' partition '{}'"
+                             .format(len(rows), collection_name, partition_name))
+
+        self._milvus_connector.flush(collection_name=collection_name)
+        self._print_info("{} rows were inserted to collection '{}', the collection currently has {} rows"
+                         .format(row_count, collection_name, self._milvus_connector.num_entities(collection_name)))
         return primary_ids
 
-    def upload(self, partition_name: str = None, clean:bool = False)->int:
-        if self._uploader is None:
-            self._print_err("Uploader is None")
-            return 0
-
-        ok, files = self._uploader.upload(self._output_folder)
-        if clean:
-            self.clean_output()
-        if not ok:
-            return 0
-
-        if self._milvus_connector is None:
-            self._print_err("Milvus connector is None")
-            return False
-
-        id = self._milvus_connector.bulk_insert(files=files,
-                                                collection_name=self._target_collection_schema['collection_name'],
-                                                partition_name=partition_name)
-        return id
```

### Comparing `milvus-ingestion-0.3.0/milvus_ingestion/util.py` & `milvus-ingestion-0.4.0/milvus_ingestion/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,28 +4,36 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
 
+import datetime
 import logging
 from logging import Logger
 
 defaultLogger = logging.getLogger()
 fmt = '%(asctime)s|%(funcName)s|%(lineno)s|%(levelname)s|%(message)s'
 formatter = logging.Formatter(fmt)
 handler = logging.StreamHandler()
 handler.setFormatter(formatter)
 defaultLogger.addHandler(handler)
 defaultLogger.setLevel('DEBUG')
 
+
 def default_logger()->Logger:
     return defaultLogger
 
+
+def _current_datetime() -> str:
+    dt = datetime.datetime.now()
+    return dt.strftime('%Y-%m-%d_%H:%M:%S.%f')
+
+
 class Base:
     def __init__(self, logger: Logger = default_logger()):
         self._logger = logger
 
     def _print_info(self, msg):
         if self._logger:
             self._logger.info(msg)
```

### Comparing `milvus-ingestion-0.3.0/setup.py` & `milvus-ingestion-0.4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / 'README.md').read_text()
 
 setuptools.setup(
     name="milvus-ingestion",
-    version="0.3.0",
+    version="0.4.0",
     author='yihua.mo',
     author_email='yihua.mo@zilliz.com',
     description="A tool to help data ingestion for Milvus",
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/yhmo/milvus-ingestion',
     license="Apache-2.0",
     packages=setuptools.find_packages(),
     include_package_data=True,
     install_requires=[
         "minio==7.1.14",
-        "pymilvus==2.2.8",
+        "pymilvus==2.2.9",
         "numpy==1.24.3",
+        "shutilwhich==1.1.0",
     ],
     classifiers=[
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
```

