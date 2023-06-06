# Comparing `tmp/twitter-api-client-0.8.8.tar.gz` & `tmp/twitter-api-client-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.8.8.tar", last modified: Tue Jun  6 03:24:06 2023, max compression
+gzip compressed data, was "twitter-api-client-0.8.9.tar", last modified: Tue Jun  6 19:10:38 2023, max compression
```

## Comparing `twitter-api-client-0.8.8.tar` & `twitter-api-client-0.8.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-06 03:24:06.656739 twitter-api-client-0.8.8/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-05-28 16:24:21.000000 twitter-api-client-0.8.8/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-06 03:24:06.656739 twitter-api-client-0.8.8/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-06 03:24:06.656739 twitter-api-client-0.8.8/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)    12740 2023-06-06 03:23:13.000000 twitter-api-client-0.8.8/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-06 03:24:06.655739 twitter-api-client-0.8.8/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-06-02 19:12:02.000000 twitter-api-client-0.8.8/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    23313 2023-06-06 03:22:31.000000 twitter-api-client-0.8.8/twitter/account.py
--rw-r--r--   0 x         (1000) x         (1000)    28671 2023-06-06 03:22:31.000000 twitter-api-client-0.8.8/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     7410 2023-06-02 20:00:37.000000 twitter-api-client-0.8.8/twitter/login.py
--rw-r--r--   0 x         (1000) x         (1000)    28193 2023-06-06 03:22:31.000000 twitter-api-client-0.8.8/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     5912 2023-06-06 03:22:31.000000 twitter-api-client-0.8.8/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     9625 2023-06-04 17:08:22.000000 twitter-api-client-0.8.8/twitter/util.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-06 03:24:06.655739 twitter-api-client-0.8.8/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-06 03:24:06.000000 twitter-api-client-0.8.8/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      355 2023-06-06 03:24:06.000000 twitter-api-client-0.8.8/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-06 03:24:06.000000 twitter-api-client-0.8.8/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       91 2023-06-06 03:24:06.000000 twitter-api-client-0.8.8/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        8 2023-06-06 03:24:06.000000 twitter-api-client-0.8.8/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-06 19:10:38.844102 twitter-api-client-0.8.9/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-05-28 16:24:21.000000 twitter-api-client-0.8.9/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-06 19:10:38.844102 twitter-api-client-0.8.9/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-06 19:10:38.845102 twitter-api-client-0.8.9/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)    12740 2023-06-06 19:09:50.000000 twitter-api-client-0.8.9/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-06 19:10:38.841102 twitter-api-client-0.8.9/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-06-02 19:12:02.000000 twitter-api-client-0.8.9/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    23524 2023-06-06 19:05:18.000000 twitter-api-client-0.8.9/twitter/account.py
+-rw-r--r--   0 x         (1000) x         (1000)    28299 2023-06-06 19:05:18.000000 twitter-api-client-0.8.9/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     7410 2023-06-02 20:00:37.000000 twitter-api-client-0.8.9/twitter/login.py
+-rw-r--r--   0 x         (1000) x         (1000)    28404 2023-06-06 19:05:18.000000 twitter-api-client-0.8.9/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     6123 2023-06-06 19:05:18.000000 twitter-api-client-0.8.9/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     9625 2023-06-04 17:08:22.000000 twitter-api-client-0.8.9/twitter/util.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-06 19:10:38.844102 twitter-api-client-0.8.9/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-06 19:10:38.000000 twitter-api-client-0.8.9/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      355 2023-06-06 19:10:38.000000 twitter-api-client-0.8.9/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-06 19:10:38.000000 twitter-api-client-0.8.9/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       91 2023-06-06 19:10:38.000000 twitter-api-client-0.8.9/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        8 2023-06-06 19:10:38.000000 twitter-api-client-0.8.9/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.8.8/LICENSE` & `twitter-api-client-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.8/PKG-INFO` & `twitter-api-client-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.8.8
+Version: 0.8.9
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
```

### Comparing `twitter-api-client-0.8.8/setup.py` & `twitter-api-client-0.8.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.8.8",
+    version="0.8.9",
     python_requires=">=3.10.10",
     description="Twitter API",
     long_description=dedent('''
     
     ## Implementation of Twitter's v1, v2, and GraphQL APIs
```

### Comparing `twitter-api-client-0.8.8/twitter/account.py` & `twitter-api-client-0.8.9/twitter/account.py`

 * *Files 0% similar despite different names*

```diff
@@ -557,16 +557,22 @@
         return r
 
     @staticmethod
     def init_logger(cfg: dict) -> Logger:
         if cfg:
             logging.config.dictConfig(cfg)
         else:
-            logging.config.dictConfig(LOG_CONFIG)
-        return logging.getLogger(__name__)
+            logging.config.dictConfig(LOGGER_CONFIG)
+
+        # Set level of all other loggers to ERROR
+        for name in logging.root.manager.loggerDict:
+            if name != LOGGER_NAME:
+                logging.getLogger(name).setLevel(logging.ERROR)
+
+        return logging.getLogger(LOGGER_NAME)
 
     @staticmethod
     def validate_session(*args, **kwargs):
         email, username, password, session = args
         if session and all(session.cookies.get(c) for c in {'ct0', 'auth_token'}):
             # authenticated session provided
             return session
```

### Comparing `twitter-api-client-0.8.8/twitter/constants.py` & `twitter-api-client-0.8.9/twitter/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 from dataclasses import dataclass
-import logging
-import logging.config
 
 MAX_IMAGE_SIZE = 5_242_880  # ~5 MB
 MAX_GIF_SIZE = 15_728_640  # ~15 MB
 MAX_VIDEO_SIZE = 536_870_912  # ~530 MB
 
 UPLOAD_CHUNK_SIZE = 4 * 1024 * 1024
 MEDIA_UPLOAD_SUCCEED = 'succeeded'
@@ -17,29 +15,16 @@
 BLUE = '\x1b[34m'
 MAGENTA = '\x1b[35m'
 CYAN = '\x1b[36m'
 WHITE = '\x1b[37m'
 BOLD = '\x1b[1m'
 RESET = '\x1b[0m'
 
-DISABLE_LOG_PROPAGATION = [
-    'httpx',
-    'httpcore',
-    'aiofiles',
-    'websockets',
-    'nest_asyncio',
-    'orjson',
-    'tqdm',
-    'bcrypt',
-    'python-gnupg',
-    'pyopenssl',
-    'uvloop',
-]
-
-LOG_CONFIG = {
+LOGGER_NAME = 'twitter'
+LOGGER_CONFIG = {
     'version': 1,
     'disable_existing_loggers': False,
     'formatters': {
         'standard': {
             'format': '%(asctime)s.%(msecs)03d [%(levelname)s] :: %(message)s',
             'datefmt': '%Y-%m-%d %H:%M:%S'
         },
@@ -55,26 +40,20 @@
             'class': 'logging.FileHandler',
             'level': 'DEBUG',
             'formatter': 'standard',
             'filename': 'log.log',
             'mode': 'a',
         },
     },
-    'root': {
-        'handlers': ['console', 'file'],
-        'level': 'DEBUG',
-    },
     'loggers': {
-        pkg: {
+        LOGGER_NAME: {
             'handlers': ['console', 'file'],
-            'level': 'WARNING',
-            'propagate': False
+            'level': 'DEBUG',
         }
-        for pkg in DISABLE_LOG_PROPAGATION
-    },
+    }
 }
 
 
 @dataclass
 class SpaceCategory:
     Top = 'Top'
     Live = 'Live'
```

### Comparing `twitter-api-client-0.8.8/twitter/login.py` & `twitter-api-client-0.8.9/twitter/login.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.8/twitter/scraper.py` & `twitter-api-client-0.8.9/twitter/scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -600,16 +600,22 @@
         return asyncio.run(process(spaces))
 
     @staticmethod
     def init_logger(cfg: dict) -> Logger:
         if cfg:
             logging.config.dictConfig(cfg)
         else:
-            logging.config.dictConfig(LOG_CONFIG)
-        return logging.getLogger(__name__)
+            logging.config.dictConfig(LOGGER_CONFIG)
+
+        # Set level of all other loggers to ERROR
+        for name in logging.root.manager.loggerDict:
+            if name != LOGGER_NAME:
+                logging.getLogger(name).setLevel(logging.ERROR)
+
+        return logging.getLogger(LOGGER_NAME)
 
     def validate_session(self, *args, **kwargs):
         email, username, password, session = args
         if session and all(session.cookies.get(c) for c in {'ct0', 'auth_token'}):
             # authenticated session provided
             return session
         if not session:
```

### Comparing `twitter-api-client-0.8.8/twitter/search.py` & `twitter-api-client-0.8.9/twitter/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,16 +135,22 @@
         return p
 
     @staticmethod
     def init_logger(cfg: dict) -> Logger:
         if cfg:
             logging.config.dictConfig(cfg)
         else:
-            logging.config.dictConfig(LOG_CONFIG)
-        return logging.getLogger(__name__)
+            logging.config.dictConfig(LOGGER_CONFIG)
+
+        # Set level of all other loggers to ERROR
+        for name in logging.root.manager.loggerDict:
+            if name != LOGGER_NAME:
+                logging.getLogger(name).setLevel(logging.ERROR)
+
+        return logging.getLogger(LOGGER_NAME)
 
     @staticmethod
     def validate_session(*args, **kwargs):
         email, username, password, session = args
         if session and all(session.cookies.get(c) for c in {'ct0', 'auth_token'}):
             # authenticated session provided
             return session
```

### Comparing `twitter-api-client-0.8.8/twitter/util.py` & `twitter-api-client-0.8.9/twitter/util.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.8/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.8.9/twitter_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.8.8
+Version: 0.8.9
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
```

