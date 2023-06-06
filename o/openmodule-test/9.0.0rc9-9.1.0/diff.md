# Comparing `tmp/openmodule_test-9.0.0rc9.tar.gz` & `tmp/openmodule_test-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmodule_test-9.0.0rc9.tar", last modified: Wed Dec 22 10:26:38 2021, max compression
+gzip compressed data, was "openmodule_test-9.1.0.tar", last modified: Wed Mar  9 10:32:56 2022, max compression
```

## Comparing `openmodule_test-9.0.0rc9.tar` & `openmodule_test-9.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-22 10:26:38.404780 openmodule_test-9.0.0rc9/
--rw-r--r--   0 root         (0) root         (0)      262 2021-12-22 10:26:38.000000 openmodule_test-9.0.0rc9/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     7099 2021-12-22 10:26:38.000000 openmodule_test-9.0.0rc9/ChangeLog
--rw-r--r--   0 root         (0) root         (0)      617 2021-12-22 10:26:38.404780 openmodule_test-9.0.0rc9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-12-22 10:26:23.000000 openmodule_test-9.0.0rc9/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      561 2021-12-22 10:26:23.000000 openmodule_test-9.0.0rc9/alert.py
--rw-rw-rw-   0 root         (0) root         (0)     2542 2021-12-22 10:26:23.000000 openmodule_test-9.0.0rc9/api.py
--rw-rw-rw-   0 root         (0) root         (0)     9515 2021-12-22 10:26:23.000000 openmodule_test-9.0.0rc9/backend.py
--rw-rw-rw-   0 root         (0) root         (0)      889 2021-12-22 10:26:23.000000 openmodule_test-9.0.0rc9/core.py
--rw-rw-rw-   0 root         (0) root         (0)     2323 2021-12-22 10:26:23.000000 openmodule_test-9.0.0rc9/database.py
--rw-rw-rw-   0 root         (0) root         (0)      759 2021-12-22 10:26:23.000000 openmodule_test-9.0.0rc9/database_models.py
--rw-rw-rw-   0 root         (0) root         (0)     3001 2021-12-22 10:26:23.000000 openmodule_test-9.0.0rc9/eventlistener.py
--rw-rw-rw-   0 root         (0) root         (0)      255 2021-12-22 10:26:23.000000 openmodule_test-9.0.0rc9/files.py
--rw-rw-rw-   0 root         (0) root         (0)     3084 2021-12-22 10:26:23.000000 openmodule_test-9.0.0rc9/gate.py
--rw-rw-rw-   0 root         (0) root         (0)     1650 2021-12-22 10:26:23.000000 openmodule_test-9.0.0rc9/health.py
--rw-rw-rw-   0 root         (0) root         (0)     3582 2021-12-22 10:26:23.000000 openmodule_test-9.0.0rc9/interrupt.py
--rw-rw-rw-   0 root         (0) root         (0)     4047 2021-12-22 10:26:23.000000 openmodule_test-9.0.0rc9/io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-22 10:26:38.404780 openmodule_test-9.0.0rc9/openmodule_test.egg-info/
--rw-r--r--   0 root         (0) root         (0)      617 2021-12-22 10:26:38.000000 openmodule_test-9.0.0rc9/openmodule_test.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      498 2021-12-22 10:26:38.000000 openmodule_test-9.0.0rc9/openmodule_test.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-12-22 10:26:38.000000 openmodule_test-9.0.0rc9/openmodule_test.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-12-22 10:26:38.000000 openmodule_test-9.0.0rc9/openmodule_test.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       24 2021-12-22 10:26:38.000000 openmodule_test-9.0.0rc9/openmodule_test.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2021-12-22 10:26:38.000000 openmodule_test-9.0.0rc9/openmodule_test.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     5263 2021-12-22 10:26:23.000000 openmodule_test-9.0.0rc9/presence.py
--rw-rw-rw-   0 root         (0) root         (0)       24 2021-12-22 10:26:23.000000 openmodule_test-9.0.0rc9/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1840 2021-12-22 10:26:23.000000 openmodule_test-9.0.0rc9/rpc.py
--rw-rw-rw-   0 root         (0) root         (0)      594 2021-12-22 10:26:38.405780 openmodule_test-9.0.0rc9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      521 2021-12-22 10:26:23.000000 openmodule_test-9.0.0rc9/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      574 2021-12-22 10:26:23.000000 openmodule_test-9.0.0rc9/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    18426 2021-12-22 10:26:23.000000 openmodule_test-9.0.0rc9/zeromq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 10:32:56.091452 openmodule_test-9.1.0/
+-rw-r--r--   0 root         (0) root         (0)      228 2022-03-09 10:32:55.000000 openmodule_test-9.1.0/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)     6770 2022-03-09 10:32:55.000000 openmodule_test-9.1.0/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)      614 2022-03-09 10:32:56.091452 openmodule_test-9.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-09 10:32:41.000000 openmodule_test-9.1.0/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      561 2022-03-09 10:32:41.000000 openmodule_test-9.1.0/alert.py
+-rw-rw-rw-   0 root         (0) root         (0)     9515 2022-03-09 10:32:41.000000 openmodule_test-9.1.0/backend.py
+-rw-rw-rw-   0 root         (0) root         (0)      889 2022-03-09 10:32:41.000000 openmodule_test-9.1.0/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     2470 2022-03-09 10:32:41.000000 openmodule_test-9.1.0/database.py
+-rw-rw-rw-   0 root         (0) root         (0)      759 2022-03-09 10:32:41.000000 openmodule_test-9.1.0/database_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3001 2022-03-09 10:32:41.000000 openmodule_test-9.1.0/eventlistener.py
+-rw-rw-rw-   0 root         (0) root         (0)      255 2022-03-09 10:32:41.000000 openmodule_test-9.1.0/files.py
+-rw-rw-rw-   0 root         (0) root         (0)     3192 2022-03-09 10:32:41.000000 openmodule_test-9.1.0/gate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1650 2022-03-09 10:32:41.000000 openmodule_test-9.1.0/health.py
+-rw-rw-rw-   0 root         (0) root         (0)     4157 2022-03-09 10:32:41.000000 openmodule_test-9.1.0/interrupt.py
+-rw-rw-rw-   0 root         (0) root         (0)     4047 2022-03-09 10:32:41.000000 openmodule_test-9.1.0/io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 10:32:56.091452 openmodule_test-9.1.0/openmodule_test.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      614 2022-03-09 10:32:55.000000 openmodule_test-9.1.0/openmodule_test.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      523 2022-03-09 10:32:56.000000 openmodule_test-9.1.0/openmodule_test.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-03-09 10:32:55.000000 openmodule_test-9.1.0/openmodule_test.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-03-09 10:32:55.000000 openmodule_test-9.1.0/openmodule_test.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       47 2022-03-09 10:32:55.000000 openmodule_test-9.1.0/openmodule_test.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)       24 2022-03-09 10:32:55.000000 openmodule_test-9.1.0/openmodule_test.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2022-03-09 10:32:55.000000 openmodule_test-9.1.0/openmodule_test.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     5263 2022-03-09 10:32:41.000000 openmodule_test-9.1.0/presence.py
+-rw-rw-rw-   0 root         (0) root         (0)       24 2022-03-09 10:32:41.000000 openmodule_test-9.1.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1840 2022-03-09 10:32:41.000000 openmodule_test-9.1.0/rpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      594 2022-03-09 10:32:56.092369 openmodule_test-9.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      521 2022-03-09 10:32:41.000000 openmodule_test-9.1.0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      574 2022-03-09 10:32:41.000000 openmodule_test-9.1.0/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    18818 2022-03-09 10:32:41.000000 openmodule_test-9.1.0/zeromq.py
```

### Comparing `openmodule_test-9.0.0rc9/ChangeLog` & `openmodule_test-9.1.0/ChangeLog`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,19 @@
 CHANGES
 =======
 
-v9.0.0.rc9
-----------
-
-* added base64 validator to payload added some models added default source entry to validate response
-
-v9.0.0.rc8
-----------
-
-* added cost entries to the access model
-
-v9.0.0.rc7
-----------
-
-* renamed status to state
-* ¯\\_(ツ)\_/¯
-* added base64\_validator
-* added timezone\_validator
-* dependencies fix because i forgot setting python interpreter
-* changed some validation model typings
-* added validation provider template class
-* added validatino provider models
-* minor change in deprecation warnings [skip ci]
-* use assert warnings instead of assert logs for failing testcase
-* some docs
-* assertion replaced with a warning to prevent unnecessary crashes as it's not breaking
-
-v9.0.0.rc6
-----------
-
-* additional logs during startup, and a better default value for broker sub port and broker pub port in the backwards compatibility functions
-
-v9.0.0.rc5
-----------
-
-* fixes in the count message definition
-
-v9.0.0.rc4
-----------
-
-* refactoring for backends aswell as some message definition cleanups
-
-v9.0.0.rc3
-----------
-
-* backwardscompatibility fix for vehicle (all ids must be empty by default)
-
-v9.0.0.rc2
-----------
+v9.1.0
+------
 
-* trigger for dev releases
+* Feature/privacy
 
-v9.0.0.rc1
-----------
+v9.0.0
+------
 
-* refactored rpc client, some cleanup and fixes across the board
+* Version 9 Release
 
 v8.1.3
 ------
 
 * Additions to Vehicle and Presence messages
 
 v8.1.2
@@ -170,19 +124,39 @@
 v6.1.0
 ------
 
 * docs [skip-ci]
 * relative path fix again
 * relative path fix
 * lazy config
+* openmodule config
 * docs [skip ci]
 
 v6.0.1
 ------
 
 * allow import of checking module
 * documentation [skip ci]
 
 v6.0.0
 ------
 
 * requirements
+* known issues
+* fixes an issue with .timestamp() and testing
+* name function which has no doc string in assertion
+* why did i do that?
+* recurrence allows empty strings again now, wait\_for\_reject raises an assertion instead of timeout error if the barrier actually opened
+* testcase for datetime-naive saves
+* git stash popMerge branch 'timezone\_checks' of gitlab.com:arivo-public/device-python/openmodule into timezone\_checks
+* why was this ignored?
+* developer error, test gate
+* check on migration/make\_migration if DateTime is used + testcase, custom types are now imported correctly
+* fix in timezone validator for optional fields
+* v6 breaking changes, added timezone / datetime checks
+* added database flush and a known issues list
+
+v5.0.1
+------
+
+* fixes a bug in the database code, which swallowed exceptions during commit()
+* api changes
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `openmodule_test-9.0.0rc9/PKG-INFO` & `openmodule_test-9.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmodule_test
-Version: 9.0.0rc9
+Version: 9.1.0
 Summary: Libraries for testing openmodule services
 Home-page: https://gitlab.com/arivo-public/device-python/openmodule.git
 Author: ARIVO
 Author-email: support@arivo.co
 License: GNU General Public License v2 (GPLv2)
 Keywords: arivo openmodule openmodule_test test
 Platform: UNKNOWN
