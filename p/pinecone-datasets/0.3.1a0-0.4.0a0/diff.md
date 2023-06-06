# Comparing `tmp/pinecone_datasets-0.3.1a0.tar.gz` & `tmp/pinecone_datasets-0.4.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinecone_datasets-0.3.1a0.tar", max compression
+gzip compressed data, was "pinecone_datasets-0.4.0a0.tar", max compression
```

## Comparing `pinecone_datasets-0.3.1a0.tar` & `pinecone_datasets-0.4.0a0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     6295 2023-03-21 13:36:03.728655 pinecone_datasets-0.3.1a0/README.md
--rw-r--r--   0        0        0      142 2023-03-22 14:50:19.983219 pinecone_datasets-0.3.1a0/pinecone_datasets/__init__.py
--rw-r--r--   0        0        0     2816 2023-03-21 13:36:03.729844 pinecone_datasets-0.3.1a0/pinecone_datasets/catalog.py
--rw-r--r--   0        0        0      706 2023-03-16 15:10:49.893876 pinecone_datasets-0.3.1a0/pinecone_datasets/cfg.py
--rw-r--r--   0        0        0     8971 2023-03-21 13:36:03.730320 pinecone_datasets-0.3.1a0/pinecone_datasets/dataset.py
--rw-r--r--   0        0        0      876 2023-03-21 13:36:03.730549 pinecone_datasets-0.3.1a0/pinecone_datasets/fs.py
--rw-r--r--   0        0        0     1672 2023-03-22 14:50:19.983675 pinecone_datasets-0.3.1a0/pinecone_datasets/public.py
--rw-r--r--   0        0        0      821 2023-03-22 14:50:19.984513 pinecone_datasets-0.3.1a0/pyproject.toml
--rw-r--r--   0        0        0     7366 1970-01-01 00:00:00.000000 pinecone_datasets-0.3.1a0/setup.py
--rw-r--r--   0        0        0     7176 1970-01-01 00:00:00.000000 pinecone_datasets-0.3.1a0/PKG-INFO
+-rw-r--r--   0        0        0     6367 2023-06-06 17:49:00.712952 pinecone_datasets-0.4.0a0/README.md
+-rw-r--r--   0        0        0      142 2023-06-06 17:49:28.255111 pinecone_datasets-0.4.0a0/pinecone_datasets/__init__.py
+-rw-r--r--   0        0        0     3088 2023-06-01 03:29:23.061670 pinecone_datasets-0.4.0a0/pinecone_datasets/catalog.py
+-rw-r--r--   0        0        0      706 2023-06-06 17:49:00.715570 pinecone_datasets-0.4.0a0/pinecone_datasets/cfg.py
+-rw-r--r--   0        0        0     8800 2023-06-06 17:49:00.716674 pinecone_datasets-0.4.0a0/pinecone_datasets/dataset.py
+-rw-r--r--   0        0        0      946 2023-05-31 10:57:13.712902 pinecone_datasets-0.4.0a0/pinecone_datasets/fs.py
+-rw-r--r--   0        0        0     1657 2023-05-31 11:31:31.876795 pinecone_datasets-0.4.0a0/pinecone_datasets/public.py
+-rw-r--r--   0        0        0      822 2023-06-06 17:51:58.311038 pinecone_datasets-0.4.0a0/pyproject.toml
+-rw-r--r--   0        0        0     7445 1970-01-01 00:00:00.000000 pinecone_datasets-0.4.0a0/setup.py
+-rw-r--r--   0        0        0     7248 1970-01-01 00:00:00.000000 pinecone_datasets-0.4.0a0/PKG-INFO
```

### Comparing `pinecone_datasets-0.3.1a0/README.md` & `pinecone_datasets-0.4.0a0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Pinecone Datasets
 
+## install
+
+```bash
+pip install pinecone-datasets
+```
+
 ## Usage
 
 You can use Pinecone Datasets to load our public datasets or with your own dataset.
 
 ### Loading Pinecone Public Datasets
 
 ```python
@@ -66,15 +72,15 @@
 index = pinecone.GRPCIndex("my-index")
 ```
 
 ## Advanced Usage
 
 ### Working with your own dataset storage
 
-Datasets is using Pinecone's public datasets bucket on GCS, you can use your own bucket by setting the `PINECONE_DATASETS_EDNPOINT` environment variable.
+Datasets is using Pinecone's public datasets bucket on GCS, you can use your own bucket by setting the `DATASETS_CATALOG_BASEPATH` environment variable.
 
 ```bash
 export PINECONE_DATASETS_ENDPOINT="gs://my-bucket"
 ```
 
 this will change the default endpoint to your bucket, and upon calling `list_datasets` or `load_dataset` it will scan your bucket and list all datasets.
 
