# Comparing `tmp/nonebot_plugin_blacklist-0.3.4.tar.gz` & `tmp/nonebot_plugin_blacklist-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_blacklist-0.3.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_blacklist-0.3.5.tar", max compression
```

## Comparing `nonebot_plugin_blacklist-0.3.4.tar` & `nonebot_plugin_blacklist-0.3.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1066 2023-06-05 01:36:00.636122 nonebot_plugin_blacklist-0.3.4/LICENSE
--rw-r--r--   0        0        0     2550 2023-06-05 01:36:00.636122 nonebot_plugin_blacklist-0.3.4/README.md
--rw-r--r--   0        0        0     8710 2023-06-05 01:36:00.636122 nonebot_plugin_blacklist-0.3.4/nonebot_plugin_blacklist/__init__.py
--rw-r--r--   0        0        0      779 2023-06-05 01:36:00.636122 nonebot_plugin_blacklist-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     3347 1970-01-01 00:00:00.000000 nonebot_plugin_blacklist-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-06 04:50:25.033394 nonebot_plugin_blacklist-0.3.5/LICENSE
+-rw-r--r--   0        0        0     2550 2023-06-06 04:50:25.033394 nonebot_plugin_blacklist-0.3.5/README.md
+-rw-r--r--   0        0        0     8812 2023-06-06 04:50:25.033394 nonebot_plugin_blacklist-0.3.5/nonebot_plugin_blacklist/__init__.py
+-rw-r--r--   0        0        0      779 2023-06-06 04:50:25.033394 nonebot_plugin_blacklist-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     3347 1970-01-01 00:00:00.000000 nonebot_plugin_blacklist-0.3.5/PKG-INFO
```

### Comparing `nonebot_plugin_blacklist-0.3.4/LICENSE` & `nonebot_plugin_blacklist-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blacklist-0.3.4/README.md` & `nonebot_plugin_blacklist-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blacklist-0.3.4/nonebot_plugin_blacklist/__init__.py` & `nonebot_plugin_blacklist-0.3.5/nonebot_plugin_blacklist/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
 def save_blacklist() -> None:
     file_path.write_text(json.dumps(blacklist), encoding='utf-8')
 
 
 if not blacklist.get('ban_auto_sleep'):
     if 'ban_auto_sleep' in blacklist['grouplist']:
+        blacklist['grouplist'] = [ uid for uid in blacklist['grouplist'] if uid != 'ban_auto_sleep' ]
         blacklist.update({'ban_auto_sleep': True})
     else:
         blacklist.update({'ban_auto_sleep': False})
     save_blacklist()
 
 
 def is_number(s: str) -> bool:
```

### Comparing `nonebot_plugin_blacklist-0.3.4/pyproject.toml` & `nonebot_plugin_blacklist-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-blacklist"
-version = "0.3.4"
+version = "0.3.5"
 description = "Blacklist in NoneBot2"
 authors = ["月ヶ瀬"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "nonebot_plugin_blacklist" },
 ]
```

### Comparing `nonebot_plugin_blacklist-0.3.4/PKG-INFO` & `nonebot_plugin_blacklist-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blacklist
-Version: 0.3.4
+Version: 0.3.5
 Summary: Blacklist in NoneBot2
 Home-page: https://github.com/tkgs0/nonebot-plugin-blacklist
 License: MIT
 Keywords: nonebot,blacklist
 Author: 月ヶ瀬
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blacklist Version: 0.3.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-blacklist Version: 0.3.5 Summary:
 Blacklist in NoneBot2 Home-page: https://github.com/tkgs0/nonebot-plugin-
 blacklist License: MIT Keywords: nonebot,blacklist Author: æã¶ç¬ Requires-
 Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: nonebot-adapter-onebot
```

