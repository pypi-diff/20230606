# Comparing `tmp/vstt-0.27.0.tar.gz` & `tmp/vstt-0.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vstt-0.27.0.tar", last modified: Fri Jun  2 12:47:36 2023, max compression
+gzip compressed data, was "vstt-0.28.0.tar", last modified: Tue Jun  6 13:38:55 2023, max compression
```

## Comparing `vstt-0.27.0.tar` & `vstt-0.28.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:47:36.739976 vstt-0.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-02 12:47:25.000000 vstt-0.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-02 12:47:36.739976 vstt-0.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-02 12:47:25.000000 vstt-0.27.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-02 12:47:25.000000 vstt-0.27.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 12:47:36.739976 vstt-0.27.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:47:36.735976 vstt-0.27.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:47:36.735976 vstt-0.27.0/src/vstt/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/display_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)    11314 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/joystick_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/meta_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/results_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/stat.py
--rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/trials_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/update.py
--rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:47:36.739976 vstt-0.27.0/src/vstt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-02 12:47:36.000000 vstt-0.27.0/src/vstt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-02 12:47:36.000000 vstt-0.27.0/src/vstt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 12:47:36.000000 vstt-0.27.0/src/vstt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-02 12:47:36.000000 vstt-0.27.0/src/vstt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-02 12:47:36.000000 vstt-0.27.0/src/vstt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-02 12:47:36.000000 vstt-0.27.0/src/vstt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:47:36.739976 vstt-0.27.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_display_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    13893 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_joystick_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_meta_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_results_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_trials_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    12342 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_vis.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_vstt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:38:55.980248 vstt-0.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-06 13:38:44.000000 vstt-0.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-06 13:38:55.980248 vstt-0.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-06 13:38:44.000000 vstt-0.28.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-06 13:38:44.000000 vstt-0.28.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 13:38:55.980248 vstt-0.28.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:38:55.976248 vstt-0.28.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:38:55.976248 vstt-0.28.0/src/vstt/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/display_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/joystick_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/meta_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/results_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14462 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15068 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/trials_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:38:55.980248 vstt-0.28.0/src/vstt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-06 13:38:55.000000 vstt-0.28.0/src/vstt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-06 13:38:55.000000 vstt-0.28.0/src/vstt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 13:38:55.000000 vstt-0.28.0/src/vstt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-06 13:38:55.000000 vstt-0.28.0/src/vstt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-06 13:38:55.000000 vstt-0.28.0/src/vstt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 13:38:55.000000 vstt-0.28.0/src/vstt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:38:55.980248 vstt-0.28.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_display_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13685 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_joystick_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_meta_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_results_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_trials_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12342 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_vis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_vstt.py
```

### Comparing `vstt-0.27.0/LICENSE` & `vstt-0.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vstt-0.27.0/PKG-INFO` & `vstt-0.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstt
-Version: 0.27.0
+Version: 0.28.0
 Summary: Visuomotor Serial Targeting Task (VSTT)
 Author-email: Liam Keegan <ssc@iwr.uni-heidelberg.de>
 License: MIT
 Project-URL: Github, https://github.com/ssciwr/vstt
 Project-URL: Issues, https://github.com/ssciwr/vstt/issues
 Project-URL: Documentation, https://vstt.readthedocs.io/
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `vstt-0.27.0/README.md` & `vstt-0.28.0/README.md`

 * *Files identical despite different names*

### Comparing `vstt-0.27.0/pyproject.toml` & `vstt-0.28.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vstt-0.27.0/src/vstt/__main__.py` & `vstt-0.28.0/src/vstt/__main__.py`

 * *Files identical despite different names*

### Comparing `vstt-0.27.0/src/vstt/common.py` & `vstt-0.28.0/src/vstt/common.py`

 * *Files identical despite different names*

### Comparing `vstt-0.27.0/src/vstt/display.py` & `vstt-0.28.0/src/vstt/display.py`

 * *Files identical despite different names*

### Comparing `vstt-0.27.0/src/vstt/display_widget.py` & `vstt-0.28.0/src/vstt/display_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.27.0/src/vstt/experiment.py` & `vstt-0.28.0/src/vstt/experiment.py`

 * *Files identical despite different names*

### Comparing `vstt-0.27.0/src/vstt/geom.py` & `vstt-0.28.0/src/vstt/geom.py`

 * *Files identical despite different names*

### Comparing `vstt-0.27.0/src/vstt/gui.py` & `vstt-0.28.0/src/vstt/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,14 +76,15 @@
             self.reload_experiment()
 
     def _open_file(self, filename: str) -> None:
         try:
             self.experiment.load_file(filename)
         except Exception as e:
             logging.warning(f"Failed to load file {filename}: {e}")
+            logging.exception(e)
             QtWidgets.QMessageBox.critical(
                 self,
                 "Invalid file",
                 f"Could not read file '{filename}'",
             )
         self.reload_experiment()
```

### Comparing `vstt-0.27.0/src/vstt/joystick_wrapper.py` & `vstt-0.28.0/src/vstt/joystick_wrapper.py`

 * *Files identical despite different names*

### Comparing `vstt-0.27.0/src/vstt/meta.py` & `vstt-0.28.0/src/vstt/meta.py`

 * *Files identical despite different names*

### Comparing `vstt-0.27.0/src/vstt/meta_widget.py` & `vstt-0.28.0/src/vstt/meta_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.27.0/src/vstt/results_widget.py` & `vstt-0.28.0/src/vstt/results_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.27.0/src/vstt/stat.py` & `vstt-0.28.0/src/vstt/stat.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from __future__ import annotations
 
