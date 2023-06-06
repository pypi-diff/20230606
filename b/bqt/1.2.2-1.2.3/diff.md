# Comparing `tmp/bqt-1.2.2.tar.gz` & `tmp/bqt-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bqt-1.2.2.tar", last modified: Tue Jun  6 17:08:23 2023, max compression
+gzip compressed data, was "bqt-1.2.3.tar", last modified: Tue Jun  6 17:44:34 2023, max compression
```

## Comparing `bqt-1.2.2.tar` & `bqt-1.2.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:08:23.424806 bqt-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-06 17:08:12.000000 bqt-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-06 17:08:12.000000 bqt-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-06 17:08:23.424806 bqt-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-06 17:08:12.000000 bqt-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:08:23.420806 bqt-1.2.2/bqt/
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:08:23.420806 bqt-1.2.2/bqt/blender_applications/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/blender_applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/blender_applications/blender_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/blender_applications/darwin_blender_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/blender_applications/win32_blender_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/blender_stylesheet.qss
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/focus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:08:23.424806 bqt-1.2.2/bqt/images/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/images/QCheckBox_checked.png
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/images/QCheckBox_unchecked.png
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/images/QCheckbox_checked_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/images/QCheckbox_unchecked_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/images/QComboBox_down_arrow.png
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/images/QRadioButton_checked.png
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/images/QRadioButton_checked_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/images/QRadioButton_unchecked.png
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/images/QRadioButton_unchecked_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/images/QSpinBox_down_arrow.png
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/images/QSpinBox_up_arrow.png
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/images/blender_icon_16.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:08:23.424806 bqt-1.2.2/bqt/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/ui/quit_dialogue.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-06-06 17:08:12.000000 bqt-1.2.2/bqt/widget_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:08:23.420806 bqt-1.2.2/bqt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-06 17:08:23.000000 bqt-1.2.2/bqt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-06 17:08:23.000000 bqt-1.2.2/bqt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 17:08:23.000000 bqt-1.2.2/bqt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 17:08:23.000000 bqt-1.2.2/bqt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-06 17:08:23.000000 bqt-1.2.2/bqt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 17:08:23.424806 bqt-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-06 17:08:12.000000 bqt-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:44:34.006703 bqt-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-06 17:44:23.000000 bqt-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-06 17:44:23.000000 bqt-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-06 17:44:34.006703 bqt-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-06 17:44:23.000000 bqt-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:44:34.002704 bqt-1.2.3/bqt/
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:44:34.006703 bqt-1.2.3/bqt/blender_applications/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/blender_applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/blender_applications/blender_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/blender_applications/darwin_blender_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/blender_applications/win32_blender_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/blender_stylesheet.qss
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/focus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:44:34.006703 bqt-1.2.3/bqt/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/images/QCheckBox_checked.png
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/images/QCheckBox_unchecked.png
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/images/QCheckbox_checked_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/images/QCheckbox_unchecked_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/images/QComboBox_down_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/images/QRadioButton_checked.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/images/QRadioButton_checked_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/images/QRadioButton_unchecked.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/images/QRadioButton_unchecked_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/images/QSpinBox_down_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/images/QSpinBox_up_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/images/blender_icon_16.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:44:34.006703 bqt-1.2.3/bqt/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/ui/quit_dialogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-06-06 17:44:23.000000 bqt-1.2.3/bqt/widget_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:44:34.006703 bqt-1.2.3/bqt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-06 17:44:33.000000 bqt-1.2.3/bqt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-06 17:44:34.000000 bqt-1.2.3/bqt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 17:44:33.000000 bqt-1.2.3/bqt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 17:44:33.000000 bqt-1.2.3/bqt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-06 17:44:33.000000 bqt-1.2.3/bqt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 17:44:34.006703 bqt-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-06 17:44:23.000000 bqt-1.2.3/setup.py
```

### Comparing `bqt-1.2.2/LICENSE` & `bqt-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bqt-1.2.2/PKG-INFO` & `bqt-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bqt
-Version: 1.2.2
+Version: 1.2.3
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
-|BQT_MANAGE_FOREGROUND| defaults to `1`, if `0`, widgets registered with `bqt.register(my_widget)` won't stay in the foreground when using Blender.|
+|BQT_MANAGE_FOREGROUND| defaults to `1`, if `0`, widgets registered with `bqt.add(my_widget)` won't stay in the foreground when using Blender.|
 |BQT_AUTO_ADD| defaults to `1`, if `0` top level widgets won't automatically be added to bqt.|
 
 - if you modify env vars, ensure they're strings
 - if you're unsure how to set env vars, google `set environment variable windows`.
 - Restart Blender (or your computer) after changing them.
 
 ### Sample code
