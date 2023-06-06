# Comparing `tmp/nonebot_plugin_multincm-0.3.5.tar.gz` & `tmp/nonebot_plugin_multincm-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_multincm-0.3.5.tar", last modified: Sun Jun  4 17:16:47 2023, max compression
+gzip compressed data, was "nonebot_plugin_multincm-0.3.6.tar", last modified: Tue Jun  6 16:39:43 2023, max compression
```

## Comparing `nonebot_plugin_multincm-0.3.5.tar` & `nonebot_plugin_multincm-0.3.6.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0     1069 2023-06-04 17:16:30.714776 nonebot_plugin_multincm-0.3.5/LICENSE
--rw-r--r--   0        0        0     8547 2023-06-04 17:16:30.714776 nonebot_plugin_multincm-0.3.5/README.md
--rw-r--r--   0        0        0     1816 2023-06-04 17:16:30.714776 nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/__init__.py
--rw-r--r--   0        0        0    12222 2023-06-04 17:16:30.714776 nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/__main__.py
--rw-r--r--   0        0        0      623 2023-06-04 17:16:30.714776 nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/config.py
--rw-r--r--   0        0        0      134 2023-06-04 17:16:30.714776 nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/const.py
--rw-r--r--   0        0        0     5556 2023-06-04 17:16:30.714776 nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/data_source.py
--rw-r--r--   0        0        0    11669 2023-06-04 17:16:30.718776 nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/draw.py
--rw-r--r--   0        0        0     2928 2023-06-04 17:16:30.718776 nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/lrc_parser.py
--rw-r--r--   0        0        0     2279 2023-06-04 17:16:30.718776 nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/msg_cache.py
--rw-r--r--   0        0        0   212591 2023-06-04 17:16:30.718776 nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/res/bg.jpg
--rw-r--r--   0        0        0     3007 2023-06-04 17:16:30.718776 nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/types.py
--rw-r--r--   0        0        0      851 2023-06-04 17:16:30.718776 nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/utils.py
--rw-r--r--   0        0        0      690 2023-06-04 17:16:47.143058 nonebot_plugin_multincm-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     9199 1970-01-01 00:00:00.000000 nonebot_plugin_multincm-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-06 16:39:29.466227 nonebot_plugin_multincm-0.3.6/LICENSE
+-rw-r--r--   0        0        0     9145 2023-06-06 16:39:29.470227 nonebot_plugin_multincm-0.3.6/README.md
+-rw-r--r--   0        0        0     1853 2023-06-06 16:39:29.470227 nonebot_plugin_multincm-0.3.6/nonebot_plugin_multincm/__init__.py
+-rw-r--r--   0        0        0    12234 2023-06-06 16:39:29.470227 nonebot_plugin_multincm-0.3.6/nonebot_plugin_multincm/__main__.py
+-rw-r--r--   0        0        0      711 2023-06-06 16:39:29.470227 nonebot_plugin_multincm-0.3.6/nonebot_plugin_multincm/config.py
+-rw-r--r--   0        0        0      134 2023-06-06 16:39:29.470227 nonebot_plugin_multincm-0.3.6/nonebot_plugin_multincm/const.py
+-rw-r--r--   0        0        0     5556 2023-06-06 16:39:29.470227 nonebot_plugin_multincm-0.3.6/nonebot_plugin_multincm/data_source.py
+-rw-r--r--   0        0        0    15315 2023-06-06 16:39:29.470227 nonebot_plugin_multincm-0.3.6/nonebot_plugin_multincm/draw.py
+-rw-r--r--   0        0        0     2928 2023-06-06 16:39:29.470227 nonebot_plugin_multincm-0.3.6/nonebot_plugin_multincm/lrc_parser.py
+-rw-r--r--   0        0        0     2279 2023-06-06 16:39:29.470227 nonebot_plugin_multincm-0.3.6/nonebot_plugin_multincm/msg_cache.py
+-rw-r--r--   0        0        0   212591 2023-06-06 16:39:29.470227 nonebot_plugin_multincm-0.3.6/nonebot_plugin_multincm/res/bg.jpg
+-rw-r--r--   0        0        0      577 2023-06-06 16:39:29.470227 nonebot_plugin_multincm-0.3.6/nonebot_plugin_multincm/res/lyric.html.jinja
+-rw-r--r--   0        0        0     2744 2023-06-06 16:39:29.470227 nonebot_plugin_multincm-0.3.6/nonebot_plugin_multincm/res/song_list.html.jinja
+-rw-r--r--   0        0        0     3007 2023-06-06 16:39:29.470227 nonebot_plugin_multincm-0.3.6/nonebot_plugin_multincm/types.py
+-rw-r--r--   0        0        0      851 2023-06-06 16:39:29.470227 nonebot_plugin_multincm-0.3.6/nonebot_plugin_multincm/utils.py
+-rw-r--r--   0        0        0      824 2023-06-06 16:39:43.782364 nonebot_plugin_multincm-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0    10001 1970-01-01 00:00:00.000000 nonebot_plugin_multincm-0.3.6/PKG-INFO
```

### Comparing `nonebot_plugin_multincm-0.3.5/LICENSE` & `nonebot_plugin_multincm-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.5/README.md` & `nonebot_plugin_multincm-0.3.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -132,28 +132,30 @@
 
 如果你安装了 [nonebot-plugin-ncm](https://github.com/kitUIN/nonebot-plugin-ncm)，本插件会与其共用同一个 Session，就可以不用填下面的账号密码了
 
 下面配置中，手机号登录 和 邮箱登录、明文密码 和 MD5 密码哈希 各选其一填写即可
 
 在 nonebot2 项目的 `.env` 文件中添加下表中的必填配置
 
-|          配置项          | 必填 | 默认值  |                               说明                                |
-| :----------------------: | :--: | :-----: | :---------------------------------------------------------------: |
-|       `NCM_CTCODE`       |  否  |  `86`   |                    手机号登录用，登录手机区号                     |
-|       `NCM_PHONE`        |  否  |   无    |                     手机号登录用，登录手机号                      |
-|       `NCM_EMAIL`        |  否  |   无    |                       邮箱登录用，登录邮箱                        |
-|      `NCM_PASSWORD`      |  否  |   无    |                帐号明文密码，邮箱登录时为邮箱密码                 |
-|   `NCM_PASSWORD_HASH`    |  否  |   无    |              帐号密码 MD5 哈希，邮箱登录时为邮箱密码              |
-|     `NCM_LIST_LIMIT`     |  否  |  `20`   |                      歌曲列表每页的最大数量                       |
-|     `NCM_LIST_FONT`      |  否  |   无    |                      渲染歌曲列表使用的字体                       |
-|    `NCM_MAX_NAME_LEN`    |  否  |  `600`  |              歌曲列表中歌名列的最大文本宽度（像素）               |
-|   `NCM_MAX_ARTIST_LEN`   |  否  |  `400`  |              歌曲列表中歌手列的最大文本宽度（像素）               |
-|   `NCM_MSG_CACHE_TIME`   |  否  | `3600`  | 缓存 Bot 已发送音乐卡片的音乐 ID 及 用户最近一次操作 的时长（秒） |
-|    `NCM_AUTO_RESOLVE`    |  否  | `False` |         当用户发送音乐链接时，是否自动解析并发送音乐卡片          |
-| `NCM_ILLEGAL_CMD_FINISH` |  否  | `False` |          当用户在点歌时输入了非法指令，是否直接退出点歌           |
+|          配置项          | 必填 |   默认值   |                               说明                                |
+| :----------------------: | :--: | :--------: | :---------------------------------------------------------------: |
+|       `NCM_CTCODE`       |  否  |    `86`    |                    手机号登录用，登录手机区号                     |
+|       `NCM_PHONE`        |  否  |     无     |                     手机号登录用，登录手机号                      |
+|       `NCM_EMAIL`        |  否  |     无     |                       邮箱登录用，登录邮箱                        |
+|      `NCM_PASSWORD`      |  否  |     无     |                帐号明文密码，邮箱登录时为邮箱密码                 |
+|   `NCM_PASSWORD_HASH`    |  否  |     无     |              帐号密码 MD5 哈希，邮箱登录时为邮箱密码              |
+|     `NCM_LIST_LIMIT`     |  否  |    `20`    |                      歌曲列表每页的最大数量                       |
+|     `NCM_LIST_FONT`      |  否  |     无     |                      渲染歌曲列表使用的字体                       |
+|    `NCM_MAX_NAME_LEN`    |  否  |   `600`    |              歌曲列表中歌名列的最大文本宽度（像素）               |
+|   `NCM_MAX_ARTIST_LEN`   |  否  |   `400`    |              歌曲列表中歌手列的最大文本宽度（像素）               |
+|   `NCM_MSG_CACHE_TIME`   |  否  |   `3600`   | 缓存 Bot 已发送音乐卡片的音乐 ID 及 用户最近一次操作 的时长（秒） |
+|    `NCM_AUTO_RESOLVE`    |  否  |  `False`   |         当用户发送音乐链接时，是否自动解析并发送音乐卡片          |
+| `NCM_ILLEGAL_CMD_FINISH` |  否  |  `False`   |          当用户在点歌时输入了非法指令，是否直接退出点歌           |
+|   `NCM_USE_PLAYWRIGHT`   |  否  |  `False`   |           是否使用 `playwright` 绘制歌曲列表与歌词图片            |
+|   `NCM_LRC_EMPTY_LINE`   |  否  | `--------` |                        填充歌词空行的字符                         |
 
 ## 🎉 使用
 
 ### 指令
 
 - 点歌 [歌曲名 / 音乐 ID]
   - 介绍：搜索歌曲。当输入音乐 ID 时会直接发送对应音乐
@@ -213,14 +215,23 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.3.6
+
+- 支持使用 `nonebot-plugin-htmlrender` (`playwright`) 渲染歌曲列表与歌词图片（默认不启用，如要启用需要自行安装 `nonebot-plugin-multincm[playwright]`）
+- 添加配置项 `NCM_USE_PLAYWRIGHT` 与 `NCM_LRC_EMPTY_LINE`
+
+### 0.3.5
+
+- 🎉 NoneBot 2.0 🚀
+
 ### 0.3.4
 
 - 修复分割线下会显示歌词翻译的问题
 
 ### 0.3.3
 
 - 新增配置项 `NCM_ILLEGAL_CMD_FINISH`
```

#### html2text {}

```diff
@@ -27,16 +27,16 @@
 "nonebot_plugin_multincm" ] ```  ## âï¸ éç½® å¦æä½ å®è£äº [nonebot-
 plugin-ncm](https://github.com/kitUIN/nonebot-plugin-
 ncm)ï¼æ¬æä»¶ä¼ä¸å¶å±ç¨åä¸ä¸ª
 Sessionï¼å°±å¯ä»¥ä¸ç¨å¡«ä¸é¢çè´¦å·å¯ç äº
 ä¸é¢éç½®ä¸­ï¼ææºå·ç»å½ å é®ç®±ç»å½ãææå¯ç  å MD5
 å¯ç åå¸ åéå¶ä¸å¡«åå³å¯ å¨ nonebot2 é¡¹ç®ç `.env`
 æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« | é»è®¤å¼ |
-è¯´æ | | :----------------------: | :--: | :-----: | :-----------------------
-----------------------------------------: | | `NCM_CTCODE` | å¦ | `86` |
+è¯´æ | | :----------------------: | :--: | :--------: | :--------------------
+-------------------------------------------: | | `NCM_CTCODE` | å¦ | `86` |
 ææºå·ç»å½ç¨ï¼ç»å½ææºåºå· | | `NCM_PHONE` | å¦ | æ  |
 ææºå·ç»å½ç¨ï¼ç»å½ææºå· | | `NCM_EMAIL` | å¦ | æ  |
 é®ç®±ç»å½ç¨ï¼ç»å½é®ç®± | | `NCM_PASSWORD` | å¦ | æ  |
 å¸å·ææå¯ç ï¼é®ç®±ç»å½æ¶ä¸ºé®ç®±å¯ç  | | `NCM_PASSWORD_HASH` |
 å¦ | æ  | å¸å·å¯ç  MD5 åå¸ï¼é®ç®±ç»å½æ¶ä¸ºé®ç®±å¯ç  | |
 `NCM_LIST_LIMIT` | å¦ | `20` | æ­æ²åè¡¨æ¯é¡µçæå¤§æ°é | |
 `NCM_LIST_FONT` | å¦ | æ  | æ¸²ææ­æ²åè¡¨ä½¿ç¨çå­ä½ | |
@@ -45,20 +45,23 @@
 `NCM_MAX_ARTIST_LEN` | å¦ | `400` |
 æ­æ²åè¡¨ä¸­æ­æåçæå¤§ææ¬å®½åº¦ï¼åç´ ï¼ | |
 `NCM_MSG_CACHE_TIME` | å¦ | `3600` | ç¼å­ Bot å·²åéé³ä¹å¡ççé³ä¹
 ID å ç¨æ·æè¿ä¸æ¬¡æä½ çæ¶é¿ï¼ç§ï¼ | | `NCM_AUTO_RESOLVE` | å¦
 | `False` |
 å½ç¨æ·åéé³ä¹é¾æ¥æ¶ï¼æ¯å¦èªå¨è§£æå¹¶åéé³ä¹å¡ç | |
 `NCM_ILLEGAL_CMD_FINISH` | å¦ | `False` |
-å½ç¨æ·å¨ç¹æ­æ¶è¾å¥äºéæ³æä»¤ï¼æ¯å¦ç´æ¥éåºç¹æ­ | ## ð
-ä½¿ç¨ ### æä»¤ - ç¹æ­ [æ­æ²å / é³ä¹ ID] -
-ä»ç»ï¼æç´¢æ­æ²ãå½è¾å¥é³ä¹ ID æ¶ä¼ç´æ¥åéå¯¹åºé³ä¹ -
-å«åï¼`ç½æäº`ã`wyy` - çµå° [æ­æ²å / èç® ID] -
-ä»ç»ï¼æç´¢çµå°èç®ãå½è¾å¥çµå° ID æ¶ä¼ç´æ¥åéå¯¹åºèç®
-- å«åï¼`å£°é³`ã`ç½æçµå°`ã`wydt`ã`wydj` - è§£æ [åå¤
+å½ç¨æ·å¨ç¹æ­æ¶è¾å¥äºéæ³æä»¤ï¼æ¯å¦ç´æ¥éåºç¹æ­ | |
+`NCM_USE_PLAYWRIGHT` | å¦ | `False` | æ¯å¦ä½¿ç¨ `playwright`
+ç»å¶æ­æ²åè¡¨ä¸æ­è¯å¾ç | | `NCM_LRC_EMPTY_LINE` | å¦ | `--------` |
+å¡«åæ­è¯ç©ºè¡çå­ç¬¦ | ## ð ä½¿ç¨ ### æä»¤ - ç¹æ­ [æ­æ²å /
+é³ä¹ ID] - ä»ç»ï¼æç´¢æ­æ²ãå½è¾å¥é³ä¹ ID
+æ¶ä¼ç´æ¥åéå¯¹åºé³ä¹ - å«åï¼`ç½æäº`ã`wyy` - çµå°
+[æ­æ²å / èç® ID] - ä»ç»ï¼æç´¢çµå°èç®ãå½è¾å¥çµå° ID
+æ¶ä¼ç´æ¥åéå¯¹åºèç® -
+å«åï¼`å£°é³`ã`ç½æçµå°`ã`wydt`ã`wydj` - è§£æ [åå¤
 é³ä¹å¡ç / é¾æ¥] - ä»ç»ï¼è·åè¯¥ é³ä¹ / çµå°èç®
 çæ­æ¾é¾æ¥å¹¶ä½¿ç¨èªå®ä¹å¡çåé -
 å«åï¼`resolve`ã`parse`ã`get` - æ­è¯ [åå¤ é³ä¹å¡ç / é¾æ¥] -
 ä»ç»ï¼è·åè¯¥é³ä¹çæ­è¯ï¼ä»¥å¾çå½¢å¼åé -
 å«åï¼`lrc`ã`lyric`ã`lyrics` - é¾æ¥ [åå¤ é³ä¹å¡ç] -
 ä»ç»ï¼è·å Bot åéçé³ä¹å¡ççç½æäºé¾æ¥ -
 å«åï¼`link`ã`url` ### Tip - ç¹å» Bot
@@ -73,15 +76,19 @@
 é¡¹ç®ä½¿ç¨çç½æäº API è°ç¨åº ### [Binaryify/NeteaseCloudMusicApi]
 (https://github.com/Binaryify/NeteaseCloudMusicApi) é¡¹ç®çµå°ç¸å³ API
 æ¥æº ### [MeetWq/pil-utils](https://github.com/MeetWq/pil-utils) è¶å¥½ç¨ç
 Pillow è¾å©åº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.3.4 -
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.3.6 - æ¯æä½¿ç¨ `nonebot-
+plugin-htmlrender` (`playwright`)
+æ¸²ææ­æ²åè¡¨ä¸æ­è¯å¾çï¼é»è®¤ä¸å¯ç¨ï¼å¦è¦å¯ç¨éè¦èªè¡å®è£
+`nonebot-plugin-multincm[playwright]`ï¼ - æ·»å éç½®é¡¹ `NCM_USE_PLAYWRIGHT`
+ä¸ `NCM_LRC_EMPTY_LINE` ### 0.3.5 - ð NoneBot 2.0 ð ### 0.3.4 -
 ä¿®å¤åå²çº¿ä¸ä¼æ¾ç¤ºæ­è¯ç¿»è¯çé®é¢ ### 0.3.3 - æ°å¢éç½®é¡¹
 `NCM_ILLEGAL_CMD_FINISH` - å¨æªå¯ç¨ `NCM_ILLEGAL_CMD_FINISH`
 æ¶è¾å¥éè¯¯æä»¤å°ä¼æç¤ºç¨æ·éåºç¹æ­ ### 0.3.2 - æ°å¢éç½®é¡¹
 `NCM_MSG_CACHE_TIME`ã`NCM_AUTO_RESOLVE` - è°æ´ç»å½æµç¨å°
 `driver.on_startup` ä¸­ ### 0.3.1 - ä¿®å¤çµå°ç¸å³ bug ### 0.3.0 -
 æ¯æçµå°èç®çè§£æä¸ç¹æ­ ### 0.2.5 - `è§£æ`ã`æ­è¯`ã`é¾æ¥`
 æä»¤å¯ä»¥ç´æ¥æ ¹æ® Bot åéçä¸ä¸ªé³ä¹å¡çä½åºååºäº -
```