+import logging
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 import pandas as pd
 from psychopy.data import TrialHandlerExt
@@ -34,62 +36,88 @@
         "i_target",
         "condition_index",
         "target_index",
         "target_pos",
         "to_target_timestamps",
         "to_target_mouse_positions",
         "to_target_success",
+        "to_target_num_timestamps_before_visible",
         "center_pos",
         "to_center_timestamps",
         "to_center_mouse_positions",
         "to_center_success",
+        "to_center_num_timestamps_before_visible",
     ]
 
 
+def _get_dat(
+    data: Dict, key: str, index: Tuple, i_target: int, default_value: Any
+) -> Any:
+    ar = data.get(key)
+    if ar is None:
+        logging.warning(
+            f"Key '{key}' not found in data, using default value {default_value}"
+        )
+        return default_value
+    try:
+        return ar[index][i_target]
+    except IndexError:
+        logging.warning(
+            f"Index error for key '{key}', index '{index}', i_target '{i_target}', using default value {default_value}"
+        )
+    return default_value
+
+
 def _get_target_data(
     trial_handler: TrialHandlerExt, index: Tuple, i_target: int
 ) -> List:
     data = trial_handler.data
     condition_index = trial_handler.sequenceIndices[index]
     target_index = data["target_indices"][index][i_target]
     target_pos = np.array(data["target_pos"][index][i_target])
     center_pos = np.array([0.0, 0.0])
     to_target_timestamps = np.array(data["to_target_timestamps"][index][i_target])
+    to_target_num_timestamps_before_visible = _get_dat(
+        data, "to_target_num_timestamps_before_visible", index, i_target, 0
+    )
     to_target_mouse_positions = np.stack(
         np.array(data["to_target_mouse_positions"][index][i_target])
     )  # type: ignore
     to_target_success = np.array(data["to_target_success"][index][i_target])
     to_center_success: Union[np.ndarray, bool]
-    if (
-        type(data["to_center_timestamps"][index]) is np.ndarray
-        and i_target < data["to_center_timestamps"][index].shape[0]
-    ):
-        to_center_timestamps = np.array(data["to_center_timestamps"][index][i_target])
-        to_center_mouse_positions = np.stack(
-            np.array(data["to_center_mouse_positions"][index][i_target])
-        )  # type: ignore
-        to_center_success = np.array(data["to_center_success"][index][i_target])
-    else:
-        to_center_timestamps = np.array([])
-        to_center_mouse_positions = np.array([])
-        to_center_success = True
+    to_center_timestamps = np.array(
+        _get_dat(data, "to_center_timestamps", index, i_target, [])
+    )
+    to_center_num_timestamps_before_visible = _get_dat(
+        data, "to_center_num_timestamps_before_visible", index, i_target, 0
+    )
+    to_center_mouse_positions = np.array(
+        _get_dat(data, "to_center_mouse_positions", index, i_target, [])
+    )
+    if to_center_mouse_positions.shape[0] > 0:
+        to_center_mouse_positions = np.stack(to_center_mouse_positions)  # type: ignore
+    to_center_success = np.array(
+        _get_dat(data, "to_center_success", index, i_target, True)
+    )
     return [
         index[0],
         index[1],
         i_target,
         condition_index,
         target_index,
         target_pos,
         to_target_timestamps,
         to_target_mouse_positions,
         to_target_success,
+        to_target_num_timestamps_before_visible,
         center_pos,
         to_center_timestamps,
         to_center_mouse_positions,
         to_center_success,
+        to_center_num_timestamps_before_visible,
     ]
 
 
 def _data_df(trial_handler: TrialHandlerExt) -> pd.DataFrame:
     data = []
     for index in np.ndindex(trial_handler.sequenceIndices.shape):
         # trials that have not yet happened have a default string instead of an array in their data
@@ -106,19 +134,24 @@
         df[f"to_{destination}_distance"] = df[f"to_{destination}_mouse_positions"].map(
             _distance
         )
         df[f"to_{destination}_reaction_time"] = df.apply(
             lambda x: _reaction_time(
                 x[f"to_{destination}_timestamps"],
                 x[f"to_{destination}_mouse_positions"],
+                x[f"to_{destination}_num_timestamps_before_visible"],
             ),
             axis=1,
         )
