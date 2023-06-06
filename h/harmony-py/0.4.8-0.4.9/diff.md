# Comparing `tmp/harmony-py-0.4.8.tar.gz` & `tmp/harmony-py-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harmony-py-0.4.8.tar", last modified: Thu Jun  1 14:56:47 2023, max compression
+gzip compressed data, was "harmony-py-0.4.9.tar", last modified: Tue Jun  6 17:06:23 2023, max compression
```

## Comparing `harmony-py-0.4.8.tar` & `harmony-py-0.4.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:56:47.493812 harmony-py-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-01 14:55:40.000000 harmony-py-0.4.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-06-01 14:55:40.000000 harmony-py-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-01 14:55:40.000000 harmony-py-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-06-01 14:56:47.493812 harmony-py-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-01 14:55:40.000000 harmony-py-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:56:47.493812 harmony-py-0.4.8/harmony/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-01 14:56:40.000000 harmony-py-0.4.8/harmony/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-06-01 14:55:40.000000 harmony-py-0.4.8/harmony/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-01 14:55:40.000000 harmony-py-0.4.8/harmony/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    51063 2023-06-01 14:55:40.000000 harmony-py-0.4.8/harmony/harmony.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-01 14:55:40.000000 harmony-py-0.4.8/harmony/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:56:47.493812 harmony-py-0.4.8/harmony_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-06-01 14:56:47.000000 harmony-py-0.4.8/harmony_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-01 14:56:47.000000 harmony-py-0.4.8/harmony_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:56:47.000000 harmony-py-0.4.8/harmony_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-01 14:56:47.000000 harmony-py-0.4.8/harmony_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-01 14:56:47.000000 harmony-py-0.4.8/harmony_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-01 14:56:47.493812 harmony-py-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-01 14:55:40.000000 harmony-py-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:56:47.493812 harmony-py-0.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-01 14:55:40.000000 harmony-py-0.4.8/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    48449 2023-06-01 14:55:40.000000 harmony-py-0.4.8/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-01 14:55:40.000000 harmony-py-0.4.8/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-06-01 14:55:40.000000 harmony-py-0.4.8/tests/test_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-01 14:55:40.000000 harmony-py-0.4.8/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:06:23.718888 harmony-py-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-06 17:05:22.000000 harmony-py-0.4.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-06-06 17:05:22.000000 harmony-py-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-06 17:05:22.000000 harmony-py-0.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-06-06 17:06:23.718888 harmony-py-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-06 17:05:22.000000 harmony-py-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:06:23.714888 harmony-py-0.4.9/harmony/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-06 17:06:16.000000 harmony-py-0.4.9/harmony/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-06-06 17:05:22.000000 harmony-py-0.4.9/harmony/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-06 17:05:22.000000 harmony-py-0.4.9/harmony/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51525 2023-06-06 17:05:22.000000 harmony-py-0.4.9/harmony/harmony.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-06 17:05:22.000000 harmony-py-0.4.9/harmony/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:06:23.718888 harmony-py-0.4.9/harmony_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-06-06 17:06:23.000000 harmony-py-0.4.9/harmony_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-06 17:06:23.000000 harmony-py-0.4.9/harmony_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 17:06:23.000000 harmony-py-0.4.9/harmony_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-06 17:06:23.000000 harmony-py-0.4.9/harmony_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 17:06:23.000000 harmony-py-0.4.9/harmony_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-06 17:06:23.718888 harmony-py-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-06 17:05:22.000000 harmony-py-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:06:23.718888 harmony-py-0.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-06 17:05:22.000000 harmony-py-0.4.9/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49438 2023-06-06 17:05:22.000000 harmony-py-0.4.9/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-06 17:05:22.000000 harmony-py-0.4.9/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-06-06 17:05:22.000000 harmony-py-0.4.9/tests/test_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-06 17:05:22.000000 harmony-py-0.4.9/tests/test_util.py
```

### Comparing `harmony-py-0.4.8/CONTRIBUTING.md` & `harmony-py-0.4.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.8/LICENSE` & `harmony-py-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.8/PKG-INFO` & `harmony-py-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harmony-py
-Version: 0.4.8
+Version: 0.4.9
 Summary: The NASA Harmony Python library
 Home-page: https://github.com/nasa/harmony-py
 Keywords: nasa,harmony,remote-sensing,science,geoscience
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `harmony-py-0.4.8/README.md` & `harmony-py-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.8/harmony/auth.py` & `harmony-py-0.4.9/harmony/auth.py`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.8/harmony/config.py` & `harmony-py-0.4.9/harmony/config.py`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.8/harmony/harmony.py` & `harmony-py-0.4.9/harmony/harmony.py`

 * *Files 1% similar despite different names*