### Comparing `nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/__init__.py` & `nonebot_plugin_multincm-0.3.6/nonebot_plugin_multincm/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from nonebot.plugin import PluginMetadata, require
 
 require("nonebot_plugin_apscheduler")
+require("nonebot_plugin_htmlrender")
 
 from . import __main__ as __main__  # noqa: E402
 from .config import ConfigModel  # noqa: E402
 
-__version__ = "0.3.5"
+__version__ = "0.3.6"
 __plugin_meta__ = PluginMetadata(
     name="MultiNCM",
     description="网易云多选点歌",
     usage=(
         "指令列表：\n"
         "▶ 点歌 [歌曲名 / 音乐 ID]\n"
         "    ▷ 介绍：搜索歌曲。当输入音乐 ID 时会直接发送对应音乐\n"
@@ -30,10 +31,10 @@
         "Tip：\n"
         "▶ 点击 Bot 发送的音乐卡片会跳转到音乐直链，可以直接下载\n"
         "▶ 使用需要回复音乐卡片的指令时，如果没有回复，会自动使用你触发发送的最近一个音乐卡片的信息"
     ),
     homepage="https://github.com/lgc-NB2Dev/nonebot-plugin-multincm",
     type="application",
     config=ConfigModel,
-    supported_adapters=["~onebot.v11"],
+    supported_adapters={"~onebot.v11"},
     extra={"License": "MIT", "Author": "student_2333"},
 )
