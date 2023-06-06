# Comparing `tmp/tencentcloud-sdk-python-cvm-3.0.906.tar.gz` & `tmp/tencentcloud-sdk-python-cvm-3.0.907.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cvm-3.0.906.tar", last modified: Mon Jun  5 00:32:01 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cvm-3.0.907.tar", last modified: Tue Jun  6 02:23:46 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cvm-3.0.906.tar` & `tencentcloud-sdk-python-cvm-3.0.907.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:32:01.000000 tencentcloud-sdk-python-cvm-3.0.906/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-05 00:32:01.000000 tencentcloud-sdk-python-cvm-3.0.906/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:32:01.000000 tencentcloud-sdk-python-cvm-3.0.906/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:32:01.000000 tencentcloud-sdk-python-cvm-3.0.906/tencentcloud/cvm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:32:01.000000 tencentcloud-sdk-python-cvm-3.0.906/tencentcloud/cvm/v20170312/
--rw-r--r--   0 root         (0) root         (0)   119300 2023-06-05 00:32:01.000000 tencentcloud-sdk-python-cvm-3.0.906/tencentcloud/cvm/v20170312/cvm_client.py
--rw-r--r--   0 root         (0) root         (0)    43023 2023-06-05 00:32:01.000000 tencentcloud-sdk-python-cvm-3.0.906/tencentcloud/cvm/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:32:01.000000 tencentcloud-sdk-python-cvm-3.0.906/tencentcloud/cvm/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   430455 2023-06-05 00:32:01.000000 tencentcloud-sdk-python-cvm-3.0.906/tencentcloud/cvm/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:32:01.000000 tencentcloud-sdk-python-cvm-3.0.906/tencentcloud/cvm/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-05 00:32:01.000000 tencentcloud-sdk-python-cvm-3.0.906/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-05 00:32:01.000000 tencentcloud-sdk-python-cvm-3.0.906/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-05 00:32:01.000000 tencentcloud-sdk-python-cvm-3.0.906/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-05 00:32:01.000000 tencentcloud-sdk-python-cvm-3.0.906/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:32:01.000000 tencentcloud-sdk-python-cvm-3.0.906/tencentcloud_sdk_python_cvm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:32:01.000000 tencentcloud-sdk-python-cvm-3.0.906/tencentcloud_sdk_python_cvm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-05 00:32:01.000000 tencentcloud-sdk-python-cvm-3.0.906/tencentcloud_sdk_python_cvm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-05 00:32:01.000000 tencentcloud-sdk-python-cvm-3.0.906/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 00:32:01.000000 tencentcloud-sdk-python-cvm-3.0.906/tencentcloud_sdk_python_cvm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:23:46.000000 tencentcloud-sdk-python-cvm-3.0.907/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-06 02:23:46.000000 tencentcloud-sdk-python-cvm-3.0.907/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:23:46.000000 tencentcloud-sdk-python-cvm-3.0.907/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:23:46.000000 tencentcloud-sdk-python-cvm-3.0.907/tencentcloud/cvm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:23:46.000000 tencentcloud-sdk-python-cvm-3.0.907/tencentcloud/cvm/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   119300 2023-06-06 02:23:46.000000 tencentcloud-sdk-python-cvm-3.0.907/tencentcloud/cvm/v20170312/cvm_client.py
+-rw-r--r--   0 root         (0) root         (0)    43461 2023-06-06 02:23:46.000000 tencentcloud-sdk-python-cvm-3.0.907/tencentcloud/cvm/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:23:46.000000 tencentcloud-sdk-python-cvm-3.0.907/tencentcloud/cvm/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   430455 2023-06-06 02:23:46.000000 tencentcloud-sdk-python-cvm-3.0.907/tencentcloud/cvm/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:23:46.000000 tencentcloud-sdk-python-cvm-3.0.907/tencentcloud/cvm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:23:46.000000 tencentcloud-sdk-python-cvm-3.0.907/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-06 02:23:46.000000 tencentcloud-sdk-python-cvm-3.0.907/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-06 02:23:46.000000 tencentcloud-sdk-python-cvm-3.0.907/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:23:46.000000 tencentcloud-sdk-python-cvm-3.0.907/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:23:46.000000 tencentcloud-sdk-python-cvm-3.0.907/tencentcloud_sdk_python_cvm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:23:46.000000 tencentcloud-sdk-python-cvm-3.0.907/tencentcloud_sdk_python_cvm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-06 02:23:46.000000 tencentcloud-sdk-python-cvm-3.0.907/tencentcloud_sdk_python_cvm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-06 02:23:46.000000 tencentcloud-sdk-python-cvm-3.0.907/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:23:46.000000 tencentcloud-sdk-python-cvm-3.0.907/tencentcloud_sdk_python_cvm.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.906/README.rst` & `tencentcloud-sdk-python-cvm-3.0.907/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.906/tencentcloud/cvm/v20170312/cvm_client.py` & `tencentcloud-sdk-python-cvm-3.0.907/tencentcloud/cvm/v20170312/cvm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.906/tencentcloud/cvm/v20170312/errorcodes.py` & `tencentcloud-sdk-python-cvm-3.0.907/tencentcloud/cvm/v20170312/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,26 +307,32 @@
 
 # 请确认存储桶是否存在。
 INVALIDPARAMETERVALUE_BUCKETNOTFOUND = 'InvalidParameterValue.BucketNotFound'
 
 # CamRoleName不合要求，只允许包含英文字母、数字或者 +=,.@_- 字符。
 INVALIDPARAMETERVALUE_CAMROLENAMEMALFORMED = 'InvalidParameterValue.CamRoleNameMalformed'
 