```

### Comparing `openmodule_test-9.0.0rc9/alert.py` & `openmodule_test-9.1.0/alert.py`

 * *Files identical despite different names*

### Comparing `openmodule_test-9.0.0rc9/backend.py` & `openmodule_test-9.1.0/backend.py`

 * *Files identical despite different names*

### Comparing `openmodule_test-9.0.0rc9/core.py` & `openmodule_test-9.1.0/core.py`

 * *Files identical despite different names*

### Comparing `openmodule_test-9.0.0rc9/database.py` & `openmodule_test-9.1.0/database.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,30 +26,34 @@
     """
     Mixin for database cleanup in test cases
     * use create_database = True for an automatic generation of a database
     * use create_database = False and set the database directly
     """
     create_database = True
     database = None
-    database_folder: str = settings.DATABASE_FOLDER
+    database_folder: str = None  # defaults to settings.DATABASE_FOLDER
     alembic_path = "../src/database"
     database_name = "database"
 
     @classmethod
+    def get_database_folder(cls):
+        return cls.database_folder or settings.DATABASE_FOLDER
+
+    @classmethod
     def setUpClass(cls) -> None:
         # we only know which databases are in use on tear down, so truncating only works in teardown
         # but in order to not be annoyed by failed tests which left broken databases, we delete all databases
         # once initially
         global _first_start
         if _first_start:
