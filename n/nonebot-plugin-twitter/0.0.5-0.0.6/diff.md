# Comparing `tmp/nonebot-plugin-twitter-0.0.5.tar.gz` & `tmp/nonebot-plugin-twitter-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-twitter-0.0.5.tar", last modified: Mon Jun  5 15:35:44 2023, max compression
+gzip compressed data, was "nonebot-plugin-twitter-0.0.6.tar", last modified: Tue Jun  6 06:01:39 2023, max compression
```

## Comparing `nonebot-plugin-twitter-0.0.5.tar` & `nonebot-plugin-twitter-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2023-06-05 15:35:33.871221 nonebot-plugin-twitter-0.0.5/LICENSE
--rw-r--r--   0        0        0     3127 2023-06-05 15:35:33.871221 nonebot-plugin-twitter-0.0.5/README.md
--rw-r--r--   0        0        0    15454 2023-06-05 15:35:33.871221 nonebot-plugin-twitter-0.0.5/nonebot_plugin_twitter/__init__.py
--rw-r--r--   0        0        0     1041 2023-06-05 15:35:33.871221 nonebot-plugin-twitter-0.0.5/nonebot_plugin_twitter/config.py
--rw-r--r--   0        0        0      646 2023-06-05 15:35:33.871221 nonebot-plugin-twitter-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3495 1970-01-01 00:00:00.000000 nonebot-plugin-twitter-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-06 06:01:26.689522 nonebot-plugin-twitter-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3369 2023-06-06 06:01:26.689522 nonebot-plugin-twitter-0.0.6/README.md
+-rw-r--r--   0        0        0    17458 2023-06-06 06:01:26.689522 nonebot-plugin-twitter-0.0.6/nonebot_plugin_twitter/__init__.py
+-rw-r--r--   0        0        0     1252 2023-06-06 06:01:26.689522 nonebot-plugin-twitter-0.0.6/nonebot_plugin_twitter/config.py
+-rw-r--r--   0        0        0      646 2023-06-06 06:01:26.689522 nonebot-plugin-twitter-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3737 1970-01-01 00:00:00.000000 nonebot-plugin-twitter-0.0.6/PKG-INFO
```

### Comparing `nonebot-plugin-twitter-0.0.5/LICENSE` & `nonebot-plugin-twitter-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.0.5/README.md` & `nonebot-plugin-twitter-0.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -77,23 +77,29 @@
  
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | bearer_token | 是 | 无 | Bearer Token |
 | twitter_proxy | 否 | 无 | proxy |
+| twitter_debug | 否 | False | debug模式 |
 | command_priority | 否 | 10 | 命令优先级 |
 