```

### Comparing `nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/__main__.py` & `nonebot_plugin_multincm-0.3.6/nonebot_plugin_multincm/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,15 +236,15 @@
     cache[page] = res
     state["page_max"] = ceil(total_count / config.ncm_list_limit)
 
     if page == 1 and len(results) == 1:
         await get_cache_by_index(cache, 1)
 
     try:
-        pic = draw_search_res(res, page)
+        pic = await draw_search_res(res, page)
     except:
         logger.exception(f"绘制{calling}列表失败")
         await matcher.finish(f"绘制{calling}列表失败，请检查后台输出")
 
     return MessageSegment.image(pic)
 
 
@@ -404,15 +404,15 @@
         logger.exception("获取歌曲歌词失败")
         await matcher.finish("获取歌曲歌词失败，请检查后台输出")
 
     lrc = format_lrc(lrc_data)
     if not lrc:
         await matcher.finish("该歌曲没有歌词")
 
-    await matcher.finish(MessageSegment.image(str_to_pic(lrc)))
+    await matcher.finish(MessageSegment.image(await str_to_pic(lrc)))
 
 
 cmd_get_cache_link = on_command(
     "链接",
     aliases={"link", "url"},
     rule=music_msg_matcher_rule,
 )
```

### Comparing `nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/config.py` & `nonebot_plugin_multincm-0.3.6/nonebot_plugin_multincm/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,10 +13,12 @@
     ncm_list_limit: int = 20
     ncm_list_font: Optional[str] = None
     ncm_max_name_len: int = 600
     ncm_max_artist_len: int = 400
     ncm_msg_cache_time: int = 3600
     ncm_auto_resolve: bool = False
     ncm_illegal_cmd_finish: bool = False
