# Comparing `tmp/tencentcloud-sdk-python-emr-3.0.906.tar.gz` & `tmp/tencentcloud-sdk-python-emr-3.0.907.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-emr-3.0.906.tar", last modified: Mon Jun  5 00:34:15 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-emr-3.0.907.tar", last modified: Tue Jun  6 02:26:34 2023, max compression
```

## Comparing `tencentcloud-sdk-python-emr-3.0.906.tar` & `tencentcloud-sdk-python-emr-3.0.907.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:34:15.000000 tencentcloud-sdk-python-emr-3.0.906/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-05 00:34:14.000000 tencentcloud-sdk-python-emr-3.0.906/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:34:15.000000 tencentcloud-sdk-python-emr-3.0.906/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:34:15.000000 tencentcloud-sdk-python-emr-3.0.906/tencentcloud/emr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:34:14.000000 tencentcloud-sdk-python-emr-3.0.906/tencentcloud/emr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:34:15.000000 tencentcloud-sdk-python-emr-3.0.906/tencentcloud/emr/v20190103/
--rw-r--r--   0 root         (0) root         (0)    27330 2023-06-05 00:34:14.000000 tencentcloud-sdk-python-emr-3.0.906/tencentcloud/emr/v20190103/emr_client.py
--rw-r--r--   0 root         (0) root         (0)    13881 2023-06-05 00:34:14.000000 tencentcloud-sdk-python-emr-3.0.906/tencentcloud/emr/v20190103/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:34:14.000000 tencentcloud-sdk-python-emr-3.0.906/tencentcloud/emr/v20190103/__init__.py
--rw-r--r--   0 root         (0) root         (0)   260148 2023-06-05 00:34:14.000000 tencentcloud-sdk-python-emr-3.0.906/tencentcloud/emr/v20190103/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-05 00:34:14.000000 tencentcloud-sdk-python-emr-3.0.906/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-05 00:34:15.000000 tencentcloud-sdk-python-emr-3.0.906/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:34:15.000000 tencentcloud-sdk-python-emr-3.0.906/tencentcloud_sdk_python_emr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:34:15.000000 tencentcloud-sdk-python-emr-3.0.906/tencentcloud_sdk_python_emr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-05 00:34:15.000000 tencentcloud-sdk-python-emr-3.0.906/tencentcloud_sdk_python_emr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-05 00:34:15.000000 tencentcloud-sdk-python-emr-3.0.906/tencentcloud_sdk_python_emr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 00:34:15.000000 tencentcloud-sdk-python-emr-3.0.906/tencentcloud_sdk_python_emr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-05 00:34:14.000000 tencentcloud-sdk-python-emr-3.0.906/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-05 00:34:15.000000 tencentcloud-sdk-python-emr-3.0.906/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:26:34.000000 tencentcloud-sdk-python-emr-3.0.907/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-06 02:26:34.000000 tencentcloud-sdk-python-emr-3.0.907/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:26:34.000000 tencentcloud-sdk-python-emr-3.0.907/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:26:34.000000 tencentcloud-sdk-python-emr-3.0.907/tencentcloud/emr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:26:34.000000 tencentcloud-sdk-python-emr-3.0.907/tencentcloud/emr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:26:34.000000 tencentcloud-sdk-python-emr-3.0.907/tencentcloud/emr/v20190103/
+-rw-r--r--   0 root         (0) root         (0)    27330 2023-06-06 02:26:34.000000 tencentcloud-sdk-python-emr-3.0.907/tencentcloud/emr/v20190103/emr_client.py
+-rw-r--r--   0 root         (0) root         (0)    13996 2023-06-06 02:26:34.000000 tencentcloud-sdk-python-emr-3.0.907/tencentcloud/emr/v20190103/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:26:34.000000 tencentcloud-sdk-python-emr-3.0.907/tencentcloud/emr/v20190103/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   260148 2023-06-06 02:26:34.000000 tencentcloud-sdk-python-emr-3.0.907/tencentcloud/emr/v20190103/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:26:34.000000 tencentcloud-sdk-python-emr-3.0.907/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-06 02:26:34.000000 tencentcloud-sdk-python-emr-3.0.907/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:26:34.000000 tencentcloud-sdk-python-emr-3.0.907/tencentcloud_sdk_python_emr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:26:34.000000 tencentcloud-sdk-python-emr-3.0.907/tencentcloud_sdk_python_emr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-06 02:26:34.000000 tencentcloud-sdk-python-emr-3.0.907/tencentcloud_sdk_python_emr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-06 02:26:34.000000 tencentcloud-sdk-python-emr-3.0.907/tencentcloud_sdk_python_emr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:26:34.000000 tencentcloud-sdk-python-emr-3.0.907/tencentcloud_sdk_python_emr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-06 02:26:34.000000 tencentcloud-sdk-python-emr-3.0.907/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:26:34.000000 tencentcloud-sdk-python-emr-3.0.907/setup.cfg
```

### Comparing `tencentcloud-sdk-python-emr-3.0.906/README.rst` & `tencentcloud-sdk-python-emr-3.0.907/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.906/tencentcloud/emr/v20190103/emr_client.py` & `tencentcloud-sdk-python-emr-3.0.907/tencentcloud/emr/v20190103/emr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.906/tencentcloud/emr/v20190103/errorcodes.py` & `tencentcloud-sdk-python-emr-3.0.907/tencentcloud/emr/v20190103/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,14 +358,17 @@
 
 # 资源不存在。
 RESOURCENOTFOUND_CDBINFONOTFOUND = 'ResourceNotFound.CDBInfoNotFound'
 
 # 无法找到该实例。
 RESOURCENOTFOUND_CLUSTERNOTFOUND = 'ResourceNotFound.ClusterNotFound'
 
+# 无法找到指定的CVM实例。
+RESOURCENOTFOUND_CVMINSTANCENOTFOUND = 'ResourceNotFound.CvmInstanceNotFound'
+
 # 无法找到硬件信息。
 RESOURCENOTFOUND_HARDWAREINFONOTFOUND = 'ResourceNotFound.HardwareInfoNotFound'
 
 # 无法找到该实例。
 RESOURCENOTFOUND_INSTANCENOTFOUND = 'ResourceNotFound.InstanceNotFound'
 
 # 无法找到监控元数据。
```

### Comparing `tencentcloud-sdk-python-emr-3.0.906/tencentcloud/emr/v20190103/models.py` & `tencentcloud-sdk-python-emr-3.0.907/tencentcloud/emr/v20190103/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.906/tencentcloud/__init__.py` & `tencentcloud-sdk-python-emr-3.0.907/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-emr-3.0.906/PKG-INFO` & `tencentcloud-sdk-python-emr-3.0.907/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-emr
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Emr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-emr-3.0.906/tencentcloud_sdk_python_emr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-emr-3.0.907/tencentcloud_sdk_python_emr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-emr
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Emr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-emr-3.0.906/setup.py` & `tencentcloud-sdk-python-emr-3.0.907/setup.py`

 * *Files identical despite different names*

