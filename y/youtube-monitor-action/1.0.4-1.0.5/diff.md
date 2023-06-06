# Comparing `tmp/youtube_monitor_action-1.0.4.tar.gz` & `tmp/youtube_monitor_action-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtube_monitor_action-1.0.4.tar", max compression
+gzip compressed data, was "youtube_monitor_action-1.0.5.tar", max compression
```

## Comparing `youtube_monitor_action-1.0.4.tar` & `youtube_monitor_action-1.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      194 2023-06-06 02:35:15.849536 youtube_monitor_action-1.0.4/CHANGELOG.md
--rw-r--r--   0        0        0     1086 2023-06-06 02:35:15.849536 youtube_monitor_action-1.0.4/LICENSE
--rw-r--r--   0        0        0      871 2023-06-06 02:46:38.224422 youtube_monitor_action-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1107 2023-06-06 02:35:15.849536 youtube_monitor_action-1.0.4/README.md
--rw-r--r--   0        0        0      140 2023-06-06 02:35:15.853536 youtube_monitor_action-1.0.4/youtube_monitor_action/__init__.py
--rw-r--r--   0        0        0     9665 2023-06-06 02:44:05.628832 youtube_monitor_action-1.0.4/youtube_monitor_action/__main__.py
--rw-r--r--   0        0        0     2355 2023-06-06 02:35:15.853536 youtube_monitor_action-1.0.4/youtube_monitor_action/_logging_utils.py
--rw-r--r--   0        0        0     2047 2023-06-06 02:46:42.890422 youtube_monitor_action-1.0.4/setup.py
--rw-r--r--   0        0        0     1913 2023-06-06 02:46:42.890422 youtube_monitor_action-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      194 2023-06-06 02:35:15.849536 youtube_monitor_action-1.0.5/CHANGELOG.md
+-rw-r--r--   0        0        0     1086 2023-06-06 02:35:15.849536 youtube_monitor_action-1.0.5/LICENSE
+-rw-r--r--   0        0        0      871 2023-06-06 02:50:55.649421 youtube_monitor_action-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1215 2023-06-06 02:50:20.877421 youtube_monitor_action-1.0.5/README.md
+-rw-r--r--   0        0        0      140 2023-06-06 02:35:15.853536 youtube_monitor_action-1.0.5/youtube_monitor_action/__init__.py
+-rw-r--r--   0        0        0     9665 2023-06-06 02:48:01.852420 youtube_monitor_action-1.0.5/youtube_monitor_action/__main__.py
+-rw-r--r--   0        0        0     2355 2023-06-06 02:35:15.853536 youtube_monitor_action-1.0.5/youtube_monitor_action/_logging_utils.py
+-rw-r--r--   0        0        0     2155 2023-06-06 02:51:10.131421 youtube_monitor_action-1.0.5/setup.py
+-rw-r--r--   0        0        0     2019 2023-06-06 02:51:10.131421 youtube_monitor_action-1.0.5/PKG-INFO
```

### Comparing `youtube_monitor_action-1.0.4/LICENSE` & `youtube_monitor_action-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `youtube_monitor_action-1.0.4/pyproject.toml` & `youtube_monitor_action-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "youtube_monitor_action"
-version = "1.0.4"
+version = "1.0.5"
 description = "Monitor for new video on YouTube Channel"
 authors = ["mshafer1"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mshafer1/youtube_monitor_action"
 include = [
     "LICENSE",
```

### Comparing `youtube_monitor_action-1.0.4/README.md` & `youtube_monitor_action-1.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # youtube_monitor_action
 A utility to perform an action after videos are live on YouTube for a given channel.
 
 This module provides the script `youtube-monitor-action`
 ```
 usage: youtube-monitor-action [-h] [-n N] [--channel CHANNEL] [--store-config]
-                              [--hibernate] [--open-in-browser] [--verbose]
-                              [--quiet] [--version] [--log-file LOG_FILE]
+                              [--hibernate] [--open-in-browser] [--shutdown]
+                              [--verbose] [--quiet] [--version]
+                              [--log-file LOG_FILE]
 
 optional arguments:
   -h, --help           show this help message and exit
   -n N                 The number of new videos to watch for
   --channel CHANNEL    (Optional) The channel id to monitor (default: load
                        from config.yaml)
   --store-config       Store channel and other settings in config and exit
 
 Actions:
   --hibernate          Hibernate computer once condition is met
   --open-in-browser    Open new videos in browser
+  --shutdown           Shutdown computer once condition is met
 
 debug:
   --verbose, -v        increase verbosity (may be repeated)
   --quiet, -q          decrease verbosity (may be repeated)
   --version, -V        print version and exit
 
 logging:
```

