# Comparing `tmp/m3u_parser-0.2.1.tar.gz` & `tmp/m3u_parser-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m3u_parser-0.2.1.tar", last modified: Mon Jun  5 07:30:53 2023, max compression
+gzip compressed data, was "m3u_parser-0.3.0.tar", last modified: Tue Jun  6 08:54:35 2023, max compression
```

## Comparing `m3u_parser-0.2.1.tar` & `m3u_parser-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 blokchainaholic   (501) staff       (20)        0 2023-06-05 07:30:53.567622 m3u_parser-0.2.1/
--rw-r--r--   0 blokchainaholic   (501) staff       (20)     1056 2023-05-27 16:53:27.000000 m3u_parser-0.2.1/LICENSE.txt
--rw-r--r--   0 blokchainaholic   (501) staff       (20)     7238 2023-06-05 07:30:53.567489 m3u_parser-0.2.1/PKG-INFO
--rw-r--r--   0 blokchainaholic   (501) staff       (20)     6562 2023-06-05 07:16:33.000000 m3u_parser-0.2.1/README.md
-drwxr-xr-x   0 blokchainaholic   (501) staff       (20)        0 2023-06-05 07:30:53.566439 m3u_parser-0.2.1/m3u_parser/
--rw-r--r--   0 blokchainaholic   (501) staff       (20)       57 2023-06-05 07:16:25.000000 m3u_parser-0.2.1/m3u_parser/__init__.py
--rw-r--r--   0 blokchainaholic   (501) staff       (20)     6018 2023-06-05 07:14:16.000000 m3u_parser-0.2.1/m3u_parser/helper.py
--rwxr-xr-x   0 blokchainaholic   (501) staff       (20)    19283 2023-06-05 07:23:26.000000 m3u_parser-0.2.1/m3u_parser/m3u_parser.py
-drwxr-xr-x   0 blokchainaholic   (501) staff       (20)        0 2023-06-05 07:30:53.567253 m3u_parser-0.2.1/m3u_parser.egg-info/
--rw-r--r--   0 blokchainaholic   (501) staff       (20)     7238 2023-06-05 07:30:53.000000 m3u_parser-0.2.1/m3u_parser.egg-info/PKG-INFO
--rw-r--r--   0 blokchainaholic   (501) staff       (20)      283 2023-06-05 07:30:53.000000 m3u_parser-0.2.1/m3u_parser.egg-info/SOURCES.txt
--rw-r--r--   0 blokchainaholic   (501) staff       (20)        1 2023-06-05 07:30:53.000000 m3u_parser-0.2.1/m3u_parser.egg-info/dependency_links.txt
--rw-r--r--   0 blokchainaholic   (501) staff       (20)       35 2023-06-05 07:30:53.000000 m3u_parser-0.2.1/m3u_parser.egg-info/requires.txt
--rw-r--r--   0 blokchainaholic   (501) staff       (20)       11 2023-06-05 07:30:53.000000 m3u_parser-0.2.1/m3u_parser.egg-info/top_level.txt
--rw-r--r--   0 blokchainaholic   (501) staff       (20)      297 2023-05-27 16:53:27.000000 m3u_parser-0.2.1/pyproject.toml
--rw-r--r--   0 blokchainaholic   (501) staff       (20)       38 2023-06-05 07:30:53.567669 m3u_parser-0.2.1/setup.cfg
--rw-r--r--   0 blokchainaholic   (501) staff       (20)     3129 2023-06-05 07:30:37.000000 m3u_parser-0.2.1/setup.py
+drwxr-xr-x   0 blokchainaholic   (501) staff       (20)        0 2023-06-06 08:54:35.225995 m3u_parser-0.3.0/
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)     1056 2023-05-27 16:53:27.000000 m3u_parser-0.3.0/LICENSE.txt
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)     8453 2023-06-06 08:54:35.225797 m3u_parser-0.3.0/PKG-INFO
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)     7777 2023-06-06 08:53:09.000000 m3u_parser-0.3.0/README.md
+drwxr-xr-x   0 blokchainaholic   (501) staff       (20)        0 2023-06-06 08:54:35.224789 m3u_parser-0.3.0/m3u_parser/
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)       57 2023-06-06 08:52:37.000000 m3u_parser-0.3.0/m3u_parser/__init__.py
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)     6018 2023-06-06 02:17:42.000000 m3u_parser-0.3.0/m3u_parser/helper.py
+-rwxr-xr-x   0 blokchainaholic   (501) staff       (20)    24399 2023-06-06 08:40:57.000000 m3u_parser-0.3.0/m3u_parser/m3u_parser.py
+drwxr-xr-x   0 blokchainaholic   (501) staff       (20)        0 2023-06-06 08:54:35.225575 m3u_parser-0.3.0/m3u_parser.egg-info/
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)     8453 2023-06-06 08:54:35.000000 m3u_parser-0.3.0/m3u_parser.egg-info/PKG-INFO
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)      283 2023-06-06 08:54:35.000000 m3u_parser-0.3.0/m3u_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)        1 2023-06-06 08:54:35.000000 m3u_parser-0.3.0/m3u_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)       35 2023-06-06 08:54:35.000000 m3u_parser-0.3.0/m3u_parser.egg-info/requires.txt
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)       11 2023-06-06 08:54:35.000000 m3u_parser-0.3.0/m3u_parser.egg-info/top_level.txt
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)      297 2023-05-27 16:53:27.000000 m3u_parser-0.3.0/pyproject.toml
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)       38 2023-06-06 08:54:35.226042 m3u_parser-0.3.0/setup.cfg
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)     3129 2023-06-06 08:53:11.000000 m3u_parser-0.3.0/setup.py
```

### Comparing `m3u_parser-0.2.1/LICENSE.txt` & `m3u_parser-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `m3u_parser-0.2.1/PKG-INFO` & `m3u_parser-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,10 @@
-Metadata-Version: 2.1
-Name: m3u_parser
-Version: 0.2.1
-Summary: A useful package for parsing m3u files or links
-Home-page: https://github.com/pawanpaudel93/m3u_parser
-Author: Pawan Paudel
-Author-email: pawanpaudel93@gmail.com
-License: ISC
-Classifier: License :: OSI Approved :: ISC License (ISCL)
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.0
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-
 # m3u_parser
 
-![version](https://img.shields.io/badge/version-0.2.1-blue.svg?cacheSeconds=2592000)
+![version](https://img.shields.io/badge/version-0.3.0-blue.svg?cacheSeconds=2592000)
 
 A Python package for parsing m3u files and extracting streams information. The package allows you to convert the parsed information into JSON or CSV format and provides various filtering and sorting options.
 
 ## Install
 
 Using pip,
 
@@ -93,14 +73,42 @@
 - `check_live` (optional): Set to `True` to check if the stream links are working or not. Default is `True`.
 - `enforce_schema` (optional): If `True`, non-existing fields in a stream are filled with None. If `False`, non-existing fields are ignored. Default is `True`.
 
 ```python
 parser.parse_m3u(path, check_live=True, enforce_schema=True)
 ```
 
+#### parse_json
+
+`parse_json(path: str, check_live: bool = True, enforce_schema: bool = True) -> None`
+
+Parses the content of a local file or URL and extracts the streams information.
+
+- `path`: The path to the json file, which can be a local file path or a URL.
+- `check_live` (optional): Set to `True` to check if the stream links are working or not. Default is `True`.
+- `enforce_schema` (optional): If `True`, non-existing fields in a stream are filled with None. If `False`, non-existing fields are ignored. Default is `True`.
+
+```python
+parser.parse_m3u(path, check_live=True, enforce_schema=True)
+```
+
+#### parse_csv
+
+`parse_csv(path: str, check_live: bool = True, enforce_schema: bool = True) -> None`
+
+Parses the content of a local file or URL and extracts the streams information.
+
+- `path`: The path to the csv file, which can be a local file path or a URL.
+- `check_live` (optional): Set to `True` to check if the stream links are working or not. Default is `True`.
+- `enforce_schema` (optional): If `True`, non-existing fields in a stream are filled with None. If `False`, non-existing fields are ignored. Default is `True`.
+
+```python
+parser.parse_m3u(path, check_live=True, enforce_schema=True)
+```
+
 #### filter_by
 
 `filter_by(key: str, filters: Union[str, list], key_splitter: str = "-", retrieve: bool = True, nested_key: bool = False) -> None`
 
 Filters the streams information based on a key and filter/s.
 
 - `key`: The key to filter on, can be a single key or nested key (e.g., "language-name").
```

