# Comparing `tmp/tencentcloud-sdk-python-apigateway-3.0.906.tar.gz` & `tmp/tencentcloud-sdk-python-apigateway-3.0.907.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-apigateway-3.0.906.tar", last modified: Mon Jun  5 00:26:18 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-apigateway-3.0.907.tar", last modified: Tue Jun  6 02:18:27 2023, max compression
```

## Comparing `tencentcloud-sdk-python-apigateway-3.0.906.tar` & `tencentcloud-sdk-python-apigateway-3.0.907.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:26:18.000000 tencentcloud-sdk-python-apigateway-3.0.906/
--rw-r--r--   0 root         (0) root         (0)      758 2023-06-05 00:26:18.000000 tencentcloud-sdk-python-apigateway-3.0.906/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:26:18.000000 tencentcloud-sdk-python-apigateway-3.0.906/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:26:18.000000 tencentcloud-sdk-python-apigateway-3.0.906/tencentcloud/apigateway/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:26:18.000000 tencentcloud-sdk-python-apigateway-3.0.906/tencentcloud/apigateway/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:26:18.000000 tencentcloud-sdk-python-apigateway-3.0.906/tencentcloud/apigateway/v20180808/
--rw-r--r--   0 root         (0) root         (0)    95979 2023-06-05 00:26:18.000000 tencentcloud-sdk-python-apigateway-3.0.906/tencentcloud/apigateway/v20180808/apigateway_client.py
--rw-r--r--   0 root         (0) root         (0)    20869 2023-06-05 00:26:18.000000 tencentcloud-sdk-python-apigateway-3.0.906/tencentcloud/apigateway/v20180808/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:26:18.000000 tencentcloud-sdk-python-apigateway-3.0.906/tencentcloud/apigateway/v20180808/__init__.py
--rw-r--r--   0 root         (0) root         (0)   394892 2023-06-05 00:26:18.000000 tencentcloud-sdk-python-apigateway-3.0.906/tencentcloud/apigateway/v20180808/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-05 00:26:18.000000 tencentcloud-sdk-python-apigateway-3.0.906/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:26:18.000000 tencentcloud-sdk-python-apigateway-3.0.906/tencentcloud_sdk_python_apigateway.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:26:18.000000 tencentcloud-sdk-python-apigateway-3.0.906/tencentcloud_sdk_python_apigateway.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-06-05 00:26:18.000000 tencentcloud-sdk-python-apigateway-3.0.906/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-06-05 00:26:18.000000 tencentcloud-sdk-python-apigateway-3.0.906/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 00:26:18.000000 tencentcloud-sdk-python-apigateway-3.0.906/tencentcloud_sdk_python_apigateway.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-06-05 00:26:18.000000 tencentcloud-sdk-python-apigateway-3.0.906/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1020 2023-06-05 00:26:18.000000 tencentcloud-sdk-python-apigateway-3.0.906/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-05 00:26:18.000000 tencentcloud-sdk-python-apigateway-3.0.906/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/
+-rw-r--r--   0 root         (0) root         (0)      758 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud/apigateway/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud/apigateway/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud/apigateway/v20180808/
+-rw-r--r--   0 root         (0) root         (0)    95967 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud/apigateway/v20180808/apigateway_client.py
+-rw-r--r--   0 root         (0) root         (0)    20869 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud/apigateway/v20180808/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud/apigateway/v20180808/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   402836 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud/apigateway/v20180808/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud_sdk_python_apigateway.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud_sdk_python_apigateway.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud_sdk_python_apigateway.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/setup.cfg
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.906/README.rst` & `tencentcloud-sdk-python-apigateway-3.0.907/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.906/tencentcloud/apigateway/v20180808/apigateway_client.py` & `tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud/apigateway/v20180808/apigateway_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,15 +350,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateUpstream(self, request):
-        """用于创建创建后端通道
+        """用于创建后端通道
 
         :param request: Request instance for CreateUpstream.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.CreateUpstreamRequest`
         :rtype: :class:`tencentcloud.apigateway.v20180808.models.CreateUpstreamResponse`
 
         """
         try:
@@ -1001,15 +1001,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeExclusiveInstances(self, request):
-        """本接口（DescribeExclusiveInstances）用于查询独享实例列表信息。​
+        """本接口（DescribeExclusiveInstances）用于查询独享实例列表信息。
 
         :param request: Request instance for DescribeExclusiveInstances.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribeExclusiveInstancesRequest`
         :rtype: :class:`tencentcloud.apigateway.v20180808.models.DescribeExclusiveInstancesResponse`
 
         """
         try:
@@ -2253,15 +2253,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def UpdateService(self, request):
-        """本接口（UpdateService）用于从服务发布的环境中运行版本切换到特定版本。用户在使用 API 网关创建服务并发布服务到某个环境后，多因为开发过程会产生多个版本，此时可调用本接口。
+        """本接口（UpdateService）用于从服务发布的环境中运行版本切换到特定版本。用户在使用 API 网关创建服务并发布服务到某个环境后，多因开发过程会产生多个版本，此时可调用本接口。
 
         :param request: Request instance for UpdateService.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.UpdateServiceRequest`
         :rtype: :class:`tencentcloud.apigateway.v20180808.models.UpdateServiceResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.906/tencentcloud/apigateway/v20180808/errorcodes.py` & `tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud/apigateway/v20180808/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.906/tencentcloud/apigateway/v20180808/models.py` & `tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud/apigateway/v20180808/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -428,14 +428,15 @@
     def __init__(self):
         r"""
         :param ServiceId: 服务唯一ID。
         :type ServiceId: str
         :param ApiId: API唯一ID。
         :type ApiId: str
         :param ApiDesc: API描述
