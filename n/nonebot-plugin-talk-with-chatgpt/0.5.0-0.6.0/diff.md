# Comparing `tmp/nonebot_plugin_talk_with_chatgpt-0.5.0.tar.gz` & `tmp/nonebot_plugin_talk_with_chatgpt-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_talk_with_chatgpt-0.5.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_talk_with_chatgpt-0.6.0.tar", max compression
```

## Comparing `nonebot_plugin_talk_with_chatgpt-0.5.0.tar` & `nonebot_plugin_talk_with_chatgpt-0.6.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0    10090 2023-05-30 10:07:54.317440 nonebot_plugin_talk_with_chatgpt-0.5.0/nonebot_plugin_talk_with_chatgpt/__init__.py
--rw-r--r--   0        0        0    13618 2023-05-30 10:02:32.009797 nonebot_plugin_talk_with_chatgpt-0.5.0/nonebot_plugin_talk_with_chatgpt/config.py
--rw-r--r--   0        0        0     5281 2023-05-18 02:26:25.865457 nonebot_plugin_talk_with_chatgpt-0.5.0/nonebot_plugin_talk_with_chatgpt/data_handle.py
--rw-r--r--   0        0        0      974 2023-05-30 10:08:15.992724 nonebot_plugin_talk_with_chatgpt-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     5588 2023-05-30 10:11:45.805532 nonebot_plugin_talk_with_chatgpt-0.5.0/README.md
--rw-r--r--   0        0        0     6505 1970-01-01 00:00:00.000000 nonebot_plugin_talk_with_chatgpt-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    10762 2023-06-06 06:19:54.130482 nonebot_plugin_talk_with_chatgpt-0.6.0/nonebot_plugin_talk_with_chatgpt/__init__.py
+-rw-r--r--   0        0        0    14035 2023-06-06 06:18:10.409339 nonebot_plugin_talk_with_chatgpt-0.6.0/nonebot_plugin_talk_with_chatgpt/config.py
+-rw-r--r--   0        0        0     6397 2023-06-06 06:12:19.089000 nonebot_plugin_talk_with_chatgpt-0.6.0/nonebot_plugin_talk_with_chatgpt/data_handle.py
+-rw-r--r--   0        0        0  7232220 2023-01-06 09:31:31.000000 nonebot_plugin_talk_with_chatgpt-0.6.0/nonebot_plugin_talk_with_chatgpt/HYWenHei-85W.ttf
+-rw-r--r--   0        0        0      994 2023-06-06 06:47:18.019759 nonebot_plugin_talk_with_chatgpt-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6039 2023-06-06 06:47:10.419571 nonebot_plugin_talk_with_chatgpt-0.6.0/README.md
+-rw-r--r--   0        0        0     6977 1970-01-01 00:00:00.000000 nonebot_plugin_talk_with_chatgpt-0.6.0/PKG-INFO
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.5.0/nonebot_plugin_talk_with_chatgpt/__init__.py` & `nonebot_plugin_talk_with_chatgpt-0.6.0/nonebot_plugin_talk_with_chatgpt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 from nonebot import on_message, on_fullmatch
 from nonebot.adapters.onebot.v11 import (
     Bot,
     MessageEvent,
     GroupMessageEvent,
     PrivateMessageEvent,
+    MessageSegment as MS,
 )
 from nonebot.log import logger
 from nonebot.plugin import PluginMetadata
 from .config import pc, var
-from .data_handle import req_chatgpt
+from .data_handle import req_chatgpt, text_to_img
 from nonebot.typing import T_State
 from html import unescape
 from nonebot.permission import SUPERUSER
 
 talk_cmd = pc.talk_with_chatgpt_talk_cmd
 talk_p_cmd = pc.talk_with_chatgpt_talk_p_cmd
 reset_cmd = pc.talk_with_chatgpt_reset_cmd
 prompt_cmd = pc.talk_with_chatgpt_prompt_cmd
 enable_cmd = pc.talk_with_chatgpt_group_enable_cmd
 
 __plugin_meta__ = PluginMetadata(
     name="talk with chatgpt",
     description="一个简单的基于accessToken验证的ChatGPT对话插件",
     usage=f"""插件命令如下
-{talk_cmd}  # 开始对话，默认群里@机器人也可以
-{reset_cmd}  # 重置对话（不会重置预设）
-{prompt_cmd}  # 设置预设（人格），设置后会重置对话
-{enable_cmd}  # 如果关闭所有群启用，则用这个命令启用
+{talk_cmd}   # 开始对话，默认群里@机器人也可以
+{reset_cmd}   # 重置对话（不会重置预设）
+{prompt_cmd}   # 设置预设（人格），设置后会重置对话
+{enable_cmd}   # 如果关闭所有群启用，则用这个命令启用
 """,
 )
 
 
 def get_id(event: MessageEvent) -> str:
     """获取会话id"""
     if isinstance(event, GroupMessageEvent):
