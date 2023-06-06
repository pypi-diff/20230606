# Comparing `tmp/tencentcloud-sdk-python-wedata-3.0.906.tar.gz` & `tmp/tencentcloud-sdk-python-wedata-3.0.907.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-wedata-3.0.906.tar", last modified: Mon Jun  5 00:46:54 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-wedata-3.0.907.tar", last modified: Tue Jun  6 02:39:30 2023, max compression
```

## Comparing `tencentcloud-sdk-python-wedata-3.0.906.tar` & `tencentcloud-sdk-python-wedata-3.0.907.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:46:54.000000 tencentcloud-sdk-python-wedata-3.0.906/
--rw-r--r--   0 root         (0) root         (0)      746 2023-06-05 00:46:53.000000 tencentcloud-sdk-python-wedata-3.0.906/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:46:54.000000 tencentcloud-sdk-python-wedata-3.0.906/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:46:54.000000 tencentcloud-sdk-python-wedata-3.0.906/tencentcloud/wedata/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:46:53.000000 tencentcloud-sdk-python-wedata-3.0.906/tencentcloud/wedata/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:46:54.000000 tencentcloud-sdk-python-wedata-3.0.906/tencentcloud/wedata/v20210820/
--rw-r--r--   0 root         (0) root         (0)     3323 2023-06-05 00:46:54.000000 tencentcloud-sdk-python-wedata-3.0.906/tencentcloud/wedata/v20210820/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:46:54.000000 tencentcloud-sdk-python-wedata-3.0.906/tencentcloud/wedata/v20210820/__init__.py
--rw-r--r--   0 root         (0) root         (0)   184325 2023-06-05 00:46:54.000000 tencentcloud-sdk-python-wedata-3.0.906/tencentcloud/wedata/v20210820/wedata_client.py
--rw-r--r--   0 root         (0) root         (0)   703148 2023-06-05 00:46:54.000000 tencentcloud-sdk-python-wedata-3.0.906/tencentcloud/wedata/v20210820/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-05 00:46:53.000000 tencentcloud-sdk-python-wedata-3.0.906/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:46:54.000000 tencentcloud-sdk-python-wedata-3.0.906/tencentcloud_sdk_python_wedata.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:46:54.000000 tencentcloud-sdk-python-wedata-3.0.906/tencentcloud_sdk_python_wedata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-06-05 00:46:54.000000 tencentcloud-sdk-python-wedata-3.0.906/tencentcloud_sdk_python_wedata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-05 00:46:54.000000 tencentcloud-sdk-python-wedata-3.0.906/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 00:46:54.000000 tencentcloud-sdk-python-wedata-3.0.906/tencentcloud_sdk_python_wedata.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-05 00:46:54.000000 tencentcloud-sdk-python-wedata-3.0.906/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1012 2023-06-05 00:46:53.000000 tencentcloud-sdk-python-wedata-3.0.906/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-05 00:46:54.000000 tencentcloud-sdk-python-wedata-3.0.906/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:39:30.000000 tencentcloud-sdk-python-wedata-3.0.907/
+-rw-r--r--   0 root         (0) root         (0)      746 2023-06-06 02:39:30.000000 tencentcloud-sdk-python-wedata-3.0.907/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:39:30.000000 tencentcloud-sdk-python-wedata-3.0.907/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:39:30.000000 tencentcloud-sdk-python-wedata-3.0.907/tencentcloud/wedata/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:39:30.000000 tencentcloud-sdk-python-wedata-3.0.907/tencentcloud/wedata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:39:30.000000 tencentcloud-sdk-python-wedata-3.0.907/tencentcloud/wedata/v20210820/
+-rw-r--r--   0 root         (0) root         (0)     3323 2023-06-06 02:39:30.000000 tencentcloud-sdk-python-wedata-3.0.907/tencentcloud/wedata/v20210820/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:39:30.000000 tencentcloud-sdk-python-wedata-3.0.907/tencentcloud/wedata/v20210820/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   184325 2023-06-06 02:39:30.000000 tencentcloud-sdk-python-wedata-3.0.907/tencentcloud/wedata/v20210820/wedata_client.py
+-rw-r--r--   0 root         (0) root         (0)   717295 2023-06-06 02:39:30.000000 tencentcloud-sdk-python-wedata-3.0.907/tencentcloud/wedata/v20210820/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:39:30.000000 tencentcloud-sdk-python-wedata-3.0.907/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:39:30.000000 tencentcloud-sdk-python-wedata-3.0.907/tencentcloud_sdk_python_wedata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:39:30.000000 tencentcloud-sdk-python-wedata-3.0.907/tencentcloud_sdk_python_wedata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-06-06 02:39:30.000000 tencentcloud-sdk-python-wedata-3.0.907/tencentcloud_sdk_python_wedata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-06 02:39:30.000000 tencentcloud-sdk-python-wedata-3.0.907/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:39:30.000000 tencentcloud-sdk-python-wedata-3.0.907/tencentcloud_sdk_python_wedata.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-06 02:39:30.000000 tencentcloud-sdk-python-wedata-3.0.907/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-06-06 02:39:30.000000 tencentcloud-sdk-python-wedata-3.0.907/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:39:30.000000 tencentcloud-sdk-python-wedata-3.0.907/setup.cfg
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.906/README.rst` & `tencentcloud-sdk-python-wedata-3.0.907/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wedata-3.0.906/tencentcloud/wedata/v20210820/errorcodes.py` & `tencentcloud-sdk-python-wedata-3.0.907/tencentcloud/wedata/v20210820/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wedata-3.0.906/tencentcloud/wedata/v20210820/wedata_client.py` & `tencentcloud-sdk-python-wedata-3.0.907/tencentcloud/wedata/v20210820/wedata_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wedata-3.0.906/tencentcloud/wedata/v20210820/models.py` & `tencentcloud-sdk-python-wedata-3.0.907/tencentcloud/wedata/v20210820/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,17 @@
         :type IsSendSuccess: int
         :param MessageId: 消息ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type MessageId: str
         :param Operator: 阈值计算算子，1 : 大于 2 ：小于
 注意：此字段可能返回 null，表示取不到有效值。
         :type Operator: int
