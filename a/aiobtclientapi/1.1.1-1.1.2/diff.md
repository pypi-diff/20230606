# Comparing `tmp/aiobtclientapi-1.1.1.tar.gz` & `tmp/aiobtclientapi-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiobtclientapi-1.1.1.tar", last modified: Fri May 26 15:23:33 2023, max compression
+gzip compressed data, was "aiobtclientapi-1.1.2.tar", last modified: Tue Jun  6 11:45:17 2023, max compression
```

## Comparing `aiobtclientapi-1.1.1.tar` & `aiobtclientapi-1.1.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-26 15:23:33.626157 aiobtclientapi-1.1.1/
--rw-------   0 ich       (1000) ich       (1000)    35149 2022-07-05 13:26:49.000000 aiobtclientapi-1.1.1/LICENSE
--rw-------   0 ich       (1000) ich       (1000)     1198 2023-05-26 15:23:33.626157 aiobtclientapi-1.1.1/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)      592 2022-08-27 13:56:53.000000 aiobtclientapi-1.1.1/README.rst
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-26 15:23:33.614157 aiobtclientapi-1.1.1/aiobtclientapi/
--rw-------   0 ich       (1000) ich       (1000)     1930 2023-05-26 14:25:52.000000 aiobtclientapi-1.1.1/aiobtclientapi/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     3976 2023-05-14 09:04:17.000000 aiobtclientapi-1.1.1/aiobtclientapi/cli.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-26 15:23:33.618157 aiobtclientapi-1.1.1/aiobtclientapi/clients/
--rw-------   0 ich       (1000) ich       (1000)      208 2022-08-04 15:44:22.000000 aiobtclientapi-1.1.1/aiobtclientapi/clients/__init__.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-26 15:23:33.618157 aiobtclientapi-1.1.1/aiobtclientapi/clients/base/
--rw-------   0 ich       (1000) ich       (1000)       25 2022-06-16 09:50:40.000000 aiobtclientapi-1.1.1/aiobtclientapi/clients/base/__init__.py
--rw-------   0 ich       (1000) ich       (1000)    18437 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.1/aiobtclientapi/clients/base/api.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-26 15:23:33.618157 aiobtclientapi-1.1.1/aiobtclientapi/clients/deluge/
--rw-------   0 ich       (1000) ich       (1000)       27 2022-07-26 09:47:43.000000 aiobtclientapi-1.1.1/aiobtclientapi/clients/deluge/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     6016 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.1/aiobtclientapi/clients/deluge/api.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-26 15:23:33.622157 aiobtclientapi-1.1.1/aiobtclientapi/clients/qbittorrent/
--rw-------   0 ich       (1000) ich       (1000)       32 2022-07-27 09:37:07.000000 aiobtclientapi-1.1.1/aiobtclientapi/clients/qbittorrent/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     5830 2023-05-26 14:24:26.000000 aiobtclientapi-1.1.1/aiobtclientapi/clients/qbittorrent/api.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-26 15:23:33.622157 aiobtclientapi-1.1.1/aiobtclientapi/clients/rtorrent/
--rw-------   0 ich       (1000) ich       (1000)       29 2022-07-27 15:40:51.000000 aiobtclientapi-1.1.1/aiobtclientapi/clients/rtorrent/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     6595 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.1/aiobtclientapi/clients/rtorrent/api.py
--rw-------   0 ich       (1000) ich       (1000)     1558 2023-05-18 09:45:43.000000 aiobtclientapi-1.1.1/aiobtclientapi/clients/rtorrent/utils.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-26 15:23:33.622157 aiobtclientapi-1.1.1/aiobtclientapi/clients/transmission/
--rw-------   0 ich       (1000) ich       (1000)       33 2022-07-30 14:17:58.000000 aiobtclientapi-1.1.1/aiobtclientapi/clients/transmission/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     6480 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.1/aiobtclientapi/clients/transmission/api.py
--rw-------   0 ich       (1000) ich       (1000)      418 2022-07-30 14:17:58.000000 aiobtclientapi-1.1.1/aiobtclientapi/clients/transmission/enums.py
--rw-------   0 ich       (1000) ich       (1000)       69 2022-07-05 13:26:49.000000 aiobtclientapi-1.1.1/aiobtclientapi/constants.py
--rw-------   0 ich       (1000) ich       (1000)     5466 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.1/aiobtclientapi/errors.py
--rw-------   0 ich       (1000) ich       (1000)     7696 2022-08-05 11:03:47.000000 aiobtclientapi-1.1.1/aiobtclientapi/response.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-26 15:23:33.626157 aiobtclientapi-1.1.1/aiobtclientapi/utils/
--rw-------   0 ich       (1000) ich       (1000)     6024 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.1/aiobtclientapi/utils/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     6674 2022-08-01 15:15:03.000000 aiobtclientapi-1.1.1/aiobtclientapi/utils/monitor.py
--rw-------   0 ich       (1000) ich       (1000)     2634 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.1/aiobtclientapi/utils/torrent.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-26 15:23:33.618157 aiobtclientapi-1.1.1/aiobtclientapi.egg-info/
--rw-------   0 ich       (1000) ich       (1000)     1198 2023-05-26 15:23:33.000000 aiobtclientapi-1.1.1/aiobtclientapi.egg-info/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)     1021 2023-05-26 15:23:33.000000 aiobtclientapi-1.1.1/aiobtclientapi.egg-info/SOURCES.txt
--rw-------   0 ich       (1000) ich       (1000)        1 2023-05-26 15:23:33.000000 aiobtclientapi-1.1.1/aiobtclientapi.egg-info/dependency_links.txt
--rw-------   0 ich       (1000) ich       (1000)       57 2023-05-26 15:23:33.000000 aiobtclientapi-1.1.1/aiobtclientapi.egg-info/entry_points.txt
--rw-------   0 ich       (1000) ich       (1000)       60 2023-05-26 15:23:33.000000 aiobtclientapi-1.1.1/aiobtclientapi.egg-info/requires.txt
--rw-------   0 ich       (1000) ich       (1000)       15 2023-05-26 15:23:33.000000 aiobtclientapi-1.1.1/aiobtclientapi.egg-info/top_level.txt
--rw-------   0 ich       (1000) ich       (1000)       38 2023-05-26 15:23:33.626157 aiobtclientapi-1.1.1/setup.cfg
--rw-------   0 ich       (1000) ich       (1000)     1384 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.1/setup.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-06 11:45:17.088531 aiobtclientapi-1.1.2/
+-rw-------   0 ich       (1000) ich       (1000)    35149 2022-07-05 13:26:49.000000 aiobtclientapi-1.1.2/LICENSE
+-rw-------   0 ich       (1000) ich       (1000)     1198 2023-06-06 11:45:17.088531 aiobtclientapi-1.1.2/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)      592 2022-08-27 13:56:53.000000 aiobtclientapi-1.1.2/README.rst
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-06 11:45:17.088531 aiobtclientapi-1.1.2/aiobtclientapi/
+-rw-------   0 ich       (1000) ich       (1000)     1930 2023-06-06 11:44:07.000000 aiobtclientapi-1.1.2/aiobtclientapi/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     3976 2023-06-06 08:40:33.000000 aiobtclientapi-1.1.2/aiobtclientapi/cli.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-06 11:45:17.088531 aiobtclientapi-1.1.2/aiobtclientapi/clients/
+-rw-------   0 ich       (1000) ich       (1000)      208 2022-08-04 15:44:22.000000 aiobtclientapi-1.1.2/aiobtclientapi/clients/__init__.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-06 11:45:17.088531 aiobtclientapi-1.1.2/aiobtclientapi/clients/base/
+-rw-------   0 ich       (1000) ich       (1000)       25 2022-06-16 09:50:40.000000 aiobtclientapi-1.1.2/aiobtclientapi/clients/base/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)    18351 2023-06-06 11:16:48.000000 aiobtclientapi-1.1.2/aiobtclientapi/clients/base/api.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-06 11:45:17.088531 aiobtclientapi-1.1.2/aiobtclientapi/clients/deluge/
+-rw-------   0 ich       (1000) ich       (1000)       27 2022-07-26 09:47:43.000000 aiobtclientapi-1.1.2/aiobtclientapi/clients/deluge/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     5956 2023-06-06 11:17:03.000000 aiobtclientapi-1.1.2/aiobtclientapi/clients/deluge/api.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-06 11:45:17.088531 aiobtclientapi-1.1.2/aiobtclientapi/clients/qbittorrent/
+-rw-------   0 ich       (1000) ich       (1000)       32 2022-07-27 09:37:07.000000 aiobtclientapi-1.1.2/aiobtclientapi/clients/qbittorrent/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     5783 2023-06-06 11:44:07.000000 aiobtclientapi-1.1.2/aiobtclientapi/clients/qbittorrent/api.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-06 11:45:17.088531 aiobtclientapi-1.1.2/aiobtclientapi/clients/rtorrent/
+-rw-------   0 ich       (1000) ich       (1000)       29 2022-07-27 15:40:51.000000 aiobtclientapi-1.1.2/aiobtclientapi/clients/rtorrent/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     6521 2023-06-06 11:44:07.000000 aiobtclientapi-1.1.2/aiobtclientapi/clients/rtorrent/api.py
+-rw-------   0 ich       (1000) ich       (1000)     1558 2023-05-18 09:45:43.000000 aiobtclientapi-1.1.2/aiobtclientapi/clients/rtorrent/utils.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-06 11:45:17.088531 aiobtclientapi-1.1.2/aiobtclientapi/clients/transmission/
+-rw-------   0 ich       (1000) ich       (1000)       33 2022-07-30 14:17:58.000000 aiobtclientapi-1.1.2/aiobtclientapi/clients/transmission/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     6603 2023-06-06 11:16:48.000000 aiobtclientapi-1.1.2/aiobtclientapi/clients/transmission/api.py
+-rw-------   0 ich       (1000) ich       (1000)      418 2022-07-30 14:17:58.000000 aiobtclientapi-1.1.2/aiobtclientapi/clients/transmission/enums.py
+-rw-------   0 ich       (1000) ich       (1000)       69 2022-07-05 13:26:49.000000 aiobtclientapi-1.1.2/aiobtclientapi/constants.py
+-rw-------   0 ich       (1000) ich       (1000)     5466 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.2/aiobtclientapi/errors.py
+-rw-------   0 ich       (1000) ich       (1000)     7696 2022-08-05 11:03:47.000000 aiobtclientapi-1.1.2/aiobtclientapi/response.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-06 11:45:17.088531 aiobtclientapi-1.1.2/aiobtclientapi/utils/
+-rw-------   0 ich       (1000) ich       (1000)     6024 2023-06-06 11:16:48.000000 aiobtclientapi-1.1.2/aiobtclientapi/utils/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     6673 2023-06-06 11:16:48.000000 aiobtclientapi-1.1.2/aiobtclientapi/utils/monitor.py
+-rw-------   0 ich       (1000) ich       (1000)     2634 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.2/aiobtclientapi/utils/torrent.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-06 11:45:17.088531 aiobtclientapi-1.1.2/aiobtclientapi.egg-info/
+-rw-------   0 ich       (1000) ich       (1000)     1198 2023-06-06 11:45:17.000000 aiobtclientapi-1.1.2/aiobtclientapi.egg-info/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)     1021 2023-06-06 11:45:17.000000 aiobtclientapi-1.1.2/aiobtclientapi.egg-info/SOURCES.txt
+-rw-------   0 ich       (1000) ich       (1000)        1 2023-06-06 11:45:17.000000 aiobtclientapi-1.1.2/aiobtclientapi.egg-info/dependency_links.txt
+-rw-------   0 ich       (1000) ich       (1000)       57 2023-06-06 11:45:17.000000 aiobtclientapi-1.1.2/aiobtclientapi.egg-info/entry_points.txt
+-rw-------   0 ich       (1000) ich       (1000)       60 2023-06-06 11:45:17.000000 aiobtclientapi-1.1.2/aiobtclientapi.egg-info/requires.txt
+-rw-------   0 ich       (1000) ich       (1000)       15 2023-06-06 11:45:17.000000 aiobtclientapi-1.1.2/aiobtclientapi.egg-info/top_level.txt
+-rw-------   0 ich       (1000) ich       (1000)       38 2023-06-06 11:45:17.088531 aiobtclientapi-1.1.2/setup.cfg
+-rw-------   0 ich       (1000) ich       (1000)     1384 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.2/setup.py
```

### Comparing `aiobtclientapi-1.1.1/LICENSE` & `aiobtclientapi-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.1/PKG-INFO` & `aiobtclientapi-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiobtclientapi
-Version: 1.1.1
+Version: 1.1.2
 Summary: Asynchronous high-level communication with BitTorrent clients
 Home-page: https://codeberg.org/plotski/aiobtclientapi
 Author: plotski
 Author-email: plotski@example.org
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `aiobtclientapi-1.1.1/README.rst` & `aiobtclientapi-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.1/aiobtclientapi/__init__.py` & `aiobtclientapi-1.1.2/aiobtclientapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Asynchronous high-level communication with BitTorrent clients
 """
 
 __project_name__ = 'aiobtclientapi'
 __description__ = 'Asynchronous high-level communication with BitTorrent clients'
 __homepage__ = 'https://codeberg.org/plotski/aiobtclientapi'
-__version__ = '1.1.1'
+__version__ = '1.1.2'
 __author__ = 'plotski'
 __author_email__ = 'plotski@example.org'
 
 # isort:skip_file
 
 from .clients import APIBase
 from .clients import DelugeAPI, QbittorrentAPI, RtorrentAPI, TransmissionAPI
```

