# Comparing `tmp/formic_opcua-1.4.0.tar.gz` & `tmp/formic_opcua-1.5.0.tar.gz`

## Comparing `formic_opcua-1.4.0.tar` & `formic_opcua-1.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/README.md
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/examples/opcua_client.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/examples/example_configs/opcua_config.yaml
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/examples/example_configs/opcua_config_1.yaml
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/examples/example_configs/opcua_config_2.yaml
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/examples/example_configs/opcua_config_3.yaml
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/examples/example_configs/opcua_config_4.yaml
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/examples/example_configs/opcua_config_5.yaml
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/formic_opcua/__init__.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/formic_opcua/client/__init__.py
--rw-r--r--   0        0        0    12221 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/formic_opcua/client/async_opcua_client.py
--rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/formic_opcua/client/opcua_client.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/formic_opcua/core/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/formic_opcua/core/exceptions.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/formic_opcua/core/parse.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/formic_opcua/core/type_conversions.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/formic_opcua/scripts/__init__.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/formic_opcua/scripts/formic_opcua_client.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/formic_opcua/scripts/formic_opcua_server.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/formic_opcua/server/__init__.py
--rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/formic_opcua/server/opcua_server.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/hooks/add_issue_prefix.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/tests/__init__.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/tests/test_server_config.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 formic_opcua-1.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 formic_opcua-1.5.0/README.md
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 formic_opcua-1.5.0/examples/opcua_client.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 formic_opcua-1.5.0/examples/example_configs/opcua_config.yaml
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 formic_opcua-1.5.0/examples/example_configs/opcua_config_1.yaml
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 formic_opcua-1.5.0/examples/example_configs/opcua_config_2.yaml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 formic_opcua-1.5.0/examples/example_configs/opcua_config_3.yaml
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 formic_opcua-1.5.0/examples/example_configs/opcua_config_4.yaml
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 formic_opcua-1.5.0/examples/example_configs/opcua_config_5.yaml
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 formic_opcua-1.5.0/formic_opcua/__init__.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 formic_opcua-1.5.0/formic_opcua/client/__init__.py
+-rw-r--r--   0        0        0    12237 2020-02-02 00:00:00.000000 formic_opcua-1.5.0/formic_opcua/client/async_opcua_client.py
+-rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 formic_opcua-1.5.0/formic_opcua/client/opcua_client.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 formic_opcua-1.5.0/formic_opcua/core/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 formic_opcua-1.5.0/formic_opcua/core/exceptions.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 formic_opcua-1.5.0/formic_opcua/core/parse.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 formic_opcua-1.5.0/formic_opcua/core/type_conversions.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.5.0/formic_opcua/scripts/__init__.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 formic_opcua-1.5.0/formic_opcua/scripts/formic_opcua_client.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 formic_opcua-1.5.0/formic_opcua/scripts/formic_opcua_server.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 formic_opcua-1.5.0/formic_opcua/server/__init__.py
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 formic_opcua-1.5.0/formic_opcua/server/opcua_server.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 formic_opcua-1.5.0/hooks/add_issue_prefix.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 formic_opcua-1.5.0/tests/test_server_config.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 formic_opcua-1.5.0/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 formic_opcua-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 formic_opcua-1.5.0/PKG-INFO
```

### Comparing `formic_opcua-1.4.0/.pre-commit-config.yaml` & `formic_opcua-1.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.4.0/examples/opcua_client.py` & `formic_opcua-1.5.0/examples/opcua_client.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.4.0/examples/example_configs/opcua_config.yaml` & `formic_opcua-1.5.0/examples/example_configs/opcua_config.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.4.0/examples/example_configs/opcua_config_1.yaml` & `formic_opcua-1.5.0/examples/example_configs/opcua_config_1.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.4.0/examples/example_configs/opcua_config_2.yaml` & `formic_opcua-1.5.0/examples/example_configs/opcua_config_2.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.4.0/formic_opcua/client/async_opcua_client.py` & `formic_opcua-1.5.0/formic_opcua/client/async_opcua_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 from formic_opcua.core import InvalidClientArgsError, convert_type, parse_settings
 
 logger = logging.getLogger(__name__)
 warnings.simplefilter('error')
 
 
 class ConnectionStatus(Enum):