+注意：此字段可能返回 null，表示取不到有效值。
         :type ApiDesc: str
         :param Path: API PATH。
         :type Path: str
         :param Method: API METHOD。
         :type Method: str
         :param CreatedTime: 服务创建时间。
         :type CreatedTime: str
@@ -602,15 +603,15 @@
 注意：此字段可能返回 null，表示取不到有效值。
         :type ServiceType: str
         :param ServiceConfig: API 的后端服务配置。
 注意：此字段可能返回 null，表示取不到有效值。
         :type ServiceConfig: :class:`tencentcloud.apigateway.v20180808.models.ServiceConfig`
         :param ServiceParameters: API的后端服务参数。
 注意：此字段可能返回 null，表示取不到有效值。
-        :type ServiceParameters: list of ServiceParameter
+        :type ServiceParameters: list of DescribeApiResultServiceParametersInfo
         :param ConstantParameters: 常量参数。
 注意：此字段可能返回 null，表示取不到有效值。
         :type ConstantParameters: list of ConstantParameter
         :param ServiceMockReturnMessage: API 的后端 Mock 返回信息。如果 ServiceType 是 Mock，则此参数必传。
 注意：此字段可能返回 null，表示取不到有效值。
         :type ServiceMockReturnMessage: str
         :param ServiceScfFunctionName: scf 函数名称。当后端类型是SCF时生效。
@@ -779,15 +780,15 @@
         self.ServiceType = params.get("ServiceType")
         if params.get("ServiceConfig") is not None:
             self.ServiceConfig = ServiceConfig()
             self.ServiceConfig._deserialize(params.get("ServiceConfig"))
         if params.get("ServiceParameters") is not None:
             self.ServiceParameters = []
             for item in params.get("ServiceParameters"):
-                obj = ServiceParameter()
+                obj = DescribeApiResultServiceParametersInfo()
                 obj._deserialize(item)
                 self.ServiceParameters.append(obj)
         if params.get("ConstantParameters") is not None:
             self.ConstantParameters = []
             for item in params.get("ConstantParameters"):
                 obj = ConstantParameter()
                 obj._deserialize(item)
@@ -1115,47 +1116,14 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class ApisStatus(AbstractModel):
-    """描述api列表状态
-
-    """
-
-    def __init__(self):
-        r"""
-        :param TotalCount: 符合条件的 API 接口数量。
-        :type TotalCount: int
-        :param ApiIdStatusSet: API 接口列表。
-        :type ApiIdStatusSet: list of DesApisStatus
-        """
-        self.TotalCount = None
-        self.ApiIdStatusSet = None
-
-
-    def _deserialize(self, params):
-        self.TotalCount = params.get("TotalCount")
-        if params.get("ApiIdStatusSet") is not None:
-            self.ApiIdStatusSet = []
-            for item in params.get("ApiIdStatusSet"):
-                obj = DesApisStatus()
-                obj._deserialize(item)
-                self.ApiIdStatusSet.append(obj)
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
 class AttachPluginRequest(AbstractModel):
     """AttachPlugin请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1796,26 +1764,21 @@
 class BindSubDomainResponse(AbstractModel):
     """BindSubDomain返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Result: 绑定操作是否成功。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Result: bool
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
-        self.Result = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
-        self.Result = params.get("Result")
         self.RequestId = params.get("RequestId")
 
 
 class BuildAPIDocRequest(AbstractModel):
     """BuildAPIDoc请求参数结构体
 
     """
