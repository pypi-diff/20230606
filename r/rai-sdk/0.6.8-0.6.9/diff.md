# Comparing `tmp/rai-sdk-0.6.8.tar.gz` & `tmp/rai-sdk-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rai-sdk-0.6.8.tar", last modified: Wed Sep  7 13:21:17 2022, max compression
+gzip compressed data, was "rai-sdk-0.6.9.tar", last modified: Tue Apr 11 10:26:57 2023, max compression
```

## Comparing `rai-sdk-0.6.8.tar` & `rai-sdk-0.6.9.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 13:21:17.006476 rai-sdk-0.6.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-09-07 13:21:06.000000 rai-sdk-0.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      744 2022-09-07 13:21:17.006476 rai-sdk-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3325 2022-09-07 13:21:06.000000 rai-sdk-0.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 13:21:17.002476 rai-sdk-0.6.8/rai_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      744 2022-09-07 13:21:16.000000 rai-sdk-0.6.8/rai_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-09-07 13:21:17.000000 rai-sdk-0.6.8/rai_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-07 13:21:16.000000 rai-sdk-0.6.8/rai_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-09-07 13:21:16.000000 rai-sdk-0.6.8/rai_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-09-07 13:21:16.000000 rai-sdk-0.6.8/rai_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 13:21:17.006476 rai-sdk-0.6.8/railib/
--rw-r--r--   0 runner    (1001) docker     (121)      663 2022-09-07 13:21:06.000000 rai-sdk-0.6.8/railib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25761 2022-09-07 13:21:06.000000 rai-sdk-0.6.8/railib/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     3172 2022-09-07 13:21:06.000000 rai-sdk-0.6.8/railib/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1955 2022-09-07 13:21:06.000000 rai-sdk-0.6.8/railib/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 13:21:17.006476 rai-sdk-0.6.8/railib/pb/
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-09-07 13:21:06.000000 rai-sdk-0.6.8/railib/pb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1914 2022-09-07 13:21:06.000000 rai-sdk-0.6.8/railib/pb/message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     7324 2022-09-07 13:21:06.000000 rai-sdk-0.6.8/railib/pb/schema_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     8570 2022-09-07 13:21:06.000000 rai-sdk-0.6.8/railib/rest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3559 2022-09-07 13:21:06.000000 rai-sdk-0.6.8/railib/show.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-07 13:21:17.006476 rai-sdk-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1638 2022-09-07 13:21:06.000000 rai-sdk-0.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:26:57.323157 rai-sdk-0.6.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 10:26:49.000000 rai-sdk-0.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-11 10:26:57.323157 rai-sdk-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-11 10:26:49.000000 rai-sdk-0.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:26:57.319157 rai-sdk-0.6.9/rai_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-11 10:26:57.000000 rai-sdk-0.6.9/rai_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-11 10:26:57.000000 rai-sdk-0.6.9/rai_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:26:57.000000 rai-sdk-0.6.9/rai_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-11 10:26:57.000000 rai-sdk-0.6.9/rai_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 10:26:57.000000 rai-sdk-0.6.9/rai_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:26:57.323157 rai-sdk-0.6.9/railib/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-11 10:26:49.000000 rai-sdk-0.6.9/railib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28280 2023-04-11 10:26:49.000000 rai-sdk-0.6.9/railib/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-11 10:26:49.000000 rai-sdk-0.6.9/railib/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-11 10:26:49.000000 rai-sdk-0.6.9/railib/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:26:57.323157 rai-sdk-0.6.9/railib/pb/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-11 10:26:49.000000 rai-sdk-0.6.9/railib/pb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-11 10:26:49.000000 rai-sdk-0.6.9/railib/pb/message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-04-11 10:26:49.000000 rai-sdk-0.6.9/railib/pb/schema_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-04-11 10:26:49.000000 rai-sdk-0.6.9/railib/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-04-11 10:26:49.000000 rai-sdk-0.6.9/railib/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 10:26:57.323157 rai-sdk-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-11 10:26:49.000000 rai-sdk-0.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:26:57.323157 rai-sdk-0.6.9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-11 10:26:49.000000 rai-sdk-0.6.9/test/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-11 10:26:49.000000 rai-sdk-0.6.9/test/test_unit.py
```

### Comparing `rai-sdk-0.6.8/LICENSE` & `rai-sdk-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rai-sdk-0.6.8/PKG-INFO` & `rai-sdk-0.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rai-sdk
-Version: 0.6.8
+Version: 0.6.9
 Summary: The RelationalAI Software Development Kit for Python
 Home-page: http://github.com/RelationalAI/rai-sdk-python
 Author: RelationalAI, Inc.
 Author-email: support@relational.ai
 License: http://www.apache.org/licenses/LICENSE-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rai-sdk-0.6.8/README.md` & `rai-sdk-0.6.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -111,7 +111,8 @@
 to submit an issue or a PR here.
 
 ## License
 
 The RelationalAI Software Development Kit for Python is licensed under the
 Apache License 2.0. See:
 https://github.com/RelationalAI/rai-sdk-python/blob/master/LICENSE