```

### Comparing `bqt-1.2.2/README.md` & `bqt-1.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 ### Environment variables
 
 | variable | description|
 |--|--|
 |BQT_DISABLE_STARTUP| if set to `1`, completely disable bqt|
 |BQT_DISABLE_WRAP| if set to `1`, disable wrapping blender in a QWindow|
 |BQT_DISABLE_CLOSE_DIALOGUE| if set to `1`, use the standard blender close dialogue|
-|BQT_MANAGE_FOREGROUND| defaults to `1`, if `0`, widgets registered with `bqt.register(my_widget)` won't stay in the foreground when using Blender.|
+|BQT_MANAGE_FOREGROUND| defaults to `1`, if `0`, widgets registered with `bqt.add(my_widget)` won't stay in the foreground when using Blender.|
 |BQT_AUTO_ADD| defaults to `1`, if `0` top level widgets won't automatically be added to bqt.|
 
 - if you modify env vars, ensure they're strings
 - if you're unsure how to set env vars, google `set environment variable windows`.
 - Restart Blender (or your computer) after changing them.
 
 ### Sample code
```

### Comparing `bqt-1.2.2/bqt/__init__.py` & `bqt-1.2.3/bqt/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 from pathlib import Path
 
 
 bl_info = {
         "name": "PySide2 Qt wrapper (bqt)",
         "description": "Enable PySide2 QtWidgets in Blender",
         "author": "tech-artists.org",
-        "version": (1, 2, 2),
+        "version": (1, 2, 3),
         "blender": (2, 80, 0),
         # "location": "",
         # "warning": "", # used for warning icon and text in add-ons panel
         # "wiki_url": "http://my.wiki.url",
         # "tracker_url": "http://my.bugtracker.url",
         "support": "COMMUNITY",
         "category": "UI"
         }
 
-register = bqt.widget_manager.register
+add = bqt.widget_manager.register
 
 # CORE FUNCTIONS #
 
 def _instantiate_QApplication() -> "bqt.blender_applications.BlenderApplication":
     # enable dpi scale, run before creating QApplication
     QApplication.setHighDpiScaleFactorRoundingPolicy(QtCore.Qt.HighDpiScaleFactorRoundingPolicy.PassThrough)
     QApplication.setAttribute(QtCore.Qt.AA_EnableHighDpiScaling)