@@ -1864,20 +1827,24 @@
     """常量参数
 
     """
 
     def __init__(self):
         r"""
         :param Name: 常量参数名称。只有 ServiceType 是 HTTP 才会用到此参数。
+注意：此字段可能返回 null，表示取不到有效值。
         :type Name: str
         :param Desc: 常量参数描述。只有 ServiceType 是 HTTP 才会用到此参数。
+注意：此字段可能返回 null，表示取不到有效值。
         :type Desc: str
         :param Position: 常量参数位置。只有 ServiceType 是 HTTP 才会用到此参数。
+注意：此字段可能返回 null，表示取不到有效值。
         :type Position: str
         :param DefaultValue: 常量参数默认值。只有 ServiceType 是 HTTP 才会用到此参数。
+注意：此字段可能返回 null，表示取不到有效值。
         :type DefaultValue: str
         """
         self.Name = None
         self.Desc = None
         self.Position = None
         self.DefaultValue = None
 
@@ -2395,29 +2362,69 @@
 
     """
 
     def __init__(self):
         r"""
         :param Result: api信息
 注意：此字段可能返回 null，表示取不到有效值。
-        :type Result: :class:`tencentcloud.apigateway.v20180808.models.CreateApiRsp`
+        :type Result: :class:`tencentcloud.apigateway.v20180808.models.CreateApiResultInfo`
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.Result = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         if params.get("Result") is not None:
-            self.Result = CreateApiRsp()
+            self.Result = CreateApiResultInfo()
             self.Result._deserialize(params.get("Result"))
         self.RequestId = params.get("RequestId")
 
 
+class CreateApiResultInfo(AbstractModel):
+    """创建api返回
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ApiId: api id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ApiId: str
+        :param Path: 路径
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Path: str
+        :param Method: 请求方法
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Method: str
+        :param CreatedTime: 创建时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreatedTime: str
+        """
+        self.ApiId = None
+        self.Path = None
+        self.Method = None
+        self.CreatedTime = None
+
+
+    def _deserialize(self, params):
+        self.ApiId = params.get("ApiId")
+        self.Path = params.get("Path")
+        self.Method = params.get("Method")
+        self.CreatedTime = params.get("CreatedTime")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class CreateApiRsp(AbstractModel):
     """创建api返回
 
     """
 
     def __init__(self):
         r"""
@@ -4241,14 +4248,64 @@
     def _deserialize(self, params):
         if params.get("Result") is not None:
             self.Result = ApiInfo()
             self.Result._deserialize(params.get("Result"))
         self.RequestId = params.get("RequestId")
 
 
+class DescribeApiResultServiceParametersInfo(AbstractModel):
+    """ServiceParameter
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Name: API的后端服务参数名称。只有ServiceType是HTTP才会用到此参数。前后端参数名称可不同。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Name: str
+        :param Position: API 的后端服务参数位置，如 head。只有 ServiceType 是 HTTP 才会用到此参数。前后端参数位置可配置不同。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Position: str
+        :param RelevantRequestParameterPosition: API 的后端服务参数对应的前端参数位置，如 head。只有 ServiceType 是 HTTP 才会用到此参数。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RelevantRequestParameterPosition: str
+        :param RelevantRequestParameterName: API 的后端服务参数对应的前端参数名称。只有 ServiceType 是 HTTP 才会用到此参数。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RelevantRequestParameterName: str
+        :param DefaultValue: API 的后端服务参数默认值。只有 ServiceType 是 HTTP 才会用到此参数。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DefaultValue: str
+        :param RelevantRequestParameterDesc: API 的后端服务参数备注。只有 ServiceType 是 HTTP 才会用到此参数。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RelevantRequestParameterDesc: str
+        """
+        self.Name = None
+        self.Position = None
+        self.RelevantRequestParameterPosition = None
+        self.RelevantRequestParameterName = None
+        self.DefaultValue = None
+        self.RelevantRequestParameterDesc = None
+
+
+    def _deserialize(self, params):
+        self.Name = params.get("Name")
+        self.Position = params.get("Position")
+        self.RelevantRequestParameterPosition = params.get("RelevantRequestParameterPosition")
+        self.RelevantRequestParameterName = params.get("RelevantRequestParameterName")
+        self.DefaultValue = params.get("DefaultValue")
+        self.RelevantRequestParameterDesc = params.get("RelevantRequestParameterDesc")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class DescribeApiUsagePlanRequest(AbstractModel):
     """DescribeApiUsagePlan请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -4346,29 +4403,53 @@
     """DescribeApisStatus返回参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param Result: API 详情列表。
-        :type Result: :class:`tencentcloud.apigateway.v20180808.models.ApisStatus`
+        :type Result: :class:`tencentcloud.apigateway.v20180808.models.DescribeApisStatusResultInfo`
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.Result = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         if params.get("Result") is not None:
-            self.Result = ApisStatus()
+            self.Result = DescribeApisStatusResultInfo()
             self.Result._deserialize(params.get("Result"))
         self.RequestId = params.get("RequestId")
 
 
+class DescribeApisStatusResultInfo(AbstractModel):
+    """描述api列表状态
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 符合条件的 API 接口数量。
+        :type TotalCount: int
+        """
+        self.TotalCount = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class DescribeExclusiveInstanceDetailRequest(AbstractModel):
     """DescribeExclusiveInstanceDetail请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -4453,29 +4534,35 @@
     """DescribeExclusiveInstances返回参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param Result: 独享实例列表查询结果
-        :type Result: :class:`tencentcloud.apigateway.v20180808.models.InstanceInfo`
+        :type Result: :class:`tencentcloud.apigateway.v20180808.models.DescribeExclusiveInstancesResult`
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.Result = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         if params.get("Result") is not None:
-            self.Result = InstanceInfo()
+            self.Result = DescribeExclusiveInstancesResult()
             self.Result._deserialize(params.get("Result"))
         self.RequestId = params.get("RequestId")
 
 
+class DescribeExclusiveInstancesResult(AbstractModel):
+    """数据结构
+
+    """
+
+
 class DescribeExclusiveInstancesStatusRequest(AbstractModel):
     """DescribeExclusiveInstancesStatus请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -5494,14 +5581,44 @@
     def _deserialize(self, params):
         if params.get("Result") is not None:
             self.Result = ServiceReleaseVersion()
             self.Result._deserialize(params.get("Result"))
         self.RequestId = params.get("RequestId")
 
 
