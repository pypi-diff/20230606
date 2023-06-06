# Comparing `tmp/metal_sdk-1.0.5.tar.gz` & `tmp/metal_sdk-1.0.6.tar.gz`

## Comparing `metal_sdk-1.0.5.tar` & `metal_sdk-1.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/.github/workflows/lint.yml
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/.github/workflows/publish.yml
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/.github/workflows/test.yml
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/examples/example.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/examples/example_async.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/src/metal_sdk/__init__.py
--rw-r--r--   0        0        0     4708 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/src/metal_sdk/metal.py
--rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/src/metal_sdk/metal_async.py
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/src/metal_sdk/motorhead.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/src/metal_sdk/motorhead_async.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/src/metal_sdk/typings.py
--rw-r--r--   0        0        0     7217 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/tests/test_metal.py
--rw-r--r--   0        0        0     7214 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/tests/test_metal_async.py
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/tests/test_motorhead.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/tests/test_motorhead_async.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/.gitignore
--rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/LICENSE
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/README.md
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 metal_sdk-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 metal_sdk-1.0.6/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 metal_sdk-1.0.6/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 metal_sdk-1.0.6/.github/workflows/test.yml
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 metal_sdk-1.0.6/examples/example.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 metal_sdk-1.0.6/examples/example_async.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metal_sdk-1.0.6/src/metal_sdk/__init__.py
+-rw-r--r--   0        0        0     6637 2020-02-02 00:00:00.000000 metal_sdk-1.0.6/src/metal_sdk/metal.py
+-rw-r--r--   0        0        0     6765 2020-02-02 00:00:00.000000 metal_sdk-1.0.6/src/metal_sdk/metal_async.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 metal_sdk-1.0.6/src/metal_sdk/motorhead.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 metal_sdk-1.0.6/src/metal_sdk/motorhead_async.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 metal_sdk-1.0.6/src/metal_sdk/typings.py
+-rw-r--r--   0        0        0     8467 2020-02-02 00:00:00.000000 metal_sdk-1.0.6/tests/test_metal.py
+-rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 metal_sdk-1.0.6/tests/test_metal_async.py
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 metal_sdk-1.0.6/tests/test_motorhead.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 metal_sdk-1.0.6/tests/test_motorhead_async.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 metal_sdk-1.0.6/.gitignore
+-rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 metal_sdk-1.0.6/LICENSE
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 metal_sdk-1.0.6/README.md
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 metal_sdk-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 metal_sdk-1.0.6/PKG-INFO
```

### Comparing `metal_sdk-1.0.5/.github/workflows/publish.yml` & `metal_sdk-1.0.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.5/.github/workflows/test.yml` & `metal_sdk-1.0.6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.5/examples/example.py` & `metal_sdk-1.0.6/examples/example.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.5/examples/example_async.py` & `metal_sdk-1.0.6/examples/example_async.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.5/src/metal_sdk/motorhead.py` & `metal_sdk-1.0.6/src/metal_sdk/motorhead.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.5/src/metal_sdk/motorhead_async.py` & `metal_sdk-1.0.6/src/metal_sdk/motorhead_async.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.5/src/metal_sdk/typings.py` & `metal_sdk-1.0.6/src/metal_sdk/typings.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.5/tests/test_metal.py` & `metal_sdk-1.0.6/tests/test_metal.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from unittest import TestCase, mock
 from src.metal_sdk.metal import Metal
 
 
 API_KEY = "api-key"
 CLIENT_ID = "client-id"
 
@@ -175,7 +176,35 @@
 
         metal.delete_many([id])
 
         self.assertEqual(metal.request.call_count, 1)
         self.assertEqual(metal.request.call_args[0][0], "delete")
         self.assertEqual(metal.request.call_args[0][1], "/v1/documents/bulk")
         self.assertEqual(metal.request.call_args[1]["json"]["ids"], [id])
