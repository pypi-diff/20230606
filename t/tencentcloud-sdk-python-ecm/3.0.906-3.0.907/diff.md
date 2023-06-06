# Comparing `tmp/tencentcloud-sdk-python-ecm-3.0.906.tar.gz` & `tmp/tencentcloud-sdk-python-ecm-3.0.907.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ecm-3.0.906.tar", last modified: Mon Jun  5 00:33:59 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ecm-3.0.907.tar", last modified: Tue Jun  6 02:26:16 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ecm-3.0.906.tar` & `tencentcloud-sdk-python-ecm-3.0.907.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:33:59.000000 tencentcloud-sdk-python-ecm-3.0.906/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-05 00:33:59.000000 tencentcloud-sdk-python-ecm-3.0.906/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:33:59.000000 tencentcloud-sdk-python-ecm-3.0.906/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:33:59.000000 tencentcloud-sdk-python-ecm-3.0.906/tencentcloud/ecm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:33:59.000000 tencentcloud-sdk-python-ecm-3.0.906/tencentcloud/ecm/v20190719/
--rw-r--r--   0 root         (0) root         (0)   126245 2023-06-05 00:33:59.000000 tencentcloud-sdk-python-ecm-3.0.906/tencentcloud/ecm/v20190719/ecm_client.py
--rw-r--r--   0 root         (0) root         (0)    23407 2023-06-05 00:33:59.000000 tencentcloud-sdk-python-ecm-3.0.906/tencentcloud/ecm/v20190719/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:33:59.000000 tencentcloud-sdk-python-ecm-3.0.906/tencentcloud/ecm/v20190719/__init__.py
--rw-r--r--   0 root         (0) root         (0)   455477 2023-06-05 00:33:59.000000 tencentcloud-sdk-python-ecm-3.0.906/tencentcloud/ecm/v20190719/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:33:59.000000 tencentcloud-sdk-python-ecm-3.0.906/tencentcloud/ecm/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-05 00:33:59.000000 tencentcloud-sdk-python-ecm-3.0.906/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-05 00:33:59.000000 tencentcloud-sdk-python-ecm-3.0.906/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-05 00:33:59.000000 tencentcloud-sdk-python-ecm-3.0.906/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-05 00:33:59.000000 tencentcloud-sdk-python-ecm-3.0.906/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:33:59.000000 tencentcloud-sdk-python-ecm-3.0.906/tencentcloud_sdk_python_ecm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:33:59.000000 tencentcloud-sdk-python-ecm-3.0.906/tencentcloud_sdk_python_ecm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-05 00:33:59.000000 tencentcloud-sdk-python-ecm-3.0.906/tencentcloud_sdk_python_ecm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-05 00:33:59.000000 tencentcloud-sdk-python-ecm-3.0.906/tencentcloud_sdk_python_ecm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 00:33:59.000000 tencentcloud-sdk-python-ecm-3.0.906/tencentcloud_sdk_python_ecm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:26:16.000000 tencentcloud-sdk-python-ecm-3.0.907/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-06 02:26:16.000000 tencentcloud-sdk-python-ecm-3.0.907/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:26:16.000000 tencentcloud-sdk-python-ecm-3.0.907/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:26:16.000000 tencentcloud-sdk-python-ecm-3.0.907/tencentcloud/ecm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:26:16.000000 tencentcloud-sdk-python-ecm-3.0.907/tencentcloud/ecm/v20190719/
+-rw-r--r--   0 root         (0) root         (0)   126245 2023-06-06 02:26:16.000000 tencentcloud-sdk-python-ecm-3.0.907/tencentcloud/ecm/v20190719/ecm_client.py
+-rw-r--r--   0 root         (0) root         (0)    23407 2023-06-06 02:26:16.000000 tencentcloud-sdk-python-ecm-3.0.907/tencentcloud/ecm/v20190719/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:26:16.000000 tencentcloud-sdk-python-ecm-3.0.907/tencentcloud/ecm/v20190719/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   456232 2023-06-06 02:26:16.000000 tencentcloud-sdk-python-ecm-3.0.907/tencentcloud/ecm/v20190719/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:26:16.000000 tencentcloud-sdk-python-ecm-3.0.907/tencentcloud/ecm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:26:16.000000 tencentcloud-sdk-python-ecm-3.0.907/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-06 02:26:16.000000 tencentcloud-sdk-python-ecm-3.0.907/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-06 02:26:16.000000 tencentcloud-sdk-python-ecm-3.0.907/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:26:16.000000 tencentcloud-sdk-python-ecm-3.0.907/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:26:16.000000 tencentcloud-sdk-python-ecm-3.0.907/tencentcloud_sdk_python_ecm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:26:16.000000 tencentcloud-sdk-python-ecm-3.0.907/tencentcloud_sdk_python_ecm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-06 02:26:16.000000 tencentcloud-sdk-python-ecm-3.0.907/tencentcloud_sdk_python_ecm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-06 02:26:16.000000 tencentcloud-sdk-python-ecm-3.0.907/tencentcloud_sdk_python_ecm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:26:16.000000 tencentcloud-sdk-python-ecm-3.0.907/tencentcloud_sdk_python_ecm.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-ecm-3.0.906/README.rst` & `tencentcloud-sdk-python-ecm-3.0.907/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecm-3.0.906/tencentcloud/ecm/v20190719/ecm_client.py` & `tencentcloud-sdk-python-ecm-3.0.907/tencentcloud/ecm/v20190719/ecm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecm-3.0.906/tencentcloud/ecm/v20190719/errorcodes.py` & `tencentcloud-sdk-python-ecm-3.0.907/tencentcloud/ecm/v20190719/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecm-3.0.906/tencentcloud/ecm/v20190719/models.py` & `tencentcloud-sdk-python-ecm-3.0.907/tencentcloud/ecm/v20190719/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5698,24 +5698,33 @@
         r"""
         :param DiskType: 磁盘类型：LOCAL_BASIC
         :type DiskType: str
         :param DiskId: 磁盘ID
         :type DiskId: str
         :param DiskSize: 磁盘大小（GB）
         :type DiskSize: int
+        :param DeleteWithInstance: 是否随实例删除。
+        :type DeleteWithInstance: bool
+        :param SnapshotId: 快照ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SnapshotId: str
         """
         self.DiskType = None
         self.DiskId = None
         self.DiskSize = None
