# Comparing `tmp/openlineage-python-0.8.2.tar.gz` & `tmp/openlineage-python-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openlineage-python-0.8.2.tar", last modified: Thu May 19 20:00:10 2022, max compression
+gzip compressed data, was "dist/openlineage-python-0.9.0.tar", last modified: Fri Jun  3 23:03:19 2022, max compression
```

## Comparing `openlineage-python-0.8.2.tar` & `openlineage-python-0.9.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-19 20:00:10.000000 openlineage-python-0.8.2/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3679 2022-05-19 20:00:10.000000 openlineage-python-0.8.2/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2801 2022-05-19 20:00:10.000000 openlineage-python-0.8.2/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-19 20:00:10.000000 openlineage-python-0.8.2/openlineage/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-19 20:00:10.000000 openlineage-python-0.8.2/openlineage/client/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      185 2022-05-19 20:00:10.000000 openlineage-python-0.8.2/openlineage/client/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2054 2022-05-19 20:00:10.000000 openlineage-python-0.8.2/openlineage/client/client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      272 2022-05-19 20:00:10.000000 openlineage-python-0.8.2/openlineage/client/constants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4732 2022-05-19 20:00:10.000000 openlineage-python-0.8.2/openlineage/client/facet.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1339 2022-05-19 20:00:10.000000 openlineage-python-0.8.2/openlineage/client/run.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1244 2022-05-19 20:00:10.000000 openlineage-python-0.8.2/openlineage/client/serde.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-19 20:00:10.000000 openlineage-python-0.8.2/openlineage/client/transport/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      852 2022-05-19 20:00:10.000000 openlineage-python-0.8.2/openlineage/client/transport/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      513 2022-05-19 20:00:10.000000 openlineage-python-0.8.2/openlineage/client/transport/console.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4450 2022-05-19 20:00:10.000000 openlineage-python-0.8.2/openlineage/client/transport/factory.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3939 2022-05-19 20:00:10.000000 openlineage-python-0.8.2/openlineage/client/transport/http.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1689 2022-05-19 20:00:10.000000 openlineage-python-0.8.2/openlineage/client/transport/kafka.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      979 2022-05-19 20:00:10.000000 openlineage-python-0.8.2/openlineage/client/transport/transport.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1219 2022-05-19 20:00:10.000000 openlineage-python-0.8.2/openlineage/client/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-19 20:00:10.000000 openlineage-python-0.8.2/openlineage_python.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3679 2022-05-19 20:00:10.000000 openlineage-python-0.8.2/openlineage_python.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      718 2022-05-19 20:00:10.000000 openlineage-python-0.8.2/openlineage_python.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-05-19 20:00:10.000000 openlineage-python-0.8.2/openlineage_python.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-05-19 20:00:10.000000 openlineage-python-0.8.2/openlineage_python.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      194 2022-05-19 20:00:10.000000 openlineage-python-0.8.2/openlineage_python.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2022-05-19 20:00:10.000000 openlineage-python-0.8.2/openlineage_python.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      502 2022-05-19 20:00:10.000000 openlineage-python-0.8.2/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      954 2022-05-19 20:00:10.000000 openlineage-python-0.8.2/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3679 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2801 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      185 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2054 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      272 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/constants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4732 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/facet.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1339 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/run.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1270 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/serde.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/transport/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      975 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/transport/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      513 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/transport/console.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4654 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/transport/factory.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3939 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/transport/http.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1689 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/transport/kafka.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      523 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/transport/noop.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      979 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/transport/transport.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1219 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage_python.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3679 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage_python.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      755 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage_python.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage_python.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage_python.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      194 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage_python.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage_python.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      502 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      954 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/setup.py
```

### Comparing `openlineage-python-0.8.2/PKG-INFO` & `openlineage-python-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlineage-python
-Version: 0.8.2
+Version: 0.9.0
 Summary: OpenLineage Python Client
 Home-page: UNKNOWN
 Author: OpenLineage
 License: UNKNOWN
 Description: # OpenLineage-python
         
         To install from source, run:
```

### Comparing `openlineage-python-0.8.2/README.md` & `openlineage-python-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `openlineage-python-0.8.2/openlineage/client/client.py` & `openlineage-python-0.9.0/openlineage/client/client.py`

 * *Files identical despite different names*

### Comparing `openlineage-python-0.8.2/openlineage/client/facet.py` & `openlineage-python-0.9.0/openlineage/client/facet.py`

 * *Files identical despite different names*

### Comparing `openlineage-python-0.8.2/openlineage/client/run.py` & `openlineage-python-0.9.0/openlineage/client/run.py`

 * *Files identical despite different names*

### Comparing `openlineage-python-0.8.2/openlineage/client/serde.py` & `openlineage-python-0.9.0/openlineage/client/serde.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             return obj.value
         if isinstance(obj, Dict):
             return dict(filter(
                 lambda x: x[1] is not None,
                 {k: cls.remove_nulls_and_enums(v) for k, v in obj.items()}.items()
             ))
         if isinstance(obj, List):
