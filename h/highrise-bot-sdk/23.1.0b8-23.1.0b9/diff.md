# Comparing `tmp/highrise_bot_sdk-23.1.0b8.tar.gz` & `tmp/highrise_bot_sdk-23.1.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "highrise_bot_sdk-23.1.0b8.tar", max compression
+gzip compressed data, was "highrise_bot_sdk-23.1.0b9.tar", max compression
```

## Comparing `highrise_bot_sdk-23.1.0b8.tar` & `highrise_bot_sdk-23.1.0b9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2673 2023-04-25 12:36:05.294701 highrise_bot_sdk-23.1.0b8/README.md
--rw-r--r--   0        0        0      992 2023-04-25 12:36:05.291545 highrise_bot_sdk-23.1.0b8/pyproject.toml
--rw-r--r--   0        0        0     8524 2023-04-25 12:23:39.561597 highrise_bot_sdk-23.1.0b8/src/highrise/__init__.py
--rw-r--r--   0        0        0     7907 2023-04-25 12:23:39.561633 highrise_bot_sdk-23.1.0b8/src/highrise/__main__.py
--rw-r--r--   0        0        0     3064 2023-03-31 11:07:05.693250 highrise_bot_sdk-23.1.0b8/src/highrise/_unions.py
--rw-r--r--   0        0        0     8531 2023-04-25 12:23:39.561662 highrise_bot_sdk-23.1.0b8/src/highrise/models.py
--rw-r--r--   0        0        0        0 2023-03-30 13:16:17.585454 highrise_bot_sdk-23.1.0b8/src/highrise/py.typed
--rw-r--r--   0        0        0     3656 1970-01-01 00:00:00.000000 highrise_bot_sdk-23.1.0b8/setup.py
--rw-r--r--   0        0        0     3305 1970-01-01 00:00:00.000000 highrise_bot_sdk-23.1.0b8/PKG-INFO
+-rw-r--r--   0        0        0     2898 2023-05-11 12:57:50.234072 highrise_bot_sdk-23.1.0b9/README.md
+-rw-r--r--   0        0        0      992 2023-04-28 08:59:38.259801 highrise_bot_sdk-23.1.0b9/pyproject.toml
+-rw-r--r--   0        0        0     8766 2023-05-11 11:53:57.781777 highrise_bot_sdk-23.1.0b9/src/highrise/__init__.py
+-rw-r--r--   0        0        0     8652 2023-05-11 11:54:03.830476 highrise_bot_sdk-23.1.0b9/src/highrise/__main__.py
+-rw-r--r--   0        0        0     3064 2023-03-31 11:07:05.693250 highrise_bot_sdk-23.1.0b9/src/highrise/_unions.py
+-rw-r--r--   0        0        0     8965 2023-05-11 11:54:03.830659 highrise_bot_sdk-23.1.0b9/src/highrise/models.py
+-rw-r--r--   0        0        0        0 2023-03-30 13:16:17.585454 highrise_bot_sdk-23.1.0b9/src/highrise/py.typed
+-rw-r--r--   0        0        0     3886 1970-01-01 00:00:00.000000 highrise_bot_sdk-23.1.0b9/setup.py
+-rw-r--r--   0        0        0     3530 1970-01-01 00:00:00.000000 highrise_bot_sdk-23.1.0b9/PKG-INFO
```

### Comparing `highrise_bot_sdk-23.1.0b8/README.md` & `highrise_bot_sdk-23.1.0b9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ---
 
 The Highrise Python Bot SDK is a python library for writing and running Highrise bots.
 
 First, install the library (preferably in a virtual environment):
 
 ```shell
-$ pip install highrise-bot-sdk==23.1.0b8
+$ pip install highrise-bot-sdk==23.1.0b9
 ```
 
 In the [`Settings` section of the Highrise website](https://highrise.game/account/settings), create a bot and generate the API token. You'll need the token to start your bot later.
 You will also need a room ID for your bot to connect to; the room needs to be owned by you or your bot user needs to have designer rights to enter it.
 
 Open a new file, and paste the following to get started (into `mybot.py` for example):
 
@@ -28,14 +28,19 @@
 
 ```
 $ highrise mybot:Bot <room ID> <API token>
 ```
 
 ## Changelog
 
+### 23.1.0b9 (2023-05-03)
+
+-- Add support for moving bot to an anchor in walk_to command (`self.highrise.walk_to(AnchorPosition)`).
+-- Change the way client ws messages are parsed, return error if message is not valid json.
+
 ### 23.1.0b8 (2023-04-25)
 
 - Add support for moving users to another room (`self.highrise.move_user_to_room(user_id, room_id)`).
 - Add handler that is triggered when user moves inside a room  (`self.on_user_move(user_id, position)`).) 
 - Expand session_metadata information with information about client rates
 - Expand session_metadata with information about sdk versions if client uses skd