@@ -144,15 +150,16 @@
 ```python
 meta.schema()
 ```
 
 in order to list a dataset you can save dataset metadata (NOTE: write permission to loacaion is needed)
 
 ```python
-dataset._save_metadata("non-listed-dataset", meta)
+dataset = Dataset("non-listed-dataset")
+dataset._save_metadata(meta)
 ```
 
 ### Uploading and listing a dataset. 
 
 pinecone datasets can load dataset from every storage where it has access (using the default access: s3, gcs or local permissions)
 
  we expect data to be uploaded to the following directory structure:
```

### Comparing `pinecone_datasets-0.3.1a0/pinecone_datasets/catalog.py` & `pinecone_datasets-0.4.0a0/pinecone_datasets/catalog.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import datetime
+from datetime import datetime
 import warnings
 import os
 import json
 from ssl import SSLCertVerificationError
-from typing import List, Optional, Union
+from typing import List, Optional, Union, Any, Dict
 import s3fs
 import gcsfs
-from pydantic import BaseModel, ValidationError
+from pydantic import BaseModel, ValidationError, Field
 import pandas as pd
 
 from pinecone_datasets import cfg
 from pinecone_datasets.fs import get_cloud_fs
 
 
 class DenseModelMetadata(BaseModel):
@@ -20,54 +20,62 @@
 
 
 class SparseModelMetdata(BaseModel):
     name: Optional[str]
     tokenizer: Optional[str]
 
 
+def get_time_now() -> str:
+    return datetime.now().strftime("%Y-%m-%d %H:%M:%S.%f")
+
+
 class DatasetMetadata(BaseModel):
     name: str
     created_at: str
     documents: int
     queries: int
     source: Optional[str]
-    bucket: str
-    task: str
+    license: Optional[str]
+    bucket: Optional[str]
+    task: Optional[str]
     dense_model: DenseModelMetadata
     sparse_model: Optional[SparseModelMetdata]
+    description: Optional[str]
+    tags: Optional[List[str]]
+    args: Optional[Dict[str, Any]]
 
 
 class Catalog(BaseModel):
     datasets: List[DatasetMetadata] = []
 
     @staticmethod
     def load(**kwargs) -> "Catalog":
         public_datasets_base_path = os.environ.get(
-            "PINECONE_DATASETS_EDNPOINT", cfg.Storage.endpoint
+            "DATASETS_CATALOG_BASEPATH", cfg.Storage.endpoint
         )
         fs = get_cloud_fs(public_datasets_base_path, **kwargs)
         if not fs:
             raise ValueError(
                 "Public datasets are only supported on cloud storage, with valid s3:// or gs:// paths"
             )
         collected_datasets = []
         try:
             for f in fs.listdir(public_datasets_base_path):
                 if f["type"] == "directory":
                     try:
                         prefix = "gs" if isinstance(fs, gcsfs.GCSFileSystem) else "s3"
                         with fs.open(f"{prefix}://{f['name']}/metadata.json") as f:
                             try:
-                                this_dataset = json.load(f)
+                                this_dataset_json = json.load(f)
                             except json.JSONDecodeError:
                                 warnings.warn(
                                     f"Not a JSON: Invalid metadata.json for {f['name']}, skipping"
                                 )
                             try:
-                                this_dataset = DatasetMetadata(**this_dataset)
+                                this_dataset = DatasetMetadata(**this_dataset_json)
                                 collected_datasets.append(this_dataset)
                             except ValidationError:
                                 warnings.warn(
                                     f"metadata file for dataset: {f['name']} is not valid, skipping"
                                 )
                     except FileNotFoundError:
                         pass
