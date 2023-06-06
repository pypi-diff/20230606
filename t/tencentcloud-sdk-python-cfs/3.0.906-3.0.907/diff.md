# Comparing `tmp/tencentcloud-sdk-python-cfs-3.0.906.tar.gz` & `tmp/tencentcloud-sdk-python-cfs-3.0.907.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cfs-3.0.906.tar", last modified: Mon Jun  5 00:29:39 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cfs-3.0.907.tar", last modified: Tue Jun  6 02:21:46 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cfs-3.0.906.tar` & `tencentcloud-sdk-python-cfs-3.0.907.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:29:39.000000 tencentcloud-sdk-python-cfs-3.0.906/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-05 00:29:39.000000 tencentcloud-sdk-python-cfs-3.0.906/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:29:39.000000 tencentcloud-sdk-python-cfs-3.0.906/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:29:39.000000 tencentcloud-sdk-python-cfs-3.0.906/tencentcloud/cfs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:29:39.000000 tencentcloud-sdk-python-cfs-3.0.906/tencentcloud/cfs/v20190719/
--rw-r--r--   0 root         (0) root         (0)    14458 2023-06-05 00:29:39.000000 tencentcloud-sdk-python-cfs-3.0.906/tencentcloud/cfs/v20190719/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    39796 2023-06-05 00:29:39.000000 tencentcloud-sdk-python-cfs-3.0.906/tencentcloud/cfs/v20190719/cfs_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:29:39.000000 tencentcloud-sdk-python-cfs-3.0.906/tencentcloud/cfs/v20190719/__init__.py
--rw-r--r--   0 root         (0) root         (0)   116710 2023-06-05 00:29:39.000000 tencentcloud-sdk-python-cfs-3.0.906/tencentcloud/cfs/v20190719/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:29:39.000000 tencentcloud-sdk-python-cfs-3.0.906/tencentcloud/cfs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-05 00:29:39.000000 tencentcloud-sdk-python-cfs-3.0.906/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:29:39.000000 tencentcloud-sdk-python-cfs-3.0.906/tencentcloud_sdk_python_cfs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:29:39.000000 tencentcloud-sdk-python-cfs-3.0.906/tencentcloud_sdk_python_cfs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-05 00:29:39.000000 tencentcloud-sdk-python-cfs-3.0.906/tencentcloud_sdk_python_cfs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-05 00:29:39.000000 tencentcloud-sdk-python-cfs-3.0.906/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 00:29:39.000000 tencentcloud-sdk-python-cfs-3.0.906/tencentcloud_sdk_python_cfs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-05 00:29:39.000000 tencentcloud-sdk-python-cfs-3.0.906/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-05 00:29:39.000000 tencentcloud-sdk-python-cfs-3.0.906/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-05 00:29:39.000000 tencentcloud-sdk-python-cfs-3.0.906/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:21:46.000000 tencentcloud-sdk-python-cfs-3.0.907/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-06 02:21:46.000000 tencentcloud-sdk-python-cfs-3.0.907/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:21:46.000000 tencentcloud-sdk-python-cfs-3.0.907/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:21:46.000000 tencentcloud-sdk-python-cfs-3.0.907/tencentcloud/cfs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:21:46.000000 tencentcloud-sdk-python-cfs-3.0.907/tencentcloud/cfs/v20190719/
+-rw-r--r--   0 root         (0) root         (0)    14458 2023-06-06 02:21:46.000000 tencentcloud-sdk-python-cfs-3.0.907/tencentcloud/cfs/v20190719/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    39796 2023-06-06 02:21:46.000000 tencentcloud-sdk-python-cfs-3.0.907/tencentcloud/cfs/v20190719/cfs_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:21:46.000000 tencentcloud-sdk-python-cfs-3.0.907/tencentcloud/cfs/v20190719/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   117345 2023-06-06 02:21:46.000000 tencentcloud-sdk-python-cfs-3.0.907/tencentcloud/cfs/v20190719/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:21:46.000000 tencentcloud-sdk-python-cfs-3.0.907/tencentcloud/cfs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:21:46.000000 tencentcloud-sdk-python-cfs-3.0.907/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:21:46.000000 tencentcloud-sdk-python-cfs-3.0.907/tencentcloud_sdk_python_cfs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:21:46.000000 tencentcloud-sdk-python-cfs-3.0.907/tencentcloud_sdk_python_cfs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-06 02:21:46.000000 tencentcloud-sdk-python-cfs-3.0.907/tencentcloud_sdk_python_cfs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-06 02:21:46.000000 tencentcloud-sdk-python-cfs-3.0.907/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:21:46.000000 tencentcloud-sdk-python-cfs-3.0.907/tencentcloud_sdk_python_cfs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-06 02:21:46.000000 tencentcloud-sdk-python-cfs-3.0.907/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-06 02:21:46.000000 tencentcloud-sdk-python-cfs-3.0.907/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:21:46.000000 tencentcloud-sdk-python-cfs-3.0.907/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.906/README.rst` & `tencentcloud-sdk-python-cfs-3.0.907/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfs-3.0.906/tencentcloud/cfs/v20190719/errorcodes.py` & `tencentcloud-sdk-python-cfs-3.0.907/tencentcloud/cfs/v20190719/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfs-3.0.906/tencentcloud/cfs/v20190719/cfs_client.py` & `tencentcloud-sdk-python-cfs-3.0.907/tencentcloud/cfs/v20190719/cfs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfs-3.0.906/tencentcloud/cfs/v20190719/models.py` & `tencentcloud-sdk-python-cfs-3.0.907/tencentcloud/cfs/v20190719/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2989,14 +2989,33 @@
 
 
 class TieringDetailInfo(AbstractModel):
     """分层存储详细信息
 
     """
 
+    def __init__(self):
+        r"""
+        :param TieringSizeInBytes: 低频存储容量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TieringSizeInBytes: int
+        """
+        self.TieringSizeInBytes = None
+
+
+    def _deserialize(self, params):
+        self.TieringSizeInBytes = params.get("TieringSizeInBytes")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
 
 class UnbindAutoSnapshotPolicyRequest(AbstractModel):
     """UnbindAutoSnapshotPolicy请求参数结构体
 
     """
 
     def __init__(self):
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.906/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cfs-3.0.907/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cfs-3.0.906/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cfs-3.0.907/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfs
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Cfs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.906/PKG-INFO` & `tencentcloud-sdk-python-cfs-3.0.907/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfs
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Cfs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.906/setup.py` & `tencentcloud-sdk-python-cfs-3.0.907/setup.py`

 * *Files identical despite different names*

