# Comparing `tmp/macrometa-target-mongo-0.0.8.tar.gz` & `tmp/macrometa-target-mongo-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-mongo-0.0.8.tar", max compression
+gzip compressed data, was "macrometa-target-mongo-0.0.9.tar", max compression
```

## Comparing `macrometa-target-mongo-0.0.8.tar` & `macrometa-target-mongo-0.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0    32393 2023-02-02 14:29:03.590187 macrometa-target-mongo-0.0.8/LICENSE
--rw-r--r--   0        0        0     6056 2023-02-02 14:29:03.590187 macrometa-target-mongo-0.0.8/macrometa_target_mongo/__init__.py
--rw-r--r--   0        0        0     9350 2023-02-02 14:29:03.590187 macrometa-target-mongo-0.0.8/macrometa_target_mongo/main.py
--rw-r--r--   0        0        0     1591 2023-02-02 14:29:03.830253 macrometa-target-mongo-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1018 1970-01-01 00:00:00.000000 macrometa-target-mongo-0.0.8/setup.py
--rw-r--r--   0        0        0     1068 1970-01-01 00:00:00.000000 macrometa-target-mongo-0.0.8/PKG-INFO
+-rwxr-xr-x   0        0        0    32393 2023-02-07 07:10:24.954189 macrometa-target-mongo-0.0.9/LICENSE
+-rw-r--r--   0        0        0     6076 2023-02-07 07:10:24.954189 macrometa-target-mongo-0.0.9/macrometa_target_mongo/__init__.py
+-rw-r--r--   0        0        0     9350 2023-02-07 07:10:24.954189 macrometa-target-mongo-0.0.9/macrometa_target_mongo/main.py
+-rw-r--r--   0        0        0     1591 2023-02-07 07:10:25.198192 macrometa-target-mongo-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1018 1970-01-01 00:00:00.000000 macrometa-target-mongo-0.0.9/setup.py
+-rw-r--r--   0        0        0     1068 1970-01-01 00:00:00.000000 macrometa-target-mongo-0.0.9/PKG-INFO
```

### Comparing `macrometa-target-mongo-0.0.8/LICENSE` & `macrometa-target-mongo-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-mongo-0.0.8/macrometa_target_mongo/__init__.py` & `macrometa-target-mongo-0.0.9/macrometa_target_mongo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,55 +48,55 @@
         """Get supported schemas using the given configurations."""
         return []
 
     def config(self) -> list[ConfigProperty]:
         """Get configuration parameters for the connector."""
         return [
             ConfigProperty('host', 'Host', ConfigAttributeType.STRING, True, False,
-                           description='MongoDB host',
+                           description='MongoDB host.',
                            placeholder_value='mongodb_host'),
             ConfigProperty('port', 'Port', ConfigAttributeType.INT, False, False,
-                           description='MongoDB port',
+                           description='MongoDB port.',
                            default_value='27017'),
-            ConfigProperty('user', 'User', ConfigAttributeType.STRING, True, False,
-                           description='MongoDB user',
+            ConfigProperty('user', 'Username', ConfigAttributeType.STRING, True, False,
+                           description='MongoDB user.',
                            placeholder_value='mongo'),
             ConfigProperty('password', 'Password', ConfigAttributeType.STRING, True, False,
-                           description='MongoDB password',
+                           description='MongoDB password.',
                            placeholder_value='password'),
             ConfigProperty('auth_database', 'Auth Database', ConfigAttributeType.STRING, True, False,
-                           description='MongoDB authentication database',
+                           description='MongoDB authentication database.',
                            default_value='admin'),
             ConfigProperty('database', 'Database', ConfigAttributeType.STRING, True, False,
-                           description='MongoDB database name',
+                           description='MongoDB database name.',
                            placeholder_value='mongo'),
             ConfigProperty('target_collection', 'Target Collection', ConfigAttributeType.STRING, True, True,
                            description="Target collection name.",
                            placeholder_value='my_collection'),
             ConfigProperty('hard_delete', 'Hard Delete', ConfigAttributeType.BOOLEAN, False, False,
                            description='When `hard_delete` option is true then the documents which are deleted from '
                                        'the source will also be deleted from MongoDB. It is achieved by continuously checking '
                                        'the `_SDC_DELETED_AT` metadata attribute sent by the source connector.',
                            default_value='false'),
-            ConfigProperty('srv', 'Srv', ConfigAttributeType.BOOLEAN, False, False,
+            ConfigProperty('srv', 'Enable Srv', ConfigAttributeType.BOOLEAN, False, False,
                            description='Uses a `mongodb+srv` protocol to connect. Disables the usage of `port` '
                                        'argument if set to `True.`',
                            default_value='false'),
             ConfigProperty('replica_set', 'Replica Set', ConfigAttributeType.STRING, False, False,
-                           description='Name of replica set',
+                           description='Name of replica set.',
                            placeholder_value='replica'),
             ConfigProperty('direct_connection', 'Direct Connection', ConfigAttributeType.BOOLEAN, False, False,
                            description='Specifies whether to connect directly to the specified MongoDB host as a standalone '
-                                       'or connect to the entire replica set of which the given MongoDB host(s) is a part.',
+                                       'or connect to the entire replica set of which the given MongoDB host is a part.',
                            default_value='false'),
-            ConfigProperty('ssl', 'SSL', ConfigAttributeType.BOOLEAN, False, False,
-                           description='Can be set to true to connect using ssl.',
+            ConfigProperty('ssl', 'Use SSL', ConfigAttributeType.BOOLEAN, False, False,
+                           description='Can be set to true to connect using SSL.',
                            default_value='false'),
             ConfigProperty('verify_mode', 'Verify Mode', ConfigAttributeType.BOOLEAN, False, False,
-                           description='Default SSL verify mode',
+                           description='Default SSL verify mode.',
                            default_value='true'),
             ConfigProperty('batch_size_rows', 'Batch Size', ConfigAttributeType.INT, False, False,
                            description='Maximum number of rows inserted per batch.',
                            default_value='50'),
             ConfigProperty('batch_flush_interval', 'Batch Flush Interval (Seconds)',
                            ConfigAttributeType.INT, False, False,
                            description='Time between batch flush executions.',
```

### Comparing `macrometa-target-mongo-0.0.8/macrometa_target_mongo/main.py` & `macrometa-target-mongo-0.0.9/macrometa_target_mongo/main.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-mongo-0.0.8/pyproject.toml` & `macrometa-target-mongo-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core==1.0.8"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-target-mongo"
-version='0.0.8'
+version='0.0.9'
 description = "Macrometa connector for writing data into MongoDB, can be used as a target for any Data Mesh Integration."
 license = "Apache-2.0"
 authors = ["Macrometa <product@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-target-mongo-0.0.8/setup.py` & `macrometa-target-mongo-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-target-mongo = '
                      'macrometa_target_mongo.main:main']}
 
 setup_kwargs = {
     'name': 'macrometa-target-mongo',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Macrometa connector for writing data into MongoDB, can be used as a target for any Data Mesh Integration.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'product@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-target-mongo-0.0.8/PKG-INFO` & `macrometa-target-mongo-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-mongo
-Version: 0.0.8
+Version: 0.0.9
 Summary: Macrometa connector for writing data into MongoDB, can be used as a target for any Data Mesh Integration.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,Target,MongoDB
 Author: Macrometa
 Author-email: product@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

