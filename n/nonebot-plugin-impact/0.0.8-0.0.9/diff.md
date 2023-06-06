# Comparing `tmp/nonebot_plugin_impact-0.0.8.tar.gz` & `tmp/nonebot_plugin_impact-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_impact-0.0.8.tar", last modified: Sat May 20 09:38:08 2023, max compression
+gzip compressed data, was "nonebot_plugin_impact-0.0.9.tar", last modified: Tue Jun  6 14:47:52 2023, max compression
```

## Comparing `nonebot_plugin_impact-0.0.8.tar` & `nonebot_plugin_impact-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 09:38:08.201155 nonebot_plugin_impact-0.0.8/
--rw-rw-rw-   0        0        0     1090 2023-01-30 13:38:17.000000 nonebot_plugin_impact-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      283 2023-05-20 09:38:08.200155 nonebot_plugin_impact-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-20 09:38:08.190157 nonebot_plugin_impact-0.0.8/nonebot_plugin_impact/
--rw-rw-rw-   0        0        0     1530 2023-05-20 09:26:09.000000 nonebot_plugin_impact-0.0.8/nonebot_plugin_impact/__init__.py
--rw-rw-rw-   0        0        0    19878 2023-05-20 09:33:27.000000 nonebot_plugin_impact-0.0.8/nonebot_plugin_impact/handle.py
--rw-rw-rw-   0        0        0     2041 2023-05-20 08:48:33.000000 nonebot_plugin_impact-0.0.8/nonebot_plugin_impact/txt2img.py
--rw-rw-rw-   0        0        0     8376 2023-05-20 09:22:54.000000 nonebot_plugin_impact-0.0.8/nonebot_plugin_impact/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-20 09:38:08.199162 nonebot_plugin_impact-0.0.8/nonebot_plugin_impact.egg-info/
--rw-rw-rw-   0        0        0      283 2023-05-20 09:38:08.000000 nonebot_plugin_impact-0.0.8/nonebot_plugin_impact.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2023-05-20 09:38:08.000000 nonebot_plugin_impact-0.0.8/nonebot_plugin_impact.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 09:38:08.000000 nonebot_plugin_impact-0.0.8/nonebot_plugin_impact.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-05-20 09:38:08.000000 nonebot_plugin_impact-0.0.8/nonebot_plugin_impact.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-05-20 09:38:08.000000 nonebot_plugin_impact-0.0.8/nonebot_plugin_impact.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 09:38:08.201155 nonebot_plugin_impact-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      503 2023-05-20 09:38:04.000000 nonebot_plugin_impact-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 14:47:52.262724 nonebot_plugin_impact-0.0.9/
+-rw-rw-rw-   0        0        0     1090 2023-01-30 13:38:17.000000 nonebot_plugin_impact-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      283 2023-06-06 14:47:52.261723 nonebot_plugin_impact-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-06 14:47:52.254724 nonebot_plugin_impact-0.0.9/nonebot_plugin_impact/
+-rw-rw-rw-   0        0        0     1667 2023-06-06 14:37:05.000000 nonebot_plugin_impact-0.0.9/nonebot_plugin_impact/__init__.py
+-rw-rw-rw-   0        0        0    19722 2023-06-06 14:39:44.000000 nonebot_plugin_impact-0.0.9/nonebot_plugin_impact/handle.py
+-rw-rw-rw-   0        0        0     2041 2023-06-06 14:34:38.000000 nonebot_plugin_impact-0.0.9/nonebot_plugin_impact/txt2img.py
+-rw-rw-rw-   0        0        0     8376 2023-06-06 14:34:38.000000 nonebot_plugin_impact-0.0.9/nonebot_plugin_impact/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-06 14:47:52.260722 nonebot_plugin_impact-0.0.9/nonebot_plugin_impact.egg-info/
+-rw-rw-rw-   0        0        0      283 2023-06-06 14:47:52.000000 nonebot_plugin_impact-0.0.9/nonebot_plugin_impact.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      370 2023-06-06 14:47:52.000000 nonebot_plugin_impact-0.0.9/nonebot_plugin_impact.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 14:47:52.000000 nonebot_plugin_impact-0.0.9/nonebot_plugin_impact.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-06-06 14:47:52.000000 nonebot_plugin_impact-0.0.9/nonebot_plugin_impact.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-06 14:47:52.000000 nonebot_plugin_impact-0.0.9/nonebot_plugin_impact.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 14:47:52.262724 nonebot_plugin_impact-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      503 2023-06-06 14:47:26.000000 nonebot_plugin_impact-0.0.9/setup.py
```

### Comparing `nonebot_plugin_impact-0.0.8/LICENSE` & `nonebot_plugin_impact-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_impact-0.0.8/nonebot_plugin_impact/__init__.py` & `nonebot_plugin_impact-0.0.9/nonebot_plugin_impact/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,13 +18,16 @@
 on_command("淫趴介绍", priority=20, block=True)
 
 
 __plugin_meta__ = PluginMetadata(
     name="impact",
     description="让群友们眼前一黑的nonebot2淫趴插件",
     usage=utils.usage,
+    type="application",
+    homepage="https://github.com/Special-Week/nonebot_plugin_impact",
+    supported_adapters={"~onebot.v11"},
     extra={
         'author':   'Special-Week',
         'version':  '?.?.?',
         'priority': 20,
     }
 )
