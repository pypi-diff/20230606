# Comparing `tmp/twitter-api-client-0.8.7.tar.gz` & `tmp/twitter-api-client-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.8.7.tar", last modified: Sun Jun  4 17:21:39 2023, max compression
+gzip compressed data, was "twitter-api-client-0.8.8.tar", last modified: Tue Jun  6 03:24:06 2023, max compression
```

## Comparing `twitter-api-client-0.8.7.tar` & `twitter-api-client-0.8.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-04 17:21:39.733603 twitter-api-client-0.8.7/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-05-28 16:24:21.000000 twitter-api-client-0.8.7/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-04 17:21:39.733603 twitter-api-client-0.8.7/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-04 17:21:39.733603 twitter-api-client-0.8.7/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)    12740 2023-06-04 17:13:56.000000 twitter-api-client-0.8.7/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-04 17:21:39.732602 twitter-api-client-0.8.7/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-06-02 19:12:02.000000 twitter-api-client-0.8.7/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    23270 2023-06-04 16:20:00.000000 twitter-api-client-0.8.7/twitter/account.py
--rw-r--r--   0 x         (1000) x         (1000)    28755 2023-06-03 21:50:49.000000 twitter-api-client-0.8.7/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     7410 2023-06-02 20:00:37.000000 twitter-api-client-0.8.7/twitter/login.py
--rw-r--r--   0 x         (1000) x         (1000)    27620 2023-06-04 17:13:56.000000 twitter-api-client-0.8.7/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     5960 2023-06-02 01:50:23.000000 twitter-api-client-0.8.7/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     9625 2023-06-04 17:08:22.000000 twitter-api-client-0.8.7/twitter/util.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-04 17:21:39.733603 twitter-api-client-0.8.7/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-04 17:21:39.000000 twitter-api-client-0.8.7/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      355 2023-06-04 17:21:39.000000 twitter-api-client-0.8.7/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-04 17:21:39.000000 twitter-api-client-0.8.7/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       91 2023-06-04 17:21:39.000000 twitter-api-client-0.8.7/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        8 2023-06-04 17:21:39.000000 twitter-api-client-0.8.7/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-06 03:24:06.656739 twitter-api-client-0.8.8/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-05-28 16:24:21.000000 twitter-api-client-0.8.8/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-06 03:24:06.656739 twitter-api-client-0.8.8/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-06 03:24:06.656739 twitter-api-client-0.8.8/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)    12740 2023-06-06 03:23:13.000000 twitter-api-client-0.8.8/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-06 03:24:06.655739 twitter-api-client-0.8.8/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-06-02 19:12:02.000000 twitter-api-client-0.8.8/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    23313 2023-06-06 03:22:31.000000 twitter-api-client-0.8.8/twitter/account.py
+-rw-r--r--   0 x         (1000) x         (1000)    28671 2023-06-06 03:22:31.000000 twitter-api-client-0.8.8/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     7410 2023-06-02 20:00:37.000000 twitter-api-client-0.8.8/twitter/login.py
+-rw-r--r--   0 x         (1000) x         (1000)    28193 2023-06-06 03:22:31.000000 twitter-api-client-0.8.8/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     5912 2023-06-06 03:22:31.000000 twitter-api-client-0.8.8/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     9625 2023-06-04 17:08:22.000000 twitter-api-client-0.8.8/twitter/util.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-06 03:24:06.655739 twitter-api-client-0.8.8/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-06 03:24:06.000000 twitter-api-client-0.8.8/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      355 2023-06-06 03:24:06.000000 twitter-api-client-0.8.8/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-06 03:24:06.000000 twitter-api-client-0.8.8/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       91 2023-06-06 03:24:06.000000 twitter-api-client-0.8.8/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        8 2023-06-06 03:24:06.000000 twitter-api-client-0.8.8/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.8.7/LICENSE` & `twitter-api-client-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.7/PKG-INFO` & `twitter-api-client-0.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.8.7
+Version: 0.8.8
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
```

### Comparing `twitter-api-client-0.8.7/setup.py` & `twitter-api-client-0.8.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.8.7",
+    version="0.8.8",
     python_requires=">=3.10.10",
     description="Twitter API",
     long_description=dedent('''
     
     ## Implementation of Twitter's v1, v2, and GraphQL APIs
```

### Comparing `twitter-api-client-0.8.7/twitter/account.py` & `twitter-api-client-0.8.8/twitter/account.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         if media:
             media_id = self._upload_media(media, is_dm=True)
             variables['message']['media'] = {'id': media_id, 'text': text}
         else:
             variables['message']['text'] = {'text': text}
         res = self.gql('POST', Operation.useSendMessageMutation, variables)
         if find_key(res, 'dm_validation_failure_type'):
-            logger.debug(f"{RED}Failed to send DM(s) to {receivers}{RESET}")
+            self.logger.debug(f"{RED}Failed to send DM(s) to {receivers}{RESET}")
         return res
 
     def tweet(self, text: str, *, media: any = None, **kwargs) -> dict:
         variables = {
             'tweet_text': text,
             'dark_request': False,
             'media': {
@@ -556,16 +556,17 @@
         r = self.session.post(url, headers=get_headers(self.session), json=params)
         return r
 
     @staticmethod
     def init_logger(cfg: dict) -> Logger:
         if cfg:
             logging.config.dictConfig(cfg)
-            return logging.getLogger(__name__)
-        return logger
+        else:
+            logging.config.dictConfig(LOG_CONFIG)
+        return logging.getLogger(__name__)
 
     @staticmethod
     def validate_session(*args, **kwargs):
         email, username, password, session = args
         if session and all(session.cookies.get(c) for c in {'ct0', 'auth_token'}):
             # authenticated session provided
             return session
```

### Comparing `twitter-api-client-0.8.7/twitter/constants.py` & `twitter-api-client-0.8.8/twitter/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     'tqdm',
     'bcrypt',
     'python-gnupg',
     'pyopenssl',
     'uvloop',
 ]
 
-LOGGING_CONFIG = {
+LOG_CONFIG = {
     'version': 1,
     'disable_existing_loggers': False,
     'formatters': {
         'standard': {
             'format': '%(asctime)s.%(msecs)03d [%(levelname)s] :: %(message)s',
             'datefmt': '%Y-%m-%d %H:%M:%S'
         },
@@ -69,17 +69,14 @@
             'level': 'WARNING',
             'propagate': False
         }
         for pkg in DISABLE_LOG_PROPAGATION
     },
 }
 
-logging.config.dictConfig(LOGGING_CONFIG)
-logger = logging.getLogger(__name__)
-
 
 @dataclass
 class SpaceCategory:
     Top = 'Top'
     Live = 'Live'
     Upcoming = 'Upcoming'
```

### Comparing `twitter-api-client-0.8.7/twitter/login.py` & `twitter-api-client-0.8.8/twitter/login.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.7/twitter/scraper.py` & `twitter-api-client-0.8.8/twitter/scraper.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,16 +31,17 @@
 
 
 class Scraper:
     def __init__(self, email: str = None, username: str = None, password: str = None, session: Client = None, **kwargs):
         self.guest = False
         self.logger = self.init_logger(kwargs.get('log_config', False))
         self.session = self.validate_session(email, username, password, session, **kwargs)
-        self.save = kwargs.get('save', True)
         self.debug = kwargs.get('debug', 0)
+        self.save = kwargs.get('save', True)
+        self.pbar = kwargs.get('pbar', True)
         self.out_path = Path('data')
 
     def users(self, screen_names: list[str], **kwargs) -> list[dict]:
         return self._run(Operation.UserByScreenName, screen_names, **kwargs)
 
     def tweets_by_id(self, tweet_ids: list[int], **kwargs) -> list[dict]:
         return self._run(Operation.TweetResultByRestId, tweet_ids, **kwargs)
@@ -116,16 +117,18 @@
             if videos:
                 video_urls = [x['variants'] for m in media if (x := m.get('video_info'))]
                 hq_videos = {sorted(v, key=lambda d: d.get('bitrate', 0))[-1]['url'] for v in video_urls}
                 [urls.append([url, video]) for video in hq_videos]
 
         async def process():
             async with AsyncClient(headers=self.session.headers, cookies=self.session.cookies) as client:
-                return await tqdm_asyncio.gather(*(download(client, x, y) for x, y in urls),
-                                                 desc='downloading media')
+                tasks = (download(client, x, y) for x, y in urls)
+                if self.pbar:
+                    return await tqdm_asyncio.gather(*tasks, desc='Downloading media')
+                return await asyncio.gather(*tasks)
 
         async def download(client: AsyncClient, post_url: str, cdn_url: str) -> None:
             name = urlsplit(post_url).path.replace('/', '_')[1:]
             ext = urlsplit(cdn_url).path.split('/')[-1]
             try:
                 r = await client.get(cdn_url)
                 async with aiofiles.open(out / f'{name}_{ext}', 'wb') as fp:
@@ -150,18 +153,18 @@
 
         async def process():
             url = set_qs('https://twitter.com/i/api/2/guide.json', trending_params)
             offsets = utc or ["-1200", "-1100", "-1000", "-0900", "-0800", "-0700", "-0600", "-0500", "-0400", "-0300",
                               "-0200", "-0100", "+0000", "+0100", "+0200", "+0300", "+0400", "+0500", "+0600", "+0700",
                               "+0800", "+0900", "+1000", "+1100", "+1200", "+1300", "+1400"]
             async with AsyncClient(headers=get_headers(self.session)) as client:
-                return await tqdm_asyncio.gather(
-                    *(get_trends(client, o, url) for o in offsets),
-                    desc='downloading media'
-                )
+                tasks = (get_trends(client, o, url) for o in offsets)
+                if self.pbar:
+                    return await tqdm_asyncio.gather(*tasks, desc='Getting trends')
+                return await asyncio.gather(*tasks)
 
         trends = asyncio.run(process())
         out = self.out_path / 'raw' / 'trends'
         out.mkdir(parents=True, exist_ok=True)
         (out / f'{time.time_ns()}.json').write_text(orjson.dumps(
             {k: v for d in trends for k, v in d.items()},
             option=orjson.OPT_INDENT_2 | orjson.OPT_SORT_KEYS).decode(), encoding='utf-8')
@@ -290,15 +293,18 @@
             }
 
         async def process():
             limits = Limits(max_connections=100, max_keepalive_connections=10)
             headers = self.session.headers if self.guest else get_headers(self.session)
             cookies = self.session.cookies
             async with AsyncClient(limits=limits, headers=headers, cookies=cookies, timeout=20) as c:
-                return await tqdm_asyncio.gather(*(get(c, key) for key in keys), desc='downloading chat')
+                tasks = (get(c, key) for key in keys)
+                if self.pbar:
+                    return await tqdm_asyncio.gather(*tasks, desc='Downloading chat data')
+                return await asyncio.gather(*tasks)
 
         return asyncio.run(process())
 
     def _download_audio(self, data: list[dict]) -> None:
         async def get(s: AsyncClient, chunk: str, rest_id: str) -> tuple:
             r = await s.get(chunk)
             return rest_id, r
@@ -307,15 +313,17 @@
             limits = Limits(max_connections=100, max_keepalive_connections=10)
             headers = self.session.headers if self.guest else get_headers(self.session)
             cookies = self.session.cookies
             async with AsyncClient(limits=limits, headers=headers, cookies=cookies, timeout=20) as c:
                 tasks = []
                 for d in data:
                     tasks.extend([get(c, chunk, d['rest_id']) for chunk in d['chunks']])
-                return await tqdm_asyncio.gather(*tasks, desc='downloading audio')
+                if self.pbar:
+                    return await tqdm_asyncio.gather(*tasks, desc='Downloading audio')
+                return await asyncio.gather(*tasks)
 
         chunks = asyncio.run(process(data))
         streams = {}
         [streams.setdefault(_id, []).append(chunk) for _id, chunk in chunks]
         # ensure chunks are in correct order
         for k, v in streams.items():
             streams[k] = sorted(v, key=lambda x: int(re.findall('_(\d+)_\w\.aac$', x.url.path)[0]))
@@ -377,18 +385,18 @@
         return r
 
     async def _process(self, operation: tuple, queries: list[dict], **kwargs):
         limits = Limits(max_connections=100, max_keepalive_connections=10)
         headers = self.session.headers if self.guest else get_headers(self.session)
         cookies = self.session.cookies
         async with AsyncClient(limits=limits, headers=headers, cookies=cookies, timeout=20) as c:
-            return await tqdm_asyncio.gather(
-                *(self._paginate(c, operation, **q, **kwargs) for q in queries),
-                desc=operation[-1],
-            )
+            tasks = (self._paginate(c, operation, **q, **kwargs) for q in queries)
+            if self.pbar:
+                return await tqdm_asyncio.gather(*tasks, desc=operation[-1])
+            return await asyncio.gather(*tasks)
 
     async def _paginate(self, client: AsyncClient, operation: tuple, **kwargs):
         limit = kwargs.pop('limit', math.inf)
         cursor = kwargs.pop('cursor', None)
         is_resuming = False
         dups = 0
         DUP_LIMIT = 3
@@ -503,15 +511,18 @@
                 url='https://proxsee.pscp.tv/api/v2/accessChatPublic',
                 json={'chat_token': r.json()['chatToken']}
             )
             return r.json()
 
         limits = Limits(max_connections=100)
         async with AsyncClient(headers=client.headers, limits=limits, timeout=30) as c:
-            return await tqdm_asyncio.gather(*(get(c, _id) for _id in spaces), desc='getting live transcripts')
+            tasks = (get(c, _id) for _id in spaces)
+            if self.pbar:
+                return await tqdm_asyncio.gather(*tasks, desc='Getting live transcripts')
+            return await asyncio.gather(*tasks)
 
     def space_live_transcript(self, room: str, frequency: int = 1):
         async def get(spaces: list[dict]):
             client = init_session()
             chats = await self._get_live_chats(client, spaces)
             await asyncio.gather(*(self._space_listener(c, frequency) for c in chats))
 
@@ -588,16 +599,17 @@
         spaces = self.spaces(rooms=rooms)
         return asyncio.run(process(spaces))
 
     @staticmethod
     def init_logger(cfg: dict) -> Logger:
         if cfg:
             logging.config.dictConfig(cfg)
-            return logging.getLogger(__name__)
-        return logger
+        else:
+            logging.config.dictConfig(LOG_CONFIG)
+        return logging.getLogger(__name__)
 
     def validate_session(self, *args, **kwargs):
         email, username, password, session = args
         if session and all(session.cookies.get(c) for c in {'ct0', 'auth_token'}):
             # authenticated session provided
             return session
         if not session:
```

### Comparing `twitter-api-client-0.8.7/twitter/search.py` & `twitter-api-client-0.8.8/twitter/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,58 +37,37 @@
 class Search:
     def __init__(self, email: str = None, username: str = None, password: str = None, session: Client = None, **kwargs):
         self.logger = self.init_logger(kwargs.get('log_config', False))
         self.session = self.validate_session(email, username, password, session, **kwargs)
         self.api = 'https://api.twitter.com/2/search/adaptive.json?'
         self.save = kwargs.get('save', True)
         self.debug = kwargs.get('debug', 0)
-        self.logger = self.init_logger(kwargs.get('log_config', False))
-
-    @staticmethod
-    def init_logger(cfg: dict) -> Logger:
-        if cfg:
-            logging.config.dictConfig(cfg)
-            return logging.getLogger(__name__)
-        return logger
-
-    @staticmethod
-    def validate_session(*args, **kwargs):
-        email, username, password, session = args
-        if session and all(session.cookies.get(c) for c in {'ct0', 'auth_token'}):
-            # authenticated session provided
-            return session
-        if not session:
-            # no session provided, login to authenticate
-            return login(email, username, password, **kwargs)
-        raise Exception('Session not authenticated. '
-                        'Please use an authenticated session or remove the `session` argument and try again.')
 
     def run(self, *args, out: str = 'data', **kwargs):
         out_path = self.make_output_dirs(out)
         if kwargs.get('latest', False):
             search_config['tweet_search_mode'] = 'live'
         return asyncio.run(self.process(args, search_config, out_path, **kwargs))
 
     async def process(self, queries: tuple, config: dict, out: Path, **kwargs) -> list:
         async with AsyncClient(headers=get_headers(self.session)) as s:
             return await asyncio.gather(*(self.paginate(q, s, config, out, **kwargs) for q in queries))
 
-    async def paginate(self, query: str, session: AsyncClient, config: dict, out: Path, **kwargs) -> list[
-        dict]:
+    async def paginate(self, query: str, session: AsyncClient, config: dict, out: Path, **kwargs) -> list[dict]:
         config['q'] = query
         data, next_cursor = await self.backoff(lambda: self.get(session, config), query, **kwargs)
         all_data = [data]
         c = colors.pop() if colors else ''
         ids = set()
         while next_cursor:
             ids |= set(data['globalObjects']['tweets'])
             if len(ids) >= kwargs.get('limit', math.inf):
                 if self.debug:
                     self.logger.debug(
-                        f'[{GREEN}success{RESET}] returned {len(ids)} search results for {c}{query}{reset}')
+                        f'[{GREEN}success{RESET}] Returned {len(ids)} search results for {c}{query}{reset}')
                 return all_data
             if self.debug:
                 self.logger.debug(f'{c}{query}{reset}')
             config['cursor'] = next_cursor
 
             data, next_cursor = await self.backoff(lambda: self.get(session, config), query, **kwargs)
             if not data:
@@ -116,15 +95,15 @@
                 if i == retries:
                     if self.debug:
                         self.logger.debug(f'Max retries exceeded\n{e}')
                     return None, None
                 t = 2 ** i + random.random()
                 if self.debug:
                     self.logger.debug(
-                        f'No data for: \u001b[1m{info}\u001b[0m | retrying in {f"{t:.2f}"} seconds\t\t{e}')
+                        f'No data for: {BOLD}{info}{RESET}, retrying in {f"{t:.2f}"} seconds\t\t{e}')
                 time.sleep(t)
 
     async def get(self, session: AsyncClient, params: dict) -> tuple:
         url = set_qs(self.api, params, update=True, safe='()')
         r = await session.get(url)
         data = r.json()
         next_cursor = self.get_cursor(data)
@@ -150,7 +129,27 @@
 
     def make_output_dirs(self, path: str) -> Path:
         p = Path(f'{path}')
         (p / 'raw').mkdir(parents=True, exist_ok=True)
         (p / 'processed').mkdir(parents=True, exist_ok=True)
         (p / 'final').mkdir(parents=True, exist_ok=True)
         return p
+
+    @staticmethod
+    def init_logger(cfg: dict) -> Logger:
+        if cfg:
+            logging.config.dictConfig(cfg)
+        else:
+            logging.config.dictConfig(LOG_CONFIG)
+        return logging.getLogger(__name__)
+
+    @staticmethod
+    def validate_session(*args, **kwargs):
+        email, username, password, session = args
+        if session and all(session.cookies.get(c) for c in {'ct0', 'auth_token'}):
+            # authenticated session provided
+            return session
+        if not session:
+            # no session provided, log-in to authenticate
+            return login(email, username, password, **kwargs)
+        raise Exception('Session not authenticated. '
+                        'Please use an authenticated session or remove the `session` argument and try again.')
```

### Comparing `twitter-api-client-0.8.7/twitter/util.py` & `twitter-api-client-0.8.8/twitter/util.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.7/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.8.8/twitter_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.8.7
+Version: 0.8.8
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
```

