# Comparing `tmp/bqt-1.2.3.tar.gz` & `tmp/bqt-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bqt-1.2.3.tar", last modified: Tue Jun  6 17:44:34 2023, max compression
+gzip compressed data, was "bqt-1.3.0.tar", last modified: Tue Jun  6 21:26:26 2023, max compression
```

## Comparing `bqt-1.2.3.tar` & `bqt-1.3.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:44:34.006703 bqt-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-06 17:44:23.000000 bqt-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-06 17:44:23.000000 bqt-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-06 17:44:34.006703 bqt-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-06 17:44:23.000000 bqt-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:44:34.002704 bqt-1.2.3/bqt/
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:44:34.006703 bqt-1.2.3/bqt/blender_applications/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/blender_applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/blender_applications/blender_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/blender_applications/darwin_blender_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/blender_applications/win32_blender_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/blender_stylesheet.qss
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/focus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:44:34.006703 bqt-1.2.3/bqt/images/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/images/QCheckBox_checked.png
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/images/QCheckBox_unchecked.png
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/images/QCheckbox_checked_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/images/QCheckbox_unchecked_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/images/QComboBox_down_arrow.png
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/images/QRadioButton_checked.png
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/images/QRadioButton_checked_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/images/QRadioButton_unchecked.png
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/images/QRadioButton_unchecked_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/images/QSpinBox_down_arrow.png
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/images/QSpinBox_up_arrow.png
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/images/blender_icon_16.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:44:34.006703 bqt-1.2.3/bqt/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/ui/quit_dialogue.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/widget_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:44:34.006703 bqt-1.2.3/bqt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-06 17:44:33.000000 bqt-1.2.3/bqt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-06 17:44:34.000000 bqt-1.2.3/bqt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 17:44:33.000000 bqt-1.2.3/bqt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 17:44:33.000000 bqt-1.2.3/bqt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-06 17:44:33.000000 bqt-1.2.3/bqt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 17:44:34.006703 bqt-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-06 17:44:23.000000 bqt-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:26:26.268336 bqt-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-06 21:26:16.000000 bqt-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-06 21:26:16.000000 bqt-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-06-06 21:26:26.268336 bqt-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-06-06 21:26:16.000000 bqt-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:26:26.264336 bqt-1.3.0/bqt/
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-06 21:26:16.000000 bqt-1.3.0/bqt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:26:26.264336 bqt-1.3.0/bqt/blender_applications/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-06 21:26:16.000000 bqt-1.3.0/bqt/blender_applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-06-06 21:26:16.000000 bqt-1.3.0/bqt/blender_applications/blender_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-06 21:26:16.000000 bqt-1.3.0/bqt/blender_applications/darwin_blender_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-06-06 21:26:16.000000 bqt-1.3.0/bqt/blender_applications/win32_blender_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-06-06 21:26:16.000000 bqt-1.3.0/bqt/blender_stylesheet.qss
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-06 21:26:16.000000 bqt-1.3.0/bqt/focus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:26:26.264336 bqt-1.3.0/bqt/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-06 21:26:16.000000 bqt-1.3.0/bqt/images/QCheckBox_checked.png
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-06 21:26:16.000000 bqt-1.3.0/bqt/images/QCheckBox_unchecked.png
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-06 21:26:16.000000 bqt-1.3.0/bqt/images/QCheckbox_checked_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-06 21:26:16.000000 bqt-1.3.0/bqt/images/QCheckbox_unchecked_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-06 21:26:16.000000 bqt-1.3.0/bqt/images/QComboBox_down_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-06 21:26:16.000000 bqt-1.3.0/bqt/images/QRadioButton_checked.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-06-06 21:26:16.000000 bqt-1.3.0/bqt/images/QRadioButton_checked_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-06 21:26:16.000000 bqt-1.3.0/bqt/images/QRadioButton_unchecked.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-06 21:26:16.000000 bqt-1.3.0/bqt/images/QRadioButton_unchecked_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-06 21:26:16.000000 bqt-1.3.0/bqt/images/QSpinBox_down_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-06 21:26:16.000000 bqt-1.3.0/bqt/images/QSpinBox_up_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-06 21:26:16.000000 bqt-1.3.0/bqt/images/blender_icon_16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-06-06 21:26:16.000000 bqt-1.3.0/bqt/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:26:26.264336 bqt-1.3.0/bqt/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-06 21:26:16.000000 bqt-1.3.0/bqt/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-06 21:26:16.000000 bqt-1.3.0/bqt/ui/quit_dialogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-06 21:26:16.000000 bqt-1.3.0/bqt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:26:26.264336 bqt-1.3.0/bqt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-06-06 21:26:26.000000 bqt-1.3.0/bqt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-06 21:26:26.000000 bqt-1.3.0/bqt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 21:26:26.000000 bqt-1.3.0/bqt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 21:26:26.000000 bqt-1.3.0/bqt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-06 21:26:26.000000 bqt-1.3.0/bqt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 21:26:26.268336 bqt-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-06 21:26:16.000000 bqt-1.3.0/setup.py
```

### Comparing `bqt-1.2.3/LICENSE` & `bqt-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bqt-1.2.3/PKG-INFO` & `bqt-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bqt
-Version: 1.2.3
+Version: 1.3.0
 Summary: Files to help bootstrap PySide2 with an event loop within Blender.
 Home-page: https://github.com/techartorg/bqt
 Author: tech-artists.org
 License: Mozilla Public License 2.0 (MPL 2.0)
 Keywords: Technical,Art,TechArt,TechArtOrg,Blender,Qt,PySide
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -74,14 +74,15 @@
 | variable | description|
 |--|--|
 |BQT_DISABLE_STARTUP| if set to `1`, completely disable bqt|
 |BQT_DISABLE_WRAP| if set to `1`, disable wrapping blender in a QWindow|
 |BQT_DISABLE_CLOSE_DIALOGUE| if set to `1`, use the standard blender close dialogue|
 |BQT_MANAGE_FOREGROUND| defaults to `1`, if `0`, widgets registered with `bqt.add(my_widget)` won't stay in the foreground when using Blender.|
 |BQT_AUTO_ADD| defaults to `1`, if `0` top level widgets won't automatically be added to bqt.|
