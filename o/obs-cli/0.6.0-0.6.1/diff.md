# Comparing `tmp/obs-cli-0.6.0.tar.gz` & `tmp/obs-cli-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obs-cli-0.6.0.tar", last modified: Tue Jun  6 08:10:16 2023, max compression
+gzip compressed data, was "obs-cli-0.6.1.tar", last modified: Tue Jun  6 08:16:39 2023, max compression
```

## Comparing `obs-cli-0.6.0.tar` & `obs-cli-0.6.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:10:16.132012 obs-cli-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:10:16.128012 obs-cli-0.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-06 08:10:01.000000 obs-cli-0.6.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:10:16.128012 obs-cli-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-06 08:10:01.000000 obs-cli-0.6.0/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-06 08:10:01.000000 obs-cli-0.6.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-06 08:10:01.000000 obs-cli-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-06 08:10:01.000000 obs-cli-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44502 2023-06-06 08:10:16.128012 obs-cli-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-06-06 08:10:01.000000 obs-cli-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:10:16.128012 obs-cli-0.6.0/obs_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44502 2023-06-06 08:10:16.000000 obs-cli-0.6.0/obs_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-06 08:10:16.000000 obs-cli-0.6.0/obs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 08:10:16.000000 obs-cli-0.6.0/obs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-06 08:10:16.000000 obs-cli-0.6.0/obs_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 08:10:16.000000 obs-cli-0.6.0/obs_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 08:10:16.000000 obs-cli-0.6.0/obs_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15200 2023-06-06 08:10:01.000000 obs-cli-0.6.0/obs_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-06 08:10:01.000000 obs-cli-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 08:10:16.132012 obs-cli-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:16:39.679880 obs-cli-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:16:39.679880 obs-cli-0.6.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-06 08:16:27.000000 obs-cli-0.6.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:16:39.679880 obs-cli-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-06 08:16:27.000000 obs-cli-0.6.1/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-06 08:16:27.000000 obs-cli-0.6.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-06 08:16:27.000000 obs-cli-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-06 08:16:27.000000 obs-cli-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44491 2023-06-06 08:16:39.679880 obs-cli-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-06 08:16:27.000000 obs-cli-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:16:39.679880 obs-cli-0.6.1/obs_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44491 2023-06-06 08:16:39.000000 obs-cli-0.6.1/obs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-06 08:16:39.000000 obs-cli-0.6.1/obs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 08:16:39.000000 obs-cli-0.6.1/obs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-06 08:16:39.000000 obs-cli-0.6.1/obs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 08:16:39.000000 obs-cli-0.6.1/obs_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 08:16:39.000000 obs-cli-0.6.1/obs_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15200 2023-06-06 08:16:27.000000 obs-cli-0.6.1/obs_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-06 08:16:27.000000 obs-cli-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 08:16:39.679880 obs-cli-0.6.1/setup.cfg
```

### Comparing `obs-cli-0.6.0/.github/workflows/release.yaml` & `obs-cli-0.6.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `obs-cli-0.6.0/LICENSE` & `obs-cli-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `obs-cli-0.6.0/PKG-INFO` & `obs-cli-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obs-cli
-Version: 0.6.0
+Version: 0.6.1
 Summary: OBS CLI
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -682,24 +682,37 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🎬🎥 OBS CLI
 
-`obs-cli` is a command-line interface for OBS Studio. It allows you to control OBS Studio from the command line, making it easier to automate scene switching, source toggling, and more.
+`obs-cli` is a command-line interface for OBS Studio.
 