-    CONNECTED = 0
-    CONNECTING = 1
-    DISCONNECTED = 2
+    CONNECTING = 10
+    CONNECTED = 20
+    DISCONNECTED = 30
 
 
 class AsyncOpcuaClient:
     def __init__(
-            self,
-            server_config_file: str = None,
-            connect_timeout: float = .5,
-            url: str = None,
-            uri: str = None,
-            username: str = None,
-            password: str = None,
+        self,
+        server_config_file: str = None,
+        connect_timeout: float = 0.5,
+        url: str = None,
+        uri: str = None,
+        username: str = None,
+        password: str = None,
     ) -> None:
         if server_config_file is None and (url is None and uri is None):
             error_message = 'No configuration arguments passed to client.'
             logger.critical(error_message)
             raise InvalidClientArgsError(error_message)
 
         if server_config_file is not None and (url is not None or uri is not None):
@@ -250,26 +250,26 @@
                 logger.info(f'Value: {value}')
                 return value
             else:
                 logger.warning('Read attempt failed')
                 self._connection_status = ConnectionStatus.DISCONNECTED
         return None
 
-    async def read_all(self, prefix: str = '') -> Dict[str, Any]:
+    async def read_all(self, prefixes: List[str] = ['']) -> Dict[str, Any]:
         logger.info(f'Attempting to read all variables on server at uri: {self._uri} and url: {self._url}.')
         results = {}
         future_results = {}
 
         if self._connection_status == ConnectionStatus.DISCONNECTED:
             logger.info('Client may not be connected to server. Attempting to connect.')
             await self.__aenter__()  # Creates a new client object and adjusts self._has_connected() appropriately
 
         if self._connection_status == ConnectionStatus.CONNECTED:
             for path in self._node_path_list:
-                if path.startswith(prefix):
+                if any([path.startswith(prefix) for prefix in prefixes]):
                     task_value = asyncio.create_task(self._read_helper(path))
                     future_results[path] = task_value
 
         if len(self._node_path_list) == 0:
             # There may never have been a connection
             self._connection_status = ConnectionStatus.DISCONNECTED
```

### Comparing `formic_opcua-1.4.0/formic_opcua/client/opcua_client.py` & `formic_opcua-1.5.0/formic_opcua/client/opcua_client.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.4.0/formic_opcua/core/parse.py` & `formic_opcua-1.5.0/formic_opcua/core/parse.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.4.0/formic_opcua/core/type_conversions.py` & `formic_opcua-1.5.0/formic_opcua/core/type_conversions.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.4.0/formic_opcua/scripts/formic_opcua_client.py` & `formic_opcua-1.5.0/formic_opcua/scripts/formic_opcua_client.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.4.0/formic_opcua/scripts/formic_opcua_server.py` & `formic_opcua-1.5.0/formic_opcua/scripts/formic_opcua_server.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.4.0/formic_opcua/server/opcua_server.py` & `formic_opcua-1.5.0/formic_opcua/server/opcua_server.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.4.0/hooks/add_issue_prefix.py` & `formic_opcua-1.5.0/hooks/add_issue_prefix.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.4.0/tests/test_server_config.py` & `formic_opcua-1.5.0/tests/test_server_config.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.4.0/.gitignore` & `formic_opcua-1.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.4.0/pyproject.toml` & `formic_opcua-1.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ['hatchling']
 build-backend = 'hatchling.build'
 
 [project]
 name = 'formic_opcua'
 requires-python = ">=3.8"
-version = "1.4.0"
+version = "1.5.0"
 authors = [
     {name = "Spencer White", email = "swhite@formic.co"},
     {name = "Damian Stempel"},
     {name = "Viachaslau Zakharchuk"}
 
 ]
 dependencies = [
```

