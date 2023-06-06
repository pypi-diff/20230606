# Comparing `tmp/antchain_baasplus-1.1.6.tar.gz` & `tmp/antchain_baasplus-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_baasplus-1.1.6.tar", last modified: Mon Apr 10 07:03:32 2023, max compression
+gzip compressed data, was "dist/antchain_baasplus-1.1.8.tar", last modified: Tue Jun  6 02:45:19 2023, max compression
```

## Comparing `antchain_baasplus-1.1.6.tar` & `antchain_baasplus-1.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:03:32.000000 antchain_baasplus-1.1.6/
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-10 07:03:31.000000 antchain_baasplus-1.1.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-10 07:03:31.000000 antchain_baasplus-1.1.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2192 2023-04-10 07:03:32.000000 antchain_baasplus-1.1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      819 2023-04-10 07:03:31.000000 antchain_baasplus-1.1.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1005 2023-04-10 07:03:31.000000 antchain_baasplus-1.1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:03:32.000000 antchain_baasplus-1.1.6/antchain_baasplus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2192 2023-04-10 07:03:31.000000 antchain_baasplus-1.1.6/antchain_baasplus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      363 2023-04-10 07:03:32.000000 antchain_baasplus-1.1.6/antchain_baasplus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 07:03:31.000000 antchain_baasplus-1.1.6/antchain_baasplus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-04-10 07:03:31.000000 antchain_baasplus-1.1.6/antchain_baasplus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-10 07:03:31.000000 antchain_baasplus-1.1.6/antchain_baasplus.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:03:32.000000 antchain_baasplus-1.1.6/antchain_sdk_baasplus/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-10 07:03:31.000000 antchain_baasplus-1.1.6/antchain_sdk_baasplus/__init__.py
--rw-r--r--   0 root         (0) root         (0)   204189 2023-04-10 07:03:31.000000 antchain_baasplus-1.1.6/antchain_sdk_baasplus/client.py
--rw-r--r--   0 root         (0) root         (0)   349423 2023-04-10 07:03:31.000000 antchain_baasplus-1.1.6/antchain_sdk_baasplus/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-10 07:03:32.000000 antchain_baasplus-1.1.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2513 2023-04-10 07:03:31.000000 antchain_baasplus-1.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:45:19.000000 antchain_baasplus-1.1.8/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-06 02:45:18.000000 antchain_baasplus-1.1.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-06 02:45:18.000000 antchain_baasplus-1.1.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-06-06 02:45:19.000000 antchain_baasplus-1.1.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      819 2023-06-06 02:45:18.000000 antchain_baasplus-1.1.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1005 2023-06-06 02:45:18.000000 antchain_baasplus-1.1.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:45:19.000000 antchain_baasplus-1.1.8/antchain_baasplus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-06-06 02:45:18.000000 antchain_baasplus-1.1.8/antchain_baasplus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      363 2023-06-06 02:45:19.000000 antchain_baasplus-1.1.8/antchain_baasplus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:45:18.000000 antchain_baasplus-1.1.8/antchain_baasplus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-06 02:45:18.000000 antchain_baasplus-1.1.8/antchain_baasplus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-06 02:45:18.000000 antchain_baasplus-1.1.8/antchain_baasplus.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:45:19.000000 antchain_baasplus-1.1.8/antchain_sdk_baasplus/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-06 02:45:18.000000 antchain_baasplus-1.1.8/antchain_sdk_baasplus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   204189 2023-06-06 02:45:18.000000 antchain_baasplus-1.1.8/antchain_sdk_baasplus/client.py
+-rw-r--r--   0 root         (0) root         (0)   355257 2023-06-06 02:45:18.000000 antchain_baasplus-1.1.8/antchain_sdk_baasplus/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-06 02:45:19.000000 antchain_baasplus-1.1.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2513 2023-06-06 02:45:18.000000 antchain_baasplus-1.1.8/setup.py
```

### Comparing `antchain_baasplus-1.1.6/LICENSE` & `antchain_baasplus-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_baasplus-1.1.6/PKG-INFO` & `antchain_baasplus-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_baasplus
-Version: 1.1.6
+Version: 1.1.8
 Summary: Ant Chain BAASPLUS SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_baasplus-1.1.6/README-CN.md` & `antchain_baasplus-1.1.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_baasplus-1.1.6/README.md` & `antchain_baasplus-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `antchain_baasplus-1.1.6/antchain_baasplus.egg-info/PKG-INFO` & `antchain_baasplus-1.1.8/antchain_baasplus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-baasplus
-Version: 1.1.6
+Version: 1.1.8
 Summary: Ant Chain BAASPLUS SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_baasplus-1.1.6/antchain_sdk_baasplus/client.py` & `antchain_baasplus-1.1.8/antchain_sdk_baasplus/client.py`

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
-                    'sdk_version': '1.1.6',
+                    'sdk_version': '1.1.8',
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
-                    'sdk_version': '1.1.6',
+                    'sdk_version': '1.1.8',
                     '_prod_code': 'BAASPLUS',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_baasplus-1.1.6/antchain_sdk_baasplus/models.py` & `antchain_baasplus-1.1.8/antchain_sdk_baasplus/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -3831,14 +3831,22 @@
         result_msg: str = None,
         code: str = None,
         enterprise_status: str = None,
         open_time: str = None,
         passed: bool = None,
         return_code: str = None,
         reason_code: str = None,
