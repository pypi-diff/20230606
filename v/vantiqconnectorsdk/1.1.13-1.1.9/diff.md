# Comparing `tmp/vantiqconnectorsdk-1.1.13.tar.gz` & `tmp/vantiqconnectorsdk-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantiqconnectorsdk-1.1.13.tar", last modified: Tue Jun  6 00:07:33 2023, max compression
+gzip compressed data, was "vantiqconnectorsdk-1.1.9.tar", last modified: Thu May 19 23:28:45 2022, max compression
```

## Comparing `vantiqconnectorsdk-1.1.13.tar` & `vantiqconnectorsdk-1.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2023-06-06 00:07:33.249905 vantiqconnectorsdk-1.1.13/
--rw-r--r--   0 fcarter    (501) staff       (20)     1079 2022-05-09 21:56:14.000000 vantiqconnectorsdk-1.1.13/LICENSE
--rw-r--r--   0 fcarter    (501) staff       (20)    19543 2023-06-06 00:07:33.250166 vantiqconnectorsdk-1.1.13/PKG-INFO
--rw-r--r--   0 fcarter    (501) staff       (20)    17912 2022-06-09 23:45:23.000000 vantiqconnectorsdk-1.1.13/README.md
--rw-r--r--   0 fcarter    (501) staff       (20)       80 2022-05-09 21:56:14.000000 vantiqconnectorsdk-1.1.13/pyproject.toml
--rw-r--r--   0 fcarter    (501) staff       (20)      712 2023-06-06 00:07:33.251793 vantiqconnectorsdk-1.1.13/setup.cfg
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2023-06-06 00:07:33.204952 vantiqconnectorsdk-1.1.13/src/
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2023-06-06 00:07:33.205104 vantiqconnectorsdk-1.1.13/src/main/
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2023-06-06 00:07:33.244871 vantiqconnectorsdk-1.1.13/src/main/python/
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2023-06-06 00:07:33.249394 vantiqconnectorsdk-1.1.13/src/main/python/vantiqconnectorsdk.egg-info/
--rw-r--r--   0 fcarter    (501) staff       (20)    19543 2023-06-06 00:07:33.000000 vantiqconnectorsdk-1.1.13/src/main/python/vantiqconnectorsdk.egg-info/PKG-INFO
--rw-r--r--   0 fcarter    (501) staff       (20)      369 2023-06-06 00:07:33.000000 vantiqconnectorsdk-1.1.13/src/main/python/vantiqconnectorsdk.egg-info/SOURCES.txt
--rw-r--r--   0 fcarter    (501) staff       (20)        1 2023-06-06 00:07:33.000000 vantiqconnectorsdk-1.1.13/src/main/python/vantiqconnectorsdk.egg-info/dependency_links.txt
--rw-r--r--   0 fcarter    (501) staff       (20)       33 2023-06-06 00:07:33.000000 vantiqconnectorsdk-1.1.13/src/main/python/vantiqconnectorsdk.egg-info/requires.txt
--rw-r--r--   0 fcarter    (501) staff       (20)       19 2023-06-06 00:07:33.000000 vantiqconnectorsdk-1.1.13/src/main/python/vantiqconnectorsdk.egg-info/top_level.txt
--rw-r--r--   0 fcarter    (501) staff       (20)    40374 2022-06-01 20:17:21.000000 vantiqconnectorsdk-1.1.13/src/main/python/vantiqconnectorsdk.py
+drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2022-05-19 23:28:45.724050 vantiqconnectorsdk-1.1.9/
+-rw-r--r--   0 fcarter    (501) staff       (20)     1079 2022-05-09 21:51:22.000000 vantiqconnectorsdk-1.1.9/LICENSE
+-rw-r--r--   0 fcarter    (501) staff       (20)    19497 2022-05-19 23:28:45.724220 vantiqconnectorsdk-1.1.9/PKG-INFO
+-rw-r--r--   0 fcarter    (501) staff       (20)    17867 2022-05-19 23:22:13.000000 vantiqconnectorsdk-1.1.9/README.md
+-rw-r--r--   0 fcarter    (501) staff       (20)       80 2022-05-09 21:51:22.000000 vantiqconnectorsdk-1.1.9/pyproject.toml
+-rw-r--r--   0 fcarter    (501) staff       (20)      709 2022-05-19 23:28:45.726211 vantiqconnectorsdk-1.1.9/setup.cfg
+drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2022-05-19 23:28:45.717038 vantiqconnectorsdk-1.1.9/src/
+drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2022-05-19 23:28:45.717155 vantiqconnectorsdk-1.1.9/src/main/
+drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2022-05-19 23:28:45.719902 vantiqconnectorsdk-1.1.9/src/main/python/
+drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2022-05-19 23:28:45.723753 vantiqconnectorsdk-1.1.9/src/main/python/vantiqconnectorsdk.egg-info/
+-rw-r--r--   0 fcarter    (501) staff       (20)    19497 2022-05-19 23:28:45.000000 vantiqconnectorsdk-1.1.9/src/main/python/vantiqconnectorsdk.egg-info/PKG-INFO
+-rw-r--r--   0 fcarter    (501) staff       (20)      369 2022-05-19 23:28:45.000000 vantiqconnectorsdk-1.1.9/src/main/python/vantiqconnectorsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 fcarter    (501) staff       (20)        1 2022-05-19 23:28:45.000000 vantiqconnectorsdk-1.1.9/src/main/python/vantiqconnectorsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 fcarter    (501) staff       (20)       31 2022-05-19 23:28:45.000000 vantiqconnectorsdk-1.1.9/src/main/python/vantiqconnectorsdk.egg-info/requires.txt
+-rw-r--r--   0 fcarter    (501) staff       (20)       19 2022-05-19 23:28:45.000000 vantiqconnectorsdk-1.1.9/src/main/python/vantiqconnectorsdk.egg-info/top_level.txt
+-rw-r--r--   0 fcarter    (501) staff       (20)    39660 2022-05-19 23:22:13.000000 vantiqconnectorsdk-1.1.9/src/main/python/vantiqconnectorsdk.py
```

### Comparing `vantiqconnectorsdk-1.1.13/LICENSE` & `vantiqconnectorsdk-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vantiqconnectorsdk-1.1.13/PKG-INFO` & `vantiqconnectorsdk-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantiqconnectorsdk
-Version: 1.1.13
+Version: 1.1.9
 Summary: SDK for building Vantiq extension sources/connectors in Python
 Home-page: https://github.com/Vantiq/vantiq-extension-sources
 Author: Vantiq, Inc
 Author-email: fcarter@vantiq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -19,16 +19,15 @@
 This repository contains the SDK for building Vantiq connectors (also known as extension sources)
 using Python. At a high level, a connector is configured and then run, responding or sending messages to messages the Vantiq server. Each connector acts as a _source_ in a Vantiq namespace.
 
 You will need credentials to a Vantiq server to use this SDK.  Please contact your Vantiq system administrator to obtain these credentials.
 
 ## Overview of a Connector
 
