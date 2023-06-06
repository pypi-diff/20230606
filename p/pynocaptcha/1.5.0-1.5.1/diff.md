# Comparing `tmp/pynocaptcha-1.5.0.tar.gz` & `tmp/pynocaptcha-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pynocaptcha-1.5.0.tar", last modified: Mon May 15 07:35:54 2023, max compression
+gzip compressed data, was "dist/pynocaptcha-1.5.1.tar", last modified: Tue Jun  6 02:58:09 2023, max compression
```

## Comparing `pynocaptcha-1.5.0.tar` & `pynocaptcha-1.5.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-05-15 07:35:54.000000 pynocaptcha-1.5.0/
--rw-r--r--   0 esbiya     (501) staff       (20)      566 2023-05-15 07:35:54.000000 pynocaptcha-1.5.0/PKG-INFO
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-05-15 07:35:54.000000 pynocaptcha-1.5.0/pynocaptcha/
--rw-r--r--   0 esbiya     (501) staff       (20)      571 2023-05-15 07:30:18.000000 pynocaptcha-1.5.0/pynocaptcha/__init__.py
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-05-15 07:35:54.000000 pynocaptcha-1.5.0/pynocaptcha/crackers/
--rw-r--r--   0 esbiya     (501) staff       (20)      961 2023-05-08 09:19:50.000000 pynocaptcha-1.5.0/pynocaptcha/crackers/akamai.py
--rw-r--r--   0 esbiya     (501) staff       (20)     4577 2023-05-11 08:54:40.000000 pynocaptcha-1.5.0/pynocaptcha/crackers/base.py
--rw-r--r--   0 esbiya     (501) staff       (20)     5186 2023-04-23 09:01:32.000000 pynocaptcha-1.5.0/pynocaptcha/crackers/cloudflare.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1339 2023-04-05 02:45:58.000000 pynocaptcha-1.5.0/pynocaptcha/crackers/hcaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)     2108 2023-05-15 07:32:09.000000 pynocaptcha-1.5.0/pynocaptcha/crackers/incapsula.py
--rw-r--r--   0 esbiya     (501) staff       (20)     2449 2023-04-23 08:59:52.000000 pynocaptcha-1.5.0/pynocaptcha/crackers/recaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)      846 2023-05-15 07:32:23.000000 pynocaptcha-1.5.0/setup.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-06-06 02:58:09.000000 pynocaptcha-1.5.1/
+-rw-r--r--   0 esbiya     (501) staff       (20)      566 2023-06-06 02:58:09.000000 pynocaptcha-1.5.1/PKG-INFO
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-06-06 02:58:09.000000 pynocaptcha-1.5.1/pynocaptcha/
+-rw-r--r--   0 esbiya     (501) staff       (20)      571 2023-05-15 07:30:18.000000 pynocaptcha-1.5.1/pynocaptcha/__init__.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-06-06 02:58:09.000000 pynocaptcha-1.5.1/pynocaptcha/crackers/
+-rw-r--r--   0 esbiya     (501) staff       (20)     1016 2023-06-06 02:53:27.000000 pynocaptcha-1.5.1/pynocaptcha/crackers/akamai.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     4715 2023-06-06 02:54:14.000000 pynocaptcha-1.5.1/pynocaptcha/crackers/base.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     5186 2023-04-23 09:01:32.000000 pynocaptcha-1.5.1/pynocaptcha/crackers/cloudflare.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1339 2023-04-05 02:45:58.000000 pynocaptcha-1.5.1/pynocaptcha/crackers/hcaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     2108 2023-05-15 07:32:09.000000 pynocaptcha-1.5.1/pynocaptcha/crackers/incapsula.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     2449 2023-04-23 08:59:52.000000 pynocaptcha-1.5.1/pynocaptcha/crackers/recaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)      846 2023-06-06 02:43:43.000000 pynocaptcha-1.5.1/setup.py
```

### Comparing `pynocaptcha-1.5.0/PKG-INFO` & `pynocaptcha-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pynocaptcha
-Version: 1.5.0
+Version: 1.5.1
 Summary: nocaptcha.io api
 Home-page: UNKNOWN
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: MIT
 Description: nocaptcha.io python api
 Keywords: nocaptcha
