# Comparing `tmp/test_graphql_sdk-0.0.9.tar.gz` & `tmp/test_graphql_sdk-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_graphql_sdk-0.0.9.tar", last modified: Mon Jun  5 13:04:17 2023, max compression
+gzip compressed data, was "test_graphql_sdk-0.1.0.tar", last modified: Tue Jun  6 10:10:29 2023, max compression
```

## Comparing `test_graphql_sdk-0.0.9.tar` & `test_graphql_sdk-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-05 13:04:17.979684 test_graphql_sdk-0.0.9/
--rw-r--r--   0 sarvesh    (501) staff       (20)     3204 2023-06-05 13:04:17.979735 test_graphql_sdk-0.0.9/PKG-INFO
--rw-r--r--   0 sarvesh    (501) staff       (20)     2692 2023-06-05 12:41:34.000000 test_graphql_sdk-0.0.9/README.md
--rw-r--r--   0 sarvesh    (501) staff       (20)       85 2023-05-31 07:35:04.000000 test_graphql_sdk-0.0.9/pyproject.toml
--rw-r--r--   0 sarvesh    (501) staff       (20)      659 2023-06-05 13:04:17.979953 test_graphql_sdk-0.0.9/setup.cfg
-drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-05 13:04:17.977466 test_graphql_sdk-0.0.9/src/
-drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-05 13:04:17.978963 test_graphql_sdk-0.0.9/src/airstack/
--rw-r--r--   0 sarvesh    (501) staff       (20)        0 2023-06-05 12:53:03.000000 test_graphql_sdk-0.0.9/src/airstack/__init__.py
--rw-r--r--   0 sarvesh    (501) staff       (20)      210 2023-06-01 15:14:21.000000 test_graphql_sdk-0.0.9/src/airstack/constant.py
--rw-r--r--   0 sarvesh    (501) staff       (20)     4819 2023-06-05 13:03:57.000000 test_graphql_sdk-0.0.9/src/airstack/execute_query.py
--rw-r--r--   0 sarvesh    (501) staff       (20)     5723 2023-06-02 16:57:40.000000 test_graphql_sdk-0.0.9/src/airstack/generic.py
--rw-r--r--   0 sarvesh    (501) staff       (20)     1816 2023-06-05 13:02:01.000000 test_graphql_sdk-0.0.9/src/airstack/send_request.py
-drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-05 13:04:17.979584 test_graphql_sdk-0.0.9/src/test_graphql_sdk.egg-info/
--rw-r--r--   0 sarvesh    (501) staff       (20)     3204 2023-06-05 13:04:17.000000 test_graphql_sdk-0.0.9/src/test_graphql_sdk.egg-info/PKG-INFO
--rw-r--r--   0 sarvesh    (501) staff       (20)      343 2023-06-05 13:04:17.000000 test_graphql_sdk-0.0.9/src/test_graphql_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 sarvesh    (501) staff       (20)        1 2023-06-05 13:04:17.000000 test_graphql_sdk-0.0.9/src/test_graphql_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 sarvesh    (501) staff       (20)        9 2023-06-05 13:04:17.000000 test_graphql_sdk-0.0.9/src/test_graphql_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-06 10:10:29.729888 test_graphql_sdk-0.1.0/
+-rw-r--r--   0 sarvesh    (501) staff       (20)     3133 2023-06-06 10:10:29.729944 test_graphql_sdk-0.1.0/PKG-INFO
+-rw-r--r--   0 sarvesh    (501) staff       (20)     2621 2023-06-06 09:14:13.000000 test_graphql_sdk-0.1.0/README.md
+-rw-r--r--   0 sarvesh    (501) staff       (20)       85 2023-05-31 07:35:04.000000 test_graphql_sdk-0.1.0/pyproject.toml
+-rw-r--r--   0 sarvesh    (501) staff       (20)      716 2023-06-06 10:10:29.730181 test_graphql_sdk-0.1.0/setup.cfg
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-06 10:10:29.728013 test_graphql_sdk-0.1.0/src/
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-06 10:10:29.729097 test_graphql_sdk-0.1.0/src/airstack/
+-rw-r--r--   0 sarvesh    (501) staff       (20)        0 2023-06-05 12:53:03.000000 test_graphql_sdk-0.1.0/src/airstack/__init__.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)      308 2023-06-06 08:53:37.000000 test_graphql_sdk-0.1.0/src/airstack/constant.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)     6370 2023-06-06 09:32:09.000000 test_graphql_sdk-0.1.0/src/airstack/execute_query.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)     5805 2023-06-06 08:57:11.000000 test_graphql_sdk-0.1.0/src/airstack/generic.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)     1816 2023-06-06 08:57:31.000000 test_graphql_sdk-0.1.0/src/airstack/send_request.py
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-06 10:10:29.729761 test_graphql_sdk-0.1.0/src/test_graphql_sdk.egg-info/
+-rw-r--r--   0 sarvesh    (501) staff       (20)     3133 2023-06-06 10:10:29.000000 test_graphql_sdk-0.1.0/src/test_graphql_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 sarvesh    (501) staff       (20)      386 2023-06-06 10:10:29.000000 test_graphql_sdk-0.1.0/src/test_graphql_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 sarvesh    (501) staff       (20)        1 2023-06-06 10:10:29.000000 test_graphql_sdk-0.1.0/src/test_graphql_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 sarvesh    (501) staff       (20)       35 2023-06-06 10:10:29.000000 test_graphql_sdk-0.1.0/src/test_graphql_sdk.egg-info/requires.txt
+-rw-r--r--   0 sarvesh    (501) staff       (20)        9 2023-06-06 10:10:29.000000 test_graphql_sdk-0.1.0/src/test_graphql_sdk.egg-info/top_level.txt
```

### Comparing `test_graphql_sdk-0.0.9/PKG-INFO` & `test_graphql_sdk-0.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test_graphql_sdk
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python sdk for airstack apis
 Home-page: https://github.com/Airstack-xyz/airstack-python-sdk
 Author: Sarvesh
 Author-email: sarveshsingh.03@gmail.com
 Project-URL: Bug Tracker, https://github.com/Airstack-xyz/airstack-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,68 +14,63 @@
 
 # airstack-python-sdk
 
 The Airstack Python SDK is a library that allows Python developers to integrate Airstack's blockchain functionalities into their applications. With this SDK, developers can perform various tasks, such as querying and fetching data from smart contracts, displaying NFT assets.
 
 # Installation
 
