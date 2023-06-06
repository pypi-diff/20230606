# Comparing `tmp/aiobafi6-0.8.1.tar.gz` & `tmp/aiobafi6-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiobafi6-0.8.1.tar", max compression
+gzip compressed data, was "aiobafi6-0.8.2.tar", max compression
```

## Comparing `aiobafi6-0.8.1.tar` & `aiobafi6-0.8.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2022-04-25 18:13:16.667502 aiobafi6-0.8.1/LICENSE
--rw-r--r--   0        0        0     1626 2022-07-26 18:35:46.629783 aiobafi6-0.8.1/README.md
--rw-r--r--   0        0        0      334 2022-07-25 05:12:07.044211 aiobafi6-0.8.1/aiobafi6/__init__.py
--rw-r--r--   0        0        0        0 2022-05-04 22:08:23.762235 aiobafi6-0.8.1/aiobafi6/cmd/__init__.py
--rw-r--r--   0        0        0     8070 2022-07-27 00:25:55.993986 aiobafi6-0.8.1/aiobafi6/cmd/main.py
--rw-r--r--   0        0        0      194 2022-07-27 00:25:56.002350 aiobafi6-0.8.1/aiobafi6/const.py
--rw-r--r--   0        0        0    25282 2023-03-17 05:22:51.960216 aiobafi6-0.8.1/aiobafi6/device.py
--rw-r--r--   0        0        0     3568 2023-03-17 03:51:41.303434 aiobafi6-0.8.1/aiobafi6/device_test.py
--rw-r--r--   0        0        0     6003 2022-07-25 05:12:07.044803 aiobafi6-0.8.1/aiobafi6/discovery.py
--rw-r--r--   0        0        0     5801 2023-03-16 17:19:16.937431 aiobafi6-0.8.1/aiobafi6/proto/aiobafi6_pb2.py
--rw-r--r--   0        0        0    11171 2023-03-16 17:19:16.937599 aiobafi6-0.8.1/aiobafi6/proto/aiobafi6_pb2.pyi
--rw-r--r--   0        0        0     3948 2022-07-25 05:12:07.045010 aiobafi6-0.8.1/aiobafi6/protoprop.py
--rw-r--r--   0        0        0     2834 2022-07-25 05:12:07.045250 aiobafi6-0.8.1/aiobafi6/protoprop_test.py
--rw-r--r--   0        0        0     1503 2022-07-25 05:12:07.039232 aiobafi6-0.8.1/aiobafi6/wireutils.py
--rw-r--r--   0        0        0     1360 2022-07-25 05:12:07.039498 aiobafi6-0.8.1/aiobafi6/wireutils_test.py
--rw-r--r--   0        0        0     1280 2023-03-17 05:24:30.343980 aiobafi6-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     2476 1970-01-01 00:00:00.000000 aiobafi6-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-04-25 18:13:16.667502 aiobafi6-0.8.2/LICENSE
+-rw-r--r--   0        0        0     1626 2022-07-26 18:35:46.629783 aiobafi6-0.8.2/README.md
+-rw-r--r--   0        0        0      334 2022-07-25 05:12:07.044211 aiobafi6-0.8.2/aiobafi6/__init__.py
+-rw-r--r--   0        0        0        0 2022-05-04 22:08:23.762235 aiobafi6-0.8.2/aiobafi6/cmd/__init__.py
+-rw-r--r--   0        0        0     8070 2022-07-27 00:25:55.993986 aiobafi6-0.8.2/aiobafi6/cmd/main.py
+-rw-r--r--   0        0        0      287 2023-06-06 16:40:13.523650 aiobafi6-0.8.2/aiobafi6/const.py
+-rw-r--r--   0        0        0    25450 2023-06-06 16:40:13.528725 aiobafi6-0.8.2/aiobafi6/device.py
+-rw-r--r--   0        0        0     4327 2023-06-06 16:40:13.528920 aiobafi6-0.8.2/aiobafi6/device_test.py
+-rw-r--r--   0        0        0     6003 2022-07-25 05:12:07.044803 aiobafi6-0.8.2/aiobafi6/discovery.py
+-rw-r--r--   0        0        0     5801 2023-03-16 17:19:16.937431 aiobafi6-0.8.2/aiobafi6/proto/aiobafi6_pb2.py
+-rw-r--r--   0        0        0    11171 2023-03-16 17:19:16.937599 aiobafi6-0.8.2/aiobafi6/proto/aiobafi6_pb2.pyi
+-rw-r--r--   0        0        0     3948 2022-07-25 05:12:07.045010 aiobafi6-0.8.2/aiobafi6/protoprop.py
+-rw-r--r--   0        0        0     2834 2022-07-25 05:12:07.045250 aiobafi6-0.8.2/aiobafi6/protoprop_test.py
+-rw-r--r--   0        0        0     1503 2022-07-25 05:12:07.039232 aiobafi6-0.8.2/aiobafi6/wireutils.py
+-rw-r--r--   0        0        0     1360 2022-07-25 05:12:07.039498 aiobafi6-0.8.2/aiobafi6/wireutils_test.py
+-rw-r--r--   0        0        0     1280 2023-06-06 16:40:13.518550 aiobafi6-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     2476 1970-01-01 00:00:00.000000 aiobafi6-0.8.2/PKG-INFO
```

### Comparing `aiobafi6-0.8.1/LICENSE` & `aiobafi6-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiobafi6-0.8.1/README.md` & `aiobafi6-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `aiobafi6-0.8.1/aiobafi6/cmd/main.py` & `aiobafi6-0.8.2/aiobafi6/cmd/main.py`

 * *Files identical despite different names*