+        legal_name: str = None,
+        legal_name_msg: str = None,
+        legal_id_no: str = None,
+        legal_id_no_msg: str = None,
+        ent_name: str = None,
+        ent_name_msg: str = None,
+        reg_no: str = None,
+        reg_no_msg: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
@@ -3856,14 +3864,30 @@
         # resultCode=1，核验不一致（人企核验不一致）
         # resultCode=2，库无（人在库中不存在，无法校验）
         # resultCode=3，企业二要素核验不通过
         # resultCode=4，查无企业，无法校验（此场景属于三要素核验）
         self.return_code = return_code
         # 核验不一致的原因编码
         self.reason_code = reason_code
+        # 法人姓名：1，2，3
+        self.legal_name = legal_name
+        # 法人姓名：1.一致 2.不一致 3.无法验证
+        self.legal_name_msg = legal_name_msg
+        # 1.一致 2.不一致 3.无法验证
+        self.legal_id_no = legal_id_no
+        # 法人身份证号：1.一致 2.不一致 3.无法核验
+        self.legal_id_no_msg = legal_id_no_msg
+        # 企业名称 1.一致 2.不一致 3.无法验证
+        self.ent_name = ent_name
+        # 企业名称 1.一致 2.不一致 3.无法验证
+        self.ent_name_msg = ent_name_msg
+        # 社会统一信用代码/注册号： 1.一致 2.不一致 3.无法验证
+        self.reg_no = reg_no
+        # 社会统一信用代码/注册号： 1.一致 2.不一致 3.无法验证
+        self.reg_no_msg = reg_no_msg
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -3884,14 +3908,30 @@
             result['open_time'] = self.open_time
         if self.passed is not None:
             result['passed'] = self.passed
         if self.return_code is not None:
             result['return_code'] = self.return_code
         if self.reason_code is not None:
             result['reason_code'] = self.reason_code
+        if self.legal_name is not None:
+            result['legal_name'] = self.legal_name
+        if self.legal_name_msg is not None:
+            result['legal_name_msg'] = self.legal_name_msg
+        if self.legal_id_no is not None:
+            result['legal_id_no'] = self.legal_id_no
+        if self.legal_id_no_msg is not None:
+            result['legal_id_no_msg'] = self.legal_id_no_msg
+        if self.ent_name is not None:
+            result['ent_name'] = self.ent_name
+        if self.ent_name_msg is not None:
+            result['ent_name_msg'] = self.ent_name_msg
+        if self.reg_no is not None:
+            result['reg_no'] = self.reg_no
+        if self.reg_no_msg is not None:
+            result['reg_no_msg'] = self.reg_no_msg
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
@@ -3906,14 +3946,30 @@
             self.open_time = m.get('open_time')
         if m.get('passed') is not None:
             self.passed = m.get('passed')
         if m.get('return_code') is not None:
             self.return_code = m.get('return_code')
         if m.get('reason_code') is not None:
             self.reason_code = m.get('reason_code')
