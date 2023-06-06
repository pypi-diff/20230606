# Comparing `tmp/melnor-bluetooth-0.0.8.tar.gz` & `tmp/melnor-bluetooth-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melnor-bluetooth-0.0.8.tar", max compression
+gzip compressed data, was "melnor-bluetooth-0.0.9.tar", max compression
```

## Comparing `melnor-bluetooth-0.0.8.tar` & `melnor-bluetooth-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2022-04-29 01:15:34.764551 melnor-bluetooth-0.0.8/LICENSE
--rw-r--r--   0        0        0     2072 2022-04-29 01:15:34.764551 melnor-bluetooth-0.0.8/README.md
--rw-r--r--   0        0        0       22 2022-04-29 01:16:14.420988 melnor-bluetooth-0.0.8/melnor_bluetooth/__init__.py
--rw-r--r--   0        0        0     2183 2022-04-29 01:15:34.764551 melnor-bluetooth-0.0.8/melnor_bluetooth/constants.py
--rw-r--r--   0        0        0     9396 2022-04-29 01:15:34.764551 melnor-bluetooth-0.0.8/melnor_bluetooth/device.py
--rw-r--r--   0        0        0      435 2022-04-29 01:15:34.764551 melnor-bluetooth-0.0.8/melnor_bluetooth/parser/battery.py
--rw-r--r--   0        0        0     1665 2022-04-29 01:15:34.764551 melnor-bluetooth-0.0.8/melnor_bluetooth/parser/date.py
--rw-r--r--   0        0        0     1392 2022-04-29 01:15:34.764551 melnor-bluetooth-0.0.8/melnor_bluetooth/scanner.py
--rw-r--r--   0        0        0     1781 2022-04-29 01:16:14.416988 melnor-bluetooth-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2958 2022-04-29 01:16:14.489748 melnor-bluetooth-0.0.8/setup.py
--rw-r--r--   0        0        0     3011 2022-04-29 01:16:14.490101 melnor-bluetooth-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2022-04-30 18:58:51.821485 melnor-bluetooth-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2072 2022-04-30 18:58:51.821485 melnor-bluetooth-0.0.9/README.md
+-rw-r--r--   0        0        0       22 2022-04-30 18:59:38.002135 melnor-bluetooth-0.0.9/melnor_bluetooth/__init__.py
+-rw-r--r--   0        0        0     2183 2022-04-30 18:58:51.821485 melnor-bluetooth-0.0.9/melnor_bluetooth/constants.py
+-rw-r--r--   0        0        0     9202 2022-04-30 18:58:51.821485 melnor-bluetooth-0.0.9/melnor_bluetooth/device.py
+-rw-r--r--   0        0        0      435 2022-04-30 18:58:51.821485 melnor-bluetooth-0.0.9/melnor_bluetooth/parser/battery.py
+-rw-r--r--   0        0        0     1665 2022-04-30 18:58:51.821485 melnor-bluetooth-0.0.9/melnor_bluetooth/parser/date.py
+-rw-r--r--   0        0        0     1392 2022-04-30 18:58:51.821485 melnor-bluetooth-0.0.9/melnor_bluetooth/scanner.py
+-rw-r--r--   0        0        0     1781 2022-04-30 18:59:38.002135 melnor-bluetooth-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2958 2022-04-30 18:59:38.086920 melnor-bluetooth-0.0.9/setup.py
+-rw-r--r--   0        0        0     3011 2022-04-30 18:59:38.087340 melnor-bluetooth-0.0.9/PKG-INFO
```

### Comparing `melnor-bluetooth-0.0.8/LICENSE` & `melnor-bluetooth-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `melnor-bluetooth-0.0.8/README.md` & `melnor-bluetooth-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `melnor-bluetooth-0.0.8/melnor_bluetooth/constants.py` & `melnor-bluetooth-0.0.9/melnor_bluetooth/constants.py`

 * *Files identical despite different names*

### Comparing `melnor-bluetooth-0.0.8/melnor_bluetooth/device.py` & `melnor-bluetooth-0.0.9/melnor_bluetooth/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 import asyncio
-import os
-import platform
 import struct
 from typing import Any, List, Union
 
 from bleak import BleakClient, BleakError
 
 from melnor_bluetooth.parser.battery import parse_battery_value
 from melnor_bluetooth.parser.date import get_timestamp, time_shift
