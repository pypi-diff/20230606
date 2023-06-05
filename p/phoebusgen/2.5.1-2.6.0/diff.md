# Comparing `tmp/phoebusgen-2.5.1.tar.gz` & `tmp/phoebusgen-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phoebusgen-2.5.1.tar", last modified: Fri Apr 14 00:07:22 2023, max compression
+gzip compressed data, was "phoebusgen-2.6.0.tar", last modified: Mon Jun  5 23:39:14 2023, max compression
```

## Comparing `phoebusgen-2.5.1.tar` & `phoebusgen-2.6.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:07:22.565672 phoebusgen-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-14 00:07:22.565672 phoebusgen-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:07:22.569672 phoebusgen-2.5.1/phoebusgen/
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/phoebusgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/phoebusgen/_shared_property_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-14 00:07:22.569672 phoebusgen-2.5.1/phoebusgen/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:07:22.565672 phoebusgen-2.5.1/phoebusgen/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/phoebusgen/config/classes.bcf
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/phoebusgen/config/color.def
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/phoebusgen/config/font.def
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:07:22.565672 phoebusgen-2.5.1/phoebusgen/screen/
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/phoebusgen/screen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/phoebusgen/screen/screen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:07:22.565672 phoebusgen-2.5.1/phoebusgen/widget/
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/phoebusgen/widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    65736 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/phoebusgen/widget/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/phoebusgen/widget/widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    27623 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/phoebusgen/widget/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:07:22.565672 phoebusgen-2.5.1/phoebusgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-14 00:07:22.000000 phoebusgen-2.5.1/phoebusgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-14 00:07:22.000000 phoebusgen-2.5.1/phoebusgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 00:07:22.000000 phoebusgen-2.5.1/phoebusgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-14 00:07:22.000000 phoebusgen-2.5.1/phoebusgen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-14 00:07:22.569672 phoebusgen-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:07:22.565672 phoebusgen-2.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/tests/test_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)    10648 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    22178 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/tests/test_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-04-14 00:07:10.000000 phoebusgen-2.5.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:39:14.021391 phoebusgen-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-06-05 23:39:14.021391 phoebusgen-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:39:14.021391 phoebusgen-2.6.0/phoebusgen/
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/phoebusgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/phoebusgen/_shared_property_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-05 23:39:14.021391 phoebusgen-2.6.0/phoebusgen/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:39:14.021391 phoebusgen-2.6.0/phoebusgen/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/phoebusgen/config/classes.bcf
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/phoebusgen/config/color.def
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/phoebusgen/config/font.def
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:39:14.021391 phoebusgen-2.6.0/phoebusgen/screen/
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/phoebusgen/screen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/phoebusgen/screen/screen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:39:14.021391 phoebusgen-2.6.0/phoebusgen/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/phoebusgen/widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65736 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/phoebusgen/widget/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/phoebusgen/widget/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27640 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/phoebusgen/widget/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:39:14.017391 phoebusgen-2.6.0/phoebusgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-06-05 23:39:14.000000 phoebusgen-2.6.0/phoebusgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-05 23:39:14.000000 phoebusgen-2.6.0/phoebusgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 23:39:14.000000 phoebusgen-2.6.0/phoebusgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-05 23:39:14.000000 phoebusgen-2.6.0/phoebusgen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-05 23:39:14.021391 phoebusgen-2.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:39:14.021391 phoebusgen-2.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/tests/test_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10648 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22198 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/tests/test_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/versioneer.py
```

### Comparing `phoebusgen-2.5.1/LICENSE` & `phoebusgen-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.5.1/PKG-INFO` & `phoebusgen-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phoebusgen
-Version: 2.5.1
+Version: 2.6.0
 Summary: Control screen generator for Phoebus
 Home-page: https://github.com/tynanford/phoebusgen
 Author: Tynan Ford
 Author-email: tford@lbl.gov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```

### Comparing `phoebusgen-2.5.1/README.md` & `phoebusgen-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.5.1/phoebusgen/__init__.py` & `phoebusgen-2.6.0/phoebusgen/__init__.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.5.1/phoebusgen/_shared_property_helpers.py` & `phoebusgen-2.6.0/phoebusgen/_shared_property_helpers.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.5.1/phoebusgen/config/classes.bcf` & `phoebusgen-2.6.0/phoebusgen/config/classes.bcf`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.5.1/phoebusgen/config/color.def` & `phoebusgen-2.6.0/phoebusgen/config/color.def`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.5.1/phoebusgen/config/font.def` & `phoebusgen-2.6.0/phoebusgen/config/font.def`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.5.1/phoebusgen/screen/__init__.py` & `phoebusgen-2.6.0/phoebusgen/screen/__init__.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.5.1/phoebusgen/screen/screen.py` & `phoebusgen-2.6.0/phoebusgen/screen/screen.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.5.1/phoebusgen/widget/__init__.py` & `phoebusgen-2.6.0/phoebusgen/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.5.1/phoebusgen/widget/properties.py` & `phoebusgen-2.6.0/phoebusgen/widget/properties.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.5.1/phoebusgen/widget/widget.py` & `phoebusgen-2.6.0/phoebusgen/widget/widget.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.5.1/phoebusgen/widget/widgets.py` & `phoebusgen-2.6.0/phoebusgen/widget/widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,15 +261,15 @@
         :param height: Widget height
         """
         _Widget.__init__(self, 'text-symbol', name, x, y, width, height)
         self.pv_name(pv_name)
 
 class TextUpdate(_Widget, _p._PVName, _p._Font, _p._ForegroundColor, _p._BackgroundColor, _p._Transparent,
                  _p._Format, _p._Precision, _p._ShowUnits, _p._HorizontalAlignment, _p._VerticalAlignment, _p._WrapWords,
-                 _p._RotationStep, _p._Border):
+                 _p._RotationStep, _p._Border, _p._AlarmBorder):
     """ TextUpdate Phoebus Widget """
     def __init__(self, name: str, pv_name: str, x: int, y: int, width: int, height: int) -> None:
         """
         Create TextUpdate Widget
 
         :param name: Widget name
         :param pv_name: Widget PV
```