```

### Comparing `highrise_bot_sdk-23.1.0b8/pyproject.toml` & `highrise_bot_sdk-23.1.0b9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "highrise-bot-sdk"
-version = "23.1.0.b8"
+version = "23.1.0.b9"
 description = "The Highrise Bot SDK, for running Highrise bots written in Python."
 authors = ["Pocket Worlds Inc <server@high.rs>"]
 license = "proprietary"
 readme = "README.md"
 packages = [{include = "highrise", from = "src"}]
```

### Comparing `highrise_bot_sdk-23.1.0b8/src/highrise/__init__.py` & `highrise_bot_sdk-23.1.0b9/src/highrise/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from aiohttp import ClientWebSocketResponse
 from cattrs.preconf.json import make_converter
 from quattro import TaskGroup
 
 from ._unions import configure_tagged_union
 from .models import (
+    AnchorHitRequest,
     AnchorPosition,
     ChangeRoomPrivilegeRequest,
     ChannelEvent,
     ChannelRequest,
     ChatEvent,
     ChatRequest,
     CurrencyItem,
@@ -114,15 +115,17 @@
         """On a tip received in the room."""
         pass
 
     async def on_channel(self, sender_id: str, message: str, tags: set[str]) -> None:
         """On a hidden channel message."""
         pass
 
-    async def on_user_move(self, user: User, pos: Position) -> None:
+    async def on_user_move(
+        self, user: User, destination: Position | AnchorPosition
+    ) -> None:
         """On a user moving in the room."""
         pass
 
 
 class Highrise:
     ws: ClientWebSocketResponse
     tg: TaskGroup
@@ -160,16 +163,19 @@
 
     async def set_indicator(self, icon: str | None) -> None:
         await _do_req_no_resp(self, IndicatorRequest(icon))
 
     async def send_channel(self, message: str, tags: set[str] = set()) -> None:
         await _do_req_no_resp(self, ChannelRequest(message, tags))
 
-    async def walk_to(self, destination: Position) -> None:
-        await _do_req_no_resp(self, FloorHitRequest(destination))
+    async def walk_to(self, destination: Position | AnchorPosition) -> None:
+        if isinstance(destination, AnchorPosition):
+            await _do_req_no_resp(self, AnchorHitRequest(destination))
+        else:
+            await _do_req_no_resp(self, FloorHitRequest(destination))
 
     async def teleport(self, user_id: str, dest: Position) -> None:
         await _do_req_no_resp(self, TeleportRequest(user_id, dest))
 
     async def get_room_users(self) -> GetRoomUsersRequest.GetRoomUsersResponse | Error:
         req_id = str(next(self._req_id))
         self._req_id_registry[req_id] = (q := Queue[Any](maxsize=1))
@@ -274,14 +280,15 @@
     | GetRoomUsersRequest
     | GetWalletRequest
     | GetRoomPrivilegeRequest
     | ChangeRoomPrivilegeRequest
     | ModerateRoomRequest
     | KeepaliveRequest
     | MoveUserToRoomRequest
+    | AnchorHitRequest
 )
 IncomingEvents = (
     Error
     | ChatEvent
     | EmoteEvent
     | ReactionEvent
     | UserJoinedEvent
```

### Comparing `highrise_bot_sdk-23.1.0b8/src/highrise/__main__.py` & `highrise_bot_sdk-23.1.0b9/src/highrise/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from math import ceil
 from os import environ, getcwd
 from sys import path
 from time import monotonic
 from typing import Any, AsyncGenerator, Final
 
 import pkg_resources
-from aiohttp import ClientSession, WebSocketError, WSServerHandshakeError
+from aiohttp import ClientSession, WebSocketError, WSMsgType, WSServerHandshakeError
 from click import argument, command
 from quattro import TaskGroup
 
 from . import BaseBot, Highrise, Incoming, IncomingEvents, converter
 from .models import (
     ChannelEvent,
     ChatEvent,
@@ -99,19 +99,31 @@
                                 f"does not match the recommended version for the API ({session_metadata.sdk_version})"
                             )
 
                         bot.highrise = chat
                         tg.create_task(bot.on_start(session_metadata))
                         while True:
                             frame = await ws.receive(READ_TIMEOUT)
+                            if frame.type in [WSMsgType.CLOSE, WSMsgType.CLOSED]:
+                                print(
+                                    f"ERROR connection with ID: {session_metadata.connection_id} closed."
+                                )
+                                # Close frame
+                                ka_task.cancel()
+                                return
                             if isinstance(frame.data, WebSocketError):
                                 print("Websocket error, exiting.")
                                 return
                             msg: IncomingEvents = converter.loads(frame.data, Incoming)  # type: ignore
                             match msg:
+                                case Error(message=error):
+                                    print(
+                                        f"ERROR: {error} closing connection with ID: {session_metadata.connection_id}"
+                                    )
+                                    raise ConnectionResetError
                                 case object(rid=rid) if hasattr(msg, "rid"):  # type: ignore
                                     if rid not in chat._req_id_registry:
                                         continue
                                     chat._req_id_registry.pop(rid).put_nowait(msg)
                                 case ChatEvent(
                                     message=message, user=user, whisper=whisper
                                 ):
@@ -149,15 +161,15 @@
                                     sender=sender, receiver=receiver, item=tip
                                 ):
                                     tg.create_task(bot.on_tip(sender, receiver, tip))
                                 case UserMovedEvent(user=user, position=pos):
                                     tg.create_task(bot.on_user_move(user, pos))
             except (ConnectionResetError, WSServerHandshakeError, TimeoutError):
                 # The throttler should kick in up-code.
