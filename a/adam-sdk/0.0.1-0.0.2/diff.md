# Comparing `tmp/adam-sdk-0.0.1.tar.gz` & `tmp/adam-sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adam-sdk-0.0.1.tar", last modified: Mon Jun  5 23:56:09 2023, max compression
+gzip compressed data, was "adam-sdk-0.0.2.tar", last modified: Tue Jun  6 10:54:44 2023, max compression
```

## Comparing `adam-sdk-0.0.1.tar` & `adam-sdk-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 23:56:09.976104 adam-sdk-0.0.1/
--rw-rw-rw-   0        0        0      468 2023-06-05 23:56:09.976104 adam-sdk-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       23 2023-06-05 22:18:33.000000 adam-sdk-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 23:56:09.956104 adam-sdk-0.0.1/adam_sdk/
--rw-rw-rw-   0        0        0     4175 2023-06-05 22:31:29.000000 adam-sdk-0.0.1/adam_sdk/AdamManager.py
-drwxrwxrwx   0        0        0        0 2023-06-05 23:56:09.972104 adam-sdk-0.0.1/adam_sdk/Controllers/
--rw-rw-rw-   0        0        0     1551 2023-06-05 22:18:51.000000 adam-sdk-0.0.1/adam_sdk/Controllers/JointController.py
--rw-rw-rw-   0        0        0     5682 2023-06-05 22:25:49.000000 adam-sdk-0.0.1/adam_sdk/Controllers/MecanumMoveController.py
--rw-rw-rw-   0        0        0     1742 2023-06-05 22:33:58.000000 adam-sdk-0.0.1/adam_sdk/JsonParser.py
-drwxrwxrwx   0        0        0        0 2023-06-05 23:56:09.975105 adam-sdk-0.0.1/adam_sdk/Models/
--rw-rw-rw-   0        0        0      247 2023-06-05 22:31:09.000000 adam-sdk-0.0.1/adam_sdk/Models/IMoveController.py
--rw-rw-rw-   0        0        0      332 2023-06-05 22:18:51.000000 adam-sdk-0.0.1/adam_sdk/Models/Joint.py
--rw-rw-rw-   0        0        0      452 2023-06-05 22:18:51.000000 adam-sdk-0.0.1/adam_sdk/Models/Motor.py
--rw-rw-rw-   0        0        0      260 2023-06-05 22:18:51.000000 adam-sdk-0.0.1/adam_sdk/Models/MotorCommand.py
--rw-rw-rw-   0        0        0       77 2023-06-05 22:18:51.000000 adam-sdk-0.0.1/adam_sdk/Models/MotorEnum.py
--rw-rw-rw-   0        0        0      225 2023-06-05 22:25:49.000000 adam-sdk-0.0.1/adam_sdk/Models/SerializableCommands.py
--rw-rw-rw-   0        0        0     2404 2023-06-05 22:30:22.000000 adam-sdk-0.0.1/adam_sdk/ServoConnection.py
--rw-rw-rw-   0        0        0      518 2023-06-05 22:31:49.000000 adam-sdk-0.0.1/adam_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 23:56:09.971104 adam-sdk-0.0.1/adam_sdk.egg-info/
--rw-rw-rw-   0        0        0      468 2023-06-05 23:56:09.000000 adam-sdk-0.0.1/adam_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      545 2023-06-05 23:56:09.000000 adam-sdk-0.0.1/adam_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 23:56:09.000000 adam-sdk-0.0.1/adam_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-06-05 23:56:09.000000 adam-sdk-0.0.1/adam_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-05 23:56:09.000000 adam-sdk-0.0.1/adam_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 23:56:09.976104 adam-sdk-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      807 2023-06-05 23:54:11.000000 adam-sdk-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:54:44.680461 adam-sdk-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-06-06 00:09:38.000000 adam-sdk-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      491 2023-06-06 10:54:44.680461 adam-sdk-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       23 2023-06-05 22:18:33.000000 adam-sdk-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 10:54:44.672460 adam-sdk-0.0.2/adam_sdk/
+-rw-rw-rw-   0        0        0     4175 2023-06-05 22:31:29.000000 adam-sdk-0.0.2/adam_sdk/AdamManager.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:54:44.676459 adam-sdk-0.0.2/adam_sdk/Controllers/
+-rw-rw-rw-   0        0        0     1551 2023-06-05 22:18:51.000000 adam-sdk-0.0.2/adam_sdk/Controllers/JointController.py
+-rw-rw-rw-   0        0        0     2453 2023-06-06 05:40:02.000000 adam-sdk-0.0.2/adam_sdk/Controllers/MecanumMoveController.py
+-rw-rw-rw-   0        0        0     3719 2023-06-06 10:43:34.000000 adam-sdk-0.0.2/adam_sdk/Controllers/MotorController.py
+-rw-rw-rw-   0        0        0     1721 2023-06-06 01:37:42.000000 adam-sdk-0.0.2/adam_sdk/JsonParser.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:54:44.679458 adam-sdk-0.0.2/adam_sdk/Models/
+-rw-rw-rw-   0        0        0      247 2023-06-05 22:31:09.000000 adam-sdk-0.0.2/adam_sdk/Models/IMoveController.py
+-rw-rw-rw-   0        0        0      332 2023-06-05 22:18:51.000000 adam-sdk-0.0.2/adam_sdk/Models/Joint.py
+-rw-rw-rw-   0        0        0      452 2023-06-05 22:18:51.000000 adam-sdk-0.0.2/adam_sdk/Models/Motor.py
+-rw-rw-rw-   0        0        0      260 2023-06-05 22:18:51.000000 adam-sdk-0.0.2/adam_sdk/Models/MotorCommand.py
+-rw-rw-rw-   0        0        0       77 2023-06-05 22:18:51.000000 adam-sdk-0.0.2/adam_sdk/Models/MotorEnum.py
+-rw-rw-rw-   0        0        0      225 2023-06-05 22:25:49.000000 adam-sdk-0.0.2/adam_sdk/Models/SerializableCommands.py
+-rw-rw-rw-   0        0        0     2404 2023-06-05 22:30:22.000000 adam-sdk-0.0.2/adam_sdk/ServoConnection.py
+-rw-rw-rw-   0        0        0      582 2023-06-06 05:40:02.000000 adam-sdk-0.0.2/adam_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:54:44.675460 adam-sdk-0.0.2/adam_sdk.egg-info/
+-rw-rw-rw-   0        0        0      491 2023-06-06 10:54:44.000000 adam-sdk-0.0.2/adam_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      593 2023-06-06 10:54:44.000000 adam-sdk-0.0.2/adam_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 10:54:44.000000 adam-sdk-0.0.2/adam_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-06 10:54:44.000000 adam-sdk-0.0.2/adam_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-06 10:54:44.000000 adam-sdk-0.0.2/adam_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 10:54:44.680461 adam-sdk-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      807 2023-06-06 10:54:44.000000 adam-sdk-0.0.2/setup.py
```

### Comparing `adam-sdk-0.0.1/adam_sdk/AdamManager.py` & `adam-sdk-0.0.2/adam_sdk/AdamManager.py`

 * *Files identical despite different names*

### Comparing `adam-sdk-0.0.1/adam_sdk/Controllers/JointController.py` & `adam-sdk-0.0.2/adam_sdk/Controllers/JointController.py`

 * *Files identical despite different names*

### Comparing `adam-sdk-0.0.1/adam_sdk/JsonParser.py` & `adam-sdk-0.0.2/adam_sdk/JsonParser.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 current = os.path.dirname(os.path.realpath(__file__))
 
 class JsonParser:
 
     @staticmethod
     def _read_config():