+
```

### Comparing `rai-sdk-0.6.8/rai_sdk.egg-info/PKG-INFO` & `rai-sdk-0.6.9/rai_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rai-sdk
-Version: 0.6.8
+Version: 0.6.9
 Summary: The RelationalAI Software Development Kit for Python
 Home-page: http://github.com/RelationalAI/rai-sdk-python
 Author: RelationalAI, Inc.
 Author-email: support@relational.ai
 License: http://www.apache.org/licenses/LICENSE-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rai-sdk-0.6.8/railib/__init__.py` & `rai-sdk-0.6.9/railib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version_info__ = (0, 6, 8)
+__version_info__ = (0, 6, 9)
 __version__ = ".".join(map(str, __version_info__))
```

### Comparing `rai-sdk-0.6.8/railib/api.py` & `rai-sdk-0.6.9/railib/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 """Operation level interface to the RelationalAI REST API."""
 
 import json
 import pyarrow as pa
 import time
 import re
 import io
+import logging
 from enum import Enum, unique
 from typing import List, Union
 from requests_toolbelt import multipart
 from . import rest
 
 from .pb.message_pb2 import MetadataInfo
 
@@ -30,14 +31,17 @@
 PATH_ENGINE = "/compute"
 PATH_DATABASE = "/database"
 PATH_TRANSACTION = "/transaction"
 PATH_TRANSACTIONS = "/transactions"
 PATH_USER = "/users"
 PATH_OAUTH_CLIENT = "/oauth-clients"
 
+# logger
+logger = logging.getLogger(__package__)
+
 
 # Engine sizes
 @unique
 class EngineSize(str, Enum):
     XS = "XS"
     S = "S"
     M = "M"
@@ -67,14 +71,19 @@
 @unique
 class Permission(str, Enum):
     # computes
     CREATE_COMPUTE = "create:compute"
     DELETE_COMPUTE = "delete:compute"
     LIST_COMPUTES = "list:compute"
     READ_COMPUTE = "read:compute"
+    # engines (duplicate to computes)
+    CREATE_ENGINE = "create:engine"
+    DELETE_ENGINE = "delete:engine"
+    LIST_ENGINES = "list:engine"
+    READ_ENGINE = "read:engine"
     # databases
     LIST_DATABASES = "list:database"
     UPDATE_DATABASE = "update:database"
     DELETE_DATABASE = "delete:database"
     # transactions
     RUN_TRANSACTION = "run:transaction"
     READ_TRANSACTION = "read:transaction"
@@ -321,145 +330,191 @@
         with pa.ipc.open_stream(file.content) as reader:
             schema = reader.schema
             batches = [batch for batch in reader]
             table = pa.Table.from_batches(batches=batches, schema=schema)
             results.append({"relationId": file.name, "table": table})
     return results
 
+# polling with specified overhead
+# delay is the overhead % of the time the transaction has been running so far
+
+
+def poll_with_specified_overhead(
+    f,
+    overhead_rate: float,
+    start_time: int = time.time(),
+    timeout: int = None,
+    max_tries: int = None,
+    max_delay: int = 120,
+):
+    tries = 0
+    max_time = time.time() + timeout if timeout else None
+
+    while True:
+        if f():
+            break
+
+        if max_tries is not None and tries >= max_tries:
+            raise Exception(f'max tries {max_tries} exhausted')
+
+        if max_time is not None and time.time() >= max_time:
+            raise Exception(f'timed out after {timeout} seconds')
+
+        tries += 1
+        duration = min((time.time() - start_time) * overhead_rate, max_delay)
+        if tries == 1:
+            time.sleep(0.5)
+        else:
+            time.sleep(duration)
+
+
+def is_engine_term_state(state: str) -> bool:
+    return state == "PROVISIONED" or ("FAILED" in state)
 
-def create_engine(ctx: Context, engine: str, size: EngineSize = EngineSize.XS):
+
+def create_engine(ctx: Context, engine: str, size: EngineSize = EngineSize.XS, **kwargs):
     data = {"region": ctx.region, "name": engine, "size": size.value}
     url = _mkurl(ctx, PATH_ENGINE)
