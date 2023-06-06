# Comparing `tmp/rtc-tools-2.5.2a4.tar.gz` & `tmp/rtc-tools-2.5.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtc-tools-2.5.2a4.tar", last modified: Tue May 30 10:06:46 2023, max compression
+gzip compressed data, was "rtc-tools-2.5.2rc2.tar", last modified: Tue Jun  6 08:39:48 2023, max compression
```

## Comparing `rtc-tools-2.5.2a4.tar` & `rtc-tools-2.5.2rc2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 10:06:46.452332 rtc-tools-2.5.2a4/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/COPYING.LESSER
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1184 2023-05-30 10:06:46.452332 rtc-tools-2.5.2a4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      750 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/README.md
--rw-rw-rw-   0 root         (0) root         (0)      388 2023-05-30 10:06:46.453332 rtc-tools-2.5.2a4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2016 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 10:06:46.442332 rtc-tools-2.5.2a4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 10:06:46.444332 rtc-tools-2.5.2a4/src/rtc_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1184 2023-05-30 10:06:46.000000 rtc-tools-2.5.2a4/src/rtc_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2071 2023-05-30 10:06:46.000000 rtc-tools-2.5.2a4/src/rtc_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 10:06:46.000000 rtc-tools-2.5.2a4/src/rtc_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      151 2023-05-30 10:06:46.000000 rtc-tools-2.5.2a4/src/rtc_tools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      130 2023-05-30 10:06:46.000000 rtc-tools-2.5.2a4/src/rtc_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-30 10:06:46.000000 rtc-tools-2.5.2a4/src/rtc_tools.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 10:06:46.453332 rtc-tools-2.5.2a4/src/rtctools/
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 10:06:46.446332 rtc-tools-2.5.2a4/src/rtctools/_internal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/_internal/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5336 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/_internal/alias_tools.py
--rw-rw-rw-   0 root         (0) root         (0)      903 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/_internal/caching.py
--rw-rw-rw-   0 root         (0) root         (0)     2243 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/_internal/casadi_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     1084 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/_internal/debug_check_helpers.py
--rw-r--r--   0 root         (0) root         (0)      499 2023-05-30 10:06:46.453332 rtc-tools-2.5.2a4/src/rtctools/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 10:06:46.447332 rtc-tools-2.5.2a4/src/rtctools/data/
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4947 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/data/csv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 10:06:46.448332 rtc-tools-2.5.2a4/src/rtctools/data/interpolation/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/data/interpolation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      958 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/data/interpolation/bspline.py
--rw-rw-rw-   0 root         (0) root         (0)     5985 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/data/interpolation/bspline1d.py
--rw-rw-rw-   0 root         (0) root         (0)     1607 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/data/interpolation/bspline2d.py
--rw-rw-rw-   0 root         (0) root         (0)    18692 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/data/netcdf.py
--rw-rw-rw-   0 root         (0) root         (0)    43530 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/data/pi.py
--rw-rw-rw-   0 root         (0) root         (0)     8853 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/data/rtc.py
--rw-rw-rw-   0 root         (0) root         (0)    13011 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/data/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 10:06:46.451332 rtc-tools-2.5.2a4/src/rtctools/optimization/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   117456 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/collocated_integrated_optimization_problem.py
--rw-rw-rw-   0 root         (0) root         (0)     9026 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/control_tree_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    16651 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/csv_lookup_table_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    11624 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/csv_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    31608 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/goal_programming_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    41999 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/goal_programming_mixin_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6782 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/homotopy_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     3126 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/initial_state_estimation_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    12558 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/io_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1019 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/linearization_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     8736 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/linearized_order_goal_programming_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    13293 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/min_abs_goal_programming_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    16198 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/modelica_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     7259 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/netcdf_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    43494 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/optimization_problem.py
--rw-rw-rw-   0 root         (0) root         (0)    10783 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/pi_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    25126 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/single_pass_goal_programming_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1753 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/timeseries.py
--rw-rw-rw-   0 root         (0) root         (0)     4193 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/rtctoolsapp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 10:06:46.452332 rtc-tools-2.5.2a4/src/rtctools/simulation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/simulation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6606 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/simulation/csv_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     6163 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/simulation/io_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     8922 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/simulation/pi_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    35341 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/simulation/simulation_problem.py
--rw-rw-rw-   0 root         (0) root         (0)     8905 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/util.py
--rw-rw-rw-   0 root         (0) root         (0)    68611 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:39:48.261309 rtc-tools-2.5.2rc2/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/COPYING.LESSER
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-06-06 08:39:48.261309 rtc-tools-2.5.2rc2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      750 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      388 2023-06-06 08:39:48.262308 rtc-tools-2.5.2rc2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2016 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:39:48.248309 rtc-tools-2.5.2rc2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:39:48.251309 rtc-tools-2.5.2rc2/src/rtc_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-06-06 08:39:48.000000 rtc-tools-2.5.2rc2/src/rtc_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2071 2023-06-06 08:39:48.000000 rtc-tools-2.5.2rc2/src/rtc_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 08:39:48.000000 rtc-tools-2.5.2rc2/src/rtc_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      151 2023-06-06 08:39:48.000000 rtc-tools-2.5.2rc2/src/rtc_tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2023-06-06 08:39:48.000000 rtc-tools-2.5.2rc2/src/rtc_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-06 08:39:48.000000 rtc-tools-2.5.2rc2/src/rtc_tools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:39:48.262308 rtc-tools-2.5.2rc2/src/rtctools/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:39:48.253309 rtc-tools-2.5.2rc2/src/rtctools/_internal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/_internal/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5336 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/_internal/alias_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      903 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/_internal/caching.py
+-rw-rw-rw-   0 root         (0) root         (0)     2243 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/_internal/casadi_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/_internal/debug_check_helpers.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-06-06 08:39:48.262308 rtc-tools-2.5.2rc2/src/rtctools/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:39:48.255308 rtc-tools-2.5.2rc2/src/rtctools/data/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4947 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/data/csv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:39:48.255308 rtc-tools-2.5.2rc2/src/rtctools/data/interpolation/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/data/interpolation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      958 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/data/interpolation/bspline.py
+-rw-rw-rw-   0 root         (0) root         (0)     5985 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/data/interpolation/bspline1d.py
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/data/interpolation/bspline2d.py
+-rw-rw-rw-   0 root         (0) root         (0)    18692 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/data/netcdf.py
+-rw-rw-rw-   0 root         (0) root         (0)    43530 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/data/pi.py
+-rw-rw-rw-   0 root         (0) root         (0)     8853 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/data/rtc.py
+-rw-rw-rw-   0 root         (0) root         (0)    13011 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/data/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:39:48.260309 rtc-tools-2.5.2rc2/src/rtctools/optimization/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   117456 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/collocated_integrated_optimization_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)     9026 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/control_tree_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    16651 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/csv_lookup_table_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    11624 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/csv_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    31608 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/goal_programming_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    41999 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/goal_programming_mixin_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6782 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/homotopy_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3126 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/initial_state_estimation_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    12558 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/io_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/linearization_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     8736 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/linearized_order_goal_programming_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    13293 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/min_abs_goal_programming_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    16198 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/modelica_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     7259 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/netcdf_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    43494 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/optimization_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)    10783 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/pi_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    25126 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/single_pass_goal_programming_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1753 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/timeseries.py
+-rw-rw-rw-   0 root         (0) root         (0)     4193 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/rtctoolsapp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:39:48.261309 rtc-tools-2.5.2rc2/src/rtctools/simulation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/simulation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6606 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/simulation/csv_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     6163 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/simulation/io_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     8922 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/simulation/pi_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    35419 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/simulation/simulation_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)     8905 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/util.py
+-rw-rw-rw-   0 root         (0) root         (0)    68611 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/versioneer.py
```

### Comparing `rtc-tools-2.5.2a4/COPYING.LESSER` & `rtc-tools-2.5.2rc2/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/PKG-INFO` & `rtc-tools-2.5.2rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtc-tools
-Version: 2.5.2a4
+Version: 2.5.2rc2
 Summary: Toolbox for control and optimization of water systems.
 Home-page: https://oss.deltares.nl/web/rtc-tools/home
 Author: Deltares
 Maintainer: Deltares
 License: UNKNOWN
 Download-URL: http://gitlab.com/deltares/rtc-tools/
 Platform: Windows
