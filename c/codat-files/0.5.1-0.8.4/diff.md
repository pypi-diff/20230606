# Comparing `tmp/codat-files-0.5.1.tar.gz` & `tmp/codat-files-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codat-files-0.5.1.tar", last modified: Fri Mar 17 05:38:16 2023, max compression
+gzip compressed data, was "codat-files-0.8.4.tar", last modified: Wed Apr  5 09:31:32 2023, max compression
```

## Comparing `codat-files-0.5.1.tar` & `codat-files-0.8.4.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:38:16.614722 codat-files-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-03-17 05:38:16.614722 codat-files-0.5.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)      954 2023-03-17 05:38:08.000000 codat-files-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 05:38:16.614722 codat-files-0.5.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1028 2023-03-17 05:38:08.000000 codat-files-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:38:16.610722 codat-files-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:38:16.610722 codat-files-0.5.1/src/codat/
--rwxr-xr-x   0 runner    (1001) docker     (123)       19 2023-03-17 05:38:08.000000 codat-files-0.5.1/src/codat/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3357 2023-03-17 05:38:08.000000 codat-files-0.5.1/src/codat/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:38:16.610722 codat-files-0.5.1/src/codat/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:38:08.000000 codat-files-0.5.1/src/codat/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:38:16.610722 codat-files-0.5.1/src/codat/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)      242 2023-03-17 05:38:08.000000 codat-files-0.5.1/src/codat/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      715 2023-03-17 05:38:08.000000 codat-files-0.5.1/src/codat/models/operations/download_files.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1712 2023-03-17 05:38:08.000000 codat-files-0.5.1/src/codat/models/operations/list_files.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      670 2023-03-17 05:38:08.000000 codat-files-0.5.1/src/codat/models/operations/upload_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:38:16.610722 codat-files-0.5.1/src/codat/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)       48 2023-03-17 05:38:08.000000 codat-files-0.5.1/src/codat/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-03-17 05:38:08.000000 codat-files-0.5.1/src/codat/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2136 2023-03-17 05:38:08.000000 codat-files-0.5.1/src/codat/sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:38:16.610722 codat-files-0.5.1/src/codat/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-03-17 05:38:08.000000 codat-files-0.5.1/src/codat/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3629 2023-03-17 05:38:08.000000 codat-files-0.5.1/src/codat/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24723 2023-03-17 05:38:08.000000 codat-files-0.5.1/src/codat/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:38:16.614722 codat-files-0.5.1/src/codat_files.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-03-17 05:38:16.000000 codat-files-0.5.1/src/codat_files.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-17 05:38:16.000000 codat-files-0.5.1/src/codat_files.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 05:38:16.000000 codat-files-0.5.1/src/codat_files.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-17 05:38:16.000000 codat-files-0.5.1/src/codat_files.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-17 05:38:16.000000 codat-files-0.5.1/src/codat_files.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:31:32.063833 codat-files-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-05 09:31:32.059833 codat-files-0.8.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)      990 2023-04-05 09:31:22.000000 codat-files-0.8.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 09:31:32.063833 codat-files-0.8.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1104 2023-04-05 09:31:22.000000 codat-files-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:31:32.055833 codat-files-0.8.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:31:32.055833 codat-files-0.8.4/src/codat/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-05 09:31:22.000000 codat-files-0.8.4/src/codat/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3802 2023-04-05 09:31:22.000000 codat-files-0.8.4/src/codat/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:31:32.059833 codat-files-0.8.4/src/codat/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-05 09:31:22.000000 codat-files-0.8.4/src/codat/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:31:32.059833 codat-files-0.8.4/src/codat/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      327 2023-04-05 09:31:22.000000 codat-files-0.8.4/src/codat/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      910 2023-04-05 09:31:22.000000 codat-files-0.8.4/src/codat/models/operations/download_files.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      761 2023-04-05 09:31:22.000000 codat-files-0.8.4/src/codat/models/operations/list_files.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1213 2023-04-05 09:31:22.000000 codat-files-0.8.4/src/codat/models/operations/upload_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:31:32.059833 codat-files-0.8.4/src/codat/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      151 2023-04-05 09:31:22.000000 codat-files-0.8.4/src/codat/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1965 2023-04-05 09:31:22.000000 codat-files-0.8.4/src/codat/models/shared/file.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-04-05 09:31:22.000000 codat-files-0.8.4/src/codat/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2521 2023-04-05 09:31:22.000000 codat-files-0.8.4/src/codat/sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:31:32.059833 codat-files-0.8.4/src/codat/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-05 09:31:22.000000 codat-files-0.8.4/src/codat/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-05 09:31:22.000000 codat-files-0.8.4/src/codat/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24799 2023-04-05 09:31:22.000000 codat-files-0.8.4/src/codat/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:31:32.059833 codat-files-0.8.4/src/codat_files.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-05 09:31:32.000000 codat-files-0.8.4/src/codat_files.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-05 09:31:32.000000 codat-files-0.8.4/src/codat_files.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 09:31:32.000000 codat-files-0.8.4/src/codat_files.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-05 09:31:32.000000 codat-files-0.8.4/src/codat_files.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-05 09:31:32.000000 codat-files-0.8.4/src/codat_files.egg-info/top_level.txt
```

### Comparing `codat-files-0.5.1/PKG-INFO` & `codat-files-0.8.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: codat-files
-Version: 0.5.1
-Summary: Python Client SDK Generated by Speakeasy
-Home-page: UNKNOWN
-Author: Speakeasy
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
 # codat-files
 
 <!-- Start SDK Installation -->
 ## SDK Installation
 
 ```bash
 pip install codat-files
@@ -29,32 +18,30 @@
     security=shared.Security(
         auth_header="YOUR_API_KEY_HERE",
     ),
 )
 
 
 req = operations.DownloadFilesRequest(
-    company_id="unde",
-    date_="2022-08-12T20:13:28.710Z",
+    company_id="8a210b68-6988-11ed-a1eb-0242ac120002",
+    date_="2022-10-23T00:00:00Z",
 )
     
 res = s.files.download_files(req)
 
-if res.status_code == 200:
+if res.data is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
-## SDK Available Operations
+## Available Resources and Operations
 
 
 ### files
 
 * `download_files` - Download all files for a company
 * `list_files` - List all files uploaded by a company
 * `upload_files` - Upload files for a company
 <!-- End SDK Available Operations -->
 
 ### SDK Generated by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
-
-
```

