# Comparing `tmp/tencentcloud-sdk-python-tbp-3.0.906.tar.gz` & `tmp/tencentcloud-sdk-python-tbp-3.0.907.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tbp-3.0.906.tar", last modified: Mon Jun  5 00:42:38 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tbp-3.0.907.tar", last modified: Tue Jun  6 02:35:07 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tbp-3.0.906.tar` & `tencentcloud-sdk-python-tbp-3.0.907.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud_sdk_python_tbp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud_sdk_python_tbp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud_sdk_python_tbp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud_sdk_python_tbp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud_sdk_python_tbp.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190311/
--rw-r--r--   0 root         (0) root         (0)     1554 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190311/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190311/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14368 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190311/models.py
--rw-r--r--   0 root         (0) root         (0)     4420 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190311/tbp_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190627/
--rw-r--r--   0 root         (0) root         (0)     1189 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190627/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190627/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13544 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190627/models.py
--rw-r--r--   0 root         (0) root         (0)     2682 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190627/tbp_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:35:07.000000 tencentcloud-sdk-python-tbp-3.0.907/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-06 02:35:07.000000 tencentcloud-sdk-python-tbp-3.0.907/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:35:07.000000 tencentcloud-sdk-python-tbp-3.0.907/tencentcloud_sdk_python_tbp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:35:07.000000 tencentcloud-sdk-python-tbp-3.0.907/tencentcloud_sdk_python_tbp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-06-06 02:35:07.000000 tencentcloud-sdk-python-tbp-3.0.907/tencentcloud_sdk_python_tbp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-06 02:35:07.000000 tencentcloud-sdk-python-tbp-3.0.907/tencentcloud_sdk_python_tbp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:35:07.000000 tencentcloud-sdk-python-tbp-3.0.907/tencentcloud_sdk_python_tbp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:35:07.000000 tencentcloud-sdk-python-tbp-3.0.907/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:35:07.000000 tencentcloud-sdk-python-tbp-3.0.907/tencentcloud/tbp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:35:07.000000 tencentcloud-sdk-python-tbp-3.0.907/tencentcloud/tbp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:35:07.000000 tencentcloud-sdk-python-tbp-3.0.907/tencentcloud/tbp/v20190311/
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-06-06 02:35:07.000000 tencentcloud-sdk-python-tbp-3.0.907/tencentcloud/tbp/v20190311/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:35:07.000000 tencentcloud-sdk-python-tbp-3.0.907/tencentcloud/tbp/v20190311/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17397 2023-06-06 02:35:07.000000 tencentcloud-sdk-python-tbp-3.0.907/tencentcloud/tbp/v20190311/models.py
+-rw-r--r--   0 root         (0) root         (0)     4420 2023-06-06 02:35:07.000000 tencentcloud-sdk-python-tbp-3.0.907/tencentcloud/tbp/v20190311/tbp_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:35:07.000000 tencentcloud-sdk-python-tbp-3.0.907/tencentcloud/tbp/v20190627/
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-06-06 02:35:07.000000 tencentcloud-sdk-python-tbp-3.0.907/tencentcloud/tbp/v20190627/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:35:07.000000 tencentcloud-sdk-python-tbp-3.0.907/tencentcloud/tbp/v20190627/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13728 2023-06-06 02:35:07.000000 tencentcloud-sdk-python-tbp-3.0.907/tencentcloud/tbp/v20190627/models.py
+-rw-r--r--   0 root         (0) root         (0)     2682 2023-06-06 02:35:07.000000 tencentcloud-sdk-python-tbp-3.0.907/tencentcloud/tbp/v20190627/tbp_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:35:07.000000 tencentcloud-sdk-python-tbp-3.0.907/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-06 02:35:07.000000 tencentcloud-sdk-python-tbp-3.0.907/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-06 02:35:07.000000 tencentcloud-sdk-python-tbp-3.0.907/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:35:07.000000 tencentcloud-sdk-python-tbp-3.0.907/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tbp-3.0.906/README.rst` & `tencentcloud-sdk-python-tbp-3.0.907/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbp-3.0.906/tencentcloud_sdk_python_tbp.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-tbp-3.0.907/tencentcloud_sdk_python_tbp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbp-3.0.906/tencentcloud_sdk_python_tbp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tbp-3.0.907/tencentcloud_sdk_python_tbp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tbp
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Tbp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190311/errorcodes.py` & `tencentcloud-sdk-python-tbp-3.0.907/tencentcloud/tbp/v20190311/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190311/models.py` & `tencentcloud-sdk-python-tbp-3.0.907/tencentcloud/tbp/v20190627/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,169 +14,78 @@
 # limitations under the License.
 
 import warnings
 
 from tencentcloud.common.abstract_model import AbstractModel
 
 