-This implementation of `obs-cli` is written in Python 3 and powered by [rich](https://github.com/Textualize/rich) and [obsws-python](https://pypi.org/project/obsws-python/). It supports the new OBS WebSocket API only.
+It allows you to control OBS Studio from the command line, making it easier to
+automate scene switching, source toggling, and more.
+
+This implementation of `obs-cli` is:
+
+- written in Python 3
+- powered by [rich](https://github.com/Textualize/rich) and
+[obsws-python](https://pypi.org/project/obsws-python/).
+
+⚠️ Only the new OBS WebSocket API (v5) is supported!
 
 ## 💻 Installation
 
-You can install `obs-cli` using pip:
+You can install `obs-cli` using pip(x):
 
 ```shell
+# pipx
 pipx install obs-cli
+
+# pip
+pip install --user obs-cli
 ```
 
 ## 🛠️ Usage
 
 Here's the general usage of `obs-cli`:
 
 ```shell
@@ -737,21 +750,21 @@
 ```shell
 obs-cli item --help
 ```
 
 For example, to hide an item named "Item1" in a scene named "Scene2":
 
 ```shell
-obs-cli item hide --scene "Scene2" --item "Item1"
+obs-cli item hide --scene "Scene2" "Item1"
 ```
 
 And to show it:
 
 ```shell
-obs-cli item show --scene "Scene2" --item "Item1"
+obs-cli item show --scene "Scene2" "Item1"
 ```
 
 To list all items in a scene:
 
 ```shell
 obs-cli item list --scene "Scene2"
 ```
@@ -763,15 +776,15 @@
 ```shell
 obs-cli input --help
 ```
 
 For example, to get the settings of an input named "Mic/Aux":
 
 ```shell
-obs-cli input get --input "Mic/Aux"
+obs-cli input get "Mic/Aux"
 ```
 
 To list all inputs:
 
 ```shell
 obs-cli input list
 ```
@@ -783,41 +796,41 @@
 ```shell
 obs-cli filter --help
 ```
 
 For example, to enable a filter named "Filter1" on an input named "Mic/Aux":
 
 ```shell
-obs-cli filter enable --input "Mic/Aux" --filter "Filter1"
+obs-cli filter enable "Mic/Aux" "Filter1"
 ```
 
 And to disable it:
 
 ```shell
-obs-cli filter disable --input "Mic/Aux" --filter "Filter1"
+obs-cli filter disable "Mic/Aux" "Filter1"
 ```
 
 To list all filters on an input:
 
 ```shell
-obs-cli filter list --input "Mic/Aux"
+obs-cli filter list "Mic/Aux"
 ```
 
 ### ⌨️ Hotkey Management
 
 You can manage hotkeys using the `hotkey` command:
 
 ```shell
 obs-cli hotkey --help
 ```
 
 For example, to trigger a hotkey named "Hotkey1":
 
 ```shell
-obs-cli hotkey trigger --hotkey "Hotkey1"
+obs-cli hotkey trigger "Hotkey1"
 ```
 
 To list all hotkeys:
 
 ```shell
 obs-cli hotkey list
 ```
@@ -916,9 +929,11 @@
 
 ```shell
 obs-cli record status
 ```
 
 ## 📄 License
 
-This project is licensed under the GPL-3.0 License. See [LICENSE](LICENSE) for more information.
+This project is licensed under the GPL-3.0 License.
+
+See [LICENSE](LICENSE) for more information.
```

### Comparing `obs-cli-0.6.0/README.md` & `obs-cli-0.6.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 # 🎬🎥 OBS CLI
 
-`obs-cli` is a command-line interface for OBS Studio. It allows you to control OBS Studio from the command line, making it easier to automate scene switching, source toggling, and more.
+`obs-cli` is a command-line interface for OBS Studio.
 
-This implementation of `obs-cli` is written in Python 3 and powered by [rich](https://github.com/Textualize/rich) and [obsws-python](https://pypi.org/project/obsws-python/). It supports the new OBS WebSocket API only.
+It allows you to control OBS Studio from the command line, making it easier to
+automate scene switching, source toggling, and more.
+
+This implementation of `obs-cli` is:
+
+- written in Python 3
+- powered by [rich](https://github.com/Textualize/rich) and
+[obsws-python](https://pypi.org/project/obsws-python/).
+
+⚠️ Only the new OBS WebSocket API (v5) is supported!
 
 ## 💻 Installation
 
-You can install `obs-cli` using pip:
+You can install `obs-cli` using pip(x):
 
 ```shell
+# pipx
 pipx install obs-cli
+
+# pip
+pip install --user obs-cli
 ```
 
 ## 🛠️ Usage
 
 Here's the general usage of `obs-cli`:
 
 ```shell
@@ -51,21 +64,21 @@
 ```shell
 obs-cli item --help
 ```
 
 For example, to hide an item named "Item1" in a scene named "Scene2":
 
 ```shell
-obs-cli item hide --scene "Scene2" --item "Item1"
+obs-cli item hide --scene "Scene2" "Item1"
 ```
 
 And to show it:
 
 ```shell
-obs-cli item show --scene "Scene2" --item "Item1"
+obs-cli item show --scene "Scene2" "Item1"
 ```
 
 To list all items in a scene:
 
 ```shell
 obs-cli item list --scene "Scene2"
 ```
@@ -77,15 +90,15 @@
 ```shell
 obs-cli input --help
 ```
 
 For example, to get the settings of an input named "Mic/Aux":
 
 ```shell
-obs-cli input get --input "Mic/Aux"
+obs-cli input get "Mic/Aux"
 ```
 
 To list all inputs:
 
 ```shell
 obs-cli input list
 ```
@@ -97,41 +110,41 @@
 ```shell
 obs-cli filter --help
 ```
 
 For example, to enable a filter named "Filter1" on an input named "Mic/Aux":
 
 ```shell
-obs-cli filter enable --input "Mic/Aux" --filter "Filter1"
+obs-cli filter enable "Mic/Aux" "Filter1"
 ```
 
 And to disable it:
 
 ```shell
-obs-cli filter disable --input "Mic/Aux" --filter "Filter1"
+obs-cli filter disable "Mic/Aux" "Filter1"
 ```
 
 To list all filters on an input:
 
 ```shell
-obs-cli filter list --input "Mic/Aux"
+obs-cli filter list "Mic/Aux"
 ```
 
 ### ⌨️ Hotkey Management
 
 You can manage hotkeys using the `hotkey` command:
 
 ```shell
 obs-cli hotkey --help
 ```
 
 For example, to trigger a hotkey named "Hotkey1":
 
 ```shell
-obs-cli hotkey trigger --hotkey "Hotkey1"
+obs-cli hotkey trigger "Hotkey1"
 ```
 
 To list all hotkeys:
 
 ```shell
 obs-cli hotkey list
 ```
@@ -230,9 +243,11 @@
 
 ```shell
 obs-cli record status
 ```
 
 ## 📄 License
 
-This project is licensed under the GPL-3.0 License. See [LICENSE](LICENSE) for more information.
+This project is licensed under the GPL-3.0 License.
+
+See [LICENSE](LICENSE) for more information.
```

### Comparing `obs-cli-0.6.0/obs_cli.egg-info/PKG-INFO` & `obs-cli-0.6.1/obs_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obs-cli
-Version: 0.6.0
+Version: 0.6.1
 Summary: OBS CLI
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -682,24 +682,37 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🎬🎥 OBS CLI
 
-`obs-cli` is a command-line interface for OBS Studio. It allows you to control OBS Studio from the command line, making it easier to automate scene switching, source toggling, and more.
+`obs-cli` is a command-line interface for OBS Studio.
 
-This implementation of `obs-cli` is written in Python 3 and powered by [rich](https://github.com/Textualize/rich) and [obsws-python](https://pypi.org/project/obsws-python/). It supports the new OBS WebSocket API only.
+It allows you to control OBS Studio from the command line, making it easier to
+automate scene switching, source toggling, and more.
+
+This implementation of `obs-cli` is:
+
+- written in Python 3
+- powered by [rich](https://github.com/Textualize/rich) and
+[obsws-python](https://pypi.org/project/obsws-python/).
+
+⚠️ Only the new OBS WebSocket API (v5) is supported!
 
 ## 💻 Installation
 
-You can install `obs-cli` using pip:
+You can install `obs-cli` using pip(x):
 
 ```shell
+# pipx
 pipx install obs-cli
+
+# pip
+pip install --user obs-cli
 ```
 
 ## 🛠️ Usage
 
 Here's the general usage of `obs-cli`:
 
 ```shell
@@ -737,21 +750,21 @@
 ```shell
 obs-cli item --help
 ```
 
 For example, to hide an item named "Item1" in a scene named "Scene2":
 
 ```shell
-obs-cli item hide --scene "Scene2" --item "Item1"
+obs-cli item hide --scene "Scene2" "Item1"
 ```
 
 And to show it:
 
 ```shell
-obs-cli item show --scene "Scene2" --item "Item1"
+obs-cli item show --scene "Scene2" "Item1"
 ```
 
 To list all items in a scene:
 
 ```shell
 obs-cli item list --scene "Scene2"
 ```
@@ -763,15 +776,15 @@
 ```shell
 obs-cli input --help
 ```
 
 For example, to get the settings of an input named "Mic/Aux":
 
 ```shell
-obs-cli input get --input "Mic/Aux"
+obs-cli input get "Mic/Aux"
 ```
 
 To list all inputs:
 
 ```shell
 obs-cli input list
 ```
@@ -783,41 +796,41 @@
 ```shell
 obs-cli filter --help
 ```
 
 For example, to enable a filter named "Filter1" on an input named "Mic/Aux":
 
 ```shell
-obs-cli filter enable --input "Mic/Aux" --filter "Filter1"
+obs-cli filter enable "Mic/Aux" "Filter1"
 ```
 
 And to disable it:
 
 ```shell
-obs-cli filter disable --input "Mic/Aux" --filter "Filter1"
+obs-cli filter disable "Mic/Aux" "Filter1"
 ```
 
 To list all filters on an input:
 
 ```shell
-obs-cli filter list --input "Mic/Aux"
+obs-cli filter list "Mic/Aux"
 ```
 
 ### ⌨️ Hotkey Management
 
 You can manage hotkeys using the `hotkey` command:
 
 ```shell
 obs-cli hotkey --help
 ```
 
 For example, to trigger a hotkey named "Hotkey1":
 
 ```shell
-obs-cli hotkey trigger --hotkey "Hotkey1"
+obs-cli hotkey trigger "Hotkey1"
 ```
 
 To list all hotkeys:
 
 ```shell
 obs-cli hotkey list
 ```
@@ -916,9 +929,11 @@
 
 ```shell
 obs-cli record status
 ```
 
 ## 📄 License
 
-This project is licensed under the GPL-3.0 License. See [LICENSE](LICENSE) for more information.
+This project is licensed under the GPL-3.0 License.
+
+See [LICENSE](LICENSE) for more information.
```

### Comparing `obs-cli-0.6.0/obs_cli.py` & `obs-cli-0.6.1/obs_cli.py`

 * *Files identical despite different names*

### Comparing `obs-cli-0.6.0/pyproject.toml` & `obs-cli-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,14 @@
 classifiers = [
   "Programming Language :: Python :: 3",
 ]
 dependencies = [
   "obsws-python",
   "rich"
 ]
-version = "0.6.0"
+version = "0.6.1"
 
 [tool.black]
 line-length = 79
 
 [project.scripts]
 obs-cli = "obs_cli:main"
```

