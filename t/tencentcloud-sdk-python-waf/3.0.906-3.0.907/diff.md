# Comparing `tmp/tencentcloud-sdk-python-waf-3.0.906.tar.gz` & `tmp/tencentcloud-sdk-python-waf-3.0.907.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.906.tar", last modified: Mon Jun  5 00:46:44 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.907.tar", last modified: Tue Jun  6 02:39:21 2023, max compression
```

## Comparing `tencentcloud-sdk-python-waf-3.0.906.tar` & `tencentcloud-sdk-python-waf-3.0.907.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:46:44.000000 tencentcloud-sdk-python-waf-3.0.906/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-05 00:46:44.000000 tencentcloud-sdk-python-waf-3.0.906/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:46:44.000000 tencentcloud-sdk-python-waf-3.0.906/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:46:44.000000 tencentcloud-sdk-python-waf-3.0.906/tencentcloud/waf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:46:44.000000 tencentcloud-sdk-python-waf-3.0.906/tencentcloud/waf/v20180125/
--rw-r--r--   0 root         (0) root         (0)    46563 2023-06-05 00:46:44.000000 tencentcloud-sdk-python-waf-3.0.906/tencentcloud/waf/v20180125/waf_client.py
--rw-r--r--   0 root         (0) root         (0)     2513 2023-06-05 00:46:44.000000 tencentcloud-sdk-python-waf-3.0.906/tencentcloud/waf/v20180125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:46:44.000000 tencentcloud-sdk-python-waf-3.0.906/tencentcloud/waf/v20180125/__init__.py
--rw-r--r--   0 root         (0) root         (0)   180770 2023-06-05 00:46:44.000000 tencentcloud-sdk-python-waf-3.0.906/tencentcloud/waf/v20180125/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:46:44.000000 tencentcloud-sdk-python-waf-3.0.906/tencentcloud/waf/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-05 00:46:44.000000 tencentcloud-sdk-python-waf-3.0.906/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-05 00:46:44.000000 tencentcloud-sdk-python-waf-3.0.906/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-05 00:46:44.000000 tencentcloud-sdk-python-waf-3.0.906/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-05 00:46:44.000000 tencentcloud-sdk-python-waf-3.0.906/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:46:44.000000 tencentcloud-sdk-python-waf-3.0.906/tencentcloud_sdk_python_waf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:46:44.000000 tencentcloud-sdk-python-waf-3.0.906/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-05 00:46:44.000000 tencentcloud-sdk-python-waf-3.0.906/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-05 00:46:44.000000 tencentcloud-sdk-python-waf-3.0.906/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 00:46:44.000000 tencentcloud-sdk-python-waf-3.0.906/tencentcloud_sdk_python_waf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/tencentcloud/waf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/tencentcloud/waf/v20180125/
+-rw-r--r--   0 root         (0) root         (0)    46563 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/tencentcloud/waf/v20180125/waf_client.py
+-rw-r--r--   0 root         (0) root         (0)     2711 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/tencentcloud/waf/v20180125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/tencentcloud/waf/v20180125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   180770 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/tencentcloud/waf/v20180125/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/tencentcloud/waf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/tencentcloud_sdk_python_waf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/tencentcloud_sdk_python_waf.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-waf-3.0.906/README.rst` & `tencentcloud-sdk-python-waf-3.0.907/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.906/tencentcloud/waf/v20180125/waf_client.py` & `tencentcloud-sdk-python-waf-3.0.907/tencentcloud/waf/v20180125/waf_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.906/tencentcloud/waf/v20180125/errorcodes.py` & `tencentcloud-sdk-python-waf-3.0.907/tencentcloud/waf/v20180125/errorcodes.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 
 # DryRun 操作，代表请求将会是成功的，只是多传了 DryRun 参数。
 DRYRUNOPERATION = 'DryRunOperation'
 
 # 操作失败。
 FAILEDOPERATION = 'FailedOperation'
 
+# 调用CLS日志服务API失败
+FAILEDOPERATION_CLSDBOPERATIONFAILED = 'FailedOperation.CLSDBOperationFailed'
+
 # CLS内部错误。
 FAILEDOPERATION_CLSINTERNALERROR = 'FailedOperation.CLSInternalError'
 
 # 操作Mysql数据库失败
 FAILEDOPERATION_MYSQLDBOPERATIONFAILED = 'FailedOperation.MysqlDBOperationFailed'
 
 # 操作Redis数据库失败
@@ -49,14 +52,17 @@
 
 # 参数取值错误。
 INVALIDPARAMETERVALUE = 'InvalidParameterValue'
 
 # 超过配额限制。
 LIMITEXCEEDED = 'LimitExceeded'
 
+# SpecificationErr
+LIMITEXCEEDED_SPECIFICATIONERR = 'LimitExceeded.SpecificationErr'
+
 # 缺少参数错误。
 MISSINGPARAMETER = 'MissingParameter'
 
 # 操作被拒绝。
 OPERATIONDENIED = 'OperationDenied'
 
 # 请求的次数超过了频率限制。
```

### Comparing `tencentcloud-sdk-python-waf-3.0.906/tencentcloud/waf/v20180125/models.py` & `tencentcloud-sdk-python-waf-3.0.907/tencentcloud/waf/v20180125/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.906/tencentcloud/__init__.py` & `tencentcloud-sdk-python-waf-3.0.907/tencentcloud/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.906'
+__version__ = '3.0.907'
```

### Comparing `tencentcloud-sdk-python-waf-3.0.906/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.907/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-waf-3.0.906/setup.py` & `tencentcloud-sdk-python-waf-3.0.907/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.906/tencentcloud_sdk_python_waf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.907/tencentcloud_sdk_python_waf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