-                print("ERROR")
+                print("ERROR: reconnecting...")
                 pass
 
 
 async def throttler(
     drops: int = 10, drop_recharge: float = 1.0
 ) -> AsyncGenerator[Any, None]:
     next_full = monotonic()
```

### Comparing `highrise_bot_sdk-23.1.0b8/src/highrise/_unions.py` & `highrise_bot_sdk-23.1.0b9/src/highrise/_unions.py`

 * *Files identical despite different names*

### Comparing `highrise_bot_sdk-23.1.0b8/src/highrise/models.py` & `highrise_bot_sdk-23.1.0b9/src/highrise/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,14 +222,33 @@
 
         rid: str | None = None
 
     Response: ClassVar = FloorHitResponse
 
 
 @define
+class AnchorHitRequest:
+    """
+    Move the bot to the given `destination`.
+
+    """
+
+    anchor: AnchorPosition
+    rid: str | None = None
+
+    @define
+    class AnchorHitResponse:
+        """The successful response to a `TeleportRequest`."""
+
+        rid: str | None = None
+
+    Response: ClassVar = AnchorHitResponse
+
+
+@define
 class GetRoomUsersRequest:
     """
     Fetch the list of users currently in the room, with their positions.
 
     """
 
     rid: str
@@ -367,21 +386,23 @@
     """
     Initial session data.
 
     This will be sent once, as the first message when a connection is established.
     user_id is the bot's user id.
     rate_limits is a dictionary of rate limits, with the key being the rate limit name and the value being a tuple of
     (limit, period).
+    connection_id is the connection id of the websocket used in bot connection.
     sdk_versions is a string containing the SDK versions recommended by the server if user is using SDK.
 
 
     """
 
     user_id: str
     rate_limits: dict[str, tuple[int, float]]
