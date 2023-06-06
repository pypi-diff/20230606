# Comparing `tmp/nonebot_plugin_game_collection-2.1.7.tar.gz` & `tmp/nonebot_plugin_game_collection-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_game_collection-2.1.7.tar", last modified: Mon Jun  5 13:00:55 2023, max compression
+gzip compressed data, was "nonebot_plugin_game_collection-2.1.8.tar", last modified: Tue Jun  6 06:37:35 2023, max compression
```

## Comparing `nonebot_plugin_game_collection-2.1.7.tar` & `nonebot_plugin_game_collection-2.1.8.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 13:00:55.690286 nonebot_plugin_game_collection-2.1.7/
--rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.1.7/LICENSE
--rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0      376 2023-06-05 13:00:55.689786 nonebot_plugin_game_collection-2.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 13:00:55.633237 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/
--rw-rw-rw-   0        0        0    17451 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/Account.py
--rw-rw-rw-   0        0        0    50013 2023-06-05 12:50:53.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/Game.py
-drwxrwxrwx   0        0        0        0 2023-06-05 13:00:55.650752 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/HorseRace/
--rw-rw-rw-   0        0        0    15602 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/HorseRace/events_main.py
--rw-rw-rw-   0        0        0     6399 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/HorseRace/horse.py
--rw-rw-rw-   0        0        0     5151 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/HorseRace/race_group.py
--rw-rw-rw-   0        0        0     9187 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/HorseRace/start.py
--rw-rw-rw-   0        0        0    11410 2023-06-04 13:24:05.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/Manager.py
--rw-rw-rw-   0        0        0    20170 2023-06-04 13:24:04.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/Market.py
--rw-rw-rw-   0        0        0    16156 2023-06-05 10:03:35.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/Prop.py
--rw-rw-rw-   0        0        0    30875 2023-06-05 12:54:00.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/__init__.py
--rw-rw-rw-   0        0        0     3249 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/config.py
-drwxrwxrwx   0        0        0        0 2023-06-05 13:00:55.655756 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/data/
--rw-rw-rw-   0        0        0      525 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/data/api.py
--rw-rw-rw-   0        0        0     5589 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/data/data.py
--rw-rw-rw-   0        0        0      102 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/data/run.py
-drwxrwxrwx   0        0        0        0 2023-06-05 13:00:55.661262 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/resource/
--rw-rw-rw-   0        0        0      171 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/resource/element_library.json
-drwxrwxrwx   0        0        0        0 2023-06-05 13:00:55.679277 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/resource/horserace/
--rw-rw-rw-   0        0        0     5488 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/resource/horserace/Stand.json
--rw-rw-rw-   0        0        0     4549 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
--rw-rw-rw-   0        0        0     1757 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
--rw-rw-rw-   0        0        0      906 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/resource/horserace/基础事件.json
--rw-rw-rw-   0        0        0     2717 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
--rw-rw-rw-   0        0        0     1257 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
--rw-rw-rw-   0        0        0    22637 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/resource/horserace/群友日常.json
--rw-rw-rw-   0        0        0     4751 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
--rw-rw-rw-   0        0        0     1010 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
--rw-rw-rw-   0        0        0     2253 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
--rw-rw-rw-   0        0        0    12958 2023-06-04 12:00:23.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/resource/menu_data.json
--rw-rw-rw-   0        0        0     5375 2023-06-04 11:46:30.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/resource/props_library.json
-drwxrwxrwx   0        0        0        0 2023-06-05 13:00:55.683280 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/resource/subprocess/
--rw-rw-rw-   0        0        0     2245 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
-drwxrwxrwx   0        0        0        0 2023-06-05 13:00:55.688284 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/utils/
--rw-rw-rw-   0        0        0     1321 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/utils/avatar.py
--rw-rw-rw-   0        0        0     7133 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/utils/chart.py
--rw-rw-rw-   0        0        0     1619 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-05 13:00:55.642745 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection.egg-info/
--rw-rw-rw-   0        0        0      376 2023-06-05 13:00:55.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2038 2023-06-05 13:00:55.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 13:00:55.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-06-05 13:00:55.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-06-05 13:00:55.000000 nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 13:00:55.690787 nonebot_plugin_game_collection-2.1.7/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-06-05 13:00:43.000000 nonebot_plugin_game_collection-2.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:37:35.700514 nonebot_plugin_game_collection-2.1.8/
+-rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.1.8/LICENSE
+-rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      376 2023-06-06 06:37:35.700014 nonebot_plugin_game_collection-2.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 06:37:35.638736 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/
+-rw-rw-rw-   0        0        0    17451 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/Account.py
+-rw-rw-rw-   0        0        0    50095 2023-06-06 06:35:38.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/Game.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:37:35.656477 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/HorseRace/
+-rw-rw-rw-   0        0        0    15602 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/HorseRace/events_main.py
+-rw-rw-rw-   0        0        0     6399 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/HorseRace/horse.py
+-rw-rw-rw-   0        0        0     5151 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/HorseRace/race_group.py
+-rw-rw-rw-   0        0        0     9187 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/HorseRace/start.py
+-rw-rw-rw-   0        0        0    11410 2023-06-04 13:24:05.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/Manager.py
+-rw-rw-rw-   0        0        0    20170 2023-06-04 13:24:04.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/Market.py
+-rw-rw-rw-   0        0        0    16156 2023-06-05 10:03:35.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/Prop.py
+-rw-rw-rw-   0        0        0    30875 2023-06-05 12:54:00.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/__init__.py
+-rw-rw-rw-   0        0        0     3249 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/config.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:37:35.663483 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/data/
+-rw-rw-rw-   0        0        0      525 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/data/api.py
+-rw-rw-rw-   0        0        0     5589 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/data/data.py
+-rw-rw-rw-   0        0        0      102 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/data/run.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:37:35.668987 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/
+-rw-rw-rw-   0        0        0      171 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/element_library.json
+drwxrwxrwx   0        0        0        0 2023-06-06 06:37:35.690007 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/
+-rw-rw-rw-   0        0        0     5488 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/Stand.json
+-rw-rw-rw-   0        0        0     4549 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
+-rw-rw-rw-   0        0        0     1757 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
+-rw-rw-rw-   0        0        0      906 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/基础事件.json
+-rw-rw-rw-   0        0        0     2717 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
+-rw-rw-rw-   0        0        0     1257 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
+-rw-rw-rw-   0        0        0    22637 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/群友日常.json
+-rw-rw-rw-   0        0        0     4751 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
+-rw-rw-rw-   0        0        0     1010 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
+-rw-rw-rw-   0        0        0     2253 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
+-rw-rw-rw-   0        0        0    12958 2023-06-04 12:00:23.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/menu_data.json
+-rw-rw-rw-   0        0        0     5375 2023-06-04 11:46:30.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/props_library.json
+drwxrwxrwx   0        0        0        0 2023-06-06 06:37:35.693008 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/subprocess/
+-rw-rw-rw-   0        0        0     2245 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:37:35.698012 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/utils/
+-rw-rw-rw-   0        0        0     1321 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/utils/avatar.py
+-rw-rw-rw-   0        0        0     7133 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/utils/chart.py
+-rw-rw-rw-   0        0        0     1619 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:37:35.647969 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-06-06 06:37:35.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2038 2023-06-06 06:37:35.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 06:37:35.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-06-06 06:37:35.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-06-06 06:37:35.000000 nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 06:37:35.701014 nonebot_plugin_game_collection-2.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      738 2023-06-06 06:37:31.000000 nonebot_plugin_game_collection-2.1.8/setup.py
```

### Comparing `nonebot_plugin_game_collection-2.1.7/LICENSE` & `nonebot_plugin_game_collection-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/README.md` & `nonebot_plugin_game_collection-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/Account.py` & `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/Account.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/Game.py` & `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/Game.py`

 * *Files 0% similar despite different names*

```diff
@@ -1133,15 +1133,16 @@
     """
     生成快乐港式五张游戏内容
         times:抽牌次数，1次到5次。
     """
     times = 1 if times < 1 else times
     times = 5 if times > 5 else times
 