+|BQT_UNIQUE_OBJECTNAME| defaults to `1`, 1 or 0, automatically delete widgets with same objectName, preventing you from opening multiple versions of the same widget window. Great if you want to ensure that clicking "my window" activates "mywindow" if already open, instead of making a new one|
 
 - if you modify env vars, ensure they're strings
 - if you're unsure how to set env vars, google `set environment variable windows`.
 - Restart Blender (or your computer) after changing them.
 
 ### Sample code
 [bqt_demo](bqt_demo) shows you how to use bqt with several qt demos you can run in Blender
```

### Comparing `bqt-1.2.3/README.md` & `bqt-1.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 | variable | description|
 |--|--|
 |BQT_DISABLE_STARTUP| if set to `1`, completely disable bqt|
 |BQT_DISABLE_WRAP| if set to `1`, disable wrapping blender in a QWindow|
 |BQT_DISABLE_CLOSE_DIALOGUE| if set to `1`, use the standard blender close dialogue|
 |BQT_MANAGE_FOREGROUND| defaults to `1`, if `0`, widgets registered with `bqt.add(my_widget)` won't stay in the foreground when using Blender.|
 |BQT_AUTO_ADD| defaults to `1`, if `0` top level widgets won't automatically be added to bqt.|
+|BQT_UNIQUE_OBJECTNAME| defaults to `1`, 1 or 0, automatically delete widgets with same objectName, preventing you from opening multiple versions of the same widget window. Great if you want to ensure that clicking "my window" activates "mywindow" if already open, instead of making a new one|
 
 - if you modify env vars, ensure they're strings
 - if you're unsure how to set env vars, google `set environment variable windows`.
 - Restart Blender (or your computer) after changing them.
 
 ### Sample code
 [bqt_demo](bqt_demo) shows you how to use bqt with several qt demos you can run in Blender
