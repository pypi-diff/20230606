# Comparing `tmp/slack-to-discord-1.1.3.tar.gz` & `tmp/slack-to-discord-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slack-to-discord-1.1.3.tar", last modified: Tue Mar 21 13:03:25 2023, max compression
+gzip compressed data, was "slack-to-discord-1.1.4.tar", last modified: Tue Jun  6 05:01:26 2023, max compression
```

## Comparing `slack-to-discord-1.1.3.tar` & `slack-to-discord-1.1.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 carey      (501) staff       (20)        0 2023-03-21 13:03:25.903400 slack-to-discord-1.1.3/
--rw-r--r--   0 carey      (501) staff       (20)     4430 2023-03-21 13:03:25.903060 slack-to-discord-1.1.3/PKG-INFO
--rw-r--r--   0 carey      (501) staff       (20)     3700 2023-02-16 01:48:06.000000 slack-to-discord-1.1.3/README.md
--rw-r--r--   0 carey      (501) staff       (20)       38 2023-03-21 13:03:25.903478 slack-to-discord-1.1.3/setup.cfg
--rw-r--r--   0 carey      (501) staff       (20)     1359 2023-03-21 12:59:36.000000 slack-to-discord-1.1.3/setup.py
-drwxr-xr-x   0 carey      (501) staff       (20)        0 2023-03-21 13:03:25.900009 slack-to-discord-1.1.3/slack_to_discord/
--rw-r--r--   0 carey      (501) staff       (20)      132 2022-10-19 02:44:12.000000 slack-to-discord-1.1.3/slack_to_discord/__init__.py
--rw-r--r--   0 carey      (501) staff       (20)     1738 2022-10-19 03:00:52.000000 slack-to-discord-1.1.3/slack_to_discord/__main__.py
--rw-r--r--   0 carey      (501) staff       (20)     9096 2023-02-16 03:38:45.000000 slack-to-discord-1.1.3/slack_to_discord/emojis.py
--rw-r--r--   0 carey      (501) staff       (20)     7188 2022-10-19 02:44:12.000000 slack-to-discord-1.1.3/slack_to_discord/http_stream.py
--rw-r--r--   0 carey      (501) staff       (20)    20595 2023-03-21 12:59:12.000000 slack-to-discord-1.1.3/slack_to_discord/importer.py
--rwxr-xr-x   0 carey      (501) staff       (20)      754 2023-02-16 03:02:54.000000 slack-to-discord-1.1.3/slack_to_discord/script.py
-drwxr-xr-x   0 carey      (501) staff       (20)        0 2023-03-21 13:03:25.902047 slack-to-discord-1.1.3/slack_to_discord.egg-info/
--rw-r--r--   0 carey      (501) staff       (20)     4430 2023-03-21 13:03:25.000000 slack-to-discord-1.1.3/slack_to_discord.egg-info/PKG-INFO
--rw-r--r--   0 carey      (501) staff       (20)      459 2023-03-21 13:03:25.000000 slack-to-discord-1.1.3/slack_to_discord.egg-info/SOURCES.txt
--rw-r--r--   0 carey      (501) staff       (20)        1 2023-03-21 13:03:25.000000 slack-to-discord-1.1.3/slack_to_discord.egg-info/dependency_links.txt
--rw-r--r--   0 carey      (501) staff       (20)       68 2023-03-21 13:03:25.000000 slack-to-discord-1.1.3/slack_to_discord.egg-info/entry_points.txt
--rw-r--r--   0 carey      (501) staff       (20)       49 2023-03-21 13:03:25.000000 slack-to-discord-1.1.3/slack_to_discord.egg-info/requires.txt
--rw-r--r--   0 carey      (501) staff       (20)       17 2023-03-21 13:03:25.000000 slack-to-discord-1.1.3/slack_to_discord.egg-info/top_level.txt
-drwxr-xr-x   0 carey      (501) staff       (20)        0 2023-03-21 13:03:25.902464 slack-to-discord-1.1.3/tests/
--rwxr-xr-x   0 carey      (501) staff       (20)     3186 2022-10-19 02:44:12.000000 slack-to-discord-1.1.3/tests/test_http_stream.py
+drwxr-xr-x   0 carey      (501) staff       (20)        0 2023-06-06 05:01:26.726762 slack-to-discord-1.1.4/
+-rw-r--r--   0 carey      (501) staff       (20)     4432 2023-06-06 05:01:26.726332 slack-to-discord-1.1.4/PKG-INFO
+-rw-r--r--   0 carey      (501) staff       (20)     3702 2023-05-14 04:31:17.000000 slack-to-discord-1.1.4/README.md
+-rw-r--r--   0 carey      (501) staff       (20)       38 2023-06-06 05:01:26.726879 slack-to-discord-1.1.4/setup.cfg
+-rw-r--r--   0 carey      (501) staff       (20)     1359 2023-06-06 04:51:11.000000 slack-to-discord-1.1.4/setup.py
+drwxr-xr-x   0 carey      (501) staff       (20)        0 2023-06-06 05:01:26.721921 slack-to-discord-1.1.4/slack_to_discord/
+-rw-r--r--   0 carey      (501) staff       (20)      132 2022-10-19 02:44:12.000000 slack-to-discord-1.1.4/slack_to_discord/__init__.py
+-rw-r--r--   0 carey      (501) staff       (20)     1756 2023-05-14 04:28:19.000000 slack-to-discord-1.1.4/slack_to_discord/__main__.py
+-rw-r--r--   0 carey      (501) staff       (20)     9096 2023-02-16 03:38:45.000000 slack-to-discord-1.1.4/slack_to_discord/emojis.py
+-rw-r--r--   0 carey      (501) staff       (20)     8435 2023-06-06 04:50:08.000000 slack-to-discord-1.1.4/slack_to_discord/http_stream.py
+-rw-r--r--   0 carey      (501) staff       (20)    20840 2023-06-06 04:50:08.000000 slack-to-discord-1.1.4/slack_to_discord/importer.py
+-rwxr-xr-x   0 carey      (501) staff       (20)      754 2023-02-16 03:02:54.000000 slack-to-discord-1.1.4/slack_to_discord/script.py
+drwxr-xr-x   0 carey      (501) staff       (20)        0 2023-06-06 05:01:26.724991 slack-to-discord-1.1.4/slack_to_discord.egg-info/
+-rw-r--r--   0 carey      (501) staff       (20)     4432 2023-06-06 05:01:26.000000 slack-to-discord-1.1.4/slack_to_discord.egg-info/PKG-INFO
+-rw-r--r--   0 carey      (501) staff       (20)      490 2023-06-06 05:01:26.000000 slack-to-discord-1.1.4/slack_to_discord.egg-info/SOURCES.txt
+-rw-r--r--   0 carey      (501) staff       (20)        1 2023-06-06 05:01:26.000000 slack-to-discord-1.1.4/slack_to_discord.egg-info/dependency_links.txt
+-rw-r--r--   0 carey      (501) staff       (20)       68 2023-06-06 05:01:26.000000 slack-to-discord-1.1.4/slack_to_discord.egg-info/entry_points.txt
+-rw-r--r--   0 carey      (501) staff       (20)       49 2023-06-06 05:01:26.000000 slack-to-discord-1.1.4/slack_to_discord.egg-info/requires.txt
+-rw-r--r--   0 carey      (501) staff       (20)       17 2023-06-06 05:01:26.000000 slack-to-discord-1.1.4/slack_to_discord.egg-info/top_level.txt
+drwxr-xr-x   0 carey      (501) staff       (20)        0 2023-06-06 05:01:26.725757 slack-to-discord-1.1.4/tests/
+-rw-r--r--   0 carey      (501) staff       (20)     2951 2023-06-06 04:50:08.000000 slack-to-discord-1.1.4/tests/test_bufferediterator.py
+-rwxr-xr-x   0 carey      (501) staff       (20)     3924 2023-06-06 04:50:08.000000 slack-to-discord-1.1.4/tests/test_http_stream.py
```

### Comparing `slack-to-discord-1.1.3/PKG-INFO` & `slack-to-discord-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-to-discord
-Version: 1.1.3
+Version: 1.1.4
 Summary: Extract data from a Slack export and import it into Discord
 Home-page: https://github.com/pR0Ps/slack-to-discord
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -54,15 +54,15 @@
 The program will read all messages from the Slack export and use a bot to post them in a Discord
 server. It's recommended to start with a completely clean server before importing history. As the
 script can only post messages, not rewrite history, any previous content will be buried by the
 imported data. It's also a good idea to make sure everything worked properly before inviting other
 users.
 
 Private channels (if you can manage to export them from Slack) will be created such that only the