@@ -68,18 +69,19 @@
         # 仅艾特但没发内容
         if event.is_tome() and pc.talk_with_chatgpt_talk_at:
             if text:
                 return True
             else:
                 return False
 
+        # 判断命令前缀
         return text[: len(talk_cmd)] == talk_cmd
 
     elif isinstance(event, PrivateMessageEvent):
-        # 判断前缀
+        # 判断命令前缀
         return text[: len(talk_cmd)] == talk_cmd
 
     return False
 
 
 async def rule_check2(event: MessageEvent, bot: Bot) -> bool:
     """其他命令判断"""
@@ -156,14 +158,22 @@
     id = get_id(event)
 
     # 根据配置是否发出提示
     if pc.talk_with_chatgpt_reply_notice:
         await talk.send("响应中...")
 
     result = await req_chatgpt(id, text)
+    if pc.talk_with_chatgpt_ban_word:
+        for w in pc.talk_with_chatgpt_ban_word:
+            if w in result:
+                result = "本次回答中包含屏蔽词！"
+                break
+
+    if pc.talk_with_chatgpt_send_with_img:
+        result = MS.image(text_to_img(result))
     await talk.finish(result, at_sender=True)
 
 
 @talk_p.got("msg", prompt="进入沉浸式对话模式，发送“退出”结束对话")
 async def _(event: PrivateMessageEvent):
     # 获取信息
     text = unescape(event.get_plaintext().strip())
@@ -173,14 +183,22 @@
     id = get_id(event)
 
     # 根据配置是否发出提示
     if pc.talk_with_chatgpt_reply_notice:
         await talk_p.send("响应中...")
 
     result = await req_chatgpt(id, text)
+    if pc.talk_with_chatgpt_ban_word:
+        for w in pc.talk_with_chatgpt_ban_word:
+            if w in result:
+                result = "本次回答中包含屏蔽词！"
+                break
+
+    if pc.talk_with_chatgpt_send_with_img:
+        result = MS.image(text_to_img(result))
     await talk_p.reject(result)
 
 
 @reset.handle()
 async def _(event: MessageEvent):
     # 获取用户id
     id = get_id(event)
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.5.0/nonebot_plugin_talk_with_chatgpt/config.py` & `nonebot_plugin_talk_with_chatgpt-0.6.0/nonebot_plugin_talk_with_chatgpt/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,37 +23,47 @@
     talk_with_chatgpt_reply_notice: bool = True
     # 群聊是否共享会话
     talk_with_chatgpt_group_share: bool = False
     # 只允许超级管理员修改预设
     talk_with_chatgpt_prompt_admin_only: bool = True
     # 是否默认允许所有群聊使用，否则需要使用命令启用
     talk_with_chatgpt_all_group_enable: bool = True
+    # 机器人的回复是否使用图片发送
+    talk_with_chatgpt_send_with_img: bool = False
 
     # 群聊艾特是否响应
     talk_with_chatgpt_talk_at: bool = True
     # 触发对话的命令前缀，群聊直接艾特也可以触发
     talk_with_chatgpt_talk_cmd: str = "/talk"
     # 私聊沉浸式对话触发命令
     talk_with_chatgpt_talk_p_cmd: str = "/hi"
     # 重置对话，就是清空聊天记录
     talk_with_chatgpt_reset_cmd: str = "/reset"
     # 设置预设
     talk_with_chatgpt_prompt_cmd: str = "/prompt"
     # 如果关闭所有群聊使用，启用该群的命令
     talk_with_chatgpt_group_enable_cmd: str = "/chatgpt"
 
+    # 敏感词屏蔽，默认不屏蔽任何词
+    talk_with_chatgpt_ban_word: List[str] = []
     # 请求超时时间
     talk_with_chatgpt_timeout: int = 60
     # chatgpt模型
     talk_with_chatgpt_api_model: str = "text-davinci-002-render-sha"
 
     # 机器人的QQ号（如果写了就按优先级响应，否则就第一个连上的响应） [1234, 5678, 6666]  ["all"]则全部响应
     talk_with_chatgpt_bot_qqnum_list: List[str] = []  # 可选
     # 插件数据文件名
     talk_with_chatgpt_data: str = "talk_with_chatgpt.json"