+        :param RegularId: 告警规则ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RegularId: str
         """
         self.AlarmId = None
         self.AlarmTime = None
         self.TaskId = None
         self.RegularName = None
         self.AlarmLevel = None
         self.AlarmWay = None
@@ -81,14 +84,15 @@
         self.TriggerType = None
         self.EstimatedTime = None
         self.InstanceId = None
         self.TaskName = None
         self.IsSendSuccess = None
         self.MessageId = None
         self.Operator = None
+        self.RegularId = None
 
 
     def _deserialize(self, params):
         self.AlarmId = params.get("AlarmId")
         self.AlarmTime = params.get("AlarmTime")
         self.TaskId = params.get("TaskId")
         self.RegularName = params.get("RegularName")
@@ -101,14 +105,15 @@
         self.TriggerType = params.get("TriggerType")
         self.EstimatedTime = params.get("EstimatedTime")
         self.InstanceId = params.get("InstanceId")
         self.TaskName = params.get("TaskName")
         self.IsSendSuccess = params.get("IsSendSuccess")
         self.MessageId = params.get("MessageId")
         self.Operator = params.get("Operator")
+        self.RegularId = params.get("RegularId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1332,32 +1337,36 @@
 
     """
 
     def __init__(self):
         r"""
         :param ProjectId: 项目名称
         :type ProjectId: str
-        :param TaskId: 任务ID
-        :type TaskId: str
         :param AlarmRegularName: 规则名称
         :type AlarmRegularName: str
+        :param TaskId: 任务ID
+        :type TaskId: str
         :param Id: 主键ID
         :type Id: str
+        :param TaskType: 任务类型:201.实时,202.离线
+        :type TaskType: int
         """
         self.ProjectId = None
-        self.TaskId = None
         self.AlarmRegularName = None
+        self.TaskId = None
         self.Id = None
+        self.TaskType = None
 
 
     def _deserialize(self, params):
         self.ProjectId = params.get("ProjectId")
-        self.TaskId = params.get("TaskId")
         self.AlarmRegularName = params.get("AlarmRegularName")
+        self.TaskId = params.get("TaskId")
         self.Id = params.get("Id")
