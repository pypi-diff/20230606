# Comparing `tmp/tencentcloud-sdk-python-tdmq-3.0.906.tar.gz` & `tmp/tencentcloud-sdk-python-tdmq-3.0.907.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.906.tar", last modified: Mon Jun  5 00:43:41 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.907.tar", last modified: Tue Jun  6 02:36:23 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tdmq-3.0.906.tar` & `tencentcloud-sdk-python-tdmq-3.0.907.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:43:41.000000 tencentcloud-sdk-python-tdmq-3.0.906/
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-05 00:43:41.000000 tencentcloud-sdk-python-tdmq-3.0.906/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:43:41.000000 tencentcloud-sdk-python-tdmq-3.0.906/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:43:41.000000 tencentcloud-sdk-python-tdmq-3.0.906/tencentcloud/tdmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:43:41.000000 tencentcloud-sdk-python-tdmq-3.0.906/tencentcloud/tdmq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:43:41.000000 tencentcloud-sdk-python-tdmq-3.0.906/tencentcloud/tdmq/v20200217/
--rw-r--r--   0 root         (0) root         (0)   103763 2023-06-05 00:43:41.000000 tencentcloud-sdk-python-tdmq-3.0.906/tencentcloud/tdmq/v20200217/tdmq_client.py
--rw-r--r--   0 root         (0) root         (0)    10117 2023-06-05 00:43:41.000000 tencentcloud-sdk-python-tdmq-3.0.906/tencentcloud/tdmq/v20200217/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:43:41.000000 tencentcloud-sdk-python-tdmq-3.0.906/tencentcloud/tdmq/v20200217/__init__.py
--rw-r--r--   0 root         (0) root         (0)   384546 2023-06-05 00:43:41.000000 tencentcloud-sdk-python-tdmq-3.0.906/tencentcloud/tdmq/v20200217/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-05 00:43:41.000000 tencentcloud-sdk-python-tdmq-3.0.906/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-05 00:43:41.000000 tencentcloud-sdk-python-tdmq-3.0.906/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:43:41.000000 tencentcloud-sdk-python-tdmq-3.0.906/tencentcloud_sdk_python_tdmq.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:43:41.000000 tencentcloud-sdk-python-tdmq-3.0.906/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-05 00:43:41.000000 tencentcloud-sdk-python-tdmq-3.0.906/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-05 00:43:41.000000 tencentcloud-sdk-python-tdmq-3.0.906/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 00:43:41.000000 tencentcloud-sdk-python-tdmq-3.0.906/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-05 00:43:41.000000 tencentcloud-sdk-python-tdmq-3.0.906/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-05 00:43:41.000000 tencentcloud-sdk-python-tdmq-3.0.906/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:36:23.000000 tencentcloud-sdk-python-tdmq-3.0.907/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-06 02:36:23.000000 tencentcloud-sdk-python-tdmq-3.0.907/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:36:23.000000 tencentcloud-sdk-python-tdmq-3.0.907/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:36:23.000000 tencentcloud-sdk-python-tdmq-3.0.907/tencentcloud/tdmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:36:23.000000 tencentcloud-sdk-python-tdmq-3.0.907/tencentcloud/tdmq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:36:23.000000 tencentcloud-sdk-python-tdmq-3.0.907/tencentcloud/tdmq/v20200217/
+-rw-r--r--   0 root         (0) root         (0)   103763 2023-06-06 02:36:23.000000 tencentcloud-sdk-python-tdmq-3.0.907/tencentcloud/tdmq/v20200217/tdmq_client.py
+-rw-r--r--   0 root         (0) root         (0)    10117 2023-06-06 02:36:23.000000 tencentcloud-sdk-python-tdmq-3.0.907/tencentcloud/tdmq/v20200217/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:36:23.000000 tencentcloud-sdk-python-tdmq-3.0.907/tencentcloud/tdmq/v20200217/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   384881 2023-06-06 02:36:23.000000 tencentcloud-sdk-python-tdmq-3.0.907/tencentcloud/tdmq/v20200217/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:36:23.000000 tencentcloud-sdk-python-tdmq-3.0.907/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-06 02:36:23.000000 tencentcloud-sdk-python-tdmq-3.0.907/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:36:23.000000 tencentcloud-sdk-python-tdmq-3.0.907/tencentcloud_sdk_python_tdmq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:36:23.000000 tencentcloud-sdk-python-tdmq-3.0.907/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-06 02:36:23.000000 tencentcloud-sdk-python-tdmq-3.0.907/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-06 02:36:23.000000 tencentcloud-sdk-python-tdmq-3.0.907/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:36:23.000000 tencentcloud-sdk-python-tdmq-3.0.907/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-06 02:36:23.000000 tencentcloud-sdk-python-tdmq-3.0.907/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:36:23.000000 tencentcloud-sdk-python-tdmq-3.0.907/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.906/README.rst` & `tencentcloud-sdk-python-tdmq-3.0.907/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.906/tencentcloud/tdmq/v20200217/tdmq_client.py` & `tencentcloud-sdk-python-tdmq-3.0.907/tencentcloud/tdmq/v20200217/tdmq_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.906/tencentcloud/tdmq/v20200217/errorcodes.py` & `tencentcloud-sdk-python-tdmq-3.0.907/tencentcloud/tdmq/v20200217/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.906/tencentcloud/tdmq/v20200217/models.py` & `tencentcloud-sdk-python-tdmq-3.0.907/tencentcloud/tdmq/v20200217/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5096,30 +5096,38 @@
         :type NamespaceName: str
         :param NeedMetrics: 是否需要监控指标，若传false，则不需要传Limit和Offset分页参数
         :type NeedMetrics: bool
         :param Limit: 查询限制条数
         :type Limit: int
         :param Offset: 查询偏移量
         :type Offset: int
+        :param Bundle: 过滤的 bundle
+        :type Bundle: str
+        :param OwnerBroker: bundle 所属的 broker ip 地址，支持模糊查询
+        :type OwnerBroker: str
         """
         self.ClusterName = None
         self.TenantId = None
         self.NamespaceName = None
         self.NeedMetrics = None
         self.Limit = None
         self.Offset = None
+        self.Bundle = None
+        self.OwnerBroker = None
 
 
     def _deserialize(self, params):
         self.ClusterName = params.get("ClusterName")
         self.TenantId = params.get("TenantId")
         self.NamespaceName = params.get("NamespaceName")
         self.NeedMetrics = params.get("NeedMetrics")
         self.Limit = params.get("Limit")
         self.Offset = params.get("Offset")
+        self.Bundle = params.get("Bundle")
+        self.OwnerBroker = params.get("OwnerBroker")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.906/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tdmq-3.0.907/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tdmq-3.0.906/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.907/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.906/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.907/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.906/setup.py` & `tencentcloud-sdk-python-tdmq-3.0.907/setup.py`

 * *Files identical despite different names*