-            for file in glob(os.path.join(cls.database_folder, "*.sqlite3")):
+            for file in glob(os.path.join(cls.get_database_folder(), "*.sqlite3")):
                 os.unlink(file)
             _first_start = False
         if cls.create_database:
-            cls.database = Database(cls.database_folder, cls.database_name, cls.alembic_path)
+            cls.database = Database(cls.get_database_folder(), cls.database_name, cls.alembic_path)
         return super().setUpClass()
 
     def delete_database(self, database: Database):
         assert not database.is_open(), "database must be shutdown before it can be deleted"
         try:
             os.unlink(database_path(database.db_folder, database.name))
         except FileNotFoundError:
```

### Comparing `openmodule_test-9.0.0rc9/database_models.py` & `openmodule_test-9.1.0/database_models.py`

 * *Files identical despite different names*

### Comparing `openmodule_test-9.0.0rc9/eventlistener.py` & `openmodule_test-9.1.0/eventlistener.py`

 * *Files identical despite different names*

### Comparing `openmodule_test-9.0.0rc9/gate.py` & `openmodule_test-9.1.0/gate.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,16 +21,18 @@
 
     open_count = 0
     reject_count = 0
 
     def __init__(self, gate: str, direction: Direction, dispatcher: MessageDispatcher):
         self.gate = gate
         self.direction = direction
