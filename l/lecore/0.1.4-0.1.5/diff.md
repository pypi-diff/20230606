# Comparing `tmp/lecore-0.1.4.tar.gz` & `tmp/lecore-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\work\gitlab\le-py-core\package-lecore\dist\.tmp-56p2or5w\lecore-0.1.4.tar", last modified: Tue Jun  6 09:04:02 2023, max compression
+gzip compressed data, was "D:\work\gitlab\le-py-core\package-lecore\dist\.tmp-cp4huyjj\lecore-0.1.5.tar", last modified: Tue Jun  6 09:09:58 2023, max compression
```

## Comparing `lecore-0.1.4.tar` & `lecore-0.1.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 09:04:02.000000 lecore-0.1.4/
--rw-rw-rw-   0        0        0     1091 2023-03-24 15:23:12.000000 lecore-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     1558 2023-06-06 09:04:02.000000 lecore-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1067 2023-03-27 13:17:27.000000 lecore-0.1.4/README.md
--rw-rw-rw-   0        0        0      702 2023-06-06 09:03:49.000000 lecore-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-06 09:04:02.000000 lecore-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-06 09:04:02.000000 lecore-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-06 09:04:02.000000 lecore-0.1.4/src/lecore/
-drwxrwxrwx   0        0        0        0 2023-06-06 09:04:02.000000 lecore-0.1.4/src/lecore/LeBin/
--rw-rw-rw-   0        0        0    12112 2023-01-16 14:47:23.000000 lecore-0.1.4/src/lecore/LeBin/RegisterMap.py
--rw-rw-rw-   0        0        0     4563 2021-08-12 11:01:11.000000 lecore-0.1.4/src/lecore/LeBin/SerialCom.py
--rw-rw-rw-   0        0        0     2933 2020-11-27 14:22:56.000000 lecore-0.1.4/src/lecore/LeBin/UpgradeFirmware.py
--rw-rw-rw-   0        0        0     5339 2021-06-08 08:56:52.000000 lecore-0.1.4/src/lecore/LeBin/VisualLeBin.py
--rw-rw-rw-   0        0        0      156 2023-06-06 09:02:40.000000 lecore-0.1.4/src/lecore/LeBin/__init__.py
--rw-rw-rw-   0        0        0     4973 2023-06-05 14:39:42.000000 lecore-0.1.4/src/lecore/Looger.py
-drwxrwxrwx   0        0        0        0 2023-06-06 09:04:02.000000 lecore-0.1.4/src/lecore/VisualModbus/
--rw-rw-rw-   0        0        0     3452 2020-11-18 16:02:58.000000 lecore-0.1.4/src/lecore/VisualModbus/AppLogging.py
--rw-rw-rw-   0        0        0     1648 2020-11-18 16:02:58.000000 lecore-0.1.4/src/lecore/VisualModbus/Crc32.py
--rw-rw-rw-   0        0        0     2903 2020-05-05 14:10:01.000000 lecore-0.1.4/src/lecore/VisualModbus/HelpAbout.py
--rw-rw-rw-   0        0        0     6975 2023-02-06 16:45:12.000000 lecore-0.1.4/src/lecore/VisualModbus/MbClient.py
--rw-rw-rw-   0        0        0     7821 2023-02-06 16:17:38.000000 lecore-0.1.4/src/lecore/VisualModbus/MbUpgrade.py
--rw-rw-rw-   0        0        0     5083 2020-11-18 16:34:05.000000 lecore-0.1.4/src/lecore/VisualModbus/ReadWrite.py
--rw-rw-rw-   0        0        0    14943 2022-02-25 08:52:05.000000 lecore-0.1.4/src/lecore/VisualModbus/RegMap.py
--rw-rw-rw-   0        0        0     8619 2021-08-09 11:26:31.000000 lecore-0.1.4/src/lecore/VisualModbus/VisualMbApp.py
--rw-rw-rw-   0        0        0     2080 2020-11-18 17:05:27.000000 lecore-0.1.4/src/lecore/VisualModbus/VmSettings.py
--rw-rw-rw-   0        0        0      344 2023-06-05 15:21:12.000000 lecore-0.1.4/src/lecore/VisualModbus/__init__.py
--rw-rw-rw-   0        0        0       28 2023-06-05 14:45:48.000000 lecore-0.1.4/src/lecore/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 09:04:02.000000 lecore-0.1.4/src/lecore.egg-info/
--rw-rw-rw-   0        0        0     1558 2023-06-06 09:04:02.000000 lecore-0.1.4/src/lecore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      831 2023-06-06 09:04:02.000000 lecore-0.1.4/src/lecore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 09:04:02.000000 lecore-0.1.4/src/lecore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-06 09:04:02.000000 lecore-0.1.4/src/lecore.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-06 09:04:02.000000 lecore-0.1.4/src/lecore.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-06 09:04:02.000000 lecore-0.1.4/tests/
--rw-rw-rw-   0        0        0      737 2023-06-05 15:05:22.000000 lecore-0.1.4/tests/test_lebin.py
--rw-rw-rw-   0        0        0     1452 2023-06-05 14:53:08.000000 lecore-0.1.4/tests/test_looger.py
--rw-rw-rw-   0        0        0      733 2023-06-05 15:20:31.000000 lecore-0.1.4/tests/test_modbus.py
+drwxrwxrwx   0        0        0        0 2023-06-06 09:09:58.000000 lecore-0.1.5/
+-rw-rw-rw-   0        0        0     1091 2023-03-24 15:23:12.000000 lecore-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     1558 2023-06-06 09:09:58.000000 lecore-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1067 2023-03-27 13:17:27.000000 lecore-0.1.5/README.md
+-rw-rw-rw-   0        0        0      702 2023-06-06 09:09:38.000000 lecore-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-06 09:09:58.000000 lecore-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-06 09:09:58.000000 lecore-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-06 09:09:58.000000 lecore-0.1.5/src/lecore/
+drwxrwxrwx   0        0        0        0 2023-06-06 09:09:58.000000 lecore-0.1.5/src/lecore/LeBin/
+-rw-rw-rw-   0        0        0    12112 2023-01-16 14:47:23.000000 lecore-0.1.5/src/lecore/LeBin/RegisterMap.py
+-rw-rw-rw-   0        0        0     4563 2021-08-12 11:01:11.000000 lecore-0.1.5/src/lecore/LeBin/SerialCom.py
+-rw-rw-rw-   0        0        0     2933 2020-11-27 14:22:56.000000 lecore-0.1.5/src/lecore/LeBin/UpgradeFirmware.py
+-rw-rw-rw-   0        0        0     5334 2023-06-06 09:06:28.000000 lecore-0.1.5/src/lecore/LeBin/VisualLeBin.py
+-rw-rw-rw-   0        0        0      156 2023-06-06 09:02:40.000000 lecore-0.1.5/src/lecore/LeBin/__init__.py
+-rw-rw-rw-   0        0        0     4973 2023-06-05 14:39:42.000000 lecore-0.1.5/src/lecore/Looger.py
+drwxrwxrwx   0        0        0        0 2023-06-06 09:09:58.000000 lecore-0.1.5/src/lecore/VisualModbus/
+-rw-rw-rw-   0        0        0     3452 2020-11-18 16:02:58.000000 lecore-0.1.5/src/lecore/VisualModbus/AppLogging.py
+-rw-rw-rw-   0        0        0     1648 2020-11-18 16:02:58.000000 lecore-0.1.5/src/lecore/VisualModbus/Crc32.py
+-rw-rw-rw-   0        0        0     2903 2020-05-05 14:10:01.000000 lecore-0.1.5/src/lecore/VisualModbus/HelpAbout.py
+-rw-rw-rw-   0        0        0     6975 2023-02-06 16:45:12.000000 lecore-0.1.5/src/lecore/VisualModbus/MbClient.py
+-rw-rw-rw-   0        0        0     7821 2023-02-06 16:17:38.000000 lecore-0.1.5/src/lecore/VisualModbus/MbUpgrade.py
+-rw-rw-rw-   0        0        0     5083 2020-11-18 16:34:05.000000 lecore-0.1.5/src/lecore/VisualModbus/ReadWrite.py
+-rw-rw-rw-   0        0        0    14943 2022-02-25 08:52:05.000000 lecore-0.1.5/src/lecore/VisualModbus/RegMap.py
+-rw-rw-rw-   0        0        0     8619 2021-08-09 11:26:31.000000 lecore-0.1.5/src/lecore/VisualModbus/VisualMbApp.py
+-rw-rw-rw-   0        0        0     2080 2020-11-18 17:05:27.000000 lecore-0.1.5/src/lecore/VisualModbus/VmSettings.py
+-rw-rw-rw-   0        0        0      344 2023-06-05 15:21:12.000000 lecore-0.1.5/src/lecore/VisualModbus/__init__.py
+-rw-rw-rw-   0        0        0       28 2023-06-05 14:45:48.000000 lecore-0.1.5/src/lecore/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 09:09:58.000000 lecore-0.1.5/src/lecore.egg-info/
+-rw-rw-rw-   0        0        0     1558 2023-06-06 09:09:58.000000 lecore-0.1.5/src/lecore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      831 2023-06-06 09:09:58.000000 lecore-0.1.5/src/lecore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 09:09:58.000000 lecore-0.1.5/src/lecore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-06 09:09:58.000000 lecore-0.1.5/src/lecore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-06 09:09:58.000000 lecore-0.1.5/src/lecore.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 09:09:58.000000 lecore-0.1.5/tests/
+-rw-rw-rw-   0        0        0      717 2023-06-06 09:09:29.000000 lecore-0.1.5/tests/test_lebin.py
+-rw-rw-rw-   0        0        0     1452 2023-06-05 14:53:08.000000 lecore-0.1.5/tests/test_looger.py
+-rw-rw-rw-   0        0        0      733 2023-06-05 15:20:31.000000 lecore-0.1.5/tests/test_modbus.py
```

### Comparing `lecore-0.1.4/LICENSE` & `lecore-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lecore-0.1.4/PKG-INFO` & `lecore-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lecore
-Version: 0.1.4
+Version: 0.1.5
 Summary: Logic Elements core utilities
 Author-email: Jan Bartovský <jan.bartovsky@logicelements.cz>
 Project-URL: Homepage, http://www.logicelements.cz
 Keywords: logicelements,looger,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lecore-0.1.4/README.md` & `lecore-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `lecore-0.1.4/src/lecore/LeBin/RegisterMap.py` & `lecore-0.1.5/src/lecore/LeBin/RegisterMap.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.4/src/lecore/LeBin/SerialCom.py` & `lecore-0.1.5/src/lecore/LeBin/SerialCom.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.4/src/lecore/LeBin/UpgradeFirmware.py` & `lecore-0.1.5/src/lecore/LeBin/UpgradeFirmware.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.4/src/lecore/LeBin/VisualLeBin.py` & `lecore-0.1.5/src/lecore/LeBin/VisualLeBin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from LeBin.RegisterMap import *
+from .RegisterMap import *
 import PySimpleGUI as SG
 
 
 class VisualLeBin:
     """
     Visual application for LeBin protocol with serial communication
     """
```

