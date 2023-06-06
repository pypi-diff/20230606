# Comparing `tmp/bqt-1.2.0.tar.gz` & `tmp/bqt-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bqt-1.2.0.tar", last modified: Tue Jun  6 14:44:43 2023, max compression
+gzip compressed data, was "bqt-1.2.1.tar", last modified: Tue Jun  6 16:43:51 2023, max compression
```

## Comparing `bqt-1.2.0.tar` & `bqt-1.2.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:44:43.911776 bqt-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-06 14:44:34.000000 bqt-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-06 14:44:34.000000 bqt-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-06 14:44:43.911776 bqt-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-06 14:44:34.000000 bqt-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:44:43.903776 bqt-1.2.0/bqt/
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:44:43.907776 bqt-1.2.0/bqt/blender_applications/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/blender_applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/blender_applications/blender_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/blender_applications/darwin_blender_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/blender_applications/win32_blender_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/blender_stylesheet.qss
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/focus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:44:43.911776 bqt-1.2.0/bqt/images/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/images/QCheckBox_checked.png
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/images/QCheckBox_unchecked.png
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/images/QCheckbox_checked_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/images/QCheckbox_unchecked_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/images/QComboBox_down_arrow.png
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/images/QRadioButton_checked.png
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/images/QRadioButton_checked_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/images/QRadioButton_unchecked.png
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/images/QRadioButton_unchecked_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/images/QSpinBox_down_arrow.png
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/images/QSpinBox_up_arrow.png
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/images/blender_icon_16.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:44:43.911776 bqt-1.2.0/bqt/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/ui/quit_dialogue.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-06 14:44:34.000000 bqt-1.2.0/bqt/widget_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:44:43.903776 bqt-1.2.0/bqt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-06 14:44:43.000000 bqt-1.2.0/bqt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-06 14:44:43.000000 bqt-1.2.0/bqt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:44:43.000000 bqt-1.2.0/bqt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 14:44:43.000000 bqt-1.2.0/bqt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-06 14:44:43.000000 bqt-1.2.0/bqt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 14:44:43.911776 bqt-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-06 14:44:34.000000 bqt-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:43:51.153515 bqt-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-06 16:43:41.000000 bqt-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-06 16:43:41.000000 bqt-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-06 16:43:51.149515 bqt-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-06 16:43:41.000000 bqt-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:43:51.149515 bqt-1.2.1/bqt/
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:43:51.149515 bqt-1.2.1/bqt/blender_applications/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/blender_applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/blender_applications/blender_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/blender_applications/darwin_blender_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/blender_applications/win32_blender_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/blender_stylesheet.qss
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/focus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:43:51.149515 bqt-1.2.1/bqt/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/images/QCheckBox_checked.png
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/images/QCheckBox_unchecked.png
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/images/QCheckbox_checked_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/images/QCheckbox_unchecked_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/images/QComboBox_down_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/images/QRadioButton_checked.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/images/QRadioButton_checked_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/images/QRadioButton_unchecked.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/images/QRadioButton_unchecked_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/images/QSpinBox_down_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/images/QSpinBox_up_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/images/blender_icon_16.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:43:51.149515 bqt-1.2.1/bqt/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/ui/quit_dialogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-06 16:43:41.000000 bqt-1.2.1/bqt/widget_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:43:51.149515 bqt-1.2.1/bqt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-06 16:43:51.000000 bqt-1.2.1/bqt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-06 16:43:51.000000 bqt-1.2.1/bqt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 16:43:51.000000 bqt-1.2.1/bqt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 16:43:51.000000 bqt-1.2.1/bqt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-06 16:43:51.000000 bqt-1.2.1/bqt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 16:43:51.153515 bqt-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-06 16:43:41.000000 bqt-1.2.1/setup.py
```

### Comparing `bqt-1.2.0/LICENSE` & `bqt-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bqt-1.2.0/PKG-INFO` & `bqt-1.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bqt
-Version: 1.2.0
+Version: 1.2.1
 Summary: Files to help bootstrap PySide2 with an event loop within Blender.
 Home-page: https://github.com/techartorg/bqt
 Author: tech-artists.org
 License: Mozilla Public License 2.0 (MPL 2.0)
 Keywords: Technical,Art,TechArt,TechArtOrg,Blender,Qt,PySide
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -72,15 +72,15 @@
 ### Environment variables
 
 | variable | description|
 |--|--|
 |BQT_DISABLE_STARTUP| if set to `1`, completely disable bqt|
 |BQT_DISABLE_WRAP| if set to `1`, disable wrapping blender in a QWindow|
 |BQT_DISABLE_CLOSE_DIALOGUE| if set to `1`, use the standard blender close dialogue|