-        dispatcher.register_handler(b"access_accept", TestGateAccessMessage, self._access_accept, register_schema=False)
-        dispatcher.register_handler(b"access_reject", TestGateAccessMessage, self._access_reject, register_schema=False)
+        dispatcher.register_handler(b"access_accept", TestGateAccessMessage, self._access_accept,
+                                    register_schema=False, match_type=False)
+        dispatcher.register_handler(b"access_reject", TestGateAccessMessage, self._access_reject,
+                                    register_schema=False, match_type=False)
         _all_gates.add(self)
 
     @classmethod
     def reset_all_counts(cls):
         for x in _all_gates:
             x.reset_call_count()
```

### Comparing `openmodule_test-9.0.0rc9/health.py` & `openmodule_test-9.1.0/health.py`

 * *Files identical despite different names*

### Comparing `openmodule_test-9.0.0rc9/interrupt.py` & `openmodule_test-9.1.0/interrupt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import os
 import time
 from multiprocessing import Process, Event
 from signal import SIGINT, SIGKILL
-from typing import Callable, Union, Type
+from typing import Callable, Union, Type, Optional
 from unittest import TestCase
 
 import multiprocessing_logging
 
 from openmodule.core import shutdown_openmodule
 from openmodule.utils.schema import Schema
 from openmodule_test.health import HealthTestMixin
@@ -29,17 +29,30 @@
 
 class InterruptTestMixin(TestCase):
     """
     Helper class for testing interrupts and exceptions in code
     for usage, look at file tests/test_interrupt
     """
 
+    process: Optional[ExceptionProcess] = None
+
+    def _kill_process(self):
+        # this is called in tear down and as a cleanup to make sure that under any circumstances the process is killed
+        # otherwise you have processes lingering around, potentially blocking ports which is quite annoying
+        if self.process and self.process.is_alive():
+            os.kill(self.process.pid, SIGKILL)
+
+    def setUp(self) -> None:
+        self.addCleanup(self._kill_process)
+        super().setUp()
+
     def tearDown(self):
         super().tearDown()
         Schema.to_file()
