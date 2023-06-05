# Comparing `tmp/twscrape-0.2.1.tar.gz` & `tmp/twscrape-0.2.2.tar.gz`

## Comparing `twscrape-0.2.1.tar` & `twscrape-0.2.2.tar`

### file list

```diff
@@ -1,41 +1,42 @@
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 twscrape-0.2.1/.gitattributes
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 twscrape-0.2.1/Makefile
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 twscrape-0.2.1/.github/CODEOWNERS
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 twscrape-0.2.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 twscrape-0.2.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 twscrape-0.2.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 twscrape-0.2.1/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/conftest.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/test_api.py
--rw-r--r--   0        0        0     7909 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/test_parser.py
--rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/test_pool.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/test_queue_client.py
--rw-r--r--   0        0        0    67646 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/mocked-data/favoriters_raw.json
--rw-r--r--   0        0        0   152580 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/mocked-data/followers_raw.json
--rw-r--r--   0        0        0   142243 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/mocked-data/following_raw.json
--rw-r--r--   0        0        0    69669 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/mocked-data/retweeters_raw.json
--rw-r--r--   0        0        0   177570 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/mocked-data/search_raw.json
--rw-r--r--   0        0        0    95327 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/mocked-data/tweet_details_raw.json
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/mocked-data/user_by_id_raw.json
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/mocked-data/user_by_login_raw.json
--rw-r--r--   0        0        0   497799 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/mocked-data/user_tweets_and_replies_raw.json
--rw-r--r--   0        0        0   496101 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/mocked-data/user_tweets_raw.json
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 twscrape-0.2.1/twscrape/__init__.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 twscrape-0.2.1/twscrape/account.py
--rw-r--r--   0        0        0     7866 2020-02-02 00:00:00.000000 twscrape-0.2.1/twscrape/accounts_pool.py
--rw-r--r--   0        0        0     9515 2020-02-02 00:00:00.000000 twscrape-0.2.1/twscrape/api.py
--rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 twscrape-0.2.1/twscrape/cli.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 twscrape-0.2.1/twscrape/constants.py
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 twscrape-0.2.1/twscrape/db.py
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 twscrape-0.2.1/twscrape/imap.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 twscrape-0.2.1/twscrape/logger.py
--rw-r--r--   0        0        0     6992 2020-02-02 00:00:00.000000 twscrape-0.2.1/twscrape/login.py
--rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 twscrape-0.2.1/twscrape/models.py
--rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 twscrape-0.2.1/twscrape/queue_client.py
--rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 twscrape-0.2.1/twscrape/utils.py
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 twscrape-0.2.1/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 twscrape-0.2.1/LICENSE
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 twscrape-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 twscrape-0.2.1/readme.md
--rw-r--r--   0        0        0     7868 2020-02-02 00:00:00.000000 twscrape-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 twscrape-0.2.2/.gitattributes
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 twscrape-0.2.2/Dockerfile-test
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 twscrape-0.2.2/Makefile
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 twscrape-0.2.2/.github/CODEOWNERS
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 twscrape-0.2.2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 twscrape-0.2.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 twscrape-0.2.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 twscrape-0.2.2/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/conftest.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/test_api.py
+-rw-r--r--   0        0        0     7909 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/test_parser.py
+-rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/test_pool.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/test_queue_client.py
+-rw-r--r--   0        0        0    67646 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/mocked-data/favoriters_raw.json
+-rw-r--r--   0        0        0   152580 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/mocked-data/followers_raw.json
+-rw-r--r--   0        0        0   142243 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/mocked-data/following_raw.json
+-rw-r--r--   0        0        0    69669 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/mocked-data/retweeters_raw.json
+-rw-r--r--   0        0        0   177570 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/mocked-data/search_raw.json
+-rw-r--r--   0        0        0    95327 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/mocked-data/tweet_details_raw.json
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/mocked-data/user_by_id_raw.json
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/mocked-data/user_by_login_raw.json
+-rw-r--r--   0        0        0   497799 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/mocked-data/user_tweets_and_replies_raw.json
+-rw-r--r--   0        0        0   496101 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/mocked-data/user_tweets_raw.json
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 twscrape-0.2.2/twscrape/__init__.py
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 twscrape-0.2.2/twscrape/account.py
+-rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 twscrape-0.2.2/twscrape/accounts_pool.py
+-rw-r--r--   0        0        0     9515 2020-02-02 00:00:00.000000 twscrape-0.2.2/twscrape/api.py
+-rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 twscrape-0.2.2/twscrape/cli.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 twscrape-0.2.2/twscrape/constants.py
+-rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 twscrape-0.2.2/twscrape/db.py
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 twscrape-0.2.2/twscrape/imap.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 twscrape-0.2.2/twscrape/logger.py
+-rw-r--r--   0        0        0     6992 2020-02-02 00:00:00.000000 twscrape-0.2.2/twscrape/login.py
+-rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 twscrape-0.2.2/twscrape/models.py
+-rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 twscrape-0.2.2/twscrape/queue_client.py
+-rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 twscrape-0.2.2/twscrape/utils.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 twscrape-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 twscrape-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 twscrape-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 twscrape-0.2.2/readme.md
+-rw-r--r--   0        0        0     7868 2020-02-02 00:00:00.000000 twscrape-0.2.2/PKG-INFO
```

