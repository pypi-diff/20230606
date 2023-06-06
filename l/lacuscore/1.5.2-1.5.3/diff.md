# Comparing `tmp/lacuscore-1.5.2.tar.gz` & `tmp/lacuscore-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacuscore-1.5.2.tar", max compression
+gzip compressed data, was "lacuscore-1.5.3.tar", max compression
```

## Comparing `lacuscore-1.5.2.tar` & `lacuscore-1.5.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1516 2022-09-13 21:10:56.118975 lacuscore-1.5.2/LICENSE
--rw-r--r--   0        0        0      941 2022-10-17 09:41:56.955953 lacuscore-1.5.2/README.md
--rw-r--r--   0        0        0      169 2022-10-12 16:05:45.482302 lacuscore-1.5.2/lacuscore/__init__.py
--rw-r--r--   0        0        0     1105 2022-10-13 11:42:38.221153 lacuscore-1.5.2/lacuscore/lacus_monitoring.py
--rw-r--r--   0        0        0    28455 2023-06-02 12:37:27.026161 lacuscore-1.5.2/lacuscore/lacuscore.py
--rw-r--r--   0        0        0        0 2022-09-13 21:10:56.122975 lacuscore-1.5.2/lacuscore/py.typed
--rw-r--r--   0        0        0     1596 2023-06-05 13:10:58.713490 lacuscore-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 lacuscore-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1516 2022-09-13 21:10:56.118975 lacuscore-1.5.3/LICENSE
+-rw-r--r--   0        0        0      941 2022-10-17 09:41:56.955953 lacuscore-1.5.3/README.md
+-rw-r--r--   0        0        0      169 2022-10-12 16:05:45.482302 lacuscore-1.5.3/lacuscore/__init__.py
+-rw-r--r--   0        0        0     1105 2022-10-13 11:42:38.221153 lacuscore-1.5.3/lacuscore/lacus_monitoring.py
+-rw-r--r--   0        0        0    30255 2023-06-06 15:21:43.073515 lacuscore-1.5.3/lacuscore/lacuscore.py
+-rw-r--r--   0        0        0        0 2022-09-13 21:10:56.122975 lacuscore-1.5.3/lacuscore/py.typed
+-rw-r--r--   0        0        0     1596 2023-06-06 15:26:47.675025 lacuscore-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 lacuscore-1.5.3/PKG-INFO
```

### Comparing `lacuscore-1.5.2/LICENSE` & `lacuscore-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lacuscore-1.5.2/README.md` & `lacuscore-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `lacuscore-1.5.2/lacuscore/lacus_monitoring.py` & `lacuscore-1.5.3/lacuscore/lacus_monitoring.py`

 * *Files identical despite different names*

### Comparing `lacuscore-1.5.2/lacuscore/lacuscore.py` & `lacuscore-1.5.3/lacuscore/lacuscore.py`

 * *Files 7% similar despite different names*