### Comparing `aiobtclientapi-1.1.1/aiobtclientapi/cli.py` & `aiobtclientapi-1.1.2/aiobtclientapi/cli.py`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.1/aiobtclientapi/clients/base/api.py` & `aiobtclientapi-1.1.2/aiobtclientapi/clients/base/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,18 +132,15 @@
             except asyncio.CancelledError:
                 if not taskinfo.detached:
                     raise
                 else:
                     _log.debug('%s: Ignoring cancelled background task: %r', self.label, taskinfo.task.get_name())
 
     monitor_interval = 0.1
-    """Seconds between requests when waiting for an RPC request to take effect"""
-
-    monitor_timeout = 3
-    """Maximum number of seconds before waiting for an RPC response fails"""
+    """Seconds between requests when waiting for an RPC call to take effect"""
 
     common_rpc_error_map = {}
     """
     Mapping of regular expressions to exceptions for all :meth:`call` calls
 
     See :meth:`aiobtclientrpc.RPCError.translate`.
     """
@@ -420,15 +417,15 @@
             await self._start_verifying(infohash)
 
             # Wait for command to take effect
             try:
                 await utils.Monitor(
                     call=utils.partial(self._torrent_is_verifying, infohash),
                     interval=0.1,
-                    timeout=1,
+                    timeout=1.0,
                 ).return_value_equals(True)
 
             except errors.TimeoutError:
                 # Verifying may never start because all files are missing or
                 # because the torrent is very small and verification was
                 # finished before Monitor's first call.
                 _log.debug('Verification finished immediately: %r', infohash)