-class CreateBotRequest(AbstractModel):
-    """CreateBot请求参数结构体
+class Group(AbstractModel):
+    """Group是消息组的具体定义，当前包含ContentType、Url、Content三个字段。其中，具体的ContentType字段定义，参考互联网MIME类型标准。
 
     """
 
     def __init__(self):
         r"""
-        :param BotName: 机器人名称
-        :type BotName: str
-        :param BotCnName: 机器人中文名称
-        :type BotCnName: str
+        :param ContentType: 消息类型参考互联网MIME类型标准，当前仅支持"text/plain"。
+        :type ContentType: str
+        :param Url: 返回内容以链接形式提供。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Url: str
+        :param Content: 普通文本。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Content: str
         """
-        self.BotName = None
-        self.BotCnName = None
+        self.ContentType = None
+        self.Url = None
+        self.Content = None
 
 
     def _deserialize(self, params):
-        self.BotName = params.get("BotName")
-        self.BotCnName = params.get("BotCnName")
+        self.ContentType = params.get("ContentType")
+        self.Url = params.get("Url")
+        self.Content = params.get("Content")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class CreateBotResponse(AbstractModel):
-    """CreateBot返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param TaskRequestId: 任务ID
-        :type TaskRequestId: str
-        :param Msg: 任务信息
-        :type Msg: str
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self.TaskRequestId = None
-        self.Msg = None
-        self.RequestId = None
-
-
-    def _deserialize(self, params):
-        self.TaskRequestId = params.get("TaskRequestId")
-        self.Msg = params.get("Msg")
-        self.RequestId = params.get("RequestId")
-
-
-class ResetRequest(AbstractModel):
-    """Reset请求参数结构体
+class ResponseMessage(AbstractModel):
+    """从TBP-RTS服务v1.3版本起，机器人以消息组列表的形式响应，消息组列表GroupList包含多组消息，用户根据需要对部分或全部消息组进行组合使用。
 
     """
 
     def __init__(self):
         r"""
