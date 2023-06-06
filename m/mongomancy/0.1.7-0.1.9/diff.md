# Comparing `tmp/mongomancy-0.1.7.tar.gz` & `tmp/mongomancy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongomancy-0.1.7.tar", last modified: Wed May 10 12:41:34 2023, max compression
+gzip compressed data, was "mongomancy-0.1.9.tar", last modified: Fri May 12 12:46:03 2023, max compression
```

## Comparing `mongomancy-0.1.7.tar` & `mongomancy-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-10 12:41:34.288725 mongomancy-0.1.7/
--rw-r--r--   0 trval     (1000) trval     (1000)     2152 2023-05-10 12:38:30.000000 mongomancy-0.1.7/CHANGELOG.md
--rw-rw-r--   0 trval     (1000) trval     (1000)     1329 2022-09-02 09:33:19.000000 mongomancy-0.1.7/CONTRIBUTING.md
--rw-r--r--   0 trval     (1000) trval     (1000)     1516 2023-04-04 08:06:59.000000 mongomancy-0.1.7/LICENSE
--rw-r--r--   0 trval     (1000) trval     (1000)       42 2023-04-12 12:30:41.000000 mongomancy-0.1.7/MANIFEST.in
--rw-r--r--   0 trval     (1000) trval     (1000)     4466 2023-05-10 12:41:34.288725 mongomancy-0.1.7/PKG-INFO
--rw-r--r--   0 trval     (1000) trval     (1000)     3675 2023-05-10 08:26:11.000000 mongomancy-0.1.7/README.md
--rw-r--r--   0 trval     (1000) trval     (1000)     1368 2023-04-12 12:30:41.000000 mongomancy-0.1.7/pyproject.toml
--rw-rw-r--   0 trval     (1000) trval     (1000)       68 2022-09-02 09:38:35.000000 mongomancy-0.1.7/requirements.txt
--rw-r--r--   0 trval     (1000) trval     (1000)       38 2023-05-10 12:41:34.288725 mongomancy-0.1.7/setup.cfg
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-10 12:41:34.285391 mongomancy-0.1.7/src/
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-10 12:41:34.288725 mongomancy-0.1.7/src/mongomancy/
--rw-r--r--   0 trval     (1000) trval     (1000)      431 2023-05-10 12:38:30.000000 mongomancy-0.1.7/src/mongomancy/__init__.py
--rw-r--r--   0 trval     (1000) trval     (1000)    14650 2023-05-10 12:38:30.000000 mongomancy-0.1.7/src/mongomancy/engine.py
--rw-rw-r--   0 trval     (1000) trval     (1000)      924 2022-08-29 12:44:42.000000 mongomancy-0.1.7/src/mongomancy/mongo_errors.py
--rw-r--r--   0 trval     (1000) trval     (1000)        0 2023-04-12 12:30:41.000000 mongomancy-0.1.7/src/mongomancy/py.typed
--rw-r--r--   0 trval     (1000) trval     (1000)    15322 2023-05-10 12:38:30.000000 mongomancy-0.1.7/src/mongomancy/schema.py
--rw-r--r--   0 trval     (1000) trval     (1000)     7743 2023-05-10 12:38:30.000000 mongomancy-0.1.7/src/mongomancy/types.py
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-10 12:41:34.288725 mongomancy-0.1.7/src/mongomancy.egg-info/
--rw-rw-r--   0 trval     (1000) trval     (1000)     4466 2023-05-10 12:41:34.000000 mongomancy-0.1.7/src/mongomancy.egg-info/PKG-INFO
--rw-rw-r--   0 trval     (1000) trval     (1000)      435 2023-05-10 12:41:34.000000 mongomancy-0.1.7/src/mongomancy.egg-info/SOURCES.txt
--rw-rw-r--   0 trval     (1000) trval     (1000)        1 2023-05-10 12:41:34.000000 mongomancy-0.1.7/src/mongomancy.egg-info/dependency_links.txt
--rw-rw-r--   0 trval     (1000) trval     (1000)       13 2023-05-10 12:41:34.000000 mongomancy-0.1.7/src/mongomancy.egg-info/requires.txt
--rw-rw-r--   0 trval     (1000) trval     (1000)       11 2023-05-10 12:41:34.000000 mongomancy-0.1.7/src/mongomancy.egg-info/top_level.txt
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-12 12:46:03.201796 mongomancy-0.1.9/
+-rw-r--r--   0 trval     (1000) trval     (1000)     2270 2023-05-12 12:45:39.000000 mongomancy-0.1.9/CHANGELOG.md
+-rw-rw-r--   0 trval     (1000) trval     (1000)     1329 2022-09-02 09:33:19.000000 mongomancy-0.1.9/CONTRIBUTING.md
+-rw-r--r--   0 trval     (1000) trval     (1000)     1516 2023-04-04 08:06:59.000000 mongomancy-0.1.9/LICENSE
+-rw-r--r--   0 trval     (1000) trval     (1000)       42 2023-04-12 12:30:41.000000 mongomancy-0.1.9/MANIFEST.in
+-rw-r--r--   0 trval     (1000) trval     (1000)     4466 2023-05-12 12:46:03.201796 mongomancy-0.1.9/PKG-INFO
+-rw-r--r--   0 trval     (1000) trval     (1000)     3675 2023-05-10 08:26:11.000000 mongomancy-0.1.9/README.md
+-rw-r--r--   0 trval     (1000) trval     (1000)     1368 2023-04-12 12:30:41.000000 mongomancy-0.1.9/pyproject.toml
+-rw-rw-r--   0 trval     (1000) trval     (1000)       68 2022-09-02 09:38:35.000000 mongomancy-0.1.9/requirements.txt
+-rw-r--r--   0 trval     (1000) trval     (1000)       38 2023-05-12 12:46:03.201796 mongomancy-0.1.9/setup.cfg
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-12 12:46:03.198463 mongomancy-0.1.9/src/
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-12 12:46:03.201796 mongomancy-0.1.9/src/mongomancy/
+-rw-r--r--   0 trval     (1000) trval     (1000)      431 2023-05-12 12:45:39.000000 mongomancy-0.1.9/src/mongomancy/__init__.py
+-rw-r--r--   0 trval     (1000) trval     (1000)    14837 2023-05-12 12:39:11.000000 mongomancy-0.1.9/src/mongomancy/engine.py
+-rw-rw-r--   0 trval     (1000) trval     (1000)      924 2022-08-29 12:44:42.000000 mongomancy-0.1.9/src/mongomancy/mongo_errors.py
+-rw-r--r--   0 trval     (1000) trval     (1000)        0 2023-04-12 12:30:41.000000 mongomancy-0.1.9/src/mongomancy/py.typed
+-rw-r--r--   0 trval     (1000) trval     (1000)    15322 2023-05-10 12:38:30.000000 mongomancy-0.1.9/src/mongomancy/schema.py
+-rw-r--r--   0 trval     (1000) trval     (1000)     7743 2023-05-10 12:38:30.000000 mongomancy-0.1.9/src/mongomancy/types.py
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-12 12:46:03.201796 mongomancy-0.1.9/src/mongomancy.egg-info/
+-rw-rw-r--   0 trval     (1000) trval     (1000)     4466 2023-05-12 12:46:03.000000 mongomancy-0.1.9/src/mongomancy.egg-info/PKG-INFO
+-rw-rw-r--   0 trval     (1000) trval     (1000)      435 2023-05-12 12:46:03.000000 mongomancy-0.1.9/src/mongomancy.egg-info/SOURCES.txt
+-rw-rw-r--   0 trval     (1000) trval     (1000)        1 2023-05-12 12:46:03.000000 mongomancy-0.1.9/src/mongomancy.egg-info/dependency_links.txt
+-rw-rw-r--   0 trval     (1000) trval     (1000)       13 2023-05-12 12:46:03.000000 mongomancy-0.1.9/src/mongomancy.egg-info/requires.txt
+-rw-rw-r--   0 trval     (1000) trval     (1000)       11 2023-05-12 12:46:03.000000 mongomancy-0.1.9/src/mongomancy.egg-info/top_level.txt
```

### Comparing `mongomancy-0.1.7/CHANGELOG.md` & `mongomancy-0.1.9/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.1.9] - 2023-05-12
+
+### Fix
+
+- ping now work even if connection is broken, and does nto fall into infinite loop
+
 ## [0.1.7] - 2023-05-10
 
 ### Fix
 
 - lock critical sections `Engine.reconnect`, `Engine.dispose` to prevent unexpected connections states
 - lock `Database.create_all` method to prevent double init at same
