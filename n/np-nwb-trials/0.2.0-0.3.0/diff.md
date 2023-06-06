# Comparing `tmp/np-nwb-trials-0.2.0.tar.gz` & `tmp/np-nwb-trials-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np-nwb-trials-0.2.0.tar", last modified: Mon Jun  5 23:57:28 2023, max compression
+gzip compressed data, was "np-nwb-trials-0.3.0.tar", last modified: Tue Jun  6 00:22:17 2023, max compression
```

## Comparing `np-nwb-trials-0.2.0.tar` & `np-nwb-trials-0.3.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0      190 2023-06-05 21:25:42.037220 np-nwb-trials-0.2.0/README.md
--rw-r--r--   0        0        0      483 2023-06-05 23:57:03.994132 np-nwb-trials-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 20:36:46.780149 np-nwb-trials-0.2.0/src/np_nwb_trials/__init__.py
--rw-r--r--   0        0        0     1677 2023-06-05 20:35:33.066291 np-nwb-trials-0.2.0/src/np_nwb_trials/nwb/__init__.py
--rw-r--r--   0        0        0      800 2023-06-03 23:13:42.700639 np-nwb-trials-0.2.0/src/np_nwb_trials/nwb/utils.py
--rw-r--r--   0        0        0    22997 2023-06-05 19:34:21.689765 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/DR_processing_script.py
--rw-r--r--   0        0        0    34647 2023-06-05 21:47:53.331424 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/DR_processing_utils.py
--rw-r--r--   0        0        0    10878 2023-06-05 21:46:47.046178 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/__init__.py
--rw-r--r--   0        0        0    12405 2023-06-04 01:10:52.103930 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/ecephys.py
--rw-r--r--   0        0        0    14024 2023-06-05 23:53:30.085854 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/probeSync.py
--rw-r--r--   0        0        0       52 2023-06-04 01:10:51.537675 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/MANIFEST.in
--rw-r--r--   0        0        0     2304 2023-06-04 01:10:51.540561 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/README.md
--rw-r--r--   0        0        0       30 2023-06-04 01:10:51.542660 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/requirements.txt
--rw-r--r--   0        0        0      198 2023-06-04 01:10:51.544484 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/requirements_acq.txt
--rw-r--r--   0        0        0       37 2023-06-04 01:10:51.546799 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/requirements_dev.txt
--rw-r--r--   0        0        0      692 2023-06-04 01:10:51.549208 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/setup.py
--rw-r--r--   0        0        0      221 2023-06-04 01:10:51.552837 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/__init__.py
--rw-r--r--   0        0        0    22374 2023-06-04 01:10:51.567544 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/dataset.py
--rw-r--r--   0        0        0      243 2023-06-04 01:10:51.570313 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/gui/README.md
--rw-r--r--   0        0        0       62 2023-06-04 01:10:51.572597 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/gui/__init__.py
--rw-r--r--   0        0        0      343 2023-06-04 01:10:51.574249 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/gui/res/checkbox.png
--rw-r--r--   0        0        0    10929 2023-06-04 01:10:51.575474 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/gui/res/darkorange_stylesheet.css
--rw-r--r--   0        0        0     1008 2023-06-04 01:10:51.576642 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/gui/res/down_arrow.png
--rw-r--r--   0        0        0     2837 2023-06-04 01:10:51.578160 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/gui/res/handle.png
--rw-r--r--   0        0        0   142112 2023-06-04 01:10:51.580860 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/gui/res/record.png
--rw-r--r--   0        0        0    29169 2023-06-04 01:10:51.582549 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/gui/res/stop.png
--rw-r--r--   0        0        0   370070 2023-06-04 01:10:51.586200 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/gui/res/visualizer.ico
--rw-r--r--   0        0        0    23284 2023-06-04 01:10:51.587954 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/gui/res/visualizer.png
--rw-r--r--   0        0        0    31493 2023-06-04 01:10:51.589621 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/gui/sync_gui.py
--rw-r--r--   0        0        0    12593 2023-06-04 01:10:51.590954 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/gui/sync_gui.ui
--rw-r--r--   0        0        0     3040 2023-06-04 01:10:51.592157 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/gui/visualizer.py
--rw-r--r--   0        0        0        0 2023-06-04 01:10:51.594102 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/ni/__init__.py
--rw-r--r--   0        0        0    31637 2023-06-04 01:10:51.599009 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/ni/daq.py
--rw-r--r--   0        0        0     7116 2023-06-04 01:10:51.600138 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/sync.py
--rw-r--r--   0        0        0     9079 2023-06-04 01:10:51.602002 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/tango/sync_device.py
--rw-r--r--   0        0        0        0 2023-06-04 01:10:51.603379 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/utils/__init__.py
--rw-r--r--   0        0        0     4068 2023-06-04 01:10:51.604379 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/utils/h5.py
--rw-r--r--   0        0        0     1872 2023-06-04 01:10:51.605362 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/utils/recover.py
--rw-r--r--   0        0        0      403 2023-06-04 01:10:51.606425 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/utils/sample.py
--rw-r--r--   0        0        0        0 2023-06-04 01:10:51.607746 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/zro/__init__.py
--rw-r--r--   0        0        0     1709 2023-06-04 01:10:51.608766 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/zro/gui_interface.py
--rw-r--r--   0        0        0     5898 2023-06-04 01:10:51.610298 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/zro/sync_device.py
--rw-r--r--   0        0        0      277 2023-06-04 01:10:51.611833 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync.egg-info/PKG-INFO
--rw-r--r--   0        0        0      713 2023-06-04 01:10:51.613022 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2023-06-04 01:10:51.613967 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       93 2023-06-04 01:10:51.614948 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync.egg-info/entry_points.txt
--rw-r--r--   0        0        0        5 2023-06-04 01:10:51.615718 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync.egg-info/top_level.txt
--rw-r--r--   0        0        0     3551 2023-06-04 01:10:51.621231 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/tests/test_dataset.py
--rw-r--r--   0        0        0     1395 2023-06-04 01:10:51.622324 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/tests/test_sync.py
--rw-r--r--   0        0        0      362 2023-06-04 01:10:51.623092 np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/tox.ini
--rw-r--r--   0        0        0      404 2023-06-05 21:52:45.358502 np-nwb-trials-0.2.0/src/np_nwb_trials/schemas.py
--rw-r--r--   0        0        0      759 2023-06-05 22:53:32.607596 np-nwb-trials-0.2.0/tests/test_nwb.py
--rw-r--r--   0        0        0      383 1970-01-01 00:00:00.000000 np-nwb-trials-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      190 2023-06-05 21:25:42.037220 np-nwb-trials-0.3.0/README.md
+-rw-r--r--   0        0        0      507 2023-06-06 00:21:13.574767 np-nwb-trials-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-05 20:36:46.780149 np-nwb-trials-0.3.0/src/np_nwb_trials/__init__.py
+-rw-r--r--   0        0        0     1677 2023-06-05 20:35:33.066291 np-nwb-trials-0.3.0/src/np_nwb_trials/nwb/__init__.py
+-rw-r--r--   0        0        0      800 2023-06-03 23:13:42.700639 np-nwb-trials-0.3.0/src/np_nwb_trials/nwb/utils.py
+-rw-r--r--   0        0        0    22997 2023-06-05 19:34:21.689765 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/DR_processing_script.py
+-rw-r--r--   0        0        0    34647 2023-06-05 21:47:53.331424 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/DR_processing_utils.py
+-rw-r--r--   0        0        0    10878 2023-06-05 21:46:47.046178 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/__init__.py
+-rw-r--r--   0        0        0    12405 2023-06-04 01:10:52.103930 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/ecephys.py
+-rw-r--r--   0        0        0    14024 2023-06-05 23:53:30.085854 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/probeSync.py
+-rw-r--r--   0        0        0       52 2023-06-04 01:10:51.537675 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/MANIFEST.in
+-rw-r--r--   0        0        0     2304 2023-06-04 01:10:51.540561 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/README.md
+-rw-r--r--   0        0        0       30 2023-06-04 01:10:51.542660 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/requirements.txt
+-rw-r--r--   0        0        0      198 2023-06-04 01:10:51.544484 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/requirements_acq.txt
+-rw-r--r--   0        0        0       37 2023-06-04 01:10:51.546799 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/requirements_dev.txt
+-rw-r--r--   0        0        0      692 2023-06-04 01:10:51.549208 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/setup.py
+-rw-r--r--   0        0        0      221 2023-06-04 01:10:51.552837 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/__init__.py
+-rw-r--r--   0        0        0    22374 2023-06-04 01:10:51.567544 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/dataset.py
+-rw-r--r--   0        0        0      243 2023-06-04 01:10:51.570313 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/gui/README.md
+-rw-r--r--   0        0        0       62 2023-06-04 01:10:51.572597 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/gui/__init__.py
+-rw-r--r--   0        0        0      343 2023-06-04 01:10:51.574249 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/gui/res/checkbox.png
+-rw-r--r--   0        0        0    10929 2023-06-04 01:10:51.575474 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/gui/res/darkorange_stylesheet.css
+-rw-r--r--   0        0        0     1008 2023-06-04 01:10:51.576642 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/gui/res/down_arrow.png
+-rw-r--r--   0        0        0     2837 2023-06-04 01:10:51.578160 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/gui/res/handle.png
+-rw-r--r--   0        0        0   142112 2023-06-04 01:10:51.580860 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/gui/res/record.png
+-rw-r--r--   0        0        0    29169 2023-06-04 01:10:51.582549 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/gui/res/stop.png
+-rw-r--r--   0        0        0   370070 2023-06-04 01:10:51.586200 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/gui/res/visualizer.ico
+-rw-r--r--   0        0        0    23284 2023-06-04 01:10:51.587954 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/gui/res/visualizer.png
+-rw-r--r--   0        0        0    31493 2023-06-04 01:10:51.589621 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/gui/sync_gui.py
+-rw-r--r--   0        0        0    12593 2023-06-04 01:10:51.590954 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/gui/sync_gui.ui
+-rw-r--r--   0        0        0     3040 2023-06-04 01:10:51.592157 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/gui/visualizer.py
+-rw-r--r--   0        0        0        0 2023-06-04 01:10:51.594102 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/ni/__init__.py
+-rw-r--r--   0        0        0    31637 2023-06-04 01:10:51.599009 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/ni/daq.py
+-rw-r--r--   0        0        0     7116 2023-06-04 01:10:51.600138 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/sync.py
+-rw-r--r--   0        0        0     9079 2023-06-04 01:10:51.602002 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/tango/sync_device.py
+-rw-r--r--   0        0        0        0 2023-06-04 01:10:51.603379 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/utils/__init__.py
+-rw-r--r--   0        0        0     4068 2023-06-04 01:10:51.604379 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/utils/h5.py
+-rw-r--r--   0        0        0     1872 2023-06-04 01:10:51.605362 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/utils/recover.py
+-rw-r--r--   0        0        0      403 2023-06-04 01:10:51.606425 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/utils/sample.py
+-rw-r--r--   0        0        0        0 2023-06-04 01:10:51.607746 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/zro/__init__.py
+-rw-r--r--   0        0        0     1709 2023-06-04 01:10:51.608766 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/zro/gui_interface.py
+-rw-r--r--   0        0        0     5898 2023-06-04 01:10:51.610298 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/zro/sync_device.py
+-rw-r--r--   0        0        0      277 2023-06-04 01:10:51.611833 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      713 2023-06-04 01:10:51.613022 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2023-06-04 01:10:51.613967 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       93 2023-06-04 01:10:51.614948 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync.egg-info/entry_points.txt
+-rw-r--r--   0        0        0        5 2023-06-04 01:10:51.615718 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync.egg-info/top_level.txt
+-rw-r--r--   0        0        0     3551 2023-06-04 01:10:51.621231 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/tests/test_dataset.py
+-rw-r--r--   0        0        0     1395 2023-06-04 01:10:51.622324 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/tests/test_sync.py
+-rw-r--r--   0        0        0      362 2023-06-04 01:10:51.623092 np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/tox.ini
+-rw-r--r--   0        0        0      404 2023-06-05 21:52:45.358502 np-nwb-trials-0.3.0/src/np_nwb_trials/schemas.py
+-rw-r--r--   0        0        0      759 2023-06-05 22:53:32.607596 np-nwb-trials-0.3.0/tests/test_nwb.py
+-rw-r--r--   0        0        0      383 1970-01-01 00:00:00.000000 np-nwb-trials-0.3.0/PKG-INFO
```

### Comparing `np-nwb-trials-0.2.0/src/np_nwb_trials/nwb/__init__.py` & `np-nwb-trials-0.3.0/src/np_nwb_trials/nwb/__init__.py`

 * *Files identical despite different names*

### Comparing `np-nwb-trials-0.2.0/src/np_nwb_trials/nwb/utils.py` & `np-nwb-trials-0.3.0/src/np_nwb_trials/nwb/utils.py`

 * *Files identical despite different names*

### Comparing `np-nwb-trials-0.2.0/src/np_nwb_trials/processing/DR_processing_script.py` & `np-nwb-trials-0.3.0/src/np_nwb_trials/processing/DR_processing_script.py`

 * *Files identical despite different names*

### Comparing `np-nwb-trials-0.2.0/src/np_nwb_trials/processing/DR_processing_utils.py` & `np-nwb-trials-0.3.0/src/np_nwb_trials/processing/DR_processing_utils.py`

 * *Files identical despite different names*

### Comparing `np-nwb-trials-0.2.0/src/np_nwb_trials/processing/__init__.py` & `np-nwb-trials-0.3.0/src/np_nwb_trials/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `np-nwb-trials-0.2.0/src/np_nwb_trials/processing/ecephys.py` & `np-nwb-trials-0.3.0/src/np_nwb_trials/processing/ecephys.py`

 * *Files identical despite different names*