+class DescribeServiceReleaseVersionResultVersionListInfo(AbstractModel):
+    """服务发布列表详情
+
+    """
+
+    def __init__(self):
+        r"""
+        :param VersionName: 版本号。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VersionName: str
+        :param VersionDesc: 版本描述。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VersionDesc: str
+        """
+        self.VersionName = None
+        self.VersionDesc = None
+
+
+    def _deserialize(self, params):
+        self.VersionName = params.get("VersionName")
+        self.VersionDesc = params.get("VersionDesc")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class DescribeServiceRequest(AbstractModel):
     """DescribeService请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -6613,27 +6730,22 @@
 
     def __init__(self):
         r"""
         :param EnvironmentName: 环境名
         :type EnvironmentName: str
         :param Quota: 限流值
         :type Quota: int
-        :param MaxQuota: 限流最大值
-注意：此字段可能返回 null，表示取不到有效值。
-        :type MaxQuota: int
         """
         self.EnvironmentName = None
         self.Quota = None
-        self.MaxQuota = None
 
 
     def _deserialize(self, params):
         self.EnvironmentName = params.get("EnvironmentName")
         self.Quota = params.get("Quota")
-        self.MaxQuota = params.get("MaxQuota")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -6774,20 +6886,24 @@
     """健康检查配置，包括TsfHealthCheckConf和TargetServicesHealthCheckConf
 
     """
 
     def __init__(self):
         r"""
         :param IsHealthCheck: 是否开启健康检查。
+注意：此字段可能返回 null，表示取不到有效值。
         :type IsHealthCheck: bool
         :param RequestVolumeThreshold: 健康检查阈值。
+注意：此字段可能返回 null，表示取不到有效值。
         :type RequestVolumeThreshold: int
         :param SleepWindowInMilliseconds: 窗口大小。
+注意：此字段可能返回 null，表示取不到有效值。
         :type SleepWindowInMilliseconds: int
         :param ErrorThresholdPercentage: 阈值百分比。