### Comparing `codat-files-0.5.1/README.md` & `codat-files-0.8.4/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: codat-files
+Version: 0.8.4
+Summary: Python Client SDK Generated by Speakeasy
+Home-page: UNKNOWN
+Author: Speakeasy
+License: UNKNOWN
+Platform: UNKNOWN
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+
 # codat-files
 
 <!-- Start SDK Installation -->
 ## SDK Installation
 
 ```bash
 pip install codat-files
@@ -18,30 +29,32 @@
     security=shared.Security(
         auth_header="YOUR_API_KEY_HERE",
     ),
 )
 
 
 req = operations.DownloadFilesRequest(
-    company_id="unde",
-    date_="2022-08-12T20:13:28.710Z",
+    company_id="8a210b68-6988-11ed-a1eb-0242ac120002",
+    date_="2022-10-23T00:00:00Z",
 )
     
 res = s.files.download_files(req)
 
-if res.status_code == 200:
+if res.data is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
-## SDK Available Operations
+## Available Resources and Operations
 
 
 ### files
 
 * `download_files` - Download all files for a company
 * `list_files` - List all files uploaded by a company
 * `upload_files` - Upload files for a company
 <!-- End SDK Available Operations -->
 
 ### SDK Generated by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
+
+
```

### Comparing `codat-files-0.5.1/setup.py` & `codat-files-0.8.4/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import setuptools
 
 try:
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="codat-files",
-    version="0.5.1",
+    version="0.8.4",
     author="Speakeasy",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi==2022.12.07",
```

### Comparing `codat-files-0.5.1/src/codat/files.py` & `codat-files-0.8.4/src/codat/files.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class Files:
+    r"""Endpoints to manage uploaded files."""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -19,73 +22,73 @@
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
     def download_files(self, request: operations.DownloadFilesRequest) -> operations.DownloadFilesResponse:
         r"""Download all files for a company
         You can specify a date to download specific files for.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.DownloadFilesRequest, base_url, '/companies/{companyId}/files/download', request)
         
         query_params = utils.get_query_params(operations.DownloadFilesRequest, request)
         
         client = self._security_client
         
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.DownloadFilesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
-            pass
+            if utils.match_content_type(content_type, 'application/octet-stream'):
+                res.data = http_res.content
 
         return res
 
     def list_files(self, request: operations.ListFilesRequest) -> operations.ListFilesResponse:
         r"""List all files uploaded by a company
         Returns an array of files that have been uploaded for a given company.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListFilesRequest, base_url, '/companies/{companyId}/files', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListFilesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[list[operations.ListFilesFile]])