-`pip3 install test-graphql-sdk`
+`pip3 install test_graphql_sdk`
 
 # Getting started
 To use the SDK you will need airstack api-key, which you can find in your profile setting section in airstack web, once you have it you can initialise the Airstackclient with the api-key.
 ```python
 from airstack.execute_query import AirstackClient
 
 api_client = AirstackClient(api_key='api-key')
 
 ```
 
 # Methods
 ## execute_query
-The execute query method query the data and return the data in asynchronous, it returns below data
-- `data`: data returned by the query
-- `status_code`: status code of the query response
-- `error`: any error that occurred while loading the query
+The execute query method query the data and return the data in asynchronous, it returns query_response which has below data
+- `query_response.data`: data returned by the query
+- `query_response.status_code`: status code of the query response
+- `query_response.error`: any error that occurred while loading the query
 
 ### Example
 ```python
 from airstack.execute_query import AirstackClient
 
 api_client = AirstackClient(api_key='api-key')
 
-data, status_code, error = await api_client.execute_query(query=query, variables=variables)
+query_response = await api_client.execute_query(query=query, variables=variables)
 ```
 
 ## execute_paginated_query
 **Note:** pagination methods only works with queries that has support for pagination, and the query passed to method must have a cursor as argument for it to work.
 
-The `execute_paginated_query` method provides a simple way to paginate the data returned by a query. It works the same as the `execute_query` method, but also returns an object with the following properties:
+The `execute_paginated_query` method provides a simple way to paginate the data returned by a query. It works the same as the `execute_query` method, it returns query_response which has below data:
 
