# Comparing `tmp/ugot-0.1.4.tar.gz` & `tmp/ugot-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ugot-0.1.4.tar", last modified: Wed May 31 07:12:08 2023, max compression
+gzip compressed data, was "ugot-0.1.5.tar", last modified: Tue Jun  6 03:00:15 2023, max compression
```

## Comparing `ugot-0.1.4.tar` & `ugot-0.1.5.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-31 07:12:08.049381 ugot-0.1.4/
--rw-r--r--   0 jesse      (501) staff       (20)     1103 2023-05-15 09:14:27.000000 ugot-0.1.4/LICENSE
--rw-r--r--   0 jesse      (501) staff       (20)      612 2023-05-31 07:12:08.049002 ugot-0.1.4/PKG-INFO
--rwxrwxrwx   0 jesse      (501) staff       (20)      246 2023-05-11 07:07:58.000000 ugot-0.1.4/README.md
--rwxrwxrwx   0 jesse      (501) staff       (20)      425 2023-05-31 07:09:42.000000 ugot-0.1.4/pyproject.toml
--rw-r--r--   0 jesse      (501) staff       (20)       38 2023-05-31 07:12:08.049494 ugot-0.1.4/setup.cfg
--rwxrwxrwx   0 jesse      (501) staff       (20)      558 2023-05-31 07:09:47.000000 ugot-0.1.4/setup.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-31 07:12:07.953365 ugot-0.1.4/ugot/
--rw-r--r--   0 jesse      (501) staff       (20)        0 2023-05-11 07:37:21.000000 ugot-0.1.4/ugot/__init__.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-31 07:12:08.011757 ugot-0.1.4/ugot/grpc_pb/
--rw-r--r--   0 jesse      (501) staff       (20)        0 2023-05-11 07:27:02.000000 ugot-0.1.4/ugot/grpc_pb/__init__.py
--rw-r--r--   0 jesse      (501) staff       (20)     6021 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/audio_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    23990 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/audio_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)     6234 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/bluetooth_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    18284 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/bluetooth_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)     9603 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/device_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    30498 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/device_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)     6103 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/gpio_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    18277 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/gpio_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)     8843 2023-05-29 08:59:43.000000 ugot-0.1.4/ugot/grpc_pb/model_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    23309 2023-05-29 08:59:43.000000 ugot-0.1.4/ugot/grpc_pb/model_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)     6803 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/network_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    24828 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/network_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)     2135 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/power_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)     5561 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/power_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)     5080 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/sensor_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    13911 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/sensor_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)    10875 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/servo_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    24766 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/servo_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)     5891 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/vision_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    16618 2023-05-15 03:20:28.000000 ugot-0.1.4/ugot/grpc_pb/vision_pb2_grpc.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-31 07:12:08.012426 ugot-0.1.4/ugot/protos/
--rw-r--r--   0 jesse      (501) staff       (20)        0 2023-05-11 07:27:02.000000 ugot-0.1.4/ugot/protos/__init__.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-31 07:12:08.039053 ugot-0.1.4/ugot/src/
--rw-r--r--   0 jesse      (501) staff       (20)        0 2023-05-11 07:27:02.000000 ugot-0.1.4/ugot/src/__init__.py
--rw-r--r--   0 jesse      (501) staff       (20)     2674 2023-05-11 07:27:02.000000 ugot-0.1.4/ugot/src/audio_client.py
--rw-r--r--   0 jesse      (501) staff       (20)      517 2023-05-11 07:27:02.000000 ugot-0.1.4/ugot/src/base_client.py
--rw-r--r--   0 jesse      (501) staff       (20)      615 2023-05-11 07:27:02.000000 ugot-0.1.4/ugot/src/bluetooth_client.py
--rw-r--r--   0 jesse      (501) staff       (20)     4159 2023-05-11 07:27:02.000000 ugot-0.1.4/ugot/src/device_client.py
--rw-r--r--   0 jesse      (501) staff       (20)     5085 2023-05-11 07:27:02.000000 ugot-0.1.4/ugot/src/enum.py
--rw-r--r--   0 jesse      (501) staff       (20)     3089 2023-05-11 07:27:02.000000 ugot-0.1.4/ugot/src/gpio_client.py
--rw-r--r--   0 jesse      (501) staff       (20)     8210 2023-05-29 08:59:43.000000 ugot-0.1.4/ugot/src/model_client.py
--rw-r--r--   0 jesse      (501) staff       (20)     5566 2023-05-11 07:27:02.000000 ugot-0.1.4/ugot/src/network_client.py
--rw-r--r--   0 jesse      (501) staff       (20)      592 2023-05-11 07:27:02.000000 ugot-0.1.4/ugot/src/power_client.py
--rw-r--r--   0 jesse      (501) staff       (20)     2245 2023-05-31 07:06:58.000000 ugot-0.1.4/ugot/src/scan_device.py
--rw-r--r--   0 jesse      (501) staff       (20)     1108 2023-05-11 07:27:02.000000 ugot-0.1.4/ugot/src/sensor_client.py
--rw-r--r--   0 jesse      (501) staff       (20)     2291 2023-05-11 07:27:02.000000 ugot-0.1.4/ugot/src/servo_client.py
--rw-r--r--   0 jesse      (501) staff       (20)     4110 2023-05-11 07:27:02.000000 ugot-0.1.4/ugot/src/util.py
--rw-r--r--   0 jesse      (501) staff       (20)    12490 2023-05-19 07:22:40.000000 ugot-0.1.4/ugot/src/vision_client.py
--rw-r--r--   0 jesse      (501) staff       (20)    87205 2023-05-31 07:06:58.000000 ugot-0.1.4/ugot/ugot.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-31 07:12:07.956184 ugot-0.1.4/ugot.egg-info/
--rw-r--r--   0 jesse      (501) staff       (20)      612 2023-05-31 07:12:07.000000 ugot-0.1.4/ugot.egg-info/PKG-INFO
--rw-r--r--   0 jesse      (501) staff       (20)     1206 2023-05-31 07:12:07.000000 ugot-0.1.4/ugot.egg-info/SOURCES.txt
--rw-r--r--   0 jesse      (501) staff       (20)        1 2023-05-31 07:12:07.000000 ugot-0.1.4/ugot.egg-info/dependency_links.txt
--rw-r--r--   0 jesse      (501) staff       (20)       67 2023-05-31 07:12:07.000000 ugot-0.1.4/ugot.egg-info/requires.txt
--rw-r--r--   0 jesse      (501) staff       (20)        5 2023-05-31 07:12:07.000000 ugot-0.1.4/ugot.egg-info/top_level.txt
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-06-06 03:00:15.779728 ugot-0.1.5/
+-rw-r--r--   0 jesse      (501) staff       (20)     1103 2023-05-15 09:14:27.000000 ugot-0.1.5/LICENSE
+-rw-r--r--   0 jesse      (501) staff       (20)      612 2023-06-06 03:00:15.779377 ugot-0.1.5/PKG-INFO
+-rwxrwxrwx   0 jesse      (501) staff       (20)      246 2023-05-11 07:07:58.000000 ugot-0.1.5/README.md
+-rwxr-xr-x   0 jesse      (501) staff       (20)      425 2023-06-06 02:57:53.000000 ugot-0.1.5/pyproject.toml
+-rw-r--r--   0 jesse      (501) staff       (20)       38 2023-06-06 03:00:15.779818 ugot-0.1.5/setup.cfg
+-rwxr-xr-x   0 jesse      (501) staff       (20)      558 2023-06-06 02:57:53.000000 ugot-0.1.5/setup.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-06-06 03:00:15.550009 ugot-0.1.5/ugot/
+-rw-r--r--   0 jesse      (501) staff       (20)        0 2023-05-11 07:37:21.000000 ugot-0.1.5/ugot/__init__.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-06-06 03:00:15.676120 ugot-0.1.5/ugot/grpc_pb/
+-rw-r--r--   0 jesse      (501) staff       (20)        0 2023-05-11 07:27:02.000000 ugot-0.1.5/ugot/grpc_pb/__init__.py
+-rw-r--r--   0 jesse      (501) staff       (20)     6021 2023-05-15 03:20:28.000000 ugot-0.1.5/ugot/grpc_pb/audio_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    23990 2023-05-15 03:20:28.000000 ugot-0.1.5/ugot/grpc_pb/audio_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)     6234 2023-05-15 03:20:28.000000 ugot-0.1.5/ugot/grpc_pb/bluetooth_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    18284 2023-05-15 03:20:28.000000 ugot-0.1.5/ugot/grpc_pb/bluetooth_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)     9603 2023-05-15 03:20:28.000000 ugot-0.1.5/ugot/grpc_pb/device_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    30498 2023-05-15 03:20:28.000000 ugot-0.1.5/ugot/grpc_pb/device_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)     6103 2023-05-15 03:20:28.000000 ugot-0.1.5/ugot/grpc_pb/gpio_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    18277 2023-05-15 03:20:28.000000 ugot-0.1.5/ugot/grpc_pb/gpio_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)     8843 2023-06-06 02:56:18.000000 ugot-0.1.5/ugot/grpc_pb/model_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    23309 2023-06-06 02:56:18.000000 ugot-0.1.5/ugot/grpc_pb/model_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)     6803 2023-05-15 03:20:28.000000 ugot-0.1.5/ugot/grpc_pb/network_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    24828 2023-05-15 03:20:28.000000 ugot-0.1.5/ugot/grpc_pb/network_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)     2135 2023-05-15 03:20:28.000000 ugot-0.1.5/ugot/grpc_pb/power_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)     5561 2023-05-15 03:20:28.000000 ugot-0.1.5/ugot/grpc_pb/power_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)     5080 2023-05-15 03:20:28.000000 ugot-0.1.5/ugot/grpc_pb/sensor_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    13911 2023-05-15 03:20:28.000000 ugot-0.1.5/ugot/grpc_pb/sensor_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)    10875 2023-05-15 03:20:28.000000 ugot-0.1.5/ugot/grpc_pb/servo_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    24766 2023-05-15 03:20:28.000000 ugot-0.1.5/ugot/grpc_pb/servo_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)     5891 2023-05-15 03:20:28.000000 ugot-0.1.5/ugot/grpc_pb/vision_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    16618 2023-05-15 03:20:28.000000 ugot-0.1.5/ugot/grpc_pb/vision_pb2_grpc.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-06-06 03:00:15.677482 ugot-0.1.5/ugot/protos/
+-rw-r--r--   0 jesse      (501) staff       (20)        0 2023-05-11 07:27:02.000000 ugot-0.1.5/ugot/protos/__init__.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-06-06 03:00:15.739097 ugot-0.1.5/ugot/src/
+-rw-r--r--   0 jesse      (501) staff       (20)        0 2023-05-11 07:27:02.000000 ugot-0.1.5/ugot/src/__init__.py
+-rw-r--r--   0 jesse      (501) staff       (20)     2674 2023-05-11 07:27:02.000000 ugot-0.1.5/ugot/src/audio_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)      517 2023-05-11 07:27:02.000000 ugot-0.1.5/ugot/src/base_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)      615 2023-05-11 07:27:02.000000 ugot-0.1.5/ugot/src/bluetooth_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)     4159 2023-05-11 07:27:02.000000 ugot-0.1.5/ugot/src/device_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)     5085 2023-05-11 07:27:02.000000 ugot-0.1.5/ugot/src/enum.py
+-rw-r--r--   0 jesse      (501) staff       (20)     3089 2023-05-11 07:27:02.000000 ugot-0.1.5/ugot/src/gpio_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)     8210 2023-06-06 02:56:18.000000 ugot-0.1.5/ugot/src/model_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)     5566 2023-05-11 07:27:02.000000 ugot-0.1.5/ugot/src/network_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)      592 2023-05-11 07:27:02.000000 ugot-0.1.5/ugot/src/power_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)     2294 2023-06-06 02:56:27.000000 ugot-0.1.5/ugot/src/scan_device.py
+-rw-r--r--   0 jesse      (501) staff       (20)     1108 2023-05-11 07:27:02.000000 ugot-0.1.5/ugot/src/sensor_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)     2291 2023-05-11 07:27:02.000000 ugot-0.1.5/ugot/src/servo_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)     4110 2023-05-11 07:27:02.000000 ugot-0.1.5/ugot/src/util.py
+-rw-r--r--   0 jesse      (501) staff       (20)    12490 2023-05-19 07:22:40.000000 ugot-0.1.5/ugot/src/vision_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)    87181 2023-06-06 02:56:27.000000 ugot-0.1.5/ugot/ugot.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-06-06 03:00:15.552472 ugot-0.1.5/ugot.egg-info/
+-rw-r--r--   0 jesse      (501) staff       (20)      612 2023-06-06 03:00:15.000000 ugot-0.1.5/ugot.egg-info/PKG-INFO
+-rw-r--r--   0 jesse      (501) staff       (20)     1206 2023-06-06 03:00:15.000000 ugot-0.1.5/ugot.egg-info/SOURCES.txt
+-rw-r--r--   0 jesse      (501) staff       (20)        1 2023-06-06 03:00:15.000000 ugot-0.1.5/ugot.egg-info/dependency_links.txt
+-rw-r--r--   0 jesse      (501) staff       (20)       67 2023-06-06 03:00:15.000000 ugot-0.1.5/ugot.egg-info/requires.txt
+-rw-r--r--   0 jesse      (501) staff       (20)        5 2023-06-06 03:00:15.000000 ugot-0.1.5/ugot.egg-info/top_level.txt
```

### Comparing `ugot-0.1.4/LICENSE` & `ugot-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/PKG-INFO` & `ugot-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ugot
-Version: 0.1.4
+Version: 0.1.5
 Summary: ugot-Python SDK
 Author-email: Jesse <jesse.huang@ubtrobot.com>
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `ugot-0.1.4/setup.py` & `ugot-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages, find_namespace_packages
 
 setup(
     name = "ugot",
-    version = "0.1.4",
+    version = "0.1.5",
     description = "ugot-Python SDK",
     long_description = "",
 
     packages = find_packages(include=["ugot","ugot.*"]),
     # package_data = {"ugot": ["*"],
     #                 },
     # packages=find_packages(),
```