-        :param BotId: 机器人标识
-        :type BotId: str
-        :param UserId: 子账户id，每个终端对应一个
-        :type UserId: str
-        :param BotVersion: 机器人版本号。BotVersion/BotEnv二选一：二者均填，仅BotVersion有效；二者均不填，默认BotEnv=dev
-        :type BotVersion: str
-        :param BotEnv: 机器人环境{dev:测试;release:线上}。BotVersion/BotEnv二选一：二者均填，仅BotVersion有效；二者均不填，默认BotEnv=dev
-        :type BotEnv: str
+        :param GroupList: 消息组列表。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type GroupList: list of Group
         """
-        self.BotId = None
-        self.UserId = None
-        self.BotVersion = None
-        self.BotEnv = None
+        self.GroupList = None
 
 
     def _deserialize(self, params):
-        self.BotId = params.get("BotId")
-        self.UserId = params.get("UserId")
-        self.BotVersion = params.get("BotVersion")
-        self.BotEnv = params.get("BotEnv")
+        if params.get("GroupList") is not None:
+            self.GroupList = []
+            for item in params.get("GroupList"):
+                obj = Group()
+                obj._deserialize(item)
+                self.GroupList.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class ResetResponse(AbstractModel):
-    """Reset返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param DialogStatus: 当前会话状态。取值:"start"/"continue"/"complete"
-注意：此字段可能返回 null，表示取不到有效值。
-        :type DialogStatus: str
-        :param BotName: 匹配到的机器人名称
-注意：此字段可能返回 null，表示取不到有效值。
-        :type BotName: str
-        :param IntentName: 匹配到的意图名称
-注意：此字段可能返回 null，表示取不到有效值。
-        :type IntentName: str
-        :param ResponseText: 机器人回答
-        :type ResponseText: str
-        :param SlotInfoList: 语义解析的槽位结果列表
-注意：此字段可能返回 null，表示取不到有效值。
-        :type SlotInfoList: list of SlotInfo
-        :param SessionAttributes: 透传字段
-注意：此字段可能返回 null，表示取不到有效值。
-        :type SessionAttributes: str
-        :param Question: 用户说法。该说法是用户原生说法或ASR识别结果，未经过语义优化
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Question: str
-        :param WaveUrl: tts合成pcm音频存储链接。仅当请求参数NeedTts=true时返回
-注意：此字段可能返回 null，表示取不到有效值。
-        :type WaveUrl: str
-        :param WaveData: tts合成的pcm音频。二进制数组经过base64编码(暂时不返回)
-注意：此字段可能返回 null，表示取不到有效值。
-        :type WaveData: str
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self.DialogStatus = None
-        self.BotName = None
-        self.IntentName = None
-        self.ResponseText = None
-        self.SlotInfoList = None
-        self.SessionAttributes = None
-        self.Question = None
-        self.WaveUrl = None
-        self.WaveData = None
-        self.RequestId = None
-
-
-    def _deserialize(self, params):
-        self.DialogStatus = params.get("DialogStatus")
-        self.BotName = params.get("BotName")
-        self.IntentName = params.get("IntentName")
-        self.ResponseText = params.get("ResponseText")
-        if params.get("SlotInfoList") is not None:
-            self.SlotInfoList = []
-            for item in params.get("SlotInfoList"):
-                obj = SlotInfo()
-                obj._deserialize(item)
-                self.SlotInfoList.append(obj)
-        self.SessionAttributes = params.get("SessionAttributes")
-        self.Question = params.get("Question")
-        self.WaveUrl = params.get("WaveUrl")
-        self.WaveData = params.get("WaveData")
-        self.RequestId = params.get("RequestId")
-
-
 class SlotInfo(AbstractModel):
     """槽位信息
 
     """
 
     def __init__(self):
         r"""
@@ -208,36 +117,44 @@
 
     """
 
     def __init__(self):
         r"""
         :param BotId: 机器人标识，用于定义抽象机器人。
         :type BotId: str
+        :param BotEnv: 机器人版本，取值"dev"或"release"，{调试版本：dev；线上版本：release}。
+        :type BotEnv: str
         :param TerminalId: 终端标识，每个终端(或线程)对应一个，区分并发多用户。
         :type TerminalId: str
         :param InputText: 请求的文本。
         :type InputText: str
-        :param BotEnv: 机器人版本，取值"dev"或"release"，{调试版本：dev；线上版本：release}。
-        :type BotEnv: str
         :param SessionAttributes: 透传字段，透传给用户自定义的WebService服务。
         :type SessionAttributes: str
+        :param PlatformType: 平台类型，{小程序：MiniProgram；小微：XiaoWei；公众号：OfficialAccount；企业微信: WXWork}。
+        :type PlatformType: str
+        :param PlatformId: 当PlatformType为微信公众号或企业微信时，传递对应微信公众号或企业微信的唯一标识
+        :type PlatformId: str
         """
         self.BotId = None
+        self.BotEnv = None
         self.TerminalId = None
         self.InputText = None
-        self.BotEnv = None
         self.SessionAttributes = None
+        self.PlatformType = None
+        self.PlatformId = None
 
 
     def _deserialize(self, params):
         self.BotId = params.get("BotId")
+        self.BotEnv = params.get("BotEnv")
         self.TerminalId = params.get("TerminalId")
         self.InputText = params.get("InputText")
-        self.BotEnv = params.get("BotEnv")
         self.SessionAttributes = params.get("SessionAttributes")
