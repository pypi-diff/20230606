# Comparing `tmp/darwin_py-0.8.9.tar.gz` & `tmp/darwin_py-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "darwin_py-0.8.9.tar", max compression
+gzip compressed data, was "darwin_py-0.9.0.tar", max compression
```

## Comparing `darwin_py-0.8.9.tar` & `darwin_py-0.9.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     1064 2023-02-01 12:54:33.569176 darwin_py-0.8.9/LICENSE
--rw-r--r--   0        0        0     4981 2023-02-01 12:54:33.569176 darwin_py-0.8.9/README.md
--rw-r--r--   0        0        0      168 2023-02-01 12:54:33.569176 darwin_py-0.8.9/darwin/__init__.py
--rw-r--r--   0        0        0     7062 2023-02-01 12:54:33.569176 darwin_py-0.8.9/darwin/backend_v2.py
--rw-r--r--   0        0        0     6172 2023-02-01 12:54:33.569176 darwin_py-0.8.9/darwin/cli.py
--rw-r--r--   0        0        0    44940 2023-02-01 12:54:33.569176 darwin_py-0.8.9/darwin/cli_functions.py
--rw-r--r--   0        0        0    42758 2023-02-01 12:54:33.569176 darwin_py-0.8.9/darwin/client.py
--rw-r--r--   0        0        0     8219 2023-02-01 12:54:33.569176 darwin_py-0.8.9/darwin/config.py
--rw-r--r--   0        0        0      126 2023-02-01 12:54:33.569176 darwin_py-0.8.9/darwin/dataset/__init__.py
--rw-r--r--   0        0        0    18108 2023-02-01 12:54:33.569176 darwin_py-0.8.9/darwin/dataset/download_manager.py
--rw-r--r--   0        0        0     3013 2023-02-01 12:54:33.569176 darwin_py-0.8.9/darwin/dataset/identifier.py
--rw-r--r--   0        0        0    16882 2023-02-01 12:54:33.569176 darwin_py-0.8.9/darwin/dataset/local_dataset.py
--rw-r--r--   0        0        0     6704 2023-02-01 12:54:33.569176 darwin_py-0.8.9/darwin/dataset/release.py
--rw-r--r--   0        0        0    31175 2023-02-01 12:54:33.569176 darwin_py-0.8.9/darwin/dataset/remote_dataset.py
--rw-r--r--   0        0        0    18078 2023-02-01 12:54:33.569176 darwin_py-0.8.9/darwin/dataset/remote_dataset_v1.py
--rw-r--r--   0        0        0    17878 2023-02-01 12:54:33.569176 darwin_py-0.8.9/darwin/dataset/remote_dataset_v2.py
--rw-r--r--   0        0        0    15702 2023-02-01 12:54:33.569176 darwin_py-0.8.9/darwin/dataset/split_manager.py
--rw-r--r--   0        0        0    21033 2023-02-01 12:54:33.569176 darwin_py-0.8.9/darwin/dataset/upload_manager.py
--rw-r--r--   0        0        0    22754 2023-02-01 12:54:33.569176 darwin_py-0.8.9/darwin/dataset/utils.py
--rw-r--r--   0        0        0    27513 2023-02-01 12:54:33.569176 darwin_py-0.8.9/darwin/datatypes.py
--rw-r--r--   0        0        0      536 2023-02-01 12:54:33.569176 darwin_py-0.8.9/darwin/doc_enum.py
--rw-r--r--   0        0        0     7151 2023-02-01 12:54:33.569176 darwin_py-0.8.9/darwin/exceptions.py
--rw-r--r--   0        0        0      489 2023-02-01 12:54:33.569176 darwin_py-0.8.9/darwin/exporter/__init__.py
--rw-r--r--   0        0        0     2026 2023-02-01 12:54:33.569176 darwin_py-0.8.9/darwin/exporter/exporter.py
--rw-r--r--   0        0        0      339 2023-02-01 12:54:33.569176 darwin_py-0.8.9/darwin/exporter/formats/__init__.py
--rw-r--r--   0        0        0    19405 2023-02-01 12:54:33.569176 darwin_py-0.8.9/darwin/exporter/formats/coco.py
--rw-r--r--   0        0        0    12170 2023-02-01 12:54:33.569176 darwin_py-0.8.9/darwin/exporter/formats/cvat.py
--rw-r--r--   0        0        0     3275 2023-02-01 12:54:33.569176 darwin_py-0.8.9/darwin/exporter/formats/darwin.py
--rw-r--r--   0        0        0     5362 2023-02-01 12:54:33.569176 darwin_py-0.8.9/darwin/exporter/formats/darwin_1_0.py
--rw-r--r--   0        0        0     5709 2023-02-01 12:54:33.569176 darwin_py-0.8.9/darwin/exporter/formats/dataloop.py
--rw-r--r--   0        0        0     2215 2023-02-01 12:54:33.569176 darwin_py-0.8.9/darwin/exporter/formats/instance_mask.py
--rw-r--r--   0        0        0     4260 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/exporter/formats/mask.py
--rw-r--r--   0        0        0     8433 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/exporter/formats/nifti.py
--rw-r--r--   0        0        0      823 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/exporter/formats/numpy_encoder.py
--rw-r--r--   0        0        0     8626 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/exporter/formats/pascalvoc.py
--rw-r--r--   0        0        0      659 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/exporter/formats/semantic_mask.py
--rw-r--r--   0        0        0      328 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/exporter/formats/semantic_mask_grey.py
--rw-r--r--   0        0        0      329 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/exporter/formats/semantic_mask_index.py
--rw-r--r--   0        0        0     3075 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/exporter/formats/yolo.py
--rw-r--r--   0        0        0      429 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/importer/__init__.py
--rw-r--r--   0        0        0      304 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/importer/formats/__init__.py
--rw-r--r--   0        0        0     7295 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/importer/formats/coco.py
--rw-r--r--   0        0        0     1286 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/importer/formats/csv_tags.py
--rw-r--r--   0        0        0     1941 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/importer/formats/csv_tags_video.py
--rw-r--r--   0        0        0      651 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/importer/formats/darwin.py
--rw-r--r--   0        0        0     2539 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/importer/formats/dataloop.py
--rw-r--r--   0        0        0     6785 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/importer/formats/labelbox.py
--rw-r--r--   0        0        0     6723 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/importer/formats/labelbox_schemas.py
--rw-r--r--   0        0        0    11225 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/importer/formats/nifti.py
--rw-r--r--   0        0        0      656 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/importer/formats/nifti_schemas.py
--rw-r--r--   0        0        0     4175 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/importer/formats/pascal_voc.py
--rw-r--r--   0        0        0    13243 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/importer/formats/superannotate.py
--rw-r--r--   0        0        0     8387 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/importer/formats/superannotate_schemas.py
--rw-r--r--   0        0        0    19782 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/importer/importer.py
--rw-r--r--   0        0        0     4714 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/item.py
--rw-r--r--   0        0        0     3602 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/item_sorter.py
--rw-r--r--   0        0        0    15168 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/options.py
--rw-r--r--   0        0        0     1159 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/path_utils.py
--rw-r--r--   0        0        0      684 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/torch/__init__.py
--rw-r--r--   0        0        0    21505 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/torch/dataset.py
--rw-r--r--   0        0        0     9389 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/torch/transforms.py
--rw-r--r--   0        0        0     4962 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/torch/utils.py
--rw-r--r--   0        0        0    34934 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/utils.py
--rw-r--r--   0        0        0     1267 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/validators.py
--rw-r--r--   0        0        0       22 2023-02-01 12:54:33.573176 darwin_py-0.8.9/darwin/version/__init__.py
--rw-r--r--   0        0        0     2833 2023-02-01 12:54:33.573176 darwin_py-0.8.9/pyproject.toml
--rw-r--r--   0        0        0     7500 1970-01-01 00:00:00.000000 darwin_py-0.8.9/setup.py
--rw-r--r--   0        0        0     7528 1970-01-01 00:00:00.000000 darwin_py-0.8.9/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-02-07 15:30:19.780017 darwin_py-0.9.0/LICENSE
+-rw-r--r--   0        0        0     4981 2023-02-07 15:30:19.784017 darwin_py-0.9.0/README.md
+-rw-r--r--   0        0        0      168 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/__init__.py
+-rw-r--r--   0        0        0     7062 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/backend_v2.py
+-rw-r--r--   0        0        0     6172 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/cli.py
+-rw-r--r--   0        0        0    45216 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/cli_functions.py
+-rw-r--r--   0        0        0    42758 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/client.py
+-rw-r--r--   0        0        0     8219 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/config.py
+-rw-r--r--   0        0        0      126 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/dataset/__init__.py
+-rw-r--r--   0        0        0    18108 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/dataset/download_manager.py
+-rw-r--r--   0        0        0     3013 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/dataset/identifier.py
+-rw-r--r--   0        0        0    16882 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/dataset/local_dataset.py
+-rw-r--r--   0        0        0     6704 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/dataset/release.py
+-rw-r--r--   0        0        0    31175 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/dataset/remote_dataset.py
+-rw-r--r--   0        0        0    18078 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/dataset/remote_dataset_v1.py
+-rw-r--r--   0        0        0    17878 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/dataset/remote_dataset_v2.py
+-rw-r--r--   0        0        0    15702 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/dataset/split_manager.py
+-rw-r--r--   0        0        0    21033 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/dataset/upload_manager.py
+-rw-r--r--   0        0        0    22754 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/dataset/utils.py
+-rw-r--r--   0        0        0    28509 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/datatypes.py
+-rw-r--r--   0        0        0      536 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/doc_enum.py
+-rw-r--r--   0        0        0     7151 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/exceptions.py
+-rw-r--r--   0        0        0      489 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/exporter/__init__.py
+-rw-r--r--   0        0        0     2026 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/exporter/exporter.py
+-rw-r--r--   0        0        0      352 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/exporter/formats/__init__.py
+-rw-r--r--   0        0        0    19405 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/exporter/formats/coco.py
+-rw-r--r--   0        0        0    12170 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/exporter/formats/cvat.py
+-rw-r--r--   0        0        0     3275 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/exporter/formats/darwin.py
+-rw-r--r--   0        0        0     5349 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/exporter/formats/darwin_1_0.py
+-rw-r--r--   0        0        0     5709 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/exporter/formats/dataloop.py
+-rw-r--r--   0        0        0     2215 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/exporter/formats/instance_mask.py
+-rw-r--r--   0        0        0     4285 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/exporter/formats/mask.py
+-rw-r--r--   0        0        0     8433 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/exporter/formats/nifti.py
+-rw-r--r--   0        0        0      823 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/exporter/formats/numpy_encoder.py
+-rw-r--r--   0        0        0     8626 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/exporter/formats/pascalvoc.py
+-rw-r--r--   0        0        0      659 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/exporter/formats/semantic_mask.py
+-rw-r--r--   0        0        0      328 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/exporter/formats/semantic_mask_grey.py
+-rw-r--r--   0        0        0      329 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/exporter/formats/semantic_mask_index.py
+-rw-r--r--   0        0        0     3075 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/exporter/formats/yolo.py
+-rw-r--r--   0        0        0      429 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/importer/__init__.py
+-rw-r--r--   0        0        0      304 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/importer/formats/__init__.py
+-rw-r--r--   0        0        0     7295 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/importer/formats/coco.py
+-rw-r--r--   0        0        0     1286 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/importer/formats/csv_tags.py
+-rw-r--r--   0        0        0     1941 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/importer/formats/csv_tags_video.py
+-rw-r--r--   0        0        0      651 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/importer/formats/darwin.py
+-rw-r--r--   0        0        0     2539 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/importer/formats/dataloop.py
+-rw-r--r--   0        0        0     6785 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/importer/formats/labelbox.py
+-rw-r--r--   0        0        0     6723 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/importer/formats/labelbox_schemas.py
+-rw-r--r--   0        0        0    11225 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/importer/formats/nifti.py
+-rw-r--r--   0        0        0      656 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/importer/formats/nifti_schemas.py
+-rw-r--r--   0        0        0     4175 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/importer/formats/pascal_voc.py
+-rw-r--r--   0        0        0    13243 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/importer/formats/superannotate.py
+-rw-r--r--   0        0        0     8387 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/importer/formats/superannotate_schemas.py
+-rw-r--r--   0        0        0    19782 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/importer/importer.py
+-rw-r--r--   0        0        0     4714 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/item.py
+-rw-r--r--   0        0        0     3602 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/item_sorter.py
+-rw-r--r--   0        0        0    15168 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/options.py
+-rw-r--r--   0        0        0     1159 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/path_utils.py
+-rw-r--r--   0        0        0      684 2023-02-07 15:30:19.784017 darwin_py-0.9.0/darwin/torch/__init__.py
+-rw-r--r--   0        0        0    21694 2023-02-07 15:30:19.788017 darwin_py-0.9.0/darwin/torch/dataset.py
+-rw-r--r--   0        0        0     9389 2023-02-07 15:30:19.788017 darwin_py-0.9.0/darwin/torch/transforms.py
+-rw-r--r--   0        0        0     4962 2023-02-07 15:30:19.788017 darwin_py-0.9.0/darwin/torch/utils.py
+-rw-r--r--   0        0        0    34934 2023-02-07 15:30:19.788017 darwin_py-0.9.0/darwin/utils.py
+-rw-r--r--   0        0        0     1267 2023-02-07 15:30:19.788017 darwin_py-0.9.0/darwin/validators.py
+-rw-r--r--   0        0        0      635 2023-02-07 15:30:19.788017 darwin_py-0.9.0/darwin/version/__init__.py
+-rw-r--r--   0        0        0     2833 2023-02-07 15:30:19.788017 darwin_py-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     7500 1970-01-01 00:00:00.000000 darwin_py-0.9.0/setup.py
+-rw-r--r--   0        0        0     7528 1970-01-01 00:00:00.000000 darwin_py-0.9.0/PKG-INFO
```

### Comparing `darwin_py-0.8.9/LICENSE` & `darwin_py-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/README.md` & `darwin_py-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/backend_v2.py` & `darwin_py-0.9.0/darwin/backend_v2.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/cli.py` & `darwin_py-0.9.0/darwin/cli.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/cli_functions.py` & `darwin_py-0.9.0/darwin/cli_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,22 @@
 from darwin.config import Config
 from darwin.dataset import RemoteDataset
 from darwin.dataset.identifier import DatasetIdentifier
 from darwin.dataset.release import Release
 from darwin.dataset.split_manager import split_dataset
 from darwin.dataset.upload_manager import LocalFile
 from darwin.dataset.utils import get_release_path