```

### Comparing `nonebot_plugin_impact-0.0.8/nonebot_plugin_impact/handle.py` & `nonebot_plugin_impact-0.0.9/nonebot_plugin_impact/handle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import asyncio
 import random
 import time
 from random import choice
-from typing import List, Tuple
+from typing import Tuple
 
 from nonebot.adapters.onebot.v11 import (Bot, GroupMessageEvent, Message,
                                          MessageSegment)
 from nonebot.matcher import Matcher
-from nonebot.params import CommandArg
-from nonebot.typing import T_State
+from nonebot.params import CommandArg, RegexGroup
 
 from .txt2img import txt_to_img
 from .utils import utils
 
 
 class Impart:
     def __init__(self) -> None:
@@ -191,27 +190,26 @@
         reply2 = f"你的排名为{index[0]+1}喵"
         await matcher.finish(reply+MessageSegment.image(img_bytes)+reply2, at_sender=True)
 
 
     async def yinpa_prehandle(
         self,
         bot: Bot,
-        state: T_State,
+        args: Tuple,
         matcher: Matcher,
         event: GroupMessageEvent,
     ) -> Tuple[int, int, str, str, list]:
         """透群员的预处理环节"""
         gid, uid  = event.group_id, event.user_id
         if not (await utils.check_group_allow(str(gid))):
             await matcher.finish(utils.not_allow, at_sender=True)
         allow = await utils.fuck_cd_check(event)  # CD检查是否允许
         if not allow:
             await matcher.finish(f"你已经榨不出来任何东西了, 请先休息{round(utils.fuck_cd_time-(time.time() - utils.ejaculation_cd[str(uid)]),3)}秒", at_sender=True)
         utils.ejaculation_cd.update({str(uid): time.time()})  # 记录时间
-        args = list(state["_matched_groups"])
         req_user_card = await utils.get_user_card(bot, group_id=int(gid), qid=int(uid))
         prep_list = await bot.get_group_member_list(group_id=gid)
         return gid,uid,req_user_card, args[0],prep_list
     
 
     async def yinpa_member_handle(
         self,
@@ -284,17 +282,17 @@
     
 
     async def yinpa(
         self,
         bot: Bot, 
         matcher: Matcher,
         event: GroupMessageEvent, 
-        state: T_State
+        args: Tuple = RegexGroup()
     ) -> None:
-        gid, uid, req_user_card, command ,prep_list= await self.yinpa_prehandle(matcher=matcher, bot=bot, state=state, event=event)
+        gid, uid, req_user_card, command ,prep_list= await self.yinpa_prehandle(matcher=matcher, bot=bot, args=args, event=event)
         lucky_user: str = await self.yinpa_identity_handle(command=command, prep_list=prep_list, req_user_card=req_user_card, matcher=matcher, event=event)
         # 获取群名片或者网名
         lucky_user_card = await utils.get_user_card(bot, gid, int(lucky_user))
         # 1--100的随机数， 保留三位
         ejaculation = round(random.uniform(1, 100), 3)
         try:
             temp = (
@@ -310,22 +308,20 @@
         # 准备调用api, 用来获取头像
         repo_1 = f"好欸！{req_user_card}({uid})用时{random.randint(1, 20)}秒 \n给 {lucky_user_card}({lucky_user}) 注入了{ejaculation}毫升的脱氧核糖核酸, 当日总注入量为：{utils.get_today_ejaculation(lucky_user)}"
         await matcher.send(repo_1 + MessageSegment.image(f"http://q1.qlogo.cn/g?b=qq&nk={lucky_user}&s=640"))  # 结束
 
 
     async def open_module(
         self,
-        state: T_State,
         matcher: Matcher,
         event: GroupMessageEvent,
+        args: Tuple = RegexGroup()
     ) -> None:
         """开关"""
         gid = str(event.group_id)
-        # 获取用户输入的参数
-        args: List[str] = list(state["_matched_groups"])
         command: str = args[0]
         if "开启" in command or "开始" in command:
             if gid in utils.groupdata:
                 utils.groupdata[gid]["allow"] = True
             else:
                 utils.groupdata.update({gid: {"allow": True}})
             utils.write_group_data()
```

### Comparing `nonebot_plugin_impact-0.0.8/nonebot_plugin_impact/txt2img.py` & `nonebot_plugin_impact-0.0.9/nonebot_plugin_impact/txt2img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_impact-0.0.8/nonebot_plugin_impact/utils.py` & `nonebot_plugin_impact-0.0.9/nonebot_plugin_impact/utils.py`

 * *Files identical despite different names*