### Comparing `lecore-0.1.4/src/lecore/Looger.py` & `lecore-0.1.5/src/lecore/Looger.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.4/src/lecore/VisualModbus/AppLogging.py` & `lecore-0.1.5/src/lecore/VisualModbus/AppLogging.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.4/src/lecore/VisualModbus/Crc32.py` & `lecore-0.1.5/src/lecore/VisualModbus/Crc32.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.4/src/lecore/VisualModbus/HelpAbout.py` & `lecore-0.1.5/src/lecore/VisualModbus/HelpAbout.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.4/src/lecore/VisualModbus/MbClient.py` & `lecore-0.1.5/src/lecore/VisualModbus/MbClient.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.4/src/lecore/VisualModbus/MbUpgrade.py` & `lecore-0.1.5/src/lecore/VisualModbus/MbUpgrade.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.4/src/lecore/VisualModbus/ReadWrite.py` & `lecore-0.1.5/src/lecore/VisualModbus/ReadWrite.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.4/src/lecore/VisualModbus/RegMap.py` & `lecore-0.1.5/src/lecore/VisualModbus/RegMap.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.4/src/lecore/VisualModbus/VisualMbApp.py` & `lecore-0.1.5/src/lecore/VisualModbus/VisualMbApp.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.4/src/lecore/VisualModbus/VmSettings.py` & `lecore-0.1.5/src/lecore/VisualModbus/VmSettings.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.4/src/lecore.egg-info/PKG-INFO` & `lecore-0.1.5/src/lecore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lecore
-Version: 0.1.4
+Version: 0.1.5
 Summary: Logic Elements core utilities
 Author-email: Jan Bartovský <jan.bartovsky@logicelements.cz>
 Project-URL: Homepage, http://www.logicelements.cz
 Keywords: logicelements,looger,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lecore-0.1.4/src/lecore.egg-info/SOURCES.txt` & `lecore-0.1.5/src/lecore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lecore-0.1.4/tests/test_lebin.py` & `lecore-0.1.5/tests/test_lebin.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 
 try:
     import lecore.LeBin as LeBin
 except ImportError:
     import src.lecore.LeBin as LeBin
 
 
+
 class TestSimple(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
         """
         Create instance of looger class
         """
-        com = LeBin.SerialCom.SerialCom()
+        com = LeBin.SerialCom()
         cls.com = com
-        cls.rm = LeBin.RegisterMap.RegisterMap(com)
+        cls.rm = LeBin.RegisterMap(com)
 
     def setUp(self) -> None:
         """
         Insert just some delay between tests
         """
         sleep(1)
```

### Comparing `lecore-0.1.4/tests/test_looger.py` & `lecore-0.1.5/tests/test_looger.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.4/tests/test_modbus.py` & `lecore-0.1.5/tests/test_modbus.py`

 * *Files identical despite different names*