+
+    def test_upload_file(self):
+        my_index = "my-index"
+        mock_file_path = "/path/to/mockfile.csv"
+
+        metal = Metal(API_KEY, CLIENT_ID, my_index)
+
+        metal._Metal__create_resource = mock.MagicMock(return_value={'data': {'url': 'https://mockuploadurl.com'}})
+        metal._Metal__upload_file_to_url = mock.MagicMock()
+        os.path.getsize = mock.MagicMock(return_value=1000)
+        os.path.basename = mock.MagicMock(return_value="mockfile.csv")
+
+        metal.upload_file(my_index, mock_file_path)
+
+        self.assertEqual(metal._Metal__create_resource.call_count, 1)
+        self.assertEqual(metal._Metal__upload_file_to_url.call_count, 1)
+
+        create_args = metal._Metal__create_resource.call_args[0]
+        self.assertEqual(create_args[0], my_index)
+        self.assertEqual(create_args[1], "mockfile.csv")
+        self.assertEqual(create_args[2], "text/csv")
+        self.assertEqual(create_args[3], 1000)
+
+        upload_args = metal._Metal__upload_file_to_url.call_args[0]
+        self.assertEqual(upload_args[0], 'https://mockuploadurl.com')
+        self.assertEqual(upload_args[1], mock_file_path)
+        self.assertEqual(upload_args[2], "text/csv")
+        self.assertEqual(upload_args[3], 1000)
```

### Comparing `metal_sdk-1.0.5/tests/test_metal_async.py` & `metal_sdk-1.0.6/tests/test_metal_async.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from unittest import TestCase, mock
 from src.metal_sdk.metal_async import Metal
 
 
 API_KEY = "api-key"
 CLIENT_ID = "client-id"
 
@@ -174,7 +175,35 @@
 
         await metal.delete_many([id])
 
         self.assertEqual(metal.request.call_count, 1)
         self.assertEqual(metal.request.call_args[0][0], "delete")
         self.assertEqual(metal.request.call_args[0][1], "/v1/documents/bulk")
         self.assertEqual(metal.request.call_args[1]["json"]["ids"], [id])
+
+    async def test_upload_file(self):
+        my_index = "my-index"
+        mock_file_path = "/path/to/mockfile.csv"
+
+        metal = Metal(API_KEY, CLIENT_ID, my_index)
+
+        metal._Metal__create_resource = mock.MagicMock(return_value={'data': {'url': 'https://mockuploadurl.com'}})
+        metal._Metal__upload_file_to_url = mock.MagicMock()
+        os.path.getsize = mock.MagicMock(return_value=1000)
+        os.path.basename = mock.MagicMock(return_value="mockfile.csv")
+
+        await metal.upload_file(my_index, mock_file_path)
+
+        self.assertEqual(metal._Metal__create_resource.call_count, 1)
+        self.assertEqual(metal._Metal__upload_file_to_url.call_count, 1)
+
+        create_args = metal._Metal__create_resource.call_args[0]
+        self.assertEqual(create_args[0], my_index)
+        self.assertEqual(create_args[1], "mockfile.csv")
+        self.assertEqual(create_args[2], "text/csv")
+        self.assertEqual(create_args[3], 1000)
+
+        upload_args = metal._Metal__upload_file_to_url.call_args[0]
+        self.assertEqual(upload_args[0], 'https://mockuploadurl.com')
+        self.assertEqual(upload_args[1], mock_file_path)
+        self.assertEqual(upload_args[2], "text/csv")
+        self.assertEqual(upload_args[3], 1000)
```

### Comparing `metal_sdk-1.0.5/tests/test_motorhead.py` & `metal_sdk-1.0.6/tests/test_motorhead.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.5/tests/test_motorhead_async.py` & `metal_sdk-1.0.6/tests/test_motorhead_async.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.5/.gitignore` & `metal_sdk-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.5/LICENSE` & `metal_sdk-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.5/README.md` & `metal_sdk-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.5/pyproject.toml` & `metal_sdk-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "metal_sdk"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="Metal Technologies Inc", email="james@getmetal.io" },
 ]
 description = "SDK for getmetal.io"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `metal_sdk-1.0.5/PKG-INFO` & `metal_sdk-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metal_sdk
-Version: 1.0.5
+Version: 1.0.6
 Summary: SDK for getmetal.io
 Project-URL: Github, https://github.com/getmetal/metal-python
 Author-email: Metal Technologies Inc <james@getmetal.io>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

