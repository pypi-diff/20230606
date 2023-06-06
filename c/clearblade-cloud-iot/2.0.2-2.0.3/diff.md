# Comparing `tmp/clearblade-cloud-iot-2.0.2.tar.gz` & `tmp/clearblade-cloud-iot-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/clearblade-cloud-iot-2.0.2.tar", last modified: Fri May 26 17:24:38 2023, max compression
+gzip compressed data, was "dist/clearblade-cloud-iot-2.0.3.tar", last modified: Tue Jun  6 17:38:15 2023, max compression
```

## Comparing `clearblade-cloud-iot-2.0.2.tar` & `clearblade-cloud-iot-2.0.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/clearblade/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/clearblade/cloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/
--rw-rw-r--   0 root         (0) root         (0)    22125 2023-05-26 17:20:22.000000 clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/device_types.py
--rw-rw-r--   0 root         (0) root         (0)    13659 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/developer_tests.py
--rw-rw-r--   0 root         (0) root         (0)     6471 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/resources.py
--rw-rw-r--   0 root         (0) root         (0)     9331 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/registry.py
--rw-rw-r--   0 root         (0) root         (0)     7497 2023-05-20 17:29:53.000000 clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/config_manager.py
--rw-rw-r--   0 root         (0) root         (0)     8201 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/registry_types.py
--rw-rw-r--   0 root         (0) root         (0)     3742 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8386 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/http_client.py
--rw-rw-r--   0 root         (0) root         (0)     2942 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/config.py
--rw-rw-r--   0 root         (0) root         (0)    22724 2023-05-23 13:52:19.000000 clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/devices.py
--rw-rw-r--   0 root         (0) root         (0)    10305 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/client.py
--rw-rw-r--   0 root         (0) root         (0)     7622 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/pagers.py
--rw-rw-r--   0 root         (0) root         (0)     3255 2023-05-26 17:20:22.000000 clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/utils.py
--rw-rw-r--   0 root         (0) root         (0)    11358 2022-11-02 06:10:48.000000 clearblade-cloud-iot-2.0.2/LICENSE
--rw-rw-r--   0 root         (0) root         (0)     1442 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.2/MANIFEST.in
--rw-rw-r--   0 root         (0) root         (0)     5090 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/google/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/google/cloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/google/cloud/iot/
--rw-rw-r--   0 root         (0) root         (0)       77 2022-11-02 06:10:48.000000 clearblade-cloud-iot-2.0.2/google/cloud/iot/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/google/cloud/iot_v1/
--rw-rw-r--   0 root         (0) root         (0)       77 2022-11-02 06:10:48.000000 clearblade-cloud-iot-2.0.2/google/cloud/iot_v1/py.typed
--rw-rw-r--   0 root         (0) root         (0)     5506 2022-11-02 06:10:48.000000 clearblade-cloud-iot-2.0.2/google/cloud/iot_v1/gapic_metadata.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/tests/unit/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.2/tests/unit/gapic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/tests/unit/gapic/iot_v1/
--rw-rw-r--   0 root         (0) root         (0)   235456 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.2/tests/unit/gapic/iot_v1/test_device_manager.py
--rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.2/tests/unit/gapic/iot_v1/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.2/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/tests/system/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/tests/system/gapic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/tests/system/gapic/v1/
--rw-rw-r--   0 root         (0) root         (0)     1557 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.2/tests/system/gapic/v1/test_system_device_manager_v1.py
--rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.2/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)       67 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     2835 2023-05-26 17:24:18.000000 clearblade-cloud-iot-2.0.2/setup.py
--rw-r--r--   0 root         (0) root         (0)     7002 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/clearblade_cloud_iot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1152 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/clearblade_cloud_iot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/clearblade_cloud_iot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/clearblade_cloud_iot.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/clearblade_cloud_iot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     7002 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/clearblade_cloud_iot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-13 22:31:57.000000 clearblade-cloud-iot-2.0.2/clearblade_cloud_iot.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       28 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/clearblade_cloud_iot.egg-info/namespace_packages.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/clearblade/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/clearblade/cloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/
+-rw-rw-r--   0 root         (0) root         (0)    22605 2023-06-06 17:32:57.000000 clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/device_types.py
+-rw-rw-r--   0 root         (0) root         (0)    13659 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/developer_tests.py
+-rw-rw-r--   0 root         (0) root         (0)     6471 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/resources.py
+-rw-rw-r--   0 root         (0) root         (0)     9331 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/registry.py
+-rw-rw-r--   0 root         (0) root         (0)     7497 2023-05-20 17:29:53.000000 clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/config_manager.py
+-rw-rw-r--   0 root         (0) root         (0)     8201 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/registry_types.py
+-rw-rw-r--   0 root         (0) root         (0)     3742 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8386 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/http_client.py
+-rw-rw-r--   0 root         (0) root         (0)     2942 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/config.py
+-rw-rw-r--   0 root         (0) root         (0)    22724 2023-05-23 13:52:19.000000 clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/devices.py
+-rw-rw-r--   0 root         (0) root         (0)    10305 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/client.py
+-rw-rw-r--   0 root         (0) root         (0)     7622 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/pagers.py
+-rw-rw-r--   0 root         (0) root         (0)     3255 2023-05-26 17:20:22.000000 clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/utils.py
+-rw-rw-r--   0 root         (0) root         (0)    11358 2022-11-02 06:10:48.000000 clearblade-cloud-iot-2.0.3/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)     1442 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.3/MANIFEST.in
+-rw-rw-r--   0 root         (0) root         (0)     5090 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.3/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/google/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/google/cloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/google/cloud/iot/
+-rw-rw-r--   0 root         (0) root         (0)       77 2022-11-02 06:10:48.000000 clearblade-cloud-iot-2.0.3/google/cloud/iot/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/google/cloud/iot_v1/
+-rw-rw-r--   0 root         (0) root         (0)       77 2022-11-02 06:10:48.000000 clearblade-cloud-iot-2.0.3/google/cloud/iot_v1/py.typed
+-rw-rw-r--   0 root         (0) root         (0)     5506 2022-11-02 06:10:48.000000 clearblade-cloud-iot-2.0.3/google/cloud/iot_v1/gapic_metadata.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/tests/unit/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.3/tests/unit/gapic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/tests/unit/gapic/iot_v1/
+-rw-rw-r--   0 root         (0) root         (0)   235456 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.3/tests/unit/gapic/iot_v1/test_device_manager.py
+-rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.3/tests/unit/gapic/iot_v1/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.3/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/tests/system/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/tests/system/gapic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/tests/system/gapic/v1/
+-rw-rw-r--   0 root         (0) root         (0)     1557 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.3/tests/system/gapic/v1/test_system_device_manager_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.3/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)       67 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     2835 2023-06-06 17:34:52.000000 clearblade-cloud-iot-2.0.3/setup.py
+-rw-r--r--   0 root         (0) root         (0)     7002 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/clearblade_cloud_iot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/clearblade_cloud_iot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/clearblade_cloud_iot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/clearblade_cloud_iot.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/clearblade_cloud_iot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     7002 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/clearblade_cloud_iot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2022-12-13 22:31:57.000000 clearblade-cloud-iot-2.0.3/clearblade_cloud_iot.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       28 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/clearblade_cloud_iot.egg-info/namespace_packages.txt
```

### Comparing `clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/device_types.py` & `clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/device_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,25 +59,28 @@
     return credentials
 
 class Device():
     """
     Data class for Clearblade Device
     """
     # TODO: find a better way to construct the Device object. I dont like so much parameter in a constructor
