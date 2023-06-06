# Comparing `tmp/tencentcloud-sdk-python-batch-3.0.906.tar.gz` & `tmp/tencentcloud-sdk-python-batch-3.0.907.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-batch-3.0.906.tar", last modified: Mon Jun  5 00:26:55 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-batch-3.0.907.tar", last modified: Tue Jun  6 02:19:04 2023, max compression
```

## Comparing `tencentcloud-sdk-python-batch-3.0.906.tar` & `tencentcloud-sdk-python-batch-3.0.907.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/
--rw-r--r--   0 root         (0) root         (0)      743 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/tencentcloud/batch/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/tencentcloud/batch/v20170312/
--rw-r--r--   0 root         (0) root         (0)     8555 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/tencentcloud/batch/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/tencentcloud/batch/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   194613 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/tencentcloud/batch/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)    31537 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/tencentcloud/batch/v20170312/batch_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/tencentcloud/batch/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/tencentcloud_sdk_python_batch.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/tencentcloud_sdk_python_batch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/tencentcloud_sdk_python_batch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/tencentcloud_sdk_python_batch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/tencentcloud_sdk_python_batch.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1010 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:19:04.000000 tencentcloud-sdk-python-batch-3.0.907/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-06-06 02:19:04.000000 tencentcloud-sdk-python-batch-3.0.907/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:19:04.000000 tencentcloud-sdk-python-batch-3.0.907/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:19:04.000000 tencentcloud-sdk-python-batch-3.0.907/tencentcloud/batch/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:19:04.000000 tencentcloud-sdk-python-batch-3.0.907/tencentcloud/batch/v20170312/
+-rw-r--r--   0 root         (0) root         (0)     8635 2023-06-06 02:19:04.000000 tencentcloud-sdk-python-batch-3.0.907/tencentcloud/batch/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:19:04.000000 tencentcloud-sdk-python-batch-3.0.907/tencentcloud/batch/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   194613 2023-06-06 02:19:04.000000 tencentcloud-sdk-python-batch-3.0.907/tencentcloud/batch/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)    31537 2023-06-06 02:19:04.000000 tencentcloud-sdk-python-batch-3.0.907/tencentcloud/batch/v20170312/batch_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:19:04.000000 tencentcloud-sdk-python-batch-3.0.907/tencentcloud/batch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:19:04.000000 tencentcloud-sdk-python-batch-3.0.907/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-06 02:19:04.000000 tencentcloud-sdk-python-batch-3.0.907/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:19:04.000000 tencentcloud-sdk-python-batch-3.0.907/tencentcloud_sdk_python_batch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:19:04.000000 tencentcloud-sdk-python-batch-3.0.907/tencentcloud_sdk_python_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-06-06 02:19:04.000000 tencentcloud-sdk-python-batch-3.0.907/tencentcloud_sdk_python_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-06 02:19:04.000000 tencentcloud-sdk-python-batch-3.0.907/tencentcloud_sdk_python_batch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:19:04.000000 tencentcloud-sdk-python-batch-3.0.907/tencentcloud_sdk_python_batch.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-06-06 02:19:04.000000 tencentcloud-sdk-python-batch-3.0.907/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:19:04.000000 tencentcloud-sdk-python-batch-3.0.907/setup.cfg
```

### Comparing `tencentcloud-sdk-python-batch-3.0.906/README.rst` & `tencentcloud-sdk-python-batch-3.0.907/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-batch-3.0.906/tencentcloud/batch/v20170312/errorcodes.py` & `tencentcloud-sdk-python-batch-3.0.907/tencentcloud/batch/v20170312/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 
 # ComputeEnv 和 EnvId 必须指定一个（且只有一个）参数。
 ALLOWEDONEATTRIBUTEINENVIDANDCOMPUTEENV = 'AllowedOneAttributeInEnvIdAndComputeEnv'
 
 # 内部错误。
 INTERNALERROR = 'InternalError'
 
+# 调用CAM API返回错误。
+INTERNALERROR_CALLCAM = 'InternalError.CallCam'
+
 # 调用Cpm API返回错误。
 INTERNALERROR_CALLCPMAPI = 'InternalError.CallCpmAPI'
 
 # 调用CVM API返回错误。
 INTERNALERROR_CALLCVM = 'InternalError.CallCvm'
 
 # 获取Tag错误。
```

### Comparing `tencentcloud-sdk-python-batch-3.0.906/tencentcloud/batch/v20170312/models.py` & `tencentcloud-sdk-python-batch-3.0.907/tencentcloud/batch/v20170312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-batch-3.0.906/tencentcloud/batch/v20170312/batch_client.py` & `tencentcloud-sdk-python-batch-3.0.907/tencentcloud/batch/v20170312/batch_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-batch-3.0.906/tencentcloud/__init__.py` & `tencentcloud-sdk-python-batch-3.0.907/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-batch-3.0.906/PKG-INFO` & `tencentcloud-sdk-python-batch-3.0.907/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-batch
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Batch SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-batch-3.0.906/tencentcloud_sdk_python_batch.egg-info/PKG-INFO` & `tencentcloud-sdk-python-batch-3.0.907/tencentcloud_sdk_python_batch.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-batch
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Batch SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-batch-3.0.906/setup.py` & `tencentcloud-sdk-python-batch-3.0.907/setup.py`

 * *Files identical despite different names*