@@ -512,9 +509,10 @@
 
     @abc.abstractmethod
     async def _get_verifying_progress(self, infohash):
         """
         Verifying progress in percent (0 to 100)
 
         After verification is done (:meth:`_torrent_is_verifying` returns
-        `False`), return the download progress of the wanted files in percent.
+        `False`), return the combined download progress of the wanted files in
+        percent.
         """
```

### Comparing `aiobtclientapi-1.1.1/aiobtclientapi/clients/deluge/api.py` & `aiobtclientapi-1.1.2/aiobtclientapi/clients/deluge/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -108,14 +108,16 @@
                     # Invalid torrent
                     r'decoding filedump failed': errors.InvalidTorrentError(torrent),
                     # Invalid magnet URI
                     r'invalid magnet info': errors.InvalidTorrentError(torrent),
                     r'non-hexadecimal number found': errors.InvalidTorrentError(torrent),
                 })
 
+    _timeout_start_torrent = 10.0
+
     async def _start_torrent(self, infohash):
         # Check current state
         state = await self._get_torrent_field(infohash, 'state')
         if state == 'Error':
             yield ('errors', 'Cannot start torrent in error state')
 
         elif state != 'Paused':
@@ -125,19 +127,21 @@
         else:
             await self.call('core.resume_torrent', infohash)
 
             # Wait for command to take effect
             await utils.Monitor(
                 call=utils.partial(self._get_torrent_field, infohash, 'state'),
                 interval=self.monitor_interval,
-                timeout=self.monitor_timeout,
+                timeout=self._timeout_start_torrent,
             ).return_value_equals('Paused', negate=True)
 
             yield ('started', infohash)
 
