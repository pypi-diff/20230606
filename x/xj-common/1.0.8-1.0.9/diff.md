# Comparing `tmp/xj_common-1.0.8.tar.gz` & `tmp/xj_common-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xj_common-1.0.8.tar", last modified: Fri Mar  3 03:10:59 2023, max compression
+gzip compressed data, was "dist\xj_common-1.0.9.tar", last modified: Mon Mar  6 04:10:45 2023, max compression
```

## Comparing `xj_common-1.0.8.tar` & `xj_common-1.0.9.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-03-03 03:10:59.000000 xj_common-1.0.8/
--rw-rw-rw-   0        0        0     1969 2023-03-03 03:10:59.000000 xj_common-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1354 2022-09-17 04:50:11.000000 xj_common-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-03-03 03:10:59.000000 xj_common-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      893 2023-03-03 03:10:52.000000 xj_common-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-03 03:10:59.000000 xj_common-1.0.8/xj_common/
--rw-rw-rw-   0        0        0        0 2022-09-17 04:50:11.000000 xj_common-1.0.8/xj_common/__init__.py
--rw-rw-rw-   0        0        0     1359 2023-03-01 03:03:35.000000 xj_common-1.0.8/xj_common/admin.py
-drwxrwxrwx   0        0        0        0 2023-03-03 03:10:59.000000 xj_common-1.0.8/xj_common/apis/
--rw-rw-rw-   0        0        0      149 2022-12-15 05:06:00.000000 xj_common-1.0.8/xj_common/apis/__init__.py
--rw-rw-rw-   0        0        0     2296 2023-03-01 08:25:09.000000 xj_common-1.0.8/xj_common/apis/notice_apis.py
--rw-rw-rw-   0        0        0     2436 2022-12-15 06:30:59.000000 xj_common-1.0.8/xj_common/apis/region_api.py
--rw-rw-rw-   0        0        0     2132 2022-11-29 06:32:59.000000 xj_common-1.0.8/xj_common/apis/translate_apis.py
--rw-rw-rw-   0        0        0      190 2022-12-06 03:25:30.000000 xj_common-1.0.8/xj_common/apps.py
--rw-rw-rw-   0        0        0     3252 2023-03-01 08:34:54.000000 xj_common-1.0.8/xj_common/models.py
--rw-rw-rw-   0        0        0      716 2023-03-01 09:12:43.000000 xj_common-1.0.8/xj_common/service_register.py
-drwxrwxrwx   0        0        0        0 2023-03-03 03:10:59.000000 xj_common-1.0.8/xj_common/services/
--rw-rw-rw-   0        0        0      162 2022-07-06 10:14:59.000000 xj_common-1.0.8/xj_common/services/__init__.py
--rw-rw-rw-   0        0        0     7859 2023-03-01 09:18:56.000000 xj_common-1.0.8/xj_common/services/notice_services.py
--rw-rw-rw-   0        0        0     4101 2022-12-15 06:31:01.000000 xj_common-1.0.8/xj_common/services/regin_service.py
--rw-rw-rw-   0        0        0     5303 2022-11-29 06:32:59.000000 xj_common-1.0.8/xj_common/services/translate_server.py
--rw-rw-rw-   0        0        0     1093 2023-03-01 08:31:41.000000 xj_common-1.0.8/xj_common/urls.py
-drwxrwxrwx   0        0        0        0 2023-03-03 03:10:59.000000 xj_common-1.0.8/xj_common/utils/
--rw-rw-rw-   0        0        0      148 2022-11-29 06:32:59.000000 xj_common-1.0.8/xj_common/utils/__init__.py
--rw-rw-rw-   0        0        0     1345 2022-11-29 06:32:59.000000 xj_common-1.0.8/xj_common/utils/custom_response.py
--rw-rw-rw-   0        0        0    15530 2023-03-03 03:08:46.000000 xj_common-1.0.8/xj_common/utils/custom_tool.py
--rw-rw-rw-   0        0        0      429 2022-11-29 06:32:59.000000 xj_common-1.0.8/xj_common/utils/j_dict.py
--rw-rw-rw-   0        0        0     7650 2022-11-29 06:32:59.000000 xj_common-1.0.8/xj_common/utils/j_valuation.py
--rw-rw-rw-   0        0        0      660 2022-11-29 06:32:59.000000 xj_common-1.0.8/xj_common/utils/join_list.py
--rw-rw-rw-   0        0        0     2932 2022-11-29 06:32:59.000000 xj_common-1.0.8/xj_common/utils/validator.py
--rw-rw-rw-   0        0        0     1379 2022-07-06 10:14:59.000000 xj_common-1.0.8/xj_common/validate.py
-drwxrwxrwx   0        0        0        0 2023-03-03 03:10:59.000000 xj_common-1.0.8/xj_common.egg-info/
--rw-rw-rw-   0        0        0     1969 2023-03-03 03:10:58.000000 xj_common-1.0.8/xj_common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      771 2023-03-03 03:10:58.000000 xj_common-1.0.8/xj_common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-03 03:10:58.000000 xj_common-1.0.8/xj_common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-03-03 03:10:58.000000 xj_common-1.0.8/xj_common.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-03-06 04:10:45.000000 xj_common-1.0.9/
+-rw-rw-rw-   0        0        0     1969 2023-03-06 04:10:45.000000 xj_common-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1354 2022-09-17 04:50:11.000000 xj_common-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-03-06 04:10:45.000000 xj_common-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      893 2023-03-06 04:08:48.000000 xj_common-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-06 04:10:45.000000 xj_common-1.0.9/xj_common/
+-rw-rw-rw-   0        0        0        0 2022-09-17 04:50:11.000000 xj_common-1.0.9/xj_common/__init__.py
+-rw-rw-rw-   0        0        0     1359 2023-03-01 03:03:35.000000 xj_common-1.0.9/xj_common/admin.py
+drwxrwxrwx   0        0        0        0 2023-03-06 04:10:45.000000 xj_common-1.0.9/xj_common/apis/
+-rw-rw-rw-   0        0        0      149 2022-12-15 05:06:00.000000 xj_common-1.0.9/xj_common/apis/__init__.py
+-rw-rw-rw-   0        0        0     2296 2023-03-01 08:25:09.000000 xj_common-1.0.9/xj_common/apis/notice_apis.py
+-rw-rw-rw-   0        0        0     2436 2022-12-15 06:30:59.000000 xj_common-1.0.9/xj_common/apis/region_api.py
+-rw-rw-rw-   0        0        0     2132 2022-11-29 06:32:59.000000 xj_common-1.0.9/xj_common/apis/translate_apis.py
+-rw-rw-rw-   0        0        0      190 2022-12-06 03:25:30.000000 xj_common-1.0.9/xj_common/apps.py
+-rw-rw-rw-   0        0        0     3252 2023-03-01 08:34:54.000000 xj_common-1.0.9/xj_common/models.py
+-rw-rw-rw-   0        0        0      716 2023-03-01 09:12:43.000000 xj_common-1.0.9/xj_common/service_register.py
+drwxrwxrwx   0        0        0        0 2023-03-06 04:10:45.000000 xj_common-1.0.9/xj_common/services/
+-rw-rw-rw-   0        0        0      162 2022-07-06 10:14:59.000000 xj_common-1.0.9/xj_common/services/__init__.py
+-rw-rw-rw-   0        0        0     7859 2023-03-01 09:18:56.000000 xj_common-1.0.9/xj_common/services/notice_services.py
+-rw-rw-rw-   0        0        0     4101 2022-12-15 06:31:01.000000 xj_common-1.0.9/xj_common/services/regin_service.py
+-rw-rw-rw-   0        0        0     5303 2022-11-29 06:32:59.000000 xj_common-1.0.9/xj_common/services/translate_server.py
+-rw-rw-rw-   0        0        0     1093 2023-03-01 08:31:41.000000 xj_common-1.0.9/xj_common/urls.py
+drwxrwxrwx   0        0        0        0 2023-03-06 04:10:45.000000 xj_common-1.0.9/xj_common/utils/
+-rw-rw-rw-   0        0        0      148 2022-11-29 06:32:59.000000 xj_common-1.0.9/xj_common/utils/__init__.py
+-rw-rw-rw-   0        0        0     1230 2023-03-06 02:51:55.000000 xj_common-1.0.9/xj_common/utils/custom_authorization.py
+-rw-rw-rw-   0        0        0     1345 2022-11-29 06:32:59.000000 xj_common-1.0.9/xj_common/utils/custom_response.py
+-rw-rw-rw-   0        0        0    15709 2023-03-03 07:09:48.000000 xj_common-1.0.9/xj_common/utils/custom_tool.py
+-rw-rw-rw-   0        0        0      429 2022-11-29 06:32:59.000000 xj_common-1.0.9/xj_common/utils/j_dict.py
+-rw-rw-rw-   0        0        0     7650 2022-11-29 06:32:59.000000 xj_common-1.0.9/xj_common/utils/j_valuation.py
+-rw-rw-rw-   0        0        0      660 2022-11-29 06:32:59.000000 xj_common-1.0.9/xj_common/utils/join_list.py
+-rw-rw-rw-   0        0        0     3767 2023-03-06 04:07:51.000000 xj_common-1.0.9/xj_common/utils/user_wrapper.py
+-rw-rw-rw-   0        0        0     2932 2022-11-29 06:32:59.000000 xj_common-1.0.9/xj_common/utils/validator.py
+-rw-rw-rw-   0        0        0     1379 2022-07-06 10:14:59.000000 xj_common-1.0.9/xj_common/validate.py
+drwxrwxrwx   0        0        0        0 2023-03-06 04:10:45.000000 xj_common-1.0.9/xj_common.egg-info/
+-rw-rw-rw-   0        0        0     1969 2023-03-06 04:10:45.000000 xj_common-1.0.9/xj_common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      843 2023-03-06 04:10:45.000000 xj_common-1.0.9/xj_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-06 04:10:45.000000 xj_common-1.0.9/xj_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-03-06 04:10:45.000000 xj_common-1.0.9/xj_common.egg-info/top_level.txt
```

### Comparing `xj_common-1.0.8/PKG-INFO` & `xj_common-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj_common
-Version: 1.0.8
+Version: 1.0.9
 Summary: 公共模块
 Home-page: UNKNOWN
 Author: 赵向明
 Author-email: sky4834@163.com
 Maintainer: 孙楷炎
 Maintainer-email: sky4834@163.com
 License: apache 3.0
