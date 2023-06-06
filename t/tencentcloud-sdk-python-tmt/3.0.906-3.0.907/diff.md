# Comparing `tmp/tencentcloud-sdk-python-tmt-3.0.906.tar.gz` & `tmp/tencentcloud-sdk-python-tmt-3.0.907.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tmt-3.0.906.tar", last modified: Mon Jun  5 00:45:09 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tmt-3.0.907.tar", last modified: Tue Jun  6 02:37:54 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tmt-3.0.906.tar` & `tencentcloud-sdk-python-tmt-3.0.907.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:45:09.000000 tencentcloud-sdk-python-tmt-3.0.906/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-05 00:45:08.000000 tencentcloud-sdk-python-tmt-3.0.906/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:45:09.000000 tencentcloud-sdk-python-tmt-3.0.906/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-05 00:45:08.000000 tencentcloud-sdk-python-tmt-3.0.906/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:45:09.000000 tencentcloud-sdk-python-tmt-3.0.906/tencentcloud/tmt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:45:09.000000 tencentcloud-sdk-python-tmt-3.0.906/tencentcloud/tmt/v20180321/
--rw-r--r--   0 root         (0) root         (0)     3545 2023-06-05 00:45:08.000000 tencentcloud-sdk-python-tmt-3.0.906/tencentcloud/tmt/v20180321/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:45:08.000000 tencentcloud-sdk-python-tmt-3.0.906/tencentcloud/tmt/v20180321/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9401 2023-06-05 00:45:08.000000 tencentcloud-sdk-python-tmt-3.0.906/tencentcloud/tmt/v20180321/tmt_client.py
--rw-r--r--   0 root         (0) root         (0)    33942 2023-06-05 00:45:08.000000 tencentcloud-sdk-python-tmt-3.0.906/tencentcloud/tmt/v20180321/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:45:08.000000 tencentcloud-sdk-python-tmt-3.0.906/tencentcloud/tmt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:45:09.000000 tencentcloud-sdk-python-tmt-3.0.906/tencentcloud_sdk_python_tmt.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:45:09.000000 tencentcloud-sdk-python-tmt-3.0.906/tencentcloud_sdk_python_tmt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-05 00:45:09.000000 tencentcloud-sdk-python-tmt-3.0.906/tencentcloud_sdk_python_tmt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-05 00:45:09.000000 tencentcloud-sdk-python-tmt-3.0.906/tencentcloud_sdk_python_tmt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 00:45:09.000000 tencentcloud-sdk-python-tmt-3.0.906/tencentcloud_sdk_python_tmt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-05 00:45:09.000000 tencentcloud-sdk-python-tmt-3.0.906/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-05 00:45:08.000000 tencentcloud-sdk-python-tmt-3.0.906/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-05 00:45:09.000000 tencentcloud-sdk-python-tmt-3.0.906/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:37:54.000000 tencentcloud-sdk-python-tmt-3.0.907/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-06 02:37:54.000000 tencentcloud-sdk-python-tmt-3.0.907/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:37:54.000000 tencentcloud-sdk-python-tmt-3.0.907/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:37:54.000000 tencentcloud-sdk-python-tmt-3.0.907/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:37:54.000000 tencentcloud-sdk-python-tmt-3.0.907/tencentcloud/tmt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:37:54.000000 tencentcloud-sdk-python-tmt-3.0.907/tencentcloud/tmt/v20180321/
+-rw-r--r--   0 root         (0) root         (0)     3623 2023-06-06 02:37:54.000000 tencentcloud-sdk-python-tmt-3.0.907/tencentcloud/tmt/v20180321/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:37:54.000000 tencentcloud-sdk-python-tmt-3.0.907/tencentcloud/tmt/v20180321/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9401 2023-06-06 02:37:54.000000 tencentcloud-sdk-python-tmt-3.0.907/tencentcloud/tmt/v20180321/tmt_client.py
+-rw-r--r--   0 root         (0) root         (0)    33942 2023-06-06 02:37:54.000000 tencentcloud-sdk-python-tmt-3.0.907/tencentcloud/tmt/v20180321/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:37:54.000000 tencentcloud-sdk-python-tmt-3.0.907/tencentcloud/tmt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:37:54.000000 tencentcloud-sdk-python-tmt-3.0.907/tencentcloud_sdk_python_tmt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:37:54.000000 tencentcloud-sdk-python-tmt-3.0.907/tencentcloud_sdk_python_tmt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-06 02:37:54.000000 tencentcloud-sdk-python-tmt-3.0.907/tencentcloud_sdk_python_tmt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-06 02:37:54.000000 tencentcloud-sdk-python-tmt-3.0.907/tencentcloud_sdk_python_tmt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:37:54.000000 tencentcloud-sdk-python-tmt-3.0.907/tencentcloud_sdk_python_tmt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-06 02:37:54.000000 tencentcloud-sdk-python-tmt-3.0.907/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-06 02:37:54.000000 tencentcloud-sdk-python-tmt-3.0.907/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:37:54.000000 tencentcloud-sdk-python-tmt-3.0.907/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tmt-3.0.906/README.rst` & `tencentcloud-sdk-python-tmt-3.0.907/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tmt-3.0.906/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tmt-3.0.907/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tmt-3.0.906/tencentcloud/tmt/v20180321/errorcodes.py` & `tencentcloud-sdk-python-tmt-3.0.907/tencentcloud/tmt/v20180321/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 
 # 内部请求错误。
 FAILEDOPERATION_REQUESTAILABERR = 'FailedOperation.RequestAiLabErr'
 
 # 账号因为欠费停止服务，请在腾讯云账户充值。
 FAILEDOPERATION_SERVICEISOLATE = 'FailedOperation.ServiceIsolate'
 
+# 帐号已停服。
+FAILEDOPERATION_STOPUSING = 'FailedOperation.StopUsing'
+
 # 服务未开通，请在腾讯云官网机器翻译控制台开通服务。
 FAILEDOPERATION_USERNOTREGISTERED = 'FailedOperation.UserNotRegistered'
 
 # 内部错误。
 INTERNALERROR = 'InternalError'
 
 # 后台服务超时，请稍后重试。
```

### Comparing `tencentcloud-sdk-python-tmt-3.0.906/tencentcloud/tmt/v20180321/tmt_client.py` & `tencentcloud-sdk-python-tmt-3.0.907/tencentcloud/tmt/v20180321/tmt_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tmt-3.0.906/tencentcloud/tmt/v20180321/models.py` & `tencentcloud-sdk-python-tmt-3.0.907/tencentcloud/tmt/v20180321/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tmt-3.0.906/tencentcloud_sdk_python_tmt.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tmt-3.0.907/tencentcloud_sdk_python_tmt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tmt
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Tmt SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tmt-3.0.906/PKG-INFO` & `tencentcloud-sdk-python-tmt-3.0.907/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tmt
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Tmt SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tmt-3.0.906/setup.py` & `tencentcloud-sdk-python-tmt-3.0.907/setup.py`

 * *Files identical despite different names*

