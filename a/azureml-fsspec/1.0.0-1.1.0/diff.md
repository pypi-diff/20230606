# Comparing `tmp/azureml_fsspec-1.0.0-py3-none-any.whl.zip` & `tmp/azureml_fsspec-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 11132 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat      251 b- defN 23-Apr-07 22:55 azureml/__init__.py
--rw-rw-rw-  2.0 fat      381 b- defN 23-Apr-07 22:56 azureml/fsspec/__init__.py
--rw-rw-rw-  2.0 fat    35396 b- defN 23-Apr-07 22:56 azureml/fsspec/spec.py
--rw-rw-rw-  2.0 fat     1021 b- defN 23-Apr-07 23:07 azureml_fsspec-1.0.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     2791 b- defN 23-Apr-07 23:07 azureml_fsspec-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Apr-07 23:07 azureml_fsspec-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       72 b- defN 23-Apr-07 23:07 azureml_fsspec-1.0.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-07 23:07 azureml_fsspec-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      763 b- defN 23-Apr-07 23:07 azureml_fsspec-1.0.0.dist-info/RECORD
-9 files, 40780 bytes uncompressed, 9802 bytes compressed:  76.0%
+Zip file size: 10974 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat      251 b- defN 23-Jun-06 00:11 azureml/__init__.py
+-rw-rw-rw-  2.0 fat      381 b- defN 23-Jun-06 00:12 azureml/fsspec/__init__.py
+-rw-rw-rw-  2.0 fat    36891 b- defN 23-Jun-06 00:12 azureml/fsspec/spec.py
+-rw-rw-rw-  2.0 fat     1021 b- defN 23-Jun-06 00:25 azureml_fsspec-1.1.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     2847 b- defN 23-Jun-06 00:25 azureml_fsspec-1.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-06 00:25 azureml_fsspec-1.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       72 b- defN 23-Jun-06 00:25 azureml_fsspec-1.1.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-06 00:25 azureml_fsspec-1.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      763 b- defN 23-Jun-06 00:25 azureml_fsspec-1.1.0.dist-info/RECORD
+9 files, 42331 bytes uncompressed, 9644 bytes compressed:  77.2%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: azureml/fsspec/__init__.py
 Comment: 
 
 Filename: azureml/fsspec/spec.py
 Comment: 
 
-Filename: azureml_fsspec-1.0.0.dist-info/LICENSE.txt
+Filename: azureml_fsspec-1.1.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: azureml_fsspec-1.0.0.dist-info/METADATA
+Filename: azureml_fsspec-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: azureml_fsspec-1.0.0.dist-info/WHEEL
+Filename: azureml_fsspec-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: azureml_fsspec-1.0.0.dist-info/entry_points.txt
+Filename: azureml_fsspec-1.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: azureml_fsspec-1.0.0.dist-info/top_level.txt
+Filename: azureml_fsspec-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: azureml_fsspec-1.0.0.dist-info/RECORD
+Filename: azureml_fsspec-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## azureml/fsspec/spec.py