-- `data`: data returned by the query
-- `status_code`: status code of the query response
-- `error`: any error that occurred while loading the query
-- `has_next_page`: a boolean indicating whether there is another page of data after the current page
-- `has_prev_page`: a boolean indicating whether there is another page of data before the current page
-- `get_next_page`: a function that can be called to fetch the next page of data
-- `get_prev_page`: a function that can be called to fetch the previous page of data
+- `query_response.data`: data returned by the query
+- `query_response.status_code`: status code of the query response
+- `query_response.error`: any error that occurred while loading the query
+- `query_response.has_next_page`: a boolean indicating whether there is another page of data after the current page
+- `query_response.has_prev_page`: a boolean indicating whether there is another page of data before the current page
+- `query_response.get_next_page()`: a function that can be called to fetch the next page of data
+- `query_response.get_prev_page()`: a function that can be called to fetch the previous page of data
 
 ### Example
 ```python
 from airstack.execute_query import AirstackClient
 
 api_client = AirstackClient(api_key='api-key')
 
-data, status_code, error, has_next_page, has_prev_page, get_next_page,
-get_prev_page = await api_client.execute_paginated_query(query=query, variables=variables)
+query_response = await api_client.execute_paginated_query(query=query, variables=variables)
 
-if has_next_page:
-    next_page_response, next_page_status, next_page_error, has_next_page, has_prev_page, get_next_page, get_prev_page = await get_next_page()
+if query_response.has_next_page:
+    next_page_response = await get_next_page()
 
-if has_prev_page:
-    prev_page_response, prev_page_status, prev_page_error, has_next_page, has_prev_page, get_next_page, get_prev_page = await get_prev_page()
+if next_page_response.has_prev_page:
+    prev_page_response = await get_prev_page()
 ```
 
 
-
-
-
-
```

### Comparing `test_graphql_sdk-0.0.9/README.md` & `test_graphql_sdk-0.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,62 @@
 # airstack-python-sdk
 
 The Airstack Python SDK is a library that allows Python developers to integrate Airstack's blockchain functionalities into their applications. With this SDK, developers can perform various tasks, such as querying and fetching data from smart contracts, displaying NFT assets.
 
 # Installation
 
-`pip3 install test-graphql-sdk`
+`pip3 install test_graphql_sdk`
 
 # Getting started
 To use the SDK you will need airstack api-key, which you can find in your profile setting section in airstack web, once you have it you can initialise the Airstackclient with the api-key.
 ```python
 from airstack.execute_query import AirstackClient
 
 api_client = AirstackClient(api_key='api-key')
 
 ```
 
 # Methods
 ## execute_query
-The execute query method query the data and return the data in asynchronous, it returns below data
-- `data`: data returned by the query
-- `status_code`: status code of the query response
-- `error`: any error that occurred while loading the query
+The execute query method query the data and return the data in asynchronous, it returns query_response which has below data
+- `query_response.data`: data returned by the query
+- `query_response.status_code`: status code of the query response
+- `query_response.error`: any error that occurred while loading the query
 
 ### Example
 ```python
 from airstack.execute_query import AirstackClient
 
 api_client = AirstackClient(api_key='api-key')
 
-data, status_code, error = await api_client.execute_query(query=query, variables=variables)
+query_response = await api_client.execute_query(query=query, variables=variables)
 ```
 
 ## execute_paginated_query
 **Note:** pagination methods only works with queries that has support for pagination, and the query passed to method must have a cursor as argument for it to work.
 
-The `execute_paginated_query` method provides a simple way to paginate the data returned by a query. It works the same as the `execute_query` method, but also returns an object with the following properties:
+The `execute_paginated_query` method provides a simple way to paginate the data returned by a query. It works the same as the `execute_query` method, it returns query_response which has below data:
 