+[![pCPq2Hs.png](https://s1.ax1x.com/2023/06/06/pCPq2Hs.png)](https://imgse.com/i/pCPq2Hs)
+
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | 关注推主 | 无 | 否 | 群聊/私聊 | 关注，指令格式：“关注推主 <推主id> [r18]” r18为可选参数，不开启和默认为不推送r18推文|
 | 取关推主 | 无 | 否 | 群聊/私聊 | 取关切割 |
 | 推主列表 | 无 | 否 | 群聊/私聊 | 展示列表 |
 | 推特推送关闭 | 群管 | 否 | 群聊/私聊 | 关闭推送 |
 | 推特推送开启 | 群管 | 否 | 群聊/私聊 | 开启推送 |
 ### 效果图
 [![pCPuhWV.png](https://s1.ax1x.com/2023/06/05/pCPuhWV.png)](https://imgse.com/i/pCPuhWV)
 [![pCPu4zT.png](https://s1.ax1x.com/2023/06/05/pCPu4zT.png)](https://imgse.com/i/pCPu4zT)
 ### 注意事项
-1.消息为合并转发发送，存在延迟和发送失败的可能
+1.推主id：
+[![pCPMu36.png](https://s1.ax1x.com/2023/06/05/pCPMu36.png)](https://imgse.com/i/pCPMu36)
+
+2.消息为合并转发发送，存在延迟和发送失败的可能
```

#### html2text {}

```diff
@@ -13,20 +13,23 @@
 [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_twitter"]  ##
 âï¸ éç½® ç³è¯· [twitter api](https://developer.twitter.com/zh-cn/docs/
 twitter-ads-api/getting-started) æé çæå¹¶è®°å½ [Bearer Token](https://
 developer.twitter.com/en/portal/dashboard) [![pCPufJ0.png](https://s1.ax1x.com/
 2023/06/05/pCPufJ0.png)](https://imgse.com/i/pCPufJ0) å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
 é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | bearer_token | æ¯ | æ 
-| Bearer Token | | twitter_proxy | å¦ | æ  | proxy | | command_priority | å¦
-| 10 | å½ä»¤ä¼åçº§ | ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé |
-éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| |
-å³æ³¨æ¨ä¸» | æ  | å¦ | ç¾¤è/ç§è |
-å³æ³¨ï¼æä»¤æ ¼å¼ï¼âå³æ³¨æ¨ä¸» <æ¨ä¸»id> [r18]â
+| Bearer Token | | twitter_proxy | å¦ | æ  | proxy | | twitter_debug | å¦ |
+False | debugæ¨¡å¼ | | command_priority | å¦ | 10 | å½ä»¤ä¼åçº§ | [!
+[pCPq2Hs.png](https://s1.ax1x.com/2023/06/06/pCPq2Hs.png)](https://imgse.com/i/
+pCPq2Hs) ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ |
+è¯´æ | |:-----:|:----:|:----:|:----:|:----:| | å³æ³¨æ¨ä¸» | æ  | å¦ |
+ç¾¤è/ç§è | å³æ³¨ï¼æä»¤æ ¼å¼ï¼âå³æ³¨æ¨ä¸» <æ¨ä¸»id> [r18]â
 r18ä¸ºå¯éåæ°ï¼ä¸å¼å¯åé»è®¤ä¸ºä¸æ¨ér18æ¨æ| | åå³æ¨ä¸» |
 æ  | å¦ | ç¾¤è/ç§è | åå³åå² | | æ¨ä¸»åè¡¨ | æ  | å¦ | ç¾¤è/
 ç§è | å±ç¤ºåè¡¨ | | æ¨ç¹æ¨éå³é­ | ç¾¤ç®¡ | å¦ | ç¾¤è/ç§è |
 å³é­æ¨é | | æ¨ç¹æ¨éå¼å¯ | ç¾¤ç®¡ | å¦ | ç¾¤è/ç§è |
 å¼å¯æ¨é | ### ææå¾ [![pCPuhWV.png](https://s1.ax1x.com/2023/06/05/
 pCPuhWV.png)](https://imgse.com/i/pCPuhWV) [![pCPu4zT.png](https://s1.ax1x.com/
 2023/06/05/pCPu4zT.png)](https://imgse.com/i/pCPu4zT) ### æ³¨æäºé¡¹
-1.æ¶æ¯ä¸ºåå¹¶è½¬ååéï¼å­å¨å»¶è¿ååéå¤±è´¥çå¯è½
+1.æ¨ä¸»idï¼ [![pCPMu36.png](https://s1.ax1x.com/2023/06/05/pCPMu36.png)]
+(https://imgse.com/i/pCPMu36)
+2.æ¶æ¯ä¸ºåå¹¶è½¬ååéï¼å­å¨å»¶è¿ååéå¤±è´¥çå¯è½
```

### Comparing `nonebot-plugin-twitter-0.0.5/nonebot_plugin_twitter/__init__.py` & `nonebot-plugin-twitter-0.0.6/nonebot_plugin_twitter/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import nonebot
 from nonebot.adapters.onebot.v11.adapter import Adapter
 from nonebot.exception import MatcherException
 from nonebot.plugin import PluginMetadata
 from pathlib import Path
 import json
 import random
-from httpx import AsyncClient
+from httpx import AsyncClient,Client
 import asyncio
 import tweepy
 from .config import Config,__version__
 
 #
 config_dev = Config.parse_obj(get_driver().config)
 
@@ -70,14 +70,54 @@
     )     
     if config_dev.twitter_proxy:
         # twitter_proxy
         client.session.proxies = {
             "http":config_dev.twitter_proxy,
             "https":config_dev.twitter_proxy
         }
+        logger.info(f"已读取 twitter proxy {client.session.proxies}")
+    
+    # Debug
+    if config_dev.twitter_debug:
+        try:
+            logger.debug("连通性测试")
+            if config_dev.twitter_proxy:
+                logger.debug("twitter proxy 测试")
+                with Client(proxies=f"http://{config_dev.twitter_proxy}") as client_test:
+                    res = client_test.get("https://twitter.com/",headers=header)
+                    if res.status_code == 200 or res.status_code == 302:
+                        logger.debug(f"连通正常：{res.status_code}")
+                    else:
+                        logger.debug(f"连通异常：{res.status_code}")
+            else:
+                logger.debug("twitter 直连 测试")
+                with Client() as client_test:
+                    res = client_test.get("https://twitter.com/",headers=header)
+                    if res.status_code == 200 or res.status_code == 302:
+                        logger.debug(f"连通正常：{res.status_code}")
+                    else:
+                        logger.debug(f"连通异常：{res.status_code}")
+        except Exception as e:
+            logger.debug(f"连通测试异常：{e}")
+                    
+        try:
+            logger.debug("获取推文测试")
+            tweet_test = client.get_tweet(id=1665797367747026948,
+                            media_fields="duration_ms,height,media_key,preview_image_url,public_metrics,type,url,width,alt_text,variants".split(
+                                ","),
+                            expansions=[
+                                'entities.mentions.username',
+                                'attachments.media_keys',
+                            ],
+                    
+                    tweet_fields=["possibly_sensitive"])
+            if tweet_test.data:
+                logger.debug("获取推文测试成功")
+        except Exception as e:
+            logger.debug(f"获取推文异常：{e}")
     
     @scheduler.scheduled_job("interval",minutes=3,id="twitter",misfire_grace_time=180)
     async def now_twitter():
         group_task_list = []
         group_list = json.loads(dirpath.read_text("utf8"))
         for group_num in group_list:
             if group_num and group_list[group_num]["status"] == "on":
@@ -122,15 +162,15 @@
                     pass
             l_list[l_num][str(user_id)][1] = ne.data[-1].id
             if type_list == "group":
                 dirpath.write_text(json.dumps(l_list))
             else:
                 pripath.write_text(json.dumps(l_list))
             # 清除垃圾
-            await asyncio.sleep(50)
+            await asyncio.sleep(80)
             for path in res["path"]:
                 os.unlink(path) 
                 os.unlink(path+".jpg")
     except Exception as e:
         pass
     
 async def get_tweet_for_id(id: int,r18: bool,name: str):
```

### Comparing `nonebot-plugin-twitter-0.0.5/nonebot_plugin_twitter/config.py` & `nonebot-plugin-twitter-0.0.6/nonebot_plugin_twitter/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     __version__ = None
 
 class Config(BaseModel):
     bearer_token: Optional[str] = ""
     twitter_proxy: Optional[str] = ""
     command_priority: int = 10
     plugin_enabled: bool = True
+    twitter_debug: bool = False
     
     @validator("bearer_token")
     def check_bearer_token(cls,v):
         if isinstance(v,str):
             logger.info("bearer_token 读取成功")
             return v
     @validator("twitter_proxy")
@@ -31,7 +32,13 @@
             return v
         
     @validator("command_priority")
     def check_command_priority(cls,v):
         if isinstance(v,int) and v >= 1:
             logger.info("command_priority 读取成功")
             return v
+    
+    @validator("twitter_debug")
+    def check_twitter_debug(cls,v):
+        if isinstance(v,bool):
+            logger.info("twitter_debug 开启成功")
+            return v
```

### Comparing `nonebot-plugin-twitter-0.0.5/pyproject.toml` & `nonebot-plugin-twitter-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-twitter"
-version = "0.0.5"
+version = "0.0.6"
 description = "NoneBot2 plugin for twitter"
 authors = [
     { name = "nek0us", email = "nekouss@gmail.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.1.3",
```

### Comparing `nonebot-plugin-twitter-0.0.5/PKG-INFO` & `nonebot-plugin-twitter-0.0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-twitter
-Version: 0.0.5
+Version: 0.0.6
 Summary: NoneBot2 plugin for twitter
 License: MIT
 Author-email: nek0us <nekouss@gmail.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/nek0us/nonebot-plugin-twitter
 Project-URL: Repository, https://github.com/nek0us/nonebot-plugin-twitter
 Description-Content-Type: text/markdown
@@ -88,24 +88,30 @@
  
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | bearer_token | 是 | 无 | Bearer Token |
 | twitter_proxy | 否 | 无 | proxy |
+| twitter_debug | 否 | False | debug模式 |
 | command_priority | 否 | 10 | 命令优先级 |
 
+[![pCPq2Hs.png](https://s1.ax1x.com/2023/06/06/pCPq2Hs.png)](https://imgse.com/i/pCPq2Hs)
+
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | 关注推主 | 无 | 否 | 群聊/私聊 | 关注，指令格式：“关注推主 <推主id> [r18]” r18为可选参数，不开启和默认为不推送r18推文|
 | 取关推主 | 无 | 否 | 群聊/私聊 | 取关切割 |
 | 推主列表 | 无 | 否 | 群聊/私聊 | 展示列表 |
 | 推特推送关闭 | 群管 | 否 | 群聊/私聊 | 关闭推送 |
 | 推特推送开启 | 群管 | 否 | 群聊/私聊 | 开启推送 |
 ### 效果图
 [![pCPuhWV.png](https://s1.ax1x.com/2023/06/05/pCPuhWV.png)](https://imgse.com/i/pCPuhWV)
 [![pCPu4zT.png](https://s1.ax1x.com/2023/06/05/pCPu4zT.png)](https://imgse.com/i/pCPu4zT)
 ### 注意事项
-1.消息为合并转发发送，存在延迟和发送失败的可能
+1.推主id：
+[![pCPMu36.png](https://s1.ax1x.com/2023/06/05/pCPMu36.png)](https://imgse.com/i/pCPMu36)
+
+2.消息为合并转发发送，存在延迟和发送失败的可能
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-twitter Version: 0.0.5 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-twitter Version: 0.0.6 Summary:
 NoneBot2 plugin for twitter License: MIT Author-email: nek0us
 gmail.com> Requires-Python: >=3.8 Project-URL: Homepage, https://github.com/
 nek0us/nonebot-plugin-twitter Project-URL: Repository, https://github.com/
 nek0us/nonebot-plugin-twitter Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # nonebot-plugin-twitter _â¨ æ¨æè®¢éæ¨éæä»¶ â¨_ [license] [pypi]
@@ -18,20 +18,23 @@
 [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_twitter"]  ##
 âï¸ éç½® ç³è¯· [twitter api](https://developer.twitter.com/zh-cn/docs/
 twitter-ads-api/getting-started) æé çæå¹¶è®°å½ [Bearer Token](https://
 developer.twitter.com/en/portal/dashboard) [![pCPufJ0.png](https://s1.ax1x.com/
 2023/06/05/pCPufJ0.png)](https://imgse.com/i/pCPufJ0) å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
 é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | bearer_token | æ¯ | æ 
-| Bearer Token | | twitter_proxy | å¦ | æ  | proxy | | command_priority | å¦
-| 10 | å½ä»¤ä¼åçº§ | ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé |
-éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| |
-å³æ³¨æ¨ä¸» | æ  | å¦ | ç¾¤è/ç§è |
-å³æ³¨ï¼æä»¤æ ¼å¼ï¼âå³æ³¨æ¨ä¸» <æ¨ä¸»id> [r18]â
+| Bearer Token | | twitter_proxy | å¦ | æ  | proxy | | twitter_debug | å¦ |
+False | debugæ¨¡å¼ | | command_priority | å¦ | 10 | å½ä»¤ä¼åçº§ | [!
+[pCPq2Hs.png](https://s1.ax1x.com/2023/06/06/pCPq2Hs.png)](https://imgse.com/i/
+pCPq2Hs) ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ |
+è¯´æ | |:-----:|:----:|:----:|:----:|:----:| | å³æ³¨æ¨ä¸» | æ  | å¦ |
+ç¾¤è/ç§è | å³æ³¨ï¼æä»¤æ ¼å¼ï¼âå³æ³¨æ¨ä¸» <æ¨ä¸»id> [r18]â
 r18ä¸ºå¯éåæ°ï¼ä¸å¼å¯åé»è®¤ä¸ºä¸æ¨ér18æ¨æ| | åå³æ¨ä¸» |
 æ  | å¦ | ç¾¤è/ç§è | åå³åå² | | æ¨ä¸»åè¡¨ | æ  | å¦ | ç¾¤è/
 ç§è | å±ç¤ºåè¡¨ | | æ¨ç¹æ¨éå³é­ | ç¾¤ç®¡ | å¦ | ç¾¤è/ç§è |
 å³é­æ¨é | | æ¨ç¹æ¨éå¼å¯ | ç¾¤ç®¡ | å¦ | ç¾¤è/ç§è |
 å¼å¯æ¨é | ### ææå¾ [![pCPuhWV.png](https://s1.ax1x.com/2023/06/05/
 pCPuhWV.png)](https://imgse.com/i/pCPuhWV) [![pCPu4zT.png](https://s1.ax1x.com/
 2023/06/05/pCPu4zT.png)](https://imgse.com/i/pCPu4zT) ### æ³¨æäºé¡¹
-1.æ¶æ¯ä¸ºåå¹¶è½¬ååéï¼å­å¨å»¶è¿ååéå¤±è´¥çå¯è½
+1.æ¨ä¸»idï¼ [![pCPMu36.png](https://s1.ax1x.com/2023/06/05/pCPMu36.png)]
+(https://imgse.com/i/pCPMu36)
+2.æ¶æ¯ä¸ºåå¹¶è½¬ååéï¼å­å¨å»¶è¿ååéå¤±è´¥çå¯è½
```