-For details about the overall structure of a connector and the protocol used between the connector and the Vantiq source, please see
-[here](https://github.com/Vantiq/vantiq-extension-sources#readme).  
+For details about the overall structure of a connector and the protocol used between the connector and the Vantiq source, please see [here](../README.md).  
 
 Each running instance of this code represents a set of connectors that connect to a single Vantiq namespace. The set of sources for the connector & the connection information is found in the server config file.  We will describe the details later.
 
 Using the Python VantiqConnector SDK, the overall operation is as follows:
 
 * Create a `VantiqConnectorSet` that manages the set of connections (one per source listed in the `server.config` file.
 * Establish a set of _handlers_ or callbacks that will allow the connectors to respond to messages from the Vantiq server. There are callbacks for the following situations:
```

### Comparing `vantiqconnectorsdk-1.1.13/README.md` & `vantiqconnectorsdk-1.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 This repository contains the SDK for building Vantiq connectors (also known as extension sources)
 using Python. At a high level, a connector is configured and then run, responding or sending messages to messages the Vantiq server. Each connector acts as a _source_ in a Vantiq namespace.
 
 You will need credentials to a Vantiq server to use this SDK.  Please contact your Vantiq system administrator to obtain these credentials.
 
 ## Overview of a Connector
 
-For details about the overall structure of a connector and the protocol used between the connector and the Vantiq source, please see
-[here](https://github.com/Vantiq/vantiq-extension-sources#readme).  
+For details about the overall structure of a connector and the protocol used between the connector and the Vantiq source, please see [here](../README.md).  
 
 Each running instance of this code represents a set of connectors that connect to a single Vantiq namespace. The set of sources for the connector & the connection information is found in the server config file.  We will describe the details later.
 
 Using the Python VantiqConnector SDK, the overall operation is as follows:
 
 * Create a `VantiqConnectorSet` that manages the set of connections (one per source listed in the `server.config` file.
 * Establish a set of _handlers_ or callbacks that will allow the connectors to respond to messages from the Vantiq server. There are callbacks for the following situations:
```

### Comparing `vantiqconnectorsdk-1.1.13/src/main/python/vantiqconnectorsdk.egg-info/PKG-INFO` & `vantiqconnectorsdk-1.1.9/src/main/python/vantiqconnectorsdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantiqconnectorsdk
-Version: 1.1.13
+Version: 1.1.9
 Summary: SDK for building Vantiq extension sources/connectors in Python
 Home-page: https://github.com/Vantiq/vantiq-extension-sources
 Author: Vantiq, Inc
 Author-email: fcarter@vantiq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -19,16 +19,15 @@
 This repository contains the SDK for building Vantiq connectors (also known as extension sources)
 using Python. At a high level, a connector is configured and then run, responding or sending messages to messages the Vantiq server. Each connector acts as a _source_ in a Vantiq namespace.
 
 You will need credentials to a Vantiq server to use this SDK.  Please contact your Vantiq system administrator to obtain these credentials.
 
 ## Overview of a Connector
 
-For details about the overall structure of a connector and the protocol used between the connector and the Vantiq source, please see
-[here](https://github.com/Vantiq/vantiq-extension-sources#readme).  
+For details about the overall structure of a connector and the protocol used between the connector and the Vantiq source, please see [here](../README.md).  
 
 Each running instance of this code represents a set of connectors that connect to a single Vantiq namespace. The set of sources for the connector & the connection information is found in the server config file.  We will describe the details later.
 
 Using the Python VantiqConnector SDK, the overall operation is as follows:
 
 * Create a `VantiqConnectorSet` that manages the set of connections (one per source listed in the `server.config` file.
 * Establish a set of _handlers_ or callbacks that will allow the connectors to respond to messages from the Vantiq server. There are callbacks for the following situations:
```

### Comparing `vantiqconnectorsdk-1.1.13/src/main/python/vantiqconnectorsdk.py` & `vantiqconnectorsdk-1.1.9/src/main/python/vantiqconnectorsdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -425,34 +425,22 @@
 
                 connect_msg = {_OPERATION: _OP_CONNECT_EXTENSION,
                                _RESOURCE_NAME: _SOURCES_RESOURCE,
                                _RESOURCE_ID: self.source_name}
                 await websocket.send(json.dumps(connect_msg))
                 raw_resp = await websocket.recv()
                 resp = json.loads(raw_resp)
+                if _STATUS in resp.keys():
+                    _vlog.debug('Connect returned: %s', resp[_STATUS])
+                    status = resp[_STATUS]
+                    if status >= 300:
+                        return _CONNECTION_FAILED
 
-                possible_status_message = 0
-                # Sometimes we get a status message back.  If so & it's OK, wait for the config message
-                while _OPERATION not in resp.keys() and possible_status_message < 10:
-                    possible_status_message += 1
-                    if _STATUS in resp.keys():
-                        _vlog.debug('Connect returned: %s', resp[_STATUS])
-                        status = resp[_STATUS]
-                        if status >= 300:
-                            return _CONNECTION_FAILED
-                    raw_resp = await websocket.recv()
-                    resp = json.loads(raw_resp)
-
-                if _OPERATION not in resp.keys():
-                    error = f'Unable to make connection. No {_OP_CONFIGURE_EXTENSION} ' \
-                                f'message received after {possible_status_message} tries.'
-                    _vlog.error(error)
-                    raise VantiqConnectorException(error)
-                else:
-                    # Otherwise, we should have a configExtension message
+                # Otherwise, we should have a configExtension message
+                if _OPERATION in resp.keys():
                     if resp[_OPERATION] == _OP_CONFIGURE_EXTENSION:
                         # Here, we have a configuration that's been returned.  Process it
                         _vlog.debug('Configuration message: %s', resp[_OPERATION])
                         if _OBJECT in resp.keys() and 'config' in resp[_OBJECT].keys():
                             _vlog.debug('Configuration is: %s', resp[_OBJECT]['config'])
                             local = self.connect_handler
                             if local:
```