+    _timeout_stop_torrent = 10.0
+
     async def _stop_torrent(self, infohash):
         # Check current state
         state = await self._get_torrent_field(infohash, 'state')
         if state == 'Error':
             yield ('errors', 'Cannot stop torrent in error state')
 
         elif state == 'Paused':
@@ -147,25 +151,22 @@
         else:
             await self.call('core.pause_torrent', infohash)
 
             # Wait for command to take effect
             await utils.Monitor(
                 call=utils.partial(self._get_torrent_field, infohash, 'state'),
                 interval=self.monitor_interval,
-                timeout=self.monitor_timeout,
+                timeout=self._timeout_stop_torrent,
             ).return_value_equals('Paused')
 
             yield ('stopped', infohash)
 
     async def _start_verifying(self, infohash):
-        _log.debug('Start verifying: %r', infohash)
         await self.call('core.force_recheck', [infohash])
 
     async def _torrent_is_verifying(self, infohash):
         state = await self._get_torrent_field(infohash, 'state')
-        _log.debug('torrent state: %r', state)
-        return state == 'Checking'
+        return state in ('Checking', 'Queued')
 
     async def _get_verifying_progress(self, infohash):
         progress = await self._get_torrent_field(infohash, 'progress')
-        _log.debug('verifying progress: %r', progress)
         return progress