```

### Comparing `pynocaptcha-1.5.0/pynocaptcha/__init__.py` & `pynocaptcha-1.5.1/pynocaptcha/__init__.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.5.0/pynocaptcha/crackers/akamai.py` & `pynocaptcha-1.5.1/pynocaptcha/crackers/akamai.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     cracker_version = "v2"    
 
     """
     recaptcha universal cracker
     :param href: 触发验证的页面地址
     :param api: akamai 提交 sensor_data 的地址
     :param telemetry: 是否 headers 中的 telemetry 参数验证形式, 默认 false
-    :param _abck: 请求 href 首页返回的 cookie _abck 值, 传了 api 参数必须传该值
-    :param bm_sz: 请求 href 首页返回的 cookie bm_sz 值, 传了 api 参数必须传该值
+    :param cookies: 请求 href 首页返回的 cookie _abck, bm_sz 值, 传了 api 参数必须传该值, 示例: { "value": "_abck=xxx; bm_sz=xxx", "uri": "https://example.com" }
+    :param device: 请求流程使用的设备类型, 可选 pc/mobile, 默认 mobile
     调用示例:
     cracker = AkamaiV2Cracker(
         user_token="xxx",
         href="xxx",
         api="xxx",
         
         # debug=True,
@@ -28,10 +28,9 @@
     
     # 必传参数
     must_check_params = ["href"]
     # 默认可选参数
     option_params = {
         "api": "",
         "telemetry": False,
-        "_abck": None,
-        "bm_sz": None
+        "device": "mobile"
     }
```

### Comparing `pynocaptcha-1.5.0/pynocaptcha/crackers/base.py` & `pynocaptcha-1.5.1/pynocaptcha/crackers/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     delete_params = []
     
     def __init__(
         self,    
         user_token: str = None,
         developer_id: str = None,   
         user_agent: str = None,
+        cookies: dict = {},
         proxy: str = None, 
         timeout: int = 30,
         debug: bool = False,
         check_useful: bool = False,
         max_retry_times: int = 3,
         internal=True,
         internal_api=True,
@@ -50,14 +51,15 @@
         if show_ad:
             logger.debug("感谢选择 nocaptcha, 我们只做别人做不到的(手动狗头)~")
             logger.debug("欢迎推荐注册, 官网地址: https://www.nocaptcha.io/")
         self.user_token = user_token
         if not self.user_token:
             raise Exception("缺少用户凭证")
         self.developer_id = developer_id
+        self.cookies = cookies
         self.user_agent = user_agent
         self.proxy = proxy
         self.timeout = timeout
         self.debug = debug
         self.check_useful = check_useful
         self.max_retry_times = max_retry_times
 
@@ -94,14 +96,16 @@
             "User-Token": self.user_token
         }
         if self.developer_id:
             headers["Developer-Id"] = self.developer_id
         
         if self.user_agent:
             self.wanda_args["user_agent"] = self.user_agent
+        if self.cookies:
+            self.wanda_args["cookies"] = self.cookies
         if self.proxy:
             self.wanda_args["proxy"] = self.proxy
 
         retry_times = 0        
         resp = {}
         while retry_times < self.max_retry_times:
             try:
```

### Comparing `pynocaptcha-1.5.0/pynocaptcha/crackers/cloudflare.py` & `pynocaptcha-1.5.1/pynocaptcha/crackers/cloudflare.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.5.0/pynocaptcha/crackers/hcaptcha.py` & `pynocaptcha-1.5.1/pynocaptcha/crackers/hcaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.5.0/pynocaptcha/crackers/incapsula.py` & `pynocaptcha-1.5.1/pynocaptcha/crackers/incapsula.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.5.0/pynocaptcha/crackers/recaptcha.py` & `pynocaptcha-1.5.1/pynocaptcha/crackers/recaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.5.0/setup.py` & `pynocaptcha-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 
 
 setup(
     name='pynocaptcha',
-    version='1.5.0',
+    version='1.5.1',
     description='nocaptcha.io api',
     long_description='nocaptcha.io python api',
     install_requires=["pyhttpx", "loguru"],
     license='MIT',
     packages=["pynocaptcha/crackers", "pynocaptcha"],
     package_dir={'pynocaptcha': 'pynocaptcha'},
     platforms=["all"],
```