-            return list(filter(lambda x: x is not None and x != {}, [
+            return list(filter(lambda x: x is not None and (isinstance(x, dict) and x != {}), [
                 cls.remove_nulls_and_enums(v) for v in obj if v is not None
             ]))
 
         # Pandas can use numpy.int64 object
         if numpy and isinstance(obj, numpy.int64):
             return int(obj)
         return obj
```

### Comparing `openlineage-python-0.8.2/openlineage/client/transport/__init__.py` & `openlineage-python-0.9.0/openlineage/client/transport/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # flake8: noqa
 from typing import Type
 
+from openlineage.client.transport.noop import NoopTransport
 from openlineage.client.transport.transport import Transport, Config, TransportFactory
 from openlineage.client.transport.factory import DefaultTransportFactory
 from openlineage.client.transport.http import HttpTransport, HttpConfig
 from openlineage.client.transport.kafka import KafkaTransport, KafkaConfig
 from openlineage.client.transport.console import ConsoleTransport
 
 
 _factory = DefaultTransportFactory()
 _factory.register_transport(HttpTransport.kind, HttpTransport)
 _factory.register_transport(KafkaTransport.kind, KafkaTransport)
 _factory.register_transport(ConsoleTransport.kind, ConsoleTransport)
+_factory.register_transport(NoopTransport.kind, NoopTransport)
 
 
 def get_default_factory():
     return _factory
 
 
 # decorator to wrap transports with
```

### Comparing `openlineage-python-0.8.2/openlineage/client/transport/console.py` & `openlineage-python-0.9.0/openlineage/client/transport/console.py`

 * *Files identical despite different names*

### Comparing `openlineage-python-0.8.2/openlineage/client/transport/factory.py` & `openlineage-python-0.9.0/openlineage/client/transport/factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # SPDX-License-Identifier: Apache-2.0.
 import inspect
 import os
 import logging
 from typing import Type, Union, Optional
 
+from openlineage.client.transport.noop import NoopConfig, NoopTransport
 from openlineage.client.transport.transport import Config, Transport, TransportFactory
 from openlineage.client.utils import try_import_from_string
 
 
 log = logging.getLogger(__name__)
 
 
@@ -21,14 +22,17 @@
     def __init__(self):
         self.transports = {}
 
     def register_transport(self, type: str, clazz: Union[Type[Transport], str]):
         self.transports[type] = clazz
 
     def create(self) -> Transport:
+        if os.environ.get("OPENLINEAGE_DISABLED", False) in [True, "true", "True"]:
+            return NoopTransport(NoopConfig())
+
         if yaml:
             yml_config = self._try_config_from_yaml()
             if yml_config:
                 return self._create_transport(yml_config)
         # Fallback to setting HTTP transport from env variables
         http = self._try_http_from_env_config()
         if http:
```

### Comparing `openlineage-python-0.8.2/openlineage/client/transport/http.py` & `openlineage-python-0.9.0/openlineage/client/transport/http.py`

 * *Files identical despite different names*

### Comparing `openlineage-python-0.8.2/openlineage/client/transport/kafka.py` & `openlineage-python-0.9.0/openlineage/client/transport/kafka.py`

 * *Files identical despite different names*

### Comparing `openlineage-python-0.8.2/openlineage/client/transport/transport.py` & `openlineage-python-0.9.0/openlineage/client/transport/transport.py`

 * *Files identical despite different names*

### Comparing `openlineage-python-0.8.2/openlineage/client/utils.py` & `openlineage-python-0.9.0/openlineage/client/utils.py`

 * *Files identical despite different names*

### Comparing `openlineage-python-0.8.2/openlineage_python.egg-info/PKG-INFO` & `openlineage-python-0.9.0/openlineage_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlineage-python
-Version: 0.8.2
+Version: 0.9.0
 Summary: OpenLineage Python Client
 Home-page: UNKNOWN
 Author: OpenLineage
 License: UNKNOWN
 Description: # OpenLineage-python
         
         To install from source, run:
```

### Comparing `openlineage-python-0.8.2/openlineage_python.egg-info/SOURCES.txt` & `openlineage-python-0.9.0/openlineage_python.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 openlineage/client/serde.py
 openlineage/client/utils.py
 openlineage/client/transport/__init__.py
 openlineage/client/transport/console.py
 openlineage/client/transport/factory.py
 openlineage/client/transport/http.py
 openlineage/client/transport/kafka.py
+openlineage/client/transport/noop.py
 openlineage/client/transport/transport.py
 openlineage_python.egg-info/PKG-INFO
 openlineage_python.egg-info/SOURCES.txt
 openlineage_python.egg-info/dependency_links.txt
 openlineage_python.egg-info/not-zip-safe
 openlineage_python.egg-info/requires.txt
 openlineage_python.egg-info/top_level.txt
```

### Comparing `openlineage-python-0.8.2/setup.py` & `openlineage-python-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "tests": ["pytest", "pytest-cov", "mock", "flake8", "requests", "pyyaml"],
     "kafka": ["confluent-kafka"],
 }
 extras_require["dev"] = set(sum(extras_require.values(), []))
 
 setup(
     name="openlineage-python",
-    version="0.8.2",
+    version="0.9.0",
     description="OpenLineage Python Client",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="OpenLineage",
     packages=find_namespace_packages(include=['openlineage.*']),
     include_package_data=True,
     install_requires=requirements,
```