+    # 字体文件路径
+    talk_with_chatgpt_font_path: str = str(
+        path.join(path.dirname(path.abspath(__file__)), "HYWenHei-85W.ttf")
+    )
+    # 字体大小
+    talk_with_chatgpt_font_size: int = 18
 
 
 driver = get_driver()
 global_config = driver.config
 pc = Config.parse_obj(global_config)
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.5.0/nonebot_plugin_talk_with_chatgpt/data_handle.py` & `nonebot_plugin_talk_with_chatgpt-0.6.0/nonebot_plugin_talk_with_chatgpt/data_handle.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from .config import pc, var
 from nonebot.log import logger
 from ujson import loads
 from asyncio import Future, sleep, Queue, create_task
 from ujson import dumps, loads
 from uuid import uuid4
 from nonebot import get_driver
+from PIL import Image, ImageDraw, ImageFont
+from io import BytesIO
 
 driver = get_driver()
 
 
 @driver.on_startup
 async def _():
     """处理队列协程"""
@@ -140,7 +142,39 @@
     # 如果是开发者模式只取需要的回答
     if var.session_data[id][2] == "开发者模式":
         resp_text = resp_text.replace("(Normal Output) ", "")
         if "(Developer Mode Output) " in resp_text:
             resp_text = resp_text.split("(Developer Mode Output) ")[1]
 
     return resp_text
+
+
+# 文字转图片
+def text_to_img(text: str, font_path: str = pc.talk_with_chatgpt_font_path) -> BytesIO:
+    """
+    字转图片
+    """
+    lines = text.splitlines()
+    line_count = len(lines)
+    # 读取字体
+    font = ImageFont.truetype(font_path, pc.talk_with_chatgpt_font_size)
+    # 获取字体的行高
+    left, top, width, line_height = font.getbbox("a")
+    # 增加行距
+    line_height += 3
+    # 获取画布需要的高度
+    height = line_height * line_count + 20
+    # 获取画布需要的宽度
+    width = int(max([font.getlength(line) for line in lines])) + 25
+    # 字体颜色
+    black_color = (0, 0, 0)
+    # 生成画布
+    image = Image.new("RGB", (width, height), (255, 255, 255))
+    draw = ImageDraw.Draw(image)
+    # 按行开画，c是计算写到第几行
+    c = 0
+    for line in lines:
+        draw.text((10, 6 + line_height * c), line, font=font, fill=black_color)
+        c += 1
+    img_bytes = BytesIO()
+    image.save(img_bytes, format="jpeg")
+    return img_bytes
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.5.0/pyproject.toml` & `nonebot_plugin_talk_with_chatgpt-0.6.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_talk_with_chatgpt"
-version = "0.5.0"
+version = "0.6.0"
 description = "Nonebot2 基于accessToken登录的ChatGPT聊天插件"
 authors = ["nikissXI <1299577815@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_talk_with_chatgpt"}]
 homepage = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt"
 repository = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt"
@@ -17,11 +17,12 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 nonebot2 = ">=2.0.0rc1"
 nonebot-adapter-onebot = ">=2.0.0"
 httpx = ">=0.22.0"
 ujson = ">=5.0.0"
+Pillow = ">=9.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.5.0/README.md` & `nonebot_plugin_talk_with_chatgpt-0.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,16 @@
 talk_with_chatgpt_reply_notice = true
 # 群聊是否共享会话
 talk_with_chatgpt_group_share = false
 # 只允许超级管理员修改预设
 talk_with_chatgpt_prompt_admin_only = true
 # 是否默认允许所有群聊使用，否则需要使用命令启用
 talk_with_chatgpt_all_group_enable = true
+# 机器人的回复是否使用图片发送
+talk_with_chatgpt_send_with_img = false
 ```
 
 #### 如果要修改触发命令就填
 ```bash
 # 群聊艾特是否响应
 talk_with_chatgpt_talk_at = true
 # 触发对话的命令前缀，默认群聊直接艾特也可以触发
@@ -80,39 +82,48 @@
 talk_with_chatgpt_prompt_cmd = /prompt
 # 如果关闭所有群聊使用，启用该群的命令
 talk_with_chatgpt_group_enable_cmd = /chatgpt
 ```
 
 #### 大概率用不上的选填项
 ```bash
+# 敏感词屏蔽，默认不屏蔽任何词
+talk_with_chatgpt_ban_word = ["示例词1", "示例词2"]
 # 请求超时时间，回答生成的时间也要算在这里面的，所以不能太短，默认60秒
 talk_with_chatgpt_timeout = 60
 # chatgpt模型，默认 text-davinci-002-render-sha，更多模型请参考 https://platform.openai.com/docs/models
 talk_with_chatgpt_api_model = text-davinci-002-render-sha
 
 # 机器人的QQ号列表，选填
 # 如果有多个bot连接，会按照填写的list，左边的机器人QQ优先级最高 1234 > 5678 > 6666，会自动切换
 # 如果不填该配置则由第一个连上的bot响应，所以单bot连可以不填，写 ["all"]则所有机器人均响应
 talk_with_chatgpt_bot_qqnum_list = [1234, 5678, 6666]
 # 插件数据文件名，默认./data/talk_with_chatgpt.json
 talk_with_chatgpt_data = talk_with_chatgpt.json
