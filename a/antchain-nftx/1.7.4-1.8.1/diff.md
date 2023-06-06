# Comparing `tmp/antchain_nftx-1.7.4.tar.gz` & `tmp/antchain_nftx-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_nftx-1.7.4.tar", last modified: Fri Sep 16 06:42:15 2022, max compression
+gzip compressed data, was "dist/antchain_nftx-1.8.1.tar", last modified: Tue Jun  6 09:43:07 2023, max compression
```

## Comparing `antchain_nftx-1.7.4.tar` & `antchain_nftx-1.8.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 06:42:15.000000 antchain_nftx-1.7.4/
--rw-r--r--   0 root         (0) root         (0)      600 2022-09-16 06:42:15.000000 antchain_nftx-1.7.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-09-16 06:42:15.000000 antchain_nftx-1.7.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2168 2022-09-16 06:42:15.000000 antchain_nftx-1.7.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      807 2022-09-16 06:42:15.000000 antchain_nftx-1.7.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      993 2022-09-16 06:42:15.000000 antchain_nftx-1.7.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 06:42:15.000000 antchain_nftx-1.7.4/antchain_nftx.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2168 2022-09-16 06:42:15.000000 antchain_nftx-1.7.4/antchain_nftx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2022-09-16 06:42:15.000000 antchain_nftx-1.7.4/antchain_nftx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-16 06:42:15.000000 antchain_nftx-1.7.4/antchain_nftx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2022-09-16 06:42:15.000000 antchain_nftx-1.7.4/antchain_nftx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2022-09-16 06:42:15.000000 antchain_nftx-1.7.4/antchain_nftx.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 06:42:15.000000 antchain_nftx-1.7.4/antchain_sdk_nftx/
--rw-r--r--   0 root         (0) root         (0)       21 2022-09-16 06:42:15.000000 antchain_nftx-1.7.4/antchain_sdk_nftx/__init__.py
--rw-r--r--   0 root         (0) root         (0)    48029 2022-09-16 06:42:15.000000 antchain_nftx-1.7.4/antchain_sdk_nftx/client.py
--rw-r--r--   0 root         (0) root         (0)    96243 2022-09-16 06:42:15.000000 antchain_nftx-1.7.4/antchain_sdk_nftx/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2022-09-16 06:42:15.000000 antchain_nftx-1.7.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2493 2022-09-16 06:42:15.000000 antchain_nftx-1.7.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      807 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      993 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/antchain_nftx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/antchain_nftx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/antchain_nftx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/antchain_nftx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/antchain_nftx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/antchain_nftx.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/antchain_sdk_nftx/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/antchain_sdk_nftx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    50083 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/antchain_sdk_nftx/client.py
+-rw-r--r--   0 root         (0) root         (0)    99666 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/antchain_sdk_nftx/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2493 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/setup.py
```

### Comparing `antchain_nftx-1.7.4/LICENSE` & `antchain_nftx-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_nftx-1.7.4/PKG-INFO` & `antchain_nftx-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_nftx
-Version: 1.7.4
+Version: 1.8.1
 Summary: Ant Chain NFTX SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_nftx-1.7.4/README-CN.md` & `antchain_nftx-1.8.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_nftx-1.7.4/README.md` & `antchain_nftx-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `antchain_nftx-1.7.4/antchain_nftx.egg-info/PKG-INFO` & `antchain_nftx-1.8.1/antchain_nftx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-nftx
-Version: 1.7.4
+Version: 1.8.1
 Summary: Ant Chain NFTX SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_nftx-1.7.4/antchain_sdk_nftx/client.py` & `antchain_nftx-1.8.1/antchain_sdk_nftx/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             'readTimeout': UtilClient.default_number(runtime.read_timeout, self._read_timeout),
             'connectTimeout': UtilClient.default_number(runtime.connect_timeout, self._connect_timeout),
             'httpProxy': UtilClient.default_string(runtime.http_proxy, self._http_proxy),
             'httpsProxy': UtilClient.default_string(runtime.https_proxy, self._https_proxy),
             'noProxy': UtilClient.default_string(runtime.no_proxy, self._no_proxy),
             'maxIdleConns': UtilClient.default_number(runtime.max_idle_conns, self._max_idle_conns),
             'maxIdleTimeMillis': self._max_idle_time_millis,
-            'keepAliveDurationMillis': self._keep_alive_duration_millis,
+            'keepAliveDuration': self._keep_alive_duration_millis,
             'maxRequests': self._max_requests,
             'maxRequestsPerHost': self._max_requests_per_host,
             'retry': {
                 'retryable': runtime.autoretry,
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.7.4',
+                    'sdk_version': '1.8.1',
                     '_prod_code': 'NFTX',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -198,15 +198,15 @@
             'readTimeout': UtilClient.default_number(runtime.read_timeout, self._read_timeout),
             'connectTimeout': UtilClient.default_number(runtime.connect_timeout, self._connect_timeout),
             'httpProxy': UtilClient.default_string(runtime.http_proxy, self._http_proxy),
             'httpsProxy': UtilClient.default_string(runtime.https_proxy, self._https_proxy),
             'noProxy': UtilClient.default_string(runtime.no_proxy, self._no_proxy),
             'maxIdleConns': UtilClient.default_number(runtime.max_idle_conns, self._max_idle_conns),
             'maxIdleTimeMillis': self._max_idle_time_millis,
-            'keepAliveDurationMillis': self._keep_alive_duration_millis,
+            'keepAliveDuration': self._keep_alive_duration_millis,
             'maxRequests': self._max_requests,
             'maxRequestsPerHost': self._max_requests_per_host,
             'retry': {
                 'retryable': runtime.autoretry,
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.7.4',
+                    'sdk_version': '1.8.1',
                     '_prod_code': 'NFTX',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -1166,7 +1166,63 @@
         Summary: 拿authcode换token
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             nftx_models.ApplyOauthTokenResponse(),
             await self.do_request_async('1.0', 'antchain.nftx.oauth.token.apply', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
+
+    def query_oauth_userinfo(
+        self,
+        request: nftx_models.QueryOauthUserinfoRequest,
+    ) -> nftx_models.QueryOauthUserinfoResponse:
+        """
+        Description: 获取用户信息
+        Summary: 获取用户信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_oauth_userinfo_ex(request, headers, runtime)
+
+    async def query_oauth_userinfo_async(
+        self,
+        request: nftx_models.QueryOauthUserinfoRequest,
+    ) -> nftx_models.QueryOauthUserinfoResponse:
+        """
+        Description: 获取用户信息
+        Summary: 获取用户信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_oauth_userinfo_ex_async(request, headers, runtime)
+
+    def query_oauth_userinfo_ex(
+        self,
+        request: nftx_models.QueryOauthUserinfoRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> nftx_models.QueryOauthUserinfoResponse:
+        """
+        Description: 获取用户信息
+        Summary: 获取用户信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            nftx_models.QueryOauthUserinfoResponse(),
+            self.do_request('1.0', 'antchain.nftx.oauth.userinfo.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_oauth_userinfo_ex_async(
+        self,
+        request: nftx_models.QueryOauthUserinfoRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> nftx_models.QueryOauthUserinfoResponse:
+        """
+        Description: 获取用户信息
+        Summary: 获取用户信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            nftx_models.QueryOauthUserinfoResponse(),
+            await self.do_request_async('1.0', 'antchain.nftx.oauth.userinfo.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
```

