# Comparing `tmp/nonebot-plugin-sky-2.2.9.tar.gz` & `tmp/nonebot-plugin-sky-2.2.9.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-sky-2.2.9.tar", last modified: Tue May 30 05:09:19 2023, max compression
+gzip compressed data, was "nonebot-plugin-sky-2.2.9.post1.tar", last modified: Tue May 30 05:14:33 2023, max compression
```

## Comparing `nonebot-plugin-sky-2.2.9.tar` & `nonebot-plugin-sky-2.2.9.post1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 05:09:19.166185 nonebot-plugin-sky-2.2.9/
--rw-rw-rw-   0        0        0    35823 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/LICENSE
--rw-rw-rw-   0        0        0    15786 2023-05-30 05:09:19.165188 nonebot-plugin-sky-2.2.9/PKG-INFO
--rw-rw-rw-   0        0        0    15262 2023-05-30 05:08:23.000000 nonebot-plugin-sky-2.2.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 05:09:19.102356 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/
--rw-rw-rw-   0        0        0     7697 2023-05-30 04:59:27.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 05:09:19.117315 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/config/
--rw-rw-rw-   0        0        0        0 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/config/__init__.py
--rw-rw-rw-   0        0        0     5707 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/config/command.py
--rw-rw-rw-   0        0        0     1810 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/config/helper_at_all.py
--rw-rw-rw-   0        0        0     1258 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/config/load_config.py
--rw-rw-rw-   0        0        0     1748 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/config/msg_forward.py
--rw-rw-rw-   0        0        0     1628 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/config/travelling_cache.py
-drwxrwxrwx   0        0        0        0 2023-05-30 05:09:19.121305 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/guild/
--rw-rw-rw-   0        0        0     1160 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/guild/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/guild/light_beauty.py
--rw-rw-rw-   0        0        0        0 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/guild/light_cute.py
-drwxrwxrwx   0        0        0        0 2023-05-30 05:09:19.124297 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/
--rw-rw-rw-   0        0        0        0 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 05:09:19.128286 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/daily_tasks/
--rw-rw-rw-   0        0        0        0 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/daily_tasks/__init__.py
--rw-rw-rw-   0        0        0     2547 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/daily_tasks/international.py
--rw-rw-rw-   0        0        0     3077 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/daily_tasks/national.py
--rw-rw-rw-   0        0        0      637 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/public_notice.py
--rw-rw-rw-   0        0        0     1083 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/queue.py
-drwxrwxrwx   0        0        0        0 2023-05-30 05:09:19.132275 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/travelling_spirit/
--rw-rw-rw-   0        0        0        0 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/travelling_spirit/__init__.py
--rw-rw-rw-   0        0        0     3225 2023-05-26 10:18:30.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/travelling_spirit/international.py
--rw-rw-rw-   0        0        0     3369 2023-05-30 04:53:54.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/travelling_spirit/national.py
-drwxrwxrwx   0        0        0        0 2023-05-30 05:09:19.139257 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/
--rw-rw-rw-   0        0        0        0 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 05:09:19.151224 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/helper_image/
--rw-rw-rw-   0        0        0    16051 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/helper_image/eating.jpg
--rw-rw-rw-   0        0        0    89789 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/helper_image/face_braid.gif
--rw-rw-rw-   0        0        0    79644 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/helper_image/face_bun.gif
--rw-rw-rw-   0        0        0    72146 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/helper_image/face_cat.gif
--rw-rw-rw-   0        0        0    87935 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/helper_image/face_fox.gif
--rw-rw-rw-   0        0        0    80542 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/helper_image/face_white_cat.gif
--rw-rw-rw-   0        0        0    95522 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/helper_image/go.jpg
--rw-rw-rw-   0        0        0      274 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/menu.py
-drwxrwxrwx   0        0        0        0 2023-05-30 05:09:19.153219 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/menu_image/
--rw-rw-rw-   0        0        0   824527 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/menu_image/menu.png
--rw-rw-rw-   0        0        0       97 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/pusher.py
--rw-rw-rw-   0        0        0     3907 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/scheduler.py
-drwxrwxrwx   0        0        0        0 2023-05-30 05:09:19.164190 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/
--rw-rw-rw-   0        0        0     2280 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/__init__.py
--rw-rw-rw-   0        0        0      405 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/bot_loader.py
--rw-rw-rw-   0        0        0      607 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/chain_reply.py
--rw-rw-rw-   0        0        0     5064 2023-05-30 05:08:23.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/check_update.py
--rw-rw-rw-   0        0        0     6447 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/data_pack.py
--rw-rw-rw-   0        0        0      391 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/date_util.py
--rw-rw-rw-   0        0        0      746 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/json_cards.py
--rw-rw-rw-   0        0        0     1264 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/notice_board.py
--rw-rw-rw-   0        0        0     6554 2023-05-30 04:55:58.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/travel_cycle.py
-drwxrwxrwx   0        0        0        0 2023-05-30 05:09:19.110335 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky.egg-info/
--rw-rw-rw-   0        0        0    15786 2023-05-30 05:09:19.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1954 2023-05-30 05:09:19.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 05:09:19.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-05-30 05:09:19.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-30 05:09:19.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 05:09:19.166185 nonebot-plugin-sky-2.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1450 2023-05-30 05:08:23.000000 nonebot-plugin-sky-2.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 05:14:33.178964 nonebot-plugin-sky-2.2.9.post1/
+-rw-rw-rw-   0        0        0    35823 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/LICENSE
+-rw-rw-rw-   0        0        0    15798 2023-05-30 05:14:33.177966 nonebot-plugin-sky-2.2.9.post1/PKG-INFO
+-rw-rw-rw-   0        0        0    15268 2023-05-30 05:14:10.000000 nonebot-plugin-sky-2.2.9.post1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 05:14:33.137074 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/
+-rw-rw-rw-   0        0        0     7697 2023-05-30 04:59:27.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 05:14:33.146050 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/config/
+-rw-rw-rw-   0        0        0        0 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/config/__init__.py
+-rw-rw-rw-   0        0        0     5707 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/config/command.py
+-rw-rw-rw-   0        0        0     1810 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/config/helper_at_all.py
+-rw-rw-rw-   0        0        0     1258 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/config/load_config.py
+-rw-rw-rw-   0        0        0     1748 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/config/msg_forward.py
+-rw-rw-rw-   0        0        0     1628 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/config/travelling_cache.py
+drwxrwxrwx   0        0        0        0 2023-05-30 05:14:33.148044 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/guild/
+-rw-rw-rw-   0        0        0     1160 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/guild/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/guild/light_beauty.py
+-rw-rw-rw-   0        0        0        0 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/guild/light_cute.py
+drwxrwxrwx   0        0        0        0 2023-05-30 05:14:33.150039 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/sky/
+-rw-rw-rw-   0        0        0        0 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/sky/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 05:14:33.153031 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/sky/daily_tasks/
+-rw-rw-rw-   0        0        0        0 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/sky/daily_tasks/__init__.py
+-rw-rw-rw-   0        0        0     2547 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/sky/daily_tasks/international.py
+-rw-rw-rw-   0        0        0     3077 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/sky/daily_tasks/national.py
+-rw-rw-rw-   0        0        0      637 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/sky/public_notice.py
+-rw-rw-rw-   0        0        0     1083 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/sky/queue.py
+drwxrwxrwx   0        0        0        0 2023-05-30 05:14:33.155026 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/sky/travelling_spirit/
+-rw-rw-rw-   0        0        0        0 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/sky/travelling_spirit/__init__.py
+-rw-rw-rw-   0        0        0     3225 2023-05-26 10:18:30.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/sky/travelling_spirit/international.py
+-rw-rw-rw-   0        0        0     3369 2023-05-30 04:53:54.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/sky/travelling_spirit/national.py
+drwxrwxrwx   0        0        0        0 2023-05-30 05:14:33.158018 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/tools/
+-rw-rw-rw-   0        0        0        0 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 05:14:33.164999 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/tools/helper_image/
+-rw-rw-rw-   0        0        0    16051 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/tools/helper_image/eating.jpg
+-rw-rw-rw-   0        0        0    89789 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/tools/helper_image/face_braid.gif
+-rw-rw-rw-   0        0        0    79644 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/tools/helper_image/face_bun.gif
+-rw-rw-rw-   0        0        0    72146 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/tools/helper_image/face_cat.gif
+-rw-rw-rw-   0        0        0    87935 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/tools/helper_image/face_fox.gif
+-rw-rw-rw-   0        0        0    80542 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/tools/helper_image/face_white_cat.gif
+-rw-rw-rw-   0        0        0    95522 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/tools/helper_image/go.jpg
+-rw-rw-rw-   0        0        0      274 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/tools/menu.py
+drwxrwxrwx   0        0        0        0 2023-05-30 05:14:33.166993 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/tools/menu_image/
+-rw-rw-rw-   0        0        0   824527 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/tools/menu_image/menu.png
+-rw-rw-rw-   0        0        0       97 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/tools/pusher.py
+-rw-rw-rw-   0        0        0     3907 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/tools/scheduler.py
+drwxrwxrwx   0        0        0        0 2023-05-30 05:14:33.175971 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/utils_/
+-rw-rw-rw-   0        0        0     2280 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/utils_/__init__.py
+-rw-rw-rw-   0        0        0      405 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/utils_/bot_loader.py
+-rw-rw-rw-   0        0        0      607 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/utils_/chain_reply.py
+-rw-rw-rw-   0        0        0     5070 2023-05-30 05:14:10.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/utils_/check_update.py
+-rw-rw-rw-   0        0        0     6447 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/utils_/data_pack.py
+-rw-rw-rw-   0        0        0      391 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/utils_/date_util.py
+-rw-rw-rw-   0        0        0      746 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/utils_/json_cards.py
+-rw-rw-rw-   0        0        0     1264 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/utils_/notice_board.py
+-rw-rw-rw-   0        0        0     6554 2023-05-30 04:55:58.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/utils_/travel_cycle.py
+drwxrwxrwx   0        0        0        0 2023-05-30 05:14:33.141063 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky.egg-info/
+-rw-rw-rw-   0        0        0    15798 2023-05-30 05:14:33.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1954 2023-05-30 05:14:33.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 05:14:33.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-05-30 05:14:33.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-30 05:14:33.000000 nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 05:14:33.178964 nonebot-plugin-sky-2.2.9.post1/setup.cfg
+-rw-rw-rw-   0        0        0     1397 2023-05-30 05:14:10.000000 nonebot-plugin-sky-2.2.9.post1/setup.py
```

### Comparing `nonebot-plugin-sky-2.2.9/LICENSE` & `nonebot-plugin-sky-2.2.9.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.9/PKG-INFO` & `nonebot-plugin-sky-2.2.9.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sky
-Version: 2.2.9
+Version: 2.2.9.post1
 Summary: nonebot2 plugin sky
 Home-page: https://github.com/Kaguya233qwq/nonebot_plugin_sky
 Author: Kaguya233qwq
 Author-email: 1435608435@qq.com
 Keywords: pip,nonebot2,nonebot,sky光遇,光遇
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -280,15 +280,15 @@
 
 新浪微博@张张幼稚园 —> *攻略内容*
 
 新浪微博&哔哩哔哩@木易不高兴了啊 —> *攻略内容*
 
 ## ✨更新日志✨
 