+        self.TaskType = params.get("TaskType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2790,27 +2799,27 @@
 class CreateOrUpdateResourceRequest(AbstractModel):
     """CreateOrUpdateResource请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param ProjectId: 项目ID
+        :param ProjectId: 项目ID，必填项
         :type ProjectId: str
-        :param Files: 文件名
+        :param Files: 文件名，必填项
         :type Files: list of str
-        :param FilePath: 文件所属路径，资源管理根路径为 /datastudio/resouce
+        :param FilePath: 必填项，文件所属路径，资源管理根路径为 /datastudio/resource/项目ID/文件夹名
         :type FilePath: str
         :param CosBucketName: cos存储桶名字
         :type CosBucketName: str
         :param CosRegion: cos所属地域
         :type CosRegion: str
         :param NewFile: 是否为新文件，新增为 true，更新为 false
         :type NewFile: bool
-        :param FilesSize: 文件大小
+        :param FilesSize: 必填项，文件大小，与 Files 字段对应
         :type FilesSize: list of str
         """
         self.ProjectId = None
         self.Files = None
         self.FilePath = None
         self.CosBucketName = None
         self.CosRegion = None
@@ -6098,23 +6107,38 @@
 
     """
 
     def __init__(self):
         r"""
         :param Data: 结果
         :type Data: str
+        :param InstanceList: 实例列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceList: list of InstanceList
+        :param TotalCount: 总条数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TotalCount: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.Data = None
+        self.InstanceList = None
+        self.TotalCount = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.Data = params.get("Data")
+        if params.get("InstanceList") is not None:
+            self.InstanceList = []
+            for item in params.get("InstanceList"):
+                obj = InstanceList()
+                obj._deserialize(item)
+                self.InstanceList.append(obj)
+        self.TotalCount = params.get("TotalCount")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeInstanceLogListRequest(AbstractModel):
     """DescribeInstanceLogList请求参数结构体
 
     """
@@ -6147,23 +6171,33 @@
 
     """
 
     def __init__(self):
         r"""
         :param Data: 日志列表
         :type Data: str
+        :param InstanceLogList: 日志列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceLogList: list of InstanceLogList
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.Data = None
+        self.InstanceLogList = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.Data = params.get("Data")
+        if params.get("InstanceLogList") is not None:
+            self.InstanceLogList = []
+            for item in params.get("InstanceLogList"):
+                obj = InstanceLogList()
+                obj._deserialize(item)
+                self.InstanceLogList.append(obj)
         self.RequestId = params.get("RequestId")
 
 
 class DescribeInstanceLogRequest(AbstractModel):
     """DescribeInstanceLog请求参数结构体
 
     """
@@ -6204,23 +6238,30 @@
 
     """
 
     def __init__(self):
         r"""
         :param Data: 返回结果
         :type Data: str
+        :param InstanceLogInfo: 返回结果
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceLogInfo: :class:`tencentcloud.wedata.v20210820.models.IntegrationInstanceLog`
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.Data = None
+        self.InstanceLogInfo = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.Data = params.get("Data")
+        if params.get("InstanceLogInfo") is not None:
+            self.InstanceLogInfo = IntegrationInstanceLog()
+            self.InstanceLogInfo._deserialize(params.get("InstanceLogInfo"))
         self.RequestId = params.get("RequestId")
 
 
 class DescribeInstanceLogsRequest(AbstractModel):
     """DescribeInstanceLogs请求参数结构体
 
     """
@@ -6937,28 +6978,33 @@
     """
 
     def __init__(self):
         r"""
         :param TaskInfoSet: 任务列表
 注意：此字段可能返回 null，表示取不到有效值。
         :type TaskInfoSet: list of IntegrationTaskInfo
+        :param TotalCount: 任务总数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TotalCount: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.TaskInfoSet = None
+        self.TotalCount = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         if params.get("TaskInfoSet") is not None:
             self.TaskInfoSet = []
             for item in params.get("TaskInfoSet"):
                 obj = IntegrationTaskInfo()
                 obj._deserialize(item)
                 self.TaskInfoSet.append(obj)
+        self.TotalCount = params.get("TotalCount")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeIntegrationVersionNodesInfoRequest(AbstractModel):
     """DescribeIntegrationVersionNodesInfo请求参数结构体
 
     """
@@ -9790,56 +9836,56 @@
 class DescribeTaskAlarmRegulationsRequest(AbstractModel):
     """DescribeTaskAlarmRegulations请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param TaskId: 任务ID
-        :type TaskId: str
         :param ProjectId: 项目ID
         :type ProjectId: str
-        :param TaskType: 任务类型(201代表实时任务，202代表离线任务)
-        :type TaskType: int
         :param PageNumber: 当前页
         :type PageNumber: int
         :param PageSize: 每页记录数
         :type PageSize: int
         :param Filters: 过滤条件(name有RegularStatus、AlarmLevel、AlarmIndicator、RegularName)
         :type Filters: list of Filter
         :param OrderFields: 排序条件(RegularId)
         :type OrderFields: list of OrderField
+        :param TaskId: 任务ID
+        :type TaskId: str
+        :param TaskType: 任务类型(201代表实时任务，202代表离线任务)
+        :type TaskType: int
         """
-        self.TaskId = None
         self.ProjectId = None
-        self.TaskType = None
         self.PageNumber = None
         self.PageSize = None
         self.Filters = None
         self.OrderFields = None
+        self.TaskId = None
+        self.TaskType = None
 
 
     def _deserialize(self, params):
-        self.TaskId = params.get("TaskId")
         self.ProjectId = params.get("ProjectId")
-        self.TaskType = params.get("TaskType")
         self.PageNumber = params.get("PageNumber")
         self.PageSize = params.get("PageSize")
         if params.get("Filters") is not None:
             self.Filters = []
             for item in params.get("Filters"):
                 obj = Filter()
                 obj._deserialize(item)
                 self.Filters.append(obj)
         if params.get("OrderFields") is not None:
             self.OrderFields = []
             for item in params.get("OrderFields"):
                 obj = OrderField()
                 obj._deserialize(item)
                 self.OrderFields.append(obj)
+        self.TaskId = params.get("TaskId")
+        self.TaskType = params.get("TaskType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -9848,15 +9894,15 @@
 class DescribeTaskAlarmRegulationsResponse(AbstractModel):
     """DescribeTaskAlarmRegulations返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param TaskAlarmInfos: 任务告警规则信息
+        :param TaskAlarmInfos: 告警规则信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type TaskAlarmInfos: list of TaskAlarmInfo
         :param TotalCount: 总记录数
 注意：此字段可能返回 null，表示取不到有效值。
         :type TotalCount: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
@@ -11989,14 +12035,94 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class InstanceList(AbstractModel):
+    """离线运维实例列表
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CostTime: 耗费时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CostTime: str
+        :param CurRunDate: 数据时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CurRunDate: str
+        :param CycleType: 周期类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CycleType: str
+        :param DoFlag: 是否补录
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DoFlag: int
+        :param InCharge: 责任人
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InCharge: str
+        :param LastLog: 日志
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LastLog: str
+        :param SchedulerDesc: 调度计划
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SchedulerDesc: str
+        :param StartTime: 开始启动时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StartTime: str
+        :param State: 实例状态
+注意：此字段可能返回 null，表示取不到有效值。
+        :type State: str
+        :param TaskId: 任务ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TaskId: str
+        :param TaskName: 任务名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TaskName: str
+        :param TryLimit: 尝试运行次数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TryLimit: int
+        """
+        self.CostTime = None
+        self.CurRunDate = None
+        self.CycleType = None
+        self.DoFlag = None
+        self.InCharge = None
+        self.LastLog = None
+        self.SchedulerDesc = None
+        self.StartTime = None
+        self.State = None
+        self.TaskId = None
+        self.TaskName = None
+        self.TryLimit = None
+
+
+    def _deserialize(self, params):
+        self.CostTime = params.get("CostTime")
+        self.CurRunDate = params.get("CurRunDate")
+        self.CycleType = params.get("CycleType")
+        self.DoFlag = params.get("DoFlag")
+        self.InCharge = params.get("InCharge")
+        self.LastLog = params.get("LastLog")
+        self.SchedulerDesc = params.get("SchedulerDesc")
+        self.StartTime = params.get("StartTime")
+        self.State = params.get("State")
+        self.TaskId = params.get("TaskId")
+        self.TaskName = params.get("TaskName")
+        self.TryLimit = params.get("TryLimit")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class InstanceLog(AbstractModel):
     """实例日志实体
 
     """
 
     def __init__(self):
         r"""
@@ -12047,14 +12173,89 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class InstanceLogList(AbstractModel):
+    """实例日志信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TaskId: 任务ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TaskId: str
+        :param CurRunDate: 数据时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CurRunDate: str
+        :param Tries: 重试次数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Tries: str
+        :param LastUpdate: 最后更新事件
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LastUpdate: str
+        :param BrokerIp: 节点ip
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BrokerIp: str
+        :param FileSize: 文件大小
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FileSize: str
+        :param OriginFileName: 原始文件名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OriginFileName: str
+        :param CreateTime: 创建时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreateTime: str
+        :param InstanceLogType: 实例日志类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceLogType: str
+        :param TaskName: 任务名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TaskName: str
+        :param CostTime: 耗费时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CostTime: str
+        """
+        self.TaskId = None
+        self.CurRunDate = None
+        self.Tries = None
+        self.LastUpdate = None
+        self.BrokerIp = None
+        self.FileSize = None
+        self.OriginFileName = None
+        self.CreateTime = None
+        self.InstanceLogType = None
+        self.TaskName = None
+        self.CostTime = None
+
+
+    def _deserialize(self, params):
+        self.TaskId = params.get("TaskId")
+        self.CurRunDate = params.get("CurRunDate")
+        self.Tries = params.get("Tries")
+        self.LastUpdate = params.get("LastUpdate")
+        self.BrokerIp = params.get("BrokerIp")
+        self.FileSize = params.get("FileSize")
+        self.OriginFileName = params.get("OriginFileName")
+        self.CreateTime = params.get("CreateTime")
+        self.InstanceLogType = params.get("InstanceLogType")
+        self.TaskName = params.get("TaskName")
+        self.CostTime = params.get("CostTime")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class InstanceNodeInfo(AbstractModel):
     """查询实时任务实例当前的节点信息
 
     """
 
     def __init__(self):
         r"""
@@ -12242,14 +12443,39 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class IntegrationInstanceLog(AbstractModel):
+    """实例日志信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param LogInfo: 任务日志信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LogInfo: str
+        """
+        self.LogInfo = None
+
+
+    def _deserialize(self, params):
+        self.LogInfo = params.get("LogInfo")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class IntegrationNodeDetail(AbstractModel):
     """集成节点详情
 
     """
 
     def __init__(self):
         r"""
@@ -12709,14 +12935,59 @@
         :type InLongManagerVersion: str
         :param DataProxyUrl: dataproxy url
 注意：此字段可能返回 null，表示取不到有效值。
         :type DataProxyUrl: list of str
         :param Submit: 任务版本是否已提交运维
 注意：此字段可能返回 null，表示取不到有效值。
         :type Submit: bool
+        :param InputDatasourceType: MYSQL
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InputDatasourceType: str
+        :param OutputDatasourceType: DLC
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OutputDatasourceType: str
+        :param NumRecordsIn: 读取条数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NumRecordsIn: int
+        :param NumRecordsOut: 写入条数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NumRecordsOut: int
+        :param ReaderDelay: 读取延迟
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ReaderDelay: float
+        :param NumRestarts: 重启次数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NumRestarts: int
+        :param CreateTime: 任务创建时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreateTime: str
+        :param UpdateTime: 任务更新时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UpdateTime: str
+        :param LastRunTime: 任务最后一次运行时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LastRunTime: str
+        :param StopTime: 任务停止时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StopTime: str
+        :param HasVersion: 作业是否已提交
+注意：此字段可能返回 null，表示取不到有效值。
+        :type HasVersion: bool
+        :param Locked: 任务是否被锁定
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Locked: bool
+        :param Locker: 任务锁定人
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Locker: str
+        :param RunningCu: 耗费资源量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RunningCu: float
+        :param TaskAlarmRegularList: 该任务关联的告警规则
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TaskAlarmRegularList: list of str
         """
         self.TaskName = None
         self.Description = None
         self.SyncType = None
         self.TaskType = None
         self.WorkflowId = None
         self.TaskId = None
@@ -12739,14 +13010,29 @@
         self.OfflineTaskAddEntity = None
         self.ExecutorGroupName = None
         self.InLongManagerUrl = None
         self.InLongStreamId = None
         self.InLongManagerVersion = None
         self.DataProxyUrl = None
         self.Submit = None
+        self.InputDatasourceType = None
+        self.OutputDatasourceType = None
+        self.NumRecordsIn = None
+        self.NumRecordsOut = None
+        self.ReaderDelay = None
+        self.NumRestarts = None
+        self.CreateTime = None
+        self.UpdateTime = None
+        self.LastRunTime = None
+        self.StopTime = None
+        self.HasVersion = None
+        self.Locked = None
+        self.Locker = None
+        self.RunningCu = None
+        self.TaskAlarmRegularList = None
 
 
     def _deserialize(self, params):
         self.TaskName = params.get("TaskName")
         self.Description = params.get("Description")
         self.SyncType = params.get("SyncType")
         self.TaskType = params.get("TaskType")
@@ -12798,14 +13084,29 @@
             self.OfflineTaskAddEntity._deserialize(params.get("OfflineTaskAddEntity"))
         self.ExecutorGroupName = params.get("ExecutorGroupName")
         self.InLongManagerUrl = params.get("InLongManagerUrl")
         self.InLongStreamId = params.get("InLongStreamId")
         self.InLongManagerVersion = params.get("InLongManagerVersion")
         self.DataProxyUrl = params.get("DataProxyUrl")
         self.Submit = params.get("Submit")
+        self.InputDatasourceType = params.get("InputDatasourceType")
+        self.OutputDatasourceType = params.get("OutputDatasourceType")
+        self.NumRecordsIn = params.get("NumRecordsIn")
+        self.NumRecordsOut = params.get("NumRecordsOut")
+        self.ReaderDelay = params.get("ReaderDelay")
+        self.NumRestarts = params.get("NumRestarts")
+        self.CreateTime = params.get("CreateTime")
+        self.UpdateTime = params.get("UpdateTime")
+        self.LastRunTime = params.get("LastRunTime")
+        self.StopTime = params.get("StopTime")
+        self.HasVersion = params.get("HasVersion")
+        self.Locked = params.get("Locked")
+        self.Locker = params.get("Locker")
+        self.RunningCu = params.get("RunningCu")
+        self.TaskAlarmRegularList = params.get("TaskAlarmRegularList")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -18951,14 +19252,38 @@
         :type AlarmIndicatorInfos: list of AlarmIndicatorInfo
         :param AlarmRecipientType: 告警接收人类型，0指定人员；1任务责任人
 注意：此字段可能返回 null，表示取不到有效值。
         :type AlarmRecipientType: int
         :param WeComHook: 企业微信群Hook地址，多个hook地址使用,隔开
 注意：此字段可能返回 null，表示取不到有效值。
         :type WeComHook: str
+        :param UpdateTime: 最近操作时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UpdateTime: str
+        :param OperatorUin: 最近操作人Uin
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OperatorUin: str
+        :param TaskCount: 关联任务数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TaskCount: int
+        :param MonitorType: 监控对象类型,1:所有任务,2:指定任务,3:指定责任人
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MonitorType: int
+        :param MonitorObjectIds: 监控对象列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MonitorObjectIds: list of str
+        :param LatestAlarmInstanceId: 最近一次告警的实例ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LatestAlarmInstanceId: str
+        :param LatestAlarmTime: 最近一次告警时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LatestAlarmTime: str
+        :param Description: 告警规则描述
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Description: str
         """
         self.TaskId = None
         self.RegularName = None
         self.RegularStatus = None
         self.AlarmLevel = None
         self.AlarmWay = None
         self.TaskType = None
@@ -18974,14 +19299,22 @@
         self.AlarmIndicatorDesc = None
         self.Operator = None
         self.NodeId = None
         self.NodeName = None
         self.AlarmIndicatorInfos = None
         self.AlarmRecipientType = None
         self.WeComHook = None
+        self.UpdateTime = None
+        self.OperatorUin = None
+        self.TaskCount = None
+        self.MonitorType = None
+        self.MonitorObjectIds = None
+        self.LatestAlarmInstanceId = None
+        self.LatestAlarmTime = None
+        self.Description = None
 
 
     def _deserialize(self, params):
         self.TaskId = params.get("TaskId")
         self.RegularName = params.get("RegularName")
         self.RegularStatus = params.get("RegularStatus")
         self.AlarmLevel = params.get("AlarmLevel")
@@ -19004,14 +19337,22 @@
             self.AlarmIndicatorInfos = []
             for item in params.get("AlarmIndicatorInfos"):
                 obj = AlarmIndicatorInfo()
                 obj._deserialize(item)
                 self.AlarmIndicatorInfos.append(obj)
         self.AlarmRecipientType = params.get("AlarmRecipientType")
         self.WeComHook = params.get("WeComHook")
+        self.UpdateTime = params.get("UpdateTime")
+        self.OperatorUin = params.get("OperatorUin")
+        self.TaskCount = params.get("TaskCount")
+        self.MonitorType = params.get("MonitorType")
+        self.MonitorObjectIds = params.get("MonitorObjectIds")
+        self.LatestAlarmInstanceId = params.get("LatestAlarmInstanceId")
+        self.LatestAlarmTime = params.get("LatestAlarmTime")
+        self.Description = params.get("Description")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.906/tencentcloud/__init__.py` & `tencentcloud-sdk-python-wedata-3.0.907/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-wedata-3.0.906/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO` & `tencentcloud-sdk-python-wedata-3.0.907/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-wedata
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Wedata SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.906/PKG-INFO` & `tencentcloud-sdk-python-wedata-3.0.907/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-wedata
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Wedata SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.906/setup.py` & `tencentcloud-sdk-python-wedata-3.0.907/setup.py`

 * *Files identical despite different names*