+    # From google SDK docs: The field ``name`` must be empty. The server generates ``name`` from the device 
+    # registry ``id`` and the ``parent`` field.
 
     def __init__(self, id: str, num_id: str = None,
                  credentials: list = [], last_heartbeat_time: str = None, last_event_time: str = None,
                  last_state_time: str = None, last_config_ack_time: str = None,
                  last_config_send_time: str = None, blocked: bool = False,
                  last_error_time: str = None, last_error_status_code: dict = None,
                  config: dict = {"cloudUpdateTime":None, "version":""} ,
                  state: dict = {"updateTime":None, "binaryData":None},
                  log_level: str = LogLevel.NONE, meta_data: dict = {}, gateway_config : dict = {"gatewayType": GatewayType.NON_GATEWAY}) -> None:
 
         self._id = id
+        self._name = ''
         self._num_id = num_id
         self._credentials = credentials
         self._last_heartbeat_time = last_heartbeat_time
         self._last_event_time = last_event_time
         self._last_state_time = last_state_time
         self._last_config_ack_time = last_config_ack_time
         self._last_config_send_time = last_config_send_time
@@ -113,15 +116,15 @@
             last_heartbeat_time = lastHeartbeatTimeFromJson
             last_event_time = lastEventTimeFromJson
             last_state_time = lastStateTimeFromJson
             last_config_ack_time = lastConfigAckTimeFromJson
             last_config_send_time = lastConfigSendTimeFromJson
             last_error_time = lastErrorTimeFromJson
 