+# 如果使用图片回复，字体大小
+talk_with_chatgpt_font_size = 18
 ```
 
 ## 插件命令（均可修改！） 
 | 指令 | 说明 |
 |:-----:|:----:|
 | /talk | 开始对话，默认群里@机器人也可以 |
 | /hi | 沉浸式对话（仅限私聊） |
 | /reset | 重置对话（不会重置预设） |
 | /prompt | 设置预设（人格），设置后会重置对话 |
+| /chatgpt | 设置预设（人格），设置后会重置对话 |
 
 ## 更新日志
+### 2023/6/6 \[v0.6.0]
+
+* 新增配置项 talk_with_chatgpt_send_with_img 和 talk_with_chatgpt_ban_word
+
 ### 2023/5/30 \[v0.5.0]
 
-* 更换了自带预设“猫娘”的内容，新增配置项talk_with_chatgpt_all_group_enable和talk_with_chatgpt_group_enable_cmd，新增命令/chatgpt
+* 更换了自带预设“猫娘”的内容，新增配置项 talk_with_chatgpt_all_group_enable 和 talk_with_chatgpt_group_enable_cmd ，新增命令/chatgpt
 
 ### 2023/5/29 \[v0.4.3]
 
 * [支持所有机器人响应命令](https://github.com/nikissXI/nonebot_plugins/issues/22)
 
 ### 2023/5/18 \[v0.4.2]
```

#### html2text {}

```diff
@@ -27,45 +27,53 @@
 ai.fakeopen.com/api/conversation #
 é»è®¤æ ä»£çï¼è§apiæåµçæ¯å¦éè¦æ¢¯å­ãè¿ä¸ªåç½®çåä»£ææµè¿æ¯ä¸éè¦æ¢¯å­çã
 talk_with_chatgpt_http_proxy = null # å¤çæ¶æ¯æ¶æ¯å¦æç¤º
 talk_with_chatgpt_reply_notice = true # ç¾¤èæ¯å¦å±äº«ä¼è¯
 talk_with_chatgpt_group_share = false # åªåè®¸è¶çº§ç®¡çåä¿®æ¹é¢è®¾
 talk_with_chatgpt_prompt_admin_only = true #
 æ¯å¦é»è®¤åè®¸ææç¾¤èä½¿ç¨ï¼å¦åéè¦ä½¿ç¨å½ä»¤å¯ç¨
-talk_with_chatgpt_all_group_enable = true ``` ####
-å¦æè¦ä¿®æ¹è§¦åå½ä»¤å°±å¡« ```bash # ç¾¤èè¾ç¹æ¯å¦ååº
-talk_with_chatgpt_talk_at = true #
+talk_with_chatgpt_all_group_enable = true #
+æºå¨äººçåå¤æ¯å¦ä½¿ç¨å¾çåé talk_with_chatgpt_send_with_img =
+false ``` #### å¦æè¦ä¿®æ¹è§¦åå½ä»¤å°±å¡« ```bash #
+ç¾¤èè¾ç¹æ¯å¦ååº talk_with_chatgpt_talk_at = true #
 è§¦åå¯¹è¯çå½ä»¤åç¼ï¼é»è®¤ç¾¤èç´æ¥è¾ç¹ä¹å¯ä»¥è§¦å
 talk_with_chatgpt_talk_cmd = /talk # ç§èæ²æµ¸å¼å¯¹è¯è§¦åå½ä»¤
 talk_with_chatgpt_talk_p_cmd = /hi #
 éç½®å¯¹è¯çå½ä»¤ï¼å°±æ¯æ¸ç©ºèå¤©è®°å½ talk_with_chatgpt_reset_cmd =
 /reset # è®¾ç½®é¢è®¾çå½ä»¤åç¼ talk_with_chatgpt_prompt_cmd = /prompt #
 å¦æå³é­ææç¾¤èä½¿ç¨ï¼å¯ç¨è¯¥ç¾¤çå½ä»¤
 talk_with_chatgpt_group_enable_cmd = /chatgpt ``` ####
 å¤§æ¦çç¨ä¸ä¸çéå¡«é¡¹ ```bash #