-from darwin.datatypes import ExportParser, ImportParser, PathLike, Team
+from darwin.datatypes import (
+    ExportParser,
+    ImportParser,
+    NumberLike,
+    PathLike,
+    Team,
+    UnknownType,
+)
 from darwin.exceptions import (
     AnnotationFileValidationError,
     IncompatibleOptions,
     InvalidLogin,
     MissingConfig,
     MissingSchema,
     NameTaken,
@@ -650,19 +657,19 @@
         with Live(progress_table):
             sync_task: TaskID = sync_metadata.add_task("")
             file_tasks: Dict[str, TaskID] = {}
             overall_task = overall_progress.add_task(
                 "[green]Total progress", filename="Total progress", total=0, visible=False
             )
 
-            def progress_callback(total_file_count, file_advancement):
+            def progress_callback(total_file_count: NumberLike, file_advancement: NumberLike) -> None:
                 sync_metadata.update(sync_task, visible=False)
                 overall_progress.update(overall_task, total=total_file_count, advance=file_advancement, visible=True)
 
-            def file_upload_callback(file_name, file_total_bytes, file_bytes_sent):
+            def file_upload_callback(file_name: str, file_total_bytes: NumberLike, file_bytes_sent: NumberLike) -> None:
                 if file_name not in file_tasks:
                     file_tasks[file_name] = file_progress.add_task(
                         f"[blue]{file_name}", filename=file_name, total=file_total_bytes
                     )
 
                 # Rich has a concurrency issue, so sometimes updating progress
                 # or removing a task fails. Wrapping this logic around a try/catch block
@@ -694,15 +701,15 @@
         if not upload_manager.blocked_count and not upload_manager.error_count:
             console.print(f"All {upload_manager.total_count} files have been successfully uploaded.\n", style="success")
             return
 
         already_existing_items = []
         other_skipped_items = []
         for item in upload_manager.blocked_items:
-            if item.reason.upper() == "ALREADY_EXISTS":
+            if item.reason is not None and item.reason.upper() == "ALREADY_EXISTS":
                 already_existing_items.append(item)
             else:
                 other_skipped_items.append(item)
 
         if already_existing_items:
             console.print(
                 f"Skipped {len(already_existing_items)} files already in the dataset.\n",
@@ -760,14 +767,16 @@
 def dataset_import(
     dataset_slug: str,
     format: str,
     files: List[PathLike],
     append: bool,
     class_prompt: bool = True,
     delete_for_empty: bool = False,
+    import_annotators: bool = False,
+    import_reviewers: bool = False,
 ) -> None:
     """
     Imports annotation files to the given dataset.
     Exits the application if no dataset with the given slug is found.
 
     Parameters
     ----------
@@ -835,15 +844,15 @@
         If True, only prints the filenames, if False it prints the full file url.
     sort_by: Optional[str]
         Sort order for listing files. Defaults to 'updated_at:desc'.
     """
     client: Client = _load_client(dataset_identifier=dataset_slug)
     try:
         dataset: RemoteDataset = client.get_remote_dataset(dataset_identifier=dataset_slug)
-        filters: Dict[str, Any] = {}
+        filters: Dict[str, UnknownType] = {}
 
         if statuses:
             for status in statuses.split(","):
                 if not _has_valid_status(status):
                     _error(f"Invalid status '{status}', available statuses: annotate, archived, complete, new, review")
             filters["statuses"] = statuses
         else:
@@ -858,15 +867,15 @@
         table: Table = Table(show_header=True, header_style="bold cyan")
         table.add_column("Name", justify="left")
 
         if not only_filenames:
             table.add_column("Status", justify="left")
             table.add_column("URL", justify="left")
 
-        for file in dataset.fetch_remote_files(filters, sort_by):
+        for file in dataset.fetch_remote_files(filters, sort_by):  # type: ignore
             if only_filenames:
                 table.add_row(file.filename)
             else:
                 image_url = dataset.workview_url_for_item(file)
                 table.add_row(file.filename, f"{file.status if not file.archived else 'archived'}", image_url)
 
         Console().print(table)
@@ -907,15 +916,15 @@
         elif status == "restore-archived":
             dataset.restore_archived(items)
         elif status == "complete":
             dataset.complete(items)
     except NotFound as e:
         _error(f"No dataset with name '{e.name}'")
     except ValueError as e:
-        _error(e)
+        _error(str(e))
 
 
 def delete_files(dataset_slug: str, files: List[str], skip_user_confirmation: bool = False) -> None:
     """
     Deletes the files from the given dataset.
     Exits the application if no dataset with the given slug is found or a general error occurs.
 
@@ -1250,15 +1259,15 @@
     return Theme({"success": "bold green", "warning": "bold yellow", "error": "bold red"})
 
 
 def _has_valid_status(status: str) -> bool:
     return status in ["new", "annotate", "review", "complete", "archived"]
 
 
-def _print_new_json_format_warning(dataset):
+def _print_new_json_format_warning(dataset: RemoteDataset) -> None:
     console = Console(theme=_console_theme(), stderr=True)
     console.print(
         f"NOTE: Your dataset has been exported using new Darwin JSON 2.0 format.",
         f"    If you wish to use the legacy Darwin format, please use the following to convert: ",
         f"",
         f"    darwin convert darwin_1.0 {dataset.local_path} OUTPUT_DIR",
         f"",
```

### Comparing `darwin_py-0.8.9/darwin/client.py` & `darwin_py-0.9.0/darwin/client.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/config.py` & `darwin_py-0.9.0/darwin/config.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/dataset/download_manager.py` & `darwin_py-0.9.0/darwin/dataset/download_manager.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/dataset/identifier.py` & `darwin_py-0.9.0/darwin/dataset/identifier.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/dataset/local_dataset.py` & `darwin_py-0.9.0/darwin/dataset/local_dataset.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/dataset/release.py` & `darwin_py-0.9.0/darwin/dataset/release.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/dataset/remote_dataset.py` & `darwin_py-0.9.0/darwin/dataset/remote_dataset.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/dataset/remote_dataset_v1.py` & `darwin_py-0.9.0/darwin/dataset/remote_dataset_v1.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/dataset/remote_dataset_v2.py` & `darwin_py-0.9.0/darwin/dataset/remote_dataset_v2.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/dataset/split_manager.py` & `darwin_py-0.9.0/darwin/dataset/split_manager.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/dataset/upload_manager.py` & `darwin_py-0.9.0/darwin/dataset/upload_manager.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/dataset/utils.py` & `darwin_py-0.9.0/darwin/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/datatypes.py` & `darwin_py-0.9.0/darwin/datatypes.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,29 +12,58 @@
     Set,
     Tuple,
     Union,
 )
 
 from darwin.path_utils import construct_full_path
 
+UnknownType = Any  # type: ignore
+NumberLike = Union[int, float]
+
 Point = Dict[str, float]
 BoundingBox = Dict[str, float]
 Polygon = List[Point]
 ComplexPolygon = List[Polygon]
-Node = Dict[str, Any]
+Node = Dict[str, UnknownType]
 EllipseData = Dict[str, Union[float, Point]]
 CuboidData = Dict[str, Dict[str, float]]
 Segment = List[int]
 
 DarwinVersionNumber = Tuple[int, int, int]
 
 PathLike = Union[str, Path]
 ErrorHandler = Callable[[int, str], None]
 
 ItemId = Union[str, int]
+JSONFreeForm = Dict[str, Any]  # type: ignore
+
+
+class JSONType:
+    def __init__(self, **kwargs: JSONFreeForm):
+        self.__dict__.update(kwargs)
+
+    def to_json(self) -> JSONFreeForm:
+        return self.__dict__
+
+    @classmethod
+    def from_json(cls, json: JSONFreeForm) -> "JSONType":
+        return cls(**json)
+
+    @classmethod
+    def from_dict(cls, json: JSONFreeForm) -> "JSONType":
+        return cls(**json)
+
+
+class DictFreeForm:
+    def __init__(self, **kwargs: JSONFreeForm):
+        self.__dict__.update(kwargs)
+
+    @classmethod
+    def from_dict(cls, json: JSONFreeForm) -> "DictFreeForm":
+        return cls(**json)
 
 
 @dataclass
 class Team:
     """
     Definition of a V7 team.
     """
@@ -94,15 +123,15 @@
     """
 
     #: The type of this ``SubAnnotation``.
     annotation_type: str
 
     #: Any external data, in any format, relevant to this ``SubAnnotation``.
     #: Used for compatibility purposes with external formats.
-    data: Any
+    data: UnknownType
 
 
 @dataclass(frozen=True, eq=True)
 class AnnotationAuthor:
     """
     Represents an annotation's author
     """
@@ -121,15 +150,15 @@
     """
 
     #: The ``AnnotationClass`` from this ``Annotation``.
     annotation_class: AnnotationClass
 
     #: Any external data, in any format, relevant to this ``Annotation``.
     #: Used for compatibility purposes with external formats.
-    data: Any
+    data: UnknownType
 
     #: List of ``SubAnnotations`` belonging to this ``Annotation``.
     subs: List[SubAnnotation] = field(default_factory=list)
 
     #: V2 slots this annotation belogs to
     slot_names: List[str] = field(default_factory=list)
 
@@ -165,15 +194,15 @@
     Represents an Annotation that belongs to a Video.
     """
 
     #: The ``AnnotationClass`` from this ``VideoAnnotation``.
     annotation_class: AnnotationClass
 
     #: A dictionary of frames for this ``VideoAnnotation``.
-    frames: Dict[int, Any]
+    frames: Dict[int, UnknownType]
 
     #: The keyframes for this ``VideoAnnotation``.
     #: Keyframes are a selection of frames from the ``frames`` attribute.
     keyframes: Dict[int, bool]
 
     #: A list of ``Segment``\'s.
     segments: List[Segment]
@@ -187,16 +216,18 @@
     #: Authorship of the annotation (annotators)
     annotators: Optional[List[AnnotationAuthor]] = None
 
     #: Authorship of the annotation (reviewers)
     reviewers: Optional[List[AnnotationAuthor]] = None
 
     def get_data(
-        self, only_keyframes: bool = True, post_processing: Optional[Callable[[Annotation, Any], Any]] = None
-    ) -> Dict[str, Any]:
+        self,
+        only_keyframes: bool = True,
+        post_processing: Optional[Callable[[Annotation, UnknownType], UnknownType]] = None,
+    ) -> Dict:
         """
         Return the post-processed frames and the additional information from this
         ``VideoAnnotation`` in a dictionary with the format:
 
         .. code-block:: python
 
             {
@@ -220,32 +251,36 @@
         Returns
         -------
         Dict[str, Any]
             A dictionary containing the processed frames, the segments of this ``VideoAnnotation``
             and whether or not it is interpolated.
         """
         if not post_processing:
-            post_processing = lambda annotation, data: data
 
-        return {
+            def post_processing(annotation: Annotation, data: UnknownType) -> UnknownType:
+                return data  # type: ignore
+
+        output = {
             "frames": {
                 frame: {
                     **post_processing(
-                        self.frames[frame],
-                        {self.frames[frame].annotation_class.annotation_type: self.frames[frame].data},
+                        self.frames[frame],  # type: ignore
+                        {self.frames[frame].annotation_class.annotation_type: self.frames[frame].data},  # type: ignore
                     ),
-                    **{"keyframe": self.keyframes[frame]},
+                    **{"keyframe": self.keyframes[frame]},  # type: ignore
                 }
                 for frame in self.frames
                 if not only_keyframes or self.keyframes[frame]
             },
             "segments": self.segments,
             "interpolated": self.interpolated,
         }
 
+        return output
+
 
 @dataclass
 class Slot:
     #: Unique slot name in the item. Will be `None` when loading V1 exports.
     name: Optional[str]
 
     #: Type of slot, e.g. image or dicom
@@ -269,15 +304,15 @@
     #: A url for each of the existing sections.
     frame_urls: Optional[List[str]] = None
 
     #: Frames per second
     fps: Optional[float] = None
 
     #: Metadata of the slot
-    metadata: Optional[Dict[str, Any]] = None
+    metadata: Optional[Dict[str, UnknownType]] = None
 
 
 @dataclass
 class AnnotationFileVersion:
     """
     Version of the AnnotationFile
     """
@@ -712,15 +747,15 @@
     """
     return Annotation(AnnotationClass(class_name, "cuboid"), cuboid, subs or [], slot_names=slot_names or [])
 
 
 def make_table(
     class_name: str,
     bounding_box: BoundingBox,
-    cells: List[Dict[str, Any]],
+    cells: List[Dict[str, UnknownType]],
     subs: Optional[List[SubAnnotation]] = None,
     slot_names: Optional[List[str]] = None,
 ) -> Annotation:
     """
     Creates and returns a table annotation.
 
     Parameters
@@ -767,15 +802,15 @@
         subs or [],
         slot_names=slot_names or [],
     )
 
 
 def make_string(
     class_name: str,
-    sources: List[Dict[str, Any]],
+    sources: List[Dict[str, UnknownType]],
     subs: Optional[List[SubAnnotation]] = None,
     slot_names: Optional[List[str]] = None,
 ) -> Annotation:
     """
     Creates and returns a string annotation.
 
     Parameters
@@ -914,15 +949,15 @@
     -------
     SubAnnotation
         A text ``SubAnnotation``.
     """
     return SubAnnotation("text", text)
 
 
-def make_opaque_sub(type: str, data: Any) -> SubAnnotation:
+def make_opaque_sub(type: str, data: UnknownType) -> SubAnnotation:
     """
     Creates and returns a opaque sub-annotation.
 
     Parameters
     ----------
     type : str
         Type of this sub-annotation
@@ -957,15 +992,15 @@
     KeyFrame
         The created ``Keyframe``.
     """
     return {"idx": idx, "annotation": annotation}
 
 
 def make_video_annotation(
-    frames: Dict[int, Any],
+    frames: Dict[int, UnknownType],
     keyframes: Dict[int, bool],
     segments: List[Segment],
     interpolated: bool,
     slot_names: List[str],
 ) -> VideoAnnotation:
     """
     Creates and returns a ``VideoAnnotation``.
@@ -987,24 +1022,24 @@
         The created ``VideoAnnotation``.
 
     Raises
     ------
     ValueError
         If some of the frames have different annotation class names.
     """
-    first_annotation: Annotation = list(frames.values())[0]
-    if not all(frame.annotation_class.name == first_annotation.annotation_class.name for frame in frames.values()):
+    first_annotation: Annotation = list(frames.values())[0]  # type: ignore
+    if not all(frame.annotation_class.name == first_annotation.annotation_class.name for frame in frames.values()):  # type: ignore
         raise ValueError("invalid argument to make_video_annotation")
 
     return VideoAnnotation(
         first_annotation.annotation_class, frames, keyframes, segments, interpolated, slot_names=slot_names or []
     )
 
 
-def _maybe_add_bounding_box_data(data: Dict[str, Any], bounding_box: Optional[Dict]) -> Dict[str, Any]:
+def _maybe_add_bounding_box_data(data: Dict[str, UnknownType], bounding_box: Optional[Dict]) -> Dict[str, UnknownType]:
     if bounding_box:
         data["bounding_box"] = {
             "x": bounding_box["x"],
             "y": bounding_box["y"],
             "w": bounding_box["w"],
             "h": bounding_box["h"],
         }
```

### Comparing `darwin_py-0.8.9/darwin/doc_enum.py` & `darwin_py-0.9.0/darwin/doc_enum.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/exceptions.py` & `darwin_py-0.9.0/darwin/exceptions.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/exporter/exporter.py` & `darwin_py-0.9.0/darwin/exporter/exporter.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/exporter/formats/coco.py` & `darwin_py-0.9.0/darwin/exporter/formats/coco.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/exporter/formats/cvat.py` & `darwin_py-0.9.0/darwin/exporter/formats/cvat.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/exporter/formats/darwin.py` & `darwin_py-0.9.0/darwin/exporter/formats/darwin.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/exporter/formats/darwin_1_0.py` & `darwin_py-0.9.0/darwin/exporter/formats/darwin_1_0.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from pathlib import Path
-from typing import Any, Dict, Iterable, List, Union
+from typing import Any, Dict, Iterable, Union
 
 import orjson as json
 
 import darwin.datatypes as dt
-from darwin.exporter.formats.numpy_encoder import NumpyEncoder
 
 
 def export(annotation_files: Iterable[dt.AnnotationFile], output_dir: Path) -> None:
     for id, annotation_file in enumerate(annotation_files):
         _export_file(annotation_file, id, output_dir)
 
 
-def _export_file(annotation_file: dt.AnnotationFile, id: int, output_dir: Path):
+def _export_file(annotation_file: dt.AnnotationFile, id: int, output_dir: Path) -> None:
     output: Dict[str, Any] = _build_json(annotation_file)
     output_file_path: Path = (output_dir / annotation_file.filename).with_suffix(".json")
     with open(output_file_path, "w") as f:
-        op = json.dumps(output, option=json.OPT_INDENT_2 | json.OPT_SERIALIZE_NUMPY).decode("utf-8")
+        op = json.dumps(output, option=json.OPT_INDENT_2 | json.OPT_SERIALIZE_NUMPY | json.OPT_NON_STR_KEYS).decode(
+            "utf-8"
+        )
         f.write(op)
 
 
 def _build_json(annotation_file: dt.AnnotationFile):
     if annotation_file.is_video:
         return _build_video_json(annotation_file)
     else:
@@ -38,15 +39,15 @@
             "url": annotation_file.image_url,
             "thumbnail_url": annotation_file.image_thumbnail_url,
             "path": annotation_file.remote_path,
             "workview_url": annotation_file.workview_url,
             **_build_metadata(annotation_file),
         },
         "annotations": list(map(_build_annotation, annotation_file.annotations)),