+        self.DeleteWithInstance = None
+        self.SnapshotId = None
 
 
     def _deserialize(self, params):
         self.DiskType = params.get("DiskType")
         self.DiskId = params.get("DiskId")
         self.DiskSize = params.get("DiskSize")
+        self.DeleteWithInstance = params.get("DeleteWithInstance")
+        self.SnapshotId = params.get("SnapshotId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -8852,14 +8861,16 @@
         :type DefaultBandwidthIn: int
         :param UserData: 自定义脚本数据
         :type UserData: str
         :param SystemDisk: 系统盘信息。
         :type SystemDisk: :class:`tencentcloud.ecm.v20190719.models.SystemDisk`
         :param DataDisks: 数据盘信息。
         :type DataDisks: list of DataDisk
+        :param DisableWanIp: 是否禁止外网ip
+        :type DisableWanIp: int
         """
         self.ModuleId = None
         self.ModuleName = None
         self.ModuleState = None
         self.DefaultSystemDiskSize = None
         self.DefaultDataDiskSize = None
         self.InstanceTypeConfig = None
@@ -8869,14 +8880,15 @@
         self.TagSet = None
         self.CloseIpDirect = None
         self.SecurityGroupIds = None
         self.DefaultBandwidthIn = None
         self.UserData = None
         self.SystemDisk = None
         self.DataDisks = None
+        self.DisableWanIp = None
 
 
     def _deserialize(self, params):
         self.ModuleId = params.get("ModuleId")
         self.ModuleName = params.get("ModuleName")
         self.ModuleState = params.get("ModuleState")
         self.DefaultSystemDiskSize = params.get("DefaultSystemDiskSize")
@@ -8904,14 +8916,15 @@
             self.SystemDisk._deserialize(params.get("SystemDisk"))
         if params.get("DataDisks") is not None:
             self.DataDisks = []
             for item in params.get("DataDisks"):
                 obj = DataDisk()
                 obj._deserialize(item)
                 self.DataDisks.append(obj)
+        self.DisableWanIp = params.get("DisableWanIp")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -9324,23 +9337,26 @@
         :type City: :class:`tencentcloud.ecm.v20190719.models.City`
         :param RegionInfo: Region信息。
         :type RegionInfo: :class:`tencentcloud.ecm.v20190719.models.RegionInfo`
         :param ISPSet: 运营商列表。
         :type ISPSet: list of ISP
         :param ISPNum: 运营商数量。
         :type ISPNum: int
+        :param LBSupported: 节点是否支持LB
+        :type LBSupported: bool
         """
         self.ZoneInfo = None
         self.Country = None
         self.Area = None
         self.Province = None
         self.City = None
         self.RegionInfo = None
         self.ISPSet = None
         self.ISPNum = None
+        self.LBSupported = None
 
 
     def _deserialize(self, params):
         if params.get("ZoneInfo") is not None:
             self.ZoneInfo = ZoneInfo()
             self.ZoneInfo._deserialize(params.get("ZoneInfo"))
         if params.get("Country") is not None:
@@ -9361,14 +9377,15 @@
         if params.get("ISPSet") is not None:
             self.ISPSet = []
             for item in params.get("ISPSet"):
                 obj = ISP()
                 obj._deserialize(item)
                 self.ISPSet.append(obj)
         self.ISPNum = params.get("ISPNum")
+        self.LBSupported = params.get("LBSupported")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ecm-3.0.906/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ecm-3.0.907/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ecm-3.0.906/PKG-INFO` & `tencentcloud-sdk-python-ecm-3.0.907/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ecm
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Ecm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ecm-3.0.906/setup.py` & `tencentcloud-sdk-python-ecm-3.0.907/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecm-3.0.906/tencentcloud_sdk_python_ecm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ecm-3.0.907/tencentcloud_sdk_python_ecm.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ecm
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Ecm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