+    ncm_use_playwright: bool = False
+    ncm_lrc_empty_line: Optional[str] = "--------"
 
 
 config: ConfigModel = ConfigModel.parse_obj(get_driver().config.dict())
```

### Comparing `nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/data_source.py` & `nonebot_plugin_multincm-0.3.6/nonebot_plugin_multincm/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/draw.py` & `nonebot_plugin_multincm-0.3.6/nonebot_plugin_multincm/draw.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,48 @@
 from dataclasses import dataclass
-from io import BytesIO
 from math import ceil
 from pathlib import Path
 from typing import List, Optional, Sequence, Tuple, Union, cast
 
+from nonebot import logger
 from pil_utils import BuildImage, Text2Image
+from pil_utils.fonts import Font
 from pil_utils.types import ColorType, HAlignType
 
-from nonebot_plugin_multincm.msg_cache import CALLING_MAP
-
 from . import lrc_parser
 from .config import config
+from .msg_cache import CALLING_MAP
 from .types import (
     Lyric,
     LyricData,
     SearchResult,
     SongSearchResult,
     User,
     VoiceSearchResult,
 )
 from .utils import format_alias, format_artists, format_time
 
-BACKGROUND = BuildImage.open(Path(__file__).parent / "res" / "bg.jpg")
+RES_DIR = Path(__file__).parent / "res"
+BACKGROUND = BuildImage.open(RES_DIR / "bg.jpg")
+
+if config.ncm_use_playwright:
+    import bbcode
+    from jinja2 import Template
+    from nonebot_plugin_htmlrender import get_new_page
+
+    SONG_LIST_TEMPLATE = Template(
+        (RES_DIR / "song_list.html.jinja").read_text(encoding="u8"),
+        enable_async=True,
+    )
+    LYRIC_TEMPLATE = Template(
+        (RES_DIR / "lyric.html.jinja").read_text(encoding="u8"),
+        enable_async=True,
+    )
+    BBCODE_PARSER = bbcode.Parser()
+    BBCODE_PARSER.install_default_formatters()
 
 
 @dataclass()
 class TableHead:
     name: str
     align: HAlignType = "left"
     min_width: Optional[int] = None
@@ -68,51 +85,52 @@
     # default left
     return 0
 
 
 def draw_table(
     heads: Sequence[Union[TableHead, str]],
     lines: Sequence[Sequence[str]],
-    fontsize: int = 30,
-    pic_padding: int = 2,
-    item_padding_w: int = 10,
-    item_padding_h: int = 15,
-    border_width: int = 3,
     border_radius: int = 15,
-    font_color: ColorType = (255, 255, 255, 255),
-    border_color: ColorType = (255, 255, 255, 100),
     **kwargs,
 ) -> BuildImage:
+    font_size = 30
+    pic_padding = 2
+    item_padding_w = 10
+    item_padding_h = 15
+    border_width = 3
+    font_color = (255, 255, 255, 255)
+    border_color = (255, 255, 255, 100)
+
     head_len = len(heads)
     for li in lines:
         if len(li) != head_len:
             raise ValueError("line length not match head length")
 
     line_len = len(lines)
     heads = [TableHead(x) if isinstance(x, str) else x for x in heads]
 
     line_texts: List[List[Text2Image]] = [
         [
             generate_line_text(
                 head,
                 f"[b]{head.name}[/b]",
-                fontsize=fontsize,
+                fontsize=font_size,
                 fill=font_color,
                 **kwargs,
             )
             for head in heads
         ],
     ]
     for line in lines:
         line_texts.append(
             [
                 generate_line_text(
                     heads[i],
                     x,
-                    fontsize=fontsize,
+                    fontsize=font_size,
                     fill=font_color,
                     **kwargs,
                 )
                 for i, x in enumerate(line)
             ],
         )
 
@@ -246,33 +264,28 @@
                 format_time(x.baseInfo.duration),
             ]
             for i, x in enumerate(res.resources)
         ],
     )
 
 
-def draw_search_res(res: SearchResult, page_num: int = 1) -> BytesIO:
+def draw_search_res_pil(
+    calling: str,
+    current_page: int,
+    max_page: int,
+    max_count: int,
+    heads: Sequence[TableHead],
+    lines: Sequence[Sequence[str]],
+) -> bytes:
     pic_padding = 50
     table_padding = 20
     table_border_radius = 15
 