```

### Comparing `aiobtclientapi-1.1.1/aiobtclientapi/clients/qbittorrent/api.py` & `aiobtclientapi-1.1.2/aiobtclientapi/clients/qbittorrent/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,14 +69,16 @@
                     torrent_bytes,               # File content
                     'application/x-bittorrent',  # MIME type
                 )),
             )
 
         return rpc_args, infohash
 
+    _timeout_add_torrent = 10.0
+
     async def _add_torrent(self, torrent, *, location, stopped, verify):
         rpc_args, infohash = await self._make_add_torrent_args(
             torrent=torrent,
             location=location,
             stopped=stopped,
             verify=verify,
         )
@@ -100,60 +102,61 @@
                     raise errors.InvalidTorrentError(torrent)
 
             else:
                 # Wait for command to take effect
                 await utils.Monitor(
                     call=self.get_infohashes,
                     interval=self.monitor_interval,
-                    timeout=self.monitor_timeout,
+                    timeout=self._timeout_add_torrent,
                 ).return_value_contains(infohash)
                 yield ('added', infohash)
 
+    _timeout_start_torrent = 10.0
+
     async def _start_torrent(self, infohash):
         # Check current state
         state = await self._get_torrent_field(infohash, 'state')
         if not state.startswith('paused'):
             yield ('already_started', infohash)
             yield errors.TorrentAlreadyStarted(infohash)
         else:
             await self.call('torrents/resume', hashes=[infohash])
 
             # Wait for command to take effect
             await utils.Monitor(
                 call=utils.partial(self._get_torrent_field, infohash, 'state'),
                 interval=self.monitor_interval,
-                timeout=self.monitor_timeout,
+                timeout=self._timeout_start_torrent,
             ).return_value_contains('paused', negate=True)
 
             yield ('started', infohash)
 