```

### Comparing `pinecone_datasets-0.3.1a0/pinecone_datasets/cfg.py` & `pinecone_datasets-0.4.0a0/pinecone_datasets/cfg.py`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.3.1a0/pinecone_datasets/dataset.py` & `pinecone_datasets-0.4.0a0/pinecone_datasets/dataset.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import sys
 import glob
 import os
 import json
+from functools import cached_property
 from typing import Any, Generator, Iterator, List, Union, Dict
 import warnings
+from urllib.parse import urlparse
 
 import gcsfs
 from pydantic import ValidationError
 import s3fs
 import polars as pl
 import pandas as pd
 import pyarrow.parquet as pq
@@ -28,88 +30,101 @@
     df: pd.DataFrame,
 ) -> Generator[Dict[str, Any], None, None]:
     for i in range(0, len(df), 1):
         yield df.iloc[i : i + 1].to_dict(orient="records")[0]
 
 
 class Dataset(object):
+    @classmethod
+    def from_path(cls, dataset_path, **kwargs):
+        """
+        Create a Dataset object from local or cloud storage
+        Args:
+            dataset_path (str): a path to a local or cloud storage path containing a valid dataset.
+
+        Keyword Args:
+            engine (str): the engine to use for loading the dataset. Options are ['polars', 'pandas']. Defaults to 'pandas'.
+
+        Returns:
+            Dataset: a Dataset object
+        """
+        return cls(dataset_path=dataset_path, **kwargs)
+
+    @classmethod
+    def from_catalog(cls, dataset_id, catalog_base_path: str = "", **kwargs):
+        """
+        Load a dataset from Pinecone's Datasets catalog, or from your own endpoint.
+
+        Args:
+            dataset_id (str): the id of the dataset to load within a catalog
+            catalog_base_path (str): the catalog's base path. Defaults to DATASETS_CATALOG_BASEPATH environment variable.
+                                     If neither are set, will use Pinecone's public catalog.
+
+        Keyword Args:
+            engine (str): the engine to use for loading the dataset. Options are ['polars', 'pandas']. Defaults to 'pandas'.
+
+        Returns:
+            Dataset: a Dataset object
+        """
+        catalog_base_path = (
+            catalog_base_path
+            if catalog_base_path
+            else os.environ.get("DATASETS_CATALOG_BASEPATH", cfg.Storage.endpoint)
+        )
+        dataset_path = os.path.join(catalog_base_path, f"{dataset_id}")
+        return cls(dataset_path=dataset_path, **kwargs)
+
     def __init__(
         self,
-        dataset_id: str = "",
-        endpoint: str = "",
+        dataset_path: str,
         engine: str = "pandas",
-        should_load_metadata: bool = False,
         **kwargs,
     ) -> None:
         """
         Dataset class to load and query datasets from the Pinecone Datasets catalog.
-
-        Args:
-            dataset_id (str, optional): The dataset id. Defaults to "".
-            base_path (str, optional): The path to the dataset. Defaults to "". by default, datasets will look for datasets at path: {base_path}/{dataset_id}/
-            engine (str, optional): The engine to use for loading the dataset. Options are ['polars', 'pandas']. Defaults to 'pandas'.
-            should_load_metadata: (bool, optional): Whether to load the metadata for the dataset. Defaults to False.
-
+        See `from_path` and `from_dataset_id` for examples on how to load a dataset.
 
         Examples:
+            ```python
             from pinecone_datasets import Dataset
-            dataset = Dataset("dataset_name")
+            dataset = Dataset.from_dataset_id("dataset_name")
+            # or
+            dataset = Dataset.from_path("gs://my-bucket/my-dataset")
+
             for doc in dataset.iter_documents(batch_size=100):
                 index.upsert(doc)
             for query in dataset.iter_queries(batch_size):
                 results = index.search(query)
                 # do something with the results
             # or
             dataset.documents # returns a pandas/polars DataFrame
             dataset.queries # returns a pandas/polars DataFrame