-    is_song = isinstance(res, SongSearchResult)
-    index_offset = (page_num - 1) * config.ncm_list_limit
-    table = draw_table(
-        *(
-            get_song_search_res_table(res, index_offset)
-            if is_song
-            else get_voice_search_res_table(res, index_offset)
-        ),
-        border_radius=table_border_radius,
-    )
+    table = draw_table(heads, lines, border_radius=table_border_radius)
 
-    calling = CALLING_MAP["song" if is_song else "voice"]
-    max_count = res.songCount if is_song else res.totalCount
-    max_page = ceil(max_count / config.ncm_list_limit)
     title_txt = Text2Image.from_text(
         f"{calling}列表",
         80,
         weight="bold",
         fill=(255, 255, 255),
         fontname=config.ncm_list_font or "",
     )
@@ -280,15 +293,15 @@
         f"Tip：[b]发送序号[/b] 选择{calling}\n其他操作：[b]上一页[/b](P) | [b]下一页[/b](N) | [b]退出[/b](E)",
         30,
         align="center",
         fill=(255, 255, 255),
         fontname=config.ncm_list_font or "",
     )
     footer_txt = Text2Image.from_bbcode_text(
-        f"第 [b]{page_num}[/b] / [b]{max_page}[/b] 页 | 共 [b]{max_count}[/b] 首",
+        f"第 [b]{current_page}[/b] / [b]{max_page}[/b] 页 | 共 [b]{max_count}[/b] 首",
         30,
         align="center",
         fill=(255, 255, 255),
         fontname=config.ncm_list_font or "",
     )
 
     width = table.width + pic_padding * 2 + table_padding * 2
