# Comparing `tmp/smarterbombing-0.1.4.tar.gz` & `tmp/smarterbombing-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smarterbombing-0.1.4.tar", max compression
+gzip compressed data, was "smarterbombing-0.1.5.tar", max compression
```

## Comparing `smarterbombing-0.1.4.tar` & `smarterbombing-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1071 2023-06-06 15:53:04.925068 smarterbombing-0.1.4/LICENSE
--rw-r--r--   0        0        0      684 2023-06-06 15:53:04.925068 smarterbombing-0.1.4/README.md
--rw-r--r--   0        0        0      860 2023-06-06 15:53:37.348858 smarterbombing-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      116 2023-06-06 15:53:04.925068 smarterbombing-0.1.4/src/smarterbombing/__init__.py
--rw-r--r--   0        0        0      769 2023-06-06 15:53:04.925068 smarterbombing-0.1.4/src/smarterbombing/__main__.py
--rw-r--r--   0        0        0    10637 2023-06-06 15:53:04.925068 smarterbombing-0.1.4/src/smarterbombing/analysis.py
--rw-r--r--   0        0        0     5473 2023-06-06 15:53:04.925068 smarterbombing-0.1.4/src/smarterbombing/app_live.py
--rw-r--r--   0        0        0     2979 2023-06-06 15:53:04.925068 smarterbombing-0.1.4/src/smarterbombing/app_offline.py
--rw-r--r--   0        0        0      817 2023-06-06 15:53:04.925068 smarterbombing-0.1.4/src/smarterbombing/configuration.py
--rw-r--r--   0        0        0     3648 2023-06-06 15:53:04.925068 smarterbombing-0.1.4/src/smarterbombing/log_reader.py
--rw-r--r--   0        0        0     3533 2023-06-06 15:53:04.925068 smarterbombing-0.1.4/src/smarterbombing/logs.py
--rw-r--r--   0        0        0        0 2023-06-06 15:53:04.925068 smarterbombing-0.1.4/src/smarterbombing/webui/__init__.py
--rw-r--r--   0        0        0     1104 2023-06-06 15:53:04.925068 smarterbombing-0.1.4/src/smarterbombing/webui/ui.py
--rw-r--r--   0        0        0     1837 2023-06-06 15:53:04.925068 smarterbombing-0.1.4/src/smarterbombing/webui/ui_configuration.py
--rw-r--r--   0        0        0     5546 2023-06-06 15:53:04.925068 smarterbombing-0.1.4/src/smarterbombing/webui/ui_live.py
--rw-r--r--   0        0        0     4199 2023-06-06 15:53:04.925068 smarterbombing-0.1.4/src/smarterbombing/webui/ui_offline_analysis.py
--rw-r--r--   0        0        0     1600 1970-01-01 00:00:00.000000 smarterbombing-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-06 16:29:40.163005 smarterbombing-0.1.5/LICENSE
+-rw-r--r--   0        0        0      782 2023-06-06 16:29:40.163005 smarterbombing-0.1.5/README.md
+-rw-r--r--   0        0        0      860 2023-06-06 16:30:11.348100 smarterbombing-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      116 2023-06-06 16:29:40.163005 smarterbombing-0.1.5/src/smarterbombing/__init__.py
+-rw-r--r--   0        0        0      769 2023-06-06 16:29:40.163005 smarterbombing-0.1.5/src/smarterbombing/__main__.py
+-rw-r--r--   0        0        0    10637 2023-06-06 16:29:40.163005 smarterbombing-0.1.5/src/smarterbombing/analysis.py
+-rw-r--r--   0        0        0     5473 2023-06-06 16:29:40.163005 smarterbombing-0.1.5/src/smarterbombing/app_live.py
+-rw-r--r--   0        0        0     2979 2023-06-06 16:29:40.163005 smarterbombing-0.1.5/src/smarterbombing/app_offline.py
+-rw-r--r--   0        0        0      817 2023-06-06 16:29:40.163005 smarterbombing-0.1.5/src/smarterbombing/configuration.py
+-rw-r--r--   0        0        0     3648 2023-06-06 16:29:40.163005 smarterbombing-0.1.5/src/smarterbombing/log_reader.py
+-rw-r--r--   0        0        0     3533 2023-06-06 16:29:40.163005 smarterbombing-0.1.5/src/smarterbombing/logs.py
+-rw-r--r--   0        0        0        0 2023-06-06 16:29:40.163005 smarterbombing-0.1.5/src/smarterbombing/webui/__init__.py
+-rw-r--r--   0        0        0     1104 2023-06-06 16:29:40.163005 smarterbombing-0.1.5/src/smarterbombing/webui/ui.py
+-rw-r--r--   0        0        0     1837 2023-06-06 16:29:40.163005 smarterbombing-0.1.5/src/smarterbombing/webui/ui_configuration.py
+-rw-r--r--   0        0        0     5546 2023-06-06 16:29:40.163005 smarterbombing-0.1.5/src/smarterbombing/webui/ui_live.py
+-rw-r--r--   0        0        0     4199 2023-06-06 16:29:40.163005 smarterbombing-0.1.5/src/smarterbombing/webui/ui_offline_analysis.py
+-rw-r--r--   0        0        0     1698 1970-01-01 00:00:00.000000 smarterbombing-0.1.5/PKG-INFO
```

### Comparing `smarterbombing-0.1.4/LICENSE` & `smarterbombing-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.4/README.md` & `smarterbombing-0.1.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 # Eve Smarterbombing
 An application analyzing Eve Online combat logs and presenting data in a Web interface.
 