-    rsp = rest.put(ctx, url, data)
+    rsp = rest.put(ctx, url, data, **kwargs)
     return json.loads(rsp.read())
 
 
-def create_user(ctx: Context, email: str, roles: List[Role] = None):
+def create_engine_wait(ctx: Context, engine: str, size: EngineSize = EngineSize.XS, **kwargs):
+    create_engine(ctx, engine, size, **kwargs)
+    poll_with_specified_overhead(
+        lambda: is_engine_term_state(get_engine(ctx, engine)["state"]),
+        overhead_rate=0.2,
+        timeout=30 * 60,
+    )
+    return get_engine(ctx, engine)
+
+
+def create_user(ctx: Context, email: str, roles: List[Role] = None, **kwargs):
     rs = roles or []
     data = {"email": email, "roles": [r.value for r in rs]}
     url = _mkurl(ctx, PATH_USER)
-    rsp = rest.post(ctx, url, data)
+    rsp = rest.post(ctx, url, data, **kwargs)
     return json.loads(rsp.read())
 
 
-def create_oauth_client(ctx: Context, name: str, permissions: List[Permission] = None):
+def create_oauth_client(ctx: Context, name: str, permissions: List[Permission] = None, **kwargs):
     ps = permissions or []
     data = {"name": name, "permissions": ps}
     url = _mkurl(ctx, PATH_OAUTH_CLIENT)
-    rsp = rest.post(ctx, url, data)
+    rsp = rest.post(ctx, url, data, **kwargs)
     return json.loads(rsp.read())["client"]
 
 
 # Derives the database open_mode based on the given arguments.
 def _create_mode(source_database: str, overwrite: bool) -> Mode:
     if source_database is not None:
         result = Mode.CLONE_OVERWRITE if overwrite else Mode.CLONE
     else:
         result = Mode.CREATE_OVERWRITE if overwrite else Mode.CREATE
     return result
 
 
-def delete_database(ctx: Context, database: str) -> dict:
+def delete_database(ctx: Context, database: str, **kwargs) -> dict:
     data = {"name": database}
     url = _mkurl(ctx, PATH_DATABASE)
-    rsp = rest.delete(ctx, url, data)
+    rsp = rest.delete(ctx, url, data, **kwargs)
     return json.loads(rsp.read())
 
 
-def delete_engine(ctx: Context, engine: str) -> dict:
+def delete_engine(ctx: Context, engine: str, **kwargs) -> dict:
     data = {"name": engine}
     url = _mkurl(ctx, PATH_ENGINE)
-    rsp = rest.delete(ctx, url, data)
+    rsp = rest.delete(ctx, url, data, **kwargs)
     return json.loads(rsp.read())
 
 
-def delete_user(ctx: Context, id: str) -> dict:
+def delete_user(ctx: Context, id: str, **kwargs) -> dict:
     url = _mkurl(ctx, f"{PATH_USER}/{id}")
-    rsp = rest.delete(ctx, url, None)
+    rsp = rest.delete(ctx, url, None, **kwargs)
     return json.loads(rsp.read())
 
 
-def disable_user(ctx: Context, userid: str) -> dict:
-    return update_user(ctx, userid, status="INACTIVE")
+def disable_user(ctx: Context, userid: str, **kwargs) -> dict:
+    return update_user(ctx, userid, status="INACTIVE", **kwargs)
 
 
-def delete_oauth_client(ctx: Context, id: str) -> dict:
+def delete_oauth_client(ctx: Context, id: str, **kwargs) -> dict:
     url = _mkurl(ctx, f"{PATH_OAUTH_CLIENT}/{id}")
-    rsp = rest.delete(ctx, url, None)
+    rsp = rest.delete(ctx, url, None, **kwargs)
     return json.loads(rsp.read())
 
 
