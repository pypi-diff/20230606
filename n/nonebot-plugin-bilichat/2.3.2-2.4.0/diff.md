# Comparing `tmp/nonebot_plugin_bilichat-2.3.2.tar.gz` & `tmp/nonebot_plugin_bilichat-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-2.3.2.tar", last modified: Sun Jun  4 16:40:05 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-2.4.0.tar", last modified: Tue Jun  6 06:36:35 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-2.3.2.tar` & `nonebot_plugin_bilichat-2.4.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    34523 2023-06-04 16:39:57.745253 nonebot_plugin_bilichat-2.3.2/LICENSE
--rw-r--r--   0        0        0    12309 2023-06-04 16:39:57.745253 nonebot_plugin_bilichat-2.3.2/README.md
--rw-r--r--   0        0        0     8870 2023-06-04 16:39:57.753253 nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     4777 2023-06-04 16:39:57.753253 nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-06-04 16:39:57.753253 nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-06-04 16:39:57.753253 nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4806 2023-06-04 16:39:57.753253 nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      871 2023-06-04 16:39:57.753253 nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     6439 2023-06-04 16:39:57.753253 nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0     8900 2023-06-04 16:39:57.753253 nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3800 2023-06-04 16:39:57.753253 nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      399 2023-06-04 16:39:57.753253 nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-06-04 16:39:57.753253 nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     4102 2023-06-04 16:39:57.753253 nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      341 2023-06-04 16:39:57.753253 nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     2854 2023-06-04 16:39:57.753253 nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1127 2023-06-04 16:39:57.753253 nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0      387 2023-06-04 16:39:57.753253 nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/model/content.py
--rw-r--r--   0        0        0      503 2023-06-04 16:39:57.753253 nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0    27359 2023-06-04 16:39:57.757253 nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/model/newbing.py
--rw-r--r--   0        0        0      323 2023-06-04 16:39:57.757253 nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-06-04 16:39:57.757253 nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0   248896 2023-06-04 16:39:57.757253 nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/static/bing_apology.jpg
--rw-r--r--   0        0        0     1363 2023-06-04 16:39:57.757253 nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     5825 2023-06-04 16:39:57.757253 nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4916 2023-06-04 16:39:57.757253 nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2343 2023-06-04 16:39:57.757253 nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1448 2023-06-04 16:39:57.757253 nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     1780 2023-06-04 16:39:57.757253 nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1470 2023-06-04 16:40:05.913328 nonebot_plugin_bilichat-2.3.2/pyproject.toml
--rw-r--r--   0        0        0    13677 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-06 06:36:19.199038 nonebot_plugin_bilichat-2.4.0/LICENSE
+-rw-r--r--   0        0        0    12555 2023-06-06 06:36:19.199038 nonebot_plugin_bilichat-2.4.0/README.md
+-rw-r--r--   0        0        0     8870 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     4882 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4806 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      871 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     6439 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0     8900 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3800 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      399 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     4102 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      341 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     2854 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1127 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0      387 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/model/content.py
+-rw-r--r--   0        0        0      503 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0    27359 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/model/newbing.py
+-rw-r--r--   0        0        0      323 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0     1363 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     5904 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4916 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2343 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1448 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1780 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1499 2023-06-06 06:36:35.352341 nonebot_plugin_bilichat-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0    13996 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.4.0/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-2.3.2/LICENSE` & `nonebot_plugin_bilichat-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.2/README.md` & `nonebot_plugin_bilichat-2.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -182,29 +182,30 @@
 
 ### AI视频总结配置项
 
 开启此功能需要安装对应的依赖 `nonebot-plugin-bilichat[openai,newbing]`
 
 | 配置项 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
