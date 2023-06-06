# Comparing `tmp/findmyorder-1.3.8.tar.gz` & `tmp/findmyorder-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.3.8.tar", max compression
+gzip compressed data, was "findmyorder-1.3.9.tar", max compression
```

## Comparing `findmyorder-1.3.8.tar` & `findmyorder-1.3.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-05-08 17:03:16.348122 findmyorder-1.3.8/LICENSE
--rw-r--r--   0        0        0     2155 2023-05-08 17:03:16.348122 findmyorder-1.3.8/README.md
--rw-r--r--   0        0        0      113 2023-05-08 17:03:17.192171 findmyorder-1.3.8/findmyorder/__init__.py
--rw-r--r--   0        0        0      630 2023-05-08 17:03:16.348122 findmyorder-1.3.8/findmyorder/config.py
--rw-r--r--   0        0        0      566 2023-05-08 17:03:16.348122 findmyorder-1.3.8/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     4116 2023-05-08 17:03:16.348122 findmyorder-1.3.8/findmyorder/main.py
--rw-r--r--   0        0        0     1758 2023-05-08 17:03:17.192171 findmyorder-1.3.8/pyproject.toml
--rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 findmyorder-1.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-22 19:47:29.499663 findmyorder-1.3.9/LICENSE
+-rw-r--r--   0        0        0     2090 2023-05-22 19:47:29.499663 findmyorder-1.3.9/README.md
+-rw-r--r--   0        0        0      113 2023-05-22 19:47:30.359736 findmyorder-1.3.9/findmyorder/__init__.py
+-rw-r--r--   0        0        0      630 2023-05-22 19:47:29.503663 findmyorder-1.3.9/findmyorder/config.py
+-rw-r--r--   0        0        0      615 2023-05-22 19:47:29.503663 findmyorder-1.3.9/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     6383 2023-05-22 19:47:29.503663 findmyorder-1.3.9/findmyorder/main.py
+-rw-r--r--   0        0        0     2042 2023-05-22 19:47:30.359736 findmyorder-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0     2951 1970-01-01 00:00:00.000000 findmyorder-1.3.9/PKG-INFO
```

### Comparing `findmyorder-1.3.8/LICENSE` & `findmyorder-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.3.8/README.md` & `findmyorder-1.3.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,66 @@
-# Find my order
+Metadata-Version: 2.1
+Name: findmyorder
+Version: 1.3.9
+Summary: A python package to identify and parse order for trade execution.
+License: MIT
+Keywords: trading,order,trade,buy,sell
+Author: mraniki
+Author-email: 8766259+mraniki@users.noreply.github.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: asyncio
+Requires-Dist: dynaconf
+Requires-Dist: emoji
+Requires-Dist: pyparsing (>=3.0.9,<4.0.0)
+Project-URL: Changelog, https://github.com/mraniki/findmyorder/blob/dev/CHANGELOG.rst
+Project-URL: Issues, https://github.com/mraniki/findmyorder/issues
+Project-URL: Support, https://github.com/mraniki/findmyorder/discussions
+Description-Content-Type: text/markdown
 
+# Find my order
 