+        self.PlatformType = params.get("PlatformType")
+        self.PlatformId = params.get("PlatformId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -261,29 +178,36 @@
         :type IntentName: str
         :param SlotInfoList: 槽位信息。
 注意：此字段可能返回 null，表示取不到有效值。
         :type SlotInfoList: list of SlotInfo
         :param InputText: 原始的用户说法。
 注意：此字段可能返回 null，表示取不到有效值。
         :type InputText: str
+        :param ResponseMessage: 机器人应答。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ResponseMessage: :class:`tencentcloud.tbp.v20190627.models.ResponseMessage`
         :param SessionAttributes: 透传字段，由用户自定义的WebService服务返回。
 注意：此字段可能返回 null，表示取不到有效值。
         :type SessionAttributes: str
-        :param ResponseText: 机器人对话的应答文本。
+        :param ResultType: 结果类型 {中间逻辑出错:0; 任务型机器人:1; 问答型机器人:2; 闲聊型机器人:3; 未匹配上，返回预设兜底话术:5; 未匹配上，返回相似问题列表:6}。
 注意：此字段可能返回 null，表示取不到有效值。
+        :type ResultType: str
+        :param ResponseText: 机器人对话的应答文本。	
         :type ResponseText: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.DialogStatus = None
         self.BotName = None
         self.IntentName = None
         self.SlotInfoList = None
         self.InputText = None
+        self.ResponseMessage = None
         self.SessionAttributes = None
+        self.ResultType = None
         self.ResponseText = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.DialogStatus = params.get("DialogStatus")
         self.BotName = params.get("BotName")
@@ -291,42 +215,54 @@
         if params.get("SlotInfoList") is not None:
             self.SlotInfoList = []
             for item in params.get("SlotInfoList"):
                 obj = SlotInfo()
                 obj._deserialize(item)
                 self.SlotInfoList.append(obj)
         self.InputText = params.get("InputText")
+        if params.get("ResponseMessage") is not None:
+            self.ResponseMessage = ResponseMessage()
+            self.ResponseMessage._deserialize(params.get("ResponseMessage"))
         self.SessionAttributes = params.get("SessionAttributes")
+        self.ResultType = params.get("ResultType")
         self.ResponseText = params.get("ResponseText")
         self.RequestId = params.get("RequestId")
 
 
 class TextResetRequest(AbstractModel):
     """TextReset请求参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param BotId: 机器人标识，用于定义抽象机器人。
         :type BotId: str
-        :param TerminalId: 终端标识，每个终端(或线程)对应一个，区分并发多用户。
-        :type TerminalId: str
         :param BotEnv: 机器人版本，取值"dev"或"release"，{调试版本：dev；线上版本：release}。
         :type BotEnv: str
+        :param TerminalId: 终端标识，每个终端(或线程)对应一个，区分并发多用户。
+        :type TerminalId: str
+        :param PlatformType: 平台类型，{小程序：MiniProgram；小微：XiaoWei；公众号：OfficialAccount；企业微信: WXWork}。
+        :type PlatformType: str
+        :param PlatformId: 当PlatformType为微信公众号或企业微信时，传递对应微信公众号或企业微信的唯一标识
+        :type PlatformId: str
         """
         self.BotId = None
-        self.TerminalId = None
         self.BotEnv = None
+        self.TerminalId = None
+        self.PlatformType = None
+        self.PlatformId = None
 
 
     def _deserialize(self, params):
         self.BotId = params.get("BotId")
-        self.TerminalId = params.get("TerminalId")
         self.BotEnv = params.get("BotEnv")
+        self.TerminalId = params.get("TerminalId")
+        self.PlatformType = params.get("PlatformType")
+        self.PlatformId = params.get("PlatformId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -335,44 +271,52 @@
 class TextResetResponse(AbstractModel):
     """TextReset返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param DialogStatus: 当前会话状态，取值："START"/"COUTINUE"/"COMPLETE"。
+        :param DialogStatus: 当前会话状态{会话开始: START; 会话中: COUTINUE; 会话结束: COMPLETE}。
 注意：此字段可能返回 null，表示取不到有效值。
         :type DialogStatus: str
         :param BotName: 匹配到的机器人名称。
 注意：此字段可能返回 null，表示取不到有效值。
         :type BotName: str
         :param IntentName: 匹配到的意图名称。
 注意：此字段可能返回 null，表示取不到有效值。
         :type IntentName: str
         :param SlotInfoList: 槽位信息。
 注意：此字段可能返回 null，表示取不到有效值。
         :type SlotInfoList: list of SlotInfo
         :param InputText: 原始的用户说法。
 注意：此字段可能返回 null，表示取不到有效值。
         :type InputText: str
+        :param ResponseMessage: 机器人应答。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ResponseMessage: :class:`tencentcloud.tbp.v20190627.models.ResponseMessage`
         :param SessionAttributes: 透传字段，由用户自定义的WebService服务返回。
 注意：此字段可能返回 null，表示取不到有效值。
         :type SessionAttributes: str
+        :param ResultType: 结果类型 {中间逻辑出错:0; 任务型机器人:1; 问答型机器人:2; 闲聊型机器人:3; 未匹配上，返回预设兜底话术:5; 未匹配上，返回相似问题列表:6}。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ResultType: str
         :param ResponseText: 机器人对话的应答文本。
 注意：此字段可能返回 null，表示取不到有效值。
         :type ResponseText: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.DialogStatus = None
         self.BotName = None
         self.IntentName = None
         self.SlotInfoList = None
         self.InputText = None
+        self.ResponseMessage = None
         self.SessionAttributes = None
+        self.ResultType = None
         self.ResponseText = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.DialogStatus = params.get("DialogStatus")
         self.BotName = params.get("BotName")
@@ -380,10 +324,14 @@
         if params.get("SlotInfoList") is not None:
             self.SlotInfoList = []
             for item in params.get("SlotInfoList"):
                 obj = SlotInfo()
                 obj._deserialize(item)
                 self.SlotInfoList.append(obj)
         self.InputText = params.get("InputText")
+        if params.get("ResponseMessage") is not None:
+            self.ResponseMessage = ResponseMessage()
+            self.ResponseMessage._deserialize(params.get("ResponseMessage"))
         self.SessionAttributes = params.get("SessionAttributes")
+        self.ResultType = params.get("ResultType")
         self.ResponseText = params.get("ResponseText")
         self.RequestId = params.get("RequestId")
```

### Comparing `tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190311/tbp_client.py` & `tencentcloud-sdk-python-tbp-3.0.907/tencentcloud/tbp/v20190311/tbp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190627/errorcodes.py` & `tencentcloud-sdk-python-tbp-3.0.907/tencentcloud/tbp/v20190627/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190627/models.py` & `tencentcloud-sdk-python-tbp-3.0.907/tencentcloud/tbp/v20190311/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,27 +14,80 @@
 # limitations under the License.
 
 import warnings
 
 from tencentcloud.common.abstract_model import AbstractModel
 
 
+class CreateBotRequest(AbstractModel):
+    """CreateBot请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param BotName: 机器人名称
+        :type BotName: str
+        :param BotCnName: 机器人中文名称
+        :type BotCnName: str
+        """
+        self.BotName = None
+        self.BotCnName = None
+
+
+    def _deserialize(self, params):
+        self.BotName = params.get("BotName")
+        self.BotCnName = params.get("BotCnName")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateBotResponse(AbstractModel):
+    """CreateBot返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TaskRequestId: 任务ID
+        :type TaskRequestId: str
+        :param Msg: 任务信息
+        :type Msg: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TaskRequestId = None
+        self.Msg = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TaskRequestId = params.get("TaskRequestId")
+        self.Msg = params.get("Msg")
+        self.RequestId = params.get("RequestId")
+
+
 class Group(AbstractModel):
     """Group是消息组的具体定义，当前包含ContentType、Url、Content三个字段。其中，具体的ContentType字段定义，参考互联网MIME类型标准。
 
     """
 
     def __init__(self):
         r"""
-        :param ContentType: 消息类型参考互联网MIME类型标准，当前仅支持"text/plain"。
+        :param ContentType: 消息类型参考互联网MIME类型标准，当前仅支持"text/plain"。	
         :type ContentType: str
-        :param Url: 返回内容以链接形式提供。
+        :param Url: 返回内容以链接形式提供。	
 注意：此字段可能返回 null，表示取不到有效值。
         :type Url: str
-        :param Content: 普通文本。
+        :param Content: 普通文本。	
 注意：此字段可能返回 null，表示取不到有效值。
         :type Content: str
         """
         self.ContentType = None
         self.Url = None
         self.Content = None
 
@@ -48,35 +101,134 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class ResetRequest(AbstractModel):
+    """Reset请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param BotId: 机器人标识
+        :type BotId: str
+        :param UserId: 子账户id，每个终端对应一个
+        :type UserId: str
+        :param BotVersion: 机器人版本号。BotVersion/BotEnv二选一：二者均填，仅BotVersion有效；二者均不填，默认BotEnv=dev
+        :type BotVersion: str
+        :param BotEnv: 机器人环境{dev:测试;release:线上}。BotVersion/BotEnv二选一：二者均填，仅BotVersion有效；二者均不填，默认BotEnv=dev
+        :type BotEnv: str
+        """
+        self.BotId = None
+        self.UserId = None
+        self.BotVersion = None
+        self.BotEnv = None
+
+
+    def _deserialize(self, params):
+        self.BotId = params.get("BotId")
+        self.UserId = params.get("UserId")
+        self.BotVersion = params.get("BotVersion")
+        self.BotEnv = params.get("BotEnv")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ResetResponse(AbstractModel):
+    """Reset返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DialogStatus: 当前会话状态。取值:"start"/"continue"/"complete"
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DialogStatus: str
+        :param BotName: 匹配到的机器人名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BotName: str
+        :param IntentName: 匹配到的意图名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IntentName: str
+        :param ResponseText: 机器人回答
+        :type ResponseText: str
+        :param SlotInfoList: 语义解析的槽位结果列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SlotInfoList: list of SlotInfo
+        :param SessionAttributes: 透传字段
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SessionAttributes: str
+        :param Question: 用户说法。该说法是用户原生说法或ASR识别结果，未经过语义优化
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Question: str
+        :param WaveUrl: tts合成pcm音频存储链接。仅当请求参数NeedTts=true时返回
+注意：此字段可能返回 null，表示取不到有效值。
+        :type WaveUrl: str
+        :param WaveData: tts合成的pcm音频。二进制数组经过base64编码(暂时不返回)
+注意：此字段可能返回 null，表示取不到有效值。
+        :type WaveData: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.DialogStatus = None
+        self.BotName = None
+        self.IntentName = None
+        self.ResponseText = None
+        self.SlotInfoList = None
+        self.SessionAttributes = None
+        self.Question = None
+        self.WaveUrl = None
+        self.WaveData = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.DialogStatus = params.get("DialogStatus")
+        self.BotName = params.get("BotName")
+        self.IntentName = params.get("IntentName")
+        self.ResponseText = params.get("ResponseText")
+        if params.get("SlotInfoList") is not None:
+            self.SlotInfoList = []
+            for item in params.get("SlotInfoList"):
+                obj = SlotInfo()
+                obj._deserialize(item)
+                self.SlotInfoList.append(obj)
+        self.SessionAttributes = params.get("SessionAttributes")
+        self.Question = params.get("Question")
+        self.WaveUrl = params.get("WaveUrl")
+        self.WaveData = params.get("WaveData")
+        self.RequestId = params.get("RequestId")
+
+
 class ResponseMessage(AbstractModel):
     """从TBP-RTS服务v1.3版本起，机器人以消息组列表的形式响应，消息组列表GroupList包含多组消息，用户根据需要对部分或全部消息组进行组合使用。
 
     """
 
     def __init__(self):
         r"""
-        :param GroupList: 消息组列表。
+        :param GroupList: 消息组列表。	
 注意：此字段可能返回 null，表示取不到有效值。
-        :type GroupList: list of Group
+        :type GroupList: :class:`tencentcloud.tbp.v20190311.models.Group`
         """
         self.GroupList = None
 
 
     def _deserialize(self, params):
         if params.get("GroupList") is not None:
-            self.GroupList = []
-            for item in params.get("GroupList"):
-                obj = Group()
-                obj._deserialize(item)
-                self.GroupList.append(obj)
+            self.GroupList = Group()
+            self.GroupList._deserialize(params.get("GroupList"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -117,44 +269,36 @@
 
     """
 
     def __init__(self):
         r"""
         :param BotId: 机器人标识，用于定义抽象机器人。
         :type BotId: str
-        :param BotEnv: 机器人版本，取值"dev"或"release"，{调试版本：dev；线上版本：release}。
-        :type BotEnv: str
         :param TerminalId: 终端标识，每个终端(或线程)对应一个，区分并发多用户。
         :type TerminalId: str
         :param InputText: 请求的文本。
         :type InputText: str
+        :param BotEnv: 机器人版本，取值"dev"或"release"，{调试版本：dev；线上版本：release}。
+        :type BotEnv: str
         :param SessionAttributes: 透传字段，透传给用户自定义的WebService服务。
         :type SessionAttributes: str
-        :param PlatformType: 平台类型，{小程序：MiniProgram；小微：XiaoWei；公众号：OfficialAccount；企业微信: WXWork}。
-        :type PlatformType: str
-        :param PlatformId: 当PlatformType为微信公众号或企业微信时，传递对应微信公众号或企业微信的唯一标识
-        :type PlatformId: str
         """
         self.BotId = None
-        self.BotEnv = None
         self.TerminalId = None
         self.InputText = None
+        self.BotEnv = None
         self.SessionAttributes = None
-        self.PlatformType = None
-        self.PlatformId = None
 
 
     def _deserialize(self, params):
         self.BotId = params.get("BotId")
-        self.BotEnv = params.get("BotEnv")
         self.TerminalId = params.get("TerminalId")
         self.InputText = params.get("InputText")
+        self.BotEnv = params.get("BotEnv")
         self.SessionAttributes = params.get("SessionAttributes")
-        self.PlatformType = params.get("PlatformType")
-        self.PlatformId = params.get("PlatformId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -178,33 +322,37 @@
         :type IntentName: str
         :param SlotInfoList: 槽位信息。
 注意：此字段可能返回 null，表示取不到有效值。
         :type SlotInfoList: list of SlotInfo
         :param InputText: 原始的用户说法。
 注意：此字段可能返回 null，表示取不到有效值。
         :type InputText: str
-        :param ResponseMessage: 机器人应答。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ResponseMessage: :class:`tencentcloud.tbp.v20190627.models.ResponseMessage`
         :param SessionAttributes: 透传字段，由用户自定义的WebService服务返回。
 注意：此字段可能返回 null，表示取不到有效值。
         :type SessionAttributes: str
-        :param ResultType: 结果类型 {中间逻辑出错:0; 任务型机器人:1; 问答型机器人:2; 闲聊型机器人:3; 未匹配上，返回预设兜底话术:5; 未匹配上，返回相似问题列表:6}。
+        :param ResponseText: 机器人对话的应答文本。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ResponseText: str
+        :param ResponseMessage: 机器人应答。	
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ResponseMessage: :class:`tencentcloud.tbp.v20190311.models.ResponseMessage`
+        :param ResultType: 结果类型 {中间逻辑出错:0; 任务型机器人:1; 问答型机器人:2; 闲聊型机器人:3; 未匹配上，返回预设兜底话术:5; 未匹配上，返回相似问题列表:6}。	
 注意：此字段可能返回 null，表示取不到有效值。
         :type ResultType: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.DialogStatus = None
         self.BotName = None
         self.IntentName = None
         self.SlotInfoList = None
         self.InputText = None
-        self.ResponseMessage = None
         self.SessionAttributes = None
+        self.ResponseText = None
+        self.ResponseMessage = None
         self.ResultType = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.DialogStatus = params.get("DialogStatus")
         self.BotName = params.get("BotName")
@@ -212,53 +360,46 @@
         if params.get("SlotInfoList") is not None:
             self.SlotInfoList = []
             for item in params.get("SlotInfoList"):
                 obj = SlotInfo()
                 obj._deserialize(item)
                 self.SlotInfoList.append(obj)
         self.InputText = params.get("InputText")
+        self.SessionAttributes = params.get("SessionAttributes")
+        self.ResponseText = params.get("ResponseText")
         if params.get("ResponseMessage") is not None:
             self.ResponseMessage = ResponseMessage()
             self.ResponseMessage._deserialize(params.get("ResponseMessage"))
-        self.SessionAttributes = params.get("SessionAttributes")
         self.ResultType = params.get("ResultType")
         self.RequestId = params.get("RequestId")
 
 
 class TextResetRequest(AbstractModel):
     """TextReset请求参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param BotId: 机器人标识，用于定义抽象机器人。
         :type BotId: str
-        :param BotEnv: 机器人版本，取值"dev"或"release"，{调试版本：dev；线上版本：release}。
-        :type BotEnv: str
         :param TerminalId: 终端标识，每个终端(或线程)对应一个，区分并发多用户。
         :type TerminalId: str
-        :param PlatformType: 平台类型，{小程序：MiniProgram；小微：XiaoWei；公众号：OfficialAccount；企业微信: WXWork}。
-        :type PlatformType: str
-        :param PlatformId: 当PlatformType为微信公众号或企业微信时，传递对应微信公众号或企业微信的唯一标识
-        :type PlatformId: str
+        :param BotEnv: 机器人版本，取值"dev"或"release"，{调试版本：dev；线上版本：release}。
+        :type BotEnv: str
         """
         self.BotId = None
-        self.BotEnv = None
         self.TerminalId = None
-        self.PlatformType = None
-        self.PlatformId = None
+        self.BotEnv = None
 
 
     def _deserialize(self, params):
         self.BotId = params.get("BotId")
-        self.BotEnv = params.get("BotEnv")
         self.TerminalId = params.get("TerminalId")
-        self.PlatformType = params.get("PlatformType")
-        self.PlatformId = params.get("PlatformId")
+        self.BotEnv = params.get("BotEnv")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -267,52 +408,44 @@
 class TextResetResponse(AbstractModel):
     """TextReset返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param DialogStatus: 当前会话状态{会话开始: START; 会话中: COUTINUE; 会话结束: COMPLETE}。
+        :param DialogStatus: 当前会话状态，取值："START"/"COUTINUE"/"COMPLETE"。
 注意：此字段可能返回 null，表示取不到有效值。
         :type DialogStatus: str
         :param BotName: 匹配到的机器人名称。
 注意：此字段可能返回 null，表示取不到有效值。
         :type BotName: str
         :param IntentName: 匹配到的意图名称。
 注意：此字段可能返回 null，表示取不到有效值。
         :type IntentName: str
         :param SlotInfoList: 槽位信息。
 注意：此字段可能返回 null，表示取不到有效值。
         :type SlotInfoList: list of SlotInfo
         :param InputText: 原始的用户说法。
 注意：此字段可能返回 null，表示取不到有效值。
         :type InputText: str
-        :param ResponseMessage: 机器人应答。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ResponseMessage: :class:`tencentcloud.tbp.v20190627.models.ResponseMessage`
         :param SessionAttributes: 透传字段，由用户自定义的WebService服务返回。
 注意：此字段可能返回 null，表示取不到有效值。
         :type SessionAttributes: str
-        :param ResultType: 结果类型 {中间逻辑出错:0; 任务型机器人:1; 问答型机器人:2; 闲聊型机器人:3; 未匹配上，返回预设兜底话术:5; 未匹配上，返回相似问题列表:6}。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ResultType: str
         :param ResponseText: 机器人对话的应答文本。
 注意：此字段可能返回 null，表示取不到有效值。
         :type ResponseText: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.DialogStatus = None
         self.BotName = None
         self.IntentName = None
         self.SlotInfoList = None
         self.InputText = None
-        self.ResponseMessage = None
         self.SessionAttributes = None
-        self.ResultType = None
         self.ResponseText = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.DialogStatus = params.get("DialogStatus")
         self.BotName = params.get("BotName")
@@ -320,14 +453,10 @@
         if params.get("SlotInfoList") is not None:
             self.SlotInfoList = []
             for item in params.get("SlotInfoList"):
                 obj = SlotInfo()
                 obj._deserialize(item)
                 self.SlotInfoList.append(obj)
         self.InputText = params.get("InputText")
-        if params.get("ResponseMessage") is not None:
-            self.ResponseMessage = ResponseMessage()
-            self.ResponseMessage._deserialize(params.get("ResponseMessage"))
         self.SessionAttributes = params.get("SessionAttributes")
-        self.ResultType = params.get("ResultType")
         self.ResponseText = params.get("ResponseText")
         self.RequestId = params.get("RequestId")
```

### Comparing `tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190627/tbp_client.py` & `tencentcloud-sdk-python-tbp-3.0.907/tencentcloud/tbp/v20190627/tbp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tbp-3.0.907/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tbp-3.0.906/PKG-INFO` & `tencentcloud-sdk-python-tbp-3.0.907/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tbp
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Tbp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tbp-3.0.906/setup.py` & `tencentcloud-sdk-python-tbp-3.0.907/setup.py`

 * *Files identical despite different names*