-        return Device(
+        theDevice = Device(
             id=get_value(json, 'id'),
             num_id=get_value(json, 'numId'),
             credentials=convertCredentialsFormatsFromString(get_value(json, 'credentials')),
             last_heartbeat_time=last_heartbeat_time,
             last_event_time=last_event_time,
             last_state_time=last_state_time,
             last_config_ack_time=last_config_ack_time,
@@ -132,19 +135,30 @@
             config=DeviceConfig.from_json(configFromJson),
             state=DeviceState.from_json(stateFromJson),
             log_level=get_value(json, 'logLevel'),
             meta_data=get_value(json, 'metadata'),
             gateway_config=get_value(json, 'gatewayConfig')
         )
 
+        #Since _name is a private attribute, we have to populate it like this
+        #because we don't allow "name" to be passed in the constructor
+
+        theDevice._name=get_value(json, 'name')
+        
+        return theDevice
+
     @property
     def id(self):
         return self._id
 
     @property
+    def name(self):
+        return self._name
+
+    @property
     def num_id(self):
         return self._num_id
 
     @property
     def credentials(self):
         return self._credentials
```

### Comparing `clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/developer_tests.py` & `clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/developer_tests.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/resources.py` & `clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/resources.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/registry.py` & `clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/registry.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/config_manager.py` & `clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/config_manager.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/registry_types.py` & `clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/registry_types.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/__init__.py` & `clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/http_client.py` & `clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/http_client.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/config.py` & `clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/config.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/devices.py` & `clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/devices.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/client.py` & `clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/client.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/pagers.py` & `clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/pagers.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/utils.py` & `clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/utils.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.2/LICENSE` & `clearblade-cloud-iot-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.2/MANIFEST.in` & `clearblade-cloud-iot-2.0.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.2/README.rst` & `clearblade-cloud-iot-2.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.2/google/cloud/iot_v1/gapic_metadata.json` & `clearblade-cloud-iot-2.0.3/google/cloud/iot_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.2/tests/unit/gapic/__init__.py` & `clearblade-cloud-iot-2.0.3/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.2/tests/unit/gapic/iot_v1/test_device_manager.py` & `clearblade-cloud-iot-2.0.3/tests/unit/gapic/iot_v1/test_device_manager.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.2/tests/unit/gapic/iot_v1/__init__.py` & `clearblade-cloud-iot-2.0.3/tests/unit/gapic/iot_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.2/tests/unit/__init__.py` & `clearblade-cloud-iot-2.0.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.2/tests/system/gapic/v1/test_system_device_manager_v1.py` & `clearblade-cloud-iot-2.0.3/tests/system/gapic/v1/test_system_device_manager_v1.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.2/tests/__init__.py` & `clearblade-cloud-iot-2.0.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.2/setup.py` & `clearblade-cloud-iot-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import io
 import os
 
 import setuptools
 
 name = "clearblade-cloud-iot"
 description = "Cloud IoT API client library"
-version = "2.0.2"
+version = "2.0.3"
 release_status = "Development Status :: 5 - Production/Stable"
 dependencies = ["httpx", "proto-plus"]
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
```

### Comparing `clearblade-cloud-iot-2.0.2/PKG-INFO` & `clearblade-cloud-iot-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: clearblade-cloud-iot
-Version: 2.0.2
+Version: 2.0.3
 Summary: Cloud IoT API client library
 Home-page: https://github.com/clearblade/python-iot
 Author: Clearblade
 Author-email: googleapis-packages@oogle.com
 License: Apache 2.0
 Description: .. Copyright 2023 ClearBlade Inc.
             Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `clearblade-cloud-iot-2.0.2/clearblade_cloud_iot.egg-info/SOURCES.txt` & `clearblade-cloud-iot-2.0.3/clearblade_cloud_iot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.2/clearblade_cloud_iot.egg-info/PKG-INFO` & `clearblade-cloud-iot-2.0.3/clearblade_cloud_iot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: clearblade-cloud-iot
-Version: 2.0.2
+Version: 2.0.3
 Summary: Cloud IoT API client library
 Home-page: https://github.com/clearblade/python-iot
 Author: Clearblade
 Author-email: googleapis-packages@oogle.com
 License: Apache 2.0
 Description: .. Copyright 2023 ClearBlade Inc.
             Licensed under the Apache License, Version 2.0 (the "License");
```