-|BQT_MANAGE_FOREGROUND| defaults to `1`, if `0`, widgets registered with `bqt.add(my_widget)` won't stay in the foreground when using Blender.|
+|BQT_MANAGE_FOREGROUND| defaults to `1`, if `0`, widgets registered with `bqt.register(my_widget)` won't stay in the foreground when using Blender.|
 |BQT_AUTO_ADD| defaults to `1`, if `0` top level widgets won't automatically be added to bqt.|
 
 - if you modify env vars, ensure they're strings
 - if you're unsure how to set env vars, google `set environment variable windows`.
 - Restart Blender (or your computer) after changing them.
 
 ### Sample code
```

### Comparing `bqt-1.2.0/README.md` & `bqt-1.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 ### Environment variables
 
 | variable | description|
 |--|--|
 |BQT_DISABLE_STARTUP| if set to `1`, completely disable bqt|
 |BQT_DISABLE_WRAP| if set to `1`, disable wrapping blender in a QWindow|
 |BQT_DISABLE_CLOSE_DIALOGUE| if set to `1`, use the standard blender close dialogue|
-|BQT_MANAGE_FOREGROUND| defaults to `1`, if `0`, widgets registered with `bqt.add(my_widget)` won't stay in the foreground when using Blender.|
+|BQT_MANAGE_FOREGROUND| defaults to `1`, if `0`, widgets registered with `bqt.register(my_widget)` won't stay in the foreground when using Blender.|
 |BQT_AUTO_ADD| defaults to `1`, if `0` top level widgets won't automatically be added to bqt.|
 
 - if you modify env vars, ensure they're strings
 - if you're unsure how to set env vars, google `set environment variable windows`.
 - Restart Blender (or your computer) after changing them.
 
 ### Sample code