### Comparing `m3u_parser-0.2.1/README.md` & `m3u_parser-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,30 @@
+Metadata-Version: 2.1
+Name: m3u_parser
+Version: 0.3.0
+Summary: A useful package for parsing m3u files or links
+Home-page: https://github.com/pawanpaudel93/m3u_parser
+Author: Pawan Paudel
+Author-email: pawanpaudel93@gmail.com
+License: ISC
+Classifier: License :: OSI Approved :: ISC License (ISCL)
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.0
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+
 # m3u_parser
 
-![version](https://img.shields.io/badge/version-0.2.1-blue.svg?cacheSeconds=2592000)
+![version](https://img.shields.io/badge/version-0.3.0-blue.svg?cacheSeconds=2592000)
 
 A Python package for parsing m3u files and extracting streams information. The package allows you to convert the parsed information into JSON or CSV format and provides various filtering and sorting options.
 
 ## Install
 
 Using pip,
 
@@ -73,14 +93,42 @@
 - `check_live` (optional): Set to `True` to check if the stream links are working or not. Default is `True`.
 - `enforce_schema` (optional): If `True`, non-existing fields in a stream are filled with None. If `False`, non-existing fields are ignored. Default is `True`.
 
 ```python
 parser.parse_m3u(path, check_live=True, enforce_schema=True)
 ```
 
+#### parse_json
+
+`parse_json(path: str, check_live: bool = True, enforce_schema: bool = True) -> None`
+
+Parses the content of a local file or URL and extracts the streams information.
+
+- `path`: The path to the json file, which can be a local file path or a URL.
+- `check_live` (optional): Set to `True` to check if the stream links are working or not. Default is `True`.
+- `enforce_schema` (optional): If `True`, non-existing fields in a stream are filled with None. If `False`, non-existing fields are ignored. Default is `True`.
+
+```python
+parser.parse_m3u(path, check_live=True, enforce_schema=True)
+```
+
+#### parse_csv
+
+`parse_csv(path: str, check_live: bool = True, enforce_schema: bool = True) -> None`
+
+Parses the content of a local file or URL and extracts the streams information.
+
+- `path`: The path to the csv file, which can be a local file path or a URL.
+- `check_live` (optional): Set to `True` to check if the stream links are working or not. Default is `True`.
+- `enforce_schema` (optional): If `True`, non-existing fields in a stream are filled with None. If `False`, non-existing fields are ignored. Default is `True`.
+
+```python
+parser.parse_m3u(path, check_live=True, enforce_schema=True)
+```
+
 #### filter_by
 
 `filter_by(key: str, filters: Union[str, list], key_splitter: str = "-", retrieve: bool = True, nested_key: bool = False) -> None`
 
 Filters the streams information based on a key and filter/s.
 
 - `key`: The key to filter on, can be a single key or nested key (e.g., "language-name").
```

### Comparing `m3u_parser-0.2.1/m3u_parser/helper.py` & `m3u_parser-0.3.0/m3u_parser/helper.py`

 * *Files identical despite different names*

### Comparing `m3u_parser-0.2.1/m3u_parser/m3u_parser.py` & `m3u_parser-0.3.0/m3u_parser/m3u_parser.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import ssl
 import time
 from typing import Union
 
 import aiohttp
 import pycountry
 import requests
+import csv
 
 try:
     from helper import get_by_regex, is_valid_url, ndict_to_csv, run_until_completed, streams_regex, setup_logger
 except ModuleNotFoundError:
     from .helper import get_by_regex, is_valid_url, ndict_to_csv, run_until_completed, streams_regex, setup_logger
 
 ssl.match_hostname = lambda cert, hostname: hostname == cert["subjectAltName"][0][1]
@@ -42,96 +43,108 @@
     INFO: Saving to file...
     """
 
     def __init__(self, useragent: str = None, timeout: int = 5):
         self._streams_info = []
         self._streams_info_backup = []
         self._lines = []
-        self._timeout = timeout
+        self._timeout = aiohttp.ClientTimeout(total=timeout)
         self._loop = None
         self._enforce_schema = True
         self._headers = {
             "User-Agent": useragent
             if useragent
-            else "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/84.0.4147.89 Safari/537.36"
+            else "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36"
         }
         self._check_live = False
-        self._content = ""
         self._file_regex = re.compile(r"^[a-zA-Z]:\\((?:.*?\\)*).*\.[\d\w]{3,5}$|^(/[^/]*)+/?.[\d\w]{3,5}$")
         self._tvg_name_regex = re.compile(r"tvg-name=\"(.*?)\"", flags=re.IGNORECASE)
         self._tvg_id_regex = re.compile(r"tvg-id=\"(.*?)\"", flags=re.IGNORECASE)
         self._logo_regex = re.compile(r"tvg-logo=\"(.*?)\"", flags=re.IGNORECASE)
         self._category_regex = re.compile(r"group-title=\"(.*?)\"", flags=re.IGNORECASE)
         self._title_regex = re.compile(r"(?!.*=\",?.*\")[,](.*?)$", flags=re.IGNORECASE)
         self._country_regex = re.compile(r"tvg-country=\"(.*?)\"", flags=re.IGNORECASE)
         self._language_regex = re.compile(r"tvg-language=\"(.*?)\"", flags=re.IGNORECASE)
         self._tvg_url_regex = re.compile(r"tvg-url=\"(.*?)\"", flags=re.IGNORECASE)
 
-    def parse_m3u(self, path: str, check_live: bool = True, enforce_schema: bool = True):
-        """Parses the content of local file/URL.
-
-        It downloads the file from the given url or use the local file path to get the content and parses line by line
-        to a structured format of streams information.
-
-        :param path: Path can be a url or local filepath
-        :type path: str
-        :param enforce_schema: If the schema is forced, non-existing fields in a stream are filled with None/null. If it is not enforced, non-existing fields are ignored
-        :type enforce_schema: bool
-        :param check_live: To check if the stream links are working or not
-        :type check_live: bool
-        :rtype: None
-
-        """
-        self._check_live = check_live
-        self._enforce_schema = enforce_schema
+    def _read_content(self, path: str, type="m3u"):
+        content = ""
         if is_valid_url(path):
-            logger.info("Started parsing m3u link...")
+            logger.info(f"Started parsing {type} link...")
             try:
-                self._content = requests.get(path).text
+                content = requests.get(path).text
             except:
-                logger.error("Cannot read anything from the url!!!")
-                return
+                raise Exception("Cannot read anything from the url!!!")
         else:
-            logger.info("Started parsing m3u file...")
+            logger.info(f"Started parsing {type} file...")
             try:
                 with open(path, encoding="utf-8", errors="ignore") as fp:
-                    self._content = fp.read()
+                    content = fp.read()
             except FileNotFoundError:
-                logger.error("File doesn't exist!!!")
-                return
-
-        # splitting contents into lines to parse them
-        self._lines = [line.strip("\n\r") for line in self._content.split("\n") if line.strip("\n\r") != ""]
-        if len(self._lines) > 0:
-            self._parse_lines()
-        else:
-            logger.error("No content to parse!!!")
+                raise Exception("File doesn't exist!!!")
+        return content
 
     @staticmethod
     async def _run_until_completed(tasks):
         for res in run_until_completed(tasks):
             _ = await res
 
-    def _parse_lines(self):
-        num_lines = len(self._lines)
-        self._streams_info.clear()
+    def _set_event_loop(self):
         try:
             self._loop = asyncio.get_event_loop()
         except RuntimeError:
             self._loop = asyncio.new_event_loop()
             asyncio.set_event_loop(self._loop)
-        coros = (self._parse_line(line_num) for line_num in range(num_lines) if "#EXTINF" in self._lines[line_num])
-        self._loop.run_until_complete(self._run_until_completed(coros))
-        self._streams_info_backup = self._streams_info.copy()
-        self._loop.run_until_complete(asyncio.sleep(0))
+
+    def _close_loop(self):
         while self._loop.is_running():
             time.sleep(0.3)
             if not self._loop.is_running():
                 self._loop.close()
                 break
+
+    def _parse_lines(self):
+        num_lines = len(self._lines)
+        self._streams_info.clear()
+        self._set_event_loop()
+        coros = (self._parse_line(line_num) for line_num in range(num_lines) if "#EXTINF" in self._lines[line_num])
+        self._loop.run_until_complete(self._run_until_completed(coros))
+        self._loop.run_until_complete(asyncio.sleep(0))
+        self._streams_info_backup = self._streams_info.copy()
+        self._close_loop()
+        logger.info("Parsing completed !!!")
+
+    async def _get_status(self, stream_link):
+        try:
+            async with aiohttp.ClientSession() as session:
+                async with session.request(
+                    "get",
+                    stream_link,
+                    headers=self._headers,
+                    timeout=self._timeout,
+                ) as response:
+                    if response.status == 200:
+                        return "GOOD"
+        except:
+            pass
+        return "BAD"
+
+    async def _check_status(self, index):
+        stream_info = self._streams_info[index]
+        stream_info["status"] = await self._get_status(stream_info.get("url"))
+        self._streams_info[index] = stream_info
+
+    def _check_streams_status(self):
+        if self._check_live and len(self._streams_info) > 0:
+            self._set_event_loop()
+            coros = (self._check_status(index) for index in range(len(self._streams_info)))
+            self._loop.run_until_complete(self._run_until_completed(coros))
+            self._loop.run_until_complete(asyncio.sleep(0))
+            self._streams_info_backup = self._streams_info.copy()
+            self._close_loop()
         logger.info("Parsing completed !!!")
 
     async def _parse_line(self, line_num: int):
         line_info = self._lines[line_num]
         stream_link = ""
         streams_link = []
         status = "BAD"
@@ -187,32 +200,170 @@
             if language != None or self._enforce_schema:
                 language_obj = pycountry.languages.get(name=language if language else "")
                 info["language"] = {
                     "code": language_obj.alpha_3 if language_obj else None,
                     "name": language,
                 }
 
-            timeout = aiohttp.ClientTimeout(total=self._timeout)
             if self._check_live and status == "BAD":
-                try:
-                    async with aiohttp.ClientSession() as session:
-                        async with session.request(
-                            "get",
-                            stream_link,
-                            headers=self._headers,
-                            timeout=timeout,
-                        ) as response:
-                            if response.status == 200:
-                                status = "GOOD"
-                except:
-                    pass
+                status = await self._get_status(stream_link)
             if self._check_live:
                 info["status"] = status
             self._streams_info.append(info)
 
+    @staticmethod
+    def _get_m3u_content(streams_info: list) -> str:
+        """Save the streams information list to m3u file.
+
+        It saves the streams information list to m3u file.
+
+        :rtype: None
+        """
+        if len(streams_info) == 0:
+            return ""
+        content = ["#EXTM3U"]
+        for stream_info in streams_info:
+            line = "#EXTINF:-1"
+            if stream_info.get("tvg") != None:
+                for key, value in stream_info["tvg"].items():
+                    if value != None:
+                        line += ' tvg-{}="{}"'.format(key, value)
+            if stream_info.get("logo") != None:
+                line += ' tvg-logo="{}"'.format(stream_info["logo"])
+            if stream_info.get("country") != None and stream_info["country"].get("code") != None:
+                line += ' tvg-country="{}"'.format(stream_info["country"]["code"])
+            if stream_info.get("language") != None and stream_info["language"].get("name") != None:
+                line += ' tvg-language="{}"'.format(stream_info["language"]["name"])
+            if stream_info.get("category") != None:
+                line += ' group-title="{}"'.format(stream_info["category"])
+            if stream_info.get("name") != None:
+                line += ',' + stream_info['name']
+            content.append(line)
+            content.append(stream_info["url"])
+        return "\n".join(content)
+
+    def parse_m3u(self, path: str, check_live: bool = True, enforce_schema: bool = True):
+        """Parses the content of local file/URL.
+
+        It downloads the file from the given url or use the local file path to get the content and parses line by line
+        to a structured format of streams information.
+
+        :param path: Path can be a url or local filepath
+        :type path: str
+        :param enforce_schema: If the schema is forced, non-existing fields in a stream are filled with None/null. If it is not enforced, non-existing fields are ignored
+        :type enforce_schema: bool
+        :param check_live: To check if the stream links are working or not
+        :type check_live: bool
+        :rtype: None
+
+        """
+        content = ""
+        self._check_live = check_live
+        self._enforce_schema = enforce_schema
+        try:
+            content = self._read_content(path, "m3u")
+        except Exception as error:
+            logger.error(error)
+            return
+
+        # splitting contents into lines to parse them
+        self._lines = [line.strip("\n\r") for line in content.split("\n") if line.strip("\n\r") != ""]
+        if len(self._lines) > 0:
+            self._parse_lines()
+        else:
+            logger.error("No content to parse!!!")
+
+    def parse_json(self, path: str, check_live: bool = True, enforce_schema: bool = True):
+        """Parses the content of local JSON file/URL.
+
+        It downloads the file from the given url or use the local file path to get the structured format of streams information.
+
+        :param path: Path can be a url or local filepath
+        :type path: str
+        :param enforce_schema: If the schema is forced, non-existing fields in a stream are filled with None/null. If it is not enforced, non-existing fields are ignored
+        :type enforce_schema: bool
+        :param check_live: To check if the stream links are working or not
+        :type check_live: bool
+        :rtype: None
+
+        """
+        content = ""
+        self._check_live = check_live
+        self._enforce_schema = enforce_schema
+        try:
+            content = self._read_content(path, "json")
+        except Exception as error:
+            logger.error(error)
+            return
+        streams_info = json.loads(content)
+        if streams_info and type(streams_info) == list and len(streams_info) > 0:
+            self._streams_info = [
+                {
+                    "name": stream_info.get("name"),
+                    "logo": stream_info.get("logo"),
+                    "url": stream_info.get("url"),
+                    "category": stream_info.get("category"),
+                    "tvg": {
+                        "id": stream_info.get("tvg_id"),
+                        "name": stream_info.get("tvg_name"),
+                        "url": stream_info.get("tvg_url"),
+                    },
+                    "country": {"code": stream_info.get("country_code"), "name": stream_info.get("country_name")},
+                    "language": {"code": stream_info.get("language_code"), "name": stream_info.get("language_name")},
+                    "status": stream_info.get("status") or "BAD",
+                }
+                for stream_info in streams_info
+                if type(stream_info) == dict and stream_info.get("url")
+            ]
+        self._check_streams_status()
+
+    def parse_csv(self, path: str, check_live: bool = True, enforce_schema: bool = True):
+        """Parses the content of local CSV file/URL.
+
+        It downloads the file from the given url or use the local file path to get the structured format of streams information.
+
+        :param path: Path can be a url or local filepath
+        :type path: str
+        :param enforce_schema: If the schema is forced, non-existing fields in a stream are filled with None/null. If it is not enforced, non-existing fields are ignored
+        :type enforce_schema: bool
+        :param check_live: To check if the stream links are working or not
+        :type check_live: bool
+        :rtype: None
+
+        """
+        content = ""
+        self._check_live = check_live
+        self._enforce_schema = enforce_schema
+        try:
+            content = self._read_content(path, "csv")
+        except Exception as error:
+            logger.error(error)
+            return
+        reader = csv.DictReader(content.splitlines(), delimiter=",")
+        get_value = lambda row, key: row.get(key) or None
+        self._streams_info = [
+            {
+                "name": get_value(row, "name"),
+                "logo": get_value(row, "logo"),
+                "url": get_value(row, "url"),
+                "category": get_value(row, "category"),
+                "tvg": {
+                    "id": get_value(row, "tvg_id"),
+                    "name": get_value(row, "tvg_name"),
+                    "url": get_value(row, "tvg_url"),
+                },
+                "country": {"code": get_value(row, "country_code"), "name": get_value(row, "country_name")},
+                "language": {"code": get_value(row, "language_code"), "name": get_value(row, "language_name")},
+                "status": get_value(row, "status") or "BAD",
+            }
+            for row in reader
+            if get_value(row, "url")
+        ]
+        self._check_streams_status()
+
     def filter_by(
         self,
         key: str,
         filters: Union[str, list],
         key_splitter: str = "-",
         retrieve: bool = True,
         nested_key: bool = False,
@@ -387,44 +538,14 @@
         if not len(self._streams_info):
             logger.error("No streams information so could not get any random stream.")
             return
         if random_shuffle:
             random.shuffle(self._streams_info)
         return random.choice(self._streams_info)
 
-    def _get_m3u_content(self) -> str:
-        """Save the streams information list to m3u file.
-
-        It saves the streams information list to m3u file.
-
-        :rtype: None
-        """
-        if len(self._streams_info) == 0:
-            return ""
-        content = ["#EXTM3U"]
-        for stream_info in self._streams_info:
-            line = "#EXTINF:-1"
-            if stream_info.get("tvg") != None:
-                for key, value in stream_info["tvg"].items():
-                    if value != None:
-                        line += ' tvg-{}="{}"'.format(key, value)
-            if stream_info.get("logo") != None:
-                line += ' tvg-logo="{}"'.format(stream_info["logo"])
-            if stream_info.get("country") != None and stream_info["country"].get("code") != None:
-                line += ' tvg-country="{}"'.format(stream_info["country"]["code"])
-            if stream_info.get("language") != None and stream_info["language"].get("name") != None:
-                line += ' tvg-language="{}"'.format(stream_info["language"]["name"])
-            if stream_info.get("category") != None:
-                line += ' group-title="{}"'.format(stream_info["category"])
-            if stream_info.get("name") != None:
-                line += ',' + stream_info['name']
-            content.append(line)
-            content.append(stream_info["url"])
-        return "\n".join(content)
-
     def to_file(self, filename: str, format: str = "json"):
         """Save to file (CSV, JSON, or M3U)
 
         It saves streams information as a CSV, JSON, or M3U file with a given filename and format parameters.
 
         :param filename: Name of the file to save streams_info as.
         :type filename: str
@@ -456,15 +577,15 @@
             if self._enforce_schema:
                 ndict_to_csv(self._streams_info, filename)
                 logger.info("Saved to file: %s" % filename)
             else:
                 logger.info("Saving to csv file not supported if the schema was not forced (enforce_schema) !!!")
 
         elif format == "m3u":
-            content = self._get_m3u_content()
+            content = self._get_m3u_content(self._streams_info)
             with open(filename, mode="w", encoding="utf-8") as fp:
                 fp.write(content)
             logger.info("Saved to file: %s" % filename)
         else:
             logger.error("Unrecognised format!!!")
 
 
@@ -474,8 +595,8 @@
         "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/86.0.4240.75 Safari/537.36"
     )
     parser = M3uParser(timeout=5, useragent=useragent)
     parser.parse_m3u(url)
     parser.remove_by_extension("mp4")
     parser.filter_by("status", "GOOD")
     print(len(parser.get_list()))
-    parser.to_file("pawan.json")
+    parser.to_file("pawan.csv")
```

### Comparing `m3u_parser-0.2.1/m3u_parser.egg-info/PKG-INFO` & `m3u_parser-0.3.0/m3u_parser.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m3u-parser
-Version: 0.2.1
+Version: 0.3.0
 Summary: A useful package for parsing m3u files or links
 Home-page: https://github.com/pawanpaudel93/m3u_parser
 Author: Pawan Paudel
 Author-email: pawanpaudel93@gmail.com
 License: ISC
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Development Status :: 3 - Alpha
@@ -16,15 +16,15 @@
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 # m3u_parser
 
-![version](https://img.shields.io/badge/version-0.2.1-blue.svg?cacheSeconds=2592000)
+![version](https://img.shields.io/badge/version-0.3.0-blue.svg?cacheSeconds=2592000)
 
 A Python package for parsing m3u files and extracting streams information. The package allows you to convert the parsed information into JSON or CSV format and provides various filtering and sorting options.
 
 ## Install
 
 Using pip,
 
@@ -93,14 +93,42 @@
 - `check_live` (optional): Set to `True` to check if the stream links are working or not. Default is `True`.
 - `enforce_schema` (optional): If `True`, non-existing fields in a stream are filled with None. If `False`, non-existing fields are ignored. Default is `True`.
 
 ```python
 parser.parse_m3u(path, check_live=True, enforce_schema=True)
 ```
 
+#### parse_json
+
+`parse_json(path: str, check_live: bool = True, enforce_schema: bool = True) -> None`
+
+Parses the content of a local file or URL and extracts the streams information.
+
+- `path`: The path to the json file, which can be a local file path or a URL.
+- `check_live` (optional): Set to `True` to check if the stream links are working or not. Default is `True`.
+- `enforce_schema` (optional): If `True`, non-existing fields in a stream are filled with None. If `False`, non-existing fields are ignored. Default is `True`.
+
+```python
+parser.parse_m3u(path, check_live=True, enforce_schema=True)
+```
+
+#### parse_csv
+
+`parse_csv(path: str, check_live: bool = True, enforce_schema: bool = True) -> None`
+
+Parses the content of a local file or URL and extracts the streams information.
+
+- `path`: The path to the csv file, which can be a local file path or a URL.
+- `check_live` (optional): Set to `True` to check if the stream links are working or not. Default is `True`.
+- `enforce_schema` (optional): If `True`, non-existing fields in a stream are filled with None. If `False`, non-existing fields are ignored. Default is `True`.
+
+```python
+parser.parse_m3u(path, check_live=True, enforce_schema=True)
+```
+
 #### filter_by
 
 `filter_by(key: str, filters: Union[str, list], key_splitter: str = "-", retrieve: bool = True, nested_key: bool = False) -> None`
 
 Filters the streams information based on a key and filter/s.
 
 - `key`: The key to filter on, can be a single key or nested key (e.g., "language-name").
```

### Comparing `m3u_parser-0.2.1/setup.py` & `m3u_parser-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Package meta-data.
 NAME = "m3u_parser"
 DESCRIPTION = "A useful package for parsing m3u files or links"
 URL = "https://github.com/pawanpaudel93/m3u_parser"
 EMAIL = "pawanpaudel93@gmail.com"
 AUTHOR = "Pawan Paudel"
 REQUIRES_PYTHON = ">=3.0"
-VERSION = "0.2.1"
+VERSION = "0.3.0"
 
 REQUIRED = ["requests", "asyncio", "aiohttp", "pycountry"]
 
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
```