-2023.5.30 v2.2.9
+2023.5.30 v2.2.9.post1
 
 这个版本修复了上版本复刻缓存方法调用错误的问题，现在可以智能化识别国服通常复刻周期
 
 2023.5.22 v2.2.8
 
 新增国服通用复刻周期函数，国服复刻已更新，国际服复刻维护中。新增若干随机文案
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sky Version: 2.2.9 Summary: nonebot2
-plugin sky Home-page: https://github.com/Kaguya233qwq/nonebot_plugin_sky
-Author: Kaguya233qwq Author-email: 1435608435@qq.com Keywords:
-pip,nonebot2,nonebot,skyåé,åé Platform: any Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
-Public License v3 (GPLv3) Classifier: Natural Language :: Chinese (Simplified)
-Description-Content-Type: text/markdown License-File: LICENSE
+Metadata-Version: 2.1 Name: nonebot-plugin-sky Version: 2.2.9.post1 Summary:
+nonebot2 plugin sky Home-page: https://github.com/Kaguya233qwq/
+nonebot_plugin_sky Author: Kaguya233qwq Author-email: 1435608435@qq.com
+Keywords: pip,nonebot2,nonebot,skyåé,åé Platform: any Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
+General Public License v3 (GPLv3) Classifier: Natural Language :: Chinese
+(Simplified) Description-Content-Type: text/markdown License-File: LICENSE
                                      [sky]
       # nonebot_plugin_sky _â¨ åºäº [NoneBot2](https://v2.nonebot.dev/
                       ) çåéæ¯æ¥æ»ç¥æä»¶ â¨_
                            [Python] [NoneBot] [pypi]
                              _âå åèéâ_
 # â¨å®è£ä¸é¨ç½²â¨
 ##ä»¥ä¸ä¸ç§ç±»åè¯·éæ©éåèªå·±çæ¹æ¡è¿è¡é¨ç½²ï¼
