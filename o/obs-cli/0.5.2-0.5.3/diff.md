# Comparing `tmp/obs-cli-0.5.2.tar.gz` & `tmp/obs-cli-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obs-cli-0.5.2.tar", last modified: Mon Jun  5 16:57:16 2023, max compression
+gzip compressed data, was "obs-cli-0.5.3.tar", last modified: Tue Jun  6 05:55:18 2023, max compression
```

## Comparing `obs-cli-0.5.2.tar` & `obs-cli-0.5.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:57:16.441636 obs-cli-0.5.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:57:16.441636 obs-cli-0.5.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-05 16:57:01.000000 obs-cli-0.5.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:57:16.441636 obs-cli-0.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-05 16:57:01.000000 obs-cli-0.5.2/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-05 16:57:01.000000 obs-cli-0.5.2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-05 16:57:01.000000 obs-cli-0.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 16:57:01.000000 obs-cli-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41622 2023-06-05 16:57:16.441636 obs-cli-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-05 16:57:01.000000 obs-cli-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:57:16.441636 obs-cli-0.5.2/obs_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41622 2023-06-05 16:57:16.000000 obs-cli-0.5.2/obs_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-05 16:57:16.000000 obs-cli-0.5.2/obs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:57:16.000000 obs-cli-0.5.2/obs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-05 16:57:16.000000 obs-cli-0.5.2/obs_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 16:57:16.000000 obs-cli-0.5.2/obs_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 16:57:16.000000 obs-cli-0.5.2/obs_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-06-05 16:57:01.000000 obs-cli-0.5.2/obs_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-05 16:57:01.000000 obs-cli-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 16:57:16.441636 obs-cli-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:55:18.301294 obs-cli-0.5.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:55:18.301294 obs-cli-0.5.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-06 05:55:08.000000 obs-cli-0.5.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:55:18.301294 obs-cli-0.5.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-06 05:55:08.000000 obs-cli-0.5.3/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-06 05:55:08.000000 obs-cli-0.5.3/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-06 05:55:08.000000 obs-cli-0.5.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-06 05:55:08.000000 obs-cli-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    43315 2023-06-06 05:55:18.301294 obs-cli-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-06 05:55:08.000000 obs-cli-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:55:18.301294 obs-cli-0.5.3/obs_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43315 2023-06-06 05:55:18.000000 obs-cli-0.5.3/obs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-06 05:55:18.000000 obs-cli-0.5.3/obs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 05:55:18.000000 obs-cli-0.5.3/obs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-06 05:55:18.000000 obs-cli-0.5.3/obs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 05:55:18.000000 obs-cli-0.5.3/obs_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 05:55:18.000000 obs-cli-0.5.3/obs_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-06-06 05:55:08.000000 obs-cli-0.5.3/obs_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-06 05:55:08.000000 obs-cli-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 05:55:18.301294 obs-cli-0.5.3/setup.cfg
```

### Comparing `obs-cli-0.5.2/.github/workflows/release.yaml` & `obs-cli-0.5.3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `obs-cli-0.5.2/LICENSE` & `obs-cli-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `obs-cli-0.5.2/PKG-INFO` & `obs-cli-0.5.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obs-cli
-Version: 0.5.2
+Version: 0.5.3
 Summary: OBS CLI
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -680,43 +680,149 @@
         
 Keywords: obs,obs-studio
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# obs-cli
+# 🎬🎥 OBS CLI
 
-Yes, this is yet another obs-cli implementation.
+`obs-cli` is a command-line interface for OBS Studio. It allows you to control OBS Studio from the command line, making it easier to automate scene switching, source toggling, and more.
 
