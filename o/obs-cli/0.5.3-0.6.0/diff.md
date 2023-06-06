# Comparing `tmp/obs-cli-0.5.3.tar.gz` & `tmp/obs-cli-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obs-cli-0.5.3.tar", last modified: Tue Jun  6 05:55:18 2023, max compression
+gzip compressed data, was "obs-cli-0.6.0.tar", last modified: Tue Jun  6 08:10:16 2023, max compression
```

## Comparing `obs-cli-0.5.3.tar` & `obs-cli-0.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:55:18.301294 obs-cli-0.5.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:55:18.301294 obs-cli-0.5.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-06 05:55:08.000000 obs-cli-0.5.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:55:18.301294 obs-cli-0.5.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-06 05:55:08.000000 obs-cli-0.5.3/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-06 05:55:08.000000 obs-cli-0.5.3/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-06 05:55:08.000000 obs-cli-0.5.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-06 05:55:08.000000 obs-cli-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    43315 2023-06-06 05:55:18.301294 obs-cli-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-06 05:55:08.000000 obs-cli-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:55:18.301294 obs-cli-0.5.3/obs_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43315 2023-06-06 05:55:18.000000 obs-cli-0.5.3/obs_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-06 05:55:18.000000 obs-cli-0.5.3/obs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 05:55:18.000000 obs-cli-0.5.3/obs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-06 05:55:18.000000 obs-cli-0.5.3/obs_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 05:55:18.000000 obs-cli-0.5.3/obs_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 05:55:18.000000 obs-cli-0.5.3/obs_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-06-06 05:55:08.000000 obs-cli-0.5.3/obs_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-06 05:55:08.000000 obs-cli-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 05:55:18.301294 obs-cli-0.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:10:16.132012 obs-cli-0.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:10:16.128012 obs-cli-0.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-06 08:10:01.000000 obs-cli-0.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:10:16.128012 obs-cli-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-06 08:10:01.000000 obs-cli-0.6.0/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-06 08:10:01.000000 obs-cli-0.6.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-06 08:10:01.000000 obs-cli-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-06 08:10:01.000000 obs-cli-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44502 2023-06-06 08:10:16.128012 obs-cli-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-06-06 08:10:01.000000 obs-cli-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:10:16.128012 obs-cli-0.6.0/obs_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44502 2023-06-06 08:10:16.000000 obs-cli-0.6.0/obs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-06 08:10:16.000000 obs-cli-0.6.0/obs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 08:10:16.000000 obs-cli-0.6.0/obs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-06 08:10:16.000000 obs-cli-0.6.0/obs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 08:10:16.000000 obs-cli-0.6.0/obs_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 08:10:16.000000 obs-cli-0.6.0/obs_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15200 2023-06-06 08:10:01.000000 obs-cli-0.6.0/obs_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-06 08:10:01.000000 obs-cli-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 08:10:16.132012 obs-cli-0.6.0/setup.cfg
```

### Comparing `obs-cli-0.5.3/.github/workflows/release.yaml` & `obs-cli-0.6.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `obs-cli-0.5.3/LICENSE` & `obs-cli-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `obs-cli-0.5.3/PKG-INFO` & `obs-cli-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obs-cli
-Version: 0.5.3
+Version: 0.6.0
 Summary: OBS CLI
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -818,11 +818,107 @@
 
 To list all hotkeys:
 
 ```shell
 obs-cli hotkey list
 ```
 
+### 🎥 Virtual Camera Management
+
+You can manage the virtual camera using the `virtualcam` command:
+
+```shell
+obs-cli virtualcam --help
+```
+
+For example, to start the virtual camera:
+
+```shell
+obs-cli virtualcam start
+```
+
+To stop the virtual camera:
+
+```shell
+obs-cli virtualcam stop
+```
+
+To toggle the virtual camera:
+
+```shell
+obs-cli virtualcam toggle
+```
+
+To get the status of the virtual camera:
+
+```shell
+obs-cli virtualcam status
+```
+
+### 📡 Stream Management
+
+You can manage the stream using the `stream` command:
+
+```shell
+obs-cli stream --help
+```
+
+For example, to start streaming:
+
+```shell
+obs-cli stream start
+```
+
+To stop streaming:
+
+```shell
+obs-cli stream stop
+```
+
+To toggle streaming:
+
+```shell
+obs-cli stream toggle
+```
+
+To get the status of the stream:
+
+```shell
+obs-cli stream status
+```
+
+### 🎥 Record Management
+
+You can manage recording using the `record` command:
+
+```shell
+obs-cli record --help
+```
+
+For example, to start recording:
+
+```shell
+obs-cli record start
+```
+
+To stop recording:
+
+```shell
+obs-cli record stop
+```
+
+To toggle recording:
+
+```shell
+obs-cli record toggle
+```
+
+To get the status of the recording:
+
+```shell
+obs-cli record status
+```
+
 ## 📄 License
 
 This project is licensed under the GPL-3.0 License. See [LICENSE](LICENSE) for more information.
