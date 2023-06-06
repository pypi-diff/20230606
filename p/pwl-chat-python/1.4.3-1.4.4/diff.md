# Comparing `tmp/pwl-chat-python-1.4.3.tar.gz` & `tmp/pwl-chat-python-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwl-chat-python-1.4.3.tar", last modified: Sun May 14 06:05:33 2023, max compression
+gzip compressed data, was "pwl-chat-python-1.4.4.tar", last modified: Tue Jun  6 09:01:17 2023, max compression
```

## Comparing `pwl-chat-python-1.4.3.tar` & `pwl-chat-python-1.4.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-14 06:05:33.211877 pwl-chat-python-1.4.3/
--rw-r--r--   0 fangcong   (501) staff       (20)     1066 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.3/LICENSE
--rw-r--r--   0 fangcong   (501) staff       (20)     2008 2023-05-14 06:05:33.211429 pwl-chat-python-1.4.3/PKG-INFO
--rw-r--r--   0 fangcong   (501) staff       (20)     1409 2023-05-11 06:39:39.000000 pwl-chat-python-1.4.3/README.md
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-14 06:05:33.201538 pwl-chat-python-1.4.3/pwl_chat_python.egg-info/
--rw-r--r--   0 fangcong   (501) staff       (20)     2008 2023-05-14 06:05:33.000000 pwl-chat-python-1.4.3/pwl_chat_python.egg-info/PKG-INFO
--rw-r--r--   0 fangcong   (501) staff       (20)      549 2023-05-14 06:05:33.000000 pwl-chat-python-1.4.3/pwl_chat_python.egg-info/SOURCES.txt
--rw-r--r--   0 fangcong   (501) staff       (20)        1 2023-05-14 06:05:33.000000 pwl-chat-python-1.4.3/pwl_chat_python.egg-info/dependency_links.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       49 2023-05-14 06:05:33.000000 pwl-chat-python-1.4.3/pwl_chat_python.egg-info/entry_points.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       45 2023-05-14 06:05:33.000000 pwl-chat-python-1.4.3/pwl_chat_python.egg-info/requires.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       31 2023-05-14 06:05:33.000000 pwl-chat-python-1.4.3/pwl_chat_python.egg-info/top_level.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       38 2023-05-14 06:05:33.212027 pwl-chat-python-1.4.3/setup.cfg
--rw-r--r--   0 fangcong   (501) staff       (20)     3546 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.3/setup.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-14 06:05:33.201994 pwl-chat-python-1.4.3/src/
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-14 06:05:33.204073 pwl-chat-python-1.4.3/src/api/
--rw-r--r--   0 fangcong   (501) staff       (20)      312 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.3/src/api/__api__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1762 2023-05-14 04:56:17.000000 pwl-chat-python-1.4.3/src/api/__init__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1743 2023-05-10 10:32:27.000000 pwl-chat-python-1.4.3/src/api/chatroom.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1124 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.3/src/api/user.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-14 06:05:33.209140 pwl-chat-python-1.4.3/src/core/
--rw-r--r--   0 fangcong   (501) staff       (20)     2817 2023-05-14 05:06:48.000000 pwl-chat-python-1.4.3/src/core/__init__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1623 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.3/src/core/blacklist.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1960 2023-05-14 05:27:58.000000 pwl-chat-python-1.4.3/src/core/chatroom.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1961 2023-05-09 06:39:45.000000 pwl-chat-python-1.4.3/src/core/cli.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1561 2023-05-14 05:06:43.000000 pwl-chat-python-1.4.3/src/core/config.py
--rw-r--r--   0 fangcong   (501) staff       (20)     5256 2023-05-14 05:47:48.000000 pwl-chat-python-1.4.3/src/core/redpacket.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1360 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.3/src/core/user.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1226 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.3/src/core/websocket.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1329 2023-05-14 04:47:23.000000 pwl-chat-python-1.4.3/src/main.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-14 06:05:33.210486 pwl-chat-python-1.4.3/src/utils/
--rw-r--r--   0 fangcong   (501) staff       (20)      977 2023-05-14 05:48:56.000000 pwl-chat-python-1.4.3/src/utils/utils.py
--rw-r--r--   0 fangcong   (501) staff       (20)       21 2023-05-14 05:57:26.000000 pwl-chat-python-1.4.3/src/utils/version.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-06 09:01:17.779948 pwl-chat-python-1.4.4/
+-rw-r--r--   0 fangcong   (501) staff       (20)     1066 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.4/LICENSE
+-rw-r--r--   0 fangcong   (501) staff       (20)     2091 2023-06-06 09:01:17.779277 pwl-chat-python-1.4.4/PKG-INFO
+-rw-r--r--   0 fangcong   (501) staff       (20)     1492 2023-05-31 01:34:56.000000 pwl-chat-python-1.4.4/README.md
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-06 09:01:17.761203 pwl-chat-python-1.4.4/pwl_chat_python.egg-info/
+-rw-r--r--   0 fangcong   (501) staff       (20)     2091 2023-06-06 09:01:17.000000 pwl-chat-python-1.4.4/pwl_chat_python.egg-info/PKG-INFO
+-rw-r--r--   0 fangcong   (501) staff       (20)      549 2023-06-06 09:01:17.000000 pwl-chat-python-1.4.4/pwl_chat_python.egg-info/SOURCES.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)        1 2023-06-06 09:01:17.000000 pwl-chat-python-1.4.4/pwl_chat_python.egg-info/dependency_links.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       49 2023-06-06 09:01:17.000000 pwl-chat-python-1.4.4/pwl_chat_python.egg-info/entry_points.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       45 2023-06-06 09:01:17.000000 pwl-chat-python-1.4.4/pwl_chat_python.egg-info/requires.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       31 2023-06-06 09:01:17.000000 pwl-chat-python-1.4.4/pwl_chat_python.egg-info/top_level.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       38 2023-06-06 09:01:17.780823 pwl-chat-python-1.4.4/setup.cfg
+-rw-r--r--   0 fangcong   (501) staff       (20)     3546 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.4/setup.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-06 09:01:17.761694 pwl-chat-python-1.4.4/src/
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-06 09:01:17.765329 pwl-chat-python-1.4.4/src/api/
+-rw-r--r--   0 fangcong   (501) staff       (20)      312 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.4/src/api/__api__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1762 2023-05-14 04:56:17.000000 pwl-chat-python-1.4.4/src/api/__init__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1743 2023-05-10 10:32:27.000000 pwl-chat-python-1.4.4/src/api/chatroom.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1124 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.4/src/api/user.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-06 09:01:17.772864 pwl-chat-python-1.4.4/src/core/
+-rw-r--r--   0 fangcong   (501) staff       (20)     2817 2023-05-14 05:06:48.000000 pwl-chat-python-1.4.4/src/core/__init__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1623 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.4/src/core/blacklist.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1960 2023-05-14 05:27:58.000000 pwl-chat-python-1.4.4/src/core/chatroom.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1933 2023-06-06 07:22:16.000000 pwl-chat-python-1.4.4/src/core/cli.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1561 2023-05-14 05:06:43.000000 pwl-chat-python-1.4.4/src/core/config.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     5311 2023-06-06 08:51:30.000000 pwl-chat-python-1.4.4/src/core/redpacket.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1360 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.4/src/core/user.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1226 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.4/src/core/websocket.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1329 2023-05-14 04:47:23.000000 pwl-chat-python-1.4.4/src/main.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-06 09:01:17.776741 pwl-chat-python-1.4.4/src/utils/
+-rw-r--r--   0 fangcong   (501) staff       (20)      977 2023-05-14 05:48:56.000000 pwl-chat-python-1.4.4/src/utils/utils.py
+-rw-r--r--   0 fangcong   (501) staff       (20)       21 2023-06-06 08:59:05.000000 pwl-chat-python-1.4.4/src/utils/version.py
```

### Comparing `pwl-chat-python-1.4.3/LICENSE` & `pwl-chat-python-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.3/PKG-INFO` & `pwl-chat-python-1.4.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwl-chat-python
-Version: 1.4.3
+Version: 1.4.4
 Summary: 摸鱼派聊天室python客户端
 Home-page: https://github.com/gakkiyomi/pwl-chat-python
 Author: gakkiyomi
 Author-email: gakkiyomi@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -12,14 +12,16 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