+        self._kill_process()
 
     def wait_for_setup(self):
         pass
 
     def _wait_for_and_uninstall_mp_handler(self, logger=None):
         """
         waits until the multiprocessing logging handler has finished
@@ -54,17 +67,17 @@
         multiprocessing_logging.uninstall_mp_handler(logger)
 
     def start_process(self, f: Callable):
         """
         starts the process and waits until it is responsive by calling calls wait_for_setup()
         """
         multiprocessing_logging.install_mp_handler()
-        process = ExceptionProcess(target=f)
-        process.start()
-        return process
+        self.process = ExceptionProcess(target=f)
+        self.process.start()
+        return self.process
 
     def assertCleanShutdown(self, process, shutdown_timeout: float = 3.0):
         """
         asserts that the process shuts down cleanly
         """
         if process.is_finished.wait(timeout=shutdown_timeout):
             self._wait_for_and_uninstall_mp_handler()
@@ -72,15 +85,15 @@
         else:
             if process.is_alive():
                 os.kill(process.pid, SIGKILL)
                 raise TimeoutError("Process took to long for shutdown")
             else:
                 raise AssertionError("Process did not finish gracefully")
 
-    def send_signal_to_process(self, process, signal: Union[Type[KeyboardInterrupt], int]):
+    def send_signal_to_process(self, process: ExceptionProcess, signal: Union[Type[KeyboardInterrupt], int]):
         self.assertFalse(process.is_finished.is_set())
         if signal == KeyboardInterrupt:
             signal = SIGINT
         os.kill(process.pid, signal)
 
     def signal_in_function(self, f: Callable, signal: Union[Type[KeyboardInterrupt], int], *,
                            raise_exception_after: float = 3.0, shutdown_timeout: float = 3.0):
```

### Comparing `openmodule_test-9.0.0rc9/io.py` & `openmodule_test-9.1.0/io.py`

 * *Files identical despite different names*

### Comparing `openmodule_test-9.0.0rc9/openmodule_test.egg-info/PKG-INFO` & `openmodule_test-9.1.0/openmodule_test.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmodule-test
-Version: 9.0.0rc9
+Version: 9.1.0
 Summary: Libraries for testing openmodule services
 Home-page: https://gitlab.com/arivo-public/device-python/openmodule.git
 Author: ARIVO
 Author-email: support@arivo.co
 License: GNU General Public License v2 (GPLv2)
 Keywords: arivo openmodule openmodule_test test
 Platform: UNKNOWN
```

### Comparing `openmodule_test-9.0.0rc9/presence.py` & `openmodule_test-9.1.0/presence.py`

 * *Files identical despite different names*

### Comparing `openmodule_test-9.0.0rc9/rpc.py` & `openmodule_test-9.1.0/rpc.py`

 * *Files identical despite different names*

### Comparing `openmodule_test-9.0.0rc9/setup.cfg` & `openmodule_test-9.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `openmodule_test-9.0.0rc9/setup.py` & `openmodule_test-9.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `openmodule_test-9.0.0rc9/utils.py` & `openmodule_test-9.1.0/utils.py`

 * *Files identical despite different names*

### Comparing `openmodule_test-9.0.0rc9/zeromq.py` & `openmodule_test-9.1.0/zeromq.py`

 * *Files 3% similar despite different names*

```diff
@@ -347,20 +347,28 @@
 
 
 class _TestRPCRequest(BaseModel):
     """
     we do not want to depend on openmodule, this is a minimal version of the zmq message for the rpc function
     """
     timestamp: float = Field(default_factory=time.time)
-    resource: Optional[str] = settings.RESOURCE
+    resource: Optional[str] = None
     name: str
     type: str
     rpc_id: UUID
     request: Optional[Dict]
 
+    def __init__(self, **kwargs):
+        resource = kwargs.pop("resource")
+        if not resource:
+            # this avoids evaluating settings.RESOURCE if resource is set in order to not trigger the settings module
+            # to start up unnecessarily (and maybe throw import errors)
+            resource = settings.RESOURCE
+        super().__init__(resource=resource, **kwargs)
+
 
 class ZMQProcotol(str, Enum):
     inproc = "inproc://"
     tcp = "tcp://"
 
 
 class ZMQTestMixin(TestCase):
@@ -414,15 +422,15 @@
 
         """
         waits until a message dispatcher receives messages, this assumes that the subscription we issue is the last
         and if it is connected, all previous subscriptions will also be connected
         """
         random_topic = "_test" + "".join(random.choices(string.ascii_letters, k=10))
         random_topic = random_topic.encode()
-        dispatcher.register_handler(random_topic, BaseModel, handler, register_schema=False)
+        dispatcher.register_handler(random_topic, BaseModel, handler, register_schema=False, match_type=False)
 
         for x in range(self.zmq_client.startup_check_iterations):
             self.zmq_client.send(random_topic, {"type": "connection-check"})
             time.sleep(self.zmq_client.startup_check_delay)
             if received:
                 break
         assert received, "error during startup and connect"
```

