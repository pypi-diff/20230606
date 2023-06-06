# Comparing `tmp/tencentcloud-sdk-python-privatedns-3.0.906.tar.gz` & `tmp/tencentcloud-sdk-python-privatedns-3.0.907.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-privatedns-3.0.906.tar", last modified: Mon Jun  5 00:40:01 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-privatedns-3.0.907.tar", last modified: Tue Jun  6 02:32:25 2023, max compression
```

## Comparing `tencentcloud-sdk-python-privatedns-3.0.906.tar` & `tencentcloud-sdk-python-privatedns-3.0.907.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:40:01.000000 tencentcloud-sdk-python-privatedns-3.0.906/
--rw-r--r--   0 root         (0) root         (0)      758 2023-06-05 00:40:01.000000 tencentcloud-sdk-python-privatedns-3.0.906/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:40:01.000000 tencentcloud-sdk-python-privatedns-3.0.906/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:40:01.000000 tencentcloud-sdk-python-privatedns-3.0.906/tencentcloud/privatedns/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:40:01.000000 tencentcloud-sdk-python-privatedns-3.0.906/tencentcloud/privatedns/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:40:01.000000 tencentcloud-sdk-python-privatedns-3.0.906/tencentcloud/privatedns/v20201028/
--rw-r--r--   0 root         (0) root         (0)     7071 2023-06-05 00:40:01.000000 tencentcloud-sdk-python-privatedns-3.0.906/tencentcloud/privatedns/v20201028/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:40:01.000000 tencentcloud-sdk-python-privatedns-3.0.906/tencentcloud/privatedns/v20201028/__init__.py
--rw-r--r--   0 root         (0) root         (0)    57994 2023-06-05 00:40:01.000000 tencentcloud-sdk-python-privatedns-3.0.906/tencentcloud/privatedns/v20201028/models.py
--rw-r--r--   0 root         (0) root         (0)    20216 2023-06-05 00:40:01.000000 tencentcloud-sdk-python-privatedns-3.0.906/tencentcloud/privatedns/v20201028/privatedns_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-05 00:40:01.000000 tencentcloud-sdk-python-privatedns-3.0.906/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:40:01.000000 tencentcloud-sdk-python-privatedns-3.0.906/tencentcloud_sdk_python_privatedns.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:40:01.000000 tencentcloud-sdk-python-privatedns-3.0.906/tencentcloud_sdk_python_privatedns.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-06-05 00:40:01.000000 tencentcloud-sdk-python-privatedns-3.0.906/tencentcloud_sdk_python_privatedns.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-06-05 00:40:01.000000 tencentcloud-sdk-python-privatedns-3.0.906/tencentcloud_sdk_python_privatedns.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 00:40:01.000000 tencentcloud-sdk-python-privatedns-3.0.906/tencentcloud_sdk_python_privatedns.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-06-05 00:40:01.000000 tencentcloud-sdk-python-privatedns-3.0.906/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1020 2023-06-05 00:40:01.000000 tencentcloud-sdk-python-privatedns-3.0.906/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-05 00:40:01.000000 tencentcloud-sdk-python-privatedns-3.0.906/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:32:25.000000 tencentcloud-sdk-python-privatedns-3.0.907/
+-rw-r--r--   0 root         (0) root         (0)      758 2023-06-06 02:32:24.000000 tencentcloud-sdk-python-privatedns-3.0.907/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:32:25.000000 tencentcloud-sdk-python-privatedns-3.0.907/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:32:25.000000 tencentcloud-sdk-python-privatedns-3.0.907/tencentcloud/privatedns/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:32:24.000000 tencentcloud-sdk-python-privatedns-3.0.907/tencentcloud/privatedns/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:32:25.000000 tencentcloud-sdk-python-privatedns-3.0.907/tencentcloud/privatedns/v20201028/
+-rw-r--r--   0 root         (0) root         (0)     7186 2023-06-06 02:32:24.000000 tencentcloud-sdk-python-privatedns-3.0.907/tencentcloud/privatedns/v20201028/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:32:24.000000 tencentcloud-sdk-python-privatedns-3.0.907/tencentcloud/privatedns/v20201028/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    57994 2023-06-06 02:32:24.000000 tencentcloud-sdk-python-privatedns-3.0.907/tencentcloud/privatedns/v20201028/models.py
+-rw-r--r--   0 root         (0) root         (0)    20216 2023-06-06 02:32:24.000000 tencentcloud-sdk-python-privatedns-3.0.907/tencentcloud/privatedns/v20201028/privatedns_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:32:24.000000 tencentcloud-sdk-python-privatedns-3.0.907/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:32:25.000000 tencentcloud-sdk-python-privatedns-3.0.907/tencentcloud_sdk_python_privatedns.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:32:25.000000 tencentcloud-sdk-python-privatedns-3.0.907/tencentcloud_sdk_python_privatedns.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-06-06 02:32:25.000000 tencentcloud-sdk-python-privatedns-3.0.907/tencentcloud_sdk_python_privatedns.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-06-06 02:32:25.000000 tencentcloud-sdk-python-privatedns-3.0.907/tencentcloud_sdk_python_privatedns.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:32:25.000000 tencentcloud-sdk-python-privatedns-3.0.907/tencentcloud_sdk_python_privatedns.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-06-06 02:32:25.000000 tencentcloud-sdk-python-privatedns-3.0.907/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-06-06 02:32:24.000000 tencentcloud-sdk-python-privatedns-3.0.907/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:32:25.000000 tencentcloud-sdk-python-privatedns-3.0.907/setup.cfg
```

### Comparing `tencentcloud-sdk-python-privatedns-3.0.906/README.rst` & `tencentcloud-sdk-python-privatedns-3.0.907/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-privatedns-3.0.906/tencentcloud/privatedns/v20201028/errorcodes.py` & `tencentcloud-sdk-python-privatedns-3.0.907/tencentcloud/privatedns/v20201028/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,17 @@
 
 # VPC非法。
 INVALIDPARAMETER_ILLEGALVPCINFO = 'InvalidParameter.IllegalVpcInfo'
 
 # MX 必须为5-50之间且为5的倍数。
 INVALIDPARAMETER_INVALIDMX = 'InvalidParameter.InvalidMX'
 