-        "dataset": str(annotation_file.dataset_name)
+        "dataset": str(annotation_file.dataset_name),
     }
 
 
 def _build_video_json(annotation_file: dt.AnnotationFile):
     return {
         "image": {
             "seq": annotation_file.seq,
@@ -59,15 +60,15 @@
             "thumbnail_url": annotation_file.image_thumbnail_url,
             "url": annotation_file.image_url,
             "path": annotation_file.remote_path,
             "workview_url": annotation_file.workview_url,
             **_build_metadata(annotation_file),
         },
         "annotations": list(map(_build_annotation, annotation_file.annotations)),
-        "dataset": str(annotation_file.dataset_name)
+        "dataset": str(annotation_file.dataset_name),
     }
 
 
 def _build_annotation(annotation):
     if isinstance(annotation, dt.VideoAnnotation):
         return _build_video_annotation(annotation)
     else:
```

### Comparing `darwin_py-0.8.9/darwin/exporter/formats/dataloop.py` & `darwin_py-0.9.0/darwin/exporter/formats/dataloop.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/exporter/formats/instance_mask.py` & `darwin_py-0.9.0/darwin/exporter/formats/instance_mask.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/exporter/formats/mask.py` & `darwin_py-0.9.0/darwin/exporter/formats/mask.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,16 +49,16 @@
         RGB_color_list = list(map(lambda x: [int(e * 255) for e in colorsys.hsv_to_rgb(*x)], HSV_colors))
         # Now we add BG class with [0 0 0] RGB value
         RGB_color_list.insert(0, [0, 0, 0])
         palette_rgb = {c: rgb for c, rgb in zip(categories, RGB_color_list)}
         RGB_colors = [c for e in RGB_color_list for c in e]
 
     for annotation_file in annotation_files:
-        image_id = os.path.splitext(annotation_file.filename)[0]
-        outfile = masks_dir / f"{image_id}.png"
+        image_rel_path = os.path.splitext(annotation_file.full_path)[0].lstrip("/")
+        outfile = masks_dir / f"{image_rel_path}.png"
         outfile.parent.mkdir(parents=True, exist_ok=True)
 
         height = annotation_file.image_height
         width = annotation_file.image_width
         if height is None or width is None:
             raise ValueError(f"Annotation file {annotation_file.filename} references an image with no height or width")
```

### Comparing `darwin_py-0.8.9/darwin/exporter/formats/nifti.py` & `darwin_py-0.9.0/darwin/exporter/formats/nifti.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/exporter/formats/numpy_encoder.py` & `darwin_py-0.9.0/darwin/exporter/formats/numpy_encoder.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/exporter/formats/pascalvoc.py` & `darwin_py-0.9.0/darwin/exporter/formats/pascalvoc.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/exporter/formats/semantic_mask.py` & `darwin_py-0.9.0/darwin/exporter/formats/semantic_mask.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/exporter/formats/yolo.py` & `darwin_py-0.9.0/darwin/exporter/formats/yolo.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/importer/formats/coco.py` & `darwin_py-0.9.0/darwin/importer/formats/coco.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/importer/formats/csv_tags.py` & `darwin_py-0.9.0/darwin/importer/formats/csv_tags.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/importer/formats/csv_tags_video.py` & `darwin_py-0.9.0/darwin/importer/formats/csv_tags_video.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/importer/formats/darwin.py` & `darwin_py-0.9.0/darwin/importer/formats/darwin.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/importer/formats/dataloop.py` & `darwin_py-0.9.0/darwin/importer/formats/dataloop.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/importer/formats/labelbox.py` & `darwin_py-0.9.0/darwin/importer/formats/labelbox.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/importer/formats/labelbox_schemas.py` & `darwin_py-0.9.0/darwin/importer/formats/labelbox_schemas.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/importer/formats/nifti.py` & `darwin_py-0.9.0/darwin/importer/formats/nifti.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/importer/formats/nifti_schemas.py` & `darwin_py-0.9.0/darwin/importer/formats/nifti_schemas.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/importer/formats/pascal_voc.py` & `darwin_py-0.9.0/darwin/importer/formats/pascal_voc.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/importer/formats/superannotate.py` & `darwin_py-0.9.0/darwin/importer/formats/superannotate.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/importer/formats/superannotate_schemas.py` & `darwin_py-0.9.0/darwin/importer/formats/superannotate_schemas.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/importer/importer.py` & `darwin_py-0.9.0/darwin/importer/importer.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/item.py` & `darwin_py-0.9.0/darwin/item.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/item_sorter.py` & `darwin_py-0.9.0/darwin/item_sorter.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/options.py` & `darwin_py-0.9.0/darwin/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import sys
 from argparse import ArgumentParser, Namespace
 from typing import Tuple
 
 import argcomplete
 
 