@@ -323,15 +336,90 @@
     y_offset += table_padding
 
     bg.paste(table, (pic_padding + table_padding, y_offset), alpha=True)
     y_offset += table.height + table_padding * 2
 
     footer_txt.draw_on_image(bg.image, ((width - footer_txt.width) // 2, y_offset))
 
-    return bg.save_jpg()
+    return bg.save_jpg().getvalue()
+
+
+def get_font_path_uri() -> Optional[str]:
+    font_path = config.ncm_list_font
+    if font_path:
+        if (path := Path(font_path)).exists():
+            return path.resolve().as_uri()
+        return Font.find(font_path).path.as_uri()
+    return None
+
+
+async def render_template(
+    template: "Template",
+    **kwargs,
+) -> bytes:
+    html_txt = await template.render_async(**kwargs)
+    logger.debug(html_txt)
+    async with get_new_page() as page:
+        await page.goto((Path(__file__).parent / "res").as_uri())
+        await page.set_content(html_txt, wait_until="networkidle")
+        main_elem = await page.query_selector(".main")
+        assert main_elem
+        return await main_elem.screenshot(type="jpeg")
+
+
+async def draw_search_res_playwright(
+    calling: str,
+    current_page: int,
+    max_page: int,
+    max_count: int,
+    heads: Sequence[TableHead],
+    lines: Sequence[Sequence[str]],
+) -> bytes:
+    for x in heads:
+        x.name = BBCODE_PARSER.format(x.name)
+    lines = [[BBCODE_PARSER.format(y) for y in x] for x in lines]
+
+    return await render_template(
+        SONG_LIST_TEMPLATE,
+        calling=calling,
+        current_page=current_page,
+        max_page=max_page,
+        max_count=max_count,
+        heads=heads,
+        lines=lines,
+        font_path=get_font_path_uri(),
+        enumerate=enumerate,
+    )
+
+
+async def draw_search_res(res: SearchResult, page_num: int = 1) -> bytes:
+    is_song = isinstance(res, SongSearchResult)
+    calling = CALLING_MAP["song" if is_song else "voice"]
+
+    index_offset = (page_num - 1) * config.ncm_list_limit
+    head, lines = (
+        get_song_search_res_table(res, index_offset)
+        if is_song
+        else get_voice_search_res_table(res, index_offset)
+    )
+
+    max_count = res.songCount if is_song else res.totalCount
+    max_page = ceil(max_count / config.ncm_list_limit)
+
+    if config.ncm_use_playwright:
+        return await draw_search_res_playwright(
+            calling,
+            page_num,
+            max_page,
+            max_count,
+            head,
+            lines,
+        )
+
+    return draw_search_res_pil(calling, page_num, max_page, max_count, head, lines)
 
 
 def format_lrc(lrc: LyricData) -> Optional[str]:
     def fmt_usr(usr: User) -> str:
         return f"{usr.nickname} [{usr.userid}]"
 
     raw = lrc.lrc
@@ -340,60 +428,101 @@
 
     lyrics = [
         lrc_parser.parse(x.lyric)
         for x in cast(List[Optional[Lyric]], [raw, lrc.romalrc, lrc.tlyric])
         if x
     ]
     lyrics = [x for x in lyrics if x]
+    empty_line = config.ncm_lrc_empty_line
 
     lines = []
     if not lyrics:
         lines.append("[i]该歌曲没有滚动歌词[/i]")
         lines.append("")
-        lines.append("--------")
+        lines.append(empty_line)
         lines.append("")
         lines.append(raw_lrc)
 
     else:
         if lyrics[0][-1].time >= 5940000:
             return None  # 纯音乐
 
         only_one = len(lyrics) == 1
-        for li in lrc_parser.merge(*lyrics):
+        for li in lrc_parser.merge(*lyrics, replace_empty_line=empty_line):
             if not only_one:
                 lines.append("")
             lines.append(f"[b]{li[0].lrc}[/b]")
             lines.extend([f"{x.lrc}" for x in li[1:]])
 
     if lrc.lyricUser or lrc.transUser:
         lines.append("")
-        lines.append("--------")
+        lines.append(empty_line)
         lines.append("")
 
         if usr := lrc.lyricUser:
             lines.append(f"歌词贡献者：{fmt_usr(usr)}")
         if usr := lrc.transUser:
             lines.append(f"翻译贡献者：{fmt_usr(usr)}")
 
     return "\n".join(lines).strip()
 
 
-def str_to_pic(
+def str_to_pic_pil(
     txt: str,
     padding: int = 20,
     font_color: ColorType = (241, 246, 249),
     bg_color: ColorType = (33, 42, 62),
-    **kwargs,
-) -> BytesIO:
+    font_size: int = 30,
+    text_align: HAlignType = "left",
+) -> bytes:
     txt2img = Text2Image.from_bbcode_text(
         txt,
         fontname=config.ncm_list_font or "",
         fill=font_color,
-        **kwargs,
+        fontsize=font_size,
+        align=text_align,
     )
     img = BuildImage.new(
         "RGBA",
         (txt2img.width + padding * 2, txt2img.height + padding * 2),
         bg_color,
     )
     txt2img.draw_on_image(img.image, (padding, padding))
-    return img.save_jpg()
+    return img.save_jpg().getvalue()
+
+
+async def str_to_pic_playwright(
+    txt: str,
+    padding: int = 20,
+    font_color: ColorType = (241, 246, 249),
+    bg_color: ColorType = (33, 42, 62),
+    font_size: int = 30,
+    text_align: HAlignType = "left",
+) -> bytes:
+    def color_type_to_css(clr: ColorType) -> str:
+        if isinstance(clr, tuple):
+            css_func = f"{'rgb' if len(clr) == 3 else 'rgba'}"
+            color_str = f"{', '.join(map(str, clr))}"
+            return f"{css_func}({color_str})"
+        return clr
+
+    return await render_template(
+        LYRIC_TEMPLATE,
+        font_path=get_font_path_uri(),
+        lrc=BBCODE_PARSER.format(txt),
+        padding=padding,
+        font_color=color_type_to_css(font_color),
+        bg_color=color_type_to_css(bg_color),
+        font_size=font_size,
+        text_align=text_align,
+    )
+
+
+async def str_to_pic(
+    txt: str,
+    padding: int = 20,
+    font_color: ColorType = (241, 246, 249),
+    bg_color: ColorType = (33, 42, 62),
+) -> bytes:
+    if config.ncm_use_playwright:
+        return await str_to_pic_playwright(txt, padding, font_color, bg_color)
+    return str_to_pic_pil(txt, padding, font_color, bg_color)
```

### Comparing `nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/lrc_parser.py` & `nonebot_plugin_multincm-0.3.6/nonebot_plugin_multincm/lrc_parser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/msg_cache.py` & `nonebot_plugin_multincm-0.3.6/nonebot_plugin_multincm/msg_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/res/bg.jpg` & `nonebot_plugin_multincm-0.3.6/nonebot_plugin_multincm/res/bg.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/types.py` & `nonebot_plugin_multincm-0.3.6/nonebot_plugin_multincm/types.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/utils.py` & `nonebot_plugin_multincm-0.3.6/nonebot_plugin_multincm/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.5/pyproject.toml` & `nonebot_plugin_multincm-0.3.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-multincm"
-version = "0.3.5"
+version = "0.3.6"
 description = "NCM Song Searcher"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.2.0",
@@ -20,14 +20,21 @@
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/lgc-NB2Dev/nonebot-plugin-multincm"
 
+[project.optional-dependencies]
+playwright = [
+    "nonebot-plugin-htmlrender>=0.2.0.3",
+    "jinja2>=3.1.2",
+    "bbcode>=1.1.0",
+]
+
 [tool.pdm.build]
 includes = []
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
```

### Comparing `nonebot_plugin_multincm-0.3.5/PKG-INFO` & `nonebot_plugin_multincm-0.3.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-multincm
-Version: 0.3.5
+Version: 0.3.6
 Summary: NCM Song Searcher
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Requires-Python: <4.0,>=3.8
 Requires-Dist: nonebot2>=2.0.0
 Requires-Dist: nonebot-adapter-onebot>=2.2.0
 Requires-Dist: pydantic>=1.10.4
 Requires-Dist: pil-utils>=0.1.7
 Requires-Dist: pyncm>=1.6.8.9.1
 Requires-Dist: typing-extensions>=4.5.0
 Requires-Dist: anyio>=3.6.2
 Requires-Dist: nonebot-plugin-apscheduler>=0.2.0
+Requires-Dist: nonebot-plugin-htmlrender>=0.2.0.3; extra == "playwright"
+Requires-Dist: jinja2>=3.1.2; extra == "playwright"
+Requires-Dist: bbcode>=1.1.0; extra == "playwright"
+Provides-Extra: playwright
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD031 MD033 MD036 MD041 -->
 
 <div align="center">
 
 <a href="https://v2.nonebot.dev/store">
@@ -151,28 +155,30 @@
 
 如果你安装了 [nonebot-plugin-ncm](https://github.com/kitUIN/nonebot-plugin-ncm)，本插件会与其共用同一个 Session，就可以不用填下面的账号密码了
 
 下面配置中，手机号登录 和 邮箱登录、明文密码 和 MD5 密码哈希 各选其一填写即可
 
 在 nonebot2 项目的 `.env` 文件中添加下表中的必填配置
 
-|          配置项          | 必填 | 默认值  |                               说明                                |
-| :----------------------: | :--: | :-----: | :---------------------------------------------------------------: |
-|       `NCM_CTCODE`       |  否  |  `86`   |                    手机号登录用，登录手机区号                     |
-|       `NCM_PHONE`        |  否  |   无    |                     手机号登录用，登录手机号                      |
-|       `NCM_EMAIL`        |  否  |   无    |                       邮箱登录用，登录邮箱                        |
-|      `NCM_PASSWORD`      |  否  |   无    |                帐号明文密码，邮箱登录时为邮箱密码                 |
-|   `NCM_PASSWORD_HASH`    |  否  |   无    |              帐号密码 MD5 哈希，邮箱登录时为邮箱密码              |
-|     `NCM_LIST_LIMIT`     |  否  |  `20`   |                      歌曲列表每页的最大数量                       |
-|     `NCM_LIST_FONT`      |  否  |   无    |                      渲染歌曲列表使用的字体                       |
-|    `NCM_MAX_NAME_LEN`    |  否  |  `600`  |              歌曲列表中歌名列的最大文本宽度（像素）               |
-|   `NCM_MAX_ARTIST_LEN`   |  否  |  `400`  |              歌曲列表中歌手列的最大文本宽度（像素）               |
-|   `NCM_MSG_CACHE_TIME`   |  否  | `3600`  | 缓存 Bot 已发送音乐卡片的音乐 ID 及 用户最近一次操作 的时长（秒） |
-|    `NCM_AUTO_RESOLVE`    |  否  | `False` |         当用户发送音乐链接时，是否自动解析并发送音乐卡片          |
-| `NCM_ILLEGAL_CMD_FINISH` |  否  | `False` |          当用户在点歌时输入了非法指令，是否直接退出点歌           |
+|          配置项          | 必填 |   默认值   |                               说明                                |
+| :----------------------: | :--: | :--------: | :---------------------------------------------------------------: |
+|       `NCM_CTCODE`       |  否  |    `86`    |                    手机号登录用，登录手机区号                     |
+|       `NCM_PHONE`        |  否  |     无     |                     手机号登录用，登录手机号                      |
+|       `NCM_EMAIL`        |  否  |     无     |                       邮箱登录用，登录邮箱                        |
+|      `NCM_PASSWORD`      |  否  |     无     |                帐号明文密码，邮箱登录时为邮箱密码                 |
+|   `NCM_PASSWORD_HASH`    |  否  |     无     |              帐号密码 MD5 哈希，邮箱登录时为邮箱密码              |
+|     `NCM_LIST_LIMIT`     |  否  |    `20`    |                      歌曲列表每页的最大数量                       |
+|     `NCM_LIST_FONT`      |  否  |     无     |                      渲染歌曲列表使用的字体                       |
+|    `NCM_MAX_NAME_LEN`    |  否  |   `600`    |              歌曲列表中歌名列的最大文本宽度（像素）               |
+|   `NCM_MAX_ARTIST_LEN`   |  否  |   `400`    |              歌曲列表中歌手列的最大文本宽度（像素）               |
+|   `NCM_MSG_CACHE_TIME`   |  否  |   `3600`   | 缓存 Bot 已发送音乐卡片的音乐 ID 及 用户最近一次操作 的时长（秒） |
+|    `NCM_AUTO_RESOLVE`    |  否  |  `False`   |         当用户发送音乐链接时，是否自动解析并发送音乐卡片          |
+| `NCM_ILLEGAL_CMD_FINISH` |  否  |  `False`   |          当用户在点歌时输入了非法指令，是否直接退出点歌           |
+|   `NCM_USE_PLAYWRIGHT`   |  否  |  `False`   |           是否使用 `playwright` 绘制歌曲列表与歌词图片            |
+|   `NCM_LRC_EMPTY_LINE`   |  否  | `--------` |                        填充歌词空行的字符                         |
 
 ## 🎉 使用
 
 ### 指令
 
 - 点歌 [歌曲名 / 音乐 ID]
   - 介绍：搜索歌曲。当输入音乐 ID 时会直接发送对应音乐
@@ -232,14 +238,23 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.3.6
+
+- 支持使用 `nonebot-plugin-htmlrender` (`playwright`) 渲染歌曲列表与歌词图片（默认不启用，如要启用需要自行安装 `nonebot-plugin-multincm[playwright]`）
+- 添加配置项 `NCM_USE_PLAYWRIGHT` 与 `NCM_LRC_EMPTY_LINE`
+
+### 0.3.5
+
+- 🎉 NoneBot 2.0 🚀
+
 ### 0.3.4
 
 - 修复分割线下会显示歌词翻译的问题
 
 ### 0.3.3
 
 - 新增配置项 `NCM_ILLEGAL_CMD_FINISH`
```

#### html2text {}

```diff
@@ -1,17 +1,19 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-multincm Version: 0.3.5 Summary: NCM
+Metadata-Version: 2.1 Name: nonebot-plugin-multincm Version: 0.3.6 Summary: NCM
 Song Searcher Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Author-Email: student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-multincm Requires-Python: <4.0,>=3.8 Requires-Dist:
 nonebot2>=2.0.0 Requires-Dist: nonebot-adapter-onebot>=2.2.0 Requires-Dist:
 pydantic>=1.10.4 Requires-Dist: pil-utils>=0.1.7 Requires-Dist:
 pyncm>=1.6.8.9.1 Requires-Dist: typing-extensions>=4.5.0 Requires-Dist:
-anyio>=3.6.2 Requires-Dist: nonebot-plugin-apscheduler>=0.2.0 Description-
-Content-Type: text/markdown
+anyio>=3.6.2 Requires-Dist: nonebot-plugin-apscheduler>=0.2.0 Requires-Dist:
+nonebot-plugin-htmlrender>=0.2.0.3; extra == "playwright" Requires-Dist:
+jinja2>=3.1.2; extra == "playwright" Requires-Dist: bbcode>=1.1.0; extra ==
+"playwright" Provides-Extra: playwright Description-Content-Type: text/markdown
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
    # NoneBot-Plugin-MultiNCM _â¨ ç½æäºå¤éç¹æ­ â¨_ [python] [pdm-
                              managed] [wakatime]
                        [license] [pypi] [pypi_download]
 ## ð ä»ç»
 ä¸ä¸ªç½æäºå¤éç¹æ­æä»¶ï¼å¯ä»¥ç¿»é¡µï¼å¯ä»¥ç»å½ç½æäºè´¦å·ç¹
@@ -37,16 +39,16 @@
 "nonebot_plugin_multincm" ] ```  ## âï¸ éç½® å¦æä½ å®è£äº [nonebot-
 plugin-ncm](https://github.com/kitUIN/nonebot-plugin-
 ncm)ï¼æ¬æä»¶ä¼ä¸å¶å±ç¨åä¸ä¸ª
 Sessionï¼å°±å¯ä»¥ä¸ç¨å¡«ä¸é¢çè´¦å·å¯ç äº
 ä¸é¢éç½®ä¸­ï¼ææºå·ç»å½ å é®ç®±ç»å½ãææå¯ç  å MD5
 å¯ç åå¸ åéå¶ä¸å¡«åå³å¯ å¨ nonebot2 é¡¹ç®ç `.env`
 æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« | é»è®¤å¼ |
-è¯´æ | | :----------------------: | :--: | :-----: | :-----------------------
-----------------------------------------: | | `NCM_CTCODE` | å¦ | `86` |
+è¯´æ | | :----------------------: | :--: | :--------: | :--------------------
+-------------------------------------------: | | `NCM_CTCODE` | å¦ | `86` |
 ææºå·ç»å½ç¨ï¼ç»å½ææºåºå· | | `NCM_PHONE` | å¦ | æ  |
 ææºå·ç»å½ç¨ï¼ç»å½ææºå· | | `NCM_EMAIL` | å¦ | æ  |
 é®ç®±ç»å½ç¨ï¼ç»å½é®ç®± | | `NCM_PASSWORD` | å¦ | æ  |
 å¸å·ææå¯ç ï¼é®ç®±ç»å½æ¶ä¸ºé®ç®±å¯ç  | | `NCM_PASSWORD_HASH` |
 å¦ | æ  | å¸å·å¯ç  MD5 åå¸ï¼é®ç®±ç»å½æ¶ä¸ºé®ç®±å¯ç  | |
 `NCM_LIST_LIMIT` | å¦ | `20` | æ­æ²åè¡¨æ¯é¡µçæå¤§æ°é | |
 `NCM_LIST_FONT` | å¦ | æ  | æ¸²ææ­æ²åè¡¨ä½¿ç¨çå­ä½ | |
@@ -55,20 +57,23 @@
 `NCM_MAX_ARTIST_LEN` | å¦ | `400` |
 æ­æ²åè¡¨ä¸­æ­æåçæå¤§ææ¬å®½åº¦ï¼åç´ ï¼ | |
 `NCM_MSG_CACHE_TIME` | å¦ | `3600` | ç¼å­ Bot å·²åéé³ä¹å¡ççé³ä¹
 ID å ç¨æ·æè¿ä¸æ¬¡æä½ çæ¶é¿ï¼ç§ï¼ | | `NCM_AUTO_RESOLVE` | å¦
 | `False` |
 å½ç¨æ·åéé³ä¹é¾æ¥æ¶ï¼æ¯å¦èªå¨è§£æå¹¶åéé³ä¹å¡ç | |
 `NCM_ILLEGAL_CMD_FINISH` | å¦ | `False` |
-å½ç¨æ·å¨ç¹æ­æ¶è¾å¥äºéæ³æä»¤ï¼æ¯å¦ç´æ¥éåºç¹æ­ | ## ð
-ä½¿ç¨ ### æä»¤ - ç¹æ­ [æ­æ²å / é³ä¹ ID] -
-ä»ç»ï¼æç´¢æ­æ²ãå½è¾å¥é³ä¹ ID æ¶ä¼ç´æ¥åéå¯¹åºé³ä¹ -
-å«åï¼`ç½æäº`ã`wyy` - çµå° [æ­æ²å / èç® ID] -
-ä»ç»ï¼æç´¢çµå°èç®ãå½è¾å¥çµå° ID æ¶ä¼ç´æ¥åéå¯¹åºèç®
-- å«åï¼`å£°é³`ã`ç½æçµå°`ã`wydt`ã`wydj` - è§£æ [åå¤
+å½ç¨æ·å¨ç¹æ­æ¶è¾å¥äºéæ³æä»¤ï¼æ¯å¦ç´æ¥éåºç¹æ­ | |
+`NCM_USE_PLAYWRIGHT` | å¦ | `False` | æ¯å¦ä½¿ç¨ `playwright`
+ç»å¶æ­æ²åè¡¨ä¸æ­è¯å¾ç | | `NCM_LRC_EMPTY_LINE` | å¦ | `--------` |
+å¡«åæ­è¯ç©ºè¡çå­ç¬¦ | ## ð ä½¿ç¨ ### æä»¤ - ç¹æ­ [æ­æ²å /
+é³ä¹ ID] - ä»ç»ï¼æç´¢æ­æ²ãå½è¾å¥é³ä¹ ID
+æ¶ä¼ç´æ¥åéå¯¹åºé³ä¹ - å«åï¼`ç½æäº`ã`wyy` - çµå°
+[æ­æ²å / èç® ID] - ä»ç»ï¼æç´¢çµå°èç®ãå½è¾å¥çµå° ID
+æ¶ä¼ç´æ¥åéå¯¹åºèç® -
+å«åï¼`å£°é³`ã`ç½æçµå°`ã`wydt`ã`wydj` - è§£æ [åå¤
 é³ä¹å¡ç / é¾æ¥] - ä»ç»ï¼è·åè¯¥ é³ä¹ / çµå°èç®
 çæ­æ¾é¾æ¥å¹¶ä½¿ç¨èªå®ä¹å¡çåé -
 å«åï¼`resolve`ã`parse`ã`get` - æ­è¯ [åå¤ é³ä¹å¡ç / é¾æ¥] -
 ä»ç»ï¼è·åè¯¥é³ä¹çæ­è¯ï¼ä»¥å¾çå½¢å¼åé -
 å«åï¼`lrc`ã`lyric`ã`lyrics` - é¾æ¥ [åå¤ é³ä¹å¡ç] -
 ä»ç»ï¼è·å Bot åéçé³ä¹å¡ççç½æäºé¾æ¥ -
 å«åï¼`link`ã`url` ### Tip - ç¹å» Bot
@@ -83,15 +88,19 @@
 é¡¹ç®ä½¿ç¨çç½æäº API è°ç¨åº ### [Binaryify/NeteaseCloudMusicApi]
 (https://github.com/Binaryify/NeteaseCloudMusicApi) é¡¹ç®çµå°ç¸å³ API
 æ¥æº ### [MeetWq/pil-utils](https://github.com/MeetWq/pil-utils) è¶å¥½ç¨ç
 Pillow è¾å©åº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.3.4 -
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.3.6 - æ¯æä½¿ç¨ `nonebot-
+plugin-htmlrender` (`playwright`)
+æ¸²ææ­æ²åè¡¨ä¸æ­è¯å¾çï¼é»è®¤ä¸å¯ç¨ï¼å¦è¦å¯ç¨éè¦èªè¡å®è£
+`nonebot-plugin-multincm[playwright]`ï¼ - æ·»å éç½®é¡¹ `NCM_USE_PLAYWRIGHT`
+ä¸ `NCM_LRC_EMPTY_LINE` ### 0.3.5 - ð NoneBot 2.0 ð ### 0.3.4 -
 ä¿®å¤åå²çº¿ä¸ä¼æ¾ç¤ºæ­è¯ç¿»è¯çé®é¢ ### 0.3.3 - æ°å¢éç½®é¡¹
 `NCM_ILLEGAL_CMD_FINISH` - å¨æªå¯ç¨ `NCM_ILLEGAL_CMD_FINISH`
 æ¶è¾å¥éè¯¯æä»¤å°ä¼æç¤ºç¨æ·éåºç¹æ­ ### 0.3.2 - æ°å¢éç½®é¡¹
 `NCM_MSG_CACHE_TIME`ã`NCM_AUTO_RESOLVE` - è°æ´ç»å½æµç¨å°
 `driver.on_startup` ä¸­ ### 0.3.1 - ä¿®å¤çµå°ç¸å³ bug ### 0.3.0 -
 æ¯æçµå°èç®çè§£æä¸ç¹æ­ ### 0.2.5 - `è§£æ`ã`æ­è¯`ã`é¾æ¥`
 æä»¤å¯ä»¥ç´æ¥æ ¹æ® Bot åéçä¸ä¸ªé³ä¹å¡çä½åºååºäº -
```