```

### Comparing `mongomancy-0.1.7/CONTRIBUTING.md` & `mongomancy-0.1.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.7/LICENSE` & `mongomancy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.7/PKG-INFO` & `mongomancy-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongomancy
-Version: 0.1.7
+Version: 0.1.9
 Summary: Pymongo based python client with data definition layer.
 Author-email: Tom Trval <thandeus@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Ryu-CZ/mongomancy
 Project-URL: Bug Tracker, https://github.com/Ryu-CZ/mongomancy/issues
 Keywords: mongo,python,pymongo,database,nosql
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `mongomancy-0.1.7/README.md` & `mongomancy-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.7/pyproject.toml` & `mongomancy-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.7/src/mongomancy/engine.py` & `mongomancy-0.1.9/src/mongomancy/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     """
     Client of Mongo Database storage. All DB communication should be handled through this class.
     """
 
     CONNECTION_ERRORS: ClassVar[Iterable[Type[pymongo.errors.PyMongoError]]] = (
         pymongo.errors.AutoReconnect,
         pymongo.errors.ConnectionFailure,
+        IOError,
     )
     disposed: bool
     client: pymongo.MongoClient
     logger: LoggerType
     semaphore_tower: types.SemaphoreTower
     retry_codes: Set[int]
     write_retry: int
@@ -193,23 +194,30 @@
     def ping(self, database: Optional[str] = None) -> bool:
         """
         Is database server reachable?
 
         :param database: database name, otherwise just ping client by listing databases
         :return: Is database server reachable?
         """
+
         is_ok = False
-        retry = self.read_retry
+        retry = max(1, self.read_retry)
         while not is_ok and retry > 0:
+            retry -= 1
+            if self.disposed:
+                try:
+                    self.reconnect()
+                except PyMongoError:
+                    is_ok = False
             try:
                 _ = self.client.list_databases()
                 is_ok = True
                 if database:
                     is_ok = self.client.get_database(database).command("ping").get("ok")
-            except (IOError, pymongo.errors.ConnectionFailure) as e:
+            except self.CONNECTION_ERRORS as e:
                 self.logger.info(f"failed to ping database={database!r} - e={e}")
                 time.sleep(self.read_retry_delay)
                 self.reconnect()
             except PyMongoError as e:
                 self.logger.info(f"failed to ping database={database!r} - e={e}")
                 self.logger.warning(traceback.format_stack())
         return bool(is_ok)
```

### Comparing `mongomancy-0.1.7/src/mongomancy/mongo_errors.py` & `mongomancy-0.1.9/src/mongomancy/mongo_errors.py`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.7/src/mongomancy/schema.py` & `mongomancy-0.1.9/src/mongomancy/schema.py`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.7/src/mongomancy/types.py` & `mongomancy-0.1.9/src/mongomancy/types.py`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.7/src/mongomancy.egg-info/PKG-INFO` & `mongomancy-0.1.9/src/mongomancy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongomancy
-Version: 0.1.7
+Version: 0.1.9
 Summary: Pymongo based python client with data definition layer.
 Author-email: Tom Trval <thandeus@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Ryu-CZ/mongomancy
 Project-URL: Bug Tracker, https://github.com/Ryu-CZ/mongomancy/issues
 Keywords: mongo,python,pymongo,database,nosql
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

