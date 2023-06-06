# Comparing `tmp/hikari_core-0.1.5.tar.gz` & `tmp/hikari_core-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikari_core-0.1.5.tar", max compression
+gzip compressed data, was "hikari_core-0.1.6.tar", max compression
```

## Comparing `hikari_core-0.1.5.tar` & `hikari_core-0.1.6.tar`

### file list

```diff
@@ -1,51 +1,42 @@
--rw-r--r--   0        0        0     3552 2023-05-15 10:55:59.938416 hikari_core-0.1.5/hikari_core/__init__.py
--rw-r--r--   0        0        0     4191 2023-05-14 15:19:46.160052 hikari_core-0.1.5/hikari_core/analyze.py
--rw-r--r--   0        0        0     3343 2023-05-14 15:19:46.161065 hikari_core-0.1.5/hikari_core/command_select.py
--rw-r--r--   0        0        0     1468 2023-05-14 15:19:46.161065 hikari_core-0.1.5/hikari_core/config.py
--rw-r--r--   0        0        0    10720 2023-05-14 15:19:46.162085 hikari_core-0.1.5/hikari_core/data_source.py
--rw-r--r--   0        0        0      743 2023-05-14 15:19:45.721315 hikari_core-0.1.5/hikari_core/Html_Render/__init__.py
--rw-r--r--   0        0        0      967 2023-05-13 14:57:53.183565 hikari_core-0.1.5/hikari_core/Html_Render/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2872 2023-05-13 14:57:53.187591 hikari_core-0.1.5/hikari_core/Html_Render/__pycache__/browser.cpython-310.pyc
--rw-r--r--   0        0        0     5164 2023-05-13 08:04:19.776227 hikari_core-0.1.5/hikari_core/Html_Render/__pycache__/data_source.cpython-310.pyc
--rw-r--r--   0        0        0     2942 2023-05-14 15:19:45.722347 hikari_core-0.1.5/hikari_core/Html_Render/browser.py
--rw-r--r--   0        0        0     5462 2023-05-14 15:19:45.723349 hikari_core-0.1.5/hikari_core/Html_Render/data_source.py
--rw-r--r--   0        0        0    18237 2023-05-14 15:19:45.725399 hikari_core-0.1.5/hikari_core/Html_Render/templates/github-markdown-light.css
--rw-r--r--   0        0        0  1458204 2023-05-14 15:19:45.876541 hikari_core-0.1.5/hikari_core/Html_Render/templates/katex/katex.min.b64_fonts.css
--rw-r--r--   0        0        0   270288 2023-05-14 15:19:45.910815 hikari_core-0.1.5/hikari_core/Html_Render/templates/katex/katex.min.js
--rw-r--r--   0        0        0     1290 2023-05-14 15:19:45.912835 hikari_core-0.1.5/hikari_core/Html_Render/templates/katex/mathtex-script-type.min.js
--rw-r--r--   0        0        0      662 2023-05-14 15:19:45.915374 hikari_core-0.1.5/hikari_core/Html_Render/templates/markdown.html
--rw-r--r--   0        0        0     4963 2023-05-14 15:19:45.917452 hikari_core-0.1.5/hikari_core/Html_Render/templates/pygments-default.css
--rw-r--r--   0        0        0      125 2023-05-14 15:19:45.917452 hikari_core-0.1.5/hikari_core/Html_Render/templates/text.css
--rw-r--r--   0        0        0      233 2023-05-14 15:19:45.918475 hikari_core-0.1.5/hikari_core/Html_Render/templates/text.html
--rw-r--r--   0        0        0     1873 2023-05-14 15:19:45.918475 hikari_core-0.1.5/hikari_core/HttpClient_Pool.py
--rw-r--r--   0        0        0     2601 2023-05-14 15:19:46.163103 hikari_core-0.1.5/hikari_core/model.py
--rw-r--r--   0        0        0        0 2023-05-14 15:19:46.163103 hikari_core-0.1.5/hikari_core/moudle/__init__.py
--rw-r--r--   0        0        0      175 2023-05-12 06:05:32.348596 hikari_core-0.1.5/hikari_core/moudle/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5400 2023-05-12 06:07:09.234200 hikari_core-0.1.5/hikari_core/moudle/__pycache__/publicAPI.cpython-310.pyc
--rw-r--r--   0        0        0     2914 2023-05-12 06:06:54.456117 hikari_core-0.1.5/hikari_core/moudle/__pycache__/wws_info.cpython-310.pyc
--rw-r--r--   0        0        0     3105 2023-05-12 06:07:46.904239 hikari_core-0.1.5/hikari_core/moudle/__pycache__/wws_recent.cpython-310.pyc
--rw-r--r--   0        0        0     7259 2023-05-14 15:19:46.164098 hikari_core-0.1.5/hikari_core/moudle/publicAPI.py
--rw-r--r--   0        0        0     2579 2023-05-14 15:19:46.164098 hikari_core-0.1.5/hikari_core/moudle/wws_info.py
--rw-r--r--   0        0        0     4556 2023-05-14 15:19:46.165108 hikari_core-0.1.5/hikari_core/moudle/wws_recent.py
--rw-r--r--   0        0        0   173084 2023-05-14 15:19:45.922537 hikari_core-0.1.5/hikari_core/Template/Chart.min.js
--rw-r--r--   0        0        0    13286 2023-05-14 15:19:45.924550 hikari_core-0.1.5/hikari_core/Template/chartjs-plugin-datalabels@1.0.0.js
--rw-r--r--   0        0        0  3313391 2023-05-12 03:16:55.346040 hikari_core-0.1.5/hikari_core/Template/echarts.js
--rw-r--r--   0        0        0     3710 2023-05-14 15:19:46.136839 hikari_core-0.1.5/hikari_core/Template/select-ship.html
--rw-r--r--   0        0        0     5118 2023-05-14 15:19:46.138837 hikari_core-0.1.5/hikari_core/Template/ship-rank.html
--rw-r--r--   0        0        0      225 2023-05-14 15:19:46.138837 hikari_core-0.1.5/hikari_core/Template/text-help.css
--rw-r--r--   0        0        0     7293 2023-05-14 15:19:46.140860 hikari_core-0.1.5/hikari_core/Template/wws-ban.html
--rw-r--r--   0        0        0    16766 2023-05-14 15:19:46.143404 hikari_core-0.1.5/hikari_core/Template/wws-box-christmas.html
--rw-r--r--   0        0        0    18454 2023-05-14 15:19:46.145419 hikari_core-0.1.5/hikari_core/Template/wws-clan.html
--rw-r--r--   0        0        0    23636 2023-05-14 15:19:46.146446 hikari_core-0.1.5/hikari_core/Template/wws-info-recent.html
--rw-r--r--   0        0        0    25512 2023-05-14 15:19:46.148454 hikari_core-0.1.5/hikari_core/Template/wws-info.html
--rw-r--r--   0        0        0     2396 2023-05-14 15:19:46.149453 hikari_core-0.1.5/hikari_core/Template/wws-personalRecord.html
--rw-r--r--   0        0        0    21667 2023-05-14 15:19:46.151465 hikari_core-0.1.5/hikari_core/Template/wws-ship-recent.html
--rw-r--r--   0        0        0    20760 2023-05-14 15:19:46.155491 hikari_core-0.1.5/hikari_core/Template/wws-ship.html
--rw-r--r--   0        0        0     9455 2023-05-14 15:19:46.157030 hikari_core-0.1.5/hikari_core/Template/wws-sx.html
--rw-r--r--   0        0        0     5793 2023-05-14 15:19:46.159058 hikari_core-0.1.5/hikari_core/Template/wws-unban.html
--rw-r--r--   0        0        0     3429 2023-05-15 06:53:14.151685 hikari_core-0.1.5/hikari_core/utils.py
--rw-r--r--   0        0        0    35823 2023-05-12 02:05:38.427107 hikari_core-0.1.5/LICENSE
--rw-r--r--   0        0        0      521 2023-05-15 10:56:28.455364 hikari_core-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       35 2023-05-12 02:05:38.429109 hikari_core-0.1.5/README.md
--rw-r--r--   0        0        0      948 1970-01-01 00:00:00.000000 hikari_core-0.1.5/setup.py
--rw-r--r--   0        0        0      781 1970-01-01 00:00:00.000000 hikari_core-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     4536 2023-05-22 02:25:09.664141 hikari_core-0.1.6/hikari_core/__init__.py
+-rw-r--r--   0        0        0     6087 2023-06-06 15:48:21.901621 hikari_core-0.1.6/hikari_core/analyze.py
+-rw-r--r--   0        0        0     3364 2023-05-17 07:49:16.245089 hikari_core-0.1.6/hikari_core/command_select.py
+-rw-r--r--   0        0        0     1468 2023-05-14 15:19:46.161065 hikari_core-0.1.6/hikari_core/config.py
+-rw-r--r--   0        0        0    10743 2023-06-06 17:17:33.374770 hikari_core-0.1.6/hikari_core/data_source.py
+-rw-r--r--   0        0        0      743 2023-05-14 15:19:45.721315 hikari_core-0.1.6/hikari_core/Html_Render/__init__.py
+-rw-r--r--   0        0        0     2942 2023-05-14 15:19:45.722347 hikari_core-0.1.6/hikari_core/Html_Render/browser.py
+-rw-r--r--   0        0        0     5462 2023-05-14 15:19:45.723349 hikari_core-0.1.6/hikari_core/Html_Render/data_source.py
+-rw-r--r--   0        0        0    18237 2023-05-14 15:19:45.725399 hikari_core-0.1.6/hikari_core/Html_Render/templates/github-markdown-light.css
+-rw-r--r--   0        0        0      662 2023-05-14 15:19:45.915374 hikari_core-0.1.6/hikari_core/Html_Render/templates/markdown.html
+-rw-r--r--   0        0        0     4963 2023-05-14 15:19:45.917452 hikari_core-0.1.6/hikari_core/Html_Render/templates/pygments-default.css
+-rw-r--r--   0        0        0      125 2023-05-14 15:19:45.917452 hikari_core-0.1.6/hikari_core/Html_Render/templates/text.css
+-rw-r--r--   0        0        0      233 2023-05-14 15:19:45.918475 hikari_core-0.1.6/hikari_core/Html_Render/templates/text.html
+-rw-r--r--   0        0        0     1968 2023-05-30 20:07:21.287212 hikari_core-0.1.6/hikari_core/HttpClient_Pool.py
+-rw-r--r--   0        0        0     3138 2023-06-06 15:31:07.314957 hikari_core-0.1.6/hikari_core/model.py
+-rw-r--r--   0        0        0        0 2023-05-14 15:19:46.163103 hikari_core-0.1.6/hikari_core/moudle/__init__.py
+-rw-r--r--   0        0        0    10479 2023-05-16 16:11:32.118354 hikari_core-0.1.6/hikari_core/moudle/publicAPI.py
+-rw-r--r--   0        0        0     2392 2023-05-30 20:07:21.289754 hikari_core-0.1.6/hikari_core/moudle/wws_info.py
+-rw-r--r--   0        0        0     3190 2023-06-06 16:41:39.549334 hikari_core-0.1.6/hikari_core/moudle/wws_recent.py
+-rw-r--r--   0        0        0     3874 2023-05-30 20:07:21.290780 hikari_core-0.1.6/hikari_core/moudle/wws_ship_info.py
+-rw-r--r--   0        0        0     3792 2023-05-17 07:49:16.247099 hikari_core-0.1.6/hikari_core/moudle/wws_ship_recent.py
+-rw-r--r--   0        0        0   173084 2023-05-15 12:36:37.138233 hikari_core-0.1.6/hikari_core/Template/Chart.min.js
+-rw-r--r--   0        0        0    13286 2023-05-15 12:36:39.500206 hikari_core-0.1.6/hikari_core/Template/chartjs-plugin-datalabels@1.0.0.js
+-rw-r--r--   0        0        0     3780 2023-05-16 16:11:32.110791 hikari_core-0.1.6/hikari_core/Template/select-ship.html
+-rw-r--r--   0        0        0     5135 2023-06-02 14:21:25.824545 hikari_core-0.1.6/hikari_core/Template/ship-rank.html
+-rw-r--r--   0        0        0      225 2023-05-15 12:30:50.607350 hikari_core-0.1.6/hikari_core/Template/text-help.css
+-rw-r--r--   0        0        0     7310 2023-06-02 14:21:25.824545 hikari_core-0.1.6/hikari_core/Template/wws-ban.html
+-rw-r--r--   0        0        0    16783 2023-06-02 14:21:25.824545 hikari_core-0.1.6/hikari_core/Template/wws-box-christmas.html
+-rw-r--r--   0        0        0    18454 2023-05-15 12:30:50.643703 hikari_core-0.1.6/hikari_core/Template/wws-clan.html
+-rw-r--r--   0        0        0    25696 2023-06-06 17:10:27.683820 hikari_core-0.1.6/hikari_core/Template/wws-info-recent.html
+-rw-r--r--   0        0        0    24942 2023-06-02 14:21:25.824545 hikari_core-0.1.6/hikari_core/Template/wws-info.html
+-rw-r--r--   0        0        0     2396 2023-05-15 12:30:50.750146 hikari_core-0.1.6/hikari_core/Template/wws-personalRecord.html
+-rw-r--r--   0        0        0    21684 2023-06-02 14:21:25.824545 hikari_core-0.1.6/hikari_core/Template/wws-ship-recent.html
+-rw-r--r--   0        0        0    20793 2023-06-02 14:21:25.824545 hikari_core-0.1.6/hikari_core/Template/wws-ship.html
+-rw-r--r--   0        0        0     9472 2023-06-02 14:21:25.824545 hikari_core-0.1.6/hikari_core/Template/wws-sx.html
+-rw-r--r--   0        0        0     5810 2023-06-02 14:21:25.824545 hikari_core-0.1.6/hikari_core/Template/wws-unban.html
+-rw-r--r--   0        0        0     4393 2023-05-16 11:20:41.711193 hikari_core-0.1.6/hikari_core/utils.py
+-rw-r--r--   0        0        0    35823 2023-05-12 02:05:38.427107 hikari_core-0.1.6/LICENSE
+-rw-r--r--   0        0        0      549 2023-06-06 17:17:25.235690 hikari_core-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-05-12 02:05:38.429109 hikari_core-0.1.6/README.md
+-rw-r--r--   0        0        0    11430 1970-01-01 00:00:00.000000 hikari_core-0.1.6/setup.py
+-rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 hikari_core-0.1.6/PKG-INFO
```

### Comparing `hikari_core-0.1.5/hikari_core/command_select.py` & `hikari_core-0.1.6/hikari_core/command_select.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+# fmt: off
 from dataclasses import dataclass
 from typing import List, Protocol, Tuple, runtime_checkable
 
 # from .game.ban_search import get_BanInfo
 # from .game.box_check import check_christmas_box
 # from .game.ocr import get_Random_Ocr_Pic
 # from .game.roll import roll_ship
 # from .game.sx import get_sx_info
 # from .moudle.publicAPI import get_ship_name
 # from .moudle.wws_bind import (change_BindInfo, delete_BindInfo, get_BindInfo,
 #                              set_BindInfo, set_special_BindInfo)
 # from .moudle.wws_clan import get_ClanInfo
 from .moudle.wws_info import get_AccountInfo
 from .moudle.wws_recent import get_RecentInfo
-
 # from .moudle.wws_record import get_record
-# from .moudle.wws_ship import get_ShipInfo, get_ShipInfoRecent
+from .moudle.wws_ship_info import get_ShipInfo
+from .moudle.wws_ship_recent import get_ShipRecent
+
 # from .moudle.wws_shiprank import get_ShipRank
+# fmt: on
 
 
 @runtime_checkable
 class Func(Protocol):
     async def __call__(self, **kwargs):
         ...
 
@@ -35,28 +38,28 @@
     # command(("切换绑定", "更换绑定", "更改绑定"), change_BindInfo),
     # command(("查询绑定", "绑定查询", "绑定列表", "查绑定"), get_BindInfo),
     # command(("删除绑定",), delete_BindInfo),
     # command(("特殊绑定",), set_special_BindInfo),
     # command(("ship.rank", "rank"), get_ShipRank),
     # command(("bind", "绑定", "set"), set_BindInfo),
     command(("recent", "近期"), None, get_RecentInfo),
-    # command(("ship","单船",),None,get_ShipInfo,),
+    command(("ship", "单船"), None, get_ShipInfo),
     # command(("record", "历史记录"), None, get_record),
     # command(("clan", "军团", "公会", "工会"), None, get_ClanInfo),
     # command(("随机表情包",), get_Random_Ocr_Pic),
     # command(("roll", "随机"), roll_ship),
     # command(("sx", "扫雪"), get_sx_info),
     # command(("ban","封号记录"),get_BanInfo),
     # command(("box", "sd", "圣诞船池"), check_christmas_box),
     # command(("搜船名", "查船名", "船名"), get_ship_name),
 ]
 
 second_command_list = [
-    # command(("recent","近期",),get_ShipInfoRecent,),
-    # command(("ship","单船",),get_ShipInfoRecent,),
+    command(("recent", "近期"), get_ShipRecent),
+    command(("ship", "单船"), get_ShipRecent),
     # command(("clan", "军团", "公会", "工会"), get_record),
     # command(("record", "历史记录"), get_record),
 ]
 
 
 async def findFunction_and_replaceKeywords(match_list, command_List, default_func) -> Tuple[command, List]:
     for com in command_List:
@@ -69,11 +72,9 @@
                     return com, match_list
     return command(None, default_func, None), match_list
 
 
 async def select_command(search_list) -> Tuple[Func, List]:
     command, search_list = await findFunction_and_replaceKeywords(search_list, first_command_list, get_AccountInfo)
     if command.func is None:
-        command, search_list = await findFunction_and_replaceKeywords(
-            search_list, second_command_list, command.default_func
-        )
+        command, search_list = await findFunction_and_replaceKeywords(search_list, second_command_list, command.default_func)
     return command.func, search_list
```

### Comparing `hikari_core-0.1.5/hikari_core/config.py` & `hikari_core-0.1.6/hikari_core/config.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.5/hikari_core/data_source.py` & `hikari_core-0.1.6/hikari_core/data_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Tuple
 
 from pydantic import BaseModel
 
 dir_path = Path(__file__).parent
 template_path = dir_path / "Template"
 yuyuko_url = "https://api.wows.shinoaki.com"
+__version__ = "0.1.6"
 
 
 @dataclass
 class matching:
     keywords: Tuple[str, ...]
     match_keywords: str
```

### Comparing `hikari_core-0.1.5/hikari_core/Html_Render/__init__.py` & `hikari_core-0.1.6/hikari_core/Html_Render/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.5/hikari_core/Html_Render/browser.py` & `hikari_core-0.1.6/hikari_core/Html_Render/browser.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.5/hikari_core/Html_Render/data_source.py` & `hikari_core-0.1.6/hikari_core/Html_Render/data_source.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.5/hikari_core/Html_Render/templates/github-markdown-light.css` & `hikari_core-0.1.6/hikari_core/Html_Render/templates/github-markdown-light.css`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.5/hikari_core/Html_Render/templates/markdown.html` & `hikari_core-0.1.6/hikari_core/Html_Render/templates/markdown.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.5/hikari_core/Html_Render/templates/pygments-default.css` & `hikari_core-0.1.6/hikari_core/Html_Render/templates/pygments-default.css`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.5/hikari_core/HttpClient_Pool.py` & `hikari_core-0.1.6/hikari_core/HttpClient_Pool.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Optional
 
 import httpx
 from httpx import AsyncClient, Request, Response
 from loguru import logger
 
 from .config import hikari_config
+from .data_source import __version__
 
 
 async def before_request(request: Request):
     logger.info(f"{request.method} {request.url}")
 
 
 async def after_response(response: Response):