-bot and guild administrators can access them. After the import completes and you invite your users,
+bot and server administrators can access them. After the import completes and you invite your users,
 you will need to manually change the roles/permissions to give everyone access to the correct
 channels.
 
 If something goes wrong with the import, you can delete all the created channels to quickly remove
 the history. At this point, you can either fix the issue yourself and re-run the export (please
 contribute your fixes back to the project!), or open an issue on the project.
 
@@ -76,13 +76,13 @@
     - Send Messages
     - Create Public Threads
     - Send Messages in Threads
     - Embed Links - to add reactions to messages (see 'Limitations' section)
     - Attach Files
     - Manage Messages - to pin messages [optional]
 3. Install `slack-to-discord` using `pip` (`pip install slack-to-discord`)
-4. Run `slack-to-discord --zipfile <slack export zip> --guild <guild name> --token <bot token>`
+4. Run `slack-to-discord --zipfile <slack export zip> --guild <server name> --token <bot token>`
    (check `slack-to-discord --help` for other options).
 5. Wait. The program will exit once the import is finished. Due to Discord rate limits, the import
    process will take a while (speed was roughly 50 messages/min for me)
 6. Inspect the imported history.
 7. Invite your users.
```

### Comparing `slack-to-discord-1.1.3/README.md` & `slack-to-discord-1.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 The program will read all messages from the Slack export and use a bot to post them in a Discord
 server. It's recommended to start with a completely clean server before importing history. As the
 script can only post messages, not rewrite history, any previous content will be buried by the
 imported data. It's also a good idea to make sure everything worked properly before inviting other
 users.
 
 Private channels (if you can manage to export them from Slack) will be created such that only the