```

### Comparing `xj_common-1.0.8/README.md` & `xj_common-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `xj_common-1.0.8/setup.py` & `xj_common-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf8') as fp:
     log_desc = fp.read()
 
 setup(
     name='xj_common',  # 模块名称
-    version='1.0.8',  # 模块版本
+    version='1.0.9',  # 模块版本
     description='公共模块',  # 项目 摘要描述
     long_description=log_desc,  # 项目描述
     long_description_content_type="text/markdown",  # md文件，markdown格式
     author='赵向明',  # 作者
     author_email='sky4834@163.com',  # 作者邮箱
     maintainer="孙楷炎",  # 维护者
     maintainer_email="sky4834@163.com",  # 维护者的邮箱地址
```

### Comparing `xj_common-1.0.8/xj_common/admin.py` & `xj_common-1.0.9/xj_common/admin.py`

 * *Files identical despite different names*

### Comparing `xj_common-1.0.8/xj_common/apis/notice_apis.py` & `xj_common-1.0.9/xj_common/apis/notice_apis.py`

 * *Files identical despite different names*

### Comparing `xj_common-1.0.8/xj_common/apis/region_api.py` & `xj_common-1.0.9/xj_common/apis/region_api.py`

 * *Files identical despite different names*

### Comparing `xj_common-1.0.8/xj_common/apis/translate_apis.py` & `xj_common-1.0.9/xj_common/apis/translate_apis.py`

 * *Files identical despite different names*