```diff
@@ -407,14 +407,19 @@
 
         >>> client = Client(token='myEDLTokenValue')
 
     By default, the Client will validate the provided credentials immediately. This can be
     disabled by passing ``should_validate_auth=False``.
     """
 
+    zarr_download_exception_msg = 'The zarr library must be used for zarr files. '\
+        'See https://github.com/nasa/harmony/blob/main/docs/Harmony%20Feature%20Examples.ipynb '\
+        'for zarr library usage example.'
+    zarr_download_exception = Exception(zarr_download_exception_msg)
+
     def __init__(
         self,
         *,
         auth: Optional[Tuple[str, str]] = None,
         should_validate_auth: bool = True,
         env: Environment = Environment.PROD,
         token: str = None,
@@ -1037,14 +1042,16 @@
             overwrite: If True, will overwrite a local file that shares a filename with the
             downloaded file. Defaults to False. If you're seeing malformed data or truncated
             files from incomplete downloads, set overwrite to True.
 
         Returns:
             A Future that resolves to the full path to the file.
         """
+        if url.endswith('zarr'):
+            raise self.zarr_download_exception
         future = self.executor.submit(self._download_file, url, directory, overwrite)
         return future
 
     def download_all(self,
                      job_id: str,
                      directory: str = '',
                      overwrite: bool = False) -> Generator[Future, None, None]:
@@ -1074,14 +1081,16 @@
             files from incomplete downloads, set overwrite to True.
 
         Returns:
             A list of Futures, each of which will return the filename (with path) for each
             result.
         """
         for url in self.result_urls(job_id, show_progress=False) or []:
+            if url.endswith('zarr'):
+                raise self.zarr_download_exception
             yield self.executor.submit(self._download_file, url, directory, overwrite)
 
     def iterator(
         self,
         job_id: str,
         directory: str = '',
         overwrite: bool = False
```

### Comparing `harmony-py-0.4.8/harmony/util.py` & `harmony-py-0.4.9/harmony/util.py`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.8/harmony_py.egg-info/PKG-INFO` & `harmony-py-0.4.9/harmony_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harmony-py
-Version: 0.4.8
+Version: 0.4.9
 Summary: The NASA Harmony Python library
 Home-page: https://github.com/nasa/harmony-py
 Keywords: nasa,harmony,remote-sensing,science,geoscience
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `harmony-py-0.4.8/setup.py` & `harmony-py-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.8/tests/test_auth.py` & `harmony-py-0.4.9/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.8/tests/test_client.py` & `harmony-py-0.4.9/tests/test_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -905,14 +905,42 @@
     )
 
     client = Client(should_validate_auth=False)
     actual_file_names = [f.result() for f in client.download_all('abcd-1234')]
 
     assert actual_file_names == expected_file_names
 
+def test_download_all_zarr(mocker):
+    expected_urls = [
+        'http://www.example.com/1',
+        'http://www.example.com/2.zarr',
+        'http://www.example.com/3',
+    ]
+
+    result_urls_mock = mocker.Mock(return_value=expected_urls)
+    mocker.patch('harmony.harmony.Client.result_urls', result_urls_mock)
+    mocker.patch(
+        'harmony.harmony.Client._download_file',
+        lambda self, url, a, b: url.split('/')[-1]
+    )
+
+    client = Client(should_validate_auth=False)
+
+    with pytest.raises(Exception) as exc_info:
+        client.download_all('abcd-1234')
+        [f.result() for f in client.download_all('abcd-1234')]
+    assert 'The zarr library must be used for zarr files.' in str(exc_info.value)
+
+def test_download_zarr():
+    client = Client(should_validate_auth=False)
+
+    with pytest.raises(Exception) as exc_info:
+        client.download('https://www.example.com/file1.zarr')
+    assert 'The zarr library must be used for zarr files.' in str(exc_info.value)
+
 def side_effect_func_for_download_file(url: str, directory: str = '', overwrite: bool = False) -> str:
     filename = url.split('/')[-1]
     return os.path.join(directory, filename)
 
 # list of links to provide on subsequent calls to _get_json
 def extra_links_for_iteration(link_type: str):
     return [
```

### Comparing `harmony-py-0.4.8/tests/test_config.py` & `harmony-py-0.4.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.8/tests/test_request.py` & `harmony-py-0.4.9/tests/test_request.py`

 * *Files identical despite different names*