+ææè¯å±è½ï¼é»è®¤ä¸å±è½ä»»ä½è¯ talk_with_chatgpt_ban_word =
+["ç¤ºä¾è¯1", "ç¤ºä¾è¯2"] #
 è¯·æ±è¶æ¶æ¶é´ï¼åç­çæçæ¶é´ä¹è¦ç®å¨è¿éé¢çï¼æä»¥ä¸è½å¤ªç­ï¼é»è®¤60ç§
 talk_with_chatgpt_timeout = 60 # chatgptæ¨¡åï¼é»è®¤ text-davinci-002-
 render-shaï¼æ´å¤æ¨¡åè¯·åè https://platform.openai.com/docs/models
 talk_with_chatgpt_api_model = text-davinci-002-render-sha #
 æºå¨äººçQQå·åè¡¨ï¼éå¡« #
 å¦ææå¤ä¸ªbotè¿æ¥ï¼ä¼æç§å¡«åçlistï¼å·¦è¾¹çæºå¨äººQQä¼åçº§æé«
 1234 > 5678 > 6666ï¼ä¼èªå¨åæ¢ #
 å¦æä¸å¡«è¯¥éç½®åç±ç¬¬ä¸ä¸ªè¿ä¸çbotååºï¼æä»¥åbotè¿å¯ä»¥ä¸å¡«ï¼å
 ["all"]åæææºå¨äººåååº talk_with_chatgpt_bot_qqnum_list = [1234,
 5678, 6666] # æä»¶æ°æ®æä»¶åï¼é»è®¤./data/talk_with_chatgpt.json
-talk_with_chatgpt_data = talk_with_chatgpt.json ``` ##
+talk_with_chatgpt_data = talk_with_chatgpt.json #
+å¦æä½¿ç¨å¾çåå¤ï¼å­ä½å¤§å° talk_with_chatgpt_font_size = 18 ``` ##
 æä»¶å½ä»¤ï¼åå¯ä¿®æ¹ï¼ï¼ | æä»¤ | è¯´æ | |:-----:|:----:| | /talk
 | å¼å§å¯¹è¯ï¼é»è®¤ç¾¤é@æºå¨äººä¹å¯ä»¥ | | /hi |
 æ²æµ¸å¼å¯¹è¯ï¼ä»éç§èï¼ | | /reset |
 éç½®å¯¹è¯ï¼ä¸ä¼éç½®é¢è®¾ï¼ | | /prompt |
+è®¾ç½®é¢è®¾ï¼äººæ ¼ï¼ï¼è®¾ç½®åä¼éç½®å¯¹è¯ | | /chatgpt |
 è®¾ç½®é¢è®¾ï¼äººæ ¼ï¼ï¼è®¾ç½®åä¼éç½®å¯¹è¯ | ## æ´æ°æ¥å¿ ### 2023/
-5/30 \[v0.5.0] *
-æ´æ¢äºèªå¸¦é¢è®¾âç«å¨âçåå®¹ï¼æ°å¢éç½®é¡¹talk_with_chatgpt_all_group_enableåtalk_with_chatgpt_group_enable_cmdï¼æ°å¢å½ä»¤/
-chatgpt ### 2023/5/29 \[v0.4.3] * [æ¯ææææºå¨äººååºå½ä»¤](https://
-github.com/nikissXI/nonebot_plugins/issues/22) ### 2023/5/18 \[v0.4.2] *
+6/6 \[v0.6.0] * æ°å¢éç½®é¡¹ talk_with_chatgpt_send_with_img å
+talk_with_chatgpt_ban_word ### 2023/5/30 \[v0.5.0] *
+æ´æ¢äºèªå¸¦é¢è®¾âç«å¨âçåå®¹ï¼æ°å¢éç½®é¡¹
+talk_with_chatgpt_all_group_enable å talk_with_chatgpt_group_enable_cmd
+ï¼æ°å¢å½ä»¤/chatgpt ### 2023/5/29 \[v0.4.3] *
+[æ¯ææææºå¨äººååºå½ä»¤](https://github.com/nikissXI/
+nonebot_plugins/issues/22) ### 2023/5/18 \[v0.4.2] *
 [ä¿®å¤ä¼è¯ä¸¢å¤±ä¸éç½®çé®é¢](https://github.com/nikissXI/
 nonebot_plugins/issues/21) ### 2023/4/22 \[v0.4.1] *
 [å¢å ç¾¤èatè§¦åå¼å³](https://github.com/nikissXI/nonebot_plugins/
 issues/21) ### 2023/4/21 \[v0.4.0] *
 æ´æ¢äºé»è®¤APIï¼ææ¶è½ç¨ï¼å»ºè®®è¿æ¯èªå·±æ­å»ºAPI *
 æ°å¢å¤é¢è®¾åè½ï¼åç½®ä¸ä¸ªé¢è®¾ï¼ç«å¨ãé­é­ãå¼åèæ¨¡å¼
 * å¢å ç§èæ²æµ¸å¼å¯¹è¯ * ä¼åå¤§éç»è ### 2023/4/11 \[v0.2.3] *
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.5.0/PKG-INFO` & `nonebot_plugin_talk_with_chatgpt-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-talk-with-chatgpt
-Version: 0.5.0
+Version: 0.6.0
 Summary: Nonebot2 基于accessToken登录的ChatGPT聊天插件
 Home-page: https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt
 License: MIT
 Author: nikissXI
 Author-email: 1299577815@qq.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Pillow (>=9.0.0)
 Requires-Dist: httpx (>=0.22.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.0.0)
 Requires-Dist: nonebot2 (>=2.0.0rc1)
 Requires-Dist: ujson (>=5.0.0)
 Project-URL: Documentation, https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt#README.md
 Project-URL: Repository, https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt
 Description-Content-Type: text/markdown