-- `data`: data returned by the query
-- `status_code`: status code of the query response
-- `error`: any error that occurred while loading the query
-- `has_next_page`: a boolean indicating whether there is another page of data after the current page
-- `has_prev_page`: a boolean indicating whether there is another page of data before the current page
-- `get_next_page`: a function that can be called to fetch the next page of data
-- `get_prev_page`: a function that can be called to fetch the previous page of data
+- `query_response.data`: data returned by the query
+- `query_response.status_code`: status code of the query response
+- `query_response.error`: any error that occurred while loading the query
+- `query_response.has_next_page`: a boolean indicating whether there is another page of data after the current page
+- `query_response.has_prev_page`: a boolean indicating whether there is another page of data before the current page
+- `query_response.get_next_page()`: a function that can be called to fetch the next page of data
+- `query_response.get_prev_page()`: a function that can be called to fetch the previous page of data
 
 ### Example
 ```python
 from airstack.execute_query import AirstackClient
 
 api_client = AirstackClient(api_key='api-key')
 
-data, status_code, error, has_next_page, has_prev_page, get_next_page,
-get_prev_page = await api_client.execute_paginated_query(query=query, variables=variables)
+query_response = await api_client.execute_paginated_query(query=query, variables=variables)
 
-if has_next_page:
-    next_page_response, next_page_status, next_page_error, has_next_page, has_prev_page, get_next_page, get_prev_page = await get_next_page()
+if query_response.has_next_page:
+    next_page_response = await get_next_page()
 
-if has_prev_page:
-    prev_page_response, prev_page_status, prev_page_error, has_next_page, has_prev_page, get_next_page, get_prev_page = await get_prev_page()
+if next_page_response.has_prev_page:
+    prev_page_response = await get_prev_page()
 ```
 
 
-
-
-
-
```

### Comparing `test_graphql_sdk-0.0.9/setup.cfg` & `test_graphql_sdk-0.1.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = test_graphql_sdk
-version = 0.0.9
+version = 0.1.0
 author = Sarvesh
 author_email = sarveshsingh.03@gmail.com
 description = Python sdk for airstack apis
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Airstack-xyz/airstack-python-sdk
 project_urls = 
@@ -15,14 +15,17 @@
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
+install_requires = 
+	aiohttp==3.8.4
+	graphql-core==2.3.1
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `test_graphql_sdk-0.0.9/src/airstack/generic.py` & `test_graphql_sdk-0.1.0/src/airstack/generic.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,21 +59,24 @@
     Returns:
 
     """
     for definition in ast.definitions:
         if definition.operation == "query":
             for selection in definition.selection_set.selections:
                 if isinstance(selection, Field):
-                    if selection.name.value == field_name or (selection.alias and selection.alias.value == field_name):
+                    if selection.name.value == field_name or (selection.alias and
+                    selection.alias.value == field_name):
                         arguments = selection.arguments
                         if not arguments:
-                            # If no arguments are present, create a new input argument with the cursor field
+                            # If no arguments are present, create a new input argument
+                            # with the cursor field
                             argument = Argument(
                                 name=Name(value='input'),
-                                value=ObjectValue(fields=[create_object_field('cursor', cursor_value)])
+                                value=ObjectValue(fields=[create_object_field('cursor',
+                                cursor_value)])
                             )
                             selection.arguments.append(argument)
                         else:
                             # If input argument exists, check if it already has a cursor field
                             for argument in arguments:
                                 if argument.name.value == 'input':
                                     input_value = argument.value
```

### Comparing `test_graphql_sdk-0.0.9/src/airstack/send_request.py` & `test_graphql_sdk-0.1.0/src/airstack/send_request.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = 'sarvesh.singh'
 
-import aiohttp
 import json
+import aiohttp
 from airstack.constant import AirstackConstants
 
 
 class SendRequest:
     """
     Send Request
     """