+    _timeout_stop_torrent = 10.0
+
     async def _stop_torrent(self, infohash):
         # Check current state
         state = await self._get_torrent_field(infohash, 'state')
         if state.startswith('paused'):
             yield ('already_stopped', infohash)
             yield errors.TorrentAlreadyStopped(infohash)
         else:
             await self.call('torrents/pause', hashes=[infohash])
 
             # Wait for command to take effect
             await utils.Monitor(
                 call=utils.partial(self._get_torrent_field, infohash, 'state'),
                 interval=self.monitor_interval,
-                timeout=self.monitor_timeout,
+                timeout=self._timeout_stop_torrent,
             ).return_value_contains('paused')
 
             yield ('stopped', infohash)
 
     async def _start_verifying(self, infohash):
-        response = await self.call('torrents/recheck', hashes=[infohash])
-        _log.debug('started verifying: %r', response)
+        await self.call('torrents/recheck', hashes=[infohash])
 
     async def _torrent_is_verifying(self, infohash):
         state = await self._get_torrent_field(infohash, 'state')
-        _log.debug('torrent state: %r', state)
         return state.startswith('checking')
 
     async def _get_verifying_progress(self, infohash):
         progress = await self._get_torrent_field(infohash, 'progress')
-        _log.debug('verifying progress: %r', progress)
         return progress * 100
```

### Comparing `aiobtclientapi-1.1.1/aiobtclientapi/clients/rtorrent/api.py` & `aiobtclientapi-1.1.2/aiobtclientapi/clients/rtorrent/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,14 +76,16 @@
             infohash = utils.torrent.get_infohash(torrent_bytes)
 
         if location:
             rpc_args.append('d.directory.set="' + location.replace('"', r'\"') + '"')
 
         return rpc_method, rpc_args, infohash
 
+    _timeout_add_torrent = 10.0
+
     async def _add_torrent(self, torrent, *, location, stopped, verify):
         rpc_method, rpc_args, infohash = await self._make_add_torrent_args(
             torrent=torrent,
             location=location,
             stopped=stopped,
             verify=verify,
         )
@@ -96,26 +98,28 @@
         else:
             await self.call(rpc_method, *rpc_args)
 
             # Wait for command to take effect
             await utils.Monitor(
                 call=self.get_infohashes,
                 interval=self.monitor_interval,
-                timeout=self.monitor_timeout,
+                timeout=self._timeout_add_torrent,
             ).return_value_contains(infohash)
             yield ('added', infohash)
 
             # rtorrent always verifies. If we stop the torrent immediately,
             # it also stops verifying and we have to tell it again to
             # verify.
             if stopped:
                 yield await self.stop(infohash)
                 if verify:
                     yield await self.verify(infohash)
 
+    _timeout_start_torrent = 10.0
+
     async def _start_torrent(self, infohash):
         # Check current state
         state = await self._get_torrent_fields(infohash, 'd.is_open', 'd.is_active')
         if state == {'d.is_open': 1, 'd.is_active': 1}:
             yield ('already_started', infohash)
             yield errors.TorrentAlreadyStarted(infohash)
 
