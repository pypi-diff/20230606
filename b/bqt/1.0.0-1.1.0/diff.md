# Comparing `tmp/bqt-1.0.0.tar.gz` & `tmp/bqt-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bqt-1.0.0.tar", last modified: Mon Jun  5 15:15:34 2023, max compression
+gzip compressed data, was "bqt-1.1.0.tar", last modified: Tue Jun  6 12:32:43 2023, max compression
```

## Comparing `bqt-1.0.0.tar` & `bqt-1.1.0.tar`

### file list

```diff
@@ -1,46 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:15:34.875142 bqt-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-05 15:15:25.000000 bqt-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-05 15:15:25.000000 bqt-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-06-05 15:15:34.875142 bqt-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-06-05 15:15:25.000000 bqt-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:15:34.867142 bqt-1.0.0/bqt/
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:15:34.867142 bqt-1.0.0/bqt/blender_applications/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/blender_applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/blender_applications/blender_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/blender_applications/darwin_blender_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/blender_applications/win32_blender_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/blender_stylesheet.qss
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/focus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:15:34.871142 bqt-1.0.0/bqt/images/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/images/QCheckBox_checked.png
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/images/QCheckBox_unchecked.png
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/images/QCheckbox_checked_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/images/QCheckbox_unchecked_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/images/QComboBox_down_arrow.png
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/images/QRadioButton_checked.png
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/images/QRadioButton_checked_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/images/QRadioButton_unchecked.png
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/images/QRadioButton_unchecked_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/images/QSpinBox_down_arrow.png
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/images/QSpinBox_up_arrow.png
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/images/blender_icon_16.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:15:34.871142 bqt-1.0.0/bqt/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/ui/quit_dialogue.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:15:34.867142 bqt-1.0.0/bqt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-06-05 15:15:34.000000 bqt-1.0.0/bqt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-05 15:15:34.000000 bqt-1.0.0/bqt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:15:34.000000 bqt-1.0.0/bqt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 15:15:34.000000 bqt-1.0.0/bqt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 15:15:34.000000 bqt-1.0.0/bqt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:15:34.875142 bqt-1.0.0/bqt_demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt_demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt_demo/anim_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt_demo/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt_demo/hello_world.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt_demo/pyside_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-05 15:15:25.000000 bqt-1.0.0/bqt_demo/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 15:15:34.875142 bqt-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-05 15:15:25.000000 bqt-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:32:43.861122 bqt-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-06 12:32:34.000000 bqt-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-06 12:32:34.000000 bqt-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-06-06 12:32:43.861122 bqt-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-06 12:32:34.000000 bqt-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:32:43.857123 bqt-1.1.0/bqt/
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:32:43.861122 bqt-1.1.0/bqt/blender_applications/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/blender_applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/blender_applications/blender_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/blender_applications/darwin_blender_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/blender_applications/win32_blender_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/blender_stylesheet.qss
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/focus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:32:43.861122 bqt-1.1.0/bqt/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/images/QCheckBox_checked.png
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/images/QCheckBox_unchecked.png
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/images/QCheckbox_checked_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/images/QCheckbox_unchecked_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/images/QComboBox_down_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/images/QRadioButton_checked.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/images/QRadioButton_checked_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/images/QRadioButton_unchecked.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/images/QRadioButton_unchecked_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/images/QSpinBox_down_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/images/QSpinBox_up_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/images/blender_icon_16.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:32:43.861122 bqt-1.1.0/bqt/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/ui/quit_dialogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-06 12:32:34.000000 bqt-1.1.0/bqt/widget_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:32:43.861122 bqt-1.1.0/bqt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-06-06 12:32:43.000000 bqt-1.1.0/bqt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-06 12:32:43.000000 bqt-1.1.0/bqt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 12:32:43.000000 bqt-1.1.0/bqt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 12:32:43.000000 bqt-1.1.0/bqt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-06 12:32:43.000000 bqt-1.1.0/bqt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 12:32:43.861122 bqt-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-06 12:32:34.000000 bqt-1.1.0/setup.py
```

### Comparing `bqt-1.0.0/LICENSE` & `bqt-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bqt-1.0.0/PKG-INFO` & `bqt-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bqt
-Version: 1.0.0
+Version: 1.1.0
 Summary: Files to help bootstrap PySide2 with an event loop within Blender.
 Home-page: https://github.com/techartorg/bqt
 Author: tech-artists.org
 License: Mozilla Public License 2.0 (MPL 2.0)
 Keywords: Technical,Art,TechArt,TechArtOrg,Blender,Qt,PySide
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -15,15 +15,15 @@
 License-File: LICENSE
 
 # bqt
 
 
 
 [![PyPI version](https://img.shields.io/pypi/v/bqt)](https://pypi.org/project/bqt/)
-[![latest tag](https://img.shields.io/github/v/tag/techartorg/bqt?label=Github)](https://github.com/techartorg/bqt) ⚠️ PyPi version is currently outdated. Install from this repo for latest.
+[![latest tag](https://img.shields.io/github/v/tag/techartorg/bqt?label=Github)](https://github.com/techartorg/bqt)
 
 
 Add QT support to Blender, letting you create custom UI for your addons with PySide2 QtWidgets.
 ![custom ui sample](https://user-images.githubusercontent.com/3758308/192096952-e9ed73be-26e4-4ad8-a85f-be4175cebbda.gif)
 
 ## Features
 | feature | description|
@@ -42,17 +42,15 @@
 ## Installation  
 
 ### install as addon (recommended)
 1. Download the latest release. You can download the zip from the repo.
 2. Extract the zip and copy the `bqt` folder to your blender addons folder.
 3. Enable the addon by going to `Edit > Preferences > Add-ons` and search for `qt`
 
-### PIP install (outdated)
-⚠ PIP install is currently outdated, do not use until further notice.
-
+### PIP install
 The installation of bqt with automatic setup for Blender requires the usage of the integrated python
 interpreter found within `../Blender Foundation/<version>/Python/bin`
 ```commandline
 python.exe -m pip install bqt
 ```
 
 ### Installing from Source
@@ -68,17 +66,21 @@
 Any updates in the repo are then reflected in blender on restart.
 e.g.:
 ```commandline
 mklink /J "C:\Users\USERNAME\AppData\Roaming\Blender Foundation\Blender\2.93\scripts\addons\bqt" "C:\Users\hanne\OneDrive\Documents\repos\_Blender\bqt\bqt"
 ```
 
 ### Environment variables
-- BQT_DISABLE_STARTUP if set to 1, completely disable bqt
-- BQT_DISABLE_WRAP if set to 1, disable wrapping blender in a QWindow
-- BQT_DISABLE_CLOSE_DIALOGUE if set to 1, use the standard blender close dialogue
+| variable | description|
+|--|--|
+|BQT_DISABLE_STARTUP| if set to `1`, completely disable bqt|
+|BQT_DISABLE_WRAP| if set to `1`, disable wrapping blender in a QWindow|
+|BQT_DISABLE_CLOSE_DIALOGUE| if set to `1`, use the standard blender close dialogue|
+|BQT_MANAGE_FOREGROUND| defaults to `1`, if `0`, widgets registered with `bqt.add(my_widget)` won't stay in the foreground when using Blender.|
+if you modify env vars, ensure they're strings
 
 ### Sample code
 [bqt_demo](bqt_demo) shows you how to use bqt with several qt demos you can run in Blender
 
 ### Community
 Discuss BQT on 
 - the BlenderArtists [thread](https://blenderartists.org/t/bqt-custom-ui-for-add-ons-tool-in-blender-with-pyqt-or-pyside/1458808)
```

### Comparing `bqt-1.0.0/README.md` & `bqt-1.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # bqt
 
 
 
 [![PyPI version](https://img.shields.io/pypi/v/bqt)](https://pypi.org/project/bqt/)
-[![latest tag](https://img.shields.io/github/v/tag/techartorg/bqt?label=Github)](https://github.com/techartorg/bqt) ⚠️ PyPi version is currently outdated. Install from this repo for latest.
+[![latest tag](https://img.shields.io/github/v/tag/techartorg/bqt?label=Github)](https://github.com/techartorg/bqt)
 
 
 Add QT support to Blender, letting you create custom UI for your addons with PySide2 QtWidgets.
 ![custom ui sample](https://user-images.githubusercontent.com/3758308/192096952-e9ed73be-26e4-4ad8-a85f-be4175cebbda.gif)
 
 ## Features
 | feature | description|
@@ -26,17 +26,15 @@
 ## Installation  
 
 ### install as addon (recommended)
 1. Download the latest release. You can download the zip from the repo.
 2. Extract the zip and copy the `bqt` folder to your blender addons folder.
 3. Enable the addon by going to `Edit > Preferences > Add-ons` and search for `qt`
 
-### PIP install (outdated)
-⚠ PIP install is currently outdated, do not use until further notice.
-
+### PIP install
 The installation of bqt with automatic setup for Blender requires the usage of the integrated python
 interpreter found within `../Blender Foundation/<version>/Python/bin`
 ```commandline
 python.exe -m pip install bqt
 ```
 
 ### Installing from Source
@@ -52,17 +50,21 @@
 Any updates in the repo are then reflected in blender on restart.
 e.g.:
 ```commandline
 mklink /J "C:\Users\USERNAME\AppData\Roaming\Blender Foundation\Blender\2.93\scripts\addons\bqt" "C:\Users\hanne\OneDrive\Documents\repos\_Blender\bqt\bqt"
 ```
 
 ### Environment variables
-- BQT_DISABLE_STARTUP if set to 1, completely disable bqt
-- BQT_DISABLE_WRAP if set to 1, disable wrapping blender in a QWindow
-- BQT_DISABLE_CLOSE_DIALOGUE if set to 1, use the standard blender close dialogue
+| variable | description|
+|--|--|
+|BQT_DISABLE_STARTUP| if set to `1`, completely disable bqt|
+|BQT_DISABLE_WRAP| if set to `1`, disable wrapping blender in a QWindow|
+|BQT_DISABLE_CLOSE_DIALOGUE| if set to `1`, use the standard blender close dialogue|
+|BQT_MANAGE_FOREGROUND| defaults to `1`, if `0`, widgets registered with `bqt.add(my_widget)` won't stay in the foreground when using Blender.|
+if you modify env vars, ensure they're strings
 
 ### Sample code
 [bqt_demo](bqt_demo) shows you how to use bqt with several qt demos you can run in Blender
 
 ### Community
 Discuss BQT on 
 - the BlenderArtists [thread](https://blenderartists.org/t/bqt-custom-ui-for-add-ons-tool-in-blender-with-pyqt-or-pyside/1458808)
```

### Comparing `bqt-1.0.0/bqt/__init__.py` & `bqt-1.1.0/bqt/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,34 +28,29 @@
         "support": "COMMUNITY",
         "category": "UI"
         }
 
 
 # CORE FUNCTIONS #
 
-def instantiate_application() -> "bqt.blender_applications.BlenderApplication":
-    """
-    Create an instance of Blender Application
-
-    Returns BlenderApplication: Application Instance
-
-    """
+def _instantiate_QApplication() -> "bqt.blender_applications.BlenderApplication":
     # enable dpi scale, run before creating QApplication
     QApplication.setHighDpiScaleFactorRoundingPolicy(QtCore.Qt.HighDpiScaleFactorRoundingPolicy.PassThrough)
     QApplication.setAttribute(QtCore.Qt.AA_EnableHighDpiScaling)
     QApplication.setAttribute(QtCore.Qt.AA_UseHighDpiPixmaps)
+
+    # add image directory to Qt search path, for blender_stylesheet
     image_directory = str(Path(__file__).parent / "images")
-    QDir.addSearchPath('images', image_directory)
-    app = QApplication.instance()
-    if not app:
-        app = load_os_module()
+    QDir.addSearchPath('images', image_directory)  # todo this is generic, might clash with other qt scripts
+
+    app = _load_os_module()
     return app
 
 
-def load_os_module() -> "bqt.blender_applications.BlenderApplication":
+def _load_os_module() -> "bqt.blender_applications.BlenderApplication":
     """Loads the correct OS platform Application Class"""
     operating_system = sys.platform
     if operating_system == "darwin":
         from .blender_applications.darwin_blender_application import DarwinBlenderApplication
 
         return DarwinBlenderApplication(sys.argv)
 
@@ -66,21 +61,21 @@
     elif operating_system == "win32":
         from .blender_applications.win32_blender_application import Win32BlenderApplication
 
         return Win32BlenderApplication(sys.argv)
 
 
 @bpy.app.handlers.persistent
-def create_global_app():
+def _create_global_app():
     """
     Create a global QApplication instance, that's maintained between Blender sessions.
     Runs after Blender finished startup.
     """
     # global qapp
-    qapp = instantiate_application()
+    qapp = _instantiate_QApplication()
 
     # save a reference to the C++ window in a global var, to prevent the parent being garbage collected
     # for some reason this works here, but not in the blender_applications init as a class attribute (self),
     # and saving it in a global in blender_applications.py causes blender to crash on startup
     global parent_window
     parent_window = qapp._blender_window.parent()
 
@@ -96,21 +91,15 @@
         logging.warning("bqt: QApplication already exists, skipping bqt registration")
         return
 
     if os.getenv("BQT_DISABLE_STARTUP", 0) == "1":
         logging.warning("bqt: BQT_DISABLE_STARTUP is set, skipping bqt registration")
         return
 
-    # only start focus operator if blender is wrapped
-    if not os.getenv("BQT_DISABLE_WRAP", 0) == "1":
-        # todo check if operator is already registered
-        bpy.utils.register_class(bqt.focus.QFocusOperator)
-        # append add_focus_handle before create_global_app, else it doesn't run on blender startup
-
-    create_global_app()
+    _create_global_app()
 
 
 def unregister():
     """
     Runs on disabling the add-on.
     """
     # todo, as long as blender is wrapped in qt, unregistering operator & callback will cause issues,
```

### Comparing `bqt-1.0.0/bqt/blender_applications/__init__.py` & `bqt-1.1.0/bqt/blender_applications/__init__.py`

 * *Files identical despite different names*

### Comparing `bqt-1.0.0/bqt/blender_applications/blender_application.py` & `bqt-1.1.0/bqt/blender_applications/blender_application.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,72 +3,103 @@
 License, v. 2.0. If a copy of the MPL was not distributed with this
 file, You can obtain one at https://mozilla.org/MPL/2.0/.
 """
 
 from abc import abstractmethod, abstractstaticmethod, ABCMeta
 from pathlib import Path
 import os
-from PySide2.QtWidgets import QApplication, QWidget
-from PySide2.QtWidgets import QMainWindow
+from PySide2.QtWidgets import QApplication, QWidget, QPushButton, QDockWidget, QMainWindow
 from PySide2.QtGui import QCloseEvent, QIcon, QImage, QPixmap, QWindow
-from PySide2.QtCore import QEvent, QObject, QRect, QSettings
+from PySide2.QtCore import QEvent, QObject, QRect, QSettings, QTimer, Qt
 from bqt.ui.quit_dialogue import BlenderClosingDialog
 import bpy
+import bqt.widget_manager
 
 
 STYLESHEET_PATH = Path(__file__).parents[1] / "blender_stylesheet.qss"
 ORGANISATION = "Tech-Artists.org"
 APP = "Blender Qt"
 WINDOW_TITLE = "Blender Qt"
 WINDOW_GROUP_NAME = "MainWindow"
 GEOMETRY = "Geometry"
 MAXIMIZED = "IsMaximized"
 FULL_SCREEN = "IsFullScreen"
+FOCUS_FRAMERATE = 15
 
 
 class BlenderApplication(QApplication):
     """
     Base Implementation for QT Blender Window Container
     """
 
     def __init__(self, *args, **kwargs):
         __metaclass__ = ABCMeta
         super().__init__(*args, **kwargs)
 
+        self._active_window_hwnd = 0
+
         if STYLESHEET_PATH.exists():
             self.setStyleSheet(STYLESHEET_PATH.read_text())
 
         QApplication.setWindowIcon(self._get_application_icon())
 
         # Blender Window
-        self._hwnd = self._get_application_hwnd()
+        self._hwnd = self._get_blender_hwnd()
         failed_to_get_handle = self._hwnd is None
 
         if os.getenv("BQT_DISABLE_WRAP") == "1" or failed_to_get_handle:
             self._blender_window = QWindow()
             self.blender_widget = QWidget.createWindowContainer(self._blender_window)
         else:
             self.blender_widget = QMainWindow()
             self.blender_widget.setWindowTitle(WINDOW_TITLE)
             self._blender_window = QWindow.fromWinId(self._hwnd)  # also sets flag to Qt.ForeignWindow
             self.window_container = QMainWindow.createWindowContainer(self._blender_window)
             self.blender_widget.setCentralWidget(self.window_container)
+
             self._set_window_geometry()
             self.blender_widget.show()
             self.focusObjectChanged.connect(self._on_focus_object_changed)
 
-    @abstractstaticmethod
-    def _get_application_hwnd() -> int:
-        """
-        This finds the blender application window and collects the
-        handler window ID
+        self.timer = QTimer()
+        self.timer.timeout.connect(self.on_update)
+        tick = int(1000 / FOCUS_FRAMERATE)  # tick 1000 / frames per second
+        self.timer.start(tick)
+
+    def on_update(self):
+        # we only need foreground managing if blender is not wrapped
+        if os.getenv("BQT_DISABLE_WRAP") == "1" and os.getenv("BQT_MANAGE_FOREGROUND", "1") == "1" and self.blender_focus_toggled():
+            bqt.widget_manager._blender_window_change(self._active_window_hwnd)
+
+    def blender_focus_toggled(self):
+        """returns true the first frame the blender window is focussed or unfoccused"""
+        current_active_hwnd = self._get_active_window_handle()
+        handle_changed = self._active_window_hwnd != current_active_hwnd
+        if not handle_changed:
+            self._active_window_hwnd = current_active_hwnd
+            return False
+        else:
+            # we toggled between 2 windows, but we only care if we toggled in or out of blender
+            non_blender_toggle = self._active_window_hwnd == 0 or current_active_hwnd == 0
+            self._active_window_hwnd = current_active_hwnd
+            return non_blender_toggle
 
-        Returns int: Handler Window ID
-        """
 
+    @staticmethod
+    def _get_active_window_handle():
+        # override this method to get the active window handle
+        return 0
+
+    @staticmethod
+    def _focus_window():
+        pass
+
+    @abstractstaticmethod
+    def _get_blender_hwnd() -> int:
+        """Get the handler window ID for the blender application window"""
         return -1
 
     @staticmethod
     def _get_application_icon() -> QIcon:
         """
         This finds the running blender process, extracts the blender icon from the blender.exe file on disk and saves it to the user's temp folder.
         It then creates a QIcon with that data and returns it.
@@ -143,14 +174,15 @@
         """
         Args:
             receiver: Object to receive event
             event: Event
 
         Returns: bool
         """
+        # todo believe this func sometimes freezes blender, ctrl-c keyboard interrupt in console shows this func as the culprit
 
         if isinstance(event, QCloseEvent) and receiver in (self.blender_widget, self._blender_window):
             # catch the close event when clicking close on the qt window,
             # ignore the event, and ask user if they want to close blender if unsaved changes.
             event.ignore()
 
             self.store_window_geometry()  # save qt window geometry, to restore on next launch
```

### Comparing `bqt-1.0.0/bqt/blender_applications/darwin_blender_application.py` & `bqt-1.1.0/bqt/blender_applications/darwin_blender_application.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,28 +13,29 @@
     import AppKit
     import objc
 
 from PySide2.QtGui import QIcon
 from PySide2.QtCore import QObject
 
 from .blender_application import BlenderApplication
+import bqt.focus
 
 
 class DarwinBlenderApplication(BlenderApplication):
     """
     Darwin (MACOS) Implementation of BlenderApplication
     """
 
     def __init__(self, *args, **kwargs):
         # OSX Specific - Needs to initialize first
         self._ns_window = self.__get_application_window() or None
 
         super().__init__(*args, **kwargs)
 
-    def _get_application_hwnd(self) -> int:
+    def _get_blender_hwnd(self) -> int:
         """
         This finds the blender application window and collects the
         handler window ID
 
         Returns int: Handler Window ID
         """
 
@@ -74,9 +75,8 @@
         """
         Args:
             focus_object: Object to track focus event
         """
 
         if focus_object is self.blender_widget:
             self._ns_window.makeKey()
-            with bpy.context.temp_override(window=bpy.context.window_manager.windows[0]):
-                bpy.ops.bqt.return_focus("INVOKE_DEFAULT")
+            bqt.focus._detect_keyboard(self._hwnd)
```

### Comparing `bqt-1.0.0/bqt/blender_applications/win32_blender_application.py` & `bqt-1.1.0/bqt/blender_applications/win32_blender_application.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 file, You can obtain one at https://mozilla.org/MPL/2.0/.
 """
 import bpy
 from PySide2.QtCore import QObject
 from .blender_application import BlenderApplication
 import ctypes
 import os
-from ctypes import wintypes
 from collections import namedtuple
 import logging
+import bqt.focus
+from ctypes import wintypes
 user32 = ctypes.windll.user32
 
 def get_class_name(hwnd):
     # returns "GHOST_WindowClass" for Blender and BlenderWindows (e.g. Preferences),
     # returns "PseudoConsoleWindow" for the terminal window
     buf_len = 256
     buf = ctypes.create_unicode_buffer(buf_len)
@@ -115,27 +116,35 @@
     Windows implementation of BlenderApplication
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     @staticmethod
-    def _get_application_hwnd() -> int or None:
-        """
-        This finds the blender application window and collects the
-        handler window ID
-
-        Returns int: Handler Window ID
-        """
-
+    def _get_blender_hwnd() -> int or None:
+        """Get the handler window ID for the blender application window"""
         hwnd = get_blender_window()
         return hwnd
 
     def _on_focus_object_changed(self, focus_object: QObject):
         """
         Args:
             QObject focus_object: Object to track focus change
         """
         if focus_object is self.blender_widget:
             ctypes.windll.user32.SetFocus(self._hwnd)
-            with bpy.context.temp_override(window=bpy.context.window_manager.windows[0]):
-                bpy.ops.bqt.return_focus("INVOKE_DEFAULT")
+            bqt.focus._detect_keyboard(self._hwnd)
+
+    @staticmethod
+    def _get_active_window_handle():
+        """
+        Get the handle from the window that's currently in focus.
+        Returns 0 for active windows not managed by Blender
+        """
+        # note that negative values are also possible
+        return user32.GetActiveWindow()
+
+    @staticmethod
+    def _focus_window(hwnd):
+        """Focus the window with the given handle."""
+        user32.SetForegroundWindow(hwnd)
+        # user32.SetFocus(hwnd)
```

### Comparing `bqt-1.0.0/bqt/blender_stylesheet.qss` & `bqt-1.1.0/bqt/blender_stylesheet.qss`

 * *Files identical despite different names*

### Comparing `bqt-1.0.0/bqt/images/QCheckBox_checked.png` & `bqt-1.1.0/bqt/images/QCheckBox_checked.png`

 * *Files identical despite different names*

### Comparing `bqt-1.0.0/bqt/images/QCheckBox_unchecked.png` & `bqt-1.1.0/bqt/images/QCheckBox_unchecked.png`

 * *Files identical despite different names*

### Comparing `bqt-1.0.0/bqt/images/QCheckbox_checked_hover.png` & `bqt-1.1.0/bqt/images/QCheckbox_checked_hover.png`

 * *Files identical despite different names*

### Comparing `bqt-1.0.0/bqt/images/QCheckbox_unchecked_hover.png` & `bqt-1.1.0/bqt/images/QCheckbox_unchecked_hover.png`

 * *Files identical despite different names*

### Comparing `bqt-1.0.0/bqt/images/QComboBox_down_arrow.png` & `bqt-1.1.0/bqt/images/QComboBox_down_arrow.png`

 * *Files identical despite different names*

### Comparing `bqt-1.0.0/bqt/images/QRadioButton_checked.png` & `bqt-1.1.0/bqt/images/QRadioButton_checked.png`

 * *Files identical despite different names*

### Comparing `bqt-1.0.0/bqt/images/QRadioButton_checked_hover.png` & `bqt-1.1.0/bqt/images/QRadioButton_checked_hover.png`

 * *Files identical despite different names*

### Comparing `bqt-1.0.0/bqt/images/QRadioButton_unchecked.png` & `bqt-1.1.0/bqt/images/QRadioButton_unchecked.png`

 * *Files identical despite different names*

### Comparing `bqt-1.0.0/bqt/images/QRadioButton_unchecked_hover.png` & `bqt-1.1.0/bqt/images/QRadioButton_unchecked_hover.png`

 * *Files identical despite different names*

### Comparing `bqt-1.0.0/bqt/images/QSpinBox_down_arrow.png` & `bqt-1.1.0/bqt/images/QSpinBox_down_arrow.png`

 * *Files identical despite different names*

### Comparing `bqt-1.0.0/bqt/images/QSpinBox_up_arrow.png` & `bqt-1.1.0/bqt/images/QSpinBox_up_arrow.png`

 * *Files identical despite different names*

### Comparing `bqt-1.0.0/bqt/ui/quit_dialogue.py` & `bqt-1.1.0/bqt/ui/quit_dialogue.py`

 * *Files identical despite different names*

### Comparing `bqt-1.0.0/bqt/utils.py` & `bqt-1.1.0/bqt/utils.py`

 * *Files identical despite different names*

### Comparing `bqt-1.0.0/bqt.egg-info/PKG-INFO` & `bqt-1.1.0/bqt.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bqt
-Version: 1.0.0
+Version: 1.1.0
 Summary: Files to help bootstrap PySide2 with an event loop within Blender.
 Home-page: https://github.com/techartorg/bqt
 Author: tech-artists.org
 License: Mozilla Public License 2.0 (MPL 2.0)
 Keywords: Technical,Art,TechArt,TechArtOrg,Blender,Qt,PySide
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -15,15 +15,15 @@
 License-File: LICENSE
 
 # bqt
 
 
 
 [![PyPI version](https://img.shields.io/pypi/v/bqt)](https://pypi.org/project/bqt/)
-[![latest tag](https://img.shields.io/github/v/tag/techartorg/bqt?label=Github)](https://github.com/techartorg/bqt) ⚠️ PyPi version is currently outdated. Install from this repo for latest.
+[![latest tag](https://img.shields.io/github/v/tag/techartorg/bqt?label=Github)](https://github.com/techartorg/bqt)
 
 
 Add QT support to Blender, letting you create custom UI for your addons with PySide2 QtWidgets.
 ![custom ui sample](https://user-images.githubusercontent.com/3758308/192096952-e9ed73be-26e4-4ad8-a85f-be4175cebbda.gif)
 
 ## Features
 | feature | description|
@@ -42,17 +42,15 @@
 ## Installation  
 
 ### install as addon (recommended)
 1. Download the latest release. You can download the zip from the repo.
 2. Extract the zip and copy the `bqt` folder to your blender addons folder.
 3. Enable the addon by going to `Edit > Preferences > Add-ons` and search for `qt`
 
-### PIP install (outdated)
-⚠ PIP install is currently outdated, do not use until further notice.
-
+### PIP install
 The installation of bqt with automatic setup for Blender requires the usage of the integrated python
 interpreter found within `../Blender Foundation/<version>/Python/bin`
 ```commandline
 python.exe -m pip install bqt
 ```
 
 ### Installing from Source
@@ -68,17 +66,21 @@
 Any updates in the repo are then reflected in blender on restart.
 e.g.:
 ```commandline
 mklink /J "C:\Users\USERNAME\AppData\Roaming\Blender Foundation\Blender\2.93\scripts\addons\bqt" "C:\Users\hanne\OneDrive\Documents\repos\_Blender\bqt\bqt"
 ```
 
 ### Environment variables
-- BQT_DISABLE_STARTUP if set to 1, completely disable bqt
-- BQT_DISABLE_WRAP if set to 1, disable wrapping blender in a QWindow
-- BQT_DISABLE_CLOSE_DIALOGUE if set to 1, use the standard blender close dialogue
+| variable | description|
+|--|--|
+|BQT_DISABLE_STARTUP| if set to `1`, completely disable bqt|
+|BQT_DISABLE_WRAP| if set to `1`, disable wrapping blender in a QWindow|
+|BQT_DISABLE_CLOSE_DIALOGUE| if set to `1`, use the standard blender close dialogue|
+|BQT_MANAGE_FOREGROUND| defaults to `1`, if `0`, widgets registered with `bqt.add(my_widget)` won't stay in the foreground when using Blender.|
+if you modify env vars, ensure they're strings
 
 ### Sample code
 [bqt_demo](bqt_demo) shows you how to use bqt with several qt demos you can run in Blender
 
 ### Community
 Discuss BQT on 
 - the BlenderArtists [thread](https://blenderartists.org/t/bqt-custom-ui-for-add-ons-tool-in-blender-with-pyqt-or-pyside/1458808)
```

### Comparing `bqt-1.0.0/bqt.egg-info/SOURCES.txt` & `bqt-1.1.0/bqt.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 setup.py
 bqt/__init__.py
 bqt/blender_stylesheet.qss
 bqt/focus.py
 bqt/utils.py
+bqt/widget_manager.py
 bqt.egg-info/PKG-INFO
 bqt.egg-info/SOURCES.txt
 bqt.egg-info/dependency_links.txt
 bqt.egg-info/requires.txt
 bqt.egg-info/top_level.txt
 bqt/blender_applications/__init__.py
 bqt/blender_applications/blender_application.py
@@ -24,14 +25,8 @@
 bqt/images/QRadioButton_checked_hover.png
 bqt/images/QRadioButton_unchecked.png
 bqt/images/QRadioButton_unchecked_hover.png
 bqt/images/QSpinBox_down_arrow.png
 bqt/images/QSpinBox_up_arrow.png
 bqt/images/blender_icon_16.png
 bqt/ui/__init__.py
-bqt/ui/quit_dialogue.py
-bqt_demo/__init__.py
-bqt_demo/anim_bar.py
-bqt_demo/demo.py
-bqt_demo/hello_world.py
-bqt_demo/pyside_widgets.py
-bqt_demo/timer.py
+bqt/ui/quit_dialogue.py
```

### Comparing `bqt-1.0.0/setup.py` & `bqt-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         # Run the standard PyPi Copy
         install.run(self)
 
 
 setup(
     # Metadata
     name="bqt",
-    version="1.0.0",
+    version="1.1.0",
     description="Files to help bootstrap PySide2 with an event loop within Blender.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=["Technical", "Art", "TechArt", "TechArtOrg", "Blender", "Qt", "PySide"],
     license="Mozilla Public License 2.0 (MPL 2.0)",
     url="https://github.com/techartorg/bqt",
     author="tech-artists.org",
@@ -51,15 +51,15 @@
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
         "Programming Language :: Python :: 3.7",
     ],
     # Requirements
     python_requires=">=3.7",
-    packages=find_packages(),
+    packages=["bqt"],
     install_requires=["PySide2"],
     # Package Data
     include_package_data=True,
     package_data={"bqt": ["*.png", "*.qss"]},
     # Install Wrapper
     cmdclass={"install": CustomInstall},
 )
```