```

### Comparing `bqt-1.2.0/bqt/__init__.py` & `bqt-1.2.1/bqt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from pathlib import Path
 
 
 bl_info = {
         "name": "PySide2 Qt wrapper (bqt)",
         "description": "Enable PySide2 QtWidgets in Blender",
         "author": "tech-artists.org",
-        "version": (1, 0),
+        "version": (1, 2, 1),
         "blender": (2, 80, 0),
         # "location": "",
         # "warning": "", # used for warning icon and text in add-ons panel
         # "wiki_url": "http://my.wiki.url",
         # "tracker_url": "http://my.bugtracker.url",
         "support": "COMMUNITY",
         "category": "UI"
```

### Comparing `bqt-1.2.0/bqt/blender_applications/__init__.py` & `bqt-1.2.1/bqt/blender_applications/__init__.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.0/bqt/blender_applications/blender_application.py` & `bqt-1.2.1/bqt/blender_applications/blender_application.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.0/bqt/blender_applications/darwin_blender_application.py` & `bqt-1.2.1/bqt/blender_applications/darwin_blender_application.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.0/bqt/blender_applications/win32_blender_application.py` & `bqt-1.2.1/bqt/blender_applications/win32_blender_application.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.0/bqt/blender_stylesheet.qss` & `bqt-1.2.1/bqt/blender_stylesheet.qss`

 * *Files identical despite different names*

### Comparing `bqt-1.2.0/bqt/focus.py` & `bqt-1.2.1/bqt/focus.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.0/bqt/images/QCheckBox_checked.png` & `bqt-1.2.1/bqt/images/QCheckBox_checked.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.0/bqt/images/QCheckBox_unchecked.png` & `bqt-1.2.1/bqt/images/QCheckBox_unchecked.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.0/bqt/images/QCheckbox_checked_hover.png` & `bqt-1.2.1/bqt/images/QCheckbox_checked_hover.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.0/bqt/images/QCheckbox_unchecked_hover.png` & `bqt-1.2.1/bqt/images/QCheckbox_unchecked_hover.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.0/bqt/images/QComboBox_down_arrow.png` & `bqt-1.2.1/bqt/images/QComboBox_down_arrow.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.0/bqt/images/QRadioButton_checked.png` & `bqt-1.2.1/bqt/images/QRadioButton_checked.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.0/bqt/images/QRadioButton_checked_hover.png` & `bqt-1.2.1/bqt/images/QRadioButton_checked_hover.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.0/bqt/images/QRadioButton_unchecked.png` & `bqt-1.2.1/bqt/images/QRadioButton_unchecked.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.0/bqt/images/QRadioButton_unchecked_hover.png` & `bqt-1.2.1/bqt/images/QRadioButton_unchecked_hover.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.0/bqt/images/QSpinBox_down_arrow.png` & `bqt-1.2.1/bqt/images/QSpinBox_down_arrow.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.0/bqt/images/QSpinBox_up_arrow.png` & `bqt-1.2.1/bqt/images/QSpinBox_up_arrow.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.0/bqt/ui/__init__.py` & `bqt-1.2.1/bqt/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.0/bqt/ui/quit_dialogue.py` & `bqt-1.2.1/bqt/ui/quit_dialogue.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.0/bqt/utils.py` & `bqt-1.2.1/bqt/utils.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.0/bqt/widget_manager.py` & `bqt-1.2.1/bqt/widget_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 """
 from PySide2.QtWidgets import QApplication
 from PySide2.QtCore import Qt
 import logging
 
 
 __widgets = []
+__excluded_widgets = []
 
 
 class WidgetData():
     def __init__(self, widget, visible):
         self.widget = widget
         self.visible = visible
 
@@ -39,15 +40,17 @@
 
     if widget in exclude:
         logging.warning("bqt: widget is in exclude list, skipping widget registration")
         return
 
     # parent to blender window
     if parent:
+        vis = widget.isVisible()
         widget.setParent(parent_widget, Qt.Window)  # default set flag to window
+        widget.setVisible(vis)  # parenting hides the widget, restore visibility
 
     # save widget so we can manage the focus and visibility
     if manage:
         data = WidgetData(widget, widget.isVisible())  # todo can we init vis state to false?
         __widgets.append(data)
 
 
@@ -92,16 +95,19 @@
             widget.hide()  # todo since we hide do we need to remove flag?
 
     # todo right now widgets stay in front of other blender windows,
     #  e.g. the preferences window, ideally we handle this
 
 
 def _orphan_toplevel_widgets():
-    # todo do we need to filter by window type?
-    return [widget for widget in QApplication.instance().topLevelWidgets() if not widget.parent()]
+    return [widget for widget in QApplication.instance().topLevelWidgets() if
+            not widget.parent()
+            and widget not in __widgets
+            and widget not in __excluded_widgets]
 
 
 def parent_orphan_widgets(exclude=None):
     """Find and parent orphan widgets to the blender widget"""
     exclude = exclude or []
+    __excluded_widgets.extend(exclude)
     for widget in _orphan_toplevel_widgets():
         register(widget, exclude=exclude)
```

### Comparing `bqt-1.2.0/bqt.egg-info/PKG-INFO` & `bqt-1.2.1/bqt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bqt
-Version: 1.2.0
+Version: 1.2.1
 Summary: Files to help bootstrap PySide2 with an event loop within Blender.
 Home-page: https://github.com/techartorg/bqt
 Author: tech-artists.org
 License: Mozilla Public License 2.0 (MPL 2.0)
 Keywords: Technical,Art,TechArt,TechArtOrg,Blender,Qt,PySide
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -72,15 +72,15 @@
 ### Environment variables
 
 | variable | description|
 |--|--|
 |BQT_DISABLE_STARTUP| if set to `1`, completely disable bqt|
 |BQT_DISABLE_WRAP| if set to `1`, disable wrapping blender in a QWindow|
 |BQT_DISABLE_CLOSE_DIALOGUE| if set to `1`, use the standard blender close dialogue|
-|BQT_MANAGE_FOREGROUND| defaults to `1`, if `0`, widgets registered with `bqt.add(my_widget)` won't stay in the foreground when using Blender.|
+|BQT_MANAGE_FOREGROUND| defaults to `1`, if `0`, widgets registered with `bqt.register(my_widget)` won't stay in the foreground when using Blender.|
 |BQT_AUTO_ADD| defaults to `1`, if `0` top level widgets won't automatically be added to bqt.|
 
 - if you modify env vars, ensure they're strings
 - if you're unsure how to set env vars, google `set environment variable windows`.
 - Restart Blender (or your computer) after changing them.
 
 ### Sample code
```

### Comparing `bqt-1.2.0/bqt.egg-info/SOURCES.txt` & `bqt-1.2.1/bqt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bqt-1.2.0/setup.py` & `bqt-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         # Run the standard PyPi Copy
         install.run(self)
 
 
 setup(
     # Metadata
     name="bqt",
-    version="1.2.0",
+    version="1.2.1",
     description="Files to help bootstrap PySide2 with an event loop within Blender.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=["Technical", "Art", "TechArt", "TechArtOrg", "Blender", "Qt", "PySide"],
     license="Mozilla Public License 2.0 (MPL 2.0)",
     url="https://github.com/techartorg/bqt",
     author="tech-artists.org",
```

