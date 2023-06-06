# Comparing `tmp/nonebot_plugin_datastore-0.6.3.tar.gz` & `tmp/nonebot_plugin_datastore-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_datastore-0.6.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_datastore-1.0.0.tar", max compression
```

## Comparing `nonebot_plugin_datastore-0.6.3.tar` & `nonebot_plugin_datastore-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1067 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/LICENSE
--rw-r--r--   0        0        0     7564 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/README.md
--rw-r--r--   0        0        0      259 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/__init__.py
--rw-r--r--   0        0        0     1772 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/config.py
--rw-r--r--   0        0        0     4093 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/db.py
--rw-r--r--   0        0        0      804 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/migrations/0f8d23241fd7_.py
--rw-r--r--   0        0        0     8844 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/plugin.py
--rw-r--r--   0        0        0     1487 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/providers/__init__.py
--rw-r--r--   0        0        0     1226 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/providers/database.py
--rw-r--r--   0        0        0     1530 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/providers/json.py
--rw-r--r--   0        0        0     1635 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/providers/toml.py
--rw-r--r--   0        0        0     1816 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/providers/yaml.py
--rw-r--r--   0        0        0        0 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/py.typed
--rw-r--r--   0        0        0        0 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/script/__init__.py
--rw-r--r--   0        0        0     6372 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/script/cli.py
--rw-r--r--   0        0        0    12170 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/script/command.py
--rw-r--r--   0        0        0      510 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/script/migration/script.py.mako
--rw-r--r--   0        0        0     3611 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/script/utils.py
--rw-r--r--   0        0        0     1889 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/utils.py
--rw-r--r--   0        0        0     2085 2023-04-24 14:44:07.043758 nonebot_plugin_datastore-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     8994 1970-01-01 00:00:00.000000 nonebot_plugin_datastore-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/LICENSE
+-rw-r--r--   0        0        0     7564 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/README.md
+-rw-r--r--   0        0        0      572 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/__init__.py
+-rw-r--r--   0        0        0     1772 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/config.py
+-rw-r--r--   0        0        0     4093 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/db.py
+-rw-r--r--   0        0        0      804 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/migrations/0f8d23241fd7_.py
+-rw-r--r--   0        0        0     8844 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/plugin.py
+-rw-r--r--   0        0        0     1487 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/providers/__init__.py
+-rw-r--r--   0        0        0     1226 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/providers/database.py
+-rw-r--r--   0        0        0     1530 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/providers/json.py
+-rw-r--r--   0        0        0     1635 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/providers/toml.py
+-rw-r--r--   0        0        0     1816 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/providers/yaml.py
+-rw-r--r--   0        0        0        0 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/py.typed
+-rw-r--r--   0        0        0        0 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/script/__init__.py
+-rw-r--r--   0        0        0     6372 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/script/cli.py
+-rw-r--r--   0        0        0    12170 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/script/command.py
+-rw-r--r--   0        0        0      510 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/script/migration/script.py.mako
+-rw-r--r--   0        0        0     3611 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/script/utils.py
+-rw-r--r--   0        0        0     1889 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/utils.py
+-rw-r--r--   0        0        0     2075 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     8989 1970-01-01 00:00:00.000000 nonebot_plugin_datastore-1.0.0/PKG-INFO
```

### Comparing `nonebot_plugin_datastore-0.6.3/LICENSE` & `nonebot_plugin_datastore-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-0.6.3/README.md` & `nonebot_plugin_datastore-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/config.py` & `nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/db.py` & `nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/migrations/0f8d23241fd7_.py` & `nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/migrations/0f8d23241fd7_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/plugin.py` & `nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/plugin.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/providers/__init__.py` & `nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/providers/database.py` & `nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/providers/database.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/providers/json.py` & `nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/providers/json.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/providers/toml.py` & `nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/providers/toml.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/providers/yaml.py` & `nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/providers/yaml.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/script/cli.py` & `nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/script/cli.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/script/command.py` & `nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/script/command.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/script/utils.py` & `nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/script/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/utils.py` & `nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-0.6.3/pyproject.toml` & `nonebot_plugin_datastore-1.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "nonebot-plugin-datastore"
-version = "0.6.3"
+version = "1.0.0"
 description = "适用于 Nonebot2 的数据存储插件"
 authors = ["hemengyang <hmy0119@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/he0119/nonebot-plugin-datastore"
 repository = "https://github.com/he0119/nonebot-plugin-datastore"
 documentation = "https://github.com/he0119/nonebot-plugin-datastore#readme"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-nonebot2 = { extras = ["httpx"], version = "^2.0.0-rc.1" }
-nonebot-plugin-localstore = ">=0.2.0,!=0.3.0,!=0.4.0,<0.5.0"
+nonebot2 = { extras = ["httpx"], version = "^2.0.0" }
+nonebot-plugin-localstore = ">=0.2.0,!=0.3.0,!=0.4.0,<0.6.0"
 sqlalchemy = { extras = ["aiosqlite"], version = "^2.0.0" }
 alembic = "^1.9.1"
 
 anyio = { version = ">=3.6", optional = true }
 click = { version = ">=8.0", optional = true }
 typing-extensions = { version = ">=4.4", optional = true }
 rtoml = { version = "^0.9.0", optional = true }
@@ -28,15 +28,15 @@
 pre-commit = "*"
 nonebug = "^0.3.1"
 pytest-cov = "^4.0.0"
 pytest-xdist = "^3.1.0"
 pytest-mock = "^3.10.0"
 pytest-asyncio = ">=0.20.3,<0.22.0"
 nb-cli = "^1.0.0"
-nonebot2 = { extras = ["httpx", "fastapi"], version = "^2.0.0-rc.1" }
+nonebot2 = { extras = ["httpx", "fastapi"], version = "^2.0.0" }
 
 [tool.poetry.extras]
 cli = ["anyio", "click", "typing-extensions"]
 toml = ["rtoml"]
 yaml = ["pyyaml"]
 all = ["anyio", "click", "typing-extensions", "rtoml", "pyyaml"]
```

### Comparing `nonebot_plugin_datastore-0.6.3/PKG-INFO` & `nonebot_plugin_datastore-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-datastore
-Version: 0.6.3
+Version: 1.0.0
 Summary: 适用于 Nonebot2 的数据存储插件
 Home-page: https://github.com/he0119/nonebot-plugin-datastore
 License: MIT
 Author: hemengyang
 Author-email: hmy0119@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -16,16 +16,16 @@
 Provides-Extra: all
 Provides-Extra: cli
 Provides-Extra: toml
 Provides-Extra: yaml
 Requires-Dist: alembic (>=1.9.1,<2.0.0)
 Requires-Dist: anyio (>=3.6) ; extra == "cli" or extra == "all"
 Requires-Dist: click (>=8.0) ; extra == "cli" or extra == "all"
-Requires-Dist: nonebot-plugin-localstore (>=0.2.0,!=0.3.0,!=0.4.0,<0.5.0)
-Requires-Dist: nonebot2[httpx] (>=2.0.0-rc.1,<3.0.0)
+Requires-Dist: nonebot-plugin-localstore (>=0.2.0,!=0.3.0,!=0.4.0,<0.6.0)
+Requires-Dist: nonebot2[httpx] (>=2.0.0,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0) ; extra == "yaml" or extra == "all"
 Requires-Dist: rtoml (>=0.9.0,<0.10.0) ; extra == "toml" or extra == "all"
 Requires-Dist: sqlalchemy[aiosqlite] (>=2.0.0,<3.0.0)
 Requires-Dist: typing-extensions (>=4.4) ; extra == "cli" or extra == "all"
 Project-URL: Documentation, https://github.com/he0119/nonebot-plugin-datastore#readme
 Project-URL: Repository, https://github.com/he0119/nonebot-plugin-datastore
 Description-Content-Type: text/markdown
```

