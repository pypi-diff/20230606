# Comparing `tmp/tencentcloud-sdk-python-live-3.0.906.tar.gz` & `tmp/tencentcloud-sdk-python-live-3.0.907.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.906.tar", last modified: Mon Jun  5 00:37:44 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.907.tar", last modified: Tue Jun  6 02:29:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-live-3.0.906.tar` & `tencentcloud-sdk-python-live-3.0.907.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:37:44.000000 tencentcloud-sdk-python-live-3.0.906/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:37:44.000000 tencentcloud-sdk-python-live-3.0.906/tencentcloud_sdk_python_live.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:37:44.000000 tencentcloud-sdk-python-live-3.0.906/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-05 00:37:44.000000 tencentcloud-sdk-python-live-3.0.906/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-05 00:37:44.000000 tencentcloud-sdk-python-live-3.0.906/tencentcloud_sdk_python_live.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 00:37:44.000000 tencentcloud-sdk-python-live-3.0.906/tencentcloud_sdk_python_live.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-05 00:37:44.000000 tencentcloud-sdk-python-live-3.0.906/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:37:44.000000 tencentcloud-sdk-python-live-3.0.906/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:37:44.000000 tencentcloud-sdk-python-live-3.0.906/tencentcloud/live/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:37:44.000000 tencentcloud-sdk-python-live-3.0.906/tencentcloud/live/v20180801/
--rw-r--r--   0 root         (0) root         (0)   137451 2023-06-05 00:37:44.000000 tencentcloud-sdk-python-live-3.0.906/tencentcloud/live/v20180801/live_client.py
--rw-r--r--   0 root         (0) root         (0)    18117 2023-06-05 00:37:44.000000 tencentcloud-sdk-python-live-3.0.906/tencentcloud/live/v20180801/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:37:44.000000 tencentcloud-sdk-python-live-3.0.906/tencentcloud/live/v20180801/__init__.py
--rw-r--r--   0 root         (0) root         (0)   433012 2023-06-05 00:37:44.000000 tencentcloud-sdk-python-live-3.0.906/tencentcloud/live/v20180801/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:37:44.000000 tencentcloud-sdk-python-live-3.0.906/tencentcloud/live/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-05 00:37:44.000000 tencentcloud-sdk-python-live-3.0.906/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-05 00:37:44.000000 tencentcloud-sdk-python-live-3.0.906/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-05 00:37:44.000000 tencentcloud-sdk-python-live-3.0.906/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-05 00:37:44.000000 tencentcloud-sdk-python-live-3.0.906/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/tencentcloud_sdk_python_live.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/tencentcloud_sdk_python_live.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/tencentcloud_sdk_python_live.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/tencentcloud/live/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/tencentcloud/live/v20180801/
+-rw-r--r--   0 root         (0) root         (0)   137451 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/tencentcloud/live/v20180801/live_client.py
+-rw-r--r--   0 root         (0) root         (0)    18487 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/tencentcloud/live/v20180801/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/tencentcloud/live/v20180801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   433012 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/tencentcloud/live/v20180801/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/tencentcloud/live/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/setup.cfg
```

### Comparing `tencentcloud-sdk-python-live-3.0.906/tencentcloud_sdk_python_live.egg-info/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.907/tencentcloud_sdk_python_live.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.906/README.rst` & `tencentcloud-sdk-python-live-3.0.907/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.906/tencentcloud/live/v20180801/live_client.py` & `tencentcloud-sdk-python-live-3.0.907/tencentcloud/live/v20180801/live_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.906/tencentcloud/live/v20180801/errorcodes.py` & `tencentcloud-sdk-python-live-3.0.907/tencentcloud/live/v20180801/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -322,14 +322,20 @@
 
 # 腾讯云证书托管 ID 错误。
 INVALIDPARAMETER_CLOUDCRTIDERROR = 'InvalidParameter.CloudCrtIdError'
 
 # 赠送的腾讯云域名已过期。
 INVALIDPARAMETER_CLOUDDOMAINISSTOP = 'InvalidParameter.CloudDomainIsStop'
 
+# 模版使用中。
+INVALIDPARAMETER_CONFINUSED = 'InvalidParameter.ConfInUsed'
+
+# 配置没有找到。
+INVALIDPARAMETER_CONFNOTFOUND = 'InvalidParameter.ConfNotFound'
+
 # 证书使用中。
 INVALIDPARAMETER_CRTDATEINUSING = 'InvalidParameter.CrtDateInUsing'
 
 # 证书不存在。
 INVALIDPARAMETER_CRTDATENOTFOUND = 'InvalidParameter.CrtDateNotFound'
 
 # 证书内容不合法。
@@ -418,14 +424,20 @@
 
 # 小程序插件没有授权。
 INVALIDPARAMETER_MPPLUGINNOUSE = 'InvalidParameter.MpPluginNoUse'
 
 # 其他错误。
 INVALIDPARAMETER_OTHERERROR = 'InvalidParameter.OtherError'
 
+# 转码模板已存在。
+INVALIDPARAMETER_PROCESSORALREADYEXIST = 'InvalidParameter.ProcessorAlreadyExist'
+
+# 规则没有找到。
+INVALIDPARAMETER_RULENOTFOUND = 'InvalidParameter.RuleNotFound'
+
 # 同一会话输出流发生变化。
 INVALIDPARAMETER_SESSIONOUTPUTSTREAMCHANGED = 'InvalidParameter.SessionOutputStreamChanged'
 
 # 任务不存在。
 INVALIDPARAMETER_TASKNOTEXIST = 'InvalidParameter.TaskNotExist'
 
 # 任务数超过限制。
```

### Comparing `tencentcloud-sdk-python-live-3.0.906/tencentcloud/live/v20180801/models.py` & `tencentcloud-sdk-python-live-3.0.907/tencentcloud/live/v20180801/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.906/tencentcloud/__init__.py` & `tencentcloud-sdk-python-live-3.0.907/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-live-3.0.906/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.907/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.906/setup.py` & `tencentcloud-sdk-python-live-3.0.907/setup.py`

 * *Files identical despite different names*