+        if m.get('legal_name') is not None:
+            self.legal_name = m.get('legal_name')
+        if m.get('legal_name_msg') is not None:
+            self.legal_name_msg = m.get('legal_name_msg')
+        if m.get('legal_id_no') is not None:
+            self.legal_id_no = m.get('legal_id_no')
+        if m.get('legal_id_no_msg') is not None:
+            self.legal_id_no_msg = m.get('legal_id_no_msg')
+        if m.get('ent_name') is not None:
+            self.ent_name = m.get('ent_name')
+        if m.get('ent_name_msg') is not None:
+            self.ent_name_msg = m.get('ent_name_msg')
+        if m.get('reg_no') is not None:
+            self.reg_no = m.get('reg_no')
+        if m.get('reg_no_msg') is not None:
+            self.reg_no_msg = m.get('reg_no_msg')
         return self
 
 
 class QueryEverifyThreemetaRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
@@ -3978,14 +4034,20 @@
         result_msg: str = None,
         code: str = None,
         enterprise_status: str = None,
         open_time: str = None,
         passed: bool = None,
         return_code: str = None,
         reason_code: str = None,
+        ent_name: str = None,
+        ent_name_msg: str = None,
+        reg_no: str = None,
+        reg_no_msg: str = None,
+        legal_name: str = None,
+        legal_name_msg: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
@@ -4003,14 +4065,28 @@
         # resultCode=1，核验不一致（人企核验不一致）
         # resultCode=2，库无（人在库中不存在，无法校验）
         # resultCode=3，企业二要素核验不通过
         # resultCode=4，查无企业，无法校验（此场景属于三要素核验）
         self.return_code = return_code
         # 核验不通过异常编码
         self.reason_code = reason_code
+        # 企业名称 1.一致 2.不一致 3.无法验证
+        self.ent_name = ent_name
+        # 企业名称 1.一致 2.不一致 3.无法验证
+        # 
+        self.ent_name_msg = ent_name_msg
+        # 社会统一信用代码/注册号： 1.一致 2.不一致 3.无法验证
+        self.reg_no = reg_no
+        # 社会统一信用代码/注册号： 1.一致 2.不一致 3.无法验证
+        self.reg_no_msg = reg_no_msg
+        # 法人姓名：1.一致 2.不一致 3.无法验证
+        # 
+        self.legal_name = legal_name
+        # 法人姓名：1.一致 2.不一致 3.无法验证
+        self.legal_name_msg = legal_name_msg
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -4031,14 +4107,26 @@
             result['open_time'] = self.open_time
         if self.passed is not None:
             result['passed'] = self.passed
         if self.return_code is not None:
             result['return_code'] = self.return_code
         if self.reason_code is not None:
             result['reason_code'] = self.reason_code
+        if self.ent_name is not None:
+            result['ent_name'] = self.ent_name
+        if self.ent_name_msg is not None:
+            result['ent_name_msg'] = self.ent_name_msg
+        if self.reg_no is not None:
+            result['reg_no'] = self.reg_no
+        if self.reg_no_msg is not None:
+            result['reg_no_msg'] = self.reg_no_msg
+        if self.legal_name is not None:
+            result['legal_name'] = self.legal_name
+        if self.legal_name_msg is not None:
+            result['legal_name_msg'] = self.legal_name_msg
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
@@ -4053,14 +4141,26 @@
             self.open_time = m.get('open_time')
         if m.get('passed') is not None:
             self.passed = m.get('passed')
         if m.get('return_code') is not None:
             self.return_code = m.get('return_code')
         if m.get('reason_code') is not None:
             self.reason_code = m.get('reason_code')