```diff
@@ -3,59 +3,58 @@
 # ---------------------------------------------------------
 """
 Contains fsspec api implementation for aml uri
 """
 from fsspec.asyn import (
     AsyncFileSystem,
     get_loop,
-    sync,
-    _run_coros_in_chunks
+    sync
 )
 from fsspec.callbacks import _DEFAULT_CALLBACK
-from fsspec.implementations.local import LocalFileSystem, make_path_posix
-# from fsspec.utils import other_paths
+from fsspec.implementations.local import make_path_posix
 
-import asyncio
 import os
 import pathlib
 import re
 import inspect
 from glob import has_magic
 import azureml.dataprep as _dprep
 from azureml.dataprep.api._loggerfactory import track, _LoggerFactory
 from azureml.dataprep.api._constants import ACTIVITY_INFO_KEY, ERROR_CODE_KEY, \
     COMPLIANT_MESSAGE_KEY, OUTER_ERROR_CODE_KEY
 from azureml.dataprep.api.functions import get_stream_properties
 from azureml.dataprep.rslex import StreamInfo, CachingOptions, BufferingOptions, Downloader, \
     Copier, PyIfDestinationExists, PyLocationInfo, PyDatastoreSource
 from azureml.dataprep.api._rslex_executor import ensure_rslex_environment
+from azureml.dataprep import UserErrorException
+
 
 _PUBLIC_API = 'PublicApi'
 _APP_NAME = 'azureml-fsspec'
 _logger = None
 _DATASTORE_HANDLER = 'AmlDatastore'
 
 # TODO change to new error code from rslex and throw customized user error
 _USER_ERROR_MESSAGES = [
-    "StreamError(NotFound)", "DataAccessError(NotFound)", "DataAccessError(PermissionDenied)", "OutputError(NotEmpty)"]
+    "StreamError(NotFound)", "DataAccessError(NotFound)", "DataAccessError(PermissionDenied)", "OutputError(NotEmpty)",
+    "DestinationError(NotEmpty)"]
 
 _STRING_TO_PYIFDESTINATIONEXISTS = {
     # if find conflict file in destination, wil leave the original file
     "APPEND": PyIfDestinationExists.APPEND,
     # if find conflict file in destination, will raise not empty error
     "FAIL_ON_FILE_CONFLICT": PyIfDestinationExists.FAIL_ON_FILE_CONFLICT,
     # if find conflict file in destination, will overwrite with new file"
     "MERGE_WITH_OVERWRITE": PyIfDestinationExists.MERGE_WITH_OVERWRITE,
 }
 
 
 def _to_py_if_destination_exists(overwrite):
     if not isinstance(overwrite, str):
-        raise ValueError(
-            'The overwrite kwargs should be a string')
+        raise ValueError('The overwrite kwargs should be a string')
 
     try:
         return _STRING_TO_PYIFDESTINATIONEXISTS[overwrite.upper()]
     except KeyError:
         raise ValueError(f"Given invalid overwrite kwargs {str(overwrite)}, supported "
                          "value are: 'APPEND', 'FAIL_ON_FILE_CONFLICT', "
                          "'MERGE_WITH_OVERWRITE'.")
@@ -268,15 +267,15 @@
         :type path: str
         :return: A list of file paths
         :rtype: list[str]
         """
         custom_dimensions = {'app_name': _APP_NAME}
         custom_dimensions.update(self._workspace_context)
 
-        with _LoggerFactory.track_activity(_get_logger(), 'glob', _PUBLIC_API,
+        with _LoggerFactory.track_activity(_get_logger(), '_glob', _PUBLIC_API,
                                            custom_dimensions) as activityLogger:
             try:
                 if not path:
                     path = self._path
                 path = self._strip_protocol(
                     path, self._workspace_context).rstrip("/")
                 path = self._get_full_path_from_fs_root(path)
@@ -319,15 +318,15 @@
         :type refresh: bool
         :return: A list of file paths if detail is False, else returns a list of dict
         :rtype: list[str] or list[dict]
         """
         custom_dimensions = {'app_name': _APP_NAME}
         custom_dimensions.update(self._workspace_context)
 
-        with _LoggerFactory.track_activity(_get_logger(), 'ls', _PUBLIC_API,
+        with _LoggerFactory.track_activity(_get_logger(), '_ls', _PUBLIC_API,
                                            custom_dimensions) as activityLogger:
             try:
                 ensure_rslex_environment()
                 if not path:
                     path = self._path
                 path = self._strip_protocol(
                     path, self._workspace_context).rstrip("/")
@@ -406,15 +405,15 @@
         if _FS_DOWNLOAD_MEMORY_CACHE_SIZE in os.environ:
             memory_cache_size = os.environ[_FS_DOWNLOAD_MEMORY_CACHE_SIZE]
 
         _FS_DOWNLOAD_READ_THREADS = '_FS_DOWNLOAD_READ_THREADS'
         if _FS_DOWNLOAD_READ_THREADS in os.environ:
             read_threads = os.environ[_FS_DOWNLOAD_READ_THREADS]
 
-        with _LoggerFactory.track_activity(_get_logger(), 'open', _PUBLIC_API,
+        with _LoggerFactory.track_activity(_get_logger(), '_open', _PUBLIC_API,
                                            custom_dimensions) as activityLogger:
             try:
                 ensure_rslex_environment()
 
                 if not path:
                     path = self._path
                 path = self._strip_protocol(path, self._workspace_context)
@@ -482,15 +481,14 @@
         return list(sorted(out))
 
     @track(_get_logger, custom_dimensions={'app_name': _APP_NAME})
     def get(self, rpath, lpath, recursive=False, callback=_DEFAULT_CALLBACK, **kwargs):
         """Copy file(s) to local."""
         return sync(self.loop, self._get, rpath, lpath, recursive, callback, **kwargs)
 
-    @track(_get_logger, custom_dimensions={'app_name': _APP_NAME})
     async def _get(
             self, rpath, lpath, recursive=False, callback=_DEFAULT_CALLBACK, **kwargs
     ):
         """Copy file(s) to local.
 
         Copies a specific file or tree of files (if recursive=True). If lpath
         ends with a "/", it will be assumed to be a directory, and target files
@@ -500,46 +498,59 @@
         The get_file method will be called concurrently on a batch of files. The
         batch_size option can configure the amount of futures that can be executed
         at the same time. If it is -1, then all the files will be uploaded concurrently.
         The default can be set for this instance by passing "batch_size" in the
         constructor, or for all instances by setting the "gather_batch_size" key
         in ``fsspec.config.conf``, falling back to 1/8th of the system limit .
         """
-        rpath = self._strip_protocol(rpath, self._workspace_context)
-        lpath = make_path_posix(lpath)
-        if (await self._info(rpath))["type"] == "file" and recursive is True:
-            raise ValueError("rpath type of single file should not use recursive download")
-        rpaths = await self._expand_path(rpath, recursive=recursive)
-        batch_size = kwargs.pop("batch_size", self.batch_size)
-        rpath = self._get_full_path_from_fs_root(rpath)
-
-        coros = []
-        callback.set_size(len(rpaths))
-
-        # needs to get parent folder if its download single file as base dir
-        base_dir = rpath if len(
-            rpaths) > 1 or recursive else self._parent(rpath)
-        kwargs.update({'base_dir': base_dir})
-        for remote_path in rpaths:
-            remote_path = self._get_full_path_from_fs_root(remote_path)
-            callback.branch(remote_path, lpath, kwargs)
-            coros.append(self._get_file(remote_path, lpath, **kwargs))
-        await _run_coros_in_chunks(coros, batch_size=batch_size, callback=callback)
+        custom_dimensions = {'app_name': _APP_NAME}
+        custom_dimensions.update(self._workspace_context)
+
+        with _LoggerFactory.track_activity(_get_logger(), '_get', _PUBLIC_API,
+                                           custom_dimensions) as activityLogger:
+            try:
+                rpath = self._strip_protocol(rpath, self._workspace_context)
+                lpath = make_path_posix(lpath)
+                if (await self._info(rpath))["type"] == "file" and recursive is True:
+                    raise ValueError("rpath type of single file should not use recursive download")
+                rpaths = await self._expand_path(rpath, recursive=recursive)
+                rpath = self._get_full_path_from_fs_root(rpath)
+
+                ensure_rslex_environment()
+                # needs to get parent folder if its download single file as base dir
+                base_dir = rpath if len(
+                    rpaths) > 1 or recursive else self._parent(rpath)
+                overwrite = kwargs.get('overwrite', "FAIL_ON_FILE_CONFLICT")
+                if_destination_exists = _to_py_if_destination_exists(overwrite)
+                kwargs.update({'base_dir': base_dir})
+                copier = Copier(PyLocationInfo('Local', lpath, {}),
+                                base_dir, if_destination_exists)
+                copier.copy_volume(PyLocationInfo('AmlDatastore', rpath, self._datastore_source), '')
+            except Exception as e:
+                if hasattr(activityLogger, ACTIVITY_INFO_KEY):
+                    activityLogger.activity_info['error_code'] = getattr(
+                        e, ERROR_CODE_KEY, '')
+                    activityLogger.activity_info['message'] = getattr(
+                        e, COMPLIANT_MESSAGE_KEY, str(e))
+                    activityLogger.activity_info['outer_error_code'] = getattr(
+                        e, OUTER_ERROR_CODE_KEY, '')
+
+                AzureMachineLearningFileSystem._map_user_error(e)
 
     async def _get_file(self, rpath, lpath, overwrite="FAIL_ON_FILE_CONFLICT", callback=_DEFAULT_CALLBACK, **kwargs):
         """
         Copy single file remote to local
         :param lpath: Path to local file
         :param rpath: Path to remote file, rpath is in the format of {datastore_name}/{relative_path}
         :param overwrite: string. Suppurts values "APPEND", "FAIL_ON_FILE_CONFLICT", "MERGE_WITH_OVERWRITE".
         """
         custom_dimensions = {'app_name': _APP_NAME}
         custom_dimensions.update(self._workspace_context)
 
-        with _LoggerFactory.track_activity(_get_logger(), 'get_file', _PUBLIC_API,
+        with _LoggerFactory.track_activity(_get_logger(), '_get_file', _PUBLIC_API,
                                            custom_dimensions) as activityLogger:
             overwrite = _to_py_if_destination_exists(overwrite)
 
             try:
                 ensure_rslex_environment()
                 base_dir = kwargs.get('base_dir', None)
 
@@ -560,15 +571,14 @@
                 AzureMachineLearningFileSystem._map_user_error(e)
 
     @track(_get_logger, custom_dimensions={'app_name': _APP_NAME})
     def put(self, lpath, rpath, recursive=False, callback=_DEFAULT_CALLBACK, **kwargs):
         """Copy file(s) to local."""
         return sync(self.loop, self._put, lpath, rpath, recursive, callback, **kwargs)
 
-    @track(_get_logger, custom_dimensions={'app_name': _APP_NAME})
     async def _put(
             self,
             lpath,
             rpath,
             recursive=False,
             callback=_DEFAULT_CALLBACK,
             batch_size=None,
@@ -583,55 +593,65 @@
         The put_file method will be called concurrently on a batch of files. The
         batch_size option can configure the amount of futures that can be executed
         at the same time. If it is -1, then all the files will be uploaded concurrently.
         The default can be set for this instance by passing "batch_size" in the
         constructor, or for all instances by setting the "gather_batch_size" key
         in ``fsspec.config.conf``, falling back to 1/8th of the system limit .
         """
-        if not rpath:
-            rpath = self._path
-        # append ending / to indicate its a directory
-        rpath = self._strip_protocol(rpath, self._workspace_context)
-        rpath = self._get_full_path_from_fs_root(rpath)
-        rpath = rpath.rstrip('/') + '/'
-        if isinstance(lpath, str):
-            lpath = make_path_posix(lpath)
-        fs = LocalFileSystem()
-        lpaths = fs.expand_path(lpath, recursive=recursive)
-        rpaths = self._other_paths(lpaths, rpath)
-        is_dir = {l_path: os.path.isdir(l_path) for l_path in lpaths}
-        rdirs = [r_path for l_path, r_path in zip(lpaths, rpaths) if is_dir[l_path]]
-        file_pairs = [(l_path, r_path) for l_path, r_path in zip(lpaths, rpaths) if not is_dir[l_path]]
-
-        await asyncio.gather(*[self._makedirs(d, exist_ok=True) for d in rdirs])
-        batch_size = batch_size or self.batch_size
-
-        coros = []
-        callback.set_size(len(file_pairs))
-        for lfile, rfile in file_pairs:
-            callback.branch(lfile, rfile, kwargs)
-            coros.append(self._put_file(lfile, rfile, **kwargs))
+        custom_dimensions = {'app_name': _APP_NAME}
+        custom_dimensions.update(self._workspace_context)
+        overwrite = kwargs.get('overwrite', "FAIL_ON_FILE_CONFLICT")
+        if_destination_exists = _to_py_if_destination_exists(overwrite)
 
-        await _run_coros_in_chunks(
-            coros, batch_size=batch_size, callback=callback
-        )
+        with _LoggerFactory.track_activity(_get_logger(), '_put', _PUBLIC_API,
+                                           custom_dimensions) as activityLogger:
+            try:
+                if not rpath:
+                    rpath = self._path
+                    # append ending / to indicate its a directory
+                rpath = self._strip_protocol(rpath, self._workspace_context)
+                rpath = self._get_full_path_from_fs_root(rpath)
+                rpath = rpath.rstrip('/') + '/'
+                if isinstance(lpath, str):
+                    lpath = make_path_posix(lpath)
+
+                ensure_rslex_environment()
+                lpath = os.path.abspath(lpath)
+                lpath = lpath.replace('\\', '/')
+                base_path = lpath
+                if not os.path.isdir(lpath):
+                    base_path = self._parent(lpath)
+
+                copier = Copier(PyLocationInfo('AmlDatastore', rpath, self._datastore_source),
+                                base_path, if_destination_exists)
+                copier.copy_volume(PyLocationInfo('Local', lpath, {}), '')
+            except Exception as e:
+                if hasattr(activityLogger, ACTIVITY_INFO_KEY):
+                    activityLogger.activity_info['error_code'] = getattr(
+                        e, ERROR_CODE_KEY, '')
+                    activityLogger.activity_info['message'] = getattr(
+                        e, COMPLIANT_MESSAGE_KEY, str(e))
+                    activityLogger.activity_info['outer_error_code'] = getattr(
+                        e, OUTER_ERROR_CODE_KEY, '')
+
+                AzureMachineLearningFileSystem._map_user_error(e)
 
     async def _put_file(
             self, lpath, rpath, overwrite="FAIL_ON_FILE_CONFLICT", callback=_DEFAULT_CALLBACK, **kwargs
     ):
         """
         Copy single file to remote
         :param lpath: Path to local file
         :param rpath: Path to remote file, rpath is in the format of {datastore_name}/{relative_path}
         :param overwrite: string. Suppurts values "APPEND", "FAIL_ON_FILE_CONFLICT", "MERGE_WITH_OVERWRITE".
         :param callback: callback function
         """
         custom_dimensions = {'app_name': _APP_NAME}
         custom_dimensions.update(self._workspace_context)
-        with _LoggerFactory.track_activity(_get_logger(), 'put_file', _PUBLIC_API,
+        with _LoggerFactory.track_activity(_get_logger(), '_put_file', _PUBLIC_API,
                                            custom_dimensions) as activityLogger:
             overwrite = _to_py_if_destination_exists(overwrite)
 
             try:
                 # rpath has the remote file name, copy_stream_info expects folder
                 rpath = self._parent(rpath)
                 ensure_rslex_environment()
@@ -659,16 +679,16 @@
 
                 AzureMachineLearningFileSystem._map_user_error(e)
 
     @track(_get_logger, custom_dimensions={'app_name': _APP_NAME})
     def _validate_args_for_open(self, mode):
         supported_modes = ['r', 'rb']
         if mode not in supported_modes:
-            raise ValueError(f'Invalid mode {mode}, supported modes are {supported_modes}, '
-                             'both means read as byte array')
+            raise UserErrorException(
+                f'Invalid mode {mode}, supported modes are {supported_modes}, both means read as byte array')
 
     def _parent(self, path):
         path = self._strip_protocol(path.rstrip("/"), self._workspace_context)
         if "/" in path:
             # path.rsplit("/", 1)[0].lstrip("/")
             return path.rsplit("/", 1)[0]
         # root path of datastore, eg: workspaceblobstore/
@@ -724,18 +744,18 @@
         datastore_uri_match = _datastore_uri_regex_pattern.match(path)
         if data_path_uri_match:
             return data_path_uri_match[1], data_path_uri_match[2], data_path_uri_match[3], data_path_uri_match[4],\
                 data_path_uri_match[5]
         elif datastore_uri_match:
             return datastore_uri_match[1], datastore_uri_match[2], datastore_uri_match[3], datastore_uri_match[4], '/'
         else:
-            raise ValueError(f'{path} is not a valid datastore uri: '
-                             f'azureml://subscriptions/([^\/]+)/resourcegroups/([^\/]+)/'
-                             f'(?:Microsoft.MachineLearningServices/)?workspaces/([^\/]+)/'
-                             f'datastores/([^\/]+)/paths/(.*)')
+            raise UserErrorException(f'{path} is not a valid datastore uri: '
+                                     f'azureml://subscriptions/([^\/]+)/resourcegroups/([^\/]+)/'
+                                     f'(?:Microsoft.MachineLearningServices/)?workspaces/([^\/]+)/'
+                                     f'datastores/([^\/]+)/paths/(.*)')
 
     @staticmethod
     def _get_kwargs_from_urls(path):
         """ Directly return the path """
         out = {}
         out["uri"] = path
         return out
```

