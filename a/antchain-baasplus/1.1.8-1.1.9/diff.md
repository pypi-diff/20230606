# Comparing `tmp/antchain_baasplus-1.1.8.tar.gz` & `tmp/antchain_baasplus-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_baasplus-1.1.8.tar", last modified: Tue Jun  6 02:45:19 2023, max compression
+gzip compressed data, was "dist/antchain_baasplus-1.1.9.tar", last modified: Tue Jun  6 04:52:45 2023, max compression
```

## Comparing `antchain_baasplus-1.1.8.tar` & `antchain_baasplus-1.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:45:19.000000 antchain_baasplus-1.1.8/
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-06 02:45:18.000000 antchain_baasplus-1.1.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-06 02:45:18.000000 antchain_baasplus-1.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2192 2023-06-06 02:45:19.000000 antchain_baasplus-1.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      819 2023-06-06 02:45:18.000000 antchain_baasplus-1.1.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1005 2023-06-06 02:45:18.000000 antchain_baasplus-1.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:45:19.000000 antchain_baasplus-1.1.8/antchain_baasplus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2192 2023-06-06 02:45:18.000000 antchain_baasplus-1.1.8/antchain_baasplus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      363 2023-06-06 02:45:19.000000 antchain_baasplus-1.1.8/antchain_baasplus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:45:18.000000 antchain_baasplus-1.1.8/antchain_baasplus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-06 02:45:18.000000 antchain_baasplus-1.1.8/antchain_baasplus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-06 02:45:18.000000 antchain_baasplus-1.1.8/antchain_baasplus.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:45:19.000000 antchain_baasplus-1.1.8/antchain_sdk_baasplus/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-06 02:45:18.000000 antchain_baasplus-1.1.8/antchain_sdk_baasplus/__init__.py
--rw-r--r--   0 root         (0) root         (0)   204189 2023-06-06 02:45:18.000000 antchain_baasplus-1.1.8/antchain_sdk_baasplus/client.py
--rw-r--r--   0 root         (0) root         (0)   355257 2023-06-06 02:45:18.000000 antchain_baasplus-1.1.8/antchain_sdk_baasplus/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-06 02:45:19.000000 antchain_baasplus-1.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2513 2023-06-06 02:45:18.000000 antchain_baasplus-1.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 04:52:45.000000 antchain_baasplus-1.1.9/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-06 04:52:44.000000 antchain_baasplus-1.1.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-06 04:52:44.000000 antchain_baasplus-1.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-06-06 04:52:45.000000 antchain_baasplus-1.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      819 2023-06-06 04:52:44.000000 antchain_baasplus-1.1.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1005 2023-06-06 04:52:44.000000 antchain_baasplus-1.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 04:52:45.000000 antchain_baasplus-1.1.9/antchain_baasplus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-06-06 04:52:45.000000 antchain_baasplus-1.1.9/antchain_baasplus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      363 2023-06-06 04:52:45.000000 antchain_baasplus-1.1.9/antchain_baasplus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 04:52:45.000000 antchain_baasplus-1.1.9/antchain_baasplus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-06 04:52:45.000000 antchain_baasplus-1.1.9/antchain_baasplus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-06 04:52:45.000000 antchain_baasplus-1.1.9/antchain_baasplus.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 04:52:45.000000 antchain_baasplus-1.1.9/antchain_sdk_baasplus/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-06 04:52:44.000000 antchain_baasplus-1.1.9/antchain_sdk_baasplus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   204189 2023-06-06 04:52:44.000000 antchain_baasplus-1.1.9/antchain_sdk_baasplus/client.py
+-rw-r--r--   0 root         (0) root         (0)   355257 2023-06-06 04:52:44.000000 antchain_baasplus-1.1.9/antchain_sdk_baasplus/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-06 04:52:45.000000 antchain_baasplus-1.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2513 2023-06-06 04:52:44.000000 antchain_baasplus-1.1.9/setup.py
```

### Comparing `antchain_baasplus-1.1.8/LICENSE` & `antchain_baasplus-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_baasplus-1.1.8/PKG-INFO` & `antchain_baasplus-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_baasplus
-Version: 1.1.8
+Version: 1.1.9
 Summary: Ant Chain BAASPLUS SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_baasplus-1.1.8/README-CN.md` & `antchain_baasplus-1.1.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_baasplus-1.1.8/README.md` & `antchain_baasplus-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `antchain_baasplus-1.1.8/antchain_baasplus.egg-info/PKG-INFO` & `antchain_baasplus-1.1.9/antchain_baasplus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-baasplus
-Version: 1.1.8
+Version: 1.1.9
 Summary: Ant Chain BAASPLUS SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_baasplus-1.1.8/antchain_sdk_baasplus/client.py` & `antchain_baasplus-1.1.9/antchain_sdk_baasplus/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.1.8',
+                    'sdk_version': '1.1.9',
                     '_prod_code': 'BAASPLUS',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.1.8',
+                    'sdk_version': '1.1.9',
                     '_prod_code': 'BAASPLUS',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_baasplus-1.1.8/antchain_sdk_baasplus/models.py` & `antchain_baasplus-1.1.9/antchain_sdk_baasplus/models.py`

 * *Files identical despite different names*

### Comparing `antchain_baasplus-1.1.8/setup.py` & `antchain_baasplus-1.1.9/setup.py`

 * *Files identical despite different names*