### Comparing `ugot-0.1.4/ugot/grpc_pb/audio_pb2.py` & `ugot-0.1.5/ugot/grpc_pb/audio_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/grpc_pb/audio_pb2_grpc.py` & `ugot-0.1.5/ugot/grpc_pb/audio_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/grpc_pb/bluetooth_pb2.py` & `ugot-0.1.5/ugot/grpc_pb/bluetooth_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/grpc_pb/bluetooth_pb2_grpc.py` & `ugot-0.1.5/ugot/grpc_pb/bluetooth_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/grpc_pb/device_pb2.py` & `ugot-0.1.5/ugot/grpc_pb/device_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/grpc_pb/device_pb2_grpc.py` & `ugot-0.1.5/ugot/grpc_pb/device_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/grpc_pb/gpio_pb2.py` & `ugot-0.1.5/ugot/grpc_pb/gpio_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/grpc_pb/gpio_pb2_grpc.py` & `ugot-0.1.5/ugot/grpc_pb/gpio_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/grpc_pb/model_pb2.py` & `ugot-0.1.5/ugot/grpc_pb/model_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/grpc_pb/model_pb2_grpc.py` & `ugot-0.1.5/ugot/grpc_pb/model_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/grpc_pb/network_pb2.py` & `ugot-0.1.5/ugot/grpc_pb/network_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/grpc_pb/network_pb2_grpc.py` & `ugot-0.1.5/ugot/grpc_pb/network_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/grpc_pb/power_pb2.py` & `ugot-0.1.5/ugot/grpc_pb/power_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/grpc_pb/power_pb2_grpc.py` & `ugot-0.1.5/ugot/grpc_pb/power_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/grpc_pb/sensor_pb2.py` & `ugot-0.1.5/ugot/grpc_pb/sensor_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/grpc_pb/sensor_pb2_grpc.py` & `ugot-0.1.5/ugot/grpc_pb/sensor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/grpc_pb/servo_pb2.py` & `ugot-0.1.5/ugot/grpc_pb/servo_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/grpc_pb/servo_pb2_grpc.py` & `ugot-0.1.5/ugot/grpc_pb/servo_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/grpc_pb/vision_pb2.py` & `ugot-0.1.5/ugot/grpc_pb/vision_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/grpc_pb/vision_pb2_grpc.py` & `ugot-0.1.5/ugot/grpc_pb/vision_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/src/audio_client.py` & `ugot-0.1.5/ugot/src/audio_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/src/base_client.py` & `ugot-0.1.5/ugot/src/base_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/src/bluetooth_client.py` & `ugot-0.1.5/ugot/src/bluetooth_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/src/device_client.py` & `ugot-0.1.5/ugot/src/device_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/src/enum.py` & `ugot-0.1.5/ugot/src/enum.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/src/gpio_client.py` & `ugot-0.1.5/ugot/src/gpio_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/src/model_client.py` & `ugot-0.1.5/ugot/src/model_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/src/network_client.py` & `ugot-0.1.5/ugot/src/network_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/src/power_client.py` & `ugot-0.1.5/ugot/src/power_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/src/scan_device.py` & `ugot-0.1.5/ugot/src/scan_device.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,16 @@
                 #print("ip: ",  socket.inet_ntoa(info.addresses[0]))
                 device_ip = socket.inet_ntoa(info.addresses[0])
                 self.device_info[result_name] = device_ip
                 DEV_LIST[result_name] = device_ip
 
 class DeviceScan:
     def __init__(self):