### Comparing `twscrape-0.2.1/.github/workflows/publish.yml` & `twscrape-0.2.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.1/tests/conftest.py` & `twscrape-0.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.1/tests/test_api.py` & `twscrape-0.2.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.1/tests/test_parser.py` & `twscrape-0.2.2/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.1/tests/test_pool.py` & `twscrape-0.2.2/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.1/tests/test_queue_client.py` & `twscrape-0.2.2/tests/test_queue_client.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.1/tests/mocked-data/favoriters_raw.json` & `twscrape-0.2.2/tests/mocked-data/favoriters_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.1/tests/mocked-data/followers_raw.json` & `twscrape-0.2.2/tests/mocked-data/followers_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.1/tests/mocked-data/following_raw.json` & `twscrape-0.2.2/tests/mocked-data/following_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.1/tests/mocked-data/retweeters_raw.json` & `twscrape-0.2.2/tests/mocked-data/retweeters_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.1/tests/mocked-data/search_raw.json` & `twscrape-0.2.2/tests/mocked-data/search_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.1/tests/mocked-data/tweet_details_raw.json` & `twscrape-0.2.2/tests/mocked-data/tweet_details_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.1/tests/mocked-data/user_by_id_raw.json` & `twscrape-0.2.2/tests/mocked-data/user_by_id_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.1/tests/mocked-data/user_by_login_raw.json` & `twscrape-0.2.2/tests/mocked-data/user_by_login_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.1/tests/mocked-data/user_tweets_and_replies_raw.json` & `twscrape-0.2.2/tests/mocked-data/user_tweets_and_replies_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.1/tests/mocked-data/user_tweets_raw.json` & `twscrape-0.2.2/tests/mocked-data/user_tweets_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.1/twscrape/account.py` & `twscrape-0.2.2/twscrape/account.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     locks: dict[str, datetime] = field(default_factory=dict)  # queue: datetime
     stats: dict[str, int] = field(default_factory=dict)  # queue: requests
     headers: dict[str, str] = field(default_factory=dict)
     cookies: dict[str, str] = field(default_factory=dict)
     proxy: str | None = None
     error_msg: str | None = None
     last_used: datetime | None = None
+    _tx: str | None = None
 
     @staticmethod
     def from_rs(rs: sqlite3.Row):
         doc = dict(rs)
         doc["locks"] = {k: from_utciso(v) for k, v in json.loads(doc["locks"]).items()}
         doc["stats"] = {k: v for k, v in json.loads(doc["stats"]).items() if isinstance(v, int)}
         doc["headers"] = json.loads(doc["headers"])
```

### Comparing `twscrape-0.2.1/twscrape/accounts_pool.py` & `twscrape-0.2.2/twscrape/accounts_pool.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # ruff: noqa: E501
 import asyncio
+import sqlite3
+import uuid
 from datetime import datetime, timezone
 
 from fake_useragent import UserAgent
 
 from .account import Account
 from .db import execute, fetchall, fetchone
 from .logger import logger