-        df[f"to_{destination}_time"] = df[f"to_{destination}_timestamps"].map(
-            lambda x: x[-1] if x.shape[0] > 0 else np.nan
+        df[f"to_{destination}_time"] = df.apply(
+            lambda x: _total_time(
+                x[f"to_{destination}_timestamps"],
+                x[f"to_{destination}_num_timestamps_before_visible"],
+            ),
+            axis=1,
         )
         df[f"to_{destination}_movement_time"] = (
             df[f"to_{destination}_time"] - df[f"to_{destination}_reaction_time"]
         )
         df[f"to_{destination}_rmse"] = df.apply(
             lambda x: _rmse(
                 x[f"to_{destination}_mouse_positions"], x[f"{destination}_pos"]
@@ -152,16 +185,16 @@
         df_stats = df_stats.drop(columns=[label])
     df_stats.to_excel(writer, sheet_name="statistics", index=False)
     # add timestamp/mouse position arrays
     if data_format == "target":
         # one sheet for each row (target) in df, with arrays of time/position data.
         # arrays transposed to columns, x-y pairs are split into two columns.
         # 6 columns:
-        #   - to_target_timestamps (negative until target displayed)
-        #   - to_center_timestamps (negative until target displayed)
+        #   - to_target_timestamps
+        #   - to_center_timestamps
         #   - to_target_mouse_positions_x
         #   - to_target_mouse_positions_y
         #   - to_center_mouse_positions_x
         #   - to_center_mouse_positions_y
         for row in df.itertuples():
             df_data = pd.concat(
                 [
@@ -185,53 +218,55 @@
             df_data.to_excel(writer, sheet_name=f"{row.Index}", index=False)
     else:
         # one sheet per trial: all targets for a trial are concatenated
         # 6 columns:
         #   - timestamps (start from zero, increases throughout the trial)
         #   - mouse_x
         #   - mouse_y
-        #   - target_index (-1 if no target is currently displayed)
-        #   - target_x (-1 if no target is currently displayed)
-        #   - target_y (-1 if no target is currently displayed)
+        #   - target_index (-99 if no target is currently displayed)
+        #   - target_x (-99 if no target is currently displayed)
+        #   - target_y (-99 if no target is currently displayed)
         for i_trial in df.i_trial.unique():
-            t0 = 0.0
             times = np.array([])
             x_positions = np.array([])
             y_positions = np.array([])
             i_targets = np.array([], dtype=np.int64)
             x_targets = np.array([])
             y_targets = np.array([])
             for row in df.loc[df.i_trial == i_trial].itertuples():
                 for dest in ["target", "center"]:
                     raw_times = getattr(row, f"to_{dest}_timestamps")
                     if raw_times.shape[-1] > 0:
-                        times = np.append(times, raw_times - raw_times[0] + t0)
+                        times = np.append(times, raw_times)
                         points = getattr(row, f"to_{dest}_mouse_positions")
                         x_positions = np.append(x_positions, points[:, 0])
                         y_positions = np.append(y_positions, points[:, 1])
                         # set target info for all timestamps
                         if dest == "center":
                             pos = (0.0, 0.0)
                             i_target = -1  # give center target the special index -1
+                            num_timestamps_before_target_visible = (
+                                row.to_center_num_timestamps_before_visible
+                            )
                         else:
                             pos = row.target_pos
                             i_target = row.i_target
+                            num_timestamps_before_target_visible = (
+                                row.to_target_num_timestamps_before_visible
+                            )
                         target_i = np.full_like(raw_times, i_target, dtype=np.int64)
                         target_x = np.full_like(raw_times, pos[0])
                         target_y = np.full_like(raw_times, pos[1])
-                        # set these to -99 if no target is visible (i.e. raw time is negative)
-                        target_i[raw_times < 0] = -99
-                        target_x[raw_times < 0] = -99
-                        target_y[raw_times < 0] = -99
+                        # if no target is visible use the special index -99
+                        target_i[0:num_timestamps_before_target_visible] = -99
+                        target_x[0:num_timestamps_before_target_visible] = -99
+                        target_y[0:num_timestamps_before_target_visible] = -99
                         i_targets = np.append(i_targets, target_i)
                         x_targets = np.append(x_targets, target_x)
                         y_targets = np.append(y_targets, target_y)
-                        t0 = (
-                            times[-1] + 1.0 / 60.0
-                        )  # add a single window flip between targets (?)
             df_data = pd.DataFrame(
                 {
                     "timestamps": times,
                     "mouse_positions_x": x_positions,
                     "mouse_positions_y": y_positions,
                     "i_target": i_targets,
                     "target_x": x_targets,
@@ -240,38 +275,91 @@
             )
             df_data.to_excel(writer, sheet_name=f"{i_trial}", index=False)
 
 
 def _reaction_time(
     mouse_times: np.ndarray,
     mouse_positions: np.ndarray,
+    to_target_num_timestamps_before_visible: int,
     epsilon: float = 1e-12,
 ) -> float:
-    if mouse_times.shape[0] != mouse_positions.shape[0] or mouse_times.shape[0] == 0:
+    """
+    The reaction time is defined as the timestamp where the cursor first moves,
+    minus the timestamp where the target becomes visible.
+    This means the reaction time can be negative if the cursor is moved before
+    the target is made visible.
+
+    :param mouse_times: The array of timestamps
+    :param mouse_positions: The array of mouse positions
+    :param to_target_num_timestamps_before_visible: The index of the first timestamp where the target is visible
+    :param epsilon: The minimum euclidean distance to qualify as moving the cursor
+    :return: The reaction time
+    """
+    if (
+        mouse_times.shape[0] != mouse_positions.shape[0]
+        or mouse_times.shape[0] == 0
+        or mouse_times.shape[0] < to_target_num_timestamps_before_visible
+    ):
         return np.nan
     i = 0
     while xydist(mouse_positions[0], mouse_positions[i]) < epsilon and i + 1 < len(
         mouse_times
     ):
         i += 1
-    return mouse_times[i]
+    return mouse_times[i] - mouse_times[to_target_num_timestamps_before_visible]
+
+
+def _total_time(
+    mouse_times: np.ndarray,
+    to_target_num_timestamps_before_visible: int,
+) -> float:
+    """
+    The time to target is defined as the final timestamp (corresponding either to the target being reached
+    or a timeout) minus the timestamp where the target becomes visible.
+
+    :param mouse_times: The array of timestamps
+    :param to_target_num_timestamps_before_visible: The index of the first timestamp where the target is visible
+    :return: The total time to target
+    """
+    if (
+        mouse_times.shape[0] == 0
+        or mouse_times.shape[0] < to_target_num_timestamps_before_visible
+    ):
+        return np.nan
+    return mouse_times[-1] - mouse_times[to_target_num_timestamps_before_visible]
 
 
 def _distance(mouse_positions: np.ndarray) -> float:
+    """
+    The euclidean point-to-point distance travelled by the cursor.
+
+    :param mouse_positions: The array of mouse positions
+    :return: The distance travelled.
+    """
     dist = 0
     for i in range(mouse_positions.shape[0] - 1):
         dist += xydist(mouse_positions[i + 1], mouse_positions[i])
     return dist
 
 
-def _rmse(mouse_positions: np.ndarray, target: np.ndarray) -> float:
+def _rmse(mouse_positions: np.ndarray, target_position: np.ndarray) -> float:
+    """
+    The Root Mean Square Error (RMSE) of the perpendicular distance from each mouse point
+    to the straight line that intersects the initial mouse location and the target.
+
+    See: https://en.wikipedia.org/wiki/Distance_from_a_point_to_a_line#Line_defined_by_two_points.
+
+    :param mouse_positions: The array of mouse positions
+    :param target: The x,y coordinates of the target
+    :return: The RMSE of the distance from the ideal trajectoty
+    """
     if mouse_positions.shape[0] <= 1:
         return np.nan
     # use first mouse position as origin point, so exclude it from RMSE measure
     x1, y1 = mouse_positions[0]
-    x2, y2 = target
+    x2, y2 = target_position
     norm = np.power(x2 - x1, 2) + np.power(y2 - y1, 2)
     norm *= mouse_positions.shape[0] - 1
     sum_of_squares = 0
     for x0, y0 in mouse_positions[1:]:
         sum_of_squares += np.power((x2 - x1) * (y1 - y0) - (x1 - x0) * (y2 - y1), 2)
     return np.sqrt(sum_of_squares / norm)
```

### Comparing `vstt-0.27.0/src/vstt/task.py` & `vstt-0.28.0/src/vstt/task.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,15 +43,17 @@
         self.target_indices = np.fromstring(
             trial["target_indices"], dtype="int", sep=" "
         )
         if trial["target_order"] == "random":
             rng.shuffle(self.target_indices)
         self.target_pos: List[np.ndarray] = []
         self.to_target_timestamps: List[np.ndarray] = []
+        self.to_target_num_timestamps_before_visible: List[int] = []
         self.to_center_timestamps: List[np.ndarray] = []
+        self.to_center_num_timestamps_before_visible: List[int] = []
         self.to_target_mouse_positions: List[np.ndarray] = []
         self.to_center_mouse_positions: List[np.ndarray] = []
         self.to_target_success: List[bool] = []
         self.to_center_success: List[bool] = []
 
 
 class TrialManager:
@@ -87,14 +89,15 @@
         )
         self.cursor_path = ShapeStim(
             win, vertices=[(0, 0)], lineColor="white", closeShape=False
         )
         self.prev_cursor_path = ShapeStim(
             win, vertices=[(0, 0)], lineColor="white", closeShape=False
         )
+        self.clock = Clock()
         if trial["show_cursor_path"]:
             self.drawables.append(self.cursor_path)
             self.drawables.append(self.prev_cursor_path)
 
 
 def _contains_mixed_length_numpy_arrays(items: Iterable) -> bool:
     return (
@@ -175,19 +178,19 @@
             self.trial_handler.thisTrialN
         )
         is_final_trial_of_block = (
             len(condition_trial_indices[self.trial_handler.thisIndex])
             == trial["weight"]
         )
         self.mouse.setPos(tom.cursor.pos)
-        previous_target_time_taken = 0.0
+        self.win.recordFrameIntervals = True
+        tom.clock.reset()
         for index in tom.data.target_indices:
-            previous_target_time_taken = self._do_target(
-                trial, index, tom, previous_target_time_taken
-            )
+            self._do_target(trial, index, tom)
+        self.win.recordFrameIntervals = False
 
         if trial["automove_cursor_to_center"]:
             tom.data.to_center_success = [True] * trial["num_targets"]
         add_trial_data_to_trial_handler(tom.data, self.trial_handler)
         if trial["post_trial_delay"] > 0:
             vis.display_results(
                 trial["post_trial_delay"],
@@ -207,133 +210,136 @@
                 self.trial_handler if trial["post_block_display_results"] else None,
                 self.experiment.display_options,
                 self.trial_handler.thisTrialN,
                 True,
                 self.win,
             )
 
-    def _do_target(
-        self,
-        trial: Dict[str, Any],
-        index: int,
-        tm: TrialManager,
-        previous_target_time_taken: float,
-    ) -> float:
-        clock = Clock()
+    def _do_target(self, trial: Dict[str, Any], index: int, tm: TrialManager) -> None:
+        minimum_window_for_flip = 1.0 / 60.0
         mouse_pos = tm.cursor.pos
-        current_target_time_taken = 0
+        stop_waiting_time = 0.0
+        stop_target_time = 0.0
+        if trial["fixed_target_intervals"]:
+            num_completed_targets = len(tm.data.to_target_timestamps)
+            stop_waiting_time = (num_completed_targets + 1) * trial["target_duration"]
+            stop_target_time = stop_waiting_time + trial["target_duration"]
         for target_index in _get_target_indices(index, trial):
-            # no target displayed
-            vis.update_target_colors(tm.targets, trial["show_inactive_targets"], None)
-            if trial["show_target_labels"]:
-                vis.update_target_label_colors(
-                    tm.target_labels, trial["show_inactive_targets"], None
-                )
+            t0 = tm.clock.getTime()
+            is_central_target = target_index == trial["num_targets"]
             mouse_times = []
             mouse_positions = []
-            is_central_target = target_index == trial["num_targets"]
             if is_central_target:
-                mouse_times = [0]
-                mouse_positions = [tm.cursor_path.vertices[-1]]
                 tm.prev_cursor_path.vertices = tm.cursor_path.vertices
-                tm.cursor_path.vertices = mouse_positions
+                tm.cursor_path.vertices = [tm.cursor_path.vertices[-1]]
             else:
                 if trial["automove_cursor_to_center"]:
                     mouse_pos = np.array([0.0, 0.0])
                     self.mouse.setPos(mouse_pos)
                     tm.cursor.setPos(mouse_pos)
                 tm.cursor_path.vertices = [mouse_pos]
                 tm.prev_cursor_path.vertices = [(0, 0)]
-                clock.reset()
-                wait_time = trial["inter_target_duration"]
-                if trial["fixed_target_intervals"]:
-                    wait_time = trial["target_duration"] - previous_target_time_taken
-                while clock.getTime() < wait_time:
-                    if trial["freeze_cursor_between_targets"]:
-                        self.mouse.setPos(mouse_pos)
-                    else:
-                        if trial["use_joystick"]:
-                            mouse_pos = tm.joystick_point_updater(
-                                mouse_pos, (self.js.getX(), self.js.getY())  # type: ignore
-                            )
-                        else:
-                            mouse_pos = tm.point_rotator(self.mouse.getPos())
-                    mouse_times.append(clock.getTime() - wait_time)
-                    mouse_positions.append(mouse_pos)
-                    if trial["show_cursor"]:
-                        tm.cursor.setPos(mouse_pos)
-                    if trial["show_cursor_path"]:
-                        tm.cursor_path.vertices = mouse_positions
-                    vis.draw_and_flip(self.win, tm.drawables, self.kb)
+                if not trial["fixed_target_intervals"]:
+                    stop_waiting_time = t0 + trial["inter_target_duration"]
+                if stop_waiting_time > t0:
+                    # no target displayed
+                    vis.update_target_colors(
+                        tm.targets, trial["show_inactive_targets"], None
+                    )
+                    if trial["show_target_labels"]:
+                        vis.update_target_label_colors(
+                            tm.target_labels, trial["show_inactive_targets"], None
+                        )
+                    # ensure we get at least a single flip
+                    should_continue_waiting = True
+                    while should_continue_waiting:
+                        if trial["freeze_cursor_between_targets"]:
+                            self.mouse.setPos(mouse_pos)
+                        vis.draw_and_flip(self.win, tm.drawables, self.kb)
+                        if not trial["freeze_cursor_between_targets"]:
+                            if trial["use_joystick"]:
+                                mouse_pos = tm.joystick_point_updater(
+                                    mouse_pos, (self.js.getX(), self.js.getY())  # type: ignore
+                                )
+                            else:
+                                mouse_pos = tm.point_rotator(self.mouse.getPos())
+                        mouse_times.append(tm.clock.getTime())
+                        mouse_positions.append(mouse_pos)
+                        if trial["show_cursor"]:
+                            tm.cursor.setPos(mouse_pos)
+                        if trial["show_cursor_path"]:
+                            tm.cursor_path.vertices = mouse_positions
+                        should_continue_waiting = (
+                            tm.clock.getTime() + minimum_window_for_flip
+                            < stop_waiting_time
+                        )
             # display current target
+            t0 = tm.clock.getTime()
             vis.update_target_colors(
                 tm.targets, trial["show_inactive_targets"], target_index
             )
             if trial["show_target_labels"]:
                 vis.update_target_label_colors(
                     tm.target_labels, trial["show_inactive_targets"], target_index
                 )
             if trial["play_sound"]:
                 Sound("A", secs=0.3, blockSize=1024, stereo=True).play()
-            if not is_central_target:
-                tm.data.target_pos.append(tm.targets.xys[target_index])
-            dist_correct, dist_any = to_target_dists(
-                mouse_pos,
-                tm.targets.xys,
-                target_index,
-                trial["add_central_target"],
-            )
-            if trial["ignore_incorrect_targets"] or is_central_target:
-                dist = dist_correct
+            if is_central_target:
+                tm.data.to_center_num_timestamps_before_visible.append(len(mouse_times))
             else:
-                dist = dist_any
-            clock.reset()
-            self.win.recordFrameIntervals = True
+                tm.data.target_pos.append(tm.targets.xys[target_index])
+                tm.data.to_target_num_timestamps_before_visible.append(len(mouse_times))
             target_size = trial["target_size"]
             if is_central_target:
                 target_size = trial["central_target_size"]
-            max_time = trial["target_duration"]
-            if trial["fixed_target_intervals"]:
-                max_time -= current_target_time_taken
-            while dist > target_size and clock.getTime() < max_time:
+            if not trial["fixed_target_intervals"]:
+                stop_target_time = t0 + trial["target_duration"]
+            dist_correct = 1.0
+            # ensure we get at least one flip
+            should_continue_target = True
+            while should_continue_target:
+                vis.draw_and_flip(self.win, tm.drawables, self.kb)
                 if trial["use_joystick"]:
                     mouse_pos = tm.joystick_point_updater(
                         mouse_pos, (self.js.getX(), self.js.getY())  # type: ignore
                     )
                 else:
                     mouse_pos = tm.point_rotator(self.mouse.getPos())
                 if trial["show_cursor"]:
                     tm.cursor.setPos(mouse_pos)
-                mouse_times.append(clock.getTime())
+                mouse_times.append(tm.clock.getTime())
                 mouse_positions.append(mouse_pos)
                 if trial["show_cursor_path"]:
                     tm.cursor_path.vertices = mouse_positions
                 dist_correct, dist_any = to_target_dists(
                     mouse_pos,
                     tm.targets.xys,
                     target_index,
                     trial["add_central_target"],
                 )
                 if trial["ignore_incorrect_targets"] or is_central_target:
                     dist = dist_correct
                 else:
                     dist = dist_any
-                vis.draw_and_flip(self.win, tm.drawables, self.kb)
-            current_target_time_taken += clock.getTime()
-            self.win.recordFrameIntervals = False
-            success = dist_correct <= target_size and clock.getTime() < max_time
+                should_continue_target = (
+                    dist > target_size
+                    and tm.clock.getTime() + minimum_window_for_flip < stop_target_time
+                )
+            success = (
+                dist_correct <= target_size
+                and tm.clock.getTime() + minimum_window_for_flip < stop_target_time
+            )
             if is_central_target:
                 tm.data.to_center_success.append(success)
             else:
                 tm.data.to_target_success.append(success)
             if is_central_target:
                 tm.data.to_center_timestamps.append(np.array(mouse_times))
                 tm.data.to_center_mouse_positions.append(np.array(mouse_positions))
             else:
                 tm.data.to_target_timestamps.append(np.array(mouse_times))
                 tm.data.to_target_mouse_positions.append(np.array(mouse_positions))
-        return current_target_time_taken
 
     def _clean_up_and_return(self, return_value: bool) -> bool:
         if self.win is not None and self.close_window_when_done:
             self.win.close()
         return return_value
```

### Comparing `vstt-0.27.0/src/vstt/trial.py` & `vstt-0.28.0/src/vstt/trial.py`

 * *Files identical despite different names*

### Comparing `vstt-0.27.0/src/vstt/trials_widget.py` & `vstt-0.28.0/src/vstt/trials_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.27.0/src/vstt/types.py` & `vstt-0.28.0/src/vstt/types.py`

 * *Files identical despite different names*

### Comparing `vstt-0.27.0/src/vstt/update.py` & `vstt-0.28.0/src/vstt/update.py`

 * *Files identical despite different names*

### Comparing `vstt-0.27.0/src/vstt/vis.py` & `vstt-0.28.0/src/vstt/vis.py`

 * *Files identical despite different names*

### Comparing `vstt-0.27.0/src/vstt.egg-info/PKG-INFO` & `vstt-0.28.0/src/vstt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstt
-Version: 0.27.0
+Version: 0.28.0
 Summary: Visuomotor Serial Targeting Task (VSTT)
 Author-email: Liam Keegan <ssc@iwr.uni-heidelberg.de>
 License: MIT
 Project-URL: Github, https://github.com/ssciwr/vstt
 Project-URL: Issues, https://github.com/ssciwr/vstt/issues
 Project-URL: Documentation, https://vstt.readthedocs.io/
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `vstt-0.27.0/src/vstt.egg-info/SOURCES.txt` & `vstt-0.28.0/src/vstt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vstt-0.27.0/tests/test_display.py` & `vstt-0.28.0/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `vstt-0.27.0/tests/test_display_widget.py` & `vstt-0.28.0/tests/test_display_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.27.0/tests/test_experiment.py` & `vstt-0.28.0/tests/test_experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,21 +227,17 @@
             elif i_target == -1:
                 dest = "center"
             else:
                 dest = None
             if dest is not None:
                 # target data from target display time
                 # get correct timestamps
-                ts = stats[f"to_{dest}_timestamps"][i_row]
-                # exclude any negative times from before target display
-                ts_correct = ts[ts >= 0]
+                ts_correct = stats[f"to_{dest}_timestamps"][i_row]
                 # get imported timestamps
                 ts = df_target.timestamps.to_numpy()
-                # subtract first timepoint to reset any offset to zero
-                ts = ts - ts[0]
                 assert np.allclose(ts, ts_correct)
                 # get correct mouse positions
                 xys = stats[f"to_{dest}_mouse_positions"][i_row]
                 n = xys.shape[0]
                 if dest == "target" or (dest == "center" and n > 0):
                     assert np.allclose(
                         df_target["mouse_positions_x"].to_numpy(), xys[:, 0]
```

### Comparing `vstt-0.27.0/tests/test_geom.py` & `vstt-0.28.0/tests/test_geom.py`

 * *Files identical despite different names*

### Comparing `vstt-0.27.0/tests/test_gui.py` & `vstt-0.28.0/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `vstt-0.27.0/tests/test_joystick_wrapper.py` & `vstt-0.28.0/tests/test_joystick_wrapper.py`

 * *Files identical despite different names*

### Comparing `vstt-0.27.0/tests/test_meta.py` & `vstt-0.28.0/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `vstt-0.27.0/tests/test_meta_widget.py` & `vstt-0.28.0/tests/test_meta_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.27.0/tests/test_results_widget.py` & `vstt-0.28.0/tests/test_results_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.27.0/tests/test_stat.py` & `vstt-0.28.0/tests/test_stat.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,20 +71,23 @@
         [-1.0, -0.5],
         [0.0, 2.0, 4.0, 6.0],
         [-0.9, -0.7, -0.5, -0.3, -0.1, 0.1, 0.3, 0.5],
         [0.0, 0.1, 0.2, 0.3, 0.4, 0.5, 0.7, 1.0, 1.1, 1.2],
     ]:
         n = len(times)
         for n_zeros in range(1, n):
-            positions = [[-1e-13, 1e-14]] * n_zeros + [[1, 1]] * (n - n_zeros)
-            reaction_time = times[n_zeros]
-            assert np.allclose(
-                vstt.stat._reaction_time(np.array(times), np.array(positions)),
-                [reaction_time],
-            )
+            for n_before_visible in range(1, n):
+                positions = [[-1e-13, 1e-14]] * n_zeros + [[1, 1]] * (n - n_zeros)
+                reaction_time = times[n_zeros] - times[n_before_visible]
+                assert np.allclose(
+                    vstt.stat._reaction_time(
+                        np.array(times), np.array(positions), n_before_visible
+                    ),
+                    [reaction_time],
+                )
 
 
 def test_rmse() -> None:
     target = np.array([1, 1])
     # all points lie on the straight line between start and end point
     assert np.allclose(vstt.stat._rmse(np.array([(0, 0), (1, 1)]), target), [0])
     assert np.allclose(vstt.stat._rmse(np.array([(0, 0), (0.2, 0.2)]), target), [0])
```

### Comparing `vstt-0.27.0/tests/test_task.py` & `vstt-0.28.0/tests/test_task.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 import threading
 from time import sleep
+from typing import Dict
 from typing import List
 from typing import Tuple
 
 import gui_test_utils as gtu
 import numpy as np
 import pyautogui
+import pytest
 import vstt
 from psychopy.visual.window import Window
 from vstt.experiment import Experiment
 from vstt.geom import points_on_circle
 from vstt.task import MotorTask
 
 
@@ -70,22 +72,31 @@
     success = task.run()
     do_task_thread.join()
     assert success is False
     assert experiment_no_trials.has_unsaved_changes is False
     assert experiment_no_trials.trial_handler_with_results is None
 
 
-def test_task_automove_to_center(
-    experiment_no_results: Experiment, window: Window
+@pytest.mark.parametrize(
+    "trial_settings",
+    [
+        {"automove_cursor_to_center": True},
+        {"add_central_target": False, "automove_cursor_to_center": False, "weight": 1},
+    ],
+    ids=["automove_to_center", "no_central_target"],
+)
+def test_task(
+    experiment_no_results: Experiment, window: Window, trial_settings: Dict
 ) -> None:
     target_pixels = []
     experiment_no_results.has_unsaved_changes = False
     assert experiment_no_results.trial_handler_with_results is None
     for trial in experiment_no_results.trial_list:
-        trial["automove_cursor_to_center"] = True
+        for key, value in trial_settings.items():
+            trial[key] = value  # type: ignore
         target_pixels.append(
             [
                 gtu.pos_to_pixels(pos)
                 for pos in points_on_circle(
                     trial["num_targets"],
                     trial["target_distance"],
                     include_centre=False,
@@ -96,60 +107,23 @@
     task = MotorTask(experiment_no_results, window)
     success = task.run()
     do_task_thread.join()
     # task ran successfully, updated experiment with results
     assert success is True
     assert experiment_no_results.has_unsaved_changes is True
     assert experiment_no_results.trial_handler_with_results is not None
+    data = experiment_no_results.trial_handler_with_results.data
     # check that we hit all the targets without timing out
-    for timestamps in experiment_no_results.trial_handler_with_results.data[
-        "to_target_timestamps"
-    ][0][0]:
+    for timestamps in data["to_target_timestamps"][0][0]:
         assert (
-            timestamps[-1]
-            < 0.5 * experiment_no_results.trial_list[0]["target_duration"]
-        )
-
-
-def test_task_no_central_target(
-    experiment_no_results: Experiment, window: Window
-) -> None:
-    target_pixels = []
-    experiment_no_results.has_unsaved_changes = False
-    assert experiment_no_results.trial_handler_with_results is None
-    for trial in experiment_no_results.trial_list:
-        trial["add_central_target"] = False
-        trial["automove_cursor_to_center"] = False
-        trial["weight"] = 1
-        target_pixels.append(
-            [
-                gtu.pos_to_pixels(pos)
-                for pos in points_on_circle(
-                    trial["num_targets"],
-                    trial["target_distance"],
-                    include_centre=False,
-                )
-            ]
-        )
-    do_task_thread = launch_do_task(experiment_no_results, target_pixels)
-    task = MotorTask(experiment_no_results, window)
-    success = task.run()
-    do_task_thread.join()
-    # task ran successfully, updated experiment with results
-    assert success is True
-    assert experiment_no_results.has_unsaved_changes is True
-    assert experiment_no_results.trial_handler_with_results is not None
-    # check that we hit all the targets without timing out
-    for timestamps in experiment_no_results.trial_handler_with_results.data[
-        "to_target_timestamps"
-    ][0][0]:
-        assert (
-            timestamps[-1]
+            timestamps[-1] - timestamps[0]
             < 0.5 * experiment_no_results.trial_list[0]["target_duration"]
         )
+    for dest in ["target", "center"]:
+        assert np.all(data[f"to_{dest}_success"][0][0])
 
 
 def test_task_no_automove_to_center(
     experiment_no_results: Experiment, window: Window
 ) -> None:
     experiment_no_results.has_unsaved_changes = False
     assert experiment_no_results.trial_handler_with_results is None
@@ -171,30 +145,29 @@
     success = task.run()
     do_task_thread.join()
     # task ran successfully, updated experiment with results
     assert success is True
     assert experiment_no_results.has_unsaved_changes is True
     assert experiment_no_results.trial_handler_with_results is not None
     # check that we hit all the targets
+    data = experiment_no_results.trial_handler_with_results.data
     for to_target_timestamps, to_center_timestamps in zip(
-        experiment_no_results.trial_handler_with_results.data["to_target_timestamps"][
-            0
-        ][0],
-        experiment_no_results.trial_handler_with_results.data["to_center_timestamps"][
-            0
-        ][0],
+        data["to_target_timestamps"][0][0],
+        data["to_center_timestamps"][0][0],
     ):
         assert (
-            to_target_timestamps[-1]
+            to_target_timestamps[-1] - to_target_timestamps[0]
             < 0.5 * experiment_no_results.trial_list[0]["target_duration"]
         )
         assert (
-            to_center_timestamps[-1]
+            to_center_timestamps[-1] - to_target_timestamps[0]
             < 0.5 * experiment_no_results.trial_list[0]["target_duration"]
         )
+    for dest in ["target", "center"]:
+        assert np.all(data[f"to_{dest}_success"][0][0])
 
 
 def test_task_fixed_intervals_no_user_input(window: Window) -> None:
     experiment = Experiment()
     experiment.metadata["display_duration"] = 0.0
     target_duration = 1.0
     trial = vstt.trial.default_trial()
@@ -213,24 +186,23 @@
     # run task without moving mouse, which will stay in center for entire experiment
     assert task.run() is True
     # task ran successfully, updated experiment with results
     assert experiment.has_unsaved_changes is True
     assert experiment.trial_handler_with_results is not None
     # check that we failed to hit all targets
     expected_success = np.full((trial["num_targets"],), False)
+    data = experiment.trial_handler_with_results.data
     for success_name in ["to_target_success", "to_center_success"]:
-        assert np.all(
-            experiment.trial_handler_with_results.data[success_name][0][0]
-            == expected_success
-        )
-    # first to_target timestamps should start at approx -target_duration,
-    # at 0 the first target is displayed for target_duration secs, so it should end at approx target_duration
-    # subsequent ones should start at approx 0.0 since previous target is not reached, and end at approx target_duration
-    all_to_target_timestamps = experiment.trial_handler_with_results.data[
-        "to_target_timestamps"
-    ][0][0]
-    delta = 0.05 * target_duration
-    assert abs(all_to_target_timestamps[0][0] + target_duration) < delta
-    assert abs(all_to_target_timestamps[0][-1] - target_duration) < delta
-    for to_target_timestamps in all_to_target_timestamps[1:]:
-        assert abs(to_target_timestamps[0]) < delta
-        assert abs(to_target_timestamps[-1] - target_duration) < delta
+        assert np.all(data[success_name][0][0] == expected_success)
+    # first to_target timestamps should start at ~0,
+    # at ~target_duration the first target is displayed for target_duration secs,
+    # subsequent ones should be displayed every ~target_duration starting from ~2*target_duration
+    all_to_target_timestamps = data["to_target_timestamps"][0][0]
+    # require timestamps to be accurate within 0.1s
+    # On CI the fps / dropped frames can be erratic so this is a conservative value.
+    # If running on real hardware these should actually be within 2/fps
+    delta = 0.1
+    assert abs(all_to_target_timestamps[0][0]) < delta
+    assert abs(all_to_target_timestamps[0][-1] - 2 * target_duration) < delta
+    for count, to_target_timestamps in enumerate(all_to_target_timestamps[1:]):
+        assert abs(to_target_timestamps[0] - (count + 2) * target_duration) < delta
+        assert abs(to_target_timestamps[-1] - (count + 3) * target_duration) < delta
```

### Comparing `vstt-0.27.0/tests/test_trial.py` & `vstt-0.28.0/tests/test_trial.py`

 * *Files identical despite different names*

### Comparing `vstt-0.27.0/tests/test_trials_widget.py` & `vstt-0.28.0/tests/test_trials_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.27.0/tests/test_update.py` & `vstt-0.28.0/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `vstt-0.27.0/tests/test_vis.py` & `vstt-0.28.0/tests/test_vis.py`

 * *Files identical despite different names*