```

### Comparing `bqt-1.2.3/bqt/__init__.py` & `bqt-1.3.0/bqt/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
 This Source Code Form is subject to the terms of the Mozilla Public
 License, v. 2.0. If a copy of the MPL was not distributed with this
 file, You can obtain one at https://mozilla.org/MPL/2.0/.
 """
 import bqt
 import bqt.focus
-import bqt.widget_manager
+import bqt.manager
 import os
 import sys
 import bpy
 import PySide2.QtCore as QtCore
 from PySide2.QtWidgets import QApplication
 from PySide2.QtCore import QDir
 import logging
 from pathlib import Path
 
 
 bl_info = {
         "name": "PySide2 Qt wrapper (bqt)",
         "description": "Enable PySide2 QtWidgets in Blender",
         "author": "tech-artists.org",
-        "version": (1, 2, 3),
+        "version": (1, 3, 0),
         "blender": (2, 80, 0),
         # "location": "",
         # "warning": "", # used for warning icon and text in add-ons panel
         # "wiki_url": "http://my.wiki.url",
         # "tracker_url": "http://my.bugtracker.url",
         "support": "COMMUNITY",
         "category": "UI"
         }
 
-add = bqt.widget_manager.register
+add = bqt.manager.register
 
 # CORE FUNCTIONS #
 
 def _instantiate_QApplication() -> "bqt.blender_applications.BlenderApplication":
     # enable dpi scale, run before creating QApplication
     QApplication.setHighDpiScaleFactorRoundingPolicy(QtCore.Qt.HighDpiScaleFactorRoundingPolicy.PassThrough)
     QApplication.setAttribute(QtCore.Qt.AA_EnableHighDpiScaling)
```

### Comparing `bqt-1.2.3/bqt/blender_applications/__init__.py` & `bqt-1.3.0/bqt/blender_applications/__init__.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.3/bqt/blender_applications/blender_application.py` & `bqt-1.3.0/bqt/blender_applications/blender_application.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pathlib import Path
 import os
 from PySide2.QtWidgets import QApplication, QWidget, QPushButton, QDockWidget, QMainWindow
 from PySide2.QtGui import QCloseEvent, QIcon, QImage, QPixmap, QWindow
 from PySide2.QtCore import QEvent, QObject, QRect, QSettings, QTimer, Qt
 from bqt.ui.quit_dialogue import BlenderClosingDialog
 import bpy
-import bqt.widget_manager
+import bqt.manager
 
 
 STYLESHEET_PATH = Path(__file__).parents[1] / "blender_stylesheet.qss"
 ORGANISATION = "Tech-Artists.org"
 APP = "Blender Qt"
 WINDOW_TITLE = "Blender Qt"
 WINDOW_GROUP_NAME = "MainWindow"
@@ -68,18 +68,18 @@
         tick = int(1000 / FOCUS_FRAMERATE)  # tick 1000 / frames per second
         self.timer.start(tick)
 
     def on_update(self):
         """qt event loop"""
         # we only need foreground managing if blender is not wrapped
         if os.getenv("BQT_DISABLE_WRAP") == "1" and os.getenv("BQT_MANAGE_FOREGROUND", "1") == "1" and self.blender_focus_toggled():
-            bqt.widget_manager._blender_window_change(self._active_window_hwnd)
+            bqt.manager._blender_window_change(self._active_window_hwnd)
 
         if os.getenv("BQT_AUTO_ADD", "1") == "1":
-            bqt.widget_manager.parent_orphan_widgets(exclude=[self.blender_widget, self._blender_window, self.window_container])  # auto parent any orphaned widgets
+            bqt.manager.parent_orphan_widgets(exclude=[self.blender_widget, self._blender_window, self.window_container])  # auto parent any orphaned widgets
 
     def blender_focus_toggled(self):
         """returns true the first frame the blender window is focussed or unfoccused"""
         current_active_hwnd = self._get_active_window_handle()
         handle_changed = self._active_window_hwnd != current_active_hwnd
         if not handle_changed:
             self._active_window_hwnd = current_active_hwnd
```

### Comparing `bqt-1.2.3/bqt/blender_applications/darwin_blender_application.py` & `bqt-1.3.0/bqt/blender_applications/darwin_blender_application.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.3/bqt/blender_applications/win32_blender_application.py` & `bqt-1.3.0/bqt/blender_applications/win32_blender_application.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.3/bqt/blender_stylesheet.qss` & `bqt-1.3.0/bqt/blender_stylesheet.qss`

 * *Files identical despite different names*

### Comparing `bqt-1.2.3/bqt/focus.py` & `bqt-1.3.0/bqt/focus.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.3/bqt/images/QCheckBox_checked.png` & `bqt-1.3.0/bqt/images/QCheckBox_checked.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.3/bqt/images/QCheckBox_unchecked.png` & `bqt-1.3.0/bqt/images/QCheckBox_unchecked.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.3/bqt/images/QCheckbox_checked_hover.png` & `bqt-1.3.0/bqt/images/QCheckbox_checked_hover.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.3/bqt/images/QCheckbox_unchecked_hover.png` & `bqt-1.3.0/bqt/images/QCheckbox_unchecked_hover.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.3/bqt/images/QComboBox_down_arrow.png` & `bqt-1.3.0/bqt/images/QComboBox_down_arrow.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.3/bqt/images/QRadioButton_checked.png` & `bqt-1.3.0/bqt/images/QRadioButton_checked.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.3/bqt/images/QRadioButton_checked_hover.png` & `bqt-1.3.0/bqt/images/QRadioButton_checked_hover.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.3/bqt/images/QRadioButton_unchecked.png` & `bqt-1.3.0/bqt/images/QRadioButton_unchecked.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.3/bqt/images/QRadioButton_unchecked_hover.png` & `bqt-1.3.0/bqt/images/QRadioButton_unchecked_hover.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.3/bqt/images/QSpinBox_down_arrow.png` & `bqt-1.3.0/bqt/images/QSpinBox_down_arrow.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.3/bqt/images/QSpinBox_up_arrow.png` & `bqt-1.3.0/bqt/images/QSpinBox_up_arrow.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.3/bqt/ui/__init__.py` & `bqt-1.3.0/bqt/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.3/bqt/ui/quit_dialogue.py` & `bqt-1.3.0/bqt/ui/quit_dialogue.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.3/bqt/utils.py` & `bqt-1.3.0/bqt/utils.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.3/bqt/widget_manager.py` & `bqt-1.3.0/bqt/manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,33 +16,52 @@
 
 class WidgetData():
     def __init__(self, widget, visible):
         self.widget = widget
         self.visible = visible
 
 
-def register(widget, exclude=None, parent=True, manage=True):
+def register(widget, exclude=None, parent=True, manage=True, unique=True):
     """
     parent widget to blender window
     Args:
         widget: child widget to parent
         parent: if True, parent the widget to the blender window
         exclude: widgets to exclude from being parented to the blender window
         manage: if True, manage the visibility of the widget
