# Comparing `tmp/superpowered-sdk-0.1.5.tar.gz` & `tmp/superpowered-sdk-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superpowered-sdk-0.1.5.tar", last modified: Tue May 23 06:02:00 2023, max compression
+gzip compressed data, was "superpowered-sdk-0.1.6.tar", last modified: Tue Jun  6 07:26:12 2023, max compression
```

## Comparing `superpowered-sdk-0.1.5.tar` & `superpowered-sdk-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:02:00.145100 superpowered-sdk-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-05-23 06:02:00.145100 superpowered-sdk-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-05-23 06:01:46.000000 superpowered-sdk-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 06:02:00.145100 superpowered-sdk-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-23 06:01:46.000000 superpowered-sdk-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:02:00.145100 superpowered-sdk-0.1.5/superpowered/
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-23 06:01:46.000000 superpowered-sdk-0.1.5/superpowered/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-23 06:01:46.000000 superpowered-sdk-0.1.5/superpowered/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-05-23 06:01:46.000000 superpowered-sdk-0.1.5/superpowered/superpowered.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:02:00.145100 superpowered-sdk-0.1.5/superpowered_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-05-23 06:01:59.000000 superpowered-sdk-0.1.5/superpowered_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-23 06:02:00.000000 superpowered-sdk-0.1.5/superpowered_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 06:01:59.000000 superpowered-sdk-0.1.5/superpowered_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 06:01:59.000000 superpowered-sdk-0.1.5/superpowered_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 06:01:59.000000 superpowered-sdk-0.1.5/superpowered_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:26:12.983679 superpowered-sdk-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-06-06 07:26:12.983679 superpowered-sdk-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-06-06 07:25:55.000000 superpowered-sdk-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 07:26:12.983679 superpowered-sdk-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-06 07:25:55.000000 superpowered-sdk-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:26:12.979679 superpowered-sdk-0.1.6/superpowered/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-06 07:25:55.000000 superpowered-sdk-0.1.6/superpowered/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-06 07:25:55.000000 superpowered-sdk-0.1.6/superpowered/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-06-06 07:25:55.000000 superpowered-sdk-0.1.6/superpowered/superpowered.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:26:12.983679 superpowered-sdk-0.1.6/superpowered_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-06-06 07:26:12.000000 superpowered-sdk-0.1.6/superpowered_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-06 07:26:12.000000 superpowered-sdk-0.1.6/superpowered_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 07:26:12.000000 superpowered-sdk-0.1.6/superpowered_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-06 07:26:12.000000 superpowered-sdk-0.1.6/superpowered_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-06 07:26:12.000000 superpowered-sdk-0.1.6/superpowered_sdk.egg-info/top_level.txt
```

### Comparing `superpowered-sdk-0.1.5/PKG-INFO` & `superpowered-sdk-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superpowered-sdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: Superpowered AI SDK
 Home-page: https://superpowered.ai
 Author: superpowered
 Author-email: justin@superpowered.ai
 License: Proprietary License
 Project-URL: Homepage, https://superpowered.ai
 Project-URL: Documentation, https://superpowered.ai/docs
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: superpowered-sdk Version: 0.1.5 Summary:
+Metadata-Version: 2.1 Name: superpowered-sdk Version: 0.1.6 Summary:
 Superpowered AI SDK Home-page: https://superpowered.ai Author: superpowered
 Author-email: justin@superpowered.ai License: Proprietary License Project-URL:
 Homepage, https://superpowered.ai Project-URL: Documentation, https://
 superpowered.ai/docs Project-URL: Contact, https://superpowered.ai/contact/
 Project-URL: End-User License Agreement, https://superpowered.ai/api-user-
 agreement/ Description: # This is the official Superpowered AI Python SDK ##
 Installation `pip install superpowered-sdk` _Note_: To create API keys, please
```

### Comparing `superpowered-sdk-0.1.5/README.md` & `superpowered-sdk-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `superpowered-sdk-0.1.5/setup.py` & `superpowered-sdk-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `superpowered-sdk-0.1.5/superpowered/__init__.py` & `superpowered-sdk-0.1.6/superpowered/__init__.py`

 * *Files identical despite different names*

### Comparing `superpowered-sdk-0.1.5/superpowered/exceptions.py` & `superpowered-sdk-0.1.6/superpowered/exceptions.py`

 * *Files identical despite different names*

### Comparing `superpowered-sdk-0.1.5/superpowered/superpowered.py` & `superpowered-sdk-0.1.6/superpowered/superpowered.py`

 * *Files 3% similar despite different names*

```diff
@@ -355,49 +355,53 @@
         message="The 'query' function has been renamed to 'query_knowledge_bases' for clarity.",
         category=RenameWarning,
         stacklevel=2
     )
     return query_knowledge_bases(knowledge_base_ids, query, top_k, summarize_results)
 
 
-def query_knowledge_bases(knowledge_base_ids: list, query: str, top_k: int = 5, summarize_results: bool = False) -> dict:
+def query_knowledge_bases(knowledge_base_ids: list, query: str, top_k: int = 5, summarize_results: bool = False, summary_system_message: str = None) -> dict:
     """
     POST /knowledge_bases/query
     """
     data = {
         'query': query,
         'knowledge_base_ids': knowledge_base_ids,
     }
     if top_k:
         data['top_k'] = top_k
     if summarize_results:
         data['summarize_results'] = summarize_results
+    if summary_system_message:
+        data['summary_system_message'] = summary_system_message
     args = {
         'method': 'POST',
         'url': f'{get_base_url()}/knowledge_bases/query',
         'json': data,
         'auth': auth(),
     }
     return make_api_call(args)
 
 
-def query_passages(query: str, passages: list, top_k: int = 5, max_chunk_length: int = 500, summarize_results: bool = False) -> dict:
+def query_passages(query: str, passages: list, top_k: int = 5, max_chunk_length: int = 500, summarize_results: bool = False, summary_system_message: str = None) -> dict:
     """
     POST /query_passages
     """
     data = {
         'query': query,
         'passages': passages,
     }
     if top_k:
         data['top_k'] = top_k
     if max_chunk_length:
         data['max_chunk_length'] = max_chunk_length
     if summarize_results:
         data['summarize_results'] = summarize_results
+    if summary_system_message:
+        data['summary_system_message'] = summary_system_message
     args = {
         'method': 'POST',
         'url': f'{get_base_url()}/query_passages',
         'json': data,
         'auth': auth(),
     }
     return make_api_call(args)
```

### Comparing `superpowered-sdk-0.1.5/superpowered_sdk.egg-info/PKG-INFO` & `superpowered-sdk-0.1.6/superpowered_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superpowered-sdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: Superpowered AI SDK
 Home-page: https://superpowered.ai
 Author: superpowered
 Author-email: justin@superpowered.ai
 License: Proprietary License
 Project-URL: Homepage, https://superpowered.ai
 Project-URL: Documentation, https://superpowered.ai/docs
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: superpowered-sdk Version: 0.1.5 Summary:
+Metadata-Version: 2.1 Name: superpowered-sdk Version: 0.1.6 Summary:
 Superpowered AI SDK Home-page: https://superpowered.ai Author: superpowered
 Author-email: justin@superpowered.ai License: Proprietary License Project-URL:
 Homepage, https://superpowered.ai Project-URL: Documentation, https://
 superpowered.ai/docs Project-URL: Contact, https://superpowered.ai/contact/
 Project-URL: End-User License Agreement, https://superpowered.ai/api-user-
 agreement/ Description: # This is the official Superpowered AI Python SDK ##
 Installation `pip install superpowered-sdk` _Note_: To create API keys, please
```