@@ -106,15 +106,15 @@
 (ç¾¤æä»¶æä¸é®å¯å¨å)
                                      [sky]
 ## â¨æè°¢ååï¼ä¸åååï¼â¨ æ°æµªå¾®å@åéééååå â>
 *æ»ç¥åå®¹* æ°æµªå¾®å@æ§æ¥ä¸æ¥ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@ä»å¤©æ¸¸ç¦»ç¿»è½¦äºå â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@å¼ å¼ å¹¼ç¨å­ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å&åå©åå©@æ¨æä¸é«å´äºå â> *æ»ç¥åå®¹* ##
-â¨æ´æ°æ¥å¿â¨ 2023.5.30 v2.2.9
+â¨æ´æ°æ¥å¿â¨ 2023.5.30 v2.2.9.post1
 è¿ä¸ªçæ¬ä¿®å¤äºä¸çæ¬å¤å»ç¼å­æ¹æ³è°ç¨éè¯¯çé®é¢ï¼ç°å¨å¯ä»¥æºè½åè¯å«å½æéå¸¸å¤å»å¨æ
 2023.5.22 v2.2.8
 æ°å¢å½æéç¨å¤å»å¨æå½æ°ï¼å½æå¤å»å·²æ´æ°ï¼å½éæå¤å»ç»´æ¤ä¸­ãæ°å¢è¥å¹²éæºææ¡
 2023.4.30 v2.2.7
 1.å¨è¿ä¸ªçæ¬ä¹åææquerytoolså½ä»¤ååºå¼ä¸åçæã
 2.æ´æ°å­£èæ¶é´ï¼ææ¶ä¸æ¯å¾åç¡® 2023.4.25 v2.2.6
 1.ä¿®å¤è·åuidå¸®å©å¾çæ æ³åéçé®é¢