@@ -170,18 +168,14 @@
             except BleakError:
                 print("Failed to connect to:", self._mac)
                 self._is_connected = False
 
     async def disconnect(self) -> None:
         await self._connection.disconnect()
 
-        # bluez tends to hang on to a device connection for too long
-        if platform.system() == "Linux":
-            os.system(f"bluetoothctl remove {self.mac}")
-
     async def fetch_state(self) -> None:
         """Updates the state of the device with the given bytes"""
 
         uuids = [
             BATTERY_UUID,
             VALVE_MANUAL_SETTINGS_UUID,
             VALVE_MANUAL_STATES_UUID,
```

### Comparing `melnor-bluetooth-0.0.8/melnor_bluetooth/parser/date.py` & `melnor-bluetooth-0.0.9/melnor_bluetooth/parser/date.py`

 * *Files identical despite different names*

### Comparing `melnor-bluetooth-0.0.8/melnor_bluetooth/scanner.py` & `melnor-bluetooth-0.0.9/melnor_bluetooth/scanner.py`

 * *Files identical despite different names*

### Comparing `melnor-bluetooth-0.0.8/pyproject.toml` & `melnor-bluetooth-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "home automation",
     "irrigation",
     "gardening"
 ]
 license = "MIT"
 name = "melnor-bluetooth"
 readme = "README.md"
-version = "0.0.8"
+version = "0.0.9"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 88
```

### Comparing `melnor-bluetooth-0.0.8/setup.py` & `melnor-bluetooth-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['aioconsole>=0.4.1,<0.5.0',
  'bleak>=0.14.2,<0.15.0',
  'tzdata>=2022.1,<2023.0',
  'tzlocal>=4.1,<5.0']
 
 setup_kwargs = {
     'name': 'melnor-bluetooth',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'A small python library for discovery and interacting with Melnor, Eden, etc Bluetooth water timers.',
     'long_description': '# Melnor Bluetooth\n\n![PyPI](https://img.shields.io/pypi/v/melnor-bluetooth?style=flat-square) ![Codecov branch](https://img.shields.io/codecov/c/github/vanstinator/melnor-bluetooth/main?style=flat-square) ![GitHub Workflow Status (branch)](https://img.shields.io/github/workflow/status/vanstinator/melnor-bluetooth/Build%20and%20Release/main?style=flat-square)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/melnor-bluetooth?style=flat-square)\n\nMelnor Bluetooth is a reverse engineered implementation of the Bluetooth protocol for all "smart" bluetooth-enabled watering valves under the Melnor, EcoAquastar, Eden, and other brands.\n\nThe library _should_ run on MacOS, Linux, or Windows. It\'s primarily developed on MacOS and other platforms likely have bugs. PRs and tests are welcome to improve quality across all platforms.\n\n\n### Getting Started\n\n#### CLI\nA simple CLI has been provided for basic debugging purposes. It\'s not intended for any real use and isn\'t suitable for running a valve in the real world.\n\nThis project uses poetry for dependency management and building. Running this project locally is as simple as the following steps:\n\n1. Clone the repository\n1. `poetry install`\n1. `poetry run cli.py`\n\n\nThe python API has been designed to be as easy to use as possible. A few examples are provided below:\n\n#### Read battery state\n```python\n  import asyncio\n\n  from melnor_bluetooth.constants import BATTERY_UUID\n  from melnor_bluetooth.device import Device\n\n  address = \'00:00:00:00:00\' # fill with your device mac address\n\n  async main():\n    device = Device(address, 4)\n    await device.connect()\n\n    print(device.battery_life);\n\n    await device.disconnect();\n\n  asyncio.run(main())\n\n```\n\n#### Turn on a zone\n```python\n  import asyncio\n\n  from melnor_bluetooth.device import Device\n\n  address = \'00:00:00:00:00\' # fill with your device mac address\n\n  async main():\n    device = Device(address, 4)\n    await device.connect()\n\n    device.zone1.is_watering = True;\n\n    await device.push_state();\n    await device.disconnect();\n\n  asyncio.run(main())\n\n```\n',
     'author': 'Justin Vanderhooft',
     'author_email': 'justinvdhooft@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `melnor-bluetooth-0.0.8/PKG-INFO` & `melnor-bluetooth-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: melnor-bluetooth
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small python library for discovery and interacting with Melnor, Eden, etc Bluetooth water timers.
 License: MIT
 Keywords: bluetooth,melnor,home automation,irrigation,gardening
 Author: Justin Vanderhooft
 Author-email: justinvdhooft@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

