# Comparing `tmp/nonebot_plugin_wordle_help-0.0.1.tar.gz` & `tmp/nonebot_plugin_wordle_help-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_wordle_help-0.0.1.tar", last modified: Wed May  3 19:54:43 2023, max compression
+gzip compressed data, was "nonebot_plugin_wordle_help-0.0.2.tar", last modified: Tue Jun  6 15:13:07 2023, max compression
```

## Comparing `nonebot_plugin_wordle_help-0.0.1.tar` & `nonebot_plugin_wordle_help-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 19:54:43.837595 nonebot_plugin_wordle_help-0.0.1/
--rw-rw-rw-   0        0        0     1064 2022-06-17 16:08:47.000000 nonebot_plugin_wordle_help-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      378 2023-05-03 19:54:43.836597 nonebot_plugin_wordle_help-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-03 19:54:43.829595 nonebot_plugin_wordle_help-0.0.1/nonebot_plugin_wordle_help/
--rw-rw-rw-   0        0        0      620 2023-05-03 19:30:24.000000 nonebot_plugin_wordle_help-0.0.1/nonebot_plugin_wordle_help/__init__.py
--rw-rw-rw-   0        0        0   318471 2023-05-03 17:55:25.000000 nonebot_plugin_wordle_help-0.0.1/nonebot_plugin_wordle_help/data.json
--rw-rw-rw-   0        0        0     1928 2023-05-03 19:15:42.000000 nonebot_plugin_wordle_help-0.0.1/nonebot_plugin_wordle_help/handle.py
-drwxrwxrwx   0        0        0        0 2023-05-03 19:54:43.835594 nonebot_plugin_wordle_help-0.0.1/nonebot_plugin_wordle_help.egg-info/
--rw-rw-rw-   0        0        0      378 2023-05-03 19:54:43.000000 nonebot_plugin_wordle_help-0.0.1/nonebot_plugin_wordle_help.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      378 2023-05-03 19:54:43.000000 nonebot_plugin_wordle_help-0.0.1/nonebot_plugin_wordle_help.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 19:54:43.000000 nonebot_plugin_wordle_help-0.0.1/nonebot_plugin_wordle_help.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-03 19:54:43.000000 nonebot_plugin_wordle_help-0.0.1/nonebot_plugin_wordle_help.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-05-03 19:54:43.000000 nonebot_plugin_wordle_help-0.0.1/nonebot_plugin_wordle_help.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 19:54:43.837595 nonebot_plugin_wordle_help-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      618 2023-05-03 19:54:29.000000 nonebot_plugin_wordle_help-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 15:13:07.661599 nonebot_plugin_wordle_help-0.0.2/
+-rw-rw-rw-   0        0        0     1064 2022-06-17 16:08:47.000000 nonebot_plugin_wordle_help-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      378 2023-06-06 15:13:07.659562 nonebot_plugin_wordle_help-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-06 15:13:07.650550 nonebot_plugin_wordle_help-0.0.2/nonebot_plugin_wordle_help/
+-rw-rw-rw-   0        0        0      804 2023-06-06 15:11:46.000000 nonebot_plugin_wordle_help-0.0.2/nonebot_plugin_wordle_help/__init__.py
+-rw-rw-rw-   0        0        0   338729 2023-06-06 15:09:58.000000 nonebot_plugin_wordle_help-0.0.2/nonebot_plugin_wordle_help/data.json
+-rw-rw-rw-   0        0        0     1980 2023-06-06 15:09:58.000000 nonebot_plugin_wordle_help-0.0.2/nonebot_plugin_wordle_help/handle.py
+drwxrwxrwx   0        0        0        0 2023-06-06 15:13:07.657559 nonebot_plugin_wordle_help-0.0.2/nonebot_plugin_wordle_help.egg-info/
+-rw-rw-rw-   0        0        0      378 2023-06-06 15:13:07.000000 nonebot_plugin_wordle_help-0.0.2/nonebot_plugin_wordle_help.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2023-06-06 15:13:07.000000 nonebot_plugin_wordle_help-0.0.2/nonebot_plugin_wordle_help.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 15:13:07.000000 nonebot_plugin_wordle_help-0.0.2/nonebot_plugin_wordle_help.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-06 15:13:07.000000 nonebot_plugin_wordle_help-0.0.2/nonebot_plugin_wordle_help.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-06-06 15:13:07.000000 nonebot_plugin_wordle_help-0.0.2/nonebot_plugin_wordle_help.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 15:13:07.661599 nonebot_plugin_wordle_help-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      618 2023-06-06 15:13:00.000000 nonebot_plugin_wordle_help-0.0.2/setup.py
```

### Comparing `nonebot_plugin_wordle_help-0.0.1/LICENSE` & `nonebot_plugin_wordle_help-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle_help-0.0.1/nonebot_plugin_wordle_help/handle.py` & `nonebot_plugin_wordle_help-0.0.2/nonebot_plugin_wordle_help/handle.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-import json
-from pathlib import Path
-from typing import List
-
-from nonebot.adapters.onebot.v11 import MessageEvent
-from nonebot.matcher import Matcher
-
-
-class WordleHelp:
-    def __init__(self) -> None:
-        """初始化, 读取单词列表"""
-        plugin_path = Path(__file__).parent
-        with open(plugin_path / "data.json",'r', encoding='utf-8') as f:
-            self.words = json.load(f)
-
-    async def get_matching_words(self, target: str) -> List[str]:
-        """获取匹配的单词"""
-        return [word for word in self.words if len(word) == len(target) and all(target[i] == "_" or word[i] == target[i] for i in range(len(word)))]
-    
-    async def main(
-        self,
-        matcher: Matcher,
-        event: MessageEvent
-    ) -> None:
-        """处理消息"""
-        target = event.get_message().__str__().strip().split("#")       # 按照#分割成列表, 理论上最多两个元素, 前者为目标单词, 后者排除的字母
-        matching_words = await self.get_matching_words(target[0])       # 先匹配单词
-        if len(target) == 2:                                            # 如果有排除的字母, 则再次筛选
-            matching_words = [word for word in matching_words if not set(word) & set(target[1])]
-
-        if len(matching_words) == 0:                                    # 如果没有匹配到单词, 则返回
-            await matcher.send("没有匹配到单词捏")
-        elif len(matching_words) > 50:                                  # 如果匹配到的单词太多, 则返回
-            await matcher.send("匹配到的单词太多了(>50), 建议您缩小一下范围")
-        else:                                                           # 返回匹配到的单词
-            await matcher.send(
-                "以下是匹配到的单词：\n"+
-                "\n".join(matching_words)
-            )
-            
-wordle_help = WordleHelp()
+import json
+from pathlib import Path
+from typing import List
+
+from nonebot.adapters.onebot.v11 import MessageEvent
+from nonebot.matcher import Matcher
+
+
+class WordleHelp:
+    def __init__(self) -> None:
+        """初始化, 读取单词列表"""
+        plugin_path = Path(__file__).parent
+        with open(plugin_path / "data.json",'r', encoding='utf-8') as f:
+            self.words: List[str] = json.load(f)
+
+    async def get_matching_words(self, target: str) -> List[str]:
+        """获取匹配的单词"""
+        return [word for word in self.words if len(word) == len(target) and all(target[i] == "_" or word[i] == target[i] for i in range(len(word)))]
+    
+    async def main(
+        self,
+        matcher: Matcher,
+        event: MessageEvent
+    ) -> None:
+        """处理消息"""
+        target = event.get_message().__str__().strip().split("#")       # 按照#分割成列表, 理论上最多两个元素, 前者为目标单词, 后者排除的字母
+        matching_words = await self.get_matching_words(target[0])       # 先匹配单词
+        if len(target) == 2:                                            # 如果有排除的字母, 则再次筛选
+            matching_words = [word for word in matching_words if not set(word) & set(target[1])]
+
+        if len(matching_words) == 0:                                    # 如果没有匹配到单词, 则返回
+            await matcher.send("没有匹配到单词捏")
+        elif len(matching_words) > 50:                                  # 如果匹配到的单词太多, 则返回
+            await matcher.send("匹配到的单词太多了(>50), 建议您缩小一下范围")
+        else:                                                           # 返回匹配到的单词
+            await matcher.send(
+                "以下是匹配到的单词：\n"+
+                "\n".join(matching_words)
+            )
+            
+wordle_help = WordleHelp()
```

### Comparing `nonebot_plugin_wordle_help-0.0.1/setup.py` & `nonebot_plugin_wordle_help-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 
 from setuptools import find_packages, setup
 name = 'nonebot_plugin_wordle_help'
 
 setup(
     name=name,
-    version='0.0.1',
+    version='0.0.2',
     author="Special-Week",
     author_email='2385612749@qq.com',
     description="wordle小游戏工具",
     python_requires=">=3.8.0",
     packages=find_packages(),
     long_description="https://github.com/Special-Week/Hinata-Bot/tree/main/src/plugins/wordle_help",
     url="https://github.com/Special-Week/Hinata-Bot/tree/main/src/plugins/wordle_help",
```