### Comparing `antchain_nftx-1.7.4/antchain_sdk_nftx/models.py` & `antchain_nftx-1.8.1/antchain_sdk_nftx/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2626,7 +2626,111 @@
         if m.get('refresh_token') is not None:
             self.refresh_token = m.get('refresh_token')
         if m.get('refresh_expire_time') is not None:
             self.refresh_expire_time = m.get('refresh_expire_time')
         return self
 
 
+class QueryOauthUserinfoRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        access_token: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 授权token
+        self.access_token = access_token
+
+    def validate(self):
+        self.validate_required(self.access_token, 'access_token')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.access_token is not None:
+            result['access_token'] = self.access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('access_token') is not None:
+            self.access_token = m.get('access_token')
+        return self
+
+
+class QueryOauthUserinfoResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        nick_name: str = None,
+        avatar: str = None,
+        open_user_id: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 用户昵称
+        self.nick_name = nick_name
+        # 头像链接
+        self.avatar = avatar
+        # open_user_id
+        self.open_user_id = open_user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.nick_name is not None:
+            result['nick_name'] = self.nick_name
+        if self.avatar is not None:
+            result['avatar'] = self.avatar
+        if self.open_user_id is not None:
+            result['open_user_id'] = self.open_user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('nick_name') is not None:
+            self.nick_name = m.get('nick_name')
+        if m.get('avatar') is not None:
+            self.avatar = m.get('avatar')
+        if m.get('open_user_id') is not None:
+            self.open_user_id = m.get('open_user_id')
+        return self
+
+
```

### Comparing `antchain_nftx-1.7.4/setup.py` & `antchain_nftx-1.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_nftx.
 
-Created on 16/09/2022
+Created on 06/06/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_nftx"
 NAME = "antchain_nftx" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain NFTX SDK Library for Python"
 AUTHOR = "Ant Chain SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/alipay/antchain-openapi-prod-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "antchain_alipay_util>=1.0.1, <2.0.0",
-    "alibabacloud_tea_util>=0.3.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.8, <1.0.0",
     "alibabacloud_rpc_util>=0.0.4, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