+    connection_id: str
     sdk_version: str | None = None
 
 
 @define
 class ChatEvent:
     """
     A chat event, sent by a `user` in the room.
```

### Comparing `highrise_bot_sdk-23.1.0b8/setup.py` & `highrise_bot_sdk-23.1.0b9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,17 +17,17 @@
  'quattro>=22.1.0,<23.0.0']
 
 entry_points = \
 {'console_scripts': ['highrise = highrise.__main__:run']}
 
 setup_kwargs = {
     'name': 'highrise-bot-sdk',
-    'version': '23.1.0b8',
+    'version': '23.1.0b9',
     'description': 'The Highrise Bot SDK, for running Highrise bots written in Python.',
-    'long_description': "# The Highrise Python Bot SDK\n\n---\n\nThe Highrise Python Bot SDK is a python library for writing and running Highrise bots.\n\nFirst, install the library (preferably in a virtual environment):\n\n```shell\n$ pip install highrise-bot-sdk==23.1.0b8\n```\n\nIn the [`Settings` section of the Highrise website](https://highrise.game/account/settings), create a bot and generate the API token. You'll need the token to start your bot later.\nYou will also need a room ID for your bot to connect to; the room needs to be owned by you or your bot user needs to have designer rights to enter it.\n\nOpen a new file, and paste the following to get started (into `mybot.py` for example):\n\n```python\nfrom highrise import BaseBot\n\nclass Bot(BaseBot):\n    pass\n```\n\nOverride methods from `BaseBot` as needed.\n\nWhen you're ready, run the bot from the terminal using the SDK, giving it the Python path to the Bot class:\n\n```\n$ highrise mybot:Bot <room ID> <API token>\n```\n\n## Changelog\n\n### 23.1.0b8 (2023-04-25)\n\n- Add support for moving users to another room (`self.highrise.move_user_to_room(user_id, room_id)`).\n- Add handler that is triggered when user moves inside a room  (`self.on_user_move(user_id, position)`).) \n- Expand session_metadata information with information about client rates\n- Expand session_metadata with information about sdk versions if client uses skd\n\n### 23.1.0b6 (2023-04-17)\n\n- Add Python 3.10 support\n\n### 23.1.0b5 (2023-04-11)\n\n- Add support for getting room permissions for users (`self.highrise.get_room_privilege(user_id)`).\n- Add support changing room permissions for users (`self.highrise.set_room_privilege(user_id, privilege)`).\n- Add support for moderating rooms (`self.highrise.moderate_room(user_id, moderate_action, action_length)`). \n- Rework how keepalive is handled\n\n### 23.1.0b4 (2023-04-05)\n\n- Methods mapping to requests with empty responses (`chat`, `send_whisper`, `send_emote`, `react`, `set_indicator`, `send_channel`, `walk_to`, `teleport`) now return `None`, and raise a `highrise.ResponseError` on an error response.\n- Fix the emote API.\n- Internally rework request handling to improve robustness.\n\n### 23.1.0b3 (2023-04-03)\n\n- Fix the chatting API.\n\n### 23.1.0b2 (2023-04-03)\n\n- Add support for receiving and sending reactions.\n- Fix support for hidden channels.\n- Migrate to the new message for avatars leaving.\n- Improve concurrency when awaiting bot methods.\n- Fix issues with teleporting users.\n- Fix issues with user coordinates.\n- Add support for fetching the bot wallet (`self.highrise.get_wallet()`).\n\n### 23.1.0b1 (2023-03-28)\n\n- Add support for emotes and hidden channel messages.\n\n### 23.1.0b0 (2023-03-10)\n\n- Initial beta release.\n",
+    'long_description': "# The Highrise Python Bot SDK\n\n---\n\nThe Highrise Python Bot SDK is a python library for writing and running Highrise bots.\n\nFirst, install the library (preferably in a virtual environment):\n\n```shell\n$ pip install highrise-bot-sdk==23.1.0b9\n```\n\nIn the [`Settings` section of the Highrise website](https://highrise.game/account/settings), create a bot and generate the API token. You'll need the token to start your bot later.\nYou will also need a room ID for your bot to connect to; the room needs to be owned by you or your bot user needs to have designer rights to enter it.\n\nOpen a new file, and paste the following to get started (into `mybot.py` for example):\n\n```python\nfrom highrise import BaseBot\n\nclass Bot(BaseBot):\n    pass\n```\n\nOverride methods from `BaseBot` as needed.\n\nWhen you're ready, run the bot from the terminal using the SDK, giving it the Python path to the Bot class:\n\n```\n$ highrise mybot:Bot <room ID> <API token>\n```\n\n## Changelog\n\n### 23.1.0b9 (2023-05-03)\n\n-- Add support for moving bot to an anchor in walk_to command (`self.highrise.walk_to(AnchorPosition)`).\n-- Change the way client ws messages are parsed, return error if message is not valid json.\n\n### 23.1.0b8 (2023-04-25)\n\n- Add support for moving users to another room (`self.highrise.move_user_to_room(user_id, room_id)`).\n- Add handler that is triggered when user moves inside a room  (`self.on_user_move(user_id, position)`).) \n- Expand session_metadata information with information about client rates\n- Expand session_metadata with information about sdk versions if client uses skd\n\n### 23.1.0b6 (2023-04-17)\n\n- Add Python 3.10 support\n\n### 23.1.0b5 (2023-04-11)\n\n- Add support for getting room permissions for users (`self.highrise.get_room_privilege(user_id)`).\n- Add support changing room permissions for users (`self.highrise.set_room_privilege(user_id, privilege)`).\n- Add support for moderating rooms (`self.highrise.moderate_room(user_id, moderate_action, action_length)`). \n- Rework how keepalive is handled\n\n### 23.1.0b4 (2023-04-05)\n\n- Methods mapping to requests with empty responses (`chat`, `send_whisper`, `send_emote`, `react`, `set_indicator`, `send_channel`, `walk_to`, `teleport`) now return `None`, and raise a `highrise.ResponseError` on an error response.\n- Fix the emote API.\n- Internally rework request handling to improve robustness.\n\n### 23.1.0b3 (2023-04-03)\n\n- Fix the chatting API.\n\n### 23.1.0b2 (2023-04-03)\n\n- Add support for receiving and sending reactions.\n- Fix support for hidden channels.\n- Migrate to the new message for avatars leaving.\n- Improve concurrency when awaiting bot methods.\n- Fix issues with teleporting users.\n- Fix issues with user coordinates.\n- Add support for fetching the bot wallet (`self.highrise.get_wallet()`).\n\n### 23.1.0b1 (2023-03-28)\n\n- Add support for emotes and hidden channel messages.\n\n### 23.1.0b0 (2023-03-10)\n\n- Initial beta release.\n",
     'author': 'Pocket Worlds Inc',
     'author_email': 'server@high.rs',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `highrise_bot_sdk-23.1.0b8/PKG-INFO` & `highrise_bot_sdk-23.1.0b9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: highrise-bot-sdk
-Version: 23.1.0b8
+Version: 23.1.0b9
 Summary: The Highrise Bot SDK, for running Highrise bots written in Python.
 License: Proprietary
 Author: Pocket Worlds Inc
 Author-email: server@high.rs
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -21,15 +21,15 @@
 ---
 
 The Highrise Python Bot SDK is a python library for writing and running Highrise bots.
 
 First, install the library (preferably in a virtual environment):
 
 ```shell
-$ pip install highrise-bot-sdk==23.1.0b8
+$ pip install highrise-bot-sdk==23.1.0b9
 ```
 
 In the [`Settings` section of the Highrise website](https://highrise.game/account/settings), create a bot and generate the API token. You'll need the token to start your bot later.
 You will also need a room ID for your bot to connect to; the room needs to be owned by you or your bot user needs to have designer rights to enter it.
 
 Open a new file, and paste the following to get started (into `mybot.py` for example):
 
@@ -46,14 +46,19 @@
 
 ```
 $ highrise mybot:Bot <room ID> <API token>
 ```
 
 ## Changelog
 
+### 23.1.0b9 (2023-05-03)
+
+-- Add support for moving bot to an anchor in walk_to command (`self.highrise.walk_to(AnchorPosition)`).
+-- Change the way client ws messages are parsed, return error if message is not valid json.
+
 ### 23.1.0b8 (2023-04-25)
 
 - Add support for moving users to another room (`self.highrise.move_user_to_room(user_id, room_id)`).
 - Add handler that is triggered when user moves inside a room  (`self.on_user_move(user_id, position)`).) 
 - Expand session_metadata information with information about client rates
 - Expand session_metadata with information about sdk versions if client uses skd
```