+        if m.get('ent_name') is not None:
+            self.ent_name = m.get('ent_name')
+        if m.get('ent_name_msg') is not None:
+            self.ent_name_msg = m.get('ent_name_msg')
+        if m.get('reg_no') is not None:
+            self.reg_no = m.get('reg_no')
+        if m.get('reg_no_msg') is not None:
+            self.reg_no_msg = m.get('reg_no_msg')
+        if m.get('legal_name') is not None:
+            self.legal_name = m.get('legal_name')
+        if m.get('legal_name_msg') is not None:
+            self.legal_name_msg = m.get('legal_name_msg')
         return self
 
 
 class QueryEverifyTwometaRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
@@ -4117,14 +4217,18 @@
         result_msg: str = None,
         enterprise_status: str = None,
         open_time: str = None,
         passed: bool = None,
         code: str = None,
         return_code: str = None,
         reason_code: str = None,
+        reg_no: str = None,
+        reg_no_msg: str = None,
+        ent_name: str = None,
+        ent_name_msg: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
@@ -4142,14 +4246,25 @@
         # resultCode=1，核验不一致（人企核验不一致）
         # resultCode=2，库无（人在库中不存在，无法校验）
         # resultCode=3，企业二要素核验不通过
         # resultCode=4，查无企业，无法校验（此场景属于三要素核验）
         self.return_code = return_code
         # 核验不通过异常编码
         self.reason_code = reason_code
+        # 社会统一信用代码/注册号： 1.一致 2.不一致 3.无法验证
+        # 
+        self.reg_no = reg_no
+        # 社会统一信用代码/注册号： 1.一致 2.不一致 3.无法验证
+        # 
+        self.reg_no_msg = reg_no_msg
+        # 企业名称 1.一致 2.不一致 3.无法验证
+        self.ent_name = ent_name
+        # 企业名称 1.一致 2.不一致 3.无法验证
+        # 
+        self.ent_name_msg = ent_name_msg
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -4170,14 +4285,22 @@
             result['passed'] = self.passed
         if self.code is not None:
             result['code'] = self.code
         if self.return_code is not None:
             result['return_code'] = self.return_code
         if self.reason_code is not None:
             result['reason_code'] = self.reason_code
+        if self.reg_no is not None:
+            result['reg_no'] = self.reg_no
+        if self.reg_no_msg is not None:
+            result['reg_no_msg'] = self.reg_no_msg
+        if self.ent_name is not None:
+            result['ent_name'] = self.ent_name
+        if self.ent_name_msg is not None:
+            result['ent_name_msg'] = self.ent_name_msg
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
@@ -4192,14 +4315,22 @@
             self.passed = m.get('passed')
         if m.get('code') is not None:
             self.code = m.get('code')
         if m.get('return_code') is not None:
             self.return_code = m.get('return_code')
         if m.get('reason_code') is not None:
             self.reason_code = m.get('reason_code')
+        if m.get('reg_no') is not None:
+            self.reg_no = m.get('reg_no')
+        if m.get('reg_no_msg') is not None:
+            self.reg_no_msg = m.get('reg_no_msg')
+        if m.get('ent_name') is not None:
+            self.ent_name = m.get('ent_name')
+        if m.get('ent_name_msg') is not None:
+            self.ent_name_msg = m.get('ent_name_msg')
         return self
 
 
 class QueryBaicorpInternalsearchlibraryRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
```

### Comparing `antchain_baasplus-1.1.6/setup.py` & `antchain_baasplus-1.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_baasplus.
 
-Created on 10/04/2023
+Created on 06/06/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_baasplus"
 NAME = "antchain_baasplus" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain BAASPLUS SDK Library for Python"
```