### Comparing `aiobafi6-0.8.1/aiobafi6/device.py` & `aiobafi6-0.8.2/aiobafi6/device.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import time
 import typing as t
 
 from google.protobuf import json_format
 from google.protobuf.message import Message
 
 from . import wireutils
-from .const import OCCUPANCY_MIN_API_VERSION
+from .const import DELAY_BETWEEN_CONNECTS_SECONDS, OCCUPANCY_MIN_API_VERSION
 from .discovery import Service
 from .proto import aiobafi6_pb2
 from .protoprop import (
     ClosedIntervalValidator,
     OffOnAuto,
     ProtoProp,
     from_proto_humidity,
@@ -37,15 +37,14 @@
     "current_rpm",
     "local_datetime",
     "stats",
     "utc_datetime",
 )
 
 _LOGGER = logging.getLogger(__name__)
-_DELAY_BETWEEN_CONNECT_ATTEMPTS_SECONDS = 30
 _MAX_SPEED = 7
 _RECV_BUFFER_LIMIT = 4096  # No message is ever expected to be > 4K
 _PROPS_REQUIRED_FOR_AVAILABLE = (
     "name",
     "model",
     "firmware_version",
     "mac_address",
@@ -89,14 +88,15 @@
     """
 
     def __init__(
         self,
         service: Service,
         query_interval_seconds: int = 60,
         ignore_volatile_props: bool = True,
+        delay_between_connects_seconds: int = DELAY_BETWEEN_CONNECTS_SECONDS,
     ):
         if len(service.ip_addresses) == 0 or service.port == 0:
             raise ValueError(
                 f"Invalid service: must have at least one address and a port: {service}"
             )
 
         self._service = copy.deepcopy(service)
@@ -116,14 +116,15 @@
         if self._loop is None:
             raise RuntimeError("no running loop")
         self._run_fut: t.Optional[asyncio.Future] = None
         self._stop_requested = False
         self._next_connect_ts: float = time.monotonic()
         self._connect_timer: t.Optional[asyncio.TimerHandle] = None
         self._connect_task: t.Optional[asyncio.Task] = None
+        self._delay_between_connects_seconds = delay_between_connects_seconds
         self._transport: t.Optional[asyncio.Transport] = None
         self._protocol: t.Optional[Protocol] = None
         self._query_timer: t.Optional[asyncio.TimerHandle] = None
 
         # Availability.
         self._available_event = asyncio.Event()
 
@@ -279,34 +280,30 @@
             self._connect_timer = self._loop.call_at(
                 self._next_connect_ts,
                 self._connect,
             )
 
     def _connect(self) -> None:
         self._connect_timer = None
-        self._next_connect_ts = (
-            time.monotonic() + _DELAY_BETWEEN_CONNECT_ATTEMPTS_SECONDS
-        )
+        self._next_connect_ts = time.monotonic() + self._delay_between_connects_seconds
         _LOGGER.debug(
             "%s: Connecting to %s:%s.",
             self.name,
             self._service.ip_addresses[0],
             self._service.port,
         )
         connect_task = asyncio.create_task(
             self._loop.create_connection(
                 lambda: Protocol(self),
                 self._service.ip_addresses[0],
                 self._service.port,
             )
         )
         connect_task.add_done_callback(self._finish_connect)
-        self._loop.call_later(
-            _DELAY_BETWEEN_CONNECT_ATTEMPTS_SECONDS, connect_task.cancel
-        )
+        self._loop.call_later(self._delay_between_connects_seconds, connect_task.cancel)
         self._connect_task = connect_task
 
     def _finish_connect(self, task: asyncio.Task) -> None:
         assert self._connect_task is task
         self._connect_task = None
         try:
             transport, protocol = task.result()
@@ -371,15 +368,15 @@
                 self._query_interval_seconds, self._query
             )
 
     def async_run(self) -> asyncio.Future:
         """Run the device asynchronously.
 
         A running `Device` schedules functions on the run loop to maintain a connection
-        to the device, send periodic property queries, and service query commits.
+        to the device, sends periodic property queries, and services query commits.
 
         Returns a future that will resolve when the device stops. Cancelling any future
         returned by this function will stop the device.
         """
         fut = self._loop.create_future()
         if self._run_fut is None:
             self._start()
@@ -420,30 +417,31 @@
         self._sched_connect_or_signal_run_fut()
 
     def _stop(self) -> None:
         """Stop the device."""
         if self._stop_requested:
             return
         _LOGGER.debug("%s: Stopping.", self.name)
-        # This will cause `_sched_connect` to signal `_run_fut`.
+        # This will cause `_sched_connect_or_signal_run_fut` to signal `_run_fut`.
         self._stop_requested = True
         # The device is not available anymore. Dispatch device callbacks so clients can
         # react to the change.
         self._available_event.clear()
         self._dispatch_callbacks()
         # If there is an active connection, close it.
         if self._transport is not None:
             self._transport.close()
         # Otherwise, if the device is opening a connection, cancel that.
         elif self._connect_task is not None:
             self._connect_task.cancel()
-        # Otherwise, if `_connect` is scheduled, cancel that and call `_sched_connect`
-        # directly because nothing else will.
+        # Otherwise, if `_connect` is scheduled, cancel that and call
+        # `_sched_connect_or_signal_run_fut` directly because nothing else will.
         elif self._connect_timer is not None:
             self._connect_timer.cancel()
+            self._connect_timer = None
             self._sched_connect_or_signal_run_fut()
 
     def _finish_run(self, _: asyncio.Future) -> None:
         """Reset the run future to None.
 
         This is the only completion callback for the run future and the only place where
         it is reset to None, indicating that the device has fully stopped and could be
```

### Comparing `aiobafi6-0.8.1/aiobafi6/device_test.py` & `aiobafi6-0.8.2/aiobafi6/device_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # pylint: disable=protected-access, missing-class-docstring, missing-function-docstring, invalid-name
 
 """Tests for device."""
 
+from __future__ import annotations
+
+import asyncio
+import typing as t
+
 import pytest
 
 from .device import Device
 from .discovery import PORT, Service
 from .proto import aiobafi6_pb2
 
 
@@ -120,7 +125,32 @@
     root = aiobafi6_pb2.Root()  # pylint: disable=no-member
     prop = root.root2.query_result.properties.add()
     prop.current_rpm = 42
     buf = root.SerializeToString()
     d._process_message(buf)
     assert d._properties.current_rpm == 42
     assert called
+
+
+@pytest.mark.asyncio
+async def test_cancel_between_connect_attempt():
+    d = Device(
+        Service(("127.0.0.1",), PORT),
+        ignore_volatile_props=False,
+        delay_between_connects_seconds=1,
+    )
+    fut = d.async_run()
+    except_context: t.Optional[dict[str, t.Any]] = None
+
+    def exception_handler(_: t.Any, context: dict[str, t.Any]) -> None:
+        nonlocal except_context
+        except_context = context
+
+    def cancel_fut():
+        fut.cancel()
+
+    loop = fut.get_loop()
+    loop.set_exception_handler(exception_handler)
+    loop.call_later(1.5, cancel_fut)
+    with pytest.raises(asyncio.CancelledError):
+        await fut
+    assert except_context is None
```

### Comparing `aiobafi6-0.8.1/aiobafi6/discovery.py` & `aiobafi6-0.8.2/aiobafi6/discovery.py`

 * *Files identical despite different names*

### Comparing `aiobafi6-0.8.1/aiobafi6/proto/aiobafi6_pb2.py` & `aiobafi6-0.8.2/aiobafi6/proto/aiobafi6_pb2.py`

 * *Files identical despite different names*

### Comparing `aiobafi6-0.8.1/aiobafi6/proto/aiobafi6_pb2.pyi` & `aiobafi6-0.8.2/aiobafi6/proto/aiobafi6_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiobafi6-0.8.1/aiobafi6/protoprop.py` & `aiobafi6-0.8.2/aiobafi6/protoprop.py`

 * *Files identical despite different names*

### Comparing `aiobafi6-0.8.1/aiobafi6/protoprop_test.py` & `aiobafi6-0.8.2/aiobafi6/protoprop_test.py`

 * *Files identical despite different names*

### Comparing `aiobafi6-0.8.1/aiobafi6/wireutils.py` & `aiobafi6-0.8.2/aiobafi6/wireutils.py`

 * *Files identical despite different names*

### Comparing `aiobafi6-0.8.1/aiobafi6/wireutils_test.py` & `aiobafi6-0.8.2/aiobafi6/wireutils_test.py`

 * *Files identical despite different names*

### Comparing `aiobafi6-0.8.1/pyproject.toml` & `aiobafi6-0.8.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiobafi6"
-version = "0.8.1"
+version = "0.8.2"
 description = "Big Ass Fans i6/Haiku protocol asynchronous Python library"
 authors = ["Jean-Francois Roy <jf@devklog.net>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/jfroy/aiobafi6"
 repository = "https://github.com/jfroy/aiobafi6"
 keywords = ["BigAssFans", "i6", "Haiku", "SenseME"]
@@ -16,21 +16,21 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 protobuf = ">=3.20"
 zeroconf = ">=0.38"
 
 [tool.poetry.dev-dependencies]
-black = "^23.1.0"
+black = "^23.3.0"
 isort = "^5.12.0"
-poethepoet = "^0.18.1"
-pytest = "^7.2.2"
-pytest-asyncio = "^0.20"
+poethepoet = "^0.20.0"
+pytest = "^7.3.1"
+pytest-asyncio = "^0.21"
 flake8 = "^6.0.0"
-pylint = "^2.17.0"
+pylint = "^2.17.4"
 
 [tool.poetry.scripts]
 aiobafi6 = 'aiobafi6.cmd.main:main'
 
 [tool.poe.tasks.protoc]
 cmd = "protoc --python_out=aiobafi6 --pyi_out=aiobafi6 proto/aiobafi6.proto"
 help = "Generate Python protobuf files"
```

### Comparing `aiobafi6-0.8.1/PKG-INFO` & `aiobafi6-0.8.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiobafi6
-Version: 0.8.1
+Version: 0.8.2
 Summary: Big Ass Fans i6/Haiku protocol asynchronous Python library
 Home-page: https://github.com/jfroy/aiobafi6
 License: Apache-2.0
 Keywords: BigAssFans,i6,Haiku,SenseME
 Author: Jean-Francois Roy
 Author-email: jf@devklog.net
 Requires-Python: >=3.9,<4.0
```