-    deck = [random_poker()[i:i+5] for i in range(0, 52, 5)]
+    deck = random_poker()
+    deck = [deck[i:i+5] for i in range(0, 50, 5)]
 
     hand1,pt1 = max_hand(deck[0:times])
     hand2,pt2 = max_hand(deck[times:2*times])
 
     return {
         "game":"cantrell",
         "round_gold":gold,
@@ -1162,14 +1163,15 @@
     session.gold = gold
     if times == 1:
         session.info = cantrell_info(gold)
     else:
         session.info = happy_cantrell_info(gold,times)
     return (f"随机牌堆已生成\n"
             f"开局金额：{gold}\n"
+            + (f"等级：Lv.{times}\n" if times > 1 else "") +
             f"{msg}")
 
 async def cantrell_check(bot:Bot, event:GroupMessageEvent):
     """
     看牌
     """
     group_id = event.group_id
```

### Comparing `nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/HorseRace/events_main.py` & `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/HorseRace/events_main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/HorseRace/horse.py` & `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/HorseRace/horse.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/HorseRace/race_group.py` & `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/HorseRace/race_group.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/HorseRace/start.py` & `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/HorseRace/start.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/Manager.py` & `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/Manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/Market.py` & `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/Market.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/Prop.py` & `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/Prop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/__init__.py` & `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/config.py` & `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/data/api.py` & `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/data/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/data/data.py` & `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/data/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/resource/horserace/Stand.json` & `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/Stand.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json` & `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json` & `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/resource/horserace/基础事件.json` & `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/基础事件.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json` & `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json` & `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/resource/horserace/群友日常.json` & `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/群友日常.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json` & `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json` & `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json` & `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/resource/menu_data.json` & `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/menu_data.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/resource/props_library.json` & `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/props_library.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/resource/subprocess/ohlc.py` & `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/resource/subprocess/ohlc.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/utils/avatar.py` & `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/utils/avatar.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/utils/chart.py` & `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/utils/chart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection/utils/utils.py` & `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection/utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/nonebot_plugin_game_collection.egg-info/SOURCES.txt` & `nonebot_plugin_game_collection-2.1.8/nonebot_plugin_game_collection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.7/setup.py` & `nonebot_plugin_game_collection-2.1.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_game_collection',
-version='2.1.7',
+version='2.1.8',
 description='改自nonebot_plugin_russian合并了nonebot_plugin_horserace还有一些自编玩法的小游戏合集。',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_game_collection","nonebot_plugin_game_collection.*"]),
```