+注意：此字段可能返回 null，表示取不到有效值。
         :type ErrorThresholdPercentage: int
         """
         self.IsHealthCheck = None
         self.RequestVolumeThreshold = None
         self.SleepWindowInMilliseconds = None
         self.ErrorThresholdPercentage = None
 
@@ -8447,29 +8563,116 @@
 
     """
 
     def __init__(self):
         r"""
         :param Result: 返回修改后的后端通道信息
 注意：此字段可能返回 null，表示取不到有效值。
-        :type Result: :class:`tencentcloud.apigateway.v20180808.models.UpstreamInfo`
+        :type Result: :class:`tencentcloud.apigateway.v20180808.models.ModifyUpstreamResultInfo`
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.Result = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         if params.get("Result") is not None:
-            self.Result = UpstreamInfo()
+            self.Result = ModifyUpstreamResultInfo()
             self.Result._deserialize(params.get("Result"))
         self.RequestId = params.get("RequestId")
 
 
+class ModifyUpstreamResultInfo(AbstractModel):
+    """后端通道详细信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param UpstreamId: 后端通道唯一ID
+        :type UpstreamId: str
+        :param UpstreamName: 后端通道名字
+        :type UpstreamName: str
+        :param UpstreamDescription: 后端通道描述
+        :type UpstreamDescription: str
+        :param Scheme: 后端协议，取值范围：HTTP, HTTPS
+        :type Scheme: str
+        :param Algorithm: 负载均衡算法，取值范围：ROUND_ROBIN
+        :type Algorithm: str
+        :param UniqVpcId: VPC唯一ID
+        :type UniqVpcId: str
+        :param Retries: 请求重试次数
+        :type Retries: int
+        :param Nodes: 后端节点
+        :type Nodes: list of UpstreamNode
+        :param CreatedTime: 创建时间
+        :type CreatedTime: str
+        :param HealthChecker: 健康检查配置
+注意：此字段可能返回 null，表示取不到有效值。
+        :type HealthChecker: :class:`tencentcloud.apigateway.v20180808.models.UpstreamHealthChecker`
+        :param UpstreamType: 后端的类型，取值范围：IP_PORT, K8S
+        :type UpstreamType: str
+        :param K8sServices: K8S容器服务配置
+注意：此字段可能返回 null，表示取不到有效值。
+        :type K8sServices: list of K8sService
+        :param UpstreamHost: 网关转发给后端的Host请求头
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UpstreamHost: str
+        """
+        self.UpstreamId = None
+        self.UpstreamName = None
+        self.UpstreamDescription = None
+        self.Scheme = None
+        self.Algorithm = None
+        self.UniqVpcId = None
+        self.Retries = None
+        self.Nodes = None
+        self.CreatedTime = None
+        self.HealthChecker = None
+        self.UpstreamType = None
+        self.K8sServices = None
+        self.UpstreamHost = None
+
+
+    def _deserialize(self, params):
+        self.UpstreamId = params.get("UpstreamId")
+        self.UpstreamName = params.get("UpstreamName")
+        self.UpstreamDescription = params.get("UpstreamDescription")
+        self.Scheme = params.get("Scheme")
+        self.Algorithm = params.get("Algorithm")
+        self.UniqVpcId = params.get("UniqVpcId")
+        self.Retries = params.get("Retries")
+        if params.get("Nodes") is not None:
+            self.Nodes = []
+            for item in params.get("Nodes"):
+                obj = UpstreamNode()
+                obj._deserialize(item)
+                self.Nodes.append(obj)
+        self.CreatedTime = params.get("CreatedTime")
+        if params.get("HealthChecker") is not None:
+            self.HealthChecker = UpstreamHealthChecker()
+            self.HealthChecker._deserialize(params.get("HealthChecker"))
+        self.UpstreamType = params.get("UpstreamType")
+        if params.get("K8sServices") is not None:
+            self.K8sServices = []
+            for item in params.get("K8sServices"):
+                obj = K8sService()
+                obj._deserialize(item)
+                self.K8sServices.append(obj)
+        self.UpstreamHost = params.get("UpstreamHost")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class ModifyUsagePlanRequest(AbstractModel):
     """ModifyUsagePlan请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -9507,26 +9710,26 @@
     def __init__(self):
         r"""
         :param TotalCount: 发布版本总数量。
 注意：此字段可能返回 null，表示取不到有效值。
         :type TotalCount: int
         :param VersionList: 发布版本列表。
 注意：此字段可能返回 null，表示取不到有效值。
-        :type VersionList: list of ServiceReleaseHistoryInfo
+        :type VersionList: list of DescribeServiceReleaseVersionResultVersionListInfo
         """
         self.TotalCount = None
         self.VersionList = None
 
 
     def _deserialize(self, params):
         self.TotalCount = params.get("TotalCount")
         if params.get("VersionList") is not None:
             self.VersionList = []
             for item in params.get("VersionList"):
