# Comparing `tmp/nonebot_plugin_treehelp-0.1.0.tar.gz` & `tmp/nonebot_plugin_treehelp-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_treehelp-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_treehelp-0.2.0.tar", max compression
```

## Comparing `nonebot_plugin_treehelp-0.1.0.tar` & `nonebot_plugin_treehelp-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2023-04-16 11:21:40.890225 nonebot_plugin_treehelp-0.1.0/LICENSE
--rw-r--r--   0        0        0     2452 2023-04-16 11:21:40.890225 nonebot_plugin_treehelp-0.1.0/README.md
--rw-r--r--   0        0        0     1495 2023-04-16 11:21:40.890225 nonebot_plugin_treehelp-0.1.0/nonebot_plugin_treehelp/__init__.py
--rw-r--r--   0        0        0     4988 2023-04-16 11:21:40.890225 nonebot_plugin_treehelp-0.1.0/nonebot_plugin_treehelp/data_source.py
--rw-r--r--   0        0        0     1312 2023-04-16 11:21:40.890225 nonebot_plugin_treehelp-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3273 1970-01-01 00:00:00.000000 nonebot_plugin_treehelp-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-06 08:36:24.907264 nonebot_plugin_treehelp-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2452 2023-06-06 08:36:24.907264 nonebot_plugin_treehelp-0.2.0/README.md
+-rw-r--r--   0        0        0     1585 2023-06-06 08:36:24.907264 nonebot_plugin_treehelp-0.2.0/nonebot_plugin_treehelp/__init__.py
+-rw-r--r--   0        0        0     5532 2023-06-06 08:36:24.907264 nonebot_plugin_treehelp-0.2.0/nonebot_plugin_treehelp/data_source.py
+-rw-r--r--   0        0        0     1348 2023-06-06 08:36:24.907264 nonebot_plugin_treehelp-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3266 1970-01-01 00:00:00.000000 nonebot_plugin_treehelp-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_treehelp-0.1.0/LICENSE` & `nonebot_plugin_treehelp-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_treehelp-0.1.0/README.md` & `nonebot_plugin_treehelp-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_treehelp-0.1.0/nonebot_plugin_treehelp/__init__.py` & `nonebot_plugin_treehelp-0.2.0/nonebot_plugin_treehelp/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 /help -t
 /help --tree
 获取某个插件的帮助
 /help 插件名
 获取某个插件的树
 /help --tree 插件名
 """,
+    type="application",
+    homepage="https://github.com/he0119/nonebot-plugin-treehelp",
 )
 
 parser = ArgumentParser("帮助", description="获取插件帮助信息")
 parser.add_argument("plugin_name", nargs="?", type=str, help="插件名", metavar="插件名")
 parser.add_argument("-t", "--tree", action="store_true", help="获取插件树")
 help_cmd = on_shell_command("help", aliases={"帮助"}, parser=parser)
```

### Comparing `nonebot_plugin_treehelp-0.1.0/nonebot_plugin_treehelp/data_source.py` & `nonebot_plugin_treehelp-0.2.0/nonebot_plugin_treehelp/data_source.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,23 +45,57 @@
                 lambda x: f"{x.metadata.name} # {x.metadata.description}",  # type: ignore
                 plugins,
             )
         )
     )
 
 
-def is_supported_adapter(bot: "Bot", plugin: "Plugin") -> bool:
+def is_supported_adapter(bot: "Bot", metadata: "PluginMetadata") -> bool:
     """是否是支持的适配器"""
-    supported_adapters = plugin.metadata.extra.get("adapters")  # type: ignore
-    if (
-        supported_adapters  # 拥有 adapters 信息
-        and isinstance(supported_adapters, (set, list))  # 并且是集合或列表
-        and bot.adapter.get_name() not in supported_adapters  # 且当前适配器名不在集合中
-    ):
+    if metadata.supported_adapters is None:
+        return True
+
+    supported_adapters = metadata.get_supported_adapters()
+    if not supported_adapters:
+        return False
+
+    for adapter in supported_adapters:
+        if isinstance(bot.adapter, adapter):
+            return True
+
+    return False
+
+
+def is_supported_type(metadata: "PluginMetadata") -> bool:
+    """是否是支持的插件类型
+
+    当前有 library 和 application 两种类型
+    仅支持 application 类型的插件
+    """
+    type_ = metadata.type
+    # 如果没有指定类型，则默认支持
+    if type_ is None:
+        return True
+    # 当前仅支持 application 类型
+    if type_ == "application":
+        return True
+    return False
+
+
+def is_supported(bot: "Bot", plugin: "Plugin") -> bool:
+    """是否是支持的插件"""
+    if plugin.metadata is None:
         return False
+
+    if not is_supported_type(plugin.metadata):
+        return False
+
+    if not is_supported_adapter(bot, plugin.metadata):
+        return False
+
     return True
 
 
 def get_plugins() -> Dict[str, "Plugin"]:
     """获取适配了元信息的插件"""
     global _plugins
 
@@ -76,15 +110,15 @@
 
 def get_plugin_list(bot: "Bot", tree: bool = False) -> str:
     """获取插件列表"""
     # 仅保留根插件
     plugins = [
         plugin
         for plugin in get_plugins().values()
-        if plugin.parent_plugin is None and is_supported_adapter(bot, plugin)
+        if plugin.parent_plugin is None and is_supported(bot, plugin)
     ]
     sorted_plugins = sorted(plugins, key=lambda x: x.metadata.name)  # type: ignore
 
     docs = ["插件："]
     if tree:
         for plugin in sorted_plugins:
             docs.append(f"{plugin.metadata.name} # {plugin.metadata.description}")  # type: ignore
@@ -106,29 +140,25 @@
             plugin = _commands.get(tuple(name.split(sep)))
             if plugin:
                 break
     if not plugin:
         return
 
     # 排除不支持的插件
-    if not is_supported_adapter(bot, plugin):
+    if not is_supported(bot, plugin):
         return
 
     metadata = cast("PluginMetadata", plugin.metadata)
 
     if tree:
         docs = [f"{metadata.name} # {metadata.description}"]
         get_tree_string(bot, docs, plugin.sub_plugins, "")
         return "\n".join(docs)
 
-    sub_plugins = [
-        plugin
-        for plugin in plugin.sub_plugins
-        if plugin.metadata is not None and is_supported_adapter(bot, plugin)
-    ]
+    sub_plugins = [plugin for plugin in plugin.sub_plugins if is_supported(bot, plugin)]
     sub_plugins_desc = format_description(sub_plugins)
     return "\n\n".join(
         [x for x in [metadata.name, metadata.usage, sub_plugins_desc] if x]
     )
 
 
 def get_tree_string(
@@ -136,17 +166,15 @@
     docs: List[str],
     plugins: Set["Plugin"],
     previous_tree_bar: str,
 ) -> None:
     """通过递归获取树形结构的字符串"""
     previous_tree_bar = previous_tree_bar.replace("├", "│")
 
-    filtered_plugins = filter(
-        lambda x: x.metadata is not None and is_supported_adapter(bot, x), plugins
-    )
+    filtered_plugins = filter(lambda x: is_supported(bot, x), plugins)
     sorted_plugins = sorted(filtered_plugins, key=lambda x: x.metadata.name)  # type: ignore
 
     tree_bar = previous_tree_bar + "├"
     total = len(sorted_plugins)
     for i, plugin in enumerate(sorted_plugins, 1):
         if i == total:
             tree_bar = previous_tree_bar + "└"
```

### Comparing `nonebot_plugin_treehelp-0.1.0/pyproject.toml` & `nonebot_plugin_treehelp-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 [tool.poetry]
 name = "nonebot-plugin-treehelp"
-version = "0.1.0"
+version = "0.2.0"
 description = "适用于 Nonebot2 的树形帮助插件"
 authors = ["hemengyang <hmy0119@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/he0119/nonebot-plugin-treehelp"
 repository = "https://github.com/he0119/nonebot-plugin-treehelp"
 documentation = "https://github.com/he0119/nonebot-plugin-treehelp#readme"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-nonebot2 = "^2.0.0-beta.5"
+nonebot2 = "^2.0.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 isort = "*"
 pre-commit = "*"
-nonebot-adapter-console = "^0.3.2"
 nb-cli = "^1.0.4"
+nonebot-adapter-console = "^0.3.2"
+nonebot-adapter-onebot = "^2.2.3"
 
 [tool.poetry.group.test.dependencies]
 nonebug = "^0.3.1"
 pytest-cov = "^4.0.0"
 pytest-xdist = "^3.0.2"
 pytest-mock = "^3.10.0"
-pytest-asyncio = "^0.20.2"
+pytest-asyncio = ">=0.20.2,<0.22.0"
 
 [tool.black]
 line-length = 88
 
 [tool.isort]
 profile = "black"
 line_length = 88
```

### Comparing `nonebot_plugin_treehelp-0.1.0/PKG-INFO` & `nonebot_plugin_treehelp-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-treehelp
-Version: 0.1.0
+Version: 0.2.0
 Summary: 适用于 Nonebot2 的树形帮助插件
 Home-page: https://github.com/he0119/nonebot-plugin-treehelp
 License: MIT
 Author: hemengyang
 Author-email: hmy0119@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: nonebot2 (>=2.0.0-beta.5,<3.0.0)
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Project-URL: Documentation, https://github.com/he0119/nonebot-plugin-treehelp#readme
 Project-URL: Repository, https://github.com/he0119/nonebot-plugin-treehelp
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-treehelp Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-treehelp Version: 0.2.0 Summary:
 éç¨äº Nonebot2 çæ å½¢å¸®å©æä»¶ Home-page: https://github.com/he0119/
 nonebot-plugin-treehelp License: MIT Author: hemengyang Author-email:
 hmy0119@gmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: nonebot2
-(>=2.0.0-beta.5,<3.0.0) Project-URL: Documentation, https://github.com/he0119/
-nonebot-plugin-treehelp#readme Project-URL: Repository, https://github.com/
-he0119/nonebot-plugin-treehelp Description-Content-Type: text/markdown
+(>=2.0.0,<3.0.0) Project-URL: Documentation, https://github.com/he0119/nonebot-
+plugin-treehelp#readme Project-URL: Repository, https://github.com/he0119/
+nonebot-plugin-treehelp Description-Content-Type: text/markdown
                                    [nonebot]
         # NoneBot Plugin TreeHelp _â¨ NoneBot æ å½¢å¸®å©æä»¶ â¨_
     [license] [pypi] [python] [https://codecov.io/gh/he0119/nonebot-plugin-
     treehelp/branch/main/graph/badge.svg?token=jd5ufc1alv] [QQ_Chat_Group]
 ## ç®ä»
 ä½¿ç¨æä»¶åæ°æ®è·åæä»¶ä¿¡æ¯ï¼å¹¶éè¿æä»¶ä¸å­æä»¶çç»ç»å½¢å¼ï¼æ¥åºåæä»¶çå¤ç§åè½ã
 æ å½¢å¸®å©æä»¶ï¼æéè¦çåè½å½ç¶æ¯æ¾ç¤ºæä»¶æ ï¼ åé `/
```