-class Options(object):
+class Options:
     """
     Has functions to parse CLI options given by the user.
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
 
         self.parser: ArgumentParser = ArgumentParser(
             description="Command line tool to create/upload/download datasets on darwin."
         )
 
         subparsers = self.parser.add_subparsers(dest="command")
         subparsers.add_parser("help", help="Show this help message and exit.")
```

### Comparing `darwin_py-0.8.9/darwin/path_utils.py` & `darwin_py-0.9.0/darwin/path_utils.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/torch/__init__.py` & `darwin_py-0.9.0/darwin/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/torch/dataset.py` & `darwin_py-0.9.0/darwin/torch/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 from darwin.cli_functions import _error, _load_client
+from darwin.client import Client
 from darwin.dataset import LocalDataset
 from darwin.dataset.identifier import DatasetIdentifier
 from darwin.torch.transforms import (
     Compose,
     ConvertPolygonsToInstanceMasks,
     ConvertPolygonsToSemanticMask,
 )
@@ -21,14 +22,15 @@
 def get_dataset(
     dataset_slug: str,
     dataset_type: str,
     partition: Optional[str] = None,
     split: str = "default",
     split_type: str = "random",
     transform: Optional[List] = None,
+    client: Optional[Client] = None,
 ) -> LocalDataset:
     """
     Creates and returns a ``LocalDataset``.
 
     Parameters
     ----------
     dataset_slug : str