```

### Comparing `nonebot-plugin-sky-2.2.9/README.md` & `nonebot-plugin-sky-2.2.9.post1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -265,15 +265,15 @@
 
 新浪微博@张张幼稚园 —> *攻略内容*
 
 新浪微博&哔哩哔哩@木易不高兴了啊 —> *攻略内容*
 
 ## ✨更新日志✨
 
-2023.5.30 v2.2.9
+2023.5.30 v2.2.9.post1
 
 这个版本修复了上版本复刻缓存方法调用错误的问题，现在可以智能化识别国服通常复刻周期
 
 2023.5.22 v2.2.8
 
 新增国服通用复刻周期函数，国服复刻已更新，国际服复刻维护中。新增若干随机文案
```

#### html2text {}

```diff
@@ -99,15 +99,15 @@
 (ç¾¤æä»¶æä¸é®å¯å¨å)
                                      [sky]
 ## â¨æè°¢ååï¼ä¸åååï¼â¨ æ°æµªå¾®å@åéééååå â>
 *æ»ç¥åå®¹* æ°æµªå¾®å@æ§æ¥ä¸æ¥ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@ä»å¤©æ¸¸ç¦»ç¿»è½¦äºå â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@å¼ å¼ å¹¼ç¨å­ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å&åå©åå©@æ¨æä¸é«å´äºå â> *æ»ç¥åå®¹* ##
