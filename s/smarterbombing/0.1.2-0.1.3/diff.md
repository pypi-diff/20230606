# Comparing `tmp/smarterbombing-0.1.2.tar.gz` & `tmp/smarterbombing-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smarterbombing-0.1.2.tar", max compression
+gzip compressed data, was "smarterbombing-0.1.3.tar", max compression
```

## Comparing `smarterbombing-0.1.2.tar` & `smarterbombing-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1071 2023-06-06 15:17:06.907608 smarterbombing-0.1.2/LICENSE
--rw-r--r--   0        0        0      684 2023-06-06 15:17:06.907608 smarterbombing-0.1.2/README.md
--rw-r--r--   0        0        0      860 2023-06-06 15:17:37.671987 smarterbombing-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      116 2023-06-06 15:17:06.907608 smarterbombing-0.1.2/src/smarterbombing/__init__.py
--rw-r--r--   0        0        0      775 2023-06-06 15:17:06.907608 smarterbombing-0.1.2/src/smarterbombing/__main__.py
--rw-r--r--   0        0        0    10681 2023-06-06 15:17:06.907608 smarterbombing-0.1.2/src/smarterbombing/analysis.py
--rw-r--r--   0        0        0     5497 2023-06-06 15:17:06.907608 smarterbombing-0.1.2/src/smarterbombing/app_live.py
--rw-r--r--   0        0        0     2979 2023-06-06 15:17:06.907608 smarterbombing-0.1.2/src/smarterbombing/app_offline.py
--rw-r--r--   0        0        0      817 2023-06-06 15:17:06.907608 smarterbombing-0.1.2/src/smarterbombing/configuration.py
--rw-r--r--   0        0        0     3645 2023-06-06 15:17:06.907608 smarterbombing-0.1.2/src/smarterbombing/log_reader.py
--rw-r--r--   0        0        0     3533 2023-06-06 15:17:06.907608 smarterbombing-0.1.2/src/smarterbombing/logs.py
--rw-r--r--   0        0        0        0 2023-06-06 15:17:06.907608 smarterbombing-0.1.2/src/smarterbombing/webui/__init__.py
--rw-r--r--   0        0        0     1104 2023-06-06 15:17:06.907608 smarterbombing-0.1.2/src/smarterbombing/webui/ui.py
--rw-r--r--   0        0        0     1837 2023-06-06 15:17:06.907608 smarterbombing-0.1.2/src/smarterbombing/webui/ui_configuration.py
--rw-r--r--   0        0        0     5546 2023-06-06 15:17:06.907608 smarterbombing-0.1.2/src/smarterbombing/webui/ui_live.py
--rw-r--r--   0        0        0     4199 2023-06-06 15:17:06.907608 smarterbombing-0.1.2/src/smarterbombing/webui/ui_offline_analysis.py
--rw-r--r--   0        0        0     1600 1970-01-01 00:00:00.000000 smarterbombing-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-06 15:42:21.966250 smarterbombing-0.1.3/LICENSE
+-rw-r--r--   0        0        0      684 2023-06-06 15:42:21.966250 smarterbombing-0.1.3/README.md
+-rw-r--r--   0        0        0      860 2023-06-06 15:42:53.154736 smarterbombing-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      116 2023-06-06 15:42:21.966250 smarterbombing-0.1.3/src/smarterbombing/__init__.py
+-rw-r--r--   0        0        0      769 2023-06-06 15:42:21.966250 smarterbombing-0.1.3/src/smarterbombing/__main__.py
+-rw-r--r--   0        0        0    10681 2023-06-06 15:42:21.966250 smarterbombing-0.1.3/src/smarterbombing/analysis.py
+-rw-r--r--   0        0        0     5497 2023-06-06 15:42:21.966250 smarterbombing-0.1.3/src/smarterbombing/app_live.py
+-rw-r--r--   0        0        0     2979 2023-06-06 15:42:21.966250 smarterbombing-0.1.3/src/smarterbombing/app_offline.py
+-rw-r--r--   0        0        0      817 2023-06-06 15:42:21.966250 smarterbombing-0.1.3/src/smarterbombing/configuration.py
+-rw-r--r--   0        0        0     3698 2023-06-06 15:42:21.966250 smarterbombing-0.1.3/src/smarterbombing/log_reader.py
+-rw-r--r--   0        0        0     3533 2023-06-06 15:42:21.966250 smarterbombing-0.1.3/src/smarterbombing/logs.py
+-rw-r--r--   0        0        0        0 2023-06-06 15:42:21.966250 smarterbombing-0.1.3/src/smarterbombing/webui/__init__.py
+-rw-r--r--   0        0        0     1104 2023-06-06 15:42:21.966250 smarterbombing-0.1.3/src/smarterbombing/webui/ui.py
+-rw-r--r--   0        0        0     1837 2023-06-06 15:42:21.966250 smarterbombing-0.1.3/src/smarterbombing/webui/ui_configuration.py
+-rw-r--r--   0        0        0     5546 2023-06-06 15:42:21.966250 smarterbombing-0.1.3/src/smarterbombing/webui/ui_live.py
+-rw-r--r--   0        0        0     4199 2023-06-06 15:42:21.966250 smarterbombing-0.1.3/src/smarterbombing/webui/ui_offline_analysis.py
+-rw-r--r--   0        0        0     1600 1970-01-01 00:00:00.000000 smarterbombing-0.1.3/PKG-INFO
```

### Comparing `smarterbombing-0.1.2/LICENSE` & `smarterbombing-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.2/README.md` & `smarterbombing-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.2/pyproject.toml` & `smarterbombing-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smarterbombing"
-version = "0.1.2"
+version = "0.1.3"
 description = "A tool which reads combat logs from Eve Online and displays statistics."
 repository = "https://github.com/agelito/eve-smarterbombing"
 authors = ["Axel Wettervik <axel.wettervik@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `smarterbombing-0.1.2/src/smarterbombing/__main__.py` & `smarterbombing-0.1.3/src/smarterbombing/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Main application entrypoint"""
 from argparse import ArgumentParser
 import sys
 
-from smarterbombing.webui.ui import run_webui
+import smarterbombing.webui.ui as ui
 
 parser = ArgumentParser(
     prog='smarterbombing',
     description='Parse Eve Online combat logs and display statistics.',
     epilog='Show your support by sending ISK in-game to Ageliten.')
 
 MODE_HELP = 'How to run smarterbombing -- webui (default)'
@@ -24,11 +24,11 @@
     required=False,
     help=PORT_HELP
 )
 
 args = parser.parse_args()
 
 if args.mode == 'webui':
