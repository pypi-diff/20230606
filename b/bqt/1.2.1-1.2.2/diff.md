# Comparing `tmp/bqt-1.2.1.tar.gz` & `tmp/bqt-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bqt-1.2.1.tar", last modified: Tue Jun  6 16:43:51 2023, max compression
+gzip compressed data, was "bqt-1.2.2.tar", last modified: Tue Jun  6 17:08:23 2023, max compression
```

## Comparing `bqt-1.2.1.tar` & `bqt-1.2.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:43:51.153515 bqt-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-06 16:43:41.000000 bqt-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-06 16:43:41.000000 bqt-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-06 16:43:51.149515 bqt-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-06 16:43:41.000000 bqt-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:43:51.149515 bqt-1.2.1/bqt/
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:43:51.149515 bqt-1.2.1/bqt/blender_applications/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/blender_applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/blender_applications/blender_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/blender_applications/darwin_blender_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/blender_applications/win32_blender_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/blender_stylesheet.qss
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/focus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:43:51.149515 bqt-1.2.1/bqt/images/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/images/QCheckBox_checked.png
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/images/QCheckBox_unchecked.png
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/images/QCheckbox_checked_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/images/QCheckbox_unchecked_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/images/QComboBox_down_arrow.png
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/images/QRadioButton_checked.png
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/images/QRadioButton_checked_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/images/QRadioButton_unchecked.png
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/images/QRadioButton_unchecked_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/images/QSpinBox_down_arrow.png
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/images/QSpinBox_up_arrow.png
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/images/blender_icon_16.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:43:51.149515 bqt-1.2.1/bqt/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/ui/quit_dialogue.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/widget_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:43:51.149515 bqt-1.2.1/bqt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-06 16:43:51.000000 bqt-1.2.1/bqt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-06 16:43:51.000000 bqt-1.2.1/bqt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 16:43:51.000000 bqt-1.2.1/bqt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 16:43:51.000000 bqt-1.2.1/bqt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-06 16:43:51.000000 bqt-1.2.1/bqt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 16:43:51.153515 bqt-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-06 16:43:41.000000 bqt-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:08:23.424806 bqt-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-06 17:08:12.000000 bqt-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-06 17:08:12.000000 bqt-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-06 17:08:23.424806 bqt-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-06 17:08:12.000000 bqt-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:08:23.420806 bqt-1.2.2/bqt/
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:08:23.420806 bqt-1.2.2/bqt/blender_applications/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/blender_applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/blender_applications/blender_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/blender_applications/darwin_blender_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/blender_applications/win32_blender_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/blender_stylesheet.qss
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/focus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:08:23.424806 bqt-1.2.2/bqt/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/images/QCheckBox_checked.png
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/images/QCheckBox_unchecked.png
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/images/QCheckbox_checked_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/images/QCheckbox_unchecked_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/images/QComboBox_down_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/images/QRadioButton_checked.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/images/QRadioButton_checked_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/images/QRadioButton_unchecked.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/images/QRadioButton_unchecked_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/images/QSpinBox_down_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/images/QSpinBox_up_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/images/blender_icon_16.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:08:23.424806 bqt-1.2.2/bqt/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/ui/quit_dialogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/widget_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:08:23.420806 bqt-1.2.2/bqt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-06 17:08:23.000000 bqt-1.2.2/bqt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-06 17:08:23.000000 bqt-1.2.2/bqt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 17:08:23.000000 bqt-1.2.2/bqt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 17:08:23.000000 bqt-1.2.2/bqt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-06 17:08:23.000000 bqt-1.2.2/bqt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 17:08:23.424806 bqt-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-06 17:08:12.000000 bqt-1.2.2/setup.py
```

### Comparing `bqt-1.2.1/LICENSE` & `bqt-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bqt-1.2.1/PKG-INFO` & `bqt-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bqt
-Version: 1.2.1
+Version: 1.2.2
 Summary: Files to help bootstrap PySide2 with an event loop within Blender.
 Home-page: https://github.com/techartorg/bqt
 Author: tech-artists.org
 License: Mozilla Public License 2.0 (MPL 2.0)
 Keywords: Technical,Art,TechArt,TechArtOrg,Blender,Qt,PySide
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `bqt-1.2.1/README.md` & `bqt-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `bqt-1.2.1/bqt/__init__.py` & `bqt-1.2.2/bqt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from pathlib import Path
 
 
 bl_info = {
         "name": "PySide2 Qt wrapper (bqt)",
         "description": "Enable PySide2 QtWidgets in Blender",
         "author": "tech-artists.org",
-        "version": (1, 2, 1),
+        "version": (1, 2, 2),
         "blender": (2, 80, 0),
         # "location": "",
         # "warning": "", # used for warning icon and text in add-ons panel
         # "wiki_url": "http://my.wiki.url",
         # "tracker_url": "http://my.bugtracker.url",
         "support": "COMMUNITY",
         "category": "UI"
```

### Comparing `bqt-1.2.1/bqt/blender_applications/__init__.py` & `bqt-1.2.2/bqt/blender_applications/__init__.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.1/bqt/blender_applications/blender_application.py` & `bqt-1.2.2/bqt/blender_applications/blender_application.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.1/bqt/blender_applications/darwin_blender_application.py` & `bqt-1.2.2/bqt/blender_applications/darwin_blender_application.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.1/bqt/blender_applications/win32_blender_application.py` & `bqt-1.2.2/bqt/blender_applications/win32_blender_application.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.1/bqt/blender_stylesheet.qss` & `bqt-1.2.2/bqt/blender_stylesheet.qss`

 * *Files identical despite different names*

### Comparing `bqt-1.2.1/bqt/focus.py` & `bqt-1.2.2/bqt/focus.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.1/bqt/images/QCheckBox_checked.png` & `bqt-1.2.2/bqt/images/QCheckBox_checked.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.1/bqt/images/QCheckBox_unchecked.png` & `bqt-1.2.2/bqt/images/QCheckBox_unchecked.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.1/bqt/images/QCheckbox_checked_hover.png` & `bqt-1.2.2/bqt/images/QCheckbox_checked_hover.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.1/bqt/images/QCheckbox_unchecked_hover.png` & `bqt-1.2.2/bqt/images/QCheckbox_unchecked_hover.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.1/bqt/images/QComboBox_down_arrow.png` & `bqt-1.2.2/bqt/images/QComboBox_down_arrow.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.1/bqt/images/QRadioButton_checked.png` & `bqt-1.2.2/bqt/images/QRadioButton_checked.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.1/bqt/images/QRadioButton_checked_hover.png` & `bqt-1.2.2/bqt/images/QRadioButton_checked_hover.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.1/bqt/images/QRadioButton_unchecked.png` & `bqt-1.2.2/bqt/images/QRadioButton_unchecked.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.1/bqt/images/QRadioButton_unchecked_hover.png` & `bqt-1.2.2/bqt/images/QRadioButton_unchecked_hover.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.1/bqt/images/QSpinBox_down_arrow.png` & `bqt-1.2.2/bqt/images/QSpinBox_down_arrow.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.1/bqt/images/QSpinBox_up_arrow.png` & `bqt-1.2.2/bqt/images/QSpinBox_up_arrow.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.1/bqt/ui/__init__.py` & `bqt-1.2.2/bqt/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.1/bqt/ui/quit_dialogue.py` & `bqt-1.2.2/bqt/ui/quit_dialogue.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.1/bqt/utils.py` & `bqt-1.2.2/bqt/utils.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.1/bqt/widget_manager.py` & `bqt-1.2.2/bqt/widget_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 - parent widget to blender window (blender_widget)
 - keep widget in front of Blender window only, even when bqt is not wrapped in qt
 """
 from PySide2.QtWidgets import QApplication
 from PySide2.QtCore import Qt
 import logging
+import os
 
 
 __widgets = []
 __excluded_widgets = []
 
 
 class WidgetData():
@@ -49,14 +50,20 @@
         widget.setVisible(vis)  # parenting hides the widget, restore visibility
 
     # save widget so we can manage the focus and visibility
     if manage:
         data = WidgetData(widget, widget.isVisible())  # todo can we init vis state to false?
         __widgets.append(data)
 
+        # ensure widget stays in foreground if blender is not wrapped in qt
+        if os.getenv("BQT_DISABLE_WRAP", "0") == "1" and os.getenv("BQT_MANAGE_FOREGROUND", "1") == "1":
+            vis = widget.isVisible()
+            widget.setWindowFlags(widget.windowFlags() | Qt.WindowStaysOnTopHint)
+            widget.setVisible(vis)
+
 
 def iter_widget_data():
     """iterate over all registered widgets, remove widgets that have been removed"""
     cleanup = []
     for widget_data in __widgets:
         if not widget_data.widget:
             cleanup.append(widget_data)
@@ -76,15 +83,15 @@
 
     for widget_data in iter_widget_data():
         widget = widget_data.widget
 
         if focussed_on_a_blender_window:
 
             # add top flag, ensure the widget stays in front of the blender window
-            widget.setWindowFlags(widget.windowFlags() | Qt.WindowStaysOnTopHint)
+            # widget.setWindowFlags(widget.windowFlags() | Qt.WindowStaysOnTopHint)  # todo move this to register?
 
             # restore visibility state of the widget
             if widget_data.visible:
                 widget.show()
 
         else:  # non-blender window
             # save visibility state of the widget
```

### Comparing `bqt-1.2.1/bqt.egg-info/PKG-INFO` & `bqt-1.2.2/bqt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bqt
-Version: 1.2.1
+Version: 1.2.2
 Summary: Files to help bootstrap PySide2 with an event loop within Blender.
 Home-page: https://github.com/techartorg/bqt
 Author: tech-artists.org
 License: Mozilla Public License 2.0 (MPL 2.0)
 Keywords: Technical,Art,TechArt,TechArtOrg,Blender,Qt,PySide
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `bqt-1.2.1/bqt.egg-info/SOURCES.txt` & `bqt-1.2.2/bqt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bqt-1.2.1/setup.py` & `bqt-1.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         # Run the standard PyPi Copy
         install.run(self)
 
 
 setup(
     # Metadata
     name="bqt",
-    version="1.2.1",
+    version="1.2.2",
     description="Files to help bootstrap PySide2 with an event loop within Blender.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=["Technical", "Art", "TechArt", "TechArtOrg", "Blender", "Qt", "PySide"],
     license="Mozilla Public License 2.0 (MPL 2.0)",
     url="https://github.com/techartorg/bqt",
     author="tech-artists.org",
```