```

### Comparing `bqt-1.2.2/bqt/blender_applications/__init__.py` & `bqt-1.2.3/bqt/blender_applications/__init__.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.2/bqt/blender_applications/blender_application.py` & `bqt-1.2.3/bqt/blender_applications/blender_application.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.2/bqt/blender_applications/darwin_blender_application.py` & `bqt-1.2.3/bqt/blender_applications/darwin_blender_application.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.2/bqt/blender_applications/win32_blender_application.py` & `bqt-1.2.3/bqt/blender_applications/win32_blender_application.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.2/bqt/blender_stylesheet.qss` & `bqt-1.2.3/bqt/blender_stylesheet.qss`

 * *Files identical despite different names*

### Comparing `bqt-1.2.2/bqt/focus.py` & `bqt-1.2.3/bqt/focus.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.2/bqt/images/QCheckBox_checked.png` & `bqt-1.2.3/bqt/images/QCheckBox_checked.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.2/bqt/images/QCheckBox_unchecked.png` & `bqt-1.2.3/bqt/images/QCheckBox_unchecked.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.2/bqt/images/QCheckbox_checked_hover.png` & `bqt-1.2.3/bqt/images/QCheckbox_checked_hover.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.2/bqt/images/QCheckbox_unchecked_hover.png` & `bqt-1.2.3/bqt/images/QCheckbox_unchecked_hover.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.2/bqt/images/QComboBox_down_arrow.png` & `bqt-1.2.3/bqt/images/QComboBox_down_arrow.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.2/bqt/images/QRadioButton_checked.png` & `bqt-1.2.3/bqt/images/QRadioButton_checked.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.2/bqt/images/QRadioButton_checked_hover.png` & `bqt-1.2.3/bqt/images/QRadioButton_checked_hover.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.2/bqt/images/QRadioButton_unchecked.png` & `bqt-1.2.3/bqt/images/QRadioButton_unchecked.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.2/bqt/images/QRadioButton_unchecked_hover.png` & `bqt-1.2.3/bqt/images/QRadioButton_unchecked_hover.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.2/bqt/images/QSpinBox_down_arrow.png` & `bqt-1.2.3/bqt/images/QSpinBox_down_arrow.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.2/bqt/images/QSpinBox_up_arrow.png` & `bqt-1.2.3/bqt/images/QSpinBox_up_arrow.png`

 * *Files identical despite different names*

### Comparing `bqt-1.2.2/bqt/ui/__init__.py` & `bqt-1.2.3/bqt/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.2/bqt/ui/quit_dialogue.py` & `bqt-1.2.3/bqt/ui/quit_dialogue.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.2/bqt/utils.py` & `bqt-1.2.3/bqt/utils.py`

 * *Files identical despite different names*

### Comparing `bqt-1.2.2/bqt/widget_manager.py` & `bqt-1.2.3/bqt/widget_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,14 +64,21 @@
 def iter_widget_data():
     """iterate over all registered widgets, remove widgets that have been removed"""
     cleanup = []
     for widget_data in __widgets:
         if not widget_data.widget:
             cleanup.append(widget_data)
             continue
+
+        try:
+            v = widget_data.widget.isVisible()
+        except RuntimeError:
+            cleanup.append(widget_data)
+            continue
+
         yield widget_data
     for widget_data in cleanup:
         __widgets.remove(widget_data)
 
 
 def _blender_window_change(hwnd: int):
     """
@@ -113,8 +120,17 @@
 
 
 def parent_orphan_widgets(exclude=None):
     """Find and parent orphan widgets to the blender widget"""
     exclude = exclude or []
     __excluded_widgets.extend(exclude)
     for widget in _orphan_toplevel_widgets():
+
+        # check if widget is window type, else skip and exclude
+        if not widget.windowType() == Qt.Window:
+            __excluded_widgets.append(widget)
+            continue
+        # todo test with various widgets, we likely exclude some valid widgets
+        #  this should fail with a combobox (dropdown) and menu
+
         register(widget, exclude=exclude)
+
```

### Comparing `bqt-1.2.2/bqt.egg-info/PKG-INFO` & `bqt-1.2.3/bqt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bqt
-Version: 1.2.2
+Version: 1.2.3
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
-|BQT_MANAGE_FOREGROUND| defaults to `1`, if `0`, widgets registered with `bqt.register(my_widget)` won't stay in the foreground when using Blender.|
+|BQT_MANAGE_FOREGROUND| defaults to `1`, if `0`, widgets registered with `bqt.add(my_widget)` won't stay in the foreground when using Blender.|
 |BQT_AUTO_ADD| defaults to `1`, if `0` top level widgets won't automatically be added to bqt.|
 
 - if you modify env vars, ensure they're strings
 - if you're unsure how to set env vars, google `set environment variable windows`.
 - Restart Blender (or your computer) after changing them.
 
 ### Sample code
```

### Comparing `bqt-1.2.2/bqt.egg-info/SOURCES.txt` & `bqt-1.2.3/bqt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bqt-1.2.2/setup.py` & `bqt-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         # Run the standard PyPi Copy
         install.run(self)
 
 
 setup(
     # Metadata
     name="bqt",
-    version="1.2.2",
+    version="1.2.3",
     description="Files to help bootstrap PySide2 with an event loop within Blender.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=["Technical", "Art", "TechArt", "TechArtOrg", "Blender", "Qt", "PySide"],
     license="Mozilla Public License 2.0 (MPL 2.0)",
     url="https://github.com/techartorg/bqt",
     author="tech-artists.org",
```