```diff
@@ -104,15 +104,19 @@
     browser: Optional[str]
     device_name: Optional[str]
     user_agent: Optional[str]
     proxy: Optional[Union[str, Dict[str, str]]]
     general_timeout_in_sec: Optional[int]
     cookies: Optional[List[Dict[str, Any]]]
     headers: Optional[Union[str, Dict[str, str]]]
-    http_credentials: Optional[Dict[str, int]]
+    http_credentials: Optional[Dict[str, str]]
+    geolocation: Optional[Dict[str, float]]
+    timezone_id: Optional[str]
+    locale: Optional[str]
+    color_scheme: Optional[str]
     viewport: Optional[Dict[str, int]]
     referer: Optional[str]
     force: Optional[bool]
     recapture_interval: Optional[int]
     priority: Optional[int]
     uuid: Optional[str]
 
@@ -178,15 +182,19 @@
                 depth: int=0,
                 browser: Optional[BROWSER]=None, device_name: Optional[str]=None,
                 user_agent: Optional[str]=None,
                 proxy: Optional[Union[str, Dict[str, str]]]=None,
                 general_timeout_in_sec: Optional[int]=None,
                 cookies: Optional[List[Dict[str, Any]]]=None,
                 headers: Optional[Union[str, Dict[str, str]]]=None,
-                http_credentials: Optional[Dict[str, int]]=None,
+                http_credentials: Optional[Dict[str, str]]=None,
+                geolocation: Optional[Dict[str, float]]=None,
+                timezone_id: Optional[str]=None,
+                locale: Optional[str]=None,
+                color_scheme: Optional[str]=None,
                 viewport: Optional[Dict[str, int]]=None,
                 referer: Optional[str]=None,
                 rendered_hostname_only: bool=True,
                 force: bool=False,
                 recapture_interval: int=300,
                 priority: int=0,
                 uuid: Optional[str]=None
@@ -200,15 +208,19 @@
                 depth: int=0,
                 browser: Optional[BROWSER]=None, device_name: Optional[str]=None,
                 user_agent: Optional[str]=None,
                 proxy: Optional[Union[str, Dict[str, str]]]=None,
                 general_timeout_in_sec: Optional[int]=None,
                 cookies: Optional[List[Dict[str, Any]]]=None,
                 headers: Optional[Union[str, Dict[str, str]]]=None,
-                http_credentials: Optional[Dict[str, int]]=None,
+                http_credentials: Optional[Dict[str, str]]=None,
+                geolocation: Optional[Dict[str, float]]=None,
+                timezone_id: Optional[str]=None,
+                locale: Optional[str]=None,
+                color_scheme: Optional[str]=None,
                 viewport: Optional[Dict[str, int]]=None,
                 referer: Optional[str]=None,
                 rendered_hostname_only: bool=True,
                 force: bool=False,
                 recapture_interval: int=300,
                 priority: int=0,
                 uuid: Optional[str]=None
@@ -225,14 +237,18 @@
         :param device_name: The name of the device, must be something Playwright knows
         :param user_agent: The user agent the browser will use for the capture
         :param proxy: SOCKS5 proxy to use for capturing
         :param general_timeout_in_sec: The capture will raise a timeout it it takes more than that time
         :param cookies: A list of cookies
         :param headers: The headers to pass to the capture
         :param http_credentials: HTTP Credentials to pass to the capture
+        :param geolocation: Geolocation of the browser to pass to the capture
+        :param timezone_id: The timezone of the browser to pass to the capture
+        :param locale: The locale of the browser to pass to the capture
+        :param color_scheme: The prefered color scheme of the browser to pass to the capture
         :param viewport: The viewport of the browser used for capturing
         :param referer: The referer URL for the capture
         :param rendered_hostname_only: If depth > 0: only capture URLs with the same hostname as the rendered page
         :param force: Force recapture, even if the same one was already done within the recapture_interval
         :param recapture_interval: The time the enqueued settings are kept in memory to avoid duplicates
         :param priority: The priority of the capture
         :param uuid: The preset priority of the capture, auto-generated if not present. Should only be used if the initiator couldn't enqueue immediately. NOTE: it will be overwritten if the UUID already exists.
@@ -267,14 +283,22 @@
                 to_enqueue['general_timeout_in_sec'] = general_timeout_in_sec
             if cookies:
                 to_enqueue['cookies'] = cookies
             if headers:
                 to_enqueue['headers'] = headers
             if http_credentials:
                 to_enqueue['http_credentials'] = http_credentials
+            if geolocation:
+                to_enqueue['geolocation'] = geolocation
+            if timezone_id:
+                to_enqueue['timezone_id'] = timezone_id
+            if locale:
+                to_enqueue['locale'] = locale
+            if color_scheme:
+                to_enqueue['color_scheme'] = color_scheme
             if viewport:
                 to_enqueue['viewport'] = viewport
             if referer:
                 to_enqueue['referer'] = referer
 
         hash_query = hashlib.sha512(pickle.dumps(to_enqueue)).hexdigest()
         if not force:
@@ -398,27 +422,29 @@
         self.redis.zadd('lacus:ongoing', {uuid: time.time()})
 
         retry = False
         try:
             setting_keys = ['depth', 'rendered_hostname_only', 'url', 'document_name',
                             'document', 'browser', 'device_name', 'user_agent', 'proxy',
                             'general_timeout_in_sec', 'cookies', 'headers', 'http_credentials',
-                            'viewport', 'referer']
+                            'viewport', 'referer', 'geolocation', 'timezone_id', 'locale',
+                            'color_scheme']
             result: CaptureResponse = {}
             to_capture: CaptureSettings = {}
             document_as_bytes = b''
             url: str = ''
             try:
                 for k, v in zip(setting_keys, self.redis.hmget(f'lacus:capture_settings:{uuid}', setting_keys)):
                     if v is None:
                         continue
-                    if k in ['url', 'document_name', 'browser', 'device_name', 'user_agent', 'referer']:
+                    if k in ['url', 'document_name', 'browser', 'device_name', 'user_agent',
+                             'referer', 'timezone_id', 'locale', 'color_scheme']:
                         # string
                         to_capture[k] = v.decode()  # type: ignore
-                    elif k in ['cookies', 'http_credentials', 'viewport']:
+                    elif k in ['cookies', 'http_credentials', 'viewport', 'geolocation']:
                         # dicts or list
                         to_capture[k] = json.loads(v)  # type: ignore
                     elif k in ['proxy', 'headers']:
                         # can be dict or str
                         try:
                             to_capture[k] = json.loads(v)  # type: ignore
                         except Exception:
@@ -518,14 +544,19 @@
                         proxy=proxy,
                         general_timeout_in_sec=general_timeout) as capture:
                     # required by Mypy: https://github.com/python/mypy/issues/3004
                     capture.headers = to_capture.get('headers')  # type: ignore
                     capture.cookies = to_capture.get('cookies')  # type: ignore
                     capture.viewport = to_capture.get('viewport')  # type: ignore
                     capture.user_agent = to_capture.get('user_agent')  # type: ignore
+                    capture.http_credentials = to_capture.get('http_credentials')  # type: ignore
+                    capture.geolocation = to_capture.get('geolocation')  # type: ignore
+                    capture.timezone_id = to_capture.get('timezone_id')  # type: ignore
+                    capture.locale = to_capture.get('locale')  # type: ignore
+                    capture.color_scheme = to_capture.get('color_scheme')  # type: ignore
                     try:
                         await asyncio.wait_for(capture.initialize_context(), timeout=general_timeout)
                     except (TimeoutError, asyncio.exceptions.TimeoutError):
                         logger.warning(f'Initializing the context for {url} took longer than the allowed general timeout ({general_timeout}s)')
                         raise RetryCapture
                     playwright_result = await asyncio.wait_for(
                         capture.capture_page(
```