### Comparing `np-nwb-trials-0.2.0/src/np_nwb_trials/processing/probeSync.py` & `np-nwb-trials-0.3.0/src/np_nwb_trials/processing/probeSync.py`

 * *Files identical despite different names*

### Comparing `np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/README.md` & `np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/README.md`

 * *Files identical despite different names*

### Comparing `np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/setup.py` & `np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/setup.py`

 * *Files identical despite different names*

### Comparing `np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/dataset.py` & `np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/dataset.py`

 * *Files identical despite different names*

### Comparing `np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/gui/res/darkorange_stylesheet.css` & `np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/gui/res/darkorange_stylesheet.css`

 * *Files identical despite different names*

### Comparing `np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/gui/res/down_arrow.png` & `np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/gui/res/down_arrow.png`

 * *Files identical despite different names*

### Comparing `np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/gui/res/handle.png` & `np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/gui/res/handle.png`

 * *Files identical despite different names*

### Comparing `np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/gui/res/record.png` & `np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/gui/res/record.png`

 * *Files identical despite different names*

### Comparing `np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/gui/res/stop.png` & `np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/gui/res/stop.png`

 * *Files identical despite different names*

### Comparing `np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/gui/res/visualizer.ico` & `np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/gui/res/visualizer.ico`

 * *Files identical despite different names*