@@ -144,21 +146,33 @@
             OR json_extract(locks, '$.{queue}') IS NULL
             OR json_extract(locks, '$.{queue}') < datetime('now')
         )
         ORDER BY RANDOM()
         LIMIT 1
         """
 
-        q2 = f"""
-        UPDATE accounts SET locks = json_set(locks, '$.{queue}', datetime('now', '+15 minutes'))
-        WHERE username = ({q1})
-        RETURNING *
-        """
+        if int(sqlite3.sqlite_version_info[1]) >= 35:
+            qs = f"""
+            UPDATE accounts SET locks = json_set(locks, '$.{queue}', datetime('now', '+15 minutes'))
+            WHERE username = ({q1})
+            RETURNING *
+            """
+            rs = await fetchone(self._db_file, qs)
+        else:
+            tx = uuid.uuid4().hex
+            qs = f"""
+            UPDATE accounts
+            SET locks = json_set(locks, '$.{queue}', datetime('now', '+15 minutes')), _tx = '{tx}'
+            WHERE username = ({q1})
+            """
+            await execute(self._db_file, qs)
+
+            qs = f"SELECT * FROM accounts WHERE _tx = '{tx}'"
+            rs = await fetchone(self._db_file, qs)
 
-        rs = await fetchone(self._db_file, q2)
         return Account.from_rs(rs) if rs else None
 
     async def get_for_queue_or_wait(self, queue: str) -> Account:
         while True:
             account = await self.get_for_queue(queue)
             if not account:
                 logger.debug(f"No accounts available for queue '{queue}' (sleeping for 5 sec)")
```

### Comparing `twscrape-0.2.1/twscrape/api.py` & `twscrape-0.2.2/twscrape/api.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.1/twscrape/cli.py` & `twscrape-0.2.2/twscrape/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 
 async def main(args):
     if args.debug:
         set_log_level("DEBUG")
 
     if args.command == "version":
         print(f"twscrape: {version('twscrape')}")
-        print(f"SQlite client: {sqlite3.version}")
-        print(f"SQlite runtime: {sqlite3.sqlite_version} ({await get_sqlite_version()})")
+        print(f"SQLite client: {sqlite3.version}")
+        print(f"SQLite runtime: {sqlite3.sqlite_version} ({await get_sqlite_version()})")
         return
 
     logger.debug(f"Using database: {args.db}")
     pool = AccountsPool(args.db)
     api = API(pool, debug=args.debug)
 
     if args.command == "accounts":
```

### Comparing `twscrape-0.2.1/twscrape/constants.py` & `twscrape-0.2.2/twscrape/constants.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.1/twscrape/db.py` & `twscrape-0.2.2/twscrape/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,17 +65,21 @@
         );"""
         await db.execute(qs)
 
     async def v2():
         await db.execute("ALTER TABLE accounts ADD COLUMN stats TEXT DEFAULT '{}' NOT NULL")
         await db.execute("ALTER TABLE accounts ADD COLUMN last_used TEXT DEFAULT NULL")
 
+    async def v3():
+        await db.execute("ALTER TABLE accounts ADD COLUMN _tx TEXT DEFAULT NULL")
+
     migrations = {
         1: v1,
         2: v2,
+        3: v3,
     }
 
     logger.debug(f"Current migration v{uv} (latest v{len(migrations)})")
 
     for i in range(uv + 1, len(migrations) + 1):
         logger.debug(f"Running migration to v{i}")
         try:
```

### Comparing `twscrape-0.2.1/twscrape/imap.py` & `twscrape-0.2.2/twscrape/imap.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.1/twscrape/login.py` & `twscrape-0.2.2/twscrape/login.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.1/twscrape/models.py` & `twscrape-0.2.2/twscrape/models.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.1/twscrape/queue_client.py` & `twscrape-0.2.2/twscrape/queue_client.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.1/twscrape/utils.py` & `twscrape-0.2.2/twscrape/utils.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.1/.gitignore` & `twscrape-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.1/LICENSE` & `twscrape-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.1/pyproject.toml` & `twscrape-0.2.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "twscrape"
-version = "0.2.1"
+version = "0.2.2"
 authors = [{name = "vladkens", email = "v.pronsky@gmail.com"}]
 description = "Twitter GraphQL and Search API implementation with SNScrape data models"
 readme = "readme.md"
 requires-python = ">=3.10"
 keywords = ["twitter", "scrape", "scrapper", "api", "snscrape"]
 license = {text = "MIT"}
 classifiers = [
```

### Comparing `twscrape-0.2.1/readme.md` & `twscrape-0.2.2/readme.md`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.1/PKG-INFO` & `twscrape-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twscrape
-Version: 0.2.1
+Version: 0.2.2
 Summary: Twitter GraphQL and Search API implementation with SNScrape data models
 Project-URL: repository, https://github.com/vladkens/twscrape
 Author-email: vladkens <v.pronsky@gmail.com>
 License: MIT
 License-File: LICENSE
 Keywords: api,scrape,scrapper,snscrape,twitter
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: twscrape Version: 0.2.1 Summary: Twitter GraphQL
+Metadata-Version: 2.1 Name: twscrape Version: 0.2.2 Summary: Twitter GraphQL
 and Search API implementation with SNScrape data models Project-URL:
 repository, https://github.com/vladkens/twscrape Author-email: vladkens
 pronsky@gmail.com> License: MIT License-File: LICENSE Keywords:
 api,scrape,scrapper,snscrape,twitter Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10 Requires-Dist: aiosqlite==0.17.0 Requires-Dist: fake-
```