@@ -83,14 +84,16 @@
 talk_with_chatgpt_reply_notice = true
 # 群聊是否共享会话
 talk_with_chatgpt_group_share = false
 # 只允许超级管理员修改预设
 talk_with_chatgpt_prompt_admin_only = true
 # 是否默认允许所有群聊使用，否则需要使用命令启用
 talk_with_chatgpt_all_group_enable = true
+# 机器人的回复是否使用图片发送
+talk_with_chatgpt_send_with_img = false
 ```
 
 #### 如果要修改触发命令就填
 ```bash
 # 群聊艾特是否响应
 talk_with_chatgpt_talk_at = true
 # 触发对话的命令前缀，默认群聊直接艾特也可以触发
@@ -103,39 +106,48 @@
 talk_with_chatgpt_prompt_cmd = /prompt
 # 如果关闭所有群聊使用，启用该群的命令
 talk_with_chatgpt_group_enable_cmd = /chatgpt
 ```
 
 #### 大概率用不上的选填项
 ```bash
+# 敏感词屏蔽，默认不屏蔽任何词
+talk_with_chatgpt_ban_word = ["示例词1", "示例词2"]
 # 请求超时时间，回答生成的时间也要算在这里面的，所以不能太短，默认60秒
 talk_with_chatgpt_timeout = 60
 # chatgpt模型，默认 text-davinci-002-render-sha，更多模型请参考 https://platform.openai.com/docs/models
 talk_with_chatgpt_api_model = text-davinci-002-render-sha
 
 # 机器人的QQ号列表，选填
 # 如果有多个bot连接，会按照填写的list，左边的机器人QQ优先级最高 1234 > 5678 > 6666，会自动切换
 # 如果不填该配置则由第一个连上的bot响应，所以单bot连可以不填，写 ["all"]则所有机器人均响应
 talk_with_chatgpt_bot_qqnum_list = [1234, 5678, 6666]
 # 插件数据文件名，默认./data/talk_with_chatgpt.json
 talk_with_chatgpt_data = talk_with_chatgpt.json