-        config_file_path = f"{os.environ.get('ADAM_CONFIGS_PATH')}/servo_range.config"
+        config_file_path = "/etc/adam_configs/servo_range.config"
         
         if os.path.isfile(config_file_path) is False:
             config_file_path = f'{current}/../examples/position_range.json'
         file = open(config_file_path)
         data = json.load(file)
         file.close()
```

### Comparing `adam-sdk-0.0.1/adam_sdk/ServoConnection.py` & `adam-sdk-0.0.2/adam_sdk/ServoConnection.py`

 * *Files identical despite different names*

### Comparing `adam-sdk-0.0.1/adam_sdk/__init__.py` & `adam-sdk-0.0.2/adam_sdk/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .AdamManager import AdamManager
 from .JsonParser import JsonParser
 from .ServoConnection import ServoConnection
 from .Controllers.JointController import JointController
 from .Controllers.MecanumMoveController import MecanumMoveController
+from .Controllers.MecanumMoveController import MotorController
 from .Models.IMoveController import IMoveController
 from .Models.Joint import Joint
 from .Models.MotorCommand import MotorCommand
 from .Models.MotorEnum import MotorEnum
 from .Models.Motor import Motor
 from .Models.SerializableCommands import SerializableCommands
```

### Comparing `adam-sdk-0.0.1/adam_sdk.egg-info/SOURCES.txt` & `adam-sdk-0.0.2/adam_sdk.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+LICENSE
 README.md
 setup.py
 adam_sdk/AdamManager.py
 adam_sdk/JsonParser.py
 adam_sdk/ServoConnection.py
 adam_sdk/__init__.py
 adam_sdk.egg-info/PKG-INFO
 adam_sdk.egg-info/SOURCES.txt
 adam_sdk.egg-info/dependency_links.txt
 adam_sdk.egg-info/requires.txt
 adam_sdk.egg-info/top_level.txt
 adam_sdk/Controllers/JointController.py
 adam_sdk/Controllers/MecanumMoveController.py
+adam_sdk/Controllers/MotorController.py
 adam_sdk/Models/IMoveController.py
 adam_sdk/Models/Joint.py
 adam_sdk/Models/Motor.py
 adam_sdk/Models/MotorCommand.py
 adam_sdk/Models/MotorEnum.py
 adam_sdk/Models/SerializableCommands.py
```

### Comparing `adam-sdk-0.0.1/setup.py` & `adam-sdk-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='adam-sdk',
-    version='0.0.1',
+    version='0.0.2',
     packages=['adam_sdk', 'adam_sdk.Controllers', 'adam_sdk.Models'],
     url='https://github.com/Adam-Software/Adam-SDK',
     license='MIT',
     author='Adam Software',
     author_email='a@nesterof.com',
     description='SDK for robot Adam',
     long_description_content_type="text/markdown",
```