-â¨æ´æ°æ¥å¿â¨ 2023.5.30 v2.2.9
+â¨æ´æ°æ¥å¿â¨ 2023.5.30 v2.2.9.post1
 è¿ä¸ªçæ¬ä¿®å¤äºä¸çæ¬å¤å»ç¼å­æ¹æ³è°ç¨éè¯¯çé®é¢ï¼ç°å¨å¯ä»¥æºè½åè¯å«å½æéå¸¸å¤å»å¨æ
 2023.5.22 v2.2.8
 æ°å¢å½æéç¨å¤å»å¨æå½æ°ï¼å½æå¤å»å·²æ´æ°ï¼å½éæå¤å»ç»´æ¤ä¸­ãæ°å¢è¥å¹²éæºææ¡
 2023.4.30 v2.2.7
 1.å¨è¿ä¸ªçæ¬ä¹åææquerytoolså½ä»¤ååºå¼ä¸åçæã
 2.æ´æ°å­£èæ¶é´ï¼ææ¶ä¸æ¯å¾åç¡® 2023.4.25 v2.2.6
 1.ä¿®å¤è·åuidå¸®å©å¾çæ æ³åéçé®é¢
```

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/__init__.py` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/config/command.py` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/config/command.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/config/helper_at_all.py` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/config/helper_at_all.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/config/load_config.py` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/config/load_config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/config/msg_forward.py` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/config/msg_forward.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/config/travelling_cache.py` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/config/travelling_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/guild/__init__.py` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/guild/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/daily_tasks/international.py` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/sky/daily_tasks/international.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/daily_tasks/national.py` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/sky/daily_tasks/national.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/public_notice.py` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/sky/public_notice.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/queue.py` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/sky/queue.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/travelling_spirit/international.py` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/sky/travelling_spirit/international.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/travelling_spirit/national.py` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/sky/travelling_spirit/national.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/helper_image/eating.jpg` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/tools/helper_image/eating.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/helper_image/face_braid.gif` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/tools/helper_image/face_braid.gif`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/helper_image/face_bun.gif` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/tools/helper_image/face_bun.gif`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/helper_image/face_cat.gif` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/tools/helper_image/face_cat.gif`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/helper_image/face_fox.gif` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/tools/helper_image/face_fox.gif`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/helper_image/face_white_cat.gif` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/tools/helper_image/face_white_cat.gif`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/helper_image/go.jpg` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/tools/helper_image/go.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/menu_image/menu.png` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/tools/menu_image/menu.png`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/scheduler.py` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/tools/scheduler.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/__init__.py` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/utils_/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/chain_reply.py` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/utils_/chain_reply.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/check_update.py` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/utils_/check_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 
 from nonebot import on_command, logger
 from ..config.command import get_cmd_alias
 
 logging.captureWarnings(True)  # 去掉建议使用SSL验证的显示
 
-Version = '2.2.9'  # 全局插件版本信息  （不用加v！）
+Version = '2.2.9.post1'  # 全局插件版本信息  （不用加v！）
 
 
 async def get_datapack_ver():
     """
     检查本地数据包版本
     """
     try:
```

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/data_pack.py` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/utils_/data_pack.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/json_cards.py` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/utils_/json_cards.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/notice_board.py` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/utils_/notice_board.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/travel_cycle.py` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky/utils_/travel_cycle.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky.egg-info/PKG-INFO` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sky
-Version: 2.2.9
+Version: 2.2.9.post1
 Summary: nonebot2 plugin sky
 Home-page: https://github.com/Kaguya233qwq/nonebot_plugin_sky
 Author: Kaguya233qwq
 Author-email: 1435608435@qq.com
 Keywords: pip,nonebot2,nonebot,sky光遇,光遇
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -280,15 +280,15 @@
 
 新浪微博@张张幼稚园 —> *攻略内容*
 
 新浪微博&哔哩哔哩@木易不高兴了啊 —> *攻略内容*
 
 ## ✨更新日志✨
 
