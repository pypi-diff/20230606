# Comparing `tmp/tencentcloud-sdk-python-lighthouse-3.0.906.tar.gz` & `tmp/tencentcloud-sdk-python-lighthouse-3.0.907.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.906.tar", last modified: Mon Jun  5 00:37:38 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.907.tar", last modified: Tue Jun  6 02:29:48 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lighthouse-3.0.906.tar` & `tencentcloud-sdk-python-lighthouse-3.0.907.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:37:38.000000 tencentcloud-sdk-python-lighthouse-3.0.906/
--rw-r--r--   0 root         (0) root         (0)      758 2023-06-05 00:37:38.000000 tencentcloud-sdk-python-lighthouse-3.0.906/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:37:38.000000 tencentcloud-sdk-python-lighthouse-3.0.906/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-05 00:37:38.000000 tencentcloud-sdk-python-lighthouse-3.0.906/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:37:38.000000 tencentcloud-sdk-python-lighthouse-3.0.906/tencentcloud/lighthouse/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:37:38.000000 tencentcloud-sdk-python-lighthouse-3.0.906/tencentcloud/lighthouse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:37:38.000000 tencentcloud-sdk-python-lighthouse-3.0.906/tencentcloud/lighthouse/v20200324/
--rw-r--r--   0 root         (0) root         (0)    25956 2023-06-05 00:37:38.000000 tencentcloud-sdk-python-lighthouse-3.0.906/tencentcloud/lighthouse/v20200324/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    92541 2023-06-05 00:37:38.000000 tencentcloud-sdk-python-lighthouse-3.0.906/tencentcloud/lighthouse/v20200324/lighthouse_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:37:38.000000 tencentcloud-sdk-python-lighthouse-3.0.906/tencentcloud/lighthouse/v20200324/__init__.py
--rw-r--r--   0 root         (0) root         (0)   240370 2023-06-05 00:37:38.000000 tencentcloud-sdk-python-lighthouse-3.0.906/tencentcloud/lighthouse/v20200324/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:37:38.000000 tencentcloud-sdk-python-lighthouse-3.0.906/tencentcloud_sdk_python_lighthouse.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:37:38.000000 tencentcloud-sdk-python-lighthouse-3.0.906/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-06-05 00:37:38.000000 tencentcloud-sdk-python-lighthouse-3.0.906/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-06-05 00:37:38.000000 tencentcloud-sdk-python-lighthouse-3.0.906/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 00:37:38.000000 tencentcloud-sdk-python-lighthouse-3.0.906/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-06-05 00:37:38.000000 tencentcloud-sdk-python-lighthouse-3.0.906/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1020 2023-06-05 00:37:38.000000 tencentcloud-sdk-python-lighthouse-3.0.906/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-05 00:37:38.000000 tencentcloud-sdk-python-lighthouse-3.0.906/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/
+-rw-r--r--   0 root         (0) root         (0)      758 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud/lighthouse/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud/lighthouse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud/lighthouse/v20200324/
+-rw-r--r--   0 root         (0) root         (0)    26133 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud/lighthouse/v20200324/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    92541 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud/lighthouse/v20200324/lighthouse_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud/lighthouse/v20200324/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   240370 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud/lighthouse/v20200324/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud_sdk_python_lighthouse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/setup.cfg
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.906/README.rst` & `tencentcloud-sdk-python-lighthouse-3.0.907/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.906/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.906/tencentcloud/lighthouse/v20200324/errorcodes.py` & `tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud/lighthouse/v20200324/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,14 +205,17 @@
 
 # 参数值非法，镜像 ID 格式非法。
 INVALIDPARAMETERVALUE_BLUEPRINTIDMALFORMED = 'InvalidParameterValue.BlueprintIdMalformed'
 
 # 套餐和镜像不匹配。
 INVALIDPARAMETERVALUE_BUNDLEANDBLUEPRINTNOTMATCH = 'InvalidParameterValue.BundleAndBlueprintNotMatch'
 
+# 所选套餐不支持镜像的操作系统平台类型。
+INVALIDPARAMETERVALUE_BUNDLENOTSUPPORTBLUEPRINTPLATFORM = 'InvalidParameterValue.BundleNotSupportBlueprintPlatform'
+
 # 云联网实例ID格式非法。
 INVALIDPARAMETERVALUE_CCNIDMALFORMED = 'InvalidParameterValue.CcnIdMalformed'
 
 # 客户令牌长度超出限制。
 INVALIDPARAMETERVALUE_CLIENTTOKENTOOLONG = 'InvalidParameterValue.ClientTokenTooLong'
 
 # 参数值非法，云硬盘备份点 ID 格式非法。
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.906/tencentcloud/lighthouse/v20200324/lighthouse_client.py` & `tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud/lighthouse/v20200324/lighthouse_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.906/tencentcloud/lighthouse/v20200324/models.py` & `tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud/lighthouse/v20200324/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.906/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.906/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.906/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.907/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.906/setup.py` & `tencentcloud-sdk-python-lighthouse-3.0.907/setup.py`

 * *Files identical despite different names*