+# 如果使用图片回复，字体大小
+talk_with_chatgpt_font_size = 18
 ```
 
 ## 插件命令（均可修改！） 
 | 指令 | 说明 |
 |:-----:|:----:|
 | /talk | 开始对话，默认群里@机器人也可以 |
 | /hi | 沉浸式对话（仅限私聊） |
 | /reset | 重置对话（不会重置预设） |
 | /prompt | 设置预设（人格），设置后会重置对话 |
+| /chatgpt | 设置预设（人格），设置后会重置对话 |
 
 ## 更新日志
+### 2023/6/6 \[v0.6.0]
+
+* 新增配置项 talk_with_chatgpt_send_with_img 和 talk_with_chatgpt_ban_word
+
 ### 2023/5/30 \[v0.5.0]
 
-* 更换了自带预设“猫娘”的内容，新增配置项talk_with_chatgpt_all_group_enable和talk_with_chatgpt_group_enable_cmd，新增命令/chatgpt
+* 更换了自带预设“猫娘”的内容，新增配置项 talk_with_chatgpt_all_group_enable 和 talk_with_chatgpt_group_enable_cmd ，新增命令/chatgpt
 
 ### 2023/5/29 \[v0.4.3]
 
 * [支持所有机器人响应命令](https://github.com/nikissXI/nonebot_plugins/issues/22)
 
 ### 2023/5/18 \[v0.4.2]
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-talk-with-chatgpt Version: 0.5.0
+Metadata-Version: 2.1 Name: nonebot-plugin-talk-with-chatgpt Version: 0.6.0
 Summary: Nonebot2 åºäºaccessTokenç»å½çChatGPTèå¤©æä»¶ Home-page:
 https://github.com/nikissXI/nonebot_plugins/tree/main/
 nonebot_plugin_talk_with_chatgpt License: MIT Author: nikissXI Author-email:
 1299577815@qq.com Requires-Python: >=3.8 Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Dist: httpx (>=0.22.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.0.0) Requires-Dist: nonebot2
-(>=2.0.0rc1) Requires-Dist: ujson (>=5.0.0) Project-URL: Documentation, https:/
-/github.com/nikissXI/nonebot_plugins/tree/main/
+Programming Language :: Python :: 3.11 Requires-Dist: Pillow (>=9.0.0)
+Requires-Dist: httpx (>=0.22.0) Requires-Dist: nonebot-adapter-onebot (>=2.0.0)
+Requires-Dist: nonebot2 (>=2.0.0rc1) Requires-Dist: ujson (>=5.0.0) Project-
+URL: Documentation, https://github.com/nikissXI/nonebot_plugins/tree/main/
 nonebot_plugin_talk_with_chatgpt#README.md Project-URL: Repository, https://
 github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt
 Description-Content-Type: text/markdown
                               [NoneBotPluginLogo]
                # nonebot_plugin_talk_with_chatgpt _â¨ Nonebot2
                     ä¸ä¸ªç®åæç¨çchatgptæä»¶ â¨_
                          [license] [nonebot2] [python]
@@ -42,45 +42,53 @@
 ai.fakeopen.com/api/conversation #
 é»è®¤æ ä»£çï¼è§apiæåµçæ¯å¦éè¦æ¢¯å­ãè¿ä¸ªåç½®çåä»£ææµè¿æ¯ä¸éè¦æ¢¯å­çã
 talk_with_chatgpt_http_proxy = null # å¤çæ¶æ¯æ¶æ¯å¦æç¤º
 talk_with_chatgpt_reply_notice = true # ç¾¤èæ¯å¦å±äº«ä¼è¯
 talk_with_chatgpt_group_share = false # åªåè®¸è¶çº§ç®¡çåä¿®æ¹é¢è®¾
 talk_with_chatgpt_prompt_admin_only = true #
 æ¯å¦é»è®¤åè®¸ææç¾¤èä½¿ç¨ï¼å¦åéè¦ä½¿ç¨å½ä»¤å¯ç¨
-talk_with_chatgpt_all_group_enable = true ``` ####
-å¦æè¦ä¿®æ¹è§¦åå½ä»¤å°±å¡« ```bash # ç¾¤èè¾ç¹æ¯å¦ååº
-talk_with_chatgpt_talk_at = true #
+talk_with_chatgpt_all_group_enable = true #
+æºå¨äººçåå¤æ¯å¦ä½¿ç¨å¾çåé talk_with_chatgpt_send_with_img =
+false ``` #### å¦æè¦ä¿®æ¹è§¦åå½ä»¤å°±å¡« ```bash #
+ç¾¤èè¾ç¹æ¯å¦ååº talk_with_chatgpt_talk_at = true #
 è§¦åå¯¹è¯çå½ä»¤åç¼ï¼é»è®¤ç¾¤èç´æ¥è¾ç¹ä¹å¯ä»¥è§¦å
 talk_with_chatgpt_talk_cmd = /talk # ç§èæ²æµ¸å¼å¯¹è¯è§¦åå½ä»¤
 talk_with_chatgpt_talk_p_cmd = /hi #
 éç½®å¯¹è¯çå½ä»¤ï¼å°±æ¯æ¸ç©ºèå¤©è®°å½ talk_with_chatgpt_reset_cmd =
 /reset # è®¾ç½®é¢è®¾çå½ä»¤åç¼ talk_with_chatgpt_prompt_cmd = /prompt #
 å¦æå³é­ææç¾¤èä½¿ç¨ï¼å¯ç¨è¯¥ç¾¤çå½ä»¤
 talk_with_chatgpt_group_enable_cmd = /chatgpt ``` ####
 å¤§æ¦çç¨ä¸ä¸çéå¡«é¡¹ ```bash #