+            ```
 
         """
-        self._documents: pl.DataFrame = None
-        self._queries: pl.DataFrame = None
-        self._metadata: DatasetMetadata = None
-        self._is_load_metadata = should_load_metadata
         self._config = cfg
-        self._endpoint = (
-            endpoint
-            if endpoint
-            else os.environ.get(
-                "PINECONE_DATASETS_EDNPOINT", self._config.Storage.endpoint
-            )
-        )
         self._engine = engine
-        self._fs = get_cloud_fs(self._endpoint, **kwargs)
-        if dataset_id:
-            self._load(dataset_id)
-
-    def _create_path(self, dataset_id: str) -> str:
-        path = os.path.join(self._endpoint, f"{dataset_id}")
-        return path
-
-    def _is_datatype_exists(self, data_type: str, dataset_id: str) -> bool:
-        if self._fs:
-            key = os.path.join(self._create_path(dataset_id), data_type).split("//")[-1]
-            for obj in self._fs.ls(self._create_path(dataset_id)):
-                if obj == key:
-                    return True
-            return False
-        else:
-            return os.path.exists(
-                os.path.join(self._create_path(dataset_id), data_type)
+        endpoint = urlparse(dataset_path)._replace(path="").geturl()
+        self._fs = get_cloud_fs(endpoint, **kwargs)
+        self._dataset_path = dataset_path
+
+        if not self._fs.exists(self._dataset_path):
+            raise FileNotFoundError(
+                "Dataset does not exist. Please check the path or dataset_id"
             )
 
+    def _is_datatype_exists(self, data_type: str) -> bool:
+        return self._fs.exists(os.path.join(self._dataset_path, data_type))
+
     def _safe_read_from_path(
-        self, data_type: str, dataset_id: str, enforced_schema: Dict[str, Any]
+        self, data_type: str, enforced_schema: Dict[str, Any]
     ) -> Union[pl.DataFrame, pd.DataFrame]:
-        read_path_str = os.path.join(
-            self._create_path(dataset_id), data_type, "*.parquet"
-        )
-        read_path = (
-            self._fs.glob(read_path_str) if self._fs else glob.glob(read_path_str)
-        )
-        if self._is_datatype_exists(data_type, dataset_id):
+        read_path_str = os.path.join(self._dataset_path, data_type, "*.parquet")
+        read_path = self._fs.glob(read_path_str)
+        if self._is_datatype_exists(data_type):
             dataset = pq.ParquetDataset(read_path, filesystem=self._fs)
             try:
                 if self._engine == "pandas":
                     df = dataset.read_pandas().to_pandas()
                 elif self._engine == "polars":
                     df = pl.from_arrow(dataset.read(), schema_overrides=enforced_schema)
                 else:
@@ -132,67 +147,41 @@
             if self._engine == "pandas":
                 return pd.DataFrame()
             elif self._engine == "polars":
                 return pl.DataFrame()
             else:
                 raise ValueError("engine must be one of ['pandas', 'polars']")
 
-    def _load_metadata(self, dataset_id: str) -> None:
-        if self._fs:
-            with self._fs.open(
-                os.path.join(self._create_path(dataset_id), "metadata.json"), "rb"
-            ) as f:
-                metadata = json.load(f)
-        else:
-            with open(
-                os.path.join(self._create_path(dataset_id), "metadata.json"), "rb"
-            ) as f:
-                metadata = json.load(f)
+    def _load_metadata(self) -> DatasetMetadata:
+        with self._fs.open(
+            os.path.join(self._dataset_path, "metadata.json"), "rb"
+        ) as f:
+            metadata = json.load(f)
         try:
             out = DatasetMetadata(**metadata)
             return out
         except ValidationError as e:
             raise e
 
-    def _save_metadata(
-        self, dataset_id: str, metadata: DatasetMetadata
-    ) -> None:  # pragma: no cover
-        if self._fs:
-            with self._fs.open(
-                os.path.join(self._create_path(dataset_id), "metadata.json"), "w"
-            ) as f:
-                json.dump(metadata.dict(), f)
-        else:
-            with open(
-                os.path.join(self._create_path(dataset_id), "metadata.json"), "w"
-            ) as f:
-                json.dump(metadata.dict(), f)
-
-    def _load(self, dataset_id: str) -> None:
-        self._documents = self._safe_read_from_path(
-            "documents", dataset_id, self._config.Schema.documents
-        )
-        self._queries = self._safe_read_from_path(
-            "queries", dataset_id, self._config.Schema.queries
-        )
-        if self._is_load_metadata:
-            self._metadata = self._load_metadata(dataset_id)
+    def _save_metadata(self, metadata: DatasetMetadata) -> None:  # pragma: no cover
+        with self._fs.open(os.path.join(self._dataset_path, "metadata.json"), "w") as f:
+            json.dump(metadata.dict(), f)
 
     def __getitem__(self, key: str) -> pl.DataFrame:
         if key in ["documents", "queries"]:
             return getattr(self, key)
         else:
             raise KeyError("Dataset does not have key: {}".format(key))
 
     def __len__(self) -> int:
-        return self._documents.shape[0]
+        return self.documents.shape[0]
 
-    @property
+    @cached_property
     def documents(self) -> Union[pl.DataFrame, pd.DataFrame]:
-        return self._documents
+        return self._safe_read_from_path("documents", self._config.Schema.documents)
 
     def iter_documents(self, batch_size: int = 1) -> Iterator[List[Dict[str, Any]]]:
         """
         Iterates over the documents in the dataset.
 
         Args:
             batch_size (int, optional): The batch size to use for the iterator. Defaults to 1.
@@ -203,29 +192,29 @@
         Examples:
             for batch in dataset.iter_documents(batch_size=100):
                 index.upsert(batch)
         """
         if isinstance(batch_size, int) and batch_size > 0:
             if self._engine == "pandas":
                 return iter_pandas_dataframe_slices(
-                    self._documents[self._config.Schema.documents_select_columns],
+                    self.documents[self._config.Schema.documents_select_columns],
                     batch_size,
                 )
             return map(
                 lambda x: x.to_dicts(),
-                self._documents.select(
+                self.documents.select(
                     self._config.Schema.documents_select_columns
                 ).iter_slices(n_rows=batch_size),
             )
         else:
             raise ValueError("batch_size must be greater than 0")
 
-    @property
+    @cached_property
     def queries(self) -> Union[pl.DataFrame, pd.DataFrame]:
-        return self._queries
+        return self._safe_read_from_path("queries", self._config.Schema.documents)
 
     def iter_queries(self) -> Iterator[Dict[str, Any]]:
         """
         Iterates over the queries in the dataset.
 
         Returns:
             Iterator[Dict[str, Any]]: An iterator over the queries in the dataset.
@@ -233,16 +222,20 @@
         Examples:
             for query in dataset.iter_queries():
                 results = index.query(**query)
                 # do something with the results
         """
         if self._engine == "pandas":
             return iter_pandas_dataframe_single(
-                self._queries[self._config.Schema.queries_select_columns]
+                self.queries[self._config.Schema.queries_select_columns]
             )
         else:
-            return self._queries.select(
-                self._queries[self._config.Schema.queries_select_columns]
+            return self.queries.select(
+                self.queries[self._config.Schema.queries_select_columns]
             ).iter_rows(named=True)
 
+    @cached_property
+    def metadata(self) -> Union[pl.DataFrame, pd.DataFrame]:
+        return self._load_metadata()
+
     def head(self, n: int = 5) -> Union[pl.DataFrame, pd.DataFrame]:
         return self.documents.head(n)
```

