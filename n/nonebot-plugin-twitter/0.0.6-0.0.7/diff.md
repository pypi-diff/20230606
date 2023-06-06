# Comparing `tmp/nonebot-plugin-twitter-0.0.6.tar.gz` & `tmp/nonebot-plugin-twitter-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-twitter-0.0.6.tar", last modified: Tue Jun  6 06:01:39 2023, max compression
+gzip compressed data, was "nonebot-plugin-twitter-0.0.7.tar", last modified: Tue Jun  6 06:04:27 2023, max compression
```

## Comparing `nonebot-plugin-twitter-0.0.6.tar` & `nonebot-plugin-twitter-0.0.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2023-06-06 06:01:26.689522 nonebot-plugin-twitter-0.0.6/LICENSE
--rw-r--r--   0        0        0     3369 2023-06-06 06:01:26.689522 nonebot-plugin-twitter-0.0.6/README.md
--rw-r--r--   0        0        0    17458 2023-06-06 06:01:26.689522 nonebot-plugin-twitter-0.0.6/nonebot_plugin_twitter/__init__.py
--rw-r--r--   0        0        0     1252 2023-06-06 06:01:26.689522 nonebot-plugin-twitter-0.0.6/nonebot_plugin_twitter/config.py
--rw-r--r--   0        0        0      646 2023-06-06 06:01:26.689522 nonebot-plugin-twitter-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3737 1970-01-01 00:00:00.000000 nonebot-plugin-twitter-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-06 06:04:17.925635 nonebot-plugin-twitter-0.0.7/LICENSE
+-rw-r--r--   0        0        0     3405 2023-06-06 06:04:17.925635 nonebot-plugin-twitter-0.0.7/README.md
+-rw-r--r--   0        0        0    17458 2023-06-06 06:04:17.929635 nonebot-plugin-twitter-0.0.7/nonebot_plugin_twitter/__init__.py
+-rw-r--r--   0        0        0     1252 2023-06-06 06:04:17.929635 nonebot-plugin-twitter-0.0.7/nonebot_plugin_twitter/config.py
+-rw-r--r--   0        0        0      646 2023-06-06 06:04:17.929635 nonebot-plugin-twitter-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3773 1970-01-01 00:00:00.000000 nonebot-plugin-twitter-0.0.7/PKG-INFO
```

### Comparing `nonebot-plugin-twitter-0.0.6/LICENSE` & `nonebot-plugin-twitter-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.0.6/README.md` & `nonebot-plugin-twitter-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 </details>
 
 ## ⚙️ 配置
 
 申请 [twitter api](https://developer.twitter.com/zh-cn/docs/twitter-ads-api/getting-started) 权限
 
-生成并记录 [Bearer Token](https://developer.twitter.com/en/portal/dashboard)
+创建一个 Project ，生成并记录 API Key 和 [Bearer Token](https://developer.twitter.com/en/portal/dashboard)
 
 [![pCPufJ0.png](https://s1.ax1x.com/2023/06/05/pCPufJ0.png)](https://imgse.com/i/pCPufJ0)
  
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
```

#### html2text {}

```diff
@@ -8,25 +8,26 @@
 ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-twitter   pdm pdm add nonebot-plugin-twitter
 poetry poetry add nonebot-plugin-twitter   conda conda install nonebot-plugin-
 twitter  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
 [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_twitter"]  ##
 âï¸ éç½® ç³è¯· [twitter api](https://developer.twitter.com/zh-cn/docs/
-twitter-ads-api/getting-started) æé çæå¹¶è®°å½ [Bearer Token](https://
-developer.twitter.com/en/portal/dashboard) [![pCPufJ0.png](https://s1.ax1x.com/
-2023/06/05/pCPufJ0.png)](https://imgse.com/i/pCPufJ0) å¨ nonebot2
-é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
-é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | bearer_token | æ¯ | æ 
-| Bearer Token | | twitter_proxy | å¦ | æ  | proxy | | twitter_debug | å¦ |
-False | debugæ¨¡å¼ | | command_priority | å¦ | 10 | å½ä»¤ä¼åçº§ | [!
-[pCPq2Hs.png](https://s1.ax1x.com/2023/06/06/pCPq2Hs.png)](https://imgse.com/i/
-pCPq2Hs) ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ |
-è¯´æ | |:-----:|:----:|:----:|:----:|:----:| | å³æ³¨æ¨ä¸» | æ  | å¦ |
-ç¾¤è/ç§è | å³æ³¨ï¼æä»¤æ ¼å¼ï¼âå³æ³¨æ¨ä¸» <æ¨ä¸»id> [r18]â
+twitter-ads-api/getting-started) æé åå»ºä¸ä¸ª Project ï¼çæå¹¶è®°å½
+API Key å [Bearer Token](https://developer.twitter.com/en/portal/dashboard)
+[![pCPufJ0.png](https://s1.ax1x.com/2023/06/05/pCPufJ0.png)](https://imgse.com/
+i/pCPufJ0) å¨ nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½®
+| éç½®é¡¹ | å¿å¡« | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| |
+bearer_token | æ¯ | æ  | Bearer Token | | twitter_proxy | å¦ | æ  | proxy |
+| twitter_debug | å¦ | False | debugæ¨¡å¼ | | command_priority | å¦ | 10 |
+å½ä»¤ä¼åçº§ | [![pCPq2Hs.png](https://s1.ax1x.com/2023/06/06/pCPq2Hs.png)]
+(https://imgse.com/i/pCPq2Hs) ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé |
+éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| |
+å³æ³¨æ¨ä¸» | æ  | å¦ | ç¾¤è/ç§è |
+å³æ³¨ï¼æä»¤æ ¼å¼ï¼âå³æ³¨æ¨ä¸» <æ¨ä¸»id> [r18]â
 r18ä¸ºå¯éåæ°ï¼ä¸å¼å¯åé»è®¤ä¸ºä¸æ¨ér18æ¨æ| | åå³æ¨ä¸» |
 æ  | å¦ | ç¾¤è/ç§è | åå³åå² | | æ¨ä¸»åè¡¨ | æ  | å¦ | ç¾¤è/
 ç§è | å±ç¤ºåè¡¨ | | æ¨ç¹æ¨éå³é­ | ç¾¤ç®¡ | å¦ | ç¾¤è/ç§è |
 å³é­æ¨é | | æ¨ç¹æ¨éå¼å¯ | ç¾¤ç®¡ | å¦ | ç¾¤è/ç§è |
 å¼å¯æ¨é | ### ææå¾ [![pCPuhWV.png](https://s1.ax1x.com/2023/06/05/
 pCPuhWV.png)](https://imgse.com/i/pCPuhWV) [![pCPu4zT.png](https://s1.ax1x.com/
 2023/06/05/pCPu4zT.png)](https://imgse.com/i/pCPu4zT) ### æ³¨æäºé¡¹
```

### Comparing `nonebot-plugin-twitter-0.0.6/nonebot_plugin_twitter/__init__.py` & `nonebot-plugin-twitter-0.0.7/nonebot_plugin_twitter/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.0.6/nonebot_plugin_twitter/config.py` & `nonebot-plugin-twitter-0.0.7/nonebot_plugin_twitter/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.0.6/pyproject.toml` & `nonebot-plugin-twitter-0.0.7/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-twitter"
-version = "0.0.6"
+version = "0.0.7"
 description = "NoneBot2 plugin for twitter"
 authors = [
     { name = "nek0us", email = "nekouss@gmail.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.1.3",
```

### Comparing `nonebot-plugin-twitter-0.0.6/PKG-INFO` & `nonebot-plugin-twitter-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-twitter
-Version: 0.0.6
+Version: 0.0.7
 Summary: NoneBot2 plugin for twitter
 License: MIT
 Author-email: nek0us <nekouss@gmail.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/nek0us/nonebot-plugin-twitter
 Project-URL: Repository, https://github.com/nek0us/nonebot-plugin-twitter
 Description-Content-Type: text/markdown
@@ -78,15 +78,15 @@
 
 </details>
 
 ## ⚙️ 配置
 
 申请 [twitter api](https://developer.twitter.com/zh-cn/docs/twitter-ads-api/getting-started) 权限
 
-生成并记录 [Bearer Token](https://developer.twitter.com/en/portal/dashboard)
+创建一个 Project ，生成并记录 API Key 和 [Bearer Token](https://developer.twitter.com/en/portal/dashboard)
 
 [![pCPufJ0.png](https://s1.ax1x.com/2023/06/05/pCPufJ0.png)](https://imgse.com/i/pCPufJ0)
  
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-twitter Version: 0.0.6 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-twitter Version: 0.0.7 Summary:
 NoneBot2 plugin for twitter License: MIT Author-email: nek0us
 gmail.com> Requires-Python: >=3.8 Project-URL: Homepage, https://github.com/
 nek0us/nonebot-plugin-twitter Project-URL: Repository, https://github.com/
 nek0us/nonebot-plugin-twitter Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # nonebot-plugin-twitter _â¨ æ¨æè®¢éæ¨éæä»¶ â¨_ [license] [pypi]
@@ -13,25 +13,26 @@
 ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-twitter   pdm pdm add nonebot-plugin-twitter
 poetry poetry add nonebot-plugin-twitter   conda conda install nonebot-plugin-
 twitter  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
 [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_twitter"]  ##
 âï¸ éç½® ç³è¯· [twitter api](https://developer.twitter.com/zh-cn/docs/
-twitter-ads-api/getting-started) æé çæå¹¶è®°å½ [Bearer Token](https://
-developer.twitter.com/en/portal/dashboard) [![pCPufJ0.png](https://s1.ax1x.com/
-2023/06/05/pCPufJ0.png)](https://imgse.com/i/pCPufJ0) å¨ nonebot2
-é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
-é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | bearer_token | æ¯ | æ 
-| Bearer Token | | twitter_proxy | å¦ | æ  | proxy | | twitter_debug | å¦ |
-False | debugæ¨¡å¼ | | command_priority | å¦ | 10 | å½ä»¤ä¼åçº§ | [!
-[pCPq2Hs.png](https://s1.ax1x.com/2023/06/06/pCPq2Hs.png)](https://imgse.com/i/
-pCPq2Hs) ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ |
-è¯´æ | |:-----:|:----:|:----:|:----:|:----:| | å³æ³¨æ¨ä¸» | æ  | å¦ |
-ç¾¤è/ç§è | å³æ³¨ï¼æä»¤æ ¼å¼ï¼âå³æ³¨æ¨ä¸» <æ¨ä¸»id> [r18]â
+twitter-ads-api/getting-started) æé åå»ºä¸ä¸ª Project ï¼çæå¹¶è®°å½
+API Key å [Bearer Token](https://developer.twitter.com/en/portal/dashboard)
+[![pCPufJ0.png](https://s1.ax1x.com/2023/06/05/pCPufJ0.png)](https://imgse.com/
+i/pCPufJ0) å¨ nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½®
+| éç½®é¡¹ | å¿å¡« | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| |
+bearer_token | æ¯ | æ  | Bearer Token | | twitter_proxy | å¦ | æ  | proxy |
+| twitter_debug | å¦ | False | debugæ¨¡å¼ | | command_priority | å¦ | 10 |
+å½ä»¤ä¼åçº§ | [![pCPq2Hs.png](https://s1.ax1x.com/2023/06/06/pCPq2Hs.png)]
+(https://imgse.com/i/pCPq2Hs) ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé |
+éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| |
+å³æ³¨æ¨ä¸» | æ  | å¦ | ç¾¤è/ç§è |
+å³æ³¨ï¼æä»¤æ ¼å¼ï¼âå³æ³¨æ¨ä¸» <æ¨ä¸»id> [r18]â
 r18ä¸ºå¯éåæ°ï¼ä¸å¼å¯åé»è®¤ä¸ºä¸æ¨ér18æ¨æ| | åå³æ¨ä¸» |
 æ  | å¦ | ç¾¤è/ç§è | åå³åå² | | æ¨ä¸»åè¡¨ | æ  | å¦ | ç¾¤è/
 ç§è | å±ç¤ºåè¡¨ | | æ¨ç¹æ¨éå³é­ | ç¾¤ç®¡ | å¦ | ç¾¤è/ç§è |
 å³é­æ¨é | | æ¨ç¹æ¨éå¼å¯ | ç¾¤ç®¡ | å¦ | ç¾¤è/ç§è |
 å¼å¯æ¨é | ### ææå¾ [![pCPuhWV.png](https://s1.ax1x.com/2023/06/05/
 pCPuhWV.png)](https://imgse.com/i/pCPuhWV) [![pCPu4zT.png](https://s1.ax1x.com/
 2023/06/05/pCPu4zT.png)](https://imgse.com/i/pCPu4zT) ### æ³¨æäºé¡¹
```