+ææè¯å±è½ï¼é»è®¤ä¸å±è½ä»»ä½è¯ talk_with_chatgpt_ban_word =
+["ç¤ºä¾è¯1", "ç¤ºä¾è¯2"] #
 è¯·æ±è¶æ¶æ¶é´ï¼åç­çæçæ¶é´ä¹è¦ç®å¨è¿éé¢çï¼æä»¥ä¸è½å¤ªç­ï¼é»è®¤60ç§
 talk_with_chatgpt_timeout = 60 # chatgptæ¨¡åï¼é»è®¤ text-davinci-002-
 render-shaï¼æ´å¤æ¨¡åè¯·åè https://platform.openai.com/docs/models
 talk_with_chatgpt_api_model = text-davinci-002-render-sha #
 æºå¨äººçQQå·åè¡¨ï¼éå¡« #
 å¦ææå¤ä¸ªbotè¿æ¥ï¼ä¼æç§å¡«åçlistï¼å·¦è¾¹çæºå¨äººQQä¼åçº§æé«
 1234 > 5678 > 6666ï¼ä¼èªå¨åæ¢ #
 å¦æä¸å¡«è¯¥éç½®åç±ç¬¬ä¸ä¸ªè¿ä¸çbotååºï¼æä»¥åbotè¿å¯ä»¥ä¸å¡«ï¼å
 ["all"]åæææºå¨äººåååº talk_with_chatgpt_bot_qqnum_list = [1234,
 5678, 6666] # æä»¶æ°æ®æä»¶åï¼é»è®¤./data/talk_with_chatgpt.json
-talk_with_chatgpt_data = talk_with_chatgpt.json ``` ##
+talk_with_chatgpt_data = talk_with_chatgpt.json #
+å¦æä½¿ç¨å¾çåå¤ï¼å­ä½å¤§å° talk_with_chatgpt_font_size = 18 ``` ##
 æä»¶å½ä»¤ï¼åå¯ä¿®æ¹ï¼ï¼ | æä»¤ | è¯´æ | |:-----:|:----:| | /talk
 | å¼å§å¯¹è¯ï¼é»è®¤ç¾¤é@æºå¨äººä¹å¯ä»¥ | | /hi |
 æ²æµ¸å¼å¯¹è¯ï¼ä»éç§èï¼ | | /reset |
 éç½®å¯¹è¯ï¼ä¸ä¼éç½®é¢è®¾ï¼ | | /prompt |
+è®¾ç½®é¢è®¾ï¼äººæ ¼ï¼ï¼è®¾ç½®åä¼éç½®å¯¹è¯ | | /chatgpt |
 è®¾ç½®é¢è®¾ï¼äººæ ¼ï¼ï¼è®¾ç½®åä¼éç½®å¯¹è¯ | ## æ´æ°æ¥å¿ ### 2023/
-5/30 \[v0.5.0] *
-æ´æ¢äºèªå¸¦é¢è®¾âç«å¨âçåå®¹ï¼æ°å¢éç½®é¡¹talk_with_chatgpt_all_group_enableåtalk_with_chatgpt_group_enable_cmdï¼æ°å¢å½ä»¤/
-chatgpt ### 2023/5/29 \[v0.4.3] * [æ¯ææææºå¨äººååºå½ä»¤](https://
-github.com/nikissXI/nonebot_plugins/issues/22) ### 2023/5/18 \[v0.4.2] *
+6/6 \[v0.6.0] * æ°å¢éç½®é¡¹ talk_with_chatgpt_send_with_img å
+talk_with_chatgpt_ban_word ### 2023/5/30 \[v0.5.0] *
+æ´æ¢äºèªå¸¦é¢è®¾âç«å¨âçåå®¹ï¼æ°å¢éç½®é¡¹
+talk_with_chatgpt_all_group_enable å talk_with_chatgpt_group_enable_cmd
+ï¼æ°å¢å½ä»¤/chatgpt ### 2023/5/29 \[v0.4.3] *
+[æ¯ææææºå¨äººååºå½ä»¤](https://github.com/nikissXI/
+nonebot_plugins/issues/22) ### 2023/5/18 \[v0.4.2] *
 [ä¿®å¤ä¼è¯ä¸¢å¤±ä¸éç½®çé®é¢](https://github.com/nikissXI/
 nonebot_plugins/issues/21) ### 2023/4/22 \[v0.4.1] *
 [å¢å ç¾¤èatè§¦åå¼å³](https://github.com/nikissXI/nonebot_plugins/
 issues/21) ### 2023/4/21 \[v0.4.0] *
 æ´æ¢äºé»è®¤APIï¼ææ¶è½ç¨ï¼å»ºè®®è¿æ¯èªå·±æ­å»ºAPI *
 æ°å¢å¤é¢è®¾åè½ï¼åç½®ä¸ä¸ªé¢è®¾ï¼ç«å¨ãé­é­ãå¼åèæ¨¡å¼
 * å¢å ç§èæ²æµ¸å¼å¯¹è¯ * ä¼åå¤§éç»è ### 2023/4/11 \[v0.2.3] *
```

