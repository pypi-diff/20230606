# Comparing `tmp/nonebot_plugin_get_nickname-0.1.1.tar.gz` & `tmp/nonebot_plugin_get_nickname-0.1.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_get_nickname-0.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_get_nickname-0.1.1.post1.tar", max compression
```

## Comparing `nonebot_plugin_get_nickname-0.1.1.tar` & `nonebot_plugin_get_nickname-0.1.1.post1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1085 2022-10-29 01:06:44.421000 nonebot_plugin_get_nickname-0.1.1/LICENSE
--rw-r--r--   0        0        0     1057 2023-06-06 15:47:24.087948 nonebot_plugin_get_nickname-0.1.1/nonebot_plugin_get_nickname/__init__.py
--rw-r--r--   0        0        0      107 2023-06-06 15:22:53.370010 nonebot_plugin_get_nickname-0.1.1/nonebot_plugin_get_nickname/errors.py
--rw-r--r--   0        0        0      822 2023-06-06 15:38:02.838277 nonebot_plugin_get_nickname-0.1.1/nonebot_plugin_get_nickname/func_manager.py
--rw-r--r--   0        0        0      584 2023-06-06 15:42:22.782113 nonebot_plugin_get_nickname-0.1.1/nonebot_plugin_get_nickname/get_bot_nickname/__init__.py
--rw-r--r--   0        0        0      601 2023-06-06 15:45:04.373910 nonebot_plugin_get_nickname-0.1.1/nonebot_plugin_get_nickname/get_bot_nickname/onebot_v11.py
--rw-r--r--   0        0        0      624 2023-06-06 15:45:04.347888 nonebot_plugin_get_nickname-0.1.1/nonebot_plugin_get_nickname/get_bot_nickname/qqguild.py
--rw-r--r--   0        0        0      560 2023-06-06 15:38:02.852274 nonebot_plugin_get_nickname-0.1.1/nonebot_plugin_get_nickname/get_nickname/__init__.py
--rw-r--r--   0        0        0     1309 2023-06-06 15:49:02.212836 nonebot_plugin_get_nickname-0.1.1/nonebot_plugin_get_nickname/get_nickname/onebot_v11.py
--rw-r--r--   0        0        0     1058 2023-06-06 15:49:02.217841 nonebot_plugin_get_nickname-0.1.1/nonebot_plugin_get_nickname/get_nickname/qqguild.py
--rw-r--r--   0        0        0      581 2023-06-06 15:20:47.652965 nonebot_plugin_get_nickname-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-01 02:38:55.716376 nonebot_plugin_get_nickname-0.1.1/README.md
--rw-r--r--   0        0        0      497 1970-01-01 00:00:00.000000 nonebot_plugin_get_nickname-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2022-10-29 01:06:44.421000 nonebot_plugin_get_nickname-0.1.1.post1/LICENSE
+-rw-r--r--   0        0        0     1073 2023-06-06 15:51:13.963401 nonebot_plugin_get_nickname-0.1.1.post1/nonebot_plugin_get_nickname/__init__.py
+-rw-r--r--   0        0        0      107 2023-06-06 15:22:53.370010 nonebot_plugin_get_nickname-0.1.1.post1/nonebot_plugin_get_nickname/errors.py
+-rw-r--r--   0        0        0      822 2023-06-06 15:38:02.838277 nonebot_plugin_get_nickname-0.1.1.post1/nonebot_plugin_get_nickname/func_manager.py
+-rw-r--r--   0        0        0      584 2023-06-06 15:42:22.782113 nonebot_plugin_get_nickname-0.1.1.post1/nonebot_plugin_get_nickname/get_bot_nickname/__init__.py
+-rw-r--r--   0        0        0      601 2023-06-06 15:45:04.373910 nonebot_plugin_get_nickname-0.1.1.post1/nonebot_plugin_get_nickname/get_bot_nickname/onebot_v11.py
+-rw-r--r--   0        0        0      624 2023-06-06 15:45:04.347888 nonebot_plugin_get_nickname-0.1.1.post1/nonebot_plugin_get_nickname/get_bot_nickname/qqguild.py
+-rw-r--r--   0        0        0      560 2023-06-06 15:38:02.852274 nonebot_plugin_get_nickname-0.1.1.post1/nonebot_plugin_get_nickname/get_nickname/__init__.py
+-rw-r--r--   0        0        0     1309 2023-06-06 15:49:02.212836 nonebot_plugin_get_nickname-0.1.1.post1/nonebot_plugin_get_nickname/get_nickname/onebot_v11.py
+-rw-r--r--   0        0        0     1058 2023-06-06 15:49:02.217841 nonebot_plugin_get_nickname-0.1.1.post1/nonebot_plugin_get_nickname/get_nickname/qqguild.py
+-rw-r--r--   0        0        0      587 2023-06-06 15:51:13.968402 nonebot_plugin_get_nickname-0.1.1.post1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-01 02:38:55.716376 nonebot_plugin_get_nickname-0.1.1.post1/README.md
+-rw-r--r--   0        0        0      503 1970-01-01 00:00:00.000000 nonebot_plugin_get_nickname-0.1.1.post1/PKG-INFO
```

### Comparing `nonebot_plugin_get_nickname-0.1.1/LICENSE` & `nonebot_plugin_get_nickname-0.1.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_get_nickname-0.1.1/nonebot_plugin_get_nickname/__init__.py` & `nonebot_plugin_get_nickname-0.1.1.post1/nonebot_plugin_get_nickname/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,12 +22,12 @@
     type="library",
     homepage="https://github.com/bot-ssttkkl/nonebot-plugin-get-nickname",
     supported_adapters={"~onebot.v11", "~qqguild"}
 )
 
 
 async def get_nickname(session_or_event: Union[Session, Event], bot: Bot, *, raise_on_failed: bool = False) -> str:
-    return await func(bot.type).get_nickname(session_or_event, bot, raise_on_failed)
+    return await func(bot.type).get_nickname(session_or_event, bot, raise_on_failed=raise_on_failed)
 
 
 async def get_bot_nickname(bot: Bot) -> str:
     return await func(bot.type).get_bot_nickname(bot)
```

### Comparing `nonebot_plugin_get_nickname-0.1.1/nonebot_plugin_get_nickname/func_manager.py` & `nonebot_plugin_get_nickname-0.1.1.post1/nonebot_plugin_get_nickname/func_manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_get_nickname-0.1.1/nonebot_plugin_get_nickname/get_bot_nickname/__init__.py` & `nonebot_plugin_get_nickname-0.1.1.post1/nonebot_plugin_get_nickname/get_bot_nickname/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_get_nickname-0.1.1/nonebot_plugin_get_nickname/get_bot_nickname/onebot_v11.py` & `nonebot_plugin_get_nickname-0.1.1.post1/nonebot_plugin_get_nickname/get_bot_nickname/onebot_v11.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_get_nickname-0.1.1/nonebot_plugin_get_nickname/get_bot_nickname/qqguild.py` & `nonebot_plugin_get_nickname-0.1.1.post1/nonebot_plugin_get_nickname/get_bot_nickname/qqguild.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_get_nickname-0.1.1/nonebot_plugin_get_nickname/get_nickname/__init__.py` & `nonebot_plugin_get_nickname-0.1.1.post1/nonebot_plugin_get_nickname/get_nickname/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_get_nickname-0.1.1/nonebot_plugin_get_nickname/get_nickname/onebot_v11.py` & `nonebot_plugin_get_nickname-0.1.1.post1/nonebot_plugin_get_nickname/get_nickname/onebot_v11.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_get_nickname-0.1.1/nonebot_plugin_get_nickname/get_nickname/qqguild.py` & `nonebot_plugin_get_nickname-0.1.1.post1/nonebot_plugin_get_nickname/get_nickname/qqguild.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_get_nickname-0.1.1/pyproject.toml` & `nonebot_plugin_get_nickname-0.1.1.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-get-nickname"
-version = "0.1.1"
+version = "0.1.1.post1"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.md"
 packages = [{include = "nonebot_plugin_get_nickname"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