### Comparing `pinecone_datasets-0.3.1a0/pinecone_datasets/fs.py` & `pinecone_datasets-0.4.0a0/pinecone_datasets/fs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Union
 
 import gcsfs
 import s3fs
+from fsspec.implementations.local import LocalFileSystem
 
 from pinecone_datasets import cfg
 
 
 def get_cloud_fs(path, **kwargs) -> Union[gcsfs.GCSFileSystem, s3fs.S3FileSystem]:
     """
     returns a filesystem object for the given path, if it is a cloud storage path (gs:// or s3://)
@@ -19,9 +20,9 @@
     """
     is_anon = path == cfg.Storage.endpoint
     if path.startswith("gs://") or "storage.googleapis.com" in path:
         fs = gcsfs.GCSFileSystem(token="anon" if is_anon else None, **kwargs)
     elif path.startswith("s3://") or "s3.amazonaws.com" in path:
         fs = s3fs.S3FileSystem(anon=is_anon, **kwargs)
     else:
-        fs = None
+        fs = LocalFileSystem()
     return fs
```

### Comparing `pinecone_datasets-0.3.1a0/pinecone_datasets/public.py` & `pinecone_datasets-0.4.0a0/pinecone_datasets/public.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 catalog = None
 
 
 def list_datasets(as_df=False, **kwargs) -> list:
     """
     List all datasets in the catalog, optionally as a pandas DataFrame.
-    Catalog is set using the `PINECONE_DATASETS_EDNPOINT` environment variable.
+    Catalog is set using the `DATASETS_CATALOG_BASEPATH` environment variable.
 
     Args:
         as_df (bool, optional): Whether to return the list as a pandas DataFrame. Defaults to False.
 
     Returns:
         list: A list of dataset names; or
         df: A pandas DataFrame of dataset names and metadata
@@ -52,8 +52,8 @@
     if not catalog:
         lst = list_datasets(as_df=False)
     else:
         lst = catalog.list_datasets(as_df=False)
     if dataset_id not in lst:
         raise FileNotFoundError(f"Dataset {dataset_id} not found in catalog")
     else:
-        return Dataset(dataset_id, should_load_metadata=True, **kwargs)
+        return Dataset.from_catalog(dataset_id, **kwargs)
```

### Comparing `pinecone_datasets-0.3.1a0/pyproject.toml` & `pinecone_datasets-0.4.0a0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "pinecone-datasets"
-version = "0.3.1-alpha"
+version = "0.4.0-alpha"
 description = "Pinecone Datasets lets you easily load datasets into your Pinecone index."
 authors = ["Pinecone"]
 maintainers = [
     "Roy Miara <miararoy@gmail.com>",
 ]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 polars = "^0.16.4"
-pyarrow = "^11.0.0"
+pyarrow = "^12.0.0"
 fsspec = "^2023.1.0"
 gcsfs = "^2023.1.0"
 s3fs = "^2023.1.0"
 pydantic = "^1.10.5"
 protobuf = ">=3.19.3,<3.20.0"
-pandas = "^1.5.3"
+pandas = "^2.0.0"
+
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.21.1"
 pinecone-client = {version="^2.2", extras=["grpc"]}
```

### Comparing `pinecone_datasets-0.3.1a0/setup.py` & `pinecone_datasets-0.4.0a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['fsspec>=2023.1.0,<2024.0.0',
  'gcsfs>=2023.1.0,<2024.0.0',
- 'pandas>=1.5.3,<2.0.0',
+ 'pandas>=2.0.0,<3.0.0',
  'polars>=0.16.4,<0.17.0',
  'protobuf>=3.19.3,<3.20.0',
- 'pyarrow>=11.0.0,<12.0.0',
+ 'pyarrow>=12.0.0,<13.0.0',
  'pydantic>=1.10.5,<2.0.0',
  's3fs>=2023.1.0,<2024.0.0']
 
 setup_kwargs = {
     'name': 'pinecone-datasets',
-    'version': '0.3.1a0',
+    'version': '0.4.0a0',
     'description': 'Pinecone Datasets lets you easily load datasets into your Pinecone index.',
-    'long_description': '# Pinecone Datasets\n\n## Usage\n\nYou can use Pinecone Datasets to load our public datasets or with your own dataset.\n\n### Loading Pinecone Public Datasets\n\n```python\nfrom pinecone_datasets import list_datasets, load_dataset\n\nlist_datasets()\n# ["quora_all-MiniLM-L6-bm25", ... ]\n\ndataset = load_dataset("quora_all-MiniLM-L6-bm25")\n\ndataset.head()\n\n# Prints\n# ┌─────┬───────────────────────────┬─────────────────────────────────────┬───────────────────┬──────┐\n# │ id  ┆ values                    ┆ sparse_values                       ┆ metadata          ┆ blob │\n# │     ┆                           ┆                                     ┆                   ┆      │\n# │ str ┆ list[f32]                 ┆ struct[2]                           ┆ struct[3]         ┆      │\n# ╞═════╪═══════════════════════════╪═════════════════════════════════════╪═══════════════════╪══════╡\n# │ 0   ┆ [0.118014, -0.069717, ... ┆ {[470065541, 52922727, ... 22364... ┆ {2017,12,"other"} ┆ .... │\n# │     ┆ 0.0060...                 ┆                                     ┆                   ┆      │\n# └─────┴───────────────────────────┴─────────────────────────────────────┴───────────────────┴──────┘\n```\n\n\n### Iterating over a Dataset documents and queries\n\nIterating over documents is useful for upserting but also for different updating. Iterating over queries is helpful in benchmarking\n\n```python\n\n# List Iterator, where every list of size N Dicts with ("id", "metadata", "values", "sparse_values")\ndataset.iter_documents(batch_size=n) \n\ndataset.iter_queries()\n\n```\n\n### upserting to Index\n\n```bash\npip install pinecone-client\n```\n\n```python\nimport pinecone\npinecone.init(api_key="API_KEY", environment="us-west1-gcp")\n\npinecone.create_index(name="my-index", dimension=384, pod_type=\'s1\')\n\nindex = pinecone.Index("my-index")\n\n# you can iterate over documents in batches\nfor batch in dataset.iter_documents(batch_size=100):\n    index.upsert(vectors=batch)\n\n# or upsert the dataset as dataframe\nindex.upsert_from_dataframe(dataset.drop(columns=["blob"]))\n\n# using gRPC\nindex = pinecone.GRPCIndex("my-index")\n```\n\n## Advanced Usage\n\n### Working with your own dataset storage\n\nDatasets is using Pinecone\'s public datasets bucket on GCS, you can use your own bucket by setting the `PINECONE_DATASETS_EDNPOINT` environment variable.\n\n```bash\nexport PINECONE_DATASETS_ENDPOINT="gs://my-bucket"\n```\n\nthis will change the default endpoint to your bucket, and upon calling `list_datasets` or `load_dataset` it will scan your bucket and list all datasets.\n\nNote that you can also use `s3://` as a prefix to your bucket.\n\n### Authenication to your own bucket\n\nFor now, Pinecone Datastes supports only GCS and S3 buckets, and with default authentication as provided by the fsspec implementation, respectively: `gcsfs` and `s3fs`.\n\n### Using aws key/secret authentication methods\n\nfirst, to set a new endpoint, set the environment variable `PINECONE_DATASETS_ENDPOINT` to your bucket.\n\n```bash\nexport PINECONE_DATASETS_ENDPOINT="s3://my-bucket"\n```\n\nthen, you can use the `key` and `secret` parameters to pass your credentials to the `list_datasets` and `load_dataset` functions.\n\n```python\nst = list_datasets(\n        key=os.environ.get("S3_ACCESS_KEY"),\n        secret=os.environ.get("S3_SECRET"),\n    )\n\nds = load_dataset(\n        "test_dataset",\n        key=os.environ.get("S3_ACCESS_KEY"),\n        secret=os.environ.get("S3_SECRET"),\n)\n```\n\n## For developers\n\nThis project is using poetry for dependency managemet. supported python version are 3.8+. To start developing, on project root directory run:\n\n```bash\npoetry install --with dev\n```\n\nTo run test locally run \n\n```bash\npoetry run pytest --cov pinecone_datasets\n```\n\nTo create a pinecone-public dataset you may need to generate a dataset metadata. For example:\n\n```python\nfrom pinecone_datasets.catalog import DatasetMetadata\n\nmeta = DatasetMetadata(\n    name="test_dataset",\n    created_at="2023-02-17 14:17:01.481785",\n    documents=2,\n    queries=2,\n    source="manual",\n    bucket="LOCAL",\n    task="unittests",\n    dense_model={"name": "bert", "dimension": 3},\n    sparse_model={"name": "bm25"},\n)\n```\n\nto see the complete schema you can run:\n\n```python\nmeta.schema()\n```\n\nin order to list a dataset you can save dataset metadata (NOTE: write permission to loacaion is needed)\n\n```python\ndataset._save_metadata("non-listed-dataset", meta)\n```\n\n### Uploading and listing a dataset. \n\npinecone datasets can load dataset from every storage where it has access (using the default access: s3, gcs or local permissions)\n\n we expect data to be uploaded to the following directory structure:\n\n    ├── base_path                     # path to where all datasets\n    │   ├── dataset_id                # name of dataset\n    │   │   ├── metadata.json         # dataset metadata (optional, only for listed)\n    │   │   ├── documents             # datasets documents\n    │   │   │   ├── file1.parquet      \n    │   │   │   └── file2.parquet      \n    │   │   ├── queries               # dataset queries\n    │   │   │   ├── file1.parquet  \n    │   │   │   └── file2.parquet   \n    └── ...\n\na listed dataset is a dataset that is loaded and listed using `load_dataset` and `list_dataset`\npinecone datasets will scan storage and will list every dataset with metadata file, for example: `s3://my-bucket/my-dataset/metadata.json`\n\n### Accessing a non-listed dataset\n\nto access a non listed dataset you can directly load it via:\n\n```python\nfrom pinecone_datasets import Dataset\n\ndataset = Dataset("non-listed-dataset")\n```\n\n\n',
+    'long_description': '# Pinecone Datasets\n\n## install\n\n```bash\npip install pinecone-datasets\n```\n\n## Usage\n\nYou can use Pinecone Datasets to load our public datasets or with your own dataset.\n\n### Loading Pinecone Public Datasets\n\n```python\nfrom pinecone_datasets import list_datasets, load_dataset\n\nlist_datasets()\n# ["quora_all-MiniLM-L6-bm25", ... ]\n\ndataset = load_dataset("quora_all-MiniLM-L6-bm25")\n\ndataset.head()\n\n# Prints\n# ┌─────┬───────────────────────────┬─────────────────────────────────────┬───────────────────┬──────┐\n# │ id  ┆ values                    ┆ sparse_values                       ┆ metadata          ┆ blob │\n# │     ┆                           ┆                                     ┆                   ┆      │\n# │ str ┆ list[f32]                 ┆ struct[2]                           ┆ struct[3]         ┆      │\n# ╞═════╪═══════════════════════════╪═════════════════════════════════════╪═══════════════════╪══════╡\n# │ 0   ┆ [0.118014, -0.069717, ... ┆ {[470065541, 52922727, ... 22364... ┆ {2017,12,"other"} ┆ .... │\n# │     ┆ 0.0060...                 ┆                                     ┆                   ┆      │\n# └─────┴───────────────────────────┴─────────────────────────────────────┴───────────────────┴──────┘\n```\n\n\n### Iterating over a Dataset documents and queries\n\nIterating over documents is useful for upserting but also for different updating. Iterating over queries is helpful in benchmarking\n\n```python\n\n# List Iterator, where every list of size N Dicts with ("id", "metadata", "values", "sparse_values")\ndataset.iter_documents(batch_size=n) \n\ndataset.iter_queries()\n\n```\n\n### upserting to Index\n\n```bash\npip install pinecone-client\n```\n\n```python\nimport pinecone\npinecone.init(api_key="API_KEY", environment="us-west1-gcp")\n\npinecone.create_index(name="my-index", dimension=384, pod_type=\'s1\')\n\nindex = pinecone.Index("my-index")\n\n# you can iterate over documents in batches\nfor batch in dataset.iter_documents(batch_size=100):\n    index.upsert(vectors=batch)\n\n# or upsert the dataset as dataframe\nindex.upsert_from_dataframe(dataset.drop(columns=["blob"]))\n\n# using gRPC\nindex = pinecone.GRPCIndex("my-index")\n```\n\n## Advanced Usage\n\n### Working with your own dataset storage\n\nDatasets is using Pinecone\'s public datasets bucket on GCS, you can use your own bucket by setting the `DATASETS_CATALOG_BASEPATH` environment variable.\n\n```bash\nexport PINECONE_DATASETS_ENDPOINT="gs://my-bucket"\n```\n\nthis will change the default endpoint to your bucket, and upon calling `list_datasets` or `load_dataset` it will scan your bucket and list all datasets.\n\nNote that you can also use `s3://` as a prefix to your bucket.\n\n### Authenication to your own bucket\n\nFor now, Pinecone Datastes supports only GCS and S3 buckets, and with default authentication as provided by the fsspec implementation, respectively: `gcsfs` and `s3fs`.\n\n### Using aws key/secret authentication methods\n\nfirst, to set a new endpoint, set the environment variable `PINECONE_DATASETS_ENDPOINT` to your bucket.\n\n```bash\nexport PINECONE_DATASETS_ENDPOINT="s3://my-bucket"\n```\n\nthen, you can use the `key` and `secret` parameters to pass your credentials to the `list_datasets` and `load_dataset` functions.\n\n```python\nst = list_datasets(\n        key=os.environ.get("S3_ACCESS_KEY"),\n        secret=os.environ.get("S3_SECRET"),\n    )\n\nds = load_dataset(\n        "test_dataset",\n        key=os.environ.get("S3_ACCESS_KEY"),\n        secret=os.environ.get("S3_SECRET"),\n)\n```\n\n## For developers\n\nThis project is using poetry for dependency managemet. supported python version are 3.8+. To start developing, on project root directory run:\n\n```bash\npoetry install --with dev\n```\n\nTo run test locally run \n\n```bash\npoetry run pytest --cov pinecone_datasets\n```\n\nTo create a pinecone-public dataset you may need to generate a dataset metadata. For example:\n\n```python\nfrom pinecone_datasets.catalog import DatasetMetadata\n\nmeta = DatasetMetadata(\n    name="test_dataset",\n    created_at="2023-02-17 14:17:01.481785",\n    documents=2,\n    queries=2,\n    source="manual",\n    bucket="LOCAL",\n    task="unittests",\n    dense_model={"name": "bert", "dimension": 3},\n    sparse_model={"name": "bm25"},\n)\n```\n\nto see the complete schema you can run:\n\n```python\nmeta.schema()\n```\n\nin order to list a dataset you can save dataset metadata (NOTE: write permission to loacaion is needed)\n\n```python\ndataset = Dataset("non-listed-dataset")\ndataset._save_metadata(meta)\n```\n\n### Uploading and listing a dataset. \n\npinecone datasets can load dataset from every storage where it has access (using the default access: s3, gcs or local permissions)\n\n we expect data to be uploaded to the following directory structure:\n\n    ├── base_path                     # path to where all datasets\n    │   ├── dataset_id                # name of dataset\n    │   │   ├── metadata.json         # dataset metadata (optional, only for listed)\n    │   │   ├── documents             # datasets documents\n    │   │   │   ├── file1.parquet      \n    │   │   │   └── file2.parquet      \n    │   │   ├── queries               # dataset queries\n    │   │   │   ├── file1.parquet  \n    │   │   │   └── file2.parquet   \n    └── ...\n\na listed dataset is a dataset that is loaded and listed using `load_dataset` and `list_dataset`\npinecone datasets will scan storage and will list every dataset with metadata file, for example: `s3://my-bucket/my-dataset/metadata.json`\n\n### Accessing a non-listed dataset\n\nto access a non listed dataset you can directly load it via:\n\n```python\nfrom pinecone_datasets import Dataset\n\ndataset = Dataset("non-listed-dataset")\n```\n\n\n',
     'author': 'Pinecone',
     'author_email': 'None',
     'maintainer': 'Roy Miara',
     'maintainer_email': 'miararoy@gmail.com',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pinecone_datasets-0.3.1a0/PKG-INFO` & `pinecone_datasets-0.4.0a0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 Metadata-Version: 2.1
 Name: pinecone-datasets
-Version: 0.3.1a0
+Version: 0.4.0a0
 Summary: Pinecone Datasets lets you easily load datasets into your Pinecone index.
 Author: Pinecone
 Maintainer: Roy Miara
 Maintainer-email: miararoy@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fsspec (>=2023.1.0,<2024.0.0)
 Requires-Dist: gcsfs (>=2023.1.0,<2024.0.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: polars (>=0.16.4,<0.17.0)
 Requires-Dist: protobuf (>=3.19.3,<3.20.0)
-Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
+Requires-Dist: pyarrow (>=12.0.0,<13.0.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: s3fs (>=2023.1.0,<2024.0.0)
 Description-Content-Type: text/markdown
 
 # Pinecone Datasets
 
+## install
+
+```bash
+pip install pinecone-datasets
+```
+
 ## Usage
 
 You can use Pinecone Datasets to load our public datasets or with your own dataset.
 
 ### Loading Pinecone Public Datasets
 
 ```python
@@ -89,15 +95,15 @@
 index = pinecone.GRPCIndex("my-index")
 ```
 
 ## Advanced Usage
 
 ### Working with your own dataset storage
 
-Datasets is using Pinecone's public datasets bucket on GCS, you can use your own bucket by setting the `PINECONE_DATASETS_EDNPOINT` environment variable.
+Datasets is using Pinecone's public datasets bucket on GCS, you can use your own bucket by setting the `DATASETS_CATALOG_BASEPATH` environment variable.
 
 ```bash
 export PINECONE_DATASETS_ENDPOINT="gs://my-bucket"
 ```
 
 this will change the default endpoint to your bucket, and upon calling `list_datasets` or `load_dataset` it will scan your bucket and list all datasets.
 
@@ -167,15 +173,16 @@
 ```python
 meta.schema()
 ```
 
 in order to list a dataset you can save dataset metadata (NOTE: write permission to loacaion is needed)
 
 ```python
-dataset._save_metadata("non-listed-dataset", meta)
+dataset = Dataset("non-listed-dataset")
+dataset._save_metadata(meta)
 ```
 
 ### Uploading and listing a dataset. 
 
 pinecone datasets can load dataset from every storage where it has access (using the default access: s3, gcs or local permissions)
 
  we expect data to be uploaded to the following directory structure:
```