-                obj = ServiceReleaseHistoryInfo()
+                obj = DescribeServiceReleaseVersionResultVersionListInfo()
                 obj._deserialize(item)
                 self.VersionList.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
@@ -10498,14 +10701,15 @@
         :param Environment: 环境名称。
         :type Environment: str
         :param UsagePlanId: 使用计划唯一ID。
         :type UsagePlanId: str
         :param UsagePlanName: 使用计划名称。
         :type UsagePlanName: str
         :param UsagePlanDesc: 使用计划描述。
+注意：此字段可能返回 null，表示取不到有效值。
         :type UsagePlanDesc: str
         :param MaxRequestNumPreSec: 使用计划qps，-1表示没有限制。
         :type MaxRequestNumPreSec: int
         :param CreatedTime: 使用计划时间。
         :type CreatedTime: str
         :param ModifiedTime: 使用计划修改时间。
         :type ModifiedTime: str
@@ -10763,26 +10967,20 @@
         :type UsagePlanId: str
         :param UsagePlanName: 使用计划名称。
 注意：此字段可能返回 null，表示取不到有效值。
         :type UsagePlanName: str
         :param UsagePlanDesc: 使用计划描述。
 注意：此字段可能返回 null，表示取不到有效值。
         :type UsagePlanDesc: str
-        :param InitQuota: 初始化调用次数。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type InitQuota: int
         :param MaxRequestNumPreSec: 每秒请求限制数。
 注意：此字段可能返回 null，表示取不到有效值。
         :type MaxRequestNumPreSec: int
         :param MaxRequestNum: 最大调用次数。
 注意：此字段可能返回 null，表示取不到有效值。
         :type MaxRequestNum: int
-        :param IsHide: 是否隐藏。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type IsHide: int
         :param CreatedTime: 创建时间。按照 ISO8601 标准表示，并且使用 UTC 时间。格式为：YYYY-MM-DDThh:mm:ssZ。
 注意：此字段可能返回 null，表示取不到有效值。
         :type CreatedTime: str
         :param ModifiedTime: 最后修改时间。按照 ISO8601 标准表示，并且使用 UTC 时间。格式为：YYYY-MM-DDThh:mm:ssZ。
 注意：此字段可能返回 null，表示取不到有效值。
         :type ModifiedTime: str
         :param BindSecretIdTotalCount: 绑定密钥的数量。
@@ -10797,34 +10995,30 @@
         :param BindEnvironments: 绑定环境详情。
 注意：此字段可能返回 null，表示取不到有效值。
         :type BindEnvironments: list of UsagePlanBindEnvironment
         """
         self.UsagePlanId = None
         self.UsagePlanName = None
         self.UsagePlanDesc = None
-        self.InitQuota = None
         self.MaxRequestNumPreSec = None
         self.MaxRequestNum = None
-        self.IsHide = None
         self.CreatedTime = None
         self.ModifiedTime = None
         self.BindSecretIdTotalCount = None
         self.BindSecretIds = None
         self.BindEnvironmentTotalCount = None
         self.BindEnvironments = None
 
 
     def _deserialize(self, params):
         self.UsagePlanId = params.get("UsagePlanId")
         self.UsagePlanName = params.get("UsagePlanName")
         self.UsagePlanDesc = params.get("UsagePlanDesc")
-        self.InitQuota = params.get("InitQuota")
         self.MaxRequestNumPreSec = params.get("MaxRequestNumPreSec")
         self.MaxRequestNum = params.get("MaxRequestNum")
-        self.IsHide = params.get("IsHide")
         self.CreatedTime = params.get("CreatedTime")
         self.ModifiedTime = params.get("ModifiedTime")
         self.BindSecretIdTotalCount = params.get("BindSecretIdTotalCount")
         self.BindSecretIds = params.get("BindSecretIds")
         self.BindEnvironmentTotalCount = params.get("BindEnvironmentTotalCount")
         if params.get("BindEnvironments") is not None:
             self.BindEnvironments = []
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.906/tencentcloud/__init__.py` & `tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-apigateway-3.0.906/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.906/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO` & `tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-apigateway
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Apigateway SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.906/PKG-INFO` & `tencentcloud-sdk-python-apigateway-3.0.907/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-apigateway
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Apigateway SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.906/setup.py` & `tencentcloud-sdk-python-apigateway-3.0.907/setup.py`

 * *Files identical despite different names*