```

### Comparing `test_graphql_sdk-0.0.9/src/test_graphql_sdk.egg-info/PKG-INFO` & `test_graphql_sdk-0.1.0/src/test_graphql_sdk.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-graphql-sdk
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python sdk for airstack apis
 Home-page: https://github.com/Airstack-xyz/airstack-python-sdk
 Author: Sarvesh
 Author-email: sarveshsingh.03@gmail.com
 Project-URL: Bug Tracker, https://github.com/Airstack-xyz/airstack-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,68 +14,63 @@
 
 # airstack-python-sdk
 
 The Airstack Python SDK is a library that allows Python developers to integrate Airstack's blockchain functionalities into their applications. With this SDK, developers can perform various tasks, such as querying and fetching data from smart contracts, displaying NFT assets.
 
 # Installation
 
-`pip3 install test-graphql-sdk`
+`pip3 install test_graphql_sdk`
 
 # Getting started
 To use the SDK you will need airstack api-key, which you can find in your profile setting section in airstack web, once you have it you can initialise the Airstackclient with the api-key.
 ```python
 from airstack.execute_query import AirstackClient
 
 api_client = AirstackClient(api_key='api-key')
 
 ```
 
 # Methods
 ## execute_query
-The execute query method query the data and return the data in asynchronous, it returns below data
-- `data`: data returned by the query
-- `status_code`: status code of the query response
-- `error`: any error that occurred while loading the query
+The execute query method query the data and return the data in asynchronous, it returns query_response which has below data
+- `query_response.data`: data returned by the query
+- `query_response.status_code`: status code of the query response
+- `query_response.error`: any error that occurred while loading the query
 
 ### Example
 ```python
 from airstack.execute_query import AirstackClient
 
 api_client = AirstackClient(api_key='api-key')
 
-data, status_code, error = await api_client.execute_query(query=query, variables=variables)
+query_response = await api_client.execute_query(query=query, variables=variables)
 ```
 
 ## execute_paginated_query
 **Note:** pagination methods only works with queries that has support for pagination, and the query passed to method must have a cursor as argument for it to work.
 
-The `execute_paginated_query` method provides a simple way to paginate the data returned by a query. It works the same as the `execute_query` method, but also returns an object with the following properties:
+The `execute_paginated_query` method provides a simple way to paginate the data returned by a query. It works the same as the `execute_query` method, it returns query_response which has below data:
 
-- `data`: data returned by the query
-- `status_code`: status code of the query response
-- `error`: any error that occurred while loading the query
-- `has_next_page`: a boolean indicating whether there is another page of data after the current page
-- `has_prev_page`: a boolean indicating whether there is another page of data before the current page
-- `get_next_page`: a function that can be called to fetch the next page of data
-- `get_prev_page`: a function that can be called to fetch the previous page of data
+- `query_response.data`: data returned by the query
+- `query_response.status_code`: status code of the query response
+- `query_response.error`: any error that occurred while loading the query
+- `query_response.has_next_page`: a boolean indicating whether there is another page of data after the current page
+- `query_response.has_prev_page`: a boolean indicating whether there is another page of data before the current page
+- `query_response.get_next_page()`: a function that can be called to fetch the next page of data
+- `query_response.get_prev_page()`: a function that can be called to fetch the previous page of data
 
 ### Example
 ```python
 from airstack.execute_query import AirstackClient
 
 api_client = AirstackClient(api_key='api-key')
 
-data, status_code, error, has_next_page, has_prev_page, get_next_page,
-get_prev_page = await api_client.execute_paginated_query(query=query, variables=variables)
+query_response = await api_client.execute_paginated_query(query=query, variables=variables)
 
-if has_next_page:
-    next_page_response, next_page_status, next_page_error, has_next_page, has_prev_page, get_next_page, get_prev_page = await get_next_page()
+if query_response.has_next_page:
+    next_page_response = await get_next_page()
 
-if has_prev_page:
-    prev_page_response, prev_page_status, prev_page_error, has_next_page, has_prev_page, get_next_page, get_prev_page = await get_prev_page()
+if next_page_response.has_prev_page:
+    prev_page_response = await get_prev_page()
 ```
 
 
-
-
-
-
```

