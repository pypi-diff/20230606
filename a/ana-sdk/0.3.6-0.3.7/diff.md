# Comparing `tmp/ana_sdk-0.3.6.tar.gz` & `tmp/ana_sdk-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ana_sdk-0.3.6.tar", max compression
+gzip compressed data, was "ana_sdk-0.3.7.tar", max compression
```

## Comparing `ana_sdk-0.3.6.tar` & `ana_sdk-0.3.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       20 2023-05-22 13:09:55.929573 ana_sdk-0.3.6/ana_sdk/__init__.py
--rw-r--r--   0        0        0    14393 2023-06-02 01:39:27.893197 ana_sdk-0.3.6/ana_sdk/ana.py
--rw-r--r--   0        0        0      138 2023-06-01 17:01:33.190199 ana_sdk-0.3.6/ana_sdk/clients/__init__.py
--rw-r--r--   0        0        0     4480 2023-06-01 17:05:04.633378 ana_sdk-0.3.6/ana_sdk/clients/ana_data_client.py
--rw-r--r--   0        0        0     1725 2023-06-01 16:58:50.036423 ana_sdk-0.3.6/ana_sdk/clients/base_client.py
--rw-r--r--   0        0        0     4634 2023-06-01 17:00:04.904107 ana_sdk-0.3.6/ana_sdk/clients/dashboard_api_client.py
--rw-r--r--   0        0        0     1438 2023-05-23 03:23:45.283114 ana_sdk-0.3.6/ana_sdk/clients/oauth_client.py
--rw-r--r--   0        0        0     3218 2023-06-01 16:57:50.848033 ana_sdk-0.3.6/ana_sdk/clients/rpa_api_client.py
--rw-r--r--   0        0        0      744 2023-05-25 20:23:48.737805 ana_sdk-0.3.6/ana_sdk/exceptions/__init__.py
--rw-r--r--   0        0        0      670 2023-06-01 17:03:26.358183 ana_sdk-0.3.6/ana_sdk/requests_auth.py
--rw-r--r--   0        0        0     4934 2023-05-25 23:15:52.044789 ana_sdk-0.3.6/ana_sdk/result_factory.py
--rw-r--r--   0        0        0      463 2023-06-02 01:39:45.457046 ana_sdk-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     2105 2023-05-22 13:11:05.921381 ana_sdk-0.3.6/README.md
--rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 ana_sdk-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0       20 2023-05-22 13:09:55.929573 ana_sdk-0.3.7/ana_sdk/__init__.py
+-rw-r--r--   0        0        0    14393 2023-06-02 01:39:27.893197 ana_sdk-0.3.7/ana_sdk/ana.py
+-rw-r--r--   0        0        0      138 2023-06-01 17:01:33.190199 ana_sdk-0.3.7/ana_sdk/clients/__init__.py
+-rw-r--r--   0        0        0     4480 2023-06-01 17:05:04.633378 ana_sdk-0.3.7/ana_sdk/clients/ana_data_client.py
+-rw-r--r--   0        0        0     1725 2023-06-01 16:58:50.036423 ana_sdk-0.3.7/ana_sdk/clients/base_client.py
+-rw-r--r--   0        0        0     4634 2023-06-01 17:00:04.904107 ana_sdk-0.3.7/ana_sdk/clients/dashboard_api_client.py
+-rw-r--r--   0        0        0     2747 2023-06-06 01:07:52.284429 ana_sdk-0.3.7/ana_sdk/clients/oauth_client.py
+-rw-r--r--   0        0        0     3218 2023-06-01 16:57:50.848033 ana_sdk-0.3.7/ana_sdk/clients/rpa_api_client.py
+-rw-r--r--   0        0        0      744 2023-05-25 20:23:48.737805 ana_sdk-0.3.7/ana_sdk/exceptions/__init__.py
+-rw-r--r--   0        0        0      733 2023-06-06 01:08:29.138897 ana_sdk-0.3.7/ana_sdk/requests_auth.py
+-rw-r--r--   0        0        0     4934 2023-05-25 23:15:52.044789 ana_sdk-0.3.7/ana_sdk/result_factory.py
+-rw-r--r--   0        0        0      463 2023-06-06 01:11:55.669087 ana_sdk-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     2105 2023-05-22 13:11:05.921381 ana_sdk-0.3.7/README.md
+-rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 ana_sdk-0.3.7/PKG-INFO
```

### Comparing `ana_sdk-0.3.6/ana_sdk/ana.py` & `ana_sdk-0.3.7/ana_sdk/ana.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.3.6/ana_sdk/clients/ana_data_client.py` & `ana_sdk-0.3.7/ana_sdk/clients/ana_data_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.3.6/ana_sdk/clients/base_client.py` & `ana_sdk-0.3.7/ana_sdk/clients/base_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.3.6/ana_sdk/clients/dashboard_api_client.py` & `ana_sdk-0.3.7/ana_sdk/clients/dashboard_api_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.3.6/ana_sdk/clients/rpa_api_client.py` & `ana_sdk-0.3.7/ana_sdk/clients/rpa_api_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.3.6/ana_sdk/exceptions/__init__.py` & `ana_sdk-0.3.7/ana_sdk/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.3.6/ana_sdk/requests_auth.py` & `ana_sdk-0.3.7/ana_sdk/requests_auth.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,11 +12,13 @@
         
         self.oauth_client = OAuthClient(
             self.email,
             self._password,
             self.env_oauth_token_full_url
         )
 
+        self._token = self.oauth_client.get_token()
+
     def __call__(self, r):
         access_token = self.oauth_client.get_token()["access_token"]
-        r.headers['Authorization'] = "Bearer " + access_token
+        r.headers['Authorization'] = "Bearer " + access_token        
         return r
```

### Comparing `ana_sdk-0.3.6/ana_sdk/result_factory.py` & `ana_sdk-0.3.7/ana_sdk/result_factory.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.3.6/README.md` & `ana_sdk-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.3.6/PKG-INFO` & `ana_sdk-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ana-sdk
-Version: 0.3.6
+Version: 0.3.7
 Summary: SDK que visa fornecer uma interface para interagir com os serviços ANA.
 License: MIT
 Author: Jovane Mafort
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