```

### Comparing `obs-cli-0.5.3/README.md` & `obs-cli-0.6.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -132,11 +132,107 @@
 
 To list all hotkeys:
 
 ```shell
 obs-cli hotkey list
 ```
 
+### 🎥 Virtual Camera Management
+
+You can manage the virtual camera using the `virtualcam` command:
+
+```shell
+obs-cli virtualcam --help
+```
+
+For example, to start the virtual camera:
+
+```shell
+obs-cli virtualcam start
+```
+
+To stop the virtual camera:
+
+```shell
+obs-cli virtualcam stop
+```
+
+To toggle the virtual camera:
+
+```shell
+obs-cli virtualcam toggle
+```
+
+To get the status of the virtual camera:
+
+```shell
+obs-cli virtualcam status
+```
+
+### 📡 Stream Management
+
+You can manage the stream using the `stream` command:
+
+```shell
+obs-cli stream --help
+```
+
+For example, to start streaming:
+
+```shell
+obs-cli stream start
+```
+
+To stop streaming:
+
+```shell
+obs-cli stream stop
+```
+
+To toggle streaming:
+
+```shell
+obs-cli stream toggle
+```
+
+To get the status of the stream:
+
+```shell
+obs-cli stream status
+```
+
+### 🎥 Record Management
+
+You can manage recording using the `record` command:
+
+```shell
+obs-cli record --help
+```
+
+For example, to start recording:
+
+```shell
+obs-cli record start
+```
+
+To stop recording:
+
+```shell
+obs-cli record stop
+```
+
+To toggle recording:
+
+```shell
+obs-cli record toggle
+```
+
+To get the status of the recording:
+
+```shell
+obs-cli record status
+```
+
 ## 📄 License
 
 This project is licensed under the GPL-3.0 License. See [LICENSE](LICENSE) for more information.
```

### Comparing `obs-cli-0.5.3/obs_cli.egg-info/PKG-INFO` & `obs-cli-0.6.0/obs_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obs-cli
-Version: 0.5.3
+Version: 0.6.0
 Summary: OBS CLI
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -818,11 +818,107 @@
 
 To list all hotkeys:
 
 ```shell
 obs-cli hotkey list
 ```
 
+### 🎥 Virtual Camera Management
+
+You can manage the virtual camera using the `virtualcam` command:
+
+```shell
+obs-cli virtualcam --help
+```
+
+For example, to start the virtual camera:
+
+```shell
+obs-cli virtualcam start
+```
+
+To stop the virtual camera:
+
+```shell
+obs-cli virtualcam stop
+```
+
+To toggle the virtual camera:
+
+```shell
+obs-cli virtualcam toggle
+```
+
+To get the status of the virtual camera:
+
+```shell
+obs-cli virtualcam status
+```
+
+### 📡 Stream Management
+
+You can manage the stream using the `stream` command:
+
+```shell
+obs-cli stream --help
+```
+
+For example, to start streaming:
+
+```shell
+obs-cli stream start
+```
+
+To stop streaming:
+
+```shell
+obs-cli stream stop
+```
+
+To toggle streaming:
+
+```shell
+obs-cli stream toggle
+```
+
+To get the status of the stream:
+
+```shell
+obs-cli stream status
+```
+
+### 🎥 Record Management
+
+You can manage recording using the `record` command:
+
+```shell
+obs-cli record --help
+```
+
+For example, to start recording:
+
+```shell
+obs-cli record start
+```
+
+To stop recording:
+
+```shell
+obs-cli record stop
+```
+
+To toggle recording:
+
+```shell
+obs-cli record toggle
+```
+
+To get the status of the recording:
+
+```shell
+obs-cli record status
+```
+
 ## 📄 License
 
 This project is licensed under the GPL-3.0 License. See [LICENSE](LICENSE) for more information.
```

### Comparing `obs-cli-0.5.3/obs_cli.py` & `obs-cli-0.6.0/obs_cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -85,14 +85,38 @@
         "action",
         choices=["list", "trigger"],
         default="list",
         help="list/trigger",
     )
     hotkey_parser.add_argument("HOTKEY", nargs="?", help="Hotkey name")
 