-bot and guild administrators can access them. After the import completes and you invite your users,
+bot and server administrators can access them. After the import completes and you invite your users,
 you will need to manually change the roles/permissions to give everyone access to the correct
 channels.
 
 If something goes wrong with the import, you can delete all the created channels to quickly remove
 the history. At this point, you can either fix the issue yourself and re-run the export (please
 contribute your fixes back to the project!), or open an issue on the project.
 
@@ -58,13 +58,13 @@
     - Send Messages
     - Create Public Threads
     - Send Messages in Threads
     - Embed Links - to add reactions to messages (see 'Limitations' section)
     - Attach Files
     - Manage Messages - to pin messages [optional]
 3. Install `slack-to-discord` using `pip` (`pip install slack-to-discord`)
-4. Run `slack-to-discord --zipfile <slack export zip> --guild <guild name> --token <bot token>`
+4. Run `slack-to-discord --zipfile <slack export zip> --guild <server name> --token <bot token>`
    (check `slack-to-discord --help` for other options).
 5. Wait. The program will exit once the import is finished. Due to Discord rate limits, the import
    process will take a while (speed was roughly 50 messages/min for me)
 6. Inspect the imported history.
 7. Invite your users.
```

### Comparing `slack-to-discord-1.1.3/setup.py` & `slack-to-discord-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         long_description = f.read()
 except Exception:
     long_description=None
 
 
 setup(
     name="slack-to-discord",
-    version="1.1.3",
+    version="1.1.4",
     description="Extract data from a Slack export and import it into Discord",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pR0Ps/slack-to-discord",
     license="GPLv3",
     python_requires=">=3.6.0",
     classifiers=[
```

### Comparing `slack-to-discord-1.1.3/slack_to_discord/__main__.py` & `slack-to-discord-1.1.4/slack_to_discord/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 def main():
     parser = argparse.ArgumentParser(
         description="Import Slack chat history into Discord"
     )
     parser.add_argument("-z", "--zipfile", help="The Slack export zip file", required=True)
     parser.add_argument("-t", "--token", help="The Discord bot token", required=True)
-    parser.add_argument("-g", "--guild", help="The Discord Guild to import history into", required=True)
+    parser.add_argument("-g", "--guild", help="The Discord Guild (ie. server name) to import history into", required=True)
     parser.add_argument("-c", "--channels", help="When specified, will only import the provided channels. Do not include the '#'s (ex: 'general', not '#general')", nargs="*")
     parser.add_argument("-s", "--start", help="The date to start importing from (YYYY-MM-DD)", required=False, default=None)
     parser.add_argument("-e", "--end", help="The date to end importing at (YYYY-MM-DD)", required=False, default=None)
     parser.add_argument("-p", "--all-private", help="Import all channels as private channels in Discord", action="store_true", default=False)
     parser.add_argument("-r", "--real-names", help="Use real names from Slack instead of usernames", action="store_true", default=False)
     parser.add_argument("-v", "--verbose", help="Show more verbose logs", action="store_true")
     args = parser.parse_args()
```

### Comparing `slack-to-discord-1.1.3/slack_to_discord/emojis.py` & `slack-to-discord-1.1.4/slack_to_discord/emojis.py`

 * *Files identical despite different names*

### Comparing `slack-to-discord-1.1.3/slack_to_discord/http_stream.py` & `slack-to-discord-1.1.4/slack_to_discord/http_stream.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,122 +1,107 @@
 #!/usr/bin/env python
 
 import io
+from tempfile import SpooledTemporaryFile
 
 import urllib3
 
 
-class IterBuffer:
-    """Provides a buffered readable interface for an iterator"""
+DEFAULT_CHUNK_SIZE = 64 * 1024  # 64K
+"""Chunk size to use to download files"""
 
-    def __init__(self, iterator=None):
-        self.reset(iterator)
+DEFAULT_BUFFER_SIZE = 10 * 1024 * 1024  # 10M
+"""How much file data to store in memory before dumping it to disk instead
 
-    def __len__(self):
-        """How much data is available to be read from the buffer"""
-        return len(self._data) - self._pos
+(only used if the remote server doesn't support range requests)
+"""
 
-    def _buff_read(self, size=-1):
-        l = len(self)
-        if size < 0 or size > l:
-            size = l
-        if size < 1:
-            return b""
 
-        ret = bytes(self._data if size == l else self._data[self._pos:self._pos+size])
-        self._pos += size
-        return ret
-
-    def _buff_fill(self, size, read1=False):
-        """Ensure enough data is in the buffer"""
-        if size == 0 or self._iter is None:
-            return
-
-        cur_size = len(self)
-        if size > 0 and cur_size >= size:
-            # have the data, don't need to read anything
-            return
-
-        if self._pos > 0:
-            self._data = self._data[self._pos:]
-            self._pos = 0
-
-        for x in self._iter:
-            self._data += x
-            cur_size += len(x)
-            if read1 or (size > 0 and cur_size >= size):
-                break
-        else:
-            self._iter = None
+class IteratorReader(io.RawIOBase):
+    """Provides an io.RawIOBase-compatible interface for an iterator"""
 
-    def relseek(self, num):
-        """Relative seek within the buffer
+    def __init__(self, iterator):
+        self._iter = iter(iterator)
+        self._extra = bytearray()
+        self._total = 0
 
-        Given the number of bytes to seek within the buffer (-/+), get as close
-        as possible and return the actual seek amount
-        """
-        actual = max(-self._pos, min(num, len(self)))
-        self._pos += actual
-        return actual
+    def readable(self):
+        return True
 
-    def read(self, size=-1):
-        """Read and return up to `size` bytes.
+    def tell(self):
+        """Return the total number of bytes that have been read so far"""
+        if self.closed:
+            raise ValueError("I/O operation on a closed {}".format(self.__class__.__name__))
+        return self._total - len(self._extra)
 
-        If the argument is omitted or negative, data is read and returned until
-        EOF is reached. An empty bytes object is returned if the stream is
-        already at EOF
-        """
-        self._buff_fill(size)
-        return self._buff_read(size)
+    def readinto(self, b):
+        """Read bytes into a pre-allocated bytes-like object b
 
-    def read1(self, size=-1):
-        """Read and return up to `size` bytes with at most one call to the iterator"""
-        self._buff_fill(size, read1=True)
-        return self._buff_read(size)
-
-    def reset(self, iterator=None):
-        """Zero out the current buffer and assign a new iterator to buffer bytes from"""
-        self._iter = iterator
-        self._data = bytearray()
-        self._pos = 0
+        Returns the number of bytes read, 0 indicates EOF
+        """
+        num = len(b)
+        if self._iter is not None:
+            while len(self._extra) < num:
+                try:
+                    new = next(self._iter)
+                except StopIteration:
+                    self._iter = None
+                    break
+                else:
+                    self._total += len(new)
+                    self._extra += new
+
+        ret, self._extra = self._extra[:num], self._extra[num:]
+
+        lret = len(ret)
+        b[:lret] = ret
+        return lret
+
+
+class BufferedIteratorReader(io.BufferedReader):
+    """Provides a io.BufferedReader interface over an IteratorReader"""
+
+    def __init__(self, iterator, buffer_size=io.DEFAULT_BUFFER_SIZE):
+        """Create a new buffered iterator reader using the given iterator"""
+        super().__init__(raw=IteratorReader(iterator), buffer_size=buffer_size)
 
 
 class SeekableHTTPStream(io.BufferedIOBase):
     """Make the contents at a URL addressable via a seekable file-like object.
 
     Seeking to arbitrary offsets is handled using HTTP range requests.
 
     Notes:
      - The server must respond with an `Accept-Ranges: bytes` header for seeking to be supported.
      - Using `__len__` or `io.SEEK_END` to seek requires the server to have sent a valid `Content-Length` header.
     """
 
-    def __init__(self, url, chunk_size=64*1024):
+    def __init__(self, url, chunk_size=DEFAULT_CHUNK_SIZE):
         self._pos = 0
         self._url = url
         self._pool = urllib3.PoolManager()
         self._resp = None
-        self._buff = IterBuffer()
+        self._buff = None
 
         self._chunk_size = chunk_size
         self._do_request()
 
         try:
-            self._content_length = int(self._resp.getheader("Content-Length"))
+            self._content_length = int(self._resp.headers.get("Content-Length"))
         except TypeError:
             self._content_length = None
 
-        self._seekable = self._resp.getheader("Accept-Ranges", "").lower() == "bytes"
+        self._seekable = self._resp.headers.get("Accept-Ranges", "").lower() == "bytes"
 
     def _reset(self):
         if self._resp:
             # release the connection back into the pool
             self._resp.release_conn()
         self._resp = None
-        self._buff.reset()
+        self._buff = None
 
     def _do_request(self, start=0):
         self._reset()
 
         headers = {}
         if start > 0:
             headers["Range"] = "bytes={}-".format(start)
@@ -133,15 +118,18 @@
         elif resp.status not in (200, 206):
             self._reset()
             raise urllib3.exceptions.HTTPError(
                 "Bad status code: {}".format(resp.status)
             )
         else:
             self._resp = resp
-            self._buff.reset(resp.stream(amt=self._chunk_size, decode_content=True))
+            self._buff = BufferedIteratorReader(
+                resp.stream(amt=self._chunk_size, decode_content=True),
+                buffer_size=self._chunk_size
+            )
 
     def __len__(self):
         if self._content_length is None:
             raise TypeError("The length of this {} is unknown".format(self.__class__.__name__))
         return self._content_length
 
     def close(self):
@@ -160,73 +148,122 @@
     def tell(self):
         return self._pos
 
     def detach(self):
         raise io.UnsupportedOperation()
 
     def read(self, size=-1):
-        ret = self._buff.read(size)
-        self._pos += len(ret)
-        return ret
-
-    def read1(self, size=-1):
-        ret = self._buff.read1(size)
-        self._pos += len(ret)
-        return ret
-
-    def readinto(self, b):
-        data = self.read(len(b))
-        l = len(data)
-        b[:l] = data
-        return l
-
-    def readinto1(self, b):
-        data = self.read1(len(b))
-        l = len(data)
-        b[:l] = data
-        return l
-
-    def seek(self, offset, whence=io.SEEK_SET):
-        if not self.seekable():
-            raise io.UnsupportedOperation(f"URL '{self._url}' does not support range requests")
+        if self._buff is None:
+            return b""
+        data = self._buff.read(size)
+        self._pos += len(data)
+        return data
 
+    def _calc_new_pos(self, offset, whence):
         if whence == io.SEEK_SET:
             new_pos = offset
         elif whence == io.SEEK_CUR:
-            new_pos = self._pos + offset
+            new_pos = self.tell() + offset
         elif whence == io.SEEK_END:
             if self._content_length is None:
                 raise io.UnsupportedOperation("can't do end-relative seeks without knowing the length")
             new_pos = len(self) + offset
         else:
             raise ValueError("Invalid whence: {}".format(whence))
 
         if self._content_length is not None:
             new_pos = min(new_pos, self._content_length)
-        new_pos = max(0, new_pos)
 
+        return max(0, new_pos)
+
+    def seek(self, offset, whence=io.SEEK_SET):
+        if not self.seekable():
+            raise io.UnsupportedOperation(f"URL '{self._url}' does not support range requests")
+
+        new_pos = self._calc_new_pos(offset, whence)
         if new_pos == self._content_length:
             # seeking to end - no more data
             self._reset()
-        else:
-            # Figure out how far off we are and seek within the buffered data
-            # to get as close as possible to the target offset
+        elif new_pos != self._pos:
+            # Figure out how far off we are and how to deal with it
             pos_diff = new_pos - self._pos
-            pos_diff -= self._buff.relseek(pos_diff)
 
-            if pos_diff == 0:
-                # seeked to an already-buffered offset - nothing else to do
-                pass
-            elif 0 < pos_diff < self._chunk_size * 2:
+            if 0 < pos_diff < self._chunk_size * 2:
                 # seeking forwards and we're close enough (within 2 iterations of
                 # the current request) that it makes sense to avoid doing another
                 # fresh HTTP request - read the data until we get to the target
                 # offset
                 self.read(pos_diff)
             else:
                 # seekable stream and we're before the current position or far
                 # enough ahead that we don't want to read everything up to it - do
                 # a range request starting at the requested offset
                 self._do_request(new_pos)
 
         self._pos = new_pos
         return self._pos
+
+
+class CachedSeekableHTTPStream(SeekableHTTPStream):
+    """An adapter for SeekableHTTPStream that ensures that the stream is always seekable
+
+    It does this by only making a single request to the start of the file and
+    caching the contents to memory/a tempfile as it's downloaded.
+    Seeking forwards will stream more data, seeking backwards will read
+    previously-downloaded data out of the cache.
+    """
+
+    def __init__(self, *args, max_buffer_size=DEFAULT_BUFFER_SIZE, force_cache=False, **kwargs):
+        super().__init__(*args, **kwargs)
+        if not force_cache and super().seekable():
+            self._cache = None
+        else:
+            self._cache = SpooledTemporaryFile(max_size=max_buffer_size)
+            self._cache_size = 0
+
+    def close(self):
+        if self._cache:
+            self._cache.close()
+        super().close()
+
+    def seekable(self):
+        return True
+
+    def tell(self):
+        if self._cache is None:
+            return super().tell()
+        else:
+            return self._cache.tell()
+
+    def read(self, size=-1):
+        if self._cache is None:
+            return super().read(size)
+
+        buff = bytearray()
+
+        buffered = min(size, self._cache_size - self.tell())
+        if buffered:
+            # get data from the buffer
+            buff += self._cache.read(buffered)
+            if buffered > 0:
+                size -= buffered
+        if size:
+            # get more data from the stream
+            new = super().read(size)
+            buff += new
+            self._cache_size += self._cache.write(new)
+
+        return bytes(buff)
+
+    def seek(self, offset, whence=io.SEEK_SET):
+        if self._cache is None:
+            return super().seek(offset, whence=whence)
+
+        new_pos = self._calc_new_pos(offset, whence)
+        pos_diff = new_pos - self.tell()
+
+        if pos_diff > 0:
+            self.read(pos_diff)
+        else:
+            self._cache.seek(new_pos)
+
+        return self.tell()
```

### Comparing `slack-to-discord-1.1.3/slack_to_discord/importer.py` & `slack-to-discord-1.1.4/slack_to_discord/importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from zipfile import ZipFile
 from datetime import datetime
 from urllib.parse import urlparse
 
 import discord
 from discord.errors import Forbidden
 
-from slack_to_discord.http_stream import SeekableHTTPStream
+from slack_to_discord.http_stream import CachedSeekableHTTPStream
 from slack_to_discord.emojis import GLOBAL_EMOJI_MAP
 
 
 # Discord size limits
 MAX_MESSAGE_SIZE = 2000
 MAX_THREADNAME_SIZE = 100
 
@@ -29,15 +29,15 @@
 DATE_FORMAT = "%Y-%m-%d"
 TIME_FORMAT = "%H:%M"
 
 # Formatting options for messages
 MSG_FORMAT = "`{time}` {text}"
 BACKUP_THREAD_NAME = "{date} {time}"  # used when the message to create the thread from has no text
 ATTACHMENT_TITLE_TEXT = "<*uploaded a file*> {title}"
-ATTACHMENT_ERROR_APPEND = "\n<file thumbnail used due to size restrictions. See original at <{url}>>"
+ATTACHMENT_ERROR_APPEND = "\n<original file not uploaded due to size restrictions. See original at <{url}>>"
 
 # Create a separator between dates? (None for no)
 DATE_SEPARATOR = "`{:-^30}`"
 
 MENTION_RE = re.compile(r"<([@!#])([^>]*?)(?:\|([^>]*?))?>")
 LINK_RE = re.compile(r"<((?:https?|mailto|tel):[A-Za-z0-9_\+\.\-\/\?\,\=\#\:\@\(\)]+)\|([^>]+)>")
 EMOJI_RE = re.compile(r":([^ /<>:]+):(?::skin-tone-(\d):)?")
@@ -106,20 +106,23 @@
                     yield x["name"], topic(x), pins(x), is_private
 
 
 def slack_filedata(f):
     # Make sure the filename has the correct extension
     # Not fixing these issues can cause pictures to not be shown
     name, *ext = (f.get("name") or "unnamed").rsplit(".", 1)
-
     ext = ext[0] if ext else ""
-    ft = f.get("filetype") or ""
-    if ext.lower() == ft.lower():
-        # extension is already correct, don't fix it
-        ft = None
+
+    # only attempt to fix filenames for things that are displayed inline
+    ft = None
+    if f.get("mimetype", "").split("/")[0].lower() in ("image", "video"):
+        ft = f.get("filetype") or ""
+        if ext.lower() == ft.lower():
+            # extension is already correct, don't fix it
+            ft = None
 
     newname = ".".join(x for x in (name or "unknown", ext, ft) if x)
 
     # Make a list of thumbnails for this file in case the original can't be posted
     thumbs = [
         f[t]
         for t in sorted(
@@ -345,19 +348,19 @@
             # Trying thumbnails - get the filename from Slack (it has the correct extension)
             filename = urlparse(url).path.rsplit("/", 1)[-1]
         else:
             filename = fd["name"]
 
         try:
             f = discord.File(
-                fp=SeekableHTTPStream(url),
+                fp=CachedSeekableHTTPStream(url),
                 filename=filename
             )
         except Exception:
-            pass
+            __log__.debug("Failed to upload file", exc_info=True)
         else:
             yield {
                 **data,
                 "file": f
             }
 
         # The original URL failed - trying thumbnails
```

### Comparing `slack-to-discord-1.1.3/slack_to_discord/script.py` & `slack-to-discord-1.1.4/slack_to_discord/script.py`

 * *Files identical despite different names*

### Comparing `slack-to-discord-1.1.3/slack_to_discord.egg-info/PKG-INFO` & `slack-to-discord-1.1.4/slack_to_discord.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-to-discord
-Version: 1.1.3
+Version: 1.1.4
 Summary: Extract data from a Slack export and import it into Discord
 Home-page: https://github.com/pR0Ps/slack-to-discord
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -54,15 +54,15 @@
 The program will read all messages from the Slack export and use a bot to post them in a Discord
 server. It's recommended to start with a completely clean server before importing history. As the
 script can only post messages, not rewrite history, any previous content will be buried by the
 imported data. It's also a good idea to make sure everything worked properly before inviting other
 users.
 
 Private channels (if you can manage to export them from Slack) will be created such that only the
-bot and guild administrators can access them. After the import completes and you invite your users,
+bot and server administrators can access them. After the import completes and you invite your users,
 you will need to manually change the roles/permissions to give everyone access to the correct
 channels.
 
 If something goes wrong with the import, you can delete all the created channels to quickly remove
 the history. At this point, you can either fix the issue yourself and re-run the export (please
 contribute your fixes back to the project!), or open an issue on the project.
 
@@ -76,13 +76,13 @@
     - Send Messages
     - Create Public Threads
     - Send Messages in Threads
     - Embed Links - to add reactions to messages (see 'Limitations' section)
     - Attach Files
     - Manage Messages - to pin messages [optional]
 3. Install `slack-to-discord` using `pip` (`pip install slack-to-discord`)
-4. Run `slack-to-discord --zipfile <slack export zip> --guild <guild name> --token <bot token>`
+4. Run `slack-to-discord --zipfile <slack export zip> --guild <server name> --token <bot token>`
    (check `slack-to-discord --help` for other options).
 5. Wait. The program will exit once the import is finished. Due to Discord rate limits, the import
    process will take a while (speed was roughly 50 messages/min for me)
 6. Inspect the imported history.
 7. Invite your users.
```

### Comparing `slack-to-discord-1.1.3/tests/test_http_stream.py` & `slack-to-discord-1.1.4/tests/test_http_stream.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #!/usr/bin/env python
 
+import functools
 from http import HTTPStatus
 import http.server
 import io
 import threading
 
 import pytest
 
-from slack_to_discord import SeekableHTTPStream
+from slack_to_discord.http_stream import SeekableHTTPStream, CachedSeekableHTTPStream
 
 
 RESP_SIZE = 100
 
 
 # TODO: make tests for non-seekable and/or unknown length responses
 
 def gen_bytes(s, e):
     return b"".join(bytes([x]) for x in range(s, e))
 
-
 class HTTPRangeRequestHandler(http.server.SimpleHTTPRequestHandler):
     def do_GET(self):
         range_ = self.headers.get("Range")
         start, end = 0, RESP_SIZE
         if range_ is not None:
             _, r = range_.split("bytes=", 1)
             s, e = r.split("-", 1)
@@ -55,16 +55,25 @@
     try:
         yield f"http://127.0.0.1:{s.server_port}"
     finally:
         s.shutdown()
         thread.join()
 
 
-def test_server(mockserver):
-    s = SeekableHTTPStream(mockserver, chunk_size=10)
+@pytest.mark.parametrize("stream_cls", [
+    SeekableHTTPStream,
+    CachedSeekableHTTPStream,
+    functools.partial(CachedSeekableHTTPStream, max_buffer_size=50, force_cache=True)
+])
+def test_http_stream(mockserver, stream_cls):
+    s = stream_cls(mockserver, chunk_size=10)
+
+    assert s.readable()
+    assert s.seekable()
+    assert not s.writable()
 
     assert len(s) == RESP_SIZE
 
     # test reading chunks
     assert s.read(10) == gen_bytes(0, 10)
     assert s.read(10) == gen_bytes(10, 20)
     assert s.read(10) == gen_bytes(20, 30)
@@ -76,36 +85,52 @@
     assert s.seek(-10, io.SEEK_END) == RESP_SIZE - 10
     assert s.seek(5, io.SEEK_SET) == 5
 
     # test reading across chunks
     assert s.read(10) == gen_bytes(5, 15)
     assert s.tell() == 15
 
-    # test seeking bck from current pos and getting data we just got just reads
+    # test seeking back from current pos and getting data we just got just reads
     # it from the buffer
     assert s.seek(-10, io.SEEK_CUR) == 5
     assert s.read(10) == gen_bytes(5, 15)
 
     # test seeking past the end stops at the end and returns no data
     assert s.seek(RESP_SIZE * 2) == RESP_SIZE
     assert s.read() == b""
 
     # test read with no args gets everything
     assert s.seek(50) == 50
     assert s.read() == gen_bytes(50, 100)
 
-    # test read1 only reads at most 1 chunk from the stream
-    assert s.seek(0) == 0
-    assert s.read(5) == gen_bytes(0, 5)
-    assert s.read1() == gen_bytes(5, 20) # 5 in the buff + 1 read of 10 bytes
-
     # test readinto
     b = bytearray(20)
     assert s.seek(5) == 5
     assert s.readinto(b) == 20
     assert s.tell() == 25
     assert bytes(b) == gen_bytes(5, 25)
 
-    # test readinto1 (partial read)
-    b = bytearray(20)
-    assert s.readinto1(b) == 15
-    assert bytes(b) == gen_bytes(25, 40) + bytes(5)
+
+def test_cached_http_stream_read_rolls(mockserver):
+    s = CachedSeekableHTTPStream(mockserver, chunk_size=10, max_buffer_size=50, force_cache=True)
+    assert s._cache
+
+    assert s.read(50) == gen_bytes(0, 50)
+    assert not s._cache._rolled
+
+    assert s.read(1) == gen_bytes(50, 51)
+    assert s._cache._rolled
+
+    assert s.seek(0) == 0
+    assert s.read() == gen_bytes(0, 100)
+
+def test_cached_http_stream_seek_rolls(mockserver):
+    s = CachedSeekableHTTPStream(mockserver, chunk_size=10, max_buffer_size=50, force_cache=True)
+    assert s._cache
+
+    assert not s._cache._rolled
+    assert s.seek(0, io.SEEK_END) == RESP_SIZE
+    assert s._cache._rolled
+    assert s.read(1) == b""
+
+    assert s.seek(0) == 0
+    assert s.read() == gen_bytes(0, 100)
```