### Comparing `xj_common-1.0.8/xj_common/models.py` & `xj_common-1.0.9/xj_common/models.py`

 * *Files identical despite different names*

### Comparing `xj_common-1.0.8/xj_common/service_register.py` & `xj_common-1.0.9/xj_common/service_register.py`

 * *Files identical despite different names*

### Comparing `xj_common-1.0.8/xj_common/services/notice_services.py` & `xj_common-1.0.9/xj_common/services/notice_services.py`

 * *Files identical despite different names*

### Comparing `xj_common-1.0.8/xj_common/services/regin_service.py` & `xj_common-1.0.9/xj_common/services/regin_service.py`

 * *Files identical despite different names*

### Comparing `xj_common-1.0.8/xj_common/services/translate_server.py` & `xj_common-1.0.9/xj_common/services/translate_server.py`

 * *Files identical despite different names*

### Comparing `xj_common-1.0.8/xj_common/urls.py` & `xj_common-1.0.9/xj_common/urls.py`

 * *Files identical despite different names*

### Comparing `xj_common-1.0.8/xj_common/utils/custom_response.py` & `xj_common-1.0.9/xj_common/utils/custom_response.py`

 * *Files identical despite different names*

### Comparing `xj_common-1.0.8/xj_common/utils/custom_tool.py` & `xj_common-1.0.9/xj_common/utils/custom_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,20 +236,21 @@
             request = arg_request
         if request is None:
             return func(instance, request, *args, request=request, request_params={}, **kwargs, )
 
         # 参数解析
         content_type = request.META.get('CONTENT_TYPE', "").split(";")[0]
         method = request.method