-    run_webui(args.port)
+    ui.run_webui(args.port)
 else:
     print(f'unrecognized mode: {args.mode}')
     sys.exit(1)
```

### Comparing `smarterbombing-0.1.2/src/smarterbombing/analysis.py` & `smarterbombing-0.1.3/src/smarterbombing/analysis.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.2/src/smarterbombing/app_live.py` & `smarterbombing-0.1.3/src/smarterbombing/app_live.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.2/src/smarterbombing/app_offline.py` & `smarterbombing-0.1.3/src/smarterbombing/app_offline.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.2/src/smarterbombing/configuration.py` & `smarterbombing-0.1.3/src/smarterbombing/configuration.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.2/src/smarterbombing/log_reader.py` & `smarterbombing-0.1.3/src/smarterbombing/log_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,17 @@
     return parsed_lines
 
 def _flatten(in_list):
     return [item for ll in in_list for item in ll]
 
 def read_all_combat_log_entries(character_files: list[CharacterLogFile]):
     """Read all combat log entries from character log files"""
+    if len(character_files) == 0:
+        return []
+
     character_log_entries = map(_read_and_parse_combat_log_lines, character_files)
 
     return _flatten(character_log_entries)
 
 def open_log_files(
         character_logs,
         filter_characters,
```

### Comparing `smarterbombing-0.1.2/src/smarterbombing/logs.py` & `smarterbombing-0.1.3/src/smarterbombing/logs.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.2/src/smarterbombing/webui/ui.py` & `smarterbombing-0.1.3/src/smarterbombing/webui/ui.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.2/src/smarterbombing/webui/ui_configuration.py` & `smarterbombing-0.1.3/src/smarterbombing/webui/ui_configuration.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.2/src/smarterbombing/webui/ui_live.py` & `smarterbombing-0.1.3/src/smarterbombing/webui/ui_live.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.2/src/smarterbombing/webui/ui_offline_analysis.py` & `smarterbombing-0.1.3/src/smarterbombing/webui/ui_offline_analysis.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.2/PKG-INFO` & `smarterbombing-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smarterbombing
-Version: 0.1.2
+Version: 0.1.3
 Summary: A tool which reads combat logs from Eve Online and displays statistics.
 Home-page: https://github.com/agelito/eve-smarterbombing
 License: MIT
 Author: Axel Wettervik
 Author-email: axel.wettervik@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