+        global DEV_LIST
+        DEV_LIST.clear()
         self.listener = DeviceListener()
         self.device_name_list=[]
         self.device_info_list={}
     def device_discovery(self):
         zeroconf = Zeroconf()
         #当连接wifi的时候服务名不带usb
         browser = ServiceBrowser(zeroconf, "_uExplore_channel_server._tcp.local.", self.listener)
```

### Comparing `ugot-0.1.4/ugot/src/sensor_client.py` & `ugot-0.1.5/ugot/src/sensor_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/src/servo_client.py` & `ugot-0.1.5/ugot/src/servo_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/src/util.py` & `ugot-0.1.5/ugot/src/util.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/src/vision_client.py` & `ugot-0.1.5/ugot/src/vision_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.4/ugot/ugot.py` & `ugot-0.1.5/ugot/ugot.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
         Returns:
             name_list (dict): 格式：{"设备名称1":"IP地址1","设备名称2":"IP地址2",...}
 
         """
         t = threading.Thread(target= self.__scan)
         t.start()
         t.join()
-        print(DEV_LIST)
         return DEV_LIST
 
     def initialize(self, device_ip):
         """初始化设备
 
         通过IP地址初始化相关设备.
```

### Comparing `ugot-0.1.4/ugot.egg-info/PKG-INFO` & `ugot-0.1.5/ugot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ugot
-Version: 0.1.4
+Version: 0.1.5
 Summary: ugot-Python SDK
 Author-email: Jesse <jesse.huang@ubtrobot.com>
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `ugot-0.1.4/ugot.egg-info/SOURCES.txt` & `ugot-0.1.5/ugot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

