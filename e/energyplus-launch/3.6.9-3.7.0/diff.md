# Comparing `tmp/energyplus_launch-3.6.9.tar.gz` & `tmp/energyplus_launch-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energyplus_launch-3.6.9.tar", last modified: Fri Jun  2 21:22:00 2023, max compression
+gzip compressed data, was "energyplus_launch-3.7.0.tar", last modified: Tue Jun  6 15:02:26 2023, max compression
```

## Comparing `energyplus_launch-3.6.9.tar` & `energyplus_launch-3.7.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 21:22:00.714933 energyplus_launch-3.6.9/
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-06-02 21:22:00.714933 energyplus_launch-3.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 21:22:00.710933 energyplus_launch-3.6.9/energyplus_launch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-06-02 21:22:00.000000 energyplus_launch-3.6.9/energyplus_launch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1300 2023-06-02 21:22:00.000000 energyplus_launch-3.6.9/energyplus_launch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 21:22:00.000000 energyplus_launch-3.6.9/energyplus_launch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-06-02 21:22:00.000000 energyplus_launch-3.6.9/energyplus_launch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-02 21:22:00.000000 energyplus_launch-3.6.9/energyplus_launch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-02 21:22:00.000000 energyplus_launch-3.6.9/energyplus_launch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 21:22:00.710933 energyplus_launch-3.6.9/eplaunch/
--rw-r--r--   0 runner    (1001) docker     (122)      389 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/configure.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 21:22:00.710933 energyplus_launch-3.6.9/eplaunch/interface/
--rw-r--r--   0 runner    (1001) docker     (122)      618 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9400 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/interface/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6090 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/interface/dialog_external_viewers.py
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/interface/dialog_generic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2366 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/interface/dialog_output.py
--rw-r--r--   0 runner    (1001) docker     (122)     5198 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/interface/dialog_weather.py
--rw-r--r--   0 runner    (1001) docker     (122)     4689 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/interface/dialog_workflow_dirs.py
--rw-r--r--   0 runner    (1001) docker     (122)    73823 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/interface/frame_main.py
--rw-r--r--   0 runner    (1001) docker     (122)     6429 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/interface/widget_dir_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     5595 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/interface/widget_file_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/interface/widget_group_list.py
--rw-r--r--   0 runner    (1001) docker     (122)      146 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/tk_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 21:22:00.714933 energyplus_launch-3.6.9/eplaunch/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10941 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/utilities/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/utilities/crossplatform.py
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/utilities/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 21:22:00.714933 energyplus_launch-3.6.9/eplaunch/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4817 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/workflows/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 21:22:00.714933 energyplus_launch-3.6.9/eplaunch/workflows/default/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/workflows/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/workflows/default/file_details.py
--rw-r--r--   0 runner    (1001) docker     (122)     3266 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/workflows/default/idf_details.py
--rw-r--r--   0 runner    (1001) docker     (122)     2163 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/workflows/default/site_location.py
--rw-r--r--   0 runner    (1001) docker     (122)    10553 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/workflows/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/workflows/workflow.py
--rw-r--r--   0 runner    (1001) docker     (122)     5368 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/workflows/workflow_tester.py
--rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/workflows/workflow_thread.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-06-02 21:22:00.714933 energyplus_launch-3.6.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1931 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:02:26.892974 energyplus_launch-3.7.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-06-06 15:02:26.892974 energyplus_launch-3.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:02:26.888975 energyplus_launch-3.7.0/energyplus_launch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-06-06 15:02:26.000000 energyplus_launch-3.7.0/energyplus_launch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1300 2023-06-06 15:02:26.000000 energyplus_launch-3.7.0/energyplus_launch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-06 15:02:26.000000 energyplus_launch-3.7.0/energyplus_launch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-06-06 15:02:26.000000 energyplus_launch-3.7.0/energyplus_launch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-06 15:02:26.000000 energyplus_launch-3.7.0/energyplus_launch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-06 15:02:26.000000 energyplus_launch-3.7.0/energyplus_launch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:02:26.888975 energyplus_launch-3.7.0/eplaunch/
+-rw-r--r--   0 runner    (1001) docker     (122)      389 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/configure.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:02:26.892974 energyplus_launch-3.7.0/eplaunch/interface/
+-rw-r--r--   0 runner    (1001) docker     (122)     1747 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9400 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/interface/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6211 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/interface/dialog_external_viewers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1518 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/interface/dialog_generic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2543 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/interface/dialog_output.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5319 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/interface/dialog_weather.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4810 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/interface/dialog_workflow_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    74924 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/interface/frame_main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6429 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/interface/widget_dir_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5595 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/interface/widget_file_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/interface/widget_group_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/tk_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:02:26.892974 energyplus_launch-3.7.0/eplaunch/utilities/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10941 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/utilities/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/utilities/crossplatform.py
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/utilities/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:02:26.892974 energyplus_launch-3.7.0/eplaunch/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4817 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/workflows/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:02:26.892974 energyplus_launch-3.7.0/eplaunch/workflows/default/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/workflows/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/workflows/default/file_details.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3266 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/workflows/default/idf_details.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2163 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/workflows/default/site_location.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10553 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/workflows/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/workflows/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5368 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/workflows/workflow_tester.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/workflows/workflow_thread.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-06-06 15:02:26.892974 energyplus_launch-3.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1931 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/setup.py
```

### Comparing `energyplus_launch-3.6.9/LICENSE` & `energyplus_launch-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.9/PKG-INFO` & `energyplus_launch-3.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyplus_launch
-Version: 3.6.9
+Version: 3.7.0
 Summary: Graphical Interface and Workflow Manager for EnergyPlus
 Home-page: https://github.com/NREL/EP-Launch
 Author: Jason Glazer and Edwin Lee for the United States Department of Energy
 License: ModifiedBSD
 Description: # EP-Launch3
         
         [![GitHub release](https://img.shields.io/github/release/nrel/ep-launch.svg?style=for-the-badge)](https://github.com/nrel/ep-launch/releases/latest)
```

### Comparing `energyplus_launch-3.6.9/README.md` & `energyplus_launch-3.7.0/README.md`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.9/energyplus_launch.egg-info/PKG-INFO` & `energyplus_launch-3.7.0/energyplus_launch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyplus-launch
-Version: 3.6.9
+Version: 3.7.0
 Summary: Graphical Interface and Workflow Manager for EnergyPlus
 Home-page: https://github.com/NREL/EP-Launch
 Author: Jason Glazer and Edwin Lee for the United States Department of Energy
 License: ModifiedBSD
 Description: # EP-Launch3
         
         [![GitHub release](https://img.shields.io/github/release/nrel/ep-launch.svg?style=for-the-badge)](https://github.com/nrel/ep-launch/releases/latest)
```

### Comparing `energyplus_launch-3.6.9/energyplus_launch.egg-info/SOURCES.txt` & `energyplus_launch-3.7.0/energyplus_launch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.9/eplaunch/interface/config.py` & `energyplus_launch-3.7.0/eplaunch/interface/config.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.9/eplaunch/interface/dialog_external_viewers.py` & `energyplus_launch-3.7.0/eplaunch/interface/dialog_external_viewers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from platform import system
 from tkinter import Tk, Toplevel, Label, Listbox, SINGLE, Variable, Entry, DISABLED, StringVar, Button, Frame, \
     filedialog, E, EW, W, LEFT, messagebox
 from typing import Dict, List, Optional
 from pathlib import Path
 
-from eplaunch.interface import set_dialog_geometry
+from eplaunch.interface import set_dialog_geometry, set_frame_or_top_level_icon
 
 
 class TkViewerDialog(Toplevel):
     CLOSE_SIGNAL_OK = 0
     CLOSE_SIGNAL_CANCEL = 1
 
     def __init__(self, parent_window, list_of_suffixes: List[str], dict_of_viewer_overrides: Dict[str, Optional[Path]]):
         super().__init__()
+        set_frame_or_top_level_icon(self, Path(__file__).resolve().parent.parent / 'icons')
         self.title("Viewers")
         self.exit_code = self.CLOSE_SIGNAL_CANCEL
         self.suffixes = ['txt'] + list_of_suffixes
         self.extension_to_viewer = dict_of_viewer_overrides
         self._define_tk_variables()
         self._build_gui()
         set_dialog_geometry(self, parent_window)
```

### Comparing `energyplus_launch-3.6.9/eplaunch/interface/dialog_output.py` & `energyplus_launch-3.7.0/eplaunch/interface/dialog_output.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+from pathlib import Path
 from tkinter import Tk, Toplevel, Frame, TOP, Button, scrolledtext, BOTH, Scrollbar, BOTTOM, X, END
 
+from eplaunch.interface import set_frame_or_top_level_icon
+
 
 class TkOutputDialog(Toplevel):
 
     def __init__(self, parent_window, workflow_id, workflow_title: str, configuration: str, x: int, y: int):
         super().__init__(parent_window)
+        set_frame_or_top_level_icon(self, Path(__file__).resolve().parent.parent / 'icons')
         self.x = x
         self.y = y
         self.desired_width = 500
         self.title(workflow_title)
         self.workflow_id = workflow_id
         self._build_gui(configuration)
```

### Comparing `energyplus_launch-3.6.9/eplaunch/interface/dialog_weather.py` & `energyplus_launch-3.7.0/eplaunch/interface/dialog_weather.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 if system() == 'Darwin':
     from tkmacosx import Button
 else:
     from tkinter.ttk import Button
 from tkinter.ttk import Separator
 from typing import List, Optional
 
-from eplaunch.interface import set_dialog_geometry
+from eplaunch.interface import set_dialog_geometry, set_frame_or_top_level_icon
 
 
 class TkWeatherDialog(Toplevel):
     CLOSE_SIGNAL_OK = 0
     CLOSE_SIGNAL_CANCEL = 1
     WEATHER_TYPE_DD = "DD"
     WEATHER_TYPE_EPW = "EPW"
 
     def __init__(self, parent_window, recent_files: List[Path], text: Optional[str] = None):
         super().__init__()
+        set_frame_or_top_level_icon(self, Path(__file__).resolve().parent.parent / 'icons')
         self.alt_text = text
         self.title("Choose Weather Configuration")
         # assume cancel to allow for closing the dialog with the X
         self.exit_code = self.CLOSE_SIGNAL_CANCEL
         self.selected_weather_file: Optional[Path] = None
         self._epw_from_select = None
         # build the gui and call required modal methods
```

### Comparing `energyplus_launch-3.6.9/eplaunch/interface/dialog_workflow_dirs.py` & `energyplus_launch-3.7.0/eplaunch/interface/dialog_workflow_dirs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from pathlib import Path
 from tkinter import Tk, Toplevel, Frame, Button, EW, NSEW, Listbox, Variable, SINGLE, Scrollbar, LEFT, BOTH, RIGHT, ALL
 from tkinter.filedialog import askdirectory
 from tkinter.messagebox import showerror
 from typing import List
 
-from eplaunch.interface import set_dialog_geometry
+from eplaunch.interface import set_dialog_geometry, set_frame_or_top_level_icon
 
 
 class TkWorkflowsDialog(Toplevel):
     CLOSE_SIGNAL_OK = 0
     CLOSE_SIGNAL_CANCEL = 1
 
     def __init__(self, parent_window, current_workflow_dirs: List[Path], auto_found_workflow_dirs: List[Path]):
         super().__init__()
+        set_frame_or_top_level_icon(self, Path(__file__).resolve().parent.parent / 'icons')
         self.title("Choose Workflow Directories")
         # assume cancel to allow for closing the dialog with the X
         self.exit_code = self.CLOSE_SIGNAL_CANCEL
         self.list_of_directories: List[Path] = []
         self._auto_find_dirs = auto_found_workflow_dirs
         self._tk_var_all_directories = Variable(value=current_workflow_dirs)
         self.selected_index = -1
```

### Comparing `energyplus_launch-3.6.9/eplaunch/interface/frame_main.py` & `energyplus_launch-3.7.0/eplaunch/interface/frame_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,14 +196,16 @@
         menu_nav.add_cascade(label="Recent", menu=self.menu_nav_recent)
         menu_nav.add_command(label="Navigate to previous folder", command=self._navigate_to_previous_folder)
         menu_nav.add_separator()
         self.menu_nav_favorites = Menu(menu_nav, tearoff=False)
         menu_nav.add_cascade(label="Favorites", menu=self.menu_nav_favorites)
         menu_nav.add_command(label="Add Current Folder to Favorites", command=self._add_folder_to_favorites)
         menu_nav.add_command(label="Remove Current Folder from Favorites", command=self._remove_folder_from_favorites)
+        menu_nav.add_separator()
+        menu_nav.add_command(label="View Keyboard Shortcuts", command=self._open_shortcuts_dialog)
         menubar.add_cascade(label="Navigation", menu=menu_nav)
 
         menu_group = Menu(menubar, tearoff=False)
         menu_group.add_command(label="Clear Current Group", command=self._clear_group)
         menu_group.add_command(label="Load new Group file...", command=self._load_new_group_file)
         menu_group.add_command(label="Save Current Group to file...", command=self._save_group_file)
         menu_group.add_command(
@@ -441,14 +443,15 @@
             self._tk_var_status_workflow.set(self.workflow_manager.current_workflow.description)
         else:
             self._tk_var_status_workflow.set('<No Workflow>')
         self._tk_var_status_message.set(message)
 
     def _handle_keyboard_press(self, event) -> None:
         # Update docs/navigation.rst whenever this set of keybindings changes
+        # Update self._list_keyboard_shortcuts() whenever this set of keybindings changes
         # relevant_modifiers
         # mod_shift = 0x1
         mod_control = 0x4
         # mod_alt = 0x20000
         if event.keysym == 'F5':
             self._update_file_list()
         elif event.keysym == 'w' and mod_control & event.state:
@@ -458,14 +461,27 @@
         elif event.keysym == 'g' and mod_control & event.state:
             self._run_workflow_on_group()
         elif event.keysym == 'm' and mod_control & event.state:
             self._cycle_through_group()
         elif event.keysym == 'z' and mod_control & event.state:
             self._navigate_to_previous_folder()
 
+    @staticmethod
+    def _list_keyboard_shortcuts() -> List[Tuple[str, str]]:
+        # Mimic the keyboard shortcuts in the function above
+        # It helps the dialog text look nice if you make sure the widths are uniform
+        return [
+            ("Control + F5", "Update File List"),
+            ("Control + w ", "Open Weather Dialog"),
+            ("Control + r ", "Run Workflow on Selected Files"),
+            ("Control + g ", "Run Workflow on Current Group"),
+            ("Control + m ", "Cycle Through Group Files"),
+            ("Control + z ", "Navigate to Previous Folder"),
+        ]
+
     # endregion
 
     # region group operations
 
     def _clear_group(self):
         self.conf.group_locations.clear()
         self._rebuild_group_menu()
@@ -1224,20 +1240,25 @@
         if self.conf.welcome_shown and VERSION == self.conf.latest_welcome_shown:
             return
         message = """
 EP-Launch has been around for many years as a part of the EnergyPlus distribution.
 Starting with the 3.0 release, it has changed drastically, completely redesigned and rewritten.
 For full documentation or a quick start guide, click the "Open Docs" button below.
 This dialog will only be shown once, but documentation is available in the Help menu."""
-        self.generic_dialogs.display(
+        self.generic_dialogs.display_with_alt_button(
             self, 'Welcome to EP-Launch ' + VERSION, message, 'Open Documentation', self._open_documentation
         )
         self.conf.welcome_shown = True
         self.conf.latest_welcome_shown = VERSION
 
+    def _open_shortcuts_dialog(self, *_) -> None:
+        shortcuts = EPLaunchWindow._list_keyboard_shortcuts()
+        text = '\n'.join([f"{r[0]}:\t{r[1]}" for r in shortcuts])
+        self.generic_dialogs.display(self, "Available Keyboard Shortcuts", text)
+
     def _open_about(self) -> None:
         text = """
 EP-Launch
 
 EP-Launch is a graphical workflow manager for EnergyPlus.
 Originally written in VB6 and released with essentially every version of EnergyPlus,
 it is now a cross platform Python tool.
```

### Comparing `energyplus_launch-3.6.9/eplaunch/interface/widget_dir_list.py` & `energyplus_launch-3.7.0/eplaunch/interface/widget_dir_list.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.9/eplaunch/interface/widget_file_list.py` & `energyplus_launch-3.7.0/eplaunch/interface/widget_file_list.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.9/eplaunch/interface/widget_group_list.py` & `energyplus_launch-3.7.0/eplaunch/interface/widget_group_list.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.9/eplaunch/utilities/cache.py` & `energyplus_launch-3.7.0/eplaunch/utilities/cache.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.9/eplaunch/utilities/crossplatform.py` & `energyplus_launch-3.7.0/eplaunch/utilities/crossplatform.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.9/eplaunch/utilities/version.py` & `energyplus_launch-3.7.0/eplaunch/utilities/version.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.9/eplaunch/workflows/base.py` & `energyplus_launch-3.7.0/eplaunch/workflows/base.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.9/eplaunch/workflows/default/file_details.py` & `energyplus_launch-3.7.0/eplaunch/workflows/default/file_details.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.9/eplaunch/workflows/default/idf_details.py` & `energyplus_launch-3.7.0/eplaunch/workflows/default/idf_details.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.9/eplaunch/workflows/default/site_location.py` & `energyplus_launch-3.7.0/eplaunch/workflows/default/site_location.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.9/eplaunch/workflows/manager.py` & `energyplus_launch-3.7.0/eplaunch/workflows/manager.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.9/eplaunch/workflows/workflow.py` & `energyplus_launch-3.7.0/eplaunch/workflows/workflow.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.9/eplaunch/workflows/workflow_tester.py` & `energyplus_launch-3.7.0/eplaunch/workflows/workflow_tester.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.9/eplaunch/workflows/workflow_thread.py` & `energyplus_launch-3.7.0/eplaunch/workflows/workflow_thread.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.9/setup.py` & `energyplus_launch-3.7.0/setup.py`

 * *Files identical despite different names*