@@ -129,19 +133,21 @@
                 infohash=infohash,
             )
 
             # Wait for command to take effect
             await utils.Monitor(
                 call=utils.partial(self._get_torrent_fields, infohash, 'd.is_open', 'd.is_active'),
                 interval=self.monitor_interval,
-                timeout=self.monitor_timeout,
+                timeout=self._timeout_start_torrent,
             ).return_value_equals({'d.is_open': 1, 'd.is_active': 1})
 
             yield ('started', infohash)
 
+    _timeout_stop_torrent = 10.0
+
     async def _stop_torrent(self, infohash):
         # Check current state
         state = await self._get_torrent_fields(infohash, 'd.is_open', 'd.is_active')
         if state == {'d.is_open': 0, 'd.is_active': 0}:
             yield ('already_stopped', infohash)
             yield errors.TorrentAlreadyStopped(infohash)
 
@@ -155,29 +161,26 @@
                 infohash=infohash,
             )
 
             # Wait for command to take effect
             await utils.Monitor(
                 call=utils.partial(self._get_torrent_fields, infohash, 'd.is_open', 'd.is_active'),
                 interval=self.monitor_interval,
-                timeout=self.monitor_timeout,
+                timeout=self._timeout_stop_torrent,
             ).return_value_equals({'d.is_open': 0, 'd.is_active': 0})
 
             yield ('stopped', infohash)
 
     async def _start_verifying(self, infohash):