+        unique: if True, prevent registering a new widget with the same objectName
     """
     exclude = exclude or []
 
     if not widget:
         logging.warning("bqt: widget is None, skipping widget registration")
         return
 
     parent_widget = QApplication.instance().blender_widget
     if widget == parent_widget:
         return
 
+    # prevent registering a new widget with the same objectName
+    if unique and os.getenv("BQT_UNIQUE_OBJECTNAME", "1") == "1":
+        obj_name = widget.objectName()
+        old_widget = None  # already registered widget with the same objectName
+        if obj_name:
+            for data in iter_widget_data():
+                if data.widget.objectName() == obj_name:
+                    old_widget = data.widget
+                    break
+        if old_widget:
+            logging.warning("bqt: widget is already registered, skipping widget registration")
+            # show old widget, delete new widget
+            old_widget.show()
+            old_widget.activateWindow()
+            widget.deleteLater()  # delete duplicate widget, todo dangerous?
+            __excluded_widgets.append(widget)
+            return
+
     if widget in exclude:
         logging.warning("bqt: widget is in exclude list, skipping widget registration")
         return
 
     # parent to blender window
     if parent:
         vis = widget.isVisible()
```

### Comparing `bqt-1.2.3/bqt.egg-info/PKG-INFO` & `bqt-1.3.0/bqt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bqt
-Version: 1.2.3
+Version: 1.3.0
 Summary: Files to help bootstrap PySide2 with an event loop within Blender.
 Home-page: https://github.com/techartorg/bqt
 Author: tech-artists.org
 License: Mozilla Public License 2.0 (MPL 2.0)
 Keywords: Technical,Art,TechArt,TechArtOrg,Blender,Qt,PySide
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -74,14 +74,15 @@
 | variable | description|
 |--|--|
 |BQT_DISABLE_STARTUP| if set to `1`, completely disable bqt|
 |BQT_DISABLE_WRAP| if set to `1`, disable wrapping blender in a QWindow|
 |BQT_DISABLE_CLOSE_DIALOGUE| if set to `1`, use the standard blender close dialogue|
 |BQT_MANAGE_FOREGROUND| defaults to `1`, if `0`, widgets registered with `bqt.add(my_widget)` won't stay in the foreground when using Blender.|
 |BQT_AUTO_ADD| defaults to `1`, if `0` top level widgets won't automatically be added to bqt.|
+|BQT_UNIQUE_OBJECTNAME| defaults to `1`, 1 or 0, automatically delete widgets with same objectName, preventing you from opening multiple versions of the same widget window. Great if you want to ensure that clicking "my window" activates "mywindow" if already open, instead of making a new one|
 
 - if you modify env vars, ensure they're strings
 - if you're unsure how to set env vars, google `set environment variable windows`.
 - Restart Blender (or your computer) after changing them.
 
 ### Sample code
 [bqt_demo](bqt_demo) shows you how to use bqt with several qt demos you can run in Blender
```

### Comparing `bqt-1.2.3/bqt.egg-info/SOURCES.txt` & `bqt-1.3.0/bqt.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 bqt/__init__.py
 bqt/blender_stylesheet.qss
 bqt/focus.py
+bqt/manager.py
 bqt/utils.py
-bqt/widget_manager.py
 bqt.egg-info/PKG-INFO
 bqt.egg-info/SOURCES.txt
 bqt.egg-info/dependency_links.txt
 bqt.egg-info/requires.txt
 bqt.egg-info/top_level.txt
 bqt/blender_applications/__init__.py
 bqt/blender_applications/blender_application.py
```

### Comparing `bqt-1.2.3/setup.py` & `bqt-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         # Run the standard PyPi Copy
         install.run(self)
 
 
 setup(
     # Metadata
     name="bqt",
-    version="1.2.3",
+    version="1.3.0",
     description="Files to help bootstrap PySide2 with an event loop within Blender.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=["Technical", "Art", "TechArt", "TechArtOrg", "Blender", "Qt", "PySide"],
     license="Mozilla Public License 2.0 (MPL 2.0)",
     url="https://github.com/techartorg/bqt",
     author="tech-artists.org",
```

