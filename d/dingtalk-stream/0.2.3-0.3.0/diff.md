# Comparing `tmp/dingtalk-stream-0.2.3.tar.gz` & `tmp/dingtalk-stream-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dingtalk-stream-0.2.3.tar", last modified: Fri Jun  2 11:05:36 2023, max compression
+gzip compressed data, was "dingtalk-stream-0.3.0.tar", last modified: Tue Jun  6 12:16:13 2023, max compression
```

## Comparing `dingtalk-stream-0.2.3.tar` & `dingtalk-stream-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:05:36.791559 dingtalk-stream-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-02 11:05:34.000000 dingtalk-stream-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-06-02 11:05:36.791559 dingtalk-stream-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-02 11:05:34.000000 dingtalk-stream-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:05:36.791559 dingtalk-stream-0.2.3/dingtalk_stream/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-02 11:05:34.000000 dingtalk-stream-0.2.3/dingtalk_stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-06-02 11:05:34.000000 dingtalk-stream-0.2.3/dingtalk_stream/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-02 11:05:34.000000 dingtalk-stream-0.2.3/dingtalk_stream/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-06-02 11:05:34.000000 dingtalk-stream-0.2.3/dingtalk_stream/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-02 11:05:34.000000 dingtalk-stream-0.2.3/dingtalk_stream/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-02 11:05:34.000000 dingtalk-stream-0.2.3/dingtalk_stream/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-06-02 11:05:34.000000 dingtalk-stream-0.2.3/dingtalk_stream/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:05:36.791559 dingtalk-stream-0.2.3/dingtalk_stream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-06-02 11:05:36.000000 dingtalk-stream-0.2.3/dingtalk_stream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-02 11:05:36.000000 dingtalk-stream-0.2.3/dingtalk_stream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 11:05:36.000000 dingtalk-stream-0.2.3/dingtalk_stream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-02 11:05:36.000000 dingtalk-stream-0.2.3/dingtalk_stream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-02 11:05:36.000000 dingtalk-stream-0.2.3/dingtalk_stream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 11:05:36.791559 dingtalk-stream-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-02 11:05:34.000000 dingtalk-stream-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:16:13.098276 dingtalk-stream-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-06 12:16:12.000000 dingtalk-stream-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-06-06 12:16:13.098276 dingtalk-stream-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-06 12:16:12.000000 dingtalk-stream-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:16:13.098276 dingtalk-stream-0.3.0/dingtalk_stream/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-06 12:16:12.000000 dingtalk-stream-0.3.0/dingtalk_stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-06-06 12:16:12.000000 dingtalk-stream-0.3.0/dingtalk_stream/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-06 12:16:12.000000 dingtalk-stream-0.3.0/dingtalk_stream/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-06-06 12:16:12.000000 dingtalk-stream-0.3.0/dingtalk_stream/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-06 12:16:12.000000 dingtalk-stream-0.3.0/dingtalk_stream/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-06-06 12:16:12.000000 dingtalk-stream-0.3.0/dingtalk_stream/interactive_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-06 12:16:12.000000 dingtalk-stream-0.3.0/dingtalk_stream/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-06-06 12:16:12.000000 dingtalk-stream-0.3.0/dingtalk_stream/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:16:13.098276 dingtalk-stream-0.3.0/dingtalk_stream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-06-06 12:16:13.000000 dingtalk-stream-0.3.0/dingtalk_stream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-06 12:16:13.000000 dingtalk-stream-0.3.0/dingtalk_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 12:16:13.000000 dingtalk-stream-0.3.0/dingtalk_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 12:16:13.000000 dingtalk-stream-0.3.0/dingtalk_stream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-06 12:16:13.000000 dingtalk-stream-0.3.0/dingtalk_stream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 12:16:13.098276 dingtalk-stream-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-06 12:16:12.000000 dingtalk-stream-0.3.0/setup.py
```

### Comparing `dingtalk-stream-0.2.3/LICENSE` & `dingtalk-stream-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.2.3/PKG-INFO` & `dingtalk-stream-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.2.3
+Version: 0.3.0
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -56,23 +56,44 @@
 
 注意：消息接收模式中，选择 “Stream 模式”
 
 ![Stream 模式](https://img.alicdn.com/imgextra/i3/O1CN01XL4piO1lkYX2F6sW6_!!6000000004857-0-tps-896-522.jpg)
 
 点击“点击调试”按钮，可以创建测试群进行测试。
 
+项目中提供了两个关于机器人的测试案例：
+
+3.1 CalcBot
+
+将用户输入的内容进行数学表达式计算，并以文本消息的方式返回计算结果。
+
 启动服务：
 ```Shell
 cd examples/calcbot
 python3 calcbot.py --client_id "put-your-client-id-here" --client_secret "put-your-client-secret-here"
 ```
 
 测试效果：
 ![calcbot](https://s1.ax1x.com/2023/05/16/p92jjIJ.png)
 
+3.2 CardBot
+
+接收用户输入，返回一张互动卡片，随后更新卡片的文本和图片内容。
+
+启动服务：
+```Shell
+cd examples/cardbot
+python3 cardbot.py --client_id "put-your-client-id-here" --client_secret "put-your-client-secret-here"
+```
+
+测试效果：
+![cardbot](https://img.alicdn.com/imgextra/i2/O1CN012Va01a24FOHrQQnWy_!!6000000007361-0-tps-2184-1296.jpg)
+
+
+
 ### 事件订阅切换到 Stream 模式（可选）
 
 进入钉钉开发者后台，选择企业内部应用，在应用管理的左侧导航中，选择“事件与回调”。
 “订阅管理”中，“推送方式”选项中，选择 “Stream 模式”，并保存
 
 
 ### 技术支持
```

### Comparing `dingtalk-stream-0.2.3/README.md` & `dingtalk-stream-0.3.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -34,23 +34,44 @@
 
 注意：消息接收模式中，选择 “Stream 模式”
 
 ![Stream 模式](https://img.alicdn.com/imgextra/i3/O1CN01XL4piO1lkYX2F6sW6_!!6000000004857-0-tps-896-522.jpg)
 
 点击“点击调试”按钮，可以创建测试群进行测试。
 
+项目中提供了两个关于机器人的测试案例：
+
+3.1 CalcBot
+
+将用户输入的内容进行数学表达式计算，并以文本消息的方式返回计算结果。
+
 启动服务：
 ```Shell
 cd examples/calcbot
 python3 calcbot.py --client_id "put-your-client-id-here" --client_secret "put-your-client-secret-here"
 ```
 
 测试效果：
 ![calcbot](https://s1.ax1x.com/2023/05/16/p92jjIJ.png)
 
+3.2 CardBot
+
+接收用户输入，返回一张互动卡片，随后更新卡片的文本和图片内容。
+
+启动服务：
+```Shell
+cd examples/cardbot
+python3 cardbot.py --client_id "put-your-client-id-here" --client_secret "put-your-client-secret-here"
+```
+
+测试效果：
+![cardbot](https://img.alicdn.com/imgextra/i2/O1CN012Va01a24FOHrQQnWy_!!6000000007361-0-tps-2184-1296.jpg)
+
+
+
 ### 事件订阅切换到 Stream 模式（可选）
 
 进入钉钉开发者后台，选择企业内部应用，在应用管理的左侧导航中，选择“事件与回调”。
 “订阅管理”中，“推送方式”选项中，选择 “Stream 模式”，并保存
 
 
 ### 技术支持
```

### Comparing `dingtalk-stream-0.2.3/dingtalk_stream/chatbot.py` & `dingtalk-stream-0.3.0/dingtalk_stream/frames.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,241 +1,239 @@
 import json
-import urllib
-import requests
-from .stream import CallbackHandler
 
 
-class AtUser(object):
+class Headers(object):
+    CONTENT_TYPE_APPLICATION_JSON = 'application/json'
+
     def __init__(self):
-        self.dingtalk_id = None
-        self.staff_id = None
+        self.app_id = None
+        self.connection_id = None
+        self.content_type = None
+        self.message_id = None
+        self.time = None
+        self.topic = None
         self.extensions = {}
+        # event fields start
+        self.event_born_time = None
+        self.event_corp_id = None
+        self.event_id = None
+        self.event_type = None
+        self.event_unified_app_id = None
+        # event fields end
 
-    @classmethod
-    def from_dict(cls, d):
-        user = AtUser()
-        data = ''
-        for name, value in d.items():
-            if name == 'dingtalkId':
-                user.dingtalk_id = value
-            elif name == 'staffId':
-                user.staff_id = value
-            else:
-                user.extensions[name] = value
-        return user
+    def __str__(self):
+        fields = {
+            'app_id': self.app_id,
+            'connection_id': self.connection_id,
+            'content_type': self.content_type,
+            'message_id': self.message_id,
+            'time': self.time,
+            'topic': self.topic,
+            'extensions': self.extensions,
+        }
+        if self.event_id is not None:
+            fields['event_born_time'] = self.event_born_time
+            fields['event_id'] = self.event_id
+            fields['event_corp_id'] = self.event_corp_id
+            fields['event_type'] = self.event_type
+            fields['event_unified_app_id'] = self.event_unified_app_id
+        return 'Headers(%s)' % ', '.join(['%s=%s' % (k, v) for k, v in fields.items()])
 
     def to_dict(self):
         result = self.extensions.copy()
-        if self.dingtalk_id is not None:
-            result['dingtalkId'] = self.dingtalk_id
-        if self.staff_id is not None:
-            result['staffId'] = self.staff_id
+        if self.app_id is not None:
+            result['appId'] = self.app_id
+        if self.connection_id is not None:
+            result['connectionId'] = self.connection_id
+        if self.content_type is not None:
+            result['contentType'] = self.content_type
+        if self.message_id is not None:
+            result['messageId'] = self.message_id
+        if self.topic is not None:
+            result['topic'] = self.topic
+        if self.time is not None:
+            result['time'] = str(self.time)
         return result
 
+    @classmethod
+    def from_dict(cls, d):
+        headers = Headers()
+        for name, value in d.items():
+            if name == 'appId':
+                headers.app_id = value
+            elif name == 'connectionId':
+                headers.connection_id = value
+            elif name == 'contentType':
+                headers.content_type = value
+            elif name == 'messageId':
+                headers.message_id = value
+            elif name == 'topic':
+                headers.topic = value
+            elif name == 'time':
+                headers.time = int(value)
+            elif name == 'eventBornTime':
+                headers.event_born_time = int(value)
+            elif name == 'eventCorpId':
+                headers.event_corp_id = value
+            elif name == 'eventId':
+                headers.event_id = value
+            elif name == 'eventType':
+                headers.event_type = value
+            elif name == 'eventUnifiedAppId':
+                headers.event_unified_app_id = value
+            else:
+                headers.extensions[name] = value
+        return headers
+
 
-class TextContent(object):
-    content: str
+class EventMessage(object):
+    TYPE = 'EVENT'
 
     def __init__(self):
-        self.content = None
+        self.spec_version = ''
+        self.type = EventMessage.TYPE
+        self.headers = Headers()
+        self.data = {}
         self.extensions = {}
 
     def __str__(self):
-        return 'TextContent(content=%s)' % self.content
+        return 'EventMessage(spec_version=%s, type=%s, headers=%s, data=%s, extensions=%s)' % (
+            self.spec_version,
+            self.type,
+            self.headers,
+            self.data,
+            self.extensions)
 
     @classmethod
     def from_dict(cls, d):
-        content = TextContent()
+        msg = EventMessage()
         data = ''
         for name, value in d.items():
-            if name == 'content':
-                content.content = value
+            if name == 'specVersion':
+                msg.spec_version = value
+            elif name == 'data':
+                data = value
+            elif name == 'type':
+                pass
+            elif name == 'headers':
+                msg.headers = Headers.from_dict(value)
             else:
-                content.extensions[name] = value
-        return content
-
-    def to_dict(self):
-        result = self.extensions.copy()
-        if self.content is not None:
-            result['content'] = self.content
-        return result
-
+                msg.extensions[name] = value
+        if data:
+            msg.data = json.loads(data)
+        return msg
 
-class ChatbotMessage(object):
-    TOPIC = '/v1.0/im/bot/messages/get'
-    text: TextContent
+class CallbackMessage(object):
+    TYPE = 'CALLBACK'
 
     def __init__(self):
-        self.is_in_at_list = None
-        self.session_webhook = None
-        self.sender_nick = None
-        self.robot_code = None
-        self.session_webhook_expired_time = None
-        self.message_id = None
-        self.sender_id = None
-        self.chatbot_user_id = None
-        self.conversation_id = None
-        self.is_admin = None
-        self.create_at = None
-        self.text = None
-        self.conversation_type = None
-        self.at_users = []
-        self.chatbot_corp_id = None
-        self.sender_corp_id = None
-        self.conversation_title = None
-        self.message_type = None
-        self.sender_staff_id = None
-
+        self.spec_version = ''
+        self.type = CallbackMessage.TYPE
+        self.headers = Headers()
+        self.data = {}
         self.extensions = {}
 
+    def __str__(self):
+        return 'CallbackMessage(spec_version=%s, type=%s, headers=%s, data=%s, extensions=%s)' % (
+            self.spec_version,
+            self.type,
+            self.headers,
+            self.data,
+            self.extensions)
+
     @classmethod
     def from_dict(cls, d):
-        msg = ChatbotMessage()
+        msg = CallbackMessage()
         data = ''
         for name, value in d.items():
-            if name == 'isInAtList':
-                msg.is_in_at_list = value
-            elif name == 'sessionWebhook':
-                msg.session_webhook = value
-            elif name == 'senderNick':
-                msg.sender_nick = value
-            elif name == 'robotCode':
-                msg.robot_code = value
-            elif name == 'sessionWebhookExpiredTime':
-                msg.session_webhook_expired_time = int(value)
-            elif name == 'msgId':
-                msg.message_id = value
-            elif name == 'senderId':
-                msg.sender_id = value
-            elif name == 'chatbotUserId':
-                msg.chatbot_user_id = value
-            elif name == 'conversationId':
-                msg.conversation_id = value
-            elif name == 'isAdmin':
-                msg.is_admin = value
-            elif name == 'createAt':
-                msg.create_at = value
-            elif name == 'text':
-                msg.text = TextContent.from_dict(value)
-            elif name == 'conversationType':
-                msg.conversation_type = value
-            elif name == 'atUsers':
-                msg.at_users = [AtUser.from_dict(i) for i in value]
-            elif name == 'chatbotCorpId':
-                msg.chatbot_corp_id = value
-            elif name == 'senderCorpId':
-                msg.sender_corp_id = value
-            elif name == 'conversationTitle':
-                msg.conversation_title = value
-            elif name == 'msgtype':
-                msg.message_type = value
-            elif name == 'senderStaffId':
-                msg.sender_staff_id = value
+            if name == 'specVersion':
+                msg.spec_version = value
+            elif name == 'data':
+                data = value
+            elif name == 'type':
+                pass
+            elif name == 'headers':
+                msg.headers = Headers.from_dict(value)
             else:
                 msg.extensions[name] = value
+        if data:
+            msg.data = json.loads(data)
         return msg
 
-    def to_dict(self):
-        result = self.extensions.copy()
-        if self.is_in_at_list is not None:
-            result['isInAtList'] = self.is_in_at_list
-        if self.session_webhook is not None:
-            result['sessionWebhook'] = self.session_webhook
-        if self.sender_nick is not None:
-            result['senderNick'] = self.sender_nick
-        if self.robot_code is not None:
-            result['robotCode'] = self.robot_code
-        if self.session_webhook_expired_time is not None:
-            result['sessionWebhookExpiredTime'] = self.session_webhook_expired_time
-        if self.message_id is not None:
-            result['msgId'] = self.message_id
-        if self.sender_id is not None:
-            result['senderId'] = self.sender_id
-        if self.chatbot_user_id is not None:
-            result['chatbotUserId'] = self.chatbot_user_id
-        if self.conversation_id is not None:
-            result['conversationId'] = self.conversation_id
-        if self.is_admin is not None:
-            result['isAdmin'] = self.is_admin
-        if self.create_at is not None:
-            result['createAt'] = self.create_at
-        if self.text is not None:
-            result['text'] = self.text.to_dict()
-        if self.conversation_type is not None:
-            result['conversationType'] = self.conversation_type
-        if self.at_users is not None:
-            result['atUsers'] = [i.to_dict() for i in self.at_users]
-        if self.chatbot_corp_id is not None:
-            result['chatbotCorpId'] = self.chatbot_corp_id
-        if self.sender_corp_id is not None:
-            result['senderCorpId'] = self.sender_corp_id
-        if self.conversation_title is not None:
-            result['conversationTitle'] = self.conversation_title
-        if self.message_type is not None:
-            result['msgtype'] = self.message_type
-        if self.sender_staff_id is not None:
-            result['senderStaffId'] = self.sender_staff_id
-        return result
+class SystemMessage(object):
+    TYPE = 'SYSTEM'
+    TOPIC_DISCONNECT = 'TAG_DISCONNECT'
+
+    def __init__(self):
+        self.spec_version = ''
+        self.type = SystemMessage.TYPE
+        self.headers = Headers()
+        self.data = {}
+        self.extensions = {}
+
+        @classmethod
+        def from_dict(cls, d):
+            msg = SystemMessage()
+            data = ''
+            for name, value in d.items():
+                if name == 'specVersion':
+                    msg.spec_version = value
+                elif name == 'data':
+                    data = value
+                elif name == 'type':
+                    pass
+                elif name == 'headers':
+                    msg.headers = Headers.from_dict(value)
+                else:
+                    msg.extensions[name] = value
+            if data:
+                msg.data = json.loads(data)
+            return msg
 
     def __str__(self):
-        return 'ChatbotMessage(message_type=%s, text=%s, sender_nick=%s, conversation_title=%s)' % (
-            self.message_type,
-            self.text,
-            self.sender_nick,
-            self.conversation_title,
+        return 'SystemMessage(spec_version=%s, type=%s, headers=%s, data=%s, extensions=%s)' % (
+            self.spec_version,
+            self.type,
+            self.headers,
+            self.data,
+            self.extensions,
         )
 
+    @classmethod
+    def from_dict(cls, d):
+        msg = SystemMessage()
+        data = ''
+        for name, value in d.items():
+            if name == 'specVersion':
+                msg.spec_version = value
+            elif name == 'data':
+                data = value
+            elif name == 'type':
+                pass
+            elif name == 'headers':
+                msg.headers = Headers.from_dict(value)
+            else:
+                msg.extensions[name] = value
+        if data:
+            msg.data = json.loads(data)
+        return msg
+
 
-class ChatbotHandler(CallbackHandler):
-    def reply_text(self,
-                         text: str,
-                         incoming_message: ChatbotMessage):
-        request_headers = {
-            'Content-Type': 'application/json',
-            'Accept': '*/*',
-        }
-        values = {
-            'msgtype': 'text',
-            'text': {
-                'content': text,
-            },
-            'at': {
-                'atUserIds': [incoming_message.sender_staff_id],
-            }
-        }
-        try:
-            response = requests.post(incoming_message.session_webhook,
-                                     headers=request_headers,
-                                     data=json.dumps(values))
-            response.raise_for_status()
-        except Exception as e:
-            self.logger.error('reply text failed, error=%s', e)
-            return None
-        return response.json()
-
-    def reply_markdown(self,
-                       title: str,
-                       text: str,
-                       incoming_message: ChatbotMessage):
-        request_headers = {
-            'Content-Type': 'application/json',
-            'Accept': '*/*',
-        }
-        values = {
-            'msgtype': 'markdown',
-            'markdown': {
-                'title': title,
-                'text': text,
-            },
-            'at': {
-                'atUserIds': [incoming_message.sender_staff_id],
-            }
+class AckMessage(object):
+    STATUS_OK = 200
+    STATUS_BAD_REQUEST = 400
+    STATUS_NOT_IMPLEMENT = 404
+    STATUS_SYSTEM_EXCEPTION = 500
+
+    def __init__(self):
+        self.code = AckMessage.STATUS_OK
+        self.headers = Headers()
+        self.message = ''
+        self.data = {}
+
+    def to_dict(self):
+        return {
+            'code': self.code,
+            'headers': self.headers.to_dict(),
+            'message': self.message,
+            'data': json.dumps(self.data),
         }
-        try:
-            response = requests.post(incoming_message.session_webhook,
-                                     headers=request_headers,
-                                     data=json.dumps(values))
-            response.raise_for_status()
-        except Exception as e:
-            self.logger.error('reply markdown failed, error=%s', e)
-            return None
-        return response.json()
```

### Comparing `dingtalk-stream-0.2.3/dingtalk_stream/handlers.py` & `dingtalk-stream-0.3.0/dingtalk_stream/handlers.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.2.3/dingtalk_stream/stream.py` & `dingtalk-stream-0.3.0/dingtalk_stream/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,13 +202,8 @@
             response = requests.post(upload_url, data=values, files=files)
             if response.status_code == 401:
                 self.reset_access_token()
             response.raise_for_status()
         except Exception as e:
             self.logger.error('upload to dingtalk failed, error=%s', e)
             return None
-        json_result = response.json()
-        if 'media_id' not in json_result:
-            self.logger.error('upload to dingtalk failed, code=%d, result=%s, headers=%s, upload_url=%s',
-                              response.status_code, json_result, response.headers, upload_url)
-            return None
-        return json_result['media_id']
+        return response.json()['media_id']
```

### Comparing `dingtalk-stream-0.2.3/dingtalk_stream.egg-info/PKG-INFO` & `dingtalk-stream-0.3.0/dingtalk_stream.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.2.3
+Version: 0.3.0
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -56,23 +56,44 @@
 
 注意：消息接收模式中，选择 “Stream 模式”
 
 ![Stream 模式](https://img.alicdn.com/imgextra/i3/O1CN01XL4piO1lkYX2F6sW6_!!6000000004857-0-tps-896-522.jpg)
 
 点击“点击调试”按钮，可以创建测试群进行测试。
 
+项目中提供了两个关于机器人的测试案例：
+
+3.1 CalcBot
+
+将用户输入的内容进行数学表达式计算，并以文本消息的方式返回计算结果。
+
 启动服务：
 ```Shell
 cd examples/calcbot
 python3 calcbot.py --client_id "put-your-client-id-here" --client_secret "put-your-client-secret-here"
 ```
 
 测试效果：
 ![calcbot](https://s1.ax1x.com/2023/05/16/p92jjIJ.png)
 
+3.2 CardBot
+
+接收用户输入，返回一张互动卡片，随后更新卡片的文本和图片内容。
+
+启动服务：
+```Shell
+cd examples/cardbot
+python3 cardbot.py --client_id "put-your-client-id-here" --client_secret "put-your-client-secret-here"
+```
+
+测试效果：
+![cardbot](https://img.alicdn.com/imgextra/i2/O1CN012Va01a24FOHrQQnWy_!!6000000007361-0-tps-2184-1296.jpg)
+
+
+
 ### 事件订阅切换到 Stream 模式（可选）
 
 进入钉钉开发者后台，选择企业内部应用，在应用管理的左侧导航中，选择“事件与回调”。
 “订阅管理”中，“推送方式”选项中，选择 “Stream 模式”，并保存
 
 
 ### 技术支持
```

### Comparing `dingtalk-stream-0.2.3/setup.py` & `dingtalk-stream-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='dingtalk-stream',
-    version='0.2.3',
+    version='0.3.0',
     description='A Python library for sending messages to DingTalk chatbot',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/open-dingtalk/dingtalk-stream-sdk-python',
     author='Ke Jie',
     author_email='jinxi.kj@alibaba-inc.com',
     license='MIT',
```