-def enable_user(ctx: Context, userid: str) -> dict:
-    return update_user(ctx, userid, status="ACTIVE")
+def enable_user(ctx: Context, userid: str, **kwargs) -> dict:
+    return update_user(ctx, userid, status="ACTIVE", **kwargs)
 
 
-def get_engine(ctx: Context, engine: str) -> dict:
-    return _get_resource(ctx, PATH_ENGINE, name=engine, deleted_on="", key="computes")
+def get_engine(ctx: Context, engine: str, **kwargs) -> dict:
+    return _get_resource(ctx, PATH_ENGINE, name=engine, deleted_on="", key="computes", **kwargs)
 
 
-def get_database(ctx: Context, database: str) -> dict:
-    return _get_resource(ctx, PATH_DATABASE, name=database, key="databases")
+def get_database(ctx: Context, database: str, **kwargs) -> dict:
+    return _get_resource(ctx, PATH_DATABASE, name=database, key="databases", **kwargs)
 
 
-def get_oauth_client(ctx: Context, id: str) -> dict:
-    return _get_resource(ctx, f"{PATH_OAUTH_CLIENT}/{id}", key="client")
+def get_oauth_client(ctx: Context, id: str, **kwargs) -> dict:
+    return _get_resource(ctx, f"{PATH_OAUTH_CLIENT}/{id}", key="client", **kwargs)
 
 
-def get_transaction(ctx: Context, id: str) -> dict:
-    return _get_resource(ctx, f"{PATH_TRANSACTIONS}/{id}", key="transaction")
+def get_transaction(ctx: Context, id: str, **kwargs) -> dict:
+    return _get_resource(ctx, f"{PATH_TRANSACTIONS}/{id}", key="transaction", **kwargs)
 
 
-def get_transaction_metadata(ctx: Context, id: str) -> list:
+def get_transaction_metadata(ctx: Context, id: str, **kwargs) -> list:
     headers = {"Accept": "application/x-protobuf"}
     url = _mkurl(ctx, f"{PATH_TRANSACTIONS}/{id}/metadata")
-    rsp = rest.get(ctx, url, headers=headers)
+    rsp = rest.get(ctx, url, headers=headers, **kwargs)
     content_type = rsp.headers.get("content-type", "")
     if "application/x-protobuf" in content_type:
         return _parse_metadata_proto(rsp.read())
 
     raise Exception(f"invalid content type for metadata proto: {content_type}")
 
 
-def list_transactions(ctx: Context) -> list:
-    return _get_collection(ctx, PATH_TRANSACTIONS, key="transactions")
+def list_transactions(ctx: Context, **kwargs) -> list:
+    return _get_collection(ctx, PATH_TRANSACTIONS, key="transactions", **kwargs)
 
 
-def get_transaction_problems(ctx: Context, id: str) -> list:
-    return _get_collection(ctx, f"{PATH_TRANSACTIONS}/{id}/problems")
+def get_transaction_problems(ctx: Context, id: str, **kwargs) -> list:
+    return _get_collection(ctx, f"{PATH_TRANSACTIONS}/{id}/problems", **kwargs)
 
 
-def get_transaction_results(ctx: Context, id: str) -> list:
+def get_transaction_results(ctx: Context, id: str, **kwargs) -> list:
     url = _mkurl(ctx, f"{PATH_TRANSACTIONS}/{id}/results")
-    rsp = rest.get(ctx, url)
+    rsp = rest.get(ctx, url, **kwargs)
     content_type = rsp.headers.get("content-type", "")
     if "multipart/form-data" in content_type:
         parts = _parse_multipart_form(content_type, rsp.read())
         return _parse_arrow_results(parts)
 
     raise Exception("invalid response type")
 
 
 # When problems are part of the results relations, this function should be
 # deprecated, get_transaction_results should be called instead
 
 
-def get_transaction_results_and_problems(ctx: Context, id: str) -> list:
+def get_transaction_results_and_problems(ctx: Context, id: str, **kwargs) -> list:
     rsp = TransactionAsyncResponse()
-    rsp.problems = get_transaction_problems(ctx, id)
-    rsp.results = get_transaction_results(ctx, id)
+    rsp.problems = get_transaction_problems(ctx, id, **kwargs)
+    rsp.results = get_transaction_results(ctx, id, **kwargs)
     return rsp
 
 
-def cancel_transaction(ctx: Context, id: str) -> dict:
-    rsp = rest.post(ctx, _mkurl(ctx, f"{PATH_TRANSACTIONS}/{id}/cancel"), {})
+def cancel_transaction(ctx: Context, id: str, **kwargs) -> dict:
+    rsp = rest.post(ctx, _mkurl(ctx, f"{PATH_TRANSACTIONS}/{id}/cancel"), {}, **kwargs)
     return json.loads(rsp.read())
 
 
-def get_user(ctx: Context, userid: str) -> dict:
-    return _get_resource(ctx, f"{PATH_USER}/{userid}", name=userid)
+def get_user(ctx: Context, userid: str, **kwargs) -> dict:
+    return _get_resource(ctx, f"{PATH_USER}/{userid}", name=userid, **kwargs)
 
 
 def list_engines(ctx: Context, state=None) -> list:
     kwargs = {}
     if state is not None:
         kwargs["state"] = state
     return _get_collection(ctx, PATH_ENGINE, key="computes", **kwargs)