+  ![摸鱼派cn.png](https://b3logfile.com/file/2023/05/摸鱼派-cn-owZQT8f.png)
+
 # pwl-chat-python
 
 > 摸鱼派聊天室 python 命令行客户端
 
 基于摸鱼打工人社区——摸鱼派开放 API 开发的摸鱼派聊天室 python 客户端程序，可以在里面边写 Bug 边愉快地吹水摸鱼。
 
 ## 安装
```

### Comparing `pwl-chat-python-1.4.3/README.md` & `pwl-chat-python-1.4.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+  ![摸鱼派cn.png](https://b3logfile.com/file/2023/05/摸鱼派-cn-owZQT8f.png)
+
 # pwl-chat-python
 
 > 摸鱼派聊天室 python 命令行客户端
 
 基于摸鱼打工人社区——摸鱼派开放 API 开发的摸鱼派聊天室 python 客户端程序，可以在里面边写 Bug 边愉快地吹水摸鱼。
 
 ## 安装
```

### Comparing `pwl-chat-python-1.4.3/pwl_chat_python.egg-info/PKG-INFO` & `pwl-chat-python-1.4.4/pwl_chat_python.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwl-chat-python
-Version: 1.4.3
+Version: 1.4.4
 Summary: 摸鱼派聊天室python客户端
 Home-page: https://github.com/gakkiyomi/pwl-chat-python
 Author: gakkiyomi
 Author-email: gakkiyomi@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -12,14 +12,16 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
+  ![摸鱼派cn.png](https://b3logfile.com/file/2023/05/摸鱼派-cn-owZQT8f.png)
+
 # pwl-chat-python
 
 > 摸鱼派聊天室 python 命令行客户端
 
 基于摸鱼打工人社区——摸鱼派开放 API 开发的摸鱼派聊天室 python 客户端程序，可以在里面边写 Bug 边愉快地吹水摸鱼。
 
 ## 安装
```

### Comparing `pwl-chat-python-1.4.3/pwl_chat_python.egg-info/SOURCES.txt` & `pwl-chat-python-1.4.4/pwl_chat_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.3/setup.py` & `pwl-chat-python-1.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.3/src/api/__init__.py` & `pwl-chat-python-1.4.4/src/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.3/src/api/chatroom.py` & `pwl-chat-python-1.4.4/src/api/chatroom.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.3/src/api/user.py` & `pwl-chat-python-1.4.4/src/api/user.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.3/src/core/__init__.py` & `pwl-chat-python-1.4.4/src/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.3/src/core/blacklist.py` & `pwl-chat-python-1.4.4/src/core/blacklist.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.3/src/core/chatroom.py` & `pwl-chat-python-1.4.4/src/core/chatroom.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.3/src/core/cli.py` & `pwl-chat-python-1.4.4/src/core/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,19 +21,19 @@
                       GLOBAL_CONFIG.auth_config.password, msg)
         elif msg == '#checked':
             if api.user.checked_status()['checkedIn']:
                 print('今日你已签到！')
             else:
                 print('今日还未签到，摸鱼也要努力呀！')
         elif msg == '#reward':
-            if api.get_yesterday_reward()['sum'] == -1:
+            reward = api.get_yesterday_reward()['sum']
+            if reward == -1:
                 print('你已经领取过昨日活跃度奖励了')
             else:
-                print('领取昨日活跃度奖励 积分: ' +
-                      str(api.user.get_liveness_info()['sum']))
+                print(f'领取昨日活跃度奖励 积分: {reward}')
         elif msg == '#liveness':
             print('当前活跃度: ' +
                   str(api.user.get_liveness_info()['liveness']))
         elif msg == '#point':
             print(
                 '当前积分: ' + str(api.user.get_user_info(GLOBAL_CONFIG.auth_config.username)['userPoint']))
         elif msg == '#online-users':
```

### Comparing `pwl-chat-python-1.4.3/src/core/config.py` & `pwl-chat-python-1.4.4/src/core/config.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.3/src/core/redpacket.py` & `pwl-chat-python-1.4.4/src/core/redpacket.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,17 +80,19 @@
         time.sleep(GLOBAL_CONFIG.redpacket_config.rate)
         open_red_packet(api, redpacket['oId'])
 
 
 def __analyzeHeartbeatRedPacket(api: FishPi, red_packet_id):
     for data in api.chatroom.more()['data']:
         if data['oId'] == red_packet_id:
-            __analyze(api, json.loads(data['content']),
-                      red_packet_id, data['time'], data['userName'])
-            return
+            if data['content']:
+                __analyze(api, json.loads(data['content']), red_packet_id, data['time'], data['userName'])
+            else:
+                return
+        return    
     print("红包助手: 你与此红包无缘")
 
 
 def __analyze(api: FishPi, packet, red_packet_id, ctime, sender):
     count = packet['count']
     got = packet['got']
     if packet['count'] == packet['got']:
```

### Comparing `pwl-chat-python-1.4.3/src/core/user.py` & `pwl-chat-python-1.4.4/src/core/user.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.3/src/core/websocket.py` & `pwl-chat-python-1.4.4/src/core/websocket.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.3/src/main.py` & `pwl-chat-python-1.4.4/src/main.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.3/src/utils/utils.py` & `pwl-chat-python-1.4.4/src/utils/utils.py`

 * *Files identical despite different names*