+                out = utils.unmarshal_json(http_res.text, Optional[list[shared.File]])
                 res.files = out
 
         return res
 
     def upload_files(self, request: operations.UploadFilesRequest) -> operations.UploadFilesResponse:
         r"""Upload files for a company
         Upload files
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.UploadFilesRequest, base_url, '/companies/{companyId}/connections/{connectionId}/files', request)
         
+        headers = {}
+        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'multipart')
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        http_res = client.request('POST', url)
+        http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.UploadFilesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if http_res.status_code == 200:
-            pass
 
         return res
```

### Comparing `codat-files-0.5.1/src/codat/models/operations/download_files.py` & `codat-files-0.8.4/src/codat/models/operations/download_files.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,25 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from datetime import datetime
 from typing import Optional
 
 
 @dataclasses.dataclass
 class DownloadFilesRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    date_: Optional[datetime] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'date', 'style': 'form', 'explode': True }})
+    
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    date_: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'date', 'style': 'form', 'explode': True }})
+    r"""Only download files uploaded on this date"""  
     
 
 @dataclasses.dataclass
 class DownloadFilesResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    data: Optional[bytes] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-files-0.5.1/src/codat/models/operations/list_files.py` & `codat-files-0.8.4/src/codat/models/operations/upload_files.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,30 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
 import requests as requests_http
-from codat import utils
-from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
-from marshmallow import fields
 from typing import Optional
 
 
 @dataclasses.dataclass
-class ListFilesRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
+class UploadFilesRequestBody:
+    
+    content: bytes = dataclasses.field(metadata={'multipart_form': { 'content': True }})  
+    request_body: str = dataclasses.field(metadata={'multipart_form': { 'field_name': 'requestBody' }})  
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ListFilesFile:
-    display_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('displayName'), 'exclude': lambda f: f is None }})
-    file_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fileName'), 'exclude': lambda f: f is None }})
-    source_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType'), 'exclude': lambda f: f is None }})
-    uploaded: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('uploaded'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+class UploadFilesRequest:
+    
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})  
+    request_body: Optional[UploadFilesRequestBody] = dataclasses.field(default=None, metadata={'multipart_form': { 'file': True }, 'request': { 'media_type': 'multipart/form-data' }})  
     
 
 @dataclasses.dataclass
-class ListFilesResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    files: Optional[list[ListFilesFile]] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+class UploadFilesResponse:
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-files-0.5.1/src/codat/utils/retries.py` & `codat-files-0.8.4/src/codat/utils/retries.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import random
 import time
 
 import requests
 
 
 class BackoffStrategy:
```

### Comparing `codat-files-0.5.1/src/codat/utils/utils.py` & `codat-files-0.8.4/src/codat/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import base64
 import json
 import re
 from dataclasses import Field, dataclass, fields, is_dataclass, make_dataclass
 from datetime import date, datetime
 from email.message import Message
 from enum import Enum
```

### Comparing `codat-files-0.5.1/src/codat_files.egg-info/PKG-INFO` & `codat-files-0.8.4/src/codat_files.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codat-files
-Version: 0.5.1
+Version: 0.8.4
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -29,27 +29,27 @@
     security=shared.Security(
         auth_header="YOUR_API_KEY_HERE",
     ),
 )
 
 
 req = operations.DownloadFilesRequest(
-    company_id="unde",
-    date_="2022-08-12T20:13:28.710Z",
+    company_id="8a210b68-6988-11ed-a1eb-0242ac120002",
+    date_="2022-10-23T00:00:00Z",
 )
     
 res = s.files.download_files(req)
 
-if res.status_code == 200:
+if res.data is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
-## SDK Available Operations
+## Available Resources and Operations
 
 
 ### files
 
 * `download_files` - Download all files for a company
 * `list_files` - List all files uploaded by a company
 * `upload_files` - Upload files for a company
```

### Comparing `codat-files-0.5.1/src/codat_files.egg-info/SOURCES.txt` & `codat-files-0.8.4/src/codat_files.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 src/codat/sdk.py
 src/codat/models/__init__.py
 src/codat/models/operations/__init__.py
 src/codat/models/operations/download_files.py
 src/codat/models/operations/list_files.py
 src/codat/models/operations/upload_files.py
 src/codat/models/shared/__init__.py
+src/codat/models/shared/file.py
 src/codat/models/shared/security.py
 src/codat/utils/__init__.py
 src/codat/utils/retries.py
 src/codat/utils/utils.py
 src/codat_files.egg-info/PKG-INFO
 src/codat_files.egg-info/SOURCES.txt
 src/codat_files.egg-info/dependency_links.txt
```