### Comparing `lacuscore-1.5.2/pyproject.toml` & `lacuscore-1.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lacuscore"
-version = "1.5.2"
+version = "1.5.3"
 description = "Core of Lacus, usable as a module"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/ail-project/LacusCore"
 documentation = "https://lacuscore.readthedocs.io/en/latest/"
 
 readme = "README.md"
@@ -28,15 +28,15 @@
 
 include = ['README.md']
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.31.0"
 Sphinx = { version = "^7.0.1", optional = true }
-playwrightcapture = {extras = ["recaptcha"], version = "^1.20.2"}
+playwrightcapture = {extras = ["recaptcha"], version = "^1.20.3"}
 defang = "^0.5.3"
 ua-parser = "^0.16.1"
 redis = {version = "^4.5.5", extras = ["hiredis"]}
 
 [tool.poetry.extras]
 docs = ["Sphinx"]
```

### Comparing `lacuscore-1.5.2/PKG-INFO` & `lacuscore-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lacuscore
-Version: 1.5.2
+Version: 1.5.3
 Summary: Core of Lacus, usable as a module
 Home-page: https://github.com/ail-project/LacusCore
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Provides-Extra: docs
 Requires-Dist: Sphinx (>=7.0.1,<8.0.0) ; extra == "docs"
 Requires-Dist: defang (>=0.5.3,<0.6.0)
-Requires-Dist: playwrightcapture[recaptcha] (>=1.20.2,<2.0.0)
+Requires-Dist: playwrightcapture[recaptcha] (>=1.20.3,<2.0.0)
 Requires-Dist: redis[hiredis] (>=4.5.5,<5.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: ua-parser (>=0.16.1,<0.17.0)
 Project-URL: Documentation, https://lacuscore.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/ail-project/LacusCore
 Description-Content-Type: text/markdown
```