```

### Comparing `rtc-tools-2.5.2a4/README.md` & `rtc-tools-2.5.2rc2/README.md`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/setup.py` & `rtc-tools-2.5.2rc2/setup.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtc_tools.egg-info/PKG-INFO` & `rtc-tools-2.5.2rc2/src/rtc_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtc-tools
-Version: 2.5.2a4
+Version: 2.5.2rc2
 Summary: Toolbox for control and optimization of water systems.
 Home-page: https://oss.deltares.nl/web/rtc-tools/home
 Author: Deltares
 Maintainer: Deltares
 License: UNKNOWN
 Download-URL: http://gitlab.com/deltares/rtc-tools/
 Platform: Windows
```

### Comparing `rtc-tools-2.5.2a4/src/rtc_tools.egg-info/SOURCES.txt` & `rtc-tools-2.5.2rc2/src/rtc_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/_internal/alias_tools.py` & `rtc-tools-2.5.2rc2/src/rtctools/_internal/alias_tools.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/_internal/caching.py` & `rtc-tools-2.5.2rc2/src/rtctools/_internal/caching.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/_internal/casadi_helpers.py` & `rtc-tools-2.5.2rc2/src/rtctools/_internal/casadi_helpers.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/_internal/debug_check_helpers.py` & `rtc-tools-2.5.2rc2/src/rtctools/_internal/debug_check_helpers.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/data/csv.py` & `rtc-tools-2.5.2rc2/src/rtctools/data/csv.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/data/interpolation/bspline.py` & `rtc-tools-2.5.2rc2/src/rtctools/data/interpolation/bspline.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/data/interpolation/bspline1d.py` & `rtc-tools-2.5.2rc2/src/rtctools/data/interpolation/bspline1d.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/data/interpolation/bspline2d.py` & `rtc-tools-2.5.2rc2/src/rtctools/data/interpolation/bspline2d.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/data/netcdf.py` & `rtc-tools-2.5.2rc2/src/rtctools/data/netcdf.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/data/pi.py` & `rtc-tools-2.5.2rc2/src/rtctools/data/pi.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/data/rtc.py` & `rtc-tools-2.5.2rc2/src/rtctools/data/rtc.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/data/storage.py` & `rtc-tools-2.5.2rc2/src/rtctools/data/storage.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/optimization/collocated_integrated_optimization_problem.py` & `rtc-tools-2.5.2rc2/src/rtctools/optimization/collocated_integrated_optimization_problem.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/optimization/control_tree_mixin.py` & `rtc-tools-2.5.2rc2/src/rtctools/optimization/control_tree_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/optimization/csv_lookup_table_mixin.py` & `rtc-tools-2.5.2rc2/src/rtctools/optimization/csv_lookup_table_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/optimization/csv_mixin.py` & `rtc-tools-2.5.2rc2/src/rtctools/optimization/csv_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/optimization/goal_programming_mixin.py` & `rtc-tools-2.5.2rc2/src/rtctools/optimization/goal_programming_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/optimization/goal_programming_mixin_base.py` & `rtc-tools-2.5.2rc2/src/rtctools/optimization/goal_programming_mixin_base.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/optimization/homotopy_mixin.py` & `rtc-tools-2.5.2rc2/src/rtctools/optimization/homotopy_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/optimization/initial_state_estimation_mixin.py` & `rtc-tools-2.5.2rc2/src/rtctools/optimization/initial_state_estimation_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/optimization/io_mixin.py` & `rtc-tools-2.5.2rc2/src/rtctools/optimization/io_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/optimization/linearization_mixin.py` & `rtc-tools-2.5.2rc2/src/rtctools/optimization/linearization_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/optimization/linearized_order_goal_programming_mixin.py` & `rtc-tools-2.5.2rc2/src/rtctools/optimization/linearized_order_goal_programming_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/optimization/min_abs_goal_programming_mixin.py` & `rtc-tools-2.5.2rc2/src/rtctools/optimization/min_abs_goal_programming_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/optimization/modelica_mixin.py` & `rtc-tools-2.5.2rc2/src/rtctools/optimization/modelica_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/optimization/netcdf_mixin.py` & `rtc-tools-2.5.2rc2/src/rtctools/optimization/netcdf_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/optimization/optimization_problem.py` & `rtc-tools-2.5.2rc2/src/rtctools/optimization/optimization_problem.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/optimization/pi_mixin.py` & `rtc-tools-2.5.2rc2/src/rtctools/optimization/pi_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/optimization/single_pass_goal_programming_mixin.py` & `rtc-tools-2.5.2rc2/src/rtctools/optimization/single_pass_goal_programming_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/optimization/timeseries.py` & `rtc-tools-2.5.2rc2/src/rtctools/optimization/timeseries.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/rtctoolsapp.py` & `rtc-tools-2.5.2rc2/src/rtctools/rtctoolsapp.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/simulation/csv_mixin.py` & `rtc-tools-2.5.2rc2/src/rtctools/simulation/csv_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/simulation/io_mixin.py` & `rtc-tools-2.5.2rc2/src/rtctools/simulation/io_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/simulation/pi_mixin.py` & `rtc-tools-2.5.2rc2/src/rtctools/simulation/pi_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/src/rtctools/simulation/simulation_problem.py` & `rtc-tools-2.5.2rc2/src/rtctools/simulation/simulation_problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -521,17 +521,20 @@
             next_state = self.__do_step(guess, dt, self.__state_vector[:-len(self.__mx['parameters'])])
         else:
             next_state = self.__do_step(guess, dt, self.__state_vector)
         # Check convergence of rootfinder
         rootfinder_stats = self.__do_step.stats()
 
         if not rootfinder_stats['success']:
-            logger.warning(
-                'Simulation has failed to converge at time {}. Solver failed with status {}'.format(
-                    self.get_current_time(), rootfinder_stats['nlpsol']['return_status']))
+            message = (
+                'Simulation has failed to converge at time {}. '
+                'Solver failed with status {}'
+            ).format(self.get_current_time(), rootfinder_stats['nlpsol']['return_status'])
+            logger.error(message)
+            raise Exception(message)
 
         if logger.getEffectiveLevel() == logging.DEBUG:
             # compute max residual
             largest_res = ca.norm_inf(
                 self.__res_vals(next_state, self.__dt, self.__state_vector[:-len(self.__mx['parameters'])])
             )
             logger.debug('Residual maximum magnitude: {:.2E}'.format(float(largest_res)))
```

### Comparing `rtc-tools-2.5.2a4/src/rtctools/util.py` & `rtc-tools-2.5.2rc2/src/rtctools/util.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a4/versioneer.py` & `rtc-tools-2.5.2rc2/versioneer.py`

 * *Files identical despite different names*