+    virtualcam_parser = subparsers.add_parser("virtualcam")
+    virtualcam_parser.add_argument(
+        "action",
+        choices=["status", "start", "stop", "toggle"],
+        default="status",
+        help="status/start/stop/toggle",
+    )
+
+    stream_parser = subparsers.add_parser("stream")
+    stream_parser.add_argument(
+        "action",
+        choices=["status", "start", "stop", "toggle"],
+        default="status",
+        help="status/start/stop/toggle",
+    )
+
+    record_parser = subparsers.add_parser("record")
+    record_parser.add_argument(
+        "action",
+        choices=["status", "start", "stop", "toggle"],
+        default="status",
+        help="status/start/stop/toggle",
+    )
+
     return parser.parse_args()
 
 
 def switch_to_scene(cl, scene, exact=False, ignorecase=True):
     regex = re.compile(
         f"^{scene}$" if exact else scene,
         re.IGNORECASE if ignorecase else re.NOFLAG,
@@ -203,14 +227,62 @@
     return cl.get_hot_key_list().hotkeys
 
 
 def trigger_hotkey(cl, hotkey):
     return cl.trigger_hot_key_by_name(hotkey)
 
 
+def virtual_camera_status(cl):
+    return cl.get_virtual_cam_status().output_active
+
+
+def virtual_camera_start(cl):
+    return cl.start_virtual_cam()
+
+
+def virtual_camera_stop(cl):
+    return cl.stop_virtual_cam()
+
+
+def virtual_camera_toggle(cl):
+    return cl.toggle_virtual_cam()
+
+
+def stream_status(cl):
+    return cl.get_stream_status().output_active
+
+
+def stream_start(cl):
+    return cl.start_stream()
+
+
+def stream_stop(cl):
+    return cl.stop_stream()
+
+
+def stream_toggle(cl):
+    return cl.toggle_stream()
+
+
+def record_status(cl):
+    return cl.get_record_status().output_active
+
+
+def record_start(cl):
+    return cl.start_record()
+
+
+def record_stop(cl):
+    return cl.stop_record()
+
+
+def record_toggle(cl):
+    return cl.toggle_record()
+
+
 def main():
     console = Console()
     logging.basicConfig()
 
     args = parse_args()
     LOGGER.setLevel(logging.DEBUG if args.debug else logging.INFO)
     LOGGER.debug(args)
@@ -338,14 +410,65 @@
                 for hk in data:
                     table.add_row(hk)
                 console.print(table)
             elif args.action == "trigger":
                 res = trigger_hotkey(cl, args.HOTKEY)
                 LOGGER.debug(res)
 
+        elif cmd == "virtualcam":
+            if args.action == "status":
+                res = virtual_camera_status(cl)
+                LOGGER.debug(res)
+                if args.quiet:
+                    sys.exit(0 if res else 1)
+                print("started" if res else "stopped")
+            elif args.action == "start":
+                res = virtual_camera_start(cl)
+                LOGGER.debug(res)
+            elif args.action == "stop":
+                res = virtual_camera_stop(cl)
+                LOGGER.debug(res)
+            elif args.action == "toggle":
+                res = virtual_camera_toggle(cl)
+                LOGGER.debug(res)
+
+        elif cmd == "stream":
+            if args.action == "status":
+                res = stream_status(cl)
+                LOGGER.debug(res)
+                if args.quiet:
+                    sys.exit(0 if res else 1)
+                print("started" if res else "stopped")
+            elif args.action == "start":
+                res = stream_start(cl)
+                LOGGER.debug(res)
+            elif args.action == "stop":
+                res = stream_stop(cl)
+                LOGGER.debug(res)
+            elif args.action == "toggle":
+                res = stream_toggle(cl)
+                LOGGER.debug(res)
+
+        elif cmd == "record":
+            if args.action == "status":
+                res = record_status(cl)
+                LOGGER.debug(res)
+                if args.quiet:
+                    sys.exit(0 if res else 1)
+                print("started" if res else "stopped")
+            elif args.action == "start":
+                res = record_start(cl)
+                LOGGER.debug(res)
+            elif args.action == "stop":
+                res = record_stop(cl)
+                LOGGER.debug(res)
+            elif args.action == "toggle":
+                res = record_toggle(cl)
+                LOGGER.debug(res)
+
         return 0
     except Exception:
         console.print_exception(show_locals=True)
         return 1
 
 
 LOGGER = logging.getLogger(__name__)
```

### Comparing `obs-cli-0.5.3/pyproject.toml` & `obs-cli-0.6.0/pyproject.toml`

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
-version = "0.5.3"
+version = "0.6.0"
 
 [tool.black]
 line-length = 79
 
 [project.scripts]
 obs-cli = "obs_cli:main"
```