-| bilichat_newbing_cookie      | str       | None               | newbing的cookie文件路径(获取方式参考[这里](https://github.com/acheong08/EdgeGPT#getting-authentication-required)和[这里](https://github.com/Harry-Jing/nonebot-plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE)) , 若留空则禁用newbing总结 |
+| bilichat_newbing_cookie      | str       | None               | newbing的cookie文件路径, 填写 `no_login` 则不进行登录（可能有次数限制）, 若留空则禁用newbing总结 |
 | bilichat_newbing_token_limit | int       | 0                  | newbing请求的文本量上限, 0为无上限 |
 | bilichat_newbing_preprocess  | bool      | True               | 是否对newbing的返回值进行预处理, 以去除其中不想要的内容 |
 | bilichat_openai_token        | str       | None               | openai的apikey, 若留空则禁用openai总结 |
 | bilichat_openai_proxy        | str       | None               | 访问openai或newbing使用的代理地址 |
 | bilichat_openai_model        | str       | gpt-3.5-turbo-0301 | 使用的语言模型名称 |
 | bilichat_openai_token_limit  | int       | 3500               | 请求的文本量上限, 计算方式可参考[tiktoken](https://github.com/openai/tiktoken) |
 
 注:
 
 1. openai 与 newbing 目前均需求科学上网才能使用，国内服务器请务必填写 `bilichat_openai_proxy` 或全局透明代理
 2. 如果同时填写了 `bilichat_openai_token` 和 `bilichat_newbing_cookie`，则会使用 `newbing` 进行总结, 并在 `newbing` 总结失败时使用 `openai` 进行总结
-3. `newbing` 和 `openai` 均有缓存机制，同一视频在**获取到正常的总结内容后**不会重复发送请求，如需刷新请求内容可以手动删除对应视频的缓存文件或整个缓存文件夹
+3. `newbing` 和 `openai` 均有缓存机制，同一视频在**获取到正常的总结内容后**不会重复发送请求，如需刷新请求内容可以 [添加参数](#参数表) 或手动删除对应视频的缓存文件或整个缓存文件夹
 4. 经测试，目前 `newbing` 至少能总结 12000 字符以上的文本，推测 token 上限应为 `gpt-4-32k-0314` 的 `32200` token，但过长的内容易造成输出内容包含额外内容或总结失败，因此也建议设置一个合理的 token 上限 ~~（反正不要钱，要啥自行车）~~
 5. 由于 `newbing` 限制较大，也不如 `openai` 听话，且需要联网查询资料，因此使用体验并不如 chatgpt ~~（反正不要钱，要啥自行车）~~
+6. newbing cookie 文件获取方式参考[这里](https://github.com/acheong08/EdgeGPT#getting-authentication-required)和[这里](https://github.com/Harry-Jing/nonebot-plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE)。目前 newbing 已正式公布且无需登录也可使用，填写 `bilichat_newbing_cookie=no_login` 即可无 cookie 使用
 
 ## 🎉 使用
 
 直接发送视频(专栏)链接即可
 
 ### 参数表
```

#### html2text {}

```diff
@@ -68,41 +68,47 @@
 -:|:----:|:----:| | bilichat_word_cloud | bool | True |
 æ¯å¦å¼å¯è¯äºåè½ | æ³¨ï¼è¯äºåè½å¨ python3.11 ä¸­ç±äº
 `wordcloud` åå®è£å¤±è´¥ææ¶æ æ³å¯ç¨ï¼è¯·ä¸è¦å¨ 3.11
 ä¸­å¼å¯æ­¤åè½ ### AIè§é¢æ»ç»éç½®é¡¹
 å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-plugin-bilichat
 [openai,newbing]` | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:
 ----:|:----:| | bilichat_newbing_cookie | str | None |
-newbingçcookieæä»¶è·¯å¾(è·åæ¹å¼åè[è¿é](https://github.com/
-acheong08/EdgeGPT#getting-authentication-required)å[è¿é](https://
-github.com/Harry-Jing/nonebot-plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE)) ,
-è¥çç©ºåç¦ç¨newbingæ»ç» | | bilichat_newbing_token_limit | int | 0 |
-newbingè¯·æ±çææ¬éä¸é, 0ä¸ºæ ä¸é | | bilichat_newbing_preprocess
-| bool | True | æ¯å¦å¯¹newbingçè¿åå¼è¿è¡é¢å¤ç,
-ä»¥å»é¤å¶ä¸­ä¸æ³è¦çåå®¹ | | bilichat_openai_token | str | None |
-openaiçapikey, è¥çç©ºåç¦ç¨openaiæ»ç» | | bilichat_openai_proxy | str
-| None | è®¿é®openaiænewbingä½¿ç¨çä»£çå°å | | bilichat_openai_model
-| str | gpt-3.5-turbo-0301 | ä½¿ç¨çè¯­è¨æ¨¡ååç§° | |
+newbingçcookieæä»¶è·¯å¾, å¡«å `no_login`
+åä¸è¿è¡ç»å½ï¼å¯è½ææ¬¡æ°éå¶ï¼, è¥çç©ºåç¦ç¨newbingæ»ç»
+| | bilichat_newbing_token_limit | int | 0 | newbingè¯·æ±çææ¬éä¸é,
+0ä¸ºæ ä¸é | | bilichat_newbing_preprocess | bool | True |
+æ¯å¦å¯¹newbingçè¿åå¼è¿è¡é¢å¤ç, ä»¥å»é¤å¶ä¸­ä¸æ³è¦çåå®¹
+| | bilichat_openai_token | str | None | openaiçapikey,
+è¥çç©ºåç¦ç¨openaiæ»ç» | | bilichat_openai_proxy | str | None |
+è®¿é®openaiænewbingä½¿ç¨çä»£çå°å | | bilichat_openai_model | str |
+gpt-3.5-turbo-0301 | ä½¿ç¨çè¯­è¨æ¨¡ååç§° | |
 bilichat_openai_token_limit | int | 3500 | è¯·æ±çææ¬éä¸é,
 è®¡ç®æ¹å¼å¯åè[tiktoken](https://github.com/openai/tiktoken) | æ³¨: 1.
 openai ä¸ newbing
 ç®ååéæ±ç§å­¦ä¸ç½æè½ä½¿ç¨ï¼å½åæå¡å¨è¯·å¡å¿å¡«å
 `bilichat_openai_proxy` æå¨å±éæä»£ç 2. å¦æåæ¶å¡«åäº
 `bilichat_openai_token` å `bilichat_newbing_cookie`ï¼åä¼ä½¿ç¨ `newbing`
 è¿è¡æ»ç», å¹¶å¨ `newbing` æ»ç»å¤±è´¥æ¶ä½¿ç¨ `openai` è¿è¡æ»ç» 3.
 `newbing` å `openai`
-åæç¼å­æºå¶ï¼åä¸è§é¢å¨**è·åå°æ­£å¸¸çæ»ç»åå®¹å**ä¸ä¼éå¤åéè¯·æ±ï¼å¦éå·æ°è¯·æ±åå®¹å¯ä»¥æå¨å é¤å¯¹åºè§é¢çç¼å­æä»¶ææ´ä¸ªç¼å­æä»¶å¤¹
-4. ç»æµè¯ï¼ç®å `newbing` è³å°è½æ»ç» 12000
+åæç¼å­æºå¶ï¼åä¸è§é¢å¨**è·åå°æ­£å¸¸çæ»ç»åå®¹å**ä¸ä¼éå¤åéè¯·æ±ï¼å¦éå·æ°è¯·æ±åå®¹å¯ä»¥
+[æ·»å åæ°](#åæ°è¡¨)
+ææå¨å é¤å¯¹åºè§é¢çç¼å­æä»¶ææ´ä¸ªç¼å­æä»¶å¤¹ 4.
+ç»æµè¯ï¼ç®å `newbing` è³å°è½æ»ç» 12000
 å­ç¬¦ä»¥ä¸çææ¬ï¼æ¨æµ token ä¸éåºä¸º `gpt-4-32k-0314` ç `32200`
 tokenï¼ä½è¿é¿çåå®¹æé æè¾åºåå®¹åå«é¢å¤åå®¹ææ»ç»å¤±è´¥ï¼å æ­¤ä¹å»ºè®®è®¾ç½®ä¸ä¸ªåçç
 token ä¸é ~~ï¼åæ­£ä¸è¦é±ï¼è¦å¥èªè¡è½¦ï¼~~ 5. ç±äº `newbing`
 éå¶è¾å¤§ï¼ä¹ä¸å¦ `openai`
 å¬è¯ï¼ä¸éè¦èç½æ¥è¯¢èµæï¼å æ­¤ä½¿ç¨ä½éªå¹¶ä¸å¦ chatgpt
-~~ï¼åæ­£ä¸è¦é±ï¼è¦å¥èªè¡è½¦ï¼~~ ## ð ä½¿ç¨ ç´æ¥åéè§é¢
-(ä¸æ )é¾æ¥å³å¯ ### åæ°è¡¨
+~~ï¼åæ­£ä¸è¦é±ï¼è¦å¥èªè¡è½¦ï¼~~ 6. newbing cookie
+æä»¶è·åæ¹å¼åè[è¿é](https://github.com/acheong08/EdgeGPT#getting-
+authentication-required)å[è¿é](https://github.com/Harry-Jing/nonebot-
+plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE)ãç®å newbing
+å·²æ­£å¼å¬å¸ä¸æ éç»å½ä¹å¯ä½¿ç¨ï¼å¡«å
+`bilichat_newbing_cookie=no_login` å³å¯æ  cookie ä½¿ç¨ ## ð ä½¿ç¨
+ç´æ¥åéè§é¢(ä¸æ )é¾æ¥å³å¯ ### åæ°è¡¨
 å¨åéè§é¢æ¶ï¼å¯ä»¥é¢å¤æ·»å ä»¥ä¸ç±»ä¼¼ shell
 æä»¤çåæ°ï¼è¿èå¯¹è§£ææµç¨è¿è¡è°æ´ãä¾å¦ ```shell
 BV12v4y1E7NT --refresh BV12v4y1E7NT -r # å¯ä»¥ä½¿ç¨ç®å BV12v4y1E7NT -r --
 no-cache # å¯ä»¥å¤ä¸ªåæ°æ··ç¨ -r BV12v4y1E7NT -n #
 è½ç¶ä¸å»ºè®®ï¼ä½ç¡®å®å¯ä»¥æåæ°æ¾åé¢ ``` | æä»¤ | ç®å |
 è¯´æ | |:-----:|:----:|:----:| | --no-cache | -n | æ¬æ¬¡æ»ç»ç¦ç¨ç¼å­
 (ä¸ä¼å½±åå·²å­å¨çç¼å­æä»¶) | | --refresh | -r |
```

### Comparing `nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -106,14 +106,17 @@
                 json.loads(Path(v).read_text("utf-8"))
             except Exception as e:
                 raise ValueError("Config bilichat_newbing_cookie got a problem occurred") from e
 
         elif Path(v).is_dir():
             raise ValueError(f"Config bilichat_newbing_cookie requires a file, but {v} is a folder")
 
+        elif v == "no_login":
+            logger.info("Using newbing summary without a cookie")
+        
         else:
             raise ValueError(f"Path {v} is not recognized")
 
         return v
 
     @validator("bilichat_word_cloud", always=True)
     def check_pypackage_wordcloud(cls, v):
```

### Comparing `nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/model/newbing.py` & `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/model/newbing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/static/bing_apology.jpg` & `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/static/bing_apology.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/summary/__init__.py` & `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,19 @@
     AbortError,
     BingChatResponseException,
 )
 from ..model.newbing import BingChatResponse
 from ..optional import capture_exception  # type: ignore
 from .text_to_image import rich_text2image
 
-cookies = json.loads(Path(plugin_config.bilichat_newbing_cookie).read_text("utf-8"))  # type: ignore
+cookies = (
+    {}
+    if plugin_config.bilichat_newbing_cookie == "no_login"
+    else json.loads(Path(plugin_config.bilichat_newbing_cookie).read_text("utf-8"))  # type: ignore
+)
 logger.info("Try init bing chatbot")
 init = False
 for count in range(5):
     try:
         bot = Chatbot(cookies=cookies, proxy=plugin_config.bilichat_openai_proxy)  # type: ignore
         logger.success("Bing chatbot init success")
         init = True
```

### Comparing `nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/summary/text_to_image.py` & `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/summary/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.2/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.2/pyproject.toml` & `nonebot_plugin_bilichat-2.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -18,22 +18,21 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "2.3.2"
+version = "2.4.0"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
-    "httpx>=0.23.3",
     "bilireq>=0.2.4",
     "qrcode>=7.4.2",
     "pillow>=9.5.0",
     "lxml>=4.9.2",
     "nonebot-plugin-localstore>=0.4.1",
     "nonebot-adapter-onebot>=2.2.2",
     "nonebot-plugin-segbuilder>=0.2.0",
@@ -54,23 +53,25 @@
     "wordcloud>=1.8.2.2",
 ]
 openai = [
     "tiktoken-async>=0.3.2",
     "minidynamicrender>=1.1.9",
 ]
 newbing = [
-    "EdgeGPT>=0.1.22.1",
+    "EdgeGPT>=0.1.22.1,<0.9.0",
     "minidynamicrender>=1.1.9",
+    "setuptools",
 ]
 all = [
     "jieba>=0.42.1",
     "wordcloud>=1.8.2.2",
     "tiktoken-async>=0.3.2",
-    "EdgeGPT>=0.1.22.1",
+    "EdgeGPT>=0.1.22.1,<0.9.0",
     "minidynamicrender>=1.1.9",
+    "setuptools",
 ]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `nonebot_plugin_bilichat-2.3.2/PKG-INFO` & `nonebot_plugin_bilichat-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 2.3.2
+Version: 2.4.0
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
-Requires-Dist: httpx>=0.23.3
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2
 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot-adapter-onebot>=2.2.2
 Requires-Dist: nonebot-plugin-segbuilder>=0.2.0
 Requires-Dist: nonebot2>=2.0.0
 Requires-Dist: nonebot-plugin-sentry>=0.2.2; extra == "extra"
 Requires-Dist: jieba>=0.42.1; extra == "wordcloud"
 Requires-Dist: wordcloud>=1.8.2.2; extra == "wordcloud"
 Requires-Dist: tiktoken-async>=0.3.2; extra == "openai"
 Requires-Dist: minidynamicrender>=1.1.9; extra == "openai"
-Requires-Dist: EdgeGPT>=0.1.22.1; extra == "newbing"
+Requires-Dist: EdgeGPT<0.9.0,>=0.1.22.1; extra == "newbing"
 Requires-Dist: minidynamicrender>=1.1.9; extra == "newbing"
+Requires-Dist: setuptools; extra == "newbing"
 Requires-Dist: jieba>=0.42.1; extra == "all"
 Requires-Dist: wordcloud>=1.8.2.2; extra == "all"
 Requires-Dist: tiktoken-async>=0.3.2; extra == "all"
-Requires-Dist: EdgeGPT>=0.1.22.1; extra == "all"
+Requires-Dist: EdgeGPT<0.9.0,>=0.1.22.1; extra == "all"
 Requires-Dist: minidynamicrender>=1.1.9; extra == "all"
+Requires-Dist: setuptools; extra == "all"
 Provides-Extra: extra
 Provides-Extra: wordcloud
 Provides-Extra: openai
 Provides-Extra: newbing
 Provides-Extra: all
 Description-Content-Type: text/markdown
 
@@ -217,29 +218,30 @@
 
 ### AI视频总结配置项
 
 开启此功能需要安装对应的依赖 `nonebot-plugin-bilichat[openai,newbing]`
 
 | 配置项 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
-| bilichat_newbing_cookie      | str       | None               | newbing的cookie文件路径(获取方式参考[这里](https://github.com/acheong08/EdgeGPT#getting-authentication-required)和[这里](https://github.com/Harry-Jing/nonebot-plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE)) , 若留空则禁用newbing总结 |
+| bilichat_newbing_cookie      | str       | None               | newbing的cookie文件路径, 填写 `no_login` 则不进行登录（可能有次数限制）, 若留空则禁用newbing总结 |
 | bilichat_newbing_token_limit | int       | 0                  | newbing请求的文本量上限, 0为无上限 |
 | bilichat_newbing_preprocess  | bool      | True               | 是否对newbing的返回值进行预处理, 以去除其中不想要的内容 |
 | bilichat_openai_token        | str       | None               | openai的apikey, 若留空则禁用openai总结 |
 | bilichat_openai_proxy        | str       | None               | 访问openai或newbing使用的代理地址 |
 | bilichat_openai_model        | str       | gpt-3.5-turbo-0301 | 使用的语言模型名称 |
 | bilichat_openai_token_limit  | int       | 3500               | 请求的文本量上限, 计算方式可参考[tiktoken](https://github.com/openai/tiktoken) |
 
 注:
 
 1. openai 与 newbing 目前均需求科学上网才能使用，国内服务器请务必填写 `bilichat_openai_proxy` 或全局透明代理
 2. 如果同时填写了 `bilichat_openai_token` 和 `bilichat_newbing_cookie`，则会使用 `newbing` 进行总结, 并在 `newbing` 总结失败时使用 `openai` 进行总结
-3. `newbing` 和 `openai` 均有缓存机制，同一视频在**获取到正常的总结内容后**不会重复发送请求，如需刷新请求内容可以手动删除对应视频的缓存文件或整个缓存文件夹
+3. `newbing` 和 `openai` 均有缓存机制，同一视频在**获取到正常的总结内容后**不会重复发送请求，如需刷新请求内容可以 [添加参数](#参数表) 或手动删除对应视频的缓存文件或整个缓存文件夹
 4. 经测试，目前 `newbing` 至少能总结 12000 字符以上的文本，推测 token 上限应为 `gpt-4-32k-0314` 的 `32200` token，但过长的内容易造成输出内容包含额外内容或总结失败，因此也建议设置一个合理的 token 上限 ~~（反正不要钱，要啥自行车）~~
 5. 由于 `newbing` 限制较大，也不如 `openai` 听话，且需要联网查询资料，因此使用体验并不如 chatgpt ~~（反正不要钱，要啥自行车）~~
+6. newbing cookie 文件获取方式参考[这里](https://github.com/acheong08/EdgeGPT#getting-authentication-required)和[这里](https://github.com/Harry-Jing/nonebot-plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE)。目前 newbing 已正式公布且无需登录也可使用，填写 `bilichat_newbing_cookie=no_login` 即可无 cookie 使用
 
 ## 🎉 使用
 
 直接发送视频(专栏)链接即可
 
 ### 参数表
```

#### html2text {}

```diff
@@ -1,26 +1,28 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.3.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.4.0 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
-httpx>=0.23.3 Requires-Dist: bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2
-Requires-Dist: pillow>=9.5.0 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-
-plugin-localstore>=0.4.1 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-
-Dist: nonebot-plugin-segbuilder>=0.2.0 Requires-Dist: nonebot2>=2.0.0 Requires-
-Dist: nonebot-plugin-sentry>=0.2.2; extra == "extra" Requires-Dist:
-jieba>=0.42.1; extra == "wordcloud" Requires-Dist: wordcloud>=1.8.2.2; extra ==
-"wordcloud" Requires-Dist: tiktoken-async>=0.3.2; extra == "openai" Requires-
-Dist: minidynamicrender>=1.1.9; extra == "openai" Requires-Dist:
-EdgeGPT>=0.1.22.1; extra == "newbing" Requires-Dist: minidynamicrender>=1.1.9;
-extra == "newbing" Requires-Dist: jieba>=0.42.1; extra == "all" Requires-Dist:
+bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2 Requires-Dist: pillow>=9.5.0
+Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-plugin-localstore>=0.4.1
+Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-Dist: nonebot-plugin-
+segbuilder>=0.2.0 Requires-Dist: nonebot2>=2.0.0 Requires-Dist: nonebot-plugin-
+sentry>=0.2.2; extra == "extra" Requires-Dist: jieba>=0.42.1; extra ==
+"wordcloud" Requires-Dist: wordcloud>=1.8.2.2; extra == "wordcloud" Requires-
+Dist: tiktoken-async>=0.3.2; extra == "openai" Requires-Dist:
+minidynamicrender>=1.1.9; extra == "openai" Requires-Dist:
+EdgeGPT<0.9.0,>=0.1.22.1; extra == "newbing" Requires-Dist:
+minidynamicrender>=1.1.9; extra == "newbing" Requires-Dist: setuptools; extra
+== "newbing" Requires-Dist: jieba>=0.42.1; extra == "all" Requires-Dist:
 wordcloud>=1.8.2.2; extra == "all" Requires-Dist: tiktoken-async>=0.3.2; extra
-== "all" Requires-Dist: EdgeGPT>=0.1.22.1; extra == "all" Requires-Dist:
-minidynamicrender>=1.1.9; extra == "all" Provides-Extra: extra Provides-Extra:
-wordcloud Provides-Extra: openai Provides-Extra: newbing Provides-Extra: all
-Description-Content-Type: text/markdown
+== "all" Requires-Dist: EdgeGPT<0.9.0,>=0.1.22.1; extra == "all" Requires-Dist:
+minidynamicrender>=1.1.9; extra == "all" Requires-Dist: setuptools; extra ==
+"all" Provides-Extra: extra Provides-Extra: wordcloud Provides-Extra: openai
+Provides-Extra: newbing Provides-Extra: all Description-Content-Type: text/
+markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
     # nonebot-plugin-bilichat _â¨ å¤åè½çBç«è§é¢è§£æå·¥å· â¨_
 [license] [PyPI_-_Downloads] [pypi] [python] [pdm-managed] [Code_style:_black]
                [onebot] [onebot] [QQ_Chat_Group] [QQ_Chat_Group]
 ## ð ä»ç»
 è§é¢é¾æ¥è§£æï¼å¹¶æ ¹æ®å¶åå®¹çæ**åºæ¬ä¿¡æ¯**ã**è¯äº**å**åå®¹æ»ç»**
@@ -87,41 +89,47 @@
 -:|:----:|:----:| | bilichat_word_cloud | bool | True |
 æ¯å¦å¼å¯è¯äºåè½ | æ³¨ï¼è¯äºåè½å¨ python3.11 ä¸­ç±äº
 `wordcloud` åå®è£å¤±è´¥ææ¶æ æ³å¯ç¨ï¼è¯·ä¸è¦å¨ 3.11
 ä¸­å¼å¯æ­¤åè½ ### AIè§é¢æ»ç»éç½®é¡¹
 å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-plugin-bilichat
 [openai,newbing]` | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:
 ----:|:----:| | bilichat_newbing_cookie | str | None |
-newbingçcookieæä»¶è·¯å¾(è·åæ¹å¼åè[è¿é](https://github.com/
-acheong08/EdgeGPT#getting-authentication-required)å[è¿é](https://
-github.com/Harry-Jing/nonebot-plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE)) ,
-è¥çç©ºåç¦ç¨newbingæ»ç» | | bilichat_newbing_token_limit | int | 0 |
-newbingè¯·æ±çææ¬éä¸é, 0ä¸ºæ ä¸é | | bilichat_newbing_preprocess
-| bool | True | æ¯å¦å¯¹newbingçè¿åå¼è¿è¡é¢å¤ç,
-ä»¥å»é¤å¶ä¸­ä¸æ³è¦çåå®¹ | | bilichat_openai_token | str | None |
-openaiçapikey, è¥çç©ºåç¦ç¨openaiæ»ç» | | bilichat_openai_proxy | str
-| None | è®¿é®openaiænewbingä½¿ç¨çä»£çå°å | | bilichat_openai_model
-| str | gpt-3.5-turbo-0301 | ä½¿ç¨çè¯­è¨æ¨¡ååç§° | |
+newbingçcookieæä»¶è·¯å¾, å¡«å `no_login`
+åä¸è¿è¡ç»å½ï¼å¯è½ææ¬¡æ°éå¶ï¼, è¥çç©ºåç¦ç¨newbingæ»ç»
+| | bilichat_newbing_token_limit | int | 0 | newbingè¯·æ±çææ¬éä¸é,
+0ä¸ºæ ä¸é | | bilichat_newbing_preprocess | bool | True |
+æ¯å¦å¯¹newbingçè¿åå¼è¿è¡é¢å¤ç, ä»¥å»é¤å¶ä¸­ä¸æ³è¦çåå®¹
+| | bilichat_openai_token | str | None | openaiçapikey,
+è¥çç©ºåç¦ç¨openaiæ»ç» | | bilichat_openai_proxy | str | None |
+è®¿é®openaiænewbingä½¿ç¨çä»£çå°å | | bilichat_openai_model | str |
+gpt-3.5-turbo-0301 | ä½¿ç¨çè¯­è¨æ¨¡ååç§° | |
 bilichat_openai_token_limit | int | 3500 | è¯·æ±çææ¬éä¸é,
 è®¡ç®æ¹å¼å¯åè[tiktoken](https://github.com/openai/tiktoken) | æ³¨: 1.
 openai ä¸ newbing
 ç®ååéæ±ç§å­¦ä¸ç½æè½ä½¿ç¨ï¼å½åæå¡å¨è¯·å¡å¿å¡«å
 `bilichat_openai_proxy` æå¨å±éæä»£ç 2. å¦æåæ¶å¡«åäº
 `bilichat_openai_token` å `bilichat_newbing_cookie`ï¼åä¼ä½¿ç¨ `newbing`
 è¿è¡æ»ç», å¹¶å¨ `newbing` æ»ç»å¤±è´¥æ¶ä½¿ç¨ `openai` è¿è¡æ»ç» 3.
 `newbing` å `openai`
-åæç¼å­æºå¶ï¼åä¸è§é¢å¨**è·åå°æ­£å¸¸çæ»ç»åå®¹å**ä¸ä¼éå¤åéè¯·æ±ï¼å¦éå·æ°è¯·æ±åå®¹å¯ä»¥æå¨å é¤å¯¹åºè§é¢çç¼å­æä»¶ææ´ä¸ªç¼å­æä»¶å¤¹
-4. ç»æµè¯ï¼ç®å `newbing` è³å°è½æ»ç» 12000
+åæç¼å­æºå¶ï¼åä¸è§é¢å¨**è·åå°æ­£å¸¸çæ»ç»åå®¹å**ä¸ä¼éå¤åéè¯·æ±ï¼å¦éå·æ°è¯·æ±åå®¹å¯ä»¥
+[æ·»å åæ°](#åæ°è¡¨)
+ææå¨å é¤å¯¹åºè§é¢çç¼å­æä»¶ææ´ä¸ªç¼å­æä»¶å¤¹ 4.
+ç»æµè¯ï¼ç®å `newbing` è³å°è½æ»ç» 12000
 å­ç¬¦ä»¥ä¸çææ¬ï¼æ¨æµ token ä¸éåºä¸º `gpt-4-32k-0314` ç `32200`
 tokenï¼ä½è¿é¿çåå®¹æé æè¾åºåå®¹åå«é¢å¤åå®¹ææ»ç»å¤±è´¥ï¼å æ­¤ä¹å»ºè®®è®¾ç½®ä¸ä¸ªåçç
 token ä¸é ~~ï¼åæ­£ä¸è¦é±ï¼è¦å¥èªè¡è½¦ï¼~~ 5. ç±äº `newbing`
 éå¶è¾å¤§ï¼ä¹ä¸å¦ `openai`
 å¬è¯ï¼ä¸éè¦èç½æ¥è¯¢èµæï¼å æ­¤ä½¿ç¨ä½éªå¹¶ä¸å¦ chatgpt
-~~ï¼åæ­£ä¸è¦é±ï¼è¦å¥èªè¡è½¦ï¼~~ ## ð ä½¿ç¨ ç´æ¥åéè§é¢
-(ä¸æ )é¾æ¥å³å¯ ### åæ°è¡¨
+~~ï¼åæ­£ä¸è¦é±ï¼è¦å¥èªè¡è½¦ï¼~~ 6. newbing cookie
+æä»¶è·åæ¹å¼åè[è¿é](https://github.com/acheong08/EdgeGPT#getting-
+authentication-required)å[è¿é](https://github.com/Harry-Jing/nonebot-
+plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE)ãç®å newbing
+å·²æ­£å¼å¬å¸ä¸æ éç»å½ä¹å¯ä½¿ç¨ï¼å¡«å
+`bilichat_newbing_cookie=no_login` å³å¯æ  cookie ä½¿ç¨ ## ð ä½¿ç¨
+ç´æ¥åéè§é¢(ä¸æ )é¾æ¥å³å¯ ### åæ°è¡¨
 å¨åéè§é¢æ¶ï¼å¯ä»¥é¢å¤æ·»å ä»¥ä¸ç±»ä¼¼ shell
 æä»¤çåæ°ï¼è¿èå¯¹è§£ææµç¨è¿è¡è°æ´ãä¾å¦ ```shell
 BV12v4y1E7NT --refresh BV12v4y1E7NT -r # å¯ä»¥ä½¿ç¨ç®å BV12v4y1E7NT -r --
 no-cache # å¯ä»¥å¤ä¸ªåæ°æ··ç¨ -r BV12v4y1E7NT -n #
 è½ç¶ä¸å»ºè®®ï¼ä½ç¡®å®å¯ä»¥æåæ°æ¾åé¢ ``` | æä»¤ | ç®å |
 è¯´æ | |:-----:|:----:|:----:| | --no-cache | -n | æ¬æ¬¡æ»ç»ç¦ç¨ç¼å­
 (ä¸ä¼å½±åå·²å­å¨çç¼å­æä»¶) | | --refresh | -r |
```