-2023.5.30 v2.2.9
+2023.5.30 v2.2.9.post1
 
 这个版本修复了上版本复刻缓存方法调用错误的问题，现在可以智能化识别国服通常复刻周期
 
 2023.5.22 v2.2.8
 
 新增国服通用复刻周期函数，国服复刻已更新，国际服复刻维护中。新增若干随机文案
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sky Version: 2.2.9 Summary: nonebot2
-plugin sky Home-page: https://github.com/Kaguya233qwq/nonebot_plugin_sky
-Author: Kaguya233qwq Author-email: 1435608435@qq.com Keywords:
-pip,nonebot2,nonebot,skyåé,åé Platform: any Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
-Public License v3 (GPLv3) Classifier: Natural Language :: Chinese (Simplified)
-Description-Content-Type: text/markdown License-File: LICENSE
+Metadata-Version: 2.1 Name: nonebot-plugin-sky Version: 2.2.9.post1 Summary:
+nonebot2 plugin sky Home-page: https://github.com/Kaguya233qwq/
+nonebot_plugin_sky Author: Kaguya233qwq Author-email: 1435608435@qq.com
+Keywords: pip,nonebot2,nonebot,skyåé,åé Platform: any Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
+General Public License v3 (GPLv3) Classifier: Natural Language :: Chinese
+(Simplified) Description-Content-Type: text/markdown License-File: LICENSE
                                      [sky]
       # nonebot_plugin_sky _â¨ åºäº [NoneBot2](https://v2.nonebot.dev/
                       ) çåéæ¯æ¥æ»ç¥æä»¶ â¨_
                            [Python] [NoneBot] [pypi]
                              _âå åèéâ_
 # â¨å®è£ä¸é¨ç½²â¨
 ##ä»¥ä¸ä¸ç§ç±»åè¯·éæ©éåèªå·±çæ¹æ¡è¿è¡é¨ç½²ï¼
@@ -106,15 +106,15 @@
 (ç¾¤æä»¶æä¸é®å¯å¨å)
                                      [sky]
 ## â¨æè°¢ååï¼ä¸åååï¼â¨ æ°æµªå¾®å@åéééååå â>
 *æ»ç¥åå®¹* æ°æµªå¾®å@æ§æ¥ä¸æ¥ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@ä»å¤©æ¸¸ç¦»ç¿»è½¦äºå â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@å¼ å¼ å¹¼ç¨å­ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å&åå©åå©@æ¨æä¸é«å´äºå â> *æ»ç¥åå®¹* ##
-â¨æ´æ°æ¥å¿â¨ 2023.5.30 v2.2.9
+â¨æ´æ°æ¥å¿â¨ 2023.5.30 v2.2.9.post1
 è¿ä¸ªçæ¬ä¿®å¤äºä¸çæ¬å¤å»ç¼å­æ¹æ³è°ç¨éè¯¯çé®é¢ï¼ç°å¨å¯ä»¥æºè½åè¯å«å½æéå¸¸å¤å»å¨æ
 2023.5.22 v2.2.8
 æ°å¢å½æéç¨å¤å»å¨æå½æ°ï¼å½æå¤å»å·²æ´æ°ï¼å½éæå¤å»ç»´æ¤ä¸­ãæ°å¢è¥å¹²éæºææ¡
 2023.4.30 v2.2.7
 1.å¨è¿ä¸ªçæ¬ä¹åææquerytoolså½ä»¤ååºå¼ä¸åçæã
 2.æ´æ°å­£èæ¶é´ï¼ææ¶ä¸æ¯å¾åç¡® 2023.4.25 v2.2.6
 1.ä¿®å¤è·åuidå¸®å©å¾çæ æ³åéçé®é¢
```

### Comparing `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky.egg-info/SOURCES.txt` & `nonebot-plugin-sky-2.2.9.post1/nonebot_plugin_sky.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.9/setup.py` & `nonebot-plugin-sky-2.2.9.post1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,25 +6,24 @@
 def get_files(path):
     """获取路径下所有文件相对路径"""
     file_list = []
     files = os.listdir(path)
     for file in files:
         file_list.append(path + '/' + file)
     file_list.append('nonebot_plugin_sky/tools/menu_image/menu.png')
-    file_list.append('nonebot_plugin_sky/sky/get_id.png')
     return file_list
 
 
 Files = get_files(r'nonebot_plugin_sky/tools/helper_image')
 
 with open("README.md", "r", encoding="utf-8", errors="ignore") as f:
     long_description = f.read()
 setuptools.setup(
     name='nonebot-plugin-sky',
-    version='v2.2.9',
+    version='v2.2.9.post1',
     author='Kaguya233qwq',
     author_email='1435608435@qq.com',
     keywords=["pip", "nonebot2", "nonebot", "sky光遇", "光遇"],
     url='https://github.com/Kaguya233qwq/nonebot_plugin_sky',
     description='''nonebot2 plugin sky''',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