-        if content_type == "text/plain" or method == "GET":
+        if content_type == "text/plain" or method == "GET":  # 不指定则默认这种content-type
             try:
                 body = request.body.decode("utf-8")
                 data = json.loads(body)
-            except Exception:
-                data = request.GET
+            except Exception as e:
+                # 允许get请求的query参数传json格式字符串，如：?group_list=["basics","bid-online"]
+                data = parse_json(request.GET.dict())
                 if not data:
                     data = request.POST
                 if not data:
                     data = {}
         elif content_type == "application/json":
             data = json.loads(request.body)
         elif content_type == "multipart/form-data":
```

### Comparing `xj_common-1.0.8/xj_common/utils/j_valuation.py` & `xj_common-1.0.9/xj_common/utils/j_valuation.py`

 * *Files identical despite different names*

### Comparing `xj_common-1.0.8/xj_common/utils/join_list.py` & `xj_common-1.0.9/xj_common/utils/join_list.py`

 * *Files identical despite different names*

### Comparing `xj_common-1.0.8/xj_common/utils/validator.py` & `xj_common-1.0.9/xj_common/utils/validator.py`

 * *Files identical despite different names*

### Comparing `xj_common-1.0.8/xj_common/validate.py` & `xj_common-1.0.9/xj_common/validate.py`

 * *Files identical despite different names*

### Comparing `xj_common-1.0.8/xj_common.egg-info/PKG-INFO` & `xj_common-1.0.9/xj_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj-common
-Version: 1.0.8
+Version: 1.0.9
 Summary: 公共模块
 Home-page: UNKNOWN
 Author: 赵向明
 Author-email: sky4834@163.com
 Maintainer: 孙楷炎
 Maintainer-email: sky4834@163.com
 License: apache 3.0
```

### Comparing `xj_common-1.0.8/xj_common.egg-info/SOURCES.txt` & `xj_common-1.0.9/xj_common.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -16,13 +16,15 @@
 xj_common/apis/region_api.py
 xj_common/apis/translate_apis.py
 xj_common/services/__init__.py
 xj_common/services/notice_services.py
 xj_common/services/regin_service.py
 xj_common/services/translate_server.py
 xj_common/utils/__init__.py
+xj_common/utils/custom_authorization.py
 xj_common/utils/custom_response.py
 xj_common/utils/custom_tool.py
 xj_common/utils/j_dict.py
 xj_common/utils/j_valuation.py
 xj_common/utils/join_list.py
+xj_common/utils/user_wrapper.py
 xj_common/utils/validator.py
```