-## Quick Start
+## ⚡ Quick Start
+
+### From PyPI
+```shell
+pip install smarterbombing
+python -m smarterbombing
+```
+
+### From Source
 ```shell
 poetry install
 poetry run python -m smarterbombing
 ```
 Open with your preferred browser:
 - Open [Web UI](http://localhost:42069)
 - Open [Web UI (Dark Mode)](http://127.0.0.1:42069/?__theme=dark)
 
 
 
-### Command line options
+### 📃 Command line options
 | Flag | Valid Values | Default | Description |
 |---   |---     |---      | ---         |
 | `--mode` | `webui` | `webui` | Which UI mode to run  |
 | `--port` | Any valid port | `42069` | Which port to host webui |
 
 
 
-## Development (Hot reload)
+## 🚧 Development
 ```shell
 poetry install
 
 poetry shell
 gradio src/smarterbombing/__main__.py
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `smarterbombing-0.1.4/pyproject.toml` & `smarterbombing-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smarterbombing"
-version = "0.1.4"
+version = "0.1.5"
 description = "A tool which reads combat logs from Eve Online and displays statistics."
 repository = "https://github.com/agelito/eve-smarterbombing"
 authors = ["Axel Wettervik <axel.wettervik@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `smarterbombing-0.1.4/src/smarterbombing/__main__.py` & `smarterbombing-0.1.5/src/smarterbombing/__main__.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.4/src/smarterbombing/analysis.py` & `smarterbombing-0.1.5/src/smarterbombing/analysis.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.4/src/smarterbombing/app_live.py` & `smarterbombing-0.1.5/src/smarterbombing/app_live.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.4/src/smarterbombing/app_offline.py` & `smarterbombing-0.1.5/src/smarterbombing/app_offline.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.4/src/smarterbombing/configuration.py` & `smarterbombing-0.1.5/src/smarterbombing/configuration.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.4/src/smarterbombing/log_reader.py` & `smarterbombing-0.1.5/src/smarterbombing/log_reader.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.4/src/smarterbombing/logs.py` & `smarterbombing-0.1.5/src/smarterbombing/logs.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.4/src/smarterbombing/webui/ui.py` & `smarterbombing-0.1.5/src/smarterbombing/webui/ui.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.4/src/smarterbombing/webui/ui_configuration.py` & `smarterbombing-0.1.5/src/smarterbombing/webui/ui_configuration.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.4/src/smarterbombing/webui/ui_live.py` & `smarterbombing-0.1.5/src/smarterbombing/webui/ui_live.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.4/src/smarterbombing/webui/ui_offline_analysis.py` & `smarterbombing-0.1.5/src/smarterbombing/webui/ui_offline_analysis.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.4/PKG-INFO` & `smarterbombing-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smarterbombing
-Version: 0.1.4
+Version: 0.1.5
 Summary: A tool which reads combat logs from Eve Online and displays statistics.
 Home-page: https://github.com/agelito/eve-smarterbombing
 License: MIT
 Author: Axel Wettervik
 Author-email: axel.wettervik@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -20,34 +20,42 @@
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/agelito/eve-smarterbombing
 Description-Content-Type: text/markdown
 
 # Eve Smarterbombing
 An application analyzing Eve Online combat logs and presenting data in a Web interface.
 
-## Quick Start
+## ⚡ Quick Start
+
+### From PyPI
+```shell
+pip install smarterbombing
+python -m smarterbombing
+```
+
+### From Source
 ```shell
 poetry install
 poetry run python -m smarterbombing
 ```
 Open with your preferred browser:
 - Open [Web UI](http://localhost:42069)
 - Open [Web UI (Dark Mode)](http://127.0.0.1:42069/?__theme=dark)
 
 
 
-### Command line options
+### 📃 Command line options
 | Flag | Valid Values | Default | Description |
 |---   |---     |---      | ---         |
 | `--mode` | `webui` | `webui` | Which UI mode to run  |
 | `--port` | Any valid port | `42069` | Which port to host webui |
 
 
 
-## Development (Hot reload)
+## 🚧 Development
 ```shell
 poetry install
 
 poetry shell
 gradio src/smarterbombing/__main__.py
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