@@ -468,30 +523,30 @@
 def list_databases(ctx: Context, state=None) -> list:
     kwargs = {}
     if state is not None:
         kwargs["state"] = state
     return _get_collection(ctx, PATH_DATABASE, key="databases", **kwargs)
 
 
-def list_users(ctx: Context) -> list:
-    return _get_collection(ctx, PATH_USER, key="users")
+def list_users(ctx: Context, **kwargs) -> list:
+    return _get_collection(ctx, PATH_USER, key="users", **kwargs)
 
 
-def list_oauth_clients(ctx: Context) -> list:
-    return _get_collection(ctx, PATH_OAUTH_CLIENT, key="clients")
+def list_oauth_clients(ctx: Context, **kwargs) -> list:
+    return _get_collection(ctx, PATH_OAUTH_CLIENT, key="clients", **kwargs)
 
 
-def update_user(ctx: Context, userid: str, status: str = None, roles=None):
+def update_user(ctx: Context, userid: str, status: str = None, roles=None, **kwargs):
     data = {}
     if status is not None:
         data["status"] = status
     if roles is not None:
         data["roles"] = roles
     url = _mkurl(ctx, f"{PATH_USER}/{userid}")
-    rsp = rest.patch(ctx, url, data)
+    rsp = rest.patch(ctx, url, data, **kwargs)
     return json.loads(rsp.read())
 
 
 class Transaction(object):
     def __init__(
         self,
         database: str,
@@ -574,21 +629,22 @@
             "readonly": self.readonly,
             # "sync_mode": "async"
         }
         if self.engine is not None:
             result["engine_name"] = self.engine
         return result
 
-    def run(self, ctx: Context, command: str, inputs: dict = None) -> Union[dict, list]:
+    def run(self, ctx: Context, command: str, language: str, inputs: dict = None, **kwargs) -> Union[dict, list]:
         data = self.data
         data["query"] = command
+        data["language"] = language
         if inputs is not None:
             inputs = [_query_action_input(k, v) for k, v in inputs.items()]
             data["v1_inputs"] = inputs
-        rsp = rest.post(ctx, _mkurl(ctx, PATH_TRANSACTIONS), data)
+        rsp = rest.post(ctx, _mkurl(ctx, PATH_TRANSACTIONS), data, **kwargs)
         content_type = rsp.headers.get("content-type", None)
         content = rsp.read()
         # todo: response model should be based on status code (200 v. 201)
         # async mode
         if content_type.lower() == "application/json":
             return json.loads(content)
         # sync mode
@@ -663,18 +719,18 @@
     actions = rsp["actions"]
     assert len(actions) == 1
     action = actions[0]
     models = action["result"]["sources"]
     return models
 
 
-def create_database(ctx: Context, database: str, source: str = None) -> dict:
+def create_database(ctx: Context, database: str, source: str = None, **kwargs) -> dict:
     data = {"name": database, "source_name": source}
     url = _mkurl(ctx, PATH_DATABASE)
-    rsp = rest.put(ctx, url, data)
+    rsp = rest.put(ctx, url, data, **kwargs)
     return json.loads(rsp.read())
 
 
 def delete_model(ctx: Context, database: str, engine: str, model: str) -> dict:
     tx = Transaction(database, engine, mode=Mode.OPEN, readonly=False)
     actions = [_delete_model_action(model)]
     return tx.run(ctx, *actions)
@@ -829,46 +885,56 @@
 def exec(
     ctx: Context,
     database: str,
     engine: str,
     command: str,
     inputs: dict = None,
     readonly: bool = True,
+    **kwargs
 ) -> TransactionAsyncResponse:
+    logger.info('exec: database %s engine %s readonly %s' % (database, engine, readonly))
+    start_time = time.time()
     txn = exec_async(ctx, database, engine, command, inputs=inputs, readonly=readonly)
     # in case of if short-path, return results directly, no need to poll for
     # state
     if not (txn.results is None):
+        logger.info('transaction id: %s' % txn.transaction["id"])
         return txn
 
     rsp = TransactionAsyncResponse()