-This one:
+This implementation of `obs-cli` is written in Python 3 and powered by [rich](https://github.com/Textualize/rich) and [obsws-python](https://pypi.org/project/obsws-python/). It supports the new OBS WebSocket API only.
 
-- is written in Python 3, powered by [rich](https://github.com/Textualize/rich) 
-and [obswd-python](https://pypi.org/project/obsws-python/)
-- 😮 Supports the *new websocket* API only
+## 💻 Installation
 
-## Installation
+You can install `obs-cli` using pip:
 
 ```shell
 pipx install obs-cli
 ```
 
-## Usage
+## 🛠️ Usage
 
-```
+Here's the general usage of `obs-cli`:
+
+```shell
 obs-cli --help
-usage: obs_cli.py [-h] [-D] [-q] [-H HOST] [-P PORT] [-p PASSWORD] [-j]
-                  {scene,item,input,filter,hotkey} ...
+```
+
+This will show you the available commands and options.
+
+## 🌟 Features
+
+### 🎞️ Scene Management
+
+You can manage scenes using the `scene` command:
+
+```shell
+obs-cli scene --help
+```
+
+For example, to switch to a scene named "Scene2":
+
+```shell
+obs-cli scene switch --scene "Scene2"
+```
+
+To list all scenes:
+
+```shell
+obs-cli scene list
+```
+
+### 📦 Item Management
 
-positional arguments:
-  {scene,item,input,filter,hotkey}
+You can manage scene items using the `item` command:
 
-options:
-  -h, --help            show this help message and exit
-  -D, --debug
-  -q, --quiet
-  -H HOST, --host HOST  host name
-  -P PORT, --port PORT  port number
-  -p PASSWORD, --password PASSWORD
-                        password ($OBS_API_PASSWORD)
-  -j, --json
+```shell
+obs-cli item --help
+```
+
+For example, to hide an item named "Item1" in a scene named "Scene2":
+
+```shell
+obs-cli item hide --scene "Scene2" --item "Item1"
+```
+
+And to show it:
+
+```shell
+obs-cli item show --scene "Scene2" --item "Item1"
+```
+
+To list all items in a scene:
+
+```shell
+obs-cli item list --scene "Scene2"
+```
+
+### 🎤 Input Management
+
+You can manage inputs using the `input` command:
+
+```shell
+obs-cli input --help
 ```
+
+For example, to get the settings of an input named "Mic/Aux":
+
+```shell
+obs-cli input get --input "Mic/Aux"
+```
+
+To list all inputs:
+
+```shell
+obs-cli input list
+```
+
+### 🎨 Filter Management
+
+You can manage filters using the `filter` command:
+
+```shell
+obs-cli filter --help
+```
+
+For example, to enable a filter named "Filter1" on an input named "Mic/Aux":
+
+```shell
+obs-cli filter enable --input "Mic/Aux" --filter "Filter1"
+```
+
+And to disable it:
+
+```shell
+obs-cli filter disable --input "Mic/Aux" --filter "Filter1"
+```
+
+To list all filters on an input:
+
+```shell
+obs-cli filter list --input "Mic/Aux"
+```
+
+### ⌨️ Hotkey Management
+
+You can manage hotkeys using the `hotkey` command:
+
+```shell
+obs-cli hotkey --help
+```
+
+For example, to trigger a hotkey named "Hotkey1":
+
+```shell
+obs-cli hotkey trigger --hotkey "Hotkey1"
+```
+
+To list all hotkeys:
+
+```shell
+obs-cli hotkey list
+```
+
+## 📄 License
+
+This project is licensed under the GPL-3.0 License. See [LICENSE](LICENSE) for more information.
+
```

### Comparing `obs-cli-0.5.2/obs_cli.egg-info/PKG-INFO` & `obs-cli-0.5.3/obs_cli.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obs-cli
-Version: 0.5.2
+Version: 0.5.3
 Summary: OBS CLI
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -680,43 +680,149 @@
         
 Keywords: obs,obs-studio
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# obs-cli
+# 🎬🎥 OBS CLI
 
-Yes, this is yet another obs-cli implementation.
+`obs-cli` is a command-line interface for OBS Studio. It allows you to control OBS Studio from the command line, making it easier to automate scene switching, source toggling, and more.
 
-This one:
+This implementation of `obs-cli` is written in Python 3 and powered by [rich](https://github.com/Textualize/rich) and [obsws-python](https://pypi.org/project/obsws-python/). It supports the new OBS WebSocket API only.
 
-- is written in Python 3, powered by [rich](https://github.com/Textualize/rich) 
-and [obswd-python](https://pypi.org/project/obsws-python/)
-- 😮 Supports the *new websocket* API only
+## 💻 Installation
 
-## Installation
+You can install `obs-cli` using pip:
 
 ```shell
 pipx install obs-cli
 ```
 
-## Usage
+## 🛠️ Usage
 
-```
+Here's the general usage of `obs-cli`:
+
+```shell
 obs-cli --help
-usage: obs_cli.py [-h] [-D] [-q] [-H HOST] [-P PORT] [-p PASSWORD] [-j]
-                  {scene,item,input,filter,hotkey} ...
+```
+
+This will show you the available commands and options.
+
+## 🌟 Features
+
+### 🎞️ Scene Management
+
+You can manage scenes using the `scene` command:
+
+```shell
+obs-cli scene --help
+```
+
+For example, to switch to a scene named "Scene2":
+
+```shell
+obs-cli scene switch --scene "Scene2"
+```
+
+To list all scenes:
+
+```shell
+obs-cli scene list
+```
+
+### 📦 Item Management
 
-positional arguments:
-  {scene,item,input,filter,hotkey}
+You can manage scene items using the `item` command:
 
-options:
-  -h, --help            show this help message and exit
-  -D, --debug
-  -q, --quiet
-  -H HOST, --host HOST  host name
-  -P PORT, --port PORT  port number
-  -p PASSWORD, --password PASSWORD
-                        password ($OBS_API_PASSWORD)
-  -j, --json
+```shell
+obs-cli item --help
+```
+
+For example, to hide an item named "Item1" in a scene named "Scene2":
+
+```shell
+obs-cli item hide --scene "Scene2" --item "Item1"
+```
+
+And to show it:
+
+```shell
+obs-cli item show --scene "Scene2" --item "Item1"
+```
+
+To list all items in a scene:
+
+```shell
+obs-cli item list --scene "Scene2"
+```
+
+### 🎤 Input Management
+
+You can manage inputs using the `input` command:
+
+```shell
+obs-cli input --help
 ```
+
+For example, to get the settings of an input named "Mic/Aux":
+
+```shell
+obs-cli input get --input "Mic/Aux"
+```
+
+To list all inputs:
+
+```shell
+obs-cli input list
+```
+
+### 🎨 Filter Management
+
+You can manage filters using the `filter` command:
+
+```shell
+obs-cli filter --help
+```
+
+For example, to enable a filter named "Filter1" on an input named "Mic/Aux":
+
+```shell
+obs-cli filter enable --input "Mic/Aux" --filter "Filter1"
+```
+
+And to disable it:
+
+```shell
+obs-cli filter disable --input "Mic/Aux" --filter "Filter1"
+```
+
+To list all filters on an input:
+
+```shell
+obs-cli filter list --input "Mic/Aux"
+```
+
+### ⌨️ Hotkey Management
+
+You can manage hotkeys using the `hotkey` command:
+
+```shell
+obs-cli hotkey --help
+```
+
+For example, to trigger a hotkey named "Hotkey1":
+
+```shell
+obs-cli hotkey trigger --hotkey "Hotkey1"
+```
+
+To list all hotkeys:
+
+```shell
+obs-cli hotkey list
+```
+
+## 📄 License
+
+This project is licensed under the GPL-3.0 License. See [LICENSE](LICENSE) for more information.
+
```

### Comparing `obs-cli-0.5.2/obs_cli.py` & `obs-cli-0.5.3/obs_cli.py`

 * *Files identical despite different names*

### Comparing `obs-cli-0.5.2/pyproject.toml` & `obs-cli-0.5.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -15,14 +15,14 @@
 classifiers = [
   "Programming Language :: Python :: 3",
 ]
 dependencies = [
   "obsws-python",
   "rich"
 ]
-version = "0.5.2"
+version = "0.5.3"
 
 [tool.black]
 line-length = 79
 
 [project.scripts]
 obs-cli = "obs_cli:main"
```