### Comparing `youtube_monitor_action-1.0.4/youtube_monitor_action/__main__.py` & `youtube_monitor_action-1.0.5/youtube_monitor_action/__main__.py`

 * *Files identical despite different names*

### Comparing `youtube_monitor_action-1.0.4/youtube_monitor_action/_logging_utils.py` & `youtube_monitor_action-1.0.5/youtube_monitor_action/_logging_utils.py`

 * *Files identical despite different names*

### Comparing `youtube_monitor_action-1.0.4/setup.py` & `youtube_monitor_action-1.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 entry_points = \
 {'console_scripts': ['youtube-monitor-action = '
                      'youtube_monitor_action.__main__:main']}
 
 setup_kwargs = {
     'name': 'youtube-monitor-action',
-    'version': '1.0.4',
+    'version': '1.0.5',
     'description': 'Monitor for new video on YouTube Channel',
-    'long_description': '# youtube_monitor_action\nA utility to perform an action after videos are live on YouTube for a given channel.\n\nThis module provides the script `youtube-monitor-action`\n```\nusage: youtube-monitor-action [-h] [-n N] [--channel CHANNEL] [--store-config]\n                              [--hibernate] [--open-in-browser] [--verbose]\n                              [--quiet] [--version] [--log-file LOG_FILE]\n\noptional arguments:\n  -h, --help           show this help message and exit\n  -n N                 The number of new videos to watch for\n  --channel CHANNEL    (Optional) The channel id to monitor (default: load\n                       from config.yaml)\n  --store-config       Store channel and other settings in config and exit\n\nActions:\n  --hibernate          Hibernate computer once condition is met\n  --open-in-browser    Open new videos in browser\n\ndebug:\n  --verbose, -v        increase verbosity (may be repeated)\n  --quiet, -q          decrease verbosity (may be repeated)\n  --version, -V        print version and exit\n\nlogging:\n  --log-file LOG_FILE  File to log to\n```\n',
+    'long_description': '# youtube_monitor_action\nA utility to perform an action after videos are live on YouTube for a given channel.\n\nThis module provides the script `youtube-monitor-action`\n```\nusage: youtube-monitor-action [-h] [-n N] [--channel CHANNEL] [--store-config]\n                              [--hibernate] [--open-in-browser] [--shutdown]\n                              [--verbose] [--quiet] [--version]\n                              [--log-file LOG_FILE]\n\noptional arguments:\n  -h, --help           show this help message and exit\n  -n N                 The number of new videos to watch for\n  --channel CHANNEL    (Optional) The channel id to monitor (default: load\n                       from config.yaml)\n  --store-config       Store channel and other settings in config and exit\n\nActions:\n  --hibernate          Hibernate computer once condition is met\n  --open-in-browser    Open new videos in browser\n  --shutdown           Shutdown computer once condition is met\n\ndebug:\n  --verbose, -v        increase verbosity (may be repeated)\n  --quiet, -q          decrease verbosity (may be repeated)\n  --version, -V        print version and exit\n\nlogging:\n  --log-file LOG_FILE  File to log to\n```\n',
     'author': 'mshafer1',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/mshafer1/youtube_monitor_action',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `youtube_monitor_action-1.0.4/PKG-INFO` & `youtube_monitor_action-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youtube-monitor-action
-Version: 1.0.4
+Version: 1.0.5
 Summary: Monitor for new video on YouTube Channel
 Home-page: https://github.com/mshafer1/youtube_monitor_action
 License: MIT
 Author: mshafer1
 Requires-Python: >=3.6.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -21,27 +21,29 @@
 
 # youtube_monitor_action
 A utility to perform an action after videos are live on YouTube for a given channel.
 
 This module provides the script `youtube-monitor-action`
 ```
 usage: youtube-monitor-action [-h] [-n N] [--channel CHANNEL] [--store-config]
-                              [--hibernate] [--open-in-browser] [--verbose]
-                              [--quiet] [--version] [--log-file LOG_FILE]
+                              [--hibernate] [--open-in-browser] [--shutdown]
+                              [--verbose] [--quiet] [--version]
+                              [--log-file LOG_FILE]
 
 optional arguments:
   -h, --help           show this help message and exit
   -n N                 The number of new videos to watch for
   --channel CHANNEL    (Optional) The channel id to monitor (default: load
                        from config.yaml)
   --store-config       Store channel and other settings in config and exit
 
 Actions:
   --hibernate          Hibernate computer once condition is met
   --open-in-browser    Open new videos in browser
+  --shutdown           Shutdown computer once condition is met
 
 debug:
   --verbose, -v        increase verbosity (may be repeated)
   --quiet, -q          decrease verbosity (may be repeated)
   --version, -V        print version and exit
 
 logging:
```