+# 该记录类型不支持 MX 优先级设置
+INVALIDPARAMETER_MXNOTSUPPORTED = 'InvalidParameter.MXNotSupported'
+
 # AAAA记录负载均衡数量超过50。
 INVALIDPARAMETER_RECORDAAAACOUNTEXCEED = 'InvalidParameter.RecordAAAACountExceed'
 
 # A记录负载均衡数量超过50。
 INVALIDPARAMETER_RECORDACOUNTEXCEED = 'InvalidParameter.RecordACountExceed'
 
 # CNAME记录负载均衡数量超过50。
```

### Comparing `tencentcloud-sdk-python-privatedns-3.0.906/tencentcloud/privatedns/v20201028/models.py` & `tencentcloud-sdk-python-privatedns-3.0.907/tencentcloud/privatedns/v20201028/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-privatedns-3.0.906/tencentcloud/privatedns/v20201028/privatedns_client.py` & `tencentcloud-sdk-python-privatedns-3.0.907/tencentcloud/privatedns/v20201028/privatedns_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-privatedns-3.0.906/tencentcloud/__init__.py` & `tencentcloud-sdk-python-privatedns-3.0.907/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-privatedns-3.0.906/tencentcloud_sdk_python_privatedns.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-privatedns-3.0.907/tencentcloud_sdk_python_privatedns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-privatedns-3.0.906/tencentcloud_sdk_python_privatedns.egg-info/PKG-INFO` & `tencentcloud-sdk-python-privatedns-3.0.907/tencentcloud_sdk_python_privatedns.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-privatedns
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Privatedns SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-privatedns-3.0.906/PKG-INFO` & `tencentcloud-sdk-python-privatedns-3.0.907/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-privatedns
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Privatedns SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-privatedns-3.0.906/setup.py` & `tencentcloud-sdk-python-privatedns-3.0.907/setup.py`

 * *Files identical despite different names*

