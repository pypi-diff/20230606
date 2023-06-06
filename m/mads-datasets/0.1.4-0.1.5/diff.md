# Comparing `tmp/mads_datasets-0.1.4.tar.gz` & `tmp/mads_datasets-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mads_datasets-0.1.4.tar", max compression
+gzip compressed data, was "mads_datasets-0.1.5.tar", max compression
```

## Comparing `mads_datasets-0.1.4.tar` & `mads_datasets-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-06-05 10:06:45.165441 mads_datasets-0.1.4/README.md
--rw-r--r--   0        0        0      164 2023-06-06 09:55:29.933711 mads_datasets-0.1.4/mads_datasets/__init__.py
--rw-r--r--   0        0        0    15354 2023-06-06 09:55:31.515738 mads_datasets-0.1.4/mads_datasets/datasetfactory.py
--rw-r--r--   0        0        0     5057 2023-06-06 09:56:28.815925 mads_datasets-0.1.4/mads_datasets/datasets.py
--rw-r--r--   0        0        0     4778 2023-06-05 10:37:07.673949 mads_datasets-0.1.4/mads_datasets/datatools.py
--rw-r--r--   0        0        0     3251 2023-06-06 08:42:57.768632 mads_datasets-0.1.4/mads_datasets/settings.py
--rw-r--r--   0        0        0      974 2023-06-06 09:56:59.047704 mads_datasets-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 mads_datasets-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-05 10:06:45.165441 mads_datasets-0.1.5/README.md
+-rw-r--r--   0        0        0      164 2023-06-06 09:55:29.933711 mads_datasets-0.1.5/mads_datasets/__init__.py
+-rw-r--r--   0        0        0    15387 2023-06-06 10:23:56.869646 mads_datasets-0.1.5/mads_datasets/datasetfactory.py
+-rw-r--r--   0        0        0     5057 2023-06-06 09:56:28.815925 mads_datasets-0.1.5/mads_datasets/datasets.py
+-rw-r--r--   0        0        0     4778 2023-06-05 10:37:07.673949 mads_datasets-0.1.5/mads_datasets/datatools.py
+-rw-r--r--   0        0        0     3251 2023-06-06 08:42:57.768632 mads_datasets-0.1.5/mads_datasets/settings.py
+-rw-r--r--   0        0        0      974 2023-06-06 10:26:31.136041 mads_datasets-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 mads_datasets-0.1.5/PKG-INFO
```

### Comparing `mads_datasets-0.1.4/mads_datasets/datasetfactory.py` & `mads_datasets-0.1.5/mads_datasets/datasetfactory.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,31 +65,28 @@
 
 
 T = TypeVar("T", bound=DatasetSettings)
 
 
 class AbstractDatasetFactory(ABC, Generic[T]):
     def __init__(
-        self, settings: T, preprocessor: Type[PreprocessorProtocol], **kwargs: Any
+        self, settings: T, preprocessor: Type[PreprocessorProtocol], datadir: Path
     ) -> None:
         self._settings = settings
-        self.data_dir = Path(
-            kwargs.get("datadir", Path.home() / ".cache/mads_datasets")
-        )
         self.preprocessor = preprocessor
+        self.datadir = datadir
 
     @property
     def settings(self) -> T:
         return self._settings
 
     def download_data(self) -> None:
         url = self._settings.dataset_url
         filename = self._settings.filename
-        datadir = self.data_dir
-        self.subfolder = Path(datadir) / self.settings.name
+        self.subfolder = Path(self.datadir) / self.settings.name
         if not self.subfolder.exists():
             logger.info("Start download...")
             self.subfolder.mkdir(parents=True)
             self.filepath = get_file(self.subfolder, filename, url=url, overwrite=False)
         else:
             logger.info(f"Dataset already exists at {self.subfolder}")
             self.filepath = self.subfolder / filename
@@ -382,38 +379,41 @@
         else:
             return 1
 
 
 class DatasetFactoryProvider:
     @staticmethod
     def create_factory(dataset_type: DatasetType, **kwargs) -> AbstractDatasetFactory:
+        datadir = Path(
+            kwargs.get("datadir", Path.home() / ".cache/mads_datasets")
+        )
         if dataset_type == DatasetType.FLOWERS:
             preprocessor = kwargs.get("preprocessor", BasePreprocessor)
             return FlowersDatasetFactory(
-                flowersdatasetsettings, preprocessor=preprocessor, **kwargs
+                flowersdatasetsettings, preprocessor=preprocessor, datadir=datadir
             )
         if dataset_type == DatasetType.IMDB:
             preprocessor = kwargs.get("preprocessor", IMDBTokenizer)
             return IMDBDatasetFactory(
-                imdbdatasetsettings, preprocessor=preprocessor, **kwargs
+                imdbdatasetsettings, preprocessor=preprocessor, datadir=datadir
             )
         if dataset_type == DatasetType.GESTURES:
             preprocessor = kwargs.get("preprocessor", PaddedPreprocessor)
             return GesturesDatasetFactory(
-                gesturesdatasetsettings, preprocessor=preprocessor, **kwargs
+                gesturesdatasetsettings, preprocessor=preprocessor, datadir=datadir
             )
         if dataset_type == DatasetType.FASHION:
             preprocessor = kwargs.get("preprocessor", BasePreprocessor)
             return FashionDatasetFactory(
-                fashionmnistsettings, preprocessor=preprocessor, **kwargs
+                fashionmnistsettings, preprocessor=preprocessor, datadir=datadir
             )
         if dataset_type == DatasetType.SUNSPOTS:
             preprocessor = kwargs.get("preprocessor", BasePreprocessor)
             return SunspotsDatasetFactory(
-                sunspotsettings, preprocessor=preprocessor, **kwargs
+                sunspotsettings, preprocessor=preprocessor, datadir=datadir
             )
 
         raise ValueError(f"Invalid dataset type: {dataset_type}")
 
 
 class BaseDatastreamer:
     """This datastreamer wil never stop
```

### Comparing `mads_datasets-0.1.4/mads_datasets/datasets.py` & `mads_datasets-0.1.5/mads_datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.1.4/mads_datasets/datatools.py` & `mads_datasets-0.1.5/mads_datasets/datatools.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.1.4/mads_datasets/settings.py` & `mads_datasets-0.1.5/mads_datasets/settings.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.1.4/pyproject.toml` & `mads_datasets-0.1.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mads-datasets"
-version = "0.1.4"
+version = "0.1.5"
 description = "Datasets for the master applied data science"
 authors = ["Raoul Grouls <Raoul.Grouls@han.nl>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "mads_datasets"}]
 
 [tool.poetry.dependencies]
```

### Comparing `mads_datasets-0.1.4/PKG-INFO` & `mads_datasets-0.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mads-datasets
-Version: 0.1.4
+Version: 0.1.5
 Summary: Datasets for the master applied data science
 License: MIT
 Author: Raoul Grouls
 Author-email: Raoul.Grouls@han.nl
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