@@ -39,28 +41,31 @@
         Selects one of the partitions ``["train", "val", "test", None]``.
     split : str, default: "default"
         Selects the split that defines the percentages used.
     split_type : str, default: "random"
         Heuristic used to do the split ``[random, stratified]``.
     transform : Optional[List], default: None
         List of PyTorch transforms.
+    client : Optional[Client], default: None
+        Client to use to retrieve the dataset.
     """
     dataset_functions = {
         "classification": ClassificationDataset,
         "instance-segmentation": InstanceSegmentationDataset,
         "semantic-segmentation": SemanticSegmentationDataset,
         "object-detection": ObjectDetectionDataset,
     }
     dataset_function = dataset_functions.get(dataset_type)
     if not dataset_function:
         list_of_types = ", ".join(dataset_functions.keys())
         return _error(f"dataset_type needs to be one of '{list_of_types}'")
 
     identifier = DatasetIdentifier.parse(dataset_slug)
-    client = _load_client(offline=True)
+    if client is None:
+        client = _load_client(offline=True)
 
     for p in client.list_local_datasets(team_slug=identifier.team_slug):
         if identifier.dataset_slug == p.name:
             return dataset_function(
                 dataset_path=p,
                 partition=partition,
                 split=split,
```

### Comparing `darwin_py-0.8.9/darwin/torch/transforms.py` & `darwin_py-0.9.0/darwin/torch/transforms.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/torch/utils.py` & `darwin_py-0.9.0/darwin/torch/utils.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/utils.py` & `darwin_py-0.9.0/darwin/utils.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/darwin/validators.py` & `darwin_py-0.9.0/darwin/validators.py`

 * *Files identical despite different names*

### Comparing `darwin_py-0.8.9/pyproject.toml` & `darwin_py-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "darwin-py"
-version = "0.8.9" # update this when you change the version - See: https://peps.python.org/pep-0440/
+version = "0.9.0" # update this when you change the version - See: https://peps.python.org/pep-0440/
 description = "Library and command line interface for darwin.v7labs.com"
 homepage = "https://docs.v7labs.com/reference/getting-started-2"
 documentation = "https://darwin-py-sdk.v7labs.com/index.html"
 repository = "https://github.com/v7labs/darwin-py"
 authors = ["V7 <info@v7labs.com>"]
 readme = "README.md"
 license = "MIT"
```

### Comparing `darwin_py-0.8.9/setup.py` & `darwin_py-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
  ':python_version < "3.7"': ['dataclasses>=0.8,<0.9']}
 
 entry_points = \
 {'console_scripts': ['darwin = darwin.cli:main']}
 
 setup_kwargs = {
     'name': 'darwin-py',
-    'version': '0.8.9',
+    'version': '0.9.0',
     'description': 'Library and command line interface for darwin.v7labs.com',
     'long_description': '# V7 Darwin Python SDK\n\nOfficial library to manage datasets along with\n[V7 Darwin annotation platform](https://darwin.v7labs.com).\n\nDarwin-py can both be used from the [command line](#usage-as-a-command-line-interface-cli) and as a [python library](#usage-as-a-python-library).\n\nMain functions are (but not limited to):\n\n- Client authentication\n- Listing local and remote datasets\n- Create/remove datasets\n- Upload/download data to/from remote datasets\n- Direct integration with PyTorch dataloaders\n\nSupport tested for python 3.8.\n\n## Installation\n\n```\npip install darwin-py\n```\n\nYou can now type `darwin` in your terminal and access the command line interface.\n\nIf you wish to use the PyTorch bindings, then you can use the `ml` flag to install all the additional requirements\n\n```\npip install darwin-py[ml]\n```\n\nTo run test, first install the `test` extra package\n\n```\npip install darwin-py[test]\n```\n\n---\n\n## Usage as a Command Line Interface (CLI)\n\nOnce installed, `darwin` is accessible as a command line tool.\nA useful way to navigate the CLI usage is through the help command `-h/--help` which will\nprovide additional information for each command available.\n\n### Client Authentication\n\nTo perform remote operations on Darwin you first need to authenticate.\nThis requires a [team-specific API-key](https://darwin.v7labs.com/?settings=api-keys).\nIf you do not already have a Darwin account, you can [contact us](https://www.v7labs.com/contact) and we can set one up for you.\n\nTo start the authentication process:\n\n```\n$ darwin authenticate\nAPI key:\nMake example-team the default team? [y/N] y\nDatasets directory [~/.darwin/datasets]:\nAuthentication succeeded.\n```\n\nYou will be then prompted to enter your API-key, whether you want to set the corresponding team as\ndefault and finally the desired location on the local file system for the datasets of that team.\nThis process will create a configuration file at `~/.darwin/config.yaml`.\nThis file will be updated with future authentications for different teams.\n\n### Listing local and remote datasets\n\nLists a summary of local existing datasets\n\n```\n$ darwin dataset local\nNAME            IMAGES     SYNC_DATE         SIZE\nmydataset       112025     yesterday     159.2 GB\n```\n\nLists a summary of remote datasets accessible by the current user.\n\n```\n$ darwin dataset remote\nNAME                       IMAGES     PROGRESS\nexample-team/mydataset     112025        73.0%\n```\n\n### Create/remove a dataset\n\nTo create an empty dataset remotely:\n\n```\n$ darwin dataset create test\nDataset \'test\' (example-team/test) has been created.\nAccess at https://darwin.v7labs.com/datasets/579\n```\n\nThe dataset will be created in the team you\'re authenticated for.\n\nTo delete the project on the server:\n\n```\n$ darwin dataset remove test\nAbout to delete example-team/test on darwin.\nDo you want to continue? [y/N] y\n```\n\n### Upload/download data to/from a remote dataset\n\nUploads data to an existing remote project.\nIt takes the dataset name and a single image (or directory) with images/videos to upload as\nparameters.\n\nThe `-e/--exclude` argument allows to indicate file extension/s to be ignored from the data_dir.\ne.g.: `-e .jpg`\n\nFor videos, the frame rate extraction rate can be specified by adding `--fps <frame_rate>`\n\nSupported extensions:\n\n- Video files: [`.mp4`, `.bpm`, `.mov` formats].\n- Image files [`.jpg`, `.jpeg`, `.png` formats].\n\n```\n$ darwin dataset push test /path/to/folder/with/images\n100%|████████████████████████| 2/2 [00:01<00:00,  1.27it/s]\n```\n\nBefore a dataset can be downloaded, a release needs to be generated:\n\n```\n$ darwin dataset export test 0.1\nDataset test successfully exported to example-team/test:0.1\n```\n\nThis version is immutable, if new images / annotations have been added you will have to create a new release to included them.\n\nTo list all available releases\n\n```\n$ darwin dataset releases test\nNAME                           IMAGES     CLASSES                   EXPORT_DATE\nexample-team/test:0.1               4           0     2019-12-07 11:37:35+00:00\n```\n\nAnd to finally download a release.\n\n```\n$ darwin dataset pull test:0.1\nDataset example-team/test:0.1 downloaded at /directory/choosen/at/authentication/time.\n```\n\n---\n\n## Usage as a Python library\n\nThe framework is designed to be usable as a standalone python library.\nUsage can be inferred from looking at the operations performed in `darwin/cli_functions.py`.\nA minimal example to download a dataset is provided below and a more extensive one can be found in\n[darwin_demo.py](./darwin_demo.py).\n\n```python\nfrom darwin.client import Client\n\nclient = Client.local() # use the configuration in ~/.darwin/config.yaml\ndataset = client.get_remote_dataset("example-team/test")\ndataset.pull() # downloads annotations and images for the latest exported version\n```\n\nFollow [this guide](https://docs.v7labs.com/docs/loading-a-dataset-in-python) for how to integrate darwin datasets directly in PyTorch.\n',
     'author': 'V7',
     'author_email': 'info@v7labs.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://docs.v7labs.com/reference/getting-started-2',
```

### Comparing `darwin_py-0.8.9/PKG-INFO` & `darwin_py-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darwin-py
-Version: 0.8.9
+Version: 0.9.0
 Summary: Library and command line interface for darwin.v7labs.com
 Home-page: https://docs.v7labs.com/reference/getting-started-2
 License: MIT
 Author: V7
 Author-email: info@v7labs.com
 Requires-Python: >=3.8.0,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

