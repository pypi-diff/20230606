# Comparing `tmp/nonebot_plugin_help-0.4.1.tar.gz` & `tmp/nonebot_plugin_help-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_help-0.4.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_help-0.5.0.tar", max compression
```

## Comparing `nonebot_plugin_help-0.4.1.tar` & `nonebot_plugin_help-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35184 2022-06-21 14:58:39.859249 nonebot_plugin_help-0.4.1/LICENSE
--rw-r--r--   0        0        0     1314 2023-04-21 16:15:46.665784 nonebot_plugin_help-0.4.1/nonebot_plugin_help/__init__.py
--rw-r--r--   0        0        0      220 2023-04-21 15:54:22.509482 nonebot_plugin_help-0.4.1/nonebot_plugin_help/config.py
--rw-r--r--   0        0        0     5147 2023-04-21 16:17:29.869180 nonebot_plugin_help-0.4.1/nonebot_plugin_help/handler.py
--rw-r--r--   0        0        0      577 2023-04-21 16:16:18.944552 nonebot_plugin_help-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     6433 2023-04-21 16:16:07.364334 nonebot_plugin_help-0.4.1/README.md
--rw-r--r--   0        0        0     7020 1970-01-01 00:00:00.000000 nonebot_plugin_help-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-06-21 14:58:39.859249 nonebot_plugin_help-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1314 2023-06-06 14:57:51.950180 nonebot_plugin_help-0.5.0/nonebot_plugin_help/__init__.py
+-rw-r--r--   0        0        0      220 2023-04-21 15:54:22.509482 nonebot_plugin_help-0.5.0/nonebot_plugin_help/config.py
+-rw-r--r--   0        0        0     5147 2023-04-21 16:17:29.869180 nonebot_plugin_help-0.5.0/nonebot_plugin_help/handler.py
+-rw-r--r--   0        0        0      570 2023-06-06 14:48:35.601209 nonebot_plugin_help-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6433 2023-04-21 16:16:07.364334 nonebot_plugin_help-0.5.0/README.md
+-rw-r--r--   0        0        0     7013 1970-01-01 00:00:00.000000 nonebot_plugin_help-0.5.0/PKG-INFO
```

### Comparing `nonebot_plugin_help-0.4.1/LICENSE` & `nonebot_plugin_help-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_help-0.4.1/nonebot_plugin_help/__init__.py` & `nonebot_plugin_help-0.5.0/nonebot_plugin_help/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .handler import helper
 
 
 default_start = list(nonebot.get_driver().config.command_start)[0]
 
 # Legacy way of self registering (use custom attributes)
 # Deprecated for nonebot-plugin-help 0.3.1+, prefer PluginMetadata.extra['version']
-__help_version__ = '0.4.1'
+__help_version__ = '0.5.0'
 # Deprecated for nonebot-plugin-help 0.3.0+, prefer PluginMetadata.name
 __help_plugin_name__ = "Nonebot2 Help Menu"
 # Deprecated for nonebot-plugin-help 0.3.0+, prefer PluginMetadata.usage
 __usage__ = f'''欢迎使用Nonebot2 Help Menu
 本插件提供公共帮助菜单能力
 此Bot配置的命令前缀：{" ".join(list(nonebot.get_driver().config.command_start))}
 '''
@@ -28,9 +28,9 @@
 本插件提供公共帮助菜单能力
 此Bot配置的命令前缀：{" ".join(list(nonebot.get_driver().config.command_start))}
 
 {default_start}help  # 获取本插件帮助
 {default_start}help list  # 展示已加载插件列表
 {default_start}help <插件名>  # 调取目标插件帮助信息
 ''',
-    extra={'version': '0.4.1'}
+    extra={'version': '0.5.0'}
 )
```

### Comparing `nonebot_plugin_help-0.4.1/nonebot_plugin_help/handler.py` & `nonebot_plugin_help-0.5.0/nonebot_plugin_help/handler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_help-0.4.1/pyproject.toml` & `nonebot_plugin_help-0.5.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "nonebot-plugin-help"
-version = "0.4.1"
+version = "0.5.0"
 description = "A general help lister for nonebot2 plugins"
 authors = ["XZhouQD <X.Zhou.QD@hotmail.com>"]
 license = "AGPL v3"
 readme = "README.md"
 homepage = "https://github.com/XZhouQD/nonebot-plugin-help"
 repository = "https://github.com/XZhouQD/nonebot-plugin-help"
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
-nonebot2 = "^2.0.0-beta.4"
+nonebot2 = "^2.0.0"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_help-0.4.1/README.md` & `nonebot_plugin_help-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_help-0.4.1/PKG-INFO` & `nonebot_plugin_help-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-help
-Version: 0.4.1
+Version: 0.5.0
 Summary: A general help lister for nonebot2 plugins
 Home-page: https://github.com/XZhouQD/nonebot-plugin-help
 License: AGPL v3
 Author: XZhouQD
 Author-email: X.Zhou.QD@hotmail.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: nonebot2 (>=2.0.0-beta.4,<3.0.0)
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/XZhouQD/nonebot-plugin-help
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # nonebot-plugin-help
 ### Nonebot2 轻量级帮助插件
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-help Version: 0.4.1 Summary: A
+Metadata-Version: 2.1 Name: nonebot-plugin-help Version: 0.5.0 Summary: A
 general help lister for nonebot2 plugins Home-page: https://github.com/XZhouQD/
 nonebot-plugin-help License: AGPL v3 Author: XZhouQD Author-email:
 X.Zhou.QD@hotmail.com Requires-Python: >=3.8.0,<4.0.0 Classifier: License ::
 Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: nonebot2
-(>=2.0.0-beta.4,<3.0.0) Project-URL: Repository, https://github.com/XZhouQD/
-nonebot-plugin-help Description-Content-Type: text/markdown
+(>=2.0.0,<3.0.0) Project-URL: Repository, https://github.com/XZhouQD/nonebot-
+plugin-help Description-Content-Type: text/markdown
 # nonebot-plugin-help ### Nonebot2 è½»éçº§å¸®å©æä»¶ [license] [pypi] [pypi
                               download] [python]
                           [python] [python] [nonebot]
 ## éç½®helpæä»¶ä¼åçº§ä¸é»å¡ï¼å¯éï¼ ![nonebot-plugin-help](https:
 //img.shields.io/static/v1?label=nonebot-plugin-help&message=0.4.0&color=red)
 0.4.0çæ¬èµ·ï¼æ°å¢æä»¶ä¼åçº§ä¸é»å¡è®¾ç½®ï¼å¯éï¼ï¼é»è®¤ä¸º`priority=1,
 block=False`
```