+# CDH磁盘扩容只支持LOCAL_BASIC和LOCAL_SSD。
+INVALIDPARAMETERVALUE_CDHONLYLOCALDATADISKRESIZE = 'InvalidParameterValue.CdhOnlyLocalDataDiskResize'
+
 # 找不到对应的CHC物理服务器。
 INVALIDPARAMETERVALUE_CHCHOSTSNOTFOUND = 'InvalidParameterValue.ChcHostsNotFound'
 
 # 该CHC未配置任何网络。
 INVALIDPARAMETERVALUE_CHCNETWORKEMPTY = 'InvalidParameterValue.ChcNetworkEmpty'
 
 # SSD云硬盘为数据盘时，购买大小不得小于100GB
 INVALIDPARAMETERVALUE_CLOUDSSDDATADISKSIZETOOSMALL = 'InvalidParameterValue.CloudSsdDataDiskSizeTooSmall'
 
 # 核心计数不合法。
 INVALIDPARAMETERVALUE_CORECOUNTVALUE = 'InvalidParameterValue.CoreCountValue'
 
+# CDC不支持指定的计费模式。
+INVALIDPARAMETERVALUE_DEDICATEDCLUSTERNOTSUPPORTEDCHARGETYPE = 'InvalidParameterValue.DedicatedClusterNotSupportedChargeType'
+
 # 已经存在部署VPC。
 INVALIDPARAMETERVALUE_DEPLOYVPCALREADYEXISTS = 'InvalidParameterValue.DeployVpcAlreadyExists'
 
 # 置放群组ID格式错误。
 INVALIDPARAMETERVALUE_DISASTERRECOVERGROUPIDMALFORMED = 'InvalidParameterValue.DisasterRecoverGroupIdMalformed'
 
 # 参数值重复。
@@ -970,14 +976,17 @@
 
 # 不支持关机不收费特性
 UNSUPPORTEDOPERATION_STOPPEDMODESTOPCHARGING = 'UnsupportedOperation.StoppedModeStopCharging'
 
 # 不支持关机不收费机器做同类型变配操作。
 UNSUPPORTEDOPERATION_STOPPEDMODESTOPCHARGINGSAMEFAMILY = 'UnsupportedOperation.StoppedModeStopChargingSameFamily'
 
+# 请求不支持该类型系统盘。
+UNSUPPORTEDOPERATION_SYSTEMDISKTYPE = 'UnsupportedOperation.SystemDiskType'
+
 # 该机型为包销机型，RenewFlag的值只允许设置为NOTIFY_AND_AUTO_RENEW。
 UNSUPPORTEDOPERATION_UNDERWRITINGINSTANCETYPEONLYSUPPORTAUTORENEW = 'UnsupportedOperation.UnderwritingInstanceTypeOnlySupportAutoRenew'
 
 # 指定机型不支持跨机型调整配置。
 UNSUPPORTEDOPERATION_UNSUPPORTEDCHANGEINSTANCEFAMILY = 'UnsupportedOperation.UnsupportedChangeInstanceFamily'
 
 # 非ARM机型不支持调整到ARM机型。
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.906/tencentcloud/cvm/v20170312/models.py` & `tencentcloud-sdk-python-cvm-3.0.907/tencentcloud/cvm/v20170312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.906/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cvm-3.0.907/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cvm-3.0.906/PKG-INFO` & `tencentcloud-sdk-python-cvm-3.0.907/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cvm
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Cvm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.906/setup.py` & `tencentcloud-sdk-python-cvm-3.0.907/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.906/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cvm-3.0.907/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cvm
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Cvm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