### Comparing `phoebusgen-2.5.1/phoebusgen.egg-info/PKG-INFO` & `phoebusgen-2.6.0/phoebusgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phoebusgen
-Version: 2.5.1
+Version: 2.6.0
 Summary: Control screen generator for Phoebus
 Home-page: https://github.com/tynanford/phoebusgen
 Author: Tynan Ford
 Author-email: tford@lbl.gov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```

### Comparing `phoebusgen-2.5.1/phoebusgen.egg-info/SOURCES.txt` & `phoebusgen-2.6.0/phoebusgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.5.1/setup.py` & `phoebusgen-2.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.5.1/tests/test_screen.py` & `phoebusgen-2.6.0/tests/test_screen.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.5.1/tests/test_widget.py` & `phoebusgen-2.6.0/tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.5.1/tests/test_widgets.py` & `phoebusgen-2.6.0/tests/test_widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
         self.pv_name = 'symbol'
         self.element = widgets.TextSymbol(self.name, self.pv_name, self.x, self.y, self.width, self.height)
 
 
 class TestTextUpdate(unittest.TestCase, ph.TestPVName, ph.TestFont, ph.TestForegroundColor,
                           ph.TestBackgroundColor, ph.TestTransparent, ph.TestFormat, ph.TestPrecision,
                           ph.TestShowUnits, ph.TestHorizontalAlignment, ph.TestVerticalAlignment,
-                          ph.TestWrapWords, ph.TestRotationStep, ph.TestBorder):
+                          ph.TestWrapWords, ph.TestRotationStep, ph.TestBorder, ph.TestAlarmBorder):
     def setUp(self):
         self.pv_name = 'TEST:ME'
         self.name = 'Generic TextUpdate'
         self.type = 'textupdate'
         self.x = 500
         self.y = 300
         self.width = 100
```

### Comparing `phoebusgen-2.5.1/versioneer.py` & `phoebusgen-2.6.0/versioneer.py`

 * *Files identical despite different names*