@@ -23,14 +24,15 @@
 async def create_client_yuyuko() -> AsyncClient:
     global _client_yuyuko
     _client_yuyuko = httpx.AsyncClient(
         headers={
             'Authorization': hikari_config.token,
             "accept": "application/json",
             "Content-Type": "application/json",
+            "Yuyuko-Client-Type": f"BOT;{__version__}",
         },
         event_hooks={
             "request": [
                 before_request,
             ],
             "response": [
                 after_response,
```

### Comparing `hikari_core-0.1.5/hikari_core/model.py` & `hikari_core-0.1.6/hikari_core/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import time
 from datetime import date
 from typing import List, Optional, Protocol, Union, runtime_checkable
 
 from pydantic import BaseModel, Field
 
 
 @runtime_checkable
@@ -16,29 +17,30 @@
 
 
 class Ship_Model(BaseModel):
     Ship_Nation: Optional[str]
     Ship_Tier: Optional[int]
     Ship_Type: Optional[str]
     Ship_Name: Optional[str]
+    ship_Name_Numbers: Optional[str]
     Ship_Id: Optional[int]
 
 
 class Input_Model(BaseModel):
     Command_Text: Optional[str] = ""  # 输入的指令,请提前去除wws
     Command_List: Optional[List]
     Search_Type: Optional[int] = 3  # 1:me  2:@  3:server+name or default
     Platform: Optional[str]
     PlatformId: Optional[str]
     Server: Optional[str]
     AccountName: Optional[str]
     AccountId: Optional[int]
     ClanName: Optional[str]
     Recent_Day: Optional[int] = 0
-    Recent_Date: Optional[date]
+    Recent_Date: Optional[str] = time.strftime("%Y-%m-%d", time.localtime())
     Select_Index: Optional[int]
     Select_Data: Optional[List]
     ShipInfo: Ship_Model = Ship_Model()
 
 
 class Output_Model(BaseModel):
     Yuyuko_Code: Optional[int]
@@ -76,10 +78,26 @@
         self.Output.Data = failed_data
         self.Output.Data_Type = str(type(failed_data))
         return self
 
     def wait(self, select_data: List):
         self.Status = "wait"
         self.Input.Select_Data = select_data
-        self.Output.Data = "等待选择"
+        self.Output.Data = select_data
         self.Output.Data_Type = str(type(self.Output.Data))
         return self
+
+    def set_template_info(self, template_name: str, width: int, height: int):
+        """配置模板解析参数
+
+        Args:
+            template_name (str): 模板名
+            width (int): 宽度
+            height (int): 高度
+
+        Returns:
+            Hikari_Model
+        """
+        self.Output.Template = template_name
+        self.Output.Width = width
+        self.Output.Height = height
+        return self
```

### Comparing `hikari_core-0.1.5/hikari_core/moudle/publicAPI.py` & `hikari_core-0.1.6/hikari_core/moudle/publicAPI.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,28 @@
+# fmt: off
 import asyncio
 import gzip
 import traceback
 from asyncio.exceptions import TimeoutError
 from base64 import b64encode
-from typing import List
+from typing import List, Tuple
 
 import orjson
+from bs4 import BeautifulSoup
 from httpx import ConnectTimeout
 from loguru import logger
 
-from ..data_source import levels, nations, shiptypes
-from ..HttpClient_Pool import get_client_wg, get_client_yuyuko
+from ..data_source import levels, nations, number_url_homes, shiptypes
+from ..HttpClient_Pool import (get_client_default, get_client_wg,
+                               get_client_yuyuko)
+from ..model import Ship_Model
 from ..utils import match_keywords
 
+# fmt: on
+
 
 async def get_nation_list():
     try:
         msg = ""
         url = "https://api.wows.shinoaki.com/public/wows/encyclopedia/nation/list"
         client_yuyuko = await get_client_yuyuko()
         resp = await client_yuyuko.get(url, timeout=None)
@@ -61,25 +67,34 @@
     except (TimeoutError, ConnectTimeout):
         logger.warning(traceback.format_exc())
     except Exception:
         logger.error(traceback.format_exc())
         return "wuwuwu出了点问题，请联系麻麻解决"
 
 
-async def get_ship_byName(shipname: str):
+async def get_ship_byName(shipname: str) -> List:
     try:
         url = "https://api.wows.shinoaki.com/public/wows/encyclopedia/ship/search"
         params = {"county": "", "level": "", "shipName": shipname, "shipType": ""}
         client_yuyuko = await get_client_yuyuko()
         resp = await client_yuyuko.get(url, params=params, timeout=None)
         result = orjson.loads(resp.content)
         List = []
         if result["code"] == 200 and result["data"]:
             for each in result["data"]:
-                List.append([each["id"], each["shipNameCn"], each["shipNameNumbers"], each["tier"], each["shipType"]])
+                List.append(
+                    Ship_Model(
+                        Ship_Nation=each["country"],
+                        Ship_Tier=each["tier"],
+                        Ship_Type=each["shipType"],
+                        Ship_Name=each["shipNameCn"],
+                        ship_Name_Numbers=each["shipNameNumbers"],
+                        Ship_Id=each["id"],
+                    )
+                )
             return List
         else:
             return None
     except (TimeoutError, ConnectTimeout):
         logger.warning(traceback.format_exc())
     except Exception:
         logger.error(traceback.format_exc())
@@ -179,7 +194,76 @@
         wg_result = orjson.loads(resp.content)
         if resp.status_code == 200 and wg_result["status"] == "ok":
             params[key] = resp.text
     except Exception:
         logger.error(traceback.format_exc())
         logger.error(f"上报url：{url}")
         return
+
+
+async def get_MyShipRank_yuyuko(params) -> int:
+    try:
+        url = "https://api.wows.shinoaki.com/upload/numbers/data/upload/user/ship/rank"
+        client_yuyuko = await get_client_yuyuko()
+        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        result = orjson.loads(resp.content)
+        if result["code"] == 200 and result["data"]:
+            if result["data"]["ranking"]:
+                return result["data"]["ranking"]
+            elif not result["data"]["ranking"] and not result["data"]["serverId"] == "cn":
+                ranking = await get_MyShipRank_Numbers(result["data"]["httpUrl"], result["data"]["serverId"])
+                if ranking:
+                    await post_MyShipRank_yuyuko(
+                        result["data"]["accountId"],
+                        ranking,
+                        result["data"]["serverId"],
+                        result["data"]["shipId"],
+                    )
+                return ranking
+            else:
+                return None
+        else:
+            return None
+    except Exception:
+        logger.error(traceback.format_exc())
+        return None
+
+
+async def get_MyShipRank_Numbers(url, server) -> int:
+    try:
+        data = None
+        client_default = await get_client_default()
+        client_default = await get_client_default()
+        resp = await client_default.get(url, timeout=10)
+        if resp.content:
+            result = orjson.loads(resp.content)
+            page_url = str(result["url"]).replace("\\", "")
+            nickname = str(result["nickname"])
+            my_rank_url = f"{number_url_homes[server]}{page_url}"
+            resp = await client_default.get(my_rank_url, timeout=10)
+            soup = BeautifulSoup(resp.content, "html.parser")
+            data = soup.select_one(f'tr[data-nickname="{nickname}"]').select_one("td").string
+        if data and data.isdigit():
+            return data
+        else:
+            return None
+    except Exception:
+        logger.error(traceback.format_exc())
+        return None
+
+
+async def post_MyShipRank_yuyuko(accountId, ranking, serverId, shipId):
+    try:
+        url = "https://api.wows.shinoaki.com/upload/numbers/data/upload/user/ship/rank"
+        post_data = {
+            "accountId": int(accountId),
+            "ranking": int(ranking),
+            "serverId": serverId,
+            "shipId": int(shipId),
+        }
+        client_yuyuko = await get_client_yuyuko()
+        resp = await client_yuyuko.post(url, json=post_data, timeout=None)
+        result = orjson.loads(resp.content)
+        return
+    except Exception:
+        logger.error(traceback.format_exc())
+        return
```

### Comparing `hikari_core-0.1.5/hikari_core/moudle/wws_info.py` & `hikari_core-0.1.6/hikari_core/moudle/wws_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,28 +20,25 @@
         else:
             return hikari.error("当前请求状态错误")
         is_cache = await check_yuyuko_cache(hikari.Input.Server, hikari.Input.AccountId)
         if is_cache:
             logger.success("上报数据成功")
         else:
             logger.success("跳过上报数据，直接请求")
-        url = "https://api.wows.shinoaki.com/public/wows/account/user/info"
+        url = "https://v3-api.wows.shinoaki.com/public/wows/account/user/info"
         if hikari.Input.Search_Type == 3:
             params = {"server": hikari.Input.Server, "accountId": hikari.Input.AccountId}
         else:
             params = {"server": hikari.Input.Platform, "accountId": hikari.Input.PlatformId}
         client_yuyuko = await get_client_yuyuko()
         resp = await client_yuyuko.get(url, params=params, timeout=None)
         result = orjson.loads(resp.content)
-        logger.success(f"本次请求总耗时{resp.elapsed.total_seconds()*1000}，服务器计算耗时:{result['queryTime']}")
         hikari.Output.Yuyuko_Code = result["code"]
         if result["code"] == 200 and result["data"]:
-            hikari.Output.Template = "wws-info.html"
-            hikari.Output.Width = 920
-            hikari.Output.Height = 1000
+            hikari = hikari.set_template_info("wws-info.html", 920, 1000)
             return hikari.success(result["data"])
         elif result["code"] == 403:
             return hikari.failed(f"{result['message']}\n请先绑定账号")
         elif result["code"] == 500:
             return hikari.failed(f"{result['message']}\n这是服务器问题，请联系雨季麻麻")
         else:
             return hikari.failed(f"{result['message']}")
```

### Comparing `hikari_core-0.1.5/hikari_core/Template/Chart.min.js` & `hikari_core-0.1.6/hikari_core/Template/Chart.min.js`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.5/hikari_core/Template/chartjs-plugin-datalabels@1.0.0.js` & `hikari_core-0.1.6/hikari_core/Template/chartjs-plugin-datalabels@1.0.0.js`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.5/hikari_core/Template/select-ship.html` & `hikari_core-0.1.6/hikari_core/Template/select-ship.html`

 * *Files 4% similar despite different names*

```diff
@@ -81,29 +81,29 @@
 				</div>
 			</div>
 			<div class="ship-list">
 				{% for ship in data %}
 				<div class="ship-item">
 					<div class="index"></div>
 					<div class="ship-inf">
-						<div class="ship-level">{{ ship[3] }}</div>
+						<div class="ship-level">{{ ship['Ship_Tier'] }}</div>
 						<div class="icon">
-							{% if ship[4] == 'Destroyer' %}
+							{% if ship['Ship_Type'] == 'Destroyer' %}
 							<img src="https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_destroyer.png">
-							{% elif ship[4] == 'Cruiser' %}
+							{% elif ship['Ship_Type'] == 'Cruiser' %}
 							<img src="https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_cruiser.png">
-							{% elif ship[4] == 'Battleship' %}
+							{% elif ship['Ship_Type'] == 'Battleship' %}
 							<img src="https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_battleship.png">
-							{% elif ship[4] == 'AirCarrier' %}
+							{% elif ship['Ship_Type'] == 'AirCarrier' %}
 							<img src="https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_aircarrier.png">
-							{% elif ship[4] == 'Submarine' %}
+							{% elif ship['Ship_Type'] == 'Submarine' %}
 							<img src="https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_submarine.png">
 							{% endif %}
 						</div>
-						<div class="ship-name">{{ ship[1] }}</div>
+						<div class="ship-name">{{ ship['Ship_Name'] }}</div>
 					</div>
 				</div>
 				{% endfor %}
 			</div>
 		</div>
 	</body>
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
 20s
 å­å¨å¤æ¡åå­ç¸ä¼¼çè¹
 è¯·å¨20ç§åéæ©å¯¹åºçåºå·
 {% for ship in data %}
-{{ ship[3] }}
-{% if ship[4] == 'Destroyer' %} [https://hikari-resource.oss-cn-
-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_destroyer.png] {% elif ship[4] ==
-'Cruiser' %} [https://hikari-resource.oss-cn-shanghai.aliyuncs.com/
-shipType_Icon/icon_sunk_cruiser.png] {% elif ship[4] == 'Battleship' %} [https:
-//hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/
-icon_sunk_battleship.png] {% elif ship[4] == 'AirCarrier' %} [https://hikari-
-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_aircarrier.png]
-{% elif ship[4] == 'Submarine' %} [https://hikari-resource.oss-cn-
+{{ ship['Ship_Tier'] }}
+{% if ship['Ship_Type'] == 'Destroyer' %} [https://hikari-resource.oss-cn-
+shanghai.aliyuncs.com/shipType_Icon/icon_sunk_destroyer.png] {% elif ship
+['Ship_Type'] == 'Cruiser' %} [https://hikari-resource.oss-cn-
+shanghai.aliyuncs.com/shipType_Icon/icon_sunk_cruiser.png] {% elif ship
+['Ship_Type'] == 'Battleship' %} [https://hikari-resource.oss-cn-
+shanghai.aliyuncs.com/shipType_Icon/icon_sunk_battleship.png] {% elif ship
+['Ship_Type'] == 'AirCarrier' %} [https://hikari-resource.oss-cn-
+shanghai.aliyuncs.com/shipType_Icon/icon_sunk_aircarrier.png] {% elif ship
+['Ship_Type'] == 'Submarine' %} [https://hikari-resource.oss-cn-
 shanghai.aliyuncs.com/shipType_Icon/icon_sunk_submarine.png] {% endif %}
-{{ ship[1] }}
+{{ ship['Ship_Name'] }}
 {% endfor %}
```

### Comparing `hikari_core-0.1.5/hikari_core/Template/ship-rank.html` & `hikari_core-0.1.6/hikari_core/Template/ship-rank.html`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 				{% endfor %}
 				
 				<div class="footer">
 					<p>©西行寺雨季&nbsp;&nbsp;©本心</p>
 					<p>https://github.com/benx1n/HikariBot</p>
 					<p>QQ频道搜索”yuyuko”即可使用稳定的腾讯官方机器人~</p>
 					<p>Design By 冷眠 H5 Converted By C1ystal</p>
-					<p>赞助鸣谢：男人们的定远号、Wishing、科长</p>
+					<p>赞助鸣谢：科长、男人们的定远号、海上最速暴毙传说</p>
 				</div>
 
 				<div style="margin: 0 50px; border-bottom: #008272 solid 5px; margin-bottom:20px;"></div>
 			</div>
 		</div>
 	</body>
```

#### html2text {}

```diff
@@ -35,8 +35,8 @@
 {{ rank['planesDestroyed'] }}
 {{ rank['maxPlanesDestroyed'] }}
 {% endfor %}
 Â©è¥¿è¡å¯ºé¨å­£  Â©æ¬å¿
 https://github.com/benx1n/HikariBot
 QQé¢éæç´¢âyuyukoâå³å¯ä½¿ç¨ç¨³å®çè¾è®¯å®æ¹æºå¨äºº~
 Design By å·ç  H5 Converted By C1ystal
-èµå©é¸£è°¢ï¼ç·äººä»¬çå®è¿å·ãWishingãç§é¿
+èµå©é¸£è°¢ï¼ç§é¿ãç·äººä»¬çå®è¿å·ãæµ·ä¸æéæ´æ¯ä¼ è¯´
```

### Comparing `hikari_core-0.1.5/hikari_core/Template/wws-ban.html` & `hikari_core-0.1.6/hikari_core/Template/wws-ban.html`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
 				{% endif %}
 			</div>
 			<div class="footer">
 				<p>©西行寺雨季&nbsp;&nbsp;©本心</p>
 				<p>https://github.com/benx1n/HikariBot</p>
 				<p>QQ频道搜索”yuyuko”即可使用稳定的腾讯官方机器人~</p>
 				<p>Design By 冷眠 H5 Converted By C1ystal</p>
-				<p>赞助鸣谢：男人们的定远号、Wishing、科长</p>
+				<p>赞助鸣谢：科长、男人们的定远号、海上最速暴毙传说</p>
 			</div>
 		</div>
 	</body>
 	
 	<script>
 		// 服务器字体颜色自动填充
 		let server_name = document.querySelector(".server").innerText;
```

#### html2text {}

```diff
@@ -24,8 +24,8 @@
 {% endfor %} {% else %}
 æªå¨å®æ¹å°ç¦åå²ä¸­å¹éå°è¯¥ç¨æ·
 {% endif %}
 Â©è¥¿è¡å¯ºé¨å­£  Â©æ¬å¿
 https://github.com/benx1n/HikariBot
 QQé¢éæç´¢âyuyukoâå³å¯ä½¿ç¨ç¨³å®çè¾è®¯å®æ¹æºå¨äºº~
 Design By å·ç  H5 Converted By C1ystal
-èµå©é¸£è°¢ï¼ç·äººä»¬çå®è¿å·ãWishingãç§é¿
+èµå©é¸£è°¢ï¼ç§é¿ãç·äººä»¬çå®è¿å·ãæµ·ä¸æéæ´æ¯ä¼ è¯´
```

### Comparing `hikari_core-0.1.5/hikari_core/Template/wws-box-christmas.html` & `hikari_core-0.1.6/hikari_core/Template/wws-box-christmas.html`

 * *Files 1% similar despite different names*

```diff
@@ -295,15 +295,15 @@
 									<span class="pr-number"><span class="pr-text"></span></span>
 									<div class="pr-bar" style="background-color: #92D050;"></div>
 									<div class="footer">
 										<p>©西行寺雨季&nbsp;&nbsp;©本心</p>
 										<p>https://github.com/benx1n/HikariBot</p>
 										<p>QQ频道搜索”yuyuko”即可使用稳定的腾讯官方机器人~</p>
 										<p>Design By 冷眠 H5 Converted By C1ystal</p>
-										<p>赞助鸣谢：男人们的定远号、Wishing、科长</p>
+										<p>赞助鸣谢：科长、男人们的定远号、海上最速暴毙传说</p>
 									</div>
 								</div>
 							</div>
 						</div>
 					</div>
 				</div>
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 å£è¯ç®±ä¸­ {{ data['count']}}
 å·²æ¥æ {{ data['have']}}
 æ¶éè¿åº¦
 Â©è¥¿è¡å¯ºé¨å­£  Â©æ¬å¿
 https://github.com/benx1n/HikariBot
 QQé¢éæç´¢âyuyukoâå³å¯ä½¿ç¨ç¨³å®çè¾è®¯å®æ¹æºå¨äºº~
 Design By å·ç  H5 Converted By C1ystal
-èµå©é¸£è°¢ï¼ç·äººä»¬çå®è¿å·ãWishingãç§é¿
+èµå©é¸£è°¢ï¼ç§é¿ãç·äººä»¬çå®è¿å·ãæµ·ä¸æéæ´æ¯ä¼ è¯´
 ç¨ææ± 
 æ»è¹åª {{ data['rareCount']}}
 å·²æ¥æ {{ data['rareHave']}}
 {% for haveData in data['rareHaveList'] %} {% if haveData['level'] == 10 %}
 {{ haveData['level'] }}   {{ haveData['nameCn'] }}
 {% endif %} {% endfor %} {% for haveData in data['rareHaveList'] %} {% if
 haveData['level'] == 9 %}
```

### Comparing `hikari_core-0.1.5/hikari_core/Template/wws-clan.html` & `hikari_core-0.1.6/hikari_core/Template/wws-clan.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.5/hikari_core/Template/wws-info-recent.html` & `hikari_core-0.1.6/hikari_core/Template/wws-ship-recent.html`

 * *Files 10% similar despite different names*

```diff
@@ -5,394 +5,434 @@
 		<title></title>
 	</head>
 	<style>
 		* {
 			padding: 0;
 			margin: 0;
 		}
-		
+
 		.flex-2 {
 			flex: 2;
 		}
-		
+
 		.flex-3 {
 			flex: 3;
 		}
-		
+
 		.flex-4 {
 			flex: 4;
 		}
-		
+
 		.flex-8 {
 			flex: 8;
 		}
-		
+
 		.flex-10 {
 			flex: 10;
 		}
-		
+
 		.main-content {
-			width: 1500px;
+			width: 1000px;
 			font-size: 30px;
 			font-family: "Microsoft YaHei";
 			font-weight: bold;
 		}
-		
+
 		.page-box {
-			width: 1500px;
+			width: 1000px;
 			display: flex;
 			flex-direction: column;
 		}
-		
+
 		.page-header {
 			display: flex;
 			flex-direction: column;
 		}
-		
+
 		.clan-user-server {
 			height: 120px;
 			text-align: center;
 			font-size: 45px;
 			line-height: 120px;
 		}
-		
+
 		.clan {
 			display: inline-block;
 			padding-right: 10px;
 			height: 120px;
 		}
-		
+
 		.user {
 			display: inline-block;
 			height: 120px;
 		}
-		
+
 		.server {
 			display: inline-block;
 			padding-left: 10px;
 		}
-		
+
 		.server-border {
 			width: 200px;
 			height: 50px;
 			line-height: 50px;
 			text-align: center;
 			background-color: #F2F2F2;
 			border-radius: 25px;
 			font-size: 35px;
 		}
-		
+
+		.ship-bar {
+			height: 80px;
+			font-size: 40px;
+			line-height: 80px;
+			text-align: center;
+			display: flex;
+		}
+
+		.ship-level {
+			flex: 1;
+			text-align: right;
+			margin-right: 30px;
+		}
+
+		.ship-icon {
+			flex: 1;
+			text-align: left;
+			margin-left: 30px;
+		}
+
+		.ship-icon img {
+			width: 80px;
+			height: 80px;
+		}
+
 		.pr {
 			display: flex;
-			height: 120px;
+			height: 100px;
 			font-weight: bold;
 			line-height: 60px;
-			padding: 0 100px;
+			padding: 0 50px;
 		}
-		
+
 		.pr-bar-bg {
 			position: relative;
 			flex: 1;
 			line-height: 80px;
 			background-color: #A6A6A6;
 			height: 80px;
 			border-radius: 40px;
 			margin-top: 10px;
 			text-align: center;
 			color: #FFFFFF;
 		}
-		
+
 		.pr-bar {
 			position: absolute;
 			top: 0;
 			left: 0;
 			height: 80px;
 			z-index: 1;
 			border-radius: 40px;
 		}
-		
+
 		.pr-number {
 			z-index: 99;
 			position: absolute;
 			left: 0px;
 			right: 0px;
 			font-size: 35px;
 			font-weight: bold;
 		}
-		
+
 		.recnet-time {
 			text-align: center;
 			font-weight: normal;
 		}
-		
+
 		.overview-change {
 			display: flex;
 			margin-top: 30px;
-			padding: 0 80px;
-			height: 450px;
+			padding: 0 30px;
+			height: 300px;
 		}
-		
+
 		.overview-change-item {
 			flex: 1;
 			display: flex;
 			flex-direction: column;
 			margin: 0 20px;
-		
+
 		}
-		
+
 		.item-top {
 			flex: 5;
 			background-color: #F2F2F2;
 			border-radius: 16px;
 		}
-		
+
 		.item-bottom {
 			display: flex;
 			flex: 4;
 			margin-top: 20px;
 		}
-		
+
 		.left-item-bottom {
 			background-color: #F2F2F2;
 			border-radius: 16px;
 		}
-		
+
 		.bottom-mini-item-left {
 			flex: 1;
 			margin-right: 10px;
 			background-color: #F2F2F2;
 			border-radius: 16px;
 		}
-		
+
 		.bottom-mini-item-right {
 			flex: 1;
 			margin-left: 10px;
 			background-color: #F2F2F2;
 			border-radius: 16px;
 		}
-		
+
 		.item-top {
 			display: flex;
 			flex-direction: column;
 		}
-		
+
 		.item-top div {
-			height: 120px;
+			height: 80px;
 			text-align: center;
-			font-size: 60px;
+			font-size: 40px;
 		}
-		
+
 		.item-top-top {
 			color: #606266;
 			font-weight: normal;
-			line-height: 150px;
+			line-height: 100px;
 		}
-		
+
 		.item-top-bottom {
-			line-height: 90px;
+			line-height: 60px;
 		}
-		
+
 		.left-item-bottom {
 			display: flex;
 			flex-direction: column;
 		}
-		
+
 		.change-pr-title {
 			color: #606266;
-			height: 95px;
+			height: 60px;
 			display: flex;
 			font-weight: normal;
-			line-height: 125px;
+			line-height: 70px;
 		}
-		
+
 		.change-pr {
-			height: 95px;
-			line-height: 75px;
+			height: 60px;
+			line-height: 50px;
 			text-align: center;
-			font-size: 45px;
+			font-size: 30px;
 		}
-		
+
 		.change-pr-title-left {
 			flex: 1;
-			font-size: 50px;
+			font-size: 35px;
 			text-align: right;
-			margin-right: 20px;
+			margin-right: 30px;
 		}
-		
+
 		.change-pr-title-right {
 			flex: 1;
+			font-size: 20px;
 		}
-		
+
 		.bottom-mini-item-left,
 		.bottom-mini-item-right {
 			display: flex;
 			flex-direction: column;
 		}
-		
+
 		.mini-item-top {
 			color: #606266;
 			font-weight: normal;
-			line-height: 135px;
+			line-height: 70px;
 		}
-		
+
 		.mini-item-bottom {
 			line-height: 45px;
+			font-size: 27px;
 		}
-		
+
 		.bottom-mini-item-left div,
 		.bottom-mini-item-right div {
-			height: 95px;
+			height: 60px;
 			text-align: center;
-			font-size: 35px;
 		}
-		
-		.information-header {
-			margin: 0 400px;
+
+		.information-header,
+		.day-header {
+			margin: 0 200px;
 			margin-top: 30px;
 			height: 60px;
 			line-height: 60px;
 			border-radius: 16px;
 			background-color: #D9D9D9;
 			text-align: center;
 		}
-		
+
 		.information-body {
-			margin: 0 100px;
+			margin: 0 50px;
 			margin-top: 30px;
 			display: flex;
 			flex-direction: column;
 			background-color: #F2F2F2;
 			border-radius: 16px;
 		}
-		
+
 		.information-col {
 			height: 60px;
 			display: flex;
 			line-height: 60px;
 		}
-		
-		.information-col-item {
+
+		.information-col-item,
+		.day-col-item {
 			flex: 1;
 			text-align: center;
 		}
-		
+
 		.information-table-header {
 			color: #606266;
 		}
-		
+
 		.information-type {
 			color: #909399;
 		}
-		
-		.random-header {
-			margin: 0 400px;
+
+		.day-body {
+			margin: 0 50px;
 			margin-top: 30px;
+		}
+
+		.day-table-header {
 			height: 60px;
 			line-height: 60px;
-			border-radius: 16px;
 			background-color: #D9D9D9;
-			text-align: center;
-		}
-		
-		.random-data {
 			display: flex;
-			flex-direction: column;
-			margin: 0 100px;
-			margin-top: 30px;
-			background-color: #F2F2F2;
 			border-radius: 16px;
+			color: #606266;
 		}
-		
-		.random-data-col {
-			display: flex;
-			height: 90px;
-		}
-		
-		.random-col-item {
-			line-height: 90px;
+
+		.date {
+			background-color: #D9D9D9;
+			width: 300px;
+			height: 40px;
+			line-height: 40px;
 			text-align: center;
+			border-radius: 20px;
+			margin-top: 10px;
 		}
-		
-		.random-table-header {
-			color: #606266;
-			height: 60px;
+
+		.day-col {
 			display: flex;
-		}
-		
-		.random-table-header .random-col-item {
+			height: 60px;
 			line-height: 60px;
+			background-color: #F2F2F2;
+			border-radius: 30px;
+			margin: 10px 0;
 		}
-		
+
 		.footer {
 			margin-top: 30px;
 			text-align: center;
 			font-weight: bold;
 			font-size: 24px;
 			color: #909399;
 			margin-bottom: 20px;
 		}
-		
-		.rank-data-col {
-			display: flex;
-			height: 90px;
-		}
 	</style>
 	<body>
 		<div class="main-content">
 			<div class="page-box">
-				
 				<div class="page-header">
 					<div class="clan-user-server">
+						
 						{% if data['clanInfo']['tag'] %}
 						<div class="clan" style="color: {{ data['clanInfo']['colorRgb'] }};">[{{ data['clanInfo']['tag'] }}]</div>
 						{% endif %}
 						<div class="user">{{ data['userName'] }}</div>
 						<div class="server">
 							<div class="server-border">
 								{{ data['serverName'] }}
 							</div>
 						</div>
 					</div>
 				</div>
-				
+
+				<div class="ship-bar">
+					{% if data['shipData'][0]['shipInfo']['shipInfo']['nameCn'] %}
+					<div class="ship-level">{{ data['shipData'][0]['shipInfo']['shipInfo']['level'] }}</div>
+					{% else %}
+					<div class="ship-level">{{ data['shipData'][0]['rankSolo']['shipInfo']['level'] }}</div>
+					{% endif %}
+					
+					{% if data['shipData'][0]['shipInfo']['shipInfo']['nameCn'] %}
+					<div class="ship-name">{{ data['shipData'][0]['shipInfo']['shipInfo']['nameCn'] }}</div>
+					{% else %}
+					<div class="ship-name">{{ data['shipData'][0]['rankSolo']['shipInfo']['nameCn'] }}</div>
+					{% endif %}
+					
+					<div class="ship-icon"><img
+									src={% if data['shipData'][0]['shipInfo']['shipInfo']['shipType'] == 'Destroyer' or data['shipData'][0]['rankSolo']['shipInfo']['shipType'] == 'Destroyer' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_destroyer.png"
+									{% elif data['shipData'][0]['shipInfo']['shipInfo']['shipType'] == 'Cruiser' or data['shipData'][0]['rankSolo']['shipInfo']['shipType'] == 'Cruiser' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_cruiser.png"
+									{% elif data['shipData'][0]['shipInfo']['shipInfo']['shipType'] == 'Battleship' or data['shipData'][0]['rankSolo']['shipInfo']['shipType'] == 'Battleship' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_battleship.png"
+									{% elif data['shipData'][0]['shipInfo']['shipInfo']['shipType'] == 'AirCarrier' or data['shipData'][0]['rankSolo']['shipInfo']['shipType'] == 'AirCarrier' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_aircarrier.png"
+									{% else %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_submarine.png"
+									{% endif %} />
+					</div>
+				</div>
+
 				<div class="pr">
 					<!-- 动态设置长度及颜色，填写PR即可 -->
 					<div class="pr-bar-bg">
-						{% if data['shipData'][0]['pvpInfo']['pr']['color'] != '#828282' %}
-						<span class="pr-number">{{ data['shipData'][0]['pvpInfo']['pr']['value'] }}&nbsp;&nbsp;&nbsp;&nbsp;<span class="pr-text"></span></span>
+						{% if data['pvpInfo']['pr']['color'] and data['pvpInfo']['pr']['color'] != '#828282' %}
+						<span class="pr-number">{{ data['pvpInfo']['pr']['value'] }} &nbsp;&nbsp;&nbsp;&nbsp;<span class="pr-text"></span></span>
 						{% else %}
-						<span class="pr-number">{{ data['shipData'][0]['rankInfo']['pr']['value'] }}&nbsp;&nbsp;&nbsp;&nbsp;<span class="pr-text"></span></span>
+						<span class="pr-number">{{ data['rankInfo']['pr']['value'] }} &nbsp;&nbsp;&nbsp;&nbsp;<span class="pr-text"></span></span>
 						{% endif %}
 						<div class="pr-bar"></div>
 					</div>
 				</div>
-				
+
 				<div class="recnet-time">
 					<span>记录时间：</span><span>{{ time.strftime('%Y-%m-%d %H:%M',time.localtime(int(abs(data['shipData'][0]['recordDateTime']/1000)))) }}—{{ time.strftime('%Y-%m-%d %H:%M',time.localtime(time.time())) }}</span>
 				</div>
-				
-				{% if data['shipData'][0]['pvpInfo']['battles'] %}
+
+				{% if data['pvpInfo']['battles'] %}
 				<div class="overview-change">
 					<div class="overview-change-item left-item">
 						<div class="left-item-top item-top">
 							<div class="overview-count-title item-top-top">场次</div>
-							<div class="overview-count item-top-bottom">{{ data['shipData'][0]['pvpInfo']['battles'] }}</div>
+							<div class="overview-count item-top-bottom">{{ data['pvpInfo']['battles'] }}</div>
 						</div>
 						<div class="left-item-bottom item-bottom">
 							<div class="change-pr-title">
 								<div class="change-pr-title-left">PR</div>
 								<div class="change-pr-title-right">较上周</div>
 							</div>
 							<div class="change-pr">暂不可用</div>
 						</div>
 					</div>
 					<div class="overview-change-item mid-item">
 						<div class="mid-item-top item-top">
 							<div class="overview-win-title item-top-top">胜率</div>
-							<div class="overview-win item-top-bottom" style="color: {{ data['shipData'][0]['pvpInfo']['winsData']['color'] }};">{{ data['shipData'][0]['pvpInfo']['wins'] }}%</div>
+							<div class="overview-win item-top-bottom" style="color: {{ data['pvpInfo']['winsData']['color'] }}">{{ data['pvpInfo']['wins'] }}%</div>
 						</div>
 						<div class="mid-item-bottom item-bottom">
 							<div class="change-avgdmg-box bottom-mini-item-left">
 								<div class="mini-item-top">场均</div>
 								<div class="mini-item-bottom change-avgdmg">暂不可用</div>
 							</div>
 							<div class="change-win-box bottom-mini-item-right">
@@ -400,171 +440,142 @@
 								<div class="mini-item-bottom change-win">暂不可用</div>
 							</div>
 						</div>
 					</div>
 					<div class="overview-change-item right-item">
 						<div class="right-item-top item-top">
 							<div class="overview-avgdmg-title item-top-top">场均</div>
-							<div class="overview-avgdmg item-top-bottom" style="color: {{ data['shipData'][0]['pvpInfo']['damageData']['color'] }};">{{ data['shipData'][0]['pvpInfo']['damage'] }}</div>
+							<div class="overview-avgdmg item-top-bottom" style="color: {{ data['pvpInfo']['damageData']['color'] }};">{{ data['pvpInfo']['damage'] }}</div>
 						</div>
 						<div class="right-item-bottom item-bottom">
 							<div class="overview-kd-box bottom-mini-item-left">
 								<div class="mini-item-top">击杀</div>
-								<div class="mini-item-bottom">{{ '%.2f' | format(data['shipData'][0]['pvpInfo']['frags']) }}</div>
+								<div class="mini-item-bottom">{{ '%.2f' | format(data['pvpInfo']['frags']) }}</div>
 							</div>
 							<div class="overview-hit-box bottom-mini-item-right">
 								<div class="mini-item-top">命中</div>
-								<div class="mini-item-bottom">{{ '%.2f' | format(data['shipData'][0]['pvpInfo']['hit']) }}%</div>
+								<div class="mini-item-bottom">{{ data['pvpInfo']['hit'] }}%</div>
 							</div>
 						</div>
 					</div>
 				</div>
 				{% endif %}
-				
-				
+
 				<div class="information-header">总体战绩</div>
-				
+
 				<div class="information-body">
 					<div class="information-col information-table-header">
 						<div class="information-col-item">类型</div>
 						<div class="information-col-item">场次</div>
 						<div class="information-col-item">胜率</div>
 						<div class="information-col-item">PR</div>
 						<div class="information-col-item">场均</div>
 						<div class="information-col-item">击杀</div>
-						<div class="information-col-item">命中</div>
 					</div>
-					{% if data['shipData'][0]['pvpSoloInfo']['battles'] %}
+					
+					{% if data['pvpSoloInfo']['battles'] %}
 					<div class="information-col">
 						<div class="information-col-item information-type">单野</div>
-						<div class="information-col-item">{{ data['shipData'][0]['pvpSoloInfo']['battles'] }}</div>
-						<div class="information-col-item" style="color: {{ data['shipData'][0]['pvpSoloInfo']['winsData']['color'] }};">{{ data['shipData'][0]['pvpSoloInfo']['wins'] }}%</div>
-						<div class="information-col-item" style="color: {{ data['shipData'][0]['pvpSoloInfo']['pr']['color'] }};">{{ data['shipData'][0]['pvpSoloInfo']['pr']['value'] }}</div>
-						<div class="information-col-item" style="color: {{ data['shipData'][0]['pvpSoloInfo']['damageData']['color'] }};">{{ data['shipData'][0]['pvpSoloInfo']['damage'] }}</div>
-						<div class="information-col-item">{{ '%.2f' | format(data['shipData'][0]['pvpSoloInfo']['frags']) }}</div>
-						<div class="information-col-item">{{ '%.2f' | format(data['shipData'][0]['pvpSoloInfo']['hit']) }}%</div>
+						<div class="information-col-item">{{ data['pvpSoloInfo']['battles'] }}</div>
+						<div class="information-col-item" style="color: {{ data['pvpSoloInfo']['winsData']['color'] }};">{{ data['pvpSoloInfo']['wins'] }}%</div>
+						<div class="information-col-item" style="color: {{ data['pvpSoloInfo']['pr']['color'] }};">{{ data['pvpSoloInfo']['pr']['value'] }}</div>
+						<div class="information-col-item" style="color: {{ data['pvpSoloInfo']['damageData']['color'] }};">{{ data['pvpSoloInfo']['damage'] }}</div>
+						<div class="information-col-item">{{ '%.2f' | format(data['pvpSoloInfo']['frags']) }}</div>
 					</div>
 					{% endif %}
-					
-					{% if data['shipData'][0]['pvpTwoInfo']['battles'] %}
+
+					{% if data['pvpTwoInfo']['battles'] %}
 					<div class="information-col">
 						<div class="information-col-item information-type">自行车</div>
-						<div class="information-col-item">{{ data['shipData'][0]['pvpTwoInfo']['battles'] }}</div>
-						<div class="information-col-item" style="color: {{ data['shipData'][0]['pvpTwoInfo']['winsData']['color'] }};">{{ data['shipData'][0]['pvpTwoInfo']['wins'] }}%</div>
-						<div class="information-col-item" style="color: {{ data['shipData'][0]['pvpTwoInfo']['pr']['color'] }};">{{ data['shipData'][0]['pvpTwoInfo']['pr']['value'] }}</div>
-						<div class="information-col-item" style="color: {{ data['shipData'][0]['pvpTwoInfo']['damageData']['color'] }};">{{ data['shipData'][0]['pvpTwoInfo']['damage'] }}</div>
-						<div class="information-col-item">{{ '%.2f' | format(data['shipData'][0]['pvpTwoInfo']['frags']) }}</div>
-						<div class="information-col-item">{{ '%.2f' | format(data['shipData'][0]['pvpTwoInfo']['hit']) }}%</div>
+						<div class="information-col-item">{{ data['pvpTwoInfo']['battles'] }}</div>
+						<div class="information-col-item" style="color: {{ data['pvpTwoInfo']['winsData']['color'] }};">{{ data['pvpTwoInfo']['wins'] }}%</div>
+						<div class="information-col-item" style="color: {{ data['pvpTwoInfo']['pr']['color'] }};">{{ data['pvpTwoInfo']['pr']['value'] }}</div>
+						<div class="information-col-item" style="color: {{ data['pvpTwoInfo']['damageData']['color'] }};">{{ data['pvpTwoInfo']['damage'] }}</div>
+						<div class="information-col-item">{{ '%.2f' | format(data['pvpTwoInfo']['frags']) }}</div>
 					</div>
 					{% endif %}
-					
-					{% if data['shipData'][0]['pvpThreeInfo']['battles'] %}
+
+
+					{% if data['pvpThreeInfo']['battles'] %}
 					<div class="information-col">
 						<div class="information-col-item information-type">三轮车</div>
-						<div class="information-col-item">{{ data['shipData'][0]['pvpThreeInfo']['battles'] }}</div>
-						<div class="information-col-item" style="color: {{ data['shipData'][0]['pvpThreeInfo']['winsData']['color'] }};">{{ data['shipData'][0]['pvpThreeInfo']['wins'] }}%</div>
-						<div class="information-col-item" style="color: {{ data['shipData'][0]['pvpThreeInfo']['pr']['color'] }};">{{ data['shipData'][0]['pvpThreeInfo']['pr']['value'] }}</div>
-						<div class="information-col-item" style="color: {{ data['shipData'][0]['pvpThreeInfo']['damageData']['color'] }};">{{ data['shipData'][0]['pvpThreeInfo']['damage'] }}</div>
-						<div class="information-col-item">{{ '%.2f' | format(data['shipData'][0]['pvpThreeInfo']['frags']) }}</div>
-						<div class="information-col-item">{{ '%.2f' | format(data['shipData'][0]['pvpThreeInfo']['hit']) }}%</div>
+						<div class="information-col-item">{{ data['pvpThreeInfo']['battles'] }}</div>
+						<div class="information-col-item" style="color: {{ data['pvpThreeInfo']['winsData']['color'] }};">{{ data['pvpThreeInfo']['wins'] }}%</div>
+						<div class="information-col-item" style="color: {{ data['pvpThreeInfo']['pr']['color'] }};">{{ data['pvpThreeInfo']['pr']['value'] }}</div>
+						<div class="information-col-item" style="color: {{ data['pvpThreeInfo']['damageData']['color'] }};">{{ data['pvpThreeInfo']['damage'] }}</div>
+						<div class="information-col-item">{{ '%.2f' | format(data['pvpThreeInfo']['frags']) }}</div>
 					</div>
 					{% endif %}
-					
-					{% if data['shipData'][0]['rankInfo']['battles'] %}
+
+
+					{% if data['rankInfo']['battles'] %}
 					<div class="information-col">
 						<div class="information-col-item information-type">排位</div>
-						<div class="information-col-item">{{ data['shipData'][0]['rankInfo']['battles'] }}</div>
-						<div class="information-col-item" style="color: {{ data['shipData'][0]['rankInfo']['winsData']['color'] }};">{{ data['shipData'][0]['rankInfo']['wins'] }}%</div>
-						<div class="information-col-item" style="color: {{ data['shipData'][0]['rankInfo']['pr']['color'] }};">{{ data['shipData'][0]['rankInfo']['pr']['value'] }}</div>
-						<div class="information-col-item" style="color: {{ data['shipData'][0]['rankInfo']['damageData']['color'] }};">{{ data['shipData'][0]['rankInfo']['damage'] }}</div>
-						<div class="information-col-item">{{ '%.2f' | format(data['shipData'][0]['rankInfo']['frags']) }}</div>
-						<div class="information-col-item">{{ '%.2f' | format(data['shipData'][0]['rankInfo']['hit']) }}%</div>
+						<div class="information-col-item">{{ data['rankInfo']['battles'] }}</div>
+						<div class="information-col-item" style="color: {{ data['rankInfo']['winsData']['color'] }};">{{ data['rankInfo']['wins'] }}%</div>
+						<div class="information-col-item" style="color: {{ data['rankInfo']['pr']['color'] }};">{{ data['rankInfo']['pr']['value'] }}</div>
+						<div class="information-col-item" style="color: {{ data['rankInfo']['damageData']['color'] }};">{{ data['rankInfo']['damage'] }}</div>
+						<div class="information-col-item">{{ '%.2f' | format(data['rankInfo']['frags']) }}</div>
 					</div>
 					{% endif %}
+
 				</div>
-				
-				{% if data['shipData'][0]['pvpInfo']['battles'] %}
-				<div class="random-header">随机战数据</div>
-				{% endif %}
-				
-				{% if data['shipData'][0]['pvpInfo']['battles'] %}
-				<div class="random-data">
-					<div class="random-table-header">
-						<div class="random-col-item flex-3">等级</div>
-						<div class="random-col-item flex-8">战舰</div>
-						<div class="random-col-item flex-3">场次</div>
-						<div class="random-col-item flex-3">PR</div>
-						<div class="random-col-item flex-3">胜率</div>
-						<div class="random-col-item flex-4">场均</div>
-						<div class="random-col-item flex-3">击杀</div>
-						<div class="random-col-item flex-3">命中</div>
-					</div>
-					{% for ship in data['shipData'][0]['shipData'] %}
-						{% if ship['shipInfo']['battles'] %}
-						<div class="random-data-col">
-							<div class="random-col-item flex-3 ship-level">{{ ship['shipInfo']['shipInfo']['level'] }}</div>
-							<div class="random-col-item flex-8">{{ ship['shipInfo']['shipInfo']['nameCn'] }}</div>
-							<div class="random-col-item flex-3">{{ ship['shipInfo']['battles'] }}</div>
-							<div class="random-col-item flex-3" style="color: {{ ship['shipInfo']['pr']['color'] }};">{{ ship['shipInfo']['pr']['value'] }}</div>
-							<div class="random-col-item flex-3" style="color: {{ ship['shipInfo']['winsData']['color'] }};">{{ ship['shipInfo']['wins'] }}%</div>
-							<div class="random-col-item flex-4" style="color: {{ ship['shipInfo']['damageData']['color'] }};">{{ ship['shipInfo']['damage'] }}</div>
-							<div class="random-col-item flex-3">{{ '%.2f' | format(ship['shipInfo']['frags']) }}</div>
-							<div class="random-col-item flex-3">{{ '%.2f' | format(ship['shipInfo']['hit']) }}%</div>
-						</div>
-						{% endif %}
-					{% endfor %}
-				</div>
-				{% endif %}
-				
-				<!-- 以下为排位数据，不再额外做类名样式 -->
-				{% if data['shipData'][0]['rankInfo']['battles'] %}
-				<div class="random-header">排位战数据</div>
-				{% endif %}
-				
-				{% if data['shipData'][0]['rankInfo']['battles'] %}
-				<div class="random-data">
-					<div class="random-table-header">
-						<div class="random-col-item flex-3">等级</div>
-						<div class="random-col-item flex-8">战舰</div>
-						<div class="random-col-item flex-3">场次</div>
-						<div class="random-col-item flex-3">PR</div>
-						<div class="random-col-item flex-3">胜率</div>
-						<div class="random-col-item flex-4">场均</div>
-						<div class="random-col-item flex-3">击杀</div>
-						<div class="random-col-item flex-3">命中</div>
-					</div>
-					{% for ship in data['shipData'][0]['shipData'] %}
-						{% if ship['rankSolo']['battles'] %}
-						<div class="rank-data-col">
-							<div class="random-col-item flex-3 ship-level">{{ ship['rankSolo']['shipInfo']['level'] }}</div>
-							<div class="random-col-item flex-8">{{ ship['rankSolo']['shipInfo']['nameCn'] }}</div>
-							<div class="random-col-item flex-3">{{ ship['rankSolo']['battles'] }}</div>
-							<div class="random-col-item flex-3" style="color: {{ ship['rankSolo']['pr']['color'] }};">{{ ship['rankSolo']['pr']['value'] }}</div>
-							<div class="random-col-item flex-3" style="color: {{ ship['rankSolo']['winsData']['color'] }};">{{ ship['rankSolo']['wins'] }}%</div>
-							<div class="random-col-item flex-4" style="color: {{ ship['rankSolo']['damageData']['color'] }};">{{ ship['rankSolo']['damage'] }}</div>
-							<div class="random-col-item flex-3">{{ '%.2f' | format(ship['rankSolo']['frags']) }}</div>
-							<div class="random-col-item flex-3">{{ '%.2f' | format(ship['rankSolo']['hit']) }}%</div>
+
+				<div class="day-header">每日战绩</div>
+
+				<div class="day-body">
+					<div class="day-table-header">
+						<div class="day-col-item">类型</div>
+						<div class="day-col-item">场次</div>
+						<div class="day-col-item">胜率</div>
+						<div class="day-col-item">PR</div>
+						<div class="day-col-item">场均</div>
+						<div class="day-col-item">击杀</div>
+					</div>
+
+
+						<div class="data-item">
+							{% for eachShipData in data['shipData'] %}
+							    {% if eachShipData['shipInfo']['battles'] or eachShipData['rankSolo']['battles'] %}
+								<div class="date">{{ time.strftime('%Y-%m-%d',time.localtime(int(abs(eachShipData['recordDateTime']/1000)))) }}</div>
+									{% for each in eachShipData %}
+										{% for index,value in enumerate(['shipSolo','shipTwo','shipThree','rankSolo']) %}
+											{% if each|string == value and eachShipData[each]['battles'] %}
+											<div class="day-data">
+												<div class="day-col">
+													<div class="day-col-item" style="color: #606266;;">{{ ['单野','自行车','三轮车','排位'][index] }}</div>
+													<div class="day-col-item">{{ eachShipData[each]['battles'] }}</div>
+													<div class="day-col-item" style="color: {{ eachShipData[each]['winsData']['color'] }};">{{ eachShipData[each]['wins'] }}%</div>
+													<div class="day-col-item" style="color: {{ eachShipData[each]['pr']['color'] }};">{{ eachShipData[each]['pr']['value'] }}</div>
+													<div class="day-col-item" style="color: {{ eachShipData[each]['damageData']['color'] }};">{{ eachShipData[each]['damage'] }}</div>
+													<div class="day-col-item">{{ '%.2f' | format(eachShipData[each]['frags']) }}</div>
+												</div>
+											</div>
+											{% endif %}
+										{% endfor %}
+									{% endfor %}
+								{% endif %}
+							{% endfor %}
 						</div>
-						{% endif %}
-					{% endfor %}
-				</div>
-				{% endif %}
-				
-				<div class="footer">
-					<p>©西行寺雨季&nbsp;&nbsp;©本心</p>
-					<p>https://github.com/benx1n/HikariBot</p>
-					<p>QQ频道搜索”yuyuko”即可使用稳定的腾讯官方机器人~</p>
-					<p>Design By 冷眠 H5 Converted By C1ystal</p>
-					<p>赞助鸣谢：男人们的定远号、Wishing、科长</p>
+
+					<div class="footer">
+						<p>©西行寺雨季&nbsp;&nbsp;©本心</p>
+						<p>https://github.com/benx1n/HikariBot</p>
+						<p>QQ频道搜索”yuyuko”即可使用稳定的腾讯官方机器人~</p>
+						<p>Design By 冷眠 H5 Converted By C1ystal</p>
+						<p>赞助鸣谢：科长、男人们的定远号、海上最速暴毙传说</p>
+					</div>
+
 				</div>
-				
+
+
+
 			</div>
 		</div>
 	</body>
-	
 	<script>
 		// PR条颜色动态变化
 		let bar_bg_width = document.querySelector('.pr-bar-bg').clientWidth;
 		let pr_number = document.querySelector('.pr-number').innerText;
 		pr_number = parseInt(pr_number);
 		if (pr_number == 0) {
 			document.querySelector(".pr-bar").style.backgroundColor = "#828282";
@@ -592,23 +603,23 @@
 			document.querySelector(".pr-bar").style.backgroundColor = "#9C27B0";
 			document.querySelector(".pr-text").innerText = "大佬水平";
 		} else {
 			document.querySelector(".pr-bar").style.backgroundColor = "#673AB7";
 			document.querySelector(".pr-text").innerText = "神佬水平";
 			pr_number = 2450; //防止pr条溢出
 		}
-	
+
 		if (pr_number < 220 && pr_number > 0) {
 			pr_number = 220; //防止pr过低导致圆角异常
 		}
 		// PR条动态长度
 		let width = bar_bg_width * (pr_number / 2450);
 		document.querySelector('.pr-bar').style.width = width + "px";
 	</script>
-	
+
 	<script>
 		// 服务器字体颜色自动填充
 		let server_name = document.querySelector(".server").innerText;
 		if (server_name == "亚服") {
 			document.querySelector(".server").style.color = "#92D050";
 		} else if (server_name == "国服") {
 			document.querySelector(".server").style.color = "#BF9000";
@@ -616,87 +627,60 @@
 			document.querySelector(".server").style.color = "#009664";
 		} else if (server_name == "美服") {
 			document.querySelector(".server").style.color = "#6872C4";
 		} else if (server_name == "俄服") {
 			document.querySelector(".server").style.color = "#FF0000";
 		}
 	</script>
-	
+
 	<script>
 		// 数据变化动态颜色填充
 		let change_avgdmg = document.querySelector(".change-avgdmg").innerText;
 		change_avgdmg = parseInt(change_avgdmg);
-	
+
 		let change_win = document.querySelector(".change-win").innerText;
 		change_win = change_win.split("%", 1);
 		change_win = parseFloat(change_win);
-	
+
 		let change_pr = document.querySelector(".change-pr").innerText;
 		change_pr = parseInt(change_pr);
-	
+
 		if (change_avgdmg > 0) {
 			document.querySelector(".change-avgdmg").style.color = "#70AD47";
 		} else {
 			document.querySelector(".change-avgdmg").style.color = "#FF0000";
 		}
-	
+
 		if (change_win > 0) {
 			document.querySelector(".change-win").style.color = "#70AD47";
 		} else {
 			document.querySelector(".change-win").style.color = "#FF0000";
 		}
-	
+
 		if (change_pr > 0) {
 			document.querySelector(".change-pr").style.color = "#70AD47";
 		} else {
 			document.querySelector(".change-pr").style.color = "#FF0000";
 		}
 	</script>
-	
+
+	<script>
+		let ship_level = document.querySelector(".ship-level").innerText;
+		let level_number = ["1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "11"];
+		let level_roma = ["I", "II", "III", "IV", "V", "VI", "VII", "VIII", "IX", "X", "★"];
+		let ship_level_roma = level_roma[level_number.indexOf(ship_level)]
+		document.querySelector(".ship-level").innerText = ship_level_roma;
+	</script>
+
 	<script>
 		let arr_information = document.getElementsByClassName('information-col');
-		for(let i=0;i<arr_information.length;i++) {
-			if(i%2 != 0 && i == (arr_information.length-1)) {
+		for (let i = 0; i < arr_information.length; i++) {
+			if (i % 2 != 0 && i == (arr_information.length - 1)) {
 				arr_information[i].style.backgroundColor = "#E4E4E4";
 				arr_information[i].style.borderBottomLeftRadius = "16px";
 				arr_information[i].style.borderBottomRightRadius = "16px";
-			} else if (i%2 != 0) {
+			} else if (i % 2 != 0) {
 				arr_information[i].style.backgroundColor = "#E4E4E4";
 			}
 		}
 	</script>
-	
-	<script>
-		let arr_random = document.getElementsByClassName('random-data-col');
-		for(let i=0;i<arr_random.length;i++) {
-			if(i%2 == 0 && i == (arr_random.length-1)) {
-				arr_random[i].style.backgroundColor = "#E4E4E4";
-				arr_random[i].style.borderBottomLeftRadius = "16px";
-				arr_random[i].style.borderBottomRightRadius = "16px";
-			} else if (i%2 == 0) {
-				arr_random[i].style.backgroundColor = "#E4E4E4";
-			}
-		}
-	</script>
-	
-	<script>
-		let ship_level_doc = document.getElementsByClassName('ship-level');
-		let level_number = ["1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "11"];
-		let level_roma = ["I", "II", "III", "IV", "V", "VI", "VII", "VIII", "IX", "X", "★"];
-		for(let k=0;k<ship_level_doc.length;k++) {
-			ship_level_doc[k].innerText = level_roma[level_number.indexOf(ship_level_doc[k].innerText)];
-		}
-	</script>
-	
-	<script>
-		let arr_rank = document.getElementsByClassName('rank-data-col');
-		for(let i=0;i<arr_rank.length;i++) {
-			if(i%2 == 0 && i == (arr_rank.length-1)) {
-				arr_rank[i].style.backgroundColor = "#E4E4E4";
-				arr_rank[i].style.borderBottomLeftRadius = "16px";
-				arr_rank[i].style.borderBottomRightRadius = "16px";
-			} else if (i%2 == 0) {
-				arr_rank[i].style.backgroundColor = "#E4E4E4";
-			}
-		}
-	</script>
 </html>
```

#### html2text {}

```diff
@@ -1,121 +1,117 @@
 {% if data['clanInfo']['tag'] %}
 [{{ data['clanInfo']['tag'] }}]
 {% endif %}
 {{ data['userName'] }}
 {{ data['serverName'] }}
-{% if data['shipData'][0]['pvpInfo']['pr']['color'] != '#828282' %} {{ data
-['shipData'][0]['pvpInfo']['pr']['value'] }}     {% else %} {{ data['shipData']
-[0]['rankInfo']['pr']['value'] }}     {% endif %}
+{% if data['shipData'][0]['shipInfo']['shipInfo']['nameCn'] %}
+{{ data['shipData'][0]['shipInfo']['shipInfo']['level'] }}
+{% else %}
+{{ data['shipData'][0]['rankSolo']['shipInfo']['level'] }}
+{% endif %} {% if data['shipData'][0]['shipInfo']['shipInfo']['nameCn'] %}
+{{ data['shipData'][0]['shipInfo']['shipInfo']['nameCn'] }}
+{% else %}
+{{ data['shipData'][0]['rankSolo']['shipInfo']['nameCn'] }}
+{% endif %}
+'shipData'][0]['shipInfo']['shipInfo']['shipType'] == 'Destroyer' or data
+['shipData'][0]['rankSolo']['shipInfo']['shipType'] == 'Destroyer' %} "https://
+hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/
+icon_sunk_destroyer.png" {% elif data['shipData'][0]['shipInfo']['shipInfo']
+['shipType'] == 'Cruiser' or data['shipData'][0]['rankSolo']['shipInfo']
+['shipType'] == 'Cruiser' %} "https://hikari-resource.oss-cn-
+shanghai.aliyuncs.com/shipType_Icon/icon_sunk_cruiser.png" {% elif data
+['shipData'][0]['shipInfo']['shipInfo']['shipType'] == 'Battleship' or data
+['shipData'][0]['rankSolo']['shipInfo']['shipType'] == 'Battleship' %} "https:/
+/hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/
+icon_sunk_battleship.png" {% elif data['shipData'][0]['shipInfo']['shipInfo']
+['shipType'] == 'AirCarrier' or data['shipData'][0]['rankSolo']['shipInfo']
+['shipType'] == 'AirCarrier' %} "https://hikari-resource.oss-cn-
+shanghai.aliyuncs.com/shipType_Icon/icon_sunk_aircarrier.png" {% else %}
+"https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/
+icon_sunk_submarine.png" {% endif %} />
+{% if data['pvpInfo']['pr']['color'] and data['pvpInfo']['pr']['color'] !=
+'#828282' %} {{ data['pvpInfo']['pr']['value'] }}      {% else %} {{ data
+['rankInfo']['pr']['value'] }}      {% endif %}
 è®°å½æ¶é´ï¼{{ time.strftime('%Y-%m-%d %H:%M',time.localtime(int(abs(data
 ['shipData'][0]['recordDateTime']/1000)))) }}â{{ time.strftime('%Y-%m-%d %H:
 %M',time.localtime(time.time())) }}
-{% if data['shipData'][0]['pvpInfo']['battles'] %}
+{% if data['pvpInfo']['battles'] %}
 åºæ¬¡
-{{ data['shipData'][0]['pvpInfo']['battles'] }}
+{{ data['pvpInfo']['battles'] }}
 PR
 è¾ä¸å¨
 æä¸å¯ç¨
 èç
-{{ data['shipData'][0]['pvpInfo']['wins'] }}%
+{{ data['pvpInfo']['wins'] }}%
 åºå
 æä¸å¯ç¨
 èç
 æä¸å¯ç¨
 åºå
-{{ data['shipData'][0]['pvpInfo']['damage'] }}
+{{ data['pvpInfo']['damage'] }}
 å»æ
-{{ '%.2f' | format(data['shipData'][0]['pvpInfo']['frags']) }}
+{{ '%.2f' | format(data['pvpInfo']['frags']) }}
 å½ä¸­
-{{ '%.2f' | format(data['shipData'][0]['pvpInfo']['hit']) }}%
+{{ data['pvpInfo']['hit'] }}%
 {% endif %}
 æ»ä½æç»©
 ç±»å
 åºæ¬¡
 èç
 PR
 åºå
 å»æ
-å½ä¸­
-{% if data['shipData'][0]['pvpSoloInfo']['battles'] %}
+{% if data['pvpSoloInfo']['battles'] %}
 åé
-{{ data['shipData'][0]['pvpSoloInfo']['battles'] }}
-{{ data['shipData'][0]['pvpSoloInfo']['wins'] }}%
-{{ data['shipData'][0]['pvpSoloInfo']['pr']['value'] }}
-{{ data['shipData'][0]['pvpSoloInfo']['damage'] }}
-{{ '%.2f' | format(data['shipData'][0]['pvpSoloInfo']['frags']) }}
-{{ '%.2f' | format(data['shipData'][0]['pvpSoloInfo']['hit']) }}%
-{% endif %} {% if data['shipData'][0]['pvpTwoInfo']['battles'] %}
+{{ data['pvpSoloInfo']['battles'] }}
+{{ data['pvpSoloInfo']['wins'] }}%
+{{ data['pvpSoloInfo']['pr']['value'] }}
+{{ data['pvpSoloInfo']['damage'] }}
+{{ '%.2f' | format(data['pvpSoloInfo']['frags']) }}
+{% endif %} {% if data['pvpTwoInfo']['battles'] %}
 èªè¡è½¦
-{{ data['shipData'][0]['pvpTwoInfo']['battles'] }}
-{{ data['shipData'][0]['pvpTwoInfo']['wins'] }}%
-{{ data['shipData'][0]['pvpTwoInfo']['pr']['value'] }}
-{{ data['shipData'][0]['pvpTwoInfo']['damage'] }}
-{{ '%.2f' | format(data['shipData'][0]['pvpTwoInfo']['frags']) }}
-{{ '%.2f' | format(data['shipData'][0]['pvpTwoInfo']['hit']) }}%
-{% endif %} {% if data['shipData'][0]['pvpThreeInfo']['battles'] %}
+{{ data['pvpTwoInfo']['battles'] }}
+{{ data['pvpTwoInfo']['wins'] }}%
+{{ data['pvpTwoInfo']['pr']['value'] }}
+{{ data['pvpTwoInfo']['damage'] }}
+{{ '%.2f' | format(data['pvpTwoInfo']['frags']) }}
+{% endif %} {% if data['pvpThreeInfo']['battles'] %}
 ä¸è½®è½¦
-{{ data['shipData'][0]['pvpThreeInfo']['battles'] }}
-{{ data['shipData'][0]['pvpThreeInfo']['wins'] }}%
-{{ data['shipData'][0]['pvpThreeInfo']['pr']['value'] }}
-{{ data['shipData'][0]['pvpThreeInfo']['damage'] }}
-{{ '%.2f' | format(data['shipData'][0]['pvpThreeInfo']['frags']) }}
-{{ '%.2f' | format(data['shipData'][0]['pvpThreeInfo']['hit']) }}%
-{% endif %} {% if data['shipData'][0]['rankInfo']['battles'] %}
+{{ data['pvpThreeInfo']['battles'] }}
+{{ data['pvpThreeInfo']['wins'] }}%
+{{ data['pvpThreeInfo']['pr']['value'] }}
+{{ data['pvpThreeInfo']['damage'] }}
+{{ '%.2f' | format(data['pvpThreeInfo']['frags']) }}
+{% endif %} {% if data['rankInfo']['battles'] %}
 æä½
-{{ data['shipData'][0]['rankInfo']['battles'] }}
-{{ data['shipData'][0]['rankInfo']['wins'] }}%
-{{ data['shipData'][0]['rankInfo']['pr']['value'] }}
-{{ data['shipData'][0]['rankInfo']['damage'] }}
-{{ '%.2f' | format(data['shipData'][0]['rankInfo']['frags']) }}
-{{ '%.2f' | format(data['shipData'][0]['rankInfo']['hit']) }}%
+{{ data['rankInfo']['battles'] }}
+{{ data['rankInfo']['wins'] }}%
+{{ data['rankInfo']['pr']['value'] }}
+{{ data['rankInfo']['damage'] }}
+{{ '%.2f' | format(data['rankInfo']['frags']) }}
 {% endif %}
-{% if data['shipData'][0]['pvpInfo']['battles'] %}
-éæºææ°æ®
-{% endif %} {% if data['shipData'][0]['pvpInfo']['battles'] %}
-ç­çº§
-æè°
+æ¯æ¥æç»©
+ç±»å
 åºæ¬¡
-PR
 èç
-åºå
-å»æ
-å½ä¸­
-{% for ship in data['shipData'][0]['shipData'] %} {% if ship['shipInfo']
-['battles'] %}
-{{ ship['shipInfo']['shipInfo']['level'] }}
-{{ ship['shipInfo']['shipInfo']['nameCn'] }}
-{{ ship['shipInfo']['battles'] }}
-{{ ship['shipInfo']['pr']['value'] }}
-{{ ship['shipInfo']['wins'] }}%
-{{ ship['shipInfo']['damage'] }}
-{{ '%.2f' | format(ship['shipInfo']['frags']) }}
-{{ '%.2f' | format(ship['shipInfo']['hit']) }}%
-{% endif %} {% endfor %}
-{% endif %}  {% if data['shipData'][0]['rankInfo']['battles'] %}
-æä½ææ°æ®
-{% endif %} {% if data['shipData'][0]['rankInfo']['battles'] %}
-ç­çº§
-æè°
-åºæ¬¡
 PR
-èç
 åºå
 å»æ
-å½ä¸­
-{% for ship in data['shipData'][0]['shipData'] %} {% if ship['rankSolo']
-['battles'] %}
-{{ ship['rankSolo']['shipInfo']['level'] }}
-{{ ship['rankSolo']['shipInfo']['nameCn'] }}
-{{ ship['rankSolo']['battles'] }}
-{{ ship['rankSolo']['pr']['value'] }}
-{{ ship['rankSolo']['wins'] }}%
-{{ ship['rankSolo']['damage'] }}
-{{ '%.2f' | format(ship['rankSolo']['frags']) }}
-{{ '%.2f' | format(ship['rankSolo']['hit']) }}%
-{% endif %} {% endfor %}
-{% endif %}
+{% for eachShipData in data['shipData'] %} {% if eachShipData['shipInfo']
+['battles'] or eachShipData['rankSolo']['battles'] %}
+{{ time.strftime('%Y-%m-%d',time.localtime(int(abs(eachShipData
+['recordDateTime']/1000)))) }}
+{% for each in eachShipData %} {% for index,value in enumerate(
+['shipSolo','shipTwo','shipThree','rankSolo']) %} {% if each|string == value
+and eachShipData[each]['battles'] %}
+{{ ['åé','èªè¡è½¦','ä¸è½®è½¦','æä½'][index] }}
+{{ eachShipData[each]['battles'] }}
+{{ eachShipData[each]['wins'] }}%
+{{ eachShipData[each]['pr']['value'] }}
+{{ eachShipData[each]['damage'] }}
+{{ '%.2f' | format(eachShipData[each]['frags']) }}
+{% endif %} {% endfor %} {% endfor %} {% endif %} {% endfor %}
 Â©è¥¿è¡å¯ºé¨å­£  Â©æ¬å¿
 https://github.com/benx1n/HikariBot
 QQé¢éæç´¢âyuyukoâå³å¯ä½¿ç¨ç¨³å®çè¾è®¯å®æ¹æºå¨äºº~
 Design By å·ç  H5 Converted By C1ystal
-èµå©é¸£è°¢ï¼ç·äººä»¬çå®è¿å·ãWishingãç§é¿
+èµå©é¸£è°¢ï¼ç§é¿ãç·äººä»¬çå®è¿å·ãæµ·ä¸æéæ´æ¯ä¼ è¯´
```

### Comparing `hikari_core-0.1.5/hikari_core/Template/wws-info.html` & `hikari_core-0.1.6/hikari_core/Template/wws-ship.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,666 +1,580 @@
 <!DOCTYPE html>
 <html>
 	<head>
 		<meta charset="utf-8">
 		<title></title>
+		<link rel="stylesheet" type="text/css" href="wws-ship.css" />
 	</head>
 	<style>
-		
 		* {
-			margin: 0;
 			padding: 0;
+			margin: 0;
 		}
-		
+
 		.main-content {
-			width: 1200px;
-			font-size: 30px;
+			width: 1000px;
+			border-radius: 16px;
 			font-family: "Microsoft YaHei";
-			font-weight: bold;
+			font-size: 30px;
 		}
-		
+
 		.page-box {
-			width: 1200px;
+			width: 1000px;
 			display: flex;
 			flex-direction: column;
 		}
-		
+
 		.page-header {
-			display: flex;
-			flex-direction: column;
-			margin-top: 30px;
+			font-size: 40px;
+			padding: 20px;
 		}
-		
+
 		.clan-user-server {
-			height: 120px;
+			height: 80px;
+			line-height: 80px;
+			font-weight: bold;
 			text-align: center;
-			font-size: 45px;
-			line-height: 120px;
 		}
-		
+
 		.clan {
 			display: inline-block;
+			height: 80px;
 			padding-right: 10px;
-			height: 120px;
 		}
-		
-		.user {
+
+		.server {
 			display: inline-block;
-			height: 120px;
+			height: 80px;
+			padding-left: 20px;
 		}
-		
-		.server {
+
+		.username {
 			display: inline-block;
-			padding-left: 10px;
+			height: 80px;
 		}
-		
+
 		.server-border {
-			width: 200px;
-			height: 50px;
-			line-height: 50px;
+			width: 160px;
+			height: 40px;
+			margin-top: 20px;
+			line-height: 40px;
 			text-align: center;
 			background-color: #F2F2F2;
-			border-radius: 25px;
-			font-size: 35px;
+			border-radius: 20px;
+			font-size: 30px;
 		}
-		
-		.image-box {
-			width: 100px;
-			height: 100px;
-			position: fixed;
-			left: 50px;
-			top: 40px;
-		}
-		
-		.image-box img {
-			width: 100px;
-			height: 100px;
-			border-radius: 50px;
+
+		.ship-detail {
+			display: flex;
+			height: 60px;
+			line-height: 60px;
+			font-weight: bold;
+		}
+
+
+		.ship-level {
+			flex: 1;
+			text-align: right;
+			padding-right: 60px;
+		}
+
+		.ship-name {
+			display: inline-block;
+			height: 60px;
+		}
+
+		.ship-icon {
+			flex: 1;
+			padding-left: 70px;
+		}
+
+		.ship-icon img {
+			width: 60px;
+			height: 60px;
+		}
+
+
+		.ranking {
+			display: flex;
+			justify-content: space-around;
+			align-content: space-around;
+			height: 60px;
+			line-height: 40px;
+			font-weight: bold;
+			margin-bottom: 15px;
+		}
+
+		.ranking_border {
+			margin-top: 10px;
+			height: 40px;
+			border-radius: 28px;
+			padding: 4px 20px;
+			background-color: #F2F2F2;
 		}
-		
+
+		.last-time {
+			height: 60px;
+			line-height: 60px;
+			text-align: center;
+			color: #606266;
+		}
+
 		.pr {
 			display: flex;
-			height: 100px;
+			height: 120px;
 			font-weight: bold;
 			line-height: 60px;
-			padding: 0 80px;
+			padding: 0 60px;
+			margin-top: 20px;
 		}
-		
+
 		.pr-bar-bg {
 			position: relative;
 			flex: 1;
 			line-height: 80px;
 			background-color: #A6A6A6;
 			height: 80px;
 			border-radius: 40px;
 			margin-top: 10px;
 			text-align: center;
 			color: #FFFFFF;
 		}
-		
+
 		.pr-bar {
 			position: absolute;
 			top: 0;
 			left: 0;
 			height: 80px;
 			z-index: 1;
 			border-radius: 40px;
 		}
-		
+
 		.pr-number {
 			z-index: 99;
 			position: absolute;
 			left: 0px;
 			right: 0px;
 			font-size: 35px;
 			font-weight: bold;
 		}
-		
-		.recnet-time {
-			text-align: center;
-			font-weight: normal;
-		}
-		
-		.overview-change {
-			display: flex;
-			margin-top: 30px;
-			padding: 0 50px;
-			height: 300px;
-		}
-		
-		.overview-change-item {
-			flex: 1;
+
+		.data-change {
+			margin: 10px 60px;
+			height: 120px;
 			display: flex;
 			flex-direction: column;
-			margin: 0 20px;
-		
-		}
-		
-		.item-top {
-			flex: 5;
-			background-color: #F2F2F2;
-			border-radius: 16px;
-		}
-		
-		.item-bottom {
-			display: flex;
-			flex: 4;
-			margin-top: 20px;
-		}
-		
-		.left-item-bottom {
 			background-color: #F2F2F2;
-			border-radius: 16px;
+			border-radius: 15px;
+			font-weight: bold;
 		}
-		
-		.bottom-mini-item-left {
+
+		.change-header {
 			flex: 1;
-			margin-right: 10px;
-			background-color: #F2F2F2;
-			border-radius: 16px;
+			display: flex;
+			background-color: #D9D9D9;
+			border-radius: 15px;
+			color: #606266;
 		}
-		
-		.bottom-mini-item-right {
+
+		.change-body {
 			flex: 1;
-			margin-left: 10px;
-			background-color: #F2F2F2;
-			border-radius: 16px;
-		}
-		
-		.item-top {
 			display: flex;
-			flex-direction: column;
 		}
-		
-		.item-top div {
-			height: 80px;
+
+		.change-header-item,
+		.change-body-item {
+			flex: 1;
 			text-align: center;
-			font-size: 40px;
-		}
-		
-		.item-top-top {
-			color: #606266;
-			font-weight: normal;
-			line-height: 100px;
-		}
-		
-		.item-top-bottom {
 			line-height: 60px;
 		}
-		
-		.left-item-bottom {
+
+		.ship-overview {
+			margin: 10px 50px;
+			height: 420px;
 			display: flex;
 			flex-direction: column;
 		}
-		
-		.change-pr-title {
-			color: #606266;
-			height: 60px;
-			display: flex;
-			font-weight: normal;
-			line-height: 70px;
-		}
-		
-		.change-pr {
-			height: 60px;
-			line-height: 50px;
-			text-align: center;
-			font-size: 30px;
-		}
-		
-		.change-pr-title-left {
+
+		.overview-col {
 			flex: 1;
-			font-size: 35px;
-			text-align: right;
-			margin-right: 30px;
+			display: flex;
 		}
-		
-		.change-pr-title-right {
+
+		.overview-item {
 			flex: 1;
-			font-size: 20px;
-		}
-		
-		.bottom-mini-item-left,
-		.bottom-mini-item-right {
+			background-color: #F2F2F2;
+			border-radius: 15px;
+			margin: 10px;
 			display: flex;
 			flex-direction: column;
+			font-size: 40px;
+			font-weight: bold;
 		}
-		
-		.mini-item-top {
+
+		.overview-item-title {
+			height: 95px;
+			line-height: 125px;
+			text-align: center;
 			color: #606266;
-			font-weight: normal;
-			line-height: 70px;
 		}
-		
-		.mini-item-bottom {
-			line-height: 45px;
-			font-size: 27px;
-		}
-		
-		.bottom-mini-item-left div,
-		.bottom-mini-item-right div {
-			height: 60px;
+
+		.overview-item-data {
+			height: 95px;
+			line-height: 65px;
 			text-align: center;
 		}
-		
-		.information-header,
-		.ship-data-header {
-			margin: 0 200px;
-			margin-top: 30px;
+
+
+
+
+		.information-header {
+			width: 680px;
+			margin: 20px 160px;
 			height: 60px;
 			line-height: 60px;
-			border-radius: 16px;
-			background-color: #D9D9D9;
+			font-weight: bold;
 			text-align: center;
+			background-color: #BFBFBF;
+			border-radius: 15px;
 		}
-		
-		.information-body,
-		.ship-data-body {
-			margin: 0 80px;
+
+		.information-body {
+			width: 880px;
+			margin: 0 60px;
 			margin-top: 30px;
 			display: flex;
 			flex-direction: column;
+			font-weight: bold;
 			background-color: #F2F2F2;
-			border-radius: 16px;
+			border-radius: 15px;
 		}
-		
-		.information-col,
-		.ship-data-col {
-			height: 60px;
+
+		.information-body-top {
 			display: flex;
-			line-height: 60px;
+			background-color: #D9D9D9;
+			border-radius: 8px;
+			color: #606266;
 		}
-		
-		.information-col-item,
-		.ship-data-col-item {
+
+		.information-item {
+			height: 60px;
+			line-height: 60px;
 			flex: 1;
 			text-align: center;
 		}
-		
-		.information-table-header,
-		.ship-data-table-header {
-			color: #606266;
+
+		.information-body-data {
+			display: flex;
+			border-radius: 8px;
 		}
-		
-		.information-type,
-		.ship-data-type {
-			color: #909399;
+
+		.ship-highest-header {
+			height: 60px;
+			line-height: 60px;
+			width: 680px;
+			margin: 40px 160px 20px 160px;
+			font-weight: bold;
+			text-align: center;
+			background-color: #BFBFBF;
+			border-radius: 15px;
 		}
-		
-		.chart-box {
-			margin: 0 80px;
-			margin-top: 30px;
+
+		.ship-highest-data {
+			width: 900px;
+			margin: 20px 50px;
+			display: flex;
+			flex-direction: column;
+		}
+
+		.high-col {
+			display: flex;
+			justify-content: space-around;
+		}
+
+		.high-item {
+			flex: 1;
+			height: 120px;
+			line-height: 100px;
 			background-color: #F2F2F2;
-			height: 400px;
+			border-radius: 8px;
 			display: flex;
-			border-radius: 16px;
+			flex-direction: column;
+			margin: 10px;
+		}
+
+		.high-item-top {
+			height: 60px;
+			line-height: 70px;
+			font-weight: bold;
+			color: #606266;
+			text-align: center;
 		}
-		
-		.chart-bar {
-			flex: 6;
-		}
-		
-		.chart-pie {
-			flex: 4;
+
+		.high-item-bottom {
+			height: 60px;
+			line-height: 50px;
+			font-weight: bold;
+			text-align: center;
 		}
-		
+
 		.footer {
-			margin-top: 30px;
 			text-align: center;
 			font-weight: bold;
 			font-size: 24px;
 			color: #909399;
 			margin-bottom: 20px;
 		}
 	</style>
 	<body>
 		<div class="main-content">
 			<div class="page-box">
 				<div class="page-header">
 
-<!-- 					<div class="image-box">
-						<img src="IMG_20220607_224103.jpg" />
-					</div> -->
-
-					<div class="clan-user-server">
-						{% if data['clanInfo']['tag'] %}
-						<div class="clan" style="color: {{ data['clanInfo']['colorRgb'] }};">[{{ data['clanInfo']['tag'] }}]</div>
+						<div class="clan-user-server">
+					 	{% if data['clanInfo']['tag'] %}
+							<div class="clan" style="color: {{ data['clanInfo']['colorRgb'] }};">
+								[{{ data['clanInfo']['tag'] }}]</div>
 						{% endif %}
-						<div class="user">{{ data['userName'] }}</div>
-						<div class="server">
-							<div class="server-border">
-								{{ data['serverName'] }}
+							<div class="username">{{ data['userName'] }}</div>
+							<div class="server">
+								<!-- 动态设置服务器字体颜色 -->
+								<div class="server-border">{{ data['serverName'] }}</div>
 							</div>
 						</div>
+
+						<div class="ship-detail">
+							{% if data['shipInfo']['shipInfo']['nameCn'] %}
+							<div class="ship-level">{{ data['shipInfo']['shipInfo']['level'] }}</div>
+							{% else %}
+							<div class="ship-level">{{ data['rankSolo']['shipInfo']['level'] }}</div>
+							{% endif %}
+
+							{% if data['shipInfo']['shipInfo']['nameCn'] %}
+							<div class="ship-name">{{ data['shipInfo']['shipInfo']['nameCn'] }}</div>
+							{% else %}
+							<div class="ship-name">{{ data['rankSolo']['shipInfo']['nameCn'] }}</div>
+							{% endif %}
+							<div class="ship-icon"><img
+									src={% if data['shipInfo']['shipInfo']['shipType'] == 'Destroyer' or data['rankSolo']['shipInfo']['shipType'] == 'Destroyer' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_destroyer.png"
+									{% elif data['shipInfo']['shipInfo']['shipType'] == 'Cruiser' or data['rankSolo']['shipInfo']['shipType'] == 'Cruiser' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_cruiser.png"
+									{% elif data['shipInfo']['shipInfo']['shipType'] == 'Battleship' or data['rankSolo']['shipInfo']['shipType'] == 'Battleship' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_battleship.png"
+									{% elif data['shipInfo']['shipInfo']['shipType'] == 'AirCarrier' or data['rankSolo']['shipInfo']['shipType'] == 'AirCarrier' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_aircarrier.png"
+									{% else %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_submarine.png"
+									{% endif %} /></div>
+						</div>
 					</div>
 
 					<div class="pr">
 						<!-- 动态设置长度及颜色，填写PR即可 -->
 						<div class="pr-bar-bg">
-							<span class="pr-number">{{ data['pr']['value'] }}&nbsp;&nbsp;&nbsp;&nbsp;<span class="pr-text"></span></span>
+							{% if data['shipInfo']['pr']['color'] and data['shipInfo']['pr']['color'] != '#828282' %}
+							<span class="pr-number">{{ data['shipInfo']['pr']['value'] }} &nbsp;&nbsp;&nbsp;&nbsp;<span
+									class="pr-text"></span></span>
+							{% else %}
+							<span class="pr-number">{{ data['rankSolo']['pr']['value'] }} &nbsp;&nbsp;&nbsp;&nbsp;<span
+									class="pr-text"></span></span>
+							{% endif %}
 							<div class="pr-bar"></div>
 						</div>
 					</div>
-
-					<div class="recnet-time">
-						<span>最后战斗时间：</span><span>{{ time.strftime('%Y-%m-%d %H:%M:%S',time.localtime(abs(data['lastDateTime']))) }}</span>
-					</div>
-
-					<div class="overview-change">
-						<div class="overview-change-item left-item">
-							<div class="left-item-top item-top">
-								<div class="overview-count-title item-top-top">场次</div>
-								<div class="overview-count item-top-bottom">{{ data['pvp']['battles'] }}</div>
-							</div>
-							<div class="left-item-bottom item-bottom">
-								<div class="change-pr-title">
-									<div class="change-pr-title-left">PR</div>
-									<div class="change-pr-title-right">较上次</div>
-								</div>
-								<div class="change-pr">{{ '%+d' | format(data['dwpDataVO']['pr']) }}</div>
-							</div>
-						</div>
-						<div class="overview-change-item mid-item">
-							<div class="mid-item-top item-top">
-								<div class="overview-win-title item-top-top">胜率</div>
-								<div class="overview-win item-top-bottom" style="color: {{ data['pvp']['winsData']['color'] }}">{{ data['pvp']['wins'] }}%</div>
-							</div>
-							<div class="mid-item-bottom item-bottom">
-								<div class="change-avgdmg-box bottom-mini-item-left">
-									<div class="mini-item-top">场均</div>
-									<div class="mini-item-bottom change-avgdmg">{{ '%+d' | format(data['dwpDataVO']['damage']) }}</div>
-								</div>
-								<div class="change-win-box bottom-mini-item-right">
-									<div class="mini-item-top">胜率</div>
-									<div class="mini-item-bottom change-win">{{ '%+.2f' | format(data['dwpDataVO']['wins']) }}%</div>
-								</div>
-							</div>
-						</div>
-						<div class="overview-change-item right-item">
-							<div class="right-item-top item-top">
-								<div class="overview-avgdmg-title item-top-top">场均</div>
-								<div class="overview-avgdmg item-top-bottom" style="color: {{ data['pvp']['damageData']['color'] }};">{{ data['pvp']['damage'] }}</div>
-							</div>
-							<div class="right-item-bottom item-bottom">
-								<div class="overview-kd-box bottom-mini-item-left">
-									<div class="mini-item-top">击杀</div>
-									<div class="mini-item-bottom">{{ '%.2f' | format(data['pvp']['frags']) }}</div>
-								</div>
-								<div class="overview-hit-box bottom-mini-item-right">
-									<div class="mini-item-top">命中</div>
-									<div class="mini-item-bottom">{{ '%.2f' | format(data['pvp']['hit']) }}%</div>
-								</div>
-							</div>
-						</div>
+					
+					<div class="last-time">
+						<span>最后战斗时间：</span><span>{{ time.strftime('%Y-%m-%d %H:%M:%S',time.localtime(abs(data['shipInfo']['lastBattlesTime']))) }}</span>
 					</div>
-
-					<div class="ship-data-header">船只数据</div>
 					
-					<div class="ship-data-body">
-						<div class="ship-data-col ship-data-table-header">
-							<div class="ship-data-col-item">类型</div>
-							<div class="ship-data-col-item">场次</div>
-							<div class="ship-data-col-item">胜率</div>
-							<div class="ship-data-col-item">PR</div>
-							<div class="ship-data-col-item">场均</div>
-							<div class="ship-data-col-item">命中</div>
-						</div>
-						
-						{% if  data['type']['Battleship']['battles']  %}
-						<div class="ship-data-col">
-							<div class="ship-data-col-item ship-data-type">战列舰</div>
-							<div class="ship-data-col-item">{{ data['type']['Battleship']['battles'] }}</div>
-							<div class="ship-data-col-item" style="color: {{ data['type']['Battleship']['winsData']['color'] }};">{{ data['type']['Battleship']['wins'] }}%</div>
-							<div class="ship-data-col-item" style="color: {{ data['type']['Battleship']['pr']['color'] }};">{{ data['type']['Battleship']['pr']['value'] }}</div>
-							<div class="ship-data-col-item" style="color: {{ data['type']['Battleship']['damageData']['color'] }};">{{ data['type']['Battleship']['damage'] }}</div>
-							<div class="ship-data-col-item">{{ '%.2f' | format (data['type']['Battleship']['hit']) }}%</div>
+					{% if data['shipRank'] %}
+					<div class="ranking">
+						<div class="ranking_border"><span
+								style="color: #606266;">排名</span>&nbsp;&nbsp;<span>{{data['shipRank']}}</span>
 						</div>
-						{% endif %}
-
-						{% if data['type']['Cruiser']['battles'] %}
-						<div class="ship-data-col">
-							<div class="ship-data-col-item ship-data-type">巡洋舰</div>
-							<div class="ship-data-col-item">{{ data['type']['Cruiser']['battles'] }}</div>
-							<div class="ship-data-col-item" style="color: {{ data['type']['Cruiser']['winsData']['color'] }};">{{ data['type']['Cruiser']['wins'] }}%</div>
-							<div class="ship-data-col-item" style="color: {{ data['type']['Cruiser']['pr']['color'] }};">{{ data['type']['Cruiser']['pr']['value'] }}</div>
-							<div class="ship-data-col-item" style="color: {{ data['type']['Cruiser']['damageData']['color'] }};">{{ data['type']['Cruiser']['damage'] }}</div>
-							<div class="ship-data-col-item">{{ '%.2f' | format (data['type']['Cruiser']['hit']) }}%</div>
+					</div>
+					{% endif %}
+					{% if data['rank'] != -1 %}
+					<div class="ranking">
+						<div class="ranking_border"><span
+								style="color: #606266;">排名</span>&nbsp;&nbsp;<span>{{data['rank']}}</span>
 						</div>
-						{% endif %}
-
+					</div>
+					{% endif %}
 
-						{% if data['type']['Destroyer']['battles'] %}
-						<div class="ship-data-col">
-							<div class="ship-data-col-item ship-data-type">驱逐舰</div>
-							<div class="ship-data-col-item">{{ data['type']['Destroyer']['battles'] }}</div>
-							<div class="ship-data-col-item" style="color: {{ data['type']['Destroyer']['winsData']['color'] }};">{{ data['type']['Destroyer']['wins'] }}%</div>
-							<div class="ship-data-col-item" style="color: {{ data['type']['Destroyer']['pr']['color'] }};">{{ data['type']['Destroyer']['pr']['value'] }}</div>
-							<div class="ship-data-col-item" style="color: {{ data['type']['Destroyer']['damageData']['color'] }};">{{ data['type']['Destroyer']['damage'] }}</div>
-							<div class="ship-data-col-item">{{ '%.2f' | format (data['type']['Destroyer']['hit']) }}%</div>
+					<div class="data-change">
+						<div class="change-header">
+							<div class="change-header-item">场均</div>
+							<div class="change-header-item">胜率</div>
+							<div class="change-header-item">PR</div>
+						</div>
+						<div class="change-body">
+							<div class="change-body-item change-avgdmg">
+								{{ '%+d' | format(data['dwpDataVO']['damage']) }}</div>
+							<div class="change-body-item change-win">{{ '%+.2f' | format(data['dwpDataVO']['wins']) }}
+							</div>
+							<div class="change-body-item change-pr">{{ '%+d' | format(data['dwpDataVO']['pr']) }}</div>
 						</div>
-						{% endif %}
+					</div>
 
-						{% if data['type']['AirCarrier']['battles'] %}
-						<div class="ship-data-col">
-							<div class="ship-data-col-item ship-data-type">航空母舰</div>
-							<div class="ship-data-col-item">{{ data['type']['AirCarrier']['battles'] }}</div>
-							<div class="ship-data-col-item" style="color: {{ data['type']['AirCarrier']['winsData']['color'] }};">{{ data['type']['AirCarrier']['wins'] }}%</div>
-							<div class="ship-data-col-item" style="color: {{ data['type']['AirCarrier']['pr']['color'] }};">{{ data['type']['AirCarrier']['pr']['value'] }}</div>
-							<div class="ship-data-col-item" style="color: {{ data['type']['AirCarrier']['damageData']['color'] }};">{{ data['type']['AirCarrier']['damage'] }}</div>
-							<div class="ship-data-col-item">{{ '%.2f' | format (data['type']['AirCarrier']['hit']) }}%</div>
+					<div class="ship-overview">
+						<div class="overview-col">
+							<div class="overview-item">
+								<div class="overview-item-title">场次</div>
+								<div class="overview-item-data">{{ data['shipInfo']['battles'] }}</div>
+							</div>
+							<div class="overview-item">
+								<div class="overview-item-title">胜率</div>
+								<div class="overview-item-data"
+									style="color: {{ data['shipInfo']['winsData']['color'] }};">
+									{{ data['shipInfo']['wins'] }}%</div>
+							</div>
+							<div class="overview-item">
+								<div class="overview-item-title">场均</div>
+								<div class="overview-item-data"
+									style="color: {{ data['shipInfo']['damageData']['color'] }};">
+									{{ data['shipInfo']['damage'] }}</div>
+							</div>
 						</div>
-						{% endif %}
-						
-						{% if data['type']['Submarine']['battles'] %}
-						<div class="ship-data-col">
-							<div class="ship-data-col-item ship-data-type">潜艇</div>
-							<div class="ship-data-col-item">{{ data['type']['Submarine']['battles'] }}</div>
-							<div class="ship-data-col-item" style="color: {{ data['type']['Submarine']['winsData']['color'] }};">{{ data['type']['Submarine']['wins'] }}%</div>
-							<div class="ship-data-col-item" style="color: {{ data['type']['Submarine']['pr']['color'] }};">{{ data['type']['Submarine']['pr']['value'] }}</div>
-							<div class="ship-data-col-item" style="color: {{ data['type']['Submarine']['damageData']['color'] }};">{{ data['type']['Submarine']['damage'] }}</div>
-							<div class="ship-data-col-item">{{ '%.2f' | format (data['type']['Submarine']['hit']) }}%</div>
+						<div class="overview-col">
+							<div class="overview-item">
+								<div class="overview-item-title">经验</div>
+								<div class="overview-item-data">{{ data['shipInfo']['xp'] }}</div>
+							</div>
+							<div class="overview-item">
+								<div class="overview-item-title">击杀</div>
+								<div class="overview-item-data">{{ '%.2f' | format(data['shipInfo']['frags']) }}</div>
+							</div>
+							<div class="overview-item">
+								<div class="overview-item-title">命中</div>
+								<div class="overview-item-data">{{ data['shipInfo']['hit'] }}%</div>
+							</div>
 						</div>
-						{% endif %}
-
 					</div>
 
-					<div class="information-header">总体战绩</div>
+					<div class="information-header">
+						总体战绩
+					</div>
 
 					<div class="information-body">
-						<div class="information-col information-table-header">
-							<div class="information-col-item">类型</div>
-							<div class="information-col-item">场次</div>
-							<div class="information-col-item">胜率</div>
-							<div class="information-col-item">PR</div>
-							<div class="information-col-item">场均</div>
-							<div class="information-col-item">击杀</div>
-						</div>
-						
-						{% if data['pvpSolo']['battles'] %}
-						<div class="information-col">
-							<div class="information-col-item information-type">单野</div>
-							<div class="information-col-item">{{ data['pvpSolo']['battles'] }}</div>
-							<div class="information-col-item" style="color: {{ data['pvpSolo']['winsData']['color'] }};">{{ data['pvpSolo']['wins'] }}%</div>
-							<div class="information-col-item" style="color: {{ data['pvpSolo']['pr']['color'] }};">{{ data['pvpSolo']['pr']['value'] }}</div>
-							<div class="information-col-item" style="color: {{ data['pvpSolo']['damageData']['color'] }};">{{ data['pvpSolo']['damage'] }}</div>
-							<div class="information-col-item">{{ '%.2f' | format(data['pvpSolo']['frags']) }}</div>
+						<div class="information-body-top">
+							<div class="information-item">类型</div>
+							<div class="information-item">场次</div>
+							<div class="information-item">胜率</div>
+							<div class="information-item">PR</div>
+							<div class="information-item">场均</div>
+							<div class="information-item">击杀</div>
+						</div>
+
+						{% if data['shipSolo']['battles'] %}
+						<div class="information-body-data">
+							<div class="information-item" style="color: #909399;">单野</div>
+							<div class="information-item">{{ data['shipSolo']['battles'] }}</div>
+							<div class="information-item" style="color: {{ data['shipSolo']['winsData']['color'] }};">
+								{{ data['shipSolo']['wins'] }}%</div>
+							<div class="information-item" style="color: {{ data['shipSolo']['pr']['color'] }};">
+								{{ data['shipSolo']['pr']['value'] }}</div>
+							<div class="information-item"
+								style="color: {{ data['shipSolo']['damageData']['color'] }};">
+								{{ data['shipSolo']['damage'] }}</div>
+							<div class="information-item">{{ '%.2f' | format(data['shipSolo']['frags']) }}</div>
 						</div>
 						{% endif %}
-
-						{% if data['pvpTwo']['battles'], %}
-						<div class="information-col">
-							<div class="information-col-item information-type">自行车</div>
-							<div class="information-col-item">{{ data['pvpTwo']['battles'] }}</div>
-							<div class="information-col-item" style="color: {{ data['pvpTwo']['winsData']['color'] }};">{{ data['pvpTwo']['wins'] }}%</div>
-							<div class="information-col-item" style="color: {{ data['pvpTwo']['pr']['color'] }};">{{ data['pvpTwo']['pr']['value'] }}</div>
-							<div class="information-col-item" style="color: {{ data['pvpTwo']['damageData']['color'] }};">{{ data['pvpTwo']['damage'] }}</div>
-							<div class="information-col-item">{{ '%.2f' | format(data['pvpTwo']['frags']) }}</div>
+						{% if data['shipTwo']['battles'] %}
+						<div class="information-body-data">
+							<div class="information-item" style="color: #909399;">自行车</div>
+							<div class="information-item">{{ data['shipTwo']['battles'] }}</div>
+							<div class="information-item" style="color: {{ data['shipTwo']['winsData']['color'] }};">
+								{{ data['shipTwo']['wins'] }}%</div>
+							<div class="information-item" style="color: {{ data['shipTwo']['pr']['color'] }};">
+								{{ data['shipTwo']['pr']['value'] }}</div>
+							<div class="information-item"
+								style="color: {{ data['shipTwo']['damageData']['color'] }};">
+								{{ data['shipTwo']['damage'] }}</div>
+							<div class="information-item">{{ '%.2f' | format(data['shipTwo']['frags']) }}</div>
 						</div>
 						{% endif %}
-
-						{% if data['pvpThree']['battles'] %}
-						<div class="information-col">
-							<div class="information-col-item information-type">三轮车</div>
-							<div class="information-col-item">{{ data['pvpThree']['battles'] }}</div>
-							<div class="information-col-item" style="color: {{ data['pvpThree']['winsData']['color'] }};">{{ data['pvpThree']['wins'] }}%</div>
-							<div class="information-col-item" style="color: {{ data['pvpThree']['pr']['color'] }};">{{ data['pvpThree']['pr']['value'] }}</div>
-							<div class="information-col-item" style="color: {{ data['pvpThree']['damageData']['color'] }};">{{ data['pvpThree']['damage'] }}</div>
-							<div class="information-col-item">{{ '%.2f' | format(data['pvpThree']['frags']) }}</div>
+						{% if data['shipThree']['battles'] %}
+						<div class="information-body-data">
+							<div class="information-item" style="color: #909399;">三轮车</div>
+							<div class="information-item">{{ data['shipThree']['battles'] }}</div>
+							<div class="information-item" style="color: {{ data['shipThree']['winsData']['color'] }};">
+								{{ data['shipThree']['wins'] }}%</div>
+							<div class="information-item" style="color: {{ data['shipThree']['pr']['color'] }};">
+								{{ data['shipThree']['pr']['value'] }}</div>
+							<div class="information-item"
+								style="color: {{ data['shipThree']['damageData']['color'] }};">
+								{{ data['shipThree']['damage'] }}</div>
+							<div class="information-item">{{ '%.2f' | format(data['shipThree']['frags']) }}</div>
 						</div>
 						{% endif %}
-
 						{% if data['rankSolo']['battles'] %}
-						<div class="information-col">
-							<div class="information-col-item information-type">排位</div>
-							<div class="information-col-item">{{ data['rankSolo']['battles'] }}</div>
-							<div class="information-col-item" style="color: {{ data['rankSolo']['winsData']['color'] }};">{{ data['rankSolo']['wins'] }}%</div>
-							<div class="information-col-item" style="color: {{ data['rankSolo']['pr']['color'] }};">{{ data['rankSolo']['pr']['value'] }}</div>
-							<div class="information-col-item" style="color: {{ data['rankSolo']['damageData']['color'] }};">{{ data['rankSolo']['damage'] }}</div>
-							<div class="information-col-item">{{ '%.2f' | format(data['rankSolo']['frags']) }}</div>
+						<div class="information-body-data">
+							<div class="information-item" style="color: #909399;">排位</div>
+							<div class="information-item">{{ data['rankSolo']['battles'] }}</div>
+							<div class="information-item" style="color: {{ data['rankSolo']['winsData']['color'] }};">
+								{{ data['rankSolo']['wins'] }}%</div>
+							<div class="information-item" style="color: {{ data['rankSolo']['pr']['color'] }};">
+								{{ data['rankSolo']['pr']['value'] }}</div>
+							<div class="information-item"
+								style="color: {{ data['rankSolo']['damageData']['color'] }};">
+								{{ data['rankSolo']['damage'] }}</div>
+							<div class="information-item">{{ '%.2f' | format(data['rankSolo']['frags']) }}</div>
 						</div>
 						{% endif %}
-						
 					</div>
 
-					<div class="chart-box">
-						<div class="chart-bar"></div>
-						<div class="chart-pie"></div>
+					<div class="ship-highest-header">
+						最高纪录
+					</div>
+
+					<div class="ship-highest-data">
+						<div class="high-col">
+							<div class="high-item">
+								<div class="high-item-top">最高伤害</div>
+								<div class="high-item-bottom">{{ data['shipInfo']['extensionDataInfo']['maxDamage'] }}
+								</div>
+							</div>
+							<div class="high-item">
+								<div class="high-item-top">侦察伤害</div>
+								<div class="high-item-bottom">
+									{{ data['shipInfo']['extensionDataInfo']['maxDamageScouting'] }}</div>
+							</div>
+							<div class="high-item">
+								<div class="high-item-top">最高潜在</div>
+								<div class="high-item-bottom">
+									{{ data['shipInfo']['extensionDataInfo']['maxTotalAgro'] }}</div>
+							</div>
+						</div>
+						<div class="high-col">
+							<div class="high-item">
+								<div class="high-item-top">经验</div>
+								<div class="high-item-bottom">{{ data['shipInfo']['extensionDataInfo']['maxXp'] }}</div>
+							</div>
+							<div class="high-item">
+								<div class="high-item-top">击杀</div>
+								<div class="high-item-bottom">{{ data['shipInfo']['extensionDataInfo']['maxFrags'] }}
+								</div>
+							</div>
+							<div class="high-item">
+								<div class="high-item-top">飞机击落</div>
+								<div class="high-item-bottom">
+									{{ data['shipInfo']['extensionDataInfo']['maxPlanesKilled'] }}</div>
+							</div>
+						</div>
 					</div>
 
 					<div class="footer">
-						<p>©西行寺雨季&nbsp;&nbsp;©本心</p>
+						<p>© 西行寺雨季&nbsp;&nbsp;© 本心</p>
 						<p>https://github.com/benx1n/HikariBot</p>
 						<p>QQ频道搜索”yuyuko”即可使用稳定的腾讯官方机器人~</p>
 						<p>Design By 冷眠 H5 Converted By C1ystal</p>
-						<p>赞助鸣谢：男人们的定远号、Wishing、科长</p>
+						<p>赞助鸣谢：科长、男人们的定远号、海上最速暴毙传说</p>
 					</div>
-
 				</div>
 			</div>
-		</div>
 	</body>
-	{% if template_path and template_path/"echarts.js" %}
-	<script src="file:\\{{template_path}}/echarts.js"></script>
-	{% else %}
-	<script src="https://cdn.jsdelivr.net/npm/echarts@5.3.3/dist/echarts.js"></script>
-	{% endif %}
-	<script>
-		window.onload = function () {
-		    drawBarChart();
-			drawPieChart();
-		};
-		
-		function drawBarChart() {
-			var barChart = echarts.init(document.querySelector('.chart-bar'));
-			var barOption = {
-				animation: false,
-				tooltip: {},
-				label: {
-					position: 'top',
-					show: true,
-					fontSize: '15',
-					color: '#303133',
-				},
-				xAxis: {
-					data: ['I', 'II', 'III', 'IV', 'V', 'VI', 'VII', 'VIII', 'IX', 'X', '★'],
-					axisLabel: {
-						align: 'center',
-						fontSize: '20',
-					}
-				},
-				yAxis: {
-					axisLabel: {
-						align: 'center',
-						fontSize: '20',
-					}
-				},
-				series: [{
-					name: '场次',
-					type: 'bar',
-					data: [
-						{{ data['battleCountAll']['1'] }},
-						{{ data['battleCountAll']['2'] }},
-						{{ data['battleCountAll']['3'] }},
-						{{ data['battleCountAll']['4'] }},
-						{{ data['battleCountAll']['5'] }},
-						{{ data['battleCountAll']['6'] }},
-						{{ data['battleCountAll']['7'] }},
-						{{ data['battleCountAll']['8'] }},
-						{{ data['battleCountAll']['9'] }},
-						{{ data['battleCountAll']['10'] }},
-						{{ data['battleCountAll']['11'] }},
-					],
-					itemStyle: {
-						color: '#D6ECFB40',
-					    borderWidth: 1,
-					    borderType: 'solid',
-					    borderColor: '#9FB8FF',
-					    shadowColor: '#9FB8FF',
-					    shadowBlur: 3
-					},
-				}]
-			};
-	
-			barChart.setOption(barOption);
-		}
-		
-		function drawPieChart() {
-			var pieChart = echarts.init(document.querySelector('.chart-pie'));
-			var pieOption = {
-				animation: false,
-				tooltip: {},
-				color: ["#FBE5D6", "#E2F0D9", "#F2E2E2", "#DAE3F3", "#D9FFFF"],
-				series: [
-			    {
-			        name: this.title,
-			        type: 'pie',
-			        selectedMode: 'single',
-			        radius: ['30%', '80%'],
-			        clockwise: false,
-			        itemStyle: {
-			            borderWidth: 5,
-			            borderColor: '#F2F2F2'
-			        },
-			        label: {
-			            position: 'inside',
-			            formatter: '{b}\n{d}%',
-			            fontSize: 20,
-			            fontWeight: 'bold',
-			        },
-			        data: [
-			            { value: {{ data['type']['Battleship']['battles'] }}, name: 'BB' },
-			            { value: {{ data['type']['Cruiser']['battles'] }}, name: 'CA' },
-			            { value: {{ data['type']['Destroyer']['battles'] }}, name: 'DD' },
-			            { value: {{ data['type']['AirCarrier']['battles'] }}, name: 'CV' },
-			            { value: {{ data['type']['Submarine']['battles'] }}, name: 'SS' }
-			        ]
-			    }],
-				graphic: {
-			    elements: [{
-			        type: 'text', 
-			        left: 'center',
-			        top: 'center',
-			        style: {
-			            text: '舰船\n场次',
-			            fontSize: 35, 
-			            textAlign: 'center', 
-			            width: 30,
-			            height: 30,
-			            fill: 'darkgray'
-			        }
-			    }]
-			}
-			};
-				
-			pieChart.setOption(pieOption);
-		}
-	</script>
-	
 	<script>
-		// PR条颜色动态变化
+		// 胜率条颜色动态变化
 		let bar_bg_width = document.querySelector('.pr-bar-bg').clientWidth;
 		let pr_number = document.querySelector('.pr-number').innerText;
 		pr_number = parseInt(pr_number);
 		if (pr_number == 0) {
 			document.querySelector(".pr-bar").style.backgroundColor = "#828282";
 			document.querySelector(".pr-text").innerText = "暂无数据";
 		} else if (pr_number < 750) {
@@ -690,15 +604,15 @@
 			document.querySelector(".pr-text").innerText = "神佬水平";
 			pr_number = 2450; //防止pr条溢出
 		}
 
 		if (pr_number < 220 && pr_number > 0) {
 			pr_number = 220; //防止pr过低导致圆角异常
 		}
-		// PR条动态长度
+		// 胜率条动态长度
 		let width = bar_bg_width * (pr_number / 2450);
 		document.querySelector('.pr-bar').style.width = width + "px";
 	</script>
 
 	<script>
 		// 服务器字体颜色自动填充
 		let server_name = document.querySelector(".server").innerText;
@@ -743,32 +657,15 @@
 			document.querySelector(".change-pr").style.color = "#70AD47";
 		} else {
 			document.querySelector(".change-pr").style.color = "#FF0000";
 		}
 	</script>
 
 	<script>
-		let arr_ship_data = document.getElementsByClassName('ship-data-col');
-		for (let i = 0; i < arr_ship_data.length; i++) {
-			if (i % 2 != 0 && i == (arr_ship_data.length - 1)) {
-				arr_ship_data[i].style.backgroundColor = "#E4E4E4";
-				arr_ship_data[i].style.borderBottomLeftRadius = "16px";
-				arr_ship_data[i].style.borderBottomRightRadius = "16px";
-			} else if (i % 2 != 0) {
-				arr_ship_data[i].style.backgroundColor = "#E4E4E4";
-			}
-		}
-	</script>
-
-	<script>
-		let arr_information = document.getElementsByClassName('information-col');
-		for (let i = 0; i < arr_information.length; i++) {
-			if (i % 2 != 0 && i == (arr_information.length - 1)) {
-				arr_information[i].style.backgroundColor = "#E4E4E4";
-				arr_information[i].style.borderBottomLeftRadius = "16px";
-				arr_information[i].style.borderBottomRightRadius = "16px";
-			} else if (i % 2 != 0) {
-				arr_information[i].style.backgroundColor = "#E4E4E4";
-			}
-		}
+		let ship_level = document.querySelector(".ship-level").innerText;
+		let level_number = ["1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "11"];
+		let level_roma = ["I", "II", "III", "IV", "V", "VI", "VII", "VIII", "IX", "X", "★"];
+		let ship_level_roma = level_roma[level_number.indexOf(ship_level)]
+		document.querySelector(".ship-level").innerText = ship_level_roma;
 	</script>
+	
 </html>
```

#### html2text {}

```diff
@@ -1,112 +1,110 @@
 {% if data['clanInfo']['tag'] %}
 [{{ data['clanInfo']['tag'] }}]
 {% endif %}
 {{ data['userName'] }}
 {{ data['serverName'] }}
-{{ data['pr']['value'] }}    
+{% if data['shipInfo']['shipInfo']['nameCn'] %}
+{{ data['shipInfo']['shipInfo']['level'] }}
+{% else %}
+{{ data['rankSolo']['shipInfo']['level'] }}
+{% endif %} {% if data['shipInfo']['shipInfo']['nameCn'] %}
+{{ data['shipInfo']['shipInfo']['nameCn'] }}
+{% else %}
+{{ data['rankSolo']['shipInfo']['nameCn'] }}
+{% endif %}
+'shipInfo']['shipInfo']['shipType'] == 'Destroyer' or data['rankSolo']
+['shipInfo']['shipType'] == 'Destroyer' %} "https://hikari-resource.oss-cn-
+shanghai.aliyuncs.com/shipType_Icon/icon_sunk_destroyer.png" {% elif data
+['shipInfo']['shipInfo']['shipType'] == 'Cruiser' or data['rankSolo']
+['shipInfo']['shipType'] == 'Cruiser' %} "https://hikari-resource.oss-cn-
+shanghai.aliyuncs.com/shipType_Icon/icon_sunk_cruiser.png" {% elif data
+['shipInfo']['shipInfo']['shipType'] == 'Battleship' or data['rankSolo']
+['shipInfo']['shipType'] == 'Battleship' %} "https://hikari-resource.oss-cn-
+shanghai.aliyuncs.com/shipType_Icon/icon_sunk_battleship.png" {% elif data
+['shipInfo']['shipInfo']['shipType'] == 'AirCarrier' or data['rankSolo']
+['shipInfo']['shipType'] == 'AirCarrier' %} "https://hikari-resource.oss-cn-
+shanghai.aliyuncs.com/shipType_Icon/icon_sunk_aircarrier.png" {% else %}
+"https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/
+icon_sunk_submarine.png" {% endif %} />
+{% if data['shipInfo']['pr']['color'] and data['shipInfo']['pr']['color'] !=
+'#828282' %} {{ data['shipInfo']['pr']['value'] }}      {% else %} {{ data
+['rankSolo']['pr']['value'] }}      {% endif %}
 æåæææ¶é´ï¼{{ time.strftime('%Y-%m-%d %H:%M:%S',time.localtime(abs
-(data['lastDateTime']))) }}
-åºæ¬¡
-{{ data['pvp']['battles'] }}
-PR
-è¾ä¸æ¬¡
-{{ '%+d' | format(data['dwpDataVO']['pr']) }}
-èç
-{{ data['pvp']['wins'] }}%
+(data['shipInfo']['lastBattlesTime']))) }}
+{% if data['shipRank'] %}
+æå  {{data['shipRank']}}
+{% endif %} {% if data['rank'] != -1 %}
+æå  {{data['rank']}}
+{% endif %}
 åºå
-{{ '%+d' | format(data['dwpDataVO']['damage']) }}
 èç
-{{ '%+.2f' | format(data['dwpDataVO']['wins']) }}%
-åºå
-{{ data['pvp']['damage'] }}
-å»æ
-{{ '%.2f' | format(data['pvp']['frags']) }}
-å½ä¸­
-{{ '%.2f' | format(data['pvp']['hit']) }}%
-è¹åªæ°æ®
-ç±»å
+PR
+{{ '%+d' | format(data['dwpDataVO']['damage']) }}
+{{ '%+.2f' | format(data['dwpDataVO']['wins']) }}
+{{ '%+d' | format(data['dwpDataVO']['pr']) }}
 åºæ¬¡
+{{ data['shipInfo']['battles'] }}
 èç
-PR
+{{ data['shipInfo']['wins'] }}%
 åºå
+{{ data['shipInfo']['damage'] }}
+ç»éª
+{{ data['shipInfo']['xp'] }}
+å»æ
+{{ '%.2f' | format(data['shipInfo']['frags']) }}
 å½ä¸­
-{% if data['type']['Battleship']['battles'] %}
-æåè°
-{{ data['type']['Battleship']['battles'] }}
-{{ data['type']['Battleship']['wins'] }}%
-{{ data['type']['Battleship']['pr']['value'] }}
-{{ data['type']['Battleship']['damage'] }}
-{{ '%.2f' | format (data['type']['Battleship']['hit']) }}%
-{% endif %} {% if data['type']['Cruiser']['battles'] %}
-å·¡æ´è°
-{{ data['type']['Cruiser']['battles'] }}
-{{ data['type']['Cruiser']['wins'] }}%
-{{ data['type']['Cruiser']['pr']['value'] }}
-{{ data['type']['Cruiser']['damage'] }}
-{{ '%.2f' | format (data['type']['Cruiser']['hit']) }}%
-{% endif %} {% if data['type']['Destroyer']['battles'] %}
-é©±éè°
-{{ data['type']['Destroyer']['battles'] }}
-{{ data['type']['Destroyer']['wins'] }}%
-{{ data['type']['Destroyer']['pr']['value'] }}
-{{ data['type']['Destroyer']['damage'] }}
-{{ '%.2f' | format (data['type']['Destroyer']['hit']) }}%
-{% endif %} {% if data['type']['AirCarrier']['battles'] %}
-èªç©ºæ¯è°
-{{ data['type']['AirCarrier']['battles'] }}
-{{ data['type']['AirCarrier']['wins'] }}%
-{{ data['type']['AirCarrier']['pr']['value'] }}
-{{ data['type']['AirCarrier']['damage'] }}
-{{ '%.2f' | format (data['type']['AirCarrier']['hit']) }}%
-{% endif %} {% if data['type']['Submarine']['battles'] %}
-æ½è
-{{ data['type']['Submarine']['battles'] }}
-{{ data['type']['Submarine']['wins'] }}%
-{{ data['type']['Submarine']['pr']['value'] }}
-{{ data['type']['Submarine']['damage'] }}
-{{ '%.2f' | format (data['type']['Submarine']['hit']) }}%
-{% endif %}
+{{ data['shipInfo']['hit'] }}%
 æ»ä½æç»©
 ç±»å
 åºæ¬¡
 èç
 PR
 åºå
 å»æ
-{% if data['pvpSolo']['battles'] %}
+{% if data['shipSolo']['battles'] %}
 åé
-{{ data['pvpSolo']['battles'] }}
-{{ data['pvpSolo']['wins'] }}%
-{{ data['pvpSolo']['pr']['value'] }}
-{{ data['pvpSolo']['damage'] }}
-{{ '%.2f' | format(data['pvpSolo']['frags']) }}
-{% endif %} {% if data['pvpTwo']['battles'], %}
+{{ data['shipSolo']['battles'] }}
+{{ data['shipSolo']['wins'] }}%
+{{ data['shipSolo']['pr']['value'] }}
+{{ data['shipSolo']['damage'] }}
+{{ '%.2f' | format(data['shipSolo']['frags']) }}
+{% endif %} {% if data['shipTwo']['battles'] %}
 èªè¡è½¦
-{{ data['pvpTwo']['battles'] }}
-{{ data['pvpTwo']['wins'] }}%
-{{ data['pvpTwo']['pr']['value'] }}
-{{ data['pvpTwo']['damage'] }}
-{{ '%.2f' | format(data['pvpTwo']['frags']) }}
-{% endif %} {% if data['pvpThree']['battles'] %}
+{{ data['shipTwo']['battles'] }}
+{{ data['shipTwo']['wins'] }}%
+{{ data['shipTwo']['pr']['value'] }}
+{{ data['shipTwo']['damage'] }}
+{{ '%.2f' | format(data['shipTwo']['frags']) }}
+{% endif %} {% if data['shipThree']['battles'] %}
 ä¸è½®è½¦
-{{ data['pvpThree']['battles'] }}
-{{ data['pvpThree']['wins'] }}%
-{{ data['pvpThree']['pr']['value'] }}
-{{ data['pvpThree']['damage'] }}
-{{ '%.2f' | format(data['pvpThree']['frags']) }}
+{{ data['shipThree']['battles'] }}
+{{ data['shipThree']['wins'] }}%
+{{ data['shipThree']['pr']['value'] }}
+{{ data['shipThree']['damage'] }}
+{{ '%.2f' | format(data['shipThree']['frags']) }}
 {% endif %} {% if data['rankSolo']['battles'] %}
 æä½
 {{ data['rankSolo']['battles'] }}
 {{ data['rankSolo']['wins'] }}%
 {{ data['rankSolo']['pr']['value'] }}
 {{ data['rankSolo']['damage'] }}
 {{ '%.2f' | format(data['rankSolo']['frags']) }}
 {% endif %}
-Â©è¥¿è¡å¯ºé¨å­£  Â©æ¬å¿
+æé«çºªå½
+æé«ä¼¤å®³
+{{ data['shipInfo']['extensionDataInfo']['maxDamage'] }}
+ä¾¦å¯ä¼¤å®³
+{{ data['shipInfo']['extensionDataInfo']['maxDamageScouting'] }}
+æé«æ½å¨
+{{ data['shipInfo']['extensionDataInfo']['maxTotalAgro'] }}
+ç»éª
+{{ data['shipInfo']['extensionDataInfo']['maxXp'] }}
+å»æ
+{{ data['shipInfo']['extensionDataInfo']['maxFrags'] }}
+é£æºå»è½
+{{ data['shipInfo']['extensionDataInfo']['maxPlanesKilled'] }}
+Â© è¥¿è¡å¯ºé¨å­£  Â© æ¬å¿
 https://github.com/benx1n/HikariBot
 QQé¢éæç´¢âyuyukoâå³å¯ä½¿ç¨ç¨³å®çè¾è®¯å®æ¹æºå¨äºº~
 Design By å·ç  H5 Converted By C1ystal
-èµå©é¸£è°¢ï¼ç·äººä»¬çå®è¿å·ãWishingãç§é¿
-{% if template_path and template_path/"echarts.js" %}
- {% else %}
- {% endif %}
+èµå©é¸£è°¢ï¼ç§é¿ãç·äººä»¬çå®è¿å·ãæµ·ä¸æéæ´æ¯ä¼ è¯´
```

### Comparing `hikari_core-0.1.5/hikari_core/Template/wws-personalRecord.html` & `hikari_core-0.1.6/hikari_core/Template/wws-personalRecord.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.5/hikari_core/Template/wws-ship-recent.html` & `hikari_core-0.1.6/hikari_core/Template/wws-info.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,686 +1,825 @@
 <!DOCTYPE html>
 <html>
-	<head>
-		<meta charset="utf-8">
-		<title></title>
-	</head>
-	<style>
-		* {
-			padding: 0;
-			margin: 0;
-		}
-
-		.flex-2 {
-			flex: 2;
-		}
-
-		.flex-3 {
-			flex: 3;
-		}
-
-		.flex-4 {
-			flex: 4;
-		}
-
-		.flex-8 {
-			flex: 8;
-		}
-
-		.flex-10 {
-			flex: 10;
-		}
-
-		.main-content {
-			width: 1000px;
-			font-size: 30px;
-			font-family: "Microsoft YaHei";
-			font-weight: bold;
-		}
-
-		.page-box {
-			width: 1000px;
-			display: flex;
-			flex-direction: column;
-		}
-
-		.page-header {
-			display: flex;
-			flex-direction: column;
-		}
-
-		.clan-user-server {
-			height: 120px;
-			text-align: center;
-			font-size: 45px;
-			line-height: 120px;
-		}
-
-		.clan {
-			display: inline-block;
-			padding-right: 10px;
-			height: 120px;
-		}
-
-		.user {
-			display: inline-block;
-			height: 120px;
-		}
-
-		.server {
-			display: inline-block;
-			padding-left: 10px;
-		}
-
-		.server-border {
-			width: 200px;
-			height: 50px;
-			line-height: 50px;
-			text-align: center;
-			background-color: #F2F2F2;
-			border-radius: 25px;
-			font-size: 35px;
-		}
-
-		.ship-bar {
-			height: 80px;
-			font-size: 40px;
-			line-height: 80px;
-			text-align: center;
-			display: flex;
-		}
-
-		.ship-level {
-			flex: 1;
-			text-align: right;
-			margin-right: 30px;
-		}
-
-		.ship-icon {
-			flex: 1;
-			text-align: left;
-			margin-left: 30px;
-		}
-
-		.ship-icon img {
-			width: 80px;
-			height: 80px;
-		}
-
-		.pr {
-			display: flex;
-			height: 100px;
-			font-weight: bold;
-			line-height: 60px;
-			padding: 0 50px;
-		}
-
-		.pr-bar-bg {
-			position: relative;
-			flex: 1;
-			line-height: 80px;
-			background-color: #A6A6A6;
-			height: 80px;
-			border-radius: 40px;
-			margin-top: 10px;
-			text-align: center;
-			color: #FFFFFF;
-		}
-
-		.pr-bar {
-			position: absolute;
-			top: 0;
-			left: 0;
-			height: 80px;
-			z-index: 1;
-			border-radius: 40px;
-		}
-
-		.pr-number {
-			z-index: 99;
-			position: absolute;
-			left: 0px;
-			right: 0px;
-			font-size: 35px;
-			font-weight: bold;
-		}
-
-		.recnet-time {
-			text-align: center;
-			font-weight: normal;
-		}
-
-		.overview-change {
-			display: flex;
-			margin-top: 30px;
-			padding: 0 30px;
-			height: 300px;
-		}
-
-		.overview-change-item {
-			flex: 1;
-			display: flex;
-			flex-direction: column;
-			margin: 0 20px;
-
-		}
-
-		.item-top {
-			flex: 5;
-			background-color: #F2F2F2;
-			border-radius: 16px;
-		}
-
-		.item-bottom {
-			display: flex;
-			flex: 4;
-			margin-top: 20px;
-		}
-
-		.left-item-bottom {
-			background-color: #F2F2F2;
-			border-radius: 16px;
-		}
-
-		.bottom-mini-item-left {
-			flex: 1;
-			margin-right: 10px;
-			background-color: #F2F2F2;
-			border-radius: 16px;
-		}
-
-		.bottom-mini-item-right {
-			flex: 1;
-			margin-left: 10px;
-			background-color: #F2F2F2;
-			border-radius: 16px;
-		}
-
-		.item-top {
-			display: flex;
-			flex-direction: column;
-		}
-
-		.item-top div {
-			height: 80px;
-			text-align: center;
-			font-size: 40px;
-		}
-
-		.item-top-top {
-			color: #606266;
-			font-weight: normal;
-			line-height: 100px;
-		}
-
-		.item-top-bottom {
-			line-height: 60px;
-		}
-
-		.left-item-bottom {
-			display: flex;
-			flex-direction: column;
-		}
-
-		.change-pr-title {
-			color: #606266;
-			height: 60px;
-			display: flex;
-			font-weight: normal;
-			line-height: 70px;
-		}
-
-		.change-pr {
-			height: 60px;
-			line-height: 50px;
-			text-align: center;
-			font-size: 30px;
-		}
-
-		.change-pr-title-left {
-			flex: 1;
-			font-size: 35px;
-			text-align: right;
-			margin-right: 30px;
-		}
-
-		.change-pr-title-right {
-			flex: 1;
-			font-size: 20px;
-		}
-
-		.bottom-mini-item-left,
-		.bottom-mini-item-right {
-			display: flex;
-			flex-direction: column;
-		}
 
-		.mini-item-top {
-			color: #606266;
-			font-weight: normal;
-			line-height: 70px;
-		}
-
-		.mini-item-bottom {
-			line-height: 45px;
-			font-size: 27px;
-		}
-
-		.bottom-mini-item-left div,
-		.bottom-mini-item-right div {
-			height: 60px;
-			text-align: center;
-		}
-
-		.information-header,
-		.day-header {
-			margin: 0 200px;
-			margin-top: 30px;
-			height: 60px;
-			line-height: 60px;
-			border-radius: 16px;
-			background-color: #D9D9D9;
-			text-align: center;
-		}
-
-		.information-body {
-			margin: 0 50px;
-			margin-top: 30px;
-			display: flex;
-			flex-direction: column;
-			background-color: #F2F2F2;
-			border-radius: 16px;
-		}
-
-		.information-col {
-			height: 60px;
-			display: flex;
-			line-height: 60px;
-		}
-
-		.information-col-item,
-		.day-col-item {
-			flex: 1;
-			text-align: center;
-		}
-
-		.information-table-header {
-			color: #606266;
-		}
-
-		.information-type {
-			color: #909399;
-		}
-
-		.day-body {
-			margin: 0 50px;
-			margin-top: 30px;
-		}
-
-		.day-table-header {
-			height: 60px;
-			line-height: 60px;
-			background-color: #D9D9D9;
-			display: flex;
-			border-radius: 16px;
-			color: #606266;
-		}
-
-		.date {
-			background-color: #D9D9D9;
-			width: 300px;
-			height: 40px;
-			line-height: 40px;
-			text-align: center;
-			border-radius: 20px;
-			margin-top: 10px;
-		}
-
-		.day-col {
-			display: flex;
-			height: 60px;
-			line-height: 60px;
-			background-color: #F2F2F2;
-			border-radius: 30px;
-			margin: 10px 0;
-		}
-
-		.footer {
-			margin-top: 30px;
-			text-align: center;
-			font-weight: bold;
-			font-size: 24px;
-			color: #909399;
-			margin-bottom: 20px;
-		}
-	</style>
-	<body>
-		<div class="main-content">
-			<div class="page-box">
-				<div class="page-header">
-					<div class="clan-user-server">
-						
-						{% if data['clanInfo']['tag'] %}
-						<div class="clan" style="color: {{ data['clanInfo']['colorRgb'] }};">[{{ data['clanInfo']['tag'] }}]</div>
-						{% endif %}
-						<div class="user">{{ data['userName'] }}</div>
-						<div class="server">
-							<div class="server-border">
-								{{ data['serverName'] }}
-							</div>
-						</div>
-					</div>
-				</div>
-
-				<div class="ship-bar">
-					{% if data['shipData'][0]['shipInfo']['shipInfo']['nameCn'] %}
-					<div class="ship-level">{{ data['shipData'][0]['shipInfo']['shipInfo']['level'] }}</div>
-					{% else %}
-					<div class="ship-level">{{ data['shipData'][0]['rankSolo']['shipInfo']['level'] }}</div>
-					{% endif %}
-					
-					{% if data['shipData'][0]['shipInfo']['shipInfo']['nameCn'] %}
-					<div class="ship-name">{{ data['shipData'][0]['shipInfo']['shipInfo']['nameCn'] }}</div>
-					{% else %}
-					<div class="ship-name">{{ data['shipData'][0]['rankSolo']['shipInfo']['nameCn'] }}</div>
+<head>
+	<meta charset="utf-8">
+	<title></title>
+</head>
+<style>
+	* {
+		margin: 0;
+		padding: 0;
+	}
+
+	.main-content {
+		width: 1200px;
+		font-size: 30px;
+		font-family: "Microsoft YaHei";
+		font-weight: bold;
+	}
+
+	.page-box {
+		width: 1200px;
+		display: flex;
+		flex-direction: column;
+	}
+
+	.page-header {
+		display: flex;
+		flex-direction: column;
+		margin-top: 30px;
+	}
+
+	.clan-user-server {
+		height: 120px;
+		text-align: center;
+		font-size: 45px;
+		line-height: 120px;
+	}
+
+	.clan {
+		display: inline-block;
+		padding-right: 10px;
+		height: 120px;
+	}
+
+	.user {
+		display: inline-block;
+		height: 120px;
+	}
+
+	.server {
+		display: inline-block;
+		padding-left: 10px;
+	}
+
+	.server-border {
+		width: 200px;
+		height: 50px;
+		line-height: 50px;
+		text-align: center;
+		background-color: #F2F2F2;
+		border-radius: 25px;
+		font-size: 35px;
+	}
+
+	.image-box {
+		width: 100px;
+		height: 100px;
+		position: fixed;
+		left: 50px;
+		top: 40px;
+	}
+
+	.image-box img {
+		width: 100px;
+		height: 100px;
+		border-radius: 50px;
+	}
+
+	.pr {
+		display: flex;
+		height: 100px;
+		font-weight: bold;
+		line-height: 60px;
+		padding: 0 80px;
+	}
+
+	.pr-bar-bg {
+		position: relative;
+		flex: 1;
+		line-height: 80px;
+		background-color: #A6A6A6;
+		height: 80px;
+		border-radius: 40px;
+		margin-top: 10px;
+		text-align: center;
+		color: #FFFFFF;
+	}
+
+	.pr-bar {
+		position: absolute;
+		top: 0;
+		left: 0;
+		height: 80px;
+		z-index: 1;
+		border-radius: 40px;
+	}
+
+	.pr-number {
+		z-index: 99;
+		position: absolute;
+		left: 0px;
+		right: 0px;
+		font-size: 35px;
+		font-weight: bold;
+	}
+
+	.recnet-time {
+		text-align: center;
+		font-weight: normal;
+	}
+
+	.overview-change {
+		display: flex;
+		margin-top: 30px;
+		padding: 0 50px;
+		height: 300px;
+	}
+
+	.overview-change-item {
+		flex: 1;
+		display: flex;
+		flex-direction: column;
+		margin: 0 20px;
+
+	}
+
+	.item-top {
+		flex: 5;
+		background-color: #F2F2F2;
+		border-radius: 16px;
+	}
+
+	.item-bottom {
+		display: flex;
+		flex: 4;
+		margin-top: 20px;
+	}
+
+	.left-item-bottom {
+		background-color: #F2F2F2;
+		border-radius: 16px;
+	}
+
+	.bottom-mini-item-left {
+		flex: 1;
+		margin-right: 10px;
+		background-color: #F2F2F2;
+		border-radius: 16px;
+	}
+
+	.bottom-mini-item-right {
+		flex: 1;
+		margin-left: 10px;
+		background-color: #F2F2F2;
+		border-radius: 16px;
+	}
+
+	.item-top {
+		display: flex;
+		flex-direction: column;
+	}
+
+	.item-top div {
+		height: 80px;
+		text-align: center;
+		font-size: 40px;
+	}
+
+	.item-top-top {
+		color: #606266;
+		font-weight: normal;
+		line-height: 100px;
+	}
+
+	.item-top-bottom {
+		line-height: 60px;
+	}
+
+	.left-item-bottom {
+		display: flex;
+		flex-direction: column;
+	}
+
+	.change-pr-title {
+		color: #606266;
+		height: 60px;
+		display: flex;
+		font-weight: normal;
+		line-height: 70px;
+	}
+
+	.change-pr {
+		height: 60px;
+		line-height: 50px;
+		text-align: center;
+		font-size: 30px;
+	}
+
+	.change-pr-title-left {
+		flex: 1;
+		font-size: 35px;
+		text-align: right;
+		margin-right: 30px;
+	}
+
+	.change-pr-title-right {
+		flex: 1;
+		font-size: 20px;
+	}
+
+	.bottom-mini-item-left,
+	.bottom-mini-item-right {
+		display: flex;
+		flex-direction: column;
+	}
+
+	.mini-item-top {
+		color: #606266;
+		font-weight: normal;
+		line-height: 70px;
+	}
+
+	.mini-item-bottom {
+		line-height: 45px;
+		font-size: 27px;
+	}
+
+	.bottom-mini-item-left div,
+	.bottom-mini-item-right div {
+		height: 60px;
+		text-align: center;
+	}
+
+	.information-header,
+	.ship-data-header {
+		margin: 0 200px;
+		margin-top: 30px;
+		height: 60px;
+		line-height: 60px;
+		border-radius: 16px;
+		background-color: #D9D9D9;
+		text-align: center;
+	}
+
+	.information-body,
+	.ship-data-body {
+		margin: 0 80px;
+		margin-top: 30px;
+		display: flex;
+		flex-direction: column;
+		background-color: #F2F2F2;
+		border-radius: 16px;
+	}
+
+	.information-col,
+	.ship-data-col {
+		height: 60px;
+		display: flex;
+		line-height: 60px;
+	}
+
+	.information-col-item,
+	.ship-data-col-item {
+		flex: 1;
+		text-align: center;
+	}
+
+	.information-table-header,
+	.ship-data-table-header {
+		color: #606266;
+	}
+
+	.information-type,
+	.ship-data-type {
+		color: #909399;
+	}
+
+	.chart-box {
+		margin: 0 80px;
+		margin-top: 30px;
+		background-color: #F2F2F2;
+		height: 400px;
+		display: flex;
+		border-radius: 16px;
+	}
+
+	.chart-bar {
+		flex: 6;
+	}
+
+	.chart-pie {
+		flex: 4;
+	}
+
+	.footer {
+		margin-top: 30px;
+		text-align: center;
+		font-weight: bold;
+		font-size: 24px;
+		color: #909399;
+		margin-bottom: 20px;
+	}
+</style>
+
+<body>
+	<div class="main-content">
+		<div class="page-box">
+			<div class="page-header">
+
+				<!-- 					<div class="image-box">
+						<img src="IMG_20220607_224103.jpg" />
+					</div> -->
+
+				<div class="clan-user-server">
+					{% if data['userInfo']['clanInfo']['tag'] %}
+					<div class="clan" style="color: {{ data['userInfo']['clanInfo']['color'] }};">[{{
+						data['userInfo']['clanInfo']['tag'] }}]</div>
 					{% endif %}
-					
-					<div class="ship-icon"><img
-									src={% if data['shipData'][0]['shipInfo']['shipInfo']['shipType'] == 'Destroyer' or data['shipData'][0]['rankSolo']['shipInfo']['shipType'] == 'Destroyer' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_destroyer.png"
-									{% elif data['shipData'][0]['shipInfo']['shipInfo']['shipType'] == 'Cruiser' or data['shipData'][0]['rankSolo']['shipInfo']['shipType'] == 'Cruiser' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_cruiser.png"
-									{% elif data['shipData'][0]['shipInfo']['shipInfo']['shipType'] == 'Battleship' or data['shipData'][0]['rankSolo']['shipInfo']['shipType'] == 'Battleship' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_battleship.png"
-									{% elif data['shipData'][0]['shipInfo']['shipInfo']['shipType'] == 'AirCarrier' or data['shipData'][0]['rankSolo']['shipInfo']['shipType'] == 'AirCarrier' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_aircarrier.png"
-									{% else %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_submarine.png"
-									{% endif %} />
+					<div class="user">{{ data['userInfo']['userName'] }}</div>
+					<div class="server">
+						<div class="server-border">
+							{{ data['userInfo']['server'] }}
+						</div>
 					</div>
 				</div>
 
 				<div class="pr">
 					<!-- 动态设置长度及颜色，填写PR即可 -->
 					<div class="pr-bar-bg">
-						{% if data['pvpInfo']['pr']['color'] and data['pvpInfo']['pr']['color'] != '#828282' %}
-						<span class="pr-number">{{ data['pvpInfo']['pr']['value'] }} &nbsp;&nbsp;&nbsp;&nbsp;<span class="pr-text"></span></span>
-						{% else %}
-						<span class="pr-number">{{ data['rankInfo']['pr']['value'] }} &nbsp;&nbsp;&nbsp;&nbsp;<span class="pr-text"></span></span>
-						{% endif %}
+						<span class="pr-number">{{ data['prInfo']['value'] }}&nbsp;&nbsp;&nbsp;&nbsp;<span
+								class="pr-text"></span></span>
 						<div class="pr-bar"></div>
 					</div>
 				</div>
 
 				<div class="recnet-time">
-					<span>记录时间：</span><span>{{ time.strftime('%Y-%m-%d %H:%M',time.localtime(int(abs(data['shipData'][0]['recordDateTime']/1000)))) }}—{{ time.strftime('%Y-%m-%d %H:%M',time.localtime(time.time())) }}</span>
+					<span>最后战斗时间：</span><span>{{ time.strftime('%Y-%m-%d
+						%H:%M:%S',time.localtime(abs(data['battleTypeInfo'][0]['shipInfo']['lastBattleTime'])))
+						}}</span>
 				</div>
 
-				{% if data['pvpInfo']['battles'] %}
 				<div class="overview-change">
 					<div class="overview-change-item left-item">
 						<div class="left-item-top item-top">
 							<div class="overview-count-title item-top-top">场次</div>
-							<div class="overview-count item-top-bottom">{{ data['pvpInfo']['battles'] }}</div>
+							<div class="overview-count item-top-bottom">{{
+								data['battleTypeInfo'][0]['shipInfo']['battleInfo']['battle'] }}</div>
 						</div>
 						<div class="left-item-bottom item-bottom">
 							<div class="change-pr-title">
 								<div class="change-pr-title-left">PR</div>
-								<div class="change-pr-title-right">较上周</div>
+								<div class="change-pr-title-right">较上次</div>
 							</div>
-							<div class="change-pr">暂不可用</div>
+							<div class="change-pr">{{ '%+d' | format(data['dwpDataVO']['pr']) }}</div>
 						</div>
 					</div>
 					<div class="overview-change-item mid-item">
 						<div class="mid-item-top item-top">
 							<div class="overview-win-title item-top-top">胜率</div>
-							<div class="overview-win item-top-bottom" style="color: {{ data['pvpInfo']['winsData']['color'] }}">{{ data['pvpInfo']['wins'] }}%</div>
+							<div class="overview-win item-top-bottom"
+								style="color: {{ data['pvp']['winsData']['color'] }}">{{ data['pvp']['wins'] }}%</div>
 						</div>
 						<div class="mid-item-bottom item-bottom">
 							<div class="change-avgdmg-box bottom-mini-item-left">
 								<div class="mini-item-top">场均</div>
-								<div class="mini-item-bottom change-avgdmg">暂不可用</div>
+								<div class="mini-item-bottom change-avgdmg">{{ '%+d' |
+									format(data['dwpDataVO']['damage']) }}</div>
 							</div>
 							<div class="change-win-box bottom-mini-item-right">
 								<div class="mini-item-top">胜率</div>
-								<div class="mini-item-bottom change-win">暂不可用</div>
+								<div class="mini-item-bottom change-win">{{ '%+.2f' | format(data['dwpDataVO']['wins'])
+									}}%</div>
 							</div>
 						</div>
 					</div>
 					<div class="overview-change-item right-item">
 						<div class="right-item-top item-top">
 							<div class="overview-avgdmg-title item-top-top">场均</div>
-							<div class="overview-avgdmg item-top-bottom" style="color: {{ data['pvpInfo']['damageData']['color'] }};">{{ data['pvpInfo']['damage'] }}</div>
+							<div class="overview-avgdmg item-top-bottom"
+								style="color: {{ data['pvp']['damageData']['color'] }};">{{ data['pvp']['damage'] }}
+							</div>
 						</div>
 						<div class="right-item-bottom item-bottom">
 							<div class="overview-kd-box bottom-mini-item-left">
 								<div class="mini-item-top">击杀</div>
-								<div class="mini-item-bottom">{{ '%.2f' | format(data['pvpInfo']['frags']) }}</div>
+								<div class="mini-item-bottom">{{ '%.2f' | format(data['pvp']['frags']) }}</div>
 							</div>
 							<div class="overview-hit-box bottom-mini-item-right">
 								<div class="mini-item-top">命中</div>
-								<div class="mini-item-bottom">{{ data['pvpInfo']['hit'] }}%</div>
+								<div class="mini-item-bottom">{{ '%.2f' | format(data['pvp']['hit']) }}%</div>
 							</div>
 						</div>
 					</div>
 				</div>
-				{% endif %}
+
+				<div class="ship-data-header">船只数据</div>
+
+				<div class="ship-data-body">
+					<div class="ship-data-col ship-data-table-header">
+						<div class="ship-data-col-item">类型</div>
+						<div class="ship-data-col-item">场次</div>
+						<div class="ship-data-col-item">胜率</div>
+						<div class="ship-data-col-item">PR</div>
+						<div class="ship-data-col-item">场均</div>
+						<div class="ship-data-col-item">命中</div>
+					</div>
+
+					{% if data['type']['Battleship']['battles'] %}
+					<div class="ship-data-col">
+						<div class="ship-data-col-item ship-data-type">战列舰</div>
+						<div class="ship-data-col-item">{{ data['type']['Battleship']['battles'] }}</div>
+						<div class="ship-data-col-item"
+							style="color: {{ data['type']['Battleship']['winsData']['color'] }};">{{
+							data['type']['Battleship']['wins'] }}%</div>
+						<div class="ship-data-col-item" style="color: {{ data['type']['Battleship']['pr']['color'] }};">
+							{{ data['type']['Battleship']['pr']['value'] }}</div>
+						<div class="ship-data-col-item"
+							style="color: {{ data['type']['Battleship']['damageData']['color'] }};">{{
+							data['type']['Battleship']['damage'] }}</div>
+						<div class="ship-data-col-item">{{ '%.2f' | format (data['type']['Battleship']['hit']) }}%</div>
+					</div>
+					{% endif %}
+
+					{% if data['type']['Cruiser']['battles'] %}
+					<div class="ship-data-col">
+						<div class="ship-data-col-item ship-data-type">巡洋舰</div>
+						<div class="ship-data-col-item">{{ data['type']['Cruiser']['battles'] }}</div>
+						<div class="ship-data-col-item"
+							style="color: {{ data['type']['Cruiser']['winsData']['color'] }};">{{
+							data['type']['Cruiser']['wins'] }}%</div>
+						<div class="ship-data-col-item" style="color: {{ data['type']['Cruiser']['pr']['color'] }};">{{
+							data['type']['Cruiser']['pr']['value'] }}</div>
+						<div class="ship-data-col-item"
+							style="color: {{ data['type']['Cruiser']['damageData']['color'] }};">{{
+							data['type']['Cruiser']['damage'] }}</div>
+						<div class="ship-data-col-item">{{ '%.2f' | format (data['type']['Cruiser']['hit']) }}%</div>
+					</div>
+					{% endif %}
+
+
+					{% if data['type']['Destroyer']['battles'] %}
+					<div class="ship-data-col">
+						<div class="ship-data-col-item ship-data-type">驱逐舰</div>
+						<div class="ship-data-col-item">{{ data['type']['Destroyer']['battles'] }}</div>
+						<div class="ship-data-col-item"
+							style="color: {{ data['type']['Destroyer']['winsData']['color'] }};">{{
+							data['type']['Destroyer']['wins'] }}%</div>
+						<div class="ship-data-col-item" style="color: {{ data['type']['Destroyer']['pr']['color'] }};">
+							{{ data['type']['Destroyer']['pr']['value'] }}</div>
+						<div class="ship-data-col-item"
+							style="color: {{ data['type']['Destroyer']['damageData']['color'] }};">{{
+							data['type']['Destroyer']['damage'] }}</div>
+						<div class="ship-data-col-item">{{ '%.2f' | format (data['type']['Destroyer']['hit']) }}%</div>
+					</div>
+					{% endif %}
+
+					{% if data['type']['AirCarrier']['battles'] %}
+					<div class="ship-data-col">
+						<div class="ship-data-col-item ship-data-type">航空母舰</div>
+						<div class="ship-data-col-item">{{ data['type']['AirCarrier']['battles'] }}</div>
+						<div class="ship-data-col-item"
+							style="color: {{ data['type']['AirCarrier']['winsData']['color'] }};">{{
+							data['type']['AirCarrier']['wins'] }}%</div>
+						<div class="ship-data-col-item" style="color: {{ data['type']['AirCarrier']['pr']['color'] }};">
+							{{ data['type']['AirCarrier']['pr']['value'] }}</div>
+						<div class="ship-data-col-item"
+							style="color: {{ data['type']['AirCarrier']['damageData']['color'] }};">{{
+							data['type']['AirCarrier']['damage'] }}</div>
+						<div class="ship-data-col-item">{{ '%.2f' | format (data['type']['AirCarrier']['hit']) }}%</div>
+					</div>
+					{% endif %}
+
+					{% if data['type']['Submarine']['battles'] %}
+					<div class="ship-data-col">
+						<div class="ship-data-col-item ship-data-type">潜艇</div>
+						<div class="ship-data-col-item">{{ data['type']['Submarine']['battles'] }}</div>
+						<div class="ship-data-col-item"
+							style="color: {{ data['type']['Submarine']['winsData']['color'] }};">{{
+							data['type']['Submarine']['wins'] }}%</div>
+						<div class="ship-data-col-item" style="color: {{ data['type']['Submarine']['pr']['color'] }};">
+							{{ data['type']['Submarine']['pr']['value'] }}</div>
+						<div class="ship-data-col-item"
+							style="color: {{ data['type']['Submarine']['damageData']['color'] }};">{{
+							data['type']['Submarine']['damage'] }}</div>
+						<div class="ship-data-col-item">{{ '%.2f' | format (data['type']['Submarine']['hit']) }}%</div>
+					</div>
+					{% endif %}
+
+				</div>
 
 				<div class="information-header">总体战绩</div>
 
 				<div class="information-body">
 					<div class="information-col information-table-header">
 						<div class="information-col-item">类型</div>
 						<div class="information-col-item">场次</div>
 						<div class="information-col-item">胜率</div>
 						<div class="information-col-item">PR</div>
 						<div class="information-col-item">场均</div>
 						<div class="information-col-item">击杀</div>
 					</div>
-					
-					{% if data['pvpSoloInfo']['battles'] %}
+
+					{% if data['pvpSolo']['battles'] %}
 					<div class="information-col">
 						<div class="information-col-item information-type">单野</div>
-						<div class="information-col-item">{{ data['pvpSoloInfo']['battles'] }}</div>
-						<div class="information-col-item" style="color: {{ data['pvpSoloInfo']['winsData']['color'] }};">{{ data['pvpSoloInfo']['wins'] }}%</div>
-						<div class="information-col-item" style="color: {{ data['pvpSoloInfo']['pr']['color'] }};">{{ data['pvpSoloInfo']['pr']['value'] }}</div>
-						<div class="information-col-item" style="color: {{ data['pvpSoloInfo']['damageData']['color'] }};">{{ data['pvpSoloInfo']['damage'] }}</div>
-						<div class="information-col-item">{{ '%.2f' | format(data['pvpSoloInfo']['frags']) }}</div>
+						<div class="information-col-item">{{ data['pvpSolo']['battles'] }}</div>
+						<div class="information-col-item" style="color: {{ data['pvpSolo']['winsData']['color'] }};">{{
+							data['pvpSolo']['wins'] }}%</div>
+						<div class="information-col-item" style="color: {{ data['pvpSolo']['pr']['color'] }};">{{
+							data['pvpSolo']['pr']['value'] }}</div>
+						<div class="information-col-item" style="color: {{ data['pvpSolo']['damageData']['color'] }};">
+							{{ data['pvpSolo']['damage'] }}</div>
+						<div class="information-col-item">{{ '%.2f' | format(data['pvpSolo']['frags']) }}</div>
 					</div>
 					{% endif %}
 
-					{% if data['pvpTwoInfo']['battles'] %}
+					{% if data['pvpTwo']['battles'], %}
 					<div class="information-col">
 						<div class="information-col-item information-type">自行车</div>
-						<div class="information-col-item">{{ data['pvpTwoInfo']['battles'] }}</div>
-						<div class="information-col-item" style="color: {{ data['pvpTwoInfo']['winsData']['color'] }};">{{ data['pvpTwoInfo']['wins'] }}%</div>
-						<div class="information-col-item" style="color: {{ data['pvpTwoInfo']['pr']['color'] }};">{{ data['pvpTwoInfo']['pr']['value'] }}</div>
-						<div class="information-col-item" style="color: {{ data['pvpTwoInfo']['damageData']['color'] }};">{{ data['pvpTwoInfo']['damage'] }}</div>
-						<div class="information-col-item">{{ '%.2f' | format(data['pvpTwoInfo']['frags']) }}</div>
+						<div class="information-col-item">{{ data['pvpTwo']['battles'] }}</div>
+						<div class="information-col-item" style="color: {{ data['pvpTwo']['winsData']['color'] }};">{{
+							data['pvpTwo']['wins'] }}%</div>
+						<div class="information-col-item" style="color: {{ data['pvpTwo']['pr']['color'] }};">{{
+							data['pvpTwo']['pr']['value'] }}</div>
+						<div class="information-col-item" style="color: {{ data['pvpTwo']['damageData']['color'] }};">{{
+							data['pvpTwo']['damage'] }}</div>
+						<div class="information-col-item">{{ '%.2f' | format(data['pvpTwo']['frags']) }}</div>
 					</div>
 					{% endif %}
 
-
-					{% if data['pvpThreeInfo']['battles'] %}
+					{% if data['pvpThree']['battles'] %}
 					<div class="information-col">
 						<div class="information-col-item information-type">三轮车</div>
-						<div class="information-col-item">{{ data['pvpThreeInfo']['battles'] }}</div>
-						<div class="information-col-item" style="color: {{ data['pvpThreeInfo']['winsData']['color'] }};">{{ data['pvpThreeInfo']['wins'] }}%</div>
-						<div class="information-col-item" style="color: {{ data['pvpThreeInfo']['pr']['color'] }};">{{ data['pvpThreeInfo']['pr']['value'] }}</div>
-						<div class="information-col-item" style="color: {{ data['pvpThreeInfo']['damageData']['color'] }};">{{ data['pvpThreeInfo']['damage'] }}</div>
-						<div class="information-col-item">{{ '%.2f' | format(data['pvpThreeInfo']['frags']) }}</div>
+						<div class="information-col-item">{{ data['pvpThree']['battles'] }}</div>
+						<div class="information-col-item" style="color: {{ data['pvpThree']['winsData']['color'] }};">{{
+							data['pvpThree']['wins'] }}%</div>
+						<div class="information-col-item" style="color: {{ data['pvpThree']['pr']['color'] }};">{{
+							data['pvpThree']['pr']['value'] }}</div>
+						<div class="information-col-item" style="color: {{ data['pvpThree']['damageData']['color'] }};">
+							{{ data['pvpThree']['damage'] }}</div>
+						<div class="information-col-item">{{ '%.2f' | format(data['pvpThree']['frags']) }}</div>
 					</div>
 					{% endif %}
 
-
-					{% if data['rankInfo']['battles'] %}
+					{% if data['rankSolo']['battles'] %}
 					<div class="information-col">
 						<div class="information-col-item information-type">排位</div>
-						<div class="information-col-item">{{ data['rankInfo']['battles'] }}</div>
-						<div class="information-col-item" style="color: {{ data['rankInfo']['winsData']['color'] }};">{{ data['rankInfo']['wins'] }}%</div>
-						<div class="information-col-item" style="color: {{ data['rankInfo']['pr']['color'] }};">{{ data['rankInfo']['pr']['value'] }}</div>
-						<div class="information-col-item" style="color: {{ data['rankInfo']['damageData']['color'] }};">{{ data['rankInfo']['damage'] }}</div>
-						<div class="information-col-item">{{ '%.2f' | format(data['rankInfo']['frags']) }}</div>
+						<div class="information-col-item">{{ data['rankSolo']['battles'] }}</div>
+						<div class="information-col-item" style="color: {{ data['rankSolo']['winsData']['color'] }};">{{
+							data['rankSolo']['wins'] }}%</div>
+						<div class="information-col-item" style="color: {{ data['rankSolo']['pr']['color'] }};">{{
+							data['rankSolo']['pr']['value'] }}</div>
+						<div class="information-col-item" style="color: {{ data['rankSolo']['damageData']['color'] }};">
+							{{ data['rankSolo']['damage'] }}</div>
+						<div class="information-col-item">{{ '%.2f' | format(data['rankSolo']['frags']) }}</div>
 					</div>
 					{% endif %}
 
 				</div>
 
-				<div class="day-header">每日战绩</div>
-
-				<div class="day-body">
-					<div class="day-table-header">
-						<div class="day-col-item">类型</div>
-						<div class="day-col-item">场次</div>
-						<div class="day-col-item">胜率</div>
-						<div class="day-col-item">PR</div>
-						<div class="day-col-item">场均</div>
-						<div class="day-col-item">击杀</div>
-					</div>
-
-
-						<div class="data-item">
-							{% for eachShipData in data['shipData'] %}
-							    {% if eachShipData['shipInfo']['battles'] or eachShipData['rankSolo']['battles'] %}
-								<div class="date">{{ time.strftime('%Y-%m-%d',time.localtime(int(abs(eachShipData['recordDateTime']/1000)))) }}</div>
-									{% for each in eachShipData %}
-										{% for index,value in enumerate(['shipSolo','shipTwo','shipThree','rankSolo']) %}
-											{% if each|string == value and eachShipData[each]['battles'] %}
-											<div class="day-data">
-												<div class="day-col">
-													<div class="day-col-item" style="color: #606266;;">{{ ['单野','自行车','三轮车','排位'][index] }}</div>
-													<div class="day-col-item">{{ eachShipData[each]['battles'] }}</div>
-													<div class="day-col-item" style="color: {{ eachShipData[each]['winsData']['color'] }};">{{ eachShipData[each]['wins'] }}%</div>
-													<div class="day-col-item" style="color: {{ eachShipData[each]['pr']['color'] }};">{{ eachShipData[each]['pr']['value'] }}</div>
-													<div class="day-col-item" style="color: {{ eachShipData[each]['damageData']['color'] }};">{{ eachShipData[each]['damage'] }}</div>
-													<div class="day-col-item">{{ '%.2f' | format(eachShipData[each]['frags']) }}</div>
-												</div>
-											</div>
-											{% endif %}
-										{% endfor %}
-									{% endfor %}
-								{% endif %}
-							{% endfor %}
-						</div>
-
-					<div class="footer">
-						<p>©西行寺雨季&nbsp;&nbsp;©本心</p>
-						<p>https://github.com/benx1n/HikariBot</p>
-						<p>QQ频道搜索”yuyuko”即可使用稳定的腾讯官方机器人~</p>
-						<p>Design By 冷眠 H5 Converted By C1ystal</p>
-						<p>赞助鸣谢：男人们的定远号、Wishing、科长</p>
-					</div>
-
+				<div class="chart-box">
+					<div class="chart-bar"></div>
+					<div class="chart-pie"></div>
 				</div>
 
-
+				<div class="footer">
+					<p>©西行寺雨季&nbsp;&nbsp;©本心</p>
+					<p>https://github.com/benx1n/HikariBot</p>
+					<p>QQ频道搜索”yuyuko”即可使用稳定的腾讯官方机器人~</p>
+					<p>Design By 冷眠 H5 Converted By C1ystal</p>
+					<p>赞助鸣谢：科长、男人们的定远号、海上最速暴毙传说</p>
+				</div>
 
 			</div>
 		</div>
-	</body>
-	<script>
-		// PR条颜色动态变化
-		let bar_bg_width = document.querySelector('.pr-bar-bg').clientWidth;
-		let pr_number = document.querySelector('.pr-number').innerText;
-		pr_number = parseInt(pr_number);
-		if (pr_number == 0) {
-			document.querySelector(".pr-bar").style.backgroundColor = "#828282";
-			document.querySelector(".pr-text").innerText = "暂无数据";
-		} else if (pr_number < 750) {
-			document.querySelector(".pr-bar").style.backgroundColor = "#F44336";
-			document.querySelector(".pr-text").innerText = "还需努力";
-		} else if (pr_number < 1100) {
-			document.querySelector(".pr-bar").style.backgroundColor = "#FF9800";
-			document.querySelector(".pr-text").innerText = "低于平均";
-		} else if (pr_number < 1350) {
-			document.querySelector(".pr-bar").style.backgroundColor = "#FFC107";
-			document.querySelector(".pr-text").innerText = "平均水平";
-			document.querySelector(".pr-number").style.color = "#303133";
-		} else if (pr_number < 1550) {
-			document.querySelector(".pr-bar").style.backgroundColor = "#8BC34A";
-			document.querySelector(".pr-text").innerText = "好";
-		} else if (pr_number < 1750) {
-			document.querySelector(".pr-bar").style.backgroundColor = "#4CAF50";
-			document.querySelector(".pr-text").innerText = "很好";
-		} else if (pr_number < 2100) {
-			document.querySelector(".pr-bar").style.backgroundColor = "#00BCD4";
-			document.querySelector(".pr-text").innerText = "非常好";
-		} else if (pr_number < 2450) {
-			document.querySelector(".pr-bar").style.backgroundColor = "#9C27B0";
-			document.querySelector(".pr-text").innerText = "大佬水平";
-		} else {
-			document.querySelector(".pr-bar").style.backgroundColor = "#673AB7";
-			document.querySelector(".pr-text").innerText = "神佬水平";
-			pr_number = 2450; //防止pr条溢出
-		}
-
-		if (pr_number < 220 && pr_number > 0) {
-			pr_number = 220; //防止pr过低导致圆角异常
-		}
-		// PR条动态长度
-		let width = bar_bg_width * (pr_number / 2450);
-		document.querySelector('.pr-bar').style.width = width + "px";
-	</script>
-
-	<script>
-		// 服务器字体颜色自动填充
-		let server_name = document.querySelector(".server").innerText;
-		if (server_name == "亚服") {
-			document.querySelector(".server").style.color = "#92D050";
-		} else if (server_name == "国服") {
-			document.querySelector(".server").style.color = "#BF9000";
-		} else if (server_name == "欧服") {
-			document.querySelector(".server").style.color = "#009664";
-		} else if (server_name == "美服") {
-			document.querySelector(".server").style.color = "#6872C4";
-		} else if (server_name == "俄服") {
-			document.querySelector(".server").style.color = "#FF0000";
-		}
-	</script>
-
-	<script>
-		// 数据变化动态颜色填充
-		let change_avgdmg = document.querySelector(".change-avgdmg").innerText;
-		change_avgdmg = parseInt(change_avgdmg);
-
-		let change_win = document.querySelector(".change-win").innerText;
-		change_win = change_win.split("%", 1);
-		change_win = parseFloat(change_win);
-
-		let change_pr = document.querySelector(".change-pr").innerText;
-		change_pr = parseInt(change_pr);
-
-		if (change_avgdmg > 0) {
-			document.querySelector(".change-avgdmg").style.color = "#70AD47";
-		} else {
-			document.querySelector(".change-avgdmg").style.color = "#FF0000";
-		}
-
-		if (change_win > 0) {
-			document.querySelector(".change-win").style.color = "#70AD47";
-		} else {
-			document.querySelector(".change-win").style.color = "#FF0000";
-		}
-
-		if (change_pr > 0) {
-			document.querySelector(".change-pr").style.color = "#70AD47";
-		} else {
-			document.querySelector(".change-pr").style.color = "#FF0000";
-		}
-	</script>
-
-	<script>
-		let ship_level = document.querySelector(".ship-level").innerText;
-		let level_number = ["1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "11"];
-		let level_roma = ["I", "II", "III", "IV", "V", "VI", "VII", "VIII", "IX", "X", "★"];
-		let ship_level_roma = level_roma[level_number.indexOf(ship_level)]
-		document.querySelector(".ship-level").innerText = ship_level_roma;
-	</script>
-
-	<script>
-		let arr_information = document.getElementsByClassName('information-col');
-		for (let i = 0; i < arr_information.length; i++) {
-			if (i % 2 != 0 && i == (arr_information.length - 1)) {
-				arr_information[i].style.backgroundColor = "#E4E4E4";
-				arr_information[i].style.borderBottomLeftRadius = "16px";
-				arr_information[i].style.borderBottomRightRadius = "16px";
-			} else if (i % 2 != 0) {
-				arr_information[i].style.backgroundColor = "#E4E4E4";
+	</div>
+</body>
+{% if template_path and template_path/"echarts.js" %}
+<script src="file:\\{{template_path}}/echarts.js"></script>
+{% else %}
+<script src="https://cdn.jsdelivr.net/npm/echarts@5.3.3/dist/echarts.js"></script>
+{% endif %}
+<script>
+	window.onload = function () {
+		drawBarChart();
+		drawPieChart();
+	};
+
+	function drawBarChart() {
+		var barChart = echarts.init(document.querySelector('.chart-bar'));
+		var barOption = {
+			animation: false,
+			tooltip: {},
+			label: {
+				position: 'top',
+				show: true,
+				fontSize: '15',
+				color: '#303133',
+			},
+			xAxis: {
+				data: ['I', 'II', 'III', 'IV', 'V', 'VI', 'VII', 'VIII', 'IX', 'X', '★'],
+				axisLabel: {
+					align: 'center',
+					fontSize: '20',
+				}
+			},
+			yAxis: {
+				axisLabel: {
+					align: 'center',
+					fontSize: '20',
+				}
+			},
+			series: [{
+				name: '场次',
+				type: 'bar',
+				data: [
+					{{ data['battleCountAll']['1'] }},
+			{{ data['battleCountAll']['2'] }},
+			{{ data['battleCountAll']['3'] }
+	},
+	{ { data['battleCountAll']['4'] } },
+	{ { data['battleCountAll']['5'] } },
+	{ { data['battleCountAll']['6'] } },
+	{ { data['battleCountAll']['7'] } },
+	{ { data['battleCountAll']['8'] } },
+	{ { data['battleCountAll']['9'] } },
+	{ { data['battleCountAll']['10'] } },
+	{ { data['battleCountAll']['11'] } },
+					],
+	itemStyle: {
+		color: '#D6ECFB40',
+			borderWidth: 1,
+				borderType: 'solid',
+					borderColor: '#9FB8FF',
+						shadowColor: '#9FB8FF',
+							shadowBlur: 3
+	},
+				}]
+			};
+
+	barChart.setOption(barOption);
+		}
+
+	function drawPieChart() {
+		var pieChart = echarts.init(document.querySelector('.chart-pie'));
+		var pieOption = {
+			animation: false,
+			tooltip: {},
+			color: ["#FBE5D6", "#E2F0D9", "#F2E2E2", "#DAE3F3", "#D9FFFF"],
+			series: [
+				{
+					name: this.title,
+					type: 'pie',
+					selectedMode: 'single',
+					radius: ['30%', '80%'],
+					clockwise: false,
+					itemStyle: {
+						borderWidth: 5,
+						borderColor: '#F2F2F2'
+					},
+					label: {
+						position: 'inside',
+						formatter: '{b}\n{d}%',
+						fontSize: 20,
+						fontWeight: 'bold',
+					},
+					data: [
+						{ value: {{ data['type']['Battleship']['battles'] }}, name: 'BB' },
+			{ value: {{ data['type']['Cruiser']['battles'] }
+	}, name: 'CA' },
+	{ value: { { data['type']['Destroyer']['battles'] } }, name: 'DD' },
+	{ value: { { data['type']['AirCarrier']['battles'] } }, name: 'CV' },
+	{ value: { { data['type']['Submarine']['battles'] } }, name: 'SS' }
+			        ]
+			    }],
+	graphic: {
+		elements: [{
+			type: 'text',
+			left: 'center',
+			top: 'center',
+			style: {
+				text: '舰船\n场次',
+				fontSize: 35,
+				textAlign: 'center',
+				width: 30,
+				height: 30,
+				fill: 'darkgray'
 			}
+		}]
+	}
+			};
+
+	pieChart.setOption(pieOption);
+		}
+</script>
+
+<script>
+	// PR条颜色动态变化
+	let bar_bg_width = document.querySelector('.pr-bar-bg').clientWidth;
+	let pr_number = document.querySelector('.pr-number').innerText;
+	pr_number = parseInt(pr_number);
+	if (pr_number == 0) {
+		document.querySelector(".pr-bar").style.backgroundColor = "#828282";
+		document.querySelector(".pr-text").innerText = "暂无数据";
+	} else if (pr_number < 750) {
+		document.querySelector(".pr-bar").style.backgroundColor = "#F44336";
+		document.querySelector(".pr-text").innerText = "还需努力";
+	} else if (pr_number < 1100) {
+		document.querySelector(".pr-bar").style.backgroundColor = "#FF9800";
+		document.querySelector(".pr-text").innerText = "低于平均";
+	} else if (pr_number < 1350) {
+		document.querySelector(".pr-bar").style.backgroundColor = "#FFC107";
+		document.querySelector(".pr-text").innerText = "平均水平";
+		document.querySelector(".pr-number").style.color = "#303133";
+	} else if (pr_number < 1550) {
+		document.querySelector(".pr-bar").style.backgroundColor = "#8BC34A";
+		document.querySelector(".pr-text").innerText = "好";
+	} else if (pr_number < 1750) {
+		document.querySelector(".pr-bar").style.backgroundColor = "#4CAF50";
+		document.querySelector(".pr-text").innerText = "很好";
+	} else if (pr_number < 2100) {
+		document.querySelector(".pr-bar").style.backgroundColor = "#00BCD4";
+		document.querySelector(".pr-text").innerText = "非常好";
+	} else if (pr_number < 2450) {
+		document.querySelector(".pr-bar").style.backgroundColor = "#9C27B0";
+		document.querySelector(".pr-text").innerText = "大佬水平";
+	} else {
+		document.querySelector(".pr-bar").style.backgroundColor = "#673AB7";
+		document.querySelector(".pr-text").innerText = "神佬水平";
+		pr_number = 2450; //防止pr条溢出
+	}
+
+	if (pr_number < 220 && pr_number > 0) {
+		pr_number = 220; //防止pr过低导致圆角异常
+	}
+	// PR条动态长度
+	let width = bar_bg_width * (pr_number / 2450);
+	document.querySelector('.pr-bar').style.width = width + "px";
+</script>
+
+<script>
+	// 服务器字体颜色自动填充
+	let server_name = document.querySelector(".server").innerText;
+	if (server_name == "亚服") {
+		document.querySelector(".server").style.color = "#92D050";
+	} else if (server_name == "国服") {
+		document.querySelector(".server").style.color = "#BF9000";
+	} else if (server_name == "欧服") {
+		document.querySelector(".server").style.color = "#009664";
+	} else if (server_name == "美服") {
+		document.querySelector(".server").style.color = "#6872C4";
+	} else if (server_name == "俄服") {
+		document.querySelector(".server").style.color = "#FF0000";
+	}
+</script>
+
+<script>
+	// 数据变化动态颜色填充
+	let change_avgdmg = document.querySelector(".change-avgdmg").innerText;
+	change_avgdmg = parseInt(change_avgdmg);
+
+	let change_win = document.querySelector(".change-win").innerText;
+	change_win = change_win.split("%", 1);
+	change_win = parseFloat(change_win);
+
+	let change_pr = document.querySelector(".change-pr").innerText;
+	change_pr = parseInt(change_pr);
+
+	if (change_avgdmg > 0) {
+		document.querySelector(".change-avgdmg").style.color = "#70AD47";
+	} else {
+		document.querySelector(".change-avgdmg").style.color = "#FF0000";
+	}
+
+	if (change_win > 0) {
+		document.querySelector(".change-win").style.color = "#70AD47";
+	} else {
+		document.querySelector(".change-win").style.color = "#FF0000";
+	}
+
+	if (change_pr > 0) {
+		document.querySelector(".change-pr").style.color = "#70AD47";
+	} else {
+		document.querySelector(".change-pr").style.color = "#FF0000";
+	}
+</script>
+
+<script>
+	let arr_ship_data = document.getElementsByClassName('ship-data-col');
+	for (let i = 0; i < arr_ship_data.length; i++) {
+		if (i % 2 != 0 && i == (arr_ship_data.length - 1)) {
+			arr_ship_data[i].style.backgroundColor = "#E4E4E4";
+			arr_ship_data[i].style.borderBottomLeftRadius = "16px";
+			arr_ship_data[i].style.borderBottomRightRadius = "16px";
+		} else if (i % 2 != 0) {
+			arr_ship_data[i].style.backgroundColor = "#E4E4E4";
+		}
+	}
+</script>
+
+<script>
+	let arr_information = document.getElementsByClassName('information-col');
+	for (let i = 0; i < arr_information.length; i++) {
+		if (i % 2 != 0 && i == (arr_information.length - 1)) {
+			arr_information[i].style.backgroundColor = "#E4E4E4";
+			arr_information[i].style.borderBottomLeftRadius = "16px";
+			arr_information[i].style.borderBottomRightRadius = "16px";
+		} else if (i % 2 != 0) {
+			arr_information[i].style.backgroundColor = "#E4E4E4";
 		}
-	</script>
-</html>
+	}
+</script>
+
+</html>
```

#### html2text {}

```diff
@@ -1,117 +1,112 @@
-{% if data['clanInfo']['tag'] %}
-[{{ data['clanInfo']['tag'] }}]
+{% if data['userInfo']['clanInfo']['tag'] %}
+[{{ data['userInfo']['clanInfo']['tag'] }}]
 {% endif %}
-{{ data['userName'] }}
-{{ data['serverName'] }}
-{% if data['shipData'][0]['shipInfo']['shipInfo']['nameCn'] %}
-{{ data['shipData'][0]['shipInfo']['shipInfo']['level'] }}
-{% else %}
-{{ data['shipData'][0]['rankSolo']['shipInfo']['level'] }}
-{% endif %} {% if data['shipData'][0]['shipInfo']['shipInfo']['nameCn'] %}
-{{ data['shipData'][0]['shipInfo']['shipInfo']['nameCn'] }}
-{% else %}
-{{ data['shipData'][0]['rankSolo']['shipInfo']['nameCn'] }}
-{% endif %}
-'shipData'][0]['shipInfo']['shipInfo']['shipType'] == 'Destroyer' or data
-['shipData'][0]['rankSolo']['shipInfo']['shipType'] == 'Destroyer' %} "https://
-hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/
-icon_sunk_destroyer.png" {% elif data['shipData'][0]['shipInfo']['shipInfo']
-['shipType'] == 'Cruiser' or data['shipData'][0]['rankSolo']['shipInfo']
-['shipType'] == 'Cruiser' %} "https://hikari-resource.oss-cn-
-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_cruiser.png" {% elif data
-['shipData'][0]['shipInfo']['shipInfo']['shipType'] == 'Battleship' or data
-['shipData'][0]['rankSolo']['shipInfo']['shipType'] == 'Battleship' %} "https:/
-/hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/
-icon_sunk_battleship.png" {% elif data['shipData'][0]['shipInfo']['shipInfo']
-['shipType'] == 'AirCarrier' or data['shipData'][0]['rankSolo']['shipInfo']
-['shipType'] == 'AirCarrier' %} "https://hikari-resource.oss-cn-
-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_aircarrier.png" {% else %}
-"https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/
-icon_sunk_submarine.png" {% endif %} />
-{% if data['pvpInfo']['pr']['color'] and data['pvpInfo']['pr']['color'] !=
-'#828282' %} {{ data['pvpInfo']['pr']['value'] }}      {% else %} {{ data
-['rankInfo']['pr']['value'] }}      {% endif %}
-è®°å½æ¶é´ï¼{{ time.strftime('%Y-%m-%d %H:%M',time.localtime(int(abs(data
-['shipData'][0]['recordDateTime']/1000)))) }}â{{ time.strftime('%Y-%m-%d %H:
-%M',time.localtime(time.time())) }}
-{% if data['pvpInfo']['battles'] %}
+{{ data['userInfo']['userName'] }}
+{{ data['userInfo']['server'] }}
+{{ data['prInfo']['value'] }}    
+æåæææ¶é´ï¼{{ time.strftime('%Y-%m-%d %H:%M:%S',time.localtime(abs
+(data['battleTypeInfo'][0]['shipInfo']['lastBattleTime']))) }}
 åºæ¬¡
-{{ data['pvpInfo']['battles'] }}
+{{ data['battleTypeInfo'][0]['shipInfo']['battleInfo']['battle'] }}
 PR
-è¾ä¸å¨
-æä¸å¯ç¨
+è¾ä¸æ¬¡
+{{ '%+d' | format(data['dwpDataVO']['pr']) }}
 èç
-{{ data['pvpInfo']['wins'] }}%
+{{ data['pvp']['wins'] }}%
 åºå
-æä¸å¯ç¨
+{{ '%+d' | format(data['dwpDataVO']['damage']) }}
 èç
-æä¸å¯ç¨
+{{ '%+.2f' | format(data['dwpDataVO']['wins']) }}%
 åºå
-{{ data['pvpInfo']['damage'] }}
+{{ data['pvp']['damage'] }}
 å»æ
-{{ '%.2f' | format(data['pvpInfo']['frags']) }}
+{{ '%.2f' | format(data['pvp']['frags']) }}
+å½ä¸­
+{{ '%.2f' | format(data['pvp']['hit']) }}%
+è¹åªæ°æ®
+ç±»å
+åºæ¬¡
+èç
+PR
+åºå
 å½ä¸­
-{{ data['pvpInfo']['hit'] }}%
+{% if data['type']['Battleship']['battles'] %}
+æåè°
+{{ data['type']['Battleship']['battles'] }}
+{{ data['type']['Battleship']['wins'] }}%
+{{ data['type']['Battleship']['pr']['value'] }}
+{{ data['type']['Battleship']['damage'] }}
+{{ '%.2f' | format (data['type']['Battleship']['hit']) }}%
+{% endif %} {% if data['type']['Cruiser']['battles'] %}
+å·¡æ´è°
+{{ data['type']['Cruiser']['battles'] }}
+{{ data['type']['Cruiser']['wins'] }}%
+{{ data['type']['Cruiser']['pr']['value'] }}
+{{ data['type']['Cruiser']['damage'] }}
+{{ '%.2f' | format (data['type']['Cruiser']['hit']) }}%
+{% endif %} {% if data['type']['Destroyer']['battles'] %}
+é©±éè°
+{{ data['type']['Destroyer']['battles'] }}
+{{ data['type']['Destroyer']['wins'] }}%
+{{ data['type']['Destroyer']['pr']['value'] }}
+{{ data['type']['Destroyer']['damage'] }}
+{{ '%.2f' | format (data['type']['Destroyer']['hit']) }}%
+{% endif %} {% if data['type']['AirCarrier']['battles'] %}
+èªç©ºæ¯è°
+{{ data['type']['AirCarrier']['battles'] }}
+{{ data['type']['AirCarrier']['wins'] }}%
+{{ data['type']['AirCarrier']['pr']['value'] }}
+{{ data['type']['AirCarrier']['damage'] }}
+{{ '%.2f' | format (data['type']['AirCarrier']['hit']) }}%
+{% endif %} {% if data['type']['Submarine']['battles'] %}
+æ½è
+{{ data['type']['Submarine']['battles'] }}
+{{ data['type']['Submarine']['wins'] }}%
+{{ data['type']['Submarine']['pr']['value'] }}
+{{ data['type']['Submarine']['damage'] }}
+{{ '%.2f' | format (data['type']['Submarine']['hit']) }}%
 {% endif %}
 æ»ä½æç»©
 ç±»å
 åºæ¬¡
 èç
 PR
 åºå
 å»æ
-{% if data['pvpSoloInfo']['battles'] %}
+{% if data['pvpSolo']['battles'] %}
 åé
-{{ data['pvpSoloInfo']['battles'] }}
-{{ data['pvpSoloInfo']['wins'] }}%
-{{ data['pvpSoloInfo']['pr']['value'] }}
-{{ data['pvpSoloInfo']['damage'] }}
-{{ '%.2f' | format(data['pvpSoloInfo']['frags']) }}
-{% endif %} {% if data['pvpTwoInfo']['battles'] %}
+{{ data['pvpSolo']['battles'] }}
+{{ data['pvpSolo']['wins'] }}%
+{{ data['pvpSolo']['pr']['value'] }}
+{{ data['pvpSolo']['damage'] }}
+{{ '%.2f' | format(data['pvpSolo']['frags']) }}
+{% endif %} {% if data['pvpTwo']['battles'], %}
 èªè¡è½¦
-{{ data['pvpTwoInfo']['battles'] }}
-{{ data['pvpTwoInfo']['wins'] }}%
-{{ data['pvpTwoInfo']['pr']['value'] }}
-{{ data['pvpTwoInfo']['damage'] }}
-{{ '%.2f' | format(data['pvpTwoInfo']['frags']) }}
-{% endif %} {% if data['pvpThreeInfo']['battles'] %}
+{{ data['pvpTwo']['battles'] }}
+{{ data['pvpTwo']['wins'] }}%
+{{ data['pvpTwo']['pr']['value'] }}
+{{ data['pvpTwo']['damage'] }}
+{{ '%.2f' | format(data['pvpTwo']['frags']) }}
+{% endif %} {% if data['pvpThree']['battles'] %}
 ä¸è½®è½¦
-{{ data['pvpThreeInfo']['battles'] }}
-{{ data['pvpThreeInfo']['wins'] }}%
-{{ data['pvpThreeInfo']['pr']['value'] }}
-{{ data['pvpThreeInfo']['damage'] }}
-{{ '%.2f' | format(data['pvpThreeInfo']['frags']) }}
-{% endif %} {% if data['rankInfo']['battles'] %}
+{{ data['pvpThree']['battles'] }}
+{{ data['pvpThree']['wins'] }}%
+{{ data['pvpThree']['pr']['value'] }}
+{{ data['pvpThree']['damage'] }}
+{{ '%.2f' | format(data['pvpThree']['frags']) }}
+{% endif %} {% if data['rankSolo']['battles'] %}
 æä½
-{{ data['rankInfo']['battles'] }}
-{{ data['rankInfo']['wins'] }}%
-{{ data['rankInfo']['pr']['value'] }}
-{{ data['rankInfo']['damage'] }}
-{{ '%.2f' | format(data['rankInfo']['frags']) }}
+{{ data['rankSolo']['battles'] }}
+{{ data['rankSolo']['wins'] }}%
+{{ data['rankSolo']['pr']['value'] }}
+{{ data['rankSolo']['damage'] }}
+{{ '%.2f' | format(data['rankSolo']['frags']) }}
 {% endif %}
-æ¯æ¥æç»©
-ç±»å
-åºæ¬¡
-èç
-PR
-åºå
-å»æ
-{% for eachShipData in data['shipData'] %} {% if eachShipData['shipInfo']
-['battles'] or eachShipData['rankSolo']['battles'] %}
-{{ time.strftime('%Y-%m-%d',time.localtime(int(abs(eachShipData
-['recordDateTime']/1000)))) }}
-{% for each in eachShipData %} {% for index,value in enumerate(
-['shipSolo','shipTwo','shipThree','rankSolo']) %} {% if each|string == value
-and eachShipData[each]['battles'] %}
-{{ ['åé','èªè¡è½¦','ä¸è½®è½¦','æä½'][index] }}
-{{ eachShipData[each]['battles'] }}
-{{ eachShipData[each]['wins'] }}%
-{{ eachShipData[each]['pr']['value'] }}
-{{ eachShipData[each]['damage'] }}
-{{ '%.2f' | format(eachShipData[each]['frags']) }}
-{% endif %} {% endfor %} {% endfor %} {% endif %} {% endfor %}
 Â©è¥¿è¡å¯ºé¨å­£  Â©æ¬å¿
 https://github.com/benx1n/HikariBot
 QQé¢éæç´¢âyuyukoâå³å¯ä½¿ç¨ç¨³å®çè¾è®¯å®æ¹æºå¨äºº~
 Design By å·ç  H5 Converted By C1ystal
-èµå©é¸£è°¢ï¼ç·äººä»¬çå®è¿å·ãWishingãç§é¿
+èµå©é¸£è°¢ï¼ç§é¿ãç·äººä»¬çå®è¿å·ãæµ·ä¸æéæ´æ¯ä¼ è¯´
+{% if template_path and template_path/"echarts.js" %}
+ {% else %}
+ {% endif %}
```

### Comparing `hikari_core-0.1.5/hikari_core/Template/wws-sx.html` & `hikari_core-0.1.6/hikari_core/Template/wws-sx.html`

 * *Files 1% similar despite different names*

```diff
@@ -372,15 +372,15 @@
 				{% endif %}
 				
 				<div class="footer">
 					<p>©西行寺雨季&nbsp;&nbsp;©本心</p>
 					<p>https://github.com/benx1n/HikariBot</p>
 					<p>QQ频道搜索”yuyuko”即可使用稳定的腾讯官方机器人~</p>
 					<p>Design By 冷眠 H5 Converted By C1ystal</p>
-					<p>赞助鸣谢：男人们的定远号、Wishing、科长</p>
+					<p>赞助鸣谢：科长、男人们的定远号、海上最速暴毙传说</p>
 				</div>
 			</div>
 		</div>
 	</body>
 	<script>
 		// 服务器字体颜色自动填充
 		let server_name = document.querySelector(".server").innerText;
```

#### html2text {}

```diff
@@ -46,8 +46,8 @@
 {% else %}
 tipsï¼æ²¡åºè¿æ¸¯çè¹åªä¸ä¼è¢«ç»è®¡å¨å
 {% endif %}
 Â©è¥¿è¡å¯ºé¨å­£  Â©æ¬å¿
 https://github.com/benx1n/HikariBot
 QQé¢éæç´¢âyuyukoâå³å¯ä½¿ç¨ç¨³å®çè¾è®¯å®æ¹æºå¨äºº~
 Design By å·ç  H5 Converted By C1ystal
-èµå©é¸£è°¢ï¼ç·äººä»¬çå®è¿å·ãWishingãç§é¿
+èµå©é¸£è°¢ï¼ç§é¿ãç·äººä»¬çå®è¿å·ãæµ·ä¸æéæ´æ¯ä¼ è¯´
```

### Comparing `hikari_core-0.1.5/hikari_core/Template/wws-unban.html` & `hikari_core-0.1.6/hikari_core/Template/wws-unban.html`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 				<div class="ban-tip">未在官方封禁历史中匹配到该用户</div>
 			</div>
 			<div class="footer">
 				<p>©西行寺雨季&nbsp;&nbsp;©本心</p>
 				<p>https://github.com/benx1n/HikariBot</p>
 				<p>QQ频道搜索”yuyuko”即可使用稳定的腾讯官方机器人~</p>
 				<p>Design By 冷眠 H5 Converted By C1ystal</p>
-				<p>赞助鸣谢：男人们的定远号、Wishing、科长</p>
+				<p>赞助鸣谢：科长、男人们的定远号、海上最速暴毙传说</p>
 			</div>
 		</div>
 	</body>
 	
 	<script>
 		// 服务器字体颜色自动填充
 		let server_name = document.querySelector(".server").innerText;
```

#### html2text {}

```diff
@@ -13,8 +13,8 @@
 åè´£ç³æï¼æ¬é¡µé¢ææä¿¡æ¯åä¸ä½ä¸ºè¯å¤å°å·çè¯æ®ï¼ä¸æ¯æç¨äºé´æç­è¡ä¸ºï¼è¯·å¤§å®¶çæ§è®¨è®º
 å¯è½ç¬¦åæ¡ä»¶çåå²è®°å½
 æªå¨å®æ¹å°ç¦åå²ä¸­å¹éå°è¯¥ç¨æ·
 Â©è¥¿è¡å¯ºé¨å­£  Â©æ¬å¿
 https://github.com/benx1n/HikariBot
 QQé¢éæç´¢âyuyukoâå³å¯ä½¿ç¨ç¨³å®çè¾è®¯å®æ¹æºå¨äºº~
 Design By å·ç  H5 Converted By C1ystal
-èµå©é¸£è°¢ï¼ç·äººä»¬çå®è¿å·ãWishingãç§é¿
+èµå©é¸£è°¢ï¼ç§é¿ãç·äººä»¬çå®è¿å·ãæµ·ä¸æéæ´æ¯ä¼ è¯´
```

### Comparing `hikari_core-0.1.5/hikari_core/utils.py` & `hikari_core-0.1.6/hikari_core/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import gzip
 import hashlib
 import io
 import time
 import traceback
 from collections import defaultdict
 from datetime import datetime, timedelta
+from typing import List, Optional, Tuple
 
 import httpx
 import orjson
 import pytz
 from loguru import logger
 
 from .data_source import template_path
@@ -27,37 +28,65 @@
                         file.write(resp.content)
         print(f"success {time.time()}")
     except Exception:
         logger.error(traceback.format_exc())
         return
 
 
-async def match_keywords(match_list, Lists):
+async def match_keywords(match_list, Lists) -> Tuple[Optional[str], List]:
+    """字段列表匹配(仅匹配单个元素)
+
+    Args:
+        match_list (List): 待匹配列表
+        Lists (List): 匹配字符列表
+
+    Returns:
+        match_keywards (str/None):匹配到的字段
+        match_list (List): 去除匹配字符后的列表
+    """
     for List in Lists:
         for kw in List.keywords:
             for match_kw in match_list:
                 if match_kw == kw or match_kw.upper() == kw.upper() or match_kw.lower() == kw.lower():
                     match_list.remove(match_kw)
                     return List.match_keywords, match_list
     return None, match_list
 
 
-async def find_and_replace_keywords(match_list, Lists):
+async def find_and_replace_keywords(match_list, Lists) -> Tuple[Optional[str], List]:
+    """字段列表匹配(可匹配同元素内更小长度)
+
+    Args:
+        match_list (List): 待匹配列表
+        Lists (List): 匹配字符列表
+
+    Returns:
+        match_keywards (str/None):匹配到的字段
+        match_list (List): 去除匹配字符后的列表
+    """
     for List in Lists:
         for kw in List.keywords:
             for i, match_kw in enumerate(match_list):
                 if match_kw.find(kw) + 1:
                     match_list[i] = str(match_kw).replace(kw, "")
                     if match_list[i] == "":
                         match_list.remove("")
                     return List.match_keywords, match_list
     return None, match_list
 
 
-def encode_gzip(bytes):
+def encode_gzip(bytes) -> str:
+    """gzip压缩
+
+    Args:
+        bytes (bytes): 需要压缩的content
+
+    Returns:
+        str (str): 压缩后数据
+    """
     buf = io.BytesIO(bytes)
     gf = gzip.GzipFile(fileobj=buf)
     return gf.read().decode("utf-8")
 
 
 class FreqLimiter:
     def __init__(self, default_cd_seconds):
@@ -105,10 +134,18 @@
         resp = await client.get(url, timeout=None)
         content = resp.read()
         content = content.replace(b"\n", b"\r\n")
         with open(path, "wb") as f:
             f.write(content)
 
 
-async def byte2md5(bytes):
+async def byte2md5(bytes) -> str:
+    """bytes转为md5
+
+    Args:
+        bytes (bytes): 原始数据
+
+    Returns:
+        str (str): md5
+    """
     res = hashlib.md5(bytes).hexdigest()
     return res
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hikari_core-0.1.5/LICENSE` & `hikari_core-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.5/pyproject.toml` & `hikari_core-0.1.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hikari-core"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["benx1n <1119809439@qq.com>"]
 readme = "README.md"
 packages = [{include = "hikari_core"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -12,11 +12,12 @@
 orjson = "^3.8.11"
 asyncio = "^3.4.3"
 APScheduler = "^3.10.1"
 jinja2 = "^3.0.0"
 pydantic = "^1.10.7"
 playwright = ">=1.17.2"
 aiofiles = ">=0.8.0"
+beautifulsoup4 = "^4.11.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `hikari_core-0.1.5/PKG-INFO` & `hikari_core-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: hikari-core
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: benx1n
 Author-email: 1119809439@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: APScheduler (>=3.10.1,<4.0.0)
 Requires-Dist: aiofiles (>=0.8.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
+Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: httpx[http2] (>=0.24.0)
 Requires-Dist: jinja2 (>=3.0.0,<4.0.0)
 Requires-Dist: orjson (>=3.8.11,<4.0.0)
 Requires-Dist: playwright (>=1.17.2)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Description-Content-Type: text/markdown
```