-    txn = get_transaction(ctx, txn.transaction["id"])
-    while True:
-        time.sleep(1)
-        txn = get_transaction(ctx, txn["id"])
-        if is_txn_term_state(txn["state"]):
-            rsp.transaction = txn
-            rsp.metadata = get_transaction_metadata(ctx, txn["id"])
-            rsp.problems = get_transaction_problems(ctx, txn["id"])
-            rsp.results = get_transaction_results(ctx, txn["id"])
-            break
+    txn = get_transaction(ctx, txn.transaction["id"], **kwargs)
+
+    poll_with_specified_overhead(
+        lambda: is_txn_term_state(get_transaction(ctx, txn["id"], **kwargs)["state"]),
+        overhead_rate=0.2,
+        start_time=start_time,
+    )
+
+    logger.info('transaction id: %s' % txn["id"])
+
+    rsp.transaction = get_transaction(ctx, txn["id"], **kwargs)
+    rsp.metadata = get_transaction_metadata(ctx, txn["id"], **kwargs)
+    rsp.problems = get_transaction_problems(ctx, txn["id"], **kwargs)
+    rsp.results = get_transaction_results(ctx, txn["id"], **kwargs)
 
     return rsp
 
 
 def exec_async(
     ctx: Context,
     database: str,
     engine: str,
     command: str,
     readonly: bool = True,
     inputs: dict = None,
+    language: str = "",
+    **kwargs,
 ) -> TransactionAsyncResponse:
     tx = TransactionAsync(database, engine, readonly=readonly)
-    rsp = tx.run(ctx, command, inputs=inputs)
+    rsp = tx.run(ctx, command, language=language, inputs=inputs, **kwargs)
 
     if isinstance(rsp, dict):
         return TransactionAsyncResponse(rsp, None, None, None)
 
     return _parse_transaction_async_response(rsp)
```

### Comparing `rai-sdk-0.6.8/railib/config.py` & `rai-sdk-0.6.9/railib/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,51 +15,29 @@
 """Reads the RAI SDK config file."""
 
 # Note, the SDK config reader is here for convenience and its use is strictly
 # optional. Many clients will chose to use other methods for managing settings
 # and client credentials.
 
 import configparser
-import json
 import os
 from pathlib import Path
 
-from .credentials import AccessKeyCredentials, ClientCredentials
+from .credentials import ClientCredentials
 
 
 def _read_config_profile(fname: str, profile: str) -> dict:
     config = configparser.ConfigParser()
     config.read(fname)
     if profile not in config:
         fname = os.path.basename(fname)
         raise Exception(f"profile '{profile}' not found in {fname}")
     return {k: config[profile][k] for k in config[profile]}
 
 
-def _read_pkey(fname: Path):
-    with open(fname) as fp:
-        data = json.load(fp)
-        pkey = data.get("sodium", {}).get("seed", None)
-        if pkey is None:
-            raise Exception("malformed private key")
-        return pkey
-
-
-# Reads access key credentials from the config file. Returns None if they
-# do not exist.
-def _read_access_key_credentials(data, path: Path):
-    akey = data.get("access_key", None)
-    if akey is not None:
-        fname = data.get("private_key_filename", None)
-        if fname is not None:
-            pkey = _read_pkey(path.with_name(fname))
-            return AccessKeyCredentials(akey, pkey)
-    return None
-
-
 # Read client credentials from the config file. Returns None if they do not
 # exist.
 def _read_client_credentials(data):
     client_id = data.get("client_id", None)
     if client_id is not None:
         client_secret = data.get("client_secret", None)
         if client_secret is not None:
@@ -68,16 +46,14 @@
     return None
 
 
 # Reads credentails from config file, preferring client credentials
 # if they exist. Returns None if no credentials exist.
 def _read_credentials(data, path):
     creds = _read_client_credentials(data)
-    if creds is None:
-        creds = _read_access_key_credentials(data, path)
     return creds
 
 
 # Returns settings from config file.
 def read(fname: str = "~/.rai/config", profile: str = "default"):
     path = Path(fname).expanduser()
     if not path.is_file():
```

### Comparing `rai-sdk-0.6.8/railib/credentials.py` & `rai-sdk-0.6.9/railib/credentials.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,40 +14,33 @@
 
 from abc import ABC
 import time
 
 
 __all__ = [
     "Credentials",
-    "AccessKeyCredentials",
     "AccessToken",
     "ClientCredentials",
 ]
 
 DEFAULT_CLIENT_CREDENTIALS_URL = "https://login.relationalai.com/oauth/token"
 
 
 # Abstract base class shared by all credential types supported by railib.
 class Credentials(ABC):
     pass
 
 
-# Represents access key credentials.
-class AccessKeyCredentials(Credentials):
-    def __init__(self, akey: str, pkey: str):
-        self.akey = akey  # access_key
-        self.pkey = pkey  # private_key
-
-
 # Represents an OAuth access token.
 class AccessToken:
-    def __init__(self, access_token: str, expires_in: int):
-        self.token = access_token
+    def __init__(self, access_token: str, scope: str, expires_in: int, created_on: float = time.time()):
+        self.access_token = access_token
+        self.scope = scope
         self.expires_in = expires_in