-        response = await self._translate_rpc_error(
+        await self._translate_rpc_error(
             self.call('d.check_hash', infohash),
             infohash=infohash,
         )
-        _log.debug('started verifying: %r', response)
 
     async def _torrent_is_verifying(self, infohash):
         hashing = await self._get_torrent_field(infohash, 'd.hashing')
-        _log.debug('torrent_is_verifying: %r', hashing)
         return hashing != 0
 
     async def _get_verifying_progress(self, infohash):
         fields = await self._get_torrent_fields(infohash, 'd.chunks_hashed', 'd.size_chunks')
         chunks_hashed, size_chunks = fields.values()
-        _log.debug('chunks hashed: %r / %r', chunks_hashed, size_chunks)
         return chunks_hashed / size_chunks * 100
```

### Comparing `aiobtclientapi-1.1.1/aiobtclientapi/clients/rtorrent/utils.py` & `aiobtclientapi-1.1.2/aiobtclientapi/clients/rtorrent/utils.py`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.1/aiobtclientapi/clients/transmission/api.py` & `aiobtclientapi-1.1.2/aiobtclientapi/clients/transmission/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,14 +83,15 @@
 
         try:
             result = await self.call('torrent-add', rpc_args)
 
         except aiobtclientrpc.RPCError as e:
             # Transmission 4.* sends
             # {"result": "duplicate torrent", "arguments": {"torrent-duplicate": ...}}
+            # This is fixed in 4.0.3: https://github.com/transmission/transmission/pull/5370
             if e.info and 'torrent-duplicate' in e.info:
                 infohash = e.info['torrent-duplicate']['hashString']
                 yield ('already_added', infohash)
                 yield errors.TorrentAlreadyAdded(infohash, name=torrent)
 
             else:
                 raise e.translate({
@@ -113,52 +114,55 @@
             elif 'torrent-added' in arguments:
                 infohash = arguments['torrent-added']['hashString']
                 yield ('added', arguments['torrent-added']['hashString'])
 
             else:
                 raise RuntimeError(f'Unexpected response: {result}')
 
+    _timeout_start_torrent = 10.0
+
     async def _start_torrent(self, infohash):
         # Check current state
         status = await self._get_torrent_field(infohash, 'status')
         if status != enums.TR_STATUS.STOPPED:
             yield ('already_started', infohash)
             yield errors.TorrentAlreadyStarted(infohash)
         else:
             await self.call('torrent-start', ids=[infohash])
 
             # Wait for command to take effect
             await utils.Monitor(
                 call=utils.partial(self._get_torrent_field, infohash, 'status'),
                 interval=self.monitor_interval,
-                timeout=self.monitor_timeout,
+                timeout=self._timeout_start_torrent,
             ).return_value_equals(enums.TR_STATUS.STOPPED, negate=True)
 
             yield ('started', infohash)
 
+    _timeout_stop_torrent = 10.0
+
     async def _stop_torrent(self, infohash):
         # Check current state
         status = await self._get_torrent_field(infohash, 'status')
         if status == enums.TR_STATUS.STOPPED:
             yield ('already_stopped', infohash)
             yield errors.TorrentAlreadyStopped(infohash)
         else:
             await self.call('torrent-stop', ids=[infohash])
 
             # Wait for command to take effect
             await utils.Monitor(
                 call=utils.partial(self._get_torrent_field, infohash, 'status'),
                 interval=self.monitor_interval,
-                timeout=self.monitor_timeout,
+                timeout=self._timeout_stop_torrent,
             ).return_value_equals(enums.TR_STATUS.STOPPED)
 
             yield ('stopped', infohash)
 
     async def _start_verifying(self, infohash):
-        _log.debug('Start verifying: %r', infohash)
         await self.call('torrent-verify', ids=[infohash])
 
     async def _torrent_is_verifying(self, infohash):
         status = await self._get_torrent_field(infohash, 'status')
         return status in (enums.TR_STATUS.CHECK, enums.TR_STATUS.CHECK_WAIT)
 
     async def _get_verifying_progress(self, infohash):
```

### Comparing `aiobtclientapi-1.1.1/aiobtclientapi/errors.py` & `aiobtclientapi-1.1.2/aiobtclientapi/errors.py`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.1/aiobtclientapi/response.py` & `aiobtclientapi-1.1.2/aiobtclientapi/response.py`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.1/aiobtclientapi/utils/__init__.py` & `aiobtclientapi-1.1.2/aiobtclientapi/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
 
     >>> async for coro in merge_async_generators(a, b, c):
     >>>     try:
     >>>         print('Good value:', await coro)
     >>>     except ValueError as e:
     >>>         print('Bad value:', e)
     """
-    aiters = [g.__aiter__() for g in generators]
+    aiters = (g.__aiter__() for g in generators)
     tasks = {
         asyncio.create_task(aiter.__anext__()): aiter
         for aiter in aiters
     }
 
     while tasks:
         done, pending_ = await asyncio.wait(
```

### Comparing `aiobtclientapi-1.1.1/aiobtclientapi/utils/monitor.py` & `aiobtclientapi-1.1.2/aiobtclientapi/utils/monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,14 @@
 
     async def _sleep(self):
         if isinstance(self._interval, (int, float)):
             await asyncio.sleep(self._interval)
         elif isinstance(self._interval, DynamicInterval):
             interval = await self._interval.next()
             await asyncio.sleep(interval)
-
         else:
             raise RuntimeError(f'Invalid interval: {self._interval!r}')
 
 
 class DynamicInterval:
     """
     Generate intervals from `min` to `max` depending on some ongoing operation
```

### Comparing `aiobtclientapi-1.1.1/aiobtclientapi/utils/torrent.py` & `aiobtclientapi-1.1.2/aiobtclientapi/utils/torrent.py`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.1/aiobtclientapi.egg-info/PKG-INFO` & `aiobtclientapi-1.1.2/aiobtclientapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiobtclientapi
-Version: 1.1.1
+Version: 1.1.2
 Summary: Asynchronous high-level communication with BitTorrent clients
 Home-page: https://codeberg.org/plotski/aiobtclientapi
 Author: plotski
 Author-email: plotski@example.org
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `aiobtclientapi-1.1.1/aiobtclientapi.egg-info/SOURCES.txt` & `aiobtclientapi-1.1.2/aiobtclientapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.1/setup.py` & `aiobtclientapi-1.1.2/setup.py`

 * *Files identical despite different names*