### Comparing `np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/gui/res/visualizer.png` & `np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/gui/res/visualizer.png`

 * *Files identical despite different names*

### Comparing `np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/gui/sync_gui.py` & `np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/gui/sync_gui.py`

 * *Files identical despite different names*

### Comparing `np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/gui/sync_gui.ui` & `np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/gui/sync_gui.ui`

 * *Files identical despite different names*

### Comparing `np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/gui/visualizer.py` & `np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/gui/visualizer.py`

 * *Files identical despite different names*

### Comparing `np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/ni/daq.py` & `np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/ni/daq.py`

 * *Files identical despite different names*

### Comparing `np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/sync.py` & `np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/sync.py`

 * *Files identical despite different names*

### Comparing `np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/tango/sync_device.py` & `np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/tango/sync_device.py`

 * *Files identical despite different names*

### Comparing `np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/utils/h5.py` & `np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/utils/h5.py`

 * *Files identical despite different names*

### Comparing `np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/utils/recover.py` & `np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/utils/recover.py`

 * *Files identical despite different names*

### Comparing `np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/zro/gui_interface.py` & `np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/zro/gui_interface.py`

 * *Files identical despite different names*

### Comparing `np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync/zro/sync_device.py` & `np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync/zro/sync_device.py`

 * *Files identical despite different names*

### Comparing `np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/sync.egg-info/SOURCES.txt` & `np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/tests/test_dataset.py` & `np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `np-nwb-trials-0.2.0/src/np_nwb_trials/processing/sync/tests/test_sync.py` & `np-nwb-trials-0.3.0/src/np_nwb_trials/processing/sync/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `np-nwb-trials-0.2.0/tests/test_nwb.py` & `np-nwb-trials-0.3.0/tests/test_nwb.py`

 * *Files identical despite different names*

