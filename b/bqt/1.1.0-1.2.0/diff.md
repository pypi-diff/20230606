# Comparing `tmp/bqt-1.1.0.tar.gz` & `tmp/bqt-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bqt-1.1.0.tar", last modified: Tue Jun  6 12:32:43 2023, max compression
+gzip compressed data, was "bqt-1.2.0.tar", last modified: Tue Jun  6 14:44:43 2023, max compression
```

## Comparing `bqt-1.1.0.tar` & `bqt-1.2.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:32:43.861122 bqt-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-06 12:32:34.000000 bqt-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-06 12:32:34.000000 bqt-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-06-06 12:32:43.861122 bqt-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-06 12:32:34.000000 bqt-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:32:43.857123 bqt-1.1.0/bqt/
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:32:43.861122 bqt-1.1.0/bqt/blender_applications/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/blender_applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/blender_applications/blender_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/blender_applications/darwin_blender_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/blender_applications/win32_blender_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/blender_stylesheet.qss
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/focus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:32:43.861122 bqt-1.1.0/bqt/images/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/images/QCheckBox_checked.png
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/images/QCheckBox_unchecked.png
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/images/QCheckbox_checked_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/images/QCheckbox_unchecked_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/images/QComboBox_down_arrow.png
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/images/QRadioButton_checked.png
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/images/QRadioButton_checked_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/images/QRadioButton_unchecked.png
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/images/QRadioButton_unchecked_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/images/QSpinBox_down_arrow.png
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/images/QSpinBox_up_arrow.png
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/images/blender_icon_16.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:32:43.861122 bqt-1.1.0/bqt/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/ui/quit_dialogue.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/widget_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:32:43.861122 bqt-1.1.0/bqt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-06-06 12:32:43.000000 bqt-1.1.0/bqt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-06 12:32:43.000000 bqt-1.1.0/bqt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 12:32:43.000000 bqt-1.1.0/bqt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 12:32:43.000000 bqt-1.1.0/bqt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-06 12:32:43.000000 bqt-1.1.0/bqt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 12:32:43.861122 bqt-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-06 12:32:34.000000 bqt-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:44:43.911776 bqt-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-06 14:44:34.000000 bqt-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-06 14:44:34.000000 bqt-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-06 14:44:43.911776 bqt-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-06 14:44:34.000000 bqt-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:44:43.903776 bqt-1.2.0/bqt/
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:44:43.907776 bqt-1.2.0/bqt/blender_applications/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/blender_applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/blender_applications/blender_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/blender_applications/darwin_blender_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/blender_applications/win32_blender_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/blender_stylesheet.qss
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/focus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:44:43.911776 bqt-1.2.0/bqt/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/images/QCheckBox_checked.png
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/images/QCheckBox_unchecked.png
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/images/QCheckbox_checked_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/images/QCheckbox_unchecked_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/images/QComboBox_down_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/images/QRadioButton_checked.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/images/QRadioButton_checked_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/images/QRadioButton_unchecked.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/images/QRadioButton_unchecked_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/images/QSpinBox_down_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/images/QSpinBox_up_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/images/blender_icon_16.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:44:43.911776 bqt-1.2.0/bqt/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/ui/quit_dialogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/widget_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:44:43.903776 bqt-1.2.0/bqt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-06 14:44:43.000000 bqt-1.2.0/bqt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-06 14:44:43.000000 bqt-1.2.0/bqt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:44:43.000000 bqt-1.2.0/bqt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 14:44:43.000000 bqt-1.2.0/bqt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-06 14:44:43.000000 bqt-1.2.0/bqt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 14:44:43.911776 bqt-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-06 14:44:34.000000 bqt-1.2.0/setup.py
```

### Comparing `bqt-1.1.0/LICENSE` & `bqt-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bqt-1.1.0/PKG-INFO` & `bqt-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bqt
-Version: 1.1.0
+Version: 1.2.0
 Summary: Files to help bootstrap PySide2 with an event loop within Blender.
 Home-page: https://github.com/techartorg/bqt
 Author: tech-artists.org
 License: Mozilla Public License 2.0 (MPL 2.0)
 Keywords: Technical,Art,TechArt,TechArtOrg,Blender,Qt,PySide
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -66,25 +66,30 @@
 Any updates in the repo are then reflected in blender on restart.
 e.g.:
 ```commandline
 mklink /J "C:\Users\USERNAME\AppData\Roaming\Blender Foundation\Blender\2.93\scripts\addons\bqt" "C:\Users\hanne\OneDrive\Documents\repos\_Blender\bqt\bqt"
 ```
 
 ### Environment variables