## Comparing `azureml_fsspec-1.0.0.dist-info/LICENSE.txt` & `azureml_fsspec-1.1.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `azureml_fsspec-1.0.0.dist-info/METADATA` & `azureml_fsspec-1.1.0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azureml-fsspec
-Version: 1.0.0
+Version: 1.1.0
 Summary: Access datastore uri with fsspec
 Home-page: https://docs.microsoft.com/python/api/overview/azure/ml/?view=azure-ml-py
 Author: Microsoft Corp
 License: Proprietary https://aka.ms/azureml-preview-sdk-license 
 Keywords: file-system,dask,azure
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,16 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6,< 4.0
 Description-Content-Type: text/markdown
-Requires-Dist: azureml-core
-Requires-Dist: azureml-dataprep (<4.11.0a,>=4.10.0a)
+Requires-Dist: azureml-dataprep (<4.12.0a,>=4.11.1)
 Requires-Dist: fsspec (>=2021.6.1)
 
 # Filesystem interface to Azure Machine Learning defined URIs
 
 ## Getting started
 
 This package can be installed using:
@@ -59,14 +58,19 @@
 df = dd.read_csv('azureml://subscriptions/{sub_id}/resourcegroups/{rs_group}/workspaces/{ws}
                           /datastores/workspaceblobstore/paths/myfolder/mydata.csv')
 ```
 
 
 # Release History
 
+## 1.1.0 (06-01-2023)
+
+### Features Added
+- upload/download performance improvement
+
 ## 1.0.0 (04-07-2023)
 
 ### Features Added
 - Added upload/download API
 - bugfix(root behavior)
 
 ## 0.1.0b1
```

