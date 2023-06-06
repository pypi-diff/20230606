# Comparing `tmp/YOMAPI-0.1.7.tar.gz` & `tmp/YOMAPI-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/YOMAPI-0.1.7.tar", last modified: Mon May  8 18:36:50 2023, max compression
+gzip compressed data, was "dist/YOMAPI-0.1.8.tar", last modified: Tue Jun  6 20:37:26 2023, max compression
```

## Comparing `YOMAPI-0.1.7.tar` & `YOMAPI-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-08 18:36:50.000000 YOMAPI-0.1.7/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-08 18:36:50.000000 YOMAPI-0.1.7/YOMAPI/
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    39853 2023-05-08 18:36:41.000000 YOMAPI-0.1.7/YOMAPI/YOMAPI.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)       68 2023-05-08 18:36:41.000000 YOMAPI-0.1.7/YOMAPI/__init__.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)       39 2023-05-08 18:36:41.000000 YOMAPI-0.1.7/setup.cfg
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      922 2023-05-08 18:36:41.000000 YOMAPI-0.1.7/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      701 2023-05-08 18:36:50.000000 YOMAPI-0.1.7/PKG-INFO
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-06 20:37:26.000000 YOMAPI-0.1.8/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-06 20:37:26.000000 YOMAPI-0.1.8/YOMAPI/
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)    41142 2023-06-06 20:37:17.000000 YOMAPI-0.1.8/YOMAPI/YOMAPI.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)       68 2023-06-06 20:37:17.000000 YOMAPI-0.1.8/YOMAPI/__init__.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)       39 2023-06-06 20:37:17.000000 YOMAPI-0.1.8/setup.cfg
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      922 2023-06-06 20:37:17.000000 YOMAPI-0.1.8/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      701 2023-06-06 20:37:26.000000 YOMAPI-0.1.8/PKG-INFO
```

### Comparing `YOMAPI-0.1.7/YOMAPI/YOMAPI.py` & `YOMAPI-0.1.8/YOMAPI/YOMAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -1096,42 +1096,62 @@
             response = session.post(path, json.dumps(data))
             self.logger.info(f'Create Job Info Message: {data["message"]} Status Code: {response.status_code}')
             jsonResponse = response.json()
         except Exception as error:
             raise ApiResponseError(path, str(error))
         return jsonResponse
 
-
-    """
-    Integration Job info endpoints
-    """
     def end_job_info(self, data, token):
         id = data["id"]
         path = self.url_v3 + f'/api/v3/admin/data-import/integration-job-info/{id}'
         session = self.__build_session(token)
         try:
             response = session.put(path, json.dumps(data))
             self.logger.info(f'End Job Info Message: {data["message"]} Status Code: {response.status_code}')
             jsonResponse = response.json()
         except Exception as error:
             raise ApiResponseError(path, str(error))
         return jsonResponse
 
-
-    """
-    Integration Job info endpoints
-    """
     def update_job_info_subprocess(self, data, token):        
         id = data["id"]
         path = self.url_v3 + f'/api/v3/admin/data-import/integration-job-info/{id}/subprocess'
         session = self.__build_session(token)
         try:
             response = session.put(path, json.dumps(data))
             self.logger.info(f'Update Job Info Subprocess: {data["processName"]} Status Code: {response.status_code}')            
             if response.status_code < 200 or response.status_code >= 299:
                 self.logger.info(response._content)
             jsonResponse = response.json()
         except Exception as error:
             raise ApiResponseError(path, str(error))
-        return jsonResponse        
+        return jsonResponse    
+
+    def get_integration_job_infos(self, token=None, input_params=None, total_pages_override=None):
+        current_page = 0
+        total_pages = float('inf') if total_pages_override is None else total_pages_override
+        integration_job_infos = []
+        while(current_page < total_pages):
+            current_page += 1
+            status, response = self.__get_integration_job_info_page(page=current_page, limit=100, token=token, input_params=input_params)
+            integration_job_infos += response['docs']
+            if total_pages_override is None: 
+              total_pages = response['totalPages']
+            self.logger.info('Sending integration-info query for page {}/{}'.format(current_page, total_pages))
+        return integration_job_infos    
 
-        
+
+    def __get_integration_job_info_page(self, page, limit, token, input_params=None):
+        path = self.url_v3 + f'/api/v3/admin/data-import/integration-job-info/'
+        session = self.__build_session(token)
+        try:
+            params = {
+                'page': page,
+                'limit': limit
+            }
+            if input_params:
+                if 'sort' in input_params: params['sort'] = input_params['sort']
+
+            response = session.get(path, params=params)
+            return (response.status_code, response.json())
+        except Exception as error:
+            raise ApiResponseError(path, str(error))
```

### Comparing `YOMAPI-0.1.7/setup.py` & `YOMAPI-0.1.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from distutils.core import setup
 setup(
   name = 'YOMAPI',
   packages = ['YOMAPI'],
-  version = '0.1.7',
+  version = '0.1.8',
   license='MIT',
   description = 'A PACKAGE TO USE THE SAME YOM API INTERFACE FROM YOM INTEGRATIONS',
   author = 'Camilo Jiménez',
   author_email = 'camilo@youorder.me',
   url = 'https://github.com/user/reponame',
   # download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz', 
   keywords = ['YOM-INTEGRATIONS'],   # Keywords that define your package best
```

### Comparing `YOMAPI-0.1.7/PKG-INFO` & `YOMAPI-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: YOMAPI
-Version: 0.1.7
+Version: 0.1.8
 Summary: A PACKAGE TO USE THE SAME YOM API INTERFACE FROM YOM INTEGRATIONS
 Home-page: https://github.com/user/reponame
 Author: Camilo Jiménez
 Author-email: camilo@youorder.me
 License: MIT
 Description: UNKNOWN
 Keywords: YOM-INTEGRATIONS
```