-        self.created_on = round(time.time())
+        self.created_on = created_on
 
     def is_expired(self):
         return (
             time.time() - self.created_on >= self.expires_in - 5
         )  # anticipate token expiration by 5 seconds
```

### Comparing `rai-sdk-0.6.8/railib/pb/message_pb2.py` & `rai-sdk-0.6.9/railib/pb/message_pb2.py`

 * *Files identical despite different names*

### Comparing `rai-sdk-0.6.8/railib/pb/schema_pb2.py` & `rai-sdk-0.6.9/railib/pb/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `rai-sdk-0.6.8/railib/rest.py` & `rai-sdk-0.6.9/railib/rest.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,25 +10,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Low level HTTP interface to the RelationalAI REST API."""
 
-import ed25519
-import base64
-from datetime import datetime
-import hashlib
 import json
+import logging
+from os import path
 from urllib.parse import urlencode, urlsplit, quote
 from urllib.request import Request, urlopen
 
 from .__init__ import __version__
 from .credentials import (
-    AccessKeyCredentials,
     AccessToken,
     Credentials,
     ClientCredentials,
 )
 
 __all__ = ["Context", "get", "put", "post", "request"]
 
@@ -36,17 +33,18 @@
 ACCESS_KEY_TOKEN_KEY = "access_token"
 CLIENT_ID_KEY = "client_id"
 CLIENT_SECRET_KEY = "client_secret"
 AUDIENCE_KEY = "audience"
 GRANT_TYPE_KEY = "grant_type"
 CLIENT_CREDENTIALS_KEY = "client_credentials"
 EXPIRES_IN_KEY = "expires_in"
+SCOPE = "scope"
 
-
-_empty = bytes("", encoding="utf8")
+# logger
+logger = logging.getLogger(__package__)
 
 
 # Context contains the state required to make rAI REST API calls.
 class Context(object):
     def __init__(self, region: str = None, credentials: Credentials = None):
         self.region = region or "us-east"
         self.credentials = credentials
@@ -115,21 +113,58 @@
         if level > 1:
             for k, v in req.headers.items():
                 print(f"{k}: {v}")
             if req.data:
                 print(json.dumps(json.loads(req.data.decode("utf8")), indent=2))
 
 
+def _cache_file() -> str:
+    return path.join(path.expanduser('~'), '.rai', 'tokens.json')
+
+
+# Read oauth cache
+def _read_cache() -> dict:
+    try:
+        with open(_cache_file(), 'r') as cache:
+            return json.loads(cache.read())
+    except Exception:
+        return {}
+
+
+# Read access token from cache
+def _read_token_cache(creds: ClientCredentials) -> AccessToken:
+    try:
+        cache = _read_cache()
+        return AccessToken(**cache[creds.client_id])
+    except Exception:
+        return None
+
+
+# write access token to cache
+def _write_token_cache(creds: ClientCredentials):
+    try:
+        cache = _read_cache()
+        cache[creds.client_id] = creds.access_token
+
+        with open(_cache_file(), 'w') as f:
+            f.write(json.dumps(cache, default=vars))
+    except Exception:
+        pass
+
+
 # Returns the current access token if valid, otherwise requests new token.
 def _get_access_token(ctx: Context, url: str) -> AccessToken:
     creds = ctx.credentials
     assert isinstance(creds, ClientCredentials)
     if creds.access_token is None or creds.access_token.is_expired():
-        creds.access_token = _request_access_token(ctx, url)
-    return creds.access_token.token
+        creds.access_token = _read_token_cache(creds)
+        if creds.access_token is None or creds.access_token.is_expired():
+            creds.access_token = _request_access_token(ctx, url)
+            _write_token_cache(creds)
+    return creds.access_token.access_token
 
 
 def _request_access_token(ctx: Context, url: str) -> AccessToken:
     creds = ctx.credentials
     assert isinstance(creds, ClientCredentials)
     # ensure the audience contains the protocol scheme
     audience = ctx.audience or f"https://{_get_host(url)}"
@@ -154,100 +189,48 @@
     )
     _print_request(req)
     with urlopen(req) as rsp:
         result = json.loads(rsp.read())
         token = result.get(ACCESS_KEY_TOKEN_KEY, None)
         if token is not None:
             expires_in = result.get(EXPIRES_IN_KEY, None)
-            return AccessToken(token, expires_in)
+            scope = result.get(SCOPE, None)
+            return AccessToken(token, scope, expires_in)
     raise Exception("failed to get the access token")
 
 
-# Implement RAI API key authentication by signing the request and adding the
-# required authorization header.
-def _sign(ctx: Context, req: Request) -> None:
-    assert isinstance(ctx.credentials, AccessKeyCredentials)
-
-    ts = datetime.utcnow()
-
-    # ISO8601 date/time strings for time of request
-    signature_date = ts.strftime("%Y%m%dT%H%M%SZ")
-    scope_date = ts.strftime("%Y%m%d")
-
-    # Authentication scope
-    scope = f"{scope_date}/{ctx.region}/{ctx.service}/rai01_request"
-
-    # SHA256 hash of content
-    content = req.data or _empty
-    content_hash = hashlib.sha256(content).hexdigest()
-
-    # Include "x-rai-date" in signed headers
-    req.headers["x-rai-date"] = signature_date
-
-    # Sort and lowercase headers to produce a canonical form
-    canonical_headers = sorted(
-        [f"{k.lower()}:{v.strip()}" for k, v in req.headers.items()]
-    )
-
-    h_names = sorted([k.lower() for k in req.headers])
-    signed_headers = ";".join(h_names)
-
-    # Create hash of canonical request
-    split_result = urlsplit(req.full_url)  # was self.url
-    canonical_form = "{}\n{}\n{}\n{}\n\n{}\n{}".format(
-        req.method,
-        _encode_path(split_result.path),
-        split_result.query,
-        "\n".join(canonical_headers),
-        signed_headers,
-        content_hash,
-    )
-
-    canonical_hash = hashlib.sha256(canonical_form.encode("utf-8")).hexdigest()
-    # Create and sign "String to sign"
-    string_to_sign = "RAI01-ED25519-SHA256\n{}\n{}\n{}".format(
-        signature_date, scope, canonical_hash
-    )
-
-    seed = base64.b64decode(ctx.credentials.pkey)
-    signing_key = ed25519.SigningKey(seed)
-    sig = signing_key.sign(string_to_sign.encode("utf-8")).hex()
-
-    req.headers["authorization"] = (
-        "RAI01-ED25519-SHA256 Credential={}/{},"
-        "SignedHeaders={},"
-        "Signature={}".format(ctx.credentials.akey, scope, signed_headers, sig)
-    )
-
-
 # Authenticate the request by signing or adding access token.
 def _authenticate(ctx: Context, req: Request) -> Request:
     creds = ctx.credentials
     if creds is None:
         return req
     if isinstance(creds, ClientCredentials):
         access_token = _get_access_token(ctx, req.full_url)
         req.headers["authorization"] = f"Bearer {access_token}"
         return req
-    if isinstance(creds, AccessKeyCredentials):
-        _sign(ctx, req)
-        return req
     raise Exception("unknown credential type")
 
 
 # Issues an RAI REST API request, and returns response contents if successful.
 def request(ctx: Context, method: str, url: str, headers={}, data=None, **kwargs):
     headers = _default_headers(url, headers)
     if kwargs:
         url = f"{url}?{_encode_qs(kwargs)}"
     data = _encode(data)
     req = Request(method=method, url=url, headers=headers, data=data)
     req = _authenticate(ctx, req)
     _print_request(req)
-    return urlopen(req)
+    rsp = urlopen(req)
+
+    # logging
+    content_type = headers["Content-Type"] if "Content-Type" in headers else ""
+    agent = headers["User-Agent"] if "User-Agent" in headers else ""
+    request_id = rsp.headers["X-Request-ID"] if "X-Request-ID" in rsp.headers else ""
+    logger.debug(f"{rsp._method} HTTP/{rsp.version} {content_type} {rsp.url} {rsp.status} {agent} {request_id}")
+    return rsp
 
 
 def delete(ctx: Context, url: str, data, headers={}, **kwargs):
     return request(ctx, "DELETE", url, headers=headers, data=data, **kwargs)
 
 
 def get(ctx: Context, url: str, headers={}, **kwargs):
```

### Comparing `rai-sdk-0.6.8/railib/show.py` & `rai-sdk-0.6.9/railib/show.py`

 * *Files identical despite different names*

### Comparing `rai-sdk-0.6.8/setup.py` & `rai-sdk-0.6.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         "Programming Language :: Python :: 3.8",
     ],
     description="The RelationalAI Software Development Kit for Python",
     install_requires=[
         "ed25519==1.5",
         "pyarrow>=6.0.1",
         "requests-toolbelt==0.9.1",
-        "protobuf==3.20.1"],
+        "protobuf==3.20.2"],
     license="http://www.apache.org/licenses/LICENSE-2.0",
     long_description="Enables access to the RelationalAI REST APIs from Python",
     long_description_content_type="text/markdown",
     name="rai-sdk",
     packages=["railib", "railib.pb"],
     url="http://github.com/RelationalAI/rai-sdk-python",
     version=railib.__version__)
```