+
 | variable | description|
 |--|--|
 |BQT_DISABLE_STARTUP| if set to `1`, completely disable bqt|
 |BQT_DISABLE_WRAP| if set to `1`, disable wrapping blender in a QWindow|
 |BQT_DISABLE_CLOSE_DIALOGUE| if set to `1`, use the standard blender close dialogue|
 |BQT_MANAGE_FOREGROUND| defaults to `1`, if `0`, widgets registered with `bqt.add(my_widget)` won't stay in the foreground when using Blender.|
-if you modify env vars, ensure they're strings
+|BQT_AUTO_ADD| defaults to `1`, if `0` top level widgets won't automatically be added to bqt.|
+
+- if you modify env vars, ensure they're strings
+- if you're unsure how to set env vars, google `set environment variable windows`.
+- Restart Blender (or your computer) after changing them.
 
 ### Sample code
 [bqt_demo](bqt_demo) shows you how to use bqt with several qt demos you can run in Blender
 
 ### Community
 Discuss BQT on 
 - the BlenderArtists [thread](https://blenderartists.org/t/bqt-custom-ui-for-add-ons-tool-in-blender-with-pyqt-or-pyside/1458808)
 - [Ynput  thread](https://community.ynput.io/t/use-bqt-for-blender-qt-integration/127)
 
-### ALternative
+### Alternative
 - Custom UI for Blender only: https://github.com/mmmrqs/bl_ui_widgets
```

### Comparing `bqt-1.1.0/README.md` & `bqt-1.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -50,25 +50,30 @@
 Any updates in the repo are then reflected in blender on restart.
 e.g.:
 ```commandline
 mklink /J "C:\Users\USERNAME\AppData\Roaming\Blender Foundation\Blender\2.93\scripts\addons\bqt" "C:\Users\hanne\OneDrive\Documents\repos\_Blender\bqt\bqt"
 ```
 
 ### Environment variables
+
 | variable | description|
 |--|--|
 |BQT_DISABLE_STARTUP| if set to `1`, completely disable bqt|
 |BQT_DISABLE_WRAP| if set to `1`, disable wrapping blender in a QWindow|
 |BQT_DISABLE_CLOSE_DIALOGUE| if set to `1`, use the standard blender close dialogue|
 |BQT_MANAGE_FOREGROUND| defaults to `1`, if `0`, widgets registered with `bqt.add(my_widget)` won't stay in the foreground when using Blender.|
-if you modify env vars, ensure they're strings
+|BQT_AUTO_ADD| defaults to `1`, if `0` top level widgets won't automatically be added to bqt.|
+
+- if you modify env vars, ensure they're strings
+- if you're unsure how to set env vars, google `set environment variable windows`.
+- Restart Blender (or your computer) after changing them.
 
 ### Sample code
 [bqt_demo](bqt_demo) shows you how to use bqt with several qt demos you can run in Blender
 
 ### Community
 Discuss BQT on 
 - the BlenderArtists [thread](https://blenderartists.org/t/bqt-custom-ui-for-add-ons-tool-in-blender-with-pyqt-or-pyside/1458808)
 - [Ynput  thread](https://community.ynput.io/t/use-bqt-for-blender-qt-integration/127)
 
-### ALternative
+### Alternative
 - Custom UI for Blender only: https://github.com/mmmrqs/bl_ui_widgets
```

### Comparing `bqt-1.1.0/bqt/__init__.py` & `bqt-1.2.0/bqt/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 This Source Code Form is subject to the terms of the Mozilla Public
 License, v. 2.0. If a copy of the MPL was not distributed with this
 file, You can obtain one at https://mozilla.org/MPL/2.0/.
 """
 import bqt
 import bqt.focus
+import bqt.widget_manager
 import os
 import sys
 import bpy
 import PySide2.QtCore as QtCore
 from PySide2.QtWidgets import QApplication
 from PySide2.QtCore import QDir
 import logging
@@ -25,14 +26,15 @@
         # "warning": "", # used for warning icon and text in add-ons panel
         # "wiki_url": "http://my.wiki.url",
         # "tracker_url": "http://my.bugtracker.url",
         "support": "COMMUNITY",
         "category": "UI"
         }
 
+register = bqt.widget_manager.register
 
 # CORE FUNCTIONS #
 
 def _instantiate_QApplication() -> "bqt.blender_applications.BlenderApplication":
     # enable dpi scale, run before creating QApplication
     QApplication.setHighDpiScaleFactorRoundingPolicy(QtCore.Qt.HighDpiScaleFactorRoundingPolicy.PassThrough)
     QApplication.setAttribute(QtCore.Qt.AA_EnableHighDpiScaling)
```

### Comparing `bqt-1.1.0/bqt/blender_applications/__init__.py` & `bqt-1.2.0/bqt/blender_applications/__init__.py`

 * *Files identical despite different names*

### Comparing `bqt-1.1.0/bqt/blender_applications/blender_application.py` & `bqt-1.2.0/bqt/blender_applications/blender_application.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,38 +42,45 @@
 
         QApplication.setWindowIcon(self._get_application_icon())
 
         # Blender Window
         self._hwnd = self._get_blender_hwnd()
         failed_to_get_handle = self._hwnd is None
 
+        self.window_container: QWidget = None
+
         if os.getenv("BQT_DISABLE_WRAP") == "1" or failed_to_get_handle:
             self._blender_window = QWindow()
             self.blender_widget = QWidget.createWindowContainer(self._blender_window)
         else:
             self.blender_widget = QMainWindow()
             self.blender_widget.setWindowTitle(WINDOW_TITLE)
             self._blender_window = QWindow.fromWinId(self._hwnd)  # also sets flag to Qt.ForeignWindow
             self.window_container = QMainWindow.createWindowContainer(self._blender_window)
             self.blender_widget.setCentralWidget(self.window_container)
 
             self._set_window_geometry()
             self.blender_widget.show()
             self.focusObjectChanged.connect(self._on_focus_object_changed)
 
+        # hookup event loop
         self.timer = QTimer()
         self.timer.timeout.connect(self.on_update)
         tick = int(1000 / FOCUS_FRAMERATE)  # tick 1000 / frames per second
         self.timer.start(tick)
 
     def on_update(self):
+        """qt event loop"""
         # we only need foreground managing if blender is not wrapped
         if os.getenv("BQT_DISABLE_WRAP") == "1" and os.getenv("BQT_MANAGE_FOREGROUND", "1") == "1" and self.blender_focus_toggled():
             bqt.widget_manager._blender_window_change(self._active_window_hwnd)
 
+        if os.getenv("BQT_AUTO_ADD", "1") == "1":
+            bqt.widget_manager.parent_orphan_widgets(exclude=[self.blender_widget, self._blender_window, self.window_container])  # auto parent any orphaned widgets
+
     def blender_focus_toggled(self):
         """returns true the first frame the blender window is focussed or unfoccused"""
         current_active_hwnd = self._get_active_window_handle()
         handle_changed = self._active_window_hwnd != current_active_hwnd
         if not handle_changed:
             self._active_window_hwnd = current_active_hwnd
             return False
```

### Comparing `bqt-1.1.0/bqt/blender_applications/darwin_blender_application.py` & `bqt-1.2.0/bqt/blender_applications/darwin_blender_application.py`

 * *Files identical despite different names*

### Comparing `bqt-1.1.0/bqt/blender_applications/win32_blender_application.py` & `bqt-1.2.0/bqt/blender_applications/win32_blender_application.py`

 * *Files identical despite different names*

### Comparing `bqt-1.1.0/bqt/blender_stylesheet.qss` & `bqt-1.2.0/bqt/blender_stylesheet.qss`

 * *Files identical despite different names*

### Comparing `bqt-1.1.0/bqt/focus.py` & `bqt-1.2.0/bqt/focus.py`

 * *Files identical despite different names*

### Comparing `bqt-1.1.0/bqt/images/QCheckBox_checked.png` & `bqt-1.2.0/bqt/images/QCheckBox_checked.png`

 * *Files identical despite different names*

### Comparing `bqt-1.1.0/bqt/images/QCheckBox_unchecked.png` & `bqt-1.2.0/bqt/images/QCheckBox_unchecked.png`

 * *Files identical despite different names*

### Comparing `bqt-1.1.0/bqt/images/QCheckbox_checked_hover.png` & `bqt-1.2.0/bqt/images/QCheckbox_checked_hover.png`

 * *Files identical despite different names*

### Comparing `bqt-1.1.0/bqt/images/QCheckbox_unchecked_hover.png` & `bqt-1.2.0/bqt/images/QCheckbox_unchecked_hover.png`

 * *Files identical despite different names*

### Comparing `bqt-1.1.0/bqt/images/QComboBox_down_arrow.png` & `bqt-1.2.0/bqt/images/QComboBox_down_arrow.png`

 * *Files identical despite different names*

### Comparing `bqt-1.1.0/bqt/images/QRadioButton_checked.png` & `bqt-1.2.0/bqt/images/QRadioButton_checked.png`

 * *Files identical despite different names*

### Comparing `bqt-1.1.0/bqt/images/QRadioButton_checked_hover.png` & `bqt-1.2.0/bqt/images/QRadioButton_checked_hover.png`

 * *Files identical despite different names*

### Comparing `bqt-1.1.0/bqt/images/QRadioButton_unchecked.png` & `bqt-1.2.0/bqt/images/QRadioButton_unchecked.png`

 * *Files identical despite different names*

### Comparing `bqt-1.1.0/bqt/images/QRadioButton_unchecked_hover.png` & `bqt-1.2.0/bqt/images/QRadioButton_unchecked_hover.png`

 * *Files identical despite different names*

### Comparing `bqt-1.1.0/bqt/images/QSpinBox_down_arrow.png` & `bqt-1.2.0/bqt/images/QSpinBox_down_arrow.png`

 * *Files identical despite different names*

### Comparing `bqt-1.1.0/bqt/images/QSpinBox_up_arrow.png` & `bqt-1.2.0/bqt/images/QSpinBox_up_arrow.png`

 * *Files identical despite different names*

### Comparing `bqt-1.1.0/bqt/ui/__init__.py` & `bqt-1.2.0/bqt/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `bqt-1.1.0/bqt/ui/quit_dialogue.py` & `bqt-1.2.0/bqt/ui/quit_dialogue.py`

 * *Files identical despite different names*

### Comparing `bqt-1.1.0/bqt/utils.py` & `bqt-1.2.0/bqt/utils.py`

 * *Files identical despite different names*

### Comparing `bqt-1.1.0/bqt.egg-info/PKG-INFO` & `bqt-1.2.0/bqt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bqt
-Version: 1.1.0
+Version: 1.2.0
 Summary: Files to help bootstrap PySide2 with an event loop within Blender.
 Home-page: https://github.com/techartorg/bqt
 Author: tech-artists.org
 License: Mozilla Public License 2.0 (MPL 2.0)
 Keywords: Technical,Art,TechArt,TechArtOrg,Blender,Qt,PySide
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -66,25 +66,30 @@
 Any updates in the repo are then reflected in blender on restart.
 e.g.:
 ```commandline
 mklink /J "C:\Users\USERNAME\AppData\Roaming\Blender Foundation\Blender\2.93\scripts\addons\bqt" "C:\Users\hanne\OneDrive\Documents\repos\_Blender\bqt\bqt"
 ```
 
 ### Environment variables
+
 | variable | description|
 |--|--|
 |BQT_DISABLE_STARTUP| if set to `1`, completely disable bqt|
 |BQT_DISABLE_WRAP| if set to `1`, disable wrapping blender in a QWindow|
 |BQT_DISABLE_CLOSE_DIALOGUE| if set to `1`, use the standard blender close dialogue|
 |BQT_MANAGE_FOREGROUND| defaults to `1`, if `0`, widgets registered with `bqt.add(my_widget)` won't stay in the foreground when using Blender.|
-if you modify env vars, ensure they're strings
+|BQT_AUTO_ADD| defaults to `1`, if `0` top level widgets won't automatically be added to bqt.|
+
+- if you modify env vars, ensure they're strings
+- if you're unsure how to set env vars, google `set environment variable windows`.
+- Restart Blender (or your computer) after changing them.
 
 ### Sample code
 [bqt_demo](bqt_demo) shows you how to use bqt with several qt demos you can run in Blender
 
 ### Community
 Discuss BQT on 
 - the BlenderArtists [thread](https://blenderartists.org/t/bqt-custom-ui-for-add-ons-tool-in-blender-with-pyqt-or-pyside/1458808)
 - [Ynput  thread](https://community.ynput.io/t/use-bqt-for-blender-qt-integration/127)
 
-### ALternative
+### Alternative
 - Custom UI for Blender only: https://github.com/mmmrqs/bl_ui_widgets
```

### Comparing `bqt-1.1.0/bqt.egg-info/SOURCES.txt` & `bqt-1.2.0/bqt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bqt-1.1.0/setup.py` & `bqt-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         # Run the standard PyPi Copy
         install.run(self)
 
 
 setup(
     # Metadata
     name="bqt",
-    version="1.1.0",
+    version="1.2.0",
     description="Files to help bootstrap PySide2 with an event loop within Blender.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=["Technical", "Art", "TechArt", "TechArtOrg", "Blender", "Qt", "PySide"],
     license="Mozilla Public License 2.0 (MPL 2.0)",
     url="https://github.com/techartorg/bqt",
     author="tech-artists.org",
```