-| <img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/233823991-cceaa05a-ff15-4796-a6bb-bcb3ee0d8859.jpg"> | A python package to identify and parse order for trade execution. |
+| <img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/233823991-cceaa05a-ff15-4796-a6bb-bcb3ee0d8859.jpg"> | A python package to identify and <br>parse order for trade execution. |
 | ------------- | ------------- |
 |[![Pypi](https://badgen.net/badge/icon/findmyorder?icon=pypi&label)](https://pypi.org/project/findmyorder/) ![Version](https://img.shields.io/pypi/v/findmyorder)<br>  ![Pypi](https://img.shields.io/pypi/dm/findmyorder)<br> [![Build](https://github.com/mraniki/findmyorder/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/findmyorder/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/findmyorder/branch/dev/graph/badge.svg?token=4838MSZNCC)](https://codecov.io/gh/mraniki/findmyorder) | Find & Parse a trade order for execution|
 
-
 Key features:
 
 - Identify an order with word `BUY SELL LONG SHORT` or your own `Bull`, `to the moon`, `pump` via config file
 - Parse and return a structured order with action and instrument as mandatory
 - Settings for custom option
 
+## Install
 
-
-
-# Install
 `pip install findmyorder`
 
-# How to use it
+## How to use it
+
 ```
 fmo = FindMyOrder()
 msg_order = "buy EURUSD sl=1000 tp=1000 q=1 comment=FOMC"
 order = await fmo.get_order(msg_order)
 #{'action': 'BUY', 'instrument': 'EURUSD', 'stop_loss': '1000', 'take_profit': '1000', 'quantity': '2', 'order_type': None, 'leverage_type': None, 'comment': None, 'timestamp': datetime.datetime(2023, 5, 3, 12, 10, 28, 731282, tzinfo=datetime.timezone.utc)}
 ```
-## Example
+
+### Example
+
 [example](https://github.com/mraniki/findmyorder/blob/main/examples/example.py)
 
-## Real use case
+### Real use case
+
 [TalkyTrader, submit trading order to CEX & DEX with messaging platform (Telegram, Matrix and Discord)](https://github.com/mraniki/tt)
 
+## Documentation
 
-# Documentation
-https://github.com/mraniki/findmyorder/wiki
+[Wiki](https://github.com/mraniki/findmyorder/wiki)
 
-## 🚧 Roadmap
 
-[🚧 Roadmap](https://github.com/mraniki/findmyorder/milestones)
+## Questions? Want to help?
 
-## Questions? Want to help? 
 [![discord](https://badgen.net/badge/icon/discord/purple?icon=discord&label)](https://discord.gg/vegJQGrRRa)
 [![telegram](https://badgen.net/badge/icon/telegram?icon=telegram&label)](https://t.me/TTTalkyTraderChat/1)
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `findmyorder-1.3.8/findmyorder/config.py` & `findmyorder-1.3.9/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.3.8/findmyorder/default_settings.toml` & `findmyorder-1.3.9/findmyorder/default_settings.toml`

 * *Files 18% similar despite different names*

```diff
@@ -10,11 +10,14 @@
 ]
 stop_loss_identifier = "sl="
 take_profit_identifier = 'tp='
 quantity_identifier = 'q='
 order_type_identifier = "spot future margin"
 leverage_type_identifier = "cross isolated"
 comment_identifier = "comment="
+stop_loss = 1000
+take_profit = 1000
+quantity = 1
 VALUE = "On Default"
 
 [testing]
 VALUE = "On Testing"
```

### Comparing `findmyorder-1.3.8/pyproject.toml` & `findmyorder-1.3.9/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 [tool.poetry]
 name = "findmyorder"
-version = "1.3.8"
+version = "1.3.9"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
 
-
 [tool.poetry.urls]
 "Changelog" =  "https://github.com/mraniki/findmyorder/blob/dev/CHANGELOG.rst"
 "Support" =  "https://github.com/mraniki/findmyorder/discussions"
 "Issues" =  "https://github.com/mraniki/findmyorder/issues"
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.11"
-dynaconf = ">=3.1.12"
-pyparsing = ">=3.0.9"
+python = "^3.10"
+asyncio = "*"
+dynaconf = "*"
+pyparsing = "^3.0.9"
+emoji = "*"
 
 [tool.poetry.dev-dependencies]
 python-semantic-release = "*"
 pytest = "*"
 pytest-cov = "*"
 pytest-asyncio = "*"
+pytest-mock = "*"
 
 [tool.pytest.ini_options]
 testpaths = "tests/"
 python_classes = [
   "Test*",
   "*Test"
 ]
@@ -41,21 +43,17 @@
 version_variable = ["pyproject.toml:version","findmyorder/__init__.py:__version__"]
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "pip install poetry && poetry build"
 commit_parser = "semantic_release.history.emoji_parser"
 use_textual_changelog_sections = true
-
-#patch_emoji
-# 🐛🚑🤖🏁🔒👽🔍💬🥅⚡♿🍏🐧
-#:ambulance:, :lock:, :bug:, :zap:, :goal_net:, :alien:, :wheelchair:, :speech_balloon:, :mag:, :apple:, :penguin:, :checkered_flag:, :robot:, :green_apple
-#minor_emoji
-#✨🥚🚸📱💄📈
-#:sparkles: ✨, :children_crossing:, :lipstick:, :iphone:, :egg:, :chart_with_upwards_trend
-#major_emoji¶
-#💥
-# :boom:
+major_emoji = ":boom:"
+#major_emoji¶ #💥:boom:
+minor_emoji = ":sparkles:,:children_crossing:,:lipstick:,:iphone:,:egg:,:chart_with_upwards_trend:"
+#minor_emoji #✨🥚🚸📱💄📈
+patch_emoji = ":ambulance:,:lock:,:arrow_up:,:bug:,:zap:,:goal_net:,:alien:,:wheelchair:,:speech_balloon:,:mag:,:apple:,:penguin:,:checkered_flag:,:robot:,:green_apple:,⚡️,🎨,🐛,🚑️,💄,🔒️,⬇️,⬆️,📌,📈,➕,➖,🔧,🌐,✏️,⏪️,📦️,👽️,🍱,♿️,💬,🗃️ ,🚸,📱,🥚,⚗️,🔍️,🏷️ ,🚩,🥅,💫,🗑️ ,🛂,🩹,👔,"
+#patch_emoji # 🐛🚑⚡🔒👽🔍💬🥅♿🍏🐧🏁🤖
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `findmyorder-1.3.8/PKG-INFO` & `findmyorder-1.3.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,65 +1,43 @@
-Metadata-Version: 2.1
-Name: findmyorder
-Version: 1.3.8
-Summary: A python package to identify and parse order for trade execution.
-License: MIT
-Keywords: trading,order,trade,buy,sell
-Author: mraniki
-Author-email: 8766259+mraniki@users.noreply.github.com
-Requires-Python: >=3.9,<3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: dynaconf (>=3.1.12)
-Requires-Dist: pyparsing (>=3.0.9)
-Project-URL: Changelog, https://github.com/mraniki/findmyorder/blob/dev/CHANGELOG.rst
-Project-URL: Issues, https://github.com/mraniki/findmyorder/issues
-Project-URL: Support, https://github.com/mraniki/findmyorder/discussions
-Description-Content-Type: text/markdown
-
 # Find my order
 
-
-| <img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/233823991-cceaa05a-ff15-4796-a6bb-bcb3ee0d8859.jpg"> | A python package to identify and parse order for trade execution. |
+| <img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/233823991-cceaa05a-ff15-4796-a6bb-bcb3ee0d8859.jpg"> | A python package to identify and <br>parse order for trade execution. |
 | ------------- | ------------- |
 |[![Pypi](https://badgen.net/badge/icon/findmyorder?icon=pypi&label)](https://pypi.org/project/findmyorder/) ![Version](https://img.shields.io/pypi/v/findmyorder)<br>  ![Pypi](https://img.shields.io/pypi/dm/findmyorder)<br> [![Build](https://github.com/mraniki/findmyorder/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/findmyorder/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/findmyorder/branch/dev/graph/badge.svg?token=4838MSZNCC)](https://codecov.io/gh/mraniki/findmyorder) | Find & Parse a trade order for execution|
 
-
 Key features:
 
 - Identify an order with word `BUY SELL LONG SHORT` or your own `Bull`, `to the moon`, `pump` via config file
 - Parse and return a structured order with action and instrument as mandatory
 - Settings for custom option
 
+## Install
 
-
-
-# Install
 `pip install findmyorder`
 
-# How to use it
+## How to use it
+
 ```
 fmo = FindMyOrder()
 msg_order = "buy EURUSD sl=1000 tp=1000 q=1 comment=FOMC"
 order = await fmo.get_order(msg_order)
 #{'action': 'BUY', 'instrument': 'EURUSD', 'stop_loss': '1000', 'take_profit': '1000', 'quantity': '2', 'order_type': None, 'leverage_type': None, 'comment': None, 'timestamp': datetime.datetime(2023, 5, 3, 12, 10, 28, 731282, tzinfo=datetime.timezone.utc)}
 ```
-## Example
+
+### Example
+
 [example](https://github.com/mraniki/findmyorder/blob/main/examples/example.py)
 
-## Real use case
+### Real use case
+
 [TalkyTrader, submit trading order to CEX & DEX with messaging platform (Telegram, Matrix and Discord)](https://github.com/mraniki/tt)
 
+## Documentation
 
-# Documentation
-https://github.com/mraniki/findmyorder/wiki
+[Wiki](https://github.com/mraniki/findmyorder/wiki)
 
-## 🚧 Roadmap
 
-[🚧 Roadmap](https://github.com/mraniki/findmyorder/milestones)
+## Questions? Want to help?
 
-## Questions? Want to help? 
 [![discord](https://badgen.net/badge/icon/discord/purple?icon=discord&label)](https://discord.gg/vegJQGrRRa)
 [![telegram](https://badgen.net/badge/icon/telegram?icon=telegram&label)](https://t.me/TTTalkyTraderChat/1)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

