# Comparing `tmp/tencentcloud-sdk-python-omics-3.0.906.tar.gz` & `tmp/tencentcloud-sdk-python-omics-3.0.907.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-omics-3.0.906.tar", last modified: Mon Jun  5 00:39:35 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-omics-3.0.907.tar", last modified: Tue Jun  6 02:31:56 2023, max compression
```

## Comparing `tencentcloud-sdk-python-omics-3.0.906.tar` & `tencentcloud-sdk-python-omics-3.0.907.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:35.000000 tencentcloud-sdk-python-omics-3.0.906/
--rw-r--r--   0 root         (0) root         (0)      743 2023-06-05 00:39:35.000000 tencentcloud-sdk-python-omics-3.0.906/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:35.000000 tencentcloud-sdk-python-omics-3.0.906/tencentcloud_sdk_python_omics.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:39:35.000000 tencentcloud-sdk-python-omics-3.0.906/tencentcloud_sdk_python_omics.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-06-05 00:39:35.000000 tencentcloud-sdk-python-omics-3.0.906/tencentcloud_sdk_python_omics.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-05 00:39:35.000000 tencentcloud-sdk-python-omics-3.0.906/tencentcloud_sdk_python_omics.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 00:39:35.000000 tencentcloud-sdk-python-omics-3.0.906/tencentcloud_sdk_python_omics.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:35.000000 tencentcloud-sdk-python-omics-3.0.906/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:35.000000 tencentcloud-sdk-python-omics-3.0.906/tencentcloud/omics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:35.000000 tencentcloud-sdk-python-omics-3.0.906/tencentcloud/omics/v20221128/
--rw-r--r--   0 root         (0) root         (0)    11298 2023-06-05 00:39:35.000000 tencentcloud-sdk-python-omics-3.0.906/tencentcloud/omics/v20221128/omics_client.py
--rw-r--r--   0 root         (0) root         (0)     3972 2023-06-05 00:39:35.000000 tencentcloud-sdk-python-omics-3.0.906/tencentcloud/omics/v20221128/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:39:35.000000 tencentcloud-sdk-python-omics-3.0.906/tencentcloud/omics/v20221128/__init__.py
--rw-r--r--   0 root         (0) root         (0)    55938 2023-06-05 00:39:35.000000 tencentcloud-sdk-python-omics-3.0.906/tencentcloud/omics/v20221128/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:39:35.000000 tencentcloud-sdk-python-omics-3.0.906/tencentcloud/omics/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-05 00:39:35.000000 tencentcloud-sdk-python-omics-3.0.906/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-05 00:39:35.000000 tencentcloud-sdk-python-omics-3.0.906/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-06-05 00:39:35.000000 tencentcloud-sdk-python-omics-3.0.906/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-05 00:39:35.000000 tencentcloud-sdk-python-omics-3.0.906/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:31:56.000000 tencentcloud-sdk-python-omics-3.0.907/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-06-06 02:31:56.000000 tencentcloud-sdk-python-omics-3.0.907/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:31:56.000000 tencentcloud-sdk-python-omics-3.0.907/tencentcloud_sdk_python_omics.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:31:56.000000 tencentcloud-sdk-python-omics-3.0.907/tencentcloud_sdk_python_omics.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-06-06 02:31:56.000000 tencentcloud-sdk-python-omics-3.0.907/tencentcloud_sdk_python_omics.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-06 02:31:56.000000 tencentcloud-sdk-python-omics-3.0.907/tencentcloud_sdk_python_omics.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:31:56.000000 tencentcloud-sdk-python-omics-3.0.907/tencentcloud_sdk_python_omics.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:31:56.000000 tencentcloud-sdk-python-omics-3.0.907/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:31:56.000000 tencentcloud-sdk-python-omics-3.0.907/tencentcloud/omics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:31:56.000000 tencentcloud-sdk-python-omics-3.0.907/tencentcloud/omics/v20221128/
+-rw-r--r--   0 root         (0) root         (0)    11298 2023-06-06 02:31:56.000000 tencentcloud-sdk-python-omics-3.0.907/tencentcloud/omics/v20221128/omics_client.py
+-rw-r--r--   0 root         (0) root         (0)     4079 2023-06-06 02:31:56.000000 tencentcloud-sdk-python-omics-3.0.907/tencentcloud/omics/v20221128/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:31:56.000000 tencentcloud-sdk-python-omics-3.0.907/tencentcloud/omics/v20221128/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    55938 2023-06-06 02:31:56.000000 tencentcloud-sdk-python-omics-3.0.907/tencentcloud/omics/v20221128/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:31:56.000000 tencentcloud-sdk-python-omics-3.0.907/tencentcloud/omics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:31:56.000000 tencentcloud-sdk-python-omics-3.0.907/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-06 02:31:56.000000 tencentcloud-sdk-python-omics-3.0.907/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-06-06 02:31:56.000000 tencentcloud-sdk-python-omics-3.0.907/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:31:56.000000 tencentcloud-sdk-python-omics-3.0.907/setup.cfg
```

### Comparing `tencentcloud-sdk-python-omics-3.0.906/README.rst` & `tencentcloud-sdk-python-omics-3.0.907/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-omics-3.0.906/tencentcloud_sdk_python_omics.egg-info/PKG-INFO` & `tencentcloud-sdk-python-omics-3.0.907/tencentcloud_sdk_python_omics.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-omics
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Omics SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-omics-3.0.906/tencentcloud/omics/v20221128/omics_client.py` & `tencentcloud-sdk-python-omics-3.0.907/tencentcloud/omics/v20221128/omics_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-omics-3.0.906/tencentcloud/omics/v20221128/errorcodes.py` & `tencentcloud-sdk-python-omics-3.0.907/tencentcloud/omics/v20221128/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,17 @@
 
 # Base64编码错误
 INVALIDPARAMETERVALUE_INVALIDBASE64ENCODE = 'InvalidParameterValue.InvalidBase64Encode'
 
 # COS路径错误
 INVALIDPARAMETERVALUE_INVALIDCOSKEY = 'InvalidParameterValue.InvalidCosKey'
 
+# CSV文件格式错误
+INVALIDPARAMETERVALUE_INVALIDCSVFORMAT = 'InvalidParameterValue.InvalidCsvFormat'
+
 # 描述错误
 INVALIDPARAMETERVALUE_INVALIDDESCRIPTION = 'InvalidParameterValue.InvalidDescription'
 
 # 表格列错误
 INVALIDPARAMETERVALUE_INVALIDHEADER = 'InvalidParameterValue.InvalidHeader'
 
 # 输入JSON格式错误
```

### Comparing `tencentcloud-sdk-python-omics-3.0.906/tencentcloud/omics/v20221128/models.py` & `tencentcloud-sdk-python-omics-3.0.907/tencentcloud/omics/v20221128/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-omics-3.0.906/tencentcloud/__init__.py` & `tencentcloud-sdk-python-omics-3.0.907/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-omics-3.0.906/PKG-INFO` & `tencentcloud-sdk-python-omics-3.0.907/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-omics
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Omics SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-omics-3.0.906/setup.py` & `tencentcloud-sdk-python-omics-3.0.907/setup.py`

 * *Files identical despite different names*

